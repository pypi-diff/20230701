# Comparing `tmp/herdmod-0.1.1.tar.gz` & `tmp/herdmod-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "herdmod-0.1.1.tar", last modified: Fri Jun 30 15:52:49 2023, max compression
+gzip compressed data, was "herdmod-0.1.2.tar", last modified: Sat Jul  1 18:23:29 2023, max compression
```

## Comparing `herdmod-0.1.1.tar` & `herdmod-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:52:49.415645 herdmod-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-30 15:52:33.000000 herdmod-0.1.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-30 15:52:33.000000 herdmod-0.1.1/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-30 15:52:33.000000 herdmod-0.1.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-30 15:52:49.411645 herdmod-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-30 15:52:33.000000 herdmod-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:52:49.411645 herdmod-0.1.1/herdmod/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-30 15:52:33.000000 herdmod-0.1.1/herdmod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:52:49.411645 herdmod-0.1.1/herdmod/filters/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-30 15:52:33.000000 herdmod-0.1.1/herdmod/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-30 15:52:33.000000 herdmod-0.1.1/herdmod/filters/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:52:49.411645 herdmod-0.1.1/herdmod/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-30 15:52:33.000000 herdmod-0.1.1/herdmod/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-30 15:52:33.000000 herdmod-0.1.1/herdmod/helpers/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:52:49.411645 herdmod-0.1.1/herdmod/listen/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-30 15:52:33.000000 herdmod-0.1.1/herdmod/listen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-06-30 15:52:33.000000 herdmod-0.1.1/herdmod/listen/listen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:52:49.411645 herdmod-0.1.1/herdmod/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-30 15:52:33.000000 herdmod-0.1.1/herdmod/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-30 15:52:33.000000 herdmod-0.1.1/herdmod/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:52:49.411645 herdmod-0.1.1/herdmod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-30 15:52:49.000000 herdmod-0.1.1/herdmod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-30 15:52:49.000000 herdmod-0.1.1/herdmod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:52:49.000000 herdmod-0.1.1/herdmod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 15:52:49.000000 herdmod-0.1.1/herdmod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 15:52:49.000000 herdmod-0.1.1/herdmod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 15:52:49.415645 herdmod-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-30 15:52:33.000000 herdmod-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:23:29.511631 herdmod-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-01 18:23:18.000000 herdmod-0.1.2/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-01 18:23:18.000000 herdmod-0.1.2/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-01 18:23:18.000000 herdmod-0.1.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-07-01 18:23:29.511631 herdmod-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-01 18:23:18.000000 herdmod-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:23:29.511631 herdmod-0.1.2/herdmod/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-01 18:23:18.000000 herdmod-0.1.2/herdmod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:23:29.511631 herdmod-0.1.2/herdmod/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-01 18:23:18.000000 herdmod-0.1.2/herdmod/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-01 18:23:18.000000 herdmod-0.1.2/herdmod/filters/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:23:29.511631 herdmod-0.1.2/herdmod/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-01 18:23:18.000000 herdmod-0.1.2/herdmod/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-01 18:23:18.000000 herdmod-0.1.2/herdmod/helpers/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:23:29.511631 herdmod-0.1.2/herdmod/listen/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-01 18:23:18.000000 herdmod-0.1.2/herdmod/listen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-01 18:23:18.000000 herdmod-0.1.2/herdmod/listen/listen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:23:29.511631 herdmod-0.1.2/herdmod/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-01 18:23:18.000000 herdmod-0.1.2/herdmod/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-01 18:23:18.000000 herdmod-0.1.2/herdmod/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:23:29.511631 herdmod-0.1.2/herdmod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-07-01 18:23:29.000000 herdmod-0.1.2/herdmod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-01 18:23:29.000000 herdmod-0.1.2/herdmod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 18:23:29.000000 herdmod-0.1.2/herdmod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-01 18:23:29.000000 herdmod-0.1.2/herdmod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-01 18:23:29.000000 herdmod-0.1.2/herdmod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 18:23:29.511631 herdmod-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-01 18:23:18.000000 herdmod-0.1.2/setup.py
```

### Comparing `herdmod-0.1.1/COPYING` & `herdmod-0.1.2/COPYING`

 * *Files identical despite different names*

### Comparing `herdmod-0.1.1/COPYING.lesser` & `herdmod-0.1.2/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `herdmod-0.1.1/NOTICE` & `herdmod-0.1.2/NOTICE`

 * *Files identical despite different names*

### Comparing `herdmod-0.1.1/PKG-INFO` & `herdmod-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herdmod
-Version: 0.1.1
+Version: 0.1.2
 Summary: A monkeypatcher add-on for Pyroherd
 Home-page: https://github.com/OnTheHerd/herdmod
 Author: OnTheHerd
 Author-email: ontheherd@onmail.com
 License: LGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `herdmod-0.1.1/README.md` & `herdmod-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `herdmod-0.1.1/herdmod/helpers/helpers.py` & `herdmod-0.1.2/herdmod/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `herdmod-0.1.1/herdmod/listen/listen.py` & `herdmod-0.1.2/herdmod/listen/listen.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,45 +54,14 @@
         if not listener or listener['future'].done():
             return
         
         listener['future'].set_exception(ListenerCanceled())
         self.clear_listener(chat_id, listener['future'])
 
 
-@patch(pyroherd.handlers.callback_query_handler.CallbackQueryHandler)
-class CallbackQueryHandler:
-    @patchable
-    def __init__(self, callback: callable, filters=None):
-        self.user_callback = callback
-        self.old__init__(self.resolve_listener, filters)
-    
-    @patchable
-    async def resolve_listener(self, client, query, *args):
-        listener = client.listening.get(query.message.chat.id)
-        if listener and not listener['future'].done():
-            listener['future'].set_result(message)
-        else:
-            if listener and listener['future'].done():
-                client.clear_listener(query.message.chat.id, listener['future'])
-            await self.user_callback(client, query, *args)
-    
-    @patchable
-    async def check(self, client, query):
-        listener = client.listening.get(query.message.chat.id)
-        
-        if listener and not listener['future'].done():
-            return await listener['filters'](client, query) if callable(listener['filters']) else True
-            
-        return (
-            await self.filters(client, query)
-            if callable(self.filters)
-            else True
-        )
-
-
 @patch(pyroherd.handlers.message_handler.MessageHandler)
 class MessageHandler:
     @patchable
     def __init__(self, callback: callable, filters=None):
         self.user_callback = callback
         self.old__init__(self.resolve_listener, filters)
```

### Comparing `herdmod-0.1.1/herdmod.egg-info/PKG-INFO` & `herdmod-0.1.2/herdmod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herdmod
-Version: 0.1.1
+Version: 0.1.2
 Summary: A monkeypatcher add-on for Pyroherd
 Home-page: https://github.com/OnTheHerd/herdmod
 Author: OnTheHerd
 Author-email: ontheherd@onmail.com
 License: LGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `herdmod-0.1.1/setup.py` & `herdmod-0.1.2/setup.py`

 * *Files identical despite different names*

