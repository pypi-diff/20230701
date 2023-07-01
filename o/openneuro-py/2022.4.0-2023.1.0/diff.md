# Comparing `tmp/openneuro-py-2022.4.0.tar.gz` & `tmp/openneuro-py-2023.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openneuro-py-2022.4.0.tar", last modified: Tue Dec 13 13:28:57 2022, max compression
+gzip compressed data, was "openneuro-py-2023.1.0.tar", last modified: Sat Jul  1 08:34:01 2023, max compression
```

## Comparing `openneuro-py-2022.4.0.tar` & `openneuro-py-2023.1.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 13:28:57.930722 openneuro-py-2022.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 13:28:57.926722 openneuro-py-2022.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2022-12-13 13:28:43.000000 openneuro-py-2022.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 13:28:57.926722 openneuro-py-2022.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2022-12-13 13:28:43.000000 openneuro-py-2022.4.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2022-12-13 13:28:43.000000 openneuro-py-2022.4.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2022-12-13 13:28:43.000000 openneuro-py-2022.4.0/.github/workflows/run-linter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2022-12-13 13:28:43.000000 openneuro-py-2022.4.0/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2022-12-13 13:28:43.000000 openneuro-py-2022.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2022-12-13 13:28:43.000000 openneuro-py-2022.4.0/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2022-12-13 13:28:43.000000 openneuro-py-2022.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    43438 2022-12-13 13:28:57.926722 openneuro-py-2022.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2022-12-13 13:28:43.000000 openneuro-py-2022.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 13:28:57.926722 openneuro-py-2022.4.0/openneuro/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2022-12-13 13:28:43.000000 openneuro-py-2022.4.0/openneuro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2022-12-13 13:28:43.000000 openneuro-py-2022.4.0/openneuro/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32477 2022-12-13 13:28:43.000000 openneuro-py-2022.4.0/openneuro/_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2022-12-13 13:28:43.000000 openneuro-py-2022.4.0/openneuro/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2022-12-13 13:28:43.000000 openneuro-py-2022.4.0/openneuro/openneuro.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 13:28:57.926722 openneuro-py-2022.4.0/openneuro/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2022-12-13 13:28:43.000000 openneuro-py-2022.4.0/openneuro/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2022-12-13 13:28:43.000000 openneuro-py-2022.4.0/openneuro/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)   421252 2022-12-13 13:28:43.000000 openneuro-py-2022.4.0/openneuro-py.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 13:28:57.926722 openneuro-py-2022.4.0/openneuro_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43438 2022-12-13 13:28:57.000000 openneuro-py-2022.4.0/openneuro_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      626 2022-12-13 13:28:57.000000 openneuro-py-2022.4.0/openneuro_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 13:28:57.000000 openneuro-py-2022.4.0/openneuro_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2022-12-13 13:28:57.000000 openneuro-py-2022.4.0/openneuro_py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2022-12-13 13:28:57.000000 openneuro-py-2022.4.0/openneuro_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-13 13:28:57.000000 openneuro-py-2022.4.0/openneuro_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2022-12-13 13:28:43.000000 openneuro-py-2022.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-13 13:28:57.930722 openneuro-py-2022.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:34:01.395962 openneuro-py-2023.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-01 08:33:49.000000 openneuro-py-2023.1.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:34:01.391962 openneuro-py-2023.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-01 08:33:49.000000 openneuro-py-2023.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:34:01.395962 openneuro-py-2023.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-01 08:33:49.000000 openneuro-py-2023.1.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-01 08:33:49.000000 openneuro-py-2023.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-01 08:33:49.000000 openneuro-py-2023.1.0/.github/workflows/run-linter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-01 08:33:49.000000 openneuro-py-2023.1.0/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-01 08:33:49.000000 openneuro-py-2023.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-01 08:33:49.000000 openneuro-py-2023.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-07-01 08:33:49.000000 openneuro-py-2023.1.0/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 08:33:49.000000 openneuro-py-2023.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43438 2023-07-01 08:34:01.395962 openneuro-py-2023.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-01 08:33:49.000000 openneuro-py-2023.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:34:01.395962 openneuro-py-2023.1.0/openneuro/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-01 08:33:49.000000 openneuro-py-2023.1.0/openneuro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-01 08:33:49.000000 openneuro-py-2023.1.0/openneuro/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31782 2023-07-01 08:33:49.000000 openneuro-py-2023.1.0/openneuro/_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-01 08:33:49.000000 openneuro-py-2023.1.0/openneuro/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-01 08:33:49.000000 openneuro-py-2023.1.0/openneuro/openneuro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:34:01.395962 openneuro-py-2023.1.0/openneuro/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-01 08:33:49.000000 openneuro-py-2023.1.0/openneuro/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-01 08:33:49.000000 openneuro-py-2023.1.0/openneuro/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)   421252 2023-07-01 08:33:49.000000 openneuro-py-2023.1.0/openneuro-py.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:34:01.395962 openneuro-py-2023.1.0/openneuro_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43438 2023-07-01 08:34:01.000000 openneuro-py-2023.1.0/openneuro_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-01 08:34:01.000000 openneuro-py-2023.1.0/openneuro_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 08:34:01.000000 openneuro-py-2023.1.0/openneuro_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-01 08:34:01.000000 openneuro-py-2023.1.0/openneuro_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-01 08:34:01.000000 openneuro-py-2023.1.0/openneuro_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 08:34:01.000000 openneuro-py-2023.1.0/openneuro_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-01 08:33:49.000000 openneuro-py-2023.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 08:34:01.395962 openneuro-py-2023.1.0/setup.cfg
```

### Comparing `openneuro-py-2022.4.0/.github/dependabot.yml` & `openneuro-py-2023.1.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `openneuro-py-2022.4.0/.github/workflows/codeql-analysis.yml` & `openneuro-py-2023.1.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `openneuro-py-2022.4.0/.github/workflows/python-publish.yml` & `openneuro-py-2023.1.0/.github/workflows/python-publish.yml`

 * *Files 11% similar despite different names*

```diff
@@ -29,11 +29,11 @@
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build
     - name: Build package
       run: python -m build
     - name: Publish package
-      uses: pypa/gh-action-pypi-publish@c7f29f7adef1a245bd91520e94867e5c6eedddcc
+      uses: pypa/gh-action-pypi-publish@f5622bde02b04381239da3573277701ceca8f6a0
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `openneuro-py-2022.4.0/.github/workflows/run-linter.yml` & `openneuro-py-2023.1.0/.github/workflows/run-tests.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 # This workflow will install Python dependencies, run tests and lint with a variety of Python versions
 # For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
 
-name: Linter
+name: Unit tests
 
 on:
   # push:
   #   branches: ['**']
   pull_request:
     branches: ['**']
   create:
     branches: [main]
     tags: ['**']
   # schedule:
   #   - cron: "0 4 * * *"
 
-jobs:
-  lint:
-
-    concurrency: lint_job
-    # cancel-in-progress: true
+concurrency:
+  group: ${{ github.workflow }}-${{ github.event.pull_request.number || github.ref }}
+  cancel-in-progress: true
 
-    runs-on: ubuntu-latest
+jobs:
+  test:
     strategy:
       fail-fast: false
       matrix:
+       # Adjust for min and max supported Python versions
         python-version: ["3.11"]
-
+        os: [ubuntu-latest, windows-latest, macos-latest]
+        include:
+          - python-version: "3.8"
+            os: ubuntu-latest
+    runs-on: ${{ matrix.os }}
+    defaults:
+      run:
+        shell: bash -e {0}
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        python -m pip install flake8
-    - name: Lint with flake8
+        python -m pip install --upgrade wheel
+    - name: Install openneuro-py
+      run: pip install .[tests]
+    - name: Test with pytest
       run: |
-        # stop the build if there are Python syntax errors, undefined names,
-        # or trailing whitespaces
-        flake8 . --count --select=E9,F63,F7,F82,W291,W293 --show-source --statistics
-        # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
-        flake8 . --count --exit-zero --max-line-length=127 --statistics
+        pytest
```

### Comparing `openneuro-py-2022.4.0/CHANGES.md` & `openneuro-py-2023.1.0/CHANGES.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Changelog
 
-## unreleased
+## 2023.1.0
 
 - Better handling of server response errors.
+- Drop support for Python 3.7. `openneuro-py` now requires Python 3.8 or newer.
+- We switched from using the unmaintained `appdirs` to `platformdirs`. If you're using private OpenNeuro repositories on macOS, you may have to enter your API tokens again.
 
 ## 2022.2.0
 
 - Support latest OpenNeuro API.
 - Display suggestions in the exception when `include` contains invalid
   entries.
 - Drop list of default excludes. OpenNeuro has fixed server response for the
