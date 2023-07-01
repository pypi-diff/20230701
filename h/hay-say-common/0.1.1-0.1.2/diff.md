# Comparing `tmp/hay_say_common-0.1.1.tar.gz` & `tmp/hay_say_common-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hay_say_common-0.1.1.tar", last modified: Fri Jun 30 19:27:13 2023, max compression
+gzip compressed data, was "hay_say_common-0.1.2.tar", last modified: Sat Jul  1 04:46:00 2023, max compression
```

## Comparing `hay_say_common-0.1.1.tar` & `hay_say_common-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 hydrusbeta  (1000) hydrusbeta  (1000)        0 2023-06-30 19:27:13.622933 hay_say_common-0.1.1/
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)    11358 2023-04-13 03:14:23.000000 hay_say_common-0.1.1/LICENSE
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      856 2023-06-30 19:27:13.622933 hay_say_common-0.1.1/PKG-INFO
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      192 2023-04-08 03:11:32.000000 hay_say_common-0.1.1/README.md
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      805 2023-06-30 19:22:28.000000 hay_say_common-0.1.1/pyproject.toml
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)       38 2023-06-30 19:27:13.622933 hay_say_common-0.1.1/setup.cfg
-drwxrwxr-x   0 hydrusbeta  (1000) hydrusbeta  (1000)        0 2023-06-30 19:27:13.622933 hay_say_common-0.1.1/src/
-drwxrwxr-x   0 hydrusbeta  (1000) hydrusbeta  (1000)        0 2023-06-30 19:27:13.622933 hay_say_common-0.1.1/src/hay_say_common/
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      872 2023-04-09 17:06:42.000000 hay_say_common-0.1.1/src/hay_say_common/__init__.py
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)     7291 2023-06-26 03:44:42.000000 hay_say_common-0.1.1/src/hay_say_common/file_integration.py
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)     2363 2023-04-08 04:46:20.000000 hay_say_common-0.1.1/src/hay_say_common/server_utility.py
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)     1116 2023-04-09 16:01:38.000000 hay_say_common-0.1.1/src/hay_say_common/utility.py
-drwxrwxr-x   0 hydrusbeta  (1000) hydrusbeta  (1000)        0 2023-06-30 19:27:13.622933 hay_say_common-0.1.1/src/hay_say_common.egg-info/
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      856 2023-06-30 19:27:13.000000 hay_say_common-0.1.1/src/hay_say_common.egg-info/PKG-INFO
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      378 2023-06-30 19:27:13.000000 hay_say_common-0.1.1/src/hay_say_common.egg-info/SOURCES.txt
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)        1 2023-06-30 19:27:13.000000 hay_say_common-0.1.1/src/hay_say_common.egg-info/dependency_links.txt
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)       52 2023-06-30 19:27:13.000000 hay_say_common-0.1.1/src/hay_say_common.egg-info/requires.txt
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)       15 2023-06-30 19:27:13.000000 hay_say_common-0.1.1/src/hay_say_common.egg-info/top_level.txt
+drwxrwxr-x   0 hydrusbeta  (1000) hydrusbeta  (1000)        0 2023-07-01 04:46:00.811364 hay_say_common-0.1.2/
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)    11358 2023-04-13 03:14:23.000000 hay_say_common-0.1.2/LICENSE
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      856 2023-07-01 04:46:00.811364 hay_say_common-0.1.2/PKG-INFO
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      192 2023-04-08 03:11:32.000000 hay_say_common-0.1.2/README.md
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      805 2023-07-01 04:45:32.000000 hay_say_common-0.1.2/pyproject.toml
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)       38 2023-07-01 04:46:00.811364 hay_say_common-0.1.2/setup.cfg
+drwxrwxr-x   0 hydrusbeta  (1000) hydrusbeta  (1000)        0 2023-07-01 04:46:00.811364 hay_say_common-0.1.2/src/
+drwxrwxr-x   0 hydrusbeta  (1000) hydrusbeta  (1000)        0 2023-07-01 04:46:00.811364 hay_say_common-0.1.2/src/hay_say_common/
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      965 2023-07-01 04:32:16.000000 hay_say_common-0.1.2/src/hay_say_common/__init__.py
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)     7291 2023-06-26 03:44:42.000000 hay_say_common-0.1.2/src/hay_say_common/file_integration.py
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)     2444 2023-07-01 04:39:54.000000 hay_say_common-0.1.2/src/hay_say_common/server_utility.py
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)     2202 2023-07-01 04:31:55.000000 hay_say_common-0.1.2/src/hay_say_common/utility.py
+drwxrwxr-x   0 hydrusbeta  (1000) hydrusbeta  (1000)        0 2023-07-01 04:46:00.811364 hay_say_common-0.1.2/src/hay_say_common.egg-info/
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      856 2023-07-01 04:46:00.000000 hay_say_common-0.1.2/src/hay_say_common.egg-info/PKG-INFO
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      378 2023-07-01 04:46:00.000000 hay_say_common-0.1.2/src/hay_say_common.egg-info/SOURCES.txt
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)        1 2023-07-01 04:46:00.000000 hay_say_common-0.1.2/src/hay_say_common.egg-info/dependency_links.txt
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)       52 2023-07-01 04:46:00.000000 hay_say_common-0.1.2/src/hay_say_common.egg-info/requires.txt
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)       15 2023-07-01 04:46:00.000000 hay_say_common-0.1.2/src/hay_say_common.egg-info/top_level.txt
```

### Comparing `hay_say_common-0.1.1/LICENSE` & `hay_say_common-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hay_say_common-0.1.1/PKG-INFO` & `hay_say_common-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hay_say_common
-Version: 0.1.1
+Version: 0.1.2
 Summary: Constants and methods that are shared between the Hay Say UI and various Docker containers it communicates with.
 Author-email: HydrusBeta <hydrusgamma@gmail.com>
 Project-URL: Homepage, https://github.com/hydrusbeta/hay_say_common
 Project-URL: Bug Tracker, https://github.com/hydrusbeta/hay_say_common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `hay_say_common-0.1.1/pyproject.toml` & `hay_say_common-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hay_say_common"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
 	{name = "HydrusBeta", email="hydrusgamma@gmail.com"},
 ]
 description = "Constants and methods that are shared between the Hay Say UI and various Docker containers it communicates with."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `hay_say_common-0.1.1/src/hay_say_common/file_integration.py` & `hay_say_common-0.1.2/src/hay_say_common/file_integration.py`

 * *Files identical despite different names*

