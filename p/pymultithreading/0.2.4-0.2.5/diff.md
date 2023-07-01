# Comparing `tmp/pymultithreading-0.2.4.tar.gz` & `tmp/pymultithreading-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymultithreading-0.2.4.tar", last modified: Fri Jun 30 19:54:18 2023, max compression
+gzip compressed data, was "pymultithreading-0.2.5.tar", last modified: Sat Jul  1 08:05:40 2023, max compression
```

## Comparing `pymultithreading-0.2.4.tar` & `pymultithreading-0.2.5.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 19:54:18.176730 pymultithreading-0.2.4/
--rw-rw-rw-   0        0        0       98 2023-06-30 19:54:17.000000 pymultithreading-0.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2045 2023-06-30 19:54:18.175728 pymultithreading-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1243 2023-06-17 10:16:35.000000 pymultithreading-0.2.4/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pymultithreading-0.2.4/build.py
-drwxrwxrwx   0        0        0        0 2023-06-30 19:54:18.160728 pymultithreading-0.2.4/multithreading/
--rw-rw-rw-   0        0        0       53 2023-06-17 10:18:28.000000 pymultithreading-0.2.4/multithreading/__init__.py
--rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 pymultithreading-0.2.4/multithreading/base.py
--rw-rw-rw-   0        0        0      220 2023-06-17 10:20:04.000000 pymultithreading-0.2.4/multithreading/document.py
--rw-rw-rw-   0        0        0    11624 2023-06-30 18:20:08.000000 pymultithreading-0.2.4/multithreading/process.py
-drwxrwxrwx   0        0        0        0 2023-06-30 19:54:18.174727 pymultithreading-0.2.4/pymultithreading.egg-info/
--rw-rw-rw-   0        0        0     2045 2023-06-30 19:54:18.000000 pymultithreading-0.2.4/pymultithreading.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-06-30 19:54:18.000000 pymultithreading-0.2.4/pymultithreading.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 19:54:18.000000 pymultithreading-0.2.4/pymultithreading.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-30 19:54:18.000000 pymultithreading-0.2.4/pymultithreading.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-30 19:54:18.000000 pymultithreading-0.2.4/pymultithreading.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      635 2023-06-30 19:54:17.000000 pymultithreading-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       20 2023-05-30 09:10:35.000000 pymultithreading-0.2.4/requirements-dev.txt
--rw-rw-rw-   0        0        0       11 2023-05-30 09:09:27.000000 pymultithreading-0.2.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 19:54:18.176730 pymultithreading-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1561 2023-06-30 19:54:06.000000 pymultithreading-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 08:05:40.295578 pymultithreading-0.2.5/
+-rw-rw-rw-   0        0        0       98 2023-07-01 08:05:40.000000 pymultithreading-0.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2045 2023-07-01 08:05:40.294673 pymultithreading-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1243 2023-06-17 10:16:35.000000 pymultithreading-0.2.5/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pymultithreading-0.2.5/build.py
+drwxrwxrwx   0        0        0        0 2023-07-01 08:05:40.285577 pymultithreading-0.2.5/multithreading/
+-rw-rw-rw-   0        0        0       53 2023-06-17 10:18:28.000000 pymultithreading-0.2.5/multithreading/__init__.py
+-rw-rw-rw-   0        0        0    11624 2023-06-30 18:20:08.000000 pymultithreading-0.2.5/multithreading/process.py
+drwxrwxrwx   0        0        0        0 2023-07-01 08:05:40.293575 pymultithreading-0.2.5/pymultithreading.egg-info/
+-rw-rw-rw-   0        0        0     2045 2023-07-01 08:05:40.000000 pymultithreading-0.2.5/pymultithreading.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-07-01 08:05:40.000000 pymultithreading-0.2.5/pymultithreading.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 08:05:40.000000 pymultithreading-0.2.5/pymultithreading.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-01 08:05:40.000000 pymultithreading-0.2.5/pymultithreading.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-01 08:05:40.000000 pymultithreading-0.2.5/pymultithreading.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      635 2023-07-01 08:05:03.000000 pymultithreading-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       20 2023-05-30 09:10:35.000000 pymultithreading-0.2.5/requirements-dev.txt
+-rw-rw-rw-   0        0        0       11 2023-05-30 09:09:27.000000 pymultithreading-0.2.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 08:05:40.295578 pymultithreading-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1561 2023-07-01 08:04:53.000000 pymultithreading-0.2.5/setup.py
```

### Comparing `pymultithreading-0.2.4/PKG-INFO` & `pymultithreading-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymultithreading
-Version: 0.2.4
+Version: 0.2.5
 Summary: A python module for creating multithreading processes easily, in a more Pythonic way.
 Home-page: https://github.com/Shahaf-F-S/multithreading
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymultithreading-0.2.4/README.md` & `pymultithreading-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pymultithreading-0.2.4/build.py` & `pymultithreading-0.2.5/build.py`

 * *Files identical despite different names*

### Comparing `pymultithreading-0.2.4/multithreading/process.py` & `pymultithreading-0.2.5/multithreading/process.py`

 * *Files identical despite different names*

### Comparing `pymultithreading-0.2.4/pymultithreading.egg-info/PKG-INFO` & `pymultithreading-0.2.5/pymultithreading.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymultithreading
-Version: 0.2.4
+Version: 0.2.5
 Summary: A python module for creating multithreading processes easily, in a more Pythonic way.
 Home-page: https://github.com/Shahaf-F-S/multithreading
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymultithreading-0.2.4/pyproject.toml` & `pymultithreading-0.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pymultithreading'
-version = '0.2.4'
+version = '0.2.5'
 description = 'A python module for creating multithreading processes easily, in a more Pythonic way.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pymultithreading-0.2.4/setup.py` & `pymultithreading-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             "__pycache__",
             "*.pyc"
         ],
         include=[],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='pymultithreading',
-        version='0.2.4',
+        version='0.2.5',
         description=(
             "A python module for creating multithreading "
             "processes easily, in a more Pythonic way."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

