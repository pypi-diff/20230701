# Comparing `tmp/chat-box-streamlit-0.0.91.tar.gz` & `tmp/chat-box-streamlit-0.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat-box-streamlit-0.0.91.tar", last modified: Sat Jul  1 09:34:09 2023, max compression
+gzip compressed data, was "chat-box-streamlit-0.0.92.tar", last modified: Sat Jul  1 10:26:48 2023, max compression
```

## Comparing `chat-box-streamlit-0.0.91.tar` & `chat-box-streamlit-0.0.92.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:34:09.403161 chat-box-streamlit-0.0.91/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-01 09:33:59.000000 chat-box-streamlit-0.0.91/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-01 09:33:59.000000 chat-box-streamlit-0.0.91/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-01 09:34:09.403161 chat-box-streamlit-0.0.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-01 09:33:59.000000 chat-box-streamlit-0.0.91/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:34:09.403161 chat-box-streamlit-0.0.91/chat_box_streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-01 09:33:59.000000 chat-box-streamlit-0.0.91/chat_box_streamlit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:34:09.403161 chat-box-streamlit-0.0.91/chat_box_streamlit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-01 09:34:09.000000 chat-box-streamlit-0.0.91/chat_box_streamlit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-01 09:34:09.000000 chat-box-streamlit-0.0.91/chat_box_streamlit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 09:34:09.000000 chat-box-streamlit-0.0.91/chat_box_streamlit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-01 09:34:09.000000 chat-box-streamlit-0.0.91/chat_box_streamlit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-01 09:34:09.000000 chat-box-streamlit-0.0.91/chat_box_streamlit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 09:34:09.403161 chat-box-streamlit-0.0.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-01 09:33:59.000000 chat-box-streamlit-0.0.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:26:48.648659 chat-box-streamlit-0.0.92/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-01 10:26:40.000000 chat-box-streamlit-0.0.92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-01 10:26:40.000000 chat-box-streamlit-0.0.92/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-01 10:26:48.648659 chat-box-streamlit-0.0.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-01 10:26:40.000000 chat-box-streamlit-0.0.92/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:26:48.644659 chat-box-streamlit-0.0.92/chat_box_streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-01 10:26:40.000000 chat-box-streamlit-0.0.92/chat_box_streamlit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:26:48.644659 chat-box-streamlit-0.0.92/chat_box_streamlit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-01 10:26:48.000000 chat-box-streamlit-0.0.92/chat_box_streamlit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-01 10:26:48.000000 chat-box-streamlit-0.0.92/chat_box_streamlit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 10:26:48.000000 chat-box-streamlit-0.0.92/chat_box_streamlit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-01 10:26:48.000000 chat-box-streamlit-0.0.92/chat_box_streamlit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-01 10:26:48.000000 chat-box-streamlit-0.0.92/chat_box_streamlit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 10:26:48.648659 chat-box-streamlit-0.0.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-01 10:26:40.000000 chat-box-streamlit-0.0.92/setup.py
```

### Comparing `chat-box-streamlit-0.0.91/LICENSE` & `chat-box-streamlit-0.0.92/LICENSE`

 * *Files identical despite different names*

### Comparing `chat-box-streamlit-0.0.91/PKG-INFO` & `chat-box-streamlit-0.0.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-box-streamlit
-Version: 0.0.91
+Version: 0.0.92
 Summary: Seamlessly visualize engaging conversations in a sleek ChatBox.
 Home-page: https://github.com/SSK-14/Streamlit-Chatbox
 Author: SSK-14
 Author-email: sanjaykumar1481999@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `chat-box-streamlit-0.0.91/README.md` & `chat-box-streamlit-0.0.92/README.md`

 * *Files identical despite different names*

### Comparing `chat-box-streamlit-0.0.91/chat_box_streamlit/__init__.py` & `chat-box-streamlit-0.0.92/chat_box_streamlit/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import os
 import streamlit as st
 import streamlit.components.v1 as components
 
 _RELEASE = True
 
 if not _RELEASE:
-    _component_func = components.declare_component(
+    _chat_box_streamlit = components.declare_component(
         "chat_box_streamlit",
         url="http://localhost:5173",
     )
 else:
     parent_dir = os.path.dirname(os.path.abspath(__file__))
     build_dir = os.path.join(parent_dir, "frontend/dist")
-    _component_func = components.declare_component("chat_box_streamlit", path=build_dir)
+    _chat_box_streamlit = components.declare_component("chat_box_streamlit", path=build_dir)
 
 
 def st_message(isLeft=True, message="", loading=False, loadingText="Loading...", placeholder="Enter your input", height=500, key=None):
-    component_value =  _component_func(component="message", isLeft=isLeft, message=message, placeholder=placeholder, loading=loading, loadingText=loadingText, height=height, key=key)
+    component_value =  _chat_box_streamlit(component="message", isLeft=isLeft, message=message, placeholder=placeholder, loading=loading, loadingText=loadingText, height=height, key=key)
     return component_value
 
 def st_input(placeholder="Enter your input", loading=False, loadingText="Loading...", rows=1, key=None):
-    component_value = _component_func(component="input", placeholder=placeholder, rows=rows, loading=loading, loadingText=loadingText, key=key)
+    component_value = _chat_box_streamlit(component="input", placeholder=placeholder, rows=rows, loading=loading, loadingText=loadingText, key=key)
     return component_value
 
 def st_display_chat(leftMessages = [], rightMessages=[], height=500, rows=1, key=None):
-    component_value = _component_func(component="", leftMessages=leftMessages, rightMessages=rightMessages, rows=rows, height=height, key=key)
+    component_value = _chat_box_streamlit(component="", leftMessages=leftMessages, rightMessages=rightMessages, rows=rows, height=height, key=key)
     return component_value
 
 if not _RELEASE:
     st.title("Chat Box Streamlit")
     st.write("This is a demo of the chat box component")
     st.write("### Input:")
     keyword = st_input(placeholder="Enter your input", loading=False, loadingText="Loading...", rows=1, key=None)
```

### Comparing `chat-box-streamlit-0.0.91/chat_box_streamlit.egg-info/PKG-INFO` & `chat-box-streamlit-0.0.92/chat_box_streamlit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-box-streamlit
-Version: 0.0.91
+Version: 0.0.92
 Summary: Seamlessly visualize engaging conversations in a sleek ChatBox.
 Home-page: https://github.com/SSK-14/Streamlit-Chatbox
 Author: SSK-14
 Author-email: sanjaykumar1481999@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `chat-box-streamlit-0.0.91/setup.py` & `chat-box-streamlit-0.0.92/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 from pathlib import Path
 
 
 setuptools.setup(
     name="chat-box-streamlit",
-    version="0.0.91",
+    version="0.0.92",
     author="SSK-14",
     author_email="sanjaykumar1481999@gmail.com",
     description="Seamlessly visualize engaging conversations in a sleek ChatBox.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/SSK-14/Streamlit-Chatbox",
     packages=setuptools.find_packages(),
```

