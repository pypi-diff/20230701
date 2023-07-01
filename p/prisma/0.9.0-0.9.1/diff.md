# Comparing `tmp/prisma-0.9.0.tar.gz` & `tmp/prisma-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prisma-0.9.0.tar", last modified: Mon Jun 12 02:14:09 2023, max compression
+gzip compressed data, was "prisma-0.9.1.tar", last modified: Sat Jul  1 09:59:52 2023, max compression
```

## Comparing `prisma-0.9.0.tar` & `prisma-0.9.1.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:14:09.599296 prisma-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 02:13:55.000000 prisma-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-12 02:13:55.000000 prisma-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-06-12 02:14:09.599296 prisma-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-06-12 02:13:55.000000 prisma-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-12 02:13:55.000000 prisma-0.9.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:14:09.591296 prisma-0.9.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-12 02:13:55.000000 prisma-0.9.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 02:13:55.000000 prisma-0.9.0/requirements/node.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 02:14:09.599296 prisma-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-12 02:13:55.000000 prisma-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:14:09.591296 prisma-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:14:09.591296 prisma-0.9.0/src/prisma/
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/_async_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/_raw_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/_sync_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:14:09.595296 prisma-0.9.0/src/prisma/binaries/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/binaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/binaries/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/binaries/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:14:09.595296 prisma-0.9.0/src/prisma/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/cli/_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:14:09.595296 prisma-0.9.0/src/prisma/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/cli/commands/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/cli/commands/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/cli/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/cli/commands/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/cli/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/cli/prisma.py
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:14:09.595296 prisma-0.9.0/src/prisma/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/engine/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/engine/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/engine/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:14:09.595296 prisma-0.9.0/src/prisma/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/jsonrpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    32409 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:14:09.599296 prisma-0.9.0/src/prisma/generator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/_header.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/_utils.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)    35089 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/actions.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/bases.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)    24388 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/builder.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)    24425 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/client.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:14:09.599296 prisma-0.9.0/src/prisma/generator/templates/engine/
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/engine/abstract.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/engine/http.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/engine/query.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/enums.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/fields.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/http.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/models.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/partials.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)    21757 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/templates/types.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/generator/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/http_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    13272 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/mypy.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:14:09.595296 prisma-0.9.0/src/prisma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-06-12 02:14:09.000000 prisma-0.9.0/src/prisma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-12 02:14:09.000000 prisma-0.9.0/src/prisma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 02:14:09.000000 prisma-0.9.0/src/prisma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-12 02:14:09.000000 prisma-0.9.0/src/prisma.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 02:14:09.000000 prisma-0.9.0/src/prisma.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-12 02:14:09.000000 prisma-0.9.0/src/prisma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 02:14:09.000000 prisma-0.9.0/src/prisma.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:14:09.599296 prisma-0.9.0/src/prisma_cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma_cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma_cleanup/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma_cleanup/_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:13:55.000000 prisma-0.9.0/src/prisma_cleanup/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:59:52.881873 prisma-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-01 09:59:35.000000 prisma-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-01 09:59:35.000000 prisma-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16610 2023-07-01 09:59:52.881873 prisma-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15104 2023-07-01 09:59:35.000000 prisma-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-01 09:59:35.000000 prisma-0.9.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:59:52.873872 prisma-0.9.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-01 09:59:35.000000 prisma-0.9.1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-01 09:59:35.000000 prisma-0.9.1/requirements/node.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 09:59:52.881873 prisma-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-07-01 09:59:35.000000 prisma-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:59:52.873872 prisma-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:59:52.877872 prisma-0.9.1/src/prisma/
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/_async_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/_raw_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/_sync_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:59:52.877872 prisma-0.9.1/src/prisma/binaries/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/binaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/binaries/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/binaries/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:59:52.877872 prisma-0.9.1/src/prisma/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/cli/_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:59:52.877872 prisma-0.9.1/src/prisma/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/cli/commands/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/cli/commands/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/cli/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/cli/commands/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/cli/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/cli/prisma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:59:52.877872 prisma-0.9.1/src/prisma/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/engine/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/engine/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/engine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:59:52.881873 prisma-0.9.1/src/prisma/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/generator/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/generator/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/generator/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/generator/jsonrpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32409 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/generator/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/generator/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:59:52.881873 prisma-0.9.1/src/prisma/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/generator/templates/_header.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/generator/templates/_utils.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)    35089 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/generator/templates/actions.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/generator/templates/bases.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)    24388 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/generator/templates/builder.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)    24425 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/generator/templates/client.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:59:52.881873 prisma-0.9.1/src/prisma/generator/templates/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/generator/templates/engine/abstract.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/generator/templates/engine/http.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     6741 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/generator/templates/engine/query.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/generator/templates/enums.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/generator/templates/fields.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/generator/templates/http.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/generator/templates/models.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/generator/templates/partials.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)    21757 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/generator/templates/types.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/generator/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/generator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/http_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13272 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/mypy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:59:52.877872 prisma-0.9.1/src/prisma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16610 2023-07-01 09:59:52.000000 prisma-0.9.1/src/prisma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-01 09:59:52.000000 prisma-0.9.1/src/prisma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 09:59:52.000000 prisma-0.9.1/src/prisma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-01 09:59:52.000000 prisma-0.9.1/src/prisma.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 09:59:52.000000 prisma-0.9.1/src/prisma.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-01 09:59:52.000000 prisma-0.9.1/src/prisma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-01 09:59:52.000000 prisma-0.9.1/src/prisma.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:59:52.881873 prisma-0.9.1/src/prisma_cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma_cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma_cleanup/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma_cleanup/_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:59:35.000000 prisma-0.9.1/src/prisma_cleanup/py.typed
```

### Comparing `prisma-0.9.0/LICENSE` & `prisma-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/PKG-INFO` & `prisma-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prisma
-Version: 0.9.0
+Version: 0.9.1
 Summary: Prisma Client Python is an auto-generated and fully type-safe database client
 Home-page: https://github.com/RobertCraigie/prisma-client-py
 Author: Robert Craigie
 Author-email: robert@craigie.dev
 Maintainer: Robert Craigie
 License: APACHE
 Project-URL: Documentation, https://prisma-client-py.readthedocs.io
