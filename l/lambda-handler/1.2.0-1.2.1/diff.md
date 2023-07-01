# Comparing `tmp/lambda_handler-1.2.0.tar.gz` & `tmp/lambda_handler-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambda_handler-1.2.0.tar", max compression
+gzip compressed data, was "lambda_handler-1.2.1.tar", max compression
```

## Comparing `lambda_handler-1.2.0.tar` & `lambda_handler-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2022-11-09 08:54:28.803833 lambda_handler-1.2.0/LICENSE
--rw-r--r--   0        0        0     4647 2023-07-01 19:01:26.885296 lambda_handler-1.2.0/README.md
--rw-r--r--   0        0        0      369 2023-07-01 19:29:19.061673 lambda_handler-1.2.0/lambda_handler/__init__.py
--rw-r--r--   0        0        0     2820 2022-11-09 09:08:20.229164 lambda_handler-1.2.0/lambda_handler/dependencies.py
--rw-r--r--   0        0        0    13929 2022-11-09 09:56:48.497145 lambda_handler-1.2.0/lambda_handler/handler.py
--rw-r--r--   0        0        0      560 2022-11-09 09:08:20.233470 lambda_handler-1.2.0/lambda_handler/model/__init__.py
--rw-r--r--   0        0        0     5927 2022-11-09 09:08:20.236865 lambda_handler-1.2.0/lambda_handler/model/base.py
--rw-r--r--   0        0        0     2134 2022-11-09 09:08:20.231006 lambda_handler-1.2.0/lambda_handler/model/direct_invocation.py
--rw-r--r--   0        0        0     3206 2022-11-09 09:08:20.234983 lambda_handler-1.2.0/lambda_handler/model/event_bridge.py
--rw-r--r--   0        0        0     3520 2023-07-01 19:29:01.272575 lambda_handler-1.2.0/lambda_handler/model/sns.py
--rw-r--r--   0        0        0     4394 2022-11-09 09:57:24.033450 lambda_handler-1.2.0/lambda_handler/model/sqs.py
--rw-r--r--   0        0        0        0 2022-11-09 09:59:06.433379 lambda_handler-1.2.0/lambda_handler/py.typed
--rw-r--r--   0        0        0     2624 2022-11-09 09:35:27.330005 lambda_handler-1.2.0/lambda_handler/types.py
--rw-r--r--   0        0        0     9375 2022-11-09 09:36:45.711163 lambda_handler-1.2.0/lambda_handler/utils.py
--rw-r--r--   0        0        0     1700 2023-07-01 19:29:19.061904 lambda_handler-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5438 1970-01-01 00:00:00.000000 lambda_handler-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-11-09 08:54:28.803833 lambda_handler-1.2.1/LICENSE
+-rw-r--r--   0        0        0     4647 2023-07-01 19:01:26.885296 lambda_handler-1.2.1/README.md
+-rw-r--r--   0        0        0      369 2023-07-01 19:41:25.684954 lambda_handler-1.2.1/lambda_handler/__init__.py
+-rw-r--r--   0        0        0     2820 2022-11-09 09:08:20.229164 lambda_handler-1.2.1/lambda_handler/dependencies.py
+-rw-r--r--   0        0        0    13929 2022-11-09 09:56:48.497145 lambda_handler-1.2.1/lambda_handler/handler.py
+-rw-r--r--   0        0        0      560 2022-11-09 09:08:20.233470 lambda_handler-1.2.1/lambda_handler/model/__init__.py
+-rw-r--r--   0        0        0     5927 2022-11-09 09:08:20.236865 lambda_handler-1.2.1/lambda_handler/model/base.py
+-rw-r--r--   0        0        0     2134 2022-11-09 09:08:20.231006 lambda_handler-1.2.1/lambda_handler/model/direct_invocation.py
+-rw-r--r--   0        0        0     3206 2022-11-09 09:08:20.234983 lambda_handler-1.2.1/lambda_handler/model/event_bridge.py
+-rw-r--r--   0        0        0     3511 2023-07-01 19:40:46.187213 lambda_handler-1.2.1/lambda_handler/model/sns.py
+-rw-r--r--   0        0        0     4394 2022-11-09 09:57:24.033450 lambda_handler-1.2.1/lambda_handler/model/sqs.py
+-rw-r--r--   0        0        0        0 2022-11-09 09:59:06.433379 lambda_handler-1.2.1/lambda_handler/py.typed
+-rw-r--r--   0        0        0     2624 2022-11-09 09:35:27.330005 lambda_handler-1.2.1/lambda_handler/types.py
+-rw-r--r--   0        0        0     9375 2022-11-09 09:36:45.711163 lambda_handler-1.2.1/lambda_handler/utils.py
+-rw-r--r--   0        0        0     1700 2023-07-01 19:41:25.685184 lambda_handler-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5438 1970-01-01 00:00:00.000000 lambda_handler-1.2.1/PKG-INFO
```

### Comparing `lambda_handler-1.2.0/LICENSE` & `lambda_handler-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lambda_handler-1.2.0/README.md` & `lambda_handler-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lambda_handler-1.2.0/lambda_handler/dependencies.py` & `lambda_handler-1.2.1/lambda_handler/dependencies.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-1.2.0/lambda_handler/handler.py` & `lambda_handler-1.2.1/lambda_handler/handler.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-1.2.0/lambda_handler/model/__init__.py` & `lambda_handler-1.2.1/lambda_handler/model/__init__.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-1.2.0/lambda_handler/model/base.py` & `lambda_handler-1.2.1/lambda_handler/model/base.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-1.2.0/lambda_handler/model/direct_invocation.py` & `lambda_handler-1.2.1/lambda_handler/model/direct_invocation.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-1.2.0/lambda_handler/model/event_bridge.py` & `lambda_handler-1.2.1/lambda_handler/model/event_bridge.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-1.2.0/lambda_handler/model/sns.py` & `lambda_handler-1.2.1/lambda_handler/model/sns.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         """Topic name, defined as the event subscription ARN of the first record
 
         Returns
         -------
         str
             Topic name
         """
