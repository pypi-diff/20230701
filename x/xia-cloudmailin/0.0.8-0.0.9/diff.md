# Comparing `tmp/xia_cloudmailin-0.0.8-cp39-none-win_amd64.whl.zip` & `tmp/xia_cloudmailin-0.0.9-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2529 bytes, number of entries: 7
--rw-r--r--  2.0 unx       97 b- defN 23-Jun-30 11:19 xia_cloudmailin/__init__.py
--rw-r--r--  2.0 unx     1587 b- defN 23-Jun-30 11:19 xia_cloudmailin/mail.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:22 xia_cloudmailin-0.0.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      420 b- defN 23-Jun-30 11:22 xia_cloudmailin-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:22 xia_cloudmailin-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-30 11:22 xia_cloudmailin-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      590 b- defN 23-Jun-30 11:22 xia_cloudmailin-0.0.8.dist-info/RECORD
-7 files, 2960 bytes uncompressed, 1469 bytes compressed:  50.4%
+Zip file size: 2526 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       97 b- defN 23-Jul-01 17:49 xia_cloudmailin/__init__.py
+-rw-r--r--  2.0 unx     1587 b- defN 23-Jul-01 17:49 xia_cloudmailin/mail.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jul-01 17:52 xia_cloudmailin-0.0.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      420 b- defN 23-Jul-01 17:52 xia_cloudmailin-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 17:52 xia_cloudmailin-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-01 17:52 xia_cloudmailin-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      590 b- defN 23-Jul-01 17:52 xia_cloudmailin-0.0.9.dist-info/RECORD
+7 files, 2960 bytes uncompressed, 1466 bytes compressed:  50.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_cloudmailin/__init__.py
 Comment: 
 
 Filename: xia_cloudmailin/mail.py
 Comment: 
 
-Filename: xia_cloudmailin-0.0.8.dist-info/LICENSE.txt
+Filename: xia_cloudmailin-0.0.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_cloudmailin-0.0.8.dist-info/METADATA
+Filename: xia_cloudmailin-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: xia_cloudmailin-0.0.8.dist-info/WHEEL
+Filename: xia_cloudmailin-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: xia_cloudmailin-0.0.8.dist-info/top_level.txt
+Filename: xia_cloudmailin-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_cloudmailin-0.0.8.dist-info/RECORD
+Filename: xia_cloudmailin-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_cloudmailin/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_cloudmailin.mail import CloudMail
 
 
 __all__ = [
     "CloudMail"
 ]
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
```

