# Comparing `tmp/cursesdict-0.10.tar.gz` & `tmp/cursesdict-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cursesdict-0.10.tar", last modified: Sat Jul  1 05:47:57 2023, max compression
+gzip compressed data, was "cursesdict-0.11.tar", last modified: Sat Jul  1 05:53:05 2023, max compression
```

## Comparing `cursesdict-0.10.tar` & `cursesdict-0.11.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 05:47:57.827172 cursesdict-0.10/
--rw-rw-rw-   0        0        0     1148 2023-07-01 05:47:52.000000 cursesdict-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      101 2023-07-01 05:47:51.000000 cursesdict-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     7737 2023-07-01 05:47:57.827172 cursesdict-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     6999 2023-07-01 05:44:51.000000 cursesdict-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 05:47:57.824180 cursesdict-0.10/cursesdict/
--rw-rw-rw-   0        0        0     6999 2023-07-01 05:44:51.000000 cursesdict-0.10/cursesdict/README.MD
--rw-rw-rw-   0        0        0    11645 2023-07-01 05:42:08.000000 cursesdict-0.10/cursesdict/__init__.py
--rw-rw-rw-   0        0        0       18 2023-07-01 05:47:56.000000 cursesdict-0.10/cursesdict/requirements.txt
--rw-rw-rw-   0        0        0     1256 2023-07-01 05:47:56.000000 cursesdict-0.10/cursesdict/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-07-01 05:47:57.826175 cursesdict-0.10/cursesdict.egg-info/
--rw-rw-rw-   0        0        0     7737 2023-07-01 05:47:57.000000 cursesdict-0.10/cursesdict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-01 05:47:57.000000 cursesdict-0.10/cursesdict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 05:47:57.000000 cursesdict-0.10/cursesdict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-01 05:47:57.000000 cursesdict-0.10/cursesdict.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-01 05:47:57.000000 cursesdict-0.10/cursesdict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-07-01 05:47:57.828169 cursesdict-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1414 2023-07-01 05:47:56.000000 cursesdict-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 05:53:05.024044 cursesdict-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-07-01 05:52:57.000000 cursesdict-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      101 2023-07-01 05:52:54.000000 cursesdict-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     7734 2023-07-01 05:53:05.024044 cursesdict-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     6996 2023-07-01 05:52:39.000000 cursesdict-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 05:53:05.021052 cursesdict-0.11/cursesdict/
+-rw-rw-rw-   0        0        0     6996 2023-07-01 05:52:39.000000 cursesdict-0.11/cursesdict/README.MD
+-rw-rw-rw-   0        0        0    11645 2023-07-01 05:42:08.000000 cursesdict-0.11/cursesdict/__init__.py
+-rw-rw-rw-   0        0        0       18 2023-07-01 05:53:04.000000 cursesdict-0.11/cursesdict/requirements.txt
+-rw-rw-rw-   0        0        0     1256 2023-07-01 05:53:04.000000 cursesdict-0.11/cursesdict/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-07-01 05:53:05.024044 cursesdict-0.11/cursesdict.egg-info/
+-rw-rw-rw-   0        0        0     7734 2023-07-01 05:53:04.000000 cursesdict-0.11/cursesdict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-01 05:53:04.000000 cursesdict-0.11/cursesdict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 05:53:04.000000 cursesdict-0.11/cursesdict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-01 05:53:04.000000 cursesdict-0.11/cursesdict.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-01 05:53:04.000000 cursesdict-0.11/cursesdict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-07-01 05:53:05.025041 cursesdict-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1414 2023-07-01 05:53:04.000000 cursesdict-0.11/setup.py
```

### Comparing `cursesdict-0.10/LICENSE.rst` & `cursesdict-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `cursesdict-0.10/PKG-INFO` & `cursesdict-0.11/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesdict
-Version: 0.10
+Version: 0.11
 Summary: creates an interactive menu system for your application or program, providing an intuitive and user-friendly interface for users to navigate and perform various actions
 Home-page: https://github.com/hansalemaos/cursesdict
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: curses,menu
 Classifier: Development Status :: 4 - Beta
@@ -14,15 +14,15 @@
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
 
 # creates an interactive menu system for your application or program, providing an intuitive and user-friendly interface for users to navigate and perform various actions
 
-## pip install ffmpegdevices
+## pip install cursesdict
 
 #### Tested against Windows 10 / Python 3.10 / Anaconda 
 #### curses from https://www.lfd.uci.edu/~gohlke/pythonlibs/#curses
 
 
 ### Simplifies menu creation:
```

### Comparing `cursesdict-0.10/README.md` & `cursesdict-0.11/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # creates an interactive menu system for your application or program, providing an intuitive and user-friendly interface for users to navigate and perform various actions
 
-## pip install ffmpegdevices
+## pip install cursesdict
 
 #### Tested against Windows 10 / Python 3.10 / Anaconda 
 #### curses from https://www.lfd.uci.edu/~gohlke/pythonlibs/#curses
 
 
 ### Simplifies menu creation:
```

### Comparing `cursesdict-0.10/cursesdict/README.MD` & `cursesdict-0.11/cursesdict/README.MD`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # creates an interactive menu system for your application or program, providing an intuitive and user-friendly interface for users to navigate and perform various actions
 
-## pip install ffmpegdevices
+## pip install cursesdict
 
 #### Tested against Windows 10 / Python 3.10 / Anaconda 
 #### curses from https://www.lfd.uci.edu/~gohlke/pythonlibs/#curses
 
 
 ### Simplifies menu creation:
```

### Comparing `cursesdict-0.10/cursesdict/__init__.py` & `cursesdict-0.11/cursesdict/__init__.py`

 * *Files identical despite different names*

### Comparing `cursesdict-0.10/cursesdict/thirdparty.json` & `cursesdict-0.11/cursesdict/thirdparty.json`

 * *Files identical despite different names*

### Comparing `cursesdict-0.10/cursesdict.egg-info/PKG-INFO` & `cursesdict-0.11/cursesdict.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesdict
-Version: 0.10
+Version: 0.11
 Summary: creates an interactive menu system for your application or program, providing an intuitive and user-friendly interface for users to navigate and perform various actions
 Home-page: https://github.com/hansalemaos/cursesdict
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: curses,menu
 Classifier: Development Status :: 4 - Beta
@@ -14,15 +14,15 @@
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
 
 # creates an interactive menu system for your application or program, providing an intuitive and user-friendly interface for users to navigate and perform various actions
 
-## pip install ffmpegdevices
+## pip install cursesdict
 
 #### Tested against Windows 10 / Python 3.10 / Anaconda 
 #### curses from https://www.lfd.uci.edu/~gohlke/pythonlibs/#curses
 
 
 ### Simplifies menu creation:
```

### Comparing `cursesdict-0.10/setup.py` & `cursesdict-0.11/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''creates an interactive menu system for your application or program, providing an intuitive and user-friendly interface for users to navigate and perform various actions'''
 
 # Setting up
 setup(
     name="cursesdict",
     version=VERSION,
     license='MIT',
```

