# Comparing `tmp/liblinear-official-2.46.1.tar.gz` & `tmp/liblinear-official-2.47.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liblinear-official-2.46.1.tar", last modified: Fri Feb 17 08:33:01 2023, max compression
+gzip compressed data, was "liblinear-official-2.47.0.tar", last modified: Sat Jul  1 10:57:28 2023, max compression
```

## Comparing `liblinear-official-2.46.1.tar` & `liblinear-official-2.47.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-02-17 08:33:01.049505 liblinear-official-2.46.1/
--rw-rw-rw-   0        0        0     1517 2023-02-15 08:40:58.000000 liblinear-official-2.46.1/LICENSE
--rw-rw-rw-   0        0        0       48 2023-02-15 08:14:49.000000 liblinear-official-2.46.1/MANIFEST.in
--rw-rw-rw-   0        0        0    18278 2023-02-17 08:33:01.048504 liblinear-official-2.46.1/PKG-INFO
--rw-rw-rw-   0        0        0    17947 2023-02-15 08:14:49.000000 liblinear-official-2.46.1/README
-drwxrwxrwx   0        0        0        0 2023-02-17 08:33:00.998288 liblinear-official-2.46.1/cpp-source/
-drwxrwxrwx   0        0        0        0 2023-02-17 08:33:01.013253 liblinear-official-2.46.1/cpp-source/blas/
--rw-rw-rw-   0        0        0      727 2023-02-15 08:40:58.000000 liblinear-official-2.46.1/cpp-source/blas/blas.h
--rw-rw-rw-   0        0        0    16959 2023-02-15 08:40:58.000000 liblinear-official-2.46.1/cpp-source/blas/blasp.h
--rw-rw-rw-   0        0        0     1322 2023-02-15 08:40:58.000000 liblinear-official-2.46.1/cpp-source/blas/daxpy.c
--rw-rw-rw-   0        0        0     1329 2023-02-15 08:40:58.000000 liblinear-official-2.46.1/cpp-source/blas/ddot.c
--rw-rw-rw-   0        0        0     1427 2023-02-15 08:40:58.000000 liblinear-official-2.46.1/cpp-source/blas/dnrm2.c
--rw-rw-rw-   0        0        0     1144 2023-02-15 08:40:58.000000 liblinear-official-2.46.1/cpp-source/blas/dscal.c
--rw-rw-rw-   0        0        0    83989 2023-02-15 08:40:58.000000 liblinear-official-2.46.1/cpp-source/linear.cpp
--rw-rw-rw-   0        0        0      526 2023-02-15 08:40:58.000000 liblinear-official-2.46.1/cpp-source/linear.def
--rw-rw-rw-   0        0        0     2788 2023-02-15 08:40:58.000000 liblinear-official-2.46.1/cpp-source/linear.h
--rw-rw-rw-   0        0        0     5414 2023-02-15 08:40:58.000000 liblinear-official-2.46.1/cpp-source/newton.cpp
--rw-rw-rw-   0        0        0      925 2023-02-15 08:40:58.000000 liblinear-official-2.46.1/cpp-source/newton.h
-drwxrwxrwx   0        0        0        0 2023-02-17 08:33:01.021226 liblinear-official-2.46.1/liblinear/
--rw-rw-rw-   0        0        0        0 2023-02-15 08:14:49.000000 liblinear-official-2.46.1/liblinear/__init__.py
--rw-rw-rw-   0        0        0     6384 2023-02-15 08:14:49.000000 liblinear-official-2.46.1/liblinear/commonutil.py
--rw-rw-rw-   0        0        0    17313 2023-02-15 08:14:49.000000 liblinear-official-2.46.1/liblinear/liblinear.py
--rw-rw-rw-   0        0        0    11566 2023-02-15 08:14:49.000000 liblinear-official-2.46.1/liblinear/liblinearutil.py
-drwxrwxrwx   0        0        0        0 2023-02-17 08:33:01.046161 liblinear-official-2.46.1/liblinear_official.egg-info/
--rw-rw-rw-   0        0        0    18278 2023-02-17 08:33:00.000000 liblinear-official-2.46.1/liblinear_official.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      588 2023-02-17 08:33:00.000000 liblinear-official-2.46.1/liblinear_official.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-17 08:33:00.000000 liblinear-official-2.46.1/liblinear_official.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-02-17 08:33:00.000000 liblinear-official-2.46.1/liblinear_official.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-02-17 08:33:00.000000 liblinear-official-2.46.1/liblinear_official.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-17 08:33:01.049505 liblinear-official-2.46.1/setup.cfg
--rw-rw-rw-   0        0        0     3607 2023-02-17 08:32:57.000000 liblinear-official-2.46.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 10:57:28.742192 liblinear-official-2.47.0/
+-rw-rw-rw-   0        0        0     1517 2023-07-01 10:57:27.000000 liblinear-official-2.47.0/LICENSE
+-rw-rw-rw-   0        0        0       48 2023-06-30 12:14:25.000000 liblinear-official-2.47.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    18278 2023-07-01 10:57:28.739819 liblinear-official-2.47.0/PKG-INFO
+-rw-rw-rw-   0        0        0    17947 2023-07-01 10:53:11.000000 liblinear-official-2.47.0/README
+drwxrwxrwx   0        0        0        0 2023-07-01 10:57:28.507650 liblinear-official-2.47.0/cpp-source/
+drwxrwxrwx   0        0        0        0 2023-07-01 10:57:28.546659 liblinear-official-2.47.0/cpp-source/blas/
+-rw-rw-rw-   0        0        0      727 2023-07-01 10:57:27.000000 liblinear-official-2.47.0/cpp-source/blas/blas.h
+-rw-rw-rw-   0        0        0    16959 2023-07-01 10:57:27.000000 liblinear-official-2.47.0/cpp-source/blas/blasp.h
+-rw-rw-rw-   0        0        0     1322 2023-07-01 10:57:27.000000 liblinear-official-2.47.0/cpp-source/blas/daxpy.c
+-rw-rw-rw-   0        0        0     1329 2023-07-01 10:57:27.000000 liblinear-official-2.47.0/cpp-source/blas/ddot.c
+-rw-rw-rw-   0        0        0     1427 2023-07-01 10:57:27.000000 liblinear-official-2.47.0/cpp-source/blas/dnrm2.c
+-rw-rw-rw-   0        0        0     1144 2023-07-01 10:57:27.000000 liblinear-official-2.47.0/cpp-source/blas/dscal.c
+-rw-rw-rw-   0        0        0    83989 2023-07-01 10:57:27.000000 liblinear-official-2.47.0/cpp-source/linear.cpp
+-rw-rw-rw-   0        0        0      526 2023-07-01 10:57:27.000000 liblinear-official-2.47.0/cpp-source/linear.def
+-rw-rw-rw-   0        0        0     2788 2023-07-01 10:57:27.000000 liblinear-official-2.47.0/cpp-source/linear.h
+-rw-rw-rw-   0        0        0     5414 2023-07-01 10:57:27.000000 liblinear-official-2.47.0/cpp-source/newton.cpp
+-rw-rw-rw-   0        0        0      925 2023-07-01 10:57:27.000000 liblinear-official-2.47.0/cpp-source/newton.h
+drwxrwxrwx   0        0        0        0 2023-07-01 10:57:28.598577 liblinear-official-2.47.0/liblinear/
+-rw-rw-rw-   0        0        0        0 2023-06-30 12:14:25.000000 liblinear-official-2.47.0/liblinear/__init__.py
+-rw-rw-rw-   0        0        0     6384 2023-06-30 12:14:25.000000 liblinear-official-2.47.0/liblinear/commonutil.py
+-rw-rw-rw-   0        0        0    17521 2023-07-01 10:53:11.000000 liblinear-official-2.47.0/liblinear/liblinear.py
+-rw-rw-rw-   0        0        0    11566 2023-07-01 10:53:11.000000 liblinear-official-2.47.0/liblinear/liblinearutil.py
+drwxrwxrwx   0        0        0        0 2023-07-01 10:57:28.737200 liblinear-official-2.47.0/liblinear_official.egg-info/
+-rw-rw-rw-   0        0        0    18278 2023-07-01 10:57:28.000000 liblinear-official-2.47.0/liblinear_official.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      588 2023-07-01 10:57:28.000000 liblinear-official-2.47.0/liblinear_official.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 10:57:28.000000 liblinear-official-2.47.0/liblinear_official.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-01 10:57:28.000000 liblinear-official-2.47.0/liblinear_official.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-01 10:57:28.000000 liblinear-official-2.47.0/liblinear_official.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 10:57:28.742192 liblinear-official-2.47.0/setup.cfg
+-rw-rw-rw-   0        0        0     3607 2023-07-01 10:53:11.000000 liblinear-official-2.47.0/setup.py
```

### Comparing `liblinear-official-2.46.1/LICENSE` & `liblinear-official-2.47.0/LICENSE`

 * *Files identical despite different names*

### Comparing `liblinear-official-2.46.1/PKG-INFO` & `liblinear-official-2.47.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liblinear-official
-Version: 2.46.1
+Version: 2.47.0
 Summary: Python binding of LIBLINEAR
 Home-page: https://www.csie.ntu.edu.tw/~cjlin/liblinear
 Author: ML group @ National Taiwan University
 Author-email: cjlin@csie.ntu.edu.tw
 License: BSD-3-Clause
 Description-Content-Type: text/plain
 License-File: LICENSE
