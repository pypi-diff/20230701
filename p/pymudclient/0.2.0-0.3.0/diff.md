# Comparing `tmp/pymudclient-0.2.0.tar.gz` & `tmp/pymudclient-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymudclient-0.2.0.tar", last modified: Thu Jun 29 13:11:45 2023, max compression
+gzip compressed data, was "pymudclient-0.3.0.tar", last modified: Sat Jul  1 06:29:53 2023, max compression
```

## Comparing `pymudclient-0.2.0.tar` & `pymudclient-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-06-29 13:11:45.281327 pymudclient-0.2.0/
--rw-r--r--   0 eddiehsu   (501) staff       (20)     1063 2023-06-29 07:55:53.000000 pymudclient-0.2.0/LICENSE
--rw-r--r--   0 eddiehsu   (501) staff       (20)     5580 2023-06-29 13:11:45.281006 pymudclient-0.2.0/PKG-INFO
--rw-r--r--   0 eddiehsu   (501) staff       (20)     4909 2023-06-29 13:06:30.000000 pymudclient-0.2.0/README.md
-drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-06-29 13:11:45.277569 pymudclient-0.2.0/pymudclient/
--rw-r--r--   0 eddiehsu   (501) staff       (20)      376 2023-06-29 12:57:57.000000 pymudclient-0.2.0/pymudclient/__init__.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      439 2023-06-29 07:55:53.000000 pymudclient-0.2.0/pymudclient/display.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     6122 2023-06-29 13:09:24.000000 pymudclient-0.2.0/pymudclient/input_cmd.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     3247 2023-06-29 07:55:53.000000 pymudclient-0.2.0/pymudclient/kbhit.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     3325 2023-06-29 08:18:52.000000 pymudclient-0.2.0/pymudclient/mud.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     1888 2023-06-29 13:07:44.000000 pymudclient-0.2.0/pymudclient/recv.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      800 2023-06-29 07:55:53.000000 pymudclient-0.2.0/pymudclient/shared_data.py
-drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-06-29 13:11:45.280531 pymudclient-0.2.0/pymudclient/utils/
--rw-r--r--   0 eddiehsu   (501) staff       (20)        0 2023-06-29 07:55:53.000000 pymudclient-0.2.0/pymudclient/utils/__init__.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      197 2023-06-29 07:55:53.000000 pymudclient-0.2.0/pymudclient/utils/codec.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     1563 2023-06-29 07:55:53.000000 pymudclient-0.2.0/pymudclient/utils/colors.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      859 2023-06-29 07:55:53.000000 pymudclient-0.2.0/pymudclient/utils/print.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      483 2023-06-29 07:55:53.000000 pymudclient-0.2.0/pymudclient/utils/telnet.py
-drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-06-29 13:11:45.279111 pymudclient-0.2.0/pymudclient.egg-info/
--rw-r--r--   0 eddiehsu   (501) staff       (20)     5580 2023-06-29 13:11:45.000000 pymudclient-0.2.0/pymudclient.egg-info/PKG-INFO
--rw-r--r--   0 eddiehsu   (501) staff       (20)      514 2023-06-29 13:11:45.000000 pymudclient-0.2.0/pymudclient.egg-info/SOURCES.txt
--rw-r--r--   0 eddiehsu   (501) staff       (20)        1 2023-06-29 13:11:45.000000 pymudclient-0.2.0/pymudclient.egg-info/dependency_links.txt
--rw-r--r--   0 eddiehsu   (501) staff       (20)       55 2023-06-29 13:11:45.000000 pymudclient-0.2.0/pymudclient.egg-info/requires.txt
--rw-r--r--   0 eddiehsu   (501) staff       (20)       12 2023-06-29 13:11:45.000000 pymudclient-0.2.0/pymudclient.egg-info/top_level.txt
--rw-r--r--   0 eddiehsu   (501) staff       (20)      689 2023-06-29 07:55:53.000000 pymudclient-0.2.0/pyproject.toml
--rw-r--r--   0 eddiehsu   (501) staff       (20)       38 2023-06-29 13:11:45.281444 pymudclient-0.2.0/setup.cfg
--rw-r--r--   0 eddiehsu   (501) staff       (20)     1362 2023-06-29 13:11:16.000000 pymudclient-0.2.0/setup.py
+drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-07-01 06:29:53.007373 pymudclient-0.3.0/
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1063 2023-06-29 07:55:53.000000 pymudclient-0.3.0/LICENSE
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     5544 2023-07-01 06:29:53.006770 pymudclient-0.3.0/PKG-INFO
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     4873 2023-07-01 06:29:09.000000 pymudclient-0.3.0/README.md
+drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-07-01 06:29:53.000673 pymudclient-0.3.0/pymudclient/
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      376 2023-06-29 12:57:57.000000 pymudclient-0.3.0/pymudclient/__init__.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      456 2023-06-29 13:26:20.000000 pymudclient-0.3.0/pymudclient/display.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     6058 2023-07-01 06:27:34.000000 pymudclient-0.3.0/pymudclient/input_cmd.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1964 2023-07-01 06:27:30.000000 pymudclient-0.3.0/pymudclient/kbhit.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     3325 2023-06-29 08:18:52.000000 pymudclient-0.3.0/pymudclient/mud.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1888 2023-06-29 13:07:44.000000 pymudclient-0.3.0/pymudclient/recv.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      800 2023-06-29 07:55:53.000000 pymudclient-0.3.0/pymudclient/shared_data.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      964 2023-07-01 05:49:45.000000 pymudclient-0.3.0/pymudclient/tmp.py
+drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-07-01 06:29:53.005621 pymudclient-0.3.0/pymudclient/utils/
+-rw-r--r--   0 eddiehsu   (501) staff       (20)        0 2023-06-29 07:55:53.000000 pymudclient-0.3.0/pymudclient/utils/__init__.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      197 2023-06-29 07:55:53.000000 pymudclient-0.3.0/pymudclient/utils/codec.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1563 2023-06-29 07:55:53.000000 pymudclient-0.3.0/pymudclient/utils/colors.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      859 2023-06-29 07:55:53.000000 pymudclient-0.3.0/pymudclient/utils/print.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      483 2023-06-29 07:55:53.000000 pymudclient-0.3.0/pymudclient/utils/telnet.py
+drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-07-01 06:29:53.002499 pymudclient-0.3.0/pymudclient.egg-info/
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     5544 2023-07-01 06:29:52.000000 pymudclient-0.3.0/pymudclient.egg-info/PKG-INFO
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      533 2023-07-01 06:29:52.000000 pymudclient-0.3.0/pymudclient.egg-info/SOURCES.txt
+-rw-r--r--   0 eddiehsu   (501) staff       (20)        1 2023-07-01 06:29:52.000000 pymudclient-0.3.0/pymudclient.egg-info/dependency_links.txt
+-rw-r--r--   0 eddiehsu   (501) staff       (20)       55 2023-07-01 06:29:52.000000 pymudclient-0.3.0/pymudclient.egg-info/requires.txt
+-rw-r--r--   0 eddiehsu   (501) staff       (20)       12 2023-07-01 06:29:52.000000 pymudclient-0.3.0/pymudclient.egg-info/top_level.txt
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      689 2023-06-29 07:55:53.000000 pymudclient-0.3.0/pyproject.toml
+-rw-r--r--   0 eddiehsu   (501) staff       (20)       38 2023-07-01 06:29:53.007549 pymudclient-0.3.0/setup.cfg
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1362 2023-07-01 06:28:51.000000 pymudclient-0.3.0/setup.py
```

### Comparing `pymudclient-0.2.0/LICENSE` & `pymudclient-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymudclient-0.2.0/PKG-INFO` & `pymudclient-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymudclient
-Version: 0.2.0
+Version: 0.3.0
 Summary: A MUD client core written in Python
 Home-page: https://github.com/griiid/PyMudClient
 Download-URL: https://pypi.org/project/pymudclient/
 Author: griiid
 Author-email: gridwing@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
