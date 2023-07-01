# Comparing `tmp/django-learngual-0.13.tar.gz` & `tmp/django-learngual-0.13.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-learngual-0.13.tar", last modified: Sat Jul  1 04:39:39 2023, max compression
+gzip compressed data, was "django-learngual-0.13.1.tar", last modified: Sat Jul  1 16:08:25 2023, max compression
```

## Comparing `django-learngual-0.13.tar` & `django-learngual-0.13.1.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 04:39:39.298497 django-learngual-0.13/
--rw-r--r--   0 user       (501) staff       (20)     2901 2023-07-01 00:27:10.000000 django-learngual-0.13/LICENSE
--rw-r--r--   0 user       (501) staff       (20)      105 2023-07-01 00:32:47.000000 django-learngual-0.13/MANIFEST.in
--rw-r--r--   0 user       (501) staff       (20)     1893 2023-07-01 04:39:39.298707 django-learngual-0.13/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      940 2023-07-01 01:54:06.000000 django-learngual-0.13/README.rst
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 04:39:39.234807 django-learngual-0.13/django_learngual.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     1893 2023-07-01 04:39:39.000000 django-learngual-0.13/django_learngual.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      719 2023-07-01 04:39:39.000000 django-learngual-0.13/django_learngual.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-07-01 04:39:39.000000 django-learngual-0.13/django_learngual.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       10 2023-07-01 04:39:39.000000 django-learngual-0.13/django_learngual.egg-info/top_level.txt
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 04:39:39.261785 django-learngual-0.13/learngual/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/__init__.py
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/admin.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 04:39:39.272364 django-learngual-0.13/learngual/api/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/api/serializers.py
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/api/views.py
--rw-r--r--   0 user       (501) staff       (20)      312 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/apps.py
--rw-r--r--   0 user       (501) staff       (20)     4533 2023-07-01 01:57:30.000000 django-learngual-0.13/learngual/auth.py
--rw-r--r--   0 user       (501) staff       (20)     5347 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/authentication.py
--rw-r--r--   0 user       (501) staff       (20)      399 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/manager.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 04:39:39.279400 django-learngual-0.13/learngual/migrations/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/migrations/__init__.py
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/models.py
--rw-r--r--   0 user       (501) staff       (20)      642 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/permissions.py
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/signals.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 04:39:39.296784 django-learngual-0.13/learngual/tests/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/tests/__init__.py
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/tests/factories.py
--rw-r--r--   0 user       (501) staff       (20)     1691 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/tests/request_mock.py
--rw-r--r--   0 user       (501) staff       (20)     1867 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/tests/test_authentication.py
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/tests/test_drf_endpoints.py
--rw-r--r--   0 user       (501) staff       (20)     6496 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/tests/test_utils.py
--rw-r--r--   0 user       (501) staff       (20)      305 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/urls.py
--rw-r--r--   0 user       (501) staff       (20)    12051 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/utils.py
--rw-r--r--   0 user       (501) staff       (20)      972 2023-07-01 04:39:39.302646 django-learngual-0.13/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)       38 2023-07-01 00:39:27.000000 django-learngual-0.13/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:08:25.220715 django-learngual-0.13.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-01 16:07:35.000000 django-learngual-0.13.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-01 16:07:35.000000 django-learngual-0.13.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-01 16:08:25.220715 django-learngual-0.13.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-01 16:07:35.000000 django-learngual-0.13.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:08:25.216715 django-learngual-0.13.1/django_learngual.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-01 16:08:25.000000 django-learngual-0.13.1/django_learngual.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-01 16:08:25.000000 django-learngual-0.13.1/django_learngual.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 16:08:25.000000 django-learngual-0.13.1/django_learngual.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 16:08:25.000000 django-learngual-0.13.1/django_learngual.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:08:25.216715 django-learngual-0.13.1/learngual/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:08:21.000000 django-learngual-0.13.1/learngual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:08:21.000000 django-learngual-0.13.1/learngual/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:08:25.216715 django-learngual-0.13.1/learngual/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:08:21.000000 django-learngual-0.13.1/learngual/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:08:21.000000 django-learngual-0.13.1/learngual/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-01 16:08:21.000000 django-learngual-0.13.1/learngual/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-07-01 16:08:21.000000 django-learngual-0.13.1/learngual/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-01 16:08:21.000000 django-learngual-0.13.1/learngual/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:08:25.216715 django-learngual-0.13.1/learngual/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:08:21.000000 django-learngual-0.13.1/learngual/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:08:21.000000 django-learngual-0.13.1/learngual/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-01 16:08:21.000000 django-learngual-0.13.1/learngual/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:08:21.000000 django-learngual-0.13.1/learngual/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:08:25.220715 django-learngual-0.13.1/learngual/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:08:21.000000 django-learngual-0.13.1/learngual/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:08:21.000000 django-learngual-0.13.1/learngual/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-01 16:08:21.000000 django-learngual-0.13.1/learngual/tests/request_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-01 16:08:21.000000 django-learngual-0.13.1/learngual/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:08:21.000000 django-learngual-0.13.1/learngual/tests/test_drf_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-01 16:08:21.000000 django-learngual-0.13.1/learngual/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-01 16:08:21.000000 django-learngual-0.13.1/learngual/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13817 2023-07-01 16:08:21.000000 django-learngual-0.13.1/learngual/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-01 16:08:25.220715 django-learngual-0.13.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 16:07:35.000000 django-learngual-0.13.1/setup.py
```

### Comparing `django-learngual-0.13/LICENSE` & `django-learngual-0.13.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13/PKG-INFO` & `django-learngual-0.13.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-learngual
-Version: 0.13
+Version: 0.13.1
 Summary: Learngual helper package
 Home-page: https://learngual.com
 Author: learngual
 Author-email: developer@leanrgual.com
 Maintainer: Aniekutmfon
 Maintainer-email: aniekutmfonekere@gmail.com
 License: Proprietary Software License Agreement
