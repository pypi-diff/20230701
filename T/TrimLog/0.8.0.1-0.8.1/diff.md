# Comparing `tmp/TrimLog-0.8.0.1.tar.gz` & `tmp/TrimLog-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TrimLog-0.8.0.1.tar", last modified: Sun Jun 18 14:13:21 2023, max compression
+gzip compressed data, was "TrimLog-0.8.1.tar", last modified: Sat Jul  1 14:34:32 2023, max compression
```

## Comparing `TrimLog-0.8.0.1.tar` & `TrimLog-0.8.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 14:13:21.619547 TrimLog-0.8.0.1/
--rw-rw-rw-   0        0        0    11386 2023-01-27 04:01:21.000000 TrimLog-0.8.0.1/LICENSE
--rw-rw-rw-   0        0        0     2617 2023-06-18 14:13:21.618551 TrimLog-0.8.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1606 2023-06-18 14:13:10.000000 TrimLog-0.8.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 14:13:21.603600 TrimLog-0.8.0.1/TrimLog/
--rw-rw-rw-   0        0        0     1298 2023-06-18 14:10:17.000000 TrimLog-0.8.0.1/TrimLog/__init__.py
--rw-rw-rw-   0        0        0      276 2023-02-02 05:01:04.000000 TrimLog-0.8.0.1/TrimLog/exceptions.py
--rw-rw-rw-   0        0        0     2433 2023-02-02 06:39:46.000000 TrimLog-0.8.0.1/TrimLog/logger_constants.py
--rw-rw-rw-   0        0        0    29545 2023-06-18 14:10:17.000000 TrimLog-0.8.0.1/TrimLog/logger_main.py
--rw-rw-rw-   0        0        0     2135 2023-02-03 07:05:46.000000 TrimLog-0.8.0.1/TrimLog/object_constants.py
--rw-rw-rw-   0        0        0     8463 2023-06-18 11:36:28.000000 TrimLog-0.8.0.1/TrimLog/pip_manager.py
--rw-rw-rw-   0        0        0     3771 2023-04-21 13:02:38.000000 TrimLog-0.8.0.1/TrimLog/test.py
-drwxrwxrwx   0        0        0        0 2023-06-18 14:13:21.616557 TrimLog-0.8.0.1/TrimLog.egg-info/
--rw-rw-rw-   0        0        0     2617 2023-06-18 14:13:21.000000 TrimLog-0.8.0.1/TrimLog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-06-18 14:13:21.000000 TrimLog-0.8.0.1/TrimLog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 14:13:21.000000 TrimLog-0.8.0.1/TrimLog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-18 14:13:21.000000 TrimLog-0.8.0.1/TrimLog.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-18 14:13:21.000000 TrimLog-0.8.0.1/TrimLog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 14:13:21.619547 TrimLog-0.8.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1549 2023-06-18 11:36:28.000000 TrimLog-0.8.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 14:34:32.797660 TrimLog-0.8.1/
+-rw-rw-rw-   0        0        0    11386 2023-01-27 04:01:21.000000 TrimLog-0.8.1/LICENSE
+-rw-rw-rw-   0        0        0     2615 2023-07-01 14:34:32.796663 TrimLog-0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1606 2023-06-18 14:13:10.000000 TrimLog-0.8.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 14:34:32.782712 TrimLog-0.8.1/TrimLog/
+-rw-rw-rw-   0        0        0     1296 2023-07-01 14:34:05.000000 TrimLog-0.8.1/TrimLog/__init__.py
+-rw-rw-rw-   0        0        0      276 2023-02-02 05:01:04.000000 TrimLog-0.8.1/TrimLog/exceptions.py
+-rw-rw-rw-   0        0        0     2433 2023-02-02 06:39:46.000000 TrimLog-0.8.1/TrimLog/logger_constants.py
+-rw-rw-rw-   0        0        0    29579 2023-07-01 14:34:05.000000 TrimLog-0.8.1/TrimLog/logger_main.py
+-rw-rw-rw-   0        0        0     2135 2023-02-03 07:05:46.000000 TrimLog-0.8.1/TrimLog/object_constants.py
+-rw-rw-rw-   0        0        0     8747 2023-07-01 14:34:05.000000 TrimLog-0.8.1/TrimLog/pip_manager.py
+-rw-rw-rw-   0        0        0     3771 2023-04-21 13:02:38.000000 TrimLog-0.8.1/TrimLog/test.py
+drwxrwxrwx   0        0        0        0 2023-07-01 14:34:32.795667 TrimLog-0.8.1/TrimLog.egg-info/
+-rw-rw-rw-   0        0        0     2615 2023-07-01 14:34:32.000000 TrimLog-0.8.1/TrimLog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-07-01 14:34:32.000000 TrimLog-0.8.1/TrimLog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 14:34:32.000000 TrimLog-0.8.1/TrimLog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-01 14:34:32.000000 TrimLog-0.8.1/TrimLog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-01 14:34:32.000000 TrimLog-0.8.1/TrimLog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 14:34:32.797660 TrimLog-0.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     1549 2023-06-18 11:36:28.000000 TrimLog-0.8.1/setup.py
```

### Comparing `TrimLog-0.8.0.1/LICENSE` & `TrimLog-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TrimLog-0.8.0.1/PKG-INFO` & `TrimLog-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrimLog
-Version: 0.8.0.1
+Version: 0.8.1
 Summary: TriMO组织的python项目log和项目管理框架库。
 Home-page: https://github.com/TriM-Organization/TrimLog
 Author: FedDragon1, Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `TrimLog-0.8.0.1/README.md` & `TrimLog-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `TrimLog-0.8.0.1/TrimLog/__init__.py` & `TrimLog-0.8.1/TrimLog/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
    You may obtain a copy of the License at
 
        https://www.apache.org/licenses/LICENSE-2.0
 """
 
 from .logger_main import *
 
-__version__: str = "v0.8.0.1"
+__version__: str = "v0.8.1"
 
 set_version(__version__)
 
 
 def get_version() -> str:
     """获取版本号"""
     return __version__
```

### Comparing `TrimLog-0.8.0.1/TrimLog/logger_constants.py` & `TrimLog-0.8.1/TrimLog/logger_constants.py`

 * *Files identical despite different names*

### Comparing `TrimLog-0.8.0.1/TrimLog/logger_main.py` & `TrimLog-0.8.1/TrimLog/logger_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from __future__ import annotations
 
 import atexit
 import platform
 import time
 
 from types import TracebackType
-from typing import Literal, Optional, Type, TypeVar
+from typing import Literal, Optional, Type, TypeVar, Union
 
 import rich.traceback
 from rich.console import Console
 from rich.traceback import Traceback
 
 from .logger_constants import *
 from .object_constants import *
@@ -55,15 +55,15 @@
 
 
 class Logger:
     """
     main logger class.
     """
 
-    instance: Logger = None
+    instance: Optional[Logger] = None
     """
     Logger.instance: used to get value for static method
     """
 
     str_start_time: str = time.strftime("%Y-%m-%d %H_%M_%S")
 
     console: Console = Console()
@@ -197,17 +197,17 @@
             self.headline_shower()
 
     def log(
         self,
         info: T,
         level: L,
         mandatory_use: bool = False,
-        frame_file: str = None,
-        frame_name: str = None,
-        frame_lineno: int = None,
+        frame_file: Optional[str] = None,
+        frame_name: Optional[str] = None,
+        frame_lineno: Optional[int] = None,
     ) -> T:
         """
         log output base function.
         :param info: things you want to output.
         :param level: the log output level.
         :param mandatory_use: allow to use this function while "self.is_logging" is False.
         :param frame_file: initiation program's file name.
