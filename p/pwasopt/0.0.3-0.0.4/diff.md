# Comparing `tmp/pwasopt-0.0.3.tar.gz` & `tmp/pwasopt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwasopt-0.0.3.tar", last modified: Sat Jul  1 10:23:25 2023, max compression
+gzip compressed data, was "pwasopt-0.0.4.tar", last modified: Sat Jul  1 16:51:25 2023, max compression
```

## Comparing `pwasopt-0.0.3.tar` & `pwasopt-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 10:23:25.862348 pwasopt-0.0.3/
--rw-rw-rw-   0        0        0    11527 2023-06-30 12:07:33.000000 pwasopt-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2669 2023-07-01 10:23:25.860349 pwasopt-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1940 2023-02-11 20:07:08.000000 pwasopt-0.0.3/README.md
--rw-rw-rw-   0        0        0      932 2023-07-01 10:15:04.000000 pwasopt-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-01 10:23:25.863349 pwasopt-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-01 10:23:25.782463 pwasopt-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-01 10:23:25.830743 pwasopt-0.0.3/src/pwasopt/
--rw-rw-rw-   0        0        0        0 2023-06-30 09:41:30.000000 pwasopt-0.0.3/src/pwasopt/__init__.py
--rw-rw-rw-   0        0        0    70455 2023-02-08 22:16:04.000000 pwasopt-0.0.3/src/pwasopt/acquisition.py
--rw-rw-rw-   0        0        0     2928 2023-02-08 22:16:44.000000 pwasopt-0.0.3/src/pwasopt/categorical_encoder.py
--rw-rw-rw-   0        0        0    14260 2023-02-08 22:16:44.000000 pwasopt-0.0.3/src/pwasopt/fit_surrogate_pwasp.py
--rw-rw-rw-   0        0        0     3273 2023-02-08 22:16:44.000000 pwasopt-0.0.3/src/pwasopt/integ_encoder.py
--rw-rw-rw-   0        0        0    21999 2023-07-01 10:21:56.000000 pwasopt-0.0.3/src/pwasopt/main_pwas.py
--rw-rw-rw-   0        0        0    22340 2023-07-01 10:21:50.000000 pwasopt-0.0.3/src/pwasopt/main_pwasp.py
--rw-rw-rw-   0        0        0     2773 2022-10-12 17:09:17.000000 pwasopt-0.0.3/src/pwasopt/pref_fun.py
--rw-rw-rw-   0        0        0     4205 2022-10-12 17:09:22.000000 pwasopt-0.0.3/src/pwasopt/pref_fun1.py
--rw-rw-rw-   0        0        0    12417 2023-06-30 12:36:24.000000 pwasopt-0.0.3/src/pwasopt/prob_setup.py
--rw-rw-rw-   0        0        0    30948 2023-06-30 12:36:24.000000 pwasopt-0.0.3/src/pwasopt/sample.py
-drwxrwxrwx   0        0        0        0 2023-07-01 10:23:25.855176 pwasopt-0.0.3/src/pwasopt.egg-info/
--rw-rw-rw-   0        0        0     2669 2023-07-01 10:23:25.000000 pwasopt-0.0.3/src/pwasopt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-07-01 10:23:25.000000 pwasopt-0.0.3/src/pwasopt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 10:23:25.000000 pwasopt-0.0.3/src/pwasopt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-07-01 10:23:25.000000 pwasopt-0.0.3/src/pwasopt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-01 10:23:25.000000 pwasopt-0.0.3/src/pwasopt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 16:51:25.957540 pwasopt-0.0.4/
+-rw-rw-rw-   0        0        0    11527 2023-06-30 12:07:33.000000 pwasopt-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0    16839 2023-07-01 16:51:25.957540 pwasopt-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    16110 2023-07-01 16:43:37.000000 pwasopt-0.0.4/README.md
+-rw-rw-rw-   0        0        0      932 2023-07-01 16:50:49.000000 pwasopt-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-01 16:51:25.957540 pwasopt-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-01 16:51:25.888530 pwasopt-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-01 16:51:25.941911 pwasopt-0.0.4/src/pwasopt/
+-rw-rw-rw-   0        0        0        0 2023-06-30 09:41:30.000000 pwasopt-0.0.4/src/pwasopt/__init__.py
+-rw-rw-rw-   0        0        0    70455 2023-02-08 22:16:04.000000 pwasopt-0.0.4/src/pwasopt/acquisition.py
+-rw-rw-rw-   0        0        0     2928 2023-02-08 22:16:44.000000 pwasopt-0.0.4/src/pwasopt/categorical_encoder.py
+-rw-rw-rw-   0        0        0    14260 2023-02-08 22:16:44.000000 pwasopt-0.0.4/src/pwasopt/fit_surrogate_pwasp.py
+-rw-rw-rw-   0        0        0     3273 2023-02-08 22:16:44.000000 pwasopt-0.0.4/src/pwasopt/integ_encoder.py
+-rw-rw-rw-   0        0        0    21999 2023-07-01 12:54:13.000000 pwasopt-0.0.4/src/pwasopt/main_pwas.py
+-rw-rw-rw-   0        0        0    22340 2023-07-01 12:53:59.000000 pwasopt-0.0.4/src/pwasopt/main_pwasp.py
+-rw-rw-rw-   0        0        0     2773 2022-10-12 17:09:17.000000 pwasopt-0.0.4/src/pwasopt/pref_fun.py
+-rw-rw-rw-   0        0        0     4205 2022-10-12 17:09:22.000000 pwasopt-0.0.4/src/pwasopt/pref_fun1.py
+-rw-rw-rw-   0        0        0    12417 2023-06-30 12:36:24.000000 pwasopt-0.0.4/src/pwasopt/prob_setup.py
+-rw-rw-rw-   0        0        0    30948 2023-06-30 12:36:24.000000 pwasopt-0.0.4/src/pwasopt/sample.py
+drwxrwxrwx   0        0        0        0 2023-07-01 16:51:25.957540 pwasopt-0.0.4/src/pwasopt.egg-info/
+-rw-rw-rw-   0        0        0    16839 2023-07-01 16:51:25.000000 pwasopt-0.0.4/src/pwasopt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-07-01 16:51:25.000000 pwasopt-0.0.4/src/pwasopt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 16:51:25.000000 pwasopt-0.0.4/src/pwasopt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-07-01 16:51:25.000000 pwasopt-0.0.4/src/pwasopt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-01 16:51:25.000000 pwasopt-0.0.4/src/pwasopt.egg-info/top_level.txt
```

### Comparing `pwasopt-0.0.3/LICENSE` & `pwasopt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.3/pyproject.toml` & `pwasopt-0.0.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pwasopt"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Mengjia Zhu", email="mengjia.zhu@imtlucca.it" },
   { name="Alberto Bemporad", email="alberto.bemporad@imtlucca.it" },
 ]
 description = "PWAS/PWASp - Global and Preference-based Optimization with Mixed Variables using (P)iece(w)ise (A)ffine (S)urrogates"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `pwasopt-0.0.3/src/pwasopt/acquisition.py` & `pwasopt-0.0.4/src/pwasopt/acquisition.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.3/src/pwasopt/categorical_encoder.py` & `pwasopt-0.0.4/src/pwasopt/categorical_encoder.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.3/src/pwasopt/fit_surrogate_pwasp.py` & `pwasopt-0.0.4/src/pwasopt/fit_surrogate_pwasp.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.3/src/pwasopt/integ_encoder.py` & `pwasopt-0.0.4/src/pwasopt/integ_encoder.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.3/src/pwasopt/main_pwas.py` & `pwasopt-0.0.4/src/pwasopt/main_pwas.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.3/src/pwasopt/main_pwasp.py` & `pwasopt-0.0.4/src/pwasopt/main_pwasp.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.3/src/pwasopt/pref_fun.py` & `pwasopt-0.0.4/src/pwasopt/pref_fun.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.3/src/pwasopt/pref_fun1.py` & `pwasopt-0.0.4/src/pwasopt/pref_fun1.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.3/src/pwasopt/prob_setup.py` & `pwasopt-0.0.4/src/pwasopt/prob_setup.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.3/src/pwasopt/sample.py` & `pwasopt-0.0.4/src/pwasopt/sample.py`

 * *Files identical despite different names*

