# Comparing `tmp/irc_api-0.0.3.tar.gz` & `tmp/irc_api-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irc_api-0.0.3.tar", last modified: Fri Jun 30 08:20:11 2023, max compression
+gzip compressed data, was "irc_api-0.0.4.tar", last modified: Sat Jul  1 15:58:05 2023, max compression
```

## Comparing `irc_api-0.0.3.tar` & `irc_api-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:20:11.479369 irc_api-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-30 08:19:58.000000 irc_api-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-30 08:20:11.479369 irc_api-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-30 08:19:58.000000 irc_api-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-30 08:19:58.000000 irc_api-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 08:20:11.479369 irc_api-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:20:11.479369 irc_api-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:20:11.479369 irc_api-0.0.3/src/irc_api/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-30 08:19:58.000000 irc_api-0.0.3/src/irc_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10169 2023-06-30 08:19:58.000000 irc_api-0.0.3/src/irc_api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-06-30 08:19:58.000000 irc_api-0.0.3/src/irc_api/irc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:20:11.479369 irc_api-0.0.3/src/irc_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-30 08:20:11.000000 irc_api-0.0.3/src/irc_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-30 08:20:11.000000 irc_api-0.0.3/src/irc_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 08:20:11.000000 irc_api-0.0.3/src/irc_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 08:20:11.000000 irc_api-0.0.3/src/irc_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:58:05.456746 irc_api-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 15:57:55.000000 irc_api-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-01 15:58:05.456746 irc_api-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-01 15:57:55.000000 irc_api-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-01 15:57:55.000000 irc_api-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 15:58:05.456746 irc_api-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:58:05.452746 irc_api-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:58:05.452746 irc_api-0.0.4/src/irc_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-01 15:57:55.000000 irc_api-0.0.4/src/irc_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-07-01 15:57:55.000000 irc_api-0.0.4/src/irc_api/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11279 2023-07-01 15:57:55.000000 irc_api-0.0.4/src/irc_api/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-01 15:57:55.000000 irc_api-0.0.4/src/irc_api/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-01 15:57:55.000000 irc_api-0.0.4/src/irc_api/irc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-01 15:57:55.000000 irc_api-0.0.4/src/irc_api/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:58:05.456746 irc_api-0.0.4/src/irc_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-01 15:58:05.000000 irc_api-0.0.4/src/irc_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-01 15:58:05.000000 irc_api-0.0.4/src/irc_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 15:58:05.000000 irc_api-0.0.4/src/irc_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-01 15:58:05.000000 irc_api-0.0.4/src/irc_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-01 15:58:05.000000 irc_api-0.0.4/src/irc_api.egg-info/top_level.txt
```

### Comparing `irc_api-0.0.3/LICENSE` & `irc_api-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `irc_api-0.0.3/PKG-INFO` & `irc_api-0.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: irc_api
-Version: 0.0.3
+Version: 0.0.4
 Summary: An API written in Python to make IRC bots.
-Author: Antoine Royer
+Author: Sha-chan
 Project-URL: Homepage, https://github.com/Shadow15510/irc_api
+Project-URL: Documentation, https://irc-api.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: doc
 License-File: LICENSE
 
 # IRC API
 
 ## Licence
 The code is provided under GNU General Public Licence version 3 or later (GPLv3+).
```

### Comparing `irc_api-0.0.3/pyproject.toml` & `irc_api-0.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,40 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "irc_api"
 authors = [
-	{name="Antoine Royer"},
+	{name="Sha-chan"},
 ]
 description = "An API written in Python to make IRC bots."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 	"Development Status :: 5 - Production/Stable",
 ]
+
 dynamic = [
 	"version",
 ]
 
+[tool.setuptools]
+license-files = [
+    "LICENSE",
+]
+
+[project.optional-dependencies]
+doc = [
+    "sphinx>=7.0.1",
+    "sphinx-rtd-theme",
+    "sphinx-autodocgen",
+]
+
 [tool.setuptools.dynamic.version]
 attr = "irc_api.__init__.__version__"
 
 [project.urls]
