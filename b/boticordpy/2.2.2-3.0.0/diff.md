# Comparing `tmp/boticordpy-2.2.2.tar.gz` & `tmp/boticordpy-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\boticordpy-2.2.2.tar", last modified: Sat Sep 10 13:34:42 2022, max compression
+gzip compressed data, was "boticordpy-3.0.0.tar", last modified: Sat Jul  1 06:31:59 2023, max compression
```

## Comparing `boticordpy-2.2.2.tar` & `boticordpy-3.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2022-09-10 13:34:42.000000 boticordpy-2.2.2/
--rw-rw-rw-   0        0        0     1060 2021-09-16 11:34:57.000000 boticordpy-2.2.2/LICENSE.txt
--rw-rw-rw-   0        0        0     2969 2022-09-10 13:34:42.000000 boticordpy-2.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2341 2022-06-08 16:02:17.000000 boticordpy-2.2.2/README.md
-drwxrwxrwx   0        0        0        0 2022-09-10 13:34:42.000000 boticordpy-2.2.2/boticordpy/
--rw-rw-rw-   0        0        0      404 2022-09-10 13:33:40.000000 boticordpy-2.2.2/boticordpy/__init__.py
--rw-rw-rw-   0        0        0     5542 2022-06-08 16:02:17.000000 boticordpy-2.2.2/boticordpy/autopost.py
--rw-rw-rw-   0        0        0     7543 2022-09-10 13:34:03.000000 boticordpy-2.2.2/boticordpy/client.py
--rw-rw-rw-   0        0        0     1388 2022-06-08 16:02:17.000000 boticordpy-2.2.2/boticordpy/exceptions.py
--rw-rw-rw-   0        0        0     4092 2022-09-10 11:20:22.000000 boticordpy-2.2.2/boticordpy/http.py
--rw-rw-rw-   0        0        0     8864 2022-09-10 11:56:31.000000 boticordpy-2.2.2/boticordpy/types.py
--rw-rw-rw-   0        0        0     4005 2022-06-08 16:02:17.000000 boticordpy-2.2.2/boticordpy/webhook.py
-drwxrwxrwx   0        0        0        0 2022-09-10 13:34:42.000000 boticordpy-2.2.2/boticordpy.egg-info/
--rw-rw-rw-   0        0        0     2969 2022-09-10 13:34:42.000000 boticordpy-2.2.2/boticordpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2022-09-10 13:34:42.000000 boticordpy-2.2.2/boticordpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-10 13:34:42.000000 boticordpy-2.2.2/boticordpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-09-10 13:34:42.000000 boticordpy-2.2.2/boticordpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-09-10 13:34:42.000000 boticordpy-2.2.2/boticordpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-10 13:34:42.000000 boticordpy-2.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1836 2022-09-10 11:20:22.000000 boticordpy-2.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 06:31:59.121819 boticordpy-3.0.0/
+-rw-rw-rw-   0        0        0     1074 2023-06-28 06:47:50.000000 boticordpy-3.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     3291 2023-07-01 06:31:59.122828 boticordpy-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2583 2023-06-28 06:47:50.000000 boticordpy-3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 06:31:59.115682 boticordpy-3.0.0/boticordpy/
+-rw-rw-rw-   0        0        0      421 2023-06-28 06:47:50.000000 boticordpy-3.0.0/boticordpy/__init__.py
+-rw-rw-rw-   0        0        0     6189 2023-06-28 06:47:50.000000 boticordpy-3.0.0/boticordpy/autopost.py
+-rw-rw-rw-   0        0        0     6656 2023-06-28 06:47:50.000000 boticordpy-3.0.0/boticordpy/client.py
+-rw-rw-rw-   0        0        0     3865 2023-06-28 06:47:50.000000 boticordpy-3.0.0/boticordpy/exceptions.py
+-rw-rw-rw-   0        0        0     2995 2023-06-28 06:47:50.000000 boticordpy-3.0.0/boticordpy/http.py
+-rw-rw-rw-   0        0        0    26747 2023-06-28 06:47:50.000000 boticordpy-3.0.0/boticordpy/types.py
+-rw-rw-rw-   0        0        0     4942 2023-06-28 06:47:50.000000 boticordpy-3.0.0/boticordpy/websocket.py
+drwxrwxrwx   0        0        0        0 2023-07-01 06:31:59.121819 boticordpy-3.0.0/boticordpy.egg-info/
+-rw-rw-rw-   0        0        0     3291 2023-07-01 06:31:58.000000 boticordpy-3.0.0/boticordpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-07-01 06:31:59.000000 boticordpy-3.0.0/boticordpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 06:31:58.000000 boticordpy-3.0.0/boticordpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-07-01 06:31:58.000000 boticordpy-3.0.0/boticordpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-01 06:31:58.000000 boticordpy-3.0.0/boticordpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-01 06:31:59.123365 boticordpy-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1990 2023-06-28 06:47:50.000000 boticordpy-3.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `boticordpy-2.2.2/LICENSE.txt` & `boticordpy-3.0.0/LICENSE.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2021 Victor Kotlin
+Copyright 2021 - 2023 Viktor K (Marakarka)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `boticordpy-2.2.2/PKG-INFO` & `boticordpy-3.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: boticordpy
-Version: 2.2.2
-Summary: A Python wrapper for BotiCord API
-Home-page: https://github.com/boticord/boticordpy
-Author: Marakarka
-Author-email: support@kerdoku.top
-License: MIT
-Project-URL: Documentation, https://py.boticord.top/en/stable
-Project-URL: Issue tracker, https://github.com/boticord/boticordpy/issues
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >= 3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 <p align="center">
 <img width="520" src="https://media.discordapp.net/attachments/929108234709639208/943873379809787964/boticordpylogo.png" alt="">
 </p>
 
 <p align="center">
   <b>
     The easiest way to use BotiCord API in Python.
