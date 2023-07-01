# Comparing `tmp/py-robocopy-0.0.1.tar.gz` & `tmp/py-robocopy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-robocopy-0.0.1.tar", last modified: Sat Jul  1 19:36:10 2023, max compression
+gzip compressed data, was "py-robocopy-0.0.2.tar", last modified: Sat Jul  1 20:19:58 2023, max compression
```

## Comparing `py-robocopy-0.0.1.tar` & `py-robocopy-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 19:36:10.361024 py-robocopy-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-07-01 14:23:24.000000 py-robocopy-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1118 2023-07-01 19:36:10.360024 py-robocopy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      554 2023-07-01 19:10:46.000000 py-robocopy-0.0.1/README.md
--rw-rw-rw-   0        0        0      552 2023-07-01 19:35:27.000000 py-robocopy-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-01 19:36:10.364028 py-robocopy-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-01 19:36:10.232941 py-robocopy-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-01 19:36:10.345014 py-robocopy-0.0.1/src/py_robocopy.egg-info/
--rw-rw-rw-   0        0        0     1118 2023-07-01 19:36:10.000000 py-robocopy-0.0.1/src/py_robocopy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-07-01 19:36:10.000000 py-robocopy-0.0.1/src/py_robocopy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 19:36:10.000000 py-robocopy-0.0.1/src/py_robocopy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-01 19:36:10.000000 py-robocopy-0.0.1/src/py_robocopy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-01 19:36:10.350018 py-robocopy-0.0.1/src/robocopy/
--rw-rw-rw-   0        0        0        0 2023-07-01 14:09:58.000000 py-robocopy-0.0.1/src/robocopy/__init__.py
--rw-rw-rw-   0        0        0      149 2023-07-01 19:35:16.000000 py-robocopy-0.0.1/src/robocopy/main.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:19:58.183582 py-robocopy-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-07-01 14:23:24.000000 py-robocopy-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1118 2023-07-01 20:19:58.182577 py-robocopy-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2023-07-01 19:10:46.000000 py-robocopy-0.0.2/README.md
+-rw-rw-rw-   0        0        0      552 2023-07-01 20:18:43.000000 py-robocopy-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-01 20:19:58.187583 py-robocopy-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-01 20:19:58.134847 py-robocopy-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-01 20:19:58.173445 py-robocopy-0.0.2/src/py_robocopy.egg-info/
+-rw-rw-rw-   0        0        0     1118 2023-07-01 20:19:58.000000 py-robocopy-0.0.2/src/py_robocopy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-07-01 20:19:58.000000 py-robocopy-0.0.2/src/py_robocopy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 20:19:58.000000 py-robocopy-0.0.2/src/py_robocopy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-01 20:19:58.000000 py-robocopy-0.0.2/src/py_robocopy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 20:19:58.176485 py-robocopy-0.0.2/src/robocopy/
+-rw-rw-rw-   0        0        0        0 2023-07-01 14:09:58.000000 py-robocopy-0.0.2/src/robocopy/__init__.py
+-rw-rw-rw-   0        0        0      147 2023-07-01 20:16:56.000000 py-robocopy-0.0.2/src/robocopy/robocopy.py
```

### Comparing `py-robocopy-0.0.1/LICENSE` & `py-robocopy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py-robocopy-0.0.1/PKG-INFO` & `py-robocopy-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-robocopy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Copies file data from one location to another.
 Author-email: Suyash Sonkesaria <suyashsonkesaria@gmail.com>
 Project-URL: Homepage, https://github.com/suyashsonkesaria/robocopy
 Project-URL: Bug Tracker, https://github.com/suyashsonkesaria/robocopy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `py-robocopy-0.0.1/README.md` & `py-robocopy-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `py-robocopy-0.0.1/pyproject.toml` & `py-robocopy-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "py-robocopy"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Suyash Sonkesaria", email="suyashsonkesaria@gmail.com" },
 ]
 description = "Copies file data from one location to another."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `py-robocopy-0.0.1/src/py_robocopy.egg-info/PKG-INFO` & `py-robocopy-0.0.2/src/py_robocopy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-robocopy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Copies file data from one location to another.
 Author-email: Suyash Sonkesaria <suyashsonkesaria@gmail.com>
 Project-URL: Homepage, https://github.com/suyashsonkesaria/robocopy
 Project-URL: Bug Tracker, https://github.com/suyashsonkesaria/robocopy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

