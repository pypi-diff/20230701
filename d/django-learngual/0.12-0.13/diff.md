# Comparing `tmp/django-learngual-0.12.tar.gz` & `tmp/django-learngual-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-learngual-0.12.tar", last modified: Sat Jul  1 03:39:33 2023, max compression
+gzip compressed data, was "django-learngual-0.13.tar", last modified: Sat Jul  1 04:39:39 2023, max compression
```

## Comparing `django-learngual-0.12.tar` & `django-learngual-0.13.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 03:39:33.839883 django-learngual-0.12/
--rw-r--r--   0 user       (501) staff       (20)     2901 2023-07-01 00:27:10.000000 django-learngual-0.12/LICENSE
--rw-r--r--   0 user       (501) staff       (20)      105 2023-07-01 00:32:47.000000 django-learngual-0.12/MANIFEST.in
--rw-r--r--   0 user       (501) staff       (20)     1893 2023-07-01 03:39:33.840080 django-learngual-0.12/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      940 2023-07-01 01:54:06.000000 django-learngual-0.12/README.rst
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 03:39:33.778790 django-learngual-0.12/django_learngual.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     1893 2023-07-01 03:39:33.000000 django-learngual-0.12/django_learngual.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      719 2023-07-01 03:39:33.000000 django-learngual-0.12/django_learngual.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-07-01 03:39:33.000000 django-learngual-0.12/django_learngual.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       10 2023-07-01 03:39:33.000000 django-learngual-0.12/django_learngual.egg-info/top_level.txt
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 03:39:33.813433 django-learngual-0.12/learngual/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/__init__.py
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/admin.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 03:39:33.828183 django-learngual-0.12/learngual/api/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/api/serializers.py
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/api/views.py
--rw-r--r--   0 user       (501) staff       (20)      312 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/apps.py
--rw-r--r--   0 user       (501) staff       (20)     4533 2023-07-01 01:57:30.000000 django-learngual-0.12/learngual/auth.py
--rw-r--r--   0 user       (501) staff       (20)     5347 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/authentication.py
--rw-r--r--   0 user       (501) staff       (20)      399 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/manager.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 03:39:33.829509 django-learngual-0.12/learngual/migrations/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/migrations/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    15755 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/models.py
--rw-r--r--   0 user       (501) staff       (20)      642 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/permissions.py
--rw-r--r--   0 user       (501) staff       (20)     2215 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/signals.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 03:39:33.839034 django-learngual-0.12/learngual/tests/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/tests/__init__.py
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/tests/factories.py
--rw-r--r--   0 user       (501) staff       (20)     1691 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/tests/request_mock.py
--rw-r--r--   0 user       (501) staff       (20)     1886 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/tests/test_authentication.py
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/tests/test_drf_endpoints.py
--rw-r--r--   0 user       (501) staff       (20)     6496 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/tests/test_utils.py
--rw-r--r--   0 user       (501) staff       (20)      305 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/urls.py
--rw-r--r--   0 user       (501) staff       (20)    12051 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/utils.py
--rw-r--r--   0 user       (501) staff       (20)      972 2023-07-01 03:39:33.842034 django-learngual-0.12/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)       38 2023-07-01 00:39:27.000000 django-learngual-0.12/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 04:39:39.298497 django-learngual-0.13/
+-rw-r--r--   0 user       (501) staff       (20)     2901 2023-07-01 00:27:10.000000 django-learngual-0.13/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)      105 2023-07-01 00:32:47.000000 django-learngual-0.13/MANIFEST.in
+-rw-r--r--   0 user       (501) staff       (20)     1893 2023-07-01 04:39:39.298707 django-learngual-0.13/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      940 2023-07-01 01:54:06.000000 django-learngual-0.13/README.rst
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 04:39:39.234807 django-learngual-0.13/django_learngual.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     1893 2023-07-01 04:39:39.000000 django-learngual-0.13/django_learngual.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      719 2023-07-01 04:39:39.000000 django-learngual-0.13/django_learngual.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-07-01 04:39:39.000000 django-learngual-0.13/django_learngual.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       10 2023-07-01 04:39:39.000000 django-learngual-0.13/django_learngual.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 04:39:39.261785 django-learngual-0.13/learngual/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/admin.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 04:39:39.272364 django-learngual-0.13/learngual/api/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/api/serializers.py
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/api/views.py
+-rw-r--r--   0 user       (501) staff       (20)      312 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/apps.py
+-rw-r--r--   0 user       (501) staff       (20)     4533 2023-07-01 01:57:30.000000 django-learngual-0.13/learngual/auth.py
+-rw-r--r--   0 user       (501) staff       (20)     5347 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/authentication.py
+-rw-r--r--   0 user       (501) staff       (20)      399 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/manager.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 04:39:39.279400 django-learngual-0.13/learngual/migrations/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/migrations/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/models.py
+-rw-r--r--   0 user       (501) staff       (20)      642 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/permissions.py
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/signals.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 04:39:39.296784 django-learngual-0.13/learngual/tests/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/tests/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/tests/factories.py
+-rw-r--r--   0 user       (501) staff       (20)     1691 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/tests/request_mock.py
+-rw-r--r--   0 user       (501) staff       (20)     1867 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/tests/test_authentication.py
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/tests/test_drf_endpoints.py
+-rw-r--r--   0 user       (501) staff       (20)     6496 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/tests/test_utils.py
+-rw-r--r--   0 user       (501) staff       (20)      305 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/urls.py
+-rw-r--r--   0 user       (501) staff       (20)    12051 2023-07-01 04:39:29.000000 django-learngual-0.13/learngual/utils.py
+-rw-r--r--   0 user       (501) staff       (20)      972 2023-07-01 04:39:39.302646 django-learngual-0.13/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-07-01 00:39:27.000000 django-learngual-0.13/setup.py
```

### Comparing `django-learngual-0.12/LICENSE` & `django-learngual-0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `django-learngual-0.12/PKG-INFO` & `django-learngual-0.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-learngual
-Version: 0.12
+Version: 0.13
 Summary: Learngual helper package
 Home-page: https://learngual.com
 Author: learngual
 Author-email: developer@leanrgual.com
 Maintainer: Aniekutmfon
 Maintainer-email: aniekutmfonekere@gmail.com
 License: Proprietary Software License Agreement
```