@@ -15,14 +15,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ====================================
 Learngual Django
 ====================================
```

### Comparing `django-learngual-0.13/README.rst` & `django-learngual-0.13.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13/django_learngual.egg-info/PKG-INFO` & `django-learngual-0.13.1/django_learngual.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-learngual
-Version: 0.13
+Version: 0.13.1
 Summary: Learngual helper package
 Home-page: https://learngual.com
 Author: learngual
 Author-email: developer@leanrgual.com
 Maintainer: Aniekutmfon
 Maintainer-email: aniekutmfonekere@gmail.com
 License: Proprietary Software License Agreement
@@ -15,14 +15,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ====================================
 Learngual Django
 ====================================
```

### Comparing `django-learngual-0.13/django_learngual.egg-info/SOURCES.txt` & `django-learngual-0.13.1/django_learngual.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 django_learngual.egg-info/PKG-INFO
 django_learngual.egg-info/SOURCES.txt
 django_learngual.egg-info/dependency_links.txt
 django_learngual.egg-info/top_level.txt
 learngual/__init__.py
 learngual/admin.py
 learngual/apps.py
-learngual/auth.py
 learngual/authentication.py
 learngual/manager.py
 learngual/models.py
 learngual/permissions.py
 learngual/signals.py
 learngual/urls.py
 learngual/utils.py
```

### Comparing `django-learngual-0.13/learngual/auth.py` & `django-learngual-0.13.1/learngual/authentication.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 import importlib
+import logging
+import os
 from uuid import uuid4
 
 import requests
 from django.conf import settings
 from django.contrib.auth import get_user_model
-from rest_framework import authentication
+from django.utils.translation import gettext_lazy as _
+from rest_framework import authentication, exceptions
 from rest_framework.request import Request
 
