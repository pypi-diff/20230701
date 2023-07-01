# Comparing `tmp/pens-0.0.8.tar.gz` & `tmp/pens-2023.6.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pens-0.0.8.tar", last modified: Fri Jun 30 23:55:54 2023, max compression
+gzip compressed data, was "pens-2023.6.30.tar", last modified: Fri Jun 30 23:59:29 2023, max compression
```

## Comparing `pens-0.0.8.tar` & `pens-2023.6.30.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-30 23:55:54.933863 pens-0.0.8/
--rw-r--r--   0 fengzhu    (502) staff       (20)    35149 2022-01-25 19:00:43.000000 pens-0.0.8/LICENSE
--rw-r--r--   0 fengzhu    (502) staff       (20)      978 2023-06-30 23:55:54.933633 pens-0.0.8/PKG-INFO
--rw-r--r--   0 fengzhu    (502) staff       (20)      429 2022-01-25 19:00:43.000000 pens-0.0.8/README.rst
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-30 23:55:54.930197 pens-0.0.8/pens/
--rw-r--r--   0 fengzhu    (502) staff       (20)      188 2022-01-25 19:00:43.000000 pens-0.0.8/pens/__init__.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    45202 2022-11-30 13:45:11.000000 pens-0.0.8/pens/ens.py
--rw-r--r--   0 fengzhu    (502) staff       (20)     6832 2022-11-30 13:45:11.000000 pens-0.0.8/pens/utils.py
--rw-r--r--   0 fengzhu    (502) staff       (20)     4182 2022-01-25 19:00:43.000000 pens-0.0.8/pens/visual.py
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-30 23:55:54.933178 pens-0.0.8/pens.egg-info/
--rw-r--r--   0 fengzhu    (502) staff       (20)      978 2023-06-30 23:55:54.000000 pens-0.0.8/pens.egg-info/PKG-INFO
--rw-r--r--   0 fengzhu    (502) staff       (20)      251 2023-06-30 23:55:54.000000 pens-0.0.8/pens.egg-info/SOURCES.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-06-30 23:55:54.000000 pens-0.0.8/pens.egg-info/dependency_links.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        1 2022-02-03 06:59:21.000000 pens-0.0.8/pens.egg-info/not-zip-safe
--rw-r--r--   0 fengzhu    (502) staff       (20)       84 2023-06-30 23:55:54.000000 pens-0.0.8/pens.egg-info/requires.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        5 2023-06-30 23:55:54.000000 pens-0.0.8/pens.egg-info/top_level.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-06-30 23:55:54.933915 pens-0.0.8/setup.cfg
--rw-r--r--   0 fengzhu    (502) staff       (20)     1057 2022-11-30 13:45:11.000000 pens-0.0.8/setup.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-30 23:59:29.220374 pens-2023.6.30/
+-rw-r--r--   0 fengzhu    (502) staff       (20)    35149 2022-01-25 19:00:43.000000 pens-2023.6.30/LICENSE
+-rw-r--r--   0 fengzhu    (502) staff       (20)      982 2023-06-30 23:59:29.220193 pens-2023.6.30/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)      429 2022-01-25 19:00:43.000000 pens-2023.6.30/README.rst
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-30 23:59:29.217734 pens-2023.6.30/pens/
+-rw-r--r--   0 fengzhu    (502) staff       (20)      188 2022-01-25 19:00:43.000000 pens-2023.6.30/pens/__init__.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    45202 2022-11-30 13:45:11.000000 pens-2023.6.30/pens/ens.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)     6832 2022-11-30 13:45:11.000000 pens-2023.6.30/pens/utils.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)     4182 2022-01-25 19:00:43.000000 pens-2023.6.30/pens/visual.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-30 23:59:29.219832 pens-2023.6.30/pens.egg-info/
+-rw-r--r--   0 fengzhu    (502) staff       (20)      982 2023-06-30 23:59:29.000000 pens-2023.6.30/pens.egg-info/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)      251 2023-06-30 23:59:29.000000 pens-2023.6.30/pens.egg-info/SOURCES.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-06-30 23:59:29.000000 pens-2023.6.30/pens.egg-info/dependency_links.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2022-02-03 06:59:21.000000 pens-2023.6.30/pens.egg-info/not-zip-safe
+-rw-r--r--   0 fengzhu    (502) staff       (20)       84 2023-06-30 23:59:29.000000 pens-2023.6.30/pens.egg-info/requires.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        5 2023-06-30 23:59:29.000000 pens-2023.6.30/pens.egg-info/top_level.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-06-30 23:59:29.220422 pens-2023.6.30/setup.cfg
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1061 2023-06-30 23:59:08.000000 pens-2023.6.30/setup.py
```

### Comparing `pens-0.0.8/LICENSE` & `pens-2023.6.30/LICENSE`

 * *Files identical despite different names*

### Comparing `pens-0.0.8/PKG-INFO` & `pens-2023.6.30/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pens
-Version: 0.0.8
+Version: 2023.6.30
 Summary: pens: utilities for comparing paleoclimate reconstruction ensembles
 Home-page: https://github.com/fzhu2e/pens
 Author: Feng Zhu, Julien Emile-Geay
-Author-email: fzhu@nuist.edu.cn, julieneg@usc.edu
+Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: GPL 3.0 license
 Keywords: paleoclimate reconstruction ensembles
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 Provides-Extra: pyleo
 License-File: LICENSE
 
 *******************************************************************
 pens: utilities for comparing paleoclimate reconstruction ensembles
 *******************************************************************
```

### Comparing `pens-0.0.8/pens/ens.py` & `pens-2023.6.30/pens/ens.py`

 * *Files identical despite different names*

### Comparing `pens-0.0.8/pens/utils.py` & `pens-2023.6.30/pens/utils.py`

 * *Files identical despite different names*

### Comparing `pens-0.0.8/pens/visual.py` & `pens-2023.6.30/pens/visual.py`

 * *Files identical despite different names*

### Comparing `pens-0.0.8/pens.egg-info/PKG-INFO` & `pens-2023.6.30/pens.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pens
-Version: 0.0.8
+Version: 2023.6.30
 Summary: pens: utilities for comparing paleoclimate reconstruction ensembles
 Home-page: https://github.com/fzhu2e/pens
 Author: Feng Zhu, Julien Emile-Geay
-Author-email: fzhu@nuist.edu.cn, julieneg@usc.edu
+Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: GPL 3.0 license
 Keywords: paleoclimate reconstruction ensembles
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 Provides-Extra: pyleo
 License-File: LICENSE
 
 *******************************************************************
 pens: utilities for comparing paleoclimate reconstruction ensembles
 *******************************************************************
```

### Comparing `pens-0.0.8/setup.py` & `pens-2023.6.30/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from setuptools import setup, find_packages
 
 with open('README.rst', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='pens',  # required
-    version='0.0.8',
+    version='2023.6.30',
     description='pens: utilities for comparing paleoclimate reconstruction ensembles',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Feng Zhu, Julien Emile-Geay',
-    author_email='fzhu@nuist.edu.cn, julieneg@usc.edu',
+    author_email='fengzhu@ucar.edu, julieneg@usc.edu',
     url='https://github.com/fzhu2e/pens',
     packages=find_packages(),
     include_package_data=True,
     license="GPL 3.0 license",
     zip_safe=False,
     keywords='paleoclimate reconstruction ensembles',
     classifiers=[
         'Natural Language :: English',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
     ],
     install_requires=[
         'termcolor',
         'pandas',
         'tqdm',
         'xarray',
         'dask',
```

