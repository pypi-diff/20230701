# Comparing `tmp/citation_report-0.1.6.tar.gz` & `tmp/citation_report-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citation_report-0.1.6.tar", max compression
+gzip compressed data, was "citation_report-0.1.7.tar", max compression
```

## Comparing `citation_report-0.1.6.tar` & `citation_report-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1491 2023-06-21 15:17:10.404107 citation_report-0.1.6/LICENSE
--rw-r--r--   0        0        0      163 2023-06-22 10:48:32.510065 citation_report-0.1.6/citation_report/__init__.py
--rw-r--r--   0        0        0     8145 2023-06-29 03:29:16.169891 citation_report-0.1.6/citation_report/main.py
--rw-r--r--   0        0        0     1787 2023-06-22 10:49:27.462730 citation_report-0.1.6/citation_report/published_report.py
--rw-r--r--   0        0        0     3165 2023-06-29 03:16:27.342549 citation_report-0.1.6/citation_report/publisher.py
--rw-r--r--   0        0        0     1375 2023-06-29 02:55:06.603891 citation_report-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      834 1970-01-01 00:00:00.000000 citation_report-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-21 15:17:10.404107 citation_report-0.1.7/LICENSE
+-rw-r--r--   0        0        0      163 2023-06-22 10:48:32.510065 citation_report-0.1.7/citation_report/__init__.py
+-rw-r--r--   0        0        0     8145 2023-06-29 03:29:16.169891 citation_report-0.1.7/citation_report/main.py
+-rw-r--r--   0        0        0     1787 2023-06-22 10:49:27.462730 citation_report-0.1.7/citation_report/published_report.py
+-rw-r--r--   0        0        0     3165 2023-06-29 03:16:27.342549 citation_report-0.1.7/citation_report/publisher.py
+-rw-r--r--   0        0        0     1372 2023-07-01 03:44:57.921582 citation_report-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      837 1970-01-01 00:00:00.000000 citation_report-0.1.7/PKG-INFO
```

### Comparing `citation_report-0.1.6/LICENSE` & `citation_report-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `citation_report-0.1.6/citation_report/main.py` & `citation_report-0.1.7/citation_report/main.py`

 * *Files identical despite different names*

### Comparing `citation_report-0.1.6/citation_report/published_report.py` & `citation_report-0.1.7/citation_report/published_report.py`

 * *Files identical despite different names*

### Comparing `citation_report-0.1.6/citation_report/publisher.py` & `citation_report-0.1.7/citation_report/publisher.py`

 * *Files identical despite different names*

### Comparing `citation_report-0.1.6/pyproject.toml` & `citation_report-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "citation-report"
-version = "0.1.6"
+version = "0.1.7"
 description = "Regex formula of Philippine Supreme Court citations in report format, i.e. SCRA, PHIL, OFFG."
 authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/citation-report"
 documentation = "https://justmars.github.io/citation-report"
 classifiers = [
   "Topic :: Text Processing :: General",
@@ -15,15 +15,15 @@
   "Framework :: Pydantic",
   "Framework :: Pytest",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 citation-date = "^0.1.5"
-pydantic = ">=2.0b3"
+pydantic = "^2.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3"
 pytest-cov = "^2.12.1"
 pre-commit = "^3.3"
 mkdocs = "^1.4.3"
 mkdocstrings = {extras = ["python"], version = "^0.22.0"}
```

### Comparing `citation_report-0.1.6/PKG-INFO` & `citation_report-0.1.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: citation-report
-Version: 0.1.6
+Version: 0.1.7
 Summary: Regex formula of Philippine Supreme Court citations in report format, i.e. SCRA, PHIL, OFFG.
 Home-page: https://lawsql.com
 Author: Marcelino G. Veloso III
 Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pydantic
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Legal Industry
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing :: General
 Classifier: Typing :: Typed
 Requires-Dist: citation-date (>=0.1.5,<0.2.0)
-Requires-Dist: pydantic (>=2.0b3)
+Requires-Dist: pydantic (>=2.0,<3.0)
 Project-URL: Documentation, https://justmars.github.io/citation-report
 Project-URL: Repository, https://github.com/justmars/citation-report
```

