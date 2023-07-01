# Comparing `tmp/xia_compiler_openapi-0.1.21-cp39-none-win_amd64.whl.zip` & `tmp/xia_compiler_openapi-0.1.22-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 8935 bytes, number of entries: 7
--rw-r--r--  2.0 unx      127 b- defN 23-Jun-30 12:33 xia_compiler_openapi/__init__.py
+-rw-r--r--  2.0 unx      126 b- defN 23-Jul-01 17:52 xia_compiler_openapi/__init__.py
 -rw-r--r--  2.0 unx    38568 b- defN 23-Jun-30 12:33 xia_compiler_openapi/compiler.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 12:33 xia_compiler_openapi-0.1.21.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      431 b- defN 23-Jun-30 12:33 xia_compiler_openapi-0.1.21.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 12:33 xia_compiler_openapi-0.1.21.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-Jun-30 12:33 xia_compiler_openapi-0.1.21.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      636 b- defN 23-Jun-30 12:33 xia_compiler_openapi-0.1.21.dist-info/RECORD
-7 files, 40033 bytes uncompressed, 7787 bytes compressed:  80.5%
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jul-01 17:52 xia_compiler_openapi-0.1.22.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      431 b- defN 23-Jul-01 17:52 xia_compiler_openapi-0.1.22.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 17:52 xia_compiler_openapi-0.1.22.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-Jul-01 17:52 xia_compiler_openapi-0.1.22.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      636 b- defN 23-Jul-01 17:52 xia_compiler_openapi-0.1.22.dist-info/RECORD
+7 files, 40032 bytes uncompressed, 7787 bytes compressed:  80.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_compiler_openapi/__init__.py
 Comment: 
 
 Filename: xia_compiler_openapi/compiler.py
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.21.dist-info/LICENSE.txt
+Filename: xia_compiler_openapi-0.1.22.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.21.dist-info/METADATA
+Filename: xia_compiler_openapi-0.1.22.dist-info/METADATA
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.21.dist-info/WHEEL
+Filename: xia_compiler_openapi-0.1.22.dist-info/WHEEL
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.21.dist-info/top_level.txt
+Filename: xia_compiler_openapi-0.1.22.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.21.dist-info/RECORD
+Filename: xia_compiler_openapi-0.1.22.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_compiler_openapi/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_compiler_openapi.compiler import XiaCompilerOpenapi
 
 
 __all__ = [
     "XiaCompilerOpenapi",
 ]
 
-__version__ = "0.1.21"
+__version__ = "0.1.22"
```

## Comparing `xia_compiler_openapi-0.1.21.dist-info/RECORD` & `xia_compiler_openapi-0.1.22.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_compiler_openapi/__init__.py,sha256=dTO9Kdfh0OPW5WX-flTzvu8VevAlgFhQv6Zc3NiA7jg,127
+xia_compiler_openapi/__init__.py,sha256=UoPthSfp5a2jTcy9ELADSesBIVshiChNtqRcmtuPkEA,126
 xia_compiler_openapi/compiler.py,sha256=KSJMToOJVlv7XDxhqLQwPHFoooFVGtM_P4XfE-yUZpk,38568
-xia_compiler_openapi-0.1.21.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
-xia_compiler_openapi-0.1.21.dist-info/METADATA,sha256=0HSCGosofSRpBWyCixuNGgO41lLhJRk6zJhYW3xWxyM,431
-xia_compiler_openapi-0.1.21.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_compiler_openapi-0.1.21.dist-info/top_level.txt,sha256=l-dHwHri9HVBghJIDfyblbK8E8exERfi3dhMi7vW3bE,21
-xia_compiler_openapi-0.1.21.dist-info/RECORD,,
+xia_compiler_openapi-0.1.22.dist-info/LICENSE.txt,sha256=VI2DRhUdOX7ADnFkyNfO3YiExtoLHTFKKd8XFlFAbWw,151
+xia_compiler_openapi-0.1.22.dist-info/METADATA,sha256=cF46w0wnquAV-jZ75odXBP6uLSO9l0MFp17qDr6oCKk,431
+xia_compiler_openapi-0.1.22.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_compiler_openapi-0.1.22.dist-info/top_level.txt,sha256=l-dHwHri9HVBghJIDfyblbK8E8exERfi3dhMi7vW3bE,21
+xia_compiler_openapi-0.1.22.dist-info/RECORD,,
```

