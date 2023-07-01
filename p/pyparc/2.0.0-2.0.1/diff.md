# Comparing `tmp/pyparc-2.0.0.tar.gz` & `tmp/pyparc-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyparc-2.0.0.tar", last modified: Sat Jul  1 07:04:54 2023, max compression
+gzip compressed data, was "pyparc-2.0.1.tar", last modified: Sat Jul  1 07:10:22 2023, max compression
```

## Comparing `pyparc-2.0.0.tar` & `pyparc-2.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-01 07:04:54.708891 pyparc-2.0.0/
--rw-r--r--   0 bemporad   (501) staff       (20)    11345 2023-01-10 10:53:45.000000 pyparc-2.0.0/LICENSE.txt
--rw-r--r--   0 bemporad   (501) staff       (20)     4524 2023-07-01 07:04:54.708776 pyparc-2.0.0/PKG-INFO
--rw-r--r--   0 bemporad   (501) staff       (20)     3894 2023-07-01 06:50:16.000000 pyparc-2.0.0/README.md
--rw-r--r--   0 bemporad   (501) staff       (20)      817 2023-07-01 07:04:35.000000 pyparc-2.0.0/pyproject.toml
--rw-r--r--   0 bemporad   (501) staff       (20)       38 2023-07-01 07:04:54.708928 pyparc-2.0.0/setup.cfg
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-01 07:04:54.707262 pyparc-2.0.0/src/
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-01 07:04:54.707920 pyparc-2.0.0/src/parc/
--rw-r--r--   0 bemporad   (501) staff       (20)        0 2023-01-10 11:29:35.000000 pyparc-2.0.0/src/parc/__init__.py
--rwxr-xr-x   0 bemporad   (501) staff       (20)    44973 2023-07-01 06:51:03.000000 pyparc-2.0.0/src/parc/parc.py
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-01 07:04:54.708501 pyparc-2.0.0/src/pyparc.egg-info/
--rw-r--r--   0 bemporad   (501) staff       (20)     4524 2023-07-01 07:04:54.000000 pyparc-2.0.0/src/pyparc.egg-info/PKG-INFO
--rw-r--r--   0 bemporad   (501) staff       (20)      262 2023-07-01 07:04:54.000000 pyparc-2.0.0/src/pyparc.egg-info/SOURCES.txt
--rw-r--r--   0 bemporad   (501) staff       (20)        1 2023-07-01 07:04:54.000000 pyparc-2.0.0/src/pyparc.egg-info/dependency_links.txt
--rw-r--r--   0 bemporad   (501) staff       (20)       56 2023-07-01 07:04:54.000000 pyparc-2.0.0/src/pyparc.egg-info/requires.txt
--rw-r--r--   0 bemporad   (501) staff       (20)        5 2023-07-01 07:04:54.000000 pyparc-2.0.0/src/pyparc.egg-info/top_level.txt
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-01 07:04:54.708629 pyparc-2.0.0/tests/
--rw-r--r--   0 bemporad   (501) staff       (20)     1326 2023-07-01 06:58:29.000000 pyparc-2.0.0/tests/test_parc.py
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-01 07:10:22.408552 pyparc-2.0.1/
+-rw-r--r--   0 bemporad   (501) staff       (20)    11345 2023-01-10 10:53:45.000000 pyparc-2.0.1/LICENSE.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)     4524 2023-07-01 07:10:22.408435 pyparc-2.0.1/PKG-INFO
+-rw-r--r--   0 bemporad   (501) staff       (20)     3894 2023-07-01 06:50:16.000000 pyparc-2.0.1/README.md
+-rw-r--r--   0 bemporad   (501) staff       (20)      821 2023-07-01 07:09:35.000000 pyparc-2.0.1/pyproject.toml
+-rw-r--r--   0 bemporad   (501) staff       (20)       38 2023-07-01 07:10:22.408588 pyparc-2.0.1/setup.cfg
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-01 07:10:22.406913 pyparc-2.0.1/src/
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-01 07:10:22.407547 pyparc-2.0.1/src/parc/
+-rw-r--r--   0 bemporad   (501) staff       (20)        0 2023-01-10 11:29:35.000000 pyparc-2.0.1/src/parc/__init__.py
+-rwxr-xr-x   0 bemporad   (501) staff       (20)    44973 2023-07-01 06:51:03.000000 pyparc-2.0.1/src/parc/parc.py
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-01 07:10:22.408166 pyparc-2.0.1/src/pyparc.egg-info/
+-rw-r--r--   0 bemporad   (501) staff       (20)     4524 2023-07-01 07:10:22.000000 pyparc-2.0.1/src/pyparc.egg-info/PKG-INFO
+-rw-r--r--   0 bemporad   (501) staff       (20)      262 2023-07-01 07:10:22.000000 pyparc-2.0.1/src/pyparc.egg-info/SOURCES.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)        1 2023-07-01 07:10:22.000000 pyparc-2.0.1/src/pyparc.egg-info/dependency_links.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)       60 2023-07-01 07:10:22.000000 pyparc-2.0.1/src/pyparc.egg-info/requires.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)        5 2023-07-01 07:10:22.000000 pyparc-2.0.1/src/pyparc.egg-info/top_level.txt
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-01 07:10:22.408279 pyparc-2.0.1/tests/
+-rw-r--r--   0 bemporad   (501) staff       (20)     1326 2023-07-01 06:58:29.000000 pyparc-2.0.1/tests/test_parc.py
```

### Comparing `pyparc-2.0.0/LICENSE.txt` & `pyparc-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyparc-2.0.0/PKG-INFO` & `pyparc-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyparc
-Version: 2.0.0
+Version: 2.0.1
 Summary: PARC - Piecewise Affine Regression and Classification
 Author-email: Alberto Bemporad <alberto.bemporad@imtlucca.it>
 Project-URL: Homepage, http://cse.lab.imtlucca.it/~bemporad/parc
 Keywords: piecewise linear regression,piecewise linear classification,multivariate regression,multivariate classification,supervised learning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyparc Version: 2.0.0 Summary: PARC - Piecewise
