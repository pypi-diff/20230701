# Comparing `tmp/selfcord.py-0.2.1.tar.gz` & `tmp/selfcord.py-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selfcord.py-0.2.1.tar", last modified: Thu Jun 22 22:39:40 2023, max compression
+gzip compressed data, was "selfcord.py-0.2.2.tar", last modified: Fri Jun 30 22:49:39 2023, max compression
```

## Comparing `selfcord.py-0.2.1.tar` & `selfcord.py-0.2.2.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:39:40.264973 selfcord.py-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-22 22:39:40.264973 selfcord.py-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-06-22 22:39:26.000000 selfcord.py-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:39:40.260972 selfcord.py-0.2.1/selfcord/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:39:40.260972 selfcord.py-0.2.1/selfcord/api/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/api/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17481 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    22142 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/api/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/api/http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:39:40.260972 selfcord.py-0.2.1/selfcord/api/voice/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/api/voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/api/voice/voice.py
--rw-r--r--   0 runner    (1001) docker     (123)    26478 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:39:40.264973 selfcord.py-0.2.1/selfcord/models/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25386 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/models/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/models/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/models/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/models/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/models/interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/models/member.py
--rw-r--r--   0 runner    (1001) docker     (123)     9777 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/models/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/models/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/models/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/models/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/models/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:39:40.264973 selfcord.py-0.2.1/selfcord/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17085 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/utils/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/selfcord/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:39:40.260972 selfcord.py-0.2.1/selfcord.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-22 22:39:40.000000 selfcord.py-0.2.1/selfcord.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-22 22:39:40.000000 selfcord.py-0.2.1/selfcord.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 22:39:40.000000 selfcord.py-0.2.1/selfcord.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-22 22:39:40.000000 selfcord.py-0.2.1/selfcord.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-22 22:39:40.000000 selfcord.py-0.2.1/selfcord.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 22:39:40.264973 selfcord.py-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:39:40.264973 selfcord.py-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-22 22:39:27.000000 selfcord.py-0.2.1/tests/test_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:49:39.103731 selfcord.py-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-30 22:49:39.103731 selfcord.py-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:49:39.103731 selfcord.py-0.2.2/selfcord/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:49:39.103731 selfcord.py-0.2.2/selfcord/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18394 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23063 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/api/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10865 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/api/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:49:39.103731 selfcord.py-0.2.2/selfcord/api/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/api/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/api/voice/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28870 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:49:39.103731 selfcord.py-0.2.2/selfcord/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29311 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/models/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/models/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/models/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12092 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/models/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/models/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/models/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10729 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/models/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/models/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/models/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:49:39.103731 selfcord.py-0.2.2/selfcord/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17065 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/utils/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:49:39.103731 selfcord.py-0.2.2/selfcord.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-30 22:49:39.000000 selfcord.py-0.2.2/selfcord.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-30 22:49:39.000000 selfcord.py-0.2.2/selfcord.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:49:39.000000 selfcord.py-0.2.2/selfcord.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-30 22:49:39.000000 selfcord.py-0.2.2/selfcord.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 22:49:39.000000 selfcord.py-0.2.2/selfcord.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 22:49:39.103731 selfcord.py-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:49:39.103731 selfcord.py-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/tests/test_commands.py
```

### Comparing `selfcord.py-0.2.1/PKG-INFO` & `selfcord.py-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: selfcord.py
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Discord API wrapper designed for selfbots!
 Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell
 License: MIT
 Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown
 Provides-Extra: voice
+License-File: LICENSE
 
 <div align="center">
 <img src="./logo.png" widht="180" height="180" style="border-radius: 100%;">
 <h1 align="center">SELFCORD</h1>
 <strong><i>A Powerful Library for Discord Selfbots</i></strong>
 <br>
 <br>
 <a href="https://www.python.org/">
 <img src="https://img.shields.io/badge/MADE%20WITH-PYTHON-red?logoColor=red&logo=Python&style=for-the-badge">
 </a>
 <a href="https://pypi.org/project/selfcord/">
-<img src="https://img.shields.io/badge/version-0.2.1-blue?logo=adguard&style=for-the-badge">
+<img src="https://img.shields.io/badge/version-0.2.2-blue?logo=adguard&style=for-the-badge">
 </a>
 <a href="https://github.com/Shell1010/Selfcord/wiki">
 <img src="https://img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge">
 </a>
 </div>
 
 ## Feautres
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 2.1 Name: selfcord.py Version: 0.2.1 Summary: A Discord API
+Metadata-Version: 2.1 Name: selfcord.py Version: 0.2.2 Summary: A Discord API
 wrapper designed for selfbots! Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell License: MIT Keywords: selfbot,discord,discordapi,discordwrapper
-Description-Content-Type: text/markdown Provides-Extra: voice
+Description-Content-Type: text/markdown Provides-Extra: voice License-File:
+LICENSE
                                  [./logo.png]
                             ****** SELFCORD ******
                    A Powerful Library for Discord Selfbots
 
                [https://img.shields.io/badge/MADE%20WITH-PYTHON-
   red?logoColor=red&logo=Python&style=for-the-badge] [https://img.shields.io/
-     badge/version-0.2.1-blue?logo=adguard&style=for-the-badge] [https://
+     badge/version-0.2.2-blue?logo=adguard&style=for-the-badge] [https://
   img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge]
 ## Feautres - Modern Pythonic API using `async`/`await` syntax - Easy to use
 with an object oriented design - Optimised for both speed and memory - Prevents
 detection of user account automation - Clean Documentation - Community Support
 ## Installation Python 3.10 or higher is required. ``` pip install selfcord.py
 ``` ## Wiki Read our [Wiki](https://github.com/Shell1010/Selfcord/wiki) in
 regards to documentation and getting started. ## Getting Started A selfbot that
```

### Comparing `selfcord.py-0.2.1/README.md` & `selfcord.py-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 <strong><i>A Powerful Library for Discord Selfbots</i></strong>
 <br>
 <br>
 <a href="https://www.python.org/">
 <img src="https://img.shields.io/badge/MADE%20WITH-PYTHON-red?logoColor=red&logo=Python&style=for-the-badge">
 </a>
 <a href="https://pypi.org/project/selfcord/">
