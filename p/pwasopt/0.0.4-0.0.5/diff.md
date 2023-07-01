# Comparing `tmp/pwasopt-0.0.4.tar.gz` & `tmp/pwasopt-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwasopt-0.0.4.tar", last modified: Sat Jul  1 16:51:25 2023, max compression
+gzip compressed data, was "pwasopt-0.0.5.tar", last modified: Sat Jul  1 21:32:37 2023, max compression
```

## Comparing `pwasopt-0.0.4.tar` & `pwasopt-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 16:51:25.957540 pwasopt-0.0.4/
--rw-rw-rw-   0        0        0    11527 2023-06-30 12:07:33.000000 pwasopt-0.0.4/LICENSE
--rw-rw-rw-   0        0        0    16839 2023-07-01 16:51:25.957540 pwasopt-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    16110 2023-07-01 16:43:37.000000 pwasopt-0.0.4/README.md
--rw-rw-rw-   0        0        0      932 2023-07-01 16:50:49.000000 pwasopt-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-01 16:51:25.957540 pwasopt-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-01 16:51:25.888530 pwasopt-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-01 16:51:25.941911 pwasopt-0.0.4/src/pwasopt/
--rw-rw-rw-   0        0        0        0 2023-06-30 09:41:30.000000 pwasopt-0.0.4/src/pwasopt/__init__.py
--rw-rw-rw-   0        0        0    70455 2023-02-08 22:16:04.000000 pwasopt-0.0.4/src/pwasopt/acquisition.py
--rw-rw-rw-   0        0        0     2928 2023-02-08 22:16:44.000000 pwasopt-0.0.4/src/pwasopt/categorical_encoder.py
--rw-rw-rw-   0        0        0    14260 2023-02-08 22:16:44.000000 pwasopt-0.0.4/src/pwasopt/fit_surrogate_pwasp.py
--rw-rw-rw-   0        0        0     3273 2023-02-08 22:16:44.000000 pwasopt-0.0.4/src/pwasopt/integ_encoder.py
--rw-rw-rw-   0        0        0    21999 2023-07-01 12:54:13.000000 pwasopt-0.0.4/src/pwasopt/main_pwas.py
--rw-rw-rw-   0        0        0    22340 2023-07-01 12:53:59.000000 pwasopt-0.0.4/src/pwasopt/main_pwasp.py
--rw-rw-rw-   0        0        0     2773 2022-10-12 17:09:17.000000 pwasopt-0.0.4/src/pwasopt/pref_fun.py
--rw-rw-rw-   0        0        0     4205 2022-10-12 17:09:22.000000 pwasopt-0.0.4/src/pwasopt/pref_fun1.py
--rw-rw-rw-   0        0        0    12417 2023-06-30 12:36:24.000000 pwasopt-0.0.4/src/pwasopt/prob_setup.py
--rw-rw-rw-   0        0        0    30948 2023-06-30 12:36:24.000000 pwasopt-0.0.4/src/pwasopt/sample.py
-drwxrwxrwx   0        0        0        0 2023-07-01 16:51:25.957540 pwasopt-0.0.4/src/pwasopt.egg-info/
--rw-rw-rw-   0        0        0    16839 2023-07-01 16:51:25.000000 pwasopt-0.0.4/src/pwasopt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-07-01 16:51:25.000000 pwasopt-0.0.4/src/pwasopt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 16:51:25.000000 pwasopt-0.0.4/src/pwasopt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-07-01 16:51:25.000000 pwasopt-0.0.4/src/pwasopt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-01 16:51:25.000000 pwasopt-0.0.4/src/pwasopt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 21:32:37.884184 pwasopt-0.0.5/
+-rw-rw-rw-   0        0        0    11527 2023-06-30 12:07:33.000000 pwasopt-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0    17149 2023-07-01 21:32:37.883185 pwasopt-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    16420 2023-07-01 21:20:12.000000 pwasopt-0.0.5/README.md
+-rw-rw-rw-   0        0        0      932 2023-07-01 21:22:06.000000 pwasopt-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-01 21:32:37.885185 pwasopt-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-01 21:32:37.817160 pwasopt-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-01 21:32:37.861154 pwasopt-0.0.5/src/pwasopt/
+-rw-rw-rw-   0        0        0        0 2023-06-30 09:41:30.000000 pwasopt-0.0.5/src/pwasopt/__init__.py
+-rw-rw-rw-   0        0        0    70455 2023-02-08 22:16:04.000000 pwasopt-0.0.5/src/pwasopt/acquisition.py
+-rw-rw-rw-   0        0        0     2928 2023-02-08 22:16:44.000000 pwasopt-0.0.5/src/pwasopt/categorical_encoder.py
+-rw-rw-rw-   0        0        0    14361 2023-07-01 21:17:48.000000 pwasopt-0.0.5/src/pwasopt/fit_surrogate_pwasp.py
+-rw-rw-rw-   0        0        0     3273 2023-02-08 22:16:44.000000 pwasopt-0.0.5/src/pwasopt/integ_encoder.py
+-rw-rw-rw-   0        0        0    21999 2023-07-01 12:54:13.000000 pwasopt-0.0.5/src/pwasopt/main_pwas.py
+-rw-rw-rw-   0        0        0    22340 2023-07-01 12:53:59.000000 pwasopt-0.0.5/src/pwasopt/main_pwasp.py
+-rw-rw-rw-   0        0        0     2773 2022-10-12 17:09:17.000000 pwasopt-0.0.5/src/pwasopt/pref_fun.py
+-rw-rw-rw-   0        0        0     4205 2022-10-12 17:09:22.000000 pwasopt-0.0.5/src/pwasopt/pref_fun1.py
+-rw-rw-rw-   0        0        0    12417 2023-06-30 12:36:24.000000 pwasopt-0.0.5/src/pwasopt/prob_setup.py
+-rw-rw-rw-   0        0        0    30948 2023-06-30 12:36:24.000000 pwasopt-0.0.5/src/pwasopt/sample.py
+drwxrwxrwx   0        0        0        0 2023-07-01 21:32:37.879407 pwasopt-0.0.5/src/pwasopt.egg-info/
+-rw-rw-rw-   0        0        0    17149 2023-07-01 21:32:37.000000 pwasopt-0.0.5/src/pwasopt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-07-01 21:32:37.000000 pwasopt-0.0.5/src/pwasopt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 21:32:37.000000 pwasopt-0.0.5/src/pwasopt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-07-01 21:32:37.000000 pwasopt-0.0.5/src/pwasopt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-01 21:32:37.000000 pwasopt-0.0.5/src/pwasopt.egg-info/top_level.txt
```

### Comparing `pwasopt-0.0.4/LICENSE` & `pwasopt-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.4/PKG-INFO` & `pwasopt-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwasopt
-Version: 0.0.4
+Version: 0.0.5
 Summary: PWAS/PWASp - Global and Preference-based Optimization with Mixed Variables using (P)iece(w)ise (A)ffine (S)urrogates
 Author-email: Mengjia Zhu <mengjia.zhu@imtlucca.it>, Alberto Bemporad <alberto.bemporad@imtlucca.it>
 Project-URL: Homepage, https://github.com/mjzhu-p/PWAS
 Keywords: Mixed-variable optimization,Mixed-integer optimization,global optimization,preference-based optimization,black-box optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -52,14 +52,18 @@
 * scipy
 * pulp
 * sklearn
 * [pyparc](https://pypi.org/project/pyparc/)
 * [pyDOE](https://pythonhosted.org/pyDOE/)
 * [pycddlib](https://pypi.org/project/pycddlib/)
 
+**Note**: PWAS/PWASp use `GUROBI` as the default solver to solve the MILP problem of acquisition optimization, 
+which is found to be the most robust during benchmark testing. Alternatively, we also include `GLPK`, which may introduce
+errors occasionally depending on the test problem and initial samples.
+
 
 <a name="basic-usage"></a>
 ## Basic usage
 
 ### Examples
 Examples of benchmark testing using PWAS/PWASp can be found in the `examples` folder:
 * `mixed_variable_benchmarks.py`: benchmark testing on constrained/unconstrained mixed-variable problems
```

### Comparing `pwasopt-0.0.4/README.md` & `pwasopt-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,18 @@
 * scipy
 * pulp
 * sklearn
 * [pyparc](https://pypi.org/project/pyparc/)
 * [pyDOE](https://pythonhosted.org/pyDOE/)
 * [pycddlib](https://pypi.org/project/pycddlib/)
 
+**Note**: PWAS/PWASp use `GUROBI` as the default solver to solve the MILP problem of acquisition optimization, 
+which is found to be the most robust during benchmark testing. Alternatively, we also include `GLPK`, which may introduce
+errors occasionally depending on the test problem and initial samples.
+
 
 <a name="basic-usage"></a>
 ## Basic usage
 
 ### Examples
 Examples of benchmark testing using PWAS/PWASp can be found in the `examples` folder:
 * `mixed_variable_benchmarks.py`: benchmark testing on constrained/unconstrained mixed-variable problems
```

### Comparing `pwasopt-0.0.4/pyproject.toml` & `pwasopt-0.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pwasopt"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Mengjia Zhu", email="mengjia.zhu@imtlucca.it" },
   { name="Alberto Bemporad", email="alberto.bemporad@imtlucca.it" },
 ]
 description = "PWAS/PWASp - Global and Preference-based Optimization with Mixed Variables using (P)iece(w)ise (A)ffine (S)urrogates"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `pwasopt-0.0.4/src/pwasopt/acquisition.py` & `pwasopt-0.0.5/src/pwasopt/acquisition.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.4/src/pwasopt/categorical_encoder.py` & `pwasopt-0.0.5/src/pwasopt/categorical_encoder.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.4/src/pwasopt/fit_surrogate_pwasp.py` & `pwasopt-0.0.5/src/pwasopt/fit_surrogate_pwasp.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,16 +105,18 @@
         for j in range(K):
             prob_param += reg_para >= -b[j]
             prob_param += reg_para >= b[j]
             for i in range(nvars_encoded):
                 prob_param += reg_para >= -a[j][i]
                 prob_param += reg_para >= a[j][i]
 
-
-        prob_param.solve(plp.GUROBI(timeLimit=timelimit, msg=0))
+        try:
+            prob_param.solve(plp.GUROBI(timeLimit=timelimit, msg=0))
+        except:
+            prob_param.solve(plp.GLPK(timeLimit=timelimit, msg=0))
 
         status = prob_param.status
 
         if status == plp.LpStatusOptimal:  # See plp.constants.LpStatus. See more in constants.py in pulp/ folder
             a_opt = np.zeros((K, nvars_encoded, 1))
             b_opt = np.zeros((K, 1))
             y_pred_opt = np.zeros((N, 1))
```

### Comparing `pwasopt-0.0.4/src/pwasopt/integ_encoder.py` & `pwasopt-0.0.5/src/pwasopt/integ_encoder.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.4/src/pwasopt/main_pwas.py` & `pwasopt-0.0.5/src/pwasopt/main_pwas.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.4/src/pwasopt/main_pwasp.py` & `pwasopt-0.0.5/src/pwasopt/main_pwasp.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.4/src/pwasopt/pref_fun.py` & `pwasopt-0.0.5/src/pwasopt/pref_fun.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.4/src/pwasopt/pref_fun1.py` & `pwasopt-0.0.5/src/pwasopt/pref_fun1.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.4/src/pwasopt/prob_setup.py` & `pwasopt-0.0.5/src/pwasopt/prob_setup.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.4/src/pwasopt/sample.py` & `pwasopt-0.0.5/src/pwasopt/sample.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.4/src/pwasopt.egg-info/PKG-INFO` & `pwasopt-0.0.5/src/pwasopt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwasopt
-Version: 0.0.4
+Version: 0.0.5
 Summary: PWAS/PWASp - Global and Preference-based Optimization with Mixed Variables using (P)iece(w)ise (A)ffine (S)urrogates
 Author-email: Mengjia Zhu <mengjia.zhu@imtlucca.it>, Alberto Bemporad <alberto.bemporad@imtlucca.it>
 Project-URL: Homepage, https://github.com/mjzhu-p/PWAS
 Keywords: Mixed-variable optimization,Mixed-integer optimization,global optimization,preference-based optimization,black-box optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -52,14 +52,18 @@
 * scipy
 * pulp
 * sklearn
 * [pyparc](https://pypi.org/project/pyparc/)
 * [pyDOE](https://pythonhosted.org/pyDOE/)
 * [pycddlib](https://pypi.org/project/pycddlib/)
 
+**Note**: PWAS/PWASp use `GUROBI` as the default solver to solve the MILP problem of acquisition optimization, 
+which is found to be the most robust during benchmark testing. Alternatively, we also include `GLPK`, which may introduce
+errors occasionally depending on the test problem and initial samples.
+
 
 <a name="basic-usage"></a>
 ## Basic usage
 
 ### Examples
 Examples of benchmark testing using PWAS/PWASp can be found in the `examples` folder:
 * `mixed_variable_benchmarks.py`: benchmark testing on constrained/unconstrained mixed-variable problems
```