@@ -14,52 +14,54 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# pymudclient: 用 Python 開發的 MUD Client 核心
+# PyMudClient: 用 Python 開發的 MUD Client 核心
 
-- [pymudclient: 用 Python 開發的 MUD Client 核心](#pymudclient-用-python-開發的-mud-client-核心)
+## 這是什麼？
+
+- MUD, Multi-User Dungeon，是多人即時虛擬類遊戲，通常以文字描述為基礎。
+- **pymudclient** 實作了連線、斷線重連、顯示、輸入介面、Alias、Trigger、Timer 的功能。
+
+---
+
+- [PyMudClient: 用 Python 開發的 MUD Client 核心](#pymudclient-用-python-開發的-mud-client-核心)
   - [這是什麼？](#這是什麼)
   - [已測試過環境](#已測試過環境)
-  - [功能說明](#功能說明)
+  - [支援功能](#支援功能)
   - [安裝](#安裝)
   - [使用範例](#使用範例)
-  - [功能說明](#功能說明-1)
+  - [功能說明](#功能說明)
     - [run](#run)
     - [Alias](#alias)
       - [Alias class 參數](#alias-class-參數)
       - [使用範例](#使用範例-1)
     - [Trigger](#trigger)
       - [Trigger class 參數](#trigger-class-參數)
       - [使用範例](#使用範例-2)
     - [Timer](#timer)
       - [Timer class 參數](#timer-class-參數)
       - [使用範例](#使用範例-3)
   - [已知問題](#已知問題)
   - [License](#license)
 
-## 這是什麼？
-
-- MUD, Multi-User Dungeon，是多人即時虛擬類遊戲，通常以文字描述為基礎。
-- **pymudclient** 實作了連線、斷線重連、顯示、輸入介面、Alias、Trigger、Timer 的功能。
-
 ## 已測試過環境
 
 - macOS Ventura 13.3.1 (a)
 - GNU/Linux 5.15.0-1032-raspi aarch64
 
-## 功能說明
+## 支援功能
 
 - 連線：根據輸入的 host 跟 port 進行連線。
 - 斷線重連：發生異常、server 重新啟動導致的斷線，會等待 3 秒後重新連線。
 - 顯示：顯示 server 回傳的內容。
-  - 有處理 big5 中文顯示的問題。
+  - 有處理輸入中文的顯示問題。
   - 只針對萬王之王 (kk.muds.idv.tw:4000) 進行測試過。
 - 輸入介面：在最後一行顯示輸入的文字；送出的文字還沒有改動時按下 Enter 會再送一次。
 
 ## 安裝
 
 `pip install pymudclient`
 
@@ -84,14 +86,16 @@
 )
 ```
 
 ## 功能說明
 
 ### run
 
+- 連線至 `<host>:<port>`
+
 ```py
 run(host, port, alias_list=None, trigger_list=None, timer_list=None)
 ```
 
 - host `string`: 連線的主機網址或 IP。
 - port `number`: 連線的主機 port。
 - alias_list `list`: (optional) Alias 清單，參考[下面說明](#alias)。
@@ -168,12 +172,12 @@
 ]
 ```
 
 - 每 900 秒傳送一個 `save` 到 host。
 
 ## 已知問題
 
-- ctrl-z 把 process 移到背景後，再 fg 切回前景，輸入會變得異常。
+- 目前沒有。
 
 ## License
 
 - [MIT](https://github.com/griiid/PyMudClient/blob/master/LICENSE)
```

### Comparing `pymudclient-0.2.0/README.md` & `pymudclient-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,47 @@
-# pymudclient: 用 Python 開發的 MUD Client 核心
+# PyMudClient: 用 Python 開發的 MUD Client 核心
 
-- [pymudclient: 用 Python 開發的 MUD Client 核心](#pymudclient-用-python-開發的-mud-client-核心)
+## 這是什麼？
+
+- MUD, Multi-User Dungeon，是多人即時虛擬類遊戲，通常以文字描述為基礎。
+- **pymudclient** 實作了連線、斷線重連、顯示、輸入介面、Alias、Trigger、Timer 的功能。
+
+---
+
+- [PyMudClient: 用 Python 開發的 MUD Client 核心](#pymudclient-用-python-開發的-mud-client-核心)
   - [這是什麼？](#這是什麼)
   - [已測試過環境](#已測試過環境)
-  - [功能說明](#功能說明)
+  - [支援功能](#支援功能)
   - [安裝](#安裝)
   - [使用範例](#使用範例)
-  - [功能說明](#功能說明-1)
+  - [功能說明](#功能說明)
     - [run](#run)
     - [Alias](#alias)
       - [Alias class 參數](#alias-class-參數)
       - [使用範例](#使用範例-1)
     - [Trigger](#trigger)
       - [Trigger class 參數](#trigger-class-參數)
       - [使用範例](#使用範例-2)
     - [Timer](#timer)
       - [Timer class 參數](#timer-class-參數)
       - [使用範例](#使用範例-3)
   - [已知問題](#已知問題)
   - [License](#license)
 
-## 這是什麼？
-
-- MUD, Multi-User Dungeon，是多人即時虛擬類遊戲，通常以文字描述為基礎。
-- **pymudclient** 實作了連線、斷線重連、顯示、輸入介面、Alias、Trigger、Timer 的功能。
-
 ## 已測試過環境
 
 - macOS Ventura 13.3.1 (a)
 - GNU/Linux 5.15.0-1032-raspi aarch64
 
-## 功能說明
+## 支援功能
 
 - 連線：根據輸入的 host 跟 port 進行連線。
 - 斷線重連：發生異常、server 重新啟動導致的斷線，會等待 3 秒後重新連線。
 - 顯示：顯示 server 回傳的內容。
-  - 有處理 big5 中文顯示的問題。
+  - 有處理輸入中文的顯示問題。
   - 只針對萬王之王 (kk.muds.idv.tw:4000) 進行測試過。
 - 輸入介面：在最後一行顯示輸入的文字；送出的文字還沒有改動時按下 Enter 會再送一次。
 
 ## 安裝
 
 `pip install pymudclient`
 
@@ -64,14 +66,16 @@
 )
 ```
 
 ## 功能說明
 
 ### run
 
+- 連線至 `<host>:<port>`
+
 ```py
 run(host, port, alias_list=None, trigger_list=None, timer_list=None)
 ```
 
 - host `string`: 連線的主機網址或 IP。
 - port `number`: 連線的主機 port。
 - alias_list `list`: (optional) Alias 清單，參考[下面說明](#alias)。
@@ -148,12 +152,12 @@
 ]
 ```
 
 - 每 900 秒傳送一個 `save` 到 host。
 
 ## 已知問題
 
-- ctrl-z 把 process 移到背景後，再 fg 切回前景，輸入會變得異常。
+- 目前沒有。
 
 ## License
 
 - [MIT](https://github.com/griiid/PyMudClient/blob/master/LICENSE)
```

### Comparing `pymudclient-0.2.0/pymudclient/input_cmd.py` & `pymudclient-0.3.0/pymudclient/input_cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,23 +14,16 @@
 from .utils.telnet import send_to_host
 
 kb = KBHit()
 
 alias_list = None
 
 
-def _getch():
-    if not kb.kbhit():
-        return None
-    return kb.getch()
-
-
 def _input_visible(char, char_ord):
-    '''ASCII 可視字元 或 中文字'''
-
+    # 不是ASCII 可視字元 或 中文字
     if char_ord < 0x20 or 0x7E < char_ord < 0x4E00 or 0x9FA5 < char_ord:
         return
 
     if g_input['last_send'] != '':
         g_input['last_send'] = ''
 
     g_input['input'] = (
@@ -39,15 +32,15 @@
     g_input['input_index'] += 1
 
 
 def _input_ctrl_c(_, char_ord):
     if char_ord != 0x03:
         return False
 
-    g_input['is_running'] = False
+    g_is_running.set(False),
     color_print('\r\n$HIY$中斷程式$NOR$')
     return True
 
 
 def _input_0x1B(_, char_ord):
     if char_ord != 0x1B:
         # Not Special Command
@@ -209,27 +202,28 @@
                     text = timer.func()
                     if text:
                         send_to_host(text)
 
 
 INPUT_FUNCTION_LIST = [
     _input_visible,
+    _input_ctrl_c,
     _input_0x1B,
     _input_backspace,
     _input_enter,
 ]
 
 
 def thread_job_input_cmd(alias_list_, timer_list):
     global alias_list
     alias_list = alias_list_
     timer_processor = TimerProcessor(timer_list)
 
     while g_is_running.get() and not g_is_reconnect.get():
-        char = _getch()
+        char = kb.getch()
         if char is None:
             timer_processor.process()
             time.sleep(0.01)
             continue
 
         char_ord = ord(char)
```

### Comparing `pymudclient-0.2.0/pymudclient/mud.py` & `pymudclient-0.3.0/pymudclient/mud.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.2.0/pymudclient/recv.py` & `pymudclient-0.3.0/pymudclient/recv.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.2.0/pymudclient/shared_data.py` & `pymudclient-0.3.0/pymudclient/shared_data.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.2.0/pymudclient/utils/colors.py` & `pymudclient-0.3.0/pymudclient/utils/colors.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.2.0/pymudclient/utils/print.py` & `pymudclient-0.3.0/pymudclient/utils/print.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.2.0/pymudclient.egg-info/PKG-INFO` & `pymudclient-0.3.0/pymudclient.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymudclient
-Version: 0.2.0
+Version: 0.3.0
 Summary: A MUD client core written in Python
 Home-page: https://github.com/griiid/PyMudClient
 Download-URL: https://pypi.org/project/pymudclient/
 Author: griiid
 Author-email: gridwing@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
@@ -14,52 +14,54 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# pymudclient: 用 Python 開發的 MUD Client 核心
+# PyMudClient: 用 Python 開發的 MUD Client 核心
 
-- [pymudclient: 用 Python 開發的 MUD Client 核心](#pymudclient-用-python-開發的-mud-client-核心)
+## 這是什麼？
+
+- MUD, Multi-User Dungeon，是多人即時虛擬類遊戲，通常以文字描述為基礎。
+- **pymudclient** 實作了連線、斷線重連、顯示、輸入介面、Alias、Trigger、Timer 的功能。
+
+---
+
+- [PyMudClient: 用 Python 開發的 MUD Client 核心](#pymudclient-用-python-開發的-mud-client-核心)
   - [這是什麼？](#這是什麼)
   - [已測試過環境](#已測試過環境)
-  - [功能說明](#功能說明)
+  - [支援功能](#支援功能)
   - [安裝](#安裝)
   - [使用範例](#使用範例)
-  - [功能說明](#功能說明-1)
+  - [功能說明](#功能說明)
     - [run](#run)
     - [Alias](#alias)
       - [Alias class 參數](#alias-class-參數)
       - [使用範例](#使用範例-1)
     - [Trigger](#trigger)
       - [Trigger class 參數](#trigger-class-參數)
       - [使用範例](#使用範例-2)
     - [Timer](#timer)
       - [Timer class 參數](#timer-class-參數)
       - [使用範例](#使用範例-3)
   - [已知問題](#已知問題)
   - [License](#license)
 
-## 這是什麼？
-
-- MUD, Multi-User Dungeon，是多人即時虛擬類遊戲，通常以文字描述為基礎。
-- **pymudclient** 實作了連線、斷線重連、顯示、輸入介面、Alias、Trigger、Timer 的功能。
-
 ## 已測試過環境
 
 - macOS Ventura 13.3.1 (a)
 - GNU/Linux 5.15.0-1032-raspi aarch64
 
-## 功能說明
+## 支援功能
 
 - 連線：根據輸入的 host 跟 port 進行連線。
 - 斷線重連：發生異常、server 重新啟動導致的斷線，會等待 3 秒後重新連線。
 - 顯示：顯示 server 回傳的內容。
-  - 有處理 big5 中文顯示的問題。
+  - 有處理輸入中文的顯示問題。
   - 只針對萬王之王 (kk.muds.idv.tw:4000) 進行測試過。
 - 輸入介面：在最後一行顯示輸入的文字；送出的文字還沒有改動時按下 Enter 會再送一次。
 
 ## 安裝
 
 `pip install pymudclient`
 
@@ -84,14 +86,16 @@
 )
 ```
 
 ## 功能說明
 
 ### run
 
+- 連線至 `<host>:<port>`
+
 ```py
 run(host, port, alias_list=None, trigger_list=None, timer_list=None)
 ```
 
 - host `string`: 連線的主機網址或 IP。
 - port `number`: 連線的主機 port。
 - alias_list `list`: (optional) Alias 清單，參考[下面說明](#alias)。
@@ -168,12 +172,12 @@
 ]
 ```
 
 - 每 900 秒傳送一個 `save` 到 host。
 
 ## 已知問題
 
-- ctrl-z 把 process 移到背景後，再 fg 切回前景，輸入會變得異常。
+- 目前沒有。
 
 ## License
 
 - [MIT](https://github.com/griiid/PyMudClient/blob/master/LICENSE)
```

### Comparing `pymudclient-0.2.0/pymudclient.egg-info/SOURCES.txt` & `pymudclient-0.3.0/pymudclient.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 pymudclient/__init__.py
 pymudclient/display.py
 pymudclient/input_cmd.py
 pymudclient/kbhit.py
 pymudclient/mud.py
 pymudclient/recv.py
 pymudclient/shared_data.py
+pymudclient/tmp.py
 pymudclient.egg-info/PKG-INFO
 pymudclient.egg-info/SOURCES.txt
 pymudclient.egg-info/dependency_links.txt
 pymudclient.egg-info/requires.txt
 pymudclient.egg-info/top_level.txt
 pymudclient/utils/__init__.py
 pymudclient/utils/codec.py
```

### Comparing `pymudclient-0.2.0/pyproject.toml` & `pymudclient-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymudclient-0.2.0/setup.py` & `pymudclient-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 PACKAGE_NAME = 'pymudclient'
 AUTHOR = 'griiid'
 AUTHOR_EMAIL = 'gridwing@gmail.com'
 URL = 'https://github.com/griiid/PyMudClient'
 DOWNLOAD_URL = 'https://pypi.org/project/pymudclient/'
 
 LICENSE = 'MIT'
-VERSION = '0.2.0'
+VERSION = '0.3.0'
 DESCRIPTION = 'A MUD client core written in Python'
 LONG_DESCRIPTION = (HERE  / 'README.md').read_text(encoding='utf8')
 LONG_DESC_TYPE = 'text/markdown'
 
 requirements = (HERE / 'requirements.txt').read_text(encoding='utf8')
 INSTALL_REQUIRES = [s.strip() for s in requirements.split('\n')]
```