+User = get_user_model()
+
+LEARNGUAL_SERVICE_API_KEY = getattr(
+    settings, "LEARNGUAL_SERVICE_API_KEY", None
+) or os.getenv("LEARNGUAL_SERVICE_API_KEY", None)
+
 """
 Configure authentication class
 REST_FRAMEWORK = {
     "DEFAULT_AUTHENTICATION_CLASSES": (
         ...
         "iam_service.users.authentication.LearngualAuthentication",
         ...
@@ -70,15 +79,15 @@
 def load_callable(path: str):
     paths = path.split(".")
     modules = importlib.import_module(".".join(paths[:-1]))
     return getattr(modules, paths[-1])
 
 
 LEARNGUAL_AUTH_RETRIEVE_URL = getattr(settings, "LEARNGUAL_AUTH_RETRIEVE_URL", None)
-LEARNGUAL_AUTH_TEST_MODE = getattr(settings, "LEARNGUAL_AUTH_MODE", None)
+LEARNGUAL_AUTH_TEST_MODE = getattr(settings, "LEARNGUAL_AUTH_TEST_MODE", None)
 LEARNGUAL_AUTH_GET_USER = getattr(settings, "LEARNGUAL_AUTH_GET_USER", None)
 
 
 assert (
     LEARNGUAL_AUTH_RETRIEVE_URL
 ), "LEARNGUAL_AUTH_RETRIEVE_URL must be provided in the settings."
 assert (
@@ -117,19 +126,39 @@
         return headers
 
     @classmethod
     def get_query_str(cls, request: Request):
         return "?{query}".format(query=request.META.get("QUERY_STRING", ""))
 
     def authenticate(self, request):
+        # logging.info(
+        #     "am here ooo %s" % dict(LEARNGUAL_AUTH_TEST_MODE=LEARNGUAL_AUTH_TEST_MODE)
+        # )
         # this is for test mode
+
+        service_key = str(
+            request.META.get("HTTP_SERVICE_KEY", "")
+            or request.GET.get("service-key", "")
+            and request.GET.get("_service-key", "")
+        )
+        if service_key:
+            if service_key == LEARNGUAL_SERVICE_API_KEY:
+                service_user = User(id="service", username="service")
+                service_user.is_service = True
+                return service_user, service_key
+
+            msg = _("Invalid service key")
+            raise exceptions.AuthenticationFailed(msg)
+
         if LEARNGUAL_AUTH_TEST_MODE:
+            logging.info("%s is in test mode" % self.__class__.__name__)
             return get_user(user_test_data), uuid4().hex
 
         header = self.get_header(request)
+
         if not header.get("authorization"):
             return None
         headers = self.get_http_headers(request)
 
         res = requests.get(
             LEARNGUAL_AUTH_RETRIEVE_URL + self.get_query_str(request), headers=headers
         )
@@ -144,10 +173,31 @@
     def get_header(self, request):
         """
         Extracts the header containing the JSON web token from the given
         request.
         """
         account_id = str(request.META.get("HTTP_ACCOUNT", ""))
         api_key = str(request.META.get("HTTP_API_KEY", ""))
+        service_key = str(
+            request.META.get("HTTP_SERVICE_KEY", "")
+            or request.GET.get("service-key", "")
+            and request.GET.get("_service-key", "")
+        )
         authorization = str(request.META.get("HTTP_AUTHORIZATION", ""))
 
-        return dict(account_id=account_id, api_key=api_key, authorization=authorization)
+        return dict(
+            account_id=account_id,
+            api_key=api_key,
+            authorization=authorization,
+            service_key=service_key,
+        )
+
+
+def default_user_authentication_rule(user):
+    # Prior to Django 1.10, inactive users could be authenticated with the
+    # default `ModelBackend`.  As of Django 1.10, the `ModelBackend`
+    # prevents inactive users from authenticating.  App designers can still
+    # allow inactive users to authenticate by opting for the new
+    # `AllowAllUsersModelBackend`.  However, we explicitly prevent inactive
+    # users from authenticating to enforce a reasonable policy and provide
+    # sensible backwards compatibility with older Django versions.
+    return user is not None and user.is_active
```

### Comparing `django-learngual-0.13/learngual/tests/request_mock.py` & `django-learngual-0.13.1/learngual/tests/request_mock.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,39 @@
 from unittest.mock import MagicMock
 
 # Mocking the requests library
 requests = MagicMock()
 
 # Mocking the get() function
-requests.get = MagicMock()
 requests.get.return_value = MagicMock(status_code=200, text="Mocked response")
 requests.get.return_value.json.return_value = {"key": "value"}
 requests.get.return_value.ok = True
 
 # Mocking the post() function
-requests.post = MagicMock()
 requests.post.return_value = MagicMock(status_code=201, text="Created")
 requests.post.return_value.json.return_value = {"key": "value"}
 requests.post.return_value.ok = True
 
 # Mocking the put() function
-requests.put = MagicMock()
 requests.put.return_value = MagicMock(status_code=204, text="No Content")
 requests.put.return_value.json.return_value = None
 requests.put.return_value.ok = True
 
 # Mocking the delete() function
-requests.delete = MagicMock()
 requests.delete.return_value = MagicMock(status_code=204, text="No Content")
 requests.delete.return_value.json.return_value = None
 requests.delete.return_value.ok = True
 
 # Mocking the patch() function
-requests.patch = MagicMock()
 requests.patch.return_value = MagicMock(status_code=200, text="Updated")
 requests.patch.return_value.json.return_value = {"key": "value"}
 requests.patch.return_value.ok = True
 
 # Mocking the head() function
-requests.head = MagicMock()
 requests.head.return_value = MagicMock(status_code=200, text="OK")
 requests.head.return_value.json.return_value = None
 requests.head.return_value.ok = True
 
 # Mocking the options() function
-requests.options = MagicMock()
 requests.options.return_value = MagicMock(status_code=200, text="OK")
 requests.options.return_value.json.return_value = None
 requests.options.return_value.ok = True
```

### Comparing `django-learngual-0.13/learngual/tests/test_utils.py` & `django-learngual-0.13.1/learngual/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+from random import choice
 from unittest.mock import patch
+from uuid import uuid4
 
 from faker import Faker
 
 from ..utils import (
+    PermissionManager,
     PermissonUtils,
     flatten_dict,
     get_nested_value,
     unflatten_dict,
     update_nested_value,
 )
 from .request_mock import requests
@@ -160,30 +163,28 @@
     }
     assert PermissonUtils(permission_data).to_flat_dict() == permission_data_flat
     assert PermissonUtils(permission_data).to_dict() == permission_data
 
 
 @patch("requests.get", return_value=requests.get)
 def test_permission_manager(mock_requests):
-    # permission_manager: PermissionManager = PermissionManager()
+    permission_manager: PermissionManager = PermissionManager()
     permission_flat_dict = {
         "metadata.request_count.value": 100000,
         "metadata.messages.value": True,
         "metadata.analytics.value": False,
     }
     permission_dict = unflatten_dict(permission_flat_dict)
     assert not permission_dict.get("metadata.request_count.value")
-    mock_requests.json.return_value = permission_dict
-    # random_key = choice(list(permission_flat_dict.keys()))
-    # res = permission_manager.retrieve_permission(
-    #     base_url="https://localhost",
-    #     permission_id=uuid4().hex[:10],
-    #     service="iam"
-    # )
-    # assert res == permission_dict,res
-    # res = permission_manager.retrieve_permission(
-    #     base_url="https://localhost",
-    #     permission_id=uuid4().hex[:10],
-    #     service="iam",
-    #     dot_path=random_key
-    # )
-    # assert res == permission_flat_dict.get(random_key),res
+    mock_requests.return_value.json.return_value = permission_dict
+    random_key = choice(list(permission_flat_dict.keys()))
+    res = permission_manager.retrieve_permission(
+        base_url="https://localhost", permission_id=uuid4().hex[:10], service="iam"
+    )
+    assert res == permission_dict, res
+    res = permission_manager.retrieve_permission(
+        base_url="https://localhost",
+        permission_id=uuid4().hex[:10],
+        service="iam",
+        dot_path=random_key,
+    )
+    assert res == permission_flat_dict.get(random_key), res
```

### Comparing `django-learngual-0.13/learngual/utils.py` & `django-learngual-0.13.1/learngual/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,46 @@
 import logging
+import os
 from typing import Any, Literal
 
 import requests
+from django.conf import settings
 from django.core.cache import cache
 
 # from django.utils import timezone
 
+LEARNGUAL_SERVICE_API_KEY = getattr(
+    settings, "LEARNGUAL_SERVICE_API_KEY", None
+) or os.getenv("LEARNGUAL_SERVICE_API_KEY", None)
+
 
 def get_service_request_headers(**kwargs) -> dict:
     """function add headers needed for request made from a service
 
     Returns:
         dict: _description_
     """
+    if LEARNGUAL_SERVICE_API_KEY:
+        kwargs["service-key"] = LEARNGUAL_SERVICE_API_KEY
 
     return {**kwargs}
 
 
 def get_service_request_params(**kwargs) -> str:
     """function return query params needed to make request as a service
 
     Returns:
         dict: _description_
     """
 
-    return ""
+    if LEARNGUAL_SERVICE_API_KEY:
+        kwargs["_service-key"] = LEARNGUAL_SERVICE_API_KEY
+    if not kwargs:
+        return ""
+    return "?" + "&".join([f"{x}={y}" for x, y in kwargs.items()])
 
 
 def get_nested_value(data: dict[str, Any], path: str):
     """
     Retrieve a nested dictionary value using a dot path, including support for accessing lists and slicing.
 
     Args:
