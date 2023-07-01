# Comparing `tmp/llvd-3.0.5.tar.gz` & `tmp/llvd-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llvd-3.0.5.tar", last modified: Fri Jun 30 14:09:38 2023, max compression
+gzip compressed data, was "llvd-3.0.6.tar", last modified: Sat Jul  1 10:00:59 2023, max compression
```

## Comparing `llvd-3.0.5.tar` & `llvd-3.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:09:38.768085 llvd-3.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-30 14:09:22.000000 llvd-3.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-06-30 14:09:38.768085 llvd-3.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-06-30 14:09:22.000000 llvd-3.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:09:38.764085 llvd-3.0.5/llvd/
--rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-30 14:09:22.000000 llvd-3.0.5/llvd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14169 2023-06-30 14:09:22.000000 llvd-3.0.5/llvd/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-30 14:09:22.000000 llvd-3.0.5/llvd/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-30 14:09:22.000000 llvd-3.0.5/llvd/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-30 14:09:22.000000 llvd-3.0.5/llvd/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 14:09:22.000000 llvd-3.0.5/llvd/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-30 14:09:22.000000 llvd-3.0.5/llvd/process_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-30 14:09:22.000000 llvd-3.0.5/llvd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:09:38.768085 llvd-3.0.5/llvd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-06-30 14:09:38.000000 llvd-3.0.5/llvd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-30 14:09:38.000000 llvd-3.0.5/llvd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:09:38.000000 llvd-3.0.5/llvd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-30 14:09:38.000000 llvd-3.0.5/llvd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-30 14:09:38.000000 llvd-3.0.5/llvd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-30 14:09:38.000000 llvd-3.0.5/llvd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:09:38.768085 llvd-3.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-30 14:09:22.000000 llvd-3.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:00:59.468662 llvd-3.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-01 10:00:42.000000 llvd-3.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-07-01 10:00:59.468662 llvd-3.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-07-01 10:00:42.000000 llvd-3.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:00:59.464662 llvd-3.0.6/llvd/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-07-01 10:00:42.000000 llvd-3.0.6/llvd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-07-01 10:00:42.000000 llvd-3.0.6/llvd/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-01 10:00:42.000000 llvd-3.0.6/llvd/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-01 10:00:42.000000 llvd-3.0.6/llvd/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-01 10:00:42.000000 llvd-3.0.6/llvd/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-01 10:00:42.000000 llvd-3.0.6/llvd/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-01 10:00:42.000000 llvd-3.0.6/llvd/process_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-01 10:00:42.000000 llvd-3.0.6/llvd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:00:59.468662 llvd-3.0.6/llvd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-07-01 10:00:59.000000 llvd-3.0.6/llvd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-01 10:00:59.000000 llvd-3.0.6/llvd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 10:00:59.000000 llvd-3.0.6/llvd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-01 10:00:59.000000 llvd-3.0.6/llvd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-01 10:00:59.000000 llvd-3.0.6/llvd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-01 10:00:59.000000 llvd-3.0.6/llvd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 10:00:59.468662 llvd-3.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-01 10:00:42.000000 llvd-3.0.6/setup.py
```

### Comparing `llvd-3.0.5/LICENSE` & `llvd-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `llvd-3.0.5/PKG-INFO` & `llvd-3.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llvd
-Version: 3.0.5
+Version: 3.0.6
 Summary: Linkedin Learning Video Downloader CLI Tool
 Home-page: https://github.com/knowbee/llvd.git
 Author: Igwaneza Bruce
 Author-email: knowbeeinc@gmail.com
 Platform: any
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `llvd-3.0.5/README.md` & `llvd-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `llvd-3.0.5/llvd/app.py` & `llvd-3.0.6/llvd/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,15 +312,15 @@
 
         self.remove_failed_downloads()
         try:
             r = requests.get(
                 config.course_url.format(self.course_slug),
                 cookies=self.cookies,
                 headers=self.headers,
-                allow_redirects=False,
+                allow_redirects=True,
             )
             course_name = r.json()["elements"][0]["title"]
             course_name = re.sub(r'[\\/*?:"<>|]', "", course_name)
             course_path = f"./{self.course_slug}"
             chapters = r.json()["elements"][0]["chapters"]
             exercise_files = r.json()["elements"][0]["exerciseFileUrls"]
             chapters_index = 1
@@ -369,21 +369,19 @@
         except requests.exceptions.ConnectionError:
             click.echo(
                 click.style(
                     f"ConnectionError: There is a connection error. Please check your connectivity.\n",
                     fg="red",
                 )
             )
-        except json.decoder.JSONDecodeError: 
-            click.echo(
-               click.style(
-                            f"The course is locked, you probably"
+        except json.decoder.JSONDecodeError as e: 
+            click.echo(click.style(
+                            f"The course is locked, you probably "
                             f"need a premium account",
-                            fg="red",
-                )
+                            fg="red")
             )
         except Exception as e:
             if os.path.exists(
                 f"{self.chapter_path}/{self.current_video_index:0=2d}. {clean_name(self.current_video_name)}.mp4"
             ):
                 os.remove(
                     f"{self.chapter_path}/{self.current_video_index:0=2d}. {clean_name(self.current_video_name)}.mp4"
```

### Comparing `llvd-3.0.5/llvd/cli.py` & `llvd-3.0.6/llvd/cli.py`

 * *Files identical despite different names*

### Comparing `llvd-3.0.5/llvd/config.py` & `llvd-3.0.6/llvd/config.py`

 * *Files identical despite different names*

### Comparing `llvd-3.0.5/llvd/downloader.py` & `llvd-3.0.6/llvd/downloader.py`

 * *Files identical despite different names*

### Comparing `llvd-3.0.5/llvd/process_io.py` & `llvd-3.0.6/llvd/process_io.py`

 * *Files identical despite different names*

### Comparing `llvd-3.0.5/llvd/utils.py` & `llvd-3.0.6/llvd/utils.py`

 * *Files identical despite different names*

### Comparing `llvd-3.0.5/llvd.egg-info/PKG-INFO` & `llvd-3.0.6/llvd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llvd
-Version: 3.0.5
+Version: 3.0.6
 Summary: Linkedin Learning Video Downloader CLI Tool
 Home-page: https://github.com/knowbee/llvd.git
 Author: Igwaneza Bruce
 Author-email: knowbeeinc@gmail.com
 Platform: any
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `llvd-3.0.5/setup.py` & `llvd-3.0.6/setup.py`

 * *Files identical despite different names*

