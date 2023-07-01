# Comparing `tmp/chat-box-streamlit-0.0.8.tar.gz` & `tmp/chat-box-streamlit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat-box-streamlit-0.0.8.tar", last modified: Sun Jun 25 07:28:30 2023, max compression
+gzip compressed data, was "chat-box-streamlit-0.0.9.tar", last modified: Sat Jul  1 09:26:40 2023, max compression
```

## Comparing `chat-box-streamlit-0.0.8.tar` & `chat-box-streamlit-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:28:30.051962 chat-box-streamlit-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-25 07:28:21.000000 chat-box-streamlit-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-25 07:28:21.000000 chat-box-streamlit-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-06-25 07:28:30.051962 chat-box-streamlit-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-25 07:28:21.000000 chat-box-streamlit-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:28:30.051962 chat-box-streamlit-0.0.8/chat_box_streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-25 07:28:21.000000 chat-box-streamlit-0.0.8/chat_box_streamlit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:28:30.051962 chat-box-streamlit-0.0.8/chat_box_streamlit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-06-25 07:28:29.000000 chat-box-streamlit-0.0.8/chat_box_streamlit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-25 07:28:30.000000 chat-box-streamlit-0.0.8/chat_box_streamlit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 07:28:29.000000 chat-box-streamlit-0.0.8/chat_box_streamlit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-25 07:28:29.000000 chat-box-streamlit-0.0.8/chat_box_streamlit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-25 07:28:29.000000 chat-box-streamlit-0.0.8/chat_box_streamlit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 07:28:30.051962 chat-box-streamlit-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-25 07:28:21.000000 chat-box-streamlit-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:26:40.624193 chat-box-streamlit-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-01 09:26:31.000000 chat-box-streamlit-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-01 09:26:31.000000 chat-box-streamlit-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-01 09:26:40.624193 chat-box-streamlit-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-01 09:26:31.000000 chat-box-streamlit-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:26:40.624193 chat-box-streamlit-0.0.9/chat_box_streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-01 09:26:31.000000 chat-box-streamlit-0.0.9/chat_box_streamlit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:26:40.624193 chat-box-streamlit-0.0.9/chat_box_streamlit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-01 09:26:40.000000 chat-box-streamlit-0.0.9/chat_box_streamlit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-01 09:26:40.000000 chat-box-streamlit-0.0.9/chat_box_streamlit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 09:26:40.000000 chat-box-streamlit-0.0.9/chat_box_streamlit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-01 09:26:40.000000 chat-box-streamlit-0.0.9/chat_box_streamlit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-01 09:26:40.000000 chat-box-streamlit-0.0.9/chat_box_streamlit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 09:26:40.624193 chat-box-streamlit-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-01 09:26:31.000000 chat-box-streamlit-0.0.9/setup.py
```

### Comparing `chat-box-streamlit-0.0.8/LICENSE` & `chat-box-streamlit-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chat-box-streamlit-0.0.8/PKG-INFO` & `chat-box-streamlit-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-box-streamlit
-Version: 0.0.8
+Version: 0.0.9
 Summary: Seamlessly visualize engaging conversations in a sleek ChatBox.
 Home-page: https://github.com/SSK-14/Streamlit-Chatbox
 Author: SSK-14
 Author-email: sanjaykumar1481999@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `chat-box-streamlit-0.0.8/README.md` & `chat-box-streamlit-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `chat-box-streamlit-0.0.8/chat_box_streamlit/__init__.py` & `chat-box-streamlit-0.0.9/chat_box_streamlit/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 import os
 import streamlit as st
 import streamlit.components.v1 as components
 
-
-_RELEASE = True
+_RELEASE = False
 
 if not _RELEASE:
     _component_func = components.declare_component(
         "chat_box_streamlit",
-        url="http://localhost:3001",
+        url="http://localhost:5173",
     )
 else:
     parent_dir = os.path.dirname(os.path.abspath(__file__))
-    build_dir = os.path.join(parent_dir, "frontend/build")
+    build_dir = os.path.join(parent_dir, "frontend/dist")
     _component_func = components.declare_component("chat_box_streamlit", path=build_dir)
 
 
 def st_message(isLeft=True, message="", loading=False, loadingText="Loading...", placeholder="Enter your input", height=500, key=None):
     component_value =  _component_func(component="message", isLeft=isLeft, message=message, placeholder=placeholder, loading=loading, loadingText=loadingText, height=height, key=key)
     return component_value
 
 def st_input(placeholder="Enter your input", loading=False, loadingText="Loading...", rows=1, key=None):
     component_value = _component_func(component="input", placeholder=placeholder, rows=rows, loading=loading, loadingText=loadingText, key=key)
     return component_value
 
 def st_display_chat(leftMessages = [], rightMessages=[], height=500, rows=1, key=None):
     component_value = _component_func(component="", leftMessages=leftMessages, rightMessages=rightMessages, rows=rows, height=height, key=key)
-    return component_value
+    return component_value
+
+if not _RELEASE:
+    st.title("Chat Box Streamlit")
+    st.write("This is a demo of the chat box component")
+    st.write("### Input:")
+    keyword = st_input(placeholder="Enter your input", loading=False, loadingText="Loading...", rows=1, key=None)
+    st.write("### Messages:")
+    st_display_chat(leftMessages = ["Hello", "How are you?"], rightMessages=["Hi", "I am fine"], height=500, rows=1, key=None)
+
```

### Comparing `chat-box-streamlit-0.0.8/chat_box_streamlit.egg-info/PKG-INFO` & `chat-box-streamlit-0.0.9/chat_box_streamlit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-box-streamlit
-Version: 0.0.8
+Version: 0.0.9
 Summary: Seamlessly visualize engaging conversations in a sleek ChatBox.
 Home-page: https://github.com/SSK-14/Streamlit-Chatbox
 Author: SSK-14
 Author-email: sanjaykumar1481999@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `chat-box-streamlit-0.0.8/setup.py` & `chat-box-streamlit-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 from pathlib import Path
 
 
 setuptools.setup(
     name="chat-box-streamlit",
-    version="0.0.8",
+    version="0.0.9",
     author="SSK-14",
     author_email="sanjaykumar1481999@gmail.com",
     description="Seamlessly visualize engaging conversations in a sleek ChatBox.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/SSK-14/Streamlit-Chatbox",
     packages=setuptools.find_packages(),
```

