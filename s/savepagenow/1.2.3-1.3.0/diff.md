# Comparing `tmp/savepagenow-1.2.3.tar.gz` & `tmp/savepagenow-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "savepagenow-1.2.3.tar", last modified: Sun Jun 26 22:37:24 2022, max compression
+gzip compressed data, was "savepagenow-1.3.0.tar", last modified: Sat Jul  1 13:31:01 2023, max compression
```

## Comparing `savepagenow-1.2.3.tar` & `savepagenow-1.3.0.tar`

### file list

```diff
@@ -1,102 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:37:24.337131 savepagenow-1.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:37:24.325131 savepagenow-1.2.3/.github/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-26 22:37:06.000000 savepagenow-1.2.3/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:37:24.325131 savepagenow-1.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      743 2022-06-26 22:37:06.000000 savepagenow-1.2.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3130 2022-06-26 22:37:06.000000 savepagenow-1.2.3/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-06-26 22:37:06.000000 savepagenow-1.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1352 2022-06-26 22:37:06.000000 savepagenow-1.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-06-26 22:37:06.000000 savepagenow-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-06-26 22:37:06.000000 savepagenow-1.2.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     1480 2022-06-26 22:37:24.337131 savepagenow-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-06-26 22:37:06.000000 savepagenow-1.2.3/Pipfile
--rw-r--r--   0 runner    (1001) docker     (121)    70706 2022-06-26 22:37:06.000000 savepagenow-1.2.3/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-06-26 22:37:06.000000 savepagenow-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:37:24.325131 savepagenow-1.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:37:24.321131 savepagenow-1.2.3/docs/_build/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:37:24.325131 savepagenow-1.2.3/docs/_build/doctrees/
--rw-r--r--   0 runner    (1001) docker     (121)     8840 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/doctrees/cli.doctree
--rw-r--r--   0 runner    (1001) docker     (121)    17048 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/doctrees/environment.pickle
--rw-r--r--   0 runner    (1001) docker     (121)     8661 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/doctrees/index.doctree
--rw-r--r--   0 runner    (1001) docker     (121)     7041 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/doctrees/install.doctree
--rw-r--r--   0 runner    (1001) docker     (121)     8270 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/doctrees/python.doctree
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:37:24.329131 savepagenow-1.2.3/docs/_build/html/
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/.buildinfo
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:37:24.329131 savepagenow-1.2.3/docs/_build/html/.doctrees/
--rw-r--r--   0 runner    (1001) docker     (121)    13465 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/.doctrees/cli.doctree
--rw-r--r--   0 runner    (1001) docker     (121)     4053 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/.doctrees/contributing.doctree
--rw-r--r--   0 runner    (1001) docker     (121)    20070 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/.doctrees/environment.pickle
--rw-r--r--   0 runner    (1001) docker     (121)    16126 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/.doctrees/exceptions.doctree
--rw-r--r--   0 runner    (1001) docker     (121)     9204 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/.doctrees/index.doctree
--rw-r--r--   0 runner    (1001) docker     (121)     7041 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/.doctrees/install.doctree
--rw-r--r--   0 runner    (1001) docker     (121)    11496 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/.doctrees/python.doctree
--rw-r--r--   0 runner    (1001) docker     (121)     8394 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/.doctrees/useragent.doctree
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:37:24.329131 savepagenow-1.2.3/docs/_build/html/_sources/
--rw-r--r--   0 runner    (1001) docker     (121)      675 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/_sources/cli.md.txt
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/_sources/contributing.md.txt
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/_sources/exceptions.md.txt
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/_sources/index.md.txt
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/_sources/install.md.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1744 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/_sources/python.md.txt
--rw-r--r--   0 runner    (1001) docker     (121)      668 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/_sources/useragent.md.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:37:24.333131 savepagenow-1.2.3/docs/_build/html/_static/
--rw-r--r--   0 runner    (1001) docker     (121)    11186 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/_static/alabaster.css
--rw-r--r--   0 runner    (1001) docker     (121)    14693 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/_static/basic.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:37:24.333131 savepagenow-1.2.3/docs/_build/html/_static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     3689 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (121)    10766 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (121)   287630 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/_static/jquery-3.5.1.js
--rw-r--r--   0 runner    (1001) docker     (121)    89476 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/_static/jquery.js
--rw-r--r--   0 runner    (1001) docker     (121)    10852 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (121)     4847 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (121)    16634 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (121)    68420 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 runner    (1001) docker     (121)    19531 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/_static/underscore.js
--rw-r--r--   0 runner    (1001) docker     (121)     8429 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/cli.html
--rw-r--r--   0 runner    (1001) docker     (121)     4048 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/contributing.html
--rw-r--r--   0 runner    (1001) docker     (121)     8306 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/exceptions.html
--rw-r--r--   0 runner    (1001) docker     (121)     6593 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/genindex.html
--rw-r--r--   0 runner    (1001) docker     (121)     6339 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/index.html
--rw-r--r--   0 runner    (1001) docker     (121)     5686 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/install.html
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/objects.inv
--rw-r--r--   0 runner    (1001) docker     (121)     3661 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/py-modindex.html
--rw-r--r--   0 runner    (1001) docker     (121)    10757 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/python.html
--rw-r--r--   0 runner    (1001) docker     (121)     3205 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/search.html
--rw-r--r--   0 runner    (1001) docker     (121)     3296 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/searchindex.js
--rw-r--r--   0 runner    (1001) docker     (121)     6576 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_build/html/useragent.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:37:24.321131 savepagenow-1.2.3/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:37:24.333131 savepagenow-1.2.3/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     3689 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:37:24.333131 savepagenow-1.2.3/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)     1523 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/_templates/nav.html
--rw-r--r--   0 runner    (1001) docker     (121)      675 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (121)      878 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/exceptions.md
--rw-r--r--   0 runner    (1001) docker     (121)      637 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/install.md
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)     1744 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/python.md
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      668 2022-06-26 22:37:06.000000 savepagenow-1.2.3/docs/useragent.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:37:24.333131 savepagenow-1.2.3/savepagenow/
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-06-26 22:37:06.000000 savepagenow-1.2.3/savepagenow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4843 2022-06-26 22:37:06.000000 savepagenow-1.2.3/savepagenow/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-06-26 22:37:06.000000 savepagenow-1.2.3/savepagenow/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:37:24.333131 savepagenow-1.2.3/savepagenow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1480 2022-06-26 22:37:23.000000 savepagenow-1.2.3/savepagenow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2544 2022-06-26 22:37:24.000000 savepagenow-1.2.3/savepagenow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-26 22:37:23.000000 savepagenow-1.2.3/savepagenow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-06-26 22:37:23.000000 savepagenow-1.2.3/savepagenow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-06-26 22:37:23.000000 savepagenow-1.2.3/savepagenow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-06-26 22:37:23.000000 savepagenow-1.2.3/savepagenow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-06-26 22:37:24.337131 savepagenow-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2505 2022-06-26 22:37:06.000000 savepagenow-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 22:37:24.333131 savepagenow-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-26 22:37:06.000000 savepagenow-1.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-06-26 22:37:06.000000 savepagenow-1.2.3/tests/test_capture.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:31:01.300133 savepagenow-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:31:01.300133 savepagenow-1.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-01 13:30:47.000000 savepagenow-1.3.0/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:31:01.300133 savepagenow-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-01 13:30:47.000000 savepagenow-1.3.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-07-01 13:30:47.000000 savepagenow-1.3.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-01 13:30:47.000000 savepagenow-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-01 13:30:47.000000 savepagenow-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-01 13:30:47.000000 savepagenow-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-01 13:31:01.300133 savepagenow-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-01 13:30:47.000000 savepagenow-1.3.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    81741 2023-07-01 13:30:47.000000 savepagenow-1.3.0/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-01 13:30:47.000000 savepagenow-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:31:01.300133 savepagenow-1.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-01 13:30:47.000000 savepagenow-1.3.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:31:01.296133 savepagenow-1.3.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:31:01.300133 savepagenow-1.3.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-07-01 13:30:47.000000 savepagenow-1.3.0/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:31:01.300133 savepagenow-1.3.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-01 13:30:47.000000 savepagenow-1.3.0/docs/_templates/nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-01 13:30:47.000000 savepagenow-1.3.0/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-01 13:30:47.000000 savepagenow-1.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-01 13:30:47.000000 savepagenow-1.3.0/docs/exceptions.md
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-01 13:30:47.000000 savepagenow-1.3.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-01 13:30:47.000000 savepagenow-1.3.0/docs/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-01 13:30:47.000000 savepagenow-1.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-01 13:30:47.000000 savepagenow-1.3.0/docs/python.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-01 13:30:47.000000 savepagenow-1.3.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-01 13:30:47.000000 savepagenow-1.3.0/docs/useragent.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:31:01.300133 savepagenow-1.3.0/savepagenow/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-01 13:30:47.000000 savepagenow-1.3.0/savepagenow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-07-01 13:30:47.000000 savepagenow-1.3.0/savepagenow/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-01 13:30:47.000000 savepagenow-1.3.0/savepagenow/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:31:01.300133 savepagenow-1.3.0/savepagenow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-01 13:31:01.000000 savepagenow-1.3.0/savepagenow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-01 13:31:01.000000 savepagenow-1.3.0/savepagenow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 13:31:01.000000 savepagenow-1.3.0/savepagenow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-01 13:31:01.000000 savepagenow-1.3.0/savepagenow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-01 13:31:01.000000 savepagenow-1.3.0/savepagenow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-01 13:31:01.000000 savepagenow-1.3.0/savepagenow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-01 13:31:01.304133 savepagenow-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-01 13:30:47.000000 savepagenow-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:31:01.300133 savepagenow-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:30:47.000000 savepagenow-1.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-01 13:30:47.000000 savepagenow-1.3.0/tests/test_capture.py
```

### Comparing `savepagenow-1.2.3/.github/workflows/docs.yml` & `savepagenow-1.3.0/.github/workflows/docs.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,35 @@
-name: "Build documentation"
+name: Build documentation
+
 on:
   push:
-  pull_request:
+    branches:
+    - main
   workflow_dispatch:
 
 jobs:
   docs:
-    name: "Build and deploy"
+    name: Build and deploy
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v1
+    - name: Checkout
+      uses: actions/checkout@v3
 
-    - uses: ammaraskar/sphinx-action@master
+    - name: Build documentation
+      uses: ammaraskar/sphinx-action@master
       with:
         docs-folder: "docs/"
 
-    - uses: actions/upload-artifact@v1
+    - name: Upload artifact
+      uses: actions/upload-artifact@v3
       with:
         name: documentation-html
         path: docs/_build/html/
 
-    - uses: shallwefootball/s3-upload-action@master
+    - name: Deploy site
+      uses: shallwefootball/s3-upload-action@master
       with:
         aws_key_id: ${{ secrets.PALEWIRE_DOCS_AWS_ACCESS_KEY_ID }}
         aws_secret_access_key: ${{ secrets.PALEWIRE_DOCS_AWS_SECRET_ACCESS_KEY }}
         aws_bucket: ${{ secrets.PALEWIRE_DOCS_AWS_BUCKET }}
         source_dir: docs/_build/html/
         destination_dir: savepagenow
```

### Comparing `savepagenow-1.2.3/.pre-commit-config.yaml` & `savepagenow-1.3.0/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.1.0
+    rev: v4.4.0
     hooks:
     -   id: trailing-whitespace
     -   id: end-of-file-fixer
     -   id: check-yaml
     -   id: check-added-large-files
         args: ['--maxkb=10000']
     -   id: check-byte-order-marker
     -   id: check-case-conflict
     -   id: check-json
     -   id: mixed-line-ending
 
 -   repo: https://github.com/psf/black
-    rev: 21.12b0
+    rev: 23.3.0
     hooks:
     -   id: black
 
 -   repo: https://github.com/asottile/blacken-docs
-    rev: v1.12.0
+    rev: 1.14.0
     hooks:
     -   id: blacken-docs
         additional_dependencies: [black]
 
 -   repo: https://github.com/timothycrosley/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
     -   id: isort
         args: ["--profile", "black", "--filter-files"]
 
--   repo: https://gitlab.com/pycqa/flake8
-    rev: 3.9.2
+-   repo: https://github.com/pycqa/flake8
+    rev: 6.0.0
     hooks:
     - id: flake8
       additional_dependencies:
         - flake8-docstrings
         - flake8-bugbear
 
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v2.31.0
+    rev: v3.7.0
     hooks:
     -   id: pyupgrade
         args: [--py37-plus]
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: 'v0.931'  # Use the sha / tag you want to point at
+    rev: 'v1.4.1'  # Use the sha / tag you want to point at
     hooks:
     -   id: mypy
         additional_dependencies:
           - types-requests
```

### Comparing `savepagenow-1.2.3/LICENSE` & `savepagenow-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `savepagenow-1.2.3/PKG-INFO` & `savepagenow-1.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 Metadata-Version: 2.1
 Name: savepagenow
-Version: 1.2.3
+Version: 1.3.0
 Summary: A simple Python wrapper and command-line interface for archive.org’s "Save Page Now" capturing service
 Home-page: https://www.github.com/palewire/savepagenow/
 Author: Ben Welsh
 Author-email: b@palewi.re
 License: MIT
 Project-URL: Documentation, http://palewi.re/docs/savepagenow
 Project-URL: Source, https://github.com/palewire/savepagenow
 Project-URL: Tracker, https://github.com/palewire/savepagenow/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Links
 
 - Documentation: [palewi.re/docs/savepagenow/](https://palewi.re/docs/savepagenow/)
 - Save Page Now at archive.org: [archive.org/web](https://archive.org/web)
 - Code: [github.com/palewire/savepagenow](https://github.com/palewire/savepagenow)
 - Issues: [github.com/palewire/savepagenow/issues](https://github.com/palewire/savepagenow/issues)
 - Packaging: [pypi.org/project/savepagenow](https://pypi.org/project/savepagenow)
-
-
```

### Comparing `savepagenow-1.2.3/Pipfile.lock` & `savepagenow-1.3.0/Pipfile.lock`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8892939814814816%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'4777043449c55048829997680588210422a8467630e20bdc602008b706a5e930'}, 'requires': "*

 * *            "{'python_version': '3.10'}}",*

 * * "'default'": "{'certifi': {'hashes': "*

 * *              "['sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7', "*

 * *              "'sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716'], "*

 * *              '\'version\': \'==2023.5.7\', \'markers\': "python_version >= \'3.6\'"}, '*

 * *              "'charset […]*

