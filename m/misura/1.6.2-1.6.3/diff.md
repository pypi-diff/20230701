# Comparing `tmp/misura-1.6.2.tar.gz` & `tmp/misura-1.6.3.tar.gz`

## Comparing `misura-1.6.2.tar` & `misura-1.6.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 misura-1.6.2/.gitattributes
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 misura-1.6.2/Makefile
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 misura-1.6.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 misura-1.6.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 misura-1.6.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 misura-1.6.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 misura-1.6.2/src/test.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 misura-1.6.2/src/misura/__init__.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 misura-1.6.2/src/misura/__main__.py
--rw-r--r--   0        0        0     4223 2020-02-02 00:00:00.000000 misura-1.6.2/src/misura/currencies.py
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 misura-1.6.2/src/misura/exceptions.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 misura-1.6.2/src/misura/globals.py
--rw-r--r--   0        0        0    25362 2020-02-02 00:00:00.000000 misura-1.6.2/src/misura/quantities.py
--rw-r--r--   0        0        0    21416 2020-02-02 00:00:00.000000 misura-1.6.2/src/misura/tables.py
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 misura-1.6.2/src/misura/utilities.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 misura-1.6.2/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 misura-1.6.2/LICENSE
--rw-r--r--   0        0        0     7196 2020-02-02 00:00:00.000000 misura-1.6.2/README.md
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 misura-1.6.2/pyproject.toml
--rw-r--r--   0        0        0     7919 2020-02-02 00:00:00.000000 misura-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 misura-1.6.3/.gitattributes
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 misura-1.6.3/Makefile
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 misura-1.6.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 misura-1.6.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 misura-1.6.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 misura-1.6.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 misura-1.6.3/src/test.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 misura-1.6.3/src/misura/__init__.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 misura-1.6.3/src/misura/__main__.py
+-rw-r--r--   0        0        0     4223 2020-02-02 00:00:00.000000 misura-1.6.3/src/misura/currencies.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 misura-1.6.3/src/misura/exceptions.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 misura-1.6.3/src/misura/globals.py
+-rw-r--r--   0        0        0    25362 2020-02-02 00:00:00.000000 misura-1.6.3/src/misura/quantities.py
+-rw-r--r--   0        0        0    21416 2020-02-02 00:00:00.000000 misura-1.6.3/src/misura/tables.py
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 misura-1.6.3/src/misura/utilities.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 misura-1.6.3/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 misura-1.6.3/LICENSE
+-rw-r--r--   0        0        0     7162 2020-02-02 00:00:00.000000 misura-1.6.3/README.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 misura-1.6.3/pyproject.toml
+-rw-r--r--   0        0        0     7859 2020-02-02 00:00:00.000000 misura-1.6.3/PKG-INFO
```

### Comparing `misura-1.6.2/.github/ISSUE_TEMPLATE/feature_request.md` & `misura-1.6.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `misura-1.6.2/.github/workflows/python-publish.yml` & `misura-1.6.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `misura-1.6.2/src/test.py` & `misura-1.6.3/src/test.py`

 * *Files identical despite different names*

### Comparing `misura-1.6.2/src/misura/currencies.py` & `misura-1.6.3/src/misura/currencies.py`

 * *Files identical despite different names*

### Comparing `misura-1.6.2/src/misura/exceptions.py` & `misura-1.6.3/src/misura/exceptions.py`

 * *Files identical despite different names*

### Comparing `misura-1.6.2/src/misura/quantities.py` & `misura-1.6.3/src/misura/quantities.py`

 * *Files identical despite different names*

### Comparing `misura-1.6.2/src/misura/tables.py` & `misura-1.6.3/src/misura/tables.py`

 * *Files identical despite different names*

### Comparing `misura-1.6.2/src/misura/utilities.py` & `misura-1.6.3/src/misura/utilities.py`

 * *Files identical despite different names*

### Comparing `misura-1.6.2/LICENSE` & `misura-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `misura-1.6.2/README.md` & `misura-1.6.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -56,22 +56,20 @@
 
 By:
 
 ```
 python -m misura
 ```
 
-you'll be able to verify the installation of **misura** along getting some informations about the library[^1]:
-
-[^1]: Example referring to version 1.6.0
+you'll be able to verify the installation of **misura** along getting some informations about the library:
 
 ```
-misura v1.6.0
+misura
 
-Python library for easy unit handling and conversion for scientific & engineering applications.
+Python library providing effortless unit handling and currency conversion for scientific and engineering purposes.
 
 Developed by Andrea Di Antonio, more on https://github.com/diantonioandrea/misura
 Documentation on https://misura.diantonioandrea.com
 Bug tracker on https://github.com/diantonioandrea/misura/issues
 ```
 
 ### Importing misura
```

### Comparing `misura-1.6.2/pyproject.toml` & `misura-1.6.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "misura"
-version = "1.6.2"
+version = "1.6.3"
 authors = [
   { name="Andrea Di Antonio", email="mail@diantonioandrea.com" },
 ]
 description = "Python library for easy unit handling and conversion for scientific & engineering applications."
 readme = "README.md"
 requires-python = ">=3.7"
-dependencies = ["colorama", "setuptools", "requests"]
+dependencies = ["colorama", "requests"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `misura-1.6.2/PKG-INFO` & `misura-1.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: misura
-Version: 1.6.2
+Version: 1.6.3
 Summary: Python library for easy unit handling and conversion for scientific & engineering applications.
 Project-URL: Homepage, https://github.com/diantonioandrea/misura
 Project-URL: Documentation, https://misura.diantonioandrea.com
 Project-URL: Bug Tracker, https://github.com/diantonioandrea/misura/issues
 Author-email: Andrea Di Antonio <mail@diantonioandrea.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: colorama
 Requires-Dist: requests
-Requires-Dist: setuptools
 Description-Content-Type: text/markdown
 
 ![GitHub](https://img.shields.io/github/license/diantonioandrea/misura)
 
 ![PyPI](https://img.shields.io/pypi/v/misura?label=misura%20on%20pypi)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/misura)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/misura)
@@ -74,22 +73,20 @@
 
 By:
 
 ```
 python -m misura
 ```
 
-you'll be able to verify the installation of **misura** along getting some informations about the library[^1]:
-
-[^1]: Example referring to version 1.6.0
+you'll be able to verify the installation of **misura** along getting some informations about the library:
 
 ```
-misura v1.6.0
+misura
 
-Python library for easy unit handling and conversion for scientific & engineering applications.
+Python library providing effortless unit handling and currency conversion for scientific and engineering purposes.
 
 Developed by Andrea Di Antonio, more on https://github.com/diantonioandrea/misura
 Documentation on https://misura.diantonioandrea.com
 Bug tracker on https://github.com/diantonioandrea/misura/issues
 ```
 
 ### Importing misura
```

