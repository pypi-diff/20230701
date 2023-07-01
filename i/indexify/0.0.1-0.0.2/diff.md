# Comparing `tmp/indexify-0.0.1.tar.gz` & `tmp/indexify-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indexify-0.0.1.tar", max compression
+gzip compressed data, was "indexify-0.0.2.tar", max compression
```

## Comparing `indexify-0.0.1.tar` & `indexify-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-05-15 05:42:57.008356 indexify-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0       24 2023-05-15 05:43:22.194846 indexify-0.0.1/README.rst
--rw-r--r--   0        0        0       35 2023-05-15 05:40:31.360078 indexify-0.0.1/indexify/__init__.py
--rw-r--r--   0        0        0     3058 2023-05-19 20:20:11.691680 indexify-0.0.1/indexify/indexify.py
--rw-r--r--   0        0        0      610 2023-05-19 20:23:00.533933 indexify-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 indexify-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-18 02:13:50.038752 indexify-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0       24 2023-05-18 02:13:50.038752 indexify-0.0.2/README.rst
+-rw-r--r--   0        0        0      248 2023-06-30 08:17:54.563913 indexify-0.0.2/indexify/__init__.py
+-rw-r--r--   0        0        0      893 2023-06-30 08:38:30.169941 indexify-0.0.2/indexify/data_containers.py
+-rw-r--r--   0        0        0      593 2023-06-30 08:18:22.671782 indexify-0.0.2/indexify/index.py
+-rw-r--r--   0        0        0     1228 2023-06-30 08:23:16.938669 indexify-0.0.2/indexify/memory.py
+-rw-r--r--   0        0        0      540 2023-06-30 08:21:01.855044 indexify-0.0.2/indexify/repository.py
+-rw-r--r--   0        0        0      640 2023-06-30 08:18:50.967650 indexify-0.0.2/indexify/utils.py
+-rw-r--r--   0        0        0      655 2023-06-30 07:59:52.097544 indexify-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 indexify-0.0.2/PKG-INFO
```

### Comparing `indexify-0.0.1/LICENSE.txt` & `indexify-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `indexify-0.0.1/pyproject.toml` & `indexify-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "indexify"
-version = "0.0.1"
+version = "0.0.2"
 description = "Python Client for Indexify"
-authors = ["Diptanu Gon Choudhury <diptanuc@gmail.com>"]
+authors = ["Diptanu Gon Choudhury <diptanuc@gmail.com>", "Vijay Parthasarathy <vijay2win@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.rst"
 homepage = "https://github.com/diptanu/indexify"
 repository = "https://github.com/diptanu/indexify"
 
 [tool.poetry.dependencies]
 python = "^3.10.0"
```

### Comparing `indexify-0.0.1/PKG-INFO` & `indexify-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indexify
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python Client for Indexify
 Home-page: https://github.com/diptanu/indexify
 License: Apache 2.0
 Author: Diptanu Gon Choudhury
 Author-email: diptanuc@gmail.com
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: License :: Other/Proprietary License
```

