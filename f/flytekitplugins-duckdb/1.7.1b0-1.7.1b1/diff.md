# Comparing `tmp/flytekitplugins-duckdb-1.7.1b0.tar.gz` & `tmp/flytekitplugins-duckdb-1.7.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-duckdb-1.7.1b0.tar", last modified: Fri Jun 16 18:14:19 2023, max compression
+gzip compressed data, was "flytekitplugins-duckdb-1.7.1b1.tar", last modified: Tue Jun 27 22:00:54 2023, max compression
```

## Comparing `flytekitplugins-duckdb-1.7.1b0.tar` & `flytekitplugins-duckdb-1.7.1b1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:19.214440 flytekitplugins-duckdb-1.7.1b0/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-16 18:14:19.210440 flytekitplugins-duckdb-1.7.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-16 18:13:54.000000 flytekitplugins-duckdb-1.7.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:19.210440 flytekitplugins-duckdb-1.7.1b0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:19.210440 flytekitplugins-duckdb-1.7.1b0/flytekitplugins/duckdb/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-16 18:13:54.000000 flytekitplugins-duckdb-1.7.1b0/flytekitplugins/duckdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-06-16 18:13:54.000000 flytekitplugins-duckdb-1.7.1b0/flytekitplugins/duckdb/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:19.210440 flytekitplugins-duckdb-1.7.1b0/flytekitplugins_duckdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-16 18:14:19.000000 flytekitplugins-duckdb-1.7.1b0/flytekitplugins_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-16 18:14:19.000000 flytekitplugins-duckdb-1.7.1b0/flytekitplugins_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 18:14:19.000000 flytekitplugins-duckdb-1.7.1b0/flytekitplugins_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 18:14:19.000000 flytekitplugins-duckdb-1.7.1b0/flytekitplugins_duckdb.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 18:14:19.000000 flytekitplugins-duckdb-1.7.1b0/flytekitplugins_duckdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 18:14:19.000000 flytekitplugins-duckdb-1.7.1b0/flytekitplugins_duckdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 18:14:19.214440 flytekitplugins-duckdb-1.7.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-16 18:14:14.000000 flytekitplugins-duckdb-1.7.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:54.268633 flytekitplugins-duckdb-1.7.1b1/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-27 22:00:54.268633 flytekitplugins-duckdb-1.7.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-27 22:00:35.000000 flytekitplugins-duckdb-1.7.1b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:54.268633 flytekitplugins-duckdb-1.7.1b1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:54.268633 flytekitplugins-duckdb-1.7.1b1/flytekitplugins/duckdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-27 22:00:35.000000 flytekitplugins-duckdb-1.7.1b1/flytekitplugins/duckdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-06-27 22:00:35.000000 flytekitplugins-duckdb-1.7.1b1/flytekitplugins/duckdb/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:54.268633 flytekitplugins-duckdb-1.7.1b1/flytekitplugins_duckdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-27 22:00:54.000000 flytekitplugins-duckdb-1.7.1b1/flytekitplugins_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-27 22:00:54.000000 flytekitplugins-duckdb-1.7.1b1/flytekitplugins_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 22:00:54.000000 flytekitplugins-duckdb-1.7.1b1/flytekitplugins_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 22:00:54.000000 flytekitplugins-duckdb-1.7.1b1/flytekitplugins_duckdb.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-27 22:00:54.000000 flytekitplugins-duckdb-1.7.1b1/flytekitplugins_duckdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 22:00:54.000000 flytekitplugins-duckdb-1.7.1b1/flytekitplugins_duckdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 22:00:54.268633 flytekitplugins-duckdb-1.7.1b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-27 22:00:50.000000 flytekitplugins-duckdb-1.7.1b1/setup.py
```

### Comparing `flytekitplugins-duckdb-1.7.1b0/PKG-INFO` & `flytekitplugins-duckdb-1.7.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-duckdb
-Version: 1.7.1b0
+Version: 1.7.1b1
 Summary: DuckDB Plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-duckdb-1.7.1b0/flytekitplugins/duckdb/task.py` & `flytekitplugins-duckdb-1.7.1b1/flytekitplugins/duckdb/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-duckdb-1.7.1b0/flytekitplugins_duckdb.egg-info/PKG-INFO` & `flytekitplugins-duckdb-1.7.1b1/flytekitplugins_duckdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-duckdb
-Version: 1.7.1b0
+Version: 1.7.1b1
 Summary: DuckDB Plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-duckdb-1.7.1b0/setup.py` & `flytekitplugins-duckdb-1.7.1b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "duckdb"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "duckdb"]
 
-__version__ = "1.7.1b0"
+__version__ = "1.7.1b1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="DuckDB Plugin for Flytekit",
```

