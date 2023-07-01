# Comparing `tmp/cursesdict-0.11.tar.gz` & `tmp/cursesdict-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cursesdict-0.11.tar", last modified: Sat Jul  1 05:53:05 2023, max compression
+gzip compressed data, was "cursesdict-0.12.tar", last modified: Sat Jul  1 06:02:36 2023, max compression
```

## Comparing `cursesdict-0.11.tar` & `cursesdict-0.12.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 05:53:05.024044 cursesdict-0.11/
--rw-rw-rw-   0        0        0     1148 2023-07-01 05:52:57.000000 cursesdict-0.11/LICENSE.rst
--rw-rw-rw-   0        0        0      101 2023-07-01 05:52:54.000000 cursesdict-0.11/MANIFEST.in
--rw-rw-rw-   0        0        0     7734 2023-07-01 05:53:05.024044 cursesdict-0.11/PKG-INFO
--rw-rw-rw-   0        0        0     6996 2023-07-01 05:52:39.000000 cursesdict-0.11/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 05:53:05.021052 cursesdict-0.11/cursesdict/
--rw-rw-rw-   0        0        0     6996 2023-07-01 05:52:39.000000 cursesdict-0.11/cursesdict/README.MD
--rw-rw-rw-   0        0        0    11645 2023-07-01 05:42:08.000000 cursesdict-0.11/cursesdict/__init__.py
--rw-rw-rw-   0        0        0       18 2023-07-01 05:53:04.000000 cursesdict-0.11/cursesdict/requirements.txt
--rw-rw-rw-   0        0        0     1256 2023-07-01 05:53:04.000000 cursesdict-0.11/cursesdict/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-07-01 05:53:05.024044 cursesdict-0.11/cursesdict.egg-info/
--rw-rw-rw-   0        0        0     7734 2023-07-01 05:53:04.000000 cursesdict-0.11/cursesdict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-01 05:53:04.000000 cursesdict-0.11/cursesdict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 05:53:04.000000 cursesdict-0.11/cursesdict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-01 05:53:04.000000 cursesdict-0.11/cursesdict.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-01 05:53:04.000000 cursesdict-0.11/cursesdict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-07-01 05:53:05.025041 cursesdict-0.11/setup.cfg
--rw-rw-rw-   0        0        0     1414 2023-07-01 05:53:04.000000 cursesdict-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 06:02:36.365243 cursesdict-0.12/
+-rw-rw-rw-   0        0        0     1148 2023-07-01 06:02:31.000000 cursesdict-0.12/LICENSE.rst
+-rw-rw-rw-   0        0        0      101 2023-07-01 06:02:29.000000 cursesdict-0.12/MANIFEST.in
+-rw-rw-rw-   0        0        0     9062 2023-07-01 06:02:36.365243 cursesdict-0.12/PKG-INFO
+-rw-rw-rw-   0        0        0     8324 2023-07-01 06:01:17.000000 cursesdict-0.12/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 06:02:36.361254 cursesdict-0.12/cursesdict/
+-rw-rw-rw-   0        0        0     8324 2023-07-01 06:01:17.000000 cursesdict-0.12/cursesdict/README.MD
+-rw-rw-rw-   0        0        0    11442 2023-07-01 05:58:30.000000 cursesdict-0.12/cursesdict/__init__.py
+-rw-rw-rw-   0        0        0       18 2023-07-01 06:02:35.000000 cursesdict-0.12/cursesdict/requirements.txt
+-rw-rw-rw-   0        0        0     1256 2023-07-01 06:02:35.000000 cursesdict-0.12/cursesdict/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-07-01 06:02:36.365243 cursesdict-0.12/cursesdict.egg-info/
+-rw-rw-rw-   0        0        0     9062 2023-07-01 06:02:36.000000 cursesdict-0.12/cursesdict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-01 06:02:36.000000 cursesdict-0.12/cursesdict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 06:02:36.000000 cursesdict-0.12/cursesdict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-01 06:02:36.000000 cursesdict-0.12/cursesdict.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-01 06:02:36.000000 cursesdict-0.12/cursesdict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-07-01 06:02:36.367238 cursesdict-0.12/setup.cfg
+-rw-rw-rw-   0        0        0     1414 2023-07-01 06:02:35.000000 cursesdict-0.12/setup.py
```

### Comparing `cursesdict-0.11/LICENSE.rst` & `cursesdict-0.12/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `cursesdict-0.11/PKG-INFO` & `cursesdict-0.12/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,13 @@
-Metadata-Version: 2.1
-Name: cursesdict
-Version: 0.11
-Summary: creates an interactive menu system for your application or program, providing an intuitive and user-friendly interface for users to navigate and perform various actions
-Home-page: https://github.com/hansalemaos/cursesdict
-Author: Johannes Fischer
-Author-email: aulasparticularesdealemaosp@gmail.com
-License: MIT
-Keywords: curses,menu
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE.rst
-
-
 # creates an interactive menu system for your application or program, providing an intuitive and user-friendly interface for users to navigate and perform various actions
 
 ## pip install cursesdict
 
 #### Tested against Windows 10 / Python 3.10 / Anaconda 
-#### curses from https://www.lfd.uci.edu/~gohlke/pythonlibs/#curses
+#### install curses from https://www.lfd.uci.edu/~gohlke/pythonlibs/#curses
 
 
 ### Simplifies menu creation: 
 
 The start_menu function abstracts away the complexities of handling user input and managing the menu structure. It provides a convenient way to define menus and associate actions with menu options.
 
 ### Customizable appearance: 
@@ -44,14 +26,16 @@
 
 The module is designed to be flexible and easily extensible. You can modify the menu structure, add new options, and define custom actions according to your requirements.
 
 
 
 ```python
 
