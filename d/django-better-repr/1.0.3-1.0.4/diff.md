# Comparing `tmp/django-better-repr-1.0.3.tar.gz` & `tmp/django-better-repr-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-better-repr-1.0.3.tar", last modified: Fri Jun 30 22:43:08 2023, max compression
+gzip compressed data, was "django-better-repr-1.0.4.tar", last modified: Sat Jul  1 16:33:49 2023, max compression
```

## Comparing `django-better-repr-1.0.3.tar` & `django-better-repr-1.0.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:43:08.310619 django-better-repr-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:43:08.290619 django-better-repr-1.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:43:08.298619 django-better-repr-1.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13957 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-06-30 22:43:08.310619 django-better-repr-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:43:08.298619 django-better-repr-1.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:43:08.298619 django-better-repr-1.0.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/pyscaffold.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-30 22:43:08.310619 django-better-repr-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:43:08.294619 django-better-repr-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:43:08.302619 django-better-repr-1.0.3/src/django_better_repr/
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/src/django_better_repr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/src/django_better_repr/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/src/django_better_repr/bases.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/src/django_better_repr/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/src/django_better_repr/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/src/django_better_repr/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:43:08.306619 django-better-repr-1.0.3/src/django_better_repr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-06-30 22:43:08.000000 django-better-repr-1.0.3/src/django_better_repr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-30 22:43:08.000000 django-better-repr-1.0.3/src/django_better_repr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:43:08.000000 django-better-repr-1.0.3/src/django_better_repr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:43:07.000000 django-better-repr-1.0.3/src/django_better_repr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-30 22:43:08.000000 django-better-repr-1.0.3/src/django_better_repr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-30 22:43:08.000000 django-better-repr-1.0.3/src/django_better_repr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:43:08.306619 django-better-repr-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:43:08.306619 django-better-repr-1.0.3/tests/example_project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      693 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:43:08.306619 django-better-repr-1.0.3/tests/example_project/example_project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/example_project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/example_project/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/example_project/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/example_project/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/example_project/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:43:08.310619 django-better-repr-1.0.3/tests/example_project/myapp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/myapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/myapp/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/myapp/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:43:08.310619 django-better-repr-1.0.3/tests/example_project/myapp/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/myapp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/myapp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/myapp/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/myapp/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/example_project/myapp/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tests/test_better_repr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-30 22:42:18.000000 django-better-repr-1.0.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:49.976361 django-better-repr-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:49.952361 django-better-repr-1.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:49.960361 django-better-repr-1.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13957 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-01 16:33:49.976361 django-better-repr-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:49.964361 django-better-repr-1.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:49.964361 django-better-repr-1.0.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/pyscaffold.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-01 16:33:49.980361 django-better-repr-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:49.956361 django-better-repr-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:49.964361 django-better-repr-1.0.4/src/django_better_repr/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/src/django_better_repr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/src/django_better_repr/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/src/django_better_repr/bases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/src/django_better_repr/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/src/django_better_repr/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/src/django_better_repr/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:49.968361 django-better-repr-1.0.4/src/django_better_repr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-01 16:33:49.000000 django-better-repr-1.0.4/src/django_better_repr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-01 16:33:49.000000 django-better-repr-1.0.4/src/django_better_repr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 16:33:49.000000 django-better-repr-1.0.4/src/django_better_repr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 16:33:49.000000 django-better-repr-1.0.4/src/django_better_repr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-01 16:33:49.000000 django-better-repr-1.0.4/src/django_better_repr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-01 16:33:49.000000 django-better-repr-1.0.4/src/django_better_repr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:49.972361 django-better-repr-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:49.972361 django-better-repr-1.0.4/tests/example_project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      693 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:49.972361 django-better-repr-1.0.4/tests/example_project/example_project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/example_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/example_project/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/example_project/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/example_project/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/example_project/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:49.976361 django-better-repr-1.0.4/tests/example_project/myapp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/myapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/myapp/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/myapp/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:49.976361 django-better-repr-1.0.4/tests/example_project/myapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/myapp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/myapp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/myapp/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/myapp/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/example_project/myapp/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tests/test_better_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-01 16:33:13.000000 django-better-repr-1.0.4/tox.ini
```

### Comparing `django-better-repr-1.0.3/.coveragerc` & `django-better-repr-1.0.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.3/.github/workflows/ci.yml` & `django-better-repr-1.0.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.3/.gitignore` & `django-better-repr-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.3/.pre-commit-config.yaml` & `django-better-repr-1.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.3/.readthedocs.yml` & `django-better-repr-1.0.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.3/CONTRIBUTING.rst` & `django-better-repr-1.0.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.3/LICENSE.txt` & `django-better-repr-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.3/PKG-INFO` & `django-better-repr-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-better-repr
-Version: 1.0.3
+Version: 1.0.4
 Summary: Django model reprs for humans!
 Home-page: https://github.com/MrSage/django-better-repr
 Author: Collin Sage
 Author-email: 3229549+MrSage@users.noreply.github.com
 License: MIT
 Project-URL: Documentation, https://github.com/MrSage/django-better-repr
 Project-URL: Source, https://github.com/MrSage/django-better-repr