```

### Comparing `openneuro-py-2022.4.0/LICENSE` & `openneuro-py-2023.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openneuro-py-2022.4.0/PKG-INFO` & `openneuro-py-2023.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openneuro-py
-Version: 2022.4.0
+Version: 2023.1.0
 Summary: A Python client for OpenNeuro.
 Author-email: Richard Höchenberger <richard.hoechenberger@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -679,15 +679,15 @@
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: homepage, https://github.com/hoechenberger/openneuro-py
 Project-URL: changelog, https://github.com/hoechenberger/openneuro-py/CHANGES.md
 Keywords: science,neuroscience
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # openneuro-py
 
 A Python client for accessing [OpenNeuro](https://openneuro.org)
```

### Comparing `openneuro-py-2022.4.0/README.md` & `openneuro-py-2023.1.0/README.md`

 * *Files identical despite different names*

### Comparing `openneuro-py-2022.4.0/openneuro/_download.py` & `openneuro-py-2023.1.0/openneuro/_download.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,47 +3,43 @@
 import fnmatch
 from difflib import get_close_matches
 import hashlib
 import asyncio
 from pathlib import Path, PurePosixPath
 import string
 import json
-from typing import Optional, Union
-if sys.version_info >= (3, 8):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
+from typing import Optional, Union, Literal
 
 if sys.version_info >= (3, 9):
     from collections.abc import Iterable, Generator
 else:
     from typing import Iterable, Generator  # Deprecated since 3.9
 
 import requests
 import httpx
 
 # Manually "enforce" notebook mode in VS Code to get progress bar widgets
 # Can be removed once https://github.com/tqdm/tqdm/issues/1213 has been merged
-if 'VSCODE_PID' in os.environ:
+if "VSCODE_PID" in os.environ:
     from tqdm.notebook import tqdm
 else:
     from tqdm.auto import tqdm
 
 import click
 import aiofiles
 from sgqlc.endpoint.requests import RequestsEndpoint
 
 from . import __version__
 from .config import BASE_URL, get_token, init_config
 
 
-if hasattr(sys.stdout, 'encoding') and sys.stdout.encoding.lower() == 'utf-8':
+if hasattr(sys.stdout, "encoding") and sys.stdout.encoding.lower() == "utf-8":
     stdout_unicode = True
-elif hasattr(sys.stdout, 'reconfigure'):
-    sys.stdout.reconfigure(encoding='utf-8')
+elif hasattr(sys.stdout, "reconfigure"):
+    sys.stdout.reconfigure(encoding="utf-8")
     stdout_unicode = True
 else:
     stdout_unicode = False
 
 
 def login():
     """Login to OpenNeuro and store an access token."""
@@ -55,215 +51,229 @@
 allowed_retry_codes = (408, 500, 502, 503, 504, 522, 524)
 allowed_retry_exceptions = (
     # For file downloads
     httpx.ConnectTimeout,
     httpx.ReadTimeout,
     httpx.ReadError,
     httpx.ConnectError,  # [Errno -3] Temporary failure in name resolution
-
     # For GraphQL requests via sgqlc (doesn't support httpx)
     requests.exceptions.ConnectTimeout,
     requests.exceptions.ReadTimeout,
-
     # "peer closed connection without sending complete message body
     #  (incomplete chunked read)"
-    httpx.RemoteProtocolError
+    httpx.RemoteProtocolError,
 )
 
 # GraphQL endpoint and queries.
 
-gql_url = 'https://openneuro.org/crn/graphql'
+gql_url = "https://openneuro.org/crn/graphql"
 
-dataset_query_template = string.Template("""
+dataset_query_template = string.Template(
+    """
     query {
         dataset(id: "$dataset_id") {
             latestSnapshot {
                 id
                 files {
                     filename
                     urls
                     size
                     directory
                     id
                 }
             }
         }
     }
-""")
+"""
+)
 
-all_snapshots_query_template = string.Template("""
+all_snapshots_query_template = string.Template(
+    """
     query {
         dataset(id: "$dataset_id") {
             snapshots {
                 id
             }
         }
     }
-""")
+"""
+)
 
-snapshot_query_template = string.Template("""
+snapshot_query_template = string.Template(
+    """
     query {
         snapshot(datasetId: "$dataset_id", tag: "$tag") {
             id
             files(tree: $tree) {
                 filename
                 urls
                 size
                 directory
                 id
             }
         }
     }
-""")
+"""
+)
 
 
 def _safe_query(query, *, timeout=None):
     with requests.Session() as session:
         try:
             token = get_token()
             session.cookies.set_cookie(
-                requests.cookies.create_cookie('accessToken', token))
-            tqdm.write('🍪 Using API token to log in')
+                requests.cookies.create_cookie("accessToken", token)
+            )
+            tqdm.write("🍪 Using API token to log in")
         except ValueError:
             pass  # No login
-        gql_endpoint = RequestsEndpoint(
-            url=gql_url, session=session, timeout=timeout)
+        gql_endpoint = RequestsEndpoint(url=gql_url, session=session, timeout=timeout)
         try:
             response_json = gql_endpoint(query=query)
             request_timed_out = False
         except allowed_retry_exceptions:
             response_json = None
             request_timed_out = True
     return response_json, request_timed_out
 
 
-def _check_snapshot_exists(*,
-                           dataset_id: str,
-                           tag: str,
-                           max_retries: int,
-                           retry_backoff: float):
+def _check_snapshot_exists(
+    *, dataset_id: str, tag: str, max_retries: int, retry_backoff: float
+):
     query = all_snapshots_query_template.substitute(dataset_id=dataset_id)
     response_json, request_timed_out = _safe_query(query)
 
     if request_timed_out and max_retries > 0:
-        tqdm.write('Request timed out while fetching list of snapshots, '
-                   'retrying …')
+        tqdm.write("Request timed out while fetching list of snapshots, " "retrying …")
         asyncio.sleep(retry_backoff)
         max_retries -= 1
         retry_backoff *= 2
-        return _check_snapshot_exists(dataset_id=dataset_id, tag=tag,
-                                      max_retries=max_retries,
-                                      retry_backoff=retry_backoff)
+        return _check_snapshot_exists(
+            dataset_id=dataset_id,
+            tag=tag,
+            max_retries=max_retries,
+            retry_backoff=retry_backoff,
+        )
     elif request_timed_out:
-        raise RuntimeError('Timeout when trying to fetch list of snapshots.')
+        raise RuntimeError("Timeout when trying to fetch list of snapshots.")
 
-    snapshots = response_json['data']['dataset']['snapshots']
-    tags = [s['id'].replace(f'{dataset_id}:', '')
-            for s in snapshots]
+    snapshots = response_json["data"]["dataset"]["snapshots"]
+    tags = [s["id"].replace(f"{dataset_id}:", "") for s in snapshots]
 
     if tag not in tags:
-        raise RuntimeError(f'The requested snapshot with the tag "{tag}" '
-                           f'does not exist for dataset {dataset_id}. '
-                           f'Existing tags: {", ".join(tags)}')
+        raise RuntimeError(
+            f'The requested snapshot with the tag "{tag}" '
+            f"does not exist for dataset {dataset_id}. "
+            f'Existing tags: {", ".join(tags)}'
+        )
 
 
-def _get_download_metadata(*,
-                           base_url: str = BASE_URL,
-                           dataset_id: str,
-                           tag: Optional[str] = None,
-                           tree: str = 'null',
-                           max_retries: int,
-                           retry_backoff: float = 0.5,
-                           check_snapshot: bool = True) -> dict:
-    """Retrieve dataset metadata required for the download.
-    """
+def _get_download_metadata(
+    *,
+    base_url: str = BASE_URL,
+    dataset_id: str,
+    tag: Optional[str] = None,
+    tree: str = "null",
+    max_retries: int,
+    retry_backoff: float = 0.5,
+    check_snapshot: bool = True,
+) -> dict:
+    """Retrieve dataset metadata required for the download."""
     if tag is None:
         query = dataset_query_template.substitute(dataset_id=dataset_id)
     else:
         if check_snapshot:
             _check_snapshot_exists(
                 dataset_id=dataset_id,
                 tag=tag,
                 max_retries=max_retries,
-                retry_backoff=retry_backoff)
-        query = snapshot_query_template.substitute(dataset_id=dataset_id,
-                                                   tag=tag, tree=tree)
+                retry_backoff=retry_backoff,
+            )
+        query = snapshot_query_template.substitute(
+            dataset_id=dataset_id, tag=tag, tree=tree
+        )
 
     response_json, request_timed_out = _safe_query(query, timeout=60)
 
     # Sometimes we do get a response, but it contains a gateway timeout error
     # message (504 or 502 status code)
