# Comparing `tmp/django-email-accounts-0.2.0.tar.gz` & `tmp/django-email-accounts-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-email-accounts-0.2.0.tar", last modified: Fri Jun 30 01:06:29 2023, max compression
+gzip compressed data, was "django-email-accounts-0.3.0.tar", last modified: Sat Jul  1 12:12:43 2023, max compression
```

## Comparing `django-email-accounts-0.2.0.tar` & `django-email-accounts-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2023-06-30 01:06:29.972272 django-email-accounts-0.2.0/
--rw-r--r--   0 fathi     (1000) fathi     (1000)    35149 2023-06-16 23:14:41.000000 django-email-accounts-0.2.0/LICENSE
--rw-r--r--   0 fathi     (1000) fathi     (1000)     3562 2023-06-30 01:06:29.972272 django-email-accounts-0.2.0/PKG-INFO
--rw-r--r--   0 fathi     (1000) fathi     (1000)     2802 2023-06-30 01:03:04.000000 django-email-accounts-0.2.0/README.md
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2023-06-30 01:06:29.970272 django-email-accounts-0.2.0/django_email_accounts.egg-info/
--rw-r--r--   0 fathi     (1000) fathi     (1000)     3562 2023-06-30 01:06:29.000000 django-email-accounts-0.2.0/django_email_accounts.egg-info/PKG-INFO
--rw-r--r--   0 fathi     (1000) fathi     (1000)      500 2023-06-30 01:06:29.000000 django-email-accounts-0.2.0/django_email_accounts.egg-info/SOURCES.txt
--rw-r--r--   0 fathi     (1000) fathi     (1000)        1 2023-06-30 01:06:29.000000 django-email-accounts-0.2.0/django_email_accounts.egg-info/dependency_links.txt
--rw-r--r--   0 fathi     (1000) fathi     (1000)       88 2023-06-30 01:06:29.000000 django-email-accounts-0.2.0/django_email_accounts.egg-info/requires.txt
--rw-r--r--   0 fathi     (1000) fathi     (1000)       15 2023-06-30 01:06:29.000000 django-email-accounts-0.2.0/django_email_accounts.egg-info/top_level.txt
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2023-06-30 01:06:29.972272 django-email-accounts-0.2.0/email_accounts/
--rw-r--r--   0 fathi     (1000) fathi     (1000)        0 2023-06-16 22:57:01.000000 django-email-accounts-0.2.0/email_accounts/__init__.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)      851 2023-06-16 23:36:24.000000 django-email-accounts-0.2.0/email_accounts/admin.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)      159 2023-06-16 23:39:48.000000 django-email-accounts-0.2.0/email_accounts/apps.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)      252 2023-06-16 23:44:36.000000 django-email-accounts-0.2.0/email_accounts/filters.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)      227 2023-06-16 23:38:04.000000 django-email-accounts-0.2.0/email_accounts/forms.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)     1773 2023-06-16 23:29:23.000000 django-email-accounts-0.2.0/email_accounts/models.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)      281 2023-06-16 23:45:27.000000 django-email-accounts-0.2.0/email_accounts/serializers.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)     1621 2023-06-30 00:43:38.000000 django-email-accounts-0.2.0/email_accounts/urls.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)        0 2023-06-16 22:58:48.000000 django-email-accounts-0.2.0/email_accounts/utils.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)      441 2023-06-16 23:42:17.000000 django-email-accounts-0.2.0/email_accounts/views.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)       38 2023-06-30 01:06:29.972272 django-email-accounts-0.2.0/setup.cfg
--rw-r--r--   0 fathi     (1000) fathi     (1000)     1125 2023-06-30 01:03:52.000000 django-email-accounts-0.2.0/setup.py
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2023-07-01 12:12:43.264272 django-email-accounts-0.3.0/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)    35149 2023-06-16 23:14:41.000000 django-email-accounts-0.3.0/LICENSE
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     4032 2023-07-01 12:12:43.264272 django-email-accounts-0.3.0/PKG-INFO
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     3272 2023-07-01 12:02:33.000000 django-email-accounts-0.3.0/README.md
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2023-07-01 12:12:43.261272 django-email-accounts-0.3.0/django_email_accounts.egg-info/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     4032 2023-07-01 12:12:43.000000 django-email-accounts-0.3.0/django_email_accounts.egg-info/PKG-INFO
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      527 2023-07-01 12:12:43.000000 django-email-accounts-0.3.0/django_email_accounts.egg-info/SOURCES.txt
+-rw-r--r--   0 fathi     (1000) fathi     (1000)        1 2023-07-01 12:12:43.000000 django-email-accounts-0.3.0/django_email_accounts.egg-info/dependency_links.txt
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       88 2023-07-01 12:12:43.000000 django-email-accounts-0.3.0/django_email_accounts.egg-info/requires.txt
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       15 2023-07-01 12:12:43.000000 django-email-accounts-0.3.0/django_email_accounts.egg-info/top_level.txt
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2023-07-01 12:12:43.263272 django-email-accounts-0.3.0/email_accounts/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)        0 2023-06-16 22:57:01.000000 django-email-accounts-0.3.0/email_accounts/__init__.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      851 2023-06-16 23:36:24.000000 django-email-accounts-0.3.0/email_accounts/admin.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      354 2023-07-01 11:51:08.000000 django-email-accounts-0.3.0/email_accounts/api_urls.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      159 2023-06-16 23:39:48.000000 django-email-accounts-0.3.0/email_accounts/apps.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      252 2023-06-16 23:44:36.000000 django-email-accounts-0.3.0/email_accounts/filters.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      227 2023-06-16 23:38:04.000000 django-email-accounts-0.3.0/email_accounts/forms.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     1773 2023-06-16 23:29:23.000000 django-email-accounts-0.3.0/email_accounts/models.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      566 2023-07-01 11:51:39.000000 django-email-accounts-0.3.0/email_accounts/serializers.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     1621 2023-06-30 00:43:38.000000 django-email-accounts-0.3.0/email_accounts/urls.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)        0 2023-06-16 22:58:48.000000 django-email-accounts-0.3.0/email_accounts/utils.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     5212 2023-07-01 12:10:33.000000 django-email-accounts-0.3.0/email_accounts/views.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       38 2023-07-01 12:12:43.264272 django-email-accounts-0.3.0/setup.cfg
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     1125 2023-07-01 11:58:35.000000 django-email-accounts-0.3.0/setup.py
```

### Comparing `django-email-accounts-0.2.0/LICENSE` & `django-email-accounts-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-email-accounts-0.2.0/PKG-INFO` & `django-email-accounts-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-email-accounts
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Django app for user management with email-based authentication.
 Home-page: https://github.com/fathiabdelmalek/django-email-accounts
 Author: Fathi Abdelmalek
 Author-email: abdelmalek.fathi.2001@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
