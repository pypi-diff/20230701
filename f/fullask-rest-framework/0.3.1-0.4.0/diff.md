# Comparing `tmp/fullask_rest_framework-0.3.1.tar.gz` & `tmp/fullask_rest_framework-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fullask_rest_framework-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fullask_rest_framework-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fullask_rest_framework-0.3.1.tar` & `fullask_rest_framework-0.4.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      292 2023-06-27 23:53:38.443363 fullask_rest_framework-0.3.1/.editorconfig
--rw-r--r--   0        0        0     1226 2023-06-27 23:53:38.443363 fullask_rest_framework-0.3.1/.gitignore
--rw-r--r--   0        0        0     1070 2023-06-27 23:53:38.443363 fullask_rest_framework-0.3.1/LICENSE
--rw-r--r--   0        0        0     4567 2023-06-27 23:53:38.443363 fullask_rest_framework-0.3.1/README.md
--rw-r--r--   0        0        0      150 2023-06-27 23:53:38.443363 fullask_rest_framework-0.3.1/fullask_rest_framework/__init__.py
--rw-r--r--   0        0        0      604 2023-06-27 23:53:38.443363 fullask_rest_framework-0.3.1/fullask_rest_framework/cli.py
--rw-r--r--   0        0        0        0 2023-06-27 23:53:38.443363 fullask_rest_framework-0.3.1/fullask_rest_framework/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 23:53:38.443363 fullask_rest_framework-0.3.1/fullask_rest_framework/contrib/admin/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 23:53:38.443363 fullask_rest_framework-0.3.1/fullask_rest_framework/contrib/admin/templates/index.html
--rw-r--r--   0        0        0      851 2023-06-27 23:53:38.443363 fullask_rest_framework-0.3.1/fullask_rest_framework/contrib/admin/templates/login_form.html
--rw-r--r--   0        0        0     1146 2023-06-27 23:53:38.443363 fullask_rest_framework-0.3.1/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css
--rw-r--r--   0        0        0        0 2023-06-27 23:53:38.443363 fullask_rest_framework-0.3.1/fullask_rest_framework/contrib/admin/views.py
--rw-r--r--   0        0        0        0 2023-06-27 23:53:38.443363 fullask_rest_framework-0.3.1/fullask_rest_framework/createproject_template/app_template/__init__.txt
--rw-r--r--   0        0        0        0 2023-06-27 23:53:38.443363 fullask_rest_framework-0.3.1/fullask_rest_framework/createproject_template/app_template/models.txt
--rw-r--r--   0        0        0        0 2023-06-27 23:53:38.443363 fullask_rest_framework-0.3.1/fullask_rest_framework/createproject_template/app_template/resources.txt
--rw-r--r--   0        0        0        0 2023-06-27 23:53:38.443363 fullask_rest_framework-0.3.1/fullask_rest_framework/createproject_template/app_template/schemas.txt
--rw-r--r--   0        0        0        0 2023-06-27 23:53:38.443363 fullask_rest_framework-0.3.1/fullask_rest_framework/createproject_template/project_template/__init__.txt
--rw-r--r--   0        0        0      112 2023-06-27 23:53:38.443363 fullask_rest_framework-0.3.1/fullask_rest_framework/createproject_template/project_template/app.txt
--rw-r--r--   0        0        0      322 2023-06-27 23:53:38.443363 fullask_rest_framework-0.3.1/fullask_rest_framework/createproject_template/project_template/config.py.txt
--rw-r--r--   0        0        0      628 2023-06-27 23:53:38.443363 fullask_rest_framework-0.3.1/fullask_rest_framework/createproject_template/project_template/factory.txt
--rw-r--r--   0        0        0       65 2023-06-27 23:53:38.443363 fullask_rest_framework-0.3.1/fullask_rest_framework/createproject_template/project_template/tests.txt
--rw-r--r--   0        0        0        0 2023-06-27 23:53:38.443363 fullask_rest_framework-0.3.1/fullask_rest_framework/entities/__init__.py
--rw-r--r--   0        0        0       49 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/fullask_rest_framework/entities/base_entity.py
--rw-r--r--   0        0        0        0 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/fullask_rest_framework/factory/__init__.py
--rw-r--r--   0        0        0     5821 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/fullask_rest_framework/factory/app_factory.py
--rw-r--r--   0        0        0      104 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/fullask_rest_framework/factory/exceptions.py
--rw-r--r--   0        0        0      683 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/fullask_rest_framework/factory/extensions.py
--rw-r--r--   0        0        0      213 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/fullask_rest_framework/factory/microapp.py
--rw-r--r--   0        0        0       46 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/fullask_rest_framework/factory/warnings.py
--rw-r--r--   0        0        0        0 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/fullask_rest_framework/orm/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/fullask_rest_framework/orm/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      302 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/fullask_rest_framework/orm/sqlalchemy/base_model.py
--rw-r--r--   0        0        0     1000 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/fullask_rest_framework/orm/sqlalchemy/mixins.py
--rw-r--r--   0        0        0        0 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/fullask_rest_framework/repositories/__init__.py
--rw-r--r--   0        0        0      243 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/fullask_rest_framework/repositories/base.py
--rw-r--r--   0        0        0     2821 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/fullask_rest_framework/repositories/crud.py
--rw-r--r--   0        0        0     8796 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/fullask_rest_framework/repositories/sqlalchemy.py
--rw-r--r--   0        0        0        0 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/fullask_rest_framework/schemas/__init__.py
--rw-r--r--   0        0        0     1212 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/fullask_rest_framework/schemas/fields.py
--rw-r--r--   0        0        0      261 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/fullask_rest_framework/schemas/filtering.py
--rw-r--r--   0        0        0     1014 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/fullask_rest_framework/schemas/pagination.py
--rw-r--r--   0        0        0      630 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/fullask_rest_framework/schemas/sorting.py
--rw-r--r--   0        0        0        0 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/fullask_rest_framework/service/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/fullask_rest_framework/utils/__init__.py
--rw-r--r--   0        0        0      572 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/fullask_rest_framework/utils/jwt.py
--rw-r--r--   0        0        0        0 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/fullask_rest_framework/vo/__init__.py
--rw-r--r--   0        0        0      346 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/fullask_rest_framework/vo/filtering.py
--rw-r--r--   0        0        0      450 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/fullask_rest_framework/vo/pagination.py
--rw-r--r--   0        0        0      407 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/fullask_rest_framework/vo/sorting.py
--rw-r--r--   0        0        0     2146 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      315 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/setup.cfg
--rw-r--r--   0        0        0      213 2023-06-27 23:53:38.447363 fullask_rest_framework-0.3.1/tox.ini
--rw-r--r--   0        0        0     5534 1970-01-01 00:00:00.000000 fullask_rest_framework-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      292 2023-07-01 17:01:00.112686 fullask_rest_framework-0.4.0/.editorconfig
+-rw-r--r--   0        0        0     1226 2023-07-01 17:01:00.112686 fullask_rest_framework-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1070 2023-07-01 17:01:00.112686 fullask_rest_framework-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3351 2023-07-01 17:01:00.112686 fullask_rest_framework-0.4.0/README.md
+-rw-r--r--   0        0        0      150 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/__init__.py
+-rw-r--r--   0        0        0      604 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/cli.py
+-rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/contrib/admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/contrib/admin/templates/index.html
+-rw-r--r--   0        0        0      851 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/contrib/admin/templates/login_form.html
+-rw-r--r--   0        0        0     1146 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css
+-rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/contrib/admin/views.py
+-rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/createproject_template/app_template/__init__.txt
+-rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/createproject_template/app_template/models.txt
+-rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/createproject_template/app_template/resources.txt
+-rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/createproject_template/app_template/schemas.txt
+-rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/createproject_template/project_template/__init__.txt
+-rw-r--r--   0        0        0      112 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/createproject_template/project_template/app.txt
+-rw-r--r--   0        0        0      322 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/createproject_template/project_template/config.py.txt
+-rw-r--r--   0        0        0      628 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/createproject_template/project_template/factory.txt
+-rw-r--r--   0        0        0       65 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/createproject_template/project_template/tests.txt
+-rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/entities/__init__.py
+-rw-r--r--   0        0        0       49 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/entities/base_entity.py
+-rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/factory/__init__.py
+-rw-r--r--   0        0        0     5947 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/factory/app_factory.py
+-rw-r--r--   0        0        0      104 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/factory/exceptions.py
+-rw-r--r--   0        0        0      683 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/factory/extensions.py
+-rw-r--r--   0        0        0      213 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/factory/microapp.py
+-rw-r--r--   0        0        0       46 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/factory/warnings.py
+-rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/orm/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/orm/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      302 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/orm/sqlalchemy/base_model.py
+-rw-r--r--   0        0        0     1000 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/orm/sqlalchemy/mixins.py
+-rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/repositories/__init__.py
+-rw-r--r--   0        0        0      243 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/repositories/base.py
+-rw-r--r--   0        0        0     2821 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/repositories/crud.py
+-rw-r--r--   0        0        0     8796 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/repositories/sqlalchemy.py
+-rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/schemas/__init__.py
+-rw-r--r--   0        0        0     1212 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/schemas/fields.py
+-rw-r--r--   0        0        0      261 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/schemas/filtering.py
+-rw-r--r--   0        0        0     1014 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/schemas/pagination.py
+-rw-r--r--   0        0        0      630 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/schemas/sorting.py
+-rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/service/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/utils/__init__.py
+-rw-r--r--   0        0        0      572 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/utils/jwt.py
+-rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/vo/__init__.py
+-rw-r--r--   0        0        0      346 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/vo/filtering.py
+-rw-r--r--   0        0        0      450 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/vo/pagination.py
+-rw-r--r--   0        0        0      407 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/vo/sorting.py
+-rw-r--r--   0        0        0     2267 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      315 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/setup.cfg
+-rw-r--r--   0        0        0      213 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/tox.ini
+-rw-r--r--   0        0        0     4318 1970-01-01 00:00:00.000000 fullask_rest_framework-0.4.0/PKG-INFO
```

### Comparing `fullask_rest_framework-0.3.1/.gitignore` & `fullask_rest_framework-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.3.1/LICENSE` & `fullask_rest_framework-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.3.1/README.md` & `fullask_rest_framework-0.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+Metadata-Version: 2.1
+Name: fullask-rest-framework
+Version: 0.4.0
+Summary: A fully-supported flask extension to build REST API.
+Author-email: tgoddessana <twicegoddessana1229@gmail.com>
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Flask
+Requires-Dist: flask-jwt-extended
+Requires-Dist: flask-sqlalchemy
+Requires-Dist: flask-marshmallow
+Requires-Dist: flask-migrate
+Requires-Dist: flask-smorest
+Requires-Dist: flask-cors
+Requires-Dist: python-dotenv
+Requires-Dist: dependency-injector
+Requires-Dist: marshmallow
+Requires-Dist: marshmallow-sqlalchemy
+
 <a name="readme-top"></a>
 
 <div align="center">
 
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
@@ -35,121 +62,65 @@
 
 ## About Fullask-REST-Framework
 
 ---
 
 Fullask REST Framework is a framework that makes it easier and faster to build REST APIs.
 
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-### Built With
-
-![Flask][Flask]
-![Python][Python]
-
-
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-<!---------------------------------------------------------------------------------------------->
-
-<br/>
-
-## Requirements
-
----
-
-- python 3.8+
-- flask 2.0 +
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-<!---------------------------------------------------------------------------------------------->
-
-<br/>
-
 ## Getting Started
 
 ---
 
 ### Installation
 
