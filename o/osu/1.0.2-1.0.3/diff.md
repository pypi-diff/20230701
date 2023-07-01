# Comparing `tmp/osu-1.0.2.tar.gz` & `tmp/osu-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osu-1.0.2.tar", last modified: Sat Jul  1 18:21:53 2023, max compression
+gzip compressed data, was "osu-1.0.3.tar", last modified: Sat Jul  1 19:11:00 2023, max compression
```

## Comparing `osu-1.0.2.tar` & `osu-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:21:53.279688 osu-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 18:21:38.000000 osu-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-01 18:21:53.279688 osu-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-01 18:21:38.000000 osu-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:21:53.279688 osu-1.0.2/osu/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-01 18:21:38.000000 osu-1.0.2/osu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-01 18:21:38.000000 osu-1.0.2/osu/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-07-01 18:21:38.000000 osu-1.0.2/osu/game.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:21:53.279688 osu-1.0.2/osu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-01 18:21:53.000000 osu-1.0.2/osu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-01 18:21:53.000000 osu-1.0.2/osu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 18:21:53.000000 osu-1.0.2/osu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-01 18:21:53.000000 osu-1.0.2/osu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-01 18:21:53.000000 osu-1.0.2/osu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 18:21:53.279688 osu-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-01 18:21:38.000000 osu-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:11:00.120826 osu-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 19:10:43.000000 osu-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-01 19:11:00.120826 osu-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-01 19:10:43.000000 osu-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:11:00.116826 osu-1.0.3/osu/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-01 19:10:43.000000 osu-1.0.3/osu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-01 19:10:43.000000 osu-1.0.3/osu/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-07-01 19:10:43.000000 osu-1.0.3/osu/game.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:11:00.120826 osu-1.0.3/osu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-01 19:11:00.000000 osu-1.0.3/osu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-01 19:11:00.000000 osu-1.0.3/osu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 19:11:00.000000 osu-1.0.3/osu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-01 19:11:00.000000 osu-1.0.3/osu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-01 19:11:00.000000 osu-1.0.3/osu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 19:11:00.120826 osu-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-01 19:10:43.000000 osu-1.0.3/setup.py
```

### Comparing `osu-1.0.2/LICENSE` & `osu-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `osu-1.0.2/README.md` & `osu-1.0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -4,22 +4,34 @@
 
 osu.py is a python library that emulates part of the online functionality of the osu! stable client.
 This is still a work in progress, but I decided to release it anyways.
 
 **IMPORTANT:**
 Use this library at your own risk! I am not responsible for anything that can happen to your account. If you want to test it out on a private server, you can set the `server` attribute when initializing the client.
 
+You can install this package with pip:
+```shell
+pip install osu
+```
+
+Or build it manually:
+```shell
+git clone https://github.com/Lekuruu/osu.py.git
+cd osu.py
+python setup.py install
+```
+
 ## Features
 
 - [x] Receiving player stats
 - [x] Sending/Receiving chat messages
 - [x] Up to 12 clients (Tournament Client)
 - [x] Spectating other players
 - [ ] Documentation
-- [ ] Multiplayer?
+- [ ] Multiplayer
 
 ## Example
 
 ```python
 from osu.constants import ServerPackets
 from osu import Game
```

### Comparing `osu-1.0.2/osu/events.py` & `osu-1.0.3/osu/events.py`

 * *Files identical despite different names*

### Comparing `osu-1.0.2/osu/game.py` & `osu-1.0.3/osu/game.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,19 +163,22 @@
                 "Please check your release stream or provide a custom version!"
             )
             return None
 
         # Parse url (e.g.: https://osu.ppy.sh/home/changelog/stable40/20230326)
         version = response.url.removesuffix("/").split("/")[-1]
 
-        if not version.isdigit():
+        if not version.replace(".", "").isdigit():
             self.logger.error(
                 f'Failed to get client version ("{version}" is not an integer).'
             )
             self.logger.error("Please provide a custom version!")
             return None
 
         self.logger.debug(f"Version: b{version}{'tourney' if self.tourney else ''}")
 
-        self.version_number = int(version)
+        try:
+            self.version_number = int(version)
+        except ValueError:
+            self.version_number = float(version)
 
         return f"b{version}{'tourney' if self.tourney else ''}"
```

