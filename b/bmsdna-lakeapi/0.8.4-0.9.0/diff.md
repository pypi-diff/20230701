# Comparing `tmp/bmsdna_lakeapi-0.8.4.tar.gz` & `tmp/bmsdna_lakeapi-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_lakeapi-0.8.4.tar", max compression
+gzip compressed data, was "bmsdna_lakeapi-0.9.0.tar", max compression
```

## Comparing `bmsdna_lakeapi-0.8.4.tar` & `bmsdna_lakeapi-0.9.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1081 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/LICENSE
--rw-r--r--   0        0        0     8929 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/README.md
--rw-r--r--   0        0        0      337 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/api/__init__.py
--rw-r--r--   0        0        0     1138 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/api/api.py
--rw-r--r--   0        0        0      625 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/context/__init__.py
--rw-r--r--   0        0        0     7183 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/context/df_base.py
--rw-r--r--   0        0        0    10630 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/context/df_duckdb.py
--rw-r--r--   0        0        0     6255 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/context/df_polars.py
--rw-r--r--   0        0        0        0 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/__init__.py
--rw-r--r--   0        0        0    11269 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/config.py
--rw-r--r--   0        0        0    12557 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/dataframe.py
--rw-r--r--   0        0        0     7474 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/detail_endpoint.py
--rw-r--r--   0        0        0    10144 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/endpoint.py
--rw-r--r--   0        0        0      187 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/env.py
--rw-r--r--   0        0        0     1012 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/log.py
--rw-r--r--   0        0        0     6887 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/model.py
--rw-r--r--   0        0        0     1479 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/partition_utils.py
--rw-r--r--   0        0        0     6813 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/response.py
--rw-r--r--   0        0        0     4437 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/route.py
--rw-r--r--   0        0        0     3781 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/sql_endpoint.py
--rw-r--r--   0        0        0     3136 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/types.py
--rw-r--r--   0        0        0     2456 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/uservalidation.py
--rw-r--r--   0        0        0      215 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/yaml.py
--rw-r--r--   0        0        0        0 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/polars_extensions/__init__.py
--rw-r--r--   0        0        0     1837 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/polars_extensions/delta.py
--rw-r--r--   0        0        0      339 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/standalone/__init__.py
--rw-r--r--   0        0        0     1784 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/tools/useradd.py
--rw-r--r--   0        0        0     1084 2023-06-15 08:07:04.216868 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/tools/validateschema.py
--rw-r--r--   0        0        0     3535 2023-06-15 08:07:04.220869 bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/utils/fast_api_utils.py
--rw-r--r--   0        0        0     2017 2023-06-15 08:07:04.220869 bmsdna_lakeapi-0.8.4/pyproject.toml
--rw-r--r--   0        0        0    10127 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/LICENSE
+-rw-r--r--   0        0        0     9068 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/README.md
+-rw-r--r--   0        0        0      337 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/api/__init__.py
+-rw-r--r--   0        0        0     1138 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/api/api.py
+-rw-r--r--   0        0        0      625 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/context/__init__.py
+-rw-r--r--   0        0        0     7183 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/context/df_base.py
+-rw-r--r--   0        0        0    10630 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/context/df_duckdb.py
+-rw-r--r--   0        0        0     6255 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/context/df_polars.py
+-rw-r--r--   0        0        0        0 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/__init__.py
+-rw-r--r--   0        0        0    11269 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/config.py
+-rw-r--r--   0        0        0    12650 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/dataframe.py
+-rw-r--r--   0        0        0     7474 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/detail_endpoint.py
+-rw-r--r--   0        0        0    10144 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/endpoint.py
+-rw-r--r--   0        0        0      187 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/env.py
+-rw-r--r--   0        0        0     1012 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/log.py
+-rw-r--r--   0        0        0     6887 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/model.py
+-rw-r--r--   0        0        0     1479 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/partition_utils.py
+-rw-r--r--   0        0        0     6813 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/response.py
+-rw-r--r--   0        0        0     4437 2023-07-01 21:26:57.012231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/route.py
+-rw-r--r--   0        0        0     3781 2023-07-01 21:26:57.012231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/sql_endpoint.py
+-rw-r--r--   0        0        0     3136 2023-07-01 21:26:57.012231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/types.py
+-rw-r--r--   0        0        0     2456 2023-07-01 21:26:57.012231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/uservalidation.py
+-rw-r--r--   0        0        0      215 2023-07-01 21:26:57.012231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/yaml.py
+-rw-r--r--   0        0        0        0 2023-07-01 21:26:57.012231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/polars_extensions/__init__.py
+-rw-r--r--   0        0        0     1837 2023-07-01 21:26:57.012231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/polars_extensions/delta.py
+-rw-r--r--   0        0        0      339 2023-07-01 21:26:57.012231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/standalone/__init__.py
+-rw-r--r--   0        0        0     1784 2023-07-01 21:26:57.012231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/tools/useradd.py
+-rw-r--r--   0        0        0     1084 2023-07-01 21:26:57.012231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/tools/validateschema.py
+-rw-r--r--   0        0        0     3535 2023-07-01 21:26:57.012231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/utils/fast_api_utils.py
+-rw-r--r--   0        0        0     2017 2023-07-01 21:26:57.012231 bmsdna_lakeapi-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    10266 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.9.0/PKG-INFO
```

### Comparing `bmsdna_lakeapi-0.8.4/LICENSE` & `bmsdna_lakeapi-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.4/README.md` & `bmsdna_lakeapi-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -217,14 +217,18 @@
 - Built-in paging, you can use limit/offset to control what you get
 - Full-text search using DuckDB's full-text search feature
 - jsonify_complex parameter to convert structs/lists to json, the client cannot handle structs/lists
 - Metadata endpoints to retrieve data types, string lengths and more
 - Easily expose entire folders by using a "\*" wildcard in both the name and the datasource.uri config, see example in the config above
 - Good test coverage
 
