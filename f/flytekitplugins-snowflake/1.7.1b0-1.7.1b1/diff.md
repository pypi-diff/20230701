# Comparing `tmp/flytekitplugins-snowflake-1.7.1b0.tar.gz` & `tmp/flytekitplugins-snowflake-1.7.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-snowflake-1.7.1b0.tar", last modified: Fri Jun 16 18:14:27 2023, max compression
+gzip compressed data, was "flytekitplugins-snowflake-1.7.1b1.tar", last modified: Tue Jun 27 22:01:00 2023, max compression
```

## Comparing `flytekitplugins-snowflake-1.7.1b0.tar` & `flytekitplugins-snowflake-1.7.1b1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:27.390380 flytekitplugins-snowflake-1.7.1b0/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-16 18:14:27.390380 flytekitplugins-snowflake-1.7.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-16 18:13:54.000000 flytekitplugins-snowflake-1.7.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:27.386380 flytekitplugins-snowflake-1.7.1b0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:27.386380 flytekitplugins-snowflake-1.7.1b0/flytekitplugins/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-16 18:13:54.000000 flytekitplugins-snowflake-1.7.1b0/flytekitplugins/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-16 18:13:54.000000 flytekitplugins-snowflake-1.7.1b0/flytekitplugins/snowflake/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:27.390380 flytekitplugins-snowflake-1.7.1b0/flytekitplugins_snowflake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-16 18:14:27.000000 flytekitplugins-snowflake-1.7.1b0/flytekitplugins_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-16 18:14:27.000000 flytekitplugins-snowflake-1.7.1b0/flytekitplugins_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 18:14:27.000000 flytekitplugins-snowflake-1.7.1b0/flytekitplugins_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 18:14:27.000000 flytekitplugins-snowflake-1.7.1b0/flytekitplugins_snowflake.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-16 18:14:27.000000 flytekitplugins-snowflake-1.7.1b0/flytekitplugins_snowflake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 18:14:27.000000 flytekitplugins-snowflake-1.7.1b0/flytekitplugins_snowflake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 18:14:27.390380 flytekitplugins-snowflake-1.7.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-16 18:14:14.000000 flytekitplugins-snowflake-1.7.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:01:00.512762 flytekitplugins-snowflake-1.7.1b1/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-27 22:01:00.512762 flytekitplugins-snowflake-1.7.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-27 22:00:35.000000 flytekitplugins-snowflake-1.7.1b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:01:00.512762 flytekitplugins-snowflake-1.7.1b1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:01:00.512762 flytekitplugins-snowflake-1.7.1b1/flytekitplugins/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-27 22:00:35.000000 flytekitplugins-snowflake-1.7.1b1/flytekitplugins/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-27 22:00:35.000000 flytekitplugins-snowflake-1.7.1b1/flytekitplugins/snowflake/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:01:00.512762 flytekitplugins-snowflake-1.7.1b1/flytekitplugins_snowflake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-27 22:01:00.000000 flytekitplugins-snowflake-1.7.1b1/flytekitplugins_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-27 22:01:00.000000 flytekitplugins-snowflake-1.7.1b1/flytekitplugins_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 22:01:00.000000 flytekitplugins-snowflake-1.7.1b1/flytekitplugins_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 22:01:00.000000 flytekitplugins-snowflake-1.7.1b1/flytekitplugins_snowflake.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-27 22:01:00.000000 flytekitplugins-snowflake-1.7.1b1/flytekitplugins_snowflake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 22:01:00.000000 flytekitplugins-snowflake-1.7.1b1/flytekitplugins_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 22:01:00.512762 flytekitplugins-snowflake-1.7.1b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-27 22:00:50.000000 flytekitplugins-snowflake-1.7.1b1/setup.py
```

### Comparing `flytekitplugins-snowflake-1.7.1b0/PKG-INFO` & `flytekitplugins-snowflake-1.7.1b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-snowflake
-Version: 1.7.1b0
+Version: 1.7.1b1
 Summary: This package holds the Snowflake plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-snowflake-1.7.1b0/README.md` & `flytekitplugins-snowflake-1.7.1b1/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-snowflake-1.7.1b0/flytekitplugins/snowflake/task.py` & `flytekitplugins-snowflake-1.7.1b1/flytekitplugins/snowflake/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-snowflake-1.7.1b0/flytekitplugins_snowflake.egg-info/PKG-INFO` & `flytekitplugins-snowflake-1.7.1b1/flytekitplugins_snowflake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-snowflake
-Version: 1.7.1b0
+Version: 1.7.1b1
 Summary: This package holds the Snowflake plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-snowflake-1.7.1b0/setup.py` & `flytekitplugins-snowflake-1.7.1b1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "snowflake"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0"]
 
-__version__ = "1.7.1b0"
+__version__ = "1.7.1b1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds the Snowflake plugins for flytekit",
```

