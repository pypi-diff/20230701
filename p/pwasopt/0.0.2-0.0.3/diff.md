# Comparing `tmp/pwasopt-0.0.2.tar.gz` & `tmp/pwasopt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwasopt-0.0.2.tar", last modified: Fri Jun 30 12:38:01 2023, max compression
+gzip compressed data, was "pwasopt-0.0.3.tar", last modified: Sat Jul  1 10:23:25 2023, max compression
```

## Comparing `pwasopt-0.0.2.tar` & `pwasopt-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 12:38:01.575028 pwasopt-0.0.2/
--rw-rw-rw-   0        0        0    11527 2023-06-30 12:07:33.000000 pwasopt-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2669 2023-06-30 12:38:01.575028 pwasopt-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1940 2023-02-11 20:07:08.000000 pwasopt-0.0.2/README.md
--rw-rw-rw-   0        0        0      923 2023-06-30 12:36:56.000000 pwasopt-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-30 12:38:01.575028 pwasopt-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-30 12:38:01.521623 pwasopt-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-30 12:38:01.559400 pwasopt-0.0.2/src/pwasopt/
--rw-rw-rw-   0        0        0        0 2023-06-30 09:41:30.000000 pwasopt-0.0.2/src/pwasopt/__init__.py
--rw-rw-rw-   0        0        0    70455 2023-02-08 22:16:04.000000 pwasopt-0.0.2/src/pwasopt/acquisition.py
--rw-rw-rw-   0        0        0     2928 2023-02-08 22:16:44.000000 pwasopt-0.0.2/src/pwasopt/categorical_encoder.py
--rw-rw-rw-   0        0        0    14260 2023-02-08 22:16:44.000000 pwasopt-0.0.2/src/pwasopt/fit_surrogate_pwasp.py
--rw-rw-rw-   0        0        0     3273 2023-02-08 22:16:44.000000 pwasopt-0.0.2/src/pwasopt/integ_encoder.py
--rw-rw-rw-   0        0        0    21920 2023-06-30 12:35:26.000000 pwasopt-0.0.2/src/pwasopt/main_pwas.py
--rw-rw-rw-   0        0        0    22232 2023-06-30 12:35:53.000000 pwasopt-0.0.2/src/pwasopt/main_pwasp.py
--rw-rw-rw-   0        0        0    44725 2022-05-24 21:25:29.000000 pwasopt-0.0.2/src/pwasopt/parc.py
--rw-rw-rw-   0        0        0     2773 2022-10-12 17:09:17.000000 pwasopt-0.0.2/src/pwasopt/pref_fun.py
--rw-rw-rw-   0        0        0     4205 2022-10-12 17:09:22.000000 pwasopt-0.0.2/src/pwasopt/pref_fun1.py
--rw-rw-rw-   0        0        0    12417 2023-06-30 12:36:24.000000 pwasopt-0.0.2/src/pwasopt/prob_setup.py
--rw-rw-rw-   0        0        0    30948 2023-06-30 12:36:24.000000 pwasopt-0.0.2/src/pwasopt/sample.py
-drwxrwxrwx   0        0        0        0 2023-06-30 12:38:01.559400 pwasopt-0.0.2/src/pwasopt.egg-info/
--rw-rw-rw-   0        0        0     2669 2023-06-30 12:38:01.000000 pwasopt-0.0.2/src/pwasopt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      524 2023-06-30 12:38:01.000000 pwasopt-0.0.2/src/pwasopt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 12:38:01.000000 pwasopt-0.0.2/src/pwasopt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-06-30 12:38:01.000000 pwasopt-0.0.2/src/pwasopt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-30 12:38:01.000000 pwasopt-0.0.2/src/pwasopt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 10:23:25.862348 pwasopt-0.0.3/
+-rw-rw-rw-   0        0        0    11527 2023-06-30 12:07:33.000000 pwasopt-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2669 2023-07-01 10:23:25.860349 pwasopt-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1940 2023-02-11 20:07:08.000000 pwasopt-0.0.3/README.md
+-rw-rw-rw-   0        0        0      932 2023-07-01 10:15:04.000000 pwasopt-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-01 10:23:25.863349 pwasopt-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-01 10:23:25.782463 pwasopt-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-01 10:23:25.830743 pwasopt-0.0.3/src/pwasopt/
+-rw-rw-rw-   0        0        0        0 2023-06-30 09:41:30.000000 pwasopt-0.0.3/src/pwasopt/__init__.py
+-rw-rw-rw-   0        0        0    70455 2023-02-08 22:16:04.000000 pwasopt-0.0.3/src/pwasopt/acquisition.py
+-rw-rw-rw-   0        0        0     2928 2023-02-08 22:16:44.000000 pwasopt-0.0.3/src/pwasopt/categorical_encoder.py
+-rw-rw-rw-   0        0        0    14260 2023-02-08 22:16:44.000000 pwasopt-0.0.3/src/pwasopt/fit_surrogate_pwasp.py
+-rw-rw-rw-   0        0        0     3273 2023-02-08 22:16:44.000000 pwasopt-0.0.3/src/pwasopt/integ_encoder.py
+-rw-rw-rw-   0        0        0    21999 2023-07-01 10:21:56.000000 pwasopt-0.0.3/src/pwasopt/main_pwas.py
+-rw-rw-rw-   0        0        0    22340 2023-07-01 10:21:50.000000 pwasopt-0.0.3/src/pwasopt/main_pwasp.py
+-rw-rw-rw-   0        0        0     2773 2022-10-12 17:09:17.000000 pwasopt-0.0.3/src/pwasopt/pref_fun.py
+-rw-rw-rw-   0        0        0     4205 2022-10-12 17:09:22.000000 pwasopt-0.0.3/src/pwasopt/pref_fun1.py
+-rw-rw-rw-   0        0        0    12417 2023-06-30 12:36:24.000000 pwasopt-0.0.3/src/pwasopt/prob_setup.py
+-rw-rw-rw-   0        0        0    30948 2023-06-30 12:36:24.000000 pwasopt-0.0.3/src/pwasopt/sample.py
+drwxrwxrwx   0        0        0        0 2023-07-01 10:23:25.855176 pwasopt-0.0.3/src/pwasopt.egg-info/
+-rw-rw-rw-   0        0        0     2669 2023-07-01 10:23:25.000000 pwasopt-0.0.3/src/pwasopt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-07-01 10:23:25.000000 pwasopt-0.0.3/src/pwasopt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 10:23:25.000000 pwasopt-0.0.3/src/pwasopt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-07-01 10:23:25.000000 pwasopt-0.0.3/src/pwasopt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-01 10:23:25.000000 pwasopt-0.0.3/src/pwasopt.egg-info/top_level.txt
```

### Comparing `pwasopt-0.0.2/LICENSE` & `pwasopt-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.2/PKG-INFO` & `pwasopt-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwasopt
-Version: 0.0.2
+Version: 0.0.3
 Summary: PWAS/PWASp - Global and Preference-based Optimization with Mixed Variables using (P)iece(w)ise (A)ffine (S)urrogates
 Author-email: Mengjia Zhu <mengjia.zhu@imtlucca.it>, Alberto Bemporad <alberto.bemporad@imtlucca.it>
 Project-URL: Homepage, https://github.com/mjzhu-p/PWAS
 Keywords: Mixed-variable optimization,Mixed-integer optimization,global optimization,preference-based optimization,black-box optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pwasopt-0.0.2/README.md` & `pwasopt-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.2/pyproject.toml` & `pwasopt-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pwasopt"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Mengjia Zhu", email="mengjia.zhu@imtlucca.it" },
   { name="Alberto Bemporad", email="alberto.bemporad@imtlucca.it" },
 ]
 description = "PWAS/PWASp - Global and Preference-based Optimization with Mixed Variables using (P)iece(w)ise (A)ffine (S)urrogates"
 readme = "README.md"
 requires-python = ">=3.7"
