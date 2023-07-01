# Comparing `tmp/play2048-4.0.tar.gz` & `tmp/play2048-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "play2048-4.0.tar", last modified: Thu Nov 10 13:11:05 2022, max compression
+gzip compressed data, was "play2048-5.0.tar", last modified: Sat Jul  1 10:48:26 2023, max compression
```

## Comparing `play2048-4.0.tar` & `play2048-5.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-11-10 13:11:06.000000 play2048-4.0/
--rw-rw-rw-   0        0        0      663 2022-11-10 13:11:06.000000 play2048-4.0/PKG-INFO
--rw-rw-rw-   0        0        0       82 2022-11-03 14:57:32.000000 play2048-4.0/README.md
-drwxrwxrwx   0        0        0        0 2022-11-10 13:11:06.000000 play2048-4.0/play2048/
--rw-rw-rw-   0        0        0       64 2022-11-03 14:37:26.000000 play2048-4.0/play2048/__init__.py
--rw-rw-rw-   0        0        0      978 2022-11-03 14:44:44.000000 play2048-4.0/play2048/custom.py
--rw-rw-rw-   0        0        0      912 2022-11-03 14:52:56.000000 play2048-4.0/play2048/enums.py
--rw-rw-rw-   0        0        0     8590 2022-11-10 12:52:36.000000 play2048-4.0/play2048/game.py
-drwxrwxrwx   0        0        0        0 2022-11-10 13:11:06.000000 play2048-4.0/play2048.egg-info/
--rw-rw-rw-   0        0        0      663 2022-11-10 13:11:06.000000 play2048-4.0/play2048.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2022-11-10 13:11:06.000000 play2048-4.0/play2048.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-10 13:11:06.000000 play2048-4.0/play2048.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-11-10 13:11:06.000000 play2048-4.0/play2048.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2022-11-10 13:11:06.000000 play2048-4.0/play2048.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-11-10 13:11:06.000000 play2048-4.0/play2048.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-11-10 13:11:06.000000 play2048-4.0/setup.cfg
--rw-rw-rw-   0        0        0      957 2022-11-10 13:10:18.000000 play2048-4.0/setup.py
+drwxrwxr-x   0 dev5-23   (1000) dev5-23   (1000)        0 2023-07-01 10:48:26.326648 play2048-5.0/
+-rw-rw-r--   0 dev5-23   (1000) dev5-23   (1000)     1066 2023-07-01 10:39:38.000000 play2048-5.0/LICENSE
+-rw-rw-r--   0 dev5-23   (1000) dev5-23   (1000)      436 2023-07-01 10:48:26.326648 play2048-5.0/PKG-INFO
+-rw-rw-r--   0 dev5-23   (1000) dev5-23   (1000)       81 2023-07-01 10:45:57.000000 play2048-5.0/README.md
+drwxrwxr-x   0 dev5-23   (1000) dev5-23   (1000)        0 2023-07-01 10:48:26.326648 play2048-5.0/play2048/
+-rw-rw-r--   0 dev5-23   (1000) dev5-23   (1000)       64 2023-07-01 10:39:38.000000 play2048-5.0/play2048/__init__.py
+-rw-rw-r--   0 dev5-23   (1000) dev5-23   (1000)      978 2023-07-01 10:39:38.000000 play2048-5.0/play2048/custom.py
+-rw-rw-r--   0 dev5-23   (1000) dev5-23   (1000)      914 2023-07-01 10:39:38.000000 play2048-5.0/play2048/enums.py
+-rw-rw-r--   0 dev5-23   (1000) dev5-23   (1000)     8496 2023-07-01 10:39:38.000000 play2048-5.0/play2048/game.py
+drwxrwxr-x   0 dev5-23   (1000) dev5-23   (1000)        0 2023-07-01 10:48:26.326648 play2048-5.0/play2048.egg-info/
+-rw-rw-r--   0 dev5-23   (1000) dev5-23   (1000)      436 2023-07-01 10:48:26.000000 play2048-5.0/play2048.egg-info/PKG-INFO
+-rw-rw-r--   0 dev5-23   (1000) dev5-23   (1000)      229 2023-07-01 10:48:26.000000 play2048-5.0/play2048.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev5-23   (1000) dev5-23   (1000)        1 2023-07-01 10:48:26.000000 play2048-5.0/play2048.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev5-23   (1000) dev5-23   (1000)        9 2023-07-01 10:48:26.000000 play2048-5.0/play2048.egg-info/top_level.txt
+-rw-rw-r--   0 dev5-23   (1000) dev5-23   (1000)       38 2023-07-01 10:48:26.326648 play2048-5.0/setup.cfg
+-rw-rw-r--   0 dev5-23   (1000) dev5-23   (1000)      533 2023-07-01 10:47:40.000000 play2048-5.0/setup.py
```

### Comparing `play2048-4.0/play2048/custom.py` & `play2048-5.0/play2048/custom.py`

 * *Files identical despite different names*

### Comparing `play2048-4.0/play2048/enums.py` & `play2048-5.0/play2048/enums.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -29,8 +29,8 @@
         _4 = "#EEE1C9",
         _8 = "#F3B27A",
         _16 = "#F69664",
         _32 = "#F77C5F",
         _64 = "#F75F3B",
         font_2 = "#776265",
         font_4 = "#776265"
-    )
+    )
```

### Comparing `play2048-4.0/play2048/game.py` & `play2048-5.0/play2048/game.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,14 @@
     [@see cmd2048](https://github.com/objectiveTM/play2048/tree/main/examples/cmd2048.py)
     """
     def __init__(self, spown = lambda :(4 if random.randint(0, 10) == 0 else 2)) -> None:
         self.arr = [[0 for i in range(4)] for i in range(4)]
         self.point = 0
         self.spown = spown
         w = 0
-        self.arr[3 + w][2] = 2
-        self.arr[2 + w][2] = 8
-        self.arr[1 + w][2] = 2
 
         try:
             pos = self._random()
             self.arr[pos[0]][pos[1]] = self.spown()
         except:pass
     
     def move(self , key:move, _debug = False):
@@ -235,8 +232,8 @@
         print(f"point: {g.point}")
         g.move(m)
         print("\n")
         print(g.encodingText())
         
         
     
-    print(g.encodingText())
+    print(g.encodingText())
```

