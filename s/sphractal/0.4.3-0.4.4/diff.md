# Comparing `tmp/sphractal-0.4.3.tar.gz` & `tmp/sphractal-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphractal-0.4.3.tar", max compression
+gzip compressed data, was "sphractal-0.4.4.tar", max compression
```

## Comparing `sphractal-0.4.3.tar` & `sphractal-0.4.4.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1082 2023-07-01 08:12:27.577598 sphractal-0.4.3/LICENSE
--rw-r--r--   0        0        0     2925 2023-07-01 08:12:27.577598 sphractal-0.4.3/README.md
--rw-r--r--   0        0        0     1978 2023-07-01 08:13:11.260939 sphractal-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     2288 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/fbc/3DbinImBCcpu.cpp
--rw-r--r--   0        0        0     3111 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/fbc/3DbinImBCgpu.cpp
--rw-r--r--   0        0        0     2084 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/fbc/README.txt
--rw-r--r--   0        0        0     3581 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/fbc/bcCPU.cpp
--rw-r--r--   0        0        0      979 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/fbc/bcCPU.h
--rw-r--r--   0        0        0     4378 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/fbc/bcCUDA2D.cu
--rw-r--r--   0        0        0     1056 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/fbc/bcCUDA2D.cuh
--rw-r--r--   0        0        0     4947 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/fbc/bcCUDA3D.cu
--rw-r--r--   0        0        0     1056 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/fbc/bcCUDA3D.cuh
--rw-r--r--   0        0        0     5867 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/fbc/bcCUDA4D.cu
--rw-r--r--   0        0        0     1056 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/fbc/bcCUDA4D.cuh
--rw-r--r--   0        0        0    10330 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/fbc/test.cpp
--rw-r--r--   0        0        0     1394 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/sphractal/__init__.py
--rw-r--r--   0        0        0    21444 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/sphractal/boxCnt.py
--rw-r--r--   0        0        0     3821 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/sphractal/constants.py
--rw-r--r--   0        0        0        0 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/sphractal/data/__init__.py
--rw-r--r--   0        0        0    20105 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/sphractal/data/example.xyz
--rw-r--r--   0        0        0      279 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/sphractal/datasets.py
--rw-r--r--   0        0        0     8881 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/sphractal/surfExact.py
--rw-r--r--   0        0        0     8119 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/sphractal/surfPointClouds.py
--rw-r--r--   0        0        0    11480 2023-07-01 08:12:27.641597 sphractal-0.4.3/src/sphractal/utils.py
--rw-r--r--   0        0        0    94223 2023-07-01 08:12:27.641597 sphractal-0.4.3/tests/fixtures.py
--rw-r--r--   0        0        0    17404 2023-07-01 08:12:27.641597 sphractal-0.4.3/tests/test_sphractal.py
--rw-r--r--   0        0        0     4194 1970-01-01 00:00:00.000000 sphractal-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-01 12:37:51.500012 sphractal-0.4.4/LICENSE
+-rw-r--r--   0        0        0     3398 2023-07-01 12:37:51.500012 sphractal-0.4.4/README.md
+-rw-r--r--   0        0        0     1990 2023-07-01 12:38:30.775572 sphractal-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      710 2023-07-01 12:37:51.560011 sphractal-0.4.4/setup.py
+-rw-r--r--   0        0        0     2288 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/fbc/3DbinImBCcpu.cpp
+-rw-r--r--   0        0        0     3111 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/fbc/3DbinImBCgpu.cpp
+-rw-r--r--   0        0        0     2084 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/fbc/README.txt
+-rw-r--r--   0        0        0     3581 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/fbc/bcCPU.cpp
+-rw-r--r--   0        0        0      979 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/fbc/bcCPU.h
+-rw-r--r--   0        0        0     4378 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/fbc/bcCUDA2D.cu
+-rw-r--r--   0        0        0     1056 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/fbc/bcCUDA2D.cuh
+-rw-r--r--   0        0        0     4947 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/fbc/bcCUDA3D.cu
+-rw-r--r--   0        0        0     1056 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/fbc/bcCUDA3D.cuh
+-rw-r--r--   0        0        0     5867 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/fbc/bcCUDA4D.cu
+-rw-r--r--   0        0        0     1056 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/fbc/bcCUDA4D.cuh
+-rw-r--r--   0        0        0    10330 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/fbc/test.cpp
+-rw-r--r--   0        0        0     1394 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/sphractal/__init__.py
+-rw-r--r--   0        0        0    21444 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/sphractal/boxCnt.py
+-rw-r--r--   0        0        0     3821 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/sphractal/constants.py
+-rw-r--r--   0        0        0        0 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/sphractal/data/__init__.py
+-rw-r--r--   0        0        0    20105 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/sphractal/data/example.xyz
+-rw-r--r--   0        0        0      279 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/sphractal/datasets.py
+-rw-r--r--   0        0        0     8881 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/sphractal/surfExact.py
+-rw-r--r--   0        0        0     8119 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/sphractal/surfPointClouds.py
+-rw-r--r--   0        0        0    11480 2023-07-01 12:37:51.560011 sphractal-0.4.4/src/sphractal/utils.py
+-rw-r--r--   0        0        0    94223 2023-07-01 12:37:51.560011 sphractal-0.4.4/tests/fixtures.py
+-rw-r--r--   0        0        0    17404 2023-07-01 12:37:51.560011 sphractal-0.4.4/tests/test_sphractal.py
+-rw-r--r--   0        0        0     4667 1970-01-01 00:00:00.000000 sphractal-0.4.4/PKG-INFO
```

### Comparing `sphractal-0.4.3/LICENSE` & `sphractal-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.3/pyproject.toml` & `sphractal-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphractal"
-version = "0.4.3"
+version = "0.4.4"
 description = "Package to estimate fractal dimension of 3D surfaces formed from overlapping spheres via box-counting algorithm."
 authors = ["Jonathan Yik Chang Ting <jonting97@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Jon-Ting/sphractal"
 repository = "https://github.com/Jon-Ting/sphractal"
 documentation = "https://sphractal.readthedocs.io/en/latest/"
@@ -13,15 +13,15 @@
     "Intended Audience :: Science/Research", 
     "Natural Language :: English", 
     "Operating System :: OS Independent", 
     "Programming Language :: C++", 
     "Programming Language :: Python :: 3", 
     "Topic :: Scientific/Engineering", 
 ]
