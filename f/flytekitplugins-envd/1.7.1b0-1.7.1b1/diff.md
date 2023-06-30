# Comparing `tmp/flytekitplugins-envd-1.7.1b0.tar.gz` & `tmp/flytekitplugins-envd-1.7.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-envd-1.7.1b0.tar", last modified: Fri Jun 16 18:14:19 2023, max compression
+gzip compressed data, was "flytekitplugins-envd-1.7.1b1.tar", last modified: Tue Jun 27 22:00:54 2023, max compression
```

## Comparing `flytekitplugins-envd-1.7.1b0.tar` & `flytekitplugins-envd-1.7.1b1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:19.694435 flytekitplugins-envd-1.7.1b0/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-16 18:14:19.694435 flytekitplugins-envd-1.7.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-16 18:13:54.000000 flytekitplugins-envd-1.7.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:19.690436 flytekitplugins-envd-1.7.1b0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:19.690436 flytekitplugins-envd-1.7.1b0/flytekitplugins/envd/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-16 18:13:54.000000 flytekitplugins-envd-1.7.1b0/flytekitplugins/envd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-16 18:13:54.000000 flytekitplugins-envd-1.7.1b0/flytekitplugins/envd/image_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:19.694435 flytekitplugins-envd-1.7.1b0/flytekitplugins_envd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-16 18:14:19.000000 flytekitplugins-envd-1.7.1b0/flytekitplugins_envd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-16 18:14:19.000000 flytekitplugins-envd-1.7.1b0/flytekitplugins_envd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 18:14:19.000000 flytekitplugins-envd-1.7.1b0/flytekitplugins_envd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 18:14:19.000000 flytekitplugins-envd-1.7.1b0/flytekitplugins_envd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 18:14:19.000000 flytekitplugins-envd-1.7.1b0/flytekitplugins_envd.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 18:14:19.000000 flytekitplugins-envd-1.7.1b0/flytekitplugins_envd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 18:14:19.000000 flytekitplugins-envd-1.7.1b0/flytekitplugins_envd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 18:14:19.694435 flytekitplugins-envd-1.7.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-16 18:14:14.000000 flytekitplugins-envd-1.7.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:54.636640 flytekitplugins-envd-1.7.1b1/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-27 22:00:54.636640 flytekitplugins-envd-1.7.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-27 22:00:35.000000 flytekitplugins-envd-1.7.1b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:54.636640 flytekitplugins-envd-1.7.1b1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:54.636640 flytekitplugins-envd-1.7.1b1/flytekitplugins/envd/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-27 22:00:35.000000 flytekitplugins-envd-1.7.1b1/flytekitplugins/envd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-27 22:00:35.000000 flytekitplugins-envd-1.7.1b1/flytekitplugins/envd/image_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:54.636640 flytekitplugins-envd-1.7.1b1/flytekitplugins_envd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-27 22:00:54.000000 flytekitplugins-envd-1.7.1b1/flytekitplugins_envd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-27 22:00:54.000000 flytekitplugins-envd-1.7.1b1/flytekitplugins_envd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 22:00:54.000000 flytekitplugins-envd-1.7.1b1/flytekitplugins_envd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 22:00:54.000000 flytekitplugins-envd-1.7.1b1/flytekitplugins_envd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 22:00:54.000000 flytekitplugins-envd-1.7.1b1/flytekitplugins_envd.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 22:00:54.000000 flytekitplugins-envd-1.7.1b1/flytekitplugins_envd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 22:00:54.000000 flytekitplugins-envd-1.7.1b1/flytekitplugins_envd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 22:00:54.636640 flytekitplugins-envd-1.7.1b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-27 22:00:50.000000 flytekitplugins-envd-1.7.1b1/setup.py
```

### Comparing `flytekitplugins-envd-1.7.1b0/PKG-INFO` & `flytekitplugins-envd-1.7.1b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-envd
-Version: 1.7.1b0
+Version: 1.7.1b1
 Summary: This package enables users to easily build a Docker image for tasks or workflows.
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-envd-1.7.1b0/README.md` & `flytekitplugins-envd-1.7.1b1/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-envd-1.7.1b0/flytekitplugins/envd/image_builder.py` & `flytekitplugins-envd-1.7.1b1/flytekitplugins/envd/image_builder.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-envd-1.7.1b0/flytekitplugins_envd.egg-info/PKG-INFO` & `flytekitplugins-envd-1.7.1b1/flytekitplugins_envd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-envd
-Version: 1.7.1b0
+Version: 1.7.1b1
 Summary: This package enables users to easily build a Docker image for tasks or workflows.
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-envd-1.7.1b0/setup.py` & `flytekitplugins-envd-1.7.1b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "envd"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit", "envd>=0.3.22"]
 
-__version__ = "1.7.1b0"
+__version__ = "1.7.1b1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package enables users to easily build a Docker image for tasks or workflows.",
```

