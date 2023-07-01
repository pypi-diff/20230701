# Comparing `tmp/easier-1.3.2.tar.gz` & `tmp/easier-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easier-1.3.2.tar", last modified: Thu May  4 16:42:47 2023, max compression
+gzip compressed data, was "easier-1.3.3.tar", last modified: Sat Jul  1 21:48:55 2023, max compression
```

## Comparing `easier-1.3.2.tar` & `easier-1.3.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-05-04 16:42:47.722475 easier-1.3.2/
--rw-rw-r--   0 rob        (501) staff       (20)       39 2017-12-14 15:28:52.000000 easier-1.3.2/CONTRIBUTORS.txt
--rw-rw-r--   0 rob        (501) staff       (20)     1081 2017-12-14 15:28:52.000000 easier-1.3.2/LICENSE
--rw-rw-r--   0 rob        (501) staff       (20)       73 2017-12-14 15:28:52.000000 easier-1.3.2/MANIFEST.in
--rw-rw-r--   0 rob        (501) staff       (20)      448 2023-05-04 16:42:47.722530 easier-1.3.2/PKG-INFO
--rw-rw-r--   0 rob        (501) staff       (20)    12815 2019-12-20 21:04:42.000000 easier-1.3.2/README.md
-drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-05-04 16:42:47.720656 easier-1.3.2/easier/
--rw-rw-r--   0 rob        (501) staff       (20)      685 2022-08-17 21:35:50.000000 easier-1.3.2/easier/__init__.py
--rw-rw-r--   0 rob        (501) staff       (20)     5674 2023-05-04 16:01:56.000000 easier-1.3.2/easier/api.py
--rw-rw-r--   0 rob        (501) staff       (20)    10490 2022-09-21 18:47:14.000000 easier-1.3.2/easier/bernstein.py
--rw-rw-r--   0 rob        (501) staff       (20)    15283 2021-08-04 15:44:52.000000 easier-1.3.2/easier/bigquery.py
--rw-rw-r--   0 rob        (501) staff       (20)     1449 2021-01-14 22:38:24.000000 easier-1.3.2/easier/cli.py
--rw-rw-r--   0 rob        (501) staff       (20)     4453 2019-12-12 19:11:35.000000 easier-1.3.2/easier/clock.py
--rw-rw-r--   0 rob        (501) staff       (20)     2118 2020-05-29 19:14:34.000000 easier-1.3.2/easier/crypt.py
--rw-rw-r--   0 rob        (501) staff       (20)     7986 2023-05-04 16:00:23.000000 easier-1.3.2/easier/dataframe_tools.py
--rw-rw-r--   0 rob        (501) staff       (20)     4416 2021-10-25 19:35:54.000000 easier-1.3.2/easier/distributions.py
--rw-rw-r--   0 rob        (501) staff       (20)     3729 2022-11-06 22:52:50.000000 easier-1.3.2/easier/duck.py
--rw-rw-r--   0 rob        (501) staff       (20)     6934 2023-01-04 21:20:27.000000 easier-1.3.2/easier/duck_model.py
--rw-rw-r--   0 rob        (501) staff       (20)     1312 2022-12-27 18:28:43.000000 easier-1.3.2/easier/ecdf_lib.py
-drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-05-04 16:42:47.722272 easier-1.3.2/easier/filtering/
--rw-rw-r--   0 rob        (501) staff       (20)       89 2021-09-24 01:20:15.000000 easier-1.3.2/easier/filtering/__init__.py
--rw-rw-r--   0 rob        (501) staff       (20)     5693 2021-09-24 01:20:25.000000 easier-1.3.2/easier/filtering/elliptic_filter.py
--rw-rw-r--   0 rob        (501) staff       (20)     2106 2021-11-24 17:03:48.000000 easier-1.3.2/easier/filtering/tvd.py
--rw-rw-r--   0 rob        (501) staff       (20)    14061 2022-08-17 21:35:50.000000 easier-1.3.2/easier/fit_lib.py
--rw-rw-r--   0 rob        (501) staff       (20)     8505 2021-01-14 20:54:34.000000 easier-1.3.2/easier/gsheet.py
--rw-rw-r--   0 rob        (501) staff       (20)     7770 2022-08-16 22:01:30.000000 easier-1.3.2/easier/hvtools.py
--rw-rw-r--   0 rob        (501) staff       (20)     1966 2023-04-21 19:26:12.000000 easier-1.3.2/easier/ibis_tools.py
--rw-rw-r--   0 rob        (501) staff       (20)     1794 2020-03-27 15:13:42.000000 easier-1.3.2/easier/item.py
--rw-rw-r--   0 rob        (501) staff       (20)     2136 2020-05-29 19:14:34.000000 easier-1.3.2/easier/iterify.py
--rw-rw-r--   0 rob        (501) staff       (20)      208 2020-05-29 19:14:34.000000 easier-1.3.2/easier/memory.py
--rw-rw-r--   0 rob        (501) staff       (20)    11444 2022-11-07 18:39:22.000000 easier-1.3.2/easier/minimodel.py
--rw-rw-r--   0 rob        (501) staff       (20)     8148 2022-08-11 18:33:31.000000 easier-1.3.2/easier/minimodel_orig.py
--rw-rw-r--   0 rob        (501) staff       (20)     4950 2021-12-08 22:15:51.000000 easier-1.3.2/easier/nice_dates.py
--rw-rw-r--   0 rob        (501) staff       (20)     2087 2020-05-29 19:14:34.000000 easier-1.3.2/easier/outlier_tools.py
--rw-rw-r--   0 rob        (501) staff       (20)     3186 2022-08-17 21:35:50.000000 easier-1.3.2/easier/parallel.py
--rw-rw-r--   0 rob        (501) staff       (20)     7743 2019-12-12 19:22:12.000000 easier-1.3.2/easier/param_state.py
--rw-rw-r--   0 rob        (501) staff       (20)     1195 2022-08-17 21:35:50.000000 easier-1.3.2/easier/plotting.py
--rw-rw-r--   0 rob        (501) staff       (20)     9482 2022-12-11 17:05:42.000000 easier-1.3.2/easier/postgres.py
--rw-rw-r--   0 rob        (501) staff       (20)      663 2018-08-08 19:33:34.000000 easier-1.3.2/easier/print_catcher.py
--rw-rw-r--   0 rob        (501) staff       (20)     6150 2022-11-10 16:40:03.000000 easier-1.3.2/easier/proportion_lib.py
--rw-rw-r--   0 rob        (501) staff       (20)     3178 2022-09-23 20:00:52.000000 easier-1.3.2/easier/salesforce.py
--rw-rw-r--   0 rob        (501) staff       (20)     3231 2020-05-29 19:14:34.000000 easier-1.3.2/easier/shaper.py
--rw-rw-r--   0 rob        (501) staff       (20)     2902 2019-12-12 19:11:38.000000 easier-1.3.2/easier/timer.py
--rw-rw-r--   0 rob        (501) staff       (20)    19244 2023-01-03 20:00:58.000000 easier-1.3.2/easier/utils.py
--rw-rw-r--   0 rob        (501) staff       (20)       22 2023-05-04 16:04:28.000000 easier-1.3.2/easier/version.py
-drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-05-04 16:42:47.721540 easier-1.3.2/easier.egg-info/
--rw-r--r--   0 rob        (501) staff       (20)      448 2023-05-04 16:42:47.000000 easier-1.3.2/easier.egg-info/PKG-INFO
--rw-r--r--   0 rob        (501) staff       (20)     1018 2023-05-04 16:42:47.000000 easier-1.3.2/easier.egg-info/SOURCES.txt
--rw-r--r--   0 rob        (501) staff       (20)        1 2023-05-04 16:42:47.000000 easier-1.3.2/easier.egg-info/dependency_links.txt
--rw-r--r--   0 rob        (501) staff       (20)      117 2023-05-04 16:42:47.000000 easier-1.3.2/easier.egg-info/entry_points.txt
--rw-r--r--   0 rob        (501) staff       (20)        1 2023-01-04 21:15:28.000000 easier-1.3.2/easier.egg-info/not-zip-safe
--rw-r--r--   0 rob        (501) staff       (20)       36 2023-05-04 16:42:47.000000 easier-1.3.2/easier.egg-info/requires.txt
--rw-r--r--   0 rob        (501) staff       (20)        7 2023-05-04 16:42:47.000000 easier-1.3.2/easier.egg-info/top_level.txt
--rw-rw-r--   0 rob        (501) staff       (20)      504 2023-05-04 16:42:47.722781 easier-1.3.2/setup.cfg
--rw-rw-r--   0 rob        (501) staff       (20)     1638 2021-01-14 22:24:18.000000 easier-1.3.2/setup.py
+drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-07-01 21:48:55.125621 easier-1.3.3/
+-rw-rw-r--   0 rob        (501) staff       (20)       39 2017-12-14 15:28:52.000000 easier-1.3.3/CONTRIBUTORS.txt
+-rw-rw-r--   0 rob        (501) staff       (20)     1081 2017-12-14 15:28:52.000000 easier-1.3.3/LICENSE
+-rw-rw-r--   0 rob        (501) staff       (20)       73 2017-12-14 15:28:52.000000 easier-1.3.3/MANIFEST.in
+-rw-rw-r--   0 rob        (501) staff       (20)      448 2023-07-01 21:48:55.125706 easier-1.3.3/PKG-INFO
+-rw-rw-r--   0 rob        (501) staff       (20)    12815 2019-12-20 21:04:42.000000 easier-1.3.3/README.md
+drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-07-01 21:48:55.123550 easier-1.3.3/easier/
+-rw-rw-r--   0 rob        (501) staff       (20)      685 2022-08-17 21:35:50.000000 easier-1.3.3/easier/__init__.py
+-rw-rw-r--   0 rob        (501) staff       (20)     5770 2023-06-05 21:20:14.000000 easier-1.3.3/easier/api.py
+-rw-rw-r--   0 rob        (501) staff       (20)    10490 2022-09-21 18:47:14.000000 easier-1.3.3/easier/bernstein.py
+-rw-rw-r--   0 rob        (501) staff       (20)    15283 2021-08-04 15:44:52.000000 easier-1.3.3/easier/bigquery.py
+-rw-rw-r--   0 rob        (501) staff       (20)     1449 2021-01-14 22:38:24.000000 easier-1.3.3/easier/cli.py
+-rw-rw-r--   0 rob        (501) staff       (20)     4453 2019-12-12 19:11:35.000000 easier-1.3.3/easier/clock.py
+-rw-rw-r--   0 rob        (501) staff       (20)     2118 2020-05-29 19:14:34.000000 easier-1.3.3/easier/crypt.py
+-rw-rw-r--   0 rob        (501) staff       (20)     7988 2023-05-05 21:10:21.000000 easier-1.3.3/easier/dataframe_tools.py
+-rw-rw-r--   0 rob        (501) staff       (20)     4416 2021-10-25 19:35:54.000000 easier-1.3.3/easier/distributions.py
+-rw-rw-r--   0 rob        (501) staff       (20)     3729 2022-11-06 22:52:50.000000 easier-1.3.3/easier/duck.py
+-rw-rw-r--   0 rob        (501) staff       (20)     6934 2023-01-04 21:20:27.000000 easier-1.3.3/easier/duck_model.py
+-rw-rw-r--   0 rob        (501) staff       (20)     1312 2022-12-27 18:28:43.000000 easier-1.3.3/easier/ecdf_lib.py
+drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-07-01 21:48:55.125447 easier-1.3.3/easier/filtering/
+-rw-rw-r--   0 rob        (501) staff       (20)       89 2021-09-24 01:20:15.000000 easier-1.3.3/easier/filtering/__init__.py
+-rw-rw-r--   0 rob        (501) staff       (20)     5693 2021-09-24 01:20:25.000000 easier-1.3.3/easier/filtering/elliptic_filter.py
+-rw-rw-r--   0 rob        (501) staff       (20)     2106 2021-11-24 17:03:48.000000 easier-1.3.3/easier/filtering/tvd.py
+-rw-rw-r--   0 rob        (501) staff       (20)    14061 2022-08-17 21:35:50.000000 easier-1.3.3/easier/fit_lib.py
+-rw-rw-r--   0 rob        (501) staff       (20)     8505 2021-01-14 20:54:34.000000 easier-1.3.3/easier/gsheet.py
+-rw-rw-r--   0 rob        (501) staff       (20)     7770 2022-08-16 22:01:30.000000 easier-1.3.3/easier/hvtools.py
+-rw-rw-r--   0 rob        (501) staff       (20)     3749 2023-07-01 21:46:38.000000 easier-1.3.3/easier/ibis_tools.py
+-rw-rw-r--   0 rob        (501) staff       (20)     1794 2020-03-27 15:13:42.000000 easier-1.3.3/easier/item.py
+-rw-rw-r--   0 rob        (501) staff       (20)     2136 2020-05-29 19:14:34.000000 easier-1.3.3/easier/iterify.py
+-rw-rw-r--   0 rob        (501) staff       (20)      208 2020-05-29 19:14:34.000000 easier-1.3.3/easier/memory.py
+-rw-rw-r--   0 rob        (501) staff       (20)    11444 2022-11-07 18:39:22.000000 easier-1.3.3/easier/minimodel.py
+-rw-rw-r--   0 rob        (501) staff       (20)     8148 2022-08-11 18:33:31.000000 easier-1.3.3/easier/minimodel_orig.py
+-rw-rw-r--   0 rob        (501) staff       (20)     4950 2021-12-08 22:15:51.000000 easier-1.3.3/easier/nice_dates.py
+-rw-rw-r--   0 rob        (501) staff       (20)     2087 2020-05-29 19:14:34.000000 easier-1.3.3/easier/outlier_tools.py
+-rw-rw-r--   0 rob        (501) staff       (20)     3186 2022-08-17 21:35:50.000000 easier-1.3.3/easier/parallel.py
+-rw-rw-r--   0 rob        (501) staff       (20)     7743 2019-12-12 19:22:12.000000 easier-1.3.3/easier/param_state.py
+-rw-rw-r--   0 rob        (501) staff       (20)     1195 2022-08-17 21:35:50.000000 easier-1.3.3/easier/plotting.py
+-rw-rw-r--   0 rob        (501) staff       (20)     9482 2022-12-11 17:05:42.000000 easier-1.3.3/easier/postgres.py
+-rw-rw-r--   0 rob        (501) staff       (20)      663 2018-08-08 19:33:34.000000 easier-1.3.3/easier/print_catcher.py
+-rw-rw-r--   0 rob        (501) staff       (20)     6150 2022-11-10 16:40:03.000000 easier-1.3.3/easier/proportion_lib.py
+-rw-rw-r--   0 rob        (501) staff       (20)     3178 2022-09-23 20:00:52.000000 easier-1.3.3/easier/salesforce.py
+-rw-rw-r--   0 rob        (501) staff       (20)     3231 2020-05-29 19:14:34.000000 easier-1.3.3/easier/shaper.py
+-rw-rw-r--   0 rob        (501) staff       (20)     2902 2019-12-12 19:11:38.000000 easier-1.3.3/easier/timer.py
+-rw-rw-r--   0 rob        (501) staff       (20)    19244 2023-01-03 20:00:58.000000 easier-1.3.3/easier/utils.py
+-rw-rw-r--   0 rob        (501) staff       (20)       22 2023-07-01 21:47:26.000000 easier-1.3.3/easier/version.py
+drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-07-01 21:48:55.124828 easier-1.3.3/easier.egg-info/
+-rw-r--r--   0 rob        (501) staff       (20)      448 2023-07-01 21:48:55.000000 easier-1.3.3/easier.egg-info/PKG-INFO
+-rw-r--r--   0 rob        (501) staff       (20)     1018 2023-07-01 21:48:55.000000 easier-1.3.3/easier.egg-info/SOURCES.txt
+-rw-r--r--   0 rob        (501) staff       (20)        1 2023-07-01 21:48:55.000000 easier-1.3.3/easier.egg-info/dependency_links.txt
+-rw-r--r--   0 rob        (501) staff       (20)      117 2023-07-01 21:48:55.000000 easier-1.3.3/easier.egg-info/entry_points.txt
+-rw-r--r--   0 rob        (501) staff       (20)        1 2023-01-04 21:15:28.000000 easier-1.3.3/easier.egg-info/not-zip-safe
+-rw-r--r--   0 rob        (501) staff       (20)       36 2023-07-01 21:48:55.000000 easier-1.3.3/easier.egg-info/requires.txt
+-rw-r--r--   0 rob        (501) staff       (20)        7 2023-07-01 21:48:55.000000 easier-1.3.3/easier.egg-info/top_level.txt
+-rw-rw-r--   0 rob        (501) staff       (20)      504 2023-07-01 21:48:55.126170 easier-1.3.3/setup.cfg
+-rw-rw-r--   0 rob        (501) staff       (20)     1638 2021-01-14 22:24:18.000000 easier-1.3.3/setup.py
```

### Comparing `easier-1.3.2/LICENSE` & `easier-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/README.md` & `easier-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/__init__.py` & `easier-1.3.3/easier/__init__.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/api.py` & `easier-1.3.3/easier/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     Fitter = Importable("easier.fit_lib", "Fitter")
     GlobalClock = Importable("easier.clock", "GlobalClock")
     Gsheet = Importable("easier.gsheet", "GSheet")
     Item = Importable("easier.item", "Item")
     MiniModel = Importable("easier.minimodel", "MiniModel")
     MiniModelPG = Importable("easier.minimodel", "MiniModelPG")
     MiniModelSqlite = Importable("easier.minimodel", "MiniModelSqlite")
