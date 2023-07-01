# Comparing `tmp/TMDBTraktSyncer-1.4.0.tar.gz` & `tmp/TMDBTraktSyncer-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TMDBTraktSyncer-1.4.0.tar", last modified: Tue Jun 27 07:51:49 2023, max compression
+gzip compressed data, was "TMDBTraktSyncer-1.4.1.tar", last modified: Sat Jul  1 01:06:16 2023, max compression
```

## Comparing `TMDBTraktSyncer-1.4.0.tar` & `TMDBTraktSyncer-1.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 07:51:49.837658 TMDBTraktSyncer-1.4.0/
--rw-rw-rw-   0        0        0     1079 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.4.0/LICENSE
--rw-rw-rw-   0        0        0    10839 2023-06-27 07:51:49.836658 TMDBTraktSyncer-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0    10091 2023-06-27 07:51:15.000000 TMDBTraktSyncer-1.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 07:51:49.802660 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/
--rw-rw-rw-   0        0        0    18069 2023-06-27 07:32:36.000000 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/TMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     4548 2023-06-27 07:34:14.000000 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0    10181 2023-06-27 07:45:31.000000 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     1669 2023-06-27 07:34:28.000000 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/errorLogger.py
--rw-rw-rw-   0        0        0     4058 2023-06-27 07:33:19.000000 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/tmdbData.py
--rw-rw-rw-   0        0        0     7120 2023-06-27 07:33:10.000000 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0     8014 2023-06-27 07:36:59.000000 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:51:49.835658 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0    10839 2023-06-27 07:51:49.000000 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-06-27 07:51:49.000000 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 07:51:49.000000 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-06-27 07:51:49.000000 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-06-27 07:51:49.000000 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-27 07:51:49.000000 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 07:51:49.838659 TMDBTraktSyncer-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1341 2023-06-27 07:50:17.000000 TMDBTraktSyncer-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 01:06:16.512729 TMDBTraktSyncer-1.4.1/
+-rw-rw-rw-   0        0        0     1079 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.4.1/LICENSE
+-rw-rw-rw-   0        0        0    10839 2023-07-01 01:06:16.511728 TMDBTraktSyncer-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10091 2023-07-01 01:05:25.000000 TMDBTraktSyncer-1.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 01:06:16.480728 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    18069 2023-06-28 04:01:34.000000 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/TMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     4548 2023-06-27 07:34:14.000000 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0    10181 2023-06-27 07:45:31.000000 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     1669 2023-06-27 07:34:28.000000 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/errorLogger.py
+-rw-rw-rw-   0        0        0     4058 2023-06-27 07:33:19.000000 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/tmdbData.py
+-rw-rw-rw-   0        0        0     7120 2023-06-27 07:33:10.000000 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0     8014 2023-06-27 07:36:59.000000 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-07-01 01:06:16.509728 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    10839 2023-07-01 01:06:16.000000 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-07-01 01:06:16.000000 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 01:06:16.000000 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-07-01 01:06:16.000000 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-07-01 01:06:16.000000 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-01 01:06:16.000000 TMDBTraktSyncer-1.4.1/TMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 01:06:16.512729 TMDBTraktSyncer-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1341 2023-07-01 01:02:52.000000 TMDBTraktSyncer-1.4.1/setup.py
```

### Comparing `TMDBTraktSyncer-1.4.0/LICENSE` & `TMDBTraktSyncer-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.4.0/PKG-INFO` & `TMDBTraktSyncer-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.4.0
+Version: 1.4.1
 Summary: A python script that syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `TMDBTraktSyncer-1.4.0/README.md` & `TMDBTraktSyncer-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/TMDBTraktSyncer.py` & `TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/TMDBTraktSyncer.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -319,16 +319,16 @@
                 account_id = json_data['id']
                 
                 # Count the total number of items
                 num_items = len(tmdb_watchlist_items_to_remove)
                 item_count = 0
                 
                 for item in tmdb_watchlist_items_to_remove:
-                    print(f" - Removing item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from TMDB Watchlist")
                     item_count += 1
+                    print(f" - Removing item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from TMDB Watchlist")
                     payload = {}  # Add any additional payload parameters if required
                     if item['Type'] == 'movie':
                         url = f"https://api.themoviedb.org/3/account/{account_id}/watchlist"
                         payload['media_type'] = "movie"
                         payload['media_id'] = item['TMDB_ID']
                         payload['watchlist'] = False  # Set watchlist to False to remove the item
                         response = EH.make_tmdb_request(url, payload=payload)
```

### Comparing `TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/authTrakt.py` & `TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/errorHandling.py` & `TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/errorLogger.py` & `TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/errorLogger.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/tmdbData.py` & `TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/tmdbData.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/traktData.py` & `TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/traktData.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/verifyCredentials.py` & `TMDBTraktSyncer-1.4.1/TMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.4.0/TMDBTraktSyncer.egg-info/PKG-INFO` & `TMDBTraktSyncer-1.4.1/TMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.4.0
+Version: 1.4.1
 Summary: A python script that syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `TMDBTraktSyncer-1.4.0/TMDBTraktSyncer.egg-info/SOURCES.txt` & `TMDBTraktSyncer-1.4.1/TMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.4.0/setup.py` & `TMDBTraktSyncer-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), 'r', encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.4.0'
+VERSION = '1.4.1'
 DESCRIPTION = 'A python script that syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.'
 
 # Setting up
 setup(
     name="TMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
```

