# Comparing `tmp/ssapi-0.4.2.tar.gz` & `tmp/ssapi-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssapi-0.4.2.tar", last modified: Sat Jun 10 16:57:17 2023, max compression
+gzip compressed data, was "ssapi-0.9.1.tar", last modified: Sat Jul  1 11:13:05 2023, max compression
```

## Comparing `ssapi-0.4.2.tar` & `ssapi-0.9.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-06-10 16:57:17.915816 ssapi-0.4.2/
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      143 2023-06-10 16:57:17.914816 ssapi-0.4.2/PKG-INFO
--rw-rw-r--   0 zedr      (1000) zedr      (1000)       30 2023-06-10 16:26:54.000000 ssapi-0.4.2/pyproject.toml
-drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-06-10 16:57:17.910816 ssapi-0.4.2/scripts/
--rwxr-xr-x   0 zedr      (1000) zedr      (1000)      497 2023-04-30 10:24:27.000000 ssapi-0.4.2/scripts/ssapi-web
--rw-rw-r--   0 zedr      (1000) zedr      (1000)       38 2023-06-10 16:57:17.915816 ssapi-0.4.2/setup.cfg
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      272 2023-06-10 16:57:02.000000 ssapi-0.4.2/setup.py
-drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-06-10 16:57:17.910816 ssapi-0.4.2/src/
-drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-06-10 16:57:17.913816 ssapi-0.4.2/src/ssapi/
--rw-rw-r--   0 zedr      (1000) zedr      (1000)        0 2022-09-17 12:56:21.000000 ssapi-0.4.2/src/ssapi/__init__.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)     3421 2023-06-10 16:51:23.000000 ssapi-0.4.2/src/ssapi/db.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)     1983 2023-06-10 16:51:23.000000 ssapi-0.4.2/src/ssapi/db_utils.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      201 2023-06-10 16:26:54.000000 ssapi-0.4.2/src/ssapi/defaults.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      722 2023-06-10 16:35:56.000000 ssapi-0.4.2/src/ssapi/entities.py
--rw-r--r--   0 zedr      (1000) zedr      (1000)      631 2023-04-30 11:11:55.000000 ssapi-0.4.2/src/ssapi/env.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      363 2023-06-10 16:26:54.000000 ssapi-0.4.2/src/ssapi/exceptions.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)     2397 2023-06-10 16:26:54.000000 ssapi-0.4.2/src/ssapi/relational.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      826 2023-06-10 16:26:54.000000 ssapi-0.4.2/src/ssapi/types.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)     1038 2023-06-10 16:26:54.000000 ssapi-0.4.2/src/ssapi/utils.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)     2353 2023-06-10 16:51:23.000000 ssapi-0.4.2/src/ssapi/web.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)     1478 2023-06-10 16:53:24.000000 ssapi-0.4.2/src/ssapi/web_decorators.py
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      809 2023-06-10 16:56:56.000000 ssapi-0.4.2/src/ssapi/web_tools.py
-drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-06-10 16:57:17.914816 ssapi-0.4.2/src/ssapi.egg-info/
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      143 2023-06-10 16:57:17.000000 ssapi-0.4.2/src/ssapi.egg-info/PKG-INFO
--rw-rw-r--   0 zedr      (1000) zedr      (1000)      480 2023-06-10 16:57:17.000000 ssapi-0.4.2/src/ssapi.egg-info/SOURCES.txt
--rw-rw-r--   0 zedr      (1000) zedr      (1000)        1 2023-06-10 16:57:17.000000 ssapi-0.4.2/src/ssapi.egg-info/dependency_links.txt
--rw-rw-r--   0 zedr      (1000) zedr      (1000)       22 2023-06-10 16:57:17.000000 ssapi-0.4.2/src/ssapi.egg-info/requires.txt
--rw-rw-r--   0 zedr      (1000) zedr      (1000)        6 2023-06-10 16:57:17.000000 ssapi-0.4.2/src/ssapi.egg-info/top_level.txt
+drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-07-01 11:13:05.389990 ssapi-0.9.1/
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      143 2023-07-01 11:13:05.389990 ssapi-0.9.1/PKG-INFO
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)       30 2023-06-10 16:26:54.000000 ssapi-0.9.1/pyproject.toml
+drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-07-01 11:13:05.386990 ssapi-0.9.1/scripts/
+-rwxr-xr-x   0 zedr      (1000) zedr      (1000)      497 2023-04-30 10:24:27.000000 ssapi-0.9.1/scripts/ssapi-web
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)       38 2023-07-01 11:13:05.390990 ssapi-0.9.1/setup.cfg
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      272 2023-07-01 11:11:01.000000 ssapi-0.9.1/setup.py
+drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-07-01 11:13:05.386990 ssapi-0.9.1/src/
+drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-07-01 11:13:05.388990 ssapi-0.9.1/src/ssapi/
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)        0 2022-09-17 12:56:21.000000 ssapi-0.9.1/src/ssapi/__init__.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)     4537 2023-07-01 11:07:20.000000 ssapi-0.9.1/src/ssapi/db.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)     1983 2023-06-10 16:51:23.000000 ssapi-0.9.1/src/ssapi/db_utils.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      201 2023-06-10 16:26:54.000000 ssapi-0.9.1/src/ssapi/defaults.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      856 2023-07-01 11:07:20.000000 ssapi-0.9.1/src/ssapi/entities.py
+-rw-r--r--   0 zedr      (1000) zedr      (1000)      631 2023-04-30 11:11:55.000000 ssapi-0.9.1/src/ssapi/env.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      363 2023-06-10 16:26:54.000000 ssapi-0.9.1/src/ssapi/exceptions.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)     2397 2023-06-10 16:26:54.000000 ssapi-0.9.1/src/ssapi/relational.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      826 2023-06-10 16:26:54.000000 ssapi-0.9.1/src/ssapi/types.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)     1038 2023-06-10 16:26:54.000000 ssapi-0.9.1/src/ssapi/utils.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)     3657 2023-07-01 11:10:33.000000 ssapi-0.9.1/src/ssapi/web.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)     1478 2023-06-10 16:53:24.000000 ssapi-0.9.1/src/ssapi/web_decorators.py
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      766 2023-07-01 11:07:20.000000 ssapi-0.9.1/src/ssapi/web_tools.py
+drwxrwxr-x   0 zedr      (1000) zedr      (1000)        0 2023-07-01 11:13:05.389990 ssapi-0.9.1/src/ssapi.egg-info/
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      143 2023-07-01 11:13:05.000000 ssapi-0.9.1/src/ssapi.egg-info/PKG-INFO
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)      480 2023-07-01 11:13:05.000000 ssapi-0.9.1/src/ssapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)        1 2023-07-01 11:13:05.000000 ssapi-0.9.1/src/ssapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)       22 2023-07-01 11:13:05.000000 ssapi-0.9.1/src/ssapi.egg-info/requires.txt
+-rw-rw-r--   0 zedr      (1000) zedr      (1000)        6 2023-07-01 11:13:05.000000 ssapi-0.9.1/src/ssapi.egg-info/top_level.txt
```

### Comparing `ssapi-0.4.2/src/ssapi/db.py` & `ssapi-0.9.1/src/ssapi/db.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,52 @@
 import typing as T
 
 from ssapi.types import Undefined
