# Comparing `tmp/knarrow-0.7.0.tar.gz` & `tmp/knarrow-0.8.0.tar.gz`

## Comparing `knarrow-0.7.0.tar` & `knarrow-0.8.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 knarrow-0.7.0/src/knarrow/__about__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 knarrow-0.7.0/src/knarrow/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 knarrow-0.7.0/src/knarrow/angle_method.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 knarrow-0.7.0/src/knarrow/angle_method.pyi
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 knarrow-0.7.0/src/knarrow/c_method.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 knarrow-0.7.0/src/knarrow/c_method.pyi
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 knarrow-0.7.0/src/knarrow/distance_method.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 knarrow-0.7.0/src/knarrow/distance_method.pyi
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 knarrow-0.7.0/src/knarrow/kneedle.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 knarrow-0.7.0/src/knarrow/kneedle.pyi
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 knarrow-0.7.0/src/knarrow/main.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 knarrow-0.7.0/src/knarrow/main.pyi
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 knarrow-0.7.0/src/knarrow/menger.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 knarrow-0.7.0/src/knarrow/menger.pyi
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 knarrow-0.7.0/src/knarrow/ols.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 knarrow-0.7.0/src/knarrow/ols.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 knarrow-0.7.0/src/knarrow/py.typed
--rw-r--r--   0        0        0     9160 2020-02-02 00:00:00.000000 knarrow-0.7.0/src/knarrow/util.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 knarrow-0.7.0/src/knarrow/util.pyi
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 knarrow-0.7.0/src/knarrow/cli/__init__.py
--rw-r--r--   0        0        0     8043 2020-02-02 00:00:00.000000 knarrow-0.7.0/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 knarrow-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 knarrow-0.7.0/README.md
--rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 knarrow-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     4065 2020-02-02 00:00:00.000000 knarrow-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 knarrow-0.8.0/src/knarrow/__about__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 knarrow-0.8.0/src/knarrow/__init__.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 knarrow-0.8.0/src/knarrow/angle_method.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 knarrow-0.8.0/src/knarrow/angle_method.pyi
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 knarrow-0.8.0/src/knarrow/c_method.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 knarrow-0.8.0/src/knarrow/c_method.pyi
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 knarrow-0.8.0/src/knarrow/distance_method.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 knarrow-0.8.0/src/knarrow/distance_method.pyi
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 knarrow-0.8.0/src/knarrow/kneedle.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 knarrow-0.8.0/src/knarrow/kneedle.pyi
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 knarrow-0.8.0/src/knarrow/main.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 knarrow-0.8.0/src/knarrow/main.pyi
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 knarrow-0.8.0/src/knarrow/menger.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 knarrow-0.8.0/src/knarrow/menger.pyi
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 knarrow-0.8.0/src/knarrow/ols.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 knarrow-0.8.0/src/knarrow/ols.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 knarrow-0.8.0/src/knarrow/py.typed
+-rw-r--r--   0        0        0     9160 2020-02-02 00:00:00.000000 knarrow-0.8.0/src/knarrow/util.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 knarrow-0.8.0/src/knarrow/util.pyi
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 knarrow-0.8.0/src/knarrow/cli/__init__.py
+-rw-r--r--   0        0        0     8043 2020-02-02 00:00:00.000000 knarrow-0.8.0/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 knarrow-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 knarrow-0.8.0/README.md
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 knarrow-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 knarrow-0.8.0/PKG-INFO
```

### Comparing `knarrow-0.7.0/src/knarrow/angle_method.py` & `knarrow-0.8.0/src/knarrow/angle_method.py`

 * *Files identical despite different names*

### Comparing `knarrow-0.7.0/src/knarrow/c_method.py` & `knarrow-0.8.0/src/knarrow/c_method.py`

 * *Files identical despite different names*

### Comparing `knarrow-0.7.0/src/knarrow/distance_method.py` & `knarrow-0.8.0/src/knarrow/distance_method.py`

 * *Files identical despite different names*

### Comparing `knarrow-0.7.0/src/knarrow/kneedle.py` & `knarrow-0.8.0/src/knarrow/kneedle.py`

 * *Files identical despite different names*

### Comparing `knarrow-0.7.0/src/knarrow/main.py` & `knarrow-0.8.0/src/knarrow/main.py`

 * *Files identical despite different names*

### Comparing `knarrow-0.7.0/src/knarrow/menger.py` & `knarrow-0.8.0/src/knarrow/menger.py`

 * *Files identical despite different names*

### Comparing `knarrow-0.7.0/src/knarrow/menger.pyi` & `knarrow-0.8.0/src/knarrow/menger.pyi`

 * *Files identical despite different names*

### Comparing `knarrow-0.7.0/src/knarrow/ols.py` & `knarrow-0.8.0/src/knarrow/ols.py`

 * *Files identical despite different names*

### Comparing `knarrow-0.7.0/src/knarrow/util.py` & `knarrow-0.8.0/src/knarrow/util.py`

 * *Files identical despite different names*

### Comparing `knarrow-0.7.0/src/knarrow/util.pyi` & `knarrow-0.8.0/src/knarrow/util.pyi`

 * *Files identical despite different names*

### Comparing `knarrow-0.7.0/src/knarrow/cli/__init__.py` & `knarrow-0.8.0/src/knarrow/cli/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 # SPDX-License-Identifier: Apache-2.0
 
 from collections import Counter
 import enum
 from functools import partial
 from pathlib import Path
