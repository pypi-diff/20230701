# Comparing `tmp/omneer-0.1.tar.gz` & `tmp/omneer-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omneer-0.1.tar", last modified: Sat Jul  1 05:35:43 2023, max compression
+gzip compressed data, was "omneer-0.11.tar", last modified: Sat Jul  1 05:51:24 2023, max compression
```

## Comparing `omneer-0.1.tar` & `omneer-0.11.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 willblair   (502) staff       (20)        0 2023-07-01 05:35:43.800131 omneer-0.1/
--rw-r--r--   0 willblair   (502) staff       (20)     3578 2023-07-01 05:35:43.799563 omneer-0.1/PKG-INFO
--rw-r--r--   0 willblair   (502) staff       (20)     3299 2023-07-01 03:48:24.000000 omneer-0.1/README.md
-drwxr-xr-x   0 willblair   (502) staff       (20)        0 2023-07-01 05:35:43.798786 omneer-0.1/omneer.egg-info/
--rw-r--r--   0 willblair   (502) staff       (20)     3578 2023-07-01 05:35:43.000000 omneer-0.1/omneer.egg-info/PKG-INFO
--rw-r--r--   0 willblair   (502) staff       (20)      200 2023-07-01 05:35:43.000000 omneer-0.1/omneer.egg-info/SOURCES.txt
--rw-r--r--   0 willblair   (502) staff       (20)        1 2023-07-01 05:35:43.000000 omneer-0.1/omneer.egg-info/dependency_links.txt
--rw-r--r--   0 willblair   (502) staff       (20)       47 2023-07-01 05:35:43.000000 omneer-0.1/omneer.egg-info/entry_points.txt
--rw-r--r--   0 willblair   (502) staff       (20)      216 2023-07-01 05:35:43.000000 omneer-0.1/omneer.egg-info/requires.txt
--rw-r--r--   0 willblair   (502) staff       (20)        1 2023-07-01 05:35:43.000000 omneer-0.1/omneer.egg-info/top_level.txt
--rw-r--r--   0 willblair   (502) staff       (20)       38 2023-07-01 05:35:43.800401 omneer-0.1/setup.cfg
--rw-r--r--   0 willblair   (502) staff       (20)      976 2023-07-01 05:35:41.000000 omneer-0.1/setup.py
+drwxr-xr-x   0 willblair   (502) staff       (20)        0 2023-07-01 05:51:24.072288 omneer-0.11/
+-rw-r--r--   0 willblair   (502) staff       (20)     3579 2023-07-01 05:51:24.071828 omneer-0.11/PKG-INFO
+-rw-r--r--   0 willblair   (502) staff       (20)     3299 2023-07-01 03:48:24.000000 omneer-0.11/README.md
+drwxr-xr-x   0 willblair   (502) staff       (20)        0 2023-07-01 05:51:24.071138 omneer-0.11/omneer.egg-info/
+-rw-r--r--   0 willblair   (502) staff       (20)     3579 2023-07-01 05:51:23.000000 omneer-0.11/omneer.egg-info/PKG-INFO
+-rw-r--r--   0 willblair   (502) staff       (20)      200 2023-07-01 05:51:24.000000 omneer-0.11/omneer.egg-info/SOURCES.txt
+-rw-r--r--   0 willblair   (502) staff       (20)        1 2023-07-01 05:51:23.000000 omneer-0.11/omneer.egg-info/dependency_links.txt
+-rw-r--r--   0 willblair   (502) staff       (20)       47 2023-07-01 05:51:23.000000 omneer-0.11/omneer.egg-info/entry_points.txt
+-rw-r--r--   0 willblair   (502) staff       (20)      216 2023-07-01 05:51:23.000000 omneer-0.11/omneer.egg-info/requires.txt
+-rw-r--r--   0 willblair   (502) staff       (20)        1 2023-07-01 05:51:24.000000 omneer-0.11/omneer.egg-info/top_level.txt
+-rw-r--r--   0 willblair   (502) staff       (20)       38 2023-07-01 05:51:24.072443 omneer-0.11/setup.cfg
+-rw-r--r--   0 willblair   (502) staff       (20)      977 2023-07-01 05:48:04.000000 omneer-0.11/setup.py
```

### Comparing `omneer-0.1/PKG-INFO` & `omneer-0.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omneer
-Version: 0.1
+Version: 0.11
 Summary: Advanced personalized medicine diagnostics for neurodegenerative disorders
 Home-page: http://omneer.xyz
 Author: William Blair
 Author-email: william.blair0708@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `omneer-0.1/README.md` & `omneer-0.11/README.md`

 * *Files identical despite different names*

### Comparing `omneer-0.1/omneer.egg-info/PKG-INFO` & `omneer-0.11/omneer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omneer
-Version: 0.1
+Version: 0.11
 Summary: Advanced personalized medicine diagnostics for neurodegenerative disorders
 Home-page: http://omneer.xyz
 Author: William Blair
 Author-email: william.blair0708@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `omneer-0.1/setup.py` & `omneer-0.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='omneer',
-    version='0.1',
+    version='0.11',
     packages=find_packages(include=['omneer', 'omneer.*']),
     url='http://omneer.xyz',
     license='MIT',
     author='William Blair',
     author_email='william.blair0708@gmail.com',
     description='Advanced personalized medicine diagnostics for neurodegenerative disorders',
     long_description=open('README.md').read(),
```

