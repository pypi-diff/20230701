# Comparing `tmp/lyrics_transcriber-0.1.0.tar.gz` & `tmp/lyrics_transcriber-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyrics_transcriber-0.1.0.tar", max compression
+gzip compressed data, was "lyrics_transcriber-0.2.0.tar", max compression
```

## Comparing `lyrics_transcriber-0.1.0.tar` & `lyrics_transcriber-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-07-01 00:07:55.170976 lyrics_transcriber-0.1.0/LICENSE
--rw-r--r--   0        0        0      175 2023-07-01 00:06:58.761216 lyrics_transcriber-0.1.0/README.md
--rw-r--r--   0        0        0       43 2023-07-01 00:11:39.196659 lyrics_transcriber-0.1.0/lyrics_transcriber/__init__.py
--rw-r--r--   0        0        0     1276 2023-07-01 00:24:21.482818 lyrics_transcriber-0.1.0/lyrics_transcriber/transcriber.py
--rw-r--r--   0        0        0        0 2023-06-30 23:05:50.978048 lyrics_transcriber-0.1.0/lyrics_transcriber/utils/__init__.py
--rwxr-xr-x   0        0        0     1771 2023-07-01 00:24:45.527729 lyrics_transcriber-0.1.0/lyrics_transcriber/utils/cli.py
--rw-r--r--   0        0        0      670 2023-07-01 00:19:31.276071 lyrics_transcriber-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 lyrics_transcriber-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-01 00:07:55.170976 lyrics_transcriber-0.2.0/LICENSE
+-rw-r--r--   0        0        0      175 2023-07-01 00:06:58.761216 lyrics_transcriber-0.2.0/README.md
+-rw-r--r--   0        0        0      166 2023-07-01 06:11:17.042441 lyrics_transcriber-0.2.0/lyrics_transcriber/__init__.py
+-rw-r--r--   0        0        0     5452 2023-07-01 06:31:01.922934 lyrics_transcriber-0.2.0/lyrics_transcriber/transcriber.py
+-rw-r--r--   0        0        0        0 2023-06-30 23:05:50.978048 lyrics_transcriber-0.2.0/lyrics_transcriber/utils/__init__.py
+-rwxr-xr-x   0        0        0     2331 2023-07-01 06:36:41.239891 lyrics_transcriber-0.2.0/lyrics_transcriber/utils/cli.py
+-rw-r--r--   0        0        0      804 2023-07-01 06:37:27.683806 lyrics_transcriber-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1032 1970-01-01 00:00:00.000000 lyrics_transcriber-0.2.0/PKG-INFO
```

### Comparing `lyrics_transcriber-0.1.0/LICENSE` & `lyrics_transcriber-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lyrics_transcriber-0.1.0/lyrics_transcriber/utils/cli.py` & `lyrics_transcriber-0.2.0/lyrics_transcriber/utils/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 #!/usr/bin/env python
 import argparse
 import datetime
 import pkg_resources
 from lyrics_transcriber import LyricsTranscriber
 
 
+def log(message):
+    timestamp = datetime.datetime.now().isoformat()
+    print(f"{timestamp} - {message}")
+
+
 def main():
     parser = argparse.ArgumentParser(
         description="Create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, from any input song file"
     )
 
-    parser.add_argument("audio_file", nargs="?", help="The audio file path to transcribe lyrics for.", default=argparse.SUPPRESS)
+    parser.add_argument("audio_filepath", nargs="?", help="The audio file path to transcribe lyrics for.", default=argparse.SUPPRESS)
     parser.add_argument("--cache_dir", default="/tmp/lyrics-transcriber-cache/", help="Optional cache directory.")
     parser.add_argument(
         "--output_dir",
         default=None,
         help="Optional directory where the resulting lyrics files will be saved. If not specified, outputs to current dir.",
     )
     parser.add_argument("--version", action="store_true", help="Show the version number and exit")
@@ -22,28 +27,36 @@
     args = parser.parse_args()
 
     if args.version:
         version = pkg_resources.get_distribution("lyrics-transcriber").version
         print(f"lyrics-transcriber version: {version}")
         exit(0)
 
-    if not hasattr(args, "audio_file"):
+    if not hasattr(args, "audio_filepath"):
         parser.print_help()
         exit(1)
 
-    log(f"LyricsTranscriber instantiating with input file: {args.audio_file}")
-
-    transcriber = LyricsTranscriber(args.audio_file, output_dir=args.output_dir, cache_dir=args.cache_dir)
+    transcriber = LyricsTranscriber(args.audio_filepath, output_dir=args.output_dir, cache_dir=args.cache_dir)
 
     log("LyricsTranscriber beginning transcription")
-    whisper_json_filepath, genius_lyrics_filepath, midico_lrc_filepath = transcriber.transcribe()
 
-    print(f"Transcription complete! Output files: {whisper_json_filepath} {genius_lyrics_filepath} {midico_lrc_filepath}")
+    result_metadata = transcriber.generate()
 
+    log(f"*** Success! ***")
 
-def log(message):
-    timestamp = datetime.datetime.now().isoformat()
-    print(f"{timestamp} - {message}")
+    formatted_duration = f'{int(result_metadata["song_duration"] // 60):02d}:{int(result_metadata["song_duration"] % 60):02d}'
+    log(f"Total Song Duration: {formatted_duration}")
+
+    formatted_singing_duration = (
+        f'{int(result_metadata["total_singing_duration"] // 60):02d}:{int(result_metadata["total_singing_duration"] % 60):02d}'
+    )
+    log(f"Total Singing Duration: {formatted_singing_duration}")
+    log(f"Singing Percentage: {result_metadata['singing_percentage']}")
+
+    log(f"*** Outputs: ***")
+    log(f"Whisper transcription output JSON file: {result_metadata['whisper_json_filepath']}")
+    log(f"MidiCo LRC output file: {result_metadata['midico_lrc_filepath']}")
+    log(f"Genius lyrics output file: {result_metadata['genius_lyrics_filepath']}")
 
 
 if __name__ == "__main__":
     main()
```

