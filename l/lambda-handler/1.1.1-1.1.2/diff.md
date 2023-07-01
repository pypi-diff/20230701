# Comparing `tmp/lambda-handler-1.1.1.tar.gz` & `tmp/lambda_handler-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambda-handler-1.1.1.tar", max compression
+gzip compressed data, was "lambda_handler-1.1.2.tar", max compression
```

## Comparing `lambda-handler-1.1.1.tar` & `lambda_handler-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0    11357 2022-11-09 08:54:28.803833 lambda-handler-1.1.1/LICENSE
--rw-r--r--   0        0        0     4647 2023-07-01 19:01:26.885296 lambda-handler-1.1.1/README.md
--rw-r--r--   0        0        0      369 2023-07-01 19:20:07.796218 lambda-handler-1.1.1/lambda_handler/__init__.py
--rw-r--r--   0        0        0     2820 2022-11-09 09:08:20.229164 lambda-handler-1.1.1/lambda_handler/dependencies.py
--rw-r--r--   0        0        0    13929 2022-11-09 09:56:48.497145 lambda-handler-1.1.1/lambda_handler/handler.py
--rw-r--r--   0        0        0      560 2022-11-09 09:08:20.233470 lambda-handler-1.1.1/lambda_handler/model/__init__.py
--rw-r--r--   0        0        0     5927 2022-11-09 09:08:20.236865 lambda-handler-1.1.1/lambda_handler/model/base.py
--rw-r--r--   0        0        0     2134 2022-11-09 09:08:20.231006 lambda-handler-1.1.1/lambda_handler/model/direct_invocation.py
--rw-r--r--   0        0        0     3206 2022-11-09 09:08:20.234983 lambda-handler-1.1.1/lambda_handler/model/event_bridge.py
--rw-r--r--   0        0        0     3555 2023-07-01 19:00:37.250044 lambda-handler-1.1.1/lambda_handler/model/sns.py
--rw-r--r--   0        0        0     4394 2022-11-09 09:57:24.033450 lambda-handler-1.1.1/lambda_handler/model/sqs.py
--rw-r--r--   0        0        0        0 2022-11-09 09:59:06.433379 lambda-handler-1.1.1/lambda_handler/py.typed
--rw-r--r--   0        0        0     2624 2022-11-09 09:35:27.330005 lambda-handler-1.1.1/lambda_handler/types.py
--rw-r--r--   0        0        0     9375 2022-11-09 09:36:45.711163 lambda-handler-1.1.1/lambda_handler/utils.py
--rw-r--r--   0        0        0     2207 2023-07-01 19:20:07.796490 lambda-handler-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     5597 2023-07-01 19:20:15.253092 lambda-handler-1.1.1/setup.py
--rw-r--r--   0        0        0     5315 2023-07-01 19:20:15.253542 lambda-handler-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-11-09 08:54:28.803833 lambda_handler-1.1.2/LICENSE
+-rw-r--r--   0        0        0     4647 2023-07-01 19:01:26.885296 lambda_handler-1.1.2/README.md
+-rw-r--r--   0        0        0      369 2023-07-01 19:23:04.088752 lambda_handler-1.1.2/lambda_handler/__init__.py
+-rw-r--r--   0        0        0     2820 2022-11-09 09:08:20.229164 lambda_handler-1.1.2/lambda_handler/dependencies.py
+-rw-r--r--   0        0        0    13929 2022-11-09 09:56:48.497145 lambda_handler-1.1.2/lambda_handler/handler.py
+-rw-r--r--   0        0        0      560 2022-11-09 09:08:20.233470 lambda_handler-1.1.2/lambda_handler/model/__init__.py
+-rw-r--r--   0        0        0     5927 2022-11-09 09:08:20.236865 lambda_handler-1.1.2/lambda_handler/model/base.py
+-rw-r--r--   0        0        0     2134 2022-11-09 09:08:20.231006 lambda_handler-1.1.2/lambda_handler/model/direct_invocation.py
+-rw-r--r--   0        0        0     3206 2022-11-09 09:08:20.234983 lambda_handler-1.1.2/lambda_handler/model/event_bridge.py
+-rw-r--r--   0        0        0     3555 2023-07-01 19:00:37.250044 lambda_handler-1.1.2/lambda_handler/model/sns.py
+-rw-r--r--   0        0        0     4394 2022-11-09 09:57:24.033450 lambda_handler-1.1.2/lambda_handler/model/sqs.py
+-rw-r--r--   0        0        0        0 2022-11-09 09:59:06.433379 lambda_handler-1.1.2/lambda_handler/py.typed
+-rw-r--r--   0        0        0     2624 2022-11-09 09:35:27.330005 lambda_handler-1.1.2/lambda_handler/types.py
+-rw-r--r--   0        0        0     9375 2022-11-09 09:36:45.711163 lambda_handler-1.1.2/lambda_handler/utils.py
+-rw-r--r--   0        0        0     1700 2023-07-01 19:23:04.088988 lambda_handler-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5438 1970-01-01 00:00:00.000000 lambda_handler-1.1.2/PKG-INFO
```

### Comparing `lambda-handler-1.1.1/LICENSE` & `lambda_handler-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lambda-handler-1.1.1/README.md` & `lambda_handler-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `lambda-handler-1.1.1/lambda_handler/dependencies.py` & `lambda_handler-1.1.2/lambda_handler/dependencies.py`

 * *Files identical despite different names*

