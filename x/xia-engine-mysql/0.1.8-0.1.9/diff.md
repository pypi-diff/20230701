# Comparing `tmp/xia_engine_mysql-0.1.8-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_mysql-0.1.9-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4148 bytes, number of entries: 7
--rw-r--r--  2.0 unx      143 b- defN 23-Jun-29 20:44 xia_engine_mysql/__init__.py
--rw-r--r--  2.0 unx     6756 b- defN 23-Jun-29 20:07 xia_engine_mysql/engine.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:46 xia_engine_mysql-0.1.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      715 b- defN 23-Jun-29 20:46 xia_engine_mysql-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:46 xia_engine_mysql-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Jun-29 20:46 xia_engine_mysql-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      600 b- defN 23-Jun-29 20:46 xia_engine_mysql-0.1.8.dist-info/RECORD
-7 files, 8481 bytes uncompressed, 3070 bytes compressed:  63.8%
+Zip file size: 4066 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      143 b- defN 23-Jun-30 11:25 xia_engine_mysql/__init__.py
+-rw-r--r--  2.0 unx     6756 b- defN 23-Jun-30 11:25 xia_engine_mysql/engine.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:26 xia_engine_mysql-0.1.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      477 b- defN 23-Jun-30 11:26 xia_engine_mysql-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:26 xia_engine_mysql-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-30 11:26 xia_engine_mysql-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      600 b- defN 23-Jun-30 11:26 xia_engine_mysql-0.1.9.dist-info/RECORD
+7 files, 8243 bytes uncompressed, 2988 bytes compressed:  63.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_mysql/__init__.py
 Comment: 
 
 Filename: xia_engine_mysql/engine.py
 Comment: 
 
-Filename: xia_engine_mysql-0.1.8.dist-info/LICENSE.txt
+Filename: xia_engine_mysql-0.1.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_mysql-0.1.8.dist-info/METADATA
+Filename: xia_engine_mysql-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_mysql-0.1.8.dist-info/WHEEL
+Filename: xia_engine_mysql-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_mysql-0.1.8.dist-info/top_level.txt
+Filename: xia_engine_mysql-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_mysql-0.1.8.dist-info/RECORD
+Filename: xia_engine_mysql-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_mysql/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_engine_mysql.engine import MysqlEngine, MysqlConnectParam
 
 __all__ = [
     "MysqlEngine", "MysqlConnectParam"
 ]
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
```

## Comparing `xia_engine_mysql-0.1.8.dist-info/RECORD` & `xia_engine_mysql-0.1.9.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_engine_mysql/__init__.py,sha256=8rJrBhjKcUCZl8h5AwOrNIVmnEMR41mPfAGS3eHmxxM,143
+xia_engine_mysql/__init__.py,sha256=-unIljGyoAg30gaHhX4NN1Wwj2TKq6OY7kafY_Qn-lE,143
 xia_engine_mysql/engine.py,sha256=1_jvr33SshZkABOXgrBSzyv_6BzWurg7zMNkMGFYWOA,6756
-xia_engine_mysql-0.1.8.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
-xia_engine_mysql-0.1.8.dist-info/METADATA,sha256=-QCOivmbrur9ICmeoUu4peWQVlAHYQCMT-1CiDHxZYs,715
-xia_engine_mysql-0.1.8.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_engine_mysql-0.1.8.dist-info/top_level.txt,sha256=iEabOz01n8HLyWdyjMLZMYHeuLxpVhBNWV3Rh6M4n1c,17
-xia_engine_mysql-0.1.8.dist-info/RECORD,,
+xia_engine_mysql-0.1.9.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
+xia_engine_mysql-0.1.9.dist-info/METADATA,sha256=RPDPOORoFVdcYX-BoZTZcly0_VUwcvxBFlp9QViiKi0,477
+xia_engine_mysql-0.1.9.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_engine_mysql-0.1.9.dist-info/top_level.txt,sha256=iEabOz01n8HLyWdyjMLZMYHeuLxpVhBNWV3Rh6M4n1c,17
+xia_engine_mysql-0.1.9.dist-info/RECORD,,
```

