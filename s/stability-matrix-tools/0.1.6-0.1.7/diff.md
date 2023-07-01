# Comparing `tmp/stability_matrix_tools-0.1.6.tar.gz` & `tmp/stability_matrix_tools-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stability_matrix_tools-0.1.6.tar", max compression
+gzip compressed data, was "stability_matrix_tools-0.1.7.tar", max compression
```

## Comparing `stability_matrix_tools-0.1.6.tar` & `stability_matrix_tools-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0    35163 2023-06-30 22:15:25.032480 stability_matrix_tools-0.1.6/LICENSE
--rw-r--r--   0        0        0      613 2023-07-01 07:26:30.246437 stability_matrix_tools-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       47 2023-06-30 22:15:24.995957 stability_matrix_tools-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-06-30 19:14:24.481835 stability_matrix_tools-0.1.6/src/stability_matrix_tools/__init__.py
--rw-r--r--   0        0        0     2329 2023-07-01 03:50:14.086249 stability_matrix_tools-0.1.6/src/stability_matrix_tools/b2.py
--rw-r--r--   0        0        0      380 2023-07-01 04:29:55.594056 stability_matrix_tools-0.1.6/src/stability_matrix_tools/cf.py
--rw-r--r--   0        0        0     3068 2023-07-01 07:09:28.831003 stability_matrix_tools-0.1.6/src/stability_matrix_tools/keys.py
--rw-r--r--   0        0        0      245 2023-07-01 06:42:59.756522 stability_matrix_tools-0.1.6/src/stability_matrix_tools/main.py
--rw-r--r--   0        0        0        0 2023-06-30 19:29:16.679181 stability_matrix_tools-0.1.6/src/stability_matrix_tools/models/__init__.py
--rw-r--r--   0        0        0      518 2023-07-01 03:35:42.001028 stability_matrix_tools-0.1.6/src/stability_matrix_tools/models/settings.py
--rw-r--r--   0        0        0     1459 2023-07-01 07:26:25.628056 stability_matrix_tools-0.1.6/src/stability_matrix_tools/models/update_info.py
--rw-r--r--   0        0        0      325 2023-06-30 21:06:10.076637 stability_matrix_tools-0.1.6/src/stability_matrix_tools/models/version.py
--rw-r--r--   0        0        0      707 2023-07-01 05:33:17.097804 stability_matrix_tools-0.1.6/src/stability_matrix_tools/updates.py
--rw-r--r--   0        0        0        0 2023-07-01 02:42:39.117279 stability_matrix_tools-0.1.6/src/stability_matrix_tools/utils/__init__.py
--rw-r--r--   0        0        0      588 2023-07-01 04:29:34.632450 stability_matrix_tools-0.1.6/src/stability_matrix_tools/utils/cf_cache.py
--rw-r--r--   0        0        0     1634 2023-06-30 21:18:44.596055 stability_matrix_tools-0.1.6/src/stability_matrix_tools/utils/progress.py
--rw-r--r--   0        0        0     1948 2023-07-01 06:57:32.338302 stability_matrix_tools-0.1.6/src/stability_matrix_tools/utils/signing.py
--rw-r--r--   0        0        0     2013 2023-06-30 21:23:45.959438 stability_matrix_tools-0.1.6/src/stability_matrix_tools/utils/uploader.py
--rw-r--r--   0        0        0     1137 1970-01-01 00:00:00.000000 stability_matrix_tools-0.1.6/setup.py
--rw-r--r--   0        0        0      772 1970-01-01 00:00:00.000000 stability_matrix_tools-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35163 2023-06-30 22:15:25.032480 stability_matrix_tools-0.1.7/LICENSE
+-rw-r--r--   0        0        0      632 2023-07-01 09:10:46.075669 stability_matrix_tools-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-06-30 22:15:24.995957 stability_matrix_tools-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 19:14:24.481835 stability_matrix_tools-0.1.7/src/stability_matrix_tools/__init__.py
+-rw-r--r--   0        0        0     2329 2023-07-01 03:50:14.086249 stability_matrix_tools-0.1.7/src/stability_matrix_tools/b2.py
+-rw-r--r--   0        0        0      380 2023-07-01 04:29:55.594056 stability_matrix_tools-0.1.7/src/stability_matrix_tools/cf.py
+-rw-r--r--   0        0        0     3068 2023-07-01 07:09:28.831003 stability_matrix_tools-0.1.7/src/stability_matrix_tools/keys.py
+-rw-r--r--   0        0        0      245 2023-07-01 06:42:59.756522 stability_matrix_tools-0.1.7/src/stability_matrix_tools/main.py
+-rw-r--r--   0        0        0        0 2023-06-30 19:29:16.679181 stability_matrix_tools-0.1.7/src/stability_matrix_tools/models/__init__.py
+-rw-r--r--   0        0        0      518 2023-07-01 03:35:42.001028 stability_matrix_tools-0.1.7/src/stability_matrix_tools/models/settings.py
+-rw-r--r--   0        0        0     1293 2023-07-01 09:06:51.555909 stability_matrix_tools-0.1.7/src/stability_matrix_tools/models/update_info.py
+-rw-r--r--   0        0        0      325 2023-06-30 21:06:10.076637 stability_matrix_tools-0.1.7/src/stability_matrix_tools/models/version.py
+-rw-r--r--   0        0        0     5371 2023-07-01 09:09:16.670644 stability_matrix_tools-0.1.7/src/stability_matrix_tools/updates.py
+-rw-r--r--   0        0        0        0 2023-07-01 02:42:39.117279 stability_matrix_tools-0.1.7/src/stability_matrix_tools/utils/__init__.py
+-rw-r--r--   0        0        0      588 2023-07-01 04:29:34.632450 stability_matrix_tools-0.1.7/src/stability_matrix_tools/utils/cf_cache.py
+-rw-r--r--   0        0        0     1634 2023-06-30 21:18:44.596055 stability_matrix_tools-0.1.7/src/stability_matrix_tools/utils/progress.py
+-rw-r--r--   0        0        0     1948 2023-07-01 06:57:32.338302 stability_matrix_tools-0.1.7/src/stability_matrix_tools/utils/signing.py
+-rw-r--r--   0        0        0      709 2023-07-01 08:56:22.308456 stability_matrix_tools-0.1.7/src/stability_matrix_tools/utils/stream_hash.py
+-rw-r--r--   0        0        0     2051 2023-07-01 08:34:51.103754 stability_matrix_tools-0.1.7/src/stability_matrix_tools/utils/uploader.py
+-rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 stability_matrix_tools-0.1.7/setup.py
+-rw-r--r--   0        0        0      811 1970-01-01 00:00:00.000000 stability_matrix_tools-0.1.7/PKG-INFO
```

### Comparing `stability_matrix_tools-0.1.6/LICENSE` & `stability_matrix_tools-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.6/pyproject.toml` & `stability_matrix_tools-0.1.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stability-matrix-tools"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["Ionite <dev@ionite.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.12"
 typer = {extras = ["all"], version = "^0.9.0"}