-<img src="https://img.shields.io/badge/version-0.2.1-blue?logo=adguard&style=for-the-badge">
+<img src="https://img.shields.io/badge/version-0.2.2-blue?logo=adguard&style=for-the-badge">
 </a>
 <a href="https://github.com/Shell1010/Selfcord/wiki">
 <img src="https://img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge">
 </a>
 </div>
 
 ## Feautres
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
                                  [./logo.png]
                             ****** SELFCORD ******
                    A Powerful Library for Discord Selfbots
 
                [https://img.shields.io/badge/MADE%20WITH-PYTHON-
   red?logoColor=red&logo=Python&style=for-the-badge] [https://img.shields.io/
-     badge/version-0.2.1-blue?logo=adguard&style=for-the-badge] [https://
+     badge/version-0.2.2-blue?logo=adguard&style=for-the-badge] [https://
   img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge]
 ## Feautres - Modern Pythonic API using `async`/`await` syntax - Easy to use
 with an object oriented design - Optimised for both speed and memory - Prevents
 detection of user account automation - Clean Documentation - Community Support
 ## Installation Python 3.10 or higher is required. ``` pip install selfcord.py
 ``` ## Wiki Read our [Wiki](https://github.com/Shell1010/Selfcord/wiki) in
 regards to documentation and getting started. ## Getting Started A selfbot that
```

### Comparing `selfcord.py-0.2.1/selfcord/api/errors.py` & `selfcord.py-0.2.2/selfcord/api/errors.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.1/selfcord/api/events.py` & `selfcord.py-0.2.2/selfcord/api/events.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import asyncio
 import time
 from time import perf_counter
 from typing import TYPE_CHECKING
 
 from aioconsole import aprint
 
+from selfcord.models.message import Action_Row, Text_Input
 from selfcord.models.sessions import Event_Session
 
 from ..models import (Client, DMChannel, GroupChannel, Guild, Message,
                       TextChannel, User, VoiceChannel)
 from ..models.role import Role
 from ..utils import logging
 from .voice import Voice
@@ -268,27 +269,27 @@
             for guild in self.user.guilds:
                 for channel in guild.channels:
                     if channel.id == id:
                         await self.bot.emit("channel_delete", channel)
                         guild.channels.remove(channel)
                         return
 
-    async def handle_guild_role_create(self, role: dict, user: Client, http: http):
+    async def handle_guild_role_create(self, data: dict, user: Client, http: http):
         """Handles what happens when a role is created
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
         """
         self.user = user
 
         for guild in self.user.guilds:
-            if role.get("guild_id") == guild.id:
-                role = Role(role, self.bot, self.http, guild_id=guild.id)
+            if data.get("guild_id") == guild.id:
+                role = Role(data, self.bot, self.http, guild_id=guild.id)
                 guild.roles.append(role)
 
         await self.bot.emit("role_create", role)
 
     async def handle_guild_role_delete(self, role: dict, user: Client, http: http):
         """Handles what happens when a role is deleted
 
@@ -472,7 +473,28 @@
 
         id = data['id']
         since = data['since']
         for type, value in types.items():
             if data.get("type") == value:
                 rs_type = type
         await self.bot.emit("relationship_remove", id, rs_type, since)
+
+    async def handle_interaction_modal_create(self, data: dict, user: Client, http: http):
+        """Handles when a text input modal is Created
+
+         Args:
+            data (dict): JSON data from gateway
+            user (Client): The client instance
+            http (http): HTTP instance
+        """
+        components = data['components'] if data.get("components") is not None else []
+        new_comps = []
+        print(data['id'])
+        for component in components:
+            if component['type'] == 1:
+                for comp in component['components']:
+                    if comp['type'] == 4:
+                        text = Text_Input(comp, self.bot, self.http)
+                        setattr(text, "id", data['id'])
+                        new_comps.append(text)
+            
+        await self.bot.emit("modal_create", new_comps)
```

### Comparing `selfcord.py-0.2.1/selfcord/api/gateway.py` & `selfcord.py-0.2.2/selfcord/api/gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -333,14 +333,16 @@
         if item:
             if self.fired:
                 log.info(f"{item}")
             try:
                 item = self.zlib.decompress(item)
             except Exception as e:
                 log.error(f"Could not decompress\n{e}")
+                await self.close()
+                await self.connect()
             item = ujson.loads(item)  # Get json message from gateway
 
             op = item.get("op")  # Op code
             data = item.get("d")  # Data
             event = item.get("t")  # The event
             s = item.get("s")
             if op == self.RECONNECT:
@@ -473,14 +475,15 @@
         self.alive = True
         payload = {
             "op": 6,
             "d": {"token": self.token, "session_id": self.bot.session_id, "seq": seq},
         }
         await self.send_json(payload)
 
+
     async def connect(self):
         """Connect to discord gateway"""
         self.ws = await websockets.connect(
             "wss://gateway.discord.gg/?encoding=json&v=9&compress=zlib-stream",
             origin="https://discord.com",
             max_size=None,
         )
@@ -493,24 +496,43 @@
         self.alive = False
         await self.ws.close()
         if self.debug:
             log.debug("Closed connection to discord gateway")
 
     async def identify(self):
         """Identify to gateway, uses amazing mobile client spoof"""
+        
         payload = {
             "op": 2,
             "d": {
+                "capabilities": 4079,
                 "token": self.token,
+                "client_state": {
+                    "api_code_version": 0,
+                    "highest_last_message_id": "0",
+                    "initial_guild_id": None,
+                    "private_channels_version": "0",
+                    "read_state_version": 0,
+                    "user_guild_settings_version": -1,
+                    "user_settings_version": -1,
+                },
+                "compress": False,
+                "presence": {
+                    "activities": [],
+                    "afk": False,
+                    "since": 0,
+                    "status": "dnd"
+                },
                 "properties": {
-                    "$os": "android",
-                    "$browser": "Discord Android",
-                    "$device": "Discord Android",
-                    "$referrer": "",
-                    "$referring_domain": "",
+                    "os": "Android",
+                    "browser": "Discord Android",
+                    "device": "Discord Android",
+                    "browser_useragent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) discord/0.0.157 Chrome/108.0.5359.215 Electron/22.3.2 Safari/537.36",
+                    "system-locale": "en-GB",
+                    "os_arch": "x64"
                 },
             },
         }
         await self.send_json(payload)
         if self.debug:
             log.debug("Sent identify payload")
             log.info(f"Idenitified with {self.token} under Discord Android")
```

### Comparing `selfcord.py-0.2.1/selfcord/api/http.py` & `selfcord.py-0.2.2/selfcord/api/http.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import random
 from base64 import b64encode
 from traceback import format_exception
 from typing import TYPE_CHECKING
 
 import aiohttp
 import ujson
+from aioconsole import aprint
 from aiohttp import ClientSession
 
 from ..models import Client, User
 from ..utils import logging
 
 lib, _, _ = __name__.partition(".")
 log = logging.getLogger(__name__)
@@ -79,15 +80,15 @@
         if self.debug:
             log.debug("Gathered cookie and fingerprint")
             log.info(f"Fingerprint Gathered: {self.fingerprint}")
 
     def remove_dupes(self, dictionary: dict):
         return set(dictionary)
 
-    async def request(self, method: str, endpoint: str, *args, **kwargs) -> dict:
+    async def request(self, method: str, endpoint: str, *args, **kwargs) -> dict | None:
         """Used to send requests
 
         Args:
             method (str): HTTP method
             endpoint (str): Discord api endpoint
 
         Raises:
