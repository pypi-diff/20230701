# Comparing `tmp/jplaw-0.1.3.tar.gz` & `tmp/jplaw-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jplaw-0.1.3.tar", last modified: Sun Jun 25 21:08:58 2023, max compression
+gzip compressed data, was "jplaw-0.1.4.tar", last modified: Sat Jul  1 05:01:21 2023, max compression
```

## Comparing `jplaw-0.1.3.tar` & `jplaw-0.1.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:08:58.949240 jplaw-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-25 21:08:48.000000 jplaw-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-25 21:08:58.949240 jplaw-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-25 21:08:48.000000 jplaw-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:08:58.945240 jplaw-0.1.3/jplaw/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/api_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/community.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/lemmy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/post.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/private_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/requestor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16571 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:08:58.949240 jplaw-0.1.3/jplaw/types/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/types/comment_sort_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/types/http_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/types/listing_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/types/modlog_action_type.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/types/post_feature_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/types/registration_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/types/search_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/types/sort_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/types/subscribed_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-06-25 21:08:48.000000 jplaw-0.1.3/jplaw/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:08:58.949240 jplaw-0.1.3/jplaw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-25 21:08:58.000000 jplaw-0.1.3/jplaw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-25 21:08:58.000000 jplaw-0.1.3/jplaw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 21:08:58.000000 jplaw-0.1.3/jplaw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-25 21:08:58.000000 jplaw-0.1.3/jplaw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-25 21:08:58.000000 jplaw-0.1.3/jplaw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-25 21:08:48.000000 jplaw-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 21:08:58.949240 jplaw-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-25 21:08:48.000000 jplaw-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:01:21.388112 jplaw-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-01 05:01:08.000000 jplaw-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-01 05:01:21.388112 jplaw-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-01 05:01:08.000000 jplaw-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:01:21.384112 jplaw-0.1.4/jplaw/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/api_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13277 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/community.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/lemmy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15339 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/private_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/requestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29866 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:01:21.388112 jplaw-0.1.4/jplaw/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/types/comment_sort_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/types/http_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/types/listing_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/types/modlog_action_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/types/post_feature_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/types/registration_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/types/search_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/types/sort_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/types/subscribed_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21163 2023-07-01 05:01:08.000000 jplaw-0.1.4/jplaw/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:01:21.384112 jplaw-0.1.4/jplaw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-01 05:01:21.000000 jplaw-0.1.4/jplaw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-01 05:01:21.000000 jplaw-0.1.4/jplaw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 05:01:21.000000 jplaw-0.1.4/jplaw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-01 05:01:21.000000 jplaw-0.1.4/jplaw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-01 05:01:21.000000 jplaw-0.1.4/jplaw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-01 05:01:08.000000 jplaw-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 05:01:21.388112 jplaw-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-01 05:01:08.000000 jplaw-0.1.4/setup.py
```

### Comparing `jplaw-0.1.3/LICENSE` & `jplaw-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.3/PKG-INFO` & `jplaw-0.1.4/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-Metadata-Version: 2.1
-Name: jplaw
-Version: 0.1.3
-Summary: A python wrapper for the lemmy HTTP API. Forked from plaw by Benjamin Jablonski (benja810)
-Author: Amar Persaud
-Author-email: Amar Persaud <tehspartaa@gmail.com>
-Project-URL: Homepage, https://github.com/amarpersaud/python-jplaw
-Project-URL: Bug Tracker, https://github.com/amarpersaud/python-jplaw/issues
-Keywords: lemmy plaw api jplaw
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
+[build-system]
+requires = ["setuptools>=61.0", "requests >=2.6.0", "tomli>=2.0.0"]
+build-backend = "setuptools.build_meta"
 
-# Python Lemmy API Wrapper
-Like PRAW but for Lemmy
+[project]
+name = "jplaw"
+dynamic = ["version"]
+authors = [
+  { name="Amar Persaud", email="tehspartaa@gmail.com" },
+]
+description = "A python wrapper for the lemmy HTTP API. Forked from plaw by Benjamin Jablonski (benja810)"
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+[project.urls]
+"Homepage" = "https://github.com/amarpersaud/python-jplaw"
+"Bug Tracker" = "https://github.com/amarpersaud/python-jplaw/issues"
 
-Written using the [Lemmy TS library](https://github.com/LemmyNet/lemmy-js-client) for reference.
-
-Forked from benja810's plaw
-
-Currently, most of the API functions are implemented, but there are likely quite a few bugs. It is a bit difficult to test at the moment without spinning up a new instance. 
-
-If you find any bugs, let me know on the [issues page](https://github.com/amarpersaud/python-jplaw/issues)
+[tool.setuptools.dynamic]
+version = {attr = "jplaw.__version__"}
```

### Comparing `jplaw-0.1.3/jplaw/api_paths.py` & `jplaw-0.1.4/jplaw/api_paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-from .types.http_type import HttpType
+"""
+Helper variables for converting between function and API path / request type.
+"""
+
+from jplaw.types.http_type import HttpType
 
 API_VERSION = "/api/v3"
 API_PATH = {
     "login" :                               { "method": HttpType.POST    , "path": "/user/login"                            },
     "getPost" :                             { "method": HttpType.GET     , "path": "/post"                                  },
     "getCommunity" :                        { "method": HttpType.GET     , "path": "/community"                             },
     "listCommunities" :                     { "method": HttpType.GET     , "path": "/community/list"                        },
```

### Comparing `jplaw-0.1.3/jplaw/requestor.py` & `jplaw-0.1.4/jplaw/requestor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+"""
+Requestor allows HTTP communication.
+"""
 from enum import Enum
 import requests
 import json
 from typing import Dict, Any, TypeVar
-from .api_paths import *
-from .types.http_type import HttpType
+from jplaw.api_paths import *
+from jplaw.types.http_type import HttpType
 
 T = TypeVar("T")
 
 class Requestor:
     def __init__(self, instance:str, username:str, password:str, headers: Dict[str, str]):
         """
-        Make an HTTP request
+        Make an HTTP requestor
         
         Args:
             instance (str): URL of instance to log in to or use
             username (str): username or email to log in with
             password (str): password of user
             headers (Dict[str,str]): Header data
         Returns:
```

### Comparing `jplaw-0.1.3/jplaw/types/modlog_action_type.py` & `jplaw-0.1.4/jplaw/types/modlog_action_type.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.3/jplaw.egg-info/SOURCES.txt` & `jplaw-0.1.4/jplaw.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 README.md
 pyproject.toml
 setup.py
 jplaw/__init__.py
 jplaw/api_paths.py
 jplaw/comment.py
 jplaw/community.py
-jplaw/language.py
+jplaw/emoji.py
 jplaw/lemmy.py
 jplaw/post.py
 jplaw/private_message.py
 jplaw/requestor.py
 jplaw/site.py
 jplaw/user.py
 jplaw.egg-info/PKG-INFO
```

