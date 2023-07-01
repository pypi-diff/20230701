# Comparing `tmp/django-learngual-0.10.tar.gz` & `tmp/django-learngual-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-learngual-0.10.tar", last modified: Sat Jul  1 01:38:43 2023, max compression
+gzip compressed data, was "django-learngual-0.11.tar", last modified: Sat Jul  1 01:57:40 2023, max compression
```

## Comparing `django-learngual-0.10.tar` & `django-learngual-0.11.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 01:38:43.159846 django-learngual-0.10/
--rw-r--r--   0 user       (501) staff       (20)     2901 2023-07-01 00:27:10.000000 django-learngual-0.10/LICENSE
--rw-r--r--   0 user       (501) staff       (20)      105 2023-07-01 00:32:47.000000 django-learngual-0.10/MANIFEST.in
--rw-r--r--   0 user       (501) staff       (20)     2516 2023-07-01 01:38:43.160016 django-learngual-0.10/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     1563 2023-07-01 00:43:46.000000 django-learngual-0.10/README.rst
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 01:38:43.147925 django-learngual-0.10/django_learngual.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     2516 2023-07-01 01:38:43.000000 django-learngual-0.10/django_learngual.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      620 2023-07-01 01:38:43.000000 django-learngual-0.10/django_learngual.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-07-01 01:38:43.000000 django-learngual-0.10/django_learngual.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       10 2023-07-01 01:38:43.000000 django-learngual-0.10/django_learngual.egg-info/top_level.txt
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 01:38:43.155295 django-learngual-0.10/learngual/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 01:38:35.000000 django-learngual-0.10/learngual/__init__.py
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 01:38:35.000000 django-learngual-0.10/learngual/admin.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 01:38:43.156380 django-learngual-0.10/learngual/api/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 01:38:35.000000 django-learngual-0.10/learngual/api/serializers.py
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 01:38:35.000000 django-learngual-0.10/learngual/api/views.py
--rw-r--r--   0 user       (501) staff       (20)      312 2023-07-01 01:38:35.000000 django-learngual-0.10/learngual/apps.py
--rw-r--r--   0 user       (501) staff       (20)     4533 2023-07-01 01:38:35.000000 django-learngual-0.10/learngual/auth.py
--rw-r--r--   0 user       (501) staff       (20)      399 2023-07-01 01:38:35.000000 django-learngual-0.10/learngual/manager.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 01:38:43.156756 django-learngual-0.10/learngual/migrations/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 01:38:35.000000 django-learngual-0.10/learngual/migrations/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    15755 2023-07-01 01:38:35.000000 django-learngual-0.10/learngual/models.py
--rw-r--r--   0 user       (501) staff       (20)      642 2023-07-01 01:38:35.000000 django-learngual-0.10/learngual/permissions.py
--rw-r--r--   0 user       (501) staff       (20)     2215 2023-07-01 01:38:35.000000 django-learngual-0.10/learngual/signals.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 01:38:43.159437 django-learngual-0.10/learngual/tests/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 01:38:35.000000 django-learngual-0.10/learngual/tests/__init__.py
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 01:38:35.000000 django-learngual-0.10/learngual/tests/factories.py
--rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 01:38:35.000000 django-learngual-0.10/learngual/tests/test_drf_endpoints.py
--rw-r--r--   0 user       (501) staff       (20)     5394 2023-07-01 01:38:35.000000 django-learngual-0.10/learngual/tests/test_utils.py
--rw-r--r--   0 user       (501) staff       (20)      305 2023-07-01 01:38:35.000000 django-learngual-0.10/learngual/urls.py
--rw-r--r--   0 user       (501) staff       (20)    12039 2023-07-01 01:38:35.000000 django-learngual-0.10/learngual/utils.py
--rw-r--r--   0 user       (501) staff       (20)      972 2023-07-01 01:38:43.160832 django-learngual-0.10/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)       38 2023-07-01 00:39:27.000000 django-learngual-0.10/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 01:57:40.118379 django-learngual-0.11/
+-rw-r--r--   0 user       (501) staff       (20)     2901 2023-07-01 00:27:10.000000 django-learngual-0.11/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)      105 2023-07-01 00:32:47.000000 django-learngual-0.11/MANIFEST.in
+-rw-r--r--   0 user       (501) staff       (20)     1893 2023-07-01 01:57:40.121263 django-learngual-0.11/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      940 2023-07-01 01:54:06.000000 django-learngual-0.11/README.rst
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 01:57:40.068234 django-learngual-0.11/django_learngual.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     1893 2023-07-01 01:57:39.000000 django-learngual-0.11/django_learngual.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      620 2023-07-01 01:57:40.000000 django-learngual-0.11/django_learngual.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-07-01 01:57:39.000000 django-learngual-0.11/django_learngual.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       10 2023-07-01 01:57:39.000000 django-learngual-0.11/django_learngual.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 01:57:40.097022 django-learngual-0.11/learngual/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 01:57:30.000000 django-learngual-0.11/learngual/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 01:57:30.000000 django-learngual-0.11/learngual/admin.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 01:57:40.113898 django-learngual-0.11/learngual/api/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 01:57:31.000000 django-learngual-0.11/learngual/api/serializers.py
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 01:57:31.000000 django-learngual-0.11/learngual/api/views.py
+-rw-r--r--   0 user       (501) staff       (20)      312 2023-07-01 01:57:30.000000 django-learngual-0.11/learngual/apps.py
+-rw-r--r--   0 user       (501) staff       (20)     4533 2023-07-01 01:57:30.000000 django-learngual-0.11/learngual/auth.py
+-rw-r--r--   0 user       (501) staff       (20)      399 2023-07-01 01:57:31.000000 django-learngual-0.11/learngual/manager.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 01:57:40.115155 django-learngual-0.11/learngual/migrations/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 01:57:30.000000 django-learngual-0.11/learngual/migrations/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    15755 2023-07-01 01:57:30.000000 django-learngual-0.11/learngual/models.py
+-rw-r--r--   0 user       (501) staff       (20)      642 2023-07-01 01:57:31.000000 django-learngual-0.11/learngual/permissions.py
+-rw-r--r--   0 user       (501) staff       (20)     2215 2023-07-01 01:57:30.000000 django-learngual-0.11/learngual/signals.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-01 01:57:40.117957 django-learngual-0.11/learngual/tests/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 01:57:30.000000 django-learngual-0.11/learngual/tests/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 01:57:30.000000 django-learngual-0.11/learngual/tests/factories.py
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-07-01 01:57:30.000000 django-learngual-0.11/learngual/tests/test_drf_endpoints.py
+-rw-r--r--   0 user       (501) staff       (20)     5394 2023-07-01 01:57:30.000000 django-learngual-0.11/learngual/tests/test_utils.py
+-rw-r--r--   0 user       (501) staff       (20)      305 2023-07-01 01:57:31.000000 django-learngual-0.11/learngual/urls.py
+-rw-r--r--   0 user       (501) staff       (20)    12039 2023-07-01 01:57:30.000000 django-learngual-0.11/learngual/utils.py
+-rw-r--r--   0 user       (501) staff       (20)      972 2023-07-01 01:57:40.123781 django-learngual-0.11/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-07-01 00:39:27.000000 django-learngual-0.11/setup.py
```

### Comparing `django-learngual-0.10/LICENSE` & `django-learngual-0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `django-learngual-0.10/PKG-INFO` & `django-learngual-0.11/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-learngual
-Version: 0.10
+Version: 0.11
 Summary: Learngual helper package
 Home-page: https://learngual.com
 Author: learngual
 Author-email: developer@leanrgual.com
 Maintainer: Aniekutmfon
 Maintainer-email: aniekutmfonekere@gmail.com
 License: Proprietary Software License Agreement
@@ -20,66 +20,54 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ====================================
-Your Django Package Name
+Learngual Django
 ====================================
 
 .. image:: https://img.shields.io/pypi/v/your-package.svg
     :target: https://pypi.python.org/pypi/your-package
 
 .. image:: https://img.shields.io/travis/your-username/your-package.svg
     :target: https://travis-ci.org/your-username/your-package
 
 Overview
 --------
 
-Your Django Package Name is a Python package that provides [brief description of your package's functionality].
+Learngual is a Python package that provides helper functions for learngual.
 
 Features
 --------
 
-- [Feature 1]
-- [Feature 2]
-- [Feature 3]
-- ...
+.. - [Feature 1]
+.. - [Feature 2]
+.. - [Feature 3]
+.. - ...
 
 Installation
 ------------
 
 You can install Your Django Package Name using pip:
 
 .. code-block:: bash
 
-    $ pip install your-package
+    $ pip install django-learngual
 
 Usage
 -----
 
-[Provide examples and code snippets demonstrating how to use your package.]
+.. [Provide examples and code snippets demonstrating how to use your package.]
 
-Contributing
-------------
-
-We welcome contributions from the community! If you would like to contribute to Your Django Package Name, please follow these guidelines:
-
-1. Fork the repository and clone it to your local machine.
-2. Create a new branch for your feature or bug fix.
-3. Make your changes and commit them with descriptive messages.
-4. Push your changes to your forked repository.
-5. Submit a pull request to the main repository.
-
-Please ensure that your code adheres to our coding standards and is accompanied by tests.
 
 License
 -------
 
-Your Django Package Name is licensed under the [name of the license]. See the [LICENSE](LICENSE) file for more details.
+Django Learngual  is licensed under the MIT.
 
 Contact
 -------
 
-If you have any questions, suggestions, or feedback, please feel free to contact us at [email address].
+If you have any questions, suggestions, or feedback, please feel free to contact us at support@learngual.com.
```

