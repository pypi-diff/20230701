# Comparing `tmp/django-sso-client-0.0.8.tar.gz` & `tmp/django-sso-client-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sso-client-0.0.8.tar", last modified: Fri Jun 23 20:06:18 2023, max compression
+gzip compressed data, was "django-sso-client-0.0.9.tar", last modified: Fri Jun 30 22:54:42 2023, max compression
```

## Comparing `django-sso-client-0.0.8.tar` & `django-sso-client-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,33 @@
-drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-23 20:06:18.007540 django-sso-client-0.0.8/
--rw-rw-r--   0 israel    (1000) israel    (1000)       38 2023-06-01 22:36:35.000000 django-sso-client-0.0.8/LICENSE.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)      958 2023-06-23 20:06:18.007540 django-sso-client-0.0.8/PKG-INFO
--rw-rw-r--   0 israel    (1000) israel    (1000)     1663 2023-06-07 13:14:46.000000 django-sso-client-0.0.8/README.md
-drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-23 20:06:18.007540 django-sso-client-0.0.8/django_client_sso/
--rw-rw-r--   0 israel    (1000) israel    (1000)       31 2023-06-02 17:02:09.000000 django-sso-client-0.0.8/django_client_sso/__init__.py
--rw-rw-r--   0 israel    (1000) israel    (1000)     1741 2023-06-02 19:03:13.000000 django-sso-client-0.0.8/django_client_sso/client_base.py
--rw-rw-r--   0 israel    (1000) israel    (1000)      386 2023-06-07 13:12:36.000000 django-sso-client-0.0.8/django_client_sso/client_office365.py
--rw-rw-r--   0 israel    (1000) israel    (1000)     2356 2023-06-23 20:05:23.000000 django-sso-client-0.0.8/django_client_sso/decorators.py
--rw-rw-r--   0 israel    (1000) israel    (1000)      361 2023-06-02 19:33:03.000000 django-sso-client-0.0.8/django_client_sso/exceptions.py
--rw-rw-r--   0 israel    (1000) israel    (1000)      700 2023-06-02 19:35:23.000000 django-sso-client-0.0.8/django_client_sso/handlers.py
-drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-23 20:06:18.007540 django-sso-client-0.0.8/django_sso_client.egg-info/
--rw-rw-r--   0 israel    (1000) israel    (1000)      958 2023-06-23 20:06:17.000000 django-sso-client-0.0.8/django_sso_client.egg-info/PKG-INFO
--rw-rw-r--   0 israel    (1000) israel    (1000)      399 2023-06-23 20:06:17.000000 django-sso-client-0.0.8/django_sso_client.egg-info/SOURCES.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)        1 2023-06-23 20:06:17.000000 django-sso-client-0.0.8/django_sso_client.egg-info/dependency_links.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)       18 2023-06-23 20:06:17.000000 django-sso-client-0.0.8/django_sso_client.egg-info/top_level.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)      106 2023-06-23 20:06:18.007540 django-sso-client-0.0.8/setup.cfg
--rw-rw-r--   0 israel    (1000) israel    (1000)     1076 2023-06-23 20:05:45.000000 django-sso-client-0.0.8/setup.py
+drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-30 22:54:42.313200 django-sso-client-0.0.9/
+-rw-rw-r--   0 israel    (1000) israel    (1000)       38 2023-06-01 22:36:35.000000 django-sso-client-0.0.9/LICENSE.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)     1012 2023-06-30 22:54:42.313200 django-sso-client-0.0.9/PKG-INFO
+-rw-rw-r--   0 israel    (1000) israel    (1000)     1663 2023-06-07 13:14:46.000000 django-sso-client-0.0.9/README.md
+drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-30 22:54:42.309200 django-sso-client-0.0.9/django_azure/
+-rw-rw-r--   0 israel    (1000) israel    (1000)       26 2023-06-30 21:19:08.000000 django-sso-client-0.0.9/django_azure/__init__.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)     2354 2023-06-30 21:44:01.000000 django-sso-client-0.0.9/django_azure/blob_storage.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)     2440 2023-06-30 22:03:52.000000 django-sso-client-0.0.9/django_azure/event_hubs.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)     3267 2023-06-30 22:06:03.000000 django-sso-client-0.0.9/django_azure/table_storage.py
+drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-30 22:54:42.309200 django-sso-client-0.0.9/django_client_db/
+-rw-rw-r--   0 israel    (1000) israel    (1000)       30 2023-06-30 21:16:32.000000 django-sso-client-0.0.9/django_client_db/__init__.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)     2056 2023-06-30 16:18:59.000000 django-sso-client-0.0.9/django_client_db/base_seeder.py
+drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-30 22:54:42.309200 django-sso-client-0.0.9/django_client_mail/
+-rw-rw-r--   0 israel    (1000) israel    (1000)       44 2023-06-30 21:27:09.000000 django-sso-client-0.0.9/django_client_mail/__init__.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)      229 2023-06-30 21:27:01.000000 django-sso-client-0.0.9/django_client_mail/email_service.py
+drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-30 22:54:42.309200 django-sso-client-0.0.9/django_client_sso/
+-rw-rw-r--   0 israel    (1000) israel    (1000)       32 2023-06-30 21:35:39.000000 django-sso-client-0.0.9/django_client_sso/__init__.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)     1716 2023-06-30 22:07:33.000000 django-sso-client-0.0.9/django_client_sso/client_base.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)      386 2023-06-07 13:12:36.000000 django-sso-client-0.0.9/django_client_sso/client_office365.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)     2356 2023-06-23 20:05:23.000000 django-sso-client-0.0.9/django_client_sso/decorators.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)      361 2023-06-02 19:33:03.000000 django-sso-client-0.0.9/django_client_sso/exceptions.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)      700 2023-06-30 22:35:24.000000 django-sso-client-0.0.9/django_client_sso/handlers.py
+drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-30 22:54:42.309200 django-sso-client-0.0.9/django_sso_client.egg-info/
+-rw-rw-r--   0 israel    (1000) israel    (1000)     1012 2023-06-30 22:54:42.000000 django-sso-client-0.0.9/django_sso_client.egg-info/PKG-INFO
+-rw-rw-r--   0 israel    (1000) israel    (1000)      717 2023-06-30 22:54:42.000000 django-sso-client-0.0.9/django_sso_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)        1 2023-06-30 22:54:42.000000 django-sso-client-0.0.9/django_sso_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)       80 2023-06-30 22:54:42.000000 django-sso-client-0.0.9/django_sso_client.egg-info/top_level.txt
+drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-06-30 22:54:42.313200 django-sso-client-0.0.9/django_utils/
+-rw-rw-r--   0 israel    (1000) israel    (1000)       26 2023-06-30 21:16:59.000000 django-sso-client-0.0.9/django_utils/__init__.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)      365 2023-06-30 19:52:08.000000 django-sso-client-0.0.9/django_utils/local_file.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)      551 2023-06-30 22:44:18.000000 django-sso-client-0.0.9/django_utils/logger_app.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)      106 2023-06-30 22:54:42.313200 django-sso-client-0.0.9/setup.cfg
+-rw-rw-r--   0 israel    (1000) israel    (1000)     1200 2023-06-30 22:54:28.000000 django-sso-client-0.0.9/setup.py
```

### Comparing `django-sso-client-0.0.8/PKG-INFO` & `django-sso-client-0.0.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: django-sso-client
-Version: 0.0.8
-Summary: Client for Django Apps - SSO TIT/Hyper by P&D
+Version: 0.0.9
+Summary: Client for Django Apps - TIT/Hyper by P&D
 Home-page: https://TITBrasil@dev.azure.com/TITBrasil/TITCS%20-%20Live4Safe/_git/DJANGO_CLIENT
 Author: TIT CS
 Author-email: contato@titcs.com.br
 License: MIT
 Project-URL: Código fonte, https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT
 Project-URL: Download, https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT
