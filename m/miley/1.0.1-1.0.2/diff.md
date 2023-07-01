# Comparing `tmp/miley-1.0.1.tar.gz` & `tmp/miley-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miley-1.0.1.tar", max compression
+gzip compressed data, was "miley-1.0.2.tar", max compression
```

## Comparing `miley-1.0.1.tar` & `miley-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-06-25 18:10:39.386980 miley-1.0.1/LICENSE
--rw-r--r--   0        0        0     1338 2023-07-01 15:13:08.751431 miley-1.0.1/README.md
--rw-r--r--   0        0        0        0 2023-06-25 18:10:53.134902 miley-1.0.1/miley/__init__.py
--rw-r--r--   0        0        0     2089 2023-07-01 14:55:34.152892 miley-1.0.1/miley/client.py
--rw-r--r--   0        0        0     1512 2023-07-01 14:19:58.928927 miley-1.0.1/miley/container_handler.py
--rw-r--r--   0        0        0      297 2023-06-27 21:32:52.536940 miley-1.0.1/miley/dir_walker.py
--rw-r--r--   0        0        0      443 2023-06-27 22:12:28.466808 miley-1.0.1/miley/hasher.py
--rwxr-xr-x   0        0        0     1743 2023-07-01 15:18:54.178132 miley-1.0.1/miley/main.py
--rw-r--r--   0        0        0      409 2023-07-01 15:19:41.650025 miley-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1817 1970-01-01 00:00:00.000000 miley-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-25 18:10:39.386980 miley-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1338 2023-07-01 15:13:08.751431 miley-1.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-25 18:10:53.134902 miley-1.0.2/miley/__init__.py
+-rw-r--r--   0        0        0     2129 2023-07-01 15:21:31.057824 miley-1.0.2/miley/client.py
+-rw-r--r--   0        0        0     1554 2023-07-01 15:21:38.105813 miley-1.0.2/miley/container_handler.py
+-rw-r--r--   0        0        0      338 2023-07-01 15:21:46.157801 miley-1.0.2/miley/dir_walker.py
+-rw-r--r--   0        0        0      484 2023-07-01 15:21:52.421792 miley-1.0.2/miley/hasher.py
+-rwxr-xr-x   0        0        0     1408 2023-07-01 15:21:22.689837 miley-1.0.2/miley/main.py
+-rw-r--r--   0        0        0      409 2023-07-01 15:22:09.493767 miley-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1817 1970-01-01 00:00:00.000000 miley-1.0.2/PKG-INFO
```

### Comparing `miley-1.0.1/LICENSE` & `miley-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `miley-1.0.1/README.md` & `miley-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `miley-1.0.1/miley/client.py` & `miley-1.0.2/miley/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import requests
 
 md5_length = 32
 sha1_length = 40
 sha256_length = 64
 
+logging.basicConfig(level=logging.INFO)
 
 class Client:
     def __init__(self):
         self.url = "https://mb-api.abuse.ch/api/v1/"
         self.malware_found = False
         self.samples_scanned = 0
         # TODO: add virus total
```

### Comparing `miley-1.0.1/miley/container_handler.py` & `miley-1.0.2/miley/container_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import json
 import logging
 import os
 import tarfile
 import docker
 
+logging.basicConfig(level=logging.INFO)
+
 class Container:
     def __init__(self):
         self.docker_client = docker.from_env()
         self.image_name = ""
         self.downloaded_image = ""
         self.export_path = "/tmp/image.tar"
         self.extracted_path = "/tmp/unpacked_image/"
@@ -38,8 +40,8 @@
                 if tarinfo.isdev():
                     continue
 
                 dest = os.path.join(self.extracted_path, tarinfo.name)
                 if not tarinfo.isdir() and os.path.exists(dest):
                     os.unlink(dest)
 
-                layer_tar.extract(tarinfo, path=self.extracted_path)
+                layer_tar.extract(tarinfo, path=self.extracted_path)
```

### Comparing `miley-1.0.1/miley/main.py` & `miley-1.0.2/miley/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -44,22 +44,11 @@
         return
 
     c = Client()
     c.query_hashes(hashes=hashes_to_scan)
 
 
 if __name__ == "__main__":
-    logging.basicConfig(level=logging.DEBUG)
+    logging.basicConfig(level=logging.INFO)
     main()
 
-"""
-scratch pad:
-Scan local directories / files:
-    ./miley --path /tmp/whatever/
-    ./miley --path /tmp/whatever/evil.exe
 
-Scan containers - should work if the container is in a remote registry or local:
-    ./miley --img alpine:latest
-
-Scan a file hash - meant for testing, but still useful:
-    ./miley --hash SHA256,SHA1,MD5
-"""
```

### Comparing `miley-1.0.1/PKG-INFO` & `miley-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miley
-Version: 1.0.1
+Version: 1.0.2
 Summary: TBD
 Author: bluesentinelsec
 Author-email: bluesentinel@protonmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