### Comparing `django-learngual-0.10/django_learngual.egg-info/PKG-INFO` & `django-learngual-0.11/django_learngual.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-learngual
-Version: 0.10
+Version: 0.11
 Summary: Learngual helper package
 Home-page: https://learngual.com
 Author: learngual
 Author-email: developer@leanrgual.com
 Maintainer: Aniekutmfon
 Maintainer-email: aniekutmfonekere@gmail.com
 License: Proprietary Software License Agreement
@@ -20,66 +20,54 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ====================================
-Your Django Package Name
+Learngual Django
 ====================================
 
 .. image:: https://img.shields.io/pypi/v/your-package.svg
     :target: https://pypi.python.org/pypi/your-package
 
 .. image:: https://img.shields.io/travis/your-username/your-package.svg
     :target: https://travis-ci.org/your-username/your-package
 
 Overview
 --------
 
-Your Django Package Name is a Python package that provides [brief description of your package's functionality].
+Learngual is a Python package that provides helper functions for learngual.
 
 Features
 --------
 
-- [Feature 1]
-- [Feature 2]
-- [Feature 3]
-- ...
+.. - [Feature 1]
+.. - [Feature 2]
+.. - [Feature 3]
+.. - ...
 
 Installation
 ------------
 
 You can install Your Django Package Name using pip:
 
 .. code-block:: bash
 
-    $ pip install your-package
+    $ pip install django-learngual
 
 Usage
 -----
 
-[Provide examples and code snippets demonstrating how to use your package.]
+.. [Provide examples and code snippets demonstrating how to use your package.]
 
-Contributing
-------------
-
-We welcome contributions from the community! If you would like to contribute to Your Django Package Name, please follow these guidelines:
-
-1. Fork the repository and clone it to your local machine.
-2. Create a new branch for your feature or bug fix.
-3. Make your changes and commit them with descriptive messages.
-4. Push your changes to your forked repository.
-5. Submit a pull request to the main repository.
-
-Please ensure that your code adheres to our coding standards and is accompanied by tests.
 
 License
 -------
 
-Your Django Package Name is licensed under the [name of the license]. See the [LICENSE](LICENSE) file for more details.
+Django Learngual  is licensed under the MIT.
 
 Contact
 -------
 
-If you have any questions, suggestions, or feedback, please feel free to contact us at [email address].
+If you have any questions, suggestions, or feedback, please feel free to contact us at support@learngual.com.
```

### Comparing `django-learngual-0.10/django_learngual.egg-info/SOURCES.txt` & `django-learngual-0.11/django_learngual.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-learngual-0.10/learngual/auth.py` & `django-learngual-0.11/learngual/auth.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.10/learngual/models.py` & `django-learngual-0.11/learngual/models.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.10/learngual/permissions.py` & `django-learngual-0.11/learngual/permissions.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.10/learngual/signals.py` & `django-learngual-0.11/learngual/signals.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.10/learngual/tests/test_utils.py` & `django-learngual-0.11/learngual/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.10/learngual/utils.py` & `django-learngual-0.11/learngual/utils.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.10/setup.cfg` & `django-learngual-0.11/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-learngual
-version = 0.10
+version = 0.11
 author = learngual
 author_email = developer@leanrgual.com
 maintainer = Aniekutmfon
 maintainer_email = aniekutmfonekere@gmail.com
 description = Learngual helper package
 long_description = file:README.rst
 long_description_content_type = text/x-rst
```

