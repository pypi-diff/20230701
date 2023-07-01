# Comparing `tmp/start_cloudflare-0.0.2.tar.gz` & `tmp/start_cloudflare-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "start_cloudflare-0.0.2.tar", max compression
+gzip compressed data, was "start_cloudflare-0.0.3.tar", max compression
```

## Comparing `start_cloudflare-0.0.2.tar` & `start_cloudflare-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      262 2023-06-22 02:15:00.368655 start_cloudflare-0.0.2/README.md
--rw-r--r--   0        0        0     1431 2023-06-22 02:54:49.599510 start_cloudflare-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       44 2023-06-22 02:54:49.600033 start_cloudflare-0.0.2/start_cloudflare/__init__.py
--rw-r--r--   0        0        0     5846 2023-06-22 02:54:49.600527 start_cloudflare-0.0.2/start_cloudflare/main.py
--rw-r--r--   0        0        0     1102 1970-01-01 00:00:00.000000 start_cloudflare-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      262 2023-06-22 02:15:00.368655 start_cloudflare-0.0.3/README.md
+-rw-r--r--   0        0        0     1351 2023-07-01 03:23:18.156179 start_cloudflare-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-06-22 02:54:49.600033 start_cloudflare-0.0.3/start_cloudflare/__init__.py
+-rw-r--r--   0        0        0     5846 2023-06-22 02:54:49.600527 start_cloudflare-0.0.3/start_cloudflare/main.py
+-rw-r--r--   0        0        0     1098 1970-01-01 00:00:00.000000 start_cloudflare-0.0.3/PKG-INFO
```

### Comparing `start_cloudflare-0.0.2/pyproject.toml` & `start_cloudflare-0.0.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "start-cloudflare"
 description = "A Pydantic BaseSettings class intended to be extended by other Cloudflare services."
-version = "0.0.2"
+version = "0.0.3"
 authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 readme = "README.md"
 homepage = "https://mv3.dev"
 repository = "https://github.com/justmars/start-cloudflare"
 documentation = "https://justmars.github.io/start-cloudflare"
 classifiers = [
   "Programming Language :: Python :: 3.11",
@@ -13,16 +13,16 @@
   "Development Status :: 4 - Beta",
   "Framework :: Pytest",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 python-dotenv = "^1.0"
-pydantic-settings = {version = "^2.0b1", allow-prereleases = true}
-pydantic = {version = "^2.0b3", allow-prereleases = true}
+pydantic-settings = "^2.0"
+pydantic = "^2.0"
 email-validator = "^2.0.0.post2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3"
 pytest-env = "^0.8.1"
 pytest-cov = "^4.1"
 pre-commit = "^3.3"
```

### Comparing `start_cloudflare-0.0.2/start_cloudflare/main.py` & `start_cloudflare-0.0.3/start_cloudflare/main.py`

 * *Files identical despite different names*

### Comparing `start_cloudflare-0.0.2/PKG-INFO` & `start_cloudflare-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: start-cloudflare
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Pydantic BaseSettings class intended to be extended by other Cloudflare services.
 Home-page: https://mv3.dev
 Author: Marcelino G. Veloso III
 Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Dist: email-validator (>=2.0.0.post2,<3.0.0)
-Requires-Dist: pydantic (>=2.0b3,<3.0)
-Requires-Dist: pydantic-settings (>=2.0b1,<3.0)
+Requires-Dist: pydantic (>=2.0,<3.0)
+Requires-Dist: pydantic-settings (>=2.0,<3.0)
 Requires-Dist: python-dotenv (>=1.0,<2.0)
 Project-URL: Documentation, https://justmars.github.io/start-cloudflare
 Project-URL: Repository, https://github.com/justmars/start-cloudflare
 Description-Content-Type: text/markdown
 
 # start-cloudflare
```

