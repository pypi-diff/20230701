# Comparing `tmp/flook-0.3.7.tar.gz` & `tmp/flook-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flook-0.3.7.tar", last modified: Sat Jul  1 18:27:46 2023, max compression
+gzip compressed data, was "flook-0.4.0.tar", last modified: Sat Jul  1 21:05:32 2023, max compression
```

## Comparing `flook-0.3.7.tar` & `flook-0.4.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:27:46.620278 flook-0.3.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:27:46.616278 flook-0.3.7/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-01 18:27:27.000000 flook-0.3.7/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-01 18:27:27.000000 flook-0.3.7/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:27:46.616278 flook-0.3.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-01 18:27:27.000000 flook-0.3.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-01 18:27:27.000000 flook-0.3.7/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:27:46.616278 flook-0.3.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-01 18:27:27.000000 flook-0.3.7/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-01 18:27:27.000000 flook-0.3.7/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-01 18:27:27.000000 flook-0.3.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-01 18:27:27.000000 flook-0.3.7/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-01 18:27:27.000000 flook-0.3.7/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-01 18:27:27.000000 flook-0.3.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-01 18:27:27.000000 flook-0.3.7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-01 18:27:27.000000 flook-0.3.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-01 18:27:27.000000 flook-0.3.7/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-01 18:27:46.620278 flook-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-01 18:27:27.000000 flook-0.3.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:27:46.616278 flook-0.3.7/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-01 18:27:27.000000 flook-0.3.7/cache/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-01 18:27:27.000000 flook-0.3.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:27:46.612278 flook-0.3.7/recipe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:27:46.616278 flook-0.3.7/recipe/motd/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-01 18:27:27.000000 flook-0.3.7/recipe/motd/motd.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-01 18:27:27.000000 flook-0.3.7/recipe/motd/recipe.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:27:46.616278 flook-0.3.7/recipe/nginx/
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-01 18:27:27.000000 flook-0.3.7/recipe/nginx/recipe.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:27:46.616278 flook-0.3.7/recipe/ping/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-01 18:27:27.000000 flook-0.3.7/recipe/ping/recipe.yml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 18:27:27.000000 flook-0.3.7/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-01 18:27:46.620278 flook-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-01 18:27:27.000000 flook-0.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:27:46.612278 flook-0.3.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:27:46.616278 flook-0.3.7/src/flook/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-01 18:27:27.000000 flook-0.3.7/src/flook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-07-01 18:27:27.000000 flook-0.3.7/src/flook/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:27:46.620278 flook-0.3.7/src/flook/command/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-01 18:27:27.000000 flook-0.3.7/src/flook/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-01 18:27:27.000000 flook-0.3.7/src/flook/command/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-01 18:27:27.000000 flook-0.3.7/src/flook/command/hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-07-01 18:27:27.000000 flook-0.3.7/src/flook/command/recipes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:27:46.620278 flook-0.3.7/src/flook/exception/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-01 18:27:27.000000 flook-0.3.7/src/flook/exception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:27:46.620278 flook-0.3.7/src/flook/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-01 18:27:27.000000 flook-0.3.7/src/flook/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-01 18:27:27.000000 flook-0.3.7/src/flook/model/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-01 18:27:27.000000 flook-0.3.7/src/flook/model/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-01 18:27:27.000000 flook-0.3.7/src/flook/model/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:27:46.620278 flook-0.3.7/src/flook/module/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-01 18:27:27.000000 flook-0.3.7/src/flook/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-01 18:27:27.000000 flook-0.3.7/src/flook/module/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-07-01 18:27:27.000000 flook-0.3.7/src/flook/module/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-01 18:27:27.000000 flook-0.3.7/src/flook/module/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-01 18:27:27.000000 flook-0.3.7/src/flook/module/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-01 18:27:27.000000 flook-0.3.7/src/flook/module/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-01 18:27:27.000000 flook-0.3.7/src/flook/module/playbook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:27:46.616278 flook-0.3.7/src/flook.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-01 18:27:46.000000 flook-0.3.7/src/flook.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-01 18:27:46.000000 flook-0.3.7/src/flook.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 18:27:46.000000 flook-0.3.7/src/flook.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 18:27:46.000000 flook-0.3.7/src/flook.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 18:27:46.000000 flook-0.3.7/src/flook.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-01 18:27:46.000000 flook-0.3.7/src/flook.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-01 18:27:46.000000 flook-0.3.7/src/flook.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:27:46.620278 flook-0.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-01 18:27:27.000000 flook-0.3.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:27:46.620278 flook-0.3.7/tests/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 18:27:27.000000 flook-0.3.7/tests/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-01 18:27:27.000000 flook-0.3.7/tests/module/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-01 18:27:27.000000 flook-0.3.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.229853 flook-0.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-01 21:05:10.000000 flook-0.4.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-01 21:05:10.000000 flook-0.4.0/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-01 21:05:10.000000 flook-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-01 21:05:10.000000 flook-0.4.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-01 21:05:10.000000 flook-0.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-01 21:05:10.000000 flook-0.4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-01 21:05:10.000000 flook-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-01 21:05:10.000000 flook-0.4.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-01 21:05:10.000000 flook-0.4.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-01 21:05:10.000000 flook-0.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-01 21:05:10.000000 flook-0.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-01 21:05:10.000000 flook-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-01 21:05:10.000000 flook-0.4.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-01 21:05:32.233853 flook-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-01 21:05:10.000000 flook-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-01 21:05:10.000000 flook-0.4.0/cache/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-01 21:05:10.000000 flook-0.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.229853 flook-0.4.0/recipe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/recipe/motd/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-01 21:05:10.000000 flook-0.4.0/recipe/motd/motd.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-01 21:05:10.000000 flook-0.4.0/recipe/motd/recipe.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/recipe/nginx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-01 21:05:10.000000 flook-0.4.0/recipe/nginx/recipe.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/recipe/ping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-01 21:05:10.000000 flook-0.4.0/recipe/ping/recipe.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 21:05:10.000000 flook-0.4.0/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-01 21:05:32.237853 flook-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-01 21:05:10.000000 flook-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.229853 flook-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/src/flook/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/src/flook/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/command/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/command/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/command/recipes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/src/flook/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/exception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/src/flook/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/model/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/model/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/model/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/src/flook/module/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/module/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/module/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/module/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/module/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/module/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-01 21:05:10.000000 flook-0.4.0/src/flook/module/playbook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/src/flook.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-01 21:05:32.000000 flook-0.4.0/src/flook.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-01 21:05:32.000000 flook-0.4.0/src/flook.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 21:05:32.000000 flook-0.4.0/src/flook.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 21:05:32.000000 flook-0.4.0/src/flook.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 21:05:31.000000 flook-0.4.0/src/flook.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-01 21:05:32.000000 flook-0.4.0/src/flook.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-01 21:05:32.000000 flook-0.4.0/src/flook.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-01 21:05:10.000000 flook-0.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:32.233853 flook-0.4.0/tests/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 21:05:10.000000 flook-0.4.0/tests/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-01 21:05:10.000000 flook-0.4.0/tests/module/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-01 21:05:10.000000 flook-0.4.0/tox.ini
```

### Comparing `flook-0.3.7/.github/workflows/release.yml` & `flook-0.4.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/.gitignore` & `flook-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/CHANGELOG.rst` & `flook-0.4.0/CHANGELOG.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+Version 0.4.0
+=============
+
+- Fix issue.
+
 Version 0.3.7
 =============
 
 - Fix issue.
 
 Version 0.3.6
 =============
