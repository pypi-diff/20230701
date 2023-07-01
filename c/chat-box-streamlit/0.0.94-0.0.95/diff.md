# Comparing `tmp/chat-box-streamlit-0.0.94.tar.gz` & `tmp/chat-box-streamlit-0.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat-box-streamlit-0.0.94.tar", last modified: Sat Jul  1 10:56:13 2023, max compression
+gzip compressed data, was "chat-box-streamlit-0.0.95.tar", last modified: Sat Jul  1 11:52:23 2023, max compression
```

## Comparing `chat-box-streamlit-0.0.94.tar` & `chat-box-streamlit-0.0.95.tar`

### file list

```diff
@@ -1,15 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:56:13.788792 chat-box-streamlit-0.0.94/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-01 10:56:01.000000 chat-box-streamlit-0.0.94/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-01 10:56:01.000000 chat-box-streamlit-0.0.94/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-01 10:56:13.788792 chat-box-streamlit-0.0.94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-01 10:56:01.000000 chat-box-streamlit-0.0.94/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:56:13.788792 chat-box-streamlit-0.0.94/chat_box_streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-01 10:56:01.000000 chat-box-streamlit-0.0.94/chat_box_streamlit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:56:13.788792 chat-box-streamlit-0.0.94/chat_box_streamlit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-01 10:56:13.000000 chat-box-streamlit-0.0.94/chat_box_streamlit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-01 10:56:13.000000 chat-box-streamlit-0.0.94/chat_box_streamlit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 10:56:13.000000 chat-box-streamlit-0.0.94/chat_box_streamlit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-01 10:56:13.000000 chat-box-streamlit-0.0.94/chat_box_streamlit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-01 10:56:13.000000 chat-box-streamlit-0.0.94/chat_box_streamlit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 10:56:13.788792 chat-box-streamlit-0.0.94/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-01 10:56:01.000000 chat-box-streamlit-0.0.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:52:23.990256 chat-box-streamlit-0.0.95/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-01 11:52:13.000000 chat-box-streamlit-0.0.95/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-01 11:52:13.000000 chat-box-streamlit-0.0.95/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-01 11:52:23.990256 chat-box-streamlit-0.0.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-01 11:52:13.000000 chat-box-streamlit-0.0.95/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:52:23.990256 chat-box-streamlit-0.0.95/chat_box_streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-01 11:52:13.000000 chat-box-streamlit-0.0.95/chat_box_streamlit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:52:23.986256 chat-box-streamlit-0.0.95/chat_box_streamlit/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:52:23.990256 chat-box-streamlit-0.0.95/chat_box_streamlit/frontend/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:52:23.990256 chat-box-streamlit-0.0.95/chat_box_streamlit/frontend/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   400495 2023-07-01 11:52:13.000000 chat-box-streamlit-0.0.95/chat_box_streamlit/frontend/dist/assets/index-ba3e6331.js
+-rw-r--r--   0 runner    (1001) docker     (123)   197459 2023-07-01 11:52:13.000000 chat-box-streamlit-0.0.95/chat_box_streamlit/frontend/dist/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    36284 2023-07-01 11:52:13.000000 chat-box-streamlit-0.0.95/chat_box_streamlit/frontend/dist/bot.png
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-01 11:52:13.000000 chat-box-streamlit-0.0.95/chat_box_streamlit/frontend/dist/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-01 11:52:13.000000 chat-box-streamlit-0.0.95/chat_box_streamlit/frontend/dist/send.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    27040 2023-07-01 11:52:13.000000 chat-box-streamlit-0.0.95/chat_box_streamlit/frontend/dist/user.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:52:23.990256 chat-box-streamlit-0.0.95/chat_box_streamlit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-01 11:52:23.000000 chat-box-streamlit-0.0.95/chat_box_streamlit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-01 11:52:23.000000 chat-box-streamlit-0.0.95/chat_box_streamlit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 11:52:23.000000 chat-box-streamlit-0.0.95/chat_box_streamlit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-01 11:52:23.000000 chat-box-streamlit-0.0.95/chat_box_streamlit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-01 11:52:23.000000 chat-box-streamlit-0.0.95/chat_box_streamlit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 11:52:23.990256 chat-box-streamlit-0.0.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-01 11:52:13.000000 chat-box-streamlit-0.0.95/setup.py
```

### Comparing `chat-box-streamlit-0.0.94/LICENSE` & `chat-box-streamlit-0.0.95/LICENSE`

 * *Files identical despite different names*

### Comparing `chat-box-streamlit-0.0.94/PKG-INFO` & `chat-box-streamlit-0.0.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-box-streamlit
-Version: 0.0.94
+Version: 0.0.95
 Summary: Seamlessly visualize engaging conversations in a sleek ChatBox.
 Home-page: https://github.com/SSK-14/Streamlit-Chatbox
 Author: SSK-14
 Author-email: sanjaykumar1481999@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `chat-box-streamlit-0.0.94/README.md` & `chat-box-streamlit-0.0.95/README.md`

 * *Files identical despite different names*

### Comparing `chat-box-streamlit-0.0.94/chat_box_streamlit/__init__.py` & `chat-box-streamlit-0.0.95/chat_box_streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `chat-box-streamlit-0.0.94/chat_box_streamlit.egg-info/PKG-INFO` & `chat-box-streamlit-0.0.95/chat_box_streamlit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-box-streamlit
-Version: 0.0.94
+Version: 0.0.95
 Summary: Seamlessly visualize engaging conversations in a sleek ChatBox.
 Home-page: https://github.com/SSK-14/Streamlit-Chatbox
 Author: SSK-14
 Author-email: sanjaykumar1481999@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `chat-box-streamlit-0.0.94/setup.py` & `chat-box-streamlit-0.0.95/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from pathlib import Path
 
 setuptools.setup(
     name="chat-box-streamlit",
-    version="0.0.94",
+    version="0.0.95",
     author="SSK-14",
     author_email="sanjaykumar1481999@gmail.com",
     description="Seamlessly visualize engaging conversations in a sleek ChatBox.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/SSK-14/Streamlit-Chatbox",
     packages=setuptools.find_packages(),
```