```

### Comparing `liblinear-official-2.46.1/README` & `liblinear-official-2.47.0/README`

 * *Files identical despite different names*

### Comparing `liblinear-official-2.46.1/cpp-source/blas/blas.h` & `liblinear-official-2.47.0/cpp-source/blas/blas.h`

 * *Files identical despite different names*

### Comparing `liblinear-official-2.46.1/cpp-source/blas/blasp.h` & `liblinear-official-2.47.0/cpp-source/blas/blasp.h`

 * *Files identical despite different names*

### Comparing `liblinear-official-2.46.1/cpp-source/blas/daxpy.c` & `liblinear-official-2.47.0/cpp-source/blas/daxpy.c`

 * *Files identical despite different names*

### Comparing `liblinear-official-2.46.1/cpp-source/blas/ddot.c` & `liblinear-official-2.47.0/cpp-source/blas/ddot.c`

 * *Files identical despite different names*

### Comparing `liblinear-official-2.46.1/cpp-source/blas/dnrm2.c` & `liblinear-official-2.47.0/cpp-source/blas/dnrm2.c`

 * *Files identical despite different names*

### Comparing `liblinear-official-2.46.1/cpp-source/blas/dscal.c` & `liblinear-official-2.47.0/cpp-source/blas/dscal.c`

 * *Files identical despite different names*

### Comparing `liblinear-official-2.46.1/cpp-source/linear.cpp` & `liblinear-official-2.47.0/cpp-source/linear.cpp`

 * *Files identical despite different names*

### Comparing `liblinear-official-2.46.1/cpp-source/linear.def` & `liblinear-official-2.47.0/cpp-source/linear.def`

 * *Files identical despite different names*

### Comparing `liblinear-official-2.46.1/cpp-source/linear.h` & `liblinear-official-2.47.0/cpp-source/linear.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #ifndef _LIBLINEAR_H
 #define _LIBLINEAR_H
 
