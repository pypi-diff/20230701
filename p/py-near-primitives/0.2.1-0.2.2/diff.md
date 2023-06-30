# Comparing `tmp/py_near_primitives-0.2.1.tar.gz` & `tmp/py_near_primitives-0.2.2.tar.gz`

## Comparing `py_near_primitives-0.2.1.tar` & `py_near_primitives-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 py_near_primitives-0.2.1/Cargo.toml
--rw-r--r--   0     1001      123    11357 2023-06-30 22:14:36.000000 py_near_primitives-0.2.1/LICENSE
--rw-r--r--   0     1001      123      730 2023-06-30 22:14:36.000000 py_near_primitives-0.2.1/README.md
--rw-r--r--   0     1001      123     1195 2023-06-30 22:14:36.000000 py_near_primitives-0.2.1/pyproject.toml
--rw-r--r--   0     1001      123    18657 2023-06-30 22:14:36.000000 py_near_primitives-0.2.1/src/lib.rs
--rw-r--r--   0     1001      123    69198 2023-06-30 22:15:02.000000 py_near_primitives-0.2.1/Cargo.lock
--rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 py_near_primitives-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 py_near_primitives-0.2.2/Cargo.toml
+-rw-r--r--   0     1001      123    11357 2023-06-30 22:32:39.000000 py_near_primitives-0.2.2/LICENSE
+-rw-r--r--   0     1001      123      730 2023-06-30 22:32:39.000000 py_near_primitives-0.2.2/README.md
+-rw-r--r--   0     1001      123     1195 2023-06-30 22:32:39.000000 py_near_primitives-0.2.2/pyproject.toml
+-rw-r--r--   0     1001      123    18886 2023-06-30 22:32:39.000000 py_near_primitives-0.2.2/src/lib.rs
+-rw-r--r--   0     1001      123    69198 2023-06-30 22:33:02.000000 py_near_primitives-0.2.2/Cargo.lock
+-rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 py_near_primitives-0.2.2/PKG-INFO
```

### Comparing `py_near_primitives-0.2.1/Cargo.toml` & `py_near_primitives-0.2.2/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "py_near_primitives"
-version = "0.2.1"
+version = "0.2.2"
 edition = "2021"
 include = ["/src", "/LICENSE", "/pyproject.toml"]
 description = "Python bindings for NEAR Rust primitives."
 license = "MIT"
 repository = "https://github.com/kevinheavey/pyonear"
 
 [lib]
```

### Comparing `py_near_primitives-0.2.1/LICENSE` & `py_near_primitives-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_near_primitives-0.2.1/README.md` & `py_near_primitives-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `py_near_primitives-0.2.1/pyproject.toml` & `py_near_primitives-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py_near_primitives"
-version = "0.2.1"
+version = "0.2.2"
 description = "Python bindings for NEAR Rust primitives."
 authors = ["pvolnov <notanemail@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
@@ -21,15 +21,15 @@
 [build-system]
 requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 
 [project]
 name = "py_near_primitives"
-version = "0.2.1"
+version = "0.2.2"
 description = "Python bindings for NEAR Rust primitives."
 authors = [ {name = "pvolnov", email = "notanemail@gmail.com"} ]
 license = {file = "LICENSE"} # relative to the package/ directory
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `py_near_primitives-0.2.1/src/lib.rs` & `py_near_primitives-0.2.2/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -330,29 +330,37 @@
             nonce: self.nonce,
             max_block_height: self.max_block_height,
             public_key: pk,
         };
         return *action.get_nep461_hash().as_bytes();
     }
 
-    fn serialize(&self) -> Vec<u8> {
+
+    #[pyo3(text_signature = "() -> bytes")]
+    fn serialize(&self) -> PyResult<Py<PyBytes>> {
         let pk = PublicKey::ED25519(ED25519PublicKey(self.public_key));
         let action = DelegateActionOriginal {
             sender_id: AccountId::from_str(self.sender_id.as_str()).unwrap(),
             receiver_id: AccountId::from_str(self.receiver_id.as_str()).unwrap(),
             actions: get_delegate_actions(self.clone()),
             nonce: self.nonce,
             max_block_height: self.max_block_height,
             public_key: pk,
         };
-        return action.try_to_vec().unwrap().to_vec();
+        let res = action.try_to_vec().unwrap().to_vec();
+
+        let py = unsafe { Python::assume_gil_acquired() };
+        let pybytes = PyBytes::new(py, &res);
+
+        Ok(pybytes.into())
     }
 
 
     #[staticmethod]
+    #[pyo3(signature = (bytes))]
     fn bytes_to_json(mut bytes: &[u8]) -> String {
         let bytes_mut: &mut &[u8] = &mut bytes;
         let action: DelegateActionOriginal = near_primitives::borsh::BorshDeserialize::deserialize(bytes_mut).unwrap();
         return serde_json::to_string(&action).unwrap();
     }
 }
```

### Comparing `py_near_primitives-0.2.1/Cargo.lock` & `py_near_primitives-0.2.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1584,15 +1584,15 @@
 checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "py_near_primitives"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
  "borsh 0.9.3",
  "derive_more",
  "ed25519-dalek",
  "near-crypto",
  "near-primitives",
  "near-primitives-core",
```

### Comparing `py_near_primitives-0.2.1/PKG-INFO` & `py_near_primitives-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_near_primitives
-Version: 0.2.1
+Version: 0.2.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Python bindings for NEAR Rust primitives.
 Author-email: pvolnov <notanemail@gmail.com>
 License: MIT
```