```

### Comparing `flook-0.3.7/CODE_OF_CONDUCT.md` & `flook-0.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/CONTRIBUTING.rst` & `flook-0.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/LICENSE.txt` & `flook-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/Makefile` & `flook-0.4.0/Makefile`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/PKG-INFO` & `flook-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flook
-Version: 0.3.7
+Version: 0.4.0
 Summary: A Lightweight and Flexible Ansible Command Line Tool.
 Home-page: https://github.com/norwik/flook/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/norwik/flook/
 Project-URL: Source, https://github.com/norwik/flook/
@@ -133,22 +133,29 @@
 12. To get a host
 
 .. code-block::
 
     $ flook host get <host_name>
 
 
-13. To delete a host
+13. To SSH into a host
+
+.. code-block::
+
+    $ flook host ssh <host_name>
+
+
+14. To delete a host
 
 .. code-block::
 
     $ flook host delete <host_name>
 
 
-14. Run a recipe towards a host
+15. Run a recipe towards a host
 
 .. code-block::
 
     $ flook recipe run <recipe_name> -h <host_name>
 
     # Some examples
     $ flook recipe run clivern/nginx -h example.com
```

### Comparing `flook-0.3.7/README.rst` & `flook-0.4.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -113,22 +113,29 @@
 12. To get a host
 
 .. code-block::
 
     $ flook host get <host_name>
 
 
