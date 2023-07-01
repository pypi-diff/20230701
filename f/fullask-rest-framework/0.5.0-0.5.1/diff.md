# Comparing `tmp/fullask_rest_framework-0.5.0.tar.gz` & `tmp/fullask_rest_framework-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fullask_rest_framework-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fullask_rest_framework-0.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fullask_rest_framework-0.5.0.tar` & `fullask_rest_framework-0.5.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      292 2023-07-01 17:48:47.582960 fullask_rest_framework-0.5.0/.editorconfig
--rw-r--r--   0        0        0     1226 2023-07-01 17:48:47.582960 fullask_rest_framework-0.5.0/.gitignore
--rw-r--r--   0        0        0     1070 2023-07-01 17:48:47.582960 fullask_rest_framework-0.5.0/LICENSE
--rw-r--r--   0        0        0     3351 2023-07-01 17:48:47.582960 fullask_rest_framework-0.5.0/README.md
--rw-r--r--   0        0        0      150 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/__init__.py
--rw-r--r--   0        0        0      604 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/cli.py
--rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/contrib/admin/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/contrib/admin/templates/index.html
--rw-r--r--   0        0        0      851 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/contrib/admin/templates/login_form.html
--rw-r--r--   0        0        0     1146 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css
--rw-r--r--   0        0        0      238 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/contrib/admin/views.py
--rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/createproject_template/app_template/__init__.txt
--rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/createproject_template/app_template/models.txt
--rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/createproject_template/app_template/resources.txt
--rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/createproject_template/app_template/schemas.txt
--rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/createproject_template/project_template/__init__.txt
--rw-r--r--   0        0        0      112 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/createproject_template/project_template/app.txt
--rw-r--r--   0        0        0      322 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/createproject_template/project_template/config.py.txt
--rw-r--r--   0        0        0      628 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/createproject_template/project_template/factory.txt
--rw-r--r--   0        0        0       65 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/createproject_template/project_template/tests.txt
--rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/entities/__init__.py
--rw-r--r--   0        0        0       49 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/entities/base_entity.py
--rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/factory/__init__.py
--rw-r--r--   0        0        0     6204 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/factory/app_factory.py
--rw-r--r--   0        0        0      104 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/factory/exceptions.py
--rw-r--r--   0        0        0      683 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/factory/extensions.py
--rw-r--r--   0        0        0      213 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/factory/microapp.py
--rw-r--r--   0        0        0       46 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/factory/warnings.py
--rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/orm/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/orm/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      302 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/orm/sqlalchemy/base_model.py
--rw-r--r--   0        0        0     1000 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/orm/sqlalchemy/mixins.py
--rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/repositories/__init__.py
--rw-r--r--   0        0        0      243 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/repositories/base.py
--rw-r--r--   0        0        0     2821 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/repositories/crud.py
--rw-r--r--   0        0        0     8796 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/repositories/sqlalchemy.py
--rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/schemas/__init__.py
--rw-r--r--   0        0        0     1212 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/schemas/fields.py
--rw-r--r--   0        0        0      261 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/schemas/filtering.py
--rw-r--r--   0        0        0     1014 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/schemas/pagination.py
--rw-r--r--   0        0        0      630 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/schemas/sorting.py
--rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/service/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/utils/__init__.py
--rw-r--r--   0        0        0      572 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/utils/jwt.py
--rw-r--r--   0        0        0        0 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/vo/__init__.py
--rw-r--r--   0        0        0      346 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/vo/filtering.py
--rw-r--r--   0        0        0      450 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/vo/pagination.py
--rw-r--r--   0        0        0      407 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/fullask_rest_framework/vo/sorting.py
--rw-r--r--   0        0        0     2267 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      316 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/setup.cfg
--rw-r--r--   0        0        0      213 2023-07-01 17:48:47.586960 fullask_rest_framework-0.5.0/tox.ini
--rw-r--r--   0        0        0     4318 1970-01-01 00:00:00.000000 fullask_rest_framework-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      292 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/.editorconfig
+-rw-r--r--   0        0        0     1226 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/.gitignore
+-rw-r--r--   0        0        0     1070 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/LICENSE
+-rw-r--r--   0        0        0     3351 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/README.md
+-rw-r--r--   0        0        0      150 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/__init__.py
+-rw-r--r--   0        0        0      604 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/cli.py
+-rw-r--r--   0        0        0        0 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/contrib/admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/contrib/admin/templates/index.html
+-rw-r--r--   0        0        0      851 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/contrib/admin/templates/login_form.html
+-rw-r--r--   0        0        0     1146 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css
+-rw-r--r--   0        0        0      202 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/contrib/admin/views.py
+-rw-r--r--   0        0        0        0 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/createproject_template/app_template/__init__.txt
+-rw-r--r--   0        0        0        0 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/createproject_template/app_template/models.txt
+-rw-r--r--   0        0        0        0 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/createproject_template/app_template/resources.txt
+-rw-r--r--   0        0        0        0 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/createproject_template/app_template/schemas.txt
+-rw-r--r--   0        0        0        0 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/createproject_template/project_template/__init__.txt
+-rw-r--r--   0        0        0      112 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/createproject_template/project_template/app.txt
+-rw-r--r--   0        0        0      322 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/createproject_template/project_template/config.py.txt
+-rw-r--r--   0        0        0      628 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/createproject_template/project_template/factory.txt
+-rw-r--r--   0        0        0       65 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/createproject_template/project_template/tests.txt
+-rw-r--r--   0        0        0        0 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/entities/__init__.py
+-rw-r--r--   0        0        0       49 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/entities/base_entity.py
+-rw-r--r--   0        0        0        0 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/factory/__init__.py
+-rw-r--r--   0        0        0     6242 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/factory/app_factory.py
+-rw-r--r--   0        0        0      104 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/factory/exceptions.py
+-rw-r--r--   0        0        0      683 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/factory/extensions.py
+-rw-r--r--   0        0        0      206 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/factory/microapp.py
+-rw-r--r--   0        0        0       46 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/factory/warnings.py
+-rw-r--r--   0        0        0        0 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/orm/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/orm/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      292 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/orm/sqlalchemy/base_model.py
+-rw-r--r--   0        0        0     1004 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/orm/sqlalchemy/mixins.py
+-rw-r--r--   0        0        0        0 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/repositories/__init__.py
+-rw-r--r--   0        0        0      243 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/repositories/base.py
+-rw-r--r--   0        0        0     2821 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/repositories/crud.py
+-rw-r--r--   0        0        0     8865 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/repositories/sqlalchemy.py
+-rw-r--r--   0        0        0        0 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/schemas/__init__.py
+-rw-r--r--   0        0        0     1212 2023-07-01 18:10:54.310546 fullask_rest_framework-0.5.1/fullask_rest_framework/schemas/fields.py
+-rw-r--r--   0        0        0      261 2023-07-01 18:10:54.310546 fullask_rest_framework-0.5.1/fullask_rest_framework/schemas/filtering.py
+-rw-r--r--   0        0        0     1014 2023-07-01 18:10:54.310546 fullask_rest_framework-0.5.1/fullask_rest_framework/schemas/pagination.py
+-rw-r--r--   0        0        0      644 2023-07-01 18:10:54.310546 fullask_rest_framework-0.5.1/fullask_rest_framework/schemas/sorting.py
+-rw-r--r--   0        0        0        0 2023-07-01 18:10:54.310546 fullask_rest_framework-0.5.1/fullask_rest_framework/service/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 18:10:54.310546 fullask_rest_framework-0.5.1/fullask_rest_framework/utils/__init__.py
+-rw-r--r--   0        0        0      572 2023-07-01 18:10:54.310546 fullask_rest_framework-0.5.1/fullask_rest_framework/utils/jwt.py
+-rw-r--r--   0        0        0      138 2023-07-01 18:10:54.310546 fullask_rest_framework-0.5.1/fullask_rest_framework/vo/__init__.py
+-rw-r--r--   0        0        0      346 2023-07-01 18:10:54.310546 fullask_rest_framework-0.5.1/fullask_rest_framework/vo/filtering.py
+-rw-r--r--   0        0        0      450 2023-07-01 18:10:54.310546 fullask_rest_framework-0.5.1/fullask_rest_framework/vo/pagination.py
+-rw-r--r--   0        0        0      407 2023-07-01 18:10:54.310546 fullask_rest_framework-0.5.1/fullask_rest_framework/vo/sorting.py
+-rw-r--r--   0        0        0     2267 2023-07-01 18:10:54.310546 fullask_rest_framework-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      316 2023-07-01 18:10:54.310546 fullask_rest_framework-0.5.1/setup.cfg
+-rw-r--r--   0        0        0      213 2023-07-01 18:10:54.310546 fullask_rest_framework-0.5.1/tox.ini
+-rw-r--r--   0        0        0     4318 1970-01-01 00:00:00.000000 fullask_rest_framework-0.5.1/PKG-INFO
```

### Comparing `fullask_rest_framework-0.5.0/.gitignore` & `fullask_rest_framework-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.5.0/LICENSE` & `fullask_rest_framework-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.5.0/README.md` & `fullask_rest_framework-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.5.0/fullask_rest_framework/cli.py` & `fullask_rest_framework-0.5.1/fullask_rest_framework/cli.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.5.0/fullask_rest_framework/contrib/admin/templates/login_form.html` & `fullask_rest_framework-0.5.1/fullask_rest_framework/contrib/admin/templates/login_form.html`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.5.0/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css` & `fullask_rest_framework-0.5.1/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.5.0/fullask_rest_framework/createproject_template/project_template/factory.txt` & `fullask_rest_framework-0.5.1/fullask_rest_framework/createproject_template/project_template/factory.txt`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.5.0/fullask_rest_framework/factory/app_factory.py` & `fullask_rest_framework-0.5.1/fullask_rest_framework/factory/app_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,16 +67,17 @@
         )
 
     @classmethod
     def _load_config(cls, flask_app: Flask, environment: str) -> None:
         # make sure that the CONFIG_MAPPING is set.
         if not cls.CONFIG_MAPPING:
             raise ConfigNotSetError(
-                "Config is not set appropriately. Make sure you have assigned the CONFIG class variable"
-                "appropriately in your application factory class."
+                "Config is not set appropriately. Make sure you have assigned"
+                "the CONFIG class variable appropriately in "
+                "your application factory class."
             )
         # make sure that the environment variable is in the CONFIG_MAPPING.keys().
         if environment not in cls.CONFIG_MAPPING.keys():
             raise ValueError(
                 f"Environment '{environment}' is not set in the CONFIG_MAPPING."
                 f"available environments are: {list(cls.CONFIG_MAPPING.keys())}"
             )