-"Homepage" = "https://github.com/Shadow15510/irc_api"
+Homepage = "https://github.com/Shadow15510/irc_api"
+Documentation = "https://irc-api.readthedocs.io/en/latest/"
```

### Comparing `irc_api-0.0.3/src/irc_api/api.py` & `irc_api-0.0.4/src/irc_api/bot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,200 +1,148 @@
+"""Provide a Bot class that react to IRC's message and events."""
+
 import logging
-import re
-from irc_api.irc import IRC, History
 from threading import Thread
 import time
+import re
 
-
-PREFIX = ""
-
-
-def command(name, alias=(), desc=""):
-    if not alias or not name in alias:
-        alias += (name,)
-    def decorator(func):
-        return Command(
-                name=name,
-                func=func,
-                events=[lambda m: True in [m.text == PREFIX + cmd or m.text.startswith(PREFIX + cmd + " ") for cmd in alias]],
-                desc=desc,
-                cmnd_type=1
-            )
-    return decorator
-
-
-def on(event, desc=""):
-    def decorator(func_or_cmnd):
-        if isinstance(func_or_cmnd, Command):
-            func_or_cmnd.events.append(event)
-            return func_or_cmnd
-        else:
-            return Command(
-                    name=func_or_cmnd.__name__,
-                    func=func_or_cmnd,
-                    events=[event],
-                    desc=desc,
-                    cmnd_type=0
-                )
-    return decorator
-
-
-def channel(channel_name, desc=""):
-    def decorator(func_or_cmnd):
-        if isinstance(func_or_cmnd, Command):
-            func_or_cmnd.events.append(lambda m: m.to == channel_name)
-            return func_or_cmnd
-        else:
-            return Command(
-                name=func_or_cmnd.__name__,
-                func=func_or_cmnd,
-                events=[lambda m: m.to == channel_name],
-                desc=desc,
-                cmnd_type=0
-            )
-    return decorator
-
-
-def user(user_name, desc=""):
-    def decorator(func_or_cmnd):
-        if isinstance(func_or_cmnd, Command):
-            func_or_cmnd.events.append(lambda m: m.author == user_name)
-            return func_or_cmnd
-        else:
-            return Command(
-                name=func_or_cmnd.__name__,
-                func=func_or_cmnd,
-                events=[lambda m: m.author == user_name],
-                desc=desc,
-                cmnd_type=0
-            )
-    return decorator
-
-
-def every(time, desc=""):
-    def decorator(func):
-        return Command(
-                name=func.__name__,
-                func=func,
-                events=time,
-                desc=desc,
-                cmnd_type=2
-            )
-
-    return decorator
-
-
-class Command:
-    def __init__(self, name, func, events, desc, cmnd_type):
-        self.name = name
-        self.func = func
-        self.events = events
-        self.cmnd_type = cmnd_type
-
-        if desc:
-            self.desc = desc
-        else:
-            self.desc = "..."
-            if func.__doc__:
-                self.desc = func.__doc__
-
-        self.bot = None
-
-    def __call__(self, msg, *args):
-        return self.func(self.bot, msg, *args)
-
-
-class WrongArg:
-    """If the transtyping has failed and the argument has no default value."""
+from irc_api.commands import BotCommand, PREFIX
+from irc_api.irc import IRC
+from irc_api.history import History
 
 
 class Bot:
     """Run the connexion between IRC's server and V5 one.
 
     Attributes
     ----------
+    prefix : str, public
+        The bot's prefix for named command.
     irc : IRC, public
         IRC wrapper which handle communication with IRC server.
-    v5 : V5, public
-        V5 wrapper which handle communication with V5 server.
+    history : History, public
+        The messages history. 
     channels : list, public
         The channels the bot will listen.
+    auth : tuple, public
+        This contains the username and the password for a SASL auth.
+    callbacks : dict, public
+        The callbacks of the bot. This dictionnary is like {name: command} where name is the name of
+        the command and command a BotCommand's instance.
+    commands_help : dict, public
+        Same that ``callbacks`` but only with the documented commands. 
+    threads : list, public
+        A list of threads for the commands with ``@api.every``.
 
     Methods
     -------
     start : NoneType, public
-        Runs the bot and connects it to IRC and V5 servers.
+        Runs the bot and connects it to IRC server.
+    send : NoneType, public
+        Send a message on the IRC server.
+    add_command : NoneType, public
+        Add a single command to the bot.
+    add_commands : NoneType, public
+        Allow to add a list of command to the bot.
+    add_commands_module : NoneType, public
+        Allow to add a module of command to the bot.
+    remove_command : NoneType, public
+        Remove a command.
     """
     def __init__(
             self,
-            auth: tuple,
             irc_params: tuple,
-            channels: list=["#general"],
             *commands_modules,
-            **kwargs
+            auth: tuple=(),
+            channels: list=["#general"],
+            prefix: str="",
+            limit: int=100,
         ):
         """Initialize the Bot instance.
 
         Parameters
         ----------
         irc_params : tuple
-            Contains the IRC server informations (host, port)
-        channels : list
+            A tuple like: (host, port) to connect to the IRC server.
+        auth : tuple, optionnal
+            Contains the IRC server informations (host, port).
+        channels : list, optionnal
             Contains the names of the channels on which the bot will connect.
-        prefix : str, optionnal
-            The prefix on which the bot will react.
+        prefix : str
+            The bot's prefix for named commands.
+        limit : int
+            The message history of the bot. By default, the bot will remind 100 messages.
+        *commands_module : optionnal
+            Modules of commands that you can give to the bot at it's creation.
+
+        Examples
+        --------
+        Assuming the module was imported as follow: ``from irc_api import api``
+        You can create a bot::
+
+            my_bot = api.Bot(
+                    irc_params=(irc.exemple.com, 6697),
+                    channels=["#general", "#bot-test"],
+                    prefix="!",
+                    cmnd_pack1, cmnd_pack2
+                )
         """
         global PREFIX