@@ -228,15 +228,15 @@
             length = 12 + style_len
 
             # 获取目前log的输出权重
             level_weight = WEIGHT_ORDER.get(level)
 
             # 获取log前面输出的执行代码位置信息
             if self.show_position:
-                if frame_lineno is None and frame_name is None and frame_file is None:
+                if not (frame_lineno and frame_name and frame_file):
                     back_frame = sys._getframe().f_back
                     frame_file: str = os.path.basename(back_frame.f_code.co_filename)
                     frame_name: str = back_frame.f_code.co_name
                     frame_lineno: int = back_frame.f_lineno
 
                 end_with = "{0}-{1}: {2}\n".format(
                     frame_file, frame_name, str(frame_lineno)
@@ -736,15 +736,15 @@
         pip_list = "Amount is bigger than default, so there's no output."
 
     # 判断是否需要检查pip安装
     if pip_manage.is_detect_pip:
         if pip_manage.pip_detect() is True:
             pip_check = "All lib is already done."
         else:
-            pip_check = pip_manage.pip_detect()
+            pip_check = str(pip_manage.pip_detect())
     else:
         pip_check = "Don't use pip check."
 
     # 判断是否需要安装未安装的pip包
     if pip_manage.is_install_pip:
         if pip_manage.pip_install() is True and pip_manage.pip_detect() is not True:
             logger.info(
```

### Comparing `TrimLog-0.8.0.1/TrimLog/object_constants.py` & `TrimLog-0.8.1/TrimLog/object_constants.py`

 * *Files identical despite different names*

### Comparing `TrimLog-0.8.0.1/TrimLog/pip_manager.py` & `TrimLog-0.8.1/TrimLog/pip_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
        https://www.apache.org/licenses/LICENSE-2.0
 
 pip管理类开发者：bgArray
 """
 
 import os
 import sys
-from typing import Dict, List, Tuple, Union
+from typing import Dict, List, Tuple, Union, Literal,Generator
 
 import pkg_resources
 
 from .exceptions import *
 
 
 # Pip method
@@ -137,16 +137,16 @@
                     continue
                 return_list.append({"need": str(i), "have": None})
             self.detect_report = return_list
             return return_list
 
     def detecting_setting(
         self,
-        requirements_list: List[pkg_resources.Requirement.parse] = None,
-        requirements_path: str = None,
+        requirements_list: Union[List[pkg_resources.Requirement], None] = None,
+        requirements_path: Union[str, None] = None,
     ) -> None:
         """
         设置要检测的对象，注意两个参数填一个且只有一个就好，建议使用path
         :param requirements_list: 传入[Requirement.parse('matplotlib'), Requirement.parse('mido')]这样的列表
         :param requirements_path: 传入requirements.txt的路径即可
         :return: None
         """
@@ -185,24 +185,28 @@
     @staticmethod
     def open_req(path: str) -> str:
         """
         打开requirements.txt
         :param path: requirements.txt path
         :return: str: thing
         """
+
+        # 这里建议用 chardet 判断编码，不然容易空
+        # https://github.com/chardet/chardet
+        req_str = ""
         try:
-            f = open(path, mode="r", encoding="utf-16")
-            return f.read(-1)
+            req_str = open(path, mode="r", encoding="utf-16").read(-1)
         except UnicodeError as e:
-            f.close()
-            if str(e) == "UTF-16 stream does not start with BOM":
-                f = open(path, mode="r", encoding="utf-8")
-                return f.read(-1)
-        finally:
-            f.close()
+
+            if e.args[-1] == "UTF-16 stream does not start with BOM":
+                req_str = open(path, mode="r", encoding="utf-8-sig").read(-1)
+            elif e.args[-1] == "truncated data":
+                req_str = open(path, mode="r", encoding="utf-8").read(-1)
+        
+        return req_str
 
     def pip_install(self) -> bool:
         """
         根据self.detect_report安装库
         :return: True/False 表示是否全部安装正确
         """
         if self.is_install_pip:
@@ -216,7 +220,9 @@
                     "pip install " if sys.platform == "win32" else "pip3 install "
                 ) + " ".join(libs_in_need)
                 os.system(command)
             if self.pip_detect():
                 return True
             else:
                 return False
+        else:
+            return True
```

### Comparing `TrimLog-0.8.0.1/TrimLog/test.py` & `TrimLog-0.8.1/TrimLog/test.py`

 * *Files identical despite different names*

### Comparing `TrimLog-0.8.0.1/TrimLog.egg-info/PKG-INFO` & `TrimLog-0.8.1/TrimLog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrimLog
-Version: 0.8.0.1
+Version: 0.8.1
 Summary: TriMO组织的python项目log和项目管理框架库。
 Home-page: https://github.com/TriM-Organization/TrimLog
 Author: FedDragon1, Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `TrimLog-0.8.0.1/setup.py` & `TrimLog-0.8.1/setup.py`

 * *Files identical despite different names*

