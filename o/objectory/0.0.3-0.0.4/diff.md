# Comparing `tmp/objectory-0.0.3.tar.gz` & `tmp/objectory-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objectory-0.0.3.tar", max compression
+gzip compressed data, was "objectory-0.0.4.tar", max compression
```

## Comparing `objectory-0.0.3.tar` & `objectory-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1501 2023-06-25 05:56:41.507082 objectory-0.0.3/LICENSE
--rw-r--r--   0        0        0     4516 2023-06-25 05:56:41.507082 objectory-0.0.3/README.md
--rw-r--r--   0        0        0     3829 2023-06-25 05:56:41.511082 objectory-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      280 2023-06-25 05:56:41.511082 objectory-0.0.3/src/objectory/__init__.py
--rw-r--r--   0        0        0    13109 2023-06-25 05:56:41.511082 objectory-0.0.3/src/objectory/abstract_factory.py
--rw-r--r--   0        0        0      138 2023-06-25 05:56:41.511082 objectory-0.0.3/src/objectory/constants.py
--rw-r--r--   0        0        0     1511 2023-06-25 05:56:41.511082 objectory-0.0.3/src/objectory/errors.py
--rw-r--r--   0        0        0    16099 2023-06-25 05:56:41.511082 objectory-0.0.3/src/objectory/registry.py
--rw-r--r--   0        0        0     1290 2023-06-25 05:56:41.511082 objectory-0.0.3/src/objectory/universal.py
--rw-r--r--   0        0        0      373 2023-06-25 05:56:41.511082 objectory-0.0.3/src/objectory/utils/__init__.py
--rw-r--r--   0        0        0     3192 2023-06-25 05:56:41.511082 objectory-0.0.3/src/objectory/utils/name_resolution.py
--rw-r--r--   0        0        0     7469 2023-06-25 05:56:41.511082 objectory-0.0.3/src/objectory/utils/object_helpers.py
--rw-r--r--   0        0        0     5571 1970-01-01 00:00:00.000000 objectory-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-07-01 20:37:13.092293 objectory-0.0.4/LICENSE
+-rw-r--r--   0        0        0     4516 2023-07-01 20:37:13.092293 objectory-0.0.4/README.md
+-rw-r--r--   0        0        0     3829 2023-07-01 20:37:13.096293 objectory-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      280 2023-07-01 20:37:13.096293 objectory-0.0.4/src/objectory/__init__.py
+-rw-r--r--   0        0        0    13109 2023-07-01 20:37:13.096293 objectory-0.0.4/src/objectory/abstract_factory.py
+-rw-r--r--   0        0        0      138 2023-07-01 20:37:13.096293 objectory-0.0.4/src/objectory/constants.py
+-rw-r--r--   0        0        0     1511 2023-07-01 20:37:13.096293 objectory-0.0.4/src/objectory/errors.py
+-rw-r--r--   0        0        0    16099 2023-07-01 20:37:13.096293 objectory-0.0.4/src/objectory/registry.py
+-rw-r--r--   0        0        0     1290 2023-07-01 20:37:13.096293 objectory-0.0.4/src/objectory/universal.py
+-rw-r--r--   0        0        0      449 2023-07-01 20:37:13.096293 objectory-0.0.4/src/objectory/utils/__init__.py
+-rw-r--r--   0        0        0     1047 2023-07-01 20:37:13.096293 objectory-0.0.4/src/objectory/utils/config.py
+-rw-r--r--   0        0        0     3192 2023-07-01 20:37:13.096293 objectory-0.0.4/src/objectory/utils/name_resolution.py
+-rw-r--r--   0        0        0     7469 2023-07-01 20:37:13.096293 objectory-0.0.4/src/objectory/utils/object_helpers.py
+-rw-r--r--   0        0        0     5571 1970-01-01 00:00:00.000000 objectory-0.0.4/PKG-INFO
```

### Comparing `objectory-0.0.3/LICENSE` & `objectory-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `objectory-0.0.3/README.md` & `objectory-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `objectory-0.0.3/pyproject.toml` & `objectory-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "objectory"
-version = "0.0.3"
+version = "0.0.4"
 description = "A light library for general purpose object factories"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/objectory"
 repository = "https://github.com/durandtibo/objectory"
 keywords = ["factory", "abstract factory", "registry"]
 license = "BSD-3-Clause"
```

### Comparing `objectory-0.0.3/src/objectory/abstract_factory.py` & `objectory-0.0.4/src/objectory/abstract_factory.py`

 * *Files identical despite different names*

### Comparing `objectory-0.0.3/src/objectory/errors.py` & `objectory-0.0.4/src/objectory/errors.py`

 * *Files identical despite different names*

### Comparing `objectory-0.0.3/src/objectory/registry.py` & `objectory-0.0.4/src/objectory/registry.py`

 * *Files identical despite different names*

### Comparing `objectory-0.0.3/src/objectory/universal.py` & `objectory-0.0.4/src/objectory/universal.py`

 * *Files identical despite different names*

### Comparing `objectory-0.0.3/src/objectory/utils/name_resolution.py` & `objectory-0.0.4/src/objectory/utils/name_resolution.py`

 * *Files identical despite different names*

### Comparing `objectory-0.0.3/src/objectory/utils/object_helpers.py` & `objectory-0.0.4/src/objectory/utils/object_helpers.py`

 * *Files identical despite different names*

### Comparing `objectory-0.0.3/PKG-INFO` & `objectory-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objectory
-Version: 0.0.3
+Version: 0.0.4
 Summary: A light library for general purpose object factories
 Home-page: https://github.com/durandtibo/objectory
 License: BSD-3-Clause
 Keywords: factory,abstract factory,registry
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<4.0
```

