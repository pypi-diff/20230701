# Comparing `tmp/pyrubi-2.2.1.tar.gz` & `tmp/pyrubi-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrubi-2.2.1.tar", last modified: Thu Jun 29 17:54:50 2023, max compression
+gzip compressed data, was "pyrubi-2.3.0.tar", last modified: Fri Jun 30 22:22:24 2023, max compression
```

## Comparing `pyrubi-2.2.1.tar` & `pyrubi-2.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 17:54:50.234609 pyrubi-2.2.1/
--rw-rw-rw-   0        0        0     2251 2023-06-29 17:54:50.234609 pyrubi-2.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1409 2023-06-29 17:51:32.000000 pyrubi-2.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 17:54:50.194502 pyrubi-2.2.1/pyrubi/
--rw-rw-rw-   0        0        0      205 2023-06-29 16:41:57.000000 pyrubi-2.2.1/pyrubi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 17:54:50.212496 pyrubi-2.2.1/pyrubi/cryption/
--rw-rw-rw-   0        0        0     3932 2023-06-27 09:26:51.000000 pyrubi-2.2.1/pyrubi/cryption/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 17:54:50.220494 pyrubi-2.2.1/pyrubi/handler/
--rw-rw-rw-   0        0        0     1142 2023-06-27 09:30:29.000000 pyrubi-2.2.1/pyrubi/handler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 17:54:50.221493 pyrubi-2.2.1/pyrubi/maker/
--rw-rw-rw-   0        0        0     3399 2023-06-27 13:42:47.000000 pyrubi-2.2.1/pyrubi/maker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 17:54:50.228611 pyrubi-2.2.1/pyrubi/message/
--rw-rw-rw-   0        0        0     3439 2023-06-29 17:42:57.000000 pyrubi-2.2.1/pyrubi/message/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 17:54:50.230611 pyrubi-2.2.1/pyrubi/methods/
--rw-rw-rw-   0        0        0    45811 2023-06-29 17:47:51.000000 pyrubi-2.2.1/pyrubi/methods/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 17:54:50.231611 pyrubi-2.2.1/pyrubi/servers/
--rw-rw-rw-   0        0        0      357 2023-06-27 08:13:23.000000 pyrubi-2.2.1/pyrubi/servers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 17:54:50.232610 pyrubi-2.2.1/pyrubi/sessions/
--rw-rw-rw-   0        0        0      672 2023-06-29 17:23:20.000000 pyrubi-2.2.1/pyrubi/sessions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 17:54:50.233610 pyrubi-2.2.1/pyrubi/tools/
--rw-rw-rw-   0        0        0     7297 2023-06-26 11:48:21.000000 pyrubi-2.2.1/pyrubi/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 17:54:50.211497 pyrubi-2.2.1/pyrubi.egg-info/
--rw-rw-rw-   0        0        0     2251 2023-06-29 17:54:50.000000 pyrubi-2.2.1/pyrubi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2023-06-29 17:54:50.000000 pyrubi-2.2.1/pyrubi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 17:54:50.000000 pyrubi-2.2.1/pyrubi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-06-29 17:54:50.000000 pyrubi-2.2.1/pyrubi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-29 17:54:50.000000 pyrubi-2.2.1/pyrubi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 17:54:50.234609 pyrubi-2.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1109 2023-06-29 17:48:53.000000 pyrubi-2.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 22:22:24.030258 pyrubi-2.3.0/
+-rw-rw-rw-   0        0        0     2255 2023-06-30 22:22:24.030258 pyrubi-2.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1409 2023-06-30 22:19:53.000000 pyrubi-2.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 22:22:23.997611 pyrubi-2.3.0/pyrubi/
+-rw-rw-rw-   0        0        0      205 2023-06-30 20:13:28.000000 pyrubi-2.3.0/pyrubi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 22:22:24.014606 pyrubi-2.3.0/pyrubi/cryption/
+-rw-rw-rw-   0        0        0     3932 2023-06-27 09:26:51.000000 pyrubi-2.3.0/pyrubi/cryption/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 22:22:24.015605 pyrubi-2.3.0/pyrubi/handler/
+-rw-rw-rw-   0        0        0     1142 2023-06-27 09:30:29.000000 pyrubi-2.3.0/pyrubi/handler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 22:22:24.016606 pyrubi-2.3.0/pyrubi/maker/
+-rw-rw-rw-   0        0        0     3399 2023-06-27 13:42:47.000000 pyrubi-2.3.0/pyrubi/maker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 22:22:24.024256 pyrubi-2.3.0/pyrubi/message/
+-rw-rw-rw-   0        0        0     3863 2023-06-30 22:04:18.000000 pyrubi-2.3.0/pyrubi/message/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 22:22:24.025259 pyrubi-2.3.0/pyrubi/methods/
+-rw-rw-rw-   0        0        0    46199 2023-06-30 21:53:00.000000 pyrubi-2.3.0/pyrubi/methods/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 22:22:24.027258 pyrubi-2.3.0/pyrubi/servers/
+-rw-rw-rw-   0        0        0      357 2023-06-27 08:13:23.000000 pyrubi-2.3.0/pyrubi/servers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 22:22:24.028258 pyrubi-2.3.0/pyrubi/sessions/
+-rw-rw-rw-   0        0        0      501 2023-06-30 20:18:21.000000 pyrubi-2.3.0/pyrubi/sessions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 22:22:24.029260 pyrubi-2.3.0/pyrubi/tools/
+-rw-rw-rw-   0        0        0     7297 2023-06-26 11:48:21.000000 pyrubi-2.3.0/pyrubi/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 22:22:24.013605 pyrubi-2.3.0/pyrubi.egg-info/
+-rw-rw-rw-   0        0        0     2255 2023-06-30 22:22:23.000000 pyrubi-2.3.0/pyrubi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2023-06-30 22:22:23.000000 pyrubi-2.3.0/pyrubi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 22:22:23.000000 pyrubi-2.3.0/pyrubi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-06-30 22:22:23.000000 pyrubi-2.3.0/pyrubi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-30 22:22:23.000000 pyrubi-2.3.0/pyrubi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 22:22:24.030258 pyrubi-2.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1113 2023-06-30 22:21:10.000000 pyrubi-2.3.0/setup.py
```

### Comparing `pyrubi-2.2.1/PKG-INFO` & `pyrubi-2.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: pyrubi
-Version: 2.2.1
+Version: 2.3.0
 Summary: This is a powerful and easy library for building self Bots in Rubika
 Home-page: https://github.com/AliGanji1/pyrubi
 Author: Ali Ganji zadeh
 Author-email: ali.ganji.za@gmail.com
