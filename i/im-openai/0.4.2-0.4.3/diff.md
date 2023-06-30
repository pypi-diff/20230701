# Comparing `tmp/im_openai-0.4.2.tar.gz` & `tmp/im_openai-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "im_openai-0.4.2.tar", last modified: Thu Jun 29 23:17:01 2023, max compression
+gzip compressed data, was "im_openai-0.4.3.tar", last modified: Fri Jun 30 23:31:18 2023, max compression
```

## Comparing `im_openai-0.4.2.tar` & `im_openai-0.4.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-29 23:17:01.134739 im_openai-0.4.2/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      150 2023-06-20 23:30:14.000000 im_openai-0.4.2/AUTHORS.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3560 2023-06-22 20:28:17.000000 im_openai-0.4.2/CONTRIBUTING.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1069 2023-06-20 23:30:14.000000 im_openai-0.4.2/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)      261 2023-06-22 20:24:41.000000 im_openai-0.4.2/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2922 2023-06-29 23:17:01.135214 im_openai-0.4.2/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1553 2023-06-24 00:40:31.000000 im_openai-0.4.2/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-29 23:17:01.089197 im_openai-0.4.2/docs/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-06-20 23:30:14.000000 im_openai-0.4.2/docs/Makefile
--rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.4.2/docs/authors.rst
--rwxr-xr-x   0 vscode    (1000) vscode    (1000)     4874 2023-06-20 23:30:14.000000 im_openai-0.4.2/docs/conf.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       33 2023-06-20 23:30:14.000000 im_openai-0.4.2/docs/contributing.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.4.2/docs/history.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)      325 2023-06-20 23:30:14.000000 im_openai-0.4.2/docs/index.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1175 2023-06-20 23:30:14.000000 im_openai-0.4.2/docs/installation.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)      807 2023-06-20 23:30:14.000000 im_openai-0.4.2/docs/make.bat
--rw-r--r--   0 vscode    (1000) vscode    (1000)       26 2023-06-22 20:24:52.000000 im_openai-0.4.2/docs/readme.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       92 2023-06-20 23:30:14.000000 im_openai-0.4.2/docs/usage.rst
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-29 23:17:01.106474 im_openai-0.4.2/im_openai/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      255 2023-06-23 16:59:08.000000 im_openai-0.4.2/im_openai/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3872 2023-06-29 18:15:38.000000 im_openai-0.4.2/im_openai/client.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2039 2023-06-29 23:15:53.000000 im_openai-0.4.2/im_openai/langchain_util.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2812 2023-06-29 18:15:40.000000 im_openai-0.4.2/im_openai/patch.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      423 2023-06-23 21:56:38.000000 im_openai-0.4.2/im_openai/template.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-29 23:17:01.123010 im_openai-0.4.2/im_openai.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2922 2023-06-29 23:17:00.000000 im_openai-0.4.2/im_openai.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-06-29 23:17:01.000000 im_openai-0.4.2/im_openai.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-29 23:17:00.000000 im_openai-0.4.2/im_openai.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-29 23:17:00.000000 im_openai-0.4.2/im_openai.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2023-06-29 23:17:00.000000 im_openai-0.4.2/im_openai.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      426 2023-06-29 23:17:01.136841 im_openai-0.4.2/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1350 2023-06-29 23:16:21.000000 im_openai-0.4.2/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-29 23:17:01.132584 im_openai-0.4.2/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       39 2023-06-20 23:30:14.000000 im_openai-0.4.2/tests/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-06-20 23:30:14.000000 im_openai-0.4.2/tests/test_im_openai.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-30 23:31:18.540176 im_openai-0.4.3/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      150 2023-06-20 23:30:14.000000 im_openai-0.4.3/AUTHORS.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3560 2023-06-22 20:28:17.000000 im_openai-0.4.3/CONTRIBUTING.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1069 2023-06-20 23:30:14.000000 im_openai-0.4.3/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      261 2023-06-22 20:24:41.000000 im_openai-0.4.3/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3021 2023-06-30 23:31:18.540635 im_openai-0.4.3/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1553 2023-06-24 00:40:31.000000 im_openai-0.4.3/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-30 23:31:18.501099 im_openai-0.4.3/docs/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-06-20 23:30:14.000000 im_openai-0.4.3/docs/Makefile
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.4.3/docs/authors.rst
+-rwxr-xr-x   0 vscode    (1000) vscode    (1000)     4874 2023-06-20 23:30:14.000000 im_openai-0.4.3/docs/conf.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       33 2023-06-20 23:30:14.000000 im_openai-0.4.3/docs/contributing.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.4.3/docs/history.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      325 2023-06-20 23:30:14.000000 im_openai-0.4.3/docs/index.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1175 2023-06-20 23:30:14.000000 im_openai-0.4.3/docs/installation.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      807 2023-06-20 23:30:14.000000 im_openai-0.4.3/docs/make.bat
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       26 2023-06-22 20:24:52.000000 im_openai-0.4.3/docs/readme.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       92 2023-06-20 23:30:14.000000 im_openai-0.4.3/docs/usage.rst
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-30 23:31:18.516930 im_openai-0.4.3/im_openai/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      255 2023-06-23 16:59:08.000000 im_openai-0.4.3/im_openai/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4888 2023-06-30 23:28:41.000000 im_openai-0.4.3/im_openai/client.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2100 2023-06-30 20:10:17.000000 im_openai-0.4.3/im_openai/langchain_util.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3048 2023-06-30 23:20:06.000000 im_openai-0.4.3/im_openai/patch.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      423 2023-06-23 21:56:38.000000 im_openai-0.4.3/im_openai/template.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-30 23:31:18.532914 im_openai-0.4.3/im_openai.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3021 2023-06-30 23:31:18.000000 im_openai-0.4.3/im_openai.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-06-30 23:31:18.000000 im_openai-0.4.3/im_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-30 23:31:18.000000 im_openai-0.4.3/im_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-30 23:31:18.000000 im_openai-0.4.3/im_openai.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2023-06-30 23:31:18.000000 im_openai-0.4.3/im_openai.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      426 2023-06-30 23:31:18.542173 im_openai-0.4.3/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1350 2023-06-30 23:30:34.000000 im_openai-0.4.3/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-30 23:31:18.538463 im_openai-0.4.3/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       39 2023-06-20 23:30:14.000000 im_openai-0.4.3/tests/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-06-20 23:30:14.000000 im_openai-0.4.3/tests/test_im_openai.py
```

### Comparing `im_openai-0.4.2/CONTRIBUTING.rst` & `im_openai-0.4.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `im_openai-0.4.2/LICENSE` & `im_openai-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `im_openai-0.4.2/PKG-INFO` & `im_openai-0.4.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im_openai
-Version: 0.4.2
+Version: 0.4.3
 Summary: Wrapper library for openai to send events to the Imaginary Programming monitor
 Home-page: https://github.com/alecf/im_openai
 Author: Alec Flett
 Author-email: alec@thegp.com
 License: MIT license
 Keywords: im_openai
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -109,7 +109,13 @@
 
 - add utility for formatting langchain messages
 
 ## 0.4.2 (2023-06-29)
 
 - remove stray breakpoint
 
