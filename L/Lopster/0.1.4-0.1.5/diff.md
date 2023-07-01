# Comparing `tmp/Lopster-0.1.4.tar.gz` & `tmp/Lopster-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lopster-0.1.4.tar", last modified: Thu Jun 29 14:27:22 2023, max compression
+gzip compressed data, was "Lopster-0.1.5.tar", last modified: Sat Jul  1 18:47:27 2023, max compression
```

## Comparing `Lopster-0.1.4.tar` & `Lopster-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 14:27:22.742744 Lopster-0.1.4/
-drwxrwxrwx   0        0        0        0 2023-06-29 14:27:22.711488 Lopster-0.1.4/Lopster/
--rw-rw-rw-   0        0        0    11640 2023-06-29 14:26:24.000000 Lopster-0.1.4/Lopster/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:27:22.742744 Lopster-0.1.4/Lopster.egg-info/
--rw-rw-rw-   0        0        0      235 2023-06-29 14:27:22.000000 Lopster-0.1.4/Lopster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-06-29 14:27:22.000000 Lopster-0.1.4/Lopster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 14:27:22.000000 Lopster-0.1.4/Lopster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-29 14:27:22.000000 Lopster-0.1.4/Lopster.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-29 14:27:22.000000 Lopster-0.1.4/Lopster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      235 2023-06-29 14:27:22.742744 Lopster-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-29 14:27:22.742744 Lopster-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      383 2023-06-29 14:26:47.000000 Lopster-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 18:47:27.342308 Lopster-0.1.5/
+drwxrwxrwx   0        0        0        0 2023-07-01 18:47:27.311022 Lopster-0.1.5/Lopster/
+-rw-rw-rw-   0        0        0    11911 2023-07-01 18:47:06.000000 Lopster-0.1.5/Lopster/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 18:47:27.342308 Lopster-0.1.5/Lopster.egg-info/
+-rw-rw-rw-   0        0        0      235 2023-07-01 18:47:27.000000 Lopster-0.1.5/Lopster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-07-01 18:47:27.000000 Lopster-0.1.5/Lopster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 18:47:27.000000 Lopster-0.1.5/Lopster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-01 18:47:27.000000 Lopster-0.1.5/Lopster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-01 18:47:27.000000 Lopster-0.1.5/Lopster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      235 2023-07-01 18:47:27.342308 Lopster-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-01 18:47:27.342308 Lopster-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      383 2023-07-01 18:23:27.000000 Lopster-0.1.5/setup.py
```

### Comparing `Lopster-0.1.4/Lopster/__init__.py` & `Lopster-0.1.5/Lopster/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,114 @@
 import math
 import inspect
 import pygame
 import pygame.font
 
+class Event:
+    _event = []
+    def __init__(self, cond,event):
+        self._event.append(self)
+        self.cond = cond
+        self.event = event
 
+    def delete(self, sure):
+        if sure:
+            self._event.remove(self)
+class Mouse:
+    def __init__(self):
+        pass
+    def leftDown(self, event):
+        def evecond(window, eve):
+            if eve == pygame.MOUSEBUTTONDOWN:
+                return  True
+            else:
+                return False
+        def even(window, eve):
+            if eve.button == 1:
+                event(window, eve)
+        ev = Event(evecond, even)
+    def leftUp(self, event):
+        def evecond(window, eve):
+            if eve == pygame.MOUSEBUTTONUP:
+                return  True
+            else:
+                return False
+        def even(window, eve):
+            if eve.button == 1:
+                event(window, eve)
+        ev = Event(evecond, even)
+    def rightDown(self, event):
+        def evecond(window, eve):
+            if eve == pygame.MOUSEBUTTONDOWN:
+                return  True
+            else:
+                return False
+        def even(window, eve):
+            if eve.button == 3:
+                event(window, eve)
+        ev = Event(evecond, even)
+    def rightUp(self, event):
+        def evecond(window, eve):
+            if eve == pygame.MOUSEBUTTONUP:
+                return  True
+            else:
+                return False
+        def even(window, eve):
+            if eve.button == 3:
+                event(window, eve)
+        ev = Event(evecond, even)
+    def wheelUp(self, event):
+        def evecond(window, eve):
+            if eve == pygame.MOUSEBUTTONUP:
+                return  True
+            else:
+                return False
+        def even(window, eve):
+            if eve.button == 2:
+                event(window, eve)
+        ev = Event(evecond, even)
+    def wheelDown(self, event):
+        def evecond(window, eve):
+            if eve == pygame.MOUSEBUTTONDOWN:
+                return  True
+            else:
+                return False
+        def even(window, eve):
+            if eve.button == 2:
+                event(window, eve)
+        ev = Event(evecond, even)
+    def wheelForward(self, event):
+        def evecond(window, eve):
+            if eve == pygame.MOUSEBUTTONDOWN:
+                return  True
+            else:
+                return False
+        def even(window, eve):
+            if eve.button == 4:
+                event(window, eve)
+        ev = Event(evecond, even)
+    def wheelBack(self, event):
+        def evecond(window, eve):
+            if eve == pygame.MOUSEBUTTONDOWN:
+                return  True
+            else:
+                return False
+        def even(window, eve):
+            if eve.button == 5:
+                event(window, eve)
+        ev = Event(evecond, even)
+    def move(self, event):
+        def evecond(window, eve):
+            if eve == pygame.MOUSEMOTION:
+                return  True
+            else:
+                return False
+        def even(window, eve):
+            event(window, eve)
+        ev = Event(evecond, even)
 class Enemy:
     _object = []
     typ = "Enemy"
 
     def __init__(self, _x, _y, _h, _w, _update):
         self._object.append(self)
         self.x = _x
