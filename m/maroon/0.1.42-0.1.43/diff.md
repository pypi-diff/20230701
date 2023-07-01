# Comparing `tmp/maroon-0.1.42.tar.gz` & `tmp/maroon-0.1.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maroon-0.1.42.tar", max compression
+gzip compressed data, was "maroon-0.1.43.tar", max compression
```

## Comparing `maroon-0.1.42.tar` & `maroon-0.1.43.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-07-01 09:17:19.766786 maroon-0.1.42/LICENSE
--rw-r--r--   0        0        0      476 2023-07-01 09:17:19.766786 maroon-0.1.42/README.md
--rw-r--r--   0        0        0        0 2023-07-01 09:17:19.766786 maroon-0.1.42/maroon/__init__.py
--rw-r--r--   0        0        0      740 2023-07-01 09:17:19.766786 maroon-0.1.42/maroon/cli.py
--rw-r--r--   0        0        0     1319 2023-07-01 09:17:19.766786 maroon-0.1.42/maroon/cue.py
--rw-r--r--   0        0        0      889 2023-07-01 09:17:19.766786 maroon-0.1.42/maroon/format.py
--rw-r--r--   0        0        0     3248 2023-07-01 09:17:19.766786 maroon-0.1.42/maroon/transform.py
--rw-r--r--   0        0        0      464 2023-07-01 09:17:19.766786 maroon-0.1.42/pyproject.toml
--rw-r--r--   0        0        0     1142 1970-01-01 00:00:00.000000 maroon-0.1.42/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-01 14:29:10.596116 maroon-0.1.43/LICENSE
+-rw-r--r--   0        0        0     1037 2023-07-01 14:29:10.596116 maroon-0.1.43/README.md
+-rw-r--r--   0        0        0        0 2023-07-01 14:29:10.596116 maroon-0.1.43/maroon/__init__.py
+-rw-r--r--   0        0        0     1025 2023-07-01 14:29:10.596116 maroon-0.1.43/maroon/cli.py
+-rw-r--r--   0        0        0     1334 2023-07-01 14:29:10.596116 maroon-0.1.43/maroon/cue.py
+-rw-r--r--   0        0        0      889 2023-07-01 14:29:10.596116 maroon-0.1.43/maroon/rename.py
+-rw-r--r--   0        0        0     4991 2023-07-01 14:29:10.596116 maroon-0.1.43/maroon/transform.py
+-rw-r--r--   0        0        0      464 2023-07-01 14:29:10.596116 maroon-0.1.43/pyproject.toml
+-rw-r--r--   0        0        0     1703 1970-01-01 00:00:00.000000 maroon-0.1.43/PKG-INFO
```

### Comparing `maroon-0.1.42/LICENSE` & `maroon-0.1.43/LICENSE`

 * *Files identical despite different names*

### Comparing `maroon-0.1.42/maroon/cue.py` & `maroon-0.1.43/maroon/cue.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from collections import namedtuple
 
 Track = namedtuple("Track", ["number", "title", "performer", "start_time"])
 
 
-def parse_cue(cue_path):
+def parse_cue(cue_path) -> list[Track]:
     with open(cue_path, "r", encoding="utf-8") as f:
         lines = f.readlines()
 
     tracks = []
     current_track = None
 
     for line in lines:
```

### Comparing `maroon-0.1.42/maroon/format.py` & `maroon-0.1.43/maroon/rename.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         old_folder_path = os.path.join(directory, folder)
         new_folder_path = os.path.join(directory, f"DISC{i}")
         os.rename(old_folder_path, new_folder_path)
 
     print(f"Renamed {len(folders_to_rename)} folders.")
 
 
-def format_music_folder(dir_name):
+def rename_music_folder(dir_name):
     print(f"Tidying directory: {dir_name}")
     _rename_folders(dir_name)
 
 
 if __name__ == "__main__":
     folder = input("Enter folder name: ")
-    format_music_folder(folder)
+    rename_music_folder(folder)
```

