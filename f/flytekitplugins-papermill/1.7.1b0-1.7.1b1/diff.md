# Comparing `tmp/flytekitplugins-papermill-1.7.1b0.tar.gz` & `tmp/flytekitplugins-papermill-1.7.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-papermill-1.7.1b0.tar", last modified: Fri Jun 16 18:14:25 2023, max compression
+gzip compressed data, was "flytekitplugins-papermill-1.7.1b1.tar", last modified: Tue Jun 27 22:00:59 2023, max compression
```

## Comparing `flytekitplugins-papermill-1.7.1b0.tar` & `flytekitplugins-papermill-1.7.1b1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:25.930387 flytekitplugins-papermill-1.7.1b0/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-16 18:14:25.930387 flytekitplugins-papermill-1.7.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-16 18:13:54.000000 flytekitplugins-papermill-1.7.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:25.930387 flytekitplugins-papermill-1.7.1b0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:25.930387 flytekitplugins-papermill-1.7.1b0/flytekitplugins/papermill/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-16 18:13:54.000000 flytekitplugins-papermill-1.7.1b0/flytekitplugins/papermill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15569 2023-06-16 18:13:54.000000 flytekitplugins-papermill-1.7.1b0/flytekitplugins/papermill/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:25.930387 flytekitplugins-papermill-1.7.1b0/flytekitplugins_papermill.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-16 18:14:25.000000 flytekitplugins-papermill-1.7.1b0/flytekitplugins_papermill.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-16 18:14:25.000000 flytekitplugins-papermill-1.7.1b0/flytekitplugins_papermill.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 18:14:25.000000 flytekitplugins-papermill-1.7.1b0/flytekitplugins_papermill.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 18:14:25.000000 flytekitplugins-papermill-1.7.1b0/flytekitplugins_papermill.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-16 18:14:25.000000 flytekitplugins-papermill-1.7.1b0/flytekitplugins_papermill.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 18:14:25.000000 flytekitplugins-papermill-1.7.1b0/flytekitplugins_papermill.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 18:14:25.930387 flytekitplugins-papermill-1.7.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-16 18:14:14.000000 flytekitplugins-papermill-1.7.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:59.420739 flytekitplugins-papermill-1.7.1b1/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-27 22:00:59.420739 flytekitplugins-papermill-1.7.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-27 22:00:35.000000 flytekitplugins-papermill-1.7.1b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:59.420739 flytekitplugins-papermill-1.7.1b1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:59.420739 flytekitplugins-papermill-1.7.1b1/flytekitplugins/papermill/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-27 22:00:35.000000 flytekitplugins-papermill-1.7.1b1/flytekitplugins/papermill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15569 2023-06-27 22:00:35.000000 flytekitplugins-papermill-1.7.1b1/flytekitplugins/papermill/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:59.420739 flytekitplugins-papermill-1.7.1b1/flytekitplugins_papermill.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-27 22:00:59.000000 flytekitplugins-papermill-1.7.1b1/flytekitplugins_papermill.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-27 22:00:59.000000 flytekitplugins-papermill-1.7.1b1/flytekitplugins_papermill.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 22:00:59.000000 flytekitplugins-papermill-1.7.1b1/flytekitplugins_papermill.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 22:00:59.000000 flytekitplugins-papermill-1.7.1b1/flytekitplugins_papermill.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-27 22:00:59.000000 flytekitplugins-papermill-1.7.1b1/flytekitplugins_papermill.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 22:00:59.000000 flytekitplugins-papermill-1.7.1b1/flytekitplugins_papermill.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 22:00:59.420739 flytekitplugins-papermill-1.7.1b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-27 22:00:50.000000 flytekitplugins-papermill-1.7.1b1/setup.py
```

### Comparing `flytekitplugins-papermill-1.7.1b0/PKG-INFO` & `flytekitplugins-papermill-1.7.1b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-papermill
-Version: 1.7.1b0
+Version: 1.7.1b1
 Summary: This is the flytekit papermill plugin
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-papermill-1.7.1b0/README.md` & `flytekitplugins-papermill-1.7.1b1/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-papermill-1.7.1b0/flytekitplugins/papermill/task.py` & `flytekitplugins-papermill-1.7.1b1/flytekitplugins/papermill/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-papermill-1.7.1b0/flytekitplugins_papermill.egg-info/PKG-INFO` & `flytekitplugins-papermill-1.7.1b1/flytekitplugins_papermill.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-papermill
-Version: 1.7.1b0
+Version: 1.7.1b1
 Summary: This is the flytekit papermill plugin
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-papermill-1.7.1b0/setup.py` & `flytekitplugins-papermill-1.7.1b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 plugin_requires = [
     "flytekit",
     "papermill>=1.2.0",
     "nbconvert>=6.0.7",
     "ipykernel>=5.0.0",
 ]
 
-__version__ = "1.7.1b0"
+__version__ = "1.7.1b1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This is the flytekit papermill plugin",
```

