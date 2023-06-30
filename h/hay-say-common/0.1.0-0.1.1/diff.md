# Comparing `tmp/hay_say_common-0.1.0.tar.gz` & `tmp/hay_say_common-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hay_say_common-0.1.0.tar", last modified: Fri Apr 14 02:06:20 2023, max compression
+gzip compressed data, was "hay_say_common-0.1.1.tar", last modified: Fri Jun 30 19:27:13 2023, max compression
```

## Comparing `hay_say_common-0.1.0.tar` & `hay_say_common-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 hydrusbeta  (1000) hydrusbeta  (1000)        0 2023-04-14 02:06:20.334288 hay_say_common-0.1.0/
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)    11358 2023-04-13 03:14:23.000000 hay_say_common-0.1.0/LICENSE
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      856 2023-04-14 02:06:20.334288 hay_say_common-0.1.0/PKG-INFO
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      192 2023-04-08 03:11:32.000000 hay_say_common-0.1.0/README.md
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      805 2023-04-14 02:03:50.000000 hay_say_common-0.1.0/pyproject.toml
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)       38 2023-04-14 02:06:20.334288 hay_say_common-0.1.0/setup.cfg
-drwxrwxr-x   0 hydrusbeta  (1000) hydrusbeta  (1000)        0 2023-04-14 02:06:20.334288 hay_say_common-0.1.0/src/
-drwxrwxr-x   0 hydrusbeta  (1000) hydrusbeta  (1000)        0 2023-04-14 02:06:20.334288 hay_say_common-0.1.0/src/hay_say_common/
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      872 2023-04-09 17:06:42.000000 hay_say_common-0.1.0/src/hay_say_common/__init__.py
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)     6896 2023-04-09 16:01:38.000000 hay_say_common-0.1.0/src/hay_say_common/file_integration.py
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)     2363 2023-04-08 04:46:20.000000 hay_say_common-0.1.0/src/hay_say_common/server_utility.py
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)     1116 2023-04-09 16:01:38.000000 hay_say_common-0.1.0/src/hay_say_common/utility.py
-drwxrwxr-x   0 hydrusbeta  (1000) hydrusbeta  (1000)        0 2023-04-14 02:06:20.334288 hay_say_common-0.1.0/src/hay_say_common.egg-info/
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      856 2023-04-14 02:06:20.000000 hay_say_common-0.1.0/src/hay_say_common.egg-info/PKG-INFO
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      378 2023-04-14 02:06:20.000000 hay_say_common-0.1.0/src/hay_say_common.egg-info/SOURCES.txt
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)        1 2023-04-14 02:06:20.000000 hay_say_common-0.1.0/src/hay_say_common.egg-info/dependency_links.txt
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)       52 2023-04-14 02:06:20.000000 hay_say_common-0.1.0/src/hay_say_common.egg-info/requires.txt
--rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)       15 2023-04-14 02:06:20.000000 hay_say_common-0.1.0/src/hay_say_common.egg-info/top_level.txt
+drwxrwxr-x   0 hydrusbeta  (1000) hydrusbeta  (1000)        0 2023-06-30 19:27:13.622933 hay_say_common-0.1.1/
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)    11358 2023-04-13 03:14:23.000000 hay_say_common-0.1.1/LICENSE
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      856 2023-06-30 19:27:13.622933 hay_say_common-0.1.1/PKG-INFO
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      192 2023-04-08 03:11:32.000000 hay_say_common-0.1.1/README.md
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      805 2023-06-30 19:22:28.000000 hay_say_common-0.1.1/pyproject.toml
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)       38 2023-06-30 19:27:13.622933 hay_say_common-0.1.1/setup.cfg
+drwxrwxr-x   0 hydrusbeta  (1000) hydrusbeta  (1000)        0 2023-06-30 19:27:13.622933 hay_say_common-0.1.1/src/
+drwxrwxr-x   0 hydrusbeta  (1000) hydrusbeta  (1000)        0 2023-06-30 19:27:13.622933 hay_say_common-0.1.1/src/hay_say_common/
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      872 2023-04-09 17:06:42.000000 hay_say_common-0.1.1/src/hay_say_common/__init__.py
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)     7291 2023-06-26 03:44:42.000000 hay_say_common-0.1.1/src/hay_say_common/file_integration.py
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)     2363 2023-04-08 04:46:20.000000 hay_say_common-0.1.1/src/hay_say_common/server_utility.py
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)     1116 2023-04-09 16:01:38.000000 hay_say_common-0.1.1/src/hay_say_common/utility.py
+drwxrwxr-x   0 hydrusbeta  (1000) hydrusbeta  (1000)        0 2023-06-30 19:27:13.622933 hay_say_common-0.1.1/src/hay_say_common.egg-info/
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      856 2023-06-30 19:27:13.000000 hay_say_common-0.1.1/src/hay_say_common.egg-info/PKG-INFO
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)      378 2023-06-30 19:27:13.000000 hay_say_common-0.1.1/src/hay_say_common.egg-info/SOURCES.txt
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)        1 2023-06-30 19:27:13.000000 hay_say_common-0.1.1/src/hay_say_common.egg-info/dependency_links.txt
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)       52 2023-06-30 19:27:13.000000 hay_say_common-0.1.1/src/hay_say_common.egg-info/requires.txt
+-rw-rw-r--   0 hydrusbeta  (1000) hydrusbeta  (1000)       15 2023-06-30 19:27:13.000000 hay_say_common-0.1.1/src/hay_say_common.egg-info/top_level.txt
```

### Comparing `hay_say_common-0.1.0/LICENSE` & `hay_say_common-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hay_say_common-0.1.0/PKG-INFO` & `hay_say_common-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hay_say_common
-Version: 0.1.0
+Version: 0.1.1
 Summary: Constants and methods that are shared between the Hay Say UI and various Docker containers it communicates with.
 Author-email: HydrusBeta <hydrusgamma@gmail.com>
 Project-URL: Homepage, https://github.com/hydrusbeta/hay_say_common
 Project-URL: Bug Tracker, https://github.com/hydrusbeta/hay_say_common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `hay_say_common-0.1.0/pyproject.toml` & `hay_say_common-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hay_say_common"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
 	{name = "HydrusBeta", email="hydrusgamma@gmail.com"},
 ]
 description = "Constants and methods that are shared between the Hay Say UI and various Docker containers it communicates with."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `hay_say_common-0.1.0/src/hay_say_common/__init__.py` & `hay_say_common-0.1.1/src/hay_say_common/__init__.py`

 * *Files identical despite different names*

