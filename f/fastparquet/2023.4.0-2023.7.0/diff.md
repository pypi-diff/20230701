# Comparing `tmp/fastparquet-2023.4.0.tar.gz` & `tmp/fastparquet-2023.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastparquet-2023.4.0.tar", last modified: Sun May  7 17:06:15 2023, max compression
+gzip compressed data, was "fastparquet-2023.7.0.tar", last modified: Sat Jul  1 17:33:57 2023, max compression
```

## Comparing `fastparquet-2023.4.0.tar` & `fastparquet-2023.7.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 17:06:15.280585 fastparquet-2023.4.0/
--rw-r--r--   0 mdurant    (502) staff       (20)      258 2022-09-26 14:54:53.000000 fastparquet-2023.4.0/.coveragerc
--rw-r--r--   0 mdurant    (502) staff       (20)       37 2022-11-14 22:02:19.000000 fastparquet-2023.4.0/.gitattributes
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 17:06:15.262603 fastparquet-2023.4.0/.github/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 17:06:15.267285 fastparquet-2023.4.0/.github/workflows/
--rw-r--r--   0 mdurant    (502) staff       (20)     4092 2023-01-11 15:24:45.000000 fastparquet-2023.4.0/.github/workflows/main.yaml
--rw-r--r--   0 mdurant    (502) staff       (20)     2430 2022-12-05 18:49:50.000000 fastparquet-2023.4.0/.github/workflows/test_wheel.yaml
--rw-r--r--   0 mdurant    (502) staff       (20)     6754 2022-12-05 18:49:50.000000 fastparquet-2023.4.0/.github/workflows/wheel.yml
--rw-r--r--   0 mdurant    (502) staff       (20)      168 2022-11-18 01:33:09.000000 fastparquet-2023.4.0/.gitignore
--rw-r--r--   0 mdurant    (502) staff       (20)    12406 2022-09-26 14:54:53.000000 fastparquet-2023.4.0/.pylintrc
--rw-r--r--   0 mdurant    (502) staff       (20)    10173 2022-09-26 14:54:53.000000 fastparquet-2023.4.0/LICENSE
--rw-r--r--   0 mdurant    (502) staff       (20)      253 2022-09-26 14:54:53.000000 fastparquet-2023.4.0/MANIFEST.in
--rw-r--r--   0 mdurant    (502) staff       (20)      109 2022-09-26 14:54:53.000000 fastparquet-2023.4.0/Makefile
--rw-r--r--   0 mdurant    (502) staff       (20)     3911 2023-05-07 17:06:15.280709 fastparquet-2023.4.0/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)     3087 2022-09-26 14:54:53.000000 fastparquet-2023.4.0/README.rst
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 17:06:15.268528 fastparquet-2023.4.0/ci/
--rw-r--r--   0 mdurant    (502) staff       (20)      262 2022-11-30 21:37:32.000000 fastparquet-2023.4.0/ci/environment-py310.yml
--rw-r--r--   0 mdurant    (502) staff       (20)      230 2022-11-17 20:55:29.000000 fastparquet-2023.4.0/ci/environment-py38.yml
--rw-r--r--   0 mdurant    (502) staff       (20)      230 2022-11-17 20:55:29.000000 fastparquet-2023.4.0/ci/environment-py38win.yml
--rw-r--r--   0 mdurant    (502) staff       (20)      246 2022-11-17 20:55:29.000000 fastparquet-2023.4.0/ci/environment-py39.yml
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 17:06:15.278785 fastparquet-2023.4.0/fastparquet/
--rwxr-xr-x   0 mdurant    (502) staff       (20)      240 2022-11-14 22:02:19.000000 fastparquet-2023.4.0/fastparquet/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)      166 2023-05-07 17:06:12.000000 fastparquet-2023.4.0/fastparquet/_version.py
--rw-r--r--   0 mdurant    (502) staff       (20)    62966 2023-05-03 19:37:33.000000 fastparquet-2023.4.0/fastparquet/api.py
--rw-r--r--   0 mdurant    (502) staff       (20)  1620350 2023-04-20 17:18:50.000000 fastparquet-2023.4.0/fastparquet/cencoding.c
--rw-r--r--   0 mdurant    (502) staff       (20)    36443 2022-12-24 03:10:19.000000 fastparquet-2023.4.0/fastparquet/cencoding.pyx
--rw-r--r--   0 mdurant    (502) staff       (20)     3681 2022-09-26 14:54:53.000000 fastparquet-2023.4.0/fastparquet/compression.py
--rw-r--r--   0 mdurant    (502) staff       (20)     9724 2023-01-03 15:56:21.000000 fastparquet-2023.4.0/fastparquet/converted_types.py
--rw-r--r--   0 mdurant    (502) staff       (20)    29093 2023-04-20 20:00:50.000000 fastparquet-2023.4.0/fastparquet/core.py
--rw-r--r--   0 mdurant    (502) staff       (20)    10759 2023-04-20 20:00:50.000000 fastparquet-2023.4.0/fastparquet/dataframe.py
--rwxr-xr-x   0 mdurant    (502) staff       (20)     1540 2022-09-26 14:54:53.000000 fastparquet-2023.4.0/fastparquet/encoding.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3731 2022-09-26 14:54:53.000000 fastparquet-2023.4.0/fastparquet/json.py
--rw-r--r--   0 mdurant    (502) staff       (20)    34890 2022-09-26 14:54:53.000000 fastparquet-2023.4.0/fastparquet/parquet.thrift
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 17:06:15.279976 fastparquet-2023.4.0/fastparquet/parquet_thrift/
--rw-r--r--   0 mdurant    (502) staff       (20)      269 2022-09-26 14:54:53.000000 fastparquet-2023.4.0/fastparquet/parquet_thrift/__init__.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 17:06:15.280374 fastparquet-2023.4.0/fastparquet/parquet_thrift/parquet/
--rw-r--r--   0 mdurant    (502) staff       (20)       34 2022-09-26 14:54:53.000000 fastparquet-2023.4.0/fastparquet/parquet_thrift/parquet/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     5681 2022-09-26 14:54:53.000000 fastparquet-2023.4.0/fastparquet/parquet_thrift/parquet/ttypes.py
--rwxr-xr-x   0 mdurant    (502) staff       (20)     7063 2022-09-26 14:54:53.000000 fastparquet-2023.4.0/fastparquet/schema.py
--rw-r--r--   0 mdurant    (502) staff       (20)   897490 2023-04-20 17:18:51.000000 fastparquet-2023.4.0/fastparquet/speedups.c
--rw-r--r--   0 mdurant    (502) staff       (20)     3287 2022-09-26 14:54:53.000000 fastparquet-2023.4.0/fastparquet/speedups.pyx
--rw-r--r--   0 mdurant    (502) staff       (20)       65 2022-09-26 14:54:53.000000 fastparquet-2023.4.0/fastparquet/thrift_structures.py
--rw-r--r--   0 mdurant    (502) staff       (20)    17203 2023-04-20 20:00:50.000000 fastparquet-2023.4.0/fastparquet/util.py
--rw-r--r--   0 mdurant    (502) staff       (20)    70155 2023-04-20 20:00:50.000000 fastparquet-2023.4.0/fastparquet/writer.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 17:06:15.279797 fastparquet-2023.4.0/fastparquet.egg-info/
--rw-r--r--   0 mdurant    (502) staff       (20)     3911 2023-05-07 17:06:13.000000 fastparquet-2023.4.0/fastparquet.egg-info/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)     1085 2023-05-07 17:06:15.000000 fastparquet-2023.4.0/fastparquet.egg-info/SOURCES.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-05-07 17:06:13.000000 fastparquet-2023.4.0/fastparquet.egg-info/dependency_links.txt
--rw-r--r--   0 mdurant    (502) staff       (20)       76 2023-05-07 17:06:13.000000 fastparquet-2023.4.0/fastparquet.egg-info/requires.txt
--rw-r--r--   0 mdurant    (502) staff       (20)       12 2023-05-07 17:06:13.000000 fastparquet-2023.4.0/fastparquet.egg-info/top_level.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      114 2022-09-26 14:54:53.000000 fastparquet-2023.4.0/pyproject.toml
--rw-r--r--   0 mdurant    (502) staff       (20)      133 2022-12-02 16:22:06.000000 fastparquet-2023.4.0/readthedocs.yml
--rw-r--r--   0 mdurant    (502) staff       (20)       58 2022-10-31 17:25:30.000000 fastparquet-2023.4.0/requirements.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      236 2023-05-07 17:06:15.281063 fastparquet-2023.4.0/setup.cfg
--rw-r--r--   0 mdurant    (502) staff       (20)     3288 2022-11-18 01:33:09.000000 fastparquet-2023.4.0/setup.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-07-01 17:33:57.413389 fastparquet-2023.7.0/
+-rw-r--r--   0 mdurant    (502) staff       (20)      258 2022-09-26 14:54:53.000000 fastparquet-2023.7.0/.coveragerc
+-rw-r--r--   0 mdurant    (502) staff       (20)       37 2022-11-14 22:02:19.000000 fastparquet-2023.7.0/.gitattributes
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-07-01 17:33:57.395441 fastparquet-2023.7.0/.github/
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-07-01 17:33:57.399454 fastparquet-2023.7.0/.github/workflows/
+-rw-r--r--   0 mdurant    (502) staff       (20)     4057 2023-07-01 01:52:53.000000 fastparquet-2023.7.0/.github/workflows/main.yaml
+-rw-r--r--   0 mdurant    (502) staff       (20)     2430 2022-12-05 18:49:50.000000 fastparquet-2023.7.0/.github/workflows/test_wheel.yaml
+-rw-r--r--   0 mdurant    (502) staff       (20)     6754 2022-12-05 18:49:50.000000 fastparquet-2023.7.0/.github/workflows/wheel.yml
+-rw-r--r--   0 mdurant    (502) staff       (20)      168 2022-11-18 01:33:09.000000 fastparquet-2023.7.0/.gitignore
+-rw-r--r--   0 mdurant    (502) staff       (20)    12406 2022-09-26 14:54:53.000000 fastparquet-2023.7.0/.pylintrc
+-rw-r--r--   0 mdurant    (502) staff       (20)    10173 2022-09-26 14:54:53.000000 fastparquet-2023.7.0/LICENSE
+-rw-r--r--   0 mdurant    (502) staff       (20)      253 2022-09-26 14:54:53.000000 fastparquet-2023.7.0/MANIFEST.in
+-rw-r--r--   0 mdurant    (502) staff       (20)      109 2022-09-26 14:54:53.000000 fastparquet-2023.7.0/Makefile
+-rw-r--r--   0 mdurant    (502) staff       (20)     3911 2023-07-01 17:33:57.413529 fastparquet-2023.7.0/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)     3087 2022-09-26 14:54:53.000000 fastparquet-2023.7.0/README.rst
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-07-01 17:33:57.400404 fastparquet-2023.7.0/ci/
+-rw-r--r--   0 mdurant    (502) staff       (20)      291 2023-07-01 01:52:53.000000 fastparquet-2023.7.0/ci/environment-py310.yml
+-rw-r--r--   0 mdurant    (502) staff       (20)      242 2023-07-01 01:52:53.000000 fastparquet-2023.7.0/ci/environment-py38.yml
+-rw-r--r--   0 mdurant    (502) staff       (20)      242 2023-07-01 01:52:53.000000 fastparquet-2023.7.0/ci/environment-py38win.yml
+-rw-r--r--   0 mdurant    (502) staff       (20)      258 2023-07-01 01:52:53.000000 fastparquet-2023.7.0/ci/environment-py39.yml
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-07-01 17:33:57.410195 fastparquet-2023.7.0/fastparquet/
+-rwxr-xr-x   0 mdurant    (502) staff       (20)      240 2022-11-14 22:02:19.000000 fastparquet-2023.7.0/fastparquet/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      166 2023-07-01 17:33:54.000000 fastparquet-2023.7.0/fastparquet/_version.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    63033 2023-05-09 14:00:26.000000 fastparquet-2023.7.0/fastparquet/api.py
+-rw-r--r--   0 mdurant    (502) staff       (20)  1620350 2023-04-20 17:18:50.000000 fastparquet-2023.7.0/fastparquet/cencoding.c
+-rw-r--r--   0 mdurant    (502) staff       (20)    36443 2022-12-24 03:10:19.000000 fastparquet-2023.7.0/fastparquet/cencoding.pyx
+-rw-r--r--   0 mdurant    (502) staff       (20)     3681 2022-09-26 14:54:53.000000 fastparquet-2023.7.0/fastparquet/compression.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     9724 2023-01-03 15:56:21.000000 fastparquet-2023.7.0/fastparquet/converted_types.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    29093 2023-04-20 20:00:50.000000 fastparquet-2023.7.0/fastparquet/core.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    10759 2023-04-20 20:00:50.000000 fastparquet-2023.7.0/fastparquet/dataframe.py
+-rwxr-xr-x   0 mdurant    (502) staff       (20)     1540 2022-09-26 14:54:53.000000 fastparquet-2023.7.0/fastparquet/encoding.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3731 2022-09-26 14:54:53.000000 fastparquet-2023.7.0/fastparquet/json.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    34890 2022-09-26 14:54:53.000000 fastparquet-2023.7.0/fastparquet/parquet.thrift
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-07-01 17:33:57.412726 fastparquet-2023.7.0/fastparquet/parquet_thrift/
+-rw-r--r--   0 mdurant    (502) staff       (20)      269 2022-09-26 14:54:53.000000 fastparquet-2023.7.0/fastparquet/parquet_thrift/__init__.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-07-01 17:33:57.413170 fastparquet-2023.7.0/fastparquet/parquet_thrift/parquet/
+-rw-r--r--   0 mdurant    (502) staff       (20)       34 2022-09-26 14:54:53.000000 fastparquet-2023.7.0/fastparquet/parquet_thrift/parquet/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     5681 2022-09-26 14:54:53.000000 fastparquet-2023.7.0/fastparquet/parquet_thrift/parquet/ttypes.py
+-rwxr-xr-x   0 mdurant    (502) staff       (20)     7063 2022-09-26 14:54:53.000000 fastparquet-2023.7.0/fastparquet/schema.py
+-rw-r--r--   0 mdurant    (502) staff       (20)   897490 2023-04-20 17:18:51.000000 fastparquet-2023.7.0/fastparquet/speedups.c
+-rw-r--r--   0 mdurant    (502) staff       (20)     3287 2022-09-26 14:54:53.000000 fastparquet-2023.7.0/fastparquet/speedups.pyx
+-rw-r--r--   0 mdurant    (502) staff       (20)       65 2022-09-26 14:54:53.000000 fastparquet-2023.7.0/fastparquet/thrift_structures.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    17203 2023-04-20 20:00:50.000000 fastparquet-2023.7.0/fastparquet/util.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    70155 2023-05-11 19:50:15.000000 fastparquet-2023.7.0/fastparquet/writer.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-07-01 17:33:57.412577 fastparquet-2023.7.0/fastparquet.egg-info/
+-rw-r--r--   0 mdurant    (502) staff       (20)     3911 2023-07-01 17:33:54.000000 fastparquet-2023.7.0/fastparquet.egg-info/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)     1085 2023-07-01 17:33:57.000000 fastparquet-2023.7.0/fastparquet.egg-info/SOURCES.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-07-01 17:33:54.000000 fastparquet-2023.7.0/fastparquet.egg-info/dependency_links.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)       76 2023-07-01 17:33:54.000000 fastparquet-2023.7.0/fastparquet.egg-info/requires.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)       12 2023-07-01 17:33:54.000000 fastparquet-2023.7.0/fastparquet.egg-info/top_level.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      114 2022-09-26 14:54:53.000000 fastparquet-2023.7.0/pyproject.toml
+-rw-r--r--   0 mdurant    (502) staff       (20)      133 2022-12-02 16:22:06.000000 fastparquet-2023.7.0/readthedocs.yml
+-rw-r--r--   0 mdurant    (502) staff       (20)       58 2022-10-31 17:25:30.000000 fastparquet-2023.7.0/requirements.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      236 2023-07-01 17:33:57.413877 fastparquet-2023.7.0/setup.cfg
+-rw-r--r--   0 mdurant    (502) staff       (20)     3288 2022-11-18 01:33:09.000000 fastparquet-2023.7.0/setup.py
```

### Comparing `fastparquet-2023.4.0/.github/workflows/main.yaml` & `fastparquet-2023.7.0/.github/workflows/main.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         uses: actions/checkout@v2
         with:
           fetch-depth: 0
 
       - name: Setup conda
         uses: mamba-org/provision-with-micromamba@main
         with:
