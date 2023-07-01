# Comparing `tmp/xia_gpt_openai-0.1.4-cp39-none-win_amd64.whl.zip` & `tmp/xia_gpt_openai-0.1.5-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2696 bytes, number of entries: 7
--rw-r--r--  2.0 unx      121 b- defN 23-Jul-01 16:13 xia_gpt_openai/__init__.py
--rw-r--r--  2.0 unx     1753 b- defN 23-Jul-01 16:13 xia_gpt_openai/gpt.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jul-01 16:15 xia_gpt_openai-0.1.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      439 b- defN 23-Jul-01 16:15 xia_gpt_openai-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 16:15 xia_gpt_openai-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jul-01 16:15 xia_gpt_openai-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      583 b- defN 23-Jul-01 16:15 xia_gpt_openai-0.1.4.dist-info/RECORD
-7 files, 3161 bytes uncompressed, 1652 bytes compressed:  47.7%
+Zip file size: 2702 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      120 b- defN 23-Jul-01 18:02 xia_gpt_openai/__init__.py
+-rw-r--r--  2.0 unx     1753 b- defN 23-Jul-01 16:14 xia_gpt_openai/gpt.py
+-rw-r--r--  2.0 unx      151 b- defN 23-Jul-01 18:02 xia_gpt_openai-0.1.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      439 b- defN 23-Jul-01 18:02 xia_gpt_openai-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jul-01 18:02 xia_gpt_openai-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jul-01 18:02 xia_gpt_openai-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      584 b- defN 23-Jul-01 18:02 xia_gpt_openai-0.1.5.dist-info/RECORD
+7 files, 3170 bytes uncompressed, 1658 bytes compressed:  47.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_gpt_openai/__init__.py
 Comment: 
 
 Filename: xia_gpt_openai/gpt.py
 Comment: 
 
-Filename: xia_gpt_openai-0.1.4.dist-info/LICENSE.txt
+Filename: xia_gpt_openai-0.1.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_gpt_openai-0.1.4.dist-info/METADATA
+Filename: xia_gpt_openai-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: xia_gpt_openai-0.1.4.dist-info/WHEEL
+Filename: xia_gpt_openai-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: xia_gpt_openai-0.1.4.dist-info/top_level.txt
+Filename: xia_gpt_openai-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_gpt_openai-0.1.4.dist-info/RECORD
+Filename: xia_gpt_openai-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_gpt_openai/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_gpt_openai.gpt import OpenaiGpt, OpenaiGpt4
 
 __all__ = [
     "OpenaiGpt", "OpenaiGpt4"
 ]
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
```

