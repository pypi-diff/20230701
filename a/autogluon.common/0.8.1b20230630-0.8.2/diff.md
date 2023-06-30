# Comparing `tmp/autogluon.common-0.8.1b20230630.tar.gz` & `tmp/autogluon.common-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.common-0.8.1b20230630.tar", last modified: Fri Jun 30 09:04:14 2023, max compression
+gzip compressed data, was "autogluon.common-0.8.2.tar", last modified: Fri Jun 30 22:16:57 2023, max compression
```

## Comparing `autogluon.common-0.8.1b20230630.tar` & `autogluon.common-0.8.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:14.144690 autogluon.common-0.8.1b20230630/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    12658 2023-06-30 09:04:14.144690 autogluon.common-0.8.1b20230630/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 09:04:14.144690 autogluon.common-0.8.1b20230630/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:14.140690 autogluon.common-0.8.1b20230630/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:14.140690 autogluon.common-0.8.1b20230630/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:14.140690 autogluon.common-0.8.1b20230630/src/autogluon/common/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:14.140690 autogluon.common-0.8.1b20230630/src/autogluon/common/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22823 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/features/feature_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/features/infer_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/features/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:14.144690 autogluon.common-0.8.1b20230630/src/autogluon/common/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/loaders/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/loaders/load_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8850 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/loaders/load_pd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/loaders/load_pkl.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/loaders/load_pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/loaders/load_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/loaders/load_str.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/loaders/load_zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:14.144690 autogluon.common-0.8.1b20230630/src/autogluon/common/model_filter/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/model_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/model_filter/_model_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:14.144690 autogluon.common-0.8.1b20230630/src/autogluon/common/savers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/savers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/savers/save_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/savers/save_pd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/savers/save_pkl.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/savers/save_pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/savers/save_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:14.144690 autogluon.common-0.8.1b20230630/src/autogluon/common/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/utils/compression_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/utils/deprecated_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/utils/distribute_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/utils/lite.py
--rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/utils/multiprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/utils/nvutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/utils/pandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/utils/path_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/utils/resource_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15651 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/utils/s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/utils/try_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-06-30 09:04:00.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-30 09:04:13.000000 autogluon.common-0.8.1b20230630/src/autogluon/common/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:04:14.140690 autogluon.common-0.8.1b20230630/src/autogluon.common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12658 2023-06-30 09:04:13.000000 autogluon.common-0.8.1b20230630/src/autogluon.common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-30 09:04:14.000000 autogluon.common-0.8.1b20230630/src/autogluon.common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:04:13.000000 autogluon.common-0.8.1b20230630/src/autogluon.common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 09:04:13.000000 autogluon.common-0.8.1b20230630/src/autogluon.common.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-30 09:04:13.000000 autogluon.common-0.8.1b20230630/src/autogluon.common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 09:04:13.000000 autogluon.common-0.8.1b20230630/src/autogluon.common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:04:13.000000 autogluon.common-0.8.1b20230630/src/autogluon.common.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:16:57.117230 autogluon.common-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    12649 2023-06-30 22:16:57.117230 autogluon.common-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 22:16:57.117230 autogluon.common-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:16:57.113230 autogluon.common-0.8.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:16:57.113230 autogluon.common-0.8.2/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:16:57.113230 autogluon.common-0.8.2/src/autogluon/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:16:57.113230 autogluon.common-0.8.2/src/autogluon/common/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22823 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/features/feature_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/features/infer_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/features/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:16:57.117230 autogluon.common-0.8.2/src/autogluon/common/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/loaders/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/loaders/load_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8850 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/loaders/load_pd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/loaders/load_pkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/loaders/load_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/loaders/load_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/loaders/load_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/loaders/load_zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:16:57.117230 autogluon.common-0.8.2/src/autogluon/common/model_filter/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/model_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/model_filter/_model_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:16:57.117230 autogluon.common-0.8.2/src/autogluon/common/savers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/savers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/savers/save_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/savers/save_pd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/savers/save_pkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/savers/save_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/savers/save_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:16:57.117230 autogluon.common-0.8.2/src/autogluon/common/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/utils/compression_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/utils/deprecated_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/utils/distribute_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/utils/lite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/utils/multiprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/utils/nvutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/utils/pandas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/utils/path_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/utils/resource_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15650 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/utils/s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/utils/try_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-06-30 22:16:45.000000 autogluon.common-0.8.2/src/autogluon/common/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-30 22:16:56.000000 autogluon.common-0.8.2/src/autogluon/common/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:16:57.113230 autogluon.common-0.8.2/src/autogluon.common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12649 2023-06-30 22:16:56.000000 autogluon.common-0.8.2/src/autogluon.common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-30 22:16:57.000000 autogluon.common-0.8.2/src/autogluon.common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:16:56.000000 autogluon.common-0.8.2/src/autogluon.common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 22:16:56.000000 autogluon.common-0.8.2/src/autogluon.common.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-30 22:16:56.000000 autogluon.common-0.8.2/src/autogluon.common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 22:16:56.000000 autogluon.common-0.8.2/src/autogluon.common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:16:56.000000 autogluon.common-0.8.2/src/autogluon.common.egg-info/zip-safe
```

### Comparing `autogluon.common-0.8.1b20230630/LICENSE` & `autogluon.common-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.1b20230630/PKG-INFO` & `autogluon.common-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.common
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