@@ -159,15 +159,15 @@
 
 ### Prisma generator
 
 A prisma schema can define one or more generators, defined by the `generator` block.
 
 A generator determines what assets are created when you run the `prisma generate` command. The `provider` value defines which Prisma Client will be created. In this case, as we want to generate Prisma Client Python, we use the `prisma-client-py` value.
 
-You can also define where the client will be generated to with the `output` option. By default Prisma Client Python will be generated to the same location it was installed to, whether thats inside a virtual environment, the global python installation or anywhere else that python packages can be imported from.
+You can also define where the client will be generated to with the `output` option. By default Prisma Client Python will be generated to the same location it was installed to, whether that's inside a virtual environment, the global python installation or anywhere else that python packages can be imported from.
 
 For more options see [configuring Prisma Client Python](https://prisma-client-py.readthedocs.io/en/stable/reference/config/).
 
 ---
 
 ### Accessing your database with Prisma Client Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prisma Version: 0.9.0 Summary: Prisma Client Python
+Metadata-Version: 2.1 Name: prisma Version: 0.9.1 Summary: Prisma Client Python
 is an auto-generated and fully type-safe database client Home-page: https://
 github.com/RobertCraigie/prisma-client-py Author: Robert Craigie Author-email:
 robert@craigie.dev Maintainer: Robert Craigie License: APACHE Project-URL:
 Documentation, https://prisma-client-py.readthedocs.io Project-URL: Source,
 https://github.com/RobertCraigie/prisma-client-py Project-URL: Tracker, https:/
 /github.com/RobertCraigie/prisma-client-py/issues Keywords:
 orm,mysql,typing,prisma,sqlite,database,postgresql Platform: UNKNOWN
@@ -89,15 +89,15 @@
 documentation pages. ### Prisma generator A prisma schema can define one or
 more generators, defined by the `generator` block. A generator determines what
 assets are created when you run the `prisma generate` command. The `provider`
 value defines which Prisma Client will be created. In this case, as we want to
 generate Prisma Client Python, we use the `prisma-client-py` value. You can
 also define where the client will be generated to with the `output` option. By
 default Prisma Client Python will be generated to the same location it was
-installed to, whether thats inside a virtual environment, the global python
+installed to, whether that's inside a virtual environment, the global python
 installation or anywhere else that python packages can be imported from. For
 more options see [configuring Prisma Client Python](https://prisma-client-
 py.readthedocs.io/en/stable/reference/config/). --- ### Accessing your database
 with Prisma Client Python Just want to play around with Prisma Client Python
 and not worry about any setup? You can try it out online on [gitpod](https://
 gitpod.io/#https://github.com/RobertCraigie/prisma-py-async-quickstart). ####
 Installing Prisma Client Python The first step with any python project should
```

### Comparing `prisma-0.9.0/README.md` & `prisma-0.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 
 ### Prisma generator
 
 A prisma schema can define one or more generators, defined by the `generator` block.
 
 A generator determines what assets are created when you run the `prisma generate` command. The `provider` value defines which Prisma Client will be created. In this case, as we want to generate Prisma Client Python, we use the `prisma-client-py` value.
 
-You can also define where the client will be generated to with the `output` option. By default Prisma Client Python will be generated to the same location it was installed to, whether thats inside a virtual environment, the global python installation or anywhere else that python packages can be imported from.
+You can also define where the client will be generated to with the `output` option. By default Prisma Client Python will be generated to the same location it was installed to, whether that's inside a virtual environment, the global python installation or anywhere else that python packages can be imported from.
 
 For more options see [configuring Prisma Client Python](https://prisma-client-py.readthedocs.io/en/stable/reference/config/).
 
 ---
 
 ### Accessing your database with Prisma Client Python
```

#### html2text {}

```diff
@@ -69,15 +69,15 @@
 documentation pages. ### Prisma generator A prisma schema can define one or
 more generators, defined by the `generator` block. A generator determines what
 assets are created when you run the `prisma generate` command. The `provider`
 value defines which Prisma Client will be created. In this case, as we want to
 generate Prisma Client Python, we use the `prisma-client-py` value. You can
 also define where the client will be generated to with the `output` option. By
 default Prisma Client Python will be generated to the same location it was
-installed to, whether thats inside a virtual environment, the global python
+installed to, whether that's inside a virtual environment, the global python
 installation or anywhere else that python packages can be imported from. For
 more options see [configuring Prisma Client Python](https://prisma-client-
 py.readthedocs.io/en/stable/reference/config/). --- ### Accessing your database
 with Prisma Client Python Just want to play around with Prisma Client Python
 and not worry about any setup? You can try it out online on [gitpod](https://
 gitpod.io/#https://github.com/RobertCraigie/prisma-py-async-quickstart). ####
 Installing Prisma Client Python The first step with any python project should
```

### Comparing `prisma-0.9.0/pyproject.toml` & `prisma-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/setup.py` & `prisma-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/__init__.py` & `prisma-0.9.1/src/prisma/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 __title__ = 'prisma'
 __author__ = 'RobertCraigie'
 __license__ = 'APACHE'
 __copyright__ = 'Copyright 2020-2023 RobertCraigie'
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 
 from typing import TYPE_CHECKING
 
 from ._config import config as config
 from .utils import setup_logging
 from . import errors as errors
 from .validator import *
```

### Comparing `prisma-0.9.0/src/prisma/_async_http.py` & `prisma-0.9.1/src/prisma/_async_http.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/_compat.py` & `prisma-0.9.1/src/prisma/_compat.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/_config.py` & `prisma-0.9.1/src/prisma/_config.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/_proxy.py` & `prisma-0.9.1/src/prisma/_proxy.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/_raw_query.py` & `prisma-0.9.1/src/prisma/_raw_query.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/_sync_http.py` & `prisma-0.9.1/src/prisma/_sync_http.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/_types.py` & `prisma-0.9.1/src/prisma/_types.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/binaries/platform.py` & `prisma-0.9.1/src/prisma/binaries/platform.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/cli/_node.py` & `prisma-0.9.1/src/prisma/cli/_node.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/cli/cli.py` & `prisma-0.9.1/src/prisma/cli/cli.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/cli/commands/dev.py` & `prisma-0.9.1/src/prisma/cli/commands/dev.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/cli/commands/fetch.py` & `prisma-0.9.1/src/prisma/cli/commands/fetch.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/cli/commands/generate.py` & `prisma-0.9.1/src/prisma/cli/commands/generate.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/cli/commands/version.py` & `prisma-0.9.1/src/prisma/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/cli/options.py` & `prisma-0.9.1/src/prisma/cli/options.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/cli/prisma.py` & `prisma-0.9.1/src/prisma/cli/prisma.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/cli/utils.py` & `prisma-0.9.1/src/prisma/cli/utils.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/engine/errors.py` & `prisma-0.9.1/src/prisma/engine/errors.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/engine/utils.py` & `prisma-0.9.1/src/prisma/engine/utils.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/errors.py` & `prisma-0.9.1/src/prisma/errors.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/generator/generator.py` & `prisma-0.9.1/src/prisma/generator/generator.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/generator/jsonrpc.py` & `prisma-0.9.1/src/prisma/generator/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/generator/models.py` & `prisma-0.9.1/src/prisma/generator/models.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/generator/schema.py` & `prisma-0.9.1/src/prisma/generator/schema.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/generator/templates/_header.py.jinja` & `prisma-0.9.1/src/prisma/generator/templates/_header.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/generator/templates/_utils.py.jinja` & `prisma-0.9.1/src/prisma/generator/templates/_utils.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/generator/templates/actions.py.jinja` & `prisma-0.9.1/src/prisma/generator/templates/actions.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/generator/templates/bases.py.jinja` & `prisma-0.9.1/src/prisma/generator/templates/bases.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/generator/templates/builder.py.jinja` & `prisma-0.9.1/src/prisma/generator/templates/builder.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/generator/templates/client.py.jinja` & `prisma-0.9.1/src/prisma/generator/templates/client.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/generator/templates/engine/abstract.py.jinja` & `prisma-0.9.1/src/prisma/generator/templates/engine/abstract.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/generator/templates/engine/http.py.jinja` & `prisma-0.9.1/src/prisma/generator/templates/engine/http.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/generator/templates/engine/query.py.jinja` & `prisma-0.9.1/src/prisma/generator/templates/engine/query.py.jinja`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,15 @@
 
         env = os.environ.copy()
         env.update(
             PRISMA_DML_PATH=str(self.dml_path.absolute()),
             RUST_LOG='error',
             RUST_LOG_FORMAT='json',
             PRISMA_CLIENT_ENGINE_TYPE='binary',
+            PRISMA_ENGINE_PROTOCOL='graphql',
         )
 
         if DEBUG:
             env.update(RUST_LOG='info')
 
         if datasources is not None:
             env.update(OVERWRITE_DATASOURCES=dumps(datasources))
```

### Comparing `prisma-0.9.0/src/prisma/generator/templates/fields.py.jinja` & `prisma-0.9.1/src/prisma/generator/templates/fields.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/generator/templates/models.py.jinja` & `prisma-0.9.1/src/prisma/generator/templates/models.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/generator/templates/partials.py.jinja` & `prisma-0.9.1/src/prisma/generator/templates/partials.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/generator/templates/types.py.jinja` & `prisma-0.9.1/src/prisma/generator/templates/types.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/generator/utils.py` & `prisma-0.9.1/src/prisma/generator/utils.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/http_abstract.py` & `prisma-0.9.1/src/prisma/http_abstract.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/mypy.py` & `prisma-0.9.1/src/prisma/mypy.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/testing.py` & `prisma-0.9.1/src/prisma/testing.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/utils.py` & `prisma-0.9.1/src/prisma/utils.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma/validator.py` & `prisma-0.9.1/src/prisma/validator.py`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma.egg-info/PKG-INFO` & `prisma-0.9.1/src/prisma.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prisma
-Version: 0.9.0
+Version: 0.9.1
 Summary: Prisma Client Python is an auto-generated and fully type-safe database client
 Home-page: https://github.com/RobertCraigie/prisma-client-py
 Author: Robert Craigie
 Author-email: robert@craigie.dev
 Maintainer: Robert Craigie
 License: APACHE
 Project-URL: Documentation, https://prisma-client-py.readthedocs.io
@@ -159,15 +159,15 @@
 
 ### Prisma generator
 
 A prisma schema can define one or more generators, defined by the `generator` block.
 
 A generator determines what assets are created when you run the `prisma generate` command. The `provider` value defines which Prisma Client will be created. In this case, as we want to generate Prisma Client Python, we use the `prisma-client-py` value.
 
-You can also define where the client will be generated to with the `output` option. By default Prisma Client Python will be generated to the same location it was installed to, whether thats inside a virtual environment, the global python installation or anywhere else that python packages can be imported from.
+You can also define where the client will be generated to with the `output` option. By default Prisma Client Python will be generated to the same location it was installed to, whether that's inside a virtual environment, the global python installation or anywhere else that python packages can be imported from.
 
 For more options see [configuring Prisma Client Python](https://prisma-client-py.readthedocs.io/en/stable/reference/config/).
 
 ---
 
 ### Accessing your database with Prisma Client Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prisma Version: 0.9.0 Summary: Prisma Client Python
+Metadata-Version: 2.1 Name: prisma Version: 0.9.1 Summary: Prisma Client Python
 is an auto-generated and fully type-safe database client Home-page: https://
 github.com/RobertCraigie/prisma-client-py Author: Robert Craigie Author-email:
 robert@craigie.dev Maintainer: Robert Craigie License: APACHE Project-URL:
 Documentation, https://prisma-client-py.readthedocs.io Project-URL: Source,
 https://github.com/RobertCraigie/prisma-client-py Project-URL: Tracker, https:/
 /github.com/RobertCraigie/prisma-client-py/issues Keywords:
 orm,mysql,typing,prisma,sqlite,database,postgresql Platform: UNKNOWN
@@ -89,15 +89,15 @@
 documentation pages. ### Prisma generator A prisma schema can define one or
 more generators, defined by the `generator` block. A generator determines what
 assets are created when you run the `prisma generate` command. The `provider`
 value defines which Prisma Client will be created. In this case, as we want to
 generate Prisma Client Python, we use the `prisma-client-py` value. You can
 also define where the client will be generated to with the `output` option. By
 default Prisma Client Python will be generated to the same location it was
-installed to, whether thats inside a virtual environment, the global python
+installed to, whether that's inside a virtual environment, the global python
 installation or anywhere else that python packages can be imported from. For
 more options see [configuring Prisma Client Python](https://prisma-client-
 py.readthedocs.io/en/stable/reference/config/). --- ### Accessing your database
 with Prisma Client Python Just want to play around with Prisma Client Python
 and not worry about any setup? You can try it out online on [gitpod](https://
 gitpod.io/#https://github.com/RobertCraigie/prisma-py-async-quickstart). ####
 Installing Prisma Client Python The first step with any python project should
```

### Comparing `prisma-0.9.0/src/prisma.egg-info/SOURCES.txt` & `prisma-0.9.1/src/prisma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prisma-0.9.0/src/prisma_cleanup/_cleanup.py` & `prisma-0.9.1/src/prisma_cleanup/_cleanup.py`

 * *Files identical despite different names*

