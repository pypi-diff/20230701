# Comparing `tmp/django-learngual-0.13.2.tar.gz` & `tmp/django-learngual-0.13.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-learngual-0.13.2.tar", last modified: Sat Jul  1 16:19:59 2023, max compression
+gzip compressed data, was "django-learngual-0.13.3.tar", last modified: Sat Jul  1 17:36:29 2023, max compression
```

## Comparing `django-learngual-0.13.2.tar` & `django-learngual-0.13.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:19:59.387439 django-learngual-0.13.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-01 16:19:01.000000 django-learngual-0.13.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-01 16:19:01.000000 django-learngual-0.13.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-01 16:19:59.387439 django-learngual-0.13.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-01 16:19:01.000000 django-learngual-0.13.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:19:59.383439 django-learngual-0.13.2/django_learngual.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-01 16:19:59.000000 django-learngual-0.13.2/django_learngual.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-01 16:19:59.000000 django-learngual-0.13.2/django_learngual.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 16:19:59.000000 django-learngual-0.13.2/django_learngual.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 16:19:59.000000 django-learngual-0.13.2/django_learngual.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:19:59.383439 django-learngual-0.13.2/learngual/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:19:54.000000 django-learngual-0.13.2/learngual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:19:54.000000 django-learngual-0.13.2/learngual/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:19:59.383439 django-learngual-0.13.2/learngual/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:19:54.000000 django-learngual-0.13.2/learngual/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:19:54.000000 django-learngual-0.13.2/learngual/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-01 16:19:54.000000 django-learngual-0.13.2/learngual/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-07-01 16:19:54.000000 django-learngual-0.13.2/learngual/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-01 16:19:54.000000 django-learngual-0.13.2/learngual/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:19:59.383439 django-learngual-0.13.2/learngual/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:19:54.000000 django-learngual-0.13.2/learngual/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:19:54.000000 django-learngual-0.13.2/learngual/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-01 16:19:54.000000 django-learngual-0.13.2/learngual/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:19:54.000000 django-learngual-0.13.2/learngual/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:19:59.387439 django-learngual-0.13.2/learngual/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:19:54.000000 django-learngual-0.13.2/learngual/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:19:54.000000 django-learngual-0.13.2/learngual/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-01 16:19:54.000000 django-learngual-0.13.2/learngual/tests/request_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-01 16:19:54.000000 django-learngual-0.13.2/learngual/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:19:54.000000 django-learngual-0.13.2/learngual/tests/test_drf_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-01 16:19:54.000000 django-learngual-0.13.2/learngual/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-01 16:19:54.000000 django-learngual-0.13.2/learngual/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    13817 2023-07-01 16:19:54.000000 django-learngual-0.13.2/learngual/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-01 16:19:59.387439 django-learngual-0.13.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 16:19:01.000000 django-learngual-0.13.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:29.346193 django-learngual-0.13.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-01 17:35:38.000000 django-learngual-0.13.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-01 17:35:38.000000 django-learngual-0.13.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-01 17:36:29.346193 django-learngual-0.13.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-01 17:35:38.000000 django-learngual-0.13.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:29.346193 django-learngual-0.13.3/django_learngual.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-01 17:36:29.000000 django-learngual-0.13.3/django_learngual.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-01 17:36:29.000000 django-learngual-0.13.3/django_learngual.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 17:36:29.000000 django-learngual-0.13.3/django_learngual.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 17:36:29.000000 django-learngual-0.13.3/django_learngual.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:29.346193 django-learngual-0.13.3/learngual/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:29.346193 django-learngual-0.13.3/learngual/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:29.346193 django-learngual-0.13.3/learngual/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:29.346193 django-learngual-0.13.3/learngual/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/tests/request_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/tests/test_drf_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13825 2023-07-01 17:36:25.000000 django-learngual-0.13.3/learngual/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-01 17:36:29.346193 django-learngual-0.13.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 17:35:38.000000 django-learngual-0.13.3/setup.py
```

### Comparing `django-learngual-0.13.2/LICENSE` & `django-learngual-0.13.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.2/PKG-INFO` & `django-learngual-0.13.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-learngual
-Version: 0.13.2
+Version: 0.13.3
 Summary: Learngual helper package
 Home-page: https://learngual.com
 Author: learngual
 Author-email: developer@leanrgual.com
 Maintainer: Aniekutmfon
 Maintainer-email: aniekutmfonekere@gmail.com
 License: Proprietary Software License Agreement
```

### Comparing `django-learngual-0.13.2/README.rst` & `django-learngual-0.13.3/README.rst`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.2/django_learngual.egg-info/PKG-INFO` & `django-learngual-0.13.3/django_learngual.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-learngual
-Version: 0.13.2
+Version: 0.13.3
 Summary: Learngual helper package
 Home-page: https://learngual.com
 Author: learngual
 Author-email: developer@leanrgual.com
 Maintainer: Aniekutmfon
 Maintainer-email: aniekutmfonekere@gmail.com
 License: Proprietary Software License Agreement
```

### Comparing `django-learngual-0.13.2/django_learngual.egg-info/SOURCES.txt` & `django-learngual-0.13.3/django_learngual.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.2/learngual/authentication.py` & `django-learngual-0.13.3/learngual/authentication.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         #     "am here ooo %s" % dict(LEARNGUAL_AUTH_TEST_MODE=LEARNGUAL_AUTH_TEST_MODE)
         # )
         # this is for test mode
 
         service_key = str(
             request.META.get("HTTP_SERVICE_KEY", "")
             or request.GET.get("service-key", "")
-            and request.GET.get("_service-key", "")
+            or request.GET.get("_service-key", "")
         )
         if service_key:
             if service_key == LEARNGUAL_SERVICE_API_KEY:
                 service_user = User(id="service", username="service")
                 service_user.is_service = True
                 return service_user, service_key
```

### Comparing `django-learngual-0.13.2/learngual/permissions.py` & `django-learngual-0.13.3/learngual/permissions.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.2/learngual/tests/request_mock.py` & `django-learngual-0.13.3/learngual/tests/request_mock.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.2/learngual/tests/test_authentication.py` & `django-learngual-0.13.3/learngual/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.2/learngual/tests/test_utils.py` & `django-learngual-0.13.3/learngual/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.2/learngual/utils.py` & `django-learngual-0.13.3/learngual/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -438,15 +438,15 @@
             permission_id (str): example: '123456', 'sdGh66gGGHgfadsty', 'product:1234567'
             service (_type_): "iam" | "pay" | "notify" | "learn" | "media"
             base_url (str):
             dot_path (str):Default:None, e.g metadata.request_count.value
             headers (dict):Default:{}
             params (str):Default:"", e.g name=ann&age=102
         """
-        url_path = f"/{service}/v1/permission/{permission_id}/"
+        url_path = f"/{service}/v1/service/permission/{permission_id}/"
         data = cache.get(url_path)
 
         params = params.strip("?")
         params = dict([x.split("=") for x in params.split("&") if x])
 
         if not data:
             res = requests.get(
```

### Comparing `django-learngual-0.13.2/setup.cfg` & `django-learngual-0.13.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-learngual
-version = 0.13.2
+version = 0.13.3
 author = learngual
 author_email = developer@leanrgual.com
 maintainer = Aniekutmfon
 maintainer_email = aniekutmfonekere@gmail.com
 description = Learngual helper package
 long_description = file:README.rst
 long_description_content_type = text/x-rst
```