-Keywords: django_client_sso
+Keywords: django_client_sso django_azure django_client_db django_client_mail django_utils
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Internationalization
 Classifier: Topic :: Scientific/Engineering :: Physics
 License-File: LICENSE.txt
 
-Client for Django Apps - SSO TIT/Hyper by P&D
+Client for Django Apps - TIT/Hyper by P&D
```

### Comparing `django-sso-client-0.0.8/README.md` & `django-sso-client-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `django-sso-client-0.0.8/django_client_sso/client_base.py` & `django-sso-client-0.0.9/django_client_sso/client_base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import requests
 import jwt
 import tempfile
 import json
-from os import path
-from django.conf import settings
+from os import path, getenv
 from django_client_sso.exceptions import Exception401
 
 class ClientBase():
     
     def __init__(self) -> None:
         self.host = settings.SSO_HOST
         self.client = settings.CLIENT_ID
```

### Comparing `django-sso-client-0.0.8/django_client_sso/decorators.py` & `django-sso-client-0.0.9/django_client_sso/decorators.py`

 * *Files identical despite different names*

### Comparing `django-sso-client-0.0.8/django_client_sso/handlers.py` & `django-sso-client-0.0.9/django_client_sso/handlers.py`

 * *Files identical despite different names*

### Comparing `django-sso-client-0.0.8/django_sso_client.egg-info/PKG-INFO` & `django-sso-client-0.0.9/django_sso_client.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: django-sso-client
-Version: 0.0.8
-Summary: Client for Django Apps - SSO TIT/Hyper by P&D
+Version: 0.0.9
+Summary: Client for Django Apps - TIT/Hyper by P&D
 Home-page: https://TITBrasil@dev.azure.com/TITBrasil/TITCS%20-%20Live4Safe/_git/DJANGO_CLIENT
 Author: TIT CS
 Author-email: contato@titcs.com.br
 License: MIT
 Project-URL: Código fonte, https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT
 Project-URL: Download, https://TITBrasil@dev.azure.com/TITBrasil/Gamefica/_git/DJANGO_CLIENT
-Keywords: django_client_sso
+Keywords: django_client_sso django_azure django_client_db django_client_mail django_utils
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Internationalization
 Classifier: Topic :: Scientific/Engineering :: Physics
 License-File: LICENSE.txt
 
-Client for Django Apps - SSO TIT/Hyper by P&D
+Client for Django Apps - TIT/Hyper by P&D
```

