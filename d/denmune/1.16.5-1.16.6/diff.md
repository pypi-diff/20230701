# Comparing `tmp/denmune-1.16.5.tar.gz` & `tmp/denmune-1.16.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denmune-1.16.5.tar", last modified: Sat May 20 11:18:23 2023, max compression
+gzip compressed data, was "denmune-1.16.6.tar", last modified: Sat Jul  1 03:25:51 2023, max compression
```

## Comparing `denmune-1.16.5.tar` & `denmune-1.16.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 11:18:23.446787 denmune-1.16.5/
--rw-rw-rw-   0        0        0     1498 2021-12-31 23:30:13.000000 denmune-1.16.5/LICENSE
--rw-rw-rw-   0        0        0       47 2021-12-27 21:52:58.000000 denmune-1.16.5/MANIFEST.in
--rw-rw-rw-   0        0        0    29731 2023-05-20 11:18:23.450024 denmune-1.16.5/PKG-INFO
--rw-rw-rw-   0        0        0    29060 2023-05-16 14:30:55.000000 denmune-1.16.5/README.md
--rw-rw-rw-   0        0        0      108 2021-12-23 20:19:35.000000 denmune-1.16.5/pyproject.toml
--rw-rw-rw-   0        0        0      810 2023-05-20 11:18:23.453024 denmune-1.16.5/setup.cfg
--rw-rw-rw-   0        0        0      257 2023-05-16 13:50:59.000000 denmune-1.16.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-20 11:18:23.329999 denmune-1.16.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-20 11:18:23.409286 denmune-1.16.5/src/denmune/
--rw-rw-rw-   0        0        0       28 2022-05-12 02:48:25.000000 denmune-1.16.5/src/denmune/__init__.py
--rw-rw-rw-   0        0        0    39270 2023-05-20 11:14:32.000000 denmune-1.16.5/src/denmune/denmune.py
-drwxrwxrwx   0        0        0        0 2023-05-20 11:18:23.440780 denmune-1.16.5/src/denmune.egg-info/
--rw-rw-rw-   0        0        0    29731 2023-05-20 11:18:23.000000 denmune-1.16.5/src/denmune.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-05-20 11:18:23.000000 denmune-1.16.5/src/denmune.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 11:18:23.000000 denmune-1.16.5/src/denmune.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2023-05-20 11:18:23.000000 denmune-1.16.5/src/denmune.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-20 11:18:23.000000 denmune-1.16.5/src/denmune.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 03:25:51.536023 denmune-1.16.6/
+-rw-rw-rw-   0        0        0     1498 2021-12-31 23:30:13.000000 denmune-1.16.6/LICENSE
+-rw-rw-rw-   0        0        0       47 2021-12-27 21:52:58.000000 denmune-1.16.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    29731 2023-07-01 03:25:51.537026 denmune-1.16.6/PKG-INFO
+-rw-rw-rw-   0        0        0    29060 2023-05-16 14:30:55.000000 denmune-1.16.6/README.md
+-rw-rw-rw-   0        0        0      108 2021-12-23 20:19:35.000000 denmune-1.16.6/pyproject.toml
+-rw-rw-rw-   0        0        0      810 2023-07-01 03:25:51.553358 denmune-1.16.6/setup.cfg
+-rw-rw-rw-   0        0        0      257 2023-05-16 13:50:59.000000 denmune-1.16.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 03:25:51.416618 denmune-1.16.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-01 03:25:51.493194 denmune-1.16.6/src/denmune/
+-rw-rw-rw-   0        0        0       28 2022-05-12 02:48:25.000000 denmune-1.16.6/src/denmune/__init__.py
+-rw-rw-rw-   0        0        0    39270 2023-05-20 11:14:32.000000 denmune-1.16.6/src/denmune/denmune.py
+drwxrwxrwx   0        0        0        0 2023-07-01 03:25:51.534018 denmune-1.16.6/src/denmune.egg-info/
+-rw-rw-rw-   0        0        0    29731 2023-07-01 03:25:51.000000 denmune-1.16.6/src/denmune.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-07-01 03:25:51.000000 denmune-1.16.6/src/denmune.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 03:25:51.000000 denmune-1.16.6/src/denmune.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2023-07-01 03:25:51.000000 denmune-1.16.6/src/denmune.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-01 03:25:51.000000 denmune-1.16.6/src/denmune.egg-info/top_level.txt
```

### Comparing `denmune-1.16.5/LICENSE` & `denmune-1.16.6/LICENSE`

 * *Files identical despite different names*

### Comparing `denmune-1.16.5/PKG-INFO` & `denmune-1.16.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denmune
-Version: 1.16.5
+Version: 1.16.6
 Summary: This is the package for DenMune Clustering Algorithm published in paper https://doi.org/10.1016/j.patcog.2020.107589
 Home-page: https://github.com/scikit-learn-contrib/denmune-clustering-algorithm
 Author: Dr. Mohamed Ali Abbas & Prof. Amin  Shoukry
 Author-email: mohamed.alyabbas@outlook.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `denmune-1.16.5/README.md` & `denmune-1.16.6/README.md`

 * *Files identical despite different names*

### Comparing `denmune-1.16.5/setup.cfg` & `denmune-1.16.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 656e 6d75 6e65 0d0a 7665 7273   = denmune..vers
-00000020: 696f 6e20 3d20 312e 3136 2e35 0d0a 6175  ion = 1.16.5..au
+00000020: 696f 6e20 3d20 312e 3136 2e36 0d0a 6175  ion = 1.16.6..au
 00000030: 7468 6f72 203d 2044 722e 204d 6f68 616d  thor = Dr. Moham
 00000040: 6564 2041 6c69 2041 6262 6173 2026 2050  ed Ali Abbas & P
 00000050: 726f 662e 2041 6d69 6e20 2053 686f 756b  rof. Amin  Shouk
 00000060: 7279 0d0a 6175 7468 6f72 5f65 6d61 696c  ry..author_email
 00000070: 203d 206d 6f68 616d 6564 2e61 6c79 6162   = mohamed.alyab
 00000080: 6261 7340 6f75 746c 6f6f 6b2e 636f 6d0d  bas@outlook.com.
 00000090: 0a64 6573 6372 6970 7469 6f6e 203d 2054  .description = T
```

### Comparing `denmune-1.16.5/src/denmune/denmune.py` & `denmune-1.16.6/src/denmune/denmune.py`

 * *Files identical despite different names*

### Comparing `denmune-1.16.5/src/denmune.egg-info/PKG-INFO` & `denmune-1.16.6/src/denmune.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denmune
-Version: 1.16.5
+Version: 1.16.6
 Summary: This is the package for DenMune Clustering Algorithm published in paper https://doi.org/10.1016/j.patcog.2020.107589
 Home-page: https://github.com/scikit-learn-contrib/denmune-clustering-algorithm
 Author: Dr. Mohamed Ali Abbas & Prof. Amin  Shoukry
 Author-email: mohamed.alyabbas@outlook.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

