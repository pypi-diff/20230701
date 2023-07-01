# Comparing `tmp/LyricLib-0.0.3.1.tar.gz` & `tmp/LyricLib-0.0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LyricLib-0.0.3.1.tar", last modified: Sat May 27 11:55:59 2023, max compression
+gzip compressed data, was "LyricLib-0.0.3.2.tar", last modified: Sat Jul  1 14:32:02 2023, max compression
```

## Comparing `LyricLib-0.0.3.1.tar` & `LyricLib-0.0.3.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 11:55:59.032659 LyricLib-0.0.3.1/
--rw-rw-rw-   0        0        0    12940 2023-05-27 11:50:34.000000 LyricLib-0.0.3.1/LICENSE.md
-drwxrwxrwx   0        0        0        0 2023-05-27 11:55:59.018706 LyricLib-0.0.3.1/LyricLib/
--rw-rw-rw-   0        0        0     1261 2023-05-01 02:54:44.000000 LyricLib-0.0.3.1/LyricLib/LICENSE(lrc-parser).md
--rw-rw-rw-   0        0        0      631 2023-05-27 11:50:34.000000 LyricLib-0.0.3.1/LyricLib/__init__.py
--rw-rw-rw-   0        0        0     1241 2023-05-01 02:54:44.000000 LyricLib-0.0.3.1/LyricLib/constants.py
--rw-rw-rw-   0        0        0     1053 2023-05-01 02:54:44.000000 LyricLib-0.0.3.1/LyricLib/exceptions.py
--rw-rw-rw-   0        0        0     7737 2023-05-27 11:50:34.000000 LyricLib-0.0.3.1/LyricLib/main.py
--rw-rw-rw-   0        0        0    11222 2023-05-27 11:50:34.000000 LyricLib-0.0.3.1/LyricLib/subclass.py
-drwxrwxrwx   0        0        0        0 2023-05-27 11:55:59.026677 LyricLib-0.0.3.1/LyricLib.egg-info/
--rw-rw-rw-   0        0        0     2753 2023-05-27 11:55:58.000000 LyricLib-0.0.3.1/LyricLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      404 2023-05-27 11:55:58.000000 LyricLib-0.0.3.1/LyricLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 11:55:58.000000 LyricLib-0.0.3.1/LyricLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-27 11:55:58.000000 LyricLib-0.0.3.1/LyricLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       41 2023-05-07 03:03:51.000000 LyricLib-0.0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2753 2023-05-27 11:55:59.031668 LyricLib-0.0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1801 2023-05-27 11:50:34.000000 LyricLib-0.0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 11:55:59.029667 LyricLib-0.0.3.1/docs/
--rw-rw-rw-   0        0        0     6577 2023-05-01 02:54:44.000000 LyricLib-0.0.3.1/docs/Lrc文件格式.md
--rw-rw-rw-   0        0        0      533 2023-05-27 11:50:34.000000 LyricLib-0.0.3.1/docs/开发日志.TXT
--rw-rw-rw-   0        0        0       42 2023-05-27 11:55:59.032659 LyricLib-0.0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1354 2023-05-07 03:03:51.000000 LyricLib-0.0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 14:32:02.883178 LyricLib-0.0.3.2/
+-rw-rw-rw-   0        0        0    12940 2023-05-27 11:50:34.000000 LyricLib-0.0.3.2/LICENSE.md
+drwxrwxrwx   0        0        0        0 2023-07-01 14:32:02.872215 LyricLib-0.0.3.2/LyricLib/
+-rw-rw-rw-   0        0        0     1261 2023-05-01 02:54:44.000000 LyricLib-0.0.3.2/LyricLib/LICENSE(lrc-parser).md
+-rw-rw-rw-   0        0        0      931 2023-07-01 14:31:54.000000 LyricLib-0.0.3.2/LyricLib/__init__.py
+-rw-rw-rw-   0        0        0     1241 2023-07-01 14:08:38.000000 LyricLib-0.0.3.2/LyricLib/constants.py
+-rw-rw-rw-   0        0        0     1307 2023-07-01 14:08:38.000000 LyricLib-0.0.3.2/LyricLib/exceptions.py
+-rw-rw-rw-   0        0        0     7737 2023-05-27 11:50:34.000000 LyricLib-0.0.3.2/LyricLib/main.py
+-rw-rw-rw-   0        0        0    11340 2023-07-01 14:08:38.000000 LyricLib-0.0.3.2/LyricLib/subclass.py
+drwxrwxrwx   0        0        0        0 2023-07-01 14:32:02.879191 LyricLib-0.0.3.2/LyricLib.egg-info/
+-rw-rw-rw-   0        0        0     2753 2023-07-01 14:32:02.000000 LyricLib-0.0.3.2/LyricLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      419 2023-07-01 14:32:02.000000 LyricLib-0.0.3.2/LyricLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 14:32:02.000000 LyricLib-0.0.3.2/LyricLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-01 14:32:02.000000 LyricLib-0.0.3.2/LyricLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       41 2023-05-07 03:03:51.000000 LyricLib-0.0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2753 2023-07-01 14:32:02.883178 LyricLib-0.0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1801 2023-05-27 11:50:34.000000 LyricLib-0.0.3.2/README.md
+-rw-rw-rw-   0        0        0     1989 2023-07-01 14:08:38.000000 LyricLib-0.0.3.2/README_EN.md
+drwxrwxrwx   0        0        0        0 2023-07-01 14:32:02.881185 LyricLib-0.0.3.2/docs/
+-rw-rw-rw-   0        0        0     7504 2023-07-01 14:08:38.000000 LyricLib-0.0.3.2/docs/Lrc文件格式.md
+-rw-rw-rw-   0        0        0      698 2023-07-01 14:08:38.000000 LyricLib-0.0.3.2/docs/开发日志.TXT
+-rw-rw-rw-   0        0        0       42 2023-07-01 14:32:02.883178 LyricLib-0.0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1354 2023-05-07 03:03:51.000000 LyricLib-0.0.3.2/setup.py
```

### Comparing `LyricLib-0.0.3.1/LICENSE.md` & `LyricLib-0.0.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `LyricLib-0.0.3.1/LyricLib/LICENSE(lrc-parser).md` & `LyricLib-0.0.3.2/LyricLib/LICENSE(lrc-parser).md`

 * *Files identical despite different names*

