# Comparing `tmp/xia_engine_terraform-0.1.18-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_terraform-0.1.19-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7570 bytes, number of entries: 7
--rw-r--r--  2.0 unx      645 b- defN 23-Jun-30 11:24 xia_engine_terraform/__init__.py
--rw-r--r--  2.0 unx    28900 b- defN 23-Jun-30 11:24 xia_engine_terraform/engine.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:28 xia_engine_terraform-0.1.18.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      480 b- defN 23-Jun-30 11:28 xia_engine_terraform-0.1.18.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:28 xia_engine_terraform-0.1.18.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-Jun-30 11:28 xia_engine_terraform-0.1.18.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      634 b- defN 23-Jun-30 11:28 xia_engine_terraform-0.1.18.dist-info/RECORD
-7 files, 30930 bytes uncompressed, 6426 bytes compressed:  79.2%
+Zip file size: 7569 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      645 b- defN 23-Jul-01 18:01 xia_engine_terraform/__init__.py
+-rw-r--r--  2.0 unx    28900 b- defN 23-Jul-01 18:01 xia_engine_terraform/engine.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jul-01 18:01 xia_engine_terraform-0.1.19.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      480 b- defN 23-Jul-01 18:01 xia_engine_terraform-0.1.19.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 18:01 xia_engine_terraform-0.1.19.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-Jul-01 18:01 xia_engine_terraform-0.1.19.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      634 b- defN 23-Jul-01 18:01 xia_engine_terraform-0.1.19.dist-info/RECORD
+7 files, 30930 bytes uncompressed, 6425 bytes compressed:  79.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_terraform/__init__.py
 Comment: 
 
 Filename: xia_engine_terraform/engine.py
 Comment: 
 
-Filename: xia_engine_terraform-0.1.18.dist-info/LICENSE.txt
+Filename: xia_engine_terraform-0.1.19.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_terraform-0.1.18.dist-info/METADATA
+Filename: xia_engine_terraform-0.1.19.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_terraform-0.1.18.dist-info/WHEEL
+Filename: xia_engine_terraform-0.1.19.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_terraform-0.1.18.dist-info/top_level.txt
+Filename: xia_engine_terraform-0.1.19.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_terraform-0.1.18.dist-info/RECORD
+Filename: xia_engine_terraform-0.1.19.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_terraform/__init__.py

```diff
@@ -6,8 +6,8 @@
 __all__ = [
     "TerraformEngine", "TerraformConnectParam", "TerraformClient",
     "TerraformLocalEngine", "TerraformLocalConnectParam", "TerraformLocalClient",
     "ScwTerraformLocalEngine", "ScwTerraformLocalConnectParam",
     "TerraformConfigFactory"
 ]
 
-__version__ = "0.1.18"
+__version__ = "0.1.19"
```

## Comparing `xia_engine_terraform-0.1.18.dist-info/RECORD` & `xia_engine_terraform-0.1.19.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_engine_terraform/__init__.py,sha256=INDnCYWKmoU5OxpVDOrHzaQ6O7OaPZSO8bgAwEv8Hz0,645
+xia_engine_terraform/__init__.py,sha256=WuKMWkEULpO9p2RcjUu1bDcP57-NAxd3PjXhsgCvn0E,645
 xia_engine_terraform/engine.py,sha256=_t4Xbj18HeoKX2369qDMO_9P_qy_PYqdeceEGLCLqo4,28900
-xia_engine_terraform-0.1.18.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
-xia_engine_terraform-0.1.18.dist-info/METADATA,sha256=dWSSuYy_cQ_QWUxmUpnS6jgySQEZsIDiVJKlNDfoX4U,480
-xia_engine_terraform-0.1.18.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_engine_terraform-0.1.18.dist-info/top_level.txt,sha256=9T86e-QQo91fnAOB3rD5xeM_4EPL7Edk_oOlmR_xquQ,21
-xia_engine_terraform-0.1.18.dist-info/RECORD,,
+xia_engine_terraform-0.1.19.dist-info/LICENSE.txt,sha256=VI2DRhUdOX7ADnFkyNfO3YiExtoLHTFKKd8XFlFAbWw,151
+xia_engine_terraform-0.1.19.dist-info/METADATA,sha256=xUeWgQZFLEl_wuTH2kZ3XUQT79JpzDbXxMzpsxJmsZE,480
+xia_engine_terraform-0.1.19.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_engine_terraform-0.1.19.dist-info/top_level.txt,sha256=9T86e-QQo91fnAOB3rD5xeM_4EPL7Edk_oOlmR_xquQ,21
+xia_engine_terraform-0.1.19.dist-info/RECORD,,
```

