# Comparing `tmp/flytekitplugins-kftensorflow-1.7.1b0.tar.gz` & `tmp/flytekitplugins-kftensorflow-1.7.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-kftensorflow-1.7.1b0.tar", last modified: Fri Jun 16 18:14:23 2023, max compression
+gzip compressed data, was "flytekitplugins-kftensorflow-1.7.1b1.tar", last modified: Tue Jun 27 22:00:57 2023, max compression
```

## Comparing `flytekitplugins-kftensorflow-1.7.1b0.tar` & `flytekitplugins-kftensorflow-1.7.1b1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:23.034402 flytekitplugins-kftensorflow-1.7.1b0/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-16 18:14:23.034402 flytekitplugins-kftensorflow-1.7.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-16 18:13:54.000000 flytekitplugins-kftensorflow-1.7.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:23.030402 flytekitplugins-kftensorflow-1.7.1b0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:23.030402 flytekitplugins-kftensorflow-1.7.1b0/flytekitplugins/kftensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-16 18:13:54.000000 flytekitplugins-kftensorflow-1.7.1b0/flytekitplugins/kftensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-06-16 18:13:54.000000 flytekitplugins-kftensorflow-1.7.1b0/flytekitplugins/kftensorflow/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:23.034402 flytekitplugins-kftensorflow-1.7.1b0/flytekitplugins_kftensorflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-16 18:14:22.000000 flytekitplugins-kftensorflow-1.7.1b0/flytekitplugins_kftensorflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-16 18:14:23.000000 flytekitplugins-kftensorflow-1.7.1b0/flytekitplugins_kftensorflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 18:14:22.000000 flytekitplugins-kftensorflow-1.7.1b0/flytekitplugins_kftensorflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 18:14:22.000000 flytekitplugins-kftensorflow-1.7.1b0/flytekitplugins_kftensorflow.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 18:14:22.000000 flytekitplugins-kftensorflow-1.7.1b0/flytekitplugins_kftensorflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 18:14:22.000000 flytekitplugins-kftensorflow-1.7.1b0/flytekitplugins_kftensorflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 18:14:23.034402 flytekitplugins-kftensorflow-1.7.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-16 18:14:14.000000 flytekitplugins-kftensorflow-1.7.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:57.220693 flytekitplugins-kftensorflow-1.7.1b1/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-27 22:00:57.220693 flytekitplugins-kftensorflow-1.7.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-27 22:00:35.000000 flytekitplugins-kftensorflow-1.7.1b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:57.220693 flytekitplugins-kftensorflow-1.7.1b1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:57.220693 flytekitplugins-kftensorflow-1.7.1b1/flytekitplugins/kftensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-27 22:00:35.000000 flytekitplugins-kftensorflow-1.7.1b1/flytekitplugins/kftensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-06-27 22:00:35.000000 flytekitplugins-kftensorflow-1.7.1b1/flytekitplugins/kftensorflow/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:57.220693 flytekitplugins-kftensorflow-1.7.1b1/flytekitplugins_kftensorflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-27 22:00:57.000000 flytekitplugins-kftensorflow-1.7.1b1/flytekitplugins_kftensorflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-27 22:00:57.000000 flytekitplugins-kftensorflow-1.7.1b1/flytekitplugins_kftensorflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 22:00:57.000000 flytekitplugins-kftensorflow-1.7.1b1/flytekitplugins_kftensorflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 22:00:57.000000 flytekitplugins-kftensorflow-1.7.1b1/flytekitplugins_kftensorflow.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 22:00:57.000000 flytekitplugins-kftensorflow-1.7.1b1/flytekitplugins_kftensorflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 22:00:57.000000 flytekitplugins-kftensorflow-1.7.1b1/flytekitplugins_kftensorflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 22:00:57.220693 flytekitplugins-kftensorflow-1.7.1b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-27 22:00:50.000000 flytekitplugins-kftensorflow-1.7.1b1/setup.py
```

### Comparing `flytekitplugins-kftensorflow-1.7.1b0/PKG-INFO` & `flytekitplugins-kftensorflow-1.7.1b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kftensorflow
-Version: 1.7.1b0
+Version: 1.7.1b1
 Summary: K8s based Tensorflow plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kftensorflow-1.7.1b0/README.md` & `flytekitplugins-kftensorflow-1.7.1b1/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-kftensorflow-1.7.1b0/flytekitplugins/kftensorflow/task.py` & `flytekitplugins-kftensorflow-1.7.1b1/flytekitplugins/kftensorflow/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-kftensorflow-1.7.1b0/flytekitplugins_kftensorflow.egg-info/PKG-INFO` & `flytekitplugins-kftensorflow-1.7.1b1/flytekitplugins_kftensorflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kftensorflow
-Version: 1.7.1b0
+Version: 1.7.1b1
 Summary: K8s based Tensorflow plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kftensorflow-1.7.1b0/setup.py` & `flytekitplugins-kftensorflow-1.7.1b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "kftensorflow"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.6.1"]
 
-__version__ = "1.7.1b0"
+__version__ = "1.7.1b1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="K8s based Tensorflow plugin for flytekit",
```

