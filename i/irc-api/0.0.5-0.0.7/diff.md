# Comparing `tmp/irc_api-0.0.5.tar.gz` & `tmp/irc_api-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irc_api-0.0.5.tar", last modified: Sat Jul  1 16:31:57 2023, max compression
+gzip compressed data, was "irc_api-0.0.7.tar", last modified: Sat Jul  1 20:02:55 2023, max compression
```

## Comparing `irc_api-0.0.5.tar` & `irc_api-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:31:57.844179 irc_api-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 16:31:42.000000 irc_api-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-01 16:31:57.844179 irc_api-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-01 16:31:42.000000 irc_api-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-01 16:31:42.000000 irc_api-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 16:31:57.844179 irc_api-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:31:57.844179 irc_api-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:31:57.844179 irc_api-0.0.5/src/irc_api/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-01 16:31:42.000000 irc_api-0.0.5/src/irc_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-07-01 16:31:42.000000 irc_api-0.0.5/src/irc_api/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    11279 2023-07-01 16:31:42.000000 irc_api-0.0.5/src/irc_api/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-01 16:31:42.000000 irc_api-0.0.5/src/irc_api/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-01 16:31:42.000000 irc_api-0.0.5/src/irc_api/irc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-01 16:31:42.000000 irc_api-0.0.5/src/irc_api/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:31:57.844179 irc_api-0.0.5/src/irc_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-01 16:31:57.000000 irc_api-0.0.5/src/irc_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-01 16:31:57.000000 irc_api-0.0.5/src/irc_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 16:31:57.000000 irc_api-0.0.5/src/irc_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-01 16:31:57.000000 irc_api-0.0.5/src/irc_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-01 16:31:57.000000 irc_api-0.0.5/src/irc_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:02:55.955528 irc_api-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 20:02:46.000000 irc_api-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-01 20:02:55.955528 irc_api-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-01 20:02:46.000000 irc_api-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-01 20:02:46.000000 irc_api-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 20:02:55.955528 irc_api-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:02:55.955528 irc_api-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:02:55.955528 irc_api-0.0.7/src/irc_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-01 20:02:46.000000 irc_api-0.0.7/src/irc_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-07-01 20:02:46.000000 irc_api-0.0.7/src/irc_api/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-07-01 20:02:46.000000 irc_api-0.0.7/src/irc_api/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-01 20:02:46.000000 irc_api-0.0.7/src/irc_api/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-01 20:02:46.000000 irc_api-0.0.7/src/irc_api/irc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-01 20:02:46.000000 irc_api-0.0.7/src/irc_api/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:02:55.955528 irc_api-0.0.7/src/irc_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-01 20:02:55.000000 irc_api-0.0.7/src/irc_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-01 20:02:55.000000 irc_api-0.0.7/src/irc_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 20:02:55.000000 irc_api-0.0.7/src/irc_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-01 20:02:55.000000 irc_api-0.0.7/src/irc_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-01 20:02:55.000000 irc_api-0.0.7/src/irc_api.egg-info/top_level.txt
```

### Comparing `irc_api-0.0.5/LICENSE` & `irc_api-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `irc_api-0.0.5/PKG-INFO` & `irc_api-0.0.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: irc_api
-Version: 0.0.5
+Version: 0.0.7
 Summary: An API written in Python to make IRC bots.
 Author: Sha-chan
 Project-URL: Homepage, https://github.com/Shadow15510/irc_api
 Project-URL: Documentation, https://irc-api.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 License-File: LICENSE
 
 # IRC API
+[![Documentation Status](https://readthedocs.org/projects/irc-api/badge/?version=latest)](https://irc-api.readthedocs.io/en/latest/?badge=latest)
 
 ## Licence
 The code is provided under GNU General Public Licence version 3 or later (GPLv3+).
 
 See LICENCE for more informations.
 
 ## Description
```

### Comparing `irc_api-0.0.5/pyproject.toml` & `irc_api-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `irc_api-0.0.5/src/irc_api/bot.py` & `irc_api-0.0.7/src/irc_api/bot.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Provide a Bot class that react to IRC's message and events."""
 
 import logging
 from threading import Thread
 import time
 import re
 