-          environment-file: ci/environment-py38.yml
+          environment-file: ci/environment-py39.yml
 
       - name: pip-install
         shell: bash -l {0}
         run: |
           git clone https://github.com/dask/dask
           pip install pyarrow
           pip install -e dask/
@@ -118,20 +118,20 @@
           environment-file: ci/environment-py310.yml
 
       - name: pip-install
         shell: bash -l {0}
         run: |
           pip install Cython
           pip install hypothesis
-          pip install pytest-xdist pytest-asyncio # Needed for a pandas test, also runs tests in parallel
+          pip install pytest-httpserver pytest-localserver pytest-xdist pytest-asyncio
           pip install -e . --no-deps # Install fastparquet
           git clone https://github.com/pandas-dev/pandas
           cd pandas
           python setup.py build_ext -j 4
-          pip install -e . --no-build-isolation --no-use-pep517
+          pip install -e . --no-build-isolation
 
       - name: Run Tests
         shell: bash -l {0}
         run: |
           pytest -v  fastparquet/ # fastparquet test suite against dev pandas
           pytest --verbose pandas/pandas/tests/io/test_parquet.py
           # Test parquet with different filesystems
```

### Comparing `fastparquet-2023.4.0/.github/workflows/test_wheel.yaml` & `fastparquet-2023.7.0/.github/workflows/test_wheel.yaml`

 * *Files identical despite different names*

### Comparing `fastparquet-2023.4.0/.github/workflows/wheel.yml` & `fastparquet-2023.7.0/.github/workflows/wheel.yml`

 * *Files identical despite different names*

### Comparing `fastparquet-2023.4.0/.pylintrc` & `fastparquet-2023.7.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `fastparquet-2023.4.0/LICENSE` & `fastparquet-2023.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastparquet-2023.4.0/PKG-INFO` & `fastparquet-2023.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastparquet
-Version: 2023.4.0
+Version: 2023.7.0
 Summary: Python support for Parquet file format
 Home-page: https://github.com/dask/fastparquet/
 Author: Martin Durant
 Author-email: mdurant@anaconda.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `fastparquet-2023.4.0/README.rst` & `fastparquet-2023.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `fastparquet-2023.4.0/fastparquet/api.py` & `fastparquet-2023.7.0/fastparquet/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,16 +314,17 @@
             new_rgs = [new_rgs]
         new_pf = object.__new__(ParquetFile)
         fmd = copy.copy(self.fmd)
         fmd.row_groups = new_rgs
         new_pf.__setstate__(
             {"fn": self.fn, "open": self.open, "fmd": fmd,
              "pandas_nulls": self.pandas_nulls, "_base_dtype": self._base_dtype,
-             "tz": self.tz}
+             "tz": self.tz, "_columns_dtype": self._columns_dtype}
         )
+        new_pf._set_attrs()
         return new_pf
 
     def __len__(self):
         """Return number of row groups."""
         if self.fmd.row_groups:
             return len(self.fmd.row_groups)
         else:
```

