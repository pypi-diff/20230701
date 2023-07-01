# Comparing `tmp/cloudflared-1.0.0.1.tar.gz` & `tmp/cloudflared-1.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudflared-1.0.0.1.tar", last modified: Sat Jul  1 13:31:18 2023, max compression
+gzip compressed data, was "cloudflared-1.0.0.2.tar", last modified: Sat Jul  1 13:34:56 2023, max compression
```

## Comparing `cloudflared-1.0.0.1.tar` & `cloudflared-1.0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 13:31:18.538086 cloudflared-1.0.0.1/
--rw-rw-rw-   0        0        0      577 2023-07-01 13:31:18.538086 cloudflared-1.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      101 2023-06-30 14:52:56.000000 cloudflared-1.0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 13:31:18.522443 cloudflared-1.0.0.1/cloudflared/
--rw-rw-rw-   0        0        0       36 2023-07-01 13:29:26.000000 cloudflared-1.0.0.1/cloudflared/__init__.py
--rw-rw-rw-   0        0        0     1332 2023-07-01 13:01:38.000000 cloudflared-1.0.0.1/cloudflared/cloudflare.py
--rw-rw-rw-   0        0        0     2164 2023-06-30 11:11:53.000000 cloudflared-1.0.0.1/cloudflared/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-01 13:31:18.538086 cloudflared-1.0.0.1/cloudflared.egg-info/
--rw-rw-rw-   0        0        0      577 2023-07-01 13:31:18.000000 cloudflared-1.0.0.1/cloudflared.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-07-01 13:31:18.000000 cloudflared-1.0.0.1/cloudflared.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 13:31:18.000000 cloudflared-1.0.0.1/cloudflared.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-01 13:31:18.000000 cloudflared-1.0.0.1/cloudflared.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-01 13:31:18.000000 cloudflared-1.0.0.1/cloudflared.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 13:31:18.538086 cloudflared-1.0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      913 2023-07-01 13:30:45.000000 cloudflared-1.0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 13:34:56.254220 cloudflared-1.0.0.2/
+-rw-rw-rw-   0        0        0      577 2023-07-01 13:34:56.254220 cloudflared-1.0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      101 2023-06-30 14:52:56.000000 cloudflared-1.0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 13:34:56.238568 cloudflared-1.0.0.2/cloudflared/
+-rw-rw-rw-   0        0        0       36 2023-07-01 13:29:26.000000 cloudflared-1.0.0.2/cloudflared/__init__.py
+-rw-rw-rw-   0        0        0     1333 2023-07-01 13:34:22.000000 cloudflared-1.0.0.2/cloudflared/cloudflare.py
+-rw-rw-rw-   0        0        0     2164 2023-06-30 11:11:53.000000 cloudflared-1.0.0.2/cloudflared/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-01 13:34:56.254220 cloudflared-1.0.0.2/cloudflared.egg-info/
+-rw-rw-rw-   0        0        0      577 2023-07-01 13:34:56.000000 cloudflared-1.0.0.2/cloudflared.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-07-01 13:34:56.000000 cloudflared-1.0.0.2/cloudflared.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 13:34:56.000000 cloudflared-1.0.0.2/cloudflared.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-01 13:34:56.000000 cloudflared-1.0.0.2/cloudflared.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-01 13:34:56.000000 cloudflared-1.0.0.2/cloudflared.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 13:34:56.254220 cloudflared-1.0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      913 2023-07-01 13:34:28.000000 cloudflared-1.0.0.2/setup.py
```

### Comparing `cloudflared-1.0.0.1/PKG-INFO` & `cloudflared-1.0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudflared
-Version: 1.0.0.1
+Version: 1.0.0.2
 Summary: A Python package to interact with cloudflared
 Home-page: https://github.com/SigireddyBalaSai/cloudflared.py
 Author: Sigireddy BalaSai
 Author-email: sigireddybalasai@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cloudflared-1.0.0.1/cloudflared/cloudflare.py` & `cloudflared-1.0.0.2/cloudflared/cloudflare.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from utils import check_all
+from .utils import check_all
 import subprocess
 
 
 class CloudflareTunnels:
     tunnels = {}
 
     def __init__(self):
```

### Comparing `cloudflared-1.0.0.1/cloudflared/utils.py` & `cloudflared-1.0.0.2/cloudflared/utils.py`

 * *Files identical despite different names*

### Comparing `cloudflared-1.0.0.1/cloudflared.egg-info/PKG-INFO` & `cloudflared-1.0.0.2/cloudflared.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudflared
-Version: 1.0.0.1
+Version: 1.0.0.2
 Summary: A Python package to interact with cloudflared
 Home-page: https://github.com/SigireddyBalaSai/cloudflared.py
 Author: Sigireddy BalaSai
 Author-email: sigireddybalasai@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cloudflared-1.0.0.1/setup.py` & `cloudflared-1.0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     with open("README.md", encoding='utf-8') as file:
         file_data = file.read()
     return file_data
 
 
 setup(
     name="cloudflared",
-    version="1.0.0.1",
+    version="1.0.0.2",
     description="A Python package to interact with cloudflared",
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/SigireddyBalaSai/cloudflared.py",
     author="Sigireddy BalaSai",
     author_email="sigireddybalasai@gmail.com",
     license="Apache-2.0",
```

