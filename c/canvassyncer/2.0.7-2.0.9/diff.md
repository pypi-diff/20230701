# Comparing `tmp/canvassyncer-2.0.7.tar.gz` & `tmp/canvassyncer-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canvassyncer-2.0.7.tar", last modified: Wed Aug 31 08:50:17 2022, max compression
+gzip compressed data, was "canvassyncer-2.0.9.tar", last modified: Wed Aug 31 16:46:38 2022, max compression
```

## Comparing `canvassyncer-2.0.7.tar` & `canvassyncer-2.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 08:50:17.804166 canvassyncer-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-08-31 08:50:08.000000 canvassyncer-2.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2867 2022-08-31 08:50:17.804166 canvassyncer-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2365 2022-08-31 08:50:08.000000 canvassyncer-2.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 08:50:17.804166 canvassyncer-2.0.7/canvassyncer/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-08-31 08:50:08.000000 canvassyncer-2.0.7/canvassyncer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17821 2022-08-31 08:50:08.000000 canvassyncer-2.0.7/canvassyncer/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 08:50:17.804166 canvassyncer-2.0.7/canvassyncer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2867 2022-08-31 08:50:17.000000 canvassyncer-2.0.7/canvassyncer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-08-31 08:50:17.000000 canvassyncer-2.0.7/canvassyncer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-31 08:50:17.000000 canvassyncer-2.0.7/canvassyncer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-08-31 08:50:17.000000 canvassyncer-2.0.7/canvassyncer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-08-31 08:50:17.000000 canvassyncer-2.0.7/canvassyncer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-08-31 08:50:17.000000 canvassyncer-2.0.7/canvassyncer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-31 08:50:17.804166 canvassyncer-2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-08-31 08:50:08.000000 canvassyncer-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 16:46:38.710918 canvassyncer-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-08-31 16:46:29.000000 canvassyncer-2.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2867 2022-08-31 16:46:38.710918 canvassyncer-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2365 2022-08-31 16:46:29.000000 canvassyncer-2.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 16:46:38.706918 canvassyncer-2.0.9/canvassyncer/
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-08-31 16:46:29.000000 canvassyncer-2.0.9/canvassyncer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17615 2022-08-31 16:46:29.000000 canvassyncer-2.0.9/canvassyncer/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 16:46:38.710918 canvassyncer-2.0.9/canvassyncer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2867 2022-08-31 16:46:38.000000 canvassyncer-2.0.9/canvassyncer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2022-08-31 16:46:38.000000 canvassyncer-2.0.9/canvassyncer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-31 16:46:38.000000 canvassyncer-2.0.9/canvassyncer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2022-08-31 16:46:38.000000 canvassyncer-2.0.9/canvassyncer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-08-31 16:46:38.000000 canvassyncer-2.0.9/canvassyncer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-08-31 16:46:38.000000 canvassyncer-2.0.9/canvassyncer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-31 16:46:38.710918 canvassyncer-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-08-31 16:46:29.000000 canvassyncer-2.0.9/setup.py
```

### Comparing `canvassyncer-2.0.7/LICENSE` & `canvassyncer-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `canvassyncer-2.0.7/PKG-INFO` & `canvassyncer-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canvassyncer
-Version: 2.0.7
+Version: 2.0.9
 Summary: The async fast canavs file syncer.
 Home-page: https://github.com/BoYanZh/Canvas-Syncer
 Author: SJTU JI Tech
 Author-email: bomingzh@sjtu.edu.cn
 Maintainer: BoYanZh
 Maintainer-email: bomingzh@sjtu.edu.cn
 License: MIT
```

### Comparing `canvassyncer-2.0.7/README.md` & `canvassyncer-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `canvassyncer-2.0.7/canvassyncer/__main__.py` & `canvassyncer-2.0.9/canvassyncer/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import platform
 from datetime import datetime, timezone
 
 import aiofiles
 import httpx
 from tqdm import tqdm
 