@@ -22,14 +123,22 @@
 
     def hide(self):
         self.typ = "NoN"
 
     def visible(self, typ):
         self.typ = typ
 
+    def onClick(self, event):
+        def is_clicked(window, eve):
+            if self.x <= eve.pos[0] <= self.x + self.w and self.y <= eve.pos[1] <= self.y + self.h:
+                event(window, eve)
+
+        mouse = Mouse()
+        mouse.leftDown(is_clicked)
+
     def cash(self):
         text = []
 
         text.append("Enemy\n")
         text.append("x = " + str(self.x) + "\n")
         text.append("y = " + str(self.y) + "\n")
         text.append("h = " + str(self.h) + "\n")
@@ -243,116 +352,15 @@
         for card in map:
             if not type(card) == "tuple":
                 drawMap[card](self.window, "NoN")
             else:
                 for subCard in card:
                     drawMap[subCard](self.window, card)
 
-class Event:
-    _event = []
-    def __init__(self, cond,event):
-        self._event.append(self)
-        self.cond = cond
-        self.event = event
 
-    def delete(self, sure):
-        if sure:
-            self._event.remove(self)
-class Mouse:
-    def __init__(self):
-        pass
-    def leftDown(self, event):
-        def evecond(window, eve):
-            if eve == pygame.MOUSEBUTTONDOWN:
-                return  True
-            else:
-                return False
-        def even(window, eve):
-            if eve.button == 1:
-                event(window, eve)
-        ev = Event(evecond, even)
-    def leftUp(self, event):
-        def evecond(window, eve):
-            if eve == pygame.MOUSEBUTTONUP:
-                return  True
-            else:
-                return False
-        def even(window, eve):
-            if eve.button == 1:
-                event(window, eve)
-        ev = Event(evecond, even)
-    def rightDown(self, event):
-        def evecond(window, eve):
-            if eve == pygame.MOUSEBUTTONDOWN:
-                return  True
-            else:
-                return False
-        def even(window, eve):
-            if eve.button == 3:
-                event(window, eve)
-        ev = Event(evecond, even)
-    def rightUp(self, event):
-        def evecond(window, eve):
-            if eve == pygame.MOUSEBUTTONUP:
-                return  True
-            else:
-                return False
-        def even(window, eve):
-            if eve.button == 3:
-                event(window, eve)
-        ev = Event(evecond, even)
-    def wheelUp(self, event):
-        def evecond(window, eve):
-            if eve == pygame.MOUSEBUTTONUP:
-                return  True
-            else:
-                return False
-        def even(window, eve):
-            if eve.button == 2:
-                event(window, eve)
-        ev = Event(evecond, even)
-    def wheelDown(self, event):
-        def evecond(window, eve):
-            if eve == pygame.MOUSEBUTTONDOWN:
-                return  True
-            else:
-                return False
-        def even(window, eve):
-            if eve.button == 2:
-                event(window, eve)
-        ev = Event(evecond, even)
-    def wheelForward(self, event):
-        def evecond(window, eve):
-            if eve == pygame.MOUSEBUTTONDOWN:
-                return  True
-            else:
-                return False
-        def even(window, eve):
-            if eve.button == 4:
-                event(window, eve)
-        ev = Event(evecond, even)
-    def wheelBack(self, event):
-        def evecond(window, eve):
-            if eve == pygame.MOUSEBUTTONDOWN:
-                return  True
-            else:
-                return False
-        def even(window, eve):
-            if eve.button == 5:
-                event(window, eve)
-        ev = Event(evecond, even)
-    def move(self, event):
-        def evecond(window, eve):
-            if eve == pygame.MOUSEMOTION:
-                return  True
-            else:
-                return False
-        def even(window, eve):
-            event(window, eve)
-        ev = Event(evecond, even)
 class RunLopster:
     _fps = 16
 
     def __init__(self, window_size, title, icon, update, fps):
         self._window_size = window_size
         self._title = title
         self._update = update
```

