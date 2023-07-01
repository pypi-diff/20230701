# Comparing `tmp/fullask_rest_framework-0.4.0.tar.gz` & `tmp/fullask_rest_framework-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fullask_rest_framework-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fullask_rest_framework-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fullask_rest_framework-0.4.0.tar` & `fullask_rest_framework-0.5.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      292 2023-07-01 17:01:00.112686 fullask_rest_framework-0.4.0/.editorconfig
--rw-r--r--   0        0        0     1226 2023-07-01 17:01:00.112686 fullask_rest_framework-0.4.0/.gitignore
--rw-r--r--   0        0        0     1070 2023-07-01 17:01:00.112686 fullask_rest_framework-0.4.0/LICENSE
--rw-r--r--   0        0        0     3351 2023-07-01 17:01:00.112686 fullask_rest_framework-0.4.0/README.md
--rw-r--r--   0        0        0      150 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/__init__.py
--rw-r--r--   0        0        0      604 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/cli.py
--rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/contrib/admin/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/contrib/admin/templates/index.html
--rw-r--r--   0        0        0      851 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/contrib/admin/templates/login_form.html
--rw-r--r--   0        0        0     1146 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css
--rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/contrib/admin/views.py
--rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/createproject_template/app_template/__init__.txt
--rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/createproject_template/app_template/models.txt
--rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/createproject_template/app_template/resources.txt
--rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/createproject_template/app_template/schemas.txt
--rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/createproject_template/project_template/__init__.txt
--rw-r--r--   0        0        0      112 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/createproject_template/project_template/app.txt
--rw-r--r--   0        0        0      322 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/createproject_template/project_template/config.py.txt
--rw-r--r--   0        0        0      628 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/createproject_template/project_template/factory.txt
--rw-r--r--   0        0        0       65 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/createproject_template/project_template/tests.txt
--rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/entities/__init__.py
--rw-r--r--   0        0        0       49 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/entities/base_entity.py
--rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/factory/__init__.py
--rw-r--r--   0        0        0     5947 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/factory/app_factory.py
--rw-r--r--   0        0        0      104 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/factory/exceptions.py
--rw-r--r--   0        0        0      683 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/factory/extensions.py
--rw-r--r--   0        0        0      213 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/factory/microapp.py
--rw-r--r--   0        0        0       46 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/factory/warnings.py
--rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/orm/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/orm/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      302 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/orm/sqlalchemy/base_model.py
--rw-r--r--   0        0        0     1000 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/orm/sqlalchemy/mixins.py
--rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/repositories/__init__.py
--rw-r--r--   0        0        0      243 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/repositories/base.py
--rw-r--r--   0        0        0     2821 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/repositories/crud.py
--rw-r--r--   0        0        0     8796 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/repositories/sqlalchemy.py
--rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/schemas/__init__.py
--rw-r--r--   0        0        0     1212 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/schemas/fields.py
--rw-r--r--   0        0        0      261 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/schemas/filtering.py
--rw-r--r--   0        0        0     1014 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/schemas/pagination.py
--rw-r--r--   0        0        0      630 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/schemas/sorting.py
--rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/service/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/utils/__init__.py
--rw-r--r--   0        0        0      572 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/utils/jwt.py
--rw-r--r--   0        0        0        0 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/vo/__init__.py
--rw-r--r--   0        0        0      346 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/vo/filtering.py
--rw-r--r--   0        0        0      450 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/vo/pagination.py
--rw-r--r--   0        0        0      407 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/fullask_rest_framework/vo/sorting.py
--rw-r--r--   0        0        0     2267 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      315 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/setup.cfg
--rw-r--r--   0        0        0      213 2023-07-01 17:01:00.116686 fullask_rest_framework-0.4.0/tox.ini
--rw-r--r--   0        0        0     4318 1970-01-01 00:00:00.000000 fullask_rest_framework-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      292 2023-07-01 17:48:47.582960 fullask_rest_framework-0.5.0/.editorconfig
+-rw-r--r--   0        0        0     1226 2023-07-01 17:48:47.582960 fullask_rest_framework-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1070 2023-07-01 17:48:47.582960 fullask_rest_framework-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3351 2023-07-01 17:48:47.582960 fullask_rest_framework-0.5.0/README.md
+-rw-r--r--   0        0        0      150 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/__init__.py
+-rw-r--r--   0        0        0      604 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/cli.py
+-rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/contrib/admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/contrib/admin/templates/index.html
+-rw-r--r--   0        0        0      851 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/contrib/admin/templates/login_form.html
+-rw-r--r--   0        0        0     1146 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css
+-rw-r--r--   0        0        0      238 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/contrib/admin/views.py
+-rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/createproject_template/app_template/__init__.txt
+-rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/createproject_template/app_template/models.txt
+-rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/createproject_template/app_template/resources.txt
+-rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/createproject_template/app_template/schemas.txt
+-rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/createproject_template/project_template/__init__.txt
+-rw-r--r--   0        0        0      112 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/createproject_template/project_template/app.txt
+-rw-r--r--   0        0        0      322 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/createproject_template/project_template/config.py.txt
+-rw-r--r--   0        0        0      628 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/createproject_template/project_template/factory.txt
+-rw-r--r--   0        0        0       65 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/createproject_template/project_template/tests.txt
+-rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/entities/__init__.py
+-rw-r--r--   0        0        0       49 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/entities/base_entity.py
+-rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/factory/__init__.py
+-rw-r--r--   0        0        0     6204 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/factory/app_factory.py
+-rw-r--r--   0        0        0      104 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/factory/exceptions.py
+-rw-r--r--   0        0        0      683 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/factory/extensions.py
+-rw-r--r--   0        0        0      213 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/factory/microapp.py
+-rw-r--r--   0        0        0       46 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/factory/warnings.py
+-rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/orm/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/orm/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      302 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/orm/sqlalchemy/base_model.py
+-rw-r--r--   0        0        0     1000 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/orm/sqlalchemy/mixins.py
+-rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/repositories/__init__.py
+-rw-r--r--   0        0        0      243 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/repositories/base.py
+-rw-r--r--   0        0        0     2821 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/repositories/crud.py
+-rw-r--r--   0        0        0     8796 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/repositories/sqlalchemy.py
+-rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/schemas/__init__.py
+-rw-r--r--   0        0        0     1212 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/schemas/fields.py
+-rw-r--r--   0        0        0      261 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/schemas/filtering.py
+-rw-r--r--   0        0        0     1014 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/schemas/pagination.py
+-rw-r--r--   0        0        0      630 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/schemas/sorting.py
+-rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/service/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/utils/__init__.py
+-rw-r--r--   0        0        0      572 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/utils/jwt.py
+-rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/vo/__init__.py
+-rw-r--r--   0        0        0      346 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/vo/filtering.py
+-rw-r--r--   0        0        0      450 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/vo/pagination.py
+-rw-r--r--   0        0        0      407 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/vo/sorting.py
+-rw-r--r--   0        0        0     2267 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      316 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/setup.cfg
+-rw-r--r--   0        0        0      213 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/tox.ini
+-rw-r--r--   0        0        0     4318 1970-01-01 00:00:00.000000 fullask_rest_framework-0.5.0/PKG-INFO
```

### Comparing `fullask_rest_framework-0.4.0/.gitignore` & `fullask_rest_framework-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.4.0/LICENSE` & `fullask_rest_framework-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.4.0/README.md` & `fullask_rest_framework-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.4.0/fullask_rest_framework/cli.py` & `fullask_rest_framework-0.5.0/fullask_rest_framework/cli.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.4.0/fullask_rest_framework/contrib/admin/templates/login_form.html` & `fullask_rest_framework-0.5.0/fullask_rest_framework/contrib/admin/templates/login_form.html`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.4.0/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css` & `fullask_rest_framework-0.5.0/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.4.0/fullask_rest_framework/createproject_template/project_template/factory.txt` & `fullask_rest_framework-0.5.0/fullask_rest_framework/createproject_template/project_template/factory.txt`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.4.0/fullask_rest_framework/factory/app_factory.py` & `fullask_rest_framework-0.5.0/fullask_rest_framework/factory/app_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import importlib
 import inspect
