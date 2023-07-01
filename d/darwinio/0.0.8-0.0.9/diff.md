# Comparing `tmp/darwinio-0.0.8.tar.gz` & `tmp/darwinio-0.0.9.tar.gz`

## Comparing `darwinio-0.0.8.tar` & `darwinio-0.0.9.tar`

### file list

```diff
@@ -1,45 +1,47 @@
--rwxr-xr-x   0        0        0     1873 2020-02-02 00:00:00.000000 darwinio-0.0.8/CONTRIBUTING.md
--rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 darwinio-0.0.8/requirements.txt
--rwxr-xr-x   0        0        0     5915 2020-02-02 00:00:00.000000 darwinio-0.0.8/documentation/characteristics.ods
--rwxr-xr-x   0        0        0      814 2020-02-02 00:00:00.000000 darwinio-0.0.8/documentation/earlystages.md
--rwxr-xr-x   0        0        0     2057 2020-02-02 00:00:00.000000 darwinio-0.0.8/documentation/implementation.md
--rwxr-xr-x   0        0        0     3062 2020-02-02 00:00:00.000000 darwinio-0.0.8/documentation/graphical_interface/empty_window.png
--rwxr-xr-x   0        0        0    11317 2020-02-02 00:00:00.000000 darwinio-0.0.8/documentation/graphical_interface/main_game.png
--rwxr-xr-x   0        0        0     7816 2020-02-02 00:00:00.000000 darwinio-0.0.8/documentation/graphical_interface/starting_window.png
--rwxr-xr-x   0        0        0    71751 2020-02-02 00:00:00.000000 darwinio-0.0.8/documentation/screenshot/main_game_play.png
--rwxr-xr-x   0        0        0    23470 2020-02-02 00:00:00.000000 darwinio-0.0.8/documentation/screenshot/titlescreen.png
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/__init__.py
--rwxr-xr-x   0        0        0     3415 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/__main__.py
--rwxr-xr-x   0        0        0     5467 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/brain.py
--rwxr-xr-x   0        0        0     2313 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/constants.py
--rwxr-xr-x   0        0        0    16148 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/distribution.py
--rwxr-xr-x   0        0        0     2697 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/genome.py
--rwxr-xr-x   0        0        0    20888 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/graphical_sim.py
--rwxr-xr-x   0        0        0     4012 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/organism.py
--rwxr-xr-x   0        0        0     1483 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/text_sim.py
--rwxr-xr-x   0        0        0     3767 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/assets/art/archaebacteria_halophile.png
--rwxr-xr-x   0        0        0     3805 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/assets/art/archaebacteria_methanogen.png
--rwxr-xr-x   0        0        0     3712 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/assets/art/archaebacteria_thermoacidophile.png
--rwxr-xr-x   0        0        0     5075 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/assets/art/eubacteria_BGA.png
--rwxr-xr-x   0        0        0     4533 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/assets/art/eubacteria_mycoplasma.png
--rwxr-xr-x   0        0        0     5241 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/assets/art/eubacteroa_chemosynthetic.png
--rwxr-xr-x   0        0        0     4269 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/assets/art/fungi-ascomycetes.png
--rwxr-xr-x   0        0        0     4427 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/assets/art/fungi-basidiomycetes.png
--rwxr-xr-x   0        0        0     3117 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/assets/art/fungi-deuteromycetes.png
--rwxr-xr-x   0        0        0    11139 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/assets/art/fungi-phycomycetes.png
--rwxr-xr-x   0        0        0     4609 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/assets/art/metaphyta-algae.png
--rwxr-xr-x   0        0        0     6760 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/assets/art/metaphyta-angiospermae.png
--rwxr-xr-x   0        0        0     4285 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/assets/art/metaphyta-bryophyta.png
--rwxr-xr-x   0        0        0     6598 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/assets/art/metaphyta-gymnospermae.png
--rwxr-xr-x   0        0        0     3474 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/assets/art/metaphyta-pterdiophyta.png
--rwxr-xr-x   0        0        0     4270 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/assets/art/protista_dinoflagellate.png
--rwxr-xr-x   0        0        0     2858 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/assets/art/protista_euglena.png
--rwxr-xr-x   0        0        0     3734 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/assets/art/protista_protozoan.png
--rwxr-xr-x   0        0        0     6104 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/assets/art/protista_slimemould.png
--rwxr-xr-x   0        0        0      859 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/assets/art/theme.json
--rwxr-xr-x   0        0        0  4128852 2020-02-02 00:00:00.000000 darwinio-0.0.8/src/darwinio/assets/audio/Darwinio.mp3
--rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 darwinio-0.0.8/.gitignore
--rwxr-xr-x   0        0        0    34915 2020-02-02 00:00:00.000000 darwinio-0.0.8/LICENSE.md
--rwxr-xr-x   0        0        0     2497 2020-02-02 00:00:00.000000 darwinio-0.0.8/README.md
--rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 darwinio-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 darwinio-0.0.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1873 2020-02-02 00:00:00.000000 darwinio-0.0.9/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 darwinio-0.0.9/requirements.txt
+-rwxr-xr-x   0        0        0     5915 2020-02-02 00:00:00.000000 darwinio-0.0.9/documentation/characteristics.ods
+-rwxr-xr-x   0        0        0     3002 2020-02-02 00:00:00.000000 darwinio-0.0.9/documentation/doc.md
+-rwxr-xr-x   0        0        0    86371 2020-02-02 00:00:00.000000 darwinio-0.0.9/documentation/doc.pdf
+-rwxr-xr-x   0        0        0      814 2020-02-02 00:00:00.000000 darwinio-0.0.9/documentation/earlystages.md
+-rwxr-xr-x   0        0        0     2057 2020-02-02 00:00:00.000000 darwinio-0.0.9/documentation/implementation.md
+-rwxr-xr-x   0        0        0     3062 2020-02-02 00:00:00.000000 darwinio-0.0.9/documentation/graphical_interface/empty_window.png
+-rwxr-xr-x   0        0        0    11317 2020-02-02 00:00:00.000000 darwinio-0.0.9/documentation/graphical_interface/main_game.png
+-rwxr-xr-x   0        0        0     7816 2020-02-02 00:00:00.000000 darwinio-0.0.9/documentation/graphical_interface/starting_window.png
+-rwxr-xr-x   0        0        0    71751 2020-02-02 00:00:00.000000 darwinio-0.0.9/documentation/screenshot/main_game_play.png
+-rwxr-xr-x   0        0        0    23470 2020-02-02 00:00:00.000000 darwinio-0.0.9/documentation/screenshot/titlescreen.png
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/__init__.py
+-rwxr-xr-x   0        0        0     3585 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/__main__.py
+-rwxr-xr-x   0        0        0     5467 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/brain.py
+-rwxr-xr-x   0        0        0     2313 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/constants.py
+-rwxr-xr-x   0        0        0    16148 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/distribution.py
+-rwxr-xr-x   0        0        0     2697 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/genome.py
+-rwxr-xr-x   0        0        0    20978 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/graphical_sim.py
+-rwxr-xr-x   0        0        0     4012 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/organism.py
+-rwxr-xr-x   0        0        0     1483 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/text_sim.py
+-rwxr-xr-x   0        0        0     3767 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/assets/art/archaebacteria_halophile.png
+-rwxr-xr-x   0        0        0     3805 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/assets/art/archaebacteria_methanogen.png
+-rwxr-xr-x   0        0        0     3712 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/assets/art/archaebacteria_thermoacidophile.png
+-rwxr-xr-x   0        0        0     5075 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/assets/art/eubacteria_BGA.png
+-rwxr-xr-x   0        0        0     4533 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/assets/art/eubacteria_mycoplasma.png
+-rwxr-xr-x   0        0        0     5241 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/assets/art/eubacteroa_chemosynthetic.png
+-rwxr-xr-x   0        0        0     4269 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/assets/art/fungi-ascomycetes.png
+-rwxr-xr-x   0        0        0     4427 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/assets/art/fungi-basidiomycetes.png
+-rwxr-xr-x   0        0        0     3117 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/assets/art/fungi-deuteromycetes.png
+-rwxr-xr-x   0        0        0    11139 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/assets/art/fungi-phycomycetes.png
+-rwxr-xr-x   0        0        0     4609 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/assets/art/metaphyta-algae.png
+-rwxr-xr-x   0        0        0     6760 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/assets/art/metaphyta-angiospermae.png
+-rwxr-xr-x   0        0        0     4285 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/assets/art/metaphyta-bryophyta.png
+-rwxr-xr-x   0        0        0     6598 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/assets/art/metaphyta-gymnospermae.png
+-rwxr-xr-x   0        0        0     3474 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/assets/art/metaphyta-pterdiophyta.png
+-rwxr-xr-x   0        0        0     4270 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/assets/art/protista_dinoflagellate.png
+-rwxr-xr-x   0        0        0     2858 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/assets/art/protista_euglena.png
+-rwxr-xr-x   0        0        0     3734 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/assets/art/protista_protozoan.png
+-rwxr-xr-x   0        0        0     6104 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/assets/art/protista_slimemould.png
+-rwxr-xr-x   0        0        0      859 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/assets/art/theme.json
+-rwxr-xr-x   0        0        0  4128852 2020-02-02 00:00:00.000000 darwinio-0.0.9/src/darwinio/assets/audio/Darwinio.mp3
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 darwinio-0.0.9/.gitignore
+-rwxr-xr-x   0        0        0    34915 2020-02-02 00:00:00.000000 darwinio-0.0.9/LICENSE.md
+-rwxr-xr-x   0        0        0     2497 2020-02-02 00:00:00.000000 darwinio-0.0.9/README.md
+-rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 darwinio-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 darwinio-0.0.9/PKG-INFO
```

