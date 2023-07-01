# Comparing `tmp/edgetest-2023.6.0.tar.gz` & `tmp/edgetest-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgetest-2023.6.0.tar", last modified: Mon Jun  5 18:07:04 2023, max compression
+gzip compressed data, was "edgetest-2023.6.1.tar", last modified: Sat Jul  1 14:42:58 2023, max compression
```

## Comparing `edgetest-2023.6.0.tar` & `edgetest-2023.6.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:07:04.553540 edgetest-2023.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-05 18:06:33.000000 edgetest-2023.6.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 18:06:33.000000 edgetest-2023.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-05 18:06:33.000000 edgetest-2023.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-06-05 18:07:04.553540 edgetest-2023.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-06-05 18:06:33.000000 edgetest-2023.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:07:04.553540 edgetest-2023.6.0/edgetest/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-05 18:06:33.000000 edgetest-2023.6.0/edgetest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-06-05 18:06:33.000000 edgetest-2023.6.0/edgetest/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-05 18:06:33.000000 edgetest-2023.6.0/edgetest/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-05 18:06:33.000000 edgetest-2023.6.0/edgetest/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-05 18:06:33.000000 edgetest-2023.6.0/edgetest/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-05 18:06:33.000000 edgetest-2023.6.0/edgetest/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-05 18:06:33.000000 edgetest-2023.6.0/edgetest/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-05 18:06:33.000000 edgetest-2023.6.0/edgetest/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    16186 2023-06-05 18:06:33.000000 edgetest-2023.6.0/edgetest/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:07:04.553540 edgetest-2023.6.0/edgetest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-06-05 18:07:04.000000 edgetest-2023.6.0/edgetest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-05 18:07:04.000000 edgetest-2023.6.0/edgetest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 18:07:04.000000 edgetest-2023.6.0/edgetest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-05 18:07:04.000000 edgetest-2023.6.0/edgetest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 18:06:37.000000 edgetest-2023.6.0/edgetest.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-05 18:07:04.000000 edgetest-2023.6.0/edgetest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-05 18:07:04.000000 edgetest-2023.6.0/edgetest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-05 18:06:33.000000 edgetest-2023.6.0/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-05 18:06:33.000000 edgetest-2023.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-05 18:07:04.557540 edgetest-2023.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-05 18:06:33.000000 edgetest-2023.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:07:04.553540 edgetest-2023.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:06:33.000000 edgetest-2023.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-05 18:06:33.000000 edgetest-2023.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-06-05 18:06:33.000000 edgetest-2023.6.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-05 18:06:33.000000 edgetest-2023.6.0/tests/test_integration_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-06-05 18:06:33.000000 edgetest-2023.6.0/tests/test_integration_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-06-05 18:06:33.000000 edgetest-2023.6.0/tests/test_interface_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12701 2023-06-05 18:06:33.000000 edgetest-2023.6.0/tests/test_interface_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-05 18:06:33.000000 edgetest-2023.6.0/tests/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-05 18:06:33.000000 edgetest-2023.6.0/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-05 18:06:33.000000 edgetest-2023.6.0/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    11553 2023-06-05 18:06:33.000000 edgetest-2023.6.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:42:58.772712 edgetest-2023.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-01 14:42:30.000000 edgetest-2023.6.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-01 14:42:30.000000 edgetest-2023.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-01 14:42:30.000000 edgetest-2023.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-07-01 14:42:58.772712 edgetest-2023.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-07-01 14:42:30.000000 edgetest-2023.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:42:58.768712 edgetest-2023.6.1/edgetest/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-01 14:42:30.000000 edgetest-2023.6.1/edgetest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-07-01 14:42:30.000000 edgetest-2023.6.1/edgetest/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-07-01 14:42:30.000000 edgetest-2023.6.1/edgetest/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-01 14:42:30.000000 edgetest-2023.6.1/edgetest/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-01 14:42:30.000000 edgetest-2023.6.1/edgetest/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-01 14:42:30.000000 edgetest-2023.6.1/edgetest/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-01 14:42:30.000000 edgetest-2023.6.1/edgetest/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-01 14:42:30.000000 edgetest-2023.6.1/edgetest/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16729 2023-07-01 14:42:30.000000 edgetest-2023.6.1/edgetest/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:42:58.768712 edgetest-2023.6.1/edgetest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-07-01 14:42:58.000000 edgetest-2023.6.1/edgetest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-01 14:42:58.000000 edgetest-2023.6.1/edgetest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 14:42:58.000000 edgetest-2023.6.1/edgetest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-01 14:42:58.000000 edgetest-2023.6.1/edgetest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 14:42:33.000000 edgetest-2023.6.1/edgetest.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-01 14:42:58.000000 edgetest-2023.6.1/edgetest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-01 14:42:58.000000 edgetest-2023.6.1/edgetest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-01 14:42:30.000000 edgetest-2023.6.1/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-01 14:42:30.000000 edgetest-2023.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-01 14:42:58.772712 edgetest-2023.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-01 14:42:30.000000 edgetest-2023.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:42:58.772712 edgetest-2023.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 14:42:30.000000 edgetest-2023.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-01 14:42:30.000000 edgetest-2023.6.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-07-01 14:42:30.000000 edgetest-2023.6.1/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-01 14:42:30.000000 edgetest-2023.6.1/tests/test_integration_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-01 14:42:30.000000 edgetest-2023.6.1/tests/test_integration_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-07-01 14:42:30.000000 edgetest-2023.6.1/tests/test_interface_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12701 2023-07-01 14:42:30.000000 edgetest-2023.6.1/tests/test_interface_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-01 14:42:30.000000 edgetest-2023.6.1/tests/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-01 14:42:30.000000 edgetest-2023.6.1/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-01 14:42:30.000000 edgetest-2023.6.1/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-07-01 14:42:30.000000 edgetest-2023.6.1/tests/test_utils.py
```

### Comparing `edgetest-2023.6.0/LICENSE` & `edgetest-2023.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edgetest-2023.6.0/PKG-INFO` & `edgetest-2023.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgetest
-Version: 2023.6.0
+Version: 2023.6.1
 Summary: Bleeding edge dependency testing
 Home-page: https://github.com/capitalone/edgetest
 Author: Akshay Gupta
 Author-email: akshay.gupta2@capitalone.com
 Maintainer: Akshay Gupta
 Maintainer-email: akshay.gupta2@capitalone.com
 License: Apache Software License
