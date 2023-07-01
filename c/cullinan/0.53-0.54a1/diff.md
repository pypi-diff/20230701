# Comparing `tmp/cullinan-0.53.tar.gz` & `tmp/cullinan-0.54a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cullinan-0.53.tar", last modified: Tue Jun 27 06:05:37 2023, max compression
+gzip compressed data, was "cullinan-0.54a1.tar", last modified: Sat Jul  1 16:48:24 2023, max compression
```

## Comparing `cullinan-0.53.tar` & `cullinan-0.54a1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:05:37.924179 cullinan-0.53/
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-06-27 06:05:25.000000 cullinan-0.53/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-27 06:05:37.924179 cullinan-0.53/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:05:37.924179 cullinan-0.53/cullinan/
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-06-27 06:05:25.000000 cullinan-0.53/cullinan/application.py
--rw-r--r--   0 runner    (1001) docker     (123)    24818 2023-06-27 06:05:25.000000 cullinan-0.53/cullinan/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-27 06:05:25.000000 cullinan-0.53/cullinan/dao.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-06-27 06:05:25.000000 cullinan-0.53/cullinan/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-27 06:05:25.000000 cullinan-0.53/cullinan/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-27 06:05:25.000000 cullinan-0.53/cullinan/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:05:37.924179 cullinan-0.53/cullinan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-27 06:05:37.000000 cullinan-0.53/cullinan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-27 06:05:37.000000 cullinan-0.53/cullinan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 06:05:37.000000 cullinan-0.53/cullinan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-27 06:05:37.000000 cullinan-0.53/cullinan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 06:05:37.000000 cullinan-0.53/cullinan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 06:05:37.924179 cullinan-0.53/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-27 06:05:25.000000 cullinan-0.53/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:48:24.073813 cullinan-0.54a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-07-01 16:48:11.000000 cullinan-0.54a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-01 16:48:24.073813 cullinan-0.54a1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:48:24.069812 cullinan-0.54a1/cullinan/
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-07-01 16:48:11.000000 cullinan-0.54a1/cullinan/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24818 2023-07-01 16:48:11.000000 cullinan-0.54a1/cullinan/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-01 16:48:11.000000 cullinan-0.54a1/cullinan/dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-01 16:48:11.000000 cullinan-0.54a1/cullinan/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-01 16:48:11.000000 cullinan-0.54a1/cullinan/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-01 16:48:11.000000 cullinan-0.54a1/cullinan/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:48:24.069812 cullinan-0.54a1/cullinan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-01 16:48:24.000000 cullinan-0.54a1/cullinan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-01 16:48:24.000000 cullinan-0.54a1/cullinan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 16:48:24.000000 cullinan-0.54a1/cullinan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 16:48:24.000000 cullinan-0.54a1/cullinan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-01 16:48:24.000000 cullinan-0.54a1/cullinan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 16:48:24.073813 cullinan-0.54a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-01 16:48:11.000000 cullinan-0.54a1/setup.py
```

### Comparing `cullinan-0.53/LICENSE` & `cullinan-0.54a1/LICENSE`

 * *Files identical despite different names*

### Comparing `cullinan-0.53/PKG-INFO` & `cullinan-0.54a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cullinan
-Version: 0.53
+Version: 0.54a1
 Summary: Cullinan is written based on tornado and Sqlalchemy to help the project quickly build web application
 Home-page: https://github.com/plumeink/Cullinan
 Author: plumeink
 Author-email: official@plumeink.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Source, https://github.com/plumeink/Cullinan
 Project-URL: Wiki, https://github.com/plumeink/Cullinan/wiki
```

### Comparing `cullinan-0.53/cullinan/application.py` & `cullinan-0.54a1/cullinan/application.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,15 +90,17 @@
         url = ""
         for index in range(1, len(item[0])):
             url = url + "/" + item[0][index]
         item[0] = url
         del item[2]
 
 
-def run():
+def run(handlers=None):
+    if handlers is None:
+        handlers = []
     print(
         "\n|||||||||||||||||||||||||||||||||||||||||||||||||\n|||                                           |||\n|||  "
         "   _____      _ _ _ "
         "               |||\n|||    / ____|    | | (_)                     |||\n|||   | |    _   _| | |_ _ __   __ "
         "_ _ __     |||\n|||   | |   | | | | | | | '_ \ / _` | '_ \    |||\n|||   | |___| |_| | | | | | | | (_| | | | "
         "|   |||\n|||    \_____\__, "
         "_|_|_|_|_| |_|\__,_|_| |_|   |||\n|||                                           "
@@ -114,15 +116,15 @@
     )
     print("\t|||\t\t└---scanning controller...")
     print("\t|||\t\t\t...")
     scan_service(file_list_func())
     scan_controller(file_list_func())
     sort_url()
     mapping = tornado.web.Application(
-        handlers=handler_list,
+        handlers=handler_list + handlers,
         **settings
     )
     print("\t|||\t\t└---loading controller finish\n\t|||\t")
     define("port", default=os.getenv("SERVER_PORT"), help="run on the given port", type=int)
     print("\t|||\tloading env finish\n\t|||\t")
     http_server = tornado.httpserver.HTTPServer(mapping)
     if os.getenv("SERVER_THREAD") is not None:
```

### Comparing `cullinan-0.53/cullinan/controller.py` & `cullinan-0.54a1/cullinan/controller.py`

 * *Files identical despite different names*

### Comparing `cullinan-0.53/cullinan/dao.py` & `cullinan-0.54a1/cullinan/dao.py`

 * *Files identical despite different names*

### Comparing `cullinan-0.53/cullinan/request.py` & `cullinan-0.54a1/cullinan/request.py`

 * *Files identical despite different names*

### Comparing `cullinan-0.53/cullinan/service.py` & `cullinan-0.54a1/cullinan/service.py`

 * *Files identical despite different names*

### Comparing `cullinan-0.53/cullinan.egg-info/PKG-INFO` & `cullinan-0.54a1/cullinan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cullinan
-Version: 0.53
+Version: 0.54a1
 Summary: Cullinan is written based on tornado and Sqlalchemy to help the project quickly build web application
 Home-page: https://github.com/plumeink/Cullinan
 Author: plumeink
 Author-email: official@plumeink.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Source, https://github.com/plumeink/Cullinan
 Project-URL: Wiki, https://github.com/plumeink/Cullinan/wiki
```

### Comparing `cullinan-0.53/setup.py` & `cullinan-0.54a1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.MD", "r", encoding="UTF-8") as fh:
     long_description = fh.read()
 
 setup(
     name='cullinan',
-    version='0.53',
+    version='0.54a1',
     packages=['cullinan'],
     description='Cullinan is written based on tornado and Sqlalchemy to help the project quickly build web application',
     author='plumeink',
     project_urls={
             'Source': 'https://github.com/plumeink/Cullinan',
             'Wiki': 'https://github.com/plumeink/Cullinan/wiki',
       },
```