@@ -44,36 +44,55 @@
 
 2. Change the default authentication user model by adding this line of code in your Django project's `settings.py` file:
 
 ```python
 AUTH_USER_MODEL = 'email_accounts.User'
 ```
 
-3. Update your project's `urls.py` file to include the email-accounts URLs:
-
+3. Update your project's `urls.py` file to include the email-accounts URLs: 
+ 
 ```python
 from django.urls import path, include
 
 urlpatterns = [
     ...
     path('accounts/', include('email_accounts.urls')),
     ...
 ]
 ```
 
+<b>Note : </b>If you want to use the restfull api instead, then here is a propre update for `urls.py`:
+
+```python
+from django.urls import path, include
+from rest_framework.routers import DefaultRouter
+
+from email_accounts.views import UserViewSet
+
+router = DefaultRouter()
+router.register('users', UserViewSet)
+
+urlpatterns = [
+    ...
+    path('api/', include(router.urls)),
+    path('api/accounts', include('email_accounts.api_urls')),
+    ...
+]
+```
+
 4. Run migrations to create the necessary database tables:
 
 ```shell
 python manage.py makemigrations email_accounts
 python manage.py migrate
 ```
 
 6. You can now use the email-accounts functionality in your Django project.
 
-If you want custom authentication templates, then, in your templates folder, create a `email_accounts` subdirectory in `templates` directory and create all authentication templates on it like this.
+<b>Note : </b> If you want custom authentication templates, then, in your templates folder, create a `email_accounts` subdirectory in `templates` directory and create all authentication templates on it like this.
 
 ```bash
 ├── templates
 │   └── email_accounts
 │       ├── login.html
 │       ├── register.html
 │       └── password
```

### Comparing `django-email-accounts-0.2.0/README.md` & `django-email-accounts-0.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -24,36 +24,55 @@
 
 2. Change the default authentication user model by adding this line of code in your Django project's `settings.py` file:
 
 ```python
 AUTH_USER_MODEL = 'email_accounts.User'
 ```
 