+import warnings
 from types import ModuleType
 from typing import Any, Dict, List, Optional
-import warnings
+
 from dependency_injector.containers import Container
 from dotenv import load_dotenv
 from flask import Flask
 from flask_smorest import Api
 
+from fullask_rest_framework.contrib.admin.views import admin_bp
 from fullask_rest_framework.factory.exceptions import ConfigNotSetError
 from fullask_rest_framework.factory.microapp import MicroApp
 
 
 class BaseApplicationFactory:
     FLASK_APP_NAME: Optional[str] = None
     CONFIG_MAPPING: Optional[dict[str, Any]] = None
@@ -29,14 +31,16 @@
         cls._load_config(flask_app=flask_app, environment=environment)
         # create a flask-smorest Api object.
         smorest_api = Api(app=flask_app)
         # configure third-party extensions.
         cls._configure_extensions(flask_app=flask_app)
         # register micro apps. this also does the Dependency Injection.
         cls._register_micro_apps(smorest_api)
+        # setup admin page.
+        cls._configure_admin(flask_app=flask_app)
         return flask_app
 
     @classmethod
     def _load_dotenv(cls) -> None:
         """
         load dotenv file, if cls.DOTENV_SETTINGS is set.
         """
@@ -144,9 +148,13 @@
     def _setup_di_container(
         cls, micro_app_container: Container, app_package_string
     ) -> None:
         """wiring the DI Container."""
         micro_app_container.wire(packages=[app_package_string])
 
     @classmethod
