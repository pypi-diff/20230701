# Comparing `tmp/stability_matrix_tools-0.1.3.tar.gz` & `tmp/stability_matrix_tools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stability_matrix_tools-0.1.3.tar", max compression
+gzip compressed data, was "stability_matrix_tools-0.1.4.tar", max compression
```

## Comparing `stability_matrix_tools-0.1.3.tar` & `stability_matrix_tools-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0    35163 2023-06-30 22:15:25.032480 stability_matrix_tools-0.1.3/LICENSE
--rw-r--r--   0        0        0      570 2023-07-01 04:34:03.473785 stability_matrix_tools-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       47 2023-06-30 22:15:24.995957 stability_matrix_tools-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-06-30 19:14:24.481835 stability_matrix_tools-0.1.3/src/stability_matrix_tools/__init__.py
--rw-r--r--   0        0        0     2329 2023-07-01 03:50:14.086249 stability_matrix_tools-0.1.3/src/stability_matrix_tools/b2.py
--rw-r--r--   0        0        0      380 2023-07-01 04:29:55.594056 stability_matrix_tools-0.1.3/src/stability_matrix_tools/cf.py
--rw-r--r--   0        0        0      201 2023-07-01 03:57:29.403922 stability_matrix_tools-0.1.3/src/stability_matrix_tools/main.py
--rw-r--r--   0        0        0        0 2023-06-30 19:29:16.679181 stability_matrix_tools-0.1.3/src/stability_matrix_tools/models/__init__.py
--rw-r--r--   0        0        0      518 2023-07-01 03:35:42.001028 stability_matrix_tools-0.1.3/src/stability_matrix_tools/models/settings.py
--rw-r--r--   0        0        0     1007 2023-07-01 03:25:17.677979 stability_matrix_tools-0.1.3/src/stability_matrix_tools/models/update_info.py
--rw-r--r--   0        0        0      325 2023-06-30 21:06:10.076637 stability_matrix_tools-0.1.3/src/stability_matrix_tools/models/version.py
--rw-r--r--   0        0        0      608 2023-07-01 03:12:38.918254 stability_matrix_tools-0.1.3/src/stability_matrix_tools/updates.py
--rw-r--r--   0        0        0        0 2023-07-01 02:42:39.117279 stability_matrix_tools-0.1.3/src/stability_matrix_tools/utils/__init__.py
--rw-r--r--   0        0        0      588 2023-07-01 04:29:34.632450 stability_matrix_tools-0.1.3/src/stability_matrix_tools/utils/cf_cache.py
--rw-r--r--   0        0        0     1634 2023-06-30 21:18:44.596055 stability_matrix_tools-0.1.3/src/stability_matrix_tools/utils/progress.py
--rw-r--r--   0        0        0      283 2023-06-30 22:33:30.407517 stability_matrix_tools-0.1.3/src/stability_matrix_tools/utils/signing.py
--rw-r--r--   0        0        0     2013 2023-06-30 21:23:45.959438 stability_matrix_tools-0.1.3/src/stability_matrix_tools/utils/uploader.py
--rw-r--r--   0        0        0     1081 1970-01-01 00:00:00.000000 stability_matrix_tools-0.1.3/setup.py
--rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 stability_matrix_tools-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35163 2023-06-30 22:15:25.032480 stability_matrix_tools-0.1.4/LICENSE
+-rw-r--r--   0        0        0      613 2023-07-01 06:53:37.882121 stability_matrix_tools-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-06-30 22:15:24.995957 stability_matrix_tools-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 19:14:24.481835 stability_matrix_tools-0.1.4/src/stability_matrix_tools/__init__.py
+-rw-r--r--   0        0        0     2329 2023-07-01 03:50:14.086249 stability_matrix_tools-0.1.4/src/stability_matrix_tools/b2.py
+-rw-r--r--   0        0        0      380 2023-07-01 04:29:55.594056 stability_matrix_tools-0.1.4/src/stability_matrix_tools/cf.py
+-rw-r--r--   0        0        0     1651 2023-07-01 06:42:39.528859 stability_matrix_tools-0.1.4/src/stability_matrix_tools/keys.py
+-rw-r--r--   0        0        0      245 2023-07-01 06:42:59.756522 stability_matrix_tools-0.1.4/src/stability_matrix_tools/main.py
+-rw-r--r--   0        0        0        0 2023-06-30 19:29:16.679181 stability_matrix_tools-0.1.4/src/stability_matrix_tools/models/__init__.py
+-rw-r--r--   0        0        0      518 2023-07-01 03:35:42.001028 stability_matrix_tools-0.1.4/src/stability_matrix_tools/models/settings.py
+-rw-r--r--   0        0        0     1476 2023-07-01 05:27:21.614780 stability_matrix_tools-0.1.4/src/stability_matrix_tools/models/update_info.py
+-rw-r--r--   0        0        0      325 2023-06-30 21:06:10.076637 stability_matrix_tools-0.1.4/src/stability_matrix_tools/models/version.py
+-rw-r--r--   0        0        0      707 2023-07-01 05:33:17.097804 stability_matrix_tools-0.1.4/src/stability_matrix_tools/updates.py
+-rw-r--r--   0        0        0        0 2023-07-01 02:42:39.117279 stability_matrix_tools-0.1.4/src/stability_matrix_tools/utils/__init__.py
+-rw-r--r--   0        0        0      588 2023-07-01 04:29:34.632450 stability_matrix_tools-0.1.4/src/stability_matrix_tools/utils/cf_cache.py
+-rw-r--r--   0        0        0     1634 2023-06-30 21:18:44.596055 stability_matrix_tools-0.1.4/src/stability_matrix_tools/utils/progress.py
+-rw-r--r--   0        0        0     1963 2023-07-01 06:48:02.174520 stability_matrix_tools-0.1.4/src/stability_matrix_tools/utils/signing.py
+-rw-r--r--   0        0        0     2013 2023-06-30 21:23:45.959438 stability_matrix_tools-0.1.4/src/stability_matrix_tools/utils/uploader.py
+-rw-r--r--   0        0        0     1137 1970-01-01 00:00:00.000000 stability_matrix_tools-0.1.4/setup.py
+-rw-r--r--   0        0        0      772 1970-01-01 00:00:00.000000 stability_matrix_tools-0.1.4/PKG-INFO
```

### Comparing `stability_matrix_tools-0.1.3/LICENSE` & `stability_matrix_tools-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.3/pyproject.toml` & `stability_matrix_tools-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tool.poetry]
 name = "stability-matrix-tools"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Ionite <dev@ionite.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.12"
 typer = {extras = ["all"], version = "^0.9.0"}
 pydantic = {extras = ["dotenv"], version = "^2.0"}
 semver = "^3.0.1"
 httpx = "^0.24.1"
 b2sdk = "^1.21.0"
 python-dotenv = "^1.0.0"
 cryptography = "^41.0.1"
