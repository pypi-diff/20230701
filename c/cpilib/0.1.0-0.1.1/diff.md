# Comparing `tmp/cpilib-0.1.0.tar.gz` & `tmp/cpilib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpilib-0.1.0.tar", max compression
+gzip compressed data, was "cpilib-0.1.1.tar", max compression
```

## Comparing `cpilib-0.1.0.tar` & `cpilib-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       38 2023-06-25 09:25:19.267328 cpilib-0.1.0/README.md
--rw-r--r--   0        0        0       27 2023-07-01 07:28:39.872746 cpilib-0.1.0/cpilib/__init__.py
--rw-r--r--   0        0        0      412 2023-06-30 13:36:51.855728 cpilib-0.1.0/cpilib/constants.py
--rw-r--r--   0        0        0       67 2023-06-26 13:38:08.779561 cpilib-0.1.0/cpilib/cpi/__init__.py
--rw-r--r--   0        0        0     4371 2023-07-01 06:14:58.685172 cpilib-0.1.0/cpilib/cpi/base_classes.py
--rw-r--r--   0        0        0      130 2023-06-30 13:41:53.526315 cpilib-0.1.0/cpilib/cpi/fr_cpi.py
--rw-r--r--   0        0        0      957 2023-07-01 07:28:40.067351 cpilib-0.1.0/cpilib/cpi/hicp.py
--rw-r--r--   0        0        0   616448 2023-07-01 06:59:14.556099 cpilib-0.1.0/cpilib/data/cpi2015.xls
--rw-r--r--   0        0        0    11030 2023-07-01 07:23:29.492175 cpilib-0.1.0/cpilib/data/hicp_labels.parquet
--rw-r--r--   0        0        0       78 2023-07-01 07:28:40.067788 cpilib-0.1.0/cpilib/utils/__init__.py
--rw-r--r--   0        0        0      175 2023-07-01 07:28:39.880994 cpilib-0.1.0/cpilib/utils/coicop.py
--rw-r--r--   0        0        0     5369 2023-06-30 13:40:42.035232 cpilib-0.1.0/cpilib/utils/eurostats.py
--rw-r--r--   0        0        0     1334 2023-07-01 07:30:24.480162 cpilib-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 cpilib-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       38 2023-06-25 09:25:19.267328 cpilib-0.1.1/README.md
+-rw-r--r--   0        0        0       27 2023-07-01 07:28:39.872746 cpilib-0.1.1/cpilib/__init__.py
+-rw-r--r--   0        0        0      412 2023-06-30 13:36:51.855728 cpilib-0.1.1/cpilib/constants.py
+-rw-r--r--   0        0        0       67 2023-06-26 13:38:08.779561 cpilib-0.1.1/cpilib/cpi/__init__.py
+-rw-r--r--   0        0        0     4371 2023-07-01 06:14:58.685172 cpilib-0.1.1/cpilib/cpi/base_classes.py
+-rw-r--r--   0        0        0      130 2023-06-30 13:41:53.526315 cpilib-0.1.1/cpilib/cpi/fr_cpi.py
+-rw-r--r--   0        0        0      957 2023-07-01 07:28:40.067351 cpilib-0.1.1/cpilib/cpi/hicp.py
+-rw-r--r--   0        0        0   616448 2023-07-01 06:59:14.556099 cpilib-0.1.1/cpilib/data/cpi2015.xls
+-rw-r--r--   0        0        0    11030 2023-07-01 07:23:29.492175 cpilib-0.1.1/cpilib/data/hicp_labels.parquet
+-rw-r--r--   0        0        0       78 2023-07-01 07:28:40.067788 cpilib-0.1.1/cpilib/utils/__init__.py
+-rw-r--r--   0        0        0      175 2023-07-01 07:28:39.880994 cpilib-0.1.1/cpilib/utils/coicop.py
+-rw-r--r--   0        0        0     5369 2023-06-30 13:40:42.035232 cpilib-0.1.1/cpilib/utils/eurostats.py
+-rw-r--r--   0        0        0     1292 2023-07-01 07:42:06.378106 cpilib-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      669 1970-01-01 00:00:00.000000 cpilib-0.1.1/PKG-INFO
```

### Comparing `cpilib-0.1.0/cpilib/cpi/base_classes.py` & `cpilib-0.1.1/cpilib/cpi/base_classes.py`

 * *Files identical despite different names*

### Comparing `cpilib-0.1.0/cpilib/cpi/hicp.py` & `cpilib-0.1.1/cpilib/cpi/hicp.py`

 * *Files identical despite different names*

### Comparing `cpilib-0.1.0/cpilib/data/cpi2015.xls` & `cpilib-0.1.1/cpilib/data/cpi2015.xls`

 * *Files identical despite different names*

### Comparing `cpilib-0.1.0/cpilib/data/hicp_labels.parquet` & `cpilib-0.1.1/cpilib/data/hicp_labels.parquet`

 * *Files identical despite different names*

### Comparing `cpilib-0.1.0/cpilib/utils/eurostats.py` & `cpilib-0.1.1/cpilib/utils/eurostats.py`

 * *Files identical despite different names*

### Comparing `cpilib-0.1.0/pyproject.toml` & `cpilib-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 [tool.poetry]
 name = "cpilib"
-version = "0.1.0"
+version = "0.1.1"
 description = "Library for handling CPI data"
 authors = ["Thomas Kientz <thomas@kientz.net>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.13"
+python = ">=3.9"
 pandas = "^2.0.2"
 pyarrow = "^12.0.1"
-networkx = "^3.1"
 plotly = "^5.15.0"
-scipy = "^1.11.0"
 tqdm = "^4.65.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "3.3.3"
 ipykernel = "^6.23.3"
 
 [tool.black]
```

### Comparing `cpilib-0.1.0/PKG-INFO` & `cpilib-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: cpilib
-Version: 0.1.0
+Version: 0.1.1
 Summary: Library for handling CPI data
 License: MIT
 Author: Thomas Kientz
 Author-email: thomas@kientz.net
-Requires-Python: >=3.9,<3.13
+Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: plotly (>=5.15.0,<6.0.0)
 Requires-Dist: pyarrow (>=12.0.1,<13.0.0)
-Requires-Dist: scipy (>=1.11.0,<2.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 ## **CPI-Lib**
 
 A CPI Python library.
```

