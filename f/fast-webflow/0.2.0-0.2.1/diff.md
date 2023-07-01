# Comparing `tmp/fast-webflow-0.2.0.tar.gz` & `tmp/fast-webflow-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-webflow-0.2.0.tar", last modified: Sat Jul  1 16:30:27 2023, max compression
+gzip compressed data, was "fast-webflow-0.2.1.tar", last modified: Sat Jul  1 17:20:38 2023, max compression
```

## Comparing `fast-webflow-0.2.0.tar` & `fast-webflow-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:30:27.803835 fast-webflow-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 16:30:18.000000 fast-webflow-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-01 16:30:27.803835 fast-webflow-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-01 16:30:18.000000 fast-webflow-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-01 16:30:18.000000 fast-webflow-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-01 16:30:27.803835 fast-webflow-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:30:27.803835 fast-webflow-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:30:27.803835 fast-webflow-0.2.0/src/cms/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-01 16:30:18.000000 fast-webflow-0.2.0/src/cms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-01 16:30:18.000000 fast-webflow-0.2.0/src/cms/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-01 16:30:18.000000 fast-webflow-0.2.0/src/cms/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-01 16:30:18.000000 fast-webflow-0.2.0/src/cms/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-01 16:30:18.000000 fast-webflow-0.2.0/src/cms/site.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-01 16:30:18.000000 fast-webflow-0.2.0/src/cms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:30:27.803835 fast-webflow-0.2.0/src/fast_webflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-01 16:30:27.000000 fast-webflow-0.2.0/src/fast_webflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-01 16:30:27.000000 fast-webflow-0.2.0/src/fast_webflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 16:30:27.000000 fast-webflow-0.2.0/src/fast_webflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-01 16:30:27.000000 fast-webflow-0.2.0/src/fast_webflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:20:38.891965 fast-webflow-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 17:20:24.000000 fast-webflow-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-01 17:20:38.891965 fast-webflow-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-01 17:20:24.000000 fast-webflow-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-01 17:20:24.000000 fast-webflow-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-01 17:20:38.891965 fast-webflow-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:20:38.887965 fast-webflow-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:20:38.891965 fast-webflow-0.2.1/src/cms/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-01 17:20:24.000000 fast-webflow-0.2.1/src/cms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-01 17:20:24.000000 fast-webflow-0.2.1/src/cms/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-01 17:20:24.000000 fast-webflow-0.2.1/src/cms/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-01 17:20:24.000000 fast-webflow-0.2.1/src/cms/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-01 17:20:24.000000 fast-webflow-0.2.1/src/cms/site.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-01 17:20:24.000000 fast-webflow-0.2.1/src/cms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:20:38.891965 fast-webflow-0.2.1/src/fast_webflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-01 17:20:38.000000 fast-webflow-0.2.1/src/fast_webflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-01 17:20:38.000000 fast-webflow-0.2.1/src/fast_webflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 17:20:38.000000 fast-webflow-0.2.1/src/fast_webflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-01 17:20:38.000000 fast-webflow-0.2.1/src/fast_webflow.egg-info/top_level.txt
```

### Comparing `fast-webflow-0.2.0/LICENSE` & `fast-webflow-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.2.0/setup.cfg` & `fast-webflow-0.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fast-webflow
-version = 0.2.0
+version = 0.2.1
 author = Thomas Cilloni
 author_email = tcilloni@outlook.com
 description = A client library to communicate with the WebFlow API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tcilloni/fast-webflow
 project_urls =
```

### Comparing `fast-webflow-0.2.0/src/cms/collection.py` & `fast-webflow-0.2.1/src/cms/collection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import requests
 from collections import UserDict
+from functools import partial
+from itertools import repeat
 
 from .utils import string_to_dict, slugify, try_request, parallelize
 from .config import make_headers
 
 
 class Collection(UserDict):
     id: str
@@ -38,14 +40,21 @@
     def post_item(self, fields: dict[str,any], draft: bool = False):
         payload = {'fields': {'_archived': False, '_draft': draft}}
         payload['fields'].update(fields)
 
         data = self._request(requests.post, self._items_url, payload)
         
         return data
+    
+
+    def post_items(self, fields_list: list[dict[str,any]], draft: bool = False):
+        post_item = partial(self.post_item, draft = draft)
+        data = parallelize(post_item, fields_list)
+        
+        return data
 
 
     def publish_items(self, item_ids: list[str]) -> dict:
         max_items = self._max_items_per_request  # API rule
         url = self._url + '/items/publish'
         data = {}
```

### Comparing `fast-webflow-0.2.0/src/cms/config.py` & `fast-webflow-0.2.1/src/cms/config.py`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.2.0/src/cms/item.py` & `fast-webflow-0.2.1/src/cms/item.py`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.2.0/src/cms/site.py` & `fast-webflow-0.2.1/src/cms/site.py`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.2.0/src/cms/utils.py` & `fast-webflow-0.2.1/src/cms/utils.py`

 * *Files identical despite different names*

