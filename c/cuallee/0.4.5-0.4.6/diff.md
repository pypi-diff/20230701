# Comparing `tmp/cuallee-0.4.5.tar.gz` & `tmp/cuallee-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuallee-0.4.5.tar", last modified: Sat Jun 10 16:44:11 2023, max compression
+gzip compressed data, was "cuallee-0.4.6.tar", last modified: Sat Jul  1 10:40:30 2023, max compression
```

## Comparing `cuallee-0.4.5.tar` & `cuallee-0.4.6.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-06-10 16:44:11.188587 cuallee-0.4.5/
--rw-rw-r--   0 herminio  (1000) herminio  (1000)    11357 2022-09-20 23:24:07.000000 cuallee-0.4.5/LICENSE
--rw-r--r--   0 herminio  (1000) herminio  (1000)    15051 2023-06-10 16:44:11.188587 cuallee-0.4.5/PKG-INFO
--rw-r--r--   0 herminio  (1000) herminio  (1000)    14258 2023-06-03 15:46:05.000000 cuallee-0.4.5/README.md
-drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-06-10 16:44:11.188587 cuallee-0.4.5/cuallee/
--rw-r--r--   0 herminio  (1000) herminio  (1000)    20708 2023-06-10 16:39:56.000000 cuallee-0.4.5/cuallee/__init__.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)     9872 2023-06-10 16:39:56.000000 cuallee-0.4.5/cuallee/duckdb_validation.py
-drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-06-10 16:44:11.188587 cuallee-0.4.5/cuallee/iso/
--rw-r--r--   0 herminio  (1000) herminio  (1000)        0 2023-06-03 15:46:05.000000 cuallee-0.4.5/cuallee/iso/__init__.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)     2244 2023-06-03 15:46:05.000000 cuallee-0.4.5/cuallee/iso/checks.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)    12990 2023-06-03 15:46:05.000000 cuallee-0.4.5/cuallee/pandas_validation.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)    16162 2023-06-10 16:39:56.000000 cuallee-0.4.5/cuallee/polars_validation.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)    31138 2023-06-03 15:46:05.000000 cuallee-0.4.5/cuallee/pyspark_validation.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)    28442 2022-12-04 15:12:29.000000 cuallee-0.4.5/cuallee/snowpark_validation.py
--rw-rw-r--   0 herminio  (1000) herminio  (1000)     2043 2022-10-23 12:45:17.000000 cuallee-0.4.5/cuallee/utils.py
-drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-06-10 16:44:11.188587 cuallee-0.4.5/cuallee.egg-info/
--rw-r--r--   0 herminio  (1000) herminio  (1000)    15051 2023-06-10 16:44:11.000000 cuallee-0.4.5/cuallee.egg-info/PKG-INFO
--rw-r--r--   0 herminio  (1000) herminio  (1000)      427 2023-06-10 16:44:11.000000 cuallee-0.4.5/cuallee.egg-info/SOURCES.txt
--rw-r--r--   0 herminio  (1000) herminio  (1000)        1 2023-06-10 16:44:11.000000 cuallee-0.4.5/cuallee.egg-info/dependency_links.txt
--rw-r--r--   0 herminio  (1000) herminio  (1000)      311 2023-06-10 16:44:11.000000 cuallee-0.4.5/cuallee.egg-info/requires.txt
--rw-r--r--   0 herminio  (1000) herminio  (1000)        8 2023-06-10 16:44:11.000000 cuallee-0.4.5/cuallee.egg-info/top_level.txt
--rw-r--r--   0 herminio  (1000) herminio  (1000)     1210 2023-06-10 16:41:33.000000 cuallee-0.4.5/pyproject.toml
--rw-r--r--   0 herminio  (1000) herminio  (1000)      109 2023-06-10 16:44:11.188587 cuallee-0.4.5/setup.cfg
+drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-07-01 10:40:30.540022 cuallee-0.4.6/
+-rw-rw-r--   0 herminio  (1000) herminio  (1000)    11357 2022-09-20 23:24:07.000000 cuallee-0.4.6/LICENSE
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    15261 2023-07-01 10:40:30.540022 cuallee-0.4.6/PKG-INFO
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    14443 2023-06-10 17:01:42.000000 cuallee-0.4.6/README.md
+drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-07-01 10:40:30.540022 cuallee-0.4.6/cuallee/
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    21186 2023-06-11 06:57:11.000000 cuallee-0.4.6/cuallee/__init__.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)     5154 2023-06-11 06:57:11.000000 cuallee-0.4.6/cuallee/bigquery_validation.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)     9872 2023-06-10 16:39:56.000000 cuallee-0.4.6/cuallee/duckdb_validation.py
+drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-07-01 10:40:30.540022 cuallee-0.4.6/cuallee/iso/
+-rw-r--r--   0 herminio  (1000) herminio  (1000)        0 2023-06-03 15:46:05.000000 cuallee-0.4.6/cuallee/iso/__init__.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)     2244 2023-06-03 15:46:05.000000 cuallee-0.4.6/cuallee/iso/checks.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    12990 2023-06-03 15:46:05.000000 cuallee-0.4.6/cuallee/pandas_validation.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    16162 2023-06-10 16:39:56.000000 cuallee-0.4.6/cuallee/polars_validation.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    31131 2023-07-01 10:40:06.000000 cuallee-0.4.6/cuallee/pyspark_validation.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    28442 2022-12-04 15:12:29.000000 cuallee-0.4.6/cuallee/snowpark_validation.py
+-rw-rw-r--   0 herminio  (1000) herminio  (1000)     2043 2022-10-23 12:45:17.000000 cuallee-0.4.6/cuallee/utils.py
+drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-07-01 10:40:30.540022 cuallee-0.4.6/cuallee.egg-info/
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    15261 2023-07-01 10:40:30.000000 cuallee-0.4.6/cuallee.egg-info/PKG-INFO
+-rw-r--r--   0 herminio  (1000) herminio  (1000)      458 2023-07-01 10:40:30.000000 cuallee-0.4.6/cuallee.egg-info/SOURCES.txt
+-rw-r--r--   0 herminio  (1000) herminio  (1000)        1 2023-07-01 10:40:30.000000 cuallee-0.4.6/cuallee.egg-info/dependency_links.txt
+-rw-r--r--   0 herminio  (1000) herminio  (1000)      369 2023-07-01 10:40:30.000000 cuallee-0.4.6/cuallee.egg-info/requires.txt
+-rw-r--r--   0 herminio  (1000) herminio  (1000)        8 2023-07-01 10:40:30.000000 cuallee-0.4.6/cuallee.egg-info/top_level.txt
+-rw-r--r--   0 herminio  (1000) herminio  (1000)     1281 2023-07-01 10:40:06.000000 cuallee-0.4.6/pyproject.toml
+-rw-r--r--   0 herminio  (1000) herminio  (1000)      109 2023-07-01 10:40:30.540022 cuallee-0.4.6/setup.cfg
```

### Comparing `cuallee-0.4.5/LICENSE` & `cuallee-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.5/PKG-INFO` & `cuallee-0.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: cuallee
-Version: 0.4.5
+Version: 0.4.6
 Summary: Python library for data validation on DataFrame APIs including Snowflake/Snowpark, Apache/PySpark and Pandas/DataFrame.
 Author-email: Virginie Grosboillot <vestalisvirginis@gmail.com>, Herminio Vazquez <canimus@gmail.com>
 Project-URL: Homepage, https://github.com/canimus/cuallee
 Project-URL: Bug Tracker, https://github.com/canimus/cuallee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: pyspark
 Provides-Extra: snowpark
 Provides-Extra: pandas