### Comparing `hay_say_common-0.1.0/src/hay_say_common/file_integration.py` & `hay_say_common-0.1.1/src/hay_say_common/file_integration.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,17 +45,25 @@
     dirs = [directory
             for directory in [os.path.join(ROOT_DIR, architecture_name + '_model_pack_' + str(index))
                               for index in range(100)]
             if os.path.exists(directory) and not os.path.isfile(directory)]
     custom_model_path = os.path.join(ROOT_DIR, 'custom_models', architecture_name)
     if os.path.exists(custom_model_path):
         dirs.append(custom_model_path)
+    characters_dir = os.path.join(ROOT_DIR, 'models', architecture_name, 'characters')
+    if os.path.exists(characters_dir):
+        dirs.append(characters_dir)
     return dirs
 
 
+def multispeaker_model_dir(architecture_name):
+    """Returns the directory where multi-speaker models are stored for the given architecture."""
+    return os.path.join(ROOT_DIR, 'models', architecture_name, 'multispeaker_models')
+
+
 def read_metadata(folder):
     """Return the metadata dictionary of a given audio_cache subfolder.
     'folder' should be one of: RAW_DIR, PREPROCESSED_DIR, OUTPUT_DIR, or POSTPROCESSED_DIR."""
     path_to_file = os.path.join(folder, METADATA_FILENAME)
     metadata = dict()
     if os.path.isfile(path_to_file):
         with open(path_to_file, 'r') as file:
```

### Comparing `hay_say_common-0.1.0/src/hay_say_common/server_utility.py` & `hay_say_common-0.1.1/src/hay_say_common/server_utility.py`

 * *Files identical despite different names*

### Comparing `hay_say_common-0.1.0/src/hay_say_common/utility.py` & `hay_say_common-0.1.1/src/hay_say_common/utility.py`

 * *Files identical despite different names*

### Comparing `hay_say_common-0.1.0/src/hay_say_common.egg-info/PKG-INFO` & `hay_say_common-0.1.1/src/hay_say_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hay-say-common
-Version: 0.1.0
+Version: 0.1.1
 Summary: Constants and methods that are shared between the Hay Say UI and various Docker containers it communicates with.
 Author-email: HydrusBeta <hydrusgamma@gmail.com>
 Project-URL: Homepage, https://github.com/hydrusbeta/hay_say_common
 Project-URL: Bug Tracker, https://github.com/hydrusbeta/hay_say_common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