@@ -12,14 +12,15 @@
 semver = "^3.0.1"
 httpx = "^0.24.1"
 b2sdk = "^1.21.0"
 python-dotenv = "^1.0.0"
 cryptography = "^41.0.1"
 keyring = "^24.2.0"
 pyperclip = "^1.8.2"
+blake3 = "^0.3.3"
 
 [tool.poetry.scripts]
 sm-tools = "stability_matrix_tools.main:app"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `stability_matrix_tools-0.1.6/src/stability_matrix_tools/b2.py` & `stability_matrix_tools-0.1.7/src/stability_matrix_tools/b2.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.6/src/stability_matrix_tools/keys.py` & `stability_matrix_tools-0.1.7/src/stability_matrix_tools/keys.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.6/src/stability_matrix_tools/models/settings.py` & `stability_matrix_tools-0.1.7/src/stability_matrix_tools/models/settings.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.6/src/stability_matrix_tools/models/update_info.py` & `stability_matrix_tools-0.1.7/src/stability_matrix_tools/models/update_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import Enum, Flag
 from datetime import datetime
-from typing import Annotated
+from typing_extensions import Annotated
 
-from pydantic import BaseModel, field_validator, ValidationError, WrapValidator
+from pydantic import BaseModel, ValidationError, WrapValidator
 from pydantic.types import AwareDatetime
 
 
 def to_camel(string: str) -> str:
     """Convert to camel case."""
     string = "".join(word.capitalize() for word in string.split("_"))
     if string and string[0].isupper():
@@ -14,44 +14,40 @@
     return string
 
 
 def validate_timestamp(value, handler):
     try:
         return handler(value)
     except ValidationError:
+        if isinstance(value, datetime):
+            return value
         return datetime.fromisoformat(value[0])
 
 
 DateTimeOffset = Annotated[AwareDatetime, WrapValidator(validate_timestamp)]
 
 
 class UpdateChannel(Enum):
     stable = "stable"
     preview = "preview"
     development = "development"
 
 
 class UpdateType(Flag):
-    normal = 0 << 1
+    normal = 1 << 0
     critical = 1 << 1
     mandatory = 1 << 2
 
 
 class UpdateInfo(BaseModel):
     version: str
     release_date: DateTimeOffset
     channel: UpdateChannel
+    type: UpdateType
     url: str
     changelog: str
-    signature: str | None = None
-    type: UpdateType | None = None
-
-    # noinspection PyMethodParameters
-    @field_validator('release_date', 'release_date', mode='before')
-    def split_str(cls, v):
-        if isinstance(v, str):
-            return v.split('|')
-        return v
+    hash_blake3: str
+    signature: str
 
     class Config:
         alias_generator = to_camel
         arbitrary_types_allowed = True
```

