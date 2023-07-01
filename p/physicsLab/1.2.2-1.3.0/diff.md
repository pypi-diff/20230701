# Comparing `tmp/physicsLab-1.2.2.tar.gz` & `tmp/physicsLab-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\physicsLab-1.2.2.tar", last modified: Sun Apr 30 08:38:11 2023, max compression
+gzip compressed data, was "dist\physicsLab-1.3.0.tar", last modified: Sat Jul  1 04:17:24 2023, max compression
```

## Comparing `physicsLab-1.2.2.tar` & `physicsLab-1.3.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 08:38:11.000000 physicsLab-1.2.2/
--rw-rw-rw-   0        0        0     1094 2023-04-05 15:16:06.000000 physicsLab-1.2.2/LICENSE.txt
--rw-rw-rw-   0        0        0     4440 2023-04-30 08:38:11.000000 physicsLab-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3880 2023-04-19 15:49:15.000000 physicsLab-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 08:38:11.000000 physicsLab-1.2.2/physicsLab/
--rw-rw-rw-   0        0        0      379 2023-04-30 06:47:35.000000 physicsLab-1.2.2/physicsLab/__init__.py
--rw-rw-rw-   0        0        0      966 2023-04-14 14:26:12.000000 physicsLab-1.2.2/physicsLab/_colorUtils.py
--rw-rw-rw-   0        0        0     3471 2023-04-30 06:47:19.000000 physicsLab-1.2.2/physicsLab/_fileGlobals.py
--rw-rw-rw-   0        0        0      715 2023-04-21 15:10:17.000000 physicsLab-1.2.2/physicsLab/_tools.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:38:11.000000 physicsLab-1.2.2/physicsLab/astrophysics/
--rw-rw-rw-   0        0        0       13 2023-04-21 15:10:17.000000 physicsLab-1.2.2/physicsLab/astrophysics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:38:11.000000 physicsLab-1.2.2/physicsLab/electricity/
--rw-rw-rw-   0        0        0      619 2023-04-28 12:19:38.000000 physicsLab-1.2.2/physicsLab/electricity/__init__.py
--rw-rw-rw-   0        0        0     4424 2023-04-28 12:17:30.000000 physicsLab-1.2.2/physicsLab/electricity/element.py
--rw-rw-rw-   0        0        0      688 2023-04-30 07:33:03.000000 physicsLab-1.2.2/physicsLab/electricity/elementPin.py
--rw-rw-rw-   0        0        0     2887 2023-04-30 06:49:55.000000 physicsLab-1.2.2/physicsLab/electricity/elementXYZ.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:38:11.000000 physicsLab-1.2.2/physicsLab/electricity/elementsClass/
--rw-rw-rw-   0        0        0      483 2023-04-28 12:01:14.000000 physicsLab-1.2.2/physicsLab/electricity/elementsClass/__init__.py
--rw-rw-rw-   0        0        0     4942 2023-04-28 09:39:05.000000 physicsLab-1.2.2/physicsLab/electricity/elementsClass/_elementClassHead.py
--rw-rw-rw-   0        0        0     9761 2023-04-28 12:34:35.000000 physicsLab-1.2.2/physicsLab/electricity/elementsClass/artificialCircuit.py
--rw-rw-rw-   0        0        0     9101 2023-04-28 12:34:35.000000 physicsLab-1.2.2/physicsLab/electricity/elementsClass/basicCircuit.py
--rw-rw-rw-   0        0        0    18300 2023-04-28 12:30:37.000000 physicsLab-1.2.2/physicsLab/electricity/elementsClass/logicCircuit.py
--rw-rw-rw-   0        0        0     4640 2023-04-28 12:34:35.000000 physicsLab-1.2.2/physicsLab/electricity/elementsClass/otherCircuit.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:38:11.000000 physicsLab-1.2.2/physicsLab/electricity/unionElements/
--rw-rw-rw-   0        0        0      297 2023-04-30 07:25:33.000000 physicsLab-1.2.2/physicsLab/electricity/unionElements/__init__.py
--rw-rw-rw-   0        0        0     1641 2023-04-30 06:47:19.000000 physicsLab-1.2.2/physicsLab/electricity/unionElements/_unionClassHead.py
--rw-rw-rw-   0        0        0    15760 2023-04-30 07:51:24.000000 physicsLab-1.2.2/physicsLab/electricity/unionElements/unionLogic.py
--rw-rw-rw-   0        0        0     1376 2023-04-28 12:35:26.000000 physicsLab-1.2.2/physicsLab/electricity/unionElements/unionMusic.py
--rw-rw-rw-   0        0        0      605 2023-04-30 08:22:07.000000 physicsLab-1.2.2/physicsLab/electricity/unionElements/unionPin.py
--rw-rw-rw-   0        0        0     1883 2023-04-30 08:29:02.000000 physicsLab-1.2.2/physicsLab/electricity/unionElements/wires.py
--rw-rw-rw-   0        0        0     3433 2023-04-30 08:03:53.000000 physicsLab-1.2.2/physicsLab/electricity/wire.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:38:11.000000 physicsLab-1.2.2/physicsLab/electromagnetism/
--rw-rw-rw-   0        0        0       13 2023-04-21 15:10:17.000000 physicsLab-1.2.2/physicsLab/electromagnetism/__init__.py
--rw-rw-rw-   0        0        0      436 2023-04-30 08:01:14.000000 physicsLab-1.2.2/physicsLab/errors.py
--rw-rw-rw-   0        0        0    11653 2023-04-28 12:47:59.000000 physicsLab-1.2.2/physicsLab/experiment.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:38:11.000000 physicsLab-1.2.2/physicsLab.egg-info/
--rw-rw-rw-   0        0        0     4440 2023-04-30 08:38:11.000000 physicsLab-1.2.2/physicsLab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1200 2023-04-30 08:38:11.000000 physicsLab-1.2.2/physicsLab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 08:38:11.000000 physicsLab-1.2.2/physicsLab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-30 08:38:11.000000 physicsLab-1.2.2/physicsLab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      581 2023-03-16 14:16:49.000000 physicsLab-1.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-30 08:38:11.000000 physicsLab-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1151 2023-04-30 08:37:00.000000 physicsLab-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 04:17:24.000000 physicsLab-1.3.0/
+-rw-rw-rw-   0        0        0     1086 2023-06-30 14:48:23.000000 physicsLab-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     4719 2023-07-01 04:17:24.000000 physicsLab-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4163 2023-06-30 14:48:23.000000 physicsLab-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 04:17:23.000000 physicsLab-1.3.0/physicsLab/
+-rw-rw-rw-   0        0        0     2685 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/__init__.py
+-rw-rw-rw-   0        0        0      966 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/_colorUtils.py
+-rw-rw-rw-   0        0        0     7004 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/_fileGlobals.py
+-rw-rw-rw-   0        0        0     1110 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/_tools.py
+drwxrwxrwx   0        0        0        0 2023-07-01 04:17:23.000000 physicsLab-1.3.0/physicsLab/astrophysics/
+-rw-rw-rw-   0        0        0       13 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/astrophysics/__init__.py
+-rw-rw-rw-   0        0        0       62 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/astrophysics/elementsClass.py
+drwxrwxrwx   0        0        0        0 2023-07-01 04:17:23.000000 physicsLab-1.3.0/physicsLab/electricity/
+-rw-rw-rw-   0        0        0      687 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/__init__.py
+-rw-rw-rw-   0        0        0      567 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/elementPin.py
+-rw-rw-rw-   0        0        0     3277 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/elementXYZ.py
+drwxrwxrwx   0        0        0        0 2023-07-01 04:17:23.000000 physicsLab-1.3.0/physicsLab/electricity/elementsClass/
+-rw-rw-rw-   0        0        0      517 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/elementsClass/__init__.py
+-rw-rw-rw-   0        0        0     5157 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/elementsClass/_elementClassHead.py
+-rw-rw-rw-   0        0        0     9060 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/elementsClass/artificialCircuit.py
+-rw-rw-rw-   0        0        0     8423 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/elementsClass/basicCircuit.py
+-rw-rw-rw-   0        0        0    17465 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/elementsClass/logicCircuit.py
+-rw-rw-rw-   0        0        0     7106 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/elementsClass/otherCircuit.py
+drwxrwxrwx   0        0        0        0 2023-07-01 04:17:23.000000 physicsLab-1.3.0/physicsLab/electricity/unionElements/
+-rw-rw-rw-   0        0        0      314 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/unionElements/__init__.py
+-rw-rw-rw-   0        0        0     2395 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/unionElements/_unionClassHead.py
+-rw-rw-rw-   0        0        0    22879 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/unionElements/unionLogic.py
+-rw-rw-rw-   0        0        0     8896 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/unionElements/unionMusic.py
+-rw-rw-rw-   0        0        0      769 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/unionElements/unionPin.py
+-rw-rw-rw-   0        0        0     2095 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/unionElements/wires.py
+-rw-rw-rw-   0        0        0     2476 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electricity/wire.py
+drwxrwxrwx   0        0        0        0 2023-07-01 04:17:24.000000 physicsLab-1.3.0/physicsLab/electromagnetism/
+-rw-rw-rw-   0        0        0       70 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electromagnetism/__init__.py
+-rw-rw-rw-   0        0        0     4483 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/electromagnetism/elementsClass.py
+-rw-rw-rw-   0        0        0     4607 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/element.py
+-rw-rw-rw-   0        0        0     1619 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/errors.py
+-rw-rw-rw-   0        0        0    11010 2023-06-30 14:48:23.000000 physicsLab-1.3.0/physicsLab/experiment.py
+drwxrwxrwx   0        0        0        0 2023-07-01 04:17:23.000000 physicsLab-1.3.0/physicsLab.egg-info/
+-rw-rw-rw-   0        0        0     4719 2023-07-01 04:17:23.000000 physicsLab-1.3.0/physicsLab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1255 2023-07-01 04:17:23.000000 physicsLab-1.3.0/physicsLab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 04:17:23.000000 physicsLab-1.3.0/physicsLab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-01 04:17:23.000000 physicsLab-1.3.0/physicsLab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 04:17:24.000000 physicsLab-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1153 2023-07-01 04:16:00.000000 physicsLab-1.3.0/setup.py
```

### Comparing `physicsLab-1.2.2/LICENSE.txt` & `physicsLab-1.3.0/LICENSE`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-Copyright (c) 2021 The Python Packaging Authority
- 
+MIT License
+
+Copyright (c) 2023 Goodenough
+
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
- 
+
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
- 
+
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `physicsLab-1.2.2/PKG-INFO` & `physicsLab-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: physicsLab
-Version: 1.2.2
+Version: 1.3.0
 Summary: Doing experiments in the physics lab AR by python
 Home-page: https://gitee.com/script2000/physicsLab
 Author: Goodenough
 Author-email: 2381642961@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE
 
 ﻿# physicsLab 物实程序化
 
 ![输入图片说明](cover.png)
 
 ## 介绍
 在物理实验室做实验的时候，我们可能会苦恼于元件不够整齐且无法浮空等等问题。这些都可以通过改存档来轻易实现！然而，手动改存档局限性很大，于是我封装了一些常用功能，让你用Python也能够轻易地做实验，**你甚至不需用知道存档在电脑的哪里**！
@@ -52,15 +52,26 @@
  # crt_wire输入格式：  
  #    crt_wire(SourcePin, TargetPin, color = "蓝")  
 crt_Wire(o.i_up, o.i_low)  
  # 将程序中生成的原件，导线等等写入存档  
 write_Experiment()  
  # 然后用物实打开存档见证奇迹  
 ```
-更详细的内容请查看[functions.md](functions.md)  
+如今有了更优雅的方式：
+```python
+from physicsLab import *
+
+with experiment('测逝', read=True, elementXYZ=True):
+    Logic_Input(0, 0, 1)
+    o = Or_Gate()
+    o.i_up - o.i_low # 连接导线
+```
+上面两段代码产生的结果是一样的  
+  
+更详细的内容请在[wiki](https://gitee.com/script2000/physicsLab/wikis/functions)中查看  
 请注意：Python采用GBK编码，而物实用的是utf-8，尽管尽量确保编码格式正确，但中文仍有可能出现问题，因此建议多用英文。  
 
 ## 优点
 1. 通过read_Experiment()，你无须把所有工作交给代码。因为用代码写并不总是意味着方便（比如连接导线）。  
 你现在可以手动连接部分导线或者添加原件，并通过保存的形式，让程序在下次也可以轻松读取。  
 这也意味着你不用一口气把控制整个电路的脚本写出来，而是每次写一部分，并把更适合代码的工作交给代码完成。  
 也就是说，写这个脚本的感觉更像在控制台上操作，非常灵活。
@@ -80,12 +91,11 @@
 ## 其他
 1. 更多内容请在[other physicsLab](https://gitee.com/script2000/temporary-warehouse/tree/master/other%20physicsLab)查看
 2. github: https://github.com/GoodenoughPhysicsLab/physicsLab
 3. gitee: https://gitee.com/script2000/physicsLab
 
 ## 参与贡献
 1.  Fork 本仓库
-2.  新建 Feat_xxx 分支
+2.  新建分支
 3.  提交代码
 4.  新建 Pull Request
-5.  补充readme
```

### Comparing `physicsLab-1.2.2/README.md` & `physicsLab-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,26 @@
  # crt_wire输入格式：  
  #    crt_wire(SourcePin, TargetPin, color = "蓝")  
 crt_Wire(o.i_up, o.i_low)  
  # 将程序中生成的原件，导线等等写入存档  
 write_Experiment()  
  # 然后用物实打开存档见证奇迹  
 ```
-更详细的内容请查看[functions.md](functions.md)  
+如今有了更优雅的方式：
+```python
+from physicsLab import *
+
+with experiment('测逝', read=True, elementXYZ=True):
+    Logic_Input(0, 0, 1)
+    o = Or_Gate()
+    o.i_up - o.i_low # 连接导线
+```
+上面两段代码产生的结果是一样的  
+  
+更详细的内容请在[wiki](https://gitee.com/script2000/physicsLab/wikis/functions)中查看  
 请注意：Python采用GBK编码，而物实用的是utf-8，尽管尽量确保编码格式正确，但中文仍有可能出现问题，因此建议多用英文。  
 
 ## 优点
 1. 通过read_Experiment()，你无须把所有工作交给代码。因为用代码写并不总是意味着方便（比如连接导线）。  
 你现在可以手动连接部分导线或者添加原件，并通过保存的形式，让程序在下次也可以轻松读取。  
 这也意味着你不用一口气把控制整个电路的脚本写出来，而是每次写一部分，并把更适合代码的工作交给代码完成。  
 也就是说，写这个脚本的感觉更像在控制台上操作，非常灵活。
@@ -63,11 +74,10 @@
 ## 其他
 1. 更多内容请在[other physicsLab](https://gitee.com/script2000/temporary-warehouse/tree/master/other%20physicsLab)查看
 2. github: https://github.com/GoodenoughPhysicsLab/physicsLab
 3. gitee: https://gitee.com/script2000/physicsLab
 
 ## 参与贡献
 1.  Fork 本仓库
-2.  新建 Feat_xxx 分支
+2.  新建分支
 3.  提交代码
-4.  新建 Pull Request
-5.  补充readme
+4.  新建 Pull Request
```

### Comparing `physicsLab-1.2.2/physicsLab/_colorUtils.py` & `physicsLab-1.3.0/physicsLab/_colorUtils.py`

 * *Files identical despite different names*