@@ -133,41 +134,42 @@
                     if self.debug:
                         log.debug(f"Sent Request Method: {method} URL: {url} Payload: {args} {kwargs}")
 
                     if resp.status == 429:
                         try:
                             json = await resp.json()
                             await asyncio.sleep(json["retry_after"])
-                            if self.debug:
-                                log.error(f"429 Ratelimited: {json}")
+                            log.error(f"429 Ratelimited: {json}")
                             continue
                         except Exception as e:
                             error = "".join(format_exception(e, e, e.__traceback__))
                             text = await resp.text()
+                            
                             log.error(f"Error upon parsing json : {text}")
-                            if self.debug:
-                                log.error(f"Error upon parsing json : \n{error}")
-                                log.info(
-                                    f"Attempted to send request to URL: {url} PAYLOAD: {kwargs}"
-                                )
-                            raise Exception(e) from e
+                            log.error(f"Error upon parsing json : \n{error}")
+                            log.info(
+                                f"Attempted to send request to URL: {url} PAYLOAD: {kwargs}"
+                            )
+                            await aprint(error)
+                            return None
 
                     elif resp.status == 401:
                         json = await resp.json()
                         log.error(f"{json} -- {resp.status}")
-                        raise Exception(f"{json}")
+                        await aprint(json)
+                        return None
 
                     elif resp.status == 403:
                         json = await resp.json()
                         log.error(f"403 Unauthorized: {json}")
-                        if self.debug:
-                            log.info(
-                                f"Attempted to send request to URL: {url} PAYLOAD: {args} {kwargs}"
-                            )
-                        raise Exception(f"{json}")
+                        log.info(
+                            f"Attempted to send request to URL: {url} PAYLOAD: {args} {kwargs}"
+                        )
+                        await aprint(json)
+                        return None
 
                     elif resp.status == 201:
                         data = await resp.json()
                         break
 
                     elif resp.status == 204:
                         data = await resp.text()
@@ -181,19 +183,21 @@
                         if self.debug:
                             log.error(f"Unknown Error: {resp.status}")
                             log.info(
                                 f"Attempted to send request to URL: {url} PAYLOAD: {args} {kwargs}"
                             )
                         try:
                             json = await resp.json()
-                            raise Exception(f"{json}")
+                            await aprint(json)
+                            return None
                         except Exception as e:
                             error = "".join(format_exception(e, e, e.__traceback__))
                             log.error(f"Unable to log response: \n{error}")
-                            raise Exception(e) from e
+                            await aprint(error)
+                            return None
         try:
             if resp.headers["set-cookie"]:
                 dcf = resp.headers["set-cookie"].split("__dcfduid=")[0].split(";")[0]
                 sdc = resp.headers["set-cookie"].split("__sdcfduid=")[0].split(";")[0]
                 cfr = resp.headers["set-cookie"].split("__cfruid=")[0].split(";")[0]
                 bm = resp.headers["set-cookie"].split("__cf_bm=")[0].split(";")[0]
```

### Comparing `selfcord.py-0.2.1/selfcord/api/voice/voice.py` & `selfcord.py-0.2.2/selfcord/api/voice/voice.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.1/selfcord/bot.py` & `selfcord.py-0.2.2/selfcord/bot.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import contextlib
 import importlib
 import inspect
 import io
 import os
 import random
 import time
+import urllib
 from collections import defaultdict
 from traceback import format_exception
 from typing import TYPE_CHECKING
 from urllib.parse import urlparse
 
 import aiofiles
 import aiohttp
@@ -557,14 +558,33 @@
         """
         await self.http.request("patch", "/users/@me", json={"password": old_pass, "new_password": new_pass})
     
     async def get_sessions(self) -> list[Session] | None:
         data = await self.http.request("get", "/auth/sessions")
         if data.get("user_sessions") is not None:
             return [Session(data, self, self.http) for data in data["user_sessions"]]
+    
+
+    async def reset_relationship(self, user_id: str):
+        """
+        Function remove a specific user from friends or unblocks a user
+
+        Args:
+            user_id (str) : user to remove
+        """
+        await self.http.request("delete", f"/users/@me/relationships/{user_id}")
+
+    async def block(self, user_id: str):
+        """
+        Function to block a user
+        
+        Args:
+            user_id (str) : user to block
+        """
+        await self.http.request("put", f"/users/@me/relationships/{user_id}", json={"type": 2})
 
     async def add_friend(self, user_id: str):
         """
         Function to add a specific user as a friend.
 
         Args:
             user_id (str): ID of the possible random user.
@@ -645,29 +665,30 @@
             )
             if self.debug:
                 log.debug("Created DM Channel")
             return DMChannel(data, bot=self, http=self.http)
         else:
             log.error("Recipient ID not specified")
 