@@ -374,42 +386,77 @@
 
     def update_permission_with_api(
         self,
         base_url: str,
         permission_id,
         service: Literal["iam", "payment", "notify", "learn", "media"] = "iam",
         permmission_data=dict(),
+        headers: dict = dict(),
+        params: str = "",
     ):
+        """_summary_
+
+        Args:
+            base_url (str): _description_
+            permission_id (_type_): _description_
+            service (Literal["iam", "payment", "notify", "learn", "media"], optional): _description_. Defaults to "iam".
+            permmission_data (_type_, optional): _description_. Defaults to dict().
+            headers (dict, optional): _description_. Defaults to dict().
+            params (str, optional): e.g name=aka&age=201. Defaults to "".
+
+        Raises:
+            requests.exceptions.RequestException: _description_
+
+        Returns:
+            _type_: _description_
+        """
+        params = params.strip("?")
+        params = dict([x.split("=") for x in params.split("&")])
+
         url_path = f"/{service}/v1/permission/{permission_id}/"
-        res = requests.patch(base_url.rstrip("/") + url_path, json=permmission_data)
+        res = requests.patch(
+            base_url.rstrip("/") + url_path + get_service_request_params(**params),
+            json=permmission_data,
+            headers=get_service_request_headers(**headers),
+        )
         if not res.ok:
             raise requests.exceptions.RequestException(res.content)
         return res.json()
 
     def retrieve_permission(
         self,
         *,
         base_url: str,
         permission_id,
         service: Literal["iam", "payment", "notify", "learn", "media"] = "iam",
         dot_path: str = None,
+        headers: dict = dict(),
+        params: str = "",
     ):
         """_summary_
 
         Args:
             permission_id (str): example: '123456', 'sdGh66gGGHgfadsty', 'product:1234567'
             service (_type_): "iam" | "pay" | "notify" | "learn" | "media"
             base_url (str):
             dot_path (str):Default:None, e.g metadata.request_count.value
+            headers (dict):Default:{}
+            params (str):Default:"", e.g name=ann&age=102
         """
         url_path = f"/{service}/v1/permission/{permission_id}/"
         data = cache.get(url_path)
 
+        params = params.strip("?")
+        params = dict([x.split("=") for x in params.split("&") if x])
+
         if not data:
-            res = requests.get(base_url.rstrip("/") + url_path)
+            res = requests.get(
+                base_url.rstrip("/") + url_path + get_service_request_params(**params),
+                headers=get_service_request_headers(**headers),
+            )
             if not res.ok:
                 raise requests.exceptions.RequestException(res.content)
             data = res.json()
             # TODO fine a way to remove the cache when a new permission is added
             # cache.set(url_path, data, timeout=timezone.timedelta(hours=1).total_seconds())
 
         if dot_path:
```

