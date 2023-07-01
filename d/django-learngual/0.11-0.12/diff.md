# Comparing `tmp/django-learngual-0.11.tar.gz` & `tmp/django-learngual-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-learngual-0.11.tar", last modified: Sat Jul  1 01:57:40 2023, max compression
+gzip compressed data, was "django-learngual-0.12.tar", last modified: Sat Jul  1 03:39:33 2023, max compression
```

## Comparing `django-learngual-0.11.tar` & `django-learngual-0.12.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 01:57:40.118379 django-learngual-0.11/
--rw-r--r--   0 user       (501) staff       (20)     2901 2023-07-01 00:27:10.000000 django-learngual-0.11/LICENSE
--rw-r--r--   0 user       (501) staff       (20)      105 2023-07-01 00:32:47.000000 django-learngual-0.11/MANIFEST.in
--rw-r--r--   0 user       (501) staff       (20)     1893 2023-07-01 01:57:40.121263 django-learngual-0.11/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      940 2023-07-01 01:54:06.000000 django-learngual-0.11/README.rst
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 01:57:40.068234 django-learngual-0.11/django_learngual.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     1893 2023-07-01 01:57:39.000000 django-learngual-0.11/django_learngual.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      620 2023-07-01 01:57:40.000000 django-learngual-0.11/django_learngual.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-07-01 01:57:39.000000 django-learngual-0.11/django_learngual.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       10 2023-07-01 01:57:39.000000 django-learngual-0.11/django_learngual.egg-info/top_level.txt
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 01:57:40.097022 django-learngual-0.11/learngual/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 01:57:30.000000 django-learngual-0.11/learngual/__init__.py
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 01:57:30.000000 django-learngual-0.11/learngual/admin.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 01:57:40.113898 django-learngual-0.11/learngual/api/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 01:57:31.000000 django-learngual-0.11/learngual/api/serializers.py
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 01:57:31.000000 django-learngual-0.11/learngual/api/views.py
--rw-r--r--   0 user       (501) staff       (20)      312 2023-07-01 01:57:30.000000 django-learngual-0.11/learngual/apps.py
--rw-r--r--   0 user       (501) staff       (20)     4533 2023-07-01 01:57:30.000000 django-learngual-0.11/learngual/auth.py
--rw-r--r--   0 user       (501) staff       (20)      399 2023-07-01 01:57:31.000000 django-learngual-0.11/learngual/manager.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 01:57:40.115155 django-learngual-0.11/learngual/migrations/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 01:57:30.000000 django-learngual-0.11/learngual/migrations/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    15755 2023-07-01 01:57:30.000000 django-learngual-0.11/learngual/models.py
--rw-r--r--   0 user       (501) staff       (20)      642 2023-07-01 01:57:31.000000 django-learngual-0.11/learngual/permissions.py
--rw-r--r--   0 user       (501) staff       (20)     2215 2023-07-01 01:57:30.000000 django-learngual-0.11/learngual/signals.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 01:57:40.117957 django-learngual-0.11/learngual/tests/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 01:57:30.000000 django-learngual-0.11/learngual/tests/__init__.py
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 01:57:30.000000 django-learngual-0.11/learngual/tests/factories.py
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 01:57:30.000000 django-learngual-0.11/learngual/tests/test_drf_endpoints.py
--rw-r--r--   0 user       (501) staff       (20)     5394 2023-07-01 01:57:30.000000 django-learngual-0.11/learngual/tests/test_utils.py
--rw-r--r--   0 user       (501) staff       (20)      305 2023-07-01 01:57:31.000000 django-learngual-0.11/learngual/urls.py
--rw-r--r--   0 user       (501) staff       (20)    12039 2023-07-01 01:57:30.000000 django-learngual-0.11/learngual/utils.py
--rw-r--r--   0 user       (501) staff       (20)      972 2023-07-01 01:57:40.123781 django-learngual-0.11/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)       38 2023-07-01 00:39:27.000000 django-learngual-0.11/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 03:39:33.839883 django-learngual-0.12/
+-rw-r--r--   0 user       (501) staff       (20)     2901 2023-07-01 00:27:10.000000 django-learngual-0.12/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)      105 2023-07-01 00:32:47.000000 django-learngual-0.12/MANIFEST.in
+-rw-r--r--   0 user       (501) staff       (20)     1893 2023-07-01 03:39:33.840080 django-learngual-0.12/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      940 2023-07-01 01:54:06.000000 django-learngual-0.12/README.rst
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 03:39:33.778790 django-learngual-0.12/django_learngual.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     1893 2023-07-01 03:39:33.000000 django-learngual-0.12/django_learngual.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      719 2023-07-01 03:39:33.000000 django-learngual-0.12/django_learngual.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-07-01 03:39:33.000000 django-learngual-0.12/django_learngual.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       10 2023-07-01 03:39:33.000000 django-learngual-0.12/django_learngual.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 03:39:33.813433 django-learngual-0.12/learngual/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/admin.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 03:39:33.828183 django-learngual-0.12/learngual/api/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/api/serializers.py
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/api/views.py
+-rw-r--r--   0 user       (501) staff       (20)      312 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/apps.py
+-rw-r--r--   0 user       (501) staff       (20)     4533 2023-07-01 01:57:30.000000 django-learngual-0.12/learngual/auth.py
+-rw-r--r--   0 user       (501) staff       (20)     5347 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/authentication.py
+-rw-r--r--   0 user       (501) staff       (20)      399 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/manager.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 03:39:33.829509 django-learngual-0.12/learngual/migrations/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/migrations/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    15755 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/models.py
+-rw-r--r--   0 user       (501) staff       (20)      642 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/permissions.py
+-rw-r--r--   0 user       (501) staff       (20)     2215 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/signals.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 03:39:33.839034 django-learngual-0.12/learngual/tests/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/tests/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/tests/factories.py
+-rw-r--r--   0 user       (501) staff       (20)     1691 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/tests/request_mock.py
+-rw-r--r--   0 user       (501) staff       (20)     1886 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/tests/test_authentication.py
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/tests/test_drf_endpoints.py
+-rw-r--r--   0 user       (501) staff       (20)     6496 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/tests/test_utils.py
+-rw-r--r--   0 user       (501) staff       (20)      305 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/urls.py
+-rw-r--r--   0 user       (501) staff       (20)    12051 2023-07-01 03:39:22.000000 django-learngual-0.12/learngual/utils.py
+-rw-r--r--   0 user       (501) staff       (20)      972 2023-07-01 03:39:33.842034 django-learngual-0.12/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-07-01 00:39:27.000000 django-learngual-0.12/setup.py
```

### Comparing `django-learngual-0.11/LICENSE` & `django-learngual-0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `django-learngual-0.11/PKG-INFO` & `django-learngual-0.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-learngual
-Version: 0.11
+Version: 0.12
 Summary: Learngual helper package
 Home-page: https://learngual.com
 Author: learngual
 Author-email: developer@leanrgual.com
 Maintainer: Aniekutmfon
 Maintainer-email: aniekutmfonekere@gmail.com
 License: Proprietary Software License Agreement
```

