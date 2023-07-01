# Comparing `tmp/spin-0.3.tar.gz` & `tmp/spin-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spin-0.3.tar", last modified: Thu Mar 23 20:45:23 2023, max compression
+gzip compressed data, was "spin-0.4.tar", last modified: Sat Jul  1 17:07:49 2023, max compression
```

## Comparing `spin-0.3.tar` & `spin-0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-03-23 20:45:23.513299 spin-0.3/
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)     1539 2023-03-17 22:23:55.000000 spin-0.3/LICENSE
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)     2173 2023-03-23 20:45:23.513299 spin-0.3/PKG-INFO
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)     4299 2023-03-23 16:34:01.000000 spin-0.3/README.md
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)      770 2023-03-23 20:43:28.000000 spin-0.3/pyproject.toml
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)       38 2023-03-23 20:45:23.513299 spin-0.3/setup.cfg
-drwxrwxr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-03-23 20:45:23.510299 spin-0.3/spin/
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)      192 2023-03-17 22:23:55.000000 spin-0.3/spin/__init__.py
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)     4009 2023-03-22 22:02:37.000000 spin-0.3/spin/__main__.py
-drwxrwxr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-03-23 20:45:23.512299 spin-0.3/spin/cmds/
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)      170 2023-03-17 22:23:55.000000 spin-0.3/spin/cmds/__init__.py
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)      174 2023-03-17 22:23:55.000000 spin-0.3/spin/cmds/build.py
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)     7624 2023-03-23 16:20:44.000000 spin-0.3/spin/cmds/meson.py
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)     2197 2023-03-17 22:23:55.000000 spin-0.3/spin/cmds/util.py
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)     1777 2023-03-17 22:23:55.000000 spin-0.3/spin/color_format.py
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)      696 2023-03-17 22:23:55.000000 spin-0.3/spin/sectioned_help.py
-drwxrwxr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-03-23 20:45:23.512299 spin-0.3/spin/tests/
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)     3428 2023-03-17 22:23:55.000000 spin-0.3/spin/tests/test_meson.py
-drwxrwxr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-03-23 20:45:23.511299 spin-0.3/spin.egg-info/
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)     2173 2023-03-23 20:45:23.000000 spin-0.3/spin.egg-info/PKG-INFO
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)      383 2023-03-23 20:45:23.000000 spin-0.3/spin.egg-info/SOURCES.txt
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)        1 2023-03-23 20:45:23.000000 spin-0.3/spin.egg-info/dependency_links.txt
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)       44 2023-03-23 20:45:23.000000 spin-0.3/spin.egg-info/entry_points.txt
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)       77 2023-03-23 20:45:23.000000 spin-0.3/spin.egg-info/requires.txt
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)        5 2023-03-23 20:45:23.000000 spin-0.3/spin.egg-info/top_level.txt
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-01 17:07:49.962760 spin-0.4/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1539 2023-05-22 22:53:56.000000 spin-0.4/LICENSE
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2173 2023-07-01 17:07:49.962760 spin-0.4/PKG-INFO
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     4318 2023-07-01 09:51:09.000000 spin-0.4/README.md
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      943 2023-07-01 17:01:45.000000 spin-0.4/pyproject.toml
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       38 2023-07-01 17:07:49.962760 spin-0.4/setup.cfg
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-01 17:07:49.958760 spin-0.4/spin/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      212 2023-07-01 16:31:53.000000 spin-0.4/spin/__init__.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     4302 2023-07-01 16:31:53.000000 spin-0.4/spin/__main__.py
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-01 17:07:49.961760 spin-0.4/spin/cmds/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      170 2023-05-22 22:53:56.000000 spin-0.4/spin/cmds/__init__.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      173 2023-07-01 09:51:09.000000 spin-0.4/spin/cmds/build.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)    12537 2023-07-01 16:56:23.000000 spin-0.4/spin/cmds/meson.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2246 2023-07-01 16:31:53.000000 spin-0.4/spin/cmds/util.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1777 2023-05-22 22:53:56.000000 spin-0.4/spin/color_format.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      697 2023-07-01 16:31:53.000000 spin-0.4/spin/sectioned_help.py
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-01 17:07:49.961760 spin-0.4/spin/tests/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     3445 2023-07-01 16:31:53.000000 spin-0.4/spin/tests/test_meson.py
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-01 17:07:49.960760 spin-0.4/spin.egg-info/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2173 2023-07-01 17:07:49.000000 spin-0.4/spin.egg-info/PKG-INFO
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      383 2023-07-01 17:07:49.000000 spin-0.4/spin.egg-info/SOURCES.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)        1 2023-07-01 17:07:49.000000 spin-0.4/spin.egg-info/dependency_links.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       44 2023-07-01 17:07:49.000000 spin-0.4/spin.egg-info/entry_points.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       77 2023-07-01 17:07:49.000000 spin-0.4/spin.egg-info/requires.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)        5 2023-07-01 17:07:49.000000 spin-0.4/spin.egg-info/top_level.txt
```

### Comparing `spin-0.3/LICENSE` & `spin-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spin-0.3/PKG-INFO` & `spin-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spin
-Version: 0.3
+Version: 0.4
 Summary: Developer tool for scientific Python libraries
 Maintainer-email: Scientific Python <spin@discuss.scientific-python.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2021--2022, Scientific Python project
         All rights reserved.
