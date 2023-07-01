# Comparing `tmp/lessweb-1.0.7.tar.gz` & `tmp/lessweb-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lessweb-1.0.7.tar", last modified: Mon Apr 10 04:55:52 2023, max compression
+gzip compressed data, was "lessweb-1.0.8.tar", last modified: Sat Jul  1 14:50:29 2023, max compression
```

## Comparing `lessweb-1.0.7.tar` & `lessweb-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-04-10 04:55:52.587458 lessweb-1.0.7/
--rw-r--r--   0 zhangji    (501) staff       (20)      556 2022-11-14 08:34:51.000000 lessweb-1.0.7/LICENSE.txt
--rw-r--r--   0 zhangji    (501) staff       (20)      356 2023-04-10 04:55:52.586660 lessweb-1.0.7/PKG-INFO
--rw-r--r--   0 zhangji    (501) staff       (20)     1649 2022-12-06 09:47:53.000000 lessweb-1.0.7/README.md
-drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-04-10 04:55:52.576064 lessweb-1.0.7/lessweb/
--rw-r--r--   0 zhangji    (501) staff       (20)      255 2023-04-10 04:54:53.000000 lessweb-1.0.7/lessweb/__init__.py
--rw-r--r--   0 zhangji    (501) staff       (20)    14206 2023-04-10 04:54:53.000000 lessweb-1.0.7/lessweb/bridge.py
--rw-r--r--   0 zhangji    (501) staff       (20)        0 2023-01-14 08:15:49.000000 lessweb-1.0.7/lessweb/py.typed
--rw-r--r--   0 zhangji    (501) staff       (20)     7860 2023-01-14 07:25:23.000000 lessweb-1.0.7/lessweb/typecast.py
-drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-04-10 04:55:52.585582 lessweb-1.0.7/lessweb.egg-info/
--rw-r--r--   0 zhangji    (501) staff       (20)      356 2023-04-10 04:55:52.000000 lessweb-1.0.7/lessweb.egg-info/PKG-INFO
--rw-r--r--   0 zhangji    (501) staff       (20)      293 2023-04-10 04:55:52.000000 lessweb-1.0.7/lessweb.egg-info/SOURCES.txt
--rw-r--r--   0 zhangji    (501) staff       (20)        1 2023-04-10 04:55:52.000000 lessweb-1.0.7/lessweb.egg-info/dependency_links.txt
--rw-r--r--   0 zhangji    (501) staff       (20)       20 2023-04-10 04:55:52.000000 lessweb-1.0.7/lessweb.egg-info/entry_points.txt
--rw-r--r--   0 zhangji    (501) staff       (20)       43 2023-04-10 04:55:52.000000 lessweb-1.0.7/lessweb.egg-info/requires.txt
--rw-r--r--   0 zhangji    (501) staff       (20)        8 2023-04-10 04:55:52.000000 lessweb-1.0.7/lessweb.egg-info/top_level.txt
--rw-r--r--   0 zhangji    (501) staff       (20)       38 2023-04-10 04:55:52.587725 lessweb-1.0.7/setup.cfg
--rw-r--r--   0 zhangji    (501) staff       (20)     1124 2023-01-14 09:41:41.000000 lessweb-1.0.7/setup.py
+drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-07-01 14:50:29.005907 lessweb-1.0.8/
+-rw-r--r--   0 zhangji    (501) staff       (20)      556 2022-11-14 08:34:51.000000 lessweb-1.0.8/LICENSE.txt
+-rw-r--r--   0 zhangji    (501) staff       (20)     1924 2023-07-01 14:50:29.005356 lessweb-1.0.8/PKG-INFO
+-rw-r--r--   0 zhangji    (501) staff       (20)     1649 2022-12-06 09:47:53.000000 lessweb-1.0.8/README.md
+drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-07-01 14:50:28.995933 lessweb-1.0.8/lessweb/
+-rw-r--r--   0 zhangji    (501) staff       (20)      255 2023-04-23 13:41:17.000000 lessweb-1.0.8/lessweb/__init__.py
+-rw-r--r--   0 zhangji    (501) staff       (20)    14244 2023-04-23 13:41:06.000000 lessweb-1.0.8/lessweb/bridge.py
+-rw-r--r--   0 zhangji    (501) staff       (20)        0 2023-01-14 08:15:49.000000 lessweb-1.0.8/lessweb/py.typed
+-rw-r--r--   0 zhangji    (501) staff       (20)     7860 2023-01-14 07:25:23.000000 lessweb-1.0.8/lessweb/typecast.py
+drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-07-01 14:50:29.004679 lessweb-1.0.8/lessweb.egg-info/
+-rw-r--r--   0 zhangji    (501) staff       (20)     1924 2023-07-01 14:50:28.000000 lessweb-1.0.8/lessweb.egg-info/PKG-INFO
+-rw-r--r--   0 zhangji    (501) staff       (20)      265 2023-07-01 14:50:28.000000 lessweb-1.0.8/lessweb.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangji    (501) staff       (20)        1 2023-07-01 14:50:28.000000 lessweb-1.0.8/lessweb.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangji    (501) staff       (20)       43 2023-07-01 14:50:28.000000 lessweb-1.0.8/lessweb.egg-info/requires.txt
+-rw-r--r--   0 zhangji    (501) staff       (20)        8 2023-07-01 14:50:28.000000 lessweb-1.0.8/lessweb.egg-info/top_level.txt
+-rw-r--r--   0 zhangji    (501) staff       (20)      520 2023-07-01 14:36:46.000000 lessweb-1.0.8/pyproject.toml
+-rw-r--r--   0 zhangji    (501) staff       (20)       38 2023-07-01 14:50:29.006080 lessweb-1.0.8/setup.cfg
```

### Comparing `lessweb-1.0.7/LICENSE.txt` & `lessweb-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lessweb-1.0.7/README.md` & `lessweb-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `lessweb-1.0.7/lessweb/bridge.py` & `lessweb-1.0.8/lessweb/bridge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from aiohttp.web import Request, Application, Response, middleware, HTTPBadRequest, HTTPError, run_app
 from aiohttp.typedefs import LooseHeaders
-from dataclasses import dataclass
+from dataclasses import dataclass, is_dataclass
 import importlib
 import inspect
 import logging
 from logging.handlers import TimedRotatingFileHandler
 import orjson
 from os import environ, listdir
 import re
@@ -255,15 +255,15 @@
                     try:
                         kwargs[name] = typecast(chosen_value, depends_type)
                     except Exception:
                         raise HTTPBadRequest(text=f'BadRequest: invalid parameter: {name}')
             else:
                 kwargs[name] = autowire(request, depends_type, name)
         result = await sp_endpoint(*args, **kwargs)
-        if isinstance(result, (dict, list)):
+        if isinstance(result, (dict, list)) or is_dataclass(result):
             return rest_response(result)
         else:
             return result
 
     return aio_endpoint
```

### Comparing `lessweb-1.0.7/lessweb/typecast.py` & `lessweb-1.0.8/lessweb/typecast.py`

 * *Files identical despite different names*

