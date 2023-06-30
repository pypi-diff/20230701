# Comparing `tmp/autogluon-0.8.1b20230630.tar.gz` & `tmp/autogluon-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon-0.8.1b20230630.tar", last modified: Fri Jun 30 09:04:43 2023, max compression
+gzip compressed data, was "autogluon-0.8.2.tar", last modified: Fri Jun 30 22:17:29 2023, max compression
```

## Comparing `autogluon-0.8.1b20230630.tar` & `autogluon-0.8.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:43.740770 autogluon-0.8.1b20230630/
--rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-06-30 09:04:43.740770 autogluon-0.8.1b20230630/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 09:04:43.740770 autogluon-0.8.1b20230630/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-30 09:04:00.000000 autogluon-0.8.1b20230630/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:43.736770 autogluon-0.8.1b20230630/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:43.736770 autogluon-0.8.1b20230630/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:43.736770 autogluon-0.8.1b20230630/src/autogluon/_internal_/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 09:04:00.000000 autogluon-0.8.1b20230630/src/autogluon/_internal_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:43.736770 autogluon-0.8.1b20230630/src/autogluon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-06-30 09:04:43.000000 autogluon-0.8.1b20230630/src/autogluon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-30 09:04:43.000000 autogluon-0.8.1b20230630/src/autogluon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:04:43.000000 autogluon-0.8.1b20230630/src/autogluon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 09:04:43.000000 autogluon-0.8.1b20230630/src/autogluon.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-30 09:04:43.000000 autogluon-0.8.1b20230630/src/autogluon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 09:04:43.000000 autogluon-0.8.1b20230630/src/autogluon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:04:43.000000 autogluon-0.8.1b20230630/src/autogluon.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:17:29.797740 autogluon-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-06-30 22:17:29.797740 autogluon-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 22:17:29.797740 autogluon-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-30 22:16:45.000000 autogluon-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:17:29.797740 autogluon-0.8.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:17:29.797740 autogluon-0.8.2/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:17:29.797740 autogluon-0.8.2/src/autogluon/_internal_/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 22:16:45.000000 autogluon-0.8.2/src/autogluon/_internal_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:17:29.797740 autogluon-0.8.2/src/autogluon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-06-30 22:17:29.000000 autogluon-0.8.2/src/autogluon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-30 22:17:29.000000 autogluon-0.8.2/src/autogluon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:17:29.000000 autogluon-0.8.2/src/autogluon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 22:17:29.000000 autogluon-0.8.2/src/autogluon.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-30 22:17:29.000000 autogluon-0.8.2/src/autogluon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 22:17:29.000000 autogluon-0.8.2/src/autogluon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:17:29.000000 autogluon-0.8.2/src/autogluon.egg-info/zip-safe
```

### Comparing `autogluon-0.8.1b20230630/PKG-INFO` & `autogluon-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.8.1b20230630
+Version: 0.8.2
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
@@ -33,15 +33,15 @@
         
         ## Example
         
         ```python
         # First install package from terminal:
         # pip install -U pip
         # pip install -U setuptools wheel
-        # pip install autogluon  # autogluon==0.8.0
+        # pip install autogluon  # autogluon==0.8.1
         
         from autogluon.tabular import TabularDataset, TabularPredictor
         train_data = TabularDataset('https://autogluon.s3.amazonaws.com/datasets/Inc/train.csv')
         test_data = TabularDataset('https://autogluon.s3.amazonaws.com/datasets/Inc/test.csv')
         predictor = TabularPredictor(label='class').fit(train_data, time_limit=120)  # Fit models for 120s
         leaderboard = predictor.leaderboard(test_data)
         ```
```

### Comparing `autogluon-0.8.1b20230630/setup.py` & `autogluon-0.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon-0.8.1b20230630/src/autogluon.egg-info/PKG-INFO` & `autogluon-0.8.2/src/autogluon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.8.1b20230630
+Version: 0.8.2
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
@@ -33,15 +33,15 @@
         
         ## Example
         
         ```python
         # First install package from terminal:
         # pip install -U pip
         # pip install -U setuptools wheel
-        # pip install autogluon  # autogluon==0.8.0
+        # pip install autogluon  # autogluon==0.8.1
         
         from autogluon.tabular import TabularDataset, TabularPredictor
         train_data = TabularDataset('https://autogluon.s3.amazonaws.com/datasets/Inc/train.csv')
         test_data = TabularDataset('https://autogluon.s3.amazonaws.com/datasets/Inc/test.csv')
         predictor = TabularPredictor(label='class').fit(train_data, time_limit=120)  # Fit models for 120s
         leaderboard = predictor.leaderboard(test_data)
         ```
```