+## 0.4.2 (2023-06-30)
+
+- pass along chat_id
+- attempt to auto-convert langchain prompt templates
+
+
```

### Comparing `im_openai-0.4.2/README.md` & `im_openai-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `im_openai-0.4.2/docs/Makefile` & `im_openai-0.4.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `im_openai-0.4.2/docs/conf.py` & `im_openai-0.4.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.4.2/docs/installation.rst` & `im_openai-0.4.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `im_openai-0.4.2/docs/make.bat` & `im_openai-0.4.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `im_openai-0.4.2/im_openai/client.py` & `im_openai-0.4.3/im_openai/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,29 @@
+import asyncio
 import os
 import time
 import uuid
+import warnings
 from contextlib import asynccontextmanager
-from typing import List
-import asyncio
+from typing import Dict, List, TypedDict
+
 import aiohttp
-import warnings
 
 
 async def send_event(
     session: aiohttp.ClientSession,
     project_key: str,
-    api_name: str,
-    prompt_event_id: str,
-    prompt_template_text: str,
-    prompt_template_chat: List,
-    prompt_params: dict = None,
-    response: str = None,
-    response_time: float = None,
+    api_name: str | None,
+    prompt_event_id: str | None,
+    prompt_template_text: str | None,
+    prompt_template_chat: List | None,
+    prompt_params: Dict | None,
+    chat_id: str | None,
+    response: str | None = None,
+    response_time: float | None = None,
 ):
     PROMPT_REPORTING_URL = os.environ.get(
         "PROMPT_REPORTING_URL", "https://app.imaginary.dev/api/event"
     )
     event = {
         "projectKey": project_key,
         "apiName": api_name,
@@ -31,45 +33,59 @@
     }
     if prompt_template_text is not None:
         if isinstance(prompt_template_text, str):
             # first default template to just the raw text
             event["promptTemplateText"] = prompt_template_text
             if prompt_params is None and getattr(prompt_template_text, "params", None):
                 # Can be TemplateString or any other
