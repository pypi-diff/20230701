# Comparing `tmp/pyparc-2.0.2.tar.gz` & `tmp/pyparc-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyparc-2.0.2.tar", last modified: Sat Jul  1 07:13:32 2023, max compression
+gzip compressed data, was "pyparc-2.0.3.tar", last modified: Sat Jul  1 07:18:04 2023, max compression
```

## Comparing `pyparc-2.0.2.tar` & `pyparc-2.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-01 07:13:32.800077 pyparc-2.0.2/
--rw-r--r--   0 bemporad   (501) staff       (20)    11345 2023-01-10 10:53:45.000000 pyparc-2.0.2/LICENSE.txt
--rw-r--r--   0 bemporad   (501) staff       (20)     4524 2023-07-01 07:13:32.799950 pyparc-2.0.2/PKG-INFO
--rw-r--r--   0 bemporad   (501) staff       (20)     3894 2023-07-01 06:50:16.000000 pyparc-2.0.2/README.md
--rw-r--r--   0 bemporad   (501) staff       (20)      827 2023-07-01 07:12:01.000000 pyparc-2.0.2/pyproject.toml
--rw-r--r--   0 bemporad   (501) staff       (20)       38 2023-07-01 07:13:32.800115 pyparc-2.0.2/setup.cfg
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-01 07:13:32.798237 pyparc-2.0.2/src/
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-01 07:13:32.798952 pyparc-2.0.2/src/parc/
--rw-r--r--   0 bemporad   (501) staff       (20)        0 2023-01-10 11:29:35.000000 pyparc-2.0.2/src/parc/__init__.py
--rwxr-xr-x   0 bemporad   (501) staff       (20)    44973 2023-07-01 06:51:03.000000 pyparc-2.0.2/src/parc/parc.py
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-01 07:13:32.799621 pyparc-2.0.2/src/pyparc.egg-info/
--rw-r--r--   0 bemporad   (501) staff       (20)     4524 2023-07-01 07:13:32.000000 pyparc-2.0.2/src/pyparc.egg-info/PKG-INFO
--rw-r--r--   0 bemporad   (501) staff       (20)      262 2023-07-01 07:13:32.000000 pyparc-2.0.2/src/pyparc.egg-info/SOURCES.txt
--rw-r--r--   0 bemporad   (501) staff       (20)        1 2023-07-01 07:13:32.000000 pyparc-2.0.2/src/pyparc.egg-info/dependency_links.txt
--rw-r--r--   0 bemporad   (501) staff       (20)       66 2023-07-01 07:13:32.000000 pyparc-2.0.2/src/pyparc.egg-info/requires.txt
--rw-r--r--   0 bemporad   (501) staff       (20)        5 2023-07-01 07:13:32.000000 pyparc-2.0.2/src/pyparc.egg-info/top_level.txt
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-01 07:13:32.799764 pyparc-2.0.2/tests/
--rw-r--r--   0 bemporad   (501) staff       (20)     1326 2023-07-01 06:58:29.000000 pyparc-2.0.2/tests/test_parc.py
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-01 07:18:04.548613 pyparc-2.0.3/
+-rw-r--r--   0 bemporad   (501) staff       (20)    11345 2023-01-10 10:53:45.000000 pyparc-2.0.3/LICENSE.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)     4524 2023-07-01 07:18:04.548488 pyparc-2.0.3/PKG-INFO
+-rw-r--r--   0 bemporad   (501) staff       (20)     3894 2023-07-01 06:50:16.000000 pyparc-2.0.3/README.md
+-rw-r--r--   0 bemporad   (501) staff       (20)      827 2023-07-01 07:16:56.000000 pyparc-2.0.3/pyproject.toml
+-rw-r--r--   0 bemporad   (501) staff       (20)       38 2023-07-01 07:18:04.548654 pyparc-2.0.3/setup.cfg
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-01 07:18:04.546802 pyparc-2.0.3/src/
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-01 07:18:04.547584 pyparc-2.0.3/src/pyparc/
+-rw-r--r--   0 bemporad   (501) staff       (20)        0 2023-01-10 11:29:35.000000 pyparc-2.0.3/src/pyparc/__init__.py
+-rwxr-xr-x   0 bemporad   (501) staff       (20)    44973 2023-07-01 06:51:03.000000 pyparc-2.0.3/src/pyparc/parc.py
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-01 07:18:04.548199 pyparc-2.0.3/src/pyparc.egg-info/
+-rw-r--r--   0 bemporad   (501) staff       (20)     4524 2023-07-01 07:18:04.000000 pyparc-2.0.3/src/pyparc.egg-info/PKG-INFO
+-rw-r--r--   0 bemporad   (501) staff       (20)      266 2023-07-01 07:18:04.000000 pyparc-2.0.3/src/pyparc.egg-info/SOURCES.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)        1 2023-07-01 07:18:04.000000 pyparc-2.0.3/src/pyparc.egg-info/dependency_links.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)       66 2023-07-01 07:18:04.000000 pyparc-2.0.3/src/pyparc.egg-info/requires.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)        7 2023-07-01 07:18:04.000000 pyparc-2.0.3/src/pyparc.egg-info/top_level.txt
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2023-07-01 07:18:04.548318 pyparc-2.0.3/tests/
+-rw-r--r--   0 bemporad   (501) staff       (20)     1326 2023-07-01 06:58:29.000000 pyparc-2.0.3/tests/test_parc.py
```

### Comparing `pyparc-2.0.2/LICENSE.txt` & `pyparc-2.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyparc-2.0.2/PKG-INFO` & `pyparc-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyparc
-Version: 2.0.2
+Version: 2.0.3
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
-Metadata-Version: 2.1 Name: pyparc Version: 2.0.2 Summary: PARC - Piecewise
+Metadata-Version: 2.1 Name: pyparc Version: 2.0.3 Summary: PARC - Piecewise
 Affine Regression and Classification Author-email: Alberto Bemporad
 bemporad@imtlucca.it> Project-URL: Homepage, http://cse.lab.imtlucca.it/
 ~bemporad/parc Keywords: piecewise linear regression,piecewise linear
 classification,multivariate regression,multivariate classification,supervised
 learning Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `pyparc-2.0.2/README.md` & `pyparc-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyparc-2.0.2/pyproject.toml` & `pyparc-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyparc"
-version = "2.0.2"
+version = "2.0.3"
 authors = [
   { name="Alberto Bemporad", email="alberto.bemporad@imtlucca.it" },
 ]
 description = "PARC - Piecewise Affine Regression and Classification"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ["numpy","scipy","sklearn","matplotlib","pypoman","mip","faiss-cpu","pickle-mixin"]
```

### Comparing `pyparc-2.0.2/src/parc/parc.py` & `pyparc-2.0.3/src/pyparc/parc.py`

 * *Files identical despite different names*

### Comparing `pyparc-2.0.2/src/pyparc.egg-info/PKG-INFO` & `pyparc-2.0.3/src/pyparc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyparc
-Version: 2.0.2
+Version: 2.0.3
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
-Metadata-Version: 2.1 Name: pyparc Version: 2.0.2 Summary: PARC - Piecewise
+Metadata-Version: 2.1 Name: pyparc Version: 2.0.3 Summary: PARC - Piecewise
 Affine Regression and Classification Author-email: Alberto Bemporad
 bemporad@imtlucca.it> Project-URL: Homepage, http://cse.lab.imtlucca.it/
 ~bemporad/parc Keywords: piecewise linear regression,piecewise linear
 classification,multivariate regression,multivariate classification,supervised
 learning Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `pyparc-2.0.2/tests/test_parc.py` & `pyparc-2.0.3/tests/test_parc.py`

 * *Files identical despite different names*