-    if (response_json is not None and 'errors' in response_json and
-            response_json['errors'][0]['message'].startswith(('504', '502'))):
+    if (
+        response_json is not None
+        and "errors" in response_json
+        and response_json["errors"][0]["message"].startswith(("504", "502"))
+    ):
         request_timed_out = True
 
     if request_timed_out and max_retries > 0:
-        tqdm.write(
-            _unicode('Request timed out while fetching metadata, retrying')
-        )
+        tqdm.write(_unicode("Request timed out while fetching metadata, retrying"))
         asyncio.sleep(retry_backoff)
         max_retries -= 1
         retry_backoff *= 2
         return _get_download_metadata(
             base_url=base_url,
             dataset_id=dataset_id,
             tag=tag,
             max_retries=max_retries,
             retry_backoff=retry_backoff,
             check_snapshot=check_snapshot,
         )
     elif request_timed_out:
-        raise RuntimeError('Timeout when trying to fetch metadata.')
+        raise RuntimeError("Timeout when trying to fetch metadata.")
 
     if response_json is not None:
-        if 'errors' in response_json:
+        if "errors" in response_json:
             msg = response_json["errors"][0]["message"]
-            if msg == 'You do not have access to read this dataset.':
+            if msg == "You do not have access to read this dataset.":
                 try:
                     # Do we have an API token?
                     get_token()
-                    raise RuntimeError('We were not permitted to download '
-                                       'this dataset. Perhaps your user '
-                                       'does not have access to it, or '
-                                       'your API token is wrong.')
+                    raise RuntimeError(
+                        "We were not permitted to download "
+                        "this dataset. Perhaps your user "
+                        "does not have access to it, or "
+                        "your API token is wrong."
+                    )
                 except ValueError as e:
                     # We don't have an API token.
-                    raise RuntimeError('It seems that this is a restricted '
-                                       'dataset. However, your API token is '
-                                       'not configured properly, so we could '
-                                       f'not log you in. {e}')
+                    raise RuntimeError(
+                        "It seems that this is a restricted "
+                        "dataset. However, your API token is "
+                        "not configured properly, so we could "
+                        f"not log you in. {e}"
+                    )
             else:
                 raise RuntimeError(f'Query failed: "{msg}"')
         elif tag is None:
-            return response_json['data']['dataset']['latestSnapshot']
+            return response_json["data"]["dataset"]["latestSnapshot"]
         else:
-            return response_json['data']['snapshot']
+            return response_json["data"]["snapshot"]
     else:
-        raise RuntimeError('Error when trying to fetch metadata.')
+        raise RuntimeError("Error when trying to fetch metadata.")
 
 
-async def _download_file(*,
-                         url: str,
-                         api_file_size: int,
-                         outfile: Path,
-                         verify_hash: bool,
-                         verify_size: bool,
-                         max_retries: int,
-                         retry_backoff: float,
-                         semaphore: asyncio.Semaphore) -> None:
-    """Download an individual file.
-    """
+async def _download_file(
+    *,
+    url: str,
+    api_file_size: int,
+    outfile: Path,
+    verify_hash: bool,
+    verify_size: bool,
+    max_retries: int,
+    retry_backoff: float,
+    semaphore: asyncio.Semaphore,
+) -> None:
+    """Download an individual file."""
     if outfile.exists():
         local_file_size = outfile.stat().st_size
     else:
         local_file_size = 0
 
     # The OpenNeuro servers are sometimes very slow to respond, so use a
     # gigantic timeout for those.
-    if url.startswith('https://openneuro.org/crn/'):
+    if url.startswith("https://openneuro.org/crn/"):
         timeout = 60
     else:
         timeout = 5
 
     # Check if we need to resume a download
     # The file sizes provided via the API often do not match the sizes reported
     # by the HTTP server. Rely on the sizes reported by the HTTP server.
@@ -271,342 +281,374 @@
         async with httpx.AsyncClient(timeout=timeout) as client:
             try:
                 response = await client.head(url)
                 headers = response.headers
             except allowed_retry_exceptions:
                 if max_retries > 0:
                     await _retry_download(
-                        url=url, outfile=outfile,
+                        url=url,
+                        outfile=outfile,
                         api_file_size=api_file_size,
-                        verify_hash=verify_hash, verify_size=verify_size,
+                        verify_hash=verify_hash,
+                        verify_size=verify_size,
                         max_retries=max_retries,
-                        retry_backoff=retry_backoff, semaphore=semaphore)
+                        retry_backoff=retry_backoff,
+                        semaphore=semaphore,
+                    )
                     return
                 else:
-                    raise RuntimeError(f'Timeout when trying to download '
-                                       f'{outfile}.')
+                    raise RuntimeError(
+                        f"Timeout when trying to download " f"{outfile}."
+                    )
 
             # Try to get the S3 MD5 hash for the file.
             try:
-                remote_file_hash = headers['etag'].strip('"')
+                remote_file_hash = headers["etag"].strip('"')
                 if len(remote_file_hash) != 32:  # It's not an MD5 hash.
                     remote_file_hash = None
             except KeyError:
                 remote_file_hash = None
 
             # Get the Content-Length.
             try:
-                remote_file_size = int(response.headers['content-length'])
+                remote_file_size = int(response.headers["content-length"])
             except KeyError:
                 # The server doesn't always set a Content-Length header.
                 remote_file_size = None
 
     headers = {}
-    headers['Accept-Encoding'] = ''  # Disable compression
+    headers["Accept-Encoding"] = ""  # Disable compression
 
     if outfile.exists() and local_file_size == remote_file_size:
         hash = hashlib.md5()
 
         if verify_hash and remote_file_hash is not None:
-            async with aiofiles.open(outfile, 'rb') as f:
+            async with aiofiles.open(outfile, "rb") as f:
                 while True:
                     data = await f.read(65536)
                     if not data:
                         break
                     hash.update(data)
 
-        if (verify_hash and
-                remote_file_hash is not None and
-                hash.hexdigest() != remote_file_hash):
-            desc = f'Re-downloading {outfile.name}: file hash mismatch.'
-            mode = 'wb'
+        if (
+            verify_hash
+            and remote_file_hash is not None
+            and hash.hexdigest() != remote_file_hash
+        ):
+            desc = f"Re-downloading {outfile.name}: file hash mismatch."
+            mode = "wb"
             outfile.unlink()
             local_file_size = 0
         else:
             # Download complete, skip.
-            desc = f'Skipping {outfile.name}: already downloaded.'
-            t = tqdm(iterable=response.aiter_bytes(),
-                     desc=desc,
-                     initial=local_file_size,
-                     total=remote_file_size, unit='B',
-                     unit_scale=True,
-                     unit_divisor=1024, leave=False)
+            desc = f"Skipping {outfile.name}: already downloaded."
+            t = tqdm(
+                iterable=response.aiter_bytes(),
+                desc=desc,
+                initial=local_file_size,
+                total=remote_file_size,
+                unit="B",
+                unit_scale=True,
+                unit_divisor=1024,
+                leave=False,
+            )
             t.close()
             return
-    elif (outfile.exists() and
-            remote_file_size is not None and
-            local_file_size < remote_file_size):
+    elif (
+        outfile.exists()
+        and remote_file_size is not None
+        and local_file_size < remote_file_size
+    ):
         # Download incomplete, resume.
-        desc = f'Resuming {outfile.name}'
-        headers['Range'] = f'bytes={local_file_size}-'
-        mode = 'ab'
+        desc = f"Resuming {outfile.name}"
+        headers["Range"] = f"bytes={local_file_size}-"
+        mode = "ab"
     elif outfile.exists():
         # Local file is larger than remote – overwrite.
-        desc = f'Re-downloading {outfile.name}: file size mismatch.'
-        mode = 'wb'
+        desc = f"Re-downloading {outfile.name}: file size mismatch."
+        mode = "wb"
         outfile.unlink()
         local_file_size = 0
     else:
         # File doesn't exist locally, download entirely.
         desc = outfile.name
-        mode = 'wb'
+        mode = "wb"
 
     async with semaphore:
         async with httpx.AsyncClient(timeout=timeout) as client:
             try:
-                async with (
-                    client.stream('GET', url=url, headers=headers)
-                ) as response:
+                async with (client.stream("GET", url=url, headers=headers)) as response:
                     if not response.is_error:
                         pass  # All good!
