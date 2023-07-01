# Comparing `tmp/deezer_downloader-2.0.4.tar.gz` & `tmp/deezer_downloader-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deezer_downloader-2.0.4.tar", max compression
+gzip compressed data, was "deezer_downloader-2.0.5.tar", max compression
```

## Comparing `deezer_downloader-2.0.4.tar` & `deezer_downloader-2.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1063 2023-04-09 20:20:53.021110 deezer_downloader-2.0.4/LICENSE
--rw-r--r--   0        0        0     7743 2023-04-29 16:28:37.070565 deezer_downloader-2.0.4/README.md
--rw-r--r--   0        0        0     1422 2023-04-10 17:50:53.352272 deezer_downloader-2.0.4/deezer_downloader/cli/deezer-downloader.ini.template
--rw-r--r--   0        0        0     1738 2023-04-09 20:56:59.983157 deezer_downloader-2.0.4/deezer_downloader/cli/runner.py
--rw-r--r--   0        0        0     1497 2023-05-01 07:47:26.683606 deezer_downloader-2.0.4/deezer_downloader/configuration.py
--rw-r--r--   0        0        0    20834 2023-04-10 17:48:00.685645 deezer_downloader-2.0.4/deezer_downloader/deezer.py
--rw-r--r--   0        0        0     5031 2023-04-29 16:38:19.755822 deezer_downloader-2.0.4/deezer_downloader/spotify.py
--rw-r--r--   0        0        0     3382 2023-04-09 20:20:53.021110 deezer_downloader-2.0.4/deezer_downloader/threadpool_queue.py
--rw-r--r--   0        0        0    10201 2023-04-10 17:34:44.980270 deezer_downloader-2.0.4/deezer_downloader/web/app.py
--rw-r--r--   0        0        0    11048 2023-04-29 16:16:41.814433 deezer_downloader-2.0.4/deezer_downloader/web/music_backend.py
--rw-r--r--   0        0        0   623500 2023-04-09 20:20:53.024443 deezer_downloader-2.0.4/deezer_downloader/web/static/css/bootstrap-4.1.3-dist.zip
--rw-r--r--   0        0        0    70682 2023-04-09 20:20:53.024443 deezer_downloader-2.0.4/deezer_downloader/web/static/css/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   155758 2023-04-09 20:20:53.024443 deezer_downloader-2.0.4/deezer_downloader/web/static/css/bootstrap.min.css
--rw-r--r--   0        0        0    31000 2023-04-09 20:20:53.024443 deezer_downloader-2.0.4/deezer_downloader/web/static/css/font-awesome.min.css
--rw-r--r--   0        0        0     1515 2023-04-09 20:20:53.024443 deezer_downloader-2.0.4/deezer_downloader/web/static/css/jquery.jgrowl.min.css
--rw-r--r--   0        0        0      327 2023-04-09 20:20:53.024443 deezer_downloader-2.0.4/deezer_downloader/web/static/favicon.ico
--rw-r--r--   0        0        0    77160 2023-04-09 20:20:53.024443 deezer_downloader-2.0.4/deezer_downloader/web/static/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0    58072 2023-04-09 20:20:53.024443 deezer_downloader-2.0.4/deezer_downloader/web/static/js/bootstrap.min.js
--rw-r--r--   0        0        0    11064 2023-04-09 20:20:53.027777 deezer_downloader-2.0.4/deezer_downloader/web/static/js/custom.js
--rw-r--r--   0        0        0     5476 2023-04-09 20:20:53.027777 deezer_downloader-2.0.4/deezer_downloader/web/static/js/jquery.jgrowl.min.js
--rw-r--r--   0        0        0    89795 2023-04-09 20:20:53.027777 deezer_downloader-2.0.4/deezer_downloader/web/static/js/jquery.min.js
--rw-r--r--   0        0        0    21004 2023-04-09 20:20:53.027777 deezer_downloader-2.0.4/deezer_downloader/web/static/js/popper.min.js
--rw-r--r--   0        0        0      194 2023-04-09 20:20:53.027777 deezer_downloader-2.0.4/deezer_downloader/web/templates/autoindex.html
--rw-r--r--   0        0        0     8735 2023-04-10 10:27:40.860066 deezer_downloader-2.0.4/deezer_downloader/web/templates/index.html
--rw-r--r--   0        0        0     2309 2023-04-29 15:45:57.946045 deezer_downloader-2.0.4/deezer_downloader/youtubedl.py
--rw-r--r--   0        0        0      977 2023-05-18 15:34:22.576711 deezer_downloader-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     8676 1970-01-01 00:00:00.000000 deezer_downloader-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-09 20:20:53.021110 deezer_downloader-2.0.5/LICENSE
+-rw-r--r--   0        0        0     7743 2023-04-29 16:28:37.070565 deezer_downloader-2.0.5/README.md
+-rw-r--r--   0        0        0     1422 2023-04-10 17:50:53.352272 deezer_downloader-2.0.5/deezer_downloader/cli/deezer-downloader.ini.template
+-rw-r--r--   0        0        0     1738 2023-04-09 20:56:59.983157 deezer_downloader-2.0.5/deezer_downloader/cli/runner.py
+-rw-r--r--   0        0        0     1497 2023-05-01 07:47:26.683606 deezer_downloader-2.0.5/deezer_downloader/configuration.py
+-rw-r--r--   0        0        0    20834 2023-04-10 17:48:00.685645 deezer_downloader-2.0.5/deezer_downloader/deezer.py
+-rw-r--r--   0        0        0     5031 2023-04-29 16:38:19.755822 deezer_downloader-2.0.5/deezer_downloader/spotify.py
+-rw-r--r--   0        0        0     3382 2023-04-09 20:20:53.021110 deezer_downloader-2.0.5/deezer_downloader/threadpool_queue.py
+-rw-r--r--   0        0        0    10201 2023-04-10 17:34:44.980270 deezer_downloader-2.0.5/deezer_downloader/web/app.py
+-rw-r--r--   0        0        0    11048 2023-04-29 16:16:41.814433 deezer_downloader-2.0.5/deezer_downloader/web/music_backend.py
+-rw-r--r--   0        0        0   623500 2023-04-09 20:20:53.024443 deezer_downloader-2.0.5/deezer_downloader/web/static/css/bootstrap-4.1.3-dist.zip
+-rw-r--r--   0        0        0    70682 2023-04-09 20:20:53.024443 deezer_downloader-2.0.5/deezer_downloader/web/static/css/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   155758 2023-04-09 20:20:53.024443 deezer_downloader-2.0.5/deezer_downloader/web/static/css/bootstrap.min.css
+-rw-r--r--   0        0        0    31000 2023-04-09 20:20:53.024443 deezer_downloader-2.0.5/deezer_downloader/web/static/css/font-awesome.min.css
+-rw-r--r--   0        0        0     1515 2023-04-09 20:20:53.024443 deezer_downloader-2.0.5/deezer_downloader/web/static/css/jquery.jgrowl.min.css
+-rw-r--r--   0        0        0      327 2023-04-09 20:20:53.024443 deezer_downloader-2.0.5/deezer_downloader/web/static/favicon.ico
+-rw-r--r--   0        0        0    77160 2023-04-09 20:20:53.024443 deezer_downloader-2.0.5/deezer_downloader/web/static/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0    58072 2023-04-09 20:20:53.024443 deezer_downloader-2.0.5/deezer_downloader/web/static/js/bootstrap.min.js
+-rw-r--r--   0        0        0    11064 2023-04-09 20:20:53.027777 deezer_downloader-2.0.5/deezer_downloader/web/static/js/custom.js
+-rw-r--r--   0        0        0     5476 2023-04-09 20:20:53.027777 deezer_downloader-2.0.5/deezer_downloader/web/static/js/jquery.jgrowl.min.js
+-rw-r--r--   0        0        0    89795 2023-04-09 20:20:53.027777 deezer_downloader-2.0.5/deezer_downloader/web/static/js/jquery.min.js
+-rw-r--r--   0        0        0    21004 2023-04-09 20:20:53.027777 deezer_downloader-2.0.5/deezer_downloader/web/static/js/popper.min.js
+-rw-r--r--   0        0        0      194 2023-04-09 20:20:53.027777 deezer_downloader-2.0.5/deezer_downloader/web/templates/autoindex.html
+-rw-r--r--   0        0        0     8735 2023-04-10 10:27:40.860066 deezer_downloader-2.0.5/deezer_downloader/web/templates/index.html
+-rw-r--r--   0        0        0     2309 2023-04-29 15:45:57.946045 deezer_downloader-2.0.5/deezer_downloader/youtubedl.py
+-rw-r--r--   0        0        0      977 2023-07-01 12:27:52.312761 deezer_downloader-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0     8676 1970-01-01 00:00:00.000000 deezer_downloader-2.0.5/PKG-INFO
```

### Comparing `deezer_downloader-2.0.4/LICENSE` & `deezer_downloader-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.4/README.md` & `deezer_downloader-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.4/deezer_downloader/cli/deezer-downloader.ini.template` & `deezer_downloader-2.0.5/deezer_downloader/cli/deezer-downloader.ini.template`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.4/deezer_downloader/cli/runner.py` & `deezer_downloader-2.0.5/deezer_downloader/cli/runner.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.4/deezer_downloader/configuration.py` & `deezer_downloader-2.0.5/deezer_downloader/configuration.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.4/deezer_downloader/deezer.py` & `deezer_downloader-2.0.5/deezer_downloader/deezer.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.4/deezer_downloader/spotify.py` & `deezer_downloader-2.0.5/deezer_downloader/spotify.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.4/deezer_downloader/threadpool_queue.py` & `deezer_downloader-2.0.5/deezer_downloader/threadpool_queue.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.4/deezer_downloader/web/app.py` & `deezer_downloader-2.0.5/deezer_downloader/web/app.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.4/deezer_downloader/web/music_backend.py` & `deezer_downloader-2.0.5/deezer_downloader/web/music_backend.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.4/deezer_downloader/web/static/css/bootstrap-4.1.3-dist.zip` & `deezer_downloader-2.0.5/deezer_downloader/web/static/css/bootstrap-4.1.3-dist.zip`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.4/deezer_downloader/web/static/css/bootstrap.bundle.min.js` & `deezer_downloader-2.0.5/deezer_downloader/web/static/css/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.4/deezer_downloader/web/static/css/bootstrap.min.css` & `deezer_downloader-2.0.5/deezer_downloader/web/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.4/deezer_downloader/web/static/css/font-awesome.min.css` & `deezer_downloader-2.0.5/deezer_downloader/web/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.4/deezer_downloader/web/static/css/jquery.jgrowl.min.css` & `deezer_downloader-2.0.5/deezer_downloader/web/static/css/jquery.jgrowl.min.css`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.4/deezer_downloader/web/static/fonts/fontawesome-webfont.woff2` & `deezer_downloader-2.0.5/deezer_downloader/web/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.4/deezer_downloader/web/static/js/bootstrap.min.js` & `deezer_downloader-2.0.5/deezer_downloader/web/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.4/deezer_downloader/web/static/js/custom.js` & `deezer_downloader-2.0.5/deezer_downloader/web/static/js/custom.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.4/deezer_downloader/web/static/js/jquery.jgrowl.min.js` & `deezer_downloader-2.0.5/deezer_downloader/web/static/js/jquery.jgrowl.min.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.4/deezer_downloader/web/static/js/jquery.min.js` & `deezer_downloader-2.0.5/deezer_downloader/web/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.4/deezer_downloader/web/static/js/popper.min.js` & `deezer_downloader-2.0.5/deezer_downloader/web/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.4/deezer_downloader/web/templates/index.html` & `deezer_downloader-2.0.5/deezer_downloader/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.4/deezer_downloader/youtubedl.py` & `deezer_downloader-2.0.5/deezer_downloader/youtubedl.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.4/pyproject.toml` & `deezer_downloader-2.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deezer-downloader"
-version = "2.0.4"
+version = "2.0.5"
 description = "download music from Deezer with a nice front end"
 authors = ["kmille <github@androidloves.me>"]
 readme = "README.md"
 packages = [{include = "deezer_downloader"}]
 repository = "https://github.com/kmille/deezer-downloader"
 homepage = "https://github.com/kmille/deezer-downloader"
```

### Comparing `deezer_downloader-2.0.4/PKG-INFO` & `deezer_downloader-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deezer-downloader
-Version: 2.0.4
+Version: 2.0.5
 Summary: download music from Deezer with a nice front end
 Home-page: https://github.com/kmille/deezer-downloader
 Author: kmille
 Author-email: github@androidloves.me
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