+Metadata-Version: 2.1 Name: pyparc Version: 2.0.1 Summary: PARC - Piecewise
 Affine Regression and Classification Author-email: Alberto Bemporad
 bemporad@imtlucca.it> Project-URL: Homepage, http://cse.lab.imtlucca.it/
 ~bemporad/parc Keywords: piecewise linear regression,piecewise linear
 classification,multivariate regression,multivariate classification,supervised
 learning Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `pyparc-2.0.0/README.md` & `pyparc-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyparc-2.0.0/pyproject.toml` & `pyparc-2.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyparc"
-version = "2.0.0"
+version = "2.0.1"
 authors = [
   { name="Alberto Bemporad", email="alberto.bemporad@imtlucca.it" },
 ]
 description = "PARC - Piecewise Affine Regression and Classification"
 readme = "README.md"
 requires-python = ">=3.7"
-dependencies = ["numpy","scipy","sklearn","matplotlib","pypoman","mip","faiss","pickle"]
+dependencies = ["numpy","scipy","sklearn","matplotlib","pypoman","mip","faiss-cpu","pickle"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 keywords = ["piecewise linear regression", "piecewise linear classification",
     "multivariate regression", "multivariate classification", "supervised learning"]
```

### Comparing `pyparc-2.0.0/src/parc/parc.py` & `pyparc-2.0.1/src/parc/parc.py`

 * *Files identical despite different names*

### Comparing `pyparc-2.0.0/src/pyparc.egg-info/PKG-INFO` & `pyparc-2.0.1/src/pyparc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyparc
-Version: 2.0.0
+Version: 2.0.1
 Summary: PARC - Piecewise Affine Regression and Classification
 Author-email: Alberto Bemporad <alberto.bemporad@imtlucca.it>
 Project-URL: Homepage, http://cse.lab.imtlucca.it/~bemporad/parc
 Keywords: piecewise linear regression,piecewise linear classification,multivariate regression,multivariate classification,supervised learning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyparc Version: 2.0.0 Summary: PARC - Piecewise
+Metadata-Version: 2.1 Name: pyparc Version: 2.0.1 Summary: PARC - Piecewise
 Affine Regression and Classification Author-email: Alberto Bemporad
 bemporad@imtlucca.it> Project-URL: Homepage, http://cse.lab.imtlucca.it/
 ~bemporad/parc Keywords: piecewise linear regression,piecewise linear
 classification,multivariate regression,multivariate classification,supervised
 learning Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `pyparc-2.0.0/tests/test_parc.py` & `pyparc-2.0.1/tests/test_parc.py`

 * *Files identical despite different names*

