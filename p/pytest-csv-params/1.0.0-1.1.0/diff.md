# Comparing `tmp/pytest-csv-params-1.0.0.tar.gz` & `tmp/pytest_csv_params-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-csv-params-1.0.0.tar", max compression
+gzip compressed data, was "pytest_csv_params-1.1.0.tar", max compression
```

## Comparing `pytest-csv-params-1.0.0.tar` & `pytest_csv_params-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     1099 2022-08-14 19:36:56.437445 pytest-csv-params-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     8448 2022-08-28 12:35:39.288832 pytest-csv-params-1.0.0/README.md
--rw-r--r--   0        0        0        0 2022-08-12 17:11:28.285736 pytest-csv-params-1.0.0/_ptcsvp/__init__.py
--rw-r--r--   0        0        0      922 2022-08-25 11:47:58.554561 pytest-csv-params-1.0.0/_ptcsvp/cmdline.py
--rw-r--r--   0        0        0      871 2022-08-25 11:47:58.554561 pytest-csv-params-1.0.0/_ptcsvp/configure.py
--rw-r--r--   0        0        0     5914 2022-08-25 11:47:58.554561 pytest-csv-params-1.0.0/_ptcsvp/parametrize.py
--rw-r--r--   0        0        0      857 2022-08-25 11:47:58.555561 pytest-csv-params-1.0.0/_ptcsvp/plugin.py
--rw-r--r--   0        0        0     1852 2022-08-25 11:47:58.555561 pytest-csv-params-1.0.0/_ptcsvp/varname.py
--rw-r--r--   0        0        0     1526 2022-08-25 11:47:58.555561 pytest-csv-params-1.0.0/_ptcsvp/version.py
--rw-r--r--   0        0        0     4522 2022-08-28 12:36:45.001498 pytest-csv-params-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-08-13 19:10:29.012951 pytest-csv-params-1.0.0/pytest_csv_params/__init__.py
--rw-r--r--   0        0        0      261 2022-08-25 11:47:58.557561 pytest-csv-params-1.0.0/pytest_csv_params/decorator.py
--rw-r--r--   0        0        0      742 2022-08-25 11:47:58.558561 pytest-csv-params-1.0.0/pytest_csv_params/dialect.py
--rw-r--r--   0        0        0      818 2022-08-25 11:47:58.558561 pytest-csv-params-1.0.0/pytest_csv_params/exception.py
--rw-r--r--   0        0        0     1009 2022-08-25 17:16:11.372108 pytest-csv-params-1.0.0/pytest_csv_params/plugin.py
--rw-r--r--   0        0        0     2373 2022-08-25 11:47:58.558561 pytest-csv-params-1.0.0/pytest_csv_params/types.py
--rw-r--r--   0        0        0     9491 2022-08-28 12:59:04.213022 pytest-csv-params-1.0.0/setup.py
--rw-r--r--   0        0        0    10177 2022-08-28 12:59:04.214196 pytest-csv-params-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-07-01 12:43:25.132884 pytest_csv_params-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     8452 2023-07-01 14:58:42.477964 pytest_csv_params-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-01 12:43:25.132884 pytest_csv_params-1.1.0/_ptcsvp/__init__.py
+-rw-r--r--   0        0        0      922 2023-07-01 12:43:25.132884 pytest_csv_params-1.1.0/_ptcsvp/cmdline.py
+-rw-r--r--   0        0        0      881 2023-07-01 14:58:42.477964 pytest_csv_params-1.1.0/_ptcsvp/configure.py
+-rw-r--r--   0        0        0     5914 2023-07-01 12:43:25.132884 pytest_csv_params-1.1.0/_ptcsvp/parametrize.py
+-rw-r--r--   0        0        0      857 2023-07-01 12:43:25.132884 pytest_csv_params-1.1.0/_ptcsvp/plugin.py
+-rw-r--r--   0        0        0     1852 2023-07-01 12:43:25.132884 pytest_csv_params-1.1.0/_ptcsvp/varname.py
+-rw-r--r--   0        0        0     1526 2023-07-01 14:58:42.477964 pytest_csv_params-1.1.0/_ptcsvp/version.py
+-rw-r--r--   0        0        0     4636 2023-07-01 14:58:42.481964 pytest_csv_params-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-01 12:43:25.144884 pytest_csv_params-1.1.0/pytest_csv_params/__init__.py
+-rw-r--r--   0        0        0      261 2023-07-01 12:43:25.144884 pytest_csv_params-1.1.0/pytest_csv_params/decorator.py
+-rw-r--r--   0        0        0      742 2023-07-01 12:43:25.144884 pytest_csv_params-1.1.0/pytest_csv_params/dialect.py
+-rw-r--r--   0        0        0      818 2023-07-01 12:43:25.144884 pytest_csv_params-1.1.0/pytest_csv_params/exception.py
+-rw-r--r--   0        0        0     1009 2023-07-01 12:43:25.144884 pytest_csv_params-1.1.0/pytest_csv_params/plugin.py
+-rw-r--r--   0        0        0     2373 2023-07-01 12:43:25.144884 pytest_csv_params-1.1.0/pytest_csv_params/types.py
+-rw-r--r--   0        0        0    10232 1970-01-01 00:00:00.000000 pytest_csv_params-1.1.0/PKG-INFO
```

### Comparing `pytest-csv-params-1.0.0/LICENSE.txt` & `pytest_csv_params-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytest-csv-params-1.0.0/README.md` & `pytest_csv_params-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 [![PyPI - Downloads](https://img.shields.io/pypi/dw/pytest-csv-params?label=PyPI%20downloads&style=flat&logo=pypi)](https://pypi.org/project/pytest-csv-params/)
 [![PyPI - Version](https://img.shields.io/pypi/v/pytest-csv-params?label=PyPI%20version&style=flat&logo=pypi)](https://pypi.org/project/pytest-csv-params/)
 [![PyPI - Status](https://img.shields.io/pypi/status/pytest-csv-params?label=PyPI%20status&style=flat&logo=pypi)](https://pypi.org/project/pytest-csv-params/)
 [![PyPI - Format](https://img.shields.io/pypi/format/pytest-csv-params?label=PyPI%20format&style=flat&logo=pypi)](https://pypi.org/project/pytest-csv-params/)
 
 ## Requirements
  
-- Python 3.8, 3.9 or 3.10
-- pytest >= 7.1
+- Python 3.8, 3.9, 3.10, 3.11
+- pytest >= 7.4
 
 There's no operating system dependent code in this plugin, so it should run anywhere where pytest runs.
 
 ## Installation
 
 Simply install it with pip...
```

### Comparing `pytest-csv-params-1.0.0/_ptcsvp/cmdline.py` & `pytest_csv_params-1.1.0/_ptcsvp/cmdline.py`

 * *Files identical despite different names*

### Comparing `pytest-csv-params-1.0.0/_ptcsvp/configure.py` & `pytest_csv_params-1.1.0/_ptcsvp/configure.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 def pytest_configure(config: Config, plugin_name: str = "csv_params") -> None:
     """
     Register our Plugin
 
     :param config: Pytets configuration class
     :param plugin_name: The name of the pytest plugin, with default value
     """
-    config.pluginmanager.register(Plugin(config), f"{plugin_name}_plugin")
+    config.pluginmanager.register(Plugin(config), name=f"{plugin_name}_plugin")
 
 
 def pytest_unconfigure(config: Config, plugin_name: str = "csv_params") -> None:
     """
     Remove our Plugin
 
     :param config: Pytest configuration class
     :param plugin_name: The name of the pytest plgin, with default value
     """
-    config.pluginmanager.unregister(f"{plugin_name}_plugin")
+    config.pluginmanager.unregister(name=f"{plugin_name}_plugin")
```

### Comparing `pytest-csv-params-1.0.0/_ptcsvp/parametrize.py` & `pytest_csv_params-1.1.0/_ptcsvp/parametrize.py`

 * *Files identical despite different names*

### Comparing `pytest-csv-params-1.0.0/_ptcsvp/plugin.py` & `pytest_csv_params-1.1.0/_ptcsvp/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-csv-params-1.0.0/_ptcsvp/varname.py` & `pytest_csv_params-1.1.0/_ptcsvp/varname.py`

 * *Files identical despite different names*

### Comparing `pytest-csv-params-1.0.0/_ptcsvp/version.py` & `pytest_csv_params-1.1.0/_ptcsvp/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,19 @@
     :raises PythonTooOldError: When the python version is too old/unsupported
     """
 
     if sys.version_info < min_version:
         raise PythonTooOldError(f"At least Python {'.'.join(map(str, min_version))} required")
 
 
-def check_pytest_version(min_version: Tuple[int, int] = (7, 1)) -> None:
+def check_pytest_version(min_version: Tuple[int, int] = (7, 4)) -> None:
     """
-    Check if the current version is at least 7.1
+    Check if the current version is at least 7.4
 
-    :param min_version: The minimum version required, as tuple, default is 7.1
+    :param min_version: The minimum version required, as tuple, default is 7.4
     :raises RuntimeError: When the pytest version is too old/unsupported
     """
 
     from pytest import __version__ as pytest_version  # pylint: disable=import-outside-toplevel
 
     pytest_min_version = ".".join(map(str, min_version))
     parsed_min_version = parse(pytest_min_version)
```

### Comparing `pytest-csv-params-1.0.0/pyproject.toml` & `pytest_csv_params-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-csv-params"
-version = "1.0.0"
+version = "1.1.0"
 description = "Pytest plugin for Test Case Parametrization with CSV files"
 authors = ["Juergen Edelbluth <csv_params@jued.de>"]
 license = "MIT"
 repository = "https://git.codebau.dev/pytest-plugins/pytest-csv-params"
 homepage = "https://git.codebau.dev/pytest-plugins/pytest-csv-params"
 readme = "README.md"
 keywords = [
@@ -48,14 +48,15 @@
     "ignore:.*BlackItem.*:_pytest.warning_types.PytestDeprecationWarning",
     "ignore:.*BlackItem.*:_pytest.warning_types.PytestRemovedIn8Warning",
     "ignore:.*PyLintFile.*:_pytest.warning_types.PytestRemovedIn8Warning",
     "ignore:.*BlackItem.*:_pytest.warning_types.PytestWarning",
     "ignore:Using the __implements__ inheritance pattern for BaseReporter is no longer supported. Child classes should only inherit BaseReporter",
     "ignore:.*zipimport.*",
     "ignore:Creating a LegacyVersion has been deprecated and will be removed in the next major release",
+    "ignore:The hookimpl .* uses old-style configuration options.*",
 ]
 junit_family = "xunit2"
 junit_logging = "all"
 junit_log_passing_tests = true
 junit_duration_report = "call"
 junit_suite_name = "pytest-csv-params"
 
@@ -99,45 +100,46 @@
     "raise NotImplementedError",
     "if __name__ == .__main__.:",
 ]
 
 [tool.mypy]
 python_version = "3.8"
 strict = true
+ignore_missing_imports = true
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 minversion = 3.25.0
-envlist = clean,py38,py39,py310
+envlist = clean,py38,py39,py310,py311
 isolated_build = True
 
 [testenv]
 commands =
     pytest --cov-append
 
 [testenv:clean]
 skip_install = true
 commands =
     coverage erase
 """
 
 [tool.black]
 line-length = 120
-target-version = ['py38', 'py39', 'py310']
+target-version = ['py38', 'py39', 'py310', 'py311']
 include = '\.pyi?$'
 
 [tool.isort]
 line_length = 120
 include_trailing_comma = true
 multi_line_output = 3
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pytest = "^7.1.2"
+pytest = "^7.4.0"
 
 [tool.poetry.dev-dependencies]
 tox = "^3.25.1"
 tox-poetry = "^0.4.1"
 pytest-black = "^0.3.12"
 pytest-isort = "^3.0.0"
 pytest-cov = "^3.0.0"
```

### Comparing `pytest-csv-params-1.0.0/pytest_csv_params/dialect.py` & `pytest_csv_params-1.1.0/pytest_csv_params/dialect.py`

 * *Files identical despite different names*

### Comparing `pytest-csv-params-1.0.0/pytest_csv_params/exception.py` & `pytest_csv_params-1.1.0/pytest_csv_params/exception.py`

 * *Files identical despite different names*

### Comparing `pytest-csv-params-1.0.0/pytest_csv_params/plugin.py` & `pytest_csv_params-1.1.0/pytest_csv_params/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-csv-params-1.0.0/pytest_csv_params/types.py` & `pytest_csv_params-1.1.0/pytest_csv_params/types.py`

 * *Files identical despite different names*

### Comparing `pytest-csv-params-1.0.0/setup.py` & `pytest_csv_params-1.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,233 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pytest-csv-params
+Version: 1.1.0
+Summary: Pytest plugin for Test Case Parametrization with CSV files
+Home-page: https://git.codebau.dev/pytest-plugins/pytest-csv-params
+License: MIT
+Keywords: py.test,pytest,csv,params,parametrize,pytest-plugin,ddt,data-driven
+Author: Juergen Edelbluth
+Author-email: csv_params@jued.de
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Environment :: Plugins
+Classifier: Framework :: Pytest
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Utilities
+Requires-Dist: pytest (>=7.4.0,<8.0.0)
+Project-URL: Changelog, https://docs.codebau.dev/pytest-plugins/pytest-csv-params/pages/changelog.html
+Project-URL: Documentation, https://docs.codebau.dev/pytest-plugins/pytest-csv-params/
+Project-URL: Issue Tracker, https://git.codebau.dev/pytest-plugins/pytest-csv-params/issues
+Project-URL: Repository, https://git.codebau.dev/pytest-plugins/pytest-csv-params
+Project-URL: Releases, https://git.codebau.dev/pytest-plugins/pytest-csv-params/releases
+Project-URL: Wiki, https://git.codebau.dev/pytest-plugins/pytest-csv-params/wiki
+Description-Content-Type: text/markdown
+
+![pytest-csv-params](https://docs.codebau.dev/pytest-plugins/pytest-csv-params/_images/pytest-csv-params.png)
+
+# pytest-csv-params
+
+A pytest plugin to parametrize data-driven tests by CSV files.
+
+[![Build Status](https://build.codebau.dev/buildStatus/icon?job=pytest-csv-params&style=flat)](https://git.codebau.dev/pytest-plugins/pytest-csv-params)
+[![PyPI - Downloads](https://img.shields.io/pypi/dw/pytest-csv-params?label=PyPI%20downloads&style=flat&logo=pypi)](https://pypi.org/project/pytest-csv-params/)
+[![PyPI - Version](https://img.shields.io/pypi/v/pytest-csv-params?label=PyPI%20version&style=flat&logo=pypi)](https://pypi.org/project/pytest-csv-params/)
+[![PyPI - Status](https://img.shields.io/pypi/status/pytest-csv-params?label=PyPI%20status&style=flat&logo=pypi)](https://pypi.org/project/pytest-csv-params/)
+[![PyPI - Format](https://img.shields.io/pypi/format/pytest-csv-params?label=PyPI%20format&style=flat&logo=pypi)](https://pypi.org/project/pytest-csv-params/)
+
+## Requirements
+ 
+- Python 3.8, 3.9, 3.10, 3.11
+- pytest >= 7.4
+
+There's no operating system dependent code in this plugin, so it should run anywhere where pytest runs.
+
+## Installation
+
+Simply install it with pip...
+
+```bash
+pip install pytest-csv-params
+```
+
+... or poetry ...
+
+```bash
+poetry add --dev pytest-csv-params
+```
+
+## Documentation / User Guide
+
+**Detailed documentation can be found under
+[docs.codebau.dev/pytest-plugins/pytest-csv-params/](https://docs.codebau.dev/pytest-plugins/pytest-csv-params/)**
+
+## Usage: Command Line Argument
+
+| Argument                | Required      | Description                                                          | Example                                      |
+|-------------------------|---------------|----------------------------------------------------------------------|----------------------------------------------|
+| `--csv-params-base-dir` | no (optional) | Define a base dir for all relative-path CSV data files (since 0.1.0) | `pytest --csv-params-base-dir /var/testdata` |
+
+## Usage: Decorator
+
+Simply decorate your test method with `@csv_params` (`pytest_csv_params.decorator.csv_params`) and the following parameters:
+
+| Parameter        | Type                     | Description                                                                                                                            | Example                                                                                        |
+|------------------|--------------------------|----------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------|
+| `data_file`      | `str`                    | The CSV file to use, relative or absolute path                                                                                         | `"/var/testdata/test1.csv"`                                                                    |
+| `base_dir`       | `str` (optional)         | Directory to look up relative CSV files (see `data_file`); overrides the command line argument                                         | `join(dirname(__file__), "assets")`                                                            |
+| `id_col`         | `str` (optional)         | Column name of the CSV that contains test case IDs                                                                                     | `"ID#"`                                                                                        |
+| `dialect`        | `csv.Dialect` (optional) | CSV Dialect definition (see [Python CSV Documentation](https://docs.python.org/3/library/csv.html#dialects-and-formatting-parameters)) | `csv.excel_tab`                                                                                |
+| `data_casts`     | `dict` (optional)        | Cast Methods for the CSV Data (see "Data Casting" below)                                                                               | `{ "a": int, "b": float }`                                                                     |
+| `header_renames` | `dict` (optional)        | Replace headers from the CSV file, so that they can be used as parameters for the test function (since 0.3.0)                          | `{ "Annual Amount of Bananas": "banana_count", "Cherry export price": "cherry_export_price" }` | 
+
+## CSV Format
+
+The default CSV format is:
+
+- `\r\n` as line ending
+- All non-numeric fields are surrounded by `"`
+- If you need a `"` in the value, use `""` (double quote)
+- Fields are separated by comma (`,`)
+
+## Usage Example
+
+This example uses the CSV example from above.
+
+```python
+from pytest_csv_params.decorator import csv_params
+
+@csv_params(
+    data_file="/data/test-lib/cases/addition.csv",
+    id_col="ID#",
+    data_casts={
+        "part_a": int,
+        "part_b": int,
+        "expected_result": int,
+    },
+)
+def test_addition(part_a, part_b, expected_result):
+    assert part_a + part_b == expected_result
+```
+
+Shorthand example (no ID col, only string values):
+
+```python
+from pytest_csv_params.decorator import csv_params
+
+@csv_params("/data/test-lib/cases/texts.csv")
+def test_texts(text_a, text_b, text_c):
+    assert f"{text_a}:{text_b}" == text_c
+```
+
+### More complex example
+
+This example features nearly all things the plugin has to offer. You find this example also in the test cases, see `tests/test_complex_example.py`.
+
+The CSV file (`tests/assets/example.csv`):
+
+```text
+"Test ID","Bananas shipped","Single Banana Weight","Apples shipped","Single Apple Weight","Container Size"
+"Order-7","1503","0.5","2545","0.25","1500"
+"Order-15","101","0.55","1474","0.33","550"
+```
+
+The Test (`tests/test_complex_example.py`):
+
+```python
+from math import ceil
+from os.path import join, dirname
+
+from pytest_csv_params.decorator import csv_params
+
+
+@csv_params(
+    data_file="example.csv",
+    base_dir=join(dirname(__file__), "assets"),
+    id_col="Test ID",
+    header_renames={
+        "Bananas shipped": "bananas_shipped",
+        "Single Banana Weight": "banana_weight",
+        "Apples shipped": "apples_shipped",
+        "Single Apple Weight": "apple_weight",
+        "Container Size": "container_size",
+    },
+    data_casts={
+        "bananas_shipped": int,
+        "banana_weight": float,
+        "apples_shipped": int,
+        "apple_weight": float,
+        "container_size": int,
+    },
+)
+def test_container_size_is_big_enough(
+    bananas_shipped: int, banana_weight: float, apples_shipped: int, apple_weight: float, container_size: int
+) -> None:
+    """
+    This is just an example test case for the documentation.
+    """
+
+    gross_weight = (banana_weight * bananas_shipped) + (apple_weight * apples_shipped)
+    assert ceil(gross_weight) <= container_size
+```
+
+If you decide not to rename the columns, the test would look like this:
+
+```python
+@csv_params(
+    data_file="example.csv",
+    base_dir=join(dirname(__file__), "assets"),
+    id_col="Test ID",
+    data_casts={
+        "Bananas_Shipped": int,
+        "Single_Banana_Weight": float,
+        "Apples_Shipped": int,
+        "Single_Apple_Weight": float,
+        "Container_Size": int,
+    },
+)
+def test_container_size_is_big_enough(
+    Bananas_Shipped: int, Single_Banana_Weight: float, Apples_Shipped: int, Single_Apple_Weight: float, Container_Size: int
+) -> None:
+    ...
+```
+
+## Changelog
+
+- A detailed changelog is here:
+  [docs.codebau.dev/pytest-plugins/pytest-csv-params/pages/changelog.html](https://docs.codebau.dev/pytest-plugins/pytest-csv-params/pages/changelog.html)
+
+## Bugs etc.
+
+Please send your issues to `csv-params_issues` (at) `jued.de`. Please include the following:
+
+- Plugin Version used
+- Pytest version
+- Python version with operating system
+
+It would be great if you could include example code that clarifies your issue.
+
+See [CONTRIBUTING.md](CONTRIBUTING.md) for details.
+
+## Pull Requests
+
+Pull requests are always welcome. Since this Gitea instance is not open to public, just send an e-mail to discuss options.
 
-packages = \
-['_ptcsvp', 'pytest_csv_params']
+Any changes that are made are to be backed by tests. Please give me a sign if you're going to break the existing API and let us discuss ways to handle that.
 
-package_data = \
-{'': ['*']}
+See [CONTRIBUTING.md](CONTRIBUTING.md) for details.
 
-install_requires = \
-['pytest>=7.1.2,<8.0.0']
-
-entry_points = \
-{'pytest11': ['pytest-csv-params = pytest_csv_params.plugin']}
-
-setup_kwargs = {
-    'name': 'pytest-csv-params',
-    'version': '1.0.0',
-    'description': 'Pytest plugin for Test Case Parametrization with CSV files',
-    'long_description': '![pytest-csv-params](https://docs.codebau.dev/pytest-plugins/pytest-csv-params/_images/pytest-csv-params.png)\n\n# pytest-csv-params\n\nA pytest plugin to parametrize data-driven tests by CSV files.\n\n[![Build Status](https://build.codebau.dev/buildStatus/icon?job=pytest-csv-params&style=flat)](https://git.codebau.dev/pytest-plugins/pytest-csv-params)\n[![PyPI - Downloads](https://img.shields.io/pypi/dw/pytest-csv-params?label=PyPI%20downloads&style=flat&logo=pypi)](https://pypi.org/project/pytest-csv-params/)\n[![PyPI - Version](https://img.shields.io/pypi/v/pytest-csv-params?label=PyPI%20version&style=flat&logo=pypi)](https://pypi.org/project/pytest-csv-params/)\n[![PyPI - Status](https://img.shields.io/pypi/status/pytest-csv-params?label=PyPI%20status&style=flat&logo=pypi)](https://pypi.org/project/pytest-csv-params/)\n[![PyPI - Format](https://img.shields.io/pypi/format/pytest-csv-params?label=PyPI%20format&style=flat&logo=pypi)](https://pypi.org/project/pytest-csv-params/)\n\n## Requirements\n \n- Python 3.8, 3.9 or 3.10\n- pytest >= 7.1\n\nThere\'s no operating system dependent code in this plugin, so it should run anywhere where pytest runs.\n\n## Installation\n\nSimply install it with pip...\n\n```bash\npip install pytest-csv-params\n```\n\n... or poetry ...\n\n```bash\npoetry add --dev pytest-csv-params\n```\n\n## Documentation / User Guide\n\n**Detailed documentation can be found under\n[docs.codebau.dev/pytest-plugins/pytest-csv-params/](https://docs.codebau.dev/pytest-plugins/pytest-csv-params/)**\n\n## Usage: Command Line Argument\n\n| Argument                | Required      | Description                                                          | Example                                      |\n|-------------------------|---------------|----------------------------------------------------------------------|----------------------------------------------|\n| `--csv-params-base-dir` | no (optional) | Define a base dir for all relative-path CSV data files (since 0.1.0) | `pytest --csv-params-base-dir /var/testdata` |\n\n## Usage: Decorator\n\nSimply decorate your test method with `@csv_params` (`pytest_csv_params.decorator.csv_params`) and the following parameters:\n\n| Parameter        | Type                     | Description                                                                                                                            | Example                                                                                        |\n|------------------|--------------------------|----------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------|\n| `data_file`      | `str`                    | The CSV file to use, relative or absolute path                                                                                         | `"/var/testdata/test1.csv"`                                                                    |\n| `base_dir`       | `str` (optional)         | Directory to look up relative CSV files (see `data_file`); overrides the command line argument                                         | `join(dirname(__file__), "assets")`                                                            |\n| `id_col`         | `str` (optional)         | Column name of the CSV that contains test case IDs                                                                                     | `"ID#"`                                                                                        |\n| `dialect`        | `csv.Dialect` (optional) | CSV Dialect definition (see [Python CSV Documentation](https://docs.python.org/3/library/csv.html#dialects-and-formatting-parameters)) | `csv.excel_tab`                                                                                |\n| `data_casts`     | `dict` (optional)        | Cast Methods for the CSV Data (see "Data Casting" below)                                                                               | `{ "a": int, "b": float }`                                                                     |\n| `header_renames` | `dict` (optional)        | Replace headers from the CSV file, so that they can be used as parameters for the test function (since 0.3.0)                          | `{ "Annual Amount of Bananas": "banana_count", "Cherry export price": "cherry_export_price" }` | \n\n## CSV Format\n\nThe default CSV format is:\n\n- `\\r\\n` as line ending\n- All non-numeric fields are surrounded by `"`\n- If you need a `"` in the value, use `""` (double quote)\n- Fields are separated by comma (`,`)\n\n## Usage Example\n\nThis example uses the CSV example from above.\n\n```python\nfrom pytest_csv_params.decorator import csv_params\n\n@csv_params(\n    data_file="/data/test-lib/cases/addition.csv",\n    id_col="ID#",\n    data_casts={\n        "part_a": int,\n        "part_b": int,\n        "expected_result": int,\n    },\n)\ndef test_addition(part_a, part_b, expected_result):\n    assert part_a + part_b == expected_result\n```\n\nShorthand example (no ID col, only string values):\n\n```python\nfrom pytest_csv_params.decorator import csv_params\n\n@csv_params("/data/test-lib/cases/texts.csv")\ndef test_texts(text_a, text_b, text_c):\n    assert f"{text_a}:{text_b}" == text_c\n```\n\n### More complex example\n\nThis example features nearly all things the plugin has to offer. You find this example also in the test cases, see `tests/test_complex_example.py`.\n\nThe CSV file (`tests/assets/example.csv`):\n\n```text\n"Test ID","Bananas shipped","Single Banana Weight","Apples shipped","Single Apple Weight","Container Size"\n"Order-7","1503","0.5","2545","0.25","1500"\n"Order-15","101","0.55","1474","0.33","550"\n```\n\nThe Test (`tests/test_complex_example.py`):\n\n```python\nfrom math import ceil\nfrom os.path import join, dirname\n\nfrom pytest_csv_params.decorator import csv_params\n\n\n@csv_params(\n    data_file="example.csv",\n    base_dir=join(dirname(__file__), "assets"),\n    id_col="Test ID",\n    header_renames={\n        "Bananas shipped": "bananas_shipped",\n        "Single Banana Weight": "banana_weight",\n        "Apples shipped": "apples_shipped",\n        "Single Apple Weight": "apple_weight",\n        "Container Size": "container_size",\n    },\n    data_casts={\n        "bananas_shipped": int,\n        "banana_weight": float,\n        "apples_shipped": int,\n        "apple_weight": float,\n        "container_size": int,\n    },\n)\ndef test_container_size_is_big_enough(\n    bananas_shipped: int, banana_weight: float, apples_shipped: int, apple_weight: float, container_size: int\n) -> None:\n    """\n    This is just an example test case for the documentation.\n    """\n\n    gross_weight = (banana_weight * bananas_shipped) + (apple_weight * apples_shipped)\n    assert ceil(gross_weight) <= container_size\n```\n\nIf you decide not to rename the columns, the test would look like this:\n\n```python\n@csv_params(\n    data_file="example.csv",\n    base_dir=join(dirname(__file__), "assets"),\n    id_col="Test ID",\n    data_casts={\n        "Bananas_Shipped": int,\n        "Single_Banana_Weight": float,\n        "Apples_Shipped": int,\n        "Single_Apple_Weight": float,\n        "Container_Size": int,\n    },\n)\ndef test_container_size_is_big_enough(\n    Bananas_Shipped: int, Single_Banana_Weight: float, Apples_Shipped: int, Single_Apple_Weight: float, Container_Size: int\n) -> None:\n    ...\n```\n\n## Changelog\n\n- A detailed changelog is here:\n  [docs.codebau.dev/pytest-plugins/pytest-csv-params/pages/changelog.html](https://docs.codebau.dev/pytest-plugins/pytest-csv-params/pages/changelog.html)\n\n## Bugs etc.\n\nPlease send your issues to `csv-params_issues` (at) `jued.de`. Please include the following:\n\n- Plugin Version used\n- Pytest version\n- Python version with operating system\n\nIt would be great if you could include example code that clarifies your issue.\n\nSee [CONTRIBUTING.md](CONTRIBUTING.md) for details.\n\n## Pull Requests\n\nPull requests are always welcome. Since this Gitea instance is not open to public, just send an e-mail to discuss options.\n\nAny changes that are made are to be backed by tests. Please give me a sign if you\'re going to break the existing API and let us discuss ways to handle that.\n\nSee [CONTRIBUTING.md](CONTRIBUTING.md) for details.\n\n## Where are the sources?\n\nThe source code is available under [git.codebau.dev/pytest-plugins/pytest-csv-params](https://git.codebau.dev/pytest-plugins/pytest-csv-params).\n',
-    'author': 'Juergen Edelbluth',
-    'author_email': 'csv_params@jued.de',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://git.codebau.dev/pytest-plugins/pytest-csv-params',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+## Where are the sources?
 
+The source code is available under [git.codebau.dev/pytest-plugins/pytest-csv-params](https://git.codebau.dev/pytest-plugins/pytest-csv-params).
 
-setup(**setup_kwargs)
```