### Comparing `django-learngual-0.12/README.rst` & `django-learngual-0.13/README.rst`

 * *Files identical despite different names*

### Comparing `django-learngual-0.12/django_learngual.egg-info/PKG-INFO` & `django-learngual-0.13/django_learngual.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-learngual
-Version: 0.12
+Version: 0.13
 Summary: Learngual helper package
 Home-page: https://learngual.com
 Author: learngual
 Author-email: developer@leanrgual.com
 Maintainer: Aniekutmfon
 Maintainer-email: aniekutmfonekere@gmail.com
 License: Proprietary Software License Agreement
```

### Comparing `django-learngual-0.12/django_learngual.egg-info/SOURCES.txt` & `django-learngual-0.13/django_learngual.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-learngual-0.12/learngual/auth.py` & `django-learngual-0.13/learngual/auth.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.12/learngual/authentication.py` & `django-learngual-0.13/learngual/authentication.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.12/learngual/permissions.py` & `django-learngual-0.13/learngual/permissions.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.12/learngual/tests/request_mock.py` & `django-learngual-0.13/learngual/tests/request_mock.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.12/learngual/tests/test_authentication.py` & `django-learngual-0.13/learngual/tests/test_authentication.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from unittest.mock import patch
 
 from django.contrib.auth import get_user_model
-from rest_framework.request import Request
-from rest_framework.test import APIClient
+from rest_framework.test import APIClient, APIRequestFactory
 
 from ..authentication import LearngualAuthentication
 from .request_mock import requests as mock_requests
-from rest_framework.test import APIRequestFactory
+
 factory = APIRequestFactory()
 User = get_user_model()
 
 
-
 @patch("iam_service.learngual.authentication.get_user")
-@patch("requests.get",return_value=mock_requests.get)
-def test_authentication(mock_req,get_user,user:User,client:APIClient):
+@patch("requests.get", return_value=mock_requests.get)
+def test_authentication(mock_req, get_user, user: User, client: APIClient):
     # Create a sample request
     get_user.return_value = user
     mock_req.json.return_value = {
         "account": {
             "id": "84bcaf2972",
             "cover_photo": None,
             "profile_photo": None,
@@ -30,23 +28,26 @@
         "email": "Bulah53@gmail.com",
         "first_name": "Caitlyn",
         "id": "40e0e7013f",
         "last_name": "Marquardt",
         "registration_step": "REGISTRATION_COMPLETED",
         "username": "Eloisa.Senger42",
     }
-    request = factory.get('/api/my-endpoint/')
+    request = factory.get("/api/my-endpoint/")
 
     # Add the custom header to the request
-    token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6InRlc3R1c2VyIiwiaWF0IjoxNjIzMzQ5NTMwLCJleHAiOjE2MjMzNTM5MzB9.6FcybZUxW1szsiavTbF-MfnEvC57lU3J0C1dd6nM2O0"
-    request.META['HTTP_AUTHORIZATION'] = 'Bearer '+token
+    token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9"
+    token += (
+        ".eyJ1c2VybmFtZSI6InRlc3R1c2VyIiwiaWF0IjoxNjIzMzQ5NTMwLCJleHAiOjE2MjMzNTM5MzB9"
+    )
+    token += ".6FcybZUxW1szsiavTbF-MfnEvC57lU3J0C1dd6nM2O0"
+    request.META["HTTP_AUTHORIZATION"] = "Bearer " + token
 
     # Authenticate the request
 
-
     # Create an instance of the custom authentication class
     auth = LearngualAuthentication()
 
     # Authenticate the request using the custom authentication class
     authenticated = auth.authenticate(request)
 
     # Assert that authentication is successful
```

### Comparing `django-learngual-0.12/learngual/tests/test_utils.py` & `django-learngual-0.13/learngual/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.12/learngual/utils.py` & `django-learngual-0.13/learngual/utils.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.12/setup.cfg` & `django-learngual-0.13/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-learngual
-version = 0.12
+version = 0.13
 author = learngual
 author_email = developer@leanrgual.com
 maintainer = Aniekutmfon
 maintainer_email = aniekutmfonekere@gmail.com
 description = Learngual helper package
 long_description = file:README.rst
 long_description_content_type = text/x-rst
```

