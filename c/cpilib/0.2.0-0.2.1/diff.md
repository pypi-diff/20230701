# Comparing `tmp/cpilib-0.2.0.tar.gz` & `tmp/cpilib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpilib-0.2.0.tar", max compression
+gzip compressed data, was "cpilib-0.2.1.tar", max compression
```

## Comparing `cpilib-0.2.0.tar` & `cpilib-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       38 2023-06-25 09:25:19.267328 cpilib-0.2.0/README.md
--rw-r--r--   0        0        0       27 2023-07-01 07:28:39.872746 cpilib-0.2.0/cpilib/__init__.py
--rw-r--r--   0        0        0      412 2023-06-30 13:36:51.855728 cpilib-0.2.0/cpilib/constants.py
--rw-r--r--   0        0        0       67 2023-06-26 13:38:08.779561 cpilib-0.2.0/cpilib/cpi/__init__.py
--rw-r--r--   0        0        0     4371 2023-07-01 06:14:58.685172 cpilib-0.2.0/cpilib/cpi/base_classes.py
--rw-r--r--   0        0        0      130 2023-06-30 13:41:53.526315 cpilib-0.2.0/cpilib/cpi/fr_cpi.py
--rw-r--r--   0        0        0     3634 2023-07-01 11:47:32.513708 cpilib-0.2.0/cpilib/cpi/hicp.py
--rw-r--r--   0        0        0   616448 2023-07-01 06:59:14.556099 cpilib-0.2.0/cpilib/data/cpi2015.xls
--rw-r--r--   0        0        0    11030 2023-07-01 07:23:29.492175 cpilib-0.2.0/cpilib/data/hicp_labels.parquet
--rw-r--r--   0        0        0       78 2023-07-01 07:28:40.067788 cpilib-0.2.0/cpilib/utils/__init__.py
--rw-r--r--   0        0        0      175 2023-07-01 07:28:39.880994 cpilib-0.2.0/cpilib/utils/coicop.py
--rw-r--r--   0        0        0     5321 2023-07-01 11:47:32.353818 cpilib-0.2.0/cpilib/utils/eurostats.py
--rw-r--r--   0        0        0     1292 2023-07-01 11:47:22.009828 cpilib-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      669 1970-01-01 00:00:00.000000 cpilib-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       38 2023-06-25 09:25:19.267328 cpilib-0.2.1/README.md
+-rw-r--r--   0        0        0       27 2023-07-01 07:28:39.872746 cpilib-0.2.1/cpilib/__init__.py
+-rw-r--r--   0        0        0      412 2023-06-30 13:36:51.855728 cpilib-0.2.1/cpilib/constants.py
+-rw-r--r--   0        0        0       67 2023-06-26 13:38:08.779561 cpilib-0.2.1/cpilib/cpi/__init__.py
+-rw-r--r--   0        0        0     4371 2023-07-01 06:14:58.685172 cpilib-0.2.1/cpilib/cpi/base_classes.py
+-rw-r--r--   0        0        0      130 2023-06-30 13:41:53.526315 cpilib-0.2.1/cpilib/cpi/fr_cpi.py
+-rw-r--r--   0        0        0     3542 2023-07-01 13:13:44.246784 cpilib-0.2.1/cpilib/cpi/hicp.py
+-rw-r--r--   0        0        0   616448 2023-07-01 06:59:14.556099 cpilib-0.2.1/cpilib/data/cpi2015.xls
+-rw-r--r--   0        0        0    11030 2023-07-01 07:23:29.492175 cpilib-0.2.1/cpilib/data/hicp_labels.parquet
+-rw-r--r--   0        0        0       78 2023-07-01 07:28:40.067788 cpilib-0.2.1/cpilib/utils/__init__.py
+-rw-r--r--   0        0        0      175 2023-07-01 07:28:39.880994 cpilib-0.2.1/cpilib/utils/coicop.py
+-rw-r--r--   0        0        0     5321 2023-07-01 11:47:32.353818 cpilib-0.2.1/cpilib/utils/eurostats.py
+-rw-r--r--   0        0        0     1292 2023-07-01 13:18:34.049116 cpilib-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      669 1970-01-01 00:00:00.000000 cpilib-0.2.1/PKG-INFO
```

### Comparing `cpilib-0.2.0/cpilib/cpi/base_classes.py` & `cpilib-0.2.1/cpilib/cpi/base_classes.py`

 * *Files identical despite different names*

### Comparing `cpilib-0.2.0/cpilib/cpi/hicp.py` & `cpilib-0.2.1/cpilib/cpi/hicp.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,34 +27,30 @@
         if date_format is not None:
             data.index = pd.to_datetime(data.index, format=date_format)
         else:
             data.index = pd.to_datetime(data.index)
         return (
             data.replace(pd.NA, np.nan)
             .replace(": c", np.nan)
-            .apply(lambda x: x.str.rstrip(" d") if x.dtype == "object" else x)
-            .apply(lambda x: x.str.rstrip(" du") if x.dtype == "object" else x)
+            .applymap(lambda x: x.rstrip(" d") if isinstance(x, str) else x)
+            .applymap(lambda x: x.rstrip(" du") if isinstance(x, str) else x)
             .astype(float)
+            .sort_index(axis=0)
         )
 
     def _load_data(self):
         logger.info("Loading HICP object from Eurostat...")
         prices = get_eurostat_dataset("prc_hicp_midx")
