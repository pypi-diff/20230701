# Comparing `tmp/python-igraph-0.9.8.tar.gz` & `tmp/python-igraph-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-igraph-0.9.8.tar", last modified: Fri Oct 29 00:54:26 2021, max compression
+gzip compressed data, was "python-igraph-0.9.9.tar", last modified: Mon Jan 10 14:50:39 2022, max compression
```

## Comparing `python-igraph-0.9.8.tar` & `python-igraph-0.9.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 tamas      (501) staff       (20)        0 2021-10-29 00:54:26.915968 python-igraph-0.9.8/
--rw-r--r--   0 tamas      (501) staff       (20)    17987 2021-10-28 19:27:21.000000 python-igraph-0.9.8/LICENSE
--rw-r--r--   0 tamas      (501) staff       (20)     2558 2021-10-29 00:54:26.915683 python-igraph-0.9.8/PKG-INFO
--rw-r--r--   0 tamas      (501) staff       (20)      893 2021-10-28 19:25:28.000000 python-igraph-0.9.8/README.md
-drwxr-xr-x   0 tamas      (501) staff       (20)        0 2021-10-29 00:54:26.915216 python-igraph-0.9.8/python_igraph.egg-info/
--rw-r--r--   0 tamas      (501) staff       (20)     2558 2021-10-29 00:54:26.000000 python-igraph-0.9.8/python_igraph.egg-info/PKG-INFO
--rw-r--r--   0 tamas      (501) staff       (20)      210 2021-10-29 00:54:26.000000 python-igraph-0.9.8/python_igraph.egg-info/SOURCES.txt
--rw-r--r--   0 tamas      (501) staff       (20)        1 2021-10-29 00:54:26.000000 python-igraph-0.9.8/python_igraph.egg-info/dependency_links.txt
--rw-r--r--   0 tamas      (501) staff       (20)      180 2021-10-29 00:54:26.000000 python-igraph-0.9.8/python_igraph.egg-info/requires.txt
--rw-r--r--   0 tamas      (501) staff       (20)        1 2021-10-29 00:54:26.000000 python-igraph-0.9.8/python_igraph.egg-info/top_level.txt
--rw-r--r--   0 tamas      (501) staff       (20)       38 2021-10-29 00:54:26.916056 python-igraph-0.9.8/setup.cfg
--rw-r--r--   0 tamas      (501) staff       (20)     3405 2021-10-29 00:52:58.000000 python-igraph-0.9.8/setup.py
+drwxr-xr-x   0 tamas      (501) staff       (20)        0 2022-01-10 14:50:39.569559 python-igraph-0.9.9/
+-rw-r--r--   0 tamas      (501) staff       (20)    17987 2021-10-28 19:27:21.000000 python-igraph-0.9.9/LICENSE
+-rw-r--r--   0 tamas      (501) staff       (20)     2551 2022-01-10 14:50:39.569468 python-igraph-0.9.9/PKG-INFO
+-rw-r--r--   0 tamas      (501) staff       (20)      893 2021-10-28 19:25:28.000000 python-igraph-0.9.9/README.md
+drwxr-xr-x   0 tamas      (501) staff       (20)        0 2022-01-10 14:50:39.569340 python-igraph-0.9.9/python_igraph.egg-info/
+-rw-r--r--   0 tamas      (501) staff       (20)     2551 2022-01-10 14:50:39.000000 python-igraph-0.9.9/python_igraph.egg-info/PKG-INFO
+-rw-r--r--   0 tamas      (501) staff       (20)      210 2022-01-10 14:50:39.000000 python-igraph-0.9.9/python_igraph.egg-info/SOURCES.txt
+-rw-r--r--   0 tamas      (501) staff       (20)        1 2022-01-10 14:50:39.000000 python-igraph-0.9.9/python_igraph.egg-info/dependency_links.txt
+-rw-r--r--   0 tamas      (501) staff       (20)      180 2022-01-10 14:50:39.000000 python-igraph-0.9.9/python_igraph.egg-info/requires.txt
+-rw-r--r--   0 tamas      (501) staff       (20)        1 2022-01-10 14:50:39.000000 python-igraph-0.9.9/python_igraph.egg-info/top_level.txt
+-rw-r--r--   0 tamas      (501) staff       (20)       38 2022-01-10 14:50:39.569589 python-igraph-0.9.9/setup.cfg
+-rw-r--r--   0 tamas      (501) staff       (20)     3398 2022-01-10 14:49:42.000000 python-igraph-0.9.9/setup.py
```

### Comparing `python-igraph-0.9.8/LICENSE` & `python-igraph-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python-igraph-0.9.8/PKG-INFO` & `python-igraph-0.9.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-igraph
-Version: 0.9.8
+Version: 0.9.9
 Summary: High performance graph data structures and algorithms (legacy package)
 Home-page: https://igraph.org/python
 Author: Tamas Nepusz
 Author-email: ntamas@gmail.com
 License: GNU General Public License (GPL)
 Project-URL: Bug Tracker, https://github.com/igraph/python-igraph/issues
 Project-URL: Changelog, https://github.com/igraph/python-igraph/blob/master/CHANGELOG.md
