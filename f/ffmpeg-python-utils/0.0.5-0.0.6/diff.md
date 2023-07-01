# Comparing `tmp/ffmpeg_python_utils-0.0.5.tar.gz` & `tmp/ffmpeg_python_utils-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffmpeg_python_utils-0.0.5.tar", last modified: Fri Jun 30 13:44:47 2023, max compression
+gzip compressed data, was "ffmpeg_python_utils-0.0.6.tar", last modified: Sat Jul  1 04:30:47 2023, max compression
```

## Comparing `ffmpeg_python_utils-0.0.5.tar` & `ffmpeg_python_utils-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 13:44:47.688860 ffmpeg_python_utils-0.0.5/
--rw-rw-rw-   0        0        0     1097 2023-06-28 17:21:41.000000 ffmpeg_python_utils-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      808 2023-06-30 13:44:47.689860 ffmpeg_python_utils-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1634 2023-06-28 22:10:37.000000 ffmpeg_python_utils-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 13:44:47.680859 ffmpeg_python_utils-0.0.5/ffmpeg_python_utils/
--rw-rw-rw-   0        0        0     1043 2023-06-28 19:38:55.000000 ffmpeg_python_utils-0.0.5/ffmpeg_python_utils/__init__.py
--rw-rw-rw-   0        0        0     1428 2023-06-30 13:37:18.000000 ffmpeg_python_utils-0.0.5/ffmpeg_python_utils/config.py
--rw-rw-rw-   0        0        0     4983 2023-06-29 09:14:35.000000 ffmpeg_python_utils-0.0.5/ffmpeg_python_utils/inc.py
--rw-rw-rw-   0        0        0    37683 2023-06-29 12:27:38.000000 ffmpeg_python_utils-0.0.5/ffmpeg_python_utils/main.py
--rw-rw-rw-   0        0        0     8297 2023-06-30 13:37:18.000000 ffmpeg_python_utils-0.0.5/ffmpeg_python_utils/other.py
-drwxrwxrwx   0        0        0        0 2023-06-30 13:44:47.687858 ffmpeg_python_utils-0.0.5/ffmpeg_python_utils.egg-info/
--rw-rw-rw-   0        0        0      808 2023-06-30 13:44:47.000000 ffmpeg_python_utils-0.0.5/ffmpeg_python_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-06-30 13:44:47.000000 ffmpeg_python_utils-0.0.5/ffmpeg_python_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 13:44:47.000000 ffmpeg_python_utils-0.0.5/ffmpeg_python_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-06-30 13:44:47.000000 ffmpeg_python_utils-0.0.5/ffmpeg_python_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-30 13:44:47.000000 ffmpeg_python_utils-0.0.5/ffmpeg_python_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 13:44:47.690861 ffmpeg_python_utils-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1130 2023-06-30 13:39:51.000000 ffmpeg_python_utils-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 04:30:47.290000 ffmpeg_python_utils-0.0.6/
+-rw-rw-rw-   0        0        0     1097 2023-06-28 17:21:41.000000 ffmpeg_python_utils-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      808 2023-07-01 04:30:47.290000 ffmpeg_python_utils-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1634 2023-06-28 22:10:37.000000 ffmpeg_python_utils-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 04:30:47.282998 ffmpeg_python_utils-0.0.6/ffmpeg_python_utils/
+-rw-rw-rw-   0        0        0      954 2023-07-01 03:26:47.000000 ffmpeg_python_utils-0.0.6/ffmpeg_python_utils/__init__.py
+-rw-rw-rw-   0        0        0     1428 2023-06-30 13:37:18.000000 ffmpeg_python_utils-0.0.6/ffmpeg_python_utils/config.py
+-rw-rw-rw-   0        0        0     4983 2023-06-29 09:14:35.000000 ffmpeg_python_utils-0.0.6/ffmpeg_python_utils/inc.py
+-rw-rw-rw-   0        0        0    37861 2023-07-01 04:27:35.000000 ffmpeg_python_utils-0.0.6/ffmpeg_python_utils/main.py
+-rw-rw-rw-   0        0        0     8297 2023-06-30 13:37:18.000000 ffmpeg_python_utils-0.0.6/ffmpeg_python_utils/other.py
+drwxrwxrwx   0        0        0        0 2023-07-01 04:30:47.288999 ffmpeg_python_utils-0.0.6/ffmpeg_python_utils.egg-info/
+-rw-rw-rw-   0        0        0      808 2023-07-01 04:30:47.000000 ffmpeg_python_utils-0.0.6/ffmpeg_python_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-07-01 04:30:47.000000 ffmpeg_python_utils-0.0.6/ffmpeg_python_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 04:30:47.000000 ffmpeg_python_utils-0.0.6/ffmpeg_python_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-01 04:30:47.000000 ffmpeg_python_utils-0.0.6/ffmpeg_python_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-01 04:30:47.000000 ffmpeg_python_utils-0.0.6/ffmpeg_python_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 04:30:47.291001 ffmpeg_python_utils-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1130 2023-07-01 04:30:23.000000 ffmpeg_python_utils-0.0.6/setup.py
```

### Comparing `ffmpeg_python_utils-0.0.5/LICENSE` & `ffmpeg_python_utils-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ffmpeg_python_utils-0.0.5/PKG-INFO` & `ffmpeg_python_utils-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ffmpeg_python_utils
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python scripts constructing ffmpeg commands and running them by subprocess.
 Home-page: https://github.com/LionelCrowl/ffmpeg-python-utils
