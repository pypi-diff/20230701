# Comparing `tmp/gwf_wrangler-0.0.1.tar.gz` & `tmp/gwf_wrangler-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwf_wrangler-0.0.1.tar", last modified: Sat Jul  1 20:00:12 2023, max compression
+gzip compressed data, was "gwf_wrangler-0.0.2.tar", last modified: Sat Jul  1 21:20:56 2023, max compression
```

## Comparing `gwf_wrangler-0.0.1.tar` & `gwf_wrangler-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-01 20:00:12.208174 gwf_wrangler-0.0.1/
--rw-rw-r--   0 rlong     (1000) rlong     (1000)     1052 2023-06-26 00:02:06.000000 gwf_wrangler-0.0.1/LICENSE
--rw-rw-r--   0 rlong     (1000) rlong     (1000)        0 2023-07-01 18:00:16.000000 gwf_wrangler-0.0.1/MANIFEST.in
--rw-rw-r--   0 rlong     (1000) rlong     (1000)     4758 2023-07-01 20:00:12.208174 gwf_wrangler-0.0.1/PKG-INFO
--rw-rw-r--   0 rlong     (1000) rlong     (1000)     3023 2023-07-01 19:03:42.000000 gwf_wrangler-0.0.1/README.md
-drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-01 20:00:12.200174 gwf_wrangler-0.0.1/gwf_wrangler.egg-info/
--rw-rw-r--   0 rlong     (1000) rlong     (1000)     4758 2023-07-01 20:00:12.000000 gwf_wrangler-0.0.1/gwf_wrangler.egg-info/PKG-INFO
--rw-rw-r--   0 rlong     (1000) rlong     (1000)      650 2023-07-01 20:00:12.000000 gwf_wrangler-0.0.1/gwf_wrangler.egg-info/SOURCES.txt
--rw-rw-r--   0 rlong     (1000) rlong     (1000)        1 2023-07-01 20:00:12.000000 gwf_wrangler-0.0.1/gwf_wrangler.egg-info/dependency_links.txt
--rw-rw-r--   0 rlong     (1000) rlong     (1000)       56 2023-07-01 20:00:12.000000 gwf_wrangler-0.0.1/gwf_wrangler.egg-info/entry_points.txt
--rw-rw-r--   0 rlong     (1000) rlong     (1000)       51 2023-07-01 20:00:12.000000 gwf_wrangler-0.0.1/gwf_wrangler.egg-info/requires.txt
--rw-rw-r--   0 rlong     (1000) rlong     (1000)       29 2023-07-01 20:00:12.000000 gwf_wrangler-0.0.1/gwf_wrangler.egg-info/top_level.txt
--rw-rw-r--   0 rlong     (1000) rlong     (1000)     1480 2023-07-01 19:59:43.000000 gwf_wrangler-0.0.1/pyproject.toml
--rw-rw-r--   0 rlong     (1000) rlong     (1000)       38 2023-07-01 20:00:12.208174 gwf_wrangler-0.0.1/setup.cfg
-drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-01 20:00:12.200174 gwf_wrangler-0.0.1/src/
-drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-01 20:00:12.204174 gwf_wrangler-0.0.1/src/wrangler/
--rw-rw-r--   0 rlong     (1000) rlong     (1000)        0 2023-07-01 17:55:42.000000 gwf_wrangler-0.0.1/src/wrangler/__init__.py
--rw-rw-r--   0 rlong     (1000) rlong     (1000)     1669 2023-07-01 18:30:53.000000 gwf_wrangler-0.0.1/src/wrangler/__main__.py
--rw-rw-r--   0 rlong     (1000) rlong     (1000)       81 2023-07-01 18:30:53.000000 gwf_wrangler-0.0.1/src/wrangler/cli.py
--rw-rw-r--   0 rlong     (1000) rlong     (1000)     3506 2023-07-01 18:30:53.000000 gwf_wrangler-0.0.1/src/wrangler/script.py
-drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-01 20:00:12.200174 gwf_wrangler-0.0.1/venv/
-drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-01 20:00:12.204174 gwf_wrangler-0.0.1/venv/bin/
--rw-rw-r--   0 rlong     (1000) rlong     (1000)     1176 2023-07-01 19:55:16.000000 gwf_wrangler-0.0.1/venv/bin/activate_this.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      631 2023-07-01 19:56:22.000000 gwf_wrangler-0.0.1/venv/bin/rst2html.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      753 2023-07-01 19:56:22.000000 gwf_wrangler-0.0.1/venv/bin/rst2html4.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)     1088 2023-07-01 19:56:22.000000 gwf_wrangler-0.0.1/venv/bin/rst2html5.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      830 2023-07-01 19:56:22.000000 gwf_wrangler-0.0.1/venv/bin/rst2latex.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      653 2023-07-01 19:56:22.000000 gwf_wrangler-0.0.1/venv/bin/rst2man.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      819 2023-07-01 19:56:22.000000 gwf_wrangler-0.0.1/venv/bin/rst2odt.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      625 2023-07-01 19:56:22.000000 gwf_wrangler-0.0.1/venv/bin/rst2odt_prepstyles.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      638 2023-07-01 19:56:22.000000 gwf_wrangler-0.0.1/venv/bin/rst2pseudoxml.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      674 2023-07-01 19:56:22.000000 gwf_wrangler-0.0.1/venv/bin/rst2s5.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      910 2023-07-01 19:56:22.000000 gwf_wrangler-0.0.1/venv/bin/rst2xetex.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      639 2023-07-01 19:56:22.000000 gwf_wrangler-0.0.1/venv/bin/rst2xml.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      707 2023-07-01 19:56:22.000000 gwf_wrangler-0.0.1/venv/bin/rstpep2html.py
+drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-01 21:20:56.990257 gwf_wrangler-0.0.2/
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     1052 2023-07-01 20:09:07.000000 gwf_wrangler-0.0.2/LICENSE
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)        0 2023-07-01 20:09:07.000000 gwf_wrangler-0.0.2/MANIFEST.in
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     4758 2023-07-01 21:20:56.990257 gwf_wrangler-0.0.2/PKG-INFO
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     3023 2023-07-01 21:14:06.000000 gwf_wrangler-0.0.2/README.md
+drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-01 21:20:56.986256 gwf_wrangler-0.0.2/gwf_wrangler.egg-info/
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     4758 2023-07-01 21:20:56.000000 gwf_wrangler-0.0.2/gwf_wrangler.egg-info/PKG-INFO
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)      614 2023-07-01 21:20:56.000000 gwf_wrangler-0.0.2/gwf_wrangler.egg-info/SOURCES.txt
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)        1 2023-07-01 21:20:56.000000 gwf_wrangler-0.0.2/gwf_wrangler.egg-info/dependency_links.txt
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)       47 2023-07-01 21:20:56.000000 gwf_wrangler-0.0.2/gwf_wrangler.egg-info/entry_points.txt
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)       63 2023-07-01 21:20:56.000000 gwf_wrangler-0.0.2/gwf_wrangler.egg-info/requires.txt
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)       29 2023-07-01 21:20:56.000000 gwf_wrangler-0.0.2/gwf_wrangler.egg-info/top_level.txt
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     1460 2023-07-01 21:20:25.000000 gwf_wrangler-0.0.2/pyproject.toml
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)       38 2023-07-01 21:20:56.990257 gwf_wrangler-0.0.2/setup.cfg
+drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-01 21:20:56.986256 gwf_wrangler-0.0.2/src/
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)        0 2023-07-01 20:09:07.000000 gwf_wrangler-0.0.2/src/__init__.py
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     1727 2023-07-01 21:04:52.000000 gwf_wrangler-0.0.2/src/__main__.py
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     1019 2023-07-01 21:10:39.000000 gwf_wrangler-0.0.2/src/cli.py
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     3577 2023-07-01 20:28:10.000000 gwf_wrangler-0.0.2/src/script.py
+drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-01 21:20:56.982257 gwf_wrangler-0.0.2/venv/
+drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-01 21:20:56.990257 gwf_wrangler-0.0.2/venv/bin/
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     1176 2023-07-01 20:23:27.000000 gwf_wrangler-0.0.2/venv/bin/activate_this.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      631 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.2/venv/bin/rst2html.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      753 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.2/venv/bin/rst2html4.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)     1088 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.2/venv/bin/rst2html5.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      830 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.2/venv/bin/rst2latex.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      653 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.2/venv/bin/rst2man.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      819 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.2/venv/bin/rst2odt.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      625 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.2/venv/bin/rst2odt_prepstyles.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      638 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.2/venv/bin/rst2pseudoxml.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      674 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.2/venv/bin/rst2s5.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      910 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.2/venv/bin/rst2xetex.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      639 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.2/venv/bin/rst2xml.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      707 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.2/venv/bin/rstpep2html.py
```

### Comparing `gwf_wrangler-0.0.1/LICENSE` & `gwf_wrangler-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.1/PKG-INFO` & `gwf_wrangler-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwf_wrangler
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python package to convert yaml files to lua scripts for the Global Workflow Project.
 Author-email: Ryan Long <ryan.long@noaa.gov>
 License: Copyright 2023 NOAA
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -19,15 +19,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
-# Wrangler (0.0.1)
+# Wrangler (0.0.2)
 
 ## Logging
 
 ### Use the Correct Levels When Logging
 
 It might be difficult to decide which level to assign each event. Fortunately, the Python logging module presents fewer levels than other logging libraries. This makes things easier by eliminating some potential ambiguity. When it comes to Python levels, here are the general guidelines:
