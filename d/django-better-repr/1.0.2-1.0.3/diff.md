# Comparing `tmp/django-better-repr-1.0.2.tar.gz` & `tmp/django-better-repr-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-better-repr-1.0.2.tar", last modified: Fri Jun 30 21:39:54 2023, max compression
+gzip compressed data, was "django-better-repr-1.0.3.tar", last modified: Fri Jun 30 22:43:08 2023, max compression
```

## Comparing `django-better-repr-1.0.2.tar` & `django-better-repr-1.0.3.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:54.742149 django-better-repr-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:54.710146 django-better-repr-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:54.722147 django-better-repr-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13957 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-06-30 21:39:54.742149 django-better-repr-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:54.726148 django-better-repr-1.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:54.726148 django-better-repr-1.0.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/pyscaffold.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-30 21:39:54.742149 django-better-repr-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:54.710146 django-better-repr-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:54.726148 django-better-repr-1.0.2/src/django_better_repr/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/src/django_better_repr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/src/django_better_repr/bases.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/src/django_better_repr/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/src/django_better_repr/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:54.730148 django-better-repr-1.0.2/src/django_better_repr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-06-30 21:39:54.000000 django-better-repr-1.0.2/src/django_better_repr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-30 21:39:54.000000 django-better-repr-1.0.2/src/django_better_repr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 21:39:54.000000 django-better-repr-1.0.2/src/django_better_repr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 21:39:54.000000 django-better-repr-1.0.2/src/django_better_repr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-30 21:39:54.000000 django-better-repr-1.0.2/src/django_better_repr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-30 21:39:54.000000 django-better-repr-1.0.2/src/django_better_repr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:54.730148 django-better-repr-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:54.734148 django-better-repr-1.0.2/tests/example_project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      693 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   180224 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/db.sqlite3
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:54.738149 django-better-repr-1.0.2/tests/example_project/example_project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/example_project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/example_project/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/example_project/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/example_project/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/example_project/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:54.738149 django-better-repr-1.0.2/tests/example_project/myapp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/myapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/myapp/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/myapp/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:54.742149 django-better-repr-1.0.2/tests/example_project/myapp/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/myapp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/myapp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/myapp/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/myapp/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/example_project/myapp/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tests/test_better_repr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-30 21:39:10.000000 django-better-repr-1.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:43:08.310619 django-better-repr-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:43:08.290619 django-better-repr-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:43:08.298619 django-better-repr-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13957 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-06-30 22:43:08.310619 django-better-repr-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:43:08.298619 django-better-repr-1.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:43:08.298619 django-better-repr-1.0.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/pyscaffold.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-30 22:43:08.310619 django-better-repr-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:43:08.294619 django-better-repr-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:43:08.302619 django-better-repr-1.0.3/src/django_better_repr/
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/src/django_better_repr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/src/django_better_repr/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/src/django_better_repr/bases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/src/django_better_repr/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/src/django_better_repr/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/src/django_better_repr/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:43:08.306619 django-better-repr-1.0.3/src/django_better_repr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-06-30 22:43:08.000000 django-better-repr-1.0.3/src/django_better_repr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-30 22:43:08.000000 django-better-repr-1.0.3/src/django_better_repr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:43:08.000000 django-better-repr-1.0.3/src/django_better_repr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:43:07.000000 django-better-repr-1.0.3/src/django_better_repr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-30 22:43:08.000000 django-better-repr-1.0.3/src/django_better_repr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-30 22:43:08.000000 django-better-repr-1.0.3/src/django_better_repr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:43:08.306619 django-better-repr-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:43:08.306619 django-better-repr-1.0.3/tests/example_project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      693 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:43:08.306619 django-better-repr-1.0.3/tests/example_project/example_project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/example_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/example_project/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/example_project/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/example_project/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/example_project/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:43:08.310619 django-better-repr-1.0.3/tests/example_project/myapp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/myapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/myapp/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/myapp/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:43:08.310619 django-better-repr-1.0.3/tests/example_project/myapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/myapp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/myapp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/myapp/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/myapp/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/myapp/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/test_better_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tox.ini
```

### Comparing `django-better-repr-1.0.2/.coveragerc` & `django-better-repr-1.0.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.2/.github/workflows/ci.yml` & `django-better-repr-1.0.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.2/.gitignore` & `django-better-repr-1.0.3/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -53,9 +53,12 @@
 .conda*/
 .python-version
 
 # Environment
 .env
 .envrc
 
+# Django
+tests/example_project/db.sqlite3
+
 # Exclusions
 !pyscaffold.cfg
