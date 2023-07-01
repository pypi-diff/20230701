# Comparing `tmp/cheetah_lint-1.3.1.tar.gz` & `tmp/cheetah_lint-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheetah_lint-1.3.1.tar", last modified: Sat Jul  2 16:32:43 2022, max compression
+gzip compressed data, was "cheetah_lint-1.4.0.tar", last modified: Sat Jul  1 18:53:35 2023, max compression
```

## Comparing `cheetah_lint-1.3.1.tar` & `cheetah_lint-1.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-07-02 16:32:43.119142 cheetah_lint-1.3.1/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2022-07-02 00:11:12.000000 cheetah_lint-1.3.1/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2230 2022-07-02 16:32:43.119142 cheetah_lint-1.3.1/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1458 2022-07-02 00:11:12.000000 cheetah_lint-1.3.1/README.md
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-07-02 16:32:43.119142 cheetah_lint-1.3.1/cheetah_lint/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-07-02 00:11:12.000000 cheetah_lint-1.3.1/cheetah_lint/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1336 2022-07-02 16:32:41.000000 cheetah_lint-1.3.1/cheetah_lint/directives.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    12830 2022-07-02 00:11:12.000000 cheetah_lint-1.3.1/cheetah_lint/flake.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      981 2022-07-02 16:32:41.000000 cheetah_lint-1.3.1/cheetah_lint/imports.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4870 2022-07-02 00:19:15.000000 cheetah_lint-1.3.1/cheetah_lint/reorder_imports.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      128 2022-07-02 00:11:12.000000 cheetah_lint-1.3.1/cheetah_lint/util.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-07-02 16:32:43.119142 cheetah_lint-1.3.1/cheetah_lint.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2230 2022-07-02 16:32:42.000000 cheetah_lint-1.3.1/cheetah_lint.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      405 2022-07-02 16:32:42.000000 cheetah_lint-1.3.1/cheetah_lint.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2022-07-02 16:32:42.000000 cheetah_lint-1.3.1/cheetah_lint.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)      118 2022-07-02 16:32:42.000000 cheetah_lint-1.3.1/cheetah_lint.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)      115 2022-07-02 16:32:42.000000 cheetah_lint-1.3.1/cheetah_lint.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       13 2022-07-02 16:32:42.000000 cheetah_lint-1.3.1/cheetah_lint.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1492 2022-07-02 16:32:43.119142 cheetah_lint-1.3.1/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-07-02 00:11:12.000000 cheetah_lint-1.3.1/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-01 18:53:35.392555 cheetah_lint-1.4.0/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-07-01 18:48:44.000000 cheetah_lint-1.4.0/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1792 2023-07-01 18:53:35.392555 cheetah_lint-1.4.0/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1241 2023-07-01 18:48:44.000000 cheetah_lint-1.4.0/README.md
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-01 18:53:35.388555 cheetah_lint-1.4.0/cheetah_lint/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-07-01 18:48:44.000000 cheetah_lint-1.4.0/cheetah_lint/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1336 2023-07-01 18:48:44.000000 cheetah_lint-1.4.0/cheetah_lint/directives.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    12777 2023-07-01 18:48:44.000000 cheetah_lint-1.4.0/cheetah_lint/flake.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      976 2023-07-01 18:49:09.000000 cheetah_lint-1.4.0/cheetah_lint/imports.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4870 2023-07-01 18:48:44.000000 cheetah_lint-1.4.0/cheetah_lint/reorder_imports.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      128 2023-07-01 18:48:44.000000 cheetah_lint-1.4.0/cheetah_lint/util.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-01 18:53:35.388555 cheetah_lint-1.4.0/cheetah_lint.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1792 2023-07-01 18:53:35.000000 cheetah_lint-1.4.0/cheetah_lint.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      405 2023-07-01 18:53:35.000000 cheetah_lint-1.4.0/cheetah_lint.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-07-01 18:53:35.000000 cheetah_lint-1.4.0/cheetah_lint.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      118 2023-07-01 18:53:35.000000 cheetah_lint-1.4.0/cheetah_lint.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       99 2023-07-01 18:53:35.000000 cheetah_lint-1.4.0/cheetah_lint.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       13 2023-07-01 18:53:35.000000 cheetah_lint-1.4.0/cheetah_lint.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1291 2023-07-01 18:53:35.392555 cheetah_lint-1.4.0/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-07-01 18:48:44.000000 cheetah_lint-1.4.0/setup.py
```

### Comparing `cheetah_lint-1.3.1/LICENSE` & `cheetah_lint-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cheetah_lint-1.3.1/PKG-INFO` & `cheetah_lint-1.4.0/cheetah_lint.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 Metadata-Version: 2.1
-Name: cheetah_lint
-Version: 1.3.1
+Name: cheetah-lint
+Version: 1.4.0
 Summary: Linting tools for the Cheetah templating language.
 Home-page: https://github.com/asottile/cheetah_lint
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.cheetah_lint?branchName=main)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=41&branchName=main)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/41/main.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=41&branchName=main)
+[![build status](https://github.com/asottile/cheetah_lint/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/cheetah_lint/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/cheetah_lint/main.svg)](https://results.pre-commit.ci/latest/github/asottile/cheetah_lint/main)
 
 cheetah_lint
 ============
 
 Linting tools for the [yelp_cheetah](https://github.com/Yelp/yelp_cheetah) templating language.
 
 
 ## Installation
 
-`pip install cheetah-lint`
+```bash
+pip install cheetah-lint
+```
 
 
 ## Console scripts
 
 ```console
 $ cheetah-reorder-imports --help
 usage: cheetah-reorder-imports [-h] [filenames [filenames ...]]
@@ -61,9 +57,7 @@
 ## As a pre-commit hook
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Hooks available:
 - `cheetah-reorder-imports` - This hook reorders imports in cheetah files.
 - `cheetah-flake` - Lint cheetah code using flake8 and some other checks.
-
-
```

### Comparing `cheetah_lint-1.3.1/README.md` & `cheetah_lint-1.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.cheetah_lint?branchName=main)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=41&branchName=main)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/41/main.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=41&branchName=main)
+[![build status](https://github.com/asottile/cheetah_lint/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/cheetah_lint/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/cheetah_lint/main.svg)](https://results.pre-commit.ci/latest/github/asottile/cheetah_lint/main)
 
 cheetah_lint
 ============
 
 Linting tools for the [yelp_cheetah](https://github.com/Yelp/yelp_cheetah) templating language.
 
 
 ## Installation
 
-`pip install cheetah-lint`
+```bash
+pip install cheetah-lint
+```
 
 
 ## Console scripts
 
 ```console
 $ cheetah-reorder-imports --help
 usage: cheetah-reorder-imports [-h] [filenames [filenames ...]]
```

### Comparing `cheetah_lint-1.3.1/cheetah_lint/directives.py` & `cheetah_lint-1.4.0/cheetah_lint/directives.py`

 * *Files identical despite different names*

### Comparing `cheetah_lint-1.3.1/cheetah_lint/flake.py` & `cheetah_lint-1.4.0/cheetah_lint/flake.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,16 +62,14 @@
     'E712',
     # test for membership should be 'not in'
     'E713',
     # test for object identity should be 'is not'
     'E714',
     # SyntaxError
     'E999',
-    # .has_key() is deprecated, use 'in'
-    'W601',
     # invalid escape sequence
     'W605',
 ))
 
 
 class NoCompilerSettingsCompiler(LegacyCompiler):
     def add_compiler_settings(self) -> None:
```

### Comparing `cheetah_lint-1.3.1/cheetah_lint/imports.py` & `cheetah_lint-1.4.0/cheetah_lint/imports.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
+from functools import cached_property
+
 import lxml.etree
-from cached_property import cached_property
 from classify_imports import Import
 from classify_imports import import_obj_from_str
 from classify_imports import ImportFrom
 
 
 def combine_import_objs(import_objs: Import | ImportFrom) -> str:
     return ''.join(f'#{import_obj}' for import_obj in import_objs)
```

### Comparing `cheetah_lint-1.3.1/cheetah_lint/reorder_imports.py` & `cheetah_lint-1.4.0/cheetah_lint/reorder_imports.py`

 * *Files identical despite different names*

### Comparing `cheetah_lint-1.3.1/cheetah_lint.egg-info/PKG-INFO` & `cheetah_lint-1.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 Metadata-Version: 2.1
-Name: cheetah-lint
-Version: 1.3.1
+Name: cheetah_lint
+Version: 1.4.0
 Summary: Linting tools for the Cheetah templating language.
 Home-page: https://github.com/asottile/cheetah_lint
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.cheetah_lint?branchName=main)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=41&branchName=main)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/41/main.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=41&branchName=main)
+[![build status](https://github.com/asottile/cheetah_lint/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/cheetah_lint/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/cheetah_lint/main.svg)](https://results.pre-commit.ci/latest/github/asottile/cheetah_lint/main)
 
 cheetah_lint
 ============
 
 Linting tools for the [yelp_cheetah](https://github.com/Yelp/yelp_cheetah) templating language.
 
 
 ## Installation
 
-`pip install cheetah-lint`
+```bash
+pip install cheetah-lint
+```
 
 
 ## Console scripts
 
 ```console
 $ cheetah-reorder-imports --help
 usage: cheetah-reorder-imports [-h] [filenames [filenames ...]]
@@ -61,9 +57,7 @@
 ## As a pre-commit hook
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Hooks available:
 - `cheetah-reorder-imports` - This hook reorders imports in cheetah files.
 - `cheetah-flake` - Lint cheetah code using flake8 and some other checks.
-
-
```

### Comparing `cheetah_lint-1.3.1/setup.cfg` & `cheetah_lint-1.4.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,32 @@
 [metadata]
 name = cheetah_lint
-version = 1.3.1
+version = 1.4.0
 description = Linting tools for the Cheetah templating language.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/cheetah_lint
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: Implementation :: CPython
 
 [options]
 packages = find:
 install_requires = 
-	cached-property
 	classify-imports
-	flake8>=3
+	flake8>=6
 	refactorlib[cheetah]>=0.15.0,<=0.15.999
 	yelp-cheetah>=0.19.0,<=0.19.999
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.packages.find]
 exclude = 
 	tests*
 	testing*
 
 [options.entry_points]
@@ -46,15 +41,14 @@
 plugins = covdefaults
 
 [mypy]
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
-no_implicit_optional = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 
 [mypy-testing.*]
 disallow_untyped_defs = false
 
 [mypy-tests.*]
```

