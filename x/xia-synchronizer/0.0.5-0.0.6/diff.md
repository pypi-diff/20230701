# Comparing `tmp/xia_synchronizer-0.0.5-cp39-none-win_amd64.whl.zip` & `tmp/xia_synchronizer-0.0.6-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2620 bytes, number of entries: 7
--rw-r--r--  2.0 unx      111 b- defN 23-Jun-30 11:44 xia_synchronizer/__init__.py
--rw-r--r--  2.0 unx     1924 b- defN 23-Jun-30 09:52 xia_synchronizer/synchronizer.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:45 xia_synchronizer-0.0.5.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      475 b- defN 23-Jun-30 11:45 xia_synchronizer-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:45 xia_synchronizer-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Jun-30 11:45 xia_synchronizer-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      606 b- defN 23-Jun-30 11:45 xia_synchronizer-0.0.5.dist-info/RECORD
-7 files, 3383 bytes uncompressed, 1530 bytes compressed:  54.8%
+Zip file size: 2621 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      111 b- defN 23-Jul-01 17:42 xia_synchronizer/__init__.py
+-rw-r--r--  2.0 unx     1924 b- defN 23-Jun-29 19:41 xia_synchronizer/synchronizer.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jul-01 17:42 xia_synchronizer-0.0.6.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      475 b- defN 23-Jul-01 17:42 xia_synchronizer-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 17:42 xia_synchronizer-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jul-01 17:42 xia_synchronizer-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      606 b- defN 23-Jul-01 17:42 xia_synchronizer-0.0.6.dist-info/RECORD
+7 files, 3383 bytes uncompressed, 1531 bytes compressed:  54.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_synchronizer/__init__.py
 Comment: 
 
 Filename: xia_synchronizer/synchronizer.py
 Comment: 
 
-Filename: xia_synchronizer-0.0.5.dist-info/LICENSE.txt
+Filename: xia_synchronizer-0.0.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_synchronizer-0.0.5.dist-info/METADATA
+Filename: xia_synchronizer-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: xia_synchronizer-0.0.5.dist-info/WHEEL
+Filename: xia_synchronizer-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: xia_synchronizer-0.0.5.dist-info/top_level.txt
+Filename: xia_synchronizer-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_synchronizer-0.0.5.dist-info/RECORD
+Filename: xia_synchronizer-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_synchronizer/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_synchronizer.synchronizer import Synchronizer
 
 __all__ = [
     "Synchronizer"
 ]
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
```

## Comparing `xia_synchronizer-0.0.5.dist-info/RECORD` & `xia_synchronizer-0.0.6.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_synchronizer/__init__.py,sha256=YzC-Xhay2Tm142HkRSKqago3sbesc7zi2ULb9B9IyFI,111
+xia_synchronizer/__init__.py,sha256=aRS_9FpjvOzDKGyZrxRVIC0QMZvpWniG020U7Ja8OxY,111
 xia_synchronizer/synchronizer.py,sha256=q45rkKyE8JxESGPTy4iVbwqY9G8WPo36Uv-3tSgND4g,1924
-xia_synchronizer-0.0.5.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
-xia_synchronizer-0.0.5.dist-info/METADATA,sha256=MVx1XpzZW9X6bV5aCZ2yHJQaOI3KbZp_JELjiSBiDyg,475
-xia_synchronizer-0.0.5.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_synchronizer-0.0.5.dist-info/top_level.txt,sha256=EahQyqx1d2L_ftYTJKK2xMeqqBeLdlPQrJTCzXNxp9M,17
-xia_synchronizer-0.0.5.dist-info/RECORD,,
+xia_synchronizer-0.0.6.dist-info/LICENSE.txt,sha256=VI2DRhUdOX7ADnFkyNfO3YiExtoLHTFKKd8XFlFAbWw,151
+xia_synchronizer-0.0.6.dist-info/METADATA,sha256=I5jah5QR7MqOUk6spvJhWIhQVyrp7cmDrwbxEiXfNNs,475
+xia_synchronizer-0.0.6.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_synchronizer-0.0.6.dist-info/top_level.txt,sha256=EahQyqx1d2L_ftYTJKK2xMeqqBeLdlPQrJTCzXNxp9M,17
+xia_synchronizer-0.0.6.dist-info/RECORD,,
```

