# Comparing `tmp/beam_postgres_connector-0.1.0.tar.gz` & `tmp/beam_postgres_connector-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beam_postgres_connector-0.1.0.tar", max compression
+gzip compressed data, was "beam_postgres_connector-0.1.1.tar", max compression
```

## Comparing `beam_postgres_connector-0.1.0.tar` & `beam_postgres_connector-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1061 2023-04-11 02:59:31.754263 beam_postgres_connector-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2346 2023-04-11 04:34:04.873082 beam_postgres_connector-0.1.0/README.md
--rw-r--r--   0        0        0     2307 2023-04-11 04:37:18.993050 beam_postgres_connector-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0       22 2023-04-10 02:39:12.173441 beam_postgres_connector-0.1.0/src/beam_postgres/__init__.py
--rwxr-xr-x   0        0        0     5028 2023-04-11 02:27:42.784662 beam_postgres_connector-0.1.0/src/beam_postgres/client.py
--rwxr-xr-x   0        0        0      417 2023-04-10 09:57:56.818016 beam_postgres_connector-0.1.0/src/beam_postgres/errors.py
--rwxr-xr-x   0        0        0     4643 2023-04-11 02:27:42.744662 beam_postgres_connector-0.1.0/src/beam_postgres/io.py
--rwxr-xr-x   0        0        0     2717 2023-04-11 02:27:42.784662 beam_postgres_connector-0.1.0/src/beam_postgres/source.py
--rwxr-xr-x   0        0        0     4018 2023-04-10 10:15:56.339706 beam_postgres_connector-0.1.0/src/beam_postgres/splitters.py
--rwxr-xr-x   0        0        0      296 2023-04-10 09:58:49.818002 beam_postgres_connector-0.1.0/src/beam_postgres/utils.py
--rw-r--r--   0        0        0     3018 1970-01-01 00:00:00.000000 beam_postgres_connector-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-11 02:59:31.754263 beam_postgres_connector-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     2349 2023-05-19 11:06:08.366962 beam_postgres_connector-0.1.1/README.md
+-rw-r--r--   0        0        0     2583 2023-07-01 01:26:11.039834 beam_postgres_connector-0.1.1/pyproject.toml
+-rwxr-xr-x   0        0        0       22 2023-05-19 11:56:11.896780 beam_postgres_connector-0.1.1/src/beam_postgres/__init__.py
+-rwxr-xr-x   0        0        0     5025 2023-06-30 13:49:21.196890 beam_postgres_connector-0.1.1/src/beam_postgres/client.py
+-rwxr-xr-x   0        0        0      417 2023-04-10 09:57:56.818016 beam_postgres_connector-0.1.1/src/beam_postgres/errors.py
+-rwxr-xr-x   0        0        0     4616 2023-06-30 13:49:21.196890 beam_postgres_connector-0.1.1/src/beam_postgres/io.py
+-rwxr-xr-x   0        0        0     2717 2023-05-19 11:56:34.495107 beam_postgres_connector-0.1.1/src/beam_postgres/source.py
+-rwxr-xr-x   0        0        0     4018 2023-04-10 10:15:56.339706 beam_postgres_connector-0.1.1/src/beam_postgres/splitters.py
+-rwxr-xr-x   0        0        0      296 2023-04-10 09:58:49.818002 beam_postgres_connector-0.1.1/src/beam_postgres/utils.py
+-rw-r--r--   0        0        0     3221 1970-01-01 00:00:00.000000 beam_postgres_connector-0.1.1/PKG-INFO
```

### Comparing `beam_postgres_connector-0.1.0/LICENSE.txt` & `beam_postgres_connector-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `beam_postgres_connector-0.1.0/README.md` & `beam_postgres_connector-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     (
         p
         | "ReadFromPostgres" >> read_from_postgres
         | "WriteToStdout" >> beam.Map(print)
     )
 ```
 
-- Write To MySQL
+- Write To Postgres
 
 ```Python
 import apache_beam as beam
 from beam_postgres.io import WriteToPostgres
 
 
 with beam.Pipeline(options=options) as p:
```

### Comparing `beam_postgres_connector-0.1.0/pyproject.toml` & `beam_postgres_connector-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 [tool.poetry]
 name = "beam-postgres-connector"
-version = "0.1.0"
+version = "0.1.1"
 description = "An io connector for PostgreSQL read/write in Apache Beam pipelines."
 authors = ["satokiyo <satokiyo@loop8.biz>"]
 readme = "README.md"
-packages = [{include = "beam_postgres", from = "src"}]
+packages = [
+    {include = "beam_postgres", from = "src"},
+]
 license = "MIT"
 keywords = ["apache beam", "beam", "postgres", "postgresql"]
