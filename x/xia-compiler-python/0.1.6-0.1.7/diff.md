# Comparing `tmp/xia_compiler_python-0.1.6-cp39-none-win_amd64.whl.zip` & `tmp/xia_compiler_python-0.1.7-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5120 bytes, number of entries: 7
--rw-r--r--  2.0 unx      115 b- defN 23-Jun-30 11:20 xia_compiler_python/__init__.py
--rw-r--r--  2.0 unx    14558 b- defN 23-Jun-30 11:20 xia_compiler_python/compiler.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:23 xia_compiler_python-0.1.6.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      430 b- defN 23-Jun-30 11:23 xia_compiler_python-0.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:23 xia_compiler_python-0.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Jun-30 11:23 xia_compiler_python-0.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      624 b- defN 23-Jun-30 11:23 xia_compiler_python-0.1.6.dist-info/RECORD
-7 files, 15997 bytes uncompressed, 3996 bytes compressed:  75.0%
+Zip file size: 5130 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      115 b- defN 23-Jul-01 18:13 xia_compiler_python/__init__.py
+-rw-r--r--  2.0 unx    14558 b- defN 23-Jul-01 18:13 xia_compiler_python/compiler.py
+-rw-r--r--  2.0 unx      151 b- defN 23-Jul-01 18:13 xia_compiler_python-0.1.7.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      430 b- defN 23-Jul-01 18:13 xia_compiler_python-0.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jul-01 18:13 xia_compiler_python-0.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Jul-01 18:13 xia_compiler_python-0.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      625 b- defN 23-Jul-01 18:13 xia_compiler_python-0.1.7.dist-info/RECORD
+7 files, 16007 bytes uncompressed, 4006 bytes compressed:  75.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_compiler_python/__init__.py
 Comment: 
 
 Filename: xia_compiler_python/compiler.py
 Comment: 
 
-Filename: xia_compiler_python-0.1.6.dist-info/LICENSE.txt
+Filename: xia_compiler_python-0.1.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_compiler_python-0.1.6.dist-info/METADATA
+Filename: xia_compiler_python-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: xia_compiler_python-0.1.6.dist-info/WHEEL
+Filename: xia_compiler_python-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: xia_compiler_python-0.1.6.dist-info/top_level.txt
+Filename: xia_compiler_python-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_compiler_python-0.1.6.dist-info/RECORD
+Filename: xia_compiler_python-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_compiler_python/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_compiler_python.compiler import PythonCompiler
 
 
 __all__ = [
     "PythonCompiler"
 ]
 
-__version__ = "0.1.6"
+__version__ = "0.1.7"
```

## Comparing `xia_compiler_python-0.1.6.dist-info/RECORD` & `xia_compiler_python-0.1.7.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_compiler_python/__init__.py,sha256=6t9XTmEtxVab7ErkAaGNSLcD7ZJMAwXh-Gkua6otIxA,115
+xia_compiler_python/__init__.py,sha256=i98ynSnymyR0W542NvWvV3iWffsf-OqnV_vSKY-R470,115
 xia_compiler_python/compiler.py,sha256=0Uy-qOcFUIkKtZ8I_umtl1m1S_X-yzM9MwmP0O_SMUI,14558
-xia_compiler_python-0.1.6.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
-xia_compiler_python-0.1.6.dist-info/METADATA,sha256=pXiAjdvKeDiQ_7hEI-OyLbN-0sghhPxwfrQUMTa5UGI,430
-xia_compiler_python-0.1.6.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_compiler_python-0.1.6.dist-info/top_level.txt,sha256=R07z9GUYJwDzaFPJq6hLs3IP0HWGFMzYXFe9Dx7Lh-c,20
-xia_compiler_python-0.1.6.dist-info/RECORD,,
+xia_compiler_python-0.1.7.dist-info/LICENSE.txt,sha256=VI2DRhUdOX7ADnFkyNfO3YiExtoLHTFKKd8XFlFAbWw,151
+xia_compiler_python-0.1.7.dist-info/METADATA,sha256=pBXnVsuiw-du_EPz1Adbo9WajIs-f0QvZJc5prrVtl4,430
+xia_compiler_python-0.1.7.dist-info/WHEEL,sha256=NsapCMY7EanMRKZsZABtoiyq2rs4aXJ4FKsV_kV91NE,108
+xia_compiler_python-0.1.7.dist-info/top_level.txt,sha256=R07z9GUYJwDzaFPJq6hLs3IP0HWGFMzYXFe9Dx7Lh-c,20
+xia_compiler_python-0.1.7.dist-info/RECORD,,
```

