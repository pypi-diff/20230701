# Comparing `tmp/xia_engine_bigquery-0.1.13-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_bigquery-0.1.14-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 12066 bytes, number of entries: 9
--rw-r--r--  2.0 unx      361 b- defN 23-Jun-30 13:28 xia_engine_bigquery/__init__.py
--rw-r--r--  2.0 unx    30111 b- defN 23-Jun-30 13:28 xia_engine_bigquery/engine.py
--rw-r--r--  2.0 unx     5338 b- defN 23-Jun-30 13:28 xia_engine_bigquery/proto.py
--rw-r--r--  2.0 unx     5526 b- defN 23-Jun-30 13:28 xia_engine_bigquery/schema.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 13:28 xia_engine_bigquery-0.1.13.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      568 b- defN 23-Jun-30 13:28 xia_engine_bigquery-0.1.13.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 13:28 xia_engine_bigquery-0.1.13.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Jun-30 13:28 xia_engine_bigquery-0.1.13.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      798 b- defN 23-Jun-30 13:28 xia_engine_bigquery-0.1.13.dist-info/RECORD
-9 files, 42972 bytes uncompressed, 10670 bytes compressed:  75.2%
+Zip file size: 12073 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      361 b- defN 23-Jul-01 18:13 xia_engine_bigquery/__init__.py
+-rw-r--r--  2.0 unx    30111 b- defN 23-Jun-29 20:47 xia_engine_bigquery/engine.py
+-rw-r--r--  2.0 unx     5338 b- defN 23-Jun-29 20:47 xia_engine_bigquery/proto.py
+-rw-r--r--  2.0 unx     5526 b- defN 23-Jun-29 20:47 xia_engine_bigquery/schema.py
+-rw-r--r--  2.0 unx      151 b- defN 23-Jul-01 18:13 xia_engine_bigquery-0.1.14.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      568 b- defN 23-Jul-01 18:13 xia_engine_bigquery-0.1.14.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jul-01 18:13 xia_engine_bigquery-0.1.14.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Jul-01 18:13 xia_engine_bigquery-0.1.14.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      799 b- defN 23-Jul-01 18:13 xia_engine_bigquery-0.1.14.dist-info/RECORD
+9 files, 42982 bytes uncompressed, 10677 bytes compressed:  75.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: xia_engine_bigquery/proto.py
 Comment: 
 
 Filename: xia_engine_bigquery/schema.py
 Comment: 
 
-Filename: xia_engine_bigquery-0.1.13.dist-info/LICENSE.txt
+Filename: xia_engine_bigquery-0.1.14.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_bigquery-0.1.13.dist-info/METADATA
+Filename: xia_engine_bigquery-0.1.14.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_bigquery-0.1.13.dist-info/WHEEL
+Filename: xia_engine_bigquery-0.1.14.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_bigquery-0.1.13.dist-info/top_level.txt
+Filename: xia_engine_bigquery-0.1.14.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_bigquery-0.1.13.dist-info/RECORD
+Filename: xia_engine_bigquery-0.1.14.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_bigquery/__init__.py

```diff
@@ -5,8 +5,8 @@
 
 __all__ = [
     "DocToProto",
     "DocToSchema",
     "BigqueryWriteEngine", "BigqueryStreamEngine", "BigqueryAppendOnlyEngine"
 ]
 
-__version__ = "0.1.13"
+__version__ = "0.1.14"
```

## Comparing `xia_engine_bigquery-0.1.13.dist-info/METADATA` & `xia_engine_bigquery-0.1.14.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-engine-bigquery
-Version: 0.1.13
+Version: 0.1.14
 Summary: UNKNOWN
-Home-page: https://develop.x-i-a.com/docs/xia-engine-bigquery/0.1.13/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-bigquery/0.1.14/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