-                prompt_params = prompt_template_text.params
+                prompt_params = prompt_template_text.params  # type: ignore
 
             # If the original template is available, send it too
             if getattr(prompt_template_text, "template", None):
-                event["promptTemplateText"] = prompt_template_text.template
+                event["promptTemplateText"] = prompt_template_text.template  # type: ignore
 
     elif prompt_template_chat is not None:
         # We're going to assume that if a non-string was passed in, then it
         # was probably a chat template, aka a chat message history
 
+        # Do any langchain conversion, in case there are langchain objects inside
+        try:
+            print("Trying langchain")
+            # import will fail if langchain is not installed
+            from .langchain_util import format_chat_template
+
+            print("Success: Converting lanchgain template")
+            prompt_template_chat = format_chat_template(prompt_template_chat)
+        except ImportError:
+            print("No langchain available")
+            pass
         # TODO: figure out template extraction for chat templates
         event["promptTemplateChat"] = prompt_template_chat
 
     if prompt_params is not None:
         event["params"] = prompt_params
     if response is not None:
         event["response"] = response
     if response_time is not None:
         event["responseTime"] = response_time
+    if chat_id is not None:
+        event["chatId"] = chat_id
 
     await session.post(PROMPT_REPORTING_URL, json=event)
 
 
 @asynccontextmanager
 async def event_session(
     project_key: str,
-    api_name: str,
-    prompt_template_text: str,
-    prompt_template_chat: List,
-    prompt_template_params: dict = None,
-    prompt_event_id: str = None,
+    api_name: str | None,
+    prompt_template_text: str | None,
+    prompt_template_chat: List | None,
+    chat_id: str | None = None,
+    prompt_template_params: dict | None = None,
+    prompt_event_id: str | None = None,
 ):
     """Context manager for sending an event to Imaginary Dev.
 
     Usage::
 
         with event_session(project_key, api_name, prompt_text, prompt_event_id) as complete_event:
             # do something
@@ -79,36 +95,38 @@
     start = time.time()
     if prompt_event_id is None:
         prompt_event_id = str(uuid.uuid4())
 
     async with aiohttp.ClientSession() as session:
         pending_events_sent = []
         first_event_sent = send_event(
-            session,
-            project_key,
-            api_name,
-            prompt_event_id,
-            prompt_template_text,
-            prompt_template_chat,
-            prompt_template_params,
+            session=session,
+            project_key=project_key,
+            api_name=api_name,
+            prompt_event_id=prompt_event_id,
+            prompt_template_text=prompt_template_text,
+            prompt_template_chat=prompt_template_chat,
+            prompt_params=prompt_template_params,
+            chat_id=chat_id,
         )
         pending_events_sent.append(first_event_sent)
 
         async def complete_event(response):
             response_time = (time.time() - start) * 1000
             second_event_sent = send_event(
-                session,
-                project_key,
-                api_name,
-                prompt_event_id,
-                prompt_template_text,
-                prompt_template_chat,
-                prompt_template_params,
-                response,
-                response_time,
+                session=session,
+                project_key=project_key,
+                api_name=api_name,
+                prompt_event_id=prompt_event_id,
+                prompt_template_text=prompt_template_text,
+                prompt_template_chat=prompt_template_chat,
+                prompt_params=prompt_template_params,
+                chat_id=chat_id,
+                response=response,
+                response_time=response_time,
             )
             pending_events_sent.append(second_event_sent)
 
         yield complete_event
         w = time.time()
         pending_events_results = await asyncio.gather(
             *pending_events_sent, return_exceptions=True
```

### Comparing `im_openai-0.4.2/im_openai/langchain_util.py` & `im_openai-0.4.3/im_openai/langchain_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,9 +45,11 @@
         return [formatted_messages]
     elif isinstance(message, BaseMessagePromptTemplate):
         vars = message.input_variables
         # create a fake dictionary mapping name -> '{name}'
         vars_as_templates = {v: f"{{{v}}}" for v in vars}
         formatted_messages = message.format_messages(**vars_as_templates)
         return format_chat_template(formatted_messages)
+    elif isinstance(message, dict):
+        return [message]
     else:
         raise ValueError(f"Got unknown type {message}")
```

### Comparing `im_openai-0.4.2/im_openai/patch.py` & `im_openai-0.4.3/im_openai/patch.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,29 @@
+import asyncio
 import os
-from typing import Callable
+from typing import Callable, List
 
 from openai import ChatCompletion, Completion
 
 from .client import event_session
-import asyncio
 
 
 def patch_openai_class(cls, get_prompt_template: Callable, get_result: Callable):
     oldcreate = cls.create
 
     async def local_create(
         cls,
         *args,
         ip_project_key=None,
-        ip_api_name=None,
-        ip_event_id=None,
-        ip_template_text=None,
-        ip_template_chat=None,
+        ip_api_name: str | None = None,
+        ip_event_id: str | None = None,
+        ip_template_text: str | None = None,
+        ip_template_chat: List | None = None,
         ip_template_params=None,
+        ip_chat_id: str | None = None,
         **kwargs
     ):
         if ip_project_key is None:
             ip_project_key = os.environ.get("PROMPT_PROJECT_KEY")
         if ip_project_key is None:
             return oldcreate(*args, **kwargs)
 
@@ -30,20 +31,21 @@
             ip_template = get_prompt_template(*args, **kwargs)
             if isinstance(ip_template, str):
                 ip_template_text = ip_template
             elif isinstance(ip_template, list):
                 ip_template_chat = ip_template
 
         async with event_session(
-            ip_project_key,
-            ip_api_name,
-            ip_template_text,
-            ip_template_chat,
-            ip_template_params,
-            ip_event_id,
+            project_key=ip_project_key,
+            api_name=ip_api_name,
+            prompt_template_text=ip_template_text,
+            prompt_template_chat=ip_template_chat,
+            chat_id=ip_chat_id,
+            prompt_template_params=ip_template_params,
+            prompt_event_id=ip_event_id,
         ) as complete_event:
             response = oldcreate(*args, **kwargs)
             await complete_event(get_result(response))
         return response
 
     oldacreate = cls.acreate
```

### Comparing `im_openai-0.4.2/im_openai.egg-info/PKG-INFO` & `im_openai-0.4.3/im_openai.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im-openai
-Version: 0.4.2
+Version: 0.4.3
 Summary: Wrapper library for openai to send events to the Imaginary Programming monitor
 Home-page: https://github.com/alecf/im_openai
 Author: Alec Flett
 Author-email: alec@thegp.com
 License: MIT license
 Keywords: im_openai
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -109,7 +109,13 @@
 
 - add utility for formatting langchain messages
 
 ## 0.4.2 (2023-06-29)
 
 - remove stray breakpoint
 
+## 0.4.2 (2023-06-30)
+
+- pass along chat_id
+- attempt to auto-convert langchain prompt templates
+
+
```

### Comparing `im_openai-0.4.2/im_openai.egg-info/SOURCES.txt` & `im_openai-0.4.3/im_openai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `im_openai-0.4.2/setup.py` & `im_openai-0.4.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords="im_openai",
     name="im_openai",
     packages=find_packages(include=["im_openai", "im_openai.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/alecf/im_openai",
-    version="0.4.2",
+    version="0.4.3",
     zip_safe=False,
 )
```

### Comparing `im_openai-0.4.2/tests/test_im_openai.py` & `im_openai-0.4.3/tests/test_im_openai.py`

 * *Files identical despite different names*

