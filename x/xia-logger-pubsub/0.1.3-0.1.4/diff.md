# Comparing `tmp/xia_logger_pubsub-0.1.3-cp39-none-win_amd64.whl.zip` & `tmp/xia_logger_pubsub-0.1.4-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 3905 bytes, number of entries: 7
--rw-r--r--  2.0 unx      106 b- defN 23-Jun-30 11:32 xia_logger_pubsub/__init__.py
+-rw-r--r--  2.0 unx      106 b- defN 23-Jul-01 18:03 xia_logger_pubsub/__init__.py
 -rw-r--r--  2.0 unx     8477 b- defN 23-Jun-29 20:55 xia_logger_pubsub/logger.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:35 xia_logger_pubsub-0.1.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      461 b- defN 23-Jun-30 11:35 xia_logger_pubsub-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:35 xia_logger_pubsub-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Jun-30 11:35 xia_logger_pubsub-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      607 b- defN 23-Jun-30 11:35 xia_logger_pubsub-0.1.3.dist-info/RECORD
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jul-01 18:06 xia_logger_pubsub-0.1.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      461 b- defN 23-Jul-01 18:06 xia_logger_pubsub-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 18:06 xia_logger_pubsub-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-Jul-01 18:06 xia_logger_pubsub-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      607 b- defN 23-Jul-01 18:06 xia_logger_pubsub-0.1.4.dist-info/RECORD
 7 files, 9919 bytes uncompressed, 2813 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_logger_pubsub/__init__.py
 Comment: 
 
 Filename: xia_logger_pubsub/logger.py
 Comment: 
 
-Filename: xia_logger_pubsub-0.1.3.dist-info/LICENSE.txt
+Filename: xia_logger_pubsub-0.1.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_logger_pubsub-0.1.3.dist-info/METADATA
+Filename: xia_logger_pubsub-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: xia_logger_pubsub-0.1.3.dist-info/WHEEL
+Filename: xia_logger_pubsub-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: xia_logger_pubsub-0.1.3.dist-info/top_level.txt
+Filename: xia_logger_pubsub-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_logger_pubsub-0.1.3.dist-info/RECORD
+Filename: xia_logger_pubsub-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_logger_pubsub/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_logger_pubsub.logger import PubsubLogger
 
 __all__ = [
     "PubsubLogger"
 ]
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
```

## Comparing `xia_logger_pubsub-0.1.3.dist-info/RECORD` & `xia_logger_pubsub-0.1.4.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_logger_pubsub/__init__.py,sha256=Sr_8JjIKfgv3wBb_5Y6QxUgsCWNBhK3AxRfS4YH1fGw,106
+xia_logger_pubsub/__init__.py,sha256=rMT3Q0ca9PGgrBPdM0YiTtPesGHR_A-CsbztwgxsRXo,106
 xia_logger_pubsub/logger.py,sha256=J4gfKeVPWEmiUx5dcHH4lBYfFbHEM3CcW2crw5bvwhc,8477
-xia_logger_pubsub-0.1.3.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
-xia_logger_pubsub-0.1.3.dist-info/METADATA,sha256=A0gWcVMLkmwKkQzSKG8pzy3K0w-cpXbyt1ALzBgDEgc,461
-xia_logger_pubsub-0.1.3.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_logger_pubsub-0.1.3.dist-info/top_level.txt,sha256=Mqcsr6nvL5Sosyn07D9D1ckGO-vobonIclRaTN-5t3o,18
-xia_logger_pubsub-0.1.3.dist-info/RECORD,,
+xia_logger_pubsub-0.1.4.dist-info/LICENSE.txt,sha256=VI2DRhUdOX7ADnFkyNfO3YiExtoLHTFKKd8XFlFAbWw,151
+xia_logger_pubsub-0.1.4.dist-info/METADATA,sha256=DJ9C0AnDfcmmBCvFvQxp1WuBFLnx2zTaffdcKBMiN70,461
+xia_logger_pubsub-0.1.4.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_logger_pubsub-0.1.4.dist-info/top_level.txt,sha256=Mqcsr6nvL5Sosyn07D9D1ckGO-vobonIclRaTN-5t3o,18
+xia_logger_pubsub-0.1.4.dist-info/RECORD,,
```

