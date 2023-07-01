# Comparing `tmp/AlgBench-1.1.0.tar.gz` & `tmp/AlgBench-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlgBench-1.1.0.tar", last modified: Fri May 26 12:05:04 2023, max compression
+gzip compressed data, was "AlgBench-2.0.0.tar", last modified: Sat Jul  1 20:12:30 2023, max compression
```

## Comparing `AlgBench-1.1.0.tar` & `AlgBench-2.0.0.tar`

### file list

```diff
@@ -1,31 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:05:04.899719 AlgBench-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 12:04:54.000000 AlgBench-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22381 2023-05-26 12:05:04.899719 AlgBench-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22003 2023-05-26 12:04:54.000000 AlgBench-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-26 12:04:55.000000 AlgBench-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 12:05:04.899719 AlgBench-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:05:04.895719 AlgBench-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:05:04.899719 AlgBench-1.1.0/src/AlgBench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22381 2023-05-26 12:05:04.000000 AlgBench-1.1.0/src/AlgBench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-26 12:05:04.000000 AlgBench-1.1.0/src/AlgBench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:05:04.000000 AlgBench-1.1.0/src/AlgBench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-26 12:05:04.000000 AlgBench-1.1.0/src/AlgBench.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-26 12:05:04.000000 AlgBench-1.1.0/src/AlgBench.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:05:04.899719 AlgBench-1.1.0/src/algbench/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-26 12:04:55.000000 AlgBench-1.1.0/src/algbench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-05-26 12:04:55.000000 AlgBench-1.1.0/src/algbench/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-26 12:04:55.000000 AlgBench-1.1.0/src/algbench/benchmark_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:05:04.899719 AlgBench-1.1.0/src/algbench/db/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-26 12:04:55.000000 AlgBench-1.1.0/src/algbench/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-26 12:04:55.000000 AlgBench-1.1.0/src/algbench/db/json_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-26 12:04:55.000000 AlgBench-1.1.0/src/algbench/db/nfs_json_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-05-26 12:04:55.000000 AlgBench-1.1.0/src/algbench/db/nfs_json_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-26 12:04:55.000000 AlgBench-1.1.0/src/algbench/db/nfs_json_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-26 12:04:55.000000 AlgBench-1.1.0/src/algbench/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-26 12:04:55.000000 AlgBench-1.1.0/src/algbench/fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-26 12:04:55.000000 AlgBench-1.1.0/src/algbench/pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:05:04.899719 AlgBench-1.1.0/src/algbench/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-26 12:04:55.000000 AlgBench-1.1.0/src/algbench/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-26 12:04:55.000000 AlgBench-1.1.0/src/algbench/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:05:04.899719 AlgBench-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-26 12:04:55.000000 AlgBench-1.1.0/tests/test_basics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:12:30.590146 AlgBench-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-01 20:12:18.000000 AlgBench-2.0.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:12:30.562146 AlgBench-2.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:12:30.574146 AlgBench-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-01 20:12:18.000000 AlgBench-2.0.0/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-01 20:12:18.000000 AlgBench-2.0.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-01 20:12:18.000000 AlgBench-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-01 20:12:18.000000 AlgBench-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-01 20:12:18.000000 AlgBench-2.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-01 20:12:18.000000 AlgBench-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-01 20:12:30.590146 AlgBench-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23809 2023-07-01 20:12:18.000000 AlgBench-2.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:12:30.578146 AlgBench-2.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-01 20:12:18.000000 AlgBench-2.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-01 20:12:18.000000 AlgBench-2.0.0/docs/algbench.db.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-01 20:12:18.000000 AlgBench-2.0.0/docs/algbench.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-01 20:12:18.000000 AlgBench-2.0.0/docs/algbench.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-01 20:12:18.000000 AlgBench-2.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-01 20:12:18.000000 AlgBench-2.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-01 20:12:18.000000 AlgBench-2.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-01 20:12:18.000000 AlgBench-2.0.0/docs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:12:30.562146 AlgBench-2.0.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:12:30.582146 AlgBench-2.0.0/examples/graph_coloring/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-01 20:12:18.000000 AlgBench-2.0.0/examples/graph_coloring/00_generate_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-01 20:12:18.000000 AlgBench-2.0.0/examples/graph_coloring/01_instances.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-01 20:12:18.000000 AlgBench-2.0.0/examples/graph_coloring/02_run_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-01 20:12:18.000000 AlgBench-2.0.0/examples/graph_coloring/02b_run_benchmark_with_slurminade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:12:30.582146 AlgBench-2.0.0/examples/graph_coloring/03_benchmark_data/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-01 20:12:18.000000 AlgBench-2.0.0/examples/graph_coloring/03_benchmark_data/algbench.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:12:30.582146 AlgBench-2.0.0/examples/graph_coloring/03_benchmark_data/arg_fingerprints/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-01 20:12:18.000000 AlgBench-2.0.0/examples/graph_coloring/03_benchmark_data/arg_fingerprints/_compressed.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:12:30.582146 AlgBench-2.0.0/examples/graph_coloring/03_benchmark_data/env_info/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-01 20:12:18.000000 AlgBench-2.0.0/examples/graph_coloring/03_benchmark_data/env_info/_compressed.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:12:30.582146 AlgBench-2.0.0/examples/graph_coloring/03_benchmark_data/results/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-01 20:12:18.000000 AlgBench-2.0.0/examples/graph_coloring/03_benchmark_data/results/_compressed.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    36424 2023-07-01 20:12:18.000000 AlgBench-2.0.0/examples/graph_coloring/04_check_results.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-01 20:12:18.000000 AlgBench-2.0.0/examples/graph_coloring/05_process_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-01 20:12:18.000000 AlgBench-2.0.0/examples/graph_coloring/06_simplified_results.json.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    15837 2023-07-01 20:12:18.000000 AlgBench-2.0.0/examples/graph_coloring/07_analyze_mean.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1072992 2023-07-01 20:12:18.000000 AlgBench-2.0.0/examples/graph_coloring/08_analyze_runtime.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   397344 2023-07-01 20:12:18.000000 AlgBench-2.0.0/examples/graph_coloring/09_analyze_quality.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-01 20:12:18.000000 AlgBench-2.0.0/examples/graph_coloring/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:12:30.586146 AlgBench-2.0.0/examples/graph_coloring/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-01 20:12:18.000000 AlgBench-2.0.0/examples/graph_coloring/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-01 20:12:18.000000 AlgBench-2.0.0/examples/graph_coloring/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-07-01 20:12:18.000000 AlgBench-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-01 20:12:18.000000 AlgBench-2.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 20:12:30.590146 AlgBench-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:12:30.566146 AlgBench-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:12:30.586146 AlgBench-2.0.0/src/AlgBench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-01 20:12:30.000000 AlgBench-2.0.0/src/AlgBench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-01 20:12:30.000000 AlgBench-2.0.0/src/AlgBench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 20:12:30.000000 AlgBench-2.0.0/src/AlgBench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-01 20:12:30.000000 AlgBench-2.0.0/src/AlgBench.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-01 20:12:30.000000 AlgBench-2.0.0/src/AlgBench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:12:30.590146 AlgBench-2.0.0/src/algbench/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-01 20:12:18.000000 AlgBench-2.0.0/src/algbench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-07-01 20:12:18.000000 AlgBench-2.0.0/src/algbench/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-01 20:12:18.000000 AlgBench-2.0.0/src/algbench/benchmark_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:12:30.590146 AlgBench-2.0.0/src/algbench/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-01 20:12:18.000000 AlgBench-2.0.0/src/algbench/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-01 20:12:18.000000 AlgBench-2.0.0/src/algbench/db/json_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-01 20:12:18.000000 AlgBench-2.0.0/src/algbench/db/nfs_json_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-07-01 20:12:18.000000 AlgBench-2.0.0/src/algbench/db/nfs_json_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-01 20:12:18.000000 AlgBench-2.0.0/src/algbench/db/nfs_json_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-01 20:12:18.000000 AlgBench-2.0.0/src/algbench/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-01 20:12:18.000000 AlgBench-2.0.0/src/algbench/fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-01 20:12:18.000000 AlgBench-2.0.0/src/algbench/log_capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-01 20:12:18.000000 AlgBench-2.0.0/src/algbench/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-01 20:12:18.000000 AlgBench-2.0.0/src/algbench/stream_with_time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:12:30.590146 AlgBench-2.0.0/src/algbench/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-01 20:12:18.000000 AlgBench-2.0.0/src/algbench/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-01 20:12:18.000000 AlgBench-2.0.0/src/algbench/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:12:30.590146 AlgBench-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-01 20:12:18.000000 AlgBench-2.0.0/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-01 20:12:18.000000 AlgBench-2.0.0/tests/test_logger.py
```

### Comparing `AlgBench-1.1.0/LICENSE` & `AlgBench-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AlgBench-1.1.0/PKG-INFO` & `AlgBench-2.0.0/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,509 +1,639 @@
-Metadata-Version: 2.1
-Name: AlgBench
-Version: 1.1.0
-Author-email: "TU Braunschweig, IBR, Algorithms Group (Dominik Krupke)" <krupke@ibr.cs.tu-bs.de>
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# AlgBench: A Python-util to run benchmarks for the empirical evaluation of algorithms.
-
-There are a number of challenges when performing benchmarks for (long-running)
-algorithms.
-
-- Saving all information requires a lot of **boilerplate code** and often you
-  forget something.
-- If you add some further instances or want to compare an additional parameter,
-  you have to check which data is already available to **skip existing
-  entries**. Same if you need to interrupt the benchmark.
-- Just piping the results into a file can create a **huge amount of data**, no
-  longer fitting into memory.
-- Proper benchmarks often take days or even weeks to run, such that
-  **parallelization** is necessary (e.g., with slurm) which requires a
-  thread-safe database.
-- Many file formats and databases are **difficult to access or impossible to
-  repair** once corrupted.
+AlgBench: A Python-util to run benchmarks for the empirical evaluation of algorithms.
+=====================================================================================
+
+.. image:: https://img.shields.io/pypi/v/algbench.svg
+   :target: https://pypi.python.org/pypi/algbench
+
+.. image:: https://img.shields.io/pypi/pyversions/algbench.svg
+   :target: https://pypi.python.org/pypi/algbench
+
+.. image:: https://img.shields.io/pypi/l/algbench.svg
+   :target: https://pypi.python.org/pypi/algbench
+
+.. image:: https://github.com/d-krupke/algbench/actions/workflows/pytest.yml/badge.svg
+   :target: https://github.com/d-krupke/AlgBench
+
+There are a number of challenges when performing benchmarks for
+(long-running) algorithms.
+
+-  Saving all information requires a lot of **boilerplate code** and
+   often you forget something.
+-  If you add some further instances or want to compare an additional
+   parameter, you have to check which data is already available to
+   **skip existing entries**. Same if you need to interrupt the
+   benchmark.
+-  Just piping the results into a file can create a **huge amount of
+   data**, no longer fitting into memory.
+-  Proper benchmarks often take days or even weeks to run, such that
+   **parallelization** is necessary (e.g., with slurm) which requires a
+   thread-safe database.
+-  Many file formats and databases are **difficult to access or
+   impossible to repair** once corrupted.
 
 AlgBench tries to ease your life by
 
