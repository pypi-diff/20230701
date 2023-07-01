# Comparing `tmp/cpilib-0.1.1.tar.gz` & `tmp/cpilib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpilib-0.1.1.tar", max compression
+gzip compressed data, was "cpilib-0.1.2.tar", max compression
```

## Comparing `cpilib-0.1.1.tar` & `cpilib-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       38 2023-06-25 09:25:19.267328 cpilib-0.1.1/README.md
--rw-r--r--   0        0        0       27 2023-07-01 07:28:39.872746 cpilib-0.1.1/cpilib/__init__.py
--rw-r--r--   0        0        0      412 2023-06-30 13:36:51.855728 cpilib-0.1.1/cpilib/constants.py
--rw-r--r--   0        0        0       67 2023-06-26 13:38:08.779561 cpilib-0.1.1/cpilib/cpi/__init__.py
--rw-r--r--   0        0        0     4371 2023-07-01 06:14:58.685172 cpilib-0.1.1/cpilib/cpi/base_classes.py
--rw-r--r--   0        0        0      130 2023-06-30 13:41:53.526315 cpilib-0.1.1/cpilib/cpi/fr_cpi.py
--rw-r--r--   0        0        0      957 2023-07-01 07:28:40.067351 cpilib-0.1.1/cpilib/cpi/hicp.py
--rw-r--r--   0        0        0   616448 2023-07-01 06:59:14.556099 cpilib-0.1.1/cpilib/data/cpi2015.xls
--rw-r--r--   0        0        0    11030 2023-07-01 07:23:29.492175 cpilib-0.1.1/cpilib/data/hicp_labels.parquet
--rw-r--r--   0        0        0       78 2023-07-01 07:28:40.067788 cpilib-0.1.1/cpilib/utils/__init__.py
--rw-r--r--   0        0        0      175 2023-07-01 07:28:39.880994 cpilib-0.1.1/cpilib/utils/coicop.py
--rw-r--r--   0        0        0     5369 2023-06-30 13:40:42.035232 cpilib-0.1.1/cpilib/utils/eurostats.py
--rw-r--r--   0        0        0     1292 2023-07-01 07:42:06.378106 cpilib-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      669 1970-01-01 00:00:00.000000 cpilib-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       38 2023-06-25 09:25:19.267328 cpilib-0.1.2/README.md
+-rw-r--r--   0        0        0       27 2023-07-01 07:28:39.872746 cpilib-0.1.2/cpilib/__init__.py
+-rw-r--r--   0        0        0      412 2023-06-30 13:36:51.855728 cpilib-0.1.2/cpilib/constants.py
+-rw-r--r--   0        0        0       67 2023-06-26 13:38:08.779561 cpilib-0.1.2/cpilib/cpi/__init__.py
+-rw-r--r--   0        0        0     4371 2023-07-01 06:14:58.685172 cpilib-0.1.2/cpilib/cpi/base_classes.py
+-rw-r--r--   0        0        0      130 2023-06-30 13:41:53.526315 cpilib-0.1.2/cpilib/cpi/fr_cpi.py
+-rw-r--r--   0        0        0     1089 2023-07-01 07:59:38.818951 cpilib-0.1.2/cpilib/cpi/hicp.py
+-rw-r--r--   0        0        0   616448 2023-07-01 06:59:14.556099 cpilib-0.1.2/cpilib/data/cpi2015.xls
+-rw-r--r--   0        0        0    11030 2023-07-01 07:23:29.492175 cpilib-0.1.2/cpilib/data/hicp_labels.parquet
+-rw-r--r--   0        0        0       78 2023-07-01 07:28:40.067788 cpilib-0.1.2/cpilib/utils/__init__.py
+-rw-r--r--   0        0        0      175 2023-07-01 07:28:39.880994 cpilib-0.1.2/cpilib/utils/coicop.py
+-rw-r--r--   0        0        0     5326 2023-07-01 07:52:44.033275 cpilib-0.1.2/cpilib/utils/eurostats.py
+-rw-r--r--   0        0        0     1292 2023-07-01 08:01:42.496966 cpilib-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      669 1970-01-01 00:00:00.000000 cpilib-0.1.2/PKG-INFO
```

### Comparing `cpilib-0.1.1/cpilib/cpi/base_classes.py` & `cpilib-0.1.2/cpilib/cpi/base_classes.py`

 * *Files identical despite different names*

### Comparing `cpilib-0.1.1/cpilib/cpi/hicp.py` & `cpilib-0.1.2/cpilib/cpi/hicp.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,27 @@
+import logging
 import pandas as pd
 
 from cpilib.cpi.base_classes import CPICountries
 from cpilib.utils import get_eurostat_dataset
 
