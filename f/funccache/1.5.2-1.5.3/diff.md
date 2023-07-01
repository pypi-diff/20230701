# Comparing `tmp/funccache-1.5.2.tar.gz` & `tmp/funccache-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funccache-1.5.2.tar", last modified: Sat Apr 29 02:30:28 2023, max compression
+gzip compressed data, was "funccache-1.5.3.tar", last modified: Sat Jul  1 06:29:49 2023, max compression
```

## Comparing `funccache-1.5.2.tar` & `funccache-1.5.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:30:28.185546 funccache-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11388 2023-04-29 02:30:17.000000 funccache-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-04-29 02:30:28.185546 funccache-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-04-29 02:30:17.000000 funccache-1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:30:28.185546 funccache-1.5.2/funccache/
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-29 02:30:17.000000 funccache-1.5.2/funccache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-04-29 02:30:17.000000 funccache-1.5.2/funccache/i funccache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:30:28.185546 funccache-1.5.2/funccache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-04-29 02:30:28.000000 funccache-1.5.2/funccache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-29 02:30:28.000000 funccache-1.5.2/funccache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 02:30:28.000000 funccache-1.5.2/funccache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-29 02:30:28.000000 funccache-1.5.2/funccache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 02:30:28.185546 funccache-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-29 02:30:17.000000 funccache-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:29:49.874118 funccache-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11388 2023-07-01 06:29:39.000000 funccache-1.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-01 06:29:49.874118 funccache-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-01 06:29:39.000000 funccache-1.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:29:49.874118 funccache-1.5.3/funccache/
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-01 06:29:39.000000 funccache-1.5.3/funccache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-07-01 06:29:39.000000 funccache-1.5.3/funccache/i funccache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:29:49.874118 funccache-1.5.3/funccache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-01 06:29:49.000000 funccache-1.5.3/funccache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-01 06:29:49.000000 funccache-1.5.3/funccache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 06:29:49.000000 funccache-1.5.3/funccache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 06:29:49.000000 funccache-1.5.3/funccache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 06:29:49.874118 funccache-1.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-01 06:29:39.000000 funccache-1.5.3/setup.py
```

### Comparing `funccache-1.5.2/LICENSE` & `funccache-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `funccache-1.5.2/PKG-INFO` & `funccache-1.5.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: funccache
-Version: 1.5.2
+Version: 1.5.3
 Summary: 如其名，它实现缓存功能，可缓存某个函数或某个类中定义的所有方法的返回值。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/funccache
-Classifier: Environment :: Web Environment
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Topic :: Text Processing :: Indexing
-Classifier: Topic :: Utilities
-Classifier: Topic :: Internet
+Classifier: Topic :: Artistic Software
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [<img alt="LOGO" src="http://www.gqylpy.com/static/img/favicon.ico" height="21" width="21"/>](http://www.gqylpy.com)
 [![Release](https://img.shields.io/github/release/gqylpy/funccache.svg?style=flat-square")](https://github.com/gqylpy/funccache/releases/latest)
 [![Python Versions](https://img.shields.io/pypi/pyversions/funccache)](https://pypi.org/project/funccache)
```

### Comparing `funccache-1.5.2/README.md` & `funccache-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `funccache-1.5.2/funccache/__init__.py` & `funccache-1.5.3/funccache/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     >>> class Alpha(metaclass=funccache):
     >>>     ...
 
     >>> @funccache
     >>> def alpha():
     >>>     ...
 
-    @version: 1.5.2
+    @version: 1.5.3
     @author: 竹永康 <gqylpy@outlook.com>
     @source: https://github.com/gqylpy/funccache
 
 ────────────────────────────────────────────────────────────────────────────────
 Copyright (c) 2022, 2023 GQYLPY <http://gqylpy.com>. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `funccache-1.5.2/funccache/i funccache.py` & `funccache-1.5.3/funccache/i funccache.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,16 +169,21 @@
         key = self.__name__, a, str(kw)
 
         try:
             cache: dict = __cache_pool__[key]
         except KeyError:
             cache = __cache_pool__[key] = {}
             cache['__exec_lock__'] = threading.Event()
-            cache['__return__'] = self.__sget(self.__name__)(*a, **kw)
-            cache['__exec_lock__'].set()
+            try:
+                cache['__return__'] = self.__sget(self.__name__)(*a, **kw)
+            except Exception as e:
+                del __cache_pool__[key]
+                raise e from None
+            finally:
+                cache['__exec_lock__'].set()
         else:
             if '__exec_lock__' in cache:
                 cache['__exec_lock__'].wait()
                 try:
                     del cache['__exec_lock__']
                 except KeyError:
                     pass
@@ -257,29 +262,29 @@
         inner.__cache_pool__ = self.__cache_pool__
 
         return inner
 
     def __core__(self, func, *a, **kw):
         key = a, str(kw)
 
-        if key not in self.__cache_pool__ or self.__cache_pool__[key][
-                '__expiration_time__'] < time.time():
+        if key not in self.__cache_pool__ or \
+                self.__cache_pool__[key]['__expiration_time__'] < time.time():
             with self.__exec_lock__:
                 self.__cache_pool__[key] = {
                     '__return__': func(*a, **kw),
                     '__expiration_time__': time.time() + self.__expires
                 }
 
         return self.__cache_pool__[key]['__return__']
 
     async def __core_async__(self, func, *a, **kw):
         key = a, str(kw)
 
-        if key not in self.__cache_pool__ or self.__cache_pool__[key][
-                '__expiration_time__'] < time.time():
+        if key not in self.__cache_pool__ or \
+                self.__cache_pool__[key]['__expiration_time__'] < time.time():
             with self.__exec_lock__:
                 self.__cache_pool__[key] = {
                     '__return__': await func(*a, **kw),
                     '__expiration_time__': time.time() + self.__expires
                 }
 
         return self.__cache_pool__[key]['__return__']
```

### Comparing `funccache-1.5.2/funccache.egg-info/PKG-INFO` & `funccache-1.5.3/funccache.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: funccache
-Version: 1.5.2
+Version: 1.5.3
 Summary: 如其名，它实现缓存功能，可缓存某个函数或某个类中定义的所有方法的返回值。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/funccache
-Classifier: Environment :: Web Environment
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Topic :: Text Processing :: Indexing
-Classifier: Topic :: Utilities
-Classifier: Topic :: Internet
+Classifier: Topic :: Artistic Software
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [<img alt="LOGO" src="http://www.gqylpy.com/static/img/favicon.ico" height="21" width="21"/>](http://www.gqylpy.com)
 [![Release](https://img.shields.io/github/release/gqylpy/funccache.svg?style=flat-square")](https://github.com/gqylpy/funccache/releases/latest)
 [![Python Versions](https://img.shields.io/pypi/pyversions/funccache)](https://pypi.org/project/funccache)
```

