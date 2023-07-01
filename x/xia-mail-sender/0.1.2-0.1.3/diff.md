# Comparing `tmp/xia_mail_sender-0.1.2-cp39-none-win_amd64.whl.zip` & `tmp/xia_mail_sender-0.1.3-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2511 bytes, number of entries: 7
--rw-r--r--  2.0 unx      100 b- defN 23-Jun-30 11:33 xia_mail_sender/__init__.py
--rw-r--r--  2.0 unx     1333 b- defN 23-Jun-29 20:53 xia_mail_sender/sender.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:36 xia_mail_sender-0.1.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      420 b- defN 23-Jun-30 11:36 xia_mail_sender-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:36 xia_mail_sender-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-30 11:36 xia_mail_sender-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      593 b- defN 23-Jun-30 11:36 xia_mail_sender-0.1.2.dist-info/RECORD
-7 files, 2712 bytes uncompressed, 1447 bytes compressed:  46.6%
+Zip file size: 2513 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      100 b- defN 23-Jul-01 18:04 xia_mail_sender/__init__.py
+-rw-r--r--  2.0 unx     1333 b- defN 23-Jul-01 18:04 xia_mail_sender/sender.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jul-01 18:08 xia_mail_sender-0.1.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      420 b- defN 23-Jul-01 18:08 xia_mail_sender-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 18:08 xia_mail_sender-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-01 18:08 xia_mail_sender-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      593 b- defN 23-Jul-01 18:08 xia_mail_sender-0.1.3.dist-info/RECORD
+7 files, 2712 bytes uncompressed, 1449 bytes compressed:  46.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_mail_sender/__init__.py
 Comment: 
 
 Filename: xia_mail_sender/sender.py
 Comment: 
 
-Filename: xia_mail_sender-0.1.2.dist-info/LICENSE.txt
+Filename: xia_mail_sender-0.1.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_mail_sender-0.1.2.dist-info/METADATA
+Filename: xia_mail_sender-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: xia_mail_sender-0.1.2.dist-info/WHEEL
+Filename: xia_mail_sender-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: xia_mail_sender-0.1.2.dist-info/top_level.txt
+Filename: xia_mail_sender-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_mail_sender-0.1.2.dist-info/RECORD
+Filename: xia_mail_sender-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_mail_sender/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_mail_sender.sender import MailSender
 
 __all__ = [
     "MailSender"
 ]
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

