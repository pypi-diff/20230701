# Comparing `tmp/xia_logger-0.1.4-cp39-none-win_amd64.whl.zip` & `tmp/xia_logger-0.1.5-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4794 bytes, number of entries: 7
--rw-r--r--  2.0 unx      159 b- defN 23-Jun-30 11:29 xia_logger/__init__.py
--rw-r--r--  2.0 unx    11135 b- defN 23-Jun-30 11:29 xia_logger/logger.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:33 xia_logger-0.1.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      489 b- defN 23-Jun-30 11:33 xia_logger-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:33 xia_logger-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-30 11:33 xia_logger-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      559 b- defN 23-Jun-30 11:33 xia_logger-0.1.4.dist-info/RECORD
-7 files, 12603 bytes uncompressed, 3800 bytes compressed:  69.8%
+Zip file size: 4796 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      159 b- defN 23-Jul-01 18:01 xia_logger/__init__.py
+-rw-r--r--  2.0 unx    11135 b- defN 23-Jun-30 10:34 xia_logger/logger.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jul-01 18:06 xia_logger-0.1.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      489 b- defN 23-Jul-01 18:06 xia_logger-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 18:06 xia_logger-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-01 18:06 xia_logger-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      559 b- defN 23-Jul-01 18:06 xia_logger-0.1.5.dist-info/RECORD
+7 files, 12603 bytes uncompressed, 3802 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_logger/__init__.py
 Comment: 
 
 Filename: xia_logger/logger.py
 Comment: 
 
-Filename: xia_logger-0.1.4.dist-info/LICENSE.txt
+Filename: xia_logger-0.1.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_logger-0.1.4.dist-info/METADATA
+Filename: xia_logger-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: xia_logger-0.1.4.dist-info/WHEEL
+Filename: xia_logger-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: xia_logger-0.1.4.dist-info/top_level.txt
+Filename: xia_logger-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_logger-0.1.4.dist-info/RECORD
+Filename: xia_logger-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_logger/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_logger.logger import Logger, HttpLogger, JsonLogger, DataLog
 
 __all__ = [
     "Logger", "HttpLogger", "JsonLogger", "DataLog"
 ]
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
```