### Comparing `physicsLab-1.2.2/physicsLab/_tools.py` & `physicsLab-1.3.0/physicsLab/_tools.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 #coding=utf-8
-import typing as _typing
+from os import walk
+from typing import *
+from collections import namedtuple
+from physicsLab._fileGlobals import FILE_HEAD
 
 # type hint
-numType = _typing.Union[int, float]
+numType = Union[int, float]
+
+# class position
+position = namedtuple("position", ["x", "y", "z"])
 
 # 四舍五入physicsLab中的数据
 # 支持传入多个数据
-def roundData(*num):
-    if not any(
-        isinstance(i, (int, float)) for i in num
-     ):
+def roundData(*num) -> Union[int, float, tuple]:
+    if not all(isinstance(val, (int, float)) for val in num):
         raise TypeError
     
     if len(num) == 1:
-        return round(num[0], 4)
-    return (round(i, 4) for i in num)
+        return float(round(num[0], 4))
+    return tuple(float(round(i, 4)) for i in num)
 
 # 生成随机字符串
 def randString(strLength: int) -> str:
     if not isinstance(strLength, int):
         raise TypeError
 
     from string import ascii_letters as _ascii_letters, digits as _digits
     from random import choice as _choice
-    return ''.join(_choice(_ascii_letters + _digits) for _ in range(strLength))
+    return ''.join(_choice(_ascii_letters + _digits) for _ in range(strLength))
+
+# 索取所有物实存档
+def getAllSav() -> List:
+    savs = [i for i in walk(FILE_HEAD)][0]
+    savs = savs[savs.__len__() - 1]
+    return [aSav for aSav in savs if aSav.endswith('sav')]
```

### Comparing `physicsLab-1.2.2/physicsLab/electricity/__init__.py` & `physicsLab-1.3.0/physicsLab/electricity/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #coding=utf-8
-# 操作元件
-from physicsLab.electricity.element import *
+# 元件引脚类
+from physicsLab.electricity.elementPin import *
 # 操作导线
 from physicsLab.electricity.wire import *
 # 元件类
 from physicsLab.electricity.elementsClass.artificialCircuit import *
 from physicsLab.electricity.elementsClass.basicCircuit import *
 from physicsLab.electricity.elementsClass.logicCircuit import *
 from physicsLab.electricity.elementsClass.otherCircuit import *
-# 元件引脚类
-from physicsLab.electricity.elementPin import *
 # 元件坐标系
 from physicsLab.electricity.elementXYZ import *
 # 模块化电路
-from physicsLab.electricity.unionElements import *
+from physicsLab.electricity.unionElements import *
+import physicsLab.electricity.unionElements.unionLogic as union
+import physicsLab.electricity.unionElements.unionMusic as music
```

### Comparing `physicsLab-1.2.2/physicsLab/electricity/element.py` & `physicsLab-1.3.0/physicsLab/element.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #coding=utf-8
 import physicsLab._tools as _tools
+import physicsLab.errors as errors
 import physicsLab._fileGlobals as _fileGlobals
 import physicsLab.electricity.elementXYZ as _elementXYZ
 import physicsLab.electricity.elementsClass as _elementsClass
 
 # 创建原件，本质上仍然是实例化
 def crt_Element(
         name: str,
@@ -14,14 +15,16 @@
     ):
     if not (isinstance(name, str)
             and isinstance(x, (int, float))
             and isinstance(y, (int, float))
             and isinstance(z, (int, float))
     ):
         raise RuntimeError("Wrong parameter type")
+#    _fileGlobals.check_ExperimentType(0)
+
     name = name.strip()
     if name == '':
         raise RuntimeError('Name cannot be an empty string')
         # 元件坐标系
     if elementXYZ == True or (_elementXYZ.is_elementXYZ() == True and elementXYZ is None):
         x, y, z = _elementXYZ.xyzTranslate(x, y, z)
     x, y, z = _tools.roundData(x, y, z)
@@ -34,30 +37,32 @@
     else:
         try:
             return eval(f"_elementsClass.{name.replace(' ', '_').replace('-', '_')}({x},{y},{z})")
         except SyntaxError:
             raise RuntimeError(f"{name} original that does not exist")
 
 # 获取对应坐标的self
-def get_Element(*args, **kwargs) -> _elementsClass.elementBase:
+def get_Element(*args, **kwargs) -> _elementsClass.electricityBase:
     # 通过坐标索引元件
     def position_Element(x: _tools.numType, y: _tools.numType, z: _tools.numType):
         if not (isinstance(x, (int, float)) and isinstance(y, (int, float)) and isinstance(z, (int, float))):
             raise TypeError('illegal argument')
-        x, y, z = _tools.roundData(x), _tools.roundData(y), _tools.roundData(z)
-        if (x, y, z) not in _fileGlobals.elements_Position.keys():
-            raise RuntimeError("Error coordinates that do not exist")
-        result: list = _fileGlobals.elements_Position[(x, y, z)]['self']
+        position = _tools.roundData(x, y, z)
+        if position not in _fileGlobals.elements_Position.keys():
+            raise RuntimeError(f"{position} do not exist")
+        result: list = _fileGlobals.elements_Position[position]['self']
         return result[0] if len(result) == 1 else result
     # 通过index（元件生成顺序）索引元件
     def index_Element(index: int):
         if 0 < index <= len(_fileGlobals.elements_Index):
             return _fileGlobals.elements_Index[index - 1]
         else:
-            raise RuntimeError
+            raise errors.getElementError
+
+#    _fileGlobals.check_ExperimentType(0)
 
     # 如果输入参数为 x=, y=, z=
     if list(kwargs.keys()) == ['x', 'y', 'z']:
         return position_Element(kwargs['x'], kwargs['y'], kwargs['z'])
     # 如果输入参数为 index=
     elif list(kwargs.keys()) == ['index']:
         return index_Element(kwargs['index'])
@@ -72,40 +77,45 @@
         else:
             raise TypeError
     else:
         raise TypeError
 
 # 删除原件
 def del_Element(self) -> None:
+#    _fileGlobals.check_ExperimentType(0)
+
     try:
         identifier = self._arguments['Identifier']
-        if self.father_type() == 'element':
+        if isinstance(self, _elementsClass.electricityBase):
             for element in _fileGlobals.Elements:
                 if identifier == element['Identifier']:
                     # 删除原件
                     _fileGlobals.Elements.remove(element)
                     # 删除导线
                     i = 0
                     while i < _fileGlobals.Wires.__len__():
                         wire = _fileGlobals.Wires[i]
-                        if (wire['Source'] == identifier or wire['Target'] == identifier):
+                        if wire['Source'] == identifier or wire['Target'] == identifier:
                             _fileGlobals.Wires.pop(i)
                         else:
                             i += 1
                     return
     except:
         raise RuntimeError('Unable to delete a nonexistent element')
 
-# 整理物实原件的角度、位置
-def format_Elements() -> None:
-    pass
-
 # 原件的数量
 def count_Elements() -> int:
     return len(_fileGlobals.Elements)
 
 # 清空原件
 def clear_Elements() -> None:
     _fileGlobals.Elements.clear()
     _fileGlobals.Wires.clear()
     _fileGlobals.elements_Index.clear()
-    _fileGlobals.elements_Position.clear()
+    _fileGlobals.elements_Position.clear()
+
+def print_Elements() -> None:
+    print(_fileGlobals.Elements)
+
+# 元件基类
+class elementBase:
+    pass
```

### Comparing `physicsLab-1.2.2/physicsLab/electricity/elementPin.py` & `physicsLab-1.3.0/physicsLab/electricity/elementPin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 #coding=utf-8
 from physicsLab.electricity.wire import crt_Wire
-import physicsLab.electricity.elementsClass._elementClassHead as _elementClassHead
 
 # 电学元件引脚类
 class element_Pin:
     __slots__ = ("element_self", "pinLabel")
-    def __init__(self, input_self: _elementClassHead.elementBase, pinLabel: int):
-        self.element_self: _elementClassHead.elementBase = input_self
+    def __init__(self, input_self, pinLabel: int) -> None:
+        self.element_self = input_self
         self.pinLabel: int = pinLabel
 
     # 重载减法运算符作为连接导线的语法
-    def __sub__(self, obj: "element_Pin"):
+    def __sub__(self, obj: "element_Pin") -> "element_Pin":
         crt_Wire(self, obj)
         return obj
 
     # 返回一个字符串形式的类型
     def type(self) -> str:
         return 'element Pin'
```

### Comparing `physicsLab-1.2.2/physicsLab/electricity/elementXYZ.py` & `physicsLab-1.3.0/physicsLab/electricity/elementXYZ.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,19 +9,28 @@
 # y轴的修正为 +0.04
 # 坐标修正部分的代码在对应的类的文件中
 # 如big_Elements的坐标修正在logicCircuit.py
 
 # _elementClassHead里的element_Init_HEAD有部分处理元件坐标系的代码，并调用了该文件
 
 import physicsLab._tools as _tools
+import physicsLab._fileGlobals as _fileGlobals
+from typing import Callable as _Callable
 
 ### define ###
 
 _elementXYZ: bool = False
 
+# 所有元件坐标系的函数都会有的操作：
+def _dec_EelementXYZ(func: _Callable) -> _Callable:
+    def result(*args, **kwargs):
+        _fileGlobals.check_ExperimentType(0)
+        func(*args, **kwargs)
+    return result
+
 # 是否将全局设置为元件坐标系
 def set_elementXYZ(boolen: bool) -> None:
     if not isinstance(boolen, bool):
         raise TypeError
     global _elementXYZ
     _elementXYZ = boolen
 
@@ -49,24 +58,26 @@
     # 修改元件坐标系原点
     x += _xOrigin
     y += _yOrigin
     z += _zOrigin
     return x, y, z
 
 # 将物实支持的坐标系转换为元件坐标系
-def translateXYZ(x: _tools.numType, y: _tools.numType, z: _tools.numType):
+def translateXYZ(x: _tools.numType, y: _tools.numType, z: _tools.numType, bigElement: bool = False):
     x /= _xUnit
     y /= _yUnit
     z /= _zUnit
     # 修改元件坐标系原点
     x -= _xOrigin
     y -= _yOrigin
     z -= _zOrigin
     # 修改大体积逻辑电路原件的坐标
+    if bigElement:
         # 暂不支持相关功能
