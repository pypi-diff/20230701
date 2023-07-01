# Comparing `tmp/itertree-1.0.3.tar.gz` & `tmp/itertree-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itertree-1.0.3.tar", last modified: Wed Jun 28 17:47:05 2023, max compression
+gzip compressed data, was "itertree-1.0.5.tar", last modified: Sat Jul  1 07:40:22 2023, max compression
```

## Comparing `itertree-1.0.3.tar` & `itertree-1.0.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 17:47:05.727141 itertree-1.0.3/
--rw-rw-rw-   0        0        0     1443 2023-06-22 21:06:01.000000 itertree-1.0.3/LICENSE
--rw-rw-rw-   0        0        0    17295 2023-06-28 17:47:05.727141 itertree-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    16683 2023-06-28 17:24:07.000000 itertree-1.0.3/README.md
--rw-rw-rw-   0        0        0      108 2021-03-31 14:04:49.000000 itertree-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      733 2023-06-28 17:47:05.729144 itertree-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      400 2023-06-28 17:24:07.000000 itertree-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-28 17:47:05.664012 itertree-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-28 17:47:05.685144 itertree-1.0.3/src/itertree/
--rw-rw-rw-   0        0        0     2452 2023-06-28 17:24:07.000000 itertree-1.0.3/src/itertree/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-28 17:47:05.701144 itertree-1.0.3/src/itertree/examples/
--rw-rw-rw-   0        0        0        0 2021-03-15 06:47:19.000000 itertree-1.0.3/src/itertree/examples/__init__.py
--rw-rw-rw-   0        0        0    19734 2023-05-30 05:28:38.000000 itertree-1.0.3/src/itertree/examples/calendar_example.py
--rw-rw-rw-   0        0        0     9669 2023-04-23 18:45:52.000000 itertree-1.0.3/src/itertree/examples/itree_data_models.py
--rw-rw-rw-   0        0        0    37511 2023-06-22 06:07:16.000000 itertree-1.0.3/src/itertree/examples/itree_docu_examples.py
--rw-rw-rw-   0        0        0     4376 2023-03-20 13:18:45.000000 itertree-1.0.3/src/itertree/examples/itree_link_example1.py
--rw-rw-rw-   0        0        0     4643 2023-06-15 20:29:07.000000 itertree-1.0.3/src/itertree/examples/itree_usage_example1.py
--rw-rw-rw-   0        0        0     5654 2023-06-15 20:27:56.000000 itertree-1.0.3/src/itertree/examples/itree_usage_example2.py
--rw-rw-rw-   0        0        0    58456 2023-06-21 11:29:14.000000 itertree-1.0.3/src/itertree/itree_data.py
--rw-rw-rw-   0        0        0    23415 2023-04-15 10:59:11.000000 itertree-1.0.3/src/itertree/itree_filters.py
--rw-rw-rw-   0        0        0    48086 2023-06-21 12:47:55.000000 itertree-1.0.3/src/itertree/itree_getitem.py
--rw-rw-rw-   0        0        0    12135 2023-06-22 19:19:49.000000 itertree-1.0.3/src/itertree/itree_helpers.py
--rw-rw-rw-   0        0        0    47842 2023-06-22 19:17:46.000000 itertree-1.0.3/src/itertree/itree_indepth.py
--rw-rw-rw-   0        0        0   146925 2023-06-28 17:22:25.000000 itertree-1.0.3/src/itertree/itree_main.py
--rw-rw-rw-   0        0        0    86824 2023-06-26 06:59:37.000000 itertree-1.0.3/src/itertree/itree_mathsets.py
--rw-rw-rw-   0        0        0    37511 2023-06-19 20:09:54.000000 itertree-1.0.3/src/itertree/itree_private.py
-drwxrwxrwx   0        0        0        0 2023-06-28 17:47:05.708144 itertree-1.0.3/src/itertree/itree_serializer/
--rw-rw-rw-   0        0        0        0 2022-12-01 07:17:33.000000 itertree-1.0.3/src/itertree/itree_serializer/__init__.py
--rw-rw-rw-   0        0        0     7505 2023-06-23 06:17:21.000000 itertree-1.0.3/src/itertree/itree_serializer/itree_json_converter.py
--rw-rw-rw-   0        0        0    20518 2023-05-11 17:09:19.000000 itertree-1.0.3/src/itertree/itree_serializer/itree_json_serialize.py
--rw-rw-rw-   0        0        0     5298 2023-06-09 14:47:12.000000 itertree-1.0.3/src/itertree/itree_serializer/itree_render_dot.py
--rw-rw-rw-   0        0        0     6730 2023-05-10 21:40:47.000000 itertree-1.0.3/src/itertree/itree_serializer/itree_renderer.py
-drwxrwxrwx   0        0        0        0 2023-06-28 17:47:05.691144 itertree-1.0.3/src/itertree.egg-info/
--rw-rw-rw-   0        0        0    17295 2023-06-28 17:47:05.000000 itertree-1.0.3/src/itertree.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1359 2023-06-28 17:47:05.000000 itertree-1.0.3/src/itertree.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 17:47:05.000000 itertree-1.0.3/src/itertree.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-28 17:47:05.000000 itertree-1.0.3/src/itertree.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-28 17:47:05.725144 itertree-1.0.3/tests/
--rw-rw-rw-   0        0        0    80119 2023-06-28 17:06:04.000000 itertree-1.0.3/tests/test_itertree_base1.py
--rw-rw-rw-   0        0        0    31107 2023-06-27 18:42:24.000000 itertree-1.0.3/tests/test_itertree_base_old.py
--rw-rw-rw-   0        0        0     4280 2023-06-12 06:06:03.000000 itertree-1.0.3/tests/test_itertree_examples.py
--rw-rw-rw-   0        0        0    10143 2023-06-26 20:21:06.000000 itertree-1.0.3/tests/test_itertree_flags.py
--rw-rw-rw-   0        0        0    16705 2023-06-27 18:42:24.000000 itertree-1.0.3/tests/test_itertree_full_feature_trees.py
--rw-rw-rw-   0        0        0    19598 2023-02-20 15:28:39.000000 itertree-1.0.3/tests/test_itertree_intervals.py
--rw-rw-rw-   0        0        0    59084 2023-06-26 20:21:06.000000 itertree-1.0.3/tests/test_itertree_iter.py
--rw-rw-rw-   0        0        0    19816 2023-06-27 18:42:24.000000 itertree-1.0.3/tests/test_itertree_links.py
--rw-rw-rw-   0        0        0    59933 2023-02-19 17:40:31.000000 itertree-1.0.3/tests/test_itertree_mathsets.py
--rw-rw-rw-   0        0        0    11308 2023-06-27 18:42:24.000000 itertree-1.0.3/tests/test_itertree_serialize.py
--rw-rw-rw-   0        0        0    19651 2023-03-01 21:50:32.000000 itertree-1.0.3/tests/test_itertree_value_models.py
+drwxrwxrwx   0        0        0        0 2023-07-01 07:40:22.044827 itertree-1.0.5/
+-rw-rw-rw-   0        0        0     1443 2023-06-22 21:06:01.000000 itertree-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0    17295 2023-07-01 07:40:22.045860 itertree-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    16683 2023-07-01 07:38:07.000000 itertree-1.0.5/README.md
+-rw-rw-rw-   0        0        0      108 2021-03-31 14:04:49.000000 itertree-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      733 2023-07-01 07:40:22.046766 itertree-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      402 2023-07-01 07:38:07.000000 itertree-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 07:40:21.974606 itertree-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-01 07:40:21.997598 itertree-1.0.5/src/itertree/
+-rw-rw-rw-   0        0        0     2452 2023-07-01 07:38:07.000000 itertree-1.0.5/src/itertree/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 07:40:22.015598 itertree-1.0.5/src/itertree/examples/
+-rw-rw-rw-   0        0        0        0 2021-03-15 06:47:19.000000 itertree-1.0.5/src/itertree/examples/__init__.py
+-rw-rw-rw-   0        0        0    19734 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/examples/calendar_example.py
+-rw-rw-rw-   0        0        0     9669 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/examples/itree_data_models.py
+-rw-rw-rw-   0        0        0    37511 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/examples/itree_docu_examples.py
+-rw-rw-rw-   0        0        0     4376 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/examples/itree_link_example1.py
+-rw-rw-rw-   0        0        0     4643 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/examples/itree_usage_example1.py
+-rw-rw-rw-   0        0        0     5654 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/examples/itree_usage_example2.py
+-rw-rw-rw-   0        0        0    58456 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/itree_data.py
+-rw-rw-rw-   0        0        0    23415 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/itree_filters.py
+-rw-rw-rw-   0        0        0    48086 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/itree_getitem.py
+-rw-rw-rw-   0        0        0    12135 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/itree_helpers.py
+-rw-rw-rw-   0        0        0    47842 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/itree_indepth.py
+-rw-rw-rw-   0        0        0   146925 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/itree_main.py
+-rw-rw-rw-   0        0        0    86824 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/itree_mathsets.py
+-rw-rw-rw-   0        0        0    37511 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/itree_private.py
+drwxrwxrwx   0        0        0        0 2023-07-01 07:40:22.023599 itertree-1.0.5/src/itertree/itree_serializer/
+-rw-rw-rw-   0        0        0        0 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/itree_serializer/__init__.py
+-rw-rw-rw-   0        0        0     7505 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/itree_serializer/itree_json_converter.py
+-rw-rw-rw-   0        0        0    20518 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/itree_serializer/itree_json_serialize.py
+-rw-rw-rw-   0        0        0     5304 2023-07-01 07:26:51.000000 itertree-1.0.5/src/itertree/itree_serializer/itree_render_dot.py
+-rw-rw-rw-   0        0        0     6730 2023-06-29 16:45:55.000000 itertree-1.0.5/src/itertree/itree_serializer/itree_renderer.py
+drwxrwxrwx   0        0        0        0 2023-07-01 07:40:22.004598 itertree-1.0.5/src/itertree.egg-info/
+-rw-rw-rw-   0        0        0    17295 2023-07-01 07:40:21.000000 itertree-1.0.5/src/itertree.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1359 2023-07-01 07:40:21.000000 itertree-1.0.5/src/itertree.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 07:40:21.000000 itertree-1.0.5/src/itertree.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-01 07:40:21.000000 itertree-1.0.5/src/itertree.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 07:40:22.042837 itertree-1.0.5/tests/
+-rw-rw-rw-   0        0        0    80119 2023-06-28 17:06:04.000000 itertree-1.0.5/tests/test_itertree_base1.py
+-rw-rw-rw-   0        0        0    31107 2023-06-27 18:42:24.000000 itertree-1.0.5/tests/test_itertree_base_old.py
+-rw-rw-rw-   0        0        0     4280 2023-06-12 06:06:03.000000 itertree-1.0.5/tests/test_itertree_examples.py
+-rw-rw-rw-   0        0        0    10143 2023-06-26 20:21:06.000000 itertree-1.0.5/tests/test_itertree_flags.py
+-rw-rw-rw-   0        0        0    16705 2023-06-27 18:42:24.000000 itertree-1.0.5/tests/test_itertree_full_feature_trees.py
+-rw-rw-rw-   0        0        0    19598 2023-02-20 15:28:39.000000 itertree-1.0.5/tests/test_itertree_intervals.py
+-rw-rw-rw-   0        0        0    59084 2023-06-26 20:21:06.000000 itertree-1.0.5/tests/test_itertree_iter.py
+-rw-rw-rw-   0        0        0    19816 2023-06-27 18:42:24.000000 itertree-1.0.5/tests/test_itertree_links.py
+-rw-rw-rw-   0        0        0    59933 2023-02-19 17:40:31.000000 itertree-1.0.5/tests/test_itertree_mathsets.py
+-rw-rw-rw-   0        0        0    11308 2023-06-27 18:42:24.000000 itertree-1.0.5/tests/test_itertree_serialize.py
+-rw-rw-rw-   0        0        0    19651 2023-03-01 21:50:32.000000 itertree-1.0.5/tests/test_itertree_value_models.py
```

### Comparing `itertree-1.0.3/LICENSE` & `itertree-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/PKG-INFO` & `itertree-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itertree
-Version: 1.0.3
+Version: 1.0.5
 Summary: Python tree structure for data storage and iterations
 Home-page: https://github.com/BR1py/itertree
 Author: B_R
 Author-email: br_development@posteo.org
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BR1py/itertree/issues
 Project-URL: Documentation, https://readthedocs.org/projects/itertree/