-dependencies = ["numpy","scipy","pulp","pyDOE","sklearn","pycddlib"]
+dependencies = ["numpy","scipy","pulp","pyDOE","sklearn","pycddlib","pyparc"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 keywords = ["Mixed-variable optimization","Mixed-integer optimization","global optimization", "preference-based optimization", "black-box optimization"]
```

### Comparing `pwasopt-0.0.2/src/pwasopt/acquisition.py` & `pwasopt-0.0.3/src/pwasopt/acquisition.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.2/src/pwasopt/categorical_encoder.py` & `pwasopt-0.0.3/src/pwasopt/categorical_encoder.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.2/src/pwasopt/fit_surrogate_pwasp.py` & `pwasopt-0.0.3/src/pwasopt/fit_surrogate_pwasp.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.2/src/pwasopt/integ_encoder.py` & `pwasopt-0.0.3/src/pwasopt/integ_encoder.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.2/src/pwasopt/main_pwas.py` & `pwasopt-0.0.3/src/pwasopt/main_pwas.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 PWAS -  Optimization with mixed variables using Piecewise Affine surrogate
 
 [1] M. Zhu and A. Bemporad, “Global and Preference-based Optimization
     with Mixed Variables using Piecewise Affine Surrogates,”
      arXiv preprint arXiv:2302.04686, 2023.
 
 reference code:
-                - parc.py by A. Bemporad, 2021, http://cse.lab.imtlucca.it/~bemporad/parc/
+                - PARC package by A. Bemporad, 2021, http://cse.lab.imtlucca.it/~bemporad/parc
                 - GLIS package by A.Bemporad & M. Zhu, 2023, https://github.com/bemporad/GLIS
 
 (C) 2021-2023 Mengjia Zhu, Alberto Bemporad
 """
 
-from pwasopt.parc import PARC
+from pyparc.parc import PARC # https://github.com/bemporad/PyPARC, https://pypi.org/project/pyparc/
 from pwasopt.prob_setup import *
 from pwasopt.sample import *
 from pwasopt.acquisition import *
 from pwasopt.categorical_encoder import *
 from pwasopt.integ_encoder import *
 
 import time
@@ -103,15 +103,15 @@
         scale_vars: bool
             if True, scale the continuous and integer variables to the range of [-1,1]
             if Flase, scaling is not performed
         shrink_range: bool
             if True, shrink the continuous and integer variables further according to the linear equality constraints
             if Flase, shrink range is not performed
 
-        PARC related parameters, see the definition in parc.py:
+        PARC related parameters, see the definition in PARC package:
             alpha, sigma, separation, maxiter, cost_tol, min_number, fit_on_partition, softmax_solver, softmax_maxiter, beta,
                 initialization, verbose, categorical
 
         timelimit: float
             maximum time allowed for the solver in PULP to solve the MILP/LP/MIP
         epsDeltaF: float
             the tolerance for the difference between function evaluations
```

### Comparing `pwasopt-0.0.2/src/pwasopt/main_pwasp.py` & `pwasopt-0.0.3/src/pwasopt/main_pwasp.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 PWASp -  Preference-based optimization with mixed variables using Piecewise Affine surrogate
 
 [1] M. Zhu and A. Bemporad, “Global and Preference-based Optimization
     with Mixed Variables using Piecewise Affine Surrogates,”
      arXiv preprint arXiv:2302.04686, 2023.
 
 reference code:
-                - parc.py by A. Bemporad, 2021, http://cse.lab.imtlucca.it/~bemporad/parc/
+                - PARC package by A. Bemporad, 2021, http://cse.lab.imtlucca.it/~bemporad/parc
                 - GLIS package by A.Bemporad & M. Zhu, 2023, https://github.com/bemporad/GLIS
 
 (C) 2021-2023 Mengjia Zhu, Alberto Bemporad
 """
 
 from pwasopt.prob_setup import *
 from pwasopt.sample import *
@@ -104,15 +104,16 @@
         scale_vars: bool
             if True, scale the continuous and integer variables to the range of [-1,1]
             if Flase, scaling is not performed
         shrink_range: bool
             if True, shrink the continuous and integer variables further according to the linear equality constraints
             if Flase, shrink range is not performed
 
-        PARC related parameters, see the definition in parc.py:
+        PARC related parameters, see the definition in PARC package:
+            Note: not used in PWASp, placeholder, used in PWAS, see main_pwas.py for more details
             alpha, sigma, separation, maxiter, cost_tol, min_number, fit_on_partition, softmax_solver, softmax_maxiter, beta,
                 initialization, verbose, categorical
 
         timelimit: float
             maximum time allowed for the solver in PULP to solve the MILP/LP/MIP
         epsDeltaF: float
             the tolerance for the difference bewtten function evaluations
```

### Comparing `pwasopt-0.0.2/src/pwasopt/pref_fun.py` & `pwasopt-0.0.3/src/pwasopt/pref_fun.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.2/src/pwasopt/pref_fun1.py` & `pwasopt-0.0.3/src/pwasopt/pref_fun1.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.2/src/pwasopt/prob_setup.py` & `pwasopt-0.0.3/src/pwasopt/prob_setup.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.2/src/pwasopt/sample.py` & `pwasopt-0.0.3/src/pwasopt/sample.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.2/src/pwasopt.egg-info/PKG-INFO` & `pwasopt-0.0.3/src/pwasopt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwasopt
-Version: 0.0.2
+Version: 0.0.3
 Summary: PWAS/PWASp - Global and Preference-based Optimization with Mixed Variables using (P)iece(w)ise (A)ffine (S)urrogates
 Author-email: Mengjia Zhu <mengjia.zhu@imtlucca.it>, Alberto Bemporad <alberto.bemporad@imtlucca.it>
 Project-URL: Homepage, https://github.com/mjzhu-p/PWAS
 Keywords: Mixed-variable optimization,Mixed-integer optimization,global optimization,preference-based optimization,black-box optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

