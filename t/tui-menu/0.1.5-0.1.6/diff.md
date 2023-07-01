# Comparing `tmp/tui-menu-0.1.5.tar.gz` & `tmp/tui-menu-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tui-menu-0.1.5.tar", last modified: Sat Jul  1 10:30:33 2023, max compression
+gzip compressed data, was "tui-menu-0.1.6.tar", last modified: Sat Jul  1 11:20:30 2023, max compression
```

## Comparing `tui-menu-0.1.5.tar` & `tui-menu-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 avili      (501) staff       (20)        0 2023-07-01 10:30:33.543769 tui-menu-0.1.5/
--rw-r--r--   0 avili      (501) staff       (20)      891 2023-07-01 10:30:33.543649 tui-menu-0.1.5/PKG-INFO
--rw-r--r--   0 avili      (501) staff       (20)     1239 2023-07-01 10:30:19.000000 tui-menu-0.1.5/pyproject.toml
--rw-r--r--   0 avili      (501) staff       (20)       38 2023-07-01 10:30:33.543810 tui-menu-0.1.5/setup.cfg
--rw-r--r--   0 avili      (501) staff       (20)      880 2023-07-01 10:30:19.000000 tui-menu-0.1.5/setup.py
-drwxr-xr-x   0 avili      (501) staff       (20)        0 2023-07-01 10:30:33.542689 tui-menu-0.1.5/tui-menu/
--rwxr-xr-x   0 avili      (501) staff       (20)     7260 2023-06-30 13:14:02.000000 tui-menu-0.1.5/tui-menu/Menu.py
--rw-r--r--   0 avili      (501) staff       (20)      148 2023-07-01 10:30:19.000000 tui-menu-0.1.5/tui-menu/__init__.py
-drwxr-xr-x   0 avili      (501) staff       (20)        0 2023-07-01 10:30:33.543469 tui-menu-0.1.5/tui_menu.egg-info/
--rw-r--r--   0 avili      (501) staff       (20)      891 2023-07-01 10:30:33.000000 tui-menu-0.1.5/tui_menu.egg-info/PKG-INFO
--rw-r--r--   0 avili      (501) staff       (20)      220 2023-07-01 10:30:33.000000 tui-menu-0.1.5/tui_menu.egg-info/SOURCES.txt
--rw-r--r--   0 avili      (501) staff       (20)        1 2023-07-01 10:30:33.000000 tui-menu-0.1.5/tui_menu.egg-info/dependency_links.txt
--rw-r--r--   0 avili      (501) staff       (20)       28 2023-07-01 10:30:33.000000 tui-menu-0.1.5/tui_menu.egg-info/requires.txt
--rw-r--r--   0 avili      (501) staff       (20)        9 2023-07-01 10:30:33.000000 tui-menu-0.1.5/tui_menu.egg-info/top_level.txt
+drwxr-xr-x   0 avili      (501) staff       (20)        0 2023-07-01 11:20:30.458062 tui-menu-0.1.6/
+-rw-r--r--   0 avili      (501) staff       (20)    35149 2023-07-01 10:44:37.000000 tui-menu-0.1.6/LICENSE
+-rw-r--r--   0 avili      (501) staff       (20)      971 2023-07-01 11:20:30.457922 tui-menu-0.1.6/PKG-INFO
+-rw-r--r--   0 avili      (501) staff       (20)       57 2023-07-01 10:44:37.000000 tui-menu-0.1.6/README.md
+-rw-r--r--   0 avili      (501) staff       (20)     1275 2023-07-01 10:58:37.000000 tui-menu-0.1.6/pyproject.toml
+-rw-r--r--   0 avili      (501) staff       (20)       38 2023-07-01 11:20:30.458109 tui-menu-0.1.6/setup.cfg
+-rw-r--r--   0 avili      (501) staff       (20)     1378 2023-07-01 11:03:01.000000 tui-menu-0.1.6/setup.py
+drwxr-xr-x   0 avili      (501) staff       (20)        0 2023-07-01 11:20:30.456940 tui-menu-0.1.6/tui-menu/
+-rwxr-xr-x   0 avili      (501) staff       (20)     7205 2023-07-01 10:48:57.000000 tui-menu-0.1.6/tui-menu/Menu.py
+-rw-r--r--   0 avili      (501) staff       (20)      148 2023-07-01 10:50:01.000000 tui-menu-0.1.6/tui-menu/__init__.py
+drwxr-xr-x   0 avili      (501) staff       (20)        0 2023-07-01 11:20:30.457712 tui-menu-0.1.6/tui_menu.egg-info/
+-rw-r--r--   0 avili      (501) staff       (20)      971 2023-07-01 11:20:30.000000 tui-menu-0.1.6/tui_menu.egg-info/PKG-INFO
+-rw-r--r--   0 avili      (501) staff       (20)      238 2023-07-01 11:20:30.000000 tui-menu-0.1.6/tui_menu.egg-info/SOURCES.txt
+-rw-r--r--   0 avili      (501) staff       (20)        1 2023-07-01 11:20:30.000000 tui-menu-0.1.6/tui_menu.egg-info/dependency_links.txt
+-rw-r--r--   0 avili      (501) staff       (20)       28 2023-07-01 11:20:30.000000 tui-menu-0.1.6/tui_menu.egg-info/requires.txt
+-rw-r--r--   0 avili      (501) staff       (20)        9 2023-07-01 11:20:30.000000 tui-menu-0.1.6/tui_menu.egg-info/top_level.txt
```

### Comparing `tui-menu-0.1.5/PKG-INFO` & `tui-menu-0.1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui-menu
-Version: 0.1.5
+Version: 0.1.6
 Summary: A module for TUI Menu driven application
 Home-page: https://github.com/avili68/tui-menu
 Author: Avi Liani
 Author-email: Avi Liani <avi@liani.co.il>
 Maintainer-email: Avi Liani <avi@liani.co.il>
 Project-URL: Repository, https://github.com/avili68/tui-menu
 Keywords: console,menu,tui
