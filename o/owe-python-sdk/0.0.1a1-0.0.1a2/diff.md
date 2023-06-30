# Comparing `tmp/owe_python_sdk-0.0.1a1.tar.gz` & `tmp/owe_python_sdk-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owe_python_sdk-0.0.1a1.tar", max compression
+gzip compressed data, was "owe_python_sdk-0.0.1a2.tar", max compression
```

## Comparing `owe_python_sdk-0.0.1a1.tar` & `owe_python_sdk-0.0.1a2.tar`

### file list

```diff
@@ -1,21 +1,24 @@
--rw-r--r--   0        0        0     2385 2023-06-30 21:58:22.524000 owe_python_sdk-0.0.1a1/owe_python_sdk/Plugin.py
--rw-r--r--   0        0        0      167 2023-06-30 21:58:36.925000 owe_python_sdk-0.0.1a1/owe_python_sdk/SchemaExtension.py
--rw-r--r--   0        0        0      261 2023-06-30 21:58:42.785000 owe_python_sdk-0.0.1a1/owe_python_sdk/TaskResult.py
--rw-r--r--   0        0        0        0 2023-06-30 20:35:08.022714 owe_python_sdk-0.0.1a1/owe_python_sdk/client/__init__.py
--rw-r--r--   0        0        0     1022 2023-06-30 21:58:15.734000 owe_python_sdk-0.0.1a1/owe_python_sdk/constants.py
--rw-r--r--   0        0        0      198 2023-04-25 19:25:09.980620 owe_python_sdk-0.0.1a1/owe_python_sdk/events/Event.py
--rw-r--r--   0        0        0     2226 2023-04-25 19:25:09.979902 owe_python_sdk-0.0.1a1/owe_python_sdk/events/EventExchange.py
--rw-r--r--   0        0        0       71 2023-04-25 19:25:09.979050 owe_python_sdk-0.0.1a1/owe_python_sdk/events/EventHandler.py
--rw-r--r--   0        0        0      553 2023-04-25 19:25:09.977930 owe_python_sdk-0.0.1a1/owe_python_sdk/events/EventPublisher.py
--rw-r--r--   0        0        0      611 2023-04-25 19:25:09.977301 owe_python_sdk-0.0.1a1/owe_python_sdk/events/ExchangeConfig.py
--rw-r--r--   0        0        0      295 2023-04-25 19:25:09.883031 owe_python_sdk-0.0.1a1/owe_python_sdk/events/__init__.py
--rw-r--r--   0        0        0      483 2023-04-25 19:25:09.976635 owe_python_sdk-0.0.1a1/owe_python_sdk/events/types.py
--rw-r--r--   0        0        0      155 2023-04-25 19:25:09.884264 owe_python_sdk-0.0.1a1/owe_python_sdk/middleware/EventHandlerMiddleware.py
--rw-r--r--   0        0        0       65 2023-04-25 19:25:09.884909 owe_python_sdk-0.0.1a1/owe_python_sdk/middleware/Middleware.py
--rw-r--r--   0        0        0      107 2023-04-25 19:25:09.885902 owe_python_sdk-0.0.1a1/owe_python_sdk/middleware/RequestMiddleware.py
--rw-r--r--   0        0        0      158 2023-04-25 19:25:09.886591 owe_python_sdk-0.0.1a1/owe_python_sdk/middleware/__init__.py
--rw-r--r--   0        0        0    20719 2023-06-30 21:58:29.649000 owe_python_sdk-0.0.1a1/owe_python_sdk/schema.py
--rw-r--r--   0        0        0      359 2023-06-30 21:58:48.174000 owe_python_sdk-0.0.1a1/owe_python_sdk/utils.py
--rw-r--r--   0        0        0      427 2023-06-30 22:23:32.105213 owe_python_sdk-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0      741 2023-06-30 22:23:38.506181 owe_python_sdk-0.0.1a1/setup.py
--rw-r--r--   0        0        0      438 2023-06-30 22:23:38.506658 owe_python_sdk-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0     2385 2023-06-30 22:36:52.821000 owe_python_sdk-0.0.1a2/owe_python_sdk/Plugin.py
+-rw-r--r--   0        0        0      167 2023-06-30 22:36:54.504000 owe_python_sdk-0.0.1a2/owe_python_sdk/SchemaExtension.py
+-rw-r--r--   0        0        0      260 2023-06-30 22:47:24.040700 owe_python_sdk-0.0.1a2/owe_python_sdk/TaskResult.py
+-rw-r--r--   0        0        0        0 2023-06-30 22:46:54.916683 owe_python_sdk-0.0.1a2/owe_python_sdk/client/__init__.py
+-rw-r--r--   0        0        0     1022 2023-06-30 22:36:52.363000 owe_python_sdk-0.0.1a2/owe_python_sdk/constants.py
+-rw-r--r--   0        0        0      198 2023-04-25 19:25:09.980620 owe_python_sdk-0.0.1a2/owe_python_sdk/events/Event.py
+-rw-r--r--   0        0        0     2226 2023-04-25 19:25:09.979902 owe_python_sdk-0.0.1a2/owe_python_sdk/events/EventExchange.py
+-rw-r--r--   0        0        0       71 2023-04-25 19:25:09.979050 owe_python_sdk-0.0.1a2/owe_python_sdk/events/EventHandler.py
+-rw-r--r--   0        0        0      553 2023-04-25 19:25:09.977930 owe_python_sdk-0.0.1a2/owe_python_sdk/events/EventPublisher.py
+-rw-r--r--   0        0        0      611 2023-04-25 19:25:09.977301 owe_python_sdk-0.0.1a2/owe_python_sdk/events/ExchangeConfig.py
+-rw-r--r--   0        0        0      295 2023-04-25 19:25:09.883031 owe_python_sdk-0.0.1a2/owe_python_sdk/events/__init__.py
+-rw-r--r--   0        0        0      483 2023-04-25 19:25:09.976635 owe_python_sdk-0.0.1a2/owe_python_sdk/events/types.py
+-rw-r--r--   0        0        0      155 2023-04-25 19:25:09.884264 owe_python_sdk-0.0.1a2/owe_python_sdk/middleware/EventHandlerMiddleware.py
+-rw-r--r--   0        0        0       65 2023-04-25 19:25:09.884909 owe_python_sdk-0.0.1a2/owe_python_sdk/middleware/Middleware.py
+-rw-r--r--   0        0        0      107 2023-04-25 19:25:09.885902 owe_python_sdk-0.0.1a2/owe_python_sdk/middleware/RequestMiddleware.py
+-rw-r--r--   0        0        0      158 2023-04-25 19:25:09.886591 owe_python_sdk-0.0.1a2/owe_python_sdk/middleware/__init__.py
+-rw-r--r--   0        0        0       70 2023-04-25 19:25:09.975961 owe_python_sdk-0.0.1a2/owe_python_sdk/runtime/__init__.py
+-rw-r--r--   0        0        0     1321 2023-06-12 23:19:13.242517 owe_python_sdk-0.0.1a2/owe_python_sdk/runtime/execution_context.py
+-rw-r--r--   0        0        0      337 2023-06-12 23:17:32.866264 owe_python_sdk-0.0.1a2/owe_python_sdk/runtime/runtime.py
+-rw-r--r--   0        0        0    20719 2023-06-30 22:36:53.261000 owe_python_sdk-0.0.1a2/owe_python_sdk/schema.py
+-rw-r--r--   0        0        0      359 2023-06-30 22:36:55.689000 owe_python_sdk-0.0.1a2/owe_python_sdk/utils.py
+-rw-r--r--   0        0        0      457 2023-06-30 22:49:15.061368 owe_python_sdk-0.0.1a2/pyproject.toml
+-rw-r--r--   0        0        0      768 2023-06-30 22:49:22.165351 owe_python_sdk-0.0.1a2/setup.py
+-rw-r--r--   0        0        0      438 2023-06-30 22:49:22.166021 owe_python_sdk-0.0.1a2/PKG-INFO
```

### Comparing `owe_python_sdk-0.0.1a1/owe_python_sdk/Plugin.py` & `owe_python_sdk-0.0.1a2/owe_python_sdk/Plugin.py`

 * *Files identical despite different names*

### Comparing `owe_python_sdk-0.0.1a1/owe_python_sdk/constants.py` & `owe_python_sdk-0.0.1a2/owe_python_sdk/constants.py`

 * *Files identical despite different names*

### Comparing `owe_python_sdk-0.0.1a1/owe_python_sdk/events/EventExchange.py` & `owe_python_sdk-0.0.1a2/owe_python_sdk/events/EventExchange.py`

 * *Files identical despite different names*

### Comparing `owe_python_sdk-0.0.1a1/owe_python_sdk/events/EventPublisher.py` & `owe_python_sdk-0.0.1a2/owe_python_sdk/events/EventPublisher.py`

 * *Files identical despite different names*

### Comparing `owe_python_sdk-0.0.1a1/owe_python_sdk/events/ExchangeConfig.py` & `owe_python_sdk-0.0.1a2/owe_python_sdk/events/ExchangeConfig.py`

 * *Files identical despite different names*

### Comparing `owe_python_sdk-0.0.1a1/owe_python_sdk/schema.py` & `owe_python_sdk-0.0.1a2/owe_python_sdk/schema.py`

 * *Files identical despite different names*

### Comparing `owe_python_sdk-0.0.1a1/setup.py` & `owe_python_sdk-0.0.1a2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['owe_python_sdk',
  'owe_python_sdk.client',
  'owe_python_sdk.events',
- 'owe_python_sdk.middleware']
+ 'owe_python_sdk.middleware',
+ 'owe_python_sdk.runtime']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['pydantic>=1.10.9,<2.0.0']
 
 setup_kwargs = {
     'name': 'owe-python-sdk',
-    'version': '0.0.1a1',
+    'version': '0.0.1a2',
     'description': '',
     'long_description': None,
     'author': 'Nathan Freeman',
     'author_email': 'nfreeman@tacc.utexas.edu.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/tapis-project/tapis-workflows',
```

