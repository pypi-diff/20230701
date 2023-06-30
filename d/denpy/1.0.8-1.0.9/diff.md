# Comparing `tmp/denpy-1.0.8.tar.gz` & `tmp/denpy-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denpy-1.0.8.tar", last modified: Mon Jun 19 21:18:38 2023, max compression
+gzip compressed data, was "denpy-1.0.9.tar", last modified: Fri Jun 30 23:45:06 2023, max compression
```

## Comparing `denpy-1.0.8.tar` & `denpy-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 21:18:38.698305 denpy-1.0.8/
--rw-rw-rw-   0        0        0      112 2023-06-19 21:18:38.697308 denpy-1.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-19 21:18:38.693318 denpy-1.0.8/denpy/
--rw-rw-rw-   0        0        0      137 2023-05-31 18:58:29.000000 denpy-1.0.8/denpy/__init__.py
--rw-rw-rw-   0        0        0      401 2023-06-01 15:01:37.000000 denpy-1.0.8/denpy/color.py
--rw-rw-rw-   0        0        0     1820 2023-06-19 20:04:44.000000 denpy-1.0.8/denpy/database.py
--rw-rw-rw-   0        0        0     1120 2023-06-17 16:24:29.000000 denpy-1.0.8/denpy/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-19 21:18:38.696310 denpy-1.0.8/denpy.egg-info/
--rw-rw-rw-   0        0        0      112 2023-06-19 21:18:38.000000 denpy-1.0.8/denpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-06-19 21:18:38.000000 denpy-1.0.8/denpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 21:18:38.000000 denpy-1.0.8/denpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-19 21:18:38.000000 denpy-1.0.8/denpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 21:18:38.698305 denpy-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      205 2023-06-19 21:18:19.000000 denpy-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 23:45:06.511959 denpy-1.0.9/
+-rw-rw-rw-   0        0        0      102 2023-06-30 23:45:06.510962 denpy-1.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-30 23:45:06.506973 denpy-1.0.9/denpy/
+-rw-rw-rw-   0        0        0      137 2023-05-31 18:58:29.000000 denpy-1.0.9/denpy/__init__.py
+-rw-rw-rw-   0        0        0      401 2023-06-01 15:01:37.000000 denpy-1.0.9/denpy/color.py
+-rw-rw-rw-   0        0        0     1917 2023-06-30 23:33:16.000000 denpy-1.0.9/denpy/database.py
+-rw-rw-rw-   0        0        0     1120 2023-06-17 16:24:29.000000 denpy-1.0.9/denpy/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 23:45:06.510962 denpy-1.0.9/denpy.egg-info/
+-rw-rw-rw-   0        0        0      102 2023-06-30 23:45:06.000000 denpy-1.0.9/denpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-06-30 23:45:06.000000 denpy-1.0.9/denpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 23:45:06.000000 denpy-1.0.9/denpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-30 23:45:06.000000 denpy-1.0.9/denpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 23:45:06.511959 denpy-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      195 2023-06-30 23:44:46.000000 denpy-1.0.9/setup.py
```

### Comparing `denpy-1.0.8/denpy/database.py` & `denpy-1.0.9/denpy/database.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import sqlite3
 
-def connect(__file__: str) -> tuple[sqlite3.Connection, sqlite3.Cursor]:
+def connect(__file__: str, file_name: str = None) -> tuple[sqlite3.Connection, sqlite3.Cursor]:
     path = __file__.replace('\\', '/').split('/')
     path.pop(-1)
     path.pop(-1)
-    path.append('database.db')
+    if file_name is None:
+        path.append('database.db')
+    else:
+        path.append(file_name)
     database = sqlite3.connect('/'.join(path))
     cursor = database.cursor()
     return database, cursor
 
 def disconnect(database: sqlite3.Connection, cursor: sqlite3.Cursor):
     database.commit()
     cursor.close()
```

### Comparing `denpy-1.0.8/denpy/utils.py` & `denpy-1.0.9/denpy/utils.py`

 * *Files identical despite different names*

