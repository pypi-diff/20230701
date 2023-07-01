# Comparing `tmp/stability_matrix_tools-0.1.1.tar.gz` & `tmp/stability_matrix_tools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stability_matrix_tools-0.1.1.tar", max compression
+gzip compressed data, was "stability_matrix_tools-0.1.2.tar", max compression
```

## Comparing `stability_matrix_tools-0.1.1.tar` & `stability_matrix_tools-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0    35163 2023-06-30 22:15:25.032480 stability_matrix_tools-0.1.1/LICENSE
--rw-r--r--   0        0        0      570 2023-07-01 02:38:36.683325 stability_matrix_tools-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       47 2023-06-30 22:15:24.995957 stability_matrix_tools-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-30 19:14:24.481835 stability_matrix_tools-0.1.1/src/stability_matrix_tools/__init__.py
--rw-r--r--   0        0        0     1322 2023-06-30 22:21:37.145999 stability_matrix_tools-0.1.1/src/stability_matrix_tools/b2.py
--rw-r--r--   0        0        0      163 2023-06-30 22:21:37.149999 stability_matrix_tools-0.1.1/src/stability_matrix_tools/main.py
--rw-r--r--   0        0        0        0 2023-06-30 19:29:16.679181 stability_matrix_tools-0.1.1/src/stability_matrix_tools/models/__init__.py
--rw-r--r--   0        0        0      422 2023-06-30 22:09:13.511327 stability_matrix_tools-0.1.1/src/stability_matrix_tools/models/settings.py
--rw-r--r--   0        0        0     1066 2023-06-30 22:21:37.143001 stability_matrix_tools-0.1.1/src/stability_matrix_tools/models/update_info.py
--rw-r--r--   0        0        0      325 2023-06-30 21:06:10.076637 stability_matrix_tools-0.1.1/src/stability_matrix_tools/models/version.py
--rw-r--r--   0        0        0     1634 2023-06-30 21:18:44.596055 stability_matrix_tools-0.1.1/src/stability_matrix_tools/progress.py
--rw-r--r--   0        0        0      283 2023-06-30 22:33:30.407517 stability_matrix_tools-0.1.1/src/stability_matrix_tools/signing.py
--rw-r--r--   0        0        0      468 2023-06-30 22:21:37.151998 stability_matrix_tools-0.1.1/src/stability_matrix_tools/updates.py
--rw-r--r--   0        0        0     2013 2023-06-30 21:23:45.959438 stability_matrix_tools-0.1.1/src/stability_matrix_tools/uploader.py
--rw-r--r--   0        0        0     1047 1970-01-01 00:00:00.000000 stability_matrix_tools-0.1.1/setup.py
--rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 stability_matrix_tools-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35163 2023-06-30 22:15:25.032480 stability_matrix_tools-0.1.2/LICENSE
+-rw-r--r--   0        0        0      570 2023-07-01 02:56:17.563524 stability_matrix_tools-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-06-30 22:15:24.995957 stability_matrix_tools-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 19:14:24.481835 stability_matrix_tools-0.1.2/src/stability_matrix_tools/__init__.py
+-rw-r--r--   0        0        0     2068 2023-07-01 02:54:27.607757 stability_matrix_tools-0.1.2/src/stability_matrix_tools/b2.py
+-rw-r--r--   0        0        0      163 2023-06-30 22:21:37.149999 stability_matrix_tools-0.1.2/src/stability_matrix_tools/main.py
+-rw-r--r--   0        0        0        0 2023-06-30 19:29:16.679181 stability_matrix_tools-0.1.2/src/stability_matrix_tools/models/__init__.py
+-rw-r--r--   0        0        0      464 2023-07-01 02:50:28.552893 stability_matrix_tools-0.1.2/src/stability_matrix_tools/models/settings.py
+-rw-r--r--   0        0        0     1066 2023-06-30 22:21:37.143001 stability_matrix_tools-0.1.2/src/stability_matrix_tools/models/update_info.py
+-rw-r--r--   0        0        0      325 2023-06-30 21:06:10.076637 stability_matrix_tools-0.1.2/src/stability_matrix_tools/models/version.py
+-rw-r--r--   0        0        0      468 2023-06-30 22:21:37.151998 stability_matrix_tools-0.1.2/src/stability_matrix_tools/updates.py
+-rw-r--r--   0        0        0        0 2023-07-01 02:42:39.117279 stability_matrix_tools-0.1.2/src/stability_matrix_tools/utils/__init__.py
+-rw-r--r--   0        0        0     1634 2023-06-30 21:18:44.596055 stability_matrix_tools-0.1.2/src/stability_matrix_tools/utils/progress.py
+-rw-r--r--   0        0        0      283 2023-06-30 22:33:30.407517 stability_matrix_tools-0.1.2/src/stability_matrix_tools/utils/signing.py
+-rw-r--r--   0        0        0     2013 2023-06-30 21:23:45.959438 stability_matrix_tools-0.1.2/src/stability_matrix_tools/utils/uploader.py
+-rw-r--r--   0        0        0     1081 1970-01-01 00:00:00.000000 stability_matrix_tools-0.1.2/setup.py
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 stability_matrix_tools-0.1.2/PKG-INFO
```

### Comparing `stability_matrix_tools-0.1.1/LICENSE` & `stability_matrix_tools-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.1/pyproject.toml` & `stability_matrix_tools-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stability-matrix-tools"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Ionite <dev@ionite.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.12"
 typer = {extras = ["all"], version = "^0.9.0"}
