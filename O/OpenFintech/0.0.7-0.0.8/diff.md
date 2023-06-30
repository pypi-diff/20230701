# Comparing `tmp/OpenFintech-0.0.7.tar.gz` & `tmp/OpenFintech-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenFintech-0.0.7.tar", last modified: Thu Jun 29 04:49:33 2023, max compression
+gzip compressed data, was "OpenFintech-0.0.8.tar", last modified: Fri Jun 30 23:20:09 2023, max compression
```

## Comparing `OpenFintech-0.0.7.tar` & `OpenFintech-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-06-29 04:49:33.104587 OpenFintech-0.0.7/
--rw-r--r--   0 harri      (501) staff       (20)    11357 2023-06-05 19:27:30.000000 OpenFintech-0.0.7/LICENSE
-drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-06-29 04:49:33.103130 OpenFintech-0.0.7/OpenFintech/
--rw-r--r--   0 harri      (501) staff       (20)     3013 2023-06-29 04:44:15.000000 OpenFintech-0.0.7/OpenFintech/FinData.py
--rw-r--r--   0 harri      (501) staff       (20)     3626 2023-06-29 04:44:16.000000 OpenFintech-0.0.7/OpenFintech/FinMongo.py
--rw-r--r--   0 harri      (501) staff       (20)     2407 2023-06-29 04:44:51.000000 OpenFintech-0.0.7/OpenFintech/Market.py
--rw-r--r--   0 harri      (501) staff       (20)     5495 2023-06-29 04:45:07.000000 OpenFintech-0.0.7/OpenFintech/Model.py
--rw-r--r--   0 harri      (501) staff       (20)     7475 2023-06-29 04:48:07.000000 OpenFintech-0.0.7/OpenFintech/User.py
--rw-r--r--   0 harri      (501) staff       (20)      185 2023-06-29 04:43:38.000000 OpenFintech-0.0.7/OpenFintech/__init__.py
--rw-r--r--   0 harri      (501) staff       (20)      855 2023-06-29 04:42:17.000000 OpenFintech-0.0.7/OpenFintech/utilities.py
-drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-06-29 04:49:33.104126 OpenFintech-0.0.7/OpenFintech.egg-info/
--rw-r--r--   0 harri      (501) staff       (20)       77 2023-06-29 04:49:33.000000 OpenFintech-0.0.7/OpenFintech.egg-info/PKG-INFO
--rw-r--r--   0 harri      (501) staff       (20)      325 2023-06-29 04:49:33.000000 OpenFintech-0.0.7/OpenFintech.egg-info/SOURCES.txt
--rw-r--r--   0 harri      (501) staff       (20)        1 2023-06-29 04:49:33.000000 OpenFintech-0.0.7/OpenFintech.egg-info/dependency_links.txt
--rw-r--r--   0 harri      (501) staff       (20)       12 2023-06-29 04:49:33.000000 OpenFintech-0.0.7/OpenFintech.egg-info/top_level.txt
--rw-r--r--   0 harri      (501) staff       (20)       77 2023-06-29 04:49:33.104393 OpenFintech-0.0.7/PKG-INFO
--rw-r--r--   0 harri      (501) staff       (20)    11338 2023-06-13 17:15:54.000000 OpenFintech-0.0.7/README.md
--rw-r--r--   0 harri      (501) staff       (20)       38 2023-06-29 04:49:33.104645 OpenFintech-0.0.7/setup.cfg
--rw-r--r--   0 harri      (501) staff       (20)      128 2023-06-29 04:48:17.000000 OpenFintech-0.0.7/setup.py
+drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-06-30 23:20:09.291715 OpenFintech-0.0.8/
+-rw-r--r--   0 harri      (501) staff       (20)    11357 2023-06-05 19:27:30.000000 OpenFintech-0.0.8/LICENSE
+drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-06-30 23:20:09.290403 OpenFintech-0.0.8/OpenFintech/
+-rw-r--r--   0 harri      (501) staff       (20)     6253 2023-06-30 23:16:16.000000 OpenFintech-0.0.8/OpenFintech/FinData.py
+-rw-r--r--   0 harri      (501) staff       (20)     3643 2023-06-30 18:57:40.000000 OpenFintech-0.0.8/OpenFintech/FinMongo.py
+-rw-r--r--   0 harri      (501) staff       (20)     2407 2023-06-30 20:43:07.000000 OpenFintech-0.0.8/OpenFintech/Market.py
+-rw-r--r--   0 harri      (501) staff       (20)     5495 2023-06-30 20:43:08.000000 OpenFintech-0.0.8/OpenFintech/Model.py
+-rw-r--r--   0 harri      (501) staff       (20)     7511 2023-06-30 18:57:40.000000 OpenFintech-0.0.8/OpenFintech/User.py
+-rw-r--r--   0 harri      (501) staff       (20)      225 2023-06-30 18:57:40.000000 OpenFintech-0.0.8/OpenFintech/__init__.py
+-rw-r--r--   0 harri      (501) staff       (20)      855 2023-06-30 18:57:40.000000 OpenFintech-0.0.8/OpenFintech/utilities.py
+drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-06-30 23:20:09.291303 OpenFintech-0.0.8/OpenFintech.egg-info/
+-rw-r--r--   0 harri      (501) staff       (20)       77 2023-06-30 23:20:09.000000 OpenFintech-0.0.8/OpenFintech.egg-info/PKG-INFO
+-rw-r--r--   0 harri      (501) staff       (20)      325 2023-06-30 23:20:09.000000 OpenFintech-0.0.8/OpenFintech.egg-info/SOURCES.txt
+-rw-r--r--   0 harri      (501) staff       (20)        1 2023-06-30 23:20:09.000000 OpenFintech-0.0.8/OpenFintech.egg-info/dependency_links.txt
+-rw-r--r--   0 harri      (501) staff       (20)       12 2023-06-30 23:20:09.000000 OpenFintech-0.0.8/OpenFintech.egg-info/top_level.txt
+-rw-r--r--   0 harri      (501) staff       (20)       77 2023-06-30 23:20:09.291542 OpenFintech-0.0.8/PKG-INFO
+-rw-r--r--   0 harri      (501) staff       (20)    11338 2023-06-13 17:15:54.000000 OpenFintech-0.0.8/README.md
+-rw-r--r--   0 harri      (501) staff       (20)       38 2023-06-30 23:20:09.291765 OpenFintech-0.0.8/setup.cfg
+-rw-r--r--   0 harri      (501) staff       (20)      128 2023-06-30 23:19:42.000000 OpenFintech-0.0.8/setup.py
```

### Comparing `OpenFintech-0.0.7/LICENSE` & `OpenFintech-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenFintech-0.0.7/OpenFintech/FinMongo.py` & `OpenFintech-0.0.8/OpenFintech/FinMongo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 import pymongo_inmemory
 from pymongo import MongoClient, errors
 from .utilities import create_logger
 # TODO: 