+    def _configure_admin(cls, flask_app: Flask):
+        flask_app.register_blueprint(admin_bp)
+
+    @classmethod
     def get_extensions(cls) -> ModuleType:
         return importlib.import_module(cls.EXTENSION_MODULE)
```

### Comparing `fullask_rest_framework-0.4.0/fullask_rest_framework/factory/extensions.py` & `fullask_rest_framework-0.5.0/fullask_rest_framework/factory/extensions.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.4.0/fullask_rest_framework/orm/sqlalchemy/mixins.py` & `fullask_rest_framework-0.5.0/fullask_rest_framework/orm/sqlalchemy/mixins.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.4.0/fullask_rest_framework/repositories/crud.py` & `fullask_rest_framework-0.5.0/fullask_rest_framework/repositories/crud.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.4.0/fullask_rest_framework/repositories/sqlalchemy.py` & `fullask_rest_framework-0.5.0/fullask_rest_framework/repositories/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.4.0/fullask_rest_framework/schemas/fields.py` & `fullask_rest_framework-0.5.0/fullask_rest_framework/schemas/fields.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.4.0/fullask_rest_framework/schemas/pagination.py` & `fullask_rest_framework-0.5.0/fullask_rest_framework/schemas/pagination.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.4.0/fullask_rest_framework/schemas/sorting.py` & `fullask_rest_framework-0.5.0/fullask_rest_framework/schemas/sorting.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.4.0/fullask_rest_framework/utils/jwt.py` & `fullask_rest_framework-0.5.0/fullask_rest_framework/utils/jwt.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.4.0/pyproject.toml` & `fullask_rest_framework-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     "docs/",
     "tests/",
     ".github/"
 ]
 
 [tool.poetry]
 name = "fullask-rest-framework"
-version = "0.4.0"
+version = "0.5.0"
 description = ""
 authors = ["tgoddessana <twicegoddessana1229@gmail.com>"]
 
 [tool.poetry.dependencies]
 pip = "*"
 python = "^3.11"
 flask = "^2.2.3"
```

### Comparing `fullask_rest_framework-0.4.0/PKG-INFO` & `fullask_rest_framework-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fullask-rest-framework
-Version: 0.4.0
+Version: 0.5.0
 Summary: A fully-supported flask extension to build REST API.
 Author-email: tgoddessana <twicegoddessana1229@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fullask-rest-framework Version: 0.4.0 Summary: A
+Metadata-Version: 2.1 Name: fullask-rest-framework Version: 0.5.0 Summary: A
 fully-supported flask extension to build REST API. Author-email: tgoddessana
 gmail.com> Requires-Python: >=3.9 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