@@ -37,17 +37,17 @@
 Provides-Extra: plotly
 Provides-Extra: plotting
 License-File: LICENSE
 
 Python interface to the igraph high performance graph
 library, primarily aimed at complex network research and analysis.
 
-**This package is deprecated; use the ``igraph`` package instead. This package will
-be kep in sync with ``igraph`` until Sep 1, 2022 and it will receive updates no
-more after Sep 1, 2022.**
+**This package is deprecated; use the igraph package instead. This package will
+be kept in sync with igraph until Sep 1, 2022 and it will not receive any
+updates after Sep 1, 2022.**
 
 Graph plotting functionality is provided by the Cairo library, so make
 sure you install the Python bindings of Cairo if you want to generate
 publication-quality graph plots. You can try either `pycairo
 <http://cairographics.org/pycairo>`_ or `cairocffi <http://cairocffi.readthedocs.io>`_,
 ``cairocffi`` is recommended because there were bug reports affecting igraph
 graph plots in Jupyter notebooks when using ``pycairo`` (but not with
```

### Comparing `python-igraph-0.9.8/README.md` & `python-igraph-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `python-igraph-0.9.8/python_igraph.egg-info/PKG-INFO` & `python-igraph-0.9.9/python_igraph.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-igraph
-Version: 0.9.8
+Version: 0.9.9
 Summary: High performance graph data structures and algorithms (legacy package)
 Home-page: https://igraph.org/python
 Author: Tamas Nepusz
 Author-email: ntamas@gmail.com
 License: GNU General Public License (GPL)
 Project-URL: Bug Tracker, https://github.com/igraph/python-igraph/issues
 Project-URL: Changelog, https://github.com/igraph/python-igraph/blob/master/CHANGELOG.md
@@ -37,17 +37,17 @@
 Provides-Extra: plotly
 Provides-Extra: plotting
 License-File: LICENSE
 
 Python interface to the igraph high performance graph
 library, primarily aimed at complex network research and analysis.
 
-**This package is deprecated; use the ``igraph`` package instead. This package will
-be kep in sync with ``igraph`` until Sep 1, 2022 and it will receive updates no
-more after Sep 1, 2022.**
+**This package is deprecated; use the igraph package instead. This package will
+be kept in sync with igraph until Sep 1, 2022 and it will not receive any
+updates after Sep 1, 2022.**
 
 Graph plotting functionality is provided by the Cairo library, so make
 sure you install the Python bindings of Cairo if you want to generate
 publication-quality graph plots. You can try either `pycairo
 <http://cairographics.org/pycairo>`_ or `cairocffi <http://cairocffi.readthedocs.io>`_,
 ``cairocffi`` is recommended because there were bug reports affecting igraph
 graph plots in Jupyter notebooks when using ``pycairo`` (but not with
```

### Comparing `python-igraph-0.9.8/setup.py` & `python-igraph-0.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,22 @@
     print("This module requires Python >= 3.6")
     sys.exit(1)
 
 ###########################################################################
 
 from setuptools import setup
 
-VERSION = "0.9.8"
+VERSION = "0.9.9"
 
 description = """Python interface to the igraph high performance graph
 library, primarily aimed at complex network research and analysis.
 
-**This package is deprecated; use the ``igraph`` package instead. This package will
-be kep in sync with ``igraph`` until Sep 1, 2022 and it will receive updates no
-more after Sep 1, 2022.**
+**This package is deprecated; use the igraph package instead. This package will
+be kept in sync with igraph until Sep 1, 2022 and it will not receive any
+updates after Sep 1, 2022.**
 
 Graph plotting functionality is provided by the Cairo library, so make
 sure you install the Python bindings of Cairo if you want to generate
 publication-quality graph plots. You can try either `pycairo
 <http://cairographics.org/pycairo>`_ or `cairocffi <http://cairocffi.readthedocs.io>`_,
 ``cairocffi`` is recommended because there were bug reports affecting igraph
 graph plots in Jupyter notebooks when using ``pycairo`` (but not with
```