+logger = logging.getLogger(__name__)
 
 class HICP(CPICountries):
     """CPI class for the Harmonized Index of Consumer Prices (HICP)."""
 
     def __init__(self):
+        logger.info("Initializing HICP object...")
         prices = get_eurostat_dataset("prc_hicp_midx")
         prices.index = pd.to_datetime(prices.index, format="%YM%m")
         prices = prices["I15"].swaplevel(0, 1, axis=1).sort_index(axis=1).sort_index(axis=0)
 
         item_weights = get_eurostat_dataset("prc_hicp_inw")
         item_weights.index = pd.to_datetime(item_weights.index)
         item_weights = item_weights.swaplevel(0, 1, axis=1).sort_index(axis=1).sort_index(axis=0)
 
         country_weights = get_eurostat_dataset("prc_hicp_cow")
         country_weights.index = pd.to_datetime(country_weights.index)
         country_weights = country_weights["COWEA19"].sort_index(axis=0)
 
         super().__init__(prices, item_weights, country_weights, 2015)
+        logger.info("Done.")
```

### Comparing `cpilib-0.1.1/cpilib/data/cpi2015.xls` & `cpilib-0.1.2/cpilib/data/cpi2015.xls`

 * *Files identical despite different names*

### Comparing `cpilib-0.1.1/cpilib/data/hicp_labels.parquet` & `cpilib-0.1.2/cpilib/data/hicp_labels.parquet`

 * *Files identical despite different names*

### Comparing `cpilib-0.1.1/cpilib/utils/eurostats.py` & `cpilib-0.1.2/cpilib/utils/eurostats.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         The filename to save the file under.
     binary : bool, optional
         If True, download file as binary.
     unzip : bool, optional
         If True, unzip the downloaded file.
     """
     if os.path.exists(filename) and file_age(filename) < 24:
-        print("Cached version exists and is less than a day old for", filename)
+        # Cached version exists and is less than a day old
         return
     try:
         with urllib.request.urlopen(url) as resp:
             if unzip:
                 with gzip.GzipFile(fileobj=resp) as data:
                     file_content = data.read()
             else:
@@ -57,16 +57,17 @@
                 file_content = file_content.decode("utf-8")
 
         dir_name = os.path.dirname(filename)
         os.makedirs(dir_name, exist_ok=True)
 
         with open(filename, "wb" if binary else "w") as f:
             f.write(file_content)
-    except Exception as e:
-        print(e)
+    except Exception:
+        pass
+        
 
 
 def get_eurostat_dictionary(dictionary, inverse=False):
     """
     Fetch a dictionary from Eurostat.
 
     Parameters
@@ -93,16 +94,15 @@
         with open(filename) as f:
             d = {}
             for line in f:
                 if len(line.strip()) > 1:
                     row = line.split("\t")
                     d[row[0]] = row[1].strip()
         return {v: k for k, v in d.items()} if inverse else d
-    except Exception as e:
-        print(e)
+    except Exception:
         return {}
 
 
 def get_eurostat_dataset(dataset, replace_codes=True, transpose=True, keep_codes=None):
     """
     Fetch a dataset from Eurostat.
```

### Comparing `cpilib-0.1.1/pyproject.toml` & `cpilib-0.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpilib"
-version = "0.1.1"
+version = "0.1.2"
 description = "Library for handling CPI data"
 authors = ["Thomas Kientz <thomas@kientz.net>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
```

### Comparing `cpilib-0.1.1/PKG-INFO` & `cpilib-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpilib
-Version: 0.1.1
+Version: 0.1.2
 Summary: Library for handling CPI data
 License: MIT
 Author: Thomas Kientz
 Author-email: thomas@kientz.net
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