-Keywords: rubika,rubika-bot,pyrubi,rubx,rubino,rubika.ir
+Keywords: rubika,rubika-bot,pyrubi,rubino,rubika.ir,pyrubika
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
 
-<h1>Pyrubi 2.2.1</h1>
+<h1>Pyrubi 2.3.0</h1>
 
 > Pyrubi is a powerful and easy library for building self Bots in Rubika
 
 <p align='center'>
-    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.2.1' width='356' class="image">
+    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.3.0' width='356' class="image">
 </p>
 
 <p align='center'>
     <a href='https://github.com/AliGanji1/pyrubi'>GitHub</a>
     •
     <a href='https://rubika.ir/pyrubika'>Documents</a>
 </p>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: pyrubi Version: 2.2.1 Summary: This is a powerful
+Metadata-Version: 2.1 Name: pyrubi Version: 2.3.0 Summary: This is a powerful
 and easy library for building self Bots in Rubika Home-page: https://
 github.com/AliGanji1/pyrubi Author: Ali Ganji zadeh Author-email:
-ali.ganji.za@gmail.com Keywords: rubika,rubika-bot,pyrubi,rubx,rubino,rubika.ir
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
-Approved :: MIT License Requires-Python: ~=3.6 Description-Content-Type: text/
-markdown
-****** Pyrubi 2.2.1 ******
+ali.ganji.za@gmail.com Keywords: rubika,rubika-
+bot,pyrubi,rubino,rubika.ir,pyrubika Classifier: Programming Language :: Python
+:: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: License :: OSI Approved :: MIT License Requires-
+Python: ~=3.6 Description-Content-Type: text/markdown
+****** Pyrubi 2.3.0 ******
 > Pyrubi is a powerful and easy library for building self Bots in Rubika
