# Comparing `tmp/ss13_tools-2.3.2.tar.gz` & `tmp/ss13_tools-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ss13_tools-2.3.2.tar", max compression
+gzip compressed data, was "ss13_tools-2.3.3.tar", max compression
```

## Comparing `ss13_tools-2.3.2.tar` & `ss13_tools-2.3.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     2301 2023-06-27 22:02:31.214661 ss13_tools-2.3.2/README.md
--rw-r--r--   0        0        0     1008 2023-06-27 22:02:31.226661 ss13_tools-2.3.2/pyproject.toml
--rw-r--r--   0        0        0      325 2023-06-27 22:02:31.226661 ss13_tools-2.3.2/ss13_tools/__init__.py
--rw-r--r--   0        0        0     1175 2023-06-27 22:02:31.226661 ss13_tools-2.3.2/ss13_tools/__main__.py
--rw-r--r--   0        0        0       22 2023-06-27 22:02:31.226661 ss13_tools-2.3.2/ss13_tools/__version__.py
--rw-r--r--   0        0        0      438 2023-06-27 22:02:31.226661 ss13_tools-2.3.2/ss13_tools/auth/__init__.py
--rw-r--r--   0        0        0      205 2023-06-27 22:02:31.226661 ss13_tools-2.3.2/ss13_tools/auth/__main__.py
--rw-r--r--   0        0        0      346 2023-06-27 22:02:31.226661 ss13_tools-2.3.2/ss13_tools/auth/constants.py
--rw-r--r--   0        0        0    10698 2023-06-27 22:02:31.226661 ss13_tools-2.3.2/ss13_tools/auth/tg.py
--rw-r--r--   0        0        0      182 2023-06-27 22:02:31.226661 ss13_tools-2.3.2/ss13_tools/byond/__init__.py
--rw-r--r--   0        0        0      543 2023-06-27 22:02:31.226661 ss13_tools-2.3.2/ss13_tools/byond/__main__.py
--rw-r--r--   0        0        0       59 2023-06-27 22:02:31.226661 ss13_tools-2.3.2/ss13_tools/byond/constants.py
--rw-r--r--   0        0        0     2424 2023-06-27 22:02:31.226661 ss13_tools-2.3.2/ss13_tools/byond/key_tools.py
--rw-r--r--   0        0        0      162 2023-06-27 22:02:31.226661 ss13_tools-2.3.2/ss13_tools/centcom/__init__.py
--rw-r--r--   0        0        0     1099 2023-06-27 22:02:31.226661 ss13_tools-2.3.2/ss13_tools/centcom/__main__.py
--rw-r--r--   0        0        0      394 2023-06-27 22:02:31.226661 ss13_tools-2.3.2/ss13_tools/centcom/ban.py
--rw-r--r--   0        0        0     1492 2023-06-27 22:02:31.226661 ss13_tools-2.3.2/ss13_tools/centcom/ban_types.py
--rw-r--r--   0        0        0       68 2023-06-27 22:02:31.226661 ss13_tools-2.3.2/ss13_tools/centcom/constants.py
--rw-r--r--   0        0        0      614 2023-06-27 22:02:31.226661 ss13_tools-2.3.2/ss13_tools/cli.py
--rw-r--r--   0        0        0      222 2023-06-27 22:02:31.226661 ss13_tools-2.3.2/ss13_tools/constants.py
--rw-r--r--   0        0        0    18265 2023-06-27 22:02:31.226661 ss13_tools-2.3.2/ss13_tools/log_buddy/README.md
--rw-r--r--   0        0        0      198 2023-06-27 22:02:31.226661 ss13_tools-2.3.2/ss13_tools/log_buddy/__init__.py
--rw-r--r--   0        0        0     5561 2023-06-27 22:02:31.226661 ss13_tools-2.3.2/ss13_tools/log_buddy/__main__.py
--rw-r--r--   0        0        0      768 2023-06-27 22:02:31.226661 ss13_tools-2.3.2/ss13_tools/log_buddy/constants.py
--rw-r--r--   0        0        0      562 2023-06-27 22:02:31.230661 ss13_tools-2.3.2/ss13_tools/log_buddy/expressions.py
--rw-r--r--   0        0        0    52497 2023-06-27 22:02:31.230661 ss13_tools-2.3.2/ss13_tools/log_buddy/log.py
--rw-r--r--   0        0        0    17063 2023-06-27 22:02:31.230661 ss13_tools-2.3.2/ss13_tools/log_buddy/log_magics.py
--rw-r--r--   0        0        0    28437 2023-06-27 22:02:31.230661 ss13_tools-2.3.2/ss13_tools/log_buddy/log_parser.py
--rw-r--r--   0        0        0      554 2023-06-27 22:02:31.230661 ss13_tools-2.3.2/ss13_tools/log_downloader/__init__.py
--rw-r--r--   0        0        0     2011 2023-06-27 22:02:31.230661 ss13_tools-2.3.2/ss13_tools/log_downloader/__main__.py
--rw-r--r--   0        0        0     7393 2023-06-27 22:02:31.230661 ss13_tools-2.3.2/ss13_tools/log_downloader/base.py
--rw-r--r--   0        0        0     4756 2023-06-27 22:02:31.230661 ss13_tools-2.3.2/ss13_tools/log_downloader/ckey.py
--rw-r--r--   0        0        0      517 2023-06-27 22:02:31.230661 ss13_tools-2.3.2/ss13_tools/log_downloader/constants.py
--rw-r--r--   0        0        0     4492 2023-06-27 22:02:31.230661 ss13_tools-2.3.2/ss13_tools/log_downloader/round.py
--rw-r--r--   0        0        0    10429 2023-06-27 22:02:31.230661 ss13_tools-2.3.2/ss13_tools/menu.py
--rw-r--r--   0        0        0     1247 2023-06-27 22:02:31.230661 ss13_tools-2.3.2/ss13_tools/menu_item.py
--rw-r--r--   0        0        0     1880 2023-06-27 22:02:31.230661 ss13_tools-2.3.2/ss13_tools/scrubby/CKeyController.py
--rw-r--r--   0        0        0     2341 2023-06-27 22:02:31.230661 ss13_tools-2.3.2/ss13_tools/scrubby/RoundController.py
--rw-r--r--   0        0        0      622 2023-06-27 22:02:31.230661 ss13_tools-2.3.2/ss13_tools/scrubby/__init__.py
--rw-r--r--   0        0        0      107 2023-06-27 22:02:31.230661 ss13_tools-2.3.2/ss13_tools/scrubby/__main__.py
--rw-r--r--   0        0        0      433 2023-06-27 22:02:31.230661 ss13_tools-2.3.2/ss13_tools/scrubby/constants.py
--rw-r--r--   0        0        0        0 2023-06-27 22:02:31.230661 ss13_tools-2.3.2/ss13_tools/scrubby/investigate.py
--rw-r--r--   0        0        0     1201 2023-06-27 22:02:31.230661 ss13_tools-2.3.2/ss13_tools/scrubby/round_data.py
--rw-r--r--   0        0        0      154 2023-06-27 22:02:31.230661 ss13_tools-2.3.2/ss13_tools/slur_detector/__init__.py
--rw-r--r--   0        0        0      320 2023-06-27 22:02:31.230661 ss13_tools-2.3.2/ss13_tools/slur_detector/__main__.py
--rw-r--r--   0        0        0       21 2023-06-27 22:02:31.230661 ss13_tools-2.3.2/ss13_tools/slur_detector/constants.py
--rw-r--r--   0        0        0     2740 2023-06-27 22:02:31.230661 ss13_tools-2.3.2/ss13_tools/slur_detector/slur_detector.py
--rw-r--r--   0        0        0      987 2023-06-27 22:02:31.230661 ss13_tools-2.3.2/ss13_tools/slur_detector/slur_file.py
--rw-r--r--   0        0        0      201 2023-06-27 22:02:31.230661 ss13_tools-2.3.2/ss13_tools/slur_detector/word_detection.py
--rw-r--r--   0        0        0      327 2023-06-27 22:02:31.230661 ss13_tools-2.3.2/ss13_tools/util.py
--rw-r--r--   0        0        0     3172 1970-01-01 00:00:00.000000 ss13_tools-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0     2301 2023-06-30 23:13:20.775557 ss13_tools-2.3.3/README.md
+-rw-r--r--   0        0        0     1008 2023-06-30 23:13:20.783557 ss13_tools-2.3.3/pyproject.toml
+-rw-r--r--   0        0        0      325 2023-06-30 23:13:20.783557 ss13_tools-2.3.3/ss13_tools/__init__.py
+-rw-r--r--   0        0        0     1175 2023-06-30 23:13:20.783557 ss13_tools-2.3.3/ss13_tools/__main__.py
+-rw-r--r--   0        0        0       22 2023-06-30 23:13:20.783557 ss13_tools-2.3.3/ss13_tools/__version__.py
+-rw-r--r--   0        0        0      438 2023-06-30 23:13:20.783557 ss13_tools-2.3.3/ss13_tools/auth/__init__.py
+-rw-r--r--   0        0        0      205 2023-06-30 23:13:20.783557 ss13_tools-2.3.3/ss13_tools/auth/__main__.py
+-rw-r--r--   0        0        0      346 2023-06-30 23:13:20.783557 ss13_tools-2.3.3/ss13_tools/auth/constants.py
+-rw-r--r--   0        0        0    10698 2023-06-30 23:13:20.783557 ss13_tools-2.3.3/ss13_tools/auth/tg.py
+-rw-r--r--   0        0        0      182 2023-06-30 23:13:20.783557 ss13_tools-2.3.3/ss13_tools/byond/__init__.py
+-rw-r--r--   0        0        0      543 2023-06-30 23:13:20.783557 ss13_tools-2.3.3/ss13_tools/byond/__main__.py
+-rw-r--r--   0        0        0       59 2023-06-30 23:13:20.783557 ss13_tools-2.3.3/ss13_tools/byond/constants.py
+-rw-r--r--   0        0        0     2424 2023-06-30 23:13:20.783557 ss13_tools-2.3.3/ss13_tools/byond/key_tools.py
+-rw-r--r--   0        0        0      162 2023-06-30 23:13:20.783557 ss13_tools-2.3.3/ss13_tools/centcom/__init__.py
+-rw-r--r--   0        0        0     1099 2023-06-30 23:13:20.783557 ss13_tools-2.3.3/ss13_tools/centcom/__main__.py
+-rw-r--r--   0        0        0      394 2023-06-30 23:13:20.783557 ss13_tools-2.3.3/ss13_tools/centcom/ban.py
+-rw-r--r--   0        0        0     1492 2023-06-30 23:13:20.783557 ss13_tools-2.3.3/ss13_tools/centcom/ban_types.py
+-rw-r--r--   0        0        0       68 2023-06-30 23:13:20.783557 ss13_tools-2.3.3/ss13_tools/centcom/constants.py
+-rw-r--r--   0        0        0      614 2023-06-30 23:13:20.783557 ss13_tools-2.3.3/ss13_tools/cli.py
+-rw-r--r--   0        0        0      222 2023-06-30 23:13:20.783557 ss13_tools-2.3.3/ss13_tools/constants.py
+-rw-r--r--   0        0        0    18265 2023-06-30 23:13:20.783557 ss13_tools-2.3.3/ss13_tools/log_buddy/README.md
+-rw-r--r--   0        0        0      198 2023-06-30 23:13:20.783557 ss13_tools-2.3.3/ss13_tools/log_buddy/__init__.py
+-rw-r--r--   0        0        0     5561 2023-06-30 23:13:20.783557 ss13_tools-2.3.3/ss13_tools/log_buddy/__main__.py
+-rw-r--r--   0        0        0      768 2023-06-30 23:13:20.783557 ss13_tools-2.3.3/ss13_tools/log_buddy/constants.py
+-rw-r--r--   0        0        0      562 2023-06-30 23:13:20.783557 ss13_tools-2.3.3/ss13_tools/log_buddy/expressions.py
+-rw-r--r--   0        0        0    52497 2023-06-30 23:13:20.787557 ss13_tools-2.3.3/ss13_tools/log_buddy/log.py
+-rw-r--r--   0        0        0    17063 2023-06-30 23:13:20.787557 ss13_tools-2.3.3/ss13_tools/log_buddy/log_magics.py
+-rw-r--r--   0        0        0    28437 2023-06-30 23:13:20.787557 ss13_tools-2.3.3/ss13_tools/log_buddy/log_parser.py
+-rw-r--r--   0        0        0      554 2023-06-30 23:13:20.787557 ss13_tools-2.3.3/ss13_tools/log_downloader/__init__.py
+-rw-r--r--   0        0        0     2011 2023-06-30 23:13:20.787557 ss13_tools-2.3.3/ss13_tools/log_downloader/__main__.py
+-rw-r--r--   0        0        0     7641 2023-06-30 23:13:20.787557 ss13_tools-2.3.3/ss13_tools/log_downloader/base.py
+-rw-r--r--   0        0        0     4783 2023-06-30 23:13:20.787557 ss13_tools-2.3.3/ss13_tools/log_downloader/ckey.py
+-rw-r--r--   0        0        0      517 2023-06-30 23:13:20.787557 ss13_tools-2.3.3/ss13_tools/log_downloader/constants.py
+-rw-r--r--   0        0        0     4546 2023-06-30 23:13:20.787557 ss13_tools-2.3.3/ss13_tools/log_downloader/round.py
+-rw-r--r--   0        0        0    10429 2023-06-30 23:13:20.787557 ss13_tools-2.3.3/ss13_tools/menu.py
+-rw-r--r--   0        0        0     1247 2023-06-30 23:13:20.787557 ss13_tools-2.3.3/ss13_tools/menu_item.py
+-rw-r--r--   0        0        0     1880 2023-06-30 23:13:20.787557 ss13_tools-2.3.3/ss13_tools/scrubby/CKeyController.py
+-rw-r--r--   0        0        0     2341 2023-06-30 23:13:20.787557 ss13_tools-2.3.3/ss13_tools/scrubby/RoundController.py
+-rw-r--r--   0        0        0      622 2023-06-30 23:13:20.787557 ss13_tools-2.3.3/ss13_tools/scrubby/__init__.py
+-rw-r--r--   0        0        0      107 2023-06-30 23:13:20.787557 ss13_tools-2.3.3/ss13_tools/scrubby/__main__.py
+-rw-r--r--   0        0        0      433 2023-06-30 23:13:20.787557 ss13_tools-2.3.3/ss13_tools/scrubby/constants.py
+-rw-r--r--   0        0        0        0 2023-06-30 23:13:20.787557 ss13_tools-2.3.3/ss13_tools/scrubby/investigate.py
+-rw-r--r--   0        0        0     1201 2023-06-30 23:13:20.787557 ss13_tools-2.3.3/ss13_tools/scrubby/round_data.py
+-rw-r--r--   0        0        0      154 2023-06-30 23:13:20.787557 ss13_tools-2.3.3/ss13_tools/slur_detector/__init__.py
+-rw-r--r--   0        0        0      320 2023-06-30 23:13:20.787557 ss13_tools-2.3.3/ss13_tools/slur_detector/__main__.py
+-rw-r--r--   0        0        0       21 2023-06-30 23:13:20.787557 ss13_tools-2.3.3/ss13_tools/slur_detector/constants.py
+-rw-r--r--   0        0        0     2740 2023-06-30 23:13:20.787557 ss13_tools-2.3.3/ss13_tools/slur_detector/slur_detector.py
+-rw-r--r--   0        0        0      987 2023-06-30 23:13:20.787557 ss13_tools-2.3.3/ss13_tools/slur_detector/slur_file.py
+-rw-r--r--   0        0        0      201 2023-06-30 23:13:20.787557 ss13_tools-2.3.3/ss13_tools/slur_detector/word_detection.py
+-rw-r--r--   0        0        0      327 2023-06-30 23:13:20.787557 ss13_tools-2.3.3/ss13_tools/util.py
+-rw-r--r--   0        0        0     3172 1970-01-01 00:00:00.000000 ss13_tools-2.3.3/PKG-INFO
```

### Comparing `ss13_tools-2.3.2/README.md` & `ss13_tools-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.3.2/pyproject.toml` & `ss13_tools-2.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SS13-tools"
-version = "2.3.2"
+version = "2.3.3"
 description = "Python toolchain for SS13"
 authors = ["RigglePrime <27156122+RigglePrime@users.noreply.github.com>", "tattle <66640614+dragomagol@users.noreply.github.com>"]
 readme = "README.md"
 repository = "https://github.com/RigglePrime/SS13-tools"
 keywords = ["ss13", "tgstation"]
 
 [tool.poetry.dependencies]