@@ -16,15 +16,15 @@
 License-File: LICENSE
 
 # itertree python package
 
 
 ## Welcome to itertree python package
 
-Release 1.0.3   - fully released
+Release 1.0.5   - fully released
 
 * Do you have to store data in a tree like structure?
 * Do you need good performance and a reach feature set in the tree object?
 * You like to serialize and store the structure in files?
 * And is it helpful for you if you can link subtrees from other trees and add local items in this "inherited" parts?
 
 Please give itertree package a try!
```

### Comparing `itertree-1.0.3/README.md` & `itertree-1.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # itertree python package
 
 
 ## Welcome to itertree python package
 
-Release 1.0.3   - fully released
+Release 1.0.5   - fully released
 
 * Do you have to store data in a tree like structure?
 * Do you need good performance and a reach feature set in the tree object?
 * You like to serialize and store the structure in files?
 * And is it helpful for you if you can link subtrees from other trees and add local items in this "inherited" parts?
 
 Please give itertree package a try!
```

### Comparing `itertree-1.0.3/setup.cfg` & `itertree-1.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2069 7465 7274 7265 652d 425f 520d   = itertree-B_R.
-00000020: 0a76 6572 7369 6f6e 203d 2031 2e30 2e33  .version = 1.0.3
+00000020: 0a76 6572 7369 6f6e 203d 2031 2e30 2e35  .version = 1.0.5
 00000030: 0d0a 6175 7468 6f72 203d 2042 2e52 2e0d  ..author = B.R..
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 6272 5f64 6576 656c 6f70 6d65 6e74 4070  br_development@p
 00000060: 6f73 7465 6f2e 6f72 670d 0a64 6573 6372  osteo.org..descr
 00000070: 6970 7469 6f6e 203d 2041 2070 6163 6b61  iption = A packa
 00000080: 6765 2066 6f72 2063 7265 6174 696e 6720  ge for creating 
 00000090: 7472 6565 2073 7472 7563 7475 7265 7320  tree structures
