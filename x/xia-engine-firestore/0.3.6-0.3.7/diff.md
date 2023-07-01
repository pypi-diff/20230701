# Comparing `tmp/xia_engine_firestore-0.3.6-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_firestore-0.3.7-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4191 bytes, number of entries: 7
--rw-r--r--  2.0 unx      116 b- defN 23-Jun-30 11:23 xia_engine_firestore/__init__.py
--rw-r--r--  2.0 unx     9905 b- defN 23-Jun-29 11:52 xia_engine_firestore/engine.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:27 xia_engine_firestore-0.3.6.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      470 b- defN 23-Jun-30 11:27 xia_engine_firestore-0.3.6.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:27 xia_engine_firestore-0.3.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-Jun-30 11:27 xia_engine_firestore-0.3.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      628 b- defN 23-Jun-30 11:27 xia_engine_firestore-0.3.6.dist-info/RECORD
-7 files, 11390 bytes uncompressed, 3057 bytes compressed:  73.2%
+Zip file size: 4192 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      116 b- defN 23-Jul-01 17:56 xia_engine_firestore/__init__.py
+-rw-r--r--  2.0 unx     9905 b- defN 23-Jul-01 17:56 xia_engine_firestore/engine.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jul-01 17:57 xia_engine_firestore-0.3.7.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      470 b- defN 23-Jul-01 17:57 xia_engine_firestore-0.3.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 17:57 xia_engine_firestore-0.3.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-Jul-01 17:57 xia_engine_firestore-0.3.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      628 b- defN 23-Jul-01 17:57 xia_engine_firestore-0.3.7.dist-info/RECORD
+7 files, 11390 bytes uncompressed, 3058 bytes compressed:  73.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_firestore/__init__.py
 Comment: 
 
 Filename: xia_engine_firestore/engine.py
 Comment: 
 
-Filename: xia_engine_firestore-0.3.6.dist-info/LICENSE.txt
+Filename: xia_engine_firestore-0.3.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_firestore-0.3.6.dist-info/METADATA
+Filename: xia_engine_firestore-0.3.7.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_firestore-0.3.6.dist-info/WHEEL
+Filename: xia_engine_firestore-0.3.7.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_firestore-0.3.6.dist-info/top_level.txt
+Filename: xia_engine_firestore-0.3.7.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_firestore-0.3.6.dist-info/RECORD
+Filename: xia_engine_firestore-0.3.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_firestore/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_engine_firestore.engine import FirestoreEngine
 
 
 __all__ = [
     "FirestoreEngine"
 ]
 
-__version__ = "0.3.6"
+__version__ = "0.3.7"
```

## Comparing `xia_engine_firestore-0.3.6.dist-info/RECORD` & `xia_engine_firestore-0.3.7.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_engine_firestore/__init__.py,sha256=gz1DPX24TIafPoIRmy0Nsprq48aBq5fZD4u8ZQzdqkc,116
+xia_engine_firestore/__init__.py,sha256=0IuDat5WTRbu5SqMSozAvP95eCQUXeTo2l2NBjSb7JE,116
 xia_engine_firestore/engine.py,sha256=BewFLUI81p_T4SXsj3IAYa3LGCrtpNa9nviBaWj5fzI,9905
-xia_engine_firestore-0.3.6.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
-xia_engine_firestore-0.3.6.dist-info/METADATA,sha256=y7ZST8zplchgtKMAVkxQqf328zcYRKTnWUj6mtRzwtM,470
-xia_engine_firestore-0.3.6.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_engine_firestore-0.3.6.dist-info/top_level.txt,sha256=NUY0_anDQ8KVQ1TnPs_SCf-78KqRmu8_ARIL_J5agrg,21
-xia_engine_firestore-0.3.6.dist-info/RECORD,,
+xia_engine_firestore-0.3.7.dist-info/LICENSE.txt,sha256=VI2DRhUdOX7ADnFkyNfO3YiExtoLHTFKKd8XFlFAbWw,151
+xia_engine_firestore-0.3.7.dist-info/METADATA,sha256=qyvxwktLuW7PI88ZHqHJYTOKcfP72CO0KKMVwoqPYvw,470
+xia_engine_firestore-0.3.7.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_engine_firestore-0.3.7.dist-info/top_level.txt,sha256=NUY0_anDQ8KVQ1TnPs_SCf-78KqRmu8_ARIL_J5agrg,21
+xia_engine_firestore-0.3.7.dist-info/RECORD,,
```

