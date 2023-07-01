# Comparing `tmp/moesifapi-1.4.0.tar.gz` & `tmp/moesifapi-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moesifapi-1.4.0.tar", last modified: Fri Aug 19 23:28:03 2022, max compression
+gzip compressed data, was "dist/moesifapi-1.4.1.tar", last modified: Sat Jul  1 00:48:09 2023, max compression
```

## Comparing `moesifapi-1.4.0.tar` & `moesifapi-1.4.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2022-08-19 23:28:03.540870 moesifapi-1.4.0/
--rwxr-xr-x   0 praveen    (501) staff       (20)    11918 2022-08-18 23:33:42.000000 moesifapi-1.4.0/LICENSE
--rw-r--r--   0 praveen    (501) staff       (20)       61 2022-08-18 23:33:42.000000 moesifapi-1.4.0/MANIFEST.in
--rw-r--r--   0 praveen    (501) staff       (20)    11105 2022-08-19 23:28:03.540980 moesifapi-1.4.0/PKG-INFO
--rwxr-xr-x   0 praveen    (501) staff       (20)    10002 2022-08-18 23:33:42.000000 moesifapi-1.4.0/README.md
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2022-08-19 23:28:03.520466 moesifapi-1.4.0/moesifapi/
--rwxr-xr-x   0 praveen    (501) staff       (20)      209 2022-08-18 23:33:42.000000 moesifapi-1.4.0/moesifapi/__init__.py
--rwxr-xr-x   0 praveen    (501) staff       (20)     5538 2022-08-18 23:33:42.000000 moesifapi-1.4.0/moesifapi/api_helper.py
--rwxr-xr-x   0 praveen    (501) staff       (20)      294 2022-08-18 23:33:42.000000 moesifapi-1.4.0/moesifapi/configuration.py
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2022-08-19 23:28:03.534999 moesifapi-1.4.0/moesifapi/controllers/
--rwxr-xr-x   0 praveen    (501) staff       (20)       94 2022-08-18 23:33:42.000000 moesifapi-1.4.0/moesifapi/controllers/__init__.py
--rwxr-xr-x   0 praveen    (501) staff       (20)    15418 2022-08-19 23:26:24.000000 moesifapi-1.4.0/moesifapi/controllers/api_controller.py
--rwxr-xr-x   0 praveen    (501) staff       (20)     1306 2022-08-18 23:33:42.000000 moesifapi-1.4.0/moesifapi/controllers/base_controller.py
--rwxr-xr-x   0 praveen    (501) staff       (20)     2342 2022-08-18 23:33:42.000000 moesifapi-1.4.0/moesifapi/controllers/health_controller.py
--rwxr-xr-x   0 praveen    (501) staff       (20)      409 2022-08-18 23:33:42.000000 moesifapi-1.4.0/moesifapi/decorators.py
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2022-08-19 23:28:03.535859 moesifapi-1.4.0/moesifapi/exceptions/
--rwxr-xr-x   0 praveen    (501) staff       (20)       29 2022-08-18 23:33:42.000000 moesifapi-1.4.0/moesifapi/exceptions/__init__.py
--rwxr-xr-x   0 praveen    (501) staff       (20)      827 2022-08-18 23:33:42.000000 moesifapi-1.4.0/moesifapi/exceptions/api_exception.py
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2022-08-19 23:28:03.537550 moesifapi-1.4.0/moesifapi/http/
--rwxr-xr-x   0 praveen    (501) staff       (20)      205 2022-08-18 23:33:42.000000 moesifapi-1.4.0/moesifapi/http/__init__.py
--rwxr-xr-x   0 praveen    (501) staff       (20)     1117 2022-08-18 23:33:42.000000 moesifapi-1.4.0/moesifapi/http/http_call_back.py
--rwxr-xr-x   0 praveen    (501) staff       (20)     7690 2022-08-18 23:33:42.000000 moesifapi-1.4.0/moesifapi/http/http_client.py
--rwxr-xr-x   0 praveen    (501) staff       (20)      962 2022-08-18 23:33:42.000000 moesifapi-1.4.0/moesifapi/http/http_context.py
--rwxr-xr-x   0 praveen    (501) staff       (20)      791 2022-08-18 23:33:42.000000 moesifapi-1.4.0/moesifapi/http/http_method_enum.py
--rwxr-xr-x   0 praveen    (501) staff       (20)     2343 2022-08-18 23:33:42.000000 moesifapi-1.4.0/moesifapi/http/http_request.py
--rwxr-xr-x   0 praveen    (501) staff       (20)     1004 2022-08-18 23:33:42.000000 moesifapi-1.4.0/moesifapi/http/http_response.py
--rwxr-xr-x   0 praveen    (501) staff       (20)     2815 2022-08-18 23:33:42.000000 moesifapi-1.4.0/moesifapi/http/requests_client.py
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2022-08-19 23:28:03.540265 moesifapi-1.4.0/moesifapi/models/
--rwxr-xr-x   0 praveen    (501) staff       (20)      211 2022-08-18 23:33:42.000000 moesifapi-1.4.0/moesifapi/models/__init__.py
--rwxr-xr-x   0 praveen    (501) staff       (20)     1836 2022-08-18 23:33:42.000000 moesifapi-1.4.0/moesifapi/models/base_model.py
--rw-r--r--   0 praveen    (501) staff       (20)     3002 2022-08-18 23:33:42.000000 moesifapi-1.4.0/moesifapi/models/campaign_model.py
--rw-r--r--   0 praveen    (501) staff       (20)     3182 2022-08-18 23:33:42.000000 moesifapi-1.4.0/moesifapi/models/company_model.py
--rwxr-xr-x   0 praveen    (501) staff       (20)     3580 2022-08-18 23:33:42.000000 moesifapi-1.4.0/moesifapi/models/event_model.py
--rwxr-xr-x   0 praveen    (501) staff       (20)     3141 2022-08-18 23:33:42.000000 moesifapi-1.4.0/moesifapi/models/event_request_model.py
--rwxr-xr-x   0 praveen    (501) staff       (20)     2638 2022-08-18 23:33:42.000000 moesifapi-1.4.0/moesifapi/models/event_response_model.py
--rwxr-xr-x   0 praveen    (501) staff       (20)     1525 2022-08-18 23:33:42.000000 moesifapi-1.4.0/moesifapi/models/status_model.py
--rw-r--r--   0 praveen    (501) staff       (20)     3470 2022-08-18 23:33:42.000000 moesifapi-1.4.0/moesifapi/models/user_model.py
--rwxr-xr-x   0 praveen    (501) staff       (20)      461 2022-08-18 23:33:42.000000 moesifapi-1.4.0/moesifapi/moesif_api_client.py
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2022-08-19 23:28:03.533930 moesifapi-1.4.0/moesifapi.egg-info/
--rw-r--r--   0 praveen    (501) staff       (20)    11105 2022-08-19 23:28:03.000000 moesifapi-1.4.0/moesifapi.egg-info/PKG-INFO
--rw-r--r--   0 praveen    (501) staff       (20)     1277 2022-08-19 23:28:03.000000 moesifapi-1.4.0/moesifapi.egg-info/SOURCES.txt
--rw-r--r--   0 praveen    (501) staff       (20)        1 2022-08-19 23:28:03.000000 moesifapi-1.4.0/moesifapi.egg-info/dependency_links.txt
--rw-r--r--   0 praveen    (501) staff       (20)       46 2022-08-19 23:28:03.000000 moesifapi-1.4.0/moesifapi.egg-info/entry_points.txt
--rw-r--r--   0 praveen    (501) staff       (20)       75 2022-08-19 23:28:03.000000 moesifapi-1.4.0/moesifapi.egg-info/requires.txt
--rw-r--r--   0 praveen    (501) staff       (20)       16 2022-08-19 23:28:03.000000 moesifapi-1.4.0/moesifapi.egg-info/top_level.txt
--rw-r--r--   0 praveen    (501) staff       (20)       67 2022-08-19 23:28:03.542250 moesifapi-1.4.0/setup.cfg
--rw-r--r--   0 praveen    (501) staff       (20)     3607 2022-08-19 23:26:24.000000 moesifapi-1.4.0/setup.py
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2022-08-19 23:28:03.517169 moesifapi-1.4.0/tests/
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2022-08-19 23:28:03.540666 moesifapi-1.4.0/tests/controllers/
--rwxr-xr-x   0 praveen    (501) staff       (20)        0 2022-08-18 23:33:42.000000 moesifapi-1.4.0/tests/controllers/__init__.py
--rwxr-xr-x   0 praveen    (501) staff       (20)      887 2022-08-18 23:33:42.000000 moesifapi-1.4.0/tests/controllers/controller_test_base.py
--rwxr-xr-x   0 praveen    (501) staff       (20)    15817 2022-08-19 23:26:24.000000 moesifapi-1.4.0/tests/controllers/test_api_controller.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-07-01 00:48:09.716854 moesifapi-1.4.1/
+-rwxr-xr-x   0 keyur      (501) staff       (20)    11918 2020-05-11 16:17:23.000000 moesifapi-1.4.1/LICENSE
+-rw-r--r--   0 keyur      (501) staff       (20)       61 2020-05-11 16:17:23.000000 moesifapi-1.4.1/MANIFEST.in
+-rw-r--r--   0 keyur      (501) staff       (20)    13766 2023-07-01 00:48:09.717284 moesifapi-1.4.1/PKG-INFO
+-rwxr-xr-x   0 keyur      (501) staff       (20)    10002 2020-05-11 16:17:23.000000 moesifapi-1.4.1/README.md
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-07-01 00:48:09.702115 moesifapi-1.4.1/moesifapi/
+-rwxr-xr-x   0 keyur      (501) staff       (20)      209 2020-05-11 16:17:23.000000 moesifapi-1.4.1/moesifapi/__init__.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     5538 2020-05-11 16:17:23.000000 moesifapi-1.4.1/moesifapi/api_helper.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)      294 2023-07-01 00:47:27.000000 moesifapi-1.4.1/moesifapi/configuration.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-07-01 00:48:09.706175 moesifapi-1.4.1/moesifapi/controllers/
+-rwxr-xr-x   0 keyur      (501) staff       (20)       94 2020-05-11 16:17:23.000000 moesifapi-1.4.1/moesifapi/controllers/__init__.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)    15418 2023-07-01 00:47:34.000000 moesifapi-1.4.1/moesifapi/controllers/api_controller.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     1306 2021-02-17 05:27:26.000000 moesifapi-1.4.1/moesifapi/controllers/base_controller.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     2342 2021-02-17 05:27:26.000000 moesifapi-1.4.1/moesifapi/controllers/health_controller.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)      409 2020-05-11 16:17:23.000000 moesifapi-1.4.1/moesifapi/decorators.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-07-01 00:48:09.707348 moesifapi-1.4.1/moesifapi/exceptions/
+-rwxr-xr-x   0 keyur      (501) staff       (20)       29 2020-05-11 16:17:23.000000 moesifapi-1.4.1/moesifapi/exceptions/__init__.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)      827 2020-05-11 16:17:23.000000 moesifapi-1.4.1/moesifapi/exceptions/api_exception.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-07-01 00:48:09.711420 moesifapi-1.4.1/moesifapi/http/
+-rwxr-xr-x   0 keyur      (501) staff       (20)      205 2020-05-11 16:17:23.000000 moesifapi-1.4.1/moesifapi/http/__init__.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     1117 2020-05-11 16:17:23.000000 moesifapi-1.4.1/moesifapi/http/http_call_back.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     7690 2020-05-11 16:17:23.000000 moesifapi-1.4.1/moesifapi/http/http_client.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)      962 2020-05-11 16:17:23.000000 moesifapi-1.4.1/moesifapi/http/http_context.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)      791 2020-05-11 16:17:23.000000 moesifapi-1.4.1/moesifapi/http/http_method_enum.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     2343 2020-05-11 16:17:23.000000 moesifapi-1.4.1/moesifapi/http/http_request.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     1004 2020-05-11 16:17:23.000000 moesifapi-1.4.1/moesifapi/http/http_response.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     2815 2020-05-11 16:17:23.000000 moesifapi-1.4.1/moesifapi/http/requests_client.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-07-01 00:48:09.715434 moesifapi-1.4.1/moesifapi/models/
+-rwxr-xr-x   0 keyur      (501) staff       (20)      211 2020-05-11 16:17:23.000000 moesifapi-1.4.1/moesifapi/models/__init__.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     1836 2020-05-11 16:17:23.000000 moesifapi-1.4.1/moesifapi/models/base_model.py
+-rw-r--r--   0 keyur      (501) staff       (20)     3002 2020-05-11 16:17:23.000000 moesifapi-1.4.1/moesifapi/models/campaign_model.py
+-rw-r--r--   0 keyur      (501) staff       (20)     3182 2020-05-11 16:17:23.000000 moesifapi-1.4.1/moesifapi/models/company_model.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     3854 2023-07-01 00:47:34.000000 moesifapi-1.4.1/moesifapi/models/event_model.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     3141 2020-05-11 16:17:23.000000 moesifapi-1.4.1/moesifapi/models/event_request_model.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     2638 2020-05-11 16:17:23.000000 moesifapi-1.4.1/moesifapi/models/event_response_model.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     1525 2020-05-11 16:17:23.000000 moesifapi-1.4.1/moesifapi/models/status_model.py
+-rw-r--r--   0 keyur      (501) staff       (20)     3470 2020-05-11 16:17:23.000000 moesifapi-1.4.1/moesifapi/models/user_model.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)      461 2020-05-11 16:17:23.000000 moesifapi-1.4.1/moesifapi/moesif_api_client.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-07-01 00:48:09.704364 moesifapi-1.4.1/moesifapi.egg-info/
+-rw-r--r--   0 keyur      (501) staff       (20)    13766 2023-07-01 00:48:09.000000 moesifapi-1.4.1/moesifapi.egg-info/PKG-INFO
+-rw-r--r--   0 keyur      (501) staff       (20)     1277 2023-07-01 00:48:09.000000 moesifapi-1.4.1/moesifapi.egg-info/SOURCES.txt
+-rw-r--r--   0 keyur      (501) staff       (20)        1 2023-07-01 00:48:09.000000 moesifapi-1.4.1/moesifapi.egg-info/dependency_links.txt
+-rw-r--r--   0 keyur      (501) staff       (20)       46 2023-07-01 00:48:09.000000 moesifapi-1.4.1/moesifapi.egg-info/entry_points.txt
+-rw-r--r--   0 keyur      (501) staff       (20)       75 2023-07-01 00:48:09.000000 moesifapi-1.4.1/moesifapi.egg-info/requires.txt
+-rw-r--r--   0 keyur      (501) staff       (20)       16 2023-07-01 00:48:09.000000 moesifapi-1.4.1/moesifapi.egg-info/top_level.txt
+-rw-r--r--   0 keyur      (501) staff       (20)       67 2023-07-01 00:48:09.718017 moesifapi-1.4.1/setup.cfg
+-rw-r--r--   0 keyur      (501) staff       (20)     3607 2023-07-01 00:47:34.000000 moesifapi-1.4.1/setup.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-07-01 00:48:09.697929 moesifapi-1.4.1/tests/
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-07-01 00:48:09.716428 moesifapi-1.4.1/tests/controllers/
+-rwxr-xr-x   0 keyur      (501) staff       (20)        0 2020-05-11 16:17:23.000000 moesifapi-1.4.1/tests/controllers/__init__.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)      887 2023-07-01 00:47:30.000000 moesifapi-1.4.1/tests/controllers/controller_test_base.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)    15817 2023-07-01 00:47:34.000000 moesifapi-1.4.1/tests/controllers/test_api_controller.py
```

### Comparing `moesifapi-1.4.0/LICENSE` & `moesifapi-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.0/PKG-INFO` & `moesifapi-1.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: moesifapi
-Version: 1.4.0
-Summary: Moesif API Lib for Python
-Home-page: https://www.moesif.com/docs/api?python#api-libs
-Author: Moesif, Inc
-Author-email: derric@moesif.com
-License: Apache Software License
-Keywords: log analysis restful api development debug
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Internet :: Log Analysis
-Classifier: Topic :: Software Development :: Debuggers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
-License-File: LICENSE
-
 # MoesifApi Lib for Python
 
 [![Built For][ico-built-for]][link-built-for]
 [![Latest Version][ico-version]][link-package]
 [![Language Versions][ico-language]][link-language]
 [![Software License][ico-license]][link-license]
 [![Source Code][ico-source]][link-source]