```

### Comparing `stability_matrix_tools-0.1.1/src/stability_matrix_tools/b2.py` & `stability_matrix_tools-0.1.2/src/stability_matrix_tools/b2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 from __future__ import annotations
 
 from stability_matrix_tools.models.settings import env
-from stability_matrix_tools.progress import RichProgressListener
-from stability_matrix_tools.uploader import Uploader
+from stability_matrix_tools.utils.progress import RichProgressListener
+from stability_matrix_tools.utils.uploader import Uploader
 
 from pathlib import Path
 from urllib.parse import urljoin
-from typing import Annotated, TypeVar
+from typing import Annotated, TypeVar, Callable, ParamSpec, Any
 
-import httpx
 import typer
 from typer import Option
 
 T = TypeVar("T")
+P = ParamSpec("P")
+
 ConfirmType = Annotated[bool, Option("--yes", "-y", help="Confirm action")]
 
 app = typer.Typer()
 
 
-def assert_exists(self, *target: T, msg: str) -> T:
+def assert_exists(*target: T, msg: str) -> T:
     """Assert that objects are truthy."""
     if not all(target):
-        typer.echo(f"❌ [yellow]{msg}")
+        typer.echo(f"❌  {msg}")
         raise SystemExit(1)
     return target
 
 
+def attempt(func: Callable[[P], T], *args: Any) -> T:
+    try:
+        return func(*args)
+    except Exception as e:
+        if env.verbose:
+            raise
+        else:
+            typer.echo(f"❌  Error: {e}")
+            raise SystemExit(1)
+
+
 @app.command()
-def upload(
-    file_path: Path,
-    b2_path: str,
-    confirm: ConfirmType = False,
-):
+def upload(file_path: Path, b2_path: str, confirm: ConfirmType = False):
     """Upload a file to a B2 bucket."""
 
     file = file_path.resolve()
     assert_exists(file, msg=f"File {file_path} does not exist.")
 
     uploader = Uploader(
         api_id=env.b2_api_id,
@@ -43,10 +51,28 @@
         bucket_name=env.b2_bucket_name,
     )
 
     with RichProgressListener("Uploading...", transient=True) as pbar:
         uploader.upload(str(file), b2_path, pbar)
 
     result = urljoin(env.cdn_root, b2_path)
-    typer.echo(f"✅ Uploaded at: {result}")
+    typer.echo(f"✅  Uploaded at: {result!r}")
+
+
+@app.command()
+def delete(b2_path: str):
+    """Delete a file from the B2 bucket."""
+    uploader = Uploader(
+        api_id=env.b2_api_id,
+        api_key=env.b2_api_key,
+        bucket_name=env.b2_bucket_name,
+    )
+
+    typer.echo(f"Deleting {b2_path}...")
+
+    file = attempt(uploader.find_file, b2_path)
+    assert_exists(file, msg="File not found in B2 bucket")
+
+    uploader.delete_file(file)
 
+    typer.echo(f"🗑️  Deleted {b2_path!r}")
```

### Comparing `stability_matrix_tools-0.1.1/src/stability_matrix_tools/models/update_info.py` & `stability_matrix_tools-0.1.2/src/stability_matrix_tools/models/update_info.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.1/src/stability_matrix_tools/progress.py` & `stability_matrix_tools-0.1.2/src/stability_matrix_tools/utils/progress.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.1/src/stability_matrix_tools/uploader.py` & `stability_matrix_tools-0.1.2/src/stability_matrix_tools/utils/uploader.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.1/setup.py` & `stability_matrix_tools-0.1.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 package_dir = \
 {'': 'src'}
 
 packages = \
-['stability_matrix_tools', 'stability_matrix_tools.models']
+['stability_matrix_tools',
+ 'stability_matrix_tools.models',
+ 'stability_matrix_tools.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['b2sdk>=1.21.0,<2.0.0',
  'cryptography>=41.0.1,<42.0.0',
@@ -20,15 +22,15 @@
  'typer[all]>=0.9.0,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['sm-tools = stability_matrix_tools.main:app']}
 
 setup_kwargs = {
     'name': 'stability-matrix-tools',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': '',
     'long_description': '# sm-tools\n Stability Matrix development tools\n',
     'author': 'Ionite',
     'author_email': 'dev@ionite.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `stability_matrix_tools-0.1.1/PKG-INFO` & `stability_matrix_tools-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stability-matrix-tools
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Ionite
 Author-email: dev@ionite.io
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