@@ -115,15 +116,16 @@
         """
         register micro apps, with cls.MICRO_APP_CONFIG settings.
         this also does the Dependency Injection,
         with dependency_injector's DynamicContainer.
         """
         if not cls.MICRO_APP_CONFIG:
             return warnings.warn(
-                "No routing is currently set for the application, please set it via MICRO_APP_CONFIG."
+                "No routing is currently set for the application, "
+                "please set it via MICRO_APP_CONFIG."
             )
         for micro_app_information in cls.MICRO_APP_CONFIG:
             for app_package_string, url_prefix in micro_app_information.items():
                 micro_app = next(
                     (
                         cls
                         for name, cls in importlib.import_module(
```

### Comparing `fullask_rest_framework-0.5.0/fullask_rest_framework/factory/extensions.py` & `fullask_rest_framework-0.5.1/fullask_rest_framework/factory/extensions.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.5.0/fullask_rest_framework/orm/sqlalchemy/mixins.py` & `fullask_rest_framework-0.5.1/fullask_rest_framework/orm/sqlalchemy/mixins.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from uuid import uuid4
 
 from fullask_rest_framework.factory.extensions import db
 
 
 class BaseMixin:
     """
-    The parent mixin of all mixins. Prevents mixins from being used as classes themselves.
+    The parent mixin of all mixins. Prevents mixins
+    from being used as classes themselves.
     """
 
     def __init__(self, *args, **kwargs) -> None:
         if type(self) is self.__class__:
             raise TypeError(
                 f"You can only use {self.__class__.__name__} for implementing Mixin."
             )
```

### Comparing `fullask_rest_framework-0.5.0/fullask_rest_framework/repositories/crud.py` & `fullask_rest_framework-0.5.1/fullask_rest_framework/repositories/crud.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.5.0/fullask_rest_framework/repositories/sqlalchemy.py` & `fullask_rest_framework-0.5.1/fullask_rest_framework/repositories/sqlalchemy.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from flask_marshmallow.sqla import SQLAlchemyAutoSchema  # type: ignore[import]
 from flask_sqlalchemy.query import Query
 from sqlalchemy import inspect, select
 
 from fullask_rest_framework.repositories.base import T
 from fullask_rest_framework.repositories.crud import CRUDRepositoryABC
 from fullask_rest_framework.vo.filtering import FilteringRequest
-from fullask_rest_framework.vo.pagination import PaginationRequest, PaginationResponse
+from fullask_rest_framework.vo.pagination import (PaginationRequest,
+                                                  PaginationResponse)
 from fullask_rest_framework.vo.sorting import SortingRequest
 
 
 class SQLAlchemyFullRepository(CRUDRepositoryABC, Generic[T]):
     """
     The implementation of CRUDRepositoryABC, with SQLAlchemy.
     this implementation has dependency with flask-sqlalchemy's SQLAlchemy object.
@@ -184,20 +185,22 @@
         # Iterate over the fields of the entity object
         for field_name, field_value in entity.__dict__.items():
             if field_name != "id":
                 setattr(model_instance, field_name, field_value)
 
     def _configure_entity(self) -> Type[T]:
         """
-        This method will find if there is a SQLAlchemy model class defined based on the entity class name.
+        This method will find if there is a SQLAlchemy model class
+        defined based on the entity class name.
 
         The rules to look for are as follows:
         {entity class name - "Entity"} + "Model"
 
-        For example, if the entity is named "CarEntity", the method will try to find the "CarModel" class.
+        For example, if the entity is named "CarEntity",
+        this method will try to find the "CarModel" class.
         """
         models = {
             mapper.class_.__name__: mapper.class_
             for mapper in self.db.Model.registry.mappers
         }
         for model_name, mapper_class in models.items():
             if model_name == self.ENTITY_CLS.__name__.replace("Entity", "") + "Model":
```

### Comparing `fullask_rest_framework-0.5.0/fullask_rest_framework/schemas/fields.py` & `fullask_rest_framework-0.5.1/fullask_rest_framework/schemas/fields.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.5.0/fullask_rest_framework/schemas/pagination.py` & `fullask_rest_framework-0.5.1/fullask_rest_framework/schemas/pagination.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.5.0/fullask_rest_framework/schemas/sorting.py` & `fullask_rest_framework-0.5.1/fullask_rest_framework/schemas/sorting.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from fullask_rest_framework.schemas import fields
 from fullask_rest_framework.vo.sorting import SortingRequest
 
 
 class SortingRequestSchema(Schema):
     sort_by = fields.Sorting(
         metadata={
-            "description": "The sort condition. It must conform to the format `fieldname:sortcondition (asc or desc)`."
+            "description": "The sort condition. It must conform to the format"
+            "`fieldname:sortcondition (asc or desc)`."
         }
     )
 
     @post_load
     def to_entity(self, data, **kwargs) -> SortingRequest:
         data = data.get("sort_by")
         if data:
```

### Comparing `fullask_rest_framework-0.5.0/fullask_rest_framework/utils/jwt.py` & `fullask_rest_framework-0.5.1/fullask_rest_framework/utils/jwt.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.5.0/pyproject.toml` & `fullask_rest_framework-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     "docs/",
     "tests/",
     ".github/"
 ]
 
 [tool.poetry]
 name = "fullask-rest-framework"
-version = "0.5.0"
+version = "0.5.1"
 description = ""
 authors = ["tgoddessana <twicegoddessana1229@gmail.com>"]
 
 [tool.poetry.dependencies]
 pip = "*"
 python = "^3.11"
 flask = "^2.2.3"
```

### Comparing `fullask_rest_framework-0.5.0/PKG-INFO` & `fullask_rest_framework-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fullask-rest-framework
-Version: 0.5.0
+Version: 0.5.1
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
-Metadata-Version: 2.1 Name: fullask-rest-framework Version: 0.5.0 Summary: A
+Metadata-Version: 2.1 Name: fullask-rest-framework Version: 0.5.1 Summary: A
 fully-supported flask extension to build REST API. Author-email: tgoddessana
 gmail.com> Requires-Python: >=3.9 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