-                    elif (response.status_code in allowed_retry_codes and
-                          max_retries > 0):
+                    elif (
+                        response.status_code in allowed_retry_codes and max_retries > 0
+                    ):
                         await _retry_download(
-                            url=url, outfile=outfile,
+                            url=url,
+                            outfile=outfile,
                             api_file_size=api_file_size,
-                            verify_hash=verify_hash, verify_size=verify_size,
+                            verify_hash=verify_hash,
+                            verify_size=verify_size,
                             max_retries=max_retries,
-                            retry_backoff=retry_backoff, semaphore=semaphore)
+                            retry_backoff=retry_backoff,
+                            semaphore=semaphore,
+                        )
                         return
                     else:
                         raise RuntimeError(
-                            f'Error {response.status_code} when trying '
-                            f'to download {outfile} from {url}')
+                            f"Error {response.status_code} when trying "
+                            f"to download {outfile} from {url}"
+                        )
 
                     await _retrieve_and_write_to_disk(
-                        response=response, outfile=outfile, mode=mode,
+                        response=response,
+                        outfile=outfile,
+                        mode=mode,
                         desc=desc,
                         local_file_size=local_file_size,
                         remote_file_size=remote_file_size,
                         remote_file_hash=remote_file_hash,
-                        verify_hash=verify_hash, verify_size=verify_size)
+                        verify_hash=verify_hash,
+                        verify_size=verify_size,
+                    )
             except allowed_retry_exceptions:
                 if max_retries > 0:
                     await _retry_download(
-                        url=url, outfile=outfile,
+                        url=url,
+                        outfile=outfile,
                         api_file_size=api_file_size,
-                        verify_hash=verify_hash, verify_size=verify_size,
+                        verify_hash=verify_hash,
+                        verify_size=verify_size,
                         max_retries=max_retries,
-                        retry_backoff=retry_backoff, semaphore=semaphore)
+                        retry_backoff=retry_backoff,
+                        semaphore=semaphore,
+                    )
                     return
                 else:
-                    raise RuntimeError(f'Timeout when trying to download '
-                                       f'{outfile}.')
+                    raise RuntimeError(
+                        f"Timeout when trying to download " f"{outfile}."
+                    )
 
 
 async def _retry_download(
     *,
     url: str,
     outfile: Path,
     api_file_size: int,
     verify_hash: bool,
     verify_size: bool,
     max_retries: int,
     retry_backoff: float,
-    semaphore: asyncio.Semaphore
+    semaphore: asyncio.Semaphore,
 ) -> None:
     tqdm.write(
-        _unicode(f'Request timed out while downloading {outfile}, retrying in '
-                 f'{retry_backoff} sec', emoji='🔄')
+        _unicode(
+            f"Request timed out while downloading {outfile}, retrying in "
+            f"{retry_backoff} sec",
+            emoji="🔄",
+        )
     )
     await asyncio.sleep(retry_backoff)
     max_retries -= 1
     retry_backoff *= 2
     semaphore.release()
-    await _download_file(url=url,
-                         api_file_size=api_file_size,
-                         outfile=outfile,
-                         verify_hash=verify_hash,
-                         verify_size=verify_size,
-                         max_retries=max_retries,
-                         retry_backoff=retry_backoff,
-                         semaphore=semaphore)
+    await _download_file(
+        url=url,
+        api_file_size=api_file_size,
+        outfile=outfile,
+        verify_hash=verify_hash,
+        verify_size=verify_size,
+        max_retries=max_retries,
+        retry_backoff=retry_backoff,
+        semaphore=semaphore,
+    )
 
 
 async def _retrieve_and_write_to_disk(
     *,
     response: httpx.Response,
     outfile: Path,
-    mode: Literal['ab', 'wb'],
+    mode: Literal["ab", "wb"],
     desc: str,
     local_file_size: int,
     remote_file_size: Optional[int],
     remote_file_hash: Optional[str],
     verify_hash: bool,
-    verify_size: bool
+    verify_size: bool,
 ) -> None:
     hash = hashlib.md5()
 
     # If we're resuming a download, ensure the already-downloaded
     # parts of the file are fed into the hash function before
     # we continue.
     if verify_hash and local_file_size > 0:
-        async with aiofiles.open(outfile, 'rb') as f:
+        async with aiofiles.open(outfile, "rb") as f:
             while True:
                 data = await f.read(65536)
                 if not data:
                     break
                 hash.update(data)
 
     async with aiofiles.open(outfile, mode=mode) as f:
-        with tqdm(desc=desc, initial=local_file_size,
-                  total=remote_file_size, unit='B',
-                  unit_scale=True, unit_divisor=1024,
-                  leave=False) as progress:
-
+        with tqdm(
+            desc=desc,
+            initial=local_file_size,
+            total=remote_file_size,
+            unit="B",
+            unit_scale=True,
+            unit_divisor=1024,
+            leave=False,
+        ) as progress:
             num_bytes_downloaded = response.num_bytes_downloaded
             # TODO Add timeout handling here, too.
             async for chunk in response.aiter_bytes():
                 await f.write(chunk)
-                progress.update(response.num_bytes_downloaded -
-                                num_bytes_downloaded)
-                num_bytes_downloaded = (response
-                                        .num_bytes_downloaded)
+                progress.update(response.num_bytes_downloaded - num_bytes_downloaded)
+                num_bytes_downloaded = response.num_bytes_downloaded
                 if verify_hash:
                     hash.update(chunk)
 
         if verify_hash and remote_file_hash is not None:
             got = hash.hexdigest()
             if got != remote_file_hash:
                 raise RuntimeError(
-                    f'Hash mismatch for:\n{outfile}\n'
-                    f'Expected:\n{remote_file_hash}\nGot:\n{got}'
+                    f"Hash mismatch for:\n{outfile}\n"
+                    f"Expected:\n{remote_file_hash}\nGot:\n{got}"
                 )
 
         # Check the file was completely downloaded.
         if verify_size:
             await f.flush()
             local_file_size = outfile.stat().st_size
-            if (remote_file_size is not None and
-                    not local_file_size == remote_file_size):
+            if remote_file_size is not None and not local_file_size == remote_file_size:
                 raise RuntimeError(
-                    f'Server claimed size of {outfile} would be '
-                    f'{remote_file_size} bytes, but downloaded '
-                    f'{local_file_size} bytes.')
+                    f"Server claimed size of {outfile} would be "
+                    f"{remote_file_size} bytes, but downloaded "
+                    f"{local_file_size} bytes."
+                )
     # Secondary check: try loading as JSON for "error" entry
     # We can get for invalid files sometimes the contents:
     # {"error": "an unknown error occurred accessing this file"}
     # This is a 58-byte file, but let's be tolerant and try loading
     # anything less than 200 as JSON and detect a dict with a single
     # "error" entry.
     if verify_size and local_file_size < 200:
         try:
-            data = json.loads(outfile.read_text('utf-8'))
+            data = json.loads(outfile.read_text("utf-8"))
         except Exception:
             pass
         else:
-            if isinstance(data, dict) and list(data) == ['error']:
+            if isinstance(data, dict) and list(data) == ["error"]:
                 raise RuntimeError(
-                    f'Error downloading:\n{outfile}:\n'
-                    f'Got JSON error response contents:\n{data}'
+                    f"Error downloading:\n{outfile}:\n"
+                    f"Got JSON error response contents:\n{data}"
                 )
 
 
-async def _download_files(*,
-                          target_dir: Path,
-                          files: Iterable[dict],
-                          verify_hash: bool,
-                          verify_size: bool,
-                          max_retries: int,
-                          retry_backoff: float,
-                          max_concurrent_downloads: int) -> None:
-    """Download files, one by one.
-    """
+async def _download_files(
+    *,
+    target_dir: Path,
+    files: Iterable[dict],
+    verify_hash: bool,
+    verify_size: bool,
+    max_retries: int,
+    retry_backoff: float,
+    max_concurrent_downloads: int,
+) -> None:
+    """Download files, one by one."""
     # Semaphore (counter) to limit maximum number of concurrent download
     # coroutines.
     semaphore = asyncio.Semaphore(max_concurrent_downloads)
     download_tasks = []
 
     for file in files:
-        filename = Path(file['filename'])
-        api_file_size = file['size']
-        url = file['urls'][0]
+        filename = Path(file["filename"])
+        api_file_size = file["size"]
+        url = file["urls"][0]
 
         outfile = target_dir / filename
         outfile.parent.mkdir(parents=True, exist_ok=True)
         download_task = _download_file(
-            url=url, api_file_size=api_file_size,
-            outfile=outfile, verify_hash=verify_hash,
-            verify_size=verify_size, max_retries=max_retries,
-            retry_backoff=retry_backoff, semaphore=semaphore)
+            url=url,
+            api_file_size=api_file_size,
+            outfile=outfile,
+            verify_hash=verify_hash,
+            verify_size=verify_size,
+            max_retries=max_retries,
+            retry_backoff=retry_backoff,
+            semaphore=semaphore,
+        )
         download_tasks.append(download_task)
 
     await asyncio.gather(*download_tasks)
 
 
