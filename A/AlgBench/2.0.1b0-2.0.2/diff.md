# Comparing `tmp/AlgBench-2.0.1b0.tar.gz` & `tmp/AlgBench-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlgBench-2.0.1b0.tar", last modified: Sat Jul  1 20:23:54 2023, max compression
+gzip compressed data, was "AlgBench-2.0.2.tar", last modified: Sat Jul  1 20:32:57 2023, max compression
```

## Comparing `AlgBench-2.0.1b0.tar` & `AlgBench-2.0.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:23:54.994362 AlgBench-2.0.1b0/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-01 20:23:43.000000 AlgBench-2.0.1b0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:23:54.986362 AlgBench-2.0.1b0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:23:54.986362 AlgBench-2.0.1b0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-01 20:23:43.000000 AlgBench-2.0.1b0/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-01 20:23:43.000000 AlgBench-2.0.1b0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-01 20:23:43.000000 AlgBench-2.0.1b0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-01 20:23:43.000000 AlgBench-2.0.1b0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-01 20:23:43.000000 AlgBench-2.0.1b0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-01 20:23:43.000000 AlgBench-2.0.1b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24359 2023-07-01 20:23:54.994362 AlgBench-2.0.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23814 2023-07-01 20:23:43.000000 AlgBench-2.0.1b0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:23:54.990362 AlgBench-2.0.1b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-01 20:23:43.000000 AlgBench-2.0.1b0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-01 20:23:43.000000 AlgBench-2.0.1b0/docs/algbench.db.rst
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-01 20:23:43.000000 AlgBench-2.0.1b0/docs/algbench.rst
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-01 20:23:43.000000 AlgBench-2.0.1b0/docs/algbench.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-01 20:23:43.000000 AlgBench-2.0.1b0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-01 20:23:43.000000 AlgBench-2.0.1b0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-01 20:23:43.000000 AlgBench-2.0.1b0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-01 20:23:43.000000 AlgBench-2.0.1b0/docs/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:23:54.986362 AlgBench-2.0.1b0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:23:54.990362 AlgBench-2.0.1b0/examples/graph_coloring/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-01 20:23:43.000000 AlgBench-2.0.1b0/examples/graph_coloring/00_generate_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-01 20:23:43.000000 AlgBench-2.0.1b0/examples/graph_coloring/01_instances.zip
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-01 20:23:43.000000 AlgBench-2.0.1b0/examples/graph_coloring/02_run_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-01 20:23:43.000000 AlgBench-2.0.1b0/examples/graph_coloring/02b_run_benchmark_with_slurminade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:23:54.990362 AlgBench-2.0.1b0/examples/graph_coloring/03_benchmark_data/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-01 20:23:43.000000 AlgBench-2.0.1b0/examples/graph_coloring/03_benchmark_data/algbench.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:23:54.994362 AlgBench-2.0.1b0/examples/graph_coloring/03_benchmark_data/arg_fingerprints/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-01 20:23:43.000000 AlgBench-2.0.1b0/examples/graph_coloring/03_benchmark_data/arg_fingerprints/_compressed.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:23:54.994362 AlgBench-2.0.1b0/examples/graph_coloring/03_benchmark_data/env_info/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-01 20:23:43.000000 AlgBench-2.0.1b0/examples/graph_coloring/03_benchmark_data/env_info/_compressed.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:23:54.994362 AlgBench-2.0.1b0/examples/graph_coloring/03_benchmark_data/results/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-01 20:23:43.000000 AlgBench-2.0.1b0/examples/graph_coloring/03_benchmark_data/results/_compressed.zip
--rw-r--r--   0 runner    (1001) docker     (123)    36424 2023-07-01 20:23:43.000000 AlgBench-2.0.1b0/examples/graph_coloring/04_check_results.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-01 20:23:43.000000 AlgBench-2.0.1b0/examples/graph_coloring/05_process_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-01 20:23:43.000000 AlgBench-2.0.1b0/examples/graph_coloring/06_simplified_results.json.zip
--rw-r--r--   0 runner    (1001) docker     (123)    15837 2023-07-01 20:23:43.000000 AlgBench-2.0.1b0/examples/graph_coloring/07_analyze_mean.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  1072992 2023-07-01 20:23:44.000000 AlgBench-2.0.1b0/examples/graph_coloring/08_analyze_runtime.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   397344 2023-07-01 20:23:44.000000 AlgBench-2.0.1b0/examples/graph_coloring/09_analyze_quality.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-01 20:23:44.000000 AlgBench-2.0.1b0/examples/graph_coloring/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:23:54.994362 AlgBench-2.0.1b0/examples/graph_coloring/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-01 20:23:44.000000 AlgBench-2.0.1b0/examples/graph_coloring/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-01 20:23:44.000000 AlgBench-2.0.1b0/examples/graph_coloring/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-01 20:23:44.000000 AlgBench-2.0.1b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-01 20:23:44.000000 AlgBench-2.0.1b0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 20:23:54.994362 AlgBench-2.0.1b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:23:54.986362 AlgBench-2.0.1b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:23:54.994362 AlgBench-2.0.1b0/src/AlgBench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24359 2023-07-01 20:23:54.000000 AlgBench-2.0.1b0/src/AlgBench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-01 20:23:54.000000 AlgBench-2.0.1b0/src/AlgBench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 20:23:54.000000 AlgBench-2.0.1b0/src/AlgBench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-01 20:23:54.000000 AlgBench-2.0.1b0/src/AlgBench.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-01 20:23:54.000000 AlgBench-2.0.1b0/src/AlgBench.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:23:54.994362 AlgBench-2.0.1b0/src/algbench/
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-01 20:23:44.000000 AlgBench-2.0.1b0/src/algbench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-07-01 20:23:44.000000 AlgBench-2.0.1b0/src/algbench/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-01 20:23:44.000000 AlgBench-2.0.1b0/src/algbench/benchmark_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:23:54.994362 AlgBench-2.0.1b0/src/algbench/db/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-01 20:23:44.000000 AlgBench-2.0.1b0/src/algbench/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-01 20:23:44.000000 AlgBench-2.0.1b0/src/algbench/db/json_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-01 20:23:44.000000 AlgBench-2.0.1b0/src/algbench/db/nfs_json_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-07-01 20:23:44.000000 AlgBench-2.0.1b0/src/algbench/db/nfs_json_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-01 20:23:44.000000 AlgBench-2.0.1b0/src/algbench/db/nfs_json_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-01 20:23:44.000000 AlgBench-2.0.1b0/src/algbench/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-01 20:23:44.000000 AlgBench-2.0.1b0/src/algbench/fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-01 20:23:44.000000 AlgBench-2.0.1b0/src/algbench/log_capture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-01 20:23:44.000000 AlgBench-2.0.1b0/src/algbench/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-01 20:23:44.000000 AlgBench-2.0.1b0/src/algbench/stream_with_time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:23:54.994362 AlgBench-2.0.1b0/src/algbench/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-01 20:23:44.000000 AlgBench-2.0.1b0/src/algbench/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-01 20:23:44.000000 AlgBench-2.0.1b0/src/algbench/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:23:54.994362 AlgBench-2.0.1b0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-01 20:23:44.000000 AlgBench-2.0.1b0/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-01 20:23:44.000000 AlgBench-2.0.1b0/tests/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.355591 AlgBench-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-01 20:32:45.000000 AlgBench-2.0.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.331591 AlgBench-2.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.339591 AlgBench-2.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-01 20:32:45.000000 AlgBench-2.0.2/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-01 20:32:45.000000 AlgBench-2.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-01 20:32:45.000000 AlgBench-2.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-01 20:32:45.000000 AlgBench-2.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-01 20:32:45.000000 AlgBench-2.0.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-01 20:32:45.000000 AlgBench-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24357 2023-07-01 20:32:57.355591 AlgBench-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23814 2023-07-01 20:32:45.000000 AlgBench-2.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.343591 AlgBench-2.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-01 20:32:45.000000 AlgBench-2.0.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-01 20:32:45.000000 AlgBench-2.0.2/docs/algbench.db.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-01 20:32:45.000000 AlgBench-2.0.2/docs/algbench.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-01 20:32:45.000000 AlgBench-2.0.2/docs/algbench.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-01 20:32:45.000000 AlgBench-2.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-01 20:32:45.000000 AlgBench-2.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-01 20:32:45.000000 AlgBench-2.0.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-01 20:32:45.000000 AlgBench-2.0.2/docs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.331591 AlgBench-2.0.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.347591 AlgBench-2.0.2/examples/graph_coloring/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-01 20:32:45.000000 AlgBench-2.0.2/examples/graph_coloring/00_generate_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/01_instances.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/02_run_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/02b_run_benchmark_with_slurminade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.347591 AlgBench-2.0.2/examples/graph_coloring/03_benchmark_data/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/03_benchmark_data/algbench.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.347591 AlgBench-2.0.2/examples/graph_coloring/03_benchmark_data/arg_fingerprints/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/03_benchmark_data/arg_fingerprints/_compressed.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.347591 AlgBench-2.0.2/examples/graph_coloring/03_benchmark_data/env_info/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/03_benchmark_data/env_info/_compressed.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.347591 AlgBench-2.0.2/examples/graph_coloring/03_benchmark_data/results/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/03_benchmark_data/results/_compressed.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    36424 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/04_check_results.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/05_process_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/06_simplified_results.json.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    15837 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/07_analyze_mean.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1072992 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/08_analyze_runtime.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   397344 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/09_analyze_quality.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.347591 AlgBench-2.0.2/examples/graph_coloring/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-01 20:32:46.000000 AlgBench-2.0.2/examples/graph_coloring/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-01 20:32:46.000000 AlgBench-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-01 20:32:46.000000 AlgBench-2.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 20:32:57.355591 AlgBench-2.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.335591 AlgBench-2.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.351591 AlgBench-2.0.2/src/AlgBench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24357 2023-07-01 20:32:57.000000 AlgBench-2.0.2/src/AlgBench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-01 20:32:57.000000 AlgBench-2.0.2/src/AlgBench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 20:32:57.000000 AlgBench-2.0.2/src/AlgBench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-01 20:32:57.000000 AlgBench-2.0.2/src/AlgBench.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-01 20:32:57.000000 AlgBench-2.0.2/src/AlgBench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.355591 AlgBench-2.0.2/src/algbench/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/benchmark_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.355591 AlgBench-2.0.2/src/algbench/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/db/json_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/db/nfs_json_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/db/nfs_json_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/db/nfs_json_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/log_capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/stream_with_time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.355591 AlgBench-2.0.2/src/algbench/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-01 20:32:46.000000 AlgBench-2.0.2/src/algbench/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:57.355591 AlgBench-2.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-01 20:32:46.000000 AlgBench-2.0.2/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-01 20:32:46.000000 AlgBench-2.0.2/tests/test_logger.py
```

### Comparing `AlgBench-2.0.1b0/.github/workflows/pytest.yml` & `AlgBench-2.0.2/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/.github/workflows/release.yml` & `AlgBench-2.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/.gitignore` & `AlgBench-2.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/.pre-commit-config.yaml` & `AlgBench-2.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/.readthedocs.yaml` & `AlgBench-2.0.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/LICENSE` & `AlgBench-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/PKG-INFO` & `AlgBench-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlgBench
-Version: 2.0.1b0
+Version: 2.0.2
 Summary: Util for benchmarking algorithms.
 Author-email: "TU Braunschweig, IBR, Algorithms Group (Dominik Krupke)" <krupke@ibr.cs.tu-bs.de>
 Project-URL: Homepage, https://github.com/d-krupke/AlgBench
 Project-URL: Issues, https://github.com/d-krupke/AlgBench/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `AlgBench-2.0.1b0/README.rst` & `AlgBench-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/docs/Makefile` & `AlgBench-2.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/docs/algbench.db.rst` & `AlgBench-2.0.2/docs/algbench.db.rst`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/docs/algbench.rst` & `AlgBench-2.0.2/docs/algbench.rst`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/docs/conf.py` & `AlgBench-2.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/docs/make.bat` & `AlgBench-2.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/examples/graph_coloring/00_generate_instances.py` & `AlgBench-2.0.2/examples/graph_coloring/00_generate_instances.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/examples/graph_coloring/02_run_benchmark.py` & `AlgBench-2.0.2/examples/graph_coloring/02_run_benchmark.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/examples/graph_coloring/02b_run_benchmark_with_slurminade.py` & `AlgBench-2.0.2/examples/graph_coloring/02b_run_benchmark_with_slurminade.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/examples/graph_coloring/04_check_results.ipynb` & `AlgBench-2.0.2/examples/graph_coloring/04_check_results.ipynb`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/examples/graph_coloring/05_process_results.py` & `AlgBench-2.0.2/examples/graph_coloring/05_process_results.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/examples/graph_coloring/07_analyze_mean.ipynb` & `AlgBench-2.0.2/examples/graph_coloring/07_analyze_mean.ipynb`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/examples/graph_coloring/08_analyze_runtime.ipynb` & `AlgBench-2.0.2/examples/graph_coloring/08_analyze_runtime.ipynb`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/examples/graph_coloring/09_analyze_quality.ipynb` & `AlgBench-2.0.2/examples/graph_coloring/09_analyze_quality.ipynb`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/examples/graph_coloring/README.md` & `AlgBench-2.0.2/examples/graph_coloring/README.md`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/examples/graph_coloring/_utils/__init__.py` & `AlgBench-2.0.2/examples/graph_coloring/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/pyproject.toml` & `AlgBench-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/src/AlgBench.egg-info/PKG-INFO` & `AlgBench-2.0.2/src/AlgBench.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlgBench
