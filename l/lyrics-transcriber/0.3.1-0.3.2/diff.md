# Comparing `tmp/lyrics_transcriber-0.3.1.tar.gz` & `tmp/lyrics_transcriber-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyrics_transcriber-0.3.1.tar", max compression
+gzip compressed data, was "lyrics_transcriber-0.3.2.tar", max compression
```

## Comparing `lyrics_transcriber-0.3.1.tar` & `lyrics_transcriber-0.3.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-07-01 00:07:55.170976 lyrics_transcriber-0.3.1/LICENSE
--rw-r--r--   0        0        0      175 2023-07-01 00:06:58.761216 lyrics_transcriber-0.3.1/README.md
--rw-r--r--   0        0        0      166 2023-07-01 06:11:17.042441 lyrics_transcriber-0.3.1/lyrics_transcriber/__init__.py
--rw-r--r--   0        0        0     8615 2023-07-01 08:02:34.607189 lyrics_transcriber-0.3.1/lyrics_transcriber/transcriber.py
--rw-r--r--   0        0        0        0 2023-06-30 23:05:50.978048 lyrics_transcriber-0.3.1/lyrics_transcriber/utils/__init__.py
--rwxr-xr-x   0        0        0     3247 2023-07-01 07:57:15.589521 lyrics_transcriber-0.3.1/lyrics_transcriber/utils/cli.py
--rw-r--r--   0        0        0      828 2023-07-01 08:05:19.714586 lyrics_transcriber-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 lyrics_transcriber-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-01 00:07:55.170976 lyrics_transcriber-0.3.2/LICENSE
+-rw-r--r--   0        0        0      175 2023-07-01 00:06:58.761216 lyrics_transcriber-0.3.2/README.md
+-rw-r--r--   0        0        0       94 2023-07-01 16:43:51.383557 lyrics_transcriber-0.3.2/lyrics_transcriber/__init__.py
+-rw-r--r--   0        0        0     8814 2023-07-01 08:07:26.470781 lyrics_transcriber-0.3.2/lyrics_transcriber/transcriber.py
+-rw-r--r--   0        0        0        0 2023-06-30 23:05:50.978048 lyrics_transcriber-0.3.2/lyrics_transcriber/utils/__init__.py
+-rwxr-xr-x   0        0        0     3247 2023-07-01 07:57:15.589521 lyrics_transcriber-0.3.2/lyrics_transcriber/utils/cli.py
+-rw-r--r--   0        0        0      828 2023-07-01 16:44:21.031404 lyrics_transcriber-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 lyrics_transcriber-0.3.2/PKG-INFO
```

### Comparing `lyrics_transcriber-0.3.1/LICENSE` & `lyrics_transcriber-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lyrics_transcriber-0.3.1/lyrics_transcriber/transcriber.py` & `lyrics_transcriber-0.3.2/lyrics_transcriber/transcriber.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,18 @@
         if self.genius_api_token and self.song_artist and self.song_title:
             log(f"fetching lyrics from Genius as genius_api_token, song_artist and song_title were set")
             self.result_metadata["genius_lyrics_filepath"] = self.get_cache_filepath("-genius.txt")
             self.write_genius_lyrics_file()
         else:
             log(f"not fetching lyrics from Genius as song_artist and song_title were not set")
 
+        # TODO: attempt to match up segments from genius lyrics with whisper segments
+
+        # TODO: output synced lyrics from self.whisper_result_dict in ASS format too, using code from the_tuul
+
         if self.output_dir is None:
             self.output_dir = os.getcwd()
 
         self.result_metadata["whisper_json_filepath"] = shutil.copy(self.result_metadata["whisper_json_filepath"], self.output_dir)
         self.result_metadata["midico_lrc_filepath"] = shutil.copy(self.result_metadata["midico_lrc_filepath"], self.output_dir)
         self.result_metadata["genius_lyrics_filepath"] = shutil.copy(self.result_metadata["genius_lyrics_filepath"], self.output_dir)
```

### Comparing `lyrics_transcriber-0.3.1/lyrics_transcriber/utils/cli.py` & `lyrics_transcriber-0.3.2/lyrics_transcriber/utils/cli.py`

 * *Files identical despite different names*

### Comparing `lyrics_transcriber-0.3.1/pyproject.toml` & `lyrics_transcriber-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lyrics-transcriber"
-version = "0.3.1"
+version = "0.3.2"
 description = "Automatically create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, using Whisper and lyrics from Genius and Spotify"
 authors = ["Andrew Beveridge <andrew@beveridge.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "lyrics_transcriber"}]
 
 [tool.poetry.dependencies]
```

### Comparing `lyrics_transcriber-0.3.1/PKG-INFO` & `lyrics_transcriber-0.3.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyrics-transcriber
-Version: 0.3.1
+Version: 0.3.2
 Summary: Automatically create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, using Whisper and lyrics from Genius and Spotify
 License: MIT
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