### Comparing `fastparquet-2023.4.0/fastparquet/cencoding.c` & `fastparquet-2023.7.0/fastparquet/cencoding.c`

 * *Files identical despite different names*

### Comparing `fastparquet-2023.4.0/fastparquet/cencoding.pyx` & `fastparquet-2023.7.0/fastparquet/cencoding.pyx`

 * *Files identical despite different names*

### Comparing `fastparquet-2023.4.0/fastparquet/compression.py` & `fastparquet-2023.7.0/fastparquet/compression.py`

 * *Files identical despite different names*

### Comparing `fastparquet-2023.4.0/fastparquet/converted_types.py` & `fastparquet-2023.7.0/fastparquet/converted_types.py`

 * *Files identical despite different names*

### Comparing `fastparquet-2023.4.0/fastparquet/core.py` & `fastparquet-2023.7.0/fastparquet/core.py`

 * *Files identical despite different names*

### Comparing `fastparquet-2023.4.0/fastparquet/dataframe.py` & `fastparquet-2023.7.0/fastparquet/dataframe.py`

 * *Files identical despite different names*

### Comparing `fastparquet-2023.4.0/fastparquet/encoding.py` & `fastparquet-2023.7.0/fastparquet/encoding.py`

 * *Files identical despite different names*

### Comparing `fastparquet-2023.4.0/fastparquet/json.py` & `fastparquet-2023.7.0/fastparquet/json.py`

 * *Files identical despite different names*

