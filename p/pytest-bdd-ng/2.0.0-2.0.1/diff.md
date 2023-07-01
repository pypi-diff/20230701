# Comparing `tmp/pytest-bdd-ng-2.0.0.tar.gz` & `tmp/pytest-bdd-ng-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-bdd-ng-2.0.0.tar", last modified: Mon Jun 26 09:57:43 2023, max compression
+gzip compressed data, was "pytest-bdd-ng-2.0.1.tar", last modified: Sat Jul  1 09:59:05 2023, max compression
```

## Comparing `pytest-bdd-ng-2.0.0.tar` & `pytest-bdd-ng-2.0.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:43.129619 pytest-bdd-ng-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-06-26 09:57:43.129619 pytest-bdd-ng-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-26 09:57:43.129619 pytest-bdd-ng-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:43.121619 pytest-bdd-ng-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:43.125619 pytest-bdd-ng-2.0.0/src/pytest_bdd/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/allure_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:43.125619 pytest-bdd-ng-2.0.0/src/pytest_bdd/compatibility/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/compatibility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/compatibility/allure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:43.125619 pytest-bdd-ng-2.0.0/src/pytest_bdd/compatibility/importlib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/compatibility/importlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/compatibility/importlib/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/compatibility/importlib/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/compatibility/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/compatibility/pytest.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/compatibility/struct_bdd.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/compatibility/tomllib.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/compatibility/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/cucumber_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/gherkin_terminal_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/message_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/mimetypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:43.125619 pytest-bdd-ng-2.0.0/src/pytest_bdd/model/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/model/gherkin_document.py
--rw-r--r--   0 runner    (1001) docker     (123)    23640 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/model/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/packaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    11549 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/scenario.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:43.129619 pytest-bdd-ng-2.0.0/src/pytest_bdd/script/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/script/bdd_tree_to_rst.py
--rw-r--r--   0 runner    (1001) docker     (123)    19536 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/steps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:43.129619 pytest-bdd-ng-2.0.0/src/pytest_bdd/struct_bdd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/struct_bdd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14996 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/struct_bdd/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9835 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/struct_bdd/model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/struct_bdd/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/struct_bdd/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:43.129619 pytest-bdd-ng-2.0.0/src/pytest_bdd/template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/template/test.py.mak
--rw-r--r--   0 runner    (1001) docker     (123)     9515 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/warning_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/webloc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:43.129619 pytest-bdd-ng-2.0.0/src/pytest_bdd_ng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-06-26 09:57:43.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd_ng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-26 09:57:43.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd_ng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:57:43.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd_ng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-26 09:57:43.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd_ng.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-26 09:57:43.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd_ng.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 09:57:43.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd_ng.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:43.129619 pytest-bdd-ng-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/tests/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:59:05.141445 pytest-bdd-ng-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-07-01 09:59:05.141445 pytest-bdd-ng-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-01 09:59:05.141445 pytest-bdd-ng-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:59:05.133445 pytest-bdd-ng-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:59:05.137445 pytest-bdd-ng-2.0.1/src/pytest_bdd/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/allure_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:59:05.137445 pytest-bdd-ng-2.0.1/src/pytest_bdd/compatibility/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/compatibility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/compatibility/allure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:59:05.137445 pytest-bdd-ng-2.0.1/src/pytest_bdd/compatibility/importlib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/compatibility/importlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/compatibility/importlib/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/compatibility/importlib/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/compatibility/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/compatibility/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/compatibility/struct_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/compatibility/tomllib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/compatibility/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/cucumber_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/gherkin_terminal_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/message_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/mimetypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:59:05.137445 pytest-bdd-ng-2.0.1/src/pytest_bdd/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/model/gherkin_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23640 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/model/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11549 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/scenario.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:59:05.137445 pytest-bdd-ng-2.0.1/src/pytest_bdd/script/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/script/bdd_tree_to_rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19536 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/steps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:59:05.137445 pytest-bdd-ng-2.0.1/src/pytest_bdd/struct_bdd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/struct_bdd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14996 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/struct_bdd/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9835 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/struct_bdd/model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/struct_bdd/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/struct_bdd/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:59:05.137445 pytest-bdd-ng-2.0.1/src/pytest_bdd/template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/template/test.py.mak
+-rw-r--r--   0 runner    (1001) docker     (123)     9515 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/warning_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd/webloc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:59:05.137445 pytest-bdd-ng-2.0.1/src/pytest_bdd_ng.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-07-01 09:59:05.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd_ng.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-01 09:59:05.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 09:59:05.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-01 09:59:05.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd_ng.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-01 09:59:05.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd_ng.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-01 09:59:05.000000 pytest-bdd-ng-2.0.1/src/pytest_bdd_ng.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:59:05.141445 pytest-bdd-ng-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/tests/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-07-01 09:58:50.000000 pytest-bdd-ng-2.0.1/tests/test_utils.py
```

### Comparing `pytest-bdd-ng-2.0.0/AUTHORS.rst` & `pytest-bdd-ng-2.0.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/LICENSE.txt` & `pytest-bdd-ng-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/PKG-INFO` & `pytest-bdd-ng-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-bdd-ng
-Version: 2.0.0
+Version: 2.0.1
 Summary: BDD for pytest
 Author: Dmitry Kolyagin, Hugo van Kemenade
 Author-email: Oleg Pidsadnyi <oleg.pidsadnyi@gmail.com>, Anatoly Bubenkov <bubenkoff@gmail.com>, Adam Coddington <me@adamcoddington.net>, Albert-Jan Nijburg <albertjan@curit.com>, Alessio Bogon <youtux@gmail.com>, Andrey Makhnach <andrey.makhnach@gmail.com>, Aron Curzon <curzona@gmail.com>, Dmitrijs Milajevs <dimazest@gmail.com>, Florian Bruhin <me@the-compiler.org>, Floris Bruynooghe <flub@devork.be>, Harro van der Klauw <hvdklauw@gmail.com>, Konstantin Goloveshko <kostya.goloveshko@gmail.com>, Laurence Rowe <l@lrowe.co.uk>, Leonardo Santagada <santagada@github.com>, Milosz Sliwinski <sliwinski.milosz@gmail.com>, Michiel Holtkamp <github@elfstone.nl>, Robin Pedersen <ropez@github.com>, Sergey Kraynev <sergejyit@gmail.com>
 Maintainer-email: Konstantin Goloveshko <kostya.goloveshko@gmail.com>
 License: Copyright (C) 2013-2023 Oleg Pidsadnyi, Anatoly Bubenkov and others
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytest-bdd-ng-2.0.0/README.rst` & `pytest-bdd-ng-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/pyproject.toml` & `pytest-bdd-ng-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
   {name="Sergey Kraynev" , email = "sergejyit@gmail.com"},
 ]
 maintainers = [
   {name="Konstantin Goloveshko" , email = "kostya.goloveshko@gmail.com"},
 ]
 license = {file = "LICENSE.txt"}
 urls = {Repository ="https://github.com/elchupanebrej/pytest-bdd-ng"}
