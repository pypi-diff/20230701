# Comparing `tmp/templatise-1.0.2.tar.gz` & `tmp/templatise-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templatise-1.0.2.tar", max compression
+gzip compressed data, was "templatise-1.1.2.tar", max compression
```

## Comparing `templatise-1.0.2.tar` & `templatise-1.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1211 2023-03-28 18:12:56.357385 templatise-1.0.2/LICENSE
--rw-r--r--   0        0        0     1861 2023-03-28 18:12:56.357385 templatise-1.0.2/README.md
--rw-r--r--   0        0        0     1778 2023-03-28 18:12:56.357385 templatise-1.0.2/pyproject.toml
--rw-r--r--   0        0        0       19 2023-03-28 18:12:56.357385 templatise-1.0.2/templatise/__init__.py
--rw-r--r--   0        0        0     3813 2023-03-28 18:12:56.357385 templatise-1.0.2/templatise/actions.py
--rw-r--r--   0        0        0     2647 2023-03-28 18:12:56.361386 templatise-1.0.2/templatise/configuration.py
--rw-r--r--   0        0        0      999 2023-03-28 18:12:56.361386 templatise-1.0.2/templatise/git.py
--rw-r--r--   0        0        0     3108 2023-03-28 18:12:56.361386 templatise-1.0.2/templatise/initialise.py
--rw-r--r--   0        0        0     1438 2023-03-28 18:12:56.361386 templatise-1.0.2/templatise/licence.py
--rw-r--r--   0        0        0      994 2023-03-28 18:12:56.361386 templatise-1.0.2/templatise/project_name.py
--rw-r--r--   0        0        0     3558 1970-01-01 00:00:00.000000 templatise-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-01 13:44:58.001272 templatise-1.1.2/LICENSE
+-rw-r--r--   0        0        0     1861 2023-07-01 13:44:58.001272 templatise-1.1.2/README.md
+-rw-r--r--   0        0        0     1778 2023-07-01 13:44:58.001272 templatise-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0       19 2023-07-01 13:44:58.001272 templatise-1.1.2/templatise/__init__.py
+-rw-r--r--   0        0        0     3813 2023-07-01 13:44:58.001272 templatise-1.1.2/templatise/actions.py
+-rw-r--r--   0        0        0     2647 2023-07-01 13:44:58.001272 templatise-1.1.2/templatise/configuration.py
+-rw-r--r--   0        0        0      999 2023-07-01 13:44:58.001272 templatise-1.1.2/templatise/git.py
+-rw-r--r--   0        0        0     3108 2023-07-01 13:44:58.005272 templatise-1.1.2/templatise/initialise.py
+-rw-r--r--   0        0        0     1438 2023-07-01 13:44:58.005272 templatise-1.1.2/templatise/licence.py
+-rw-r--r--   0        0        0      994 2023-07-01 13:44:58.005272 templatise-1.1.2/templatise/project_name.py
+-rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 templatise-1.1.2/PKG-INFO
```

### Comparing `templatise-1.0.2/LICENSE` & `templatise-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `templatise-1.0.2/README.md` & `templatise-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `templatise-1.0.2/pyproject.toml` & `templatise-1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ]
 description = "You can use template.py to create a new GitHub repository."
 keywords = ["python", "template", "vscode", "devcontainers"]
 license = "unlicense"
 name = "templatise"
 readme = "README.md"
 repository = "https://github.com/alunduil/template.py"
-version = "1.0.2"
+version = "1.1.2"
 
 [tool.poetry.dependencies]
 beautifulsoup4 = "^4.11.1"
 click = "^8.1.3"
 click-log = "^0.4.0"
 python = "^3.7.2"
 requests = "^2.28.1"
```

### Comparing `templatise-1.0.2/templatise/actions.py` & `templatise-1.1.2/templatise/actions.py`

 * *Files identical despite different names*

### Comparing `templatise-1.0.2/templatise/configuration.py` & `templatise-1.1.2/templatise/configuration.py`

 * *Files identical despite different names*

### Comparing `templatise-1.0.2/templatise/git.py` & `templatise-1.1.2/templatise/git.py`

 * *Files identical despite different names*

### Comparing `templatise-1.0.2/templatise/initialise.py` & `templatise-1.1.2/templatise/initialise.py`

 * *Files identical despite different names*

### Comparing `templatise-1.0.2/templatise/licence.py` & `templatise-1.1.2/templatise/licence.py`

 * *Files identical despite different names*

### Comparing `templatise-1.0.2/templatise/project_name.py` & `templatise-1.1.2/templatise/project_name.py`

 * *Files identical despite different names*

### Comparing `templatise-1.0.2/PKG-INFO` & `templatise-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templatise
-Version: 1.0.2
+Version: 1.1.2
 Summary: You can use template.py to create a new GitHub repository.
 Home-page: https://github.com/alunduil/template.py
 License: Unlicense
 Keywords: python,template,vscode,devcontainers
 Author: Alex Brandt
 Author-email: alunduil@gmail.com
 Requires-Python: >=3.7.2,<4.0.0
@@ -16,19 +16,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Typing :: Typed
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-log (>=0.4.0,<0.5.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
```