```

### Comparing `gwf_wrangler-0.0.1/README.md` & `gwf_wrangler-0.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-# Wrangler (0.0.1)
+# Wrangler (0.0.2)
 
 ## Logging
 
 ### Use the Correct Levels When Logging
 
 It might be difficult to decide which level to assign each event. Fortunately, the Python logging module presents fewer levels than other logging libraries. This makes things easier by eliminating some potential ambiguity. When it comes to Python levels, here are the general guidelines:
```

### Comparing `gwf_wrangler-0.0.1/gwf_wrangler.egg-info/PKG-INFO` & `gwf_wrangler-0.0.2/gwf_wrangler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwf-wrangler
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python package to convert yaml files to lua scripts for the Global Workflow Project.
 Author-email: Ryan Long <ryan.long@noaa.gov>
 License: Copyright 2023 NOAA
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -19,15 +19,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
-# Wrangler (0.0.1)
+# Wrangler (0.0.2)
 
 ## Logging
 
 ### Use the Correct Levels When Logging
 
 It might be difficult to decide which level to assign each event. Fortunately, the Python logging module presents fewer levels than other logging libraries. This makes things easier by eliminating some potential ambiguity. When it comes to Python levels, here are the general guidelines:
```

### Comparing `gwf_wrangler-0.0.1/gwf_wrangler.egg-info/SOURCES.txt` & `gwf_wrangler-0.0.2/gwf_wrangler.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 pyproject.toml
 gwf_wrangler.egg-info/PKG-INFO
 gwf_wrangler.egg-info/SOURCES.txt
 gwf_wrangler.egg-info/dependency_links.txt
 gwf_wrangler.egg-info/entry_points.txt
 gwf_wrangler.egg-info/requires.txt
 gwf_wrangler.egg-info/top_level.txt