### Comparing `lambda-handler-1.1.1/lambda_handler/handler.py` & `lambda_handler-1.1.2/lambda_handler/handler.py`

 * *Files identical despite different names*

### Comparing `lambda-handler-1.1.1/lambda_handler/model/__init__.py` & `lambda_handler-1.1.2/lambda_handler/model/__init__.py`

 * *Files identical despite different names*

### Comparing `lambda-handler-1.1.1/lambda_handler/model/base.py` & `lambda_handler-1.1.2/lambda_handler/model/base.py`

 * *Files identical despite different names*

### Comparing `lambda-handler-1.1.1/lambda_handler/model/direct_invocation.py` & `lambda_handler-1.1.2/lambda_handler/model/direct_invocation.py`

 * *Files identical despite different names*

### Comparing `lambda-handler-1.1.1/lambda_handler/model/event_bridge.py` & `lambda_handler-1.1.2/lambda_handler/model/event_bridge.py`

 * *Files identical despite different names*

### Comparing `lambda-handler-1.1.1/lambda_handler/model/sns.py` & `lambda_handler-1.1.2/lambda_handler/model/sns.py`

 * *Files identical despite different names*

### Comparing `lambda-handler-1.1.1/lambda_handler/model/sqs.py` & `lambda_handler-1.1.2/lambda_handler/model/sqs.py`

 * *Files identical despite different names*

### Comparing `lambda-handler-1.1.1/lambda_handler/types.py` & `lambda_handler-1.1.2/lambda_handler/types.py`

 * *Files identical despite different names*

### Comparing `lambda-handler-1.1.1/lambda_handler/utils.py` & `lambda_handler-1.1.2/lambda_handler/utils.py`

 * *Files identical despite different names*

### Comparing `lambda-handler-1.1.1/pyproject.toml` & `lambda_handler-1.1.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,14 @@
-[project]
-name = "lambda-handler"
-version = "1.1.1"
-authors = [
-  { name="Matthew Badger", email="matt@branchenergy.com" },
-]
-description = "A Python package for routing and validating AWS events inside a Lambda function"
-readme = "README.md"
-requires-python = ">=3.8"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/branchenergy/lambda_handler"
-"Bug Tracker" = "https://github.com/branchenergy/lambda_handler/issues"
-
 [tool.poetry]
 name = "lambda-handler"
-version = "1.1.1"
+version = "1.1.2"
 description = "A Python package for routing and validating AWS events inside a Lambda function"
 authors = ["Matthew Badger <matt@branchenergy.com>"]
