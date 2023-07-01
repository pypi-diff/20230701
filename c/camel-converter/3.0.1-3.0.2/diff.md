# Comparing `tmp/camel_converter-3.0.1.tar.gz` & `tmp/camel_converter-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camel_converter-3.0.1.tar", max compression
+gzip compressed data, was "camel_converter-3.0.2.tar", max compression
```

## Comparing `camel_converter-3.0.1.tar` & `camel_converter-3.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-06-25 12:57:35.391050 camel_converter-3.0.1/LICENSE
--rw-r--r--   0        0        0     4291 2023-06-25 12:57:35.391050 camel_converter-3.0.1/README.md
--rw-r--r--   0        0        0     4216 2023-06-25 12:57:35.391050 camel_converter-3.0.1/camel_converter/__init__.py
--rw-r--r--   0        0        0     1128 2023-06-25 12:57:35.391050 camel_converter-3.0.1/camel_converter/decorators.py
--rw-r--r--   0        0        0        0 2023-06-25 12:57:35.391050 camel_converter-3.0.1/camel_converter/py.typed
--rw-r--r--   0        0        0      648 2023-06-25 12:57:35.391050 camel_converter-3.0.1/camel_converter/pydantic_base.py
--rw-r--r--   0        0        0     1860 2023-06-25 12:57:35.391050 camel_converter-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     5355 1970-01-01 00:00:00.000000 camel_converter-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-01 14:20:46.106745 camel_converter-3.0.2/LICENSE
+-rw-r--r--   0        0        0     4291 2023-07-01 14:20:46.106745 camel_converter-3.0.2/README.md
+-rw-r--r--   0        0        0     4216 2023-07-01 14:20:46.106745 camel_converter-3.0.2/camel_converter/__init__.py
+-rw-r--r--   0        0        0     1128 2023-07-01 14:20:46.106745 camel_converter-3.0.2/camel_converter/decorators.py
+-rw-r--r--   0        0        0        0 2023-07-01 14:20:46.106745 camel_converter-3.0.2/camel_converter/py.typed
+-rw-r--r--   0        0        0     1319 2023-07-01 14:20:46.106745 camel_converter-3.0.2/camel_converter/pydantic_base.py
+-rw-r--r--   0        0        0     1860 2023-07-01 14:20:46.106745 camel_converter-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5355 1970-01-01 00:00:00.000000 camel_converter-3.0.2/PKG-INFO
```

### Comparing `camel_converter-3.0.1/LICENSE` & `camel_converter-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `camel_converter-3.0.1/README.md` & `camel_converter-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `camel_converter-3.0.1/camel_converter/__init__.py` & `camel_converter-3.0.2/camel_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_converter-3.0.1/camel_converter/decorators.py` & `camel_converter-3.0.2/camel_converter/decorators.py`

 * *Files identical despite different names*

### Comparing `camel_converter-3.0.1/pyproject.toml` & `camel_converter-3.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "camel-converter"
-version = "3.0.1"
+version = "3.0.2"
 description = "Converts a string from snake case to camel case or camel case to snake case"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/camel-converter"
 homepage = "https://github.com/sanders41/camel-converter"
 documentation = "https://github.com/sanders41/camel-converter"
```

### Comparing `camel_converter-3.0.1/PKG-INFO` & `camel_converter-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camel-converter
-Version: 3.0.1
+Version: 3.0.2
 Summary: Converts a string from snake case to camel case or camel case to snake case
 Home-page: https://github.com/sanders41/camel-converter
 License: MIT
 Keywords: python,pydantic
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
 Requires-Python: >=3.8,<4.0
```