-        if kwargs.get('prefix'):
-            PREFIX = kwargs.get('prefix')
+        PREFIX = prefix
         self.prefix = PREFIX
 
         self.irc = IRC(*irc_params)
-        self.history = History(kwargs.get('limit'))
+        self.history = History(limit)
         self.channels = channels
         self.auth = auth
         self.callbacks = {}
         self.commands_help = {}
         self.threads = []
 
         if commands_modules:
             self.add_commands_modules(*commands_modules)
 
     def start(self, nick: str):
-        """Starts the bot and connect it to the given IRC and V5 servers."""
+        """Start the bot and connect it to IRC. Handle the messages and callbacks too.
+
+        Parameters
+        ----------
+        nick : str
+            The nickname of the bot.
+        """
         # Start IRC
-        self.irc.connexion(self.auth[0], self.auth[1], nick)
+        self.irc.connexion(nick, self.auth)
 
         # Join channels
         for channel in self.channels:
             self.irc.join(channel)
 
         # mainloop
         while True:
             message = self.irc.receive()
             self.history.add(message)
             logging.info("received %s", message)
             if message is not None:
                 for callback in self.callbacks.values():
                     if not False in [event(message) for event in callback.events]:
                         logging.info("matched %s", callback.name)
-                        
-                        # @api.on
+
+                        # others command types
                         if callback.cmnd_type == 0:
                             callback(message)
 
                         # @api.command
                         elif callback.cmnd_type == 1:
                             args = check_args(callback.func, *parse(message.text)[1:])
                             if isinstance(args, list):
                                 callback(message, *args)
                             else:
                                 self.send(
                                         message.to,
-                                        "Erreur : les arguments donnés ne correspondent pas."
+                                        "Error: arguments mismatch."
                                     )
 
     def send(self, target: str, message: str):
         """Send a message to the specified target (channel or user).
 
         Parameters
         ----------
@@ -202,124 +150,174 @@
             The target of the message. It can be a channel or user (private message).
         message : str
             The content of the message to send.
         """
         for line in message.splitlines():
             self.irc.send(f"PRIVMSG {target} :{line}")
 
-    def add_command(self, command, add_to_help=False):
+    def add_command(self, command, add_to_help: bool=False):
+        """Add a single command to the bot.
+
+        Parameters
+        ----------
+        command : BotCommand
+            The command to add to the bot.
+        add_to_help : bool, optionnal
+            If the command should be added to the documented functions.
+        """
         command.bot = self
 
         if command.cmnd_type == 2:
             def timed_func(bot):
                 while True:
                     command.func(bot)
                     time.sleep(command.events)
                     logging.info("auto call : %s", command.name)
 
