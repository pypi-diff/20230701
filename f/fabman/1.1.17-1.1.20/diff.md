# Comparing `tmp/fabman-1.1.17.tar.gz` & `tmp/fabman-1.1.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabman-1.1.17.tar", last modified: Wed Jun 28 22:58:15 2023, max compression
+gzip compressed data, was "fabman-1.1.20.tar", last modified: Fri Jun 30 23:11:11 2023, max compression
```

## Comparing `fabman-1.1.17.tar` & `fabman-1.1.20.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:58:15.227360 fabman-1.1.17/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-28 22:58:04.000000 fabman-1.1.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-28 22:58:15.227360 fabman-1.1.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-28 22:58:04.000000 fabman-1.1.17/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:58:15.223360 fabman-1.1.17/fabman/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-28 22:58:04.000000 fabman-1.1.17/fabman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-28 22:58:04.000000 fabman-1.1.17/fabman/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-28 22:58:04.000000 fabman-1.1.17/fabman/api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-28 22:58:04.000000 fabman-1.1.17/fabman/booking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-28 22:58:04.000000 fabman-1.1.17/fabman/charge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-28 22:58:04.000000 fabman-1.1.17/fabman/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21268 2023-06-28 22:58:04.000000 fabman-1.1.17/fabman/fabman.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-28 22:58:04.000000 fabman-1.1.17/fabman/fabman_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-28 22:58:04.000000 fabman-1.1.17/fabman/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-28 22:58:04.000000 fabman-1.1.17/fabman/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    19794 2023-06-28 22:58:04.000000 fabman-1.1.17/fabman/member.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-06-28 22:58:04.000000 fabman-1.1.17/fabman/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-28 22:58:04.000000 fabman-1.1.17/fabman/paginated_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-28 22:58:04.000000 fabman-1.1.17/fabman/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-28 22:58:04.000000 fabman-1.1.17/fabman/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-06-28 22:58:04.000000 fabman-1.1.17/fabman/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-28 22:58:04.000000 fabman-1.1.17/fabman/resource_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-28 22:58:04.000000 fabman-1.1.17/fabman/resource_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-06-28 22:58:04.000000 fabman-1.1.17/fabman/space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-28 22:58:04.000000 fabman-1.1.17/fabman/training_course.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-28 22:58:04.000000 fabman-1.1.17/fabman/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-28 22:58:04.000000 fabman-1.1.17/fabman/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:58:15.227360 fabman-1.1.17/fabman.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-28 22:58:15.000000 fabman-1.1.17/fabman.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-28 22:58:15.000000 fabman-1.1.17/fabman.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 22:58:15.000000 fabman-1.1.17/fabman.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-28 22:58:15.000000 fabman-1.1.17/fabman.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-28 22:58:15.000000 fabman-1.1.17/fabman.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-28 22:58:04.000000 fabman-1.1.17/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-28 22:58:15.227360 fabman-1.1.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-28 22:58:04.000000 fabman-1.1.17/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:58:15.227360 fabman-1.1.17/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-28 22:58:04.000000 fabman-1.1.17/tests/test_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-28 22:58:04.000000 fabman-1.1.17/tests/test_api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-28 22:58:04.000000 fabman-1.1.17/tests/test_booking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-28 22:58:04.000000 fabman-1.1.17/tests/test_charge.py
--rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-06-28 22:58:04.000000 fabman-1.1.17/tests/test_fabman.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-28 22:58:04.000000 fabman-1.1.17/tests/test_invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-28 22:58:04.000000 fabman-1.1.17/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-06-28 22:58:04.000000 fabman-1.1.17/tests/test_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-06-28 22:58:04.000000 fabman-1.1.17/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-28 22:58:04.000000 fabman-1.1.17/tests/test_paginated_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-28 22:58:04.000000 fabman-1.1.17/tests/test_payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-06-28 22:58:04.000000 fabman-1.1.17/tests/test_requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-28 22:58:04.000000 fabman-1.1.17/tests/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-28 22:58:04.000000 fabman-1.1.17/tests/test_resource_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-28 22:58:04.000000 fabman-1.1.17/tests/test_resource_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-28 22:58:04.000000 fabman-1.1.17/tests/test_sanity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-06-28 22:58:04.000000 fabman-1.1.17/tests/test_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-28 22:58:04.000000 fabman-1.1.17/tests/test_training_course.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-28 22:58:04.000000 fabman-1.1.17/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-28 22:58:04.000000 fabman-1.1.17/tests/test_webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:11.561270 fabman-1.1.20/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-30 23:10:59.000000 fabman-1.1.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-30 23:11:11.561270 fabman-1.1.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-30 23:10:59.000000 fabman-1.1.20/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:11.557270 fabman-1.1.20/fabman/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/booking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25890 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/fabman.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/fabman_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23297 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/paginated_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/resource_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/resource_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10862 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/training_course.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:11.557270 fabman-1.1.20/fabman.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-30 23:11:11.000000 fabman-1.1.20/fabman.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-30 23:11:11.000000 fabman-1.1.20/fabman.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 23:11:11.000000 fabman-1.1.20/fabman.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-30 23:11:11.000000 fabman-1.1.20/fabman.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 23:11:11.000000 fabman-1.1.20/fabman.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-30 23:10:59.000000 fabman-1.1.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-30 23:11:11.561270 fabman-1.1.20/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-30 23:10:59.000000 fabman-1.1.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:11.561270 fabman-1.1.20/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_booking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18081 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_fabman.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14450 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_paginated_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_resource_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_resource_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_sanity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_training_course.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_webhook.py
```

### Comparing `fabman-1.1.17/LICENSE` & `fabman-1.1.20/LICENSE`

 * *Files identical despite different names*

### Comparing `fabman-1.1.17/PKG-INFO` & `fabman-1.1.20/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: fabman
-Version: 1.1.17
+Version: 1.1.20
 Summary: Python wrappers for interacting with the Fabman API
 Author: Davin Lawrence
 Author-email: Davin Lawrence <davin.lawrence@utexas.edu>
 Project-URL: Homepage, https://github.com/utexas-engr-tiw/fabman-api
