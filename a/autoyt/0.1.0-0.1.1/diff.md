# Comparing `tmp/autoyt-0.1.0.tar.gz` & `tmp/autoyt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoyt-0.1.0.tar", last modified: Sat Jul  1 11:12:20 2023, max compression
+gzip compressed data, was "autoyt-0.1.1.tar", last modified: Sat Jul  1 11:26:45 2023, max compression
```

## Comparing `autoyt-0.1.0.tar` & `autoyt-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,21 @@
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-07-01 11:12:20.523914 autoyt-0.1.0/
--rwxrwxrwx   0 user      (1000) user      (1000)    35182 2023-06-19 16:22:47.000000 autoyt-0.1.0/LICENSE
--rwxrwxrwx   0 user      (1000) user      (1000)     5797 2023-07-01 11:12:20.519915 autoyt-0.1.0/PKG-INFO
--rwxrwxrwx   0 user      (1000) user      (1000)     5472 2023-06-23 18:12:03.000000 autoyt-0.1.0/README.md
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-07-01 11:12:20.262272 autoyt-0.1.0/autoyt/
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-07-01 11:12:20.264272 autoyt-0.1.0/autoyt/src/
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-07-01 11:12:20.474581 autoyt-0.1.0/autoyt/src/autoyt.egg-info/
--rwxrwxrwx   0 user      (1000) user      (1000)     5797 2023-07-01 11:12:20.000000 autoyt-0.1.0/autoyt/src/autoyt.egg-info/PKG-INFO
--rwxrwxrwx   0 user      (1000) user      (1000)      230 2023-07-01 11:12:20.000000 autoyt-0.1.0/autoyt/src/autoyt.egg-info/SOURCES.txt
--rwxrwxrwx   0 user      (1000) user      (1000)        1 2023-07-01 11:12:20.000000 autoyt-0.1.0/autoyt/src/autoyt.egg-info/dependency_links.txt
--rwxrwxrwx   0 user      (1000) user      (1000)       14 2023-07-01 11:12:20.000000 autoyt-0.1.0/autoyt/src/autoyt.egg-info/requires.txt
--rwxrwxrwx   0 user      (1000) user      (1000)        7 2023-07-01 11:12:20.000000 autoyt-0.1.0/autoyt/src/autoyt.egg-info/top_level.txt
--rwxrwxrwx   0 user      (1000) user      (1000)       38 2023-07-01 11:12:20.524915 autoyt-0.1.0/setup.cfg
--rwxrwxrwx   0 user      (1000) user      (1000)      779 2023-07-01 11:11:52.000000 autoyt-0.1.0/setup.py
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-07-01 11:26:45.516083 autoyt-0.1.1/
+-rwxrwxrwx   0 user      (1000) user      (1000)    35182 2023-06-19 16:22:47.000000 autoyt-0.1.1/LICENSE
+-rwxrwxrwx   0 user      (1000) user      (1000)     5797 2023-07-01 11:26:45.513082 autoyt-0.1.1/PKG-INFO
+-rwxrwxrwx   0 user      (1000) user      (1000)     5472 2023-06-23 18:12:03.000000 autoyt-0.1.1/README.md
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-07-01 11:26:45.083706 autoyt-0.1.1/autoyt/
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-07-01 11:26:45.093226 autoyt-0.1.1/autoyt/src/
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-07-01 11:26:45.311311 autoyt-0.1.1/autoyt/src/autoyt/
+-rwxrwxrwx   0 user      (1000) user      (1000)     2264 2023-07-01 10:47:55.000000 autoyt-0.1.1/autoyt/src/autoyt/cache.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     3053 2023-07-01 10:51:50.000000 autoyt-0.1.1/autoyt/src/autoyt/config.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     1452 2023-06-23 17:29:24.000000 autoyt-0.1.1/autoyt/src/autoyt/converter.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     3662 2023-06-25 16:07:47.000000 autoyt-0.1.1/autoyt/src/autoyt/downloader.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     1803 2023-06-23 13:40:25.000000 autoyt-0.1.1/autoyt/src/autoyt/videos.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     1738 2023-06-23 17:30:12.000000 autoyt-0.1.1/autoyt/src/autoyt/youtubeinfo.py
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-07-01 11:26:45.477083 autoyt-0.1.1/autoyt/src/autoyt.egg-info/
+-rwxrwxrwx   0 user      (1000) user      (1000)     5797 2023-07-01 11:26:44.000000 autoyt-0.1.1/autoyt/src/autoyt.egg-info/PKG-INFO
+-rwxrwxrwx   0 user      (1000) user      (1000)      409 2023-07-01 11:26:45.000000 autoyt-0.1.1/autoyt/src/autoyt.egg-info/SOURCES.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)        1 2023-07-01 11:26:44.000000 autoyt-0.1.1/autoyt/src/autoyt.egg-info/dependency_links.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)       14 2023-07-01 11:26:44.000000 autoyt-0.1.1/autoyt/src/autoyt.egg-info/requires.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)        7 2023-07-01 11:26:44.000000 autoyt-0.1.1/autoyt/src/autoyt.egg-info/top_level.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)       38 2023-07-01 11:26:45.517082 autoyt-0.1.1/setup.cfg
+-rwxrwxrwx   0 user      (1000) user      (1000)      763 2023-07-01 11:22:37.000000 autoyt-0.1.1/setup.py
```

### Comparing `autoyt-0.1.0/LICENSE` & `autoyt-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autoyt-0.1.0/PKG-INFO` & `autoyt-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoyt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python script for quickly searching and downloading new content out of YouTube.
 Home-page: https://github.com/two-six/autoYT
 Author: Two-Six
 Author-email: twopsix@gmail.com
 License: AGPLv3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `autoyt-0.1.0/README.md` & `autoyt-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `autoyt-0.1.0/autoyt/src/autoyt.egg-info/PKG-INFO` & `autoyt-0.1.1/autoyt/src/autoyt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoyt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python script for quickly searching and downloading new content out of YouTube.
 Home-page: https://github.com/two-six/autoYT
 Author: Two-Six
 Author-email: twopsix@gmail.com
 License: AGPLv3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `autoyt-0.1.0/setup.py` & `autoyt-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="autoyt",
-    version="0.1.0",
+    version="0.1.1",
     author="Two-Six",
     author_email="twopsix@gmail.com",
     url="https://github.com/two-six/autoYT",
     description="Python script for quickly searching and downloading new content out of YouTube.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    packages=setuptools.find_packages(),
+    packages=["autoyt"],
     license="AGPLv3",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     py_modules=["autoyt"],
```

