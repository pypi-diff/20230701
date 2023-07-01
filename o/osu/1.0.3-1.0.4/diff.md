# Comparing `tmp/osu-1.0.3.tar.gz` & `tmp/osu-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osu-1.0.3.tar", last modified: Sat Jul  1 19:11:00 2023, max compression
+gzip compressed data, was "osu-1.0.4.tar", last modified: Sat Jul  1 20:49:23 2023, max compression
```

## Comparing `osu-1.0.3.tar` & `osu-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:11:00.120826 osu-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 19:10:43.000000 osu-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-01 19:11:00.120826 osu-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-01 19:10:43.000000 osu-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:11:00.116826 osu-1.0.3/osu/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-01 19:10:43.000000 osu-1.0.3/osu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-01 19:10:43.000000 osu-1.0.3/osu/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-07-01 19:10:43.000000 osu-1.0.3/osu/game.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:11:00.120826 osu-1.0.3/osu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-01 19:11:00.000000 osu-1.0.3/osu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-01 19:11:00.000000 osu-1.0.3/osu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 19:11:00.000000 osu-1.0.3/osu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-01 19:11:00.000000 osu-1.0.3/osu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-01 19:11:00.000000 osu-1.0.3/osu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 19:11:00.120826 osu-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-01 19:10:43.000000 osu-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:49:23.933954 osu-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 20:49:09.000000 osu-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-01 20:49:23.933954 osu-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-01 20:49:09.000000 osu-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:49:23.925954 osu-1.0.4/osu/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-01 20:49:09.000000 osu-1.0.4/osu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:49:23.929954 osu-1.0.4/osu/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-01 20:49:09.000000 osu-1.0.4/osu/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-01 20:49:09.000000 osu-1.0.4/osu/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-01 20:49:09.000000 osu-1.0.4/osu/api/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:49:23.929954 osu-1.0.4/osu/bancho/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-01 20:49:09.000000 osu-1.0.4/osu/bancho/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-07-01 20:49:09.000000 osu-1.0.4/osu/bancho/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-07-01 20:49:09.000000 osu-1.0.4/osu/bancho/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15520 2023-07-01 20:49:09.000000 osu-1.0.4/osu/bancho/packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-07-01 20:49:09.000000 osu-1.0.4/osu/bancho/streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-01 20:49:09.000000 osu-1.0.4/osu/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-07-01 20:49:09.000000 osu-1.0.4/osu/game.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:49:23.933954 osu-1.0.4/osu/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-01 20:49:09.000000 osu-1.0.4/osu/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-01 20:49:09.000000 osu-1.0.4/osu/objects/beatmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-01 20:49:09.000000 osu-1.0.4/osu/objects/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-01 20:49:09.000000 osu-1.0.4/osu/objects/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-01 20:49:09.000000 osu-1.0.4/osu/objects/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-01 20:49:09.000000 osu-1.0.4/osu/objects/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-01 20:49:09.000000 osu-1.0.4/osu/objects/replays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-01 20:49:09.000000 osu-1.0.4/osu/objects/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:49:23.929954 osu-1.0.4/osu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-01 20:49:23.000000 osu-1.0.4/osu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-01 20:49:23.000000 osu-1.0.4/osu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 20:49:23.000000 osu-1.0.4/osu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-01 20:49:23.000000 osu-1.0.4/osu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-01 20:49:23.000000 osu-1.0.4/osu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 20:49:23.933954 osu-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-01 20:49:09.000000 osu-1.0.4/setup.py
```

### Comparing `osu-1.0.3/LICENSE` & `osu-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `osu-1.0.3/README.md` & `osu-1.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 - [x] Up to 12 clients (Tournament Client)
 - [x] Spectating other players
 - [ ] Documentation
 - [ ] Multiplayer
 
 ## Example
 
+Here is a small example of how to use this package:
+
 ```python
 from osu.constants import ServerPackets
 from osu import Game
 
 # Initialize the game class
 game = Game(
   USERNAME,
@@ -47,10 +49,12 @@
   if message.startswith('!ping'):
     sender.send_message('pong!')
 
 # Run the game
 game.run()
 ```
 
+[This project](https://github.com/Lekuruu/osu-recorder) is also a good example.
+
 ---
 
 If you have any questions, feel free to contact me on discord: `lekuru`
```

### Comparing `osu-1.0.3/osu/events.py` & `osu-1.0.4/osu/events.py`

 * *Files identical despite different names*

### Comparing `osu-1.0.3/osu/game.py` & `osu-1.0.4/osu/game.py`

 * *Files identical despite different names*

