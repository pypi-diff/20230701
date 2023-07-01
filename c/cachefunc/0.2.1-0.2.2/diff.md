# Comparing `tmp/cachefunc-0.2.1.tar.gz` & `tmp/cachefunc-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cachefunc-0.2.1.tar", max compression
+gzip compressed data, was "cachefunc-0.2.2.tar", max compression
```

## Comparing `cachefunc-0.2.1.tar` & `cachefunc-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      141 2023-07-01 16:06:52.553259 cachefunc-0.2.1/README.md
--rw-r--r--   0        0        0      222 2023-07-01 20:11:47.197988 cachefunc-0.2.1/cachefunc/__init__.py
--rw-r--r--   0        0        0     2181 2023-07-01 20:11:47.198253 cachefunc-0.2.1/cachefunc/cache/base.py
--rw-r--r--   0        0        0      919 2023-07-01 20:11:47.198477 cachefunc-0.2.1/cachefunc/cache/dict_cache.py
--rw-r--r--   0        0        0      565 2023-07-01 20:11:47.198686 cachefunc-0.2.1/cachefunc/cache/redis_cache.py
--rw-r--r--   0        0        0      680 2023-07-01 20:19:20.506787 cachefunc-0.2.1/cachefunc/log.py
--rw-r--r--   0        0        0     1221 2023-07-01 20:11:47.199174 cachefunc-0.2.1/cachefunc/main.py
--rw-r--r--   0        0        0      287 2023-07-01 20:17:54.139654 cachefunc-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 cachefunc-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      141 2023-07-01 16:06:52.553259 cachefunc-0.2.2/README.md
+-rw-r--r--   0        0        0      222 2023-07-01 20:11:47.197988 cachefunc-0.2.2/cachefunc/__init__.py
+-rw-r--r--   0        0        0     2181 2023-07-01 20:11:47.198253 cachefunc-0.2.2/cachefunc/cache/base.py
+-rw-r--r--   0        0        0      919 2023-07-01 20:11:47.198477 cachefunc-0.2.2/cachefunc/cache/dict_cache.py
+-rw-r--r--   0        0        0      565 2023-07-01 20:11:47.198686 cachefunc-0.2.2/cachefunc/cache/redis_cache.py
+-rw-r--r--   0        0        0      680 2023-07-01 20:19:20.506787 cachefunc-0.2.2/cachefunc/log.py
+-rw-r--r--   0        0        0     1190 2023-07-01 20:25:52.221635 cachefunc-0.2.2/cachefunc/main.py
+-rw-r--r--   0        0        0      287 2023-07-01 20:26:11.818201 cachefunc-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 cachefunc-0.2.2/PKG-INFO
```

### Comparing `cachefunc-0.2.1/cachefunc/cache/base.py` & `cachefunc-0.2.2/cachefunc/cache/base.py`

 * *Files identical despite different names*

### Comparing `cachefunc-0.2.1/cachefunc/cache/dict_cache.py` & `cachefunc-0.2.2/cachefunc/cache/dict_cache.py`

 * *Files identical despite different names*

### Comparing `cachefunc-0.2.1/cachefunc/cache/redis_cache.py` & `cachefunc-0.2.2/cachefunc/cache/redis_cache.py`

 * *Files identical despite different names*

### Comparing `cachefunc-0.2.1/cachefunc/log.py` & `cachefunc-0.2.2/cachefunc/log.py`

 * *Files identical despite different names*

### Comparing `cachefunc-0.2.1/cachefunc/main.py` & `cachefunc-0.2.2/cachefunc/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from contextlib import suppress
-from datetime import timedelta
 from functools import wraps
 from typing import Any, Callable, Coroutine
 
 from cachefunc.cache.base import BaseCache, NotCached
 from cachefunc.cache.dict_cache import DictCache
```

### Comparing `cachefunc-0.2.1/PKG-INFO` & `cachefunc-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cachefunc
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 License: MIT
 Author: Petrov Mikhail
 Author-email: petrov.ma@icloud.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

