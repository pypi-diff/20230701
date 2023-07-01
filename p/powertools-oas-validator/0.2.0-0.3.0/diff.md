# Comparing `tmp/powertools_oas_validator-0.2.0.tar.gz` & `tmp/powertools_oas_validator-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powertools_oas_validator-0.2.0.tar", max compression
+gzip compressed data, was "powertools_oas_validator-0.3.0.tar", max compression
```

## Comparing `powertools_oas_validator-0.2.0.tar` & `powertools_oas_validator-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1077 2023-07-01 16:36:35.268406 powertools_oas_validator-0.2.0/LICENSE
--rw-r--r--   0        0        0       26 2023-07-01 16:36:35.268406 powertools_oas_validator-0.2.0/README.md
--rw-r--r--   0        0        0       13 2023-07-01 16:36:35.268406 powertools_oas_validator-0.2.0/powertools_oas_validator/__init__.py
--rw-r--r--   0        0        0      145 2023-07-01 16:36:35.268406 powertools_oas_validator-0.2.0/powertools_oas_validator/exceptions.py
--rw-r--r--   0        0        0     1580 2023-07-01 16:36:35.268406 powertools_oas_validator-0.2.0/powertools_oas_validator/middleware.py
--rw-r--r--   0        0        0       13 2023-07-01 16:36:35.268406 powertools_oas_validator-0.2.0/powertools_oas_validator/services/__init__.py
--rw-r--r--   0        0        0     3693 2023-07-01 16:36:35.268406 powertools_oas_validator-0.2.0/powertools_oas_validator/services/request_validator.py
--rw-r--r--   0        0        0     1198 2023-07-01 16:36:35.272406 powertools_oas_validator-0.2.0/powertools_oas_validator/services/spec_loader.py
--rw-r--r--   0        0        0     3635 2023-07-01 16:36:35.272406 powertools_oas_validator-0.2.0/powertools_oas_validator/services/spec_validator.py
--rw-r--r--   0        0        0      681 2023-07-01 16:36:35.272406 powertools_oas_validator-0.2.0/powertools_oas_validator/types.py
--rw-r--r--   0        0        0      804 2023-07-01 16:36:35.272406 powertools_oas_validator-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 powertools_oas_validator-0.2.0/setup.py
--rw-r--r--   0        0        0      709 1970-01-01 00:00:00.000000 powertools_oas_validator-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-01 17:16:03.073293 powertools_oas_validator-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2696 2023-07-01 17:16:03.073293 powertools_oas_validator-0.3.0/README.md
+-rw-r--r--   0        0        0       13 2023-07-01 17:16:03.073293 powertools_oas_validator-0.3.0/powertools_oas_validator/__init__.py
+-rw-r--r--   0        0        0      145 2023-07-01 17:16:03.073293 powertools_oas_validator-0.3.0/powertools_oas_validator/exceptions.py
+-rw-r--r--   0        0        0     1580 2023-07-01 17:16:03.073293 powertools_oas_validator-0.3.0/powertools_oas_validator/middleware.py
+-rw-r--r--   0        0        0       13 2023-07-01 17:16:03.073293 powertools_oas_validator-0.3.0/powertools_oas_validator/services/__init__.py
+-rw-r--r--   0        0        0     3693 2023-07-01 17:16:03.073293 powertools_oas_validator-0.3.0/powertools_oas_validator/services/request_validator.py
+-rw-r--r--   0        0        0     1198 2023-07-01 17:16:03.073293 powertools_oas_validator-0.3.0/powertools_oas_validator/services/spec_loader.py
+-rw-r--r--   0        0        0     3635 2023-07-01 17:16:03.073293 powertools_oas_validator-0.3.0/powertools_oas_validator/services/spec_validator.py
+-rw-r--r--   0        0        0      681 2023-07-01 17:16:03.073293 powertools_oas_validator-0.3.0/powertools_oas_validator/types.py
+-rw-r--r--   0        0        0      801 2023-07-01 17:16:03.073293 powertools_oas_validator-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3590 1970-01-01 00:00:00.000000 powertools_oas_validator-0.3.0/setup.py
+-rw-r--r--   0        0        0     3376 1970-01-01 00:00:00.000000 powertools_oas_validator-0.3.0/PKG-INFO
```

### Comparing `powertools_oas_validator-0.2.0/LICENSE` & `powertools_oas_validator-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.2.0/powertools_oas_validator/middleware.py` & `powertools_oas_validator-0.3.0/powertools_oas_validator/middleware.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.2.0/powertools_oas_validator/services/request_validator.py` & `powertools_oas_validator-0.3.0/powertools_oas_validator/services/request_validator.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.2.0/powertools_oas_validator/services/spec_loader.py` & `powertools_oas_validator-0.3.0/powertools_oas_validator/services/spec_loader.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.2.0/powertools_oas_validator/services/spec_validator.py` & `powertools_oas_validator-0.3.0/powertools_oas_validator/services/spec_validator.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.2.0/powertools_oas_validator/types.py` & `powertools_oas_validator-0.3.0/powertools_oas_validator/types.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.2.0/pyproject.toml` & `powertools_oas_validator-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "powertools-oas-validator"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
-authors = ["Rasmus Hansen <Rasmus.Hansen@LifeWorks.com>"]
+authors = ["Rasmus Hansen <R.FangelHansen@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [{include = "powertools_oas_validator"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aws-lambda-powertools = "^2.18.0"
```

