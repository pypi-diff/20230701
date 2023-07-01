# Comparing `tmp/y2mate-api-0.0.8.tar.gz` & `tmp/y2mate-api-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "y2mate-api-0.0.8.tar", last modified: Fri Jun 23 12:37:25 2023, max compression
+gzip compressed data, was "y2mate-api-0.0.9.tar", last modified: Sat Jul  1 20:45:50 2023, max compression
```

## Comparing `y2mate-api-0.0.8.tar` & `y2mate-api-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-23 12:37:25.734000 y2mate-api-0.0.8/
--rw-rw----   0 root         (0) everybody  (9997)     1064 2023-06-16 15:42:28.000000 y2mate-api-0.0.8/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)    11042 2023-06-23 12:37:25.718000 y2mate-api-0.0.8/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     9947 2023-06-23 12:11:48.000000 y2mate-api-0.0.8/README.md
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-23 12:37:25.734000 y2mate-api-0.0.8/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1590 2023-06-23 12:31:47.000000 y2mate-api-0.0.8/setup.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-23 12:37:25.262000 y2mate-api-0.0.8/tests/
--rw-rw----   0 root         (0) everybody  (9997)     1567 2023-06-21 13:35:40.000000 y2mate-api-0.0.8/tests/test_download.py
--rw-rw----   0 root         (0) everybody  (9997)     5577 2023-06-20 21:29:31.000000 y2mate-api-0.0.8/tests/test_queries.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-23 12:37:25.386000 y2mate-api-0.0.8/y2mate_api/
--rw-rw----   0 root         (0) everybody  (9997)      490 2023-06-22 17:33:46.000000 y2mate-api-0.0.8/y2mate_api/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)       34 2023-06-19 18:39:03.000000 y2mate-api-0.0.8/y2mate_api/__main__.py
--rw-rw----   0 root         (0) everybody  (9997)     5707 2023-06-22 15:05:00.000000 y2mate-api-0.0.8/y2mate_api/console.py
--rw-rw----   0 root         (0) everybody  (9997)    14847 2023-06-23 12:01:05.000000 y2mate-api-0.0.8/y2mate_api/downloader.py
--rw-rw----   0 root         (0) everybody  (9997)    14731 2023-06-22 17:22:06.000000 y2mate-api-0.0.8/y2mate_api/main.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-23 12:37:25.650000 y2mate-api-0.0.8/y2mate_api.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)    11042 2023-06-23 12:37:24.000000 y2mate-api-0.0.8/y2mate_api.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      389 2023-06-23 12:37:24.000000 y2mate-api-0.0.8/y2mate_api.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-23 12:37:24.000000 y2mate-api-0.0.8/y2mate_api.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       51 2023-06-23 12:37:24.000000 y2mate-api-0.0.8/y2mate_api.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       85 2023-06-23 12:37:24.000000 y2mate-api-0.0.8/y2mate_api.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)       11 2023-06-23 12:37:24.000000 y2mate-api-0.0.8/y2mate_api.egg-info/top_level.txt
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-01 20:45:50.389384 y2mate-api-0.0.9/
+-rw-rw----   0 root         (0) everybody  (9997)     1064 2023-06-16 15:42:28.000000 y2mate-api-0.0.9/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)    11314 2023-07-01 20:45:50.373384 y2mate-api-0.0.9/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)    10219 2023-07-01 20:44:36.000000 y2mate-api-0.0.9/README.md
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-01 20:45:50.389384 y2mate-api-0.0.9/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1587 2023-06-30 18:02:19.000000 y2mate-api-0.0.9/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-01 20:45:49.865383 y2mate-api-0.0.9/tests/
+-rw-rw----   0 root         (0) everybody  (9997)     1567 2023-06-21 13:35:40.000000 y2mate-api-0.0.9/tests/test_download.py
+-rw-rw----   0 root         (0) everybody  (9997)     5577 2023-06-20 21:29:31.000000 y2mate-api-0.0.9/tests/test_queries.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-01 20:45:50.037384 y2mate-api-0.0.9/y2mate_api/
+-rw-rw----   0 root         (0) everybody  (9997)      490 2023-06-30 18:01:50.000000 y2mate-api-0.0.9/y2mate_api/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)       34 2023-06-19 18:39:03.000000 y2mate-api-0.0.9/y2mate_api/__main__.py
+-rw-rw----   0 root         (0) everybody  (9997)     5860 2023-07-01 20:41:24.000000 y2mate-api-0.0.9/y2mate_api/console.py
+-rw-rw----   0 root         (0) everybody  (9997)    15396 2023-07-01 20:39:21.000000 y2mate-api-0.0.9/y2mate_api/downloader.py
+-rw-rw----   0 root         (0) everybody  (9997)    14731 2023-06-22 17:22:06.000000 y2mate-api-0.0.9/y2mate_api/main.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-01 20:45:50.345384 y2mate-api-0.0.9/y2mate_api.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)    11314 2023-07-01 20:45:48.000000 y2mate-api-0.0.9/y2mate_api.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      389 2023-07-01 20:45:49.000000 y2mate-api-0.0.9/y2mate_api.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-01 20:45:48.000000 y2mate-api-0.0.9/y2mate_api.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       51 2023-07-01 20:45:48.000000 y2mate-api-0.0.9/y2mate_api.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       99 2023-07-01 20:45:48.000000 y2mate-api-0.0.9/y2mate_api.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)       11 2023-07-01 20:45:48.000000 y2mate-api-0.0.9/y2mate_api.egg-info/top_level.txt
```

### Comparing `y2mate-api-0.0.8/LICENSE` & `y2mate-api-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `y2mate-api-0.0.8/PKG-INFO` & `y2mate-api-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: y2mate-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: Download youtube videos and audios by title or link
 Home-page: https://github.com/Simatwa/y2mate-api
 Author: Smartwa
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/y2mate-api/issues/new
@@ -25,17 +25,17 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">y2mate-api</h1>
 
 <p align="center">
-<a href="https://github.com/Simatwa/y2mate-api"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a>
+<a href="https://github.com/Simatwa/y2mate-api/actions/workflows/python-test.yml"><img src="https://github.com/Simatwa/y2mate-api/actions/workflows/python-test.yml/badge.svg" alt="Python Test"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.8&color=green"/></a>
+<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.9&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/y2mate-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
 </p>
 
@@ -152,15 +152,15 @@
 **Note** : You can still use  **video id** such as `POPoAjWFkGg` as query parameter.
 
 ## Other parameters
 
 - `Handler`
   * author : Video author i.e Youtube Channel
   * timeout : http requests timeout
-  * ask : Confirm before downloading media
+  * confirm : Confirm before downloading media
   * unique : Auto-ignore previously downloaded media
   * thread : Download (x) value of file at a time.
 
 - `Handler.run`
   * format : Media format mp4/mp3
   * quality : Media quality such as 720p/128kbps
   * resolver : Additional format info : [m4a,3gp,mp4,mp3]
@@ -176,32 +176,33 @@
 - `Handler.save`
   * third_dict : Response of `third_query.run()`
   * dir : Directory for saving the contents
   * progress_bar : Display download progress bar
   * quiet : Not to stdout anything
   * naming_format : Format for generating media filename using the `third_query` response keys
   * chunk_size : Size of chunks in KB for downloads
- 
+  * play : Auto-play media after downloading 
 </details>
  
 <details>
 <summary>
 	
 For more info run `$ y2mate -h`
 
 </summary>
 
 ```
 usage: y2mate [-h] [-v] [-f mp3|mp4]
               [-q 4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
               [-r m4a|3gp|mp4|mp3] [-k [KEYWORD ...]]
               [-a [AUTHOR ...]] [-l LIMIT] [-d PATH]
-              [-t TIMEOUT] [-c CHUNK] [-i PATH] [-o FORMAT]
-              [-thr THREAD] [--disable-bar] [--ask]
-              [--unique] [--quiet] [--history] [--clear]
+              [-t TIMEOUT] [-c CHUNK] [-i PATH]
+              [-o FORMAT] [-thr THREAD] [--disable-bar]
+              [--confirm] [--unique] [--quiet]
+              [--history] [--clear] [--play]
               [query ...]
 
 Download youtube videos and audios by title or link
 
 positional arguments:
   query                 Youtube video title, link or id -
                         None
@@ -214,49 +215,54 @@
                         Specify media type - audio/video
   -q 4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps, --quality 4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps
                         Media quality - auto
   -r m4a|3gp|mp4|mp3, --resolver m4a|3gp|mp4|mp3
                         Other media formats incase of
                         multiple options - mp4/mp3
   -k [KEYWORD ...], --keyword [KEYWORD ...]
-                        Media should contain this keywords -
-                        None
+                        Media should contain this
+                        keywords - None
   -a [AUTHOR ...], --author [AUTHOR ...]
                         Media author i.e YouTube channel
                         name - None
   -l LIMIT, --limit LIMIT
                         Total videos to be downloaded - 1
-  -d PATH, --dir PATH   Directory for saving the contents -
-                        /data/data/com.termux/files/home
+  -d PATH, --dir PATH   Directory for saving the contents
+                        - /storage/emulated/0/git/Smartwa
+                        /y2mate-api
   -t TIMEOUT, --timeout TIMEOUT
-                        Http request timeout in seconds - 30
+                        Http request timeout in seconds -
+                        30
   -c CHUNK, --chunk CHUNK
-                        Chunk-size for downloading files in
-                        KB - 256
+                        Chunk-size for downloading files
+                        in KB - 256
   -i PATH, --input PATH
-                        Path to text file containing query
-                        per line - None
+                        Path to text file containing
+                        query per line - None
   -o FORMAT, --output FORMAT
                         Format for generating filename
-                        %(key)s : [title,vid,fquality,ftype]
-                        or 'pretty' - None
+                        %(key)s :
+                        [title,vid,fquality,ftype] or
+                        'pretty' - None
   -thr THREAD, --thread THREAD
-                        Download [x] amount of videos/audios
-                        at once - 1
+                        Download [x] amount of
+                        videos/audios at once - 1
   --disable-bar         Disable download progress bar -
                         False
-  --ask                 Confirm before downloading file -
+  --confirm             Confirm before downloading file -
                         False
   --unique              Auto-skip any media that you once
                         dowloaded - False
   --quiet               Not to stdout anything other than
                         logs - False
   --history             Stdout all media metadata ever
                         downloaded - False
-  --clear               Clear all download histories - False
+  --clear               Clear all download histories -
+                        False
+  --play                Play media after download - False
 
 This script has no official relation with y2mate.com
 ```
 </details>
 
 - Review [CHANGELOG](https://github.com/Simatwa/y2mate-api/blob/main/Docs/CHANGELOG.md) for latest updates.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.8 Summary: Download youtube
+Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.9 Summary: Download youtube
 videos and audios by title or link Home-page: https://github.com/Simatwa/
 y2mate-api Author: Smartwa Author-email: smartwacaleb@gmail.com Maintainer:
 Smartwa License: MIT Project-URL: Bug Report, https://github.com/Simatwa/
 y2mate-api/issues/new Keywords: y2mate,videos,video-api,youtube Classifier:
 License :: OSI Approved :: MIT License Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: Free For Home Use Classifier: Intended
@@ -10,15 +10,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE
                            ****** y2mate-api ******
- [Github] [License] [PyPi] [Black] [Passing] [coverage] [Progress] [Downloads]
+    [Python_Test] [License] [PyPi] [Black] [Passing] [coverage] [Progress]
+                                  [Downloads]
 > Download youtube videos and audios by **title/id/url** # Installation -
 Either of the following ways will get you ready. 1. Pip a. From source ```sh
 pip install git+https://github.com/Simatwa/y2mate-api.git ``` b. From pypi
 ```sh pip install y2mate-api ``` 2. Locally ```sh git clone https://github.com/
 Simatwa/y2mate-api.git cd y2mate-api pip install . ``` # Usage `$ y2mate -f
 p4> `   Developer docs  1.Generate download links and other metadata - Video
 ```py from y2mate_api import Handler api = Handler("Quantum computing in
@@ -52,57 +53,59 @@
 download the first video found and save it in the `current directory` You can
 as well specify total videos to be downloaded by using `limit` argument. For
 instance: ```py from y2mate_api import Handler api = Handler("https://youtu.be/
 POPoAjWFkGg") api.auto_save(limit=10) # This will download the video in path
 and 9 other videos related to the query specified ``` **Note** : You can still
 use **video id** such as `POPoAjWFkGg` as query parameter. ## Other parameters
 - `Handler` * author : Video author i.e Youtube Channel * timeout : http
-requests timeout * ask : Confirm before downloading media * unique : Auto-
+requests timeout * confirm : Confirm before downloading media * unique : Auto-
 ignore previously downloaded media * thread : Download (x) value of file at a
 time. - `Handler.run` * format : Media format mp4/mp3 * quality : Media quality
 such as 720p/128kbps * resolver : Additional format info : [m4a,3gp,mp4,mp3] *
 limit : Total videos to be retrieved * keyword : Phrase(s) that must be in
 media title * author : Video author i.e Youtube Channel - `Handler.auto_save` *
 dir : Path to Directory for saving the media files * iterator : Function that
 yields third_query object - `Handler.run` * progress_bar : Stdout media-name &
 Display progress bar - `Handler.save` * third_dict : Response of
 `third_query.run()` * dir : Directory for saving the contents * progress_bar :
 Display download progress bar * quiet : Not to stdout anything * naming_format
 : Format for generating media filename using the `third_query` response keys *
-chunk_size : Size of chunks in KB for downloads    For more info run `$ y2mate
--h`  ``` usage: y2mate [-h] [-v] [-f mp3|mp4] [-
+chunk_size : Size of chunks in KB for downloads * play : Auto-play media after
+downloading    For more info run `$ y2mate -h`  ``` usage: y2mate [-h] [-v] [-
+f mp3|mp4] [-
 q
 4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
 [-r m4a|3gp|mp4|mp3] [-k [KEYWORD ...]] [-a [AUTHOR ...]] [-l LIMIT] [-d PATH]
 [-t TIMEOUT] [-c CHUNK] [-i PATH] [-o FORMAT] [-thr THREAD] [--disable-bar] [--
-ask] [--unique] [--quiet] [--history] [--clear] [query ...] Download youtube
-videos and audios by title or link positional arguments: query Youtube video
-title, link or id - None options: -h, --help show this help message and exit -
-v, --version show program's version number and exit -f mp3|mp4, --format
-mp3|mp4 Specify media type - audio/video -
+confirm] [--unique] [--quiet] [--history] [--clear] [--play] [query ...]
+Download youtube videos and audios by title or link positional arguments: query
+Youtube video title, link or id - None options: -h, --help show this help
+message and exit -v, --version show program's version number and exit -
+f mp3|mp4, --format mp3|mp4 Specify media type - audio/video -
 q
 4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps,
 --quality
 4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps
 Media quality - auto -r m4a|3gp|mp4|mp3, --resolver m4a|3gp|mp4|mp3 Other media
 formats incase of multiple options - mp4/mp3 -k [KEYWORD ...], --keyword
 [KEYWORD ...] Media should contain this keywords - None -a [AUTHOR ...], --
 author [AUTHOR ...] Media author i.e YouTube channel name - None -l LIMIT, --
 limit LIMIT Total videos to be downloaded - 1 -d PATH, --dir PATH Directory for
-saving the contents - /data/data/com.termux/files/home -t TIMEOUT, --timeout
-TIMEOUT Http request timeout in seconds - 30 -c CHUNK, --chunk CHUNK Chunk-size
-for downloading files in KB - 256 -i PATH, --input PATH Path to text file
-containing query per line - None -o FORMAT, --output FORMAT Format for
+saving the contents - /storage/emulated/0/git/Smartwa /y2mate-api -t TIMEOUT, -
+-timeout TIMEOUT Http request timeout in seconds - 30 -c CHUNK, --chunk CHUNK
+Chunk-size for downloading files in KB - 256 -i PATH, --input PATH Path to text
+file containing query per line - None -o FORMAT, --output FORMAT Format for
 generating filename %(key)s : [title,vid,fquality,ftype] or 'pretty' - None -
 thr THREAD, --thread THREAD Download [x] amount of videos/audios at once - 1 --
-disable-bar Disable download progress bar - False --ask Confirm before
+disable-bar Disable download progress bar - False --confirm Confirm before
 downloading file - False --unique Auto-skip any media that you once dowloaded -
 False --quiet Not to stdout anything other than logs - False --history Stdout
 all media metadata ever downloaded - False --clear Clear all download histories
-- False This script has no official relation with y2mate.com ```  - Review
-[CHANGELOG](https://github.com/Simatwa/y2mate-api/blob/main/Docs/CHANGELOG.md)
-for latest updates. ## Disclaimer This repository is intended for educational
-and personal use only. The use of this repository for any commercial or illegal
-purposes is strictly prohibited. The repository owner does not endorse or
-encourage the downloading or sharing of copyrighted material without
-permission. The repository owner is not responsible for any misuse of the
-software or any legal consequences that may arise from such misuse.
+- False --play Play media after download - False This script has no official
+relation with y2mate.com ```  - Review [CHANGELOG](https://github.com/Simatwa/
+y2mate-api/blob/main/Docs/CHANGELOG.md) for latest updates. ## Disclaimer This
+repository is intended for educational and personal use only. The use of this
+repository for any commercial or illegal purposes is strictly prohibited. The
+repository owner does not endorse or encourage the downloading or sharing of
+copyrighted material without permission. The repository owner is not
+responsible for any misuse of the software or any legal consequences that may
+arise from such misuse.
```

### Comparing `y2mate-api-0.0.8/README.md` & `y2mate-api-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <h1 align="center">y2mate-api</h1>
 
 <p align="center">
-<a href="https://github.com/Simatwa/y2mate-api"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a>
+<a href="https://github.com/Simatwa/y2mate-api/actions/workflows/python-test.yml"><img src="https://github.com/Simatwa/y2mate-api/actions/workflows/python-test.yml/badge.svg" alt="Python Test"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.8&color=green"/></a>
+<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.9&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/y2mate-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
 </p>
 
@@ -124,15 +124,15 @@
 **Note** : You can still use  **video id** such as `POPoAjWFkGg` as query parameter.
 
 ## Other parameters
 
 - `Handler`
   * author : Video author i.e Youtube Channel
   * timeout : http requests timeout
-  * ask : Confirm before downloading media
+  * confirm : Confirm before downloading media
   * unique : Auto-ignore previously downloaded media
   * thread : Download (x) value of file at a time.
 
 - `Handler.run`
   * format : Media format mp4/mp3
   * quality : Media quality such as 720p/128kbps
   * resolver : Additional format info : [m4a,3gp,mp4,mp3]
@@ -148,32 +148,33 @@
 - `Handler.save`
   * third_dict : Response of `third_query.run()`
   * dir : Directory for saving the contents
   * progress_bar : Display download progress bar
   * quiet : Not to stdout anything
   * naming_format : Format for generating media filename using the `third_query` response keys
   * chunk_size : Size of chunks in KB for downloads
- 
+  * play : Auto-play media after downloading 
 </details>
  
 <details>
 <summary>
 	
 For more info run `$ y2mate -h`
 
 </summary>
 
 ```
 usage: y2mate [-h] [-v] [-f mp3|mp4]
               [-q 4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
               [-r m4a|3gp|mp4|mp3] [-k [KEYWORD ...]]
               [-a [AUTHOR ...]] [-l LIMIT] [-d PATH]
-              [-t TIMEOUT] [-c CHUNK] [-i PATH] [-o FORMAT]
-              [-thr THREAD] [--disable-bar] [--ask]
-              [--unique] [--quiet] [--history] [--clear]
+              [-t TIMEOUT] [-c CHUNK] [-i PATH]
+              [-o FORMAT] [-thr THREAD] [--disable-bar]
+              [--confirm] [--unique] [--quiet]
+              [--history] [--clear] [--play]
               [query ...]
 
 Download youtube videos and audios by title or link
 
 positional arguments:
   query                 Youtube video title, link or id -
                         None
@@ -186,49 +187,54 @@
                         Specify media type - audio/video
   -q 4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps, --quality 4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps
                         Media quality - auto
   -r m4a|3gp|mp4|mp3, --resolver m4a|3gp|mp4|mp3
                         Other media formats incase of
                         multiple options - mp4/mp3
   -k [KEYWORD ...], --keyword [KEYWORD ...]
-                        Media should contain this keywords -
-                        None
+                        Media should contain this
+                        keywords - None
   -a [AUTHOR ...], --author [AUTHOR ...]
                         Media author i.e YouTube channel
                         name - None
   -l LIMIT, --limit LIMIT
                         Total videos to be downloaded - 1
-  -d PATH, --dir PATH   Directory for saving the contents -
-                        /data/data/com.termux/files/home
+  -d PATH, --dir PATH   Directory for saving the contents
+                        - /storage/emulated/0/git/Smartwa
+                        /y2mate-api
   -t TIMEOUT, --timeout TIMEOUT
-                        Http request timeout in seconds - 30
+                        Http request timeout in seconds -
+                        30
   -c CHUNK, --chunk CHUNK
-                        Chunk-size for downloading files in
-                        KB - 256
+                        Chunk-size for downloading files
+                        in KB - 256
   -i PATH, --input PATH
-                        Path to text file containing query
-                        per line - None
+                        Path to text file containing
+                        query per line - None
   -o FORMAT, --output FORMAT
                         Format for generating filename
-                        %(key)s : [title,vid,fquality,ftype]
-                        or 'pretty' - None
+                        %(key)s :
+                        [title,vid,fquality,ftype] or
+                        'pretty' - None
   -thr THREAD, --thread THREAD
-                        Download [x] amount of videos/audios
-                        at once - 1
+                        Download [x] amount of
+                        videos/audios at once - 1
   --disable-bar         Disable download progress bar -
                         False
-  --ask                 Confirm before downloading file -
+  --confirm             Confirm before downloading file -
                         False
   --unique              Auto-skip any media that you once
                         dowloaded - False
   --quiet               Not to stdout anything other than
                         logs - False
   --history             Stdout all media metadata ever
                         downloaded - False
-  --clear               Clear all download histories - False
+  --clear               Clear all download histories -
+                        False
+  --play                Play media after download - False
 
 This script has no official relation with y2mate.com
 ```
 </details>
 
 - Review [CHANGELOG](https://github.com/Simatwa/y2mate-api/blob/main/Docs/CHANGELOG.md) for latest updates.
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
                            ****** y2mate-api ******
- [Github] [License] [PyPi] [Black] [Passing] [coverage] [Progress] [Downloads]
+    [Python_Test] [License] [PyPi] [Black] [Passing] [coverage] [Progress]
+                                  [Downloads]
 > Download youtube videos and audios by **title/id/url** # Installation -
 Either of the following ways will get you ready. 1. Pip a. From source ```sh
 pip install git+https://github.com/Simatwa/y2mate-api.git ``` b. From pypi
 ```sh pip install y2mate-api ``` 2. Locally ```sh git clone https://github.com/
 Simatwa/y2mate-api.git cd y2mate-api pip install . ``` # Usage `$ y2mate -f
 p4> `   Developer docs  1.Generate download links and other metadata - Video
 ```py from y2mate_api import Handler api = Handler("Quantum computing in
@@ -37,57 +38,59 @@
 download the first video found and save it in the `current directory` You can
 as well specify total videos to be downloaded by using `limit` argument. For
 instance: ```py from y2mate_api import Handler api = Handler("https://youtu.be/
 POPoAjWFkGg") api.auto_save(limit=10) # This will download the video in path
 and 9 other videos related to the query specified ``` **Note** : You can still
 use **video id** such as `POPoAjWFkGg` as query parameter. ## Other parameters
 - `Handler` * author : Video author i.e Youtube Channel * timeout : http
-requests timeout * ask : Confirm before downloading media * unique : Auto-
+requests timeout * confirm : Confirm before downloading media * unique : Auto-
 ignore previously downloaded media * thread : Download (x) value of file at a
 time. - `Handler.run` * format : Media format mp4/mp3 * quality : Media quality
 such as 720p/128kbps * resolver : Additional format info : [m4a,3gp,mp4,mp3] *
 limit : Total videos to be retrieved * keyword : Phrase(s) that must be in
 media title * author : Video author i.e Youtube Channel - `Handler.auto_save` *
 dir : Path to Directory for saving the media files * iterator : Function that
 yields third_query object - `Handler.run` * progress_bar : Stdout media-name &
 Display progress bar - `Handler.save` * third_dict : Response of
 `third_query.run()` * dir : Directory for saving the contents * progress_bar :
 Display download progress bar * quiet : Not to stdout anything * naming_format
 : Format for generating media filename using the `third_query` response keys *
-chunk_size : Size of chunks in KB for downloads    For more info run `$ y2mate
--h`  ``` usage: y2mate [-h] [-v] [-f mp3|mp4] [-
+chunk_size : Size of chunks in KB for downloads * play : Auto-play media after
+downloading    For more info run `$ y2mate -h`  ``` usage: y2mate [-h] [-v] [-
+f mp3|mp4] [-
 q
 4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
 [-r m4a|3gp|mp4|mp3] [-k [KEYWORD ...]] [-a [AUTHOR ...]] [-l LIMIT] [-d PATH]
 [-t TIMEOUT] [-c CHUNK] [-i PATH] [-o FORMAT] [-thr THREAD] [--disable-bar] [--
-ask] [--unique] [--quiet] [--history] [--clear] [query ...] Download youtube
-videos and audios by title or link positional arguments: query Youtube video
-title, link or id - None options: -h, --help show this help message and exit -
-v, --version show program's version number and exit -f mp3|mp4, --format
-mp3|mp4 Specify media type - audio/video -
+confirm] [--unique] [--quiet] [--history] [--clear] [--play] [query ...]
+Download youtube videos and audios by title or link positional arguments: query
+Youtube video title, link or id - None options: -h, --help show this help
+message and exit -v, --version show program's version number and exit -
+f mp3|mp4, --format mp3|mp4 Specify media type - audio/video -
 q
 4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps,
 --quality
 4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps
 Media quality - auto -r m4a|3gp|mp4|mp3, --resolver m4a|3gp|mp4|mp3 Other media
 formats incase of multiple options - mp4/mp3 -k [KEYWORD ...], --keyword
 [KEYWORD ...] Media should contain this keywords - None -a [AUTHOR ...], --
 author [AUTHOR ...] Media author i.e YouTube channel name - None -l LIMIT, --
 limit LIMIT Total videos to be downloaded - 1 -d PATH, --dir PATH Directory for
-saving the contents - /data/data/com.termux/files/home -t TIMEOUT, --timeout
-TIMEOUT Http request timeout in seconds - 30 -c CHUNK, --chunk CHUNK Chunk-size
-for downloading files in KB - 256 -i PATH, --input PATH Path to text file
-containing query per line - None -o FORMAT, --output FORMAT Format for
+saving the contents - /storage/emulated/0/git/Smartwa /y2mate-api -t TIMEOUT, -
+-timeout TIMEOUT Http request timeout in seconds - 30 -c CHUNK, --chunk CHUNK
+Chunk-size for downloading files in KB - 256 -i PATH, --input PATH Path to text
+file containing query per line - None -o FORMAT, --output FORMAT Format for
 generating filename %(key)s : [title,vid,fquality,ftype] or 'pretty' - None -
 thr THREAD, --thread THREAD Download [x] amount of videos/audios at once - 1 --
-disable-bar Disable download progress bar - False --ask Confirm before
+disable-bar Disable download progress bar - False --confirm Confirm before
 downloading file - False --unique Auto-skip any media that you once dowloaded -
 False --quiet Not to stdout anything other than logs - False --history Stdout
 all media metadata ever downloaded - False --clear Clear all download histories
-- False This script has no official relation with y2mate.com ```  - Review
-[CHANGELOG](https://github.com/Simatwa/y2mate-api/blob/main/Docs/CHANGELOG.md)
-for latest updates. ## Disclaimer This repository is intended for educational
-and personal use only. The use of this repository for any commercial or illegal
-purposes is strictly prohibited. The repository owner does not endorse or
-encourage the downloading or sharing of copyrighted material without
-permission. The repository owner is not responsible for any misuse of the
-software or any legal consequences that may arise from such misuse.
+- False --play Play media after download - False This script has no official
+relation with y2mate.com ```  - Review [CHANGELOG](https://github.com/Simatwa/
+y2mate-api/blob/main/Docs/CHANGELOG.md) for latest updates. ## Disclaimer This
+repository is intended for educational and personal use only. The use of this
+repository for any commercial or illegal purposes is strictly prohibited. The
+repository owner does not endorse or encourage the downloading or sharing of
+copyrighted material without permission. The repository owner is not
+responsible for any misuse of the software or any legal consequences that may
+arise from such misuse.
```

### Comparing `y2mate-api-0.0.8/setup.py` & `y2mate-api-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.0.8"
+version = "0.0.9"
 info = "Download youtube videos and audios by title or link"
 author = "Smartwa"
 repo = "https://github.com/Simatwa/y2mate-api"
 
 setup(
     name="y2mate-api",
     packages=["y2mate_api"],
@@ -13,20 +13,21 @@
     author=author,
     maintainer=author,
     author_email="smartwacaleb@gmail.com",
     description=info,
     url=repo,
     project_urls={"Bug Report": f"{repo}/issues/new"},
     install_requires=[
-        "argparse>=1.1",
-        "requests>=2.0.2",
-        "tqdm==4.65.0",
-        "colorama==0.4.6",
-        "appdirs==1.4.4",
-        "getch==1.0",
+    "argparse>=1.1",
+    "tqdm==4.65.0",
+    "requests==2.28.2",
+    "colorama==0.4.6",
+    "appdirs==1.4.4",
+    "getch==1.0",
+    "click==8.1.3",
     ],
     python_requires=">=3.8",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Development Status :: 4 - Beta",
```

### Comparing `y2mate-api-0.0.8/tests/test_download.py` & `y2mate-api-0.0.9/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `y2mate-api-0.0.8/tests/test_queries.py` & `y2mate-api-0.0.9/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `y2mate-api-0.0.8/y2mate_api/console.py` & `y2mate-api-0.0.9/y2mate_api/console.py`

 * *Files 5% similar despite different names*

```diff
@@ -121,15 +121,15 @@
     )
     parser.add_argument(
         "--disable-bar",
         help="Disable download progress bar - %(default)s",
         action="store_true",
     )
     parser.add_argument(
-        "--ask",
+        "--confirm",
         help="Confirm before downloading file - %(default)s",
         action="store_true",
     )
     parser.add_argument(
         "--unique",
         help="Auto-skip any media that you once dowloaded - %(default)s",
         action="store_true",
@@ -145,14 +145,17 @@
         action="store_true",
     )
     parser.add_argument(
         "--clear",
         help="Clear all download histories - %(default)s",
         action="store_true",
     )
+    parser.add_argument(
+        "--play", help="Play media after download - %(default)s", action="store_true"
+    )
     return parser.parse_args()
 
 
 @utils.error_handler(exit_on_error=True)
 def main():
     args = get_args()
     from . import Handler
@@ -167,26 +170,27 @@
     if not args.format:
         raise Exception("You must specify media format [ -f mp3/4]")
     h_mult_args = lambda v: v if not v else " ".join(v)
     handler_init_args = dict(
         query=h_mult_args(args.query),
         author=args.author,
         timeout=args.timeout,
-        ask=args.ask,
+        confirm=args.confirm,
         unique=args.unique,
         thread=args.thread,
     )
     auto_save_args = dict(
         dir=args.dir,
         progress_bar=args.disable_bar == False,
         quiet=args.quiet,
         naming_format=f"%(title)s{' - %(fquality)s' if args.format=='mp4' else ''}.%(ftype)s"
         if str(args.output).lower() == "pretty"
         else args.output,
         chunk_size=args.chunk,
+        play=args.play,
         format=args.format,
         quality=args.quality,
         resolver=args.resolver,
         limit=args.limit,
         keyword=h_mult_args(args.keyword),
         author=h_mult_args(args.author),
     )
```

### Comparing `y2mate-api-0.0.8/y2mate_api/downloader.py` & `y2mate-api-0.0.9/y2mate_api/downloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .main import requests, logging, utils, first_query, second_query, third_query
 from tqdm import tqdm
 from colorama import Fore
 from os import path, getcwd
 from threading import Thread
 from getch import getch
 from sys import stdout
+from click import launch as launch_media
 
 """
 - query string
 - format mp4/3
 - quality 720p/128kbps
 - keywords
 - Specify video author
@@ -22,37 +23,37 @@
 
 class Handler:
     def __init__(
         self,
         query: str,
         author: str = None,
         timeout: int = 30,
-        ask: bool = False,
+        confirm: bool = False,
         unique: bool = False,
         thread: int = 0,
     ):
         r"""Initializes this `class`
         :param query: Video name or youtube link
         :type query: str
         :param author: (Optional) Author (Channel) of the videos
         :type author: str
         :param timeout: (Optional) Http request timeout
         :type timeout: int
-        :param ask: (Optional) Confirm before downloading media
-        :type ask: bool
+        :param confirm: (Optional) Confirm before downloading media
+        :type confirm: bool
         :param unique: (Optional) Ignore previously downloaded media
-        :type ask: bool
+        :type confirm: bool
         :param thread: (Optional) Thread the download process through `auto-save` method
         :type thread int
         """
         self.query = query
         self.author = author
         self.timeout = timeout
         self.keyword = None
-        self.ask = ask
+        self.confirm = confirm
         self.unique = unique
         self.thread = thread
         self.vitems = []
         self.related = []
         self.dropped = []
         self.total = 1
         self.saved_videos = utils.get_history()
@@ -99,23 +100,23 @@
         video_id = second_query_obj.vid
         video_author = second_query_obj.a
         video_title = second_query_obj.title
         confirm = lambda choice: True if choice.lower() in ("yes", "y") else False
         if video_id in self.saved_videos:
             if self.unique:
                 return False, "Duplicate"
-            if self.ask:
+            if self.confirm:
                 stdout.write(
                     f">> Re-download : {Fore.GREEN+video_title+Fore.RESET} by {Fore.YELLOW+video_author+Fore.RESET} - [y/N]? :"
                 )
                 stdout.flush()
                 choice = getch()
                 print("\n[*] Ok processing...", end="\r")
                 return confirm(choice), "User's choice"
-        if self.ask:
+        if self.confirm:
             stdout.write(
                 f">> Download : {Fore.GREEN+video_title+Fore.RESET} by {Fore.YELLOW+video_author+Fore.RESET} - [Y/n]? :"
             )
             stdout.flush()
             choice = getch()
             print("\n[*] Ok processing...", end="\r")
             return confirm(choice), "User's choice"
@@ -277,30 +278,33 @@
         self,
         dir: str = "",
         iterator: object = None,
         progress_bar=True,
         quiet: bool = False,
         naming_format: str = None,
         chunk_size: int = 512,
+        play: bool = False,
         *args,
         **kwargs,
     ):
         r"""Query and save all the media
         :param dir: (Optional) Path to Directory for saving the media files
         :param iterator: (Optional) Function that yields third_query object - `Handler.run`
         :param progress_bar: (Optional) Display progress bar
         :param quiet: (Optional) Not to stdout anything
         :param naming_format: (Optional) Format for generating filename
         :param chunk_size: (Optional) Chunk_size for downloading files in KB
+        :param play: (Optional) Auto-play the media after download
         :type dir: str
         :type iterator: object
         :type progress_bar: bool
         :type quiet: bool
         :type naming_format: str
         :type chunk_size: int
+        :type play: bool
         args & kwargs for the iterator
         :rtype: None
         """
         iterator_object = iterator or self.run(*args, **kwargs)
 
         for x, entry in enumerate(iterator_object):
 
@@ -310,48 +314,54 @@
                     args=(
                         entry,
                         dir,
                         False,
                         quiet,
                         naming_format,
                         chunk_size,
+                        play,
                     ),
                 )
                 t1.start()
                 thread_count = x + 1
                 if thread_count % self.thread == 0 or thread_count == self.total:
                     logging.debug(
                         f"Waiting for current running threads to finish - thread_count : {thread_count}"
                     )
                     t1.join()
             else:
-                self.save(entry, dir, progress_bar, quiet, naming_format, chunk_size)
+                self.save(
+                    entry, dir, progress_bar, quiet, naming_format, chunk_size, play
+                )
 
     def save(
         self,
         third_dict: dict,
         dir: str = "",
         progress_bar=True,
         quiet: bool = False,
         naming_format: str = None,
         chunk_size: int = 512,
+        play: bool = False,
     ):
         r"""Download media based on response of `third_query` dict-data-type
         :param third_dict: Response of `third_query.run()`
         :param dir: (Optional) Directory for saving the contents
         :param progress_bar: (Optional) Display download progress bar
         :param quiet: (Optional) Not to stdout anything
         :param naming_format: (Optional) Format for generating filename
         :param chunk_size: (Optional) Chunk_size for downloading files in KB
+        :param play: (Optional) Auto-play the media after download
         :type third_dict: dict
         :type dir: str
         :type progress_bar: bool
         :type quiet: bool
         :type naming_format: str
         :type chunk_size: int
+        :type play: bool
         :rtype: None
         """
         if third_dict:
             assert third_dict.get(
                 "dlink"
             ), "The video selected does not support that quality, try lower qualities."
             if third_dict.get("mess"):
@@ -364,30 +374,33 @@
             save_to = path.join(dir, filename)
 
             third_dict["saved_to"] = (
                 save_to
                 if any([save_to.startswith("/"), ":" in save_to])
                 else path.join(getcwd(), dir, filename)
             )
+            try_play_media = lambda: launch_media(third_dict["saved_to"]) if play else None
             if progress_bar:
                 if not quiet:
                     print(f"{filename}")
                 with tqdm(
                     total=size_in_bytes,
                     bar_format="%s%d MB %s{bar} %s{l_bar}%s"
                     % (Fore.GREEN, size_in_mb, Fore.CYAN, Fore.YELLOW, Fore.RESET),
                 ) as p_bar:
                     with open(save_to, "wb") as fh:
                         for chunks in resp.iter_content(chunk_size=chunk_size_in_bytes):
                             fh.write(chunks)
                             p_bar.update(chunk_size_in_bytes)
                     utils.add_history(third_dict)
+                    try_play_media()
                     return save_to
             else:
                 with open(save_to, "wb") as fh:
                     for chunks in resp.iter_content(chunk_size=chunk_size_in_bytes):
                         fh.write(chunks)
                 utils.add_history(third_dict)
+                try_play_media()
                 logging.info(f"{filename} - {size_in_mb}MB ✅")
                 return save_to
         else:
             logging.error(f"Empty `third_dict` parameter parsed : {third_dict}")
```

### Comparing `y2mate-api-0.0.8/y2mate_api/main.py` & `y2mate-api-0.0.9/y2mate_api/main.py`

 * *Files identical despite different names*

### Comparing `y2mate-api-0.0.8/y2mate_api.egg-info/PKG-INFO` & `y2mate-api-0.0.9/y2mate_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: y2mate-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: Download youtube videos and audios by title or link
 Home-page: https://github.com/Simatwa/y2mate-api
 Author: Smartwa
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/y2mate-api/issues/new
@@ -25,17 +25,17 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">y2mate-api</h1>
 
 <p align="center">
-<a href="https://github.com/Simatwa/y2mate-api"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a>
+<a href="https://github.com/Simatwa/y2mate-api/actions/workflows/python-test.yml"><img src="https://github.com/Simatwa/y2mate-api/actions/workflows/python-test.yml/badge.svg" alt="Python Test"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.8&color=green"/></a>
+<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.9&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/y2mate-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
 </p>
 
@@ -152,15 +152,15 @@
 **Note** : You can still use  **video id** such as `POPoAjWFkGg` as query parameter.
 
 ## Other parameters
 
 - `Handler`
   * author : Video author i.e Youtube Channel
   * timeout : http requests timeout
-  * ask : Confirm before downloading media
+  * confirm : Confirm before downloading media
   * unique : Auto-ignore previously downloaded media
   * thread : Download (x) value of file at a time.
 
 - `Handler.run`
   * format : Media format mp4/mp3
   * quality : Media quality such as 720p/128kbps
   * resolver : Additional format info : [m4a,3gp,mp4,mp3]
@@ -176,32 +176,33 @@
 - `Handler.save`
   * third_dict : Response of `third_query.run()`
   * dir : Directory for saving the contents
   * progress_bar : Display download progress bar
   * quiet : Not to stdout anything
   * naming_format : Format for generating media filename using the `third_query` response keys
   * chunk_size : Size of chunks in KB for downloads
- 
+  * play : Auto-play media after downloading 
 </details>
  
 <details>
 <summary>
 	
 For more info run `$ y2mate -h`
 
 </summary>
 
 ```
 usage: y2mate [-h] [-v] [-f mp3|mp4]
               [-q 4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
               [-r m4a|3gp|mp4|mp3] [-k [KEYWORD ...]]
               [-a [AUTHOR ...]] [-l LIMIT] [-d PATH]
-              [-t TIMEOUT] [-c CHUNK] [-i PATH] [-o FORMAT]
-              [-thr THREAD] [--disable-bar] [--ask]
-              [--unique] [--quiet] [--history] [--clear]
+              [-t TIMEOUT] [-c CHUNK] [-i PATH]
+              [-o FORMAT] [-thr THREAD] [--disable-bar]
+              [--confirm] [--unique] [--quiet]
+              [--history] [--clear] [--play]
               [query ...]
 
 Download youtube videos and audios by title or link
 
 positional arguments:
   query                 Youtube video title, link or id -
                         None
@@ -214,49 +215,54 @@
                         Specify media type - audio/video
   -q 4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps, --quality 4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps
                         Media quality - auto
   -r m4a|3gp|mp4|mp3, --resolver m4a|3gp|mp4|mp3
                         Other media formats incase of
                         multiple options - mp4/mp3
   -k [KEYWORD ...], --keyword [KEYWORD ...]
-                        Media should contain this keywords -
-                        None
+                        Media should contain this
+                        keywords - None
   -a [AUTHOR ...], --author [AUTHOR ...]
                         Media author i.e YouTube channel
                         name - None
   -l LIMIT, --limit LIMIT
                         Total videos to be downloaded - 1
-  -d PATH, --dir PATH   Directory for saving the contents -
-                        /data/data/com.termux/files/home
+  -d PATH, --dir PATH   Directory for saving the contents
+                        - /storage/emulated/0/git/Smartwa
+                        /y2mate-api
   -t TIMEOUT, --timeout TIMEOUT
-                        Http request timeout in seconds - 30
+                        Http request timeout in seconds -
+                        30
   -c CHUNK, --chunk CHUNK
-                        Chunk-size for downloading files in
-                        KB - 256
+                        Chunk-size for downloading files
+                        in KB - 256
   -i PATH, --input PATH
-                        Path to text file containing query
-                        per line - None
+                        Path to text file containing
+                        query per line - None
   -o FORMAT, --output FORMAT
                         Format for generating filename
-                        %(key)s : [title,vid,fquality,ftype]
-                        or 'pretty' - None
+                        %(key)s :
+                        [title,vid,fquality,ftype] or
+                        'pretty' - None
   -thr THREAD, --thread THREAD
-                        Download [x] amount of videos/audios
-                        at once - 1
+                        Download [x] amount of
+                        videos/audios at once - 1
   --disable-bar         Disable download progress bar -
                         False
-  --ask                 Confirm before downloading file -
+  --confirm             Confirm before downloading file -
                         False
   --unique              Auto-skip any media that you once
                         dowloaded - False
   --quiet               Not to stdout anything other than
                         logs - False
   --history             Stdout all media metadata ever
                         downloaded - False
-  --clear               Clear all download histories - False
+  --clear               Clear all download histories -
+                        False
+  --play                Play media after download - False
 
 This script has no official relation with y2mate.com
 ```
 </details>
 
 - Review [CHANGELOG](https://github.com/Simatwa/y2mate-api/blob/main/Docs/CHANGELOG.md) for latest updates.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.8 Summary: Download youtube
+Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.9 Summary: Download youtube
 videos and audios by title or link Home-page: https://github.com/Simatwa/
 y2mate-api Author: Smartwa Author-email: smartwacaleb@gmail.com Maintainer:
 Smartwa License: MIT Project-URL: Bug Report, https://github.com/Simatwa/
 y2mate-api/issues/new Keywords: y2mate,videos,video-api,youtube Classifier:
 License :: OSI Approved :: MIT License Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: Free For Home Use Classifier: Intended
@@ -10,15 +10,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE
                            ****** y2mate-api ******
- [Github] [License] [PyPi] [Black] [Passing] [coverage] [Progress] [Downloads]
+    [Python_Test] [License] [PyPi] [Black] [Passing] [coverage] [Progress]
+                                  [Downloads]
 > Download youtube videos and audios by **title/id/url** # Installation -
 Either of the following ways will get you ready. 1. Pip a. From source ```sh
 pip install git+https://github.com/Simatwa/y2mate-api.git ``` b. From pypi
 ```sh pip install y2mate-api ``` 2. Locally ```sh git clone https://github.com/
 Simatwa/y2mate-api.git cd y2mate-api pip install . ``` # Usage `$ y2mate -f
 p4> `   Developer docs  1.Generate download links and other metadata - Video
 ```py from y2mate_api import Handler api = Handler("Quantum computing in
@@ -52,57 +53,59 @@
 download the first video found and save it in the `current directory` You can
 as well specify total videos to be downloaded by using `limit` argument. For
 instance: ```py from y2mate_api import Handler api = Handler("https://youtu.be/
 POPoAjWFkGg") api.auto_save(limit=10) # This will download the video in path
 and 9 other videos related to the query specified ``` **Note** : You can still
 use **video id** such as `POPoAjWFkGg` as query parameter. ## Other parameters
 - `Handler` * author : Video author i.e Youtube Channel * timeout : http
-requests timeout * ask : Confirm before downloading media * unique : Auto-
+requests timeout * confirm : Confirm before downloading media * unique : Auto-
 ignore previously downloaded media * thread : Download (x) value of file at a
 time. - `Handler.run` * format : Media format mp4/mp3 * quality : Media quality
 such as 720p/128kbps * resolver : Additional format info : [m4a,3gp,mp4,mp3] *
 limit : Total videos to be retrieved * keyword : Phrase(s) that must be in
 media title * author : Video author i.e Youtube Channel - `Handler.auto_save` *
 dir : Path to Directory for saving the media files * iterator : Function that
 yields third_query object - `Handler.run` * progress_bar : Stdout media-name &
 Display progress bar - `Handler.save` * third_dict : Response of
 `third_query.run()` * dir : Directory for saving the contents * progress_bar :
 Display download progress bar * quiet : Not to stdout anything * naming_format
 : Format for generating media filename using the `third_query` response keys *
-chunk_size : Size of chunks in KB for downloads    For more info run `$ y2mate
--h`  ``` usage: y2mate [-h] [-v] [-f mp3|mp4] [-
+chunk_size : Size of chunks in KB for downloads * play : Auto-play media after
+downloading    For more info run `$ y2mate -h`  ``` usage: y2mate [-h] [-v] [-
+f mp3|mp4] [-
 q
 4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
 [-r m4a|3gp|mp4|mp3] [-k [KEYWORD ...]] [-a [AUTHOR ...]] [-l LIMIT] [-d PATH]
 [-t TIMEOUT] [-c CHUNK] [-i PATH] [-o FORMAT] [-thr THREAD] [--disable-bar] [--
-ask] [--unique] [--quiet] [--history] [--clear] [query ...] Download youtube
-videos and audios by title or link positional arguments: query Youtube video
-title, link or id - None options: -h, --help show this help message and exit -
-v, --version show program's version number and exit -f mp3|mp4, --format
-mp3|mp4 Specify media type - audio/video -
+confirm] [--unique] [--quiet] [--history] [--clear] [--play] [query ...]
+Download youtube videos and audios by title or link positional arguments: query
+Youtube video title, link or id - None options: -h, --help show this help
+message and exit -v, --version show program's version number and exit -
+f mp3|mp4, --format mp3|mp4 Specify media type - audio/video -
 q
 4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps,
 --quality
 4k|1080p|720p|480p|360p|240p|144p|auto|best|worst|mp3|m4a|.m4a|128kbps|192kbps|328kbps
 Media quality - auto -r m4a|3gp|mp4|mp3, --resolver m4a|3gp|mp4|mp3 Other media
 formats incase of multiple options - mp4/mp3 -k [KEYWORD ...], --keyword
 [KEYWORD ...] Media should contain this keywords - None -a [AUTHOR ...], --
 author [AUTHOR ...] Media author i.e YouTube channel name - None -l LIMIT, --
 limit LIMIT Total videos to be downloaded - 1 -d PATH, --dir PATH Directory for
-saving the contents - /data/data/com.termux/files/home -t TIMEOUT, --timeout
-TIMEOUT Http request timeout in seconds - 30 -c CHUNK, --chunk CHUNK Chunk-size
-for downloading files in KB - 256 -i PATH, --input PATH Path to text file
-containing query per line - None -o FORMAT, --output FORMAT Format for
+saving the contents - /storage/emulated/0/git/Smartwa /y2mate-api -t TIMEOUT, -
+-timeout TIMEOUT Http request timeout in seconds - 30 -c CHUNK, --chunk CHUNK
+Chunk-size for downloading files in KB - 256 -i PATH, --input PATH Path to text
+file containing query per line - None -o FORMAT, --output FORMAT Format for
 generating filename %(key)s : [title,vid,fquality,ftype] or 'pretty' - None -
 thr THREAD, --thread THREAD Download [x] amount of videos/audios at once - 1 --
-disable-bar Disable download progress bar - False --ask Confirm before
+disable-bar Disable download progress bar - False --confirm Confirm before
 downloading file - False --unique Auto-skip any media that you once dowloaded -
 False --quiet Not to stdout anything other than logs - False --history Stdout
 all media metadata ever downloaded - False --clear Clear all download histories
-- False This script has no official relation with y2mate.com ```  - Review
-[CHANGELOG](https://github.com/Simatwa/y2mate-api/blob/main/Docs/CHANGELOG.md)
-for latest updates. ## Disclaimer This repository is intended for educational
-and personal use only. The use of this repository for any commercial or illegal
-purposes is strictly prohibited. The repository owner does not endorse or
-encourage the downloading or sharing of copyrighted material without
-permission. The repository owner is not responsible for any misuse of the
-software or any legal consequences that may arise from such misuse.
+- False --play Play media after download - False This script has no official
+relation with y2mate.com ```  - Review [CHANGELOG](https://github.com/Simatwa/
+y2mate-api/blob/main/Docs/CHANGELOG.md) for latest updates. ## Disclaimer This
+repository is intended for educational and personal use only. The use of this
+repository for any commercial or illegal purposes is strictly prohibited. The
+repository owner does not endorse or encourage the downloading or sharing of
+copyrighted material without permission. The repository owner is not
+responsible for any misuse of the software or any legal consequences that may
+arise from such misuse.
```

