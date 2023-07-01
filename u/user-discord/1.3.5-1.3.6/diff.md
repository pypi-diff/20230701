# Comparing `tmp/user_discord-1.3.5.tar.gz` & `tmp/user_discord-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user_discord-1.3.5.tar", last modified: Thu Jun 29 23:25:37 2023, max compression
+gzip compressed data, was "user_discord-1.3.6.tar", last modified: Sat Jul  1 20:50:34 2023, max compression
```

## Comparing `user_discord-1.3.5.tar` & `user_discord-1.3.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 23:25:37.885252 user_discord-1.3.5/
--rw-rw-rw-   0        0        0      335 2023-06-29 23:25:37.886251 user_discord-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     3267 2023-06-24 17:50:03.000000 user_discord-1.3.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-29 23:25:37.888252 user_discord-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0      646 2023-06-29 23:25:32.000000 user_discord-1.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 23:25:37.856026 user_discord-1.3.5/user_discord/
--rw-rw-rw-   0        0        0      598 2023-06-29 23:25:29.000000 user_discord-1.3.5/user_discord/__init__.py
--rw-rw-rw-   0        0        0     1891 2023-06-29 23:20:15.000000 user_discord-1.3.5/user_discord/socket.py
--rw-rw-rw-   0        0        0     4102 2023-06-29 23:25:15.000000 user_discord-1.3.5/user_discord/user_discord.py
-drwxrwxrwx   0        0        0        0 2023-06-29 23:25:37.883254 user_discord-1.3.5/user_discord/utils/
--rw-rw-rw-   0        0        0       85 2023-06-24 18:15:10.000000 user_discord-1.3.5/user_discord/utils/__init__.py
--rw-rw-rw-   0        0        0     1426 2023-06-24 16:38:07.000000 user_discord-1.3.5/user_discord/utils/objects.py
--rw-rw-rw-   0        0        0      818 2023-06-24 16:38:09.000000 user_discord-1.3.5/user_discord/utils/payloads.py
-drwxrwxrwx   0        0        0        0 2023-06-29 23:25:37.876258 user_discord-1.3.5/user_discord.egg-info/
--rw-rw-rw-   0        0        0      335 2023-06-29 23:25:37.000000 user_discord-1.3.5/user_discord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-06-29 23:25:37.000000 user_discord-1.3.5/user_discord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 23:25:37.000000 user_discord-1.3.5/user_discord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-29 23:25:37.000000 user_discord-1.3.5/user_discord.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-29 23:25:37.000000 user_discord-1.3.5/user_discord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 20:50:34.265312 user_discord-1.3.6/
+-rw-rw-rw-   0        0        0      335 2023-07-01 20:50:34.265312 user_discord-1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3267 2023-06-24 17:50:03.000000 user_discord-1.3.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-01 20:50:34.268308 user_discord-1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      646 2023-07-01 20:49:59.000000 user_discord-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:50:34.160481 user_discord-1.3.6/user_discord/
+-rw-rw-rw-   0        0        0      598 2023-07-01 20:50:06.000000 user_discord-1.3.6/user_discord/__init__.py
+-rw-rw-rw-   0        0        0     2625 2023-06-30 01:04:08.000000 user_discord-1.3.6/user_discord/socket.py
+-rw-rw-rw-   0        0        0     4400 2023-06-30 01:04:19.000000 user_discord-1.3.6/user_discord/user_discord.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:50:34.263313 user_discord-1.3.6/user_discord/utils/
+-rw-rw-rw-   0        0        0       85 2023-06-24 18:15:10.000000 user_discord-1.3.6/user_discord/utils/__init__.py
+-rw-rw-rw-   0        0        0     1426 2023-06-24 16:38:07.000000 user_discord-1.3.6/user_discord/utils/objects.py
+-rw-rw-rw-   0        0        0      818 2023-06-24 16:38:09.000000 user_discord-1.3.6/user_discord/utils/payloads.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:50:34.204132 user_discord-1.3.6/user_discord.egg-info/
+-rw-rw-rw-   0        0        0      335 2023-07-01 20:50:32.000000 user_discord-1.3.6/user_discord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-07-01 20:50:32.000000 user_discord-1.3.6/user_discord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 20:50:32.000000 user_discord-1.3.6/user_discord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-07-01 20:50:32.000000 user_discord-1.3.6/user_discord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-01 20:50:32.000000 user_discord-1.3.6/user_discord.egg-info/top_level.txt
```

### Comparing `user_discord-1.3.5/README.md` & `user_discord-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `user_discord-1.3.5/setup.py` & `user_discord-1.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 long_description ="""By: nxslayer\nInstall: pip install user_discord"""
 
 setup(
     name="user_discord",
     license="MIT",
     author="nxSlayer",
-    version="1.3.5",
+    version="1.3.6",
     author_email="princediscordslay@gmail.com",
     description="Library for discord bots.",
     url="https://github.com/nxSlayer/user-discord",
     packages=find_packages(),
     long_description=long_description,
     install_requires=requirements,
     keywords=[
```

### Comparing `user_discord-1.3.5/user_discord/__init__.py` & `user_discord-1.3.6/user_discord/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,9 +11,9 @@
 from .utils import payloads
 
 from requests import get
 from json import loads
 
 __newest__ = loads(get("https://pypi.org/pypi/user-discord/json").text)["info"]["version"]
 
-if '1.3.5' != __newest__:
+if '1.3.6' != __newest__:
     print(f"(user-discord) There is a new version, please update for better results")
```

### Comparing `user_discord-1.3.5/user_discord/user_discord.py` & `user_discord-1.3.6/user_discord/user_discord.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import base64
 import requests
 import websocket
 from requests.structures import CaseInsensitiveDict
 from threading import Thread
 from user_discord.utils.payloads import StartSocket
 from user_discord.utils.objects import MessageContent
+from . import SocketDiscord
 
 
 class ClientDiscord:
 
   def __init__(self):
     
     self.token = None
@@ -136,8 +137,15 @@
 
     api = "https://discord.com/api/v9/users/@me"
     payload = {"avatar": data}
     res = self.web.patch(api, json=payload)
     if res.status_code != 200:
       return Exception(res.text)
     else:
-      return res.json()
+      return res.json()
+      
+  def update_members(self, socket, guild_id, channel_id):
+    socket.send_json({"op":14,"d":{"guild_id":guild_id,"channels":{channel_id:[[0,99]]}}})
+    time.sleep(2)
+    try:data = json.load(open('cache/guild_members.json'))
+    except:data = []
+    return data
```

### Comparing `user_discord-1.3.5/user_discord/utils/objects.py` & `user_discord-1.3.6/user_discord/utils/objects.py`

 * *Files identical despite different names*

### Comparing `user_discord-1.3.5/user_discord/utils/payloads.py` & `user_discord-1.3.6/user_discord/utils/payloads.py`

 * *Files identical despite different names*

