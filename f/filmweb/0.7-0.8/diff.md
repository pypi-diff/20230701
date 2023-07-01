# Comparing `tmp/filmweb-0.7.tar.gz` & `tmp/filmweb-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filmweb-0.7.tar", last modified: Tue May 23 16:27:03 2023, max compression
+gzip compressed data, was "filmweb-0.8.tar", last modified: Sat Jul  1 17:54:48 2023, max compression
```

## Comparing `filmweb-0.7.tar` & `filmweb-0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 16:27:03.682055 filmweb-0.7/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1070 2020-08-04 13:32:10.000000 filmweb-0.7/LICENSE
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6072 2023-05-23 16:27:03.678055 filmweb-0.7/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5542 2023-05-23 16:14:25.000000 filmweb-0.7/README.md
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 16:27:03.674055 filmweb-0.7/filmweb/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-01-20 17:59:47.000000 filmweb-0.7/filmweb/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2842 2023-05-23 15:14:56.000000 filmweb-0.7/filmweb/getter.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2992 2023-05-23 15:53:42.000000 filmweb-0.7/filmweb/main.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3489 2023-05-23 15:57:56.000000 filmweb-0.7/filmweb/parser.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 16:27:03.678055 filmweb-0.7/filmweb.egg-info/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6072 2023-05-23 16:27:03.000000 filmweb-0.7/filmweb.egg-info/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      309 2023-05-23 16:27:03.000000 filmweb-0.7/filmweb.egg-info/SOURCES.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-05-23 16:27:03.000000 filmweb-0.7/filmweb.egg-info/dependency_links.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       46 2023-05-23 16:27:03.000000 filmweb-0.7/filmweb.egg-info/entry_points.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2023-05-23 16:27:03.000000 filmweb-0.7/filmweb.egg-info/requires.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        8 2023-05-23 16:27:03.000000 filmweb-0.7/filmweb.egg-info/top_level.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      824 2023-05-23 08:48:38.000000 filmweb-0.7/pyproject.toml
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2023-05-23 08:48:14.000000 filmweb-0.7/requirements.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2023-05-23 16:27:03.682055 filmweb-0.7/setup.cfg
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-07-01 17:54:48.079788 filmweb-0.8/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1070 2020-08-04 13:32:10.000000 filmweb-0.8/LICENSE
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6079 2023-07-01 17:54:48.075788 filmweb-0.8/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5542 2023-05-23 16:14:25.000000 filmweb-0.8/README.md
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-07-01 17:54:48.071788 filmweb-0.8/filmweb/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-01-20 17:59:47.000000 filmweb-0.8/filmweb/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2842 2023-05-23 15:14:56.000000 filmweb-0.8/filmweb/getter.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2992 2023-05-23 15:53:42.000000 filmweb-0.8/filmweb/main.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3489 2023-05-23 15:57:56.000000 filmweb-0.8/filmweb/parser.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-07-01 17:54:48.075788 filmweb-0.8/filmweb.egg-info/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6079 2023-07-01 17:54:48.000000 filmweb-0.8/filmweb.egg-info/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      309 2023-07-01 17:54:48.000000 filmweb-0.8/filmweb.egg-info/SOURCES.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-07-01 17:54:48.000000 filmweb-0.8/filmweb.egg-info/dependency_links.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       46 2023-07-01 17:54:48.000000 filmweb-0.8/filmweb.egg-info/entry_points.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2023-07-01 17:54:48.000000 filmweb-0.8/filmweb.egg-info/requires.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        8 2023-07-01 17:54:48.000000 filmweb-0.8/filmweb.egg-info/top_level.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      831 2023-07-01 17:46:04.000000 filmweb-0.8/pyproject.toml
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2023-07-01 17:49:18.000000 filmweb-0.8/requirements.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2023-07-01 17:54:48.079788 filmweb-0.8/setup.cfg
```

### Comparing `filmweb-0.7/LICENSE` & `filmweb-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `filmweb-0.7/PKG-INFO` & `filmweb-0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: filmweb
-Version: 0.7
+Version: 0.8
 Summary: Export movie ratings from filmweb.pl
 Author: Piotr Patrzyk
 License: MIT
-Project-URL: Source, https://github.com/ppatrzyk/filmweb
+Project-URL: Source, https://github.com/ppatrzyk/filmweb-export
 Keywords: filmweb,movie,crawler,data
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet
 Requires-Python: >=3.10
```

### Comparing `filmweb-0.7/README.md` & `filmweb-0.8/README.md`

 * *Files identical despite different names*

### Comparing `filmweb-0.7/filmweb/getter.py` & `filmweb-0.8/filmweb/getter.py`

 * *Files identical despite different names*

### Comparing `filmweb-0.7/filmweb/main.py` & `filmweb-0.8/filmweb/main.py`

 * *Files identical despite different names*

### Comparing `filmweb-0.7/filmweb/parser.py` & `filmweb-0.8/filmweb/parser.py`

 * *Files identical despite different names*

### Comparing `filmweb-0.7/filmweb.egg-info/PKG-INFO` & `filmweb-0.8/filmweb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: filmweb
-Version: 0.7
+Version: 0.8
 Summary: Export movie ratings from filmweb.pl
 Author: Piotr Patrzyk
 License: MIT
-Project-URL: Source, https://github.com/ppatrzyk/filmweb
+Project-URL: Source, https://github.com/ppatrzyk/filmweb-export
 Keywords: filmweb,movie,crawler,data
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet
 Requires-Python: >=3.10
```

### Comparing `filmweb-0.7/pyproject.toml` & `filmweb-0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "filmweb"
-version = "0.7"
+version = "0.8"
 description = "Export movie ratings from filmweb.pl"
 authors = [ {name = "Piotr Patrzyk"}, ]
 license = {text = "MIT"}
 readme = "README.md"
 requires-python = ">=3.10"
 dynamic = ["dependencies", ]
 keywords = ["filmweb", "movie", "crawler", "data"]
@@ -13,15 +13,15 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Topic :: Internet",
 ]
 
 [project.urls]
-Source = "https://github.com/ppatrzyk/filmweb"
+Source = "https://github.com/ppatrzyk/filmweb-export"
 
 [project.scripts]
 filmweb = "filmweb.main:main"
 
 [build-system]
 requires = ["setuptools", ]
 build-backend = "setuptools.build_meta"
```

