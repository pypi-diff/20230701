# Comparing `tmp/dotenv-cli-3.1.1.tar.gz` & `tmp/dotenv-cli-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotenv-cli-3.1.1.tar", last modified: Thu Apr 13 08:38:24 2023, max compression
+gzip compressed data, was "dotenv-cli-3.2.0.tar", last modified: Sat Jul  1 11:48:51 2023, max compression
```

## Comparing `dotenv-cli-3.1.1.tar` & `dotenv-cli-3.2.0.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-04-13 08:38:24.991097 dotenv-cli-3.1.1/
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1072 2018-10-14 16:13:37.000000 dotenv-cli-3.1.1/LICENSE
--rw-r--r--   0 venthur   (1000) venthur   (1000)       31 2019-04-28 11:56:54.000000 dotenv-cli-3.1.1/MANIFEST.in
--rw-r--r--   0 venthur   (1000) venthur   (1000)     2876 2023-04-13 08:38:24.991097 dotenv-cli-3.1.1/PKG-INFO
--rw-r--r--   0 venthur   (1000) venthur   (1000)     2347 2019-08-03 12:37:48.000000 dotenv-cli-3.1.1/README.md
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-04-13 08:38:24.987097 dotenv-cli-3.1.1/completion/
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-04-13 08:38:24.987097 dotenv-cli-3.1.1/completion/bash/
--rw-r--r--   0 venthur   (1000) venthur   (1000)      869 2019-04-28 11:56:54.000000 dotenv-cli-3.1.1/completion/bash/dotenv
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-04-13 08:38:24.991097 dotenv-cli-3.1.1/dotenv_cli/
--rw-r--r--   0 venthur   (1000) venthur   (1000)       65 2022-09-07 18:14:49.000000 dotenv-cli-3.1.1/dotenv_cli/__init__.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1162 2022-09-07 18:14:49.000000 dotenv-cli-3.1.1/dotenv_cli/cli.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)     2758 2022-09-07 18:14:49.000000 dotenv-cli-3.1.1/dotenv_cli/core.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)       22 2023-04-13 08:20:01.000000 dotenv-cli-3.1.1/dotenv_cli/version.py
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-04-13 08:38:24.991097 dotenv-cli-3.1.1/dotenv_cli.egg-info/
--rw-r--r--   0 venthur   (1000) venthur   (1000)     2876 2023-04-13 08:38:24.000000 dotenv-cli-3.1.1/dotenv_cli.egg-info/PKG-INFO
--rw-r--r--   0 venthur   (1000) venthur   (1000)      359 2023-04-13 08:38:24.000000 dotenv-cli-3.1.1/dotenv_cli.egg-info/SOURCES.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)        1 2023-04-13 08:38:24.000000 dotenv-cli-3.1.1/dotenv_cli.egg-info/dependency_links.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)       47 2023-04-13 08:38:24.000000 dotenv-cli-3.1.1/dotenv_cli.egg-info/entry_points.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)       44 2023-04-13 08:38:24.000000 dotenv-cli-3.1.1/dotenv_cli.egg-info/requires.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)       11 2023-04-13 08:38:24.000000 dotenv-cli-3.1.1/dotenv_cli.egg-info/top_level.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)      232 2023-04-13 08:38:24.991097 dotenv-cli-3.1.1/setup.cfg
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1076 2022-05-31 18:04:39.000000 dotenv-cli-3.1.1/setup.py
+drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-07-01 11:48:51.242150 dotenv-cli-3.2.0/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     1072 2018-10-14 16:13:37.000000 dotenv-cli-3.2.0/LICENSE
+-rw-r--r--   0 venthur   (1000) venthur   (1000)       31 2019-04-28 11:56:54.000000 dotenv-cli-3.2.0/MANIFEST.in
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     4204 2023-07-01 11:48:51.242150 dotenv-cli-3.2.0/PKG-INFO
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     2347 2019-08-03 12:37:48.000000 dotenv-cli-3.2.0/README.md
+drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-07-01 11:48:51.234150 dotenv-cli-3.2.0/completion/
+drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-07-01 11:48:51.238150 dotenv-cli-3.2.0/completion/bash/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      869 2019-04-28 11:56:54.000000 dotenv-cli-3.2.0/completion/bash/dotenv
+drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-07-01 11:48:51.238150 dotenv-cli-3.2.0/dotenv_cli/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)       66 2023-07-01 11:21:02.000000 dotenv-cli-3.2.0/dotenv_cli/__init__.py
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     1201 2023-07-01 11:21:02.000000 dotenv-cli-3.2.0/dotenv_cli/cli.py
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     3102 2023-07-01 11:21:02.000000 dotenv-cli-3.2.0/dotenv_cli/core.py
+-rw-r--r--   0 venthur   (1000) venthur   (1000)       22 2023-07-01 11:24:12.000000 dotenv-cli-3.2.0/dotenv_cli/version.py
+drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-07-01 11:48:51.238150 dotenv-cli-3.2.0/dotenv_cli.egg-info/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     4204 2023-07-01 11:48:51.000000 dotenv-cli-3.2.0/dotenv_cli.egg-info/PKG-INFO
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      414 2023-07-01 11:48:51.000000 dotenv-cli-3.2.0/dotenv_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 venthur   (1000) venthur   (1000)        1 2023-07-01 11:48:51.000000 dotenv-cli-3.2.0/dotenv_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 venthur   (1000) venthur   (1000)       47 2023-07-01 11:48:51.000000 dotenv-cli-3.2.0/dotenv_cli.egg-info/entry_points.txt
+-rw-r--r--   0 venthur   (1000) venthur   (1000)       49 2023-07-01 11:48:51.000000 dotenv-cli-3.2.0/dotenv_cli.egg-info/requires.txt
+-rw-r--r--   0 venthur   (1000) venthur   (1000)       11 2023-07-01 11:48:51.000000 dotenv-cli-3.2.0/dotenv_cli.egg-info/top_level.txt
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     1210 2023-07-01 11:21:02.000000 dotenv-cli-3.2.0/pyproject.toml
+-rw-r--r--   0 venthur   (1000) venthur   (1000)       38 2023-07-01 11:48:51.242150 dotenv-cli-3.2.0/setup.cfg
+drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-07-01 11:48:51.238150 dotenv-cli-3.2.0/tests/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     1499 2023-07-01 11:21:02.000000 dotenv-cli-3.2.0/tests/test_cli.py
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     3951 2023-07-01 11:21:02.000000 dotenv-cli-3.2.0/tests/test_core.py
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      108 2023-07-01 11:21:02.000000 dotenv-cli-3.2.0/tests/test_version.py
```

### Comparing `dotenv-cli-3.1.1/LICENSE` & `dotenv-cli-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dotenv-cli-3.1.1/PKG-INFO` & `dotenv-cli-3.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,42 @@
 Metadata-Version: 2.1
 Name: dotenv-cli
