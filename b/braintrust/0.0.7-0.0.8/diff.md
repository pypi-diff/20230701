# Comparing `tmp/braintrust-0.0.7.tar.gz` & `tmp/braintrust-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braintrust-0.0.7.tar", last modified: Fri Jun 30 23:15:39 2023, max compression
+gzip compressed data, was "braintrust-0.0.8.tar", last modified: Fri Jun 30 23:32:32 2023, max compression
```

## Comparing `braintrust-0.0.7.tar` & `braintrust-0.0.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:15:39.478192 braintrust-0.0.7/
--rw-r--r--   0 ankur      (501) staff       (20)      483 2023-06-30 23:15:39.478017 braintrust-0.0.7/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)       49 2023-04-02 02:49:19.000000 braintrust-0.0.7/README.md
--rw-r--r--   0 ankur      (501) staff       (20)       38 2023-06-30 23:15:39.478246 braintrust-0.0.7/setup.cfg
--rw-r--r--   0 ankur      (501) staff       (20)     1640 2023-06-30 23:03:25.000000 braintrust-0.0.7/setup.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:15:39.473242 braintrust-0.0.7/src/
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:15:39.475991 braintrust-0.0.7/src/braintrust/
--rw-r--r--   0 ankur      (501) staff       (20)    35300 2023-06-30 23:03:25.000000 braintrust-0.0.7/src/braintrust/__init__.py
--rw-r--r--   0 ankur      (501) staff       (20)      427 2023-06-22 23:54:28.000000 braintrust-0.0.7/src/braintrust/aws.py
--rw-r--r--   0 ankur      (501) staff       (20)      171 2023-06-30 23:03:25.000000 braintrust-0.0.7/src/braintrust/cache.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:15:39.477049 braintrust-0.0.7/src/braintrust/cli/
--rw-r--r--   0 ankur      (501) staff       (20)        0 2023-06-22 23:54:28.000000 braintrust-0.0.7/src/braintrust/cli/__init__.py
--rw-r--r--   0 ankur      (501) staff       (20)     1406 2023-06-22 23:54:28.000000 braintrust-0.0.7/src/braintrust/cli/__main__.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:15:39.477754 braintrust-0.0.7/src/braintrust/cli/install/
--rw-r--r--   0 ankur      (501) staff       (20)      472 2023-06-22 23:54:28.000000 braintrust-0.0.7/src/braintrust/cli/install/__init__.py
--rw-r--r--   0 ankur      (501) staff       (20)     8207 2023-06-22 23:54:28.000000 braintrust-0.0.7/src/braintrust/cli/install/api.py
--rw-r--r--   0 ankur      (501) staff       (20)     6421 2023-06-22 23:54:28.000000 braintrust-0.0.7/src/braintrust/cli/install/redshift.py
--rw-r--r--   0 ankur      (501) staff       (20)      399 2023-06-30 23:03:25.000000 braintrust-0.0.7/src/braintrust/duckutil.py
--rw-r--r--   0 ankur      (501) staff       (20)     2878 2023-06-30 23:03:25.000000 braintrust-0.0.7/src/braintrust/gitutil.py
--rw-r--r--   0 ankur      (501) staff       (20)      811 2023-04-15 21:46:41.000000 braintrust-0.0.7/src/braintrust/oai.py
--rw-r--r--   0 ankur      (501) staff       (20)      307 2023-06-30 23:03:25.000000 braintrust-0.0.7/src/braintrust/util.py
--rw-r--r--   0 ankur      (501) staff       (20)       18 2023-06-30 23:15:16.000000 braintrust-0.0.7/src/braintrust/version.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:15:39.476824 braintrust-0.0.7/src/braintrust.egg-info/
--rw-r--r--   0 ankur      (501) staff       (20)      483 2023-06-30 23:15:39.000000 braintrust-0.0.7/src/braintrust.egg-info/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)      619 2023-06-30 23:15:39.000000 braintrust-0.0.7/src/braintrust.egg-info/SOURCES.txt
--rw-r--r--   0 ankur      (501) staff       (20)        1 2023-06-30 23:15:39.000000 braintrust-0.0.7/src/braintrust.egg-info/dependency_links.txt
--rw-r--r--   0 ankur      (501) staff       (20)       60 2023-06-30 23:15:39.000000 braintrust-0.0.7/src/braintrust.egg-info/entry_points.txt
--rw-r--r--   0 ankur      (501) staff       (20)      316 2023-06-30 23:15:39.000000 braintrust-0.0.7/src/braintrust.egg-info/requires.txt
--rw-r--r--   0 ankur      (501) staff       (20)       11 2023-06-30 23:15:39.000000 braintrust-0.0.7/src/braintrust.egg-info/top_level.txt
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:32:32.074586 braintrust-0.0.8/
+-rw-r--r--   0 ankur      (501) staff       (20)      483 2023-06-30 23:32:32.074450 braintrust-0.0.8/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)       49 2023-04-02 02:49:19.000000 braintrust-0.0.8/README.md
+-rw-r--r--   0 ankur      (501) staff       (20)       38 2023-06-30 23:32:32.074628 braintrust-0.0.8/setup.cfg
+-rw-r--r--   0 ankur      (501) staff       (20)     1640 2023-06-30 23:03:25.000000 braintrust-0.0.8/setup.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:32:32.070388 braintrust-0.0.8/src/
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:32:32.072667 braintrust-0.0.8/src/braintrust/
+-rw-r--r--   0 ankur      (501) staff       (20)    35426 2023-06-30 23:31:00.000000 braintrust-0.0.8/src/braintrust/__init__.py
+-rw-r--r--   0 ankur      (501) staff       (20)      427 2023-06-22 23:54:28.000000 braintrust-0.0.8/src/braintrust/aws.py
+-rw-r--r--   0 ankur      (501) staff       (20)      171 2023-06-30 23:03:25.000000 braintrust-0.0.8/src/braintrust/cache.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:32:32.073600 braintrust-0.0.8/src/braintrust/cli/
+-rw-r--r--   0 ankur      (501) staff       (20)        0 2023-06-22 23:54:28.000000 braintrust-0.0.8/src/braintrust/cli/__init__.py
+-rw-r--r--   0 ankur      (501) staff       (20)     1406 2023-06-22 23:54:28.000000 braintrust-0.0.8/src/braintrust/cli/__main__.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:32:32.074196 braintrust-0.0.8/src/braintrust/cli/install/
+-rw-r--r--   0 ankur      (501) staff       (20)      472 2023-06-22 23:54:28.000000 braintrust-0.0.8/src/braintrust/cli/install/__init__.py
+-rw-r--r--   0 ankur      (501) staff       (20)     8207 2023-06-22 23:54:28.000000 braintrust-0.0.8/src/braintrust/cli/install/api.py
+-rw-r--r--   0 ankur      (501) staff       (20)     6421 2023-06-22 23:54:28.000000 braintrust-0.0.8/src/braintrust/cli/install/redshift.py
+-rw-r--r--   0 ankur      (501) staff       (20)      399 2023-06-30 23:03:25.000000 braintrust-0.0.8/src/braintrust/duckutil.py
+-rw-r--r--   0 ankur      (501) staff       (20)     2878 2023-06-30 23:03:25.000000 braintrust-0.0.8/src/braintrust/gitutil.py
+-rw-r--r--   0 ankur      (501) staff       (20)      811 2023-04-15 21:46:41.000000 braintrust-0.0.8/src/braintrust/oai.py
+-rw-r--r--   0 ankur      (501) staff       (20)      307 2023-06-30 23:03:25.000000 braintrust-0.0.8/src/braintrust/util.py
+-rw-r--r--   0 ankur      (501) staff       (20)       18 2023-06-30 23:31:25.000000 braintrust-0.0.8/src/braintrust/version.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:32:32.073375 braintrust-0.0.8/src/braintrust.egg-info/
+-rw-r--r--   0 ankur      (501) staff       (20)      483 2023-06-30 23:32:32.000000 braintrust-0.0.8/src/braintrust.egg-info/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)      619 2023-06-30 23:32:32.000000 braintrust-0.0.8/src/braintrust.egg-info/SOURCES.txt
+-rw-r--r--   0 ankur      (501) staff       (20)        1 2023-06-30 23:32:32.000000 braintrust-0.0.8/src/braintrust.egg-info/dependency_links.txt
+-rw-r--r--   0 ankur      (501) staff       (20)       60 2023-06-30 23:32:32.000000 braintrust-0.0.8/src/braintrust.egg-info/entry_points.txt
+-rw-r--r--   0 ankur      (501) staff       (20)      316 2023-06-30 23:32:32.000000 braintrust-0.0.8/src/braintrust.egg-info/requires.txt
+-rw-r--r--   0 ankur      (501) staff       (20)       11 2023-06-30 23:32:32.000000 braintrust-0.0.8/src/braintrust.egg-info/top_level.txt
```

### Comparing `braintrust-0.0.7/setup.py` & `braintrust-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.7/src/braintrust/__init__.py` & `braintrust-0.0.8/src/braintrust/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,15 +307,21 @@
 
 def _ensure_experiment(experiment_id):
     experiment_path = EXPERIMENTS_PATH / f"{experiment_id}.parquet"
 
     if not experiment_path.exists():
         os.makedirs(EXPERIMENTS_PATH, exist_ok=True)
         conn = api_conn()
-        resp = conn.get("experiment", params={"experiment_id": experiment_id})
+        resp = conn.get(
+            "experiment",
+            params={"experiment_id": experiment_id},
+            headers={
+                "Accept": "application/octet-stream",
+            },
+        )
 
         with open(experiment_path, "wb") as f:
             f.write(resp.content)
 
     return experiment_path
```

### Comparing `braintrust-0.0.7/src/braintrust/cli/__main__.py` & `braintrust-0.0.8/src/braintrust/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.7/src/braintrust/cli/install/api.py` & `braintrust-0.0.8/src/braintrust/cli/install/api.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.7/src/braintrust/cli/install/redshift.py` & `braintrust-0.0.8/src/braintrust/cli/install/redshift.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.7/src/braintrust/gitutil.py` & `braintrust-0.0.8/src/braintrust/gitutil.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.7/src/braintrust/oai.py` & `braintrust-0.0.8/src/braintrust/oai.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.7/src/braintrust.egg-info/SOURCES.txt` & `braintrust-0.0.8/src/braintrust.egg-info/SOURCES.txt`

 * *Files identical despite different names*