-    async def join_guild(self, code: str) -> Guild | None:
-        """Helper function to join guilds
+    async def join_invite(self, code: str) -> Guild | None:
+        """Helper function to join invites
         
         Args:
             code (str): Invite Code
         Returns:
             Guild object | None
         """
         data = await self.http.request("post", f"/invites/{code}", json = {
             "session_id": f"{self.session_id}"
         }
         )
-        if data is not None:
+        try:
             return Guild(data['guild'], self, self.http)
-        return None
+        except:
+            return GroupChannel(data['channel'], self, self.http)
     async def redeem_nitro(self, code: str):
         """Helper function to redeem nitro
 
         Args:
             code (str): Nitro code
         """
         async with aiohttp.ClientSession() as session:
@@ -713,7 +734,51 @@
             afk (bool): True or False
             activity (dict): Selfcord.Activity method.
         """
         await self.gateway.change_presence(status, afk, activity=activity)
         if self.debug:
             log.debug("Finished changing presence")
             log.info(f"Changed Status to {status}, AFK to {afk}")
+
+    async def change_status(self, status: str, message: str | None = None, emoji: str | None = None):
+        """
+        Change status for yourself
+
+        Args:
+            status (str) : online, offline, dnd, invisible
+            message (str | None) : message for custom status
+            emoji (str | None) : emoji for custom status
+        """
+        json = {"status": status}
+        if message is not None:
+            if "custom_status" in json:
+                json['custom_status'].update({"text": message})
+            else:
+                json['custom_status'] = {"text": message}
+        if emoji is not None:
+            emoji = emoji.encode("utf-8").decode("utf-8")
+            if "custom_status" in json:
+                json['custom_status'].update({"emoji_name": emoji})
+            else:
+                json['custom_status'] = {"emoji_name": emoji}
+
+        await self.http.request("patch", "/users/@me/settings", json=json)
+
+    async def friend_invite(self):
+        """Get discord friend invite for specified ID"""
+        json = await self.http.request("post", "/users/@me/invites", json={"max_age":0,"max_uses":0,"target_type":None, "flags":0})
+        return json['code']
+
+    async def view_invites(self):
+        """View discord friend invites"""
+        json = await self.http.request("get", "/users/@me/invites")
+        invites = []
+        for items in json:
+            invite = {}
+            for key, value in items.items():
+                if key == "code":
+                    invite['code'] = value
+                if key == "expires_at":
+                    invite['expiry'] = value
+            if invite.get("code") is not None and invite.get("expiry") is not None:
+                invites.append(invite)
+        return invites
```

### Comparing `selfcord.py-0.2.1/selfcord/models/__init__.py` & `selfcord.py-0.2.2/selfcord/models/__init__.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.1/selfcord/models/channel.py` & `selfcord.py-0.2.2/selfcord/models/channel.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         content: str | None = None,
         author: str | None = None,
         mentions: str | None = None,
         has: str | None = None,
         before: float | None = None,
         after: float | None = None,
         offset: int | None = None,
+        pinned: bool | None = None
         ):
         """
         Search through channel with specific parameters
 
         Args:
             content (str) : Content to search for.
             author (str) : Author to search for.
@@ -68,14 +69,15 @@
             "content": content,
             "author_id": author,
             "mentions": mentions,
             "has": has,
             "max_id": before,
             "min_id": after,
             "offset": offset,
+            "pinned": pinned,
         }
         index = 0
         for key, value in params.items():
             if value is not None:
                 index += 1
                 param = f"{key}={value}"
                 if index == 1:
@@ -83,17 +85,23 @@
                 else:
                     param = "&" + param
                 url += param
                 
         json = await self.http.request("get", url)
         total = json.get("total_results")
         messages = json['messages']if json.get("messages") is not None else []
-        
-        messages = [Message(msg, self.bot, self.http) for msgs in messages for msg in msgs]
-        return total, messages
+        new_msgs = []
+        for msgs in messages:
+            for msg in msgs:
+                msg = Message(msg, self.bot, self.http)
+                if msg.guild_id is None:
+                    if hasattr(self, "guild_id"):
+                        setattr(msg, "guild_id", self.guild_id)
+                new_msgs.append(msg)
+        return total, new_msgs
         
 
     async def history(self, amount: int = 100, user: bool = False) -> list[Message] | None:
         """
         Get channel message history.
 
         Args:
@@ -169,15 +177,16 @@
                     pass
             items.append({"uploaded_filename": upload_filename, "filename": os.path.basename(upload_filename) , "id": id})
         return items
     
     async def delayed_delete(self, message: Message, time: int):
         await asyncio.sleep(time)
         await message.delete()
-
+    
+    
 
     async def purge(self, amount: int = 0) -> None:
         """
         Delete a number of messages, starting from the most recent.
 
         Args:
             amount(int) : Number of messages to purge/delete.
@@ -204,14 +213,15 @@
                         for message in msgs[i : i + 3]
                     )
                 )
                 await asyncio.sleep(0.4)
         else:
             while True:
                 if len(msgs) >= amount:
+                    msgs = msgs[:amount]
                     break
                 _, new_msgs = await self.search(author=self.bot.user.id, offset=len(msgs))
                 msgs += new_msgs
                 if len(new_msgs) == 0:
                     break
             for i in range(0, len(msgs), 3):
                 await asyncio.gather(
@@ -220,19 +230,15 @@
                         for message in msgs[i : i + 3]
                     ),
                 )
                 await asyncio.sleep(0.4)
 
 
 
-
-        
-
-
-    async def spam(self, amount: int, content: str, file_paths: list[str] = [], tts=False) -> None:
+    async def spam(self, amount: int, content, file_paths: list[str] = [], tts=False) -> None:
         """
         Send multiple of the same message.
 
         Args:
             - amount(int) : Number of spam messages to send.
             - content(str) : The message to send.
             - tts(bool) = False : Specify whether it is a TTS message.