-
 install using pip command.
 
    ```
    pip install fullask-rest-framework
    ```
 
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
 <!---------------------------------------------------------------------------------------------->
 
 <br/>
 
 ## Usage
 
 ---
 
 
 
 _For more examples, please refer to the [Documentation](https://tgoddessana.github.io/fullask-rest-framework/)_
 
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
-<!---------------------------------------------------------------------------------------------->
-
-<br/>
-
-## Commit convention
-
----
-
-- FEAT : A new feature.
-- FIX : A bug fix.
-- TYPO : A typo fix.
-- DOCS : Documentation only changes. this includes "README.md", and "/docs/".
-- REFACTOR : A code change that neither fixes a bug nor adds a feature.
-- DEPLOY : A code change for deploy this package.
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!---------------------------------------------------------------------------------------------->
 
+
 <br/>
 
 ## License
 
 ---
 
-Distributed under the MIT License. See `LICENSE.txt` for more information.
+Distributed under the MIT License. See `LICENSE` for more information.
+
 
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!---------------------------------------------------------------------------------------------->
 
 <br/>
 
 ## Contact
 
 ---
 
 - Email: twicegoddessana1229@gmail.com
-- Project Link: [https://github.com/tgoddessana/flask-rest-framework](https://github.com/tgoddessana/flask-rest-framework)
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
+- Project
+  Link: [https://github.com/tgoddessana/flask-rest-framework](https://github.com/tgoddessana/flask-rest-framework)
 
 <!---------------------------------------------------------------------------------------------->
 <!---------------------------------------------------------------------------------------------->
 
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 
@@ -176,7 +147,8 @@
 [product-screenshot]: images/screenshot.png
 
 [Flask]: https://img.shields.io/badge/flask-00000?style=for-the-badge&logo=flask&logoColor=white
 
 [Python]: https://img.shields.io/badge/python-306998?style=for-the-badge&logo=python&logoColor=white
 
 
+
```

#### html2text {}

```diff
@@ -1,57 +1,49 @@
+Metadata-Version: 2.1 Name: fullask-rest-framework Version: 0.4.0 Summary: A
+fully-supported flask extension to build REST API. Author-email: tgoddessana
+gmail.com> Requires-Python: >=3.9 Description-Content-Type: text/markdown
+Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
+:: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
+Natural Language :: English Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Flask Requires-Dist: flask-jwt-extended Requires-Dist: flask-
+sqlalchemy Requires-Dist: flask-marshmallow Requires-Dist: flask-migrate
+Requires-Dist: flask-smorest Requires-Dist: flask-cors Requires-Dist: python-
+dotenv Requires-Dist: dependency-injector Requires-Dist: marshmallow Requires-
+Dist: marshmallow-sqlalchemy
    [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
 shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
       shield]][issues-url] [![MIT License][license-shield]][license-url]
 
                                        >
                        **** Fullask-REST-Framework ****
              A fully-supported flask extension to build REST API.
                              Explore_the_docs_Â»
 
 ## About Fullask-REST-Framework --- Fullask REST Framework is a framework that
-makes it easier and faster to build REST APIs.
-                                                                  (back_to_top)
-### Built With ![Flask][Flask] ![Python][Python]
-                                                                  (back_to_top)
-
-## Requirements --- - python 3.8+ - flask 2.0 +
-                                                                  (back_to_top)
-
-## Getting Started --- ### Installation install using pip command. ``` pip
-install fullask-rest-framework ```
-                                                                  (back_to_top)
-
+makes it easier and faster to build REST APIs. ## Getting Started --- ###
+Installation install using pip command. ``` pip install fullask-rest-framework
+```
 ## Usage --- _For more examples, please refer to the [Documentation](https://
 tgoddessana.github.io/fullask-rest-framework/)_
-                                                                  (back_to_top)
-
-## Commit convention --- - FEAT : A new feature. - FIX : A bug fix. - TYPO : A
-typo fix. - DOCS : Documentation only changes. this includes "README.md", and
-"/docs/". - REFACTOR : A code change that neither fixes a bug nor adds a
-feature. - DEPLOY : A code change for deploy this package.
-                                                                  (back_to_top)
-
-## License --- Distributed under the MIT License. See `LICENSE.txt` for more
+## License --- Distributed under the MIT License. See `LICENSE` for more
 information.
-                                                                  (back_to_top)
-
 ## Contact --- - Email: twicegoddessana1229@gmail.com - Project Link: [https://
 github.com/tgoddessana/flask-rest-framework](https://github.com/tgoddessana/
-flask-rest-framework)
-                                                                  (back_to_top)
-    [contributors-shield]: https://img.shields.io/github/contributors/
-tgoddessana/flask-rest-framework.svg?style=for-the-badge [contributors-url]:
-https://github.com/tgoddessana/flask-rest-framework/graphs/contributors [forks-
-shield]: https://img.shields.io/github/forks/tgoddessana/flask-rest-
-framework.svg?style=for-the-badge [forks-url]: https://github.com/tgoddessana/
-flask-rest-framework/network/members [stars-shield]: https://img.shields.io/
-github/stars/tgoddessana/flask-rest-framework.svg?style=for-the-badge [stars-
-url]: https://github.com/tgoddessana/flask-rest-framework/stargazers [issues-
-shield]: https://img.shields.io/github/issues/tgoddessana/flask-rest-
-framework.svg?style=for-the-badge [issues-url]: https://github.com/tgoddessana/
-flask-rest-framework/issues [license-shield]: https://img.shields.io/github/
-license/tgoddessana/flask-rest-framework.svg?style=for-the-badge [license-url]:
-https://github.com/tgoddessana/flask-rest-framework/blob/master/LICENSE.txt
-[product-screenshot]: images/screenshot.png [Flask]: https://img.shields.io/
-badge/flask-00000?style=for-the-badge&logo=flask&logoColor=white [Python]:
-https://img.shields.io/badge/python-306998?style=for-the-
-badge&logo=python&logoColor=white
+flask-rest-framework)     [contributors-shield]: https://img.shields.io/github/
+contributors/tgoddessana/flask-rest-framework.svg?style=for-the-badge
+[contributors-url]: https://github.com/tgoddessana/flask-rest-framework/graphs/
+contributors [forks-shield]: https://img.shields.io/github/forks/tgoddessana/
+flask-rest-framework.svg?style=for-the-badge [forks-url]: https://github.com/
+tgoddessana/flask-rest-framework/network/members [stars-shield]: https://
+img.shields.io/github/stars/tgoddessana/flask-rest-framework.svg?style=for-the-
+badge [stars-url]: https://github.com/tgoddessana/flask-rest-framework/
+stargazers [issues-shield]: https://img.shields.io/github/issues/tgoddessana/
+flask-rest-framework.svg?style=for-the-badge [issues-url]: https://github.com/
+tgoddessana/flask-rest-framework/issues [license-shield]: https://
+img.shields.io/github/license/tgoddessana/flask-rest-framework.svg?style=for-
+the-badge [license-url]: https://github.com/tgoddessana/flask-rest-framework/
+blob/master/LICENSE.txt [product-screenshot]: images/screenshot.png [Flask]:
+https://img.shields.io/badge/flask-00000?style=for-the-
+badge&logo=flask&logoColor=white [Python]: https://img.shields.io/badge/python-
+306998?style=for-the-badge&logo=python&logoColor=white
```

### Comparing `fullask_rest_framework-0.3.1/fullask_rest_framework/cli.py` & `fullask_rest_framework-0.4.0/fullask_rest_framework/cli.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.3.1/fullask_rest_framework/contrib/admin/templates/login_form.html` & `fullask_rest_framework-0.4.0/fullask_rest_framework/contrib/admin/templates/login_form.html`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.3.1/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css` & `fullask_rest_framework-0.4.0/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.3.1/fullask_rest_framework/createproject_template/project_template/factory.txt` & `fullask_rest_framework-0.4.0/fullask_rest_framework/createproject_template/project_template/factory.txt`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.3.1/fullask_rest_framework/factory/app_factory.py` & `fullask_rest_framework-0.4.0/fullask_rest_framework/factory/app_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import importlib
 import inspect
 from types import ModuleType
 from typing import Any, Dict, List, Optional
-
+import warnings
 from dependency_injector.containers import Container
 from dotenv import load_dotenv
 from flask import Flask
 from flask_smorest import Api
 
 from fullask_rest_framework.factory.exceptions import ConfigNotSetError
 from fullask_rest_framework.factory.microapp import MicroApp
 
 
 class BaseApplicationFactory:
     FLASK_APP_NAME: Optional[str] = None
-    APP_BASE_DIR: Optional[str] = None
     CONFIG_MAPPING: Optional[dict[str, Any]] = None
-    EXTENSION_MODULE: Optional[str] = None
+    EXTENSION_MODULE: str = "fullask_rest_framework.factory.extensions"
     MICRO_APP_CONFIG: Optional[List[Dict[str, str]]] = None
     DOTENV_SETTINGS: Optional[dict] = None
 
     @classmethod
     def create_app(cls, environment: str) -> Flask:
         # load environment variables.
         cls._load_dotenv()
@@ -111,39 +110,43 @@
     def _register_micro_apps(cls, smorest_api: Api) -> None:
         """
         register micro apps, with cls.MICRO_APP_CONFIG settings.
         this also does the Dependency Injection,
         with dependency_injector's DynamicContainer.
         """
         if not cls.MICRO_APP_CONFIG:
-            return
+            return warnings.warn(
+                "No routing is currently set for the application, please set it via MICRO_APP_CONFIG."
+            )
         for micro_app_information in cls.MICRO_APP_CONFIG:
             for app_package_string, url_prefix in micro_app_information.items():
-                app_module = importlib.import_module(app_package_string)
                 micro_app = next(
                     (
                         cls
-                        for name, cls in app_module.__dict__.items()
+                        for name, cls in importlib.import_module(
+                            app_package_string
+                        ).__dict__.items()
                         if inspect.isclass(cls)
                         and issubclass(cls, MicroApp)
                         and cls is not MicroApp
                     ),
                     None,
                 )
                 # Register Blueprint.
                 for blueprint in micro_app.blueprints:
                     smorest_api.register_blueprint(blueprint, url_prefix=url_prefix)
-                # get the microapp container.
+                # get the microapp container and wire it.
                 cls._setup_di_container(
-                    micro_app_container=micro_app.microapp_container
+                    micro_app_container=micro_app.microapp_container,
+                    app_package_string=app_package_string,
                 )
 
     @classmethod
-    def _setup_di_container(cls, micro_app_container: Container) -> None:
+    def _setup_di_container(
+        cls, micro_app_container: Container, app_package_string
+    ) -> None:
         """wiring the DI Container."""
-        micro_app_container.wire(packages=[cls.APP_BASE_DIR])
+        micro_app_container.wire(packages=[app_package_string])
 
     @classmethod
     def get_extensions(cls) -> ModuleType:
-        if cls.EXTENSION_MODULE is not None:
-            return importlib.import_module(cls.EXTENSION_MODULE)
-        return importlib.import_module("fullask_rest_framework.factory.extensions")
+        return importlib.import_module(cls.EXTENSION_MODULE)
```

### Comparing `fullask_rest_framework-0.3.1/fullask_rest_framework/factory/extensions.py` & `fullask_rest_framework-0.4.0/fullask_rest_framework/factory/extensions.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.3.1/fullask_rest_framework/orm/sqlalchemy/mixins.py` & `fullask_rest_framework-0.4.0/fullask_rest_framework/orm/sqlalchemy/mixins.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.3.1/fullask_rest_framework/repositories/crud.py` & `fullask_rest_framework-0.4.0/fullask_rest_framework/repositories/crud.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.3.1/fullask_rest_framework/repositories/sqlalchemy.py` & `fullask_rest_framework-0.4.0/fullask_rest_framework/repositories/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.3.1/fullask_rest_framework/schemas/fields.py` & `fullask_rest_framework-0.4.0/fullask_rest_framework/schemas/fields.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.3.1/fullask_rest_framework/schemas/pagination.py` & `fullask_rest_framework-0.4.0/fullask_rest_framework/schemas/pagination.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.3.1/fullask_rest_framework/schemas/sorting.py` & `fullask_rest_framework-0.4.0/fullask_rest_framework/schemas/sorting.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.3.1/fullask_rest_framework/utils/jwt.py` & `fullask_rest_framework-0.4.0/fullask_rest_framework/utils/jwt.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.3.1/pyproject.toml` & `fullask_rest_framework-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     "docs/",
     "tests/",
     ".github/"
 ]
 
 [tool.poetry]
 name = "fullask-rest-framework"
-version = "0.3.1"
+version = "0.4.0"
 description = ""
 authors = ["tgoddessana <twicegoddessana1229@gmail.com>"]
 
 [tool.poetry.dependencies]
 pip = "*"
 python = "^3.11"
 flask = "^2.2.3"
@@ -67,15 +67,15 @@
 marshmallow = "^3.19.0"
 marshmallow-sqlalchemy = "^0.29.0"
 flask-sqlalchemy = "^3.0.3"
 flask-marshmallow = "^0.15.0"
 flask-migrate = "^4.0.4"
 flask-smorest = "^0.42.0"
 python-dotenv = "^1.0.0"
-flask-cors = "^3.0.10"
+flask-cors = "^4.0.0"
 dependency_injector = "*"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
 wheel = "^0.40.0"
 twine = "^4.0.2"
@@ -84,14 +84,21 @@
 flit = "^3.9.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.1.0"
 flake8 = "^6.0.0"
 tox = "*"
+mypy = "*"
 coverage = "*"
+types-Flask-Cors = "*"
+types-Flask-Migrate = "*"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "*"
 sphinx-rtd-theme = "^1.2.0"
 myst-parser = "*"
 jinja2 = "^3.0"
+
+[tool.mypy]
+exclude = ["docs"]
+ignore_missing_imports = true
```

