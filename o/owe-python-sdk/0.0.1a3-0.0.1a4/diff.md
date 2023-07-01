# Comparing `tmp/owe_python_sdk-0.0.1a3.tar.gz` & `tmp/owe_python_sdk-0.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owe_python_sdk-0.0.1a3.tar", max compression
+gzip compressed data, was "owe_python_sdk-0.0.1a4.tar", max compression
```

## Comparing `owe_python_sdk-0.0.1a3.tar` & `owe_python_sdk-0.0.1a4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     2385 2023-06-30 22:36:52.821000 owe_python_sdk-0.0.1a3/owe_python_sdk/Plugin.py
--rw-r--r--   0        0        0      167 2023-06-30 22:36:54.504000 owe_python_sdk-0.0.1a3/owe_python_sdk/SchemaExtension.py
--rw-r--r--   0        0        0      260 2023-06-30 22:47:24.040700 owe_python_sdk-0.0.1a3/owe_python_sdk/TaskResult.py
--rw-r--r--   0        0        0     1067 2023-07-01 21:11:40.022061 owe_python_sdk-0.0.1a3/owe_python_sdk/client/__init__.py
--rw-r--r--   0        0        0     1022 2023-06-30 22:36:52.363000 owe_python_sdk-0.0.1a3/owe_python_sdk/constants.py
--rw-r--r--   0        0        0      198 2023-04-25 19:25:09.980620 owe_python_sdk-0.0.1a3/owe_python_sdk/events/Event.py
--rw-r--r--   0        0        0     2226 2023-04-25 19:25:09.979902 owe_python_sdk-0.0.1a3/owe_python_sdk/events/EventExchange.py
--rw-r--r--   0        0        0       71 2023-04-25 19:25:09.979050 owe_python_sdk-0.0.1a3/owe_python_sdk/events/EventHandler.py
--rw-r--r--   0        0        0      553 2023-04-25 19:25:09.977930 owe_python_sdk-0.0.1a3/owe_python_sdk/events/EventPublisher.py
--rw-r--r--   0        0        0      611 2023-04-25 19:25:09.977301 owe_python_sdk-0.0.1a3/owe_python_sdk/events/ExchangeConfig.py
--rw-r--r--   0        0        0      295 2023-04-25 19:25:09.883031 owe_python_sdk-0.0.1a3/owe_python_sdk/events/__init__.py
--rw-r--r--   0        0        0      483 2023-04-25 19:25:09.976635 owe_python_sdk-0.0.1a3/owe_python_sdk/events/types.py
--rw-r--r--   0        0        0      155 2023-04-25 19:25:09.884264 owe_python_sdk-0.0.1a3/owe_python_sdk/middleware/EventHandlerMiddleware.py
--rw-r--r--   0        0        0       65 2023-04-25 19:25:09.884909 owe_python_sdk-0.0.1a3/owe_python_sdk/middleware/Middleware.py
--rw-r--r--   0        0        0      107 2023-04-25 19:25:09.885902 owe_python_sdk-0.0.1a3/owe_python_sdk/middleware/RequestMiddleware.py
--rw-r--r--   0        0        0      158 2023-04-25 19:25:09.886591 owe_python_sdk-0.0.1a3/owe_python_sdk/middleware/__init__.py
--rw-r--r--   0        0        0       70 2023-04-25 19:25:09.975961 owe_python_sdk-0.0.1a3/owe_python_sdk/runtime/__init__.py
--rw-r--r--   0        0        0     1321 2023-06-12 23:19:13.242517 owe_python_sdk-0.0.1a3/owe_python_sdk/runtime/execution_context.py
--rw-r--r--   0        0        0      337 2023-06-12 23:17:32.866264 owe_python_sdk-0.0.1a3/owe_python_sdk/runtime/runtime.py
--rw-r--r--   0        0        0    20719 2023-06-30 22:36:53.261000 owe_python_sdk-0.0.1a3/owe_python_sdk/schema.py
--rw-r--r--   0        0        0      359 2023-06-30 22:36:55.689000 owe_python_sdk-0.0.1a3/owe_python_sdk/utils.py
--rw-r--r--   0        0        0      457 2023-07-01 21:15:52.359766 owe_python_sdk-0.0.1a3/pyproject.toml
--rw-r--r--   0        0        0      768 2023-07-01 21:18:05.429746 owe_python_sdk-0.0.1a3/setup.py
--rw-r--r--   0        0        0      438 2023-07-01 21:18:05.430045 owe_python_sdk-0.0.1a3/PKG-INFO
+-rw-r--r--   0        0        0     2385 2023-06-30 22:36:52.821000 owe_python_sdk-0.0.1a4/owe_python_sdk/Plugin.py
+-rw-r--r--   0        0        0      167 2023-06-30 22:36:54.504000 owe_python_sdk-0.0.1a4/owe_python_sdk/SchemaExtension.py
+-rw-r--r--   0        0        0      260 2023-06-30 22:47:24.040700 owe_python_sdk-0.0.1a4/owe_python_sdk/TaskResult.py
+-rw-r--r--   0        0        0     1071 2023-07-01 21:24:46.143379 owe_python_sdk-0.0.1a4/owe_python_sdk/client/__init__.py
+-rw-r--r--   0        0        0     1022 2023-06-30 22:36:52.363000 owe_python_sdk-0.0.1a4/owe_python_sdk/constants.py
+-rw-r--r--   0        0        0      198 2023-04-25 19:25:09.980620 owe_python_sdk-0.0.1a4/owe_python_sdk/events/Event.py
+-rw-r--r--   0        0        0     2226 2023-04-25 19:25:09.979902 owe_python_sdk-0.0.1a4/owe_python_sdk/events/EventExchange.py
+-rw-r--r--   0        0        0       71 2023-04-25 19:25:09.979050 owe_python_sdk-0.0.1a4/owe_python_sdk/events/EventHandler.py
+-rw-r--r--   0        0        0      553 2023-04-25 19:25:09.977930 owe_python_sdk-0.0.1a4/owe_python_sdk/events/EventPublisher.py
+-rw-r--r--   0        0        0      611 2023-04-25 19:25:09.977301 owe_python_sdk-0.0.1a4/owe_python_sdk/events/ExchangeConfig.py
+-rw-r--r--   0        0        0      295 2023-04-25 19:25:09.883031 owe_python_sdk-0.0.1a4/owe_python_sdk/events/__init__.py
+-rw-r--r--   0        0        0      483 2023-04-25 19:25:09.976635 owe_python_sdk-0.0.1a4/owe_python_sdk/events/types.py
+-rw-r--r--   0        0        0      155 2023-04-25 19:25:09.884264 owe_python_sdk-0.0.1a4/owe_python_sdk/middleware/EventHandlerMiddleware.py
+-rw-r--r--   0        0        0       65 2023-04-25 19:25:09.884909 owe_python_sdk-0.0.1a4/owe_python_sdk/middleware/Middleware.py
+-rw-r--r--   0        0        0      107 2023-04-25 19:25:09.885902 owe_python_sdk-0.0.1a4/owe_python_sdk/middleware/RequestMiddleware.py
+-rw-r--r--   0        0        0      158 2023-04-25 19:25:09.886591 owe_python_sdk-0.0.1a4/owe_python_sdk/middleware/__init__.py
+-rw-r--r--   0        0        0       70 2023-04-25 19:25:09.975961 owe_python_sdk-0.0.1a4/owe_python_sdk/runtime/__init__.py
+-rw-r--r--   0        0        0     1321 2023-06-12 23:19:13.242517 owe_python_sdk-0.0.1a4/owe_python_sdk/runtime/execution_context.py
+-rw-r--r--   0        0        0      337 2023-06-12 23:17:32.866264 owe_python_sdk-0.0.1a4/owe_python_sdk/runtime/runtime.py
+-rw-r--r--   0        0        0    20719 2023-06-30 22:36:53.261000 owe_python_sdk-0.0.1a4/owe_python_sdk/schema.py
+-rw-r--r--   0        0        0      359 2023-06-30 22:36:55.689000 owe_python_sdk-0.0.1a4/owe_python_sdk/utils.py
+-rw-r--r--   0        0        0      457 2023-07-01 21:24:59.771022 owe_python_sdk-0.0.1a4/pyproject.toml
+-rw-r--r--   0        0        0      768 2023-07-01 21:25:10.844260 owe_python_sdk-0.0.1a4/setup.py
+-rw-r--r--   0        0        0      438 2023-07-01 21:25:10.844859 owe_python_sdk-0.0.1a4/PKG-INFO
```

### Comparing `owe_python_sdk-0.0.1a3/owe_python_sdk/Plugin.py` & `owe_python_sdk-0.0.1a4/owe_python_sdk/Plugin.py`

 * *Files identical despite different names*

### Comparing `owe_python_sdk-0.0.1a3/owe_python_sdk/client/__init__.py` & `owe_python_sdk-0.0.1a4/owe_python_sdk/client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import List
 
 from owe_python_sdk import schema as owe_schema
 
 
 class Task:
     def __init__(self, schema: dict):
