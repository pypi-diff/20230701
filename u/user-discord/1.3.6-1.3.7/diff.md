# Comparing `tmp/user_discord-1.3.6.tar.gz` & `tmp/user_discord-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user_discord-1.3.6.tar", last modified: Sat Jul  1 20:50:34 2023, max compression
+gzip compressed data, was "user_discord-1.3.7.tar", last modified: Sat Jul  1 21:29:17 2023, max compression
```

## Comparing `user_discord-1.3.6.tar` & `user_discord-1.3.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 20:50:34.265312 user_discord-1.3.6/
--rw-rw-rw-   0        0        0      335 2023-07-01 20:50:34.265312 user_discord-1.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     3267 2023-06-24 17:50:03.000000 user_discord-1.3.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-01 20:50:34.268308 user_discord-1.3.6/setup.cfg
--rw-rw-rw-   0        0        0      646 2023-07-01 20:49:59.000000 user_discord-1.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 20:50:34.160481 user_discord-1.3.6/user_discord/
--rw-rw-rw-   0        0        0      598 2023-07-01 20:50:06.000000 user_discord-1.3.6/user_discord/__init__.py
--rw-rw-rw-   0        0        0     2625 2023-06-30 01:04:08.000000 user_discord-1.3.6/user_discord/socket.py
--rw-rw-rw-   0        0        0     4400 2023-06-30 01:04:19.000000 user_discord-1.3.6/user_discord/user_discord.py
-drwxrwxrwx   0        0        0        0 2023-07-01 20:50:34.263313 user_discord-1.3.6/user_discord/utils/
--rw-rw-rw-   0        0        0       85 2023-06-24 18:15:10.000000 user_discord-1.3.6/user_discord/utils/__init__.py
--rw-rw-rw-   0        0        0     1426 2023-06-24 16:38:07.000000 user_discord-1.3.6/user_discord/utils/objects.py
--rw-rw-rw-   0        0        0      818 2023-06-24 16:38:09.000000 user_discord-1.3.6/user_discord/utils/payloads.py
-drwxrwxrwx   0        0        0        0 2023-07-01 20:50:34.204132 user_discord-1.3.6/user_discord.egg-info/
--rw-rw-rw-   0        0        0      335 2023-07-01 20:50:32.000000 user_discord-1.3.6/user_discord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-07-01 20:50:32.000000 user_discord-1.3.6/user_discord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 20:50:32.000000 user_discord-1.3.6/user_discord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-07-01 20:50:32.000000 user_discord-1.3.6/user_discord.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-01 20:50:32.000000 user_discord-1.3.6/user_discord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 21:29:17.941354 user_discord-1.3.7/
+-rw-rw-rw-   0        0        0      335 2023-07-01 21:29:17.942354 user_discord-1.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3267 2023-06-24 17:50:03.000000 user_discord-1.3.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-01 21:29:17.944351 user_discord-1.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      646 2023-07-01 21:29:01.000000 user_discord-1.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 21:29:17.888246 user_discord-1.3.7/user_discord/
+-rw-rw-rw-   0        0        0      598 2023-07-01 21:28:54.000000 user_discord-1.3.7/user_discord/__init__.py
+-rw-rw-rw-   0        0        0     2510 2023-07-01 21:28:04.000000 user_discord-1.3.7/user_discord/socket.py
+-rw-rw-rw-   0        0        0     4414 2023-07-01 21:28:44.000000 user_discord-1.3.7/user_discord/user_discord.py
+drwxrwxrwx   0        0        0        0 2023-07-01 21:29:17.939354 user_discord-1.3.7/user_discord/utils/
+-rw-rw-rw-   0        0        0       85 2023-06-24 18:15:10.000000 user_discord-1.3.7/user_discord/utils/__init__.py
+-rw-rw-rw-   0        0        0     1426 2023-06-24 16:38:07.000000 user_discord-1.3.7/user_discord/utils/objects.py
+-rw-rw-rw-   0        0        0      818 2023-06-24 16:38:09.000000 user_discord-1.3.7/user_discord/utils/payloads.py
+drwxrwxrwx   0        0        0        0 2023-07-01 21:29:17.924363 user_discord-1.3.7/user_discord.egg-info/
+-rw-rw-rw-   0        0        0      335 2023-07-01 21:29:17.000000 user_discord-1.3.7/user_discord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-07-01 21:29:17.000000 user_discord-1.3.7/user_discord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 21:29:17.000000 user_discord-1.3.7/user_discord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-07-01 21:29:17.000000 user_discord-1.3.7/user_discord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-01 21:29:17.000000 user_discord-1.3.7/user_discord.egg-info/top_level.txt
```

### Comparing `user_discord-1.3.6/README.md` & `user_discord-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `user_discord-1.3.6/setup.py` & `user_discord-1.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 long_description ="""By: nxslayer\nInstall: pip install user_discord"""
 
 setup(
     name="user_discord",
     license="MIT",
     author="nxSlayer",
-    version="1.3.6",
+    version="1.3.7",
     author_email="princediscordslay@gmail.com",
     description="Library for discord bots.",
     url="https://github.com/nxSlayer/user-discord",
     packages=find_packages(),
     long_description=long_description,
     install_requires=requirements,
     keywords=[
```