+Project-URL: Documentation, https://fabman-api.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/utexas-engr-tiw/fabman-api/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -25,14 +26,16 @@
 
 [![Fabman on PyPI](https://img.shields.io/pypi/v/fabman.svg)](https://pypi.python.org/pypi/fabman)
 [![License](https://img.shields.io/pypi/l/fabman.svg)](https://pypi.python.org/pypi/fabman)
 [![Python Versions](https://img.shields.io/pypi/pyversions/fabman.svg)](https://pypi.python.org/pypi/fabman)
 [![Build Status](https://github.com/utexas-engr-tiw/fabman-api/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/utexas-engr-tiw/fabman-api/actions)
 [![Coverage](https://codecov.io/gh/utexas-engr-tiw/fabman-api/branch/main/graph/badge.svg?token=AGABZU5YOJ)](https://codecov.io/gh/utexas-engr-tiw/fabman-api)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Documentation Status](https://readthedocs.org/projects/fabman-api/badge/?version=latest)](https://fabman-api.readthedocs.io/en/latest/?badge=latest)
+
 
 # Fabman API 
 
 Library for interfacing with the Fabman API. Created for Texas Inventionworks as part of the Cockrell School of Engineering at the University of Texas at Austin.
 
 Official documentation for the Fabman API can be found [here](https://github.com/FabmanHQ/fabman-api). Live interaction and description of all endpoints can further be found [here](https://fabman.io/api/v1/documentation#/). This library is currently targeting version 2.3.1 of the Fabman API.
 
@@ -56,19 +59,20 @@
 f = Fabman(API_KEY)
 ...
 ```
 
 From there, you can begin interacting with api endpoints as described in the official documentation. Most top-level methods return an object which manages that object. For example, to get a single member and update that member's name,
 ```python
 member = f.get_member(12345)
-member.update(firstName="Natalie", lastName="Wynn")
+member.update(firstName="Kira", lastName="Nerys")
 ```
+
 All parameters except for IDs are taken in as kwargs and should follow the camelCase naming conventions found on the Fabman API. Moreover, the library performs minimal checking of parameters, leaving that to the Fabman API. For required fields for create and update fields, refer to the [Live Fabman API Documentation](https://fabman.io/api/v1/documentation#/). The one exception to this is the `lockVersion` requirement for update methods. All update methods will automatically add the current `lockVersion` parameter to the body.
 
+Refer to the [library documentation](https://fabman-api.readthedocs.io/en/latest/) more information on this library.
+
 ## Contributing
 
 We would love contributions! We are a small development team. To contribute, familiarize yourself with the code, the layout, make your edits and a pull request. We currently need help with
 
-* Writing Mock Tests
-* Coverage of API endpoints
 * Real life testing of the API
 * Documentation
```

### Comparing `fabman-1.1.17/README.md` & `fabman-1.1.20/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 [![Fabman on PyPI](https://img.shields.io/pypi/v/fabman.svg)](https://pypi.python.org/pypi/fabman)
 [![License](https://img.shields.io/pypi/l/fabman.svg)](https://pypi.python.org/pypi/fabman)
 [![Python Versions](https://img.shields.io/pypi/pyversions/fabman.svg)](https://pypi.python.org/pypi/fabman)
 [![Build Status](https://github.com/utexas-engr-tiw/fabman-api/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/utexas-engr-tiw/fabman-api/actions)
 [![Coverage](https://codecov.io/gh/utexas-engr-tiw/fabman-api/branch/main/graph/badge.svg?token=AGABZU5YOJ)](https://codecov.io/gh/utexas-engr-tiw/fabman-api)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Documentation Status](https://readthedocs.org/projects/fabman-api/badge/?version=latest)](https://fabman-api.readthedocs.io/en/latest/?badge=latest)
+
 
 # Fabman API 
 
 Library for interfacing with the Fabman API. Created for Texas Inventionworks as part of the Cockrell School of Engineering at the University of Texas at Austin.
 
 Official documentation for the Fabman API can be found [here](https://github.com/FabmanHQ/fabman-api). Live interaction and description of all endpoints can further be found [here](https://fabman.io/api/v1/documentation#/). This library is currently targeting version 2.3.1 of the Fabman API.
 
@@ -31,19 +33,20 @@
 f = Fabman(API_KEY)
 ...
 ```
 
 From there, you can begin interacting with api endpoints as described in the official documentation. Most top-level methods return an object which manages that object. For example, to get a single member and update that member's name,
 ```python
 member = f.get_member(12345)
-member.update(firstName="Natalie", lastName="Wynn")
+member.update(firstName="Kira", lastName="Nerys")
 ```
+
 All parameters except for IDs are taken in as kwargs and should follow the camelCase naming conventions found on the Fabman API. Moreover, the library performs minimal checking of parameters, leaving that to the Fabman API. For required fields for create and update fields, refer to the [Live Fabman API Documentation](https://fabman.io/api/v1/documentation#/). The one exception to this is the `lockVersion` requirement for update methods. All update methods will automatically add the current `lockVersion` parameter to the body.
 
+Refer to the [library documentation](https://fabman-api.readthedocs.io/en/latest/) more information on this library.
+
 ## Contributing
 
 We would love contributions! We are a small development team. To contribute, familiarize yourself with the code, the layout, make your edits and a pull request. We currently need help with
 
-* Writing Mock Tests
-* Coverage of API endpoints
 * Real life testing of the API
 * Documentation
```

### Comparing `fabman-1.1.17/fabman/account.py` & `fabman-1.1.20/fabman/account.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,16 +15,19 @@
         return f"Account #{self.id}: {self.name}"
 
     def update(self, **kwargs) -> None:
         """
         Update information on the account. Note that many fields may be unalterable
         by the API key holder.
 
-        Calls "PUT /accounts/{id}"
-        Documentation: https://fabman.io/api/v1/documentation#/account/putAccountsId
+        :calls: "PUT /accounts/{id}" \
+		<https://fabman.io/api/v1/documentation#/account/putAccountsId>
+
+        :returns: None
+        :rtype: None
         """
         uri = f"/accounts/{self.id}"
 
         kwargs.update({"lockVersion": self.lockVersion})
 
         response = self._requester.request("PUT", uri, _kwargs=kwargs)
 
@@ -33,14 +36,18 @@
         for attr, val in data.items():
             setattr(self, attr, val)
 
     def get_payment_info(self, **kwargs) -> requests.Response:
         """
         Get information about the payment plan of the account.
 
-        Calls "GET /accounts/{id}/payment-info"
+        :calls: "GET /accounts/{id}/payment-info" \
+        <https://fabman.io/api/v1/documentation#/accounts/getAccountsIdPaymentinfo>
+        
+        :returns: Information about the payment plan of the account.
+        :rtype: dict
         """
         uri = f"/accounts/{self.id}/payment-info"
 
         response = self._requester.request("GET", uri, _kwargs=kwargs)
 
         return response.json()
```

### Comparing `fabman-1.1.17/fabman/api_key.py` & `fabman-1.1.20/fabman/api_key.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,54 +2,65 @@
 
 import requests
 
 from fabman.fabman_object import FabmanObject
 
 
 class ApiKey(FabmanObject):
-    """Class for interacting with the api-keys endpoints on the Fabman API"""
+    """
+    Class for interacting with the api-keys endpoints on the Fabman API
+    """
 
     def __str__(self):
         return f"ApiKey #{self.id}: {self.label}"
 
     def delete(self, **kwargs) -> requests.Response:
         """
         Deletes an api-key. *WARNING: This is irreversible.*
 
-        Calls "DELETE /api-keys/{apiKeyId}"
-        Documentation https://fabman.io/api/v1/documentation#/api-keys/deleteApiKeysId
+        :calls: "DELETE /api-keys/{apiKeyId}" \
+		<https://fabman.io/api/v1/documentation#/api-keys/deleteApiKeysId>
+  
+        :returns: Response from the API with status code 204 (No Content) if successful
+        :rtype: requests.Response
         """
 
         uri = f"/api-keys/{self.id}"
 
         response = self._requester.request("DELETE", uri, _kwargs=kwargs)
 
         return response
 
     def get_token(self, **kwargs) -> requests.Response:
         """
         Returns the token for an api-key. Must be called with a valid api-key.
 
-        Calls "GET /api-keys/{apiKeyId}/token"
-        Documentation https://fabman.io/api/v1/documentation#/api-keys/getApiKeysIdToken
+        :calls: "GET /api-keys/{apiKeyId}/token" \
+		<https://fabman.io/api/v1/documentation#/api-keys/getApiKeysIdToken>
+  
+        :returns: Response from the API with status code 200 (OK) if successful
+        :rtype: requests.Response
         """
 
         uri = f"/api-keys/{self.id}/token"
 
         response = self._requester.request("GET", uri, _kwargs=kwargs)
 
         return response.json()
 
     def update(self, **kwargs) -> None:
         """
         Updates the api-key. Attributes are updated in place with new information
         returned by the API.
 
-        Calls "PUT /api-keys/{apiKeyId}"
-        Documentation https://fabman.io/api/v1/documentation#/api-keys/putApiKeysId
+        :calls: "PUT /api-keys/{apiKeyId}" \
+		<https://fabman.io/api/v1/documentation#/api-keys/putApiKeysId>
+  
+        :returns: None
+        :rtype: None
         """
 
         uri = f"/api-keys/{self.id}"
 
         kwargs.update({"lockVersion": self.lockVersion})
         response = self._requester.request("PUT", uri, _kwargs=kwargs)
```

### Comparing `fabman-1.1.17/fabman/booking.py` & `fabman-1.1.20/fabman/booking.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,31 +14,37 @@
     def __str__(self):
         return f"Booking #{self.id}: {self.fromDateTime} - {self.untilDateTime}"
 
     def delete(self, **kwargs) -> requests.Response:
         """
         Deletes the booking. *WARNING: THIS CANNOT BE UNDONE.*
 
-        Calls "DELETE /bookings/{id}"
-        Documentation: https://fabman.io/api/v1/documentation#/bookings/deleteBookingsId
+        :calls: "DELETE /bookings/{id}" \
+		<https://fabman.io/api/v1/documentation#/bookings/deleteBookingsId>
+  
+        :returns: Response from the API with status code 204 (No Content) if successful
+        :rtype: requests.Response
         """
 
         uri = f"/bookings/{self.id}"
 
         response = self._requester.request("DELETE", uri, _kwargs=kwargs)
 
         return response
 
     def update(self, **kwargs) -> None:
         """
         Update the booking object on the server. Returns the updated booking object.
         Updates all information in place.
 
-        Calls "PUT /bookings/{id}"
-        Documentation: https://fabman.io/api/v1/documentation#/bookings/putBookingsId
+        :calls: "PUT /bookings/{id}" \
+		<https://fabman.io/api/v1/documentation#/bookings/putBookingsId>
+
+        :returns: None
+        :rtype: None
         """
 
         uri = f"/bookings/{self.id}"
 
         kwargs.update({"lockVersion": self.lockVersion})
 
         response = self._requester.request("PUT", uri, _kwargs=kwargs)
```

### Comparing `fabman-1.1.17/fabman/charge.py` & `fabman-1.1.20/fabman/charge.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,31 +11,37 @@
     def __str__(self):
         return f"Charge #{self.id}: {self.price} {self.description}"
 
     def delete(self, **kwargs) -> requests.Response:
         """
         Deletes the charge. *WARNING: THIS CANNOT BE UNDONE.*
 
-        Calls "DELETE /charges/{id}"
-        Documentation: https://fabman.io/api/v1/documentation
+        :calls: "DELETE /charges/{id}" \
+		<https://fabman.io/api/v1/documentation#/charges/deleteChargesId>
+  
+        :returns: Response from the API with status code 204 (No Content) if successful
+        :rlist: requests.Response
         """
 
         response = self._requester.request(
             "DELETE", f"/charges/{self.id}", _kwargs=kwargs
         )
 
         return response
 
     def update(self, **kwargs) -> None:
         """
         Update the charge object on the server. Updates all information in place
         with returned data from the server.
 
-        Calls "PUT /charges/{id}"
-        Documentation: https://fabman.io/api/v1/documentation#/charges/putChargesId
+        :calls: "PUT /charges/{id}" \
+		<https://fabman.io/api/v1/documentation#/charges/putChargesId>
+  
+        :returns: None
+        :rlist: None
         """
 
         kwargs.update({"lockVersion": self.lockVersion})
 
         response = self._requester.request("PUT", f"/charges/{self.id}", _kwargs=kwargs)
 
         data = response.json()
```

### Comparing `fabman-1.1.17/fabman/exceptions.py` & `fabman-1.1.20/fabman/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,38 +16,55 @@
             self.message = message
 
     def __str__(self):
         return str(self.message)
 
 
 class BadRequest(FabmanException):
-    """Fabman was unable to understand the request. More information may be needed"""
+    """
+    Fabman was unable to understand the request. More information may be needed or
+    arguments may need to be fixed.
+    """
 
 
 class InvalidAccessToken(FabmanException):
-    """The access token provided was invalid"""
+    """
+    The access token provided was invalid.
+    """
 
 
 class Unauthorized(FabmanException):
-    """The access token provided was not authorized to access the resource"""
+    """
+    The access token provided was not authorized to access the resource.
+    """
 
 
 class ResourceDoesNotExist(FabmanException):
-    """The resource requested does not exist"""
+    """
+    The resource requested does not exist.
+    """
 
 
 class ForbiddenError(FabmanException):
-    """The access token provided does not have permission to access the resource"""
+    """
+    The access token provided does not have permission to access the resource.
+    """
 
 
 class Conflict(FabmanException):
-    """The request could not be completed due to a conflict with the current
-    state of the resource"""
+    """
+    The request could not be completed due to a conflict with the current
+    state of the resource.
+    """
 
 
 class UnprocessableEntity(FabmanException):
-    """The request was well-formed but was unable to be followed due to semantic errors"""
+    """
+    The request was well-formed but was unable to be followed due to semantic errors.
+    """
 
 
 class RateLimitExceeded(FabmanException):
-    """The request was valid, but too may requests have been issued from this access token.
-    Please try again later"""
+    """
+    The request was valid, but too may requests have been issued from this access token.
+    Please try again later.
+    """
```

### Comparing `fabman-1.1.17/fabman/invoice.py` & `fabman-1.1.20/fabman/invoice.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,31 +11,37 @@
     def __str__(self):
         return f"Invoice #{self.id}: {self.total} {self.state}"
 
     def cancel(self) -> requests.Response:
         """
         Cancels an invoice. Takes no arguments.
 
-        Calls "POST /invoices/{id}/cancel"
-        Documentation: https://fabman.io/api/v1/documentation#/invoices/postInvoicesIdCancel
+        :calls: "POST /invoices/{id}/cancel" \
+		<https://fabman.io/api/v1/documentation#/invoices/postInvoicesIdCancel>
+  
+        :returns: An empty dict if successful.
+        :type: dict
         """
 
         data = {"lockVersion": self.lockVersion}
 
         uri = f"/invoices/{self.id}/cancel"
         response = self._requester.request("POST", uri, _kwargs=data)
 
         return response.json()
 
     def details(self, **kwargs) -> requests.Response:
         """
         Returns details about the invoice. Takes no arguments.
 
-        Calls "GET /invoices/{id}/details"
-        Documentation: https://fabman.io/api/v1/documentation
+        :calls: "GET /invoices/{id}/details" \
+		<https://fabman.io/api/v1/documentation>
+  
+        :returns: A dict containing details about the invoice.
+        :rtype: dict
         """
 
         if "details" in self._embedded:
             return self._embedded["details"]
 
         uri = f"/invoices/{self.id}/details"
 
@@ -46,16 +52,19 @@
         return response.json()
 
     def update(self, **kwargs) -> None:
         """
         Updates the invoice. Attributes are updated in place with new information
         provided by the API
 
-        Calls "PUT /invoices/{id}"
-        Documentation: https://fabman.io/api/v1/documentation#/invoices/putInvoicesId
+        :calls: "PUT /invoices/{id}" \
+		<https://fabman.io/api/v1/documentation#/invoices/putInvoicesId>
+  
+        :returns: None -- updates attributes of the current object
+        :rtype: None
         """
 
         kwargs.update({"lockVersion": self.lockVersion})
 
         uri = f"/invoices/{self.id}"
         response = self._requester.request("PUT", uri, _kwargs=kwargs)
```

### Comparing `fabman-1.1.17/fabman/member.py` & `fabman-1.1.20/fabman/member.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,44 +15,53 @@
     """
 
     def __str__(self):
         return f"{self.id}: {self.scope} - {self.amount}"
 
     def delete(self, **kwargs) -> requests.Response:
         """
-        Deletes a credit from a user account. *WARNING: THIS CANNOT BE UNDONE.*
+        Deletes a credit from a user account. **WARNING: THIS CANNOT BE UNDONE.**
 
-        Calls "DELETE /members/{member_id}/credits/{credit_id}"
-        Documentation https://fabman.io/api/v1/documentation#/members/deleteMembersIdCreditsCreditId
+        :calls: "DELETE /members/{member_id}/credits/{credit_id}" \
+		<https://fabman.io/api/v1/documentation#/members/deleteMembersIdCreditsCreditid>
+
+        :returns: An empty dict if successful.
+        :rtype: dict
         """
         response = self._requester.request(
             "DELETE", f"/members/{self.member_id}/credits/{self.id}", _kwargs=kwargs
         )
 
         return response
 
     def get_uses(self, **kwargs) -> requests.Response:
         """
         Retrieves a list of uses of the credit.
 
-        Calls "GET /members/{member_id}/credits/{credit_id}/uses"
-        Documentation https://fabman.io/api/v1/documentation#/members/getMembersIdCreditsCreditidUses
+        :calls: "GET /members/{member_id}/credits/{credit_id}/uses" \
+		<https://fabman.io/api/v1/documentation#/members/getMembersIdCreditsCreditidUses>
+  
+        :return: A list of uses of the credit.
+        :rtype: list
         """
         response = self._requester.request(
             "GET", f"/members/{self.member_id}/credits/{self.id}/uses", _kwargs=kwargs
         )
 
         return response.json()
 
     def update(self, **kwargs) -> None:
         """
         Updates an existing credit in place
 
-        Calls "PUT /members/{id}/credits/{creditId}"
-        Documentation: https://fabman.io/api/v1/documentation#/members/putMembersIdCreditsCreditId
+        :calls: "PUT /members/{id}/credits/{creditId}" \
+		<https://fabman.io/api/v1/documentation#/members/putMembersIdCreditsCreditid>
+  
+        :returns: None
+        :rtype: None
         """
         kwargs.update({"lockVersion": self.lockVersion})
         response = self._requester.request(
             "PUT", f"/members/{self.member_id}/credits/{self.id}", _kwargs=kwargs
         )
 
         data = response.json()
@@ -67,32 +76,38 @@
     """
 
     def __str__(self):
         return f"{self.member} - {self.type}"
 
     def delete(self, **kwargs) -> requests.Response:
         """
-        Deletes a member key
+        Deletes a member key. **WARNING: THIS CANNOT BE UNDONE.**
 
-        Calls "DELETE /members/{self.member}/key"
-        Documentation: https://fabman.io/api/v1/documentation#/members/deleteMembersIdKey
+        :calls: "DELETE /members/{self.member}/key" \
+		<https://fabman.io/api/v1/documentation#/members/deleteMembersIdKey>
+  
+        :returns: Response information of delete call
+        :rtype: requests.Response
         """
         response = self._requester.request(
             "DELETE", f"/members/{self.member}/key", _kwargs=kwargs
         )
 
         return response
 
     def update(self, **kwargs) -> None:
         """
         Updates a member key and updates the MemberKey object in place with new
         data from the API.
 
-        Calls "PUT /member{self.member}/key"
-        Documentation: https://fabman.io/api/v1/documentation#/members/putMembersIdKey
+        :calls: "PUT /member{self.member}/key" \
+		<https://fabman.io/api/v1/documentation#/members/putMembersIdKey>
+  
+        :returns: None
+        :rtype: None
         """
 
         kwargs.update({"lockVersion": self.lockVersion})
 
         response = self._requester.request(
             "PUT", f"/members/{self.member}/key", _kwargs=kwargs
         )
@@ -110,30 +125,36 @@
 
     def __str__(self):
         return f"{self.id} - {self.package}"
 
     def delete(self, **kwargs) -> requests.Response:
         """Removes the package from the current user account. *WARNING: THIS CANNOT BE UNDONE.*
 
-        Calls "DELETE /members/{id}/packages/{memberPackageId}"
-        Documentation: https://fabman.io/api/v1/documentation#/members/deleteMembersIdPackagesMemberPackageId
+        :calls: "DELETE /members/{id}/packages/{memberPackageId}" \
+		<https://fabman.io/api/v1/documentation#/members/deleteMembersIdPackagesMemberpackageid>
+
+        :returns: Response information of delete call
+        :rtype: requests.Response
         """
 
         response = self._requester.request(
             "DELETE", f"/members/{self.member_id}/packages/{self.id}", _kwargs=kwargs
         )
 
         return response
 
     def get_package(self, **kwargs) -> Package:
         """
         Gets information about the package
 
-        Calls "GET /packages/{id}"
-        Documentation: https://fabman.io/api/v1/documentation#/packages/getPackagesId
+        :calls: "GET /packages/{id}" \
+		<https://fabman.io/api/v1/documentation#/packages/getPackagesId>
+        
+        :returns: :code:`fabman.package.Package` object with Package details
+        :rtype: fabman.package.Package
         """
         if "package" in self._embedded:
             data = self._embedded["package"]
         else:
             response = self._requester.request(
                 "GET", f"/packages/{self.package}", _kwargs=kwargs
             )
@@ -142,16 +163,19 @@
         return Package(self._requester, data)
 
     def update(self, **kwargs) -> None:
         """
         Updates a member package and updates the MemberPackage object in place with new
         data from the API
 
-        Calls "PUT /members/{id}/packages/{memberPackageId}"
-        Documentation: https://fabman.io/api/v1/documentation#/members/putMembersIdPackagesMemberPackageId
+        :calls: "PUT /members/{id}/packages/{memberPackageId}" \
+		<https://fabman.io/api/v1/documentation#/members/putMembersIdPackagesMemberpackageid>
+  
+        :returns: None
+        :rtype: None
         """
         kwargs.update({"lockVersion": self.lockVersion})
 
         response = self._requester.request(
             "PUT", f"/members/{self.member_id}/packages/{self.id}", _kwargs=kwargs
         )
 
@@ -168,16 +192,20 @@
 
     def __str__(self):
         return f"{self.id}: {self.firstName} {self.lastName}"
 
     def create_credit(self, **kwargs) -> MemberCredit:
         """
         Creates a member credit
-        calls "POST /members/{id}/credits"
-        Documentation: https://fabman.io/api/v1/documentation#/members/postMembersIdCredits
+        
+        :calls: "POST /members/{id}/credits" \
+		<https://fabman.io/api/v1/documentation#/members/postMembersIdCredits>
+
+        :returns: :code:`fabman.member.MemberCredit` object with credit details
+        :rtype: fabman.member.MemberCredit
         """
 
         kwargs.update({"lockVersion": self.lockVersion})
 
         response = self._requester.request(
             "POST",
             f"/members/{self.id}/credits",
@@ -190,132 +218,178 @@
         return MemberCredit(self._requester, data)
 
     def create_key(self, **kwargs) -> MemberKey:
         """
         Creates a key for the member if one does not already exist. If member already has
         a key, use `update_key()`.
 
-        Calls "POST /members/{id}/key"
-        Documentation: https://fabman.io/api/v1/documentation#/members/postMembersIdKey
+        :calls: "POST /members/{id}/key" \
+		<https://fabman.io/api/v1/documentation#/members/postMembersIdKey>
+  
+        :returns: :code:`fabman.member.MemberKey` object with key details
+        :rtype: fabman.member.MemberKey
         """
 
         response = self._requester.request(
             "POST", f"/members/{self.id}/key", _kwargs=kwargs
         )
 
         return MemberKey(self._requester, response.json())
 
     def delete(self, **kwargs) -> requests.Response:
         """
         Deletes a member
-        calls "DELETE /members/{id}"
-        Documentation: https://fabman.io/api/v1/documentation#/members/deleteMembersId
+        
+        :calls: "DELETE /members/{id}" \
+		<https://fabman.io/api/v1/documentation#/members/deleteMembersId>
+  
+        :returns: Response information of delete call
+        :rtype: requests.Response
         """
         return self._requester.request(
             "DELETE",
             f"/members/{self.id}",
             _kwargs=kwargs,
         )
 
     def delete_change(self, change_id: int, **kwargs) -> requests.Response:
         """
         Deletes a member change given change ID
-        calls "DELETE /members/{id}/changes/{changeId}"
-        Documentation: https://fabman.io/api/v1/documentation#/members/deleteMembersIdChangesChangeId
+        
+        :calls: "DELETE /members/{id}/changes/{changeId}" \
+		<https://fabman.io/api/v1/documentation#/members/deleteMembersIdChangesChangeid>
+
+        :param change_id: ID of the change to delete
+        :type change_id: int
+        :return: Response information of delete call
+        :rtype: requests.Response
         """
         return self._requester.request(
             "DELETE",
             f"/members/{self.id}/changes/{change_id}",
             _kwargs=kwargs,
         )
 
     def delete_device_change(self, change_id: int, **kwargs) -> requests.Response:
         """
         Deletes a member device change given change ID
-        Calls "DELETE /members/{id}/device/changes/{changeId}"
-        Documentation: https://fabman.io/api/v1/documentation#/members/deleteMembersIdDeviceChangesChangeId
+        
+        :calls: "DELETE /members/{id}/device/changes/{changeId}" \
+		<https://fabman.io/api/v1/documentation#/members/deleteMembersIdDeviceChangesChangeid>
+
+        :param change_id: ID of the change to delete
+        :type change_id: int
+        :returns: Response information of delete call
+        :rtype: requests.Response
         """
         return self._requester.request(
             "DELETE",
             f"/members/{self.id}/device/changes/{change_id}",
             _kwargs=kwargs,
         )
 
     def delete_payment_method(self, **kwargs) -> requests.Response:
         """
         Deletes a member payment method
-        Calls "DELETE /members/{id}/payment-method"
-        Documentation: https://fabman.io/api/v1/documentation#/members/deleteMembersIdPaymentMethod
+        
+        :calls: "DELETE /members/{id}/payment-method" \
+		<https://fabman.io/api/v1/documentation#/members/deleteMembersIdPaymentmethod>
+  
+        :returns: Response information of delete call
+        :rtype: requests.Response
         """
         return self._requester.request(
             "DELETE",
             f"/members/{self.id}/payment-method",
             _kwargs=kwargs,
         )
 
     def delete_training(self, training_id: int, **kwargs) -> requests.Response:
         """
         Deletes a member training given training ID
-        Calls "DELETE /members/{id}/trainings/{trainingId}"
-        Documentation: https://fabman.io/api/v1/documentation#/members/deleteMembersIdTrainingsTrainingId
+        
+        :calls: "DELETE /members/{id}/trainings/{trainingId}" \
+		<https://fabman.io/api/v1/documentation#/members/deleteMembersIdTrainingsTrainingid>
+
+        :param training_id: ID of the training to delete
+        :type training_id: int
+        :returns: Response information of delete call
+        :rtype: requests.Response
         """
         return self._requester.request(
             "DELETE",
             f"/members/{self.id}/trainings/{training_id}",
             _kwargs=kwargs,
         )
 
     def get_balance_items(self, **kwargs) -> requests.Response:
         """
         Retrieves the balance items of a member
-        calls "GET /members/{id}/balance-items"
-        Documentation: https://fabman.io/api/v1/documentation#/members/getMembersIdBalanceitems
+        
+        :calls: "GET /members/{id}/balance-items" \
+		<https://fabman.io/api/v1/documentation#/members/getMembersIdBalanceitems>
+  
+        :returns: Response information of get call
+        :rtype: requests.Response
         """
         response = self._requester.request(
             "GET",
             f"/members/{self.id}/balance-items",
             _kwargs=kwargs,
         )
 
         return response.json()
 
     def get_changes(self, **kwargs) -> requests.Response:
         """
         Retrieves the changes of a member
-        calls "GET /members/{id}/changes"
-        Documentation: https://fabman.io/api/v1/documentation#/members/getMembersIdChanges
+        
+        :calls: "GET /members/{id}/changes" \
+		<https://fabman.io/api/v1/documentation#/members/getMembersIdChanges>
+  
+        :returns: List of changes of a member
+        :rtype: list
         """
         response = self._requester.request(
             "GET",
             f"/members/{self.id}/changes",
             _kwargs=kwargs,
         )
 
         return response.json()
 
     def get_credits(self, **kwargs) -> PaginatedList:
         """
         Retrieves the credits of a member
-        calls "GET /members/{id}/credits"
-        Documentation: https://fabman.io/api/v1/documentation#/members/getMembersIdCredits
+        :calls: "GET /members/{id}/credits" \
+		<https://fabman.io/api/v1/documentation#/members/getMembersIdCredits>
+  
+        :returns: List of credits of a member
+        :rtype: fabman.paginated_list.PaginatedList
         """
         return PaginatedList(
             MemberCredit,
             self._requester,
             "GET",
             f"/members/{self.id}/credits",
             extra_attribs={"member_id": self.id},
             **kwargs,
         )
 
     def get_credit(self, credit_id: int, **kwargs) -> MemberCredit:
         """
         Retrieves a credit of a member
-        calls "GET /members/{id}/credits/{creditId}"
-        Documentation: https://fabman.io/api/v1/documentation#/members/getMembersIdCreditsCreditId
+        
+        :calls: "GET /members/{id}/credits/{creditId}" \
+		<https://fabman.io/api/v1/documentation#/members/getMembersIdCreditsCreditid>
+  
+        :param credit_id: ID of the credit to retrieve
+        :type credit_id: int
+        :returns: :code:`fabman.member.MemberCredit` object with credit details
+        :rtype: fabman.member.MemberCredit
         """
         response = self._requester.request(
             "GET",
             f"/members/{self.id}/credits/{credit_id}",
             _kwargs=kwargs,
         )
 
@@ -323,16 +397,20 @@
         data.update({"member_id": self.id})
 
         return MemberCredit(self._requester, data)
 
     def get_device(self, **kwargs) -> requests.Response:
         """
         Retrieves the device of a member used to authenticate on a bridge.
-        calls "GET /members/{id}/devices"
-        Documentation: https://fabman.io/api/v1/documentation#/members/getMembersIdDevice
+        
+        :calls: "GET /members/{id}/devices" \
+		<https://fabman.io/api/v1/documentation#/members/getMembersIdDevice>
+  
+        :returns: Device information
+        :rtype: dict
         """
         if "device" in self._embedded:
             return self._embedded["device"]
 
         response = self._requester.request(
             "GET",
             f"/members/{self.id}/device",
@@ -340,84 +418,108 @@
         )
 
         return response.json()
 
     def get_device_changes(self, **kwargs) -> requests.Response:
         """
         Retrieves the device changes of a member
-        calls "GET /members/{id}/device/changes"
-        Documentation: https://fabman.io/api/v1/documentation#/members/getMembersIdDeviceChanges
+        
+        :calls: "GET /members/{id}/device/changes" \
+		<https://fabman.io/api/v1/documentation#/members/getMembersIdDeviceChanges>
+
+        :returns: List of device changes of a member
+        :rtype: list
         """
         response = self._requester.request(
             "GET",
             f"/members/{self.id}/device/changes",
             _kwargs=kwargs,
         )
 
         return response.json()
 
     def get_device_change(self, change_id: int, **kwargs) -> requests.Response:
         """
         Retrieves a device change of a member given the change ID
-        calls "GET /members/{id}/device/changes/{changeId}"
-        Documentation: https://fabman.io/api/v1/documentation#/members/getMembersIdDeviceChangesChangeId
+        
+        :calls: "GET /members/{id}/device/changes/{changeId}" \
+		<https://fabman.io/api/v1/documentation#/members/getMembersIdDeviceChangesChangeId>
+  
+        :param change_id: ID of the change to retrieve
+        :type change_id: int
+        :returns: Device change information
+        :rtype: dict
         """
         response = self._requester.request(
             "GET",
             f"/members/{self.id}/device/changes/{change_id}",
             _kwargs=kwargs,
         )
 
         return response.json()
 
     def get_export(self, **kwargs) -> requests.Response:
         """
-        Retrieves the export of a member
-        calls "GET /members/{id}/export"
-        Documentation: https://fabman.io/api/v1/documentation#/members/getMembersIdExport
+        Retrieves the export of a member. This is a placeholder for future functionality.
+        
+        :calls: "GET /members/{id}/export" \
+		<https://fabman.io/api/v1/documentation#/members/getMembersIdExport>
+  
+        :raises: NotImplementedError
         """
         raise NotImplementedError("get_export not implemented yet")
 
     def get_invitation(self, **kwargs) -> requests.Response:
         """
         Retrieves the invitation status of a member
-        calls "GET /members/{id}/invitations"
-        Documentation: https://fabman.io/api/v1/documentation#/members/getMembersIdInvitation
+        
+        :calls: "GET /members/{id}/invitations" \
+		<https://fabman.io/api/v1/documentation#/members/getMembersIdInvitation>
+  
+        :returns: Invitation status of a member
+        :rtype: dict
         """
         response = self._requester.request(
             "GET",
             f"/members/{self.id}/invitation",
             _kwargs=kwargs,
         )
 
         return response.json()
 
-    def get_key(self, **kwargs):
+    def get_key(self, **kwargs) -> MemberKey:
         """
         Retrieves the keycard number of a member
-        calls "GET /members/{id}/key"
-        Documentation: https://fabman.io/api/v1/documentation#/members/getMembersIdKey
+        
+        :calls: "GET /members/{id}/key" \
+		<https://fabman.io/api/v1/documentation#/members/getMembersIdKey>
+  
+        :returns: :code:`fabman.member.MemberKey` object with key details
+        :rtype: fabman.member.MemberKey
         """
         if "key" in self._embedded:
-            return self._embedded["key"]
+            return MemberKey(self._requester, self._embedded["key"])
 
         response = self._requester.request(
             "GET",
             f"/members/{self.id}/key",
             _kwargs=kwargs,
         )
 
         return MemberKey(self._requester, response.json())
 
     def get_packages(self, **kwargs) -> Union[list, PaginatedList]:
         """
         Retrieves the packages of a member
 
-        calls "GET /members/{id}/packages"
-        Documentation: https://fabman.io/api/v1/documentation#/members/getMembersIdPackages
+        :calls: "GET /members/{id}/packages" \
+		<https://fabman.io/api/v1/documentation#/members/getMembersIdPackages>
+  
+        :returns: List of packages of a member
+        :rtype: fabman.paginated_list.PaginatedList
         """
         if "memberPackages" in self._embedded:
             out = []
             for package in self._embedded["memberPackages"]:
                 package.update({"member_id": self.id})
                 out.append(MemberPackage(self._requester, package))
             return out
@@ -430,21 +532,27 @@
             extra_attribs={"member_id": self.id},
             **kwargs,
         )
 
     def get_package(self, member_package_id: int, **kwargs) -> MemberPackage:
         """
         Retrieves a package of a member
-        calls "GET /members/{id}/packages/{memberPackageId}"
-        Documentation: https://fabman.io/api/v1/documentation#/members/getMembersIdPackagesMemberPackageId
+        
+        :calls: "GET /members/{id}/packages/{memberPackageId}" \
+		<https://fabman.io/api/v1/documentation#/members/getMembersIdPackagesMemberpackageid>
+  
+        :param member_package_id: ID of the package to retrieve
+        :type member_package_id: int
+        :returns: :code:`fabman.member.MemberPackage` object with package details
+        :rtype: fabman.member.MemberPackage
         """
         if "memberPackages" in self._embedded:
             for package in self._embedded["memberPackages"]:
                 if package["id"] == member_package_id:
-                    return package
+                    return MemberPackage(self._requester, package)
 
         response = self._requester.request(
             "GET",
             f"/members/{self.id}/packages/{member_package_id}",
             _kwargs=kwargs,
         )
 
@@ -452,58 +560,72 @@
         data.update({"member_id": self.id})
 
         return MemberPackage(self._requester, data)
 
     def get_payment_account(self, **kwargs) -> requests.Response:
         """
         Retrieves the payment account of a member
-        calls "GET /members/{id}/payment-account"
-        Documentation: https://fabman.io/api/v1/documentation#/members/getMembersIdPaymentAccount
+        
+        :calls: "GET /members/{id}/payment-account" \
+		<https://fabman.io/api/v1/documentation#/members/getMembersIdPaymentaccount>
+  
+        :returns: Payment account information
+        :rtype: dict
         """
         response = self._requester.request(
             "GET",
             f"/members/{self.id}/payment-account",
             _kwargs=kwargs,
         )
 
         return response.json()
 
     def get_payment_method(self, **kwargs) -> requests.Response:
         """
         Retrieves the payment method of a member
-        calls "GET /members/{id}/payment-method"
-        Documentation: https://fabman.io/api/v1/documentation#/members/getMembersIdPaymentMethod
+        :calls: "GET /members/{id}/payment-method" \
+		<https://fabman.io/api/v1/documentation#/members/getMembersIdPaymentmethod>
+  
+        :returns: Payment method information
+        :rtype: dict
         """
         response = self._requester.request(
             "GET",
             f"/members/{self.id}/payment-method",
             _kwargs=kwargs,
         )
 
         return response.json()
 
     def get_payment_method_mandate_preview(self, **kwargs) -> requests.Response:
         """
         Retrieves the payment method mandate preview of a member
-        calls "GET /members/{id}/payment-method-mandate-preview"
-        Documentation: https://fabman.io/api/v1/documentation#/members/getMembersIdPaymentMethodMandatePreview
+        
+        :calls: "GET /members/{id}/payment-method-mandate-preview" \
+		<https://fabman.io/api/v1/documentation#/members/getMembersIdPaymentmethodmandatepreview>
+  
+        :returns: Payment method mandate preview information
+        :rtype: dict
         """
         response = self._requester.request(
             "GET",
             f"/members/{self.id}/payment-method-mandate-preview",
             _kwargs=kwargs,
         )
 
         return response.json()
 
     def get_privileges(self, **kwargs) -> requests.Response:
         """
         Retrieves the privileges of a member
-        calls "GET /members/{id}/privileges"
-        Documentation: https://fabman.io/api/v1/documentation#/members/getMembersIdPrivileges
+        :calls: "GET /members/{id}/privileges" \
+		<https://fabman.io/api/v1/documentation#/members/getMembersIdPrivileges>
+  
+        :returns: privileges of a member
+        :rtype: dict
         """
         if "privileges" in self._embedded:
             return self._embedded["privileges"]
 
         response = self._requester.request(
             "GET",
             f"/members/{self.id}/privileges",
@@ -511,47 +633,61 @@
         )
 
         return response.json()
 
     def get_trained_resources(self, **kwargs) -> requests.Response:
         """
         Retrieves the trained resources of a member
-        calls "GET /members/{id}/trained-resources"
-        Documentation: https://fabman.io/api/v1/documentation#/members/getMembersIdTrainedResources
+        :calls: "GET /members/{id}/trained-resources" \
+		<https://fabman.io/api/v1/documentation#/members/getMembersIdTrainedResources>
+  
+        :return: Trained resources of a member
+        :rtype: list
         """
         response = self._requester.request(
             "GET",
             f"/members/{self.id}/trained-resources",
             _kwargs=kwargs,
         )
 
         return response.json()
 
     def get_trainings(self, **kwargs) -> requests.Response:
         """
+        TODO: Move to MemberTrainings object
+        
         Retrieves the trainings of a member
-        calls "GET /members/{id}/trainings"
-        Documentation: https://fabman.io/api/v1/documentation#/members/getMembersIdTrainings
+        :calls: "GET /members/{id}/trainings" \
+		<https://fabman.io/api/v1/documentation#/members/getMembersIdTrainings>
+
+        :return: List of trainings of a member
+        :rtype: list
         """
         if "trainings" in self._embedded:
             return self._embedded["trainings"]
 
         response = self._requester.request(
             "GET",
             f"/members/{self.id}/trainings",
             _kwargs=kwargs,
         )
 
         return response.json()
 
     def get_training(self, training_id: int, **kwargs) -> requests.Response:
         """
+        TODO: Move this to MemberTraining Object
         Retrieves a training of a member
-        calls "GET /members/{id}/trainings/{trainingId}"
-        Documentation: https://fabman.io/api/v1/documentation#/members/getMembersIdTrainingsTrainingId
+        :calls: "GET /members/{id}/trainings/{trainingId}" \
+		<https://fabman.io/api/v1/documentation#/members/getMembersIdTrainingstrainingid>
+        
+        :param training_id: ID of the training to retrieve
+        :type training_id: int
+        :return: Training information
+        :rtype: dict
         """
         if "trainings" in self._embedded:
             for training in self._embedded["trainings"]:
                 if training["id"] == training_id:
                     return training
 
         response = self._requester.request(
@@ -563,32 +699,38 @@
         return response.json()
 
     def refresh(self) -> None:
         """
         Updates the objects with more recent data from the API. Needs to be called
         when update() fails for lockVersioning.
 
-        Calls "GET /members/{id}"
-        Documentation https://fabman.io/api/v1/documentation#/members/getMembersId
+        :calls: "GET /members/{id}" \
+		<https://fabman.io/api/v1/documentation#/members/getMembersId>
+  
+        :returns: None -- updates attributes of the current object
+        :rtype: None
         """
 
         response = self._requester.request("GET", f"/members/{self.id}")
 
         data = response.json()
 
         for attr, val in data.items():
             setattr(self, attr, val)
 
     def update(self, **kwargs) -> None:
         """
         Updates the member object and sets the modified attributes based on what
         is returned by the server.  Member object is updated in place.
 
-        calls "PUT /members/{id}"
-        Documentation: https://fabman.io/api/v1/documentation#/members/putMembersId
+        :calls: "PUT /members/{id}" \
+		<https://fabman.io/api/v1/documentation#/members/putMembersId>
+  
+        :returns: None -- updates attributes of the current object
+        :rtype: None
         """
 
         kwargs.update({"lockVersion": self.lockVersion})
 
         response = self._requester.request(
             "PUT",
             f"/members/{self.id}",
```

### Comparing `fabman-1.1.17/fabman/package.py` & `fabman-1.1.20/fabman/package.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,30 +12,36 @@
     def __str__(self):
         return f"PackageCredit #{self.id}, Package #{self.package_id}: {self.scope}"
 
     def delete(self, **kwargs) -> requests.Response:
         """
         Deletes a credit from a package. *WARNING: This is irreversible.*
 
-        Calls "DELETE /packages/{packageId}/credits/{creditId}"
-        Documentation https://fabman.io/api/v1/documentation#/packages/deletePackagesPackageIdCreditsCreditId
+        :calls: "DELETE /packages/{packageId}/credits/{creditId}" \
+		<https://fabman.io/api/v1/documentation#/packages/deletePackagesIdCreditsCreditid>
+  
+        :returns: response information of call
+        :rtype: requests.Response
         """
 
         uri = f"/packages/{self.package_id}/credits/{self.id}"
 
         response = self._requester.request("DELETE", uri, _kwargs=kwargs)
 
         return response
 
     def update(self, **kwargs) -> None:
         """
         Updates the credit. Attributes are updated in place with new information.
 
-        Calls "PUT /packages/{packageId}/credits/{creditId}"
-        Documentation https://fabman.io/api/v1/documentation#/packages/putPackagesPackageIdCreditsCreditId
+        :calls: "PUT /packages/{packageId}/credits/{creditId}" \
+		<https://fabman.io/api/v1/documentation#/packages/putPackagesIdCreditsCreditid>
+
+        :return: None -- attributes are updated in place
+        :rtype: None
         """
 
         uri = f"/packages/{self.package_id}/credits/{self.id}"
 
         kwargs.update({"lockVersion": self.lockVersion})
         response = self._requester.request("PUT", uri, _kwargs=kwargs)
 
@@ -51,30 +57,36 @@
     def __str__(self):
         return f"PackagePermission #{self.id}, Package #{self.package_id}: {self.type}"
 
     def delete(self, **kwargs) -> requests.Response:
         """
         Deletes a permission from a package. *WARNING: This is irreversible.*
 
-        Calls "DELETE /packages/{packageId}/permissions/{permissionId}"
-        Documentation https://fabman.io/api/v1/documentation#/packages/deletePackagesPackageIdPermissionsPermissionId
+        :calls: "DELETE /packages/{packageId}/permissions/{permissionId}" \
+		<https://fabman.io/api/v1/documentation#/packages/deletePackagesIdPermissionsPermissionid>
+
+        :return: response information of call
+        :rtype: requests.Response
         """
 
         uri = f"/packages/{self.package_id}/permissions/{self.id}"
 
         response = self._requester.request("DELETE", uri, _kwargs=kwargs)
 
         return response
 
     def update(self, **kwargs) -> None:
         """
         Updates the permission. Attributes are updated in place with new information.
 
-        Calls "PUT /packages/{packageId}/permissions/{permissionId}"
-        Documentation https://fabman.io/api/v1/documentation#/packages/putPackagesPackageIdPermissionsPermissionId
+        :calls: "PUT /packages/{packageId}/permissions/{permissionId}" \
+		<https://fabman.io/api/v1/documentation#/packages/putPackagesIdPermissionsPermissionid>
+  
+        :return: None -- attributes are updated in place
+        :rtype: None
         """
 
         uri = f"/packages/{self.package_id}/permissions/{self.id}"
 
         kwargs.update({"lockVersion": self.lockVersion})
         response = self._requester.request("PUT", uri, _kwargs=kwargs)
 
@@ -90,32 +102,38 @@
     def __str__(self):
         return f"Package #{self.id}: {self.name}"
 
     def create_credit(self, **kwargs) -> PackageCredit:
         """
         Create a credit for this package. Takes no arguments.
 
-        Calls "POST /packages/{id}/credits"
-        Documentation: https://fabman.io/api/v1/documentation#/packages/postPackagesIdCredits
+        :calls: "POST /packages/{id}/credits" \
+		<https://fabman.io/api/v1/documentation#/packages/postPackagesIdCredits>
+
+        :return: Object with information and methods of the new credit
+        :rtype: fabman.package.PackageCredit
         """
 
         uri = f"/packages/{self.id}/credits"
         response = self._requester.request("POST", uri, _kwargs=kwargs)
 
         data = response.json()
         data.update({"package_id": self.id})
 
         return PackageCredit(self._requester, data)
 
     def create_permission(self, **kwargs) -> PackagePermission:
         """
         Create a new permission for this package. Gives new abilities to package hodlers.
 
-        Calls "POST /packages/{id}/permissions"
-        Documentation: https://fabman.io/api/v1/documentation#/packages/postPackagesIdPermissions
+        :calls: "POST /packages/{id}/permissions" \
+		<https://fabman.io/api/v1/documentation#/packages/postPackagesIdPermissions>
+  
+        :return: Object with information and methods of the new permission
+        :rtype: fabman.package.PackagePermission
         """
 
         uri = f"/packages/{self.id}/permissions"
 
         response = self._requester.request("POST", uri, _kwargs=kwargs)
 
         data = response.json()
@@ -123,16 +141,21 @@
 
         return PackagePermission(self._requester, data)
 
     def get_credit(self, credit_id, **kwargs) -> PackageCredit:
         """
         Return a credit for this package given a credit_id.
 
-        Calls "GET /packages/{id}/credits/{creditId}"
-        Documentation: https://fabman.io/api/v1/documentation#/packages/getPackagesIdCreditsCreditId
+        :calls: "GET /packages/{id}/credits/{creditId}" \
+		<https://fabman.io/api/v1/documentation#/packages/getPackagesIdCreditsCreditid>
+
+        :param credit_id: ID of the credit to retrieve
+        :type credit_id: int
+        :return: Object with information and methods of the credit
+        :rtype: fabman.package.PackageCredit
         """
 
         uri = f"/packages/{self.id}/credits/{credit_id}"
         response = self._requester.request("GET", uri, _kwargs=kwargs)
 
         data = response.json()
         data.update({"package_id": self.id})
@@ -141,14 +164,17 @@
 
     def get_credits(self, **kwargs) -> PaginatedList:
         """
         Return a PaginatedList of credits for this package
 
         Calls: "GET /packages/{id}/credits"
         Documentation: https://fabman.io/api/v1/documentation#/packages/getPackagesIdCredits
+
+        :return: List of credits for this package
+        :rtype: fabman.paginated_list.PaginatedList
         """
 
         return PaginatedList(
             PackageCredit,
             self._requester,
             "GET",
             f"/packages/{self.id}/credits",
@@ -156,31 +182,37 @@
             kwargs=kwargs,
         )
 
     def get_permission(self, permission_id, **kwargs) -> PackagePermission:
         """
         Return a permission for this package given a permission_id.
 
-        Calls "GET /packages/{id}/permissions/{permissionId}"
-        Documentation: https://fabman.io/api/v1/documentation#/packages/getPackagesIdPermissionsPermissionId
+        :calls: "GET /packages/{id}/permissions/{permissionId}" \
+		<https://fabman.io/api/v1/documentation#/packages/getPackagesIdPermissionsPermissionid>
+  
+        :returns: Object with information and methods of the permission
+        :rtype: fabman.package.PackagePermission
         """
         uri = f"/packages/{self.id}/permissions/{permission_id}"
         response = self._requester.request("GET", uri, _kwargs=kwargs)
 
         data = response.json()
         data.update({"package_id": self.id})
 
         return PackagePermission(self._requester, data)
 
     def get_permissions(self, **kwargs) -> PaginatedList:
         """
         Return a PaginatedList of permissions for the package.
 
-        Calls "GET /packages/{id}/permissions"
-        Documentation: https://fabman.io/api/v1/documentation#/packages/getPackagesIdPermissions
+        :calls: "GET /packages/{id}/permissions" \
+		<https://fabman.io/api/v1/documentation#/packages/getPackagesIdPermissions>
+
+        :returns: List of permissions for the package
+        :rtype: fabman.paginated_list.PaginatedList
         """
 
         return PaginatedList(
             PackagePermission,
             self._requester,
             "GET",
             f"/packages/{self.id}/permissions",
@@ -188,31 +220,37 @@
             kwargs=kwargs,
         )
 
     def delete(self, **kwargs) -> requests.Response:
         """
         Deletes the package. Takes no arguments. **WARNINGL: This is irreversible.**
 
-        Calls "DELETE /packages/{id}"
-        Documentation https://fabman.io/api/v1/documentation#/packages/deletePackagesId
+        :calls: "DELETE /packages/{id}" \
+		<https://fabman.io/api/v1/documentation#/packages/deletePackagesId>
+  
+        :returns: response information of call
+        :rtype: requests.Response
         """
 
         uri = f"/packages/{self.id}"
 
         response = self._requester.request("DELETE", uri, _kwargs=kwargs)
 
         return response
 
     def update(self, **kwargs) -> None:
         """
         Update information on the package. Note that many fields may be unalterable
         by the API key holder.
 
-        Calls "PUT /packages/{id}"
-        Documentation: https://fabman.io/api/v1/documentation#/packages/putPackagesId
+        :calls: "PUT /packages/{id}" \
+		<https://fabman.io/api/v1/documentation#/packages/putPackagesId>
+  
+        :return: None -- attributes are updated in place
+        :rtype: None
         """
 
         uri = f"/packages/{self.id}"
 
         kwargs.update({"lockVersion": self.lockVersion})
 
         response = self._requester.request("PUT", uri, _kwargs=kwargs)
```

### Comparing `fabman-1.1.17/fabman/paginated_list.py` & `fabman-1.1.20/fabman/paginated_list.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.17/fabman/payment.py` & `fabman-1.1.20/fabman/webhook.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,89 @@
-"""Defines the Payment object"""
+"""Defines the Webhook class"""
 
 import requests
 
 from fabman.fabman_object import FabmanObject
 
 
-class Payment(FabmanObject):
-    """Defines the Payment object for interacting with payments on the Fabman API"""
+class Webhook(FabmanObject):
+    """
+    Class for interacting with the webhooks endpoint on the Fabman API
+    """
 
-    def __str__(self) -> str:
-        return f"Payment #{self.id}: {self.notes}"
+    def __str__(self):
+        return f"Webhook #{self.id}: {self.label}"
 
-    def delete(self, **kwargs) -> requests.Response:
+    def delete(self, **kwargs):
         """
-        Deletes a payment. *WARNING: This is irreversible.*
+        Deletes a webhook. *WARNING: This is irreversible.*
 
-        Calls "DELETE /payments/{id}"
-        Documentation: https://fabman.io/api/v1/documentation#/payments/deletePaymentsId
+        :calls: "DELETE /webhooks/{webhookId}" \
+		<https://fabman.io/api/v1/documentation#/webhooks/deleteWebhooksId>
+  
+        :return: response information of call
+        :rtype: requests.Response
         """
-        uri = f"/payments/{self.id}"
+
+        uri = f"/webhooks/{self.id}"
 
         response = self._requester.request("DELETE", uri, _kwargs=kwargs)
 
         return response
 
-    def request_payment(self, **kwargs) -> requests.Response:
+    def get_events(self, **kwargs) -> requests.Response:
+        """
+        Returns the events for a webhook.
+
+        :calls: "GET /webhooks/{webhookId}/events" \
+		<https://fabman.io/api/v1/documentation#/webhooks/getWebhooksIdEvents>
+  
+        :return: response information of call
+        :rtype: requests.Response
+        """
+
+        if "events" in self._embedded:
+            return self._embedded["events"]
+
+        uri = f"/webhooks/{self.id}/events"
+
+        response = self._requester.request("GET", uri, _kwargs=kwargs)
+
+        return response
+
+    def send_test_event(self, **kwargs) -> requests.Response:
         """
-        Requests a payment from the customer.
+        Sends a test event to the webhook.
 
-        Calls "POST /payments/{id}/request-payment"
-        Documentation: https://fabman.io/api/v1/documentation#/payments/postPaymentsIdRequestPayment
+        :calls: "POST /webhooks/{webhookId}/events" \
+		<https://fabman.io/api/v1/documentation#/webhooks/postWebhooksIdTest>
+  
+        :return: response information of call
+        :rtype: requests.Response
         """
-        uri = f"/payments/{self.id}/request-payment"
+
+        uri = f"/webhooks/{self.id}/test"
 
         response = self._requester.request("POST", uri, _kwargs=kwargs)
 
         return response
 
     def update(self, **kwargs) -> None:
         """
-        Updates a payment. Attributes are modified in place using updated information
-        from the API.
+        Updates the webhook. Attributes are updated in place with new information
 
-        Calls "PUT /payments/{id}"
-        Documentation: https://fabman.io/api/v1/documentation#/payments/putPaymentsId
+        :calls: "PUT /webhooks/{webhookId}" \
+		<https://fabman.io/api/v1/documentation#/webhooks/putWebhooksId>
+  
+        :return: None -- attributes are updated in place
+        :rtype: None
         """
 
-        uri = f"/payments/{self.id}"
+        uri = f"/webhooks/{self.id}"
 
         kwargs.update({"lockVersion": self.lockVersion})
-
         response = self._requester.request("PUT", uri, _kwargs=kwargs)
 
         data = response.json()
 
         for attr, val in data.items():
             setattr(self, attr, val)
```

### Comparing `fabman-1.1.17/fabman/requester.py` & `fabman-1.1.20/fabman/requester.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,83 +31,58 @@
 class Requester(object):
     """Main class responsible for handling all http requests to the API.
     Based on canvasapi.requester.Requester found at
     https://github.com/ucfopen/canvasapi/blob/develop/canvasapi/requester.py
     """
 
     def __init__(self, base_url: str, access_token: str) -> None:
-        """_summary_
-
-        Args:
-            base_url (str): The base url of Fabman API. Should simply https://api.fabman.io/v1
-            access_token (_type_): Access token to access the API
+        """
+        :param base_url: The base URL of the Fabman instance's API.
+        :type base_url: str
+        :param access_token: The API key to authenticate requests with.
+        :type access_token: str
         """
 
         self.base_url = base_url
         self.__access_token = access_token
         self.__session = requests.Session()
         self.__cache = []
 
     def _delete_request(
         self, url: str, headers: dict, data: Optional[dict] = None, **kwargs
     ) -> requests.Response:
-        """Handles a delete request to the API. Should never be called directly
-
-        Args:
-            url (str): url for the request
-            headers (dict): dictionary of headers
-            data (_type_, optional): data as part of the delete requests. Defaults to None.
-
-        Returns:
-            requests.Response
+        """
+        Handles a delete request to the API. Should never be called directly
         """
 
         return self.__session.delete(url, headers=headers, data=data, **kwargs)
 
     def _get_request(
         self, url: str, headers: dict, params: Optional[dict] = None, **kwargs
     ) -> requests.Response:
-        """Handles a get request to the API. Should never be called directly
-
-        Args:
-            url (str): url for the request
-            headers (dict): dictionary of headers
-            params (List, optional): dictionary of parameters. Defaults to None.
-        Returns:
-
-            requests.Response
+        """
+        Handles a get request to the API. Should never be called directly
         """
 
         return self.__session.get(url, headers=headers, params=params, **kwargs)
 
     def _post_request(
         self, url: str, headers: dict, data: Optional[dict] = None, **kwargs
     ) -> requests.Response:
-        """Handles a post request to the API. Should never be called directly
-
-        Args:
-            url (str): url for the request
-            headers (dict): dictionary of headers
-            data (dict, optional): dictionary of data. Defaults to None.
-
-        Returns:
-            requests.Response
+        """
+        Handles a post request to the API. Should never be called directly
         """
 
         return self.__session.post(url, headers=headers, data=data, **kwargs)
 
     def _put_request(
         self, url: str, headers: dict, data: Optional[dict] = None, **kwargs
     ) -> requests.Response:
-        """Handles a put request to the API. Should never be called directly
-
-        Args:
-            url (str): url for the request
-            headers (dict): dictionary of headers
-            data (dict, optional): dictionary of data. Defaults to None.
+        """
+        Handles a put request to the API. Should never be called directly
         """
 
         return self.__session.put(url, headers=headers, data=data, **kwargs)
 
     def request(
         self,
         method: str,
@@ -115,43 +90,35 @@
         headers: Optional[dict] = None,
         use_auth: Optional[bool] = True,
         _url: Optional[str] = None,
         _kwargs: Optional[dict] = None,
         json: Optional[bool] = False,
         **kwargs,
     ) -> requests.Response:
-        """Main method for handling requests to the API. Should never be called directly except for
+        """
+        Main method for handling requests to the API. Should never be called directly except for
         testing or from the Fabman class.
 
-        Args:
-            method (str): Method to be declared. Should be one of GET, POST, PUT, PATCH, DELETE
-            endpoint (Optional[str], optional): Endpoint of the api to call. Defaults to None.
-            headers (Optional[dict], optional): Any special headers to be added to the request.
-            Authorization headers are automatically handled. Defaults to None.
-            use_auth (Optional[bool], optional): Should the api call use authorization? Should be
-            true in almost any case. Defaults to True.
-            _url (Optional[str], optional): URL to call, should be None in most cases. Defaults
-            to None.
-            _kwargs (Optional[List], optional): Any special kwargs to use inside of the call.
-            Defaults to None.
-            json (Optional[bool], optional): Sending dict or json? Defaults to False.
-
-        Raises:
-            ValueError
-            BadRequest
-            InvalidAccessToken
-            Unauthorized
-            ForbiddenError
-            ResourceDoesNotExist
-            Conflict
-            UnprocessableEntity
-            FabmanException
+        :param method: The HTTP method to use for the request.
+        :type method: str
+        :param endpoint: The API endpoint to call.
+        :type endpoint: str
+        :param headers: HTTP headers to send with the request.
+        :type headers: dict
+        :param use_auth: Whether or not to include the access token in the request.
+        :type use_auth: bool
+        :param _url: The full URL to use for the request. This overrides the base_url and endpoint.
+        :type _url: str
+        :param _kwargs: Keyword arguments from the calling argument. These are morphed into the params or body of the request depending on :code:`method`.
+        :type _kwargs: dict
+        :param json: Whether or not to send the data as JSON.
+        :type json: bool
 
-        Returns:
-            _type_: _description_
+        :return: The response object if the call was successful
+        :rtype: requests.Response
         """
         full_url = _url if _url else f"{self.base_url}{endpoint}"
 
         if not headers:
             headers = {}
 
         if use_auth:
```

### Comparing `fabman-1.1.17/fabman/resource.py` & `fabman-1.1.20/fabman/resource.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,16 +13,19 @@
         return f"Resource #{self.resource_id}: {self.serialNumber}"
 
     def update(self, **kwargs) -> None:
         """
         Update the bridge object on the server. Returns the updated bridge object.
         Updates all information in place.
 
-        Calls "PUT /resources/{resource_id}/bridge"
-        Documentation: https://fabman.io/api/v1/documentation#/resources/putResourcesIdBridge
+        :calls: "PUT /resources/{resource_id}/bridge" \
+		<https://fabman.io/api/v1/documentation#/resources/putResourcesIdBridge>
+  
+        :return: None -- attributes are updated in place
+        :rtype: None
         """
         uri = f"/resources/{self.resource_id}/bridge"
 
         response = self._requester.request("PUT", uri, _kwargs=kwargs)
 
         data = response.json()
 
@@ -40,44 +43,54 @@
         return f"Resource #{self.id}: {self.name}"
 
     def delete_bridge(self, **kwargs) -> requests.Response:
         """
         Delete the bridge that is currently connected to this resource. If no bridge
         is currently connected, this will do nothing.
 
-        Calls "DELETE /resources/{id}/bridge"
-        Documentation: https://fabman.io/api/v1/documentation#/resources/deleteResourcesIdBridge
+        :calls: "DELETE /resources/{id}/bridge" \
+		<https://fabman.io/api/v1/documentation#/resources/deleteResourcesIdBridge>
+  
+        :return: response information of call
+        :rtype: requests.Response
         """
         uri = f"/resources/{self.id}/bridge"
 
         response = self._requester.request("DELETE", uri, _kwargs=kwargs)
 
         return response
 
     def delete(self, **kwargs) -> requests.Response:
         """
         Deletes the resource. *WARNING: THIS CANNOT BE UNDONE.* All future API
         calls from this resource will fail.
 
-        Calls "DELETE /resources/{id}"
-        Documentation: https://fabman.io/api/v1/documentation#/resources/deleteResourcesId
+        :calls: "DELETE /resources/{id}" \
+		<https://fabman.io/api/v1/documentation#/resources/deleteResourcesId>
+  
+        :return: response information of call
+        :rtype: requests.Response
         """
         uri = f"/resources/{self.id}"
 
         response = self._requester.request("DELETE", uri, _kwargs=kwargs)
 
         return response
 
     def get_bridge(self, **kwargs) -> ResourceBridge:
         """
         Get the bridge that is currently connected to this resource. If no bridge is
         connected, this will return an empty list.
 
-        Calls "GET /resources/{id}/bridge"
-        Documentation: https://fabman.io/api/v1/documentation#/resources/getResourcesIdBridge
+        :calls: "GET /resources/{id}/bridge" \
+		<https://fabman.io/api/v1/documentation#/resources/getResourcesIdBridge>
+  
+        :return: ResourceBridge object with information on the bridge
+        :rtype: fabman.resource.ResourceBridge
+        
         """
         uri = f"/resources/{self.id}/bridge"
 
         response = self._requester.request("GET", uri, _kwargs=kwargs)
 
         data = response.json()
         data.update({"resource_id": self.id})
@@ -86,43 +99,52 @@
 
     def get_bridge_api_key(self, **kwargs) -> requests.Response:
         """
         Get the API key for the bridge that is currently connected to this resource.
         For most users, this will return a 204 code with an empty body. Only superusers
         or users who have created a custom bridge should be able to access this endpoint.
 
-        Calls "GET /resources/{id}/bridge/api-key"
-        Documentation: https://fabman.io/api/v1/documentation#/resources/getResourcesIdBridgeApiKey
+        :calls: "GET /resources/{id}/bridge/api-key" \
+		<https://fabman.io/api/v1/documentation#/resources/getResourcesIdBridgeApikey>
+
+        :return: response information of call
+        :rtype: dict
         """
         uri = f"/resources/{self.id}/bridge/api-key"
 
         response = self._requester.request("GET", uri, _kwargs=kwargs)
 
         return response.json()
 
     def switch_on(self, **kwargs) -> requests.Response:
         """
         Switch on the resource. Requires "code" field to be in the data packet.
         Does not seem to work without the proper code, which is undocumented.
 
-        Calls "POST /resources/{id}/switch-on"
-        Documentation: https://fabman.io/api/v1/documentation#/resources/postResourcesIdSwitchOn
+        :calls: "POST /resources/{id}/switch-on" \
+		<https://fabman.io/api/v1/documentation#/resources/postResourcesIdBridgeSwitchon>
+  
+        :return: response information of call
+        :rtype: requests.Response
         """
         uri = f"/resources/{self.id}/switch-on"
 
         response = self._requester.request("POST", uri, _kwargs=kwargs)
 
         return response
 
     def update(self, **kwargs) -> None:
         """
         Update the resource.
 
-        Calls "PUT /resources/{id}"
-        Documentation: https://fabman.io/api/v1/documentation#/resources/putResourcesId
+        :calls: "PUT /resources/{id}" \
+		<https://fabman.io/api/v1/documentation#/resources/putResourcesId>
+  
+        :return: None -- attributes are updated in place
+        :rtype: None
         """
         uri = f"/resources/{self.id}"
 
         kwargs.update({"lockVersion": self.lockVersion})
 
         response = self._requester.request("PUT", uri, _kwargs=kwargs)
```

### Comparing `fabman-1.1.17/fabman/resource_log.py` & `fabman-1.1.20/fabman/resource_log.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,31 +11,37 @@
     def __str__(self):
         return f"ResourceLog #{self.id}, Resource #{self.resource} - {self.type}"
 
     def delete(self, **kwargs) -> requests.Response:
         """
         Deletes a resource-log. *WARNING: This is irreversible.*
 
-        Calls "DELETE /resource-logs/{resourceLogId}"
-        Documentation https://fabman.io/api/v1/documentation#/resource-logs/deleteResourceLogsResourceLogId
+        :calls: "DELETE /resource-logs/{resourceLogId}" \
+		<https://fabman.io/api/v1/documentation#/resource-logs/deleteResourcelogsId>
+  
+        :return: response information of call
+        :rtype: requests.Response
         """
 
         uri = f"/resource-logs/{self.id}"
 
         response = self._requester.request("DELETE", uri, _kwargs=kwargs)
 
         return response
 
     def update(self, **kwargs) -> None:
         """
         Updates the resource-log. Attributes are updated in place with new information
         retrieved from the API.
 
-        Calls "PUT /resource-logs/{resourceLogId}"
-        Documentation https://fabman.io/api/v1/documentation#/resource-logs/putResourceLogsResourceLogId
+        :calls: "PUT /resource-logs/{resourceLogId}" \
+		<https://fabman.io/api/v1/documentation#/resource-logs/putResourcelogsId>
+  
+        :return: None -- attributes are updated in place
+        :rtype: None
         """
 
         uri = f"/resource-logs/{self.id}"
 
         kwargs.update({"lockVersion": self.lockVersion})
 
         response = self._requester.request("PUT", uri, _kwargs=kwargs)
```

### Comparing `fabman-1.1.17/fabman/resource_type.py` & `fabman-1.1.20/fabman/resource_type.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,31 +14,37 @@
     def delete(self, **kwargs) -> requests.Response:
         """
         Deletes a resource-type. *WARNING: This is irreversible and may have
         unintended consequences.* Resource Types are used to group resources and
         are therefore tied to all resources of that type. Be sure you know
         what you are doing when using this endpoint. There is no confirmation.
 
-        Calls "DELETE /resource-types/{resourceTypeId}"
-        Documentation https://fabman.io/api/v1/documentation#/resource-types/deleteResourceTypesResourceTypeId
+        :calls: "DELETE /resource-types/{resourceTypeId}" \
+		<https://fabman.io/api/v1/documentation#/resource-types/deleteResourcetypesId>
+  
+        :return: response information of call
+        :rtype: requests.Response
         """
 
         uri = f"/resource-types/{self.id}"
 
         response = self._requester.request("DELETE", uri, _kwargs=kwargs)
 
         return response
 
     def update(self, **kwargs) -> None:
         """
         Updates the resource-type. Attributes are updated in place with new information
         retrieved from the API.
 
-        Calls "PUT /resource-types/{resourceTypeId}"
-        Documentation https://fabman.io/api/v1/documentation#/resource-types/putResourceTypesResourceTypeId
+        :calls: "PUT /resource-types/{resourceTypeId}" \
+		<https://fabman.io/api/v1/documentation#/resource-types/putResourcetypesId>
+
+        :return: None -- attributes are updated in place
+        :rtype: None
         """
 
         uri = f"/resource-types/{self.id}"
 
         response = self._requester.request("PUT", uri, _kwargs=kwargs)
 
         data = response.json()
```

### Comparing `fabman-1.1.17/fabman/space.py` & `fabman-1.1.20/fabman/space.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,31 +14,37 @@
     def __str__(self):
         return f"SpaceBillingSettings for space #{self.space}"
 
     def delete_stripe(self, **kwargs) -> requests.Response:
         """
         Deletes Stripe information from a space. *WARNING: This is irreversible.*
 
-        Calls "DELETE /space/{id]/billing-settings/stripe"
-        Documentation https://fabman.io/api/v1/documentation#/spaces/deleteSpacesIdBillingsettingsStripe
+        :calls: "DELETE /space/{id]/billing-settings/stripe" \
+		<https://fabman.io/api/v1/documentation#/spaces/deleteSpacesIdBillingsettingsStripe>
+  
+        :return: response information of call
+        :rtype: requests.Response
         """
 
         uri = f"/spaces/{self.space_id}/billing-settings/stripe"
 
         response = self._requester.request("DELETE", uri, _kwargs=kwargs)
 
         return response
 
     def update(self, **kwargs) -> None:
         """
         Updates the space-billing-settings. Attributes are updated in place with new information
         retrieved from the API.
 
-        Calls "PUT /space-billing-settings/{spaceBillingSettingsId}"
-        Documentation https://fabman.io/api/v1/documentation#/space-billing-settings/putSpaceBillingSettingsSpaceBillingSettingsId
+        :calls: "PUT /space-billing-settings/{spaceBillingSettingsId}" \
+		<https://fabman.io/api/v1/documentation#/space-billing-settings/putSpaceBillingSettingsSpaceBillingSettingsId>
+  
+        :return: None -- attributes are updated in place
+        :rtype: None
         """
 
         uri = f"/spaces/{self.space_id}/billing-settings"
 
         kwargs.update({"lockVersion": self.lockVersion})
 
         response = self._requester.request("PUT", uri, _kwargs=kwargs)
@@ -47,18 +53,20 @@
 
         for attr, val in data.items():
             setattr(self, attr, val)
 
     def update_stripe(self, **kwargs) -> None:
         """
         Updates the space-billing-settings. Attributes are updated in place with new information
-        retrieved from the API.
+        retrieved from the API. Placeholder for future implementation
 
-        Calls "PUT /space-billing-settings/{spaceBillingSettingsId}"
-        Documentation https://fabman.io/api/v1/documentation
+        :calls: "PUT /space-billing-settings/{spaceBillingSettingsId}" \
+		<https://fabman.io/api/v1/documentation>
+  
+        :raises: NotImplementedError
         """
 
         raise NotImplementedError("This method is not yet implemented.")
 
 
 class SpaceHoliday(FabmanObject):
     """Class for interacting with the space/{id}/holidays endpoints on the Fabman API"""
@@ -66,32 +74,37 @@
     def __str__(self):
         return f"SpaceHoliday #{self.id}: {self.title}"
 
     def delete(self, **kwargs) -> requests.Response:
         """
         Deletes a space holiday. *WARNING: This is irreversible.*
 
-        Calls "DELETE /space/{spaceId}/holidays/{holidayId}"
-        Documentation https://fabman.io/api/v1/documentation#/spaces/deleteSpacesIdHolidaysHolidayid
+        :calls: "DELETE /space/{spaceId}/holidays/{holidayId}" \
+		<https://fabman.io/api/v1/documentation#/spaces/deleteSpacesIdHolidaysHolidayid>
+  
+        :return: response information of call
+        :rtype: requests.Response
         """
 
         uri = f"/spaces/{self.space_id}/holidays/{self.id}"
 
         response = self._requester.request("DELETE", uri, _kwargs=kwargs)
 
         return response
 
     def update(self, **kwargs) -> None:
         """
         Updates the space holiday. Attributes are updated in place with new information
         retrieved from the API.
 
-        Calls "PUT /space/{spaceId}/holidays/{holidayId}"
-        #/spaces/putSpacesIdHolidaysHolidayid
-        Documentation https://fabman.io/api/v1/documentation
+        :calls: "PUT /space/{spaceId}/holidays/{holidayId}" \
+		<https://fabman.io/api/v1/documentation#/spaces/putSpacesIdHolidaysHolidayid>
+  
+        :return: None -- attributes are updated in place
+        :rtype: None
         """
 
         uri = f"/spaces/{self.space_id}/holidays/{self.id}"
 
         kwargs.update({"lockVersion": self.lockVersion})
 
         response = self._requester.request("PUT", uri, _kwargs=kwargs)
@@ -108,58 +121,70 @@
     def __str__(self):
         return f"Space #{self.id}: {self.name}"
 
     def create_holiday(self, **kwargs) -> SpaceHoliday:
         """
         Creates a new holiday for the space.
 
-        Calls "POST /spaces/{spaceId}/holidays"
-        Documentation https://fabman.io/api/v1/documentation#/spaces/postSpacesIdHolidays
+        :calls: "POST /spaces/{spaceId}/holidays" \
+		<https://fabman.io/api/v1/documentation#/spaces/postSpacesIdHolidays>
+  
+        :return: Object with new holiday information
+        :rtype: fabman.space.SpaceHoliday
         """
 
         uri = f"/spaces/{self.id}/holidays"
 
         response = self._requester.request("POST", uri, _kwargs=kwargs)
 
         return SpaceHoliday(self._requester, response.json())
 
     def delete(self, **kwargs) -> requests.Response:
         """
         Deletes a space. *WARNING: This is irreversible.*
 
-        Calls "DELETE /spaces/{spaceId}"
-        Documentation https://fabman.io/api/v1/documentation#/spaces/deleteSpacesId
+        :calls: "DELETE /spaces/{spaceId}" \
+		<https://fabman.io/api/v1/documentation#/spaces/deleteSpacesId>
+
+        :return: response information of call
+        :rtype: requests.Response
         """
 
         uri = f"/spaces/{self.id}"
 
         response = self._requester.request("DELETE", uri, _kwargs=kwargs)
 
         return response
 
     def delete_calendar_token(self, **kwargs) -> requests.Response:
         """
         Deletes a space calendar token. *WARNING: This is irreversible.*
 
-        Calls "DELETE /spaces/{spaceId}/calendar-token"
-        Documentation https://fabman.io/api/v1/documentation#/spaces/deleteSpacesIdCalendartoken
+        :calls: "DELETE /spaces/{spaceId}/calendar-token" \
+		<https://fabman.io/api/v1/documentation#/spaces/deleteSpacesIdCalendartoken>
+  
+        :return: response information of call
+        :rtype: requests.Response
         """
 
         uri = f"/spaces/{self.id}/calendar-token"
 
         response = self._requester.request("DELETE", uri, _kwargs=kwargs)
 
         return response
 
     def get_billing_settings(self, **kwargs) -> SpaceBillingSettings:
         """
         Returns the billing settings for the space.
 
-        Calls "GET /spaces/{spaceId}/billing-settings"
-        Documentation https://fabman.io/api/v1/documentation#/spaces/getSpacesIdBillingsettings
+        :calls: "GET /spaces/{spaceId}/billing-settings" \
+		<https://fabman.io/api/v1/documentation#/spaces/getSpacesIdBillingsettings>
+  
+        :return: Object with billing settings information
+        :rtype: fabman.space.SpaceBillingSettings
         """
         if "billingSettings" in self._embedded:
             settings = self._embedded["billingSettings"]
             settings.update({"space_id": self.id})
             return SpaceBillingSettings(self._requester, settings)
 
         uri = f"/spaces/{self.id}/billing-settings"
@@ -171,55 +196,68 @@
 
         return SpaceBillingSettings(self._requester, data)
 
     def get_holiday(self, holiday_id, **kwargs) -> SpaceHoliday:
         """
         Returns a specific holiday for the space given a holiday_id.
 
-        Calls "GET /spaces/{spaceId}/holidays/{holidayId}"
-        Documentation https://fabman.io/api/v1/documentation#/spaces/getSpacesIdHolidaysHolidayid
+        :calls: "GET /spaces/{spaceId}/holidays/{holidayId}" \
+		<https://fabman.io/api/v1/documentation#/spaces/getSpacesIdHolidaysHolidayid>
+        
+        :param holiday_id: ID of the holiday to retrieve
+        :type holiday_id: int
+        :return: Object with holiday information
+        :rtype: fabman.space.SpaceHoliday
         """
 
         uri = f"/spaces/{self.id}/holidays/{holiday_id}"
 
         response = self._requester.request("GET", uri, _kwargs=kwargs)
 
         data = response.json()
         data.update({"space_id": self.id})
 
         return SpaceHoliday(self._requester, data)
 
     def get_holidays(self, **kwargs) -> Union[list, PaginatedList]:
         """
-        Returns a list of holidays for the space.
+        Returns a list of holidays for the space. If the information is cached from an embedded call, 
+        a list of SpaceHoliday objects is returned. Otherwise, a PaginatedList will be returned.
 
-        Calls "GET /spaces/{spaceId}/holidays"
-        Documentation https://fabman.io/api/v1/documentation#/spaces/getSpacesIdHolidays
+        :calls: "GET /spaces/{spaceId}/holidays" \
+		<https://fabman.io/api/v1/documentation#/spaces/getSpacesIdHolidays>
+  
+        :return: List of SpaceHoliday Objects
+        :rtype: list[fabman.space.SpaceHoliday] or fabman.paginated_list.PaginatedList
         """
         if "holidays" in self._embedded:
             out = []
-            for holiday in self._embedded["holiday"]:
-                setattr(holiday, "space_id", self.id)
+            for holiday in self._embedded["holidays"]:
+                holiday.update({"space_id": self.id})
                 out.append(SpaceHoliday(self._requester, holiday))
+            return out
 
         return PaginatedList(
             SpaceHoliday,
             self._requester,
             "GET",
             f"/spaces/{self.id}/holidays",
             extra_attribs={"space_id": self.id},
             kwargs=kwargs,
         )
 
-    def get_opening_hours(self, **kwargs) -> requests.Response:
+    def get_opening_hours(self, **kwargs) -> Union[list, requests.Response]:
         """
         Get the opening hours for the space.
 
-        Calls "GET /spaces/{spaceId}/opening-hours"
-        Documentation https://fabman.io/api/v1/documentation#/spaces/getSpacesIdOpeninghours
+        :calls: "GET /spaces/{spaceId}/opening-hours" \
+		<https://fabman.io/api/v1/documentation#/spaces/getSpacesIdOpeninghours>
+
+        :return: List of opening hours
+        :rtype: list
         """
 
         if "openingHours" in self._embedded:
             return self._embedded["openingHours"]
 
         uri = f"/spaces/{self.id}/opening-hours"
 
@@ -228,16 +266,19 @@
         return response
 
     def update(self, **kwargs) -> None:
         """
         Updates the space. Attributes are updated in place with new information
         from the API.
 
-        Calls "PUT /spaces/{spaceId}"
-        Documentation https://fabman.io/api/v1/documentation#/spaces/putSpacesId
+        :calls: "PUT /spaces/{spaceId}" \
+		<https://fabman.io/api/v1/documentation#/spaces/putSpacesId>
+
+        :return: None -- attributes are updated in place
+        :rtype: None
         """
 
         uri = f"/spaces/{self.id}"
 
         kwargs.update({"lockVersion": self.lockVersion})
 
         response = self._requester.request("PUT", uri, _kwargs=kwargs)
@@ -248,16 +289,19 @@
             setattr(self, attr, val)
 
     def update_calendar_token(self, **kwargs) -> requests.Response:
         """
         Updates the space calendar token and returns a link to the new calendar ics
         file. Calendar Token attribute is updated in place with new information.
 
-        Calls "PUT /spaces/{spaceId}/calendar-token"
-        Documentation https://fabman.io/api/v1/documentation#/spaces/putSpacesIdCalendartoken
+        :calls: "PUT /spaces/{spaceId}/calendar-token" \
+		<https://fabman.io/api/v1/documentation#/spaces/putSpacesIdCalendartoken>
+
+        :return: response information of call
+        :rtype: requests.Response
         """
 
         uri = f"/spaces/{self.id}/calendar-token"
 
         response = self._requester.request("PUT", uri, _kwargs=kwargs)
 
         data = response.json()
@@ -270,16 +314,19 @@
 
     def update_opening_hours(self, **kwargs) -> requests.Response:
         """
         Updates the opening hours of a space. If the the openingHours key is
         present in the _embedded attribute, the opening hours are updated in
         place with information returned by the api.
 
-        calls "PUT /spaces/{spaceId}/opening-hours"
-        Documentation https://fabman.io/api/v1/documentation#/spaces/putSpacesIdOpeninghours
+        :calls: "PUT /spaces/{spaceId}/opening-hours" \
+		<https://fabman.io/api/v1/documentation#/spaces/putSpacesIdOpeninghours>
+  
+        :return: response information of call
+        :rtype: requests.Response
         """
 
         uri = f"/spaces/{self.id}/opening-hours"
 
         response = self._requester.request("PUT", uri, _kwargs=kwargs)
 
         if "openingHours" in self._embedded:
```

### Comparing `fabman-1.1.17/fabman/training_course.py` & `fabman-1.1.20/fabman/training_course.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,37 +6,43 @@
 
 class TrainingCourse(FabmanObject):
     """TrainingCourse Object handles all API calls that operate on a single TrainingCourse."""
 
     def __str__(self):
         return f"TrainingCourse #{self.id}: {self.title}"
 
+    def delete(self, **kwargs) -> requests.Response:
+        """
+        Delete the training course. *WARNING: THIS CANNOT BE UNDONE.*
+
+        :calls: "DELETE /training-courses/{id}" \
+		<https://fabman.io/api/v1/documentation#/training-courses/deleteTrainingcoursesId>
+  
+        :return: response information of call
+        :rtype: requests.Response
+        """
+        uri = f"/training-courses/{self.id}"
+
+        response = self._requester.request("DELETE", uri, _kwargs=kwargs)
+
+        return response
+
     def update(self, **kwargs) -> None:
         """
         Update the training course with the given data. Will create the data
         if the training course does not exist.
 
-        Calls "PUT /training-courses/{id}"
-        Documentation https://fabman.io/api/v1/documentation#/training-courses/putTrainingcoursesId
+        :calls: "PUT /training-courses/{id}" \
+		<https://fabman.io/api/v1/documentation#/training-courses/putTrainingcoursesId>
+  
+        :return: None -- attributes are updated in place
+        :rtype: None
         """
         uri = f"/training-courses/{self.id}"
 
         kwargs.update({"lockVersion": self.lockVersion})
         response = self._requester.request("PUT", uri, _kwargs=kwargs)
 
         data = response.json()
 
         for attr, val in data.items():
             setattr(self, attr, val)
-
-    def delete(self, **kwargs) -> requests.Response:
-        """
-        Delete the training course. *WARNING: THIS CANNOT BE UNDONE.*
-
-        Calls "DELETE /training-courses/{id}"
-        Documentation https://fabman.io/api/v1/documentation#/training-courses/deleteTrainingcoursesId
-        """
-        uri = f"/training-courses/{self.id}"
-
-        response = self._requester.request("DELETE", uri, _kwargs=kwargs)
-
-        return response
```

### Comparing `fabman-1.1.17/fabman/util.py` & `fabman-1.1.20/fabman/util.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.17/fabman.egg-info/PKG-INFO` & `fabman-1.1.20/fabman.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: fabman
-Version: 1.1.17
+Version: 1.1.20
 Summary: Python wrappers for interacting with the Fabman API
 Author: Davin Lawrence
 Author-email: Davin Lawrence <davin.lawrence@utexas.edu>
 Project-URL: Homepage, https://github.com/utexas-engr-tiw/fabman-api
+Project-URL: Documentation, https://fabman-api.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/utexas-engr-tiw/fabman-api/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -25,14 +26,16 @@
 
 [![Fabman on PyPI](https://img.shields.io/pypi/v/fabman.svg)](https://pypi.python.org/pypi/fabman)
 [![License](https://img.shields.io/pypi/l/fabman.svg)](https://pypi.python.org/pypi/fabman)
 [![Python Versions](https://img.shields.io/pypi/pyversions/fabman.svg)](https://pypi.python.org/pypi/fabman)
 [![Build Status](https://github.com/utexas-engr-tiw/fabman-api/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/utexas-engr-tiw/fabman-api/actions)
 [![Coverage](https://codecov.io/gh/utexas-engr-tiw/fabman-api/branch/main/graph/badge.svg?token=AGABZU5YOJ)](https://codecov.io/gh/utexas-engr-tiw/fabman-api)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Documentation Status](https://readthedocs.org/projects/fabman-api/badge/?version=latest)](https://fabman-api.readthedocs.io/en/latest/?badge=latest)
+
 
 # Fabman API 
 
 Library for interfacing with the Fabman API. Created for Texas Inventionworks as part of the Cockrell School of Engineering at the University of Texas at Austin.
 
 Official documentation for the Fabman API can be found [here](https://github.com/FabmanHQ/fabman-api). Live interaction and description of all endpoints can further be found [here](https://fabman.io/api/v1/documentation#/). This library is currently targeting version 2.3.1 of the Fabman API.
 
@@ -56,19 +59,20 @@
 f = Fabman(API_KEY)
 ...
 ```
 
 From there, you can begin interacting with api endpoints as described in the official documentation. Most top-level methods return an object which manages that object. For example, to get a single member and update that member's name,
 ```python
 member = f.get_member(12345)
-member.update(firstName="Natalie", lastName="Wynn")
+member.update(firstName="Kira", lastName="Nerys")
 ```
+
 All parameters except for IDs are taken in as kwargs and should follow the camelCase naming conventions found on the Fabman API. Moreover, the library performs minimal checking of parameters, leaving that to the Fabman API. For required fields for create and update fields, refer to the [Live Fabman API Documentation](https://fabman.io/api/v1/documentation#/). The one exception to this is the `lockVersion` requirement for update methods. All update methods will automatically add the current `lockVersion` parameter to the body.
 
+Refer to the [library documentation](https://fabman-api.readthedocs.io/en/latest/) more information on this library.
+
 ## Contributing
 
 We would love contributions! We are a small development team. To contribute, familiarize yourself with the code, the layout, make your edits and a pull request. We currently need help with
 
-* Writing Mock Tests
-* Coverage of API endpoints
 * Real life testing of the API
 * Documentation
```

### Comparing `fabman-1.1.17/fabman.egg-info/SOURCES.txt` & `fabman-1.1.20/fabman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fabman-1.1.17/pyproject.toml` & `fabman-1.1.20/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel>=0.37.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fabman"
-version = "1.1.17"
+version = "1.1.20"
 authors = [
     {name = "Davin Lawrence", email="davin.lawrence@utexas.edu"},
 ]
 dependencies = [
     "requests>=2.31.0",
     "arrow>=1.2.3",
     "pytz==2023.3"
@@ -30,8 +30,9 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Education"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/utexas-engr-tiw/fabman-api"
-"Bug Tracker" = "https://github.com/utexas-engr-tiw/fabman-api/issues"
+"Documentation" = "https://fabman-api.readthedocs.io/en/latest/"
+"Bug Tracker" = "https://github.com/utexas-engr-tiw/fabman-api/issues"
```

### Comparing `fabman-1.1.17/setup.py` & `fabman-1.1.20/setup.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.17/tests/test_account.py` & `fabman-1.1.20/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.17/tests/test_api_key.py` & `fabman-1.1.20/tests/test_api_key.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.17/tests/test_booking.py` & `fabman-1.1.20/tests/test_booking.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.17/tests/test_charge.py` & `fabman-1.1.20/tests/test_charge.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.17/tests/test_fabman.py` & `fabman-1.1.20/tests/test_fabman.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,22 +403,14 @@
 
         resources = self.fabman.get_resource_logs()
         self.assertIsInstance(resources, PaginatedList)
         self.assertIsInstance(resources[0], ResourceLog)
         self.assertTrue(hasattr(resources[0], "id"))
         self.assertTrue(resources[0].id == 1)
 
-    def test_get_resource_type(self, m):
-        register_uris({"fabman": ["get_resource_type_by_id"]}, m)
-
-        resource_type = self.fabman.get_resource_type(1)
-        self.assertIsInstance(resource_type, ResourceType)
-        self.assertTrue(hasattr(resource_type, "id"))
-        self.assertTrue(resource_type.id == 1)
-
     def test_get_resource_types(self, m):
         register_uris({"fabman": ["get_resource_types"]}, m)
 
         resource_types = self.fabman.get_resource_types()
         self.assertIsInstance(resource_types, PaginatedList)
         self.assertTrue(hasattr(resource_types[0], "id"))
         self.assertTrue(resource_types[0].id == 1)
```

### Comparing `fabman-1.1.17/tests/test_invoice.py` & `fabman-1.1.20/tests/test_invoice.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.17/tests/test_job.py` & `fabman-1.1.20/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.17/tests/test_member.py` & `fabman-1.1.20/tests/test_member.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Tests for the Member class."""
-# pylint: disable=missing-function-docstring, missing-class-docstring, invalid-name, unused-argument
+# pylint: disable=missing-function-docstring, missing-class-docstring, invalid-name, unused-argument, protected-access
 
 import unittest
 import warnings
 
 import requests_mock
 
 from fabman import Fabman
@@ -110,15 +110,15 @@
         self.assertIsInstance(credit, MemberCredit)
 
     def test_get_device(self, m):
         register_uris({"member": ["get_device"]}, m)
 
         device = self.member.get_device()
         self.assertIsInstance(device, dict)
-        self.assertEqual(device["name"], "Apple iPhone")
+        self.assertEqual(device["name"], "Starfleet Tricorder")
 
     def test_get_device_embeded(self, m):
         register_uris({"fabman": ["get_member_by_id_device_embed"]}, m)
 
         member = self.fabman.get_member(1, embed=["device"])
 
         self.assertIsInstance(member, Member)
@@ -135,14 +135,60 @@
     def test_get_device_changes_by_id(self, m):
         register_uris({"member": ["get_device_change_by_id"]}, m)
 
         change = self.member.get_device_change(1)
 
         self.assertIsInstance(change, dict)
 
+    def test_get_embeds(self, m):
+        register_uris({"member": ["get_embeds"]}, m)
+
+        member = self.fabman.get_member(
+            1, embed=["memberPackages", "trainings", "key", "privileges", "device"]
+        )
+        self.assertIsInstance(member, Member)
+        self.assertTrue(hasattr(member, "_embedded"))
+        self.assertTrue("memberPackages" in member._embedded)
+        self.assertTrue("trainings" in member._embedded)
+        self.assertTrue("key" in member._embedded)
+        self.assertTrue("privileges" in member._embedded)
+        self.assertTrue("device" in member._embedded)
+
+        # memberPackages
+        packages = member.get_packages()
+        self.assertIsInstance(packages, list)
+        self.assertIsInstance(packages[0], MemberPackage)
+
+        package = member.get_package(1)
+        self.assertIsInstance(package, MemberPackage)
+
+        # trainings
+        trainings = member.get_trainings()
+        self.assertIsInstance(trainings, list)
+        self.assertTrue(trainings[0]["id"] == 2)
+
+        training = member.get_training(2)
+        self.assertIsInstance(training, dict)
+        self.assertTrue(training["id"] == 2)
+
+        # key
+        key = member.get_key()
+        self.assertIsInstance(key, MemberKey)
+        self.assertTrue(key.lockVersion == 4)
+
+        # privileges
+        privileges = member.get_privileges()
+        self.assertIsInstance(privileges, dict)
+        self.assertTrue(privileges["privileges"] == "member")
+
+        # device
+        device = member.get_device()
+        self.assertIsInstance(device, dict)
+        self.assertTrue(device["name"] == "Starfleet Communicator")
+
     def test_get_invitation(self, m):
         register_uris({"member": ["get_invitation"]}, m)
 
         invitation = self.member.get_invitation()
         self.assertIsInstance(invitation, dict)
 
     def test_get_key_empty(self, m):
```

### Comparing `fabman-1.1.17/tests/test_package.py` & `fabman-1.1.20/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.17/tests/test_paginated_list.py` & `fabman-1.1.20/tests/test_resource_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,45 @@
-"""Tests for the PaginatedList class."""
+"""Test for the ResourceType class"""
 # pylint: disable=missing-docstring, invalid-name, unused-argument
 
 import unittest
 
+import requests
 import requests_mock
 
 from fabman import Fabman
-from fabman.paginated_list import PaginatedList
+from fabman.resource_type import ResourceType
 from tests import settings
-from tests.util import register_uris
+from tests.util import register_uris, validate_update
 
 
 @requests_mock.Mocker()
-class TestPaginatedList(unittest.TestCase):
+class TestResourceType(unittest.TestCase):
     def setUp(self):
         self.fabman = Fabman(settings.API_KEY)
 
         with requests_mock.Mocker() as m:
-            register_uris({"fabman": ["get_members"]}, m)
+            register_uris({"fabman": ["get_resource_types"]}, m)
 
-            self.paginated_list: PaginatedList = self.fabman.get_members(limit=1)
+            self.resource_type: ResourceType = self.fabman.get_resource_types()[0]
 
-    def test_sanity(self, m):
-        self.assertEqual(1, 1)
+    def test_instance(self, m):
+        self.assertIsInstance(self.resource_type, ResourceType)
 
-    def test_repr(self, m):
-        self.assertEqual("<PaginatedList of type Member>", repr(self.paginated_list))
-
-    def test_format_link(self, m):
-        headers = {
-            "link": '<https://fabman.io/api/v1/members?limit=1&offset=1>; rel="next", <https://fabman.io/api/v1/members?limit=1&offset=2>; rel="last"'
-        }
-        link = self.paginated_list._PaginatedList__format_link(headers)
-        self.assertEqual(link, "/members?limit=1&offset=1")
+    def test_str(self, m):
+        string = str(self.resource_type)
+        self.assertTrue(string == "ResourceType #1: Starship")
+
+    def test_delete(self, m):
+        register_uris({"resource_type": ["delete"]}, m)
+
+        resp = self.resource_type.delete()
+        self.assertTrue(m.called)
+        self.assertIsInstance(resp, requests.Response)
+        self.assertTrue(resp.status_code == 204)
+
+    def test_update(self, m):
+        register_uris({"resource_type": ["update"]}, m)
+
+        self.resource_type.update(name="Victory Class Starship")
+        self.assertTrue(m.called)
+        self.assertTrue(self.resource_type.name == "Victory Class Starship")
```

### Comparing `fabman-1.1.17/tests/test_payment.py` & `fabman-1.1.20/tests/test_payment.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.17/tests/test_requester.py` & `fabman-1.1.20/tests/test_requester.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.17/tests/test_resource.py` & `fabman-1.1.20/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.17/tests/test_resource_log.py` & `fabman-1.1.20/tests/test_resource_log.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.17/tests/test_sanity.py` & `fabman-1.1.20/tests/test_sanity.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.17/tests/test_space.py` & `fabman-1.1.20/tests/test_space.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Tests for the Space class."""
-# pylint: disable=missing-docstring, invalid-name, unused-argument
+# pylint: disable=missing-docstring, invalid-name, unused-argument, protected-access
 
 import unittest
 
 import requests
 import requests_mock
 
 from fabman import Fabman
@@ -63,14 +63,42 @@
     def test_get_billing_settings(self, m):
         register_uris({"space": ["get_billing_settings"]}, m)
 
         billing = self.space.get_billing_settings()
         self.assertIsInstance(billing, SpaceBillingSettings)
         self.assertTrue(hasattr(billing, "space_id"))
 
+    def test_get_embedded(self, m):
+        register_uris({"space": ["get_embedded"]}, m)
+
+        space = self.fabman.get_space(
+            1, embed=["billingSettings", "holidays", "openingHours"]
+        )
+        self.assertIsInstance(space, Space)
+        self.assertTrue(hasattr(space, "_embedded"))
+
+        # billingSettings
+        self.assertTrue("billingSettings" in space._embedded)
+        billing = space.get_billing_settings()
+        self.assertIsInstance(billing, SpaceBillingSettings)
+        self.assertTrue(hasattr(billing, "space_id"))
+
+        # holidays
+        self.assertTrue("holidays" in space._embedded)
+        holidays = space.get_holidays()
+        self.assertIsInstance(holidays, list)
+        self.assertTrue(len(holidays) == 3)
+        self.assertIsInstance(holidays[0], SpaceHoliday)
+        self.assertTrue(hasattr(holidays[0], "space_id"))
+
+        # openingHours
+        self.assertTrue("openingHours" in space._embedded)
+        opening_hours = space.get_opening_hours()
+        self.assertIsInstance(opening_hours, list)
+
     def test_get_holiday(self, m):
         register_uris({"space": ["get_holiday"]}, m)
 
         holiday = self.space.get_holiday(1)
         self.assertIsInstance(holiday, SpaceHoliday)
         self.assertTrue(hasattr(holiday, "id"))
         self.assertTrue(holiday.id == 1)
```

### Comparing `fabman-1.1.17/tests/test_training_course.py` & `fabman-1.1.20/tests/test_training_course.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.17/tests/test_util.py` & `fabman-1.1.20/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.17/tests/test_webhook.py` & `fabman-1.1.20/tests/test_webhook.py`

 * *Files identical despite different names*