-__version__ = "2.0.7"
+__version__ = "2.0.9"
 CONFIG_PATH = os.path.join(
     os.path.dirname(os.path.abspath(__file__)), ".canvassyncer.json"
 )
 PAGES_PER_TIME = 8
 
 
 class AsyncSemClient:
@@ -53,22 +53,19 @@
         self.tqdm.close()
         if self.failures:
             print(f"Fail to download these {len(self.failures)} file(s):")
             for text in self.failures:
                 print(text)
 
     async def json(self, *args, **kwargs):
+        checkError = bool(kwargs.pop("checkError", False))
         async with self.sem:
             resp = await self.client.get(*args, **kwargs)
         res = resp.json()
-        if (
-            kwargs.get("checkError") == True
-            and isinstance(res, dict)
-            and res.get("errors")
-        ):
+        if checkError and isinstance(res, dict) and res.get("errors"):
             errMsg = res["errors"][0].get("message", "unknown error.")
             print(f"\nError: {errMsg}")
             exit(1)
         return res
 
     async def head(self, *args, **kwargs):
         async with self.sem:
@@ -327,72 +324,64 @@
 
 def initConfig():
     oldConfig = {}
     if os.path.exists(CONFIG_PATH):
         oldConfig = json.load(open(CONFIG_PATH))
     elif os.path.exists("./canvassyncer.json"):
         oldConfig = json.load(open("./canvassyncer.json"))
+
+    def promptConfigStr(promptStr, key, *, defaultValOnMissing=None):
+        defaultVal = oldConfig.get(key)
+        if defaultVal is None:
+            if defaultValOnMissing is not None:
+                defaultVal = defaultValOnMissing
+            else:
+                defaultVal = ""
+        elif isinstance(defaultVal, list):
+            defaultVal = " ".join((str(val) for val in defaultVal))
+        defaultVal = str(defaultVal)
+        tipStr = f"(Default: {defaultVal})" if defaultVal else ""
+        res = input(f"{promptStr}{tipStr}: ").strip()
+        if not res:
+            res = defaultVal
+        return res
+
     print("Generating new config file...")