```

### Comparing `django-better-repr-1.0.2/.pre-commit-config.yaml` & `django-better-repr-1.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.2/.readthedocs.yml` & `django-better-repr-1.0.3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.2/CONTRIBUTING.rst` & `django-better-repr-1.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.2/LICENSE.txt` & `django-better-repr-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.2/PKG-INFO` & `django-better-repr-1.0.3/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: django-better-repr
-Version: 1.0.2
-Summary: Django model reprs for humans!
-Home-page: https://github.com/MrSage/django-better-repr
-Author: Collin Sage
-Author-email: 3229549+MrSage@users.noreply.github.com
-License: MIT
-Project-URL: Documentation, https://github.com/MrSage/django-better-repr
-Project-URL: Source, https://github.com/MrSage/django-better-repr
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst; charset=UTF-8
-Provides-Extra: testing
-License-File: LICENSE.txt
-
 .. These are examples of badges you might want to add to your README:
    please update the URLs accordingly
 
     .. image:: https://api.cirrus-ci.com/github/<USER>/django-better-repr.svg?branch=main
         :alt: Built Status
         :target: https://cirrus-ci.com/github/<USER>/django-better-repr
     .. image:: https://readthedocs.org/projects/django-better-repr/badge/?version=latest
@@ -61,15 +43,28 @@
 Installation
 ============
 
 ::
 
    pip install django-better-repr
 
-And that's it!
+If you want to automatically improve the repr of all models in your project then add `django_better_repr`
+to your installed apps.
+
+::
+
+   # settings.py
+   INSTALLED_APPS = [
+      ...,
+      'django_better_repr',
+      ...,
+   ]
+
+Want to customize which apps get configured but don't want to decorate each class individually?
+Head on down to the **Configuration** section.
 
 How to use:
 ===========
 
 The repr logic in this library is designed to produce the smallest, most meaningful repr possible
 for your Django models. That means that fields which aren't set won't show up in the repr. This
 should reduce noise and let you get the most value out of your reprs.
@@ -109,14 +104,16 @@
 ::
 
    # settings.py
    BETTER_REPR_CONFIG = {
       'ENABLE_MULTILINE_REPRS': True,  # bool (default: True), whether or not to allow multiline reprs
       'SINGLE_LINE_PARTS_LIMIT': 4,  # int (default: 4), the number of fields a repr can have before switching to multi line
       'MULTILINE_WHITESPACE': '\t',  # str (default: '\t'), the whitespace string to use for multiline reprs
+      'AUTO_CONFIGURE_INCLUDE_MODELS': [],  # list (default: a sentinel for all models), which models to auto include if the auto configuration application is added to INSTALLED_APPS
+      'AUTO_CONFIGURE_EXCLUDE_MODELS': [],  # list (default: []), which models to exclude from the auto setup if the auto configuration application is added to INSTALLED_APPS
    }
 
 
 .. _pyscaffold-notes:
 
 Making Changes & Contributing
 =============================
```

### Comparing `django-better-repr-1.0.2/README.rst` & `django-better-repr-1.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: django-better-repr
+Version: 1.0.3
+Summary: Django model reprs for humans!
+Home-page: https://github.com/MrSage/django-better-repr
+Author: Collin Sage
+Author-email: 3229549+MrSage@users.noreply.github.com
+License: MIT
+Project-URL: Documentation, https://github.com/MrSage/django-better-repr
+Project-URL: Source, https://github.com/MrSage/django-better-repr
+Platform: any
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst; charset=UTF-8
+Provides-Extra: testing
+License-File: LICENSE.txt
+
 .. These are examples of badges you might want to add to your README:
    please update the URLs accordingly
 
     .. image:: https://api.cirrus-ci.com/github/<USER>/django-better-repr.svg?branch=main
         :alt: Built Status
         :target: https://cirrus-ci.com/github/<USER>/django-better-repr
     .. image:: https://readthedocs.org/projects/django-better-repr/badge/?version=latest
@@ -43,15 +61,28 @@
 Installation
 ============
 
 ::
 
    pip install django-better-repr
 
-And that's it!
+If you want to automatically improve the repr of all models in your project then add `django_better_repr`
+to your installed apps.
+
+::
+
+   # settings.py
+   INSTALLED_APPS = [
+      ...,
+      'django_better_repr',
+      ...,
+   ]
+
+Want to customize which apps get configured but don't want to decorate each class individually?
+Head on down to the **Configuration** section.
 
 How to use:
 ===========
 
 The repr logic in this library is designed to produce the smallest, most meaningful repr possible
 for your Django models. That means that fields which aren't set won't show up in the repr. This
 should reduce noise and let you get the most value out of your reprs.
