# Comparing `tmp/hugchat_api-0.0.1.2.tar.gz` & `tmp/hugchat_api-0.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugchat_api-0.0.1.2.tar", last modified: Thu Jun 22 16:48:40 2023, max compression
+gzip compressed data, was "hugchat_api-0.0.1.3.tar", last modified: Sat Jul  1 04:46:37 2023, max compression
```

## Comparing `hugchat_api-0.0.1.2.tar` & `hugchat_api-0.0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 16:48:40.171840 hugchat_api-0.0.1.2/
--rw-rw-rw-   0        0        0    35823 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.2/LICENSE
--rw-rw-rw-   0        0        0     6097 2023-06-22 16:48:40.170840 hugchat_api-0.0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5229 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 16:48:40.151840 hugchat_api-0.0.1.2/hugchat_api/
--rw-rw-rw-   0        0        0      283 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.2/hugchat_api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:48:40.168841 hugchat_api-0.0.1.2/hugchat_api/core/
--rw-rw-rw-   0        0        0    13732 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.2/hugchat_api/core/Bot.py
--rw-rw-rw-   0        0        0       55 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.2/hugchat_api/core/Exceptions.py
--rw-rw-rw-   0        0        0     1641 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.2/hugchat_api/core/Message.py
--rw-rw-rw-   0        0        0     6507 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.2/hugchat_api/core/Sign.py
--rw-rw-rw-   0        0        0     1278 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.2/hugchat_api/core/ThreadPool.py
--rw-rw-rw-   0        0        0     4247 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.2/hugchat_api/core/WebSearch.py
--rw-rw-rw-   0        0        0      758 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.2/hugchat_api/core/__init__.py
--rw-rw-rw-   0        0        0     6829 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.2/hugchat_api/terminal_cli.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:48:40.169840 hugchat_api-0.0.1.2/hugchat_api/utils/
--rw-rw-rw-   0        0        0     1726 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.2/hugchat_api/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:48:40.157840 hugchat_api-0.0.1.2/hugchat_api.egg-info/
--rw-rw-rw-   0        0        0     6097 2023-06-22 16:48:39.000000 hugchat_api-0.0.1.2/hugchat_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      480 2023-06-22 16:48:40.000000 hugchat_api-0.0.1.2/hugchat_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 16:48:39.000000 hugchat_api-0.0.1.2/hugchat_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-22 16:48:39.000000 hugchat_api-0.0.1.2/hugchat_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-22 16:48:39.000000 hugchat_api-0.0.1.2/hugchat_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 16:48:40.171840 hugchat_api-0.0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1227 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 04:46:37.433829 hugchat_api-0.0.1.3/
+-rw-rw-rw-   0        0        0    35823 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     6237 2023-07-01 04:46:37.433829 hugchat_api-0.0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5397 2023-07-01 04:40:39.000000 hugchat_api-0.0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 04:46:37.415839 hugchat_api-0.0.1.3/hugchat_api/
+-rw-rw-rw-   0        0        0      296 2023-07-01 04:40:39.000000 hugchat_api-0.0.1.3/hugchat_api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 04:46:37.430829 hugchat_api-0.0.1.3/hugchat_api/core/
+-rw-rw-rw-   0        0        0    13732 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.3/hugchat_api/core/Bot.py
+-rw-rw-rw-   0        0        0       55 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.3/hugchat_api/core/Exceptions.py
+-rw-rw-rw-   0        0        0     1641 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.3/hugchat_api/core/Message.py
+-rw-rw-rw-   0        0        0     7178 2023-07-01 04:40:39.000000 hugchat_api-0.0.1.3/hugchat_api/core/Sign.py
+-rw-rw-rw-   0        0        0     1278 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.3/hugchat_api/core/ThreadPool.py
+-rw-rw-rw-   0        0        0     4247 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.3/hugchat_api/core/WebSearch.py
+-rw-rw-rw-   0        0        0      758 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.3/hugchat_api/core/__init__.py
+-rw-rw-rw-   0        0        0     6737 2023-07-01 04:40:39.000000 hugchat_api-0.0.1.3/hugchat_api/terminal_cli.py
+drwxrwxrwx   0        0        0        0 2023-07-01 04:46:37.431820 hugchat_api-0.0.1.3/hugchat_api/utils/
+-rw-rw-rw-   0        0        0     1726 2023-06-22 16:47:49.000000 hugchat_api-0.0.1.3/hugchat_api/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 04:46:37.421839 hugchat_api-0.0.1.3/hugchat_api.egg-info/
+-rw-rw-rw-   0        0        0     6237 2023-07-01 04:46:37.000000 hugchat_api-0.0.1.3/hugchat_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      480 2023-07-01 04:46:37.000000 hugchat_api-0.0.1.3/hugchat_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 04:46:37.000000 hugchat_api-0.0.1.3/hugchat_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-01 04:46:37.000000 hugchat_api-0.0.1.3/hugchat_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-01 04:46:37.000000 hugchat_api-0.0.1.3/hugchat_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 04:46:37.434839 hugchat_api-0.0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1193 2023-07-01 04:40:39.000000 hugchat_api-0.0.1.3/setup.py
```

### Comparing `hugchat_api-0.0.1.2/LICENSE` & `hugchat_api-0.0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hugchat_api-0.0.1.2/PKG-INFO` & `hugchat_api-0.0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hugchat_api
-Version: 0.0.1.2
-Summary: Hugging chat web api, use for chat with an Open-Assistant language model, 'Search Web' supported.
+Version: 0.0.1.3
+Summary: Chat using huggingchat, 'stream' response and 'Search Web' supported.
 Home-page: https://github.com/ogios/huggingchat-api
 Author: ogios
 Author-email: 2134692955@qq.com
 License: GNU General Public License v3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: curl
 License-File: LICENSE
 
 # Huggingchat api
 