```diff
@@ -1,813 +1,952 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "43da5d0c59f685f363438bb5f678320da0153b0c872e98aed22bd38eb7f8b312"
+            "sha256": "4777043449c55048829997680588210422a8467630e20bdc602008b706a5e930"
         },
         "pipfile-spec": 6,
         "requires": {
-            "python_version": "3.9"
+            "python_version": "3.10"
         },
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.python.org/simple",
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "certifi": {
             "hashes": [
-                "sha256:78884e7c1d4b00ce3cea67b44566851c4343c120abd683433ce934a68ea58872",
-                "sha256:d62a0163eb4c2344ac042ab2bdf75399a71a2d8c7d47eac2e2ee91b9d6339569"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
-            "version": "==2021.10.8"
+            "markers": "python_version >= '3.6'",
+            "version": "==2023.5.7"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:2857e29ff0d34db842cd7ca3230549d1a697f96ee6d3fb071cfa6c7393832597",
-                "sha256:6881edbebdb17b39b4eaaa821b438bf6eddffb4468cf344f09f89def34a8b1df"
+                "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
+                "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
+                "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
+                "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
+                "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62",
+                "sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230",
+                "sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be",
+                "sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c",
+                "sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0",
+                "sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448",
+                "sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f",
+                "sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649",
+                "sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d",
+                "sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0",
+                "sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706",
+                "sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a",
+                "sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59",
+                "sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23",
+                "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5",
+                "sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb",
+                "sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e",
+                "sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e",
+                "sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c",
+                "sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28",
+                "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d",
+                "sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41",
+                "sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974",
+                "sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce",
+                "sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f",
+                "sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1",
+                "sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d",
+                "sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8",
+                "sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017",
+                "sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31",
+                "sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7",
+                "sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8",
+                "sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e",
+                "sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14",
+                "sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd",
+                "sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d",
+                "sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795",
+                "sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b",
+                "sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b",
+                "sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b",
+                "sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203",
+                "sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f",
+                "sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19",
+                "sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1",
+                "sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a",
+                "sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac",
+                "sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9",
+                "sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0",
+                "sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137",
+                "sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f",
+                "sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6",
+                "sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5",
+                "sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909",
+                "sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f",
+                "sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0",
+                "sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324",
+                "sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755",
+                "sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb",
+                "sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854",
+                "sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c",
+                "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60",
+                "sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84",
+                "sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0",
+                "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b",
+                "sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1",
+                "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
+                "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
+                "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
+                "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
+                "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
+                "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
             ],
-            "markers": "python_version >= '3'",
-            "version": "==2.0.12"
+            "markers": "python_full_version >= '3.7.0'",
+            "version": "==3.1.0"
         },
         "click": {
             "hashes": [
-                "sha256:19a4baa64da924c5e0cd889aba8e947f280309f1a2ce0947a3e3a7bcb7cc72d6",
-                "sha256:977c213473c7665d3aa092b41ff12063227751c41d7b17165013e10069cc5cd2"
+                "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
+                "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
             ],
             "index": "pypi",
-            "version": "==8.1.0"
+            "version": "==8.1.3"
         },
         "idna": {
             "hashes": [
-                "sha256:84d9dd047ffa80596e0f246e2eab0b391788b0503584e8945f2368256d2735ff",
-                "sha256:9d643ff0a55b762d5cdb124b8eaa99c66322e2157b69160bc32796e824360e6d"
+                "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
+                "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
-            "markers": "python_version >= '3'",
-            "version": "==3.3"
+            "markers": "python_version >= '3.5'",
+            "version": "==3.4"
         },
         "requests": {
             "hashes": [
-                "sha256:68d7c56fd5a8999887728ef304a6d12edc7be74f1cfa47714fc8b414525c9a61",
-                "sha256:f22fa1e554c9ddfd16e6e41ac79759e17be9e492b3587efa038054674760e72d"
+                "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
+                "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
             "index": "pypi",
-            "version": "==2.27.1"
+            "version": "==2.31.0"
         },
         "urllib3": {
             "hashes": [
-                "sha256:44ece4d53fb1706f667c9bd1c648f5469a2ec925fcf3a776667042d645472c14",
-                "sha256:aabaf16477806a5e1dd19aa41f8c2b7950dd3c746362d7e3223dbe6de6ac448e"
+                "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1",
+                "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4' and python_version < '4'",
-            "version": "==1.26.9"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.0.3"
         }
     },
     "develop": {
         "alabaster": {
             "hashes": [
-                "sha256:446438bdcca0e05bd45ea2de1668c1d9b032e1a9154c2c259092d77031ddd359",
-                "sha256:a661d72d58e6ea8a57f7a86e37d86716863ee5e92788398526d58b26a4e4dc02"
+                "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3",
+                "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
             ],
-            "version": "==0.7.12"
+            "markers": "python_version >= '3.6'",
+            "version": "==0.7.13"
         },
         "attrs": {
             "hashes": [
-                "sha256:2d27e3784d7a565d36ab851fe94887c5eccd6a463168875832a1be79c82828b4",
-                "sha256:626ba8234211db98e869df76230a137c4c40a12d72445c45d5f5b716f076e2fd"
+                "sha256:1f28b4522cdc2fb4256ac1a020c78acf9cba2c6b461ccd2c126f3aa8e8335d04",
+                "sha256:6279836d581513a26f1bf235f9acd333bc9115683f14f7e8fae46c98fc50e015"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==21.4.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==23.1.0"
         },
         "babel": {
             "hashes": [
-                "sha256:ab49e12b91d937cd11f0b67cb259a57ab4ad2b59ac7a3b41d6c06c0ac5b0def9",
-                "sha256:bc0c176f9f6a994582230df350aa6e05ba2ebe4b3ac317eab29d9be5d2768da0"
+                "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610",
+                "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==2.9.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.12.1"
         },
         "black": {
             "hashes": [
-                "sha256:35020b8886c022ced9282b51b5a875b6d1ab0c387b31a065b84db7c33085ca79",
-                "sha256:bc58025940a896d7e5356952228b68f793cf5fcb342be703c3a2669a1488cb72"
+                "sha256:064101748afa12ad2291c2b91c960be28b817c0c7eaa35bec09cc63aa56493c5",
+                "sha256:0945e13506be58bf7db93ee5853243eb368ace1c08a24c65ce108986eac65915",
+                "sha256:11c410f71b876f961d1de77b9699ad19f939094c3a677323f43d7a29855fe326",
+                "sha256:1c7b8d606e728a41ea1ccbd7264677e494e87cf630e399262ced92d4a8dac940",
+                "sha256:1d06691f1eb8de91cd1b322f21e3bfc9efe0c7ca1f0e1eb1db44ea367dff656b",
+                "sha256:3238f2aacf827d18d26db07524e44741233ae09a584273aa059066d644ca7b30",
+                "sha256:32daa9783106c28815d05b724238e30718f34155653d4d6e125dc7daec8e260c",
+                "sha256:35d1381d7a22cc5b2be2f72c7dfdae4072a3336060635718cc7e1ede24221d6c",
+                "sha256:3a150542a204124ed00683f0db1f5cf1c2aaaa9cc3495b7a3b5976fb136090ab",
+                "sha256:48f9d345675bb7fbc3dd85821b12487e1b9a75242028adad0333ce36ed2a6d27",
+                "sha256:50cb33cac881766a5cd9913e10ff75b1e8eb71babf4c7104f2e9c52da1fb7de2",
+                "sha256:562bd3a70495facf56814293149e51aa1be9931567474993c7942ff7d3533961",
+                "sha256:67de8d0c209eb5b330cce2469503de11bca4085880d62f1628bd9972cc3366b9",
+                "sha256:6b39abdfb402002b8a7d030ccc85cf5afff64ee90fa4c5aebc531e3ad0175ddb",
+                "sha256:6f3c333ea1dd6771b2d3777482429864f8e258899f6ff05826c3a4fcc5ce3f70",
+                "sha256:714290490c18fb0126baa0fca0a54ee795f7502b44177e1ce7624ba1c00f2331",
+                "sha256:7c3eb7cea23904399866c55826b31c1f55bbcd3890ce22ff70466b907b6775c2",
+                "sha256:92c543f6854c28a3c7f39f4d9b7694f9a6eb9d3c5e2ece488c327b6e7ea9b266",
+                "sha256:a6f6886c9869d4daae2d1715ce34a19bbc4b95006d20ed785ca00fa03cba312d",
+                "sha256:a8a968125d0a6a404842fa1bf0b349a568634f856aa08ffaff40ae0dfa52e7c6",
+                "sha256:c7ab5790333c448903c4b721b59c0d80b11fe5e9803d8703e84dcb8da56fec1b",
+                "sha256:e114420bf26b90d4b9daa597351337762b63039752bdf72bf361364c1aa05925",
+                "sha256:e198cf27888ad6f4ff331ca1c48ffc038848ea9f031a3b40ba36aced7e22f2c8",
+                "sha256:ec751418022185b0c1bb7d7736e6933d40bbb14c14a0abcf9123d1b159f98dd4",
+                "sha256:f0bd2f4a58d6666500542b26354978218a9babcdc972722f4bf90779524515f3"
             ],
             "index": "pypi",
-            "version": "==22.3.0"
+            "version": "==23.3.0"
         },
         "bleach": {
             "hashes": [
-                "sha256:0900d8b37eba61a802ee40ac0061f8c2b5dee29c1927dd1d233e075ebf5a71da",
-                "sha256:4d2651ab93271d1129ac9cbc679f524565cc8a1b791909c4a51eac4446a15994"
+                "sha256:1a1a85c1595e07d8db14c5f09f09e6433502c51c595970edc090551f0db99414",
+                "sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==4.1.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==6.0.0"
         },
         "certifi": {
             "hashes": [
-                "sha256:78884e7c1d4b00ce3cea67b44566851c4343c120abd683433ce934a68ea58872",
-                "sha256:d62a0163eb4c2344ac042ab2bdf75399a71a2d8c7d47eac2e2ee91b9d6339569"
-            ],
-            "version": "==2021.10.8"
-        },
-        "cffi": {
-            "hashes": [
-                "sha256:00c878c90cb53ccfaae6b8bc18ad05d2036553e6d9d1d9dbcf323bbe83854ca3",
-                "sha256:0104fb5ae2391d46a4cb082abdd5c69ea4eab79d8d44eaaf79f1b1fd806ee4c2",
-                "sha256:06c48159c1abed75c2e721b1715c379fa3200c7784271b3c46df01383b593636",
-                "sha256:0808014eb713677ec1292301ea4c81ad277b6cdf2fdd90fd540af98c0b101d20",
-                "sha256:10dffb601ccfb65262a27233ac273d552ddc4d8ae1bf93b21c94b8511bffe728",
-                "sha256:14cd121ea63ecdae71efa69c15c5543a4b5fbcd0bbe2aad864baca0063cecf27",
-                "sha256:17771976e82e9f94976180f76468546834d22a7cc404b17c22df2a2c81db0c66",
-                "sha256:181dee03b1170ff1969489acf1c26533710231c58f95534e3edac87fff06c443",
-                "sha256:23cfe892bd5dd8941608f93348c0737e369e51c100d03718f108bf1add7bd6d0",
-                "sha256:263cc3d821c4ab2213cbe8cd8b355a7f72a8324577dc865ef98487c1aeee2bc7",
-                "sha256:2756c88cbb94231c7a147402476be2c4df2f6078099a6f4a480d239a8817ae39",
-                "sha256:27c219baf94952ae9d50ec19651a687b826792055353d07648a5695413e0c605",
-                "sha256:2a23af14f408d53d5e6cd4e3d9a24ff9e05906ad574822a10563efcef137979a",
-                "sha256:31fb708d9d7c3f49a60f04cf5b119aeefe5644daba1cd2a0fe389b674fd1de37",
-                "sha256:3415c89f9204ee60cd09b235810be700e993e343a408693e80ce7f6a40108029",
-                "sha256:3773c4d81e6e818df2efbc7dd77325ca0dcb688116050fb2b3011218eda36139",
-                "sha256:3b96a311ac60a3f6be21d2572e46ce67f09abcf4d09344c49274eb9e0bf345fc",
-                "sha256:3f7d084648d77af029acb79a0ff49a0ad7e9d09057a9bf46596dac9514dc07df",
-                "sha256:41d45de54cd277a7878919867c0f08b0cf817605e4eb94093e7516505d3c8d14",
-                "sha256:4238e6dab5d6a8ba812de994bbb0a79bddbdf80994e4ce802b6f6f3142fcc880",
-                "sha256:45db3a33139e9c8f7c09234b5784a5e33d31fd6907800b316decad50af323ff2",
-                "sha256:45e8636704eacc432a206ac7345a5d3d2c62d95a507ec70d62f23cd91770482a",
-                "sha256:4958391dbd6249d7ad855b9ca88fae690783a6be9e86df65865058ed81fc860e",
-                "sha256:4a306fa632e8f0928956a41fa8e1d6243c71e7eb59ffbd165fc0b41e316b2474",
-                "sha256:57e9ac9ccc3101fac9d6014fba037473e4358ef4e89f8e181f8951a2c0162024",
-                "sha256:59888172256cac5629e60e72e86598027aca6bf01fa2465bdb676d37636573e8",
-                "sha256:5e069f72d497312b24fcc02073d70cb989045d1c91cbd53979366077959933e0",
-                "sha256:64d4ec9f448dfe041705426000cc13e34e6e5bb13736e9fd62e34a0b0c41566e",
-                "sha256:6dc2737a3674b3e344847c8686cf29e500584ccad76204efea14f451d4cc669a",
-                "sha256:74fdfdbfdc48d3f47148976f49fab3251e550a8720bebc99bf1483f5bfb5db3e",
-                "sha256:75e4024375654472cc27e91cbe9eaa08567f7fbdf822638be2814ce059f58032",
-                "sha256:786902fb9ba7433aae840e0ed609f45c7bcd4e225ebb9c753aa39725bb3e6ad6",
-                "sha256:8b6c2ea03845c9f501ed1313e78de148cd3f6cad741a75d43a29b43da27f2e1e",
-                "sha256:91d77d2a782be4274da750752bb1650a97bfd8f291022b379bb8e01c66b4e96b",
-                "sha256:91ec59c33514b7c7559a6acda53bbfe1b283949c34fe7440bcf917f96ac0723e",
-                "sha256:920f0d66a896c2d99f0adbb391f990a84091179542c205fa53ce5787aff87954",
-                "sha256:a5263e363c27b653a90078143adb3d076c1a748ec9ecc78ea2fb916f9b861962",
-                "sha256:abb9a20a72ac4e0fdb50dae135ba5e77880518e742077ced47eb1499e29a443c",
-                "sha256:c2051981a968d7de9dd2d7b87bcb9c939c74a34626a6e2f8181455dd49ed69e4",
-                "sha256:c21c9e3896c23007803a875460fb786118f0cdd4434359577ea25eb556e34c55",
-                "sha256:c2502a1a03b6312837279c8c1bd3ebedf6c12c4228ddbad40912d671ccc8a962",
-                "sha256:d4d692a89c5cf08a8557fdeb329b82e7bf609aadfaed6c0d79f5a449a3c7c023",
-                "sha256:da5db4e883f1ce37f55c667e5c0de439df76ac4cb55964655906306918e7363c",
-                "sha256:e7022a66d9b55e93e1a845d8c9eba2a1bebd4966cd8bfc25d9cd07d515b33fa6",
-                "sha256:ef1f279350da2c586a69d32fc8733092fd32cc8ac95139a00377841f59a3f8d8",
-                "sha256:f54a64f8b0c8ff0b64d18aa76675262e1700f3995182267998c31ae974fbc382",
-                "sha256:f5c7150ad32ba43a07c4479f40241756145a1f03b43480e058cfd862bf5041c7",
-                "sha256:f6f824dc3bce0edab5f427efcfb1d63ee75b6fcb7282900ccaf925be84efb0fc",
-                "sha256:fd8a250edc26254fe5b33be00402e6d287f562b6a5b2152dec302fa15bb3e997",
-                "sha256:ffaa5c925128e29efbde7301d8ecaf35c8c60ffbcd6a1ffd3a552177c8e5e796"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
-            "version": "==1.15.0"
+            "markers": "python_version >= '3.6'",
+            "version": "==2023.5.7"
         },
         "cfgv": {
             "hashes": [
                 "sha256:c6a0883f3917a037485059700b9e75da2464e6c27051014ad85ba6aaa5884426",
                 "sha256:f5a830efb9ce7a445376bb66ec94c638a9787422f96264c98edc6bdeed8ab736"
             ],
             "markers": "python_full_version >= '3.6.1'",
             "version": "==3.3.1"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:2857e29ff0d34db842cd7ca3230549d1a697f96ee6d3fb071cfa6c7393832597",
-                "sha256:6881edbebdb17b39b4eaaa821b438bf6eddffb4468cf344f09f89def34a8b1df"
+                "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
+                "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
+                "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
+                "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
+                "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62",
+                "sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230",
+                "sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be",
+                "sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c",
+                "sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0",
+                "sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448",
+                "sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f",
+                "sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649",
+                "sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d",
+                "sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0",
+                "sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706",
+                "sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a",
+                "sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59",
+                "sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23",
+                "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5",
+                "sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb",
+                "sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e",
+                "sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e",
+                "sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c",
+                "sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28",
+                "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d",
+                "sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41",
+                "sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974",
+                "sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce",
+                "sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f",
+                "sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1",
+                "sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d",
+                "sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8",
+                "sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017",
+                "sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31",
+                "sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7",
+                "sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8",
+                "sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e",
+                "sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14",
+                "sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd",
+                "sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d",
+                "sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795",
+                "sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b",
+                "sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b",
+                "sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b",
+                "sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203",
+                "sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f",
+                "sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19",
+                "sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1",
+                "sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a",
+                "sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac",
+                "sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9",
+                "sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0",
+                "sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137",
+                "sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f",
+                "sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6",
+                "sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5",
+                "sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909",
+                "sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f",
+                "sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0",
+                "sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324",
+                "sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755",
+                "sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb",
+                "sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854",
+                "sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c",
+                "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60",
+                "sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84",
+                "sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0",
+                "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b",
+                "sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1",
+                "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
+                "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
+                "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
+                "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
+                "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
+                "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
             ],
-            "markers": "python_version >= '3'",
-            "version": "==2.0.12"
+            "markers": "python_full_version >= '3.7.0'",
+            "version": "==3.1.0"
         },
         "click": {
             "hashes": [
-                "sha256:19a4baa64da924c5e0cd889aba8e947f280309f1a2ce0947a3e3a7bcb7cc72d6",
-                "sha256:977c213473c7665d3aa092b41ff12063227751c41d7b17165013e10069cc5cd2"
+                "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
+                "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
             ],
             "index": "pypi",
-            "version": "==8.1.0"
+            "version": "==8.1.3"
         },
         "colorama": {
             "hashes": [
-                "sha256:5941b2b48a20143d2267e95b1c2a7603ce057ee39fd88e7329b0c292aa16869b",
-                "sha256:9f47eda37229f68eee03b24b9748937c7dc3868f906e8ba69fbcbdd3bc5dc3e2"
+                "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44",
+                "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==0.4.4"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
+            "version": "==0.4.6"
         },
         "coverage": {
             "hashes": [
-                "sha256:03e2a7826086b91ef345ff18742ee9fc47a6839ccd517061ef8fa1976e652ce9",
-                "sha256:07e6db90cd9686c767dcc593dff16c8c09f9814f5e9c51034066cad3373b914d",
-                "sha256:18d520c6860515a771708937d2f78f63cc47ab3b80cb78e86573b0a760161faf",
-                "sha256:1ebf730d2381158ecf3dfd4453fbca0613e16eaa547b4170e2450c9707665ce7",
-                "sha256:21b7745788866028adeb1e0eca3bf1101109e2dc58456cb49d2d9b99a8c516e6",
-                "sha256:26e2deacd414fc2f97dd9f7676ee3eaecd299ca751412d89f40bc01557a6b1b4",
-                "sha256:2c6dbb42f3ad25760010c45191e9757e7dce981cbfb90e42feef301d71540059",
-                "sha256:2fea046bfb455510e05be95e879f0e768d45c10c11509e20e06d8fcaa31d9e39",
-                "sha256:34626a7eee2a3da12af0507780bb51eb52dca0e1751fd1471d0810539cefb536",
-                "sha256:37d1141ad6b2466a7b53a22e08fe76994c2d35a5b6b469590424a9953155afac",
-                "sha256:46191097ebc381fbf89bdce207a6c107ac4ec0890d8d20f3360345ff5976155c",
-                "sha256:4dd8bafa458b5c7d061540f1ee9f18025a68e2d8471b3e858a9dad47c8d41903",
-                "sha256:4e21876082ed887baed0146fe222f861b5815455ada3b33b890f4105d806128d",
-                "sha256:58303469e9a272b4abdb9e302a780072c0633cdcc0165db7eec0f9e32f901e05",
-                "sha256:5ca5aeb4344b30d0bec47481536b8ba1181d50dbe783b0e4ad03c95dc1296684",
-                "sha256:68353fe7cdf91f109fc7d474461b46e7f1f14e533e911a2a2cbb8b0fc8613cf1",
-                "sha256:6f89d05e028d274ce4fa1a86887b071ae1755082ef94a6740238cd7a8178804f",
-                "sha256:7a15dc0a14008f1da3d1ebd44bdda3e357dbabdf5a0b5034d38fcde0b5c234b7",
-                "sha256:8bdde1177f2311ee552f47ae6e5aa7750c0e3291ca6b75f71f7ffe1f1dab3dca",
-                "sha256:8ce257cac556cb03be4a248d92ed36904a59a4a5ff55a994e92214cde15c5bad",
-                "sha256:8cf5cfcb1521dc3255d845d9dca3ff204b3229401994ef8d1984b32746bb45ca",
-                "sha256:8fbbdc8d55990eac1b0919ca69eb5a988a802b854488c34b8f37f3e2025fa90d",
-                "sha256:9548f10d8be799551eb3a9c74bbf2b4934ddb330e08a73320123c07f95cc2d92",
-                "sha256:96f8a1cb43ca1422f36492bebe63312d396491a9165ed3b9231e778d43a7fca4",
-                "sha256:9b27d894748475fa858f9597c0ee1d4829f44683f3813633aaf94b19cb5453cf",
-                "sha256:9baff2a45ae1f17c8078452e9e5962e518eab705e50a0aa8083733ea7d45f3a6",
-                "sha256:a2a8b8bcc399edb4347a5ca8b9b87e7524c0967b335fbb08a83c8421489ddee1",
-                "sha256:acf53bc2cf7282ab9b8ba346746afe703474004d9e566ad164c91a7a59f188a4",
-                "sha256:b0be84e5a6209858a1d3e8d1806c46214e867ce1b0fd32e4ea03f4bd8b2e3359",
-                "sha256:b31651d018b23ec463e95cf10070d0b2c548aa950a03d0b559eaa11c7e5a6fa3",
-                "sha256:b78e5afb39941572209f71866aa0b206c12f0109835aa0d601e41552f9b3e620",
-                "sha256:c76aeef1b95aff3905fb2ae2d96e319caca5b76fa41d3470b19d4e4a3a313512",
-                "sha256:dd035edafefee4d573140a76fdc785dc38829fe5a455c4bb12bac8c20cfc3d69",
-                "sha256:dd6fe30bd519694b356cbfcaca9bd5c1737cddd20778c6a581ae20dc8c04def2",
-                "sha256:e5f4e1edcf57ce94e5475fe09e5afa3e3145081318e5fd1a43a6b4539a97e518",
-                "sha256:ec6bc7fe73a938933d4178c9b23c4e0568e43e220aef9472c4f6044bfc6dd0f0",
-                "sha256:f1555ea6d6da108e1999b2463ea1003fe03f29213e459145e70edbaf3e004aaa",
-                "sha256:f5fa5803f47e095d7ad8443d28b01d48c0359484fec1b9d8606d0e3282084bc4",
-                "sha256:f7331dbf301b7289013175087636bbaf5b2405e57259dd2c42fdcc9fcc47325e",
-                "sha256:f9987b0354b06d4df0f4d3e0ec1ae76d7ce7cbca9a2f98c25041eb79eec766f1",
-                "sha256:fd9e830e9d8d89b20ab1e5af09b32d33e1a08ef4c4e14411e559556fd788e6b2"
+                "sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f",
+                "sha256:06fb182e69f33f6cd1d39a6c597294cff3143554b64b9825d1dc69d18cc2fff2",
+                "sha256:0a5f9e1dbd7fbe30196578ca36f3fba75376fb99888c395c5880b355e2875f8a",
+                "sha256:0e1f928eaf5469c11e886fe0885ad2bf1ec606434e79842a879277895a50942a",
+                "sha256:171717c7cb6b453aebac9a2ef603699da237f341b38eebfee9be75d27dc38e01",
+                "sha256:1e9d683426464e4a252bf70c3498756055016f99ddaec3774bf368e76bbe02b6",
+                "sha256:201e7389591af40950a6480bd9edfa8ed04346ff80002cec1a66cac4549c1ad7",
+                "sha256:245167dd26180ab4c91d5e1496a30be4cd721a5cf2abf52974f965f10f11419f",
+                "sha256:2aee274c46590717f38ae5e4650988d1af340fe06167546cc32fe2f58ed05b02",
+                "sha256:2e07b54284e381531c87f785f613b833569c14ecacdcb85d56b25c4622c16c3c",
+                "sha256:31563e97dae5598556600466ad9beea39fb04e0229e61c12eaa206e0aa202063",
+                "sha256:33d6d3ea29d5b3a1a632b3c4e4f4ecae24ef170b0b9ee493883f2df10039959a",
+                "sha256:3d376df58cc111dc8e21e3b6e24606b5bb5dee6024f46a5abca99124b2229ef5",
+                "sha256:419bfd2caae268623dd469eff96d510a920c90928b60f2073d79f8fe2bbc5959",
+                "sha256:48c19d2159d433ccc99e729ceae7d5293fbffa0bdb94952d3579983d1c8c9d97",
+                "sha256:49969a9f7ffa086d973d91cec8d2e31080436ef0fb4a359cae927e742abfaaa6",
+                "sha256:52edc1a60c0d34afa421c9c37078817b2e67a392cab17d97283b64c5833f427f",
+                "sha256:537891ae8ce59ef63d0123f7ac9e2ae0fc8b72c7ccbe5296fec45fd68967b6c9",
+                "sha256:54b896376ab563bd38453cecb813c295cf347cf5906e8b41d340b0321a5433e5",
+                "sha256:58c2ccc2f00ecb51253cbe5d8d7122a34590fac9646a960d1430d5b15321d95f",
+                "sha256:5b7540161790b2f28143191f5f8ec02fb132660ff175b7747b95dcb77ac26562",
+                "sha256:5baa06420f837184130752b7c5ea0808762083bf3487b5038d68b012e5937dbe",
+                "sha256:5e330fc79bd7207e46c7d7fd2bb4af2963f5f635703925543a70b99574b0fea9",
+                "sha256:61b9a528fb348373c433e8966535074b802c7a5d7f23c4f421e6c6e2f1697a6f",
+                "sha256:63426706118b7f5cf6bb6c895dc215d8a418d5952544042c8a2d9fe87fcf09cb",
+                "sha256:6d040ef7c9859bb11dfeb056ff5b3872436e3b5e401817d87a31e1750b9ae2fb",
+                "sha256:6f48351d66575f535669306aa7d6d6f71bc43372473b54a832222803eb956fd1",
+                "sha256:7ee7d9d4822c8acc74a5e26c50604dff824710bc8de424904c0982e25c39c6cb",
+                "sha256:81c13a1fc7468c40f13420732805a4c38a105d89848b7c10af65a90beff25250",
+                "sha256:8d13c64ee2d33eccf7437961b6ea7ad8673e2be040b4f7fd4fd4d4d28d9ccb1e",
+                "sha256:8de8bb0e5ad103888d65abef8bca41ab93721647590a3f740100cd65c3b00511",
+                "sha256:8fa03bce9bfbeeef9f3b160a8bed39a221d82308b4152b27d82d8daa7041fee5",
+                "sha256:924d94291ca674905fe9481f12294eb11f2d3d3fd1adb20314ba89e94f44ed59",
+                "sha256:975d70ab7e3c80a3fe86001d8751f6778905ec723f5b110aed1e450da9d4b7f2",
+                "sha256:976b9c42fb2a43ebf304fa7d4a310e5f16cc99992f33eced91ef6f908bd8f33d",
+                "sha256:9e31cb64d7de6b6f09702bb27c02d1904b3aebfca610c12772452c4e6c21a0d3",
+                "sha256:a342242fe22407f3c17f4b499276a02b01e80f861f1682ad1d95b04018e0c0d4",
+                "sha256:a3d33a6b3eae87ceaefa91ffdc130b5e8536182cd6dfdbfc1aa56b46ff8c86de",
+                "sha256:a895fcc7b15c3fc72beb43cdcbdf0ddb7d2ebc959edac9cef390b0d14f39f8a9",
+                "sha256:afb17f84d56068a7c29f5fa37bfd38d5aba69e3304af08ee94da8ed5b0865833",
+                "sha256:b1c546aca0ca4d028901d825015dc8e4d56aac4b541877690eb76490f1dc8ed0",
+                "sha256:b29019c76039dc3c0fd815c41392a044ce555d9bcdd38b0fb60fb4cd8e475ba9",
+                "sha256:b46517c02ccd08092f4fa99f24c3b83d8f92f739b4657b0f146246a0ca6a831d",
+                "sha256:b7aa5f8a41217360e600da646004f878250a0d6738bcdc11a0a39928d7dc2050",
+                "sha256:b7b4c971f05e6ae490fef852c218b0e79d4e52f79ef0c8475566584a8fb3e01d",
+                "sha256:ba90a9563ba44a72fda2e85302c3abc71c5589cea608ca16c22b9804262aaeb6",
+                "sha256:cb017fd1b2603ef59e374ba2063f593abe0fc45f2ad9abdde5b4d83bd922a353",
+                "sha256:d22656368f0e6189e24722214ed8d66b8022db19d182927b9a248a2a8a2f67eb",
+                "sha256:d2c2db7fd82e9b72937969bceac4d6ca89660db0a0967614ce2481e81a0b771e",
+                "sha256:d39b5b4f2a66ccae8b7263ac3c8170994b65266797fb96cbbfd3fb5b23921db8",
+                "sha256:d62a5c7dad11015c66fbb9d881bc4caa5b12f16292f857842d9d1871595f4495",
+                "sha256:e7d9405291c6928619403db1d10bd07888888ec1abcbd9748fdaa971d7d661b2",
+                "sha256:e84606b74eb7de6ff581a7915e2dab7a28a0517fbe1c9239eb227e1354064dcd",
+                "sha256:eb393e5ebc85245347950143969b241d08b52b88a3dc39479822e073a1a8eb27",
+                "sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1",
+                "sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818",
+                "sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4",
+                "sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e",
+                "sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850",
+                "sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3"
             ],
             "index": "pypi",
-            "version": "==6.3.2"
+            "version": "==7.2.7"
         },
-        "cryptography": {
+        "distlib": {
             "hashes": [
-                "sha256:0a3bf09bb0b7a2c93ce7b98cb107e9170a90c51a0162a20af1c61c765b90e60b",
-                "sha256:1f64a62b3b75e4005df19d3b5235abd43fa6358d5516cfc43d87aeba8d08dd51",
-                "sha256:32db5cc49c73f39aac27574522cecd0a4bb7384e71198bc65a0d23f901e89bb7",
-                "sha256:4881d09298cd0b669bb15b9cfe6166f16fc1277b4ed0d04a22f3d6430cb30f1d",
-                "sha256:4e2dddd38a5ba733be6a025a1475a9f45e4e41139d1321f412c6b360b19070b6",
-                "sha256:53e0285b49fd0ab6e604f4c5d9c5ddd98de77018542e88366923f152dbeb3c29",
-                "sha256:70f8f4f7bb2ac9f340655cbac89d68c527af5bb4387522a8413e841e3e6628c9",
-                "sha256:7b2d54e787a884ffc6e187262823b6feb06c338084bbe80d45166a1cb1c6c5bf",
-                "sha256:7be666cc4599b415f320839e36367b273db8501127b38316f3b9f22f17a0b815",
-                "sha256:8241cac0aae90b82d6b5c443b853723bcc66963970c67e56e71a2609dc4b5eaf",
-                "sha256:82740818f2f240a5da8dfb8943b360e4f24022b093207160c77cadade47d7c85",
-                "sha256:8897b7b7ec077c819187a123174b645eb680c13df68354ed99f9b40a50898f77",
-                "sha256:c2c5250ff0d36fd58550252f54915776940e4e866f38f3a7866d92b32a654b86",
-                "sha256:ca9f686517ec2c4a4ce930207f75c00bf03d94e5063cbc00a1dc42531511b7eb",
-                "sha256:d2b3d199647468d410994dbeb8cec5816fb74feb9368aedf300af709ef507e3e",
-                "sha256:da73d095f8590ad437cd5e9faf6628a218aa7c387e1fdf67b888b47ba56a17f0",
-                "sha256:e167b6b710c7f7bc54e67ef593f8731e1f45aa35f8a8a7b72d6e42ec76afd4b3",
-                "sha256:ea634401ca02367c1567f012317502ef3437522e2fc44a3ea1844de028fa4b84",
-                "sha256:ec6597aa85ce03f3e507566b8bcdf9da2227ec86c4266bd5e6ab4d9e0cc8dab2",
-                "sha256:f64b232348ee82f13aac22856515ce0195837f6968aeaa94a3d0353ea2ec06a6"
+                "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
+                "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==36.0.2"
+            "version": "==0.3.6"
         },
-        "distlib": {
+        "docutils": {
             "hashes": [
-                "sha256:6564fe0a8f51e734df6333d08b8b94d4ea8ee6b99b5ed50613f731fd4089f34b",
-                "sha256:e4b58818180336dc9c529bfb9a0b58728ffc09ad92027a3f30b7cd91e3458579"
+                "sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6",
+                "sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b"
             ],
-            "version": "==0.3.4"
+            "markers": "python_version >= '3.7'",
+            "version": "==0.20.1"
         },
-        "docutils": {
+        "exceptiongroup": {
             "hashes": [
-                "sha256:686577d2e4c32380bb50cbb22f575ed742d58168cee37e99117a854bcd88f125",
-                "sha256:cf316c8370a737a022b72b56874f6602acf974a37a9fba42ec2876387549fc61"
+                "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e",
+                "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==0.17.1"
+            "markers": "python_version < '3.11'",
+            "version": "==1.1.1"
         },
         "filelock": {
             "hashes": [
-                "sha256:9cd540a9352e432c7246a48fe4e8712b10acb1df2ad1f30e8c070b82ae1fed85",
-                "sha256:f8314284bfffbdcfa0ff3d7992b023d4c628ced6feb957351d4c48d059f56bc0"
+                "sha256:002740518d8aa59a26b0c76e10fb8c6e15eae825d34b6fdf670333fd7b938d81",
+                "sha256:cbb791cdea2a72f23da6ac5b5269ab0a0d161e9ef0100e653b69049a7706d1ec"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.6.0"
+            "version": "==3.12.2"
         },
         "flake8": {
             "hashes": [
-                "sha256:479b1304f72536a55948cb40a32dce8bb0ffe3501e26eaf292c7e60eb5e0428d",
-                "sha256:806e034dda44114815e23c16ef92f95c91e4c71100ff52813adf7132a6ad870d"
+                "sha256:3833794e27ff64ea4e9cf5d410082a8b97ff1a06c16aa3d2027339cd0f1195c7",
+                "sha256:c61007e76655af75e6785a931f452915b371dc48f56efd765247c8fe68f2b181"
             ],
             "index": "pypi",
-            "version": "==4.0.1"
+            "version": "==6.0.0"
         },
         "flake8-bugbear": {
             "hashes": [
-                "sha256:e0dc2a36474490d5b1a2d57f9e4ef570abc09f07cbb712b29802e28a2367ff19",
-                "sha256:ec5ec92195720cee1589315416b844ffa5e82f73a78e65329e8055322df1e939"
+                "sha256:1d9eae6d262a3823765f4579cdab169963d1d2288b02f0f5c6e829b03dded509",
+                "sha256:8631e1071c9d85d24a615f235565c16c9a2ac57add4a14636d331bf9f4ef14fa"
             ],
             "index": "pypi",
-            "version": "==22.3.23"
+            "version": "==23.6.5"
         },
         "flake8-docstrings": {
             "hashes": [
-                "sha256:99cac583d6c7e32dd28bbfbef120a7c0d1b6dde4adb5a9fd441c4227a6534bde",
-                "sha256:9fe7c6a306064af8e62a055c2f61e9eb1da55f84bb39caef2b84ce53708ac34b"
+                "sha256:4c8cc748dc16e6869728699e5d0d685da9a10b0ea718e090b1ba088e67a941af",
+                "sha256:51f2344026da083fc084166a9353f5082b01f72901df422f74b4d953ae88ac75"
             ],
             "index": "pypi",
-            "version": "==1.6.0"
+            "version": "==1.7.0"
         },
         "identify": {
             "hashes": [
-                "sha256:3f3244a559290e7d3deb9e9adc7b33594c1bc85a9dd82e0f1be519bf12a1ec17",
-                "sha256:5f06b14366bd1facb88b00540a1de05b69b310cbc2654db3c7e07fa3a4339323"
+                "sha256:0aac67d5b4812498056d28a9a512a483f5085cc28640b02b258a59dac34301d4",
+                "sha256:986dbfb38b1140e763e413e6feb44cd731faf72d1909543178aa79b0e258265d"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.4.12"
+            "version": "==2.5.24"
         },
         "idna": {
             "hashes": [
-                "sha256:84d9dd047ffa80596e0f246e2eab0b391788b0503584e8945f2368256d2735ff",
-                "sha256:9d643ff0a55b762d5cdb124b8eaa99c66322e2157b69160bc32796e824360e6d"
+                "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
+                "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
-            "markers": "python_version >= '3'",
-            "version": "==3.3"
+            "markers": "python_version >= '3.5'",
+            "version": "==3.4"
         },
         "imagesize": {
             "hashes": [
-                "sha256:1db2f82529e53c3e929e8926a1fa9235aa82d0bd0c580359c67ec31b2fddaa8c",
-                "sha256:cd1750d452385ca327479d45b64d9c7729ecf0b3969a58148298c77092261f9d"
+                "sha256:0d8d18d08f840c19d0ee7ca1fd82490fdc3729b7ac93f49870406ddde8ef8d8b",
+                "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==1.3.0"
+            "version": "==1.4.1"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:1208431ca90a8cca1a6b8af391bb53c1a2db74e5d1cef6ddced95d4b2062edc6",
-                "sha256:ea4c597ebf37142f827b8f39299579e31685c31d3a438b59f469406afd0f2539"
+                "sha256:1aaf550d4f73e5d6783e7acb77aec43d49da8017410afae93822cc9cca98c4d4",
+                "sha256:cb52082e659e97afc5dac71e79de97d8681de3aa07ff18578330904a9d18e5b5"
             ],
-            "markers": "python_version < '3.10'",
-            "version": "==4.11.3"
+            "markers": "python_version >= '3.7'",
+            "version": "==6.7.0"
         },
         "iniconfig": {
             "hashes": [
-                "sha256:011e24c64b7f47f6ebd835bb12a743f2fbe9a26d4cecaa7f53bc4f35ee9da8b3",
-                "sha256:bc3af051d7d14b2ee5ef9969666def0cd1a000e121eaea580d4a313df4b37f32"
+                "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
+                "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
-            "version": "==1.1.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.0.0"
         },
-        "jeepney": {
+        "jaraco.classes": {
             "hashes": [
-                "sha256:1b5a0ea5c0e7b166b2f5895b91a08c14de8915afda4407fb5022a195224958ac",
-                "sha256:fa9e232dfa0c498bd0b8a3a73b8d8a31978304dcef0515adc859d4e096f96f4f"
+                "sha256:2353de3288bc6b82120752201c6b1c1a14b058267fa424ed5ce5984e3b922158",
+                "sha256:89559fa5c1d3c34eff6f631ad80bb21f378dbcbb35dd161fd2c6b93f5be2f98a"
             ],
-            "markers": "sys_platform == 'linux'",
-            "version": "==0.7.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==3.2.3"
         },
         "jinja2": {
             "hashes": [
-                "sha256:539835f51a74a69f41b848a9645dbdc35b4f20a3b601e2d9a7e22947b15ff119",
-                "sha256:640bed4bb501cbd17194b3cace1dc2126f5b619cf068a726b98192a0fde74ae9"
+                "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852",
+                "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.1.1"
+            "version": "==3.1.2"
         },
         "keyring": {
             "hashes": [
-                "sha256:9012508e141a80bd1c0b6778d5c610dd9f8c464d75ac6774248500503f972fb9",
-                "sha256:b0d28928ac3ec8e42ef4cc227822647a19f1d544f21f96457965dc01cf555261"
+                "sha256:4901caaf597bfd3bbd78c9a0c7c4c29fcd8310dab2cffefe749e916b6527acd6",
+                "sha256:ca0746a19ec421219f4d713f848fa297a661a8a8c1504867e55bfb5e09091509"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==23.5.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==24.2.0"
         },
         "livereload": {
             "hashes": [
-                "sha256:776f2f865e59fde56490a56bcc6773b6917366bce0c267c60ee8aaf1a0959869"
+                "sha256:776f2f865e59fde56490a56bcc6773b6917366bce0c267c60ee8aaf1a0959869",
+                "sha256:ad4ac6f53b2d62bb6ce1a5e6e96f1f00976a32348afedcb4b6d68df2a1d346e4"
             ],
             "version": "==2.6.3"
         },
         "markdown-it-py": {
             "hashes": [
-                "sha256:31974138ca8cafbcb62213f4974b29571b940e78364584729233f59b8dfdb8bd",
-                "sha256:7b5c153ae1ab2cde00a33938bce68f3ad5d68fbe363f946de7d28555bed4e08a"
+                "sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1",
+                "sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb"
             ],
-            "markers": "python_version ~= '3.6'",
-            "version": "==2.0.1"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.0.0"
         },
         "markupsafe": {
             "hashes": [
-                "sha256:0212a68688482dc52b2d45013df70d169f542b7394fc744c02a57374a4207003",
-                "sha256:089cf3dbf0cd6c100f02945abeb18484bd1ee57a079aefd52cffd17fba910b88",
-                "sha256:10c1bfff05d95783da83491be968e8fe789263689c02724e0c691933c52994f5",
-                "sha256:33b74d289bd2f5e527beadcaa3f401e0df0a89927c1559c8566c066fa4248ab7",
-                "sha256:3799351e2336dc91ea70b034983ee71cf2f9533cdff7c14c90ea126bfd95d65a",
-                "sha256:3ce11ee3f23f79dbd06fb3d63e2f6af7b12db1d46932fe7bd8afa259a5996603",
-                "sha256:421be9fbf0ffe9ffd7a378aafebbf6f4602d564d34be190fc19a193232fd12b1",
-                "sha256:43093fb83d8343aac0b1baa75516da6092f58f41200907ef92448ecab8825135",
-                "sha256:46d00d6cfecdde84d40e572d63735ef81423ad31184100411e6e3388d405e247",
-                "sha256:4a33dea2b688b3190ee12bd7cfa29d39c9ed176bda40bfa11099a3ce5d3a7ac6",
-                "sha256:4b9fe39a2ccc108a4accc2676e77da025ce383c108593d65cc909add5c3bd601",
-                "sha256:56442863ed2b06d19c37f94d999035e15ee982988920e12a5b4ba29b62ad1f77",
-                "sha256:671cd1187ed5e62818414afe79ed29da836dde67166a9fac6d435873c44fdd02",
-                "sha256:694deca8d702d5db21ec83983ce0bb4b26a578e71fbdbd4fdcd387daa90e4d5e",
-                "sha256:6a074d34ee7a5ce3effbc526b7083ec9731bb3cbf921bbe1d3005d4d2bdb3a63",
-                "sha256:6d0072fea50feec76a4c418096652f2c3238eaa014b2f94aeb1d56a66b41403f",
-                "sha256:6fbf47b5d3728c6aea2abb0589b5d30459e369baa772e0f37a0320185e87c980",
-                "sha256:7f91197cc9e48f989d12e4e6fbc46495c446636dfc81b9ccf50bb0ec74b91d4b",
-                "sha256:86b1f75c4e7c2ac2ccdaec2b9022845dbb81880ca318bb7a0a01fbf7813e3812",
-                "sha256:8dc1c72a69aa7e082593c4a203dcf94ddb74bb5c8a731e4e1eb68d031e8498ff",
-                "sha256:8e3dcf21f367459434c18e71b2a9532d96547aef8a871872a5bd69a715c15f96",
-                "sha256:8e576a51ad59e4bfaac456023a78f6b5e6e7651dcd383bcc3e18d06f9b55d6d1",
-                "sha256:96e37a3dc86e80bf81758c152fe66dbf60ed5eca3d26305edf01892257049925",
-                "sha256:97a68e6ada378df82bc9f16b800ab77cbf4b2fada0081794318520138c088e4a",
-                "sha256:99a2a507ed3ac881b975a2976d59f38c19386d128e7a9a18b7df6fff1fd4c1d6",
-                "sha256:a49907dd8420c5685cfa064a1335b6754b74541bbb3706c259c02ed65b644b3e",
-                "sha256:b09bf97215625a311f669476f44b8b318b075847b49316d3e28c08e41a7a573f",
-                "sha256:b7bd98b796e2b6553da7225aeb61f447f80a1ca64f41d83612e6139ca5213aa4",
-                "sha256:b87db4360013327109564f0e591bd2a3b318547bcef31b468a92ee504d07ae4f",
-                "sha256:bcb3ed405ed3222f9904899563d6fc492ff75cce56cba05e32eff40e6acbeaa3",
-                "sha256:d4306c36ca495956b6d568d276ac11fdd9c30a36f1b6eb928070dc5360b22e1c",
-                "sha256:d5ee4f386140395a2c818d149221149c54849dfcfcb9f1debfe07a8b8bd63f9a",
-                "sha256:dda30ba7e87fbbb7eab1ec9f58678558fd9a6b8b853530e176eabd064da81417",
-                "sha256:e04e26803c9c3851c931eac40c695602c6295b8d432cbe78609649ad9bd2da8a",
-                "sha256:e1c0b87e09fa55a220f058d1d49d3fb8df88fbfab58558f1198e08c1e1de842a",
-                "sha256:e72591e9ecd94d7feb70c1cbd7be7b3ebea3f548870aa91e2732960fa4d57a37",
-                "sha256:e8c843bbcda3a2f1e3c2ab25913c80a3c5376cd00c6e8c4a86a89a28c8dc5452",
-                "sha256:efc1913fd2ca4f334418481c7e595c00aad186563bbc1ec76067848c7ca0a933",
-                "sha256:f121a1420d4e173a5d96e47e9a0c0dcff965afdf1626d28de1460815f7c4ee7a",
-                "sha256:fc7b548b17d238737688817ab67deebb30e8073c95749d55538ed473130ec0c7"
+                "sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e",
+                "sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e",
+                "sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431",
+                "sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686",
+                "sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559",
+                "sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc",
+                "sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c",
+                "sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0",
+                "sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4",
+                "sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9",
+                "sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575",
+                "sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba",
+                "sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d",
+                "sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3",
+                "sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00",
+                "sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155",
+                "sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac",
+                "sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52",
+                "sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f",
+                "sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8",
+                "sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b",
+                "sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24",
+                "sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea",
+                "sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198",
+                "sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0",
+                "sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee",
+                "sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be",
+                "sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2",
+                "sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707",
+                "sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6",
+                "sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58",
+                "sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779",
+                "sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636",
+                "sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c",
+                "sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad",
+                "sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee",
+                "sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc",
+                "sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2",
+                "sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48",
+                "sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7",
+                "sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e",
+                "sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b",
+                "sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa",
+                "sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5",
+                "sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e",
+                "sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb",
+                "sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9",
+                "sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57",
+                "sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc",
+                "sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.1.1"
+            "version": "==2.1.3"
         },
         "mccabe": {
             "hashes": [
-                "sha256:ab8a6258860da4b6677da4bd2fe5dc2c659cff31b3ee4f7f5d64e79735b80d42",
-                "sha256:dd8d182285a0fe56bace7f45b5e7d1a6ebcbf524e8f3bd87eb0f125271b8831f"
+                "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325",
+                "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
-            "version": "==0.6.1"
+            "markers": "python_version >= '3.6'",
+            "version": "==0.7.0"
         },
         "mdit-py-plugins": {
             "hashes": [
-                "sha256:b1279701cee2dbf50e188d3da5f51fee8d78d038cdf99be57c6b9d1aa93b4073",
-                "sha256:ecc24f51eeec6ab7eecc2f9724e8272c2fb191c2e93cf98109120c2cace69750"
+                "sha256:b51b3bb70691f57f974e257e367107857a93b36f322a9e6d44ca5bf28ec2def9",
+                "sha256:d8ab27e9aed6c38aa716819fedfde15ca275715955f8a185a8e1cf90fb1d2c1b"
             ],
-            "markers": "python_version ~= '3.6'",
-            "version": "==0.3.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==0.4.0"
         },
         "mdurl": {
             "hashes": [
-                "sha256:40654d6dcb8d21501ed13c21cc0bd6fc42ff07ceb8be30029e5ae63ebc2ecfda",
-                "sha256:94873a969008ee48880fb21bad7de0349fef529f3be178969af5817239e9b990"
+                "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8",
+                "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==0.1.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==0.1.2"
+        },
+        "more-itertools": {
+            "hashes": [
+                "sha256:cabaa341ad0389ea83c17a94566a53ae4c9d07349861ecb14dc6d0345cf9ac5d",
+                "sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==9.1.0"
         },
         "multidict": {
             "hashes": [
-                "sha256:0327292e745a880459ef71be14e709aaea2f783f3537588fb4ed09b6c01bca60",
-                "sha256:041b81a5f6b38244b34dc18c7b6aba91f9cdaf854d9a39e5ff0b58e2b5773b9c",
-                "sha256:0556a1d4ea2d949efe5fd76a09b4a82e3a4a30700553a6725535098d8d9fb672",
-                "sha256:05f6949d6169878a03e607a21e3b862eaf8e356590e8bdae4227eedadacf6e51",
-                "sha256:07a017cfa00c9890011628eab2503bee5872f27144936a52eaab449be5eaf032",
-                "sha256:0b9e95a740109c6047602f4db4da9949e6c5945cefbad34a1299775ddc9a62e2",
-                "sha256:19adcfc2a7197cdc3987044e3f415168fc5dc1f720c932eb1ef4f71a2067e08b",
-                "sha256:19d9bad105dfb34eb539c97b132057a4e709919ec4dd883ece5838bcbf262b80",
-                "sha256:225383a6603c086e6cef0f2f05564acb4f4d5f019a4e3e983f572b8530f70c88",
-                "sha256:23b616fdc3c74c9fe01d76ce0d1ce872d2d396d8fa8e4899398ad64fb5aa214a",
-                "sha256:2957489cba47c2539a8eb7ab32ff49101439ccf78eab724c828c1a54ff3ff98d",
-                "sha256:2d36e929d7f6a16d4eb11b250719c39560dd70545356365b494249e2186bc389",
-                "sha256:2e4a0785b84fb59e43c18a015ffc575ba93f7d1dbd272b4cdad9f5134b8a006c",
-                "sha256:3368bf2398b0e0fcbf46d85795adc4c259299fec50c1416d0f77c0a843a3eed9",
-                "sha256:373ba9d1d061c76462d74e7de1c0c8e267e9791ee8cfefcf6b0b2495762c370c",
-                "sha256:4070613ea2227da2bfb2c35a6041e4371b0af6b0be57f424fe2318b42a748516",
-                "sha256:45183c96ddf61bf96d2684d9fbaf6f3564d86b34cb125761f9a0ef9e36c1d55b",
-                "sha256:4571f1beddff25f3e925eea34268422622963cd8dc395bb8778eb28418248e43",
-                "sha256:47e6a7e923e9cada7c139531feac59448f1f47727a79076c0b1ee80274cd8eee",
-                "sha256:47fbeedbf94bed6547d3aa632075d804867a352d86688c04e606971595460227",
-                "sha256:497988d6b6ec6ed6f87030ec03280b696ca47dbf0648045e4e1d28b80346560d",
-                "sha256:4bae31803d708f6f15fd98be6a6ac0b6958fcf68fda3c77a048a4f9073704aae",
-                "sha256:50bd442726e288e884f7be9071016c15a8742eb689a593a0cac49ea093eef0a7",
-                "sha256:514fe2b8d750d6cdb4712346a2c5084a80220821a3e91f3f71eec11cf8d28fd4",
-                "sha256:5774d9218d77befa7b70d836004a768fb9aa4fdb53c97498f4d8d3f67bb9cfa9",
-                "sha256:5fdda29a3c7e76a064f2477c9aab1ba96fd94e02e386f1e665bca1807fc5386f",
-                "sha256:5ff3bd75f38e4c43f1f470f2df7a4d430b821c4ce22be384e1459cb57d6bb013",
-                "sha256:626fe10ac87851f4cffecee161fc6f8f9853f0f6f1035b59337a51d29ff3b4f9",
-                "sha256:6701bf8a5d03a43375909ac91b6980aea74b0f5402fbe9428fc3f6edf5d9677e",
-                "sha256:684133b1e1fe91eda8fa7447f137c9490a064c6b7f392aa857bba83a28cfb693",
-                "sha256:6f3cdef8a247d1eafa649085812f8a310e728bdf3900ff6c434eafb2d443b23a",
-                "sha256:75bdf08716edde767b09e76829db8c1e5ca9d8bb0a8d4bd94ae1eafe3dac5e15",
-                "sha256:7c40b7bbece294ae3a87c1bc2abff0ff9beef41d14188cda94ada7bcea99b0fb",
-                "sha256:8004dca28e15b86d1b1372515f32eb6f814bdf6f00952699bdeb541691091f96",
-                "sha256:8064b7c6f0af936a741ea1efd18690bacfbae4078c0c385d7c3f611d11f0cf87",
-                "sha256:89171b2c769e03a953d5969b2f272efa931426355b6c0cb508022976a17fd376",
-                "sha256:8cbf0132f3de7cc6c6ce00147cc78e6439ea736cee6bca4f068bcf892b0fd658",
-                "sha256:9cc57c68cb9139c7cd6fc39f211b02198e69fb90ce4bc4a094cf5fe0d20fd8b0",
-                "sha256:a007b1638e148c3cfb6bf0bdc4f82776cef0ac487191d093cdc316905e504071",
-                "sha256:a2c34a93e1d2aa35fbf1485e5010337c72c6791407d03aa5f4eed920343dd360",
-                "sha256:a45e1135cb07086833ce969555df39149680e5471c04dfd6a915abd2fc3f6dbc",
-                "sha256:ac0e27844758d7177989ce406acc6a83c16ed4524ebc363c1f748cba184d89d3",
-                "sha256:aef9cc3d9c7d63d924adac329c33835e0243b5052a6dfcbf7732a921c6e918ba",
-                "sha256:b9d153e7f1f9ba0b23ad1568b3b9e17301e23b042c23870f9ee0522dc5cc79e8",
-                "sha256:bfba7c6d5d7c9099ba21f84662b037a0ffd4a5e6b26ac07d19e423e6fdf965a9",
-                "sha256:c207fff63adcdf5a485969131dc70e4b194327666b7e8a87a97fbc4fd80a53b2",
-                "sha256:d0509e469d48940147e1235d994cd849a8f8195e0bca65f8f5439c56e17872a3",
-                "sha256:d16cce709ebfadc91278a1c005e3c17dd5f71f5098bfae1035149785ea6e9c68",
-                "sha256:d48b8ee1d4068561ce8033d2c344cf5232cb29ee1a0206a7b828c79cbc5982b8",
-                "sha256:de989b195c3d636ba000ee4281cd03bb1234635b124bf4cd89eeee9ca8fcb09d",
-                "sha256:e07c8e79d6e6fd37b42f3250dba122053fddb319e84b55dd3a8d6446e1a7ee49",
-                "sha256:e2c2e459f7050aeb7c1b1276763364884595d47000c1cddb51764c0d8976e608",
-                "sha256:e5b20e9599ba74391ca0cfbd7b328fcc20976823ba19bc573983a25b32e92b57",
-                "sha256:e875b6086e325bab7e680e4316d667fc0e5e174bb5611eb16b3ea121c8951b86",
-                "sha256:f4f052ee022928d34fe1f4d2bc743f32609fb79ed9c49a1710a5ad6b2198db20",
-                "sha256:fcb91630817aa8b9bc4a74023e4198480587269c272c58b3279875ed7235c293",
-                "sha256:fd9fc9c4849a07f3635ccffa895d57abce554b467d611a5009ba4f39b78a8849",
-                "sha256:feba80698173761cddd814fa22e88b0661e98cb810f9f986c54aa34d281e4937",
-                "sha256:feea820722e69451743a3d56ad74948b68bf456984d63c1a92e8347b7b88452d"
+                "sha256:01a3a55bd90018c9c080fbb0b9f4891db37d148a0a18722b42f94694f8b6d4c9",
+                "sha256:0b1a97283e0c85772d613878028fec909f003993e1007eafa715b24b377cb9b8",
+                "sha256:0dfad7a5a1e39c53ed00d2dd0c2e36aed4650936dc18fd9a1826a5ae1cad6f03",
+                "sha256:11bdf3f5e1518b24530b8241529d2050014c884cf18b6fc69c0c2b30ca248710",
+                "sha256:1502e24330eb681bdaa3eb70d6358e818e8e8f908a22a1851dfd4e15bc2f8161",
+                "sha256:16ab77bbeb596e14212e7bab8429f24c1579234a3a462105cda4a66904998664",
+                "sha256:16d232d4e5396c2efbbf4f6d4df89bfa905eb0d4dc5b3549d872ab898451f569",
+                "sha256:21a12c4eb6ddc9952c415f24eef97e3e55ba3af61f67c7bc388dcdec1404a067",
+                "sha256:27c523fbfbdfd19c6867af7346332b62b586eed663887392cff78d614f9ec313",
+                "sha256:281af09f488903fde97923c7744bb001a9b23b039a909460d0f14edc7bf59706",
+                "sha256:33029f5734336aa0d4c0384525da0387ef89148dc7191aae00ca5fb23d7aafc2",
+                "sha256:3601a3cece3819534b11d4efc1eb76047488fddd0c85a3948099d5da4d504636",
+                "sha256:3666906492efb76453c0e7b97f2cf459b0682e7402c0489a95484965dbc1da49",
+                "sha256:36c63aaa167f6c6b04ef2c85704e93af16c11d20de1d133e39de6a0e84582a93",
+                "sha256:39ff62e7d0f26c248b15e364517a72932a611a9b75f35b45be078d81bdb86603",
+                "sha256:43644e38f42e3af682690876cff722d301ac585c5b9e1eacc013b7a3f7b696a0",
+                "sha256:4372381634485bec7e46718edc71528024fcdc6f835baefe517b34a33c731d60",
+                "sha256:458f37be2d9e4c95e2d8866a851663cbc76e865b78395090786f6cd9b3bbf4f4",
+                "sha256:45e1ecb0379bfaab5eef059f50115b54571acfbe422a14f668fc8c27ba410e7e",
+                "sha256:4b9d9e4e2b37daddb5c23ea33a3417901fa7c7b3dee2d855f63ee67a0b21e5b1",
+                "sha256:4ceef517eca3e03c1cceb22030a3e39cb399ac86bff4e426d4fc6ae49052cc60",
+                "sha256:4d1a3d7ef5e96b1c9e92f973e43aa5e5b96c659c9bc3124acbbd81b0b9c8a951",
+                "sha256:4dcbb0906e38440fa3e325df2359ac6cb043df8e58c965bb45f4e406ecb162cc",
+                "sha256:509eac6cf09c794aa27bcacfd4d62c885cce62bef7b2c3e8b2e49d365b5003fe",
+                "sha256:52509b5be062d9eafc8170e53026fbc54cf3b32759a23d07fd935fb04fc22d95",
+                "sha256:52f2dffc8acaba9a2f27174c41c9e57f60b907bb9f096b36b1a1f3be71c6284d",
+                "sha256:574b7eae1ab267e5f8285f0fe881f17efe4b98c39a40858247720935b893bba8",
+                "sha256:5979b5632c3e3534e42ca6ff856bb24b2e3071b37861c2c727ce220d80eee9ed",
+                "sha256:59d43b61c59d82f2effb39a93c48b845efe23a3852d201ed2d24ba830d0b4cf2",
+                "sha256:5a4dcf02b908c3b8b17a45fb0f15b695bf117a67b76b7ad18b73cf8e92608775",
+                "sha256:5cad9430ab3e2e4fa4a2ef4450f548768400a2ac635841bc2a56a2052cdbeb87",
+                "sha256:5fc1b16f586f049820c5c5b17bb4ee7583092fa0d1c4e28b5239181ff9532e0c",
+                "sha256:62501642008a8b9871ddfccbf83e4222cf8ac0d5aeedf73da36153ef2ec222d2",
+                "sha256:64bdf1086b6043bf519869678f5f2757f473dee970d7abf6da91ec00acb9cb98",
+                "sha256:64da238a09d6039e3bd39bb3aee9c21a5e34f28bfa5aa22518581f910ff94af3",
+                "sha256:666daae833559deb2d609afa4490b85830ab0dfca811a98b70a205621a6109fe",
+                "sha256:67040058f37a2a51ed8ea8f6b0e6ee5bd78ca67f169ce6122f3e2ec80dfe9b78",
+                "sha256:6748717bb10339c4760c1e63da040f5f29f5ed6e59d76daee30305894069a660",
+                "sha256:6b181d8c23da913d4ff585afd1155a0e1194c0b50c54fcfe286f70cdaf2b7176",
+                "sha256:6ed5f161328b7df384d71b07317f4d8656434e34591f20552c7bcef27b0ab88e",
+                "sha256:7582a1d1030e15422262de9f58711774e02fa80df0d1578995c76214f6954988",
+                "sha256:7d18748f2d30f94f498e852c67d61261c643b349b9d2a581131725595c45ec6c",
+                "sha256:7d6ae9d593ef8641544d6263c7fa6408cc90370c8cb2bbb65f8d43e5b0351d9c",
+                "sha256:81a4f0b34bd92df3da93315c6a59034df95866014ac08535fc819f043bfd51f0",
+                "sha256:8316a77808c501004802f9beebde51c9f857054a0c871bd6da8280e718444449",
+                "sha256:853888594621e6604c978ce2a0444a1e6e70c8d253ab65ba11657659dcc9100f",
+                "sha256:99b76c052e9f1bc0721f7541e5e8c05db3941eb9ebe7b8553c625ef88d6eefde",
+                "sha256:a2e4369eb3d47d2034032a26c7a80fcb21a2cb22e1173d761a162f11e562caa5",
+                "sha256:ab55edc2e84460694295f401215f4a58597f8f7c9466faec545093045476327d",
+                "sha256:af048912e045a2dc732847d33821a9d84ba553f5c5f028adbd364dd4765092ac",
+                "sha256:b1a2eeedcead3a41694130495593a559a668f382eee0727352b9a41e1c45759a",
+                "sha256:b1e8b901e607795ec06c9e42530788c45ac21ef3aaa11dbd0c69de543bfb79a9",
+                "sha256:b41156839806aecb3641f3208c0dafd3ac7775b9c4c422d82ee2a45c34ba81ca",
+                "sha256:b692f419760c0e65d060959df05f2a531945af31fda0c8a3b3195d4efd06de11",
+                "sha256:bc779e9e6f7fda81b3f9aa58e3a6091d49ad528b11ed19f6621408806204ad35",
+                "sha256:bf6774e60d67a9efe02b3616fee22441d86fab4c6d335f9d2051d19d90a40063",
+                "sha256:c048099e4c9e9d615545e2001d3d8a4380bd403e1a0578734e0d31703d1b0c0b",
+                "sha256:c5cb09abb18c1ea940fb99360ea0396f34d46566f157122c92dfa069d3e0e982",
+                "sha256:cc8e1d0c705233c5dd0c5e6460fbad7827d5d36f310a0fadfd45cc3029762258",
+                "sha256:d5e3fc56f88cc98ef8139255cf8cd63eb2c586531e43310ff859d6bb3a6b51f1",
+                "sha256:d6aa0418fcc838522256761b3415822626f866758ee0bc6632c9486b179d0b52",
+                "sha256:d6c254ba6e45d8e72739281ebc46ea5eb5f101234f3ce171f0e9f5cc86991480",
+                "sha256:d6d635d5209b82a3492508cf5b365f3446afb65ae7ebd755e70e18f287b0adf7",
+                "sha256:dcfe792765fab89c365123c81046ad4103fcabbc4f56d1c1997e6715e8015461",
+                "sha256:ddd3915998d93fbcd2566ddf9cf62cdb35c9e093075f862935573d265cf8f65d",
+                "sha256:ddff9c4e225a63a5afab9dd15590432c22e8057e1a9a13d28ed128ecf047bbdc",
+                "sha256:e41b7e2b59679edfa309e8db64fdf22399eec4b0b24694e1b2104fb789207779",
+                "sha256:e69924bfcdda39b722ef4d9aa762b2dd38e4632b3641b1d9a57ca9cd18f2f83a",
+                "sha256:ea20853c6dbbb53ed34cb4d080382169b6f4554d394015f1bef35e881bf83547",
+                "sha256:ee2a1ece51b9b9e7752e742cfb661d2a29e7bcdba2d27e66e28a99f1890e4fa0",
+                "sha256:eeb6dcc05e911516ae3d1f207d4b0520d07f54484c49dfc294d6e7d63b734171",
+                "sha256:f70b98cd94886b49d91170ef23ec5c0e8ebb6f242d734ed7ed677b24d50c82cf",
+                "sha256:fc35cb4676846ef752816d5be2193a1e8367b4c1397b74a565a9d0389c433a1d",
+                "sha256:ff959bee35038c4624250473988b24f846cbeb2c6639de3602c073f10410ceba"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==6.0.2"
+            "version": "==6.0.4"
         },
         "mypy": {
             "hashes": [
-                "sha256:0e2dd88410937423fba18e57147dd07cd8381291b93d5b1984626f173a26543e",
-                "sha256:10daab80bc40f84e3f087d896cdb53dc811a9f04eae4b3f95779c26edee89d16",
-                "sha256:17e44649fec92e9f82102b48a3bf7b4a5510ad0cd22fa21a104826b5db4903e2",
-                "sha256:1a0459c333f00e6a11cbf6b468b870c2b99a906cb72d6eadf3d1d95d38c9352c",
-                "sha256:246e1aa127d5b78488a4a0594bd95f6d6fb9d63cf08a66dafbff8595d8891f67",
-                "sha256:2b184db8c618c43c3a31b32ff00cd28195d39e9c24e7c3b401f3db7f6e5767f5",
-                "sha256:2bc249409a7168d37c658e062e1ab5173300984a2dada2589638568ddc1db02b",
-                "sha256:3841b5433ff936bff2f4dc8d54cf2cdbfea5d8e88cedfac45c161368e5770ba6",
-                "sha256:4c3e497588afccfa4334a9986b56f703e75793133c4be3a02d06a3df16b67a58",
-                "sha256:5bf44840fb43ac4074636fd47ee476d73f0039f4f54e86d7265077dc199be24d",
-                "sha256:64235137edc16bee6f095aba73be5334677d6f6bdb7fa03cfab90164fa294a17",
-                "sha256:6776e5fa22381cc761df53e7496a805801c1a751b27b99a9ff2f0ca848c7eca0",
-                "sha256:6ce34a118d1a898f47def970a2042b8af6bdcc01546454726c7dd2171aa6dfca",
-                "sha256:6f6ad963172152e112b87cc7ec103ba0f2db2f1cd8997237827c052a3903eaa6",
-                "sha256:6f7106cbf9cc2f403693bf50ed7c9fa5bb3dfa9007b240db3c910929abe2a322",
-                "sha256:7742d2c4e46bb5017b51c810283a6a389296cda03df805a4f7869a6f41246534",
-                "sha256:9521c1265ccaaa1791d2c13582f06facf815f426cd8b07c3a485f486a8ffc1f3",
-                "sha256:a1b383fe99678d7402754fe90448d4037f9512ce70c21f8aee3b8bf48ffc51db",
-                "sha256:b840cfe89c4ab6386c40300689cd8645fc8d2d5f20101c7f8bd23d15fca14904",
-                "sha256:d8d3ba77e56b84cd47a8ee45b62c84b6d80d32383928fe2548c9a124ea0a725c",
-                "sha256:dcd955f36e0180258a96f880348fbca54ce092b40fbb4b37372ae3b25a0b0a46",
-                "sha256:e865fec858d75b78b4d63266c9aff770ecb6a39dfb6d6b56c47f7f8aba6baba8",
-                "sha256:edf7237137a1a9330046dbb14796963d734dd740a98d5e144a3eb1d267f5f9ee"
+                "sha256:01fd2e9f85622d981fd9063bfaef1aed6e336eaacca00892cd2d82801ab7c042",
+                "sha256:0dde1d180cd84f0624c5dcaaa89c89775550a675aff96b5848de78fb11adabcd",
+                "sha256:141dedfdbfe8a04142881ff30ce6e6653c9685b354876b12e4fe6c78598b45e2",
+                "sha256:16f0db5b641ba159eff72cff08edc3875f2b62b2fa2bc24f68c1e7a4e8232d01",
+                "sha256:190b6bab0302cec4e9e6767d3eb66085aef2a1cc98fe04936d8a42ed2ba77bb7",
+                "sha256:2460a58faeea905aeb1b9b36f5065f2dc9a9c6e4c992a6499a2360c6c74ceca3",
+                "sha256:34a9239d5b3502c17f07fd7c0b2ae6b7dd7d7f6af35fbb5072c6208e76295816",
+                "sha256:43b592511672017f5b1a483527fd2684347fdffc041c9ef53428c8dc530f79a3",
+                "sha256:43d24f6437925ce50139a310a64b2ab048cb2d3694c84c71c3f2a1626d8101dc",
+                "sha256:45d32cec14e7b97af848bddd97d85ea4f0db4d5a149ed9676caa4eb2f7402bb4",
+                "sha256:470c969bb3f9a9efcedbadcd19a74ffb34a25f8e6b0e02dae7c0e71f8372f97b",
+                "sha256:566e72b0cd6598503e48ea610e0052d1b8168e60a46e0bfd34b3acf2d57f96a8",
+                "sha256:5703097c4936bbb9e9bce41478c8d08edd2865e177dc4c52be759f81ee4dd26c",
+                "sha256:7549fbf655e5825d787bbc9ecf6028731973f78088fbca3a1f4145c39ef09462",
+                "sha256:8207b7105829eca6f3d774f64a904190bb2231de91b8b186d21ffd98005f14a7",
+                "sha256:8c4d8e89aa7de683e2056a581ce63c46a0c41e31bd2b6d34144e2c80f5ea53dc",
+                "sha256:98324ec3ecf12296e6422939e54763faedbfcc502ea4a4c38502082711867258",
+                "sha256:9bbcd9ab8ea1f2e1c8031c21445b511442cc45c89951e49bbf852cbb70755b1b",
+                "sha256:9d40652cc4fe33871ad3338581dca3297ff5f2213d0df345bcfbde5162abf0c9",
+                "sha256:a2746d69a8196698146a3dbe29104f9eb6a2a4d8a27878d92169a6c0b74435b6",
+                "sha256:ae704dcfaa180ff7c4cfbad23e74321a2b774f92ca77fd94ce1049175a21c97f",
+                "sha256:bfdca17c36ae01a21274a3c387a63aa1aafe72bff976522886869ef131b937f1",
+                "sha256:c482e1246726616088532b5e964e39765b6d1520791348e6c9dc3af25b233828",
+                "sha256:ca637024ca67ab24a7fd6f65d280572c3794665eaf5edcc7e90a866544076878",
+                "sha256:e02d700ec8d9b1859790c0475df4e4092c7bf3272a4fd2c9f33d87fac4427b8f",
+                "sha256:e5952d2d18b79f7dc25e62e014fe5a23eb1a3d2bc66318df8988a01b1a037c5b"
             ],
             "index": "pypi",
-            "version": "==0.942"
+            "version": "==1.4.1"
         },
         "mypy-extensions": {
             "hashes": [
-                "sha256:090fedd75945a69ae91ce1303b5824f428daf5a028d2f6ab8a299250a846f15d",
-                "sha256:2d82818f5bb3e369420cb3c4060a7970edba416647068eb4c5343488a6c604a8"
+                "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
+                "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
-            "version": "==0.4.3"
+            "markers": "python_version >= '3.5'",
+            "version": "==1.0.0"
         },
         "myst-parser": {
             "hashes": [
-                "sha256:555ec2950aba5ae5dac5c162c7e9a43ad4a7291cfac644d8f5f84da8efa6f356",
-                "sha256:d412347a5cacb77ebc03d7f7ffef050cd61957d46f234313d350e84e24972260"
+                "sha256:7c36344ae39c8e740dad7fdabf5aa6fc4897a813083c6cc9990044eb93656b14",
+                "sha256:ea929a67a6a0b1683cdbe19b8d2e724cd7643f8aa3e7bb18dd65beac3483bead"
             ],
             "index": "pypi",
-            "version": "==0.17.0"
+            "version": "==2.0.0"
         },
         "nodeenv": {
             "hashes": [
-                "sha256:3ef13ff90291ba2a4a7a4ff9a979b63ffdd00a464dbe04acf0ea6471517a4c2b",
-                "sha256:621e6b7076565ddcacd2db0294c0381e01fd28945ab36bcf00f41c5daf63bef7"
+                "sha256:d51e0c37e64fbf47d017feac3145cdbb58836d7eee8c6f6d3b6880c5456227d2",
+                "sha256:df865724bb3c3adc86b3876fa209771517b0cfe596beff01a92700e0e8be4cec"
             ],
-            "version": "==1.6.0"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
+            "version": "==1.8.0"
         },
         "packaging": {
             "hashes": [
-                "sha256:dd47c42927d89ab911e606518907cc2d3a1f38bbd026385970643f9c5b8ecfeb",
-                "sha256:ef103e05f519cdc783ae24ea4e2e0f508a9c99b2d4969652eed6a2e1ea5bd522"
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==21.3"
+            "markers": "python_version >= '3.7'",
+            "version": "==23.1"
         },
         "pathspec": {
             "hashes": [
-                "sha256:7d15c4ddb0b5c802d161efc417ec1a2558ea2653c2e8ad9c19098201dc1c993a",
-                "sha256:e564499435a2673d586f6b2130bb5b95f04a3ba06f81b8f895b651a3c76aabb1"
+                "sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687",
+                "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"
             ],
-            "version": "==0.9.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==0.11.1"
         },
         "pkginfo": {
             "hashes": [
-                "sha256:542e0d0b6750e2e21c20179803e40ab50598d8066d51097a0e382cba9eb02bff",
-                "sha256:c24c487c6a7f72c66e816ab1796b96ac6c3d14d49338293d2141664330b55ffc"
+                "sha256:4b7a555a6d5a22169fcc9cf7bfd78d296b0361adad412a346c1226849af5e546",
+                "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
             ],
-            "version": "==1.8.2"
+            "markers": "python_version >= '3.6'",
+            "version": "==1.9.6"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:7535e70dfa32e84d4b34996ea99c5e432fa29a708d0f4e394bbcb2a8faa4f16d",
-                "sha256:bcae7cab893c2d310a711b70b24efb93334febe65f8de776ee320b517471e227"
+                "sha256:b0cabcb11063d21a0b261d557acb0a9d2126350e63b70cdf7db6347baea456dc",
+                "sha256:ca9ed98ce73076ba72e092b23d3c93ea6c4e186b3f1c3dad6edd98ff6ffcca2e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.5.1"
+            "version": "==3.8.0"
         },
         "pluggy": {
             "hashes": [
-                "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
-                "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
+                "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849",
+                "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==1.0.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==1.2.0"
         },
         "pockets": {
             "hashes": [
                 "sha256:68597934193c08a08eb2bf6a1d85593f627c22f9b065cc727a4f03f669d96d86",
                 "sha256:9320f1a3c6f7a9133fe3b571f283bcf3353cd70249025ae8d618e40e9f7e92b3"
             ],
             "version": "==0.9.1"
         },
         "pre-commit": {
             "hashes": [
-                "sha256:725fa7459782d7bec5ead072810e47351de01709be838c2ce1726b9591dad616",
-                "sha256:c1a8040ff15ad3d648c70cc3e55b93e4d2d5b687320955505587fd79bbaed06a"
+                "sha256:10badb65d6a38caff29703362271d7dca483d01da88f9d7e05d0b97171c136cb",
+                "sha256:a2256f489cd913d575c145132ae196fe335da32d91a8294b7afe6622335dd023"
             ],
             "index": "pypi",
-            "version": "==2.17.0"
-        },
-        "py": {
-            "hashes": [
-                "sha256:51c75c4126074b472f746a24399ad32f6053d1b34b68d2fa41e558e6f4a98719",
-                "sha256:607c53218732647dff4acdfcd50cb62615cedf612e72d1724fb1a0cc6405b378"
-            ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==1.11.0"
+            "version": "==3.3.3"
         },
         "pycodestyle": {
             "hashes": [
-                "sha256:720f8b39dde8b293825e7ff02c475f3077124006db4f440dcbc9a20b76548a20",
-                "sha256:eddd5847ef438ea1c7870ca7eb78a9d47ce0cdb4851a5523949f2601d0cbbe7f"
+                "sha256:347187bdb476329d98f695c213d7295a846d1152ff4fe9bacb8a9590b8ee7053",
+                "sha256:8a4eaf0d0495c7395bdab3589ac2db602797d76207242c17d470186815706610"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==2.8.0"
-        },
-        "pycparser": {
-            "hashes": [
-                "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
-                "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
-            ],
-            "version": "==2.21"
+            "markers": "python_version >= '3.6'",
+            "version": "==2.10.0"
         },
         "pydocstyle": {
             "hashes": [
-                "sha256:1d41b7c459ba0ee6c345f2eb9ae827cab14a7533a88c5c6f7e94923f72df92dc",
-                "sha256:6987826d6775056839940041beef5c08cc7e3d71d63149b48e36727f70144dc4"
+                "sha256:118762d452a49d6b05e194ef344a55822987a462831ade91ec5c06fd2169d019",
+                "sha256:7ce43f0c0ac87b07494eb9c0b462c0b73e6ff276807f204d6b53edc72b7e44e1"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==6.1.1"
+            "version": "==6.3.0"
         },
         "pyflakes": {
             "hashes": [
-                "sha256:05a85c2872edf37a4ed30b0cce2f6093e1d0581f8c19d7393122da7e25b2b24c",
-                "sha256:3bb3a3f256f4b7968c9c788781e4ff07dce46bdf12339dcda61053375426ee2e"
+                "sha256:ec55bf7fe21fff7f1ad2f7da62363d749e2a470500eab1b555334b67aa1ef8cf",
+                "sha256:ec8b276a6b60bd80defed25add7e439881c19e64850afd9b346283d4165fd0fd"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==2.4.0"
+            "markers": "python_version >= '3.6'",
+            "version": "==3.0.1"
         },
         "pygments": {
             "hashes": [
-                "sha256:44238f1b60a76d78fc8ca0528ee429702aae011c265fe6a8dd8b63049ae41c65",
-                "sha256:4e426f72023d88d03b2fa258de560726ce890ff3b630f88c21cbb8b2503b8c6a"
+                "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
+                "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
-            "markers": "python_version >= '3.5'",
-            "version": "==2.11.2"
-        },
-        "pyparsing": {
-            "hashes": [
-                "sha256:18ee9022775d270c55187733956460083db60b37d0d0fb357445f3094eed3eea",
-                "sha256:a6c06a88f252e6c322f65faf8f418b16213b51bdfaece0524c1c1bc30c63c484"
-            ],
-            "markers": "python_version >= '3.6'",
-            "version": "==3.0.7"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.15.1"
         },
         "pytest": {
             "hashes": [
-                "sha256:841132caef6b1ad17a9afde46dc4f6cfa59a05f9555aae5151f73bdf2820ca63",
-                "sha256:92f723789a8fdd7180b6b06483874feca4c48a5c76968e03bb3e7f806a1869ea"
+                "sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32",
+                "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"
             ],
             "index": "pypi",
-            "version": "==7.1.1"
+            "version": "==7.4.0"
         },
         "pytest-vcr": {
             "hashes": [
                 "sha256:23ee51b75abbcc43d926272773aae4f39f93aceb75ed56852d0bf618f92e1896",
                 "sha256:2f316e0539399bea0296e8b8401145c62b6f85e9066af7e57b6151481b0d6d9c"
             ],
             "index": "pypi",
             "version": "==1.0.2"
         },
-        "pytz": {
-            "hashes": [
-                "sha256:1e760e2fe6a8163bc0b3d9a19c4f84342afa0a2affebfaa84b01b978a02ecaa7",
-                "sha256:e68985985296d9a66a881eb3193b0906246245294a881e7c8afe623866ac6a5c"
-            ],
-            "version": "==2022.1"
-        },
         "pyyaml": {
             "hashes": [
+                "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
                 "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
                 "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
                 "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
                 "sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b",
                 "sha256:0ce82d761c532fe4ec3f87fc45688bdd3a4c1dc5e0b4a19814b9009a29baefd4",
                 "sha256:1e4747bc279b4f613a09eb64bba2ba602d8a6664c6ce6396a4d0cd413a50ce07",
                 "sha256:213c60cd50106436cc818accf5baa1aba61c0189ff610f64f4a3e8c6726218ba",
                 "sha256:231710d57adfd809ef5d34183b8ed1eeae3f76459c18fb4a0b373ad56bedcdd9",
                 "sha256:277a0ef2981ca40581a47093e9e2d13b3f1fbbeffae064c1d21bfceba2030287",
                 "sha256:2cd5df3de48857ed0544b34e2d40e9fac445930039f3cfe4bcc592a1f836d513",
                 "sha256:40527857252b61eacd1d9af500c3337ba8deb8fc298940291486c465c8b46ec0",
+                "sha256:432557aa2c09802be39460360ddffd48156e30721f5e8d917f01d31694216782",
                 "sha256:473f9edb243cb1935ab5a084eb238d842fb8f404ed2193a915d1784b5a6b5fc0",
                 "sha256:48c346915c114f5fdb3ead70312bd042a953a8ce5c7106d5bfb1a5254e47da92",
                 "sha256:50602afada6d6cbfad699b0c7bb50d5ccffa7e46a3d738092afddc1f9758427f",
                 "sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2",
                 "sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc",
+                "sha256:81957921f441d50af23654aa6c5e5eaf9b06aba7f0a19c18a538dc7ef291c5a1",
                 "sha256:819b3830a1543db06c4d4b865e70ded25be52a2e0631ccd2f6a47a2822f2fd7c",
                 "sha256:897b80890765f037df3403d22bab41627ca8811ae55e9a722fd0392850ec4d86",
                 "sha256:98c4d36e99714e55cfbaaee6dd5badbc9a1ec339ebfc3b1f52e293aee6bb71a4",
                 "sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c",
                 "sha256:9fa600030013c4de8165339db93d182b9431076eb98eb40ee068700c9c813e34",
                 "sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b",
+                "sha256:afa17f5bc4d1b10afd4466fd3a44dc0e245382deca5b3c353d8b757f9e3ecb8d",
                 "sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c",
                 "sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb",
+                "sha256:bfaef573a63ba8923503d27530362590ff4f576c626d86a9fed95822a8255fd7",
                 "sha256:c5687b8d43cf58545ade1fe3e055f70eac7a5a1a0bf42824308d868289a95737",
                 "sha256:cba8c411ef271aa037d7357a2bc8f9ee8b58b9965831d9e51baf703280dc73d3",
                 "sha256:d15a181d1ecd0d4270dc32edb46f7cb7733c7c508857278d3d378d14d606db2d",
+                "sha256:d4b0ba9512519522b118090257be113b9468d804b19d63c71dbcf4a48fa32358",
                 "sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53",
                 "sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78",
                 "sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803",
                 "sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a",
+                "sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f",
                 "sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174",
                 "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==6.0"
         },
         "readme-renderer": {
             "hashes": [
-                "sha256:262510fe6aae81ed4e94d8b169077f325614c0b1a45916a80442c6576264a9c2",
-                "sha256:dfb4d17f21706d145f7473e0b61ca245ba58e810cf9b2209a48239677f82e5b0"
+                "sha256:9f77b519d96d03d7d7dce44977ba543090a14397c4f60de5b6eb5b8048110aa4",
+                "sha256:e18feb2a1e7706f2865b81ebb460056d93fb29d69daa10b223c00faa7bd9a00a"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==34.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==40.0"
         },
         "requests": {
             "hashes": [
-                "sha256:68d7c56fd5a8999887728ef304a6d12edc7be74f1cfa47714fc8b414525c9a61",
-                "sha256:f22fa1e554c9ddfd16e6e41ac79759e17be9e492b3587efa038054674760e72d"
+                "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
+                "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
             "index": "pypi",
-            "version": "==2.27.1"
+            "version": "==2.31.0"
         },
         "requests-toolbelt": {
             "hashes": [
-                "sha256:380606e1d10dc85c3bd47bf5a6095f815ec007be7a8b69c878507068df059e6f",
-                "sha256:968089d4584ad4ad7c171454f0a5c6dac23971e9472521ea3b6d49d610aa6fc0"
+                "sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6",
+                "sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06"
             ],
-            "version": "==0.9.1"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "version": "==1.0.0"
         },
         "rfc3986": {
             "hashes": [
                 "sha256:50b1502b60e289cb37883f3dfd34532b8873c7de9f49bb546641ce9cbd256ebd",
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
-        "secretstorage": {
+        "rich": {
             "hashes": [
-                "sha256:422d82c36172d88d6a0ed5afdec956514b189ddbfb72fefab0c8a1cee4eaf71f",
-                "sha256:fd666c51a6bf200643495a04abb261f83229dcb6fd8472ec393df7ffc8b6f195"
+                "sha256:8f87bc7ee54675732fa66a05ebfe489e27264caeeff3728c945d25971b6485ec",
+                "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"
             ],
-            "markers": "sys_platform == 'linux'",
-            "version": "==3.3.1"
+            "markers": "python_full_version >= '3.7.0'",
+            "version": "==13.4.2"
         },
         "setuptools": {
             "hashes": [
-                "sha256:8f4813dd6a4d6cc17bde85fb2e635fe19763f96efbb0ddf5575562e5ee0bc47a",
-                "sha256:c3d4e2ab578fbf83775755cd76dae73627915a22832cf4ea5de895978767833b"
+                "sha256:11e52c67415a381d10d6b462ced9cfb97066179f0e871399e006c4ab101fc85f",
+                "sha256:baf1fdb41c6da4cd2eae722e135500da913332ab3f2f5c7d33af9b492acb5235"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==61.2.0"
+            "version": "==68.0.0"
         },
         "setuptools-scm": {
             "hashes": [
-                "sha256:6833ac65c6ed9711a4d5d2266f8024cfa07c533a0e55f4c12f6eff280a5a9e30",
-                "sha256:acea13255093849de7ccb11af9e1fb8bde7067783450cee9ef7a93139bddf6d4"
+                "sha256:6c508345a771aad7d56ebff0e70628bf2b0ec7573762be9960214730de278f27",
+                "sha256:73988b6d848709e2af142aa48c986ea29592bbcfca5375678064708205253d8e"
             ],
             "index": "pypi",
-            "version": "==6.4.2"
+            "version": "==7.1.0"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -818,59 +957,59 @@
                 "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1",
                 "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"
             ],
             "version": "==2.2.0"
         },
         "sphinx": {
             "hashes": [
-                "sha256:7bf8ca9637a4ee15af412d1a1d9689fec70523a68ca9bb9127c2f3eeb344e2e6",
-                "sha256:ebf612653238bcc8f4359627a9b7ce44ede6fdd75d9d30f68255c7383d3a6226"
+                "sha256:60c5e04756c1709a98845ed27a2eed7a556af3993afb66e77fec48189f742616",
+                "sha256:61e025f788c5977d9412587e733733a289e2b9fdc2fef8868ddfbfc4ccfe881d"
             ],
             "index": "pypi",
-            "version": "==4.5.0"
+            "version": "==7.0.1"
         },
         "sphinx-autobuild": {
             "hashes": [
                 "sha256:8fe8cbfdb75db04475232f05187c776f46f6e9e04cacf1e49ce81bdac649ccac",
                 "sha256:de1ca3b66e271d2b5b5140c35034c89e47f263f2cd5db302c9217065f7443f05"
             ],
             "index": "pypi",
             "version": "==2021.3.14"
         },
         "sphinx-click": {
             "hashes": [
-                "sha256:36dbf271b1d2600fb05bd598ddeed0b6b6acf35beaf8bc9d507ba7716b232b0e",
-                "sha256:8fb0b048a577d346d741782e44d041d7e908922858273d99746f305870116121"
+                "sha256:2821c10a68fc9ee6ce7c92fad26540d8d8c8f45e6d7258f0e4fb7529ae8fab49",
+                "sha256:cc67692bd28f482c7f01531c61b64e9d2f069bfcf3d24cbbb51d4a84a749fa48"
             ],
             "index": "pypi",
-            "version": "==3.1.0"
+            "version": "==4.4.0"
         },
         "sphinxcontrib-applehelp": {
             "hashes": [
-                "sha256:806111e5e962be97c29ec4c1e7fe277bfd19e9652fb1a4392105b43e01af885a",
-                "sha256:a072735ec80e7675e3f432fcae8610ecf509c5f1869d17e2eecff44389cdbc58"
+                "sha256:29d341f67fb0f6f586b23ad80e072c8e6ad0b48417db2bde114a4c9746feb228",
+                "sha256:828f867945bbe39817c210a1abfd1bc4895c8b73fcaade56d45357a348a07d7e"
             ],
-            "markers": "python_version >= '3.5'",
-            "version": "==1.0.2"
+            "markers": "python_version >= '3.8'",
+            "version": "==1.0.4"
         },
         "sphinxcontrib-devhelp": {
             "hashes": [
                 "sha256:8165223f9a335cc1af7ffe1ed31d2871f325254c0423bc0c4c7cd1c1e4734a2e",
                 "sha256:ff7f1afa7b9642e7060379360a67e9c41e8f3121f2ce9164266f61b9f4b338e4"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.0.2"
         },
         "sphinxcontrib-htmlhelp": {
             "hashes": [
-                "sha256:d412243dfb797ae3ec2b59eca0e52dac12e75a241bf0e4eb861e450d06c6ed07",
-                "sha256:f5f8bb2d0d629f398bf47d0d69c07bc13b65f75a81ad9e2f71a63d4b7a2f6db2"
+                "sha256:0cbdd302815330058422b98a113195c9249825d681e18f11e8b1f78a2f11efff",
+                "sha256:c38cb46dccf316c79de6e5515e1770414b797162b23cd3d06e67020e1d2a6903"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.0.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==2.0.1"
         },
         "sphinxcontrib-jsmath": {
             "hashes": [
                 "sha256:2ec2eaebfb78f3f2078e73666b1415417a116cc848b72e5172e596c871103178",
                 "sha256:a9925e4a4587247ed2191a22df5f6970656cb8ca2bd6284309578f2153e0c4b8"
             ],
             "markers": "python_version >= '3.5'",
@@ -896,298 +1035,265 @@
             "hashes": [
                 "sha256:352a9a00ae864471d3a7ead8d7d79f5fc0b57e8b3f95e9867eb9eb28999b92fd",
                 "sha256:aa5f6de5dfdf809ef505c4895e51ef5c9eac17d0f287933eb49ec495280b6952"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.1.5"
         },
-        "toml": {
-            "hashes": [
-                "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b",
-                "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"
-            ],
-            "markers": "python_version >= '2.6' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==0.10.2"
-        },
         "tomli": {
             "hashes": [
                 "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc",
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
-            "markers": "python_version >= '3.7'",
+            "markers": "python_version < '3.11'",
             "version": "==2.0.1"
         },
         "tornado": {
             "hashes": [
-                "sha256:0a00ff4561e2929a2c37ce706cb8233b7907e0cdc22eab98888aca5dd3775feb",
-                "sha256:0d321a39c36e5f2c4ff12b4ed58d41390460f798422c4504e09eb5678e09998c",
-                "sha256:1e8225a1070cd8eec59a996c43229fe8f95689cb16e552d130b9793cb570a288",
-                "sha256:20241b3cb4f425e971cb0a8e4ffc9b0a861530ae3c52f2b0434e6c1b57e9fd95",
-                "sha256:25ad220258349a12ae87ede08a7b04aca51237721f63b1808d39bdb4b2164558",
-                "sha256:33892118b165401f291070100d6d09359ca74addda679b60390b09f8ef325ffe",
-                "sha256:33c6e81d7bd55b468d2e793517c909b139960b6c790a60b7991b9b6b76fb9791",
-                "sha256:3447475585bae2e77ecb832fc0300c3695516a47d46cefa0528181a34c5b9d3d",
-                "sha256:34ca2dac9e4d7afb0bed4677512e36a52f09caa6fded70b4e3e1c89dbd92c326",
-                "sha256:3e63498f680547ed24d2c71e6497f24bca791aca2fe116dbc2bd0ac7f191691b",
-                "sha256:548430be2740e327b3fe0201abe471f314741efcb0067ec4f2d7dcfb4825f3e4",
-                "sha256:6196a5c39286cc37c024cd78834fb9345e464525d8991c21e908cc046d1cc02c",
-                "sha256:61b32d06ae8a036a6607805e6720ef00a3c98207038444ba7fd3d169cd998910",
-                "sha256:6286efab1ed6e74b7028327365cf7346b1d777d63ab30e21a0f4d5b275fc17d5",
-                "sha256:65d98939f1a2e74b58839f8c4dab3b6b3c1ce84972ae712be02845e65391ac7c",
-                "sha256:66324e4e1beede9ac79e60f88de548da58b1f8ab4b2f1354d8375774f997e6c0",
-                "sha256:6c77c9937962577a6a76917845d06af6ab9197702a42e1346d8ae2e76b5e3675",
-                "sha256:70dec29e8ac485dbf57481baee40781c63e381bebea080991893cd297742b8fd",
-                "sha256:7250a3fa399f08ec9cb3f7b1b987955d17e044f1ade821b32e5f435130250d7f",
-                "sha256:748290bf9112b581c525e6e6d3820621ff020ed95af6f17fedef416b27ed564c",
-                "sha256:7da13da6f985aab7f6f28debab00c67ff9cbacd588e8477034c0652ac141feea",
-                "sha256:8f959b26f2634a091bb42241c3ed8d3cedb506e7c27b8dd5c7b9f745318ddbb6",
-                "sha256:9de9e5188a782be6b1ce866e8a51bc76a0fbaa0e16613823fc38e4fc2556ad05",
-                "sha256:a48900ecea1cbb71b8c71c620dee15b62f85f7c14189bdeee54966fbd9a0c5bd",
-                "sha256:b87936fd2c317b6ee08a5741ea06b9d11a6074ef4cc42e031bc6403f82a32575",
-                "sha256:c77da1263aa361938476f04c4b6c8916001b90b2c2fdd92d8d535e1af48fba5a",
-                "sha256:cb5ec8eead331e3bb4ce8066cf06d2dfef1bfb1b2a73082dfe8a161301b76e37",
-                "sha256:cc0ee35043162abbf717b7df924597ade8e5395e7b66d18270116f8745ceb795",
-                "sha256:d14d30e7f46a0476efb0deb5b61343b1526f73ebb5ed84f23dc794bdb88f9d9f",
-                "sha256:d371e811d6b156d82aa5f9a4e08b58debf97c302a35714f6f45e35139c332e32",
-                "sha256:d3d20ea5782ba63ed13bc2b8c291a053c8d807a8fa927d941bd718468f7b950c",
-                "sha256:d3f7594930c423fd9f5d1a76bee85a2c36fd8b4b16921cae7e965f22575e9c01",
-                "sha256:dcef026f608f678c118779cd6591c8af6e9b4155c44e0d1bc0c87c036fb8c8c4",
-                "sha256:e0791ac58d91ac58f694d8d2957884df8e4e2f6687cdf367ef7eb7497f79eaa2",
-                "sha256:e385b637ac3acaae8022e7e47dfa7b83d3620e432e3ecb9a3f7f58f150e50921",
-                "sha256:e519d64089b0876c7b467274468709dadf11e41d65f63bba207e04217f47c085",
-                "sha256:e7229e60ac41a1202444497ddde70a48d33909e484f96eb0da9baf8dc68541df",
-                "sha256:ed3ad863b1b40cd1d4bd21e7498329ccaece75db5a5bf58cd3c9f130843e7102",
-                "sha256:f0ba29bafd8e7e22920567ce0d232c26d4d47c8b5cf4ed7b562b5db39fa199c5",
-                "sha256:fa2ba70284fa42c2a5ecb35e322e68823288a4251f9ba9cc77be04ae15eada68",
-                "sha256:fba85b6cd9c39be262fcd23865652920832b61583de2a2ca907dbd8e8a8c81e5"
+                "sha256:05615096845cf50a895026f749195bf0b10b8909f9be672f50b0fe69cba368e4",
+                "sha256:0c325e66c8123c606eea33084976c832aa4e766b7dff8aedd7587ea44a604cdf",
+                "sha256:29e71c847a35f6e10ca3b5c2990a52ce38b233019d8e858b755ea6ce4dcdd19d",
+                "sha256:4b927c4f19b71e627b13f3db2324e4ae660527143f9e1f2e2fb404f3a187e2ba",
+                "sha256:5b17b1cf5f8354efa3d37c6e28fdfd9c1c1e5122f2cb56dac121ac61baa47cbe",
+                "sha256:6a0848f1aea0d196a7c4f6772197cbe2abc4266f836b0aac76947872cd29b411",
+                "sha256:7efcbcc30b7c654eb6a8c9c9da787a851c18f8ccd4a5a3a95b05c7accfa068d2",
+                "sha256:834ae7540ad3a83199a8da8f9f2d383e3c3d5130a328889e4cc991acc81e87a0",
+                "sha256:b46a6ab20f5c7c1cb949c72c1994a4585d2eaa0be4853f50a03b5031e964fc7c",
+                "sha256:c2de14066c4a38b4ecbbcd55c5cc4b5340eb04f1c5e81da7451ef555859c833f",
+                "sha256:c367ab6c0393d71171123ca5515c61ff62fe09024fa6bf299cd1339dc9456829"
             ],
             "markers": "python_version > '2.7'",
-            "version": "==6.1"
-        },
-        "tqdm": {
-            "hashes": [
-                "sha256:4230a49119a416c88cc47d0d2d32d5d90f1a282d5e497d49801950704e49863d",
-                "sha256:6461b009d6792008d0000e1b0c7ca50195ec78c0e808a3a6b668a56a3236c3a5"
-            ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==4.63.1"
+            "version": "==6.3.2"
         },
         "twine": {
             "hashes": [
-                "sha256:8efa52658e0ae770686a13b675569328f1fba9837e5de1867bfe5f46a9aefe19",
-                "sha256:d0550fca9dc19f3d5e8eadfce0c227294df0a2a951251a4385797c8a6198b7c8"
+                "sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8",
+                "sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8"
             ],
             "index": "pypi",
-            "version": "==3.8.0"
+            "version": "==4.0.2"
         },
         "types-requests": {
             "hashes": [
-                "sha256:2d371183c535208d2cc8fe7473d9b49c344c7077eb70302eb708638fb86086a8",
-                "sha256:77d09182a68e447e9e8b0ffc21abf54618b96f07689dffbb6a41cf0356542969"
+                "sha256:3de667cffa123ce698591de0ad7db034a5317457a596eb0b4944e5a9d9e8d1ac",
+                "sha256:afb06ef8f25ba83d59a1d424bd7a5a939082f94b94e90ab5e6116bd2559deaa3"
             ],
             "index": "pypi",
-            "version": "==2.27.15"
+            "version": "==2.31.0.1"
         },
         "types-urllib3": {
             "hashes": [
-                "sha256:24d64e441168851eb05f1d022de18ae31558f5649c8f1117e384c2e85e31315b",
-                "sha256:bd0abc01e9fb963e4fddd561a56d21cc371b988d1245662195c90379077139cd"
+                "sha256:3300538c9dc11dad32eae4827ac313f5d986b8b21494801f1bf97a1ac6c03ae5",
+                "sha256:5dbd1d2bef14efee43f5318b5d36d805a489f6600252bb53626d4bfafd95e27c"
             ],
-            "version": "==1.26.11"
+            "version": "==1.26.25.13"
         },
         "typing-extensions": {
             "hashes": [
-                "sha256:1a9462dcc3347a79b1f1c0271fbe79e844580bb598bafa1ed208b94da3cdcd42",
-                "sha256:21c85e0fe4b9a155d0799430b0ad741cdce7e359660ccbd8b530613e8df88ce2"
+                "sha256:5d8c9dac95c27d20df12fb1d97b9793ab8b2af8a3a525e68c80e21060c161771",
+                "sha256:935ccf31549830cda708b42289d44b6f74084d616a00be651601a4f968e77c82"
             ],
             "index": "pypi",
-            "version": "==4.1.1"
+            "version": "==4.7.0"
         },
         "urllib3": {
             "hashes": [
-                "sha256:44ece4d53fb1706f667c9bd1c648f5469a2ec925fcf3a776667042d645472c14",
-                "sha256:aabaf16477806a5e1dd19aa41f8c2b7950dd3c746362d7e3223dbe6de6ac448e"
+                "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1",
+                "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4' and python_version < '4'",
-            "version": "==1.26.9"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.0.3"
         },
         "vcrpy": {
             "hashes": [
-                "sha256:12c3fcdae7b88ecf11fc0d3e6d77586549d4575a2ceee18e82eee75c1f626162",
-                "sha256:57095bf22fc0a2d99ee9674cdafebed0f3ba763018582450706f7d3a74fff599"
+                "sha256:1ef3ddea819a26eda10b560c70bd74c41855241d431745712e31a5b2de2d05a8",
+                "sha256:28b66c87be7678896e9e78fee4f6695e3fb153d5d7e5f635416a33658452bb44"
             ],
-            "markers": "python_version >= '3.5'",
-            "version": "==4.1.1"
+            "markers": "python_version >= '3.8'",
+            "version": "==5.0.0"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:1e8588f35e8b42c6ec6841a13c5e88239de1e6e4e4cedfd3916b306dc826ec66",
-                "sha256:8e5b402037287126e81ccde9432b95a8be5b19d36584f64957060a3488c11ca8"
+                "sha256:34da10f14fea9be20e0fd7f04aba9732f84e593dac291b757ce42e3368a39419",
+                "sha256:8ff19a38c1021c742148edc4f81cb43d7f8c6816d2ede2ab72af5b84c749ade1"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==20.14.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==20.23.1"
         },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
         },
         "wrapt": {
             "hashes": [
-                "sha256:00108411e0f34c52ce16f81f1d308a571df7784932cc7491d1e94be2ee93374b",
-                "sha256:01f799def9b96a8ec1ef6b9c1bbaf2bbc859b87545efbecc4a78faea13d0e3a0",
-                "sha256:09d16ae7a13cff43660155383a2372b4aa09109c7127aa3f24c3cf99b891c330",
-                "sha256:14e7e2c5f5fca67e9a6d5f753d21f138398cad2b1159913ec9e9a67745f09ba3",
-                "sha256:167e4793dc987f77fd476862d32fa404d42b71f6a85d3b38cbce711dba5e6b68",
-                "sha256:1807054aa7b61ad8d8103b3b30c9764de2e9d0c0978e9d3fc337e4e74bf25faa",
-                "sha256:1f83e9c21cd5275991076b2ba1cd35418af3504667affb4745b48937e214bafe",
-                "sha256:21b1106bff6ece8cb203ef45b4f5778d7226c941c83aaaa1e1f0f4f32cc148cd",
-                "sha256:22626dca56fd7f55a0733e604f1027277eb0f4f3d95ff28f15d27ac25a45f71b",
-                "sha256:23f96134a3aa24cc50614920cc087e22f87439053d886e474638c68c8d15dc80",
-                "sha256:2498762814dd7dd2a1d0248eda2afbc3dd9c11537bc8200a4b21789b6df6cd38",
-                "sha256:28c659878f684365d53cf59dc9a1929ea2eecd7ac65da762be8b1ba193f7e84f",
-                "sha256:2eca15d6b947cfff51ed76b2d60fd172c6ecd418ddab1c5126032d27f74bc350",
-                "sha256:354d9fc6b1e44750e2a67b4b108841f5f5ea08853453ecbf44c81fdc2e0d50bd",
-                "sha256:36a76a7527df8583112b24adc01748cd51a2d14e905b337a6fefa8b96fc708fb",
-                "sha256:3a0a4ca02752ced5f37498827e49c414d694ad7cf451ee850e3ff160f2bee9d3",
-                "sha256:3a71dbd792cc7a3d772ef8cd08d3048593f13d6f40a11f3427c000cf0a5b36a0",
-                "sha256:3a88254881e8a8c4784ecc9cb2249ff757fd94b911d5df9a5984961b96113fff",
-                "sha256:47045ed35481e857918ae78b54891fac0c1d197f22c95778e66302668309336c",
-                "sha256:4775a574e9d84e0212f5b18886cace049a42e13e12009bb0491562a48bb2b758",
-                "sha256:493da1f8b1bb8a623c16552fb4a1e164c0200447eb83d3f68b44315ead3f9036",
-                "sha256:4b847029e2d5e11fd536c9ac3136ddc3f54bc9488a75ef7d040a3900406a91eb",
-                "sha256:59d7d92cee84a547d91267f0fea381c363121d70fe90b12cd88241bd9b0e1763",
-                "sha256:5a0898a640559dec00f3614ffb11d97a2666ee9a2a6bad1259c9facd01a1d4d9",
-                "sha256:5a9a1889cc01ed2ed5f34574c90745fab1dd06ec2eee663e8ebeefe363e8efd7",
-                "sha256:5b835b86bd5a1bdbe257d610eecab07bf685b1af2a7563093e0e69180c1d4af1",
-                "sha256:5f24ca7953f2643d59a9c87d6e272d8adddd4a53bb62b9208f36db408d7aafc7",
-                "sha256:61e1a064906ccba038aa3c4a5a82f6199749efbbb3cef0804ae5c37f550eded0",
-                "sha256:65bf3eb34721bf18b5a021a1ad7aa05947a1767d1aa272b725728014475ea7d5",
-                "sha256:6807bcee549a8cb2f38f73f469703a1d8d5d990815c3004f21ddb68a567385ce",
-                "sha256:68aeefac31c1f73949662ba8affaf9950b9938b712fb9d428fa2a07e40ee57f8",
-                "sha256:6915682f9a9bc4cf2908e83caf5895a685da1fbd20b6d485dafb8e218a338279",
-                "sha256:6d9810d4f697d58fd66039ab959e6d37e63ab377008ef1d63904df25956c7db0",
-                "sha256:729d5e96566f44fccac6c4447ec2332636b4fe273f03da128fff8d5559782b06",
-                "sha256:748df39ed634851350efa87690c2237a678ed794fe9ede3f0d79f071ee042561",
-                "sha256:763a73ab377390e2af26042f685a26787c402390f682443727b847e9496e4a2a",
-                "sha256:8323a43bd9c91f62bb7d4be74cc9ff10090e7ef820e27bfe8815c57e68261311",
-                "sha256:8529b07b49b2d89d6917cfa157d3ea1dfb4d319d51e23030664a827fe5fd2131",
-                "sha256:87fa943e8bbe40c8c1ba4086971a6fefbf75e9991217c55ed1bcb2f1985bd3d4",
-                "sha256:88236b90dda77f0394f878324cfbae05ae6fde8a84d548cfe73a75278d760291",
-                "sha256:891c353e95bb11abb548ca95c8b98050f3620a7378332eb90d6acdef35b401d4",
-                "sha256:89ba3d548ee1e6291a20f3c7380c92f71e358ce8b9e48161401e087e0bc740f8",
-                "sha256:8c6be72eac3c14baa473620e04f74186c5d8f45d80f8f2b4eda6e1d18af808e8",
-                "sha256:9a242871b3d8eecc56d350e5e03ea1854de47b17f040446da0e47dc3e0b9ad4d",
-                "sha256:9a3ff5fb015f6feb78340143584d9f8a0b91b6293d6b5cf4295b3e95d179b88c",
-                "sha256:9a5a544861b21e0e7575b6023adebe7a8c6321127bb1d238eb40d99803a0e8bd",
-                "sha256:9d57677238a0c5411c76097b8b93bdebb02eb845814c90f0b01727527a179e4d",
-                "sha256:9d8c68c4145041b4eeae96239802cfdfd9ef927754a5be3f50505f09f309d8c6",
-                "sha256:9d9fcd06c952efa4b6b95f3d788a819b7f33d11bea377be6b8980c95e7d10775",
-                "sha256:a0057b5435a65b933cbf5d859cd4956624df37b8bf0917c71756e4b3d9958b9e",
-                "sha256:a65bffd24409454b889af33b6c49d0d9bcd1a219b972fba975ac935f17bdf627",
-                "sha256:b0ed6ad6c9640671689c2dbe6244680fe8b897c08fd1fab2228429b66c518e5e",
-                "sha256:b21650fa6907e523869e0396c5bd591cc326e5c1dd594dcdccac089561cacfb8",
-                "sha256:b3f7e671fb19734c872566e57ce7fc235fa953d7c181bb4ef138e17d607dc8a1",
-                "sha256:b77159d9862374da213f741af0c361720200ab7ad21b9f12556e0eb95912cd48",
-                "sha256:bb36fbb48b22985d13a6b496ea5fb9bb2a076fea943831643836c9f6febbcfdc",
-                "sha256:d066ffc5ed0be00cd0352c95800a519cf9e4b5dd34a028d301bdc7177c72daf3",
-                "sha256:d332eecf307fca852d02b63f35a7872de32d5ba8b4ec32da82f45df986b39ff6",
-                "sha256:d808a5a5411982a09fef6b49aac62986274ab050e9d3e9817ad65b2791ed1425",
-                "sha256:d9bdfa74d369256e4218000a629978590fd7cb6cf6893251dad13d051090436d",
-                "sha256:db6a0ddc1282ceb9032e41853e659c9b638789be38e5b8ad7498caac00231c23",
-                "sha256:debaf04f813ada978d7d16c7dfa16f3c9c2ec9adf4656efdc4defdf841fc2f0c",
-                "sha256:f0408e2dbad9e82b4c960274214af533f856a199c9274bd4aff55d4634dedc33",
-                "sha256:f2f3bc7cd9c9fcd39143f11342eb5963317bd54ecc98e3650ca22704b69d9653"
+                "sha256:02fce1852f755f44f95af51f69d22e45080102e9d00258053b79367d07af39c0",
+                "sha256:077ff0d1f9d9e4ce6476c1a924a3332452c1406e59d90a2cf24aeb29eeac9420",
+                "sha256:078e2a1a86544e644a68422f881c48b84fef6d18f8c7a957ffd3f2e0a74a0d4a",
+                "sha256:0970ddb69bba00670e58955f8019bec4a42d1785db3faa043c33d81de2bf843c",
+                "sha256:1286eb30261894e4c70d124d44b7fd07825340869945c79d05bda53a40caa079",
+                "sha256:21f6d9a0d5b3a207cdf7acf8e58d7d13d463e639f0c7e01d82cdb671e6cb7923",
+                "sha256:230ae493696a371f1dbffaad3dafbb742a4d27a0afd2b1aecebe52b740167e7f",
+                "sha256:26458da5653aa5b3d8dc8b24192f574a58984c749401f98fff994d41d3f08da1",
+                "sha256:2cf56d0e237280baed46f0b5316661da892565ff58309d4d2ed7dba763d984b8",
+                "sha256:2e51de54d4fb8fb50d6ee8327f9828306a959ae394d3e01a1ba8b2f937747d86",
+                "sha256:2fbfbca668dd15b744418265a9607baa970c347eefd0db6a518aaf0cfbd153c0",
+                "sha256:38adf7198f8f154502883242f9fe7333ab05a5b02de7d83aa2d88ea621f13364",
+                "sha256:3a8564f283394634a7a7054b7983e47dbf39c07712d7b177b37e03f2467a024e",
+                "sha256:3abbe948c3cbde2689370a262a8d04e32ec2dd4f27103669a45c6929bcdbfe7c",
+                "sha256:3bbe623731d03b186b3d6b0d6f51865bf598587c38d6f7b0be2e27414f7f214e",
+                "sha256:40737a081d7497efea35ab9304b829b857f21558acfc7b3272f908d33b0d9d4c",
+                "sha256:41d07d029dd4157ae27beab04d22b8e261eddfc6ecd64ff7000b10dc8b3a5727",
+                "sha256:46ed616d5fb42f98630ed70c3529541408166c22cdfd4540b88d5f21006b0eff",
+                "sha256:493d389a2b63c88ad56cdc35d0fa5752daac56ca755805b1b0c530f785767d5e",
+                "sha256:4ff0d20f2e670800d3ed2b220d40984162089a6e2c9646fdb09b85e6f9a8fc29",
+                "sha256:54accd4b8bc202966bafafd16e69da9d5640ff92389d33d28555c5fd4f25ccb7",
+                "sha256:56374914b132c702aa9aa9959c550004b8847148f95e1b824772d453ac204a72",
+                "sha256:578383d740457fa790fdf85e6d346fda1416a40549fe8db08e5e9bd281c6a475",
+                "sha256:58d7a75d731e8c63614222bcb21dd992b4ab01a399f1f09dd82af17bbfc2368a",
+                "sha256:5c5aa28df055697d7c37d2099a7bc09f559d5053c3349b1ad0c39000e611d317",
+                "sha256:5fc8e02f5984a55d2c653f5fea93531e9836abbd84342c1d1e17abc4a15084c2",
+                "sha256:63424c681923b9f3bfbc5e3205aafe790904053d42ddcc08542181a30a7a51bd",
+                "sha256:64b1df0f83706b4ef4cfb4fb0e4c2669100fd7ecacfb59e091fad300d4e04640",
+                "sha256:74934ebd71950e3db69960a7da29204f89624dde411afbfb3b4858c1409b1e98",
+                "sha256:75669d77bb2c071333417617a235324a1618dba66f82a750362eccbe5b61d248",
+                "sha256:75760a47c06b5974aa5e01949bf7e66d2af4d08cb8c1d6516af5e39595397f5e",
+                "sha256:76407ab327158c510f44ded207e2f76b657303e17cb7a572ffe2f5a8a48aa04d",
+                "sha256:76e9c727a874b4856d11a32fb0b389afc61ce8aaf281ada613713ddeadd1cfec",
+                "sha256:77d4c1b881076c3ba173484dfa53d3582c1c8ff1f914c6461ab70c8428b796c1",
+                "sha256:780c82a41dc493b62fc5884fb1d3a3b81106642c5c5c78d6a0d4cbe96d62ba7e",
+                "sha256:7dc0713bf81287a00516ef43137273b23ee414fe41a3c14be10dd95ed98a2df9",
+                "sha256:7eebcdbe3677e58dd4c0e03b4f2cfa346ed4049687d839adad68cc38bb559c92",
+                "sha256:896689fddba4f23ef7c718279e42f8834041a21342d95e56922e1c10c0cc7afb",
+                "sha256:96177eb5645b1c6985f5c11d03fc2dbda9ad24ec0f3a46dcce91445747e15094",
+                "sha256:96e25c8603a155559231c19c0349245eeb4ac0096fe3c1d0be5c47e075bd4f46",
+                "sha256:9d37ac69edc5614b90516807de32d08cb8e7b12260a285ee330955604ed9dd29",
+                "sha256:9ed6aa0726b9b60911f4aed8ec5b8dd7bf3491476015819f56473ffaef8959bd",
+                "sha256:a487f72a25904e2b4bbc0817ce7a8de94363bd7e79890510174da9d901c38705",
+                "sha256:a4cbb9ff5795cd66f0066bdf5947f170f5d63a9274f99bdbca02fd973adcf2a8",
+                "sha256:a74d56552ddbde46c246b5b89199cb3fd182f9c346c784e1a93e4dc3f5ec9975",
+                "sha256:a89ce3fd220ff144bd9d54da333ec0de0399b52c9ac3d2ce34b569cf1a5748fb",
+                "sha256:abd52a09d03adf9c763d706df707c343293d5d106aea53483e0ec8d9e310ad5e",
+                "sha256:abd8f36c99512755b8456047b7be10372fca271bf1467a1caa88db991e7c421b",
+                "sha256:af5bd9ccb188f6a5fdda9f1f09d9f4c86cc8a539bd48a0bfdc97723970348418",
+                "sha256:b02f21c1e2074943312d03d243ac4388319f2456576b2c6023041c4d57cd7019",
+                "sha256:b06fa97478a5f478fb05e1980980a7cdf2712015493b44d0c87606c1513ed5b1",
+                "sha256:b0724f05c396b0a4c36a3226c31648385deb6a65d8992644c12a4963c70326ba",
+                "sha256:b130fe77361d6771ecf5a219d8e0817d61b236b7d8b37cc045172e574ed219e6",
+                "sha256:b56d5519e470d3f2fe4aa7585f0632b060d532d0696c5bdfb5e8319e1d0f69a2",
+                "sha256:b67b819628e3b748fd3c2192c15fb951f549d0f47c0449af0764d7647302fda3",
+                "sha256:ba1711cda2d30634a7e452fc79eabcadaffedf241ff206db2ee93dd2c89a60e7",
+                "sha256:bbeccb1aa40ab88cd29e6c7d8585582c99548f55f9b2581dfc5ba68c59a85752",
+                "sha256:bd84395aab8e4d36263cd1b9308cd504f6cf713b7d6d3ce25ea55670baec5416",
+                "sha256:c99f4309f5145b93eca6e35ac1a988f0dc0a7ccf9ccdcd78d3c0adf57224e62f",
+                "sha256:ca1cccf838cd28d5a0883b342474c630ac48cac5df0ee6eacc9c7290f76b11c1",
+                "sha256:cd525e0e52a5ff16653a3fc9e3dd827981917d34996600bbc34c05d048ca35cc",
+                "sha256:cdb4f085756c96a3af04e6eca7f08b1345e94b53af8921b25c72f096e704e145",
+                "sha256:ce42618f67741d4697684e501ef02f29e758a123aa2d669e2d964ff734ee00ee",
+                "sha256:d06730c6aed78cee4126234cf2d071e01b44b915e725a6cb439a879ec9754a3a",
+                "sha256:d5fe3e099cf07d0fb5a1e23d399e5d4d1ca3e6dfcbe5c8570ccff3e9208274f7",
+                "sha256:d6bcbfc99f55655c3d93feb7ef3800bd5bbe963a755687cbf1f490a71fb7794b",
+                "sha256:d787272ed958a05b2c86311d3a4135d3c2aeea4fc655705f074130aa57d71653",
+                "sha256:e169e957c33576f47e21864cf3fc9ff47c223a4ebca8960079b8bd36cb014fd0",
+                "sha256:e20076a211cd6f9b44a6be58f7eeafa7ab5720eb796975d0c03f05b47d89eb90",
+                "sha256:e826aadda3cae59295b95343db8f3d965fb31059da7de01ee8d1c40a60398b29",
+                "sha256:eef4d64c650f33347c1f9266fa5ae001440b232ad9b98f1f43dfe7a79435c0a6",
+                "sha256:f2e69b3ed24544b0d3dbe2c5c0ba5153ce50dcebb576fdc4696d52aa22db6034",
+                "sha256:f87ec75864c37c4c6cb908d282e1969e79763e0d9becdfe9fe5473b7bb1e5f09",
+                "sha256:fbec11614dba0424ca72f4e8ba3c420dba07b4a7c206c8c8e4e73f2e98f4c559",
+                "sha256:fd69666217b62fa5d7c6aa88e507493a34dec4fa20c5bd925e4bc12fce586639"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==1.14.0"
+            "version": "==1.15.0"
         },
         "yarl": {
             "hashes": [
-                "sha256:044daf3012e43d4b3538562da94a88fb12a6490652dbc29fb19adfa02cf72eac",
-                "sha256:0cba38120db72123db7c58322fa69e3c0efa933040ffb586c3a87c063ec7cae8",
-                "sha256:167ab7f64e409e9bdd99333fe8c67b5574a1f0495dcfd905bc7454e766729b9e",
-                "sha256:1be4bbb3d27a4e9aa5f3df2ab61e3701ce8fcbd3e9846dbce7c033a7e8136746",
-                "sha256:1ca56f002eaf7998b5fcf73b2421790da9d2586331805f38acd9997743114e98",
-                "sha256:1d3d5ad8ea96bd6d643d80c7b8d5977b4e2fb1bab6c9da7322616fd26203d125",
-                "sha256:1eb6480ef366d75b54c68164094a6a560c247370a68c02dddb11f20c4c6d3c9d",
-                "sha256:1edc172dcca3f11b38a9d5c7505c83c1913c0addc99cd28e993efeaafdfaa18d",
-                "sha256:211fcd65c58bf250fb994b53bc45a442ddc9f441f6fec53e65de8cba48ded986",
-                "sha256:29e0656d5497733dcddc21797da5a2ab990c0cb9719f1f969e58a4abac66234d",
-                "sha256:368bcf400247318382cc150aaa632582d0780b28ee6053cd80268c7e72796dec",
-                "sha256:39d5493c5ecd75c8093fa7700a2fb5c94fe28c839c8e40144b7ab7ccba6938c8",
-                "sha256:3abddf0b8e41445426d29f955b24aeecc83fa1072be1be4e0d194134a7d9baee",
-                "sha256:3bf8cfe8856708ede6a73907bf0501f2dc4e104085e070a41f5d88e7faf237f3",
-                "sha256:3ec1d9a0d7780416e657f1e405ba35ec1ba453a4f1511eb8b9fbab81cb8b3ce1",
-                "sha256:45399b46d60c253327a460e99856752009fcee5f5d3c80b2f7c0cae1c38d56dd",
-                "sha256:52690eb521d690ab041c3919666bea13ab9fbff80d615ec16fa81a297131276b",
-                "sha256:534b047277a9a19d858cde163aba93f3e1677d5acd92f7d10ace419d478540de",
-                "sha256:580c1f15500e137a8c37053e4cbf6058944d4c114701fa59944607505c2fe3a0",
-                "sha256:59218fef177296451b23214c91ea3aba7858b4ae3306dde120224cfe0f7a6ee8",
-                "sha256:5ba63585a89c9885f18331a55d25fe81dc2d82b71311ff8bd378fc8004202ff6",
-                "sha256:5bb7d54b8f61ba6eee541fba4b83d22b8a046b4ef4d8eb7f15a7e35db2e1e245",
-                "sha256:6152224d0a1eb254f97df3997d79dadd8bb2c1a02ef283dbb34b97d4f8492d23",
-                "sha256:67e94028817defe5e705079b10a8438b8cb56e7115fa01640e9c0bb3edf67332",
-                "sha256:695ba021a9e04418507fa930d5f0704edbce47076bdcfeeaba1c83683e5649d1",
-                "sha256:6a1a9fe17621af43e9b9fcea8bd088ba682c8192d744b386ee3c47b56eaabb2c",
-                "sha256:6ab0c3274d0a846840bf6c27d2c60ba771a12e4d7586bf550eefc2df0b56b3b4",
-                "sha256:6feca8b6bfb9eef6ee057628e71e1734caf520a907b6ec0d62839e8293e945c0",
-                "sha256:737e401cd0c493f7e3dd4db72aca11cfe069531c9761b8ea474926936b3c57c8",
-                "sha256:788713c2896f426a4e166b11f4ec538b5736294ebf7d5f654ae445fd44270832",
-                "sha256:797c2c412b04403d2da075fb93c123df35239cd7b4cc4e0cd9e5839b73f52c58",
-                "sha256:8300401dc88cad23f5b4e4c1226f44a5aa696436a4026e456fe0e5d2f7f486e6",
-                "sha256:87f6e082bce21464857ba58b569370e7b547d239ca22248be68ea5d6b51464a1",
-                "sha256:89ccbf58e6a0ab89d487c92a490cb5660d06c3a47ca08872859672f9c511fc52",
-                "sha256:8b0915ee85150963a9504c10de4e4729ae700af11df0dc5550e6587ed7891e92",
-                "sha256:8cce6f9fa3df25f55521fbb5c7e4a736683148bcc0c75b21863789e5185f9185",
-                "sha256:95a1873b6c0dd1c437fb3bb4a4aaa699a48c218ac7ca1e74b0bee0ab16c7d60d",
-                "sha256:9b4c77d92d56a4c5027572752aa35082e40c561eec776048330d2907aead891d",
-                "sha256:9bfcd43c65fbb339dc7086b5315750efa42a34eefad0256ba114cd8ad3896f4b",
-                "sha256:9c1f083e7e71b2dd01f7cd7434a5f88c15213194df38bc29b388ccdf1492b739",
-                "sha256:a1d0894f238763717bdcfea74558c94e3bc34aeacd3351d769460c1a586a8b05",
-                "sha256:a467a431a0817a292121c13cbe637348b546e6ef47ca14a790aa2fa8cc93df63",
-                "sha256:aa32aaa97d8b2ed4e54dc65d241a0da1c627454950f7d7b1f95b13985afd6c5d",
-                "sha256:ac10bbac36cd89eac19f4e51c032ba6b412b3892b685076f4acd2de18ca990aa",
-                "sha256:ac35ccde589ab6a1870a484ed136d49a26bcd06b6a1c6397b1967ca13ceb3913",
-                "sha256:bab827163113177aee910adb1f48ff7af31ee0289f434f7e22d10baf624a6dfe",
-                "sha256:baf81561f2972fb895e7844882898bda1eef4b07b5b385bcd308d2098f1a767b",
-                "sha256:bf19725fec28452474d9887a128e98dd67eee7b7d52e932e6949c532d820dc3b",
-                "sha256:c01a89a44bb672c38f42b49cdb0ad667b116d731b3f4c896f72302ff77d71656",
-                "sha256:c0910c6b6c31359d2f6184828888c983d54d09d581a4a23547a35f1d0b9484b1",
-                "sha256:c10ea1e80a697cf7d80d1ed414b5cb8f1eec07d618f54637067ae3c0334133c4",
-                "sha256:c1164a2eac148d85bbdd23e07dfcc930f2e633220f3eb3c3e2a25f6148c2819e",
-                "sha256:c145ab54702334c42237a6c6c4cc08703b6aa9b94e2f227ceb3d477d20c36c63",
-                "sha256:c17965ff3706beedafd458c452bf15bac693ecd146a60a06a214614dc097a271",
-                "sha256:c19324a1c5399b602f3b6e7db9478e5b1adf5cf58901996fc973fe4fccd73eed",
-                "sha256:c2a1ac41a6aa980db03d098a5531f13985edcb451bcd9d00670b03129922cd0d",
-                "sha256:c6ddcd80d79c96eb19c354d9dca95291589c5954099836b7c8d29278a7ec0bda",
-                "sha256:c9c6d927e098c2d360695f2e9d38870b2e92e0919be07dbe339aefa32a090265",
-                "sha256:cc8b7a7254c0fc3187d43d6cb54b5032d2365efd1df0cd1749c0c4df5f0ad45f",
-                "sha256:cff3ba513db55cc6a35076f32c4cdc27032bd075c9faef31fec749e64b45d26c",
-                "sha256:d260d4dc495c05d6600264a197d9d6f7fc9347f21d2594926202fd08cf89a8ba",
-                "sha256:d6f3d62e16c10e88d2168ba2d065aa374e3c538998ed04996cd373ff2036d64c",
-                "sha256:da6df107b9ccfe52d3a48165e48d72db0eca3e3029b5b8cb4fe6ee3cb870ba8b",
-                "sha256:dfe4b95b7e00c6635a72e2d00b478e8a28bfb122dc76349a06e20792eb53a523",
-                "sha256:e39378894ee6ae9f555ae2de332d513a5763276a9265f8e7cbaeb1b1ee74623a",
-                "sha256:ede3b46cdb719c794427dcce9d8beb4abe8b9aa1e97526cc20de9bd6583ad1ef",
-                "sha256:f2a8508f7350512434e41065684076f640ecce176d262a7d54f0da41d99c5a95",
-                "sha256:f44477ae29025d8ea87ec308539f95963ffdc31a82f42ca9deecf2d505242e72",
-                "sha256:f64394bd7ceef1237cc604b5a89bf748c95982a84bcd3c4bbeb40f685c810794",
-                "sha256:fc4dd8b01a8112809e6b636b00f487846956402834a7fd59d46d4f4267181c41",
-                "sha256:fce78593346c014d0d986b7ebc80d782b7f5e19843ca798ed62f8e3ba8728576",
-                "sha256:fd547ec596d90c8676e369dd8a581a21227fe9b4ad37d0dc7feb4ccf544c2d59"
+                "sha256:04ab9d4b9f587c06d801c2abfe9317b77cdf996c65a90d5e84ecc45010823571",
+                "sha256:066c163aec9d3d073dc9ffe5dd3ad05069bcb03fcaab8d221290ba99f9f69ee3",
+                "sha256:13414591ff516e04fcdee8dc051c13fd3db13b673c7a4cb1350e6b2ad9639ad3",
+                "sha256:149ddea5abf329752ea5051b61bd6c1d979e13fbf122d3a1f9f0c8be6cb6f63c",
+                "sha256:159d81f22d7a43e6eabc36d7194cb53f2f15f498dbbfa8edc8a3239350f59fe7",
+                "sha256:1b1bba902cba32cdec51fca038fd53f8beee88b77efc373968d1ed021024cc04",
+                "sha256:22a94666751778629f1ec4280b08eb11815783c63f52092a5953faf73be24191",
+                "sha256:2a96c19c52ff442a808c105901d0bdfd2e28575b3d5f82e2f5fd67e20dc5f4ea",
+                "sha256:2b0738fb871812722a0ac2154be1f049c6223b9f6f22eec352996b69775b36d4",
+                "sha256:2c315df3293cd521033533d242d15eab26583360b58f7ee5d9565f15fee1bef4",
+                "sha256:32f1d071b3f362c80f1a7d322bfd7b2d11e33d2adf395cc1dd4df36c9c243095",
+                "sha256:3458a24e4ea3fd8930e934c129b676c27452e4ebda80fbe47b56d8c6c7a63a9e",
+                "sha256:38a3928ae37558bc1b559f67410df446d1fbfa87318b124bf5032c31e3447b74",
+                "sha256:3da8a678ca8b96c8606bbb8bfacd99a12ad5dd288bc6f7979baddd62f71c63ef",
+                "sha256:494053246b119b041960ddcd20fd76224149cfea8ed8777b687358727911dd33",
+                "sha256:50f33040f3836e912ed16d212f6cc1efb3231a8a60526a407aeb66c1c1956dde",
+                "sha256:52a25809fcbecfc63ac9ba0c0fb586f90837f5425edfd1ec9f3372b119585e45",
+                "sha256:53338749febd28935d55b41bf0bcc79d634881195a39f6b2f767870b72514caf",
+                "sha256:5415d5a4b080dc9612b1b63cba008db84e908b95848369aa1da3686ae27b6d2b",
+                "sha256:5610f80cf43b6202e2c33ba3ec2ee0a2884f8f423c8f4f62906731d876ef4fac",
+                "sha256:566185e8ebc0898b11f8026447eacd02e46226716229cea8db37496c8cdd26e0",
+                "sha256:56ff08ab5df8429901ebdc5d15941b59f6253393cb5da07b4170beefcf1b2528",
+                "sha256:59723a029760079b7d991a401386390c4be5bfec1e7dd83e25a6a0881859e716",
+                "sha256:5fcd436ea16fee7d4207c045b1e340020e58a2597301cfbcfdbe5abd2356c2fb",
+                "sha256:61016e7d582bc46a5378ffdd02cd0314fb8ba52f40f9cf4d9a5e7dbef88dee18",
+                "sha256:63c48f6cef34e6319a74c727376e95626f84ea091f92c0250a98e53e62c77c72",
+                "sha256:646d663eb2232d7909e6601f1a9107e66f9791f290a1b3dc7057818fe44fc2b6",
+                "sha256:662e6016409828ee910f5d9602a2729a8a57d74b163c89a837de3fea050c7582",
+                "sha256:674ca19cbee4a82c9f54e0d1eee28116e63bc6fd1e96c43031d11cbab8b2afd5",
+                "sha256:6a5883464143ab3ae9ba68daae8e7c5c95b969462bbe42e2464d60e7e2698368",
+                "sha256:6e7221580dc1db478464cfeef9b03b95c5852cc22894e418562997df0d074ccc",
+                "sha256:75df5ef94c3fdc393c6b19d80e6ef1ecc9ae2f4263c09cacb178d871c02a5ba9",
+                "sha256:783185c75c12a017cc345015ea359cc801c3b29a2966c2655cd12b233bf5a2be",
+                "sha256:822b30a0f22e588b32d3120f6d41e4ed021806418b4c9f0bc3048b8c8cb3f92a",
+                "sha256:8288d7cd28f8119b07dd49b7230d6b4562f9b61ee9a4ab02221060d21136be80",
+                "sha256:82aa6264b36c50acfb2424ad5ca537a2060ab6de158a5bd2a72a032cc75b9eb8",
+                "sha256:832b7e711027c114d79dffb92576acd1bd2decc467dec60e1cac96912602d0e6",
+                "sha256:838162460b3a08987546e881a2bfa573960bb559dfa739e7800ceeec92e64417",
+                "sha256:83fcc480d7549ccebe9415d96d9263e2d4226798c37ebd18c930fce43dfb9574",
+                "sha256:84e0b1599334b1e1478db01b756e55937d4614f8654311eb26012091be109d59",
+                "sha256:891c0e3ec5ec881541f6c5113d8df0315ce5440e244a716b95f2525b7b9f3608",
+                "sha256:8c2ad583743d16ddbdf6bb14b5cd76bf43b0d0006e918809d5d4ddf7bde8dd82",
+                "sha256:8c56986609b057b4839968ba901944af91b8e92f1725d1a2d77cbac6972b9ed1",
+                "sha256:8ea48e0a2f931064469bdabca50c2f578b565fc446f302a79ba6cc0ee7f384d3",
+                "sha256:8ec53a0ea2a80c5cd1ab397925f94bff59222aa3cf9c6da938ce05c9ec20428d",
+                "sha256:95d2ecefbcf4e744ea952d073c6922e72ee650ffc79028eb1e320e732898d7e8",
+                "sha256:9b3152f2f5677b997ae6c804b73da05a39daa6a9e85a512e0e6823d81cdad7cc",
+                "sha256:9bf345c3a4f5ba7f766430f97f9cc1320786f19584acc7086491f45524a551ac",
+                "sha256:a60347f234c2212a9f0361955007fcf4033a75bf600a33c88a0a8e91af77c0e8",
+                "sha256:a74dcbfe780e62f4b5a062714576f16c2f3493a0394e555ab141bf0d746bb955",
+                "sha256:a83503934c6273806aed765035716216cc9ab4e0364f7f066227e1aaea90b8d0",
+                "sha256:ac9bb4c5ce3975aeac288cfcb5061ce60e0d14d92209e780c93954076c7c4367",
+                "sha256:aff634b15beff8902d1f918012fc2a42e0dbae6f469fce134c8a0dc51ca423bb",
+                "sha256:b03917871bf859a81ccb180c9a2e6c1e04d2f6a51d953e6a5cdd70c93d4e5a2a",
+                "sha256:b124e2a6d223b65ba8768d5706d103280914d61f5cae3afbc50fc3dfcc016623",
+                "sha256:b25322201585c69abc7b0e89e72790469f7dad90d26754717f3310bfe30331c2",
+                "sha256:b7232f8dfbd225d57340e441d8caf8652a6acd06b389ea2d3222b8bc89cbfca6",
+                "sha256:b8cc1863402472f16c600e3e93d542b7e7542a540f95c30afd472e8e549fc3f7",
+                "sha256:b9a4e67ad7b646cd6f0938c7ebfd60e481b7410f574c560e455e938d2da8e0f4",
+                "sha256:be6b3fdec5c62f2a67cb3f8c6dbf56bbf3f61c0f046f84645cd1ca73532ea051",
+                "sha256:bf74d08542c3a9ea97bb8f343d4fcbd4d8f91bba5ec9d5d7f792dbe727f88938",
+                "sha256:c027a6e96ef77d401d8d5a5c8d6bc478e8042f1e448272e8d9752cb0aff8b5c8",
+                "sha256:c0c77533b5ed4bcc38e943178ccae29b9bcf48ffd1063f5821192f23a1bd27b9",
+                "sha256:c1012fa63eb6c032f3ce5d2171c267992ae0c00b9e164efe4d73db818465fac3",
+                "sha256:c3a53ba34a636a256d767c086ceb111358876e1fb6b50dfc4d3f4951d40133d5",
+                "sha256:d4e2c6d555e77b37288eaf45b8f60f0737c9efa3452c6c44626a5455aeb250b9",
+                "sha256:de119f56f3c5f0e2fb4dee508531a32b069a5f2c6e827b272d1e0ff5ac040333",
+                "sha256:e65610c5792870d45d7b68c677681376fcf9cc1c289f23e8e8b39c1485384185",
+                "sha256:e9fdc7ac0d42bc3ea78818557fab03af6181e076a2944f43c38684b4b6bed8e3",
+                "sha256:ee4afac41415d52d53a9833ebae7e32b344be72835bbb589018c9e938045a560",
+                "sha256:f364d3480bffd3aa566e886587eaca7c8c04d74f6e8933f3f2c996b7f09bee1b",
+                "sha256:f3b078dbe227f79be488ffcfc7a9edb3409d018e0952cf13f15fd6512847f3f7",
+                "sha256:f4e2d08f07a3d7d3e12549052eb5ad3eab1c349c53ac51c209a0e5991bbada78",
+                "sha256:f7a3d8146575e08c29ed1cd287068e6d02f1c7bdff8970db96683b9591b86ee7"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==1.7.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==1.9.2"
         },
         "zipp": {
             "hashes": [
-                "sha256:9f50f446828eb9d45b267433fd3e9da8d801f614129124863f9c51ebceafb87d",
-                "sha256:b47250dd24f92b7dd6a0a8fc5244da14608f3ca90a5efcd37a3b1642fac9a375"
+                "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
+                "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.7.0"
+            "version": "==3.15.0"
         }
     }
 }
```