-from ssapi.entities import Sale, Return
+from ssapi.entities import Sale, Return, Transaction
 from ssapi.relational import Database
 from ssapi.db_utils import (
     create_date_where_clause,
     create_shop_where_clause,
     WhereClause,
 )
 
 
 class ShopDatabase(Database):
     """A database that stores data about shops"""
 
     def _tables_init(self) -> None:
         """Initialize the tables"""
         self.conn.execute(
-            "CREATE TABLE IF NOT EXISTS shops" "(" "name VARCHAR(255)" ")"
-        )
-        self.conn.execute(
             "CREATE TABLE IF NOT EXISTS sales"
             "("
             "id INTEGER PRIMARY KEY,"
-            "product VARCHAR(255), "
-            "shop VARCHAR(255), "
+            "product CHAR, "
+            "shop CHAR, "
             "quantity INT, "
             "date DATE DEFAULT CURRENT_TIMESTAMP, "
             "is_discounted BOOLEAN"
             ")"
         )
         self.conn.execute(
             "CREATE TABLE IF NOT EXISTS returns"
             "("
             "id INTEGER PRIMARY KEY,"
-            "product VARCHAR(255), "
-            "shop VARCHAR(255), "
+            "product CHAR, "
+            "shop CHAR, "
             "quantity INT, "
             "date DATE DEFAULT CURRENT_TIMESTAMP"
             ")"
         )
