# Comparing `tmp/fogLedger-2.0.0.tar.gz` & `tmp/fogLedger-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fogLedger-2.0.0.tar", last modified: Sat Jul  1 13:43:03 2023, max compression
+gzip compressed data, was "fogLedger-2.0.2.tar", last modified: Sat Jul  1 14:04:50 2023, max compression
```

## Comparing `fogLedger-2.0.0.tar` & `fogLedger-2.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 matheus   (1000) matheus   (1000)        0 2023-07-01 13:43:03.820892 fogLedger-2.0.0/
--rw-r--r--   0 matheus   (1000) matheus   (1000)     1062 2023-07-01 13:29:47.000000 fogLedger-2.0.0/LICENSE.txt
--rw-r--r--   0 matheus   (1000) matheus   (1000)      515 2023-07-01 13:43:03.820892 fogLedger-2.0.0/PKG-INFO
--rw-r--r--   0 matheus   (1000) matheus   (1000)     2054 2023-05-27 11:43:06.000000 fogLedger-2.0.0/README.md
-drwxr-xr-x   0 matheus   (1000) matheus   (1000)        0 2023-07-01 13:43:03.820892 fogLedger-2.0.0/fogLedger.egg-info/
--rw-r--r--   0 matheus   (1000) matheus   (1000)      515 2023-07-01 13:43:03.000000 fogLedger-2.0.0/fogLedger.egg-info/PKG-INFO
--rw-r--r--   0 matheus   (1000) matheus   (1000)      318 2023-07-01 13:43:03.000000 fogLedger-2.0.0/fogLedger.egg-info/SOURCES.txt
--rw-r--r--   0 matheus   (1000) matheus   (1000)        1 2023-07-01 13:43:03.000000 fogLedger-2.0.0/fogLedger.egg-info/dependency_links.txt
--rw-r--r--   0 matheus   (1000) matheus   (1000)        1 2023-07-01 13:33:01.000000 fogLedger-2.0.0/fogLedger.egg-info/not-zip-safe
--rw-r--r--   0 matheus   (1000) matheus   (1000)       14 2023-07-01 13:43:03.000000 fogLedger-2.0.0/fogLedger.egg-info/requires.txt
--rw-r--r--   0 matheus   (1000) matheus   (1000)       10 2023-07-01 13:43:03.000000 fogLedger-2.0.0/fogLedger.egg-info/top_level.txt
-drwxr-xr-x   0 matheus   (1000) matheus   (1000)        0 2023-07-01 13:43:03.820892 fogLedger-2.0.0/fogledger/
--rw-r--r--   0 matheus   (1000) matheus   (1000)        0 2023-05-25 23:56:28.000000 fogLedger-2.0.0/fogledger/__init__.py
-drwxr-xr-x   0 matheus   (1000) matheus   (1000)        0 2023-07-01 13:43:03.820892 fogLedger-2.0.0/fogledger/indy/
--rw-r--r--   0 matheus   (1000) matheus   (1000)     5235 2023-06-28 13:38:45.000000 fogLedger-2.0.0/fogledger/indy/IndyBasic.py
--rw-r--r--   0 matheus   (1000) matheus   (1000)       48 2023-05-25 23:57:43.000000 fogLedger-2.0.0/fogledger/indy/__init__.py
--rw-r--r--   0 matheus   (1000) matheus   (1000)       84 2023-07-01 13:32:06.000000 fogLedger-2.0.0/pyproject.toml
--rw-r--r--   0 matheus   (1000) matheus   (1000)       38 2023-07-01 13:43:03.820892 fogLedger-2.0.0/setup.cfg
--rw-r--r--   0 matheus   (1000) matheus   (1000)      765 2023-07-01 13:42:57.000000 fogLedger-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:04:50.400639 fogLedger-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-01 14:04:40.000000 fogLedger-2.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-01 14:04:50.400639 fogLedger-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-01 14:04:40.000000 fogLedger-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:04:50.400639 fogLedger-2.0.2/fogLedger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-01 14:04:50.000000 fogLedger-2.0.2/fogLedger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-01 14:04:50.000000 fogLedger-2.0.2/fogLedger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 14:04:50.000000 fogLedger-2.0.2/fogLedger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 14:04:40.000000 fogLedger-2.0.2/fogLedger.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-01 14:04:50.000000 fogLedger-2.0.2/fogLedger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 14:04:50.000000 fogLedger-2.0.2/fogLedger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:04:50.400639 fogLedger-2.0.2/fogledger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 14:04:40.000000 fogLedger-2.0.2/fogledger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:04:50.400639 fogLedger-2.0.2/fogledger/indy/
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-07-01 14:04:40.000000 fogLedger-2.0.2/fogledger/indy/IndyBasic.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-01 14:04:40.000000 fogLedger-2.0.2/fogledger/indy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-01 14:04:40.000000 fogLedger-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 14:04:50.400639 fogLedger-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-01 14:04:40.000000 fogLedger-2.0.2/setup.py
```

### Comparing `fogLedger-2.0.0/LICENSE.txt` & `fogLedger-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fogLedger-2.0.0/PKG-INFO` & `fogLedger-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fogLedger
-Version: 2.0.0
+Version: 2.0.2
 Summary: Plugin to build DLTs in Fogbed.
 Home-page: https://github.com/larsid/FogLedger/tree/v2.0.0
 Author: Matheus Nascimento
 Author-email: matheusnascimentoti99@gmail.com
 Keywords: networking,emulator,protocol,Internet,dlt,indy,fog
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fogLedger-2.0.0/README.md` & `fogLedger-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fogLedger-2.0.0/fogLedger.egg-info/PKG-INFO` & `fogLedger-2.0.2/fogLedger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fogLedger
-Version: 2.0.0
+Version: 2.0.2
 Summary: Plugin to build DLTs in Fogbed.
 Home-page: https://github.com/larsid/FogLedger/tree/v2.0.0
 Author: Matheus Nascimento
 Author-email: matheusnascimentoti99@gmail.com
 Keywords: networking,emulator,protocol,Internet,dlt,indy,fog
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fogLedger-2.0.0/fogledger/indy/IndyBasic.py` & `fogLedger-2.0.2/fogledger/indy/IndyBasic.py`

 * *Files identical despite different names*

### Comparing `fogLedger-2.0.0/setup.py` & `fogLedger-2.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="fogLedger",
-    version="2.0.0",
+    version="2.0.2",
     description='Plugin to build DLTs in Fogbed.',
     long_description='Plugin to build DLT in Fogbed. Suport Hyperledger Indy',
     keywords=['networking', 'emulator', 'protocol', 'Internet', 'dlt', 'indy', 'fog'],
     url='https://github.com/larsid/FogLedger/tree/v2.0.0',
     author='Matheus Nascimento',
     author_email='matheusnascimentoti99@gmail.com',
     classifiers = [
```

