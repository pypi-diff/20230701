# Comparing `tmp/nanorequests-0.6.tar.gz` & `tmp/nanorequests-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanorequests-0.6.tar", last modified: Sat Jul  1 07:20:51 2023, max compression
+gzip compressed data, was "nanorequests-0.7.tar", last modified: Sat Jul  1 07:31:40 2023, max compression
```

## Comparing `nanorequests-0.6.tar` & `nanorequests-0.7.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 07:20:51.412986 nanorequests-0.6/
--rw-r--r--   0 viral      (501) staff       (20)     1070 2023-06-26 15:52:46.000000 nanorequests-0.6/LICENSE.txt
--rw-r--r--   0 viral      (501) staff       (20)      356 2023-07-01 07:20:51.413055 nanorequests-0.6/PKG-INFO
--rw-r--r--   0 viral      (501) staff       (20)      136 2023-06-26 15:52:46.000000 nanorequests-0.6/README.md
-drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 07:20:51.412490 nanorequests-0.6/nanorequests.egg-info/
--rw-r--r--   0 viral      (501) staff       (20)      356 2023-07-01 07:20:51.000000 nanorequests-0.6/nanorequests.egg-info/PKG-INFO
--rw-r--r--   0 viral      (501) staff       (20)      267 2023-07-01 07:20:51.000000 nanorequests-0.6/nanorequests.egg-info/SOURCES.txt
--rw-r--r--   0 viral      (501) staff       (20)        1 2023-07-01 07:20:51.000000 nanorequests-0.6/nanorequests.egg-info/dependency_links.txt
--rw-r--r--   0 viral      (501) staff       (20)        9 2023-07-01 07:20:51.000000 nanorequests-0.6/nanorequests.egg-info/requires.txt
--rw-r--r--   0 viral      (501) staff       (20)       30 2023-07-01 07:20:51.000000 nanorequests-0.6/nanorequests.egg-info/top_level.txt
--rw-r--r--   0 viral      (501) staff       (20)     3849 2023-07-01 07:18:32.000000 nanorequests-0.6/nanorequests.py
--rw-r--r--   0 viral      (501) staff       (20)      107 2023-07-01 07:20:51.413298 nanorequests-0.6/setup.cfg
--rw-r--r--   0 viral      (501) staff       (20)      507 2023-07-01 07:19:24.000000 nanorequests-0.6/setup.py
-drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 07:20:51.412688 nanorequests-0.6/tests/
--rw-r--r--   0 viral      (501) staff       (20)        0 2023-07-01 05:12:27.000000 nanorequests-0.6/tests/__init__.py
--rw-r--r--   0 viral      (501) staff       (20)     3184 2023-07-01 07:18:32.000000 nanorequests-0.6/tests/main.py
+drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 07:31:40.387686 nanorequests-0.7/
+-rw-r--r--   0 viral      (501) staff       (20)     1070 2023-06-26 15:52:46.000000 nanorequests-0.7/LICENSE.txt
+-rw-r--r--   0 viral      (501) staff       (20)      347 2023-07-01 07:31:40.387833 nanorequests-0.7/PKG-INFO
+-rw-r--r--   0 viral      (501) staff       (20)      136 2023-06-26 15:52:46.000000 nanorequests-0.7/README.md
+drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 07:31:40.385727 nanorequests-0.7/nanorequests.egg-info/
+-rw-r--r--   0 viral      (501) staff       (20)      347 2023-07-01 07:31:40.000000 nanorequests-0.7/nanorequests.egg-info/PKG-INFO
+-rw-r--r--   0 viral      (501) staff       (20)      309 2023-07-01 07:31:40.000000 nanorequests-0.7/nanorequests.egg-info/SOURCES.txt
+-rw-r--r--   0 viral      (501) staff       (20)        1 2023-07-01 07:31:40.000000 nanorequests-0.7/nanorequests.egg-info/dependency_links.txt
+-rw-r--r--   0 viral      (501) staff       (20)        9 2023-07-01 07:31:40.000000 nanorequests-0.7/nanorequests.egg-info/requires.txt
+-rw-r--r--   0 viral      (501) staff       (20)       28 2023-07-01 07:31:40.000000 nanorequests-0.7/nanorequests.egg-info/top_level.txt
+-rw-r--r--   0 viral      (501) staff       (20)      107 2023-07-01 07:31:40.388278 nanorequests-0.7/setup.cfg
+-rw-r--r--   0 viral      (501) staff       (20)      490 2023-07-01 07:30:58.000000 nanorequests-0.7/setup.py
+drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 07:31:40.386786 nanorequests-0.7/src/
+-rw-r--r--   0 viral      (501) staff       (20)        0 2023-07-01 07:24:40.000000 nanorequests-0.7/src/__init__.py
+-rw-r--r--   0 viral      (501) staff       (20)     4164 2023-07-01 05:31:42.000000 nanorequests-0.7/src/nanoexceptions.py
+-rw-r--r--   0 viral      (501) staff       (20)     3853 2023-07-01 07:25:32.000000 nanorequests-0.7/src/nanorequests.py
+drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 07:31:40.387206 nanorequests-0.7/tests/
+-rw-r--r--   0 viral      (501) staff       (20)        0 2023-07-01 05:12:27.000000 nanorequests-0.7/tests/__init__.py
+-rw-r--r--   0 viral      (501) staff       (20)     3192 2023-07-01 07:26:05.000000 nanorequests-0.7/tests/main.py
```

### Comparing `nanorequests-0.6/LICENSE.txt` & `nanorequests-0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nanorequests-0.6/nanorequests.py` & `nanorequests-0.7/src/nanorequests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
 
-from nanoexceptions import *
+from src.nanoexceptions import *
 
 
 class NanoRequests:
     @staticmethod
     def _make_request(method, url, headers=None, json=None, timeout=None, **kwargs):
         try:
             response = method(url, headers=headers, json=json, timeout=timeout, **kwargs)
```

### Comparing `nanorequests-0.6/tests/main.py` & `nanorequests-0.7/tests/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import unittest
 from unittest import mock
 
-from nanoexceptions import (
+from src.nanoexceptions import (
     RedirectionException,
     NotFoundException,
     ForbiddenException,
     TooManyRequestsException,
     BadRequestException,
     InternalServerErrorException
 )
-from nanorequests import NanoRequests
+from src.nanorequests import NanoRequests
 
 
 def mock_requests_get(response_status_code, response_json=None, response_text=None):
     mock_response = mock.MagicMock()
     mock_response.status_code = response_status_code
     mock_response.headers.get.return_value = 'application/json'
```