-#define LIBLINEAR_VERSION 246
+#define LIBLINEAR_VERSION 247
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 extern int liblinear_version;
```

### Comparing `liblinear-official-2.46.1/cpp-source/newton.cpp` & `liblinear-official-2.47.0/cpp-source/newton.cpp`

 * *Files identical despite different names*

### Comparing `liblinear-official-2.46.1/cpp-source/newton.h` & `liblinear-official-2.47.0/cpp-source/newton.h`

 * *Files identical despite different names*

### Comparing `liblinear-official-2.46.1/liblinear/commonutil.py` & `liblinear-official-2.47.0/liblinear/commonutil.py`

 * *Files identical despite different names*

### Comparing `liblinear-official-2.46.1/liblinear/liblinear.py` & `liblinear-official-2.47.0/liblinear/liblinear.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,17 @@
         prob_slice = slice(prob_rowptr[i], prob_rowptr[i+1]-2)
         prob_ind[prob_slice] = x_ind[x_slice]+1
         prob_val[prob_slice] = x_val[x_slice]
 
 def csr_to_problem(x, prob):
     # Extra space for termination node and (possibly) bias term
     x_space = prob.x_space = np.empty((x.nnz+x.shape[0]*2), dtype=feature_node)
-    prob.rowptr = x.indptr.copy()
+    # rowptr has to be a 64bit integer because it will later be used for pointer arithmetic,
+    # which overflows when the added pointer points to an address that is numerically high.
+    prob.rowptr = x.indptr.astype(np.int64, copy=True)
     prob.rowptr[1:] += 2*np.arange(1,x.shape[0]+1)
     prob_ind = x_space["index"]
     prob_val = x_space["value"]
     prob_ind[:] = -1
     if jit_enabled:
         csr_to_problem_jit(x.shape[0], x.data, x.indices, x.indptr, prob_val, prob_ind, prob.rowptr)
     else:
```

### Comparing `liblinear-official-2.46.1/liblinear/liblinearutil.py` & `liblinear-official-2.47.0/liblinear/liblinearutil.py`

 * *Files identical despite different names*

### Comparing `liblinear-official-2.46.1/liblinear_official.egg-info/PKG-INFO` & `liblinear-official-2.47.0/liblinear_official.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liblinear-official
-Version: 2.46.1
+Version: 2.47.0
 Summary: Python binding of LIBLINEAR
 Home-page: https://www.csie.ntu.edu.tw/~cjlin/liblinear
 Author: ML group @ National Taiwan University
 Author-email: cjlin@csie.ntu.edu.tw
 License: BSD-3-Clause
 Description-Content-Type: text/plain
 License-File: LICENSE
```

### Comparing `liblinear-official-2.46.1/liblinear_official.egg-info/SOURCES.txt` & `liblinear-official-2.47.0/liblinear_official.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liblinear-official-2.46.1/setup.py` & `liblinear-official-2.47.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from distutils.command.build_ext import build_ext
 
 build_ext.get_export_symbols = lambda x, y: []
 
 
 PACKAGE_DIR = "liblinear"
 PACKAGE_NAME = "liblinear-official"
-VERSION = "2.46.1"
+VERSION = "2.47.0"
 cpp_dir = "cpp-source"
 # should be consistent with dynamic_lib_name in liblinear/liblinear.py
 dynamic_lib_name = "clib"
 
 # sources to be included to build the shared library
 source_codes = [
     path.join("blas", "daxpy.c"),
```