-Version: 3.1.1
+Version: 3.2.0
 Summary: Simple dotenv CLI.
-Home-page: https://github.com/venthur/dotenv-cli
-Author: Bastian Venthur
-Author-email: mail@venthur.de
-License: MIT
-Keywords: dotenv cli .env
+Author-email: Bastian Venthur <mail@venthur.de>
+License: MIT License
+        
+        Copyright (c) 2018 Bastian Venthur
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Source, https://github.com/venthur/dotenv-cli
+Project-URL: Changelog, https://github.com/venthur/dotenv-cli/blob/master/CHANGELOG.md
+Keywords: dotenv,cli,.env
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # dotenv CLI
 
 Dotenv-CLI is a simple package that provides the `dotenv` command. It reads the
```

### Comparing `dotenv-cli-3.1.1/README.md` & `dotenv-cli-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dotenv-cli-3.1.1/completion/bash/dotenv` & `dotenv-cli-3.2.0/completion/bash/dotenv`

 * *Files identical despite different names*

### Comparing `dotenv-cli-3.1.1/dotenv_cli/core.py` & `dotenv-cli-3.2.0/dotenv_cli/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # remove when we don't support py38 anymore
 from __future__ import annotations
+
 import atexit
 import logging
 import os
-from subprocess import Popen  # , PIPE, STDOUT
-
+from subprocess import Popen
+from typing import NoReturn
 
 logger = logging.getLogger(__name__)
 
 
 def read_dotenv(filename: str) -> dict[str, str]:
     """Read dotenv file.
 
@@ -19,84 +20,93 @@
 
     Returns
     -------
     dict
 
     """
     try:
