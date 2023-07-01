# Comparing `tmp/pyvhs-0.1.1.tar.gz` & `tmp/pyvhs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvhs-0.1.1.tar", max compression
+gzip compressed data, was "pyvhs-0.1.2.tar", max compression
```

## Comparing `pyvhs-0.1.1.tar` & `pyvhs-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1068 2023-06-19 13:27:10.974931 pyvhs-0.1.1/LICENSE
--rw-r--r--   0        0        0     9080 2023-06-24 13:34:33.656701 pyvhs-0.1.1/README.md
--rw-r--r--   0        0        0   176080 2023-06-19 12:45:19.455984 pyvhs-0.1.1/doc/imgs/playback.png
--rw-r--r--   0        0        0   242536 2023-06-19 12:48:00.793752 pyvhs-0.1.1/doc/imgs/pyvhs.png
--rw-r--r--   0        0        0      570 2023-06-24 14:00:52.772960 pyvhs-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-19 19:27:59.639929 pyvhs-0.1.1/pyvhs/__init__.py
--rw-r--r--   0        0        0    59151 2023-06-17 12:32:19.507485 pyvhs-0.1.1/pyvhs/template_imgs/template001.png
--rw-r--r--   0        0        0     2321 2023-06-17 12:48:13.782701 pyvhs-0.1.1/pyvhs/template_imgs/template002.png
--rw-r--r--   0        0        0        0 2023-06-18 18:24:43.368411 pyvhs-0.1.1/pyvhs/utils/__init__.py
--rw-r--r--   0        0        0     8282 2023-06-24 11:23:09.359583 pyvhs-0.1.1/pyvhs/utils/edits.py
--rw-r--r--   0        0        0      976 2023-06-22 00:50:19.366984 pyvhs-0.1.1/pyvhs/utils/files.py
--rw-r--r--   0        0        0     4006 2023-06-24 13:58:02.727393 pyvhs-0.1.1/pyvhs/vhs.py
--rw-r--r--   0        0        0     9926 1970-01-01 00:00:00.000000 pyvhs-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-19 13:27:10.974931 pyvhs-0.1.2/LICENSE
+-rw-r--r--   0        0        0     9080 2023-06-24 13:34:33.656701 pyvhs-0.1.2/README.md
+-rw-r--r--   0        0        0   176080 2023-06-19 12:45:19.455984 pyvhs-0.1.2/doc/imgs/playback.png
+-rw-r--r--   0        0        0   242536 2023-06-19 12:48:00.793752 pyvhs-0.1.2/doc/imgs/pyvhs.png
+-rw-r--r--   0        0        0      570 2023-07-01 16:40:20.739303 pyvhs-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-19 19:27:59.639929 pyvhs-0.1.2/pyvhs/__init__.py
+-rw-r--r--   0        0        0    59151 2023-06-17 12:32:19.507485 pyvhs-0.1.2/pyvhs/template_imgs/template001.png
+-rw-r--r--   0        0        0     2321 2023-06-17 12:48:13.782701 pyvhs-0.1.2/pyvhs/template_imgs/template002.png
+-rw-r--r--   0        0        0        0 2023-06-18 18:24:43.368411 pyvhs-0.1.2/pyvhs/utils/__init__.py
+-rw-r--r--   0        0        0    11843 2023-07-01 16:39:33.865046 pyvhs-0.1.2/pyvhs/utils/edits.py
+-rw-r--r--   0        0        0     1217 2023-07-01 16:36:30.187897 pyvhs-0.1.2/pyvhs/utils/files.py
+-rw-r--r--   0        0        0     4565 2023-07-01 16:36:30.187897 pyvhs-0.1.2/pyvhs/vhs.py
+-rw-r--r--   0        0        0     9926 1970-01-01 00:00:00.000000 pyvhs-0.1.2/PKG-INFO
```

### Comparing `pyvhs-0.1.1/LICENSE` & `pyvhs-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvhs-0.1.1/README.md` & `pyvhs-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyvhs-0.1.1/doc/imgs/playback.png` & `pyvhs-0.1.2/doc/imgs/playback.png`

 * *Files identical despite different names*

### Comparing `pyvhs-0.1.1/doc/imgs/pyvhs.png` & `pyvhs-0.1.2/doc/imgs/pyvhs.png`

 * *Files identical despite different names*

### Comparing `pyvhs-0.1.1/pyproject.toml` & `pyvhs-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyvhs"
-version = "0.1.1"
+version = "0.1.2"
 description = "Digitized VHS Cassette Editing with Python"
 authors = ["Myles Dunlap"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mddunlap924/PyVHS/tree/main"
 keywords = ["vhs", "vcr", "image processing", "video"]
```

### Comparing `pyvhs-0.1.1/pyvhs/template_imgs/template001.png` & `pyvhs-0.1.2/pyvhs/template_imgs/template001.png`

 * *Files identical despite different names*

### Comparing `pyvhs-0.1.1/pyvhs/template_imgs/template002.png` & `pyvhs-0.1.2/pyvhs/template_imgs/template002.png`

 * *Files identical despite different names*

### Comparing `pyvhs-0.1.1/pyvhs/utils/edits.py` & `pyvhs-0.1.2/pyvhs/utils/edits.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,29 @@
 from multiprocessing import Pool, cpu_count
 from functools import partial
 import numpy as np
 from skimage.metrics import structural_similarity as ssim
 from moviepy.editor import VideoFileClip, concatenate_videoclips
 
 
+def convert(seconds):
+    """
+    Converts seconds into hours, minutes, seconds
+
+    Args:
+        seconds (_type_): Total seconds
+
+    Returns:
+        _type_: Hours, mintues, seconds
+    """
+    min, sec = divmod(seconds, 60)
+    hour, min = divmod(min, 60)
+    return '%dhours %02dminutes %02dseconds' % (hour, min, sec)
+
+
 def templates_similarity(template_imgs: list,
                          img: np.array,
                          threshold: float):
     """
     The maximum Structural Similarity Index (SSIM) between a list of template images
     and a video frame.
 
@@ -97,21 +112,36 @@
     # seqs = [(key, start, length), ...]
     seqs = [(key, sum(s[1] for s in seqs[:i]), len) for i, (key, len) in enumerate(seqs)]
 
     # Sequences equal to one
     # (i.e., no time-to-time differences in being identified as blank image)
     # index of blank segments in vec >= num_seq_blanks
     blank_segs = [[s[1], s[1] + s[2] - 1]
-                  for s in seqs 
+                  for s in seqs
                   if s[0] == 1 and s[2] >= num_sequentially_blanks]
 
     footage_segs = [[s[1], s[1] + s[2] - 1]
-                    for s in seqs 
+                    for s in seqs
                     if s[0] == 0 and s[2] >= num_sequentially_footage]
-    return blank_segs, footage_segs
+
+    # Add an time step at start and end to ensure no footage is lost
+    # This will retain some blue screens
+    footage_segs_final = []
+    for footage_seg in footage_segs:
+        start, end = footage_seg[0], footage_seg[1]
+        if start == 0:
+            start = 0
+        else:
+            start = start -1
+        if end == len(blanks):
+            end = end
+        else:
+            end = end + 1
+        footage_segs_final.append([start, end])
+    return blank_segs, footage_segs_final
 
 
 class EditVideo:
     def __init__(self,
                  path_original: Path,
                  path_edited: Path,
                  templates: list,
@@ -141,14 +171,17 @@
         clip = VideoFileClip(self.path_original.as_posix())
         self.duration = clip.duration
         # self.nframes = clip.nframes
         self.end_time = math.floor(self.duration)
         del clip
         _ = gc.collect()
 
+        # Path to save log file
+        self.path_log = self.path_original.parent / (self.path_original.stem + '_log.txt')
+
         # Attributes to calculate
         self.blank_segments = []
         self.keep_segments = []
         return
 
     def __resize_templates(self, frame_w: int, frame_h: int):
         """
@@ -206,15 +239,15 @@
         blank_times = [int(i[1]) for i in footage_blank_segments]
 
         # Extract time segments with blanks (i.e., cutout)
         # and footage (i.e., keep)
         (blank_segments,
          keep_segments) = extract_segments(blanks=blank_times,
                                            num_sequentially_blanks=2,
-                                           num_sequentially_footage=2)
+                                           num_sequentially_footage=1)
         self.blank_segments = blank_segments
         self.keep_segments = keep_segments
         # Exit the program if no keep_segments are found (i.e., entire video is blank)
         if not keep_segments:
             raise AssertionError((f'No Footage Found for Video: '
                                   f'{self.path_original.as_posix()}'))
 