### Comparing `darwinio-0.0.8/CONTRIBUTING.md` & `darwinio-0.0.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/documentation/characteristics.ods` & `darwinio-0.0.9/documentation/characteristics.ods`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/documentation/earlystages.md` & `darwinio-0.0.9/documentation/earlystages.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/documentation/implementation.md` & `darwinio-0.0.9/documentation/implementation.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/documentation/graphical_interface/empty_window.png` & `darwinio-0.0.9/documentation/graphical_interface/empty_window.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/documentation/graphical_interface/main_game.png` & `darwinio-0.0.9/documentation/graphical_interface/main_game.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/documentation/graphical_interface/starting_window.png` & `darwinio-0.0.9/documentation/graphical_interface/starting_window.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/documentation/screenshot/main_game_play.png` & `darwinio-0.0.9/documentation/screenshot/main_game_play.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/documentation/screenshot/titlescreen.png` & `darwinio-0.0.9/documentation/screenshot/titlescreen.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/src/darwinio/__main__.py` & `darwinio-0.0.9/src/darwinio/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,22 +50,30 @@
     pg.mixer.music.play()
 
     world = gsim.World(world_size)
 
     # Create the states
     title = gsim.TitleScreen(screen, constants.TITLE_ASCII_ART)
     license_notice = gsim.TextScreen(screen, constants.LICENSE_NOTICE, 2)
