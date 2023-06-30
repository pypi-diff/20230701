# Comparing `tmp/owe_python_sdk-0.0.1.tar.gz` & `tmp/owe_python_sdk-0.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owe_python_sdk-0.0.1.tar", max compression
+gzip compressed data, was "owe_python_sdk-0.0.1a0.tar", max compression
```

## Comparing `owe_python_sdk-0.0.1.tar` & `owe_python_sdk-0.0.1a0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0        4 2023-06-30 21:31:09.785507 owe_python_sdk-0.0.1/.gitignore
--rw-r--r--   0        0        0     2385 2023-04-25 19:25:09.876316 owe_python_sdk-0.0.1/Plugin.py
--rw-r--r--   0        0        0      167 2023-04-25 19:25:09.877165 owe_python_sdk-0.0.1/SchemaExtension.py
--rw-r--r--   0        0        0      261 2023-04-25 19:25:09.982753 owe_python_sdk-0.0.1/TaskResult.py
--rw-r--r--   0        0        0       22 2023-04-25 19:25:09.981755 owe_python_sdk-0.0.1/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 20:35:08.022714 owe_python_sdk-0.0.1/client/__init__.py
--rw-r--r--   0        0        0     1022 2023-06-10 00:46:15.618643 owe_python_sdk-0.0.1/constants.py
--rw-r--r--   0        0        0      198 2023-04-25 19:25:09.980620 owe_python_sdk-0.0.1/events/Event.py
--rw-r--r--   0        0        0     2226 2023-04-25 19:25:09.979902 owe_python_sdk-0.0.1/events/EventExchange.py
--rw-r--r--   0        0        0       71 2023-04-25 19:25:09.979050 owe_python_sdk-0.0.1/events/EventHandler.py
--rw-r--r--   0        0        0      553 2023-04-25 19:25:09.977930 owe_python_sdk-0.0.1/events/EventPublisher.py
--rw-r--r--   0        0        0      611 2023-04-25 19:25:09.977301 owe_python_sdk-0.0.1/events/ExchangeConfig.py
--rw-r--r--   0        0        0      295 2023-04-25 19:25:09.883031 owe_python_sdk-0.0.1/events/__init__.py
--rw-r--r--   0        0        0      483 2023-04-25 19:25:09.976635 owe_python_sdk-0.0.1/events/types.py
--rw-r--r--   0        0        0      155 2023-04-25 19:25:09.884264 owe_python_sdk-0.0.1/middleware/EventHandlerMiddleware.py
--rw-r--r--   0        0        0       65 2023-04-25 19:25:09.884909 owe_python_sdk-0.0.1/middleware/Middleware.py
--rw-r--r--   0        0        0      107 2023-04-25 19:25:09.885902 owe_python_sdk-0.0.1/middleware/RequestMiddleware.py
--rw-r--r--   0        0        0      158 2023-04-25 19:25:09.886591 owe_python_sdk-0.0.1/middleware/__init__.py
--rw-r--r--   0        0        0      451 2023-06-30 21:30:42.642007 owe_python_sdk-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    20719 2023-06-29 00:23:41.607657 owe_python_sdk-0.0.1/schema.py
--rw-r--r--   0        0        0      359 2023-04-25 19:25:09.888964 owe_python_sdk-0.0.1/utils.py
--rw-r--r--   0        0        0      798 2023-06-30 21:32:14.023402 owe_python_sdk-0.0.1/setup.py
--rw-r--r--   0        0        0      436 2023-06-30 21:32:14.023995 owe_python_sdk-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2385 2023-06-30 21:58:22.524000 owe_python_sdk-0.0.1a0/owe_python_sdk/Plugin.py
+-rw-r--r--   0        0        0      167 2023-06-30 21:58:36.925000 owe_python_sdk-0.0.1a0/owe_python_sdk/SchemaExtension.py
+-rw-r--r--   0        0        0      261 2023-06-30 21:58:42.785000 owe_python_sdk-0.0.1a0/owe_python_sdk/TaskResult.py
+-rw-r--r--   0        0        0        0 2023-06-30 20:35:08.022714 owe_python_sdk-0.0.1a0/owe_python_sdk/client/__init__.py
+-rw-r--r--   0        0        0     1022 2023-06-30 21:58:15.734000 owe_python_sdk-0.0.1a0/owe_python_sdk/constants.py
+-rw-r--r--   0        0        0      198 2023-04-25 19:25:09.980620 owe_python_sdk-0.0.1a0/owe_python_sdk/events/Event.py
+-rw-r--r--   0        0        0     2226 2023-04-25 19:25:09.979902 owe_python_sdk-0.0.1a0/owe_python_sdk/events/EventExchange.py
+-rw-r--r--   0        0        0       71 2023-04-25 19:25:09.979050 owe_python_sdk-0.0.1a0/owe_python_sdk/events/EventHandler.py
+-rw-r--r--   0        0        0      553 2023-04-25 19:25:09.977930 owe_python_sdk-0.0.1a0/owe_python_sdk/events/EventPublisher.py
+-rw-r--r--   0        0        0      611 2023-04-25 19:25:09.977301 owe_python_sdk-0.0.1a0/owe_python_sdk/events/ExchangeConfig.py
+-rw-r--r--   0        0        0      295 2023-04-25 19:25:09.883031 owe_python_sdk-0.0.1a0/owe_python_sdk/events/__init__.py
+-rw-r--r--   0        0        0      483 2023-04-25 19:25:09.976635 owe_python_sdk-0.0.1a0/owe_python_sdk/events/types.py
+-rw-r--r--   0        0        0      155 2023-04-25 19:25:09.884264 owe_python_sdk-0.0.1a0/owe_python_sdk/middleware/EventHandlerMiddleware.py
+-rw-r--r--   0        0        0       65 2023-04-25 19:25:09.884909 owe_python_sdk-0.0.1a0/owe_python_sdk/middleware/Middleware.py
+-rw-r--r--   0        0        0      107 2023-04-25 19:25:09.885902 owe_python_sdk-0.0.1a0/owe_python_sdk/middleware/RequestMiddleware.py
+-rw-r--r--   0        0        0      158 2023-04-25 19:25:09.886591 owe_python_sdk-0.0.1a0/owe_python_sdk/middleware/__init__.py
+-rw-r--r--   0        0        0       70 2023-04-25 19:25:09.975961 owe_python_sdk-0.0.1a0/owe_python_sdk/runtime/__init__.py
+-rw-r--r--   0        0        0     1321 2023-06-12 23:19:13.242517 owe_python_sdk-0.0.1a0/owe_python_sdk/runtime/execution_context.py
+-rw-r--r--   0        0        0      337 2023-06-12 23:17:32.866264 owe_python_sdk-0.0.1a0/owe_python_sdk/runtime/runtime.py
+-rw-r--r--   0        0        0    20719 2023-06-30 21:58:29.649000 owe_python_sdk-0.0.1a0/owe_python_sdk/schema.py
+-rw-r--r--   0        0        0      359 2023-06-30 21:58:48.174000 owe_python_sdk-0.0.1a0/owe_python_sdk/utils.py
+-rw-r--r--   0        0        0      411 2023-06-30 22:00:58.014197 owe_python_sdk-0.0.1a0/pyproject.toml
+-rw-r--r--   0        0        0      768 2023-06-30 22:01:11.598279 owe_python_sdk-0.0.1a0/setup.py
+-rw-r--r--   0        0        0      438 2023-06-30 22:01:11.598683 owe_python_sdk-0.0.1a0/PKG-INFO
```

### Comparing `owe_python_sdk-0.0.1/Plugin.py` & `owe_python_sdk-0.0.1a0/owe_python_sdk/Plugin.py`

 * *Files identical despite different names*

### Comparing `owe_python_sdk-0.0.1/constants.py` & `owe_python_sdk-0.0.1a0/owe_python_sdk/constants.py`

 * *Files identical despite different names*

### Comparing `owe_python_sdk-0.0.1/events/EventExchange.py` & `owe_python_sdk-0.0.1a0/owe_python_sdk/events/EventExchange.py`

 * *Files identical despite different names*

### Comparing `owe_python_sdk-0.0.1/events/EventPublisher.py` & `owe_python_sdk-0.0.1a0/owe_python_sdk/events/EventPublisher.py`

 * *Files identical despite different names*

### Comparing `owe_python_sdk-0.0.1/events/ExchangeConfig.py` & `owe_python_sdk-0.0.1a0/owe_python_sdk/events/ExchangeConfig.py`

 * *Files identical despite different names*

### Comparing `owe_python_sdk-0.0.1/schema.py` & `owe_python_sdk-0.0.1a0/owe_python_sdk/schema.py`

 * *Files identical despite different names*

### Comparing `owe_python_sdk-0.0.1/setup.py` & `owe_python_sdk-0.0.1a0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
-package_dir = \
-{'': '.'}
-
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
-    'version': '0.0.1',
+    'version': '0.0.1a0',
     'description': '',
     'long_description': None,
     'author': 'Nathan Freeman',
     'author_email': 'nfreeman@tacc.utexas.edu.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/tapis-project/tapis-workflows',
-    'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.9,<4.0',
 }
```