-            self.threads.append(Thread(target=lambda bot: timed_func(bot), args=(self,)))
+            self.threads.append(Thread(target=timed_func, args=(self,)))
             self.threads[-1].start()
         else:
             self.callbacks[command.name] = command
 
-        if add_to_help and command.cmnd_type == 1:
+        if add_to_help:
             self.commands_help[command.name] = command
 
-    def add_commands(self, *commands, **kwargs):
+    def add_commands(self, *commands):
         """Add a list of commands to the bot.
 
         Parameters
         ----------
-        commands : list
-            A list of command's instances.
+        *commands
+            The commands' instances.
         """
         add_to_help = "auto_help" in [cmnd.name for cmnd in commands]
         for command in commands:
             self.add_command(command, add_to_help=add_to_help)
 
     def add_commands_modules(self, *commands_modules):
+        """Add a module of commands to the bot. You can give several modules.
+
+        Parameters
+        ----------
+        *commands
+            The commands modules to add to the bot.
+        """
         for commands_module in commands_modules:
             add_to_help = "auto_help" in dir(commands_module)
             for cmnd_name in dir(commands_module):
-                    cmnd = getattr(commands_module, cmnd_name)
-                    if isinstance(cmnd, Command):
-                        self.add_command(cmnd, add_to_help=add_to_help)
+                cmnd = getattr(commands_module, cmnd_name)
+                if isinstance(cmnd, BotCommand):
+                    self.add_command(cmnd, add_to_help=add_to_help)
 
     def remove_command(self, command_name: str):
-        if command_name in self.callbacks.keys():
-            self.callbacks.pop(command_name)
+        """Remove a command.
 
+        Parameters
+        ----------
+        command_name : str
+            The name of the command to delete.
+        """
+        if command_name in self.callbacks:
+            self.callbacks.pop(command_name)
+            self.commands_help.pop(command_name)
 
-@command("aide", alias=("aide", "help", "doc", "assistance"))
-def auto_help(bot, msg, fct_name: str=""):
-    """Aide des commandes disponibles."""
-    if fct_name and fct_name in bot.commands_help.keys():
-        cmnd = bot.commands_help[fct_name]
-        answer = f"Aide sur la commande : {bot.prefix}{fct_name}\n"
-        for line in bot.commands_help[fct_name].desc.splitlines():
-            answer += f" │ {line}\n"
-    else:
-        answer = f"Liste des commandes ({PREFIX}aide <cmnd> pour plus d'info)\n"
-        for cmnd_name in bot.commands_help.keys():
-            answer += f" - {cmnd_name}\n"
 
-    bot.send(msg.to, answer)
+class WrongArg:
+    """If the transtyping has failed and the argument has no default value."""
 
 
 def parse(message):
+    """Parse the given message to detect the command and the arguments. If a command's name is
+    'cmnd' and the bot receive the message ``cmnd arg1 arg2`` this function will returns
+    ``[arg1, arg2]``. It allows to have a powerfull commands with custom arguments.
+
+    Parameters
+    ----------
+    message : irc_api.irc.Message
+        The message to parse.
+
+    Returns
+    -------
+    args_to_return : list
+        The list of the given arguments in the message.
+    """
     pattern = re.compile(r"((\"[^\"]+\"\ *)|(\'[^\']+\'\ *)|([^\ ]+\ *))", re.IGNORECASE)
     args_to_return = []
     for match in re.findall(pattern, message):
         match = match[0].strip().rstrip()
         if (match.startswith("\"") and match.endswith("\"")) \
                 or (match.startswith("'") and match.endswith("'")):
             args_to_return.append(match[1: -1])
         else:
             args_to_return.append(match)
     return args_to_return
 
 
-def convert(data, new_type, default=None):
+def convert(data, new_type: type, default=None):
+    """Transtype a given variable into a given type. Returns a default value in case of failure.
+
+    Parameters
+    ----------
+    data
+        The given data to transtype.
+    new_type : type
+
+
+    """
     try:
         return new_type(data)
