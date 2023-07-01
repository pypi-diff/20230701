# Comparing `tmp/revChatGPT-6.7.3.tar.gz` & `tmp/revChatGPT-6.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.7.3.tar", last modified: Fri Jun 30 16:00:19 2023, max compression
+gzip compressed data, was "revChatGPT-6.7.4.tar", last modified: Sat Jul  1 06:25:05 2023, max compression
```

## Comparing `revChatGPT-6.7.3.tar` & `revChatGPT-6.7.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:00:19.895680 revChatGPT-6.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-30 15:59:44.000000 revChatGPT-6.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-30 16:00:19.895680 revChatGPT-6.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-30 16:00:19.000000 revChatGPT-6.7.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-30 16:00:19.895680 revChatGPT-6.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-30 15:59:44.000000 revChatGPT-6.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:00:19.887680 revChatGPT-6.7.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:00:19.891680 revChatGPT-6.7.3/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    60830 2023-06-30 15:59:44.000000 revChatGPT-6.7.3/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    25039 2023-06-30 15:59:44.000000 revChatGPT-6.7.3/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-30 15:59:44.000000 revChatGPT-6.7.3/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-30 15:59:44.000000 revChatGPT-6.7.3/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:00:19.891680 revChatGPT-6.7.3/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-30 15:59:44.000000 revChatGPT-6.7.3/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-30 15:59:44.000000 revChatGPT-6.7.3/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-30 15:59:44.000000 revChatGPT-6.7.3/src/revChatGPT/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 15:59:44.000000 revChatGPT-6.7.3/src/revChatGPT/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:00:19.891680 revChatGPT-6.7.3/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-30 16:00:19.000000 revChatGPT-6.7.3/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-30 16:00:19.000000 revChatGPT-6.7.3/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:00:19.000000 revChatGPT-6.7.3/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-30 16:00:19.000000 revChatGPT-6.7.3/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-30 16:00:19.000000 revChatGPT-6.7.3/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:00:19.895680 revChatGPT-6.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-30 15:59:44.000000 revChatGPT-6.7.3/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:25:05.938345 revChatGPT-6.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-01 06:24:37.000000 revChatGPT-6.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-07-01 06:25:05.942345 revChatGPT-6.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-01 06:25:05.000000 revChatGPT-6.7.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-01 06:25:05.942345 revChatGPT-6.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-01 06:24:37.000000 revChatGPT-6.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:25:05.938345 revChatGPT-6.7.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:25:05.938345 revChatGPT-6.7.4/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    60837 2023-07-01 06:24:37.000000 revChatGPT-6.7.4/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25039 2023-07-01 06:24:37.000000 revChatGPT-6.7.4/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-01 06:24:37.000000 revChatGPT-6.7.4/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-01 06:24:37.000000 revChatGPT-6.7.4/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:25:05.938345 revChatGPT-6.7.4/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-01 06:24:37.000000 revChatGPT-6.7.4/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-01 06:24:37.000000 revChatGPT-6.7.4/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-01 06:24:37.000000 revChatGPT-6.7.4/src/revChatGPT/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-01 06:24:37.000000 revChatGPT-6.7.4/src/revChatGPT/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:25:05.938345 revChatGPT-6.7.4/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-07-01 06:25:05.000000 revChatGPT-6.7.4/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-01 06:25:05.000000 revChatGPT-6.7.4/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 06:25:05.000000 revChatGPT-6.7.4/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-01 06:25:05.000000 revChatGPT-6.7.4/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-01 06:25:05.000000 revChatGPT-6.7.4/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:25:05.938345 revChatGPT-6.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-01 06:24:37.000000 revChatGPT-6.7.4/tests/test_recipient.py
```

### Comparing `revChatGPT-6.7.3/LICENSE` & `revChatGPT-6.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.3/PKG-INFO` & `revChatGPT-6.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.7.3
+Version: 6.7.4
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.7.3/README.md` & `revChatGPT-6.7.4/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.3/setup.py` & `revChatGPT-6.7.4/setup.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.3/src/revChatGPT/V1.py` & `revChatGPT-6.7.4/src/revChatGPT/V1.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,18 +12,20 @@
 import subprocess
 import sys
 import time
 import uuid
 from functools import wraps
 from os import environ
 from os import getenv
+from os import startfile
 from pathlib import Path
 from typing import AsyncGenerator
 from typing import Generator
 from typing import NoReturn
+import tempfile
 
 # Import function type
 from typing import Callable as function
 
 import httpx
 import requests
 import tls_client
@@ -118,46 +120,40 @@
 session = tls_client.Session(
     client_identifier="firefox110",
     random_tls_extension_order=True,
 )
 
 
 def captcha_solver(images: list[str], challenge_details: dict) -> int:
-    # mkdir captcha
-    if not Path("captcha").exists():
-        Path("captcha").mkdir()
-
-    filenames: list[Path] = []
-
-    for image in images:
-        filename = Path("captcha", f"{time.time()}.jpeg")
-        with open(filename, "wb") as f:
-            f.write(base64.b64decode(image))
-        print(f"Saved captcha image to {filename}")
-        # If MacOS, open the image
-        if sys.platform == "darwin":
-            subprocess.call(["open", filename])
-        if sys.platform == "linux":
-            subprocess.call(["xdg-open", filename])
-        if sys.platform == "win32":
-            subprocess.call(["start", filename])
-        filenames.append(filename)
-
-    print(f'Captcha instructions: {challenge_details.get("instructions")}')
-    print(
-        "Developer instructions: The captcha images have an index starting from 0 from left to right",
-    )
-    print("Enter the index of the images that matches the captcha instructions:")
-    index = int(input())
-
-    # Delete the images
-    for filename in filenames:
-        filename.unlink()
+    # Create tempfile
+    with tempfile.TemporaryDirectory() as tempdir:
+        filenames: list[Path] = []
+
+        for image in images:
+            filename = Path(tempdir, f"{time.time()}.jpeg")
+            with open(filename, "wb") as f:
+                f.write(base64.b64decode(image))
+            print(f"Saved captcha image to {filename}")
+            # If MacOS, open the image
+            if sys.platform == "darwin":
+                subprocess.call(["open", filename])
+            if sys.platform == "linux":
+                subprocess.call(["xdg-open", filename])
+            if sys.platform == "win32":
+                startfile(filename)
+            filenames.append(filename)
+
+        print(f'Captcha instructions: {challenge_details.get("instructions")}')
+        print(
+            "Developer instructions: The captcha images have an index starting from 0 from left to right",
+        )
+        print("Enter the index of the images that matches the captcha instructions:")
+        index = int(input())
 
-    return index
+        return index
 
 
 def get_arkose_token(
     download_images: bool = True,
     solver: function = captcha_solver,
 ) -> str:
     """
```

### Comparing `revChatGPT-6.7.3/src/revChatGPT/V3.py` & `revChatGPT-6.7.4/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.3/src/revChatGPT/__init__.py` & `revChatGPT-6.7.4/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.3/src/revChatGPT/__main__.py` & `revChatGPT-6.7.4/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.3/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.7.4/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.3/src/revChatGPT/typings.py` & `revChatGPT-6.7.4/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.3/src/revChatGPT/utils.py` & `revChatGPT-6.7.4/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.3/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.7.4/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.7.3
+Version: 6.7.4
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.7.3/tests/test_recipient.py` & `revChatGPT-6.7.4/tests/test_recipient.py`

 * *Files identical despite different names*