+import sys
 from typing import List, Optional
 
 import typer
 
 from knarrow import find_knee
 
 from ..__about__ import __version__
@@ -45,20 +46,18 @@
         raise typer.Exit(0)
 
 
 @app.command()
 def main(
     method: Method = typer.Option("all", help="The method to use to calculate the knee's position"),
     files: List[Path] = typer.Argument(
-        None,
         allow_dash=True,
         exists=True,
         dir_okay=False,
         readable=True,
-        callback=stdin_callback,
         help="List of input files (default: stdin)",
         show_default=False,
     ),
     sort: bool = typer.Option(False, help="Whether or not to sort the input"),
     delimiter: str = typer.Option(
         ",", help="If the input is 2-dimensional, split the dimensions by this option's value"
     ),
@@ -70,15 +69,16 @@
         None,
         "--version",
         callback=version_callback,
         is_eager=True,
     ),  # version boilerplate
 ):
     for path in files:
-        with path.open("r") as file:
+        file = sys.stdin if str(path) == "-" else path.open("r")
+        with file:
             rows = list(map(str.strip, file))
             split = partial(str.split, sep=delimiter)
             values = map(split, rows)
             numbers = list(tuple(float(value) for value in row) for row in values)
             indices = list(range(len(numbers)))
             if sort:
                 indices.sort(key=lambda i: numbers[i])
@@ -95,9 +95,9 @@
                 )
                 most_common = counter.most_common(1).pop(0)
                 knee = most_common[0]
             else:
                 knee = find_knee(numbers, method=method.value, sort=sort, smoothing=smoothing)
 
             result = indices[knee] if output == Output.INDEX else rows[indices[knee]]
-            print(path.name, result)
+            print(file.name if str(path) == "-" else path.name, result)
     return