-13. To delete a host
+13. To SSH into a host
+
+.. code-block::
+
+    $ flook host ssh <host_name>
+
+
+14. To delete a host
 
 .. code-block::
 
     $ flook host delete <host_name>
 
 
-14. Run a recipe towards a host
+15. Run a recipe towards a host
 
 .. code-block::
 
     $ flook recipe run <recipe_name> -h <host_name>
 
     # Some examples
     $ flook recipe run clivern/nginx -h example.com
```

### Comparing `flook-0.3.7/recipe/motd/recipe.yml` & `flook-0.4.0/recipe/motd/recipe.yml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 
 vars:
-  version: v0.3
+  version: v0.4
 
 templates:
   motd.j2: motd.j2
 
 tasks:
   - name: check mandatory variables
     assert:
```

### Comparing `flook-0.3.7/recipe/nginx/recipe.yml` & `flook-0.4.0/recipe/nginx/recipe.yml`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/recipe/ping/recipe.yml` & `flook-0.4.0/recipe/ping/recipe.yml`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/setup.cfg` & `flook-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/setup.py` & `flook-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/src/flook/__init__.py` & `flook-0.4.0/src/flook/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/src/flook/cli.py` & `flook-0.4.0/src/flook/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,21 @@
 @click.option(
     "-o", "--output", "output", type=click.STRING, default="", help="Output format"
 )
 def get(name, output):
     return Hosts().init().get(name, output)
 
 
+# SSH to a host sub command
+@host.command(help="SSH to a host")
+@click.argument("name")
+def ssh(name):
+    return Hosts().init().ssh(name)
+
+
 # Delete host sub command
 @host.command(help="Delete a host")
 @click.argument("name")
 def delete(name):
     return Hosts().init().delete(name)
 
 
