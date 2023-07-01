# Comparing `tmp/xia_api_flask-0.1.18-cp39-none-win_amd64.whl.zip` & `tmp/xia_api_flask-0.1.19-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5970 bytes, number of entries: 7
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 11:14 xia_api_flask/__init__.py
--rw-r--r--  2.0 unx    18246 b- defN 23-Jun-29 20:33 xia_api_flask/rest.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:18 xia_api_flask-0.1.18.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      507 b- defN 23-Jun-30 11:18 xia_api_flask-0.1.18.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:18 xia_api_flask-0.1.18.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Jun-30 11:18 xia_api_flask-0.1.18.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      582 b- defN 23-Jun-30 11:18 xia_api_flask-0.1.18.dist-info/RECORD
-7 files, 19691 bytes uncompressed, 4928 bytes compressed:  75.0%
+Zip file size: 5976 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-01 17:47 xia_api_flask/__init__.py
+-rw-r--r--  2.0 unx    18246 b- defN 23-Jun-29 20:35 xia_api_flask/rest.py
+-rw-r--r--  2.0 unx      151 b- defN 23-Jul-01 17:48 xia_api_flask-0.1.19.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      507 b- defN 23-Jul-01 17:48 xia_api_flask-0.1.19.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jul-01 17:48 xia_api_flask-0.1.19.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Jul-01 17:48 xia_api_flask-0.1.19.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      583 b- defN 23-Jul-01 17:48 xia_api_flask-0.1.19.dist-info/RECORD
+7 files, 19701 bytes uncompressed, 4934 bytes compressed:  75.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_api_flask/__init__.py
 Comment: 
 
 Filename: xia_api_flask/rest.py
 Comment: 
 
-Filename: xia_api_flask-0.1.18.dist-info/LICENSE.txt
+Filename: xia_api_flask-0.1.19.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_api_flask-0.1.18.dist-info/METADATA
+Filename: xia_api_flask-0.1.19.dist-info/METADATA
 Comment: 
 
-Filename: xia_api_flask-0.1.18.dist-info/WHEEL
+Filename: xia_api_flask-0.1.19.dist-info/WHEEL
 Comment: 
 
-Filename: xia_api_flask-0.1.18.dist-info/top_level.txt
+Filename: xia_api_flask-0.1.19.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_api_flask-0.1.18.dist-info/RECORD
+Filename: xia_api_flask-0.1.19.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_api_flask/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_api_flask.rest import Restful
 
 __all__ = [
     "Restful",
 ]
 
-__version__ = "0.1.18"
+__version__ = "0.1.19"
```

