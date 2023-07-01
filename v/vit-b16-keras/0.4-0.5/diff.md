# Comparing `tmp/vit-b16-keras-0.4.tar.gz` & `tmp/vit-b16-keras-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vit-b16-keras-0.4.tar", last modified: Fri Jun 30 18:55:52 2023, max compression
+gzip compressed data, was "vit-b16-keras-0.5.tar", last modified: Sat Jul  1 11:07:39 2023, max compression
```

## Comparing `vit-b16-keras-0.4.tar` & `vit-b16-keras-0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 18:55:52.011655 vit-b16-keras-0.4/
--rw-rw-rw-   0        0        0      616 2023-06-30 18:55:52.010139 vit-b16-keras-0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-30 18:55:52.011655 vit-b16-keras-0.4/setup.cfg
--rw-rw-rw-   0        0        0      852 2023-06-30 18:55:43.000000 vit-b16-keras-0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 18:55:51.988874 vit-b16-keras-0.4/vit_b16_keras/
--rw-rw-rw-   0        0        0       40 2023-06-30 17:45:23.000000 vit-b16-keras-0.4/vit_b16_keras/__init__.py
--rw-rw-rw-   0        0        0      352 2023-06-30 18:55:32.000000 vit-b16-keras-0.4/vit_b16_keras/vit_b16.py
-drwxrwxrwx   0        0        0        0 2023-06-30 18:55:52.008130 vit-b16-keras-0.4/vit_b16_keras.egg-info/
--rw-rw-rw-   0        0        0      616 2023-06-30 18:55:51.000000 vit-b16-keras-0.4/vit_b16_keras.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-06-30 18:55:51.000000 vit-b16-keras-0.4/vit_b16_keras.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 18:55:51.000000 vit-b16-keras-0.4/vit_b16_keras.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-30 18:55:51.000000 vit-b16-keras-0.4/vit_b16_keras.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-30 18:55:51.000000 vit-b16-keras-0.4/vit_b16_keras.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 11:07:39.569587 vit-b16-keras-0.5/
+-rw-rw-rw-   0        0        0      616 2023-07-01 11:07:39.567586 vit-b16-keras-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-01 11:07:39.569587 vit-b16-keras-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      852 2023-07-01 11:07:09.000000 vit-b16-keras-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 11:07:39.538909 vit-b16-keras-0.5/vit_b16_keras/
+-rw-rw-rw-   0        0        0       40 2023-06-30 17:45:23.000000 vit-b16-keras-0.5/vit_b16_keras/__init__.py
+-rw-rw-rw-   0        0        0      351 2023-07-01 11:06:27.000000 vit-b16-keras-0.5/vit_b16_keras/vit_b16.py
+drwxrwxrwx   0        0        0        0 2023-07-01 11:07:39.565587 vit-b16-keras-0.5/vit_b16_keras.egg-info/
+-rw-rw-rw-   0        0        0      616 2023-07-01 11:07:39.000000 vit-b16-keras-0.5/vit_b16_keras.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-07-01 11:07:39.000000 vit-b16-keras-0.5/vit_b16_keras.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 11:07:39.000000 vit-b16-keras-0.5/vit_b16_keras.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-01 11:07:39.000000 vit-b16-keras-0.5/vit_b16_keras.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-01 11:07:39.000000 vit-b16-keras-0.5/vit_b16_keras.egg-info/top_level.txt
```

### Comparing `vit-b16-keras-0.4/PKG-INFO` & `vit-b16-keras-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vit-b16-keras
-Version: 0.4
+Version: 0.5
 Summary: vit-b16-keras
 Home-page: UNKNOWN
 Author: Elena Paul
 Author-email: wohani7266@dotvilla.com
 License: UNKNOWN
 Description: A package to install vision transformer
 Keywords: arithmetic,math,mathematics
```

### Comparing `vit-b16-keras-0.4/setup.py` & `vit-b16-keras-0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = '0.4'
+VERSION = '0.5'
 DESCRIPTION = 'vit-b16-keras'
 LONG_DESCRIPTION = 'A package to install vision transformer'
 
 # Setting up
 setup(
     name="vit-b16-keras",
     version=VERSION,
```

### Comparing `vit-b16-keras-0.4/vit_b16_keras.egg-info/PKG-INFO` & `vit-b16-keras-0.5/vit_b16_keras.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vit-b16-keras
-Version: 0.4
+Version: 0.5
 Summary: vit-b16-keras
 Home-page: UNKNOWN
 Author: Elena Paul
 Author-email: wohani7266@dotvilla.com
 License: UNKNOWN
 Description: A package to install vision transformer
 Keywords: arithmetic,math,mathematics
```

