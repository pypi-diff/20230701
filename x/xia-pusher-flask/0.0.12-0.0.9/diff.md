# Comparing `tmp/xia_pusher_flask-0.0.12-cp39-none-macosx_11_0_x86_64.whl.zip` & `tmp/xia_pusher_flask-0.0.9-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2526 bytes, number of entries: 7
--rw-r--r--  2.0 unx       97 b- defN 23-Jul-01 18:08 xia_pusher_flask/__init__.py
--rw-r--r--  2.0 unx     1212 b- defN 23-Jun-29 20:58 xia_pusher_flask/api.py
--rw-r--r--  2.0 unx      151 b- defN 23-Jul-01 18:08 xia_pusher_flask-0.0.12.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      478 b- defN 23-Jul-01 18:08 xia_pusher_flask-0.0.12.dist-info/METADATA
--rw-r--r--  2.0 unx      108 b- defN 23-Jul-01 18:08 xia_pusher_flask-0.0.12.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Jul-01 18:08 xia_pusher_flask-0.0.12.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      602 b- defN 23-Jul-01 18:08 xia_pusher_flask-0.0.12.dist-info/RECORD
-7 files, 2665 bytes uncompressed, 1444 bytes compressed:  45.8%
+Zip file size: 112126 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       97 b- defN 23-Jun-26 13:15 xia_pusher_flask/__init__.py
+-rw-r--r--  2.0 unx   272384 b- defN 23-Jun-26 13:17 xia_pusher_flask/api.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 13:17 xia_pusher_flask-0.0.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      714 b- defN 23-Jun-26 13:17 xia_pusher_flask-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 13:17 xia_pusher_flask-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-26 13:17 xia_pusher_flask-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      614 b- defN 23-Jun-26 13:17 xia_pusher_flask-0.0.9.dist-info/RECORD
+7 files, 274076 bytes uncompressed, 111022 bytes compressed:  59.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_pusher_flask/__init__.py
 Comment: 
 
-Filename: xia_pusher_flask/api.py
+Filename: xia_pusher_flask/api.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_pusher_flask-0.0.12.dist-info/LICENSE.txt
+Filename: xia_pusher_flask-0.0.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_pusher_flask-0.0.12.dist-info/METADATA
+Filename: xia_pusher_flask-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: xia_pusher_flask-0.0.12.dist-info/WHEEL
+Filename: xia_pusher_flask-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: xia_pusher_flask-0.0.12.dist-info/top_level.txt
+Filename: xia_pusher_flask-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_pusher_flask-0.0.12.dist-info/RECORD
+Filename: xia_pusher_flask-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_pusher_flask/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_pusher_flask.api import PusherApi
 
 __all__ = [
     "PusherApi"
 ]
 
-__version__ = "0.0.12"
+__version__ = "0.0.9"
```

