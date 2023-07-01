# Comparing `tmp/betabageldb-0.1.1.tar.gz` & `tmp/betabageldb-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betabageldb-0.1.1.tar", last modified: Sat Jul  1 11:34:05 2023, max compression
+gzip compressed data, was "betabageldb-0.1.2.tar", last modified: Sat Jul  1 11:59:36 2023, max compression
```

## Comparing `betabageldb-0.1.1.tar` & `betabageldb-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-01 11:34:05.271417 betabageldb-0.1.1/
--rw-r--r--   0 bidhan     (501) staff       (20)     5921 2023-07-01 11:14:26.000000 betabageldb-0.1.1/BagelDB.py
--rw-r--r--   0 bidhan     (501) staff       (20)       82 2023-06-27 19:31:31.000000 betabageldb-0.1.1/LICENSE.txt
--rw-r--r--   0 bidhan     (501) staff       (20)     4384 2023-07-01 11:34:05.270875 betabageldb-0.1.1/PKG-INFO
--rw-r--r--   0 bidhan     (501) staff       (20)     3753 2023-07-01 11:28:45.000000 betabageldb-0.1.1/README.md
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-01 11:34:05.270414 betabageldb-0.1.1/betabageldb.egg-info/
--rw-r--r--   0 bidhan     (501) staff       (20)     4384 2023-07-01 11:34:05.000000 betabageldb-0.1.1/betabageldb.egg-info/PKG-INFO
--rw-r--r--   0 bidhan     (501) staff       (20)      215 2023-07-01 11:34:05.000000 betabageldb-0.1.1/betabageldb.egg-info/SOURCES.txt
--rw-r--r--   0 bidhan     (501) staff       (20)        1 2023-07-01 11:34:05.000000 betabageldb-0.1.1/betabageldb.egg-info/dependency_links.txt
--rw-r--r--   0 bidhan     (501) staff       (20)        9 2023-07-01 11:34:05.000000 betabageldb-0.1.1/betabageldb.egg-info/requires.txt
--rw-r--r--   0 bidhan     (501) staff       (20)        8 2023-07-01 11:34:05.000000 betabageldb-0.1.1/betabageldb.egg-info/top_level.txt
--rw-r--r--   0 bidhan     (501) staff       (20)       38 2023-07-01 11:34:05.271474 betabageldb-0.1.1/setup.cfg
--rw-r--r--   0 bidhan     (501) staff       (20)      795 2023-07-01 11:33:50.000000 betabageldb-0.1.1/setup.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-01 11:59:36.990789 betabageldb-0.1.2/
+-rw-r--r--   0 bidhan     (501) staff       (20)     5921 2023-07-01 11:14:26.000000 betabageldb-0.1.2/BagelDB.py
+-rw-r--r--   0 bidhan     (501) staff       (20)       82 2023-06-27 19:31:31.000000 betabageldb-0.1.2/LICENSE.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)     4384 2023-07-01 11:59:36.990539 betabageldb-0.1.2/PKG-INFO
+-rw-r--r--   0 bidhan     (501) staff       (20)     3753 2023-07-01 11:28:45.000000 betabageldb-0.1.2/README.md
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-01 11:59:36.989575 betabageldb-0.1.2/betabageldb.egg-info/
+-rw-r--r--   0 bidhan     (501) staff       (20)     4384 2023-07-01 11:59:36.000000 betabageldb-0.1.2/betabageldb.egg-info/PKG-INFO
+-rw-r--r--   0 bidhan     (501) staff       (20)      215 2023-07-01 11:59:36.000000 betabageldb-0.1.2/betabageldb.egg-info/SOURCES.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)        1 2023-07-01 11:59:36.000000 betabageldb-0.1.2/betabageldb.egg-info/dependency_links.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)        9 2023-07-01 11:59:36.000000 betabageldb-0.1.2/betabageldb.egg-info/requires.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)        1 2023-07-01 11:59:36.000000 betabageldb-0.1.2/betabageldb.egg-info/top_level.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)       38 2023-07-01 11:59:36.990829 betabageldb-0.1.2/setup.cfg
+-rw-r--r--   0 bidhan     (501) staff       (20)      838 2023-07-01 11:59:05.000000 betabageldb-0.1.2/setup.py
```

### Comparing `betabageldb-0.1.1/BagelDB.py` & `betabageldb-0.1.2/BagelDB.py`

 * *Files identical despite different names*

### Comparing `betabageldb-0.1.1/PKG-INFO` & `betabageldb-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betabageldb
-Version: 0.1.1
+Version: 0.1.2
 Summary: BagelDB is a Python library for interacting with the BagelDB API.
 Home-page: https://github.com/Bagel-DB/Client
 Author: Bidhan Roy
 Author-email: bidhan@bageldb.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `betabageldb-0.1.1/README.md` & `betabageldb-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `betabageldb-0.1.1/betabageldb.egg-info/PKG-INFO` & `betabageldb-0.1.2/betabageldb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betabageldb
-Version: 0.1.1
+Version: 0.1.2
 Summary: BagelDB is a Python library for interacting with the BagelDB API.
 Home-page: https://github.com/Bagel-DB/Client
 Author: Bidhan Roy
 Author-email: bidhan@bageldb.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `betabageldb-0.1.1/setup.py` & `betabageldb-0.1.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 setup(
     name="betabageldb",
-    version="0.1.1",
+    version="0.1.2",
     description="BagelDB is a Python library for interacting with the BagelDB API.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Bidhan Roy",
     author_email="bidhan@bageldb.ai",
     url="https://github.com/Bagel-DB/Client",
-    py_modules=["BagelDB"],
+    packages=find_packages(),  # changed from py_modules
     install_requires=["requests"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
 )
-
```