### Comparing `savepagenow-1.2.3/docs/Makefile` & `savepagenow-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `savepagenow-1.2.3/docs/_build/html/_sources/cli.md.txt` & `savepagenow-1.3.0/docs/cli.md`

 * *Files identical despite different names*

### Comparing `savepagenow-1.2.3/docs/_build/html/_sources/index.md.txt` & `savepagenow-1.3.0/docs/index.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 00000000: 6060 607b 696e 636c 7564 657d 205f 7465  ```{include} _te
 00000010: 6d70 6c61 7465 732f 6e61 762e 6874 6d6c  mplates/nav.html
 00000020: 0a60 6060 0a0a 2320 7361 7665 7061 6765  .```..# savepage
 00000030: 6e6f 770a 0a41 2073 696d 706c 6520 5079  now..A simple Py
 00000040: 7468 6f6e 2077 7261 7070 6572 2061 6e64  thon wrapper and
 00000050: 2063 6f6d 6d61 6e64 2d6c 696e 6520 696e   command-line in
 00000060: 7465 7266 6163 6520 666f 7220 6172 6368  terface for arch
-00000070: 6976 652e 6f72 67e2 8099 7320 2253 6176  ive.org...s "Sav
-00000080: 6520 5061 6765 204e 6f77 2220 6361 7074  e Page Now" capt
-00000090: 7572 696e 6720 7365 7276 6963 650a 0a60  uring service..`
-000000a0: 6060 7b74 6f63 7472 6565 7d0a 3a6d 6178  ``{toctree}.:max
-000000b0: 6465 7074 683a 2031 0a3a 6e61 6d65 3a20  depth: 1.:name: 
-000000c0: 6d61 7374 6572 746f 630a 0a69 6e73 7461  mastertoc..insta
-000000d0: 6c6c 0a70 7974 686f 6e0a 636c 690a 7573  ll.python.cli.us
-000000e0: 6572 6167 656e 740a 6578 6365 7074 696f  eragent.exceptio
-000000f0: 6e73 0a60 6060 0a0a 2323 204c 696e 6b73  ns.```..## Links
-00000100: 0a0a 2d20 446f 6375 6d65 6e74 6174 696f  ..- Documentatio
-00000110: 6e3a 205b 7061 6c65 7769 2e72 652f 646f  n: [palewi.re/do
-00000120: 6373 2f73 6176 6570 6167 656e 6f77 2f5d  cs/savepagenow/]
-00000130: 2868 7474 7073 3a2f 2f70 616c 6577 692e  (https://palewi.
-00000140: 7265 2f64 6f63 732f 7361 7665 7061 6765  re/docs/savepage
-00000150: 6e6f 772f 290a 2d20 436f 6465 3a20 5b67  now/).- Code: [g
-00000160: 6974 6875 622e 636f 6d2f 7061 6c65 7769  ithub.com/palewi
-00000170: 7265 2f73 6176 6570 6167 656e 6f77 5d28  re/savepagenow](
-00000180: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000190: 6f6d 2f70 616c 6577 6972 652f 7361 7665  om/palewire/save
-000001a0: 7061 6765 6e6f 7729 0a2d 2049 7373 7565  pagenow).- Issue
-000001b0: 733a 205b 6769 7468 7562 2e63 6f6d 2f70  s: [github.com/p
-000001c0: 616c 6577 6972 652f 7361 7665 7061 6765  alewire/savepage
-000001d0: 6e6f 772f 6973 7375 6573 5d28 6874 7470  now/issues](http
-000001e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
-000001f0: 616c 6577 6972 652f 7361 7665 7061 6765  alewire/savepage
-00000200: 6e6f 772f 6973 7375 6573 290a 2d20 5061  now/issues).- Pa
-00000210: 636b 6167 696e 673a 205b 7079 7069 2e6f  ckaging: [pypi.o
-00000220: 7267 2f70 726f 6a65 6374 2f73 6176 6570  rg/project/savep
-00000230: 6167 656e 6f77 5d28 6874 7470 733a 2f2f  agenow](https://
-00000240: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
-00000250: 2f73 6176 6570 6167 656e 6f77 290a       /savepagenow).
+00000070: 6976 652e 6f72 67e2 8099 7320 5be2 809c  ive.org...s [...
+00000080: 5361 7665 2050 6167 6520 4e6f 77e2 809d  Save Page Now...
+00000090: 5d28 6874 7470 733a 2f2f 6172 6368 6976  ](https://archiv
+000000a0: 652e 6f72 672f 7765 6229 2063 6170 7475  e.org/web) captu
+000000b0: 7269 6e67 2073 6572 7669 6365 0a0a 6060  ring service..``
+000000c0: 607b 746f 6374 7265 657d 0a3a 6d61 7864  `{toctree}.:maxd
+000000d0: 6570 7468 3a20 310a 3a6e 616d 653a 206d  epth: 1.:name: m
+000000e0: 6173 7465 7274 6f63 0a0a 696e 7374 616c  astertoc..instal
+000000f0: 6c0a 7079 7468 6f6e 0a63 6c69 0a75 7365  l.python.cli.use
+00000100: 7261 6765 6e74 0a65 7863 6570 7469 6f6e  ragent.exception
+00000110: 730a 6060 600a 0a23 2320 4c69 6e6b 730a  s.```..## Links.
+00000120: 0a2d 2044 6f63 756d 656e 7461 7469 6f6e  .- Documentation
+00000130: 3a20 5b70 616c 6577 692e 7265 2f64 6f63  : [palewi.re/doc
+00000140: 732f 7361 7665 7061 6765 6e6f 772f 5d28  s/savepagenow/](
+00000150: 6874 7470 733a 2f2f 7061 6c65 7769 2e72  https://palewi.r
+00000160: 652f 646f 6373 2f73 6176 6570 6167 656e  e/docs/savepagen
+00000170: 6f77 2f29 0a2d 2043 6f64 653a 205b 6769  ow/).- Code: [gi
+00000180: 7468 7562 2e63 6f6d 2f70 616c 6577 6972  thub.com/palewir
+00000190: 652f 7361 7665 7061 6765 6e6f 775d 2868  e/savepagenow](h
+000001a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000001b0: 6d2f 7061 6c65 7769 7265 2f73 6176 6570  m/palewire/savep
+000001c0: 6167 656e 6f77 290a 2d20 4973 7375 6573  agenow).- Issues
+000001d0: 3a20 5b67 6974 6875 622e 636f 6d2f 7061  : [github.com/pa
+000001e0: 6c65 7769 7265 2f73 6176 6570 6167 656e  lewire/savepagen
+000001f0: 6f77 2f69 7373 7565 735d 2868 7474 7073  ow/issues](https
+00000200: 3a2f 2f67 6974 6875 622e 636f 6d2f 7061  ://github.com/pa
+00000210: 6c65 7769 7265 2f73 6176 6570 6167 656e  lewire/savepagen
+00000220: 6f77 2f69 7373 7565 7329 0a2d 2050 6163  ow/issues).- Pac
+00000230: 6b61 6769 6e67 3a20 5b70 7970 692e 6f72  kaging: [pypi.or
+00000240: 672f 7072 6f6a 6563 742f 7361 7665 7061  g/project/savepa
+00000250: 6765 6e6f 775d 2868 7474 7073 3a2f 2f70  genow](https://p
+00000260: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+00000270: 7361 7665 7061 6765 6e6f 7729 0a         savepagenow).
```