-    world_build = gsim.Organism_selection(screen, world)
-    help_screen = gsim.TextScreen(screen, constants.HELP, 4)
+    world_build = gsim.Organism_selection(screen, world, 4)
+    init_help_screen = gsim.TextScreen(screen, constants.HELP, 3)
+    help_screen = gsim.TextScreen(screen, constants.HELP, 5)
     with gsim.get_asset_path("art", "archaebacteria_halophile.png") as path:
         main_game = gsim.Simulation(screen, world, path)
 
     # Create the state machine
     statemachine = gsim.StateMachine(
-        [title, license_notice, world_build, main_game, help_screen]
+        [
+            title,
+            license_notice,
+            init_help_screen,
+            world_build,
+            main_game,
+            help_screen,
+        ]
     )
     while True:
         time_delta = clock.tick(fps) / 1000.0
 
         events = pg.event.get()
         for event in events:
             if event.type == pg.QUIT:
@@ -81,15 +89,15 @@
                     if music_playing:
                         pg.mixer.music.pause()
                     else:
                         pg.mixer.music.unpause()
                         music_playing = not music_playing
                 if event.mod & pg.KMOD_LSHIFT and event.key == pg.K_h:
                     prev_index: int = statemachine.state_index
-                    statemachine.state_index = 4
+                    statemachine.state_index = 5
                     help_screen.next_state_index = prev_index
 
         screen.fill("#423E4A")
         statemachine.run_state(events, time_delta)
         pg.display.flip()
