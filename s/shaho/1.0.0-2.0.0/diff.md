# Comparing `tmp/shaho-1.0.0.tar.gz` & `tmp/shaho-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaho-1.0.0.tar", last modified: Mon Jun 19 22:24:05 2023, max compression
+gzip compressed data, was "shaho-2.0.0.tar", last modified: Sat Jul  1 21:33:17 2023, max compression
```

## Comparing `shaho-1.0.0.tar` & `shaho-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,14 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-19 22:24:05.632726 shaho-1.0.0/
--rw-rw----   0 root         (0) everybody  (9997)     1081 2023-06-19 22:22:31.000000 shaho-1.0.0/LICENCE
--rw-rw----   0 root         (0) everybody  (9997)      902 2023-06-19 22:24:05.602726 shaho-1.0.0/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)        8 2023-06-19 22:20:40.000000 shaho-1.0.0/README.md
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-19 22:24:05.632726 shaho-1.0.0/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1059 2023-06-19 22:20:00.000000 shaho-1.0.0/setup.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-19 22:24:05.432726 shaho-1.0.0/shaho/
--rw-rw----   0 root         (0) everybody  (9997)      443 2022-11-20 12:25:14.000000 shaho-1.0.0/shaho/Device.py
--rw-rw----   0 root         (0) everybody  (9997)     1311 2022-11-20 12:25:14.000000 shaho-1.0.0/shaho/WebAdress.py
--rw-rw----   0 root         (0) everybody  (9997)       14 2023-06-19 22:14:59.000000 shaho-1.0.0/shaho/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)      375 2022-11-20 12:25:14.000000 shaho-1.0.0/shaho/clines_ph_web.py
--rw-rw----   0 root         (0) everybody  (9997)       52 2023-06-19 22:15:39.000000 shaho-1.0.0/shaho/copyright.py
--rw-rw----   0 root         (0) everybody  (9997)     1954 2022-11-20 12:25:14.000000 shaho-1.0.0/shaho/encoder.py
--rw-rw----   0 root         (0) everybody  (9997)    77456 2023-06-19 22:14:40.000000 shaho-1.0.0/shaho/mb.py
--rw-rw----   0 root         (0) everybody  (9997)      293 2023-06-19 22:17:00.000000 shaho-1.0.0/shaho/send_server.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-19 22:24:05.572726 shaho-1.0.0/shaho.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      902 2023-06-19 22:24:04.000000 shaho-1.0.0/shaho.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      287 2023-06-19 22:24:04.000000 shaho-1.0.0/shaho.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-19 22:24:04.000000 shaho-1.0.0/shaho.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)        6 2023-06-19 22:24:04.000000 shaho-1.0.0/shaho.egg-info/top_level.txt
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-01 21:33:17.149191 shaho-2.0.0/
+-rw-rw----   0 root         (0) everybody  (9997)     1081 2023-06-19 22:22:31.000000 shaho-2.0.0/LICENCE
+-rw-rw----   0 root         (0) everybody  (9997)      902 2023-07-01 21:33:17.119191 shaho-2.0.0/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)        8 2023-06-19 22:20:40.000000 shaho-2.0.0/README.md
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-01 21:33:17.149191 shaho-2.0.0/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1059 2023-07-01 21:06:13.000000 shaho-2.0.0/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-01 21:33:16.939190 shaho-2.0.0/shaho/
+-rw-rw----   0 root         (0) everybody  (9997)       14 2023-06-19 22:14:59.000000 shaho-2.0.0/shaho/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    18290 2023-07-01 21:30:03.000000 shaho-2.0.0/shaho/mb.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-01 21:33:17.099191 shaho-2.0.0/shaho.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      902 2023-07-01 21:33:16.000000 shaho-2.0.0/shaho.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      172 2023-07-01 21:33:16.000000 shaho-2.0.0/shaho.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-01 21:33:16.000000 shaho-2.0.0/shaho.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)        6 2023-07-01 21:33:16.000000 shaho-2.0.0/shaho.egg-info/top_level.txt
```

### Comparing `shaho-1.0.0/LICENCE` & `shaho-2.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `shaho-1.0.0/PKG-INFO` & `shaho-2.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaho
-Version: 1.0.0
+Version: 2.0.0
 Summary:  library Robot
 Home-page: https://github.com
 Author: shaho
 Author-email: mbshahoorg@gmail.com
 License: MIT
 Keywords: shaho,Shaho
 Platform: UNKNOWN
```

### Comparing `shaho-1.0.0/setup.py` & `shaho-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import re
 from setuptools import setup
 
 _long_description = open('README.md').read()
 
 setup(
     name = "shaho",
-    version = "1.0.0",
+    version = "2.0.0",
     author = "shaho",
     author_email = "mbshahoorg@gmail.com",
     description = (" library Robot"),
     license = "MIT",
     keywords = ["shaho","Shaho"],
     url = "https://github.com",
     packages=['shaho'],
```

### Comparing `shaho-1.0.0/shaho.egg-info/PKG-INFO` & `shaho-2.0.0/shaho.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaho
-Version: 1.0.0
+Version: 2.0.0
 Summary:  library Robot
 Home-page: https://github.com
 Author: shaho
 Author-email: mbshahoorg@gmail.com
 License: MIT
 Keywords: shaho,Shaho
 Platform: UNKNOWN
```

