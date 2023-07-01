# Comparing `tmp/cachefunc-0.1.0.tar.gz` & `tmp/cachefunc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cachefunc-0.1.0.tar", max compression
+gzip compressed data, was "cachefunc-0.2.0.tar", max compression
```

## Comparing `cachefunc-0.1.0.tar` & `cachefunc-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,9 @@
--rw-r--r--   0        0        0      141 2023-07-01 16:06:52.553259 cachefunc-0.1.0/README.md
--rw-r--r--   0        0        0       93 2023-07-01 16:06:32.184502 cachefunc-0.1.0/cachefunc/__init__.py
--rw-r--r--   0        0        0     2412 2023-07-01 16:06:32.184415 cachefunc-0.1.0/cachefunc/main.py
--rw-r--r--   0        0        0      287 2023-07-01 16:06:43.832394 cachefunc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 cachefunc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      141 2023-07-01 16:06:52.553259 cachefunc-0.2.0/README.md
+-rw-r--r--   0        0        0      222 2023-07-01 20:00:37.898378 cachefunc-0.2.0/cachefunc/__init__.py
+-rw-r--r--   0        0        0     2181 2023-07-01 19:52:19.517124 cachefunc-0.2.0/cachefunc/cache/base.py
+-rw-r--r--   0        0        0      919 2023-07-01 19:55:21.155626 cachefunc-0.2.0/cachefunc/cache/dict_cache.py
+-rw-r--r--   0        0        0      565 2023-07-01 20:00:47.770599 cachefunc-0.2.0/cachefunc/cache/redis_cache.py
+-rw-r--r--   0        0        0      680 2023-07-01 19:37:45.799914 cachefunc-0.2.0/cachefunc/log.py
+-rw-r--r--   0        0        0     1221 2023-07-01 19:56:11.198726 cachefunc-0.2.0/cachefunc/main.py
+-rw-r--r--   0        0        0      287 2023-07-01 19:15:11.509820 cachefunc-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 cachefunc-0.2.0/PKG-INFO
```

### Comparing `cachefunc-0.1.0/PKG-INFO` & `cachefunc-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cachefunc
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 License: MIT
 Author: Petrov Mikhail
 Author-email: petrov.ma@icloud.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

