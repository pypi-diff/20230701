# Comparing `tmp/xia_engine_sql-0.2.3-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_sql-0.2.4-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 10964 bytes, number of entries: 7
--rw-r--r--  2.0 unx      170 b- defN 23-Jun-30 11:23 xia_engine_sql/__init__.py
--rw-r--r--  2.0 unx    41248 b- defN 23-Jun-30 11:23 xia_engine_sql/engine.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:27 xia_engine_sql-0.2.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      420 b- defN 23-Jun-30 11:27 xia_engine_sql-0.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:27 xia_engine_sql-0.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jun-30 11:27 xia_engine_sql-0.2.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      587 b- defN 23-Jun-30 11:27 xia_engine_sql-0.2.3.dist-info/RECORD
-7 files, 42690 bytes uncompressed, 9914 bytes compressed:  76.8%
+Zip file size: 10968 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      170 b- defN 23-Jul-01 17:57 xia_engine_sql/__init__.py
+-rw-r--r--  2.0 unx    41248 b- defN 23-Jun-30 11:24 xia_engine_sql/engine.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jul-01 17:59 xia_engine_sql-0.2.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      420 b- defN 23-Jul-01 17:59 xia_engine_sql-0.2.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 17:59 xia_engine_sql-0.2.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jul-01 17:59 xia_engine_sql-0.2.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      587 b- defN 23-Jul-01 17:59 xia_engine_sql-0.2.4.dist-info/RECORD
+7 files, 42690 bytes uncompressed, 9918 bytes compressed:  76.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_sql/__init__.py
 Comment: 
 
 Filename: xia_engine_sql/engine.py
 Comment: 
 
-Filename: xia_engine_sql-0.2.3.dist-info/LICENSE.txt
+Filename: xia_engine_sql-0.2.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_sql-0.2.3.dist-info/METADATA
+Filename: xia_engine_sql-0.2.4.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_sql-0.2.3.dist-info/WHEEL
+Filename: xia_engine_sql-0.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_sql-0.2.3.dist-info/top_level.txt
+Filename: xia_engine_sql-0.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_sql-0.2.3.dist-info/RECORD
+Filename: xia_engine_sql-0.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_sql/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_engine_sql.engine import SqlEngine, SqliteEngine, SqliteConnectParam
 
 
 __all__ = [
     "SqlEngine", "SqliteEngine", "SqliteConnectParam"
 ]
 
-__version__ = "0.2.3"
+__version__ = "0.2.4"
```

