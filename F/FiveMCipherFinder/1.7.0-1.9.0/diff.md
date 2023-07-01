# Comparing `tmp/FiveMCipherFinder-1.7.0.tar.gz` & `tmp/FiveMCipherFinder-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FiveMCipherFinder-1.7.0.tar", last modified: Wed Jun 28 12:33:48 2023, max compression
+gzip compressed data, was "FiveMCipherFinder-1.9.0.tar", last modified: Sat Jul  1 08:07:27 2023, max compression
```

## Comparing `FiveMCipherFinder-1.7.0.tar` & `FiveMCipherFinder-1.9.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:33:48.198967 FiveMCipherFinder-1.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:33:48.198967 FiveMCipherFinder-1.7.0/FiveMCipherFinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-28 12:33:48.000000 FiveMCipherFinder-1.7.0/FiveMCipherFinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-28 12:33:48.000000 FiveMCipherFinder-1.7.0/FiveMCipherFinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 12:33:48.000000 FiveMCipherFinder-1.7.0/FiveMCipherFinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-28 12:33:48.000000 FiveMCipherFinder-1.7.0/FiveMCipherFinder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-28 12:33:48.000000 FiveMCipherFinder-1.7.0/FiveMCipherFinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-28 12:33:38.000000 FiveMCipherFinder-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-28 12:33:48.198967 FiveMCipherFinder-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-28 12:33:38.000000 FiveMCipherFinder-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:33:48.198967 FiveMCipherFinder-1.7.0/cipherFinder/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-28 12:33:38.000000 FiveMCipherFinder-1.7.0/cipherFinder/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5319 2023-06-28 12:33:38.000000 FiveMCipherFinder-1.7.0/cipherFinder/finder.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-28 12:33:38.000000 FiveMCipherFinder-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-28 12:33:48.198967 FiveMCipherFinder-1.7.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-06-28 12:33:38.000000 FiveMCipherFinder-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:07:27.759294 FiveMCipherFinder-1.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:07:27.759294 FiveMCipherFinder-1.9.0/FiveMCipherFinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-01 08:07:27.000000 FiveMCipherFinder-1.9.0/FiveMCipherFinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-01 08:07:27.000000 FiveMCipherFinder-1.9.0/FiveMCipherFinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 08:07:27.000000 FiveMCipherFinder-1.9.0/FiveMCipherFinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-01 08:07:27.000000 FiveMCipherFinder-1.9.0/FiveMCipherFinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-01 08:07:27.000000 FiveMCipherFinder-1.9.0/FiveMCipherFinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-01 08:07:14.000000 FiveMCipherFinder-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-01 08:07:27.759294 FiveMCipherFinder-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-01 08:07:14.000000 FiveMCipherFinder-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:07:27.759294 FiveMCipherFinder-1.9.0/cipherFinder/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-01 08:07:14.000000 FiveMCipherFinder-1.9.0/cipherFinder/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6190 2023-07-01 08:07:14.000000 FiveMCipherFinder-1.9.0/cipherFinder/finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-01 08:07:14.000000 FiveMCipherFinder-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-01 08:07:27.759294 FiveMCipherFinder-1.9.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-07-01 08:07:14.000000 FiveMCipherFinder-1.9.0/setup.py
```

### Comparing `FiveMCipherFinder-1.7.0/FiveMCipherFinder.egg-info/PKG-INFO` & `FiveMCipherFinder-1.9.0/FiveMCipherFinder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: FiveMCipherFinder
-Version: 1.7.0
+Version: 1.9.0
 Summary: Finds Cipher in lua scripts.
 Home-page: https://github.com/exersalza/FivemCipherFinder
 Author: exersalza
 License: MIT
 Project-URL: Source, https://github.com/exersalza/FivemCipherFinder
 Project-URL: Issues, https://github.com/exersalza/FivemCipherFinder/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# FivemCipherFinder (v1.7.0)
+# FivemCipherFinder (v1.9.0)
 <div align="center">
   <h2> Visitors </h2>
 <img src="https://profile-counter.glitch.me/FivemCipherFinder/count.svg" />
 </div>
 
 [![Pylint](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml/badge.svg)](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml)
```

### Comparing `FiveMCipherFinder-1.7.0/LICENSE` & `FiveMCipherFinder-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FiveMCipherFinder-1.7.0/PKG-INFO` & `FiveMCipherFinder-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: FiveMCipherFinder
-Version: 1.7.0
+Version: 1.9.0
 Summary: Finds Cipher in lua scripts.
 Home-page: https://github.com/exersalza/FivemCipherFinder
 Author: exersalza
 License: MIT
 Project-URL: Source, https://github.com/exersalza/FivemCipherFinder
 Project-URL: Issues, https://github.com/exersalza/FivemCipherFinder/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# FivemCipherFinder (v1.7.0)
+# FivemCipherFinder (v1.9.0)
 <div align="center">
   <h2> Visitors </h2>
 <img src="https://profile-counter.glitch.me/FivemCipherFinder/count.svg" />
 </div>
 
 [![Pylint](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml/badge.svg)](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml)
```

### Comparing `FiveMCipherFinder-1.7.0/README.md` & `FiveMCipherFinder-1.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# FivemCipherFinder (v1.7.0)
+# FivemCipherFinder (v1.9.0)
 <div align="center">
   <h2> Visitors </h2>
 <img src="https://profile-counter.glitch.me/FivemCipherFinder/count.svg" />
 </div>
 
 [![Pylint](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml/badge.svg)](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml)
```

### Comparing `FiveMCipherFinder-1.7.0/cipherFinder/finder.py` & `FiveMCipherFinder-1.9.0/cipherFinder/finder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/bin/python3.11
 
