# Comparing `tmp/ambrosio-0.0.1.tar.gz` & `tmp/ambrosio-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambrosio-0.0.1.tar", max compression
+gzip compressed data, was "ambrosio-0.0.2.tar", max compression
```

## Comparing `ambrosio-0.0.1.tar` & `ambrosio-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1211 2023-07-01 06:56:26.474970 ambrosio-0.0.1/LICENSE
--rw-r--r--   0        0        0      447 2023-07-01 07:47:27.856863 ambrosio-0.0.1/README.md
--rw-r--r--   0        0        0     1051 2023-07-01 07:52:02.027295 ambrosio-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       24 2023-07-01 07:47:27.859411 ambrosio-0.0.1/src/ambrosio/__init__.py
--rw-r--r--   0        0        0       48 2023-07-01 07:47:27.861735 ambrosio-0.0.1/src/ambrosio/ui/__init__.py
--rw-r--r--   0        0        0       81 2023-07-01 07:47:27.862068 ambrosio-0.0.1/src/ambrosio/ui/cli/__init__.py
--rw-r--r--   0        0        0      353 2023-07-01 07:47:48.876114 ambrosio-0.0.1/src/ambrosio/ui/cli/main.py
--rw-r--r--   0        0        0      993 1970-01-01 00:00:00.000000 ambrosio-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-01 06:56:26.474970 ambrosio-0.0.2/LICENSE
+-rw-r--r--   0        0        0      447 2023-07-01 07:47:27.856863 ambrosio-0.0.2/README.md
+-rw-r--r--   0        0        0     1052 2023-07-01 08:23:58.267860 ambrosio-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-07-01 07:47:27.859411 ambrosio-0.0.2/src/ambrosio/__init__.py
+-rw-r--r--   0        0        0       48 2023-07-01 07:47:27.861735 ambrosio-0.0.2/src/ambrosio/ui/__init__.py
+-rw-r--r--   0        0        0       81 2023-07-01 07:47:27.862068 ambrosio-0.0.2/src/ambrosio/ui/cli/__init__.py
+-rw-r--r--   0        0        0      886 2023-07-01 08:22:08.523040 ambrosio-0.0.2/src/ambrosio/ui/cli/main.py
+-rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 ambrosio-0.0.2/PKG-INFO
```

### Comparing `ambrosio-0.0.1/LICENSE` & `ambrosio-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ambrosio-0.0.1/pyproject.toml` & `ambrosio-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 
 [tool.poetry]
 name = "ambrosio"
-version = "0.0.1"
-description = "Ambrosio helps accomplish tasks in the command line"
+version = "0.0.2"
+description = "Ambrosio helps accomplish tasks in the command line."
 authors = ["Luís Miranda <luistm@gmail.com>"]
 license = "The Unlicence"
 readme = "README.md"
 packages = [{ include = "ambrosio", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `ambrosio-0.0.1/PKG-INFO` & `ambrosio-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ambrosio
-Version: 0.0.1
-Summary: Ambrosio helps accomplish tasks in the command line
+Version: 0.0.2
+Summary: Ambrosio helps accomplish tasks in the command line.
 License: The Unlicence
 Author: Luís Miranda
 Author-email: luistm@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

