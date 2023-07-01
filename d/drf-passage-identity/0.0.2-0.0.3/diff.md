# Comparing `tmp/drf-passage-identity-0.0.2.tar.gz` & `tmp/drf-passage-identity-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-passage-identity-0.0.2.tar", last modified: Thu Jun 29 12:44:48 2023, max compression
+gzip compressed data, was "drf-passage-identity-0.0.3.tar", last modified: Sat Jul  1 02:41:06 2023, max compression
```

## Comparing `drf-passage-identity-0.0.2.tar` & `drf-passage-identity-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 12:44:48.411280 drf-passage-identity-0.0.2/
--rw-rw-rw-   0        0        0     1088 2023-06-28 10:32:49.000000 drf-passage-identity-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       37 2023-06-28 10:33:26.000000 drf-passage-identity-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      926 2023-06-29 12:44:48.411391 drf-passage-identity-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       38 2023-06-28 10:23:41.000000 drf-passage-identity-0.0.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-29 12:44:48.396586 drf-passage-identity-0.0.2/drf_passage_identity.egg-info/
--rw-rw-rw-   0        0        0      926 2023-06-29 12:44:48.000000 drf-passage-identity-0.0.2/drf_passage_identity.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      577 2023-06-29 12:44:48.000000 drf-passage-identity-0.0.2/drf_passage_identity.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 12:44:48.000000 drf-passage-identity-0.0.2/drf_passage_identity.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-06-29 12:44:48.000000 drf-passage-identity-0.0.2/drf_passage_identity.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-29 12:44:48.000000 drf-passage-identity-0.0.2/drf_passage_identity.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-29 12:44:48.408453 drf-passage-identity-0.0.2/passage_auth/
--rw-rw-rw-   0        0        0        0 2023-06-28 07:29:32.000000 drf-passage-identity-0.0.2/passage_auth/__init__.py
--rw-rw-rw-   0        0        0      152 2023-06-28 07:46:00.000000 drf-passage-identity-0.0.2/passage_auth/admin.py
--rw-rw-rw-   0        0        0      161 2023-06-28 07:29:32.000000 drf-passage-identity-0.0.2/passage_auth/apps.py
--rw-rw-rw-   0        0        0     1376 2023-06-29 12:29:36.000000 drf-passage-identity-0.0.2/passage_auth/authentication.py
--rw-rw-rw-   0        0        0     1317 2023-06-28 07:30:18.000000 drf-passage-identity-0.0.2/passage_auth/manager.py
-drwxrwxrwx   0        0        0        0 2023-06-29 12:44:48.410217 drf-passage-identity-0.0.2/passage_auth/migrations/
--rw-rw-rw-   0        0        0     2069 2023-06-28 07:40:16.000000 drf-passage-identity-0.0.2/passage_auth/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-06-28 07:29:32.000000 drf-passage-identity-0.0.2/passage_auth/migrations/__init__.py
--rw-rw-rw-   0        0        0      881 2023-06-28 07:30:03.000000 drf-passage-identity-0.0.2/passage_auth/models.py
--rw-rw-rw-   0        0        0      366 2023-06-28 07:56:48.000000 drf-passage-identity-0.0.2/passage_auth/setup.py
--rw-rw-rw-   0        0        0       63 2023-06-28 07:29:32.000000 drf-passage-identity-0.0.2/passage_auth/tests.py
--rw-rw-rw-   0        0        0      141 2023-06-29 12:33:29.000000 drf-passage-identity-0.0.2/passage_auth/urls.py
--rw-rw-rw-   0        0        0      460 2023-06-29 12:29:54.000000 drf-passage-identity-0.0.2/passage_auth/views.py
--rw-rw-rw-   0        0        0      959 2023-06-29 12:44:48.412484 drf-passage-identity-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-06-28 10:34:13.000000 drf-passage-identity-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 02:41:06.867493 drf-passage-identity-0.0.3/
+-rw-rw-rw-   0        0        0     1088 2023-06-28 10:32:49.000000 drf-passage-identity-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       37 2023-06-28 10:33:26.000000 drf-passage-identity-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2367 2023-07-01 02:41:06.867493 drf-passage-identity-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1481 2023-07-01 02:40:12.000000 drf-passage-identity-0.0.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-01 02:41:06.847864 drf-passage-identity-0.0.3/drf_passage_identity.egg-info/
+-rw-rw-rw-   0        0        0     2367 2023-07-01 02:41:06.000000 drf-passage-identity-0.0.3/drf_passage_identity.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      577 2023-07-01 02:41:06.000000 drf-passage-identity-0.0.3/drf_passage_identity.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 02:41:06.000000 drf-passage-identity-0.0.3/drf_passage_identity.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-01 02:41:06.000000 drf-passage-identity-0.0.3/drf_passage_identity.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-01 02:41:06.000000 drf-passage-identity-0.0.3/drf_passage_identity.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 02:41:06.862381 drf-passage-identity-0.0.3/passage_auth/
+-rw-rw-rw-   0        0        0        0 2023-06-28 07:29:32.000000 drf-passage-identity-0.0.3/passage_auth/__init__.py
+-rw-rw-rw-   0        0        0      152 2023-06-28 07:46:00.000000 drf-passage-identity-0.0.3/passage_auth/admin.py
+-rw-rw-rw-   0        0        0      161 2023-06-28 07:29:32.000000 drf-passage-identity-0.0.3/passage_auth/apps.py
+-rw-rw-rw-   0        0        0     1376 2023-06-29 12:29:36.000000 drf-passage-identity-0.0.3/passage_auth/authentication.py
+-rw-rw-rw-   0        0        0     1317 2023-06-28 07:30:18.000000 drf-passage-identity-0.0.3/passage_auth/manager.py
+drwxrwxrwx   0        0        0        0 2023-07-01 02:41:06.866528 drf-passage-identity-0.0.3/passage_auth/migrations/
+-rw-rw-rw-   0        0        0     2069 2023-06-28 07:40:16.000000 drf-passage-identity-0.0.3/passage_auth/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 07:29:32.000000 drf-passage-identity-0.0.3/passage_auth/migrations/__init__.py
+-rw-rw-rw-   0        0        0      881 2023-06-28 07:30:03.000000 drf-passage-identity-0.0.3/passage_auth/models.py
+-rw-rw-rw-   0        0        0      366 2023-06-28 07:56:48.000000 drf-passage-identity-0.0.3/passage_auth/setup.py
+-rw-rw-rw-   0        0        0       63 2023-06-28 07:29:32.000000 drf-passage-identity-0.0.3/passage_auth/tests.py
+-rw-rw-rw-   0        0        0      141 2023-06-29 12:33:29.000000 drf-passage-identity-0.0.3/passage_auth/urls.py
+-rw-rw-rw-   0        0        0      460 2023-06-29 12:29:54.000000 drf-passage-identity-0.0.3/passage_auth/views.py
+-rw-rw-rw-   0        0        0      959 2023-07-01 02:41:06.869260 drf-passage-identity-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-06-28 10:34:13.000000 drf-passage-identity-0.0.3/setup.py
```

### Comparing `drf-passage-identity-0.0.2/LICENSE` & `drf-passage-identity-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-passage-identity-0.0.2/drf_passage_identity.egg-info/SOURCES.txt` & `drf-passage-identity-0.0.3/drf_passage_identity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf-passage-identity-0.0.2/passage_auth/authentication.py` & `drf-passage-identity-0.0.3/passage_auth/authentication.py`

 * *Files identical despite different names*

### Comparing `drf-passage-identity-0.0.2/passage_auth/manager.py` & `drf-passage-identity-0.0.3/passage_auth/manager.py`

 * *Files identical despite different names*

### Comparing `drf-passage-identity-0.0.2/passage_auth/migrations/0001_initial.py` & `drf-passage-identity-0.0.3/passage_auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf-passage-identity-0.0.2/passage_auth/models.py` & `drf-passage-identity-0.0.3/passage_auth/models.py`

 * *Files identical despite different names*

### Comparing `drf-passage-identity-0.0.2/setup.cfg` & `drf-passage-identity-0.0.3/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 7266 2d70 6173 7361 6765 2d69   = drf-passage-i
 00000020: 6465 6e74 6974 790d 0a76 6572 7369 6f6e  dentity..version
-00000030: 203d 2030 2e30 2e32 0d0a 6465 7363 7269   = 0.0.2..descri
+00000030: 203d 2030 2e30 2e33 0d0a 6465 7363 7269   = 0.0.3..descri
 00000040: 7074 696f 6e20 3d20 4120 446a 616e 676f  ption = A Django
 00000050: 2061 7070 2074 6f20 6175 7468 656e 7469   app to authenti
 00000060: 6361 7465 2075 7365 7273 2070 6173 7377  cate users passw
 00000070: 6f72 646c 6573 7320 7573 696e 6720 5061  ordless using Pa
 00000080: 7373 6167 652e 0d0a 6c6f 6e67 5f64 6573  ssage...long_des
 00000090: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
 000000a0: 2052 4541 444d 452e 7273 740d 0a6c 6f6e   README.rst..lon
```