-        prices = (
-            self.clean_dataframe(prices, date_format="%YM%m")["I15"]
-            .swaplevel(0, 1, axis=1)
-            .sort_index(axis=1)
-            .sort_index(axis=0)
-        )
+        prices = self.clean_dataframe(prices["I15"], date_format="%YM%m").swaplevel(0, 1, axis=1).sort_index(axis=1)
 
         item_weights = get_eurostat_dataset("prc_hicp_inw")
-        item_weights = self.clean_dataframe(item_weights).swaplevel(0, 1, axis=1).sort_index(axis=1).sort_index(axis=0)
+        item_weights = self.clean_dataframe(item_weights).swaplevel(0, 1, axis=1).sort_index(axis=1)
 
         country_weights = get_eurostat_dataset("prc_hicp_cow")
-        country_weights = self.clean_dataframe(country_weights)["COWEA19"].sort_index(axis=0)
+        country_weights = self.clean_dataframe(country_weights["COWEA19"])
 
         prices.to_parquet("cache/prices.parquet")
         item_weights.to_parquet("cache/item_weights.parquet")
         country_weights.to_parquet("cache/country_weights.parquet")
 
         return prices, item_weights, country_weights
```

### Comparing `cpilib-0.2.0/cpilib/data/cpi2015.xls` & `cpilib-0.2.1/cpilib/data/cpi2015.xls`

 * *Files identical despite different names*

### Comparing `cpilib-0.2.0/cpilib/data/hicp_labels.parquet` & `cpilib-0.2.1/cpilib/data/hicp_labels.parquet`

 * *Files identical despite different names*

### Comparing `cpilib-0.2.0/cpilib/utils/eurostats.py` & `cpilib-0.2.1/cpilib/utils/eurostats.py`

 * *Files identical despite different names*

### Comparing `cpilib-0.2.0/pyproject.toml` & `cpilib-0.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpilib"
-version = "0.2.0"
+version = "0.2.1"
 description = "Library for handling CPI data"
 authors = ["Thomas Kientz <thomas@kientz.net>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
```

### Comparing `cpilib-0.2.0/PKG-INFO` & `cpilib-0.2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpilib
-Version: 0.2.0
+Version: 0.2.1
 Summary: Library for handling CPI data
 License: MIT
 Author: Thomas Kientz
 Author-email: thomas@kientz.net
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