-def _get_local_tag(
-    *,
-    dataset_id: str,
-    dataset_dir: Path
-) -> Optional[str]:
-    """Get the local dataset revision.
-    """
-    local_json_path = dataset_dir / 'dataset_description.json'
+def _get_local_tag(*, dataset_id: str, dataset_dir: Path) -> Optional[str]:
+    """Get the local dataset revision."""
+    local_json_path = dataset_dir / "dataset_description.json"
     if not local_json_path.exists():
         return None
 
-    local_json_file_content = local_json_path.read_text(encoding='utf-8')
+    local_json_file_content = local_json_path.read_text(encoding="utf-8")
     if not local_json_file_content:
         return None
 
     local_json = json.loads(local_json_file_content)
 
-    if 'DatasetDOI' not in local_json:
-        raise RuntimeError('Local "dataset_description.json" does not contain '
-                           '"DatasetDOI" field. Are you sure this is the '
-                           'correct directory?')
+    if "DatasetDOI" not in local_json:
+        raise RuntimeError(
+            'Local "dataset_description.json" does not contain '
+            '"DatasetDOI" field. Are you sure this is the '
+            "correct directory?"
+        )
 
-    local_doi = local_json['DatasetDOI']
-    if local_doi.startswith('doi:'):
+    local_doi = local_json["DatasetDOI"]
+    if local_doi.startswith("doi:"):
         # Remove the "protocol" prefix
         local_doi = local_doi[4:]
 
-    expected_doi_start = f'10.18112/openneuro.{dataset_id}.v'
+    expected_doi_start = f"10.18112/openneuro.{dataset_id}.v"
 
     if not local_doi.startswith(expected_doi_start):
-        raise RuntimeError(f'The existing dataset in the target directory '
-                           f'appears to be different from the one you '
-                           f'requested to download. "DatasetDOI" field in '
-                           f'local "dataset_description.json": '
-                           f'{local_json["DatasetDOI"]}. '
-                           f'Requested dataset: {dataset_id}')
+        raise RuntimeError(
+            f"The existing dataset in the target directory "
+            f"appears to be different from the one you "
+            f'requested to download. "DatasetDOI" field in '
+            f'local "dataset_description.json": '
+            f'{local_json["DatasetDOI"]}. '
+            f"Requested dataset: {dataset_id}"
+        )
 
-    local_version = (local_doi
-                     .replace(f'10.18112/openneuro.{dataset_id}.v', ''))
+    local_version = local_doi.replace(f"10.18112/openneuro.{dataset_id}.v", "")
     return local_version
 
 
-def _unicode(
-    msg: str,
-    *,
-    emoji: str = ' ',
-    end: str = '…'
-) -> str:
+def _unicode(msg: str, *, emoji: str = " ", end: str = "…") -> str:
     if stdout_unicode:
-        msg = f'{emoji} {msg} {end}'
-    elif end == '…':
-        msg = f'{msg} ...'
+        msg = f"{emoji} {msg} {end}"
+    elif end == "…":
+        msg = f"{msg} ..."
     return msg
 
 
 def _iterate_filenames(
     files: Iterable[dict],
     *,
     dataset_id: str,
     tag: str,
     max_retries: int,
-    root: str = '',
+    root: str = "",
     include: Iterable[str] = tuple(),
 ) -> Generator[dict, None, None]:
     """Iterate over all files in a dataset, yielding filenames."""
     directories = list()
     for entity in files:
         if root:
-            entity['filename'] = f'{root}/{entity["filename"]}'
-        if entity['directory']:
+            entity["filename"] = f'{root}/{entity["filename"]}'
+        if entity["directory"]:
             directories.append(entity)
         else:
             yield entity
 
     for directory in directories:
         # Only bother with directories that are in the include list
         if include:
@@ -623,37 +665,38 @@
             # --include="sub-CON001/*"
             #
             # All three of these should traverse `sub-CON001` and its
             # subdirectories.
             n_parts = len(PurePosixPath(root).parts)
             dir_include = [PurePosixPath(inc) for inc in include]
             dir_include = [  # for stuff like sub-CON001/*
-                '/'.join(inc.parts[:n_parts] + ('*',))
+                "/".join(inc.parts[:n_parts] + ("*",))
                 for inc in dir_include
                 if len(inc.parts) >= n_parts
             ] + [  # and stuff like sub-CON001/*.eeg
-                '/'.join(inc.parts[:n_parts - 1] + ('*',))
+                "/".join(inc.parts[: n_parts - 1] + ("*",))
                 for inc in dir_include
                 if len(inc.parts) >= n_parts - 1 and len(inc.parts) > 1
             ]  # we want to traverse sub-CON001 in both cases
             matches_include, _ = _match_include_exclude(
-                directory['filename'], include=dir_include, exclude=[])
+                directory["filename"], include=dir_include, exclude=[]
+            )
             if dir_include and not any(matches_include):
                 continue
         # Query filenames
-        this_dir = directory['filename']
+        this_dir = directory["filename"]
         metadata = _get_download_metadata(
             dataset_id=dataset_id,
             tag=tag,
             tree=f'"{directory["id"]}"',
             max_retries=max_retries,
             check_snapshot=False,
         )
         dir_iterator = _iterate_filenames(
-            metadata['files'],
+            metadata["files"],
             dataset_id=dataset_id,
             tag=tag,
             max_retries=max_retries,
             root=this_dir,
             include=include,
         )
         for path in dir_iterator:
@@ -663,32 +706,35 @@
 def _match_include_exclude(
     filename: str,
     *,
     include: Iterable[str],
     exclude: Iterable[str],
 ) -> bool:
     """Check if a filename matches an include or exclude pattern."""
-    matches_keep = [filename.startswith(i) or fnmatch.fnmatch(filename, i)
-                    for i in include]
-    matches_remove = [filename.startswith(e) or
-                      fnmatch.fnmatch(filename, e)
-                      for e in exclude]
+    matches_keep = [
+        filename.startswith(i) or fnmatch.fnmatch(filename, i) for i in include
+    ]
+    matches_remove = [
+        filename.startswith(e) or fnmatch.fnmatch(filename, e) for e in exclude
+    ]
     return matches_keep, matches_remove
 
 
-def download(*,
-             dataset: str,
-             tag: Optional[str] = None,
-             target_dir: Optional[Union[Path, str]] = None,
-             include: Optional[Iterable[str]] = None,
-             exclude: Optional[Iterable[str]] = None,
-             verify_hash: bool = True,
-             verify_size: bool = True,
-             max_retries: int = 5,
-             max_concurrent_downloads: int = 5) -> None:
+def download(
+    *,
+    dataset: str,
+    tag: Optional[str] = None,
+    target_dir: Optional[Union[Path, str]] = None,
+    include: Optional[Iterable[str]] = None,
+    exclude: Optional[Iterable[str]] = None,
+    verify_hash: bool = True,
+    verify_size: bool = True,
+    max_retries: int = 5,
+    max_concurrent_downloads: int = 5,
+) -> None:
     """Download datasets from OpenNeuro.
 
     Parameters
     ----------
     dataset
         The dataset to retrieve, for example ``ds000248``.
     tag
@@ -712,28 +758,30 @@
         Whether to check if the downloaded file size matches what the server
         announced.
     max_retries
         Try the specified number of times to download a file before failing.
     max_concurrent_downloads
         The maximum number of downloads to run in parallel.
     """
-    msg_problems = 'problems 🤯' if stdout_unicode else 'problems'
-    msg_bugs = 'bugs 🪲' if stdout_unicode else 'bugs'
-    msg_hello = '👋 Hello!' if stdout_unicode else 'Hello!'
-    msg_great_to_see_you = 'Great to see you!'
+    msg_problems = "problems 🤯" if stdout_unicode else "problems"
+    msg_bugs = "bugs 🪲" if stdout_unicode else "bugs"
+    msg_hello = "👋 Hello!" if stdout_unicode else "Hello!"
+    msg_great_to_see_you = "Great to see you!"
     if stdout_unicode:
-        msg_great_to_see_you += ' 🤗'
-    msg_please = '👉 Please' if stdout_unicode else '   Please'
+        msg_great_to_see_you += " 🤗"
+    msg_please = "👉 Please" if stdout_unicode else "   Please"
 
-    msg = (f'\n{msg_hello} This is openneuro-py {__version__}. '
-           f'{msg_great_to_see_you}\n\n'
-           f'   {msg_please} report {msg_problems} and {msg_bugs} at\n'
-           f'      https://github.com/hoechenberger/openneuro-py/issues\n')
+    msg = (
+        f"\n{msg_hello} This is openneuro-py {__version__}. "
+        f"{msg_great_to_see_you}\n\n"
+        f"   {msg_please} report {msg_problems} and {msg_bugs} at\n"
+        f"      https://github.com/hoechenberger/openneuro-py/issues\n"
+    )
     tqdm.write(msg)