-include = ["tests/*", "src/fbc/*"]
+include = ["tests/*", "src/fbc/*", "setup.py"]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 matplotlib = ">=3.7.1"
 statsmodels = ">=0.14.0"
 scipy = {version = ">=1.11.0", python = ">=3.9,<3.13"}
 numba = ">=0.57.1"
```

### Comparing `sphractal-0.4.3/src/fbc/3DbinImBCcpu.cpp` & `sphractal-0.4.4/src/fbc/3DbinImBCcpu.cpp`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.3/src/fbc/3DbinImBCgpu.cpp` & `sphractal-0.4.4/src/fbc/3DbinImBCgpu.cpp`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.3/src/fbc/README.txt` & `sphractal-0.4.4/src/fbc/README.txt`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.3/src/fbc/bcCPU.cpp` & `sphractal-0.4.4/src/fbc/bcCPU.cpp`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.3/src/fbc/bcCPU.h` & `sphractal-0.4.4/src/fbc/bcCPU.h`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.3/src/fbc/bcCUDA2D.cu` & `sphractal-0.4.4/src/fbc/bcCUDA2D.cu`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.3/src/fbc/bcCUDA2D.cuh` & `sphractal-0.4.4/src/fbc/bcCUDA2D.cuh`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.3/src/fbc/bcCUDA3D.cu` & `sphractal-0.4.4/src/fbc/bcCUDA3D.cu`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.3/src/fbc/bcCUDA3D.cuh` & `sphractal-0.4.4/src/fbc/bcCUDA3D.cuh`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.3/src/fbc/bcCUDA4D.cu` & `sphractal-0.4.4/src/fbc/bcCUDA4D.cu`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.3/src/fbc/bcCUDA4D.cuh` & `sphractal-0.4.4/src/fbc/bcCUDA4D.cuh`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.3/src/fbc/test.cpp` & `sphractal-0.4.4/src/fbc/test.cpp`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.3/src/sphractal/__init__.py` & `sphractal-0.4.4/src/sphractal/__init__.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.3/src/sphractal/boxCnt.py` & `sphractal-0.4.4/src/sphractal/boxCnt.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.3/src/sphractal/constants.py` & `sphractal-0.4.4/src/sphractal/constants.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.3/src/sphractal/data/example.xyz` & `sphractal-0.4.4/src/sphractal/data/example.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.3/src/sphractal/surfExact.py` & `sphractal-0.4.4/src/sphractal/surfExact.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.3/src/sphractal/surfPointClouds.py` & `sphractal-0.4.4/src/sphractal/surfPointClouds.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.3/src/sphractal/utils.py` & `sphractal-0.4.4/src/sphractal/utils.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.3/tests/fixtures.py` & `sphractal-0.4.4/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.3/tests/test_sphractal.py` & `sphractal-0.4.4/tests/test_sphractal.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.4.3/PKG-INFO` & `sphractal-0.4.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphractal
-Version: 0.4.3
+Version: 0.4.4
 Summary: Package to estimate fractal dimension of 3D surfaces formed from overlapping spheres via box-counting algorithm.
 Home-page: https://github.com/Jon-Ting/sphractal
 License: MIT
 Keywords: box-counting,box-count,fractal,dimension,sphere,surface
 Author: Jonathan Yik Chang Ting
 Author-email: jonting97@gmail.com
 Requires-Python: >=3.9
@@ -35,21 +35,33 @@
 
 `Sphractal` is a package that provides functionality to estimate the fractal dimension of complex 3D surfaces formed 
 from overlapping spheres via box-counting algorithm. 
 
 ## Features
 
 ### Current
-* Representation of the surface as either point clouds or exact surfaces.
+* Representation of the surface as either point clouds (feature yet to be made available due to C++ compilation issues) or exact surfaces.
 * Efficient algorithm for 3D box-counting calculations.
 * Customisable parameters to control the level of detail and accuracy of the calculation.
 
 ### To be Done
 * Set path for exeDir.
 * Publish to Conda.
+  * cd condaForge/
+  * conda skeleton pypi sphractal
+  * vim sphractal/meta.yaml ('name', 'version', 'git_rev', 'git_url', 'imports', 'home', 'noarch', 'maintainer')
+  * vim build.sh
+  * vim bld.bat
+  * conda-build sphractal (record path)
+  * conda install --use-local sphractal
+  * conda list
+  * anaconda login
+  * anaconda upload PATH_TO_BZ2
+  * conda config --set anaconda_upload yes
+  * anaconda logout
 * Nested multiprocessing.
 * Better looking plots, allow figure size to be specified, allow choice for 'paper' and 'presentation'.
 * Consider transforming xyz coordinates when atoms are read in to avoid using minXYZ repetitively in `scanAtom()`.
 
 ## Installation
 
 Use `pip` or `conda` (yet to be implemented) to install `Sphractal`:
```

