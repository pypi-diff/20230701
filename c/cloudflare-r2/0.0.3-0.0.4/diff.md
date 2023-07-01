# Comparing `tmp/cloudflare_r2-0.0.3.tar.gz` & `tmp/cloudflare_r2-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudflare_r2-0.0.3.tar", max compression
+gzip compressed data, was "cloudflare_r2-0.0.4.tar", max compression
```

## Comparing `cloudflare_r2-0.0.3.tar` & `cloudflare_r2-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1491 2023-06-14 11:00:13.758722 cloudflare_r2-0.0.3/LICENSE
--rw-r--r--   0        0        0      253 2023-06-14 11:00:13.758802 cloudflare_r2-0.0.3/README.md
--rw-r--r--   0        0        0       51 2023-06-22 03:03:18.531837 cloudflare_r2-0.0.3/cloudflare_r2/__init__.py
--rw-r--r--   0        0        0     8191 2023-06-22 03:03:18.532194 cloudflare_r2-0.0.3/cloudflare_r2/main.py
--rw-r--r--   0        0        0      824 2023-06-22 03:03:18.532406 cloudflare_r2-0.0.3/cloudflare_r2/nb.ipynb
--rw-r--r--   0        0        0     1280 2023-06-22 03:03:18.532729 cloudflare_r2-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      968 1970-01-01 00:00:00.000000 cloudflare_r2-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-14 11:00:13.758722 cloudflare_r2-0.0.4/LICENSE
+-rw-r--r--   0        0        0      253 2023-06-14 11:00:13.758802 cloudflare_r2-0.0.4/README.md
+-rw-r--r--   0        0        0       51 2023-06-22 03:03:18.531837 cloudflare_r2-0.0.4/cloudflare_r2/__init__.py
+-rw-r--r--   0        0        0     8191 2023-06-22 03:03:18.532194 cloudflare_r2-0.0.4/cloudflare_r2/main.py
+-rw-r--r--   0        0        0      824 2023-06-22 03:03:18.532406 cloudflare_r2-0.0.4/cloudflare_r2/nb.ipynb
+-rw-r--r--   0        0        0     1280 2023-07-01 03:44:13.111327 cloudflare_r2-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      968 1970-01-01 00:00:00.000000 cloudflare_r2-0.0.4/PKG-INFO
```

### Comparing `cloudflare_r2-0.0.3/LICENSE` & `cloudflare_r2-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudflare_r2-0.0.3/cloudflare_r2/main.py` & `cloudflare_r2-0.0.4/cloudflare_r2/main.py`

 * *Files identical despite different names*

### Comparing `cloudflare_r2-0.0.3/cloudflare_r2/nb.ipynb` & `cloudflare_r2-0.0.4/cloudflare_r2/nb.ipynb`

 * *Files identical despite different names*

### Comparing `cloudflare_r2-0.0.3/pyproject.toml` & `cloudflare_r2-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "cloudflare-r2"
 description = "Wrapper around commonly used boto3 functions in Cloudflare R2 API."
-version = "0.0.3"
+version = "0.0.4"
 authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 readme = "README.md"
 homepage = "https://mv3.dev"
 repository = "https://github.com/justmars/cloudflare-r2"
 documentation = "https://justmars.github.io/cloudflare-r2"
 classifiers = [
   "Programming Language :: Python :: 3.11",
   "Typing :: Typed",
   "Development Status :: 4 - Beta",
   "Framework :: Pytest",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-start-cloudflare = "^0.0.2"
+start-cloudflare = "^0.0.3"
 boto3 = "^1.26"
 
 [tool.poetry.group.dev.dependencies] # latest as of June 2023
 pytest = "^7.3"
 pytest-cov = "^2.12.1"
 pre-commit = "^3.3"
 mkdocs = "^1.4.3"
```

### Comparing `cloudflare_r2-0.0.3/PKG-INFO` & `cloudflare_r2-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: cloudflare-r2
-Version: 0.0.3
+Version: 0.0.4
 Summary: Wrapper around commonly used boto3 functions in Cloudflare R2 API.
 Home-page: https://mv3.dev
 Author: Marcelino G. Veloso III
 Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Dist: boto3 (>=1.26,<2.0)
-Requires-Dist: start-cloudflare (>=0.0.2,<0.0.3)
+Requires-Dist: start-cloudflare (>=0.0.3,<0.0.4)
 Project-URL: Documentation, https://justmars.github.io/cloudflare-r2
 Project-URL: Repository, https://github.com/justmars/cloudflare-r2
 Description-Content-Type: text/markdown
 
 # cloudflare-r2
 
 ![Github CI](https://github.com/justmars/cloudflare-r2/actions/workflows/main.yml/badge.svg)
```