-    except:
+    except ValueError:
         return default
 
 
 def check_args(func, *input_args):
+    """Check if the given args fit to the function in terms of number and type.
+
+    Parameters
+    ----------
+    func : function
+        The function the user wants to run.
+    *input_args
+        The arguments given by the user.
+
+    Returns
+    -------
+    converted_args : list
+        The list of the arguments with the right type. The surplus arguments are ignored.
+    """
     # gets the defaults values given in arguments
     defaults = getattr(func, "__defaults__")
     if not defaults:
         defaults = []
 
     # gets the arguments and their types
     annotations = getattr(func, "__annotations__")
     if not annotations:
         return []
 
-    # nb of required arguments
+    # number of required arguments
     required_args = len(annotations) - len(defaults)
 
     # if the number of given arguments just can't match
     if len(input_args) < required_args:
         return None
 
     wrong_arg = WrongArg()
     converted_args = []
     for index, arg_type in enumerate(annotations.values()):
         # construction of a tuple (type, default_value) for each expected argument
         if index + 1 > required_args:
-            check_args = (arg_type, defaults[index - required_args])
+            checked_args = (arg_type, defaults[index - required_args])
         else:
-            check_args = (arg_type, wrong_arg)
+            checked_args = (arg_type, wrong_arg)
 
         # transtypes each given arguments to its target type
         if len(input_args) > index:
-            converted_args.append(convert(input_args[index], *check_args))
+            converted_args.append(convert(input_args[index], *checked_args))
         else:
