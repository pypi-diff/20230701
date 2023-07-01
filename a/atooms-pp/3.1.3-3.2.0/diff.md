# Comparing `tmp/atooms-pp-3.1.3.tar.gz` & `tmp/atooms-pp-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atooms-pp-3.1.3.tar", last modified: Sat Mar 11 08:28:58 2023, max compression
+gzip compressed data, was "atooms-pp-3.2.0.tar", last modified: Sat Jul  1 07:37:40 2023, max compression
```

## Comparing `atooms-pp-3.1.3.tar` & `atooms-pp-3.2.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-03-11 08:28:58.735547 atooms-pp-3.1.3/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     5485 2023-03-11 08:28:58.735547 atooms-pp-3.1.3/PKG-INFO
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     3967 2022-02-15 14:06:29.000000 atooms-pp-3.1.3/README.md
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-03-11 08:28:58.715547 atooms-pp-3.1.3/atooms/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      159 2019-07-25 13:44:35.000000 atooms-pp-3.1.3/atooms/__init__.py
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-03-11 08:28:58.731547 atooms-pp-3.1.3/atooms/postprocessing/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      662 2022-04-05 17:07:33.000000 atooms-pp-3.1.3/atooms/postprocessing/__init__.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)       55 2023-03-10 16:43:58.000000 atooms-pp-3.1.3/atooms/postprocessing/_commit.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)       22 2023-03-11 08:28:56.000000 atooms-pp-3.1.3/atooms/postprocessing/_version.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1571 2022-04-05 17:07:33.000000 atooms-pp-3.1.3/atooms/postprocessing/alpha2.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    15572 2022-10-13 10:18:27.000000 atooms-pp-3.1.3/atooms/postprocessing/api.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     4538 2022-06-01 11:14:00.000000 atooms-pp-3.1.3/atooms/postprocessing/ba.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     4528 2022-05-25 15:04:19.000000 atooms-pp-3.1.3/atooms/postprocessing/chi4t.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1984 2022-04-05 17:07:33.000000 atooms-pp-3.1.3/atooms/postprocessing/core.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    25392 2023-02-23 17:01:00.000000 atooms-pp-3.1.3/atooms/postprocessing/correlation.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2138 2022-04-05 17:07:33.000000 atooms-pp-3.1.3/atooms/postprocessing/filter.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    16940 2023-01-11 10:39:54.000000 atooms-pp-3.1.3/atooms/postprocessing/fkt.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2809 2022-05-25 15:04:19.000000 atooms-pp-3.1.3/atooms/postprocessing/fourierspace.f90
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    13938 2022-12-21 14:16:35.000000 atooms-pp-3.1.3/atooms/postprocessing/fourierspace.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    14103 2022-12-19 15:12:39.000000 atooms-pp-3.1.3/atooms/postprocessing/gr.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     8521 2023-03-10 21:48:33.000000 atooms-pp-3.1.3/atooms/postprocessing/helpers.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2922 2022-10-13 10:49:58.000000 atooms-pp-3.1.3/atooms/postprocessing/ik.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    10533 2023-02-25 08:24:45.000000 atooms-pp-3.1.3/atooms/postprocessing/linkedcells.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     3755 2022-04-05 17:07:33.000000 atooms-pp-3.1.3/atooms/postprocessing/msd.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     3906 2022-12-17 22:45:31.000000 atooms-pp-3.1.3/atooms/postprocessing/partial.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1750 2022-04-05 17:07:33.000000 atooms-pp-3.1.3/atooms/postprocessing/progress.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     3034 2022-04-05 17:07:33.000000 atooms-pp-3.1.3/atooms/postprocessing/qt.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    27450 2022-12-16 22:45:23.000000 atooms-pp-3.1.3/atooms/postprocessing/realspace.f90
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     4201 2023-03-10 21:56:15.000000 atooms-pp-3.1.3/atooms/postprocessing/s4kt.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1767 2022-04-05 17:07:33.000000 atooms-pp-3.1.3/atooms/postprocessing/sacf.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     9867 2022-10-13 10:49:58.000000 atooms-pp-3.1.3/atooms/postprocessing/sk.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1603 2022-04-05 17:07:33.000000 atooms-pp-3.1.3/atooms/postprocessing/susceptibility.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1254 2022-04-05 17:07:33.000000 atooms-pp-3.1.3/atooms/postprocessing/vacf.py
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-03-11 08:28:58.735547 atooms-pp-3.1.3/atooms_pp.egg-info/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     5485 2023-03-11 08:28:58.000000 atooms-pp-3.1.3/atooms_pp.egg-info/PKG-INFO
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1102 2023-03-11 08:28:58.000000 atooms-pp-3.1.3/atooms_pp.egg-info/SOURCES.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)        1 2023-03-11 08:28:58.000000 atooms-pp-3.1.3/atooms_pp.egg-info/dependency_links.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)       26 2023-03-11 08:28:58.000000 atooms-pp-3.1.3/atooms_pp.egg-info/requires.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)       29 2023-03-11 08:28:58.000000 atooms-pp-3.1.3/atooms_pp.egg-info/top_level.txt
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-03-11 08:28:58.735547 atooms-pp-3.1.3/bin/
--rwxrwxr-x   0 coslo     (1000) coslo     (1000)      797 2019-07-25 13:44:35.000000 atooms-pp-3.1.3/bin/acf.py
--rwxrwxr-x   0 coslo     (1000) coslo     (1000)     3381 2020-11-04 22:11:46.000000 atooms-pp-3.1.3/bin/pp.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      173 2023-03-11 08:28:58.739547 atooms-pp-3.1.3/setup.cfg
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2137 2022-10-01 13:23:49.000000 atooms-pp-3.1.3/setup.py
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-07-01 07:37:40.484302 atooms-pp-3.2.0/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    35147 2021-11-14 11:19:34.000000 atooms-pp-3.2.0/LICENSE
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     4736 2023-07-01 07:37:40.484302 atooms-pp-3.2.0/PKG-INFO
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     3967 2022-02-15 14:06:29.000000 atooms-pp-3.2.0/README.md
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-07-01 07:37:40.472302 atooms-pp-3.2.0/atooms/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      159 2019-07-25 13:44:35.000000 atooms-pp-3.2.0/atooms/__init__.py
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-07-01 07:37:40.480302 atooms-pp-3.2.0/atooms/postprocessing/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      662 2022-04-05 17:07:33.000000 atooms-pp-3.2.0/atooms/postprocessing/__init__.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)       55 2023-03-10 16:43:58.000000 atooms-pp-3.2.0/atooms/postprocessing/_commit.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)       22 2023-07-01 07:37:38.000000 atooms-pp-3.2.0/atooms/postprocessing/_version.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1571 2022-04-05 17:07:33.000000 atooms-pp-3.2.0/atooms/postprocessing/alpha2.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    15572 2022-10-13 10:18:27.000000 atooms-pp-3.2.0/atooms/postprocessing/api.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     6005 2023-07-01 07:13:13.000000 atooms-pp-3.2.0/atooms/postprocessing/ba.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     4528 2022-05-25 15:04:19.000000 atooms-pp-3.2.0/atooms/postprocessing/chi4t.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1981 2023-04-15 13:28:02.000000 atooms-pp-3.2.0/atooms/postprocessing/core.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    25392 2023-02-23 17:01:00.000000 atooms-pp-3.2.0/atooms/postprocessing/correlation.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2138 2022-04-05 17:07:33.000000 atooms-pp-3.2.0/atooms/postprocessing/filter.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    16940 2023-04-15 13:28:01.000000 atooms-pp-3.2.0/atooms/postprocessing/fkt.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2809 2022-05-25 15:04:19.000000 atooms-pp-3.2.0/atooms/postprocessing/fourierspace.f90
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    13938 2023-04-15 13:28:00.000000 atooms-pp-3.2.0/atooms/postprocessing/fourierspace.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    13913 2023-06-30 17:00:38.000000 atooms-pp-3.2.0/atooms/postprocessing/gr.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     8521 2023-04-15 13:28:01.000000 atooms-pp-3.2.0/atooms/postprocessing/helpers.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2922 2022-10-13 10:49:58.000000 atooms-pp-3.2.0/atooms/postprocessing/ik.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    10533 2023-04-15 13:28:01.000000 atooms-pp-3.2.0/atooms/postprocessing/linkedcells.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     3755 2022-04-05 17:07:33.000000 atooms-pp-3.2.0/atooms/postprocessing/msd.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     3906 2023-04-15 13:28:00.000000 atooms-pp-3.2.0/atooms/postprocessing/partial.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1750 2022-04-05 17:07:33.000000 atooms-pp-3.2.0/atooms/postprocessing/progress.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     3034 2022-04-05 17:07:33.000000 atooms-pp-3.2.0/atooms/postprocessing/qt.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    27450 2023-04-15 13:28:00.000000 atooms-pp-3.2.0/atooms/postprocessing/realspace.f90
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     4201 2023-04-15 13:28:01.000000 atooms-pp-3.2.0/atooms/postprocessing/s4kt.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1767 2022-04-05 17:07:33.000000 atooms-pp-3.2.0/atooms/postprocessing/sacf.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     9867 2022-10-13 10:49:58.000000 atooms-pp-3.2.0/atooms/postprocessing/sk.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1603 2022-04-05 17:07:33.000000 atooms-pp-3.2.0/atooms/postprocessing/susceptibility.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1254 2022-04-05 17:07:33.000000 atooms-pp-3.2.0/atooms/postprocessing/vacf.py
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-07-01 07:37:40.484302 atooms-pp-3.2.0/atooms_pp.egg-info/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     4736 2023-07-01 07:37:40.000000 atooms-pp-3.2.0/atooms_pp.egg-info/PKG-INFO
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1110 2023-07-01 07:37:40.000000 atooms-pp-3.2.0/atooms_pp.egg-info/SOURCES.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)        1 2023-07-01 07:37:40.000000 atooms-pp-3.2.0/atooms_pp.egg-info/dependency_links.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)       26 2023-07-01 07:37:40.000000 atooms-pp-3.2.0/atooms_pp.egg-info/requires.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)       29 2023-07-01 07:37:40.000000 atooms-pp-3.2.0/atooms_pp.egg-info/top_level.txt
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2023-07-01 07:37:40.484302 atooms-pp-3.2.0/bin/
+-rwxrwxr-x   0 coslo     (1000) coslo     (1000)      797 2019-07-25 13:44:35.000000 atooms-pp-3.2.0/bin/acf.py
+-rwxrwxr-x   0 coslo     (1000) coslo     (1000)     3381 2020-11-04 22:11:46.000000 atooms-pp-3.2.0/bin/pp.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      173 2023-07-01 07:37:40.484302 atooms-pp-3.2.0/setup.cfg
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2137 2022-10-01 13:23:49.000000 atooms-pp-3.2.0/setup.py
```

### Comparing `atooms-pp-3.1.3/PKG-INFO` & `atooms-pp-3.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,114 +1,117 @@
 Metadata-Version: 2.1
 Name: atooms-pp