-version = "2.0.0"
+version = "2.0.1"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: Pytest",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX",
     "Operating System :: Microsoft :: Windows",
@@ -59,15 +59,15 @@
     "importlib-resources",
     "Mako",
     "ordered_set",
     "packaging",
     "parse",
     "parse_type>=0.6.0",
     "py",
-    "pydantic>=1.0",
+    "pydantic>=1.0, <2.0.0",
     "pytest>=5.0",
     "setuptools>=58",
     "six>=1.16;python_version~='3.8'",
     "types-docopt",
     "typing-extensions;python_version<'3.10.0'",
 ]
```

### Comparing `pytest-bdd-ng-2.0.0/setup.cfg` & `pytest-bdd-ng-2.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/allure_logging.py` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/allure_logging.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/collector.py` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/collector.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/compatibility/parser.py` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/compatibility/parser.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/compatibility/pytest.py` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/compatibility/pytest.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/cucumber_json.py` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/cucumber_json.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/exceptions.py` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/generation.py` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/generation.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/gherkin_terminal_reporter.py` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/gherkin_terminal_reporter.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/hooks.py` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/hooks.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/message_plugin.py` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/message_plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/model/gherkin_document.py` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/model/gherkin_document.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/model/messages.py` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/model/messages.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/packaging.py` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/packaging.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/parser.py` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/parser.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/parsers.py` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/parsers.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/plugin.py` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/reporting.py` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/reporting.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/runner.py` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/runner.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/scenario.py` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/scenario.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/script/bdd_tree_to_rst.py` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/script/bdd_tree_to_rst.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/steps.py` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/steps.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/struct_bdd/model.py` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/struct_bdd/model.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/struct_bdd/model_builder.py` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/struct_bdd/model_builder.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/struct_bdd/parser.py` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/struct_bdd/parser.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/struct_bdd/plugin.py` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/struct_bdd/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/template/test.py.mak` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/template/test.py.mak`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/utils.py` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/utils.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/warning_types.py` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/warning_types.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd/webloc.py` & `pytest-bdd-ng-2.0.1/src/pytest_bdd/webloc.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd_ng.egg-info/PKG-INFO` & `pytest-bdd-ng-2.0.1/src/pytest_bdd_ng.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-bdd-ng
-Version: 2.0.0
+Version: 2.0.1
 Summary: BDD for pytest
 Author: Dmitry Kolyagin, Hugo van Kemenade
 Author-email: Oleg Pidsadnyi <oleg.pidsadnyi@gmail.com>, Anatoly Bubenkov <bubenkoff@gmail.com>, Adam Coddington <me@adamcoddington.net>, Albert-Jan Nijburg <albertjan@curit.com>, Alessio Bogon <youtux@gmail.com>, Andrey Makhnach <andrey.makhnach@gmail.com>, Aron Curzon <curzona@gmail.com>, Dmitrijs Milajevs <dimazest@gmail.com>, Florian Bruhin <me@the-compiler.org>, Floris Bruynooghe <flub@devork.be>, Harro van der Klauw <hvdklauw@gmail.com>, Konstantin Goloveshko <kostya.goloveshko@gmail.com>, Laurence Rowe <l@lrowe.co.uk>, Leonardo Santagada <santagada@github.com>, Milosz Sliwinski <sliwinski.milosz@gmail.com>, Michiel Holtkamp <github@elfstone.nl>, Robin Pedersen <ropez@github.com>, Sergey Kraynev <sergejyit@gmail.com>
 Maintainer-email: Konstantin Goloveshko <kostya.goloveshko@gmail.com>
 License: Copyright (C) 2013-2023 Oleg Pidsadnyi, Anatoly Bubenkov and others
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytest-bdd-ng-2.0.0/src/pytest_bdd_ng.egg-info/SOURCES.txt` & `pytest-bdd-ng-2.0.1/src/pytest_bdd_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/tests/test_hooks.py` & `pytest-bdd-ng-2.0.1/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `pytest-bdd-ng-2.0.0/tests/test_utils.py` & `pytest-bdd-ng-2.0.1/tests/test_utils.py`

 * *Files identical despite different names*

