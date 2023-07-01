# Comparing `tmp/cachefunc-0.2.2.tar.gz` & `tmp/cachefunc-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cachefunc-0.2.2.tar", max compression
+gzip compressed data, was "cachefunc-0.2.3.tar", max compression
```

## Comparing `cachefunc-0.2.2.tar` & `cachefunc-0.2.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      141 2023-07-01 16:06:52.553259 cachefunc-0.2.2/README.md
--rw-r--r--   0        0        0      222 2023-07-01 20:11:47.197988 cachefunc-0.2.2/cachefunc/__init__.py
--rw-r--r--   0        0        0     2181 2023-07-01 20:11:47.198253 cachefunc-0.2.2/cachefunc/cache/base.py
--rw-r--r--   0        0        0      919 2023-07-01 20:11:47.198477 cachefunc-0.2.2/cachefunc/cache/dict_cache.py
--rw-r--r--   0        0        0      565 2023-07-01 20:11:47.198686 cachefunc-0.2.2/cachefunc/cache/redis_cache.py
--rw-r--r--   0        0        0      680 2023-07-01 20:19:20.506787 cachefunc-0.2.2/cachefunc/log.py
--rw-r--r--   0        0        0     1190 2023-07-01 20:25:52.221635 cachefunc-0.2.2/cachefunc/main.py
--rw-r--r--   0        0        0      287 2023-07-01 20:26:11.818201 cachefunc-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 cachefunc-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      196 2023-07-01 20:34:00.051916 cachefunc-0.2.3/README.md
+-rw-r--r--   0        0        0      222 2023-07-01 20:11:47.197988 cachefunc-0.2.3/cachefunc/__init__.py
+-rw-r--r--   0        0        0     2181 2023-07-01 20:11:47.198253 cachefunc-0.2.3/cachefunc/cache/base.py
+-rw-r--r--   0        0        0      919 2023-07-01 20:11:47.198477 cachefunc-0.2.3/cachefunc/cache/dict_cache.py
+-rw-r--r--   0        0        0      565 2023-07-01 20:11:47.198686 cachefunc-0.2.3/cachefunc/cache/redis_cache.py
+-rw-r--r--   0        0        0      680 2023-07-01 20:19:20.506787 cachefunc-0.2.3/cachefunc/log.py
+-rw-r--r--   0        0        0     1190 2023-07-01 20:25:52.221635 cachefunc-0.2.3/cachefunc/main.py
+-rw-r--r--   0        0        0      287 2023-07-01 20:34:34.884602 cachefunc-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      651 1970-01-01 00:00:00.000000 cachefunc-0.2.3/PKG-INFO
```

### Comparing `cachefunc-0.2.2/cachefunc/cache/base.py` & `cachefunc-0.2.3/cachefunc/cache/base.py`

 * *Files identical despite different names*

### Comparing `cachefunc-0.2.2/cachefunc/cache/dict_cache.py` & `cachefunc-0.2.3/cachefunc/cache/dict_cache.py`

 * *Files identical despite different names*

### Comparing `cachefunc-0.2.2/cachefunc/cache/redis_cache.py` & `cachefunc-0.2.3/cachefunc/cache/redis_cache.py`

 * *Files identical despite different names*

### Comparing `cachefunc-0.2.2/cachefunc/log.py` & `cachefunc-0.2.3/cachefunc/log.py`

 * *Files identical despite different names*

### Comparing `cachefunc-0.2.2/cachefunc/main.py` & `cachefunc-0.2.3/cachefunc/main.py`

 * *Files identical despite different names*

### Comparing `cachefunc-0.2.2/PKG-INFO` & `cachefunc-0.2.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cachefunc
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 License: MIT
 Author: Petrov Mikhail
 Author-email: petrov.ma@icloud.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,10 +13,12 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # cachefunc
 
 Library for caching functions and coroutines result with decorators
 
+## [Homepage](https://github.com/ma-petrov/cachefunc)
+
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
```

