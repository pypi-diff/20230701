# Comparing `tmp/xia_service-0.0.5-cp39-none-win_amd64.whl.zip` & `tmp/xia_service-0.0.6-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2398 bytes, number of entries: 7
--rw-r--r--  2.0 unx       93 b- defN 23-Jun-30 11:37 xia_service/__init__.py
--rw-r--r--  2.0 unx     1269 b- defN 23-Jun-30 11:37 xia_service/service.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:40 xia_service-0.0.5.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      440 b- defN 23-Jun-30 11:40 xia_service-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:40 xia_service-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-30 11:40 xia_service-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      565 b- defN 23-Jun-30 11:40 xia_service-0.0.5.dist-info/RECORD
-7 files, 2629 bytes uncompressed, 1388 bytes compressed:  47.2%
+Zip file size: 2395 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       93 b- defN 23-Jul-01 18:09 xia_service/__init__.py
+-rw-r--r--  2.0 unx     1269 b- defN 23-Jun-29 20:57 xia_service/service.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jul-01 18:12 xia_service-0.0.6.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      440 b- defN 23-Jul-01 18:12 xia_service-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 18:12 xia_service-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jul-01 18:12 xia_service-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      565 b- defN 23-Jul-01 18:12 xia_service-0.0.6.dist-info/RECORD
+7 files, 2629 bytes uncompressed, 1385 bytes compressed:  47.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_service/__init__.py
 Comment: 
 
 Filename: xia_service/service.py
 Comment: 
 
-Filename: xia_service-0.0.5.dist-info/LICENSE.txt
+Filename: xia_service-0.0.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_service-0.0.5.dist-info/METADATA
+Filename: xia_service-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: xia_service-0.0.5.dist-info/WHEEL
+Filename: xia_service-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: xia_service-0.0.5.dist-info/top_level.txt
+Filename: xia_service-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_service-0.0.5.dist-info/RECORD
+Filename: xia_service-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_service/__init__.py

```diff
@@ -2,8 +2,8 @@
 
 
 __all__ = [
     "Service"
 ]
 
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
```