-**Leave a star and you could win a billion(**
+**You Star You Win A BILLION$$$(maybe,it's not impossible that it would happen)**
 
 > This is my first pypi project. Experienced some annoying moments, but i managed to do it anyway
 
 [![PyPI version](https://img.shields.io/pypi/v/hugchat-api.svg)](https://pypi.python.org/pypi/hugchat-api/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/hugchat-api.svg)](https://pypi.python.org/pypi/hugchat-api/)
 
 [![Downloads](https://static.pepy.tech/badge/hugchat-api)](https://pepy.tech/project/hugchat-api)
@@ -214,7 +214,11 @@
 #WEB_SEARCH is set to `True`
 (647e09ccabd9de3d82d6fba0) > hi
 # ...(steps about web search)
 #(Open-Assistant): ...
 ```
 
 </details>
+
+## Download status
+seperated in regions(country_code). powered by bigquery and mermaid.
+![test](http://47.94.146.109:8000/.md)
```

### Comparing `hugchat_api-0.0.1.2/README.md` & `hugchat_api-0.0.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Huggingchat api
 
-**Leave a star and you could win a billion(**
+**You Star You Win A BILLION$$$(maybe,it's not impossible that it would happen)**
 
 > This is my first pypi project. Experienced some annoying moments, but i managed to do it anyway
 
 [![PyPI version](https://img.shields.io/pypi/v/hugchat-api.svg)](https://pypi.python.org/pypi/hugchat-api/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/hugchat-api.svg)](https://pypi.python.org/pypi/hugchat-api/)
 
 [![Downloads](https://static.pepy.tech/badge/hugchat-api)](https://pepy.tech/project/hugchat-api)
@@ -193,7 +193,11 @@
 #WEB_SEARCH is set to `True`
 (647e09ccabd9de3d82d6fba0) > hi
 # ...(steps about web search)
 #(Open-Assistant): ...
 ```
 
 </details>
+
+## Download status
+seperated in regions(country_code). powered by bigquery and mermaid.
+![test](http://47.94.146.109:8000/.md)
```

### Comparing `hugchat_api-0.0.1.2/hugchat_api/core/Bot.py` & `hugchat_api-0.0.1.3/hugchat_api/core/Bot.py`

 * *Files identical despite different names*

### Comparing `hugchat_api-0.0.1.2/hugchat_api/core/Message.py` & `hugchat_api-0.0.1.3/hugchat_api/core/Message.py`

 * *Files identical despite different names*

### Comparing `hugchat_api-0.0.1.2/hugchat_api/core/Sign.py` & `hugchat_api-0.0.1.3/hugchat_api/core/Sign.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import os
-import re
+# import re
 import requests
 
 import requests.utils
 import requests.sessions
 import json
 
 
@@ -15,14 +15,16 @@
         self.headers = {
             "Referer": "https://huggingface.co/",
             # "Content-Type": "application/json",
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36 Edg/112.0.1722.64",
         }
         self.cookies = requests.sessions.RequestsCookieJar()
         
+        self.DEFAULT_PATH_DIR = os.path.dirname(os.path.abspath(__file__)) + "/usercookies"
+        self.DEFAULT_COOKIE_PATH = self.DEFAULT_PATH_DIR + f"/{email}.json"
         # self.COOKIE_DIR = os.path.dirname(os.path.abspath(__file__)) + "/usercookies"
         # self.COOKIE_PATH = self.COOKIE_DIR + f"/{self.email}.json"
         # if not os.path.exists(self.COOKIE_DIR):
         #     logging.info("Cookie directory not found, creating...")
         #     os.makedirs(self.COOKIE_DIR)
         # logging.info(f"Cookie store path: {self.COOKIE_PATH}")
     
@@ -82,36 +84,43 @@
                 return location
             else:
                 raise Exception("No authorize url!")
         else:
             raise Exception("Something went wrong!")
     
     def _grantAuth(self, url: str) -> int:
-        res = self._requestsGet(url)
-        if res.status_code != 200:
-            raise Exception("grant auth fatal!")
-        csrf = re.findall('/oauth/authorize.*?name="csrf" value="(.*?)"', res.text)
-        if len(csrf) == 0:
-            raise Exception("No csrf found!")
-        data = {
-            "csrf": csrf[0]
-        }
-        
-        res = self._requestsPost(url, data=data, allow_redirects=False)
-        if res.status_code != 303:
-            raise Exception(f"get hf-chat cookies fatal! - {res.status_code}")
-        else:
-            location = res.headers.get("Location")
-        res = self._requestsGet(location, allow_redirects=False)
-        if res.status_code != 302:
-            raise Exception(f"get hf-chat cookie fatal! - {res.status_code}")
-        else:
-            return 1
+        res = self._requestsGet(url, allow_redirects=False)
+        if res.headers.__contains__("location"):
+            location = res.headers["location"]
+            res = self._requestsGet(location, allow_redirects=False)
+            if res.cookies.__contains__("hf-chat"):
+                return 1
+        raise Exception("grantAuth fatal")
+        # if res.status_code != 200:
+        #     raise Exception("grant auth fatal!")
+        # csrf = re.findall('/oauth/authorize.*?name="csrf" value="(.*?)"', res.text)
+        # if len(csrf) == 0:
+        #     raise Exception("No csrf found!")
+        # data = {
+        #     "csrf": csrf[0]
+        # }
+        #
+        # res = self._requestsPost(url, data=data, allow_redirects=False)
+        # if res.status_code != 303:
+        #     raise Exception(f"get hf-chat cookies fatal! - {res.status_code}")
+        # else:
+        #     location = res.headers.get("Location")
+        # res = self._requestsGet(location, allow_redirects=False)
+        # if res.status_code != 302:
+        #     raise Exception(f"get hf-chat cookie fatal! - {res.status_code}")
+        # else:
+        #     return 1
     
-    def saveCookiesToDir(self, cookie_dir_path: str) -> str:
+    def saveCookiesToDir(self, cookie_dir_path: str = None) -> str:
+        cookie_dir_path = self.DEFAULT_PATH_DIR if not cookie_dir_path else cookie_dir_path
         if not cookie_dir_path.endswith("/"):
             cookie_dir_path += "/"
         cookie_path = cookie_dir_path + f"{self.email}.json"
         if not os.path.exists(cookie_dir_path):
             logging.info("Cookie directory not exist, creating...")
             os.makedirs(cookie_dir_path)
         logging.info(f"Cookie store path: {cookie_path}")
@@ -127,15 +136,16 @@
             return ""
         files = os.listdir(cookie_dir_path)
         for i in files:
             if i == f"{self.email}.json":
                 return cookie_dir_path + i
         return ""
     
-    def loadCookiesFromDir(self, cookie_dir_path: str) -> requests.sessions.RequestsCookieJar:
+    def loadCookiesFromDir(self, cookie_dir_path: str = None) -> requests.sessions.RequestsCookieJar:
+        cookie_dir_path = self.DEFAULT_PATH_DIR if not cookie_dir_path else cookie_dir_path
         cookie_path = self._getCookiePath(cookie_dir_path)
         if not cookie_path:
             raise Exception(f"Cookie not found. please check the path given: {cookie_dir_path}.\n" +
                             f"Cookie file must be named like this: 'your_email'+'.json': '{self.email}.json'")
         
         with open(cookie_path, "r", encoding="utf-8") as f:
             try:
@@ -143,25 +153,24 @@
                 for i in js.keys():
                     self.cookies.set(i, js[i])
                     logging.info(f"{i} loaded")
                 return self.cookies
             except:
                 raise Exception("load cookies from files fatal. Please check the format")
     
-    def login(self, save: bool = False, cookie_dir_path: str = "") -> requests.sessions.RequestsCookieJar:
+    def login(self, save: bool = False, cookie_dir_path: str = None) -> requests.sessions.RequestsCookieJar:
         self._SigninWithEmail()
         location = self._getAuthURL()
         if self._grantAuth(location):
             pass
         if save:
-            if not cookie_dir_path:
-                raise Exception("Please specify where to store your cookies")
             self.saveCookiesToDir(cookie_dir_path)
         return self.cookies
 
 
 if __name__ == "__main__":
-    email = ""
-    passwd = ""
+    email = os.getenv("EMAIL")
+    passwd = os.getenv("PASSWD")
     sign = Sign(email, passwd)
     cookies = sign.login()
+    sign.saveCookiesToDir()
     print(cookies)
```

### Comparing `hugchat_api-0.0.1.2/hugchat_api/core/ThreadPool.py` & `hugchat_api-0.0.1.3/hugchat_api/core/ThreadPool.py`

 * *Files identical despite different names*

### Comparing `hugchat_api-0.0.1.2/hugchat_api/core/WebSearch.py` & `hugchat_api-0.0.1.3/hugchat_api/core/WebSearch.py`

 * *Files identical despite different names*

### Comparing `hugchat_api-0.0.1.2/hugchat_api/core/__init__.py` & `hugchat_api-0.0.1.3/hugchat_api/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hugchat_api-0.0.1.2/hugchat_api/terminal_cli.py` & `hugchat_api-0.0.1.3/hugchat_api/terminal_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,48 @@
 
 from .core import HuggingChat
 from .core.Message import Message
 from .core.Sign import Sign
 from .core.Bot import Bot
 from .utils import color, formatHistory, formatConversations, getTextFromInput, getIdByIndex
 
-COOKIE_DIR_PATH = os.path.abspath(os.path.dirname(__file__)) + "/usercookies"
+# COOKIE_DIR_PATH = os.path.abspath(os.path.dirname(__file__)) + "/usercookies"
 # CONSOLE = Console()
 hug = HuggingChat()
 
 # FLAG = False
 WEB_SEARCH = False
 NEW_CONVERSATION = False
 
 logging.getLogger().setLevel(logging.INFO)
 
 def checkCookies(u):
     login = Sign(u, None)
     try:
-        login.loadCookiesFromDir(COOKIE_DIR_PATH)
+        login.loadCookiesFromDir()
         return True
     except Exception as e:
         # print(e)
         return False
 
 
 def login(u, p=None, force=False):
     if not p:
         logging.info(f"No Password input, trying to load it from mysql or files")
         login = Sign(u, p)
-        cookies = login.loadCookiesFromDir(COOKIE_DIR_PATH)
+        cookies = login.loadCookiesFromDir()
     else:
         login = Sign(u, p)
         if force:
-            cookies = login.login(save=True, cookie_dir_path=COOKIE_DIR_PATH)
+            cookies = login.login(save=True)
         else:
             try:
-                cookies = login.loadCookiesFromDir(COOKIE_DIR_PATH)
+                cookies = login.loadCookiesFromDir()
             except:
-                cookies = login.login(save=True, cookie_dir_path=COOKIE_DIR_PATH)
+                cookies = login.login(save=True)
     return cookies
 
 
 def updateMSG(message: Message):
     # global FLAG
     while not message.done:
         if message.error:
@@ -196,9 +196,9 @@
                 # FLAG = True
         except Exception as e:
             traceback.print_exc()
 
 
 if __name__ == "__main__":
     EMAIL = os.getenv("EMAIL")
-    PASSWD = ""
+    PASSWD = os.getenv("PASSWD")
     main(EMAIL, PASSWD)
```

### Comparing `hugchat_api-0.0.1.2/hugchat_api/utils/__init__.py` & `hugchat_api-0.0.1.3/hugchat_api/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hugchat_api-0.0.1.2/hugchat_api.egg-info/PKG-INFO` & `hugchat_api-0.0.1.3/hugchat_api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hugchat-api
-Version: 0.0.1.2
-Summary: Hugging chat web api, use for chat with an Open-Assistant language model, 'Search Web' supported.
+Version: 0.0.1.3
+Summary: Chat using huggingchat, 'stream' response and 'Search Web' supported.
 Home-page: https://github.com/ogios/huggingchat-api
 Author: ogios
 Author-email: 2134692955@qq.com
 License: GNU General Public License v3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: curl
 License-File: LICENSE
 
 # Huggingchat api
 
-**Leave a star and you could win a billion(**
+**You Star You Win A BILLION$$$(maybe,it's not impossible that it would happen)**
 
 > This is my first pypi project. Experienced some annoying moments, but i managed to do it anyway
 
 [![PyPI version](https://img.shields.io/pypi/v/hugchat-api.svg)](https://pypi.python.org/pypi/hugchat-api/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/hugchat-api.svg)](https://pypi.python.org/pypi/hugchat-api/)
 
 [![Downloads](https://static.pepy.tech/badge/hugchat-api)](https://pepy.tech/project/hugchat-api)
@@ -214,7 +214,11 @@
 #WEB_SEARCH is set to `True`
 (647e09ccabd9de3d82d6fba0) > hi
 # ...(steps about web search)
 #(Open-Assistant): ...
 ```
 
 </details>
+
+## Download status
+seperated in regions(country_code). powered by bigquery and mermaid.
+![test](http://47.94.146.109:8000/.md)
```

### Comparing `hugchat_api-0.0.1.2/setup.py` & `hugchat_api-0.0.1.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from setuptools import find_packages
 from distutils.core import setup
+
+from hugchat_api import __version__, __description__, __email__, __url__, __author__
+
 setup(
     name="hugchat_api",
-    version="0.0.1.2",
-    author="ogios",
-    author_email="2134692955@qq.com",
-    description="Hugging chat web api, use for chat with an Open-Assistant language model, 'Search Web' supported.",
-    url="https://github.com/ogios/huggingchat-api",
+    version=__version__,
+    author=__author__,
+    author_email=__email__,
+    description=__description__,
+    url=__url__,
     packages=find_packages(),
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
```

