# Comparing `tmp/django_cloud_storages-1.1.1.tar.gz` & `tmp/django_cloud_storages-1.1.2.tar.gz`

## Comparing `django_cloud_storages-1.1.1.tar` & `django_cloud_storages-1.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/.readthedocs.yaml
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/manage.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/requirements.txt
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/setup.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/.vscode/settings.json
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/cloud_storages/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/cloud_storages/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/cloud_storages/backends/__init__.py
--rw-r--r--   0        0        0    14076 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/cloud_storages/backends/appwrite.py
--rw-r--r--   0        0        0     8708 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/cloud_storages/backends/dropbox.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/docs/Makefile
--rw-r--r--   0        0        0     8858 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/docs/conf.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/docs/index.rst
--rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/docs/make.bat
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/docs/requirements.txt
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/docs/backends/appwrite.rst
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/docs/backends/dropbox.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/tests/settings.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/tests/test_appwrite.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/tests/test_dropbox.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/tests/test_folder/test_file.txt
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/LICENSE
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/README.md
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/.readthedocs.yaml
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/manage.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/requirements.txt
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/setup.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/.vscode/settings.json
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/cloud_storages/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/cloud_storages/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/cloud_storages/backends/__init__.py
+-rw-r--r--   0        0        0    14076 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/cloud_storages/backends/appwrite.py
+-rw-r--r--   0        0        0     8708 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/cloud_storages/backends/dropbox.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/docs/Makefile
+-rw-r--r--   0        0        0     8858 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/docs/conf.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/docs/index.rst
+-rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/docs/make.bat
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/docs/requirements.txt
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/docs/backends/appwrite.rst
+-rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/docs/backends/dropbox.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/tests/settings.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/tests/test_appwrite.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/tests/test_dropbox.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/tests/test_folder/test_file.txt
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/LICENSE
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/README.md
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/PKG-INFO
```

### Comparing `django_cloud_storages-1.1.1/.readthedocs.yaml` & `django_cloud_storages-1.1.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.1/manage.py` & `django_cloud_storages-1.1.2/manage.py`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.1/requirements.txt` & `django_cloud_storages-1.1.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.1/cloud_storages/utils.py` & `django_cloud_storages-1.1.2/cloud_storages/utils.py`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.1/cloud_storages/backends/appwrite.py` & `django_cloud_storages-1.1.2/cloud_storages/backends/appwrite.py`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.1/cloud_storages/backends/dropbox.py` & `django_cloud_storages-1.1.2/cloud_storages/backends/dropbox.py`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.1/docs/Makefile` & `django_cloud_storages-1.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.1/docs/conf.py` & `django_cloud_storages-1.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.1/docs/index.rst` & `django_cloud_storages-1.1.2/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
    contain the root `toctree` directive.
 
 Welcome to django-cloud-storages's documentation!
 =================================================
 
 django-cloud-storages is a package developed for django to work with cloud storages to store/upload media files.
 
-At the moment this package support the following cloud storage services.
+At the moment this package support the following cloud storage services -
 
 .. toctree::
    :maxdepth: 1
    :glob:
 
    backends/*
```

### Comparing `django_cloud_storages-1.1.1/docs/make.bat` & `django_cloud_storages-1.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.1/docs/backends/appwrite.rst` & `django_cloud_storages-1.1.2/docs/backends/appwrite.rst`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.1/docs/backends/dropbox.rst` & `django_cloud_storages-1.1.2/docs/backends/dropbox.rst`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.1/tests/settings.py` & `django_cloud_storages-1.1.2/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.1/tests/test_appwrite.py` & `django_cloud_storages-1.1.2/tests/test_appwrite.py`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.1/tests/test_dropbox.py` & `django_cloud_storages-1.1.2/tests/test_dropbox.py`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.1/.gitignore` & `django_cloud_storages-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.1/LICENSE` & `django_cloud_storages-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.1/README.md` & `django_cloud_storages-1.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # Welcome to django-cloud-storages's
 
 django-cloud-storages is a package developed for django to work with cloud storages to store/upload media files.
 
 This package extends the [django Storage class](https://docs.djangoproject.com/en/4.2/ref/files/storage/#django.core.files.storage.Storage) to provide file storage in cloud.
 
+At the moment this package support the following cloud storage services -
+
+* AppWrite
+* DropBox
 
 ### **Installation**
 
 ---
 
 Use pip to install from PyPI:
 
    `pip install django-cloud-storages`
 
 It will install all the cloud storage backends (available in this package), you can choose any of the storage backend as per your requirement.
 
 ### **Documentation**
 
-The documentation for the package *django-cloud-storage* is available at [https://django-cloud-storages.readthedocs.io](https://django-cloud-storages.readthedocs.io/)
+The documentation for the package *django-cloud-storage* is available at [https://django-cloud-storages.readthedocs.io](https://django-cloud-storages.readthedocs.io/).
 
 ### **Contributing**
 
 ---
 
 To contribute to django-cloud-storages [create a fork](https://github.com/Samiddha99/django-cloud-storages) on GitHub. Clone your fork, make some changes, and submit a pull request.
```

### Comparing `django_cloud_storages-1.1.1/pyproject.toml` & `django_cloud_storages-1.1.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = ["hatchling", "django", "requests", "dropbox", "appwrite"]
 build-backend = "hatchling.build"
 
 [project]
 name = "django-cloud-storages"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="Samiddha Chakrabarti", email="samiddha99@protonmail.com" },
 ]
 description = "Cloud file storages for django."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Samiddha99/django-cloud-storages"
+"Documentation" = "https://django-cloud-storages.readthedocs.io"
 "Bug Tracker" = "https://github.com/Samiddha99/django-cloud-storages/issues"
```

### Comparing `django_cloud_storages-1.1.1/PKG-INFO` & `django_cloud_storages-1.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: django-cloud-storages
-Version: 1.1.1
+Version: 1.1.2
 Summary: Cloud file storages for django.
 Project-URL: Homepage, https://github.com/Samiddha99/django-cloud-storages
+Project-URL: Documentation, https://django-cloud-storages.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/Samiddha99/django-cloud-storages/issues
 Author-email: Samiddha Chakrabarti <samiddha99@protonmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
@@ -14,28 +15,32 @@
 
 # Welcome to django-cloud-storages's
 
 django-cloud-storages is a package developed for django to work with cloud storages to store/upload media files.
 
 This package extends the [django Storage class](https://docs.djangoproject.com/en/4.2/ref/files/storage/#django.core.files.storage.Storage) to provide file storage in cloud.
 
+At the moment this package support the following cloud storage services -
+
+* AppWrite
+* DropBox
 
 ### **Installation**
 
 ---
 
 Use pip to install from PyPI:
 
    `pip install django-cloud-storages`
 
 It will install all the cloud storage backends (available in this package), you can choose any of the storage backend as per your requirement.
 
 ### **Documentation**
 
-The documentation for the package *django-cloud-storage* is available at [https://django-cloud-storages.readthedocs.io](https://django-cloud-storages.readthedocs.io/)
+The documentation for the package *django-cloud-storage* is available at [https://django-cloud-storages.readthedocs.io](https://django-cloud-storages.readthedocs.io/).
 
 ### **Contributing**
 
 ---
 
 To contribute to django-cloud-storages [create a fork](https://github.com/Samiddha99/django-cloud-storages) on GitHub. Clone your fork, make some changes, and submit a pull request.
```

