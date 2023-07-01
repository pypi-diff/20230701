# Comparing `tmp/openapi-pydantic-models-0.2.0.tar.gz` & `tmp/openapi-pydantic-models-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi-pydantic-models-0.2.0.tar", last modified: Tue Jun 27 06:25:28 2023, max compression
+gzip compressed data, was "openapi-pydantic-models-1.0.0.tar", last modified: Sat Jul  1 07:11:18 2023, max compression
```

## Comparing `openapi-pydantic-models-0.2.0.tar` & `openapi-pydantic-models-1.0.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:25:28.663330 openapi-pydantic-models-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-06-27 06:25:28.663330 openapi-pydantic-models-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 06:25:28.663330 openapi-pydantic-models-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:25:28.659330 openapi-pydantic-models-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:25:28.659330 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:25:28.659330 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/commons/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/commons/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/commons/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:25:28.663330 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/callback_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/components_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/contact_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/encoding_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/example_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/external_documentation_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/header_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/info_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/license_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/link_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/locations.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/media_type_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/oauth_flow_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/oauth_flows_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/openapi_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/operation_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/parameter_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/path_item_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/paths_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/reference_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/request_body_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/response_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/responses_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/schema_object.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/security_requirement_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/security_scheme_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/server_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/server_variable_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/specification_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/styles.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-27 06:25:18.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/tag_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:25:28.659330 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-06-27 06:25:28.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-27 06:25:28.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 06:25:28.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 06:25:28.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-27 06:25:28.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-27 06:25:28.000000 openapi-pydantic-models-0.2.0/src/openapi_pydantic_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:11:18.111245 openapi-pydantic-models-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-01 07:11:18.111245 openapi-pydantic-models-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 07:11:18.111245 openapi-pydantic-models-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:11:18.095245 openapi-pydantic-models-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:11:18.099245 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:11:18.099245 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/commons/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/commons/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/commons/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:11:18.111245 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/callback_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/components_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/contact_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/encoding_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/example_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/external_documentation_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/header_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/info_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/license_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/link_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/media_type_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/oauth_flow_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/oauth_flows_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/openapi_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/operation_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/parameter_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/path_item_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/paths_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/reference_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/request_body_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/response_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/responses_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/schema_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/security_requirement_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/security_scheme_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/server_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/server_variable_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/specification_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/styles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/tag_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:11:18.099245 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-01 07:11:18.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-01 07:11:18.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 07:11:18.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 07:11:17.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-01 07:11:18.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-01 07:11:18.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models.egg-info/top_level.txt
```

### Comparing `openapi-pydantic-models-0.2.0/.gitignore` & `openapi-pydantic-models-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.2.0/LICENSE` & `openapi-pydantic-models-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.2.0/MANIFEST.in` & `openapi-pydantic-models-1.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.2.0/PKG-INFO` & `openapi-pydantic-models-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: openapi-pydantic-models
-Version: 0.2.0
+Version: 1.0.0
 Summary: pydantic models for OpeanAPI Specification 3.1.0 objects.
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/openapi-pydantic-models
 Keywords: OpenAPI OAS
 Platform: any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -46,15 +46,15 @@
 import yaml
 
 from openapi_pydantic_models import OpenAPIObject
 
 url = "https://rapidocweb.com/specs/petstore_extended.yaml"
 response = requests.get(url)
 data = yaml.full_load(response.text)
-spec = OpenAPIObject.parse_obj(data)
+spec = OpenAPIObject.model_validate(data)
 ```
 
 All parts of OpenAPI object tree are represented by Python classes with static type
 infos:
 
 ```py
 repr(spec.paths["/pet/{petId}/uploadImage"].post.responses["200"])
@@ -72,19 +72,19 @@
             encoding=None
         )
     },
     links=None
 )
 ```
 
-Any object from object tree can always be exported back to OpenaAPI data (`dict`) via
-`dict()` method:
+Any object from object tree can always be exported back to OpenaAPI data (`model_dump`) via
+`model_dump()` method:
 
 ```py