-from irc_api.commands import BotCommand, PREFIX
 from irc_api.irc import IRC
 from irc_api.history import History
 
+PREFIX = ""
 
 class Bot:
     """Run the connexion between IRC's server and V5 one.
 
     Attributes
     ----------
     prefix : str, public
@@ -47,19 +47,19 @@
         Allow to add a module of command to the bot.
     remove_command : NoneType, public
         Remove a command.
     """
     def __init__(
             self,
             irc_params: tuple,
-            *commands_modules,
             auth: tuple=(),
             channels: list=["#general"],
             prefix: str="",
             limit: int=100,
+            *commands_modules
         ):
         """Initialize the Bot instance.
 
         Parameters
         ----------
         irc_params : tuple
             A tuple like: (host, port) to connect to the IRC server.
@@ -217,14 +217,86 @@
             The name of the command to delete.
         """
         if command_name in self.callbacks:
             self.callbacks.pop(command_name)
             self.commands_help.pop(command_name)
 
 
+class BotCommand:
+    """Implement a bot command.
+
+    Attributes
+    ----------
+    name : str, public
+        The name of the command.
+    func : function, public
+        The function to execute when the BotCommand is called.
+    events : list, public
+        The list of the conditions on which the BotCommand will be called.
+    desc : str, public
+        The description of the BotCommand. By default, the function's docstring is used.
+    cmnd_type : int, public
+        The type of the command.
+        - if ``cmnd_type = 0``, the command is triggered on an event.
+        - if ``cmnd_type = 1``, the command is a named command.
+        - if ``cmnd_type = 2``, the command is a routine automatically triggered.
+    bot : irc_api.bot.Bot, public
+        The bot the command belongs to.
+    """
+    def __init__(self, name: str, func, events: list, desc: str, cmnd_type: int):
+        """Constructor method.
+
+        Parameters
+        ----------
+        name : str
+            The name of the command.
+        func : function
+            The function to execute when the BotCommand is called.
+        events : list
+            The list of the conditions on which the BotCommand will be called.
+        desc : str
+            The description of the BotCommand. By default, the function's docstring is used.
+        cmnd_type : int
+            The type of the command.
+            - if ``cmnd_type = 0``, the command is triggered on an event.
+            - if ``cmnd_type = 1``, the command is a named command.
+            - if ``cmnd_type = 2``, the command is a routine automatically triggered.
+        """
+        self.name = name
+        self.func = func
+        self.events = events
+        self.cmnd_type = cmnd_type
+
+        if desc:
+            self.desc = desc
+        else:
+            self.desc = "..."
+            if func.__doc__:
+                self.desc = func.__doc__
+
+        self.bot = None
+
+    def __call__(self, msg, *args):
+        """Call the function with the message that trigger the command and the given arguments.
+
+        Parameters
+        ----------
+        msg : irc_api.message.Message
+            The message that triggered the BotCommand.
+        *args
+            The arguments to give to the function.
+
+        Returns
+        -------
+        out
+            The output of ``BotCommand.func``.
+        """
+        return self.func(self.bot, msg, *args)
+
+
 class WrongArg:
     """If the transtyping has failed and the argument has no default value."""
 
 
 def parse(message):
     """Parse the given message to detect the command and the arguments. If a command's name is
     'cmnd' and the bot receive the message ``cmnd arg1 arg2`` this function will returns
```

### Comparing `irc_api-0.0.5/src/irc_api/history.py` & `irc_api-0.0.7/src/irc_api/history.py`

 * *Files identical despite different names*

### Comparing `irc_api-0.0.5/src/irc_api/irc.py` & `irc_api-0.0.7/src/irc_api/irc.py`

 * *Files identical despite different names*

### Comparing `irc_api-0.0.5/src/irc_api/message.py` & `irc_api-0.0.7/src/irc_api/message.py`

 * *Files identical despite different names*

