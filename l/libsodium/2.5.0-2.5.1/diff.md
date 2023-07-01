# Comparing `tmp/libsodium-2.5.0.tar.gz` & `tmp/libsodium-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsodium-2.5.0.tar", last modified: Sat Jun 17 19:49:13 2023, max compression
+gzip compressed data, was "libsodium-2.5.1.tar", last modified: Sat Jul  1 18:29:57 2023, max compression
```

## Comparing `libsodium-2.5.0.tar` & `libsodium-2.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:49:13.772675 libsodium-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-17 19:48:47.000000 libsodium-2.5.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-17 19:49:13.772675 libsodium-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-17 19:48:47.000000 libsodium-2.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-17 19:48:47.000000 libsodium-2.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-17 19:49:13.772675 libsodium-2.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:49:13.768675 libsodium-2.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:49:13.772675 libsodium-2.5.0/src/libsodium/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-17 19:48:47.000000 libsodium-2.5.0/src/libsodium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26876 2023-06-17 19:48:47.000000 libsodium-2.5.0/src/libsodium/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-17 19:48:47.000000 libsodium-2.5.0/src/libsodium/classes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:49:13.772675 libsodium-2.5.0/src/libsodium/db/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-17 19:48:47.000000 libsodium-2.5.0/src/libsodium/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-17 19:48:47.000000 libsodium-2.5.0/src/libsodium/db/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-17 19:48:47.000000 libsodium-2.5.0/src/libsodium/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-06-17 19:48:47.000000 libsodium-2.5.0/src/libsodium/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:49:13.772675 libsodium-2.5.0/src/libsodium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-17 19:49:13.000000 libsodium-2.5.0/src/libsodium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-17 19:49:13.000000 libsodium-2.5.0/src/libsodium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 19:49:13.000000 libsodium-2.5.0/src/libsodium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-17 19:49:13.000000 libsodium-2.5.0/src/libsodium.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:29:57.102473 libsodium-2.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-01 18:29:26.000000 libsodium-2.5.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-01 18:29:57.102473 libsodium-2.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-01 18:29:26.000000 libsodium-2.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-01 18:29:26.000000 libsodium-2.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-01 18:29:57.102473 libsodium-2.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:29:57.098473 libsodium-2.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:29:57.098473 libsodium-2.5.1/src/libsodium/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-01 18:29:26.000000 libsodium-2.5.1/src/libsodium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26876 2023-07-01 18:29:26.000000 libsodium-2.5.1/src/libsodium/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-01 18:29:26.000000 libsodium-2.5.1/src/libsodium/classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:29:57.102473 libsodium-2.5.1/src/libsodium/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-01 18:29:26.000000 libsodium-2.5.1/src/libsodium/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-01 18:29:26.000000 libsodium-2.5.1/src/libsodium/db/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-01 18:29:26.000000 libsodium-2.5.1/src/libsodium/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-07-01 18:29:26.000000 libsodium-2.5.1/src/libsodium/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:29:57.102473 libsodium-2.5.1/src/libsodium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-01 18:29:57.000000 libsodium-2.5.1/src/libsodium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-01 18:29:57.000000 libsodium-2.5.1/src/libsodium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 18:29:57.000000 libsodium-2.5.1/src/libsodium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 18:29:57.000000 libsodium-2.5.1/src/libsodium.egg-info/top_level.txt
```

### Comparing `libsodium-2.5.0/LICENCE` & `libsodium-2.5.1/LICENCE`

 * *Files identical despite different names*

### Comparing `libsodium-2.5.0/PKG-INFO` & `libsodium-2.5.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: libsodium
-Version: 2.5.0
+Version: 2.5.1
 Summary: A simple web framework
 Home-page: https://libsodium.readthedocs.io/en/latest/
 Author: Ahsan Ahmed
 Author-email: ahsan.ahmed3246@gmail.com
 Project-URL: Docs, https://libsodium.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
-# Sodium v2.50
+# Sodium v2.51
 [![Documentation Status](https://readthedocs.org/projects/libsodium/badge/?version=latest)](https://libsodium.readthedocs.io/en/latest/?badge=latest)
 ![PyPI](https://img.shields.io/pypi/v/libsodium)
 
 Sodium is a WSGI web framework(like django) that is built for creating API's.
 # Instalation
 Linux/MacOS:
 ```
```

### Comparing `libsodium-2.5.0/setup.cfg` & `libsodium-2.5.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = libsodium
-version = 2.5.0
+version = 2.5.1
 author = Ahsan Ahmed
 author_email = ahsan.ahmed3246@gmail.com
 description = A simple web framework
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://libsodium.readthedocs.io/en/latest/
 project_urls =
```

### Comparing `libsodium-2.5.0/src/libsodium/__main__.py` & `libsodium-2.5.1/src/libsodium/__main__.py`

 * *Files identical despite different names*

### Comparing `libsodium-2.5.0/src/libsodium/classes.py` & `libsodium-2.5.1/src/libsodium/classes.py`

 * *Files identical despite different names*

### Comparing `libsodium-2.5.0/src/libsodium/wsgi.py` & `libsodium-2.5.1/src/libsodium/wsgi.py`

 * *Files identical despite different names*

### Comparing `libsodium-2.5.0/src/libsodium.egg-info/PKG-INFO` & `libsodium-2.5.1/src/libsodium.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: libsodium
-Version: 2.5.0
+Version: 2.5.1
 Summary: A simple web framework
 Home-page: https://libsodium.readthedocs.io/en/latest/
 Author: Ahsan Ahmed
 Author-email: ahsan.ahmed3246@gmail.com
 Project-URL: Docs, https://libsodium.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
-# Sodium v2.50
+# Sodium v2.51
 [![Documentation Status](https://readthedocs.org/projects/libsodium/badge/?version=latest)](https://libsodium.readthedocs.io/en/latest/?badge=latest)
 ![PyPI](https://img.shields.io/pypi/v/libsodium)
 
 Sodium is a WSGI web framework(like django) that is built for creating API's.
 # Instalation
 Linux/MacOS:
 ```
```