### Comparing `user_discord-1.3.6/user_discord/__init__.py` & `user_discord-1.3.7/user_discord/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,9 +11,9 @@
 from .utils import payloads
 
 from requests import get
 from json import loads
 
 __newest__ = loads(get("https://pypi.org/pypi/user-discord/json").text)["info"]["version"]
 
-if '1.3.6' != __newest__:
+if '1.3.7' != __newest__:
     print(f"(user-discord) There is a new version, please update for better results")
```

### Comparing `user_discord-1.3.6/user_discord/socket.py` & `user_discord-1.3.7/user_discord/socket.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 import random
 import base64
 import requests
 import websocket
 from requests.structures import CaseInsensitiveDict
 from threading import Thread
 from .utils.payloads import StartSocket
-from .utils.objects import MessageContent
+from .utils.objects import MessageContent, AuthorProfile
 import os
 
 
 class SocketDiscord:
     def __init__(self, client):
         self.events = {}
         self.ws = None
         self.token = client.token
+        self.client = client
         
 
     def on(self, event):
         def event_ready(handler):
             if event not in self.events:
                 self.events[event] = []
             self.events[event].append(handler)
@@ -66,27 +67,20 @@
       self.session_id = self.session_id.get('d').get('session_id')
 
     def get_object(self, data):
       if data['t'] == 'MESSAGE_CREATE':
         return MessageContent(data).MessageContent
 
       if data['t'] == 'GUILD_MEMBER_LIST_UPDATE':
-        try:
-          os.mkdir('cache')
-        except:
-          pass
         if data['s'] == 3:
-          with open('./cache/guild_members.json', 'w') as filesave:
-            try:
-              date = []
-              for item in data['d']['ops'][0]['items']:
-                if item.get('member'):
-                  date.append(item['member']['user'])
-              filesave.write(json.dumps(date))
-            except:filesave.write('[]')
+          try:
+            for item in data['d']['ops'][0]['items']:
+              if item.get('member'):
+                self.client.online_members.append(AuthorProfile(item['member']['user']).AuthorProfile)
+          except:self.client.online_members = []
       
       return data
       
     def event_manager(self):
       while True:
         event = self.receive_json()
         try:
```

### Comparing `user_discord-1.3.6/user_discord/user_discord.py` & `user_discord-1.3.7/user_discord/user_discord.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,17 @@
     self.token = None
 
     self.username = None
     self.email = None
     self.id = None
     self.telephone = None
 
+    #Guild parameters
+    self.online_members = []
+
     self.headers = CaseInsensitiveDict()
 
 
   def generate_nonce(self):
     return str(random.randint(1121966494243094528, 2121966494243094528))
 
   def login_token(self, token):
@@ -139,13 +142,12 @@
     payload = {"avatar": data}
     res = self.web.patch(api, json=payload)
     if res.status_code != 200:
       return Exception(res.text)
     else:
       return res.json()
       
-  def update_members(self, socket, guild_id, channel_id):
+  def get_members(self, socket, guild_id, channel_id):
+    #Get members from channel
     socket.send_json({"op":14,"d":{"guild_id":guild_id,"channels":{channel_id:[[0,99]]}}})
     time.sleep(2)
-    try:data = json.load(open('cache/guild_members.json'))
-    except:data = []
-    return data
+    return self.online_members
```

### Comparing `user_discord-1.3.6/user_discord/utils/objects.py` & `user_discord-1.3.7/user_discord/utils/objects.py`

 * *Files identical despite different names*

### Comparing `user_discord-1.3.6/user_discord/utils/payloads.py` & `user_discord-1.3.7/user_discord/utils/payloads.py`

 * *Files identical despite different names*

