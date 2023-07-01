# Comparing `tmp/Navix-0.2.1.tar.gz` & `tmp/Navix-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Navix-0.2.1.tar", last modified: Mon Jun 19 21:27:11 2023, max compression
+gzip compressed data, was "Navix-0.3.5.tar", last modified: Sat Jul  1 07:54:26 2023, max compression
```

## Comparing `Navix-0.2.1.tar` & `Navix-0.3.5.tar`

### file list

```diff
@@ -1,45 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:27:11.332955 Navix-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:27:11.324955 Navix-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:27:11.328955 Navix-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-19 21:26:55.000000 Navix-0.2.1/.github/workflows/CD.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-19 21:26:55.000000 Navix-0.2.1/.github/workflows/CI.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-19 21:26:55.000000 Navix-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 21:26:55.000000 Navix-0.2.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-19 21:26:55.000000 Navix-0.2.1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-19 21:26:55.000000 Navix-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 21:26:55.000000 Navix-0.2.1/NOTICE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:27:11.328955 Navix-0.2.1/Navix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-06-19 21:27:11.000000 Navix-0.2.1/Navix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-19 21:27:11.000000 Navix-0.2.1/Navix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 21:27:11.000000 Navix-0.2.1/Navix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-19 21:27:11.000000 Navix-0.2.1/Navix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-19 21:27:11.000000 Navix-0.2.1/Navix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-06-19 21:27:11.332955 Navix-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-19 21:26:55.000000 Navix-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:27:11.328955 Navix-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-19 21:26:55.000000 Navix-0.2.1/docs/design_notes.md
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-19 21:26:55.000000 Navix-0.2.1/docs/profiling.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:27:11.332955 Navix-0.2.1/navix/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-19 21:26:55.000000 Navix-0.2.1/navix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-06-19 21:26:55.000000 Navix-0.2.1/navix/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-19 21:26:55.000000 Navix-0.2.1/navix/components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:27:11.332955 Navix-0.2.1/navix/environments/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-19 21:26:55.000000 Navix-0.2.1/navix/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-19 21:26:55.000000 Navix-0.2.1/navix/environments/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-19 21:26:55.000000 Navix-0.2.1/navix/environments/keydoor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-19 21:26:55.000000 Navix-0.2.1/navix/environments/room.py
--rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-06-19 21:26:55.000000 Navix-0.2.1/navix/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-06-19 21:26:55.000000 Navix-0.2.1/navix/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-06-19 21:26:55.000000 Navix-0.2.1/navix/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-06-19 21:26:55.000000 Navix-0.2.1/navix/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-19 21:26:55.000000 Navix-0.2.1/navix/terminations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-19 21:26:55.000000 Navix-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-19 21:26:55.000000 Navix-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 21:27:11.332955 Navix-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:27:11.332955 Navix-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-19 21:26:55.000000 Navix-0.2.1/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-19 21:26:55.000000 Navix-0.2.1/tests/test_environments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-19 21:26:55.000000 Navix-0.2.1/tests/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-19 21:26:55.000000 Navix-0.2.1/tests/test_observations.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-19 21:26:55.000000 Navix-0.2.1/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-19 21:26:55.000000 Navix-0.2.1/tests/test_terminations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:54:26.787100 Navix-0.3.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:54:26.779101 Navix-0.3.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:54:26.783100 Navix-0.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-01 07:54:16.000000 Navix-0.3.5/.github/workflows/CD.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-01 07:54:16.000000 Navix-0.3.5/.github/workflows/CI.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-01 07:54:16.000000 Navix-0.3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-01 07:54:16.000000 Navix-0.3.5/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-01 07:54:16.000000 Navix-0.3.5/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-07-01 07:54:16.000000 Navix-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-01 07:54:16.000000 Navix-0.3.5/NOTICE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:54:26.783100 Navix-0.3.5/Navix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18431 2023-07-01 07:54:26.000000 Navix-0.3.5/Navix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-01 07:54:26.000000 Navix-0.3.5/Navix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 07:54:26.000000 Navix-0.3.5/Navix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-01 07:54:26.000000 Navix-0.3.5/Navix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-01 07:54:26.000000 Navix-0.3.5/Navix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18431 2023-07-01 07:54:26.783100 Navix-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-01 07:54:16.000000 Navix-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:54:26.783100 Navix-0.3.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-01 07:54:16.000000 Navix-0.3.5/docs/design_notes.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-01 07:54:16.000000 Navix-0.3.5/docs/performance.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:54:26.783100 Navix-0.3.5/navix/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-01 07:54:16.000000 Navix-0.3.5/navix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-01 07:54:16.000000 Navix-0.3.5/navix/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-07-01 07:54:16.000000 Navix-0.3.5/navix/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-01 07:54:16.000000 Navix-0.3.5/navix/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-07-01 07:54:16.000000 Navix-0.3.5/navix/entities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:54:26.783100 Navix-0.3.5/navix/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-01 07:54:16.000000 Navix-0.3.5/navix/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-01 07:54:16.000000 Navix-0.3.5/navix/environments/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-01 07:54:16.000000 Navix-0.3.5/navix/environments/keydoor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-01 07:54:16.000000 Navix-0.3.5/navix/environments/room.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-07-01 07:54:16.000000 Navix-0.3.5/navix/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-07-01 07:54:16.000000 Navix-0.3.5/navix/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-07-01 07:54:16.000000 Navix-0.3.5/navix/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-01 07:54:16.000000 Navix-0.3.5/navix/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-01 07:54:16.000000 Navix-0.3.5/navix/terminations.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-01 07:54:17.000000 Navix-0.3.5/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-01 07:54:16.000000 Navix-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-01 07:54:16.000000 Navix-0.3.5/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:54:26.783100 Navix-0.3.5/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      808 2023-07-01 07:54:16.000000 Navix-0.3.5/scripts/release.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 07:54:26.787100 Navix-0.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:54:26.783100 Navix-0.3.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:54:26.783100 Navix-0.3.5/tests/performance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-01 07:54:16.000000 Navix-0.3.5/tests/performance/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-01 07:54:16.000000 Navix-0.3.5/tests/performance/minigrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-01 07:54:16.000000 Navix-0.3.5/tests/performance/minigrid_report.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-01 07:54:16.000000 Navix-0.3.5/tests/performance/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-01 07:54:16.000000 Navix-0.3.5/tests/performance/observations_keydoor_report.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-01 07:54:16.000000 Navix-0.3.5/tests/performance/observations_room_report.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-01 07:54:16.000000 Navix-0.3.5/tests/performance/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-07-01 07:54:16.000000 Navix-0.3.5/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-01 07:54:16.000000 Navix-0.3.5/tests/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-01 07:54:16.000000 Navix-0.3.5/tests/test_environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-01 07:54:16.000000 Navix-0.3.5/tests/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-01 07:54:16.000000 Navix-0.3.5/tests/test_observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-01 07:54:16.000000 Navix-0.3.5/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-01 07:54:16.000000 Navix-0.3.5/tests/test_terminations.py
```

### Comparing `Navix-0.2.1/.github/workflows/CI.yml` & `Navix-0.3.5/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `Navix-0.2.1/.gitignore` & `Navix-0.3.5/.gitignore`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # setuptools_scm
 helx/version.py
 