### Comparing `savepagenow-1.2.3/docs/_build/html/_sources/python.md.txt` & `savepagenow-1.3.0/docs/python.md`

 * *Files 20% similar despite different names*

```diff
@@ -11,99 +11,141 @@
 000000a0: 6f6e 0a61 7263 6869 7665 5f75 726c 203d  on.archive_url =
 000000b0: 2073 6176 6570 6167 656e 6f77 2e63 6170   savepagenow.cap
 000000c0: 7475 7265 2822 6874 7470 3a2f 2f77 7777  ture("http://www
 000000d0: 2e65 7861 6d70 6c65 2e63 6f6d 2f22 290a  .example.com/").
 000000e0: 6060 600a 0a53 6565 2077 6865 7265 2069  ```..See where i
 000000f0: 7427 7320 7374 6f72 6564 2e0a 0a60 6060  t's stored...```
 00000100: 7079 7468 6f6e 0a70 7269 6e74 2861 7263  python.print(arc
-00000110: 6869 7665 5f75 726c 290a 6060 600a 0a49  hive_url).```..I
-00000120: 6620 6120 5552 4c20 6861 7320 6265 656e  f a URL has been
-00000130: 2072 6563 656e 746c 7920 6361 6368 6564   recently cached
-00000140: 2c20 6172 6368 6976 652e 6f72 6720 6d61  , archive.org ma
-00000150: 7920 7265 7475 726e 2074 6865 2055 524c  y return the URL
-00000160: 2074 6f20 7468 6174 2070 6167 6520 7261   to that page ra
-00000170: 7468 6572 2074 6861 6e20 636f 6e64 7563  ther than conduc
-00000180: 7420 6120 6e65 7720 6361 7074 7572 652e  t a new capture.
-00000190: 2057 6865 6e20 7468 6174 2068 6170 7065   When that happe
-000001a0: 6e73 2c20 7468 6520 6060 6361 7074 7572  ns, the ``captur
-000001b0: 6560 6020 6d65 7468 6f64 2077 696c 6c20  e`` method will 
-000001c0: 7261 6973 6520 6120 6060 4361 6368 6564  raise a ``Cached
-000001d0: 5061 6765 6060 2065 7863 6570 7469 6f6e  Page`` exception
-000001e0: 2e0a 0a54 6869 7320 6973 206c 696b 656c  ...This is likel
-000001f0: 7920 6861 7070 656e 2069 6620 796f 7520  y happen if you 
-00000200: 7265 7175 6573 7420 7468 6520 7361 6d65  request the same
-00000210: 2055 524c 2074 7769 6365 2077 6974 6869   URL twice withi
-00000220: 6e20 6120 6665 7720 7365 636f 6e64 732e  n a few seconds.
-00000230: 0a0a 6060 600a 7361 7665 7061 6765 6e6f  ..```.savepageno
-00000240: 772e 6361 7074 7572 6528 2268 7474 703a  w.capture("http:
-00000250: 2f2f 7777 772e 6578 616d 706c 652e 636f  //www.example.co
-00000260: 6d2f 2229 0a27 6874 7470 733a 2f2f 7765  m/").'https://we
-00000270: 622e 6172 6368 6976 652e 6f72 672f 7765  b.archive.org/we
-00000280: 622f 3230 3136 3130 3139 3036 3236 3337  b/20161019062637
-00000290: 2f68 7474 703a 2f2f 7777 772e 6578 616d  /http://www.exam
-000002a0: 706c 652e 636f 6d2f 270a 7361 7665 7061  ple.com/'.savepa
-000002b0: 6765 6e6f 772e 6361 7074 7572 6528 2268  genow.capture("h
-000002c0: 7474 703a 2f2f 7777 772e 6578 616d 706c  ttp://www.exampl
-000002d0: 652e 636f 6d2f 2229 0a54 7261 6365 6261  e.com/").Traceba
-000002e0: 636b 2028 6d6f 7374 2072 6563 656e 7420  ck (most recent 
-000002f0: 6361 6c6c 206c 6173 7429 3a0a 2020 2046  call last):.   F
-00000300: 696c 6520 223c 7374 6469 6e3e 222c 206c  ile "<stdin>", l
-00000310: 696e 6520 312c 2069 6e20 3c6d 6f64 756c  ine 1, in <modul
-00000320: 653e 0a20 2020 4669 6c65 2022 7361 7665  e>.   File "save
-00000330: 7061 6765 6e6f 772f 5f5f 696e 6974 5f5f  pagenow/__init__
-00000340: 2e70 7922 2c20 6c69 6e65 2033 362c 2069  .py", line 36, i
-00000350: 6e20 6361 7074 7572 650a 2020 2020 2020  n capture.      
-00000360: 6172 6368 6976 655f 7572 6c0a 7361 7665  archive_url.save
-00000370: 7061 6765 6e6f 772e 6578 6365 7074 696f  pagenow.exceptio
-00000380: 6e73 2e43 6163 6865 6450 6167 653a 2061  ns.CachedPage: a
-00000390: 7263 6869 7665 2e6f 7267 2072 6574 7572  rchive.org retur
-000003a0: 6e65 6420 6120 6361 6368 6564 2076 6572  ned a cached ver
-000003b0: 7369 6f6e 206f 6620 7468 6973 2070 6167  sion of this pag
-000003c0: 653a 2068 7474 7073 3a2f 2f77 6562 2e61  e: https://web.a
-000003d0: 7263 6869 7665 2e6f 7267 2f77 6562 2f32  rchive.org/web/2
-000003e0: 3031 3631 3031 3930 3632 3633 372f 6874  0161019062637/ht
-000003f0: 7470 3a2f 2f77 7777 2e65 7861 6d70 6c65  tp://www.example
-00000400: 2e63 6f6d 2f0a 6060 600a 0a59 6f75 2063  .com/.```..You c
-00000410: 616e 2063 7261 6674 2079 6f75 7220 636f  an craft your co
-00000420: 6465 2074 6f20 6361 7463 6820 7468 6174  de to catch that
-00000430: 2065 7863 6570 7469 6f6e 2079 6f75 7273   exception yours
-00000440: 656c 662c 206f 7220 7573 6520 7468 6520  elf, or use the 
-00000450: 6275 696c 742d 696e 2060 6063 6170 7475  built-in ``captu
-00000460: 7265 5f6f 725f 6361 6368 6560 6020 6d65  re_or_cache`` me
-00000470: 7468 6f64 2c20 7768 6963 6820 7769 6c6c  thod, which will
-00000480: 2072 6574 7572 6e20 7468 6520 5552 4c20   return the URL 
-00000490: 7072 6f76 6964 6564 2062 7920 6172 6368  provided by arch
-000004a0: 6976 652e 6f72 6720 616c 6f6e 6720 7769  ive.org along wi
-000004b0: 7468 2061 2062 6f6f 6c65 616e 2069 6e64  th a boolean ind
-000004c0: 6963 6174 696e 6720 6966 2069 7420 6973  icating if it is
-000004d0: 2061 2066 7265 7368 2063 6170 7475 7265   a fresh capture
-000004e0: 2028 5472 7565 2920 6f72 2066 726f 6d20   (True) or from 
-000004f0: 7468 6520 6361 6368 6520 2846 616c 7365  the cache (False
-00000500: 292e 0a0a 6060 6070 7974 686f 6e0a 7361  )...```python.sa
-00000510: 7665 7061 6765 6e6f 772e 6361 7074 7572  vepagenow.captur
-00000520: 655f 6f72 5f63 6163 6865 2822 6874 7470  e_or_cache("http
-00000530: 3a2f 2f77 7777 2e65 7861 6d70 6c65 2e63  ://www.example.c
-00000540: 6f6d 2f22 290a 2822 6874 7470 733a 2f2f  om/").("https://
-00000550: 7765 622e 6172 6368 6976 652e 6f72 672f  web.archive.org/
-00000560: 7765 622f 3230 3136 3130 3139 3036 3238  web/201610190628
-00000570: 3332 2f68 7474 703a 2f2f 7777 772e 6578  32/http://www.ex
-00000580: 616d 706c 652e 636f 6d2f 222c 2054 7275  ample.com/", Tru
-00000590: 6529 0a73 6176 6570 6167 656e 6f77 2e63  e).savepagenow.c
-000005a0: 6170 7475 7265 5f6f 725f 6361 6368 6528  apture_or_cache(
-000005b0: 2268 7474 703a 2f2f 7777 772e 6578 616d  "http://www.exam
-000005c0: 706c 652e 636f 6d2f 2229 0a28 2268 7474  ple.com/").("htt
-000005d0: 7073 3a2f 2f77 6562 2e61 7263 6869 7665  ps://web.archive
-000005e0: 2e6f 7267 2f77 6562 2f32 3031 3631 3031  .org/web/2016101
-000005f0: 3930 3632 3833 322f 6874 7470 3a2f 2f77  9062832/http://w
-00000600: 7777 2e65 7861 6d70 6c65 2e63 6f6d 2f22  ww.example.com/"
-00000610: 2c20 4661 6c73 6529 0a60 6060 0a0a 5468  , False).```..Th
-00000620: 6572 6527 7320 6e6f 2061 6363 6f75 6e74  ere's no account
-00000630: 696e 6720 666f 7220 7461 7374 6520 6275  ing for taste bu
-00000640: 7420 796f 7520 636f 756c 6420 6372 6166  t you could craf
-00000650: 7420 6120 6c69 6e65 2074 6f20 6861 6e64  t a line to hand
-00000660: 6c65 2074 6861 7420 636f 6d6d 616e 6420  le that command 
-00000670: 6c69 6b65 2073 6f3a 0a0a 6060 6070 7974  like so:..```pyt
-00000680: 686f 6e0a 7572 6c2c 2063 6170 7475 7265  hon.url, capture
-00000690: 6420 3d20 7361 7665 7061 6765 6e6f 772e  d = savepagenow.
-000006a0: 6361 7074 7572 655f 6f72 5f63 6163 6865  capture_or_cache
-000006b0: 2822 6874 7470 3a2f 2f77 7777 2e65 7861  ("http://www.exa
-000006c0: 6d70 6c65 2e63 6f6d 2f22 290a 6060 600a  mple.com/").```.
+00000110: 6869 7665 5f75 726c 290a 6060 600a 0a23  hive_url).```..#
+00000120: 2323 2041 7574 6865 6e74 6963 6174 696f  ## Authenticatio
+00000130: 6e2e 0a0a 4279 2064 6566 6175 6c74 2c20  n...By default, 
+00000140: 7361 7665 7061 6765 6e6f 7720 7365 6e64  savepagenow send
+00000150: 7320 616e 6f6e 796d 6f75 7320 7265 7175  s anonymous requ
+00000160: 6573 7473 2c20 7768 6963 6820 6172 6520  ests, which are 
+00000170: 6c69 6d69 7465 6420 746f 2066 6f75 7220  limited to four 
+00000180: 6361 7074 7572 6573 2070 6572 206d 696e  captures per min
+00000190: 7574 652e 0a0a 4175 7468 656e 7469 6361  ute...Authentica
+000001a0: 7465 6420 7265 7175 6573 7473 2061 7265  ted requests are
+000001b0: 2061 6c6c 6f77 6564 2031 3220 6361 7074   allowed 12 capt
+000001c0: 7572 6573 2070 6572 206d 696e 7574 652e  ures per minute.
+000001d0: 2054 6f20 7461 6b65 2061 6476 616e 7461   To take advanta
+000001e0: 6765 206f 6620 7468 6973 2c20 796f 7520  ge of this, you 
+000001f0: 6d75 7374 2072 6567 6973 7465 7220 616e  must register an
+00000200: 2061 6363 6f75 6e74 2077 6974 6820 5b61   account with [a
+00000210: 7263 6869 7665 2e6f 7267 5d28 6874 7470  rchive.org](http
+00000220: 733a 2f2f 6172 6368 6976 652e 6f72 672f  s://archive.org/
+00000230: 6163 636f 756e 742f 6c6f 6769 6e2e 6372  account/login.cr
+00000240: 6561 7465 6163 636f 756e 742e 7068 7029  eateaccount.php)
+00000250: 2061 6e64 0a73 6574 2079 6f75 7220 5b41   and.set your [A
+00000260: 5049 2063 7265 6465 6e74 6961 6c73 5d28  PI credentials](
+00000270: 6874 7470 733a 2f2f 6172 6368 6976 652e  https://archive.
+00000280: 6f72 672f 6163 636f 756e 742f 7333 2e70  org/account/s3.p
+00000290: 6870 2920 746f 2074 6865 206c 6f63 616c  hp) to the local
+000002a0: 2065 6e76 6972 6f6e 6d65 6e74 2076 6172   environment var
+000002b0: 6961 626c 6573 2060 6053 4156 4550 4147  iables ``SAVEPAG
+000002c0: 454e 4f57 5f41 4343 4553 535f 4b45 5960  ENOW_ACCESS_KEY`
+000002d0: 6020 616e 6420 6060 5341 5645 5041 4745  ` and ``SAVEPAGE
+000002e0: 4e4f 575f 5345 4352 4554 5f4b 4559 6060  NOW_SECRET_KEY``
+000002f0: 2e0a 0a54 6865 6e20 796f 7520 6361 6e20  ...Then you can 
+00000300: 7275 6e20 6063 6170 7475 7265 2829 6020  run `capture()` 
+00000310: 7769 7468 2074 6865 2061 7574 6865 6e74  with the authent
+00000320: 6963 6174 6520 666c 6167 2073 6574 2074  icate flag set t
+00000330: 6f20 7472 7565 206c 696b 6520 736f 3a0a  o true like so:.
+00000340: 0a60 6060 7079 7468 6f6e 0a61 7263 6869  .```python.archi
+00000350: 7665 5f75 726c 203d 2073 6176 6570 6167  ve_url = savepag
+00000360: 656e 6f77 2e63 6170 7475 7265 2822 6874  enow.capture("ht
+00000370: 7470 733a 2f2f 7777 772e 6578 616d 706c  tps://www.exampl
+00000380: 652e 636f 6d2f 222c 2061 7574 6865 6e74  e.com/", authent
+00000390: 6963 6174 653d 5472 7565 290a 6060 600a  icate=True).```.
+000003a0: 0a23 2323 2043 6163 6865 6420 7061 6765  .### Cached page
+000003b0: 730a 0a49 6620 6120 5552 4c20 6861 7320  s..If a URL has 
+000003c0: 6265 656e 2072 6563 656e 746c 7920 6361  been recently ca
+000003d0: 6368 6564 2c20 6172 6368 6976 652e 6f72  ched, archive.or
+000003e0: 6720 6d61 7920 7265 7475 726e 2074 6865  g may return the
+000003f0: 2055 524c 2074 6f20 7468 6174 2070 6167   URL to that pag
+00000400: 6520 7261 7468 6572 2074 6861 6e20 636f  e rather than co
+00000410: 6e64 7563 7420 6120 6e65 7720 6361 7074  nduct a new capt
+00000420: 7572 652e 2057 6865 6e20 7468 6174 2068  ure. When that h
+00000430: 6170 7065 6e73 2c20 7468 6520 6060 6361  appens, the ``ca
+00000440: 7074 7572 6560 6020 6d65 7468 6f64 2077  pture`` method w
+00000450: 696c 6c20 7261 6973 6520 6120 6060 4361  ill raise a ``Ca
+00000460: 6368 6564 5061 6765 6060 2065 7863 6570  chedPage`` excep
+00000470: 7469 6f6e 2e0a 0a54 6869 7320 6973 206c  tion...This is l
+00000480: 696b 656c 7920 6861 7070 656e 2069 6620  ikely happen if 
+00000490: 796f 7520 7265 7175 6573 7420 7468 6520  you request the 
+000004a0: 7361 6d65 2055 524c 2074 7769 6365 2077  same URL twice w
+000004b0: 6974 6869 6e20 6120 6665 7720 7365 636f  ithin a few seco
+000004c0: 6e64 732e 0a0a 6060 600a 7361 7665 7061  nds...```.savepa
+000004d0: 6765 6e6f 772e 6361 7074 7572 6528 2268  genow.capture("h
+000004e0: 7474 703a 2f2f 7777 772e 6578 616d 706c  ttp://www.exampl
+000004f0: 652e 636f 6d2f 2229 0a27 6874 7470 733a  e.com/").'https:
+00000500: 2f2f 7765 622e 6172 6368 6976 652e 6f72  //web.archive.or
+00000510: 672f 7765 622f 3230 3136 3130 3139 3036  g/web/2016101906
+00000520: 3236 3337 2f68 7474 703a 2f2f 7777 772e  2637/http://www.
+00000530: 6578 616d 706c 652e 636f 6d2f 270a 7361  example.com/'.sa
+00000540: 7665 7061 6765 6e6f 772e 6361 7074 7572  vepagenow.captur
+00000550: 6528 2268 7474 703a 2f2f 7777 772e 6578  e("http://www.ex
+00000560: 616d 706c 652e 636f 6d2f 2229 0a54 7261  ample.com/").Tra
+00000570: 6365 6261 636b 2028 6d6f 7374 2072 6563  ceback (most rec
+00000580: 656e 7420 6361 6c6c 206c 6173 7429 3a0a  ent call last):.
+00000590: 2020 2046 696c 6520 223c 7374 6469 6e3e     File "<stdin>
+000005a0: 222c 206c 696e 6520 312c 2069 6e20 3c6d  ", line 1, in <m
+000005b0: 6f64 756c 653e 0a20 2020 4669 6c65 2022  odule>.   File "
+000005c0: 7361 7665 7061 6765 6e6f 772f 5f5f 696e  savepagenow/__in
+000005d0: 6974 5f5f 2e70 7922 2c20 6c69 6e65 2033  it__.py", line 3
+000005e0: 362c 2069 6e20 6361 7074 7572 650a 2020  6, in capture.  
+000005f0: 2020 2020 6172 6368 6976 655f 7572 6c0a      archive_url.
+00000600: 7361 7665 7061 6765 6e6f 772e 6578 6365  savepagenow.exce
+00000610: 7074 696f 6e73 2e43 6163 6865 6450 6167  ptions.CachedPag
+00000620: 653a 2061 7263 6869 7665 2e6f 7267 2072  e: archive.org r
+00000630: 6574 7572 6e65 6420 6120 6361 6368 6564  eturned a cached
+00000640: 2076 6572 7369 6f6e 206f 6620 7468 6973   version of this
+00000650: 2070 6167 653a 2068 7474 7073 3a2f 2f77   page: https://w
+00000660: 6562 2e61 7263 6869 7665 2e6f 7267 2f77  eb.archive.org/w
+00000670: 6562 2f32 3031 3631 3031 3930 3632 3633  eb/2016101906263
+00000680: 372f 6874 7470 3a2f 2f77 7777 2e65 7861  7/http://www.exa
+00000690: 6d70 6c65 2e63 6f6d 2f0a 6060 600a 0a59  mple.com/.```..Y
+000006a0: 6f75 2063 616e 2063 7261 6674 2079 6f75  ou can craft you
+000006b0: 7220 636f 6465 2074 6f20 6361 7463 6820  r code to catch 
+000006c0: 7468 6174 2065 7863 6570 7469 6f6e 2079  that exception y
+000006d0: 6f75 7273 656c 662c 206f 7220 7573 6520  ourself, or use 
+000006e0: 7468 6520 6275 696c 742d 696e 2060 6063  the built-in ``c
+000006f0: 6170 7475 7265 5f6f 725f 6361 6368 6560  apture_or_cache`
+00000700: 6020 6d65 7468 6f64 2c20 7768 6963 6820  ` method, which 
+00000710: 7769 6c6c 2072 6574 7572 6e20 7468 6520  will return the 
+00000720: 5552 4c20 7072 6f76 6964 6564 2062 7920  URL provided by 
+00000730: 6172 6368 6976 652e 6f72 6720 616c 6f6e  archive.org alon
+00000740: 6720 7769 7468 2061 2062 6f6f 6c65 616e  g with a boolean
+00000750: 2069 6e64 6963 6174 696e 6720 6966 2069   indicating if i
+00000760: 7420 6973 2061 2066 7265 7368 2063 6170  t is a fresh cap
+00000770: 7475 7265 2028 5472 7565 2920 6f72 2066  ture (True) or f
+00000780: 726f 6d20 7468 6520 6361 6368 6520 2846  rom the cache (F
+00000790: 616c 7365 292e 0a0a 6060 6070 7974 686f  alse)...```pytho
+000007a0: 6e0a 7361 7665 7061 6765 6e6f 772e 6361  n.savepagenow.ca
+000007b0: 7074 7572 655f 6f72 5f63 6163 6865 2822  pture_or_cache("
+000007c0: 6874 7470 3a2f 2f77 7777 2e65 7861 6d70  http://www.examp
+000007d0: 6c65 2e63 6f6d 2f22 290a 2822 6874 7470  le.com/").("http
+000007e0: 733a 2f2f 7765 622e 6172 6368 6976 652e  s://web.archive.
+000007f0: 6f72 672f 7765 622f 3230 3136 3130 3139  org/web/20161019
+00000800: 3036 3238 3332 2f68 7474 703a 2f2f 7777  062832/http://ww
+00000810: 772e 6578 616d 706c 652e 636f 6d2f 222c  w.example.com/",
+00000820: 2054 7275 6529 0a73 6176 6570 6167 656e   True).savepagen
+00000830: 6f77 2e63 6170 7475 7265 5f6f 725f 6361  ow.capture_or_ca
+00000840: 6368 6528 2268 7474 703a 2f2f 7777 772e  che("http://www.
+00000850: 6578 616d 706c 652e 636f 6d2f 2229 0a28  example.com/").(
+00000860: 2268 7474 7073 3a2f 2f77 6562 2e61 7263  "https://web.arc
+00000870: 6869 7665 2e6f 7267 2f77 6562 2f32 3031  hive.org/web/201
+00000880: 3631 3031 3930 3632 3833 322f 6874 7470  61019062832/http
+00000890: 3a2f 2f77 7777 2e65 7861 6d70 6c65 2e63  ://www.example.c
+000008a0: 6f6d 2f22 2c20 4661 6c73 6529 0a60 6060  om/", False).```
+000008b0: 0a0a 5468 6572 6527 7320 6e6f 2061 6363  ..There's no acc
+000008c0: 6f75 6e74 696e 6720 666f 7220 7461 7374  ounting for tast
+000008d0: 6520 6275 7420 796f 7520 636f 756c 6420  e but you could 
+000008e0: 6372 6166 7420 6120 6c69 6e65 2074 6f20  craft a line to 
+000008f0: 6861 6e64 6c65 2074 6861 7420 636f 6d6d  handle that comm
+00000900: 616e 6420 6c69 6b65 2073 6f3a 0a0a 6060  and like so:..``
+00000910: 6070 7974 686f 6e0a 7572 6c2c 2063 6170  `python.url, cap
+00000920: 7475 7265 6420 3d20 7361 7665 7061 6765  tured = savepage
+00000930: 6e6f 772e 6361 7074 7572 655f 6f72 5f63  now.capture_or_c
+00000940: 6163 6865 2822 6874 7470 3a2f 2f77 7777  ache("http://www
+00000950: 2e65 7861 6d70 6c65 2e63 6f6d 2f22 290a  .example.com/").
+00000960: 6060 600a                                ```.
```

### Comparing `savepagenow-1.2.3/docs/_build/html/_sources/useragent.md.txt` & `savepagenow-1.3.0/docs/useragent.md`

 * *Files identical despite different names*

### Comparing `savepagenow-1.2.3/docs/_build/html/_static/css/custom.css` & `savepagenow-1.3.0/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `savepagenow-1.2.3/docs/_templates/nav.html` & `savepagenow-1.3.0/docs/_templates/nav.html`

 * *Files identical despite different names*

### Comparing `savepagenow-1.2.3/docs/conf.py` & `savepagenow-1.3.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # Insert the parent directory into the path
 sys.path.insert(0, os.path.abspath(".."))
 
 extensions = [
     "myst_parser",
     "sphinx.ext.autodoc",
-    "sphinxcontrib.napoleon",
+    "sphinx.ext.napoleon",
     "sphinx_click",
 ]
 templates_path = ["_templates"]
 source_suffix = ".rst"
 master_doc = "index"
 
 project = "savepagenow"
```

### Comparing `savepagenow-1.2.3/docs/make.bat` & `savepagenow-1.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `savepagenow-1.2.3/savepagenow/api.py` & `savepagenow-1.3.0/savepagenow/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,95 @@
+from __future__ import annotations
+
+import os
 import typing
 from urllib.parse import urljoin
 
 import click
 import requests
 from requests.utils import parse_header_links
 
 from .exceptions import (
     BadGateway,
     BlockedByRobots,
     CachedPage,
     Forbidden,
     TooManyRequests,
+    Unauthorized,
     UnknownError,
     WaybackRuntimeError,
 )
 
+DEFAULT_USER_AGENT = "savepagenow (https://github.com/pastpages/savepagenow)"
+
 
 def capture(
-    target_url,
-    user_agent="savepagenow (https://github.com/pastpages/savepagenow)",
-    accept_cache=False,
+    target_url: str,
+    user_agent: str = DEFAULT_USER_AGENT,
+    accept_cache: bool = False,
+    authenticate: bool = False,
 ):
     """
     Archive the provided URL using archive.org's Wayback Machine.
 
     Returns the archive.org URL where the capture is stored.
 
     Raises a CachedPage exception if archive.org declines to conduct a new
     capture and returns a previous snapshot instead.
 
-    To silence that exception, pass into True to the ``accept_cache`` keyword
+    To silence that exception, pass into True to the `accept_cache` keyword
     argument.
+
+    By default the request is anonymous. Pass the `authenticate` flag to
+    login the request. It will use the `SAVEPAGENOW_ACCESS_KEY` and `SAVEPAGENOW_SECRET_KEY`
+    environment variables to authenticate the request.
     """
     # Put together the URL that will save our request
     domain = "https://web.archive.org"
     save_url = urljoin(domain, "/save/")
     request_url = save_url + target_url
 
-    # Send the capture request to archive.org
-    headers = {
-        "User-Agent": user_agent,
-    }
+    # Access Keys for Internet Archive API
+    if authenticate:
+        access_key = os.getenv("SAVEPAGENOW_ACCESS_KEY")
+        secret_key = os.getenv("SAVEPAGENOW_SECRET_KEY")
+        try:
+            assert access_key and secret_key
+        except AssertionError:
+            raise ValueError(
+                "You must set SAVEPAGENOW_ACCESS_KEY and SAVEPAGENOW_SECRET_KEY environment variables to use the authenticate flag"
+            )
+        headers = {
+            "Accept": "application/json",
+            "User-Agent": user_agent,
+            "Authorization": f"LOW {access_key}:{secret_key}",
+            "Content-Type": "application/x-www-form-urlencoded",
+        }
+    else:
+        headers = {
+            "User-Agent": user_agent,
+        }
+
+    # Make the request
     response = requests.get(request_url, headers=headers)
 
     # If it has an error header, raise that.
     has_error_header = "X-Archive-Wayback-Runtime-Error" in response.headers
     if has_error_header:
         error_header = response.headers["X-Archive-Wayback-Runtime-Error"]
         if error_header == "RobotAccessControlException: Blocked By Robots":
             raise BlockedByRobots("archive.org returned blocked by robots.txt error")
         else:
             raise WaybackRuntimeError(error_header)
 
     # If it has an error code, raise that
     status_code = response.status_code
-    if status_code == 403:
+    if status_code == 401:
+        raise Unauthorized("Your archive.org access key and/or secret is not valid")
+    elif status_code == 403:
         raise Forbidden(response.headers)
     elif status_code == 429:
         raise TooManyRequests(response.headers)
     elif status_code == 502:
         raise BadGateway(response.headers)
     elif status_code == 520:
         raise UnknownError(response.headers)
@@ -94,46 +125,78 @@
             raise CachedPage(msg)
 
     # Finally, return the archived URL
     return archive_url
 
 
 def capture_or_cache(
-    target_url, user_agent="savepagenow (https://github.com/pastpages/savepagenow)"
+    target_url: str,
+    user_agent: str = DEFAULT_USER_AGENT,
+    authenticate: bool = False,
 ):
     """
     Archive the provided URL using archive.org's Wayback Machine, unless the page has been recently captured.
 
     Returns a tuple with the archive.org URL where the capture is stored,
     along with a boolean indicating if a new capture was conducted.
 
     If the boolean is True, archive.org conducted a new capture. If it is False,
     archive.org has returned a recently cached capture instead, likely taken
     in the previous minutes.
     """
     try:
-        return capture(target_url, user_agent=user_agent, accept_cache=False), True
+        return (
+            capture(
+                target_url,
+                user_agent=user_agent,
+                accept_cache=False,
+                authenticate=authenticate,
+            ),
+            True,
+        )
     except CachedPage:
-        return capture(target_url, user_agent=user_agent, accept_cache=True), False
+        return (
+            capture(
+                target_url,
+                user_agent=user_agent,
+                accept_cache=True,
+                authenticate=authenticate,
+            ),
+            False,
+        )
 
 
 @click.command()
 @click.argument("url")
 @click.option("-ua", "--user-agent", help="User-Agent header for the web request")
 @click.option("-c", "--accept-cache", help="Accept and return cached URL", is_flag=True)
-def cli(url: str, user_agent: typing.Optional[str] = None, accept_cache: bool = False):
+@click.option(
+    "-a",
+    "--authenticate",
+    help="Allows you to run saves with authentication",
+    is_flag=True,
+)
+def cli(
+    url: str,
+    user_agent: str | None = None,
+    accept_cache: bool = False,
+    authenticate: bool = False,
+):
     """
     Archive the provided URL using archive.org's Wayback Machine.
 
-    Raises a CachedPage exception if archive.org declines to conduct a new capture and returns a previous snapshot instead.
+    Raises a CachedPage exception if archive.org declines to
+    conduct a new capture and returns a previous snapshot instead.
     """
-    kwargs: typing.Dict[typing.Any, typing.Any] = {}
+    kwargs: dict[str, typing.Any] = {}
     if user_agent:
         kwargs["user_agent"] = user_agent
     if accept_cache:
         kwargs["accept_cache"] = accept_cache
+    if authenticate:
+        kwargs["authenticate"] = authenticate
     archive_url = capture(url, **kwargs)
     click.echo(archive_url)
 
 
 if __name__ == "__main__":
-    cli()  # type: ignore
+    cli()
```

### Comparing `savepagenow-1.2.3/savepagenow/exceptions.py` & `savepagenow-1.3.0/savepagenow/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 class CachedPage(Exception):
     """Raised when archive.org declines to make a new capture and instead returns the cached version of most recent archive."""
 
     pass
 
 
 class WaybackRuntimeError(Exception):
-    """An error returned by the Wayback Machine."""
+    """A generic error returned by the Wayback Machine."""
 
     pass
 
 
 class BlockedByRobots(WaybackRuntimeError):
-    """Raised when archive.org has been blocked by the site's robots.txt access control instructions."""
+    """Raised when archive.org has been blocked by the site's robots.txt."""
 
     pass
 
 
 class BadGateway(WaybackRuntimeError):
-    """Raised when archive.org when you receive a 502 bad gateway status code in response to your request."""
+    """Raised when you receive a 502 bad gateway status code."""
+
+    pass
+
+
+class Unauthorized(WaybackRuntimeError):
+    """Raised when you receive a 401 unauthorized status code."""
 
     pass
 
 
 class Forbidden(WaybackRuntimeError):
-    """Raised when archive.org when you receive a 403 forbidden status code in response to your request."""
+    """Raised when you receive a 403 forbidden status code."""
 
     pass
 
 
 class TooManyRequests(WaybackRuntimeError):
-    """Raised when archive.org when you have exceeded its throttle on request frequency. Slow it down."""
+    """Raised when you have exceeded the throttle on request frequency."""
 
     pass
 
 
 class UnknownError(WaybackRuntimeError):
-    """Raised when archive.org when you receive a 520 unknown status code in response to your request."""
+    """Raised when you receive a 520 unknown status code."""
 
     pass
```

### Comparing `savepagenow-1.2.3/savepagenow.egg-info/PKG-INFO` & `savepagenow-1.3.0/savepagenow.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 Metadata-Version: 2.1
 Name: savepagenow
-Version: 1.2.3
+Version: 1.3.0
 Summary: A simple Python wrapper and command-line interface for archive.org’s "Save Page Now" capturing service
 Home-page: https://www.github.com/palewire/savepagenow/
 Author: Ben Welsh
 Author-email: b@palewi.re
 License: MIT
 Project-URL: Documentation, http://palewi.re/docs/savepagenow
 Project-URL: Source, https://github.com/palewire/savepagenow
 Project-URL: Tracker, https://github.com/palewire/savepagenow/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Links
 
 - Documentation: [palewi.re/docs/savepagenow/](https://palewi.re/docs/savepagenow/)
 - Save Page Now at archive.org: [archive.org/web](https://archive.org/web)
 - Code: [github.com/palewire/savepagenow](https://github.com/palewire/savepagenow)
 - Issues: [github.com/palewire/savepagenow/issues](https://github.com/palewire/savepagenow/issues)
 - Packaging: [pypi.org/project/savepagenow](https://pypi.org/project/savepagenow)
-
-
```

### Comparing `savepagenow-1.2.3/setup.py` & `savepagenow-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,18 +56,18 @@
     """,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
     ],
     setup_requires=["setuptools_scm"],
     use_scm_version={"version_scheme": version_scheme, "local_scheme": local_version},
     project_urls={
         "Documentation": "http://palewi.re/docs/savepagenow",
         "Source": "https://github.com/palewire/savepagenow",
```

