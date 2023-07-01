# Comparing `tmp/scriptl-0.1.tar.gz` & `tmp/scriptl-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scriptl-0.1.tar", last modified: Sat Jul  1 18:48:35 2023, max compression
+gzip compressed data, was "scriptl-0.2.tar", last modified: Sat Jul  1 18:49:47 2023, max compression
```

## Comparing `scriptl-0.1.tar` & `scriptl-0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 dylan     (1000) dylanr    (1000)        0 2023-07-01 18:48:35.046689 scriptl-0.1/
--rw-r--r--   0 dylan     (1000) dylanr    (1000)      769 2023-07-01 18:48:35.046689 scriptl-0.1/PKG-INFO
--rw-r--r--   0 dylan     (1000) dylanr    (1000)      272 2023-07-01 18:35:22.000000 scriptl-0.1/README.md
--rw-r--r--   0 dylan     (1000) dylanr    (1000)      499 2023-07-01 18:48:30.000000 scriptl-0.1/pyproject.toml
-drwxr-xr-x   0 dylan     (1000) dylanr    (1000)        0 2023-07-01 18:48:35.046689 scriptl-0.1/scriptl/
--rw-r--r--   0 dylan     (1000) dylanr    (1000)      164 2023-07-01 18:47:39.000000 scriptl-0.1/scriptl/__init__.py
-drwxr-xr-x   0 dylan     (1000) dylanr    (1000)        0 2023-07-01 18:48:35.046689 scriptl-0.1/scriptl.egg-info/
--rw-r--r--   0 dylan     (1000) dylanr    (1000)      769 2023-07-01 18:48:35.000000 scriptl-0.1/scriptl.egg-info/PKG-INFO
--rw-r--r--   0 dylan     (1000) dylanr    (1000)      168 2023-07-01 18:48:35.000000 scriptl-0.1/scriptl.egg-info/SOURCES.txt
--rw-r--r--   0 dylan     (1000) dylanr    (1000)        1 2023-07-01 18:48:35.000000 scriptl-0.1/scriptl.egg-info/dependency_links.txt
--rw-r--r--   0 dylan     (1000) dylanr    (1000)        8 2023-07-01 18:48:35.000000 scriptl-0.1/scriptl.egg-info/top_level.txt
--rw-r--r--   0 dylan     (1000) dylanr    (1000)       38 2023-07-01 18:48:35.046689 scriptl-0.1/setup.cfg
+drwxr-xr-x   0 dylan     (1000) dylanr    (1000)        0 2023-07-01 18:49:47.112924 scriptl-0.2/
+-rw-r--r--   0 dylan     (1000) dylanr    (1000)      769 2023-07-01 18:49:47.112924 scriptl-0.2/PKG-INFO
+-rw-r--r--   0 dylan     (1000) dylanr    (1000)      272 2023-07-01 18:35:22.000000 scriptl-0.2/README.md
+-rw-r--r--   0 dylan     (1000) dylanr    (1000)      499 2023-07-01 18:49:42.000000 scriptl-0.2/pyproject.toml
+drwxr-xr-x   0 dylan     (1000) dylanr    (1000)        0 2023-07-01 18:49:47.109591 scriptl-0.2/scriptl/
+-rw-r--r--   0 dylan     (1000) dylanr    (1000)      192 2023-07-01 18:49:27.000000 scriptl-0.2/scriptl/__init__.py
+-rw-r--r--   0 dylan     (1000) dylanr    (1000)        0 2023-07-01 18:49:33.000000 scriptl-0.2/scriptl/console.py
+drwxr-xr-x   0 dylan     (1000) dylanr    (1000)        0 2023-07-01 18:49:47.109591 scriptl-0.2/scriptl.egg-info/
+-rw-r--r--   0 dylan     (1000) dylanr    (1000)      769 2023-07-01 18:49:47.000000 scriptl-0.2/scriptl.egg-info/PKG-INFO
+-rw-r--r--   0 dylan     (1000) dylanr    (1000)      187 2023-07-01 18:49:47.000000 scriptl-0.2/scriptl.egg-info/SOURCES.txt
+-rw-r--r--   0 dylan     (1000) dylanr    (1000)        1 2023-07-01 18:49:47.000000 scriptl-0.2/scriptl.egg-info/dependency_links.txt
+-rw-r--r--   0 dylan     (1000) dylanr    (1000)        8 2023-07-01 18:49:47.000000 scriptl-0.2/scriptl.egg-info/top_level.txt
+-rw-r--r--   0 dylan     (1000) dylanr    (1000)       38 2023-07-01 18:49:47.112924 scriptl-0.2/setup.cfg
```

### Comparing `scriptl-0.1/PKG-INFO` & `scriptl-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scriptl
-Version: 0.1
+Version: 0.2
 Summary: Scriptl: Making Python programming a little easier
 Author-email: The Open Project <opendylan@proton.me>
 Project-URL: Homepage, https://github.com/dylanopen/scriptl
 Project-URL: Bug Tracker, https://github.com/dylanopen/scriptl/issues
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `scriptl-0.1/scriptl.egg-info/PKG-INFO` & `scriptl-0.2/scriptl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scriptl
-Version: 0.1
+Version: 0.2
 Summary: Scriptl: Making Python programming a little easier
 Author-email: The Open Project <opendylan@proton.me>
 Project-URL: Homepage, https://github.com/dylanopen/scriptl
 Project-URL: Bug Tracker, https://github.com/dylanopen/scriptl/issues
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

