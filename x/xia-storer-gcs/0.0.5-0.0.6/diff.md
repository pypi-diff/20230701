# Comparing `tmp/xia_storer_gcs-0.0.5-cp39-none-win_amd64.whl.zip` & `tmp/xia_storer_gcs-0.0.6-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2873 bytes, number of entries: 7
--rw-r--r--  2.0 unx       83 b- defN 23-Jun-30 11:41 xia_storer_gcs/__init__.py
--rw-r--r--  2.0 unx     2653 b- defN 23-Jun-30 11:41 xia_storer_gcs/storer.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:44 xia_storer_gcs-0.0.5.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      477 b- defN 23-Jun-30 11:44 xia_storer_gcs-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:44 xia_storer_gcs-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jun-30 11:44 xia_storer_gcs-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      585 b- defN 23-Jun-30 11:44 xia_storer_gcs-0.0.5.dist-info/RECORD
-7 files, 4063 bytes uncompressed, 1823 bytes compressed:  55.1%
+Zip file size: 2813 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       83 b- defN 23-Jul-01 18:13 xia_storer_gcs/__init__.py
+-rw-r--r--  2.0 unx     2653 b- defN 23-Jul-01 14:33 xia_storer_gcs/storer.py
+-rw-rw-rw-  2.0 unx       67 b- defN 23-Jul-01 18:13 xia_storer_gcs-0.0.6.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      477 b- defN 23-Jul-01 18:13 xia_storer_gcs-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 18:13 xia_storer_gcs-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jul-01 18:13 xia_storer_gcs-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      584 b- defN 23-Jul-01 18:13 xia_storer_gcs-0.0.6.dist-info/RECORD
+7 files, 3978 bytes uncompressed, 1763 bytes compressed:  55.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_storer_gcs/__init__.py
 Comment: 
 
 Filename: xia_storer_gcs/storer.py
 Comment: 
 
-Filename: xia_storer_gcs-0.0.5.dist-info/LICENSE.txt
+Filename: xia_storer_gcs-0.0.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_storer_gcs-0.0.5.dist-info/METADATA
+Filename: xia_storer_gcs-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: xia_storer_gcs-0.0.5.dist-info/WHEEL
+Filename: xia_storer_gcs-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: xia_storer_gcs-0.0.5.dist-info/top_level.txt
+Filename: xia_storer_gcs-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_storer_gcs-0.0.5.dist-info/RECORD
+Filename: xia_storer_gcs-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_storer_gcs/__init__.py

```diff
@@ -1,8 +1,8 @@
 from storer import GcsStorer
 
 __all__ = [
     "GcsStorer"
 ]
 
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
```

