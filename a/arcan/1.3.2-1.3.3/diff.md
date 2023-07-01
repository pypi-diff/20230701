# Comparing `tmp/arcan-1.3.2.tar.gz` & `tmp/arcan-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcan-1.3.2.tar", max compression
+gzip compressed data, was "arcan-1.3.3.tar", max compression
```

## Comparing `arcan-1.3.2.tar` & `arcan-1.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1711 2023-07-01 03:17:09.680677 arcan-1.3.2/LICENSE
--rw-r--r--   0        0        0     5132 2023-07-01 03:17:09.680677 arcan-1.3.2/README.md
--rw-r--r--   0        0        0      907 2023-07-01 03:17:09.680677 arcan-1.3.2/arcan/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 03:17:09.684677 arcan-1.3.2/arcan/engines/__init__.py
--rw-r--r--   0        0        0       24 2023-07-01 03:17:09.684677 arcan-1.3.2/arcan/engines/io.py
--rw-r--r--   0        0        0        0 2023-07-01 03:17:09.684677 arcan-1.3.2/arcan/governance/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 03:17:09.684677 arcan-1.3.2/arcan/governance/catalog/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 03:17:09.684677 arcan-1.3.2/arcan/governance/lifecycle/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 03:17:09.684677 arcan-1.3.2/arcan/governance/mdm/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 03:17:09.684677 arcan-1.3.2/arcan/governance/quality/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 03:17:09.684677 arcan-1.3.2/arcan/ml/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 03:17:09.684677 arcan-1.3.2/arcan/orchestrator/__init__.py
--rw-r--r--   0        0        0      478 2023-07-01 03:17:09.684677 arcan-1.3.2/arcan/processing/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 03:17:09.684677 arcan-1.3.2/arcan/processing/pipelines/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 03:17:09.684677 arcan-1.3.2/arcan/processing/quality/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 03:17:09.684677 arcan-1.3.2/arcan/processing/transformations/__init__.py
--rw-r--r--   0        0        0       91 2023-07-01 03:17:09.684677 arcan-1.3.2/arcan/session/__init__.py
--rw-r--r--   0        0        0       62 2023-07-01 03:17:09.684677 arcan-1.3.2/main.py
--rw-r--r--   0        0        0      735 2023-07-01 03:17:09.684677 arcan-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     5855 1970-01-01 00:00:00.000000 arcan-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1711 2023-07-01 04:49:55.080226 arcan-1.3.3/LICENSE
+-rw-r--r--   0        0        0     5132 2023-07-01 04:49:55.080226 arcan-1.3.3/README.md
+-rw-r--r--   0        0        0      907 2023-07-01 04:49:55.084226 arcan-1.3.3/arcan/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 04:49:55.084226 arcan-1.3.3/arcan/engines/__init__.py
+-rw-r--r--   0        0        0       24 2023-07-01 04:49:55.084226 arcan-1.3.3/arcan/engines/io.py
+-rw-r--r--   0        0        0        0 2023-07-01 04:49:55.084226 arcan-1.3.3/arcan/governance/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 04:49:55.084226 arcan-1.3.3/arcan/governance/catalog/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 04:49:55.084226 arcan-1.3.3/arcan/governance/lifecycle/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 04:49:55.084226 arcan-1.3.3/arcan/governance/mdm/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 04:49:55.084226 arcan-1.3.3/arcan/governance/quality/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 04:49:55.084226 arcan-1.3.3/arcan/ml/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 04:49:55.084226 arcan-1.3.3/arcan/orchestrator/__init__.py
+-rw-r--r--   0        0        0      478 2023-07-01 04:49:55.084226 arcan-1.3.3/arcan/processing/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 04:49:55.084226 arcan-1.3.3/arcan/processing/pipelines/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 04:49:55.084226 arcan-1.3.3/arcan/processing/quality/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 04:49:55.084226 arcan-1.3.3/arcan/processing/transformations/__init__.py
+-rw-r--r--   0        0        0       91 2023-07-01 04:49:55.084226 arcan-1.3.3/arcan/session/__init__.py
+-rw-r--r--   0        0        0       62 2023-07-01 04:49:55.084226 arcan-1.3.3/main.py
+-rw-r--r--   0        0        0      735 2023-07-01 04:49:55.088226 arcan-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     5855 1970-01-01 00:00:00.000000 arcan-1.3.3/PKG-INFO
```

### Comparing `arcan-1.3.2/LICENSE` & `arcan-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arcan-1.3.2/README.md` & `arcan-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `arcan-1.3.2/arcan/__init__.py` & `arcan-1.3.3/arcan/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # %%
 from modal import Stub, web_endpoint
 from modal import Image, Stub, web_endpoint
 
-__version__ = "1.3.2"
+__version__ = "1.3.3"
 
 
 # %%
 # %%
 def get_arcan_version():
     try:
         import arcan
```

### Comparing `arcan-1.3.2/pyproject.toml` & `arcan-1.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arcan"
-version = "1.3.2"
+version = "1.3.3"
 description = "A multiheaded modern data bridging package based on pipeline manifests to integrate between any modern (and old) data stack tools"
 authors = ["Carlos D. Escobar-Valbuena <carlosdavidescobar@gmail.com>"]
 license = "arcan.ai Non-Commercial Open Source License"
 readme = "README.md"
 packages = [
     {include = "arcan"},
     {include = "main.py"}
```

### Comparing `arcan-1.3.2/PKG-INFO` & `arcan-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcan
-Version: 1.3.2
+Version: 1.3.3
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
-Metadata-Version: 2.1 Name: arcan Version: 1.3.2 Summary: A multiheaded modern
+Metadata-Version: 2.1 Name: arcan Version: 1.3.3 Summary: A multiheaded modern
 data bridging package based on pipeline manifests to integrate between any
 modern (and old) data stack tools License: arcan.ai Non-Commercial Open Source
 License Author: Carlos D. Escobar-Valbuena Author-email:
 carlosdavidescobar@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License
 :: Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: fastapi (>=0.98.0,<0.99.0) Requires-
```

