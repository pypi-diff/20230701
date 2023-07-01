# Comparing `tmp/samp_query-0.4.0.tar.gz` & `tmp/samp_query-0.5.0.tar.gz`

## Comparing `samp_query-0.4.0.tar` & `samp_query-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    12337 2020-02-02 00:00:00.000000 samp_query-0.4.0/samp_query/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 samp_query-0.4.0/samp_query/py.typed
--rw-r--r--   0        0        0     3587 2020-02-02 00:00:00.000000 samp_query-0.4.0/samp_query/rcon.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 samp_query-0.4.0/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 samp_query-0.4.0/LICENSE
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 samp_query-0.4.0/README.md
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 samp_query-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 samp_query-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    12337 2020-02-02 00:00:00.000000 samp_query-0.5.0/samp_query/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 samp_query-0.5.0/samp_query/py.typed
+-rw-r--r--   0        0        0     3587 2020-02-02 00:00:00.000000 samp_query-0.5.0/samp_query/rcon.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 samp_query-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 samp_query-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 samp_query-0.5.0/README.md
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 samp_query-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 samp_query-0.5.0/PKG-INFO
```

### Comparing `samp_query-0.4.0/samp_query/__init__.py` & `samp_query-0.5.0/samp_query/__init__.py`

 * *Files identical despite different names*

### Comparing `samp_query-0.4.0/samp_query/rcon.py` & `samp_query-0.5.0/samp_query/rcon.py`

 * *Files identical despite different names*

### Comparing `samp_query-0.4.0/LICENSE` & `samp_query-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `samp_query-0.4.0/README.md` & `samp_query-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `samp_query-0.4.0/pyproject.toml` & `samp_query-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "samp_query"
-version = "0.4.0"
+version = "0.5.0"
 authors = [
   { name="The Cheaterman", email="the.cheaterman@gmail.com" },
 ]
 description = "A SAMP query/RCON client for Python using trio."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -18,15 +18,16 @@
 ]
 
 [project.scripts]
 samp-rcon = "samp_query.rcon:run"
 
 [project.urls]
 "Homepage" = "https://github.com/Cheaterman/samp-query"
-"Bug Tracker" = "https://github.com/Cheaterman/samp-query/issues"
+"Documentation" = "https://cheaterman.github.io/samp-query/"
+"Issue tracker" = "https://github.com/Cheaterman/samp-query/issues"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
 include = [
```

### Comparing `samp_query-0.4.0/PKG-INFO` & `samp_query-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: samp_query
-Version: 0.4.0
+Version: 0.5.0
 Summary: A SAMP query/RCON client for Python using trio.
 Project-URL: Homepage, https://github.com/Cheaterman/samp-query
-Project-URL: Bug Tracker, https://github.com/Cheaterman/samp-query/issues
+Project-URL: Documentation, https://cheaterman.github.io/samp-query/
+Project-URL: Issue tracker, https://github.com/Cheaterman/samp-query/issues
 Author-email: The Cheaterman <the.cheaterman@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: faust-cchardet
```

