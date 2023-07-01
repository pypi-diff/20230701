# Comparing `tmp/hugchat_api-0.0.1.3.tar.gz` & `tmp/hugchat_api-0.0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugchat_api-0.0.1.3.tar", last modified: Sat Jul  1 04:46:37 2023, max compression
+gzip compressed data, was "hugchat_api-0.0.1.4.tar", last modified: Sat Jul  1 05:02:09 2023, max compression
```

## Comparing `hugchat_api-0.0.1.3.tar` & `hugchat_api-0.0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 04:46:37.433829 hugchat_api-0.0.1.3/
--rw-rw-rw-   0        0        0    35823 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.3/LICENSE
--rw-rw-rw-   0        0        0     6237 2023-07-01 04:46:37.433829 hugchat_api-0.0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     5397 2023-07-01 04:40:39.000000 hugchat_api-0.0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 04:46:37.415839 hugchat_api-0.0.1.3/hugchat_api/
--rw-rw-rw-   0        0        0      296 2023-07-01 04:40:39.000000 hugchat_api-0.0.1.3/hugchat_api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 04:46:37.430829 hugchat_api-0.0.1.3/hugchat_api/core/
--rw-rw-rw-   0        0        0    13732 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.3/hugchat_api/core/Bot.py
--rw-rw-rw-   0        0        0       55 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.3/hugchat_api/core/Exceptions.py
--rw-rw-rw-   0        0        0     1641 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.3/hugchat_api/core/Message.py
--rw-rw-rw-   0        0        0     7178 2023-07-01 04:40:39.000000 hugchat_api-0.0.1.3/hugchat_api/core/Sign.py
--rw-rw-rw-   0        0        0     1278 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.3/hugchat_api/core/ThreadPool.py
--rw-rw-rw-   0        0        0     4247 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.3/hugchat_api/core/WebSearch.py
--rw-rw-rw-   0        0        0      758 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.3/hugchat_api/core/__init__.py
--rw-rw-rw-   0        0        0     6737 2023-07-01 04:40:39.000000 hugchat_api-0.0.1.3/hugchat_api/terminal_cli.py
-drwxrwxrwx   0        0        0        0 2023-07-01 04:46:37.431820 hugchat_api-0.0.1.3/hugchat_api/utils/
--rw-rw-rw-   0        0        0     1726 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.3/hugchat_api/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 04:46:37.421839 hugchat_api-0.0.1.3/hugchat_api.egg-info/
--rw-rw-rw-   0        0        0     6237 2023-07-01 04:46:37.000000 hugchat_api-0.0.1.3/hugchat_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      480 2023-07-01 04:46:37.000000 hugchat_api-0.0.1.3/hugchat_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 04:46:37.000000 hugchat_api-0.0.1.3/hugchat_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-01 04:46:37.000000 hugchat_api-0.0.1.3/hugchat_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-01 04:46:37.000000 hugchat_api-0.0.1.3/hugchat_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 04:46:37.434839 hugchat_api-0.0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1193 2023-07-01 04:40:39.000000 hugchat_api-0.0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 05:02:09.620181 hugchat_api-0.0.1.4/
+-rw-rw-rw-   0        0        0    35823 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     6237 2023-07-01 05:02:09.619180 hugchat_api-0.0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5397 2023-07-01 04:40:39.000000 hugchat_api-0.0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 05:02:09.600170 hugchat_api-0.0.1.4/hugchat_api/
+-rw-rw-rw-   0        0        0      296 2023-07-01 05:01:45.000000 hugchat_api-0.0.1.4/hugchat_api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 05:02:09.616181 hugchat_api-0.0.1.4/hugchat_api/core/
+-rw-rw-rw-   0        0        0    13732 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.4/hugchat_api/core/Bot.py
+-rw-rw-rw-   0        0        0       55 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.4/hugchat_api/core/Exceptions.py
+-rw-rw-rw-   0        0        0     1641 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.4/hugchat_api/core/Message.py
+-rw-rw-rw-   0        0        0     7133 2023-07-01 05:01:45.000000 hugchat_api-0.0.1.4/hugchat_api/core/Sign.py
+-rw-rw-rw-   0        0        0     1278 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.4/hugchat_api/core/ThreadPool.py
+-rw-rw-rw-   0        0        0     4247 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.4/hugchat_api/core/WebSearch.py
+-rw-rw-rw-   0        0        0      758 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.4/hugchat_api/core/__init__.py
+-rw-rw-rw-   0        0        0     6737 2023-07-01 04:40:39.000000 hugchat_api-0.0.1.4/hugchat_api/terminal_cli.py
+drwxrwxrwx   0        0        0        0 2023-07-01 05:02:09.618170 hugchat_api-0.0.1.4/hugchat_api/utils/
+-rw-rw-rw-   0        0        0     1726 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.4/hugchat_api/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 05:02:09.606183 hugchat_api-0.0.1.4/hugchat_api.egg-info/
+-rw-rw-rw-   0        0        0     6237 2023-07-01 05:02:09.000000 hugchat_api-0.0.1.4/hugchat_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      480 2023-07-01 05:02:09.000000 hugchat_api-0.0.1.4/hugchat_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 05:02:09.000000 hugchat_api-0.0.1.4/hugchat_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-01 05:02:09.000000 hugchat_api-0.0.1.4/hugchat_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-01 05:02:09.000000 hugchat_api-0.0.1.4/hugchat_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 05:02:09.620181 hugchat_api-0.0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1193 2023-07-01 04:40:39.000000 hugchat_api-0.0.1.4/setup.py
```

### Comparing `hugchat_api-0.0.1.3/LICENSE` & `hugchat_api-0.0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hugchat_api-0.0.1.3/PKG-INFO` & `hugchat_api-0.0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat_api
-Version: 0.0.1.3
+Version: 0.0.1.4
 Summary: Chat using huggingchat, 'stream' response and 'Search Web' supported.
 Home-page: https://github.com/ogios/huggingchat-api
 Author: ogios
 Author-email: 2134692955@qq.com
 License: GNU General Public License v3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `hugchat_api-0.0.1.3/README.md` & `hugchat_api-0.0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `hugchat_api-0.0.1.3/hugchat_api/core/Bot.py` & `hugchat_api-0.0.1.4/hugchat_api/core/Bot.py`

 * *Files identical despite different names*

### Comparing `hugchat_api-0.0.1.3/hugchat_api/core/Message.py` & `hugchat_api-0.0.1.4/hugchat_api/core/Message.py`

 * *Files identical despite different names*

### Comparing `hugchat_api-0.0.1.3/hugchat_api/core/Sign.py` & `hugchat_api-0.0.1.4/hugchat_api/core/Sign.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import os
-# import re
+import re
 import requests
 
 import requests.utils
 import requests.sessions
 import json
 
 
