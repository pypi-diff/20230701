# Comparing `tmp/letterboxd_stats-0.2.4.tar.gz` & `tmp/letterboxd_stats-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "letterboxd_stats-0.2.4.tar", last modified: Fri Jun 30 20:18:09 2023, max compression
+gzip compressed data, was "letterboxd_stats-0.2.5.tar", last modified: Sat Jul  1 09:44:58 2023, max compression
```

## Comparing `letterboxd_stats-0.2.4.tar` & `letterboxd_stats-0.2.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-06-30 20:18:09.228808 letterboxd_stats-0.2.4/
--rw-rw-r--   0 marco     (1001) marco     (1001)     1089 2023-03-06 16:16:14.000000 letterboxd_stats-0.2.4/LICENCE
--rw-rw-r--   0 marco     (1001) marco     (1001)     2964 2023-06-30 20:18:09.228808 letterboxd_stats-0.2.4/PKG-INFO
--rw-rw-r--   0 marco     (1001) marco     (1001)     2446 2023-04-23 13:25:28.000000 letterboxd_stats-0.2.4/README.md
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-06-30 20:18:09.228808 letterboxd_stats-0.2.4/letterboxd_stats/
--rw-rw-r--   0 marco     (1001) marco     (1001)     1472 2023-06-30 20:01:47.000000 letterboxd_stats-0.2.4/letterboxd_stats/__init__.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     5331 2023-06-30 11:32:08.000000 letterboxd_stats-0.2.4/letterboxd_stats/cli.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     4440 2023-06-26 09:44:09.000000 letterboxd_stats-0.2.4/letterboxd_stats/data.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     3081 2023-06-13 14:08:12.000000 letterboxd_stats-0.2.4/letterboxd_stats/main.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     2864 2023-06-30 15:36:50.000000 letterboxd_stats-0.2.4/letterboxd_stats/tmdb.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     6306 2023-06-30 20:08:17.000000 letterboxd_stats-0.2.4/letterboxd_stats/web_scraper.py
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-06-30 20:18:09.228808 letterboxd_stats-0.2.4/letterboxd_stats.egg-info/
--rw-rw-r--   0 marco     (1001) marco     (1001)     2964 2023-06-30 20:18:09.000000 letterboxd_stats-0.2.4/letterboxd_stats.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1001) marco     (1001)      434 2023-06-30 20:18:09.000000 letterboxd_stats-0.2.4/letterboxd_stats.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)        1 2023-06-30 20:18:09.000000 letterboxd_stats-0.2.4/letterboxd_stats.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)       64 2023-06-30 20:18:09.000000 letterboxd_stats-0.2.4/letterboxd_stats.egg-info/entry_points.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)      142 2023-06-30 20:18:09.000000 letterboxd_stats-0.2.4/letterboxd_stats.egg-info/requires.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)       17 2023-06-30 20:18:09.000000 letterboxd_stats-0.2.4/letterboxd_stats.egg-info/top_level.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)      886 2023-06-30 20:14:27.000000 letterboxd_stats-0.2.4/pyproject.toml
--rw-rw-r--   0 marco     (1001) marco     (1001)       38 2023-06-30 20:18:09.228808 letterboxd_stats-0.2.4/setup.cfg
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-07-01 09:44:58.775144 letterboxd_stats-0.2.5/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     1089 2023-03-06 16:16:14.000000 letterboxd_stats-0.2.5/LICENCE
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2964 2023-07-01 09:44:58.775144 letterboxd_stats-0.2.5/PKG-INFO
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2446 2023-04-23 13:25:28.000000 letterboxd_stats-0.2.5/README.md
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-07-01 09:44:58.775144 letterboxd_stats-0.2.5/letterboxd_stats/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     1472 2023-06-30 20:22:08.000000 letterboxd_stats-0.2.5/letterboxd_stats/__init__.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     5331 2023-06-30 11:32:08.000000 letterboxd_stats-0.2.5/letterboxd_stats/cli.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     4440 2023-06-26 09:44:09.000000 letterboxd_stats-0.2.5/letterboxd_stats/data.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     3081 2023-06-13 14:08:12.000000 letterboxd_stats-0.2.5/letterboxd_stats/main.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2864 2023-06-30 15:36:50.000000 letterboxd_stats-0.2.5/letterboxd_stats/tmdb.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     6619 2023-07-01 09:24:22.000000 letterboxd_stats-0.2.5/letterboxd_stats/web_scraper.py
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-07-01 09:44:58.775144 letterboxd_stats-0.2.5/letterboxd_stats.egg-info/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2964 2023-07-01 09:44:58.000000 letterboxd_stats-0.2.5/letterboxd_stats.egg-info/PKG-INFO
+-rw-rw-r--   0 marco     (1001) marco     (1001)      434 2023-07-01 09:44:58.000000 letterboxd_stats-0.2.5/letterboxd_stats.egg-info/SOURCES.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)        1 2023-07-01 09:44:58.000000 letterboxd_stats-0.2.5/letterboxd_stats.egg-info/dependency_links.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)       64 2023-07-01 09:44:58.000000 letterboxd_stats-0.2.5/letterboxd_stats.egg-info/entry_points.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)      126 2023-07-01 09:44:58.000000 letterboxd_stats-0.2.5/letterboxd_stats.egg-info/requires.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)       17 2023-07-01 09:44:58.000000 letterboxd_stats-0.2.5/letterboxd_stats.egg-info/top_level.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)      887 2023-07-01 09:43:53.000000 letterboxd_stats-0.2.5/pyproject.toml
+-rw-rw-r--   0 marco     (1001) marco     (1001)       38 2023-07-01 09:44:58.775144 letterboxd_stats-0.2.5/setup.cfg
```

### Comparing `letterboxd_stats-0.2.4/LICENCE` & `letterboxd_stats-0.2.5/LICENCE`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.4/PKG-INFO` & `letterboxd_stats-0.2.5/letterboxd_stats.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: letterboxd_stats
-Version: 0.2.4
+Name: letterboxd-stats
+Version: 0.2.5
 Summary: Get information about your Letterboxd activity.
 Author: mBaratta96
 Project-URL: Homepage, https://github.com/mBaratta96/letterboxd_stats
 Project-URL: Bug Tracker, https://github.com/mBaratta96/letterboxd_stats/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `letterboxd_stats-0.2.4/README.md` & `letterboxd_stats-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.4/letterboxd_stats/__init__.py` & `letterboxd_stats-0.2.5/letterboxd_stats/__init__.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.4/letterboxd_stats/cli.py` & `letterboxd_stats-0.2.5/letterboxd_stats/cli.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.4/letterboxd_stats/data.py` & `letterboxd_stats-0.2.5/letterboxd_stats/data.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.4/letterboxd_stats/main.py` & `letterboxd_stats-0.2.5/letterboxd_stats/main.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.4/letterboxd_stats/tmdb.py` & `letterboxd_stats-0.2.5/letterboxd_stats/tmdb.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.2.4/letterboxd_stats/web_scraper.py` & `letterboxd_stats-0.2.5/letterboxd_stats/web_scraper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from zipfile import ZipFile
 from letterboxd_stats import config
 from letterboxd_stats import cli
 import requests
 from lxml import html
