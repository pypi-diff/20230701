# Comparing `tmp/xia_token_flask-0.1.15-cp39-none-win_amd64.whl.zip` & `tmp/xia_token_flask-0.1.16-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5294 bytes, number of entries: 7
--rw-r--r--  2.0 unx      102 b- defN 23-Jun-30 11:42 xia_token_flask/__init__.py
--rw-r--r--  2.0 unx    17714 b- defN 23-Jun-30 10:38 xia_token_flask/token.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:44 xia_token_flask-0.1.15.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      466 b- defN 23-Jun-30 11:44 xia_token_flask-0.1.15.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:44 xia_token_flask-0.1.15.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-30 11:44 xia_token_flask-0.1.15.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      598 b- defN 23-Jun-30 11:44 xia_token_flask-0.1.15.dist-info/RECORD
-7 files, 19146 bytes uncompressed, 4222 bytes compressed:  77.9%
+Zip file size: 5295 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      102 b- defN 23-Jul-01 18:15 xia_token_flask/__init__.py
+-rw-r--r--  2.0 unx    17714 b- defN 23-Jun-30 11:41 xia_token_flask/token.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jul-01 18:18 xia_token_flask-0.1.16.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      466 b- defN 23-Jul-01 18:18 xia_token_flask-0.1.16.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 18:18 xia_token_flask-0.1.16.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-01 18:18 xia_token_flask-0.1.16.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      598 b- defN 23-Jul-01 18:18 xia_token_flask-0.1.16.dist-info/RECORD
+7 files, 19146 bytes uncompressed, 4223 bytes compressed:  77.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_token_flask/__init__.py
 Comment: 
 
 Filename: xia_token_flask/token.py
 Comment: 
 
-Filename: xia_token_flask-0.1.15.dist-info/LICENSE.txt
+Filename: xia_token_flask-0.1.16.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_token_flask-0.1.15.dist-info/METADATA
+Filename: xia_token_flask-0.1.16.dist-info/METADATA
 Comment: 
 
-Filename: xia_token_flask-0.1.15.dist-info/WHEEL
+Filename: xia_token_flask-0.1.16.dist-info/WHEEL
 Comment: 
 
-Filename: xia_token_flask-0.1.15.dist-info/top_level.txt
+Filename: xia_token_flask-0.1.16.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_token_flask-0.1.15.dist-info/RECORD
+Filename: xia_token_flask-0.1.16.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_token_flask/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_token_flask.token import FlaskToken
 
 
 __all__ = [
     "FlaskToken",
 ]
 
-__version__ = "0.1.15"
+__version__ = "0.1.16"
```

