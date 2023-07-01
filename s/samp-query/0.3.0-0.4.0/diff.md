# Comparing `tmp/samp_query-0.3.0.tar.gz` & `tmp/samp_query-0.4.0.tar.gz`

## Comparing `samp_query-0.3.0.tar` & `samp_query-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    12337 2020-02-02 00:00:00.000000 samp_query-0.3.0/samp_query/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 samp_query-0.3.0/samp_query/py.typed
--rw-r--r--   0        0        0     3587 2020-02-02 00:00:00.000000 samp_query-0.3.0/samp_query/rcon.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 samp_query-0.3.0/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 samp_query-0.3.0/LICENSE
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 samp_query-0.3.0/README.md
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 samp_query-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 samp_query-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    12337 2020-02-02 00:00:00.000000 samp_query-0.4.0/samp_query/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 samp_query-0.4.0/samp_query/py.typed
+-rw-r--r--   0        0        0     3587 2020-02-02 00:00:00.000000 samp_query-0.4.0/samp_query/rcon.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 samp_query-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 samp_query-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 samp_query-0.4.0/README.md
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 samp_query-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 samp_query-0.4.0/PKG-INFO
```

### Comparing `samp_query-0.3.0/samp_query/__init__.py` & `samp_query-0.4.0/samp_query/__init__.py`

 * *Files identical despite different names*

### Comparing `samp_query-0.3.0/samp_query/rcon.py` & `samp_query-0.4.0/samp_query/rcon.py`

 * *Files identical despite different names*

### Comparing `samp_query-0.3.0/LICENSE` & `samp_query-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `samp_query-0.3.0/README.md` & `samp_query-0.4.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-samp_query
+samp-query
 ==========
 
 [![CI](https://github.com/Cheaterman/samp-query/actions/workflows/ci.yml/badge.svg)](https://github.com/Cheaterman/samp-query/actions/workflows/ci.yml)
 
+![samp-query logo](https://cheaterman.github.io/samp-query/_static/favicon.ico)
+
 samp-query is a Python library for interacting with SA-MP/open.mp servers using the query protocol.
 It provides functionality to query server information, retrieve player list, show rules, and execute remote console (RCON) commands.
 
 Installation
 ------------
 
 To install the library, you can use `pip`:
@@ -36,15 +38,14 @@
 
 async def main():
     client = Client(
         ip='127.0.0.1',
         port=7777,
         rcon_password=None,  # Your rcon password as string
     )
-    await client.connect()
 
     info = await client.info()
     print(f'Server Name: {info.name}')
     print(f'Player Count: {info.players}/{info.max_players}')
 
     player_list = await client.players()
     print('Players:')
```

### Comparing `samp_query-0.3.0/pyproject.toml` & `samp_query-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "samp_query"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
   { name="The Cheaterman", email="the.cheaterman@gmail.com" },
 ]
 description = "A SAMP query/RCON client for Python using trio."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `samp_query-0.3.0/PKG-INFO` & `samp_query-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: samp_query
-Version: 0.3.0
+Version: 0.4.0
 Summary: A SAMP query/RCON client for Python using trio.
 Project-URL: Homepage, https://github.com/Cheaterman/samp-query
 Project-URL: Bug Tracker, https://github.com/Cheaterman/samp-query/issues
 Author-email: The Cheaterman <the.cheaterman@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: faust-cchardet
 Requires-Dist: trio
 Description-Content-Type: text/markdown
 
-samp_query
+samp-query
 ==========
 
 [![CI](https://github.com/Cheaterman/samp-query/actions/workflows/ci.yml/badge.svg)](https://github.com/Cheaterman/samp-query/actions/workflows/ci.yml)
 
+![samp-query logo](https://cheaterman.github.io/samp-query/_static/favicon.ico)
+
 samp-query is a Python library for interacting with SA-MP/open.mp servers using the query protocol.
 It provides functionality to query server information, retrieve player list, show rules, and execute remote console (RCON) commands.
 
 Installation
 ------------
 
 To install the library, you can use `pip`:
@@ -52,15 +54,14 @@
 
 async def main():
     client = Client(
         ip='127.0.0.1',
         port=7777,
         rcon_password=None,  # Your rcon password as string
     )
-    await client.connect()
 
     info = await client.info()
     print(f'Server Name: {info.name}')
     print(f'Player Count: {info.players}/{info.max_players}')
 
     player_list = await client.players()
     print('Players:')
```