@@ -357,9 +328,7 @@
   [ico-source]: https://img.shields.io/github/last-commit/moesif/moesifapi-python.svg?style=social
 
   [link-built-for]: https://www.python.org/
   [link-package]: https://pypi.python.org/pypi/moesifapi
   [link-language]: https://pypi.python.org/pypi/moesifapi
   [link-license]: https://raw.githubusercontent.com/Moesif/moesifapi-python/master/LICENSE
   [link-source]: https://github.com/Moesif/moesifapi-python
-
-
```

### Comparing `moesifapi-1.4.0/README.md` & `moesifapi-1.4.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,334 +1,362 @@
-# MoesifApi Lib for Python
-
-[![Built For][ico-built-for]][link-built-for]
-[![Latest Version][ico-version]][link-package]
-[![Language Versions][ico-language]][link-language]
-[![Software License][ico-license]][link-license]
-[![Source Code][ico-source]][link-source]
-
-[Source Code on GitHub](https://github.com/moesif/moesifapi-python)
-
-This SDK uses the Requests library and will work for Python 2.7 — 3.5.
-
-If you are using Django as your platform, we have [moesifapi-python](https://github.com/Moesif/moesifapi-python) middleware, you can use that middleware directly.
-
-__Check out Moesif's [Developer Documentation](https://www.moesif.com/docs) and [Python API Reference](https://www.moesif.com/docs/api?python) to learn more__
-
-
-## How to install:
-
-```
-pip install moesifapi
-```
-
-## How to use:
-
-The code uses Python packages named requests, jsonpickle and dateutil.
-After having resolved the dependencies, you can easily use the SDK following these steps.
-
-Your Moesif Application Id can be found in the [_Moesif Portal_](https://www.moesif.com/).
-After signing up for a Moesif account, your Moesif Application Id will be displayed during the onboarding steps. 
-
-You can always find your Moesif Application Id at any time by logging 
-into the [_Moesif Portal_](https://www.moesif.com/), click on the top right menu,
- and then clicking _Installation_.
-
-### Create Event
-
-```python
-from __future__ import print_function
-from moesifapi.moesif_api_client import *
-from moesifapi.models import *
-
-client = MoesifAPIClient(my_application_id)
-api_client = client.api
-
-# Note: we recommend sending all API Calls via MVC framework middleware.
-
-req_headers = APIHelper.json_deserialize("""  {
-  "Host": "api.acmeinc.com",
-  "Accept": "*/*",
-  "Connection": "Keep-Alive",
-  "User-Agent": "Dalvik/2.1.0 (Linux; U; Android 5.0.2; C6906 Build/14.5.A.0.242)",
-  "Content-Type": "application/json",
-  "Content-Length": "126",
-  "Accept-Encoding": "gzip"
-} """)
-
-req_body = APIHelper.json_deserialize( """{
-  "items": [
-    {
-      "type": 1,
-      "id": "fwfrf"
-    },
-    {
-      "type": 2,
-      "id": "d43d3f"
-    }
-  ]
-}""")
-
-rsp_headers = APIHelper.json_deserialize("""  {
-    "Date": "Tue, 23 Aug 2019 23:46:49 GMT",
-    "Vary": "Accept-Encoding",
-    "Pragma": "no-cache",
-    "Expires": "-1",
-    "Content-Type": "application/json; charset=utf-8"
-    "Cache-Control": "no-cache"
-  } """)
-
-rsp_body = APIHelper.json_deserialize( """{
-    "Error": "InvalidArgumentException",
-    "Message": "Missing field field_a"
-  }""")
-
-metadata = APIHelper.json_deserialize("""{
-    "field1": "foo",
-    "field2": "bar"
-  }""")
-
-
-
-event_req = EventRequestModel(time = "2019-09-09T04:45:42.914",
-    uri = "https://api.acmeinc.com/items/reviews/",
-    verb = "PATCH",
-    api_version = "1.1.0",
-    ip_address = "61.48.220.123",
-    headers = req_headers,
-    body = req_body)
-
-event_rsp = EventResponseModel(time = "2019-09-09T04:45:42.914",
-    status = 500,
-    headers = rsp_headers,
-    body = rsp_body)
-
-event_model = EventModel(request = event_req,
-    response = event_rsp,
-    user_id = "12345",
-    company_id = "67890",
-    session_token = "23jdf0owekfmcn4u3qypxg09w4d8ayrcdx8nu2ng]s98y18cx98q3yhwmnhcfx43f",
-    metadata = metadata)
-
-
-# Perform the API call through the SDK function
-api_client.create_event(event_model)
-
-
-api_client.create_event(my_api_event_model)
-```
-
-## Update a Single User
-
-Create or update a user profile in Moesif.
-The metadata field can be any customer demographic or other info you want to store.
-Only the `userId` field is required.
-For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-a-user).
-
-```python
-from moesifapi.moesif_api_client import *
-from moesifapi.models import *
-
-api_client = MoesifAPIClient("YOUR_COLLECTOR_APPLICATION_ID").api
-
-# Only user_id is required.
-# Campaign object is optional, but useful if you want to track ROI of acquisition channels
-# See https://www.moesif.com/docs/api#users for campaign schema
-# metadata can be any custom object
-user = {
-  'user_id': '12345',
-  'company_id': '67890', # If set, associate user with a company object
-  'campaign': {
-    'utm_source': 'google',
-    'utm_medium': 'cpc', 
-    'utm_campaign': 'adwords',
-    'utm_term': 'api+tooling',
-    'utm_content': 'landing'
-  },
-  'metadata': {
-    'email': 'john@acmeinc.com',
-    'first_name': 'John',
-    'last_name': 'Doe',
-    'title': 'Software Engineer',
-    'sales_info': {
-        'stage': 'Customer',
-        'lifetime_value': 24000,
-        'account_owner': 'mary@contoso.com'
-    },
-  }
-}
-
-update_user = api_client.update_user(user)
-```
-
-## Update Users in Batch
-
-Similar to UpdateUser, but used to update a list of users in one batch. 
-Only the `userId` field is required.
-For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-users-in-batch).
-
-```python
-from moesifapi.moesif_api_client import *
-from moesifapi.models import *
-
-api_client = MoesifAPIClient("YOUR_COLLECTOR_APPLICATION_ID").api
-
-userA = {
-  'user_id': '12345',
-  'company_id': '67890', # If set, associate user with a company object
-  'metadata': {
-    'email': 'john@acmeinc.com',
-    'first_name': 'John',
-    'last_name': 'Doe',
-    'title': 'Software Engineer',
-    'sales_info': {
-        'stage': 'Customer',
-        'lifetime_value': 24000,
-        'account_owner': 'mary@contoso.com'
-    },
-  }
-}
-
-userB = {
-  'user_id': '54321',
-  'company_id': '67890', # If set, associate user with a company object
-  'metadata': {
-    'email': 'mary@acmeinc.com',
-    'first_name': 'Mary',
-    'last_name': 'Jane',
-    'title': 'Software Engineer',
-    'sales_info': {
-        'stage': 'Customer',
-        'lifetime_value': 48000,
-        'account_owner': 'mary@contoso.com'
-    },
-  }
-}
-update_users = api_client.update_users_batch([userA, userB])
-```
-
-## Update a Single Company
-
-Create or update a company profile in Moesif.
-The metadata field can be any company demographic or other info you want to store.
-Only the `companyId` field is required.
-For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-a-company).
-
-```python
-from moesifapi.moesif_api_client import *
-from moesifapi.models import *
-
-api_client = MoesifAPIClient("YOUR_COLLECTOR_APPLICATION_ID").api
-
-# Only company_id is required.
-# Campaign object is optional, but useful if you want to track ROI of acquisition channels
-# See https://www.moesif.com/docs/api#update-a-company for campaign schema
-# metadata can be any custom object
-company = {
-  'company_id': '12345',
-  'company_domain': 'acmeinc.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
-  'campaign': {
-    'utm_source': 'google',
-    'utm_medium': 'cpc', 
-    'utm_campaign': 'adwords',
-    'utm_term': 'api+tooling',
-    'utm_content': 'landing'
-  },
-  'metadata': {
-    'org_name': 'Acme, Inc',
-    'plan_name': 'Free',
-    'deal_stage': 'Lead',
-    'mrr': 24000,
-    'demographics': {
-        'alexa_ranking': 500000,
-        'employee_count': 47
-    },
-  }
-}
-
-update_company = api_client.update_company(company)
-```
-
-## Update Companies in Batch
-
-Similar to updateCompany, but used to update a list of companies in one batch. 
-Only the `companyId` field is required.
-For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-companies-in-batch).
-
-
-```python
-from moesifapi.moesif_api_client import *
-from moesifapi.models import *
-
-api_client = MoesifAPIClient("YOUR_COLLECTOR_APPLICATION_ID").api
-
-# Only company_id is required.
-# Campaign object is optional, but useful if you want to track ROI of acquisition channels
-# See https://www.moesif.com/docs/api#update-a-company for campaign schema
-# metadata can be any custom object
-companies = [{
-  'company_id': '67890',
-  'company_domain': 'acmeinc.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
-  'campaign': {
-    'utm_source': 'google',
-    'utm_medium': 'cpc', 
-    'utm_campaign': 'adwords',
-    'utm_term': 'api+tooling',
-    'utm_content': 'landing'
-  },
-  'metadata': {
-    'org_name': 'Acme, Inc',
-    'plan_name': 'Free',
-    'deal_stage': 'Lead',
-    'mrr': 24000,
-    'demographics': {
-        'alexa_ranking': 500000,
-        'employee_count': 47
-    },
-  }
-},
-{
-  'company_id': '09876',
-  'company_domain': 'contoso.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
-  'campaign': {
-    'utm_source': 'facebook',
-    'utm_medium': 'cpc', 
-    'utm_campaign': 'retargeting'
-  },
-  'metadata': {
-    'org_name': 'Contoso, Inc',
-    'plan_name': 'Paid',
-    'deal_stage': 'Lead',
-    'mrr': 48000,
-    'demographics': {
-        'alexa_ranking': 500000,
-        'employee_count': 53
-    },
-  }
-}]
-
-update_company = api_client.update_companies(companies)
-```
-
-## How to test:
-
-You can test the SDK with automatically generated test
-cases. unittest is used as the testing framework and nose is used as the test
-runner. You can run the tests as follows:
-
-  1. Manually clone the git repo
-  2. From terminal/cmd navigate to the root directory of the SDK.
-  3. Invoke 'pip install -r requirements.txt'
-  4. Add your own application id to 'test/controllers/controller_test_base'
-  5. Invoke 'nosetests tests/controllers/test_api_controller.py'
-
-  [ico-built-for]: https://img.shields.io/badge/built%20for-python-blue.svg
-  [ico-version]: https://img.shields.io/pypi/v/moesifapi.svg
-  [ico-language]: https://img.shields.io/pypi/pyversions/moesifapi.svg
-  [ico-license]: https://img.shields.io/badge/License-Apache%202.0-green.svg
-  [ico-source]: https://img.shields.io/github/last-commit/moesif/moesifapi-python.svg?style=social
-
-  [link-built-for]: https://www.python.org/
-  [link-package]: https://pypi.python.org/pypi/moesifapi
-  [link-language]: https://pypi.python.org/pypi/moesifapi
-  [link-license]: https://raw.githubusercontent.com/Moesif/moesifapi-python/master/LICENSE
-  [link-source]: https://github.com/Moesif/moesifapi-python
+Metadata-Version: 2.1
+Name: moesifapi
+Version: 1.4.1
+Summary: Moesif API Lib for Python
+Home-page: https://www.moesif.com/docs/api?python#api-libs
+Author: Moesif, Inc
+Author-email: derric@moesif.com
+License: Apache Software License
+Description: # MoesifApi Lib for Python
+        
+        [![Built For][ico-built-for]][link-built-for]
+        [![Latest Version][ico-version]][link-package]
+        [![Language Versions][ico-language]][link-language]
+        [![Software License][ico-license]][link-license]
+        [![Source Code][ico-source]][link-source]
+        
+        [Source Code on GitHub](https://github.com/moesif/moesifapi-python)
+        
+        This SDK uses the Requests library and will work for Python 2.7 — 3.5.
+        
+        If you are using Django as your platform, we have [moesifapi-python](https://github.com/Moesif/moesifapi-python) middleware, you can use that middleware directly.
+        
+        __Check out Moesif's [Developer Documentation](https://www.moesif.com/docs) and [Python API Reference](https://www.moesif.com/docs/api?python) to learn more__
+        
+        
+        ## How to install:
+        
+        ```
+        pip install moesifapi
+        ```
+        
+        ## How to use:
+        
+        The code uses Python packages named requests, jsonpickle and dateutil.
+        After having resolved the dependencies, you can easily use the SDK following these steps.
+        
+        Your Moesif Application Id can be found in the [_Moesif Portal_](https://www.moesif.com/).
+        After signing up for a Moesif account, your Moesif Application Id will be displayed during the onboarding steps. 
+        
+        You can always find your Moesif Application Id at any time by logging 
+        into the [_Moesif Portal_](https://www.moesif.com/), click on the top right menu,
+         and then clicking _Installation_.
+        
+        ### Create Event
+        
+        ```python
+        from __future__ import print_function
+        from moesifapi.moesif_api_client import *
+        from moesifapi.models import *
+        
+        client = MoesifAPIClient(my_application_id)
+        api_client = client.api
+        
+        # Note: we recommend sending all API Calls via MVC framework middleware.
+        
+        req_headers = APIHelper.json_deserialize("""  {
+          "Host": "api.acmeinc.com",
+          "Accept": "*/*",
+          "Connection": "Keep-Alive",
+          "User-Agent": "Dalvik/2.1.0 (Linux; U; Android 5.0.2; C6906 Build/14.5.A.0.242)",
+          "Content-Type": "application/json",
+          "Content-Length": "126",
+          "Accept-Encoding": "gzip"
+        } """)
+        
+        req_body = APIHelper.json_deserialize( """{
+          "items": [
+            {
+              "type": 1,
+              "id": "fwfrf"
+            },
+            {
+              "type": 2,
+              "id": "d43d3f"
+            }
+          ]
+        }""")
+        
+        rsp_headers = APIHelper.json_deserialize("""  {
+            "Date": "Tue, 23 Aug 2019 23:46:49 GMT",
+            "Vary": "Accept-Encoding",
+            "Pragma": "no-cache",
+            "Expires": "-1",
+            "Content-Type": "application/json; charset=utf-8"
+            "Cache-Control": "no-cache"
+          } """)
+        
+        rsp_body = APIHelper.json_deserialize( """{
+            "Error": "InvalidArgumentException",
+            "Message": "Missing field field_a"
+          }""")
+        
+        metadata = APIHelper.json_deserialize("""{
+            "field1": "foo",
+            "field2": "bar"
+          }""")
+        
+        
+        
+        event_req = EventRequestModel(time = "2019-09-09T04:45:42.914",
+            uri = "https://api.acmeinc.com/items/reviews/",
+            verb = "PATCH",
+            api_version = "1.1.0",
+            ip_address = "61.48.220.123",
+            headers = req_headers,
+            body = req_body)
+        
+        event_rsp = EventResponseModel(time = "2019-09-09T04:45:42.914",
+            status = 500,
+            headers = rsp_headers,
+            body = rsp_body)
+        
+        event_model = EventModel(request = event_req,
+            response = event_rsp,
+            user_id = "12345",
+            company_id = "67890",
+            session_token = "23jdf0owekfmcn4u3qypxg09w4d8ayrcdx8nu2ng]s98y18cx98q3yhwmnhcfx43f",
+            metadata = metadata)
+        
+        
+        # Perform the API call through the SDK function
+        api_client.create_event(event_model)
+        
+        
+        api_client.create_event(my_api_event_model)
+        ```
+        
+        ## Update a Single User
+        
+        Create or update a user profile in Moesif.
+        The metadata field can be any customer demographic or other info you want to store.
+        Only the `userId` field is required.
+        For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-a-user).
+        
+        ```python
+        from moesifapi.moesif_api_client import *
+        from moesifapi.models import *
+        
+        api_client = MoesifAPIClient("YOUR_COLLECTOR_APPLICATION_ID").api
+        
+        # Only user_id is required.
+        # Campaign object is optional, but useful if you want to track ROI of acquisition channels
+        # See https://www.moesif.com/docs/api#users for campaign schema
+        # metadata can be any custom object
+        user = {
+          'user_id': '12345',
+          'company_id': '67890', # If set, associate user with a company object
+          'campaign': {
+            'utm_source': 'google',
+            'utm_medium': 'cpc', 
+            'utm_campaign': 'adwords',
+            'utm_term': 'api+tooling',
+            'utm_content': 'landing'
+          },
+          'metadata': {
+            'email': 'john@acmeinc.com',
+            'first_name': 'John',
+            'last_name': 'Doe',
+            'title': 'Software Engineer',
+            'sales_info': {
+                'stage': 'Customer',
+                'lifetime_value': 24000,
+                'account_owner': 'mary@contoso.com'
+            },
+          }
+        }
+        
+        update_user = api_client.update_user(user)
+        ```
+        
+        ## Update Users in Batch
+        
+        Similar to UpdateUser, but used to update a list of users in one batch. 
+        Only the `userId` field is required.
+        For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-users-in-batch).
+        
+        ```python
+        from moesifapi.moesif_api_client import *
+        from moesifapi.models import *
+        
+        api_client = MoesifAPIClient("YOUR_COLLECTOR_APPLICATION_ID").api
+        
+        userA = {
+          'user_id': '12345',
+          'company_id': '67890', # If set, associate user with a company object
+          'metadata': {
+            'email': 'john@acmeinc.com',
+            'first_name': 'John',
+            'last_name': 'Doe',
+            'title': 'Software Engineer',
+            'sales_info': {
+                'stage': 'Customer',
+                'lifetime_value': 24000,
+                'account_owner': 'mary@contoso.com'
+            },
+          }
+        }
+        
+        userB = {
+          'user_id': '54321',
+          'company_id': '67890', # If set, associate user with a company object
+          'metadata': {
+            'email': 'mary@acmeinc.com',
+            'first_name': 'Mary',
+            'last_name': 'Jane',
+            'title': 'Software Engineer',
+            'sales_info': {
+                'stage': 'Customer',
+                'lifetime_value': 48000,
+                'account_owner': 'mary@contoso.com'
+            },
+          }
+        }
+        update_users = api_client.update_users_batch([userA, userB])
+        ```
+        
+        ## Update a Single Company
+        
+        Create or update a company profile in Moesif.
+        The metadata field can be any company demographic or other info you want to store.
+        Only the `companyId` field is required.
+        For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-a-company).
+        
+        ```python
+        from moesifapi.moesif_api_client import *
+        from moesifapi.models import *
+        
+        api_client = MoesifAPIClient("YOUR_COLLECTOR_APPLICATION_ID").api
+        
+        # Only company_id is required.
+        # Campaign object is optional, but useful if you want to track ROI of acquisition channels
+        # See https://www.moesif.com/docs/api#update-a-company for campaign schema
+        # metadata can be any custom object
+        company = {
+          'company_id': '12345',
+          'company_domain': 'acmeinc.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
+          'campaign': {
+            'utm_source': 'google',
+            'utm_medium': 'cpc', 
+            'utm_campaign': 'adwords',
+            'utm_term': 'api+tooling',
+            'utm_content': 'landing'
+          },
+          'metadata': {
+            'org_name': 'Acme, Inc',
+            'plan_name': 'Free',
+            'deal_stage': 'Lead',
+            'mrr': 24000,
+            'demographics': {
+                'alexa_ranking': 500000,
+                'employee_count': 47
+            },
+          }
+        }
+        
+        update_company = api_client.update_company(company)
+        ```
+        
+        ## Update Companies in Batch
+        
+        Similar to updateCompany, but used to update a list of companies in one batch. 
+        Only the `companyId` field is required.
+        For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-companies-in-batch).
+        
+        
+        ```python
+        from moesifapi.moesif_api_client import *
+        from moesifapi.models import *
+        
+        api_client = MoesifAPIClient("YOUR_COLLECTOR_APPLICATION_ID").api
+        
+        # Only company_id is required.
+        # Campaign object is optional, but useful if you want to track ROI of acquisition channels
+        # See https://www.moesif.com/docs/api#update-a-company for campaign schema
+        # metadata can be any custom object
+        companies = [{
+          'company_id': '67890',
+          'company_domain': 'acmeinc.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
+          'campaign': {
+            'utm_source': 'google',
+            'utm_medium': 'cpc', 
+            'utm_campaign': 'adwords',
+            'utm_term': 'api+tooling',
+            'utm_content': 'landing'
+          },
+          'metadata': {
+            'org_name': 'Acme, Inc',
+            'plan_name': 'Free',
+            'deal_stage': 'Lead',
+            'mrr': 24000,
+            'demographics': {
+                'alexa_ranking': 500000,
+                'employee_count': 47
+            },
+          }
+        },
+        {
+          'company_id': '09876',
+          'company_domain': 'contoso.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
+          'campaign': {
+            'utm_source': 'facebook',
+            'utm_medium': 'cpc', 
+            'utm_campaign': 'retargeting'
+          },
+          'metadata': {
+            'org_name': 'Contoso, Inc',
+            'plan_name': 'Paid',
+            'deal_stage': 'Lead',
+            'mrr': 48000,
+            'demographics': {
+                'alexa_ranking': 500000,
+                'employee_count': 53
+            },
+          }
+        }]
+        
+        update_company = api_client.update_companies(companies)
+        ```
+        
+        ## How to test:
+        
+        You can test the SDK with automatically generated test
+        cases. unittest is used as the testing framework and nose is used as the test
+        runner. You can run the tests as follows:
+        
+          1. Manually clone the git repo
+          2. From terminal/cmd navigate to the root directory of the SDK.
+          3. Invoke 'pip install -r requirements.txt'
+          4. Add your own application id to 'test/controllers/controller_test_base'
+          5. Invoke 'nosetests tests/controllers/test_api_controller.py'
+        
+          [ico-built-for]: https://img.shields.io/badge/built%20for-python-blue.svg
+          [ico-version]: https://img.shields.io/pypi/v/moesifapi.svg
+          [ico-language]: https://img.shields.io/pypi/pyversions/moesifapi.svg
+          [ico-license]: https://img.shields.io/badge/License-Apache%202.0-green.svg
+          [ico-source]: https://img.shields.io/github/last-commit/moesif/moesifapi-python.svg?style=social
+        
+          [link-built-for]: https://www.python.org/
+          [link-package]: https://pypi.python.org/pypi/moesifapi
+          [link-language]: https://pypi.python.org/pypi/moesifapi
+          [link-license]: https://raw.githubusercontent.com/Moesif/moesifapi-python/master/LICENSE
+          [link-source]: https://github.com/Moesif/moesifapi-python
+        
+Keywords: log analysis restful api development debug
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Internet :: Log Analysis
+Classifier: Topic :: Software Development :: Debuggers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.6
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: test
```

### Comparing `moesifapi-1.4.0/moesifapi/api_helper.py` & `moesifapi-1.4.1/moesifapi/api_helper.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.0/moesifapi/controllers/api_controller.py` & `moesifapi-1.4.1/moesifapi/controllers/api_controller.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.0/moesifapi/controllers/base_controller.py` & `moesifapi-1.4.1/moesifapi/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.0/moesifapi/controllers/health_controller.py` & `moesifapi-1.4.1/moesifapi/controllers/health_controller.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.0/moesifapi/exceptions/api_exception.py` & `moesifapi-1.4.1/moesifapi/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.0/moesifapi/http/http_call_back.py` & `moesifapi-1.4.1/moesifapi/http/http_call_back.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.0/moesifapi/http/http_client.py` & `moesifapi-1.4.1/moesifapi/http/http_client.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.0/moesifapi/http/http_context.py` & `moesifapi-1.4.1/moesifapi/http/http_context.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.0/moesifapi/http/http_method_enum.py` & `moesifapi-1.4.1/moesifapi/http/http_method_enum.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.0/moesifapi/http/http_request.py` & `moesifapi-1.4.1/moesifapi/http/http_request.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.0/moesifapi/http/http_response.py` & `moesifapi-1.4.1/moesifapi/http/http_response.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.0/moesifapi/http/requests_client.py` & `moesifapi-1.4.1/moesifapi/http/requests_client.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.0/moesifapi/models/base_model.py` & `moesifapi-1.4.1/moesifapi/models/base_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.0/moesifapi/models/campaign_model.py` & `moesifapi-1.4.1/moesifapi/models/campaign_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.0/moesifapi/models/company_model.py` & `moesifapi-1.4.1/moesifapi/models/company_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.0/moesifapi/models/event_model.py` & `moesifapi-1.4.1/moesifapi/models/event_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,51 +21,54 @@
         session_token (string): End user's auth/session token
         tags (string): comma separated list of tags, see documentation
         user_id (string): End user's user_id string from your app
         company_id (string): End user's company_id string from your app
         metadata (object): Any custom data for the event.
         direction (string): API direction, incoming or outgoing
         weight (int): Weight of an API call