### Comparing `hay_say_common-0.1.1/src/hay_say_common/server_utility.py` & `hay_say_common-0.1.2/src/hay_say_common/server_utility.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 from flask import request
 
 import os
 import traceback
 import json
 
 
+"""Methods that are useful across multiple architecture servers"""
+
+
 def create_link(existing_path, desired_link_path):
     if not os.path.exists(desired_link_path):
         os.symlink(existing_path, desired_link_path)
 
 
 def get_model_path(architecture, character):
     character_dir = [os.path.join(model_dir, character)
@@ -49,12 +52,12 @@
     output_files = get_file_list(OUTPUT_DIR)
     return 'An error occurred while generating the output: \n' + traceback.format_exc() + \
            '\n\nPayload:\n' + json.dumps(request.json) + \
            '\n\nInput Audio Dir Listing: \n' + input_files + \
            '\n\nOutput Audio Dir Listing: \n' + output_files
 
 
-def get_file_list(folder):
-    if os.path.exists(folder):
-        return ', '.join(os.listdir(folder))
+def get_file_list(directory):
+    if os.path.exists(directory):
+        return ', '.join(os.listdir(directory))
     else:
-        return 'directory does not exist'
+        return directory + ' does not exist'
```

### Comparing `hay_say_common-0.1.1/src/hay_say_common.egg-info/PKG-INFO` & `hay_say_common-0.1.2/src/hay_say_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hay-say-common
-Version: 0.1.1
+Version: 0.1.2
 Summary: Constants and methods that are shared between the Hay Say UI and various Docker containers it communicates with.
 Author-email: HydrusBeta <hydrusgamma@gmail.com>
 Project-URL: Homepage, https://github.com/hydrusbeta/hay_say_common
 Project-URL: Bug Tracker, https://github.com/hydrusbeta/hay_say_common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

