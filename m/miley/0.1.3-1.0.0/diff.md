# Comparing `tmp/miley-0.1.3.tar.gz` & `tmp/miley-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miley-0.1.3.tar", max compression
+gzip compressed data, was "miley-1.0.0.tar", max compression
```

## Comparing `miley-0.1.3.tar` & `miley-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-06-25 18:10:39.386980 miley-0.1.3/LICENSE
--rw-r--r--   0        0        0       12 2023-06-25 18:10:39.386980 miley-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-06-25 18:10:53.134902 miley-0.1.3/miley/__init__.py
--rw-r--r--   0        0        0     1843 2023-06-25 21:43:45.094117 miley-0.1.3/miley/client.py
--rwxr-xr-x   0        0        0     1526 2023-06-25 21:40:35.841891 miley-0.1.3/miley/main.py
--rw-r--r--   0        0        0      391 2023-06-25 21:45:11.778267 miley-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      452 1970-01-01 00:00:00.000000 miley-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-25 18:10:39.386980 miley-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1338 2023-07-01 15:13:08.751431 miley-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-25 18:10:53.134902 miley-1.0.0/miley/__init__.py
+-rw-r--r--   0        0        0     2089 2023-07-01 14:55:34.152892 miley-1.0.0/miley/client.py
+-rw-r--r--   0        0        0     1512 2023-07-01 14:19:58.928927 miley-1.0.0/miley/container_handler.py
+-rw-r--r--   0        0        0      297 2023-06-27 21:32:52.536940 miley-1.0.0/miley/dir_walker.py
+-rw-r--r--   0        0        0      443 2023-06-27 22:12:28.466808 miley-1.0.0/miley/hasher.py
+-rwxr-xr-x   0        0        0     1742 2023-07-01 14:21:09.233589 miley-1.0.0/miley/main.py
+-rw-r--r--   0        0        0      409 2023-07-01 15:13:43.391249 miley-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1817 1970-01-01 00:00:00.000000 miley-1.0.0/PKG-INFO
```

### Comparing `miley-0.1.3/LICENSE` & `miley-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `miley-0.1.3/miley/client.py` & `miley-1.0.0/miley/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import json
 import logging
+import time
 
 import requests
 
 md5_length = 32
 sha1_length = 40
 sha256_length = 64
 
@@ -14,38 +16,46 @@
         self.samples_scanned = 0
         # TODO: add virus total
 
     def query_hashes(self, hashes=None):
         if not self.is_valid_hash(hashes):
             return
 
-        logging.info("querying hashes against malware database")
+        num_hashes_to_scan = len(hashes)
         for each_hash in hashes:
             if each_hash == "":
                 continue
 
+            logging.info(f"querying {self.samples_scanned} / {num_hashes_to_scan} hashes against malware database")
+
             data = {"query": "get_info", "hash": each_hash}
-            response = requests.post(self.url, data=data)
-            j = response.json()
+            try:
+                response = requests.post(self.url, data=data)
+                j = response.json()
+            except Exception as e:
+                logging.error(e)
+                time.sleep(1)
+                continue
+
             self.samples_scanned += 1
 
             self.is_malware_detected(result_in_json=j)
 
         if self.malware_found == False:
-            logging.info(f"scanned {self.samples_scanned} sample(s); no malware was detected")
+            logging.info(f"no malware was detected")
 
         return self.malware_found
 
     def is_malware_detected(self, result_in_json) -> bool:
         r = result_in_json["query_status"]
 
         if r == "ok":  # query status of 'ok' means malware was detected
             logging.warning("[!] MALWARE DETECTED!")
             self.malware_found = True
-            print(result_in_json)
+            print(json.dumps(result_in_json, indent=2))
             return True
 
         elif r == "hash_not_found":
             return False
 
         elif r == "http_post_expected" or r == "illegal_hash" or r == "no_hash_provided":
             logging.error(result_in_json)
```

### Comparing `miley-0.1.3/miley/main.py` & `miley-1.0.0/miley/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 #!/usr/bin/env python3
 
 import argparse
 import logging
 import os
 
 from miley.client import *
+from miley.container_handler import *
+from miley.dir_walker import *
+from miley.hasher import *
+
 
 
 def main():
     parser = argparse.ArgumentParser(prog="miley", description="A light weight malware scanner")
     parser.add_argument("--hash", help="An MD5, SHA1, or SHA256 hash to scan")
     parser.add_argument("--path", help="Path to a directory or file to scan")
     parser.add_argument("--img", help="A container image of the form 'NAME[:TAG|@DIGEST]'")
@@ -17,31 +21,34 @@
 
     hashes_to_scan = []
 
     if args.hash is not None:
         hashes_to_scan.append(args.hash)
 
     elif args.path is not None:
-        logging.error("sorry, not implemented yet")
-        return
+        files = walk_dir(args.path)
+        hashes_to_scan = hash_files(files)
 
     elif args.img is not None:
-        logging.error("sorry, not implemented yet")
-        return
+        c = Container()
+        c.get(args.img)
+        c.unpack_container_archive()
+        files = walk_dir(c.extracted_path)
+        hashes_to_scan = hash_files(files)
 
     elif args.tar is not None:
         logging.error("sorry, not implemented yet")
         return
 
     else:
         parser.print_help()
         return
 
     c = Client()
-    c.query_hashes(hashes=[args.hash])
+    c.query_hashes(hashes=hashes_to_scan)
 
 
 if __name__ == "__main__":
     logging.basicConfig(level=logging.INFO)
     main()
 
 """
```

