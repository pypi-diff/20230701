# Comparing `tmp/irc_api-0.0.8.tar.gz` & `tmp/irc_api-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irc_api-0.0.8.tar", last modified: Sat Jul  1 20:07:34 2023, max compression
+gzip compressed data, was "irc_api-0.0.9.tar", last modified: Sat Jul  1 20:19:09 2023, max compression
```

## Comparing `irc_api-0.0.8.tar` & `irc_api-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:07:34.248079 irc_api-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 20:07:21.000000 irc_api-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-01 20:07:34.248079 irc_api-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-01 20:07:21.000000 irc_api-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-01 20:07:21.000000 irc_api-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 20:07:34.248079 irc_api-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:07:34.244079 irc_api-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:07:34.248079 irc_api-0.0.8/src/irc_api/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-01 20:07:21.000000 irc_api-0.0.8/src/irc_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-07-01 20:07:21.000000 irc_api-0.0.8/src/irc_api/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-07-01 20:07:21.000000 irc_api-0.0.8/src/irc_api/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-01 20:07:21.000000 irc_api-0.0.8/src/irc_api/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-01 20:07:21.000000 irc_api-0.0.8/src/irc_api/irc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-01 20:07:21.000000 irc_api-0.0.8/src/irc_api/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:07:34.248079 irc_api-0.0.8/src/irc_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-01 20:07:34.000000 irc_api-0.0.8/src/irc_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-01 20:07:34.000000 irc_api-0.0.8/src/irc_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 20:07:34.000000 irc_api-0.0.8/src/irc_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-01 20:07:34.000000 irc_api-0.0.8/src/irc_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-01 20:07:34.000000 irc_api-0.0.8/src/irc_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:19:09.750967 irc_api-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 20:18:56.000000 irc_api-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-01 20:19:09.746967 irc_api-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-01 20:18:56.000000 irc_api-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-01 20:18:56.000000 irc_api-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 20:19:09.750967 irc_api-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:19:09.742967 irc_api-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:19:09.746967 irc_api-0.0.9/src/irc_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-01 20:18:56.000000 irc_api-0.0.9/src/irc_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-07-01 20:18:56.000000 irc_api-0.0.9/src/irc_api/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-07-01 20:18:56.000000 irc_api-0.0.9/src/irc_api/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-01 20:18:56.000000 irc_api-0.0.9/src/irc_api/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-01 20:18:56.000000 irc_api-0.0.9/src/irc_api/irc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-01 20:18:56.000000 irc_api-0.0.9/src/irc_api/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:19:09.746967 irc_api-0.0.9/src/irc_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-01 20:19:09.000000 irc_api-0.0.9/src/irc_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-01 20:19:09.000000 irc_api-0.0.9/src/irc_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 20:19:09.000000 irc_api-0.0.9/src/irc_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-01 20:19:09.000000 irc_api-0.0.9/src/irc_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-01 20:19:09.000000 irc_api-0.0.9/src/irc_api.egg-info/top_level.txt
```

### Comparing `irc_api-0.0.8/LICENSE` & `irc_api-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `irc_api-0.0.8/PKG-INFO` & `irc_api-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irc_api
-Version: 0.0.8
+Version: 0.0.9
 Summary: An API written in Python to make IRC bots.
 Author: Sha-chan
 Project-URL: Homepage, https://github.com/Shadow15510/irc_api
 Project-URL: Documentation, https://irc-api.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `irc_api-0.0.8/pyproject.toml` & `irc_api-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `irc_api-0.0.8/src/irc_api/bot.py` & `irc_api-0.0.9/src/irc_api/bot.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -47,19 +47,19 @@
         Allow to add a module of command to the bot.
     remove_command : NoneType, public
         Remove a command.
     """
     def __init__(
             self,
             irc_params: tuple,
+            *commands_modules
             auth: tuple=(),
             channels: list=["#general"],
             prefix: str="",
             limit: int=100,
-            *commands_modules
         ):
         """Initialize the Bot instance.
 
         Parameters
         ----------
         irc_params : tuple
             A tuple like: (host, port) to connect to the IRC server.
```

### Comparing `irc_api-0.0.8/src/irc_api/commands.py` & `irc_api-0.0.9/src/irc_api/commands.py`

 * *Files identical despite different names*

### Comparing `irc_api-0.0.8/src/irc_api/history.py` & `irc_api-0.0.9/src/irc_api/history.py`

 * *Files identical despite different names*

### Comparing `irc_api-0.0.8/src/irc_api/irc.py` & `irc_api-0.0.9/src/irc_api/irc.py`

 * *Files identical despite different names*

### Comparing `irc_api-0.0.8/src/irc_api/message.py` & `irc_api-0.0.9/src/irc_api/message.py`

 * *Files identical despite different names*

### Comparing `irc_api-0.0.8/src/irc_api.egg-info/PKG-INFO` & `irc_api-0.0.9/src/irc_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irc-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: An API written in Python to make IRC bots.
 Author: Sha-chan
 Project-URL: Homepage, https://github.com/Shadow15510/irc_api
 Project-URL: Documentation, https://irc-api.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 5 - Production/Stable
```