+# developing
+playground.ipynb
+
 # vscode
 .vscode/
 wandb/
 .DS_Store
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
```

### Comparing `Navix-0.2.1/COPYRIGHT` & `Navix-0.3.5/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `Navix-0.2.1/LICENSE` & `Navix-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Navix-0.2.1/Navix.egg-info/PKG-INFO` & `Navix-0.3.5/Navix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Navix
-Version: 0.2.1
+Version: 0.3.5
 Summary: Accelerated gridworld navigation with JAX for deep reinforcement learning
 Author-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 Maintainer-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -250,34 +250,43 @@
 [![CI](https://github.com/epignatelli/navix/actions/workflows/CI.yml/badge.svg)](https://github.com/epignatelli/navix/actions/workflows/CI.yml)
 [![CD](https://github.com/epignatelli/navix/actions/workflows/CD.yml/badge.svg)](https://github.com/epignatelli/navix/actions/workflows/CD.yml)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/epignatelli/navix?color=%23216477&label=Release)
 
 **[Quickstart](#what-is-navix)** | **[Installation](#installation)** | **[Examples](#examples)** | **[Cite](#cite)**
 
 ## What is NAVIX?
-NAVIX is [minigrid](https://github.com/Farama-Foundation/Minigrid) in JAX, **>10000x** faster with Autograd and XLA support.
+NAVIX is [minigrid](https://github.com/Farama-Foundation/Minigrid) in JAX, **>1000x** faster with Autograd and XLA support.
 You can see a superficial performance comparison [here](docs/profiling.ipynb).
 
+The library is in active development, and we are working on adding more environments and features.
+If you want join the development and contribute, please [open a discussion](https://github.com/epignatelli/navix/discussions/new?category=general) and let's have a chat!
+
 
 ## Installation
 We currently support the OSs supported by JAX.
 You can find a description [here](https://github.com/google/jax#installation).
 
 You might want to follow the same guide to install jax for your faviourite accelerator
 (e.g. [CPU](https://github.com/google/jax#pip-installation-cpu),
 [GPU](https://github.com/google/jax#pip-installation-gpu-cuda-installed-locally-harder), or
 [TPU](https://github.com/google/jax#pip-installation-colab-tpu)
 ).
 
-Then, install `navix` and its dependencies with:
+- ### Stable
+Then, install the stable version of `navix` and its dependencies with:
 ```bash
 pip install navix
 ```
 
----
+- ### Nightly
+Or, if you prefer to install the latest version from source:
+```bash
+pip install git+https://github.com/epignatelli/navix
+```
+
 ## Examples
 
 ### XLA compilation
 One straightforward use case is to accelerate the computation of the environment with XLA compilation.
 For example, here we vectorise the environment to run multiple environments in parallel, and compile **the full training run**.
 
 You can find a partial performance comparison with [minigrid](https://github.com/Farama-Foundation/Minigrid) in the [docs](docs/profiling.ipynb).
@@ -317,8 +326,7 @@
   author = {Pignatelli, Eduardo},
   title = {Navix: Accelerated gridworld navigation with JAX},
   year = {2023},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/epignatelli/navix}}
   }
-```
```

### Comparing `Navix-0.2.1/PKG-INFO` & `Navix-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Navix
-Version: 0.2.1
+Version: 0.3.5
 Summary: Accelerated gridworld navigation with JAX for deep reinforcement learning
 Author-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 Maintainer-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -250,34 +250,43 @@
 [![CI](https://github.com/epignatelli/navix/actions/workflows/CI.yml/badge.svg)](https://github.com/epignatelli/navix/actions/workflows/CI.yml)
 [![CD](https://github.com/epignatelli/navix/actions/workflows/CD.yml/badge.svg)](https://github.com/epignatelli/navix/actions/workflows/CD.yml)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/epignatelli/navix?color=%23216477&label=Release)
 
 **[Quickstart](#what-is-navix)** | **[Installation](#installation)** | **[Examples](#examples)** | **[Cite](#cite)**
 
 ## What is NAVIX?
-NAVIX is [minigrid](https://github.com/Farama-Foundation/Minigrid) in JAX, **>10000x** faster with Autograd and XLA support.
+NAVIX is [minigrid](https://github.com/Farama-Foundation/Minigrid) in JAX, **>1000x** faster with Autograd and XLA support.
 You can see a superficial performance comparison [here](docs/profiling.ipynb).
 
+The library is in active development, and we are working on adding more environments and features.
+If you want join the development and contribute, please [open a discussion](https://github.com/epignatelli/navix/discussions/new?category=general) and let's have a chat!
+
 
 ## Installation
 We currently support the OSs supported by JAX.
 You can find a description [here](https://github.com/google/jax#installation).
 
 You might want to follow the same guide to install jax for your faviourite accelerator
 (e.g. [CPU](https://github.com/google/jax#pip-installation-cpu),
 [GPU](https://github.com/google/jax#pip-installation-gpu-cuda-installed-locally-harder), or
 [TPU](https://github.com/google/jax#pip-installation-colab-tpu)
 ).
 
-Then, install `navix` and its dependencies with:
+- ### Stable
+Then, install the stable version of `navix` and its dependencies with:
 ```bash
 pip install navix
 ```
 
----
+- ### Nightly
+Or, if you prefer to install the latest version from source:
+```bash
+pip install git+https://github.com/epignatelli/navix
+```
+
 ## Examples
 
 ### XLA compilation
 One straightforward use case is to accelerate the computation of the environment with XLA compilation.
 For example, here we vectorise the environment to run multiple environments in parallel, and compile **the full training run**.
 
 You can find a partial performance comparison with [minigrid](https://github.com/Farama-Foundation/Minigrid) in the [docs](docs/profiling.ipynb).
@@ -317,8 +326,7 @@
   author = {Pignatelli, Eduardo},
   title = {Navix: Accelerated gridworld navigation with JAX},
   year = {2023},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/epignatelli/navix}}
   }
-```
```

### Comparing `Navix-0.2.1/README.md` & `Navix-0.3.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,34 +4,43 @@
 [![CI](https://github.com/epignatelli/navix/actions/workflows/CI.yml/badge.svg)](https://github.com/epignatelli/navix/actions/workflows/CI.yml)
 [![CD](https://github.com/epignatelli/navix/actions/workflows/CD.yml/badge.svg)](https://github.com/epignatelli/navix/actions/workflows/CD.yml)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/epignatelli/navix?color=%23216477&label=Release)
 
 **[Quickstart](#what-is-navix)** | **[Installation](#installation)** | **[Examples](#examples)** | **[Cite](#cite)**
 
 ## What is NAVIX?
-NAVIX is [minigrid](https://github.com/Farama-Foundation/Minigrid) in JAX, **>10000x** faster with Autograd and XLA support.
+NAVIX is [minigrid](https://github.com/Farama-Foundation/Minigrid) in JAX, **>1000x** faster with Autograd and XLA support.
 You can see a superficial performance comparison [here](docs/profiling.ipynb).
 
+The library is in active development, and we are working on adding more environments and features.
+If you want join the development and contribute, please [open a discussion](https://github.com/epignatelli/navix/discussions/new?category=general) and let's have a chat!
+
 
 ## Installation
 We currently support the OSs supported by JAX.
 You can find a description [here](https://github.com/google/jax#installation).
 
 You might want to follow the same guide to install jax for your faviourite accelerator
 (e.g. [CPU](https://github.com/google/jax#pip-installation-cpu),
 [GPU](https://github.com/google/jax#pip-installation-gpu-cuda-installed-locally-harder), or
 [TPU](https://github.com/google/jax#pip-installation-colab-tpu)
 ).
 
-Then, install `navix` and its dependencies with:
+- ### Stable
+Then, install the stable version of `navix` and its dependencies with:
 ```bash
 pip install navix
 ```
 
----
+- ### Nightly
+Or, if you prefer to install the latest version from source:
+```bash
+pip install git+https://github.com/epignatelli/navix
+```
+
 ## Examples
 
 ### XLA compilation
 One straightforward use case is to accelerate the computation of the environment with XLA compilation.
 For example, here we vectorise the environment to run multiple environments in parallel, and compile **the full training run**.
 
 You can find a partial performance comparison with [minigrid](https://github.com/Farama-Foundation/Minigrid) in the [docs](docs/profiling.ipynb).
@@ -71,8 +80,7 @@
   author = {Pignatelli, Eduardo},
   title = {Navix: Accelerated gridworld navigation with JAX},
   year = {2023},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/epignatelli/navix}}
   }
-```
```

### Comparing `Navix-0.2.1/docs/design_notes.md` & `Navix-0.3.5/docs/design_notes.md`

 * *Files identical despite different names*

### Comparing `Navix-0.2.1/navix/__init__.py` & `Navix-0.3.5/navix/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,21 +14,18 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 
-__version__ = "0.2.1"
-__version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
-
-
 from . import (
     actions,
     components,
+    entities,
     graphics,
     grid,
     observations,
     tasks,
     environments,
     terminations,
 )
```

### Comparing `Navix-0.2.1/navix/actions.py` & `Navix-0.3.5/navix/actions.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,47 +16,53 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from __future__ import annotations
 from typing import Tuple
 
-import chex
 import jax
 import jax.numpy as jnp
 from jax import Array
 
-from .components import Consumable, Pickable, State
+from .entities import Door, Key, State
+from .components import DISCARD_PILE_COORDS
+from .grid import translate, rotate, positions_equal
 
 
 DIRECTIONS = {0: "east", 1: "south", 2: "west", 3: "north"}
 
 
 def _rotate(state: State, spin: int) -> State:
-    direction = (state.player.direction + spin) % 4
-    player = state.player.replace(direction=direction)
-    return state.replace(player=player)
-
-
-def _translate(position: Array, direction: Array) -> Array:
-    moves = (
-        lambda position: position + jnp.asarray((0, 1)),  # east
-        lambda position: position + jnp.asarray((1, 0)),  # south
-        lambda position: position + jnp.asarray((0, -1)),  # west
-        lambda position: position + jnp.asarray((-1, 0)),  # north
-    )
-    return jax.lax.switch(direction, moves, position)
+    direction = rotate(state.players.direction, spin)
+    player = state.players.replace(direction=direction)
+    return state.replace(players=player)
+
+
+def _walkable(state: State, position: Array) -> Array:
+    # according to the grid
+    walkable = jnp.equal(state.grid[tuple(position)], 0)
+
+    # and not occupied by another non-walkable entity
+    occupied_keys = positions_equal(position, state.keys.position)
+    # occupied by a door, and door is not open
+    occupied_doors = positions_equal(position, state.doors.position)
+    occupied_doors = occupied_doors & ~state.doors.open
+
+    occupied = jnp.any(jnp.logical_or(occupied_keys, occupied_doors))
+    # return: if walkable and not occupied
+    return jnp.logical_and(walkable, jnp.logical_not(occupied))
 
 
 def _move(state: State, direction: Array) -> State:
-    new_position = _translate(state.player.position, direction)
-    can_move = jnp.equal(state.grid[tuple(state.player.position)], 0)
-    new_position = jnp.where(can_move, new_position, state.player.position)
-    player = state.player.replace(position=new_position)
-    return state.replace(player=player)
+    new_position = translate(state.players.position, direction)
+    can_move = _walkable(state, new_position)
+    new_position = jnp.where(can_move, new_position, state.players.position)
+    player = state.players.replace(position=new_position)
+    return state.replace(players=player)
 
 
 def undefined(state: State) -> State:
     # this is problematic because jax.lax.switch evaluates
     # all *python* branches (no XLA computation is performed)
     # even though only one is selected
     # one option is the following, but this breaks type checking
@@ -75,69 +81,68 @@
 
 
 def rotate_ccw(state: State) -> State:
     return _rotate(state, -1)
 
 
 def forward(state: State) -> State:
-    return _move(state, state.player.direction)
+    return _move(state, state.players.direction)
 
 
 def right(state: State) -> State:
-    return _move(state, state.player.direction + 1)
+    return _move(state, state.players.direction + 1)
 
 
 def backward(state: State) -> State:
-    return _move(state, state.player.direction + 2)
+    return _move(state, state.players.direction + 2)
 
 
 def left(state: State) -> State:
-    return _move(state, state.player.direction + 3)
+    return _move(state, state.players.direction + 3)
 
 
 def pickup(state: State) -> State:
-    position_in_front = _translate(state.player.position, state.player.direction)
+    position_in_front = translate(state.players.position, state.players.direction)
+
+    key_found = positions_equal(position_in_front, state.keys.position)
+
+    # update keys
+    positions = jnp.where(key_found, DISCARD_PILE_COORDS, state.keys.position)
+    keys = state.keys.replace(position=positions)
+
+    # update player's pocket, if the pocket has something else, we overwrite it
+    key = jnp.sum(state.keys.id * key_found, dtype=jnp.int32)
+    player = jax.lax.cond(jnp.any(key_found), lambda: state.players.replace(pocket=key), lambda: state.players)
 
-    def _update(key: Pickable) -> Tuple[Array, Pickable]:
-        match = jnp.array_equal(position_in_front, key.position)
-        # update player's pocket
-        pocket = jnp.where(match, key.id, state.player.pocket)
-        # set to (-1, -1) the position of the key that was picked up
-        unset_position = jnp.asarray((-1, -1))
-        position = jnp.where(match, unset_position, key.position)
-        key = key.replace(position=position)
-        return pocket, key
-
-    pockets, keys = jax.vmap(_update)(state.keys)
-    pocket = jnp.max(pockets, axis=0)
-    player = state.player.replace(pocket=pocket)
-    return state.replace(player=player, keys=keys)
+    return state.replace(players=player, keys=keys)
 
 
 def open(state: State) -> State:
-    position_in_front = _translate(state.player.position, state.player.direction)
+    """Unlocks and opens an openable object (like a door) if possible"""
+    # get the tile in front of the player
+    position_in_front = translate(state.players.position, state.players.direction)
+
+    # check if there is a door in front of the player
+    door_found = positions_equal(position_in_front, state.doors.position)
+
+    # and that, if so, either it does not require a key or the player has the key
+    requires_key = state.doors.requires != -1
+    key_match = state.players.pocket == state.doors.requires
+    can_open = door_found & (key_match | ~requires_key )
+
+    # update doors if closed and can_open
+    do_open = (~state.doors.open & can_open)
+    open = jnp.where(do_open, True, state.doors.open)
+    doors = state.doors.replace(open=open)
+
+    # remove key from player's pocket
+    pocket = jnp.asarray(state.players.pocket * jnp.any(can_open), dtype=jnp.int32)
+    player = jax.lax.cond(jnp.any(can_open), lambda: state.players.replace(pocket=pocket), lambda: state.players)
 
-    def _update(door: Consumable) -> Tuple[Array, Consumable]:
-        match = jnp.array_equal(position_in_front, door.position)
-        replacement = jnp.asarray((match - 1) * door.replacement, dtype=jnp.int32)
-
-        # update grid
-        grid = jnp.zeros_like(state.grid).at[tuple(door.position)].set(replacement)
-
-        # set to (-1, -1) the position of the door that was opened
-        unset_position = jnp.asarray((-1, -1))
-        position = jnp.where(match, unset_position, door.position)
-        door = door.replace(position=position)
-        return grid, door
-
-    grid, doors = jax.vmap(_update)(state.doors)
-    # the max makes sure that if there was a wall (-1), and it has been opened (x>0)
-    # we get the new value of the grid
-    grid = jnp.max(grid, axis=0)
-    return state.replace(grid=grid, doors=doors)
+    return state.replace(players=player, doors=doors)
 
 
 # TODO(epignatelli): a mutable dictionary here is dangerous
 ACTIONS = {
     # -1: undefined,
     0: noop,
     1: rotate_cw,
```

### Comparing `Navix-0.2.1/navix/environments/__init__.py` & `Navix-0.3.5/navix/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `Navix-0.2.1/navix/environments/environment.py` & `Navix-0.3.5/navix/environments/environment.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,19 +25,18 @@
 from typing import Any, Callable, Dict
 import jax
 import jax.numpy as jnp
 from jax.random import KeyArray
 from jax import Array
 from flax import struct
 
-from .. import tasks
-from ..components import State
-from .. import terminations
+
+from .. import tasks, terminations, observations
+from ..entities import State
 from ..actions import ACTIONS
-from .. import observations
 
 
 class StepType(IntEnum):
     TRANSITION = 0
     """discount > 0, episode continues"""
     TRUNCATION = 1
     """discount > 0, episode ends"""
@@ -64,15 +63,15 @@
 
 class Environment(struct.PyTreeNode):
     height: int = struct.field(pytree_node=False)
     width: int = struct.field(pytree_node=False)
     max_steps: int = struct.field(pytree_node=False)
     gamma: float = struct.field(pytree_node=False, default=1.0)
     observation_fn: Callable[[State], Array] = struct.field(
-        pytree_node=False, default=observations.categorical
+        pytree_node=False, default=observations.none
     )
     reward_fn: Callable[[State, Array, State], Array] = struct.field(
         pytree_node=False, default=tasks.navigation
     )
     termination_fn: Callable[[State, Array, State], Array] = struct.field(
         pytree_node=False, default=terminations.on_navigation_completion
     )
```

### Comparing `Navix-0.2.1/navix/environments/keydoor.py` & `Navix-0.3.5/navix/environments/keydoor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 import jax
 import jax.numpy as jnp
+from jax.random import KeyArray
 
-from navix.environments import Environment
-from navix.components import State, Player, Pickable, Consumable, Goal
-from navix.environments import Timestep
-from navix.grid import two_rooms, random_positions, random_directions, mask_by_coordinates
+from ..graphics import RenderingCache
+from ..environments import Environment
+from ..entities import State, Player, Key, Door, Goal
+from ..environments import Timestep
+from ..grid import (
+    two_rooms,
+    random_positions,
+    random_directions,
+    mask_by_coordinates,
+)
 
 
 class KeyDoor(Environment):
-    def reset(self, key) -> Timestep:
+    def reset(self, key: KeyArray) -> Timestep:
         key, k1, k2, k3, k4 = jax.random.split(key, 5)
 
         grid, wall_at = two_rooms(height=self.height, width=self.width, key=k4)
 
+        # add the door
+        door_pos = jnp.asarray([jax.random.randint(k3, (), 1, self.height - 1), wall_at])
+        doors = Door.create(position=door_pos, requires=jnp.asarray(3))
+
         # spawn player and key in the first room
         out_of_bounds = jnp.asarray(self.height)
         first_room_mask = mask_by_coordinates(grid, (out_of_bounds, wall_at), jnp.less)
         first_room = jnp.where(first_room_mask, grid, -1)
-
         # player
         player_pos = random_positions(k1, first_room)
         player_dir = random_directions(k2)
-        player = Player(position=player_pos, direction=player_dir)
-
+        player = Player.create(position=player_pos, direction=player_dir)
         # key
-        key_pos = random_positions(k2, first_room, exclude=player_pos[None])
-        keys = Pickable(position=key_pos[None], id=jnp.asarray(3)[None])
+        key_pos = random_positions(k2, first_room, exclude=player_pos)
+        keys = Key.create(position=key_pos, id=jnp.asarray(3))
 
         # spawn the goal in the second room
         second_room = jnp.where(first_room_mask, -1, grid)
-        goal_pos = random_positions(k2, second_room, exclude=jnp.stack([player_pos, key_pos]))
-        goals = Goal(position=goal_pos[None])
+        goal_pos = random_positions(k2, second_room)
+        goals = Goal.create(position=goal_pos, probability=jnp.asarray(1.0))
 
-        # add the door
-        door_coordinates = jnp.asarray(
-            [
-                jax.random.randint(k3, (), 1, self.height - 1),
-                wall_at,
-            ]
-        )
-        doors = Consumable(
-            position=door_coordinates[None], requires=jnp.asarray(3)[None]
-        )
+        # remove the wall beneath the door
+        grid = grid.at[tuple(door_pos)].set(0)
 
         state = State(
             key=key,
             grid=grid,
-            player=player,
+            players=player,
             goals=goals,
             keys=keys,
             doors=doors,
+            cache=RenderingCache.init(grid),
         )
         return Timestep(
             t=jnp.asarray(0, dtype=jnp.int32),
             observation=self.observation(state),
             action=jnp.asarray(-1, dtype=jnp.int32),
             reward=jnp.asarray(0.0, dtype=jnp.float32),
             step_type=jnp.asarray(0, dtype=jnp.int32),
```

### Comparing `Navix-0.2.1/navix/environments/room.py` & `Navix-0.3.5/navix/environments/room.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,42 +15,52 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 
 from __future__ import annotations
+from typing import Callable
 
 import jax
 import jax.numpy as jnp
 from jax.random import KeyArray
 
-from ..components import Goal, Player, State
+
+from ..entities import Goal, Player, State
 from ..grid import random_positions, random_directions, room
+from ..graphics import RenderingCache
 from .environment import Environment, Timestep
 
 
 class Room(Environment):
     def reset(self, key: KeyArray) -> Timestep:
         key, k1, k2 = jax.random.split(key, 3)
 
         # map
         grid = room(height=self.height, width=self.width)
-        positions = random_positions(k1, grid, n=2)
-        direction = random_directions(k2, n=1)
+        # TODO(epignatelli): if rendering gets slower, we can always
+        # split `reset`` into `init` and `reset`, start the cache in `init`
+        # and change it only when necessary in `reset`
+        # e.g., Room doesn't need to change the cache
+        # at every reset (and so many others) but KeyDoor does
+
         # player
-        player = Player(position=positions[0], direction=direction)
+        player_pos, goal_pos = random_positions(k1, grid, n=2)
+        direction = random_directions(k2, n=1)
+        player = Player.create(position=player_pos, direction=direction)
         # goal
-        goal = Goal(position=positions[1][None])
+        goal = Goal.create(position=goal_pos, probability=jnp.asarray(1.0))
 
         # systems
         state = State(
             key=key,
             grid=grid,
-            player=player,
+            cache=RenderingCache.init(grid),
+            players=player,
             goals=goal,
         )
 
         return Timestep(
             t=jnp.asarray(0, dtype=jnp.int32),
             observation=self.observation(state),
             action=jnp.asarray(0, dtype=jnp.int32),
```

### Comparing `Navix-0.2.1/navix/tasks.py` & `Navix-0.3.5/navix/tasks.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from typing import Callable
 
 
 import jax
 import jax.numpy as jnp
 from jax import Array
 
-from .components import State
+from .entities import State
 
 
 def compose(*fns: Callable[[State, Array, State], Array]):
     def composed(prev_state: State, action: Array, state: State) -> Array:
         reward = jnp.asarray(0.0)
         for fn in fns:
             reward += fn(prev_state, action, state)
@@ -41,15 +41,15 @@
 
 def free(state: State) -> Array:
     return jnp.asarray(0.0)
 
 
 def navigation(prev_state: State, action: Array, state: State) -> Array:
     reached = jax.vmap(jnp.array_equal, in_axes=(None, 0))(
-        state.player.position, state.goals.position
+        state.players.position, state.goals.position
     )
     any_reached = jnp.sum(reached)
 
     draw = jax.random.uniform(state.key, ())
     reward = any_reached * jnp.greater_equal(draw, state.goals.probability)
     reward = jnp.asarray(reward, jnp.float32).squeeze()
 
@@ -72,11 +72,11 @@
     return -jnp.asarray(cost)
 
 
 def wall_hit_cost(
     prev_state: State, action: Array, state: State, cost: float = 0.01
 ) -> Array:
     # if state is unchanged, maybe the wall was hit
-    didnt_move = jnp.array_equal(prev_state.player.position, state.player.position)
+    didnt_move = jnp.array_equal(prev_state.players.position, state.players.position)
     but_wanted_to = jnp.less_equal(3, action) * jnp.less_equal(action, 6)
     hit = jnp.logical_and(didnt_move, but_wanted_to)
     return -jnp.asarray(cost) * hit
```

### Comparing `Navix-0.2.1/navix/terminations.py` & `Navix-0.3.5/navix/terminations.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 
 
 from __future__ import annotations
 
 from jax import Array
 import jax
 import jax.numpy as jnp
-from .components import State
+from .entities import State
+from .grid import positions_equal
 
 
 def check_truncation(terminated: Array, truncated: Array) -> Array:
-    return jnp.asarray(truncated + 2 * terminated, dtype=jnp.int32)
+    result = jnp.asarray(truncated + 2 * terminated, dtype=jnp.int32)
+    return jnp.clip(result, 0, 2)
 
 
 def on_navigation_completion(prev_state: State, action: Array, state: State) -> Array:
-    reached = jax.vmap(jnp.array_equal, in_axes=(None, 0))(
-        state.player.position, state.goals.position
-    )
+    reached = positions_equal(state.players.position, state.goals.position)
     return jnp.any(reached)
```

### Comparing `Navix-0.2.1/pyproject.toml` & `Navix-0.3.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -54,23 +54,22 @@
 [project.urls]
 homepage = "https://github.com/epignatelli/navix"
 repository = "https://github.com/epignatelli/navix"
 bug_tracker = "https://github.com/epignatelli/navix/issues"
 
 
 [tool.setuptools.dynamic]
-version = {attr = "navix.__version__"}
+version = {attr = "navix._version.__version__"}
 dependencies = {file = "./requirements.txt"}
 
 
 [tool.setuptools.packages.find]
 include = ["navix*"]
-exclude = ["test", "examples"]
+exclude = ["tests", "examples", "scripts", "docs"]
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
-
 [tool.black]
 line-length = 88
```

### Comparing `Navix-0.2.1/tests/test_environments.py` & `Navix-0.3.5/tests/test_environments.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def test_room():
     def f():
         env = nx.environments.Room(height=3, width=3, max_steps=8)
         key = jax.random.PRNGKey(4)
         reset = jax.jit(env.reset)
         step = jax.jit(env.step)
         timestep = reset(key)
-        # these are optimal actions for navigation + action_cost
+        # these are optimal actios for navigation + action_cost
         actions = (
             0,  # noop sanity check
             2,  # rotate_ccw
             3,  # forward
             3,  # forward
             2,  # rotate_ccw
             3,  # forward
@@ -69,8 +69,8 @@
 
     f()
     jax.jit(f)()
 
 
 if __name__ == "__main__":
     test_room()
-    # test_keydoor()
+    test_keydoor()
```

### Comparing `Navix-0.2.1/tests/test_tasks.py` & `Navix-0.3.5/tests/test_tasks.py`

 * *Files identical despite different names*