-#  Copyright (c) 2022. - exersalza
+#  Copyright (c) 2022-2023 - exersalza
 #
 #  Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
 #  furnished to do so, subject to the following conditions:
@@ -29,19 +29,18 @@
 from datetime import datetime as dt
 from gibberish_detector import detector
 
 REGEX = r'(((\\x|\\u)([a-fA-F0-9]{2})){2})'
 COLORS = ['\033[0m', '\033[91m', '\033[92m']
 
 det = detector.create_from_model('big.model')
-
 log = []
 
 
-def validate_lines(lines) -> list[tuple]:
+def validate_lines(lines: list) -> list[tuple]:
     """ Validate the lines that are given through the 'lines' parameter.
 
     Parameters
     ----------
     lines : list
         The lines from the current read file.
 
@@ -57,15 +56,15 @@
     for ln, line in enumerate(lines, start=1):  # ln: lineNumber
         if re.findall(REGEX, rf'{line}', re.MULTILINE and re.IGNORECASE):
             ret.append((ln, line))
 
     return ret
 
 
-def do_gibberish_check(lines) -> list[tuple[str, int]]:
+def do_gibberish_check(lines: list) -> list[tuple[str, int]]:
     """ Do a check if the given lines are making any sens.
     Can still throw false-positives
 
     Parameters
     ----------
     lines : list
         The lines from the current read file.
@@ -84,15 +83,32 @@
         if 'local' in i and det.is_gibberish(rf'{i}'):
             matches.append((l_counter, i))
 
         l_counter += 1
     return matches
 
 
-def check_file(d, file, count) -> tuple[int, int]: 
+def check_file(d: str, file: str, count: int) -> tuple[int, int]: 
+    """ Iterate over a file and check the lines
+
+    Parameters
+    ----------
+    d : str
+        Give the path to the file e.g "/home/wildCiphers"
+    file : str
+        Give a file name to scan e.g "wildCipherInHere.lua"
+    count: int
+        Give the current cipher count.
+    
+    Returns
+    -------
+    tuple[ret_code, count]
+        A Tuple with the return code and the current cipher count.
+    """
+
     with open(f'{d}/{file}', 'r', encoding='utf-8') as f:
         try:
             lines = f.readlines()
         except UnicodeDecodeError:
             print(f'Can\'t decode `{d}/{file}`.')
             return 1, count
         
@@ -110,40 +126,55 @@
                     print(to_log)
 
 
                 log.append(to_log + f'Line: {line!r}\n----------------\n')
                 count += 1
     return 0, count
 
+def write_log_file(**kw) -> int: 
+    with open(f'CipherLog-{dt.now():%H-%M-%S}.txt', 'w+', encoding='utf-8') as f:
+        f.writelines(log)
+        
+        print(f'{kw.pop("red")}Oh no, the program found a spy in your files x.x '
+          f'Check the CipherLog.txt for location and trigger. {kw.pop("count")} where found!'
+          f'{kw.pop("white")}\n#staysafe')
+    return 0
 
 def main() -> int:
     """ Validates lua files.
 
     Usage:
     ------
-    Run the program: `find-cipher <path> [exclude path] [--verbose]`.
+    Run the program: `find-cipher [path] [exclude path] [OPTIONS...]`.
 
     args:
-        path : Give the path to search, when no path is given, the current working directory will be used `.` .
-        exclude path : Optional : Exclude directory's where you don't want to search.
-        --verbose : Optional : Print a Cipher directly to the Command line on found.
-
+        path : Optional : 
+            Give the path to search, when no path is given, the 
+            current working directory will be used `.`
+        exclude path : Optional : 
+            Exclude directory's where you don't want to search.
+        --verbose : Optional : 
+            Print a Cipher directly to the Command line on found.
+        --v2 : Optional : 
+            Uses an extra algorithm to find gibberish or randomly generated
+            variable/function/table names. It can introduce more palse-positiv
+            because of obfuscated scripts, but can help to find ciphers.
 
     Advertisement:
     --------------
     Get your beautiful Cipher today, just smack the play button and find some.
     I hope you don't have any but always be sure to have none.
 
     Returns
     -------
     int
         Return code
     """
 
-    if '-h' in sys.argv:
+    if '-h' in sys.argv or '--help' in sys.argv:
         print(main.__doc__)
         return 0
 
     pattern = ''.join([(i.replace(',', ')|(') if '--' not in i else '') for i in sys.argv[2:]])
     local_path = '.'
     count = 0 
 
@@ -157,30 +188,22 @@
         for file in files:
             if '.lua' not in file:
                 continue
 
             _, count = check_file(d, file, count)
     # Write log
     
-    red = ''
-    green = ''
-    white = ''
+    red = green = white = ''
 
     if 'linux' in platform.platform().lower():
         white, red, green = COLORS
 
     if log:
-        with open(f'CipherLog-{dt.now():%H-%M-%S}.txt', 'w+', encoding='utf-8') as f:
-            f.writelines(log)
-        
-        print(f'{red}Oh no, the program found a spy in your files x.x '
-              f'Check the CipherLog.txt for location and trigger. {count} where found!'
-              f'{white}\n#staysafe')
-        return 0
-    
+        return write_log_file(white=white, red=red, count=count)
+
     print(f'{green}Nice! There were no Cipher\'s found!{white}')
 
     return 0
 
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `FiveMCipherFinder-1.7.0/setup.cfg` & `FiveMCipherFinder-1.9.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = FiveMCipherFinder
-version = 1.7.0
+version = 1.9.0
 description = Finds Cipher in lua scripts.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 author = exersalza
 url = https://github.com/exersalza/FivemCipherFinder
 project_urls =
```

