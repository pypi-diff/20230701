# Comparing `tmp/swoop.db-2.0.0.tar.gz` & `tmp/swoop.db-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swoop.db-2.0.0.tar", last modified: Thu Jun 22 21:40:37 2023, max compression
+gzip compressed data, was "swoop.db-7.0.0.tar", last modified: Sat Jul  1 05:29:23 2023, max compression
```

## Comparing `swoop.db-2.0.0.tar` & `swoop.db-7.0.0.tar`

### file list

```diff
@@ -1,56 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:40:37.558473 swoop.db-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-22 21:40:19.000000 swoop.db-2.0.0/.env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:40:37.550473 swoop.db-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:40:37.554473 swoop.db-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-22 21:40:19.000000 swoop.db-2.0.0/.github/workflows/publish-image.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-22 21:40:19.000000 swoop.db-2.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-22 21:40:19.000000 swoop.db-2.0.0/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-22 21:40:19.000000 swoop.db-2.0.0/.github/workflows/snyk-scan.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-22 21:40:19.000000 swoop.db-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-22 21:40:19.000000 swoop.db-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-22 21:40:19.000000 swoop.db-2.0.0/.snyk
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-22 21:40:19.000000 swoop.db-2.0.0/.sqlfluff
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-22 21:40:19.000000 swoop.db-2.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-22 21:40:19.000000 swoop.db-2.0.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-22 21:40:19.000000 swoop.db-2.0.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-22 21:40:19.000000 swoop.db-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-22 21:40:37.558473 swoop.db-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-22 21:40:19.000000 swoop.db-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-22 21:40:19.000000 swoop.db-2.0.0/RELEASE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:40:37.554473 swoop.db-2.0.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-06-22 21:40:19.000000 swoop.db-2.0.0/bin/get-max-migration-version.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-22 21:40:19.000000 swoop.db-2.0.0/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-22 21:40:19.000000 swoop.db-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-22 21:40:19.000000 swoop.db-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 21:40:37.558473 swoop.db-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:40:37.554473 swoop.db-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:40:37.554473 swoop.db-2.0.0/src/swoop/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:40:37.554473 swoop.db-2.0.0/src/swoop/db/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-22 21:40:19.000000 swoop.db-2.0.0/src/swoop/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-22 21:40:19.000000 swoop.db-2.0.0/src/swoop/db/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-22 21:40:19.000000 swoop.db-2.0.0/src/swoop/db/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:40:37.558473 swoop.db-2.0.0/src/swoop/db/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-22 21:40:19.000000 swoop.db-2.0.0/src/swoop/db/fixtures/base_01.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:40:37.558473 swoop.db-2.0.0/src/swoop/db/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    15663 2023-06-22 21:40:19.000000 swoop.db-2.0.0/src/swoop/db/migrations/00000_base_schema.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-22 21:40:19.000000 swoop.db-2.0.0/src/swoop/db/migrations/00001_version.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-06-22 21:40:19.000000 swoop.db-2.0.0/src/swoop/db/migrations/00002_cache_func.down.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-22 21:40:19.000000 swoop.db-2.0.0/src/swoop/db/migrations/00002_cache_func.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:40:19.000000 swoop.db-2.0.0/src/swoop/db/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-06-22 21:40:19.000000 swoop.db-2.0.0/src/swoop/db/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:40:37.554473 swoop.db-2.0.0/src/swoop.db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-22 21:40:37.000000 swoop.db-2.0.0/src/swoop.db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-22 21:40:37.000000 swoop.db-2.0.0/src/swoop.db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 21:40:37.000000 swoop.db-2.0.0/src/swoop.db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-22 21:40:37.000000 swoop.db-2.0.0/src/swoop.db.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-22 21:40:37.000000 swoop.db-2.0.0/src/swoop.db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 21:40:37.000000 swoop.db-2.0.0/src/swoop.db.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:40:37.558473 swoop.db-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-06-22 21:40:19.000000 swoop.db-2.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:40:37.558473 swoop.db-2.0.0/tests/pgtap/
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-22 21:40:19.000000 swoop.db-2.0.0/tests/pgtap/test_action.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-06-22 21:40:19.000000 swoop.db-2.0.0/tests/pgtap/test_find_cached_action_for_payload.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-22 21:40:19.000000 swoop.db-2.0.0/tests/pgtap/test_item_inserts.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-22 21:40:19.000000 swoop.db-2.0.0/tests/pgtap/test_limit-locking.sql
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-22 21:40:19.000000 swoop.db-2.0.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-22 21:40:19.000000 swoop.db-2.0.0/tests/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:23.791331 swoop.db-7.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-01 05:29:07.000000 swoop.db-7.0.0/.env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:23.783331 swoop.db-7.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:23.787331 swoop.db-7.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-01 05:29:07.000000 swoop.db-7.0.0/.github/workflows/publish-image.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-01 05:29:07.000000 swoop.db-7.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-01 05:29:07.000000 swoop.db-7.0.0/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-01 05:29:07.000000 swoop.db-7.0.0/.github/workflows/snyk-scan.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-01 05:29:07.000000 swoop.db-7.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-01 05:29:07.000000 swoop.db-7.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-01 05:29:07.000000 swoop.db-7.0.0/.snyk
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-01 05:29:07.000000 swoop.db-7.0.0/.sqlfluff
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-01 05:29:07.000000 swoop.db-7.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-01 05:29:07.000000 swoop.db-7.0.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-01 05:29:07.000000 swoop.db-7.0.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-01 05:29:07.000000 swoop.db-7.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-01 05:29:23.791331 swoop.db-7.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-01 05:29:07.000000 swoop.db-7.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-01 05:29:07.000000 swoop.db-7.0.0/RELEASE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:23.787331 swoop.db-7.0.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-07-01 05:29:07.000000 swoop.db-7.0.0/bin/get-max-migration-version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-01 05:29:07.000000 swoop.db-7.0.0/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-01 05:29:07.000000 swoop.db-7.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-01 05:29:07.000000 swoop.db-7.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 05:29:23.791331 swoop.db-7.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:23.783331 swoop.db-7.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:23.783331 swoop.db-7.0.0/src/swoop/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:23.787331 swoop.db-7.0.0/src/swoop/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:23.787331 swoop.db-7.0.0/src/swoop/db/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/fixtures/base_01.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:23.787331 swoop.db-7.0.0/src/swoop/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    15663 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/migrations/00000_base_schema.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/migrations/00001_version.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/migrations/00002_cache_func.down.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/migrations/00002_cache_func.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/migrations/00003_remove_items.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/migrations/00004_update_thread.down.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/migrations/00004_update_thread.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/migrations/00005_handler_type.down.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/migrations/00005_handler_type.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/migrations/00006_workflow_constraint.down.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/migrations/00006_workflow_constraint.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/migrations/00007_change-uuid-formats.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16734 2023-07-01 05:29:07.000000 swoop.db-7.0.0/src/swoop/db/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:23.787331 swoop.db-7.0.0/src/swoop.db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-01 05:29:23.000000 swoop.db-7.0.0/src/swoop.db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-01 05:29:23.000000 swoop.db-7.0.0/src/swoop.db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 05:29:23.000000 swoop.db-7.0.0/src/swoop.db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-01 05:29:23.000000 swoop.db-7.0.0/src/swoop.db.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-01 05:29:23.000000 swoop.db-7.0.0/src/swoop.db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-01 05:29:23.000000 swoop.db-7.0.0/src/swoop.db.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:23.791331 swoop.db-7.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:23.783331 swoop.db-7.0.0/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:23.791331 swoop.db-7.0.0/tests/fixtures/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/fixtures/migrations/0_base_01.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/fixtures/migrations/1_result.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/fixtures/migrations/2_base_01.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/fixtures/migrations/2_result.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/fixtures/migrations/6_base_01.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/fixtures/migrations/6_result.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/fixtures/migrations/7_base_01.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/fixtures/migrations/7_result.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/fixtures/migrations/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:29:23.791331 swoop.db-7.0.0/tests/pgtap/
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/pgtap/test_action.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/pgtap/test_find_cached_action_for_payload.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/pgtap/test_limit-locking.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/pgtap/test_uuid_v7.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-01 05:29:07.000000 swoop.db-7.0.0/tests/test_migrations.py
```

### Comparing `swoop.db-2.0.0/.env` & `swoop.db-7.0.0/.env`

 * *Files identical despite different names*

### Comparing `swoop.db-2.0.0/.github/workflows/publish-image.yml` & `swoop.db-7.0.0/.github/workflows/publish-image.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-2.0.0/.github/workflows/python-publish.yml` & `swoop.db-7.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-2.0.0/.github/workflows/python-test.yml` & `swoop.db-7.0.0/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-2.0.0/.github/workflows/snyk-scan.yml` & `swoop.db-7.0.0/.github/workflows/snyk-scan.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-2.0.0/.gitignore` & `swoop.db-7.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `swoop.db-2.0.0/.pre-commit-config.yaml` & `swoop.db-7.0.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -71,7 +71,8 @@
         #  - `--processes 0` to use maximum parallelism
         # By default, this hook applies all rules.
         entry: sqlfluff fix --force --show-lint-violations --processes 0
         language: python
         description: "Fixes sql lint errors with `SQLFluff`"
         types: [sql]
         require_serial: true
+        exclude: ^tests/fixtures/migrations/
```