@@ -36,20 +18,20 @@
 
 
 <h2>Features</h2>
 
 * Object-oriented
 * Full BotiCord API Coverage
 * Modern Pythonic API using `async`/`await` syntax
-* BotiCord Webhooks
+* BotiCord Websocket
 * It is not necessary to use any particular library used to interact with the Discord API.
 
 <h2>Installation</h2>
 
-<b>Python 3.6 or newer is required.</b>
+<b>Python 3.8 or newer is required.</b>
 
 Enter one of these commands to install the library:
 
 ```
 pip install boticordpy
 ```
 
@@ -63,44 +45,47 @@
 
 You can find other examples in an examples folder. 
 
 **Discord.py Autopost example**
 
 ```py
 from discord.ext import commands
-
 from boticordpy import BoticordClient
 
 bot = commands.Bot(command_prefix="!")
 
 
+# Function that will return the current bot's stats.
 async def get_stats():
     return {"servers": len(bot.guilds), "shards": 0, "users": len(bot.users)}
 
 
+# Function that will be called if stats are posted successfully.
 async def on_success_posting():
-    print("stats posting successfully")
+    print("wow stats posting works")
+
 
-boticord_client = BoticordClient("your_api_token")
+boticord_client = BoticordClient(
+    "your_boticord_api_token", version=3
+)  # <--- BotiCord API token
 autopost = (
     boticord_client.autopost()
     .init_stats(get_stats)
     .on_success(on_success_posting)
-    .start()
+    .start("id_of_your_bot")  # <--- ID of your bot
 )
 
-bot.run("bot token")
+bot.run("bot token")  # <--- Discord bot's token
+
 ```
 
 <h2>Links</h2>
 
 * [PyPi](https://pypi.org/project/boticordpy)
 * [Documentation](https://py.boticord.top)
 * [Github](https://github.com/boticord/boticordpy)
 * [BotiCord](https://boticord.top/)
 * [Support](https://boticord.top/discord)
 
 <h2>Help</h2>
 
 If You need any help we recommend you to check the documentation. You can find us [here](https://bcord.cc/support). Main developer is **[Marakarka](https://boticord.top/profile/585766846268047370)**
-
-
```

#### html2text {}

```diff
@@ -1,34 +1,29 @@
-Metadata-Version: 2.1 Name: boticordpy Version: 2.2.2 Summary: A Python wrapper
-for BotiCord API Home-page: https://github.com/boticord/boticordpy Author:
-Marakarka Author-email: support@kerdoku.top License: MIT Project-URL:
-Documentation, https://py.boticord.top/en/stable Project-URL: Issue tracker,
-https://github.com/boticord/boticordpy/issues Platform: UNKNOWN Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.7 Requires-Python:
->= 3.6 Description-Content-Type: text/markdown License-File: LICENSE.txt
            The easiest way to use BotiCord API in Python.  Â·  Docs
 
 ***** Features *****
 * Object-oriented * Full BotiCord API Coverage * Modern Pythonic API using
-`async`/`await` syntax * BotiCord Webhooks * It is not necessary to use any
+`async`/`await` syntax * BotiCord Websocket * It is not necessary to use any
 particular library used to interact with the Discord API.
 ***** Installation *****
-Python 3.6 or newer is required. Enter one of these commands to install the
+Python 3.8 or newer is required. Enter one of these commands to install the
 library: ``` pip install boticordpy ``` ``` python3 -m pip install boticordpy
 ``` Or just clone the repo: https://github.com/boticord/boticordpy
 ***** Examples *****
 You can find other examples in an examples folder. **Discord.py Autopost
 example** ```py from discord.ext import commands from boticordpy import
-BoticordClient bot = commands.Bot(command_prefix="!") async def get_stats():
-return {"servers": len(bot.guilds), "shards": 0, "users": len(bot.users)} async
-def on_success_posting(): print("stats posting successfully") boticord_client =
-BoticordClient("your_api_token") autopost = ( boticord_client.autopost()
-.init_stats(get_stats) .on_success(on_success_posting) .start() ) bot.run("bot
-token") ```
+BoticordClient bot = commands.Bot(command_prefix="!") # Function that will
+return the current bot's stats. async def get_stats(): return {"servers": len
+(bot.guilds), "shards": 0, "users": len(bot.users)} # Function that will be
+called if stats are posted successfully. async def on_success_posting(): print
+("wow stats posting works") boticord_client = BoticordClient
+( "your_boticord_api_token", version=3 ) # <--- BotiCord API token autopost =
+( boticord_client.autopost() .init_stats(get_stats) .on_success
+(on_success_posting) .start("id_of_your_bot") # <--- ID of your bot ) bot.run
+("bot token") # <--- Discord bot's token ```
 ***** Links *****
 * [PyPi](https://pypi.org/project/boticordpy) * [Documentation](https://
 py.boticord.top) * [Github](https://github.com/boticord/boticordpy) *
 [BotiCord](https://boticord.top/) * [Support](https://boticord.top/discord)
 ***** Help *****
 If You need any help we recommend you to check the documentation. You can find
 us [here](https://bcord.cc/support). Main developer is **[Marakarka](https://
```

### Comparing `boticordpy-2.2.2/boticordpy/autopost.py` & `boticordpy-3.0.0/boticordpy/autopost.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import asyncio
 import typing
+import logging
 
 from . import exceptions as bexc
 
+_logger = logging.getLogger("boticord.autopost")
+
 
 class AutoPost:
     """
     You can use this class to post stats automatically.
 
     Args:
         client (:obj:`~.client.BoticordClient`)
@@ -24,20 +27,24 @@
     )
 
     _success: typing.Any
     _error: typing.Any
     _stats: typing.Any
     _task: typing.Optional["asyncio.Task[None]"]
 
+    bot_id: str
+
     def __init__(self, client):
         self.client = client
         self._stopped: bool = False
         self._interval: int = 900
         self._task: typing.Optional["asyncio.Task[None]"] = None
 
+        self.bot_id = None
+
     @property
     def is_running(self) -> bool:
         """
         Is autopost running?
         """
         return self._task is not None and not self._task.done()
 
@@ -61,14 +68,16 @@
         def inner(func):
             if not asyncio.iscoroutinefunction(func):
                 raise TypeError(f"<{func.__qualname__}> must be a coroutine function")
 
             self._success = callback
             return func
 
+        _logger.info("Registering success callback")
+
         return inner
 
     def on_error(self, callback: typing.Any = None):
         """
         Registers error callback.
 
         .. warning::
@@ -87,14 +96,16 @@
         def inner(func):
             if not asyncio.iscoroutinefunction(func):
                 raise TypeError(f"<{func.__qualname__}> must be a coroutine function")
 
             self._error = callback
             return func
 
+        _logger.info("Registering error callback")
+
         return inner
 
     def init_stats(self, callback: typing.Any = None):
         """
         Registers a function that will return stats. Registered Function Must return dictionary.
 
         .. warning::
@@ -112,14 +123,16 @@
         def inner(func):
             if not asyncio.iscoroutinefunction(func):
                 raise TypeError(f"<{func.__qualname__}> must be a coroutine function")
 
             self._stats = callback
             return func
 
+        _logger.info("Registered stats initialization function")
+
         return inner
 
     @property
     def interval(self) -> float:
         """The interval between posting stats."""
         return self._interval
 
@@ -141,50 +154,63 @@
         self._interval = seconds
         return self
 
     async def _internal_loop(self) -> None:
         while True:
             stats = await self._stats()
             try:
-                await self.client.http.post_bot_stats(stats)
+                await self.client.http.post_bot_stats(self.bot_id, stats)
+                _logger.info("Tried to post bot stats")
             except Exception as err:
                 on_error = getattr(self, "_error", None)
                 if on_error:
                     await on_error(err)
             else:
                 on_success = getattr(self, "_success", None)
                 if on_success:
                     await on_success()
 
             if self._stopped:
                 return None
 
             await asyncio.sleep(self._interval)
 
-    def start(self):
+    def start(self, bot_id: typing.Union[str, int]):
         """
         Starts the loop.
 
+        Args:
+            bot_id ( Union[:obj:`int`, :obj:`str`] )
+                Id of the bot to send stats of.
+
         Raises:
             :obj:`~.exceptions.InternalException`
                 If there's no callback (for getting stats) provided or the autopost is already running.
         """
+
+        self.bot_id = bot_id
+
         if not hasattr(self, "_stats"):
             raise bexc.InternalException("You must provide stats")
 
         if self.is_running:
             raise bexc.InternalException(
                 "Automatically stats posting is already running"
             )
 
         task = asyncio.ensure_future(self._internal_loop())
         self._task = task
+
+        _logger.info("Started autoposting")
+
         return task
 
     def stop(self) -> None:
         """
         Stops the autopost.
         """
         if not self.is_running:
             return None
 
         self._stopped = True
+
+        _logger.info("Stopped autoposting")
```

### Comparing `boticordpy-2.2.2/boticordpy.egg-info/PKG-INFO` & `boticordpy-3.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: boticordpy
-Version: 2.2.2
+Version: 3.0.0
 Summary: A Python wrapper for BotiCord API
 Home-page: https://github.com/boticord/boticordpy
 Author: Marakarka
 Author-email: support@kerdoku.top
 License: MIT
 Project-URL: Documentation, https://py.boticord.top/en/stable
 Project-URL: Issue tracker, https://github.com/boticord/boticordpy/issues
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >= 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <p align="center">
 <img width="520" src="https://media.discordapp.net/attachments/929108234709639208/943873379809787964/boticordpylogo.png" alt="">
 </p>
 
@@ -36,20 +37,20 @@
 
 
 <h2>Features</h2>
 
 * Object-oriented
 * Full BotiCord API Coverage
 * Modern Pythonic API using `async`/`await` syntax
-* BotiCord Webhooks
+* BotiCord Websocket
 * It is not necessary to use any particular library used to interact with the Discord API.
 
 <h2>Installation</h2>
 
-<b>Python 3.6 or newer is required.</b>
+<b>Python 3.8 or newer is required.</b>
 
 Enter one of these commands to install the library:
 
 ```
 pip install boticordpy
 ```
 
@@ -63,44 +64,47 @@
 
 You can find other examples in an examples folder. 
 
 **Discord.py Autopost example**
 
 ```py
 from discord.ext import commands
-
 from boticordpy import BoticordClient
 
 bot = commands.Bot(command_prefix="!")
 
 
+# Function that will return the current bot's stats.
 async def get_stats():
     return {"servers": len(bot.guilds), "shards": 0, "users": len(bot.users)}
 
 
+# Function that will be called if stats are posted successfully.
 async def on_success_posting():
-    print("stats posting successfully")
+    print("wow stats posting works")
+
 
-boticord_client = BoticordClient("your_api_token")
+boticord_client = BoticordClient(
+    "your_boticord_api_token", version=3
+)  # <--- BotiCord API token
 autopost = (
     boticord_client.autopost()
     .init_stats(get_stats)
     .on_success(on_success_posting)
-    .start()
+    .start("id_of_your_bot")  # <--- ID of your bot
 )
 
-bot.run("bot token")
+bot.run("bot token")  # <--- Discord bot's token
+
 ```
 
 <h2>Links</h2>
 
 * [PyPi](https://pypi.org/project/boticordpy)
 * [Documentation](https://py.boticord.top)
 * [Github](https://github.com/boticord/boticordpy)
 * [BotiCord](https://boticord.top/)
 * [Support](https://boticord.top/discord)
 
 <h2>Help</h2>
 
 If You need any help we recommend you to check the documentation. You can find us [here](https://bcord.cc/support). Main developer is **[Marakarka](https://boticord.top/profile/585766846268047370)**
-
-
```

#### html2text {}

```diff
@@ -1,34 +1,39 @@
-Metadata-Version: 2.1 Name: boticordpy Version: 2.2.2 Summary: A Python wrapper
+Metadata-Version: 2.1 Name: boticordpy Version: 3.0.0 Summary: A Python wrapper
 for BotiCord API Home-page: https://github.com/boticord/boticordpy Author:
 Marakarka Author-email: support@kerdoku.top License: MIT Project-URL:
 Documentation, https://py.boticord.top/en/stable Project-URL: Issue tracker,
-https://github.com/boticord/boticordpy/issues Platform: UNKNOWN Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.7 Requires-Python:
->= 3.6 Description-Content-Type: text/markdown License-File: LICENSE.txt
+https://github.com/boticord/boticordpy/issues Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >= 3.8 Description-Content-Type: text/markdown License-File:
+LICENSE.txt
            The easiest way to use BotiCord API in Python.  Â·  Docs
 
 ***** Features *****
 * Object-oriented * Full BotiCord API Coverage * Modern Pythonic API using
-`async`/`await` syntax * BotiCord Webhooks * It is not necessary to use any
+`async`/`await` syntax * BotiCord Websocket * It is not necessary to use any
 particular library used to interact with the Discord API.
 ***** Installation *****
-Python 3.6 or newer is required. Enter one of these commands to install the
+Python 3.8 or newer is required. Enter one of these commands to install the
 library: ``` pip install boticordpy ``` ``` python3 -m pip install boticordpy
 ``` Or just clone the repo: https://github.com/boticord/boticordpy
 ***** Examples *****
 You can find other examples in an examples folder. **Discord.py Autopost
 example** ```py from discord.ext import commands from boticordpy import
-BoticordClient bot = commands.Bot(command_prefix="!") async def get_stats():
-return {"servers": len(bot.guilds), "shards": 0, "users": len(bot.users)} async
-def on_success_posting(): print("stats posting successfully") boticord_client =
-BoticordClient("your_api_token") autopost = ( boticord_client.autopost()
-.init_stats(get_stats) .on_success(on_success_posting) .start() ) bot.run("bot
-token") ```
+BoticordClient bot = commands.Bot(command_prefix="!") # Function that will
+return the current bot's stats. async def get_stats(): return {"servers": len
+(bot.guilds), "shards": 0, "users": len(bot.users)} # Function that will be
+called if stats are posted successfully. async def on_success_posting(): print
+("wow stats posting works") boticord_client = BoticordClient
+( "your_boticord_api_token", version=3 ) # <--- BotiCord API token autopost =
+( boticord_client.autopost() .init_stats(get_stats) .on_success
+(on_success_posting) .start("id_of_your_bot") # <--- ID of your bot ) bot.run
+("bot token") # <--- Discord bot's token ```
 ***** Links *****
 * [PyPi](https://pypi.org/project/boticordpy) * [Documentation](https://
 py.boticord.top) * [Github](https://github.com/boticord/boticordpy) *
 [BotiCord](https://boticord.top/) * [Support](https://boticord.top/discord)
 ***** Help *****
 If You need any help we recommend you to check the documentation. You can find
 us [here](https://bcord.cc/support). Main developer is **[Marakarka](https://
```

### Comparing `boticordpy-2.2.2/setup.py` & `boticordpy-3.0.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -40,22 +40,25 @@
     name="boticordpy",
     project_urls={
         "Documentation": "https://py.boticord.top/en/stable",
         "Issue tracker": "https://github.com/boticord/boticordpy/issues",
     },
     packages=find_packages(),
     version=version,
-    python_requires=">= 3.6",
+    python_requires=">= 3.8",
     description="A Python wrapper for BotiCord API",
     long_description=README,
     long_description_content_type="text/markdown",
+    include_package_data=True,
     url="https://github.com/boticord/boticordpy",
     author="Marakarka",
     author_email="support@kerdoku.top",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
-    install_requires=["aiohttp"],
+    install_requires=["aiohttp", "typing_extensions"],
 )
```

