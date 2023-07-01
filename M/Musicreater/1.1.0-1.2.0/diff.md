# Comparing `tmp/Musicreater-1.1.0.tar.gz` & `tmp/Musicreater-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Musicreater-1.1.0.tar", last modified: Sun Jun  4 13:34:27 2023, max compression
+gzip compressed data, was "Musicreater-1.2.0.tar", last modified: Sat Jul  1 13:54:25 2023, max compression
```

## Comparing `Musicreater-1.1.0.tar` & `Musicreater-1.2.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 13:34:27.370883 Musicreater-1.1.0/
--rw-rw-rw-   0        0        0    13072 2023-05-27 11:45:04.000000 Musicreater-1.1.0/LICENSE.md
-drwxrwxrwx   0        0        0        0 2023-06-04 13:34:27.295138 Musicreater-1.1.0/Musicreater/
--rw-rw-rw-   0        0        0      825 2023-06-04 13:30:48.000000 Musicreater-1.1.0/Musicreater/__init__.py
--rw-rw-rw-   0        0        0     6525 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/constants.py
--rw-rw-rw-   0        0        0     2903 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/exceptions.py
--rw-rw-rw-   0        0        0     6961 2023-06-04 13:30:48.000000 Musicreater-1.1.0/Musicreater/experiment.py
--rw-rw-rw-   0        0        0    10301 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/magicmain.py
--rw-rw-rw-   0        0        0    31166 2023-06-04 13:30:48.000000 Musicreater-1.1.0/Musicreater/main.py
-drwxrwxrwx   0        0        0        0 2023-06-04 13:34:27.334006 Musicreater-1.1.0/Musicreater/plugin/
--rw-rw-rw-   0        0        0      559 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/plugin/__init__.py
--rw-rw-rw-   0        0        0     2112 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/plugin/archive.py
--rw-rw-rw-   0        0        0     5999 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/plugin/bdx.py
-drwxrwxrwx   0        0        0        0 2023-06-04 13:34:27.338991 Musicreater-1.1.0/Musicreater/plugin/bdxfile/
--rw-rw-rw-   0        0        0      513 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/plugin/bdxfile/__init__.py
--rw-rw-rw-   0        0        0     6194 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/plugin/bdxfile/main.py
--rw-rw-rw-   0        0        0      809 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/plugin/common.py
-drwxrwxrwx   0        0        0        0 2023-06-04 13:34:27.344969 Musicreater-1.1.0/Musicreater/plugin/funcpack/
--rw-rw-rw-   0        0        0      513 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/plugin/funcpack/__init__.py
--rw-rw-rw-   0        0        0     3896 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/plugin/funcpack/main.py
--rw-rw-rw-   0        0        0     2492 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/plugin/main.py
-drwxrwxrwx   0        0        0        0 2023-06-04 13:34:27.350951 Musicreater-1.1.0/Musicreater/plugin/mcstructfile/
--rw-rw-rw-   0        0        0      521 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/plugin/mcstructfile/__init__.py
--rw-rw-rw-   0        0        0     1941 2023-06-04 13:30:48.000000 Musicreater-1.1.0/Musicreater/plugin/mcstructfile/main.py
-drwxrwxrwx   0        0        0        0 2023-06-04 13:34:27.356930 Musicreater-1.1.0/Musicreater/plugin/mcstructpack/
--rw-rw-rw-   0        0        0      513 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/plugin/mcstructpack/__init__.py
--rw-rw-rw-   0        0        0     6242 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/plugin/mcstructpack/main.py
--rw-rw-rw-   0        0        0     7153 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/plugin/mcstructure.py
--rw-rw-rw-   0        0        0     3797 2023-06-04 13:30:48.000000 Musicreater-1.1.0/Musicreater/plugin/noteblock.py
-drwxrwxrwx   0        0        0        0 2023-06-04 13:34:27.364904 Musicreater-1.1.0/Musicreater/plugin/websocket/
--rw-rw-rw-   0        0        0      522 2023-06-04 13:30:48.000000 Musicreater-1.1.0/Musicreater/plugin/websocket/__init__.py
--rw-rw-rw-   0        0        0      771 2023-06-04 13:30:48.000000 Musicreater-1.1.0/Musicreater/plugin/websocket/main.py
--rw-rw-rw-   0        0        0     1168 2023-06-04 13:30:48.000000 Musicreater-1.1.0/Musicreater/plugin/websocket.py
--rw-rw-rw-   0        0        0     4535 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/subclass.py
--rw-rw-rw-   0        0        0      848 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-04 13:34:27.310087 Musicreater-1.1.0/Musicreater.egg-info/
--rw-rw-rw-   0        0        0     7816 2023-06-04 13:34:26.000000 Musicreater-1.1.0/Musicreater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1031 2023-06-04 13:34:27.000000 Musicreater-1.1.0/Musicreater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 13:34:26.000000 Musicreater-1.1.0/Musicreater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-06-04 13:34:26.000000 Musicreater-1.1.0/Musicreater.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-04 13:34:26.000000 Musicreater-1.1.0/Musicreater.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7816 2023-06-04 13:34:27.369886 Musicreater-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     6747 2023-05-27 11:45:04.000000 Musicreater-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-04 13:34:27.370883 Musicreater-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1597 2023-05-27 11:45:04.000000 Musicreater-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 13:54:25.697469 Musicreater-1.2.0/
+-rw-rw-rw-   0        0        0    13072 2023-07-01 13:48:04.000000 Musicreater-1.2.0/LICENSE.md
+drwxrwxrwx   0        0        0        0 2023-07-01 13:54:25.649052 Musicreater-1.2.0/Musicreater/
+-rw-rw-rw-   0        0        0      991 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/__init__.py
+-rw-rw-rw-   0        0        0     6525 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/constants.py
+-rw-rw-rw-   0        0        0     3142 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/exceptions.py
+-rw-rw-rw-   0        0        0    18362 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/experiment.py
+-rw-rw-rw-   0        0        0    10301 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/magicmain.py
+-rw-rw-rw-   0        0        0    28535 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/main.py
+drwxrwxrwx   0        0        0        0 2023-07-01 13:54:25.676538 Musicreater-1.2.0/Musicreater/plugin/
+-rw-rw-rw-   0        0        0      581 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/__init__.py
+-rw-rw-rw-   0        0        0     2435 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/archive.py
+-rw-rw-rw-   0        0        0     5999 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/bdx.py
+drwxrwxrwx   0        0        0        0 2023-07-01 13:54:25.679528 Musicreater-1.2.0/Musicreater/plugin/bdxfile/
+-rw-rw-rw-   0        0        0      569 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/bdxfile/__init__.py
+-rw-rw-rw-   0        0        0     6211 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/bdxfile/main.py
+-rw-rw-rw-   0        0        0      809 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/common.py
+drwxrwxrwx   0        0        0        0 2023-07-01 13:54:25.683513 Musicreater-1.2.0/Musicreater/plugin/funcpack/
+-rw-rw-rw-   0        0        0      547 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/funcpack/__init__.py
+-rw-rw-rw-   0        0        0     4182 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/funcpack/main.py
+-rw-rw-rw-   0        0        0     2523 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/main.py
+drwxrwxrwx   0        0        0        0 2023-07-01 13:54:25.687500 Musicreater-1.2.0/Musicreater/plugin/mcstructfile/
+-rw-rw-rw-   0        0        0      557 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/mcstructfile/__init__.py
+-rw-rw-rw-   0        0        0     1943 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/mcstructfile/main.py
+drwxrwxrwx   0        0        0        0 2023-07-01 13:54:25.691488 Musicreater-1.2.0/Musicreater/plugin/mcstructpack/
+-rw-rw-rw-   0        0        0      550 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/mcstructpack/__init__.py
+-rw-rw-rw-   0        0        0     6253 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/mcstructpack/main.py
+-rw-rw-rw-   0        0        0     7219 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/mcstructure.py
+-rw-rw-rw-   0        0        0     3797 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/noteblock.py
+drwxrwxrwx   0        0        0        0 2023-07-01 13:54:25.694483 Musicreater-1.2.0/Musicreater/plugin/websocket/
+-rw-rw-rw-   0        0        0      522 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/websocket/__init__.py
+-rw-rw-rw-   0        0        0      771 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/websocket/main.py
+-rw-rw-rw-   0        0        0     1168 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/websocket.py
+-rw-rw-rw-   0        0        0    13264 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/previous.py
+-rw-rw-rw-   0        0        0     4238 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/subclass.py
+-rw-rw-rw-   0        0        0     1125 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-01 13:54:25.659595 Musicreater-1.2.0/Musicreater.egg-info/
+-rw-rw-rw-   0        0        0     7718 2023-07-01 13:54:25.000000 Musicreater-1.2.0/Musicreater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1055 2023-07-01 13:54:25.000000 Musicreater-1.2.0/Musicreater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 13:54:25.000000 Musicreater-1.2.0/Musicreater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-07-01 13:54:25.000000 Musicreater-1.2.0/Musicreater.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-01 13:54:25.000000 Musicreater-1.2.0/Musicreater.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7718 2023-07-01 13:54:25.696478 Musicreater-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6842 2023-07-01 13:48:04.000000 Musicreater-1.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-01 13:54:25.697469 Musicreater-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1600 2023-07-01 13:48:04.000000 Musicreater-1.2.0/setup.py
```

### Comparing `Musicreater-1.1.0/LICENSE.md` & `Musicreater-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Musicreater-1.1.0/Musicreater/__init__.py` & `Musicreater-1.2.0/Musicreater/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,12 +13,20 @@
 """
 
 # 睿穆组织 开发交流群 861684859
 # Email TriM-Organization@hotmail.com
 # 若需转载或借鉴 许可声明请查看仓库目录下的 License.md
 
 
-__version__ = "1.1.0"
-__all__ = []
+__version__ = "1.2.0"
+__vername__ = "更高效的算法管理"
 __author__ = (("金羿", "Eilles Wan"), ("诸葛亮与八卦阵", "bgArray"), ("鸣凤鸽子", "MingFengPigeon"))
+__all__ = [
+    # 主要类
+    "MidiConvert",
+    # 附加类
+    # "SingleNote",
+    "SingleCommand",
+    # "TimeStamp", 未来功能
+]
 
 from .main import *
```

### Comparing `Musicreater-1.1.0/Musicreater/constants.py` & `Musicreater-1.2.0/Musicreater/constants.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.1.0/Musicreater/exceptions.py` & `Musicreater-1.2.0/Musicreater/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,25 +13,23 @@
 """
 
 # 睿穆组织 开发交流群 861684859
 # Email TriM-Organization@hotmail.com
 # 若需转载或借鉴 许可声明请查看仓库目录下的 License.md
 
 
-
-
 class MSCTBaseException(Exception):
     """音·创库版本的所有错误均继承于此"""
 
     def __init__(self, *args):
         """音·创库版本的所有错误均继承于此"""
         super().__init__(*args)
 
     def miao(
-            self,
+        self,
     ):
         for i in self.args:
             print(i + "喵！")
 
     def crash_it(self):
         raise self
 
@@ -48,14 +46,22 @@
     """Midi文件损坏"""
 
     def __init__(self, *args):
         """Midi文件损坏"""
         super().__init__("MIDI文件损坏：无法读取MIDI文件", *args)
 
 
+class MidiUnboundError(MSCTBaseException):
+    """未定义Midi对象"""
+
+    def __init__(self, *args):
+        """未绑定Midi对象"""
+        super().__init__("未定义MidiFile对象：你甚至没有对象就想要生孩子？", *args)
+
+
 class CommandFormatError(RuntimeError):
     """指令格式与目标格式不匹配而引起的错误"""
 
     def __init__(self, *args):
         """指令格式与目标格式不匹配而引起的错误"""
         super().__init__("指令格式不匹配", *args)
```

### Comparing `Musicreater-1.1.0/Musicreater/magicmain.py` & `Musicreater-1.2.0/Musicreater/magicmain.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.1.0/Musicreater/main.py` & `Musicreater-1.2.0/Musicreater/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,30 +15,56 @@
 """
 
 # 音·创 开发交流群 861684859
 # Email TriM-Organization@hotmail.com
 # 若需转载或借鉴 许可声明请查看仓库根目录下的 License.md
 
 
-import os
+# BUG退散！BUG退散！                    BUG退散！BUG退散！
+# 异常、错误作乱之时                     異常、誤りが、困った時は
+# 二六字组！万国码合！二六字组！万国码合！   グループ！コード＃！グループ！コード＃！
+# 赶快呼叫 程序员！Let's Go！            直ぐに呼びましょプログラマ レッツゴー！
+
+
+
 import math
-from typing import Tuple, List, Union
+import os
+from typing import List, Literal, Tuple, Union
 
 import mido
 
-from .exceptions import *
 from .constants import *
-from .utils import *
+from .exceptions import *
 from .subclass import *
+from .utils import *
 
-VM = TypeVar("VM", mido.MidiFile, None)  # void mido
+VoidMido = Union[mido.MidiFile, None]  # void mido
 """
 空Midi类类型
 """
 
+ChannelType = Dict[
+    int,
+    Dict[
+        int,
+        List[
+            Union[
+                Tuple[Literal["PgmC"], int, int],
+                Tuple[Literal["NoteS"], int, int, int],
+                Tuple[Literal["NoteE"], int, int],
+            ]
+        ],
+    ],
+]
+"""
+以字典所标记的频道信息类型
+
+Dict[int,Dict[int,List[Union[Tuple[Literal["PgmC"], int, int],Tuple[Literal["NoteS"], int, int, int],Tuple[Literal["NoteE"], int, int],]],],]
+"""
+
 """
 学习笔记：
 tempo:  microseconds per quarter note 毫秒每四分音符，换句话说就是一拍占多少毫秒
 tick:  midi帧
 ticks_per_beat:  帧每拍，即一拍多少帧
 
 那么：
@@ -71,41 +97,41 @@
 
 @dataclass(init=False)
 class MidiConvert:
     """
     将Midi文件转换为我的世界内容
     """
 
-    midi: VM
+    midi: VoidMido
     """MidiFile对象"""
 
     midi_music_name: str
     """Midi乐曲名"""
 
     enable_old_exe_format: bool
     """是否启用旧版execute指令格式"""
 
     execute_cmd_head: str
     """execute指令头部"""
 
-    channels: Dict[int, Dict[int, List[Tuple[str, int, int, Union[None, int]]]]]
+    channels: ChannelType
     """频道信息字典"""
 
     music_command_list: List[SingleCommand]
     """音乐指令列表"""
 
     music_tick_num: int
     """音乐总延迟"""
 
     progress_bar_command: List[SingleCommand]
     """进度条指令列表"""
 
     def __init__(
         self,
-        midi_obj: VM,
+        midi_obj: VoidMido,
         midi_name: str,
         enable_old_exe_format: bool = False,
     ):
         """
         简单的midi转换类，将midi对象转换为我的世界结构或者包
 
         Parameters
@@ -114,15 +140,15 @@
             需要处理的midi对象
         midi_name: MIDI乐曲名称
             此音乐之名
         enable_old_exe_format: bool
             是否启用旧版(≤1.19)指令格式，默认为否
         """
 