### Comparing `LyricLib-0.0.3.1/LyricLib/constants.py` & `LyricLib-0.0.3.2/LyricLib/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,18 +17,18 @@
     "au": "LyricAuthor",
     "length": "Length",
     "by": "Recorder",
     "re": "Editor",
     "ve": "Version",
     "offset": "Offset",
 }
-'''LRC歌词ID标签转元信息名称'''
+"""LRC歌词ID标签转元信息名称"""
 
 STABLE_LRC_TIME_FORMAT_STYLE = r"{mm}:{ss}.{xx}"
-'''标准LRC时间格式'''
+"""标准LRC时间格式"""
 
 # 正则表达式
 
 # 标签匹配模式
 LRC_TAG_PATTERN = r"\[.*?\]"
 
 # 时间戳标签匹配模式
```

### Comparing `LyricLib-0.0.3.1/LyricLib/exceptions.py` & `LyricLib-0.0.3.2/LyricLib/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,49 @@
-
-
 class LyricBaseException(Exception):
     """歌词库的所有错误均继承于此"""
 
     def __init__(self, *args):
         """歌词库的所有错误均继承于此"""
         super().__init__(*args)
 
     def aowu(
-            self,
+        self,
     ):
         for i in self.args:
             print(i + "嗷呜！")
 
     def crash_it(self):
         raise self
 
 
-
-
 class LrcDestroyedError(LyricBaseException):
     """Lrc文件损坏"""
 
     def __init__(self, *args):
         """Lrc文件损坏"""
         super().__init__("Lrc文件损坏", *args)
 
 
-
 class TimeTooPreciseError(LyricBaseException):
     """时间过于精确"""
 
     def __init__(self, *args):
         """时间过于精确"""
         super().__init__("时间过于精确", *args)
 
 
 class WordTagError(LyricBaseException):
     """字词标签错误"""
 
     def __init__(self, words_less_than_tags: bool = True, *args):
         """字词标签未一一对应"""