+        self.conn.execute(
+            "CREATE TABLE IF NOT EXISTS settings"
+            "("
+            "owner CHAR PRIMARY KEY,"
+            "data CHAR"
+            ")"
+        )
 
     def add_sales(self, *sales: Sale) -> int:
         """Record sale transactions and return the number of rows created"""
         cur = self.conn.executemany(
             "INSERT INTO sales VALUES(?, ?, ?, ?, ?, ?)",
             (sale.as_tuple() for sale in sales),
         )
@@ -77,27 +81,59 @@
         where = where.AND(WhereClause.create(is_discounted=is_discounted))
         cur = self.conn.execute(
             f"SELECT * FROM sales {where.clause}", where.values
         )
         for result in cur.fetchall():
             yield Sale(*result)
 
-    def get_sale(self, id: int) -> T.Optional[Sale]:
-        """Get a specific sale by its id"""
-        cur = self.conn.execute("SELECT * FROM sales WHERE id=?", (id,))
-        if result := cur.fetchone():
-            return Sale(*result)
-        else:
-            return None
-
     def get_returns(
-        self, date_start=None, date_end=None
+        self,
+        date_start="",
+        date_end="",
+        shop="",
     ) -> T.Generator[Return, None, None]:
         """Get the sales according to the given criteria"""
-        cur = self.conn.execute("SELECT * FROM returns")
+        where = create_date_where_clause(date_start, date_end)
+        where = where.AND(create_shop_where_clause(shop))
+        cur = self.conn.execute(
+            f"SELECT * FROM returns {where.clause}", where.values
+        )
         for result in cur.fetchall():
             yield Return(*result)
 
+    def _get_transaction(
+        self, transaction_type: T.Type[Transaction], id: int
+    ) -> T.Optional[Transaction]:
+        """Get a transaction by Id"""
+        stmt = f"SELECT * FROM {transaction_type.Meta.table_name} WHERE id=?"
+        cur = self.conn.execute(stmt, (id,))
+        if result := cur.fetchone():
+            return transaction_type(*result)
+        else:
+            return None
+
+    def get_sale(self, id: int) -> T.Optional[Sale]:
+        """Get a specific sale by its id"""
+        return self._get_transaction(Sale, id)
+
+    def get_return(self, id: int) -> T.Optional[Return]:
+        """Get a specific sale by its id"""
+        return self._get_transaction(Return, id)
+
     def get_products(self) -> T.Generator[tuple, None, None]:
         cur = self.conn.execute("SELECT DISTINCT product FROM sales")
         for item in cur.fetchall():
             yield item[0]
+
+    def put_settings(self, owner: str, string_data: str) -> None:
+        self.conn.execute(
+            "REPLACE INTO settings VALUES(?, ?)", (owner, string_data)
+        )
+        self.conn.commit()
+
+    def get_settings(self, owner: str) -> str:
+        cur = self.conn.execute(
+            "SELECT data FROM settings WHERE owner=?", (owner,)
+        )
+        data = cur.fetchone()
+        if data is not None:
+            return data[0]
```

### Comparing `ssapi-0.4.2/src/ssapi/db_utils.py` & `ssapi-0.9.1/src/ssapi/db_utils.py`

 * *Files identical despite different names*

### Comparing `ssapi-0.4.2/src/ssapi/env.py` & `ssapi-0.9.1/src/ssapi/env.py`

 * *Files identical despite different names*

### Comparing `ssapi-0.4.2/src/ssapi/relational.py` & `ssapi-0.9.1/src/ssapi/relational.py`

 * *Files identical despite different names*

### Comparing `ssapi-0.4.2/src/ssapi/types.py` & `ssapi-0.9.1/src/ssapi/types.py`

 * *Files identical despite different names*

### Comparing `ssapi-0.4.2/src/ssapi/utils.py` & `ssapi-0.9.1/src/ssapi/utils.py`

 * *Files identical despite different names*

### Comparing `ssapi-0.4.2/src/ssapi/web.py` & `ssapi-0.9.1/src/ssapi/web.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,34 @@
+import pkg_resources
+from ast import literal_eval
+
 from bottle import get, post, request, response, default_app, Bottle
 
