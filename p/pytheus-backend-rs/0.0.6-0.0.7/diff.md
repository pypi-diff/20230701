# Comparing `tmp/pytheus_backend_rs-0.0.6.tar.gz` & `tmp/pytheus_backend_rs-0.0.7.tar.gz`

## Comparing `pytheus_backend_rs-0.0.6.tar` & `pytheus_backend_rs-0.0.7.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0      370 1970-01-01 00:00:00.000000 pytheus_backend_rs-0.0.6/Cargo.toml
--rw-r--r--   0     1001      123     2792 2023-06-27 00:50:17.000000 pytheus_backend_rs-0.0.6/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-06-27 00:50:17.000000 pytheus_backend_rs-0.0.6/.gitignore
--rw-r--r--   0     1001      123      620 2023-06-27 00:50:17.000000 pytheus_backend_rs-0.0.6/pyproject.toml
--rw-r--r--   0     1001      123    13415 2023-06-27 00:50:17.000000 pytheus_backend_rs-0.0.6/src/lib.rs
--rw-r--r--   0     1001      123    13468 2023-06-27 00:50:17.000000 pytheus_backend_rs-0.0.6/Cargo.lock
--rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 pytheus_backend_rs-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 pytheus_backend_rs-0.0.7/Cargo.toml
+-rw-r--r--   0     1001      123     2792 2023-06-30 23:27:45.000000 pytheus_backend_rs-0.0.7/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-06-30 23:27:45.000000 pytheus_backend_rs-0.0.7/.gitignore
+-rw-r--r--   0     1001      123    11357 2023-06-30 23:27:45.000000 pytheus_backend_rs-0.0.7/LICENSE
+-rw-r--r--   0     1001      123      620 2023-06-30 23:27:45.000000 pytheus_backend_rs-0.0.7/pyproject.toml
+-rw-r--r--   0     1001      123    14381 2023-06-30 23:27:45.000000 pytheus_backend_rs-0.0.7/src/lib.rs
+-rw-r--r--   0     1001      123        0 2023-06-30 23:27:45.000000 pytheus_backend_rs-0.0.7/tests/__init__.py
+-rw-r--r--   0     1001      123     5615 2023-06-30 23:27:45.000000 pytheus_backend_rs-0.0.7/tests/test_redis.py
+-rw-r--r--   0     1001      123    13922 2023-06-30 23:27:45.000000 pytheus_backend_rs-0.0.7/Cargo.lock
+-rw-r--r--   0        0        0      530 1970-01-01 00:00:00.000000 pytheus_backend_rs-0.0.7/PKG-INFO
```

### Comparing `pytheus_backend_rs-0.0.6/.github/workflows/CI.yml` & `pytheus_backend_rs-0.0.7/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pytheus_backend_rs-0.0.6/.gitignore` & `pytheus_backend_rs-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pytheus_backend_rs-0.0.6/pyproject.toml` & `pytheus_backend_rs-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytheus_backend_rs-0.0.6/src/lib.rs` & `pytheus_backend_rs-0.0.7/src/lib.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 use crossbeam::channel;
 use itertools::Itertools;
+use log::{error, info};
 use pyo3::exceptions::PyException;
 use pyo3::intern;
 use pyo3::prelude::*;
 use pyo3::types::{PyDict, PyType};
 use redis::ConnectionLike;
 use std::collections::HashMap;
 use std::sync::{mpsc, Mutex, OnceLock};
@@ -18,15 +19,15 @@
     Inc,
     Dec,
     Set,
 }
 
 #[derive(Debug)]
 struct RedisPipelineJobResult {
-    values: Vec<f64>,
+    values: Result<Vec<f64>, PyErr>,
 }
 
 struct RedisJob {
     action: BackendAction,
     key_name: String,
     labels_hash: Option<String>,
     value: f64,
@@ -43,15 +44,17 @@
     #[pyo3(get)]
     config: Py<PyDict>,
     #[pyo3(get)]
     metric: Py<PyAny>,
     #[pyo3(get)]
     histogram_bucket: Option<String>,
     redis_job_tx: mpsc::Sender<RedisJob>,
+    #[pyo3(get)]
     key_name: String,
+    #[pyo3(get)]
     labels_hash: Option<String>,
 }
 
 // Sample(suffix='_bucket', labels={'le': '0.005'}, value=0.0
 #[derive(Debug, FromPyObject)]
 struct Sample<'a> {
     suffix: String,