### Comparing `django-learngual-0.11/README.rst` & `django-learngual-0.12/README.rst`

 * *Files identical despite different names*

### Comparing `django-learngual-0.11/django_learngual.egg-info/PKG-INFO` & `django-learngual-0.12/django_learngual.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-learngual
-Version: 0.11
+Version: 0.12
 Summary: Learngual helper package
 Home-page: https://learngual.com
 Author: learngual
 Author-email: developer@leanrgual.com
 Maintainer: Aniekutmfon
 Maintainer-email: aniekutmfonekere@gmail.com
 License: Proprietary Software License Agreement
```

### Comparing `django-learngual-0.11/learngual/auth.py` & `django-learngual-0.12/learngual/auth.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.11/learngual/models.py` & `django-learngual-0.12/learngual/models.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.11/learngual/permissions.py` & `django-learngual-0.12/learngual/permissions.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.11/learngual/signals.py` & `django-learngual-0.12/learngual/signals.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.11/learngual/tests/test_utils.py` & `django-learngual-0.12/learngual/tests/test_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from unittest.mock import patch
+
 from faker import Faker
 
 from ..utils import (
     PermissonUtils,
     flatten_dict,
     get_nested_value,
     unflatten_dict,
     update_nested_value,
 )
+from .request_mock import requests
 
 faker = Faker()
 
 
 def test_update_nested_value():
     permission_data: dict = dict(
         metadata=dict(
@@ -153,7 +156,34 @@
         "metadata.manage_courses.value": permission_data.get("metadata", {})
         .get("manage_courses", {})
         .get("value"),
         "metadata.ids": permission_data.get("metadata", {}).get("ids"),
     }
     assert PermissonUtils(permission_data).to_flat_dict() == permission_data_flat
     assert PermissonUtils(permission_data).to_dict() == permission_data
+
+
+@patch("requests.get", return_value=requests.get)
+def test_permission_manager(mock_requests):
+    # permission_manager: PermissionManager = PermissionManager()
+    permission_flat_dict = {
+        "metadata.request_count.value": 100000,
+        "metadata.messages.value": True,
+        "metadata.analytics.value": False,
+    }
+    permission_dict = unflatten_dict(permission_flat_dict)
+    assert not permission_dict.get("metadata.request_count.value")
+    mock_requests.json.return_value = permission_dict
+    # random_key = choice(list(permission_flat_dict.keys()))
+    # res = permission_manager.retrieve_permission(
+    #     base_url="https://localhost",
+    #     permission_id=uuid4().hex[:10],
+    #     service="iam"
+    # )
+    # assert res == permission_dict,res
+    # res = permission_manager.retrieve_permission(
+    #     base_url="https://localhost",
+    #     permission_id=uuid4().hex[:10],
+    #     service="iam",
+    #     dot_path=random_key
+    # )
+    # assert res == permission_flat_dict.get(random_key),res
```

### Comparing `django-learngual-0.11/learngual/utils.py` & `django-learngual-0.12/learngual/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Any, Literal
 
 import requests
 from django.core.cache import cache
 
 # from django.utils import timezone
 
+
 def get_service_request_headers(**kwargs) -> dict:
     """function add headers needed for request made from a service
 
     Returns:
         dict: _description_
     """
 
@@ -382,14 +383,15 @@
         res = requests.patch(base_url.rstrip("/") + url_path, json=permmission_data)
         if not res.ok:
             raise requests.exceptions.RequestException(res.content)
         return res.json()
 
     def retrieve_permission(
         self,
+        *,
         base_url: str,
         permission_id,
         service: Literal["iam", "payment", "notify", "learn", "media"] = "iam",
         dot_path: str = None,
     ):
         """_summary_
```

### Comparing `django-learngual-0.11/setup.cfg` & `django-learngual-0.12/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-learngual
-version = 0.11
+version = 0.12
 author = learngual
 author_email = developer@leanrgual.com
 maintainer = Aniekutmfon
 maintainer_email = aniekutmfonekere@gmail.com
 description = Learngual helper package
 long_description = file:README.rst
 long_description_content_type = text/x-rst
```

