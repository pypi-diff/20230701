# Comparing `tmp/toolcat-0.0.4.tar.gz` & `tmp/toolcat-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolcat-0.0.4.tar", max compression
+gzip compressed data, was "toolcat-0.0.5.tar", max compression
```

## Comparing `toolcat-0.0.4.tar` & `toolcat-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1211 2023-06-03 18:15:32.691464 toolcat-0.0.4/LICENSE
--rw-r--r--   0        0        0      182 2023-06-03 20:00:15.609596 toolcat-0.0.4/README.md
--rw-r--r--   0        0        0     1086 2023-06-04 13:07:01.784435 toolcat-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       24 2023-06-03 18:15:32.694245 toolcat-0.0.4/src/toolcat/__init__.py
--rw-r--r--   0        0        0     2382 2023-06-03 23:01:48.937333 toolcat-0.0.4/src/toolcat/database.py
--rw-r--r--   0        0        0     1400 2023-06-03 23:01:51.316471 toolcat-0.0.4/src/toolcat/database_test.py
--rw-r--r--   0        0        0      607 2023-06-03 18:52:10.387158 toolcat-0.0.4/src/toolcat/project.py
--rw-r--r--   0        0        0     1096 2023-06-03 19:12:14.817042 toolcat-0.0.4/src/toolcat/projects_test.py
--rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 toolcat-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-06-03 18:15:32.691464 toolcat-0.0.5/LICENSE
+-rw-r--r--   0        0        0      182 2023-06-03 20:00:15.609596 toolcat-0.0.5/README.md
+-rw-r--r--   0        0        0     1086 2023-07-01 08:43:26.072517 toolcat-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-06-03 18:15:32.694245 toolcat-0.0.5/src/toolcat/__init__.py
+-rw-r--r--   0        0        0     2382 2023-06-03 23:01:48.937333 toolcat-0.0.5/src/toolcat/database.py
+-rw-r--r--   0        0        0     1400 2023-06-03 23:01:51.316471 toolcat-0.0.5/src/toolcat/database_test.py
+-rw-r--r--   0        0        0      831 2023-07-01 08:42:42.223538 toolcat-0.0.5/src/toolcat/project.py
+-rw-r--r--   0        0        0     1096 2023-06-03 19:12:14.817042 toolcat-0.0.5/src/toolcat/projects_test.py
+-rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 toolcat-0.0.5/PKG-INFO
```

### Comparing `toolcat-0.0.4/LICENSE` & `toolcat-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `toolcat-0.0.4/pyproject.toml` & `toolcat-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 [tool.mypy]
 ignore_missing_imports = true
 # https://stackoverflow.com/questions/62265366/does-mypy-only-type-check-a-function-if-it-declares-a-return-type
 check_untyped_defs = true
 
 [tool.poetry]
 name = "toolcat"
-version = "0.0.4"
+version = "0.0.5"
 description = "Essential Libraries and Tools for Streamlined Development"
 authors = ["Luís Miranda <luistm@gmail.com>"]
 license = "The Unlicence"
 readme = "README.md"
 packages = [{ include = "toolcat", from = "src" }]
 
 [tool.poetry.dependencies]
```

### Comparing `toolcat-0.0.4/src/toolcat/database.py` & `toolcat-0.0.5/src/toolcat/database.py`

 * *Files identical despite different names*

### Comparing `toolcat-0.0.4/src/toolcat/database_test.py` & `toolcat-0.0.5/src/toolcat/database_test.py`

 * *Files identical despite different names*

### Comparing `toolcat-0.0.4/src/toolcat/project.py` & `toolcat-0.0.5/src/toolcat/project.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import importlib.metadata
 from pathlib import Path
 
 import toml
 
 
 def update_version_in_pyproject_toml(version: str, pyproject_path: str) -> None:
     """
@@ -16,7 +17,16 @@
     """
     pyproject_toml_path = Path(pyproject_path)
     pyproject_toml = toml.load(pyproject_toml_path)
     pyproject_toml["tool"]["poetry"]["version"] = version
 
     with open(pyproject_toml_path, "w") as f:
         toml.dump(pyproject_toml, f)
+
+
+def summary(package_name):
+    """
+    Finds the summary for a package.
+    """
+    package = importlib.metadata.metadata(package_name)
+    description = package["Summary"]
+    return description
```

### Comparing `toolcat-0.0.4/src/toolcat/projects_test.py` & `toolcat-0.0.5/src/toolcat/projects_test.py`

 * *Files identical despite different names*

### Comparing `toolcat-0.0.4/PKG-INFO` & `toolcat-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolcat
-Version: 0.0.4
+Version: 0.0.5
 Summary: Essential Libraries and Tools for Streamlined Development
 License: The Unlicence
 Author: Luís Miranda
 Author-email: luistm@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