```

### Comparing `spin-0.3/README.md` & `spin-0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -45,31 +45,29 @@
 ```toml
 [tool.spin.commands]
 "Build" = [
   "spin.cmds.meson.build",
   "spin.cmds.meson.test"
 ]
 "Environments" = [
-  "spin.cmds.meson.shell",
   "spin.cmds.meson.ipython",
-  "spin.cmds.meson.python"
+  "spin.cmds.meson.run"
 ]
 ```
 
 These commands will then be rendered as:
 
 ```
 Build:
   build  🔧 Build package with Meson/ninja and install
   test   🔧 Run tests
 
 Environments:
-  shell    💻 Launch shell with PYTHONPATH set
   ipython  💻 Launch IPython shell with PYTHONPATH set
-  python   🐍 Launch Python shell with PYTHONPATH set
+  run      🏁 Run a shell command with PYTHONPATH set
 ```
 
 ## Running
 
 ```
 spin
 ```
@@ -86,22 +84,24 @@
 
 ```
   build    🔧 Build package with Meson/ninja and install to `build-install`
   ipython  💻 Launch IPython shell with PYTHONPATH set
   python   🐍 Launch Python shell with PYTHONPATH set
   shell    💻 Launch shell with PYTHONPATH set
   test     🔧 Run pytest
+  run      🏁 Run a shell command with PYTHONPATH set
+  docs     📖 Build Sphinx documentation
 ```
 
 ### [Build](https://pypa-build.readthedocs.io/en/stable/) (PEP 517 builder)
 
 `spin` was started with Meson in mind, but we're working on expanding commands for PEP 517 `build`.
 
 ```
-  sdist    📦 Build a source distribution in `dist/`.
+  sdist    📦 Build a source distribution in `dist/`
 ```
 
 ## 🧪 Custom commands
 
 `spin` can invoke custom commands. These commands define their own arguments, and have access to the `pyproject.toml` file for further configuration.
 
 See, e.g., the [example custom command](https://github.com/scientific-python/spin/blob/main/example_pkg/.spin/cmds.py).
```

### Comparing `spin-0.3/pyproject.toml` & `spin-0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "spin"
-version = "0.3"
+version = "0.4"
 requires-python = ">=3.7"
 description = "Developer tool for scientific Python libraries"
 license = {file = "LICENSE"}
 maintainers = [
   {name = "Scientific Python", email = "spin@discuss.scientific-python.org"}
 ]
 classifiers = [
@@ -17,19 +17,33 @@
   "colorama; platform_system == 'Windows'"
 ]
 
 [project.scripts]
 spin = "spin.__main__:main"
 
 [project.optional-dependencies]
-lint = ["pre-commit >= 3.2"]
+lint = ["pre-commit >= 3.3"]
 
 [project.urls]
 homepage = "https://github.com/scientific-python/spin"
 
 [tool.setuptools.packages.find]
 include = ["spin*"]
 
 [tool.pytest.ini_options]
 filterwarnings = [
   "ignore:cannot collect 'test' because it is not a function:",
 ]
+
+[tool.ruff]
+line-length = 88
+target-version = "py37"
+select = [
+    "C",
+    "E",
+    "F",
+    "W",
+    "B",
+    "I",
+    "UP",
+]
+ignore = ["B006", "C901", "E501", "E722"]
```

### Comparing `spin-0.3/spin/__main__.py` & `spin-0.4/spin/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 import collections
+import importlib
+import importlib.util
 import os
 import sys
-import importlib
-from glob import glob
 
 import click
 import toml
 
 from spin import cmds as _cmds
-from spin.cmds import util
-from spin.sectioned_help import SectionedHelpGroup
 from spin.color_format import ColorHelpFormatter
-
+from spin.sectioned_help import SectionedHelpGroup
 
 click.Context.formatter_class = ColorHelpFormatter
 
 
 class DotDict(collections.UserDict):
     def __getitem__(self, key):
         subitem = self.data
         for subkey in key.split("."):
             try:
                 subitem = subitem[subkey]
             except KeyError:
                 raise KeyError(f"`{key}` not found in configuration") from None
         return subitem
 
+    # Fix for Python 3.12
+    # See https://github.com/python/cpython/issues/105524
+    def __contains__(self, key):
+        subitem = self.data
+        for subkey in key.split("."):
+            try:
+                subitem = subitem[subkey]
+            except KeyError:
+                return False
+        return True
+
 
 def main():
     if not os.path.exists("pyproject.toml"):
         print("Error: cannot find [pyproject.toml]")
         sys.exit(1)
 
     with open("pyproject.toml") as f:
@@ -73,15 +82,15 @@
         "spin.shell": _cmds.meson.shell,
     }
 
     for section, cmds in config_cmds.items():
         for cmd in cmds:
             if cmd not in commands:
                 # First, see if we can directly import the command