+keyring = "^24.2.0"
+pyperclip = "^1.8.2"
 
 [tool.poetry.scripts]
 sm-tools = "stability_matrix_tools.main:app"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `stability_matrix_tools-0.1.3/src/stability_matrix_tools/b2.py` & `stability_matrix_tools-0.1.4/src/stability_matrix_tools/b2.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.3/src/stability_matrix_tools/models/settings.py` & `stability_matrix_tools-0.1.4/src/stability_matrix_tools/models/settings.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.3/src/stability_matrix_tools/utils/cf_cache.py` & `stability_matrix_tools-0.1.4/src/stability_matrix_tools/utils/cf_cache.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.3/src/stability_matrix_tools/utils/progress.py` & `stability_matrix_tools-0.1.4/src/stability_matrix_tools/utils/progress.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.3/src/stability_matrix_tools/utils/uploader.py` & `stability_matrix_tools-0.1.4/src/stability_matrix_tools/utils/uploader.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.3/setup.py` & `stability_matrix_tools-0.1.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,25 +12,27 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['b2sdk>=1.21.0,<2.0.0',
  'cryptography>=41.0.1,<42.0.0',
  'httpx>=0.24.1,<0.25.0',
+ 'keyring>=24.2.0,<25.0.0',
  'pydantic[dotenv]>=2.0,<3.0',
+ 'pyperclip>=1.8.2,<2.0.0',
  'python-dotenv>=1.0.0,<2.0.0',
  'semver>=3.0.1,<4.0.0',
  'typer[all]>=0.9.0,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['sm-tools = stability_matrix_tools.main:app']}
 
 setup_kwargs = {
     'name': 'stability-matrix-tools',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': '',
     'long_description': '# sm-tools\n Stability Matrix development tools\n',
     'author': 'Ionite',
     'author_email': 'dev@ionite.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `stability_matrix_tools-0.1.3/PKG-INFO` & `stability_matrix_tools-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: stability-matrix-tools
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Ionite
 Author-email: dev@ionite.io
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: b2sdk (>=1.21.0,<2.0.0)
 Requires-Dist: cryptography (>=41.0.1,<42.0.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
+Requires-Dist: keyring (>=24.2.0,<25.0.0)
 Requires-Dist: pydantic[dotenv] (>=2.0,<3.0)
+Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: semver (>=3.0.1,<4.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # sm-tools
  Stability Matrix development tools
```