### Comparing `swoop.db-2.0.0/.snyk` & `swoop.db-7.0.0/.snyk`

 * *Files identical despite different names*

### Comparing `swoop.db-2.0.0/CONTRIBUTING.md` & `swoop.db-7.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `swoop.db-2.0.0/Dockerfile` & `swoop.db-7.0.0/Dockerfile`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # build python venv for inclusion into image
-FROM postgres:15-bullseye as APP
+FROM postgres:15 as APP
 RUN apt-get update && apt-get install -y git python3-venv
 WORKDIR /opt/swoop/db
 RUN python3 -m venv --copies swoop-db-venv
 COPY requirements.txt .
 RUN ./swoop-db-venv/bin/pip install -r requirements.txt
 RUN --mount=source=.git,target=.git,type=bind git clone . clone
 RUN ./swoop-db-venv/bin/pip install ./clone
@@ -23,13 +23,13 @@
     trap "rm -rf '$tmp'" EXIT && \
     cd "$tmp" && \
     curl -fsSL https://github.com/theory/pgtap/archive/refs/tags/v${PGTAP_VERSION}.tar.gz \
         -o pgtap.tar.gz && \
     tar -xzf pgtap.tar.gz --strip-components 1 && \
     make install
 
-ENV PGDATABASE: "${PGDATABASE:-swoop}" \
-    PGUSER: "${PGUSER:-postgres}"
+ENV PGDATABASE: "${PGDATABASE:-swoop}"
+ENV PGUSER: "${PGUSER:-postgres}"
 
 # copy the python venv into this output image and add it's bin to the path
 COPY --from=APP /opt/swoop/db/swoop-db-venv /opt/swoop/db/swoop-db-venv
 ENV PATH=/opt/swoop/db/swoop-db-venv/bin:$PATH