```

### Comparing `django-better-repr-1.0.3/README.rst` & `django-better-repr-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.3/docs/Makefile` & `django-better-repr-1.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.3/docs/conf.py` & `django-better-repr-1.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.3/docs/index.rst` & `django-better-repr-1.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.3/manage.py` & `django-better-repr-1.0.4/manage.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.3/setup.cfg` & `django-better-repr-1.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.3/setup.py` & `django-better-repr-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.3/src/django_better_repr/__init__.py` & `django-better-repr-1.0.4/src/django_better_repr/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 
-from src.django_better_repr.bases import BetterRepr
+from django_better_repr.bases import BetterRepr
 
 if sys.version_info[:2] >= (3, 8):
     # TODO: Import directly (no need for conditional) when `python_requires = >= 3.8`
     from importlib.metadata import PackageNotFoundError, version  # pragma: no cover
 else:
     from importlib_metadata import PackageNotFoundError, version  # pragma: no cover
```

### Comparing `django-better-repr-1.0.3/src/django_better_repr/bases.py` & `django-better-repr-1.0.4/src/django_better_repr/bases.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.3/src/django_better_repr/config.py` & `django-better-repr-1.0.4/src/django_better_repr/config.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.3/src/django_better_repr.egg-info/PKG-INFO` & `django-better-repr-1.0.4/src/django_better_repr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-better-repr
-Version: 1.0.3
+Version: 1.0.4
 Summary: Django model reprs for humans!
 Home-page: https://github.com/MrSage/django-better-repr
 Author: Collin Sage
 Author-email: 3229549+MrSage@users.noreply.github.com
 License: MIT
 Project-URL: Documentation, https://github.com/MrSage/django-better-repr
 Project-URL: Source, https://github.com/MrSage/django-better-repr
```

### Comparing `django-better-repr-1.0.3/src/django_better_repr.egg-info/SOURCES.txt` & `django-better-repr-1.0.4/src/django_better_repr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.3/tests/example_project/__main__.py` & `django-better-repr-1.0.4/tests/example_project/__main__.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.3/tests/example_project/example_project/settings.py` & `django-better-repr-1.0.4/tests/example_project/example_project/settings.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.3/tests/example_project/example_project/urls.py` & `django-better-repr-1.0.4/tests/example_project/example_project/urls.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.3/tests/example_project/myapp/migrations/0001_initial.py` & `django-better-repr-1.0.4/tests/example_project/myapp/migrations/0001_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Generated by Django 4.2.2 on 2023-06-30 22:41
 
 import django.db.models.deletion
 from django.db import migrations, models
 
-import src.django_better_repr.bases
+import django_better_repr.bases
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
@@ -15,50 +15,50 @@
 
     operations = [
         migrations.CreateModel(
             name='JustForFKs',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
             ],
-            bases=(src.django_better_repr.bases.BetterRepr, models.Model),
+            bases=(django_better_repr.bases.BetterRepr, models.Model),
         ),
         migrations.CreateModel(
             name='JustForM2Ms',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
             ],
-            bases=(src.django_better_repr.bases.BetterRepr, models.Model),
+            bases=(django_better_repr.bases.BetterRepr, models.Model),
         ),
         migrations.CreateModel(
             name='WithoutDecorator',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('one', models.CharField(max_length=16)),
                 ('two', models.CharField(default='Default', max_length=32, null=True)),
             ],
-            bases=(src.django_better_repr.bases.BetterRepr, models.Model),
+            bases=(django_better_repr.bases.BetterRepr, models.Model),
         ),
         migrations.CreateModel(
             name='FourOrMoreFields',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('one', models.CharField(max_length=16)),
                 ('two', models.CharField(default='Default', max_length=32, null=True)),
                 ('three', models.IntegerField(null=True)),
                 ('six', models.FloatField()),
                 ('five', models.ManyToManyField(to='myapp.justform2ms')),
                 ('four', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='myapp.justforfks')),
             ],
-            bases=(src.django_better_repr.bases.BetterRepr, models.Model),
+            bases=(django_better_repr.bases.BetterRepr, models.Model),
         ),
         migrations.CreateModel(
             name='FourOrLessFields',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('one', models.CharField(max_length=16)),
                 ('two', models.CharField(default='Default', max_length=32, null=True)),
                 ('three', models.IntegerField(null=True)),
                 ('four', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='myapp.justforfks')),
             ],
-            bases=(src.django_better_repr.bases.BetterRepr, models.Model),
+            bases=(django_better_repr.bases.BetterRepr, models.Model),
         ),
     ]
```

### Comparing `django-better-repr-1.0.3/tests/example_project/myapp/models.py` & `django-better-repr-1.0.4/tests/example_project/myapp/models.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.3/tests/test_better_repr.py` & `django-better-repr-1.0.4/tests/test_better_repr.py`

 * *Files identical despite different names*

### Comparing `django-better-repr-1.0.3/tox.ini` & `django-better-repr-1.0.4/tox.ini`

 * *Files identical despite different names*

