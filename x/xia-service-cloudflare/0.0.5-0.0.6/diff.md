# Comparing `tmp/xia_service_cloudflare-0.0.5-cp39-none-win_amd64.whl.zip` & `tmp/xia_service_cloudflare-0.0.6-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3793 bytes, number of entries: 8
--rw-r--r--  2.0 unx      293 b- defN 23-Jun-30 11:37 xia_service_cloudflare/__init__.py
--rw-r--r--  2.0 unx     5892 b- defN 23-Jun-30 11:37 xia_service_cloudflare/engine.py
--rw-r--r--  2.0 unx      131 b- defN 23-Jun-30 11:37 xia_service_cloudflare/service.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:41 xia_service_cloudflare-0.0.5.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      461 b- defN 23-Jun-30 11:41 xia_service_cloudflare-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:41 xia_service_cloudflare-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       23 b- defN 23-Jun-30 11:41 xia_service_cloudflare-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      731 b- defN 23-Jun-30 11:41 xia_service_cloudflare-0.0.5.dist-info/RECORD
-8 files, 7781 bytes uncompressed, 2489 bytes compressed:  68.0%
+Zip file size: 3804 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      293 b- defN 23-Jul-01 18:09 xia_service_cloudflare/__init__.py
+-rw-r--r--  2.0 unx     5892 b- defN 23-Jun-29 20:59 xia_service_cloudflare/engine.py
+-rw-r--r--  2.0 unx      131 b- defN 23-Jun-29 20:59 xia_service_cloudflare/service.py
+-rw-r--r--  2.0 unx      151 b- defN 23-Jul-01 18:09 xia_service_cloudflare-0.0.6.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      461 b- defN 23-Jul-01 18:09 xia_service_cloudflare-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jul-01 18:09 xia_service_cloudflare-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       23 b- defN 23-Jul-01 18:09 xia_service_cloudflare-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      732 b- defN 23-Jul-01 18:09 xia_service_cloudflare-0.0.6.dist-info/RECORD
+8 files, 7791 bytes uncompressed, 2500 bytes compressed:  67.9%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: xia_service_cloudflare/engine.py
 Comment: 
 
 Filename: xia_service_cloudflare/service.py
 Comment: 
 
-Filename: xia_service_cloudflare-0.0.5.dist-info/LICENSE.txt
+Filename: xia_service_cloudflare-0.0.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_service_cloudflare-0.0.5.dist-info/METADATA
+Filename: xia_service_cloudflare-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: xia_service_cloudflare-0.0.5.dist-info/WHEEL
+Filename: xia_service_cloudflare-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: xia_service_cloudflare-0.0.5.dist-info/top_level.txt
+Filename: xia_service_cloudflare-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_service_cloudflare-0.0.5.dist-info/RECORD
+Filename: xia_service_cloudflare-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_service_cloudflare/__init__.py

```diff
@@ -4,8 +4,8 @@
 
 __all__ = [
     "CfServiceAdmEngine", "CfServiceAdmParam", "CfServiceAdmClient",
     "CloudflareService"
 ]
 
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
```

## Comparing `xia_service_cloudflare-0.0.5.dist-info/RECORD` & `xia_service_cloudflare-0.0.6.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-xia_service_cloudflare/__init__.py,sha256=9-8nTKl7hRHRQ2V5GLLA6HUdOYd5xKlKWKTOjjKel5A,293
+xia_service_cloudflare/__init__.py,sha256=ao8G8McG2cK2budYq5yxF4JuM_PlgCGvLwjM6kL_66Q,293
 xia_service_cloudflare/engine.py,sha256=eDu973kWrdIjdEHfX1tX_qzJg5PntHCVIhw49_9fLAI,5892
 xia_service_cloudflare/service.py,sha256=H0MHhO_VBf1mxkPjjE9w10KHXGOwf6NZzgZ4ejG4FOo,131
-xia_service_cloudflare-0.0.5.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
-xia_service_cloudflare-0.0.5.dist-info/METADATA,sha256=KxBwq9cmhmfR9Eqn-i96Dvl1ppwpha4ZNKTuSuSdy0A,461
-xia_service_cloudflare-0.0.5.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_service_cloudflare-0.0.5.dist-info/top_level.txt,sha256=MFS9cmitDr8e_hFma0-hfOG0KSm_f_B0DAwzJzmhtTQ,23
-xia_service_cloudflare-0.0.5.dist-info/RECORD,,
+xia_service_cloudflare-0.0.6.dist-info/LICENSE.txt,sha256=VI2DRhUdOX7ADnFkyNfO3YiExtoLHTFKKd8XFlFAbWw,151
+xia_service_cloudflare-0.0.6.dist-info/METADATA,sha256=WItg35gNF6Dk13S5Ud-yfReeCEP7eXDhyx7yI6wS4bM,461
+xia_service_cloudflare-0.0.6.dist-info/WHEEL,sha256=NsapCMY7EanMRKZsZABtoiyq2rs4aXJ4FKsV_kV91NE,108
+xia_service_cloudflare-0.0.6.dist-info/top_level.txt,sha256=MFS9cmitDr8e_hFma0-hfOG0KSm_f_B0DAwzJzmhtTQ,23
+xia_service_cloudflare-0.0.6.dist-info/RECORD,,
```

