# Comparing `tmp/xia_storer-0.1.3-cp39-none-win_amd64.whl.zip` & `tmp/xia_storer-0.1.4-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 2498 bytes, number of entries: 7
--rw-r--r--  2.0 unx      115 b- defN 23-Jun-30 11:39 xia_storer/__init__.py
--rw-r--r--  2.0 unx     1994 b- defN 23-Jun-30 11:39 xia_storer/storer.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:42 xia_storer-0.1.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      386 b- defN 23-Jun-30 11:42 xia_storer-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:42 xia_storer-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-30 11:42 xia_storer-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      558 b- defN 23-Jun-30 11:42 xia_storer-0.1.3.dist-info/RECORD
+-rw-r--r--  2.0 unx      115 b- defN 23-Jul-01 18:15 xia_storer/__init__.py
+-rw-r--r--  2.0 unx     1994 b- defN 23-Jul-01 18:15 xia_storer/storer.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jul-01 18:18 xia_storer-0.1.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      386 b- defN 23-Jul-01 18:18 xia_storer-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 18:18 xia_storer-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-01 18:18 xia_storer-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      558 b- defN 23-Jul-01 18:18 xia_storer-0.1.4.dist-info/RECORD
 7 files, 3314 bytes uncompressed, 1504 bytes compressed:  54.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_storer/__init__.py
 Comment: 
 
 Filename: xia_storer/storer.py
 Comment: 
 
-Filename: xia_storer-0.1.3.dist-info/LICENSE.txt
+Filename: xia_storer-0.1.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_storer-0.1.3.dist-info/METADATA
+Filename: xia_storer-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: xia_storer-0.1.3.dist-info/WHEEL
+Filename: xia_storer-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: xia_storer-0.1.3.dist-info/top_level.txt
+Filename: xia_storer-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_storer-0.1.3.dist-info/RECORD
+Filename: xia_storer-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_storer/__init__.py

```diff
@@ -2,8 +2,8 @@
 
 
 __all__ = [
     'Storer', "FileStorer"
 ]
 
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
```