-Version: 2.0.1b0
+Version: 2.0.2
 Summary: Util for benchmarking algorithms.
 Author-email: "TU Braunschweig, IBR, Algorithms Group (Dominik Krupke)" <krupke@ibr.cs.tu-bs.de>
 Project-URL: Homepage, https://github.com/d-krupke/AlgBench
 Project-URL: Issues, https://github.com/d-krupke/AlgBench/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `AlgBench-2.0.1b0/src/AlgBench.egg-info/SOURCES.txt` & `AlgBench-2.0.2/src/AlgBench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/src/algbench/__init__.py` & `AlgBench-2.0.2/src/algbench/__init__.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/src/algbench/benchmark.py` & `AlgBench-2.0.2/src/algbench/benchmark.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/src/algbench/benchmark_db.py` & `AlgBench-2.0.2/src/algbench/benchmark_db.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/src/algbench/db/json_serializer.py` & `AlgBench-2.0.2/src/algbench/db/json_serializer.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/src/algbench/db/nfs_json_dict.py` & `AlgBench-2.0.2/src/algbench/db/nfs_json_dict.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/src/algbench/db/nfs_json_list.py` & `AlgBench-2.0.2/src/algbench/db/nfs_json_list.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/src/algbench/db/nfs_json_set.py` & `AlgBench-2.0.2/src/algbench/db/nfs_json_set.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/src/algbench/environment.py` & `AlgBench-2.0.2/src/algbench/environment.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/src/algbench/log_capture.py` & `AlgBench-2.0.2/src/algbench/log_capture.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/src/algbench/pandas.py` & `AlgBench-2.0.2/src/algbench/pandas.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/src/algbench/stream_with_time.py` & `AlgBench-2.0.2/src/algbench/stream_with_time.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/src/algbench/utils/timer.py` & `AlgBench-2.0.2/src/algbench/utils/timer.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/tests/test_basics.py` & `AlgBench-2.0.2/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.0.1b0/tests/test_logger.py` & `AlgBench-2.0.2/tests/test_logger.py`

 * *Files identical despite different names*

