# Comparing `tmp/genetic-algo-0.0.3.tar.gz` & `tmp/genetic-algo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genetic-algo-0.0.3.tar", last modified: Tue Jun 20 18:49:39 2023, max compression
+gzip compressed data, was "genetic-algo-0.0.4.tar", last modified: Sat Jul  1 09:06:03 2023, max compression
```

## Comparing `genetic-algo-0.0.3.tar` & `genetic-algo-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 18:49:39.462435 genetic-algo-0.0.3/
--rw-rw-rw-   0        0        0      115 2023-06-20 18:49:39.000000 genetic-algo-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2066 2023-06-20 18:49:39.461435 genetic-algo-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1255 2023-05-28 10:00:20.000000 genetic-algo-0.0.3/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 genetic-algo-0.0.3/build.py
-drwxrwxrwx   0        0        0        0 2023-06-20 18:49:39.444844 genetic-algo-0.0.3/genetic_algo/
--rw-rw-rw-   0        0        0     8934 2023-06-20 16:13:53.000000 genetic-algo-0.0.3/genetic_algo/attributes.py
--rw-rw-rw-   0        0        0     5518 2023-05-28 10:08:23.000000 genetic-algo-0.0.3/genetic_algo/base.py
--rw-rw-rw-   0        0        0      448 2023-06-03 06:46:07.000000 genetic-algo-0.0.3/genetic_algo/document.py
--rw-rw-rw-   0        0        0     5955 2023-06-03 06:57:31.000000 genetic-algo-0.0.3/genetic_algo/driver.py
--rw-rw-rw-   0        0        0    15381 2023-06-18 09:15:27.000000 genetic-algo-0.0.3/genetic_algo/environment.py
--rw-rw-rw-   0        0        0     4841 2023-06-20 18:47:51.000000 genetic-algo-0.0.3/genetic_algo/solution.py
-drwxrwxrwx   0        0        0        0 2023-06-20 18:49:39.460435 genetic-algo-0.0.3/genetic_algo.egg-info/
--rw-rw-rw-   0        0        0     2066 2023-06-20 18:49:39.000000 genetic-algo-0.0.3/genetic_algo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2023-06-20 18:49:39.000000 genetic-algo-0.0.3/genetic_algo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 18:49:39.000000 genetic-algo-0.0.3/genetic_algo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 18:49:39.000000 genetic-algo-0.0.3/genetic_algo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-20 18:49:39.000000 genetic-algo-0.0.3/genetic_algo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      645 2023-06-20 18:49:39.000000 genetic-algo-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       38 2023-06-18 08:47:03.000000 genetic-algo-0.0.3/requirements-dev.txt
--rw-rw-rw-   0        0        0       29 2023-06-18 08:47:03.000000 genetic-algo-0.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 18:49:39.462435 genetic-algo-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1601 2023-06-20 18:49:27.000000 genetic-algo-0.0.3/setup.py
--rw-rw-rw-   0        0        0     2645 2023-06-03 07:02:29.000000 genetic-algo-0.0.3/test.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:06:03.698225 genetic-algo-0.0.4/
+-rw-rw-rw-   0        0        0      115 2023-07-01 09:06:03.000000 genetic-algo-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2040 2023-07-01 09:06:03.698225 genetic-algo-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1229 2023-07-01 09:05:38.000000 genetic-algo-0.0.4/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 genetic-algo-0.0.4/build.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:06:03.688228 genetic-algo-0.0.4/genetic_algo/
+-rw-rw-rw-   0        0        0     8934 2023-06-20 16:13:53.000000 genetic-algo-0.0.4/genetic_algo/attributes.py
+-rw-rw-rw-   0        0        0     5955 2023-06-03 06:57:31.000000 genetic-algo-0.0.4/genetic_algo/driver.py
+-rw-rw-rw-   0        0        0    15381 2023-06-18 09:15:27.000000 genetic-algo-0.0.4/genetic_algo/environment.py
+-rw-rw-rw-   0        0        0     4841 2023-06-20 18:47:51.000000 genetic-algo-0.0.4/genetic_algo/solution.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:06:03.697224 genetic-algo-0.0.4/genetic_algo.egg-info/
+-rw-rw-rw-   0        0        0     2040 2023-07-01 09:06:03.000000 genetic-algo-0.0.4/genetic_algo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      382 2023-07-01 09:06:03.000000 genetic-algo-0.0.4/genetic_algo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 09:06:03.000000 genetic-algo-0.0.4/genetic_algo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 09:06:03.000000 genetic-algo-0.0.4/genetic_algo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-01 09:06:03.000000 genetic-algo-0.0.4/genetic_algo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      645 2023-07-01 09:06:03.000000 genetic-algo-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       38 2023-06-18 08:47:03.000000 genetic-algo-0.0.4/requirements-dev.txt
+-rw-rw-rw-   0        0        0       29 2023-06-18 08:47:03.000000 genetic-algo-0.0.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 09:06:03.699241 genetic-algo-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1601 2023-07-01 09:05:58.000000 genetic-algo-0.0.4/setup.py
+-rw-rw-rw-   0        0        0     2645 2023-06-03 07:02:29.000000 genetic-algo-0.0.4/test.py
```

### Comparing `genetic-algo-0.0.3/PKG-INFO` & `genetic-algo-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genetic-algo
-Version: 0.0.3
+Version: 0.0.4
 Summary: A framework for developing Genetic-Algorithm programs to solve problems dynamically and explicitly.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -25,15 +25,14 @@
 first of all
 ------------
 
 #### specifics:
 
 - writen and owned by: Shahaf Frank-Shapir
 - all the rights are saved for: Shahaf Frank-Shapir
