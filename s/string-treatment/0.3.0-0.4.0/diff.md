# Comparing `tmp/string_treatment-0.3.0.tar.gz` & `tmp/string_treatment-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "string_treatment-0.3.0.tar", last modified: Sat Jul  1 00:04:28 2023, max compression
+gzip compressed data, was "string_treatment-0.4.0.tar", last modified: Sat Jul  1 14:58:18 2023, max compression
```

## Comparing `string_treatment-0.3.0.tar` & `string_treatment-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 00:04:28.200965 string_treatment-0.3.0/
--rw-rw-rw-   0        0        0     1091 2023-06-30 17:16:02.000000 string_treatment-0.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0      539 2023-07-01 00:04:28.202998 string_treatment-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1086 2023-07-01 00:02:37.000000 string_treatment-0.3.0/README.md
--rw-rw-rw-   0        0        0      169 2023-06-30 16:32:03.000000 string_treatment-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0      651 2023-07-01 00:04:28.207284 string_treatment-0.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-01 00:04:28.093943 string_treatment-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-01 00:04:28.141130 string_treatment-0.3.0/src/string_treatment/
--rw-rw-rw-   0        0        0        0 2023-06-30 16:48:39.000000 string_treatment-0.3.0/src/string_treatment/__init__.py
--rw-rw-rw-   0        0        0     3472 2023-07-01 00:00:50.000000 string_treatment-0.3.0/src/string_treatment/string_treatment.py
-drwxrwxrwx   0        0        0        0 2023-07-01 00:04:28.196240 string_treatment-0.3.0/src/string_treatment.egg-info/
--rw-rw-rw-   0        0        0      539 2023-07-01 00:04:28.000000 string_treatment-0.3.0/src/string_treatment.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-07-01 00:04:28.000000 string_treatment-0.3.0/src/string_treatment.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 00:04:28.000000 string_treatment-0.3.0/src/string_treatment.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-01 00:04:28.000000 string_treatment-0.3.0/src/string_treatment.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 14:58:18.199161 string_treatment-0.4.0/
+-rw-rw-rw-   0        0        0     1091 2023-06-30 17:16:02.000000 string_treatment-0.4.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      539 2023-07-01 14:58:18.200159 string_treatment-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1305 2023-07-01 14:56:52.000000 string_treatment-0.4.0/README.md
+-rw-rw-rw-   0        0        0      169 2023-06-30 16:32:03.000000 string_treatment-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0      651 2023-07-01 14:58:18.207170 string_treatment-0.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-01 14:58:18.121753 string_treatment-0.4.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-01 14:58:18.166899 string_treatment-0.4.0/src/string_treatment/
+-rw-rw-rw-   0        0        0     3472 2023-07-01 00:00:50.000000 string_treatment-0.4.0/src/string_treatment/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 14:58:18.198160 string_treatment-0.4.0/src/string_treatment.egg-info/
+-rw-rw-rw-   0        0        0      539 2023-07-01 14:58:18.000000 string_treatment-0.4.0/src/string_treatment.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-07-01 14:58:18.000000 string_treatment-0.4.0/src/string_treatment.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 14:58:18.000000 string_treatment-0.4.0/src/string_treatment.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-01 14:58:18.000000 string_treatment-0.4.0/src/string_treatment.egg-info/top_level.txt
```

### Comparing `string_treatment-0.3.0/LICENSE.txt` & `string_treatment-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `string_treatment-0.3.0/PKG-INFO` & `string_treatment-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: string_treatment
-Version: 0.3.0
+Version: 0.4.0
 Summary: String treatment package
 Home-page: https://github.com/guilhermehuther/string_treatment
 Author: Guilherme Huther Baldo
 Author-email: guilhermehuther@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `string_treatment-0.3.0/README.md` & `string_treatment-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![Downloads](https://static.pepy.tech/badge/string_treatment)](https://pepy.tech/project/string_treatment) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
 # Overview
 
 **string_treatment** is a library for cleaning and adjusting data with inconsistency.
 
 # Installation
 Install the latest stable version from PyPI:
```

### Comparing `string_treatment-0.3.0/setup.cfg` & `string_treatment-0.4.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 7472 696e 675f 7472 6561 746d   = string_treatm
 00000020: 656e 740d 0a76 6572 7369 6f6e 203d 2030  ent..version = 0
-00000030: 2e33 2e30 0d0a 6175 7468 6f72 203d 2047  .3.0..author = G
+00000030: 2e34 2e30 0d0a 6175 7468 6f72 203d 2047  .4.0..author = G
 00000040: 7569 6c68 6572 6d65 2048 7574 6865 7220  uilherme Huther 
 00000050: 4261 6c64 6f0d 0a61 7574 686f 725f 656d  Baldo..author_em
 00000060: 6169 6c20 3d20 6775 696c 6865 726d 6568  ail = guilhermeh
 00000070: 7574 6865 7240 676d 6169 6c2e 636f 6d0d  uther@gmail.com.
 00000080: 0a64 6573 6372 6970 7469 6f6e 203d 2053  .description = S
 00000090: 7472 696e 6720 7472 6561 746d 656e 7420  tring treatment 
 000000a0: 7061 636b 6167 650d 0a6c 6f6e 675f 6465  package..long_de
```

### Comparing `string_treatment-0.3.0/src/string_treatment/string_treatment.py` & `string_treatment-0.4.0/src/string_treatment/__init__.py`

 * *Files identical despite different names*

### Comparing `string_treatment-0.3.0/src/string_treatment.egg-info/PKG-INFO` & `string_treatment-0.4.0/src/string_treatment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: string-treatment
-Version: 0.3.0
+Version: 0.4.0
 Summary: String treatment package
 Home-page: https://github.com/guilhermehuther/string_treatment
 Author: Guilherme Huther Baldo
 Author-email: guilhermehuther@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

