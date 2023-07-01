# Comparing `tmp/irc_api-0.0.7.tar.gz` & `tmp/irc_api-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irc_api-0.0.7.tar", last modified: Sat Jul  1 20:02:55 2023, max compression
+gzip compressed data, was "irc_api-0.0.8.tar", last modified: Sat Jul  1 20:07:34 2023, max compression
```

## Comparing `irc_api-0.0.7.tar` & `irc_api-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:02:55.955528 irc_api-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 20:02:46.000000 irc_api-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-01 20:02:55.955528 irc_api-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-01 20:02:46.000000 irc_api-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-01 20:02:46.000000 irc_api-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 20:02:55.955528 irc_api-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:02:55.955528 irc_api-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:02:55.955528 irc_api-0.0.7/src/irc_api/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-01 20:02:46.000000 irc_api-0.0.7/src/irc_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-07-01 20:02:46.000000 irc_api-0.0.7/src/irc_api/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-07-01 20:02:46.000000 irc_api-0.0.7/src/irc_api/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-01 20:02:46.000000 irc_api-0.0.7/src/irc_api/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-01 20:02:46.000000 irc_api-0.0.7/src/irc_api/irc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-01 20:02:46.000000 irc_api-0.0.7/src/irc_api/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:02:55.955528 irc_api-0.0.7/src/irc_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-01 20:02:55.000000 irc_api-0.0.7/src/irc_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-01 20:02:55.000000 irc_api-0.0.7/src/irc_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 20:02:55.000000 irc_api-0.0.7/src/irc_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-01 20:02:55.000000 irc_api-0.0.7/src/irc_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-01 20:02:55.000000 irc_api-0.0.7/src/irc_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:07:34.248079 irc_api-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 20:07:21.000000 irc_api-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-01 20:07:34.248079 irc_api-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-01 20:07:21.000000 irc_api-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-01 20:07:21.000000 irc_api-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 20:07:34.248079 irc_api-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:07:34.244079 irc_api-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:07:34.248079 irc_api-0.0.8/src/irc_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-01 20:07:21.000000 irc_api-0.0.8/src/irc_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-07-01 20:07:21.000000 irc_api-0.0.8/src/irc_api/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-07-01 20:07:21.000000 irc_api-0.0.8/src/irc_api/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-01 20:07:21.000000 irc_api-0.0.8/src/irc_api/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-01 20:07:21.000000 irc_api-0.0.8/src/irc_api/irc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-01 20:07:21.000000 irc_api-0.0.8/src/irc_api/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:07:34.248079 irc_api-0.0.8/src/irc_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-01 20:07:34.000000 irc_api-0.0.8/src/irc_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-01 20:07:34.000000 irc_api-0.0.8/src/irc_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 20:07:34.000000 irc_api-0.0.8/src/irc_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-01 20:07:34.000000 irc_api-0.0.8/src/irc_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-01 20:07:34.000000 irc_api-0.0.8/src/irc_api.egg-info/top_level.txt
```

### Comparing `irc_api-0.0.7/LICENSE` & `irc_api-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `irc_api-0.0.7/PKG-INFO` & `irc_api-0.0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irc_api
-Version: 0.0.7
+Version: 0.0.8
 Summary: An API written in Python to make IRC bots.
 Author: Sha-chan
 Project-URL: Homepage, https://github.com/Shadow15510/irc_api
 Project-URL: Documentation, https://irc-api.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `irc_api-0.0.7/pyproject.toml` & `irc_api-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `irc_api-0.0.7/src/irc_api/bot.py` & `irc_api-0.0.8/src/irc_api/bot.py`

 * *Files identical despite different names*

### Comparing `irc_api-0.0.7/src/irc_api/commands.py` & `irc_api-0.0.8/src/irc_api/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Defines the decorators for bot commands."""
-from irc_api.bot import PREFIX
+from irc_api.bot import BotCommand, PREFIX
 
 def command(name: str, alias: tuple=(), desc: str=""):
     """Create a new bot's command. Note that's a decorator.
     
     Parameters
     ----------
     name : str
```

### Comparing `irc_api-0.0.7/src/irc_api/history.py` & `irc_api-0.0.8/src/irc_api/history.py`

 * *Files identical despite different names*

### Comparing `irc_api-0.0.7/src/irc_api/irc.py` & `irc_api-0.0.8/src/irc_api/irc.py`

 * *Files identical despite different names*

### Comparing `irc_api-0.0.7/src/irc_api/message.py` & `irc_api-0.0.8/src/irc_api/message.py`

 * *Files identical despite different names*

### Comparing `irc_api-0.0.7/src/irc_api.egg-info/PKG-INFO` & `irc_api-0.0.8/src/irc_api.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irc-api
-Version: 0.0.7
+Version: 0.0.8
 Summary: An API written in Python to make IRC bots.
 Author: Sha-chan
 Project-URL: Homepage, https://github.com/Shadow15510/irc_api
 Project-URL: Documentation, https://irc-api.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 5 - Production/Stable
```