-    tqdm.write(_unicode(f'Preparing to download {dataset}', emoji='🌍'))
+    tqdm.write(_unicode(f"Preparing to download {dataset}", emoji="🌍"))
 
     if target_dir is None:
         target_dir = Path(dataset)
     else:
         target_dir = Path(target_dir)
     target_dir = target_dir.expanduser().resolve()
 
@@ -747,141 +795,169 @@
     metadata = _get_download_metadata(
         dataset_id=dataset,
         tag=tag,
         max_retries=max_retries,
         retry_backoff=retry_backoff,
     )
     del tag
-    tag = metadata['id'].replace(f'{dataset}:', '')
+    tag = metadata["id"].replace(f"{dataset}:", "")
     if target_dir.exists():
-        target_dir_empty = len(list(target_dir.rglob('*'))) == 0
+        target_dir_empty = len(list(target_dir.rglob("*"))) == 0
 
         if not target_dir_empty:
-            local_tag = _get_local_tag(dataset_id=dataset,
-                                       dataset_dir=target_dir)
+            local_tag = _get_local_tag(dataset_id=dataset, dataset_dir=target_dir)
 
             if local_tag is None:
-                tqdm.write('Cannot determine local revision of the dataset, '
-                           'and the target directory is not empty. If the '
-                           'download fails, you may want to try again with a '
-                           'fresh (empty) target directory.')
+                tqdm.write(
+                    "Cannot determine local revision of the dataset, "
+                    "and the target directory is not empty. If the "
+                    "download fails, you may want to try again with a "
+                    "fresh (empty) target directory."
+                )
             elif local_tag != tag:
                 raise FileExistsError(
-                    f'You requested to download revision {tag}, but '
-                    f'revision {local_tag} exists locally in the designated '
-                    f'target directory. Please either remove this dataset or '
-                    f'specify a different target directory, and try again.'
+                    f"You requested to download revision {tag}, but "
+                    f"revision {local_tag} exists locally in the designated "
+                    f"target directory. Please either remove this dataset or "
+                    f"specify a different target directory, and try again."
                 )
 
     files = []
     include_counts = [0] * len(include)  # Keep track of include matches.
     filenames = []
-    these_files = metadata['files']
+    these_files = metadata["files"]
     del metadata
 
     for file in tqdm(
         _iterate_filenames(
-            these_files, dataset_id=dataset, tag=tag, max_retries=max_retries,
+            these_files,
+            dataset_id=dataset,
+            tag=tag,
+            max_retries=max_retries,
             include=include,
         ),
-        desc=_unicode(
-            f'Traversing directories for {dataset}', end='', emoji='📁'
-        ),
-        unit=' entities'
+        desc=_unicode(f"Traversing directories for {dataset}", end="", emoji="📁"),
+        unit=" entities",
     ):
-        filename: str = file['filename']  # TODO properly define metadata type
+        filename: str = file["filename"]  # TODO properly define metadata type
         filenames.append(filename)
 
         # Always include essential BIDS files.
-        if filename in ('dataset_description.json',
-                        'participants.tsv',
-                        'participants.json',
-                        'README',
-                        'CHANGES'):
+        if filename in (
+            "dataset_description.json",
+            "participants.tsv",
+            "participants.json",
+            "README",
+            "CHANGES",
+        ):
             files.append(file)
             # Keep track of include matches.
             if filename in include:
                 include_counts[include.index(filename)] += 1
             continue
 
         matches_keep, matches_exclude = _match_include_exclude(
-            filename, include=include, exclude=exclude)
+            filename, include=include, exclude=exclude
+        )
         if (not include or any(matches_keep)) and not any(matches_exclude):
             files.append(file)
             # Keep track of include matches.
             if any(matches_keep):
                 include_counts[matches_keep.index(True)] += 1
 
     if include:
         for idx, count in enumerate(include_counts):
             if count == 0:
                 this = include[idx]
                 maybe = get_close_matches(this, filenames)
                 if maybe:
                     extra = (
-                        'Perhaps you mean one of these paths:\n- ' +
-                        '\n- '.join(maybe) + '\n'
+                        "Perhaps you mean one of these paths:\n- "
+                        + "\n- ".join(maybe)
+                        + "\n"
                     )
                 else:
-                    extra = (
-                        'There were no similar filenames found in the '
-                        'metadata. '
-                    )
+                    extra = "There were no similar filenames found in the " "metadata. "
                 raise RuntimeError(
-                    f'Could not find path in the dataset:\n- {this}\n{extra}'
-                    'Please check your includes.'
+                    f"Could not find path in the dataset:\n- {this}\n{extra}"
+                    "Please check your includes."
                 )
 
-    msg = (f'Retrieving up to {len(files)} files '
-           f'({max_concurrent_downloads} concurrent downloads).')
-    tqdm.write(_unicode(msg, emoji='📥', end=''))
-
-    kwargs = dict(target_dir=target_dir,
-                  files=files,
-                  verify_hash=verify_hash,
-                  verify_size=verify_size,
-                  max_retries=max_retries,
-                  retry_backoff=retry_backoff,
-                  max_concurrent_downloads=max_concurrent_downloads)
+    msg = (
+        f"Retrieving up to {len(files)} files "
+        f"({max_concurrent_downloads} concurrent downloads)."
+    )
+    tqdm.write(_unicode(msg, emoji="📥", end=""))
+
+    kwargs = dict(
+        target_dir=target_dir,
+        files=files,
+        verify_hash=verify_hash,
+        verify_size=verify_size,
+        max_retries=max_retries,
+        retry_backoff=retry_backoff,
+        max_concurrent_downloads=max_concurrent_downloads,
+    )
 
     # Try to re-use event loop if it already exists. This is required e.g.
     # for use in Jupyter notebooks.
     try:
         loop = asyncio.get_running_loop()
     except RuntimeError:
         loop = None
 
     if loop:
         loop.create_task(_download_files(**kwargs))
     else:
         asyncio.run(_download_files(**kwargs))
 
-    tqdm.write(
-        _unicode(f'Finished downloading {dataset}.\n', emoji='✅', end='')
-    )
-    tqdm.write(_unicode('Please enjoy your brains.\n', emoji='🧠', end=''))
+    tqdm.write(_unicode(f"Finished downloading {dataset}.\n", emoji="✅", end=""))
+    tqdm.write(_unicode("Please enjoy your brains.\n", emoji="🧠", end=""))
 
 
 @click.command()
-@click.option('--dataset', required=True, help='The OpenNeuro dataset name.')
-@click.option('--tag', help='The tag (version) of the dataset.')
-@click.option('--target_dir', help='The directory to download to.')
-@click.option('--include', multiple=True,
-              help='Only include the specified file or directory. Can be '
-                   'passed multiple times.')
-@click.option('--exclude', multiple=True,
-              help='Exclude the specified file or directory. Can be passed '
-                   'multiple times.')
-@click.option('--verify_hash', type=bool, default=True, show_default=True,
-              help='Whether to print the SHA256 hash of each downloaded file.')
-@click.option('--verify_size', type=bool, default=True, show_default=True,
-              help='Whether to check the downloaded file size matches what '
-                   'the server announced.')
-@click.option('--max_retries', type=int, default=5, show_default=True,
-              help='Try the specified number of times to download a file '
-                   'before failing.')
-@click.option('--max_concurrent_downloads', type=int, default=5,
-              show_default=True,
-              help='The maximum number of downloads to run in parallel.')
+@click.option("--dataset", required=True, help="The OpenNeuro dataset name.")
+@click.option("--tag", help="The tag (version) of the dataset.")
+@click.option("--target_dir", help="The directory to download to.")
+@click.option(
+    "--include",
+    multiple=True,
+    help="Only include the specified file or directory. Can be "
+    "passed multiple times.",
+)
+@click.option(
+    "--exclude",
+    multiple=True,
+    help="Exclude the specified file or directory. Can be passed " "multiple times.",
+)
+@click.option(
+    "--verify_hash",
+    type=bool,
+    default=True,
+    show_default=True,
+    help="Whether to print the SHA256 hash of each downloaded file.",
+)
+@click.option(
+    "--verify_size",
+    type=bool,
+    default=True,
+    show_default=True,
+    help="Whether to check the downloaded file size matches what "
+    "the server announced.",
+)
+@click.option(
+    "--max_retries",
+    type=int,
+    default=5,
+    show_default=True,
+    help="Try the specified number of times to download a file " "before failing.",
+)
+@click.option(
+    "--max_concurrent_downloads",
+    type=int,
+    default=5,
+    show_default=True,
+    help="The maximum number of downloads to run in parallel.",
+)
 def download_cli(**kwargs):
     """Download datasets from OpenNeuro."""
     download(**kwargs)