@@ -90,34 +90,34 @@
     def _grantAuth(self, url: str) -> int:
         res = self._requestsGet(url, allow_redirects=False)
         if res.headers.__contains__("location"):
             location = res.headers["location"]
             res = self._requestsGet(location, allow_redirects=False)
             if res.cookies.__contains__("hf-chat"):
                 return 1
-        raise Exception("grantAuth fatal")
-        # if res.status_code != 200:
-        #     raise Exception("grant auth fatal!")
-        # csrf = re.findall('/oauth/authorize.*?name="csrf" value="(.*?)"', res.text)
-        # if len(csrf) == 0:
-        #     raise Exception("No csrf found!")
-        # data = {
-        #     "csrf": csrf[0]
-        # }
-        #
-        # res = self._requestsPost(url, data=data, allow_redirects=False)
-        # if res.status_code != 303:
-        #     raise Exception(f"get hf-chat cookies fatal! - {res.status_code}")
-        # else:
-        #     location = res.headers.get("Location")
-        # res = self._requestsGet(location, allow_redirects=False)
-        # if res.status_code != 302:
-        #     raise Exception(f"get hf-chat cookie fatal! - {res.status_code}")
-        # else:
-        #     return 1
+        # raise Exception("grantAuth fatal")
+        if res.status_code != 200:
+            raise Exception("grant auth fatal!")
+        csrf = re.findall('/oauth/authorize.*?name="csrf" value="(.*?)"', res.text)
+        if len(csrf) == 0:
+            raise Exception("No csrf found!")
+        data = {
+            "csrf": csrf[0]
+        }
+
+        res = self._requestsPost(url, data=data, allow_redirects=False)
+        if res.status_code != 303:
+            raise Exception(f"get hf-chat cookies fatal! - {res.status_code}")
+        else:
+            location = res.headers.get("Location")
+        res = self._requestsGet(location, allow_redirects=False)
+        if res.status_code != 302:
+            raise Exception(f"get hf-chat cookie fatal! - {res.status_code}")
+        else:
+            return 1
     
     def saveCookiesToDir(self, cookie_dir_path: str = None) -> str:
         cookie_dir_path = self.DEFAULT_PATH_DIR if not cookie_dir_path else cookie_dir_path
         if not cookie_dir_path.endswith("/"):
             cookie_dir_path += "/"
         cookie_path = cookie_dir_path + f"{self.email}.json"
         if not os.path.exists(cookie_dir_path):
```

### Comparing `hugchat_api-0.0.1.3/hugchat_api/core/ThreadPool.py` & `hugchat_api-0.0.1.4/hugchat_api/core/ThreadPool.py`

 * *Files identical despite different names*

### Comparing `hugchat_api-0.0.1.3/hugchat_api/core/WebSearch.py` & `hugchat_api-0.0.1.4/hugchat_api/core/WebSearch.py`

 * *Files identical despite different names*

### Comparing `hugchat_api-0.0.1.3/hugchat_api/core/__init__.py` & `hugchat_api-0.0.1.4/hugchat_api/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hugchat_api-0.0.1.3/hugchat_api/terminal_cli.py` & `hugchat_api-0.0.1.4/hugchat_api/terminal_cli.py`

 * *Files identical despite different names*

### Comparing `hugchat_api-0.0.1.3/hugchat_api/utils/__init__.py` & `hugchat_api-0.0.1.4/hugchat_api/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hugchat_api-0.0.1.3/hugchat_api.egg-info/PKG-INFO` & `hugchat_api-0.0.1.4/hugchat_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat-api
-Version: 0.0.1.3
+Version: 0.0.1.4
 Summary: Chat using huggingchat, 'stream' response and 'Search Web' supported.
 Home-page: https://github.com/ogios/huggingchat-api
 Author: ogios
 Author-email: 2134692955@qq.com
 License: GNU General Public License v3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `hugchat_api-0.0.1.3/setup.py` & `hugchat_api-0.0.1.4/setup.py`

 * *Files identical despite different names*

