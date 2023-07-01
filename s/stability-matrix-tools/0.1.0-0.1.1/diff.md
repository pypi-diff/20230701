# Comparing `tmp/stability_matrix_tools-0.1.0.tar.gz` & `tmp/stability_matrix_tools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stability_matrix_tools-0.1.0.tar", max compression
+gzip compressed data, was "stability_matrix_tools-0.1.1.tar", max compression
```

## Comparing `stability_matrix_tools-0.1.0.tar` & `stability_matrix_tools-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0    35163 2023-06-30 22:15:25.032480 stability_matrix_tools-0.1.0/LICENSE
--rw-r--r--   0        0        0      530 2023-06-30 22:22:00.375969 stability_matrix_tools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       47 2023-06-30 22:15:24.995957 stability_matrix_tools-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-30 19:14:24.481835 stability_matrix_tools-0.1.0/src/stability_matrix_tools/__init__.py
--rw-r--r--   0        0        0     1322 2023-06-30 22:21:37.145999 stability_matrix_tools-0.1.0/src/stability_matrix_tools/b2.py
--rw-r--r--   0        0        0      163 2023-06-30 22:21:37.149999 stability_matrix_tools-0.1.0/src/stability_matrix_tools/main.py
--rw-r--r--   0        0        0        0 2023-06-30 19:29:16.679181 stability_matrix_tools-0.1.0/src/stability_matrix_tools/models/__init__.py
--rw-r--r--   0        0        0      422 2023-06-30 22:09:13.511327 stability_matrix_tools-0.1.0/src/stability_matrix_tools/models/settings.py
--rw-r--r--   0        0        0     1066 2023-06-30 22:21:37.143001 stability_matrix_tools-0.1.0/src/stability_matrix_tools/models/update_info.py
--rw-r--r--   0        0        0      325 2023-06-30 21:06:10.076637 stability_matrix_tools-0.1.0/src/stability_matrix_tools/models/version.py
--rw-r--r--   0        0        0     1634 2023-06-30 21:18:44.596055 stability_matrix_tools-0.1.0/src/stability_matrix_tools/progress.py
--rw-r--r--   0        0        0      468 2023-06-30 22:21:37.151998 stability_matrix_tools-0.1.0/src/stability_matrix_tools/updates.py
--rw-r--r--   0        0        0     2013 2023-06-30 21:23:45.959438 stability_matrix_tools-0.1.0/src/stability_matrix_tools/uploader.py
--rw-r--r--   0        0        0     1000 1970-01-01 00:00:00.000000 stability_matrix_tools-0.1.0/setup.py
--rw-r--r--   0        0        0      641 1970-01-01 00:00:00.000000 stability_matrix_tools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35163 2023-06-30 22:15:25.032480 stability_matrix_tools-0.1.1/LICENSE
+-rw-r--r--   0        0        0      570 2023-07-01 02:38:36.683325 stability_matrix_tools-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-06-30 22:15:24.995957 stability_matrix_tools-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 19:14:24.481835 stability_matrix_tools-0.1.1/src/stability_matrix_tools/__init__.py
+-rw-r--r--   0        0        0     1322 2023-06-30 22:21:37.145999 stability_matrix_tools-0.1.1/src/stability_matrix_tools/b2.py
+-rw-r--r--   0        0        0      163 2023-06-30 22:21:37.149999 stability_matrix_tools-0.1.1/src/stability_matrix_tools/main.py
+-rw-r--r--   0        0        0        0 2023-06-30 19:29:16.679181 stability_matrix_tools-0.1.1/src/stability_matrix_tools/models/__init__.py
+-rw-r--r--   0        0        0      422 2023-06-30 22:09:13.511327 stability_matrix_tools-0.1.1/src/stability_matrix_tools/models/settings.py
+-rw-r--r--   0        0        0     1066 2023-06-30 22:21:37.143001 stability_matrix_tools-0.1.1/src/stability_matrix_tools/models/update_info.py
+-rw-r--r--   0        0        0      325 2023-06-30 21:06:10.076637 stability_matrix_tools-0.1.1/src/stability_matrix_tools/models/version.py
+-rw-r--r--   0        0        0     1634 2023-06-30 21:18:44.596055 stability_matrix_tools-0.1.1/src/stability_matrix_tools/progress.py
+-rw-r--r--   0        0        0      283 2023-06-30 22:33:30.407517 stability_matrix_tools-0.1.1/src/stability_matrix_tools/signing.py
+-rw-r--r--   0        0        0      468 2023-06-30 22:21:37.151998 stability_matrix_tools-0.1.1/src/stability_matrix_tools/updates.py
+-rw-r--r--   0        0        0     2013 2023-06-30 21:23:45.959438 stability_matrix_tools-0.1.1/src/stability_matrix_tools/uploader.py
+-rw-r--r--   0        0        0     1047 1970-01-01 00:00:00.000000 stability_matrix_tools-0.1.1/setup.py
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 stability_matrix_tools-0.1.1/PKG-INFO
```

### Comparing `stability_matrix_tools-0.1.0/LICENSE` & `stability_matrix_tools-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.0/src/stability_matrix_tools/b2.py` & `stability_matrix_tools-0.1.1/src/stability_matrix_tools/b2.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.0/src/stability_matrix_tools/models/update_info.py` & `stability_matrix_tools-0.1.1/src/stability_matrix_tools/models/update_info.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.0/src/stability_matrix_tools/progress.py` & `stability_matrix_tools-0.1.1/src/stability_matrix_tools/progress.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.0/src/stability_matrix_tools/uploader.py` & `stability_matrix_tools-0.1.1/src/stability_matrix_tools/uploader.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.0/setup.py` & `stability_matrix_tools-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,26 +8,27 @@
 ['stability_matrix_tools', 'stability_matrix_tools.models']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['b2sdk>=1.21.0,<2.0.0',
+ 'cryptography>=41.0.1,<42.0.0',
  'httpx>=0.24.1,<0.25.0',
  'pydantic[dotenv]>=2.0,<3.0',
  'python-dotenv>=1.0.0,<2.0.0',
  'semver>=3.0.1,<4.0.0',
  'typer[all]>=0.9.0,<0.10.0']
 
 entry_points = \
-{'console_scripts': ['sm-tools = sm_tools.main:app']}
+{'console_scripts': ['sm-tools = stability_matrix_tools.main:app']}
 
 setup_kwargs = {
     'name': 'stability-matrix-tools',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': '# sm-tools\n Stability Matrix development tools\n',
     'author': 'Ionite',
     'author_email': 'dev@ionite.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `stability_matrix_tools-0.1.0/PKG-INFO` & `stability_matrix_tools-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: stability-matrix-tools
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Ionite
 Author-email: dev@ionite.io
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: b2sdk (>=1.21.0,<2.0.0)
+Requires-Dist: cryptography (>=41.0.1,<42.0.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: pydantic[dotenv] (>=2.0,<3.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: semver (>=3.0.1,<4.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
```

