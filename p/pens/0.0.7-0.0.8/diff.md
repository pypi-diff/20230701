# Comparing `tmp/pens-0.0.7.tar.gz` & `tmp/pens-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pens-0.0.7.tar", last modified: Wed May 25 16:33:57 2022, max compression
+gzip compressed data, was "pens-0.0.8.tar", last modified: Fri Jun 30 23:55:54 2023, max compression
```

## Comparing `pens-0.0.7.tar` & `pens-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 fzhu       (501) staff       (20)        0 2022-05-25 16:33:57.898815 pens-0.0.7/
--rw-r--r--   0 fzhu       (501) staff       (20)    35149 2022-01-22 02:03:12.000000 pens-0.0.7/LICENSE
--rw-r--r--   0 fzhu       (501) staff       (20)      997 2022-05-25 16:33:57.898234 pens-0.0.7/PKG-INFO
--rw-r--r--   0 fzhu       (501) staff       (20)      429 2022-01-22 04:20:42.000000 pens-0.0.7/README.rst
-drwxr-xr-x   0 fzhu       (501) staff       (20)        0 2022-05-25 16:33:57.870632 pens-0.0.7/pens/
--rw-r--r--   0 fzhu       (501) staff       (20)      188 2022-01-22 05:20:50.000000 pens-0.0.7/pens/__init__.py
--rw-r--r--   0 fzhu       (501) staff       (20)    11542 2022-05-25 16:17:03.000000 pens-0.0.7/pens/ens.py
--rw-r--r--   0 fzhu       (501) staff       (20)     3411 2022-05-25 16:32:32.000000 pens-0.0.7/pens/utils.py
--rw-r--r--   0 fzhu       (501) staff       (20)     4182 2022-01-22 04:22:28.000000 pens-0.0.7/pens/visual.py
-drwxr-xr-x   0 fzhu       (501) staff       (20)        0 2022-05-25 16:33:57.895453 pens-0.0.7/pens.egg-info/
--rw-r--r--   0 fzhu       (501) staff       (20)      997 2022-05-25 16:33:57.000000 pens-0.0.7/pens.egg-info/PKG-INFO
--rw-r--r--   0 fzhu       (501) staff       (20)      251 2022-05-25 16:33:57.000000 pens-0.0.7/pens.egg-info/SOURCES.txt
--rw-r--r--   0 fzhu       (501) staff       (20)        1 2022-05-25 16:33:57.000000 pens-0.0.7/pens.egg-info/dependency_links.txt
--rw-r--r--   0 fzhu       (501) staff       (20)        1 2022-01-22 02:12:42.000000 pens-0.0.7/pens.egg-info/not-zip-safe
--rw-r--r--   0 fzhu       (501) staff       (20)       53 2022-05-25 16:33:57.000000 pens-0.0.7/pens.egg-info/requires.txt
--rw-r--r--   0 fzhu       (501) staff       (20)        5 2022-05-25 16:33:57.000000 pens-0.0.7/pens.egg-info/top_level.txt
--rw-r--r--   0 fzhu       (501) staff       (20)       38 2022-05-25 16:33:57.898931 pens-0.0.7/setup.cfg
--rw-r--r--   0 fzhu       (501) staff       (20)      994 2022-05-25 16:33:07.000000 pens-0.0.7/setup.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-30 23:55:54.933863 pens-0.0.8/
+-rw-r--r--   0 fengzhu    (502) staff       (20)    35149 2022-01-25 19:00:43.000000 pens-0.0.8/LICENSE
+-rw-r--r--   0 fengzhu    (502) staff       (20)      978 2023-06-30 23:55:54.933633 pens-0.0.8/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)      429 2022-01-25 19:00:43.000000 pens-0.0.8/README.rst
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-30 23:55:54.930197 pens-0.0.8/pens/
+-rw-r--r--   0 fengzhu    (502) staff       (20)      188 2022-01-25 19:00:43.000000 pens-0.0.8/pens/__init__.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    45202 2022-11-30 13:45:11.000000 pens-0.0.8/pens/ens.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)     6832 2022-11-30 13:45:11.000000 pens-0.0.8/pens/utils.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)     4182 2022-01-25 19:00:43.000000 pens-0.0.8/pens/visual.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-30 23:55:54.933178 pens-0.0.8/pens.egg-info/
+-rw-r--r--   0 fengzhu    (502) staff       (20)      978 2023-06-30 23:55:54.000000 pens-0.0.8/pens.egg-info/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)      251 2023-06-30 23:55:54.000000 pens-0.0.8/pens.egg-info/SOURCES.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-06-30 23:55:54.000000 pens-0.0.8/pens.egg-info/dependency_links.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2022-02-03 06:59:21.000000 pens-0.0.8/pens.egg-info/not-zip-safe
+-rw-r--r--   0 fengzhu    (502) staff       (20)       84 2023-06-30 23:55:54.000000 pens-0.0.8/pens.egg-info/requires.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        5 2023-06-30 23:55:54.000000 pens-0.0.8/pens.egg-info/top_level.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-06-30 23:55:54.933915 pens-0.0.8/setup.cfg
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1057 2022-11-30 13:45:11.000000 pens-0.0.8/setup.py
```

### Comparing `pens-0.0.7/LICENSE` & `pens-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pens-0.0.7/PKG-INFO` & `pens-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pens
-Version: 0.0.7
+Version: 0.0.8
 Summary: pens: utilities for comparing paleoclimate reconstruction ensembles
 Home-page: https://github.com/fzhu2e/pens
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fzhu@nuist.edu.cn, julieneg@usc.edu
 License: GPL 3.0 license