-Version: 3.1.3
+Version: 3.2.0
 Summary: Post-processing tools for particle simulations
 Home-page: https://framagit.org/atooms/postprocessing
 Author: Daniele Coslovich
 Author-email: daniele.coslovich@umontpellier.fr
 License: GPLv3
-Description: # Postprocessing
-        
-        [![pypi](https://img.shields.io/pypi/v/atooms-pp.svg)](https://pypi.python.org/pypi/atooms-pp/)
-        [![version](https://img.shields.io/pypi/pyversions/atooms-pp.svg)](https://pypi.python.org/pypi/atooms-pp/)
-        [![license](https://img.shields.io/pypi/l/atooms-pp.svg)](https://en.wikipedia.org/wiki/GNU_General_Public_License)
-        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/git/https%3A%2F%2Fframagit.org%2Fatooms%2Fpostprocessing/HEAD?labpath=docs%2Findex.ipynb)
-        [![pipeline](https://framagit.org/atooms/postprocessing/badges/master/pipeline.svg)](https://framagit.org/atooms/postprocessing/badges/master/pipeline.svg)
-        [![coverage report](https://framagit.org/atooms/postprocessing/badges/master/coverage.svg?job=test:f90)](https://framagit.org/atooms/postprocessing/-/commits/master)
-        
-        A Python package to compute static and dynamic correlation functions from simulations of interacting particles, such as molecular dynamics or Monte Carlo simulations. Based on [atooms](https://framagit.org/atooms/atooms).
-        
-        ## Quick start
-        
-        Postprocessing works on trajectories. Any trajectory format recognized by
-        [atooms](https://framagit.org/atooms/atooms.git) can be processed, for instance most "xyz" files
-        should work fine. If you use a custom trajectory format, it is easy to [add it](https://atooms.frama.io/atooms/).
-        
-        As an example, we compute the structure factor S(k) from the file `trajectory.xyz` in the `data/` folder.
-        
-        ### From the command line
-        
-        ```sh
-        pp.py --norigins 0.2 msd data/trajectory.xyz
-        ```
-        We just used 20% of the available time frames to compute the averages using the `--norigins` flag. Without it, `atooms-pp` applies an heuristics to determine the number of time frames required to achieve a reasonable data quality. The results of the calculation are stored in the file `data/trajectory.xyz.pp.sk`. 
-        
-        ### From Python
-        
-        The same calculation can be done from Python:
-        
-        ```python
-        from atooms.trajectory import Trajectory
-        import atooms.postprocessing as pp
-        
-        with Trajectory('data/trajectory.xyz') as t:
-             p = pp.StructureFactor(t)
-             p.do()
-        ```
-        
-        ## Features
-        
-        Available correlation and distribution functions
-        
-        - *Real space*
-          - radial distribution function
-          - mean square displacement
-          - velocity auto-correlation function
-          - self overlap functions
-          - collective overlap functions
-          - dynamic susceptibility of the self overlap function
-          - non-Gaussian parameter
-          - bond-angle distribution
-        - *Fourier space*
-          - structure factor
-          - spectral density
-          - self intermediate scattering functions
-          - collective intermediate scattering functions
-          - four-point dynamic susceptibility
-        
-        ## Documentation
-        
-        Check out the [tutorial](https://atooms.frama.io/postprocessing/tutorial) for more examples and the [public API](https://atooms.frama.io/postprocessing/api/postprocessing) for full details.
-        
-        Org-mode and jupyter notebooks are available under `docs/`. You can run the tutorial interactively on [Binder]( https://mybinder.org/v2/git/https%3A%2F%2Fframagit.org%2Fatooms%2Fpostprocessing/HEAD?labpath=docs%2Findex.ipynb).
-        
-        ## Requirements
-        
-        - [numpy](https://pypi.org/project/numpy/)
-        - [atooms](https://framagit.org/atooms/postprocessing.git)
-        - [optional] [argh](https://pypi.org/project/argh/) (only needed when using `pp.py`)
-        - [optional] [tqdm](https://pypi.org/project/tqdm/) (enable progress bars)
-        - [optional] [argcomplete](https://pypi.org/project/argcomplete/) (enable tab-completion for `pp.py`)
-        - [optional] fortran compiler for more efficient execution
-        
-        ## Installation
-        
-        Install with `pip`
-        ```
-        pip install atooms-pp
-        ```
-        
-        Or clone the project repository
-        ```
-        git clone https://framagit.org/atooms/postprocessing.git
-        cd postprocessing
-        make install
-        ```
-        
-        ## Contributing
-        
-        Contributions to the project are welcome. If you wish to contribute, check out [these guidelines](https://framagit.org/atooms/atooms/-/blob/master/CONTRIBUTING.md).
-        
-        ## Authors
-        
-        Daniele Coslovich: https://www.units.it/daniele.coslovich/
-        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Postprocessing
+
+[![pypi](https://img.shields.io/pypi/v/atooms-pp.svg)](https://pypi.python.org/pypi/atooms-pp/)
+[![version](https://img.shields.io/pypi/pyversions/atooms-pp.svg)](https://pypi.python.org/pypi/atooms-pp/)
+[![license](https://img.shields.io/pypi/l/atooms-pp.svg)](https://en.wikipedia.org/wiki/GNU_General_Public_License)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/git/https%3A%2F%2Fframagit.org%2Fatooms%2Fpostprocessing/HEAD?labpath=docs%2Findex.ipynb)
+[![pipeline](https://framagit.org/atooms/postprocessing/badges/master/pipeline.svg)](https://framagit.org/atooms/postprocessing/badges/master/pipeline.svg)
+[![coverage report](https://framagit.org/atooms/postprocessing/badges/master/coverage.svg?job=test:f90)](https://framagit.org/atooms/postprocessing/-/commits/master)
+
+A Python package to compute static and dynamic correlation functions from simulations of interacting particles, such as molecular dynamics or Monte Carlo simulations. Based on [atooms](https://framagit.org/atooms/atooms).
+
+## Quick start
+
+Postprocessing works on trajectories. Any trajectory format recognized by
+[atooms](https://framagit.org/atooms/atooms.git) can be processed, for instance most "xyz" files
+should work fine. If you use a custom trajectory format, it is easy to [add it](https://atooms.frama.io/atooms/).
+
+As an example, we compute the structure factor S(k) from the file `trajectory.xyz` in the `data/` folder.
+
+### From the command line
+
+```sh
+pp.py --norigins 0.2 msd data/trajectory.xyz
+```
+We just used 20% of the available time frames to compute the averages using the `--norigins` flag. Without it, `atooms-pp` applies an heuristics to determine the number of time frames required to achieve a reasonable data quality. The results of the calculation are stored in the file `data/trajectory.xyz.pp.sk`. 
+
+### From Python
+
+The same calculation can be done from Python:
+
+```python
+from atooms.trajectory import Trajectory
+import atooms.postprocessing as pp
+
+with Trajectory('data/trajectory.xyz') as t:
+     p = pp.StructureFactor(t)
+     p.do()
+```
+
+## Features
+
+Available correlation and distribution functions
+
+- *Real space*
+  - radial distribution function
+  - mean square displacement
+  - velocity auto-correlation function
+  - self overlap functions
+  - collective overlap functions
+  - dynamic susceptibility of the self overlap function
+  - non-Gaussian parameter
+  - bond-angle distribution
+- *Fourier space*
+  - structure factor
+  - spectral density
+  - self intermediate scattering functions
+  - collective intermediate scattering functions
+  - four-point dynamic susceptibility
+
+## Documentation
+
+Check out the [tutorial](https://atooms.frama.io/postprocessing/tutorial) for more examples and the [public API](https://atooms.frama.io/postprocessing/api/postprocessing) for full details.
+
+Org-mode and jupyter notebooks are available under `docs/`. You can run the tutorial interactively on [Binder]( https://mybinder.org/v2/git/https%3A%2F%2Fframagit.org%2Fatooms%2Fpostprocessing/HEAD?labpath=docs%2Findex.ipynb).
+
+## Requirements
+
+- [numpy](https://pypi.org/project/numpy/)
+- [atooms](https://framagit.org/atooms/postprocessing.git)
+- [optional] [argh](https://pypi.org/project/argh/) (only needed when using `pp.py`)
+- [optional] [tqdm](https://pypi.org/project/tqdm/) (enable progress bars)
+- [optional] [argcomplete](https://pypi.org/project/argcomplete/) (enable tab-completion for `pp.py`)
+- [optional] fortran compiler for more efficient execution
+
+## Installation
+
+Install with `pip`
+```
+pip install atooms-pp
+```
+
+Or clone the project repository
+```
+git clone https://framagit.org/atooms/postprocessing.git
+cd postprocessing
+make install
+```
+
+## Contributing
+
+Contributions to the project are welcome. If you wish to contribute, check out [these guidelines](https://framagit.org/atooms/atooms/-/blob/master/CONTRIBUTING.md).
+
+## Authors
+
+Daniele Coslovich: https://www.units.it/daniele.coslovich/
+
+
```

### Comparing `atooms-pp-3.1.3/README.md` & `atooms-pp-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.1.3/atooms/postprocessing/__init__.py` & `atooms-pp-3.2.0/atooms/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.1.3/atooms/postprocessing/alpha2.py` & `atooms-pp-3.2.0/atooms/postprocessing/alpha2.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.1.3/atooms/postprocessing/api.py` & `atooms-pp-3.2.0/atooms/postprocessing/api.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.1.3/atooms/postprocessing/chi4t.py` & `atooms-pp-3.2.0/atooms/postprocessing/chi4t.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.1.3/atooms/postprocessing/core.py` & `atooms-pp-3.2.0/atooms/postprocessing/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,34 +23,34 @@
     def __init__(self, prog, *args, **kwargs):
         argparse.RawDescriptionHelpFormatter.__init__(self, prog,
                                                       indent_increment=2,
                                                       max_help_position=60,
                                                       width=None)
 
     def _get_help_string(self, action):
-        help = action.help
+        msg = action.help
         if '%(default)' not in action.help:
             if action.default is not argparse.SUPPRESS:
                 defaulting_nargs = [argparse.OPTIONAL, argparse.ZERO_OR_MORE]
                 if action.option_strings or action.nargs in defaulting_nargs:
-                    help += ' [default: %(default)s]'
-        return help
+                    msg += ' [default: %(default)s]'
+        return msg
 
-    def __add_whitespace(self, idx, iWSpace, text):
+    def __add_whitespace(self, idx, iwspace, text):
         if idx == 0:
             return text
-        return (" " * iWSpace) + text
+        return (" " * iwspace) + text
 
     def _split_lines(self, text, width):
         import re
         import textwrap as _textwrap
-        textRows = text.splitlines()
-        for idx, line in enumerate(textRows):
+        textrows = text.splitlines()
+        for idx, line in enumerate(textrows):
             search = re.search(r'\s*[0-9\-]{0,}\.?\s*', line)
             if line.strip() == "":
-                textRows[idx] = " "
+                textrows[idx] = " "
             elif search:
-                lWSpace = search.end()
-                lines = [self.__add_whitespace(i, lWSpace, x) for i, x in enumerate(_textwrap.wrap(line, width))]
-                textRows[idx] = lines
+                lwspace = search.end()
+                lines = [self.__add_whitespace(i, lwspace, x) for i, x in enumerate(_textwrap.wrap(line, width))]
+                textrows[idx] = lines
 
-        return [item for sublist in textRows for item in sublist]
+        return [item for sublist in textrows for item in sublist]
```

### Comparing `atooms-pp-3.1.3/atooms/postprocessing/correlation.py` & `atooms-pp-3.2.0/atooms/postprocessing/correlation.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.1.3/atooms/postprocessing/filter.py` & `atooms-pp-3.2.0/atooms/postprocessing/filter.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.1.3/atooms/postprocessing/fkt.py` & `atooms-pp-3.2.0/atooms/postprocessing/fkt.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.1.3/atooms/postprocessing/fourierspace.f90` & `atooms-pp-3.2.0/atooms/postprocessing/fourierspace.f90`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.1.3/atooms/postprocessing/fourierspace.py` & `atooms-pp-3.2.0/atooms/postprocessing/fourierspace.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.1.3/atooms/postprocessing/gr.py` & `atooms-pp-3.2.0/atooms/postprocessing/gr.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,20 +260,19 @@
             if len(pos_0) == 0 or len(pos_1) == 0:
                 continue
 
             # Switch between self and distinct calculation
             distinct = pos_0 is not pos_1
             remove_self_term = False
 
-            # Store side
+            # With a non-periodic cell, which just bounds the physical
+            # domain, we crop particles away from the surface (within rmax)
             system = self.trajectory.read(i)
             if system.cell is not None and hasattr(system.cell, 'periodic') and \
-               sum(system.cell.periodic) == 0 and self.rmax > 0:
-                # With a non-periodic cell, which just bounds the physical
-                # domain, we crop particles away from the surface (within rmax)
+               sum(system.cell.periodic) == 0:
                 assert self.rmax > 0, 'provide rmax>0'
                 # Booleans do not work here, so we just use integers,
                 # which are 1 is particles are on the surface and 0 otherwise
                 mask = compute.on_surface_c(pos_0, system.cell.side, self.rmax)
                 pos_0 = pos_0[mask == 0, :]
                 # Force distinct calculation. This gives a spurious signal at r=0, which we remove
                 distinct = True
@@ -283,14 +282,15 @@
             # This will only happen if the system is within a cell (and all directions are periodic)
             if linkedcells:
                 if not distinct:
                     neighbors, number_of_neighbors = linkedcells.compute(system.cell.side, pos_0, as_array=True, periodic=system.cell.periodic)
                 else:
                     neighbors, number_of_neighbors = linkedcells.compute(system.cell.side, pos_0, pos_1, as_array=True, periodic=system.cell.periodic)
 
+            # Store side
             # If there is no cell and anyway along non-periodic directions,
             # we replace sides with infty to work with f90 kernels (which apply PBC)
             if system.cell is not None:
                 side = system.cell.side.copy()
                 # TODO: fix partly periodic boundaries
                 assert sum(system.cell.periodic) in [0, ndims], \
                     'partly periodic cells are not supported yet'
@@ -319,19 +319,14 @@
                 if linkedcells is None:
                     compute.gr_distinct_c(pos_0, pos_1, side, dr, gr, bins)
                 else:
                     compute.gr_neighbors_distinct_c('C', pos_0, pos_1, neighbors, number_of_neighbors, side, dr, gr, bins)
 
             # Damned copies in python
             gr_all.append(gr.copy())
-
-        # import matplotlib.pyplot as plt
-        # plt.plot(pos_0[:, 0], pos_0[:, 1], 'o')
-        # plt.plot(pos_1[:, 0], pos_1[:, 1], '+')
-        # plt.show()
         
         # Normalization
         # Array r is used to compute shells, we thus use the bin boundaries
         r = bins - (bins[1] - bins[0]) / 2
         N_0 = numpy.average(N_0)
         N_1 = numpy.average(N_1)
         if system.cell is not None:
```

### Comparing `atooms-pp-3.1.3/atooms/postprocessing/helpers.py` & `atooms-pp-3.2.0/atooms/postprocessing/helpers.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.1.3/atooms/postprocessing/ik.py` & `atooms-pp-3.2.0/atooms/postprocessing/ik.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.1.3/atooms/postprocessing/linkedcells.py` & `atooms-pp-3.2.0/atooms/postprocessing/linkedcells.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.1.3/atooms/postprocessing/msd.py` & `atooms-pp-3.2.0/atooms/postprocessing/msd.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.1.3/atooms/postprocessing/partial.py` & `atooms-pp-3.2.0/atooms/postprocessing/partial.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.1.3/atooms/postprocessing/progress.py` & `atooms-pp-3.2.0/atooms/postprocessing/progress.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.1.3/atooms/postprocessing/qt.py` & `atooms-pp-3.2.0/atooms/postprocessing/qt.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.1.3/atooms/postprocessing/realspace.f90` & `atooms-pp-3.2.0/atooms/postprocessing/realspace.f90`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.1.3/atooms/postprocessing/s4kt.py` & `atooms-pp-3.2.0/atooms/postprocessing/s4kt.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.1.3/atooms/postprocessing/sacf.py` & `atooms-pp-3.2.0/atooms/postprocessing/sacf.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.1.3/atooms/postprocessing/sk.py` & `atooms-pp-3.2.0/atooms/postprocessing/sk.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.1.3/atooms/postprocessing/susceptibility.py` & `atooms-pp-3.2.0/atooms/postprocessing/susceptibility.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.1.3/atooms/postprocessing/vacf.py` & `atooms-pp-3.2.0/atooms/postprocessing/vacf.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.1.3/atooms_pp.egg-info/PKG-INFO` & `atooms-pp-3.2.0/atooms_pp.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,114 +1,117 @@
 Metadata-Version: 2.1
 Name: atooms-pp
-Version: 3.1.3
+Version: 3.2.0
 Summary: Post-processing tools for particle simulations
 Home-page: https://framagit.org/atooms/postprocessing
 Author: Daniele Coslovich
 Author-email: daniele.coslovich@umontpellier.fr
 License: GPLv3
-Description: # Postprocessing
-        
-        [![pypi](https://img.shields.io/pypi/v/atooms-pp.svg)](https://pypi.python.org/pypi/atooms-pp/)
-        [![version](https://img.shields.io/pypi/pyversions/atooms-pp.svg)](https://pypi.python.org/pypi/atooms-pp/)
-        [![license](https://img.shields.io/pypi/l/atooms-pp.svg)](https://en.wikipedia.org/wiki/GNU_General_Public_License)
-        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/git/https%3A%2F%2Fframagit.org%2Fatooms%2Fpostprocessing/HEAD?labpath=docs%2Findex.ipynb)
-        [![pipeline](https://framagit.org/atooms/postprocessing/badges/master/pipeline.svg)](https://framagit.org/atooms/postprocessing/badges/master/pipeline.svg)
-        [![coverage report](https://framagit.org/atooms/postprocessing/badges/master/coverage.svg?job=test:f90)](https://framagit.org/atooms/postprocessing/-/commits/master)
-        
-        A Python package to compute static and dynamic correlation functions from simulations of interacting particles, such as molecular dynamics or Monte Carlo simulations. Based on [atooms](https://framagit.org/atooms/atooms).
-        
-        ## Quick start
-        
-        Postprocessing works on trajectories. Any trajectory format recognized by
-        [atooms](https://framagit.org/atooms/atooms.git) can be processed, for instance most "xyz" files
-        should work fine. If you use a custom trajectory format, it is easy to [add it](https://atooms.frama.io/atooms/).
-        
-        As an example, we compute the structure factor S(k) from the file `trajectory.xyz` in the `data/` folder.
-        
-        ### From the command line
-        
-        ```sh
-        pp.py --norigins 0.2 msd data/trajectory.xyz
-        ```
-        We just used 20% of the available time frames to compute the averages using the `--norigins` flag. Without it, `atooms-pp` applies an heuristics to determine the number of time frames required to achieve a reasonable data quality. The results of the calculation are stored in the file `data/trajectory.xyz.pp.sk`. 
-        
-        ### From Python
-        
-        The same calculation can be done from Python:
-        
-        ```python
-        from atooms.trajectory import Trajectory
-        import atooms.postprocessing as pp
-        
-        with Trajectory('data/trajectory.xyz') as t:
-             p = pp.StructureFactor(t)
-             p.do()
-        ```
-        
-        ## Features
-        
-        Available correlation and distribution functions
-        
-        - *Real space*
-          - radial distribution function
-          - mean square displacement
-          - velocity auto-correlation function
-          - self overlap functions
-          - collective overlap functions
-          - dynamic susceptibility of the self overlap function
-          - non-Gaussian parameter
-          - bond-angle distribution
-        - *Fourier space*
-          - structure factor
-          - spectral density
-          - self intermediate scattering functions
-          - collective intermediate scattering functions
-          - four-point dynamic susceptibility
-        
-        ## Documentation
-        
-        Check out the [tutorial](https://atooms.frama.io/postprocessing/tutorial) for more examples and the [public API](https://atooms.frama.io/postprocessing/api/postprocessing) for full details.
-        
-        Org-mode and jupyter notebooks are available under `docs/`. You can run the tutorial interactively on [Binder]( https://mybinder.org/v2/git/https%3A%2F%2Fframagit.org%2Fatooms%2Fpostprocessing/HEAD?labpath=docs%2Findex.ipynb).
-        
-        ## Requirements
-        
-        - [numpy](https://pypi.org/project/numpy/)
-        - [atooms](https://framagit.org/atooms/postprocessing.git)
-        - [optional] [argh](https://pypi.org/project/argh/) (only needed when using `pp.py`)
-        - [optional] [tqdm](https://pypi.org/project/tqdm/) (enable progress bars)
-        - [optional] [argcomplete](https://pypi.org/project/argcomplete/) (enable tab-completion for `pp.py`)
-        - [optional] fortran compiler for more efficient execution
-        
-        ## Installation
-        
-        Install with `pip`
-        ```
-        pip install atooms-pp
-        ```
-        
-        Or clone the project repository
-        ```
-        git clone https://framagit.org/atooms/postprocessing.git
-        cd postprocessing
-        make install
-        ```
-        
-        ## Contributing
-        
-        Contributions to the project are welcome. If you wish to contribute, check out [these guidelines](https://framagit.org/atooms/atooms/-/blob/master/CONTRIBUTING.md).
-        
-        ## Authors
-        
-        Daniele Coslovich: https://www.units.it/daniele.coslovich/
-        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Postprocessing
+
+[![pypi](https://img.shields.io/pypi/v/atooms-pp.svg)](https://pypi.python.org/pypi/atooms-pp/)
+[![version](https://img.shields.io/pypi/pyversions/atooms-pp.svg)](https://pypi.python.org/pypi/atooms-pp/)
+[![license](https://img.shields.io/pypi/l/atooms-pp.svg)](https://en.wikipedia.org/wiki/GNU_General_Public_License)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/git/https%3A%2F%2Fframagit.org%2Fatooms%2Fpostprocessing/HEAD?labpath=docs%2Findex.ipynb)
+[![pipeline](https://framagit.org/atooms/postprocessing/badges/master/pipeline.svg)](https://framagit.org/atooms/postprocessing/badges/master/pipeline.svg)
+[![coverage report](https://framagit.org/atooms/postprocessing/badges/master/coverage.svg?job=test:f90)](https://framagit.org/atooms/postprocessing/-/commits/master)
+
+A Python package to compute static and dynamic correlation functions from simulations of interacting particles, such as molecular dynamics or Monte Carlo simulations. Based on [atooms](https://framagit.org/atooms/atooms).
+
+## Quick start
+
+Postprocessing works on trajectories. Any trajectory format recognized by
+[atooms](https://framagit.org/atooms/atooms.git) can be processed, for instance most "xyz" files
+should work fine. If you use a custom trajectory format, it is easy to [add it](https://atooms.frama.io/atooms/).
+
+As an example, we compute the structure factor S(k) from the file `trajectory.xyz` in the `data/` folder.
+
+### From the command line
+
+```sh
+pp.py --norigins 0.2 msd data/trajectory.xyz
+```
+We just used 20% of the available time frames to compute the averages using the `--norigins` flag. Without it, `atooms-pp` applies an heuristics to determine the number of time frames required to achieve a reasonable data quality. The results of the calculation are stored in the file `data/trajectory.xyz.pp.sk`. 
+
+### From Python
+
+The same calculation can be done from Python:
+
+```python
+from atooms.trajectory import Trajectory
+import atooms.postprocessing as pp
+
+with Trajectory('data/trajectory.xyz') as t:
+     p = pp.StructureFactor(t)
+     p.do()
+```
+
+## Features
+
+Available correlation and distribution functions
+
+- *Real space*
+  - radial distribution function
+  - mean square displacement
+  - velocity auto-correlation function
+  - self overlap functions
+  - collective overlap functions
+  - dynamic susceptibility of the self overlap function
+  - non-Gaussian parameter
+  - bond-angle distribution
+- *Fourier space*
+  - structure factor
+  - spectral density
+  - self intermediate scattering functions
+  - collective intermediate scattering functions
+  - four-point dynamic susceptibility
+
+## Documentation
+
+Check out the [tutorial](https://atooms.frama.io/postprocessing/tutorial) for more examples and the [public API](https://atooms.frama.io/postprocessing/api/postprocessing) for full details.
+
+Org-mode and jupyter notebooks are available under `docs/`. You can run the tutorial interactively on [Binder]( https://mybinder.org/v2/git/https%3A%2F%2Fframagit.org%2Fatooms%2Fpostprocessing/HEAD?labpath=docs%2Findex.ipynb).
+
+## Requirements
+
+- [numpy](https://pypi.org/project/numpy/)
+- [atooms](https://framagit.org/atooms/postprocessing.git)
+- [optional] [argh](https://pypi.org/project/argh/) (only needed when using `pp.py`)
+- [optional] [tqdm](https://pypi.org/project/tqdm/) (enable progress bars)
+- [optional] [argcomplete](https://pypi.org/project/argcomplete/) (enable tab-completion for `pp.py`)
+- [optional] fortran compiler for more efficient execution
+
+## Installation
+
+Install with `pip`
+```
+pip install atooms-pp
+```
+
+Or clone the project repository
+```
+git clone https://framagit.org/atooms/postprocessing.git
+cd postprocessing
+make install
+```
+
+## Contributing
+
+Contributions to the project are welcome. If you wish to contribute, check out [these guidelines](https://framagit.org/atooms/atooms/-/blob/master/CONTRIBUTING.md).
+
+## Authors
+
+Daniele Coslovich: https://www.units.it/daniele.coslovich/
+
+
```

### Comparing `atooms-pp-3.1.3/atooms_pp.egg-info/SOURCES.txt` & `atooms-pp-3.2.0/atooms_pp.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 atooms/__init__.py
 atooms/postprocessing/__init__.py
 atooms/postprocessing/_commit.py
 atooms/postprocessing/_version.py
```

### Comparing `atooms-pp-3.1.3/bin/acf.py` & `atooms-pp-3.2.0/bin/acf.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.1.3/bin/pp.py` & `atooms-pp-3.2.0/bin/pp.py`

 * *Files identical despite different names*

### Comparing `atooms-pp-3.1.3/setup.py` & `atooms-pp-3.2.0/setup.py`

 * *Files identical despite different names*