```

### Comparing `itertree-1.0.3/src/itertree/__init__.py` & `itertree-1.0.5/src/itertree/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 This part of code contains the initialization and publishing of the iTree related classes of the itertree package.
 """
 
 from __future__ import absolute_import
 
 __package__ = 'itertree'
-__version__ = '1.0.3'
+__version__ = '1.0.5'
 __licence__ = 'MIT incl. human protect patch'
 __author__ = 'B.R.'
 __url__ = 'https://github.com/BR1py/itertree'
 __description__ = 'Python tree structure for data storage and iterations'
 
 from .itree_helpers import iTLink, NoTag, NoKey, NoValue, Tag, iTFLAG, getter_to_list,INF,INF_PLUS,INF_MINUS,Any,TagIdx
 from .itree_main import iTree
```

### Comparing `itertree-1.0.3/src/itertree/examples/calendar_example.py` & `itertree-1.0.5/src/itertree/examples/calendar_example.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/src/itertree/examples/itree_data_models.py` & `itertree-1.0.5/src/itertree/examples/itree_data_models.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/src/itertree/examples/itree_docu_examples.py` & `itertree-1.0.5/src/itertree/examples/itree_docu_examples.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/src/itertree/examples/itree_link_example1.py` & `itertree-1.0.5/src/itertree/examples/itree_link_example1.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/src/itertree/examples/itree_usage_example1.py` & `itertree-1.0.5/src/itertree/examples/itree_usage_example1.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/src/itertree/examples/itree_usage_example2.py` & `itertree-1.0.5/src/itertree/examples/itree_usage_example2.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/src/itertree/itree_data.py` & `itertree-1.0.5/src/itertree/itree_data.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/src/itertree/itree_filters.py` & `itertree-1.0.5/src/itertree/itree_filters.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/src/itertree/itree_getitem.py` & `itertree-1.0.5/src/itertree/itree_getitem.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/src/itertree/itree_helpers.py` & `itertree-1.0.5/src/itertree/itree_helpers.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/src/itertree/itree_indepth.py` & `itertree-1.0.5/src/itertree/itree_indepth.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/src/itertree/itree_main.py` & `itertree-1.0.5/src/itertree/itree_main.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/src/itertree/itree_mathsets.py` & `itertree-1.0.5/src/itertree/itree_mathsets.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/src/itertree/itree_private.py` & `itertree-1.0.5/src/itertree/itree_private.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/src/itertree/itree_serializer/itree_json_converter.py` & `itertree-1.0.5/src/itertree/itree_serializer/itree_json_converter.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/src/itertree/itree_serializer/itree_json_serialize.py` & `itertree-1.0.5/src/itertree/itree_serializer/itree_json_serialize.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/src/itertree/itree_serializer/itree_render_dot.py` & `itertree-1.0.5/src/itertree/itree_serializer/itree_render_dot.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,15 +100,15 @@
                 item_str= item + ' [label="%s"'%label
         if itree_object.is_linked:
             item_str=item_str+', fillcolor=grey'
         elif itree_object.is_value_read_only:
             item_str = item_str + ', fillcolor=cadetblue1'
         elif itree_object.is_link_root:
             item_str = item_str + ', fillcolor=cornflowerblue'
-        item_str=item_str.replace('{','\{').replace('}','\}')
+        item_str = item_str.replace('{', '\\{').replace('}', '\\}')
         return item,item_str+'];'
 
     def render_children(self,out,parent,itree,number,filter_method=None):
         if filter_method:
             iterator=filter(filter_method,itree)
         else:
             iterator = itree
```

### Comparing `itertree-1.0.3/src/itertree/itree_serializer/itree_renderer.py` & `itertree-1.0.5/src/itertree/itree_serializer/itree_renderer.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/src/itertree.egg-info/PKG-INFO` & `itertree-1.0.5/src/itertree.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itertree
-Version: 1.0.3
+Version: 1.0.5
 Summary: Python tree structure for data storage and iterations
 Home-page: https://github.com/BR1py/itertree
 Author: B_R
 Author-email: br_development@posteo.org
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BR1py/itertree/issues
 Project-URL: Documentation, https://readthedocs.org/projects/itertree/
@@ -16,15 +16,15 @@
 License-File: LICENSE
 
 # itertree python package
 
 
 ## Welcome to itertree python package
 
-Release 1.0.3   - fully released
+Release 1.0.5   - fully released
 
 * Do you have to store data in a tree like structure?
 * Do you need good performance and a reach feature set in the tree object?
 * You like to serialize and store the structure in files?
 * And is it helpful for you if you can link subtrees from other trees and add local items in this "inherited" parts?
 
 Please give itertree package a try!
```

### Comparing `itertree-1.0.3/src/itertree.egg-info/SOURCES.txt` & `itertree-1.0.5/src/itertree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/tests/test_itertree_base1.py` & `itertree-1.0.5/tests/test_itertree_base1.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/tests/test_itertree_base_old.py` & `itertree-1.0.5/tests/test_itertree_base_old.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/tests/test_itertree_examples.py` & `itertree-1.0.5/tests/test_itertree_examples.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/tests/test_itertree_flags.py` & `itertree-1.0.5/tests/test_itertree_flags.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/tests/test_itertree_full_feature_trees.py` & `itertree-1.0.5/tests/test_itertree_full_feature_trees.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/tests/test_itertree_intervals.py` & `itertree-1.0.5/tests/test_itertree_intervals.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/tests/test_itertree_iter.py` & `itertree-1.0.5/tests/test_itertree_iter.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/tests/test_itertree_links.py` & `itertree-1.0.5/tests/test_itertree_links.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/tests/test_itertree_mathsets.py` & `itertree-1.0.5/tests/test_itertree_mathsets.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/tests/test_itertree_serialize.py` & `itertree-1.0.5/tests/test_itertree_serialize.py`

 * *Files identical despite different names*

### Comparing `itertree-1.0.3/tests/test_itertree_value_models.py` & `itertree-1.0.5/tests/test_itertree_value_models.py`

 * *Files identical despite different names*