-Download-URL: https://github.com/LionelCrowl/ffmpeg-python-utils/archive/v0.0.5.zip
+Download-URL: https://github.com/LionelCrowl/ffmpeg-python-utils/archive/v0.0.6.zip
 Author: LionelCrowl
 Author-email: mr.lihenko@yandex.ru
 License: MIT License, see LICENSE file
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ffmpeg_python_utils-0.0.5/README.md` & `ffmpeg_python_utils-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ffmpeg_python_utils-0.0.5/ffmpeg_python_utils/__init__.py` & `ffmpeg_python_utils-0.0.6/ffmpeg_python_utils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,11 +26,7 @@
            'get_rotated_video',
            'get_subclips_with_sound',
            'get_video_from_picture',
            'get_video_info',
            'remove_silence_from_audio_file',
            'find_offsets',
            ]
-
-__author__ = 'LionelCrowl'
-__version__ = '0.0.1'
-__email__ = 'mr.lihenko@yandex.ru'
```

### Comparing `ffmpeg_python_utils-0.0.5/ffmpeg_python_utils/config.py` & `ffmpeg_python_utils-0.0.6/ffmpeg_python_utils/config.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_python_utils-0.0.5/ffmpeg_python_utils/inc.py` & `ffmpeg_python_utils-0.0.6/ffmpeg_python_utils/inc.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_python_utils-0.0.5/ffmpeg_python_utils/main.py` & `ffmpeg_python_utils-0.0.6/ffmpeg_python_utils/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,15 @@
             border_str += f':borderw={border_width}'
         filter_str += f'[0:v]' if i == 0 else f'[v{i}]'
         filter_str += f"drawtext=fontfile='{fonts_paths[i]}':text='{texts[i]}':fontsize={font_sizes[i]}:" \
                       f"fontcolor={font_colors[i]}{fade_str}:x={x_y_coordinates[i][0]}:y={x_y_coordinates[i][1]}{border_str}"
         if start_times is not None and durations is not None:
             filter_str += f":enable='between(t,{start_times[i]},{start_times[i] + durations[i]})'"
         filter_str += f'[v{i + 1}]'
-        filter_str += ';'
+        filter_str += ';' if i != len(texts) - 1 else ''
     # Run
     cmd = f'ffmpeg -y -i "{input_video_path}" -movflags +faststart ' \
           f'-filter_complex "{filter_str}" -map [v{len(texts)}] -map 0:a {C_CODEC_SETTINGS[C_CODEC]} {output_path}'
     run_command(cmd, filter_str)
 
     return output_path
 