-        self.midi: VM = midi_obj
+        self.midi: VoidMido = midi_obj
 
         self.midi_music_name: str = midi_name
 
         self.enable_old_exe_format: bool = enable_old_exe_format
 
         self.execute_cmd_head = (
             "execute {} ~ ~ ~ "
@@ -147,15 +173,17 @@
         ----------
         midi_file: str
             midi文件地址
         enable_old_exe_format: bool
             是否启用旧版(≤1.19)指令格式，默认为否
         """
 
-        midi_music_name = os.path.splitext(os.path.basename(midi_file_path))[0].replace(' ','_')
+        midi_music_name = os.path.splitext(os.path.basename(midi_file_path))[0].replace(
+            " ", "_"
+        )
         """文件名，不含路径且不含后缀"""
 
         try:
             return cls(mido.MidiFile(midi_file_path), midi_music_name, old_exe_format)
         except (ValueError, TypeError) as E:
             raise MidiDestroyedError(f"文件{midi_file_path}损坏：{E}")
         except FileNotFoundError as E:
@@ -487,90 +515,89 @@
             )
 
         self.progress_bar_command = result
         return result
 
     def to_music_channels(
         self,
-    ) -> Dict[int, Dict[int, List[Tuple[str, int, int, Union[None, int]]]]]:
+    ) -> ChannelType:
         """
-        使用金羿的转换思路，将midi解析并转换为频道信息
+        使用金羿的转换思路，将midi解析并转换为频道信息字典
 
         Returns
         -------
-        Dict[int, Dict[int, List[Tuple[str,int,int,Union[None,int]]]]]
+        以频道作为分割的Midi信息字典:
+        Dict[int,Dict[int,List[Union[Tuple[Literal["PgmC"], int, int],Tuple[Literal["NoteS"], int, int, int],Tuple[Literal["NoteE"], int, int],]],],]
         """
+        if self.midi is None:
+            raise MidiUnboundError(
+                "你是否正在使用的是一个由 copy_important 生成的MidiConvert对象？这是不可复用的。"
+            )
 
         # 一个midi中仅有16个通道 我们通过通道来识别而不是音轨
-        midi_channels = empty_midi_channels()
+        midi_channels: ChannelType = empty_midi_channels()
+        tempo = mido.midifiles.midifiles.DEFAULT_TEMPO
 
+        # a = 0
         # 我们来用通道统计音乐信息
         # 但是是用分轨的思路的
         for track_no, track in enumerate(self.midi.tracks):
+            # print(track_no,track)
             microseconds = 0
+            if not track:
+                continue
 
+            # print(track_no,"="*20)
             for msg in track:
+                # print("+++",msg)
                 if msg.time != 0:
-                    try:
-                        microseconds += (
-                            msg.time * tempo / self.midi.ticks_per_beat / 1000
-                        )
-                        # print(microseconds)
-                    except NameError:
-                        # raise NotDefineTempoError("计算当前分数时出错 未定义参量 Tempo")
-                        microseconds += (
-                            msg.time
-                            * mido.midifiles.midifiles.DEFAULT_TEMPO
-                            / self.midi.ticks_per_beat
-                        ) / 1000
+                    microseconds += msg.time * tempo / self.midi.ticks_per_beat / 1000
 
                 if msg.is_meta:
                     if msg.type == "set_tempo":
                         tempo = msg.tempo
                 else:
-                    # 曾用于调试模式
-                    #     try:
-                    #         if msg.channel > 15:
-                    #             raise ChannelOverFlowError(f"当前消息 {msg} 的通道超限(≤15)")
-                    #     except AttributeError:
-                    #         pass
 
                     if not track_no in midi_channels[msg.channel].keys():
                         midi_channels[msg.channel][track_no] = []
                     if msg.type == "program_change":
                         midi_channels[msg.channel][track_no].append(
                             ("PgmC", msg.program, microseconds)
                         )
 
                     elif msg.type == "note_on" and msg.velocity != 0:
                         midi_channels[msg.channel][track_no].append(
                             ("NoteS", msg.note, msg.velocity, microseconds)
                         )
+                        # a+=1
 
                     elif (msg.type == "note_on" and msg.velocity == 0) or (
                         msg.type == "note_off"
                     ):
                         midi_channels[msg.channel][track_no].append(
                             ("NoteE", msg.note, microseconds)
                         )
 
+        # print(a)
+
         """整合后的音乐通道格式
         每个通道包括若干消息元素其中逃不过这三种：
 
         1 切换乐器消息
         ("PgmC", 切换后的乐器ID: int, 距离演奏开始的毫秒)
 
         2 音符开始消息
         ("NoteS", 开始的音符ID, 力度（响度）, 距离演奏开始的毫秒)
 
         3 音符结束消息
-        ("NoteS", 结束的音符ID, 距离演奏开始的毫秒)"""
-
+        ("NoteE", 结束的音符ID, 距离演奏开始的毫秒)"""
+        del tempo, self.channels
         self.channels = midi_channels
-        return self.channels
+        # [print([print(no,tno,sum([True if i[0] == 'NoteS' else False for i in track])) for tno,track in cna.items()]) if cna else False for no,cna in midi_channels.items()]
+        return midi_channels
 
     def to_command_list_in_score(
         self,
         scoreboard_name: str = "mscplay",
         max_volume: float = 1.0,
         speed: float = 1.0,
     ) -> Tuple[List[List[SingleCommand]], int, int]:
@@ -594,14 +621,15 @@
         if speed == 0:
             raise ZeroSpeedError("播放速度仅可为正实数")
         max_volume = 1 if max_volume > 1 else (0.001 if max_volume <= 0 else max_volume)
 
         tracks = []
         cmdAmount = 0
         maxScore = 0
+        InstID = -1
 
         self.to_music_channels()
 
         # 此处 我们把通道视为音轨
         for i in self.channels.keys():
             # 如果当前通道为空 则跳过
             if not self.channels[i]:
@@ -616,53 +644,51 @@
                 nowTrack = []
 
                 for msg in track:
                     if msg[0] == "PgmC":
                         InstID = msg[1]
 
                     elif msg[0] == "NoteS":
-                        try:
-                            soundID, _X = (
-                                self.perc_inst_to_soundID_withX(InstID)
-                                if SpecialBits
-                                else self.inst_to_souldID_withX(InstID)
-                            )
-                        except UnboundLocalError as E:
-                            # raise NotDefineProgramError(f"未定义乐器便提前演奏。\n{E}")
-                            soundID, _X = (
-                                self.perc_inst_to_soundID_withX(-1)
-                                if SpecialBits
-                                else self.inst_to_souldID_withX(-1)
-                            )
+                        soundID, _X = (
+                            self.perc_inst_to_soundID_withX(msg[1])
+                            if SpecialBits
+                            else self.inst_to_souldID_withX(InstID)
+                        )
                         score_now = round(msg[-1] / float(speed) / 50)
                         maxScore = max(maxScore, score_now)
+                        mc_pitch = "" if SpecialBits else 2 ** ((msg[1] - 60 - _X) / 12)
 
                         nowTrack.append(
                             SingleCommand(
                                 self.execute_cmd_head.format(
                                     "@a[scores=({}={})]".format(
                                         scoreboard_name, score_now
                                     )
                                     .replace("(", r"{")
                                     .replace(")", r"}")
                                 )
-                                + f"playsound {soundID} @s ^ ^ ^{1 / max_volume - 1} {msg[2] / 128} "
-                                f"{2 ** ((msg[1] - 60 - _X) / 12)}",
+                                + "playsound {} @s ^ ^ ^{} {} {}".format(
+                                    soundID, 1 / max_volume - 1, msg[2] / 128, mc_pitch
+                                ),
                                 annotation="在{}播放{}%的{}音".format(
-                                    mctick2timestr(score_now), max_volume * 100, ""
+                                    mctick2timestr(score_now),
+                                    max_volume * 100,
+                                    "{}:{}".format(soundID, mc_pitch),
                                 ),
                             ),
                         )
 
                         cmdAmount += 1
 
                 if nowTrack:
                     self.music_command_list.extend(nowTrack)
                     tracks.append(nowTrack)
 
+        # print(cmdAmount)
+        del InstID
         self.music_tick_num = maxScore
         return (tracks, cmdAmount, maxScore)
 
     def to_command_list_in_delay(
         self,
         max_volume: float = 1.0,
         speed: float = 1.0,
@@ -688,14 +714,16 @@
         if speed == 0:
             raise ZeroSpeedError("播放速度仅可为正实数")
         max_volume = 1 if max_volume > 1 else (0.001 if max_volume <= 0 else max_volume)
 
         self.to_music_channels()
 
         tracks = {}
+        InstID = -1
+        # cmd_amount = 0
 
         # 此处 我们把通道视为音轨
         for i in self.channels.keys():
             # 如果当前通道为空 则跳过
             if not self.channels[i]:
                 continue
 
@@ -706,29 +734,21 @@
 
             for track_no, track in self.channels[i].items():
                 for msg in track:
                     if msg[0] == "PgmC":
                         InstID = msg[1]
 
                     elif msg[0] == "NoteS":
-                        try:
-                            soundID, _X = (
-                                self.perc_inst_to_soundID_withX(msg[1])
-                                if SpecialBits
-                                else self.inst_to_souldID_withX(InstID)
-                            )
-                        except UnboundLocalError as E:
-                            # raise NotDefineProgramError(f"未定义乐器便提前演奏。\n{E}")
-                            soundID, _X = (
-                                self.perc_inst_to_soundID_withX(-1)
-                                if SpecialBits
-                                else self.inst_to_souldID_withX(-1)
-                            )
+                        soundID, _X = (
+                            self.perc_inst_to_soundID_withX(msg[1])
+                            if SpecialBits
+                            else self.inst_to_souldID_withX(InstID)
+                        )
+
                         score_now = round(msg[-1] / float(speed) / 50)
-                        # print(score_now)
 
                         try:
                             tracks[score_now].append(
                                 self.execute_cmd_head.format(player_selector)
                                 + f"playsound {soundID} @s ^ ^ ^{128 / max_volume / msg[2] - 1} {msg[2] / 128} "
                                 + (
                                     ""
@@ -743,14 +763,19 @@
                                 + (
                                     ""
                                     if SpecialBits
                                     else f"{2 ** ((msg[1] - 60 - _X) / 12)}"
                                 )
                             ]
 
+                        # cmd_amount += 1
+
+        # print(cmd_amount)
+
+        del InstID
         all_ticks = list(tracks.keys())
         all_ticks.sort()
         results = []
 
         for i in range(len(all_ticks)):
             for j in range(len(tracks[all_ticks[i]])):
                 results.append(
@@ -769,91 +794,15 @@
                             mctick2timestr(i), max_volume * 100, ""
                         ),
                     )
                 )
 
         self.music_command_list = results
         self.music_tick_num = max(all_ticks)
-        return [results, self.music_tick_num]
-
-
-    def to_dict(
-        self,
-    ) -> dict:
-        """
-        使用金羿的转换思路，将midi转换为字典
-        :return: dict()
-        """
-
-        # 一个midi中仅有16个通道 我们通过通道来识别而不是音轨
-        channels = empty_midi_channels()
-
-        # 我们来用通道统计音乐信息
-        # 但是是用分轨的思路的
-        for track_no, track in enumerate(self.midi.tracks):
-            microseconds = 0
-
-            for msg in track:
-                if msg.time != 0:
-                    try:
-                        microseconds += (
-                            msg.time * tempo / self.midi.ticks_per_beat / 1000
-                        )
-                        # print(microseconds)
-                    except NameError:
-                        # raise NotDefineTempoError("计算当前分数时出错 未定义参量 Tempo")
-                        microseconds += (
-                            msg.time
-                            * mido.midifiles.midifiles.DEFAULT_TEMPO
-                            / self.midi.ticks_per_beat
-                        ) / 1000
-
-                if msg.is_meta:
-                    if msg.type == "set_tempo":
-                        tempo = msg.tempo
-                else:
-                    try:
-                        # 曾用于调试模式
-                        # if msg.channel > 15:
-                        # raise ChannelOverFlowError(f"当前消息 {msg} 的通道超限(≤15)")
-                        if not track_no in channels[msg.channel].keys():
-                            channels[msg.channel][track_no] = []
-                    except AttributeError:
-                        pass
-
-                    if msg.type == "program_change":
-                        channels[msg.channel][track_no].append(
-                            ("PgmC", msg.program, microseconds)
-                        )
-
-                    elif msg.type == "note_on" and msg.velocity != 0:
-                        channels[msg.channel][track_no].append(
-                            ("NoteS", msg.note, msg.velocity, microseconds)
-                        )
-
-                    elif (msg.type == "note_on" and msg.velocity == 0) or (
-                        msg.type == "note_off"
-                    ):
-                        channels[msg.channel][track_no].append(
-                            ("NoteE", msg.note, microseconds)
-                        )
-
-        """整合后的音乐通道格式
-        每个通道包括若干消息元素其中逃不过这三种：
-
-        1 切换乐器消息
-        ("PgmC", 切换后的乐器ID: int, 距离演奏开始的毫秒)
-
-        2 音符开始消息
-        ("NoteS", 开始的音符ID, 力度（响度）, 距离演奏开始的毫秒)
-
-        3 音符结束消息
-        ("NoteS", 结束的音符ID, 距离演奏开始的毫秒)"""
-
-        return channels
+        return results, self.music_tick_num
 
     def copy_important(self):
         dst = MidiConvert(
             midi_obj=None,
             midi_name=self.midi_music_name,
             enable_old_exe_format=self.enable_old_exe_format,
         )
```

### Comparing `Musicreater-1.1.0/Musicreater/plugin/__init__.py` & `Musicreater-1.2.0/Musicreater/plugin/mcstructfile/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # -*- coding: utf-8 -*-
 """
-存放非音·创本体的附加内容（插件？）
+用以生成单个mcstructure文件的附加功能
 
 版权所有 © 2023 音·创 开发者
 Copyright © 2023 all the developers of Musicreater
 
 开源相关声明请见 仓库根目录下的 License.md
 Terms & Conditions: License.md in the root directory
 """
 
 # 睿穆组织 开发交流群 861684859
 # Email TriM-Organization@hotmail.com
 # 若需转载或借鉴 许可声明请查看仓库目录下的 License.md
 
 
-__all__ = []
-__author__ = (("金羿", "Eilles Wan"), ("诸葛亮与八卦阵", "bgArray"))
+__all__ = [
+    "to_mcstructure_file_in_delay"
+]
+__author__ = (("金羿", "Eilles Wan"),)
+
+from .main import *
 
-from .main import *
```

### Comparing `Musicreater-1.1.0/Musicreater/plugin/archive.py` & `Musicreater-1.2.0/Musicreater/plugin/archive.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 # Email TriM-Organization@hotmail.com
 # 若需转载或借鉴 许可声明请查看仓库目录下的 License.md
 
 
 import os
 import uuid
 import zipfile
-from typing import List
+import datetime
+from typing import List, Union, Literal
 
 
 def compress_zipfile(sourceDir, outFilename, compression=8, exceptFile=None):
     """使用compression指定的算法打包目录为zip文件\n
     默认算法为DEFLATED(8),可用算法如下：\n
     STORED = 0\n
     DEFLATED = 8\n
@@ -42,24 +43,31 @@
             arc_name = pathfile[pre_len:].strip(os.path.sep)  # 相对路径
             zipf.write(pathfile, arc_name)
     zipf.close()
 
 
 def behavior_mcpack_manifest(
     pack_description: str = "",
-    pack_version: List[int] = [0, 0, 1],
+    pack_version: Union[List[int], Literal[None]] = None,
     pack_name: str = "",
-    pack_uuid: str = None,
+    pack_uuid: Union[str, Literal[None]] = None,
     modules_description: str = "",
     modules_version: List[int] = [0, 0, 1],
-    modules_uuid: str = None,
+    modules_uuid: Union[str, Literal[None]] = None,
 ):
     """
     生成一个我的世界行为包组件的定义清单文件
     """
+    if not pack_version:
+        now_date = datetime.datetime.now()
+        pack_version = [
+            now_date.year,
+            now_date.month * 100 + now_date.day,
+            now_date.hour * 100 + now_date.minute,
+        ]
     return {
         "format_version": 1,
         "header": {
             "description": pack_description,
             "version": pack_version,
             "name": pack_name,
             "uuid": str(uuid.uuid4()) if not pack_uuid else pack_uuid,
```

### Comparing `Musicreater-1.1.0/Musicreater/plugin/bdx.py` & `Musicreater-1.2.0/Musicreater/plugin/bdx.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.1.0/Musicreater/plugin/bdxfile/__init__.py` & `Musicreater-1.2.0/Musicreater/plugin/mcstructpack/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # -*- coding: utf-8 -*-
 """
-用以生成BDX结构文件的附加功能
+用以生成结构附加包的附加功能
 
 版权所有 © 2023 音·创 开发者
 Copyright © 2023 all the developers of Musicreater
 
 开源相关声明请见 仓库根目录下的 License.md
 Terms & Conditions: License.md in the root directory
 """
 
 # 睿穆组织 开发交流群 861684859
 # Email TriM-Organization@hotmail.com
 # 若需转载或借鉴 许可声明请查看仓库目录下的 License.md
 
 
-__all__ = []
+__all__ = [
+    "to_mcstructure_addon_in_delay"
+]
 __author__ = (("金羿", "Eilles Wan"),)
 
 from .main import *
```

### Comparing `Musicreater-1.1.0/Musicreater/plugin/bdxfile/main.py` & `Musicreater-1.2.0/Musicreater/plugin/bdxfile/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,22 @@
 
 # 睿穆组织 开发交流群 861684859
 # Email TriM-Organization@hotmail.com
 # 若需转载或借鉴 许可声明请查看仓库目录下的 License.md
 
 
 import os
+
 import brotli
 
 from ...main import MidiConvert
-from ..bdx import commands_to_BDX_bytes, bdx_move, x, y, z, form_command_block_in_BDX_bytes
-from ..main import ConvertConfig
 from ...subclass import SingleCommand
+from ..bdx import (bdx_move, commands_to_BDX_bytes,
+                   form_command_block_in_BDX_bytes, x, y, z)
+from ..main import ConvertConfig
 
 
 def to_BDX_file_in_score(
     midi_cvt: MidiConvert,
     data_cfg: ConvertConfig,
     scoreboard_name: str = "mscplay",
     auto_reset: bool = False,
@@ -138,15 +140,15 @@
         部分转换通用参数
     player: str
         玩家选择器，默认为`@a`
     author: str
         作者名称
     max_height: int
         生成结构最大高度
-    
+
     Returns
     -------
     tuple[int指令数量, int音乐总延迟, tuple[int,]结构大小, tuple[int,]终点坐标]
     """
 
     cmdlist, max_delay = midi_cvt.to_command_list_in_delay(
         data_cfg.volume_ratio,
@@ -165,15 +167,14 @@
     ) as f:
         f.write("BD@")
 
     _bytes = (
         b"BDX\x00" + author.encode("utf-8") + b" & Musicreater\x00\x01command_block\x00"
     )
 
-
     cmdBytes, size, finalPos = commands_to_BDX_bytes(cmdlist, max_height - 1)
 
     if data_cfg.progressbar_style:
         scb_name = midi_cvt.midi_music_name[:3] + "Pgb"
         _bytes += form_command_block_in_BDX_bytes(
             r"scoreboard objectives add {} dummy {}计".replace(r"{}", scb_name),
             1,
```

### Comparing `Musicreater-1.1.0/Musicreater/plugin/common.py` & `Musicreater-1.2.0/Musicreater/plugin/common.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.1.0/Musicreater/plugin/funcpack/__init__.py` & `Musicreater-1.2.0/Musicreater/plugin/funcpack/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,12 +10,14 @@
 """
 
 # 睿穆组织 开发交流群 861684859
 # Email TriM-Organization@hotmail.com
 # 若需转载或借鉴 许可声明请查看仓库目录下的 License.md
 
 
-__all__ = []
+__all__ = [
+    "to_function_addon_in_score"
+]
 __author__ = (("金羿", "Eilles Wan"),)
 
 from .main import *
```

### Comparing `Musicreater-1.1.0/Musicreater/plugin/funcpack/main.py` & `Musicreater-1.2.0/Musicreater/plugin/funcpack/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,20 +53,24 @@
 
     # 当文件f夹{self.outputPath}/temp/functions存在时清空其下所有项目，然后创建
     if os.path.exists(f"{data_cfg.dist_path}/temp/functions/"):
         shutil.rmtree(f"{data_cfg.dist_path}/temp/functions/")
     os.makedirs(f"{data_cfg.dist_path}/temp/functions/mscplay")
 
     # 写入manifest.json
-    open(f"{data_cfg.dist_path}/temp/manifest.json", "w", encoding="utf-8").write(
-        json.dumps(
-            behavior_mcpack_manifest("midiPlay"),
+    with open(f"{data_cfg.dist_path}/temp/manifest.json", "w", encoding="utf-8") as f:
+        json.dump(
+            behavior_mcpack_manifest(
+                pack_description=f"{midi_cvt.midi_music_name} 音乐播放包，MCFUNCTION(MCPACK) 计分播放器 - 由 音·创 生成",
+                pack_name=midi_cvt.midi_music_name + "播放",
+                modules_description=f"无 - 由 音·创 生成",
+            ),
+            fp=f,
             indent=4,
         )
-    )
 
     # 将命令列表写入文件
     index_file = open(
         f"{data_cfg.dist_path}/temp/functions/index.mcfunction", "w", encoding="utf-8"
     )
     for i in range(len(cmdlist)):
         index_file.write(f"function mscplay/track{i + 1}\n")
```

### Comparing `Musicreater-1.1.0/Musicreater/plugin/main.py` & `Musicreater-1.2.0/Musicreater/plugin/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # 睿穆组织 开发交流群 861684859
 # Email TriM-Organization@hotmail.com
 # 若需转载或借鉴 许可声明请查看仓库目录下的 License.md
 
 
 from dataclasses import dataclass
-from typing import Tuple, Union
+from typing import Tuple, Union, Literal
 
 from ..constants import DEFAULT_PROGRESSBAR_STYLE
 
 
 @dataclass(init=False)
 class ConvertConfig:
     """
@@ -30,15 +30,15 @@
 
     volume_ratio: float
     """音量比例"""
 
     speed_multiplier: float
     """速度倍率"""
 
-    progressbar_style: Tuple[str, Tuple[str, str]]
+    progressbar_style: Union[Tuple[str, Tuple[str, str]], Literal[None]]
     """进度条样式组"""
 
     dist_path: str
     """输出目录"""
 
     def __init__(
         self,
```

### Comparing `Musicreater-1.1.0/Musicreater/plugin/mcstructfile/__init__.py` & `Musicreater-1.2.0/Musicreater/plugin/websocket/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-用以生成单个mcstructure文件的附加功能
+用以启动WebSocket服务器播放的附加功能
 
 版权所有 © 2023 音·创 开发者
 Copyright © 2023 all the developers of Musicreater
 
 开源相关声明请见 仓库根目录下的 License.md
 Terms & Conditions: License.md in the root directory
 """
```

### Comparing `Musicreater-1.1.0/Musicreater/plugin/mcstructfile/main.py` & `Musicreater-1.2.0/Musicreater/plugin/mcstructfile/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,9 +67,10 @@
         struct.dump(f)
 
     return size, max_delay
 
 
 def to_mcstructure_file_in_redstone(
     midi_cvt: MidiConvert,
-    data_cfg: ConvertConfig,):
-    pass
+    data_cfg: ConvertConfig,
+):
+    pass
```

### Comparing `Musicreater-1.1.0/Musicreater/plugin/mcstructpack/main.py` & `Musicreater-1.2.0/Musicreater/plugin/mcstructpack/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,16 +17,15 @@
 
 from TrimMCStruct import Structure
 
 from ...exceptions import CommandFormatError
 from ...main import MidiConvert
 from ..archive import behavior_mcpack_manifest, compress_zipfile
 from ..main import ConvertConfig
-from ..mcstructure import (commands_to_structure,
-                           form_command_block_in_NBT_struct)
+from ..mcstructure import commands_to_structure, form_command_block_in_NBT_struct
 
 
 def to_mcstructure_addon_in_delay(
     midi_cvt: MidiConvert,
     data_cfg: ConvertConfig,
     player: str = "@a",
     max_height: int = 64,
@@ -68,19 +67,20 @@
     os.makedirs(f"{data_cfg.dist_path}/temp/functions/")
     os.makedirs(f"{data_cfg.dist_path}/temp/structures/")
 
     # 写入manifest.json
     with open(f"{data_cfg.dist_path}/temp/manifest.json", "w", encoding="utf-8") as f:
         json.dump(
             behavior_mcpack_manifest(
-                pack_description=f"Music {midi_cvt.midi_music_name} Play pack, structure in delay - Generated by Musicreater",
-                pack_name=midi_cvt.midi_music_name,
-                modules_description=f"None - Generated by Musicreater",
+                pack_description=f"{midi_cvt.midi_music_name} 音乐播放包，MCSTRUCTURE(MCPACK) 延迟播放器 - 由 音·创 生成",
+                pack_name=midi_cvt.midi_music_name + "播放",
+                modules_description=f"无 - 由 音·创 生成",
             ),
             fp=f,
+            indent=4,
         )
 
     # 将命令列表写入文件
     index_file = open(
         f"{data_cfg.dist_path}/temp/functions/index.mcfunction", "w", encoding="utf-8"
     )
```

### Comparing `Musicreater-1.1.0/Musicreater/plugin/mcstructure.py` & `Musicreater-1.2.0/Musicreater/plugin/mcstructure.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,27 @@
 """
 
 # 睿穆组织 开发交流群 861684859
 # Email TriM-Organization@hotmail.com
 # 若需转载或借鉴 许可声明请查看仓库目录下的 License.md
 
 
-from typing import List
+from typing import List, Tuple
 
 from TrimMCStruct import Block, Structure, TAG_Byte, TAG_Long
 
 from ..subclass import SingleCommand
 from .common import bottem_side_length_of_smallest_square_bottom_box
 
 
 def form_note_block_in_NBT_struct(
-    note: int, coordinate: tuple, instrument: str = "note.harp", powered: bool = False
+    note: int,
+    coordinate: Tuple[int, int, int],
+    instrument: str = "note.harp",
+    powered: bool = False,
 ):
     """生成音符盒方块
     :param note: `int`(0~24)
         音符的音高
     :param coordinate: `tuple[int,int,int]`
         此方块所在之相对坐标
     :param instrument: `str`
@@ -50,15 +53,15 @@
         {
             "block_entity_data": {
                 "note": TAG_Byte(note),
                 "id": "noteblock",
                 "x": coordinate[0],
                 "y": coordinate[1],
                 "z": coordinate[2],
-            }
+            }  # type: ignore
         },
     )
 
 
 def form_repeater_in_NBT_struct(delay: int, facing: int):
     """生成中继器方块
     :param facing:
@@ -158,15 +161,15 @@
                 "conditionalMode": condition,
                 "id": "CommandBlock",
                 "isMovable": True,
                 "powered": False,  # 是否已激活
                 "x": coordinate[0],
                 "y": coordinate[1],
                 "z": coordinate[2],
-            }
+            } # type: ignore
         },
         compability_version=17959425,
     )
 
 
 def commands_to_structure(
     commands: List[SingleCommand],
```

### Comparing `Musicreater-1.1.0/Musicreater/plugin/noteblock.py` & `Musicreater-1.2.0/Musicreater/plugin/noteblock.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.1.0/Musicreater/plugin/websocket/__init__.py` & `Musicreater-1.2.0/Musicreater/plugin/bdxfile/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # -*- coding: utf-8 -*-
 """
-用以启动WebSocket服务器播放的附加功能
+用以生成BDX结构文件的附加功能
 
 版权所有 © 2023 音·创 开发者
 Copyright © 2023 all the developers of Musicreater
 
 开源相关声明请见 仓库根目录下的 License.md
 Terms & Conditions: License.md in the root directory
 """
 
 # 睿穆组织 开发交流群 861684859
 # Email TriM-Organization@hotmail.com
 # 若需转载或借鉴 许可声明请查看仓库目录下的 License.md
 
 
-__all__ = []
+__all__ = [
+    "to_BDX_file_in_score",
+    "to_BDX_file_in_delay"
+]
 __author__ = (("金羿", "Eilles Wan"),)
 
 from .main import *
```

### Comparing `Musicreater-1.1.0/Musicreater/plugin/websocket/main.py` & `Musicreater-1.2.0/Musicreater/plugin/websocket/main.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.1.0/Musicreater/plugin/websocket.py` & `Musicreater-1.2.0/Musicreater/plugin/websocket.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.1.0/Musicreater/subclass.py` & `Musicreater-1.2.0/Musicreater/subclass.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,17 +14,14 @@
 
 # 睿穆组织 开发交流群 861684859
 # Email TriM-Organization@hotmail.com
 # 若需转载或借鉴 许可声明请查看仓库目录下的 License.md
 
 
 from dataclasses import dataclass
-from typing import TypeVar
-
-T = TypeVar("T")  # Declare type variable
 
 
 @dataclass(init=False)
 class SingleNote:
     """存储单个音符的类"""
 
     instrument: int
@@ -32,40 +29,45 @@
 
     note: int
     """音符编号"""
 
     velocity: int
     """力度/响度"""
 
-    startTime: int
+    start_time: int
     """开始之时 ms"""
 
-    lastTime: int
+    duration: int
     """音符持续时间 ms"""
 
+    track_no: int
+    """音符所处的音轨"""
+
     def __init__(
-        self, instrument: int, pitch: int, velocity: int, startTime: int, lastTime: int
+        self, instrument: int, pitch: int, velocity: int, startTime: int, lastTime: int, track_number:int = 0
     ):
         """用于存储单个音符的类
         :param instrument 乐器编号
         :param pitch 音符编号
         :param velocity 力度/响度
         :param startTime 开始之时(ms)
             注：此处的时间是用从乐曲开始到当前的毫秒数
         :param lastTime 音符延续时间(ms)"""
         self.instrument: int = instrument
         """乐器编号"""
         self.note: int = pitch
         """音符编号"""
         self.velocity: int = velocity
         """力度/响度"""
-        self.startTime: int = startTime
+        self.start_time: int = startTime
         """开始之时 ms"""
-        self.lastTime: int = lastTime
+        self.duration: int = lastTime
         """音符持续时间 ms"""
+        self.track_no: int = track_number
+        """音符所处的音轨"""
 
     @property
     def inst(self):
         """乐器编号"""
         return self.instrument
 
     @inst.setter
@@ -76,27 +78,27 @@
     def pitch(self):
         """音符编号"""
         return self.note
 
     def __str__(self):
         return (
             f"Note(inst = {self.inst}, pitch = {self.note}, velocity = {self.velocity}, "
-            f"startTime = {self.startTime}, lastTime = {self.lastTime}, )"
+            f"startTime = {self.start_time}, lastTime = {self.duration}, )"
         )
 
     def __tuple__(self):
-        return self.inst, self.note, self.velocity, self.startTime, self.lastTime
+        return self.inst, self.note, self.velocity, self.start_time, self.duration
 
     def __dict__(self):
         return {
             "inst": self.inst,
             "pitch": self.note,
             "velocity": self.velocity,
-            "startTime": self.startTime,
-            "lastTime": self.lastTime,
+            "startTime": self.start_time,
+            "lastTime": self.duration,
         }
 
 
 @dataclass(init=False)
 class SingleCommand:
     """存储单个指令的类"""
 
@@ -164,22 +166,7 @@
             cmd=self.command_text,
         )
 
     def __eq__(self, other) -> bool:
         if not isinstance(other, self.__class__):
             return False
         return self.__str__() == other.__str__()
