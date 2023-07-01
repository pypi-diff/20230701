# Comparing `tmp/stability_matrix_tools-0.1.2.tar.gz` & `tmp/stability_matrix_tools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stability_matrix_tools-0.1.2.tar", max compression
+gzip compressed data, was "stability_matrix_tools-0.1.3.tar", max compression
```

## Comparing `stability_matrix_tools-0.1.2.tar` & `stability_matrix_tools-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0    35163 2023-06-30 22:15:25.032480 stability_matrix_tools-0.1.2/LICENSE
--rw-r--r--   0        0        0      570 2023-07-01 02:56:17.563524 stability_matrix_tools-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       47 2023-06-30 22:15:24.995957 stability_matrix_tools-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-06-30 19:14:24.481835 stability_matrix_tools-0.1.2/src/stability_matrix_tools/__init__.py
--rw-r--r--   0        0        0     2068 2023-07-01 02:54:27.607757 stability_matrix_tools-0.1.2/src/stability_matrix_tools/b2.py
--rw-r--r--   0        0        0      163 2023-06-30 22:21:37.149999 stability_matrix_tools-0.1.2/src/stability_matrix_tools/main.py
--rw-r--r--   0        0        0        0 2023-06-30 19:29:16.679181 stability_matrix_tools-0.1.2/src/stability_matrix_tools/models/__init__.py
--rw-r--r--   0        0        0      464 2023-07-01 02:50:28.552893 stability_matrix_tools-0.1.2/src/stability_matrix_tools/models/settings.py
--rw-r--r--   0        0        0     1066 2023-06-30 22:21:37.143001 stability_matrix_tools-0.1.2/src/stability_matrix_tools/models/update_info.py
--rw-r--r--   0        0        0      325 2023-06-30 21:06:10.076637 stability_matrix_tools-0.1.2/src/stability_matrix_tools/models/version.py
--rw-r--r--   0        0        0      468 2023-06-30 22:21:37.151998 stability_matrix_tools-0.1.2/src/stability_matrix_tools/updates.py
--rw-r--r--   0        0        0        0 2023-07-01 02:42:39.117279 stability_matrix_tools-0.1.2/src/stability_matrix_tools/utils/__init__.py
--rw-r--r--   0        0        0     1634 2023-06-30 21:18:44.596055 stability_matrix_tools-0.1.2/src/stability_matrix_tools/utils/progress.py
--rw-r--r--   0        0        0      283 2023-06-30 22:33:30.407517 stability_matrix_tools-0.1.2/src/stability_matrix_tools/utils/signing.py
--rw-r--r--   0        0        0     2013 2023-06-30 21:23:45.959438 stability_matrix_tools-0.1.2/src/stability_matrix_tools/utils/uploader.py
--rw-r--r--   0        0        0     1081 1970-01-01 00:00:00.000000 stability_matrix_tools-0.1.2/setup.py
--rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 stability_matrix_tools-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35163 2023-06-30 22:15:25.032480 stability_matrix_tools-0.1.3/LICENSE
+-rw-r--r--   0        0        0      570 2023-07-01 04:34:03.473785 stability_matrix_tools-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-06-30 22:15:24.995957 stability_matrix_tools-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 19:14:24.481835 stability_matrix_tools-0.1.3/src/stability_matrix_tools/__init__.py
+-rw-r--r--   0        0        0     2329 2023-07-01 03:50:14.086249 stability_matrix_tools-0.1.3/src/stability_matrix_tools/b2.py
+-rw-r--r--   0        0        0      380 2023-07-01 04:29:55.594056 stability_matrix_tools-0.1.3/src/stability_matrix_tools/cf.py
+-rw-r--r--   0        0        0      201 2023-07-01 03:57:29.403922 stability_matrix_tools-0.1.3/src/stability_matrix_tools/main.py
+-rw-r--r--   0        0        0        0 2023-06-30 19:29:16.679181 stability_matrix_tools-0.1.3/src/stability_matrix_tools/models/__init__.py
+-rw-r--r--   0        0        0      518 2023-07-01 03:35:42.001028 stability_matrix_tools-0.1.3/src/stability_matrix_tools/models/settings.py
+-rw-r--r--   0        0        0     1007 2023-07-01 03:25:17.677979 stability_matrix_tools-0.1.3/src/stability_matrix_tools/models/update_info.py
+-rw-r--r--   0        0        0      325 2023-06-30 21:06:10.076637 stability_matrix_tools-0.1.3/src/stability_matrix_tools/models/version.py
+-rw-r--r--   0        0        0      608 2023-07-01 03:12:38.918254 stability_matrix_tools-0.1.3/src/stability_matrix_tools/updates.py
+-rw-r--r--   0        0        0        0 2023-07-01 02:42:39.117279 stability_matrix_tools-0.1.3/src/stability_matrix_tools/utils/__init__.py
+-rw-r--r--   0        0        0      588 2023-07-01 04:29:34.632450 stability_matrix_tools-0.1.3/src/stability_matrix_tools/utils/cf_cache.py
+-rw-r--r--   0        0        0     1634 2023-06-30 21:18:44.596055 stability_matrix_tools-0.1.3/src/stability_matrix_tools/utils/progress.py
+-rw-r--r--   0        0        0      283 2023-06-30 22:33:30.407517 stability_matrix_tools-0.1.3/src/stability_matrix_tools/utils/signing.py
+-rw-r--r--   0        0        0     2013 2023-06-30 21:23:45.959438 stability_matrix_tools-0.1.3/src/stability_matrix_tools/utils/uploader.py
+-rw-r--r--   0        0        0     1081 1970-01-01 00:00:00.000000 stability_matrix_tools-0.1.3/setup.py
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 stability_matrix_tools-0.1.3/PKG-INFO
```

### Comparing `stability_matrix_tools-0.1.2/LICENSE` & `stability_matrix_tools-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.2/pyproject.toml` & `stability_matrix_tools-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stability-matrix-tools"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Ionite <dev@ionite.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.12"
 typer = {extras = ["all"], version = "^0.9.0"}
