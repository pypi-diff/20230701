# Comparing `tmp/IMDBTraktSyncer-1.5.4.tar.gz` & `tmp/IMDBTraktSyncer-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDBTraktSyncer-1.5.4.tar", last modified: Tue Jun 27 08:05:19 2023, max compression
+gzip compressed data, was "IMDBTraktSyncer-1.5.5.tar", last modified: Sat Jul  1 00:58:12 2023, max compression
```

## Comparing `IMDBTraktSyncer-1.5.4.tar` & `IMDBTraktSyncer-1.5.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 08:05:19.970382 IMDBTraktSyncer-1.5.4/
-drwxrwxrwx   0        0        0        0 2023-06-27 08:05:19.946384 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    35244 2023-06-27 07:18:11.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     4624 2023-06-19 09:47:47.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4317 2023-06-19 09:47:23.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     6946 2023-06-27 06:49:08.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     1669 2023-06-25 00:09:11.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/errorLogger.py
--rw-rw-rw-   0        0        0    10647 2023-06-25 00:08:47.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/imdbData.py
--rw-rw-rw-   0        0        0    10353 2023-06-19 09:48:23.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0    12192 2023-06-19 15:47:42.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:05:19.967384 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0    12155 2023-06-27 08:05:19.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2023-06-27 08:05:19.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 08:05:19.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-06-27 08:05:19.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-06-27 08:05:19.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-27 08:05:19.000000 IMDBTraktSyncer-1.5.4/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.5.4/LICENSE
--rw-rw-rw-   0        0        0    12155 2023-06-27 08:05:19.969383 IMDBTraktSyncer-1.5.4/PKG-INFO
--rw-rw-rw-   0        0        0    11409 2023-06-27 08:02:25.000000 IMDBTraktSyncer-1.5.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-27 08:05:19.970382 IMDBTraktSyncer-1.5.4/setup.cfg
--rw-rw-rw-   0        0        0     1377 2023-06-27 08:04:31.000000 IMDBTraktSyncer-1.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 00:58:12.187823 IMDBTraktSyncer-1.5.5/
+drwxrwxrwx   0        0        0        0 2023-07-01 00:58:12.155671 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    35244 2023-06-27 07:18:11.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     4624 2023-06-19 09:47:47.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4317 2023-06-19 09:47:23.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     6946 2023-06-27 06:49:08.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     1669 2023-06-25 00:09:11.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/errorLogger.py
+-rw-rw-rw-   0        0        0    10884 2023-06-28 04:22:19.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/imdbData.py
+-rw-rw-rw-   0        0        0    10353 2023-06-19 09:48:23.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0    12192 2023-06-19 15:47:42.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-07-01 00:58:12.185669 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    12155 2023-07-01 00:58:11.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      549 2023-07-01 00:58:12.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 00:58:11.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-07-01 00:58:11.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-07-01 00:58:11.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-01 00:58:11.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.5.5/LICENSE
+-rw-rw-rw-   0        0        0    12155 2023-07-01 00:58:12.187823 IMDBTraktSyncer-1.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0    11409 2023-07-01 00:57:17.000000 IMDBTraktSyncer-1.5.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-01 00:58:12.188825 IMDBTraktSyncer-1.5.5/setup.cfg
+-rw-rw-rw-   0        0        0     1377 2023-07-01 00:57:43.000000 IMDBTraktSyncer-1.5.5/setup.py
```

### Comparing `IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/IMDBTraktSyncer.py` & `IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/IMDBTraktSyncer.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/authTrakt.py` & `IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/checkChromedriver.py` & `IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/errorHandling.py` & `IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/errorLogger.py` & `IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/errorLogger.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/imdbData.py` & `IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/imdbData.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,19 +185,23 @@
                     reviews.append(review)
 
                 try:
                     # Check if "Next" link exists
                     next_link = driver.find_element(By.CSS_SELECTOR, "a.next-page")
                     if next_link.get_attribute("href") == "#":
                         break  # No more pages, exit the loop
-
+                    
+                    # Get the current url before clicking the "Next" link
+                    current_url = driver.current_url
+                    
+                    # Click the "Next" link
                     next_link.click()
 
                     # Wait until the URL changes
-                    wait.until(EC.url_changes(current_url))
+                    wait.until(lambda driver: driver.current_url != current_url)
                     
                     # Refresh review_elements
                     review_elements = wait.until(EC.presence_of_all_elements_located((By.CSS_SELECTOR, ".imdb-user-review")))
 
                 except NoSuchElementException:
                     # "Next" link not found on IMDB reviews page, exit the loop without error
                     error_message = '"Next" link not found on IMDB reviews page. Exiting the loop without error.'
```

### Comparing `IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/traktData.py` & `IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/traktData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.4/IMDBTraktSyncer/verifyCredentials.py` & `IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.4/IMDBTraktSyncer.egg-info/PKG-INFO` & `IMDBTraktSyncer-1.5.5/IMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.5.4
+Version: 1.5.5
 Summary: A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `IMDBTraktSyncer-1.5.4/IMDBTraktSyncer.egg-info/SOURCES.txt` & `IMDBTraktSyncer-1.5.5/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.4/LICENSE` & `IMDBTraktSyncer-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.4/PKG-INFO` & `IMDBTraktSyncer-1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.5.4
+Version: 1.5.5
 Summary: A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `IMDBTraktSyncer-1.5.4/README.md` & `IMDBTraktSyncer-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.4/setup.py` & `IMDBTraktSyncer-1.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), 'r', encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.5.4'
+VERSION = '1.5.5'
 DESCRIPTION = 'A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
```

