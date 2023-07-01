# Comparing `tmp/xia_git-0.1.4-cp39-none-win_amd64.whl.zip` & `tmp/xia_git-0.1.5-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3342 bytes, number of entries: 7
--rw-r--r--  2.0 unx       75 b- defN 23-Jun-30 11:28 xia_git/__init__.py
+Zip file size: 3344 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       75 b- defN 23-Jul-01 17:59 xia_git/__init__.py
 -rw-r--r--  2.0 unx     5437 b- defN 23-Jun-29 17:31 xia_git/git.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:31 xia_git-0.1.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      405 b- defN 23-Jun-30 11:31 xia_git-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:31 xia_git-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-30 11:31 xia_git-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      532 b- defN 23-Jun-30 11:31 xia_git-0.1.4.dist-info/RECORD
-7 files, 6707 bytes uncompressed, 2396 bytes compressed:  64.3%
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jul-01 18:03 xia_git-0.1.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      405 b- defN 23-Jul-01 18:03 xia_git-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 18:03 xia_git-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-01 18:03 xia_git-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      532 b- defN 23-Jul-01 18:03 xia_git-0.1.5.dist-info/RECORD
+7 files, 6707 bytes uncompressed, 2398 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_git/__init__.py
 Comment: 
 
 Filename: xia_git/git.py
 Comment: 
 
-Filename: xia_git-0.1.4.dist-info/LICENSE.txt
+Filename: xia_git-0.1.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_git-0.1.4.dist-info/METADATA
+Filename: xia_git-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: xia_git-0.1.4.dist-info/WHEEL
+Filename: xia_git-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: xia_git-0.1.4.dist-info/top_level.txt
+Filename: xia_git-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_git-0.1.4.dist-info/RECORD
+Filename: xia_git-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_git/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_git.git import Git
 
 __all__ = [
     "Git"
 ]
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
```

## Comparing `xia_git-0.1.4.dist-info/RECORD` & `xia_git-0.1.5.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_git/__init__.py,sha256=wBIM_1ciIqd4ZdnjeH4NcYnFIAvtiNNktbR-EP8wCOw,75
+xia_git/__init__.py,sha256=5MrkqKC4qjFaLvY8lJQ5Fhu02ye3Vy3b9fyQa5TIj60,75
 xia_git/git.py,sha256=YE-PbwkALdjts50o4Jlmdbc_5cUpMla1J40JoqAbKUw,5437
-xia_git-0.1.4.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
-xia_git-0.1.4.dist-info/METADATA,sha256=dviINd5uNfk3BTTxC1SlPXwHn6ks4PZ9SxQD5d24yzI,405
-xia_git-0.1.4.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_git-0.1.4.dist-info/top_level.txt,sha256=ABnAcKKQ0PdOskOMU7mTZ4Tx475kcJ5AYKB9qZvg0IY,8
-xia_git-0.1.4.dist-info/RECORD,,
+xia_git-0.1.5.dist-info/LICENSE.txt,sha256=VI2DRhUdOX7ADnFkyNfO3YiExtoLHTFKKd8XFlFAbWw,151
+xia_git-0.1.5.dist-info/METADATA,sha256=k6dVDYjQbIzjL1yqyPp2AWDOtjZa9PYG5bUMp3jqzcw,405
+xia_git-0.1.5.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_git-0.1.5.dist-info/top_level.txt,sha256=ABnAcKKQ0PdOskOMU7mTZ4Tx475kcJ5AYKB9qZvg0IY,8
+xia_git-0.1.5.dist-info/RECORD,,
```