@@ -230,11 +263,68 @@
     def save_video(self, final_video_clip: VideoFileClip):
         """
         Save the final video clip to disk
 
         Args:
             final_video_clip (VideoFileClip): Final video clip to be saved to disk
         """
+        # Save final video to disk
         final_video_clip.write_videofile(self.path_edited.as_posix(),
                                          verbose=False)
         return
+
+
+    def save_logger(self,
+                    final_video_clip,
+                    *,
+                    print_blanks: bool=True,
+                    print_keeps: bool=False):
+        """
+        Save a text file showing the segments that were blank (i.e., removed). 
+        The units are in seconds.
+
+        Args:
+            final_video_clip (VideoFileClip): Final video clip.
+            print_blanks (bool, optional): Blank segments in the video clip. Defaults to True.
+            print_keeps (bool, optional): Footage segments in the video clip. Defaults to False.
+        """
+
+        # Save log file to disk
+        with open(self.path_log, 'w') as f:
+            # Original Video Info:
+            f.write((f'Original Video Information:\n\t'
+                        f'Path: {self.path_original.as_posix()}'))
+            f.write(f'Duration: {convert(seconds=self.duration)}\n')
+
+            # Final Video Info:
+            f.write((f'\nEdited/Saved Video Information:\n\t'
+                        f'Path: {self.path_edited.as_posix()}'))
+            f.write(f'Duration: {convert(seconds=final_video_clip.duration)}\n')
+
+            # Amount of time cropped out of final video
+            f.write((f'\nTotal Time of Blank Segments Removed: '
+                        f'{convert(seconds=self.duration - final_video_clip.duration)}\n'))
+
+            # Blank Segments
+            if print_blanks:
+                f.write('\nOriginal Video - Blank Segment Information')
+                if self.blank_segments:
+                    f.write(f'\n\tTotal Num. of Blank Segments: {len(self.blank_segments):,}\n')
+                    for i, blank_seg in enumerate(self.blank_segments):
+                        f.write((f'\tBlank Segment #{(i + 1):,}: '
+                                 f'{blank_seg[0]:,} - {blank_seg[1]:,} seconds\n'))
+                else:
+                    f.write('\n\tNo Blank Segments Identified\n')
+
+            # Keep Segments (i.e., footage saved in new video)
+            if print_keeps:
+                f.write('\nOriginal Video - Footage Segment Information')
+                if self.keep_segments:
+                    f.write(f'\n\tTotal Num. of Footage Segments: {len(self.keep_segments):,}\n')
+                    for i, keep_seg in enumerate(self.keep_segments):
+                        f.write((f'\tFootage Segment #{(i + 1):,}: '
+                                 f'{keep_seg[0]:,} - {keep_seg[1]:,} seconds\n'))
+                else:
+                    f.write('\tNo Footage Segments Identified\n')
+        print(f'\n\tLog File Saved at: \n\t{self.path_log}')
+        return
```

### Comparing `pyvhs-0.1.1/pyvhs/utils/files.py` & `pyvhs-0.1.2/pyvhs/utils/files.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,15 +14,23 @@
 
     def list_videos(self):
 
         # List all files in directory
         if self.is_dir:
             # Assume only video files in the directory
             tmp = list(self.path.glob('**/*'))
