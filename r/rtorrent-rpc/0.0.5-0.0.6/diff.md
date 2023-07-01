# Comparing `tmp/rtorrent_rpc-0.0.5.tar.gz` & `tmp/rtorrent_rpc-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtorrent_rpc-0.0.5.tar", max compression
+gzip compressed data, was "rtorrent_rpc-0.0.6.tar", max compression
```

## Comparing `rtorrent_rpc-0.0.5.tar` & `rtorrent_rpc-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1084 2023-06-30 00:45:58.965145 rtorrent_rpc-0.0.5/LICENSE
--rw-r--r--   0        0        0     2511 2023-06-30 00:45:58.965145 rtorrent_rpc-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      741 2023-06-30 00:45:58.965145 rtorrent_rpc-0.0.5/readme.md
--rw-r--r--   0        0        0    22601 2023-06-30 00:45:58.965145 rtorrent_rpc-0.0.5/rtorrent_rpc/__init__.py
--rw-r--r--   0        0        0     1812 2023-06-30 00:45:58.965145 rtorrent_rpc-0.0.5/rtorrent_rpc/helper.py
--rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 rtorrent_rpc-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-07-01 16:17:25.017527 rtorrent_rpc-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2523 2023-07-01 16:17:25.017527 rtorrent_rpc-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      741 2023-07-01 16:17:25.017527 rtorrent_rpc-0.0.6/readme.md
+-rw-r--r--   0        0        0    22583 2023-07-01 16:17:25.017527 rtorrent_rpc-0.0.6/rtorrent_rpc/__init__.py
+-rw-r--r--   0        0        0     2098 2023-07-01 16:17:25.017527 rtorrent_rpc-0.0.6/rtorrent_rpc/helper.py
+-rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 rtorrent_rpc-0.0.6/PKG-INFO
```

### Comparing `rtorrent_rpc-0.0.5/LICENSE` & `rtorrent_rpc-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.0.5/pyproject.toml` & `rtorrent_rpc-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rtorrent-rpc"
-version = "0.0.5"
+version = "0.0.6"
 description = "Typed rtorrent rpc client"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'readme.md'
 repository = 'https://github.com/trim21/rtorrent-rpc'
 license = 'MIT'
 packages = [{ include = 'rtorrent_rpc' }]
 keywords = ['rtorrent', 'rpc']
@@ -104,14 +104,15 @@
     'INP001',
     'N806',
     'N802',
     'N803',
     'E501',
     'BLE001',
     'RUF002',
+    'S324',
     'S301',
     'S314',
     'S101',
     'N815',
     'S104',
     'C901',
     'PLR0913',
```

### Comparing `rtorrent_rpc-0.0.5/readme.md` & `rtorrent_rpc-0.0.6/readme.md`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.0.5/rtorrent_rpc/__init__.py` & `rtorrent_rpc-0.0.6/rtorrent_rpc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import xmlrpc.client
 from collections.abc import Iterator
 from typing import Any, Literal, Protocol, TypeAlias, TypedDict
 
 from rtorrent_xmlrpc import SCGIServerProxy
 from typing_extensions import NotRequired
 
-__all__ = ["RTorrent"]
+__all__ = ["RTorrent", "MultiCall"]
 
 Unknown: TypeAlias = Any
 
 
 class MultiCall(TypedDict):
     methodName: str
     params: NotRequired[Any]
@@ -50,19 +50,25 @@
 
     def add_torrent_by_file(
         self,
         content: bytes,
         directory: str,
         tags: list[str] | None = None,
     ) -> None:
+        """
+
+        :param content: raw torrent content
+        :param directory: download base directory
+        :param tags: optional tags for download
+        """
         params = [
             "",
             content,
             'd.tied_to_file.set=""',
-            f"d.custom.set=addtime,{int(time.time())}",
+            f"d.custom.set=addtime,{int(time.time())}",  # this custom is commonly used by ruTorrent and flood.
             f'd.directory_base.set="{directory}"',
         ]
 
         if tags:
             params.append(f'd.custom1.set="{_encode_tags(tags)}"')
 
         self.rpc.load.raw_start_verbose(*params)
@@ -859,16 +865,7 @@
     "d.session_file",
     "cfg.scrape_interval.active",
     "cfg.scrape_interval.active.set",
     "cfg.scrape_interval.idle",
     "cfg.scrape_interval.idle.set",
     "d.last_scrape.send_set",
 ]
-
-# p = xmlrpc.server.SimpleXMLRPCServer(addr=('127.0.0.1', 5000))
-
-# rt = SCGIServerProxy('scgi://127.0.0.1:5000/')
-
-# info_hash = '2E0BBFB20C2AC4E497D3FD2BDEF2189382010E7A'
-
-# print(rt.d.last_scrape.send_set(info_hash))
-# print(rt.d.tracker(info_hash))
```

### Comparing `rtorrent_rpc-0.0.5/rtorrent_rpc/helper.py` & `rtorrent_rpc-0.0.6/rtorrent_rpc/helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,20 @@
+import hashlib
 from pathlib import Path
 from typing import Any
 
 import bencodepy
 
-__all__ = ["add_completed_resume_file"]
+__all__ = ["add_completed_resume_file", "get_torrent_info_hash"]
+
+
+def get_torrent_info_hash(content: bytes) -> str:
+    """get torrent info_hash in low case string"""
+    data = bencodepy.bdecode(content)
+    return hashlib.sha1(bencodepy.bencode(data[b"info"])).hexdigest()
 
 
 def add_completed_resume_file(base_save_path: Path, torrent_content: bytes) -> bytes:
     """update torrent content, add resume data to torrent.
 
     based on [rtorrent_fast_resume.pl](https://github.com/rakshasa/rtorrent/blob/master/doc/rtorrent_fast_resume.pl)
     """
@@ -17,33 +24,33 @@
     files = []
 
     t_files = data[b"info"].get(b"files")
 
     piece_count = int(len(data[b"info"][b"pieces"]) / 20)
     if t_files:
         for file in t_files:
-            file_path = base_save_path.joinpath(*file[b"path"])
+            file_path = base_save_path.joinpath(*[p.decode() for p in file[b"path"]])
             if not file_path.exists():
                 files.append({b"complete": 0, b"mtime": 0, b"priority": 0})
                 continue
 
             stat = file_path.lstat()
             if stat.st_size == file[b"length"]:
                 files.append(
                     {
-                        b"complete": int(file.length / piece_length),
+                        b"complete": int(file[b"length"] / piece_length),
                         b"mtime": int(stat.st_mtime),
                         b"priority": 1,
                     }
                 )
             else:
                 files.append({b"complete": 0, b"mtime": 0, b"priority": 1})
     else:
         # return torrent_content
-        stat = base_save_path.joinpath(data[b"info"][b"name"]).lstat()
+        stat = base_save_path.joinpath(data[b"info"][b"name"].decode()).lstat()
         if stat.st_size == data[b"info"][b"length"]:
             files.append(
                 {b"complete": piece_count, b"mtime": int(stat.st_mtime), b"priority": 1}
             )
         else:
             return torrent_content
```

### Comparing `rtorrent_rpc-0.0.5/PKG-INFO` & `rtorrent_rpc-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtorrent-rpc
-Version: 0.0.5
+Version: 0.0.6
 Summary: Typed rtorrent rpc client
 Home-page: https://github.com/trim21/rtorrent-rpc
 License: MIT
 Keywords: rtorrent,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.10,<4.0
```