+homepage = "https://github.com/satokiyo/beam-postgres-connector"
+repository = "https://github.com/satokiyo/beam-postgres-connector"
 
 [tool.poetry.group.dev.dependencies]
 tox = "^4.4.11"
 black = "^23.3.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 mypy = "^1.2.0"
 pytest = "^7.3.0"
 types-psycopg2 = "^2.9.21.9"
 types-python-dateutil = "^2.8.19.12"
 pyproject-flake8 = "^6.0.0.post1"
+poetry = "^1.5.1"
+poetry-dynamic-versioning = "^0.24.0"
 
-
-[project.urls]
-Homepage = "https://github.com/satokiyo/beam-postgres-connector"
-
+[tool.poetry-dynamic-versioning]
+enable = false
+style = "pep440"
+format = "{base}"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 apache-beam = "^2.46.0"
 psycopg2-binary = "^2.9.6"
-
+poetry-dynamic-versioning = "^0.24.0"
 
 [build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.black]
 line-length = 88
 
 [tool.isort]
 profile = "black"
 line_length = 88
@@ -47,15 +52,14 @@
 
 [tool.flake8]
 max-line-length = 88
 max-complexity = 18
 ignore = "E203,E266,E402,E501,W503,"
 exclude = ["__pycache__", "__init__.py"]
 
-
 [tool.mypy]
 no_strict_optional = true
 show_error_context = false
 show_column_numbers = true
 ignore_missing_imports = true
 no_implicit_optional = true
 warn_return_any = true
@@ -74,15 +78,14 @@
     "__init__.py$",
 ]
 
 [[tool.mypy.overrides]]
 module = "apache_beam.*"
 ignore_missing_imports = true
 
-
 [tool.pytest.ini_options]
 minversion = "6.0"
 pythonpath = ["src"]
 #addopts = "-rsxX -l --tb=short --strict-markers -v --ff --pdb --setup-show"
 testpaths = [
     "tests/",
 ]
```

### Comparing `beam_postgres_connector-0.1.0/src/beam_postgres/client.py` & `beam_postgres_connector-0.1.1/src/beam_postgres/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,9 +156,9 @@
         conn = psycopg2.connect(**config)
         yield conn
 
     except PostgresConnectorError as e:
         raise PostgresConnectorError(
             f"Failed to connect postgres, Raise exception: {e}"
         )
-    finally:
+    else:
         conn.close()
```

### Comparing `beam_postgres_connector-0.1.0/src/beam_postgres/io.py` & `beam_postgres_connector-0.1.1/src/beam_postgres/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                 f"{'NULL' if value is None else value}"
                 if isinstance(value, (type(None), int, float))
                 else f"'{value}'"
                 for value in values
             ]
         )
 
-        query = f"INSERT INTO {self._config['database']}.{self._table}({column_str}) VALUES({value_str});"
+        query = f"INSERT INTO {self._table}({column_str}) VALUES({value_str});"
 
         self._queries.append(query)
 
         if len(self._queries) > self._batch_size:
             self._client.record_loader("\n".join(self._queries))
             self._queries.clear()
```

### Comparing `beam_postgres_connector-0.1.0/src/beam_postgres/source.py` & `beam_postgres_connector-0.1.1/src/beam_postgres/source.py`

 * *Files identical despite different names*

### Comparing `beam_postgres_connector-0.1.0/src/beam_postgres/splitters.py` & `beam_postgres_connector-0.1.1/src/beam_postgres/splitters.py`

 * *Files identical despite different names*

### Comparing `beam_postgres_connector-0.1.0/PKG-INFO` & `beam_postgres_connector-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: beam-postgres-connector
-Version: 0.1.0
+Version: 0.1.1
 Summary: An io connector for PostgreSQL read/write in Apache Beam pipelines.
+Home-page: https://github.com/satokiyo/beam-postgres-connector
 License: MIT
 Keywords: apache beam,beam,postgres,postgresql
 Author: satokiyo
 Author-email: satokiyo@loop8.biz
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: apache-beam (>=2.46.0,<3.0.0)
+Requires-Dist: poetry-dynamic-versioning (>=0.24.0,<0.25.0)
 Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
+Project-URL: Repository, https://github.com/satokiyo/beam-postgres-connector
 Description-Content-Type: text/markdown
 
 # Beam - Postgres connector
 
 [![PyPI](https://img.shields.io/pypi/v/beam-postgres-connector.svg)][pypi-project]
 [![Supported Versions](https://img.shields.io/pypi/pyversions/beam-postgres-connector.svg)][pypi-project]
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
@@ -54,15 +57,15 @@
     (
         p
         | "ReadFromPostgres" >> read_from_postgres
         | "WriteToStdout" >> beam.Map(print)
     )
 ```
 
-- Write To MySQL
+- Write To Postgres
 
 ```Python
 import apache_beam as beam
 from beam_postgres.io import WriteToPostgres
 
 
 with beam.Pipeline(options=options) as p:
```