-            self.original = [i for i in tmp if i.is_file()]
+
+            # Check that the path is a file
+            tmp = [i for i in tmp if i.is_file()]
+
+            # Remove text files from being processed if they are present
+            tmp = [i for i in tmp if i.suffix != '.txt']
+
+            # Video files to be processed
+            self.original = tmp
         elif self.is_file:
             # Assume the file is video
             self.original = [self.path]
         else:
             raise ValueError('-dir provided is not a directory or file')
 
         # List edited files to be saved
```

### Comparing `pyvhs-0.1.1/pyvhs/vhs.py` & `pyvhs-0.1.2/pyvhs/vhs.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,15 +31,16 @@
     # Determine if running in debug mode
     # If in debug manually point to CFG file
     is_debugger = debugger_is_active()
 
     # Parse the arguments
     if is_debugger:
         args = argparse.Namespace()
-        args.dir = '/nvme4tb/videos_to_edit'
+        args.dir = '/nvme4tb/test_video'
+        args.template_imgs = DEFAULT_PATH_TEMPLATES
     else:
         arg_desc = '''Remove template images from a video file'''
         parser = argparse.ArgumentParser(formatter_class = argparse.RawDescriptionHelpFormatter,
                                          description= arg_desc)
         parser.add_argument("-dir",
                             required=True,
                             type=str,
@@ -89,18 +90,28 @@
             # Identify segments of footage to keep
             final_clip = video_edit.remove_blank_frames()
             print((f'\nIdentified Blank Segments: '
                    f'{round((time.time() - st) / 60, 3)} mins.'))
 
             # Save edited video to disk
             st = time.time()
-            print(f'Saving New Video at: {path_edit}')
-            video_edit.save_video(final_video_clip=final_clip)
-            print((f'\nEdited Video Saved: '
-                   f'{round((time.time() - st) / 60, 3)} mins.'))
+            if video_edit.blank_segments:
+                print(f'Saving New Video at: {path_edit}')
+                video_edit.save_video(final_video_clip=final_clip)
+                print((f'\nEdited Video Saved: '
+                    f'{round((time.time() - st) / 60, 3)} mins.'))
+            else:
+                print((f'Not Saving Edited Video because No Blank '
+                       f'Segments Identified for Video.: \n\t'
+                       f'{path_org.as_posix()}'))
+
+            # Log which segments of the video were blank (i.e., removed and/or kept)
+            video_edit.save_logger(final_video_clip=final_clip,
+                                   print_blanks=True,
+                                   print_keeps=True)
 
             # Clean up memory
             del video_edit, final_clip
             _ = gc.collect()
             print(f'Completed Video {i + 1} of {total_videos}\n\n')
         except Exception:
             print(f'Error for Video: {path_org.as_posix()}')
```

### Comparing `pyvhs-0.1.1/PKG-INFO` & `pyvhs-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvhs
-Version: 0.1.1
+Version: 0.1.2
 Summary: Digitized VHS Cassette Editing with Python
 Home-page: https://github.com/mddunlap924/PyVHS/tree/main
 License: MIT
 Keywords: vhs,vcr,image processing,video
 Author: Myles Dunlap
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyvhs Version: 0.1.1 Summary: Digitized VHS
+Metadata-Version: 2.1 Name: pyvhs Version: 0.1.2 Summary: Digitized VHS
 Cassette Editing with Python Home-page: https://github.com/mddunlap924/PyVHS/
 tree/main License: MIT Keywords: vhs,vcr,image processing,video Author: Myles
 Dunlap Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: matplotlib (>=3.7.1,<4.0.0) Requires-
```

