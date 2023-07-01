# Comparing `tmp/xia_puller-0.0.19-cp39-none-win_amd64.whl.zip` & `tmp/xia_puller-0.0.20-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 114705 bytes, number of entries: 7
--rw-r--r--  2.0 unx       88 b- defN 23-Jun-30 11:33 xia_puller/__init__.py
--rw-r--r--  2.0 unx   278528 b- defN 23-Jun-30 11:44 xia_puller/puller.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:44 xia_puller-0.0.19.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      465 b- defN 23-Jun-30 11:44 xia_puller-0.0.19.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:44 xia_puller-0.0.19.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-30 11:44 xia_puller-0.0.19.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      580 b- defN 23-Jun-30 11:44 xia_puller-0.0.19.dist-info/RECORD
-7 files, 279922 bytes uncompressed, 113669 bytes compressed:  59.4%
+Zip file size: 114709 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       89 b- defN 23-Jul-01 13:13 xia_puller/__init__.py
+-rw-r--r--  2.0 unx   278528 b- defN 23-Jul-01 13:15 xia_puller/puller.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jul-01 13:15 xia_puller-0.0.20.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      465 b- defN 23-Jul-01 13:15 xia_puller-0.0.20.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 13:15 xia_puller-0.0.20.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-01 13:15 xia_puller-0.0.20.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      580 b- defN 23-Jul-01 13:15 xia_puller-0.0.20.dist-info/RECORD
+7 files, 279923 bytes uncompressed, 113673 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_puller/__init__.py
 Comment: 
 
 Filename: xia_puller/puller.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_puller-0.0.19.dist-info/LICENSE.txt
+Filename: xia_puller-0.0.20.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_puller-0.0.19.dist-info/METADATA
+Filename: xia_puller-0.0.20.dist-info/METADATA
 Comment: 
 
-Filename: xia_puller-0.0.19.dist-info/WHEEL
+Filename: xia_puller-0.0.20.dist-info/WHEEL
 Comment: 
 
-Filename: xia_puller-0.0.19.dist-info/top_level.txt
+Filename: xia_puller-0.0.20.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_puller-0.0.19.dist-info/RECORD
+Filename: xia_puller-0.0.20.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_puller/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_puller.puller import Puller
 
 __all__ = [
     "Puller"
 ]
 
-__version__ = "0.0.19"
+__version__ = "0.0.20"
```

