# Comparing `tmp/xia_engine_terraform_gcs-0.1.3-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_terraform_gcs-0.1.4-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3521 bytes, number of entries: 7
--rw-r--r--  2.0 unx      377 b- defN 23-Jun-30 11:24 xia_engine_terraform_gcs/__init__.py
--rw-r--r--  2.0 unx     4325 b- defN 23-Jun-30 11:24 xia_engine_terraform_gcs/engine.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:29 xia_engine_terraform_gcs-0.1.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      508 b- defN 23-Jun-30 11:29 xia_engine_terraform_gcs-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:29 xia_engine_terraform_gcs-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       25 b- defN 23-Jun-30 11:29 xia_engine_terraform_gcs-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      656 b- defN 23-Jun-30 11:29 xia_engine_terraform_gcs-0.1.3.dist-info/RECORD
-7 files, 6141 bytes uncompressed, 2331 bytes compressed:  62.0%
+Zip file size: 3525 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      377 b- defN 23-Jul-01 17:58 xia_engine_terraform_gcs/__init__.py
+-rw-r--r--  2.0 unx     4325 b- defN 23-Jun-30 11:27 xia_engine_terraform_gcs/engine.py
+-rw-r--r--  2.0 unx      151 b- defN 23-Jul-01 17:58 xia_engine_terraform_gcs-0.1.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      508 b- defN 23-Jul-01 17:58 xia_engine_terraform_gcs-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jul-01 17:58 xia_engine_terraform_gcs-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       25 b- defN 23-Jul-01 17:58 xia_engine_terraform_gcs-0.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      657 b- defN 23-Jul-01 17:58 xia_engine_terraform_gcs-0.1.4.dist-info/RECORD
+7 files, 6151 bytes uncompressed, 2335 bytes compressed:  62.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_terraform_gcs/__init__.py
 Comment: 
 
 Filename: xia_engine_terraform_gcs/engine.py
 Comment: 
 
-Filename: xia_engine_terraform_gcs-0.1.3.dist-info/LICENSE.txt
+Filename: xia_engine_terraform_gcs-0.1.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_terraform_gcs-0.1.3.dist-info/METADATA
+Filename: xia_engine_terraform_gcs-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_terraform_gcs-0.1.3.dist-info/WHEEL
+Filename: xia_engine_terraform_gcs-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_terraform_gcs-0.1.3.dist-info/top_level.txt
+Filename: xia_engine_terraform_gcs-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_terraform_gcs-0.1.3.dist-info/RECORD
+Filename: xia_engine_terraform_gcs-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_terraform_gcs/__init__.py

```diff
@@ -3,8 +3,8 @@
 
 
 __all__ = [
     "TerraformGcsEngine", "TerraformGcsConnectParam", "TerraformGcsClient",
     "ScwTerraformGcsEngine", "ScwTerraformGcsConnectParam"
 ]
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
```

## Comparing `xia_engine_terraform_gcs-0.1.3.dist-info/RECORD` & `xia_engine_terraform_gcs-0.1.4.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_engine_terraform_gcs/__init__.py,sha256=SzpeKzxbg0T5O3junslP5xJ6fkojZe6s_6UfSK3vtGE,377
+xia_engine_terraform_gcs/__init__.py,sha256=A49JfHiJcOgoKuxEz0-zX3-Iq8g3FgB_PLZWeiuk1O0,377
 xia_engine_terraform_gcs/engine.py,sha256=0lVS5HwriZsOyZL71cBzenlMXdOxERQrneMX6dQus6k,4325
-xia_engine_terraform_gcs-0.1.3.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
-xia_engine_terraform_gcs-0.1.3.dist-info/METADATA,sha256=oTWf2AZXIQCGZsGB0YCy3E4KpnrVwAWY9QKvsJmFX10,508
-xia_engine_terraform_gcs-0.1.3.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_engine_terraform_gcs-0.1.3.dist-info/top_level.txt,sha256=iRljnR7jo0lVXDe6suGjsY4FzFzjk-Xas_iLcd7D2EU,25
-xia_engine_terraform_gcs-0.1.3.dist-info/RECORD,,
+xia_engine_terraform_gcs-0.1.4.dist-info/LICENSE.txt,sha256=VI2DRhUdOX7ADnFkyNfO3YiExtoLHTFKKd8XFlFAbWw,151
+xia_engine_terraform_gcs-0.1.4.dist-info/METADATA,sha256=eJUzqTMMyMeZ-746PF852rp-lkTzBWlM_idihXneACg,508
+xia_engine_terraform_gcs-0.1.4.dist-info/WHEEL,sha256=NsapCMY7EanMRKZsZABtoiyq2rs4aXJ4FKsV_kV91NE,108
+xia_engine_terraform_gcs-0.1.4.dist-info/top_level.txt,sha256=iRljnR7jo0lVXDe6suGjsY4FzFzjk-Xas_iLcd7D2EU,25
+xia_engine_terraform_gcs-0.1.4.dist-info/RECORD,,
```