@@ -257,15 +263,15 @@
         Args:
             - content(str) : Message content. Should be string type or similar. Discord `embed` type is not allowed.
             - tts(bool) : Specify whether message is text-to-speech or not
 
         Returns:
             Message object.
         """
-        json = {"content": content, "nonce": self.make_nonce, "tts": tts}
+        json = {"content": str(content), "nonce": self.make_nonce, "tts": tts}
         if file_paths != []:
             vals = await self.upload_image(file_paths)
             json |= {"attachments" : vals}
 
         if hasattr(self, "guild_id"):
             resp = await self.http.request(
                 method="post",
@@ -289,27 +295,27 @@
                 json=json
             )
         if delete_after is not None:
             asyncio.create_task(self.delayed_delete(Message(resp, self.bot, self.http), delete_after))
 
         return Message(resp, self.bot, self.http)
 
-    async def reply(self, message: Message, content: str, file_paths: list[str] = [], delete_after: int | None = None, tts=False) -> Message:
+    async def reply(self, message: Message, content, file_paths: list[str] = [], delete_after: int | None = None, tts=False) -> Message:
         """Reply to a specific message
 
         Args:
             message (str): Message to reply to
             content (_type_, optional): Message content to reply with. Defaults to None.
             tts (bool, optional): Specify whether message is text-to-speech or not. Defaults to False.
 
         Returns:
             Message object.
         """
         json = {
-            "content": content,
+            "content": str(content),
             "tts": tts,
             "nonce": self.make_nonce,
             "message_reference": {
                 "channel_id": f"{self.id}",
                 "message_id": f"{message.id}",
             },
         }
@@ -438,20 +444,22 @@
 
         self.topic = data.get("topic")
         self.rate_limit_per_user = data.get("rate_limit_per_user")
         self.position = data.get("position")
         self.name = data.get("name")
         self.id = data.get("id")
         self.guild_id = data.get("guild_id")
+        self.guild = self.bot.get_guild(self.guild_id)
         self.last_message_id = data.get("last_message_id")
         self.flags = data.get("flags")
         self.default_thread_rate_limit_per_user = data.get(
             "default_thread_rate_limit_per_user"
         )
         self.category_id = data.get("parent_id")
+        self.permission_overwrites = data.get("permission_overwrites")
 
     async def delete(self):
         """
         Deletes the text channel object.
 
         Args:
             No arguments required
@@ -549,14 +557,80 @@
                 "target_type": None,
                 "temporary": False,
                 "flags": 0,
             },
         )
         return "https://discord.gg/" + data["code"]
 
+class ForumChannel(Messageable):
+    """Forum Channel object"""
+    def __init__(self, data: dict, bot: Bot, http: http) -> None:
+        super().__init__(http, bot)
+        self.bot = bot
+        self.http = http
+        self._update(data)
+    
+    def _update(self, data):
+        self.id = data.get("id")
+        self.type = 15
+        self.last_message_id = data.get("last_message_id")
+        self.flags = data.get("flags")
+        self.guild_id = data.get("guild_id")
+        self.guild = self.bot.get_guild(self.guild_id)
+        self.name = data.get("name")
+        self.category_id = data.get("parent_id")
+        self.rate_limit_per_user = data.get("rate_limit_per_user")
+        self.topic = data.get("topic")
+        self.position = data.get("position")
+        self.permission_overwrites = data.get("permission_overwrites")
+        self.available_tags = data.get("available_tags")
+        self.default_reaction = data.get("default_reaction_emoji")
+        self.default_sort = data.get("default_sort_order")
+        self.default_forum_layout = data.get("default_forum_layout")
+        self.icon_emoji = data.get("icon_emoji")
+        self.theme_color = data.get("theme_color")
+
+    async def thread_create(self, name: str, description: str, applied_tags):
+        referer = f"https://discord.com/channels/{self.guild_id}/{self.id}"
+        await self.http.request("post", f"/channels/{self.id}/threads?use_nested_field=true", headers={"origin": "https://discord.com", "referer": referer}, json={"name": name, "message" : { "content": description}, "applied_tags": applied_tags, "auto_archive_duration": 4320})
+
+class ThreadChannel(Messageable):
+    def __init__(self, data: dict, bot: Bot, http: http):
+        super().__init__(http, bot)
+        self.bot = bot
+        self.http = http
+        self._update(data)
+
+    def _update(self, data):
+        self.id = data.get("id")
+        self.type = data.get("type")
+        self.last_message_id = data.get("last_message_id")
+        self.flags = data.get("flags")
+        self.guild_id = data.get("guild_id")
+        self.guild = self.bot.get_guild(self.guild_id)
+        self.name = data.get("name")
+        self.category_id = data.get("parent_id")
+        self.rate_limit_per_user = data.get("rate_limit_per_user")
+        self.bitrate = data.get("bitrate")
+        self.user_limit = data.get("user_limit")
+        self.rtc_region = data.get("rtc_region")
+        self.owner_id = data.get("owner_id")
+        metadata = data.get("thread_metadata")
+        self.archived = metadata.get("archived")
+        self.archive_timestamp = metadata.get("archive_timestamp")
+        self.auto_archive_duration = metadata.get("auto_archive_duration")
+        self.locked = metadata.get("locked")
+        self.create_timestamp = metadata.get("create_timestamp")
+        self.message_count = data.get("message_count")
+        self.member_count = data.get("member_count")
+        self.total_message_sent = data.get("total_message_sent")
+        self.member_ids = data.get("member_ids_preview")
+        self.members = [User(id, self.bot, self.http) if data.get("member_ids") is not None else [] for id in data['member_ids']]
+
+        
 
 class VoiceChannel(Voiceable, Messageable):
     """Voice Channel Object"""
 
     def __init__(self, data: dict, bot: Bot, http: http) -> None:
         super().__init__(http, bot)
         self.permissions: list[Permission] = []
@@ -576,22 +650,25 @@
 
         Args:
             data (dict): JSON data from gateway
         """
         self.name = data.get("name")
         self.id = data.get("id")
         self.guild_id = data.get("guild_id")
+        self.guild = self.bot.get_guild(self.guild_id)
         self.last_message_id = data.get("last_message_id")
         self.rtc_region = data.get("rtc_region")
         self.flags = data.get("flags")
         self.bitrate = data.get("bitrate")
         self.rate_limit_per_user = data.get("rate_limit_per_user")
         self.position = data.get("position")
         self.category_id = data.get("parent_id")
+        self.permission_overwrites = data.get("permission_overwrites")
 
+        
     async def delete(self):
         """
         Deletes the voice channel object.
         """
         await self.http.request(method="delete", endpoint=f"/channels/{self.id}")
         del self
 
@@ -671,16 +748,19 @@
 
         Args:
             data (dict): JSON data from gateway
         """
         self.name = data.get("name")
         self.id = data.get("id")
         self.guild_id = data.get("guild_id")
