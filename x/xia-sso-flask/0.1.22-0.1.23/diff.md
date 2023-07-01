# Comparing `tmp/xia_sso_flask-0.1.22-cp39-none-win_amd64.whl.zip` & `tmp/xia_sso_flask-0.1.23-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 4122 bytes, number of entries: 7
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:40 xia_sso_flask/__init__.py
--rw-r--r--  2.0 unx     7568 b- defN 23-Jun-30 11:40 xia_sso_flask/sso.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:41 xia_sso_flask-0.1.22.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      501 b- defN 23-Jun-30 11:41 xia_sso_flask-0.1.22.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:41 xia_sso_flask-0.1.22.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Jun-30 11:41 xia_sso_flask-0.1.22.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      580 b- defN 23-Jun-30 11:41 xia_sso_flask-0.1.22.dist-info/RECORD
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 18:09 xia_sso_flask/__init__.py
+-rw-r--r--  2.0 unx     7568 b- defN 23-Jul-01 18:09 xia_sso_flask/sso.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jul-01 18:12 xia_sso_flask-0.1.23.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      501 b- defN 23-Jul-01 18:12 xia_sso_flask-0.1.23.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 18:12 xia_sso_flask-0.1.23.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Jul-01 18:12 xia_sso_flask-0.1.23.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      580 b- defN 23-Jul-01 18:12 xia_sso_flask-0.1.23.dist-info/RECORD
 7 files, 9012 bytes uncompressed, 3082 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_sso_flask/__init__.py
 Comment: 
 
 Filename: xia_sso_flask/sso.py
 Comment: 
 
-Filename: xia_sso_flask-0.1.22.dist-info/LICENSE.txt
+Filename: xia_sso_flask-0.1.23.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_sso_flask-0.1.22.dist-info/METADATA
+Filename: xia_sso_flask-0.1.23.dist-info/METADATA
 Comment: 
 
-Filename: xia_sso_flask-0.1.22.dist-info/WHEEL
+Filename: xia_sso_flask-0.1.23.dist-info/WHEEL
 Comment: 
 
-Filename: xia_sso_flask-0.1.22.dist-info/top_level.txt
+Filename: xia_sso_flask-0.1.23.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_sso_flask-0.1.22.dist-info/RECORD
+Filename: xia_sso_flask-0.1.23.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_sso_flask/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_sso_flask.sso import XiaSsoFlask
 
 __all__ = [
     "XiaSsoFlask",
 ]
 
-__version__ = "0.1.22"
+__version__ = "0.1.23"
```

## Comparing `xia_sso_flask-0.1.22.dist-info/RECORD` & `xia_sso_flask-0.1.23.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_sso_flask/__init__.py,sha256=5s6l6Cwbf1L5KdwqtO8C1ueMnulVvoog8TJth_yIstU,99
+xia_sso_flask/__init__.py,sha256=5IPOeonqEofVvTYwnbYxgyIVqgUGKP9huIM3z4D-3BM,99
 xia_sso_flask/sso.py,sha256=T_TvchEMI5A3W1CyheANYqH8oYgpn7AruPsz3GfwR-Q,7568
-xia_sso_flask-0.1.22.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
-xia_sso_flask-0.1.22.dist-info/METADATA,sha256=W4nmBrTfePYoDEIiaHCsT7PP8AoDNU7lR3r__FoTSp4,501
-xia_sso_flask-0.1.22.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_sso_flask-0.1.22.dist-info/top_level.txt,sha256=yYx7mFCVHYNw9aHXAf7T_8djYexDhG9AXQVA01XrSwY,14
-xia_sso_flask-0.1.22.dist-info/RECORD,,
+xia_sso_flask-0.1.23.dist-info/LICENSE.txt,sha256=VI2DRhUdOX7ADnFkyNfO3YiExtoLHTFKKd8XFlFAbWw,151
+xia_sso_flask-0.1.23.dist-info/METADATA,sha256=JllYskXAoVvnCq2ICNt9sQphViNRL_L84TWVnMTh5lk,501
+xia_sso_flask-0.1.23.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_sso_flask-0.1.23.dist-info/top_level.txt,sha256=yYx7mFCVHYNw9aHXAf7T_8djYexDhG9AXQVA01XrSwY,14
+xia_sso_flask-0.1.23.dist-info/RECORD,,
```

