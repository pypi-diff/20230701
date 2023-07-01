# Comparing `tmp/pcdataloader-2.0.3.tar.gz` & `tmp/pcdataloader-3.2.0.tar.gz`

## Comparing `pcdataloader-2.0.3.tar` & `pcdataloader-3.2.0.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 pcdataloader-2.0.3/pcDataLoader/__init__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pcdataloader-2.0.3/.gitignore
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 pcdataloader-2.0.3/LICENSE
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 pcdataloader-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 pcdataloader-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 pcdataloader-3.2.0/pcDataLoader/__init__.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 pcdataloader-3.2.0/.gitignore
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 pcdataloader-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 pcdataloader-3.2.0/PKG-INFO
```

### Comparing `pcdataloader-2.0.3/pyproject.toml` & `pcdataloader-3.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -2,22 +2,14 @@
 # A hatchling based setup module.
 #
 # See:
 # https://packaging.python.org/en/latest/
 # https://packaging.python.org/en/latest/tutorials/packaging-projects/
 # https://hatch.pypa.io/latest/
 #
-# language: python3
-# author: Elmar Bucher
-# date: 2023-06-16
-# license: BSD-3-Clause
-#
-# description:
-#     a simple, pip installable gateway module to the pcdl module.
-#
 # releasing a next version on pypi:
 # 0. # increase version number below
 # 2. git commit -m'@ pcDataLoader : pcdl python3 module bridge.'
 # 3. git tag -a v0.0.0 -m'version 0.0.0'
 # 4. rm -r dist
 # 6. python3 -m build --sdist  # make source distribution
 # 7. python3 -m build --wheel  # make binary distribution python wheel
@@ -33,15 +25,15 @@
 
 
 [project]
 # name of the project
 # pip install pcDataLoader
 # import pcDataLoader as pc
 name = "pcDataLoader"
-version = "2.0.3"
+version = "3.2.0"
 
 description = 'LOAD "pcdl",8,1'
 requires-python = ">=3.6, <4"
 
 license = "BSD-3-Clause"
 #license-files = {paths = ["LICENSE"]}
 
@@ -64,15 +56,15 @@
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
 ]
 
 dependencies = [
-    "pcdl<3",
+    "pcdl",
 ]
 
 
 [project.urls]
 "Homepage lab" = "http://www.mathcancer.org/"
 "Homepage project" = "http://physicell.org/"
 Hompage = "https://github.com/elmbeech/physicelldataloader"
```

### Comparing `pcdataloader-2.0.3/PKG-INFO` & `pcdataloader-3.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: pcDataLoader
-Version: 2.0.3
+Version: 3.2.0
 Summary: LOAD "pcdl",8,1
 Project-URL: Homepage lab, http://www.mathcancer.org/
 Project-URL: Homepage project, http://physicell.org/
 Project-URL: Hompage, https://github.com/elmbeech/physicelldataloader
 Project-URL: Documentation, https://github.com/elmbeech/physicelldataloader/tree/master/man
 Project-URL: Issues, https://github.com/elmbeech/physicelldataloader/issues
 Project-URL: Source, https://github.com/elmbeech/physicelldataloader
 Author-email: Elmar Bucher <epbucher@iu.edu>
 Maintainer-email: Elmar Bucher <epbucher@iu.edu>
 License-Expression: BSD-3-Clause
-License-File: LICENSE
 Keywords: analysis,data,physicell,python3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: <4,>=3.6
-Requires-Dist: pcdl<3
+Requires-Dist: pcdl
```