+        self.guild = self.bot.get_guild(self.guild_id)
         self.position = data.get("position")
         self.flags = data.get("flags")
+        self.permission_overwrites = data.get("permission_overwrites")
+
 
     async def delete(self):
         """Deletes the Category object."""
         await self.http.request(method="delete", endpoint=f"/channels/{self.id}")
         del self
 
 
@@ -736,16 +816,15 @@
 
     def _update(self, data: dict):
         """Updater method intended to create the attributes for the object
 
         Args:
             data (dict): JSON data from gateway
         """
-        for user in data.get("recipients"):
-            self.recipients.append(User(user, self.bot, self.http))
+        self.recipients = [User(data, self.bot, self.http) if data.get("recipients") is not None else [] for data in data['recipients']]
         self.name = data.get("name")
         self.owner_id = data.get("owner_id")
         self.last_message_id = data.get("last_message_id")
         self.id = data.get("id")
         self.flags = data.get("flags")
         self.icon = data.get("icon")
```

### Comparing `selfcord.py-0.2.1/selfcord/models/client.py` & `selfcord.py-0.2.2/selfcord/models/client.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.1/selfcord/models/emoji.py` & `selfcord.py-0.2.2/selfcord/models/emoji.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.1/selfcord/models/guild.py` & `selfcord.py-0.2.2/selfcord/models/guild.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 import random
 from datetime import datetime, timedelta, timezone
 from itertools import zip_longest
 from typing import TYPE_CHECKING
 
-from .channel import Category, Messageable, TextChannel, VoiceChannel
+from .channel import (Category, ForumChannel, Messageable, TextChannel,
+                      ThreadChannel, VoiceChannel)
 from .emoji import Emoji
 from .role import Role
 from .user import User
 
 if TYPE_CHECKING:
     from ..api import http
     from ..bot import Bot
@@ -84,31 +85,105 @@
                 self.members.append(user)
 
             if channel != None:
                 type = channel.get("type")
                 if type == self.TEXTCHANNEL or type not in [
                     self.VOICECHANNEL,
                     self.CATEGORY,
+                    self.GUILD_FORUM
                 ]:
                     channel = TextChannel(channel, self.bot, self.http)
                 elif type == self.VOICECHANNEL:
                     channel = VoiceChannel(channel, self.bot, self.http)
+                elif type == self.GUILD_FORUM:
+                    channel = ForumChannel(channel, self.bot, self.http)
+                elif type in [self.PUBLIC_THREAD, self.PRIVATE_THREAD]:
+                    channel = ThreadChannel(channel, self.bot, self.http)
                 else:
                     channel = Category(channel, self.bot, self.http)
                 channel.guild_id = self.id
                 self.channels.append(channel)
             if role != None:
                 role = Role(role, self.bot, self.http, guild_id=self.id)
                 self.roles.append(role)
 
             if emoji != None:
                 emoji = Emoji(emoji, self.bot, self.http)
                 emoji.guild_id = self.id
                 self.emojis.append(emoji)
 
+    async def search(
+        self,
+        content: str | None = None,
+        author: str | None = None,
+        mentions: str | None = None,
+        has: str | None = None,
+        before: float | None = None,
+        after: float | None = None,
+        offset: int | None = None,
+        pinned: str | None = None,
+        channel: str | None = None
+    ):
+        """
+        Search through channel with specific parameters
+
+        Args:
+            content (str) : Content to search for.
+            author (str) : Author to search for.
+            mentions (str) : Mention to search for.
+            has (str) : Message that contains (file, image, video, etc).
+            before (time) : Before a timestamp.
+            after (time) : After a timestamp.
+            offset (int) : How many messages after to search.
+
+        Returns:
+            total (int) : Total amount of messages possible of receiving.
+            messages (list[Message]) : List of message objects gathered
+
+        """
+        from selfcord.models import Message
+        url = f"/guilds/{self.id}/messages/search"
+        params = {
+            "content": content,
+            "author_id": author,
+            "mentions": mentions,
+            "has": has,
+            "max_id": before,
+            "min_id": after,
+            "offset": offset,
+            "pinned": pinned,
+            "channel_id": channel,
+        }
+        index = 0
+        for key, value in params.items():
+            if value is not None:
+                index += 1
+                param = f"{key}={value}"
+                if index == 1:
+                    param = "?" + param
+                else:
+                    param = "&" + param
+                url += param
+
+        json = await self.http.request("get", url)
+        total = json.get("total_results")
+        messages = json['messages']if json.get("messages") is not None else []
+        
+        new_msgs = []
+        for msgs in messages:
+            for msg in msgs:
+                msg = Message(msg, self.bot, self.http)
+                if msg.guild_id is None:
+                    setattr(msg, "guild_id", self.id)
+                new_msgs.append(msg)
+        return total, new_msgs
+ 
+
+
+
     async def ban(self, user_id: str):
         """Bans a user from the guild
 
         Args:
             user_id (str): User ID specified to ban
         """
         await self.http.request(
@@ -143,15 +218,15 @@
         )
         await self.http.request(
             method="patch",
             endpoint=f"/guilds/{self.id}/members/{user_id}",
             json={"communication_disabled_until": str(duration)},
         )
 
-    async def txt_channel_create(self, name: str, parent_id: str = None):
+    async def txt_channel_create(self, name: str, parent_id: str | None= None):
         """Creates a Text Channel in the guild
 
         Args:
             name (str): Name of the channel
             parent_id (str, optional): ID of the category. Defaults to None.
         """
         payload = {"name": name, "permission_overwrites": [], "type": 0}
@@ -159,14 +234,27 @@
             payload["parent_id"] = parent_id
 
         channel = await self.http.request(
             method="post", endpoint=f"/guilds/{self.id}/channels", json=payload
         )
         return TextChannel(channel, self.bot, self.http)
 