-        super().__init__("字词标签错误：字词{}标签个数".format("小于" if words_less_than_tags else "大于"), *args)
+        super().__init__(
+            "字词标签错误：字词{}标签个数".format("小于" if words_less_than_tags else "大于"), *args
+        )
+
+
+class TimeTagError(LyricBaseException):
+    """时间标签错误"""
 
+    def __init__(self, sth: str = "", *args):
+        """未匹配到时间标签"""
+        super().__init__("无法在 {} 中匹配时间标签。".format(sth), *args)
```

### Comparing `LyricLib-0.0.3.1/LyricLib/main.py` & `LyricLib-0.0.3.2/LyricLib/main.py`

 * *Files identical despite different names*

### Comparing `LyricLib-0.0.3.1/LyricLib/subclass.py` & `LyricLib-0.0.3.2/LyricLib/subclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 from dataclasses import dataclass
 from enum import Enum
-from typing import Dict, List, Union
+from typing import Dict, List, Union, Tuple
 
 from .constants import *
 from .exceptions import *
 
 
 class TagType(Enum):
     """标签类型类"""
@@ -13,15 +13,15 @@
     ID = 0  # ID标签
     TIME = 1  # 时间戳标签
     UNKNOWN = 2  # 未知标签
 
 
 @dataclass(init=False)
 class TimeStamp:
-    """时间类"""
+    """时间戳类"""
 
     hours: int
     minutes: int
     seconds: int
     microseconds: int
 
     def __init__(
@@ -67,15 +67,15 @@
             return cls(
                 *cls.parse_lrc_time_tag(time_tag_str.replace("[", "").replace("]", ""))
             )
         except TimeTooPreciseError:
             raise LrcDestroyedError("时间标签出现错误: {}".format(time_tag_str), time_tag_str)
 
     @staticmethod
-    def parse_lrc_time_tag(time_tag_str):
+    def parse_lrc_time_tag(time_tag_str) -> Tuple[int,...]:
         """
         将LRC文件的字符串格式的时间戳解析为 时、分、秒、毫秒
 
         Parameters
         ----------
         time_tag_str: int
             时间戳字符串
@@ -83,15 +83,18 @@
         Returns
         -------
 
         tuple(int时, int分, int秒, int毫秒)
         """
 
         m = re.match(LRC_TIME_PATTERN, time_tag_str)
-        time_parts = m.groupdict()
+        if m:
+            time_parts = m.groupdict()
+        else:
+            raise TimeTagError(time_tag_str)
 
         # 毫秒
         ms = 0
         if time_parts["p4"] is not None:
             # ".xxx秒" ---> 毫秒
             ms = int(float(time_parts["p4"]) * 1000)
 
@@ -120,45 +123,45 @@
 
     @property
     def get_hours(self) -> int:
         """时间戳中的小时部分"""
         return self.hours
 
     @property
-    def in_hours(self) -> int:
+    def in_hours(self) -> float:
         """以小时为单位的时间戳"""
         return (
             self.hours
             + self.minutes / 60
             + self.seconds / 360
             + self.microseconds / 360000
         )
 
     @property
     def get_minutes(self) -> int:
         """时间戳中的分钟部分"""
         return self.minutes
 
     @property
-    def in_minutes(self) -> int:
+    def in_minutes(self) -> float:
         """以分钟为单位的时间戳"""
         return (
             self.hours * 60
             + self.minutes
             + self.seconds / 60
             + self.microseconds / 60000
         )
 
     @property
     def get_seconds(self) -> int:
         """时间戳中的秒数部分"""
         return self.seconds
 
     @property
-    def in_seconds(self) -> int:
+    def in_seconds(self) -> float:
         """以秒为单位的时间戳"""
         return (
             self.hours * 360
             + self.minutes * 60
             + self.seconds
             + self.microseconds / 1000
         )
@@ -275,15 +278,15 @@
                 TimeStamp.from_lrc_time_tag(time_tag_str=time_str_list[i])
             ] = word_list[i]
             # print("=====")
         return cls(sentence, word_extension)
 
     def __str__(self) -> str:
         if self.word_extension:
-            "".join(
+            return "".join(
                 [
                     r"<{}>{}".format(time.to_lrc_str(), word)
                     for time, word in self.word_extension.items()
                 ]
             )
         else:
             return self.whole_context
```

### Comparing `LyricLib-0.0.3.1/LyricLib.egg-info/PKG-INFO` & `LyricLib-0.0.3.2/LyricLib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LyricLib
-Version: 0.0.3.1
+Version: 0.0.3.2
 Summary: 歌词的处理库
 Home-page: https://github.com/TriM-Organization/Lyric
 Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `LyricLib-0.0.3.1/PKG-INFO` & `LyricLib-0.0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LyricLib
-Version: 0.0.3.1
+Version: 0.0.3.2
 Summary: 歌词的处理库
 Home-page: https://github.com/TriM-Organization/Lyric
 Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `LyricLib-0.0.3.1/README.md` & `LyricLib-0.0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `LyricLib-0.0.3.1/docs/Lrc文件格式.md` & `LyricLib-0.0.3.2/docs/Lrc文件格式.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# LRC文件格式
+# LRC 文件格式
 
 非常感谢 [thecasttim](https://gitee.com/thecasttim) 的 [LrcParser](https://gitee.com/thecasttim/lrc-parser) 项目，为此项目提供了非常大的参考。可以说，本项目就是基于它进行了进一步的修改而开发的。本文件基于其编写的[README.md](https://gitee.com/thecasttim/lrc-parser/blob/master/README.md)而改写而来。
 
-LRC是英文**L**y**r**i**c**，即歌词的缩写，被用做歌词文件的扩展名。以`.lrc`为扩展名的歌词文件可以在各类有相关支持的数码播放器中与所播放之歌曲同步显示歌词。此类文件是一种包含由“标签（tag）”所标记的时间信息的、基于纯文本的歌词专用格式。大部分MP3播放器显示歌词的方法亦为LRC格式的歌词文件，此类文件也是当前网络上最流行的一种歌词格式。
+LRC 是英文**L**y**r**i**c**，即歌词的缩写，被用做歌词文件的扩展名。以`.lrc`为扩展名的歌词文件可以在各类有相关支持的数码播放器中与所播放之歌曲同步显示歌词。此类文件是一种包含由“标签（tag）”所标记的时间信息的、基于纯文本的歌词专用格式。大部分 MP3 播放器显示歌词的方法亦为 LRC 格式的歌词文件，此类文件也是当前网络上最流行的一种歌词格式。
 
 ## 元素
 
-LRC文件以 **标签** （Tag）来进行控制整个歌词整体信息。标签一共有两种：*ID标签*（ID-Tag） 和 *时间标签*（Time-Tag）
+LRC 文件以 **标签** （Tag）来进行控制整个歌词整体信息。标签一共有两种：_ID 标签_（ID-Tag） 和 _时间标签_（Time-Tag）
 
-### **ID标签**
+### **ID 标签**
 
-LRC格式歌词的**ID标签**存储了歌曲的元信息。其可能位于其他标签之前，亦可以在任意位置，在这里，我建议在编辑文件时，把**有关歌曲信息的ID标签**均置于整个文件的最前端，因为部分播放器可能采用的是惰性文件读取的方法读词，即按行读取歌词文件，此时将无法正常显示相关歌曲信息。
+LRC 格式歌词的**ID 标签**存储了歌曲的元信息。其可能位于其他标签之前，亦可以在任意位置，在这里，我建议在编辑文件时，把**有关歌曲信息的 ID 标签**均置于整个文件的最前端，因为部分播放器可能采用的是惰性文件读取的方法读词，即按行读取歌词文件，此时将无法正常显示相关歌曲信息。
 
-标准的LRC歌词文件中，**ID标签**包括：
+标准的 LRC 歌词文件中，**ID 标签**包括：
 
 ```wiki
 [ar:演唱者]
 [al:本歌所在的专辑]
 [ti:本歌的标题]
 [au:歌词作者]
 [length:本歌的长度]
@@ -37,43 +37,44 @@
 [by:金羿]
 [re:Python Lyric]
 [ve:0.0.1]
 ```
 
 ### **时间标签**
 
-LRC具有**单句标签**（简单格式）和**字词标签**（增强格式）两种时间标记方式，前者是必须的，后者是可拓展的。在时间标签所标记处，是要显示的歌词。
+LRC 具有**单句标签**（简单格式）和**字词标签**（增强格式）两种时间标记方式，前者是必须的，后者是可拓展的。在时间标签所标记处，是要显示的歌词。
 
-同上述ID标签的理，尽量按照时间顺序排序歌词，你永远也无法预测下一个播放器会偷怎样的懒。
+同上述 ID 标签的理，尽量按照时间顺序排序歌词，你永远也无法预测下一个播放器会偷怎样的懒。
 
-***单句标签***即每一个时间标签对应的是一行歌词，其格式可以为：
+**_单句标签_**即每一个时间标签对应的是一行歌词，其格式可以为：
 
 ```wiki
 [mm:ss.fff]歌词
 [mm:ss.xx]歌词
 [hh:mm:ss]歌词
 [hh:mm:ss.fff]歌词
 [hh:mm:ss.xx]歌词
 [mm:ss]歌词
 [mm:ss.xx][mm:ss.xx][mm:ss.xx]重复出现的歌词
 ```
 
 其中，正规的写法是前五个，最正规的是第一个，形如 **[mm:ss.fff]** 的是时间标签，**歌词** 为显示的单句歌词。在部分编辑器中，无需精确时间时，会省略最后的`xx`部分，但这不是正规写法。在时间标签中 **hh** 是小时数，**mm** 为分钟数, **ss** 为秒数，**fff** 和 **xx** 所表示的都是精确的时间数值，单位不同，详见下表。
 
-在上面示例中的最后一个出现重复的歌词，那么说明这一行歌词在前面n个标签声明的时间点都有出现，虽然这是一个节省文件大小的好方法，但是现在都*2023*年了，省这几个字节有必要吗？而且这也是一种不规范的写法，**尽量避免**。
+在上面示例中的最后一个出现重复的歌词，那么说明这一行歌词在前面 n 个标签声明的时间点都有出现，虽然这是一个节省文件大小的好方法，但是现在都*2023*年了，省这几个字节有必要吗？而且这也是一种不规范的写法，**尽量避免**。
 
-|标记|说明|单位|
-|---|---|---|
-|**hh**|距离歌曲开始时的小时数，最大为99，不知道有没有劣质的播放器会有超限的情况，但是我猜一首歌唱九十多小时的人是不存在的；连电影字幕也不可能吧。|**时**|
-|**mm**|距离歌曲开始时的分钟数，当不存在第一个**hh**参数时，最大为99，不知道有没有劣质的播放器会有超限的情况，但是我猜一首歌唱一个半多小时的人是不存在的；除非你用LRC文件来存的是电影字幕。|**分**|
-|**ss**|距离当前分钟开始时的秒数，最大为59，部分劣质的编辑器会在60的边界反复横跳。|**秒**|
-|**xx**|距离当前秒开始时的百分之一秒数，最大为99，一定不能超限！否则就是**fff**标记了。|**十毫秒** 或曰 **百分之一秒**|
-|**fff**|距离当前秒开始时的毫秒数，最大为999，同理，鬼知道有没有超限的情况，但是咱写的时候千万别乱来啊。|**毫秒**|
+| 标记    | 说明                                                                                                                                                                                   | 单位                           |
+| ------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------ |
+| **hh**  | 距离歌曲开始时的小时数，最大为 99，不知道有没有劣质的播放器会有超限的情况，但是我猜一首歌唱九十多小时的人是不存在的；连电影字幕也不可能吧。                                            | **时**                         |
+| **mm**  | 距离歌曲开始时的分钟数，当不存在第一个**hh**参数时，最大为 99，不知道有没有劣质的播放器会有超限的情况，但是我猜一首歌唱一个半多小时的人是不存在的；除非你用 LRC 文件来存的是电影字幕。 | **分**                         |
+| **ss**  | 距离当前分钟开始时的秒数，最大为 59，部分劣质的编辑器会在 60 的边界反复横跳。                                                                                                          | **秒**                         |
+| **xx**  | 距离当前秒开始时的百分之一秒数，最大为 99，一定不能超限！否则就是**fff**标记了。                                                                                                       | **十毫秒** 或曰 **百分之一秒** |
+| **fff** | 距离当前秒开始时的毫秒数，最大为 999，同理，鬼知道有没有超限的情况，但是咱写的时候千万别乱来啊。                                                                                       | **毫秒**                       |
 
 例如：
+
 ```wiki
 [00:10.00] 第一行歌词（精确到十毫秒）
 [00:10.001] 第二行歌词（精确到一毫秒）
 [00:00:12.123] 第三行歌词（没必要的写法）
 [00:18] 第四行歌词（精确到一秒的不标准的写法）
 ...
 [mm:ss.xx] 最后一行歌词
@@ -81,60 +82,56 @@
 
 > 注意！
 >
 > 还有一种其实更不负责任的写法，它与小时的解析互相冲突了。就是 \[mm:ss:xx\]。
 >
 > 这里不做讨论了，这种再说就没意思了，大家懂的都懂。
 
-***歌词***部分，由于一些卡拉OK播放器的需要，可以设置男女对唱的标签：
+**_歌词_**部分，由于一些卡拉 OK 播放器的需要，可以设置男女对唱的标签：
 
-+ M：男
-+ F：女
-+ D：合唱
+- M：男
+- F：女
+- D：合唱
 
 例如：
+
 ```wiki
 [00:12.00]第一行歌词
 [00:15.00]F: 第二行歌词
 [00:16.50]M: 第三行歌词
 [00:17.20]第四行歌词
 [00:18.00]D: 第五行歌词
 [00:22.20] 第六行歌词
 ```
 
-***字词标签***是夹在歌词部分之中的，其对简单LRC格式进行了增强，可以标注单个词的出现时间。其格式应为：
+**_字词标签_**是夹在歌词部分之中的，其对简单 LRC 格式进行了增强，可以标注单个词的出现时间。其格式应为：
 
 ```wiki
 [mm:ss.xx]<mm:ss.xx>第1行第1个词<mm:ss.xx>第1行第2个词<mm:ss.xx> ... 第1行最后的词<mm:ss.xx>
 [mm:ss.xx]<mm:ss.xx>第2行第1个词<mm:ss.xx>第2行第2个词<mm:ss.xx> ... 第2最后的词<mm:ss.xx>
 ...
 [mm:ss.xx]<mm:ss.xx>最后1行第1个词<mm:ss.xx>最后1行第2个词<mm:ss.xx>...最后1行最后的词<mm:ss.xx>
 ```
+
 在每个词之后的**字词时间标签**标记了从上一个字词标签到本字词标签中的词所在歌曲中的出现时间，字词标签不可像前面我说过“**尽量避免**”的那个单句标签那样进行叠加使用。
 
 一个字词时间标签的格式，标准的长这样：`<mm:ss.xx>` 或者 `<mm:ss.fff>` 之类的，同理上面单句标签的理，就是把方括号换成了尖括号，或者说把英文中括号换成了一对大于小于号，不论怎么说就这样，当然也有一大打不规范写法，这里就不说了。
 
-
-
-
-
 ## 参考
 
-+ LRC文件格式
+- LRC 文件格式
 
   https://en.wikipedia.org/wiki/LRC_(file_format)
 
   https://blog.csdn.net/beijingak/article/details/7601534
 
   https://www.cnblogs.com/tocy/p/subtitle-format-lyric.html
 
   https://baike.baidu.com/item/lrc/46935
 
-+ LRC歌词开发标准参考
+- LRC 歌词开发标准参考
 
   https://www.cnblogs.com/lbnnbs/p/4781993.html
 
-+ LRC生成器
+- LRC 生成器
 
   http://www.lrcgenerator.com/
-
-
```

### Comparing `LyricLib-0.0.3.1/docs/开发日志.TXT` & `LyricLib-0.0.3.2/docs/开发日志.TXT`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 
+0.0.3.2 2023 07 01
+0.	修复 SingleLineLyric 类中 __str__ 函数在包含字词标签时输出为 None 的问题
+1.	规范一些代码，使得类型更易查找
+
 0.0.3.1	2023 05 21
 0.	修改部分注释，完善命名规范
 
 0.0.3	2023 05 07
 0.	完善 TimeStamp 类
 1.	完善样例代码中的一些说明
 2.	完善部分功能
```

### Comparing `LyricLib-0.0.3.1/setup.py` & `LyricLib-0.0.3.2/setup.py`

 * *Files identical despite different names*