-homepage = "https://github.com/branchenergy/lambda_handler"
+homepage = "https://github.com/branchenergy/lambda-handler"
+repository = "https://github.com/branchenergy/lambda-handler"
 license = "Apache 2.0"
 packages = [
   {include = "lambda_handler"},
   {include = "lambda_handler/py.typed"},
 ]
 readme = "README.md"
 
@@ -65,9 +47,9 @@
     "invalid-name"                    # Calm down Pylint
 ]
 
 [tool.pytest.ini_options]
 addopts = "--cov=lambda_handler --cov-report term-missing"
 
 [build-system]
-requires = ["poetry-core>=1.1.1"]
+requires = ["poetry-core>=1.1.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lambda-handler-1.1.1/setup.py` & `lambda_handler-1.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,172 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: lambda-handler
+Version: 1.1.2
+Summary: A Python package for routing and validating AWS events inside a Lambda function
+Home-page: https://github.com/branchenergy/lambda-handler
+License: Apache 2.0
+Author: Matthew Badger
+Author-email: matt@branchenergy.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: fastapi
+Requires-Dist: pydantic (>=1.10.2,<2.0.0)
+Project-URL: Repository, https://github.com/branchenergy/lambda-handler
+Description-Content-Type: text/markdown
 
-packages = \
-['lambda_handler', 'lambda_handler.model']
+# Lambda Handler
 
-package_data = \
-{'': ['*']}
+This project defines a Python class, `LambdaHandler`, and associated Pydantic-derived
+event classes, for handling API Gateway events from a range of sources, in particular:
 
-modules = \
-['py']
-install_requires = \
-['pydantic>=1.10.2,<2.0.0']
-
-setup_kwargs = {
-    'name': 'lambda-handler',
-    'version': '1.1.1',
-    'description': 'A Python package for routing and validating AWS events inside a Lambda function',
-    'long_description': '# Lambda Handler\n\nThis project defines a Python class, `LambdaHandler`, and associated Pydantic-derived\nevent classes, for handling API Gateway events from a range of sources, in particular:\n\n- Direct Invocation\n- EventBridge\n- SQS queues\n- SNS topics\n\nWhen not using the optional FastAPI support (see below), the package\'s only dependency\nis pydantic.\n\n## Use\n\n```python\nfrom lambda_handler import (\n    LambdaHandler,\n    EventBridgeEvent,\n    SnsEvent,\n    LambdaResponse,\n)\n\nhandler = LambdaHandler()\n\n@handler.sns(topic_name="MyTopic")\ndef handle_mytopic(event: SnsEvent) -> LambdaResponse:\n    body = frobincate()\n    return LambdaResponse(status_code=200, body=body)\n\n@handler.event_bridge(resource_name="MyResource")\ndef handle_myresource(event: EventBridgeEvent) -> LambdaResponse:\n    body = fizzbuzz()\n    return LambdaResponse(status_code=200, body=body)\n```\n\nThe handler looks after both the event parsing (so your functions should always\naccept an event of some `*Event` type), and its response as a properly-formatted\ndictionary.\n\n## Combining with FastAPI\n\nA notable omission from the events that are handled by `LambdaHandler` directly are\nHTTP requests. These can be handled by an instance of `FastAPI`, as follows:\n\n```python\nfrom fastapi import FastAPI\nfrom lambda_handler import LambdaHandler\n\napp = FastAPI(title="My HTTP handler")\n\n@app.get("/")\ndef index():\n    return "Hello, World!"\n\nhandler = LambdaHandler(fastapi_app=app)\n```\n\nThe handler will then take care of everything on your behalf. If you\'d prefer, you\ncan set `fastapi_app` later instead, and the handler will take care of that, too.\n\n```python\nfrom fastapi import FastAPI\nfrom lambda_handler import LambdaHandler, SnsEvent, LambdaResponse\n\nhandler = LambdaHandler()\n\n@handler.sns(topic_name="MyTopic")\ndef handle_mytopic(event: SnsEvent) -> LambdaResponse:\n    body = frobincate()\n    return LambdaResponse(status_code=200, body=body)\n\n\napp = FastAPI(title="My HTTP handler")\n\n@app.get("/")\ndef index():\n    return "Hello, World!"\n\nhandler.fastapi_app = app\n```\n\nFastAPI support requires the package to be installed with optional extras:\n`pip install "lambda-handler[fastapi]"`, and is built on top of the existing\n[Mangum](https://mangum.io/) package.\n\n## Model Validation\n\nThe `*Event` models lambda-handler defines use [pydantic](pydantic-docs.helpmanual.io/)\nfor parsing and validation, and these models are _generic_. This means that you can\npass a type argument to the class when defining your function, and it will correctly\nparse the content of the event (see below) to that type. If this is confusing, it\'s\neasier to see it in action:\n\n```python\nfrom lambda_handler import LambdaHandler, SnsEvent, LambdaResponse\nfrom pydantic import BaseModel\n\nhandler = LambdaHandler()\n\nclass MyModel(BaseModel):\n    thing: str\n\n@handler.sns(topic_name=topic_name)\ndef test_func(event: SnsEvent[MyModel]) -> LambdaResponse:\n    assert isinstance(event.records[0].sns.message, MyModel)\n    return LambdaResponse(status_code="200")\n```\n\nHere, we have parametrised `SnsEvent` with `MyModel` in the signature of `test_func`,\nmeaning that the `message` attribute is parsed to a `MyModel` instance in the process.\n\n### Parametrised Event Attributes\n\nThe following attributes are those which are parsed to a Pydantic model for each event\ntype:\n\n| Event Type              | Parsed Attribute                  |\n|:------------------------|:----------------------------------|\n| `DirectInvocationEvent` | `event.direct_invocation.body`    |\n| `EventBridgeEvent`      | `event.detail`                    |\n| `SnsEvent`              | `event.records[i].sns.message`    |\n| `SqsEvent`              | `event.records[i].body`           |\n\n\n## Dealing with Raw Data\n\nIf you don\'t want to deal with parsed event objects, you can include the `raw=True`\nparameter to any of the wrapping methods of `LambdaHandler` and write a function\nthat accepts and returns a `Dict[str, Any]` instead. Note that, in this case, the\nevent object will still be parsed by the `AwsEvent` subclasses for identification,\nbut the event object will be passed as-is in dictionary format to the function.\n\n```python\nfrom fastapi import FastAPI\nfrom lambda_handler import LambdaHandler, SnsEvent, LambdaResponse\n\nfrom typing import Any, Dict\n\nhandler = LambdaHandler()\n\n@handler.sns(topic_name="MyTopic")\ndef handle_mytopic(event: SnsEvent) -> LambdaResponse:\n    body = frobincate()\n    return LambdaResponse(status_code=200, body=body)\n\n@handler.sns(topic_name="MyOtherTopic". raw=True)\ndef handle_mytopic(event: Dict[str, Any]) -> Dict[str, Any]:\n    body = frobincate()\n    return {"statusCode": "200"}\n```\n',
-    'author': 'Matthew Badger',
-    'author_email': 'matt@branchenergy.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/branchenergy/lambda_handler',
-    'packages': packages,
-    'package_data': package_data,
-    'py_modules': modules,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+- Direct Invocation
+- EventBridge
+- SQS queues
+- SNS topics
 
+When not using the optional FastAPI support (see below), the package's only dependency
+is pydantic.
+
+## Use
+
+```python
+from lambda_handler import (
+    LambdaHandler,
+    EventBridgeEvent,
+    SnsEvent,
+    LambdaResponse,
+)
+
+handler = LambdaHandler()
+
+@handler.sns(topic_name="MyTopic")
+def handle_mytopic(event: SnsEvent) -> LambdaResponse:
+    body = frobincate()
+    return LambdaResponse(status_code=200, body=body)
+
+@handler.event_bridge(resource_name="MyResource")
+def handle_myresource(event: EventBridgeEvent) -> LambdaResponse:
+    body = fizzbuzz()
+    return LambdaResponse(status_code=200, body=body)
+```
+
+The handler looks after both the event parsing (so your functions should always
+accept an event of some `*Event` type), and its response as a properly-formatted
+dictionary.
+
+## Combining with FastAPI
+
+A notable omission from the events that are handled by `LambdaHandler` directly are
+HTTP requests. These can be handled by an instance of `FastAPI`, as follows:
+
+```python
+from fastapi import FastAPI
+from lambda_handler import LambdaHandler
+
+app = FastAPI(title="My HTTP handler")
+
+@app.get("/")
+def index():
+    return "Hello, World!"
+
+handler = LambdaHandler(fastapi_app=app)
+```
+
+The handler will then take care of everything on your behalf. If you'd prefer, you
+can set `fastapi_app` later instead, and the handler will take care of that, too.
+
+```python
+from fastapi import FastAPI
+from lambda_handler import LambdaHandler, SnsEvent, LambdaResponse
+
+handler = LambdaHandler()
+
+@handler.sns(topic_name="MyTopic")
+def handle_mytopic(event: SnsEvent) -> LambdaResponse:
+    body = frobincate()
+    return LambdaResponse(status_code=200, body=body)
+
+
+app = FastAPI(title="My HTTP handler")
+
+@app.get("/")
+def index():
+    return "Hello, World!"
+
+handler.fastapi_app = app
+```
+
+FastAPI support requires the package to be installed with optional extras:
+`pip install "lambda-handler[fastapi]"`, and is built on top of the existing
+[Mangum](https://mangum.io/) package.
+
+## Model Validation
+
+The `*Event` models lambda-handler defines use [pydantic](pydantic-docs.helpmanual.io/)
+for parsing and validation, and these models are _generic_. This means that you can
+pass a type argument to the class when defining your function, and it will correctly
+parse the content of the event (see below) to that type. If this is confusing, it's
+easier to see it in action:
+
+```python
+from lambda_handler import LambdaHandler, SnsEvent, LambdaResponse
+from pydantic import BaseModel
+
+handler = LambdaHandler()
+
+class MyModel(BaseModel):
+    thing: str
+
+@handler.sns(topic_name=topic_name)
+def test_func(event: SnsEvent[MyModel]) -> LambdaResponse:
+    assert isinstance(event.records[0].sns.message, MyModel)
+    return LambdaResponse(status_code="200")
+```
+
+Here, we have parametrised `SnsEvent` with `MyModel` in the signature of `test_func`,
+meaning that the `message` attribute is parsed to a `MyModel` instance in the process.
+
+### Parametrised Event Attributes
+
+The following attributes are those which are parsed to a Pydantic model for each event
+type:
+
+| Event Type              | Parsed Attribute                  |
+|:------------------------|:----------------------------------|
+| `DirectInvocationEvent` | `event.direct_invocation.body`    |
+| `EventBridgeEvent`      | `event.detail`                    |
+| `SnsEvent`              | `event.records[i].sns.message`    |
+| `SqsEvent`              | `event.records[i].body`           |
+
+
+## Dealing with Raw Data
+
+If you don't want to deal with parsed event objects, you can include the `raw=True`
+parameter to any of the wrapping methods of `LambdaHandler` and write a function
+that accepts and returns a `Dict[str, Any]` instead. Note that, in this case, the
+event object will still be parsed by the `AwsEvent` subclasses for identification,
+but the event object will be passed as-is in dictionary format to the function.
+
+```python
+from fastapi import FastAPI
+from lambda_handler import LambdaHandler, SnsEvent, LambdaResponse
+
+from typing import Any, Dict
+
+handler = LambdaHandler()
+
+@handler.sns(topic_name="MyTopic")
+def handle_mytopic(event: SnsEvent) -> LambdaResponse:
+    body = frobincate()
+    return LambdaResponse(status_code=200, body=body)
+
+@handler.sns(topic_name="MyOtherTopic". raw=True)
+def handle_mytopic(event: Dict[str, Any]) -> Dict[str, Any]:
+    body = frobincate()
+    return {"statusCode": "200"}
+```
 
-setup(**setup_kwargs)
```