@@ -91,14 +122,16 @@
 ::
 
    # settings.py
    BETTER_REPR_CONFIG = {
       'ENABLE_MULTILINE_REPRS': True,  # bool (default: True), whether or not to allow multiline reprs
       'SINGLE_LINE_PARTS_LIMIT': 4,  # int (default: 4), the number of fields a repr can have before switching to multi line
       'MULTILINE_WHITESPACE': '\t',  # str (default: '\t'), the whitespace string to use for multiline reprs
+      'AUTO_CONFIGURE_INCLUDE_MODELS': [],  # list (default: a sentinel for all models), which models to auto include if the auto configuration application is added to INSTALLED_APPS
+      'AUTO_CONFIGURE_EXCLUDE_MODELS': [],  # list (default: []), which models to exclude from the auto setup if the auto configuration application is added to INSTALLED_APPS
    }
 
 
 .. _pyscaffold-notes:
 
 Making Changes & Contributing
 =============================
```

### Comparing `django-better-repr-1.0.2/docs/Makefile` & `django-better-repr-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.2/docs/conf.py` & `django-better-repr-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.2/docs/index.rst` & `django-better-repr-1.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.2/manage.py` & `django-better-repr-1.0.3/manage.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.2/setup.cfg` & `django-better-repr-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.2/setup.py` & `django-better-repr-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.2/src/django_better_repr/__init__.py` & `django-better-repr-1.0.3/src/django_better_repr/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     __version__ = "unknown"
 finally:
     del version, PackageNotFoundError
 
 
 def better_repr(klass: type = None, /, ):
     def decorator(kls: type):
-        kls.__bases__ = (BetterRepr, *kls.__bases__)
+        if BetterRepr not in kls.__bases__:
+            kls.__bases__ = (BetterRepr, *kls.__bases__)
         return kls
 
     if klass:
         return decorator(klass)
     else:
         return decorator
```

### Comparing `django-better-repr-1.0.2/src/django_better_repr/bases.py` & `django-better-repr-1.0.3/src/django_better_repr/bases.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.2/src/django_better_repr.egg-info/PKG-INFO` & `django-better-repr-1.0.3/src/django_better_repr.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-better-repr
-Version: 1.0.2
+Version: 1.0.3
 Summary: Django model reprs for humans!
 Home-page: https://github.com/MrSage/django-better-repr
 Author: Collin Sage
 Author-email: 3229549+MrSage@users.noreply.github.com
 License: MIT
 Project-URL: Documentation, https://github.com/MrSage/django-better-repr
 Project-URL: Source, https://github.com/MrSage/django-better-repr
@@ -61,15 +61,28 @@
 Installation
 ============
 
 ::
 
    pip install django-better-repr
 
-And that's it!
+If you want to automatically improve the repr of all models in your project then add `django_better_repr`
+to your installed apps.
+
+::
+
+   # settings.py
+   INSTALLED_APPS = [
+      ...,
+      'django_better_repr',
+      ...,
+   ]
+
+Want to customize which apps get configured but don't want to decorate each class individually?
+Head on down to the **Configuration** section.
 
 How to use:
 ===========
 
 The repr logic in this library is designed to produce the smallest, most meaningful repr possible
 for your Django models. That means that fields which aren't set won't show up in the repr. This
 should reduce noise and let you get the most value out of your reprs.
@@ -109,14 +122,16 @@
 ::
 
    # settings.py
    BETTER_REPR_CONFIG = {
       'ENABLE_MULTILINE_REPRS': True,  # bool (default: True), whether or not to allow multiline reprs
       'SINGLE_LINE_PARTS_LIMIT': 4,  # int (default: 4), the number of fields a repr can have before switching to multi line
       'MULTILINE_WHITESPACE': '\t',  # str (default: '\t'), the whitespace string to use for multiline reprs
+      'AUTO_CONFIGURE_INCLUDE_MODELS': [],  # list (default: a sentinel for all models), which models to auto include if the auto configuration application is added to INSTALLED_APPS
+      'AUTO_CONFIGURE_EXCLUDE_MODELS': [],  # list (default: []), which models to exclude from the auto setup if the auto configuration application is added to INSTALLED_APPS
    }
 
 
 .. _pyscaffold-notes:
 
 Making Changes & Contributing
 =============================
```

### Comparing `django-better-repr-1.0.2/src/django_better_repr.egg-info/SOURCES.txt` & `django-better-repr-1.0.3/src/django_better_repr.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,29 +22,30 @@
 docs/contributing.rst
 docs/index.rst
 docs/license.rst
 docs/readme.rst
 docs/requirements.txt
 docs/_static/.gitignore
 src/django_better_repr/__init__.py
+src/django_better_repr/apps.py
 src/django_better_repr/bases.py
 src/django_better_repr/config.py
 src/django_better_repr/exceptions.py