### Comparing `fastparquet-2023.4.0/fastparquet/parquet.thrift` & `fastparquet-2023.7.0/fastparquet/parquet.thrift`

 * *Files identical despite different names*

### Comparing `fastparquet-2023.4.0/fastparquet/parquet_thrift/parquet/ttypes.py` & `fastparquet-2023.7.0/fastparquet/parquet_thrift/parquet/ttypes.py`

 * *Files identical despite different names*

### Comparing `fastparquet-2023.4.0/fastparquet/schema.py` & `fastparquet-2023.7.0/fastparquet/schema.py`

 * *Files identical despite different names*

### Comparing `fastparquet-2023.4.0/fastparquet/speedups.c` & `fastparquet-2023.7.0/fastparquet/speedups.c`

 * *Files identical despite different names*

### Comparing `fastparquet-2023.4.0/fastparquet/speedups.pyx` & `fastparquet-2023.7.0/fastparquet/speedups.pyx`

 * *Files identical despite different names*

### Comparing `fastparquet-2023.4.0/fastparquet/util.py` & `fastparquet-2023.7.0/fastparquet/util.py`

 * *Files identical despite different names*

### Comparing `fastparquet-2023.4.0/fastparquet/writer.py` & `fastparquet-2023.7.0/fastparquet/writer.py`

 * *Files identical despite different names*

### Comparing `fastparquet-2023.4.0/fastparquet.egg-info/PKG-INFO` & `fastparquet-2023.7.0/fastparquet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastparquet
-Version: 2023.4.0
+Version: 2023.7.0
 Summary: Python support for Parquet file format
 Home-page: https://github.com/dask/fastparquet/
 Author: Martin Durant
 Author-email: mdurant@anaconda.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `fastparquet-2023.4.0/fastparquet.egg-info/SOURCES.txt` & `fastparquet-2023.7.0/fastparquet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastparquet-2023.4.0/setup.py` & `fastparquet-2023.7.0/setup.py`

 * *Files identical despite different names*