### Comparing `autogluon.common-0.8.1b20230630/setup.py` & `autogluon.common-0.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon/common/features/feature_metadata.py` & `autogluon.common-0.8.2/src/autogluon/common/features/feature_metadata.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon/common/features/infer_types.py` & `autogluon.common-0.8.2/src/autogluon/common/features/infer_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon/common/features/types.py` & `autogluon.common-0.8.2/src/autogluon/common/features/types.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon/common/loaders/_utils.py` & `autogluon.common-0.8.2/src/autogluon/common/loaders/_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon/common/loaders/load_pd.py` & `autogluon.common-0.8.2/src/autogluon/common/loaders/load_pd.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon/common/loaders/load_pkl.py` & `autogluon.common-0.8.2/src/autogluon/common/loaders/load_pkl.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon/common/loaders/load_pointer.py` & `autogluon.common-0.8.2/src/autogluon/common/loaders/load_pointer.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon/common/loaders/load_s3.py` & `autogluon.common-0.8.2/src/autogluon/common/loaders/load_s3.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon/common/loaders/load_str.py` & `autogluon.common-0.8.2/src/autogluon/common/loaders/load_str.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon/common/model_filter/_model_filter.py` & `autogluon.common-0.8.2/src/autogluon/common/model_filter/_model_filter.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon/common/savers/save_json.py` & `autogluon.common-0.8.2/src/autogluon/common/savers/save_json.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon/common/savers/save_pd.py` & `autogluon.common-0.8.2/src/autogluon/common/savers/save_pd.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     sep: str = ",",
     compression: str = "gzip",
     header: bool = True,
     json_dump_columns: Optional[List[str]] = None,
 ):
     """
     Save pandas DataFrame to the file path.
-    If local path, directories will be created autmatically if necessary to save the file.
+    If local path, directories will be created automatically if necessary to save the file.
         If local, will be relative to working directory unless specified as absolute.
     If S3 path, you must have permissions to save to the S3 location available via boto3 in the current session.
 
     By default will save the header and index.
     If saving to CSV, column dtypes may not be maintained upon loading the file.
     To ensure identical column dtypes when loading, save in Parquet format.
```

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon/common/savers/save_pkl.py` & `autogluon.common-0.8.2/src/autogluon/common/savers/save_pkl.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon/common/savers/save_str.py` & `autogluon.common-0.8.2/src/autogluon/common/savers/save_str.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon/common/space.py` & `autogluon.common-0.8.2/src/autogluon/common/space.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon/common/utils/compression_utils.py` & `autogluon.common-0.8.2/src/autogluon/common/utils/compression_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon/common/utils/deprecated_utils.py` & `autogluon.common-0.8.2/src/autogluon/common/utils/deprecated_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon/common/utils/distribute_utils.py` & `autogluon.common-0.8.2/src/autogluon/common/utils/distribute_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon/common/utils/file_utils.py` & `autogluon.common-0.8.2/src/autogluon/common/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon/common/utils/log_utils.py` & `autogluon.common-0.8.2/src/autogluon/common/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon/common/utils/multiprocessing_utils.py` & `autogluon.common-0.8.2/src/autogluon/common/utils/multiprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon/common/utils/nvutil.py` & `autogluon.common-0.8.2/src/autogluon/common/utils/nvutil.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon/common/utils/pandas_utils.py` & `autogluon.common-0.8.2/src/autogluon/common/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon/common/utils/path_converter.py` & `autogluon.common-0.8.2/src/autogluon/common/utils/path_converter.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon/common/utils/resource_utils.py` & `autogluon.common-0.8.2/src/autogluon/common/utils/resource_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 
 
 class RayResourceManager:
     """Manager that fetches ray cluster resources info. This class should only be used within a ray cluster."""
 
     @staticmethod
     def _init_ray():
-        """Initialize ray runtime if not already initialized. Will force the existance of a cluster already being spinned up"""
+        """Initialize ray runtime if not already initialized. Will force the existence of a cluster already being spinned up"""
         try_import_ray()
         import ray
 
         if not ray.is_initialized():
             ray.init(
                 address="auto",  # Force ray to connect to an existing cluster. There should be one. Otherwise, something went wrong
                 log_to_driver=False,
```

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon/common/utils/s3_utils.py` & `autogluon.common-0.8.2/src/autogluon/common/utils/s3_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     prefix: str
         The prefix to upload to
         To upload to the root of the bucket, specify `prefix=''` (empty string)
     folder_to_upload: str
         The local folder to upload to s3
     dry_run: bool, default = False
         Whether to perform uploading
-        If True, will isntead log every file that will be uploaded and the s3 path to be uploaded to
+        If True, will instead log every file that will be uploaded and the s3 path to be uploaded to
     verbose: bool, default = True
         Whether to log detailed loggings
     """
     if prefix.endswith("/"):
         prefix = prefix[:-1]
     files_to_upload = _get_local_objs_to_upload_and_s3_prefix(folder_to_upload=folder_to_upload)
     if verbose:
