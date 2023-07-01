# Comparing `tmp/statute_utils-0.5.0.tar.gz` & `tmp/statute_utils-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statute_utils-0.5.0.tar", max compression
+gzip compressed data, was "statute_utils-0.5.1.tar", max compression
```

## Comparing `statute_utils-0.5.0.tar` & `statute_utils-0.5.1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.5.0/LICENSE
--rw-r--r--   0        0        0      898 2023-07-01 01:29:45.722010 statute_utils-0.5.0/README.md
--rw-r--r--   0        0        0     1297 2023-07-01 04:37:03.663696 statute_utils-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      431 2023-07-01 04:37:03.664040 statute_utils-0.5.0/statute_utils/__init__.py
--rw-r--r--   0        0        0      310 2023-07-01 04:37:03.664324 statute_utils-0.5.0/statute_utils/components/__init__.py
--rw-r--r--   0        0        0     9093 2023-07-01 04:37:03.664630 statute_utils-0.5.0/statute_utils/components/category.py
--rw-r--r--   0        0        0     1150 2023-07-01 04:37:03.664832 statute_utils-0.5.0/statute_utils/components/rule.py
--rw-r--r--   0        0        0     2015 2023-07-01 04:37:03.664929 statute_utils-0.5.0/statute_utils/components/short.py
--rw-r--r--   0        0        0     4683 2023-07-01 04:37:03.665122 statute_utils-0.5.0/statute_utils/components/utils.py
--rw-r--r--   0        0        0     7805 2023-07-01 04:37:03.665405 statute_utils-0.5.0/statute_utils/main.py
--rw-r--r--   0        0        0     2500 2023-07-01 04:37:03.665660 statute_utils-0.5.0/statute_utils/models.py
--rw-r--r--   0        0        0    13202 2023-07-01 04:37:03.665877 statute_utils-0.5.0/statute_utils/models_names.py
--rw-r--r--   0        0        0     6682 2023-07-01 04:37:03.666097 statute_utils-0.5.0/statute_utils/models_serials.py
--rw-r--r--   0        0        0      249 2023-07-01 04:12:57.597987 statute_utils-0.5.0/statute_utils/recipes/__init__.py
--rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.5.0/statute_utils/recipes/const.py
--rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.5.0/statute_utils/recipes/digits.py
--rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.5.0/statute_utils/recipes/roc.py
--rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.5.0/statute_utils/recipes/spain.py
--rw-r--r--   0        0        0     4739 2023-07-01 04:37:03.666304 statute_utils-0.5.0/statute_utils/tree.py
--rw-r--r--   0        0        0     1618 1970-01-01 00:00:00.000000 statute_utils-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.5.1/LICENSE
+-rw-r--r--   0        0        0      898 2023-07-01 01:29:45.722010 statute_utils-0.5.1/README.md
+-rw-r--r--   0        0        0     1320 2023-07-01 05:30:27.557835 statute_utils-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      457 2023-07-01 06:23:31.949055 statute_utils-0.5.1/statute_utils/__init__.py
+-rw-r--r--   0        0        0      275 2023-07-01 05:31:15.495445 statute_utils-0.5.1/statute_utils/components/__init__.py
+-rw-r--r--   0        0        0     9093 2023-07-01 04:37:03.664630 statute_utils-0.5.1/statute_utils/components/category.py
+-rw-r--r--   0        0        0     2015 2023-07-01 04:37:03.664929 statute_utils-0.5.1/statute_utils/components/short.py
+-rw-r--r--   0        0        0     4683 2023-07-01 04:37:03.665122 statute_utils-0.5.1/statute_utils/components/utils.py
+-rw-r--r--   0        0        0     9658 2023-07-01 06:55:45.539814 statute_utils-0.5.1/statute_utils/main.py
+-rw-r--r--   0        0        0     5022 2023-07-01 06:44:19.410593 statute_utils-0.5.1/statute_utils/models.py
+-rw-r--r--   0        0        0     9962 2023-07-01 06:48:01.652846 statute_utils-0.5.1/statute_utils/models_names.py
+-rw-r--r--   0        0        0     6682 2023-07-01 06:21:01.765608 statute_utils-0.5.1/statute_utils/models_serials.py
+-rw-r--r--   0        0        0      249 2023-07-01 04:12:57.597987 statute_utils-0.5.1/statute_utils/recipes/__init__.py
+-rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.5.1/statute_utils/recipes/const.py
+-rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.5.1/statute_utils/recipes/digits.py
+-rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.5.1/statute_utils/recipes/roc.py
+-rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.5.1/statute_utils/recipes/spain.py
+-rw-r--r--   0        0        0     4709 2023-07-01 06:20:32.418706 statute_utils-0.5.1/statute_utils/tree.py
+-rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 statute_utils-0.5.1/PKG-INFO
```

### Comparing `statute_utils-0.5.0/LICENSE` & `statute_utils-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.0/README.md` & `statute_utils-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.0/pyproject.toml` & `statute_utils-0.5.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "statute-utils"
-version = "0.5.0"
+version = "0.5.1"
 description = "Philippine statutory law pattern matching and unit retrieval."
 authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 readme = "README.md"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/statute-utils"
 documentation = "https://justmars.github.io/statute-utils"
 classifiers = [
@@ -14,14 +14,15 @@
   "Intended Audience :: Legal Industry",
   "Framework :: Pytest",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 python-slugify = "^8.0"
+sqlite-utils = "^3.33"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3"
 pytest-cov = "^2.12.1"
 pre-commit = "^3.3"
 mkdocs = "^1.4.3"
 mkdocstrings = {extras = ["python"], version = "^0.22.0"}
```

### Comparing `statute_utils-0.5.0/statute_utils/components/category.py` & `statute_utils-0.5.1/statute_utils/components/category.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.0/statute_utils/components/short.py` & `statute_utils-0.5.1/statute_utils/components/short.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.0/statute_utils/components/utils.py` & `statute_utils-0.5.1/statute_utils/components/utils.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.0/statute_utils/models_serials.py` & `statute_utils-0.5.1/statute_utils/models_serials.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.0/statute_utils/recipes/digits.py` & `statute_utils-0.5.1/statute_utils/recipes/digits.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.0/statute_utils/recipes/spain.py` & `statute_utils-0.5.1/statute_utils/recipes/spain.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.0/statute_utils/tree.py` & `statute_utils-0.5.1/statute_utils/tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import datetime
 from collections.abc import Iterator
 from pathlib import Path
 from typing import NamedTuple
 
 import yaml
 
-from .components import Rule, StatuteSerialCategory, StatuteTitle, set_node_ids, walk
-
-STATUTE_DIR = Path().home().joinpath("code/corpus-statutes")
+from .components import StatuteSerialCategory, StatuteTitle, set_node_ids, walk
+from .models import STATUTE_DIR, Rule
 
 
 class Statute(NamedTuple):
     """A instance is dependent on a statute path from a fixed
     `STATUTE_DIR`. The shape of the Python object will be different
     from the shape of the dumpable `.yml` export."""
```

### Comparing `statute_utils-0.5.0/PKG-INFO` & `statute_utils-0.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: statute-utils
-Version: 0.5.0
+Version: 0.5.1
 Summary: Philippine statutory law pattern matching and unit retrieval.
 Home-page: https://lawsql.com
 Author: Marcelino G. Veloso III
 Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Legal Industry
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Dist: python-slugify (>=8.0,<9.0)
+Requires-Dist: sqlite-utils (>=3.33,<4.0)
 Project-URL: Documentation, https://justmars.github.io/statute-utils
 Project-URL: Repository, https://github.com/justmars/statute-utils
 Description-Content-Type: text/markdown
 
 # statute-utils
 
 ![Github CI](https://github.com/justmars/statute-utils/actions/workflows/main.yml/badge.svg)
```