-    prevu = oldConfig.get("canvasURL", "") if oldConfig else "https://umjicanvas.com"
-    url = input("Canvas url(Defuault: " + prevu + "):").strip()
-    if not url:
-        url = prevu
-    tipStr = f"(Default: {oldConfig.get('token', '')})" if oldConfig else ""
-    token = input(f"Canvas access token{tipStr}:").strip()
-    if not token:
-        token = oldConfig.get("token", "")
-    tipStr = (
-        f"(Default: {' '.join(oldConfig.get('courseCodes', []))})" if oldConfig else ""
-    )
-    courseCodes = (
-        input(f"Courses to sync in course codes(split with space){tipStr}:")
-        .strip()
-        .split()
+    url = promptConfigStr(
+        "Canvas url", "canvasURL", defaultValOnMissing="https://umjicanvas.com"
     )
-    if not courseCodes:
-        courseCodes = oldConfig.get("courseCodes", [])
-    tipStr = (
-        f"(Default: {' '.join([str(item) for item in oldConfig.get('courseIDs', [])])})"
-        if oldConfig
-        else ""
+    token = promptConfigStr("Canvas access token", "token")
+    courseCodesStr = promptConfigStr(
+        "Courses to sync in course codes(split with space)", "courseCodes"
+    )
+    courseCodes = courseCodesStr.split()
+    courseIDsStr = promptConfigStr(
+        "Courses to sync in course ID(split with space)", "courseIDs"
+    )
+    courseIDs = [int(courseID) for courseID in courseIDsStr.split()]
+    downloadDir = promptConfigStr(
+        "Path to save canvas files",
+        "downloadDir",
+        defaultValOnMissing=os.path.abspath(""),
     )
-    courseIDs = (
-        input(f"Courses to sync in course ID(split with space){tipStr}:")
-        .strip()
-        .split()
+    filesizeThreshStr = promptConfigStr(
+        "Maximum file size to download(MB)", "filesizeThresh", defaultValOnMissing=250
     )
-    if not courseIDs:
-        courseIDs = oldConfig.get("courseIDs", [])
-    courseIDs = [int(courseID) for courseID in courseIDs]
-    tipStr = f"(Default: {oldConfig.get('downloadDir', os.path.abspath(''))})"
-    downloadDir = input(f"Path to save canvas files{tipStr}:").strip()
-    if not downloadDir:
-        downloadDir = oldConfig.get("downloadDir", os.path.abspath(""))
-    tipStr = (
-        f"(Default: {oldConfig.get('filesizeThresh', '')})"
-        if oldConfig
-        else f"(Default: 250)"
-    )
-    filesizeThresh = input(f"Maximum file size to download(MB){tipStr}:").strip()
     try:
-        filesizeThresh = float(filesizeThresh)
+        filesizeThresh = float(filesizeThreshStr)
     except Exception:
         filesizeThresh = 250
-    json.dump(
-        {
-            "canvasURL": url,
-            "token": token,
-            "courseCodes": courseCodes,
-            "courseIDs": courseIDs,
-            "downloadDir": downloadDir,
-            "filesizeThresh": filesizeThresh,
-        },
-        open(CONFIG_PATH, mode="w", encoding="utf-8"),
-        indent=4,
-    )
+    return {
+        "canvasURL": url,
+        "token": token,
+        "courseCodes": courseCodes,
+        "courseIDs": courseIDs,
+        "downloadDir": downloadDir,
+        "filesizeThresh": filesizeThresh,
+    }
 
 
 def getConfig():
     parser = argparse.ArgumentParser(description="A Simple Canvas File Syncer")
     parser.add_argument("-r", help="recreate config file", action="store_true")
     parser.add_argument("-y", help="confirm all prompts", action="store_true")
     parser.add_argument(
@@ -422,23 +411,25 @@
     )
     args = parser.parse_args()
     configPath = args.path
     if args.r or not os.path.exists(configPath):
         if not os.path.exists(configPath):
             print("Config file not exist, creating...")
         try:
-            initConfig()
+            json.dump(
+                initConfig(),
+                open(configPath, mode="w", encoding="utf-8"),
+                indent=4,
+            )
         except Exception as e:
             print(f"\nError: {e.__class__.__name__}. Failed to create config file.")
             if args.debug:
                 print(traceback.format_exc())
             exit(1)
-        if args.r:
-            return
-    config = json.load(open(configPath, "r", encoding="UTF-8"))
+    config = json.load(open(configPath, mode="r", encoding="utf-8"))
     config["y"] = args.y
     config["proxies"] = args.proxy
     config["no_subfolder"] = args.no_subfolder
     config["connection_count"] = args.connection
     config["no_keep_older_version"] = args.no_keep_older_version
     config["debug"] = args.debug
     return config
@@ -462,18 +453,17 @@
                     f"to {config['connection_count']} and retrying..."
                 )
     except KeyboardInterrupt as e:
         raise e
     except Exception as e:
         errorName = e.__class__.__name__
         print(
-            f"Unexpected error: {errorName}. Please check your network and token!",
-            end="",
+            f"Unexpected error: {errorName}. Please check your network and token!"
+            + ("" if config["debug"] else " Or use -d for detailed information.")
         )
-        print("" if config["debug"] else " Or use -d for detailed information.")
         if config["debug"]:
             print(traceback.format_exc())
     finally:
         if syncer:
             await syncer.aclose()
```

### Comparing `canvassyncer-2.0.7/canvassyncer.egg-info/PKG-INFO` & `canvassyncer-2.0.9/canvassyncer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canvassyncer
-Version: 2.0.7
+Version: 2.0.9
 Summary: The async fast canavs file syncer.
 Home-page: https://github.com/BoYanZh/Canvas-Syncer
 Author: SJTU JI Tech
 Author-email: bomingzh@sjtu.edu.cn
 Maintainer: BoYanZh
 Maintainer-email: bomingzh@sjtu.edu.cn
 License: MIT
```

### Comparing `canvassyncer-2.0.7/setup.py` & `canvassyncer-2.0.9/setup.py`

 * *Files identical despite different names*