@@ -138,14 +141,52 @@
                 None => pipe.set(&received.key_name, received.value).ignore(),
             };
             pipe.expire(&received.key_name, EXPIRE_KEY_SECONDS).ignore();
         }
     }
 }
 
+fn handle_generate_metrics_job(
+    pipeline: redis::Pipeline,
+    connection: &mut r2d2::PooledConnection<redis::Client>,
+    pool: &r2d2::Pool<redis::Client>,
+) -> Result<Vec<f64>, Box<dyn std::error::Error>> {
+    if !connection.is_open() {
+        *connection = pool.get()?
+    }
+
+    let results: Vec<Option<f64>> = pipeline.query(connection)?;
+    let values = results.into_iter().map(|val| val.unwrap_or(0f64)).collect();
+
+    Ok(values)
+}
+
+fn handle_backend_action_job(
+    received: RedisJob,
+    connection: &mut r2d2::PooledConnection<redis::Client>,
+    pool: &r2d2::Pool<redis::Client>,
+    rx: &mpsc::Receiver<RedisJob>,
+) -> Result<(), Box<dyn std::error::Error>> {
+    if !connection.is_open() {
+        *connection = pool.get()?;
+    }
+
+    let mut pipe = redis::pipe();
+
+    add_job_to_pipeline(received, &mut pipe);
+
+    for received in rx.try_iter() {
+        add_job_to_pipeline(received, &mut pipe);
+    }
+
+    pipe.query::<()>(connection)?;
+
+    Ok(())
+}
+
 #[pymethods]
 impl RedisBackend {
     #[new]
     fn new(config: &PyDict, metric: &PyAny, histogram_bucket: Option<String>) -> PyResult<Self> {
         // producer
         let redis_job_tx_mutex = REDIS_JOB_TX.get().unwrap();
         let redis_job_tx = redis_job_tx_mutex.lock().unwrap();
@@ -224,55 +265,40 @@
 
         let (pipeline_tx, pipeline_rx) = crossbeam::channel::unbounded();
         REDIS_PIPELINE_JOB_TX.get_or_init(|| Mutex::new(pipeline_tx));
 
         for i in 0..4 {
             let cloned_pipeline_rx = pipeline_rx.clone();
             let pool = pool.clone();
+            info!("Starting pipeline thread....{i}");
             thread::spawn(move || {
-                println!("Starting pipeline thread....{i}");
+                // the first connection happens at startup so we let it panic
                 let mut connection = pool.get().unwrap();
                 while let Ok(received) = cloned_pipeline_rx.recv() {
-                    if !connection.is_open() {
-                        connection = pool.get().unwrap();
-                    }
-
-                    let pipe = received.pipeline;
-                    let results: Vec<Option<f64>> = pipe.query(&mut connection).unwrap();
-
-                    let values = results.into_iter().map(|val| val.unwrap_or(0f64)).collect();
-
-                    received
-                        .result_tx
-                        .send(RedisPipelineJobResult { values })
-                        .unwrap();
+                    let values =
+                        handle_generate_metrics_job(received.pipeline, &mut connection, &pool);
+                    let values = values.map_err(|e| PyException::new_err(e.to_string()));
+
+                    // NOTE: might want to log the failure
+                    let _ = received.result_tx.send(RedisPipelineJobResult { values });
                 }
             });
         }
 
-        thread::spawn(move || {
-            println!("Starting BackendAction thread....");
+        info!("Starting BackendAction thread....");
+        thread::spawn(move || loop {
+            // the first connection happens at startup so we let it panic
             let mut connection = pool.get().unwrap();
             while let Ok(received) = rx.recv() {
-                if !connection.is_open() {
-                    connection = pool.get().unwrap();
-                }
-
-                let mut pipe = redis::pipe();
-
-                add_job_to_pipeline(received, &mut pipe);
-
-                for received in rx.try_iter() {
-                    add_job_to_pipeline(received, &mut pipe);
-                }
-
-                let _: () = pipe.query(&mut connection).unwrap();
+                handle_backend_action_job(received, &mut connection, &pool, &rx)
+                    .unwrap_or_else(|e| error!("{}", e.to_string()));
             }
         });
 
+        info!("RedisBackend initialized");
         Ok(())
     }
 
     #[classmethod]
     fn _generate_samples(cls: &PyType, registry: &PyAny) -> PyResult<PyObject> {
         let py = cls.py();
         let collectors = registry.call_method0(intern!(py, "collect"))?;
@@ -338,51 +364,51 @@
 
         // map back the values from redis into the appropriate Sample
         let mut samples_vec_united = vec![];
         for samples_vec in &mut samples_result_dict.samples_vec {
             samples_vec_united.extend(samples_vec);
         }
 
-        for (sample, value) in samples_vec_united.iter_mut().zip(job_result.values) {
+        for (sample, value) in samples_vec_united.iter_mut().zip(job_result.values?) {
             sample.value = value
         }
         samples_result_dict.into_py(py)
     }
 
     fn inc(&self, value: f64) {
         self.redis_job_tx
             .send(RedisJob {
                 action: BackendAction::Inc,
                 key_name: self.key_name.clone(),
                 labels_hash: self.labels_hash.clone(), // I wonder if only the String inside should be cloned into a new Some
                 value,
             })
-            .unwrap();
+            .unwrap_or_else(|_| error!("`inc` operation failed"));
     }
 
     fn dec(&self, value: f64) {
         self.redis_job_tx
             .send(RedisJob {
                 action: BackendAction::Dec,
                 key_name: self.key_name.clone(),
                 labels_hash: self.labels_hash.clone(),
                 value: -value,
             })
-            .unwrap();
+            .unwrap_or_else(|_| error!("`dec` operation failed"));
     }
 
     fn set(&self, value: f64) {
         self.redis_job_tx
             .send(RedisJob {
                 action: BackendAction::Set,
                 key_name: self.key_name.clone(),
                 labels_hash: self.labels_hash.clone(),
                 value,
             })
-            .unwrap();
+            .unwrap_or_else(|_| error!("`set` operation failed"));
     }
 
     fn get(self_: PyRef<Self>) -> PyRef<'_, RedisBackend> {
         // This returns itself so that we have a RedisBackend instance to retrieve key_name and
         // labels_hash to query redis when collecting samples via a pipeline.
         self_
     }
@@ -431,12 +457,14 @@
         *data
     }
 }
 
 /// A Python module implemented in Rust.
 #[pymodule]
 fn pytheus_backend_rs(_py: Python, m: &PyModule) -> PyResult<()> {
+    pyo3_log::init();
+
     m.add_class::<RedisBackend>()?;
     m.add_class::<SingleProcessBackend>()?;
     m.add_class::<OutSample>()?;
     Ok(())
 }
```

### Comparing `pytheus_backend_rs-0.0.6/Cargo.lock` & `pytheus_backend_rs-0.0.7/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
+name = "arc-swap"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bddcadddf5e9015d310179a59bb28c4d4b9920ad0f11e8e14dbadf654890c9a6"
+
+[[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "bitflags"
@@ -264,14 +270,25 @@
 checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
+name = "pyo3-log"
+version = "0.8.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c94ff6535a6bae58d7d0b85e60d4c53f7f84d0d0aa35d6a28c3f3e70bfe51444"
+dependencies = [
+ "arc-swap",
+ "log",
+ "pyo3",
+]
+
+[[package]]
 name = "pyo3-macros"
 version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
@@ -288,19 +305,21 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pytheus-backend-rs"
-version = "0.0.6"
+version = "0.0.7"
 dependencies = [
  "crossbeam",
  "itertools",
+ "log",
  "pyo3",
+ "pyo3-log",
  "r2d2",
  "redis",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.28"
```