-src/wrangler/__init__.py
-src/wrangler/__main__.py
-src/wrangler/cli.py
-src/wrangler/script.py
+src/__init__.py
+src/__main__.py
+src/cli.py
+src/script.py
 venv/bin/activate_this.py
 venv/bin/rst2html.py
 venv/bin/rst2html4.py
 venv/bin/rst2html5.py
 venv/bin/rst2latex.py
 venv/bin/rst2man.py
 venv/bin/rst2odt.py
```

### Comparing `gwf_wrangler-0.0.1/pyproject.toml` & `gwf_wrangler-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 requires = ["setuptools", "versioneer[toml]"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gwf_wrangler"
 description = "A python package to convert yaml files to lua scripts for the Global Workflow Project."
 readme = "README.md"
-version = "0.0.1"
+version = "0.0.2"
 dependencies = ["PyYAML"]
 authors = [{ name = "Ryan Long", email = "ryan.long@noaa.gov" }]
 keywords = ["globalworkflow", "global workflow", "esmf"]
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 
 [project.optional-dependencies]
-dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
+dev = ["black", "bumpver", "isort", "pip-tools", "pytest", "twine", "build"]
 
 
 [project.scripts]
-wrangler = "src.wrangler.__main__:main"
+wrangler = "src.__main__:main"
 
 [project.urls]
 "Homepage" = "https://github.com/pypa/wrangler"
 "Bug Tracker" = "https://github.com/pypa/wrangler/issues"
 
 [tool.setuptools.packages]
 find = {} # Scan the project directory with the default parameters
@@ -37,17 +37,17 @@
 style = "pep440"
 versionfile_source = "src/wrangler/_version.py"
 versionfile_build = "wrangler/_version.py"
 tag_prefix = ""
 # parentdir_prefix = "myproject-"
 
 [tool.bumpver]
-current_version = "0.0.1"
+current_version = "0.0.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
-"pyproject.toml" = ['version = "{current_version}"']
+"pyproject.toml" = ['']
 "README.md" = ["{pep440_version}"]
```

### Comparing `gwf_wrangler-0.0.1/src/wrangler/__main__.py` & `gwf_wrangler-0.0.2/src/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """main execution"""
 
 import logging
 from pathlib import Path
 
 import yaml
 
-from src.wrangler.script import Script, find_script, to_lua
+from src.script import Script, find_script, to_lua
+from src.cli import get_cli_data
 
 
 def load_scripts_from_yamls(_paths: list[Path]) -> list[Script]:
     """instantiates Script instances from yaml files"""
     results = []
     for _path in _paths:
         logging.info("extracting scripts from %s", _path)
@@ -42,17 +43,16 @@
     """main execution"""
     logging.basicConfig(
         level=logging.DEBUG,
         format="%(asctime)s %(levelname)s %(message)s",
         datefmt="%Y-%m-%d %H:%M:%S",
         filename="wrangler.log",
     )
-
-    _input = [
-        Path("./tests/fixtures/test.yaml"),
-        Path("./tests/fixtures/test copy.yaml"),
-    ]
-    write_scripts_to_lua(Path("./"), load_scripts_from_yamls(_input), "common")
+    data = get_cli_data()
+    _input = data["queue"]
+    output_path = Path(data["output_path"])
+    output_path.mkdir(parents=True, exist_ok=True)
+    write_scripts_to_lua(output_path, load_scripts_from_yamls(_input), "common")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `gwf_wrangler-0.0.1/src/wrangler/script.py` & `gwf_wrangler-0.0.2/src/script.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Convert yaml config files to LUA scripts"""
 import json
 import os
 from typing import Any
 
 # Configuration
 
-ORDER = ["modulepaths", "modules", "help", "environment", "whatis", "extra"]
+ORDER = ["help", "modulepaths", "modules", "environment", "whatis", "extra"]
 
 
 def ensure_list(value):
     """ensures a value is a list or coerces to list of len 1"""
     return value if isinstance(value, list) else [value]
 
 
@@ -33,17 +33,22 @@
         key, _value = value.split("/")
         results.append(f'load(pathJoin("{key}", "{os.environ.get(_value)}"))\n')
     return results
 
 
 def module_paths(values: list[str]) -> list[str]:
     """returns list of PosixPaths"""
+    print(values)
     if not values:
         return []
-    return [f'prepend_path("MODULEPATH", pathJoin("{_path}"))\n' for _path in values]
+    return [
+        f'prepend_path("MODULEPATH", pathJoin("{_path}"))\n'
+        for _path in values
+        if _path != "None"
+    ]
 
 
 def what_is(values: list[str]) -> list[str]:
     """returns list of WhatIs"""
     if not values:
         return []
     return [f'whatis("{value}")\n' for value in ensure_list(values)]
@@ -106,15 +111,16 @@
         if key in self.data:
             return self.data[key]
         return default
 
 
 def to_lua(_script: Script, **kwargs) -> list[str]:
     """converts a Script instance to a lua script"""
-    order = ORDER if kwargs.get("order") is None else kwargs.get("order")
+    order = kwargs.get("order")
+    order = ORDER if order is None else order
     results = []
     for key in order:
         for _line in MAPPER_PROPS[key](_script.get(key, None)):
             results.append(_line)
     return results
```

### Comparing `gwf_wrangler-0.0.1/venv/bin/activate_this.py` & `gwf_wrangler-0.0.2/venv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.1/venv/bin/rst2html.py` & `gwf_wrangler-0.0.2/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.1/venv/bin/rst2html4.py` & `gwf_wrangler-0.0.2/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.1/venv/bin/rst2html5.py` & `gwf_wrangler-0.0.2/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.1/venv/bin/rst2latex.py` & `gwf_wrangler-0.0.2/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.1/venv/bin/rst2man.py` & `gwf_wrangler-0.0.2/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.1/venv/bin/rst2odt.py` & `gwf_wrangler-0.0.2/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.1/venv/bin/rst2odt_prepstyles.py` & `gwf_wrangler-0.0.2/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.1/venv/bin/rst2pseudoxml.py` & `gwf_wrangler-0.0.2/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.1/venv/bin/rst2s5.py` & `gwf_wrangler-0.0.2/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.1/venv/bin/rst2xetex.py` & `gwf_wrangler-0.0.2/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.1/venv/bin/rst2xml.py` & `gwf_wrangler-0.0.2/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.1/venv/bin/rstpep2html.py` & `gwf_wrangler-0.0.2/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