@@ -163,27 +163,27 @@
     error_if_exists: bool, default = True
         Whether to raise an error if the root folder exists already
     delete_if_exists: bool, default = False
         Whether to delete the local root folder and all contents within if the root folder exists already
         If `error_if_exists=True`, deletion will not occur.
     dry_run: bool, default = False
         Whether to perform the directory creation and file downloading.
-        If True, will isntead log every file that will be downloaded and every directory that will be created
+        If True, will instead log every file that will be downloaded and every directory that will be created
     verbose: bool, default = True
         Whether to log detailed loggings
     **kwargs
         Optional arguments to `list_bucket_prefix_suffix_contains_s3` that allow
         more control of which objects are considered.
     """
     s3_to_local_tuple_list = get_s3_to_local_tuple_list_from_s3_folder(s3_bucket=bucket, s3_prefix=prefix, local_path=local_path, suffix=suffix, **kwargs)
     if verbose:
         logger.log(20, f"Will download {len(s3_to_local_tuple_list)} objects from s3://{bucket}/{prefix} to {local_path}")
     if os.path.isdir(local_path) and not dry_run:
         if error_if_exists:
-            raise ValueError(f"Directory {local_path} already exsists. Please pass in a different `local_path` or set `error_if_exsits` to `False`")
+            raise ValueError(f"Directory {local_path} already exists. Please pass in a different `local_path` or set `error_if_exsits` to `False`")
         if delete_if_exists:
             logger.warning(f"Will delete {local_path} and all its content within because this folder already exists and `delete_if_exists` = `True`")
             shutil.rmtree(local_path)
     download_s3_files(s3_to_local_tuple_list=s3_to_local_tuple_list, dry_run=dry_run)
 
 
 def get_s3_to_local_tuple_list_from_s3_folder(*, s3_bucket: str, s3_prefix: str, local_path: str, **kwargs) -> List[Tuple[str, str]]:
```

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon/common/utils/try_import.py` & `autogluon.common-0.8.2/src/autogluon/common/utils/try_import.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon/common/utils/utils.py` & `autogluon.common-0.8.2/src/autogluon/common/utils/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon.common.egg-info/PKG-INFO` & `autogluon.common-0.8.2/src/autogluon.common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.common
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

### Comparing `autogluon.common-0.8.1b20230630/src/autogluon.common.egg-info/SOURCES.txt` & `autogluon.common-0.8.2/src/autogluon.common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

