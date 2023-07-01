# Comparing `tmp/arcan-1.3.0.tar.gz` & `tmp/arcan-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcan-1.3.0.tar", max compression
+gzip compressed data, was "arcan-1.3.1.tar", max compression
```

## Comparing `arcan-1.3.0.tar` & `arcan-1.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1711 2023-06-30 23:04:03.659730 arcan-1.3.0/LICENSE
--rw-r--r--   0        0        0     5132 2023-06-30 23:04:03.659730 arcan-1.3.0/README.md
--rw-r--r--   0        0        0      907 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/engines/__init__.py
--rw-r--r--   0        0        0       24 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/engines/io.py
--rw-r--r--   0        0        0        0 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/governance/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/governance/catalog/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/governance/lifecycle/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/governance/mdm/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/governance/quality/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/ml/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/orchestrator/__init__.py
--rw-r--r--   0        0        0      478 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/processing/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/processing/pipelines/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/processing/quality/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/processing/transformations/__init__.py
--rw-r--r--   0        0        0       91 2023-06-30 23:04:03.659730 arcan-1.3.0/arcan/session/__init__.py
--rw-r--r--   0        0        0       62 2023-06-30 23:04:03.659730 arcan-1.3.0/main.py
--rw-r--r--   0        0        0      735 2023-06-30 23:04:03.663730 arcan-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     5855 1970-01-01 00:00:00.000000 arcan-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1711 2023-07-01 03:06:51.599609 arcan-1.3.1/LICENSE
+-rw-r--r--   0        0        0     5132 2023-07-01 03:06:51.599609 arcan-1.3.1/README.md
+-rw-r--r--   0        0        0      907 2023-07-01 03:06:51.599609 arcan-1.3.1/arcan/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 03:06:51.599609 arcan-1.3.1/arcan/engines/__init__.py
+-rw-r--r--   0        0        0       24 2023-07-01 03:06:51.599609 arcan-1.3.1/arcan/engines/io.py
+-rw-r--r--   0        0        0        0 2023-07-01 03:06:51.599609 arcan-1.3.1/arcan/governance/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 03:06:51.599609 arcan-1.3.1/arcan/governance/catalog/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 03:06:51.599609 arcan-1.3.1/arcan/governance/lifecycle/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 03:06:51.599609 arcan-1.3.1/arcan/governance/mdm/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 03:06:51.599609 arcan-1.3.1/arcan/governance/quality/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 03:06:51.599609 arcan-1.3.1/arcan/ml/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 03:06:51.599609 arcan-1.3.1/arcan/orchestrator/__init__.py
+-rw-r--r--   0        0        0      478 2023-07-01 03:06:51.603609 arcan-1.3.1/arcan/processing/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 03:06:51.603609 arcan-1.3.1/arcan/processing/pipelines/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 03:06:51.603609 arcan-1.3.1/arcan/processing/quality/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 03:06:51.603609 arcan-1.3.1/arcan/processing/transformations/__init__.py
+-rw-r--r--   0        0        0       91 2023-07-01 03:06:51.603609 arcan-1.3.1/arcan/session/__init__.py
+-rw-r--r--   0        0        0       62 2023-07-01 03:06:51.603609 arcan-1.3.1/main.py
+-rw-r--r--   0        0        0      735 2023-07-01 03:06:51.603609 arcan-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5855 1970-01-01 00:00:00.000000 arcan-1.3.1/PKG-INFO
```

### Comparing `arcan-1.3.0/LICENSE` & `arcan-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arcan-1.3.0/README.md` & `arcan-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `arcan-1.3.0/arcan/__init__.py` & `arcan-1.3.1/arcan/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # %%
 from modal import Stub, web_endpoint
 from modal import Image, Stub, web_endpoint
 
-__version__ = "1.3.0"
+__version__ = "1.3.1"
 
 
 # %%
 # %%
 def get_arcan_version():
     try:
         import arcan
```

### Comparing `arcan-1.3.0/pyproject.toml` & `arcan-1.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arcan"
-version = "1.3.0"
+version = "1.3.1"
 description = "A multiheaded modern data bridging package based on pipeline manifests to integrate between any modern (and old) data stack tools"
 authors = ["Carlos D. Escobar-Valbuena <carlosdavidescobar@gmail.com>"]
 license = "arcan.ai Non-Commercial Open Source License"
 readme = "README.md"
 packages = [
     {include = "arcan"},
     {include = "main.py"}
```

### Comparing `arcan-1.3.0/PKG-INFO` & `arcan-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcan
-Version: 1.3.0
+Version: 1.3.1
 Summary: A multiheaded modern data bridging package based on pipeline manifests to integrate between any modern (and old) data stack tools
 License: arcan.ai Non-Commercial Open Source License
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: arcan Version: 1.3.0 Summary: A multiheaded modern
+Metadata-Version: 2.1 Name: arcan Version: 1.3.1 Summary: A multiheaded modern
 data bridging package based on pipeline manifests to integrate between any
 modern (and old) data stack tools License: arcan.ai Non-Commercial Open Source
 License Author: Carlos D. Escobar-Valbuena Author-email:
 carlosdavidescobar@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License
 :: Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: fastapi (>=0.98.0,<0.99.0) Requires-
```