+# Important! The script can't be executed from ipython, Pycharm, the terminal, etc. 
+# Open cmd.exe, activate your env, and start the script!
 
 start_menu(
     menudict: dict,
     menu_len: int = 40,
     n_spaces_right: int = 5,
     n_spaces_left: int = 2,
     menu_len_selected: int = 40,
@@ -102,96 +86,100 @@
 
 The start_menu function is called with the stama dictionary as the argument. This will display the menu and allow the user to navigate and interact with the options.
 
 	
 	
 ```python
 import subprocess
-from cursesdict import start_menu
+
+from cursesdict import start_menu, menu_config
+
 
 def fufu1(key):
-	filetest = "c:\\testestestest.txt"
-	with open(filetest, mode="w", encoding="utf-8") as f:
-		f.write(str(key))
-		f.write("\n")
-	subprocess.Popen(f"notepad.exe {filetest}", shell=True)
+    filetest = "c:\\testestestest.txt"
+    with open(filetest, mode="w", encoding="utf-8") as f:
+        f.write(str(key))
+        f.write("\n")
+    subprocess.Popen(f"notepad.exe {filetest}", shell=True)
+    menu_config.is_active = False  # exits the menu
 
 
 stama = {
-	"main": {
-		"menu_header": "Imaginary School - Main Menu",
-		"option_0": {
-			"Exercises": lambda: fufu1("Imaginary School - Main Menu - Exercises")
-		},
-		"option_1": {"Review": lambda: fufu1("Imaginary School - Main Menu - Review")},
-		"option_2": {
-			"Talk to a teacher": lambda: fufu1(
-				"Imaginary School - Main Menu - Talk to a teacher"
-			)
-		},
-		"option_3": {
-			"Blackboard": lambda: fufu1("Imaginary School - Main Menu - Blackboard")
-		},
-		"option_4": {
-			"Vocabulary Training": {
-				"menu_header": "Welcome to the Vocabulary Training section:",
-				"option_0": {
-					"A1": lambda: fufu1(
-						"Imaginary School - Main Menu - Vocabulary Training - A1"
-					)
-				},
-				"option_1": {
-					"A2": lambda: fufu1(
-						"Imaginary School - Main Menu - Vocabulary Training - A2"
-					)
-				},
-				"option_2": {
-					"B1-B2": lambda: fufu1(
-						"Imaginary School - Main Menu - Vocabulary Training - B1-B2"
-					)
-				},
-				"option_3": {
-					"C1-C2": lambda: fufu1(
-						"Imaginary School - Main Menu - Vocabulary Training - C1-C2"
-					)
-				},
-				"option_4": {
-					"Training for Tests": {
-						"menu_header": "Specific Test Training",
-						"option_0": {
-							"Sub Option 0": lambda: fufu1(
-								"Imaginary School - Main Menu - Vocabulary Training - Suboption 0"
-							)
-						},
-						"option_1": {
-							"Sub Option 1": lambda: fufu1(
-								"Imaginary School - Main Menu - Vocabulary Training - Suboption 1"
-							)
-						},
-						"option_2": {
-							"Sub Option 2": lambda: fufu1(
-								"Imaginary School - Main Menu - Vocabulary Training - SubOption 2"
-							)
-						},
-						"option_3": {
-							"Sub Option 3": lambda: fufu1(
-								"Imaginary School - Main Menu - Vocabulary Training - Suboption 3"
-							)
-						},
-						"option_4": {
-							"Sub Option 4": lambda: fufu1(
-								"Imaginary School - Main Menu - Vocabulary Training - Suboption 4"
-							)
-						},
-						"option_5": {
-							"Go back": ("main", "option_4", "Vocabulary Training")
-						},
-					},
-				},
-				"option_5": {"Go back": ("main",)},
-			},
-		},
-	}
+    "main": {
+        "menu_header": "Imaginary School - Main Menu",
+        "option_0": {
+            "Exercises": lambda: fufu1("Imaginary School - Main Menu - Exercises")
+        },
+        "option_1": {"Review": lambda: fufu1("Imaginary School - Main Menu - Review")},
+        "option_2": {
+            "Talk to a teacher": lambda: fufu1(
+                "Imaginary School - Main Menu - Talk to a teacher"
+            )
+        },
+        "option_3": {
+            "Blackboard": lambda: fufu1("Imaginary School - Main Menu - Blackboard")
+        },
+        "option_4": {
+            "Vocabulary Training": {
+                "menu_header": "Welcome to the Vocabulary Training section:",
+                "option_0": {
+                    "A1": lambda: fufu1(
+                        "Imaginary School - Main Menu - Vocabulary Training - A1"
+                    )
+                },
+                "option_1": {
+                    "A2": lambda: fufu1(
+                        "Imaginary School - Main Menu - Vocabulary Training - A2"
+                    )
+                },
+                "option_2": {
+                    "B1-B2": lambda: fufu1(
+                        "Imaginary School - Main Menu - Vocabulary Training - B1-B2"
+                    )
+                },
+                "option_3": {
+                    "C1-C2": lambda: fufu1(
+                        "Imaginary School - Main Menu - Vocabulary Training - C1-C2"
+                    )
+                },
+                "option_4": {
+                    "Training for Tests": {
+                        "menu_header": "Specific Test Training",
+                        "option_0": {
+                            "Sub Option 0": lambda: fufu1(
+                                "Imaginary School - Main Menu - Vocabulary Training - Suboption 0"
+                            )
+                        },
+                        "option_1": {
+                            "Sub Option 1": lambda: fufu1(
+                                "Imaginary School - Main Menu - Vocabulary Training - Suboption 1"
+                            )
+                        },
+                        "option_2": {
+                            "Sub Option 2": lambda: fufu1(
+                                "Imaginary School - Main Menu - Vocabulary Training - SubOption 2"
+                            )
+                        },
+                        "option_3": {
+                            "Sub Option 3": lambda: fufu1(
+                                "Imaginary School - Main Menu - Vocabulary Training - Suboption 3"
+                            )
+                        },
+                        "option_4": {
+                            "Sub Option 4": lambda: fufu1(
+                                "Imaginary School - Main Menu - Vocabulary Training - Suboption 4"
+                            )
+                        },
+                        "option_5": {
+                            "Go back": ("main", "option_4", "Vocabulary Training")
+                        },
+                    },
+                },
+                "option_5": {"Go back": ("main",)},
+            },
+        },
+    }
 }
 start_menu(stama)
 
-```
+
+```
```

### Comparing `cursesdict-0.11/README.md` & `cursesdict-0.12/cursesdict/README.MD`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # creates an interactive menu system for your application or program, providing an intuitive and user-friendly interface for users to navigate and perform various actions
 
 ## pip install cursesdict
 
 #### Tested against Windows 10 / Python 3.10 / Anaconda 
-#### curses from https://www.lfd.uci.edu/~gohlke/pythonlibs/#curses
+#### install curses from https://www.lfd.uci.edu/~gohlke/pythonlibs/#curses
 
 
 ### Simplifies menu creation: 
 
 The start_menu function abstracts away the complexities of handling user input and managing the menu structure. It provides a convenient way to define menus and associate actions with menu options.
 
 ### Customizable appearance: 
@@ -26,14 +26,16 @@
 
 The module is designed to be flexible and easily extensible. You can modify the menu structure, add new options, and define custom actions according to your requirements.
 
 
 
 ```python
 
+# Important! The script can't be executed from ipython, Pycharm, the terminal, etc. 
+# Open cmd.exe, activate your env, and start the script!
 
 start_menu(
     menudict: dict,
     menu_len: int = 40,
     n_spaces_right: int = 5,
     n_spaces_left: int = 2,
     menu_len_selected: int = 40,
@@ -84,96 +86,100 @@
 
 The start_menu function is called with the stama dictionary as the argument. This will display the menu and allow the user to navigate and interact with the options.
 
 	
 	
 ```python
 import subprocess
-from cursesdict import start_menu
+
+from cursesdict import start_menu, menu_config
+
 
 def fufu1(key):
-	filetest = "c:\\testestestest.txt"
-	with open(filetest, mode="w", encoding="utf-8") as f:
-		f.write(str(key))
-		f.write("\n")
-	subprocess.Popen(f"notepad.exe {filetest}", shell=True)
+    filetest = "c:\\testestestest.txt"
+    with open(filetest, mode="w", encoding="utf-8") as f:
+        f.write(str(key))
+        f.write("\n")
+    subprocess.Popen(f"notepad.exe {filetest}", shell=True)
+    menu_config.is_active = False  # exits the menu
 
 
 stama = {
-	"main": {
-		"menu_header": "Imaginary School - Main Menu",
-		"option_0": {
-			"Exercises": lambda: fufu1("Imaginary School - Main Menu - Exercises")
-		},
-		"option_1": {"Review": lambda: fufu1("Imaginary School - Main Menu - Review")},
-		"option_2": {
-			"Talk to a teacher": lambda: fufu1(
-				"Imaginary School - Main Menu - Talk to a teacher"
-			)
-		},
-		"option_3": {
-			"Blackboard": lambda: fufu1("Imaginary School - Main Menu - Blackboard")
-		},
-		"option_4": {
-			"Vocabulary Training": {
-				"menu_header": "Welcome to the Vocabulary Training section:",
-				"option_0": {
-					"A1": lambda: fufu1(
-						"Imaginary School - Main Menu - Vocabulary Training - A1"
-					)
-				},
-				"option_1": {
-					"A2": lambda: fufu1(
-						"Imaginary School - Main Menu - Vocabulary Training - A2"
-					)
-				},
-				"option_2": {
-					"B1-B2": lambda: fufu1(
-						"Imaginary School - Main Menu - Vocabulary Training - B1-B2"
-					)
-				},
-				"option_3": {
-					"C1-C2": lambda: fufu1(
-						"Imaginary School - Main Menu - Vocabulary Training - C1-C2"
-					)
-				},
-				"option_4": {
-					"Training for Tests": {
-						"menu_header": "Specific Test Training",
-						"option_0": {
-							"Sub Option 0": lambda: fufu1(
-								"Imaginary School - Main Menu - Vocabulary Training - Suboption 0"
-							)
-						},
-						"option_1": {
-							"Sub Option 1": lambda: fufu1(
-								"Imaginary School - Main Menu - Vocabulary Training - Suboption 1"
-							)
-						},
-						"option_2": {
-							"Sub Option 2": lambda: fufu1(
-								"Imaginary School - Main Menu - Vocabulary Training - SubOption 2"
-							)
-						},
-						"option_3": {
-							"Sub Option 3": lambda: fufu1(
-								"Imaginary School - Main Menu - Vocabulary Training - Suboption 3"
-							)
-						},
-						"option_4": {
-							"Sub Option 4": lambda: fufu1(
-								"Imaginary School - Main Menu - Vocabulary Training - Suboption 4"
-							)
-						},
-						"option_5": {
-							"Go back": ("main", "option_4", "Vocabulary Training")
-						},
-					},
-				},
-				"option_5": {"Go back": ("main",)},
-			},
-		},
-	}
+    "main": {
+        "menu_header": "Imaginary School - Main Menu",
+        "option_0": {
+            "Exercises": lambda: fufu1("Imaginary School - Main Menu - Exercises")
+        },
+        "option_1": {"Review": lambda: fufu1("Imaginary School - Main Menu - Review")},
+        "option_2": {
+            "Talk to a teacher": lambda: fufu1(
+                "Imaginary School - Main Menu - Talk to a teacher"
+            )
+        },
+        "option_3": {
+            "Blackboard": lambda: fufu1("Imaginary School - Main Menu - Blackboard")
+        },
+        "option_4": {
+            "Vocabulary Training": {
+                "menu_header": "Welcome to the Vocabulary Training section:",
+                "option_0": {
+                    "A1": lambda: fufu1(
+                        "Imaginary School - Main Menu - Vocabulary Training - A1"
+                    )
+                },
+                "option_1": {
+                    "A2": lambda: fufu1(
+                        "Imaginary School - Main Menu - Vocabulary Training - A2"
+                    )
+                },
+                "option_2": {
+                    "B1-B2": lambda: fufu1(
+                        "Imaginary School - Main Menu - Vocabulary Training - B1-B2"
+                    )
+                },
+                "option_3": {
+                    "C1-C2": lambda: fufu1(
+                        "Imaginary School - Main Menu - Vocabulary Training - C1-C2"
+                    )
+                },
+                "option_4": {
+                    "Training for Tests": {
+                        "menu_header": "Specific Test Training",
+                        "option_0": {
+                            "Sub Option 0": lambda: fufu1(
+                                "Imaginary School - Main Menu - Vocabulary Training - Suboption 0"
+                            )
+                        },
+                        "option_1": {
+                            "Sub Option 1": lambda: fufu1(
+                                "Imaginary School - Main Menu - Vocabulary Training - Suboption 1"
+                            )
+                        },
+                        "option_2": {
+                            "Sub Option 2": lambda: fufu1(
+                                "Imaginary School - Main Menu - Vocabulary Training - SubOption 2"
+                            )
+                        },
+                        "option_3": {
+                            "Sub Option 3": lambda: fufu1(
+                                "Imaginary School - Main Menu - Vocabulary Training - Suboption 3"
+                            )
+                        },
+                        "option_4": {
+                            "Sub Option 4": lambda: fufu1(
+                                "Imaginary School - Main Menu - Vocabulary Training - Suboption 4"
+                            )
+                        },
+                        "option_5": {
+                            "Go back": ("main", "option_4", "Vocabulary Training")
+                        },
+                    },
+                },
+                "option_5": {"Go back": ("main",)},
+            },
+        },
+    }
 }
 start_menu(stama)
 
+
 ```
```

### Comparing `cursesdict-0.11/cursesdict/__init__.py` & `cursesdict-0.12/cursesdict/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 menu_config.use_rjust = True
 menu_config.refresh_sleep = 0.001
 menu_config.quit_keys = [""]
 menu_config.enter_keys = ["PADENTER"]
 menu_config.key_up_keys = ["KEY_UP"]
 menu_config.key_down_keys = ["KEY_DOWN"]
 menu_config.menudict = {}
-
+menu_config.is_active = True
 
 # https://www.lfd.uci.edu/~gohlke/pythonlibs/#curses
 
 
 def start_menu(
     menudict: dict,
     menu_len: int = 40,
@@ -60,102 +60,106 @@
             key_up_keys (tuple or list, optional): Keys to navigate up in the menu. Defaults to ("KEY_UP",).
             key_down_keys (tuple or list, optional): Keys to navigate down in the menu. Defaults to ("KEY_DOWN",).
 
         Returns:
             None
 
         Example:
-    import subprocess
-    from cursesdict import start_menu
+import subprocess
 
-    def fufu1(key):
-        filetest = "c:\\testestestest.txt"
-        with open(filetest, mode="w", encoding="utf-8") as f:
-            f.write(str(key))
-            f.write("\n")
-        subprocess.Popen(f"notepad.exe {filetest}", shell=True)
-
-
-    stama = {
-        "main": {
-            "menu_header": "Imaginary School - Main Menu",
-            "option_0": {
-                "Exercises": lambda: fufu1("Imaginary School - Main Menu - Exercises")
-            },
-            "option_1": {"Review": lambda: fufu1("Imaginary School - Main Menu - Review")},
-            "option_2": {
-                "Talk to a teacher": lambda: fufu1(
-                    "Imaginary School - Main Menu - Talk to a teacher"
-                )
-            },
-            "option_3": {
-                "Blackboard": lambda: fufu1("Imaginary School - Main Menu - Blackboard")
-            },
-            "option_4": {
-                "Vocabulary Training": {
-                    "menu_header": "Welcome to the Vocabulary Training section:",
-                    "option_0": {
-                        "A1": lambda: fufu1(
-                            "Imaginary School - Main Menu - Vocabulary Training - A1"
-                        )
-                    },
-                    "option_1": {
-                        "A2": lambda: fufu1(
-                            "Imaginary School - Main Menu - Vocabulary Training - A2"
-                        )
-                    },
-                    "option_2": {
-                        "B1-B2": lambda: fufu1(
-                            "Imaginary School - Main Menu - Vocabulary Training - B1-B2"
-                        )
-                    },
-                    "option_3": {
-                        "C1-C2": lambda: fufu1(
-                            "Imaginary School - Main Menu - Vocabulary Training - C1-C2"
-                        )
-                    },
-                    "option_4": {
-                        "Training for Tests": {
-                            "menu_header": "Specific Test Training",
-                            "option_0": {
-                                "Sub Option 0": lambda: fufu1(
-                                    "Imaginary School - Main Menu - Vocabulary Training - Suboption 0"
-                                )
-                            },
-                            "option_1": {
-                                "Sub Option 1": lambda: fufu1(
-                                    "Imaginary School - Main Menu - Vocabulary Training - Suboption 1"
-                                )
-                            },
-                            "option_2": {
-                                "Sub Option 2": lambda: fufu1(
-                                    "Imaginary School - Main Menu - Vocabulary Training - SubOption 2"
-                                )
-                            },
-                            "option_3": {
-                                "Sub Option 3": lambda: fufu1(
-                                    "Imaginary School - Main Menu - Vocabulary Training - Suboption 3"
-                                )
-                            },
-                            "option_4": {
-                                "Sub Option 4": lambda: fufu1(
-                                    "Imaginary School - Main Menu - Vocabulary Training - Suboption 4"
-                                )
-                            },
-                            "option_5": {
-                                "Go back": ("main", "option_4", "Vocabulary Training")
-                            },
+from cursesdict import start_menu, menu_config
+
+
+def fufu1(key):
+    filetest = "c:\\testestestest.txt"
+    with open(filetest, mode="w", encoding="utf-8") as f:
+        f.write(str(key))
+        f.write("\n")
+    subprocess.Popen(f"notepad.exe {filetest}", shell=True)
+    menu_config.is_active = False  # exits the menu
+
+
+stama = {
+    "main": {
+        "menu_header": "Imaginary School - Main Menu",
+        "option_0": {
+            "Exercises": lambda: fufu1("Imaginary School - Main Menu - Exercises")
+        },
+        "option_1": {"Review": lambda: fufu1("Imaginary School - Main Menu - Review")},
+        "option_2": {
+            "Talk to a teacher": lambda: fufu1(
+                "Imaginary School - Main Menu - Talk to a teacher"
+            )
+        },
+        "option_3": {
+            "Blackboard": lambda: fufu1("Imaginary School - Main Menu - Blackboard")
+        },
+        "option_4": {
+            "Vocabulary Training": {
+                "menu_header": "Welcome to the Vocabulary Training section:",
+                "option_0": {
+                    "A1": lambda: fufu1(
+                        "Imaginary School - Main Menu - Vocabulary Training - A1"
+                    )
+                },
+                "option_1": {
+                    "A2": lambda: fufu1(
+                        "Imaginary School - Main Menu - Vocabulary Training - A2"
+                    )
+                },
+                "option_2": {
+                    "B1-B2": lambda: fufu1(
+                        "Imaginary School - Main Menu - Vocabulary Training - B1-B2"
+                    )
+                },
+                "option_3": {
+                    "C1-C2": lambda: fufu1(
+                        "Imaginary School - Main Menu - Vocabulary Training - C1-C2"
+                    )
+                },
+                "option_4": {
+                    "Training for Tests": {
+                        "menu_header": "Specific Test Training",
+                        "option_0": {
+                            "Sub Option 0": lambda: fufu1(
+                                "Imaginary School - Main Menu - Vocabulary Training - Suboption 0"
+                            )
+                        },
+                        "option_1": {
+                            "Sub Option 1": lambda: fufu1(
+                                "Imaginary School - Main Menu - Vocabulary Training - Suboption 1"
+                            )
+                        },
+                        "option_2": {
+                            "Sub Option 2": lambda: fufu1(
+                                "Imaginary School - Main Menu - Vocabulary Training - SubOption 2"
+                            )
+                        },
+                        "option_3": {
+                            "Sub Option 3": lambda: fufu1(
+                                "Imaginary School - Main Menu - Vocabulary Training - Suboption 3"
+                            )
+                        },
+                        "option_4": {
+                            "Sub Option 4": lambda: fufu1(
+                                "Imaginary School - Main Menu - Vocabulary Training - Suboption 4"
+                            )
+                        },
+                        "option_5": {
+                            "Go back": ("main", "option_4", "Vocabulary Training")
                         },
                     },
-                    "option_5": {"Go back": ("main",)},
                 },
+                "option_5": {"Go back": ("main",)},
             },
-        }
+        },
     }
-    start_menu(stama)
+}
+start_menu(stama)
+
 
     """
     menu_config.menulen = menu_len
     menu_config.add_spaces_right = n_spaces_right
     menu_config.add_spaces_left = n_spaces_left
     menu_config.menulen_highlighted = menu_len_selected
     menu_config.add_spaces_right_highlighted = n_spaces_right_selected
@@ -263,15 +267,15 @@
     juststring = rjust if menu_config.use_rjust else ljust
     active_choices = get_active_dict(menu_config.menudict, ["main"])
     active_menu_choices = get_active_menu_items(active_choices)
     print_menu(
         header=active_choices["menu_header"], all_menu_choices=active_menu_choices
     )
 
-    while True:
+    while menu_config.is_active:
         print_menu(
             header=active_choices["menu_header"], all_menu_choices=active_menu_choices
         )
 
         key = stdscr.getkey()
 
         if key in menu_config.quit_keys:
@@ -290,8 +294,9 @@
                 active_choices = get_active_dict(menu_config.menudict, fu)
                 active_menu_choices = get_active_menu_items(active_choices)
                 current_choice = 0
         if key in menu_config.key_down_keys:
             current_choice = (current_choice + 1) % len(active_menu_choices)
         elif key == menu_config.key_up_keys:
             current_choice = (current_choice - 1) % len(active_menu_choices)
+    break_window()
     curses.endwin()
```

### Comparing `cursesdict-0.11/cursesdict/thirdparty.json` & `cursesdict-0.12/cursesdict/thirdparty.json`

 * *Files identical despite different names*

### Comparing `cursesdict-0.11/setup.py` & `cursesdict-0.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.11'''
+VERSION = '''0.12'''
 DESCRIPTION = '''creates an interactive menu system for your application or program, providing an intuitive and user-friendly interface for users to navigate and perform various actions'''
 
 # Setting up
 setup(
     name="cursesdict",
     version=VERSION,
     license='MIT',
```