-        return self.records[0].event_subscription_arn.split(":")[-1]
+        return self.records[0].sns.topic_arn.split(":")[-1]
 
     @property
     def event_key(self) -> str:
         """Event key, defined as the topic name
 
         Returns
         -------
```

### Comparing `lambda_handler-1.2.0/lambda_handler/model/sqs.py` & `lambda_handler-1.2.1/lambda_handler/model/sqs.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-1.2.0/lambda_handler/types.py` & `lambda_handler-1.2.1/lambda_handler/types.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-1.2.0/lambda_handler/utils.py` & `lambda_handler-1.2.1/lambda_handler/utils.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-1.2.0/pyproject.toml` & `lambda_handler-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lambda-handler"
-version = "1.2.0"
+version = "1.2.1"
 description = "A Python package for routing and validating AWS events inside a Lambda function"
 authors = ["Matthew Badger <matt@branchenergy.com>"]
 homepage = "https://github.com/branchenergy/lambda-handler"
 repository = "https://github.com/branchenergy/lambda-handler"
 license = "Apache 2.0"
 packages = [
   {include = "lambda_handler"},
@@ -47,9 +47,9 @@
     "invalid-name"                    # Calm down Pylint
 ]
 
 [tool.pytest.ini_options]
 addopts = "--cov=lambda_handler --cov-report term-missing"
 
 [build-system]
-requires = ["poetry-core>=1.2.0"]
+requires = ["poetry-core>=1.2.1"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lambda_handler-1.2.0/PKG-INFO` & `lambda_handler-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambda-handler
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python package for routing and validating AWS events inside a Lambda function
 Home-page: https://github.com/branchenergy/lambda-handler
 License: Apache 2.0
 Author: Matthew Badger
 Author-email: matt@branchenergy.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

