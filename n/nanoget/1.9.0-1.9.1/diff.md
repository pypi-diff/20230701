# Comparing `tmp/nanoget-1.9.0.tar.gz` & `tmp/nanoget-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nanoget-1.9.0.tar", last modified: Tue Aug 27 11:47:26 2019, max compression
+gzip compressed data, was "dist/nanoget-1.9.1.tar", last modified: Tue Oct 22 05:26:10 2019, max compression
```

## Comparing `nanoget-1.9.0.tar` & `nanoget-1.9.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-08-27 11:47:26.000000 nanoget-1.9.0/
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       66 2019-03-15 13:38:08.000000 nanoget-1.9.0/MANIFEST.in
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)     2455 2019-08-27 11:47:26.000000 nanoget-1.9.0/PKG-INFO
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)     1415 2019-01-29 10:18:36.000000 nanoget-1.9.0/README.md
-drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-08-27 11:47:26.000000 nanoget-1.9.0/nanoget/
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       56 2019-01-29 10:18:36.000000 nanoget-1.9.0/nanoget/__init__.py
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)    17048 2019-08-27 11:29:24.000000 nanoget-1.9.0/nanoget/extraction_functions.py
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)     6345 2019-08-27 10:41:28.000000 nanoget-1.9.0/nanoget/nanoget.py
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     1320 2019-08-27 11:28:32.000000 nanoget-1.9.0/nanoget/utils.py
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       22 2019-07-23 09:43:40.000000 nanoget-1.9.0/nanoget/version.py
-drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-08-27 11:47:26.000000 nanoget-1.9.0/nanoget.egg-info/
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)     2455 2019-08-27 11:47:26.000000 nanoget-1.9.0/nanoget.egg-info/PKG-INFO
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)      333 2019-08-27 11:47:26.000000 nanoget-1.9.0/nanoget.egg-info/SOURCES.txt
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)        1 2019-08-27 11:47:26.000000 nanoget-1.9.0/nanoget.egg-info/dependency_links.txt
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       55 2019-08-27 11:47:26.000000 nanoget-1.9.0/nanoget.egg-info/requires.txt
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       16 2019-08-27 11:47:26.000000 nanoget-1.9.0/nanoget.egg-info/top_level.txt
-drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-08-27 11:47:26.000000 nanoget-1.9.0/scripts/
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)      537 2019-03-15 13:35:45.000000 nanoget-1.9.0/scripts/test.py
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       85 2019-03-15 13:35:58.000000 nanoget-1.9.0/scripts/test.sh
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       70 2019-08-27 11:47:26.000000 nanoget-1.9.0/setup.cfg
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)     1440 2019-01-29 10:18:36.000000 nanoget-1.9.0/setup.py
+drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-10-22 05:26:10.000000 nanoget-1.9.1/
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       66 2019-03-15 13:38:08.000000 nanoget-1.9.1/MANIFEST.in
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)     2455 2019-10-22 05:26:10.000000 nanoget-1.9.1/PKG-INFO
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)     1415 2019-01-29 10:18:36.000000 nanoget-1.9.1/README.md
+drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-10-22 05:26:10.000000 nanoget-1.9.1/nanoget/
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       56 2019-01-29 10:18:36.000000 nanoget-1.9.1/nanoget/__init__.py
+-rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)    17064 2019-10-21 14:13:28.000000 nanoget-1.9.1/nanoget/extraction_functions.py
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)     6345 2019-08-27 10:41:28.000000 nanoget-1.9.1/nanoget/nanoget.py
+-rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     1320 2019-08-27 11:28:32.000000 nanoget-1.9.1/nanoget/utils.py
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       22 2019-10-21 14:14:00.000000 nanoget-1.9.1/nanoget/version.py
+drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-10-22 05:26:10.000000 nanoget-1.9.1/nanoget.egg-info/
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)     2455 2019-10-22 05:26:09.000000 nanoget-1.9.1/nanoget.egg-info/PKG-INFO
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)      333 2019-10-22 05:26:10.000000 nanoget-1.9.1/nanoget.egg-info/SOURCES.txt
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)        1 2019-10-22 05:26:09.000000 nanoget-1.9.1/nanoget.egg-info/dependency_links.txt
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       55 2019-10-22 05:26:09.000000 nanoget-1.9.1/nanoget.egg-info/requires.txt
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       16 2019-10-22 05:26:09.000000 nanoget-1.9.1/nanoget.egg-info/top_level.txt
+drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-10-22 05:26:10.000000 nanoget-1.9.1/scripts/
+-rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)      537 2019-03-15 13:35:45.000000 nanoget-1.9.1/scripts/test.py
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       85 2019-03-15 13:35:58.000000 nanoget-1.9.1/scripts/test.sh
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       70 2019-10-22 05:26:10.000000 nanoget-1.9.1/setup.cfg
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)     1440 2019-01-29 10:18:36.000000 nanoget-1.9.1/setup.py
```

### Comparing `nanoget-1.9.0/PKG-INFO` & `nanoget-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoget
-Version: 1.9.0
+Version: 1.9.1
 Summary: Functions to extract information from Oxford Nanopore sequencing data and alignments.
 Home-page: https://github.com/wdecoster/nanoget
 Author: Wouter De Coster
 Author-email: decosterwouter@gmail.com
 License: MIT
 Description: # nanoget
         This module provides functions to extract useful metrics from Oxford Nanopore sequencing reads and alignments.
```

### Comparing `nanoget-1.9.0/README.md` & `nanoget-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `nanoget-1.9.0/nanoget/extraction_functions.py` & `nanoget-1.9.1/nanoget/extraction_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
     Extracting lengths
     """
     logging.info("Nanoget: Starting to collect statistics from ubam file {}.".format(bam))
     samfile = pysam.AlignmentFile(bam, "rb", check_sq=False)
     if not samfile.has_index():
         pysam.index(bam)
         # Need to reload the samfile after creating index
-        samfile = pysam.AlignmentFile(bam, "rb")
+        samfile = pysam.AlignmentFile(bam, "rb", check_sq=False)
         logging.info("Nanoget: No index for bam file could be found, created index.")
     datadf = pd.DataFrame(
         data=[(read.query_name, nanomath.ave_qual(read.query_qualities), read.query_length)
               for read in samfile.fetch(until_eof=True)],
         columns=["readIDs", "quals", "lengths"]) \
         .dropna(axis='columns', how='all') \
         .dropna(axis='index', how='any')
```

### Comparing `nanoget-1.9.0/nanoget/nanoget.py` & `nanoget-1.9.1/nanoget/nanoget.py`

 * *Files identical despite different names*

### Comparing `nanoget-1.9.0/nanoget/utils.py` & `nanoget-1.9.1/nanoget/utils.py`

 * *Files identical despite different names*

### Comparing `nanoget-1.9.0/nanoget.egg-info/PKG-INFO` & `nanoget-1.9.1/nanoget.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoget
-Version: 1.9.0
+Version: 1.9.1
 Summary: Functions to extract information from Oxford Nanopore sequencing data and alignments.
 Home-page: https://github.com/wdecoster/nanoget
 Author: Wouter De Coster
 Author-email: decosterwouter@gmail.com
 License: MIT
 Description: # nanoget
         This module provides functions to extract useful metrics from Oxford Nanopore sequencing reads and alignments.
```

### Comparing `nanoget-1.9.0/scripts/test.py` & `nanoget-1.9.1/scripts/test.py`

 * *Files identical despite different names*

### Comparing `nanoget-1.9.0/setup.py` & `nanoget-1.9.1/setup.py`

 * *Files identical despite different names*