-        self.schema = owe_schema.Task(**schema)
+        self.schema = owe_schema.BaseTask(**schema)
 
     def depends_on(self, task: Task, *tasks: List[Task]) -> None:
         dependencies = [task, *tasks]
         for dep in dependencies:
             if type(dep) != self.__class__.__name__:
                 raise TypeError(f"Task dependencies must be of type {self.__class__.__name__} | Recieved {type(dep)}")
```

### Comparing `owe_python_sdk-0.0.1a3/owe_python_sdk/constants.py` & `owe_python_sdk-0.0.1a4/owe_python_sdk/constants.py`

 * *Files identical despite different names*

### Comparing `owe_python_sdk-0.0.1a3/owe_python_sdk/events/EventExchange.py` & `owe_python_sdk-0.0.1a4/owe_python_sdk/events/EventExchange.py`

 * *Files identical despite different names*

### Comparing `owe_python_sdk-0.0.1a3/owe_python_sdk/events/EventPublisher.py` & `owe_python_sdk-0.0.1a4/owe_python_sdk/events/EventPublisher.py`

 * *Files identical despite different names*

### Comparing `owe_python_sdk-0.0.1a3/owe_python_sdk/events/ExchangeConfig.py` & `owe_python_sdk-0.0.1a4/owe_python_sdk/events/ExchangeConfig.py`

 * *Files identical despite different names*

### Comparing `owe_python_sdk-0.0.1a3/owe_python_sdk/runtime/execution_context.py` & `owe_python_sdk-0.0.1a4/owe_python_sdk/runtime/execution_context.py`

 * *Files identical despite different names*

### Comparing `owe_python_sdk-0.0.1a3/owe_python_sdk/schema.py` & `owe_python_sdk-0.0.1a4/owe_python_sdk/schema.py`

 * *Files identical despite different names*

### Comparing `owe_python_sdk-0.0.1a3/setup.py` & `owe_python_sdk-0.0.1a4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pydantic>=1.10.9,<2.0.0']
 
 setup_kwargs = {
     'name': 'owe-python-sdk',
-    'version': '0.0.1a3',
+    'version': '0.0.1a4',
     'description': '',
     'long_description': None,
     'author': 'Nathan Freeman',
     'author_email': 'nfreeman@tacc.utexas.edu.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/tapis-project/tapis-workflows',
```