-- saving a lot of the information and data (function arguments, return values,
-  runtime, environment information, stdout, etc.) automatically with a single
-  line of code
-- remembering which function arguments have already run and skipping those
-- providing a compressible database to save memory, and saving highly redundant
-  information, e.g., of the environment, only once
-- providing an NFS-compatible parallel database and compatibility to
-  distribution libraries, such as slurminade
-- using a simple format based on JSON and Zip to allow simple parsing and even
-  repairing broken databases by hand
+-  saving a lot of the information and data (function arguments, return
+   values, runtime, environment information, stdout, etc.) automatically
+   with a single line of code
+-  remembering which function arguments have already run and skipping
+   those
+-  providing a compressible database to save memory, and saving highly
+   redundant information, e.g., of the environment, only once
+-  providing an NFS-compatible parallel database and compatibility to
+   distribution libraries, such as slurminade
+-  using a simple format based on JSON and Zip to allow simple parsing
+   and even repairing broken databases by hand
 
 There is a predecessor project, called
-[AeMeasure](https://github.com/d-krupke/AeMeasure). AeMeasure made saving the
-data easy, but required more boilerplate code and reading the data was more
-difficult and less efficient.
-
-## Other things you should know about for empirical/experimental evaluations
-
-The following tools I consider essential for empirical evaluations (of algorithms):
-
-* [pandas](https://pandas.pydata.org/): Simple and powerful tool for working with data tables. Do your experiments and parse the important data into a pandas DataFrame.
-* [seaborn](https://seaborn.pydata.org/) and [matplotlib](https://matplotlib.org/): Creating beautiful plots from pandas DataFrames with little work.
-* [JupyterLab](https://jupyterlab.readthedocs.io/en/latest/): Interactive Python+Markdown documents. Great for analyzing data and sharing the insights. Works great with pandas and seaborn.
-
-AlgBench essentially takes over the part of saving the information from the runs and allowing you to easily extract pandas DataFrames from it.
-For very simple studies, you could also directly save your data into a Pandas DataFrame but even for nearly every serious experiment, you run into the problems mentioned in the beginning.
-
-Note that the actual algorithms can also be writen in another, more efficient programming language.
-It is reasonably easy to create Python-bindings, e.g., for C++ with [PyBind11](https://pybind11.readthedocs.io/), or just call the binaries with Python.
-
-Publishable evaluations often require extensive experiments that are best performed on a cluster of shared workstations.
-Many institutes and companies are using [slurm](https://slurm.schedmd.com/documentation.html) to schedule and distribute the workloads.
-The data is usually shared via a network file system (NFS), for which AlgBench is designed.
-While you usually also have databases available, they are not made for just dumping all the data you may need for analyzis and potentially debugging into.
-We developed an additonal tool [slurminade](https://github.com/d-krupke/slurminade) that allows you to distribute your experiments with just a few additional lines.
-You can see this in an example: [original script](./examples/graph_coloring/02_run_benchmark.py) vs [script with slurminade](./examples/graph_coloring/02b_run_benchmark_with_slurminade.py).
-
-Let me further recommend the books [A Guide To Experimental Algorithmics by Catherine McGeoch](https://www.cambridge.org/core/books/guide-to-experimental-algorithmics/CDB0CB718F6250E0806C909E1D3D1082) here that gives a good introduction into the big picture of performing empirical evluations for algorithms.
-If you want to know more about actually implementing complex algorithms for difficult problems, I recommend to read [In Pursuit of the Traveling Salesman by Bill Cook](https://press.princeton.edu/books/paperback/9780691163529/in-pursuit-of-the-traveling-salesman) or [The Traveling Salesman Problem: A Computational Study by Appelgate et al.](https://www.math.uwaterloo.ca/tsp/book/index.html) to really go into details.
-The Traveling Salesman Problem is an excellent example for this because it is probably had gotten the most attention of any NP-hard combinatorial problems.
-However, it can also be intimidating as you probably won't have the funds to look into any problem as deep as the Travelings Salesman Problem has been looked at.
-Maybe you want to read some papers from the SIAM Symposium on Algorithm Engineering and Experiments (ALENEX) to see how smaller studies can be performed (though, for most papers you will find aspects that could be improved).
+`AeMeasure <https://github.com/d-krupke/AeMeasure>`__. AeMeasure made
+saving the data easy, but required more boilerplate code and reading the
+data was more difficult and less efficient.
+
+Other things you should know about for empirical/experimental evaluations
+-------------------------------------------------------------------------
+
+The following tools I consider essential for empirical evaluations (of
+algorithms):
+
+-  `pandas <https://pandas.pydata.org/>`__: Simple and powerful tool for
+   working with data tables. Do your experiments and parse the important
+   data into a pandas DataFrame.
+-  `seaborn <https://seaborn.pydata.org/>`__ and
+   `matplotlib <https://matplotlib.org/>`__: Creating beautiful plots
+   from pandas DataFrames with little work.
+-  `JupyterLab <https://jupyterlab.readthedocs.io/en/latest/>`__:
+   Interactive Python+Markdown documents. Great for analyzing data and
+   sharing the insights. Works great with pandas and seaborn.
+
+AlgBench essentially takes over the part of saving the information from
+the runs and allowing you to easily extract pandas DataFrames from it.
+For very simple studies, you could also directly save your data into a
+Pandas DataFrame but even for nearly every serious experiment, you run
+into the problems mentioned in the beginning.
+
+Note that the actual algorithms can also be written in another, more
+efficient programming language. It is reasonably easy to create
+Python-bindings, e.g., for C++ with
+`pybind11 <https://pybind11.readthedocs.io/>`__, or just call the
+binaries with Python.
+
+Publishable evaluations often require extensive experiments that are
+best performed on a cluster of shared workstations. Many institutes and
+companies are using
+`slurm <https://slurm.schedmd.com/documentation.html>`__ to schedule and
+distribute the workloads. The data is usually shared via a network file
+system (NFS), for which AlgBench is designed. While you usually also
+have databases available, they are not made for just dumping all the
+data you may need for analyzis and potentially debugging into. We
+developed an additional tool
+`slurminade <https://github.com/d-krupke/slurminade>`__ that allows you
+to distribute your experiments with just a few additional lines. You can
+see this in an example: `original
+script <./examples/graph_coloring/02_run_benchmark.py>`__ vs `script
+with
+slurminade <./examples/graph_coloring/02b_run_benchmark_with_slurminade.py>`__.
+
+Let me further recommend the books `A Guide To Experimental Algorithmics
+by Catherine
+McGeoch <https://www.cambridge.org/core/books/guide-to-experimental-algorithmics/CDB0CB718F6250E0806C909E1D3D1082>`__
+here that gives a good introduction into the big picture of performing
+empirical evaluations for algorithms. If you want to know more about
+actually implementing complex algorithms for difficult problems, I
+recommend to read `In Pursuit of the Traveling Salesman by Bill
+Cook <https://press.princeton.edu/books/paperback/9780691163529/in-pursuit-of-the-traveling-salesman>`__
+or `The Traveling Salesman Problem: A Computational Study by Appelgate
+et al. <https://www.math.uwaterloo.ca/tsp/book/index.html>`__ to really
+go into details. The Traveling Salesman Problem is an excellent example
+for this because it is probably had gotten the most attention of any
+NP-hard combinatorial problems. However, it can also be intimidating as
+you probably won’t have the funds to look into any problem as deep as
+the Travelings Salesman Problem has been looked at. Maybe you want to
+read some papers from the SIAM Symposium on Algorithm Engineering and
+Experiments (ALENEX) to see how smaller studies can be performed
+(though, for most papers you will find aspects that could be improved).
 
-## Installation
+Installation
+------------
 
 You can install AlgBench using pip
 
-```bash
-pip install -U algbench
-```
-
-## Usage
-
-There is one important class `Benchmark` to run the benchmark, and two important
-functions `describe` and `read_as_pandas` to analyze the results.
-
-<p>
-<table width="100%" cellspacing=0 cellpadding=2 border=0 summary="section">
-<tr bgcolor="#ffc8d8">
-<td colspan=3 valign=bottom>&nbsp;<br>
-<font color="#000000" face="helvetica, arial"><a name="Benchmark">class <strong>Benchmark</strong></a>(<a href="builtins.html#object">builtins.object</a>)</font></td></tr>
-
-<tr bgcolor="#ffc8d8"><td rowspan=2><tt>&nbsp;&nbsp;&nbsp;</tt></td>
-<td colspan=2><tt>Benchmark(path:&nbsp;str)&nbsp;-&amp;gt;&nbsp;None<br>
-&nbsp;<br>
-This&nbsp;is&nbsp;the&nbsp;heart&nbsp;of&nbsp;the&nbsp;library.&nbsp;It&nbsp;allows&nbsp;to&nbsp;run,&nbsp;save,&nbsp;and&nbsp;load<br>
-a&nbsp;benchmark.<br>
-&nbsp;<br>
-The&nbsp;function&nbsp;`add`&nbsp;will&nbsp;run&nbsp;a&nbsp;configuration,&nbsp;if&nbsp;it&nbsp;is&nbsp;not<br>
-already&nbsp;in&nbsp;the&nbsp;database.&nbsp;You&nbsp;can&nbsp;also&nbsp;split&nbsp;this&nbsp;into&nbsp;`check`&nbsp;and<br>
-`run`.&nbsp;This&nbsp;may&nbsp;be&nbsp;advised&nbsp;if&nbsp;you&nbsp;want&nbsp;to&nbsp;distribute&nbsp;the&nbsp;execution.<br>
-&nbsp;<br>
-```python<br>
-from&nbsp;algbench&nbsp;import&nbsp;Benchmark<br>
-&nbsp;<br>
-benchmark&nbsp;=&nbsp;Benchmark("./test_benchmark")<br>
-&nbsp;<br>
-&nbsp;<br>
-def&nbsp;f(x,&nbsp;_test=2,&nbsp;default="default"):<br>
-&nbsp;&nbsp;&nbsp;&nbsp;print(x)&nbsp;&nbsp;#&nbsp;here&nbsp;you&nbsp;would&nbsp;run&nbsp;your&nbsp;algorithm<br>
-&nbsp;&nbsp;&nbsp;&nbsp;return&nbsp;{"r1":&nbsp;x,&nbsp;"r2":&nbsp;"test"}<br>
-&nbsp;<br>
-&nbsp;<br>
-benchmark.<a href="#Benchmark-add">add</a>(f,&nbsp;1,&nbsp;_test=None)<br>
-benchmark.<a href="#Benchmark-add">add</a>(f,&nbsp;2)<br>
-benchmark.<a href="#Benchmark-add">add</a>(f,&nbsp;3,&nbsp;_test=None)<br>
-&nbsp;<br>
-benchmark.<a href="#Benchmark-compress">compress</a>()<br>
-&nbsp;<br>
-for&nbsp;entry&nbsp;in&nbsp;benchmark:<br>
-&nbsp;&nbsp;&nbsp;&nbsp;print(entry["parameters"],&nbsp;entry["data"])<br>
-```<br>
-&nbsp;<br>
-The&nbsp;following&nbsp;functions&nbsp;are&nbsp;thread-safe:<br>
--&nbsp;exists<br>
--&nbsp;run<br>
--&nbsp;add<br>
--&nbsp;insert<br>
--&nbsp;front<br>
--&nbsp;__iter__<br>
-&nbsp;<br>
-Don't&nbsp;call&nbsp;any&nbsp;of&nbsp;the&nbsp;other&nbsp;functions&nbsp;while&nbsp;the&nbsp;benchmark&nbsp;is<br>
-running.&nbsp;It&nbsp;could&nbsp;lead&nbsp;to&nbsp;data&nbsp;loss.<br>&nbsp;</tt></td></tr>
-<tr><td>&nbsp;</td>
-<td width="100%">Methods defined here:<br>
-<dl><dt><a name="Benchmark-__init__"><strong>__init__</strong></a>(self, path: str) -&gt; None</dt><dd><tt>Just&nbsp;specify&nbsp;the&nbsp;path&nbsp;of&nbsp;where&nbsp;to&nbsp;put&nbsp;the<br>
-database&nbsp;and&nbsp;everything&nbsp;else&nbsp;happens&nbsp;magically.<br>
-Make&nbsp;sure&nbsp;not&nbsp;to&nbsp;use&nbsp;the&nbsp;same&nbsp;path&nbsp;for&nbsp;different<br>
-databases,&nbsp;as&nbsp;they&nbsp;will&nbsp;get&nbsp;mixed.</tt></dd></dl>
-
-<dl><dt><a name="Benchmark-__iter__"><strong>__iter__</strong></a>(self) -&gt; Generator[Dict, NoneType, NoneType]</dt><dd><tt>Iterate&nbsp;over&nbsp;all&nbsp;entries&nbsp;in&nbsp;the&nbsp;benchmark.<br>
-Use&nbsp;`front`&nbsp;to&nbsp;get&nbsp;a&nbsp;preview&nbsp;on&nbsp;how&nbsp;an&nbsp;entry&nbsp;looks&nbsp;like.</tt></dd></dl>
-
-<dl><dt><a name="Benchmark-add"><strong>add</strong></a>(self, func: Callable, *args, **kwargs)</dt><dd><tt>Will&nbsp;add&nbsp;the&nbsp;function&nbsp;call&nbsp;with&nbsp;the&nbsp;arguments<br>
-to&nbsp;the&nbsp;benchmark&nbsp;if&nbsp;not&nbsp;yet&nbsp;contained.<br>
-&nbsp;<br>
-Combination&nbsp;of&nbsp;`check`&nbsp;and&nbsp;`run`.<br>
-Will&nbsp;only&nbsp;call&nbsp;`run`&nbsp;if&nbsp;the&nbsp;arguments&nbsp;are&nbsp;not<br>
-yet&nbsp;in&nbsp;the&nbsp;benchmark.</tt></dd></dl>
-
-<dl><dt><a name="Benchmark-clear"><strong>clear</strong></a>(self)</dt><dd><tt>Clears&nbsp;all&nbsp;entries&nbsp;of&nbsp;the&nbsp;benchmark,&nbsp;without&nbsp;deleting<br>
-the&nbsp;benchmark&nbsp;itself.&nbsp;You&nbsp;can&nbsp;continue&nbsp;to&nbsp;use&nbsp;it&nbsp;afterwards.<br>
-&nbsp;<br>
-NOT&nbsp;THREAD-SAFE!</tt></dd></dl>
-
-<dl><dt><a name="Benchmark-compress"><strong>compress</strong></a>(self)</dt><dd><tt>Compress&nbsp;the&nbsp;data&nbsp;of&nbsp;the&nbsp;benchmark&nbsp;to&nbsp;take&nbsp;less&nbsp;disk&nbsp;space.<br>
-&nbsp;<br>
-NOT&nbsp;THREAD-SAFE!</tt></dd></dl>
-
-<dl><dt><a name="Benchmark-delete"><strong>delete</strong></a>(self)</dt><dd><tt>Delete&nbsp;the&nbsp;benchmark&nbsp;and&nbsp;all&nbsp;its&nbsp;files.&nbsp;Do&nbsp;not&nbsp;use&nbsp;it&nbsp;afterwards,<br>
-there&nbsp;are&nbsp;no&nbsp;files&nbsp;left&nbsp;to&nbsp;write&nbsp;results&nbsp;into.<br>
-If&nbsp;you&nbsp;just&nbsp;want&nbsp;to&nbsp;delete&nbsp;the&nbsp;content,&nbsp;use&nbsp;`clear.<br>
-&nbsp;<br>
-NOT&nbsp;THREAD-SAFE!</tt></dd></dl>
-
-<dl><dt><a name="Benchmark-delete_if"><strong>delete_if</strong></a>(self, condition: Callable[[Dict], bool])</dt><dd><tt>Delete&nbsp;entries&nbsp;if&nbsp;a&nbsp;specific&nbsp;condition&nbsp;is&nbsp;met.<br>
-This&nbsp;is&nbsp;currently&nbsp;inefficiently,&nbsp;as&nbsp;always&nbsp;a&nbsp;copy<br>
-of&nbsp;the&nbsp;benchmark&nbsp;is&nbsp;created.<br>
-Use&nbsp;`front`&nbsp;to&nbsp;get&nbsp;a&nbsp;preview&nbsp;on&nbsp;how&nbsp;an&nbsp;entry&nbsp;that&nbsp;is<br>
-passed&nbsp;to&nbsp;the&nbsp;condition&nbsp;looks&nbsp;like.<br>
-&nbsp;<br>
-NOT&nbsp;THREAD-SAFE!</tt></dd></dl>
-
-<dl><dt><a name="Benchmark-exists"><strong>exists</strong></a>(self, func: Callable, *args, **kwargs) -&gt; bool</dt><dd><tt>Use&nbsp;this&nbsp;function&nbsp;to&nbsp;check&nbsp;if&nbsp;an&nbsp;entry&nbsp;already&nbsp;exist&nbsp;and&nbsp;thus<br>
-does&nbsp;not&nbsp;have&nbsp;to&nbsp;be&nbsp;run&nbsp;again.&nbsp;If&nbsp;you&nbsp;want&nbsp;to&nbsp;have&nbsp;multiple<br>
-samples,&nbsp;add&nbsp;a&nbsp;sample&nbsp;index&nbsp;argument.<br>
-Caveat:&nbsp;This&nbsp;function&nbsp;may&nbsp;have&nbsp;false&nbsp;negatives.&nbsp;i.e.,&nbsp;says&nbsp;that&nbsp;it<br>
-&nbsp;&nbsp;does&nbsp;not&nbsp;exist&nbsp;despite&nbsp;it&nbsp;existing&nbsp;(only&nbsp;for&nbsp;fresh&nbsp;data).</tt></dd></dl>
-
-<dl><dt><a name="Benchmark-front"><strong>front</strong></a>(self) -&gt; Optional[Dict]</dt><dd><tt>Return&nbsp;the&nbsp;first&nbsp;entry&nbsp;of&nbsp;the&nbsp;benchmark.<br>
-Useful&nbsp;for&nbsp;checking&nbsp;its&nbsp;content.</tt></dd></dl>
-
-<dl><dt><a name="Benchmark-insert"><strong>insert</strong></a>(self, entry: Dict)</dt><dd><tt>Insert&nbsp;a&nbsp;raw&nbsp;entry,&nbsp;as&nbsp;returned&nbsp;by&nbsp;`__iter__`&nbsp;or&nbsp;`front`.</tt></dd></dl>
-
-<dl><dt><a name="Benchmark-repair"><strong>repair</strong></a>(self)</dt><dd><tt>Repairs&nbsp;the&nbsp;benchmark&nbsp;in&nbsp;case&nbsp;it&nbsp;has&nbsp;some&nbsp;broken&nbsp;entries.<br>
-&nbsp;<br>
-NOT&nbsp;THREAD-SAFE!</tt></dd></dl>
-
-<dl><dt><a name="Benchmark-run"><strong>run</strong></a>(self, func: Callable, *args, **kwargs)</dt><dd><tt>Will&nbsp;add&nbsp;the&nbsp;function&nbsp;call&nbsp;with&nbsp;the&nbsp;arguments<br>
-to&nbsp;the&nbsp;benchmark.</tt></dd></dl>
-
-<hr>
-Data descriptors defined here:<br>
-<dl><dt><strong>__dict__</strong></dt>
-<dd><tt>dictionary&nbsp;for&nbsp;instance&nbsp;variables&nbsp;(if&nbsp;defined)</tt></dd>
-</dl>
-<dl><dt><strong>__weakref__</strong></dt>
-<dd><tt>list&nbsp;of&nbsp;weak&nbsp;references&nbsp;to&nbsp;the&nbsp;object&nbsp;(if&nbsp;defined)</tt></dd>
-</dl>
-</td></tr></table>
-
-You can find [an example for graph coloring](./examples/graph_coloring/). The
-important parts are shown below.
-
-### Running a benchmark
-
-```python
-from _utils import InstanceDb
-from algbench import Benchmark
-import networkx as nx
-
-benchmark = Benchmark("03_benchmark_data")
-instances = InstanceDb("./01_instances.zip")
-
-
-def load_instance_and_run(instance_name: str, alg_params):
-    # load the instance outside the actual measurement
-    g = instances[instance_name]
-
-    def eval_greedy_alg(instance_name: str, alg_params, _instance: nx.Graph):
-        # arguments starting with `_` are not saved.
-        coloring = nx.coloring.greedy_coloring.greedy_color(_instance, **alg_params)
-        return {  # the returned values are saved to the database
-            "num_vertices": _instance.number_of_nodes(),
-            "num_edges": _instance.number_of_edges(),
-            "coloring": coloring,
-            "n_colors": max(coloring.values()) + 1,
-        }
-
-    benchmark.add(eval_greedy_alg, instance_name, alg_params, g)
-
-
-alg_params_to_evaluate = [
-    {"strategy": "largest_first", "interchange": True},
-    {"strategy": "largest_first", "interchange": False},
-    {"strategy": "random_sequential", "interchange": True},
-    {"strategy": "random_sequential", "interchange": False},
-    {"strategy": "smallest_last", "interchange": True},
-    {"strategy": "smallest_last", "interchange": False},
-    {"strategy": "independent_set"},
-    {"strategy": "connected_sequential_bfs", "interchange": True},
-    {"strategy": "connected_sequential_bfs", "interchange": False},
-    {"strategy": "connected_sequential_dfs", "interchange": True},
-    {"strategy": "connected_sequential_dfs", "interchange": False},
-    {"strategy": "saturation_largest_first"},
-]
-
-if __name__ == "__main__":
-    for instance_name in instances:
-        print(instance_name)
-        for conf in alg_params_to_evaluate:
-            load_instance_and_run(instance_name, conf)
-    benchmark.compress()
-```
-
-### Analyzing the data
-
-```python
-from algbench import describe, read_as_pandas, Benchmark
-
-describe("./03_benchmark_data/")
-```
-
-<details>
-<summary>Output</summary>
-<pre>
- result:
-| num_vertices: 68
-| num_edges: 697
-| coloring:
-|| 0: 7
-|| 1: 8
-|| 2: 2
-|| 3: 5
-|| 4: 3
-|| 5: 7
-|| 6: 7
-|| 7: 6
-|| 8: 5
-|| 9: 4
-|| 10: 5
-|| 11: 4
-|| 12: 0
-|| 13: 6
-|| 14: 0
-|| 15: 3
-|| 16: 5
-|| 17: 5
-|| 18: 7
-|| 19: 0
-|| ...
-| n_colors: 9
- timestamp: 2023-05-25T21:58:39.201553
- runtime: 0.002952098846435547
- stdout: 
- stderr: 
- env_fingerprint: 53ad3b5b29d082d7e2bca6881ec9fe35fe441ae1
- args_fingerprint: 10ce65b7a61d5ecbfcb1f4e390d72122f7a1f6ec
- parameters:
-| func: eval_greedy_alg
-| args:
-|| instance_name: graph_0
-|| alg_params:
-||| strategy: largest_first
-||| interchange: True
- argv: ['02_run_benchmark.py']
- env:
-| hostname: workstation-r7
-| python_version: 3.10.9 (main, Jan 11 2023, 15:21:40) [GCC 11.2.0]
-| python: /home/krupke/anaconda3/envs/mo310/bin/python3
-| cwd: /home/krupke/Repositories/AlgBench/examples/graph_coloring
-| environment: [{'name': 'virtualenv', 'path': '/home/krupke/.local/lib/python3.10/site-pack...
-| git_revision: 5357426feb4b49174c313ffa33e2cadf6a83e226
-| python_file: /home/krupke/Repositories/AlgBench/examples/graph_coloring/02_run_benchmark.py
-</pre>
-</details>
-
-```python
-# we can also see the raw data of the first entry using `front`
-Benchmark("./03_benchmark_data/").front()
-```
-
-<details>
-<summary>Output</summary>
-<pre>
-{'result': {'num_vertices': 68,
-  'num_edges': 697,
-  'coloring': {'0': 7,
-   '1': 8,
-   '2': 2,
-   '3': 5,
-   '4': 3,
-   '5': 7,
-   '6': 7,
-   '7': 6,
-   '8': 5,
-   '9': 4,
-   '10': 5,
-   '11': 4,
-   '12': 0,
-   '13': 6,
-   '14': 0,
-   '15': 3,
-   '16': 5,
-   '17': 5,
-   '18': 7,
-   '19': 0,
-   '20': 2,
-   '21': 3,
-    ...},
-  'n_colors': 9},
- 'timestamp': '2023-05-25T21:58:39.201553',
- 'runtime': 0.002952098846435547,
- 'stdout': '',
- 'stderr': '',
- 'env_fingerprint': '53ad3b5b29d082d7e2bca6881ec9fe35fe441ae1',
- 'args_fingerprint': '10ce65b7a61d5ecbfcb1f4e390d72122f7a1f6ec',
- 'parameters': {'func': 'eval_greedy_alg',
-  'args': {'instance_name': 'graph_0',
-   'alg_params': {'strategy': 'largest_first', 'interchange': True}}},
- 'argv': ['02_run_benchmark.py'],
- 'env': {'hostname': 'workstation-r7',
-  'python_version': '3.10.9 (main, Jan 11 2023, 15:21:40) [GCC 11.2.0]',
-  'python': '/home/krupke/anaconda3/envs/mo310/bin/python3',
-  'cwd': '/home/krupke/Repositories/AlgBench/examples/graph_coloring',
-  'environment': [{'name': 'virtualenv',
-    'path': '/home/krupke/.local/lib/python3.10/site-packages',
-    'version': '20.14.1'},
-   {'name': 'cfgv',
-    'path': '/home/krupke/.local/lib/python3.10/site-packages',
-    'version': '3.3.1'},
-  ...],
-  'git_revision': '5357426feb4b49174c313ffa33e2cadf6a83e226',
-  'python_file': '/home/krupke/Repositories/AlgBench/examples/graph_coloring/02_run_benchmark.py'}}
-</pre>
-</details>
-
-```python
-# we can extract a full pandas tables using `read_as_pandas`
-t = read_as_pandas(
-    "./03_benchmark_data/",
-    lambda result: {
-        "instance": result["parameters"]["args"]["instance_name"],
-        "strategy": result["parameters"]["args"]["alg_params"]["strategy"],
-        "interchange": result["parameters"]["args"]["alg_params"].get(
-            "interchange", None
-        ),
-        "colors": result["result"]["n_colors"],
-        "runtime": result["runtime"],
-        "num_vertices": result["result"]["num_vertices"],
-        "num_edges": result["result"]["num_edges"],
-    },
-)
-print(t)
-```
-
-<details>
-<summary>Output</summary>
-
-```
-       instance                  strategy interchange  colors   runtime ...
-0       graph_0             largest_first        True       9  0.002952  
-1       graph_0             largest_first       False      10  0.000183
-2       graph_0         random_sequential        True       9  0.003562
-3       graph_0         random_sequential       False      12  0.000173
-4       graph_0             smallest_last        True       9  0.003813
-...         ...                       ...         ...     ...       ...
-5995  graph_499  connected_sequential_bfs        True       3  0.000216
-5996  graph_499  connected_sequential_bfs       False       3  0.000132
-5997  graph_499  connected_sequential_dfs        True       3  0.000231
-5998  graph_499  connected_sequential_dfs       False       4  0.000132
-5999  graph_499  saturation_largest_first        None       3  0.000202
-
-
-[6000 rows x 7 columns]
-```
-</details>
+.. code:: bash
+
+   pip install -U algbench
+
+Usage
+-----
+
+There is one important class ``Benchmark`` to run the benchmark, and two
+important functions ``describe`` and ``read_as_pandas`` to analyze the
+results.
+
+1. Create a function that creates an entry in the database. Name all
+   arguments that should be saved and used for identifying entries
+   without ``_`` in the front. They should be JSON-compatible. Name all
+   arguments that provide higher objects, such as the instance database,
+   with an ``_`` in the front to tell *algbench* not to try to save or
+   compare them. Return everything you want to be saved for the
+   benchmark, best as a dictionary.
+
+.. code:: python
+
+   def create_benchmark_entry(
+       instance_name: str,  # instance identifier for the database
+       alg_parameters: dict,  # readable parameters for the algorithm
+       _instance,  # the parsed instance (not to be added to the database)
+   ):
+       solution = alg(_instance, **alg_parameters)
+       return {"objective_value": solution.obj()}
+
+2. Create a ``Benchmark``-object by passing it a path for the database.
+
+.. code:: python
+
+   from algbench import Benchmark
+
+   benchmark = Benchmark("./my_benchmark")
+
+   # Optionally if logging is used):
+   import logging
+
+   # Configure with logger should be captured and with which level
+   benchmark.capture_logger("my_alg", logging.INFO)
+   benchmark.capture_logger("my_alg.submodule", logging.WARNING)
+
+3. Use ``Benchmark.add`` to the function for all missing entries.
+
+.. code:: python
+
+   for instance_name, instance in instance_db:
+       for params in params_to_compare:
+           benchmark.add(
+               create_benchmark_entry,  # function (could also be a lambda)
+               # arguments for function
+               instance_name=instance_name,
+               alg_parameters=params,
+               _instance=instance,
+           )
+   benchmark.compress()  # reduce the size of the database by file compression
+
+4. Use a for loop to iterate over all raw entries
+
+.. code:: python
+
+   benchmark = Benchmark("./my_benchmark")
+   for entry in benchmark:
+       print(entry)  # dictionary
+
+or ``read_as_pandas`` to extract a simple pandas table
+
+.. code:: python
+
+   t = read_as_pandas(
+       "./my_benchmark/",
+       lambda result: {
+           "instance": result["parameters"]["args"]["instance_name"],
+           "alg_params": result["parameters"]["args"]["alg_params"],
+           "obj": result["result"]["objective_value"],
+           "runtime": result["runtime"],  # automatically saved
+       },
+   )
+
+You can use ``describe("./my_benchmark")`` to get an overview of the
+available entries.
+
+The ``Benchmark`` class provides further functionality, e.g., for
+deleting selected entries or reparing a broken database.
+
+You can find `an example for graph
+coloring <./examples/graph_coloring/>`__. The important parts are shown
+below.
+
+Running a benchmark
+~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+   from _utils import InstanceDb
+   from algbench import Benchmark
+   import networkx as nx
+
+   benchmark = Benchmark("03_benchmark_data")
+   instances = InstanceDb("./01_instances.zip")
+
+
+   def load_instance_and_run(instance_name: str, alg_params):
+       # load the instance outside the actual measurement
+       g = instances[instance_name]
+
+       def eval_greedy_alg(instance_name: str, alg_params, _instance: nx.Graph):
+           # arguments starting with `_` are not saved.
+           coloring = nx.coloring.greedy_coloring.greedy_color(_instance, **alg_params)
+           return {  # the returned values are saved to the database
+               "num_vertices": _instance.number_of_nodes(),
+               "num_edges": _instance.number_of_edges(),
+               "coloring": coloring,
+               "n_colors": max(coloring.values()) + 1,
+           }
+
+       benchmark.add(eval_greedy_alg, instance_name, alg_params, g)
+
+
+   alg_params_to_evaluate = [
+       {"strategy": "largest_first", "interchange": True},
+       {"strategy": "largest_first", "interchange": False},
+       {"strategy": "random_sequential", "interchange": True},
+       {"strategy": "random_sequential", "interchange": False},
+       {"strategy": "smallest_last", "interchange": True},
+       {"strategy": "smallest_last", "interchange": False},
+       {"strategy": "independent_set"},
+       {"strategy": "connected_sequential_bfs", "interchange": True},
+       {"strategy": "connected_sequential_bfs", "interchange": False},
+       {"strategy": "connected_sequential_dfs", "interchange": True},
+       {"strategy": "connected_sequential_dfs", "interchange": False},
+       {"strategy": "saturation_largest_first"},
+   ]
+
+   if __name__ == "__main__":
+       for instance_name in instances:
+           print(instance_name)
+           for conf in alg_params_to_evaluate:
+               load_instance_and_run(instance_name, conf)
+       benchmark.compress()
+
+Analyzing the data
+~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+   from algbench import describe, read_as_pandas, Benchmark
+
+   describe("./03_benchmark_data/")
+
+
+Output:
+
+::
+
+    result:
+   | num_vertices: 68
+   | num_edges: 697
+   | coloring:
+   || 0: 7
+   || 1: 8
+   || 2: 2
+   || 3: 5
+   || 4: 3
+   || 5: 7
+   || 6: 7
+   || 7: 6
+   || 8: 5
+   || 9: 4
+   || 10: 5
+   || 11: 4
+   || 12: 0
+   || 13: 6
+   || 14: 0
+   || 15: 3
+   || 16: 5
+   || 17: 5
+   || 18: 7
+   || 19: 0
+   || ...
+   | n_colors: 9
+    timestamp: 2023-05-25T21:58:39.201553
+    runtime: 0.002952098846435547
+    stdout:
+    stderr:
+    env_fingerprint: 53ad3b5b29d082d7e2bca6881ec9fe35fe441ae1
+    args_fingerprint: 10ce65b7a61d5ecbfcb1f4e390d72122f7a1f6ec
+    parameters:
+   | func: eval_greedy_alg
+   | args:
+   || instance_name: graph_0
+   || alg_params:
+   ||| strategy: largest_first
+   ||| interchange: True
+    argv: ['02_run_benchmark.py']
+    env:
+   | hostname: workstation-r7
+   | python_version: 3.10.9 (main, Jan 11 2023, 15:21:40) [GCC 11.2.0]
+   | python: /home/krupke/anaconda3/envs/mo310/bin/python3
+   | cwd: /home/krupke/Repositories/AlgBench/examples/graph_coloring
+   | environment: [{'name': 'virtualenv', 'path': '/home/krupke/.local/lib/python3.10/site-pack...
+   | git_revision: 5357426feb4b49174c313ffa33e2cadf6a83e226
+   | python_file: /home/krupke/Repositories/AlgBench/examples/graph_coloring/02_run_benchmark.py
+
+
+
+
+.. code:: python
+
+   # we can also see the raw data of the first entry using `front`
+   Benchmark("./03_benchmark_data/").front()
+
+
+
+Output:
+
+::
+
+   {'result': {'num_vertices': 68,
+     'num_edges': 697,
+     'coloring': {'0': 7,
+      '1': 8,
+      '2': 2,
+      '3': 5,
+      '4': 3,
+      '5': 7,
+      '6': 7,
+      '7': 6,
+      '8': 5,
+      '9': 4,
+      '10': 5,
+      '11': 4,
+      '12': 0,
+      '13': 6,
+      '14': 0,
+      '15': 3,
+      '16': 5,
+      '17': 5,
+      '18': 7,
+      '19': 0,
+      '20': 2,
+      '21': 3,
+       ...},
+     'n_colors': 9},
+    'timestamp': '2023-05-25T21:58:39.201553',
+    'runtime': 0.002952098846435547,
+    'stdout': '',
+    'stderr': '',
+    'env_fingerprint': '53ad3b5b29d082d7e2bca6881ec9fe35fe441ae1',
+    'args_fingerprint': '10ce65b7a61d5ecbfcb1f4e390d72122f7a1f6ec',
+    'parameters': {'func': 'eval_greedy_alg',
+     'args': {'instance_name': 'graph_0',
+      'alg_params': {'strategy': 'largest_first', 'interchange': True}}},
+    'argv': ['02_run_benchmark.py'],
+    'env': {'hostname': 'workstation-r7',
+     'python_version': '3.10.9 (main, Jan 11 2023, 15:21:40) [GCC 11.2.0]',
+     'python': '/home/krupke/anaconda3/envs/mo310/bin/python3',
+     'cwd': '/home/krupke/Repositories/AlgBench/examples/graph_coloring',
+     'environment': [{'name': 'virtualenv',
+       'path': '/home/krupke/.local/lib/python3.10/site-packages',
+       'version': '20.14.1'},
+      {'name': 'cfgv',
+       'path': '/home/krupke/.local/lib/python3.10/site-packages',
+       'version': '3.3.1'},
+     ...],
+     'git_revision': '5357426feb4b49174c313ffa33e2cadf6a83e226',
+     'python_file': '/home/krupke/Repositories/AlgBench/examples/graph_coloring/02_run_benchmark.py'}}
+
+
+.. code:: python
+
+   # we can extract a full pandas tables using `read_as_pandas`
+   t = read_as_pandas(
+       "./03_benchmark_data/",
+       lambda result: {
+           "instance": result["parameters"]["args"]["instance_name"],
+           "strategy": result["parameters"]["args"]["alg_params"]["strategy"],
+           "interchange": result["parameters"]["args"]["alg_params"].get(
+               "interchange", None
+           ),
+           "colors": result["result"]["n_colors"],
+           "runtime": result["runtime"],
+           "num_vertices": result["result"]["num_vertices"],
+           "num_edges": result["result"]["num_edges"],
+       },
+   )
+   print(t)
+
+Output:
+
+::
+
+          instance                  strategy interchange  colors   runtime ...
+   0       graph_0             largest_first        True       9  0.002952
+   1       graph_0             largest_first       False      10  0.000183
+   2       graph_0         random_sequential        True       9  0.003562
+   3       graph_0         random_sequential       False      12  0.000173
+   4       graph_0             smallest_last        True       9  0.003813
+   ...         ...                       ...         ...     ...       ...
+   5995  graph_499  connected_sequential_bfs        True       3  0.000216
+   5996  graph_499  connected_sequential_bfs       False       3  0.000132
+   5997  graph_499  connected_sequential_dfs        True       3  0.000231
+   5998  graph_499  connected_sequential_dfs       False       4  0.000132
+   5999  graph_499  saturation_largest_first        None       3  0.000202
+
 
-## Which information is saved?
+   [6000 rows x 7 columns]
+
+
+Which information is saved?
+---------------------------
 
 The following information is saved automatically:
 
-- function name
-- all arguments that do not begin with "\_"
-- the returned values
-- runtime
-- current date and time
-- hostname
-- Python version
-- Python binary path
-- current working directory
-- stdout and stderr
-- all installed modules and their versions
-- git revision
-- path of the python file
-
-## On doing good empirical evaluations of algorithms
-
-To get a feeling on the interesting instances and parameters, or generally on
-where to look deeper, you should first perform an explorative study. For such an
-explorative study, you should select some random parameters and instances, and
-just look how the numbers look. Iteratively change the parameters and instances,
-until you know what to evaluate properly. At that point, you can state some
-research questions and design corresponding workhorse studies to answer them.
+-  function name
+-  all arguments that do not begin with “\_” (use this to pass parsed
+   instances etc.)
+-  the returned values
+-  runtime
+-  current date and time
+-  hostname
+-  Python version
+-  Python binary path
+-  current working directory
+-  stdout and stderr
+-  all installed modules and their versions
+-  git revision
+-  path of the python file
+
+Things to be aware of
+---------------------
+
+-  Only function name and arguments not starting with “\_” are used to
+   compare entries. If an argument (or part of it) is not
+   JSON-compatible, the string of it is used.
+-  Arguments and return values that cannot be translated to json are
+   converted to string in the database. The default string conversion
+   may not be very useful.
+-  The stdout/strerr capturing only works if Python’s stdout/stderr are
+   used. E.g., C++ write by default to the system’s stdout/stderr and
+   cannot be captured (if you have been wondering, why C++-modules have
+   a bad output it Jupyter-notebooks: this is the reason). PyBind11
+   allows you `to change that
+   behavior <https://pybind11.readthedocs.io/en/stable/advanced/pycpp/utilities.html#using-python-s-print-function-in-c>`__.
+-  Global variables are not saved. Try to pass all important parameters
+   as function arguments, as they can also alter the benchmark and are
+   important to distinguish entries (e.g., you would want to recompute
+   an entry if the timelimit has been changed. This is only possible if
+   you tell algbench this by making it an argument).
+-  ‘sys.argv’ and the filename are saved, but not used for
+   distinguishing entries.
+
+On doing good empirical evaluations of algorithms
+-------------------------------------------------
+
+To get a feeling on the interesting instances and parameters, or
+generally on where to look deeper, you should first perform an
+explorative study. For such an explorative study, you should select some
+random parameters and instances, and just look how the numbers look.
+Iteratively change the parameters and instances, until you know what to
+evaluate properly. At that point, you can state some research questions
+and design corresponding workhorse studies to answer them.
 
 Here are some general hints:
 
-- Create a separate folder for every study.
-- Add a README.md into each folder that describes the study. At least describe
-  in a sentence, who created this study when in which context.
-- Have separated, numerated files for preparing, running, processing, checking,
-  and evaluating the study.
-- Extract a simplified pandas table from the database with only the important
-  data (e.g., stdout or environment information are only necessary for debugging
-  and don't need to be shared for evaluation). You can save pandas tables as
-  `.json.zip` such that they are small and can simply be added to your Git, even
-  when the full data is too large.
-- The file for checking the generated data should also describe it.
-- Use a separate Jupyter-notebook for each family of plots you want to generate.
-- Save the plots into files whose name you can easily trace back to the
-  generating notebook. You will probably copy them later into some paper and
-  half a year later, when you receive the reviews and want to do some changes,
-  you have to find the code that generated them.
+-  Do not mix algorithm code and experiment code, even if it saves you
+   rebuilding your package after every change. Such a mixed setup may
+   save you a command line, but it is harder to log and many problems
+   may remain unnoticed until you try to publish your algorithm. The
+   little overhead is worth it in the long run.
+-  Create a separate folder for every study. Don’t mix too much because
+   you want to reduce redundancies: Once things become complicated, you
+   may draw conclusions from the wrong data without noticing.
+-  Add a README.md into each folder that describes the study. At least
+   describe in a sentence, who created this study when in which context.
+-  Have separated, numerated files for preparing, running, processing,
+   checking, and evaluating the study.
+-  Extract a simplified pandas table from the database with only the
+   important data (e.g., stdout or environment information are only
+   necessary for debugging and don’t need to be shared for evaluation).
+   You can save pandas tables as ``.json.zip`` such that they are small
+   and can simply be added to your Git, even when the full data is too
+   large.
+-  The file for checking the generated data should also describe it.
+-  Use a separate Jupyter-notebook for each family of plots you want to
+   generate.
+-  Save the plots into files whose name you can easily trace back to the
+   generating notebook. You will probably copy them later into some
+   paper and half a year later, when you receive the reviews and want to
+   do some changes, you have to find the code that generated them.
+
+
+On gaining more insights using logging
+---------------------------------------
+
+If you develop complex algorithms, you often want to not only measure
+the runtime of thw whole algorithm, but also of its parts, as well as
+other information, such as the number of iterations, the current
+solution, etc. You can use the Python logging framework for this. The
+logging framework allows you to create loggers that can be configured
+individually. You can also create a logger for each module and
+submodule, and configure them individually. You can also configure
+handlers for the loggers, e.g., to write them to a file or to the
+console. You can also configure the level of the loggers and handlers,
+such that you can easily switch between different levels of logging.
+AlgBench allows you to capture the loggers and save them to the
+database. You can then extract them and analyze them.
+
+You can also use simple ``print`` statements, but they are not as
+flexible as the logging framework. While AlgBench can actually
+add the runtime to the print statements, it is not as easy to
+configure the output as with the logging framework. There is no
+way to disable the output for individual parts of your algorithm,
+or to change the level of the output. The logging framework is
+as easy to use as print statements, but much more flexible.
+It can be more expensive, but ``print`` statements are also not
+free and should be used with care.
+
+Here is an example for using the logging framework:
+
+.. code:: python
+
+   import logging
+
+
+   def my_alg():
+       logger = logging.getLogger("my_alg")
+       logger.info("Starting my_alg")
+       # do something
+       logger.info("Finished my_alg")
+
+
+   logger = logging.getLogger("my_alg")
+   logger.setLevel(logging.INFO)
+   logger.addHandler(logging.StreamHandler())
+   my_alg()
+
+A further advantage of the logging framework is that you can separate
+the message structure from the data. This allows you to easily query
+for specific events and directly extract the data you want to analyze.
+
+.. code:: python
+   logger.info("Submodule X needed %d iterations", 42)
+
+Will be saved as a dictionary with a separate field for the message and
+the data:
+
+::
+
+   {
+       "msg": "Submodule X needed %d iterations",
+       "args": [42],
+   }
+
+A further alternative is to use a dedicated class for stats that you
+pass around. This is generally a good idea, but takes more work and
+requires you to change the code. The logging framework is a good
+compromise between flexibility and ease of use.
+
+If your algorithm may be run in parallel or different contexts, you may want to allow
+to pass a logger to the algorithm. This allows you to create a
+separate logger for each context to separate the logs.
+
+::
+   Note that AlgBench v2 automatically adds the runtime to print statments and log entries.
 
-## Using Git LFS for the data
+Using Git LFS for the data
+--------------------------
 
-The data are large binary files. Use Git LFS to add them to your repository more
-efficiently.
+The data are large binary files. Use Git LFS to add them to your
+repository more efficiently.
 
-You can find a guide [here](https://git-lfs.com/) on how to install Git LFS.
+You can find a guide `here <https://git-lfs.com/>`__ on how to install
+Git LFS.
 
 Run
 
-```bash
-git lfs install
-````
+.. code:: bash
+
+   git lfs install
 
 to set up git LFS and
 
-```bash
-git lfs track "*.zip"
-```
+.. code:: bash
+
+   git lfs track "*.zip"
 
 to manage all zips via LFS.
 
-Alternatively, you can also just edit `.gitattributes` by hand
+Alternatively, you can also just edit ``.gitattributes`` by hand
+
+::
+
+   *.zip filter=lfs diff=lfs merge=lfs -text
+
+Finally, add ``.gitattributes`` to git via
 
-```
-*.zip filter=lfs diff=lfs merge=lfs -text
-```
-
-Finally, add `.gitattributes` to git via
-
-```bash
-git add .gitattributes
-```
-
-# Version History
-
-- **1.1.0** Some changes for efficiency turned out to be less robust in case of, e.g., keyboard interrupt. Fixed that.
-- **1.0.0** Changing the database layout, making it more efficient (breaking
-  change!).
-- **0.2.0** Changing database slightly to contain meta data and doing more
-  caching. Saving some more information.
-- **0.1.3** Fixed bug in arg fingerprint set.
-- **0.1.2** Fixed bug with empty rows in pandas table.
-- **0.1.1** Fixed bug with `delete_if`.
-- **0.1.0** First complete version
+.. code:: bash
+
+   git add .gitattributes
+
+Version History
+===============
+
+- **2.0.0** Extensive change of stdout/stderr handling and new logging functionality.
+   By default, stdout and stderr will now be saved with the runtime of the function.
+   Additionally, you can now capture loggers of the Python logging framework and save them to the database.
+   This is especially useful if you use a library that uses the logging framework. Prefere ``logging`` over ``print`` for logging information.
+-  **1.1.0** Some changes for efficiency turned out to be less robust in
+   case of, e.g., keyboard interrupt. Fixed that.
+-  **1.0.0** Changing the database layout, making it more efficient
+   (breaking change!).
+-  **0.2.0** Changing database slightly to contain meta data and doing
+   more caching. Saving some more information.
+-  **0.1.3** Fixed bug in arg fingerprint set.
+-  **0.1.2** Fixed bug with empty rows in pandas table.
+-  **0.1.1** Fixed bug with ``delete_if``.
+-  **0.1.0** First complete version
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `AlgBench-1.1.0/src/algbench/benchmark_db.py` & `AlgBench-2.0.0/src/algbench/benchmark_db.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-import shutil
-from .fingerprint import fingerprint
-from .db import NfsJsonSet, NfsJsonDict, NfsJsonList
-from .environment import get_environment_info
-
 import json
 import os
-import typing
+import shutil
 import sys
+import typing
+
+from .db import NfsJsonDict, NfsJsonList, NfsJsonSet
+from .environment import get_environment_info
+from .fingerprint import fingerprint
 
 
 class BenchmarkDb:
     def __init__(self, path) -> None:
         self.path = path
         self._create_or_check_info_file()
         self._arg_fingerprints = NfsJsonSet(os.path.join(path, "arg_fingerprints"))
         self._data = NfsJsonList(os.path.join(path, "results"))
         self._env_data = NfsJsonDict(os.path.join(path, "env_info"))
 
     def _create_or_check_info_file(self):
         info_path = os.path.join(self.path, "algbench.json")
         if os.path.exists(info_path):
-            with open(info_path, "r") as f:
+            with open(info_path) as f:
                 info = json.load(f)
                 if info.get("version", "v0.0.0")[1] == "0":
-                    raise RuntimeError(
-                        "Incompatible database of old version of AlgBench."
-                    )
+                    msg = "Incompatible database of old version of AlgBench."
+                    raise RuntimeError(msg)
         else:
             os.makedirs(self.path, exist_ok=True)
             with open(info_path, "w") as f:
                 json.dump({"version": "v1.0.0"}, f)
 
     def contains_fingerprint(self, fingerprint):
         return fingerprint in self._arg_fingerprints
```

### Comparing `AlgBench-1.1.0/src/algbench/db/json_serializer.py` & `AlgBench-2.0.0/src/algbench/db/json_serializer.py`

 * *Files identical despite different names*

### Comparing `AlgBench-1.1.0/src/algbench/db/nfs_json_dict.py` & `AlgBench-2.0.0/src/algbench/db/nfs_json_dict.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,58 +1,54 @@
-from .nfs_json_list import NfsJsonList
+import json
+import typing
 
 from .json_serializer import to_json
-import typing
-import json
+from .nfs_json_list import NfsJsonList
 
 
 def _equal(a, b):
     return json.dumps(a) == json.dumps(b)
 
 
 class NfsJsonDict:
     def __init__(self, path) -> None:
         self._db = NfsJsonList(path)
-        self._values: typing.Dict = dict()
+        self._values: typing.Dict = {}
         self.load()
 
     def load(self):
         data = self._db.load()
         for d in data:
             if not isinstance(d, dict):
-                raise ValueError(
-                    "Found data that is not a dict. "
-                    "Are you sure this is a NfsJsonDict-database?"
-                )
+                msg = "Found data that is not a dict. Are you sure this is a NfsJsonDict-database?"
+                raise ValueError(msg)
             self._values.update(d)
 
     def __contains__(self, item: str):
         return item in self._values
 
     def __setitem__(self, key: str, value):
         key = str(key)
         value = to_json(value)
-        if key in self._values:
-            if _equal(self._values[key], value):
-                return
+        if key in self._values and _equal(self._values[key], value):
+            return
         self._db.append({key: value})
         self._values[key] = value
 
     def __getitem__(self, key: str):
         return self._values[key]
 
     def get(self, *args, **kwargs):
         return self._values.get(*args, **kwargs)
 
     def update(self, *args, **kwargs):
         return self._values.update(*args, **kwargs)
 
     def items(self):
-        for key, value in self._values.items():
-            yield key, value
+        yield from self._values.items()
 
     def compress(self):
         self.load()  # in case there have been writes in the meantime
         self._db.clear()
         self._db.append(self._values)
         self._db.compress()
```

### Comparing `AlgBench-1.1.0/src/algbench/db/nfs_json_list.py` & `AlgBench-2.0.0/src/algbench/db/nfs_json_list.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-from .json_serializer import to_json
-import logging
-
-
-import shutil
 import datetime
 import json
+import logging
 import os
 import os.path
 import pathlib
 import random
+import shutil
 import socket
 import typing
 import zipfile
 from zipfile import ZipFile
 
+from .json_serializer import to_json
+
 _log = logging.getLogger("AlgBench")
 
 
 class NfsJsonList:
     """
     A simple database to dump data (dictionaries) into. Should be reasonably threadsafe
     even for slurm pools with NFS.
@@ -26,27 +25,26 @@
     def __init__(self, path: typing.Union[str, pathlib.Path]):
         self.path: typing.Union[str, pathlib.Path] = path
         if not os.path.exists(path):
             # Could fail in very few unlucky cases on an NFS (parallel creations)
             os.makedirs(path, exist_ok=True)
             _log.info(f"Created new database '{path}'.")
         if os.path.isfile(path):
-            raise RuntimeError(
-                f"Cannot create database {path} because there "
-                "exists an equally named file."
-            )
+            msg = f"Cannot create database {path} because there exists an equally named file."
+            raise RuntimeError(msg)
         self._subfile_path: typing.Union[str, pathlib.Path] = self._get_unique_name()
         self._cache: typing.List = []
 
     def _get_unique_name(self, _tries=3):
         """
         Generate a unique file name to prevent collisions of parallel processes.
         """
         if _tries <= 0:
-            raise RuntimeError("Could not generate a unique file name. This is odd.")
+            msg = "Could not generate a unique file name. This is odd."
+            raise RuntimeError(msg)
         hostname = socket.gethostname()
         timestamp = datetime.datetime.now().strftime("%Y%m%d%H%M")
         rand = random.randint(0, 10000)
         name = f"{timestamp}-{hostname}-{rand}.data"
         if os.path.exists(name):
             return self._get_unique_name(_tries=_tries - 1)
         return name
@@ -89,22 +87,23 @@
         path = os.path.join(self.path, self._subfile_path)
         with open(path, "a") as f:
             for data in self._cache:
                 data = to_json(data)
                 f.write(json.dumps(data) + "\n")
             _log.info(f"Wrote {len(self._cache)} entries to disk.")
         if os.path.getsize(path) <= 0:
-            raise RuntimeError("Could not write to disk. Resulting file has zero size.")
+            msg = "Could not write to disk. Resulting file has zero size."
+            raise RuntimeError(msg)
         if not os.path.isfile(path):
-            raise RuntimeError("Could not write to disk for unknown reasons.")
+            msg = "Could not write to disk for unknown reasons."
+            raise RuntimeError(msg)
         self._cache.clear()
 
     def iter_cache(self):
-        for entry in self._cache:
-            yield entry
+        yield from self._cache
 
     def iter_compressed(self):
         compr_path = os.path.join(self.path, "_compressed.zip")
         if os.path.exists(compr_path):
             with ZipFile(compr_path, "r") as z:
                 for filename in z.filelist:
                     with z.open(filename, "r") as f:
@@ -121,15 +120,15 @@
 
     def iter_uncompressed(self):
         # load uncompressed data
         for fp in os.listdir(self.path):
             path = os.path.join(self.path, fp)
             if not os.path.isfile(path) or not path.endswith(".data"):
                 continue
-            with open(path, "r") as f:
+            with open(path) as f:
                 for entry in f.readlines():
                     try:
                         entry_ = json.loads(entry)
                         yield entry_
                     except Exception:
                         # Just continue. Probably a synchronization thing of the NFS.
                         _log.warning(f'Could not load "{entry}" in "{path}".')
```

### Comparing `AlgBench-1.1.0/src/algbench/db/nfs_json_set.py` & `AlgBench-2.0.0/src/algbench/db/nfs_json_set.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import typing
+
 from .json_serializer import to_json
 from .nfs_json_list import NfsJsonList
-import typing
 
 
 class NfsJsonSet:
     def __init__(self, path) -> None:
         self._db = NfsJsonList(path)
         self._values: typing.Set = set()
         self.load()
@@ -24,16 +25,15 @@
         return item
 
     def update(self, items):
         for item in items:
             self.add(item)
 
     def __iter__(self):
-        for item in self._values:
-            yield item
+        yield from self._values
 
     def compress(self):
         """
         WARNING: This operation is not thread-safe!
         """
         self.load()  # in case there have been writes in the meantime
         self._db.clear()
```

### Comparing `AlgBench-1.1.0/src/algbench/environment.py` & `AlgBench-2.0.0/src/algbench/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 code is running.
 """
 import os
 import socket
 import subprocess
 import sys
 import typing
-import pkg_resources
+
 import __main__
+import pkg_resources
 
 __cached = None
 
 
 def get_git_revision() -> typing.Optional[str]:
     """
     Return the git revision of the current working directory.
```

### Comparing `AlgBench-1.1.0/src/algbench/utils/timer.py` & `AlgBench-2.0.0/src/algbench/utils/timer.py`

 * *Files identical despite different names*

### Comparing `AlgBench-1.1.0/tests/test_basics.py` & `AlgBench-2.0.0/tests/test_basics.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-from algbench.benchmark import Benchmark
-
+from algbench import Benchmark, describe
+import logging
 
 def test_simple():
     benchmark = Benchmark("./test_benchmark")
 
     def f(x, _test=2, default="default"):
         print(x)
+        logging.getLogger("test").info("f(%d)", x)
         return {"r1": x, "r2": "test"}
 
+    benchmark.capture_logger("test", logging.INFO)
     benchmark.add(f, 1, _test=None)
     benchmark.add(f, 2)
     benchmark.add(f, 3, _test=None)
 
     benchmark.compress()
     benchmark.delete_if(lambda entry: False)
     n = 0
     for entry in benchmark:
         print({k: v for k, v in entry.items() if k != "env"})
         n += 1
     assert n == 3
+
+    describe("./test_benchmark")
     benchmark.delete()
```