```

### Comparing `swoop.db-2.0.0/LICENSE` & `swoop.db-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swoop.db-2.0.0/PKG-INFO` & `swoop.db-7.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swoop.db
-Version: 2.0.0
+Version: 7.0.0
 Summary: Database for STAC Workflow Open Orchestration Framework
 Author-email: Jarrett Keifer <jkeifer@element84.com>
 License: Apache License 2.0
 Keywords: postgresql,sql,stac,workflow,geospatial
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `swoop.db-2.0.0/README.md` & `swoop.db-7.0.0/README.md`

 * *Files identical despite different names*

### Comparing `swoop.db-2.0.0/RELEASE.md` & `swoop.db-7.0.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `swoop.db-2.0.0/docker-compose.yml` & `swoop.db-7.0.0/docker-compose.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 version: '3.8'
 
 services:
   postgres:
-    build:
-      dockerfile: Dockerfile
+    build: .
     restart: always
     environment:
       POSTGRES_PASSWORD: "${PGPASSWORD:-password}"
       POSTGRES_USER: "${PGUSER:-postgres}"
       PGUSER: "${PGUSER:-postgres}"
       PGPASSWORD: "${PGPASSWORD:-password}"
       PGDATABASE: "${PGDATABASE:-swoop}"
```

### Comparing `swoop.db-2.0.0/pyproject.toml` & `swoop.db-7.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swoop.db-2.0.0/src/swoop/db/cli.py` & `swoop.db-7.0.0/src/swoop/db/cli.py`

 * *Files identical despite different names*

### Comparing `swoop.db-2.0.0/src/swoop/db/fixtures/base_01.sql` & `swoop.db-7.0.0/tests/fixtures/migrations/2_base_01.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-2.0.0/src/swoop/db/migrations/00000_base_schema.up.sql` & `swoop.db-7.0.0/src/swoop/db/migrations/00000_base_schema.up.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-2.0.0/src/swoop/db/migrations/00002_cache_func.down.sql` & `swoop.db-7.0.0/src/swoop/db/migrations/00002_cache_func.down.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-2.0.0/src/swoop/db/migrations/00002_cache_func.up.sql` & `swoop.db-7.0.0/src/swoop/db/migrations/00002_cache_func.up.sql`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,17 @@
 $$;
 
 
 -- Update check_cache function
 
 DROP FUNCTION IF EXISTS swoop.check_cache;
 
-CREATE FUNCTION swoop.find_cached_action_for_payload(plhash bytea, wf_version smallint)
+CREATE FUNCTION swoop.find_cached_action_for_payload(
+  plhash bytea, wf_version smallint
+)
 RETURNS uuid
 LANGUAGE plpgsql VOLATILE
 AS $$
 DECLARE
   v_status text;
   n_version smallint;
   d_invalid timestamptz;
```

### Comparing `swoop.db-2.0.0/src/swoop/db/schema.sql` & `swoop.db-7.0.0/src/swoop/db/schema.sql`

 * *Files 12% similar despite different names*