-spec.paths["/pet/{petId}/uploadImage"].post.responses["200"].dict()
+spec.paths["/pet/{petId}/uploadImage"].post.responses["200"].model_dump()
 
 {
     'description': 'successful operation',
      'content': {
         'application/json': {
             'schema': {
                 '$ref': '#/components/schemas/ApiResponse'
@@ -101,51 +101,51 @@
 from openapi_pydantic_models import ResponseObject
 
 data = {
     "description": 'successful operation',
     "foo": "bar"
 }
 
-obj = ResponseObject.parse_obj(data)
+obj = ResponseObject.model_validate(data)
 
 # ValidationError: 1 validation error for ResponseObject
 # foo
 #   extra fields not permitted (type=value_error.extra)
 ```
 
 Any other validations defined by OpenAPI Specification are not implemented.
-`openapi-pydantic-models` intends to make programmatic editing of OpenAPI specifications easier
-and developer friendly (compared to working with "raw" `dict`-s). Complex spec
+`openapi-pydantic-models` intends to make programmatic editing of OpenAPI specifications
+easier and developer friendly (compared to working with "raw" `dict`-s). Complex spec
 validations are already implemented in other packages.
 
 Even though "extra" fields in input are not allowed, [4.9 Specification
 Extensions](https://spec.openapis.org/oas/v3.1.0#specificationExtensions) are fully and
 transparently supported for objects that allow them:
 
 ```py
 data = {
     "description": 'successful operation',
     "x-foo": "bar",
     "x-bar": [42]
 }
-obj = ResponseObject.parse_obj(data)
+obj = ResponseObject.model_validate(data)
 
 obj.extensions
 ExtensionsStorage({'x-foo': 'bar', 'x-bar': [42]})
 
-obj.dict()
+obj.model_dump()
 {'description': 'successful operation', 'x-foo': 'bar', 'x-bar': [42]}
 ```
 
 And of course, all objects can be edited:
 
 ```py
 obj.description = "ZOMG!"
 obj.extensions["x-baz"] = {1: {2: 3}}
-obj.dict()
+obj.model_dump()
 {'description': 'ZOMG!', 'x-foo': 'bar', 'x-bar': [42], 'x-baz': {1: {2: 3}}}
 ```
 
 where specification extensions are protected from invalid keys:
 
 ```py
 obj.extensions["baz"] = 34
```

### Comparing `openapi-pydantic-models-0.2.0/README.md` & `openapi-pydantic-models-1.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import yaml
 
 from openapi_pydantic_models import OpenAPIObject
 
 url = "https://rapidocweb.com/specs/petstore_extended.yaml"
 response = requests.get(url)
 data = yaml.full_load(response.text)
-spec = OpenAPIObject.parse_obj(data)
+spec = OpenAPIObject.model_validate(data)
 ```
 
 All parts of OpenAPI object tree are represented by Python classes with static type
 infos:
 
 ```py
 repr(spec.paths["/pet/{petId}/uploadImage"].post.responses["200"])
@@ -48,19 +48,19 @@
             encoding=None
         )
     },
     links=None
 )
 ```
 
-Any object from object tree can always be exported back to OpenaAPI data (`dict`) via
-`dict()` method:
+Any object from object tree can always be exported back to OpenaAPI data (`model_dump`) via
+`model_dump()` method:
 
 ```py
-spec.paths["/pet/{petId}/uploadImage"].post.responses["200"].dict()
+spec.paths["/pet/{petId}/uploadImage"].post.responses["200"].model_dump()
 
 {
     'description': 'successful operation',
      'content': {
         'application/json': {
             'schema': {
                 '$ref': '#/components/schemas/ApiResponse'
@@ -77,51 +77,51 @@
 from openapi_pydantic_models import ResponseObject
 
 data = {
     "description": 'successful operation',
     "foo": "bar"
 }
 
-obj = ResponseObject.parse_obj(data)
+obj = ResponseObject.model_validate(data)
 
 # ValidationError: 1 validation error for ResponseObject
 # foo
 #   extra fields not permitted (type=value_error.extra)
 ```
 
 Any other validations defined by OpenAPI Specification are not implemented.
-`openapi-pydantic-models` intends to make programmatic editing of OpenAPI specifications easier
-and developer friendly (compared to working with "raw" `dict`-s). Complex spec
+`openapi-pydantic-models` intends to make programmatic editing of OpenAPI specifications
+easier and developer friendly (compared to working with "raw" `dict`-s). Complex spec
 validations are already implemented in other packages.
 
 Even though "extra" fields in input are not allowed, [4.9 Specification
 Extensions](https://spec.openapis.org/oas/v3.1.0#specificationExtensions) are fully and
 transparently supported for objects that allow them:
 
 ```py
 data = {
     "description": 'successful operation',
     "x-foo": "bar",
     "x-bar": [42]
 }
-obj = ResponseObject.parse_obj(data)
+obj = ResponseObject.model_validate(data)
 
 obj.extensions
 ExtensionsStorage({'x-foo': 'bar', 'x-bar': [42]})
 
-obj.dict()
+obj.model_dump()
 {'description': 'successful operation', 'x-foo': 'bar', 'x-bar': [42]}
 ```
 
 And of course, all objects can be edited:
 
 ```py
 obj.description = "ZOMG!"
 obj.extensions["x-baz"] = {1: {2: 3}}
-obj.dict()
+obj.model_dump()
 {'description': 'ZOMG!', 'x-foo': 'bar', 'x-bar': [42], 'x-baz': {1: {2: 3}}}
 ```
 
 where specification extensions are protected from invalid keys:
 
 ```py
 obj.extensions["baz"] = 34
```

### Comparing `openapi-pydantic-models-0.2.0/pyproject.toml` & `openapi-pydantic-models-1.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [build-system]
 requires = ["setuptools>=65", "wheel"]
 
 
 [project]
 name = "openapi-pydantic-models"
-version = "0.2.0"
+version = "1.0.0"
 description = "pydantic models for OpeanAPI Specification 3.1.0 objects."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
 ]
 keywords = ["OpenAPI OAS"]
 license = { text = "MIT" }
 authors = [{ name = "Tomislav Adamic", email = "tomislav.adamic@gmail.com" }]
-dependencies = ["pydantic"]
+dependencies = ["pydantic >= 2.0"]
 
 
 [project.urls]
 Source = "https://github.com/tadams42/openapi-pydantic-models"
 
 
 [project.optional-dependencies]
```

### Comparing `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/commons/base_model.py` & `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/commons/base_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,20 +3,23 @@
 from pydantic import BaseModel as PydanticBaseModel
 
 from .utilities import exclude_blanks
 
 
 class BaseModel(PydanticBaseModel):
     class Config:
-        anystr_strip_whitespace = True
+        from_attributes = True
+        str_strip_whitespace = True
         extra = "forbid"
         use_enum_values = True
 
-    def dict(
+    def model_dump(
         self, *, by_alias: bool = True, exclude_none: bool = True, **kwargs
     ) -> dict[str, Any]:
-        retv = super().dict(exclude_none=exclude_none, by_alias=by_alias, **kwargs)
+        retv = super().model_dump(
+            exclude_none=exclude_none, by_alias=by_alias, **kwargs
+        )
 
         if exclude_none:
             retv = exclude_blanks(retv)
 
         return retv or dict()
```

### Comparing `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/commons/utilities.py` & `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/commons/utilities.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/__init__.py` & `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/callback_object.py` & `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/callback_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         if ExtensionsStorage.is_key(str(key)):
             raise KeyError(f'Extensions must be accessed via self.extensions["{key}"]!')
 
         v = None
         for typ in [ReferenceObject, PathItemObject]:
             if v is None:
                 try:
-                    v = typ.parse_obj(value)
+                    v = typ.model_validate(value)
                 except Exception:
                     pass
         if v is None:
             raise ValueError(v)
 
         self._data.__setitem__(str(key), v)
 
@@ -75,41 +75,41 @@
 
     def __len__(self) -> int:
         return self._data.__len__()
 
     def __str__(self) -> str:
         return str(
             {
-                k: v.dict(by_alias=True, exclude_none=False)
+                k: v.model_dump(by_alias=True, exclude_none=False)
                 if isinstance(v, (ReferenceObject, PathItemObject))
                 else v
                 for k, v in self._data.items()
             }
         )
 
     def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}("
             + repr(
                 {
-                    k: v.dict(by_alias=True, exclude_none=False)
+                    k: v.model_dump(by_alias=True, exclude_none=False)
                     if isinstance(v, (ReferenceObject, PathItemObject))
                     else v
                     for k, v in self._data.items()
                 }
             )
             + ")"
         )
 
-    def dict(
+    def model_dump(
         self, *, by_alias: bool = True, exclude_none: bool = True, **kwargs
     ) -> dict[str, Any]:
         retv = {
             k: (
-                v.dict(by_alias=by_alias, exclude_none=exclude_none, **kwargs)
+                v.model_dump(by_alias=by_alias, exclude_none=exclude_none, **kwargs)
                 if isinstance(v, (ReferenceObject, PathItemObject))
                 else v
             )
             for k, v in itertools.chain(self._data.items(), self._ext.items())
         }
 
         if exclude_none:
```

### Comparing `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/components_object.py` & `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/components_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/encoding_object.py` & `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/encoding_object.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING
 
 from .reference_object import ReferenceObject
 from .specification_extensions import SpecificationExtendable
 from .styles import Styles
 
 if TYPE_CHECKING:
     from .header_object import HeaderObject
```

### Comparing `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/header_object.py` & `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/header_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/media_type_object.py` & `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/media_type_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/openapi_object.py` & `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/openapi_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/operation_object.py` & `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/operation_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/parameter_object.py` & `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/parameter_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/path_item_object.py` & `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/path_item_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/paths_object.py` & `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/paths_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         if ExtensionsStorage.is_key(str(key)):
             raise KeyError(f'Extensions must be accessed via self.extensions["{key}"]!')
 
         v = None
         for typ in [PathItemObject]:
             if v is None:
                 try:
-                    v = typ.parse_obj(value)
+                    v = typ.model_validate(value)
                 except Exception:
                     pass
         if v is None:
             raise ValueError(v)
 
         self._data.__setitem__(str(key), v)
 
@@ -85,41 +85,41 @@
 
     def __len__(self) -> int:
         return self._data.__len__()
 
     def __str__(self) -> str:
         return str(
             {
-                k: v.dict(by_alias=True, exclude_none=False)
+                k: v.model_dump(by_alias=True, exclude_none=False)
                 if isinstance(v, PathItemObject)
                 else v
                 for k, v in self._data.items()
             }
         )
 
     def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}("
             + repr(
                 {
-                    k: v.dict(by_alias=True, exclude_none=False)
+                    k: v.model_dump(by_alias=True, exclude_none=False)
                     if isinstance(v, PathItemObject)
                     else v
                     for k, v in self._data.items()
                 }
             )
             + ")"
         )
 
-    def dict(
+    def model_dump(
         self, *, by_alias: bool = True, exclude_none: bool = True, **kwargs
     ) -> dict[str, Any]:
         retv = {
             k: (
-                v.dict(by_alias=by_alias, exclude_none=exclude_none, **kwargs)
+                v.model_dump(by_alias=by_alias, exclude_none=exclude_none, **kwargs)
                 if isinstance(v, PathItemObject)
                 else v
             )
             for k, v in itertools.chain(self._data.items(), self._ext.items())
         }
 
         if exclude_none:
```

### Comparing `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/responses_object.py` & `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/responses_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         if ExtensionsStorage.is_key(str(key)):
             raise KeyError(f'Extensions must be accessed via self.extensions["{key}"]!')
 
         v = None
         for typ in [ReferenceObject, ResponseObject]:
             if v is None:
                 try:
-                    v = typ.parse_obj(value)
+                    v = typ.model_validate(value)
                 except Exception:
                     pass
         if v is None:
             raise ValueError(v)
 
         self._data.__setitem__(str(key), v)
 
@@ -78,43 +78,43 @@
         return self._data.__iter__()
 
     def __len__(self) -> int:
         return self._data.__len__()
 
     def __str__(self) -> str:
         data = {
-            k: v.dict(by_alias=True, exclude_none=False)
+            k: v.model_dump(by_alias=True, exclude_none=False)
             if isinstance(v, (ReferenceObject, ResponseObject))
             else v
             for k, v in self._data.items()
         }
 
         if self.default:
-            data["default"] = self.default.dict(by_alias=True, exclude_none=False)
+            data["default"] = self.default.model_dump(by_alias=True, exclude_none=False)
 
         return str(data)
 
     def __repr__(self) -> str:
         data = {
-            k: v.dict(by_alias=True, exclude_none=False)
+            k: v.model_dump(by_alias=True, exclude_none=False)
             if isinstance(v, (ReferenceObject, ResponseObject))
             else v
             for k, v in self._data.items()
         }
         if self.default:
-            data["default"] = self.default.dict(by_alias=True, exclude_none=False)
+            data["default"] = self.default.model_dump(by_alias=True, exclude_none=False)
 
         return f"{self.__class__.__name__}({repr(data)})"
 
-    def dict(
+    def model_dump(
         self, *, by_alias: bool = True, exclude_none: bool = True, **kwargs
     ) -> dict[str, Any]:
         retv = {
             k: (
-                v.dict(by_alias=by_alias, exclude_none=exclude_none, **kwargs)
+                v.model_dump(by_alias=by_alias, exclude_none=exclude_none, **kwargs)
                 if isinstance(v, (ReferenceObject, ResponseObject))
                 else v
             )
             for k, v in itertools.chain(self._data.items(), self._ext.items())
         }
 
         if exclude_none:
```

### Comparing `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/security_scheme_object.py` & `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/security_scheme_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models/openapi_3_1/specification_extensions.py` & `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/specification_extensions.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,24 +78,24 @@
 
         obj = SomeModel(**data)
 
         repr(obj)
         >>> SomeModel(attr='...')
         repr(obj.extensions)
         >>> "ExtensionsStorage({'x-foo': 42, 'x-bar': ['baz']})"
-        obj.dict()
+        obj.model_dump()
         >>> {'attr': '...', 'x-foo': 42, 'x-bar': ['baz']}
 
-        obj = SomeModel.parse_obj(data)
+        obj = SomeModel.model_validate(data)
 
         repr(obj)
         >>> SomeModel(attr='...')
         repr(obj.extensions)
         >>> "ExtensionsStorage({'x-foo': 42, 'x-bar': ['baz']})"
-        obj.dict()
+        obj.model_dump()
         >>> {'attr': '...', 'x-foo': 42, 'x-bar': ['baz']}
     """
 
     _ext: ExtensionsStorage = PrivateAttr(default_factory=ExtensionsStorage)
 
     def __init__(self, **data):
         super().__init__(
@@ -103,19 +103,19 @@
         )
         self._ext = ExtensionsStorage(data)
 
     @property
     def extensions(self) -> ExtensionsStorage:
         return self._ext
 
-    def dict(
+    def model_dump(
         self, *, by_alias: bool = True, exclude_none: bool = True, **kwargs
     ) -> dict[str, Any]:
         retv = (
-            super().dict(exclude_none=exclude_none, by_alias=by_alias, **kwargs)
+            super().model_dump(exclude_none=exclude_none, by_alias=by_alias, **kwargs)
             or dict()
         )
 
         for k, v in self._ext.items():
             retv[str(k)] = v
 
         if exclude_none:
```

### Comparing `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models.egg-info/PKG-INFO` & `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: openapi-pydantic-models
-Version: 0.2.0
+Version: 1.0.0
 Summary: pydantic models for OpeanAPI Specification 3.1.0 objects.
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/openapi-pydantic-models
 Keywords: OpenAPI OAS
 Platform: any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -46,15 +46,15 @@
 import yaml
 
 from openapi_pydantic_models import OpenAPIObject
 
 url = "https://rapidocweb.com/specs/petstore_extended.yaml"
 response = requests.get(url)
 data = yaml.full_load(response.text)
-spec = OpenAPIObject.parse_obj(data)
+spec = OpenAPIObject.model_validate(data)
 ```
 
 All parts of OpenAPI object tree are represented by Python classes with static type
 infos:
 
 ```py
 repr(spec.paths["/pet/{petId}/uploadImage"].post.responses["200"])
@@ -72,19 +72,19 @@
             encoding=None
         )
     },
     links=None
 )
 ```
 
-Any object from object tree can always be exported back to OpenaAPI data (`dict`) via
-`dict()` method:
+Any object from object tree can always be exported back to OpenaAPI data (`model_dump`) via
+`model_dump()` method:
 
 ```py
-spec.paths["/pet/{petId}/uploadImage"].post.responses["200"].dict()
+spec.paths["/pet/{petId}/uploadImage"].post.responses["200"].model_dump()
 
 {
     'description': 'successful operation',
      'content': {
         'application/json': {
             'schema': {
                 '$ref': '#/components/schemas/ApiResponse'
@@ -101,51 +101,51 @@
 from openapi_pydantic_models import ResponseObject
 
 data = {
     "description": 'successful operation',
     "foo": "bar"
 }
 
-obj = ResponseObject.parse_obj(data)
+obj = ResponseObject.model_validate(data)
 
 # ValidationError: 1 validation error for ResponseObject
 # foo
 #   extra fields not permitted (type=value_error.extra)
 ```
 
 Any other validations defined by OpenAPI Specification are not implemented.
-`openapi-pydantic-models` intends to make programmatic editing of OpenAPI specifications easier
-and developer friendly (compared to working with "raw" `dict`-s). Complex spec
+`openapi-pydantic-models` intends to make programmatic editing of OpenAPI specifications
+easier and developer friendly (compared to working with "raw" `dict`-s). Complex spec
 validations are already implemented in other packages.
 
 Even though "extra" fields in input are not allowed, [4.9 Specification
 Extensions](https://spec.openapis.org/oas/v3.1.0#specificationExtensions) are fully and
 transparently supported for objects that allow them:
 
 ```py
 data = {
     "description": 'successful operation',
     "x-foo": "bar",
     "x-bar": [42]
 }
-obj = ResponseObject.parse_obj(data)
+obj = ResponseObject.model_validate(data)
 
 obj.extensions
 ExtensionsStorage({'x-foo': 'bar', 'x-bar': [42]})
 
-obj.dict()
+obj.model_dump()
 {'description': 'successful operation', 'x-foo': 'bar', 'x-bar': [42]}
 ```
 
 And of course, all objects can be edited:
 
 ```py
 obj.description = "ZOMG!"
 obj.extensions["x-baz"] = {1: {2: 3}}
-obj.dict()
+obj.model_dump()
 {'description': 'ZOMG!', 'x-foo': 'bar', 'x-bar': [42], 'x-baz': {1: {2: 3}}}
 ```
 
 where specification extensions are protected from invalid keys:
 
 ```py
 obj.extensions["baz"] = 34
```

### Comparing `openapi-pydantic-models-0.2.0/src/openapi_pydantic_models.egg-info/SOURCES.txt` & `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