+    OrderedSchema = Importable('easier.ibis_tools', 'get_order_schema_class', instantiate=True)
     PG = Importable("easier.postgres", "PG")
     Parallel = Importable("easier.parallel", "Parallel")
     ParamState = Importable("easier.param_state", "ParamState")
     PrintCatcher = Importable("easier.print_catcher", "PrintCatcher")
     Proportion = Importable("easier.proportion_lib", "Proportion")
     SalesForceReport = Importable("easier.salesforce", "SalesForceReport")
     Scaler = Importable("easier.utils", "Scaler")
```

### Comparing `easier-1.3.2/easier/bernstein.py` & `easier-1.3.3/easier/bernstein.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/bigquery.py` & `easier-1.3.3/easier/bigquery.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/cli.py` & `easier-1.3.3/easier/cli.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/clock.py` & `easier-1.3.3/easier/clock.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/crypt.py` & `easier-1.3.3/easier/crypt.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/dataframe_tools.py` & `easier-1.3.3/easier/dataframe_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,15 +186,15 @@
     if non_numerics_are_index:
         index_cols = non_delta_cols + [new_time_col_name]
         df = df.groupby(by=index_cols).sum().sort_index()
 
     return df
 
 
-def weekday_string(ser, kind="tag"):
+def weekday_string(ser, kind="slug"):
     """
     Transform a pandas series of datetims into strings
     corresponding to their weekday.
     Args:
         ser: a pandas series object of timestamps
         kind: ['tag', 'slug', 'name']
               tag -> ['0_mon', '1_tue', ...]
@@ -219,15 +219,15 @@
     elif kind == "name":
         out = [calendar.day_name[d] for d in ser]
 
     out = pd.Series(out, index=ser.index)
     return out
 
 
-def month_string(ser, kind="tag"):
+def month_string(ser, kind="slug"):
     """
     Transform a pandas series of datetims into strings
     corresponding to their months.
     Args:
         ser: a pandas series object of timestamps
         kind: ['tag', 'slug', 'name']
               tag -> [a_jan', 'b_feb', ...]
```

### Comparing `easier-1.3.2/easier/distributions.py` & `easier-1.3.3/easier/distributions.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/duck.py` & `easier-1.3.3/easier/duck.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/duck_model.py` & `easier-1.3.3/easier/duck_model.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/ecdf_lib.py` & `easier-1.3.3/easier/ecdf_lib.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/filtering/elliptic_filter.py` & `easier-1.3.3/easier/filtering/elliptic_filter.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/filtering/tvd.py` & `easier-1.3.3/easier/filtering/tvd.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/fit_lib.py` & `easier-1.3.3/easier/fit_lib.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/gsheet.py` & `easier-1.3.3/easier/gsheet.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/hvtools.py` & `easier-1.3.3/easier/hvtools.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/item.py` & `easier-1.3.3/easier/item.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/iterify.py` & `easier-1.3.3/easier/iterify.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/minimodel.py` & `easier-1.3.3/easier/minimodel.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/minimodel_orig.py` & `easier-1.3.3/easier/minimodel_orig.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/nice_dates.py` & `easier-1.3.3/easier/nice_dates.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/outlier_tools.py` & `easier-1.3.3/easier/outlier_tools.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/parallel.py` & `easier-1.3.3/easier/parallel.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/param_state.py` & `easier-1.3.3/easier/param_state.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/plotting.py` & `easier-1.3.3/easier/plotting.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/postgres.py` & `easier-1.3.3/easier/postgres.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/print_catcher.py` & `easier-1.3.3/easier/print_catcher.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/proportion_lib.py` & `easier-1.3.3/easier/proportion_lib.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/salesforce.py` & `easier-1.3.3/easier/salesforce.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/shaper.py` & `easier-1.3.3/easier/shaper.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/timer.py` & `easier-1.3.3/easier/timer.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier/utils.py` & `easier-1.3.3/easier/utils.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/easier.egg-info/SOURCES.txt` & `easier-1.3.3/easier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easier-1.3.2/setup.py` & `easier-1.3.3/setup.py`

 * *Files identical despite different names*