-
-
-class MethodList(list):
-    """函数列表，列表中的所有元素均为函数"""
-
-    def __init__(self, in_=()):
-        """函数列表，列表中的所有元素均为函数"""
-        super().__init__()
-        self._T = [_x for _x in in_]
-
-    def __getitem__(self, item) -> T:
-        return self._T[item]
-
-    def __len__(self) -> int:
-        return self._T.__len__()
```

### Comparing `Musicreater-1.1.0/Musicreater.egg-info/PKG-INFO` & `Musicreater-1.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: Musicreater
-Version: 1.1.0
-Summary: 一款免费开源的 《我的世界》 mid音乐转换库。
-Home-page: https://github.com/TriM-Organization/Musicreater
-Author: Eilles Wan, bgArray
-Author-email: TriM-Organization@hotmail.com
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: Chinese (Simplified)
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 <h1 align="center">
     音·创 Musicreater
 </h1>
 
 <p align="center">
     <img width="128" height="128" src="https://gitee.com/TriM-Organization/Musicreater/raw/master/resources/msctIcon.ico">
     </img>
@@ -85,17 +63,17 @@
   python setup.py install
   ```
 
 以上命令中 `python`、`pip` 请依照各个环境不同灵活更换，可能为`python3`或`pip3`之类。
 
 ## 文档 📄
 
-[生成文件的使用](https://github.com/TriM-Organization/Musicreater/blob/master/docs/%E7%94%9F%E6%88%90%E6%96%87%E4%BB%B6%E7%9A%84%E4%BD%BF%E7%94%A8%E8%AF%B4%E6%98%8E.md)
+[生成文件的使用](./docs/%E7%94%9F%E6%88%90%E6%96%87%E4%BB%B6%E7%9A%84%E4%BD%BF%E7%94%A8%E8%AF%B4%E6%98%8E.md)
 
-[仓库 API 文档](https://github.com/TriM-Organization/Musicreater/blob/master/docs/%E5%BA%93%E7%9A%84%E7%94%9F%E6%88%90%E4%B8%8E%E5%8A%9F%E8%83%BD%E6%96%87%E6%A1%A3.md)
+[仓库 API 文档](./docs/%E5%BA%93%E7%9A%84%E7%94%9F%E6%88%90%E4%B8%8E%E5%8A%9F%E8%83%BD%E6%96%87%E6%A1%A3.md)
 
 ## 作者 ✒
 
 金羿 Eilles：我的世界基岩版指令师，个人开发者，B 站不知名 UP 主，江西在校高中生。
 
 诸葛亮与八卦阵 bgArray：我的世界基岩版玩家，喜欢编程和音乐，深圳初二学生。
 
@@ -107,16 +85,17 @@
 - 感谢由 **Charlie_Ping “查理平”** 带来的 BDX 文件转换参考，以及 MIDI-我的世界对应乐器 参考表格
 - 感谢由 **[CMA_2401PT](https://github.com/CMA2401PT)** 为我们的软件开发的一些方面进行指导，同时我们参考了他的 BDXworkshop 作为 BDX 结构编辑的参考
 - 感谢由 **[Dislink Sforza](https://github.com/Dislink) “断联·斯福尔扎”**\<QQ1600515314\> 带来的 midi 音色解析以及转换指令的算法，我们将其改编并应用；同时，感谢他的[网页版转换器](https://dislink.github.io/midi2bdx/)给我们的开发与更新带来巨大的压力和动力，让我们在原本一骑绝尘的摸鱼道路上转向开发，希望他能考上一个理想的大学！
 - 感谢 **Touch “偷吃”**\<QQ1793537164\> 提供的 BDX 导入测试支持，并对程序的改进提供了丰富的意见；同时也感谢他的不断尝试新的内容，使我们的排错更进一步
 - 感谢 **Mono**\<QQ738893087\> 反馈安装时的问题，辅助我们找到了视窗操作系统下的兼容性问题；感谢其反馈延迟播放器出现的重大问题，让我们得以修改全部延迟播放错误；尤其感谢他对于我们的软件的大力宣传
 - 感谢 **Ammelia “艾米利亚”**\<QQ2838334637\> 敦促我们进行新的功能开发，并为新功能提出了非常优秀的大量建议，以及提供的 BDX 导入测试支持，为我们的新结构生成算法提供了大量的实际理论支持
 - 感谢 **[神羽](https://gitee.com/snowykami) “[SnowyKami](https://github.com/snowyfirefly)”** 对我们项目的支持与宣传，希望他能考得一所优秀的大学！
-- 感谢 **指令师\_苦力怕 playjuice123**\<QQ240667197\>为我们的程序找出错误，并提醒我们修复一个一直存在的大 bug。
-- 感谢 **雷霆**\<QQ3555268519\>用他那令所有开发者都大为光火的操作方法为我们的程序找出错误，并提醒修复 bug。
+- 感谢 **指令师\_苦力怕 playjuice123**\<QQ240667197\> 为我们的程序找出错误，并提醒我们修复一个一直存在的大 bug。
+- 感谢 **雷霆**\<QQ3555268519\> 用他那令所有开发者都大为光火的操作方法为我们的程序找出错误，并提醒修复 bug。
+- 感谢 **小埋**\<2039310975\> 反馈附加包生成时缺少描述和标题的问题。
 
 >     感谢广大群友为此程序提供的测试等支持
 >
 >     若您对我们有所贡献但您的名字没有显示在此列表中，请联系我们！
 
 ## 联系 📞
```