```

### Comparing `openneuro-py-2022.4.0/openneuro/config.py` & `openneuro-py-2023.1.0/openneuro/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,61 +1,58 @@
 from pathlib import Path
 import os
-import sys
 import stat
 import json
 import getpass
-if sys.version_info >= (3, 8):
-    from typing import TypedDict
-else:
-    from typing_extensions import TypedDict
+from typing import TypedDict
 
-import appdirs
+import platformdirs
 from tqdm.auto import tqdm
 
 
 CONFIG_DIR = Path(
-    appdirs.user_config_dir(appname='openneuro-py', appauthor=False, roaming=True)
+    platformdirs.user_config_dir(appname="openneuro-py", appauthor=False, roaming=True)
 )
 CONFIG_DIR.mkdir(parents=True, exist_ok=True)
-CONFIG_PATH = CONFIG_DIR / 'config.json'
-BASE_URL = 'https://openneuro.org/'
+CONFIG_PATH = CONFIG_DIR / "config.json"
+BASE_URL = "https://openneuro.org/"
 
 
 class Config(TypedDict):
     endpoint: str
     apikey: str
 
 
 def init_config() -> None:
-    """Initialize a new OpenNeuro configuration file.
-    """
-    tqdm.write('🙏 Please login to your OpenNeuro account and go to: '
-               'My Account → Obtain an API Key')
-    api_key = getpass.getpass('OpenNeuro API key (input hidden): ')
+    """Initialize a new OpenNeuro configuration file."""
+    tqdm.write(
+        "🙏 Please login to your OpenNeuro account and go to: "
+        "My Account → Obtain an API Key"
+    )
+    api_key = getpass.getpass("OpenNeuro API key (input hidden): ")
 
     config: Config = {
-        'endpoint': BASE_URL,
-        'apikey': api_key,
+        "endpoint": BASE_URL,
+        "apikey": api_key,
     }
 
-    with open(CONFIG_PATH, 'w', encoding='utf-8') as f:
+    with open(CONFIG_PATH, "w", encoding="utf-8") as f:
         json.dump(config, f, indent=2)
     os.chmod(CONFIG_PATH, stat.S_IRUSR | stat.S_IWUSR)
 
 
 def load_config() -> dict:
     """Load an OpenNeuro configuration file, and return its contents.
 
     Returns
     -------
     dict
         The configuration options.
     """
-    with open(CONFIG_PATH, 'r', encoding='utf-8') as f:
+    with open(CONFIG_PATH, "r", encoding="utf-8") as f:
         config = json.load(f)
     return config
 
 
 def get_token() -> str:
     """Get the OpenNeuro API token if configured with the 'login' command.
 
@@ -66,16 +63,18 @@
     Raises
     ------
     ValueError
         When no token has been configured yet.
     """
     if not CONFIG_PATH.exists():
         raise ValueError(
-            'Could not read API token as no openneuro-py configuration '
+            "Could not read API token as no openneuro-py configuration "
             'file exists. Run "openneuro login" to generate it.'
         )
     config = load_config()
-    if 'apikey' not in config:
-        raise ValueError('An openneuro-py configuration file was found, but did not '
-                         'contain an "apikey" entry. Run "openneuro login" to '
-                         'add such an entry.')
-    return config['apikey']
+    if "apikey" not in config:
+        raise ValueError(
+            "An openneuro-py configuration file was found, but did not "
+            'contain an "apikey" entry. Run "openneuro login" to '
+            "add such an entry."
+        )
+    return config["apikey"]
```

### Comparing `openneuro-py-2022.4.0/openneuro/openneuro.py` & `openneuro-py-2023.1.0/openneuro/openneuro.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,20 +10,19 @@
 from ._download import login, download_cli
 from . import __version__
 
 
 @click.group()
 @click.version_option(version=__version__)
 def cli() -> None:
-    """Access OpenNeuro datasets.
-    """
+    """Access OpenNeuro datasets."""
     pass
 
 
 @click.command()
 def login_cli():
     """Login to OpenNeuro and store an access token."""
     login()
 
 
-cli.add_command(download_cli, name='download')
-cli.add_command(login_cli, name='login')
+cli.add_command(download_cli, name="download")
+cli.add_command(login_cli, name="login")
```

### Comparing `openneuro-py-2022.4.0/openneuro/tests/test_config.py` & `openneuro-py-2023.1.0/openneuro/tests/test_config.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 import openneuro
 from openneuro.config import init_config, load_config, get_token, Config
 
 
 def test_config(tmp_path: Path):
     """Test creating and reading the config file."""
-    with mock.patch.object(openneuro.config, 'CONFIG_PATH', tmp_path / '.openneuro'):
+    with mock.patch.object(openneuro.config, "CONFIG_PATH", tmp_path / ".openneuro"):
         assert not openneuro.config.CONFIG_PATH.exists()
 
-        with mock.patch('getpass.getpass', lambda _: 'test'):
+        with mock.patch("getpass.getpass", lambda _: "test"):
             init_config()
         assert openneuro.config.CONFIG_PATH.exists()
 
-        expected_config = Config(endpoint='https://openneuro.org/', apikey='test')
+        expected_config = Config(endpoint="https://openneuro.org/", apikey="test")
         assert load_config() == expected_config
-        assert get_token() == 'test'
+        assert get_token() == "test"
```

### Comparing `openneuro-py-2022.4.0/openneuro/tests/test_download.py` & `openneuro-py-2023.1.0/openneuro/tests/test_download.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,148 +3,132 @@
 
 import pytest
 from unittest import mock
 import openneuro
 from openneuro import download
 
 
-dataset_id_aws = 'ds000246'
-tag_aws = '1.0.0'
-include_aws = 'sub-0001/anat'
+dataset_id_aws = "ds000246"
+tag_aws = "1.0.0"
+include_aws = "sub-0001/anat"
 exclude_aws = []
 
-dataset_id_on = 'ds000117'
+dataset_id_on = "ds000117"
 tag_on = None
-include_on = 'sub-16/ses-meg'
-exclude_on = '*.fif'  # save GBs of downloads
+include_on = "sub-16/ses-meg"
+exclude_on = "*.fif"  # save GBs of downloads
 
-invalid_tag = 'abcdefg'
+invalid_tag = "abcdefg"
 
 
 @pytest.mark.parametrize(
-    ('dataset_id', 'tag', 'include', 'exclude'),
+    ("dataset_id", "tag", "include", "exclude"),
     [
         (dataset_id_aws, tag_aws, include_aws, exclude_aws),
         (dataset_id_on, tag_on, include_on, exclude_on),
-    ]
+    ],
 )
 def test_download(tmp_path: Path, dataset_id, tag, include, exclude):
     """Test downloading some files."""
-    download(dataset=dataset_id, tag=tag, target_dir=tmp_path, include=include,
-             exclude=exclude)
+    download(
+        dataset=dataset_id,
+        tag=tag,
+        target_dir=tmp_path,
+        include=include,
+        exclude=exclude,
+    )
 
 
-def test_download_invalid_tag(tmp_path: Path, dataset_id=dataset_id_aws,
-                              invalid_tag=invalid_tag):
+def test_download_invalid_tag(
+    tmp_path: Path, dataset_id=dataset_id_aws, invalid_tag=invalid_tag
+):
     """Test handling of a non-existent tag."""
-    with pytest.raises(RuntimeError, match='snapshot.*does not exist'):
+    with pytest.raises(RuntimeError, match="snapshot.*does not exist"):
         download(dataset=dataset_id, tag=invalid_tag, target_dir=tmp_path)
 
 
 def test_resume_download(tmp_path: Path):
     """Test resuming of a dataset download."""
-    dataset = 'ds000246'
-    tag = '1.0.0'
-    include = ['CHANGES']
-    download(dataset=dataset, tag=tag, target_dir=tmp_path,
-             include=include)
+    dataset = "ds000246"
+    tag = "1.0.0"
+    include = ["CHANGES"]
+    download(dataset=dataset, tag=tag, target_dir=tmp_path, include=include)
 
     # Download some more files
-    include = ['sub-0001/meg/*.jpg']
-    download(dataset=dataset, tag=tag, target_dir=tmp_path,
-             include=include)
+    include = ["sub-0001/meg/*.jpg"]
+    download(dataset=dataset, tag=tag, target_dir=tmp_path, include=include)
 
     # Download from a different revision / tag
