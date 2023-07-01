# Comparing `tmp/xia_broadcast-0.1.3-cp39-none-win_amd64.whl.zip` & `tmp/xia_broadcast-0.1.4-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4157 bytes, number of entries: 7
--rw-r--r--  2.0 unx      131 b- defN 23-Jun-30 11:15 xia_broadcast/__init__.py
--rw-r--r--  2.0 unx     7587 b- defN 23-Jun-29 17:07 xia_broadcast/broadcast.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:18 xia_broadcast-0.1.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      442 b- defN 23-Jun-30 11:18 xia_broadcast-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:18 xia_broadcast-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Jun-30 11:18 xia_broadcast-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      582 b- defN 23-Jun-30 11:18 xia_broadcast-0.1.3.dist-info/RECORD
-7 files, 9006 bytes uncompressed, 3115 bytes compressed:  65.4%
+Zip file size: 4164 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      131 b- defN 23-Jul-01 17:48 xia_broadcast/__init__.py
+-rw-r--r--  2.0 unx     7587 b- defN 23-Jun-29 20:35 xia_broadcast/broadcast.py
+-rw-r--r--  2.0 unx      151 b- defN 23-Jul-01 17:48 xia_broadcast-0.1.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      442 b- defN 23-Jul-01 17:48 xia_broadcast-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jul-01 17:48 xia_broadcast-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Jul-01 17:48 xia_broadcast-0.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      583 b- defN 23-Jul-01 17:48 xia_broadcast-0.1.4.dist-info/RECORD
+7 files, 9016 bytes uncompressed, 3122 bytes compressed:  65.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_broadcast/__init__.py
 Comment: 
 
 Filename: xia_broadcast/broadcast.py
 Comment: 
 
-Filename: xia_broadcast-0.1.3.dist-info/LICENSE.txt
+Filename: xia_broadcast-0.1.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_broadcast-0.1.3.dist-info/METADATA
+Filename: xia_broadcast-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: xia_broadcast-0.1.3.dist-info/WHEEL
+Filename: xia_broadcast-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: xia_broadcast-0.1.3.dist-info/top_level.txt
+Filename: xia_broadcast-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_broadcast-0.1.3.dist-info/RECORD
+Filename: xia_broadcast-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_broadcast/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_broadcast.broadcast import AuthClient, Broadcaster
 
 
 __all__ = [
     "AuthClient", "Broadcaster",
 ]
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
```

## Comparing `xia_broadcast-0.1.3.dist-info/RECORD` & `xia_broadcast-0.1.4.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_broadcast/__init__.py,sha256=gCCh9WJCjR1McgNs_PQK_q2ivlGDYpN8_BkqzaX_j6M,131
+xia_broadcast/__init__.py,sha256=wxEFtaAPNHRzsF39kRzLUbxb90aY7jncidTdNnbiwUc,131
 xia_broadcast/broadcast.py,sha256=6f423ThasO3F0ff6KUqXwKgKCKhtOySfLtjLcaO2l4o,7587
-xia_broadcast-0.1.3.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
-xia_broadcast-0.1.3.dist-info/METADATA,sha256=0tqGZYmEMX16FhyotgdF2Sdq-JvSyMFUMZgxCoAn42E,442
-xia_broadcast-0.1.3.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_broadcast-0.1.3.dist-info/top_level.txt,sha256=BVEHXFDj1kIY7lo8v-H6KOU-bvTC9FQrjB2mSvZppd8,14
-xia_broadcast-0.1.3.dist-info/RECORD,,
+xia_broadcast-0.1.4.dist-info/LICENSE.txt,sha256=VI2DRhUdOX7ADnFkyNfO3YiExtoLHTFKKd8XFlFAbWw,151
+xia_broadcast-0.1.4.dist-info/METADATA,sha256=Qe_7iSFKVyyQ5hUNXBOWPW_lAiTu3NGuOyxnCDxtw9k,442
+xia_broadcast-0.1.4.dist-info/WHEEL,sha256=NsapCMY7EanMRKZsZABtoiyq2rs4aXJ4FKsV_kV91NE,108
+xia_broadcast-0.1.4.dist-info/top_level.txt,sha256=BVEHXFDj1kIY7lo8v-H6KOU-bvTC9FQrjB2mSvZppd8,14
+xia_broadcast-0.1.4.dist-info/RECORD,,
```

