# Comparing `tmp/felt_upload-0.1.0.tar.gz` & `tmp/felt_upload-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "felt_upload-0.1.0.tar", max compression
+gzip compressed data, was "felt_upload-0.1.1.tar", max compression
```

## Comparing `felt_upload-0.1.0.tar` & `felt_upload-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-06-29 21:12:41.723508 felt_upload-0.1.0/LICENSE
--rw-r--r--   0        0        0     2351 2023-06-30 00:34:45.717853 felt_upload-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-26 03:08:19.466446 felt_upload-0.1.0/felt_upload/__init__.py
--rw-r--r--   0        0        0       71 2023-06-30 00:00:11.711917 felt_upload-0.1.0/felt_upload/__main__.py
--rw-r--r--   0        0        0     4865 2023-06-30 16:25:53.346569 felt_upload-0.1.0/felt_upload/api.py
--rw-r--r--   0        0        0     5863 2023-06-30 00:00:11.712018 felt_upload-0.1.0/felt_upload/cli.py
--rw-r--r--   0        0        0     1074 2023-06-30 19:52:44.925318 felt_upload-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3086 1970-01-01 00:00:00.000000 felt_upload-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-30 22:21:13.744606 felt_upload-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2351 2023-06-30 22:21:13.744606 felt_upload-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 22:21:13.744606 felt_upload-0.1.1/felt_upload/__init__.py
+-rw-r--r--   0        0        0       71 2023-06-30 22:21:13.744606 felt_upload-0.1.1/felt_upload/__main__.py
+-rw-r--r--   0        0        0     4865 2023-06-30 22:21:13.744606 felt_upload-0.1.1/felt_upload/api.py
+-rw-r--r--   0        0        0     5863 2023-06-30 22:21:13.744606 felt_upload-0.1.1/felt_upload/cli.py
+-rw-r--r--   0        0        0     1074 2023-06-30 22:21:13.744606 felt_upload-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3086 1970-01-01 00:00:00.000000 felt_upload-0.1.1/PKG-INFO
```

### Comparing `felt_upload-0.1.0/LICENSE` & `felt_upload-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `felt_upload-0.1.0/README.md` & `felt_upload-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `felt_upload-0.1.0/felt_upload/api.py` & `felt_upload-0.1.1/felt_upload/api.py`

 * *Files identical despite different names*

### Comparing `felt_upload-0.1.0/felt_upload/cli.py` & `felt_upload-0.1.1/felt_upload/cli.py`

 * *Files identical despite different names*

### Comparing `felt_upload-0.1.0/pyproject.toml` & `felt_upload-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "felt-upload"
-version = "0.1.0"
+version = "0.1.1"
 description = "CLI tool to upload data to Felt"
 authors = ["Oleksii Vykaliuk <alekzvik@gmail.com>"]
 readme = "README.md"
 packages = [{include = "felt_upload"}]
 license = "MIT"
 repository = "https://github.com/alekzvik/felt_upload"
```

### Comparing `felt_upload-0.1.0/PKG-INFO` & `felt_upload-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: felt-upload
-Version: 0.1.0
+Version: 0.1.1
 Summary: CLI tool to upload data to Felt
 Home-page: https://github.com/alekzvik/felt_upload
 License: MIT
 Author: Oleksii Vykaliuk
 Author-email: alekzvik@gmail.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
```