-                if not ":" in cmd:
+                if ":" not in cmd:
                     path, func = cmd.rsplit(".", maxsplit=1)
                     try:
                         mod = importlib.import_module(path)
                     except ImportError:
                         print(
                             f"!! Could not import module `{path}` to load command `{cmd}`"
                         )
```

### Comparing `spin-0.3/spin/cmds/util.py` & `spin-0.4/spin/cmds/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import os
-import sys
-import subprocess
 import shlex
-import sysconfig
-from pathlib import Path
+import subprocess
+import sys
 
 import click
 
 
 def run(
     cmd, cwd=None, replace=False, sys_exit=True, output=True, echo=True, *args, **kwargs
 ):
@@ -15,14 +13,15 @@
 
     Parameters
     ----------
     cwd : str
         Change to this directory before execution.
     replace : bool
         Whether to replace the current process.
+        Note that this has no effect on Windows.
     sys_exit : bool
         Whether to exit if the shell command returns with error != 0.
     output : bool
         Whether to display output as the process runs.
         If set to ``False``, can be accessed afterwards as
         ``p.stdout``.
         If `sys_exit` is True and the process fails, output is printed
@@ -42,15 +41,15 @@
     if echo:
         click.secho(f"$ {cmdstr}", bold=True, fg="bright_blue")
 
     if output is False:
         output_kwargs = {"stdout": subprocess.PIPE, "stderr": subprocess.STDOUT}
         kwargs = {**output_kwargs, **kwargs}
 
-    if replace:
+    if replace and (sys.platform in ("linux", "darwin")):
         os.execvp(cmd[0], cmd)
         print(f"Failed to launch `{cmd}`")
         sys.exit(-1)
     else:
         p = subprocess.run(cmd, *args, **kwargs)
         if p.returncode != 0 and sys_exit:
             # Output was suppressed, but the process failed, so print it anyway
```

### Comparing `spin-0.3/spin/color_format.py` & `spin-0.4/spin/color_format.py`

 * *Files identical despite different names*

### Comparing `spin-0.3/spin/sectioned_help.py` & `spin-0.4/spin/sectioned_help.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import click
 import collections
 
+import click
+
 
 class SectionedHelpGroup(click.Group):
     """Organize commands as sections"""
 
     def __init__(self, *args, **kwargs):
         self.section_commands = collections.defaultdict(list)
         super().__init__(*args, **kwargs)
```

### Comparing `spin-0.3/spin/tests/test_meson.py` & `spin-0.4/spin/tests/test_meson.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import tempfile
-import sys
 import os
-from os.path import join as pjoin, normpath
+import sys
+import tempfile
+from os.path import join as pjoin
+from os.path import normpath
 
 import pytest
 
 from spin.cmds import meson
 
 
 def make_paths(root, paths):
@@ -74,15 +75,15 @@
                 meson._get_site_packages()
 
     # If there are multiple site-package paths, but without version information,
     # refuse the temptation to guess
     with tempfile.TemporaryDirectory() as d:
         install_dir = pjoin(d, "build-install")
         make_paths(
-            install_dir, [f"/Python3/x/site-packages", f"/Python3/y/site-packages"]
+            install_dir, ["/Python3/x/site-packages", "/Python3/y/site-packages"]
         )
         with pytest.raises(FileNotFoundError):
             meson._get_site_packages()
 
     # Multiple site-package paths found, but none that matches our Python
     with tempfile.TemporaryDirectory() as d:
         with monkeypatch.context() as m:
```

### Comparing `spin-0.3/spin.egg-info/PKG-INFO` & `spin-0.4/spin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spin
-Version: 0.3
+Version: 0.4
 Summary: Developer tool for scientific Python libraries
 Maintainer-email: Scientific Python <spin@discuss.scientific-python.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2021--2022, Scientific Python project
         All rights reserved.
```

