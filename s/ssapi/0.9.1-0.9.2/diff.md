# Comparing `tmp/ssapi-0.9.1.tar.gz` & `tmp/ssapi-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssapi-0.9.1.tar", last modified: Sat Jul  1 11:13:05 2023, max compression
+gzip compressed data, was "ssapi-0.9.2.tar", last modified: Sat Jul  1 11:57:07 2023, max compression
```

## Comparing `ssapi-0.9.1.tar` & `ssapi-0.9.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-07-01 11:13:05.389990 ssapi-0.9.1/
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      143 2023-07-01 11:13:05.389990 ssapi-0.9.1/PKG-INFO
--rw-rw-r--   0 zedr      (1000) zedr      (1000)       30 2023-06-10 16:26:54.000000 ssapi-0.9.1/pyproject.toml
-drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-07-01 11:13:05.386990 ssapi-0.9.1/scripts/
--rwxr-xr-x   0 zedr      (1000) zedr      (1000)      497 2023-04-30 10:24:27.000000 ssapi-0.9.1/scripts/ssapi-web
--rw-rw-r--   0 zedr      (1000) zedr      (1000)       38 2023-07-01 11:13:05.390990 ssapi-0.9.1/setup.cfg
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      272 2023-07-01 11:11:01.000000 ssapi-0.9.1/setup.py
-drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-07-01 11:13:05.386990 ssapi-0.9.1/src/
-drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-07-01 11:13:05.388990 ssapi-0.9.1/src/ssapi/
--rw-rw-r--   0 zedr      (1000) zedr      (1000)        0 2022-09-17 12:56:21.000000 ssapi-0.9.1/src/ssapi/__init__.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)     4537 2023-07-01 11:07:20.000000 ssapi-0.9.1/src/ssapi/db.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)     1983 2023-06-10 16:51:23.000000 ssapi-0.9.1/src/ssapi/db_utils.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      201 2023-06-10 16:26:54.000000 ssapi-0.9.1/src/ssapi/defaults.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      856 2023-07-01 11:07:20.000000 ssapi-0.9.1/src/ssapi/entities.py
--rw-r--r--   0 zedr      (1000) zedr      (1000)      631 2023-04-30 11:11:55.000000 ssapi-0.9.1/src/ssapi/env.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      363 2023-06-10 16:26:54.000000 ssapi-0.9.1/src/ssapi/exceptions.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)     2397 2023-06-10 16:26:54.000000 ssapi-0.9.1/src/ssapi/relational.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      826 2023-06-10 16:26:54.000000 ssapi-0.9.1/src/ssapi/types.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)     1038 2023-06-10 16:26:54.000000 ssapi-0.9.1/src/ssapi/utils.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)     3657 2023-07-01 11:10:33.000000 ssapi-0.9.1/src/ssapi/web.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)     1478 2023-06-10 16:53:24.000000 ssapi-0.9.1/src/ssapi/web_decorators.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      766 2023-07-01 11:07:20.000000 ssapi-0.9.1/src/ssapi/web_tools.py
-drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-07-01 11:13:05.389990 ssapi-0.9.1/src/ssapi.egg-info/
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      143 2023-07-01 11:13:05.000000 ssapi-0.9.1/src/ssapi.egg-info/PKG-INFO
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      480 2023-07-01 11:13:05.000000 ssapi-0.9.1/src/ssapi.egg-info/SOURCES.txt
--rw-rw-r--   0 zedr      (1000) zedr      (1000)        1 2023-07-01 11:13:05.000000 ssapi-0.9.1/src/ssapi.egg-info/dependency_links.txt
--rw-rw-r--   0 zedr      (1000) zedr      (1000)       22 2023-07-01 11:13:05.000000 ssapi-0.9.1/src/ssapi.egg-info/requires.txt
--rw-rw-r--   0 zedr      (1000) zedr      (1000)        6 2023-07-01 11:13:05.000000 ssapi-0.9.1/src/ssapi.egg-info/top_level.txt
+drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-07-01 11:57:07.818235 ssapi-0.9.2/
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      143 2023-07-01 11:57:07.818235 ssapi-0.9.2/PKG-INFO
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)       30 2023-06-10 16:26:54.000000 ssapi-0.9.2/pyproject.toml
+drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-07-01 11:57:07.814234 ssapi-0.9.2/scripts/
+-rwxr-xr-x   0 zedr      (1000) zedr      (1000)      497 2023-04-30 10:24:27.000000 ssapi-0.9.2/scripts/ssapi-web
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)       38 2023-07-01 11:57:07.818235 ssapi-0.9.2/setup.cfg
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      272 2023-07-01 11:54:08.000000 ssapi-0.9.2/setup.py
+drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-07-01 11:57:07.814234 ssapi-0.9.2/src/
+drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-07-01 11:57:07.817234 ssapi-0.9.2/src/ssapi/
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)        0 2022-09-17 12:56:21.000000 ssapi-0.9.2/src/ssapi/__init__.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)     4566 2023-07-01 11:56:26.000000 ssapi-0.9.2/src/ssapi/db.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)     1983 2023-06-10 16:51:23.000000 ssapi-0.9.2/src/ssapi/db_utils.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      201 2023-06-10 16:26:54.000000 ssapi-0.9.2/src/ssapi/defaults.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      857 2023-07-01 11:54:40.000000 ssapi-0.9.2/src/ssapi/entities.py
+-rw-r--r--   0 zedr      (1000) zedr      (1000)      631 2023-04-30 11:11:55.000000 ssapi-0.9.2/src/ssapi/env.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      363 2023-06-10 16:26:54.000000 ssapi-0.9.2/src/ssapi/exceptions.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)     2397 2023-06-10 16:26:54.000000 ssapi-0.9.2/src/ssapi/relational.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      826 2023-06-10 16:26:54.000000 ssapi-0.9.2/src/ssapi/types.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)     1038 2023-06-10 16:26:54.000000 ssapi-0.9.2/src/ssapi/utils.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)     4200 2023-07-01 11:54:44.000000 ssapi-0.9.2/src/ssapi/web.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)     1478 2023-06-10 16:53:24.000000 ssapi-0.9.2/src/ssapi/web_decorators.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      766 2023-07-01 11:07:20.000000 ssapi-0.9.2/src/ssapi/web_tools.py
+drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-07-01 11:57:07.817234 ssapi-0.9.2/src/ssapi.egg-info/
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      143 2023-07-01 11:57:07.000000 ssapi-0.9.2/src/ssapi.egg-info/PKG-INFO
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      480 2023-07-01 11:57:07.000000 ssapi-0.9.2/src/ssapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)        1 2023-07-01 11:57:07.000000 ssapi-0.9.2/src/ssapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)       22 2023-07-01 11:57:07.000000 ssapi-0.9.2/src/ssapi.egg-info/requires.txt
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)        6 2023-07-01 11:57:07.000000 ssapi-0.9.2/src/ssapi.egg-info/top_level.txt
```

### Comparing `ssapi-0.9.1/src/ssapi/db.py` & `ssapi-0.9.2/src/ssapi/db.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import typing as T
 
 from ssapi.types import Undefined
 from ssapi.entities import Sale, Return, Transaction
 from ssapi.relational import Database
 from ssapi.db_utils import (
     create_date_where_clause,
@@ -120,20 +121,19 @@
         return self._get_transaction(Return, id)
 
     def get_products(self) -> T.Generator[tuple, None, None]:
         cur = self.conn.execute("SELECT DISTINCT product FROM sales")
         for item in cur.fetchall():
             yield item[0]
 
-    def put_settings(self, owner: str, string_data: str) -> None:
+    def put_settings(self, owner: str, data: dict) -> None:
         self.conn.execute(
-            "REPLACE INTO settings VALUES(?, ?)", (owner, string_data)
+            "REPLACE INTO settings VALUES(?, ?)", (owner, json.dumps(data))
         )
         self.conn.commit()
 
-    def get_settings(self, owner: str) -> str:
+    def get_settings(self, owner: str) -> T.Optional[dict]:
         cur = self.conn.execute(
             "SELECT data FROM settings WHERE owner=?", (owner,)
         )
         data = cur.fetchone()
-        if data is not None:
-            return data[0]
+        return None if data is None else json.loads(data[0])
```

### Comparing `ssapi-0.9.1/src/ssapi/db_utils.py` & `ssapi-0.9.2/src/ssapi/db_utils.py`

 * *Files identical despite different names*

### Comparing `ssapi-0.9.1/src/ssapi/entities.py` & `ssapi-0.9.2/src/ssapi/entities.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     date: Optional[str] = None
 
     class Constraints:
         product = constraint(len, 255, operator.lt)
         shop = constraint(len, 255, operator.lt)
 
     class Meta:
-        table_name: ""
+        table_name = ""
 
 
 @dataclass
 class Sale(Transaction):
     """A sale of a certain amount of product"""
 
     is_discounted: bool = False
```

### Comparing `ssapi-0.9.1/src/ssapi/env.py` & `ssapi-0.9.2/src/ssapi/env.py`

 * *Files identical despite different names*

### Comparing `ssapi-0.9.1/src/ssapi/relational.py` & `ssapi-0.9.2/src/ssapi/relational.py`

 * *Files identical despite different names*

### Comparing `ssapi-0.9.1/src/ssapi/types.py` & `ssapi-0.9.2/src/ssapi/types.py`

 * *Files identical despite different names*

### Comparing `ssapi-0.9.1/src/ssapi/utils.py` & `ssapi-0.9.2/src/ssapi/utils.py`

 * *Files identical despite different names*

### Comparing `ssapi-0.9.1/src/ssapi/web.py` & `ssapi-0.9.2/src/ssapi/web.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pkg_resources
 from ast import literal_eval
 
-from bottle import get, post, request, response, default_app, Bottle
+from bottle import get, post, put, request, response, default_app, Bottle
 
 from ssapi.entities import Sale, Return
 from ssapi.env import get_env_database
 from ssapi.types import Undefined
 from ssapi.web_tools import get_bottle_routes
 from ssapi.web_decorators import accepts_json, returns_json, handles_db_errors
 
@@ -17,18 +17,15 @@
 
 @get("/")
 @returns_json
 def get_root():
     app = get_application()
     routes = get_bottle_routes(app)
     pkg_version = pkg_resources.get_distribution("ssapi").version
-    return {
-        "version": pkg_version,
-        "resources": routes
-    }
+    return {"version": pkg_version, "resources": routes}
 
 
 @get("/shops")
 @returns_json
 def get_shops():
     return list(get_env_database().get_shops())
 
@@ -145,9 +142,32 @@
 
 @post("/drop")
 @returns_json
 def drop():
     # FIXME: add security
     db = get_env_database()
     db.drop()
-    db.open()
-    return {"outcome": f"Database dropped at: {db.name}"}
+    try:
+        return {"outcome": f"Database dropped at: {db.name}"}
+    finally:
+        db.open()
+
+
+@put("/settings/<owner_id>")
+@accepts_json
+@returns_json
+def put_settings(owner_id):
+    data = request.adapted_json
+    db = get_env_database()
+    db.put_settings(owner_id, data)
+    return {"outcome": f"Settings updated successfully at: {db.name}"}
+
+
+@get("/settings/<owner_id>")
+@returns_json
+def get_settings(owner_id):
+    data = get_env_database().get_settings(owner_id)
+    if data is None:
+        response.status = 404
+        return {"outcome": f"failed - owner '{owner_id}' not found"}
+    else:
+        return data
```

### Comparing `ssapi-0.9.1/src/ssapi/web_decorators.py` & `ssapi-0.9.2/src/ssapi/web_decorators.py`

 * *Files identical despite different names*

### Comparing `ssapi-0.9.1/src/ssapi/web_tools.py` & `ssapi-0.9.2/src/ssapi/web_tools.py`

 * *Files identical despite different names*