-    new_tag = '00001'
-    include = ['CHANGES']
-    with pytest.raises(FileExistsError, match=f'revision {tag} exists'):
-        download(dataset=dataset, tag=new_tag, target_dir=tmp_path,
-                 include=include)
+    new_tag = "00001"
+    include = ["CHANGES"]
+    with pytest.raises(FileExistsError, match=f"revision {tag} exists"):
+        download(dataset=dataset, tag=new_tag, target_dir=tmp_path, include=include)
 
     # Try to "resume" from a different dataset
-    new_dataset = 'ds000117'
-    with pytest.raises(RuntimeError,
-                       match='existing dataset.*appears to be different'):
+    new_dataset = "ds000117"
+    with pytest.raises(RuntimeError, match="existing dataset.*appears to be different"):
         download(dataset=new_dataset, target_dir=tmp_path, include=include)
 
     # Remove "DatasetDOI" from JSON
-    json_path = tmp_path / 'dataset_description.json'
-    with json_path.open('r', encoding='utf-8') as f:
+    json_path = tmp_path / "dataset_description.json"
+    with json_path.open("r", encoding="utf-8") as f:
         dataset_json = json.load(f)
 
-    del dataset_json['DatasetDOI']
-    with json_path.open('w', encoding='utf-8') as f:
+    del dataset_json["DatasetDOI"]
+    with json_path.open("w", encoding="utf-8") as f:
         json.dump(dataset_json, f)
 
-    with pytest.raises(RuntimeError,
-                       match=r'does not contain "DatasetDOI"'):
+    with pytest.raises(RuntimeError, match=r'does not contain "DatasetDOI"'):
         download(dataset=dataset, target_dir=tmp_path)
 
     # We should be able to resume a download even if "datset_description.jon"
     # is missing
     json_path.unlink()
-    include = ['sub-0001/meg/sub-0001_coordsystem.json']
-    download(dataset=dataset, tag=tag, target_dir=tmp_path,
-             include=include)
+    include = ["sub-0001/meg/sub-0001_coordsystem.json"]
+    download(dataset=dataset, tag=tag, target_dir=tmp_path, include=include)
 
 
 def test_ds000248(tmp_path: Path):
     """Test a dataset for that we ship default excludes."""
-    dataset = 'ds000248'
-    download(
-        dataset=dataset,
-        include=['participants.tsv'],
-        target_dir=tmp_path
-    )
+    dataset = "ds000248"
+    download(dataset=dataset, include=["participants.tsv"], target_dir=tmp_path)
 
 
 def test_doi_handling(tmp_path: Path):
     """Test that we can handle DOIs that start with 'doi:`."""
-    dataset = 'ds000248'
-    download(
-        dataset=dataset,
-        include=['participants.tsv'],
-        target_dir=tmp_path
-    )
+    dataset = "ds000248"
+    download(dataset=dataset, include=["participants.tsv"], target_dir=tmp_path)
 
     # Now inject a `doi:` prefix into the DOI
-    dataset_description_path = tmp_path / 'dataset_description.json'
-    dataset_description_text = \
-        dataset_description_path.read_text(encoding='utf-8')
+    dataset_description_path = tmp_path / "dataset_description.json"
+    dataset_description_text = dataset_description_path.read_text(encoding="utf-8")
     dataset_description = json.loads(dataset_description_text)
     # Make sure we can dumps to get the same thing back (if they change their
     # indent 4->8 for example, we might try to resume our download of the file
     # and things will break in a challenging way)
     dataset_description_rt = json.dumps(dataset_description, indent=4)
     assert dataset_description_text == dataset_description_rt
     # Ensure the dataset doesn't already have the problematic prefix, then add
-    assert not dataset_description['DatasetDOI'].startswith('doi:')
-    dataset_description['DatasetDOI'] = (
-        'doi:' + dataset_description['DatasetDOI']
-    )
+    assert not dataset_description["DatasetDOI"].startswith("doi:")
+    dataset_description["DatasetDOI"] = "doi:" + dataset_description["DatasetDOI"]
     dataset_description_path.write_text(
-        data=json.dumps(dataset_description, indent=4),
-        encoding='utf-8'
+        data=json.dumps(dataset_description, indent=4), encoding="utf-8"
     )
 
     # Try to download again
-    download(
-        dataset=dataset,
-        include=['participants.tsv'],
-        target_dir=tmp_path
-    )
+    download(dataset=dataset, include=["participants.tsv"], target_dir=tmp_path)
 
 
 def test_restricted_dataset(tmp_path: Path):
     """Test downloading a restricted dataset."""
     # API token for dummy user alijflsdvbjielsdlkjfeiljsvj@gmail.com
-    token = 'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxOGNhNjE2ZS00OWQxLTRmOTUtODI1OS0xNzYwYzVhYjZjMDciLCJlbWFpbCI6ImFsaWpmbHNkdmJqaWVsc2Rsa2pmZWlsanN2akBnbWFpbC5jb20iLCJwcm92aWRlciI6Imdvb2dsZSIsIm5hbWUiOiJzZGZrbGVpamZsa3NkamYgc2xmZGRsa2phYWlmbCIsImFkbWluIjpmYWxzZSwiaWF0IjoxNjY1NDY4MjM4LCJleHAiOjE2OTcwMDQyMzh9.7YVL_Cagli84nTmumdcmrV1bW5hZMq3VJlMUDmTEpGU'  # noqa
+    token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxOGNhNjE2ZS00OWQxLTRmOTUtODI1OS0xNzYwYzVhYjZjMDciLCJlbWFpbCI6ImFsaWpmbHNkdmJqaWVsc2Rsa2pmZWlsanN2akBnbWFpbC5jb20iLCJwcm92aWRlciI6Imdvb2dsZSIsIm5hbWUiOiJzZGZrbGVpamZsa3NkamYgc2xmZGRsa2phYWlmbCIsImFkbWluIjpmYWxzZSwiaWF0IjoxNjY1NDY4MjM4LCJleHAiOjE2OTcwMDQyMzh9.7YVL_Cagli84nTmumdcmrV1bW5hZMq3VJlMUDmTEpGU"  # noqa
 
-    with mock.patch.object(openneuro.config, 'CONFIG_PATH', tmp_path / '.openneuro'):
-        with mock.patch('getpass.getpass', lambda _: token):
+    with mock.patch.object(openneuro.config, "CONFIG_PATH", tmp_path / ".openneuro"):
+        with mock.patch("getpass.getpass", lambda _: token):
             openneuro.config.init_config()
 
         # This is a restricted dataset that is only available if the API token
         # was used correctly.
-        download(dataset='ds004287', target_dir=tmp_path)
+        download(dataset="ds004287", target_dir=tmp_path)
 
-    assert (tmp_path / 'README').exists()
+    assert (tmp_path / "README").exists()
```

### Comparing `openneuro-py-2022.4.0/openneuro-py.gif` & `openneuro-py-2023.1.0/openneuro-py.gif`

 * *Files identical despite different names*

### Comparing `openneuro-py-2022.4.0/openneuro_py.egg-info/PKG-INFO` & `openneuro-py-2023.1.0/openneuro_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openneuro-py
-Version: 2022.4.0
+Version: 2023.1.0
 Summary: A Python client for OpenNeuro.
 Author-email: Richard Höchenberger <richard.hoechenberger@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -679,15 +679,15 @@
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: homepage, https://github.com/hoechenberger/openneuro-py
 Project-URL: changelog, https://github.com/hoechenberger/openneuro-py/CHANGES.md
 Keywords: science,neuroscience
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # openneuro-py
 
 A Python client for accessing [OpenNeuro](https://openneuro.org)
```

### Comparing `openneuro-py-2022.4.0/openneuro_py.egg-info/SOURCES.txt` & `openneuro-py-2023.1.0/openneuro_py.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+.git-blame-ignore-revs
 .gitignore
+.pre-commit-config.yaml
 CHANGES.md
 LICENSE
 README.md
 openneuro-py.gif
 pyproject.toml
 .github/dependabot.yml
 .github/workflows/codeql-analysis.yml
```

### Comparing `openneuro-py-2022.4.0/pyproject.toml` & `openneuro-py-2023.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "openneuro-py"
 description = "A Python client for OpenNeuro."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["science", "neuroscience"]
 authors = [
   {name = "Richard Höchenberger", email = "richard.hoechenberger@gmail.com"},
 ]
 classifiers = [
   "Intended Audience :: Science/Research",
@@ -15,17 +15,15 @@
 dependencies = [
     "httpx >= 0.15",
     "requests",
     "tqdm",
     "click",
     "aiofiles",
     "sgqlc",
-    "importlib-metadata; python_version < '3.8'",
-    "typing-extensions; python_version < '3.8'",
-    "appdirs",
+    "platformdirs",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 tests = [
     "pytest"
 ]
```

