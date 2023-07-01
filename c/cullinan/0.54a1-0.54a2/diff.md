# Comparing `tmp/cullinan-0.54a1.tar.gz` & `tmp/cullinan-0.54a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cullinan-0.54a1.tar", last modified: Sat Jul  1 16:48:24 2023, max compression
+gzip compressed data, was "cullinan-0.54a2.tar", last modified: Sat Jul  1 17:01:19 2023, max compression
```

## Comparing `cullinan-0.54a1.tar` & `cullinan-0.54a2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:48:24.073813 cullinan-0.54a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-07-01 16:48:11.000000 cullinan-0.54a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-01 16:48:24.073813 cullinan-0.54a1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:48:24.069812 cullinan-0.54a1/cullinan/
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-07-01 16:48:11.000000 cullinan-0.54a1/cullinan/application.py
--rw-r--r--   0 runner    (1001) docker     (123)    24818 2023-07-01 16:48:11.000000 cullinan-0.54a1/cullinan/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-01 16:48:11.000000 cullinan-0.54a1/cullinan/dao.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-01 16:48:11.000000 cullinan-0.54a1/cullinan/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-01 16:48:11.000000 cullinan-0.54a1/cullinan/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-01 16:48:11.000000 cullinan-0.54a1/cullinan/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:48:24.069812 cullinan-0.54a1/cullinan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-01 16:48:24.000000 cullinan-0.54a1/cullinan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-01 16:48:24.000000 cullinan-0.54a1/cullinan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 16:48:24.000000 cullinan-0.54a1/cullinan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 16:48:24.000000 cullinan-0.54a1/cullinan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-01 16:48:24.000000 cullinan-0.54a1/cullinan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 16:48:24.073813 cullinan-0.54a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-01 16:48:11.000000 cullinan-0.54a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:01:19.602800 cullinan-0.54a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-07-01 17:01:09.000000 cullinan-0.54a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-01 17:01:19.602800 cullinan-0.54a2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:01:19.602800 cullinan-0.54a2/cullinan/
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-07-01 17:01:09.000000 cullinan-0.54a2/cullinan/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24818 2023-07-01 17:01:09.000000 cullinan-0.54a2/cullinan/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-01 17:01:09.000000 cullinan-0.54a2/cullinan/dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-01 17:01:09.000000 cullinan-0.54a2/cullinan/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-01 17:01:09.000000 cullinan-0.54a2/cullinan/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-01 17:01:09.000000 cullinan-0.54a2/cullinan/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:01:19.602800 cullinan-0.54a2/cullinan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-01 17:01:19.000000 cullinan-0.54a2/cullinan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-01 17:01:19.000000 cullinan-0.54a2/cullinan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 17:01:19.000000 cullinan-0.54a2/cullinan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 17:01:19.000000 cullinan-0.54a2/cullinan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-01 17:01:19.000000 cullinan-0.54a2/cullinan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 17:01:19.602800 cullinan-0.54a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-01 17:01:09.000000 cullinan-0.54a2/setup.py
```

### Comparing `cullinan-0.54a1/LICENSE` & `cullinan-0.54a2/LICENSE`

 * *Files identical despite different names*

### Comparing `cullinan-0.54a1/PKG-INFO` & `cullinan-0.54a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cullinan
-Version: 0.54a1
+Version: 0.54a2
 Summary: Cullinan is written based on tornado and Sqlalchemy to help the project quickly build web application
 Home-page: https://github.com/plumeink/Cullinan
 Author: plumeink
 Author-email: official@plumeink.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Source, https://github.com/plumeink/Cullinan
 Project-URL: Wiki, https://github.com/plumeink/Cullinan/wiki
```

### Comparing `cullinan-0.54a1/cullinan/application.py` & `cullinan-0.54a2/cullinan/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,16 @@
         if url_list[index] == '([a-zA-Z0-9-]+)':
             index_list.append(index)
     index_list.append('*')
     return index_list
 
 
 def sort_url():
+    if handler_list.__len__() == 0:
+        return
     handler_list_length = []
     for index in range(0, handler_list.__len__()):
         handler_list[index] = list(handler_list[index])
         handler_list[index][0] = handler_list[index][0].split('/')
         index_list = get_index_list(handler_list[index][0])
         handler_list_length.append(index_list.__len__())
         handler_list[index].append(index_list)
```

### Comparing `cullinan-0.54a1/cullinan/controller.py` & `cullinan-0.54a2/cullinan/controller.py`

 * *Files identical despite different names*

### Comparing `cullinan-0.54a1/cullinan/dao.py` & `cullinan-0.54a2/cullinan/dao.py`

 * *Files identical despite different names*

### Comparing `cullinan-0.54a1/cullinan/request.py` & `cullinan-0.54a2/cullinan/request.py`

 * *Files identical despite different names*

### Comparing `cullinan-0.54a1/cullinan/service.py` & `cullinan-0.54a2/cullinan/service.py`

 * *Files identical despite different names*

### Comparing `cullinan-0.54a1/cullinan.egg-info/PKG-INFO` & `cullinan-0.54a2/cullinan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cullinan
-Version: 0.54a1
+Version: 0.54a2
 Summary: Cullinan is written based on tornado and Sqlalchemy to help the project quickly build web application
 Home-page: https://github.com/plumeink/Cullinan
 Author: plumeink
 Author-email: official@plumeink.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Source, https://github.com/plumeink/Cullinan
 Project-URL: Wiki, https://github.com/plumeink/Cullinan/wiki
```

### Comparing `cullinan-0.54a1/setup.py` & `cullinan-0.54a2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.MD", "r", encoding="UTF-8") as fh:
     long_description = fh.read()
 
 setup(
     name='cullinan',
-    version='0.54a1',
+    version='0.54a2',
     packages=['cullinan'],
     description='Cullinan is written based on tornado and Sqlalchemy to help the project quickly build web application',
     author='plumeink',
     project_urls={
             'Source': 'https://github.com/plumeink/Cullinan',
             'Wiki': 'https://github.com/plumeink/Cullinan/wiki',
       },
```

