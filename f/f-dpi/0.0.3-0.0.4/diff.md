# Comparing `tmp/f_dpi-0.0.3.tar.gz` & `tmp/f_dpi-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f_dpi-0.0.3.tar", last modified: Sat Jul  1 06:43:43 2023, max compression
+gzip compressed data, was "f_dpi-0.0.4.tar", last modified: Sat Jul  1 06:48:25 2023, max compression
```

## Comparing `f_dpi-0.0.3.tar` & `f_dpi-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 06:43:43.720578 f_dpi-0.0.3/
--rw-rw-rw-   0        0        0      147 2023-07-01 06:43:43.720578 f_dpi-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-04-17 20:39:54.000000 f_dpi-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 06:43:43.709824 f_dpi-0.0.3/f_dpi/
--rw-rw-rw-   0        0        0       62 2023-07-01 06:26:53.000000 f_dpi-0.0.3/f_dpi/__init__.py
--rw-rw-rw-   0        0        0       21 2023-07-01 06:43:32.000000 f_dpi-0.0.3/f_dpi/__version__.py
--rw-rw-rw-   0        0        0     1428 2023-07-01 06:35:23.000000 f_dpi-0.0.3/f_dpi/f_dpi.py
-drwxrwxrwx   0        0        0        0 2023-07-01 06:43:43.719577 f_dpi-0.0.3/f_dpi.egg-info/
--rw-rw-rw-   0        0        0      147 2023-07-01 06:43:43.000000 f_dpi-0.0.3/f_dpi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-07-01 06:43:43.000000 f_dpi-0.0.3/f_dpi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 06:43:43.000000 f_dpi-0.0.3/f_dpi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-07-01 06:43:43.000000 f_dpi-0.0.3/f_dpi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-01 06:43:43.000000 f_dpi-0.0.3/f_dpi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-01 06:43:43.721577 f_dpi-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      523 2023-07-01 06:43:41.000000 f_dpi-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 06:48:25.474054 f_dpi-0.0.4/
+-rw-rw-rw-   0        0        0      147 2023-07-01 06:48:25.474054 f_dpi-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-04-17 20:39:54.000000 f_dpi-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 06:48:25.460734 f_dpi-0.0.4/f_dpi/
+-rw-rw-rw-   0        0        0       62 2023-07-01 06:26:53.000000 f_dpi-0.0.4/f_dpi/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-07-01 06:48:02.000000 f_dpi-0.0.4/f_dpi/__version__.py
+-rw-rw-rw-   0        0        0     1427 2023-07-01 06:44:42.000000 f_dpi-0.0.4/f_dpi/f_dpi.py
+drwxrwxrwx   0        0        0        0 2023-07-01 06:48:25.473044 f_dpi-0.0.4/f_dpi.egg-info/
+-rw-rw-rw-   0        0        0      147 2023-07-01 06:48:25.000000 f_dpi-0.0.4/f_dpi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-07-01 06:48:25.000000 f_dpi-0.0.4/f_dpi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 06:48:25.000000 f_dpi-0.0.4/f_dpi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 06:48:25.000000 f_dpi-0.0.4/f_dpi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-01 06:48:25.000000 f_dpi-0.0.4/f_dpi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-01 06:48:25.475054 f_dpi-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      523 2023-07-01 06:48:10.000000 f_dpi-0.0.4/setup.py
```

### Comparing `f_dpi-0.0.3/f_dpi/f_dpi.py` & `f_dpi-0.0.4/f_dpi/f_dpi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import cv2
 from PIL import Image, ImageDraw
-import nuympy as np
+import numpy as np
 
 def test():
 	print('test success')
 
 def imshow(img):
     cv2.imshow('image', img)
     cv2.waitKey()
```

### Comparing `f_dpi-0.0.3/setup.py` & `f_dpi-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name                = 'f_dpi',
-    version             = '0.0.3',
+    version             = '0.0.4',
     author              = 'jskim1102',
     author_email        = 'deepi.contact.us@gmail.com',
     long_description=long_description,
     install_requires    =  requirements,
     packages=setuptools.find_packages(),
     python_requires     = '>=3.8',
 )
```