+    async def forum_channel_create(self, name: str, parent_id : str | None = None):
+        """Creates a Forum channel in the guild
+
+        Args:
+            name (str): Name of the channel
+            parent_id  (str, optional): ID of the category, defaults to None.
+        """
+        payload = {"name": name, "permission_overwrites": [], "type": 15}
+        if parent_id is not None:
+            payload['parent_id'] = parent_id
+
+        return ForumChannel((await self.http.request("post", f"/guilds/{self.id}/channels", json=payload)), self.bot, self.http)
+
     async def vc_channel_create(self, name: str):
         """Creates a voice channel in the guild
 
         Args:
             name (str): Name of the channel
         """
         channel = await self.http.request(
```

### Comparing `selfcord.py-0.2.1/selfcord/models/interactions.py` & `selfcord.py-0.2.2/selfcord/models/interactions.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.1/selfcord/models/member.py` & `selfcord.py-0.2.2/selfcord/models/member.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.1/selfcord/models/message.py` & `selfcord.py-0.2.2/selfcord/models/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,14 @@
             "nonce": self.message.make_nonce,
             "session_id": self.bot.session_id,
             "type": 3,
         }
         if self.message.guild_id is not None:
             json['guild_id'] = self.message.guild_id
         json = await self.http.request("post", "/interactions", json=json)
-        log.info(json)
 
 
 
 class Action_Row:
     ACTION_ROW = 1
     BUTTON = 2
     STRING_SELECT = 3
@@ -85,15 +84,15 @@
             self.components = []
             for component in components:
                 if component.get("type") == self.BUTTON:
                     self.components.append(Button(component, message, self.bot, self.http))
                 elif component.get("type") in [self.STRING_SELECT, self.USER_SELECT, self.ROLE_SELECT, self.CHANNEL_SELECT, self.MENTIONABLE_SELECT]:
                     self.components.append(Select_Menu(component, message, self.bot, self.http))
                 elif component.get("type") == self.TEXT_INPUT:
