# Comparing `tmp/xia_puller_flask-0.0.8-cp39-none-win_amd64.whl.zip` & `tmp/xia_puller_flask-0.0.9-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2463 bytes, number of entries: 7
--rw-r--r--  2.0 unx       96 b- defN 23-Jun-30 11:35 xia_puller_flask/__init__.py
--rw-r--r--  2.0 unx     1104 b- defN 23-Jun-30 11:35 xia_puller_flask/api.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:38 xia_puller_flask-0.0.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      476 b- defN 23-Jun-30 11:38 xia_puller_flask-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:38 xia_puller_flask-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Jun-30 11:38 xia_puller_flask-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      596 b- defN 23-Jun-30 11:38 xia_puller_flask-0.0.8.dist-info/RECORD
-7 files, 2539 bytes uncompressed, 1391 bytes compressed:  45.2%
+Zip file size: 2457 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       96 b- defN 23-Jun-30 21:24 xia_puller_flask/__init__.py
+-rw-r--r--  2.0 unx     1104 b- defN 23-Jun-30 08:48 xia_puller_flask/api.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 21:24 xia_puller_flask-0.0.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      476 b- defN 23-Jun-30 21:24 xia_puller_flask-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 21:24 xia_puller_flask-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-30 21:24 xia_puller_flask-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      596 b- defN 23-Jun-30 21:24 xia_puller_flask-0.0.9.dist-info/RECORD
+7 files, 2539 bytes uncompressed, 1385 bytes compressed:  45.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_puller_flask/__init__.py
 Comment: 
 
 Filename: xia_puller_flask/api.py
 Comment: 
 
-Filename: xia_puller_flask-0.0.8.dist-info/LICENSE.txt
+Filename: xia_puller_flask-0.0.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_puller_flask-0.0.8.dist-info/METADATA
+Filename: xia_puller_flask-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: xia_puller_flask-0.0.8.dist-info/WHEEL
+Filename: xia_puller_flask-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: xia_puller_flask-0.0.8.dist-info/top_level.txt
+Filename: xia_puller_flask-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_puller_flask-0.0.8.dist-info/RECORD
+Filename: xia_puller_flask-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_puller_flask/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_puller_flask.api import PullerApi
 
 __all__ = [
     "PullerApi"
 ]
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
```

