# Comparing `tmp/xia_mail-0.1.2-cp39-none-win_amd64.whl.zip` & `tmp/xia_mail-0.1.3-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 2844 bytes, number of entries: 7
--rw-r--r--  2.0 unx      138 b- defN 23-Jun-30 11:32 xia_mail/__init__.py
--rw-r--r--  2.0 unx     2683 b- defN 23-Jun-29 20:12 xia_mail/mail.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:36 xia_mail-0.1.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      434 b- defN 23-Jun-30 11:36 xia_mail-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:36 xia_mail-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-30 11:36 xia_mail-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      541 b- defN 23-Jun-30 11:36 xia_mail-0.1.2.dist-info/RECORD
+-rw-r--r--  2.0 unx      138 b- defN 23-Jul-01 18:15 xia_mail/__init__.py
+-rw-r--r--  2.0 unx     2683 b- defN 23-Jul-01 18:15 xia_mail/mail.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jul-01 18:17 xia_mail-0.1.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      434 b- defN 23-Jul-01 18:17 xia_mail-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 18:17 xia_mail-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-01 18:17 xia_mail-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      541 b- defN 23-Jul-01 18:17 xia_mail-0.1.3.dist-info/RECORD
 7 files, 4055 bytes uncompressed, 1882 bytes compressed:  53.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_mail/__init__.py
 Comment: 
 
 Filename: xia_mail/mail.py
 Comment: 
 
-Filename: xia_mail-0.1.2.dist-info/LICENSE.txt
+Filename: xia_mail-0.1.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_mail-0.1.2.dist-info/METADATA
+Filename: xia_mail-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: xia_mail-0.1.2.dist-info/WHEEL
+Filename: xia_mail-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: xia_mail-0.1.2.dist-info/top_level.txt
+Filename: xia_mail-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_mail-0.1.2.dist-info/RECORD
+Filename: xia_mail-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_mail/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_mail.mail import MailField, MailAttachment, Mail
 
 
 __all__ = [
     "MailField", "MailAttachment", "Mail"
 ]
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

## Comparing `xia_mail-0.1.2.dist-info/RECORD` & `xia_mail-0.1.3.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_mail/__init__.py,sha256=wVTGBFcqOPwcVopsQ2lQe-CvTAELUICpSAAVa0uVAYE,138
+xia_mail/__init__.py,sha256=nuVFz6s8ePm345ZeyYUSuU0jXKo39jrcwSy-j0xwrcg,138
 xia_mail/mail.py,sha256=QKrwlWQednpKUTKiV0atoFTJRN3dtvrcNj9KBYDw0qc,2683
-xia_mail-0.1.2.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
-xia_mail-0.1.2.dist-info/METADATA,sha256=zPLxVETYEEu0Cw-e974ZRRC7u_jfmjFtqOrazUTXurM,434
-xia_mail-0.1.2.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_mail-0.1.2.dist-info/top_level.txt,sha256=q_fa-0_Tng_khWSC5LtvPYkIL4WOMwctdIklSmEm8GI,9
-xia_mail-0.1.2.dist-info/RECORD,,
+xia_mail-0.1.3.dist-info/LICENSE.txt,sha256=VI2DRhUdOX7ADnFkyNfO3YiExtoLHTFKKd8XFlFAbWw,151
+xia_mail-0.1.3.dist-info/METADATA,sha256=E9rzHYbvLT24qSoBLsnxnUl_3I54QEa8dFuZRzW2ifw,434
+xia_mail-0.1.3.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_mail-0.1.3.dist-info/top_level.txt,sha256=q_fa-0_Tng_khWSC5LtvPYkIL4WOMwctdIklSmEm8GI,9
+xia_mail-0.1.3.dist-info/RECORD,,
```

