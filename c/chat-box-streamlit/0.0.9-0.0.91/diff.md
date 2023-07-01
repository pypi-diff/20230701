# Comparing `tmp/chat-box-streamlit-0.0.9.tar.gz` & `tmp/chat-box-streamlit-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat-box-streamlit-0.0.9.tar", last modified: Sat Jul  1 09:26:40 2023, max compression
+gzip compressed data, was "chat-box-streamlit-0.0.91.tar", last modified: Sat Jul  1 09:34:09 2023, max compression
```

## Comparing `chat-box-streamlit-0.0.9.tar` & `chat-box-streamlit-0.0.91.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:26:40.624193 chat-box-streamlit-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-01 09:26:31.000000 chat-box-streamlit-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-01 09:26:31.000000 chat-box-streamlit-0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-01 09:26:40.624193 chat-box-streamlit-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-01 09:26:31.000000 chat-box-streamlit-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:26:40.624193 chat-box-streamlit-0.0.9/chat_box_streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-01 09:26:31.000000 chat-box-streamlit-0.0.9/chat_box_streamlit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:26:40.624193 chat-box-streamlit-0.0.9/chat_box_streamlit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-01 09:26:40.000000 chat-box-streamlit-0.0.9/chat_box_streamlit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-01 09:26:40.000000 chat-box-streamlit-0.0.9/chat_box_streamlit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 09:26:40.000000 chat-box-streamlit-0.0.9/chat_box_streamlit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-01 09:26:40.000000 chat-box-streamlit-0.0.9/chat_box_streamlit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-01 09:26:40.000000 chat-box-streamlit-0.0.9/chat_box_streamlit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 09:26:40.624193 chat-box-streamlit-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-01 09:26:31.000000 chat-box-streamlit-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:34:09.403161 chat-box-streamlit-0.0.91/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-01 09:33:59.000000 chat-box-streamlit-0.0.91/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-01 09:33:59.000000 chat-box-streamlit-0.0.91/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-01 09:34:09.403161 chat-box-streamlit-0.0.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-01 09:33:59.000000 chat-box-streamlit-0.0.91/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:34:09.403161 chat-box-streamlit-0.0.91/chat_box_streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-01 09:33:59.000000 chat-box-streamlit-0.0.91/chat_box_streamlit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:34:09.403161 chat-box-streamlit-0.0.91/chat_box_streamlit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-01 09:34:09.000000 chat-box-streamlit-0.0.91/chat_box_streamlit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-01 09:34:09.000000 chat-box-streamlit-0.0.91/chat_box_streamlit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 09:34:09.000000 chat-box-streamlit-0.0.91/chat_box_streamlit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-01 09:34:09.000000 chat-box-streamlit-0.0.91/chat_box_streamlit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-01 09:34:09.000000 chat-box-streamlit-0.0.91/chat_box_streamlit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 09:34:09.403161 chat-box-streamlit-0.0.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-01 09:33:59.000000 chat-box-streamlit-0.0.91/setup.py
```

### Comparing `chat-box-streamlit-0.0.9/LICENSE` & `chat-box-streamlit-0.0.91/LICENSE`

 * *Files identical despite different names*

### Comparing `chat-box-streamlit-0.0.9/PKG-INFO` & `chat-box-streamlit-0.0.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-box-streamlit
-Version: 0.0.9
+Version: 0.0.91
 Summary: Seamlessly visualize engaging conversations in a sleek ChatBox.
 Home-page: https://github.com/SSK-14/Streamlit-Chatbox
 Author: SSK-14
 Author-email: sanjaykumar1481999@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `chat-box-streamlit-0.0.9/README.md` & `chat-box-streamlit-0.0.91/README.md`

 * *Files identical despite different names*

### Comparing `chat-box-streamlit-0.0.9/chat_box_streamlit/__init__.py` & `chat-box-streamlit-0.0.91/chat_box_streamlit/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import streamlit as st
 import streamlit.components.v1 as components
 
-_RELEASE = False
+_RELEASE = True
 
 if not _RELEASE:
     _component_func = components.declare_component(
         "chat_box_streamlit",
         url="http://localhost:5173",
     )
 else:
```

### Comparing `chat-box-streamlit-0.0.9/chat_box_streamlit.egg-info/PKG-INFO` & `chat-box-streamlit-0.0.91/chat_box_streamlit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-box-streamlit
-Version: 0.0.9
+Version: 0.0.91
 Summary: Seamlessly visualize engaging conversations in a sleek ChatBox.
 Home-page: https://github.com/SSK-14/Streamlit-Chatbox
 Author: SSK-14
 Author-email: sanjaykumar1481999@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `chat-box-streamlit-0.0.9/setup.py` & `chat-box-streamlit-0.0.91/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 from pathlib import Path
 
 
 setuptools.setup(
     name="chat-box-streamlit",
-    version="0.0.9",
+    version="0.0.91",
     author="SSK-14",
     author_email="sanjaykumar1481999@gmail.com",
     description="Seamlessly visualize engaging conversations in a sleek ChatBox.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/SSK-14/Streamlit-Chatbox",
     packages=setuptools.find_packages(),
```

