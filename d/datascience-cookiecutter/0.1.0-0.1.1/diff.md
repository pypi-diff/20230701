# Comparing `tmp/datascience_cookiecutter-0.1.0.tar.gz` & `tmp/datascience_cookiecutter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datascience_cookiecutter-0.1.0.tar", last modified: Sat Jul  1 21:04:03 2023, max compression
+gzip compressed data, was "datascience_cookiecutter-0.1.1.tar", last modified: Sat Jul  1 21:32:35 2023, max compression
```

## Comparing `datascience_cookiecutter-0.1.0.tar` & `datascience_cookiecutter-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      902 2023-07-01 20:38:51.925391 datascience_cookiecutter-0.1.0/README.md
--rw-r--r--   0        0        0      137 2023-06-30 19:36:30.086501 datascience_cookiecutter-0.1.0/datascience_cookiecutter/__init__.py
--rw-r--r--   0        0        0      479 2023-07-01 20:57:47.212751 datascience_cookiecutter-0.1.0/datascience_cookiecutter/cli.py
--rw-r--r--   0        0        0     3886 2023-07-01 20:44:47.026545 datascience_cookiecutter-0.1.0/datascience_cookiecutter/folderbuilder.py
--rw-r--r--   0        0        0     3363 2023-07-01 20:48:08.567048 datascience_cookiecutter-0.1.0/datascience_cookiecutter/templates.py
--rw-r--r--   0        0        0      834 2023-07-01 21:04:03.558662 datascience_cookiecutter-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8042 2023-06-30 22:34:34.542238 datascience_cookiecutter-0.1.0/tests/test_datascience_cookiecutter.py
--rw-r--r--   0        0        0     1532 1970-01-01 00:00:00.000000 datascience_cookiecutter-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      909 2023-07-01 21:28:19.151138 datascience_cookiecutter-0.1.1/README.md
+-rw-r--r--   0        0        0      161 2023-07-01 21:32:11.821252 datascience_cookiecutter-0.1.1/datascience_cookiecutter/__init__.py
+-rw-r--r--   0        0        0      490 2023-07-01 21:31:26.287090 datascience_cookiecutter-0.1.1/datascience_cookiecutter/cli.py
+-rw-r--r--   0        0        0     3910 2023-07-01 21:30:54.160107 datascience_cookiecutter-0.1.1/datascience_cookiecutter/folderbuilder.py
+-rw-r--r--   0        0        0     3363 2023-07-01 20:48:08.567048 datascience_cookiecutter-0.1.1/datascience_cookiecutter/templates.py
+-rw-r--r--   0        0        0      833 2023-07-01 21:32:35.286332 datascience_cookiecutter-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     8042 2023-06-30 22:34:34.542238 datascience_cookiecutter-0.1.1/tests/test_datascience_cookiecutter.py
+-rw-r--r--   0        0        0     1539 1970-01-01 00:00:00.000000 datascience_cookiecutter-0.1.1/PKG-INFO
```

### Comparing `datascience_cookiecutter-0.1.0/README.md` & `datascience_cookiecutter-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 <!-- [![PyPi version](https://badgen.net/pypi/v/mltrainer/)](https://pypi.org/project/mltrainer/) -->
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
+```
 .
 ├── Makefile
 ├── README.md
 ├── data
 │   ├── final
 │   ├── processed
 │   ├── raw
@@ -21,7 +22,8 @@
 ├── reports
 │   ├── img
 │   └── report.md
 ├── test
 │   ├── __init__.py
 │   └── main.py
 └── tests
+```
```

### Comparing `datascience_cookiecutter-0.1.0/datascience_cookiecutter/folderbuilder.py` & `datascience_cookiecutter-0.1.1/datascience_cookiecutter/folderbuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import subprocess
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 from loguru import logger
 
-from .templates import CookiecutterSettings, FileTemplate
+from datascience_cookiecutter.templates import CookiecutterSettings, FileTemplate
 
 if TYPE_CHECKING:
     from .templates import Folder
 
 
 class Cookiecutter:
     def __init__(self, settings: CookiecutterSettings):
```

### Comparing `datascience_cookiecutter-0.1.0/datascience_cookiecutter/templates.py` & `datascience_cookiecutter-0.1.1/datascience_cookiecutter/templates.py`

 * *Files identical despite different names*

### Comparing `datascience_cookiecutter-0.1.0/pyproject.toml` & `datascience_cookiecutter-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "datascience-cookiecutter"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = [
     { name = "", email = "" },
 ]
 dependencies = [
     "pydantic>=2.0",
     "loguru>=0.7.0",
@@ -27,19 +27,19 @@
     "pytest>=7.4.0",
     "ruff>=0.0.275",
     "black>=23.3.0",
     "isort>=5.11.5",
     "mypy>=1.4.1",
 ]
 
-[tool.urls]
+[tool.pdm.urls]
 GitHub = "https://github.com/raoulg/datascience-cookiecutter"
 
 [tool.pdm.scripts.cookiecutter]
-call = "datascience_cookiecutter.cli:main"
+call = "datascience_cookiecutter.cli"
 deps = [
     "click",
 ]
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `datascience_cookiecutter-0.1.0/tests/test_datascience_cookiecutter.py` & `datascience_cookiecutter-0.1.1/tests/test_datascience_cookiecutter.py`

 * *Files identical despite different names*

### Comparing `datascience_cookiecutter-0.1.0/PKG-INFO` & `datascience_cookiecutter-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datascience-cookiecutter
-Version: 0.1.0
+Version: 0.1.1
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Environment :: Console
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Requires-Dist: pydantic>=2.0
@@ -20,14 +20,15 @@
 
 
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 <!-- [![PyPi version](https://badgen.net/pypi/v/mltrainer/)](https://pypi.org/project/mltrainer/) -->
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
+```
 .
 ├── Makefile
 ├── README.md
 ├── data
 │   ├── final
 │   ├── processed
 │   ├── raw
@@ -41,7 +42,8 @@
 ├── reports
 │   ├── img
 │   └── report.md
 ├── test
 │   ├── __init__.py
 │   └── main.py
 └── tests
+```
```

