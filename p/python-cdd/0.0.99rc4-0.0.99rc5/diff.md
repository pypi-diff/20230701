# Comparing `tmp/python-cdd-0.0.99rc4.tar.gz` & `tmp/python-cdd-0.0.99rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-cdd-0.0.99rc4.tar", last modified: Mon Mar 27 20:41:04 2023, max compression
+gzip compressed data, was "python-cdd-0.0.99rc5.tar", last modified: Sat Jul  1 02:50:09 2023, max compression
```

## Comparing `python-cdd-0.0.99rc4.tar` & `python-cdd-0.0.99rc5.tar`

### file list

```diff
@@ -1,230 +1,230 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.245643 python-cdd-0.0.99rc4/
--rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/LICENSE-APACHE
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/LICENSE-MIT
--rw-r--r--   0 runner    (1001) docker     (123)    31962 2023-03-27 20:41:04.245643 python-cdd-0.0.99rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    30254 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.217641 python-cdd-0.0.99rc4/cdd/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16899 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.217641 python-cdd-0.0.99rc4/cdd/argparse_function/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/argparse_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12171 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/argparse_function/emit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/argparse_function/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.217641 python-cdd-0.0.99rc4/cdd/argparse_function/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/argparse_function/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/argparse_function/utils/emit_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.217641 python-cdd-0.0.99rc4/cdd/class_/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/class_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/class_/emit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12911 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/class_/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.217641 python-cdd-0.0.99rc4/cdd/class_/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/class_/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/class_/utils/emit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/class_/utils/parse_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.221642 python-cdd-0.0.99rc4/cdd/compound/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/compound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/compound/doctrans.py
--rw-r--r--   0 runner    (1001) docker     (123)    13479 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/compound/doctrans_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9111 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/compound/exmod.py
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/compound/exmod_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/compound/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    15371 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/compound/gen_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.221642 python-cdd-0.0.99rc4/cdd/compound/openapi/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/compound/openapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/compound/openapi/emit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/compound/openapi/gen_openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/compound/openapi/gen_routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/compound/openapi/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.221642 python-cdd-0.0.99rc4/cdd/compound/openapi/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/compound/openapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/compound/openapi/utils/emit_openapi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25032 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/compound/openapi/utils/emit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/compound/openapi/utils/parse_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/compound/sync_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.221642 python-cdd-0.0.99rc4/cdd/docstring/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/docstring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/docstring/emit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/docstring/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.221642 python-cdd-0.0.99rc4/cdd/docstring/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/docstring/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/docstring/utils/emit_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.221642 python-cdd-0.0.99rc4/cdd/function/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/function/emit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/function/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.221642 python-cdd-0.0.99rc4/cdd/function/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/function/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/function/utils/emit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/function/utils/parse_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.221642 python-cdd-0.0.99rc4/cdd/json_schema/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/json_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/json_schema/emit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/json_schema/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.225642 python-cdd-0.0.99rc4/cdd/json_schema/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/json_schema/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/json_schema/utils/emit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/json_schema/utils/parse_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.225642 python-cdd-0.0.99rc4/cdd/pydantic/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/pydantic/emit.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/pydantic/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.225642 python-cdd-0.0.99rc4/cdd/routes/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.225642 python-cdd-0.0.99rc4/cdd/routes/emit/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/routes/emit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/routes/emit/bottle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/routes/emit/bottle_constants_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.225642 python-cdd-0.0.99rc4/cdd/routes/parse/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/routes/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/routes/parse/bottle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/routes/parse/bottle_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/routes/parse/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/routes/parse/fastapi_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.225642 python-cdd-0.0.99rc4/cdd/shared/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11812 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/shared/ast_cst_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    54988 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/shared/ast_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/shared/conformance.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/shared/cst.py
--rw-r--r--   0 runner    (1001) docker     (123)    17254 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/shared/cst_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12251 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/shared/defaults_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    36685 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/shared/docstring_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)    24541 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/shared/docstring_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.225642 python-cdd-0.0.99rc4/cdd/shared/emit/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/shared/emit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/shared/emit/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.229642 python-cdd-0.0.99rc4/cdd/shared/emit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/shared/emit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/shared/emit/utils/emitter_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.229642 python-cdd-0.0.99rc4/cdd/shared/parse/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/shared/parse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.229642 python-cdd-0.0.99rc4/cdd/shared/parse/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/shared/parse/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/shared/parse/utils/parser_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/shared/pkg_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    33717 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/shared/pure_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/shared/source_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.229642 python-cdd-0.0.99rc4/cdd/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11956 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/sqlalchemy/emit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/sqlalchemy/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.229642 python-cdd-0.0.99rc4/cdd/sqlalchemy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/sqlalchemy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11813 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/sqlalchemy/utils/parse_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/sqlalchemy/utils/shared_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.229642 python-cdd-0.0.99rc4/cdd/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.233642 python-cdd-0.0.99rc4/cdd/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34014 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/tests/mocks/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    47192 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/tests/mocks/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/tests/mocks/cst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/tests/mocks/cstify.py
--rw-r--r--   0 runner    (1001) docker     (123)    35593 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/tests/mocks/docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/tests/mocks/doctrans.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/tests/mocks/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/tests/mocks/exmod.py
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/tests/mocks/fastapi_routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/tests/mocks/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    42393 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/tests/mocks/ir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/tests/mocks/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    33730 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/tests/mocks/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/tests/mocks/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/tests/mocks/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-03-27 20:40:13.000000 python-cdd-0.0.99rc4/cdd/tests/mocks/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)    18892 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/mocks/sqlalchemy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.233642 python-cdd-0.0.99rc4/cdd/tests/test_argparse_function/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_argparse_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_argparse_function/test_emit_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_argparse_function/test_parse_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_ast_equality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.233642 python-cdd-0.0.99rc4/cdd/tests/test_class/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_class/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_class/test_emit_class_.py
--rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_class/test_parse_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.233642 python-cdd-0.0.99rc4/cdd/tests/test_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_cli/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_cli/test_cli_doctrans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_cli/test_cli_exmod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_cli/test_cli_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_cli/test_cli_gen_routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_cli/test_cli_openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_cli/test_cli_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_cli/test_cli_sync_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.237643 python-cdd-0.0.99rc4/cdd/tests/test_compound/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_compound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_compound/test_doctrans.py
--rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_compound/test_doctrans_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25473 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_compound/test_exmod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_compound/test_exmod_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13007 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_compound/test_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_compound/test_gen_routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_compound/test_gen_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_compound/test_openapi_bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_compound/test_openapi_sub.py
--rw-r--r--   0 runner    (1001) docker     (123)    15128 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_compound/test_sync_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.237643 python-cdd-0.0.99rc4/cdd/tests/test_docstring/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_docstring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_docstring/test_emit_docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_docstring/test_parse_docstring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.237643 python-cdd-0.0.99rc4/cdd/tests/test_emit/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_emit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_emit/test_emit_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_emit/test_emitter_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_emit/test_emitters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.237643 python-cdd-0.0.99rc4/cdd/tests/test_function/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_function/test_emit_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_function/test_parse_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.237643 python-cdd-0.0.99rc4/cdd/tests/test_json_schema/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_json_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_json_schema/test_emit_json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_json_schema/test_emit_json_schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_json_schema/test_parse_json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_json_schema/test_parse_json_schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13653 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_marshall_docstring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.237643 python-cdd-0.0.99rc4/cdd/tests/test_parse/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8819 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_parse/test_parser_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_parse/test_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.237643 python-cdd-0.0.99rc4/cdd/tests/test_pydantic/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_pydantic/test_emit_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_pydantic/test_parse_pydantic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.241643 python-cdd-0.0.99rc4/cdd/tests/test_routes/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_routes/test_bottle_route_emit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_routes/test_bottle_route_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_routes/test_fastapi_routes_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_routes/test_route_emit.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_routes/test_route_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.241643 python-cdd-0.0.99rc4/cdd/tests/test_shared/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15916 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_shared/test_ast_cst_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    41239 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_shared/test_ast_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_shared/test_conformance.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_shared/test_cst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_shared/test_cst_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_shared/test_default_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8809 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_shared/test_docstring_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_shared/test_pkg_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_shared/test_pure_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_shared/test_source_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.241643 python-cdd-0.0.99rc4/cdd/tests/test_sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_sqlalchemy/test_emit_sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13020 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_sqlalchemy/test_emit_sqlalchemy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_sqlalchemy/test_parse_sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_sqlalchemy/test_parse_sqlalchemy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/test_utils_for_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    12968 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/cdd/tests/utils_for_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:41:04.245643 python-cdd-0.0.99rc4/python_cdd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    31962 2023-03-27 20:41:04.000000 python-cdd-0.0.99rc4/python_cdd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-03-27 20:41:04.000000 python-cdd-0.0.99rc4/python_cdd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 20:41:04.000000 python-cdd-0.0.99rc4/python_cdd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-27 20:41:04.000000 python-cdd-0.0.99rc4/python_cdd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-27 20:41:04.000000 python-cdd-0.0.99rc4/python_cdd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 20:41:04.245643 python-cdd-0.0.99rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-03-27 20:40:14.000000 python-cdd-0.0.99rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.181331 python-cdd-0.0.99rc5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/LICENSE-APACHE
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/LICENSE-MIT
+-rw-r--r--   0 runner    (1001) docker     (123)    33371 2023-07-01 02:50:09.181331 python-cdd-0.0.99rc5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31663 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.157331 python-cdd-0.0.99rc5/cdd/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17081 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.157331 python-cdd-0.0.99rc5/cdd/argparse_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/argparse_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12171 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/argparse_function/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/argparse_function/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.157331 python-cdd-0.0.99rc5/cdd/argparse_function/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/argparse_function/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/argparse_function/utils/emit_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.157331 python-cdd-0.0.99rc5/cdd/class_/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/class_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/class_/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12911 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/class_/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.157331 python-cdd-0.0.99rc5/cdd/class_/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/class_/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/class_/utils/emit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/class_/utils/parse_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.161332 python-cdd-0.0.99rc5/cdd/compound/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/doctrans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13479 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/doctrans_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/exmod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/exmod_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/gen_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.161332 python-cdd-0.0.99rc5/cdd/compound/openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/openapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/openapi/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/openapi/gen_openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/openapi/gen_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/openapi/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.161332 python-cdd-0.0.99rc5/cdd/compound/openapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/openapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/openapi/utils/emit_openapi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25134 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/openapi/utils/emit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/openapi/utils/parse_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/compound/sync_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.161332 python-cdd-0.0.99rc5/cdd/docstring/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/docstring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/docstring/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/docstring/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.161332 python-cdd-0.0.99rc5/cdd/docstring/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/docstring/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/docstring/utils/emit_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.161332 python-cdd-0.0.99rc5/cdd/function/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/function/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/function/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.161332 python-cdd-0.0.99rc5/cdd/function/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/function/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/function/utils/emit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/function/utils/parse_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.161332 python-cdd-0.0.99rc5/cdd/json_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/json_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/json_schema/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/json_schema/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.161332 python-cdd-0.0.99rc5/cdd/json_schema/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/json_schema/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/json_schema/utils/emit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/json_schema/utils/parse_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.165331 python-cdd-0.0.99rc5/cdd/pydantic/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/pydantic/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/pydantic/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.165331 python-cdd-0.0.99rc5/cdd/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.165331 python-cdd-0.0.99rc5/cdd/routes/emit/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/routes/emit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/routes/emit/bottle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/routes/emit/bottle_constants_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.165331 python-cdd-0.0.99rc5/cdd/routes/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/routes/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/routes/parse/bottle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/routes/parse/bottle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/routes/parse/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/routes/parse/fastapi_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.165331 python-cdd-0.0.99rc5/cdd/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11812 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/ast_cst_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59574 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/ast_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/conformance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/cst.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17254 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/cst_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12251 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/defaults_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36707 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/docstring_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24541 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/docstring_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.165331 python-cdd-0.0.99rc5/cdd/shared/emit/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/emit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/emit/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.165331 python-cdd-0.0.99rc5/cdd/shared/emit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/emit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/emit/utils/emitter_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.165331 python-cdd-0.0.99rc5/cdd/shared/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/parse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.165331 python-cdd-0.0.99rc5/cdd/shared/parse/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/parse/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/parse/utils/parser_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/pkg_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35026 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/pure_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/shared/source_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.165331 python-cdd-0.0.99rc5/cdd/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12073 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/sqlalchemy/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/sqlalchemy/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.169331 python-cdd-0.0.99rc5/cdd/sqlalchemy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/sqlalchemy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11813 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/sqlalchemy/utils/parse_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/sqlalchemy/utils/shared_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.169331 python-cdd-0.0.99rc5/cdd/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.169331 python-cdd-0.0.99rc5/cdd/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34014 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47192 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/cst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/cstify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35593 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/doctrans.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/exmod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/fastapi_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42393 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33730 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18892 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/mocks/sqlalchemy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.169331 python-cdd-0.0.99rc5/cdd/tests/test_argparse_function/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_argparse_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_argparse_function/test_emit_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_argparse_function/test_parse_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_ast_equality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.169331 python-cdd-0.0.99rc5/cdd/tests/test_class/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_class/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_class/test_emit_class_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_class/test_parse_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.173331 python-cdd-0.0.99rc5/cdd/tests/test_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli_doctrans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli_exmod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli_gen_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli_openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli_sync_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.173331 python-cdd-0.0.99rc5/cdd/tests/test_compound/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_compound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_compound/test_doctrans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_compound/test_doctrans_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24367 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_compound/test_exmod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_compound/test_exmod_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13007 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_compound/test_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_compound/test_gen_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_compound/test_gen_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_compound/test_openapi_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_compound/test_openapi_sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15128 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_compound/test_sync_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.173331 python-cdd-0.0.99rc5/cdd/tests/test_docstring/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_docstring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_docstring/test_emit_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_docstring/test_parse_docstring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.177332 python-cdd-0.0.99rc5/cdd/tests/test_emit/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_emit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_emit/test_emit_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_emit/test_emitter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_emit/test_emitters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.177332 python-cdd-0.0.99rc5/cdd/tests/test_function/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_function/test_emit_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_function/test_parse_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.177332 python-cdd-0.0.99rc5/cdd/tests/test_json_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_json_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_json_schema/test_emit_json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_json_schema/test_emit_json_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_json_schema/test_parse_json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_json_schema/test_parse_json_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13653 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_marshall_docstring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.177332 python-cdd-0.0.99rc5/cdd/tests/test_parse/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8819 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_parse/test_parser_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_parse/test_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.177332 python-cdd-0.0.99rc5/cdd/tests/test_pydantic/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_pydantic/test_emit_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_pydantic/test_parse_pydantic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.177332 python-cdd-0.0.99rc5/cdd/tests/test_routes/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_routes/test_bottle_route_emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_routes/test_bottle_route_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_routes/test_fastapi_routes_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_routes/test_route_emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_routes/test_route_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.181331 python-cdd-0.0.99rc5/cdd/tests/test_shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15916 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_shared/test_ast_cst_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41239 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_shared/test_ast_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_shared/test_conformance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_shared/test_cst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_shared/test_cst_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_shared/test_default_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8809 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_shared/test_docstring_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_shared/test_pkg_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_shared/test_pure_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_shared/test_source_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.181331 python-cdd-0.0.99rc5/cdd/tests/test_sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_sqlalchemy/test_emit_sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_sqlalchemy/test_emit_sqlalchemy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_sqlalchemy/test_parse_sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_sqlalchemy/test_parse_sqlalchemy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/test_utils_for_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12968 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/cdd/tests/utils_for_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 02:50:09.181331 python-cdd-0.0.99rc5/python_cdd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    33371 2023-07-01 02:50:09.000000 python-cdd-0.0.99rc5/python_cdd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-07-01 02:50:09.000000 python-cdd-0.0.99rc5/python_cdd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 02:50:09.000000 python-cdd-0.0.99rc5/python_cdd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-01 02:50:09.000000 python-cdd-0.0.99rc5/python_cdd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-01 02:50:09.000000 python-cdd-0.0.99rc5/python_cdd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 02:50:09.181331 python-cdd-0.0.99rc5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-01 02:49:26.000000 python-cdd-0.0.99rc5/setup.py
```

### Comparing `python-cdd-0.0.99rc4/LICENSE-APACHE` & `python-cdd-0.0.99rc5/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/LICENSE-MIT` & `python-cdd-0.0.99rc5/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/PKG-INFO` & `python-cdd-0.0.99rc5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-cdd
-Version: 0.0.99rc4
+Version: 0.0.99rc5
 Summary: Open API to/fro routes, models, and tests. Convert between docstrings, classes, methods, argparse, pydantic, and SQLalchemy.
 Home-page: https://github.com/offscale/cdd-python
 Author: Samuel Marks
 Author-email: 807580+SamuelMarks@users.noreply.github.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -512,21 +512,20 @@
   inline ([PEP484](https://python.org/dev/peps/pep-0484)–style))
 - Switch between docstring formats (to/from {numpy, ReST, google})
 - Desktop GUI with wxWidgets, from the argparse layer through [Gooey](https://github.com/chriskiehl/Gooey) [one liner]
 
 ## CLI for this project
 
     $ python -m cdd --help
-    
     usage: python -m cdd [-h] [--version]
                          {sync_properties,sync,gen,gen_routes,openapi,doctrans,exmod}
                          ...
     
     Open API to/fro routes, models, and tests. Convert between docstrings,
-    classes, methods, argparse, and SQLalchemy.
+    classes, methods, argparse, pydantic, and SQLalchemy.
     
     positional arguments:
       {sync_properties,sync,gen,gen_routes,openapi,doctrans,exmod}
         sync_properties     Synchronise one or more properties between input and
                             input_str Python files
         sync                Force argparse, classes, and/or methods to be
                             equivalent
@@ -543,43 +542,44 @@
     options:
       -h, --help            show this help message and exit
       --version             show program's version number and exit
 
 ### `sync`
 
     $ python -m cdd sync --help
-
     usage: python -m cdd sync [-h] [--argparse-function ARGPARSE_FUNCTIONS]
                               [--argparse-function-name ARGPARSE_FUNCTION_NAMES]
                               [--class CLASSES] [--class-name CLASS_NAMES]
                               [--function FUNCTIONS]
-                              [--function-name FUNCTION_NAMES] --truth
-                              {argparse_function,class,function}
+                              [--function-name FUNCTION_NAMES] [--no-word-wrap]
+                              --truth
+                              {argparse_function,class,function,sqlalchemy,sqlalchemy_table}
     
     options:
       -h, --help            show this help message and exit
       --argparse-function ARGPARSE_FUNCTIONS
                             File where argparse function is `def`ined.
       --argparse-function-name ARGPARSE_FUNCTION_NAMES
                             Name of argparse function.
       --class CLASSES       File where class `class` is declared.
       --class-name CLASS_NAMES
                             Name of `class`
       --function FUNCTIONS  File where function is `def`ined.
       --function-name FUNCTION_NAMES
                             Name of Function. If method, use Python resolution
                             syntax, i.e., ClassName.function_name
-      --truth {argparse_function,class,function}
+      --no-word-wrap        Whether word-wrap is disabled (on emission). None
+                            enables word-wrap. Defaults to None.
+      --truth {argparse_function,class,function,sqlalchemy,sqlalchemy_table}
                             Single source of truth. Others will be generated from
                             this. Will run with first found choice.
 
 ### `sync_properties`
 
     $ python -m cdd sync_properties --help
-
     usage: python -m cdd sync_properties [-h] --input-filename INPUT_FILENAME
                                          --input-param INPUT_PARAMS [--input-eval]
                                          --output-filename OUTPUT_FILENAME
                                          --output-param OUTPUT_PARAMS
                                          [--output-param-wrap OUTPUT_PARAM_WRAP]
     
     options:
@@ -600,54 +600,59 @@
       --output-param-wrap OUTPUT_PARAM_WRAP
                             Wrap all input_str params with this. E.g.,
                             `Optional[Union[{output_param}, str]]`
 
 ### `gen`
 
     $ python -m cdd gen --help
-
     usage: python -m cdd gen [-h] --name-tpl NAME_TPL --input-mapping
                              INPUT_MAPPING [--prepend PREPEND]
                              [--imports-from-file IMPORTS_FROM_FILE]
-                             [--parse {argparse,class,function,sqlalchemy,sqlalchemy_table}]
+                             [--parse {argparse,class,function,json_schema,pydantic,sqlalchemy,sqlalchemy_table,infer}]
                              --emit
-                             {argparse,class,function,sqlalchemy,sqlalchemy_table}
+                             {argparse,class,function,json_schema,pydantic,sqlalchemy,sqlalchemy_table}
                              --output-filename OUTPUT_FILENAME [--emit-call]
-                             [--decorator DECORATOR_LIST]
+                             [--emit-and-infer-imports] [--no-word-wrap]
+                             [--decorator DECORATOR_LIST] [--phase PHASE]
     
-    optional arguments:
+    options:
       -h, --help            show this help message and exit
       --name-tpl NAME_TPL   Template for the name, e.g., `{name}Config`.
       --input-mapping INPUT_MAPPING
                             Fully-qualified module, filepath, or directory.
       --prepend PREPEND     Prepend file with this. Use '\n' for newlines.
       --imports-from-file IMPORTS_FROM_FILE
                             Extract imports from file and append to `output_file`.
                             If module or other symbol path given, resolve file
                             then use it.
-      --parse {argparse,class,function,sqlalchemy,sqlalchemy_table}
+      --parse {argparse,class,function,json_schema,pydantic,sqlalchemy,sqlalchemy_table,infer}
                             What type the input is.
-      --emit {argparse,class,function,sqlalchemy,sqlalchemy_table}
-                            What type to generate.
+      --emit {argparse,class,function,json_schema,pydantic,sqlalchemy,sqlalchemy_table}
+                            Which type to generate.
       --output-filename OUTPUT_FILENAME, -o OUTPUT_FILENAME
                             Output file to write to.
       --emit-call           Whether to place all the previous body into a new
                             `__call__` internal function
+      --emit-and-infer-imports
+                            Whether to emit and infer imports at the top of the
+                            generated code
+      --no-word-wrap        Whether word-wrap is disabled (on emission). None
+                            enables word-wrap. Defaults to None.
       --decorator DECORATOR_LIST
                             List of decorators.
-
+      --phase PHASE         Which phase to run through. E.g., SQLalchemy may
+                            require multiple phases to resolve foreign keys.
 
 PS: If you're outputting JSON-schema and want a file per schema then:
 
     python -c 'import sys,json,os; f=open(sys.argv[1], "rt"); d=json.load(f); f.close(); [(lambda f: json.dump(sc,f) or f.close())(open(os.path.join(os.path.dirname(sys.argv[1]), sc["$id"].rpartition("/")[2]), "wt")) for sc in d["schemas"]]' <path_to_json_file>
 
 ### `gen_routes`
 
     $ python -m cdd gen_routes --help
-
     usage: python -m cdd gen_routes [-h] --crud {CRUD,CR,C,R,U,D,CR,CU,CD,CRD}
                                     [--app-name APP_NAME] --model-path MODEL_PATH
                                     --model-name MODEL_NAME --routes-path
                                     ROUTES_PATH [--route ROUTE]
     
     options:
       -h, --help            show this help message and exit
@@ -666,74 +671,79 @@
                             'foo/routes'
       --route ROUTE         Name of the route, defaults to
                             `/api/{model_name.lower()}`
 
 ### `openapi`
 
     $ python -m cdd openapi --help
-
     usage: python -m cdd openapi [-h] [--app-name APP_NAME] --model-paths
-                                 MODEL_PATHS --routes-paths
-                                 [ROUTES_PATHS [ROUTES_PATHS ...]]
+                                 MODEL_PATHS --routes-paths [ROUTES_PATHS ...]
     
-    optional arguments:
+    options:
       -h, --help            show this help message and exit
       --app-name APP_NAME   Name of app (e.g., `app_name = Bottle();
                             @app_name.get('/api') def slash(): pass`)
       --model-paths MODEL_PATHS
                             Python module resolution (foo.models) or filepath
                             (foo/models)
-      --routes-paths [ROUTES_PATHS [ROUTES_PATHS ...]]
+      --routes-paths [ROUTES_PATHS ...]
                             Python module resolution 'foo.routes' or filepath
                             'foo/routes'
 
 ### `doctrans`
 
     $ python -m cdd doctrans --help
-    
     usage: python -m cdd doctrans [-h] --filename FILENAME --format
                                   {rest,google,numpydoc}
-                                  (--type-annotations | --no-type-annotations)
+                                  (--type-annotations | --no-type-annotations | --no-word-wrap)
     
     options:
       -h, --help            show this help message and exit
       --filename FILENAME   Python file to convert docstrings within. Edited in
                             place.
       --format {rest,google,numpydoc}
                             The docstring format to replace existing format with.
       --type-annotations    Inline the type, i.e., annotate PEP484 (outside
                             docstring. Requires 3.6+)
       --no-type-annotations
                             Ensure all types are in docstring (rather than a
                             PEP484 type annotation)
+      --no-word-wrap        Whether word-wrap is disabled (on emission). None
+                            enables word-wrap. Defaults to None.
 
 ### `exmod`
 
     $ python -m cdd exmod --help
-    
     usage: python -m cdd exmod [-h] --module MODULE --emit
-                               {argparse,class,function,sqlalchemy,sqlalchemy_table}
-                               [--blacklist BLACKLIST] [--whitelist WHITELIST]
-                               --output-directory OUTPUT_DIRECTORY [--dry-run]
+                               {argparse,class,function,json_schema,pydantic,sqlalchemy,sqlalchemy_table}
+                               [--no-word-wrap] [--blacklist BLACKLIST]
+                               [--whitelist WHITELIST] --output-directory
+                               OUTPUT_DIRECTORY
+                               [--target-module-name TARGET_MODULE_NAME]
+                               [--dry-run]
     
     options:
       -h, --help            show this help message and exit
       --module MODULE, -m MODULE
                             The module or fully-qualified name (FQN) to expose.
-      --emit {argparse,class,function,sqlalchemy,sqlalchemy_table}
-                            What type to generate.
+      --emit {argparse,class,function,json_schema,pydantic,sqlalchemy,sqlalchemy_table}
+                            Which type to generate.
+      --no-word-wrap        Whether word-wrap is disabled (on emission). None
+                            enables word-wrap. Defaults to None.
       --blacklist BLACKLIST
                             Modules/FQN to omit. If unspecified will emit all
                             (unless whitelist).
       --whitelist WHITELIST
                             Modules/FQN to emit. If unspecified will emit all
                             (minus blacklist).
       --output-directory OUTPUT_DIRECTORY, -o OUTPUT_DIRECTORY
                             Where to place the generated exposed interfaces to the
                             given `--module`.
+      --target-module-name TARGET_MODULE_NAME
+                            Target module name. Defaults to `${module}.gold`.
       --dry-run             Show what would be created; don't actually write to
                             the filesystem.
 
 ---
 
 ## License
```

### Comparing `python-cdd-0.0.99rc4/README.md` & `python-cdd-0.0.99rc5/python_cdd.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,43 @@
+Metadata-Version: 2.1
+Name: python-cdd
+Version: 0.0.99rc5
+Summary: Open API to/fro routes, models, and tests. Convert between docstrings, classes, methods, argparse, pydantic, and SQLalchemy.
+Home-page: https://github.com/offscale/cdd-python
+Author: Samuel Marks
+Author-email: 807580+SamuelMarks@users.noreply.github.com
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Compilers
+Classifier: Topic :: Software Development :: Pre-processors
+Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE-APACHE
+License-File: LICENSE-MIT
+
 cdd-python
 ==========
 ![Python version range](https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8%20|%203.9%20|%203.10%20|%203.11-blue.svg)
 ![Python implementation](https://img.shields.io/badge/implementation-cpython-blue.svg)
 [![License](https://img.shields.io/badge/license-Apache--2.0%20OR%20MIT-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Linting, testing, coverage, and release](https://github.com/offscale/cdd-python/workflows/Linting,%20testing,%20coverage,%20and%20release/badge.svg)](https://github.com/offscale/cdd-python/actions)
 ![Tested OSs, others may work](https://img.shields.io/badge/Tested%20on-Linux%20|%20macOS%20|%20Windows-green)
@@ -476,21 +512,20 @@
   inline ([PEP484](https://python.org/dev/peps/pep-0484)–style))
 - Switch between docstring formats (to/from {numpy, ReST, google})
 - Desktop GUI with wxWidgets, from the argparse layer through [Gooey](https://github.com/chriskiehl/Gooey) [one liner]
 
 ## CLI for this project
 
     $ python -m cdd --help
-    
     usage: python -m cdd [-h] [--version]
                          {sync_properties,sync,gen,gen_routes,openapi,doctrans,exmod}
                          ...
     
     Open API to/fro routes, models, and tests. Convert between docstrings,
-    classes, methods, argparse, and SQLalchemy.
+    classes, methods, argparse, pydantic, and SQLalchemy.
     
     positional arguments:
       {sync_properties,sync,gen,gen_routes,openapi,doctrans,exmod}
         sync_properties     Synchronise one or more properties between input and
                             input_str Python files
         sync                Force argparse, classes, and/or methods to be
                             equivalent
@@ -507,43 +542,44 @@
     options:
       -h, --help            show this help message and exit
       --version             show program's version number and exit
 
 ### `sync`
 
     $ python -m cdd sync --help
-
     usage: python -m cdd sync [-h] [--argparse-function ARGPARSE_FUNCTIONS]
                               [--argparse-function-name ARGPARSE_FUNCTION_NAMES]
                               [--class CLASSES] [--class-name CLASS_NAMES]
                               [--function FUNCTIONS]
-                              [--function-name FUNCTION_NAMES] --truth
-                              {argparse_function,class,function}
+                              [--function-name FUNCTION_NAMES] [--no-word-wrap]
+                              --truth
+                              {argparse_function,class,function,sqlalchemy,sqlalchemy_table}
     
     options:
       -h, --help            show this help message and exit
       --argparse-function ARGPARSE_FUNCTIONS
                             File where argparse function is `def`ined.
       --argparse-function-name ARGPARSE_FUNCTION_NAMES
                             Name of argparse function.
       --class CLASSES       File where class `class` is declared.
       --class-name CLASS_NAMES
                             Name of `class`
       --function FUNCTIONS  File where function is `def`ined.
       --function-name FUNCTION_NAMES
                             Name of Function. If method, use Python resolution
                             syntax, i.e., ClassName.function_name
-      --truth {argparse_function,class,function}
+      --no-word-wrap        Whether word-wrap is disabled (on emission). None
+                            enables word-wrap. Defaults to None.
+      --truth {argparse_function,class,function,sqlalchemy,sqlalchemy_table}
                             Single source of truth. Others will be generated from
                             this. Will run with first found choice.
 
 ### `sync_properties`
 
     $ python -m cdd sync_properties --help
-
     usage: python -m cdd sync_properties [-h] --input-filename INPUT_FILENAME
                                          --input-param INPUT_PARAMS [--input-eval]
                                          --output-filename OUTPUT_FILENAME
                                          --output-param OUTPUT_PARAMS
                                          [--output-param-wrap OUTPUT_PARAM_WRAP]
     
     options:
@@ -564,54 +600,59 @@
       --output-param-wrap OUTPUT_PARAM_WRAP
                             Wrap all input_str params with this. E.g.,
                             `Optional[Union[{output_param}, str]]`
 
 ### `gen`
 
     $ python -m cdd gen --help
-
     usage: python -m cdd gen [-h] --name-tpl NAME_TPL --input-mapping
                              INPUT_MAPPING [--prepend PREPEND]
                              [--imports-from-file IMPORTS_FROM_FILE]
-                             [--parse {argparse,class,function,sqlalchemy,sqlalchemy_table}]
+                             [--parse {argparse,class,function,json_schema,pydantic,sqlalchemy,sqlalchemy_table,infer}]
                              --emit
-                             {argparse,class,function,sqlalchemy,sqlalchemy_table}
+                             {argparse,class,function,json_schema,pydantic,sqlalchemy,sqlalchemy_table}
                              --output-filename OUTPUT_FILENAME [--emit-call]
-                             [--decorator DECORATOR_LIST]
+                             [--emit-and-infer-imports] [--no-word-wrap]
+                             [--decorator DECORATOR_LIST] [--phase PHASE]
     
-    optional arguments:
+    options:
       -h, --help            show this help message and exit
       --name-tpl NAME_TPL   Template for the name, e.g., `{name}Config`.
       --input-mapping INPUT_MAPPING
                             Fully-qualified module, filepath, or directory.
       --prepend PREPEND     Prepend file with this. Use '\n' for newlines.
       --imports-from-file IMPORTS_FROM_FILE
                             Extract imports from file and append to `output_file`.
                             If module or other symbol path given, resolve file
                             then use it.
-      --parse {argparse,class,function,sqlalchemy,sqlalchemy_table}
+      --parse {argparse,class,function,json_schema,pydantic,sqlalchemy,sqlalchemy_table,infer}
                             What type the input is.
-      --emit {argparse,class,function,sqlalchemy,sqlalchemy_table}
-                            What type to generate.
+      --emit {argparse,class,function,json_schema,pydantic,sqlalchemy,sqlalchemy_table}
+                            Which type to generate.
       --output-filename OUTPUT_FILENAME, -o OUTPUT_FILENAME
                             Output file to write to.
       --emit-call           Whether to place all the previous body into a new
                             `__call__` internal function
+      --emit-and-infer-imports
+                            Whether to emit and infer imports at the top of the
+                            generated code
+      --no-word-wrap        Whether word-wrap is disabled (on emission). None
+                            enables word-wrap. Defaults to None.
       --decorator DECORATOR_LIST
                             List of decorators.
-
+      --phase PHASE         Which phase to run through. E.g., SQLalchemy may
+                            require multiple phases to resolve foreign keys.
 
 PS: If you're outputting JSON-schema and want a file per schema then:
 
     python -c 'import sys,json,os; f=open(sys.argv[1], "rt"); d=json.load(f); f.close(); [(lambda f: json.dump(sc,f) or f.close())(open(os.path.join(os.path.dirname(sys.argv[1]), sc["$id"].rpartition("/")[2]), "wt")) for sc in d["schemas"]]' <path_to_json_file>
 
 ### `gen_routes`
 
     $ python -m cdd gen_routes --help
-
     usage: python -m cdd gen_routes [-h] --crud {CRUD,CR,C,R,U,D,CR,CU,CD,CRD}
                                     [--app-name APP_NAME] --model-path MODEL_PATH
                                     --model-name MODEL_NAME --routes-path
                                     ROUTES_PATH [--route ROUTE]
     
     options:
       -h, --help            show this help message and exit
@@ -630,74 +671,79 @@
                             'foo/routes'
       --route ROUTE         Name of the route, defaults to
                             `/api/{model_name.lower()}`
 
 ### `openapi`
 
     $ python -m cdd openapi --help
-
     usage: python -m cdd openapi [-h] [--app-name APP_NAME] --model-paths
-                                 MODEL_PATHS --routes-paths
-                                 [ROUTES_PATHS [ROUTES_PATHS ...]]
+                                 MODEL_PATHS --routes-paths [ROUTES_PATHS ...]
     
-    optional arguments:
+    options:
       -h, --help            show this help message and exit
       --app-name APP_NAME   Name of app (e.g., `app_name = Bottle();
                             @app_name.get('/api') def slash(): pass`)
       --model-paths MODEL_PATHS
                             Python module resolution (foo.models) or filepath
                             (foo/models)
-      --routes-paths [ROUTES_PATHS [ROUTES_PATHS ...]]
+      --routes-paths [ROUTES_PATHS ...]
                             Python module resolution 'foo.routes' or filepath
                             'foo/routes'
 
 ### `doctrans`
 
     $ python -m cdd doctrans --help
-    
     usage: python -m cdd doctrans [-h] --filename FILENAME --format
                                   {rest,google,numpydoc}
-                                  (--type-annotations | --no-type-annotations)
+                                  (--type-annotations | --no-type-annotations | --no-word-wrap)
     
     options:
       -h, --help            show this help message and exit
       --filename FILENAME   Python file to convert docstrings within. Edited in
                             place.
       --format {rest,google,numpydoc}
                             The docstring format to replace existing format with.
       --type-annotations    Inline the type, i.e., annotate PEP484 (outside
                             docstring. Requires 3.6+)
       --no-type-annotations
                             Ensure all types are in docstring (rather than a
                             PEP484 type annotation)
+      --no-word-wrap        Whether word-wrap is disabled (on emission). None
+                            enables word-wrap. Defaults to None.
 
 ### `exmod`
 
     $ python -m cdd exmod --help
-    
     usage: python -m cdd exmod [-h] --module MODULE --emit
-                               {argparse,class,function,sqlalchemy,sqlalchemy_table}
-                               [--blacklist BLACKLIST] [--whitelist WHITELIST]
-                               --output-directory OUTPUT_DIRECTORY [--dry-run]
+                               {argparse,class,function,json_schema,pydantic,sqlalchemy,sqlalchemy_table}
+                               [--no-word-wrap] [--blacklist BLACKLIST]
+                               [--whitelist WHITELIST] --output-directory
+                               OUTPUT_DIRECTORY
+                               [--target-module-name TARGET_MODULE_NAME]
+                               [--dry-run]
     
     options:
       -h, --help            show this help message and exit
       --module MODULE, -m MODULE
                             The module or fully-qualified name (FQN) to expose.
-      --emit {argparse,class,function,sqlalchemy,sqlalchemy_table}
-                            What type to generate.
+      --emit {argparse,class,function,json_schema,pydantic,sqlalchemy,sqlalchemy_table}
+                            Which type to generate.
+      --no-word-wrap        Whether word-wrap is disabled (on emission). None
+                            enables word-wrap. Defaults to None.
       --blacklist BLACKLIST
                             Modules/FQN to omit. If unspecified will emit all
                             (unless whitelist).
       --whitelist WHITELIST
                             Modules/FQN to emit. If unspecified will emit all
                             (minus blacklist).
       --output-directory OUTPUT_DIRECTORY, -o OUTPUT_DIRECTORY
                             Where to place the generated exposed interfaces to the
                             given `--module`.
+      --target-module-name TARGET_MODULE_NAME
+                            Target module name. Defaults to `${module}.gold`.
       --dry-run             Show what would be created; don't actually write to
                             the filesystem.
 
 ---
 
 ## License
```

### Comparing `python-cdd-0.0.99rc4/cdd/__main__.py` & `python-cdd-0.0.99rc5/cdd/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -416,14 +416,21 @@
     exmod_parser.add_argument(
         "--output-directory",
         "-o",
         help="Where to place the generated exposed interfaces to the given `--module`.",
         required=True,
     )
     exmod_parser.add_argument(
+        "--target-module-name",
+        help="Target module name. Defaults to `${module}.gold`.",
+        required=False,
+        default=None,
+    )
+
+    exmod_parser.add_argument(
         "--dry-run",
         help="Show what would be created; don't actually write to the filesystem.",
         action="store_true",
     )
 
     return parser
```

### Comparing `python-cdd-0.0.99rc4/cdd/argparse_function/emit.py` & `python-cdd-0.0.99rc5/cdd/argparse_function/emit.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/argparse_function/parse.py` & `python-cdd-0.0.99rc5/cdd/argparse_function/parse.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/argparse_function/utils/emit_utils.py` & `python-cdd-0.0.99rc5/cdd/argparse_function/utils/emit_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/class_/emit.py` & `python-cdd-0.0.99rc5/cdd/class_/emit.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/class_/parse.py` & `python-cdd-0.0.99rc5/cdd/class_/parse.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/class_/utils/emit_utils.py` & `python-cdd-0.0.99rc5/cdd/class_/utils/emit_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/class_/utils/parse_utils.py` & `python-cdd-0.0.99rc5/cdd/class_/utils/parse_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/compound/doctrans.py` & `python-cdd-0.0.99rc5/cdd/compound/doctrans.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/compound/doctrans_utils.py` & `python-cdd-0.0.99rc5/cdd/compound/doctrans_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/compound/gen.py` & `python-cdd-0.0.99rc5/cdd/compound/gen.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/compound/gen_utils.py` & `python-cdd-0.0.99rc5/cdd/compound/gen_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     optimise_imports,
     set_value,
 )
 from cdd.shared.emit.utils.emitter_utils import get_emitter
 from cdd.shared.parse import kind2instance_type
 from cdd.shared.parse.utils.parser_utils import get_parser
 from cdd.shared.pure_utils import (
+    ensure_valid_identifier,
     find_module_filepath,
     pascal_to_upper_camelcase,
     rpartial,
 )
 from cdd.shared.source_transformer import ast_parse, to_code
 
 
@@ -103,15 +104,15 @@
             },
             "json_schema": {
                 "identifier": _name,
             },
             "sqlalchemy": {"table_name": _name},
             "sqlalchemy_table": {"table_name": _name},
         }[emit_name]
-    )(None if name == "infer" else name_tpl.format(name=name))
+    )(None if name == "infer" else ensure_valid_identifier(name_tpl.format(name=name)))
 
 
 def gen_file(
     name_tpl,
     input_mapping_it,
     parse_name,
     emit_name,
@@ -398,15 +399,15 @@
     :rtype: ```Tuple[AST]```
     """
     emitter = get_emitter(emit_name)
     return tuple(
         print("\nGenerating: {name!r}".format(name=name))
         or global__all__.append(name_tpl.format(name=name))
         or emitter(
-            print("obj:", obj, ";") or get_parser(obj, parse_name)(obj),
+            get_parser(obj, parse_name)(obj),
             emit_default_doc=emit_default_doc,
             word_wrap=no_word_wrap is None,
             **get_emit_kwarg(decorator_list, emit_call, emit_name, name_tpl, name),
         )
         for name, obj in input_mapping_it
     )
```

### Comparing `python-cdd-0.0.99rc4/cdd/compound/openapi/emit.py` & `python-cdd-0.0.99rc5/cdd/compound/openapi/emit.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/compound/openapi/gen_openapi.py` & `python-cdd-0.0.99rc5/cdd/compound/openapi/gen_openapi.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/compound/openapi/gen_routes.py` & `python-cdd-0.0.99rc5/cdd/compound/openapi/gen_routes.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/compound/openapi/parse.py` & `python-cdd-0.0.99rc5/cdd/compound/openapi/parse.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/compound/openapi/utils/emit_openapi_utils.py` & `python-cdd-0.0.99rc5/cdd/compound/openapi/utils/emit_openapi_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/compound/openapi/utils/emit_utils.py` & `python-cdd-0.0.99rc5/cdd/compound/openapi/utils/emit_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,21 @@
 from itertools import chain, filterfalse
 from json import dumps
 from operator import attrgetter, eq, methodcaller
 from os import path
 from platform import system
 
 import cdd.sqlalchemy.utils.shared_utils
-from cdd.shared.ast_utils import get_value, maybe_type_comment, set_arg, set_value
+from cdd.shared.ast_utils import (
+    NoneStr,
+    get_value,
+    maybe_type_comment,
+    set_arg,
+    set_value,
+)
 from cdd.shared.pure_utils import (
     find_module_filepath,
     namespaced_upper_camelcase_to_pascal,
     none_types,
     rpartial,
     tab,
 )
@@ -114,29 +120,31 @@
             ast.keyword(
                 arg=k, value=v if isinstance(v, AST) else set_value(v), identifier=None
             )
             for k, v in _param["x_typ"]["sql"]["constraints"].items()
         ]
 
     # TODO: Maybe `CREATE TYPE` and use that?
-    if _param["typ"] == "dict" and "ir" in _param:
+    if _param.get("typ") == "dict" and "ir" in _param:
         keywords.append(
             ast.keyword(
                 arg="comment",
                 value=set_value("[schema={}]".format(dumps(_param["ir"]))),
                 identifier=None,
             )
         )
 
     if has_default:
         # if default == NoneStr: default = None
         keywords.append(
             ast.keyword(
                 arg="default",
-                value=default if isinstance(default, AST) else set_value(default),
+                value=default
+                if isinstance(default, AST)
+                else set_value(None if default == NoneStr else default),
                 identifier=None,
             )
         )
 
     if isinstance(nullable, bool):
         keywords.append(
             ast.keyword(arg="nullable", value=set_value(nullable), identifier=None)
```

### Comparing `python-cdd-0.0.99rc4/cdd/compound/openapi/utils/parse_utils.py` & `python-cdd-0.0.99rc5/cdd/compound/openapi/utils/parse_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/compound/sync_properties.py` & `python-cdd-0.0.99rc5/cdd/compound/sync_properties.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/docstring/emit.py` & `python-cdd-0.0.99rc5/cdd/docstring/emit.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/docstring/parse.py` & `python-cdd-0.0.99rc5/cdd/docstring/parse.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/docstring/utils/emit_utils.py` & `python-cdd-0.0.99rc5/cdd/docstring/utils/emit_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/function/emit.py` & `python-cdd-0.0.99rc5/cdd/function/emit.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/function/parse.py` & `python-cdd-0.0.99rc5/cdd/function/parse.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/function/utils/emit_utils.py` & `python-cdd-0.0.99rc5/cdd/function/utils/emit_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/function/utils/parse_utils.py` & `python-cdd-0.0.99rc5/cdd/function/utils/parse_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/json_schema/emit.py` & `python-cdd-0.0.99rc5/cdd/json_schema/emit.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/json_schema/parse.py` & `python-cdd-0.0.99rc5/cdd/json_schema/parse.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/json_schema/utils/emit_utils.py` & `python-cdd-0.0.99rc5/cdd/json_schema/utils/emit_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/json_schema/utils/parse_utils.py` & `python-cdd-0.0.99rc5/cdd/json_schema/utils/parse_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/routes/emit/bottle.py` & `python-cdd-0.0.99rc5/cdd/routes/emit/bottle.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/routes/emit/bottle_constants_utils.py` & `python-cdd-0.0.99rc5/cdd/routes/emit/bottle_constants_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/routes/parse/bottle.py` & `python-cdd-0.0.99rc5/cdd/routes/parse/bottle.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/routes/parse/bottle_utils.py` & `python-cdd-0.0.99rc5/cdd/routes/parse/bottle_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/routes/parse/fastapi.py` & `python-cdd-0.0.99rc5/cdd/routes/parse/fastapi.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/routes/parse/fastapi_utils.py` & `python-cdd-0.0.99rc5/cdd/routes/parse/fastapi_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/shared/ast_cst_utils.py` & `python-cdd-0.0.99rc5/cdd/shared/ast_cst_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/shared/ast_utils.py` & `python-cdd-0.0.99rc5/cdd/shared/ast_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,22 +34,23 @@
     Tuple,
     UnaryOp,
     alias,
     iter_child_nodes,
     keyword,
     walk,
 )
+from collections import namedtuple
 from contextlib import suppress
 from copy import deepcopy
 from functools import partial
 from importlib import import_module
 from inspect import isclass, isfunction
 from itertools import chain, filterfalse, groupby
 from json import dumps
-from operator import attrgetter, contains, inv, itemgetter, neg, not_, pos
+from operator import attrgetter, contains, inv, neg, not_, pos
 
 from yaml import safe_dump_all
 
 from cdd.shared.defaults_utils import extract_default, needs_quoting
 from cdd.shared.pure_utils import (
     PY_GTE_3_8,
     PY_GTE_3_9,
@@ -837,30 +838,41 @@
             ):
                 return child_node
             elif hasattr(child_node, "name") and child_node.name == query:
                 cursor = child_node.body
                 break
 
 
-def annotate_ancestry(node):
+def annotate_ancestry(node, filename=None):
     """
     Look to your roots. Find the child; find the parent.
-    Sets _location attribute to every child node.
+    Sets _location and __file__ attributes to every child node.
 
     :param node: AST node. Will be annotated in-place.
     :type node: ```AST```
 
+    :param filename: Where the node was originally defined. Sets the `__file__` attribute to this.
+    :type filename: ```Optional[str]```
+
     :return: Annotated AST node; also `node` arg will be annotated in-place.
     :rtype: ```AST```
     """
     # print("annotating", getattr(node, "name", None))
     node._location = [node.name] if hasattr(node, "name") else []
+    if filename not in (None, "<unknown>") and isinstance(
+        node, (AnnAssign, Assign, AsyncFunctionDef, ClassDef, FunctionDef, Module)
+    ):
+        setattr(node, "__file__", filename)
     parent_location = []
     for _node in walk(node):
         name = [_node.name] if hasattr(_node, "name") else []
+        if filename not in (None, "<unknown>") and isinstance(
+            _node, (AnnAssign, Assign, AsyncFunctionDef, ClassDef, FunctionDef, Module)
+        ):
+            setattr(_node, "__file__", filename)
         for child_node in iter_child_nodes(_node):
             if hasattr(child_node, "name") and not isinstance(child_node, alias):
                 child_node._location = name + [child_node.name]
                 parent_location = child_node._location
             elif isinstance(child_node, (Constant, Str)):
                 child_node._location = parent_location + [get_value(child_node)]
             elif isinstance(child_node, Assign) and all(
@@ -1079,14 +1091,37 @@
         and isinstance(node.targets[0], Name)
     ):
         return set_arg(node.targets[0].id)
     else:
         raise NotImplementedError(type(node).__name__)
 
 
+def construct_module_with_symbols(module, symbols):
+    """
+    Create a module out of the input module that only contains nodes
+    with a name contained in `symbols`
+
+    :param module: Input module
+    :type module: ```Module```
+
+    :param symbols: Symbols
+    :type symbols: ```FrozenSet[str]```
+
+    :return: Module with only members whose `.name` is in `symbols`
+    :rtype: ```Module```
+    """
+    return Module(
+        body=list(
+            filter(lambda node: getattr(node, "name", "") in symbols, module.body)
+        ),
+        type_ignores=[],
+        stmt=None,
+    )
+
+
 def it2literal(it):
     """
     Convert a collection of constants into a type annotation
 
     :param it: collection of constants
     :type it: ```Union[Tuple[Union[str, int, float], ...], List[Union[str, int, float], ...]]```
 
@@ -1592,27 +1627,30 @@
             expr=None,
             lineno=None,
             **maybe_type_comment,
         )
     )
 
 
-def merge_modules(mod0, mod1, remove_imports_from_second=True):
+def merge_modules(mod0, mod1, remove_imports_from_second=True, deduplicate_names=False):
     """
     Merge modules (removing module docstring from mod1)
 
     :param mod0: Module
     :type mod0: ```Module```
 
     :param mod1: Module
     :type mod1: ```Module```
 
     :param remove_imports_from_second: Whether to remove global imports from second module
     :type remove_imports_from_second: ```bool```
 
+    :param deduplicate_names: Whether to deduplicate names; names can be function|class|AnnAssign|Assign name
+    :type deduplicate_names: ```bool```
+
     :return: Merged module (copy)
     :rtype: ```Module```
     """
     mod1_body = (
         mod1.body[1:]
         if mod1.body and isinstance(get_value(mod1.body[0]), (Str, Constant))
         else mod1.body
@@ -1626,14 +1664,54 @@
                 rpartial(isinstance, (ImportFrom, Import)),
                 mod1_body,
             )
         )
         if remove_imports_from_second
         else deepcopy(mod1_body)
     )
+    if deduplicate_names:
+
+        def unique_nodes(node):
+            """
+            :param node: AST node
+            :type node: ```AST```
+
+            :return: node if name is in `seen` set else None; with side-effect of adding to `seen`
+            :rtype: ```bool```
+            """
+
+            def side_effect_ret(name):
+                """
+                :param name: Name
+                :type name: ```str```
+
+                :return: node if name is in `seen` set else None; with side-effect of adding to `seen`
+                :rtype: ```bool```
+                """
+                if name in seen:
+                    return None
+                else:
+                    seen.add(node.name)
+                    return node
+
+            if isinstance(node, (FunctionDef, AsyncFunctionDef, ClassDef)):
+                return side_effect_ret(node.name)
+            elif isinstance(node, AnnAssign):
+                return side_effect_ret(get_value(node.target))
+            elif isinstance(node, Assign):
+                return any(
+                    filter(
+                        lambda target: side_effect_ret(get_value(target)), node.targets
+                    )
+                )
+            else:
+                return node
+
+        seen = set()
+        new_mod.body = list(filter(None, map(unique_nodes, new_mod.body)))
 
     return new_mod
 
 
 def optimise_imports(imports):
     """
     Optimise imports involves:
@@ -1649,37 +1727,76 @@
 
     :return: `ImportFrom` nodes
     :rtype: ```List[ImportFrom]```
     """
     seen_pair = set()
     return [
         ImportFrom(
-            module=module,
-            names=list(
-                map(
-                    itemgetter(1),
-                    filter(
-                        lambda key_alias: key_alias[0] not in seen_pair
-                        and (seen_pair.add(key_alias[0]) or True),
-                        map(
-                            lambda _alias: (
-                                _alias.name + (getattr(_alias, "asname", None) or ""),
-                                _alias,
-                            ),
-                            chain.from_iterable(map(attrgetter("names"), symbols)),
+            module=module_name,
+            level=sym[0].level,
+            names=list(map(lambda al: alias(name=al.name, asname=al.asname), sym[1])),
+        )
+        for module_name, symbols in map(
+            lambda key_group: (
+                key_group[0],
+                filter(
+                    None,
+                    map(
+                        lambda node: (
+                            lambda filtered: (
+                                namedtuple("_", ("level",))(node.level),
+                                filtered,
+                            )
+                            if filtered
+                            else None
+                        )(
+                            tuple(
+                                filter(
+                                    None,
+                                    map(
+                                        lambda name_asname_key: None
+                                        if name_asname_key.key in seen_pair
+                                        else (
+                                            seen_pair.add(name_asname_key.key)
+                                            or namedtuple("_", ("name", "asname"))(
+                                                name_asname_key.name,
+                                                name_asname_key.asname,
+                                            )
+                                        ),
+                                        map(
+                                            lambda _alias: namedtuple(
+                                                "_", ("name", "asname", "key")
+                                            )(
+                                                _alias.name,
+                                                _alias.asname,
+                                                "{}{}{}".format(
+                                                    key_group[0],
+                                                    _alias.name,
+                                                    _alias.asname,
+                                                ),
+                                            ),
+                                            node.names,
+                                        ),
+                                    ),
+                                )
+                            )
                         ),
+                        key_group[1],
                     ),
-                )
+                ),
+            ),
+            groupby(
+                sorted(
+                    imports,
+                    key=attrgetter("module"),
+                ),
+                key=attrgetter("module"),
             ),
-            level=1,
-            identifier=None,
-        )
-        for module, symbols in groupby(
-            sorted(imports, key=attrgetter("module")), attrgetter("module")
         )
+        for sym in symbols
     ]
 
 
 def infer_imports(module):
     """
     Infer imports
 
@@ -1734,14 +1851,15 @@
     "RewriteAtQuery",
     "Set_to_set",
     "Tuple_to_tuple",
     "annotate_ancestry",
     "ast_type_to_python_type",
     "cmp_ast",
     "code_quoted",
+    "construct_module_with_symbols",
     "emit_ann_assign",
     "emit_arg",
     "find_ast_type",
     "find_in_ast",
     "func_arg2param",
     "get_at_root",
     "get_doc_str",
```

### Comparing `python-cdd-0.0.99rc4/cdd/shared/conformance.py` & `python-cdd-0.0.99rc5/cdd/shared/conformance.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/shared/cst.py` & `python-cdd-0.0.99rc5/cdd/shared/cst.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/shared/cst_utils.py` & `python-cdd-0.0.99rc5/cdd/shared/cst_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/shared/defaults_utils.py` & `python-cdd-0.0.99rc5/cdd/shared/defaults_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/shared/docstring_parsers.py` & `python-cdd-0.0.99rc5/cdd/shared/docstring_parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -995,8 +995,8 @@
     return (
         ("typ", (lambda v: "dict" if v.startswith("**") else v)(val.replace("```", "")))
         if input_str.startswith(sw)
         else ("doc", val)
     )
 
 
-__all__ = ["parse_docstring", "Style"]
+__all__ = ["parse_docstring", "_set_name_and_type", "Style"]
```

### Comparing `python-cdd-0.0.99rc4/cdd/shared/docstring_utils.py` & `python-cdd-0.0.99rc5/cdd/shared/docstring_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/shared/emit/__init__.py` & `python-cdd-0.0.99rc5/cdd/shared/emit/__init__.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/shared/emit/file.py` & `python-cdd-0.0.99rc5/cdd/shared/emit/file.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/shared/emit/utils/emitter_utils.py` & `python-cdd-0.0.99rc5/cdd/shared/emit/utils/emitter_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/shared/parse/__init__.py` & `python-cdd-0.0.99rc5/cdd/shared/parse/__init__.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/shared/parse/utils/parser_utils.py` & `python-cdd-0.0.99rc5/cdd/shared/parse/utils/parser_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/shared/pkg_utils.py` & `python-cdd-0.0.99rc5/cdd/shared/pkg_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     :param remove_hints: Hints as to what can be removed
     :type remove_hints: ```Tuple[str]```
 
     :return: Relative path (if derived) else original
     :rtype: ```str```
     """
     _filename = filename.casefold()
-    for elem in remove_hints + (get_python_lib(), get_python_lib(prefix="")):
+    lib = get_python_lib(), get_python_lib(prefix="")
+    for elem in remove_hints + lib:
         if _filename.startswith(elem.casefold()):
             return filename[len(elem) + 1 :]
     return filename
 
 
 __all__ = ["relative_filename"]
```

### Comparing `python-cdd-0.0.99rc4/cdd/shared/pure_utils.py` & `python-cdd-0.0.99rc5/cdd/shared/pure_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,34 +11,52 @@
 from inspect import getmodule
 from itertools import chain, count, filterfalse, islice, takewhile, zip_longest
 from json import JSONEncoder
 from keyword import iskeyword
 from operator import attrgetter, eq, itemgetter
 from os import environ, extsep, listdir, path
 from pprint import PrettyPrinter
-from sys import version_info
+from sys import stderr, version_info
 from textwrap import fill as _fill
 from textwrap import indent
+from types import BuiltinFunctionType
 from typing import Callable, Dict, FrozenSet, Optional, Tuple, Union
 
-pp: Callable[[object], None] = PrettyPrinter(indent=4, width=100).pprint
+pp: Callable[[object], None] = PrettyPrinter(indent=4, width=100, stream=stderr).pprint
 tab: str = environ.get("DOCTRANS_TAB", " " * 4)
 simple_types: Dict[Optional[str], Union[int, float, complex, str, bool, None]] = {
     "int": 0,
     "float": 0.0,
     "complex": 0j,
     "str": "",
     "bool": False,
     None: None,
 }
 
 line_length = environ.get("DOCTRANS_LINE_LENGTH", 100)
 fill = partial(_fill, width=line_length)
 
 
+def read_file_to_str(filename, mode="rt"):
+    """
+    Read filename into a str, closing the file afterwards
+
+    :param filename: Input filename
+    :type filename: ```str```
+
+    :param mode: File mode
+    :type mode: ```str```
+
+    :return: Filename content as str
+    :rtype: ```str```
+    """
+    with open(filename, mode) as f:
+        return f.read()
+
+
 # From https://github.com/Suor/funcy/blob/0ee7ae8/funcy/funcs.py#L34-L36
 def rpartial(func, *args):
     """Partially applies last arguments."""
     return lambda *a: func(*(a + args))
 
 
 def remove_whitespace_comments(source):
@@ -830,31 +848,37 @@
                     (attrgetter(rest_path) if rest_path else identity)(
                         extra_symbols[pkg]
                     )
                 )
             raise
 
 
-def find_module_filepath(module_name, submodule_name):
+def find_module_filepath(module_name, submodule_name, none_when_no_spec=False):
     """
     Find module's file location without first importing it
 
     :param module_name: Module name, e.g., "cdd.tests"
     :type: ```str```
 
     :param submodule_name: Submodule name, e.g., "test_pure_utils"
     :type: ```str```
 
+    :param none_when_no_spec: When `find_spec` returns `None` return that. If `False` raises `AssertionError` then.
+    :type none_when_no_spec: ```bool```
+
     :return: Module location
     :rpath: ```str```
     """
     assert module_name is not None
     assert submodule_name is not None
     module_spec = find_spec(module_name)
-    assert module_spec is not None, "spec not found for {}".format(module_name)
+    if module_spec is None:
+        if none_when_no_spec:
+            return module_spec
+        raise AssertionError("spec not found for {}".format(module_name))
     module_origin = module_spec.origin
     module_parent = path.dirname(module_origin)
 
     return next(
         filter(
             path.exists,
             (
@@ -1014,14 +1038,34 @@
         run_per_line(
             "\n".join(map(lambda line: sep if len(line) == 0 else line, s.splitlines()))
         ),
         sep=sep,
     )
 
 
+def ensure_valid_identifier(s):
+    """
+    Ensure identifier is valid
+
+    :param s: Potentially valid identifier
+    :type s: ```str```
+
+    :return: Valid identifier from `s`
+    :rtype: ```str```
+    """
+    if not s:
+        return "_"
+    elif iskeyword(s):
+        return "{}_".format(s)
+    elif s[0].isdigit():
+        s = "_{}".format(s)
+    valid = frozenset("_ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz")
+    return "".join(filter(valid.__contains__, s))
+
+
 def set_attr(obj, key, val):
     """
     Sets the named attribute on the given object to the specified value.
 
     set_attr(x, 'y', v) is equivalent to ``x.y = v; return x''
 
     :param obj: An object
@@ -1072,30 +1116,32 @@
         Handle `set` by giving a sorted list in its place
         """
         return (sorted if isinstance(obj, set) else partial(JSONEncoder.default, self))(
             obj
         )
 
 
-def no_magic_dir2attr(p_object):
+def no_magic_or_builtin_dir2attr(p_object):
     """
     Dictionary of `dir` without the __ prefix magics (also without _ prefix)
+    and without builtins
     return the names comprising (some of) the attributes
     of the given object, and of attributes reachable from it.
 
     :param p_object: Object
     :type p_object: ```Any```
 
     :return: Dict of name to attribute value
     :rtype: ```dict```
     """
     return {
         attr: getattr(p_object, attr)
         for attr in dir(p_object)
         if not attr.startswith("_")
+        and not isinstance(getattr(p_object, attr), BuiltinFunctionType)
     }
 
 
 def pascal_to_upper_camelcase(s):
     """
     Transform pascal input to upper camelcase
 
@@ -1188,14 +1234,15 @@
     "ENCODING",
     "INIT_FILENAME",
     "PY3_8",
     "PY_GTE_3_8",
     "PY_GTE_3_9",
     "SetEncoder",
     "all_dunder_for_module",
+    "append_to_dict",
     "assert_equal",
     "balanced_parentheses",
     "blockwise",
     "code_quoted",
     "count_chars_from",
     "count_iter_items",
     "deindent",
@@ -1210,27 +1257,27 @@
     "is_ir_empty",
     "is_triple_quoted",
     "location_within",
     "lstrip_namespace",
     "multiline",
     "namespaced_pascal_to_upper_camelcase",
     "namespaced_upper_camelcase_to_pascal",
-    "no_magic_dir2attr",
+    "no_magic_or_builtin_dir2attr",
     "none_types",
     "num_of_nls",
     "omit_whitespace",
     "paren_wrap_code",
     "parse_comment_from_line",
     "pascal_to_upper_camelcase",
     "pluralise",
     "pp",
     "quote",
+    "read_file_to_str",
     "reindent",
     "remove_whitespace_comments",
-    "append_to_dict",
     "rpartial",
     "sanitise",
     "sanitise_emit_name",
     "set_attr",
     "set_item",
     "simple_types",
     "strip_split",
```

### Comparing `python-cdd-0.0.99rc4/cdd/shared/source_transformer.py` & `python-cdd-0.0.99rc5/cdd/shared/source_transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,16 @@
     :type skip_docstring_remit: ```bool```
 
     :return: AST node
     :rtype: node: ```AST```
     """
     parsed_ast = parse(source, filename=filename, mode=mode)
     if not skip_annotate:
-        annotate_ancestry(parsed_ast)
+        annotate_ancestry(parsed_ast, filename=filename)
+        setattr(parsed_ast, "__file__", filename)
     if not skip_docstring_remit and isinstance(
         parsed_ast, (Module, ClassDef, FunctionDef, AsyncFunctionDef)
     ):
         docstring = get_docstring(parsed_ast, clean=True)
         if docstring is None:
             return parsed_ast
```

### Comparing `python-cdd-0.0.99rc4/cdd/sqlalchemy/emit.py` & `python-cdd-0.0.99rc5/cdd/sqlalchemy/emit.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,20 @@
 from itertools import chain
 from operator import add
 from os import environ
 
 import cdd.compound.openapi.utils.emit_utils
 from cdd.docstring.emit import docstring
 from cdd.shared.ast_utils import maybe_type_comment, set_value
-from cdd.shared.pure_utils import deindent, indent_all_but_first, tab
+from cdd.shared.pure_utils import (
+    deindent,
+    ensure_valid_identifier,
+    indent_all_but_first,
+    tab,
+)
 
 FORCE_PK_ID = environ.get("FORCE_PK_ID", False) not in (False, 0, "0", "false")
 
 
 def sqlalchemy_table(
     intermediate_repr,
     name="config_tbl",
@@ -68,17 +73,19 @@
 
     :return: AST of the Table expression + assignment
     :rtype: ```ClassDef```
     """
     return Assign(
         targets=[
             Name(
-                name
-                if name not in (None, "config_tbl") or not intermediate_repr["name"]
-                else intermediate_repr["name"],
+                ensure_valid_identifier(
+                    name
+                    if name not in (None, "config_tbl") or not intermediate_repr["name"]
+                    else intermediate_repr["name"]
+                ),
                 Store(),
             )
         ],
         value=Call(
             func=Name("Table", Load()),
             args=list(
                 chain.from_iterable(
```

### Comparing `python-cdd-0.0.99rc4/cdd/sqlalchemy/parse.py` & `python-cdd-0.0.99rc5/cdd/sqlalchemy/parse.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/sqlalchemy/utils/parse_utils.py` & `python-cdd-0.0.99rc5/cdd/sqlalchemy/utils/parse_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/sqlalchemy/utils/shared_utils.py` & `python-cdd-0.0.99rc5/cdd/sqlalchemy/utils/shared_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 import ast
 from ast import Call, Expr, Load, Name, Subscript, Tuple, keyword
 from operator import attrgetter
 
 import cdd.compound.openapi.utils.emit_utils
-from cdd.shared.ast_utils import get_value, set_value
+from cdd.shared.ast_utils import NoneStr, get_value, set_value
 from cdd.shared.pure_utils import PY_GTE_3_9, rpartial
 from cdd.shared.source_transformer import to_code
 
 
 def update_args_infer_typ_sqlalchemy(_param, args, name, nullable, x_typ_sql):
     """
     :param _param: Param with typ
@@ -27,14 +27,16 @@
     :type nullable: ```Optional[bool]```
 
     :param x_typ_sql:
     :type x_typ_sql: ```dict```
 
     :rtype: ```bool```
     """
+    if _param["typ"] is None:
+        return _param.get("default") == NoneStr
     if _param["typ"].startswith("Optional["):
         _param["typ"] = _param["typ"][len("Optional[") : -1]
         nullable = True
     if "Literal[" in _param["typ"]:
         parsed_typ = get_value(ast.parse(_param["typ"]).body[0])
         assert (
             parsed_typ.value.id == "Literal"
```

### Comparing `python-cdd-0.0.99rc4/cdd/tests/mocks/__init__.py` & `python-cdd-0.0.99rc5/cdd/tests/mocks/__init__.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/mocks/argparse.py` & `python-cdd-0.0.99rc5/cdd/tests/mocks/argparse.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/mocks/classes.py` & `python-cdd-0.0.99rc5/cdd/tests/mocks/classes.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/mocks/cst.py` & `python-cdd-0.0.99rc5/cdd/tests/mocks/cst.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/mocks/cstify.py` & `python-cdd-0.0.99rc5/cdd/tests/mocks/cstify.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/mocks/docstrings.py` & `python-cdd-0.0.99rc5/cdd/tests/mocks/docstrings.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/mocks/doctrans.py` & `python-cdd-0.0.99rc5/cdd/tests/mocks/doctrans.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/mocks/exmod.py` & `python-cdd-0.0.99rc5/cdd/tests/mocks/exmod.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from operator import attrgetter
 from os import path
 from os.path import extsep
 
 from setuptools import find_packages, setup
 
 package_name = {package_name!r}
+module_name = {module_name!r}
 
 
 def main():
     """Main function for setup.py; this actually does the installation"""
     with open(
         path.join(
             path.abspath(path.dirname(__file__)),
```

### Comparing `python-cdd-0.0.99rc4/cdd/tests/mocks/fastapi_routes.py` & `python-cdd-0.0.99rc5/cdd/tests/mocks/fastapi_routes.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/mocks/gen.py` & `python-cdd-0.0.99rc5/cdd/tests/mocks/gen.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/mocks/ir.py` & `python-cdd-0.0.99rc5/cdd/tests/mocks/ir.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/mocks/json_schema.py` & `python-cdd-0.0.99rc5/cdd/tests/mocks/json_schema.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/mocks/methods.py` & `python-cdd-0.0.99rc5/cdd/tests/mocks/methods.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/mocks/openapi.py` & `python-cdd-0.0.99rc5/cdd/tests/mocks/openapi.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/mocks/pydantic.py` & `python-cdd-0.0.99rc5/cdd/tests/mocks/pydantic.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/mocks/routes.py` & `python-cdd-0.0.99rc5/cdd/tests/mocks/routes.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/mocks/sqlalchemy.py` & `python-cdd-0.0.99rc5/cdd/tests/mocks/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_argparse_function/test_emit_argparse.py` & `python-cdd-0.0.99rc5/cdd/tests/test_argparse_function/test_emit_argparse.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_argparse_function/test_parse_argparse.py` & `python-cdd-0.0.99rc5/cdd/tests/test_argparse_function/test_parse_argparse.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_ast_equality.py` & `python-cdd-0.0.99rc5/cdd/tests/test_ast_equality.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_class/test_emit_class_.py` & `python-cdd-0.0.99rc5/cdd/tests/test_class/test_emit_class_.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_class/test_parse_class.py` & `python-cdd-0.0.99rc5/cdd/tests/test_class/test_parse_class.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_cli/test_cli.py` & `python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_cli/test_cli_doctrans.py` & `python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli_doctrans.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_cli/test_cli_exmod.py` & `python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli_exmod.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_cli/test_cli_gen.py` & `python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli_gen.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_cli/test_cli_gen_routes.py` & `python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli_gen_routes.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_cli/test_cli_openapi.py` & `python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli_openapi.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_cli/test_cli_sync.py` & `python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli_sync.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_cli/test_cli_sync_properties.py` & `python-cdd-0.0.99rc5/cdd/tests/test_cli/test_cli_sync_properties.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_compound/test_doctrans.py` & `python-cdd-0.0.99rc5/cdd/tests/test_compound/test_doctrans.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_compound/test_doctrans_utils.py` & `python-cdd-0.0.99rc5/cdd/tests/test_compound/test_doctrans_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_compound/test_exmod.py` & `python-cdd-0.0.99rc5/cdd/tests/test_compound/test_exmod.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,225 +1,183 @@
 """ Tests for exmod subcommand """
 
-from ast import ClassDef
+from ast import Assign, ClassDef, ImportFrom, List, Load, Module, Name, Store, alias
 from functools import partial
 from io import StringIO
 from itertools import chain, groupby
-from operator import add, itemgetter
+from operator import itemgetter
 from os import environ, listdir, mkdir, path, walk
 from os.path import extsep
-from subprocess import DEVNULL, call
+from subprocess import run
 from sys import executable, platform
 from tempfile import TemporaryDirectory
 from unittest import TestCase
 from unittest.mock import patch
 
 import cdd.class_.parse
 from cdd.compound.exmod import exmod
+from cdd.shared.ast_utils import maybe_type_comment, set_value
 from cdd.shared.pkg_utils import relative_filename
 from cdd.shared.pure_utils import ENCODING, INIT_FILENAME, rpartial, unquote
-from cdd.shared.source_transformer import ast_parse
+from cdd.shared.source_transformer import ast_parse, to_code
 from cdd.tests.mocks import imports_header
 from cdd.tests.mocks.classes import class_str
 from cdd.tests.mocks.exmod import setup_py_mock
 from cdd.tests.utils_for_tests import unittest_main
 
 
 class TestExMod(TestCase):
     """Test class for exmod.py"""
 
+    parent_name = ""
+    parent_dir = ""
+    child_name = ""
+    child_dir = ""
+    grandchild_name = ""
+    grandchild_dir = ""
+    module_hierarchy = ()
+
+    @classmethod
+    def setUpClass(cls) -> None:
+        """
+        Create module hierarchy
+        """
+        cls.parent_name, cls.parent_dir = "parent", "parent_dir"
+        cls.child_name, cls.child_dir = "child", path.join(cls.parent_dir, "child_dir")
+        cls.grandchild_name, cls.grandchild_dir = "grandchild", path.join(
+            cls.child_dir, "grandchild_dir"
+        )
+        cls.module_hierarchy = (
+            (cls.parent_name, cls.parent_dir),
+            (cls.child_name, cls.child_dir),
+            (cls.grandchild_name, cls.grandchild_dir),
+        )
+
     def test_exmod(self) -> None:
         """Tests `exmod`"""
 
         try:
-            with TemporaryDirectory(
-                prefix="gold", suffix="gold"
-            ) as existent_module_dir, TemporaryDirectory(
-                prefix="gen", suffix="gen"
-            ) as new_module_dir:
-                self._create_fs(existent_module_dir)
-                # sys.path.insert(0, existent_module_dir)
-                self._pip(["install", "."], existent_module_dir)
+            with TemporaryDirectory(prefix="search_root", suffix="search_path") as root:
+                _, new_module_dir = self.create_and_install_pkg(root)
 
                 exmod(
                     module=self.module_name,
                     emit_name="class",
                     blacklist=tuple(),
                     whitelist=tuple(),
                     mock_imports=True,
                     output_directory=new_module_dir,
+                    target_module_name=None,
                     no_word_wrap=None,
                     dry_run=False,
                 )
                 self._check_emission(new_module_dir)
         finally:
             # sys.path.remove(existent_module_dir)
-            self._pip(["uninstall", "-y", self.module_name])
+            self._pip(["uninstall", "-y", self.package_root_name])
 
     def test_exmod_blacklist(self) -> None:
         """Tests `exmod` blacklist"""
 
         try:
-            with TemporaryDirectory(
-                prefix="gold", suffix="gold"
-            ) as existent_module_dir, TemporaryDirectory(
-                prefix="gen", suffix="gen"
-            ) as new_module_dir:
-                self._create_fs(existent_module_dir)
-                self._pip(["install", "."], existent_module_dir)
+            with TemporaryDirectory(prefix="search_root", suffix="search_path") as root:
+                existent_module_dir, new_module_dir = self.create_and_install_pkg(root)
                 exmod(
                     module=self.module_name,
                     emit_name="class",
-                    blacklist=(".".join((self.module_name,) * 2),),
+                    blacklist=(".".join((existent_module_dir,) * 2),),
                     whitelist=tuple(),
                     mock_imports=True,
                     output_directory=new_module_dir,
+                    target_module_name=None,
                     no_word_wrap=None,
                     dry_run=False,
                 )
-                self.assertListEqual(listdir(new_module_dir), [])
+                self.assertListEqual(
+                    listdir(new_module_dir), [INIT_FILENAME, self.parent_dir]
+                )
         finally:
-            self._pip(["uninstall", "-y", self.module_name])
+            self._pip(["uninstall", "-y", self.package_root_name])
 
     def test_exmod_whitelist(self) -> None:
         """Tests `exmod` whitelist"""
 
         try:
-            with TemporaryDirectory(
-                prefix="gold", suffix="gold"
-            ) as existent_module_dir, TemporaryDirectory(
-                prefix="gen", suffix="gen"
-            ) as new_module_dir:
-                self._create_fs(existent_module_dir)
-                self._pip(["install", "."], existent_module_dir)
-                existent_module_name = path.basename(existent_module_dir)
+            with TemporaryDirectory(prefix="search_root", suffix="search_path") as root:
+                existent_module_dir, new_module_dir = self.create_and_install_pkg(root)
                 exmod(
                     module=self.module_name,
                     emit_name="class",
                     blacklist=tuple(),
-                    whitelist=(".".join((existent_module_name,) * 2),),
+                    whitelist=(".".join((self.package_root_name, "gen")),),
                     mock_imports=True,
                     output_directory=new_module_dir,
+                    target_module_name=None,
                     no_word_wrap=None,
                     dry_run=False,
                 )
 
+                new_module_dir_len = len(new_module_dir + path.sep)
                 gen, gold = map(
                     sorted,
                     (
-                        map(
-                            lambda p: (
-                                lambda _p: path.join("gold", _p.partition(path.sep)[2])
-                                if _p.startswith("gold") and _p.count("gold") == 2
-                                else _p
-                            )(p.partition(path.sep)[2]),
-                            (
-                                path.join(dirpath, filename)[
-                                    len(new_module_dir + path.sep) :
-                                ]
-                                for (dirpath, dirnames, filenames) in walk(
-                                    new_module_dir
-                                )
-                                for filename in filenames
-                            ),
-                        ),
                         (
-                            INIT_FILENAME,
-                            *chain.from_iterable(
-                                map(
-                                    lambda i: map(
-                                        partial(
-                                            path.join,
-                                            self.module_hierarchy[i][1],
-                                        ),
-                                        (
-                                            "{name}{sep}py".format(
-                                                name=self.module_hierarchy[i][0],
-                                                sep=extsep,
-                                            ),
-                                            INIT_FILENAME,
-                                        ),
-                                    ),
-                                    range(len(self.module_hierarchy)),
-                                ),
-                            ),
+                            path.join(dirpath, filename)[new_module_dir_len:]
+                            for (dirpath, dirnames, filenames) in walk(new_module_dir)
+                            for filename in filenames
                         ),
-                    ),
-                )
-                all_tests_running = len(gold) == 7
-                if all_tests_running:
-                    gold = list(
                         chain.from_iterable(
                             (
-                                gold[:1],
+                                (INIT_FILENAME,),
                                 chain.from_iterable(
-                                    map(
-                                        lambda p: (p, p),
-                                        map(
-                                            partial(path.join, "gold", "parent_dir"),
-                                            (
-                                                INIT_FILENAME,
-                                                *map(
-                                                    partial(path.join, "child_dir"),
-                                                    (
-                                                        INIT_FILENAME,
-                                                        "child{sep}py".format(
-                                                            sep=extsep
-                                                        ),
-                                                        path.join(
-                                                            "grandchild_dir",
-                                                            INIT_FILENAME,
-                                                        ),
-                                                        path.join(
-                                                            "grandchild_dir",
-                                                            "grandchild{sep}py".format(
-                                                                sep=extsep
-                                                            ),
-                                                        ),
-                                                    ),
-                                                ),
-                                                "parent{sep}py".format(sep=extsep),
-                                            ),
+                                    (
+                                        path.join(directory, INIT_FILENAME),
+                                        "{basepath}{extsep}py".format(
+                                            basepath=path.join(directory, name),
+                                            extsep=path.extsep,
                                         ),
                                     )
+                                    for name, directory in self.module_hierarchy
                                 ),
-                                gold[1:],
                             )
-                        )
-                    )
+                        ),
+                    ),
+                )
 
                 self.assertListEqual(gen, gold)
         finally:
-            self._pip(["uninstall", "-y", self.module_name])
+            self._pip(["uninstall", "-y", self.package_root_name])
 
     def test_exmod_module_directory(self) -> None:
         """Tests `exmod` module whence directory"""
 
         with TemporaryDirectory() as tempdir, self.assertRaises(ModuleNotFoundError):
             exmod(
                 module=tempdir,
                 emit_name="cool_name",
                 blacklist=tuple(),
                 whitelist=tuple(),
                 mock_imports=True,
                 output_directory=path.join(tempdir, "nonexistent"),
+                target_module_name=None,
                 no_word_wrap=None,
                 dry_run=False,
             )
 
     def test_exmod_no_module(self) -> None:
         """Tests that ModuleNotFound error is raised when module is not installed"""
         with TemporaryDirectory() as tempdir, self.assertRaises(ModuleNotFoundError):
             exmod(
                 module="fubar",
                 emit_name="uncool_name",
                 blacklist=tuple(),
                 whitelist=tuple(),
                 mock_imports=True,
                 output_directory=path.join(tempdir, "nonexistent"),
+                target_module_name=None,
                 no_word_wrap=None,
                 dry_run=False,
             )
 
     def test_exmod_output_directory_nonexistent(self) -> None:
         """Tests `exmod` module whence directory does not exist"""
 
@@ -229,38 +187,37 @@
             exmod(
                 module=output_directory,
                 emit_name=None,
                 blacklist=tuple(),
                 whitelist=tuple(),
                 mock_imports=True,
                 output_directory=output_directory,
+                target_module_name=None,
                 no_word_wrap=None,
                 dry_run=False,
             )
 
     def test_exmod_dry_run(self) -> None:
         """Tests `exmod` dry_run"""
 
         try:
-            with TemporaryDirectory(
-                prefix="gold", suffix="gold"
-            ) as existent_module_dir, TemporaryDirectory(
-                prefix="gen", suffix="gen"
-            ) as new_module_dir:
-                self._create_fs(existent_module_dir)
-                self._pip(["install", "."], existent_module_dir)
+            with TemporaryDirectory(prefix="search_root", suffix="search_path") as root:
+                _, new_module_dir = self.create_and_install_pkg(root)
 
-                with patch("sys.stdout", new_callable=StringIO) as f:
+                with patch(
+                    "cdd.compound.exmod_utils.EXMOD_OUT_STREAM", new_callable=StringIO
+                ) as f:
                     exmod(
                         module=self.module_name,
                         emit_name="class",
                         blacklist=tuple(),
                         whitelist=tuple(),
                         mock_imports=True,
                         output_directory=new_module_dir,
+                        target_module_name=None,
                         no_word_wrap=None,
                         dry_run=True,
                     )
                     r = f.getvalue()
 
                 result = dict(
                     map(
@@ -304,195 +261,235 @@
                         ),
                     )
                 )
 
                 all_tests_running = len(result["write"]) == 1
 
                 key_counts = (
-                    (("mkdir", 10), ("touch", 4), ("write", 1))
+                    (("mkdir", 4), ("touch", 1), ("write", 1))
                     if all_tests_running
                     else (("mkdir", 7), ("touch", 4), ("write", 4))
                 )
 
                 for key, count in key_counts:
                     self.assertEqual(count, len(result[key]), key)
 
-                gold_module_name = next(
-                    map(
-                        lambda p: p.partition(path.sep)[0],
-                        filter(rpartial(str.startswith, "gold"), result["mkdir"]),
-                    ),
-                    path.basename(self.gold_dir),
-                )
-                gold = {
-                    k: tuple(map(unquote, map(repr, v)))
-                    for k, v in {
-                        "mkdir": chain.from_iterable(
-                            (
-                                (new_module_dir,),
-                                map(
-                                    partial(path.join, gold_module_name),
-                                    (
-                                        self.module_hierarchy[0][1],
-                                        self.module_hierarchy[1][1],
-                                        self.module_hierarchy[2][1],
-                                    ),
-                                )
-                                if all_tests_running
-                                else iter(()),
-                                (
-                                    self.module_hierarchy[0][1],
-                                    self.module_hierarchy[1][1],
-                                    path.join(
-                                        self.module_hierarchy[1][1],
-                                        self.module_hierarchy[1][0],
-                                    ),
-                                    self.module_hierarchy[2][1],
-                                    path.join(
-                                        self.module_hierarchy[2][1],
-                                        self.module_hierarchy[2][0],
-                                    ),
-                                    path.join(
-                                        self.module_hierarchy[0][1],
-                                        self.module_hierarchy[0][0],
-                                    ),
-                                ),
+                gold = dict(
+                    touch=(path.join(path.dirname(self.gold_dir), INIT_FILENAME),),
+                    **{
+                        k: tuple(
+                            map(
+                                rpartial(str.rstrip, path.sep),
+                                map(partial(path.join, new_module_dir), v),
                             )
-                        ),
-                        "touch": (
-                            INIT_FILENAME,
-                            *map(
-                                rpartial(path.join, INIT_FILENAME),
-                                (
-                                    self.module_hierarchy[0][1],
-                                    self.module_hierarchy[1][1],
-                                    self.module_hierarchy[2][1],
+                        )
+                        for k, v in {
+                            "mkdir": ("", *map(itemgetter(1), self.module_hierarchy)),
+                            "write": (INIT_FILENAME,),
+                        }.items()
+                    },
+                )
+                self.maxDiff = None
+                self.assertDictEqual(result, gold)
+
+                self._check_emission(new_module_dir, dry_run=True)
+        finally:
+            self._pip(["uninstall", "-y", self.package_root_name])
+
+    def create_and_install_pkg(self, root):
+        """
+        Create and install the pacakge
+
+        :param root: Root directory
+        :type root: ```str```
+
+        :return: existent_module_dir, new_module_dir
+        :rtype: ```Tuple[str,str]```
+        """
+        self.package_root_name = path.basename(root)
+        existent_module_dir = path.join(root, self.package_root_name, "gen")
+        new_module_dir = path.join(root, self.package_root_name, "gold")
+        package_root_mod_dir = path.join(root, self.package_root_name)
+        mkdir(package_root_mod_dir)
+        with open(
+            path.join(package_root_mod_dir, "__init__{extsep}py".format(extsep=extsep)),
+            "wt",
+        ) as f:
+            f.write(
+                "{encoding}\n\n"
+                "{mod}\n".format(
+                    encoding=ENCODING,
+                    mod=to_code(
+                        Module(
+                            body=[
+                                ImportFrom(
+                                    module=".".join((self.package_root_name, "gen")),
+                                    names=[
+                                        alias(
+                                            "*",
+                                            None,
+                                            identifier=None,
+                                            identifier_name=None,
+                                        )
+                                    ],
+                                    level=0,
                                 ),
-                            ),
-                        ),
-                        "write": (
-                            lambda write_block: tuple(write_block[:1])
-                            if all_tests_running
-                            else write_block
-                        )(
-                            (
-                                INIT_FILENAME,
-                                path.join(
-                                    self.module_hierarchy[1][1],
-                                    "{name}{extsep}py".format(
-                                        name=self.module_hierarchy[1][0],
-                                        extsep=extsep,
+                                Assign(
+                                    targets=[Name("__author__", Store())],
+                                    value=set_value(
+                                        environ.get("CDD_AUTHOR", "Samuel Marks")
                                     ),
+                                    expr=None,
+                                    lineno=None,
+                                    **maybe_type_comment,
                                 ),
-                                path.join(
-                                    self.module_hierarchy[2][1],
-                                    "{name}{extsep}py".format(
-                                        name=self.module_hierarchy[2][0],
-                                        extsep=extsep,
+                                Assign(
+                                    targets=[Name("__version__", Store())],
+                                    value=set_value(
+                                        environ.get("CDD_VERSION", "0.0.0")
                                     ),
+                                    expr=None,
+                                    lineno=None,
+                                    **maybe_type_comment,
                                 ),
-                                path.join(
-                                    self.module_hierarchy[0][1],
-                                    "{name}{extsep}py".format(
-                                        name=self.module_hierarchy[0][0],
-                                        extsep=extsep,
+                                Assign(
+                                    targets=[Name("__all__", Store())],
+                                    value=List(
+                                        ctx=Load(),
+                                        elts=list(
+                                            map(
+                                                set_value,
+                                                chain.from_iterable(
+                                                    (
+                                                        (
+                                                            "__author__",
+                                                            "__version__",
+                                                        ),
+                                                        map(
+                                                            itemgetter(0),
+                                                            self.module_hierarchy,
+                                                        ),
+                                                    )
+                                                ),
+                                            )
+                                        ),
+                                        expr=None,
                                     ),
+                                    expr=None,
+                                    lineno=None,
+                                    **maybe_type_comment,
                                 ),
-                            )
-                        ),
-                    }.items()
-                }
-
-                self.assertDictEqual(result, gold)
-
-                self._check_emission(new_module_dir, dry_run=True)
-        finally:
-            self._pip(["uninstall", "-y", self.module_name])
+                            ],
+                            type_ignores=[],
+                            stmt=None,
+                        )
+                    ),
+                )
+            )
+        mkdir(new_module_dir)
+        self._create_fs(existent_module_dir)
+        self._pip(["install", "."], root)
+        return existent_module_dir, new_module_dir
 
-    def _create_fs(self, tempdir):
+    def _create_fs(self, module_root):
         """
-        Populate filesystem from `tempdir` root with module hierarchy &etc. for later exposure (exmod)
+        Populate filesystem from `module_root` root with module hierarchy &etc. for later exposure (exmod)
 
-        :param tempdir: Temporary directory
-        :type tempdir: ```str```
+        :param module_root: Root directory for module, one directory below setup.py
+        :type module_root: ```str```
 
-        :return: tempdir
+        :return: module_root
         :rtype: ```str```
         """
-        self.module_name, self.gold_dir = path.basename(tempdir), tempdir
-        self.parent_name, self.parent_dir = "parent", "parent_dir"
-        self.child_name, self.child_dir = "child", path.join(
-            self.parent_dir, "child_dir"
-        )
-        self.grandchild_name, self.grandchild_dir = "grandchild", path.join(
-            self.child_dir, "grandchild_dir"
-        )
-        self.module_hierarchy = (
-            (self.parent_name, self.parent_dir),
-            (self.child_name, self.child_dir),
-            (self.grandchild_name, self.grandchild_dir),
-        )
+        self.module_name, self.gold_dir = path.basename(module_root), module_root
+        package_root = path.dirname(path.dirname(module_root))
+        self.module_root_name = self.module_name
+
+        self.module_name = ".".join((self.package_root_name, self.module_name))
 
         with open(
-            path.join(tempdir, "setup{extsep}py".format(extsep=extsep)), "wt"
+            path.join(package_root, "setup{extsep}py".format(extsep=extsep)), "wt"
         ) as f:
             f.write(
-                setup_py_mock.format(encoding=ENCODING, package_name=self.module_name)
+                setup_py_mock.format(
+                    encoding=ENCODING,
+                    package_name=self.package_root_name,
+                    module_name=self.module_root_name,
+                )
             )
 
-        open(path.join(tempdir, "README{extsep}md".format(extsep=extsep)), "a").close()
-        mkdir(path.join(tempdir, self.module_name))
+        open(
+            path.join(package_root, "README{extsep}md".format(extsep=extsep)), "a"
+        ).close()
+        mkdir(module_root)
+
+        mod = Module(
+            body=list(
+                chain.from_iterable(
+                    (
+                        (
+                            ImportFrom(
+                                module=".".join(
+                                    (
+                                        self.package_root_name,
+                                        "gen",
+                                        directory.replace(path.sep, "."),
+                                    )
+                                ),
+                                names=[
+                                    alias(
+                                        name,
+                                        None,
+                                        identifier=None,
+                                        identifier_name=None,
+                                    )
+                                ],
+                                level=0,
+                            )
+                            for name, directory in self.module_hierarchy
+                        ),
+                        (
+                            Assign(
+                                targets=[Name("__all__", Store())],
+                                value=List(
+                                    ctx=Load(),
+                                    elts=list(
+                                        map(
+                                            set_value,
+                                            map(itemgetter(0), self.module_hierarchy),
+                                        )
+                                    ),
+                                    expr=None,
+                                ),
+                                expr=None,
+                                lineno=None,
+                                **maybe_type_comment,
+                            ),
+                        ),
+                    )
+                )
+            ),
+            type_ignores=[],
+            stmt=None,
+        )
+
         with open(
-            path.join(tempdir, self.module_name, INIT_FILENAME),
+            path.join(module_root, INIT_FILENAME),
             "wt",
         ) as f:
             f.write(
                 "{encoding}\n\n"
-                "{imports}\n"
-                "__author__ = {author!r}\n"
-                "__version__ = {version!r}\n\n"
-                "{all__}\n".format(
+                "{mod}".format(
                     encoding=ENCODING,
-                    imports="\n".join(
-                        (
-                            "import {module_name}.{other_imports}\n".format(
-                                module_name=self.module_name,
-                                other_imports="\nimport {module_name}.".format(
-                                    module_name=self.module_name
-                                ).join(
-                                    map(
-                                        rpartial(str.replace, path.sep, "."),
-                                        map(itemgetter(1), self.module_hierarchy),
-                                    )
-                                ),
-                            ),
-                        )
-                    ),
-                    # module_name=self.module_name,
-                    # parent_name=self.parent_name,
-                    # cls_name="{name}Class".format(name=self.parent_name.title()),
-                    author=environ.get("CDD_AUTHOR", "Samuel Marks"),
-                    version=environ.get("CDD_VERSION", "0.0.0"),
-                    all__="__all__ = {__all__!r}".format(
-                        __all__=list(
-                            map(
-                                rpartial(add, "_dir"),
-                                (
-                                    self.parent_name,
-                                    self.child_name,
-                                    self.grandchild_name,
-                                ),
-                            )
-                        )
-                    ),
+                    mod=to_code(mod),
                 )
             )
 
         for name, _folder in self.module_hierarchy:
-            folder = path.join(tempdir, self.module_name, _folder)
+            folder = path.join(module_root, _folder)
             mkdir(folder)
             cls_name = "{name}Class".format(name=name.title())
             with open(
                 path.join(folder, "__init__{extsep}py".format(extsep=extsep)), "wt"
             ) as f:
                 f.write(
                     "{encoding}\n\n"
@@ -515,31 +512,41 @@
                         encoding=ENCODING,
                         imports_header=imports_header,
                         class_str=class_str.replace("ConfigClass", cls_name),
                         cls_name=cls_name,
                     )
                 )
 
-        return tempdir
+        return module_root
 
     def _check_emission(self, tempdir, dry_run=False):
         """
         Confirm whether emission conforms to gen by verifying their IRs are equivalent
 
         :param tempdir: Temporary directory
         :type tempdir: ```str```
 
         :param dry_run: Show what would be created; don't actually write to the filesystem
         :type dry_run: ```bool```
         """
         new_module_name = path.basename(tempdir)
 
         for name, folder in self.module_hierarchy:
-            gen_folder = path.join(tempdir, new_module_name, folder)
-            gold_folder = path.join(self.gold_dir, self.module_name, folder)
+            gen_folder = path.join(
+                tempdir,
+                *(folder,)
+                if tempdir.rpartition(path.sep)[2] == new_module_name
+                else (new_module_name, folder),
+            )
+            gold_folder = path.join(
+                self.gold_dir,
+                *(folder,)
+                if self.gold_dir.endswith(self.module_name.replace(".", path.sep))
+                else (self.module_name, folder),
+            )
 
             def _open(_folder):
                 """
                 :param _folder: Folder to join on
                 :type _folder: ```str``
 
                 :return: Open IO
@@ -548,36 +555,36 @@
                 return open(
                     path.join(
                         _folder, "{name}{extsep}py".format(name=name, extsep=extsep)
                     ),
                     "rt",
                 )
 
-            self.assertTrue(path.isdir(gold_folder))
+            self.assertTrue(
+                path.isdir(gold_folder), "Expected {!r} to exist".format(gold_folder)
+            )
 
             gen_is_dir = path.isdir(gen_folder)
             if dry_run:
                 self.assertFalse(gen_is_dir)
             else:
-                self.assertTrue(gen_is_dir)
+                self.assertTrue(gen_is_dir, gen_folder)
 
                 with _open(gen_folder) as gen, _open(gold_folder) as gold:
                     gen_ir, gold_ir = map(
                         lambda ir: ir["_internal"].__delitem__("original_doc_str")
                         or ir,
                         map(
                             lambda node: cdd.class_.parse.class_(
                                 next(
                                     filter(
                                         rpartial(isinstance, ClassDef),
-                                        (
-                                            lambda node_read: ast_parse(  # print("%%%%%\n", node_read, ';') or
-                                                node_read
-                                            ).body
-                                        )(node.read()),
+                                        (lambda node_read: ast_parse(node_read).body)(
+                                            node.read()
+                                        ),
                                     )
                                 )
                             ),
                             (gen, gold),
                         ),
                     )
                     self.assertDictEqual(gold_ir, gen_ir)
@@ -590,19 +597,17 @@
         :param pip_args: Arguments to give pip
         :type pip_args: ```List[str]```
 
         :param cwd: Current working directory to run the command from. Defaults to current dir.
         :type cwd: ```Optional[str]```
         """
         self.assertEqual(
-            call(
+            run(
                 [executable, "-m", "pip"] + pip_args,
-                cwd=cwd,
-                stdout=DEVNULL,
-                stderr=DEVNULL,
-            ),
+                cwd=cwd,  # stdout=DEVNULL
+            ).returncode,
             0,
             "EXIT_SUCCESS not reached",
         )
 
 
 unittest_main()
```

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_compound/test_exmod_utils.py` & `python-cdd-0.0.99rc5/cdd/tests/test_compound/test_exmod_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 class TestExmodUtils(TestCase):
     """Test class for emitter_utils"""
 
     def test_emit_file_on_hierarchy_dry_run(self) -> None:
         """Test that `emit_file_on_hierarchy` works with dry_run"""
 
         ir = {"name": "YEP", "doc": None}
-        with patch("sys.stdout", new_callable=StringIO) as f:
+        with patch(
+            "cdd.compound.exmod_utils.EXMOD_OUT_STREAM", new_callable=StringIO
+        ) as f:
             emit_file_on_hierarchy(
                 ("", "foo_dir", ir),
                 "argparse",
                 "",
                 "",
                 True,
                 None,
@@ -41,15 +43,15 @@
         )
 
     def test_emit_file_on_hierarchy(self) -> None:
         """Test `emit_file_on_hierarchy`"""
 
         ir = {"name": "YEP", "doc": None}
         with patch(
-            "sys.stdout", new_callable=StringIO
+            "cdd.compound.exmod_utils.EXMOD_OUT_STREAM", new_callable=StringIO
         ), TemporaryDirectory() as tempdir:
             open(path.join(tempdir, INIT_FILENAME), "a").close()
             emit_file_on_hierarchy(
                 ("foo.bar", "foo_dir", ir),
                 "argparse",
                 "",
                 "",
@@ -59,17 +61,19 @@
                 no_word_wrap=None,
                 dry_run=False,
             )
             self.assertTrue(path.isdir(tempdir))
 
     def test__emit_symbols_isfile_emit_filename_true(self) -> None:
         """Test `_emit_symbol` when `isfile_emit_filename is True`"""
-        with patch("sys.stdout", new_callable=StringIO), patch(
-            "cdd.shared.ast_utils.merge_modules", MagicMock()
-        ) as f, patch("cdd.shared.ast_utils.merge_assignment_lists", MagicMock()) as g:
+        with patch(
+            "cdd.compound.exmod_utils.EXMOD_OUT_STREAM", new_callable=StringIO
+        ), patch("cdd.shared.ast_utils.merge_modules", MagicMock()) as f, patch(
+            "cdd.shared.ast_utils.merge_assignment_lists", MagicMock()
+        ) as g:
             _emit_symbol(
                 name_orig_ir=("", "", dict()),
                 emit_name="argparse",
                 module_name="module_name",
                 emit_filename="emit_filename",
                 existent_mod=None,
                 init_filepath="",
```

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_compound/test_gen.py` & `python-cdd-0.0.99rc5/cdd/tests/test_compound/test_gen.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_compound/test_gen_routes.py` & `python-cdd-0.0.99rc5/cdd/tests/test_compound/test_gen_routes.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_compound/test_gen_utils.py` & `python-cdd-0.0.99rc5/cdd/tests/test_compound/test_gen_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_compound/test_openapi_bulk.py` & `python-cdd-0.0.99rc5/cdd/tests/test_compound/test_openapi_bulk.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_compound/test_openapi_sub.py` & `python-cdd-0.0.99rc5/cdd/tests/test_compound/test_openapi_sub.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_compound/test_sync_properties.py` & `python-cdd-0.0.99rc5/cdd/tests/test_compound/test_sync_properties.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_docstring/test_emit_docstring.py` & `python-cdd-0.0.99rc5/cdd/tests/test_docstring/test_emit_docstring.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_docstring/test_parse_docstring.py` & `python-cdd-0.0.99rc5/cdd/tests/test_docstring/test_parse_docstring.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_emit/test_emit_file.py` & `python-cdd-0.0.99rc5/cdd/tests/test_emit/test_emit_file.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_emit/test_emitter_utils.py` & `python-cdd-0.0.99rc5/cdd/tests/test_emit/test_emitter_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_emit/test_emitters.py` & `python-cdd-0.0.99rc5/cdd/tests/test_emit/test_emitters.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_function/test_emit_function.py` & `python-cdd-0.0.99rc5/cdd/tests/test_function/test_emit_function.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_function/test_parse_function.py` & `python-cdd-0.0.99rc5/cdd/tests/test_function/test_parse_function.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_json_schema/test_emit_json_schema.py` & `python-cdd-0.0.99rc5/cdd/tests/test_json_schema/test_emit_json_schema.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_json_schema/test_emit_json_schema_utils.py` & `python-cdd-0.0.99rc5/cdd/tests/test_json_schema/test_emit_json_schema_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_json_schema/test_parse_json_schema.py` & `python-cdd-0.0.99rc5/cdd/tests/test_json_schema/test_parse_json_schema.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_json_schema/test_parse_json_schema_utils.py` & `python-cdd-0.0.99rc5/cdd/tests/test_json_schema/test_parse_json_schema_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_marshall_docstring.py` & `python-cdd-0.0.99rc5/cdd/tests/test_marshall_docstring.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_parse/test_parser_utils.py` & `python-cdd-0.0.99rc5/cdd/tests/test_parse/test_parser_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_parse/test_parsers.py` & `python-cdd-0.0.99rc5/cdd/tests/test_parse/test_parsers.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_pydantic/test_emit_pydantic.py` & `python-cdd-0.0.99rc5/cdd/tests/test_pydantic/test_emit_pydantic.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_pydantic/test_parse_pydantic.py` & `python-cdd-0.0.99rc5/cdd/tests/test_pydantic/test_parse_pydantic.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_routes/test_bottle_route_emit.py` & `python-cdd-0.0.99rc5/cdd/tests/test_routes/test_bottle_route_emit.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_routes/test_bottle_route_parse.py` & `python-cdd-0.0.99rc5/cdd/tests/test_routes/test_bottle_route_parse.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_routes/test_fastapi_routes_parse.py` & `python-cdd-0.0.99rc5/cdd/tests/test_routes/test_fastapi_routes_parse.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_routes/test_route_emit.py` & `python-cdd-0.0.99rc5/cdd/tests/test_routes/test_route_emit.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_routes/test_route_parse.py` & `python-cdd-0.0.99rc5/cdd/tests/test_routes/test_route_parse.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_setup.py` & `python-cdd-0.0.99rc5/cdd/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_shared/test_ast_cst_utils.py` & `python-cdd-0.0.99rc5/cdd/tests/test_shared/test_ast_cst_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_shared/test_ast_utils.py` & `python-cdd-0.0.99rc5/cdd/tests/test_shared/test_ast_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_shared/test_conformance.py` & `python-cdd-0.0.99rc5/cdd/tests/test_shared/test_conformance.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_shared/test_cst.py` & `python-cdd-0.0.99rc5/cdd/tests/test_shared/test_cst.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_shared/test_cst_utils.py` & `python-cdd-0.0.99rc5/cdd/tests/test_shared/test_cst_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_shared/test_default_utils.py` & `python-cdd-0.0.99rc5/cdd/tests/test_shared/test_default_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_shared/test_docstring_utils.py` & `python-cdd-0.0.99rc5/cdd/tests/test_shared/test_docstring_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_shared/test_pure_utils.py` & `python-cdd-0.0.99rc5/cdd/tests/test_shared/test_pure_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_shared/test_source_transformer.py` & `python-cdd-0.0.99rc5/cdd/tests/test_shared/test_source_transformer.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_sqlalchemy/test_emit_sqlalchemy.py` & `python-cdd-0.0.99rc5/cdd/tests/test_sqlalchemy/test_emit_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_sqlalchemy/test_emit_sqlalchemy_utils.py` & `python-cdd-0.0.99rc5/cdd/tests/test_sqlalchemy/test_emit_sqlalchemy_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -206,16 +206,20 @@
         primary_element = Column(Integer, ForeignKey('element.element_id'))
         ```
         """
         with TemporaryDirectory() as tempdir:
             mod_name = "test_update_with_imports_from_columns"
             temp_mod_dir = path.join(tempdir, mod_name)
             mkdir(temp_mod_dir)
-            node_filename = path.join(temp_mod_dir, "Node.py")
-            element_filename = path.join(temp_mod_dir, "Element.py")
+            node_filename = path.join(
+                temp_mod_dir, "Node{sep}py".format(sep=path.extsep)
+            )
+            element_filename = path.join(
+                temp_mod_dir, "Element{sep}py".format(sep=path.extsep)
+            )
             node_pk_with_phase1_fk = deepcopy(node_pk_tbl_class)
             node_pk_with_phase1_fk.body[2] = Assign(
                 targets=[Name(id="primary_element", ctx=Store())],
                 value=Call(
                     func=Name(id="Column", ctx=Load()),
                     args=[
                         Name(id="Element", ctx=Load()),
@@ -281,16 +285,20 @@
         primary_element = Column(Integer, ForeignKey('element.element_id'))
         ```
         """
         with TemporaryDirectory() as tempdir:
             mod_name = "test_update_with_imports_from_columns"
             temp_mod_dir = path.join(tempdir, mod_name)
             mkdir(temp_mod_dir)
-            node_filename = path.join(temp_mod_dir, "node.py")
-            element_filename = path.join(temp_mod_dir, "element.py")
+            node_filename = path.join(
+                temp_mod_dir, "node{sep}py".format(sep=path.extsep)
+            )
+            element_filename = path.join(
+                temp_mod_dir, "element{sep}py".format(sep=path.extsep)
+            )
             node_pk_with_phase1_fk = deepcopy(node_pk_tbl_class)
             node_pk_with_phase1_fk.body[2] = Assign(
                 targets=[Name(id="primary_element", ctx=Store())],
                 value=Call(
                     func=Name(id="Column", ctx=Load()),
                     args=[
                         Name(id="element", ctx=Load()),
```

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_sqlalchemy/test_parse_sqlalchemy.py` & `python-cdd-0.0.99rc5/cdd/tests/test_sqlalchemy/test_parse_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_sqlalchemy/test_parse_sqlalchemy_utils.py` & `python-cdd-0.0.99rc5/cdd/tests/test_sqlalchemy/test_parse_sqlalchemy_utils.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/test_utils_for_tests.py` & `python-cdd-0.0.99rc5/cdd/tests/test_utils_for_tests.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/cdd/tests/utils_for_tests.py` & `python-cdd-0.0.99rc5/cdd/tests/utils_for_tests.py`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/python_cdd.egg-info/PKG-INFO` & `python-cdd-0.0.99rc5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,7 @@
-Metadata-Version: 2.1
-Name: python-cdd
-Version: 0.0.99rc4
-Summary: Open API to/fro routes, models, and tests. Convert between docstrings, classes, methods, argparse, pydantic, and SQLalchemy.
-Home-page: https://github.com/offscale/cdd-python
-Author: Samuel Marks
-Author-email: 807580+SamuelMarks@users.noreply.github.com
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Topic :: Software Development :: Code Generators
-Classifier: Topic :: Software Development :: Compilers
-Classifier: Topic :: Software Development :: Pre-processors
-Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE-APACHE
-License-File: LICENSE-MIT
-
 cdd-python
 ==========
 ![Python version range](https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8%20|%203.9%20|%203.10%20|%203.11-blue.svg)
 ![Python implementation](https://img.shields.io/badge/implementation-cpython-blue.svg)
 [![License](https://img.shields.io/badge/license-Apache--2.0%20OR%20MIT-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Linting, testing, coverage, and release](https://github.com/offscale/cdd-python/workflows/Linting,%20testing,%20coverage,%20and%20release/badge.svg)](https://github.com/offscale/cdd-python/actions)
 ![Tested OSs, others may work](https://img.shields.io/badge/Tested%20on-Linux%20|%20macOS%20|%20Windows-green)
@@ -512,21 +476,20 @@
   inline ([PEP484](https://python.org/dev/peps/pep-0484)–style))
 - Switch between docstring formats (to/from {numpy, ReST, google})
 - Desktop GUI with wxWidgets, from the argparse layer through [Gooey](https://github.com/chriskiehl/Gooey) [one liner]
 
 ## CLI for this project
 
     $ python -m cdd --help
-    
     usage: python -m cdd [-h] [--version]
                          {sync_properties,sync,gen,gen_routes,openapi,doctrans,exmod}
                          ...
     
     Open API to/fro routes, models, and tests. Convert between docstrings,
-    classes, methods, argparse, and SQLalchemy.
+    classes, methods, argparse, pydantic, and SQLalchemy.
     
     positional arguments:
       {sync_properties,sync,gen,gen_routes,openapi,doctrans,exmod}
         sync_properties     Synchronise one or more properties between input and
                             input_str Python files
         sync                Force argparse, classes, and/or methods to be
                             equivalent
@@ -543,43 +506,44 @@
     options:
       -h, --help            show this help message and exit
       --version             show program's version number and exit
 
 ### `sync`
 
     $ python -m cdd sync --help
-
     usage: python -m cdd sync [-h] [--argparse-function ARGPARSE_FUNCTIONS]
                               [--argparse-function-name ARGPARSE_FUNCTION_NAMES]
                               [--class CLASSES] [--class-name CLASS_NAMES]
                               [--function FUNCTIONS]
-                              [--function-name FUNCTION_NAMES] --truth
-                              {argparse_function,class,function}
+                              [--function-name FUNCTION_NAMES] [--no-word-wrap]
+                              --truth
+                              {argparse_function,class,function,sqlalchemy,sqlalchemy_table}
     
     options:
       -h, --help            show this help message and exit
       --argparse-function ARGPARSE_FUNCTIONS
                             File where argparse function is `def`ined.
       --argparse-function-name ARGPARSE_FUNCTION_NAMES
                             Name of argparse function.
       --class CLASSES       File where class `class` is declared.
       --class-name CLASS_NAMES
                             Name of `class`
       --function FUNCTIONS  File where function is `def`ined.
       --function-name FUNCTION_NAMES
                             Name of Function. If method, use Python resolution
                             syntax, i.e., ClassName.function_name
-      --truth {argparse_function,class,function}
+      --no-word-wrap        Whether word-wrap is disabled (on emission). None
+                            enables word-wrap. Defaults to None.
+      --truth {argparse_function,class,function,sqlalchemy,sqlalchemy_table}
                             Single source of truth. Others will be generated from
                             this. Will run with first found choice.
 
 ### `sync_properties`
 
     $ python -m cdd sync_properties --help
-
     usage: python -m cdd sync_properties [-h] --input-filename INPUT_FILENAME
                                          --input-param INPUT_PARAMS [--input-eval]
                                          --output-filename OUTPUT_FILENAME
                                          --output-param OUTPUT_PARAMS
                                          [--output-param-wrap OUTPUT_PARAM_WRAP]
     
     options:
@@ -600,54 +564,59 @@
       --output-param-wrap OUTPUT_PARAM_WRAP
                             Wrap all input_str params with this. E.g.,
                             `Optional[Union[{output_param}, str]]`
 
 ### `gen`
 
     $ python -m cdd gen --help
-
     usage: python -m cdd gen [-h] --name-tpl NAME_TPL --input-mapping
                              INPUT_MAPPING [--prepend PREPEND]
                              [--imports-from-file IMPORTS_FROM_FILE]
-                             [--parse {argparse,class,function,sqlalchemy,sqlalchemy_table}]
+                             [--parse {argparse,class,function,json_schema,pydantic,sqlalchemy,sqlalchemy_table,infer}]
                              --emit
-                             {argparse,class,function,sqlalchemy,sqlalchemy_table}
+                             {argparse,class,function,json_schema,pydantic,sqlalchemy,sqlalchemy_table}
                              --output-filename OUTPUT_FILENAME [--emit-call]
-                             [--decorator DECORATOR_LIST]
+                             [--emit-and-infer-imports] [--no-word-wrap]
+                             [--decorator DECORATOR_LIST] [--phase PHASE]
     
-    optional arguments:
+    options:
       -h, --help            show this help message and exit
       --name-tpl NAME_TPL   Template for the name, e.g., `{name}Config`.
       --input-mapping INPUT_MAPPING
                             Fully-qualified module, filepath, or directory.
       --prepend PREPEND     Prepend file with this. Use '\n' for newlines.
       --imports-from-file IMPORTS_FROM_FILE
                             Extract imports from file and append to `output_file`.
                             If module or other symbol path given, resolve file
                             then use it.
-      --parse {argparse,class,function,sqlalchemy,sqlalchemy_table}
+      --parse {argparse,class,function,json_schema,pydantic,sqlalchemy,sqlalchemy_table,infer}
                             What type the input is.
-      --emit {argparse,class,function,sqlalchemy,sqlalchemy_table}
-                            What type to generate.
+      --emit {argparse,class,function,json_schema,pydantic,sqlalchemy,sqlalchemy_table}
+                            Which type to generate.
       --output-filename OUTPUT_FILENAME, -o OUTPUT_FILENAME
                             Output file to write to.
       --emit-call           Whether to place all the previous body into a new
                             `__call__` internal function
+      --emit-and-infer-imports
+                            Whether to emit and infer imports at the top of the
+                            generated code
+      --no-word-wrap        Whether word-wrap is disabled (on emission). None
+                            enables word-wrap. Defaults to None.
       --decorator DECORATOR_LIST
                             List of decorators.
-
+      --phase PHASE         Which phase to run through. E.g., SQLalchemy may
+                            require multiple phases to resolve foreign keys.
 
 PS: If you're outputting JSON-schema and want a file per schema then:
 
     python -c 'import sys,json,os; f=open(sys.argv[1], "rt"); d=json.load(f); f.close(); [(lambda f: json.dump(sc,f) or f.close())(open(os.path.join(os.path.dirname(sys.argv[1]), sc["$id"].rpartition("/")[2]), "wt")) for sc in d["schemas"]]' <path_to_json_file>
 
 ### `gen_routes`
 
     $ python -m cdd gen_routes --help
-
     usage: python -m cdd gen_routes [-h] --crud {CRUD,CR,C,R,U,D,CR,CU,CD,CRD}
                                     [--app-name APP_NAME] --model-path MODEL_PATH
                                     --model-name MODEL_NAME --routes-path
                                     ROUTES_PATH [--route ROUTE]
     
     options:
       -h, --help            show this help message and exit
@@ -666,74 +635,79 @@
                             'foo/routes'
       --route ROUTE         Name of the route, defaults to
                             `/api/{model_name.lower()}`
 
 ### `openapi`
 
     $ python -m cdd openapi --help
-
     usage: python -m cdd openapi [-h] [--app-name APP_NAME] --model-paths
-                                 MODEL_PATHS --routes-paths
-                                 [ROUTES_PATHS [ROUTES_PATHS ...]]
+                                 MODEL_PATHS --routes-paths [ROUTES_PATHS ...]
     
-    optional arguments:
+    options:
       -h, --help            show this help message and exit
       --app-name APP_NAME   Name of app (e.g., `app_name = Bottle();
                             @app_name.get('/api') def slash(): pass`)
       --model-paths MODEL_PATHS
                             Python module resolution (foo.models) or filepath
                             (foo/models)
-      --routes-paths [ROUTES_PATHS [ROUTES_PATHS ...]]
+      --routes-paths [ROUTES_PATHS ...]
                             Python module resolution 'foo.routes' or filepath
                             'foo/routes'
 
 ### `doctrans`
 
     $ python -m cdd doctrans --help
-    
     usage: python -m cdd doctrans [-h] --filename FILENAME --format
                                   {rest,google,numpydoc}
-                                  (--type-annotations | --no-type-annotations)
+                                  (--type-annotations | --no-type-annotations | --no-word-wrap)
     
     options:
       -h, --help            show this help message and exit
       --filename FILENAME   Python file to convert docstrings within. Edited in
                             place.
       --format {rest,google,numpydoc}
                             The docstring format to replace existing format with.
       --type-annotations    Inline the type, i.e., annotate PEP484 (outside
                             docstring. Requires 3.6+)
       --no-type-annotations
                             Ensure all types are in docstring (rather than a
                             PEP484 type annotation)
+      --no-word-wrap        Whether word-wrap is disabled (on emission). None
+                            enables word-wrap. Defaults to None.
 
 ### `exmod`
 
     $ python -m cdd exmod --help
-    
     usage: python -m cdd exmod [-h] --module MODULE --emit
-                               {argparse,class,function,sqlalchemy,sqlalchemy_table}
-                               [--blacklist BLACKLIST] [--whitelist WHITELIST]
-                               --output-directory OUTPUT_DIRECTORY [--dry-run]
+                               {argparse,class,function,json_schema,pydantic,sqlalchemy,sqlalchemy_table}
+                               [--no-word-wrap] [--blacklist BLACKLIST]
+                               [--whitelist WHITELIST] --output-directory
+                               OUTPUT_DIRECTORY
+                               [--target-module-name TARGET_MODULE_NAME]
+                               [--dry-run]
     
     options:
       -h, --help            show this help message and exit
       --module MODULE, -m MODULE
                             The module or fully-qualified name (FQN) to expose.
-      --emit {argparse,class,function,sqlalchemy,sqlalchemy_table}
-                            What type to generate.
+      --emit {argparse,class,function,json_schema,pydantic,sqlalchemy,sqlalchemy_table}
+                            Which type to generate.
+      --no-word-wrap        Whether word-wrap is disabled (on emission). None
+                            enables word-wrap. Defaults to None.
       --blacklist BLACKLIST
                             Modules/FQN to omit. If unspecified will emit all
                             (unless whitelist).
       --whitelist WHITELIST
                             Modules/FQN to emit. If unspecified will emit all
                             (minus blacklist).
       --output-directory OUTPUT_DIRECTORY, -o OUTPUT_DIRECTORY
                             Where to place the generated exposed interfaces to the
                             given `--module`.
+      --target-module-name TARGET_MODULE_NAME
+                            Target module name. Defaults to `${module}.gold`.
       --dry-run             Show what would be created; don't actually write to
                             the filesystem.
 
 ---
 
 ## License
```

### Comparing `python-cdd-0.0.99rc4/python_cdd.egg-info/SOURCES.txt` & `python-cdd-0.0.99rc5/python_cdd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-cdd-0.0.99rc4/setup.py` & `python-cdd-0.0.99rc5/setup.py`

 * *Files identical despite different names*

