# Comparing `tmp/Galvatron-0.0.2.tar.gz` & `tmp/Galvatron-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Galvatron-0.0.2.tar", last modified: Sat Jul  1 17:42:14 2023, max compression
+gzip compressed data, was "Galvatron-0.0.3.tar", last modified: Sat Jul  1 18:50:57 2023, max compression
```

## Comparing `Galvatron-0.0.2.tar` & `Galvatron-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:42:14.506199 Galvatron-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:42:14.502199 Galvatron-0.0.2/Galvatron/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-01 17:42:02.000000 Galvatron-0.0.2/Galvatron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-01 17:42:02.000000 Galvatron-0.0.2/Galvatron/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:42:14.506199 Galvatron-0.0.2/Galvatron.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-01 17:42:14.000000 Galvatron-0.0.2/Galvatron.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-01 17:42:14.000000 Galvatron-0.0.2/Galvatron.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 17:42:14.000000 Galvatron-0.0.2/Galvatron.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-01 17:42:14.000000 Galvatron-0.0.2/Galvatron.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 17:42:14.000000 Galvatron-0.0.2/Galvatron.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-01 17:42:02.000000 Galvatron-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-01 17:42:14.506199 Galvatron-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-01 17:42:02.000000 Galvatron-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 17:42:14.506199 Galvatron-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-01 17:42:02.000000 Galvatron-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:50:57.778049 Galvatron-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:50:57.778049 Galvatron-0.0.3/Galvatron/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-01 18:50:44.000000 Galvatron-0.0.3/Galvatron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-07-01 18:50:44.000000 Galvatron-0.0.3/Galvatron/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:50:57.778049 Galvatron-0.0.3/Galvatron.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-01 18:50:57.000000 Galvatron-0.0.3/Galvatron.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-01 18:50:57.000000 Galvatron-0.0.3/Galvatron.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 18:50:57.000000 Galvatron-0.0.3/Galvatron.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-01 18:50:57.000000 Galvatron-0.0.3/Galvatron.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 18:50:57.000000 Galvatron-0.0.3/Galvatron.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-01 18:50:44.000000 Galvatron-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-01 18:50:57.778049 Galvatron-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-07-01 18:50:44.000000 Galvatron-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 18:50:57.778049 Galvatron-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-01 18:50:44.000000 Galvatron-0.0.3/setup.py
```

### Comparing `Galvatron-0.0.2/Galvatron.egg-info/PKG-INFO` & `Galvatron-0.0.3/Galvatron.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Galvatron
-Version: 0.0.2
+Version: 0.0.3
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/Galvatron
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Galvatron-0.0.2/LICENSE` & `Galvatron-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Galvatron-0.0.2/PKG-INFO` & `Galvatron-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Galvatron
-Version: 0.0.2
+Version: 0.0.3
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/Galvatron
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Galvatron-0.0.2/setup.py` & `Galvatron-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'Galvatron',
   packages = find_packages(exclude=[]),
-  version = '0.0.2',
+  version = '0.0.3',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/Galvatron',
   keywords = [
```

