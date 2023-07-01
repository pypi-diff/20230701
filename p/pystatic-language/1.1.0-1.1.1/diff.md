# Comparing `tmp/pystatic-language-1.1.0.tar.gz` & `tmp/pystatic-language-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystatic-language-1.1.0.tar", last modified: Thu Jun 29 08:39:53 2023, max compression
+gzip compressed data, was "pystatic-language-1.1.1.tar", last modified: Sat Jul  1 08:19:44 2023, max compression
```

## Comparing `pystatic-language-1.1.0.tar` & `pystatic-language-1.1.1.tar`

### file list

```diff
@@ -1,25 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 08:39:53.127553 pystatic-language-1.1.0/
--rw-rw-rw-   0        0        0      115 2023-06-29 08:39:52.000000 pystatic-language-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4116 2023-06-29 08:39:53.126554 pystatic-language-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3028 2023-06-29 08:39:46.000000 pystatic-language-1.1.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pystatic-language-1.1.0/build.py
--rw-rw-rw-   0        0        0      925 2023-06-29 08:39:52.000000 pystatic-language-1.1.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-29 08:39:53.112555 pystatic-language-1.1.0/pystatic/
--rw-rw-rw-   0        0        0     4714 2023-03-10 17:43:12.000000 pystatic-language-1.1.0/pystatic/base.py
--rw-rw-rw-   0        0        0     2900 2023-06-29 08:31:21.000000 pystatic-language-1.1.0/pystatic/casting.py
--rw-rw-rw-   0        0        0     1408 2023-06-29 08:31:59.000000 pystatic-language-1.1.0/pystatic/clean.py
--rw-rw-rw-   0        0        0      489 2023-03-16 09:08:51.000000 pystatic-language-1.1.0/pystatic/document.py
--rw-rw-rw-   0        0        0     5536 2023-06-29 08:34:59.000000 pystatic-language-1.1.0/pystatic/overload.py
--rw-rw-rw-   0        0        0     2879 2023-06-29 08:35:26.000000 pystatic-language-1.1.0/pystatic/private.py
--rw-rw-rw-   0        0        0     8106 2023-06-29 07:23:27.000000 pystatic-language-1.1.0/pystatic/types.py
-drwxrwxrwx   0        0        0        0 2023-06-29 08:39:53.125555 pystatic-language-1.1.0/pystatic_language.egg-info/
--rw-rw-rw-   0        0        0     4116 2023-06-29 08:39:53.000000 pystatic-language-1.1.0/pystatic_language.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-06-29 08:39:53.000000 pystatic-language-1.1.0/pystatic_language.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 08:39:53.000000 pystatic-language-1.1.0/pystatic_language.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-06-29 08:39:53.000000 pystatic-language-1.1.0/pystatic_language.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-29 08:39:53.000000 pystatic-language-1.1.0/pystatic_language.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       24 2023-03-16 09:21:08.000000 pystatic-language-1.1.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       15 2023-03-16 09:10:53.000000 pystatic-language-1.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 08:39:53.127553 pystatic-language-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1952 2023-06-29 08:30:42.000000 pystatic-language-1.1.0/setup.py
--rw-rw-rw-   0        0        0     2783 2023-06-29 08:38:30.000000 pystatic-language-1.1.0/test.py
+drwxrwxrwx   0        0        0        0 2023-07-01 08:19:44.302041 pystatic-language-1.1.1/
+-rw-rw-rw-   0        0        0      115 2023-07-01 08:19:43.000000 pystatic-language-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4116 2023-07-01 08:19:44.302041 pystatic-language-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3028 2023-06-29 08:39:46.000000 pystatic-language-1.1.1/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pystatic-language-1.1.1/build.py
+-rw-rw-rw-   0        0        0      925 2023-07-01 08:19:43.000000 pystatic-language-1.1.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-01 08:19:44.284794 pystatic-language-1.1.1/pystatic/
+-rw-rw-rw-   0        0        0     2900 2023-06-29 08:31:21.000000 pystatic-language-1.1.1/pystatic/casting.py
+-rw-rw-rw-   0        0        0     1408 2023-06-29 08:31:59.000000 pystatic-language-1.1.1/pystatic/clean.py
+-rw-rw-rw-   0        0        0     5536 2023-06-29 08:34:59.000000 pystatic-language-1.1.1/pystatic/overload.py
+-rw-rw-rw-   0        0        0     2879 2023-06-29 08:35:26.000000 pystatic-language-1.1.1/pystatic/private.py
+-rw-rw-rw-   0        0        0     8106 2023-06-29 07:23:27.000000 pystatic-language-1.1.1/pystatic/types.py
+drwxrwxrwx   0        0        0        0 2023-07-01 08:19:44.301037 pystatic-language-1.1.1/pystatic_language.egg-info/
+-rw-rw-rw-   0        0        0     4116 2023-07-01 08:19:44.000000 pystatic-language-1.1.1/pystatic_language.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2023-07-01 08:19:44.000000 pystatic-language-1.1.1/pystatic_language.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 08:19:44.000000 pystatic-language-1.1.1/pystatic_language.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-07-01 08:19:44.000000 pystatic-language-1.1.1/pystatic_language.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-01 08:19:44.000000 pystatic-language-1.1.1/pystatic_language.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       24 2023-03-16 09:21:08.000000 pystatic-language-1.1.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       15 2023-03-16 09:10:53.000000 pystatic-language-1.1.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 08:19:44.302041 pystatic-language-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1952 2023-07-01 08:19:22.000000 pystatic-language-1.1.1/setup.py
+-rw-rw-rw-   0        0        0     2783 2023-06-29 08:38:30.000000 pystatic-language-1.1.1/test.py
```

### Comparing `pystatic-language-1.1.0/PKG-INFO` & `pystatic-language-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystatic-language
-Version: 1.1.0
+Version: 1.1.1
 Summary: This package is a collection of methods and classes for making python more secure, robust, and reliable. This could be achieved through the simple usage of decorators, function calls and inheritance of base classes. Generally, this package can make python a programming language, closer to other static-typed languages, without losing python's dynamic powerful features and.
 Home-page: https://github.com/Shahaf-F-S/pystatic
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pystatic-language-1.1.0/README.md` & `pystatic-language-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pystatic-language-1.1.0/build.py` & `pystatic-language-1.1.1/build.py`

 * *Files identical despite different names*

### Comparing `pystatic-language-1.1.0/pyproject.toml` & `pystatic-language-1.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pystatic-language'
-version = '1.1.0'
+version = '1.1.1'
 description = "This package is a collection of methods and classes for making python more secure, robust, and reliable. This could be achieved through the simple usage of decorators, function calls and inheritance of base classes. Generally, this package can make python a programming language, closer to other static-typed languages, without losing python's dynamic powerful features and."
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pystatic-language-1.1.0/pystatic/casting.py` & `pystatic-language-1.1.1/pystatic/casting.py`

 * *Files identical despite different names*

### Comparing `pystatic-language-1.1.0/pystatic/clean.py` & `pystatic-language-1.1.1/pystatic/clean.py`

 * *Files identical despite different names*

### Comparing `pystatic-language-1.1.0/pystatic/overload.py` & `pystatic-language-1.1.1/pystatic/overload.py`

 * *Files identical despite different names*

### Comparing `pystatic-language-1.1.0/pystatic/private.py` & `pystatic-language-1.1.1/pystatic/private.py`

 * *Files identical despite different names*

### Comparing `pystatic-language-1.1.0/pystatic/types.py` & `pystatic-language-1.1.1/pystatic/types.py`

 * *Files identical despite different names*

### Comparing `pystatic-language-1.1.0/pystatic_language.egg-info/PKG-INFO` & `pystatic-language-1.1.1/pystatic_language.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystatic-language
-Version: 1.1.0
+Version: 1.1.1
 Summary: This package is a collection of methods and classes for making python more secure, robust, and reliable. This could be achieved through the simple usage of decorators, function calls and inheritance of base classes. Generally, this package can make python a programming language, closer to other static-typed languages, without losing python's dynamic powerful features and.
 Home-page: https://github.com/Shahaf-F-S/pystatic
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pystatic-language-1.1.0/setup.py` & `pystatic-language-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "test.py"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='pystatic-language',
-        version='1.1.0',
+        version='1.1.1',
         description=(
             "This package is a collection of methods and classes for "
             "making python more secure, robust, and reliable. "
             "This could be achieved through the simple usage of decorators, "
             "function calls and inheritance of base classes. "
             "Generally, this package can make python a programming language, "
             "closer to other static-typed languages, "
```

### Comparing `pystatic-language-1.1.0/test.py` & `pystatic-language-1.1.1/test.py`

 * *Files identical despite different names*

