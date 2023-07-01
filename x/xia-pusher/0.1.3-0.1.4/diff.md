# Comparing `tmp/xia_pusher-0.1.3-cp39-none-win_amd64.whl.zip` & `tmp/xia_pusher-0.1.4-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 2549 bytes, number of entries: 7
--rw-r--r--  2.0 unx       87 b- defN 23-Jun-30 11:35 xia_pusher/__init__.py
--rw-r--r--  2.0 unx     1743 b- defN 23-Jun-29 20:54 xia_pusher/pusher.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:40 xia_pusher-0.1.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      463 b- defN 23-Jun-30 11:40 xia_pusher-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:40 xia_pusher-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-30 11:40 xia_pusher-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      557 b- defN 23-Jun-30 11:40 xia_pusher-0.1.3.dist-info/RECORD
+-rw-r--r--  2.0 unx       87 b- defN 23-Jul-01 18:04 xia_pusher/__init__.py
+-rw-r--r--  2.0 unx     1743 b- defN 23-Jul-01 18:04 xia_pusher/pusher.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jul-01 18:09 xia_pusher-0.1.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      463 b- defN 23-Jul-01 18:09 xia_pusher-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 18:09 xia_pusher-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-01 18:09 xia_pusher-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      557 b- defN 23-Jul-01 18:09 xia_pusher-0.1.4.dist-info/RECORD
 7 files, 3111 bytes uncompressed, 1555 bytes compressed:  50.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_pusher/__init__.py
 Comment: 
 
 Filename: xia_pusher/pusher.py
 Comment: 
 
-Filename: xia_pusher-0.1.3.dist-info/LICENSE.txt
+Filename: xia_pusher-0.1.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_pusher-0.1.3.dist-info/METADATA
+Filename: xia_pusher-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: xia_pusher-0.1.3.dist-info/WHEEL
+Filename: xia_pusher-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: xia_pusher-0.1.3.dist-info/top_level.txt
+Filename: xia_pusher-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_pusher-0.1.3.dist-info/RECORD
+Filename: xia_pusher-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_pusher/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_pusher.pusher import Pusher
 
 __all__ = [
     "Pusher"
 ]
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
```