```

### Comparing `ss13_tools-2.3.2/ss13_tools/__main__.py` & `ss13_tools-2.3.3/ss13_tools/__main__.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.3.2/ss13_tools/auth/tg.py` & `ss13_tools-2.3.3/ss13_tools/auth/tg.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.3.2/ss13_tools/byond/__main__.py` & `ss13_tools-2.3.3/ss13_tools/byond/__main__.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.3.2/ss13_tools/byond/key_tools.py` & `ss13_tools-2.3.3/ss13_tools/byond/key_tools.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.3.2/ss13_tools/centcom/__main__.py` & `ss13_tools-2.3.3/ss13_tools/centcom/__main__.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.3.2/ss13_tools/centcom/ban_types.py` & `ss13_tools-2.3.3/ss13_tools/centcom/ban_types.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.3.2/ss13_tools/cli.py` & `ss13_tools-2.3.3/ss13_tools/cli.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.3.2/ss13_tools/log_buddy/README.md` & `ss13_tools-2.3.3/ss13_tools/log_buddy/README.md`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.3.2/ss13_tools/log_buddy/__main__.py` & `ss13_tools-2.3.3/ss13_tools/log_buddy/__main__.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.3.2/ss13_tools/log_buddy/constants.py` & `ss13_tools-2.3.3/ss13_tools/log_buddy/constants.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.3.2/ss13_tools/log_buddy/expressions.py` & `ss13_tools-2.3.3/ss13_tools/log_buddy/expressions.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.3.2/ss13_tools/log_buddy/log.py` & `ss13_tools-2.3.3/ss13_tools/log_buddy/log.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.3.2/ss13_tools/log_buddy/log_magics.py` & `ss13_tools-2.3.3/ss13_tools/log_buddy/log_magics.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.3.2/ss13_tools/log_buddy/log_parser.py` & `ss13_tools-2.3.3/ss13_tools/log_buddy/log_parser.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.3.2/ss13_tools/log_downloader/__init__.py` & `ss13_tools-2.3.3/ss13_tools/log_downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.3.2/ss13_tools/log_downloader/__main__.py` & `ss13_tools-2.3.3/ss13_tools/log_downloader/__main__.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.3.2/ss13_tools/log_downloader/base.py` & `ss13_tools-2.3.3/ss13_tools/log_downloader/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,21 +36,30 @@
         )
 
 
 class LogDownloader(ABC):
     """Log downloader object. For downloading logs.
     Either pass the arguments in the constructor or call `interactive()`"""
 
-    user_agent: Annotated[str, "User agent so people know who keeps spamming requests (and for raw logs)"] = USER_AGENT
-    output_path: Annotated[str, "Where should we write the file to?"] = DEFAULT_OUTPUT_PATH
-    round_resources: Annotated[list[RoundResource], "The list of round resoruces to download"] = []
-    files: Annotated[list[str], "Which files do we want to dowload?"] = DEFAULT_FILES.copy()
-    output_only_log_line: Annotated[bool, "Should we format our line or not?"] = False
-    silent: Annotated[bool, "Should we be quiet?"] = False
-    __authed = False
+    user_agent: Annotated[str, "User agent so people know who keeps spamming requests (and for raw logs)"]
+    output_path: Annotated[str, "Where should we write the file to?"]
+    round_resources: Annotated[list[RoundResource], "The list of round resoruces to download"]
+    files: Annotated[list[str], "Which files do we want to dowload?"]
+    output_only_log_line: Annotated[bool, "Should we format our line or not?"]
+    silent: Annotated[bool, "Should we be quiet?"]
+    __authed: Annotated[bool, "Are we authenticated?"]
+
+    def __init__(self) -> None:
+        self.user_agent = USER_AGENT
+        self.output_path = DEFAULT_OUTPUT_PATH
+        self.round_resources = []
+        self.files = DEFAULT_FILES.copy()
+        self.output_only_log_line = False
+        self.silent = False
+        self.__authed = False
 
     def authenticate(self, token: str, override_old: bool) -> bool:
         """Tries to authenticate against the TG forums"""
         if is_authenticated():
             return True
         return create_from_token(token=token, override_old=override_old)
```