+## Further projects
+
+- [lakeapi2sql](https://github.com/bmsuisse/lakeapi2sql) Allows you to read from lake api and write to MS SQL Server
+
 ## Work in progress
 
 Please note that this is a work in progress, changes will be made and things may break. Especially at this early stage.
 We recommend only using the export from `bmsdna.lakeapi` for now and not to use the submodules.
 
 ## Limitations
```

### Comparing `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/api/api.py` & `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/api/api.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/context/__init__.py` & `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/context/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/context/df_base.py` & `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/context/df_base.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/context/df_duckdb.py` & `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/context/df_duckdb.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/context/df_polars.py` & `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/context/df_polars.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/config.py` & `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/config.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/dataframe.py` & `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,21 +233,22 @@
     return cast(pypika.Criterion, expr)
 
 
 @cache
 async def _create_inner_expr(columns: Optional[List[str]], prmdef, e):
     inner_expr: Optional[pypika.Criterion] = None
     for ck, cv in e.items():
+        logger.info(f"key = {ck}, value = {cv}, columns = {columns}")
         if (columns and not ck in columns) and not ck in prmdef.combi:
             pass
         else:
             if inner_expr is None:
-                inner_expr = pypika.Field(ck) == cv if cv else pypika.Field(ck).isnull()
+                inner_expr = pypika.Field(ck) == cv if cv or cv == 0 else pypika.Field(ck).isnull()
             else:
-                inner_expr = inner_expr & (pypika.Field(ck) == cv if cv else pypika.Field(ck).isnull())
+                inner_expr = inner_expr & (pypika.Field(ck) == cv if cv or cv == 0 else pypika.Field(ck).isnull())
     return inner_expr
 
 
 @cache
 async def filter_df_based_on_params(
     params: dict[str, Any],
     param_def: list[Union[Param, str]],
```

### Comparing `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/detail_endpoint.py` & `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/detail_endpoint.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/endpoint.py` & `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/endpoint.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/log.py` & `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/log.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/model.py` & `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/model.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/partition_utils.py` & `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/partition_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/response.py` & `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/response.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/route.py` & `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/route.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/sql_endpoint.py` & `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/sql_endpoint.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/types.py` & `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/types.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/core/uservalidation.py` & `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/uservalidation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/polars_extensions/delta.py` & `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/polars_extensions/delta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/tools/useradd.py` & `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/tools/useradd.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/tools/validateschema.py` & `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/tools/validateschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.4/bmsdna/lakeapi/utils/fast_api_utils.py` & `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/utils/fast_api_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.4/pyproject.toml` & `bmsdna_lakeapi-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-lakeapi"
-version = "0.8.4"
+version = "0.9.0"
 description = ""
 authors = ["DWH Team <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmsdna"}]
 
 [tool.poetry.dependencies]
```

### Comparing `bmsdna_lakeapi-0.8.4/PKG-INFO` & `bmsdna_lakeapi-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-lakeapi
-Version: 0.8.4
+Version: 0.9.0
 Summary: 
 License: MIT
 Author: DWH Team
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -249,14 +249,18 @@
 - Built-in paging, you can use limit/offset to control what you get
 - Full-text search using DuckDB's full-text search feature
 - jsonify_complex parameter to convert structs/lists to json, the client cannot handle structs/lists
 - Metadata endpoints to retrieve data types, string lengths and more
 - Easily expose entire folders by using a "\*" wildcard in both the name and the datasource.uri config, see example in the config above
 - Good test coverage
 
+## Further projects
+
+- [lakeapi2sql](https://github.com/bmsuisse/lakeapi2sql) Allows you to read from lake api and write to MS SQL Server
+
 ## Work in progress
 
 Please note that this is a work in progress, changes will be made and things may break. Especially at this early stage.
 We recommend only using the export from `bmsdna.lakeapi` for now and not to use the submodules.
 
 ## Limitations
```

