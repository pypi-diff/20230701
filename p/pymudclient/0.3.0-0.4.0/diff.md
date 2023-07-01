# Comparing `tmp/pymudclient-0.3.0.tar.gz` & `tmp/pymudclient-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymudclient-0.3.0.tar", last modified: Sat Jul  1 06:29:53 2023, max compression
+gzip compressed data, was "pymudclient-0.4.0.tar", last modified: Sat Jul  1 16:30:30 2023, max compression
```

## Comparing `pymudclient-0.3.0.tar` & `pymudclient-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-07-01 06:29:53.007373 pymudclient-0.3.0/
--rw-r--r--   0 eddiehsu   (501) staff       (20)     1063 2023-06-29 07:55:53.000000 pymudclient-0.3.0/LICENSE
--rw-r--r--   0 eddiehsu   (501) staff       (20)     5544 2023-07-01 06:29:53.006770 pymudclient-0.3.0/PKG-INFO
--rw-r--r--   0 eddiehsu   (501) staff       (20)     4873 2023-07-01 06:29:09.000000 pymudclient-0.3.0/README.md
-drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-07-01 06:29:53.000673 pymudclient-0.3.0/pymudclient/
--rw-r--r--   0 eddiehsu   (501) staff       (20)      376 2023-06-29 12:57:57.000000 pymudclient-0.3.0/pymudclient/__init__.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      456 2023-06-29 13:26:20.000000 pymudclient-0.3.0/pymudclient/display.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     6058 2023-07-01 06:27:34.000000 pymudclient-0.3.0/pymudclient/input_cmd.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     1964 2023-07-01 06:27:30.000000 pymudclient-0.3.0/pymudclient/kbhit.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     3325 2023-06-29 08:18:52.000000 pymudclient-0.3.0/pymudclient/mud.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     1888 2023-06-29 13:07:44.000000 pymudclient-0.3.0/pymudclient/recv.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      800 2023-06-29 07:55:53.000000 pymudclient-0.3.0/pymudclient/shared_data.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      964 2023-07-01 05:49:45.000000 pymudclient-0.3.0/pymudclient/tmp.py
-drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-07-01 06:29:53.005621 pymudclient-0.3.0/pymudclient/utils/
--rw-r--r--   0 eddiehsu   (501) staff       (20)        0 2023-06-29 07:55:53.000000 pymudclient-0.3.0/pymudclient/utils/__init__.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      197 2023-06-29 07:55:53.000000 pymudclient-0.3.0/pymudclient/utils/codec.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     1563 2023-06-29 07:55:53.000000 pymudclient-0.3.0/pymudclient/utils/colors.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      859 2023-06-29 07:55:53.000000 pymudclient-0.3.0/pymudclient/utils/print.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      483 2023-06-29 07:55:53.000000 pymudclient-0.3.0/pymudclient/utils/telnet.py
-drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-07-01 06:29:53.002499 pymudclient-0.3.0/pymudclient.egg-info/
--rw-r--r--   0 eddiehsu   (501) staff       (20)     5544 2023-07-01 06:29:52.000000 pymudclient-0.3.0/pymudclient.egg-info/PKG-INFO
--rw-r--r--   0 eddiehsu   (501) staff       (20)      533 2023-07-01 06:29:52.000000 pymudclient-0.3.0/pymudclient.egg-info/SOURCES.txt
--rw-r--r--   0 eddiehsu   (501) staff       (20)        1 2023-07-01 06:29:52.000000 pymudclient-0.3.0/pymudclient.egg-info/dependency_links.txt
--rw-r--r--   0 eddiehsu   (501) staff       (20)       55 2023-07-01 06:29:52.000000 pymudclient-0.3.0/pymudclient.egg-info/requires.txt
--rw-r--r--   0 eddiehsu   (501) staff       (20)       12 2023-07-01 06:29:52.000000 pymudclient-0.3.0/pymudclient.egg-info/top_level.txt
--rw-r--r--   0 eddiehsu   (501) staff       (20)      689 2023-06-29 07:55:53.000000 pymudclient-0.3.0/pyproject.toml
--rw-r--r--   0 eddiehsu   (501) staff       (20)       38 2023-07-01 06:29:53.007549 pymudclient-0.3.0/setup.cfg
--rw-r--r--   0 eddiehsu   (501) staff       (20)     1362 2023-07-01 06:28:51.000000 pymudclient-0.3.0/setup.py
+drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-07-01 16:30:30.867963 pymudclient-0.4.0/
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1063 2023-06-29 07:55:53.000000 pymudclient-0.4.0/LICENSE
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     6301 2023-07-01 16:30:30.867658 pymudclient-0.4.0/PKG-INFO
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     5630 2023-07-01 16:30:00.000000 pymudclient-0.4.0/README.md
+drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-07-01 16:30:30.863504 pymudclient-0.4.0/pymudclient/
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      376 2023-06-29 12:57:57.000000 pymudclient-0.4.0/pymudclient/__init__.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      456 2023-07-01 06:34:42.000000 pymudclient-0.4.0/pymudclient/display.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     7001 2023-07-01 15:57:58.000000 pymudclient-0.4.0/pymudclient/input_cmd.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     4543 2023-07-01 16:13:21.000000 pymudclient-0.4.0/pymudclient/kbhit.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     3365 2023-07-01 16:17:10.000000 pymudclient-0.4.0/pymudclient/mud.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1924 2023-07-01 16:00:32.000000 pymudclient-0.4.0/pymudclient/recv.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      800 2023-06-29 07:55:53.000000 pymudclient-0.4.0/pymudclient/shared_data.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1396 2023-07-01 13:53:52.000000 pymudclient-0.4.0/pymudclient/tmp.py
+drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-07-01 16:30:30.867103 pymudclient-0.4.0/pymudclient/utils/
+-rw-r--r--   0 eddiehsu   (501) staff       (20)        0 2023-06-29 07:55:53.000000 pymudclient-0.4.0/pymudclient/utils/__init__.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      197 2023-06-29 07:55:53.000000 pymudclient-0.4.0/pymudclient/utils/codec.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1563 2023-06-29 07:55:53.000000 pymudclient-0.4.0/pymudclient/utils/colors.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1331 2023-07-01 16:16:19.000000 pymudclient-0.4.0/pymudclient/utils/print.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      483 2023-06-29 07:55:53.000000 pymudclient-0.4.0/pymudclient/utils/telnet.py
+drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-07-01 16:30:30.865368 pymudclient-0.4.0/pymudclient.egg-info/
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     6301 2023-07-01 16:30:30.000000 pymudclient-0.4.0/pymudclient.egg-info/PKG-INFO
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      533 2023-07-01 16:30:30.000000 pymudclient-0.4.0/pymudclient.egg-info/SOURCES.txt
+-rw-r--r--   0 eddiehsu   (501) staff       (20)        1 2023-07-01 16:30:30.000000 pymudclient-0.4.0/pymudclient.egg-info/dependency_links.txt
+-rw-r--r--   0 eddiehsu   (501) staff       (20)       55 2023-07-01 16:30:30.000000 pymudclient-0.4.0/pymudclient.egg-info/requires.txt
+-rw-r--r--   0 eddiehsu   (501) staff       (20)       12 2023-07-01 16:30:30.000000 pymudclient-0.4.0/pymudclient.egg-info/top_level.txt
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      689 2023-06-29 07:55:53.000000 pymudclient-0.4.0/pyproject.toml
+-rw-r--r--   0 eddiehsu   (501) staff       (20)       38 2023-07-01 16:30:30.868058 pymudclient-0.4.0/setup.cfg
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1362 2023-07-01 16:20:26.000000 pymudclient-0.4.0/setup.py
```

### Comparing `pymudclient-0.3.0/LICENSE` & `pymudclient-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymudclient-0.3.0/PKG-INFO` & `pymudclient-0.4.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: pymudclient
-Version: 0.3.0
-Summary: A MUD client core written in Python
-Home-page: https://github.com/griiid/PyMudClient
-Download-URL: https://pypi.org/project/pymudclient/
-Author: griiid
-Author-email: gridwing@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # PyMudClient: 用 Python 開發的 MUD Client 核心
 
 ## 這是什麼？
 
 - MUD, Multi-User Dungeon，是多人即時虛擬類遊戲，通常以文字描述為基礎。
 - **pymudclient** 實作了連線、斷線重連、顯示、輸入介面、Alias、Trigger、Timer 的功能。
 
