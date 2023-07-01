# Comparing `tmp/asgihandler-0.4.9.tar.gz` & `tmp/asgihandler-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgihandler-0.4.9.tar", last modified: Sat Jul  1 00:56:49 2023, max compression
+gzip compressed data, was "asgihandler-0.5.0.tar", last modified: Sat Jul  1 02:23:51 2023, max compression
```

## Comparing `asgihandler-0.4.9.tar` & `asgihandler-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 00:56:49.825082 asgihandler-0.4.9/
--rw-rw-rw-   0        0        0     1067 2022-07-16 23:50:52.000000 asgihandler-0.4.9/LICENSE
--rw-rw-rw-   0        0        0       27 2022-07-16 23:50:52.000000 asgihandler-0.4.9/MANIFEST.in
--rw-rw-rw-   0        0        0     3117 2023-07-01 00:56:49.824083 asgihandler-0.4.9/PKG-INFO
--rw-rw-rw-   0        0        0     2483 2023-05-02 06:18:39.000000 asgihandler-0.4.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 00:56:49.811100 asgihandler-0.4.9/asgihandler/
--rw-rw-rw-   0        0        0       21 2022-07-16 23:50:52.000000 asgihandler-0.4.9/asgihandler/__init__.py
--rw-rw-rw-   0        0        0       68 2022-07-16 23:55:07.000000 asgihandler-0.4.9/asgihandler/__version__.py
--rw-rw-rw-   0        0        0     1272 2023-07-01 00:56:19.000000 asgihandler-0.4.9/asgihandler/core.py
--rw-rw-rw-   0        0        0      496 2023-07-01 00:56:19.000000 asgihandler-0.4.9/asgihandler/userCheck.py
-drwxrwxrwx   0        0        0        0 2023-07-01 00:56:49.823081 asgihandler-0.4.9/asgihandler.egg-info/
--rw-rw-rw-   0        0        0     3117 2023-07-01 00:56:49.000000 asgihandler-0.4.9/asgihandler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-07-01 00:56:49.000000 asgihandler-0.4.9/asgihandler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 00:56:49.000000 asgihandler-0.4.9/asgihandler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-01 00:56:49.000000 asgihandler-0.4.9/asgihandler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-01 00:56:49.000000 asgihandler-0.4.9/asgihandler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 00:56:49.825082 asgihandler-0.4.9/setup.cfg
--rw-rw-rw-   0        0        0     3878 2023-07-01 00:54:53.000000 asgihandler-0.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 02:23:51.923526 asgihandler-0.5.0/
+-rw-rw-rw-   0        0        0     1067 2022-07-16 23:50:52.000000 asgihandler-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0       27 2022-07-16 23:50:52.000000 asgihandler-0.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3117 2023-07-01 02:23:51.922526 asgihandler-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2483 2023-05-02 06:18:39.000000 asgihandler-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 02:23:51.905526 asgihandler-0.5.0/asgihandler/
+-rw-rw-rw-   0        0        0       21 2022-07-16 23:50:52.000000 asgihandler-0.5.0/asgihandler/__init__.py
+-rw-rw-rw-   0        0        0       68 2022-07-16 23:55:07.000000 asgihandler-0.5.0/asgihandler/__version__.py
+-rw-rw-rw-   0        0        0     1272 2023-07-01 00:56:19.000000 asgihandler-0.5.0/asgihandler/core.py
+-rw-rw-rw-   0        0        0      521 2023-07-01 02:13:18.000000 asgihandler-0.5.0/asgihandler/userCheck.py
+drwxrwxrwx   0        0        0        0 2023-07-01 02:23:51.921524 asgihandler-0.5.0/asgihandler.egg-info/
+-rw-rw-rw-   0        0        0     3117 2023-07-01 02:23:51.000000 asgihandler-0.5.0/asgihandler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-07-01 02:23:51.000000 asgihandler-0.5.0/asgihandler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 02:23:51.000000 asgihandler-0.5.0/asgihandler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-01 02:23:51.000000 asgihandler-0.5.0/asgihandler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-01 02:23:51.000000 asgihandler-0.5.0/asgihandler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 02:23:51.923526 asgihandler-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     3878 2023-07-01 02:23:48.000000 asgihandler-0.5.0/setup.py
```

### Comparing `asgihandler-0.4.9/LICENSE` & `asgihandler-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asgihandler-0.4.9/PKG-INFO` & `asgihandler-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgihandler
-Version: 0.4.9
+Version: 0.5.0
 Summary: ASGIHandler
 Home-page: https://github.com/GreaterWMS/GreaterWMS
 Author: Singosgu
 Author-email: singosgu@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `asgihandler-0.4.9/README.md` & `asgihandler-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `asgihandler-0.4.9/asgihandler/core.py` & `asgihandler-0.5.0/asgihandler/core.py`

 * *Files identical despite different names*

### Comparing `asgihandler-0.4.9/asgihandler.egg-info/PKG-INFO` & `asgihandler-0.5.0/asgihandler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgihandler
-Version: 0.4.9
+Version: 0.5.0
 Summary: ASGIHandler
 Home-page: https://github.com/GreaterWMS/GreaterWMS
 Author: Singosgu
 Author-email: singosgu@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `asgihandler-0.4.9/setup.py` & `asgihandler-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'asgihandler'
 DESCRIPTION = 'ASGIHandler'
 URL = 'https://github.com/GreaterWMS/GreaterWMS'
 EMAIL = 'singosgu@gmail.com'
 AUTHOR = 'Singosgu'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '0.4.9'
+VERSION = '0.5.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
 ]
 
 # What packages are optional?
```

