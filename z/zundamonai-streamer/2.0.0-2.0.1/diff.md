# Comparing `tmp/zundamonai-streamer-2.0.0.tar.gz` & `tmp/zundamonai-streamer-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zundamonai-streamer-2.0.0.tar", last modified: Sat Jul  1 18:19:56 2023, max compression
+gzip compressed data, was "zundamonai-streamer-2.0.1.tar", last modified: Sat Jul  1 21:34:59 2023, max compression
```

## Comparing `zundamonai-streamer-2.0.0.tar` & `zundamonai-streamer-2.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-07-01 18:19:56.775040 zundamonai-streamer-2.0.0/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-06-05 06:55:47.000000 zundamonai-streamer-2.0.0/LICENSE
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     7651 2023-07-01 17:54:59.000000 zundamonai-streamer-2.0.0/LICENSE_ffmpeg
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      658 2023-07-01 18:19:56.775040 zundamonai-streamer-2.0.0/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     8475 2023-07-01 17:54:59.000000 zundamonai-streamer-2.0.0/README.md
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-07-01 18:19:56.775040 zundamonai-streamer-2.0.0/setup.cfg
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1197 2023-07-01 18:13:31.000000 zundamonai-streamer-2.0.0/setup.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-07-01 18:19:56.775040 zundamonai-streamer-2.0.0/src/
--rwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     5946 2023-07-01 17:54:59.000000 zundamonai-streamer-2.0.0/src/ZundamonAIStreamer.py
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     3966 2023-07-01 17:54:59.000000 zundamonai-streamer-2.0.0/src/ZundamonAIStreamerManager.py
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)    16934 2023-07-01 17:54:59.000000 zundamonai-streamer-2.0.0/src/ZundamonAIStreamerUI.py
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      134 2023-07-01 18:12:49.000000 zundamonai-streamer-2.0.0/src/__init__.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-07-01 18:19:56.775040 zundamonai-streamer-2.0.0/src/zundamonai_streamer.egg-info/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      658 2023-07-01 18:19:56.000000 zundamonai-streamer-2.0.0/src/zundamonai_streamer.egg-info/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      424 2023-07-01 18:19:56.000000 zundamonai-streamer-2.0.0/src/zundamonai_streamer.egg-info/SOURCES.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-07-01 18:19:56.000000 zundamonai-streamer-2.0.0/src/zundamonai_streamer.egg-info/dependency_links.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-07-01 17:54:59.000000 zundamonai-streamer-2.0.0/src/zundamonai_streamer.egg-info/not-zip-safe
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      140 2023-07-01 18:19:56.000000 zundamonai-streamer-2.0.0/src/zundamonai_streamer.egg-info/requires.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       75 2023-07-01 18:19:56.000000 zundamonai-streamer-2.0.0/src/zundamonai_streamer.egg-info/top_level.txt
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-07-01 21:34:59.415040 zundamonai-streamer-2.0.1/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-06-05 06:55:47.000000 zundamonai-streamer-2.0.1/LICENSE
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     7651 2023-07-01 17:54:59.000000 zundamonai-streamer-2.0.1/LICENSE_ffmpeg
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      658 2023-07-01 21:34:59.415040 zundamonai-streamer-2.0.1/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     8475 2023-07-01 17:54:59.000000 zundamonai-streamer-2.0.1/README.md
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-07-01 21:34:59.415040 zundamonai-streamer-2.0.1/setup.cfg
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1197 2023-07-01 21:27:02.000000 zundamonai-streamer-2.0.1/setup.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-07-01 21:34:59.415040 zundamonai-streamer-2.0.1/src/
+-rwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     5946 2023-07-01 17:54:59.000000 zundamonai-streamer-2.0.1/src/ZundamonAIStreamer.py
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     3966 2023-07-01 17:54:59.000000 zundamonai-streamer-2.0.1/src/ZundamonAIStreamerManager.py
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)    16934 2023-07-01 17:54:59.000000 zundamonai-streamer-2.0.1/src/ZundamonAIStreamerUI.py
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      134 2023-07-01 21:27:15.000000 zundamonai-streamer-2.0.1/src/__init__.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-07-01 21:34:59.415040 zundamonai-streamer-2.0.1/src/zundamonai_streamer.egg-info/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      658 2023-07-01 21:34:59.000000 zundamonai-streamer-2.0.1/src/zundamonai_streamer.egg-info/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      424 2023-07-01 21:34:59.000000 zundamonai-streamer-2.0.1/src/zundamonai_streamer.egg-info/SOURCES.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-07-01 21:34:59.000000 zundamonai-streamer-2.0.1/src/zundamonai_streamer.egg-info/dependency_links.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-07-01 17:54:59.000000 zundamonai-streamer-2.0.1/src/zundamonai_streamer.egg-info/not-zip-safe
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       90 2023-07-01 21:34:59.000000 zundamonai-streamer-2.0.1/src/zundamonai_streamer.egg-info/requires.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       75 2023-07-01 21:34:59.000000 zundamonai-streamer-2.0.1/src/zundamonai_streamer.egg-info/top_level.txt
```

### Comparing `zundamonai-streamer-2.0.0/LICENSE` & `zundamonai-streamer-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zundamonai-streamer-2.0.0/LICENSE_ffmpeg` & `zundamonai-streamer-2.0.1/LICENSE_ffmpeg`

 * *Files identical despite different names*

### Comparing `zundamonai-streamer-2.0.0/PKG-INFO` & `zundamonai-streamer-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zundamonai-streamer
-Version: 2.0.0
+Version: 2.0.1
 Summary: Zundamon with ChatGPT brain answers aloud YouTube chat messages.
 Home-page: https://github.com/GeneralYadoc/ChatAIStreamer
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `zundamonai-streamer-2.0.0/README.md` & `zundamonai-streamer-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `zundamonai-streamer-2.0.0/setup.py` & `zundamonai-streamer-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def _requires_from_file(filename):
     return open(filename).read().splitlines()
 
 
 setup(
     name="zundamonai-streamer",
-    version="2.0.0",
+    version="2.0.1",
     license="MIT",
     description="Zundamon with ChatGPT brain answers aloud YouTube chat messages.",
     author="General Yadoc",
     author_email="133023047+GeneralYadoc@users.noreply.github.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         'Programming Language :: Python',
```

### Comparing `zundamonai-streamer-2.0.0/src/ZundamonAIStreamer.py` & `zundamonai-streamer-2.0.1/src/ZundamonAIStreamer.py`

 * *Files identical despite different names*

### Comparing `zundamonai-streamer-2.0.0/src/ZundamonAIStreamerManager.py` & `zundamonai-streamer-2.0.1/src/ZundamonAIStreamerManager.py`

 * *Files identical despite different names*

### Comparing `zundamonai-streamer-2.0.0/src/ZundamonAIStreamerUI.py` & `zundamonai-streamer-2.0.1/src/ZundamonAIStreamerUI.py`

 * *Files identical despite different names*

### Comparing `zundamonai-streamer-2.0.0/src/zundamonai_streamer.egg-info/PKG-INFO` & `zundamonai-streamer-2.0.1/src/zundamonai_streamer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zundamonai-streamer
-Version: 2.0.0
+Version: 2.0.1
 Summary: Zundamon with ChatGPT brain answers aloud YouTube chat messages.
 Home-page: https://github.com/GeneralYadoc/ChatAIStreamer
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