-Keywords: paleocliamte reconstruction ensembles
-Platform: UNKNOWN
+Keywords: paleoclimate reconstruction ensembles
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: pyleo
 License-File: LICENSE
 
@@ -22,8 +21,7 @@
 `pens` aims to provide a toolbox for comparing paleoclimate reconstruction ensembles.
 
 Documentation
 =============
 
 + Homepage: https://fzhu2e.github.io/pens
 + Installation: https://fzhu2e.github.io/pens/ug-installation.html
-
```

### Comparing `pens-0.0.7/pens/visual.py` & `pens-0.0.8/pens/visual.py`

 * *Files identical despite different names*

### Comparing `pens-0.0.7/pens.egg-info/PKG-INFO` & `pens-0.0.8/pens.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pens
-Version: 0.0.7
+Version: 0.0.8
 Summary: pens: utilities for comparing paleoclimate reconstruction ensembles
 Home-page: https://github.com/fzhu2e/pens
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fzhu@nuist.edu.cn, julieneg@usc.edu
 License: GPL 3.0 license
-Keywords: paleocliamte reconstruction ensembles
-Platform: UNKNOWN
+Keywords: paleoclimate reconstruction ensembles
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: pyleo
 License-File: LICENSE
 
@@ -22,8 +21,7 @@
 `pens` aims to provide a toolbox for comparing paleoclimate reconstruction ensembles.
 
 Documentation
 =============
 
 + Homepage: https://fzhu2e.github.io/pens
 + Installation: https://fzhu2e.github.io/pens/ug-installation.html
-
```

### Comparing `pens-0.0.7/setup.py` & `pens-0.0.8/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 from setuptools import setup, find_packages
 
 with open('README.rst', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='pens',  # required
-    version='0.0.7',
+    version='0.0.8',
     description='pens: utilities for comparing paleoclimate reconstruction ensembles',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Feng Zhu, Julien Emile-Geay',
     author_email='fzhu@nuist.edu.cn, julieneg@usc.edu',
     url='https://github.com/fzhu2e/pens',
     packages=find_packages(),
     include_package_data=True,
     license="GPL 3.0 license",
     zip_safe=False,
-    keywords='paleocliamte reconstruction ensembles',
+    keywords='paleoclimate reconstruction ensembles',
     classifiers=[
         'Natural Language :: English',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     install_requires=[
         'termcolor',
         'pandas',
         'tqdm',
         'xarray',
         'dask',
+        'stochastic',
+        'properscoring',
+        'covar'
     ],
     extras_require={
         'pyleo': ['pyleoclim'],
     }
 )
```

