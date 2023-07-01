# Comparing `tmp/monstermash-1.7.0.tar.gz` & `tmp/monstermash-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monstermash-1.7.0.tar", max compression
+gzip compressed data, was "monstermash-1.7.1.tar", max compression
```

## Comparing `monstermash-1.7.0.tar` & `monstermash-1.7.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2170 2023-07-01 03:34:19.111696 monstermash-1.7.0/README.md
--rw-r--r--   0        0        0     1152 2023-07-01 03:34:19.111696 monstermash-1.7.0/pyproject.toml
--rw-r--r--   0        0        0       86 2023-07-01 03:34:19.111696 monstermash-1.7.0/src/monstermash/__init__.py
--rw-r--r--   0        0        0     4205 2023-07-01 03:34:19.111696 monstermash-1.7.0/src/monstermash/__main__.py
--rw-r--r--   0        0        0     1024 2023-07-01 03:34:19.111696 monstermash-1.7.0/src/monstermash/config.py
--rw-r--r--   0        0        0     3680 2023-07-01 03:34:19.111696 monstermash-1.7.0/src/monstermash/crypt.py
--rw-r--r--   0        0        0      399 2023-07-01 03:34:19.111696 monstermash-1.7.0/src/monstermash/datamodels.py
--rw-r--r--   0        0        0     1272 2023-07-01 03:34:19.111696 monstermash-1.7.0/src/monstermash/parser.py
--rw-r--r--   0        0        0        0 2023-07-01 03:34:19.111696 monstermash-1.7.0/src/monstermash/utils/__init__.py
--rw-r--r--   0        0        0      709 2023-07-01 03:34:19.111696 monstermash-1.7.0/src/monstermash/utils/file.py
--rw-r--r--   0        0        0     2729 1970-01-01 00:00:00.000000 monstermash-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     2170 2023-07-01 03:38:27.004420 monstermash-1.7.1/README.md
+-rw-r--r--   0        0        0     1152 2023-07-01 03:38:27.004420 monstermash-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0       86 2023-07-01 03:38:27.004420 monstermash-1.7.1/src/monstermash/__init__.py
+-rw-r--r--   0        0        0     4205 2023-07-01 03:38:27.004420 monstermash-1.7.1/src/monstermash/__main__.py
+-rw-r--r--   0        0        0     1024 2023-07-01 03:38:27.004420 monstermash-1.7.1/src/monstermash/config.py
+-rw-r--r--   0        0        0     3680 2023-07-01 03:38:27.008421 monstermash-1.7.1/src/monstermash/crypt.py
+-rw-r--r--   0        0        0      399 2023-07-01 03:38:27.008421 monstermash-1.7.1/src/monstermash/datamodels.py
+-rw-r--r--   0        0        0     1272 2023-07-01 03:38:27.008421 monstermash-1.7.1/src/monstermash/parser.py
+-rw-r--r--   0        0        0        0 2023-07-01 03:38:27.008421 monstermash-1.7.1/src/monstermash/utils/__init__.py
+-rw-r--r--   0        0        0      709 2023-07-01 03:38:27.008421 monstermash-1.7.1/src/monstermash/utils/file.py
+-rw-r--r--   0        0        0     2729 1970-01-01 00:00:00.000000 monstermash-1.7.1/PKG-INFO
```

### Comparing `monstermash-1.7.0/README.md` & `monstermash-1.7.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ##  🧟 Monstermash
 
-> 1️⃣ version: 1.7.0
+> 1️⃣ version: 1.7.1
 
 > ✍️ author: Mitchell Lisle
 
 ## Install
 Install from PyPi
 
 ```shell
```

### Comparing `monstermash-1.7.0/pyproject.toml` & `monstermash-1.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monstermash"
-version = "1.7.0"
+version = "1.7.1"
 description = ""
 authors = ["Mitchell Lisle <m.lisle90@gmail.com>"]
 readme = "README.md"
 packages = [{include = "monstermash", from = "src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
```

### Comparing `monstermash-1.7.0/src/monstermash/__main__.py` & `monstermash-1.7.1/src/monstermash/__main__.py`

 * *Files identical despite different names*

### Comparing `monstermash-1.7.0/src/monstermash/config.py` & `monstermash-1.7.1/src/monstermash/config.py`

 * *Files identical despite different names*

### Comparing `monstermash-1.7.0/src/monstermash/crypt.py` & `monstermash-1.7.1/src/monstermash/crypt.py`

 * *Files identical despite different names*

### Comparing `monstermash-1.7.0/src/monstermash/parser.py` & `monstermash-1.7.1/src/monstermash/parser.py`

 * *Files identical despite different names*

### Comparing `monstermash-1.7.0/src/monstermash/utils/file.py` & `monstermash-1.7.1/src/monstermash/utils/file.py`

 * *Files identical despite different names*

### Comparing `monstermash-1.7.0/PKG-INFO` & `monstermash-1.7.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monstermash
-Version: 1.7.0
+Version: 1.7.1
 Summary: 
 Author: Mitchell Lisle
 Author-email: m.lisle90@gmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -13,15 +13,15 @@
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pynacl (>=1.5.0,<2.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 ##  🧟 Monstermash
 
-> 1️⃣ version: 1.7.0
+> 1️⃣ version: 1.7.1
 
 > ✍️ author: Mitchell Lisle
 
 ## Install
 Install from PyPi
 
 ```shell
```