-
+        blocked_by (string): Any governance rule that applied to the event
     """
 
     def __init__(self,
                  request = None,
                  response = None,
                  session_token = None,
                  tags = None,
                  user_id = None,
                  company_id=None,
                  metadata = None,
                  direction=None,
-                 weight=None):
+                 weight=None,
+                 blocked_by=None):
         """Constructor for the EventModel class"""
 
         # Initialize members of the class
         self.request = request
         self.response = response
         self.session_token = session_token
         self.tags = tags
         self.user_id = user_id
         self.company_id = company_id
         self.metadata = metadata
         self.direction = direction
         self.weight = weight
+        self.blocked_by = blocked_by
 
         # Create a mapping from Model property names to API property names
         self.names = {
             "request" : "request",
             "response" : "response",
             "session_token" : "session_token",
             "tags" : "tags",
             "user_id" : "user_id",
             "company_id" : "company_id",
             "metadata" : "metadata",
             "direction": "direction",
-            "weight": "weight"
+            "weight": "weight",
+            "blocked_by": "blocked_by"
         }
 
 
     @classmethod
     def from_dictionary(cls,
                         dictionary):
         """Creates an instance of this model from a dictionary
@@ -88,17 +91,19 @@
             session_token = dictionary.get("session_token")
             tags = dictionary.get("tags")
             user_id = dictionary.get("user_id")
             company_id = dictionary.get("company_id")
             metadata = dictionary.get("metadata")
             direction = dictionary.get("direction")
             weight = dictionary.get("weight")
