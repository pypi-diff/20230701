# Comparing `tmp/nanorequests-0.4.tar.gz` & `tmp/nanorequests-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanorequests-0.4.tar", last modified: Sat Jul  1 07:01:09 2023, max compression
+gzip compressed data, was "nanorequests-0.5.tar", last modified: Sat Jul  1 07:14:48 2023, max compression
```

## Comparing `nanorequests-0.4.tar` & `nanorequests-0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 07:01:09.002962 nanorequests-0.4/
--rw-r--r--   0 viral      (501) staff       (20)     1070 2023-06-26 15:52:46.000000 nanorequests-0.4/LICENSE.txt
--rw-r--r--   0 viral      (501) staff       (20)      356 2023-07-01 07:01:09.003031 nanorequests-0.4/PKG-INFO
--rw-r--r--   0 viral      (501) staff       (20)      136 2023-06-26 15:52:46.000000 nanorequests-0.4/README.md
-drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 07:01:09.002514 nanorequests-0.4/nanorequests.egg-info/
--rw-r--r--   0 viral      (501) staff       (20)      356 2023-07-01 07:01:08.000000 nanorequests-0.4/nanorequests.egg-info/PKG-INFO
--rw-r--r--   0 viral      (501) staff       (20)      267 2023-07-01 07:01:08.000000 nanorequests-0.4/nanorequests.egg-info/SOURCES.txt
--rw-r--r--   0 viral      (501) staff       (20)        1 2023-07-01 07:01:08.000000 nanorequests-0.4/nanorequests.egg-info/dependency_links.txt
--rw-r--r--   0 viral      (501) staff       (20)        9 2023-07-01 07:01:08.000000 nanorequests-0.4/nanorequests.egg-info/requires.txt
--rw-r--r--   0 viral      (501) staff       (20)       13 2023-07-01 07:01:08.000000 nanorequests-0.4/nanorequests.egg-info/top_level.txt
--rw-r--r--   0 viral      (501) staff       (20)     3844 2023-07-01 06:03:28.000000 nanorequests-0.4/nanorequests.py
--rw-r--r--   0 viral      (501) staff       (20)      107 2023-07-01 07:01:09.003267 nanorequests-0.4/setup.cfg
--rw-r--r--   0 viral      (501) staff       (20)      463 2023-07-01 07:00:34.000000 nanorequests-0.4/setup.py
-drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 07:01:09.002745 nanorequests-0.4/tests/
--rw-r--r--   0 viral      (501) staff       (20)        0 2023-07-01 05:12:27.000000 nanorequests-0.4/tests/__init__.py
--rw-r--r--   0 viral      (501) staff       (20)     3180 2023-07-01 06:03:28.000000 nanorequests-0.4/tests/main.py
+drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 07:14:48.576195 nanorequests-0.5/
+-rw-r--r--   0 viral      (501) staff       (20)     1070 2023-06-26 15:52:46.000000 nanorequests-0.5/LICENSE.txt
+-rw-r--r--   0 viral      (501) staff       (20)      356 2023-07-01 07:14:48.576253 nanorequests-0.5/PKG-INFO
+-rw-r--r--   0 viral      (501) staff       (20)      136 2023-06-26 15:52:46.000000 nanorequests-0.5/README.md
+drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 07:14:48.575225 nanorequests-0.5/nanorequests.egg-info/
+-rw-r--r--   0 viral      (501) staff       (20)      356 2023-07-01 07:14:48.000000 nanorequests-0.5/nanorequests.egg-info/PKG-INFO
+-rw-r--r--   0 viral      (501) staff       (20)      267 2023-07-01 07:14:48.000000 nanorequests-0.5/nanorequests.egg-info/SOURCES.txt
+-rw-r--r--   0 viral      (501) staff       (20)        1 2023-07-01 07:14:48.000000 nanorequests-0.5/nanorequests.egg-info/dependency_links.txt
+-rw-r--r--   0 viral      (501) staff       (20)        9 2023-07-01 07:14:48.000000 nanorequests-0.5/nanorequests.egg-info/requires.txt
+-rw-r--r--   0 viral      (501) staff       (20)       13 2023-07-01 07:14:48.000000 nanorequests-0.5/nanorequests.egg-info/top_level.txt
+-rw-r--r--   0 viral      (501) staff       (20)     3846 2023-07-01 07:12:41.000000 nanorequests-0.5/nanorequests.py
+-rw-r--r--   0 viral      (501) staff       (20)      107 2023-07-01 07:14:48.576506 nanorequests-0.5/setup.cfg
+-rw-r--r--   0 viral      (501) staff       (20)      463 2023-07-01 07:14:33.000000 nanorequests-0.5/setup.py
+drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 07:14:48.575419 nanorequests-0.5/tests/
+-rw-r--r--   0 viral      (501) staff       (20)        0 2023-07-01 05:12:27.000000 nanorequests-0.5/tests/__init__.py
+-rw-r--r--   0 viral      (501) staff       (20)     3180 2023-07-01 06:03:28.000000 nanorequests-0.5/tests/main.py
```

### Comparing `nanorequests-0.4/LICENSE.txt` & `nanorequests-0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nanorequests-0.4/nanorequests.py` & `nanorequests-0.5/nanorequests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import requests
-from exceptions import *
+
+from .exceptions import *
 
 
 class NanoRequests:
     @staticmethod
     def _make_request(method, url, headers=None, json=None, timeout=None, **kwargs):
         try:
             response = method(url, headers=headers, json=json, timeout=timeout, **kwargs)
```

### Comparing `nanorequests-0.4/tests/main.py` & `nanorequests-0.5/tests/main.py`

 * *Files identical despite different names*