+src/django_better_repr/signals.py
 src/django_better_repr.egg-info/PKG-INFO
 src/django_better_repr.egg-info/SOURCES.txt
 src/django_better_repr.egg-info/dependency_links.txt
 src/django_better_repr.egg-info/not-zip-safe
 src/django_better_repr.egg-info/requires.txt
 src/django_better_repr.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
 tests/test_better_repr.py
 tests/example_project/__init__.py
 tests/example_project/__main__.py
-tests/example_project/db.sqlite3
 tests/example_project/example_project/__init__.py
 tests/example_project/example_project/asgi.py
 tests/example_project/example_project/settings.py
 tests/example_project/example_project/urls.py
 tests/example_project/example_project/wsgi.py
 tests/example_project/myapp/__init__.py
 tests/example_project/myapp/admin.py
```

### Comparing `django-better-repr-1.0.2/tests/example_project/__main__.py` & `django-better-repr-1.0.3/tests/example_project/__main__.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.2/tests/example_project/example_project/settings.py` & `django-better-repr-1.0.3/tests/example_project/example_project/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     'django.contrib.admin',
     'django.contrib.auth',
     'django.contrib.contenttypes',
     'django.contrib.sessions',
     'django.contrib.messages',
     'django.contrib.staticfiles',
     'tests.example_project.myapp',
+    'django_better_repr',
 ]
 
 MIDDLEWARE = [
     'django.middleware.security.SecurityMiddleware',
     'django.contrib.sessions.middleware.SessionMiddleware',
     'django.middleware.common.CommonMiddleware',
     'django.middleware.csrf.CsrfViewMiddleware',
```

### Comparing `django-better-repr-1.0.2/tests/example_project/example_project/urls.py` & `django-better-repr-1.0.3/tests/example_project/example_project/urls.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.2/tests/example_project/myapp/migrations/0001_initial.py` & `django-better-repr-1.0.3/tests/example_project/myapp/migrations/0001_initial.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 4.2.2 on 2023-06-30 21:09
+# Generated by Django 4.2.2 on 2023-06-30 22:41
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 import src.django_better_repr.bases
 
 
@@ -15,20 +15,31 @@
 
     operations = [
         migrations.CreateModel(
             name='JustForFKs',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
             ],
+            bases=(src.django_better_repr.bases.BetterRepr, models.Model),
         ),
         migrations.CreateModel(
             name='JustForM2Ms',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
             ],
+            bases=(src.django_better_repr.bases.BetterRepr, models.Model),
+        ),
+        migrations.CreateModel(
+            name='WithoutDecorator',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('one', models.CharField(max_length=16)),
+                ('two', models.CharField(default='Default', max_length=32, null=True)),
+            ],
+            bases=(src.django_better_repr.bases.BetterRepr, models.Model),
         ),
         migrations.CreateModel(
             name='FourOrMoreFields',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('one', models.CharField(max_length=16)),
                 ('two', models.CharField(default='Default', max_length=32, null=True)),
```

### Comparing `django-better-repr-1.0.2/tests/example_project/myapp/models.py` & `django-better-repr-1.0.3/tests/example_project/myapp/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,7 +25,12 @@
 class FourOrMoreFields(models.Model):
     one = models.CharField(max_length=16)
     two = models.CharField(max_length=32, default='Default', null=True)
     three = models.IntegerField(null=True)
     four = models.ForeignKey(to=JustForFKs, on_delete=models.CASCADE)
     five = models.ManyToManyField(to=JustForM2Ms)
     six = models.FloatField()
+
+
+class WithoutDecorator(models.Model):
+    one = models.CharField(max_length=16)
+    two = models.CharField(max_length=32, default='Default', null=True)
```

### Comparing `django-better-repr-1.0.2/tests/test_better_repr.py` & `django-better-repr-1.0.3/tests/test_better_repr.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pytest
 
 from tests.example_project.myapp.models import (
     FourOrLessFields,
     FourOrMoreFields,
     JustForFKs,
+    WithoutDecorator,
 )
 
 
 def test_with_four_or_less_fields():
     instance = FourOrLessFields()
     actual = repr(instance)
     expected = "FourOrLessFields()"
@@ -65,7 +66,18 @@
         four=JustForFKs.objects.create(),
         six=99.9,
     )
     actual = repr(instance)
     expected = "FourOrMoreFields(\n\tone='one',\n\ttwo='two',\n\tthree='three',\n\tfour_id=1,\n\tsix=99.9,\n)"
 
     assert actual == expected
+
+
+@pytest.mark.django_db
+def test_auto_configure_works():
+    instance = WithoutDecorator.objects.create(
+        one='one',
+        two='two',
+    )
+    actual = repr(instance)
+    expected = "WithoutDecorator(id=1, one='one', two='two')"
+    assert actual == expected
```

### Comparing `django-better-repr-1.0.2/tox.ini` & `django-better-repr-1.0.3/tox.ini`

 * *Files identical despite different names*

