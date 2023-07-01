# Comparing `tmp/xia_analytics-0.0.6-cp39-none-win_amd64.whl.zip` & `tmp/xia_analytics-0.0.7-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2287 bytes, number of entries: 7
--rw-r--r--  2.0 unx       95 b- defN 23-Jun-30 11:14 xia_analytics/__init__.py
--rw-r--r--  2.0 unx      750 b- defN 23-Jun-29 20:32 xia_analytics/analyzer.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:17 xia_analytics-0.0.6.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      418 b- defN 23-Jun-30 11:17 xia_analytics-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:17 xia_analytics-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Jun-30 11:17 xia_analytics-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      579 b- defN 23-Jun-30 11:17 xia_analytics-0.0.6.dist-info/RECORD
-7 files, 2106 bytes uncompressed, 1247 bytes compressed:  40.8%
+Zip file size: 2281 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       95 b- defN 23-Jul-01 17:44 xia_analytics/__init__.py
+-rw-r--r--  2.0 unx      750 b- defN 23-Jul-01 17:44 xia_analytics/analyzer.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jul-01 17:47 xia_analytics-0.0.7.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      418 b- defN 23-Jul-01 17:47 xia_analytics-0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 17:47 xia_analytics-0.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Jul-01 17:47 xia_analytics-0.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      579 b- defN 23-Jul-01 17:47 xia_analytics-0.0.7.dist-info/RECORD
+7 files, 2106 bytes uncompressed, 1241 bytes compressed:  41.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_analytics/__init__.py
 Comment: 
 
 Filename: xia_analytics/analyzer.py
 Comment: 
 
-Filename: xia_analytics-0.0.6.dist-info/LICENSE.txt
+Filename: xia_analytics-0.0.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_analytics-0.0.6.dist-info/METADATA
+Filename: xia_analytics-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: xia_analytics-0.0.6.dist-info/WHEEL
+Filename: xia_analytics-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: xia_analytics-0.0.6.dist-info/top_level.txt
+Filename: xia_analytics-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_analytics-0.0.6.dist-info/RECORD
+Filename: xia_analytics-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_analytics/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_analytics.analyzer import Analyzer
 
 __all__ = [
    "Analyzer"
 ]
 
-__version__ = "0.0.6"
+__version__ = "0.0.7"
```