#### html2text {}

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1 Name: Musicreater Version: 1.1.0 Summary:
-ä¸æ¬¾åè´¹å¼æºç ãæçä¸çã midé³ä¹è½¬æ¢åºã Home-page:
-https://github.com/TriM-Organization/Musicreater Author: Eilles Wan, bgArray
-Author-email: TriM-Organization@hotmail.com Classifier: Intended Audience ::
-Developers Classifier: Natural Language :: Chinese (Simplified) Classifier:
-License :: OSI Approved :: Apache Software License Classifier: Operating System
-:: OS Independent Classifier: Topic :: Software Development :: Libraries
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Description-Content-Type: text/markdown
-License-File: LICENSE.md
                       ****** é³Â·å Musicreater ******
     [https://gitee.com/TriM-Organization/Musicreater/raw/master/resources/
                                 msctIcon.ico]
    **** ä¸æ¬¾åè´¹å¼æºçãæçä¸çãæ°å­é³é¢è½¬æ¢åºã ****
 [https://forthebadge.com/images/badges/built-with-love.svg] [Fork_me_on_Gitee]_
 [![][Bilibili: éç¾¿ELS]](https://space.bilibili.com/397369002/) [![]
 [Bilibili: è¯¸èäº®ä¸å«å¦éµ]](https://space.bilibili.com/604072474) [!
@@ -36,19 +23,17 @@
 pip install Musicreater ``` - å¦æåºç°éè¯¯ï¼å¯ä»¥å°è¯ï¼ ```bash pip
 install -i https://pypi.python.org/simple Musicreater ``` - åçº§ï¼ ```bash
 pip install -i https://pypi.python.org/simple Musicreater --upgrade ``` -
 åéä»åºå¹¶å®è£ ```bash git clone https://gitee.com/TriM-Organization/
 Musicreater.git cd Musicreater python setup.py install ``` ä»¥ä¸å½ä»¤ä¸­
 `python`ã`pip`
 è¯·ä¾ç§åä¸ªç¯å¢ä¸åçµæ´»æ´æ¢ï¼å¯è½ä¸º`python3`æ`pip3`ä¹ç±»ã
-## ææ¡£ ð [çææä»¶çä½¿ç¨](https://github.com/TriM-Organization/
-Musicreater/blob/master/docs/
+## ææ¡£ ð [çææä»¶çä½¿ç¨](./docs/
 %E7%94%9F%E6%88%90%E6%96%87%E4%BB%B6%E7%9A%84%E4%BD%BF%E7%94%A8%E8%AF%B4%E6%98%8E.md)
-[ä»åº API ææ¡£](https://github.com/TriM-Organization/Musicreater/blob/
-master/docs/
+[ä»åº API ææ¡£](./docs/
 %E5%BA%93%E7%9A%84%E7%94%9F%E6%88%90%E4%B8%8E%E5%8A%9F%E8%83%BD%E6%96%87%E6%A1%A3.md)
 ## ä½è â éç¾¿
 Eillesï¼æçä¸çåºå²©çæä»¤å¸ï¼ä¸ªäººå¼åèï¼B ç«ä¸ç¥å UP
 ä¸»ï¼æ±è¥¿å¨æ ¡é«ä¸­çã è¯¸èäº®ä¸å«å¦éµ
 bgArrayï¼æçä¸çåºå²©çç©å®¶ï¼åæ¬¢ç¼ç¨åé³ä¹ï¼æ·±å³åäºå­¦çã
 ## è´è°¢ ð æ¬è´è°¢åè¡¨æåæ é¡ºåºã - æè°¢ **ææ¢¦**\>
 æ¾åºæä»¤çæéè¯¯ bug å¹¶ææ­£ - æè°¢ç± **Charlie_Ping
@@ -68,19 +53,21 @@
 - æè°¢ **Ammelia âè¾ç±³å©äºâ**\>
 æ¦ä¿æä»¬è¿è¡æ°çåè½å¼åï¼å¹¶ä¸ºæ°åè½æåºäºéå¸¸ä¼ç§çå¤§éå»ºè®®ï¼ä»¥åæä¾ç
 BDX
 å¯¼å¥æµè¯æ¯æï¼ä¸ºæä»¬çæ°ç»æçæç®æ³æä¾äºå¤§éçå®éçè®ºæ¯æ
 - æè°¢ **[ç¥ç¾½](https://gitee.com/snowykami) â[SnowyKami](https://
 github.com/snowyfirefly)â**
 å¯¹æä»¬é¡¹ç®çæ¯æä¸å®£ä¼ ï¼å¸æä»è½èå¾ä¸æä¼ç§çå¤§å­¦ï¼
-- æè°¢ **æä»¤å¸\_è¦åæ
-playjuice123**\>ä¸ºæä»¬çç¨åºæ¾åºéè¯¯ï¼å¹¶æéæä»¬ä¿®å¤ä¸ä¸ªä¸ç´å­å¨çå¤§
-bugã - æè°¢
-**é·é**\>ç¨ä»é£ä»¤ææå¼åèé½å¤§ä¸ºåç«çæä½æ¹æ³ä¸ºæä»¬çç¨åºæ¾åºéè¯¯ï¼å¹¶æéä¿®å¤
-bugã > æè°¢å¹¿å¤§ç¾¤åä¸ºæ­¤ç¨åºæä¾çæµè¯ç­æ¯æ > >
+- æè°¢ **æä»¤å¸\_è¦åæ playjuice123**\>
+ä¸ºæä»¬çç¨åºæ¾åºéè¯¯ï¼å¹¶æéæä»¬ä¿®å¤ä¸ä¸ªä¸ç´å­å¨çå¤§
+bugã - æè°¢ **é·é**\>
+ç¨ä»é£ä»¤ææå¼åèé½å¤§ä¸ºåç«çæä½æ¹æ³ä¸ºæä»¬çç¨åºæ¾åºéè¯¯ï¼å¹¶æéä¿®å¤
+bugã - æè°¢ **å°å**\<2039310975\>
+åé¦éå åçææ¶ç¼ºå°æè¿°åæ é¢çé®é¢ã >
+æè°¢å¹¿å¤§ç¾¤åä¸ºæ­¤ç¨åºæä¾çæµè¯ç­æ¯æ > >
 è¥æ¨å¯¹æä»¬ææè´¡ç®ä½æ¨çåå­æ²¡ææ¾ç¤ºå¨æ­¤åè¡¨ä¸­ï¼è¯·èç³»æä»¬ï¼
 ## èç³» ð è¥éå°åºä¸­çé®é¢ï¼æ¬¢è¿å¨[æ­¤](https://gitee.com/
 TriM-Organization/Musicreater/issues/new)æåºä½ ç issueã
 å¦æéè¦ä¸å¼åç»è¿è¡äº¤æµï¼æ¬¢è¿å å¥æä»¬ç[å¼åé²è Q
 ç¾¤](https://jq.qq.com/?_wv=1027&k=hpeRxrYr)ã --- æ­¤é¡¹ç®å¹¶éä¸ä¸ªå®æ¹
 ãæçä¸çãï¼_Minecraft_ï¼é¡¹ç® æ­¤é¡¹ç®ä¸é¶å±æå³èäº Mojang
 Studios æ å¾®è½¯ æ­¤é¡¹ç®äº¦ä¸é¶å±æå³èäº ç½æ âMinecraftâæ¯
```

### Comparing `Musicreater-1.1.0/Musicreater.egg-info/SOURCES.txt` & `Musicreater-1.2.0/Musicreater.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 Musicreater/__init__.py
 Musicreater/constants.py
 Musicreater/exceptions.py
 Musicreater/experiment.py
 Musicreater/magicmain.py
 Musicreater/main.py
+Musicreater/previous.py
 Musicreater/subclass.py
 Musicreater/utils.py
 Musicreater.egg-info/PKG-INFO
 Musicreater.egg-info/SOURCES.txt
 Musicreater.egg-info/dependency_links.txt
 Musicreater.egg-info/requires.txt
 Musicreater.egg-info/top_level.txt
```

### Comparing `Musicreater-1.1.0/PKG-INFO` & `Musicreater-1.2.0/Musicreater.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 204d 7573  : 2.1..Name: Mus
 00000020: 6963 7265 6174 6572 0d0a 5665 7273 696f  icreater..Versio
-00000030: 6e3a 2031 2e31 2e30 0d0a 5375 6d6d 6172  n: 1.1.0..Summar
+00000030: 6e3a 2031 2e32 2e30 0d0a 5375 6d6d 6172  n: 1.2.0..Summar
 00000040: 793a 20e4 b880 e6ac bee5 858d e8b4 b9e5  y: .............
 00000050: bc80 e6ba 90e7 9a84 20e3 808a e688 91e7  ........ .......
 00000060: 9a84 e4b8 96e7 958c e380 8b20 6d69 64e9  ........... mid.
 00000070: 9fb3 e4b9 90e8 bdac e68d a2e5 ba93 e380  ................
 00000080: 820d 0a48 6f6d 652d 7061 6765 3a20 6874  ...Home-page: ht
 00000090: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 000000a0: 2f54 7269 4d2d 4f72 6761 6e69 7a61 7469  /TriM-Organizati
@@ -61,429 +61,423 @@
 000003c0: 3d22 6365 6e74 6572 223e 0d0a 2020 2020  ="center">..    
 000003d0: e99f b3c2 b7e5 889b 204d 7573 6963 7265  ........ Musicre
 000003e0: 6174 6572 0d0a 3c2f 6831 3e0d 0a0d 0a3c  ater..</h1>....<
 000003f0: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
 00000400: 3e0d 0a20 2020 203c 696d 6720 7769 6474  >..    <img widt
 00000410: 683d 2231 3238 2220 6865 6967 6874 3d22  h="128" height="
 00000420: 3132 3822 2073 7263 3d22 6874 7470 733a  128" src="https:
-00000430: 2f2f 6769 7465 652e 636f 6d2f 5472 694d  //gitee.com/TriM
-00000440: 2d4f 7267 616e 697a 6174 696f 6e2f 4d75  -Organization/Mu
-00000450: 7369 6372 6561 7465 722f 7261 772f 6d61  sicreater/raw/ma
-00000460: 7374 6572 2f72 6573 6f75 7263 6573 2f6d  ster/resources/m
-00000470: 7363 7449 636f 6e2e 6963 6f22 3e0d 0a20  sctIcon.ico">.. 
-00000480: 2020 203c 2f69 6d67 3e0d 0a3c 2f70 3e0d     </img>..</p>.
-00000490: 0a0d 0a3c 6833 2061 6c69 676e 3d22 6365  ...<h3 align="ce
-000004a0: 6e74 6572 223e e4b8 80e6 acbe e585 8de8  nter">..........
-000004b0: b4b9 e5bc 80e6 ba90 e79a 84e3 808a e688  ................
-000004c0: 91e7 9a84 e4b8 96e7 958c e380 8be6 95b0  ................
-000004d0: e5ad 97e9 9fb3 e9a2 91e8 bdac e68d a2e5  ................
-000004e0: ba93 e380 823c 2f68 333e 0d0a 0d0a 3c70  .....</h3>....<p
-000004f0: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
-00000500: 0d0a 2020 2020 3c69 6d67 2073 7263 3d22  ..    <img src="
-00000510: 6874 7470 733a 2f2f 666f 7274 6865 6261  https://fortheba
-00000520: 6467 652e 636f 6d2f 696d 6167 6573 2f62  dge.com/images/b
-00000530: 6164 6765 732f 6275 696c 742d 7769 7468  adges/built-with
-00000540: 2d6c 6f76 652e 7376 6722 3e0d 0a20 2020  -love.svg">..   
-00000550: 203c 6120 6872 6566 3d27 6874 7470 733a   <a href='https:
-00000560: 2f2f 6769 7465 652e 636f 6d2f 5472 694d  //gitee.com/TriM
-00000570: 2d4f 7267 616e 697a 6174 696f 6e2f 4d75  -Organization/Mu
-00000580: 7369 6372 6561 7465 7227 3e0d 0a20 2020  sicreater'>..   
-00000590: 2020 2020 203c 696d 6720 616c 6967 6e3d       <img align=
-000005a0: 2272 6967 6874 2220 7372 633d 2768 7474  "right" src='htt
-000005b0: 7073 3a2f 2f67 6974 6565 2e63 6f6d 2f54  ps://gitee.com/T
-000005c0: 7269 4d2d 4f72 6761 6e69 7a61 7469 6f6e  riM-Organization
-000005d0: 2f4d 7573 6963 7265 6174 6572 2f77 6964  /Musicreater/wid
-000005e0: 6765 7473 2f77 6964 6765 745f 312e 7376  gets/widget_1.sv
-000005f0: 6727 2061 6c74 3d27 466f 726b 206d 6520  g' alt='Fork me 
-00000600: 6f6e 2047 6974 6565 273e 0d0a 2020 2020  on Gitee'>..    
-00000610: 2020 2020 3c2f 696d 673e 0d0a 2020 2020      </img>..    
-00000620: 3c2f 613e 0d0a 3c70 3e0d 0a0d 0a5b 215b  </a>..<p>....[![
-00000630: 5d5b 4269 6c69 6269 6c69 3a20 e987 91e7  ][Bilibili: ....
-00000640: bebf 454c 535d 5d28 6874 7470 733a 2f2f  ..ELS]](https://
-00000650: 7370 6163 652e 6269 6c69 6269 6c69 2e63  space.bilibili.c
-00000660: 6f6d 2f33 3937 3336 3930 3032 2f29 0d0a  om/397369002/)..
-00000670: 5b21 5b5d 5b42 696c 6962 696c 693a 20e8  [![][Bilibili: .
-00000680: afb8 e891 9be4 baae e4b8 8ee5 85ab e58d  ................
-00000690: a6e9 98b5 5d5d 2868 7474 7073 3a2f 2f73  ....]](https://s
-000006a0: 7061 6365 2e62 696c 6962 696c 692e 636f  pace.bilibili.co
-000006b0: 6d2f 3630 3430 3732 3437 3429 0d0a 5b21  m/604072474)..[!
-000006c0: 5b43 6f64 6553 7479 6c65 3a20 626c 6163  [CodeStyle: blac
-000006d0: 6b5d 5d28 6874 7470 733a 2f2f 6769 7468  k]](https://gith
-000006e0: 7562 2e63 6f6d 2f70 7366 2f62 6c61 636b  ub.com/psf/black
-000006f0: 290d 0a5b 215b 5d5b 7079 7468 6f6e 5d5d  )..[![][python]]
-00000700: 2868 7474 7073 3a2f 2f77 7777 2e70 7974  (https://www.pyt
-00000710: 686f 6e2e 6f72 672f 290d 0a5b 215b 5d5b  hon.org/)..[![][
-00000720: 6c69 6365 6e73 655d 5d28 4c49 4345 4e53  license]](LICENS
-00000730: 4529 0d0a 5b21 5b5d 5b72 656c 6561 7365  E)..[![][release
-00000740: 5d5d 282e 2e2f 2e2e 2f72 656c 6561 7365  ]](../../release
-00000750: 7329 0d0a 0d0a 5b21 5b47 6974 6565 5374  s)....[![GiteeSt
-00000760: 6172 5d28 6874 7470 733a 2f2f 6769 7465  ar](https://gite
-00000770: 652e 636f 6d2f 5472 694d 2d4f 7267 616e  e.com/TriM-Organ
-00000780: 697a 6174 696f 6e2f 4d75 7369 6372 6561  ization/Musicrea
-00000790: 7465 722f 6261 6467 652f 7374 6172 2e73  ter/badge/star.s
-000007a0: 7667 3f74 6865 6d65 3d67 7261 7929 5d28  vg?theme=gray)](
-000007b0: 6874 7470 733a 2f2f 6769 7465 652e 636f  https://gitee.co
-000007c0: 6d2f 5472 694d 2d4f 7267 616e 697a 6174  m/TriM-Organizat
-000007d0: 696f 6e2f 4d75 7369 6372 6561 7465 722f  ion/Musicreater/
-000007e0: 7374 6172 6761 7a65 7273 290d 0a5b 215b  stargazers)..[![
-000007f0: 4769 7465 6546 6f72 6b5d 2868 7474 7073  GiteeFork](https
-00000800: 3a2f 2f67 6974 6565 2e63 6f6d 2f54 7269  ://gitee.com/Tri
-00000810: 4d2d 4f72 6761 6e69 7a61 7469 6f6e 2f4d  M-Organization/M
-00000820: 7573 6963 7265 6174 6572 2f62 6164 6765  usicreater/badge
-00000830: 2f66 6f72 6b2e 7376 673f 7468 656d 653d  /fork.svg?theme=
-00000840: 6772 6179 295d 2868 7474 7073 3a2f 2f67  gray)](https://g
-00000850: 6974 6565 2e63 6f6d 2f54 7269 4d2d 4f72  itee.com/TriM-Or
-00000860: 6761 6e69 7a61 7469 6f6e 2f4d 7573 6963  ganization/Music
-00000870: 7265 6174 6572 2f6d 656d 6265 7273 290d  reater/members).
-00000880: 0a5b 215b 4769 7448 7562 2052 6570 6f20  .[![GitHub Repo 
-00000890: 7374 6172 735d 2868 7474 7073 3a2f 2f69  stars](https://i
-000008a0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
-000008b0: 7468 7562 2f73 7461 7273 2f54 7269 4d2d  thub/stars/TriM-
-000008c0: 4f72 6761 6e69 7a61 7469 6f6e 2f4d 7573  Organization/Mus
-000008d0: 6963 7265 6174 6572 3f63 6f6c 6f72 3d77  icreater?color=w
-000008e0: 6869 7465 266c 6f67 6f3d 4769 7448 7562  hite&logo=GitHub
-000008f0: 2673 7479 6c65 3d70 6c61 7374 6963 295d  &style=plastic)]
-00000900: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000910: 636f 6d2f 5472 694d 2d4f 7267 616e 697a  com/TriM-Organiz
-00000920: 6174 696f 6e2f 4d75 7369 6372 6561 7465  ation/Musicreate
-00000930: 722f 7374 6172 6761 7a65 7273 290d 0a5b  r/stargazers)..[
-00000940: 215b 4769 7448 7562 2052 6570 6f20 466f  ![GitHub Repo Fo
-00000950: 726b 735d 2868 7474 7073 3a2f 2f69 6d67  rks](https://img
-00000960: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
-00000970: 7562 2f66 6f72 6b73 2f54 7269 4d2d 4f72  ub/forks/TriM-Or
-00000980: 6761 6e69 7a61 7469 6f6e 2f4d 7573 6963  ganization/Music
-00000990: 7265 6174 6572 3f63 6f6c 6f72 3d77 6869  reater?color=whi
-000009a0: 7465 266c 6f67 6f3d 4769 7448 7562 2673  te&logo=GitHub&s
-000009b0: 7479 6c65 3d70 6c61 7374 6963 295d 2868  tyle=plastic)](h
-000009c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000009d0: 6d2f 5472 694d 2d4f 7267 616e 697a 6174  m/TriM-Organizat
-000009e0: 696f 6e2f 4d75 7369 6372 6561 7465 722f  ion/Musicreater/
-000009f0: 666f 726b 7329 0d0a 0d0a e7ae 80e4 bd93  forks)..........
-00000a00: e4b8 ade6 9687 20f0 9f87 a8f0 9f87 b320  ...... ........ 
-00000a10: 7c20 5b45 6e67 6c69 7368 f09f 87ac f09f  | [English......
-00000a20: 87a7 5d28 5245 4144 4d45 5f45 4e2e 6d64  ..](README_EN.md
-00000a30: 290d 0a0d 0a23 2320 e4bb 8be7 bb8d 20f0  )....## ...... .
-00000a40: 9f9a 800d 0a0d 0ae9 9fb3 c2b7 e588 9b20  ............... 
-00000a50: e698 afe4 b880 e4b8 aae5 858d e8b4 b9e5  ................
-00000a60: bc80 e6ba 90e7 9a84 e992 88e5 afb9 202a  .............. *
-00000a70: 2ae3 808a e688 91e7 9a84 e4b8 96e7 958c  *...............
-00000a80: e380 8b2a 2a20 e79a 8420 4d49 4449 20e9  ...** ... MIDI .
-00000a90: 9fb3 e4b9 90e8 bdac e68d a2e5 ba93 0d0a  ................
-00000aa0: 0d0a e6ac a2e8 bf8e e58a a0e7 bea4 efbc  ................
-00000ab0: 9a5b 3836 3136 3834 3835 395d 2868 7474  .[861684859](htt
-00000ac0: 7073 3a2f 2f6a 712e 7171 2e63 6f6d 2f3f  ps://jq.qq.com/?
-00000ad0: 5f77 763d 3130 3237 266b 3d68 7065 5278  _wv=1027&k=hpeRx
-00000ae0: 7259 7229 0d0a 0d0a 2323 20e5 ae89 e8a3  rYr)....## .....
-00000af0: 8520 f09f 94b3 0d0a 0d0a 2d20 e4bd bfe7  . ........- ....
-00000b00: 94a8 2070 7970 690d 0a0d 0a20 2060 6060  .. pypi....  ```
-00000b10: 6261 7368 0d0a 2020 7069 7020 696e 7374  bash..  pip inst
-00000b20: 616c 6c20 4d75 7369 6372 6561 7465 720d  all Musicreater.
-00000b30: 0a20 2060 6060 0d0a 0d0a 2d20 e5a6 82e6  .  ```....- ....
-00000b40: 9e9c e587 bae7 8eb0 e994 99e8 afaf efbc  ................
-00000b50: 8ce5 8faf e4bb a5e5 b09d e8af 95ef bc9a  ................
-00000b60: 0d0a 2020 6060 6062 6173 680d 0a20 2070  ..  ```bash..  p
-00000b70: 6970 2069 6e73 7461 6c6c 202d 6920 6874  ip install -i ht
-00000b80: 7470 733a 2f2f 7079 7069 2e70 7974 686f  tps://pypi.pytho
-00000b90: 6e2e 6f72 672f 7369 6d70 6c65 204d 7573  n.org/simple Mus
-00000ba0: 6963 7265 6174 6572 0d0a 2020 6060 600d  icreater..  ```.
-00000bb0: 0a0d 0a2d 20e5 8d87 e7ba a7ef bc9a 0d0a  ...- ...........
-00000bc0: 0d0a 2020 6060 6062 6173 680d 0a20 2070  ..  ```bash..  p
-00000bd0: 6970 2069 6e73 7461 6c6c 202d 6920 6874  ip install -i ht
-00000be0: 7470 733a 2f2f 7079 7069 2e70 7974 686f  tps://pypi.pytho
-00000bf0: 6e2e 6f72 672f 7369 6d70 6c65 204d 7573  n.org/simple Mus
-00000c00: 6963 7265 6174 6572 202d 2d75 7067 7261  icreater --upgra
-00000c10: 6465 0d0a 2020 6060 600d 0a0d 0a2d 20e5  de..  ```....- .
-00000c20: 858b e99a 86e4 bb93 e5ba 93e5 b9b6 e5ae  ................
-00000c30: 89e8 a385 0d0a 2020 6060 6062 6173 680d  ......  ```bash.
-00000c40: 0a20 2067 6974 2063 6c6f 6e65 2068 7474  .  git clone htt
-00000c50: 7073 3a2f 2f67 6974 6565 2e63 6f6d 2f54  ps://gitee.com/T
-00000c60: 7269 4d2d 4f72 6761 6e69 7a61 7469 6f6e  riM-Organization
-00000c70: 2f4d 7573 6963 7265 6174 6572 2e67 6974  /Musicreater.git
-00000c80: 0d0a 2020 6364 204d 7573 6963 7265 6174  ..  cd Musicreat
-00000c90: 6572 0d0a 2020 7079 7468 6f6e 2073 6574  er..  python set
-00000ca0: 7570 2e70 7920 696e 7374 616c 6c0d 0a20  up.py install.. 
-00000cb0: 2060 6060 0d0a 0d0a e4bb a5e4 b88a e591   ```............
-00000cc0: bde4 bba4 e4b8 ad20 6070 7974 686f 6e60  ....... `python`
-00000cd0: e380 8160 7069 7060 20e8 afb7 e4be 9de7  ...`pip` .......
-00000ce0: 85a7 e590 84e4 b8aa e78e afe5 a283 e4b8  ................
-00000cf0: 8de5 908c e781 b5e6 b4bb e69b b4e6 8da2  ................
-00000d00: efbc 8ce5 8faf e883 bde4 b8ba 6070 7974  ............`pyt
-00000d10: 686f 6e33 60e6 8896 6070 6970 3360 e4b9  hon3`...`pip3`..
-00000d20: 8be7 b1bb e380 820d 0a0d 0a23 2320 e696  ...........## ..
-00000d30: 87e6 a1a3 20f0 9f93 840d 0a0d 0a5b e794  .... ........[..
-00000d40: 9fe6 8890 e696 87e4 bbb6 e79a 84e4 bdbf  ................
-00000d50: e794 a85d 2868 7474 7073 3a2f 2f67 6974  ...](https://git
-00000d60: 6875 622e 636f 6d2f 5472 694d 2d4f 7267  hub.com/TriM-Org
-00000d70: 616e 697a 6174 696f 6e2f 4d75 7369 6372  anization/Musicr
-00000d80: 6561 7465 722f 626c 6f62 2f6d 6173 7465  eater/blob/maste
-00000d90: 722f 646f 6373 2f25 4537 2539 3425 3946  r/docs/%E7%94%9F
-00000da0: 2545 3625 3838 2539 3025 4536 2539 3625  %E6%88%90%E6%96%
-00000db0: 3837 2545 3425 4242 2542 3625 4537 2539  87%E4%BB%B6%E7%9
-00000dc0: 4125 3834 2545 3425 4244 2542 4625 4537  A%84%E4%BD%BF%E7
-00000dd0: 2539 3425 4138 2545 3825 4146 2542 3425  %94%A8%E8%AF%B4%
-00000de0: 4536 2539 3825 3845 2e6d 6429 0d0a 0d0a  E6%98%8E.md)....
-00000df0: 5be4 bb93 e5ba 9320 4150 4920 e696 87e6  [...... API ....
-00000e00: a1a3 5d28 6874 7470 733a 2f2f 6769 7468  ..](https://gith
-00000e10: 7562 2e63 6f6d 2f54 7269 4d2d 4f72 6761  ub.com/TriM-Orga
-00000e20: 6e69 7a61 7469 6f6e 2f4d 7573 6963 7265  nization/Musicre
-00000e30: 6174 6572 2f62 6c6f 622f 6d61 7374 6572  ater/blob/master
-00000e40: 2f64 6f63 732f 2545 3525 4241 2539 3325  /docs/%E5%BA%93%
-00000e50: 4537 2539 4125 3834 2545 3725 3934 2539  E7%9A%84%E7%94%9
-00000e60: 4625 4536 2538 3825 3930 2545 3425 4238  F%E6%88%90%E4%B8
-00000e70: 2538 4525 4535 2538 4125 3946 2545 3825  %8E%E5%8A%9F%E8%
-00000e80: 3833 2542 4425 4536 2539 3625 3837 2545  83%BD%E6%96%87%E
-00000e90: 3625 4131 2541 332e 6d64 290d 0a0d 0a23  6%A1%A3.md)....#
-00000ea0: 2320 e4bd 9ce8 8085 20e2 9c92 0d0a 0d0a  # ...... .......
-00000eb0: e987 91e7 bebf 2045 696c 6c65 73ef bc9a  ...... Eilles...
-00000ec0: e688 91e7 9a84 e4b8 96e7 958c e59f bae5  ................
-00000ed0: b2a9 e789 88e6 8c87 e4bb a4e5 b888 efbc  ................
-00000ee0: 8ce4 b8aa e4ba bae5 bc80 e58f 91e8 8085  ................
-00000ef0: efbc 8c42 20e7 ab99 e4b8 8de7 9fa5 e590  ...B ...........
-00000f00: 8d20 5550 20e4 b8bb efbc 8ce6 b19f e8a5  . UP ...........
-00000f10: bfe5 9ca8 e6a0 a1e9 ab98 e4b8 ade7 949f  ................
-00000f20: e380 820d 0a0d 0ae8 afb8 e891 9be4 baae  ................
-00000f30: e4b8 8ee5 85ab e58d a6e9 98b5 2062 6741  ............ bgA
-00000f40: 7272 6179 efbc 9ae6 8891 e79a 84e4 b896  rray............
-00000f50: e795 8ce5 9fba e5b2 a9e7 8988 e78e a9e5  ................
-00000f60: aeb6 efbc 8ce5 969c e6ac a2e7 bc96 e7a8  ................
-00000f70: 8be5 928c e99f b3e4 b990 efbc 8ce6 b7b1  ................
-00000f80: e59c b3e5 889d e4ba 8ce5 ada6 e794 9fe3  ................
-00000f90: 8082 0d0a 0d0a 2323 20e8 87b4 e8b0 a220  ......## ...... 
-00000fa0: f09f 998f 0d0a 0d0a e69c ace8 87b4 e8b0  ................
-00000fb0: a2e5 8897 e8a1 a8e6 8e92 e590 8de6 97a0  ................
-00000fc0: e9a1 bae5 ba8f e380 820d 0a0d 0a2d 20e6  .............- .
-00000fd0: 849f e8b0 a220 2a2a e698 80e6 a2a6 2a2a  ..... **......**
-00000fe0: 5c3c 5151 3135 3135 3339 3938 3835 5c3e  \<QQ1515399885\>
-00000ff0: 20e6 89be e587 bae6 8c87 e4bb a4e7 949f   ...............
-00001000: e688 90e9 9499 e8af af20 6275 6720 e5b9  ......... bug ..
-00001010: b6e6 8c87 e6ad a30d 0a2d 20e6 849f e8b0  .........- .....
-00001020: a2e7 94b1 202a 2a43 6861 726c 6965 5f50  .... **Charlie_P
-00001030: 696e 6720 e280 9ce6 9fa5 e790 86e5 b9b3  ing ............
-00001040: e280 9d2a 2a20 e5b8 a6e6 9da5 e79a 8420  ...** ......... 
-00001050: 4244 5820 e696 87e4 bbb6 e8bd ace6 8da2  BDX ............
-00001060: e58f 82e8 8083 efbc 8ce4 bba5 e58f 8a20  ............... 
-00001070: 4d49 4449 2de6 8891 e79a 84e4 b896 e795  MIDI-...........
-00001080: 8ce5 afb9 e5ba 94e4 b990 e599 a820 e58f  ............. ..
-00001090: 82e8 8083 e8a1 a8e6 a0bc 0d0a 2d20 e684  ............- ..
-000010a0: 9fe8 b0a2 e794 b120 2a2a 5b43 4d41 5f32  ....... **[CMA_2
-000010b0: 3430 3150 545d 2868 7474 7073 3a2f 2f67  401PT](https://g
-000010c0: 6974 6875 622e 636f 6d2f 434d 4132 3430  ithub.com/CMA240
-000010d0: 3150 5429 2a2a 20e4 b8ba e688 91e4 bbac  1PT)** .........
-000010e0: e79a 84e8 bdaf e4bb b6e5 bc80 e58f 91e7  ................
-000010f0: 9a84 e4b8 80e4 ba9b e696 b9e9 9da2 e8bf  ................
-00001100: 9be8 a18c e68c 87e5 afbc efbc 8ce5 908c  ................
-00001110: e697 b6e6 8891 e4bb ace5 8f82 e880 83e4  ................
-00001120: ba86 e4bb 96e7 9a84 2042 4458 776f 726b  ........ BDXwork
-00001130: 7368 6f70 20e4 bd9c e4b8 ba20 4244 5820  shop ...... BDX 
-00001140: e7bb 93e6 9e84 e7bc 96e8 be91 e79a 84e5  ................
-00001150: 8f82 e880 830d 0a2d 20e6 849f e8b0 a2e7  .......- .......
-00001160: 94b1 202a 2a5b 4469 736c 696e 6b20 5366  .. **[Dislink Sf
-00001170: 6f72 7a61 5d28 6874 7470 733a 2f2f 6769  orza](https://gi
-00001180: 7468 7562 2e63 6f6d 2f44 6973 6c69 6e6b  thub.com/Dislink
-00001190: 2920 e280 9ce6 96ad e881 94c2 b7e6 96af  ) ..............
-000011a0: e7a6 8fe5 b094 e689 8ee2 809d 2a2a 5c3c  ............**\<
-000011b0: 5151 3136 3030 3531 3533 3134 5c3e 20e5  QQ1600515314\> .
-000011c0: b8a6 e69d a5e7 9a84 206d 6964 6920 e99f  ........ midi ..
-000011d0: b3e8 89b2 e8a7 a3e6 9e90 e4bb a5e5 8f8a  ................
-000011e0: e8bd ace6 8da2 e68c 87e4 bba4 e79a 84e7  ................
-000011f0: ae97 e6b3 95ef bc8c e688 91e4 bbac e5b0  ................
-00001200: 86e5 85b6 e694 b9e7 bc96 e5b9 b6e5 ba94  ................
-00001210: e794 a8ef bc9b e590 8ce6 97b6 efbc 8ce6  ................
-00001220: 849f e8b0 a2e4 bb96 e79a 845b e7bd 91e9  ...........[....
-00001230: a1b5 e789 88e8 bdac e68d a2e5 99a8 5d28  ..............](
-00001240: 6874 7470 733a 2f2f 6469 736c 696e 6b2e  https://dislink.
-00001250: 6769 7468 7562 2e69 6f2f 6d69 6469 3262  github.io/midi2b
-00001260: 6478 2f29 e7bb 99e6 8891 e4bb ace7 9a84  dx/)............
-00001270: e5bc 80e5 8f91 e4b8 8ee6 9bb4 e696 b0e5  ................
-00001280: b8a6 e69d a5e5 b7a8 e5a4 a7e7 9a84 e58e  ................
-00001290: 8be5 8a9b e592 8ce5 8aa8 e58a 9bef bc8c  ................
-000012a0: e8ae a9e6 8891 e4bb ace5 9ca8 e58e 9fe6  ................
-000012b0: 9cac e4b8 80e9 aa91 e7bb 9de5 b098 e79a  ................
-000012c0: 84e6 91b8 e9b1 bce9 8193 e8b7 afe4 b88a  ................
-000012d0: e8bd ace5 9091 e5bc 80e5 8f91 efbc 8ce5  ................
-000012e0: b88c e69c 9be4 bb96 e883 bde8 8083 e4b8  ................
-000012f0: 8ae4 b880 e4b8 aae7 9086 e683 b3e7 9a84  ................
-00001300: e5a4 a7e5 ada6 efbc 810d 0a2d 20e6 849f  ...........- ...
-00001310: e8b0 a220 2a2a 546f 7563 6820 e280 9ce5  ... **Touch ....
-00001320: 81b7 e590 83e2 809d 2a2a 5c3c 5151 3137  ........**\<QQ17
-00001330: 3933 3533 3731 3634 5c3e 20e6 8f90 e4be  93537164\> .....
-00001340: 9be7 9a84 2042 4458 20e5 afbc e585 a5e6  .... BDX .......
-00001350: b58b e8af 95e6 94af e68c 81ef bc8c e5b9  ................
-00001360: b6e5 afb9 e7a8 8be5 ba8f e79a 84e6 94b9  ................
-00001370: e8bf 9be6 8f90 e4be 9be4 ba86 e4b8 b0e5  ................
-00001380: af8c e79a 84e6 848f e8a7 81ef bc9b e590  ................
-00001390: 8ce6 97b6 e4b9 9fe6 849f e8b0 a2e4 bb96  ................
-000013a0: e79a 84e4 b88d e696 ade5 b09d e8af 95e6  ................
-000013b0: 96b0 e79a 84e5 8685 e5ae b9ef bc8c e4bd  ................
-000013c0: bfe6 8891 e4bb ace7 9a84 e68e 92e9 9499  ................
-000013d0: e69b b4e8 bf9b e4b8 80e6 ada5 0d0a 2d20  ..............- 
-000013e0: e684 9fe8 b0a2 202a 2a4d 6f6e 6f2a 2a5c  ...... **Mono**\
-000013f0: 3c51 5137 3338 3839 3330 3837 5c3e 20e5  <QQ738893087\> .
-00001400: 8f8d e9a6 88e5 ae89 e8a3 85e6 97b6 e79a  ................
-00001410: 84e9 97ae e9a2 98ef bc8c e8be 85e5 8aa9  ................
-00001420: e688 91e4 bbac e689 bee5 88b0 e4ba 86e8  ................
-00001430: a786 e7aa 97e6 938d e4bd 9ce7 b3bb e7bb  ................
-00001440: 9fe4 b88b e79a 84e5 85bc e5ae b9e6 80a7  ................
-00001450: e997 aee9 a298 efbc 9be6 849f e8b0 a2e5  ................
-00001460: 85b6 e58f 8de9 a688 e5bb b6e8 bf9f e692  ................
-00001470: ade6 94be e599 a8e5 87ba e78e b0e7 9a84  ................
-00001480: e987 8de5 a4a7 e997 aee9 a298 efbc 8ce8  ................
-00001490: aea9 e688 91e4 bbac e5be 97e4 bba5 e4bf  ................
-000014a0: aee6 94b9 e585 a8e9 83a8 e5bb b6e8 bf9f  ................
-000014b0: e692 ade6 94be e994 99e8 afaf efbc 9be5  ................
-000014c0: b0a4 e585 b6e6 849f e8b0 a2e4 bb96 e5af  ................
-000014d0: b9e4 ba8e e688 91e4 bbac e79a 84e8 bdaf  ................
-000014e0: e4bb b6e7 9a84 e5a4 a7e5 8a9b e5ae a3e4  ................
-000014f0: bca0 0d0a 2d20 e684 9fe8 b0a2 202a 2a41  ....- ...... **A
-00001500: 6d6d 656c 6961 20e2 809c e889 bee7 b1b3  mmelia .........
-00001510: e588 a9e4 ba9a e280 9d2a 2a5c 3c51 5132  .........**\<QQ2
-00001520: 3833 3833 3334 3633 375c 3e20 e695 a6e4  838334637\> ....
-00001530: bf83 e688 91e4 bbac e8bf 9be8 a18c e696  ................
-00001540: b0e7 9a84 e58a 9fe8 83bd e5bc 80e5 8f91  ................
-00001550: efbc 8ce5 b9b6 e4b8 bae6 96b0 e58a 9fe8  ................
-00001560: 83bd e68f 90e5 87ba e4ba 86e9 9d9e e5b8  ................
-00001570: b8e4 bc98 e7a7 80e7 9a84 e5a4 a7e9 878f  ................
-00001580: e5bb bae8 aeae efbc 8ce4 bba5 e58f 8ae6  ................
-00001590: 8f90 e4be 9be7 9a84 2042 4458 20e5 afbc  ........ BDX ...
-000015a0: e585 a5e6 b58b e8af 95e6 94af e68c 81ef  ................
-000015b0: bc8c e4b8 bae6 8891 e4bb ace7 9a84 e696  ................
-000015c0: b0e7 bb93 e69e 84e7 949f e688 90e7 ae97  ................
-000015d0: e6b3 95e6 8f90 e4be 9be4 ba86 e5a4 a7e9  ................
-000015e0: 878f e79a 84e5 ae9e e999 85e7 9086 e8ae  ................
-000015f0: bae6 94af e68c 810d 0a2d 20e6 849f e8b0  .........- .....
-00001600: a220 2a2a 5be7 a59e e7be bd5d 2868 7474  . **[......](htt
-00001610: 7073 3a2f 2f67 6974 6565 2e63 6f6d 2f73  ps://gitee.com/s
-00001620: 6e6f 7779 6b61 6d69 2920 e280 9c5b 536e  nowykami) ...[Sn
-00001630: 6f77 794b 616d 695d 2868 7474 7073 3a2f  owyKami](https:/
-00001640: 2f67 6974 6875 622e 636f 6d2f 736e 6f77  /github.com/snow
-00001650: 7966 6972 6566 6c79 29e2 809d 2a2a 20e5  yfirefly)...** .
-00001660: afb9 e688 91e4 bbac e9a1 b9e7 9bae e79a  ................
-00001670: 84e6 94af e68c 81e4 b88e e5ae a3e4 bca0  ................
-00001680: efbc 8ce5 b88c e69c 9be4 bb96 e883 bde8  ................
-00001690: 8083 e5be 97e4 b880 e689 80e4 bc98 e7a7  ................
-000016a0: 80e7 9a84 e5a4 a7e5 ada6 efbc 810d 0a2d  ...............-
-000016b0: 20e6 849f e8b0 a220 2a2a e68c 87e4 bba4   ...... **......
-000016c0: e5b8 885c 5fe8 8ba6 e58a 9be6 8095 2070  ...\_......... p
-000016d0: 6c61 796a 7569 6365 3132 332a 2a5c 3c51  layjuice123**\<Q
-000016e0: 5132 3430 3636 3731 3937 5c3e e4b8 bae6  Q240667197\>....
-000016f0: 8891 e4bb ace7 9a84 e7a8 8be5 ba8f e689  ................
-00001700: bee5 87ba e994 99e8 afaf efbc 8ce5 b9b6  ................
-00001710: e68f 90e9 8692 e688 91e4 bbac e4bf aee5  ................
-00001720: a48d e4b8 80e4 b8aa e4b8 80e7 9bb4 e5ad  ................
-00001730: 98e5 9ca8 e79a 84e5 a4a7 2062 7567 e380  .......... bug..
-00001740: 820d 0a2d 20e6 849f e8b0 a220 2a2a e99b  ...- ...... **..
-00001750: b7e9 9c86 2a2a 5c3c 5151 3335 3535 3236  ....**\<QQ355526
-00001760: 3835 3139 5c3e e794 a8e4 bb96 e982 a3e4  8519\>..........
-00001770: bba4 e689 80e6 9c89 e5bc 80e5 8f91 e880  ................
-00001780: 85e9 83bd e5a4 a7e4 b8ba e585 89e7 81ab  ................
-00001790: e79a 84e6 938d e4bd 9ce6 96b9 e6b3 95e4  ................
-000017a0: b8ba e688 91e4 bbac e79a 84e7 a88b e5ba  ................
-000017b0: 8fe6 89be e587 bae9 9499 e8af afef bc8c  ................
-000017c0: e5b9 b6e6 8f90 e986 92e4 bfae e5a4 8d20  ............... 
-000017d0: 6275 67e3 8082 0d0a 0d0a 3e20 2020 2020  bug.......>     
-000017e0: e684 9fe8 b0a2 e5b9 bfe5 a4a7 e7be a4e5  ................
-000017f0: 8f8b e4b8 bae6 ada4 e7a8 8be5 ba8f e68f  ................
-00001800: 90e4 be9b e79a 84e6 b58b e8af 95e7 ad89  ................
-00001810: e694 afe6 8c81 0d0a 3e0d 0a3e 2020 2020  ........>..>    
-00001820: 20e8 8ba5 e682 a8e5 afb9 e688 91e4 bbac   ...............
-00001830: e69c 89e6 8980 e8b4 a1e7 8cae e4bd 86e6  ................
-00001840: 82a8 e79a 84e5 908d e5ad 97e6 b2a1 e69c  ................
-00001850: 89e6 98be e7a4 bae5 9ca8 e6ad a4e5 8897  ................
-00001860: e8a1 a8e4 b8ad efbc 8ce8 afb7 e881 94e7  ................
-00001870: b3bb e688 91e4 bbac efbc 810d 0a0d 0a23  ...............#
-00001880: 2320 e881 94e7 b3bb 20f0 9f93 9e0d 0a0d  # ...... .......
-00001890: 0ae8 8ba5 e981 87e5 88b0 e5ba 93e4 b8ad  ................
-000018a0: e79a 84e9 97ae e9a2 98ef bc8c e6ac a2e8  ................
-000018b0: bf8e e59c a85b e6ad a45d 2868 7474 7073  .....[...](https
-000018c0: 3a2f 2f67 6974 6565 2e63 6f6d 2f54 7269  ://gitee.com/Tri
-000018d0: 4d2d 4f72 6761 6e69 7a61 7469 6f6e 2f4d  M-Organization/M
-000018e0: 7573 6963 7265 6174 6572 2f69 7373 7565  usicreater/issue
-000018f0: 732f 6e65 7729 e68f 90e5 87ba e4bd a0e7  s/new)..........
-00001900: 9a84 2069 7373 7565 e380 820d 0a0d 0ae5  .. issue........
-00001910: a682 e69e 9ce9 9c80 e8a6 81e4 b88e e5bc  ................
-00001920: 80e5 8f91 e7bb 84e8 bf9b e8a1 8ce4 baa4  ................
-00001930: e6b5 81ef bc8c e6ac a2e8 bf8e e58a a0e5  ................
-00001940: 85a5 e688 91e4 bbac e79a 845b e5bc 80e5  ...........[....
-00001950: 8f91 e997 b2e8 818a 2051 20e7 bea4 5d28  ........ Q ...](
-00001960: 6874 7470 733a 2f2f 6a71 2e71 712e 636f  https://jq.qq.co
-00001970: 6d2f 3f5f 7776 3d31 3032 3726 6b3d 6870  m/?_wv=1027&k=hp
-00001980: 6552 7872 5972 29e3 8082 0d0a 0d0a 2d2d  eRxrYr).......--
-00001990: 2d0d 0a0d 0ae6 ada4 e9a1 b9e7 9bae e5b9  -...............
-000019a0: b6e9 9d9e e4b8 80e4 b8aa e5ae 98e6 96b9  ................
-000019b0: 20e3 808a e688 91e7 9a84 e4b8 96e7 958c   ...............
-000019c0: e380 8bef bc88 5f4d 696e 6563 7261 6674  ......_Minecraft
-000019d0: 5fef bc89 e9a1 b9e7 9bae 0d0a 0d0a e6ad  _...............
-000019e0: a4e9 a1b9 e79b aee4 b88d e99a b6e5 b19e  ................
-000019f0: e688 96e5 85b3 e881 94e4 ba8e 204d 6f6a  ............ Moj
-00001a00: 616e 6720 5374 7564 696f 7320 e688 9620  ang Studios ... 
-00001a10: e5be aee8 bdaf 0d0a 0d0a e6ad a4e9 a1b9  ................
-00001a20: e79b aee4 baa6 e4b8 8de9 9ab6 e5b1 9ee6  ................
-00001a30: 8896 e585 b3e8 8194 e4ba 8e20 e7bd 91e6  ........... ....
-00001a40: 9893 0d0a 0d0a e280 9c4d 696e 6563 7261  .........Minecra
-00001a50: 6674 e280 9de6 98af 204d 6f6a 616e 6720  ft...... Mojang 
-00001a60: 5379 6e65 7267 6965 7320 4142 20e7 9a84  Synergies AB ...
-00001a70: e595 86e6 a087 efbc 8ce6 ada4 e9a1 b9e7  ................
-00001a80: 9bae e4b8 ade6 8980 e69c 89e5 afb9 e4ba  ................
-00001a90: 8ee2 809c e688 91e7 9a84 e4b8 96e7 958c  ................
-00001aa0: e280 9de3 8081 e280 9c4d 696e 6563 7261  .........Minecra
-00001ab0: 6674 e280 9de7 ad89 e79b b8e5 85b3 e7a7  ft..............
-00001ac0: b0e5 91bc e59d 87e4 b8ba e5bc 95e7 94a8  ................
-00001ad0: e680 a7e4 bdbf e794 a80d 0a0d 0a2d 20e4  .............- .
-00001ae0: b88a e696 87e6 8f90 e58f 8ae7 9a84 20e7  .............. .
-00001af0: bd91 e698 9320 e585 ace5 8fb8 efbc 8ce6  ..... ..........
-00001b00: 8c87 e4bb a3e7 9a84 e698 afe5 9ca8 e4b8  ................
-00001b10: ade5 9bbd e5a4 a7e9 9986 e8bf 90e8 90a5  ................
-00001b20: e380 8ae6 8891 e79a 84e4 b896 e795 8cef  ................
-00001b30: bc9a e4b8 ade5 9bbd e789 88e3 808b e79a  ................
-00001b40: 84e4 b88a e6b5 b7e7 bd91 e4b9 8be6 9893  ................
-00001b50: e7bd 91e7 bb9c e7a7 91e6 8a80 e58f 91e5  ................
-00001b60: b195 e69c 89e9 9990 e585 ace5 8fb8 0d0a  ................
-00001b70: 0d0a 4e4f 5420 414e 204f 4646 4943 4941  ..NOT AN OFFICIA
-00001b80: 4c20 4d49 4e45 4352 4146 5420 5052 4f44  L MINECRAFT PROD
-00001b90: 5543 542e 0d0a 0d0a 4e4f 5420 4150 5052  UCT.....NOT APPR
-00001ba0: 4f56 4544 2042 5920 4f52 2041 5353 4f43  OVED BY OR ASSOC
-00001bb0: 4941 5445 4420 5749 5448 204d 4f4a 414e  IATED WITH MOJAN
-00001bc0: 4720 4f52 204d 4943 524f 534f 4654 2e0d  G OR MICROSOFT..
-00001bd0: 0a0d 0a4e 4f54 2041 5050 524f 5645 4420  ...NOT APPROVED 
-00001be0: 4259 204f 5220 4153 534f 4349 4154 4544  BY OR ASSOCIATED
-00001bf0: 2057 4954 4820 4e45 5445 4153 452e 0d0a   WITH NETEASE...
-00001c00: 0d0a 5b42 696c 6962 696c 693a 20e9 8791  ..[Bilibili: ...
-00001c10: e7be bf45 4c53 5d3a 2068 7474 7073 3a2f  ...ELS]: https:/
-00001c20: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00001c30: 6261 6467 652f 4269 6c69 6269 6c69 2d25  badge/Bilibili-%
-00001c40: 4535 2538 3725 3843 2545 3425 4241 2539  E5%87%8C%E4%BA%9
-00001c50: 3125 4539 2538 3725 3931 2545 3725 4245  1%E9%87%91%E7%BE
-00001c60: 2542 462d 3030 4131 4537 3f73 7479 6c65  %BF-00A1E7?style
-00001c70: 3d66 6f72 2d74 6865 2d62 6164 6765 0d0a  =for-the-badge..
-00001c80: 5b42 696c 6962 696c 693a 20e8 afb8 e891  [Bilibili: .....
-00001c90: 9be4 baae e4b8 8ee5 85ab e58d a6e9 98b5  ................
-00001ca0: 5d3a 2068 7474 7073 3a2f 2f69 6d67 2e73  ]: https://img.s
-00001cb0: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-00001cc0: 4269 6c69 6269 6c69 2d25 4538 2541 4625  Bilibili-%E8%AF%
-00001cd0: 4238 2545 3825 3931 2539 4225 4534 2542  B8%E8%91%9B%E4%B
-00001ce0: 4125 4145 2545 3425 4238 2538 4525 4535  A%AE%E4%B8%8E%E5
-00001cf0: 2538 3525 4142 2545 3525 3844 2541 3625  %85%AB%E5%8D%A6%
-00001d00: 4539 2539 3825 4235 2d30 3041 3145 373f  E9%98%B5-00A1E7?
-00001d10: 7374 796c 653d 666f 722d 7468 652d 6261  style=for-the-ba
-00001d20: 6467 650d 0a5b 436f 6465 5374 796c 653a  dge..[CodeStyle:
-00001d30: 2062 6c61 636b 5d3a 2068 7474 7073 3a2f   black]: https:/
-00001d40: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00001d50: 6261 6467 652f 636f 6465 2532 3073 7479  badge/code%20sty
-00001d60: 6c65 2d62 6c61 636b 2d31 3231 3131 302e  le-black-121110.
-00001d70: 7376 673f 7374 796c 653d 666f 722d 7468  svg?style=for-th
-00001d80: 652d 6261 6467 650d 0a5b 7079 7468 6f6e  e-badge..[python
-00001d90: 5d3a 2068 7474 7073 3a2f 2f69 6d67 2e73  ]: https://img.s
-00001da0: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-00001db0: 7079 7468 6f6e 2d33 2e38 2d41 4237 3046  python-3.8-AB70F
-00001dc0: 463f 7374 796c 653d 666f 722d 7468 652d  F?style=for-the-
-00001dd0: 6261 6467 650d 0a5b 7265 6c65 6173 655d  badge..[release]
-00001de0: 3a20 6874 7470 733a 2f2f 696d 672e 7368  : https://img.sh
-00001df0: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
-00001e00: 762f 7265 6c65 6173 652f 4569 6c6c 6573  v/release/Eilles
-00001e10: 5761 6e2f 4d75 7369 6372 6561 7465 723f  Wan/Musicreater?
-00001e20: 7374 796c 653d 666f 722d 7468 652d 6261  style=for-the-ba
-00001e30: 6467 650d 0a5b 6c69 6365 6e73 655d 3a20  dge..[license]: 
-00001e40: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00001e50: 6c64 732e 696f 2f62 6164 6765 2f4c 6963  lds.io/badge/Lic
-00001e60: 656e 6365 2d41 7061 6368 652d 3232 3842  ence-Apache-228B
-00001e70: 3232 3f73 7479 6c65 3d66 6f72 2d74 6865  22?style=for-the
-00001e80: 2d62 6164 6765 0d0a                      -badge..
+00000430: 2f2f 7331 2e61 7831 782e 636f 6d2f 3230  //s1.ax1x.com/20
+00000440: 3232 2f30 352f 3036 2f4f 7568 6768 6a2e  22/05/06/Ouhghj.
+00000450: 6d64 2e70 6e67 2220 3e0d 0a20 2020 203c  md.png" >..    <
+00000460: 2f69 6d67 3e0d 0a3c 2f70 3e0d 0a0d 0a3c  /img>..</p>....<
+00000470: 6833 2061 6c69 676e 3d22 6365 6e74 6572  h3 align="center
+00000480: 223e 4120 6672 6565 206f 7065 6e2d 736f  ">A free open-so
+00000490: 7572 6365 206c 6962 7261 7279 206f 6620  urce library of 
+000004a0: 636f 6e76 6572 7469 6e67 2064 6967 6974  converting digit
+000004b0: 616c 206d 7573 6963 2066 696c 6573 2069  al music files i
+000004c0: 6e74 6f20 3c69 3e4d 696e 6563 7261 6674  nto <i>Minecraft
+000004d0: 3c2f 693e 2066 6f72 6d61 7473 2e3c 2f68  </i> formats.</h
+000004e0: 333e 0d0a 0d0a 3c70 2061 6c69 676e 3d22  3>....<p align="
+000004f0: 6365 6e74 6572 223e 0d0a 2020 2020 3c69  center">..    <i
+00000500: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000510: 666f 7274 6865 6261 6467 652e 636f 6d2f  forthebadge.com/
+00000520: 696d 6167 6573 2f62 6164 6765 732f 6275  images/badges/bu
+00000530: 696c 742d 7769 7468 2d6c 6f76 652e 7376  ilt-with-love.sv
+00000540: 6722 3e0d 0a20 2020 203c 2f69 6d67 3e0d  g">..    </img>.
+00000550: 0a3c 703e 0d0a 0d0a 5b21 5b5d 5b42 696c  .<p>....[![][Bil
+00000560: 6962 696c 693a 2045 696c 6c65 735d 5d28  ibili: Eilles]](
+00000570: 6874 7470 733a 2f2f 7370 6163 652e 6269  https://space.bi
+00000580: 6c69 6269 6c69 2e63 6f6d 2f33 3937 3336  libili.com/39736
+00000590: 3930 3032 2f29 0d0a 5b21 5b5d 5b42 696c  9002/)..[![][Bil
+000005a0: 6962 696c 693a 2062 6741 7272 6179 5d5d  ibili: bgArray]]
+000005b0: 2868 7474 7073 3a2f 2f73 7061 6365 2e62  (https://space.b
+000005c0: 696c 6962 696c 692e 636f 6d2f 3630 3430  ilibili.com/6040
+000005d0: 3732 3437 3429 0d0a 5b21 5b43 6f64 6553  72474)..[![CodeS
+000005e0: 7479 6c65 3a20 626c 6163 6b5d 5d28 6874  tyle: black]](ht
+000005f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000600: 2f70 7366 2f62 6c61 636b 290d 0a5b 215b  /psf/black)..[![
+00000610: 5d5b 7079 7468 6f6e 5d5d 2868 7474 7073  ][python]](https
+00000620: 3a2f 2f77 7777 2e70 7974 686f 6e2e 6f72  ://www.python.or
+00000630: 672f 290d 0a5b 215b 5d5b 6c69 6365 6e73  g/)..[![][licens
+00000640: 655d 5d28 4c49 4345 4e53 4529 0d0a 5b21  e]](LICENSE)..[!
+00000650: 5b5d 5b72 656c 6561 7365 5d5d 282e 2e2f  [][release]](../
+00000660: 2e2e 2f72 656c 6561 7365 7329 0d0a 0d0a  ../releases)....
+00000670: 5b21 5b47 6974 6565 5374 6172 5d28 6874  [![GiteeStar](ht
+00000680: 7470 733a 2f2f 6769 7465 652e 636f 6d2f  tps://gitee.com/
+00000690: 5472 694d 2d4f 7267 616e 697a 6174 696f  TriM-Organizatio
+000006a0: 6e2f 4d75 7369 6372 6561 7465 722f 6261  n/Musicreater/ba
+000006b0: 6467 652f 7374 6172 2e73 7667 3f74 6865  dge/star.svg?the
+000006c0: 6d65 3d67 7261 7929 5d28 6874 7470 733a  me=gray)](https:
+000006d0: 2f2f 6769 7465 652e 636f 6d2f 5472 694d  //gitee.com/TriM
+000006e0: 2d4f 7267 616e 697a 6174 696f 6e2f 4d75  -Organization/Mu
+000006f0: 7369 6372 6561 7465 722f 7374 6172 6761  sicreater/starga
+00000700: 7a65 7273 290d 0a5b 215b 4769 7465 6546  zers)..[![GiteeF
+00000710: 6f72 6b5d 2868 7474 7073 3a2f 2f67 6974  ork](https://git
+00000720: 6565 2e63 6f6d 2f54 7269 4d2d 4f72 6761  ee.com/TriM-Orga
+00000730: 6e69 7a61 7469 6f6e 2f4d 7573 6963 7265  nization/Musicre
+00000740: 6174 6572 2f62 6164 6765 2f66 6f72 6b2e  ater/badge/fork.
+00000750: 7376 673f 7468 656d 653d 6772 6179 295d  svg?theme=gray)]
+00000760: 2868 7474 7073 3a2f 2f67 6974 6565 2e63  (https://gitee.c
+00000770: 6f6d 2f54 7269 4d2d 4f72 6761 6e69 7a61  om/TriM-Organiza
+00000780: 7469 6f6e 2f4d 7573 6963 7265 6174 6572  tion/Musicreater
+00000790: 2f6d 656d 6265 7273 290d 0a5b 215b 4769  /members)..[![Gi
+000007a0: 7448 7562 2052 6570 6f20 7374 6172 735d  tHub Repo stars]
+000007b0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+000007c0: 656c 6473 2e69 6f2f 6769 7468 7562 2f73  elds.io/github/s
+000007d0: 7461 7273 2f54 7269 4d2d 4f72 6761 6e69  tars/TriM-Organi
+000007e0: 7a61 7469 6f6e 2f4d 7573 6963 7265 6174  zation/Musicreat
+000007f0: 6572 3f63 6f6c 6f72 3d77 6869 7465 266c  er?color=white&l
+00000800: 6f67 6f3d 4769 7448 7562 2673 7479 6c65  ogo=GitHub&style
+00000810: 3d70 6c61 7374 6963 295d 2868 7474 7073  =plastic)](https
+00000820: 3a2f 2f67 6974 6875 622e 636f 6d2f 5472  ://github.com/Tr
+00000830: 694d 2d4f 7267 616e 697a 6174 696f 6e2f  iM-Organization/
+00000840: 4d75 7369 6372 6561 7465 722f 7374 6172  Musicreater/star
+00000850: 6761 7a65 7273 290d 0a5b 215b 4769 7448  gazers)..[![GitH
+00000860: 7562 2052 6570 6f20 466f 726b 735d 2868  ub Repo Forks](h
+00000870: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000880: 6473 2e69 6f2f 6769 7468 7562 2f66 6f72  ds.io/github/for
+00000890: 6b73 2f54 7269 4d2d 4f72 6761 6e69 7a61  ks/TriM-Organiza
+000008a0: 7469 6f6e 2f4d 7573 6963 7265 6174 6572  tion/Musicreater
+000008b0: 3f63 6f6c 6f72 3d77 6869 7465 266c 6f67  ?color=white&log
+000008c0: 6f3d 4769 7448 7562 2673 7479 6c65 3d70  o=GitHub&style=p
+000008d0: 6c61 7374 6963 295d 2868 7474 7073 3a2f  lastic)](https:/
+000008e0: 2f67 6974 6875 622e 636f 6d2f 5472 694d  /github.com/TriM
+000008f0: 2d4f 7267 616e 697a 6174 696f 6e2f 4d75  -Organization/Mu
+00000900: 7369 6372 6561 7465 722f 666f 726b 7329  sicreater/forks)
+00000910: 0d0a 0d0a 5be7 ae80 e4bd 93e4 b8ad e696  ....[...........
+00000920: 8720 f09f 87a8 f09f 87b3 5d28 5245 4144  . ........](READ
+00000930: 4d45 2e6d 6429 207c 2045 6e67 6c69 7368  ME.md) | English
+00000940: f09f 87ac f09f 87a7 0d0a 0d0a 2a2a 4e6f  ............**No
+00000950: 7469 6365 2074 6861 7420 7468 6520 6c61  tice that the la
+00000960: 6e67 7561 6765 2074 7261 6e73 6c61 7469  nguage translati
+00000970: 6f6e 206f 6620 5f4d 7573 6963 7265 6174  on of _Musicreat
+00000980: 6572 5f20 6d61 7920 6265 2061 206c 6974  er_ may be a lit
+00000990: 746c 6520 534c 4f57 2e2a 2a0d 0a0d 0a23  tle SLOW.**....#
+000009a0: 2320 496e 7472 6f64 7563 7469 6f6e f09f  # Introduction..
+000009b0: 9a80 0d0a 0d0a 4d75 7369 6372 6561 7465  ......Musicreate
+000009c0: 7220 6973 2061 2066 7265 6520 6f70 656e  r is a free open
+000009d0: 2d73 6f75 7263 6520 6c69 6272 6172 7920  -source library 
+000009e0: 7573 6564 2066 6f72 2063 6f6e 7665 7274  used for convert
+000009f0: 696e 6720 6469 6769 7461 6c20 6d75 7369  ing digital musi
+00000a00: 6320 6669 6c65 7320 696e 746f 2066 6f72  c files into for
+00000a10: 6d61 7473 2074 6861 7420 636f 756c 6420  mats that could 
+00000a20: 6265 2072 6561 6420 696e 205f 4d69 6e65  be read in _Mine
+00000a30: 6372 6166 745f 2e0d 0a0d 0a57 656c 636f  craft_.....Welco
+00000a40: 6d65 2074 6f20 6a6f 696e 206f 7572 2051  me to join our Q
+00000a50: 5120 6772 6f75 703a 205b 3836 3136 3834  Q group: [861684
+00000a60: 3835 395d 2868 7474 7073 3a2f 2f6a 712e  859](https://jq.
+00000a70: 7171 2e63 6f6d 2f3f 5f77 763d 3130 3237  qq.com/?_wv=1027
+00000a80: 266b 3d68 7065 5278 7259 7229 0d0a 0d0a  &k=hpeRxrYr)....
+00000a90: 2323 2049 6e73 7461 6c6c 6174 696f 6e20  ## Installation 
+00000aa0: f09f 94b3 0d0a 0d0a 2d20 5669 6120 7079  ........- Via py
+00000ab0: 7069 0d0a 0d0a 2020 6060 6062 6173 680d  pi....  ```bash.
+00000ac0: 0a20 2070 6970 2069 6e73 7461 6c6c 204d  .  pip install M
+00000ad0: 7573 6963 7265 6174 6572 0d0a 2020 6060  usicreater..  ``
+00000ae0: 600d 0a0d 0a2d 2049 6620 6e6f 7420 776f  `....- If not wo
+00000af0: 726b 2c20 616c 736f 2074 7279 3a0d 0a20  rk, also try:.. 
+00000b00: 2060 6060 6261 7368 0d0a 2020 7069 7020   ```bash..  pip 
+00000b10: 696e 7374 616c 6c20 2d69 2068 7474 7073  install -i https
+00000b20: 3a2f 2f70 7970 692e 7079 7468 6f6e 2e6f  ://pypi.python.o
+00000b30: 7267 2f73 696d 706c 6520 4d75 7369 6372  rg/simple Musicr
+00000b40: 6561 7465 720d 0a20 2060 6060 0d0a 0d0a  eater..  ```....
+00000b50: 2d20 5570 6461 7465 3a0d 0a0d 0a20 2060  - Update:....  `
+00000b60: 6060 6261 7368 0d0a 2020 7069 7020 696e  ``bash..  pip in
+00000b70: 7374 616c 6c20 2d69 2068 7474 7073 3a2f  stall -i https:/
+00000b80: 2f70 7970 692e 7079 7468 6f6e 2e6f 7267  /pypi.python.org
+00000b90: 2f73 696d 706c 6520 4d75 7369 6372 6561  /simple Musicrea
+00000ba0: 7465 7220 2d2d 7570 6772 6164 650d 0a20  ter --upgrade.. 
+00000bb0: 2060 6060 0d0a 0d0a 2d20 436c 6f6e 6520   ```....- Clone 
+00000bc0: 7265 706f 2061 6e64 2049 6e73 7461 6c6c  repo and Install
+00000bd0: 3a0d 0a20 2060 6060 6261 7368 0d0a 2020  :..  ```bash..  
+00000be0: 6769 7420 636c 6f6e 6520 6874 7470 733a  git clone https:
+00000bf0: 2f2f 6769 7468 7562 2e63 6f6d 2f54 7269  //github.com/Tri
+00000c00: 4d2d 4f72 6761 6e69 7a61 7469 6f6e 2f4d  M-Organization/M
+00000c10: 7573 6963 7265 6174 6572 2e67 6974 0d0a  usicreater.git..
+00000c20: 2020 6364 204d 7573 6963 7265 6174 6572    cd Musicreater
+00000c30: 0d0a 2020 7079 7468 6f6e 2073 6574 7570  ..  python setup
+00000c40: 2e70 7920 696e 7374 616c 6c0d 0a20 2060  .py install..  `
+00000c50: 6060 0d0a 0d0a 436f 6d6d 616e 6473 2073  ``....Commands s
+00000c60: 7563 6820 6173 2060 7079 7468 6f6e 60e3  uch as `python`.
+00000c70: 8081 6070 6970 6020 636f 756c 6420 6265  ..`pip` could be
+00000c80: 2063 6861 6e67 6564 2074 6f20 736f 6d65   changed to some
+00000c90: 206c 696b 6520 6070 7974 686f 6e33 6020   like `python3` 
+00000ca0: 6f72 2060 7069 7033 6020 6163 636f 7264  or `pip3` accord
+00000cb0: 696e 6720 746f 2074 6865 2064 6966 6665  ing to the diffe
+00000cc0: 7265 6e63 6520 6f66 2070 6c61 7466 6f72  rence of platfor
+00000cd0: 6d73 2e0d 0a0d 0a0d 0a23 2320 446f 6375  ms.......## Docu
+00000ce0: 6d65 6e74 6174 696f 6ef0 9f93 840d 0a0d  mentation.......
+00000cf0: 0a28 4e6f 7420 696e 2045 6e67 6c69 7368  .(Not in English
+00000d00: 2079 6574 290d 0a0d 0a5b e794 9fe6 8890   yet)....[......
+00000d10: e696 87e4 bbb6 e79a 84e4 bdbf e794 a85d  ...............]
+00000d20: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000d30: 636f 6d2f 5472 694d 2d4f 7267 616e 697a  com/TriM-Organiz
+00000d40: 6174 696f 6e2f 4d75 7369 6372 6561 7465  ation/Musicreate
+00000d50: 722f 626c 6f62 2f6d 6173 7465 722f 646f  r/blob/master/do
+00000d60: 6373 2f25 4537 2539 3425 3946 2545 3625  cs/%E7%94%9F%E6%
+00000d70: 3838 2539 3025 4536 2539 3625 3837 2545  88%90%E6%96%87%E
+00000d80: 3425 4242 2542 3625 4537 2539 4125 3834  4%BB%B6%E7%9A%84
+00000d90: 2545 3425 4244 2542 4625 4537 2539 3425  %E4%BD%BF%E7%94%
+00000da0: 4138 2545 3825 4146 2542 3425 4536 2539  A8%E8%AF%B4%E6%9
+00000db0: 3825 3845 2e6d 6429 0d0a 0d0a 5be4 bb93  8%8E.md)....[...
+00000dc0: e5ba 9320 4150 4920 e696 87e6 a1a3 5d28  ... API ......](
+00000dd0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000de0: 6f6d 2f54 7269 4d2d 4f72 6761 6e69 7a61  om/TriM-Organiza
+00000df0: 7469 6f6e 2f4d 7573 6963 7265 6174 6572  tion/Musicreater
+00000e00: 2f62 6c6f 622f 6d61 7374 6572 2f64 6f63  /blob/master/doc
+00000e10: 732f 2545 3525 4241 2539 3325 4537 2539  s/%E5%BA%93%E7%9
+00000e20: 4125 3834 2545 3725 3934 2539 4625 4536  A%84%E7%94%9F%E6
+00000e30: 2538 3825 3930 2545 3425 4238 2538 4525  %88%90%E4%B8%8E%
+00000e40: 4535 2538 4125 3946 2545 3825 3833 2542  E5%8A%9F%E8%83%B
+00000e50: 4425 4536 2539 3625 3837 2545 3625 4131  D%E6%96%87%E6%A1
+00000e60: 2541 332e 6d64 290d 0a0d 0a23 2323 2041  %A3.md)....### A
+00000e70: 7574 686f 7273 e29c 920d 0a0d 0a45 696c  uthors.......Eil
+00000e80: 6c65 7320 28e9 8791 e7be bf29 efbc 9a41  les (......)...A
+00000e90: 2073 656e 696f 7220 6869 6768 2073 6368   senior high sch
+00000ea0: 6f6f 6c20 7374 7564 656e 742c 2069 6e64  ool student, ind
+00000eb0: 6976 6964 7561 6c20 6465 7665 6c6f 7065  ividual develope
+00000ec0: 722c 2075 6e66 616d 6f75 7320 4269 6c69  r, unfamous Bili
+00000ed0: 6269 6c69 2055 5065 722c 2077 6869 6368  bili UPer, which
+00000ee0: 206b 6e6f 7773 2061 206c 6974 746c 6520   knows a little 
+00000ef0: 6162 6f75 7420 636f 6d6d 616e 6473 2069  about commands i
+00000f00: 6e20 5f4d 696e 6563 7261 6674 3a20 4265  n _Minecraft: Be
+00000f10: 6472 6f63 6b20 4564 6974 696f 6e5f 0d0a  drock Edition_..
+00000f20: 0d0a 6267 4172 7261 7920 22e8 afb8 e891  ..bgArray ".....
+00000f30: 9be4 baae e4b8 8ee5 85ab e58d a6e9 98b5  ................
+00000f40: 223a 2041 206a 756e 696f 7220 6869 6768  ": A junior high
+00000f50: 2073 6368 6f6f 6c20 7374 7564 656e 742c   school student,
+00000f60: 2070 6c61 7965 7220 6f66 205f 4d69 6e65   player of _Mine
+00000f70: 6372 6166 743a 2042 6564 726f 636b 2045  craft: Bedrock E
+00000f80: 6469 7469 6f6e 5f2c 2077 6869 6368 2069  dition_, which i
+00000f90: 7320 6120 6661 6e20 6f66 206d 7573 6963  s a fan of music
+00000fa0: 2061 6e64 2070 726f 6772 616d 6d69 6e67   and programming
+00000fb0: 2e0d 0a0d 0a23 2320 5468 616e 6b73 f09f  .....## Thanks..
+00000fc0: 998f 0d0a 0d0a 5468 6973 206c 6973 7420  ......This list 
+00000fd0: 6973 206e 6f74 2069 6e20 616e 7920 6f72  is not in any or
+00000fe0: 6465 722e 0d0a 0d0a 2d20 5468 616e 6b20  der.....- Thank 
+00000ff0: 5fe6 9880 e6a2 a65f 5c3c 5151 3135 3135  _......_\<QQ1515
+00001000: 3339 3938 3835 5c3e 2066 6f72 2066 696e  399885\> for fin
+00001010: 6469 6e67 2061 6e64 2063 6f72 7265 6374  ding and correct
+00001020: 696e 6720 7468 6520 6275 6773 2069 6e20  ing the bugs in 
+00001030: 7468 6520 636f 6d6d 616e 6473 2074 6861  the commands tha
+00001040: 7420 5f4d 7573 6963 7265 6174 6572 5f20  t _Musicreater_ 
+00001050: 6765 6e65 7261 7465 642e 0d0a 2d20 5468  generated...- Th
+00001060: 616e 6b20 5f43 6861 726c 6965 5f50 696e  ank _Charlie_Pin
+00001070: 6720 e280 9ce6 9fa5 e790 86e5 b9b3 e280  g ..............
+00001080: 9d5f 2066 6f72 2074 6865 2062 6478 2063  ._ for the bdx c
+00001090: 6f6e 7665 7274 2066 756e 6374 696f 6e20  onvert function 
+000010a0: 666f 7220 7265 6665 7265 6e63 652c 2061  for reference, a
+000010b0: 6e64 2074 6865 2072 6566 6572 656e 6365  nd the reference
+000010c0: 2063 6861 7274 2074 6861 7427 7320 7573   chart that's us
+000010d0: 6564 2074 6f20 636f 6e76 6572 7420 7468  ed to convert th
+000010e0: 6520 6d69 6427 7320 696e 7374 7275 6d65  e mid's instrume
+000010f0: 6e74 7320 696e 746f 204d 696e 6563 7261  nts into Minecra
+00001100: 6674 2773 2069 6e73 7472 756d 656e 7473  ft's instruments
+00001110: 2e0d 0a2d 2054 6861 6e6b 205f 5b43 4d41  ...- Thank _[CMA
+00001120: 5f32 3430 3150 545d 2868 7474 7073 3a2f  _2401PT](https:/
+00001130: 2f67 6974 6875 622e 636f 6d2f 434d 4132  /github.com/CMA2
+00001140: 3430 3150 5429 5f20 666f 7220 4244 5857  401PT)_ for BDXW
+00001150: 6f72 6b53 686f 7020 666f 7220 7265 6665  orkShop for refe
+00001160: 7265 6e63 6520 6f66 2074 6865 202e 6264  rence of the .bd
+00001170: 7820 7374 7275 6374 7572 6527 7320 6f70  x structure's op
+00001180: 6572 6174 696f 6e2c 2061 6e64 2068 6973  eration, and his
+00001190: 2067 7569 6461 6e63 6520 696e 2073 6f6d   guidance in som
+000011a0: 6520 6173 7065 6374 7320 6f66 206f 7572  e aspects of our
+000011b0: 2064 6576 656c 6f70 6d65 6e74 2e0d 0a2d   development...-
+000011c0: 2054 6861 6e6b 205f 5b44 6973 6c69 6e6b   Thank _[Dislink
+000011d0: 2053 666f 727a 615d 2868 7474 7073 3a2f   Sforza](https:/
+000011e0: 2f67 6974 6875 622e 636f 6d2f 4469 736c  /github.com/Disl
+000011f0: 696e 6b29 20e2 809c e696 ade8 8194 c2b7  ink) ...........
+00001200: e696 afe7 a68f e5b0 94e6 898e e280 9d5f  ..............._
+00001210: 205c 3c51 5131 3630 3035 3135 3331 345c   \<QQ1600515314\
+00001220: 3e20 666f 7220 6869 7320 6d69 6469 2061  > for his midi a
+00001230: 6e61 6c79 7369 7320 616c 676f 7269 7468  nalysis algorith
+00001240: 6d20 6272 6f75 6768 7420 746f 2075 732c  m brought to us,
+00001250: 2077 6520 6861 6420 6164 6170 7465 6420   we had adapted 
+00001260: 6974 2061 6e64 206d 6164 6520 6974 2061  it and made it a
+00001270: 7070 6c69 6564 2069 6e20 6f6e 6520 6f66  pplied in one of
+00001280: 206f 7572 2077 6f72 6b69 6e67 206d 6574   our working met
+00001290: 686f 643b 2041 6c73 6f2c 2074 6861 6e6b  hod; Also, thank
+000012a0: 2068 696d 2066 6f72 2074 6865 205b 5765   him for the [We
+000012b0: 6243 6f6e 7665 7274 6f72 5d28 6874 7470  bConvertor](http
+000012c0: 733a 2f2f 6469 736c 696e 6b2e 6769 7468  s://dislink.gith
+000012d0: 7562 2e69 6f2f 6d69 6469 3262 6478 2f29  ub.io/midi2bdx/)
+000012e0: 2077 6869 6368 2062 726f 7567 6874 2075   which brought u
+000012f0: 7320 736f 206d 7563 6820 7072 6573 7375  s so much pressu
+00001300: 7265 2061 6e64 2070 6f77 6572 2074 6f20  re and power to 
+00001310: 6465 7665 6c6f 7020 6173 2077 656c 6c20  develop as well 
+00001320: 6173 2075 7064 6174 6520 6f75 7220 7072  as update our pr
+00001330: 6f6a 6563 7473 2062 6574 7465 722c 2069  ojects better, i
+00001340: 6e73 7465 6164 206f 6620 6c6f 6166 206f  nstead of loaf o
+00001350: 6e20 6f75 7220 7072 6f6a 6563 742e 2057  n our project. W
+00001360: 6520 686f 7065 2068 6520 6361 6e20 6765  e hope he can ge
+00001370: 7420 696e 746f 2061 2067 6f6f 6420 756e  t into a good un
+00001380: 6976 6572 7369 7479 2061 7320 6865 2077  iversity as he w
+00001390: 616e 7474 6564 2074 6f21 0d0a 2d20 5468  antted to!..- Th
+000013a0: 616e 6b20 5f54 6f75 6368 20e2 809c e581  ank _Touch .....
+000013b0: b7e5 9083 e280 9d5f 5c3c 5151 3137 3933  ......._\<QQ1793
+000013c0: 3533 3731 3634 5c3e 2066 6f72 2073 7570  537164\> for sup
+000013d0: 706f 7274 206f 6620 6465 6275 6767 696e  port of debuggin
+000013e0: 6720 616e 6420 7465 7374 696e 6720 7072  g and testing pr
+000013f0: 6f67 7261 6d20 616e 6420 616c 676f 7269  ogram and algori
+00001400: 7468 6d2c 2061 7320 7765 6c6c 2068 6973  thm, as well his
+00001410: 2f68 6572 2073 7567 6765 7374 696f 6e73  /her suggestions
+00001420: 2074 6f20 7468 6520 696d 7072 6f76 656d   to the improvem
+00001430: 656e 7420 6f66 206f 7572 2070 726f 6a65  ent of our proje
+00001440: 6374 0d0a 2d20 5468 616e 6b20 5f4d 6f6e  ct..- Thank _Mon
+00001450: 6f5f 5c3c 5151 3733 3838 3933 3038 375c  o_\<QQ738893087\
+00001460: 3e20 666f 7220 7265 706f 7274 696e 6720  > for reporting 
+00001470: 7072 6f62 6c65 6d73 2077 6869 6c65 2069  problems while i
+00001480: 6e73 7461 6c6c 696e 670d 0a2d 2054 6861  nstalling..- Tha
+00001490: 6e6b 205f 416d 6d65 6c69 6120 e280 9ce8  nk _Ammelia ....
+000014a0: 89be e7b1 b3e5 88a9 e4ba 9ae2 809d 5f5c  .............._\
+000014b0: 3c51 5132 3833 3833 3334 3633 375c 3e20  <QQ2838334637\> 
+000014c0: 666f 7220 7572 6769 6e67 2075 7320 746f  for urging us to
+000014d0: 2064 6576 656c 6f70 206e 6577 2066 756e   develop new fun
+000014e0: 6374 696f 6e73 2c20 616e 6420 7075 7420  ctions, and put 
+000014f0: 666f 7277 6172 6420 6120 6c6f 7420 6f66  forward a lot of
+00001500: 2065 7863 656c 6c65 6e74 2073 7567 6765   excellent sugge
+00001510: 7374 696f 6e73 2066 6f72 206e 6577 2066  stions for new f
+00001520: 756e 6374 696f 6e73 2c20 6173 2077 656c  unctions, as wel
+00001530: 6c20 6173 2074 6865 2042 4458 2066 696c  l as the BDX fil
+00001540: 6527 7320 696d 706f 7274 696e 6720 7465  e's importing te
+00001550: 7374 2073 7570 706f 7274 2070 726f 7669  st support provi
+00001560: 6465 642c 2077 6869 6368 2068 6173 2067  ded, which has g
+00001570: 6976 656e 2061 206c 6f74 206f 6620 7072  iven a lot of pr
+00001580: 6163 7469 6361 6c20 7468 656f 7265 7469  actical theoreti
+00001590: 6361 6c20 7375 7070 6f72 7420 666f 7220  cal support for 
+000015a0: 6f75 7220 6e65 7720 5374 7275 6374 7572  our new Structur
+000015b0: 6520 4765 6e65 7261 7469 6e67 2041 6c67  e Generating Alg
+000015c0: 6f72 6974 686d 0d0a 2d20 5468 616e 6b20  orithm..- Thank 
+000015d0: 5f5b e7a5 9ee7 bebd 5d28 6874 7470 733a  _[......](https:
+000015e0: 2f2f 6769 7465 652e 636f 6d2f 736e 6f77  //gitee.com/snow
+000015f0: 796b 616d 6929 20e2 809c 5b53 6e6f 7779  ykami) ...[Snowy
+00001600: 4b61 6d69 5d28 6874 7470 733a 2f2f 6769  Kami](https://gi
+00001610: 7468 7562 2e63 6f6d 2f73 6e6f 7779 6669  thub.com/snowyfi
+00001620: 7265 666c 7929 e280 9d5f 2066 6f72 2073  refly)..._ for s
+00001630: 7570 706f 7274 696e 6720 616e 6420 7072  upporting and pr
+00001640: 6f6d 6f74 696e 6720 6f75 7220 7072 6f6a  omoting our proj
+00001650: 6563 742e 2048 6f70 6520 6865 2063 6f75  ect. Hope he cou
+00001660: 6c64 2067 6574 2069 6e74 6f20 6120 676f  ld get into a go
+00001670: 6f64 2075 6e69 7665 7273 6974 7921 0d0a  od university!..
+00001680: 2d20 5468 616e 6b20 2a2a e68c 87e4 bba4  - Thank **......
+00001690: e5b8 885c 5fe8 8ba6 e58a 9be6 8095 2070  ...\_......... p
+000016a0: 6c61 796a 7569 6365 3132 332a 2a5c 3c51  layjuice123**\<Q
+000016b0: 5132 3430 3636 3731 3937 5c3e 2066 6f72  Q240667197\> for
+000016c0: 2066 696e 6469 6e67 2062 7567 7320 7769   finding bugs wi
+000016d0: 7468 696e 206f 7572 2063 6f64 652c 2061  thin our code, a
+000016e0: 6e64 206e 6f74 6963 6564 2075 7320 746f  nd noticed us to
+000016f0: 2072 6570 6169 7220 6120 6269 6720 7072   repair a big pr
+00001700: 6f62 6c65 6d2e 0d0a 2d20 5468 616e 6b20  oblem...- Thank 
+00001710: 2a2a e99b b7e9 9c86 2a2a 5c3c 5151 3335  **......**\<QQ35
+00001720: 3535 3236 3835 3139 5c3e 2066 6f72 2068  55268519\> for h
+00001730: 6973 2061 6e6e 6f79 696e 6720 616e 6420  is annoying and 
+00001740: 7072 6f76 6f6b 696e 6720 6f70 6572 6174  provoking operat
+00001750: 696f 6e73 2077 6869 6368 206d 6179 2061  ions which may a
+00001760: 7761 6b65 2073 6f6d 6520 7072 6f62 6c65  wake some proble
+00001770: 6d73 2077 6974 6869 6e20 7468 6520 7072  ms within the pr
+00001780: 6f67 7261 6d20 6279 2063 6861 6e63 6520  ogram by chance 
+00001790: 616e 6420 7265 6d69 6e64 696e 6720 7573  and reminding us
+000017a0: 2074 6f20 7265 7061 6972 2e0d 0a0d 0a3e   to repair.....>
+000017b0: 2054 6861 6e6b 7320 666f 7220 6120 6c6f   Thanks for a lo
+000017c0: 7420 6f66 2067 726f 7570 6d61 7465 7327  t of groupmates'
+000017d0: 2073 7570 706f 7274 2061 6e64 2068 656c   support and hel
+000017e0: 700d 0a3e 0d0a 3e20 4966 2079 6f75 2068  p..>..> If you h
+000017f0: 6176 6520 6769 7665 6e20 636f 6e74 7269  ave given contri
+00001800: 6275 7469 6f6e 2062 7574 2068 6176 656e  bution but haven
+00001810: 2774 2062 6565 6e20 696e 2074 6865 206c  't been in the l
+00001820: 6973 742c 2070 6c65 6173 6520 636f 6e74  ist, please cont
+00001830: 6163 7420 7573 210d 0a0d 0a23 2320 436f  act us!....## Co
+00001840: 6e74 6163 7420 5573 f09f 939e 0d0a 0d0a  ntact Us........
+00001850: 4d65 6574 2070 726f 626c 656d 733f 2057  Meet problems? W
+00001860: 656c 636f 6d65 2074 6f20 6769 7665 206f  elcome to give o
+00001870: 7574 2079 6f75 7220 6973 7375 6520 5b68  ut your issue [h
+00001880: 6572 655d 2868 7474 7073 3a2f 2f67 6974  ere](https://git
+00001890: 6875 622e 636f 6d2f 4569 6c6c 6573 5761  hub.com/EillesWa
+000018a0: 6e2f 4d75 7369 6372 6561 7465 722f 6973  n/Musicreater/is
+000018b0: 7375 6573 2f6e 6577 2921 0d0a 0d0a 5761  sues/new)!....Wa
+000018c0: 6e74 2074 6f20 6765 7420 696e 2063 6f6e  nt to get in con
+000018d0: 7461 6374 206f 6620 6465 7665 6c6f 7065  tact of develope
+000018e0: 7273 3f20 5765 6c63 6f6d 6520 746f 206a  rs? Welcome to j
+000018f0: 6f69 6e20 6f75 7220 5b43 6861 7420 5151  oin our [Chat QQ
+00001900: 2067 726f 7570 5d28 6874 7470 733a 2f2f   group](https://
+00001910: 6a71 2e71 712e 636f 6d2f 3f5f 7776 3d31  jq.qq.com/?_wv=1
+00001920: 3032 3726 6b3d 6870 6552 7872 5972 292e  027&k=hpeRxrYr).
+00001930: 0d0a 0d0a 2d2d 2d0d 0a0d 0a4e 4f54 2041  ....---....NOT A
+00001940: 4e20 4f46 4649 4349 414c 204d 494e 4543  N OFFICIAL MINEC
+00001950: 5241 4654 2050 524f 4455 4354 2e0d 0a0d  RAFT PRODUCT....
+00001960: 0a4e 4f54 2041 5050 524f 5645 4420 4259  .NOT APPROVED BY
+00001970: 204f 5220 4153 534f 4349 4154 4544 2057   OR ASSOCIATED W
+00001980: 4954 4820 4d4f 4a41 4e47 204f 5220 4d49  ITH MOJANG OR MI
+00001990: 4352 4f53 4f46 542e 0d0a 0d0a 4e4f 5420  CROSOFT.....NOT 
+000019a0: 4150 5052 4f56 4544 2042 5920 4f52 2041  APPROVED BY OR A
+000019b0: 5353 4f43 4941 5445 4420 5749 5448 204e  SSOCIATED WITH N
+000019c0: 4554 4541 5345 2e0d 0a0d 0ae6 ada4 e9a1  ETEASE..........
+000019d0: b9e7 9bae e5b9 b6e9 9d9e e4b8 80e4 b8aa  ................
+000019e0: e5ae 98e6 96b9 20e3 808a e688 91e7 9a84  ...... .........
+000019f0: e4b8 96e7 958c e380 8bef bc88 5f4d 696e  ............_Min
+00001a00: 6563 7261 6674 5fef bc89 e9a1 b9e7 9bae  ecraft_.........
+00001a10: 0d0a 0d0a e6ad a4e9 a1b9 e79b aee4 b88d  ................
+00001a20: e99a b6e5 b19e e688 96e5 85b3 e881 94e4  ................
+00001a30: ba8e 204d 6f6a 616e 6720 5374 7564 696f  .. Mojang Studio
+00001a40: 7320 e688 9620 e5be aee8 bdaf 0d0a 0d0a  s ... ..........
+00001a50: e6ad a4e9 a1b9 e79b aee4 baa6 e4b8 8de9  ................
+00001a60: 9ab6 e5b1 9ee6 8896 e585 b3e8 8194 e4ba  ................
+00001a70: 8e20 e7bd 91e6 9893 20e7 9bb8 e585 b30d  . ...... .......
+00001a80: 0a0d 0ae2 809c 4d69 6e65 6372 6166 74e2  ......Minecraft.
+00001a90: 809d e698 af20 4d6f 6a61 6e67 2053 796e  ..... Mojang Syn
+00001aa0: 6572 6769 6573 2041 4220 e79a 84e5 9586  ergies AB ......
+00001ab0: e6a0 87ef bc8c e6ad a4e9 a1b9 e79b aee4  ................
+00001ac0: b8ad e689 80e6 9c89 e5af b9e4 ba8e e280  ................
+00001ad0: 9ce6 8891 e79a 84e4 b896 e795 8ce2 809d  ................
+00001ae0: e380 81e2 809c 4d69 6e65 6372 6166 74e2  ......Minecraft.
+00001af0: 809d e7ad 89e7 9bb8 e585 b3e7 a7b0 e591  ................
+00001b00: bce5 9d87 e4b8 bae5 bc95 e794 a8e6 80a7  ................
+00001b10: e4bd bfe7 94a8 0d0a 0d0a 2d20 e4b8 8ae6  ..........- ....
+00001b20: 9687 e68f 90e5 8f8a e79a 8420 e7bd 91e6  ........... ....
+00001b30: 9893 20e5 85ac e58f b8ef bc8c e68c 87e4  .. .............
+00001b40: bba3 e79a 84e6 98af e59c a8e4 b8ad e59b  ................
+00001b50: bde5 a4a7 e999 86e8 bf90 e890 a5e3 808a  ................
+00001b60: e688 91e7 9a84 e4b8 96e7 958c efbc 9ae4  ................
+00001b70: b8ad e59b bde7 8988 e380 8be7 9a84 e4b8  ................
+00001b80: 8ae6 b5b7 e7bd 91e4 b98b e698 93e7 bd91  ................
+00001b90: e7bb 9ce7 a791 e68a 80e5 8f91 e5b1 95e6  ................
+00001ba0: 9c89 e999 90e5 85ac e58f b80d 0a0d 0a0d  ................
+00001bb0: 0a5b 4269 6c69 6269 6c69 3a20 4569 6c6c  .[Bilibili: Eill
+00001bc0: 6573 5d3a 2068 7474 7073 3a2f 2f69 6d67  es]: https://img
+00001bd0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+00001be0: 652f 4269 6c69 6269 6c69 2d25 4535 2538  e/Bilibili-%E5%8
+00001bf0: 3725 3843 2545 3425 4241 2539 3125 4539  7%8C%E4%BA%91%E9
+00001c00: 2538 3725 3931 2545 3725 4245 2542 462d  %87%91%E7%BE%BF-
+00001c10: 3030 4131 4537 3f73 7479 6c65 3d66 6f72  00A1E7?style=for
+00001c20: 2d74 6865 2d62 6164 6765 0d0a 5b42 696c  -the-badge..[Bil
+00001c30: 6962 696c 693a 2062 6741 7272 6179 5d3a  ibili: bgArray]:
+00001c40: 2068 7474 7073 3a2f 2f69 6d67 2e73 6869   https://img.shi
+00001c50: 656c 6473 2e69 6f2f 6261 6467 652f 4269  elds.io/badge/Bi
+00001c60: 6c69 6269 6c69 2d25 4538 2541 4625 4238  libili-%E8%AF%B8
+00001c70: 2545 3825 3931 2539 4225 4534 2542 4125  %E8%91%9B%E4%BA%
+00001c80: 4145 2545 3425 4238 2538 4525 4535 2538  AE%E4%B8%8E%E5%8
+00001c90: 3525 4142 2545 3525 3844 2541 3625 4539  5%AB%E5%8D%A6%E9
+00001ca0: 2539 3825 4235 2d30 3041 3145 373f 7374  %98%B5-00A1E7?st
+00001cb0: 796c 653d 666f 722d 7468 652d 6261 6467  yle=for-the-badg
+00001cc0: 650d 0a5b 436f 6465 5374 796c 653a 2062  e..[CodeStyle: b
+00001cd0: 6c61 636b 5d3a 2068 7474 7073 3a2f 2f69  lack]: https://i
+00001ce0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+00001cf0: 6467 652f 636f 6465 2532 3073 7479 6c65  dge/code%20style
+00001d00: 2d62 6c61 636b 2d31 3231 3131 302e 7376  -black-121110.sv
+00001d10: 673f 7374 796c 653d 666f 722d 7468 652d  g?style=for-the-
+00001d20: 6261 6467 650d 0a5b 7079 7468 6f6e 5d3a  badge..[python]:
+00001d30: 2068 7474 7073 3a2f 2f69 6d67 2e73 6869   https://img.shi
+00001d40: 656c 6473 2e69 6f2f 6261 6467 652f 7079  elds.io/badge/py
+00001d50: 7468 6f6e 2d33 2e38 2d41 4237 3046 463f  thon-3.8-AB70FF?
+00001d60: 7374 796c 653d 666f 722d 7468 652d 6261  style=for-the-ba
+00001d70: 6467 650d 0a5b 7265 6c65 6173 655d 3a20  dge..[release]: 
+00001d80: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00001d90: 6c64 732e 696f 2f67 6974 6875 622f 762f  lds.io/github/v/
+00001da0: 7265 6c65 6173 652f 4569 6c6c 6573 5761  release/EillesWa
+00001db0: 6e2f 4d75 7369 6372 6561 7465 723f 7374  n/Musicreater?st
+00001dc0: 796c 653d 666f 722d 7468 652d 6261 6467  yle=for-the-badg
+00001dd0: 650d 0a5b 6c69 6365 6e73 655d 3a20 6874  e..[license]: ht
+00001de0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00001df0: 732e 696f 2f62 6164 6765 2f4c 6963 656e  s.io/badge/Licen
+00001e00: 6365 2d41 7061 6368 652d 3232 3842 3232  ce-Apache-228B22
+00001e10: 3f73 7479 6c65 3d66 6f72 2d74 6865 2d62  ?style=for-the-b
+00001e20: 6164 6765 0d0a                           adge..
```

### Comparing `Musicreater-1.1.0/setup.py` & `Musicreater-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 import setuptools
 import Musicreater
 
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     dependences = fh.read().strip().split("\n")
 
-with open("README.md", "r", encoding="utf-8") as fh:
+with open("README_EN.md", "r", encoding="utf-8") as fh:
     long_description = fh.read().replace(
         "./docs/", "https://github.com/TriM-Organization/Musicreater/blob/master/docs/"
     )
 
 setuptools.setup(
     name="Musicreater",
     version=Musicreater.__version__,
```

