# Comparing `tmp/galaxy-auth-23.0.3.tar.gz` & `tmp/galaxy-auth-23.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/auth/dist/.tmp-ej9t4mbd/galaxy-auth-23.0.3.tar", last modified: Mon Jun 26 09:54:23 2023, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/auth/dist/.tmp-i8rkpjth/galaxy-auth-23.0.4.tar", last modified: Fri Jun 30 22:06:36 2023, max compression
```

## Comparing `galaxy-auth-23.0.3.tar` & `galaxy-auth-23.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:54:23.000000 galaxy-auth-23.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-26 09:48:33.000000 galaxy-auth-23.0.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-26 09:48:32.000000 galaxy-auth-23.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-26 09:48:33.000000 galaxy-auth-23.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-26 09:54:23.000000 galaxy-auth-23.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-26 09:48:33.000000 galaxy-auth-23.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-26 09:48:33.000000 galaxy-auth-23.0.3/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:54:23.000000 galaxy-auth-23.0.3/galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-26 09:48:33.000000 galaxy-auth-23.0.3/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:54:23.000000 galaxy-auth-23.0.3/galaxy/auth/
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-06-26 09:48:33.000000 galaxy-auth-23.0.3/galaxy/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:54:23.000000 galaxy-auth-23.0.3/galaxy/auth/providers/
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-26 09:48:33.000000 galaxy-auth-23.0.3/galaxy/auth/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-26 09:48:33.000000 galaxy-auth-23.0.3/galaxy/auth/providers/alwaysreject.py
--rw-r--r--   0 runner    (1001) docker     (123)    18471 2023-06-26 09:48:33.000000 galaxy-auth-23.0.3/galaxy/auth/providers/ldap_ad.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-26 09:48:33.000000 galaxy-auth-23.0.3/galaxy/auth/providers/localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-06-26 09:48:33.000000 galaxy-auth-23.0.3/galaxy/auth/providers/pam_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-26 09:48:33.000000 galaxy-auth-23.0.3/galaxy/auth/util.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:48:33.000000 galaxy-auth-23.0.3/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:54:23.000000 galaxy-auth-23.0.3/galaxy_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-26 09:54:23.000000 galaxy-auth-23.0.3/galaxy_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-26 09:54:23.000000 galaxy-auth-23.0.3/galaxy_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:54:23.000000 galaxy-auth-23.0.3/galaxy_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 09:54:23.000000 galaxy-auth-23.0.3/galaxy_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 09:54:23.000000 galaxy-auth-23.0.3/galaxy_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 09:48:33.000000 galaxy-auth-23.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-26 09:54:23.000000 galaxy-auth-23.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 09:48:33.000000 galaxy-auth-23.0.3/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:06:36.000000 galaxy-auth-23.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-30 22:00:50.000000 galaxy-auth-23.0.4/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-30 22:00:49.000000 galaxy-auth-23.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-30 22:00:50.000000 galaxy-auth-23.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-30 22:06:36.000000 galaxy-auth-23.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-30 22:00:50.000000 galaxy-auth-23.0.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-30 22:00:50.000000 galaxy-auth-23.0.4/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:06:36.000000 galaxy-auth-23.0.4/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-30 22:00:50.000000 galaxy-auth-23.0.4/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:06:36.000000 galaxy-auth-23.0.4/galaxy/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-06-30 22:00:50.000000 galaxy-auth-23.0.4/galaxy/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:06:36.000000 galaxy-auth-23.0.4/galaxy/auth/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-30 22:00:50.000000 galaxy-auth-23.0.4/galaxy/auth/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-30 22:00:50.000000 galaxy-auth-23.0.4/galaxy/auth/providers/alwaysreject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18471 2023-06-30 22:00:50.000000 galaxy-auth-23.0.4/galaxy/auth/providers/ldap_ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-30 22:00:50.000000 galaxy-auth-23.0.4/galaxy/auth/providers/localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-06-30 22:00:50.000000 galaxy-auth-23.0.4/galaxy/auth/providers/pam_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-30 22:00:50.000000 galaxy-auth-23.0.4/galaxy/auth/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:00:50.000000 galaxy-auth-23.0.4/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:06:36.000000 galaxy-auth-23.0.4/galaxy_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-30 22:06:36.000000 galaxy-auth-23.0.4/galaxy_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-30 22:06:36.000000 galaxy-auth-23.0.4/galaxy_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:06:36.000000 galaxy-auth-23.0.4/galaxy_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-30 22:06:36.000000 galaxy-auth-23.0.4/galaxy_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 22:06:36.000000 galaxy-auth-23.0.4/galaxy_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-30 22:00:50.000000 galaxy-auth-23.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-30 22:06:36.000000 galaxy-auth-23.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 22:00:50.000000 galaxy-auth-23.0.4/test-requirements.txt
```

### Comparing `galaxy-auth-23.0.3/HISTORY.rst` & `galaxy-auth-23.0.4/HISTORY.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.4 (2023-06-30)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.3 (2023-06-26)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.2 (2023-06-13)
```

### Comparing `galaxy-auth-23.0.3/LICENSE` & `galaxy-auth-23.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-auth-23.0.3/PKG-INFO` & `galaxy-auth-23.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-auth
-Version: 23.0.3
+Version: 23.0.4
 Summary: Galaxy auth framework and implementations
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -43,14 +43,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.4 (2023-06-30)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.3 (2023-06-26)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.2 (2023-06-13)
```

### Comparing `galaxy-auth-23.0.3/galaxy/auth/__init__.py` & `galaxy-auth-23.0.4/galaxy/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-auth-23.0.3/galaxy/auth/providers/__init__.py` & `galaxy-auth-23.0.4/galaxy/auth/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-auth-23.0.3/galaxy/auth/providers/alwaysreject.py` & `galaxy-auth-23.0.4/galaxy/auth/providers/alwaysreject.py`

 * *Files identical despite different names*

### Comparing `galaxy-auth-23.0.3/galaxy/auth/providers/ldap_ad.py` & `galaxy-auth-23.0.4/galaxy/auth/providers/ldap_ad.py`

 * *Files identical despite different names*

### Comparing `galaxy-auth-23.0.3/galaxy/auth/providers/localdb.py` & `galaxy-auth-23.0.4/galaxy/auth/providers/localdb.py`

 * *Files identical despite different names*

### Comparing `galaxy-auth-23.0.3/galaxy/auth/providers/pam_auth.py` & `galaxy-auth-23.0.4/galaxy/auth/providers/pam_auth.py`

 * *Files identical despite different names*

### Comparing `galaxy-auth-23.0.3/galaxy/auth/util.py` & `galaxy-auth-23.0.4/galaxy/auth/util.py`

 * *Files identical despite different names*

### Comparing `galaxy-auth-23.0.3/galaxy_auth.egg-info/PKG-INFO` & `galaxy-auth-23.0.4/galaxy_auth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-auth
-Version: 23.0.3
+Version: 23.0.4
 Summary: Galaxy auth framework and implementations
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -43,14 +43,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.4 (2023-06-30)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.3 (2023-06-26)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.2 (2023-06-13)
```

### Comparing `galaxy-auth-23.0.3/galaxy_auth.egg-info/SOURCES.txt` & `galaxy-auth-23.0.4/galaxy_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-auth-23.0.3/setup.cfg` & `galaxy-auth-23.0.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-auth
 url = https://github.com/galaxyproject/galaxy
-version = 23.0.3
+version = 23.0.4
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-data
 	galaxy-util
 packages = find:
```