```diff
@@ -25,45 +25,143 @@
 (
   'RETRIES_EXHAUSTED',
   'Call did not fail within allowed time or number of retries'
 ),
 ('INFO', 'Event is informational and does not change thread state');
 
 
+-- gen_uuid_v7() modified from
+-- https://gist.github.com/kjmph/5bd772b2c2df145aa645b837da7eca74
+--
+-- Original license:
+--
+-- Copyright 2023 Kyle Hubert <kjmph@users.noreply.github.com>
+-- (https://github.com/kjmph)
+--
+-- Permission is hereby granted, free of charge, to any person obtaining a copy
+-- of this software and associated documentation files (the “Software”), to
+-- deal in the Software without restriction, including without limitation the
+-- rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
+-- sell copies of the Software, and to permit persons to whom the Software is
+-- furnished to do so, subject to the following conditions:
+--
+-- The above copyright notice and this permission notice shall be included in
+-- all copies or substantial portions of the Software.
+--
+-- THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+-- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+-- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+-- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+-- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+-- FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
+-- IN THE SOFTWARE.
+CREATE FUNCTION public.gen_uuid_v7(_timestamp timestamptz)
+RETURNS uuid
+LANGUAGE plpgsql VOLATILE
+AS $$
+DECLARE
+  _unix_ts_ms bytea;
+  _uuid_bytes bytea;
+BEGIN
+  _unix_ts_ms = substring(
+    int8send(floor(extract(epoch from _timestamp) * 1000)::bigint) from 3
+  );
+
+  -- use random v4 uuid as starting point (which has the same variant we need)
+  _uuid_bytes = uuid_send(gen_random_uuid());
+
+  -- overlay timestamp
+  _uuid_bytes = overlay(_uuid_bytes PLACING _unix_ts_ms FROM 1 FOR 6);
+
+  -- set version 7
+  _uuid_bytes = set_byte(
+    _uuid_bytes,
+    6,
+    (b'0111' || get_byte(_uuid_bytes, 6)::bit(4))::bit(8)::int
+  );
+
+  RETURN encode(_uuid_bytes, 'hex')::uuid;
+END;
+$$;
+
+
+CREATE FUNCTION public.uuid_version(_uuid_bytes bytea)
+RETURNS integer
+LANGUAGE sql IMMUTABLE PARALLEL SAFE STRICT LEAKPROOF
+AS $$
+  SELECT get_byte(_uuid_bytes, 6)::bit(8)::bit(4)::int;
+$$;
+
+
+CREATE FUNCTION public.uuid_version(_uuid uuid)
+RETURNS integer
+LANGUAGE sql IMMUTABLE PARALLEL SAFE STRICT LEAKPROOF
+AS $$
+  SELECT uuid_version(uuid_send(_uuid));
+$$;
+
+
+CREATE FUNCTION public.timestamp_from_uuid_v7(_uuid uuid)
+RETURNS timestamptz
+LANGUAGE plpgsql IMMUTABLE PARALLEL SAFE STRICT LEAKPROOF
+AS $$
+DECLARE
+  _uuid_version integer;
+  _uuid_bytes bytea;
+BEGIN
+  SELECT uuid_send(_uuid) INTO _uuid_bytes;
+  SELECT uuid_version(_uuid_bytes) INTO _uuid_version;
+
+  IF _uuid_version != 7 THEN
+    RAISE EXCEPTION 'UUID must be version 7, not %', _uuid_version
+      USING HINT = 'You can only call this function with a UUID v7 input';
+  END IF;
+
+  RETURN to_timestamp(('x0000' || encode(
+    substring(_uuid_bytes FOR 4) || substring(_uuid_bytes FROM 5 FOR 2),
+    'hex'
+  ))::bit(64)::bigint::numeric / 1000);
+END;
+$$;
+
+
 CREATE TABLE swoop.payload_cache (
-  payload_uuid uuid DEFAULT gen_random_uuid() PRIMARY KEY,
-  payload_hash bytea UNIQUE,
+  payload_uuid uuid PRIMARY KEY CHECK (uuid_version(payload_uuid) = 5),
   workflow_name text NOT NULL,
   created_at timestamptz NOT NULL DEFAULT now(),
   invalid_after timestamptz
 );
 
-CREATE INDEX ON swoop.payload_cache (payload_hash);
-
 
 CREATE TABLE swoop.action (
-  action_uuid uuid NOT NULL DEFAULT gen_random_uuid(),
+  action_uuid uuid NOT NULL DEFAULT gen_uuid_v7(now()),
   action_type text NOT NULL CHECK (action_type IN ('callback', 'workflow')),
   action_name text,
   handler_name text NOT NULL,
   parent_uuid uuid, -- reference omitted, we don't need referential integrity
   created_at timestamptz NOT NULL DEFAULT now(),
   priority smallint DEFAULT 100,
   payload_uuid uuid REFERENCES swoop.payload_cache ON DELETE RESTRICT,
   workflow_version smallint NOT NULL,
+  handler_type text NOT NULL,
+
+  CONSTRAINT uuid_timestamp_matches_created_at CHECK (
+    timestamp_from_uuid_v7(action_uuid) = date_trunc('ms', created_at)
+  ),
 
   CONSTRAINT workflow_or_callback CHECK (
     CASE
       WHEN action_type = 'callback'
         THEN
           parent_uuid IS NOT NULL
           AND payload_uuid IS NULL
       WHEN action_type = 'workflow' THEN
         action_name IS NOT NULL
         AND payload_uuid IS NOT NULL
+        AND parent_uuid IS NULL
     END
   )
 ) PARTITION BY RANGE (created_at);
 
 CREATE INDEX ON swoop.action (created_at);
 CREATE INDEX ON swoop.action (action_uuid);
 CREATE INDEX ON swoop.action (handler_name);
@@ -107,15 +205,17 @@
   --   swoop.lock_thread(thread.lock_id)
   --   swoop.unlock_thread(thread.lock_id)
   lock_id integer GENERATED ALWAYS AS IDENTITY (
     SEQUENCE NAME swoop.thread_lock_id_seq
     MINVALUE -2147483648
     START WITH 1
     CYCLE
-  )
+  ),
+  started_at timestamptz
+
 ) PARTITION BY RANGE (created_at);
 
 CREATE INDEX ON swoop.thread (created_at);
 CREATE INDEX ON swoop.thread (action_uuid);
 CREATE INDEX ON swoop.thread (status);
 CREATE INDEX ON swoop.thread (handler_name);
 CREATE TABLE swoop.thread_template (LIKE swoop.thread);
@@ -152,30 +252,14 @@
   'event_time',
   'native',
   'monthly',
   p_template_table => 'swoop.event_template'
 );
 
 
-CREATE TABLE swoop.input_item (
-  item_uuid uuid PRIMARY KEY DEFAULT gen_random_uuid(),
-  item_id text NOT NULL,
-  collection text,
-  UNIQUE NULLS NOT DISTINCT (item_id, collection)
-);
-
-CREATE TABLE swoop.item_payload (
-  item_uuid uuid REFERENCES swoop.input_item ON DELETE RESTRICT,
-  payload_uuid uuid REFERENCES swoop.payload_cache ON DELETE CASCADE,
-  PRIMARY KEY (item_uuid, payload_uuid)
-);
-
-CREATE INDEX ON swoop.item_payload (item_uuid);
-
-
 CREATE FUNCTION swoop.add_pending_event()
 RETURNS trigger
 LANGUAGE plpgsql VOLATILE
 AS $$
 DECLARE
 BEGIN
   INSERT INTO swoop.event (event_time, action_uuid, status, event_source) VALUES
@@ -222,34 +306,44 @@
 CREATE FUNCTION swoop.update_thread()
 RETURNS trigger
 LANGUAGE plpgsql VOLATILE
 AS $$
 DECLARE
   _latest timestamptz;
   _next_attempt timestamptz;
+  _started timestamptz;
 BEGIN
-  SELECT last_update FROM swoop.thread WHERE action_uuid = NEW.action_uuid INTO _latest;
+  SELECT last_update, started_at FROM swoop.thread WHERE action_uuid = NEW.action_uuid
+    INTO _latest, _started;
 
   -- If the event time is older than the last update we don't update the thread
   -- (we can't use a trigger condition to filter this because we don't know the
   -- last update time from the event alone).
   IF _latest IS NOT NULL AND NEW.event_time < _latest THEN
+    IF NEW.status = 'RUNNING' THEN
+        UPDATE swoop.thread as t SET started_at = NEW.event_time WHERE t.action_uuid = NEW.action_uuid;
+    END IF;
     RETURN NULL;
   END IF;
 
   -- If we need a next attempt time let's calculate it
   IF NEW.retry_seconds IS NOT NULL THEN
     SELECT NEW.event_time + (NEW.retry_seconds * interval '1 second') INTO _next_attempt;
   END IF;
 
+  IF _started IS NULL AND NEW.status = 'RUNNING' THEN
+    SELECT  NEW.event_time INTO _started;
+  END IF;
+
   UPDATE swoop.thread as t SET
     last_update = NEW.event_time,
     status = NEW.status,
     next_attempt_after = _next_attempt,
-    error = NEW.error
+    error = NEW.error,
+    started_at = _started
   WHERE
     t.action_uuid = NEW.action_uuid;
 
   -- We _could_ try to drop the thread lock here, which would be nice for
   -- swoop-conductor so it didn't have to explicitly unlock, but the unlock
   -- function raises a warning. Being explicit isn't the worst thing either,
   -- given the complications with possible relocking and the need for clients
@@ -423,15 +517,19 @@
 BEGIN
   RETURN (
     SELECT pg_advisory_unlock(to_regclass('swoop.thread')::oid::integer, _lock_id)
   );
 END;
 $$;
 
-CREATE FUNCTION swoop.find_cached_action_for_payload(plhash bytea, wf_version smallint)
+
+CREATE FUNCTION swoop.find_cached_action_for_payload(
+  _payload_uuid uuid,
+  _wf_version smallint
+)
 RETURNS uuid
 LANGUAGE plpgsql VOLATILE
 AS $$
 DECLARE
   v_status text;
   n_version smallint;
   d_invalid timestamptz;
@@ -440,22 +538,22 @@
   SELECT t.status, a.workflow_version, p.invalid_after, a.action_uuid
   INTO v_status, n_version, d_invalid, v_action_id
   FROM swoop.payload_cache p
   INNER JOIN swoop.action a
   USING (payload_uuid)
   INNER JOIN swoop.thread t
   USING (action_uuid)
-  WHERE p.payload_hash = plhash
+  WHERE p.payload_uuid = _payload_uuid
   ORDER BY t.created_at DESC
   LIMIT 1;
 
   IF v_status IN ('RUNNING', 'PENDING', 'QUEUED', 'BACKOFF') THEN
   -- Redirect to job details for that workflow, and do not process
     RETURN v_action_id;
-  ELSIF wf_version > n_version THEN
+  ELSIF _wf_version > n_version THEN
     RETURN null;
   ELSIF d_invalid IS NOT NULL and d_invalid < now() THEN
     RETURN null;
   ELSIF v_status IN ('SUCCESSFUL', 'INVALID') THEN
     RETURN v_action_id;
   ELSE
     RETURN null;
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `swoop.db-2.0.0/src/swoop.db.egg-info/PKG-INFO` & `swoop.db-7.0.0/src/swoop.db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swoop.db
-Version: 2.0.0
+Version: 7.0.0
 Summary: Database for STAC Workflow Open Orchestration Framework
 Author-email: Jarrett Keifer <jkeifer@element84.com>
 License: Apache License 2.0
 Keywords: postgresql,sql,stac,workflow,geospatial
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `swoop.db-2.0.0/tests/conftest.py` & `swoop.db-7.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swoop.db-2.0.0/tests/pgtap/test_find_cached_action_for_payload.sql` & `swoop.db-7.0.0/tests/pgtap/test_find_cached_action_for_payload.sql`

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,63 @@
 BEGIN;
 SET search_path = tap, public;
 SELECT plan(7);
 
 SELECT results_eq(
   $$
-    SELECT swoop.find_cached_action_for_payload(convert_to('hash_test', 'utf-8'), 1::smallint)
+    SELECT swoop.find_cached_action_for_payload(gen_random_uuid(), 1::smallint)
   $$,
   $$
     VALUES (
       null::uuid
     )
   $$,
   'return null for payload that does not have a cache entry'
 );
 
 
 INSERT INTO swoop.payload_cache (
   payload_uuid,
-  payload_hash,
   workflow_name
 ) VALUES (
-  'e8d87aa6-6c42-47ed-a33c-94498fb2c20e',
-  convert_to('hash1', 'utf-8'),
+  'e8d87aa6-6c42-57ed-a33c-94498fb2c20e',
   'mirror'
 );
 
 INSERT INTO swoop.payload_cache (
   payload_uuid,
-  payload_hash,
   workflow_name
 ) VALUES (
-  'b262902b-b968-4cad-aabc-8f26f3d048e2',
-  convert_to('hash2', 'utf-8'),
+  'b262902b-b968-5cad-aabc-8f26f3d048e2',
   'mirror'
 );
 
 INSERT INTO swoop.payload_cache (
   payload_uuid,
-  payload_hash,
   workflow_name
 ) VALUES (
-  'd5d64165-82df-4836-b78e-af4daee55d38',
-  convert_to('hash3', 'utf-8'),
+  'd5d64165-82df-5836-b78e-af4daee55d38',
   'cirrus'
 );
 
 INSERT INTO swoop.payload_cache (
   payload_uuid,
-  payload_hash,
   workflow_name
 ) VALUES (
-  '737490d3-fba6-4236-af35-ec6ef9d25ec8',
-  convert_to('hash4', 'utf-8'),
+  '737490d3-fba6-5236-af35-ec6ef9d25ec8',
   'mirror'
 );
 
 
 SELECT results_eq(
   $$
-    SELECT swoop.find_cached_action_for_payload(convert_to('hash1', 'utf-8'), 2::smallint)
+    SELECT swoop.find_cached_action_for_payload(
+      'e8d87aa6-6c42-57ed-a33c-94498fb2c20e'::uuid,
+      2::smallint
+    )
   $$,
   $$
     VALUES (
       null::uuid
     )
   $$,
   'return null for payload that has cache but no action entry.'
@@ -70,106 +65,117 @@
 
 
 INSERT INTO swoop.action (
   action_uuid,
   action_type,
   action_name,
   handler_name,
+  handler_type,
   parent_uuid,
   created_at,
   priority,
   payload_uuid,
   workflow_version
 ) VALUES (
-  '2595f2da-81a6-423c-84db-935e6791046e',
+  '0187c88d-a9e0-757e-aa36-2fbb6c834cb5',
   'workflow',
   'action_1',
   'handler_foo',
-  'cf8ff7f0-ce5d-4de6-8026-4e551787385f',
+  'argo-workflow',
+  null,
   '2023-04-28 15:49:00+00',
   100,
-  'e8d87aa6-6c42-47ed-a33c-94498fb2c20e',
+  'e8d87aa6-6c42-57ed-a33c-94498fb2c20e',
   1
 );
 
 INSERT INTO swoop.action (
   action_uuid,
   action_type,
   action_name,
   handler_name,
+  handler_type,
   parent_uuid,
   created_at,
   priority,
   payload_uuid,
   workflow_version
 )
 VALUES (
-  '71ba4b00-245e-4189-9ee8-0016a3ac274d',
+  '0187c893-2820-77b1-a7b2-f29206b702ae',
   'workflow',
   'action_2',
   'handler_foo',
-  '04001ac8-2cae-4536-8ae7-bf0c55897594',
+  'argo-workflow',
+  null,
   '2023-04-28 15:55:00+00',
   100,
-  'e8d87aa6-6c42-47ed-a33c-94498fb2c20e',
+  'e8d87aa6-6c42-57ed-a33c-94498fb2c20e',
   2
 );
 
 INSERT INTO swoop.action (
   action_uuid,
   action_type,
   action_name,
   handler_name,
+  handler_type,
   parent_uuid,
   created_at,
   priority,
   payload_uuid,
   workflow_version
 ) VALUES (
-  '81842304-0aa9-4609-89f0-1c86819b0752',
+  '0187c895-e740-7a17-9757-1d82de96c033',
   'workflow',
   'action_3',
   'handler_foo',
-  'c11e2bb6-4e22-427c-bc05-e709c98bbf41',
+  'argo-workflow',
+  null,
   '2023-04-28 15:58:00+00',
   100,
-  'e8d87aa6-6c42-47ed-a33c-94498fb2c20e',
+  'e8d87aa6-6c42-57ed-a33c-94498fb2c20e',
   3
 );
 
 INSERT INTO swoop.action (
   action_uuid,
   action_type,
   action_name,
   handler_name,
+  handler_type,
   parent_uuid,
   created_at,
   priority,
   payload_uuid,
   workflow_version
 ) VALUES (
-  '7716319b-5064-41fc-be04-0e1330c0c290',
+  '0187d2e2-9f40-7824-9392-fc2c6abc799a',
   'workflow',
   'action_1',
   'handler_foo',
-  '8606e6d4-0f43-43d3-be7a-6966869a4735',
+  'cirrus-workflow',
+  null,
   '2023-04-30 15:58:00+00',
   100,
-  '737490d3-fba6-4236-af35-ec6ef9d25ec8',
+  '737490d3-fba6-5236-af35-ec6ef9d25ec8',
   3
 );
 
 
 DELETE FROM swoop.thread
-WHERE action_uuid = '7716319b-5064-41fc-be04-0e1330c0c290';
+WHERE action_uuid = '0187d2e2-9f40-7824-9392-fc2c6abc799a';
 
 
 SELECT results_eq(
   $$
-    SELECT swoop.find_cached_action_for_payload(convert_to('hash4', 'utf-8'), 2::smallint)
+    SELECT swoop.find_cached_action_for_payload(
+      '737490d3-fba6-5236-af35-ec6ef9d25ec8'::uuid,
+      2::smallint
+    )
   $$,
   $$
     VALUES (
       null::uuid
     )
   $$,
   'return null for payload that has cache and action entry but no thread'
@@ -184,15 +190,15 @@
   priority,
   status,
   next_attempt_after,
   error
 ) VALUES (
   '2023-04-28 15:49:00+00',
   '2023-04-28 15:49:00+00',
-  '2595f2da-81a6-423c-84db-935e6791046e',
+  '0187c88d-a9e0-757e-aa36-2fbb6c834cb5',
   'handler_foo',
   100,
   'PENDING',
   null,
   null
 );
 
@@ -204,15 +210,15 @@
   priority,
   status,
   next_attempt_after,
   error
 ) VALUES (
   '2023-04-28 15:55:00+00',
   '2023-04-28 15:55:00+00',
-  '71ba4b00-245e-4189-9ee8-0016a3ac274d',
+  '0187c893-2820-77b1-a7b2-f29206b702ae',
   'handler_foo',
   100,
   'PENDING',
   null,
   null
 );
 