+Provides-Extra: bigquery
 Provides-Extra: duckdb
 Provides-Extra: polars
 Provides-Extra: iso
 Provides-Extra: test
 License-File: LICENSE
 
 # cuallee
@@ -39,16 +40,16 @@
 
 Provider | API | Versions
  ------- | ----------- | ------
 ![snowflake](logos/snowflake.svg?raw=true "Snowpark DataFrame API")| `snowpark` | `1.4.0`
 ![databricks](logos/databricks.svg?raw=true "PySpark DataFrame API")| `pyspark` | `3.4.0`, `3.3.x`, `3.2.x`
 ![bigquery](logos/bigquery.png?raw=true "BigQuery Client API")| `bigquery` | `3.4.1`
 ![pandas](logos/pandas.svg?raw=true "Pandas DataFrame API")| `pandas`| `2.0.1`, `1.5.x`, `1.4.x`
-![duckdb](logos/duckdb.png?raw=true "DuckDB API")|`duckdb` | `0.7.1`
-![polars](logos/polars.svg?raw=true "Polars API")|`polars`|`0.15.x (wip)` 
+![duckdb](logos/duckdb.png?raw=true "DuckDB API")|`duckdb` | `0.7.1`, `0.8.0`
+![polars](logos/polars.svg?raw=true "Polars API")|`polars`|`0.18.2` 
  
  <sub>Logos are trademarks of their own brands.</sub>
 
 ## Stats
 [![PyPI version](https://badge.fury.io/py/cuallee.svg)](https://badge.fury.io/py/cuallee)
 [![ci](https://github.com/canimus/cuallee/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/canimus/cuallee/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/canimus/cuallee/branch/main/graph/badge.svg?token=D7SOV620MS)](https://codecov.io/gh/canimus/cuallee)
@@ -283,21 +284,28 @@
 1   2  2022-10-31 23:15:06  test  WARNING  tpep_pickup_datetime  is_complete   N/A  19817583         0.0        1.0             1.0   PASS
 ```
 
 ## Roadmap
 
 `100%` data frame agnostic implementation of data quality checks.
 Define once, `run everywhere`
-- [x] PySpark 3.3.0
-- [x] PySpark 3.2.x 
-- [x] Snowpark DataFrame
-- [x] Pandas DataFrame
-- [x] DuckDB Tables
-- [x] BigQuery Client
-- Polars DataFrame
+- ~~[x] PySpark 3.4.0~~
+- ~~[x] PySpark 3.3.0~~
+- ~~[x] PySpark 3.2.x~~
+- ~~[x] Snowpark DataFrame~~
+- ~~[x] Pandas DataFrame~~
+- ~~[x] DuckDB Tables~~
+- ~~[x] BigQuery Client~~
+- ~~[x] Polars DataFrame~~
+- [ ] Metadata check
+- [ ] OpenMetadata Integration
+- [ ] Dagster Integration
+- [ ] PDF Report
+- [ ] Help us in a discussion?
+
 
 
 Whilst expanding the functionality feels a bit as an overkill because you most likely can connect `spark` via its drivers to whatever `DBMS` of your choice.
 In the desire to make it even more `user-friendly` we are aiming to make `cuallee` portable to all the providers above.
 
 ## Authors
 - [canimus](https://github.com/canimus) / Herminio Vazquez / 🇲🇽
```

### Comparing `cuallee-0.4.5/README.md` & `cuallee-0.4.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 Provider | API | Versions
  ------- | ----------- | ------
 ![snowflake](logos/snowflake.svg?raw=true "Snowpark DataFrame API")| `snowpark` | `1.4.0`
 ![databricks](logos/databricks.svg?raw=true "PySpark DataFrame API")| `pyspark` | `3.4.0`, `3.3.x`, `3.2.x`
 ![bigquery](logos/bigquery.png?raw=true "BigQuery Client API")| `bigquery` | `3.4.1`
 ![pandas](logos/pandas.svg?raw=true "Pandas DataFrame API")| `pandas`| `2.0.1`, `1.5.x`, `1.4.x`
-![duckdb](logos/duckdb.png?raw=true "DuckDB API")|`duckdb` | `0.7.1`
-![polars](logos/polars.svg?raw=true "Polars API")|`polars`|`0.15.x (wip)` 
+![duckdb](logos/duckdb.png?raw=true "DuckDB API")|`duckdb` | `0.7.1`, `0.8.0`
+![polars](logos/polars.svg?raw=true "Polars API")|`polars`|`0.18.2` 
  
  <sub>Logos are trademarks of their own brands.</sub>
 
 ## Stats
 [![PyPI version](https://badge.fury.io/py/cuallee.svg)](https://badge.fury.io/py/cuallee)
 [![ci](https://github.com/canimus/cuallee/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/canimus/cuallee/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/canimus/cuallee/branch/main/graph/badge.svg?token=D7SOV620MS)](https://codecov.io/gh/canimus/cuallee)
@@ -262,21 +262,28 @@
 1   2  2022-10-31 23:15:06  test  WARNING  tpep_pickup_datetime  is_complete   N/A  19817583         0.0        1.0             1.0   PASS
 ```
 
 ## Roadmap
 
 `100%` data frame agnostic implementation of data quality checks.
 Define once, `run everywhere`
-- [x] PySpark 3.3.0
-- [x] PySpark 3.2.x 
-- [x] Snowpark DataFrame
-- [x] Pandas DataFrame
-- [x] DuckDB Tables
-- [x] BigQuery Client
-- Polars DataFrame
+- ~~[x] PySpark 3.4.0~~
+- ~~[x] PySpark 3.3.0~~
+- ~~[x] PySpark 3.2.x~~
+- ~~[x] Snowpark DataFrame~~
+- ~~[x] Pandas DataFrame~~
+- ~~[x] DuckDB Tables~~
+- ~~[x] BigQuery Client~~
+- ~~[x] Polars DataFrame~~
+- [ ] Metadata check
+- [ ] OpenMetadata Integration
+- [ ] Dagster Integration
+- [ ] PDF Report
+- [ ] Help us in a discussion?
+
 
 
 Whilst expanding the functionality feels a bit as an overkill because you most likely can connect `spark` via its drivers to whatever `DBMS` of your choice.
 In the desire to make it even more `user-friendly` we are aiming to make `cuallee` portable to all the providers above.
 
 ## Authors
 - [canimus](https://github.com/canimus) / Herminio Vazquez / 🇲🇽
```

### Comparing `cuallee-0.4.5/cuallee/__init__.py` & `cuallee-0.4.6/cuallee/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,21 @@
 try:
     from duckdb import DuckDBPyConnection as duckdb_dataframe  # type: ignore
 
     logger.debug(Fore.GREEN + "[OK]" + Fore.WHITE + " DuckDB")
 except:
     logger.debug(Fore.RED + "[KO]" + Fore.WHITE + " DuckDB")
 
+try:
+    from google.cloud import bigquery
+
+    logger.debug(Fore.GREEN + "[OK]" + Fore.WHITE + " BigQuery")
+except:
+    logger.debug(Fore.RED + "[KO]" + Fore.WHITE + " BigQuery")
+
 
 logger.debug(Style.RESET_ALL)
 
 logger = logging.getLogger(__name__)
 
 
 class CheckLevel(enum.Enum):
@@ -549,24 +556,29 @@
 
         # When dataframe is Pandas DataFrame API
         elif "pandas_dataframe" in globals() and isinstance(
             dataframe, pandas_dataframe
         ):
             self.compute_engine = importlib.import_module("cuallee.pandas_validation")
 
+        # When dataframe is Snowpark DataFrame API
         elif "snowpark_dataframe" in globals() and isinstance(
             dataframe, snowpark_dataframe
         ):
             self.compute_engine = importlib.import_module("cuallee.snowpark_validation")
 
         elif "duckdb_dataframe" in globals() and isinstance(
             dataframe, duckdb_dataframe
         ):
             self.compute_engine = importlib.import_module("cuallee.duckdb_validation")
 
+        # TODO: BigQuery source (pandas DataFrame/ json / file / uri)
+        elif "bigquery" in globals() and isinstance(dataframe, bigquery.table.Table):
+            self.compute_engine = importlib.import_module("cuallee.bigquery_validation")
+
         elif "polars_dataframe" in globals() and isinstance(
             dataframe, polars_dataframe
         ):
             self.compute_engine = importlib.import_module("cuallee.polars_validation")
 
         assert self.compute_engine.validate_data_types(
             self.rules, dataframe
```

### Comparing `cuallee-0.4.5/cuallee/duckdb_validation.py` & `cuallee-0.4.6/cuallee/duckdb_validation.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.5/cuallee/iso/checks.py` & `cuallee-0.4.6/cuallee/iso/checks.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.5/cuallee/pandas_validation.py` & `cuallee-0.4.6/cuallee/pandas_validation.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.5/cuallee/polars_validation.py` & `cuallee-0.4.6/cuallee/polars_validation.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.5/cuallee/pyspark_validation.py` & `cuallee-0.4.6/cuallee/pyspark_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         return self.compute_instruction
 
     def is_unique(self, rule: Rule):
         """Validation for unique values in column"""
         predicate = None  # F.count_distinct(F.col(rule.column))
         self.compute_instruction = ComputeInstruction(
             predicate,
-            F.approx_count_distinct(F.col(f"`{rule.column}`")),
+            F.count_distinct(F.col(f"`{rule.column}`")),
             ComputeMethod.SELECT,
         )
         return self.compute_instruction
 
     def are_unique(self, rule: Rule):
         """Validation for unique values in a group of columns"""
         predicate = None  # TODO:  .groupBy("value").count.filter("count > 1")
```

### Comparing `cuallee-0.4.5/cuallee/snowpark_validation.py` & `cuallee-0.4.6/cuallee/snowpark_validation.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.5/cuallee/utils.py` & `cuallee-0.4.6/cuallee/utils.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.5/cuallee.egg-info/PKG-INFO` & `cuallee-0.4.6/cuallee.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: cuallee
-Version: 0.4.5
+Version: 0.4.6
 Summary: Python library for data validation on DataFrame APIs including Snowflake/Snowpark, Apache/PySpark and Pandas/DataFrame.
 Author-email: Virginie Grosboillot <vestalisvirginis@gmail.com>, Herminio Vazquez <canimus@gmail.com>
 Project-URL: Homepage, https://github.com/canimus/cuallee
 Project-URL: Bug Tracker, https://github.com/canimus/cuallee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: pyspark
 Provides-Extra: snowpark
 Provides-Extra: pandas
+Provides-Extra: bigquery
 Provides-Extra: duckdb
 Provides-Extra: polars
 Provides-Extra: iso
 Provides-Extra: test
 License-File: LICENSE
 
 # cuallee
@@ -39,16 +40,16 @@
 
 Provider | API | Versions
  ------- | ----------- | ------
 ![snowflake](logos/snowflake.svg?raw=true "Snowpark DataFrame API")| `snowpark` | `1.4.0`
 ![databricks](logos/databricks.svg?raw=true "PySpark DataFrame API")| `pyspark` | `3.4.0`, `3.3.x`, `3.2.x`
 ![bigquery](logos/bigquery.png?raw=true "BigQuery Client API")| `bigquery` | `3.4.1`
 ![pandas](logos/pandas.svg?raw=true "Pandas DataFrame API")| `pandas`| `2.0.1`, `1.5.x`, `1.4.x`
-![duckdb](logos/duckdb.png?raw=true "DuckDB API")|`duckdb` | `0.7.1`
-![polars](logos/polars.svg?raw=true "Polars API")|`polars`|`0.15.x (wip)` 
+![duckdb](logos/duckdb.png?raw=true "DuckDB API")|`duckdb` | `0.7.1`, `0.8.0`
+![polars](logos/polars.svg?raw=true "Polars API")|`polars`|`0.18.2` 
  
  <sub>Logos are trademarks of their own brands.</sub>
 
 ## Stats
 [![PyPI version](https://badge.fury.io/py/cuallee.svg)](https://badge.fury.io/py/cuallee)
 [![ci](https://github.com/canimus/cuallee/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/canimus/cuallee/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/canimus/cuallee/branch/main/graph/badge.svg?token=D7SOV620MS)](https://codecov.io/gh/canimus/cuallee)
@@ -283,21 +284,28 @@
 1   2  2022-10-31 23:15:06  test  WARNING  tpep_pickup_datetime  is_complete   N/A  19817583         0.0        1.0             1.0   PASS
 ```
 
 ## Roadmap
 
 `100%` data frame agnostic implementation of data quality checks.
 Define once, `run everywhere`
-- [x] PySpark 3.3.0
-- [x] PySpark 3.2.x 
-- [x] Snowpark DataFrame
-- [x] Pandas DataFrame
-- [x] DuckDB Tables
-- [x] BigQuery Client
-- Polars DataFrame
+- ~~[x] PySpark 3.4.0~~
+- ~~[x] PySpark 3.3.0~~
+- ~~[x] PySpark 3.2.x~~
+- ~~[x] Snowpark DataFrame~~
+- ~~[x] Pandas DataFrame~~
+- ~~[x] DuckDB Tables~~
+- ~~[x] BigQuery Client~~
+- ~~[x] Polars DataFrame~~
+- [ ] Metadata check
+- [ ] OpenMetadata Integration
+- [ ] Dagster Integration
+- [ ] PDF Report
+- [ ] Help us in a discussion?
+
 
 
 Whilst expanding the functionality feels a bit as an overkill because you most likely can connect `spark` via its drivers to whatever `DBMS` of your choice.
 In the desire to make it even more `user-friendly` we are aiming to make `cuallee` portable to all the providers above.
 
 ## Authors
 - [canimus](https://github.com/canimus) / Herminio Vazquez / 🇲🇽
```

### Comparing `cuallee-0.4.5/pyproject.toml` & `cuallee-0.4.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cuallee"
-version = "0.4.5"
+version = "0.4.6"
 authors = [
   { name="Virginie Grosboillot", email="vestalisvirginis@gmail.com" },
   { name="Herminio Vazquez", email="canimus@gmail.com"}
 ]
 description = "Python library for data validation on DataFrame APIs including Snowflake/Snowpark, Apache/PySpark and Pandas/DataFrame."
 readme = "README.md"
 requires-python = ">=3.8"
@@ -33,14 +33,18 @@
 snowpark = [
   "snowflake-snowpark-python>=1.4.0",
   "pyarrow >= 10.0.1"
 ]
 pandas = [
   "pandas>=2.0.1"
 ]
+bigquery =[
+  "google-cloud-bigquery>=3.10.0",
+  "pyarrow >= 11.0.0"
+]
 duckdb = [
   "duckdb>=0.7.1"
 ]
 polars = [
   "polars>=0.15.7"
 ]
 iso = [
```

