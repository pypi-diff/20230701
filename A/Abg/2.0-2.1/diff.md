# Comparing `tmp/Abg-2.0.tar.gz` & `tmp/Abg-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Abg-2.0.tar", last modified: Mon Jun 26 02:44:09 2023, max compression
+gzip compressed data, was "Abg-2.1.tar", last modified: Sat Jul  1 13:41:32 2023, max compression
```

## Comparing `Abg-2.0.tar` & `Abg-2.1.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:44:09.681949 Abg-2.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:44:09.677948 Abg-2.0/Abg/
--rw-r--r--   0 root         (0) root         (0)      242 2023-06-26 02:43:45.000000 Abg-2.0/Abg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:44:09.677948 Abg-2.0/Abg/chat_status/
--rw-r--r--   0 root         (0) root         (0)      109 2023-06-26 02:43:45.000000 Abg-2.0/Abg/chat_status/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5154 2023-06-26 02:43:45.000000 Abg-2.0/Abg/chat_status/chat_status.py
--rw-r--r--   0 root         (0) root         (0)     2348 2023-06-26 02:43:45.000000 Abg-2.0/Abg/chat_status/custom_filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:44:09.681949 Abg-2.0/Abg/helpers/
--rw-r--r--   0 root         (0) root         (0)      784 2023-06-26 02:43:45.000000 Abg-2.0/Abg/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3179 2023-06-26 02:43:45.000000 Abg-2.0/Abg/helpers/helpers.py
--rw-r--r--   0 root         (0) root         (0)     1596 2023-06-26 02:43:45.000000 Abg-2.0/Abg/helpers/http_helper.py
--rw-r--r--   0 root         (0) root         (0)     2591 2023-06-26 02:43:45.000000 Abg-2.0/Abg/helpers/human_read.py
--rw-r--r--   0 root         (0) root         (0)     1279 2023-06-26 02:43:45.000000 Abg-2.0/Abg/helpers/parser.py
--rw-r--r--   0 root         (0) root         (0)     2533 2023-06-26 02:43:45.000000 Abg-2.0/Abg/helpers/pyro_progress.py
--rw-r--r--   0 root         (0) root         (0)     2834 2023-06-26 02:43:45.000000 Abg-2.0/Abg/helpers/ratelimit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:44:09.681949 Abg-2.0/Abg/inline/
--rw-r--r--   0 root         (0) root         (0)      274 2023-06-26 02:43:45.000000 Abg-2.0/Abg/inline/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6105 2023-06-26 02:43:45.000000 Abg-2.0/Abg/inline/inline_keyboard.py
--rw-r--r--   0 root         (0) root         (0)     4267 2023-06-26 02:43:45.000000 Abg-2.0/Abg/inline/inline_pagination_keyboard.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-06-26 02:43:45.000000 Abg-2.0/Abg/inline/reply_keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:44:09.681949 Abg-2.0/Abg/patch/
--rw-r--r--   0 root         (0) root         (0)       79 2023-06-26 02:43:45.000000 Abg-2.0/Abg/patch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:44:09.681949 Abg-2.0/Abg/patch/bound/
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-26 02:43:45.000000 Abg-2.0/Abg/patch/bound/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11979 2023-06-26 02:43:45.000000 Abg-2.0/Abg/patch/bound/message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:44:09.681949 Abg-2.0/Abg/patch/listen/
--rw-r--r--   0 root         (0) root         (0)       55 2023-06-26 02:43:45.000000 Abg-2.0/Abg/patch/listen/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12016 2023-06-26 02:43:45.000000 Abg-2.0/Abg/patch/listen/listen.py
--rw-r--r--   0 root         (0) root         (0)      776 2023-06-26 02:43:45.000000 Abg-2.0/Abg/patch/listen/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:44:09.681949 Abg-2.0/Abg/patch/methods/
--rw-r--r--   0 root         (0) root         (0)      127 2023-06-26 02:43:45.000000 Abg-2.0/Abg/patch/methods/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2172 2023-06-26 02:43:45.000000 Abg-2.0/Abg/patch/methods/edit_message_text.py
--rw-r--r--   0 root         (0) root         (0)     1713 2023-06-26 02:43:45.000000 Abg-2.0/Abg/patch/methods/send_as_file.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-06-26 02:43:45.000000 Abg-2.0/Abg/patch/methods/send_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 02:44:09.677948 Abg-2.0/Abg.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4988 2023-06-26 02:44:09.000000 Abg-2.0/Abg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      830 2023-06-26 02:44:09.000000 Abg-2.0/Abg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 02:44:09.000000 Abg-2.0/Abg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-26 02:44:09.000000 Abg-2.0/Abg.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     4988 2023-06-26 02:44:09.681949 Abg-2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2460 2023-06-26 02:43:45.000000 Abg-2.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 02:44:09.681949 Abg-2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2994 2023-06-26 02:43:45.000000 Abg-2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 13:41:32.005030 Abg-2.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 13:41:32.001030 Abg-2.1/Abg/
+-rw-r--r--   0 root         (0) root         (0)      125 2023-07-01 13:41:05.000000 Abg-2.1/Abg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 13:41:32.001030 Abg-2.1/Abg/chat_status/
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-01 13:41:05.000000 Abg-2.1/Abg/chat_status/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5154 2023-07-01 13:41:05.000000 Abg-2.1/Abg/chat_status/chat_status.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2023-07-01 13:41:05.000000 Abg-2.1/Abg/chat_status/custom_filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 13:41:32.005030 Abg-2.1/Abg/helpers/
+-rw-r--r--   0 root         (0) root         (0)      831 2023-07-01 13:41:05.000000 Abg-2.1/Abg/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3179 2023-07-01 13:41:05.000000 Abg-2.1/Abg/helpers/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2023-07-01 13:41:05.000000 Abg-2.1/Abg/helpers/http_helper.py
+-rw-r--r--   0 root         (0) root         (0)     2589 2023-07-01 13:41:05.000000 Abg-2.1/Abg/helpers/human_read.py
+-rw-r--r--   0 root         (0) root         (0)     7350 2023-07-01 13:41:05.000000 Abg-2.1/Abg/helpers/msg_types.py
+-rw-r--r--   0 root         (0) root         (0)     1279 2023-07-01 13:41:05.000000 Abg-2.1/Abg/helpers/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2533 2023-07-01 13:41:05.000000 Abg-2.1/Abg/helpers/pyro_progress.py
+-rw-r--r--   0 root         (0) root         (0)     2834 2023-07-01 13:41:05.000000 Abg-2.1/Abg/helpers/ratelimit.py
+-rw-r--r--   0 root         (0) root         (0)     5357 2023-07-01 13:41:05.000000 Abg-2.1/Abg/helpers/string.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 13:41:32.005030 Abg-2.1/Abg/inline/
+-rw-r--r--   0 root         (0) root         (0)      274 2023-07-01 13:41:05.000000 Abg-2.1/Abg/inline/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6105 2023-07-01 13:41:05.000000 Abg-2.1/Abg/inline/inline_keyboard.py
+-rw-r--r--   0 root         (0) root         (0)     4267 2023-07-01 13:41:05.000000 Abg-2.1/Abg/inline/inline_pagination_keyboard.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-07-01 13:41:05.000000 Abg-2.1/Abg/inline/reply_keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 13:41:32.005030 Abg-2.1/Abg/patch/
+-rw-r--r--   0 root         (0) root         (0)       79 2023-07-01 13:41:05.000000 Abg-2.1/Abg/patch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 13:41:32.005030 Abg-2.1/Abg/patch/bound/
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-01 13:41:05.000000 Abg-2.1/Abg/patch/bound/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11979 2023-07-01 13:41:05.000000 Abg-2.1/Abg/patch/bound/message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 13:41:32.005030 Abg-2.1/Abg/patch/listen/
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-01 13:41:05.000000 Abg-2.1/Abg/patch/listen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12016 2023-07-01 13:41:05.000000 Abg-2.1/Abg/patch/listen/listen.py
+-rw-r--r--   0 root         (0) root         (0)      776 2023-07-01 13:41:05.000000 Abg-2.1/Abg/patch/listen/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 13:41:32.005030 Abg-2.1/Abg/patch/methods/
+-rw-r--r--   0 root         (0) root         (0)      127 2023-07-01 13:41:05.000000 Abg-2.1/Abg/patch/methods/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2172 2023-07-01 13:41:05.000000 Abg-2.1/Abg/patch/methods/edit_message_text.py
+-rw-r--r--   0 root         (0) root         (0)     1713 2023-07-01 13:41:05.000000 Abg-2.1/Abg/patch/methods/send_as_file.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-07-01 13:41:05.000000 Abg-2.1/Abg/patch/methods/send_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 13:41:32.001030 Abg-2.1/Abg.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4948 2023-07-01 13:41:31.000000 Abg-2.1/Abg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      877 2023-07-01 13:41:31.000000 Abg-2.1/Abg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-01 13:41:31.000000 Abg-2.1/Abg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-01 13:41:31.000000 Abg-2.1/Abg.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     4948 2023-07-01 13:41:32.005030 Abg-2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2420 2023-07-01 13:41:05.000000 Abg-2.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-01 13:41:32.005030 Abg-2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2994 2023-07-01 13:41:05.000000 Abg-2.1/setup.py
```

### Comparing `Abg-2.0/Abg/chat_status/chat_status.py` & `Abg-2.1/Abg/chat_status/chat_status.py`

 * *Files identical despite different names*

### Comparing `Abg-2.0/Abg/chat_status/custom_filters.py` & `Abg-2.1/Abg/chat_status/custom_filters.py`

 * *Files identical despite different names*

### Comparing `Abg-2.0/Abg/helpers/__init__.py` & `Abg-2.1/Abg/helpers/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,7 +14,9 @@
 
 along with Abg.  If not, see <https://www.gnu.org/licenses/>.
 """
 from .helpers import *
 from .human_read import *
 from .parser import *
 from .pyro_progress import *
+from .msg_types import *
+from .string import *
```

### Comparing `Abg-2.0/Abg/helpers/helpers.py` & `Abg-2.1/Abg/helpers/helpers.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,48 @@
                 btn(button, button) if type(button) == str else btn(*button)
             )  # InlineKeyboardButton
             line.append(button)
         lines.append(line)
     return InlineKeyboardMarkup(inline_keyboard=lines)
     # return {'inline_keyboard': lines}
 
+def ikb2(rows=None, back=False, todo="start_back"):
+    # rows = pass the rows
+    # back - if want to make back button
+    # todo - callback data of back button
+
+    if rows is None:
+        rows = []
+    lines = []
+    try:
+        for row in rows:
+            line = []
+            for button in row:
+                btn_text = button.split(".")[1].upper()
+                button = btn(btn_text, button)  # InlineKeyboardButton
+                line.append(button)
+            lines.append(line)
+    except AttributeError:
+        for row in rows:
+            line = []
+            for button in row:
+                button = btn(*button)  # Will make the kb which don't have "." in them
+                line.append(button)
+            lines.append(line)
+    except TypeError:
+        # make a code to handel that error
+        line = []
+        for button in rows:
+            button = btn(*button)  # InlineKeyboardButton
+            line.append(button)
+        lines.append(line)
+    if back:
+        back_btn = [(btn("« ʙᴀᴄᴋ", todo))]
+        lines.append(back_btn)
+    return InlineKeyboardMarkup(inline_keyboard=lines)
 
 def btn(text, value, type="callback_data"):
     return InlineKeyboardButton(text, **{type: value})
     # return {'text': text, type: value}
 
 
 # The inverse of above
@@ -80,41 +114,7 @@
     return ForceReply(selective=selective)
 
 
 def array_chunk(input, size):
     return [input[i : i + size] for i in range(0, len(input), size)]
 
 
-def ikb2(rows=None, back=False, todo="start_back"):
-    # rows = pass the rows
-    # back - if want to make back button
-    # todo - callback data of back button
-
-    if rows is None:
-        rows = []
-    lines = []
-    try:
-        for row in rows:
-            line = []
-            for button in row:
-                btn_text = button.split(".")[1].upper()
-                button = btn(btn_text, button)  # InlineKeyboardButton
-                line.append(button)
-            lines.append(line)
-    except AttributeError:
-        for row in rows:
-            line = []
-            for button in row:
-                button = btn(*button)  # Will make the kb which don't have "." in them
-                line.append(button)
-            lines.append(line)
-    except TypeError:
-        # make a code to handel that error
-        line = []
-        for button in rows:
-            button = btn(*button)  # InlineKeyboardButton
-            line.append(button)
-        lines.append(line)
-    if back:
-        back_btn = [(btn("« ʙᴀᴄᴋ", todo))]
-        lines.append(back_btn)
-    return InlineKeyboardMarkup(inline_keyboard=lines)
```

### Comparing `Abg-2.0/Abg/helpers/http_helper.py` & `Abg-2.1/Abg/helpers/http_helper.py`

 * *Files identical despite different names*

### Comparing `Abg-2.0/Abg/helpers/human_read.py` & `Abg-2.1/Abg/helpers/human_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 SIZE_UNITS = ["B", "KB", "MB", "GB", "TB", "PB"]
 
 
 def get_readable_time(seconds: int) -> str:
     count = 0
     ping_time = ""
     time_list = []
-    time_suffix_list = ["sᴇᴄ.", "ᴍɪɴ.", "ʜᴏᴜʀ", "ᴅᴀʏ", "ᴡᴇᴇᴋ", "ᴍᴏɴᴛʜ", "ʏᴇᴀʀ"]
+    time_suffix_list = ["sᴇᴄ", "ᴍɪɴ", "ʜᴏᴜʀ", "ᴅᴀʏ", "ᴡᴇᴇᴋ", "ᴍᴏɴᴛʜ", "ʏᴇᴀʀ"]
     while count < 4:
         count += 1
         remainder, result = divmod(seconds, 60) if count < 3 else divmod(seconds, 24)
         if seconds == 0 and remainder == 0:
             break
         time_list.append(int(result))
         seconds = int(remainder)
```

### Comparing `Abg-2.0/Abg/helpers/parser.py` & `Abg-2.1/Abg/helpers/parser.py`

 * *Files identical despite different names*

### Comparing `Abg-2.0/Abg/helpers/pyro_progress.py` & `Abg-2.1/Abg/helpers/pyro_progress.py`

 * *Files identical despite different names*

### Comparing `Abg-2.0/Abg/helpers/ratelimit.py` & `Abg-2.1/Abg/helpers/ratelimit.py`

 * *Files identical despite different names*

### Comparing `Abg-2.0/Abg/inline/inline_keyboard.py` & `Abg-2.1/Abg/inline/inline_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-2.0/Abg/inline/inline_pagination_keyboard.py` & `Abg-2.1/Abg/inline/inline_pagination_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-2.0/Abg/inline/reply_keyboard.py` & `Abg-2.1/Abg/inline/reply_keyboard.py`

 * *Files identical despite different names*

### Comparing `Abg-2.0/Abg/patch/bound/message.py` & `Abg-2.1/Abg/patch/bound/message.py`

 * *Files identical despite different names*

### Comparing `Abg-2.0/Abg/patch/listen/listen.py` & `Abg-2.1/Abg/patch/listen/listen.py`

 * *Files identical despite different names*

### Comparing `Abg-2.0/Abg/patch/listen/utils.py` & `Abg-2.1/Abg/patch/listen/utils.py`

 * *Files identical despite different names*

### Comparing `Abg-2.0/Abg/patch/methods/edit_message_text.py` & `Abg-2.1/Abg/patch/methods/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `Abg-2.0/Abg/patch/methods/send_as_file.py` & `Abg-2.1/Abg/patch/methods/send_as_file.py`

 * *Files identical despite different names*

### Comparing `Abg-2.0/Abg/patch/methods/send_message.py` & `Abg-2.1/Abg/patch/methods/send_message.py`

 * *Files identical despite different names*

### Comparing `Abg-2.0/Abg.egg-info/PKG-INFO` & `Abg-2.1/Abg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: Abg
-Version: 2.0
+Version: 2.1
 Summary: Telegram bot helpers
 Home-page: https://github.com/Abishnoi69
 Author: Abishnoi1M
 Author-email: Abishnoi69@Abg.org
 License: MIT
 Download-URL: https://github.com/Abishnoi69/Abg/releases/latest
 Project-URL: Tracker, https://github.com/Abishnoi69/Abg/issues
 Project-URL: Community, https://t.me/Abgpy
 Project-URL: Source, https://github.com/Abishnoi69/Abg
 Project-URL: Documentation, https://github.com/Abishnoi69/Abg/tree/master/doce
 Description: # ᴀʙɢ :->
         > 
-        ### • Conversation ingram
+        ### • Conversation
         
         ```python
         from pyrogram import filters, Client
         from pyrogram.types import Message
         from Abg import patch  # type : ignore
         
         app = Client("my_account")
@@ -97,15 +97,15 @@
         ```bash
         pip3 install Abg
         ```
         
         ━━━━━━━━━━━━━━━━━━━━
         ## ɴᴏᴛᴇ :->
         
-        - This library is made for my personal Project so don't take it deeply  [you can use this 24*7 running ] 
+        - This library is made for my personal Project so don't take it deeply  
         - My Project [@AbgRobot](https://t.me/AbgRobot) / [@Exon_Robot](https://t.me/Exon_Robot) & [@ExonMusicBot](https://t.me/ExonMusicBot)
         
         - ᴇɴᴊᴏʏ ʙᴀʙʏ ♡ 
         
         ━━━━━━━━━━━━━━━━━━━━
```

### Comparing `Abg-2.0/Abg.egg-info/SOURCES.txt` & `Abg-2.1/Abg.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 Abg/chat_status/__init__.py
 Abg/chat_status/chat_status.py
 Abg/chat_status/custom_filters.py
 Abg/helpers/__init__.py
 Abg/helpers/helpers.py
 Abg/helpers/http_helper.py
 Abg/helpers/human_read.py
+Abg/helpers/msg_types.py
 Abg/helpers/parser.py
 Abg/helpers/pyro_progress.py
 Abg/helpers/ratelimit.py
+Abg/helpers/string.py
 Abg/inline/__init__.py
 Abg/inline/inline_keyboard.py
 Abg/inline/inline_pagination_keyboard.py
 Abg/inline/reply_keyboard.py
 Abg/patch/__init__.py
 Abg/patch/bound/__init__.py
 Abg/patch/bound/message.py
```

### Comparing `Abg-2.0/PKG-INFO` & `Abg-2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: Abg
-Version: 2.0
+Version: 2.1
 Summary: Telegram bot helpers
 Home-page: https://github.com/Abishnoi69
 Author: Abishnoi1M
 Author-email: Abishnoi69@Abg.org
 License: MIT
 Download-URL: https://github.com/Abishnoi69/Abg/releases/latest
 Project-URL: Tracker, https://github.com/Abishnoi69/Abg/issues
 Project-URL: Community, https://t.me/Abgpy
 Project-URL: Source, https://github.com/Abishnoi69/Abg
 Project-URL: Documentation, https://github.com/Abishnoi69/Abg/tree/master/doce
 Description: # ᴀʙɢ :->
         > 
-        ### • Conversation ingram
+        ### • Conversation
         
         ```python
         from pyrogram import filters, Client
         from pyrogram.types import Message
         from Abg import patch  # type : ignore
         
         app = Client("my_account")
@@ -97,15 +97,15 @@
         ```bash
         pip3 install Abg
         ```
         
         ━━━━━━━━━━━━━━━━━━━━
         ## ɴᴏᴛᴇ :->
         
-        - This library is made for my personal Project so don't take it deeply  [you can use this 24*7 running ] 
+        - This library is made for my personal Project so don't take it deeply  
         - My Project [@AbgRobot](https://t.me/AbgRobot) / [@Exon_Robot](https://t.me/Exon_Robot) & [@ExonMusicBot](https://t.me/ExonMusicBot)
         
         - ᴇɴᴊᴏʏ ʙᴀʙʏ ♡ 
         
         ━━━━━━━━━━━━━━━━━━━━
```

### Comparing `Abg-2.0/README.md` & `Abg-2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # ᴀʙɢ :->
 > 
-### • Conversation ingram
+### • Conversation
 
 ```python
 from pyrogram import filters, Client
 from pyrogram.types import Message
 from Abg import patch  # type : ignore
 
 app = Client("my_account")
@@ -84,14 +84,14 @@
 ```bash
 pip3 install Abg
 ```
 
 ━━━━━━━━━━━━━━━━━━━━
 ## ɴᴏᴛᴇ :->
 
-- This library is made for my personal Project so don't take it deeply  [you can use this 24*7 running ] 
+- This library is made for my personal Project so don't take it deeply  
 - My Project [@AbgRobot](https://t.me/AbgRobot) / [@Exon_Robot](https://t.me/Exon_Robot) & [@ExonMusicBot](https://t.me/ExonMusicBot)
 
 - ᴇɴᴊᴏʏ ʙᴀʙʏ ♡ 
 
 ━━━━━━━━━━━━━━━━━━━━
```

### Comparing `Abg-2.0/setup.py` & `Abg-2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     with open(file, encoding="utf-8") as r:
         return [i.strip() for i in r]
 """
 
 setuptools.setup(
     name="Abg",
     packages=setuptools.find_packages(),
-    version="2.0",
+    version="2.1",
     description="Telegram bot helpers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Abishnoi69",
     download_url="https://github.com/Abishnoi69/Abg/releases/latest",
     author="Abishnoi1M",
     author_email="Abishnoi69@Abg.org",
```