-                    self.components.append(Text_Input(component, message, self.bot, self.http))
+                    self.components.append(Text_Input(component, self.bot, self.http))
         else:
             self.components = []
         
 class Select_Menu:
     TYPES = {
         "STRING_SELECT" : 3,
         "USER_SELECT" : 5,
@@ -118,29 +117,38 @@
             self.channel_types = data.get("channel_types")
         self.placeholder = data.get("placeholder")
         self.min_values = data.get("min_values")
         self.max_values = data.get("max_values")
         self.disabled = data.get("disabled")
 
 class Text_Input:
-    def __init__(self, data: dict, message: Message, bot: Bot, http: http) -> None:
-        self._update(data, message)
+    def __init__(self, data: dict, bot: Bot, http: http) -> None:
+        self.bot = bot
+        self.http = http
+        self._update(data)
 
-    def _update(self, data: dict, message: Message):
+    def _update(self, data: dict):
         self.type = 4
-        self.message = message
         self.custom_id = data.get("custom_id")
         self.style = data.get("style")
         self.label = data.get("label")
         self.min_length = data.get("min_length")
         self.max_length = data.get("max_length")
         self.required = data.get("required")
         self.value = data.get("value")
         self.placeholder = data.get("placeholder")
+        self.id = data.get("id")
 
+    
+    async def trigger(self, value: str, message: Message, comp_id: str):
+        comp_id = "form_" + comp_id
+        json = {"type": 5, "application_id": message.author.id, "channel_id": message.channel_id, "data": {"id": self.id, "custom_id": comp_id, "components": [{"type": 1, "components": [{"type": self.type, "custom_id":self.custom_id, "value": value,}]}]}, "session_id": self.bot.session_id, "nonce": message.make_nonce}
+        if message.guild_id is not None:
+            json['guild_id'] = message.guild_id
+        await self.http.request("post", "/interactions", json=json)
 
 class Select_Option:
     def __init__(self, data) -> None:
         self._update(data)
 
     def _update(self, data):
         self.label = data.get("label")
@@ -200,15 +208,15 @@
             if component.get("type") == 1:
                 self.components.append(Action_Row(component, self, self.bot, self.http))
             elif component.get("type") == 2:
                 self.components.append(Button(component, self, self.bot, self.http))
             elif component.get("type") in [self.STRING_SELECT, self.USER_SELECT, self.ROLE_SELECT, self.CHANNEL_SELECT, self.MENTIONABLE_SELECT]:
                 self.components.append(Select_Menu(component, self, self.bot, self.http))
             elif component.get("type") == 4:
-                self.components.append(Text_Input(component, self, self.bot, self.http))
+                self.components.append(Text_Input(component, self.bot, self.http))
             else:
                 self.components.append(component)
 
         self.timestamp = time.time()
         self.channel_id = data.get("channel_id")
 
         attachments = data.get("attachments")
@@ -221,14 +229,18 @@
                 self.mentions.append(User(mention, self.bot, self.http))
         self.guild_id = data.get("guild_id")
 
         self.channel = self.bot.get_channel(self.channel_id)
 
         self.guild = self.bot.get_guild(self.guild_id)
 
+    async def thread_create(self, name: str):
+        """Create a thread for message object"""
+        await self.http.request("post", f"/channels/{self.channel_id}/messages/{self.id}/threads", headers={"origin": "https://discord.com", "referer": f"https://discord.com/{self.guild_id}/self.channel_id"}, json = {"name": name, "auto_archive_duration": 4320, "location": "Message", "type": 11})
+
     async def delete(self):
         """Delete the Message Object"""
         await self.http.request(
             method="delete", endpoint=f"/channels/{self.channel_id}/messages/{self.id}"
         )
 
     async def edit(self, content: str, file_paths: list[str] = [], delete_after: int | None = None) -> Message:
```

### Comparing `selfcord.py-0.2.1/selfcord/models/permission.py` & `selfcord.py-0.2.2/selfcord/models/permission.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.1/selfcord/models/role.py` & `selfcord.py-0.2.2/selfcord/models/role.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.1/selfcord/models/sessions.py` & `selfcord.py-0.2.2/selfcord/models/sessions.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.1/selfcord/models/user.py` & `selfcord.py-0.2.2/selfcord/models/user.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.1/selfcord/models/webhook.py` & `selfcord.py-0.2.2/selfcord/models/webhook.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.1/selfcord/utils/command.py` & `selfcord.py-0.2.2/selfcord/utils/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -473,35 +473,35 @@
                 args.insert(0, self)
         try:
             await func(*args, **kwargs)
         except Exception as e:
             error = "".join(format_exception(e, e, e.__traceback__))
             log.error(f"Could not run command \n{error}")
 
-    async def reply(self, content: str, file_paths: list[str] = [], delete_after: int | None = None, tts=False) -> Message:
+    async def reply(self, content, file_paths: list[str] = [], delete_after: int | None = None, tts=False) -> Message:
         """Helper function to reply to your own message containing the command
 
         Args:
             content (str): The message you would like to send
             tts (bool, optional): Whether message should be tts or not. Defaults to False.
         """
         message: Message = await self.channel.reply(self.message, content, file_paths, delete_after, tts)
         return message
 
-    async def send(self, content: str, file_paths: list[str] = [], delete_after: int | None = None, tts=False) -> Message:
+    async def send(self, content, file_paths: list[str] = [], delete_after: int | None = None, tts=False) -> Message:
         """Helper function to send message to the current channel
 
         Args:
             content (str): The message you would like to send
             tts (bool, optional): Whether message should be tts or not. Defaults to False.
         """
         message: Message = await self.channel.send(content=content, file_paths=file_paths, delete_after=delete_after, tts=tts)
         return message
 
-    async def spam(self, amount: int, content: str, file_paths: list[str] = [], tts: bool = False):
+    async def spam(self, amount: int, content, file_paths: list[str] = [], tts: bool = False):
         """Helper function to spam messages in the current channel (uses asyncio.gather !!!!)
 
         Args:
             amount (int): Amount of messages to spam
             content (str): The message you would like to send
         """
         await self.channel.spam(amount, content, file_paths, tts)
@@ -510,15 +510,15 @@
         """Helper function to purge messages in the current channel, uses asyncio gather.
 
         Args:
             amount (int): The amount of messages to purge, defaults to All.
         """
         await self.channel.purge(amount)
 
-    async def edit(self, content: str, file_paths: list[str] = [], delete_after: int | None = None) -> Message:
+    async def edit(self, content, file_paths: list[str] = [], delete_after: int | None = None) -> Message:
         """Helper function to edit the message you sent
 
         Args:
             content (str): Content to edit to
         """
         message = await self.message.edit(content, file_paths, delete_after)
         return message
```

### Comparing `selfcord.py-0.2.1/selfcord/utils/logging.py` & `selfcord.py-0.2.2/selfcord/utils/logging.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.1/selfcord.py.egg-info/PKG-INFO` & `selfcord.py-0.2.2/selfcord.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: selfcord.py
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Discord API wrapper designed for selfbots!
 Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell
 License: MIT
 Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown
 Provides-Extra: voice
+License-File: LICENSE
 
 <div align="center">
 <img src="./logo.png" widht="180" height="180" style="border-radius: 100%;">
 <h1 align="center">SELFCORD</h1>
 <strong><i>A Powerful Library for Discord Selfbots</i></strong>
 <br>
 <br>
 <a href="https://www.python.org/">
 <img src="https://img.shields.io/badge/MADE%20WITH-PYTHON-red?logoColor=red&logo=Python&style=for-the-badge">
 </a>
 <a href="https://pypi.org/project/selfcord/">
-<img src="https://img.shields.io/badge/version-0.2.1-blue?logo=adguard&style=for-the-badge">
+<img src="https://img.shields.io/badge/version-0.2.2-blue?logo=adguard&style=for-the-badge">
 </a>
 <a href="https://github.com/Shell1010/Selfcord/wiki">
 <img src="https://img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge">
 </a>
 </div>
 
 ## Feautres
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 2.1 Name: selfcord.py Version: 0.2.1 Summary: A Discord API
+Metadata-Version: 2.1 Name: selfcord.py Version: 0.2.2 Summary: A Discord API
 wrapper designed for selfbots! Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell License: MIT Keywords: selfbot,discord,discordapi,discordwrapper
-Description-Content-Type: text/markdown Provides-Extra: voice
+Description-Content-Type: text/markdown Provides-Extra: voice License-File:
+LICENSE
                                  [./logo.png]
                             ****** SELFCORD ******
                    A Powerful Library for Discord Selfbots
 
                [https://img.shields.io/badge/MADE%20WITH-PYTHON-
   red?logoColor=red&logo=Python&style=for-the-badge] [https://img.shields.io/
-     badge/version-0.2.1-blue?logo=adguard&style=for-the-badge] [https://
+     badge/version-0.2.2-blue?logo=adguard&style=for-the-badge] [https://
   img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge]
 ## Feautres - Modern Pythonic API using `async`/`await` syntax - Easy to use
 with an object oriented design - Optimised for both speed and memory - Prevents
 detection of user account automation - Clean Documentation - Community Support
 ## Installation Python 3.10 or higher is required. ``` pip install selfcord.py
 ``` ## Wiki Read our [Wiki](https://github.com/Shell1010/Selfcord/wiki) in
 regards to documentation and getting started. ## Getting Started A selfbot that
```

### Comparing `selfcord.py-0.2.1/selfcord.py.egg-info/SOURCES.txt` & `selfcord.py-0.2.2/selfcord.py.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 selfcord/__init__.py
 selfcord/bot.py
 selfcord.py.egg-info/PKG-INFO
 selfcord.py.egg-info/SOURCES.txt
 selfcord.py.egg-info/dependency_links.txt
```

### Comparing `selfcord.py-0.2.1/setup.py` & `selfcord.py-0.2.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
                 "selfcord",
                 "selfcord.api",
                 "selfcord.utils",
                 "selfcord.models",
                 "selfcord.api.voice",
             ]
         ),
-        version="0.2.1",
+        version="0.2.2",
         description="A Discord API wrapper designed for selfbots!",
         readme="README.md",
         author="Shell",
         extras_require={"voice": ["pynacl==1.5.0", "opuslib==3.0.1"]},
         license="MIT",
         install_requires=[
             "aiohttp==3.7.4.post0",
```