+        pass
     return x, y, z
 
 # 设置元件坐标系原点O，输入值为物实坐标系
 def set_O(x: _tools.numType, y: _tools.numType, z: _tools.numType) -> None:
     if (isinstance(x, (int, float)) and
         isinstance(y, (int, float)) and
         isinstance(z, (int, float))
```

### Comparing `physicsLab-1.2.2/physicsLab/electricity/elementsClass/_elementClassHead.py` & `physicsLab-1.3.0/physicsLab/electricity/elementsClass/_elementClassHead.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,88 @@
 # coding=utf-8
 import physicsLab._tools as _tools
-from typing import Callable as _Callable
+import physicsLab.errors as errors
 import physicsLab._fileGlobals as _fileGlobals
 import physicsLab.electricity.elementPin as _elementPin
 import physicsLab.electricity.elementXYZ as _elementXYZ
 
-# 是否为big_Element
-is_big_Element: bool = False
+# electricity class's metaClass
+class eletricityMeta(type):
+    # element index
+    __index = 1
+
+    def __call__(
+            cls,
+            x: _tools.numType = 0,
+            y: _tools.numType = 0,
+            z: _tools.numType = 0,
+            elementXYZ: bool = None,
+            *args, **kwargs
+    ):
+        self = cls.__new__(cls)
+        if not (
+                isinstance(x, (float, int)) and
+                isinstance(y, (float, int)) and
+                isinstance(z, (float, int))
+        ):
+            raise TypeError('illegal argument')
+        _fileGlobals.check_ExperimentType(0)
+
+        x, y, z = _tools.roundData(x, y, z)
+        self._position = (x, y, z)
+        # 元件坐标系
+        if elementXYZ == True or (_elementXYZ.is_elementXYZ() == True and elementXYZ is None):
+            x, y, z = _elementXYZ.xyzTranslate(x, y, z)
+        self.__init__(x, y, z, *args, **kwargs)
+        # 若是big_Element，则修正坐标
+        if isinstance(self, is_big_element):
+            x, y, z = _elementXYZ.amend_big_Element(x, y, z)
+
+        self._arguments["Identifier"] = _tools.randString(32)
+        # x, z, y 物实采用欧拉坐标系
+        self._arguments["Position"] = f"{x},{z},{y}"
+        _fileGlobals.Elements.append(self._arguments)
+
+        # 该坐标是否已存在，则存入列表
+        if self._position in _fileGlobals.elements_Position.keys():
+            _fileGlobals.elements_Position[self._position]['self'].append(self)
+        else:
+            elementDict: dict = {
+                'self': [self],
+                'elementXYZ': _elementXYZ.is_elementXYZ,  # 是否为元件坐标系
+                'originPosition': tuple(_elementXYZ.get_OriginPosition())  # 坐标原点
+            }
+            _fileGlobals.elements_Position[self._position] = elementDict
+        self.set_Rotation()
+        # 通过元件生成顺序来索引元件
+        self._index = eletricityMeta.__index
+        _fileGlobals.elements_Index.append(self)
+        # 元件index索引加1
+        eletricityMeta.__index += 1
+        return self
+
+
+# 所有电学元件的父类
+class electricityBase(metaclass=eletricityMeta):
+    # 类无法被实例化
+    def __init__(self, *args, **kwargs):
+        raise errors.instantiateError
 
-# 所有元件的父类
-class elementBase:
     # 设置原件的角度
     def set_Rotation(self, xRotation: _tools.numType = 0, yRotation: _tools.numType = 0,
                      zRotation: _tools.numType = 180):
-        if not (isinstance(xRotation, (int, float)) and isinstance(yRotation, (int, float)) and isinstance(zRotation, (
-        int, float))):
+        if not (
+                isinstance(xRotation, (int, float)) and
+                isinstance(yRotation, (int, float)) and
+                isinstance(zRotation, (int, float))
+        ):
             raise RuntimeError('illegal argument')
-        self._arguments[
-            "Rotation"] = f"{_tools.roundData(xRotation)},{_tools.roundData(zRotation)},{_tools.roundData(yRotation)}"
+
+        self._arguments["Rotation"] = \
+            f"{_tools.roundData(xRotation)},{_tools.roundData(zRotation)},{_tools.roundData(yRotation)}"
         return self
 
     # 重新设置元件的坐标
     def set_Position(self, x: _tools.numType, y: _tools.numType, z: _tools.numType):
         if not (isinstance(x, (int, float)) and isinstance(y, (int, float)) and isinstance(z, (int, float))):
             raise RuntimeError('illegal argument')
         x, y, z = _tools.roundData(x), _tools.roundData(y), _tools.roundData(z)
@@ -31,16 +92,15 @@
         _fileGlobals.elements_Position[self._position] = self
         return self
 
     # 格式化坐标参数，主要避免浮点误差
     def format_Position(self) -> tuple:
         if not isinstance(self._position, tuple) or self._position.__len__() != 3:
             raise RuntimeError("Position must be a tuple of length three but gets some other value")
-        self._position = (_tools.roundData(self._position[0]), _tools.roundData(self._position[1]),
-                          _tools.roundData(self._position[2]))
+        self._position = _tools.roundData(self._position[0], self._position[1], self._position[2])
         return self._position
 
     # 获取原件的坐标
     def get_Position(self) -> tuple:
         return self._position
 
     # 获取父类的类型
@@ -55,72 +115,14 @@
     def type(self) -> str:
         return self._arguments['ModelID']
 
     # 打印参数
     def print_arguments(self) -> None:
         print(self._arguments)
 
-
-# __init__ 装饰器
-_index = 1
-
-
-def element_Init_HEAD(func: _Callable) -> _Callable:
-    def result(
-            self,
-            x: _tools.numType = 0,
-            y: _tools.numType = 0,
-            z: _tools.numType = 0,
-            elementXYZ: bool = None
-    ) -> None:
-        if not (
-                isinstance(x, (float, int)) and
-                isinstance(y, (float, int)) and
-                isinstance(z, (float, int))
-        ):
-            raise TypeError('illegal argument')
-        # 初始化全局变量
-        global is_big_Element
-        is_big_Element = False
-
-        x, y, z = _tools.roundData(x, y, z)
-        self._position = (x, y, z)
-        # 元件坐标系
-        if elementXYZ == True or (_elementXYZ.is_elementXYZ() == True and elementXYZ is None):
-            x, y, z = _elementXYZ.xyzTranslate(x, y, z)
-        func(self, x, y, z)
-        # 若是big_Element，则修正坐标
-        if is_big_Element:
-            x, y, z = _elementXYZ.amend_big_Element(x, y, z)
-
-        self._arguments["Identifier"] = _tools.randString(32)
-        # x, z, y 物实采用欧拉坐标系
-        self._arguments["Position"] = f"{x},{z},{y}"
-        _fileGlobals.Elements.append(self._arguments)
-
-        # 该坐标是否已存在，则存入列表
-        if self._position in _fileGlobals.elements_Position.keys():
-            _fileGlobals.elements_Position[self._position]['self'].append(self)
-        else:
-            elementDict: dict = {
-                'self': [self],
-                'elementXYZ': _elementXYZ.is_elementXYZ,  # 是否为元件坐标系
-                'originPosition': tuple(_elementXYZ.get_OriginPosition())  # 坐标原点
-            }
-            _fileGlobals.elements_Position[self._position] = elementDict
-        self.set_Rotation()
-        # 通过元件生成顺序来索引元件
-        global _index
-        self._index = _index
-        _fileGlobals.elements_Index.append(self)
-        # 元件index索引加1
-        _index += 1
-    return result
-
-
 # 双引脚模拟电路原件的引脚
 def two_pin_ArtificialCircuit_Pin(cls):
     @property
     def red(self):
         return _elementPin.element_Pin(self, 0)
 
     cls.red, cls.l = red, red
@@ -128,7 +130,11 @@
     @property
     def black(self):
         return _elementPin.element_Pin(self, 1)
 
     cls.black, cls.r = black, black
 
     return cls
+
+# 仅用于判断是否为2体积元件
+class is_big_element:
+    pass
```

### Comparing `physicsLab-1.2.2/physicsLab/electricity/elementsClass/artificialCircuit.py` & `physicsLab-1.3.0/physicsLab/electricity/elementsClass/basicCircuit.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,205 +1,171 @@
 #coding=utf-8
-import physicsLab._tools as _tools
-from ..elementXYZ import amend_big_Element
+from physicsLab._tools import numType
 import physicsLab.electricity.elementPin as _elementPin
-import physicsLab.electricity.elementsClass._elementClassHead as _elementClassHead
+from ._elementClassHead import electricityBase, two_pin_ArtificialCircuit_Pin
 
+# 开关基类
 
-# 555定时器
-class NE555(_elementClassHead.elementBase):
-    @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
-        self._arguments = {'ModelID': '555 Timer', 'Identifier': '', 'IsBroken': False,
-                           'IsLocked': False, 'Properties': {'高电平': 3.0, '低电平': 0.0, '锁定': 1.0},
-                           'Statistics': {'供电': 10, '放电': 0.0, '阈值': 4,
-                                          '控制': 6.6666666666666666, '触发': 4,
-                                          '输出': 0, '重设': 10, '接地': 0},
-                           'Position': '', 'Rotation': '', 'DiagramCached': False,
-                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
-        _elementClassHead.is_big_Element = True
+class _switch_electricity(electricityBase):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
+        self._arguments = {"ModelID": "", "Identifier": "", "IsBroken": False,
+                          "IsLocked": False, "Properties": {"开关": 0, "锁定": 1.0},
+                          "Statistics": {}, "Position": "",
+                          "Rotation": '', "DiagramCached": False,
+                          "DiagramPosition": {"X": 0, "Y": 0, "Z": 0, "Magnitude": 0}, "DiagramRotation": 0}
+
+# 简单开关
+@two_pin_ArtificialCircuit_Pin
+class Simple_Switch(_switch_electricity):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
+        super(Simple_Switch, self).__init__(x, y, z, elementXYZ)
+        self._arguments['ModelID'] = 'Simple Switch'
+
+# 单刀双掷开关
+class SPDT_Switch(_switch_electricity):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
+        super(SPDT_Switch, self).__init__(x, y, z, elementXYZ)
+        self._arguments['ModelID'] = 'SPDT Switch'
 
     @property
-    def VCC(self) -> _elementPin.element_Pin:
+    def l(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
 
     @property
-    def Dis(self) -> _elementPin.element_Pin:
+    def mid(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
     @property
-    def Thr(self) -> _elementPin.element_Pin:
+    def r(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 2)
 
+# 双刀双掷开关
+class DPDT_Switch(_switch_electricity):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
+        super(DPDT_Switch, self).__init__(x, y, z, elementXYZ)
+        self._arguments['ModelID'] = 'DPDT Switch'
+
     @property
-    def Ctrl(self) -> _elementPin.element_Pin:
+    def l_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 3)
 
     @property
-    def Trig(self) -> _elementPin.element_Pin:
+    def mid_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 4)
 
     @property
-    def Out(self) -> _elementPin.element_Pin:
+    def r_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 5)
 
     @property
-    def Reset(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 6)
+    def l_low(self) -> _elementPin.element_Pin:
+        return _elementPin.element_Pin(self, 0)
 
     @property
-    def Ground(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 7)
-
-# 电容
-@_elementClassHead.two_pin_ArtificialCircuit_Pin
-class Basic_Capacitor(_elementClassHead.elementBase):
-    @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
-        self._arguments = {'ModelID': 'Basic Capacitor', 'Identifier': '',
-                           'IsBroken': False, 'IsLocked': False, 'Properties': {'耐压': 16.0, '电容': 1e-06, '内阻': 5.0, '锁定': 1.0},
-                           'Statistics': {}, 'Position': '',
-                           'Rotation': '', 'DiagramCached': False,
-                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
-
-# 接地
-class Ground_Component(_elementClassHead.elementBase):
-    @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
-        self._arguments = {'ModelID': 'Ground Component', 'Identifier': '',
-                           'IsBroken': False, 'IsLocked': False, 'Properties': {'锁定': 1.0},
-                           'Statistics': {'电流': 0}, 'Position': '',
-                           'Rotation': '', 'DiagramCached': False,
-                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
+    def mid_low(self) -> _elementPin.element_Pin:
+        return _elementPin.element_Pin(self, 1)
 
     @property
-    def i(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
+    def r_low(self) -> _elementPin.element_Pin:
+        return _elementPin.element_Pin(self, 2)
 
-# 运算放大器
-class Operational_Amplifier(_elementClassHead.elementBase):
-    @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
-        self._arguments = {'ModelID': 'Operational Amplifier', 'Identifier': '',
-                           'IsBroken': False, 'IsLocked': False,
-                           'Properties': {'增益系数': 100_0000.0, '最大电压': 15.0, '最小电压': -15.0, '锁定': 1.0},
-                           'Statistics': {'电压-': 0, '电压+': 0, '输出电压': 0,
-                                          '输出电流': 0, '输出功率': 0},
+# 按钮开关
+@two_pin_ArtificialCircuit_Pin
+class Push_Switch(electricityBase):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
+        self._arguments = {
+            'ModelID': 'Push Switch', 'Identifier': '', 'IsBroken': False, 'IsLocked': False,
+            'Properties': {'开关': 0.0, '默认开关': 0.0, '锁定': 1.0}, 'Statistics': {'电流': 0.0}, 'Position': '',
+            'Rotation': '', 'DiagramCached': False, 'DiagramPosition': {
+                'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
+
+
+# 一节电池
+@two_pin_ArtificialCircuit_Pin
+class Battery_Source(electricityBase):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
+        self._arguments = {'ModelID': 'Battery Source', 'Identifier': '',
+                           'IsBroken': False, 'IsLocked': False, 'Properties': {'最大功率': 16.2, '电压': 3.0, '内阻': 0.5},
+                           'Statistics': {'电流': 0, '功率': 0, '电压': 0},
                            'Position': '',
                            'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
-    @property
-    def i_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
-
-    @property
-    def i_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 1)
-
-    @property
-    def o(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 2)
-
-# 继电器
-class Relay_Component(_elementClassHead.elementBase):
-    @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
-        self._arguments = {'ModelID': 'Relay Component', 'Identifier': '', 'IsBroken': False, 'IsLocked': False,
-                           'Properties': {'开关': 0.0, '线圈电感': 0.2, '线圈电阻': 20.0,
-                                          '接通电流': 0.02, '额定电流': 1.0, '锁定': 1.0}, 'Statistics': {},
-                           'Position': '', 'Rotation': '',
-                           'DiagramCached': False, 'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0},
+# 学生电源
+class Student_Source(electricityBase):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
+        self._arguments = {'ModelID': 'Student Source', 'Identifier': '', 'IsBroken': False, 'IsLocked': False,
+                           'Properties': {'交流电压': 3.0, '直流电压': 3.0, '开关': 0.0, '频率': 50.0},
+                           'Statistics': {'瞬间功率': 0.0, '瞬间电压': 0.0, '瞬间电流': 0.0,
+                                          '瞬间电阻': 0.0, '功率': 0.0, '电阻': 0.0, '电流': 0.0,
+                                          '瞬间功率1': 0.0, '瞬间电压1': 0.0, '瞬间电流1': 0.0,
+                                          '瞬间电阻1': 0.0,
+                                          '功率1': 0.0, '电阻1': 0.0, '电流1': 0.0},
+                           'Position': '',
+                           'Rotation': '', 'DiagramCached': False,
+                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0},
                            'DiagramRotation': 0}
 
     @property
-    def l_up(self) -> _elementPin.element_Pin:
+    def l(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
 
     @property
-    def l_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 2)
-
-    @property
-    def mid(self) -> _elementPin.element_Pin:
+    def l_mid(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
     @property
-    def r_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 4)
+    def r_mid(self) -> _elementPin.element_Pin:
+        return _elementPin.element_Pin(self, 2)
 
     @property
-    def r_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 5)
+    def r(self) -> _elementPin.element_Pin:
+        return _elementPin.element_Pin(self, 3)
 
-# n mos
-class N_MOSFET(_elementClassHead.elementBase):
-    @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
-        self._arguments = {'ModelID': 'N-MOSFET', 'Identifier': '', 'IsBroken': False,
-                           'IsLocked': False, 'Properties': {'PNP': 1.0, '放大系数': 0.027, '阈值电压': 1.5, '最大功率': 100.0, '锁定': 1.0},
-                           'Statistics': {'电压GS': 0.0, '电压': 0.0, '电流': 0.0, '功率': 0.0, '状态': 0.0},
+# 电阻
+@two_pin_ArtificialCircuit_Pin
+class Resistor(electricityBase):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
+        self._arguments = {'ModelID': 'Resistor', 'Identifier': '', 'IsBroken': False,
+                           'IsLocked': False,
+                           'Properties': {'最大电阻': 1000_0000.0, '最小电阻': 0.1, '电阻': 10, '锁定': 1.0},
+                           'Statistics': {'瞬间功率': 0, '瞬间电流': 0,
+                                          '瞬间电压': 0, '功率': 0,
+                                          '电压': 0, '电流': 0},
                            'Position': '', 'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
-    @property
-    def D(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 2)
-
-    @property
-    def S(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 1)
-
-    @property
-    def G(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
+# 保险丝
+@two_pin_ArtificialCircuit_Pin
+class Fuse_Component(electricityBase):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
+        self._arguments = {'ModelID': 'Fuse Component', 'Identifier': '', 'IsBroken': False, 'IsLocked': False,
+                           'Properties': {'开关': 1.0, '额定电流': 0.30000001192092896, '熔断电流': 0.5, '锁定': 1.0},
+                           'Statistics': {'瞬间功率': 0.0, '瞬间电流': 0.0, '瞬间电压': 0.0, '功率': 0.0, '电压': 0.0, '电流': 0.0},
+                           'Position': '', 'Rotation': '', 'DiagramCached': False,
+                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
-# 波形发生器基类
-class _source_element(_elementClassHead.elementBase):
-    @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
-        self._arguments = {'ModelID': '', 'Identifier': '',
-                           'IsBroken': False, 'IsLocked': False,
-                           'Properties': {'电压': 3.0, '内阻': 0.5, '频率': 20000.0, '偏移': 0.0, '占空比': 0.5, '锁定': 1.0},
-                           'Statistics': {'电流': 0.0, '功率': 0.0, '电压': -3.0},
+# 滑动变阻器
+class Slide_Rheostat(electricityBase):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
+        self._arguments = {'ModelID': 'Slide Rheostat', 'Identifier': '', 'IsBroken': False, 'IsLocked': False,
+                           'Properties': {'额定电阻': 10.0, '滑块位置': 0.0, '电阻1': 10, '电阻2': 10.0, '锁定': 1.0},
+                           'Statistics': {'瞬间功率': 0.0, '瞬间电流': 0.0, '瞬间电压': 0.0, '功率': 0.0, '电压': 0.0, '电流': 0.0,
+                                          '瞬间功率1': 0.0, '瞬间电流1': 0.0, '瞬间电压1': 0.0, '功率1': 0.0, '电压1': 0.0, '电流1': 0.0},
                            'Position': '', 'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
-    def l(self) -> _elementPin.element_Pin:
+    def l_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
-    i = l
 
     @property
-    def r(self) -> _elementPin.element_Pin:
+    def r_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
-    o = r
 
-# 正弦波发生器
-class Sinewave_Source(_source_element):
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
-        super(Sinewave_Source, self).__init__(x, y, z, elementXYZ)
-        self._arguments['ModelID'] = 'Sinewave Source'
-
-# 方波发生器
-class Square_Source(_source_element):
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
-        super(Square_Source, self).__init__(x, y, z, elementXYZ)
-        self._arguments['ModelID'] = 'Square Source'
-
-# 三角波发生器
-class Triangle_Source(_source_element):
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
-        super(Triangle_Source, self).__init__(x, y, z, elementXYZ)
-        self._arguments['ModelID'] = 'Triangle Source'
-
-# 锯齿波发生器
-class Sawtooth_Source(_source_element):
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
-        super(Sawtooth_Source, self).__init__(x, y, z, elementXYZ)
-        self._arguments['ModelID'] = 'Sawtooth Source'
-
-# 尖峰波发生器
-class Pulse_Source(_source_element):
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
-        super(Pulse_Source, self).__init__(x, y, z, elementXYZ)
-        self._arguments['ModelID'] = 'Pulse Source'
+    @property
+    def l_up(self) -> _elementPin.element_Pin:
+        return _elementPin.element_Pin(self, 2)
+
+    @property
+    def r_up(self) -> _elementPin.element_Pin:
+        return _elementPin.element_Pin(self, 3)
```

### Comparing `physicsLab-1.2.2/physicsLab/electricity/elementsClass/basicCircuit.py` & `physicsLab-1.3.0/physicsLab/electricity/elementsClass/artificialCircuit.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,178 +1,196 @@
 #coding=utf-8
-import physicsLab._tools as _tools
+from physicsLab._tools import numType
 import physicsLab.electricity.elementPin as _elementPin
-import physicsLab.electricity.elementsClass._elementClassHead as _elementClassHead
+from ._elementClassHead import electricityBase, is_big_element, two_pin_ArtificialCircuit_Pin
 
-# 开关基类
 
-class _switch_Element(_elementClassHead.elementBase):
-    @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
-        self._arguments = {"ModelID": "", "Identifier": "", "IsBroken": False,
-                          "IsLocked": False, "Properties": {"开关": 0, "锁定": 1.0},
-                          "Statistics": {}, "Position": "",
-                          "Rotation": '', "DiagramCached": False,
-                          "DiagramPosition": {"X": 0, "Y": 0, "Z": 0, "Magnitude": 0}, "DiagramRotation": 0}
-
-# 简单开关
-@_elementClassHead.two_pin_ArtificialCircuit_Pin
-class Simple_Switch(_switch_Element):
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
-        super(Simple_Switch, self).__init__(x, y, z, elementXYZ)
-        self._arguments['ModelID'] = 'Simple Switch'
-
-# 单刀双掷开关
-class SPDT_Switch(_switch_Element):
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
-        super(SPDT_Switch, self).__init__(x, y, z, elementXYZ)
-        self._arguments['ModelID'] = 'SPDT Switch'
+# 555定时器
+class NE555(electricityBase, is_big_element):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
+        self._arguments = {'ModelID': '555 Timer', 'Identifier': '', 'IsBroken': False,
+                           'IsLocked': False, 'Properties': {'高电平': 3.0, '低电平': 0.0, '锁定': 1.0},
+                           'Statistics': {'供电': 10, '放电': 0.0, '阈值': 4,
+                                          '控制': 6.6666666666666666, '触发': 4,
+                                          '输出': 0, '重设': 10, '接地': 0},
+                           'Position': '', 'Rotation': '', 'DiagramCached': False,
+                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
-    def l(self) -> _elementPin.element_Pin:
+    def VCC(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
 
     @property
-    def mid(self) -> _elementPin.element_Pin:
+    def Dis(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
     @property
-    def r(self) -> _elementPin.element_Pin:
+    def Thr(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 2)
 
-# 双刀双掷开关
-class DPDT_Switch(_switch_Element):
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
-        super(DPDT_Switch, self).__init__(x, y, z, elementXYZ)
-        self._arguments['ModelID'] = 'DPDT Switch'
-
     @property
-    def l_up(self) -> _elementPin.element_Pin:
+    def Ctrl(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 3)
 
     @property
-    def mid_up(self) -> _elementPin.element_Pin:
+    def Trig(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 4)
 
     @property
-    def r_up(self) -> _elementPin.element_Pin:
+    def Out(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 5)
 
     @property
-    def l_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
+    def Reset(self) -> _elementPin.element_Pin:
+        return _elementPin.element_Pin(self, 6)
 
     @property
-    def mid_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 1)
+    def Ground(self) -> _elementPin.element_Pin:
+        return _elementPin.element_Pin(self, 7)
 
-    @property
-    def r_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 2)
+# 电容
+@two_pin_ArtificialCircuit_Pin
+class Basic_Capacitor(electricityBase):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
+        self._arguments = {'ModelID': 'Basic Capacitor', 'Identifier': '',
+                           'IsBroken': False, 'IsLocked': False, 'Properties': {'耐压': 16.0, '电容': 1e-06, '内阻': 5.0, '锁定': 1.0},
+                           'Statistics': {}, 'Position': '',
+                           'Rotation': '', 'DiagramCached': False,
+                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
-# 按钮开关
-@_elementClassHead.two_pin_ArtificialCircuit_Pin
-class Push_Switch(_elementClassHead.elementBase):
-    @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
-        self._arguments = {
-            'ModelID': 'Push Switch', 'Identifier': '', 'IsBroken': False, 'IsLocked': False,
-            'Properties': {'开关': 0.0, '默认开关': 0.0, '锁定': 1.0}, 'Statistics': {'电流': 0.0}, 'Position': '',
-            'Rotation': '', 'DiagramCached': False, 'DiagramPosition': {
-                'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
-
-
-# 一节电池
-@_elementClassHead.two_pin_ArtificialCircuit_Pin
-class Battery_Source(_elementClassHead.elementBase):
-    @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
-        self._arguments = {'ModelID': 'Battery Source', 'Identifier': '',
-                           'IsBroken': False, 'IsLocked': False, 'Properties': {'最大功率': 16.2, '电压': 3.0, '内阻': 0.5},
-                           'Statistics': {'电流': 0, '功率': 0, '电压': 0},
-                           'Position': '',
+# 接地
+class Ground_Component(electricityBase):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
+        self._arguments = {'ModelID': 'Ground Component', 'Identifier': '',
+                           'IsBroken': False, 'IsLocked': False, 'Properties': {'锁定': 1.0},
+                           'Statistics': {'电流': 0}, 'Position': '',
                            'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
-# 学生电源
-class Student_Source(_elementClassHead.elementBase):
-    @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
-        self._arguments = {'ModelID': 'Student Source', 'Identifier': '', 'IsBroken': False, 'IsLocked': False,
-                           'Properties': {'交流电压': 3.0, '直流电压': 3.0, '开关': 0.0, '频率': 50.0},
-                           'Statistics': {'瞬间功率': 0.0, '瞬间电压': 0.0, '瞬间电流': 0.0,
-                                          '瞬间电阻': 0.0, '功率': 0.0, '电阻': 0.0, '电流': 0.0,
-                                          '瞬间功率1': 0.0, '瞬间电压1': 0.0, '瞬间电流1': 0.0,
-                                          '瞬间电阻1': 0.0,
-                                          '功率1': 0.0, '电阻1': 0.0, '电流1': 0.0},
+    @property
+    def i(self) -> _elementPin.element_Pin:
+        return _elementPin.element_Pin(self, 0)
+
+# 运算放大器
+class Operational_Amplifier(electricityBase):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
+        self._arguments = {'ModelID': 'Operational Amplifier', 'Identifier': '',
+                           'IsBroken': False, 'IsLocked': False,
+                           'Properties': {'增益系数': 100_0000.0, '最大电压': 15.0, '最小电压': -15.0, '锁定': 1.0},
+                           'Statistics': {'电压-': 0, '电压+': 0, '输出电压': 0,
+                                          '输出电流': 0, '输出功率': 0},
                            'Position': '',
                            'Rotation': '', 'DiagramCached': False,
-                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0},
-                           'DiagramRotation': 0}
+                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
-    def l(self) -> _elementPin.element_Pin:
+    def i_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
 
     @property
-    def l_mid(self) -> _elementPin.element_Pin:
+    def i_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
     @property
-    def r_mid(self) -> _elementPin.element_Pin:
+    def o(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 2)
 
+# 继电器
+class Relay_Component(electricityBase):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
+        self._arguments = {'ModelID': 'Relay Component', 'Identifier': '', 'IsBroken': False, 'IsLocked': False,
+                           'Properties': {'开关': 0.0, '线圈电感': 0.2, '线圈电阻': 20.0,
+                                          '接通电流': 0.02, '额定电流': 1.0, '锁定': 1.0}, 'Statistics': {},
+                           'Position': '', 'Rotation': '',
+                           'DiagramCached': False, 'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0},
+                           'DiagramRotation': 0}
+
     @property
-    def r(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 3)
+    def l_up(self) -> _elementPin.element_Pin:
+        return _elementPin.element_Pin(self, 0)
 
-# 电阻
-@_elementClassHead.two_pin_ArtificialCircuit_Pin
-class Resistor(_elementClassHead.elementBase):
-    @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
-        self._arguments = {'ModelID': 'Resistor', 'Identifier': '', 'IsBroken': False,
-                           'IsLocked': False,
-                           'Properties': {'最大电阻': 1000_0000.0, '最小电阻': 0.1, '电阻': 10, '锁定': 1.0},
-                           'Statistics': {'瞬间功率': 0, '瞬间电流': 0,
-                                          '瞬间电压': 0, '功率': 0,
-                                          '电压': 0, '电流': 0},
-                           'Position': '', 'Rotation': '', 'DiagramCached': False,
-                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
+    @property
+    def l_low(self) -> _elementPin.element_Pin:
+        return _elementPin.element_Pin(self, 2)
 
-# 保险丝
-@_elementClassHead.two_pin_ArtificialCircuit_Pin
-class Fuse_Component(_elementClassHead.elementBase):
-    @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
-        self._arguments = {'ModelID': 'Fuse Component', 'Identifier': '', 'IsBroken': False, 'IsLocked': False,
-                           'Properties': {'开关': 1.0, '额定电流': 0.30000001192092896, '熔断电流': 0.5, '锁定': 1.0},
-                           'Statistics': {'瞬间功率': 0.0, '瞬间电流': 0.0, '瞬间电压': 0.0, '功率': 0.0, '电压': 0.0, '电流': 0.0},
-                           'Position': '', 'Rotation': '', 'DiagramCached': False,
-                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
+    @property
+    def mid(self) -> _elementPin.element_Pin:
+        return _elementPin.element_Pin(self, 1)
+
+    @property
+    def r_up(self) -> _elementPin.element_Pin:
+        return _elementPin.element_Pin(self, 4)
+
+    @property
+    def r_low(self) -> _elementPin.element_Pin:
+        return _elementPin.element_Pin(self, 5)
 
-# 滑动变阻器
-class Slide_Rheostat(_elementClassHead.elementBase):
-    @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
-        self._arguments = {'ModelID': 'Slide Rheostat', 'Identifier': '', 'IsBroken': False, 'IsLocked': False,
-                           'Properties': {'额定电阻': 10.0, '滑块位置': 0.0, '电阻1': 10, '电阻2': 10.0, '锁定': 1.0},
-                           'Statistics': {'瞬间功率': 0.0, '瞬间电流': 0.0, '瞬间电压': 0.0, '功率': 0.0, '电压': 0.0, '电流': 0.0,
-                                          '瞬间功率1': 0.0, '瞬间电流1': 0.0, '瞬间电压1': 0.0, '功率1': 0.0, '电压1': 0.0, '电流1': 0.0},
+# n mos
+class N_MOSFET(electricityBase):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
+        self._arguments = {'ModelID': 'N-MOSFET', 'Identifier': '', 'IsBroken': False,
+                           'IsLocked': False, 'Properties': {'PNP': 1.0, '放大系数': 0.027, '阈值电压': 1.5, '最大功率': 100.0, '锁定': 1.0},
+                           'Statistics': {'电压GS': 0.0, '电压': 0.0, '电流': 0.0, '功率': 0.0, '状态': 0.0},
                            'Position': '', 'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
-    def l_low(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 0)
+    def D(self) -> _elementPin.element_Pin:
+        return _elementPin.element_Pin(self, 2)
 
     @property
-    def r_low(self) -> _elementPin.element_Pin:
+    def S(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
     @property
-    def l_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 2)
+    def G(self) -> _elementPin.element_Pin:
+        return _elementPin.element_Pin(self, 0)
+
+# 波形发生器基类
+class _source_electricity(electricityBase):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
+        self._arguments = {'ModelID': '', 'Identifier': '',
+                           'IsBroken': False, 'IsLocked': False,
+                           'Properties': {'电压': 3.0, '内阻': 0.5, '频率': 20000.0, '偏移': 0.0, '占空比': 0.5, '锁定': 1.0},
+                           'Statistics': {'电流': 0.0, '功率': 0.0, '电压': -3.0},
+                           'Position': '', 'Rotation': '', 'DiagramCached': False,
+                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
-    def r_up(self) -> _elementPin.element_Pin:
-        return _elementPin.element_Pin(self, 3)
+    def l(self) -> _elementPin.element_Pin:
+        return _elementPin.element_Pin(self, 0)
+    i = l
+
+    @property
+    def r(self) -> _elementPin.element_Pin:
+        return _elementPin.element_Pin(self, 1)
+    o = r
+
+# 正弦波发生器
+class Sinewave_Source(_source_electricity):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
+        super(Sinewave_Source, self).__init__(x, y, z, elementXYZ)
+        self._arguments['ModelID'] = 'Sinewave Source'
+
+# 方波发生器
+class Square_Source(_source_electricity):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
+        super(Square_Source, self).__init__(x, y, z, elementXYZ)
+        self._arguments['ModelID'] = 'Square Source'
+
+# 三角波发生器
+class Triangle_Source(_source_electricity):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
+        super(Triangle_Source, self).__init__(x, y, z, elementXYZ)
+        self._arguments['ModelID'] = 'Triangle Source'
+
+# 锯齿波发生器
+class Sawtooth_Source(_source_electricity):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
+        super(Sawtooth_Source, self).__init__(x, y, z, elementXYZ)
+        self._arguments['ModelID'] = 'Sawtooth Source'
+
+# 尖峰波发生器
+class Pulse_Source(_source_electricity):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
+        super(Pulse_Source, self).__init__(x, y, z, elementXYZ)
+        self._arguments['ModelID'] = 'Pulse Source'
```

### Comparing `physicsLab-1.2.2/physicsLab/electricity/elementsClass/logicCircuit.py` & `physicsLab-1.3.0/physicsLab/electricity/elementsClass/logicCircuit.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,64 @@
 #coding=utf-8
-import physicsLab._tools as _tools
+from physicsLab._tools import numType
 import physicsLab.electricity.elementPin as _elementPin
-import physicsLab.electricity.elementsClass._elementClassHead as _elementClassHead
+from ._elementClassHead import electricityBase, is_big_element
 
-class _logicBase(_elementClassHead.elementBase):
+class _logicBase(electricityBase):
     # 设置高电平的值
-    def set_HighLeaveValue(self, num: _tools.numType) -> None:
+    def set_HighLeaveValue(self, num: numType) -> None:
         if not isinstance(num, (int, float)):
             raise RuntimeError('illegal argument')
         self._arguments['Properties']['高电平'] = num
 
     # 设置低电平的值
-    def set_LowLeaveValue(self, num: _tools.numType) -> None:
+    def set_LowLeaveValue(self, num: numType) -> None:
         if not isinstance(num, (int, float)):
             raise RuntimeError('illegal argument')
         self._arguments['Properties']['低电平'] = num
 
 
 # _arguments是参数的意思
 
 # 逻辑输入
 class Logic_Input(_logicBase):
-    @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         self._arguments = {"ModelID": "Logic Input", "Identifier": "",
                           "IsBroken": False, "IsLocked": False, "Properties": {"高电平": 3.0, "低电平": 0.0, "锁定": 1.0, "开关": 0},
                           "Statistics": {"电流": 0.0, "电压": 0.0, "功率": 0.0},
                           "Position": "",
                           "Rotation": "", "DiagramCached": False,
                           "DiagramPosition": {"X": 0, "Y": 0, "Magnitude": 0.0},
                           "DiagramRotation": 0}
 
-    def set_highLevel(self) -> None:
+    def set_highLevel(self) -> "Logic_Input":
         self._arguments['Properties']['开关'] = 1.0
+        return self
 
     @property
     def o(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 0)
 
 # 逻辑输出
 class Logic_Output(_logicBase):
-    @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': 'Logic Output', 'Identifier': "",
                           'IsBroken': False, 'IsLocked': False,
                           'Properties': {'状态': 0.0, '高电平': 3.0, '低电平': 0.0, '锁定': 1.0}, 'Statistics': {},
                           'Position': "",
                           'Rotation': '0,180,0', 'DiagramCached': False,
                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
     def i(self) -> _elementPin.element_Pin:
             return _elementPin.element_Pin(self, 0)
 
 # 2引脚门电路
 class _2_pin_Gate(_logicBase):
-    @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': '', 'Identifier': "", 'IsBroken': False,
                           'IsLocked': False, 'Properties': {'高电平': 3.0, '低电平': 0.0, '最大电流': 0.1, '锁定': 1.0},
                           'Statistics': {}, 'Position': "", 'Rotation': '', 'DiagramCached': False,
                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
     def i(self) -> _elementPin.element_Pin:
@@ -68,28 +66,27 @@
 
     @property
     def o(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
 # 是门
 class Yes_Gate(_2_pin_Gate):
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(Yes_Gate, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'Yes Gate'
 
 # 非门
 class No_Gate(_2_pin_Gate):
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(No_Gate, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'No Gate'
 
 # 3引脚门电路
 class _3_pin_Gate(_logicBase):
-    @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': '', 'Identifier': '', 'IsBroken': False,
                           'IsLocked': False, 'Properties': {'高电平': 3.0, '低电平': 0.0, '最大电流': 0.1, '锁定': 1.0},
                           'Statistics': {}, 'Position': "", 'Rotation': "", 'DiagramCached': False,
                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     @property
     def i_up(self) -> _elementPin.element_Pin:
@@ -101,73 +98,71 @@
 
     @property
     def o(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 2)
 
 # 或门
 class Or_Gate(_3_pin_Gate):
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(Or_Gate, self).__init__(x, y, z, elementXYZ)
         self._arguments["ModelID"] = 'Or Gate'
 
 # 与门
 class And_Gate(_3_pin_Gate):
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(And_Gate, self).__init__(x, y, z, elementXYZ)
         self._arguments["ModelID"] = 'And Gate'
 
 # 或非门
 class Nor_Gate(_3_pin_Gate):
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(Nor_Gate, self).__init__(x, y, z, elementXYZ)
         self._arguments["ModelID"] = 'Nor Gate'
 
 # 与非门
 class Nand_Gate(_3_pin_Gate):
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(Nand_Gate, self).__init__(x, y, z, elementXYZ)
         self._arguments["ModelID"] = 'Nand Gate'
 
 # 异或门
 class Xor_Gate(_3_pin_Gate):
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(Xor_Gate, self).__init__(x, y, z, elementXYZ)
         self._arguments["ModelID"] = 'Xor Gate'
 
 # 同或门
 class Xnor_Gate(_3_pin_Gate):
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(Xnor_Gate, self).__init__(x, y, z, elementXYZ)
         self._arguments["ModelID"] = 'Xnor Gate'
 
 # 蕴含门
 class Imp_Gate(_3_pin_Gate):
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(Imp_Gate, self).__init__(x, y, z, elementXYZ)
         self._arguments["ModelID"] = 'Imp Gate'
 
 # 蕴含非门
 class Nimp_Gate(_3_pin_Gate):
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(Nimp_Gate, self).__init__(x, y, z, elementXYZ)
         self._arguments["ModelID"] = 'Nimp Gate'
 
 # 2体积元件父类
-class _big_element(_logicBase):
-    @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+class _big_element(_logicBase, is_big_element):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': '', 'Identifier': '', 'IsBroken': False,
                           'IsLocked': False, 'Properties': {'高电平': 3.0, '低电平': 0.0, '锁定': 1.0}, 'Statistics': {},
                           'Position': '', 'Rotation': '', 'DiagramCached': False,
                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
-        _elementClassHead.is_big_Element = True
 
 # 半加器
 class Half_Adder(_big_element):
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(Half_Adder, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'Half Adder'
 
     @property
     def i_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 2)
 
@@ -181,15 +176,15 @@
 
     @property
     def o_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
 # 全加器
 class Full_Adder(_big_element):
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(Full_Adder, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'Full Adder'
 
     @property
     def i_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 2)
 
@@ -207,15 +202,15 @@
 
     @property
     def o_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
 # 二位乘法器
 class Multiplier(_big_element):
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(Multiplier, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'Multiplier'
 
     @property
     def i_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 4)
 
@@ -245,15 +240,15 @@
 
     @property
     def o_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 3)
 
 # D触发器
 class D_Flipflop(_big_element):
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(D_Flipflop, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'D Flipflop'
 
     @property
     def i_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 2)
 
@@ -267,15 +262,15 @@
 
     @property
     def o_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
 # T触发器
 class T_Flipflop(_big_element):
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(T_Flipflop, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'T Flipflop'
 
     @property
     def i_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 2)
 
@@ -289,15 +284,15 @@
 
     @property
     def o_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
 # JK触发器
 class JK_Flipflop(_big_element):
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(JK_Flipflop, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'JK Flipflop'
 
     @property
     def i_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 2)
 
@@ -315,15 +310,15 @@
 
     @property
     def o_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 1)
 
 # 计数器
 class Counter(_big_element):
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(Counter, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'Counter'
 
     @property
     def i_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 4)
 
@@ -345,15 +340,15 @@
 
     @property
     def o_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 3)
 
 # 随机数发生器
 class Random_Generator(_big_element):
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         super(Random_Generator, self).__init__(x, y, z, elementXYZ)
         self._arguments['ModelID'] = 'Random Generator'
 
     @property
     def i_up(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 4)
 
@@ -374,17 +369,16 @@
         return _elementPin.element_Pin(self, 2)
 
     @property
     def o_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 3)
 
 # 8位输入器
-class eight_bit_Input(_logicBase):
-    @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+class eight_bit_Input(_logicBase, is_big_element):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': '8bit Input', 'Identifier': '', 'IsBroken': False,
                            'IsLocked': False, 'Properties': {'高电平': 3.0, '低电平': 0.0, '十进制': 0.0, '锁定': 1.0},
                            'Statistics': {}, 'Position': '', 'Rotation': '', 'DiagramCached': False,
                            'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
 
     def set_num(self, num : int):
         if 0 <= num <= 255:
@@ -421,17 +415,16 @@
         return _elementPin.element_Pin(self, 6)
 
     @property
     def o_low(self) -> _elementPin.element_Pin:
         return _elementPin.element_Pin(self, 7)
 
 # 8位显示器
-class eight_bit_Display(_logicBase):
-    @_elementClassHead.element_Init_HEAD
-    def __init__(self, x: _tools.numType = 0, y: _tools.numType = 0, z: _tools.numType = 0, elementXYZ = None):
+class eight_bit_Display(_logicBase, is_big_element):
+    def __init__(self, x: numType = 0, y: numType = 0, z: numType = 0, elementXYZ = None):
         self._arguments = {'ModelID': '8bit Display', 'Identifier': '',
                           'IsBroken': False, 'IsLocked': False,
                           'Properties': {'高电平': 3.0, '低电平': 0.0, '状态': 0.0, '锁定': 1.0},
                           'Statistics': {'7': 0.0, '6': 0.0, '5': 0.0, '4': 0.0, '3': 0.0, '2': 0.0, '1': 0.0, '0': 0.0,
                                          '十进制': 0.0}, 'Position': '',
                           'Rotation': '', 'DiagramCached': False,
                           'DiagramPosition': {'X': 0, 'Y': 0, 'Magnitude': 0.0}, 'DiagramRotation': 0}
```

### Comparing `physicsLab-1.2.2/physicsLab/electricity/unionElements/_unionClassHead.py` & `physicsLab-1.3.0/physicsLab/electricity/unionElements/_unionClassHead.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,34 @@
 #coding=utf-8
 import physicsLab._tools as _tools
+import physicsLab.errors as errors
+import physicsLab._fileGlobals as _fileGlobals
 import physicsLab.electricity.elementXYZ as _elementXYZ
-# Union class的基类
-class unionBase:
+import physicsLab.electricity.elementsClass as _elementsClass
+
+class UnionMeta(type):
+    def __new__(metaCls, name: str, base: tuple, attrs: dict):
+        cls = metaCls.__new__(metaCls, name, base, attrs)
+        # obj = cls.__new__()
+        # obj.__init__()
+        pass
+        return type.__new__(name, base, attrs)
+
+# Union class的基类 MixIn Class
+class UnionBase:
+    # 此类无法被实例化
+    def __init__(self, *args, **kwargs):
+        raise errors.instantiateError
+
     # 获取以模块化电路生成顺序为item的原件的self
-    def __getitem__(self, item):
-        return self.__elements[item]
+    # 一定有self._elements
+    def __getitem__(self, item: int) -> "_elementsClass.electricityBase":
+        if not isinstance(item, int):
+            raise TypeError
+        return self._elements[item]
     # 设置坐标
     def set_Position(self, x, y, z):
         pass
 
 # union class __init__装饰器
 def union_Init_HEAD(
         x: _tools.numType,
@@ -17,26 +36,27 @@
         z: _tools.numType,
         bitLength: int,
         elementXYZ: bool,  # x, y, z是否为元件坐标系
         unionHeading: bool,  # False: 生成的元件为竖直方向，否则为横方向
         fold: bool,  # False: 生成元件时不会在同一水平面的元件超过一定数量后z + 1继续生成元件
         foldMaxNum: int  # 达到foldMaxNum个元件数时即在z轴自动折叠
 ):
+    _fileGlobals.check_ExperimentType(0)
         # input type check
     if foldMaxNum <= 0 or not(
         isinstance(x, (int, float)) or
         isinstance(y, (int, float)) or
         isinstance(z, (int, float)) or
         isinstance(elementXYZ, bool) or
         isinstance(unionHeading, bool) or
         isinstance(fold, bool) or
         isinstance(foldMaxNum, int)
     ):
         raise TypeError
-    if not isinstance(bitLength, int):
-        raise TypeError("bitLength must get a integer")
+    if not isinstance(bitLength, int) or bitLength < 1:
+        raise errors.bitLengthError("bitLength must get a integer")
 
     # 元件坐标系，如果输入坐标不是元件坐标系就强转为元件坐标系
     if not (elementXYZ == True or (_elementXYZ.is_elementXYZ() == True and elementXYZ is None)):
         x, y, z = _elementXYZ.translateXYZ(x, y, z)
 
     return _tools.roundData(x, y, z)
```

### Comparing `physicsLab-1.2.2/physicsLab/electricity/unionElements/unionLogic.py` & `physicsLab-1.3.0/physicsLab/electricity/unionElements/unionLogic.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,255 @@
 #coding=utf-8
 # 模块化电路
 import typing as _typing
 import physicsLab._tools as _tools
+import physicsLab.errors as _errors
 import physicsLab.electricity as electricity
-import physicsLab.electricity.elementXYZ as _elementXYZ
 import physicsLab.electricity.elementsClass as _elementsClass
-from physicsLab.electricity.unionElements.unionPin import unionPin
+from physicsLab.electricity.unionElements.unionPin import union_Pin
 import physicsLab.electricity.unionElements._unionClassHead as _unionClassHead
 
+# unionHeading与fold的判断的代码
+def _unionHeading_fold(
+        func1: _typing.Callable,
+        func2: _typing.Callable,
+        func3: _typing.Callable,
+        func4: _typing.Callable,
+        unionHeading: bool,
+        fold: bool
+):
+    if unionHeading: # 生成元件为横方向
+        if fold: # z轴折叠
+            func1()
+        else:
+            func2()
+    else: # 竖方向
+        if fold:
+            func3()
+        else:
+            func4()
+
+# 用metaClass检查是否有self._elements
+class _union_LogicMeta(type):
+    pass
+
+# 模块化电路逻辑电路基类
+class Union_LogicBase(_unionClassHead.UnionBase):
+    # 设置高电平的值
+    def set_HighLeaveValue(self, num: _tools.numType) -> "Union_LogicBase":
+        for element in self._elements:
+            element.set_HighLeaveValue(num)
+        return self
+
+    def set_LowLeaveValue(self, num: _tools.numType) -> "Union_LogicBase":
+        for element in self._elements:
+            element.set_LowLeaveValue(num)
+        return self
+
 # 任意引脚加法电路
-class union_Sum:
-    def __init__(self, x : _tools.numType = 0, y : _tools.numType = 0, z : _tools.numType = 0, bitCount : int = 1):
-        if not (
-                isinstance(x, (float, int)) and isinstance(y, (float, int)) and
-                isinstance(z, (float, int)) and isinstance(bitCount, int) and bitCount > 0
-        ):
-            raise RuntimeError('Error in input parameters')
-        x, y, z = _tools.roundData(x), _tools.roundData(y), _tools.roundData(z)
-        electricity.Full_Adder(x, y, z)
-        for count in range(1, bitCount):
-            if count % 8 != 0:
-                y = _tools.roundData(y + 0.2)
-                electricity.crt_Wire(
-                    electricity.Full_Adder(x, y, z).i_low,
-                    electricity.get_Element(x, y - 0.2, z).o_low
+class Sum(Union_LogicBase):
+    def __init__(
+            self,
+            x: _tools.numType = 0,
+            y: _tools.numType = 0,
+            z: _tools.numType = 0,
+            bitLength: int = None,
+            elementXYZ: bool = None,  # x, y, z是否为元件坐标系
+            unionHeading: bool = False,  # False: 生成的元件为竖直方向，否则为横方向
+            fold: bool = False,  # False: 生成元件时不会在同一水平面的元件超过一定数量后z + 1继续生成元件
+            foldMaxNum: int = 4  # 达到foldMaxNum个元件数时即在z轴自动折叠
+    ) -> None:
+        def link_union_Sum(elements: _typing.List[_elementsClass.Full_Adder]) -> None:
+            for i in range(elements.__len__() - 1):
+                elements[i].o_low - elements[i + 1].i_low
+
+        def func1():
+            zcor = z
+            for i in range(bitLength):
+                self._elements.append(
+                    electricity.Full_Adder(x + i % foldMaxNum, y, zcor, True)
                 )
-            else:
-                y -= 1.4
-                z = _tools.roundData(z + 0.1)
-                electricity.crt_Wire(
-                    electricity.Full_Adder(x, y, z).i_low,
-                    electricity.get_Element(x, y + 1.4, z - 0.1).o_low
+                if i == foldMaxNum - 1:
+                    zcor += 1
+
+        def func2():
+            for increase in range(bitLength):
+                self._elements.append(
+                    electricity.Full_Adder(x + increase, y, z, True)
+                )
+
+        def func3():
+            zcor = z
+            for i in range(bitLength):
+                self._elements.append(
+                    electricity.Full_Adder(x, y + (i % foldMaxNum) * 2, zcor, True)
+                )
+                if i == foldMaxNum - 1:
+                    zcor += 1
+
+        def func4():
+            for increase in range(bitLength):
+                self._elements.append(
+                    electricity.Full_Adder(x, y + increase * 2, z, True)
                 )
 
+        # main
+        # if bitLength < 2:
+        #     raise errors.bitLengthError
+
+        x, y, z = _unionClassHead.union_Init_HEAD(
+            x, y, z,
+            bitLength,
+            elementXYZ,
+            unionHeading,
+            fold,
+            foldMaxNum
+        )
+
+        self._elements: _typing.List[_elementsClass.Full_Adder] = []
+        _unionHeading_fold(
+            func1, func2, func3, func4, unionHeading, fold
+        )
+        link_union_Sum(self._elements)
+
+    @property
+    def data_Input1(self) -> union_Pin:
+        return union_Pin(
+            self,
+            *(element.i_mid for element in self._elements)
+        )
+
+    @property
+    def data_Input2(self) -> union_Pin:
+        return union_Pin(
+            self,
+            *(element.i_up for element in self._elements)
+        )
+
+    @property
+    def data_Output(self) -> union_Pin:
+        return union_Pin(
+            self,
+            *(element.o_up for element in self._elements),
+            self._elements[-1].o_low
+        )
+
 # 任意引脚减法电路
-class union_Sub:
-    pass
+class Sub(Union_LogicBase):
+    def __init__(
+            self,
+            x: _tools.numType = 0,
+            y: _tools.numType = 0,
+            z: _tools.numType = 0,
+            bitLength: int = None,
+            elementXYZ: bool = None,  # x, y, z是否为元件坐标系
+            unionHeading: bool = False,  # False: 生成的元件为竖直方向，否则为横方向
+            fold: bool = False,  # False: 生成元件时不会在同一水平面的元件超过一定数量后z + 1继续生成元件
+            foldMaxNum: int = 4  # 达到foldMaxNum个元件数时即在z轴自动折叠
+    ) -> None:
+        def link_union_Sub(
+                fullAdders: _typing.List[_elementsClass.Full_Adder],
+                noGates: _typing.List[_elementsClass.No_Gate]
+        ) -> None:
+            self._elements[0].o - fullAdders[0].i_low
+            for i in range(fullAdders.__len__() - 1):
+                fullAdders[i].o_low - fullAdders[i + 1].i_low
+                noGates[i].o - fullAdders[i].i_mid
+            noGates[-1].o - fullAdders[-1].i_mid
+
+        def func1():
+            zcor = z
+            for i in range(bitLength):
+                self._fullAdders.append(
+                    electricity.Full_Adder(x + i % foldMaxNum, y - 2, zcor, True)
+                )
+                self._noGates.append(
+                    electricity.No_Gate(x + i % foldMaxNum, y, zcor, True)
+                )
+                if i == foldMaxNum - 1:
+                    zcor += 1
+
+        def func2():
+            for increase in range(bitLength):
+                self._fullAdders.append(
+                    electricity.Full_Adder(x + increase, y - 2, z, True)
+                )
+                self._noGates.append(
+                    electricity.No_Gate(x + increase, y, z, True)
+                )
+
+        def func3():
+            zcor = z
+            for i in range(bitLength):
+                self._fullAdders.append(
+                    electricity.Full_Adder(x + 1, y + (i % foldMaxNum) * 2, zcor, True)
+                )
+                self._noGates.append(
+                    electricity.No_Gate(x, y + (i % foldMaxNum) * 2 + 1, zcor, True)
+                )
+                if i == foldMaxNum - 1:
+                    zcor += 1
+
+        def func4():
+            for increase in range(bitLength):
+                self._fullAdders.append(
+                    electricity.Full_Adder(x + 1, y + increase * 2, z, True)
+                )
+                self._noGates.append(
+                    electricity.No_Gate(x, y + increase * 2 + 1, z, True)
+                )
+
+        x, y, z = _unionClassHead.union_Init_HEAD(
+            x, y, z,
+            bitLength,
+            elementXYZ,
+            unionHeading,
+            fold,
+            foldMaxNum
+        )
+
+        self._elements: _typing.List[_typing.Union[_elementsClass.Full_Adder, _elementsClass.No_Gate]] = [
+            _elementsClass.No_Gate(x, y, z, True)
+        ]
+
+        self._noGates: _typing.List[_elementsClass.No_Gate] = []
+        self._fullAdders: _typing.List[_elementsClass.Full_Adder] = []
+
+        _unionHeading_fold(
+            func1, func2, func3, func4, unionHeading, fold
+        )
+        link_union_Sub(self._fullAdders, self._noGates)
+        self._elements.extend(self._fullAdders + self._noGates)
+
+    # 被减数
+    @property
+    def minuend(self) -> union_Pin:
+        return union_Pin(
+            self,
+            *(e.i_up for e in self._fullAdders)
+        )
+
+    # 减数
+    @property
+    def subtrahend(self):
+        return union_Pin(
+            self,
+            *(e.i for e in self._noGates)
+        )
+
+    @property
+    def outputs(self):
+        return union_Pin(
+            self,
+            *(e.o_up for e in self._fullAdders),
+            self._fullAdders[-1].o_low
+        )
 
 # 2-4译码器
-class union_2_4_Decoder:
+class _two_four_Decoder:
     def __init__(self, x : _tools.numType = 0, y : _tools.numType = 0, z : _tools.numType = 0):
         if not (isinstance(x, (int, float)) and isinstance(y, (int, float)) and isinstance(z, (int, float))):
             raise RuntimeError('illegal argument')
         self.x = x
         self.y = y
         self.z = z
         obj1 = electricity.Nor_Gate(x, y, z)
@@ -57,15 +264,15 @@
         return electricity.element_Pin(electricity.get_Element(self.x, self.y + 0.3, self.z), 0)
 
     @property
     def i_low(self):
         return electricity.element_Pin(electricity.get_Element(self.x, self.y + 0.3, self.z), 1)
 
 # 4-16译码器
-class union_4_16_Decoder:
+class _four_sixteen_Decoder:
     def __init__(self, x : _tools.numType = 0, y : _tools.numType = 0, z : _tools.numType = 0):
         if not (isinstance(x, (int, float)) and isinstance(y, (int, float)) and isinstance(z, (int, float))):
             raise RuntimeError('illegal argument')
         self.x = x
         self.y = y
         self.z = z
         obj1 = electricity.Nor_Gate(x, y, z); obj2 = electricity.Nimp_Gate(x, y + 0.1, z)
@@ -87,15 +294,15 @@
                     electricity.crt_Wire(obj4.o, obj.i_up)
                 eval(f'crt_Wire(obj{round((i - 0.3) / 0.15) + 5}.o, obj.i_upmid)')
                 eval(f'crt_Wire(obj{round((i - 0.3) / 0.15) + 5}.o, obj.i_lowmid)')
 
     # 输入译码器的数据
     @property
     def inputData(self):
-        return unionPin(
+        return union_Pin(
             electricity.element_Pin(electricity.get_Element(self.x + 0.15, self.y + 0.3, self.z), 0),
             electricity.element_Pin(electricity.get_Element(self.x + 0.15, self.y + 0.3, self.z), 1),
             electricity.element_Pin(electricity.get_Element(self.x, self.y + 0.3, self.z), 0),
             electricity.element_Pin(electricity.get_Element(self.x, self.y + 0.3, self.z), 1)
         )
 
     # 输出译码器的数据
@@ -178,36 +385,16 @@
     def o14(self):
         return electricity.get_Element(self.x + 0.3, self.y + 0.25, self.z).o_lowmid
 
     @property
     def o15(self):
         return electricity.get_Element(self.x + 0.3, self.y + 0.25, self.z).o_upmid
 
-# unionHeading与fold的判断的代码
-def _unionHeading_fold(
-        func1: _typing.Callable,
-        func2: _typing.Callable,
-        func3: _typing.Callable,
-        func4: _typing.Callable,
-        unionHeading: bool,
-        fold: bool
-):
-    if unionHeading: # 生成元件为横方向
-        if fold: # z轴折叠
-            func1()
-        else:
-            func2()
-    else: # 竖方向
-        if fold:
-            func3()
-        else:
-            func4()
-
 # 多个逻辑输入（暂不支持m * n矩阵排列元件的方式）
-class inputs(_unionClassHead.unionBase):
+class Inputs(Union_LogicBase):
     def __init__(
             self,
             x: _tools.numType = 0,
             y: _tools.numType = 0,
             z: _tools.numType = 0,
             bitLength: int = None,
             elementXYZ: bool = None,  # x, y, z是否为元件坐标系
@@ -215,62 +402,65 @@
             fold: bool = False,  # False: 生成元件时不会在同一水平面的元件超过一定数量后z + 1继续生成元件
             foldMaxNum: int = 8  # 达到foldMaxNum个元件数时即在z轴自动折叠
     ) -> None:
         # 搭配_unionHeading_fold使用
         def func1():
             zcor = z
             for i in range(bitLength):
-                self.__elements.append(
+                self._elements.append(
                     electricity.Logic_Input(x + i % foldMaxNum, y, zcor, True)
                 )
                 if i == foldMaxNum - 1:
                     zcor += 1
 
         def func2():
             for i in range(bitLength):
-                self.__elements.append(
+                self._elements.append(
                     _elementsClass.Logic_Input(x + i, y, z, True)
                 )
 
         def func3():
             zcor = z
             for i in range(bitLength):
-                self.__elements.append(
+                self._elements.append(
                     electricity.Logic_Input(x, y + i % foldMaxNum, zcor, True)
                 )
                 if i == foldMaxNum - 1:
                     zcor += 1
 
         def func4():
             for i in range(bitLength):
-                self.__elements.append(
+                self._elements.append(
                     _elementsClass.Logic_Input(x, y + i, z, True)
                 )
 
         # main
         x, y, z = _unionClassHead.union_Init_HEAD(
             x, y, z,
             bitLength,
             elementXYZ,
             unionHeading,
             fold,
             foldMaxNum
         )
 
-        self.__elements: _typing.List[_elementsClass.Logic_Input] = []
+        self._elements: _typing.List[_elementsClass.Logic_Input] = []
         _unionHeading_fold(
             func1, func2, func3, func4, unionHeading, fold
         )
 
     @property
-    def data_Output(self) -> unionPin:
-        return unionPin(*(element.o for element in self.__elements))
+    def data_Output(self) -> union_Pin:
+        return union_Pin(
+            self,
+            *(element.o for element in self._elements)
+        )
 
 # 多个逻辑输入（暂不支持m * n矩阵排列元件的方式）
-class outputs(_unionClassHead.unionBase):
+class Outputs(Union_LogicBase):
     def __init__(
             self,
             x: _tools.numType = 0,
             y: _tools.numType = 0,
             z: _tools.numType = 0,
             bitLength: int = None,
             elementXYZ: bool = None,  # x, y, z是否为元件坐标系
@@ -278,134 +468,164 @@
             fold: bool = False,  # False: 生成元件时不会在同一水平面的元件超过一定数量后z + 1继续生成元件
             foldMaxNum: int = 8  # 达到foldMaxNum个元件数时即在z轴自动折叠
     ) -> None:
         # 搭配_unionHeading_fold使用
         def func1():
             zcor = z
             for i in range(bitLength):
-                self.__elements.append(
+                self._elements.append(
                     electricity.Logic_Output(x + i % foldMaxNum, y, zcor, True)
                 )
                 if i == foldMaxNum - 1:
                     zcor += 1
 
         def func2():
             for i in range(bitLength):
-                self.__elements.append(
+                self._elements.append(
                     _elementsClass.Logic_Output(x + i, y, z, True)
                 )
 
         def func3():
             zcor = z
             for i in range(bitLength):
-                self.__elements.append(
+                self._elements.append(
                     electricity.Logic_Output(x, y + i % foldMaxNum, zcor, True)
                 )
                 if i == foldMaxNum - 1:
                     zcor += 1
 
         def func4():
             for i in range(bitLength):
-                self.__elements.append(
+                self._elements.append(
                     _elementsClass.Logic_Output(x, y + i, z, True)
                 )
 
         # main
         x, y, z = _unionClassHead.union_Init_HEAD(
             x, y, z,
             bitLength,
             elementXYZ,
             unionHeading,
             fold,
             foldMaxNum
         )
 
-        self.__elements: _typing.List[_elementsClass.Logic_Output] = []
+        self._elements: _typing.List[_elementsClass.Logic_Output] = []
         _unionHeading_fold(
             func1, func2, func3, func4, unionHeading, fold
         )
 
     @property
-    def data_Input(self) -> unionPin:
-        return unionPin(*(element.i for element in self.__elements))
+    def data_Input(self) -> union_Pin:
+        return union_Pin(
+            self,
+            *(element.i for element in self._elements)
+        )
 
 # D触发器流水灯
-class d_WaterLamp(_unionClassHead.unionBase):
+class D_WaterLamp(Union_LogicBase):
     def __init__(
             self,
             x: _tools.numType = 0,
             y: _tools.numType = 0,
             z: _tools.numType = 0,
             bitLength: int = None,
             elementXYZ: bool = None, # x, y, z是否为元件坐标系
             unionHeading: bool = False, # False: 生成的元件为竖直方向，否则为横方向
             fold: bool = False, # False: 生成元件时不会在同一水平面的元件超过一定数量后z + 1继续生成元件
-            foldMaxNum: int = 4 # 达到foldMaxNum个元件数时即在z轴自动折叠
+            foldMaxNum: int = 4, # 达到foldMaxNum个元件数时即在z轴自动折叠
+            is_loop: bool = True # 是否使流水灯循环
     ) -> None:
         # D触流水灯导线连接方式
         def link_D_Flipflop(elements: _typing.List[_elementsClass.D_Flipflop]) -> None:
             # 连接clk
             for i in range(len(elements) - 1):
                 elements[i].i_low - elements[i + 1].i_low
             # 连接数据传输导线
             elements[0].o_low - elements[1].i_up
             for i in range(1, len(elements) - 1):
                 elements[i].o_up - elements[i + 1].i_up
             # 流水灯循环导线
-            elements[-1].o_low - elements[0].i_up
+            if is_loop:
+                elements[-1].o_low - elements[0].i_up
+            else:
+                firstElement = elements[0]
+                orGate = _elementsClass.Or_Gate(*firstElement.get_Position(), True)
+                orGate.i_up - orGate.o
+                orGate.o - firstElement.i_up
+                orGate.i_low - firstElement.i_low
 
         def func1():
             zcor = z
             for i in range(bitLength):
-                self.__elements.append(
+                self._elements.append(
                     electricity.D_Flipflop(x + i % foldMaxNum, y, zcor, True)
                 )
                 if i == foldMaxNum - 1:
                     zcor += 1
 
         def func2():
             for increase in range(bitLength):
-                self.__elements.append(
+                self._elements.append(
                     electricity.D_Flipflop(x + increase, y, z, True)
                 )
 
         def func3():
             zcor = z
             for i in range(bitLength):
-                self.__elements.append(
+                self._elements.append(
                     electricity.D_Flipflop(x, y + (i % foldMaxNum) * 2, zcor, True)
                 )
                 if i == foldMaxNum - 1:
                     zcor += 1
 
         def func4():
             for increase in range(bitLength):
-                self.__elements.append(
+                self._elements.append(
                     electricity.D_Flipflop(x, y + increase * 2, z, True)
                 )
 
         # main
+        if bitLength < 2:
+            raise _errors.bitLengthError
+
         x, y, z = _unionClassHead.union_Init_HEAD(
             x, y, z,
             bitLength,
             elementXYZ,
             unionHeading,
             fold,
             foldMaxNum
         )
 
-        self.__elements: _typing.List[_elementsClass.D_Flipflop] = []
+        if not isinstance(is_loop, bool):
+            raise TypeError
+
+        self._elements: _typing.List[_elementsClass.D_Flipflop] = []
         _unionHeading_fold(
             func1, func2, func3, func4, unionHeading, fold
         )
-        link_D_Flipflop(self.__elements)
+        link_D_Flipflop(self._elements)
 
     @property
-    def data_Input(self) -> unionPin:
-        return unionPin(self.__elements[0].i_low)
+    def data_Input(self) -> union_Pin:
+        return union_Pin(
+            self,
+            self._elements[0].i_low
+        )
 
     @property
-    def data_Output(self) -> unionPin:
-        return unionPin(
-            self.__elements[0].o_low,
-            *(element.o_up for element in self.__elements[1:])
+    def data_Output(self) -> union_Pin:
+        return union_Pin(
+            self,
+            self._elements[0].o_low,
+            *(element.o_up for element in self._elements[1:])
+        )
+
+    # 与data_Output相反的引脚
+    @property
+    def neg_data_Output(self) -> union_Pin:
+        return union_Pin(
+            self,
+            self._elements[0].o_up,
+            *(element.o_low for element in self._elements[1:])
         )
```

### Comparing `physicsLab-1.2.2/physicsLab/electricity/unionElements/unionPin.py` & `physicsLab-1.3.0/physicsLab/electricity/unionElements/unionPin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 #coding=utf-8
 import typing as _typing
 import physicsLab.electricity.elementPin as elementPin
 from physicsLab.electricity.unionElements.wires import crt_Wires
+import physicsLab.electricity.unionElements._unionClassHead as _unionClassHead
 
 # 模块化电路的“引脚”，输入输出都是数据
-class unionPin:
-    __slots__ = ("elementPins")
-    def __init__(
-            self,
-            *elementPins,
-    ):
+class union_Pin:
+    __slots__ = ("union_self", "elementPins")
+    def __init__(self, union_self: _unionClassHead.UnionBase, *elementPins):
+        self.union_self = union_self
         self.elementPins: _typing.Tuple[elementPin.element_Pin] = tuple(elementPins)
 
     # 通过unionPin[num]来索引单个bit
     def __getitem__(self, item):
-        pass
+        return self.elementPins[item]
 
-    def __sub__(self, other: "unionPin"):
+    def __sub__(self, other: "union_Pin"):
         crt_Wires(self, other)
```

### Comparing `physicsLab-1.2.2/physicsLab/electricity/unionElements/wires.py` & `physicsLab-1.3.0/physicsLab/electricity/unionElements/wires.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,47 +3,50 @@
 import physicsLab.errors as errors
 import physicsLab.electricity.elementPin as _elementPin
 from physicsLab.electricity.wire import crt_Wire, del_Wire
 import physicsLab.electricity.unionElements.unionPin as _unionPin
 
 def check_TypeUnionPin(func: Callable):
     def result(
-        sourcePin: Union["_unionPin.unionPin", "_elementPin.element_Pin"],
-        targetPin: Union["_unionPin.unionPin", "_elementPin.element_Pin"],
+        sourcePin: Union["_unionPin.union_Pin", "_elementPin.element_Pin"],
+        targetPin: Union["_unionPin.union_Pin", "_elementPin.element_Pin"],
         color="蓝"
     ) -> None:
         if isinstance(sourcePin, _elementPin.element_Pin):
-            sourcePin = _unionPin.unionPin(sourcePin)
+            sourcePin = _unionPin.union_Pin(sourcePin.element_self, sourcePin)
         if isinstance(targetPin, _elementPin.element_Pin):
-            targetPin = _unionPin.unionPin(targetPin)
+            targetPin = _unionPin.union_Pin(targetPin.element_self, targetPin)
 
         if not (
-            isinstance(sourcePin, _unionPin.unionPin) or
-            isinstance(targetPin, _unionPin.unionPin)
+                isinstance(sourcePin, _unionPin.union_Pin) or
+                isinstance(targetPin, _unionPin.union_Pin)
         ):
             raise TypeError
 
         if len(sourcePin.elementPins) != len(targetPin.elementPins):
-            errors.warning("The number of input and output pins is not equal")
+            errors.warning(
+                f"The number of {sourcePin.union_self.__class__.__name__}'s output pin "
+                f"are not equal to {targetPin.union_self.__class__.__name__}'s input pin."
+            )
 
         func(sourcePin, targetPin, color)
     return result
 
 # 为unionPin连接导线，相当于自动对数据进行连接导线
 @check_TypeUnionPin
 def crt_Wires(
-        sourcePin: Union["_unionPin.unionPin", "_elementPin.element_Pin"],
-        targetPin: Union["_unionPin.unionPin", "_elementPin.element_Pin"],
+        sourcePin: Union["_unionPin.union_Pin", "_elementPin.element_Pin"],
+        targetPin: Union["_unionPin.union_Pin", "_elementPin.element_Pin"],
         color="蓝"
 ) -> None:
     for i, o in zip(sourcePin.elementPins, targetPin.elementPins):
         crt_Wire(i, o, color)
 
 # 删除unionPin的导线
 @check_TypeUnionPin
 def del_Wires(
-        sourcePin: Union["_unionPin.unionPin", "_elementPin.element_Pin"],
-        targetPin: Union["_unionPin.unionPin", "_elementPin.element_Pin"],
+        sourcePin: Union["_unionPin.union_Pin", "_elementPin.element_Pin"],
+        targetPin: Union["_unionPin.union_Pin", "_elementPin.element_Pin"],
         color="蓝"
 ) -> None:
     for i, o in zip(sourcePin.elementPins, targetPin.elementPins):
         del_Wire(i, o, color)
```

### Comparing `physicsLab-1.2.2/physicsLab/electricity/wire.py` & `physicsLab-1.3.0/physicsLab/electricity/wire.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,22 @@
 #coding=utf-8
 import physicsLab.errors as errors
 import physicsLab._fileGlobals as _fileGlobals
 import physicsLab.electricity.elementPin as _elementPin
 
-# 老版本连接导线函数，不推荐使用
-def old_crt_wire(SourceLabel, SourcePin : int, TargetLabel, TargetPin : int, color = "蓝") -> None: # SourceLabel : Union[_element, tuple]
-    SourcePin, TargetPin = int(SourcePin), int(TargetPin)
-    if (isinstance(SourceLabel, tuple) and len(SourceLabel) == 3):
-        SourceLabel = _fileGlobals.elements_Position[SourceLabel]
-    elif (SourceLabel not in _fileGlobals.elements_Position.values()):
-        raise RuntimeError("SourceLabel must be a Positon or self")
-    if (isinstance(TargetLabel, tuple) and len(TargetLabel) == 3):
-        TargetLabel = _fileGlobals.elements_Position[TargetLabel]
-    elif (TargetLabel not in _fileGlobals.elements_Position.values()):
-        raise RuntimeError("TargetLabel must be a Positon or self")
-
-    if (color not in ["黑", "蓝", "红", "绿", "黄"]):
-        raise RuntimeError("illegal color")
-    _fileGlobals.Wires.append({"Source": SourceLabel._arguments["Identifier"], "SourcePin": SourcePin,
-                   "Target": TargetLabel._arguments["Identifier"], "TargetPin": TargetPin,
-                   "ColorName": f"{color}色导线"})
-
 # 检查函数参数是否是导线
 def _check_typeWire(func):
     def result(SourcePin: "_elementPin.element_Pin", TargetPin: "_elementPin.element_Pin", color: str = '蓝') -> None:
         if (
                 isinstance(SourcePin, _elementPin.element_Pin) and
                 isinstance(TargetPin, _elementPin.element_Pin)
         ):
             if (color not in ["黑", "蓝", "红", "绿", "黄"]):
-                raise errors.wireColorError("illegal color")
+                raise errors.wireColorError
+            _fileGlobals.check_ExperimentType(0)
 
             func(SourcePin, TargetPin, color)
 
     return result
 
 # 新版连接导线
 @_check_typeWire
@@ -57,16 +40,22 @@
             "Source": TargetPin.element_self._arguments["Identifier"], "SourcePin": TargetPin.pinLabel,
             "Target": SourcePin.element_self._arguments["Identifier"], "TargetPin": SourcePin.pinLabel,
             "ColorName": f"{color}色导线"
         }
         if a_wire in _fileGlobals.Wires:
             _fileGlobals.Wires.remove(a_wire)
         else:
-            raise errors.wireColorError
+            raise errors.wireNotFoundError
 
 # 删除所有导线
 def clear_Wires() -> None:
+    _fileGlobals.check_ExperimentType(0)
     _fileGlobals.Wires.clear()
 
 # 获取当前导线数
 def count_Wires() -> int:
-    return len(_fileGlobals.Wires)
+    _fileGlobals.check_ExperimentType(0)
+    return len(_fileGlobals.Wires)
+
+# 打印导线的json
+def print_Wires() -> None:
+    print(_fileGlobals.Wires)
```

### Comparing `physicsLab-1.2.2/physicsLab/experiment.py` & `physicsLab-1.3.0/physicsLab/experiment.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,79 @@
 #coding=utf-8
-import os as _os
-import sys as _sys
-import json as _json
+import os
+import json
+from typing import Union
 
 import physicsLab._tools as _tools
 import physicsLab.errors as errors
 import physicsLab._colorUtils as _colorUtils
 import physicsLab._fileGlobals as _fileGlobals
-from physicsLab.electricity.element import crt_Element
-import physicsLab.electricity.elementXYZ as _elementXYZ
-
-### define ###
-
-def print_Elements():
-    print(_fileGlobals.Elements)
-
-def print_wires():
-    print(_fileGlobals.Wires)
-
-def print_elements_Address():
-    print(_fileGlobals.elements_Position)
-
-### end define ###
 
 # 实验（存档）类，主要与'with'关键字搭配使用
 class experiment:
     def __init__(
             self,
             file: str,
             read: bool = False, # 是否读取存档原有状态
-            elementXYZ: bool = False
+            delete: bool = False, #是否删除实验
+            write: bool = True,
+            elementXYZ: bool = False,
+            type: Union[int, str] = None
     ):
         if not (
-            isinstance(file, str)
-            and isinstance(read, bool)
+            isinstance(file, str) or
+            isinstance(read, bool) or
+            isinstance(delete, bool) or
+            isinstance(elementXYZ, bool) or
+            isinstance(write, bool) or
+            (
+                isinstance(type, (int ,str)) or
+                type is None
+            )
         ):
             raise TypeError
 
         self.file = file
         self.read = read
+        self.delete = delete
+        self.write = write
         self.elementXYZ = elementXYZ
+        self.type = type
 
     # 上下文管理器，搭配with使用
     def __enter__(self):
         try:
             open_Experiment(self.file)
         except errors.openExperimentError: # 如果存档不存在
-            crt_Experiment(self.file)
+            crt_Experiment(self.file, self.type)
+        except TypeError:
+            raise TypeError
 
         if self.read:
             read_Experiment()
         if self.elementXYZ:
+            _fileGlobals.check_ExperimentType(0)
+            import physicsLab.electricity.elementXYZ as _elementXYZ
             _elementXYZ.set_elementXYZ(True)
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        write_Experiment()
+        if self.write:
+            write_Experiment()
+        if self.delete:
+            del_Experiment()
 
 # 输入sav文件名并读取（旧函数，不建议使用）
 def old_open_Experiment(file: str) -> None:
     file = file.strip()
     if (not file.endswith('.sav')):
         raise RuntimeError("The input parameters are incorrect")
 
-    _fileGlobals.savName = f"{_fileGlobals.FILE_HEAD}\\{file}"
+    _fileGlobals.savName = f"{_fileGlobals.FILE_HEAD}/{file}"
     with open(_fileGlobals.savName, encoding="UTF-8") as f:
-        InternalName = (_json.loads(f.read().replace('\n', '')))["InternalName"]
+        InternalName = (json.loads(f.read().replace('\n', '')))["InternalName"]
         _fileGlobals.sav["InternalName"] = InternalName
         try: # 当Summary为None时触发TypeError
             _fileGlobals.sav["Summary"]["Subject"] = InternalName
         except TypeError:
             pass
 
 # 将import了physicsLab的文件的第一行添加上 #coding=utf-8
@@ -89,125 +94,115 @@
             # 在cmd或IDLE上运行时会关闭打印彩字功能
             _colorUtils.printColor = False
         func(*args, **kwargs)
     return result
 
 # 打开一个指定的sav文件（支持输入本地实验的名字或sav文件名）
 @_utf8_coding
-def open_Experiment(file : str) -> None:
-    _fileGlobals.fileGlobals_init()
-    file = file.strip()
-    if file.endswith('.sav'):
-        old_open_Experiment(file)
+def open_Experiment(fileName : str) -> None:
+    fileName = fileName.strip()
+    if fileName.endswith('.sav'):
+        old_open_Experiment(fileName)
     else:
-        savs = [i for i in _os.walk(_fileGlobals.FILE_HEAD)][0]
-        savs = savs[savs.__len__() - 1]
-        savs = [aSav for aSav in savs if aSav.endswith('sav')]
+        savs = _tools.getAllSav()
         for aSav in savs:
-            with open(f"{_fileGlobals.FILE_HEAD}\\{aSav}", encoding='utf-8') as f:
+            with open(f"{_fileGlobals.FILE_HEAD}/{aSav}", encoding='utf-8') as f:
                 try:
-                    f = _json.loads(f.read().replace('\n', ''))
-                except _json.decoder.JSONDecodeError:
+                    f = json.loads(f.read().replace('\n', ''))
+                except json.decoder.JSONDecodeError: # 文件不是物实存档
                     pass
                 else:
-                    if (f.get("InternalName") == file):
+                    if f["InternalName"]== fileName:
+                        # 初始化package全局变量
+                        _fileGlobals.fileGlobals_init(f["Type"])
+
                         old_open_Experiment(aSav)
                         return
-        raise errors.openExperimentError(f'No such experiment "{file}"')
+        raise errors.openExperimentError(f'No such experiment "{fileName}"')
 
 # 创建存档
 @_utf8_coding
-def crt_Experiment(name : str) -> None:
-    _fileGlobals.fileGlobals_init()
-    # 检查是否存在重名的存档
-    savs = [i for i in _os.walk(_fileGlobals.FILE_HEAD)][0]
-    savs = savs[savs.__len__() - 1]
-    savs = [aSav for aSav in savs if aSav.endswith('sav')]
+def crt_Experiment(fileName : str, experimentType: str = None) -> None:
+    _fileGlobals.fileGlobals_init(experimentType)
+    savs = _tools.getAllSav()
     for aSav in savs:
-        with open(f"{_fileGlobals.FILE_HEAD}\\{aSav}", encoding='utf-8') as f:
+        with open(f"{_fileGlobals.FILE_HEAD}/{aSav}", 'r', encoding='utf-8') as f:
             try:
-                f = _json.loads(f.read().replace('\n', ''))
-            except:
-                pass
+                f = json.loads(f.read().replace('\n', ''))
+            except json.decoder.JSONDecodeError:
+                continue
             else:
-                if f['InternalName'] == name:
-                    raise RuntimeError('Duplicate name archives are forbidden')
+                if f['InternalName'] == fileName:
+                    raise errors.crtExperimentFailError
     # 创建存档
-    if not isinstance(name, str):
-        name = str(name)
+    if not isinstance(fileName, str):
+        fileName = str(fileName)
     _fileGlobals.savName = _tools.randString(34)
-    _fileGlobals.savName = f'{_fileGlobals.FILE_HEAD}\\{_fileGlobals.savName}.sav'
-    with open(_fileGlobals.savName, 'w', encoding='utf-8'):
-        pass
-    rename_Experiment(name)
+    _fileGlobals.savName = f'{_fileGlobals.FILE_HEAD}/{_fileGlobals.savName}.sav'
+    rename_Experiment(fileName)
 
 # 将编译完成的json写入sav
 def write_Experiment() -> None:
     def _format_StatusSave(stringJson: str) -> str:
         stringJson = stringJson.replace('{\\\"ModelID', '\n      {\\\"ModelID') # format element json
         stringJson = stringJson.replace('DiagramRotation\\\": 0}]', 'DiagramRotation\\\": 0}\n    ]') # format end element json
         stringJson = stringJson.replace('{\\\"Source', '\n      {\\\"Source')
         stringJson = stringJson.replace("色导线\\\"}]}", "色导线\\\"}\n    ]}")
         return stringJson
 
-    global _ifndef_open_Experiment
-    _ifndef_open_Experiment = False
-
     _fileGlobals.StatusSave["Elements"] = _fileGlobals.Elements
     _fileGlobals.StatusSave["Wires"] = _fileGlobals.Wires
-    _fileGlobals.sav["Experiment"]["StatusSave"] = _json.dumps(_fileGlobals.StatusSave, ensure_ascii=False)
+    _fileGlobals.sav["Experiment"]["StatusSave"] = \
+        json.dumps(_fileGlobals.StatusSave, ensure_ascii=False, separators=(',', ': '))
     with open(_fileGlobals.savName, "w", encoding="UTF-8") as f:
         f.write(
-                _format_StatusSave(_json.dumps(_fileGlobals.sav, indent=2, ensure_ascii=False))
+                _format_StatusSave(json.dumps(_fileGlobals.sav, indent=2, ensure_ascii=False, separators=(',', ': ')))
         )
-    # 存档回滚
-    f = ''
-    try:
-        f = open(f'{_fileGlobals.savName[:len(_fileGlobals.savName) - 4:]}_rollBack_sav.txt')
-    except FileNotFoundError:
-        f = open(f'{_fileGlobals.savName[:len(_fileGlobals.savName) - 4:]}_rollBack_sav.txt', 'w')
-    finally:
-        f.close()
-    experiments = []
-    with open(f'{_fileGlobals.savName[:len(_fileGlobals.savName) - 4:]}_rollBack_sav.txt', 'r', encoding='utf-8') as f:
-        f = f.read()
-        if f == '':
-            experiments.append(_fileGlobals.sav)
-        else:
-            experiments = _json.loads(f)
-            experiments.append(_fileGlobals.sav)
-        if experiments.__len__() > 10:
-            experiments.pop(0)
-    with open(f'{_fileGlobals.savName[:len(_fileGlobals.savName) - 4:]}_rollBack_sav.txt', 'w', encoding='utf-8') as f:
-        f.write(_json.dumps(experiments, indent=2, ensure_ascii=False))
     # 编译成功，打印信息
-    _colorUtils.printf(
-        f"Successfully compiled! {_fileGlobals.Elements.__len__()} elements, {_fileGlobals.Wires.__len__()} wires.",
-        _colorUtils.GREEN
-    )
+    if _fileGlobals.get_experimentType() == 0:
+        _colorUtils.printf(
+            f"Successfully compiled! {_fileGlobals.Elements.__len__()} elements, {_fileGlobals.Wires.__len__()} wires.",
+            _colorUtils.GREEN
+        )
+    else:
+        _colorUtils.printf(
+            f"Successfully compiled! {_fileGlobals.Elements.__len__()} elements.",
+            _colorUtils.GREEN
+        )
 
 # 读取sav文件已有的原件与导线
 def read_Experiment() -> None:
     with open(_fileGlobals.savName, encoding='UTF-8') as f:
-        readmem = _json.loads(f.read().replace('\n', ''))
+        readmem = json.loads(f.read().replace('\n', ''))
         # 元件
-        _local_Elements = _json.loads(readmem["Experiment"]["StatusSave"])["Elements"]
+        _local_Elements = json.loads(readmem["Experiment"]["StatusSave"])["Elements"]
         # 导线
-        _fileGlobals.Wires = _json.loads(readmem['Experiment']['StatusSave'])['Wires']
+        _fileGlobals.Wires = json.loads(readmem['Experiment']['StatusSave'])['Wires']
+        # 实验介绍
+        _fileGlobals.sav['Summary']["Description"] = readmem["Summary"]["Description"]
 
         for element in _local_Elements:
             # 坐标标准化（消除浮点误差）
             sign1 = element['Position'].find(',')
             sign2 = element['Position'].find(',', sign1 + 1)
             num1 = _tools.roundData(float(element['Position'][:sign1:]))
             num2 = _tools.roundData(float(element['Position'][sign1 + 1: sign2:]))
             num3 = _tools.roundData(float(element['Position'][sign2 + 1::]))
             element['Position'] = f"{num1},{num2},{num3}"  # x, z, y
             # 实例化对象
-            obj = crt_Element(element["ModelID"], num1, num3, num2, elementXYZ=False)
+            obj = None
+            from physicsLab.element import crt_Element
+
+            if _fileGlobals.get_experimentType() == 0:
+                obj = crt_Element(element["ModelID"], num1, num3, num2, elementXYZ=False)
+            elif _fileGlobals.get_experimentType() == 3 or _fileGlobals.get_experimentType() == 4:
+                obj = crt_Element(element["ModelID"], num1, num3, num2)
+            else:
+                raise errors.openExperimentError
+
             sign1 = element['Rotation'].find(',')
             sign2 = element['Rotation'].find(',', sign1 + 1)
             x = float(element['Rotation'][:sign1:])
             z = float(element['Rotation'][sign1 + 1: sign2:])
             y = float(element['Rotation'][sign2 + 1::])
             obj.set_Rotation(x, y, z)
             obj._arguments['Identifier'] = element['Identifier']
@@ -218,69 +213,56 @@
             elif obj.type() == '8bit Input':
                 obj._arguments['Statistics'] = element['Statistics']
                 obj._arguments['Properties']['十进制'] = element['Properties']['十进制']
 
 # 重命名sav
 def rename_Experiment(name: str) -> None:
     # 检查是否重名
-    savs = [i for i in _os.walk(_fileGlobals.FILE_HEAD)][0]
+    savs = [i for i in os.walk(_fileGlobals.FILE_HEAD)][0]
     savs = savs[savs.__len__() - 1]
     savs = [aSav for aSav in savs if aSav.endswith('sav')]
     for aSav in savs:
-        with open(f"{_fileGlobals.FILE_HEAD}\\{aSav}", encoding='utf-8') as f:
+        with open(f"{_fileGlobals.FILE_HEAD}/{aSav}", encoding='utf-8') as f:
             try:
-                f = _json.loads(f.read().replace('\n', ''))
+                f = json.loads(f.read().replace('\n', ''))
             except:
                 pass
             else:
                 if f['InternalName'] == name:
                     raise RuntimeError('Duplicate name archives are forbidden')
     # 重命名存档
     name = str(name)
     _fileGlobals.sav["Summary"]["Subject"] = name
     _fileGlobals.sav["InternalName"] = name
 
 # 打开一个存档的窗口
 def show_Experiment() -> None:
-    _os.popen(f'notepad {_fileGlobals.savName}')
+    os.popen(f'notepad {_fileGlobals.savName}')
 os_Experiment = show_Experiment
 
 # 删除存档
 def del_Experiment() -> None:
-    _os.remove(_fileGlobals.savName)
-    _os.remove(f"{_fileGlobals.savName.replace('.sav', '_rollBack_sav.txt')}")
-    try:
-        _os.remove(_fileGlobals.savName.replace('.sav', '.jpg'))
-    except:
-        _sys.exit()
-
-# 存档回滚
-def rollBack_Experiment(back: int = 1):
-    if not isinstance(back, int) and (back < 1 or back >= 10):
-        raise RuntimeError('back must be an integer between 1 and 10')
-    f = ''
-    try:
-        f = open(f'{_fileGlobals.savName[:len(_fileGlobals.savName) - 4:]}_rollBack_sav.txt')
+    os.remove(_fileGlobals.savName)
+    try: # 用存档生成的实验无图片，因此可能删除失败
+        os.remove(_fileGlobals.savName.replace('.sav', '.jpg'))
     except FileNotFoundError:
-        f = open(f'{_fileGlobals.savName[:len(_fileGlobals.savName) - 4:]}_rollBack_sav.txt', 'w')
-    finally:
-        f.close()
-    with open(f'{_fileGlobals.savName[:len(_fileGlobals.savName) - 4:]}_rollBack_sav.txt', encoding='utf-8') as f:
-        reader = f.read().replace('\n', '')
-        if reader == '':
-            raise RuntimeError('There is no archive to roll back')
-        f = _json.loads(reader)
-        _fileGlobals.sav = _json.loads(f[len(f) - 1 - back]['Experiment']['StatusSave'])
-        _fileGlobals.Elements = _fileGlobals.sav['Elements']
-        _fileGlobals.Wires = _fileGlobals.sav['Wires']
-
-# 发布实验时输入实验介绍
-def introduce_Experiment(introduction: str) -> None:
-    if not isinstance(introduction, str) or introduction is None:
-        raise TypeError
-    _fileGlobals.sav['Summary']['Description'] = introduction.split('\n')
+        pass
+    _colorUtils.printf("Successfully delete experiment!", _colorUtils.BLUE)
+
+# 发布实验
+def yield_Experiment(title: str = None, introduction: str = None) -> None:
+    # 发布实验时输入实验介绍
+    def introduce_Experiment(introduction: str) -> None:
+        if introduction is not None:
+            _fileGlobals.sav['Summary']['Description'] = introduction.split('\n')
+
+    # 发布实验时输入实验标题
+    def title_Experiment(title: str) -> None:
+        if title is not None:
+            _fileGlobals.sav['Summary']['Subject'] = title
 
-# 发布实验时输入实验标题
-def title_Experiment(title: str) -> None:
-    if isinstance(title, str) or title is None:
+    if (not isinstance(title, str) and title is not None) or \
+            (not isinstance(introduction, str) and introduction is not None):
         raise TypeError
-    _fileGlobals.sav['Summary']['Subject'] = title
+
+    introduce_Experiment(introduction)
+    title_Experiment(title)
```

### Comparing `physicsLab-1.2.2/physicsLab.egg-info/PKG-INFO` & `physicsLab-1.3.0/physicsLab.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: physicsLab
-Version: 1.2.2
+Version: 1.3.0
 Summary: Doing experiments in the physics lab AR by python
 Home-page: https://gitee.com/script2000/physicsLab
 Author: Goodenough
 Author-email: 2381642961@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE
 
 ﻿# physicsLab 物实程序化
 
 ![输入图片说明](cover.png)
 
 ## 介绍
 在物理实验室做实验的时候，我们可能会苦恼于元件不够整齐且无法浮空等等问题。这些都可以通过改存档来轻易实现！然而，手动改存档局限性很大，于是我封装了一些常用功能，让你用Python也能够轻易地做实验，**你甚至不需用知道存档在电脑的哪里**！
@@ -52,15 +52,26 @@
  # crt_wire输入格式：  
  #    crt_wire(SourcePin, TargetPin, color = "蓝")  
 crt_Wire(o.i_up, o.i_low)  
  # 将程序中生成的原件，导线等等写入存档  
 write_Experiment()  
  # 然后用物实打开存档见证奇迹  
 ```
-更详细的内容请查看[functions.md](functions.md)  
+如今有了更优雅的方式：
+```python
+from physicsLab import *
+
+with experiment('测逝', read=True, elementXYZ=True):
+    Logic_Input(0, 0, 1)
+    o = Or_Gate()
+    o.i_up - o.i_low # 连接导线
+```
+上面两段代码产生的结果是一样的  
+  
+更详细的内容请在[wiki](https://gitee.com/script2000/physicsLab/wikis/functions)中查看  
 请注意：Python采用GBK编码，而物实用的是utf-8，尽管尽量确保编码格式正确，但中文仍有可能出现问题，因此建议多用英文。  
 
 ## 优点
 1. 通过read_Experiment()，你无须把所有工作交给代码。因为用代码写并不总是意味着方便（比如连接导线）。  
 你现在可以手动连接部分导线或者添加原件，并通过保存的形式，让程序在下次也可以轻松读取。  
 这也意味着你不用一口气把控制整个电路的脚本写出来，而是每次写一部分，并把更适合代码的工作交给代码完成。  
 也就是说，写这个脚本的感觉更像在控制台上操作，非常灵活。
@@ -80,12 +91,11 @@
 ## 其他
 1. 更多内容请在[other physicsLab](https://gitee.com/script2000/temporary-warehouse/tree/master/other%20physicsLab)查看
 2. github: https://github.com/GoodenoughPhysicsLab/physicsLab
 3. gitee: https://gitee.com/script2000/physicsLab
 
 ## 参与贡献
 1.  Fork 本仓库
-2.  新建 Feat_xxx 分支
+2.  新建分支
 3.  提交代码
 4.  新建 Pull Request
-5.  补充readme
```

### Comparing `physicsLab-1.2.2/physicsLab.egg-info/SOURCES.txt` & `physicsLab-1.3.0/physicsLab.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-LICENSE.txt
+LICENSE
 README.md
-pyproject.toml
 setup.py
 physicsLab/__init__.py
 physicsLab/_colorUtils.py
 physicsLab/_fileGlobals.py
 physicsLab/_tools.py
+physicsLab/element.py
 physicsLab/errors.py
 physicsLab/experiment.py
 physicsLab.egg-info/PKG-INFO
 physicsLab.egg-info/SOURCES.txt
 physicsLab.egg-info/dependency_links.txt
 physicsLab.egg-info/top_level.txt
 physicsLab/astrophysics/__init__.py
+physicsLab/astrophysics/elementsClass.py
 physicsLab/electricity/__init__.py
-physicsLab/electricity/element.py
 physicsLab/electricity/elementPin.py
 physicsLab/electricity/elementXYZ.py
 physicsLab/electricity/wire.py
 physicsLab/electricity/elementsClass/__init__.py
 physicsLab/electricity/elementsClass/_elementClassHead.py
 physicsLab/electricity/elementsClass/artificialCircuit.py
 physicsLab/electricity/elementsClass/basicCircuit.py
@@ -26,8 +26,9 @@
 physicsLab/electricity/elementsClass/otherCircuit.py
 physicsLab/electricity/unionElements/__init__.py
 physicsLab/electricity/unionElements/_unionClassHead.py
 physicsLab/electricity/unionElements/unionLogic.py
 physicsLab/electricity/unionElements/unionMusic.py
 physicsLab/electricity/unionElements/unionPin.py
 physicsLab/electricity/unionElements/wires.py
-physicsLab/electromagnetism/__init__.py
+physicsLab/electromagnetism/__init__.py
+physicsLab/electromagnetism/elementsClass.py
```

### Comparing `physicsLab-1.2.2/setup.py` & `physicsLab-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("D:/program_physicsLab/README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="physicsLab",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="1.2.2",  # 包版本号，便于维护版本
+    version="1.3.0",  # 包版本号，便于维护版本
     author="Goodenough",  # 作者，可以写自己的姓名
     author_email="2381642961@qq.com",  # 作者联系方式，可写自己的邮箱地址
     description="Doing experiments in the physics lab AR by python",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://gitee.com/script2000/physicsLab",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: Chinese (Simplified)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',  # 对python的最低版本要求
-)
+)
```