@@ -13,18 +13,18 @@
 Project-URL: Source Code, https://github.com/capitalone/edgetest
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: qa
 Provides-Extra: build
 Provides-Extra: dev
 License-File: LICENSE
@@ -69,15 +69,15 @@
 - [Contributing](#contributing)
 - [License](#license)
 - [Roadmap](#roadmap)
 
 Install
 -------
 
-Create a ``conda`` environment with Python 3.7+ and install from PyPI:
+Create a ``conda`` environment with Python 3.8+ and install from PyPI:
 
 ```console
 $ python -m pip install edgetest
 ```
 
 or conda-forge:
```

### Comparing `edgetest-2023.6.0/README.md` & `edgetest-2023.6.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 - [Contributing](#contributing)
 - [License](#license)
 - [Roadmap](#roadmap)
 
 Install
 -------
 
-Create a ``conda`` environment with Python 3.7+ and install from PyPI:
+Create a ``conda`` environment with Python 3.8+ and install from PyPI:
 
 ```console
 $ python -m pip install edgetest
 ```
 
 or conda-forge:
```

### Comparing `edgetest-2023.6.0/edgetest/core.py` & `edgetest-2023.6.1/edgetest/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 from subprocess import Popen
 from typing import Dict, List, Optional
 
 from pluggy._hooks import _HookRelay
 
 from .logger import get_logger
-from .utils import _run_command, pushd
+from .utils import _isin_case_dashhyphen_ins, _run_command, pushd
 
 LOG = get_logger(__name__)
 
 
 class TestPackage:
     """Run test commands with bleeding edge dependencies.
 
@@ -145,15 +145,19 @@
             for this environment.
         """
         # Get the version for the upgraded package(s)
         out, _ = _run_command(self.python_path, "-m", "pip", "list", "--format", "json")
         outjson = json.loads(out)
 
         upgrade_wo_extras = [pkg.split("[")[0] for pkg in self.upgrade]
-        return [pkg for pkg in outjson if pkg.get("name", "") in upgrade_wo_extras]
+        return [
+            pkg
+            for pkg in outjson
+            if _isin_case_dashhyphen_ins(pkg.get("name", ""), upgrade_wo_extras)
+        ]
 
     def run_tests(self, command: str) -> int:
         """Run the tests in the package directory.
 
         Parameters
         ----------
         command : str
```

### Comparing `edgetest-2023.6.0/edgetest/hookspecs.py` & `edgetest-2023.6.1/edgetest/hookspecs.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.6.0/edgetest/interface.py` & `edgetest-2023.6.1/edgetest/interface.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.6.0/edgetest/lib.py` & `edgetest-2023.6.1/edgetest/lib.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.6.0/edgetest/logger.py` & `edgetest-2023.6.1/edgetest/logger.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.6.0/edgetest/report.py` & `edgetest-2023.6.1/edgetest/report.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.6.0/edgetest/schema.py` & `edgetest-2023.6.1/edgetest/schema.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.6.0/edgetest/utils.py` & `edgetest-2023.6.1/edgetest/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -475,7 +475,28 @@
             upgraded = upgrade_requirements(
                 fname_or_buf="\n".join(dependencies),
                 upgraded_packages=upgraded_packages,
             )
             parser["project"]["optional-dependencies"][extra] = upgraded.split("\n")  # type: ignore
 
     return parser
+
+
+def _isin_case_dashhyphen_ins(a: str, vals: List[str]) -> bool:
+    """Run isin check that is case and dash/hyphen insensitive.
+
+    Paramaters
+    ----------
+    a : str
+        String value to check for membership against ``vals``.
+    vals : list of str
+        List of strings to check ``a`` against.
+
+    Returns
+    -------
+    bool
+        Return ``True`` if ``a`` in vals, otherwise ``False``.
+    """
+    for b in vals:
+        if a.replace("_", "-").lower() == b.replace("_", "-").lower():
+            return True
+    return False
```

### Comparing `edgetest-2023.6.0/edgetest.egg-info/PKG-INFO` & `edgetest-2023.6.1/edgetest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgetest
-Version: 2023.6.0
+Version: 2023.6.1
 Summary: Bleeding edge dependency testing
 Home-page: https://github.com/capitalone/edgetest
 Author: Akshay Gupta
 Author-email: akshay.gupta2@capitalone.com
 Maintainer: Akshay Gupta
 Maintainer-email: akshay.gupta2@capitalone.com
 License: Apache Software License
@@ -13,18 +13,18 @@
 Project-URL: Source Code, https://github.com/capitalone/edgetest
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: qa
 Provides-Extra: build
 Provides-Extra: dev
 License-File: LICENSE
@@ -69,15 +69,15 @@
 - [Contributing](#contributing)
 - [License](#license)
 - [Roadmap](#roadmap)
 
 Install
 -------
 
-Create a ``conda`` environment with Python 3.7+ and install from PyPI:
+Create a ``conda`` environment with Python 3.8+ and install from PyPI:
 
 ```console
 $ python -m pip install edgetest
 ```
 
 or conda-forge:
```

### Comparing `edgetest-2023.6.0/edgetest.egg-info/SOURCES.txt` & `edgetest-2023.6.1/edgetest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edgetest-2023.6.0/edgetest.egg-info/requires.txt` & `edgetest-2023.6.1/edgetest.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `edgetest-2023.6.0/pull_request_template.md` & `edgetest-2023.6.1/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `edgetest-2023.6.0/requirements.txt` & `edgetest-2023.6.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `edgetest-2023.6.0/setup.cfg` & `edgetest-2023.6.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 author = Akshay Gupta
 author_email = akshay.gupta2@capitalone.com
 license = Apache Software License
 maintainer = Akshay Gupta
 maintainer_email = akshay.gupta2@capitalone.com
 url = https://github.com/capitalone/edgetest
 python_requires = 
-	>=3.7.0
+	>=3.8.0
 project_urls = 
 	Documentation = https://capitalone.github.io/edgetest/
 	Bug Tracker = https://github.com/capitalone/edgetest/issues
 	Source Code = https://github.com/capitalone/edgetest
 classifiers = 
 	Intended Audience :: Developers
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
 	Cerberus<=1.3.4,>=1.3.0
@@ -96,15 +96,15 @@
 	bumpver
 
 [options.entry_points]
 console_scripts = 
 	edgetest = edgetest.interface:cli
 
 [bumpver]
-current_version = "2023.6.0"
+current_version = "2023.6.1"
 version_pattern = "YYYY.MM.INC0"
 commit_message = "Bump {old_version} to {new_version}"
 commit = True
 
 [bumpver:file_patterns]
 docs/source/conf.py = 
 	version = "{version}"
```

### Comparing `edgetest-2023.6.0/tests/conftest.py` & `edgetest-2023.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.6.0/tests/test_core.py` & `edgetest-2023.6.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.6.0/tests/test_integration_cfg.py` & `edgetest-2023.6.1/tests/test_integration_cfg.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,27 +42,27 @@
     >=3.7.0
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires =
-    click<=8.0.0,>=7.1
+    scikit-learn>=1.0,<=1.2.0
     dask[dataframe]<=2022.1.0
 
 [options.extras_require]
 tests =
     pytest
 
 [edgetest.envs.core]
 extras =
     tests
 upgrade =
-    click
-    dask[dataframe]
+    Scikit_Learn
+    Dask[DataFrame]
 """
 
 
 SETUP_PY = """
 from setuptools import setup
 
 setup()
@@ -105,14 +105,15 @@
 
         # Run the CLI
         result = runner.invoke(cli, ["--config=setup.cfg"])
 
         assert result.exit_code == 0
         assert Path(loc, ".edgetest").is_dir()
         assert Path(loc, ".edgetest", "pandas").is_dir()
+        assert "pandas" in result.stdout
 
         if not sys.platform == "win32":
             assert Path(
                 loc, ".edgetest", "pandas", "lib", PY_VER, "site-packages", "pandas"
             ).is_dir()
 
 
@@ -146,17 +147,19 @@
             assert Path(
                 loc, ".edgetest", "core", "lib", PY_VER, "site-packages", "dask"
             ).is_dir()
             assert Path(
                 loc, ".edgetest", "core", "lib", PY_VER, "site-packages", "pandas"
             ).is_dir()
             assert Path(
-                loc, ".edgetest", "core", "lib", PY_VER, "site-packages", "click"
+                loc, ".edgetest", "core", "lib", PY_VER, "site-packages", "sklearn"
             ).is_dir()
 
         config = configparser.ConfigParser()
         config.read("setup.cfg")
 
-        assert "click" in config["options"]["install_requires"]
+        assert "scikit-learn" in config["options"]["install_requires"]
         assert "dask[dataframe]" in config["options"]["install_requires"]
         assert config["edgetest.envs.core"]["extras"] == "\ntests"
-        assert config["edgetest.envs.core"]["upgrade"] == "\nclick\ndask[dataframe]"
+        assert config["edgetest.envs.core"]["upgrade"] == "\nScikit_Learn\nDask[DataFrame]"
+        assert "dask" in result.stdout
+        assert "scikit-learn" in result.stdout
```

### Comparing `edgetest-2023.6.0/tests/test_integration_toml.py` & `edgetest-2023.6.1/tests/test_integration_toml.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,22 +27,22 @@
 
 SETUP_TOML_DASK = """
 [project]
 name = "toy_package"
 version = "0.1.0"
 description = "Fake description"
 requires-python = ">=3.7.0"
-dependencies = ["click<=8.0.0,>=7.1", "dask[dataframe]<=2022.1.0"]
+dependencies = ["Scikit_Learn>=1.0,<=1.2.0", "Dask[dataframe]<=2022.1.0"]
 
 [project.optional-dependencies]
 tests = ["pytest"]
 
 [edgetest.envs.core]
 extras = ["tests"]
-upgrade = ["click", "dask[dataframe]"]
+upgrade = ["scikit-learn", "dask[dataframe]"]
 """
 
 
 SETUP_PY = """
 from setuptools import setup
 
 setup()
@@ -85,14 +85,15 @@
 
         # Run the CLI
         result = runner.invoke(cli, ["--config=pyproject.toml"])
 
         assert result.exit_code == 0
         assert Path(loc, ".edgetest").is_dir()
         assert Path(loc, ".edgetest", "pandas").is_dir()
+        assert "pandas" in result.stdout
 
         if not sys.platform == "win32":
             assert Path(
                 loc, ".edgetest", "pandas", "lib", PY_VER, "site-packages", "pandas"
             ).is_dir()
 
 
@@ -126,19 +127,21 @@
             assert Path(
                 loc, ".edgetest", "core", "lib", PY_VER, "site-packages", "dask"
             ).is_dir()
             assert Path(
                 loc, ".edgetest", "core", "lib", PY_VER, "site-packages", "pandas"
             ).is_dir()
             assert Path(
-                loc, ".edgetest", "core", "lib", PY_VER, "site-packages", "click"
+                loc, ".edgetest", "core", "lib", PY_VER, "site-packages", "sklearn"
             ).is_dir()
 
         config = load(open("pyproject.toml"))
 
-        assert "click" in config["project"]["dependencies"][0]
-        assert "dask" in config["project"]["dependencies"][1]
+        assert "Scikit_Learn" in config["project"]["dependencies"][0]
+        assert "Dask" in config["project"]["dependencies"][1]
         assert config["edgetest"]["envs"]["core"]["extras"] == ["tests"]
         assert config["edgetest"]["envs"]["core"]["upgrade"] == [
-            "click",
+            "scikit-learn",
             "dask[dataframe]",
         ]
+        assert "dask" in result.stdout
+        assert "scikit-learn" in result.stdout
```

### Comparing `edgetest-2023.6.0/tests/test_interface_cfg.py` & `edgetest-2023.6.1/tests/test_interface_cfg.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.6.0/tests/test_interface_toml.py` & `edgetest-2023.6.1/tests/test_interface_toml.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.6.0/tests/test_lib.py` & `edgetest-2023.6.1/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.6.0/tests/test_report.py` & `edgetest-2023.6.1/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.6.0/tests/test_schema.py` & `edgetest-2023.6.1/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `edgetest-2023.6.0/tests/test_utils.py` & `edgetest-2023.6.1/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from edgetest.utils import (
     _convert_toml_array_to_string,
     gen_requirements_config,
     parse_cfg,
     parse_toml,
     upgrade_pyproject_toml,
     upgrade_setup_cfg,
+    _isin_case_dashhyphen_ins,
 )
 
 REQS = """
 mydep1>=0.1.0,<=0.2.0
 mydep2<=0.10.0
 """
 
@@ -477,7 +478,19 @@
         filename=conf_loc,
     ) == {
         "project": {
             "dependencies": ["pandas<=2.0.0,>=1.0.0", "numpy<=3.0.0,>=1.0.0"],
             "optional-dependencies": {"tests": ["pytest<=4.0.0,>=1.0.0"]},
         }
     }
+
+
+def test_isin_case_dashhyphen_ins():
+    vals = ["pandas", "python-dateutil"]
+
+    assert _isin_case_dashhyphen_ins("pandas", vals)
+    assert _isin_case_dashhyphen_ins("Pandas", vals)
+    assert not _isin_case_dashhyphen_ins("Panda$", vals)
+    assert _isin_case_dashhyphen_ins("python-dateutil", vals)
+    assert _isin_case_dashhyphen_ins("Python_Dateutil", vals)
+    assert not _isin_case_dashhyphen_ins("Python_Dateut1l", vals)
+    assert not _isin_case_dashhyphen_ins("pandaspython-dateutil", vals)
```