@@ -268,15 +268,16 @@
         if opacities and opacities[i] and opacities[i] != 1:
             filter_str_0 += f'format=pix_fmts=rgba,colorchannelmixer=aa={opacities[i]}'
         if fade_duration or (opacities and opacities[i] and opacities[i] != 1):
             filter_str_0 += f'[img{i + 1}];'
 
         filter_str_1 += f"[0]" if i == 0 else f"[bg{i - 1}]"
         filter_str_1 += f"[{if_img_str}{i + 1}]overlay=x={x_y_coordinates[i][0]}:y={x_y_coordinates[i][1]}:" \
-                        f"enable='between(t,{start_times[i]},{start_times[i] + durations[i]})':shortest=1[bg{i}];"
+                        f"enable='between(t,{start_times[i]},{start_times[i] + durations[i]})':shortest=1[bg{i}]"
+        filter_str_1 += ';' if i != len(input_image_paths) - 1 else ''
 
     # Run command
     cmd = (f'ffmpeg -y {files_str} '
            f'-filter_complex "{filter_str_0 + filter_str_1}" '
            f'-map [bg{len(input_image_paths) - 1}]  -map 0 -map 0:a  -c:a copy {C_CODEC_SETTINGS[C_CODEC]} '
            f'-movflags +faststart "{output_path}" ')
     run_command(cmd, filter_str_0 + filter_str_1)
@@ -431,15 +432,16 @@
             fade_duration = min(fade_duration, durations[i] / 2)
             filter_str_0 += f'fade=t=in:st={start_times[i]}:d={fade_duration}:alpha=1,fade=t=out:st={start_times[i] + durations[i] - fade_duration}:d={fade_duration}:alpha=1,'
         if fade_duration or (opacities and opacities[i] and opacities[i] != 1):
             filter_str_0 += f'format=pix_fmts=rgba,colorchannelmixer=aa={opacities[i]},'
         filter_str_0 += f'scale={goal_sizes[i][0]}:{goal_sizes[i][1]}[v{i + 1}];'
 
         filter_str_1 += f'[orig]' if i == 0 else f'[fin{i}]'
-        filter_str_1 += f'[v{i + 1}]overlay={x_y_coordinates[i][0]}:{x_y_coordinates[i][1]}[fin{i + 1}];'
+        filter_str_1 += f'[v{i + 1}]overlay={x_y_coordinates[i][0]}:{x_y_coordinates[i][1]}[fin{i + 1}]'
+        filter_str_1 += ';' if i != len(video_to_overlay_paths) - 1 else ''
 
     # Run command
     cmd = f'ffmpeg -y -i "{input_video_path}" {input_str} -movflags +faststart -filter_complex ' \
           f'"{filter_str_0 + filter_str_1}"' \
           f' -map [fin{len(video_to_overlay_paths)}] -map 0:a ' \
           f'{C_CODEC_SETTINGS[codec_to_use]}' \
           f' -c:a copy "{output_path}"'
```

### Comparing `ffmpeg_python_utils-0.0.5/ffmpeg_python_utils/other.py` & `ffmpeg_python_utils-0.0.6/ffmpeg_python_utils/other.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_python_utils-0.0.5/ffmpeg_python_utils.egg-info/PKG-INFO` & `ffmpeg_python_utils-0.0.6/ffmpeg_python_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ffmpeg-python-utils
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python scripts constructing ffmpeg commands and running them by subprocess.
 Home-page: https://github.com/LionelCrowl/ffmpeg-python-utils
-Download-URL: https://github.com/LionelCrowl/ffmpeg-python-utils/archive/v0.0.5.zip
+Download-URL: https://github.com/LionelCrowl/ffmpeg-python-utils/archive/v0.0.6.zip
 Author: LionelCrowl
 Author-email: mr.lihenko@yandex.ru
 License: MIT License, see LICENSE file
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ffmpeg_python_utils-0.0.5/setup.py` & `ffmpeg_python_utils-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = '0.0.5'
+version = '0.0.6'
 
 description = 'Python scripts constructing ffmpeg commands and running them by subprocess.'
 
 long_description = ''' Python scripts constructing ffmpeg commands and running them by subprocess.
                     Check documentation: https://lionelcrowl.github.io/ffmpeg-python-utils/
                     '''
```