@@ -159,17 +166,15 @@
 )
 @click.option("-t", "--tags", "tags", type=click.STRING, default="", help="Recipe tags")
 @click.option("-f", "--force", "force", is_flag=True, default=False, help="Force add")
 def add(name, path, tags, force):
     return (
         Recipes()
         .init()
-        .add(
-            name, {"path": path, "tags": tags.split(",") if tags != "" else []}, force
-        )
+        .add(name, {"path": path, "tags": tags.split(",") if tags != "" else []}, force)
     )
 
 
 # List recipes sub command
 @recipe.command(help="List all recipes")
 @click.option("-t", "--tag", "tag", type=click.STRING, default="", help="Recipe tag")
 @click.option(
```

### Comparing `flook-0.3.7/src/flook/command/__init__.py` & `flook-0.4.0/src/flook/command/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/src/flook/command/configs.py` & `flook-0.4.0/src/flook/command/configs.py`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/src/flook/command/hosts.py` & `flook-0.4.0/src/flook/command/hosts.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,29 +17,32 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import click
+import subprocess
 
 from flook.model.host import Host
 from flook.module.logger import Logger
 from flook.module.database import Database
 from flook.module.output import Output
 from flook.module.config import Config
+from flook.module.file_system import FileSystem
 
 
 class Hosts:
     """Hosts Class"""
 
     def __init__(self):
         self.output = Output()
         self.database = Database()
         self.config = Config()
+        self.file_system = FileSystem()
         self.logger = Logger().get_logger(__name__)
 
     def init(self):
         """Init database and configs"""
         self._configs = self.config.load()
         self.database.connect(self._configs["database"]["path"])
         self.database.migrate()
@@ -108,12 +111,40 @@
 
         print(
             self.output.render(
                 data, Output.JSON if output.lower() == "json" else Output.DEFAULT
             )
         )
 
+    def ssh(self, name):
+        """SSH to a host"""
+        host = self.database.get_host(name)
+
+        if host is None:
+            raise click.ClickException(f"Host with name {name} not found")
+
+        if host.ssh_private_key == "":
+            raise click.ClickException(
+                f"SSH feature is only for hosts with private keys"
+            )
+
+        tmp_path = self._configs["cache"]["path"]
+
+        if self.file_system.file_exists(f"{tmp_path}/{host.id}.pem"):
+            self.file_system.delete_file(f"{tmp_path}/{host.id}.pem")
+
+        self.file_system.write_file(
+            f"{tmp_path}/{host.id}.pem",
+            host.ssh_private_key,
+        )
+
+        self.file_system.change_permission(f"{tmp_path}/{host.id}.pem", 0o400)
+
+        cmd = f"ssh -o StrictHostKeyChecking=no -i {tmp_path}/{host.id}.pem -p {host.port} {host.user}@{host.ip}"
+
+        subprocess.run(cmd.split(" "))
+
     def delete(self, name):
         """Delete a host"""
         self.database.delete_host(name)
 
         click.echo(f"Host with name {name} got deleted")
```

### Comparing `flook-0.3.7/src/flook/command/recipes.py` & `flook-0.4.0/src/flook/command/recipes.py`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/src/flook/exception/__init__.py` & `flook-0.4.0/src/flook/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/src/flook/model/__init__.py` & `flook-0.4.0/src/flook/model/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/src/flook/model/host.py` & `flook-0.4.0/src/flook/model/host.py`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/src/flook/model/recipe.py` & `flook-0.4.0/src/flook/model/recipe.py`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/src/flook/model/task.py` & `flook-0.4.0/src/flook/model/task.py`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/src/flook/module/__init__.py` & `flook-0.4.0/src/flook/module/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/src/flook/module/config.py` & `flook-0.4.0/src/flook/module/config.py`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/src/flook/module/database.py` & `flook-0.4.0/src/flook/module/database.py`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/src/flook/module/file_system.py` & `flook-0.4.0/src/flook/module/file_system.py`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/src/flook/module/logger.py` & `flook-0.4.0/src/flook/module/logger.py`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/src/flook/module/output.py` & `flook-0.4.0/src/flook/module/output.py`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/src/flook/module/playbook.py` & `flook-0.4.0/src/flook/module/playbook.py`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/src/flook.egg-info/PKG-INFO` & `flook-0.4.0/src/flook.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flook
-Version: 0.3.7
+Version: 0.4.0
 Summary: A Lightweight and Flexible Ansible Command Line Tool.
 Home-page: https://github.com/norwik/flook/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/norwik/flook/
 Project-URL: Source, https://github.com/norwik/flook/
@@ -133,22 +133,29 @@
 12. To get a host
 
 .. code-block::
 
     $ flook host get <host_name>
 
 
-13. To delete a host
+13. To SSH into a host
+
+.. code-block::
+
+    $ flook host ssh <host_name>
+
+
+14. To delete a host
 
 .. code-block::
 
     $ flook host delete <host_name>
 
 
-14. Run a recipe towards a host
+15. Run a recipe towards a host
 
 .. code-block::
 
     $ flook recipe run <recipe_name> -h <host_name>
 
     # Some examples
     $ flook recipe run clivern/nginx -h example.com
```

### Comparing `flook-0.3.7/src/flook.egg-info/SOURCES.txt` & `flook-0.4.0/src/flook.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/tests/__init__.py` & `flook-0.4.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/tests/module/test_logger.py` & `flook-0.4.0/tests/module/test_logger.py`

 * *Files identical despite different names*

### Comparing `flook-0.3.7/tox.ini` & `flook-0.4.0/tox.ini`

 * *Files identical despite different names*