-            converted_args.append(check_args[1])
+            converted_args.append(checked_args[1])
 
     # if an argument has no default value and transtyping has failed
     if wrong_arg in converted_args:
         return None
 
     return converted_args
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `irc_api-0.0.3/src/irc_api/irc.py` & `irc_api-0.0.4/src/irc_api/irc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,49 @@
-"""
-irc (IRC API)
-=============
-
-Description
------------
-Manage the IRC layer.
-"""
+"""Manage the IRC layer."""
 
 import logging
-import re
 import socket
 import ssl
 
-from functools import wraps
 from queue import Queue
 from threading import Thread
 
+from irc_api.message import Message
+
 
 class IRC:
     """Manage connexion to an IRC server, authentication and callbacks.
 
     Attributes
     ----------
     connected : bool, public
         If the bot is connected to an IRC server or not.
-    callbacks : list, public
-        List of the registred callbacks.
 
     socket : ssl.SSLSocket, private
         The IRC's socket.
     inbox : Queue, private
         Queue of the incomming messages.
     handler : Thread, private
 
     Methods
     -------
-    start : NoneType, public
+    connexion : NoneType, public
         Starts the IRC layer and manage authentication.
-    run : NoneType, public
-        Mainloop, allows to handle public messages.
     send : NoneType, public
         Sends a message to a given channel.
     receive : Message, public
-        Same as ``run`` for private messages.
+        Receive a new raw message and return the processed message. 
     join : NoneType, public
         Allows to join a given channel.
-    on : function, public
-        Add a callback on a given message.
+    waitfor : str, public
+        Wait for a raw message that matches the given condition.
 
     handle : NoneType, private
         Handles the ping and store incoming messages into the inbox attribute.
-    send : NoneType, private
-        Send message to a target.
-    recv : str, private
-        Get the oldest incoming message and returns it.
-    waitfor : str, private
-        Wait for a raw message that matches the given condition.
+    
     """
     def __init__(self, host: str, port: int):
         """Initialize an IRC wrapper.
 
         Parameters
         ----------
         host : str
@@ -76,34 +60,47 @@
                 socket.create_connection((host, port)),
                 server_hostname=host
             )
         self.__inbox = Queue()
         self.__handler = Thread(target=self.__handle)
 
     # Public methods
-    def connexion(self, username: str, password: str, nick: str):
+    def connexion(self, nick: str, auth: tuple=()):
         """Start the IRC layer. Manage authentication as well.
 
         Parameters
         ----------
         nick : str
-            The username for login and nickname once connected.
-        password : str
-            The password for authentification.
+            The nickname used.
+        auth : tuple, optionnal
+            The tuple (username, password) for a SASL authentication. Leave empty if no SASL auth is
+            required.
         """
         self.__handler.start()
 
         self.send(f"USER {nick} * * :{nick}")
         self.send(f"NICK {nick}")
-        self.waitfor(lambda m: "NOTICE" in m and "/AUTH" in m)
-        self.send(f"AUTH {username}:{password}")
+        if auth:
+            self.waitfor(lambda m: "NOTICE" in m and "/AUTH" in m)
+            self.send(f"AUTH {auth[0]}:{auth[1]}")
+
         self.waitfor(lambda m: "You are now logged in" in m)
 
         self.connected = True
 
+    def send(self, raw: str):
+        """Wrap and encode raw message to send.
+
+        Parameters
+        ----------
+        raw : str
+            The raw message to send.
+        """
+        self.__socket.send(f"{raw}\r\n".encode())
+
     def receive(self):
         """Receive a private message.
         
         Returns
         -------
         msg : Message
             The incoming processed private message.
@@ -122,24 +119,14 @@
         ----------
         channel : str
             The name of the channel to join.
         """
         self.send(f"JOIN {channel}")
         logging.info("joined %s", channel)
 
-    def send(self, raw: str):
-        """Wrap and encode raw message to send.
-
-        Parameters
-        ----------
-        raw : str
-            The raw message to send.
-        """
-        self.__socket.send(f"{raw}\r\n".encode())
-
     def waitfor(self, condition):
         """Wait for a raw message that matches the condition.
 
         Parameters
         ----------
         condition : function
             ``condition`` is a function that must taking a raw message in parameter and returns a
@@ -163,67 +150,12 @@
             data = self.__socket.recv(4096).decode()
 
             # Split multiple lines
             for msg in data.split('\r\n'):
                 # Manage ping
                 if msg.startswith("PING"):
                     self.send(msg.replace("PING", "PONG"))
-                
+
                 # Or add a new message to inbox
                 elif len(msg):
                     self.__inbox.put(msg)
                     logging.debug("received %s", msg)
-
-
-class History:
-    def __init__(self, limit: int):
-        self.__content = []
-        if limit:
-            self.__limit = limit
-        else:
-            self.__limit = 100
-
-    def __len__(self):
-        return len(self.__content)
-
-    def add(self, elmnt):
-        if len(self.__content) == self.__limit:
-            self.__content.pop(0)
-        self.__content.append(elmnt)
-
-    def get(self):
-        return self.__content
-
-
-class Message:
-    """Parse the raw message in three fields : author, the channel, and text.
-    
-    Attributes
-    ----------
-    pattern : re.Pattern, public
-        The message parsing pattern.
-    author : str, public
-        The message's author.
-    to : str, public
-        The message's origin (channel or DM).
-    text : str, public
-        The message's content.
-    """
-    pattern = re.compile(
-            r"^:(?P<author>[\w.~|\-\[\]]+)(?:!(?P<host>\S+))? PRIVMSG (?P<to>\S+) :(?P<text>.+)"
-        )
-
-    def __init__(self, raw: str):
-        match = re.search(Message.pattern, raw)
-        if match:
-            self.author = match.group("author")
-            self.to = match.group("to")
-            self.text = match.group("text")
-            logging.debug("sucessfully parsed %s into %s", raw, self.__str__())
-        else:
-            self.author = ""
-            self.to = ""
-            self.text = ""
-            logging.warning("failed to parse %s into valid message", raw)
-
-    def __str__(self):
-        return f"{self.author} to {self.to}: {self.text}"
```

### Comparing `irc_api-0.0.3/src/irc_api.egg-info/PKG-INFO` & `irc_api-0.0.4/src/irc_api.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: irc-api
-Version: 0.0.3
+Version: 0.0.4
 Summary: An API written in Python to make IRC bots.
-Author: Antoine Royer
+Author: Sha-chan
 Project-URL: Homepage, https://github.com/Shadow15510/irc_api
+Project-URL: Documentation, https://irc-api.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: doc
 License-File: LICENSE
 
 # IRC API
 
 ## Licence
 The code is provided under GNU General Public Licence version 3 or later (GPLv3+).
```

