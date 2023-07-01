# Comparing `tmp/venv_pack2-0.6.1-py3-none-any.whl.zip` & `tmp/venv_pack2-0.6.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 21643 bytes, number of entries: 15
+Zip file size: 21633 bytes, number of entries: 15
 -rw-rw-r--  2.0 unx      114 b- defN 23-May-25 01:09 venv_pack/__init__.py
 -rw-rw-r--  2.0 unx     5605 b- defN 23-May-25 01:09 venv_pack/__main__.py
--rw-rw-r--  2.0 unx    24901 b- defN 23-May-25 08:08 venv_pack/core.py
+-rw-rw-r--  2.0 unx    24930 b- defN 23-Jul-01 12:24 venv_pack/core.py
 -rw-rw-r--  2.0 unx     5070 b- defN 23-May-25 01:09 venv_pack/formats.py
 -rw-rw-r--  2.0 unx     2893 b- defN 23-May-25 01:09 venv_pack/progress.py
 -rw-rw-r--  2.0 unx     2681 b- defN 23-May-25 01:09 venv_pack/scripts/CPYTHON_LICENSE.txt
 -rw-rw-r--  2.0 unx     8990 b- defN 23-May-25 01:09 venv_pack/scripts/common/Activate.ps1
 -rw-rw-r--  2.0 unx     2766 b- defN 23-May-25 01:09 venv_pack/scripts/common/activate
 -rw-rw-r--  2.0 unx     1529 b- defN 23-May-25 01:09 venv_pack/scripts/nt/activate.bat
--rw-rw-r--  2.0 unx     1498 b- defN 23-May-25 08:12 venv_pack2-0.6.1.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     2596 b- defN 23-May-25 08:12 venv_pack2-0.6.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-25 08:12 venv_pack2-0.6.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       75 b- defN 23-May-25 08:12 venv_pack2-0.6.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       10 b- defN 23-May-25 08:12 venv_pack2-0.6.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1256 b- defN 23-May-25 08:12 venv_pack2-0.6.1.dist-info/RECORD
-15 files, 60076 bytes uncompressed, 19559 bytes compressed:  67.4%
+-rw-rw-r--  2.0 unx     1498 b- defN 23-Jul-01 12:31 venv_pack2-0.6.2.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     2576 b- defN 23-Jul-01 12:31 venv_pack2-0.6.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-01 12:31 venv_pack2-0.6.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       54 b- defN 23-Jul-01 12:31 venv_pack2-0.6.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jul-01 12:31 venv_pack2-0.6.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1256 b- defN 23-Jul-01 12:31 venv_pack2-0.6.2.dist-info/RECORD
+15 files, 60064 bytes uncompressed, 19549 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -21,26 +21,26 @@
 
 Filename: venv_pack/scripts/common/activate
 Comment: 
 
 Filename: venv_pack/scripts/nt/activate.bat
 Comment: 
 
-Filename: venv_pack2-0.6.1.dist-info/LICENSE.txt
+Filename: venv_pack2-0.6.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: venv_pack2-0.6.1.dist-info/METADATA
+Filename: venv_pack2-0.6.2.dist-info/METADATA
 Comment: 
 
-Filename: venv_pack2-0.6.1.dist-info/WHEEL
+Filename: venv_pack2-0.6.2.dist-info/WHEEL
 Comment: 
 
-Filename: venv_pack2-0.6.1.dist-info/entry_points.txt
+Filename: venv_pack2-0.6.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: venv_pack2-0.6.1.dist-info/top_level.txt
+Filename: venv_pack2-0.6.2.dist-info/top_level.txt
 Comment: 
 
-Filename: venv_pack2-0.6.1.dist-info/RECORD
+Filename: venv_pack2-0.6.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## venv_pack/core.py

```diff
@@ -598,15 +598,15 @@
 
         shebang, executable, options = shebang_match.groups()
 
         if executable.startswith(prefix_b):
             # shebang points inside environment, rewrite
             new_shebang = (b'#!%s'
                            if on_win else
-                           b'#!/bin/sh\n"exec" "`dirname $(readlink -f $0)`/%s" "$0" "$@"\n')\
+                           b'#!/bin/sh\n"exec" "`dirname $( /usr/bin/readlink -f $0 || readlink -f $0 )`/%s" "$0" "$@"\n')\
                           % os.path.basename(executable)
             data = data.replace(shebang, new_shebang)
 
         return data, True, target
 
     return data, False, target
```