-        with open(filename, 'r') as fh:
+        with open(filename, "r") as fh:
             data = fh.read()
     except FileNotFoundError:
-        logger.warning(f"{filename} does not exist, continuing without "
-                       "setting environment variables.")
+        logger.warning(
+            f"{filename} does not exist, continuing without "
+            "setting environment variables."
+        )
         data = ""
 
     res = {}
     for line in data.splitlines():
         logger.debug(line)
 
         line = line.strip()
 
         # ignore comments
-        if line.startswith('#'):
+        if line.startswith("#"):
             continue
 
         # ignore empty lines or lines w/o '='
-        if '=' not in line:
+        if "=" not in line:
             continue
 
-        key, value = line.split('=', 1)
+        key, value = line.split("=", 1)
 
         # allow export
-        if key.startswith('export '):
-            key = key.split(' ', 1)[-1]
+        if key.startswith("export "):
+            key = key.split(" ", 1)[-1]
 
         key = key.strip()
         value = value.strip()
 
         # remove quotes (not sure if this is standard behaviour)
         if len(value) >= 2 and value[0] == value[-1] == '"':
             value = value[1:-1]
             # escape escape characters
-            value = bytes(value, 'utf-8').decode('unicode-escape')
+            value = bytes(value, "utf-8").decode("unicode-escape")
 
         elif len(value) >= 2 and value[0] == value[-1] == "'":
             value = value[1:-1]
 
         res[key] = value
     logger.debug(res)
     return res
 
 
-def run_dotenv(filename: str, command: list[str]) -> int:
+def run_dotenv(filename: str, command: list[str]) -> NoReturn | int:
     """Run dotenv.
 
     This function executes the commands with the environment variables
     parsed from filename.
 
     Parameters
     ----------
     filename
         path to the .env file
     command
         command to execute
 
     Returns
     -------
-    int
-        the return value
+    NoReturn | int
+        The exit status code in Windows. In POSIX-compatible systems, the
+        function does not return normally.
 
     """
     # read dotenv
     dotenv = read_dotenv(filename)
 
     # update env
     env = os.environ.copy()
     env.update(dotenv)
 
+    # in POSIX, we replace the current process with the command, execvpe does
+    # not return
+    if os.name == "posix":
+        os.execvpe(command[0], command, env)
+
+    # in Windows, we spawn a new process
     # execute
     proc = Popen(
         command,
         # stdin=PIPE,
         # stdout=PIPE,
         # stderr=STDOUT,
         universal_newlines=True,
```

### Comparing `dotenv-cli-3.1.1/dotenv_cli.egg-info/PKG-INFO` & `dotenv-cli-3.2.0/dotenv_cli.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,42 @@
 Metadata-Version: 2.1
 Name: dotenv-cli
-Version: 3.1.1
+Version: 3.2.0
 Summary: Simple dotenv CLI.
-Home-page: https://github.com/venthur/dotenv-cli
-Author: Bastian Venthur
-Author-email: mail@venthur.de
-License: MIT
-Keywords: dotenv cli .env
+Author-email: Bastian Venthur <mail@venthur.de>
+License: MIT License
+        
+        Copyright (c) 2018 Bastian Venthur
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Source, https://github.com/venthur/dotenv-cli
+Project-URL: Changelog, https://github.com/venthur/dotenv-cli/blob/master/CHANGELOG.md
+Keywords: dotenv,cli,.env
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # dotenv CLI
 
 Dotenv-CLI is a simple package that provides the `dotenv` command. It reads the
```