-                            [Pyrubi Library 2.2.1]
+                            [Pyrubi Library 2.3.0]
                              GitHub â¢ Documents
 [![Downloads](https://static.pepy.tech/badge/pyrubi)](https://pepy.tech/
 project/pyrubi) **The Pyrubi library is compatible with version 6 of the
 Rubik's API**
 ===============================================================================
 ## Install or Update: ``` bash pip install -U pyrubi ```
 ===============================================================================
```

### Comparing `pyrubi-2.2.1/README.md` & `pyrubi-2.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-<h1>Pyrubi 2.2.1</h1>
+<h1>Pyrubi 2.3.0</h1>
 
 > Pyrubi is a powerful and easy library for building self Bots in Rubika
 
 <p align='center'>
-    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.2.1' width='356' class="image">
+    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.3.0' width='356' class="image">
 </p>
 
 <p align='center'>
     <a href='https://github.com/AliGanji1/pyrubi'>GitHub</a>
     •
     <a href='https://rubika.ir/pyrubika'>Documents</a>
 </p>
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-****** Pyrubi 2.2.1 ******
+****** Pyrubi 2.3.0 ******
 > Pyrubi is a powerful and easy library for building self Bots in Rubika
-                            [Pyrubi Library 2.2.1]
+                            [Pyrubi Library 2.3.0]
                              GitHub â¢ Documents
 [![Downloads](https://static.pepy.tech/badge/pyrubi)](https://pepy.tech/
 project/pyrubi) **The Pyrubi library is compatible with version 6 of the
 Rubik's API**
 ===============================================================================
 ## Install or Update: ``` bash pip install -U pyrubi ```
 ===============================================================================
```

### Comparing `pyrubi-2.2.1/pyrubi/cryption/__init__.py` & `pyrubi-2.3.0/pyrubi/cryption/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubi-2.2.1/pyrubi/handler/__init__.py` & `pyrubi-2.3.0/pyrubi/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubi-2.2.1/pyrubi/maker/__init__.py` & `pyrubi-2.3.0/pyrubi/maker/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubi-2.2.1/pyrubi/message/__init__.py` & `pyrubi-2.3.0/pyrubi/message/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 class message:
 
     def __init__(self, data):
         self.data = data
+        del data
 
     def chat_id(self):
         return self.data['message_updates'][0]['object_guid'] if 'message_updates' in self.data else self.data['object_guid']
 
     def author_id(self):
         return self.data['message_updates'][0]['message']['author_object_guid'] if 'message_updates' in self.data else self.data['last_message']['author_object_guid']
 
@@ -15,53 +16,64 @@
     def reply_to_message_id(self):
         return self.data['message_updates'][0]['message'].get('reply_to_message_id')
 
     def text(self):
         return str(self.data['message_updates'][0]['message'].get('text') if 'message_updates' in self.data else self.data['last_message'].get('text'))
 
     def chat_type(self):
-        return self.data['message_updates'][0]['type'] if 'message_updates' in self.data else self.data['abs_object']['type']
+        try:
+            return self.data['message_updates'][0].get('type') if 'message_updates' in self.data else self.data['abs_object'].get('type')
+        except:
+            pass
 
     def author_type(self):
         return self.data['message_updates'][0]['message']['author_type'] if 'message_updates' in self.data else self.data['last_message']['author_type']
 
     def message_type(self):
-        return self.data['message_updates'][0]['message'].get('type') if 'message_updates' in self.data else self.data['last_message']['type']
+        try:
+            return self.data['message_updates'][0]['message'].get('type') if 'message_updates' in self.data else self.data['last_message'].get('type')
+        except:
+            pass
 
     def is_forward(self):
         return 'forwarded_from' in self.data['message_updates'][0]['message'].keys() if 'message_updates' in self.data else None
         
     def forward_type(self):
-        return self.data['message_updates'][0]['message']['forwarded_from'].get('type_from') if 'message_updates' in self.data else None
+        if self.is_forward():
+            return self.data['message_updates'][0]['message']['forwarded_from'].get('type_from') if 'message_updates' in self.data else None
         
     def forward_id(self):
-        return self.data['message_updates'][0]['message']['forwarded_from'].get('object_guid') if 'message_updates' in self.data else None
+        if self.is_forward():
+            return self.data['message_updates'][0]['message']['forwarded_from'].get('object_guid') if 'message_updates' in self.data else None
         
     def forward_message_id(self):
-        return self.data['message_updates'][0]['message']['forwarded_from'].get('message_id') if 'message_updates' in self.data else None
-        
-    def is_event(self):
-        return 'event_data' in self.data['message_updates'][0]['message'].keys() if 'message_updates' in self.data else self.message_type() == 'Other'
+        if self.is_forward():
+            return self.data['message_updates'][0]['message']['forwarded_from'].get('message_id') if 'message_updates' in self.data else None
 
     def is_user_chat(self):
         return self.chat_type() == 'User'
 
     def is_group_chat(self):
         return self.chat_type() == 'Group'
 
     def is_channel_chat(self):
         return self.chat_type() == 'Channel'
 
     def chat_title(self):
-        return str(self.data['show_notifications'][0].get('title') if 'message_updates' in self.data else self.data['abs_object'].get('title'))
+        return str(self.data['show_notifications'][0].get('title') if 'show_notifications' in self.data else self.data['abs_object'].get('title', f"{self.data['abs_object']['first_name']} {self.data['abs_object']['last_name']}") if "abs_object" in self.data else None)
 
     def author_title(self):
         return self.data['chat_updates'][0]['chat']['last_message'].get('author_title', self.chat_title()) if 'message_updates' in self.data else self.data['last_message'].get('author_title', self.chat_title())
 
+    def is_event(self):
+        return 'event_data' in self.data['message_updates'][0]['message'].keys() if 'message_updates' in self.data else self.message_type() == 'Other'
+
     def event_type(self):
-        return self.data['message_updates'][0]['message']['event_data'].get('type') if 'message_updates' in self.data else None
+        if self.is_event():
+            return self.data['message_updates'][0]['message']['event_data'].get('type') if 'message_updates' in self.data else None
 
     def event_id(self):
-        return self.data['message_updates'][0]['message']['event_data']['performer_object'].get('object_guid') if 'message_updates' in self.data else None
+        if self.is_event():
+            return self.data['message_updates'][0]['message']['event_data']['performer_object'].get('object_guid') if 'message_updates' in self.data else None
         
     def count_unseen(self):
         return self.data['chat_updates'][0]['chat'].get('count_unseen', '0') if 'message_updates' in self.data else None
```

### Comparing `pyrubi-2.2.1/pyrubi/methods/__init__.py` & `pyrubi-2.3.0/pyrubi/methods/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,29 +60,31 @@
 
             return session_data
         
         return sign_in_data
 
     def on_message(self, chat_filter=[], message_filter=[]):
         for recv in self.hs():
-            if 'chat_updates' in recv.keys() and recv["message_updates"]:
+            if 'chat_updates' in recv.keys() and recv.get('message_updates'):
                 msg = message(recv)
                 if not msg.chat_type() in chat_filter and not msg.message_type() in message_filter:
                     yield msg
 
     def get_chats_update(self, chat_filter=[], message_filter=[]):
         while True:
             try:
-                msg = message(chats_update)
-                chats_update = self.method('getChatsUpdates', {'state': round(time()) - 200})['chats'][0]
-                if not msg.chat_type() in chat_filter and not msg.message_type() in message_filter:
-                    if not msg.message_id() in self.got_messages_update:
-                        self.got_messages_update.append(msg.message_id())
-                        yield msg
-            except IndexError:
+                chats_update = self.method('getChatsUpdates', {'state': round(time()) - 200})['chats']
+                if chats_update:
+                    msg = message(chats_update[0])
+                    if not msg.chat_type() in chat_filter and not msg.message_type() in message_filter:
+                        if not msg.message_id() in self.got_messages_update:
+                            self.got_messages_update.append(msg.message_id())
+                            yield msg
+            except Exception as error:
+                print(error.args)
                 continue
 
     def get_chats_update2(self):
         return self.method('getChatsUpdates', {'state': round(time()) - 200})['chats']
 
     def send_text(self, chat_id, text, message_id = None):
         metadata = tools.check_metadata(text)
@@ -485,14 +487,23 @@
         return self.method('getObjectByUsername', {'username': username.replace('@', '')})
 
     def get_chat_last_message(self, chat_id):
         return self.get_chat_info(chat_id)['chat'].get('last_message', None)
 
     def get_chat_last_message_id(self, chat_id):
         return self.get_chat_info(chat_id)['chat']['last_message_id']
+    
+    def get_group_mention_list(self, group_id, search_mention):
+        return self.method(
+            'getGroupMentionList',
+            {
+                "group_guid": group_id,
+                "search_mention": search_mention
+            }
+        )['in_chat_members']
 
     def delete_chat_history(self, chat_id):
         return self.method(
             'deleteChatHistory',
             {
                 'object_guid': chat_id,
                 'last_message_id': self.get_chat_last_message_id(chat_id)
```

### Comparing `pyrubi-2.2.1/pyrubi/tools/__init__.py` & `pyrubi-2.3.0/pyrubi/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubi-2.2.1/pyrubi.egg-info/PKG-INFO` & `pyrubi-2.3.0/pyrubi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: pyrubi
-Version: 2.2.1
+Version: 2.3.0
 Summary: This is a powerful and easy library for building self Bots in Rubika
 Home-page: https://github.com/AliGanji1/pyrubi
 Author: Ali Ganji zadeh
 Author-email: ali.ganji.za@gmail.com
-Keywords: rubika,rubika-bot,pyrubi,rubx,rubino,rubika.ir
+Keywords: rubika,rubika-bot,pyrubi,rubino,rubika.ir,pyrubika
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
 
-<h1>Pyrubi 2.2.1</h1>
+<h1>Pyrubi 2.3.0</h1>
 
 > Pyrubi is a powerful and easy library for building self Bots in Rubika
 
 <p align='center'>
-    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.2.1' width='356' class="image">
+    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.3.0' width='356' class="image">
 </p>
 
 <p align='center'>
     <a href='https://github.com/AliGanji1/pyrubi'>GitHub</a>
     •
     <a href='https://rubika.ir/pyrubika'>Documents</a>
 </p>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: pyrubi Version: 2.2.1 Summary: This is a powerful
+Metadata-Version: 2.1 Name: pyrubi Version: 2.3.0 Summary: This is a powerful
 and easy library for building self Bots in Rubika Home-page: https://
 github.com/AliGanji1/pyrubi Author: Ali Ganji zadeh Author-email:
-ali.ganji.za@gmail.com Keywords: rubika,rubika-bot,pyrubi,rubx,rubino,rubika.ir
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
-Approved :: MIT License Requires-Python: ~=3.6 Description-Content-Type: text/
-markdown
-****** Pyrubi 2.2.1 ******
+ali.ganji.za@gmail.com Keywords: rubika,rubika-
+bot,pyrubi,rubino,rubika.ir,pyrubika Classifier: Programming Language :: Python
+:: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: License :: OSI Approved :: MIT License Requires-
+Python: ~=3.6 Description-Content-Type: text/markdown
+****** Pyrubi 2.3.0 ******
 > Pyrubi is a powerful and easy library for building self Bots in Rubika
-                            [Pyrubi Library 2.2.1]
+                            [Pyrubi Library 2.3.0]
                              GitHub â¢ Documents
 [![Downloads](https://static.pepy.tech/badge/pyrubi)](https://pepy.tech/
 project/pyrubi) **The Pyrubi library is compatible with version 6 of the
 Rubik's API**
 ===============================================================================
 ## Install or Update: ``` bash pip install -U pyrubi ```
 ===============================================================================
```

### Comparing `pyrubi-2.2.1/setup.py` & `pyrubi-2.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'pyrubi',
-    version = '2.2.1',
+    version = '2.3.0',
     author='Ali Ganji zadeh',
     author_email = 'ali.ganji.za@gmail.com',
     description = 'This is a powerful and easy library for building self Bots in Rubika',
-    keywords = ['rubika', 'rubika-bot', 'pyrubi', 'rubx', 'rubino', 'rubika.ir'],
+    keywords = ['rubika', 'rubika-bot', 'pyrubi', 'rubino', 'rubika.ir', 'pyrubika'],
     long_description = open("README.md", encoding="utf-8").read(),
     python_requires="~=3.6",
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/AliGanji1/pyrubi',
     packages = find_packages(),
     install_requires = ['pycryptodome', 'websocket-client', 'requests', 'urllib3', 'pillow', 'mutagen', 'tinytag'],
     classifiers = [
```