@@ -224,15 +230,15 @@
   priority,
   status,
   next_attempt_after,
   error
 ) VALUES (
   '2023-04-28 15:58:00+00',
   '2023-04-28 15:58:00+00',
-  '81842304-0aa9-4609-89f0-1c86819b0752',
+  '0187c895-e740-7a17-9757-1d82de96c033',
   'handler_foo',
   100,
   'SUCCESSFUL',
   null,
   null
 );
 
@@ -244,52 +250,61 @@
   priority,
   status,
   next_attempt_after,
   error
 ) VALUES (
   '2023-04-30 15:58:00+00',
   '2023-04-30 15:58:00+00',
-  '7716319b-5064-41fc-be04-0e1330c0c290',
+  '0187d2e2-9f40-7824-9392-fc2c6abc799a',
   'handler_foo',
   100,
   'PENDING',
   null,
   null
 );
 
 
 SELECT results_eq(
   $$
-    SELECT swoop.find_cached_action_for_payload(convert_to('hash1', 'utf-8'), 2::smallint)
+    SELECT swoop.find_cached_action_for_payload(
+      'e8d87aa6-6c42-57ed-a33c-94498fb2c20e'::uuid,
+      2::smallint
+    )
   $$,
   $$
     VALUES (
-      '81842304-0aa9-4609-89f0-1c86819b0752'::uuid
+      '0187c895-e740-7a17-9757-1d82de96c033'::uuid
     )
   $$,
   'return action_uuid when cache, action, thread entries exist and PENDING.'
 );
 
 
 SELECT results_eq(
   $$
-    SELECT swoop.find_cached_action_for_payload(convert_to('hash1', 'utf-8'), 3::smallint)
+    SELECT swoop.find_cached_action_for_payload(
+      'e8d87aa6-6c42-57ed-a33c-94498fb2c20e'::uuid,
+      3::smallint
+    )
   $$,
   $$
     VALUES (
-      '81842304-0aa9-4609-89f0-1c86819b0752'::uuid
+      '0187c895-e740-7a17-9757-1d82de96c033'::uuid
     )
   $$,
   'return action_uuid when cache, action, thread entries exist and SUCCESSFUL.'
 );
 
 
 SELECT results_eq(
   $$
-    SELECT swoop.find_cached_action_for_payload(convert_to('hash1', 'utf-8'), 4::smallint)
+    SELECT swoop.find_cached_action_for_payload(
+      'e8d87aa6-6c42-57ed-a33c-94498fb2c20e'::uuid,
+      4::smallint
+    )
   $$,
   $$
     VALUES (
       null::uuid
     )
   $$,
   'return null when workflow_version is greater than what is in database.'
@@ -298,21 +313,24 @@
 
 /* Set invalid_after to an arbitrary date in the past for
  a payload_uuid, and set the corresponding thread for the action
 associated with that payload_uuid to a FAILED state
 */
 
 UPDATE swoop.payload_cache SET invalid_after = '2000-01-01 00:00:00+00'
-WHERE payload_uuid = 'e8d87aa6-6c42-47ed-a33c-94498fb2c20e';
+WHERE payload_uuid = 'e8d87aa6-6c42-57ed-a33c-94498fb2c20e';
 UPDATE swoop.thread SET status = 'FAILED'
-WHERE action_uuid = '81842304-0aa9-4609-89f0-1c86819b0752';
+WHERE action_uuid = '0187c895-e740-7a17-9757-1d82de96c033';
 
 SELECT results_eq(
   $$
-    SELECT swoop.find_cached_action_for_payload(convert_to('hash1', 'utf-8'), 3::smallint)
+    SELECT swoop.find_cached_action_for_payload(
+      'e8d87aa6-6c42-57ed-a33c-94498fb2c20e'::uuid,
+      3::smallint
+    )
   $$,
   $$
     VALUES (
       null::uuid
     )
   $$,
   'return null when invalid_after is not null and greater than current date.'
```

### Comparing `swoop.db-2.0.0/tests/pgtap/test_limit-locking.sql` & `swoop.db-7.0.0/tests/pgtap/test_limit-locking.sql`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,41 @@
 BEGIN;
 
 SET search_path = tap, public;
 SELECT plan(3);
 
 INSERT INTO swoop.payload_cache (
   payload_uuid,
-  payload_hash,
   workflow_name,
   created_at,
   invalid_after
 ) VALUES (
-  'cdc73916-500c-4501-a658-dd706a943d19'::uuid,
-  decode('123\000456', 'escape'),
+  'cdc73916-500c-5501-a658-dd706a943d19'::uuid,
   'workflow-a',
   '2023-04-14 00:25:07.388012+00'::timestamptz,
   '2023-04-20 00:25:07.388012+00'::timestamptz
 );
 
 DO
 $$
 BEGIN
   FOR i in 1..300 LOOP
     INSERT INTO swoop.action (
-      action_uuid,
       action_type,
       handler_name,
+      handler_type,
       action_name,
-      created_at,
       payload_uuid,
       workflow_version
     ) VALUES (
-      gen_random_uuid(),
       'workflow',
+      'argo-handler',
       'argo-workflow',
       'workflow-a',
-      now(),
-      'cdc73916-500c-4501-a658-dd706a943d19'::uuid,
+      'cdc73916-500c-5501-a658-dd706a943d19'::uuid,
       1
     );
   END LOOP;
 END;
 $$;
 
 SELECT
```

### Comparing `swoop.db-2.0.0/tests/test_database.py` & `swoop.db-7.0.0/tests/test_database.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 async def test_verify(pg_dump) -> None:
     assert await SwoopDB().verify(pg_dump=pg_dump)
 
 
 @pytest.mark.asyncio
 async def test_load_fixture() -> None:
     DB_NAME = "swoop_db_load_fixture"
+    test_db = SwoopDB()
     try:
-        test_db = SwoopDB()
         await test_db.create_database(DB_NAME)
         await test_db.load_schema(database=DB_NAME)
         await test_db.load_fixture("base_01", database=DB_NAME)
+    finally:
         await test_db.drop_database(DB_NAME)
-    except Exception as exc:
-        assert False, f"Fixture could not be applied to database: {exc}"
+    assert True
```

