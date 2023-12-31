# Comparing `tmp/datascience_cookiecutter-0.1.1.tar.gz` & `tmp/datascience_cookiecutter-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datascience_cookiecutter-0.1.1.tar", last modified: Sat Jul  1 21:32:35 2023, max compression
+gzip compressed data, was "datascience_cookiecutter-0.1.2.tar", last modified: Sat Jul  1 21:35:32 2023, max compression
```

## Comparing `datascience_cookiecutter-0.1.1.tar` & `datascience_cookiecutter-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      909 2023-07-01 21:28:19.151138 datascience_cookiecutter-0.1.1/README.md
--rw-r--r--   0        0        0      161 2023-07-01 21:32:11.821252 datascience_cookiecutter-0.1.1/datascience_cookiecutter/__init__.py
--rw-r--r--   0        0        0      490 2023-07-01 21:31:26.287090 datascience_cookiecutter-0.1.1/datascience_cookiecutter/cli.py
--rw-r--r--   0        0        0     3910 2023-07-01 21:30:54.160107 datascience_cookiecutter-0.1.1/datascience_cookiecutter/folderbuilder.py
--rw-r--r--   0        0        0     3363 2023-07-01 20:48:08.567048 datascience_cookiecutter-0.1.1/datascience_cookiecutter/templates.py
--rw-r--r--   0        0        0      833 2023-07-01 21:32:35.286332 datascience_cookiecutter-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     8042 2023-06-30 22:34:34.542238 datascience_cookiecutter-0.1.1/tests/test_datascience_cookiecutter.py
--rw-r--r--   0        0        0     1539 1970-01-01 00:00:00.000000 datascience_cookiecutter-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      909 2023-07-01 21:28:19.151138 datascience_cookiecutter-0.1.2/README.md
+-rw-r--r--   0        0        0      161 2023-07-01 21:35:26.303545 datascience_cookiecutter-0.1.2/datascience_cookiecutter/__init__.py
+-rw-r--r--   0        0        0      490 2023-07-01 21:31:26.287090 datascience_cookiecutter-0.1.2/datascience_cookiecutter/cli.py
+-rw-r--r--   0        0        0     3910 2023-07-01 21:30:54.160107 datascience_cookiecutter-0.1.2/datascience_cookiecutter/folderbuilder.py
+-rw-r--r--   0        0        0     3363 2023-07-01 20:48:08.567048 datascience_cookiecutter-0.1.2/datascience_cookiecutter/templates.py
+-rw-r--r--   0        0        0      838 2023-07-01 21:35:32.740285 datascience_cookiecutter-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     8042 2023-06-30 22:34:34.542238 datascience_cookiecutter-0.1.2/tests/test_datascience_cookiecutter.py
+-rw-r--r--   0        0        0     1539 1970-01-01 00:00:00.000000 datascience_cookiecutter-0.1.2/PKG-INFO
```

### Comparing `datascience_cookiecutter-0.1.1/README.md` & `datascience_cookiecutter-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `datascience_cookiecutter-0.1.1/datascience_cookiecutter/folderbuilder.py` & `datascience_cookiecutter-0.1.2/datascience_cookiecutter/folderbuilder.py`

 * *Files identical despite different names*

### Comparing `datascience_cookiecutter-0.1.1/datascience_cookiecutter/templates.py` & `datascience_cookiecutter-0.1.2/datascience_cookiecutter/templates.py`

 * *Files identical despite different names*

### Comparing `datascience_cookiecutter-0.1.1/pyproject.toml` & `datascience_cookiecutter-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "datascience-cookiecutter"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = [
     { name = "", email = "" },
 ]
 dependencies = [
     "pydantic>=2.0",
     "loguru>=0.7.0",
@@ -31,15 +31,15 @@
     "mypy>=1.4.1",
 ]
 
 [tool.pdm.urls]
 GitHub = "https://github.com/raoulg/datascience-cookiecutter"
 
 [tool.pdm.scripts.cookiecutter]
-call = "datascience_cookiecutter.cli"
+call = "datascience_cookiecutter.cli:main"
 deps = [
     "click",
 ]
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `datascience_cookiecutter-0.1.1/tests/test_datascience_cookiecutter.py` & `datascience_cookiecutter-0.1.2/tests/test_datascience_cookiecutter.py`

 * *Files identical despite different names*

### Comparing `datascience_cookiecutter-0.1.1/PKG-INFO` & `datascience_cookiecutter-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datascience-cookiecutter
-Version: 0.1.1
+Version: 0.1.2
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Environment :: Console
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Requires-Dist: pydantic>=2.0
```

