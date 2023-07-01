# Comparing `tmp/lyrics_transcriber-0.2.0.tar.gz` & `tmp/lyrics_transcriber-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyrics_transcriber-0.2.0.tar", max compression
+gzip compressed data, was "lyrics_transcriber-0.3.0.tar", max compression
```

## Comparing `lyrics_transcriber-0.2.0.tar` & `lyrics_transcriber-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-07-01 00:07:55.170976 lyrics_transcriber-0.2.0/LICENSE
--rw-r--r--   0        0        0      175 2023-07-01 00:06:58.761216 lyrics_transcriber-0.2.0/README.md
--rw-r--r--   0        0        0      166 2023-07-01 06:11:17.042441 lyrics_transcriber-0.2.0/lyrics_transcriber/__init__.py
--rw-r--r--   0        0        0     5452 2023-07-01 06:31:01.922934 lyrics_transcriber-0.2.0/lyrics_transcriber/transcriber.py
--rw-r--r--   0        0        0        0 2023-06-30 23:05:50.978048 lyrics_transcriber-0.2.0/lyrics_transcriber/utils/__init__.py
--rwxr-xr-x   0        0        0     2331 2023-07-01 06:36:41.239891 lyrics_transcriber-0.2.0/lyrics_transcriber/utils/cli.py
--rw-r--r--   0        0        0      804 2023-07-01 06:37:27.683806 lyrics_transcriber-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1032 1970-01-01 00:00:00.000000 lyrics_transcriber-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-01 00:07:55.170976 lyrics_transcriber-0.3.0/LICENSE
+-rw-r--r--   0        0        0      175 2023-07-01 00:06:58.761216 lyrics_transcriber-0.3.0/README.md
+-rw-r--r--   0        0        0      166 2023-07-01 06:11:17.042441 lyrics_transcriber-0.3.0/lyrics_transcriber/__init__.py
+-rw-r--r--   0        0        0     8127 2023-07-01 07:52:25.913256 lyrics_transcriber-0.3.0/lyrics_transcriber/transcriber.py
+-rw-r--r--   0        0        0        0 2023-06-30 23:05:50.978048 lyrics_transcriber-0.3.0/lyrics_transcriber/utils/__init__.py
+-rwxr-xr-x   0        0        0     3246 2023-07-01 07:48:04.117826 lyrics_transcriber-0.3.0/lyrics_transcriber/utils/cli.py
+-rw-r--r--   0        0        0      828 2023-07-01 07:53:19.156629 lyrics_transcriber-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 lyrics_transcriber-0.3.0/PKG-INFO
```

### Comparing `lyrics_transcriber-0.2.0/LICENSE` & `lyrics_transcriber-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lyrics_transcriber-0.2.0/pyproject.toml` & `lyrics_transcriber-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lyrics-transcriber"
-version = "0.2.0"
+version = "0.3.0"
 description = "Automatically create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, using Whisper and lyrics from Genius and Spotify"
 authors = ["Andrew Beveridge <andrew@beveridge.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "lyrics_transcriber"}]
 
 [tool.poetry.dependencies]
@@ -14,14 +14,15 @@
 llvmlite = "^0"
 numba = "^0.57"
 numpy = "^1"
 onnx = "^1"
 onnxruntime = "^1"
 torch = "^1"
 tqdm = "^4"
+lyricsgenius = "^3.0.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 
 [tool.black]
 line-length = 140
```

### Comparing `lyrics_transcriber-0.2.0/PKG-INFO` & `lyrics_transcriber-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: lyrics-transcriber
-Version: 0.2.0
+Version: 0.3.0
 Summary: Automatically create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, using Whisper and lyrics from Genius and Spotify
 License: MIT
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Cython (>=0,<1)
 Requires-Dist: dtw-python (>=1,<2)
 Requires-Dist: llvmlite (>=0,<1)
+Requires-Dist: lyricsgenius (>=3.0.1,<4.0.0)
 Requires-Dist: numba (>=0.57,<0.58)
 Requires-Dist: numpy (>=1,<2)
 Requires-Dist: onnx (>=1,<2)
 Requires-Dist: onnxruntime (>=1,<2)
 Requires-Dist: torch (>=1,<2)
 Requires-Dist: tqdm (>=4,<5)
 Description-Content-Type: text/markdown
```

