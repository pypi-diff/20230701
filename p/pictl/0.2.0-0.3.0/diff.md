# Comparing `tmp/pictl-0.2.0.tar.gz` & `tmp/pictl-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pictl-0.2.0.tar", max compression
+gzip compressed data, was "pictl-0.3.0.tar", max compression
```

## Comparing `pictl-0.2.0.tar` & `pictl-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1069 2023-06-27 06:25:56.664657 pictl-0.2.0/LICENSE
--rw-r--r--   0        0        0     3651 2023-06-27 06:25:56.664657 pictl-0.2.0/README.md
--rw-r--r--   0        0        0      375 2023-06-27 06:25:56.664657 pictl-0.2.0/pictl/__init__.py
--rw-r--r--   0        0        0       77 2023-06-27 06:25:56.664657 pictl-0.2.0/pictl/cli/__init__.py
--rw-r--r--   0        0        0     2979 2023-06-27 06:25:56.664657 pictl-0.2.0/pictl/cli/main.py
--rw-r--r--   0        0        0      133 2023-06-27 06:25:56.664657 pictl-0.2.0/pictl/config/__init__.py
--rw-r--r--   0        0        0     4308 2023-06-27 06:25:56.664657 pictl-0.2.0/pictl/config/config.py
--rw-r--r--   0        0        0     1400 2023-06-27 06:25:56.664657 pictl-0.2.0/pictl/config/regions.py
--rw-r--r--   0        0        0       90 2023-06-27 06:25:56.664657 pictl-0.2.0/pictl/pic/__init__.py
--rw-r--r--   0        0        0      973 2023-06-27 06:25:56.664657 pictl-0.2.0/pictl/pic/pic.py
--rw-r--r--   0        0        0      128 2023-06-27 06:25:56.664657 pictl-0.2.0/pictl/upload/__init__.py
--rw-r--r--   0        0        0     1763 2023-06-27 06:25:56.664657 pictl-0.2.0/pictl/upload/upload.py
--rw-r--r--   0        0        0      271 2023-06-27 06:25:56.664657 pictl-0.2.0/pictl/utils/__init__.py
--rw-r--r--   0        0        0     1473 2023-06-27 06:25:56.664657 pictl-0.2.0/pictl/utils/utils.py
--rw-r--r--   0        0        0      558 2023-06-27 06:25:56.664657 pictl-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4350 1970-01-01 00:00:00.000000 pictl-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-01 07:49:54.762188 pictl-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3651 2023-07-01 07:49:54.762188 pictl-0.3.0/README.md
+-rw-r--r--   0        0        0      375 2023-07-01 07:49:54.762188 pictl-0.3.0/pictl/__init__.py
+-rw-r--r--   0        0        0       77 2023-07-01 07:49:54.762188 pictl-0.3.0/pictl/cli/__init__.py
+-rw-r--r--   0        0        0     2979 2023-07-01 07:49:54.762188 pictl-0.3.0/pictl/cli/main.py
+-rw-r--r--   0        0        0      133 2023-07-01 07:49:54.762188 pictl-0.3.0/pictl/config/__init__.py
+-rw-r--r--   0        0        0     5884 2023-07-01 07:49:54.762188 pictl-0.3.0/pictl/config/config.py
+-rw-r--r--   0        0        0     6109 2023-07-01 07:49:54.762188 pictl-0.3.0/pictl/config/regions.py
+-rw-r--r--   0        0        0       90 2023-07-01 07:49:54.762188 pictl-0.3.0/pictl/pic/__init__.py
+-rw-r--r--   0        0        0      973 2023-07-01 07:49:54.762188 pictl-0.3.0/pictl/pic/pic.py
+-rw-r--r--   0        0        0      128 2023-07-01 07:49:54.762188 pictl-0.3.0/pictl/upload/__init__.py
+-rw-r--r--   0        0        0     2003 2023-07-01 07:49:54.762188 pictl-0.3.0/pictl/upload/upload.py
+-rw-r--r--   0        0        0      271 2023-07-01 07:49:54.762188 pictl-0.3.0/pictl/utils/__init__.py
+-rw-r--r--   0        0        0     1473 2023-07-01 07:49:54.762188 pictl-0.3.0/pictl/utils/utils.py
+-rw-r--r--   0        0        0      558 2023-07-01 07:49:54.762188 pictl-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4350 1970-01-01 00:00:00.000000 pictl-0.3.0/PKG-INFO
```

### Comparing `pictl-0.2.0/LICENSE` & `pictl-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pictl-0.2.0/README.md` & `pictl-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pictl-0.2.0/pictl/cli/main.py` & `pictl-0.3.0/pictl/cli/main.py`

 * *Files identical despite different names*

### Comparing `pictl-0.2.0/pictl/pic/pic.py` & `pictl-0.3.0/pictl/pic/pic.py`

 * *Files identical despite different names*

### Comparing `pictl-0.2.0/pictl/upload/upload.py` & `pictl-0.3.0/pictl/upload/upload.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Upload module"""
 
 import boto3
+from botocore.config import Config as BConfig
 from rich import print as rprint
 
 from pictl.config import Config
 from pictl.utils import get_content_type, get_object_key
 
 
 def upload(filename: str, group: str) -> None:
@@ -28,14 +29,18 @@
 def upload_s3(settings: dict, filename: str, group: str):
     resource = {
         "endpoint_url": settings[group]["endpoint"],
         "aws_access_key_id": settings[group]["key"],
         "aws_secret_access_key": settings[group]["secret"],
         "region_name": settings[group]["region"],
     }
+    if settings[group]["type"] in ["OSS(Aliyun)", "DO", "OVH(High)"]:
+        resource["config"] = BConfig(
+            s3={"addressing_style": "virtual", "signature_version": "s3v4"}
+        )
     s3 = boto3.resource("s3", **resource)
     with open(filename, "rb") as data:
         content_type = get_content_type(filename)
         key = get_object_key(filename, settings[group]["prefix"])
         s3.Bucket(settings[group]["bucket"]).put_object(
             Key=key,
             Body=data,
```

### Comparing `pictl-0.2.0/pictl/utils/utils.py` & `pictl-0.3.0/pictl/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pictl-0.2.0/pyproject.toml` & `pictl-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pictl"
-version = "0.2.0"
+version = "0.3.0"
 description = "A command line tool for image processing and uploading (ex. S3-type)"
 authors = ["zhonger <zhonger@live.cn>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `pictl-0.2.0/PKG-INFO` & `pictl-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pictl
-Version: 0.2.0
+Version: 0.3.0
 Summary: A command line tool for image processing and uploading (ex. S3-type)
 License: MIT
 Author: zhonger
 Author-email: zhonger@live.cn
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