## Comparing `venv_pack2-0.6.1.dist-info/LICENSE.txt` & `venv_pack2-0.6.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `venv_pack2-0.6.1.dist-info/METADATA` & `venv_pack2-0.6.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: venv-pack2
-Version: 0.6.1
+Version: 0.6.2
 Summary: Package virtual environments for redistribution
 Home-page: https://github.com/mrmathematica/venv-pack
 Maintainer: mrmathematica
 Maintainer-email: mrmathematica@yahoo.com
 License: BSD
 Project-URL: Source Code, https://github.com/mrmathematica/venv-pack
 Keywords: venv packaging
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Software Distribution
 Classifier: Topic :: Software Development :: Build Tools
 Description-Content-Type: text/markdown
@@ -83,9 +82,7 @@
 Unpack environment into directory `my_env`
 ```
 md my_env
 python -m zipfile -e venv.zip my_env\ 
 ```
 
 All features of venv should keep working from my_env folder. 
-
-
```

## Comparing `venv_pack2-0.6.1.dist-info/RECORD` & `venv_pack2-0.6.2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 venv_pack/__init__.py,sha256=aBYgEdvPK8d8yQWwcHcLLUGCL_uUDRQRvYXdgZ-c3aY,114
 venv_pack/__main__.py,sha256=L_Yp84RYhsOl2Q-_CCeZe6IVisQO67WFL1DE_mEiUNA,5605
-venv_pack/core.py,sha256=lYi5PmELJsec9SIcKbhfLfLQNAmMBNIUez0KAwM6mQU,24901
+venv_pack/core.py,sha256=PZXanhVpwvqDih7SSASN8VZOUlpPm-2SP7W9KRypfiE,24930
 venv_pack/formats.py,sha256=cC380QlLVzonLQ5ycqLa7XLpjXNHnO0H14P0aCmkWAg,5070
 venv_pack/progress.py,sha256=amSS1NfqXDvTI9czLR8fcrgsUUQfNwkUz2h8FfhlcrY,2893
 venv_pack/scripts/CPYTHON_LICENSE.txt,sha256=MfcsvSFae8Doi2k1HNK-eA4ehM4feYBgj8oXbdbeMVg,2681
 venv_pack/scripts/common/Activate.ps1,sha256=oo4_TLfQ1yrK6kjjoT59PC8NWRQljfTWS3DVBZMZRs4,8990
 venv_pack/scripts/common/activate,sha256=Eq5j_QUW59ue-g_F7_nCJb9QaemVArExDLKzo2x-j3o,2766
 venv_pack/scripts/nt/activate.bat,sha256=MuKCJeLMN_g9GfaGMCJaVz7TVsCnTcyYpaoy6fyrOAE,1529
-venv_pack2-0.6.1.dist-info/LICENSE.txt,sha256=1c6xVheX4OZP3iTOwSXgk4MWqRWn6hNq3SauwqTFm6Y,1498
-venv_pack2-0.6.1.dist-info/METADATA,sha256=vWhOPQdBQns1Fnda11pjsumqKuQEIThApp9dZoUbl-E,2596
-venv_pack2-0.6.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-venv_pack2-0.6.1.dist-info/entry_points.txt,sha256=Ufh-YTREHMDYwNx_g32AGRfrleYSnJBp7VdqwUpjMKQ,75
-venv_pack2-0.6.1.dist-info/top_level.txt,sha256=qd1qiBpbP-8h-S5OlHAVLUK-d_UdmcKXm6bB4lSgM-c,10
-venv_pack2-0.6.1.dist-info/RECORD,,
+venv_pack2-0.6.2.dist-info/LICENSE.txt,sha256=1c6xVheX4OZP3iTOwSXgk4MWqRWn6hNq3SauwqTFm6Y,1498
+venv_pack2-0.6.2.dist-info/METADATA,sha256=GWM7ATiwZvPkycq_IAXkMRdB54LfM5eLNne3ajMElHY,2576
+venv_pack2-0.6.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+venv_pack2-0.6.2.dist-info/entry_points.txt,sha256=k0W2KHiJ6IJ2Yg8OaNfNLI9Mgsj-7j7Iahw85q35ooI,54
+venv_pack2-0.6.2.dist-info/top_level.txt,sha256=qd1qiBpbP-8h-S5OlHAVLUK-d_UdmcKXm6bB4lSgM-c,10
+venv_pack2-0.6.2.dist-info/RECORD,,
```