```

### Comparing `darwinio-0.0.8/src/darwinio/brain.py` & `darwinio-0.0.9/src/darwinio/brain.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/src/darwinio/constants.py` & `darwinio-0.0.9/src/darwinio/constants.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/src/darwinio/distribution.py` & `darwinio-0.0.9/src/darwinio/distribution.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/src/darwinio/genome.py` & `darwinio-0.0.9/src/darwinio/genome.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/src/darwinio/graphical_sim.py` & `darwinio-0.0.9/src/darwinio/graphical_sim.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,17 +217,22 @@
     done_button (pgui.elements.UIButton): The button for indicating completion
     of organism selection.
 
     skip_button (pgui.elements.UIButton): The button for skipping organism
     selection.
     """
 
-    def __init__(self, surface: pg.Surface, world: World):
+    def __init__(
+        self,
+        surface: pg.Surface,
+        world: World,
+        next_state_index: Union[int, None],
+    ):
         surface_size = width, height = surface.get_size()
-        super().__init__(surface, surface_size, 3)
+        super().__init__(surface, surface_size, next_state_index)
         self.world: World = world
 
         self.title = pgui.elements.UITextBox(
             "<b>Select the range of your random organisms</b>",
             pg.Rect((width // 2) - 350 // 2, 50, 350, 50),
             self.manager,
         )
@@ -436,15 +441,15 @@
         for event in events:
             if event.type == pgui.UI_BUTTON_PRESSED:
                 if event.ui_element == self.start_button:
                     self.running = not self.running
                     self.last_time = 0
                 if event.ui_element == self.restart_button:
                     self.running = False
-                    return 2
+                    return 3
             if event.type == pg.KEYDOWN:
                 if event.key == pg.K_SPACE:
                     self.running = not self.running
                     self.last_time = 0
 
             # change the temp/food content
             if event.type == pgui.UI_HORIZONTAL_SLIDER_MOVED:
```

### Comparing `darwinio-0.0.8/src/darwinio/organism.py` & `darwinio-0.0.9/src/darwinio/organism.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/src/darwinio/text_sim.py` & `darwinio-0.0.9/src/darwinio/text_sim.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/src/darwinio/assets/art/archaebacteria_halophile.png` & `darwinio-0.0.9/src/darwinio/assets/art/archaebacteria_halophile.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/src/darwinio/assets/art/archaebacteria_methanogen.png` & `darwinio-0.0.9/src/darwinio/assets/art/archaebacteria_methanogen.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/src/darwinio/assets/art/archaebacteria_thermoacidophile.png` & `darwinio-0.0.9/src/darwinio/assets/art/archaebacteria_thermoacidophile.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/src/darwinio/assets/art/eubacteria_BGA.png` & `darwinio-0.0.9/src/darwinio/assets/art/eubacteria_BGA.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/src/darwinio/assets/art/eubacteria_mycoplasma.png` & `darwinio-0.0.9/src/darwinio/assets/art/eubacteria_mycoplasma.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/src/darwinio/assets/art/eubacteroa_chemosynthetic.png` & `darwinio-0.0.9/src/darwinio/assets/art/eubacteroa_chemosynthetic.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/src/darwinio/assets/art/fungi-ascomycetes.png` & `darwinio-0.0.9/src/darwinio/assets/art/fungi-ascomycetes.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/src/darwinio/assets/art/fungi-basidiomycetes.png` & `darwinio-0.0.9/src/darwinio/assets/art/fungi-basidiomycetes.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/src/darwinio/assets/art/fungi-deuteromycetes.png` & `darwinio-0.0.9/src/darwinio/assets/art/fungi-deuteromycetes.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/src/darwinio/assets/art/fungi-phycomycetes.png` & `darwinio-0.0.9/src/darwinio/assets/art/fungi-phycomycetes.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/src/darwinio/assets/art/metaphyta-algae.png` & `darwinio-0.0.9/src/darwinio/assets/art/metaphyta-algae.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/src/darwinio/assets/art/metaphyta-angiospermae.png` & `darwinio-0.0.9/src/darwinio/assets/art/metaphyta-angiospermae.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/src/darwinio/assets/art/metaphyta-bryophyta.png` & `darwinio-0.0.9/src/darwinio/assets/art/metaphyta-bryophyta.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/src/darwinio/assets/art/metaphyta-gymnospermae.png` & `darwinio-0.0.9/src/darwinio/assets/art/metaphyta-gymnospermae.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/src/darwinio/assets/art/metaphyta-pterdiophyta.png` & `darwinio-0.0.9/src/darwinio/assets/art/metaphyta-pterdiophyta.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/src/darwinio/assets/art/protista_dinoflagellate.png` & `darwinio-0.0.9/src/darwinio/assets/art/protista_dinoflagellate.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/src/darwinio/assets/art/protista_euglena.png` & `darwinio-0.0.9/src/darwinio/assets/art/protista_euglena.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/src/darwinio/assets/art/protista_protozoan.png` & `darwinio-0.0.9/src/darwinio/assets/art/protista_protozoan.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/src/darwinio/assets/art/protista_slimemould.png` & `darwinio-0.0.9/src/darwinio/assets/art/protista_slimemould.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/src/darwinio/assets/art/theme.json` & `darwinio-0.0.9/src/darwinio/assets/art/theme.json`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/src/darwinio/assets/audio/Darwinio.mp3` & `darwinio-0.0.9/src/darwinio/assets/audio/Darwinio.mp3`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/LICENSE.md` & `darwinio-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/README.md` & `darwinio-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.0.8/pyproject.toml` & `darwinio-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [tool.hatch.build]
 exclude = [
   "*.wav",
 ]
 
 [project]
 name = "darwinio"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Tushar Maharana", email="tusharhero@sdf.org" },
   { name="Mihir Nallagonda", email="adhikshithamihir@gmail.com" },
 ]
 description = "An evolution simulator"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `darwinio-0.0.8/PKG-INFO` & `darwinio-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darwinio
-Version: 0.0.8
+Version: 0.0.9
 Summary: An evolution simulator
 Project-URL: Homepage, https://github.com/tusharhero/darwinio
 Project-URL: Bug Tracker, https://github.com/tusharhero/darwinio/issues
 Author-email: Tushar Maharana <tusharhero@sdf.org>, Mihir Nallagonda <adhikshithamihir@gmail.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