+            blocked_by = dictionary.get("blocked_by")
             # Return an object of this model
             return cls(request,
                        response,
                        session_token,
                        tags,
                        user_id,
                        company_id,
                        metadata,
                        direction,
-                       weight)
+                       weight,
+                       blocked_by)
```

### Comparing `moesifapi-1.4.0/moesifapi/models/event_request_model.py` & `moesifapi-1.4.1/moesifapi/models/event_request_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.0/moesifapi/models/event_response_model.py` & `moesifapi-1.4.1/moesifapi/models/event_response_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.0/moesifapi/models/status_model.py` & `moesifapi-1.4.1/moesifapi/models/status_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.0/moesifapi/models/user_model.py` & `moesifapi-1.4.1/moesifapi/models/user_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.0/moesifapi.egg-info/PKG-INFO` & `moesifapi-1.4.1/moesifapi.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,350 @@
 Metadata-Version: 2.1
 Name: moesifapi
-Version: 1.4.0
+Version: 1.4.1
 Summary: Moesif API Lib for Python
 Home-page: https://www.moesif.com/docs/api?python#api-libs
 Author: Moesif, Inc
 Author-email: derric@moesif.com
 License: Apache Software License
+Description: # MoesifApi Lib for Python
+        
+        [![Built For][ico-built-for]][link-built-for]
+        [![Latest Version][ico-version]][link-package]
+        [![Language Versions][ico-language]][link-language]
+        [![Software License][ico-license]][link-license]
+        [![Source Code][ico-source]][link-source]
+        
+        [Source Code on GitHub](https://github.com/moesif/moesifapi-python)
+        
+        This SDK uses the Requests library and will work for Python 2.7 — 3.5.
+        
+        If you are using Django as your platform, we have [moesifapi-python](https://github.com/Moesif/moesifapi-python) middleware, you can use that middleware directly.
+        
+        __Check out Moesif's [Developer Documentation](https://www.moesif.com/docs) and [Python API Reference](https://www.moesif.com/docs/api?python) to learn more__
+        
+        
+        ## How to install:
+        
+        ```
+        pip install moesifapi
+        ```
+        
+        ## How to use:
+        
+        The code uses Python packages named requests, jsonpickle and dateutil.
+        After having resolved the dependencies, you can easily use the SDK following these steps.
+        
+        Your Moesif Application Id can be found in the [_Moesif Portal_](https://www.moesif.com/).
+        After signing up for a Moesif account, your Moesif Application Id will be displayed during the onboarding steps. 
+        
+        You can always find your Moesif Application Id at any time by logging 
+        into the [_Moesif Portal_](https://www.moesif.com/), click on the top right menu,
+         and then clicking _Installation_.
+        
+        ### Create Event
+        
+        ```python
+        from __future__ import print_function
+        from moesifapi.moesif_api_client import *
+        from moesifapi.models import *
+        
+        client = MoesifAPIClient(my_application_id)
+        api_client = client.api
+        
+        # Note: we recommend sending all API Calls via MVC framework middleware.
+        
+        req_headers = APIHelper.json_deserialize("""  {
+          "Host": "api.acmeinc.com",
+          "Accept": "*/*",
+          "Connection": "Keep-Alive",
+          "User-Agent": "Dalvik/2.1.0 (Linux; U; Android 5.0.2; C6906 Build/14.5.A.0.242)",
+          "Content-Type": "application/json",
+          "Content-Length": "126",
+          "Accept-Encoding": "gzip"
+        } """)
+        
+        req_body = APIHelper.json_deserialize( """{
+          "items": [
+            {
+              "type": 1,
+              "id": "fwfrf"
+            },
+            {
+              "type": 2,
+              "id": "d43d3f"
+            }
+          ]
+        }""")
+        
+        rsp_headers = APIHelper.json_deserialize("""  {
+            "Date": "Tue, 23 Aug 2019 23:46:49 GMT",
+            "Vary": "Accept-Encoding",
+            "Pragma": "no-cache",
+            "Expires": "-1",
+            "Content-Type": "application/json; charset=utf-8"
+            "Cache-Control": "no-cache"
+          } """)
+        
+        rsp_body = APIHelper.json_deserialize( """{
+            "Error": "InvalidArgumentException",
+            "Message": "Missing field field_a"
+          }""")
+        
+        metadata = APIHelper.json_deserialize("""{
+            "field1": "foo",
+            "field2": "bar"
+          }""")
+        
+        
+        
+        event_req = EventRequestModel(time = "2019-09-09T04:45:42.914",
+            uri = "https://api.acmeinc.com/items/reviews/",
+            verb = "PATCH",
+            api_version = "1.1.0",
+            ip_address = "61.48.220.123",
+            headers = req_headers,
+            body = req_body)
+        
+        event_rsp = EventResponseModel(time = "2019-09-09T04:45:42.914",
+            status = 500,
+            headers = rsp_headers,
+            body = rsp_body)
+        
+        event_model = EventModel(request = event_req,
+            response = event_rsp,
+            user_id = "12345",
+            company_id = "67890",
+            session_token = "23jdf0owekfmcn4u3qypxg09w4d8ayrcdx8nu2ng]s98y18cx98q3yhwmnhcfx43f",
+            metadata = metadata)
+        
+        
+        # Perform the API call through the SDK function
+        api_client.create_event(event_model)
+        
+        
+        api_client.create_event(my_api_event_model)
+        ```
+        
+        ## Update a Single User
+        
+        Create or update a user profile in Moesif.
+        The metadata field can be any customer demographic or other info you want to store.
+        Only the `userId` field is required.
+        For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-a-user).
+        
+        ```python
+        from moesifapi.moesif_api_client import *
+        from moesifapi.models import *
+        
+        api_client = MoesifAPIClient("YOUR_COLLECTOR_APPLICATION_ID").api
+        
+        # Only user_id is required.
+        # Campaign object is optional, but useful if you want to track ROI of acquisition channels
+        # See https://www.moesif.com/docs/api#users for campaign schema
+        # metadata can be any custom object
+        user = {
+          'user_id': '12345',
+          'company_id': '67890', # If set, associate user with a company object
+          'campaign': {
+            'utm_source': 'google',
+            'utm_medium': 'cpc', 
+            'utm_campaign': 'adwords',
+            'utm_term': 'api+tooling',
+            'utm_content': 'landing'
+          },
+          'metadata': {
+            'email': 'john@acmeinc.com',
+            'first_name': 'John',
+            'last_name': 'Doe',
+            'title': 'Software Engineer',
+            'sales_info': {
+                'stage': 'Customer',
+                'lifetime_value': 24000,
+                'account_owner': 'mary@contoso.com'
+            },
+          }
+        }
+        
+        update_user = api_client.update_user(user)
+        ```
+        
+        ## Update Users in Batch
+        
+        Similar to UpdateUser, but used to update a list of users in one batch. 
+        Only the `userId` field is required.
+        For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-users-in-batch).
+        
+        ```python
+        from moesifapi.moesif_api_client import *
+        from moesifapi.models import *
+        
+        api_client = MoesifAPIClient("YOUR_COLLECTOR_APPLICATION_ID").api
+        
+        userA = {
+          'user_id': '12345',
+          'company_id': '67890', # If set, associate user with a company object
+          'metadata': {
+            'email': 'john@acmeinc.com',
+            'first_name': 'John',
+            'last_name': 'Doe',
+            'title': 'Software Engineer',
+            'sales_info': {
+                'stage': 'Customer',
+                'lifetime_value': 24000,
+                'account_owner': 'mary@contoso.com'
+            },
+          }
+        }
+        
+        userB = {
+          'user_id': '54321',
+          'company_id': '67890', # If set, associate user with a company object
+          'metadata': {
+            'email': 'mary@acmeinc.com',
+            'first_name': 'Mary',
+            'last_name': 'Jane',
+            'title': 'Software Engineer',
+            'sales_info': {
+                'stage': 'Customer',
+                'lifetime_value': 48000,
+                'account_owner': 'mary@contoso.com'
+            },
+          }
+        }
+        update_users = api_client.update_users_batch([userA, userB])
+        ```
+        
+        ## Update a Single Company
+        
+        Create or update a company profile in Moesif.
+        The metadata field can be any company demographic or other info you want to store.
+        Only the `companyId` field is required.
+        For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-a-company).
+        
+        ```python
+        from moesifapi.moesif_api_client import *
+        from moesifapi.models import *
+        
+        api_client = MoesifAPIClient("YOUR_COLLECTOR_APPLICATION_ID").api
+        
+        # Only company_id is required.
+        # Campaign object is optional, but useful if you want to track ROI of acquisition channels
+        # See https://www.moesif.com/docs/api#update-a-company for campaign schema
+        # metadata can be any custom object
+        company = {
+          'company_id': '12345',
+          'company_domain': 'acmeinc.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
+          'campaign': {
+            'utm_source': 'google',
+            'utm_medium': 'cpc', 
+            'utm_campaign': 'adwords',
+            'utm_term': 'api+tooling',
+            'utm_content': 'landing'
+          },
+          'metadata': {
+            'org_name': 'Acme, Inc',
+            'plan_name': 'Free',
+            'deal_stage': 'Lead',
+            'mrr': 24000,
+            'demographics': {
+                'alexa_ranking': 500000,
+                'employee_count': 47
+            },
+          }
+        }
+        
+        update_company = api_client.update_company(company)
+        ```
+        
+        ## Update Companies in Batch
+        
+        Similar to updateCompany, but used to update a list of companies in one batch. 
+        Only the `companyId` field is required.
+        For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-companies-in-batch).
+        
+        
+        ```python
+        from moesifapi.moesif_api_client import *
+        from moesifapi.models import *
+        
+        api_client = MoesifAPIClient("YOUR_COLLECTOR_APPLICATION_ID").api
+        
+        # Only company_id is required.
+        # Campaign object is optional, but useful if you want to track ROI of acquisition channels
+        # See https://www.moesif.com/docs/api#update-a-company for campaign schema
+        # metadata can be any custom object
+        companies = [{
+          'company_id': '67890',
+          'company_domain': 'acmeinc.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
+          'campaign': {
+            'utm_source': 'google',
+            'utm_medium': 'cpc', 
+            'utm_campaign': 'adwords',
+            'utm_term': 'api+tooling',
+            'utm_content': 'landing'
+          },
+          'metadata': {
+            'org_name': 'Acme, Inc',
+            'plan_name': 'Free',
+            'deal_stage': 'Lead',
+            'mrr': 24000,
+            'demographics': {
+                'alexa_ranking': 500000,
+                'employee_count': 47
+            },
+          }
+        },
+        {
+          'company_id': '09876',
+          'company_domain': 'contoso.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
+          'campaign': {
+            'utm_source': 'facebook',
+            'utm_medium': 'cpc', 
+            'utm_campaign': 'retargeting'
+          },
+          'metadata': {
+            'org_name': 'Contoso, Inc',
+            'plan_name': 'Paid',
+            'deal_stage': 'Lead',
+            'mrr': 48000,
+            'demographics': {
+                'alexa_ranking': 500000,
+                'employee_count': 53
+            },
+          }
+        }]
+        
+        update_company = api_client.update_companies(companies)
+        ```
+        
+        ## How to test:
+        
+        You can test the SDK with automatically generated test
+        cases. unittest is used as the testing framework and nose is used as the test
+        runner. You can run the tests as follows:
+        
+          1. Manually clone the git repo
+          2. From terminal/cmd navigate to the root directory of the SDK.
+          3. Invoke 'pip install -r requirements.txt'
+          4. Add your own application id to 'test/controllers/controller_test_base'
+          5. Invoke 'nosetests tests/controllers/test_api_controller.py'
+        
+          [ico-built-for]: https://img.shields.io/badge/built%20for-python-blue.svg
+          [ico-version]: https://img.shields.io/pypi/v/moesifapi.svg
+          [ico-language]: https://img.shields.io/pypi/pyversions/moesifapi.svg
+          [ico-license]: https://img.shields.io/badge/License-Apache%202.0-green.svg
+          [ico-source]: https://img.shields.io/github/last-commit/moesif/moesifapi-python.svg?style=social
+        
+          [link-built-for]: https://www.python.org/
+          [link-package]: https://pypi.python.org/pypi/moesifapi
+          [link-language]: https://pypi.python.org/pypi/moesifapi
+          [link-license]: https://raw.githubusercontent.com/Moesif/moesifapi-python/master/LICENSE
+          [link-source]: https://github.com/Moesif/moesifapi-python
+        
 Keywords: log analysis restful api development debug
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: Log Analysis
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Software Development :: Libraries
@@ -21,345 +356,7 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
-License-File: LICENSE
-
-# MoesifApi Lib for Python
-
-[![Built For][ico-built-for]][link-built-for]
-[![Latest Version][ico-version]][link-package]
-[![Language Versions][ico-language]][link-language]
-[![Software License][ico-license]][link-license]
-[![Source Code][ico-source]][link-source]
-
-[Source Code on GitHub](https://github.com/moesif/moesifapi-python)
-
-This SDK uses the Requests library and will work for Python 2.7 — 3.5.
-
-If you are using Django as your platform, we have [moesifapi-python](https://github.com/Moesif/moesifapi-python) middleware, you can use that middleware directly.
-
-__Check out Moesif's [Developer Documentation](https://www.moesif.com/docs) and [Python API Reference](https://www.moesif.com/docs/api?python) to learn more__
-
-
-## How to install:
-
-```
-pip install moesifapi
-```
-
-## How to use:
-
-The code uses Python packages named requests, jsonpickle and dateutil.
-After having resolved the dependencies, you can easily use the SDK following these steps.
-
-Your Moesif Application Id can be found in the [_Moesif Portal_](https://www.moesif.com/).
-After signing up for a Moesif account, your Moesif Application Id will be displayed during the onboarding steps. 
-
-You can always find your Moesif Application Id at any time by logging 
-into the [_Moesif Portal_](https://www.moesif.com/), click on the top right menu,
- and then clicking _Installation_.
-
-### Create Event
-
-```python
-from __future__ import print_function
-from moesifapi.moesif_api_client import *
-from moesifapi.models import *
-
-client = MoesifAPIClient(my_application_id)
-api_client = client.api
-
-# Note: we recommend sending all API Calls via MVC framework middleware.
-
-req_headers = APIHelper.json_deserialize("""  {
-  "Host": "api.acmeinc.com",
-  "Accept": "*/*",
-  "Connection": "Keep-Alive",
-  "User-Agent": "Dalvik/2.1.0 (Linux; U; Android 5.0.2; C6906 Build/14.5.A.0.242)",
-  "Content-Type": "application/json",
-  "Content-Length": "126",
-  "Accept-Encoding": "gzip"
-} """)
-
-req_body = APIHelper.json_deserialize( """{
-  "items": [
-    {
-      "type": 1,
-      "id": "fwfrf"
-    },
-    {
-      "type": 2,
-      "id": "d43d3f"
-    }
-  ]
-}""")
-
-rsp_headers = APIHelper.json_deserialize("""  {
-    "Date": "Tue, 23 Aug 2019 23:46:49 GMT",
-    "Vary": "Accept-Encoding",
-    "Pragma": "no-cache",
-    "Expires": "-1",
-    "Content-Type": "application/json; charset=utf-8"
-    "Cache-Control": "no-cache"
-  } """)
-
-rsp_body = APIHelper.json_deserialize( """{
-    "Error": "InvalidArgumentException",
-    "Message": "Missing field field_a"
-  }""")
-
-metadata = APIHelper.json_deserialize("""{
-    "field1": "foo",
-    "field2": "bar"
-  }""")
-
-
-
-event_req = EventRequestModel(time = "2019-09-09T04:45:42.914",
-    uri = "https://api.acmeinc.com/items/reviews/",
-    verb = "PATCH",
-    api_version = "1.1.0",
-    ip_address = "61.48.220.123",
-    headers = req_headers,
-    body = req_body)
-
-event_rsp = EventResponseModel(time = "2019-09-09T04:45:42.914",
-    status = 500,
-    headers = rsp_headers,
-    body = rsp_body)
-
-event_model = EventModel(request = event_req,
-    response = event_rsp,
-    user_id = "12345",
-    company_id = "67890",
-    session_token = "23jdf0owekfmcn4u3qypxg09w4d8ayrcdx8nu2ng]s98y18cx98q3yhwmnhcfx43f",
-    metadata = metadata)
-
-
-# Perform the API call through the SDK function
-api_client.create_event(event_model)
-
-
-api_client.create_event(my_api_event_model)
-```
-
-## Update a Single User
-
-Create or update a user profile in Moesif.
-The metadata field can be any customer demographic or other info you want to store.
-Only the `userId` field is required.
-For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-a-user).
-
-```python
-from moesifapi.moesif_api_client import *
-from moesifapi.models import *
-
-api_client = MoesifAPIClient("YOUR_COLLECTOR_APPLICATION_ID").api
-
-# Only user_id is required.
-# Campaign object is optional, but useful if you want to track ROI of acquisition channels
-# See https://www.moesif.com/docs/api#users for campaign schema
-# metadata can be any custom object
-user = {
-  'user_id': '12345',
-  'company_id': '67890', # If set, associate user with a company object
-  'campaign': {
-    'utm_source': 'google',
-    'utm_medium': 'cpc', 
-    'utm_campaign': 'adwords',
-    'utm_term': 'api+tooling',
-    'utm_content': 'landing'
-  },
-  'metadata': {
-    'email': 'john@acmeinc.com',
-    'first_name': 'John',
-    'last_name': 'Doe',
-    'title': 'Software Engineer',
-    'sales_info': {
-        'stage': 'Customer',
-        'lifetime_value': 24000,
-        'account_owner': 'mary@contoso.com'
-    },
-  }
-}
-
-update_user = api_client.update_user(user)
-```
-
-## Update Users in Batch
-
-Similar to UpdateUser, but used to update a list of users in one batch. 
-Only the `userId` field is required.
-For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-users-in-batch).
-
-```python
-from moesifapi.moesif_api_client import *
-from moesifapi.models import *
-
-api_client = MoesifAPIClient("YOUR_COLLECTOR_APPLICATION_ID").api
-
-userA = {
-  'user_id': '12345',
-  'company_id': '67890', # If set, associate user with a company object
-  'metadata': {
-    'email': 'john@acmeinc.com',
-    'first_name': 'John',
-    'last_name': 'Doe',
-    'title': 'Software Engineer',
-    'sales_info': {
-        'stage': 'Customer',
-        'lifetime_value': 24000,
-        'account_owner': 'mary@contoso.com'
-    },
-  }
-}
-
-userB = {
-  'user_id': '54321',
-  'company_id': '67890', # If set, associate user with a company object
-  'metadata': {
-    'email': 'mary@acmeinc.com',
-    'first_name': 'Mary',
-    'last_name': 'Jane',
-    'title': 'Software Engineer',
-    'sales_info': {
-        'stage': 'Customer',
-        'lifetime_value': 48000,
-        'account_owner': 'mary@contoso.com'
-    },
-  }
-}
-update_users = api_client.update_users_batch([userA, userB])
-```
-
-## Update a Single Company
-
-Create or update a company profile in Moesif.
-The metadata field can be any company demographic or other info you want to store.
-Only the `companyId` field is required.
-For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-a-company).
-
-```python
-from moesifapi.moesif_api_client import *
-from moesifapi.models import *
-
-api_client = MoesifAPIClient("YOUR_COLLECTOR_APPLICATION_ID").api
-
-# Only company_id is required.
-# Campaign object is optional, but useful if you want to track ROI of acquisition channels
-# See https://www.moesif.com/docs/api#update-a-company for campaign schema
-# metadata can be any custom object
-company = {
-  'company_id': '12345',
-  'company_domain': 'acmeinc.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
-  'campaign': {
-    'utm_source': 'google',
-    'utm_medium': 'cpc', 
-    'utm_campaign': 'adwords',
-    'utm_term': 'api+tooling',
-    'utm_content': 'landing'
-  },
-  'metadata': {
-    'org_name': 'Acme, Inc',
-    'plan_name': 'Free',
-    'deal_stage': 'Lead',
-    'mrr': 24000,
-    'demographics': {
-        'alexa_ranking': 500000,
-        'employee_count': 47
-    },
-  }
-}
-
-update_company = api_client.update_company(company)
-```
-
-## Update Companies in Batch
-
-Similar to updateCompany, but used to update a list of companies in one batch. 
-Only the `companyId` field is required.
-For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-companies-in-batch).
-
-
-```python
-from moesifapi.moesif_api_client import *
-from moesifapi.models import *
-
-api_client = MoesifAPIClient("YOUR_COLLECTOR_APPLICATION_ID").api
-
-# Only company_id is required.
-# Campaign object is optional, but useful if you want to track ROI of acquisition channels
-# See https://www.moesif.com/docs/api#update-a-company for campaign schema
-# metadata can be any custom object
-companies = [{
-  'company_id': '67890',
-  'company_domain': 'acmeinc.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
-  'campaign': {
-    'utm_source': 'google',
-    'utm_medium': 'cpc', 
-    'utm_campaign': 'adwords',
-    'utm_term': 'api+tooling',
-    'utm_content': 'landing'
-  },
-  'metadata': {
-    'org_name': 'Acme, Inc',
-    'plan_name': 'Free',
-    'deal_stage': 'Lead',
-    'mrr': 24000,
-    'demographics': {
-        'alexa_ranking': 500000,
-        'employee_count': 47
-    },
-  }
-},
-{
-  'company_id': '09876',
-  'company_domain': 'contoso.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
-  'campaign': {
-    'utm_source': 'facebook',
-    'utm_medium': 'cpc', 
-    'utm_campaign': 'retargeting'
-  },
-  'metadata': {
-    'org_name': 'Contoso, Inc',
-    'plan_name': 'Paid',
-    'deal_stage': 'Lead',
-    'mrr': 48000,
-    'demographics': {
-        'alexa_ranking': 500000,
-        'employee_count': 53
-    },
-  }
-}]
-
-update_company = api_client.update_companies(companies)
-```
-
-## How to test:
-
-You can test the SDK with automatically generated test
-cases. unittest is used as the testing framework and nose is used as the test
-runner. You can run the tests as follows:
-
-  1. Manually clone the git repo
-  2. From terminal/cmd navigate to the root directory of the SDK.
-  3. Invoke 'pip install -r requirements.txt'
-  4. Add your own application id to 'test/controllers/controller_test_base'
-  5. Invoke 'nosetests tests/controllers/test_api_controller.py'
-
-  [ico-built-for]: https://img.shields.io/badge/built%20for-python-blue.svg
-  [ico-version]: https://img.shields.io/pypi/v/moesifapi.svg
-  [ico-language]: https://img.shields.io/pypi/pyversions/moesifapi.svg
-  [ico-license]: https://img.shields.io/badge/License-Apache%202.0-green.svg
-  [ico-source]: https://img.shields.io/github/last-commit/moesif/moesifapi-python.svg?style=social
-
-  [link-built-for]: https://www.python.org/
-  [link-package]: https://pypi.python.org/pypi/moesifapi
-  [link-language]: https://pypi.python.org/pypi/moesifapi
-  [link-license]: https://raw.githubusercontent.com/Moesif/moesifapi-python/master/LICENSE
-  [link-source]: https://github.com/Moesif/moesifapi-python
-
-
```

### Comparing `moesifapi-1.4.0/moesifapi.egg-info/SOURCES.txt` & `moesifapi-1.4.1/moesifapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.0/setup.py` & `moesifapi-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 setup(
     name='moesifapi',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.4.0',
+    version='1.4.1',
 
     description='Moesif API Lib for Python',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     # The project's main homepage.
     url='https://www.moesif.com/docs/api?python#api-libs',
```

### Comparing `moesifapi-1.4.0/tests/controllers/controller_test_base.py` & `moesifapi-1.4.1/tests/controllers/controller_test_base.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.0/tests/controllers/test_api_controller.py` & `moesifapi-1.4.1/tests/controllers/test_api_controller.py`

 * *Files identical despite different names*

