# Comparing `tmp/xia_logger_gcp-0.1.3-cp39-none-win_amd64.whl.zip` & `tmp/xia_logger_gcp-0.1.4-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2265 bytes, number of entries: 7
--rw-r--r--  2.0 unx       97 b- defN 23-Jun-30 11:32 xia_logger_gcp/__init__.py
--rw-r--r--  2.0 unx      549 b- defN 23-Jun-30 11:32 xia_logger_gcp/logger.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:35 xia_logger_gcp-0.1.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      456 b- defN 23-Jun-30 11:35 xia_logger_gcp-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:35 xia_logger_gcp-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jun-30 11:35 xia_logger_gcp-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      584 b- defN 23-Jun-30 11:35 xia_logger_gcp-0.1.3.dist-info/RECORD
-7 files, 1951 bytes uncompressed, 1215 bytes compressed:  37.7%
+Zip file size: 2274 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       97 b- defN 23-Jul-01 18:03 xia_logger_gcp/__init__.py
+-rw-r--r--  2.0 unx      549 b- defN 23-Jun-29 20:53 xia_logger_gcp/logger.py
+-rw-r--r--  2.0 unx      151 b- defN 23-Jul-01 18:03 xia_logger_gcp-0.1.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      456 b- defN 23-Jul-01 18:03 xia_logger_gcp-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jul-01 18:03 xia_logger_gcp-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jul-01 18:03 xia_logger_gcp-0.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      585 b- defN 23-Jul-01 18:03 xia_logger_gcp-0.1.4.dist-info/RECORD
+7 files, 1961 bytes uncompressed, 1224 bytes compressed:  37.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_logger_gcp/__init__.py
 Comment: 
 
 Filename: xia_logger_gcp/logger.py
 Comment: 
 
-Filename: xia_logger_gcp-0.1.3.dist-info/LICENSE.txt
+Filename: xia_logger_gcp-0.1.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_logger_gcp-0.1.3.dist-info/METADATA
+Filename: xia_logger_gcp-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: xia_logger_gcp-0.1.3.dist-info/WHEEL
+Filename: xia_logger_gcp-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: xia_logger_gcp-0.1.3.dist-info/top_level.txt
+Filename: xia_logger_gcp-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_logger_gcp-0.1.3.dist-info/RECORD
+Filename: xia_logger_gcp-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_logger_gcp/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_logger_gcp.logger import GcpLogger
 
 __all__ = [
     "GcpLogger"
 ]
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
```

