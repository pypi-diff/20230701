# Comparing `tmp/xia_coder-0.0.7-cp39-none-win_amd64.whl.zip` & `tmp/xia_coder-0.0.8-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3805 bytes, number of entries: 7
--rw-r--r--  2.0 unx       83 b- defN 23-Jun-30 11:18 xia_coder/__init__.py
+Zip file size: 3803 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       83 b- defN 23-Jul-01 17:49 xia_coder/__init__.py
 -rw-r--r--  2.0 unx     6257 b- defN 23-Jun-29 20:38 xia_coder/coder.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:22 xia_coder-0.0.7.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      410 b- defN 23-Jun-30 11:22 xia_coder-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:22 xia_coder-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-30 11:22 xia_coder-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      549 b- defN 23-Jun-30 11:22 xia_coder-0.0.7.dist-info/RECORD
-7 files, 7559 bytes uncompressed, 2827 bytes compressed:  62.6%
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jul-01 17:51 xia_coder-0.0.8.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      410 b- defN 23-Jul-01 17:51 xia_coder-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 17:51 xia_coder-0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-01 17:51 xia_coder-0.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      549 b- defN 23-Jul-01 17:51 xia_coder-0.0.8.dist-info/RECORD
+7 files, 7559 bytes uncompressed, 2825 bytes compressed:  62.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_coder/__init__.py
 Comment: 
 
 Filename: xia_coder/coder.py
 Comment: 
 
-Filename: xia_coder-0.0.7.dist-info/LICENSE.txt
+Filename: xia_coder-0.0.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_coder-0.0.7.dist-info/METADATA
+Filename: xia_coder-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: xia_coder-0.0.7.dist-info/WHEEL
+Filename: xia_coder-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: xia_coder-0.0.7.dist-info/top_level.txt
+Filename: xia_coder-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_coder-0.0.7.dist-info/RECORD
+Filename: xia_coder-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_coder/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_coder.coder import Coder
 
 __all__ = [
     "Coder"
 ]
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
```

