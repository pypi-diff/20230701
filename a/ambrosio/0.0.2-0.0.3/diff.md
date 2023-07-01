# Comparing `tmp/ambrosio-0.0.2.tar.gz` & `tmp/ambrosio-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambrosio-0.0.2.tar", max compression
+gzip compressed data, was "ambrosio-0.0.3.tar", max compression
```

## Comparing `ambrosio-0.0.2.tar` & `ambrosio-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1211 2023-07-01 06:56:26.474970 ambrosio-0.0.2/LICENSE
--rw-r--r--   0        0        0      447 2023-07-01 07:47:27.856863 ambrosio-0.0.2/README.md
--rw-r--r--   0        0        0     1052 2023-07-01 08:23:58.267860 ambrosio-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       24 2023-07-01 07:47:27.859411 ambrosio-0.0.2/src/ambrosio/__init__.py
--rw-r--r--   0        0        0       48 2023-07-01 07:47:27.861735 ambrosio-0.0.2/src/ambrosio/ui/__init__.py
--rw-r--r--   0        0        0       81 2023-07-01 07:47:27.862068 ambrosio-0.0.2/src/ambrosio/ui/cli/__init__.py
--rw-r--r--   0        0        0      886 2023-07-01 08:22:08.523040 ambrosio-0.0.2/src/ambrosio/ui/cli/main.py
--rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 ambrosio-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-01 06:56:26.474970 ambrosio-0.0.3/LICENSE
+-rw-r--r--   0        0        0      447 2023-07-01 07:47:27.856863 ambrosio-0.0.3/README.md
+-rw-r--r--   0        0        0     1052 2023-07-01 10:45:21.280733 ambrosio-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-07-01 07:47:27.859411 ambrosio-0.0.3/src/ambrosio/__init__.py
+-rw-r--r--   0        0        0       48 2023-07-01 07:47:27.861735 ambrosio-0.0.3/src/ambrosio/ui/__init__.py
+-rw-r--r--   0        0        0       81 2023-07-01 07:47:27.862068 ambrosio-0.0.3/src/ambrosio/ui/cli/__init__.py
+-rw-r--r--   0        0        0      633 2023-07-01 10:24:19.630149 ambrosio-0.0.3/src/ambrosio/ui/cli/main.py
+-rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 ambrosio-0.0.3/PKG-INFO
```

### Comparing `ambrosio-0.0.2/LICENSE` & `ambrosio-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ambrosio-0.0.2/pyproject.toml` & `ambrosio-0.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -7,39 +7,39 @@
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 
 [tool.poetry]
 name = "ambrosio"
-version = "0.0.2"
+version = "0.0.3"
 description = "Ambrosio helps accomplish tasks in the command line."
 authors = ["Luís Miranda <luistm@gmail.com>"]
 license = "The Unlicence"
 readme = "README.md"
 packages = [{ include = "ambrosio", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 awesome-slugify = "^1.6.5"
+toolcat = "^0.0.5"
 typer = "^0.9.0"
 
 [tool.poetry.group.dev.dependencies]
 bandit = { extras = ["toml"], version = "^1.7.5" }
 behave = "^1.2.6"
 black = "^23.3.0"
 coverage = "^7.2.7"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 nox = "^2023.4.22"
 pre-commit = "^3.3.3"
 pytest = "^7.4.0"
 pytest-bdd = "^6.1.1"
 pytest-xdist = "^3.3.1"
-toolcat = "^0.0.4"
 types-python-slugify = "^8.0.0.2"
 
 [tool.poetry.scripts]
 ambrosio = "ambrosio.ui.cli.main:app"
 am = "ambrosio.ui.cli.main:app"
```

### Comparing `ambrosio-0.0.2/PKG-INFO` & `ambrosio-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: ambrosio
-Version: 0.0.2
+Version: 0.0.3
 Summary: Ambrosio helps accomplish tasks in the command line.
 License: The Unlicence
 Author: Luís Miranda
 Author-email: luistm@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: awesome-slugify (>=1.6.5,<2.0.0)
+Requires-Dist: toolcat (>=0.0.5,<0.0.6)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # Ambrosio
 
 Ambrosio helps accomplish tasks in the command line
```

