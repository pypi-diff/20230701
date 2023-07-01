# Comparing `tmp/dynamic-service-1.0.0.tar.gz` & `tmp/dynamic-service-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic-service-1.0.0.tar", last modified: Sat Jul  1 09:41:36 2023, max compression
+gzip compressed data, was "dynamic-service-1.0.1.tar", last modified: Sat Jul  1 09:44:20 2023, max compression
```

## Comparing `dynamic-service-1.0.0.tar` & `dynamic-service-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 09:41:36.032973 dynamic-service-1.0.0/
--rw-rw-rw-   0        0        0      123 2023-07-01 09:41:35.000000 dynamic-service-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2037 2023-07-01 09:41:36.032973 dynamic-service-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1219 2023-07-01 08:56:11.000000 dynamic-service-1.0.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 dynamic-service-1.0.0/build.py
-drwxrwxrwx   0        0        0        0 2023-07-01 09:41:36.009081 dynamic-service-1.0.0/dynamic_service/
--rw-rw-rw-   0        0        0     1439 2023-07-01 08:46:12.000000 dynamic-service-1.0.0/dynamic_service/base.py
-drwxrwxrwx   0        0        0        0 2023-07-01 09:41:36.029971 dynamic-service-1.0.0/dynamic_service/endpoints/
--rw-rw-rw-   0        0        0      210 2023-07-01 09:41:01.000000 dynamic-service-1.0.0/dynamic_service/endpoints/__init__.py
--rw-rw-rw-   0        0        0     2599 2023-04-12 14:12:33.000000 dynamic-service-1.0.0/dynamic_service/endpoints/data.py
--rw-rw-rw-   0        0        0     9764 2023-07-01 09:41:01.000000 dynamic-service-1.0.0/dynamic_service/endpoints/engine.py
--rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 dynamic-service-1.0.0/dynamic_service/endpoints/exceptions.py
--rw-rw-rw-   0        0        0     1608 2023-07-01 09:41:01.000000 dynamic-service-1.0.0/dynamic_service/endpoints/process.py
-drwxrwxrwx   0        0        0        0 2023-07-01 09:41:36.031973 dynamic-service-1.0.0/dynamic_service/service/
--rw-rw-rw-   0        0        0      106 2023-07-01 09:41:01.000000 dynamic-service-1.0.0/dynamic_service/service/__init__.py
--rw-rw-rw-   0        0        0    19706 2023-07-01 09:41:01.000000 dynamic-service-1.0.0/dynamic_service/service/rest.py
--rw-rw-rw-   0        0        0     3012 2023-07-01 09:41:01.000000 dynamic-service-1.0.0/dynamic_service/service/sockets.py
-drwxrwxrwx   0        0        0        0 2023-07-01 09:41:36.025973 dynamic-service-1.0.0/dynamic_service.egg-info/
--rw-rw-rw-   0        0        0     2037 2023-07-01 09:41:35.000000 dynamic-service-1.0.0/dynamic_service.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      598 2023-07-01 09:41:35.000000 dynamic-service-1.0.0/dynamic_service.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 09:41:35.000000 dynamic-service-1.0.0/dynamic_service.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-07-01 09:41:35.000000 dynamic-service-1.0.0/dynamic_service.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-01 09:41:35.000000 dynamic-service-1.0.0/dynamic_service.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      627 2023-07-01 09:41:35.000000 dynamic-service-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       78 2023-06-15 21:47:31.000000 dynamic-service-1.0.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       69 2023-06-15 21:46:16.000000 dynamic-service-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 09:41:36.032973 dynamic-service-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1596 2023-07-01 09:41:01.000000 dynamic-service-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:44:20.046517 dynamic-service-1.0.1/
+-rw-rw-rw-   0        0        0      236 2023-07-01 09:44:19.000000 dynamic-service-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2037 2023-07-01 09:44:20.046517 dynamic-service-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1219 2023-07-01 08:56:11.000000 dynamic-service-1.0.1/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 dynamic-service-1.0.1/build.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:44:20.025441 dynamic-service-1.0.1/dynamic_service/
+-rw-rw-rw-   0        0        0     1439 2023-07-01 08:46:12.000000 dynamic-service-1.0.1/dynamic_service/base.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:44:20.041542 dynamic-service-1.0.1/dynamic_service/endpoints/
+-rw-rw-rw-   0        0        0      210 2023-07-01 09:41:01.000000 dynamic-service-1.0.1/dynamic_service/endpoints/__init__.py
+-rw-rw-rw-   0        0        0     2599 2023-04-12 14:12:33.000000 dynamic-service-1.0.1/dynamic_service/endpoints/data.py
+-rw-rw-rw-   0        0        0     9764 2023-07-01 09:41:01.000000 dynamic-service-1.0.1/dynamic_service/endpoints/engine.py
+-rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 dynamic-service-1.0.1/dynamic_service/endpoints/exceptions.py
+-rw-rw-rw-   0        0        0     1608 2023-07-01 09:41:01.000000 dynamic-service-1.0.1/dynamic_service/endpoints/process.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:44:20.043516 dynamic-service-1.0.1/dynamic_service/service/
+-rw-rw-rw-   0        0        0      106 2023-07-01 09:41:01.000000 dynamic-service-1.0.1/dynamic_service/service/__init__.py
+-rw-rw-rw-   0        0        0    19706 2023-07-01 09:41:01.000000 dynamic-service-1.0.1/dynamic_service/service/rest.py
+-rw-rw-rw-   0        0        0     3012 2023-07-01 09:41:01.000000 dynamic-service-1.0.1/dynamic_service/service/sockets.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:44:20.014444 dynamic-service-1.0.1/dynamic_service/source/
+drwxrwxrwx   0        0        0        0 2023-07-01 09:44:20.014444 dynamic-service-1.0.1/dynamic_service/source/assets/
+drwxrwxrwx   0        0        0        0 2023-07-01 09:44:20.045542 dynamic-service-1.0.1/dynamic_service/source/assets/icon/
+-rw-rw-rw-   0        0        0     2834 2023-02-04 16:41:18.000000 dynamic-service-1.0.1/dynamic_service/source/assets/icon/icon.ico
+-rw-rw-rw-   0        0        0    27619 2023-02-04 16:40:24.000000 dynamic-service-1.0.1/dynamic_service/source/assets/icon/icon.png
+drwxrwxrwx   0        0        0        0 2023-07-01 09:44:20.037546 dynamic-service-1.0.1/dynamic_service.egg-info/
+-rw-rw-rw-   0        0        0     2037 2023-07-01 09:44:19.000000 dynamic-service-1.0.1/dynamic_service.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2023-07-01 09:44:20.000000 dynamic-service-1.0.1/dynamic_service.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 09:44:19.000000 dynamic-service-1.0.1/dynamic_service.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-07-01 09:44:20.000000 dynamic-service-1.0.1/dynamic_service.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-01 09:44:20.000000 dynamic-service-1.0.1/dynamic_service.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      627 2023-07-01 09:44:19.000000 dynamic-service-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       78 2023-06-15 21:47:31.000000 dynamic-service-1.0.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       69 2023-06-15 21:46:16.000000 dynamic-service-1.0.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 09:44:20.046517 dynamic-service-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2023-07-01 09:44:13.000000 dynamic-service-1.0.1/setup.py
```

### Comparing `dynamic-service-1.0.0/PKG-INFO` & `dynamic-service-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-service
-Version: 1.0.0
+Version: 1.0.1
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/dynamic-service
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `dynamic-service-1.0.0/README.md` & `dynamic-service-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.0.0/build.py` & `dynamic-service-1.0.1/build.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.0.0/dynamic_service/base.py` & `dynamic-service-1.0.1/dynamic_service/base.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.0.0/dynamic_service/endpoints/data.py` & `dynamic-service-1.0.1/dynamic_service/endpoints/data.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.0.0/dynamic_service/endpoints/engine.py` & `dynamic-service-1.0.1/dynamic_service/endpoints/engine.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.0.0/dynamic_service/endpoints/exceptions.py` & `dynamic-service-1.0.1/dynamic_service/endpoints/exceptions.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.0.0/dynamic_service/endpoints/process.py` & `dynamic-service-1.0.1/dynamic_service/endpoints/process.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.0.0/dynamic_service/service/rest.py` & `dynamic-service-1.0.1/dynamic_service/service/rest.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.0.0/dynamic_service/service/sockets.py` & `dynamic-service-1.0.1/dynamic_service/service/sockets.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.0.0/dynamic_service.egg-info/PKG-INFO` & `dynamic-service-1.0.1/dynamic_service.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-service
-Version: 1.0.0
+Version: 1.0.1
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/dynamic-service
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `dynamic-service-1.0.0/dynamic_service.egg-info/SOURCES.txt` & `dynamic-service-1.0.1/dynamic_service.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -14,8 +14,10 @@
 dynamic_service/endpoints/__init__.py
 dynamic_service/endpoints/data.py
 dynamic_service/endpoints/engine.py
 dynamic_service/endpoints/exceptions.py
 dynamic_service/endpoints/process.py
 dynamic_service/service/__init__.py
 dynamic_service/service/rest.py
-dynamic_service/service/sockets.py
+dynamic_service/service/sockets.py
+dynamic_service/source/assets/icon/icon.ico
+dynamic_service/source/assets/icon/icon.png
```

### Comparing `dynamic-service-1.0.0/pyproject.toml` & `dynamic-service-1.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'dynamic-service'
-version = '1.0.0'
+version = '1.0.1'
 description = 'A framework for developing responsive, live and dynamic REST APIs with python.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `dynamic-service-1.0.0/setup.py` & `dynamic-service-1.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,20 +18,20 @@
         package="dynamic_service",
         project="pyproject.toml",
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         include=[
-            "live_api/source"
+            "dynamic_service/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='dynamic-service',
-        version='1.0.0',
+        version='1.0.1',
         description=(
             "A framework for developing responsive, "
             "live and dynamic REST APIs with python."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