```

### Comparing `knarrow-0.7.0/.gitignore` & `knarrow-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `knarrow-0.7.0/LICENSE.txt` & `knarrow-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `knarrow-0.7.0/README.md` & `knarrow-0.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # knarrow
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/knarrow)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/knarrow)
 ![PyPI - License](https://img.shields.io/pypi/l/knarrow)
 ![PyPI](https://img.shields.io/pypi/v/knarrow)
 ![PyPI - Format](https://img.shields.io/pypi/format/knarrow)
 ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/InCogNiTo124/knarrow)
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/InCogNiTo124/knarrow/python)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/InCogNiTo124/knarrow/.github/workflows/lint-and-test.yml?branch=master)
 ![Read the Docs](https://img.shields.io/readthedocs/knarrow)
 ![Website](https://img.shields.io/website?url=https%3A%2F%2Fknarrow.readthedocs.org)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Shoot a `knarrow` to the knee ;)
 
 _(The lib is better than this pun, I swear.)_
@@ -51,23 +51,26 @@
 >>> find_knee(A.T)  # also works with x in the first column, y in the second column
 4
 >>> find_knee(x, y, smoothing=0.01)  # for better results use cubic spline smoothing
 4
 ```
 
 ### CLI
-This library also comes with a handy CLI:
+This library can also come with a handy CLI if you install it with the `cli` extra:
 ```shell
-$ cat data.txt | knarrow
-stdin 11
-$ cat data.txt | knarrow -o value
-stdin 59874.14171519781845532648
+$ pip install "knarrow[cli]"
+$ cat data.txt | knarrow -
+<stdin> 11
+$ cat data.txt | knarrow -o value -
+<stdin> 59874.14171519781845532648
 $ knarrow --sort -d ',' -o value shuf_delim.txt
 shuf_delim.txt 20
 ```
+_(the `-` for stdin is, unfortunately, mandatory)_
+Try writing `knarrow --help` for more info.
 
 ## Similar projects
 
-While I've come up with most of these methods by myself, I am not the only one. Here is a (non-comprehensive) list of projects I've found that implement a similar funcionality and may have been an inspiration for me:
+While I've come up with most of these methods by myself, I am not the only one. Here is a (non-comprehensive) list of projects I've found that implement a similar functionality and may have been an inspiration for me:
 - [mariolpantunes/knee](https://github.com/mariolpantunes/knee)
 
-Note: this project was bootstrapped by [python-blueprint](https://github.com/johnthagen/python-blueprint)
+Note: this project was bootstrapped by [python-blueprint](https://github.com/johnthagen/python-blueprint). Since then, it has been heavily modified, though.
```

### Comparing `knarrow-0.7.0/pyproject.toml` & `knarrow-0.8.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -2,30 +2,29 @@
 requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 name = "knarrow"
 description = 'Shoot a knarrow to the knee'
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = [ "optimization", "knee", "elbow", "kneedle" ]
 authors = [
   { name = "Marijan Smetko", email = "msmetko@msmetko.xyz" },
 ]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "Intended Audience :: Information Technology",
   "Intended Audience :: Science/Research",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
   "Topic :: Scientific/Engineering :: Information Analysis",
   "Topic :: Scientific/Engineering :: Mathematics",
@@ -34,15 +33,15 @@
 ]
 dependencies = [
   "numpy",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
-cli = ["typer[all]==0.7.0"]
+cli = ["typer[all]==0.9.0"]
 
 [project.urls]
 Documentation = "https://github.com/InCogNiTo124/knarrow#readme"
 Issues = "https://github.com/InCogNiTo124/knarrow/issues"
 Source = "https://github.com/InCogNiTo124/knarrow"
 
 [project.scripts]
@@ -79,30 +78,30 @@
 [tool.hatch.build.targets.wheel]
 packages = ["src/knarrow"]
 
 [tool.hatch.build.targets.sdist]
 include = ["src/knarrow/*"]
 
 [[tool.hatch.envs.test.matrix]]
-python = ["37", "38", "39", "310", "311"]
+python = ["3.8", "3.9", "3.10", "3.11"]  # matches entries in workflow
 
 ### TODO perhaps optimize the tool configurations
 [tool.mypy]
 plugins = "numpy.typing.mypy_plugin"
 ignore_missing_imports = true
 allow_untyped_calls = true
 strict = false
 exclude = "venv"
 # If certain strict config options are too pedantic for a project,
 # disable them selectively here by setting to false.
 
 [tool.black]
 # Use the more relaxed max line length permitted in PEP8.
 line-length = 120
-target-version = ["py36", "py37", "py38", "py39"]
+target-version = ["py38", "py39", "py310", "py311"]
 # black will automatically exclude all files listed in .gitignore
 # If you need to exclude additional folders, consider using extend-exclude to avoid disabling the
 # default .gitignore behaviour.
 
 [tool.isort]
 profile = "black"
 line_length = 120
```

### Comparing `knarrow-0.7.0/PKG-INFO` & `knarrow-0.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knarrow
-Version: 0.7.0
+Version: 0.8.0
 Summary: Shoot a knarrow to the knee
 Project-URL: Documentation, https://github.com/InCogNiTo124/knarrow#readme
 Project-URL: Issues, https://github.com/InCogNiTo124/knarrow/issues
 Project-URL: Source, https://github.com/InCogNiTo124/knarrow
 Author-email: Marijan Smetko <msmetko@msmetko.xyz>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
@@ -13,38 +13,37 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: numpy
 Provides-Extra: cli
-Requires-Dist: typer[all]==0.7.0; extra == 'cli'
+Requires-Dist: typer[all]==0.9.0; extra == 'cli'
 Description-Content-Type: text/markdown
 
 # knarrow
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/knarrow)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/knarrow)
 ![PyPI - License](https://img.shields.io/pypi/l/knarrow)
 ![PyPI](https://img.shields.io/pypi/v/knarrow)
 ![PyPI - Format](https://img.shields.io/pypi/format/knarrow)
 ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/InCogNiTo124/knarrow)
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/InCogNiTo124/knarrow/python)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/InCogNiTo124/knarrow/.github/workflows/lint-and-test.yml?branch=master)
 ![Read the Docs](https://img.shields.io/readthedocs/knarrow)
 ![Website](https://img.shields.io/website?url=https%3A%2F%2Fknarrow.readthedocs.org)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Shoot a `knarrow` to the knee ;)
 
 _(The lib is better than this pun, I swear.)_
@@ -86,23 +85,26 @@
 >>> find_knee(A.T)  # also works with x in the first column, y in the second column
 4
 >>> find_knee(x, y, smoothing=0.01)  # for better results use cubic spline smoothing
 4
 ```
 
 ### CLI
-This library also comes with a handy CLI:
+This library can also come with a handy CLI if you install it with the `cli` extra:
 ```shell
-$ cat data.txt | knarrow
-stdin 11
-$ cat data.txt | knarrow -o value
-stdin 59874.14171519781845532648
+$ pip install "knarrow[cli]"
+$ cat data.txt | knarrow -
+<stdin> 11
+$ cat data.txt | knarrow -o value -
+<stdin> 59874.14171519781845532648
 $ knarrow --sort -d ',' -o value shuf_delim.txt
 shuf_delim.txt 20
 ```
+_(the `-` for stdin is, unfortunately, mandatory)_
+Try writing `knarrow --help` for more info.
 
 ## Similar projects
 
-While I've come up with most of these methods by myself, I am not the only one. Here is a (non-comprehensive) list of projects I've found that implement a similar funcionality and may have been an inspiration for me:
+While I've come up with most of these methods by myself, I am not the only one. Here is a (non-comprehensive) list of projects I've found that implement a similar functionality and may have been an inspiration for me:
 - [mariolpantunes/knee](https://github.com/mariolpantunes/knee)
 
-Note: this project was bootstrapped by [python-blueprint](https://github.com/johnthagen/python-blueprint)
+Note: this project was bootstrapped by [python-blueprint](https://github.com/johnthagen/python-blueprint). Since then, it has been heavily modified, though.
```