+# Finish __str__
 # Add CRUD features (with returns optionally in Pandas DF's)
 # Add custom error message returns (dict/JSON like an API would)
 
 class FinMongo:
 
     def __init__(self, host: str = None, logger:logging.Logger = None):
```

### Comparing `OpenFintech-0.0.7/OpenFintech/Market.py` & `OpenFintech-0.0.8/OpenFintech/Market.py`

 * *Files identical despite different names*

### Comparing `OpenFintech-0.0.7/OpenFintech/Model.py` & `OpenFintech-0.0.8/OpenFintech/Model.py`

 * *Files identical despite different names*

### Comparing `OpenFintech-0.0.7/OpenFintech/User.py` & `OpenFintech-0.0.8/OpenFintech/User.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from datetime import datetime as dt
 from .FinMongo import FinMongo
 from .utilities import create_logger
 # TODO:
 # Add functionality to insert many users (data in create_users could be a list of dict's)
 # Improve data validation (e.x., email format validation) 
 
 class User:
```

### Comparing `OpenFintech-0.0.7/OpenFintech/utilities.py` & `OpenFintech-0.0.8/OpenFintech/utilities.py`

 * *Files identical despite different names*

### Comparing `OpenFintech-0.0.7/README.md` & `OpenFintech-0.0.8/README.md`

 * *Files identical despite different names*

