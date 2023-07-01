# Comparing `tmp/xia_cache-0.1.5-cp39-none-win_amd64.whl.zip` & `tmp/xia_cache-0.1.6-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2699 bytes, number of entries: 7
--rw-r--r--  2.0 unx      113 b- defN 23-Jun-30 11:16 xia_cache/__init__.py
--rw-r--r--  2.0 unx     3965 b- defN 23-Jun-30 11:16 xia_cache/cache.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:21 xia_cache-0.1.5.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      436 b- defN 23-Jun-30 11:21 xia_cache-0.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:21 xia_cache-0.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-30 11:21 xia_cache-0.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      550 b- defN 23-Jun-30 11:21 xia_cache-0.1.5.dist-info/RECORD
-7 files, 5324 bytes uncompressed, 1721 bytes compressed:  67.7%
+Zip file size: 2701 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      113 b- defN 23-Jul-01 18:15 xia_cache/__init__.py
+-rw-r--r--  2.0 unx     3965 b- defN 23-Jul-01 18:15 xia_cache/cache.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jul-01 18:16 xia_cache-0.1.6.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      436 b- defN 23-Jul-01 18:16 xia_cache-0.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 18:16 xia_cache-0.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-01 18:16 xia_cache-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      550 b- defN 23-Jul-01 18:16 xia_cache-0.1.6.dist-info/RECORD
+7 files, 5324 bytes uncompressed, 1723 bytes compressed:  67.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_cache/__init__.py
 Comment: 
 
 Filename: xia_cache/cache.py
 Comment: 
 
-Filename: xia_cache-0.1.5.dist-info/LICENSE.txt
+Filename: xia_cache-0.1.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_cache-0.1.5.dist-info/METADATA
+Filename: xia_cache-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: xia_cache-0.1.5.dist-info/WHEEL
+Filename: xia_cache-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: xia_cache-0.1.5.dist-info/top_level.txt
+Filename: xia_cache-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_cache-0.1.5.dist-info/RECORD
+Filename: xia_cache-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_cache/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_cache.cache import Cache, LruRamCache
 
 
 __all__ = [
     "Cache", "LruRamCache",
 ]
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
```