-3. Update your project's `urls.py` file to include the email-accounts URLs:
-
+3. Update your project's `urls.py` file to include the email-accounts URLs: 
+ 
 ```python
 from django.urls import path, include
 
 urlpatterns = [
     ...
     path('accounts/', include('email_accounts.urls')),
     ...
 ]
 ```
 
+<b>Note : </b>If you want to use the restfull api instead, then here is a propre update for `urls.py`:
+
+```python
+from django.urls import path, include
+from rest_framework.routers import DefaultRouter
+
+from email_accounts.views import UserViewSet
+
+router = DefaultRouter()
+router.register('users', UserViewSet)
+
+urlpatterns = [
+    ...
+    path('api/', include(router.urls)),
+    path('api/accounts', include('email_accounts.api_urls')),
+    ...
+]
+```
+
 4. Run migrations to create the necessary database tables:
 
 ```shell
 python manage.py makemigrations email_accounts
 python manage.py migrate
 ```
 
 6. You can now use the email-accounts functionality in your Django project.
 
-If you want custom authentication templates, then, in your templates folder, create a `email_accounts` subdirectory in `templates` directory and create all authentication templates on it like this.
+<b>Note : </b> If you want custom authentication templates, then, in your templates folder, create a `email_accounts` subdirectory in `templates` directory and create all authentication templates on it like this.
 
 ```bash
 ├── templates
 │   └── email_accounts
 │       ├── login.html
 │       ├── register.html
 │       └── password
```

### Comparing `django-email-accounts-0.2.0/django_email_accounts.egg-info/PKG-INFO` & `django-email-accounts-0.3.0/django_email_accounts.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-email-accounts
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Django app for user management with email-based authentication.
 Home-page: https://github.com/fathiabdelmalek/django-email-accounts
 Author: Fathi Abdelmalek
 Author-email: abdelmalek.fathi.2001@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
@@ -44,36 +44,55 @@
 
 2. Change the default authentication user model by adding this line of code in your Django project's `settings.py` file:
 
 ```python
 AUTH_USER_MODEL = 'email_accounts.User'
 ```
 
-3. Update your project's `urls.py` file to include the email-accounts URLs:
-
+3. Update your project's `urls.py` file to include the email-accounts URLs: 
+ 
 ```python
 from django.urls import path, include
 
 urlpatterns = [
     ...
     path('accounts/', include('email_accounts.urls')),
     ...
 ]
 ```
 
+<b>Note : </b>If you want to use the restfull api instead, then here is a propre update for `urls.py`:
+
+```python
+from django.urls import path, include
+from rest_framework.routers import DefaultRouter
+
+from email_accounts.views import UserViewSet
+
+router = DefaultRouter()
+router.register('users', UserViewSet)
+
+urlpatterns = [
+    ...
+    path('api/', include(router.urls)),
+    path('api/accounts', include('email_accounts.api_urls')),
+    ...
+]
+```
+
 4. Run migrations to create the necessary database tables:
 
 ```shell
 python manage.py makemigrations email_accounts
 python manage.py migrate
 ```
 
 6. You can now use the email-accounts functionality in your Django project.
 
-If you want custom authentication templates, then, in your templates folder, create a `email_accounts` subdirectory in `templates` directory and create all authentication templates on it like this.
+<b>Note : </b> If you want custom authentication templates, then, in your templates folder, create a `email_accounts` subdirectory in `templates` directory and create all authentication templates on it like this.
 
 ```bash
 ├── templates
 │   └── email_accounts
 │       ├── login.html
 │       ├── register.html
 │       └── password
```

### Comparing `django-email-accounts-0.2.0/email_accounts/admin.py` & `django-email-accounts-0.3.0/email_accounts/admin.py`

 * *Files identical despite different names*

### Comparing `django-email-accounts-0.2.0/email_accounts/models.py` & `django-email-accounts-0.3.0/email_accounts/models.py`

 * *Files identical despite different names*

### Comparing `django-email-accounts-0.2.0/email_accounts/urls.py` & `django-email-accounts-0.3.0/email_accounts/urls.py`

 * *Files identical despite different names*

### Comparing `django-email-accounts-0.2.0/setup.py` & `django-email-accounts-0.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 extras_require = {
     "rest_framework": ["djangorestframework>=3.12"],
     "filters": ["django-filter>=2.4"],
 }
 
 setup(
     name='django-email-accounts',
-    version='0.2.0',
+    version='0.3.0',
     author='Fathi Abdelmalek',
     author_email='abdelmalek.fathi.2001@gmail.com',
     description='A Django app for user management with email-based authentication.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/fathiabdelmalek/django-email-accounts',
     packages=find_packages(),
```

