# Comparing `tmp/felt_upload-0.1.1.tar.gz` & `tmp/felt_upload-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "felt_upload-0.1.1.tar", max compression
+gzip compressed data, was "felt_upload-0.1.2.tar", max compression
```

## Comparing `felt_upload-0.1.1.tar` & `felt_upload-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-06-30 22:21:13.744606 felt_upload-0.1.1/LICENSE
--rw-r--r--   0        0        0     2351 2023-06-30 22:21:13.744606 felt_upload-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-30 22:21:13.744606 felt_upload-0.1.1/felt_upload/__init__.py
--rw-r--r--   0        0        0       71 2023-06-30 22:21:13.744606 felt_upload-0.1.1/felt_upload/__main__.py
--rw-r--r--   0        0        0     4865 2023-06-30 22:21:13.744606 felt_upload-0.1.1/felt_upload/api.py
--rw-r--r--   0        0        0     5863 2023-06-30 22:21:13.744606 felt_upload-0.1.1/felt_upload/cli.py
--rw-r--r--   0        0        0     1074 2023-06-30 22:21:13.744606 felt_upload-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3086 1970-01-01 00:00:00.000000 felt_upload-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-30 23:12:41.264865 felt_upload-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2351 2023-06-30 23:12:41.264865 felt_upload-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 23:12:41.264865 felt_upload-0.1.2/felt_upload/__init__.py
+-rw-r--r--   0        0        0       71 2023-06-30 23:12:41.264865 felt_upload-0.1.2/felt_upload/__main__.py
+-rw-r--r--   0        0        0     4871 2023-06-30 23:12:41.264865 felt_upload-0.1.2/felt_upload/api.py
+-rw-r--r--   0        0        0     5863 2023-06-30 23:12:41.264865 felt_upload-0.1.2/felt_upload/cli.py
+-rw-r--r--   0        0        0     1074 2023-06-30 23:12:41.264865 felt_upload-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3136 1970-01-01 00:00:00.000000 felt_upload-0.1.2/PKG-INFO
```

### Comparing `felt_upload-0.1.1/LICENSE` & `felt_upload-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `felt_upload-0.1.1/README.md` & `felt_upload-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `felt_upload-0.1.1/felt_upload/api.py` & `felt_upload-0.1.2/felt_upload/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from pathlib import Path
-from typing import Any, Callable, List, Optional
+from typing import Any, Callable, Dict, List, Optional
 from urllib.parse import urljoin
 
 import requests
 from requests_toolbelt import MultipartEncoderMonitor
 
 
 class FeltAPIError(Exception):
     pass
 
 
 class UnauthorizedError(FeltAPIError):
     pass
 
 
-def drop_empty(dct: dict[Any, Any]) -> dict[Any, Any]:
+def drop_empty(dct: Dict[Any, Any]) -> Dict[Any, Any]:
     """Drop empty values from a dict."""
     return {key: value for key, value in dct.items() if value}
 
 
 class Felt:
     def __init__(
         self,
@@ -27,15 +27,15 @@
         session: Optional[requests.Session] = None,
     ):
         self.api_token = api_token
         self.base_url = base_url
         self.session = session or requests.Session()
 
     @property
-    def _headers(self) -> dict[str, str]:
+    def _headers(self) -> Dict[str, str]:
         return {
             "authorization": f"Bearer {self.api_token}",
             "content-type": "application/json",
         }
 
     def _request(self, method: str, url: str, **kwargs: Any) -> Any:
         resp = self.session.request(
@@ -50,15 +50,15 @@
 
         if resp.status_code == 401:
             raise UnauthorizedError
         else:
             resp.raise_for_status()
         return resp.json()
 
-    def user(self) -> dict[str, str]:
+    def user(self) -> Dict[str, str]:
         """Make a /user request"""
         json_data = self._request("get", "user")
         return {
             "name": json_data["data"]["attributes"]["name"],
             "email": json_data["data"]["attributes"]["email"],
         }
 
@@ -66,15 +66,15 @@
         self,
         title: Optional[str] = None,
         *,
         basemap: Optional[str] = None,
         zoom: Optional[float] = None,
         lat: Optional[float] = None,
         lon: Optional[float] = None,
-    ) -> dict[str, str]:
+    ) -> Dict[str, str]:
         """Create an empty map."""
         data = self._request(
             "post",
             "maps",
             json=drop_empty(
                 {
                     "title": title,
@@ -96,15 +96,15 @@
         map_id: str,
         files: List[Path],
         *,
         name: Optional[str] = None,
         fill_color: Optional[str] = None,
         stroke_color: Optional[str] = None,
         update_file_progress: Optional[Callable[[str, int, int], None]] = None,
-    ) -> dict[str, str]:
+    ) -> Dict[str, str]:
         """Create a layer and upload files."""
         data = self._request(
             "post",
             f"maps/{map_id}/layers",
             json=drop_empty(
                 {
                     "name": name,
@@ -152,15 +152,15 @@
 
     def import_layer(
         self,
         map_id: str,
         layer_url: str,
         *,
         name: Optional[str] = None,
-    ) -> dict[str, str]:
+    ) -> Dict[str, str]:
         """Import layer from a url."""
         resp = self._request(
             "post",
             f"maps/{map_id}/layers/url_import",
             json=drop_empty(
                 {
                     "layer_url": layer_url,
```

### Comparing `felt_upload-0.1.1/felt_upload/cli.py` & `felt_upload-0.1.2/felt_upload/cli.py`

 * *Files identical despite different names*

### Comparing `felt_upload-0.1.1/pyproject.toml` & `felt_upload-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "felt-upload"
-version = "0.1.1"
+version = "0.1.2"
 description = "CLI tool to upload data to Felt"
 authors = ["Oleksii Vykaliuk <alekzvik@gmail.com>"]
 readme = "README.md"
 packages = [{include = "felt_upload"}]
 license = "MIT"
 repository = "https://github.com/alekzvik/felt_upload"
 
 [tool.poetry.scripts]
 felt-upload = "felt_upload.cli:app"
 
 [tool.poetry.dependencies]
-python = ">=3.9"
+python = ">=3.8"
 requests = "^2.31.0"
 typer = {extras = ["all"], version = "^0.9.0"}
 requests-toolbelt = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "*"
 black = "*"
```

### Comparing `felt_upload-0.1.1/PKG-INFO` & `felt_upload-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: felt-upload
-Version: 0.1.1
+Version: 0.1.2
 Summary: CLI tool to upload data to Felt
 Home-page: https://github.com/alekzvik/felt_upload
 License: MIT
 Author: Oleksii Vykaliuk
 Author-email: alekzvik@gmail.com
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/alekzvik/felt_upload
```

