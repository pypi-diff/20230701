# Comparing `tmp/xia_broadcast_fastapi-0.1.2-cp39-none-win_amd64.whl.zip` & `tmp/xia_broadcast_fastapi-0.1.3-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3698 bytes, number of entries: 7
--rw-r--r--  2.0 unx      129 b- defN 23-Jun-30 11:15 xia_broadcast_fastapi/__init__.py
--rw-r--r--  2.0 unx     4771 b- defN 23-Jun-29 20:33 xia_broadcast_fastapi/broadcaster.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:19 xia_broadcast_fastapi-0.1.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      486 b- defN 23-Jun-30 11:19 xia_broadcast_fastapi-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:19 xia_broadcast_fastapi-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-30 11:19 xia_broadcast_fastapi-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      640 b- defN 23-Jun-30 11:19 xia_broadcast_fastapi-0.1.2.dist-info/RECORD
-7 files, 6298 bytes uncompressed, 2540 bytes compressed:  59.7%
+Zip file size: 3701 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      129 b- defN 23-Jul-01 17:48 xia_broadcast_fastapi/__init__.py
+-rw-r--r--  2.0 unx     4771 b- defN 23-Jun-29 20:35 xia_broadcast_fastapi/broadcaster.py
+-rw-r--r--  2.0 unx      151 b- defN 23-Jul-01 17:48 xia_broadcast_fastapi-0.1.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      486 b- defN 23-Jul-01 17:48 xia_broadcast_fastapi-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jul-01 17:48 xia_broadcast_fastapi-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-01 17:48 xia_broadcast_fastapi-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      641 b- defN 23-Jul-01 17:48 xia_broadcast_fastapi-0.1.3.dist-info/RECORD
+7 files, 6308 bytes uncompressed, 2543 bytes compressed:  59.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_broadcast_fastapi/__init__.py
 Comment: 
 
 Filename: xia_broadcast_fastapi/broadcaster.py
 Comment: 
 
-Filename: xia_broadcast_fastapi-0.1.2.dist-info/LICENSE.txt
+Filename: xia_broadcast_fastapi-0.1.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_broadcast_fastapi-0.1.2.dist-info/METADATA
+Filename: xia_broadcast_fastapi-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: xia_broadcast_fastapi-0.1.2.dist-info/WHEEL
+Filename: xia_broadcast_fastapi-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: xia_broadcast_fastapi-0.1.2.dist-info/top_level.txt
+Filename: xia_broadcast_fastapi-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_broadcast_fastapi-0.1.2.dist-info/RECORD
+Filename: xia_broadcast_fastapi-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_broadcast_fastapi/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_broadcast_fastapi.broadcaster import BroadcasterFastapi
 
 
 __all__ = [
     "BroadcasterFastapi",
 ]
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

