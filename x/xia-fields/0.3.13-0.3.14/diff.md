# Comparing `tmp/xia_fields-0.3.13-cp39-none-win_amd64.whl.zip` & `tmp/xia_fields-0.3.14-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 10280 bytes, number of entries: 9
--rw-r--r--  2.0 unx     1177 b- defN 23-Jun-30 11:24 xia_fields/__init__.py
--rw-r--r--  2.0 unx    13346 b- defN 23-Jun-30 10:30 xia_fields/base.py
--rw-r--r--  2.0 unx    13317 b- defN 23-Jun-30 10:30 xia_fields/fields.py
--rw-r--r--  2.0 unx     9575 b- defN 23-Jun-30 10:30 xia_fields/fields_ext.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:29 xia_fields-0.3.13.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      388 b- defN 23-Jun-30 11:29 xia_fields-0.3.13.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:29 xia_fields-0.3.13.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-30 11:29 xia_fields-0.3.13.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      722 b- defN 23-Jun-30 11:29 xia_fields-0.3.13.dist-info/RECORD
-9 files, 38786 bytes uncompressed, 9040 bytes compressed:  76.7%
+Zip file size: 10281 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     1177 b- defN 23-Jul-01 18:13 xia_fields/__init__.py
+-rw-r--r--  2.0 unx    13346 b- defN 23-Jul-01 14:26 xia_fields/base.py
+-rw-r--r--  2.0 unx    13317 b- defN 23-Jul-01 14:26 xia_fields/fields.py
+-rw-r--r--  2.0 unx     9575 b- defN 23-Jul-01 14:26 xia_fields/fields_ext.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jul-01 18:17 xia_fields-0.3.14.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      388 b- defN 23-Jul-01 18:17 xia_fields-0.3.14.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 18:17 xia_fields-0.3.14.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-01 18:17 xia_fields-0.3.14.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      722 b- defN 23-Jul-01 18:17 xia_fields-0.3.14.dist-info/RECORD
+9 files, 38786 bytes uncompressed, 9041 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: xia_fields/fields.py
 Comment: 
 
 Filename: xia_fields/fields_ext.py
 Comment: 
 
-Filename: xia_fields-0.3.13.dist-info/LICENSE.txt
+Filename: xia_fields-0.3.14.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_fields-0.3.13.dist-info/METADATA
+Filename: xia_fields-0.3.14.dist-info/METADATA
 Comment: 
 
-Filename: xia_fields-0.3.13.dist-info/WHEEL
+Filename: xia_fields-0.3.14.dist-info/WHEEL
 Comment: 
 
-Filename: xia_fields-0.3.13.dist-info/top_level.txt
+Filename: xia_fields-0.3.14.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_fields-0.3.13.dist-info/RECORD
+Filename: xia_fields-0.3.14.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_fields/__init__.py

```diff
@@ -14,8 +14,8 @@
     "JsonField", "DictField", "CompressedStringField",
     "Int64Field", "Int32Field", "SFixed64Field", "SFixed32Field",
     "UInt64Field", "UInt32Field", "Fixed64Field", "Fixed32Field",
     "DoubleField", "DateField", "TimestampField", "TimeField", "DateTimeField",
     "OsEnvironField"
 ]
 
-__version__ = "0.3.13"
+__version__ = "0.3.14"
```