### Comparing `stability_matrix_tools-0.1.6/src/stability_matrix_tools/utils/cf_cache.py` & `stability_matrix_tools-0.1.7/src/stability_matrix_tools/utils/cf_cache.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.6/src/stability_matrix_tools/utils/progress.py` & `stability_matrix_tools-0.1.7/src/stability_matrix_tools/utils/progress.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.6/src/stability_matrix_tools/utils/signing.py` & `stability_matrix_tools-0.1.7/src/stability_matrix_tools/utils/signing.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.6/src/stability_matrix_tools/utils/uploader.py` & `stability_matrix_tools-0.1.7/src/stability_matrix_tools/utils/uploader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import os
+from pathlib import Path
 
 import b2sdk.exception as b2_exception
 import b2sdk.file_version
 from b2sdk.progress import AbstractProgressListener
 from b2sdk.v2 import B2Api, InMemoryAccountInfo
 
 
@@ -29,20 +30,20 @@
             search = self.bucket.get_file_info_by_name(b2_path)
         except b2_exception.FileNotPresent:
             return None
         return search
 
     def upload(
         self,
-        file_path: str,
+        file_path: str | Path,
         b2_path: str,
         progress_listener: AbstractProgressListener | None = None,
     ):
         """Uploads a file to the B2 bucket."""
-        file_name = os.path.basename(file_path)
+        file_name = os.path.basename(str(file_path))
         base_name, ext = os.path.splitext(file_name)
 
         # Upload the file
         try:
             self.bucket.upload_local_file(
                 local_file=file_path,
                 file_name=b2_path,
```

### Comparing `stability_matrix_tools-0.1.6/setup.py` & `stability_matrix_tools-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,29 +10,30 @@
  'stability_matrix_tools.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['b2sdk>=1.21.0,<2.0.0',
+ 'blake3>=0.3.3,<0.4.0',
  'cryptography>=41.0.1,<42.0.0',
  'httpx>=0.24.1,<0.25.0',
  'keyring>=24.2.0,<25.0.0',
  'pydantic[dotenv]>=2.0,<3.0',
  'pyperclip>=1.8.2,<2.0.0',
  'python-dotenv>=1.0.0,<2.0.0',
  'semver>=3.0.1,<4.0.0',
  'typer[all]>=0.9.0,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['sm-tools = stability_matrix_tools.main:app']}
 
 setup_kwargs = {
     'name': 'stability-matrix-tools',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': '',
     'long_description': '# sm-tools\n Stability Matrix development tools\n',
     'author': 'Ionite',
     'author_email': 'dev@ionite.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `stability_matrix_tools-0.1.6/PKG-INFO` & `stability_matrix_tools-0.1.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: stability-matrix-tools
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: Ionite
 Author-email: dev@ionite.io
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: b2sdk (>=1.21.0,<2.0.0)
+Requires-Dist: blake3 (>=0.3.3,<0.4.0)
 Requires-Dist: cryptography (>=41.0.1,<42.0.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: keyring (>=24.2.0,<25.0.0)
 Requires-Dist: pydantic[dotenv] (>=2.0,<3.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: semver (>=3.0.1,<4.0.0)
```

