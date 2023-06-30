# Comparing `tmp/ffmpegdevices-0.10.tar.gz` & `tmp/ffmpegdevices-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffmpegdevices-0.10.tar", last modified: Fri Jun 30 17:57:11 2023, max compression
+gzip compressed data, was "ffmpegdevices-0.12.tar", last modified: Fri Jun 30 22:29:36 2023, max compression
```

## Comparing `ffmpegdevices-0.10.tar` & `ffmpegdevices-0.12.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 17:57:11.267133 ffmpegdevices-0.10/
--rw-rw-rw-   0        0        0     1148 2023-06-30 17:57:05.000000 ffmpegdevices-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      110 2023-06-30 17:57:04.000000 ffmpegdevices-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     1943 2023-06-30 17:57:11.268130 ffmpegdevices-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     1285 2023-06-30 17:55:04.000000 ffmpegdevices-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 17:57:11.264141 ffmpegdevices-0.10/ffmpegdevices/
--rw-rw-rw-   0        0        0     1285 2023-06-30 17:55:04.000000 ffmpegdevices-0.10/ffmpegdevices/README.MD
--rw-rw-rw-   0        0        0     2546 2023-06-30 17:51:00.000000 ffmpegdevices-0.10/ffmpegdevices/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-30 17:57:10.000000 ffmpegdevices-0.10/ffmpegdevices/requirements.txt
--rw-rw-rw-   0        0        0        2 2023-06-30 17:57:10.000000 ffmpegdevices-0.10/ffmpegdevices/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-06-30 17:57:11.267133 ffmpegdevices-0.10/ffmpegdevices.egg-info/
--rw-rw-rw-   0        0        0     1943 2023-06-30 17:57:11.000000 ffmpegdevices-0.10/ffmpegdevices.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-06-30 17:57:11.000000 ffmpegdevices-0.10/ffmpegdevices.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 17:57:11.000000 ffmpegdevices-0.10/ffmpegdevices.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-30 17:57:11.000000 ffmpegdevices-0.10/ffmpegdevices.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-06-30 17:57:11.268641 ffmpegdevices-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1294 2023-06-30 17:57:10.000000 ffmpegdevices-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 22:29:36.666978 ffmpegdevices-0.12/
+-rw-rw-rw-   0        0        0     1148 2023-06-30 22:29:29.000000 ffmpegdevices-0.12/LICENSE.rst
+-rw-rw-rw-   0        0        0      110 2023-06-30 22:29:28.000000 ffmpegdevices-0.12/MANIFEST.in
+-rw-rw-rw-   0        0        0    16848 2023-06-30 22:29:36.666978 ffmpegdevices-0.12/PKG-INFO
+-rw-rw-rw-   0        0        0    16190 2023-06-30 22:27:30.000000 ffmpegdevices-0.12/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 22:29:36.663987 ffmpegdevices-0.12/ffmpegdevices/
+-rw-rw-rw-   0        0        0    16190 2023-06-30 22:27:30.000000 ffmpegdevices-0.12/ffmpegdevices/README.MD
+-rw-rw-rw-   0        0        0    20509 2023-06-30 22:27:52.000000 ffmpegdevices-0.12/ffmpegdevices/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-30 22:29:35.000000 ffmpegdevices-0.12/ffmpegdevices/requirements.txt
+-rw-rw-rw-   0        0        0        2 2023-06-30 22:29:35.000000 ffmpegdevices-0.12/ffmpegdevices/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-06-30 22:29:36.665980 ffmpegdevices-0.12/ffmpegdevices.egg-info/
+-rw-rw-rw-   0        0        0    16848 2023-06-30 22:29:36.000000 ffmpegdevices-0.12/ffmpegdevices.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-06-30 22:29:36.000000 ffmpegdevices-0.12/ffmpegdevices.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 22:29:36.000000 ffmpegdevices-0.12/ffmpegdevices.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-30 22:29:36.000000 ffmpegdevices-0.12/ffmpegdevices.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-06-30 22:29:36.667986 ffmpegdevices-0.12/setup.cfg
+-rw-rw-rw-   0        0        0     1294 2023-06-30 22:29:35.000000 ffmpegdevices-0.12/setup.py
```

### Comparing `ffmpegdevices-0.10/LICENSE.rst` & `ffmpegdevices-0.12/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ffmpegdevices-0.10/setup.py` & `ffmpegdevices-0.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.12'''
 DESCRIPTION = '''Retrieves information about all available video and audio devices using FFmpeg.'''
 
 # Setting up
 setup(
     name="ffmpegdevices",
     version=VERSION,
     license='MIT',
```