```

### Comparing `stability_matrix_tools-0.1.2/src/stability_matrix_tools/b2.py` & `stability_matrix_tools-0.1.3/src/stability_matrix_tools/b2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from stability_matrix_tools.models.settings import env
 from stability_matrix_tools.utils.progress import RichProgressListener
 from stability_matrix_tools.utils.uploader import Uploader
+from stability_matrix_tools.utils.cf_cache import cache_purge
 
 from pathlib import Path
 from urllib.parse import urljoin
 from typing import Annotated, TypeVar, Callable, ParamSpec, Any
 
 import typer
 from typer import Option
@@ -50,14 +51,17 @@
         api_key=env.b2_api_key,
         bucket_name=env.b2_bucket_name,
     )
 
     with RichProgressListener("Uploading...", transient=True) as pbar:
         uploader.upload(str(file), b2_path, pbar)
 
+    typer.echo("Updating Cloudflare cache...")
+    cache_purge(urljoin(env.cdn_root, b2_path))
+
     result = urljoin(env.cdn_root, b2_path)
     typer.echo(f"✅  Uploaded at: {result!r}")
 
 
 @app.command()
 def delete(b2_path: str):
     """Delete a file from the B2 bucket."""
@@ -70,9 +74,12 @@
     typer.echo(f"Deleting {b2_path}...")
 
     file = attempt(uploader.find_file, b2_path)
     assert_exists(file, msg="File not found in B2 bucket")
 
     uploader.delete_file(file)
 
+    typer.echo("Updating Cloudflare cache...")
+    cache_purge(urljoin(env.cdn_root, b2_path))
+
     typer.echo(f"🗑️  Deleted {b2_path!r}")
```

### Comparing `stability_matrix_tools-0.1.2/src/stability_matrix_tools/models/update_info.py` & `stability_matrix_tools-0.1.3/src/stability_matrix_tools/models/update_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from enum import Enum, Flag
 from datetime import datetime
 
 from stability_matrix_tools.models.version import Version
 
-from pydantic import BaseModel, ConfigDict, RootModel
+from pydantic import BaseModel, ConfigDict, field_validator
+from pydantic.types import NaiveDatetime
 
 
 def to_camel(string: str) -> str:
     """Convert to camel case."""
     string = "".join(word.capitalize() for word in string.split("_"))
     if string and string[0].isupper():
         string = string[0].lower() + string[1:]
@@ -23,22 +24,19 @@
 class UpdateType(Flag, boundary="keep"):
     normal = 0 << 1
     critical = 1 << 1
     mandatory = 1 << 2
 
 
 class UpdateInfo(BaseModel):
-    model_config = ConfigDict(alias_generator=to_camel, arbitrary_types_allowed=True)
-
-    version: Version
-    release_date: datetime
+    version: str
+    release_date: NaiveDatetime
     channel: UpdateChannel
     url: str
     changelog: str
     signature: str | None
     type: UpdateType | None
 
+    class Config:
+        alias_generator = to_camel
+        arbitrary_types_allowed = True
 
-class Updates(RootModel):
-    model_config = ConfigDict(alias_generator=to_camel)
-
-    root: list[UpdateInfo]
```

### Comparing `stability_matrix_tools-0.1.2/src/stability_matrix_tools/utils/progress.py` & `stability_matrix_tools-0.1.3/src/stability_matrix_tools/utils/progress.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.2/src/stability_matrix_tools/utils/uploader.py` & `stability_matrix_tools-0.1.3/src/stability_matrix_tools/utils/uploader.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.2/setup.py` & `stability_matrix_tools-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  'typer[all]>=0.9.0,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['sm-tools = stability_matrix_tools.main:app']}
 
 setup_kwargs = {
     'name': 'stability-matrix-tools',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': '',
     'long_description': '# sm-tools\n Stability Matrix development tools\n',
     'author': 'Ionite',
     'author_email': 'dev@ionite.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `stability_matrix_tools-0.1.2/PKG-INFO` & `stability_matrix_tools-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stability-matrix-tools
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Ionite
 Author-email: dev@ionite.io
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

