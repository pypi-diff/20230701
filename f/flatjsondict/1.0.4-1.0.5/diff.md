# Comparing `tmp/flatjsondict-1.0.4.tar.gz` & `tmp/flatjsondict-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatjsondict-1.0.4.tar", max compression
+gzip compressed data, was "flatjsondict-1.0.5.tar", max compression
```

## Comparing `flatjsondict-1.0.4.tar` & `flatjsondict-1.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1497 2023-06-28 01:41:16.459729 flatjsondict-1.0.4/LICENSE
--rw-r--r--   0        0        0     3087 2023-06-28 01:41:16.459729 flatjsondict-1.0.4/README.md
--rw-r--r--   0        0        0       58 2023-06-28 01:41:16.459729 flatjsondict-1.0.4/flatjsondict/__init__.py
--rw-r--r--   0        0        0    17264 2023-06-28 01:41:16.460729 flatjsondict-1.0.4/flatjsondict/flatjsondict.py
--rw-r--r--   0        0        0      546 2023-06-28 01:41:16.460729 flatjsondict-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     3933 1970-01-01 00:00:00.000000 flatjsondict-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-07-01 04:54:47.135752 flatjsondict-1.0.5/LICENSE
+-rw-r--r--   0        0        0     3087 2023-07-01 04:54:47.135752 flatjsondict-1.0.5/README.md
+-rw-r--r--   0        0        0       58 2023-07-01 04:54:47.135752 flatjsondict-1.0.5/flatjsondict/__init__.py
+-rw-r--r--   0        0        0    17414 2023-07-01 04:54:47.136752 flatjsondict-1.0.5/flatjsondict/flatjsondict.py
+-rw-r--r--   0        0        0      546 2023-07-01 04:54:47.136752 flatjsondict-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3933 1970-01-01 00:00:00.000000 flatjsondict-1.0.5/PKG-INFO
```

### Comparing `flatjsondict-1.0.4/LICENSE` & `flatjsondict-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flatjsondict-1.0.4/README.md` & `flatjsondict-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `flatjsondict-1.0.4/flatjsondict/flatjsondict.py` & `flatjsondict-1.0.5/flatjsondict/flatjsondict.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 import logging
 from collections.abc import MutableMapping
 from typing import (
-    Optional, Union, Self, Generator
+    Optional, Union, Generator
 )
+from typing import TypeVar
+try:
+    from typing import Self
+except ImportError:
+    from typing import TypeVar
+    Self = TypeVar("Self", bound="FlatJson")
 from itertools import zip_longest
 
 logger = logging.getLogger(__name__)
 
 # -----------------------------------------------------------------------------
 # FlatJson class
```

### Comparing `flatjsondict-1.0.4/pyproject.toml` & `flatjsondict-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flatjsondict"
-version = "1.0.4"
+version = "1.0.5"
 description = "JSON-like data manipulation and transformation to and from nested parent-child and flat label-value data items."
 authors = ["Martins Bruvelis <martins.bruvelis@gmail.com>"]
 readme = "README.md"
 repository = "https://gitlab.com/martins-bruvelis/flatjsondict"
 documentation = "https://gitlab.com/martins-bruvelis/flatjsondict/-/blob/main/README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `flatjsondict-1.0.4/PKG-INFO` & `flatjsondict-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatjsondict
-Version: 1.0.4
+Version: 1.0.5
 Summary: JSON-like data manipulation and transformation to and from nested parent-child and flat label-value data items.
 Home-page: https://gitlab.com/martins-bruvelis/flatjsondict
 Author: Martins Bruvelis
 Author-email: martins.bruvelis@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

