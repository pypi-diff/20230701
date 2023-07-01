# Comparing `tmp/xia_agent_flask-0.0.8-cp39-none-win_amd64.whl.zip` & `tmp/xia_agent_flask-0.0.9-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2660 bytes, number of entries: 7
--rw-r--r--  2.0 unx      251 b- defN 23-Jun-30 11:13 xia_agent_flask/__init__.py
--rw-r--r--  2.0 unx     1888 b- defN 23-Jun-30 11:13 xia_agent_flask/api.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:17 xia_agent_flask-0.0.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      520 b- defN 23-Jun-30 11:17 xia_agent_flask-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:17 xia_agent_flask-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-30 11:17 xia_agent_flask-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      590 b- defN 23-Jun-30 11:17 xia_agent_flask-0.0.8.dist-info/RECORD
-7 files, 3515 bytes uncompressed, 1602 bytes compressed:  54.4%
+Zip file size: 2659 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      251 b- defN 23-Jul-01 17:44 xia_agent_flask/__init__.py
+-rw-r--r--  2.0 unx     1888 b- defN 23-Jun-29 20:32 xia_agent_flask/api.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jul-01 17:45 xia_agent_flask-0.0.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      520 b- defN 23-Jul-01 17:45 xia_agent_flask-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-01 17:45 xia_agent_flask-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-01 17:45 xia_agent_flask-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      590 b- defN 23-Jul-01 17:45 xia_agent_flask-0.0.9.dist-info/RECORD
+7 files, 3515 bytes uncompressed, 1601 bytes compressed:  54.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_agent_flask/__init__.py
 Comment: 
 
 Filename: xia_agent_flask/api.py
 Comment: 
 
-Filename: xia_agent_flask-0.0.8.dist-info/LICENSE.txt
+Filename: xia_agent_flask-0.0.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_agent_flask-0.0.8.dist-info/METADATA
+Filename: xia_agent_flask-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: xia_agent_flask-0.0.8.dist-info/WHEEL
+Filename: xia_agent_flask-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: xia_agent_flask-0.0.8.dist-info/top_level.txt
+Filename: xia_agent_flask-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_agent_flask-0.0.8.dist-info/RECORD
+Filename: xia_agent_flask-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_agent_flask/__init__.py

```diff
@@ -3,8 +3,8 @@
 
 
 __all__ = [
    "AgentFunctionApi",
    "FlaskRequestParser", "GcpLogParser", "PubsubLogParser"
 ]
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
```

## Comparing `xia_agent_flask-0.0.8.dist-info/METADATA` & `xia_agent_flask-0.0.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-agent-flask
-Version: 0.0.8
+Version: 0.0.9
 Summary: UNKNOWN
-Home-page: https://develop.x-i-a.com/docs/xia-agent-flask/0.0.8/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-agent-flask/0.0.9/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