-from ssapi.entities import Sale
+from ssapi.entities import Sale, Return
 from ssapi.env import get_env_database
 from ssapi.types import Undefined
 from ssapi.web_tools import get_bottle_routes
 from ssapi.web_decorators import accepts_json, returns_json, handles_db_errors
-from ast import literal_eval
 
 
 def get_application() -> Bottle:
     """Get the WSGI application"""
     return default_app()
 
 
 @get("/")
 @returns_json
 def get_root():
     app = get_application()
     routes = get_bottle_routes(app)
-    del routes["/"]
-    return routes
+    pkg_version = pkg_resources.get_distribution("ssapi").version
+    return {
+        "version": pkg_version,
+        "resources": routes
+    }
 
 
 @get("/shops")
 @returns_json
 def get_shops():
     return list(get_env_database().get_shops())
 
@@ -58,14 +63,40 @@
     if sale:
         return dict(sale.as_map())
     else:
         response.status = 404
         return {"outcome": f"not found: {request.path}"}
 
 
+@get("/returns")
+@returns_json
+def get_returns():
+    query = request.query.decode()
+    start = query.get("start", None)
+    end = query.get("end", None)
+    shop = query.get("shop", None)
+    return [
+        dict(sale.as_map())
+        for sale in get_env_database().get_returns(
+            date_start=start, date_end=end, shop=shop
+        )
+    ]
+
+
+@get("/returns/<id:int>")
+@returns_json
+def get_return(id: int) -> dict:
+    return_ = get_env_database().get_return(id)
+    if return_:
+        return dict(return_.as_map())
+    else:
+        response.status = 404
+        return {"outcome": f"not found: {request.path}"}
+
+
 @post("/sales")
 @accepts_json
 @returns_json
 @handles_db_errors
 def post_sales():
     try:
         new_sale = Sale(**request.adapted_json)
@@ -80,22 +111,43 @@
         db = get_env_database()
         count = db.add_sales(new_sale)
         outcome = f"creation ({count}) succeeded in database at: {db.name}"
 
     return {"outcome": outcome}
 
 
+@post("/returns")
+@accepts_json
+@returns_json
+@handles_db_errors
+def post_returns():
+    try:
+        new_return = Return(**request.adapted_json)
+    except TypeError as exc:
+        response.status = 400
+        outcome = (
+            f"creation failed: "
+            f"invalid parameters for type 'sale': "
+            f"{request.json} {exc}"
+        )
+    else:
+        db = get_env_database()
+        count = db.add_returns(new_return)
+        outcome = f"creation ({count}) succeeded in database at: {db.name}"
+
+    return {"outcome": outcome}
+
+
 @get("/products")
 @returns_json
 def get_products():
     return tuple(get_env_database().get_products())
 
 
 @post("/drop")
-@accepts_json
 @returns_json
 def drop():
     # FIXME: add security
     db = get_env_database()
     db.drop()
     db.open()
     return {"outcome": f"Database dropped at: {db.name}"}
```

### Comparing `ssapi-0.4.2/src/ssapi/web_decorators.py` & `ssapi-0.9.1/src/ssapi/web_decorators.py`

 * *Files identical despite different names*

### Comparing `ssapi-0.4.2/src/ssapi/web_tools.py` & `ssapi-0.9.1/src/ssapi/web_tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,14 @@
 
 camel_case_rxp = re.compile(r"^(?P<minor>[a-z]+)(?P<major>[A-Z]{1}\w*)$")
 
 
 def camel_to_snake_case(data: dict):
     """Convert camelCase to snake_case"""
     new_data = {}
-
-    if not data:
-        return new_data
-
     for key, val in data.items():
         if matched := camel_case_rxp.match(key):
             minor, major = matched.groups()
             new_data[f"{minor}_{major.lower()}"] = val
         else:
             new_data[key] = val
```

