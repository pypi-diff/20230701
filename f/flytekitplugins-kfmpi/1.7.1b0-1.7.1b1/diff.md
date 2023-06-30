# Comparing `tmp/flytekitplugins-kfmpi-1.7.1b0.tar.gz` & `tmp/flytekitplugins-kfmpi-1.7.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-kfmpi-1.7.1b0.tar", last modified: Fri Jun 16 18:14:22 2023, max compression
+gzip compressed data, was "flytekitplugins-kfmpi-1.7.1b1.tar", last modified: Tue Jun 27 22:00:56 2023, max compression
```

## Comparing `flytekitplugins-kfmpi-1.7.1b0.tar` & `flytekitplugins-kfmpi-1.7.1b1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:22.082412 flytekitplugins-kfmpi-1.7.1b0/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-16 18:14:22.078412 flytekitplugins-kfmpi-1.7.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-16 18:13:54.000000 flytekitplugins-kfmpi-1.7.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:22.078412 flytekitplugins-kfmpi-1.7.1b0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:22.078412 flytekitplugins-kfmpi-1.7.1b0/flytekitplugins/kfmpi/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-16 18:13:54.000000 flytekitplugins-kfmpi-1.7.1b0/flytekitplugins/kfmpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-06-16 18:13:54.000000 flytekitplugins-kfmpi-1.7.1b0/flytekitplugins/kfmpi/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:22.078412 flytekitplugins-kfmpi-1.7.1b0/flytekitplugins_kfmpi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-16 18:14:22.000000 flytekitplugins-kfmpi-1.7.1b0/flytekitplugins_kfmpi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-16 18:14:22.000000 flytekitplugins-kfmpi-1.7.1b0/flytekitplugins_kfmpi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 18:14:22.000000 flytekitplugins-kfmpi-1.7.1b0/flytekitplugins_kfmpi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 18:14:22.000000 flytekitplugins-kfmpi-1.7.1b0/flytekitplugins_kfmpi.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-16 18:14:22.000000 flytekitplugins-kfmpi-1.7.1b0/flytekitplugins_kfmpi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 18:14:22.000000 flytekitplugins-kfmpi-1.7.1b0/flytekitplugins_kfmpi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 18:14:22.082412 flytekitplugins-kfmpi-1.7.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-16 18:14:14.000000 flytekitplugins-kfmpi-1.7.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:56.488678 flytekitplugins-kfmpi-1.7.1b1/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-27 22:00:56.488678 flytekitplugins-kfmpi-1.7.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-27 22:00:35.000000 flytekitplugins-kfmpi-1.7.1b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:56.484678 flytekitplugins-kfmpi-1.7.1b1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:56.488678 flytekitplugins-kfmpi-1.7.1b1/flytekitplugins/kfmpi/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-27 22:00:35.000000 flytekitplugins-kfmpi-1.7.1b1/flytekitplugins/kfmpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-06-27 22:00:35.000000 flytekitplugins-kfmpi-1.7.1b1/flytekitplugins/kfmpi/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:56.488678 flytekitplugins-kfmpi-1.7.1b1/flytekitplugins_kfmpi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-27 22:00:56.000000 flytekitplugins-kfmpi-1.7.1b1/flytekitplugins_kfmpi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-27 22:00:56.000000 flytekitplugins-kfmpi-1.7.1b1/flytekitplugins_kfmpi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 22:00:56.000000 flytekitplugins-kfmpi-1.7.1b1/flytekitplugins_kfmpi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 22:00:56.000000 flytekitplugins-kfmpi-1.7.1b1/flytekitplugins_kfmpi.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 22:00:56.000000 flytekitplugins-kfmpi-1.7.1b1/flytekitplugins_kfmpi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 22:00:56.000000 flytekitplugins-kfmpi-1.7.1b1/flytekitplugins_kfmpi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 22:00:56.488678 flytekitplugins-kfmpi-1.7.1b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-27 22:00:50.000000 flytekitplugins-kfmpi-1.7.1b1/setup.py
```

### Comparing `flytekitplugins-kfmpi-1.7.1b0/PKG-INFO` & `flytekitplugins-kfmpi-1.7.1b1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfmpi
-Version: 1.7.1b0
+Version: 1.7.1b1
 Summary: K8s based MPI plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kfmpi-1.7.1b0/README.md` & `flytekitplugins-kfmpi-1.7.1b1/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-kfmpi-1.7.1b0/flytekitplugins/kfmpi/task.py` & `flytekitplugins-kfmpi-1.7.1b1/flytekitplugins/kfmpi/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-kfmpi-1.7.1b0/flytekitplugins_kfmpi.egg-info/PKG-INFO` & `flytekitplugins-kfmpi-1.7.1b1/flytekitplugins_kfmpi.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfmpi
-Version: 1.7.1b0
+Version: 1.7.1b1
 Summary: K8s based MPI plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kfmpi-1.7.1b0/setup.py` & `flytekitplugins-kfmpi-1.7.1b1/setup.py`

 * *Files identical despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "kfmpi"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.6.1,<2.0.0"]
 
-__version__ = "1.7.1b0"
+__version__ = "1.7.1b1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="K8s based MPI plugin for flytekit",
```