-import pickledb
+import shelve
 
 URL = "https://letterboxd.com"
 LOGIN_PAGE = URL + "/user/login.do"
 DATA_PAGE = URL + "/data/export"
 ADD_DIARY_URL = URL + "/s/save-diary-entry"
 MOVIE_OPERATIONS = {
     "Add to diary": "add_film_diary",
@@ -20,15 +20,14 @@
     "diary": lambda s: f"/csi/film/{s}/sidebar-user-actions/?esiAllowUser=true",
     "add_watchlist": lambda s: f"/film/{s}/add-to-watchlist/",
     "remove_watchlist": lambda s: f"/film/{s}/remove-from-watchlist/",
     "film_page": lambda s: f"/film/{s}",
 }
 
 cache_path = os.path.expanduser(os.path.join(config["root_folder"], "static", "cache.db"))
-tmdb_id_cache = pickledb.load(cache_path, auto_dump=True)
 
 
 class Downloader:
     def __init__(self):
         self.session = requests.Session()
         self.session.get(URL)
 
@@ -91,34 +90,46 @@
         getattr(self, MOVIE_OPERATIONS[answer])(link)
 
 
 def create_movie_url(title: str, operation: str):
     return URL + OPERATIONS_URLS[operation](title)
 
 
-def get_tmdb_id(link: str, is_diary: bool):
-    if tmdb_id_cache.exists(link):
-        return tmdb_id_cache.get(link)
+def _get_tmdb_id_from_web(link: str, is_diary: bool):
     res = requests.get(link)
     movie_page = html.fromstring(res.text)
     if is_diary:
         title_link = movie_page.xpath("//span[@class='film-title-wrapper']/a")
         if len(title_link) == 0:
-            return None
+            raise ValueError("No movie link found.")
         movie_link = title_link[0]
         movie_url = URL + movie_link.get("href")
         movie_page = html.fromstring(requests.get(movie_url).text)
     tmdb_link = movie_page.xpath("//a[@data-track-action='TMDb']")
     if len(tmdb_link) == 0:
-        return None
+        raise ValueError("No Movie link found")
     id = tmdb_link[0].get("href").split("/")[-2]
-    tmdb_id_cache.set(link, id)
     return int(id)
 
 
+def get_tmdb_id(link: str, is_diary: bool):
+    tmdb_id_cache = shelve.open(cache_path, writeback=False, protocol=5)
+    if link in tmdb_id_cache:
+        id = tmdb_id_cache[link]
+    else:
+        try:
+            id = _get_tmdb_id_from_web(link, is_diary)
+            tmdb_id_cache[link] = id
+        except ValueError as e:
+            print(e)
+            id = None
+    tmdb_id_cache.close()
+    return id
+
+
 def select_optional_operation():
     return cli.select_value(["Exit"] + list(MOVIE_OPERATIONS.keys()), "Select operation:")
 
 
 def search_film(title: str, allow_selection=False):
     search_url = create_movie_url(title, "search")
     res = requests.get(search_url)
```

### Comparing `letterboxd_stats-0.2.4/letterboxd_stats.egg-info/PKG-INFO` & `letterboxd_stats-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: letterboxd-stats
-Version: 0.2.4
+Name: letterboxd_stats
+Version: 0.2.5
 Summary: Get information about your Letterboxd activity.
 Author: mBaratta96
 Project-URL: Homepage, https://github.com/mBaratta96/letterboxd_stats
 Project-URL: Bug Tracker, https://github.com/mBaratta96/letterboxd_stats/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `letterboxd_stats-0.2.4/pyproject.toml` & `letterboxd_stats-0.2.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "letterboxd_stats"
-version = "0.2.4"
+version = "0.2.5"
 authors = [{ name = "mBaratta96" }]
 description = "Get information about your Letterboxd activity."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
-  "Programming Language :: Python :: 3",
-  "License :: OSI Approved :: MIT License",
-  "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
 ]
 dependencies = [
-  "ascii_magic~=2.3.0",
-  "inquirerpy~=0.3.4",
-  "lxml~=4.9.0",
-  "pandas~=1.5.1",
-  "pickleDB~=0.9.2",
-  "platformdirs~=3.0.0",
-  "rich~=13.3.5",
-  "tmdbv3api~=1.7.7",
-  "tomli~=2.0.1",
+    "ascii_magic~=2.3.0",
+    "inquirerpy~=0.3.4",
+    "lxml~=4.9.0",
+    "pandas~=1.5.1",
+    "platformdirs~=3.0.0",
+    "rich~=13.3.5",
+    "tmdbv3api~=1.7.7",
+    "tomli~=2.0.1",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/mBaratta96/letterboxd_stats"
 "Bug Tracker" = "https://github.com/mBaratta96/letterboxd_stats/issues"
 
 [project.scripts]
```