@@ -16,7 +16,12 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# TUI-Menu
+
+This is a Module for Menu driven TUI scripts
```

### Comparing `tui-menu-0.1.5/pyproject.toml` & `tui-menu-0.1.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools >= 65",
     "wheel >= 0.38",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tui-menu"
-version = "0.1.5"
+dynamic = ["version"]
 description = "A module for TUI Menu driven application"
 readme = "README.md"
 requires-python = ">=3"
 license = {file = "LICENSE.txt"}
 keywords = ["console", "menu", "tui"]
 authors = [
     {name = "Avi Liani", email = "avi@liani.co.il"},
@@ -33,14 +33,15 @@
 ]
 
 dependencies = [
     "console>=0.9907",
     "ezenv>=0.92"
 ]
 
-# dynamic = ["version", "description"]
+[tool.setuptools.dynamic]
+version = {attr = "tui-menu.__version__"}
 
 [project.urls]
-#Homepage = "https://example.com"
-#Documentation = "https://readthedocs.org"
+# Homepage = "https://example.com"
+# Documentation = "https://readthedocs.org"
 Repository = "https://github.com/avili68/tui-menu"
-#Changelog = "https://github.com/me/spam/blob/master/CHANGELOG.md"
+# Changelog = "https://github.com/me/spam/blob/master/CHANGELOG.md"
```

### Comparing `tui-menu-0.1.5/tui-menu/Menu.py` & `tui-menu-0.1.6/tui-menu/Menu.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,16 +166,15 @@
         Returns:
             int : the line where the courser need to be
         """
         row = 1
         clear_screen()
         # display the menu title with underline of '='
         row = print_in_line(row, 6, fx.italic + self.title() + fx.end)
-        row = print_in_line(row, 5, "=" * (len(self.title()) + 2))
-        row += 1
+        row = print_in_line(row, 5, "=" * (len(self.title()) + 2)) + 1
 
         # generate sorted list of menu options
         keys_list = list(self._items)
         keys_list.sort()
 
         for key in keys_list:
             string_line = f"{key} ) {self._items[key].value()}"
@@ -183,19 +182,17 @@
                 # if menu option is a sub-menu add '->' to indicate it
                 string_line += " -->"
             row = print_in_line(row, 6, string_line)
 
         if self.level() != 0:
             # if sub-menu, add the 'return' option
             row = print_in_line(row + 1, 6, "r ) Return to previous menu") + 1
-            # row += 2
 
         # add the 'exit' option
         row = print_in_line(row + 1, 6, "x ) Exit") + 1
-        # row += 2
 
         return row
 
     def get_option(self):
         """
         get the menu selected option from the user.
         make sure only valid option  was pressed
```

### Comparing `tui-menu-0.1.5/tui_menu.egg-info/PKG-INFO` & `tui-menu-0.1.6/tui_menu.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui-menu
-Version: 0.1.5
+Version: 0.1.6
 Summary: A module for TUI Menu driven application
 Home-page: https://github.com/avili68/tui-menu
 Author: Avi Liani
 Author-email: Avi Liani <avi@liani.co.il>
 Maintainer-email: Avi Liani <avi@liani.co.il>
 Project-URL: Repository, https://github.com/avili68/tui-menu
 Keywords: console,menu,tui
@@ -16,7 +16,12 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# TUI-Menu
+
+This is a Module for Menu driven TUI scripts
```