@@ -29,26 +9,28 @@
 
 - [PyMudClient: 用 Python 開發的 MUD Client 核心](#pymudclient-用-python-開發的-mud-client-核心)
   - [這是什麼？](#這是什麼)
   - [已測試過環境](#已測試過環境)
   - [支援功能](#支援功能)
   - [安裝](#安裝)
   - [使用範例](#使用範例)
-  - [功能說明](#功能說明)
+  - [輸入介面](#輸入介面)
+  - [API Reference](#api-reference)
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
+  - [尚未實作功能](#尚未實作功能)
   - [License](#license)
 
 ## 已測試過環境
 
 - macOS Ventura 13.3.1 (a)
 - GNU/Linux 5.15.0-1032-raspi aarch64
 
@@ -82,15 +64,24 @@
     PORT,
     alias_list=ALIAS_LIST,
     trigger_list=TRIGGER_LIST,
     timer_list=TIMER_LIST,
 )
 ```
 
-## 功能說明
+## 輸入介面
+
+- 輸入的文字會固定出現在最後一行。
+- 可使用 左/右/Home/End 移動位置。
+- 可使用 Backspace/Ctrl-H 刪除游標位置前面的字元。
+- 可使用 Delete 刪除游標位置後面的字元。
+- 可使用 Ctrl-W 刪除前面一個 word (仿照 vim 功能)。
+- 按下 Enter 送出後，會記住最後一次送出的文字，可以進行編輯，或直接按 Enter 再送一次。
+
+## API Reference
 
 ### run
 
 - 連線至 `<host>:<port>`
 
 ```py
 run(host, port, alias_list=None, trigger_list=None, timer_list=None)
@@ -174,10 +165,15 @@
 
 - 每 900 秒傳送一個 `save` 到 host。
 
 ## 已知問題
 
 - 目前沒有。
 
+## 尚未實作功能
+
+- 輸入功能的歷史紀錄，可按 上/下 選擇過去送出過的文字。
+- 有看過有些 mud 是有小地圖的功能，應該是 host 傳送過來更新的，這功能需要深入研究 mud 的資料傳送規則。
+
 ## License
 
 - [MIT](https://github.com/griiid/PyMudClient/blob/master/LICENSE)
```

### Comparing `pymudclient-0.3.0/README.md` & `pymudclient-0.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: pymudclient
+Version: 0.4.0
+Summary: A MUD client core written in Python
+Home-page: https://github.com/griiid/PyMudClient
+Download-URL: https://pypi.org/project/pymudclient/
+Author: griiid
+Author-email: gridwing@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # PyMudClient: 用 Python 開發的 MUD Client 核心
 
 ## 這是什麼？
 
 - MUD, Multi-User Dungeon，是多人即時虛擬類遊戲，通常以文字描述為基礎。
 - **pymudclient** 實作了連線、斷線重連、顯示、輸入介面、Alias、Trigger、Timer 的功能。
 
@@ -9,26 +29,28 @@
 
 - [PyMudClient: 用 Python 開發的 MUD Client 核心](#pymudclient-用-python-開發的-mud-client-核心)
   - [這是什麼？](#這是什麼)
   - [已測試過環境](#已測試過環境)
   - [支援功能](#支援功能)
   - [安裝](#安裝)
   - [使用範例](#使用範例)
-  - [功能說明](#功能說明)
+  - [輸入介面](#輸入介面)
+  - [API Reference](#api-reference)
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
+  - [尚未實作功能](#尚未實作功能)
   - [License](#license)
 
 ## 已測試過環境
 
 - macOS Ventura 13.3.1 (a)
 - GNU/Linux 5.15.0-1032-raspi aarch64
 
@@ -62,15 +84,24 @@
     PORT,
     alias_list=ALIAS_LIST,
     trigger_list=TRIGGER_LIST,
     timer_list=TIMER_LIST,
 )
 ```
 
-## 功能說明
+## 輸入介面
+
+- 輸入的文字會固定出現在最後一行。
+- 可使用 左/右/Home/End 移動位置。
+- 可使用 Backspace/Ctrl-H 刪除游標位置前面的字元。
+- 可使用 Delete 刪除游標位置後面的字元。
+- 可使用 Ctrl-W 刪除前面一個 word (仿照 vim 功能)。
+- 按下 Enter 送出後，會記住最後一次送出的文字，可以進行編輯，或直接按 Enter 再送一次。
+
+## API Reference
 
 ### run
 
 - 連線至 `<host>:<port>`
 
 ```py
 run(host, port, alias_list=None, trigger_list=None, timer_list=None)
@@ -154,10 +185,15 @@
 
 - 每 900 秒傳送一個 `save` 到 host。
 
 ## 已知問題
 
 - 目前沒有。
 
+## 尚未實作功能
+
+- 輸入功能的歷史紀錄，可按 上/下 選擇過去送出過的文字。
+- 有看過有些 mud 是有小地圖的功能，應該是 host 傳送過來更新的，這功能需要深入研究 mud 的資料傳送規則。
+
 ## License
 
 - [MIT](https://github.com/griiid/PyMudClient/blob/master/LICENSE)
```

### Comparing `pymudclient-0.3.0/pymudclient/mud.py` & `pymudclient-0.4.0/pymudclient/mud.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,14 +51,17 @@
         thread_list.append((thread, func.__name__))
         thread.start()
 
     return thread_list
 
 
 def thread_wait_close(thread_list):
+    if not thread_list:
+        return
+
     color_print(f'$HIY$等待 {len(thread_list)} 個 thread 關閉...$NOR$')
     for thread, name in thread_list:
         thread.join()
         color_print(f'$CYN${name}$NOR$ 已關閉')
     thread_list.clear()
```

### Comparing `pymudclient-0.3.0/pymudclient/recv.py` & `pymudclient-0.4.0/pymudclient/recv.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,19 +31,19 @@
     content_text_only = ansi_escape.sub('', content).lstrip('> ').rstrip()
 
     for trigger in trigger_list:
         match = re.search(trigger.pattern, content_text_only)
         if not match:
             continue
 
-        if trigger.data:
+        if trigger.data is not None:
             send_to_host(trigger.data, display=False)
-        elif trigger.func:
+        elif trigger.func is not None:
             data = trigger.func(match.groups())
-            if data:
+            if data is not None:
                 send_to_host(data, display=False)
 
 
 IGNORE_LINES = []
 
 
 def thread_job_recv(trigger_list):
```

### Comparing `pymudclient-0.3.0/pymudclient/shared_data.py` & `pymudclient-0.4.0/pymudclient/shared_data.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.3.0/pymudclient/tmp.py` & `pymudclient-0.4.0/pymudclient/tmp.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,12 @@
+#ref: https://github.com/thomasballinger/curtsies/blob/master/curtsies/input.py
+
 import atexit
+import fcntl
+import os
 import sys
 import termios
 import time
 import tty
 
 
 def _get_reset_tc_attr_function(fd, attr_origin):
@@ -16,16 +20,24 @@
 
     # Get origin tty control I/O attributes
     attr_origin = termios.tcgetattr(fd)
 
     atexit.register(_get_reset_tc_attr_function(fd, attr_origin))
 
     try:
-        # Use raw terminal mode
+        # Use raw terminal mode, therefore we can get ctrl-c, ctrl-z
         tty.setraw(fd, termios.TCSANOW)
+
+        attr_new = termios.tcgetattr(fd)
+        attr_new[3] &= ~termios.ECHO & ~termios.ICANON
+        if sys.platform == 'darwin':
+            VDSUSP = termios.VSUSP + 1
+            attr_new[-1][VDSUSP] = 0
+        termios.tcsetattr(fd, termios.TCSANOW, attr_new)
+
         return sys.stdin.read(1)
     except BlockingIOError:
         return None
     except Exception:
         return None
     finally:
         # fcntl.fcntl(fd, fcntl.F_SETFL, orig_fl)
@@ -33,13 +45,14 @@
 
 
 if __name__ == '__main__':
     while True:
         # ch = Nonblocking.read()
         ch = getch()
         if not ch:
+            print('.')
             time.sleep(0.01)
             continue
 
         print(repr(ch))
         if ch == 'q':
             break
```

### Comparing `pymudclient-0.3.0/pymudclient/utils/colors.py` & `pymudclient-0.4.0/pymudclient/utils/colors.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.3.0/pymudclient/utils/print.py` & `pymudclient-0.4.0/pymudclient/utils/print.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,51 @@
+import fcntl
+import os
 import sys
 
 from ..shared_data import g_input
 from .codec import enc
 from .colors import color_convert
 
 # ANSI Escape Code: https://gist.github.com/fnky/458719343aabd01cfb17a3a4f7296797
 
 
+class UnblockTTY:
+
+    def __enter__(self):
+        self.fd = sys.stdin.fileno()
+        self.flags_save = fcntl.fcntl(self.fd, fcntl.F_GETFL)
+        flags = self.flags_save & ~os.O_NONBLOCK
+        fcntl.fcntl(self.fd, fcntl.F_SETFL, flags)
+
+    def __exit__(self, *args):
+        fcntl.fcntl(self.fd, fcntl.F_SETFL, self.flags_save)
+
+
+def _unblock_print(*args, **kwargs):
+    with UnblockTTY():
+        print(*args, **kwargs)
+
+
 def _set_end(kwargs):
     if 'end' not in kwargs:
         kwargs['end'] = '\r\n'
 
 
 def color_print(text, *args, **kwargs):
     text = color_convert(text)
     _set_end(kwargs)
-    print(text, *args, **kwargs)
+    _unblock_print(text, *args, **kwargs)
 
 
 def replace_line_print(text, color=True, *args, **kwargs):
     if color:
         color_print(f'\x1B[2K\r{text}\x1B[m', *args, **kwargs)
     else:
-        print(f'\x1B[2K\r{text}\x1B[m', *args, **kwargs)
+        _unblock_print(f'\x1B[2K\r{text}\x1B[m', *args, **kwargs)
 
 
 def move_cursor_to_index():
     if g_input['input_index'] <= 0:
         return
 
     cursor_pos = len(enc(g_input['input'][:g_input['input_index']]))
```

### Comparing `pymudclient-0.3.0/pymudclient.egg-info/PKG-INFO` & `pymudclient-0.4.0/pymudclient.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymudclient
-Version: 0.3.0
+Version: 0.4.0
 Summary: A MUD client core written in Python
 Home-page: https://github.com/griiid/PyMudClient
 Download-URL: https://pypi.org/project/pymudclient/
 Author: griiid
 Author-email: gridwing@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
@@ -29,26 +29,28 @@
 
 - [PyMudClient: 用 Python 開發的 MUD Client 核心](#pymudclient-用-python-開發的-mud-client-核心)
   - [這是什麼？](#這是什麼)
   - [已測試過環境](#已測試過環境)
   - [支援功能](#支援功能)
   - [安裝](#安裝)
   - [使用範例](#使用範例)
-  - [功能說明](#功能說明)
+  - [輸入介面](#輸入介面)
+  - [API Reference](#api-reference)
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
+  - [尚未實作功能](#尚未實作功能)
   - [License](#license)
 
 ## 已測試過環境
 
 - macOS Ventura 13.3.1 (a)
 - GNU/Linux 5.15.0-1032-raspi aarch64
 
@@ -82,15 +84,24 @@
     PORT,
     alias_list=ALIAS_LIST,
     trigger_list=TRIGGER_LIST,
     timer_list=TIMER_LIST,
 )
 ```
 
-## 功能說明
+## 輸入介面
+
+- 輸入的文字會固定出現在最後一行。
+- 可使用 左/右/Home/End 移動位置。
+- 可使用 Backspace/Ctrl-H 刪除游標位置前面的字元。
+- 可使用 Delete 刪除游標位置後面的字元。
+- 可使用 Ctrl-W 刪除前面一個 word (仿照 vim 功能)。
+- 按下 Enter 送出後，會記住最後一次送出的文字，可以進行編輯，或直接按 Enter 再送一次。
+
+## API Reference
 
 ### run
 
 - 連線至 `<host>:<port>`
 
 ```py
 run(host, port, alias_list=None, trigger_list=None, timer_list=None)
@@ -174,10 +185,15 @@
 
 - 每 900 秒傳送一個 `save` 到 host。
 
 ## 已知問題
 
 - 目前沒有。
 
+## 尚未實作功能
+
+- 輸入功能的歷史紀錄，可按 上/下 選擇過去送出過的文字。
+- 有看過有些 mud 是有小地圖的功能，應該是 host 傳送過來更新的，這功能需要深入研究 mud 的資料傳送規則。
+
 ## License
 
 - [MIT](https://github.com/griiid/PyMudClient/blob/master/LICENSE)
```

### Comparing `pymudclient-0.3.0/pymudclient.egg-info/SOURCES.txt` & `pymudclient-0.4.0/pymudclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymudclient-0.3.0/pyproject.toml` & `pymudclient-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymudclient-0.3.0/setup.py` & `pymudclient-0.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 PACKAGE_NAME = 'pymudclient'
 AUTHOR = 'griiid'
 AUTHOR_EMAIL = 'gridwing@gmail.com'
 URL = 'https://github.com/griiid/PyMudClient'
 DOWNLOAD_URL = 'https://pypi.org/project/pymudclient/'
 
 LICENSE = 'MIT'
-VERSION = '0.3.0'
+VERSION = '0.4.0'
 DESCRIPTION = 'A MUD client core written in Python'
 LONG_DESCRIPTION = (HERE  / 'README.md').read_text(encoding='utf8')
 LONG_DESC_TYPE = 'text/markdown'
 
 requirements = (HERE / 'requirements.txt').read_text(encoding='utf8')
 INSTALL_REQUIRES = [s.strip() for s in requirements.split('\n')]
```

