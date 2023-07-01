# Comparing `tmp/xia_easy_proto-1.0.7-cp39-none-win_amd64.whl.zip` & `tmp/xia_easy_proto-1.0.8-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3500 bytes, number of entries: 7
--rw-r--r--  2.0 unx       96 b- defN 23-Jun-30 11:22 xia_easy_proto/__init__.py
--rw-r--r--  2.0 unx     6009 b- defN 23-Jun-30 09:52 xia_easy_proto/proto.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:24 xia_easy_proto-1.0.7.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      418 b- defN 23-Jun-30 11:24 xia_easy_proto-1.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:24 xia_easy_proto-1.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jun-30 11:24 xia_easy_proto-1.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      584 b- defN 23-Jun-30 11:24 xia_easy_proto-1.0.7.dist-info/RECORD
-7 files, 7372 bytes uncompressed, 2452 bytes compressed:  66.7%
+Zip file size: 3501 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       96 b- defN 23-Jul-01 17:53 xia_easy_proto/__init__.py
+-rw-r--r--  2.0 unx     6009 b- defN 23-Jul-01 17:53 xia_easy_proto/proto.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jul-01 17:53 xia_easy_proto-1.0.8.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      418 b- defN 23-Jul-01 17:53 xia_easy_proto-1.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 17:53 xia_easy_proto-1.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jul-01 17:53 xia_easy_proto-1.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      584 b- defN 23-Jul-01 17:53 xia_easy_proto-1.0.8.dist-info/RECORD
+7 files, 7372 bytes uncompressed, 2453 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_easy_proto/__init__.py
 Comment: 
 
 Filename: xia_easy_proto/proto.py
 Comment: 
 
-Filename: xia_easy_proto-1.0.7.dist-info/LICENSE.txt
+Filename: xia_easy_proto-1.0.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_easy_proto-1.0.7.dist-info/METADATA
+Filename: xia_easy_proto-1.0.8.dist-info/METADATA
 Comment: 
 
-Filename: xia_easy_proto-1.0.7.dist-info/WHEEL
+Filename: xia_easy_proto-1.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: xia_easy_proto-1.0.7.dist-info/top_level.txt
+Filename: xia_easy_proto-1.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_easy_proto-1.0.7.dist-info/RECORD
+Filename: xia_easy_proto-1.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_easy_proto/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_easy_proto.proto import EasyProto
 
 __all__ = [
     "EasyProto"
 ]
 
-__version__ = "1.0.7"
+__version__ = "1.0.8"
```

## Comparing `xia_easy_proto-1.0.7.dist-info/RECORD` & `xia_easy_proto-1.0.8.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_easy_proto/__init__.py,sha256=bMUnBIxTwbSq8AI6IyMakov3awrUyMQZUcjbPCTJ0ow,96
+xia_easy_proto/__init__.py,sha256=gcMtE_ySMOqBv6PVnlAhwk3mA7EQ0Nc4oS4W_HzdeR0,96
 xia_easy_proto/proto.py,sha256=r9ca8pyRsSMvFQgIrcMJdeGVNchGNPgAEfLrj05Y3Qs,6009
-xia_easy_proto-1.0.7.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
-xia_easy_proto-1.0.7.dist-info/METADATA,sha256=bNP7jCffNByipJJLTgEWTnd4IJ0_K2hmt-jd453j7dI,418
-xia_easy_proto-1.0.7.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_easy_proto-1.0.7.dist-info/top_level.txt,sha256=KPFU7QdTuBBTOvgTGU291M0vL3KHeNgMRHO3mvz1jAc,15
-xia_easy_proto-1.0.7.dist-info/RECORD,,
+xia_easy_proto-1.0.8.dist-info/LICENSE.txt,sha256=VI2DRhUdOX7ADnFkyNfO3YiExtoLHTFKKd8XFlFAbWw,151
+xia_easy_proto-1.0.8.dist-info/METADATA,sha256=PsIWguFk-pY1rVRpHg1pknu6Kit2fEU-6HC-kFXs7HM,418
+xia_easy_proto-1.0.8.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_easy_proto-1.0.8.dist-info/top_level.txt,sha256=KPFU7QdTuBBTOvgTGU291M0vL3KHeNgMRHO3mvz1jAc,15
+xia_easy_proto-1.0.8.dist-info/RECORD,,
```