### Comparing `ss13_tools-2.3.2/ss13_tools/log_downloader/ckey.py` & `ss13_tools-2.3.3/ss13_tools/log_downloader/ckey.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         = DEFAULT_ONLY_PLAYED
     number_of_rounds: Annotated[int, "The number of rounds to download"] = DEFAULT_NUMBER_OF_ROUNDS
     output_path: Annotated[str, "Where should we write the file to?"] = DEFAULT_CKEY_OUTPUT_PATH.format(ckey="output")
     filter_logs: Annotated[bool, "Should we filter the logs?"] = True
 
     def __init__(self, key: str = None, only_played: bool = DEFAULT_ONLY_PLAYED,
                  number_of_rounds: int = DEFAULT_NUMBER_OF_ROUNDS, output_path: str = None) -> None:
+        super().__init__()
         self.key = key
         self.ckey = canonicalize(key) if self.key else None
         self.only_played = only_played
         self.number_of_rounds = number_of_rounds
         output_path = output_path or DEFAULT_CKEY_OUTPUT_PATH
         self.output_path = output_path.format(ckey=self.ckey or "output")
```

### Comparing `ss13_tools-2.3.2/ss13_tools/log_downloader/constants.py` & `ss13_tools-2.3.3/ss13_tools/log_downloader/constants.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.3.2/ss13_tools/log_downloader/round.py` & `ss13_tools-2.3.3/ss13_tools/log_downloader/round.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 class RoundLogDownloader(LogDownloader):
     """Downloads a span of rounds"""
     lbound: Annotated[int, "Left boundary"]
     rbound: Annotated[int, "Right boundary"]
 
     def __init__(self, start_round: int, end_round: int, output_path: str = None) -> None:
+        super().__init__()
         self.lbound = min(start_round, end_round)
         self.rbound = max(start_round, end_round)
         self.output_path = output_path or DEFAULT_ROUND_OUTPUT_PATH.format(start=self.lbound, end=self.rbound)
 
     async def _update_round_list(self) -> None:
         def round_list_generator():
             i = self.lbound
@@ -63,14 +64,15 @@
 
 
 class RoundListLogDownloader(LogDownloader):
     """Downloads a span of rounds"""
     round_list: Annotated[list[int], "List of rounds to get"]
 
     def __init__(self, round_list, output_path: str = None) -> None:
+        super().__init__()
         self.round_list = round_list
         self.output_path = output_path or DEFAULT_ROUND_LIST_OUTPUT_PATH
 
     async def _update_round_list(self) -> None:
         async for round_info in get_round_info_from_ids(self.round_list):
             round_info.timestamp = isoparse(round_info.timestamp)
             for file_name in self.files:
```

### Comparing `ss13_tools-2.3.2/ss13_tools/menu.py` & `ss13_tools-2.3.3/ss13_tools/menu.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.3.2/ss13_tools/menu_item.py` & `ss13_tools-2.3.3/ss13_tools/menu_item.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.3.2/ss13_tools/scrubby/CKeyController.py` & `ss13_tools-2.3.3/ss13_tools/scrubby/CKeyController.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.3.2/ss13_tools/scrubby/RoundController.py` & `ss13_tools-2.3.3/ss13_tools/scrubby/RoundController.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.3.2/ss13_tools/scrubby/__init__.py` & `ss13_tools-2.3.3/ss13_tools/scrubby/__init__.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.3.2/ss13_tools/scrubby/round_data.py` & `ss13_tools-2.3.3/ss13_tools/scrubby/round_data.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.3.2/ss13_tools/slur_detector/slur_detector.py` & `ss13_tools-2.3.3/ss13_tools/slur_detector/slur_detector.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.3.2/ss13_tools/slur_detector/slur_file.py` & `ss13_tools-2.3.3/ss13_tools/slur_detector/slur_file.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.3.2/PKG-INFO` & `ss13_tools-2.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ss13-tools
-Version: 2.3.2
+Version: 2.3.3
 Summary: Python toolchain for SS13
 Home-page: https://github.com/RigglePrime/SS13-tools
 Keywords: ss13,tgstation
 Author: RigglePrime
 Author-email: 27156122+RigglePrime@users.noreply.github.com
 Requires-Python: >=3.9.1,<3.12
 Classifier: Programming Language :: Python :: 3
```