-- program version: 0.0.0
 - programming languages: python 3.9.12 (100%)
 
 before we start
 ---------------
 
 #### description:
```

### Comparing `genetic-algo-0.0.3/README.md` & `genetic-algo-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 first of all
 ------------
 
 #### specifics:
 
 - writen and owned by: Shahaf Frank-Shapir
 - all the rights are saved for: Shahaf Frank-Shapir
-- program version: 0.0.0
 - programming languages: python 3.9.12 (100%)
 
 before we start
 ---------------
 
 #### description:
```

### Comparing `genetic-algo-0.0.3/build.py` & `genetic-algo-0.0.4/build.py`

 * *Files identical despite different names*

### Comparing `genetic-algo-0.0.3/genetic_algo/attributes.py` & `genetic-algo-0.0.4/genetic_algo/attributes.py`

 * *Files identical despite different names*

### Comparing `genetic-algo-0.0.3/genetic_algo/driver.py` & `genetic-algo-0.0.4/genetic_algo/driver.py`

 * *Files identical despite different names*

### Comparing `genetic-algo-0.0.3/genetic_algo/environment.py` & `genetic-algo-0.0.4/genetic_algo/environment.py`

 * *Files identical despite different names*

### Comparing `genetic-algo-0.0.3/genetic_algo/solution.py` & `genetic-algo-0.0.4/genetic_algo/solution.py`

 * *Files identical despite different names*

### Comparing `genetic-algo-0.0.3/genetic_algo.egg-info/PKG-INFO` & `genetic-algo-0.0.4/genetic_algo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genetic-algo
-Version: 0.0.3
+Version: 0.0.4
 Summary: A framework for developing Genetic-Algorithm programs to solve problems dynamically and explicitly.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -25,15 +25,14 @@
 first of all
 ------------
 
 #### specifics:
 
 - writen and owned by: Shahaf Frank-Shapir
 - all the rights are saved for: Shahaf Frank-Shapir
-- program version: 0.0.0
 - programming languages: python 3.9.12 (100%)
 
 before we start
 ---------------
 
 #### description:
```

### Comparing `genetic-algo-0.0.3/pyproject.toml` & `genetic-algo-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'genetic-algo'
-version = '0.0.3'
+version = '0.0.4'
 description = 'A framework for developing Genetic-Algorithm programs to solve problems dynamically and explicitly.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `genetic-algo-0.0.3/setup.py` & `genetic-algo-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "test.py"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='genetic-algo',
-        version='0.0.3',
+        version='0.0.4',
         description=(
             "A framework for developing Genetic-Algorithm "
             "programs to solve problems dynamically and explicitly."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

### Comparing `genetic-algo-0.0.3/test.py` & `genetic-algo-0.0.4/test.py`

 * *Files identical despite different names*

