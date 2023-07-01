# Comparing `tmp/tkintertools-2.6.6.tar.gz` & `tmp/tkintertools-2.6.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkintertools-2.6.6.tar", last modified: Sat Jul  1 13:18:19 2023, max compression
+gzip compressed data, was "tkintertools-2.6.6.dev0.tar", last modified: Thu Jun 29 09:43:34 2023, max compression
```

## Comparing `tkintertools-2.6.6.tar` & `tkintertools-2.6.6.dev0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 13:18:19.345691 tkintertools-2.6.6/
--rw-rw-rw-   0        0        0     9267 2023-06-20 19:03:57.000000 tkintertools-2.6.6/LICENSE.txt
--rw-rw-rw-   0        0        0     9971 2023-07-01 13:18:19.344695 tkintertools-2.6.6/PKG-INFO
--rw-rw-rw-   0        0        0     9342 2023-07-01 12:59:48.000000 tkintertools-2.6.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-01 13:18:19.345691 tkintertools-2.6.6/setup.cfg
--rw-rw-rw-   0        0        0     1536 2023-07-01 13:15:08.000000 tkintertools-2.6.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 13:18:19.331431 tkintertools-2.6.6/tkintertools/
--rw-rw-rw-   0        0        0     2859 2023-07-01 13:08:48.000000 tkintertools-2.6.6/tkintertools/__init__.py
--rw-rw-rw-   0        0        0    62351 2023-06-28 20:32:13.000000 tkintertools-2.6.6/tkintertools/__main__.py
--rw-rw-rw-   0        0        0     1999 2023-06-16 16:48:27.000000 tkintertools-2.6.6/tkintertools/constants.py
--rw-rw-rw-   0        0        0    23200 2023-07-01 12:24:50.000000 tkintertools-2.6.6/tkintertools/tools_3d.py
-drwxrwxrwx   0        0        0        0 2023-07-01 13:18:19.341692 tkintertools-2.6.6/tkintertools.egg-info/
--rw-rw-rw-   0        0        0     9971 2023-07-01 13:18:19.000000 tkintertools-2.6.6/tkintertools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-07-01 13:18:19.000000 tkintertools-2.6.6/tkintertools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 13:18:19.000000 tkintertools-2.6.6/tkintertools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-01 13:18:19.000000 tkintertools-2.6.6/tkintertools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 09:43:34.023952 tkintertools-2.6.6.dev0/
+-rw-rw-rw-   0        0        0     9267 2023-06-20 19:03:57.000000 tkintertools-2.6.6.dev0/LICENSE.txt
+-rw-rw-rw-   0        0        0     9062 2023-06-29 09:43:34.022947 tkintertools-2.6.6.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0     8428 2023-06-29 09:04:12.000000 tkintertools-2.6.6.dev0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-29 09:43:34.023952 tkintertools-2.6.6.dev0/setup.cfg
+-rw-rw-rw-   0        0        0     1370 2023-06-29 06:36:36.000000 tkintertools-2.6.6.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 09:43:34.010671 tkintertools-2.6.6.dev0/tkintertools/
+-rw-rw-rw-   0        0        0     2863 2023-06-29 07:57:18.000000 tkintertools-2.6.6.dev0/tkintertools/__init__.py
+-rw-rw-rw-   0        0        0    62351 2023-06-28 20:32:13.000000 tkintertools-2.6.6.dev0/tkintertools/__main__.py
+-rw-rw-rw-   0        0        0     1999 2023-06-16 16:48:27.000000 tkintertools-2.6.6.dev0/tkintertools/constants.py
+-rw-rw-rw-   0        0        0    21734 2023-06-29 07:51:40.000000 tkintertools-2.6.6.dev0/tkintertools/tools_3d.py
+drwxrwxrwx   0        0        0        0 2023-06-29 09:43:34.020749 tkintertools-2.6.6.dev0/tkintertools.egg-info/
+-rw-rw-rw-   0        0        0     9062 2023-06-29 09:43:33.000000 tkintertools-2.6.6.dev0/tkintertools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-06-29 09:43:33.000000 tkintertools-2.6.6.dev0/tkintertools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 09:43:33.000000 tkintertools-2.6.6.dev0/tkintertools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-29 09:43:33.000000 tkintertools-2.6.6.dev0/tkintertools.egg-info/top_level.txt
```

### Comparing `tkintertools-2.6.6/LICENSE.txt` & `tkintertools-2.6.6.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tkintertools-2.6.6/PKG-INFO` & `tkintertools-2.6.6.dev0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkintertools
-Version: 2.6.6
+Version: 2.6.6.dev0
 Summary: An auxiliary module of the tkinter module.
 Home-page: https://github.com/Xiaokang2022/tkintertools
 Author: Xiaokang2022
 Author-email: 2951256653@qq.com
 Maintainer: Xiaokang2022
 Maintainer-email: 2951256653@qq.com
 License: MulanPSL-2.0
@@ -23,57 +23,57 @@
 <img src="tkt.png" style="height: 128px" alt="Logo" />
 
 `tkintertools` 模块是 `tkinter` 模块的一个辅助模块\
 The `tkintertools` module is an auxiliary module of the `tkinter` module
 
 [![Version](https://img.shields.io/pypi/v/tkintertools?label=Version)](.)
 [![License](https://img.shields.io/pypi/l/tkintertools?label=License)](LICENSE.txt)
-[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/07/01-orange)](CHANGELOG.md)
+[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/06/29-orange)](CHANGELOG.md)
 [![ToDo](https://img.shields.io/badge/ToDo-16-yellow)](TODO.md)
 [![Size](https://img.shields.io/github/languages/code-size/Xiaokang2022/tkintertools?label=Size)](tkintertools)
-[![Wiki](https://img.shields.io/badge/Wiki-14-purple)](https://github.com/Xiaokang2022/tkintertools/wiki)\
+[![Wiki](https://img.shields.io/badge/Wiki-15-purple)](https://github.com/Xiaokang2022/tkintertools/wiki)\
 [![Downloads](https://img.shields.io/pypi/dm/tkintertools?label=Downloads&logo=pypi)](https://pypistats.org/packages/tkintertools)
 [![Owner](https://img.shields.io/badge/Owner-Xiaokang2022-white?logo=about.me)](https://github.com/Xiaokang2022)
 [![Blog](https://img.shields.io/badge/Blog-小康2022@CSDN-red)](https://xiaokang2022.blog.csdn.net)
 [![Email](https://img.shields.io/badge/Email-2951256653@qq.com-cyan)](mailto:2951256653@qq.com)
 
 [![Insights](https://repobeats.axiom.co/api/embed/ab8fae686a5a96f91fa71c40c53c189310924f5e.svg)](https://github.com/Xiaokang2022/tkintertools/pulse)
 
 </div>
 
 Install/模块安装👇
 -----------------
 
 ### Stable Version/稳定版本
 
-* Version/最新版本 : `2.6.6`
-* Release/发布日期 : 2023/07/01 (UTC+08)
+* Version/最新版本 : `2.6.5`
+* Release/发布日期 : 2023/06/17 (UTC+08)
 
 这个是目前的最新稳定版，相对于开发版本而言比较稳定，bug 大体上是没有那么多的，推荐使用这个。  
 稳定版和开发版相比，它在发布之前有个测试的步骤，经过测试之后（各项功能正常运行，多平台兼容）才会发布。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.6
+pip install tkintertools==2.6.5
 ```
 
 ### Development Version/开发版本
 
-* Version/最新版本 : `2.6.6.dev0`
+* Version/最新版本 : `2.6.6.dev`
 * Release/发布日期 : 2023/06/29 (UTC+08)
 
 这个是我正在开发的版本，可能有新功能，bug 可能会比较多，但也可能会比原来的版本更加稳定。  
 开发版没有经过多操作系统的测试，仅能保证在 Windows 系统下运行所有功能，在其他的操作系统上，可能有部分功能无法正常运行。  
 大家可以在 Issues 中提出一些建议，我可能会适当采纳一些并在开发版本中更改或实现。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.6.dev0
+pip install tkintertools==2.6.6.dev
 ```
 
 > **Warning**  
 > 开发版仅作示例，各函数或类的 API 并非最终确定结果，直接使用开发版可能导致后续无法与稳定版兼容！  
 > 若不指定具体的版本号，则会下载最新的稳定版本，也就是说，开发版本只能通过指定的版本号获取！
 
 ### Requirements/环境需求
@@ -92,97 +92,66 @@
 ![Python3.10.*](https://img.shields.io/badge/Python-3.10.*-blue?logo=python)
 ![Python3.11.*](https://img.shields.io/badge/Python-3.11.*-blue?logo=python)
 ![Python3.12.*](https://img.shields.io/badge/Python-3.12.*-blue?logo=python)
 
 News/最新功能👇
 --------------
 
-**最新版本: tkintertools-v2.6.6**
+**最新版本: tkintertools-2.6.6.dev 开发版**
 
 > **Note**  
-> 现将开发版（`tkintertools-dev`）合并到稳定版（`tkintertools`）中，版本号格式变为 `*.*.*.dev*`，大家在通过 pip 工具进行下载时请注意！近段时间内将删除 PyPi 上的 tkintertools-dev！
+> 现将开发版（`tkintertools-dev`）合并到稳定版（`tkintertools`）中，版本号格式变为 `*.*.*.dev`，大家在通过 pip 工具进行下载时请注意！近段时间内将删除 PyPi 上的 tkintertools-dev！
 
 下面是本次版本更新内容条目：
 
-- [X] 3D 子模块的类 `_Point`、`_Line`、`_Side` 和 `Geometry` 都新增一个方法 `center` 返回该 3D 对象的几何中心；
 - [X] 新增抽象类 `_3D_Object` 来作为类 `_Point`、`_Line` 和 `_Side` 的元基类；
 - [X] 优化了 3D 子模块中的参数传递，使用者不需要时刻保证 `list` 的传递性，且原来只能使用 `list` 类型的参数现在为 `Iterable` 类型；
 - [X] 3D 子模块中 3D 对象居中方式改变，相比原来性能提升了不少，代码量也减少了；
 - [X] 改正了部分错误的类型提示，完善了部分缺少的方法注释；
 - [X] 3D 子模块中原来用函数 `hypot` 计算两点间距离，现在直接用函数 `dist` 计算两点间欧几里得距离，提高性能；
 - [X] 3D 子模块中优化了类 `Point` 的控件位置显示，让其始终保持在最前；
-- [X] 3D 子模块中相机距离的计算公式优化，提高了一点性能；
 - [X] 3D 子模块的类 `Point` 及其父类 `_Point` 的参数 `point1` 和 `point2` 分别被重命名为 `point_start` 和 `point_end`；
 - [X] 3D 子模块的类 `Space` 的参数 `origin_color` 被更改为四个新的参数，分别是 `origin_size`、`origin_width`、`origin_fill` 和 `origin_outline`；
 - [X] 3D 子模块的类 `Canvas_3D` 和 `Space` 移除参数 `dx` 和 `dy`，画布默认视野保持居中，也就是说，现在它们的中心位置才是原来的左上角顶点；
 
 下面是一个主要新功能的示例程序，运行下面的示例程序时，其拥有以下功能：
 
 * 按住鼠标左键拖动可以旋转这多个几何体；
 * 按住鼠标右键拖动可以移动这些几何体在空间中的位置；
 * 滚动鼠标中键可以放大和缩小画面；
-* 这多个几何体会自动地旋转以及上下浮动；
 
 下面是示例程序的效果图（运行环境为 Windows11-Python3.11.4）：
 
-![news](news.gif)
+![news](news.png)
 
 <details><summary><b>点击查看源代码</b></summary>
 
 ```python
 import math  # 数学支持
 
 import tkintertools as tkt  # 引入基础模块
 from tkintertools import tools_3d as t3d  # 引入 3d 子模块
 
 root = tkt.Tk('3D', 1280, 720)  # 创建窗口
 space = t3d.Space(root, 1280, 720, 0, 0)  # 创建空间
+last_point = [0, 100*math.cos(-math.pi/3), 100*math.sin(-math.pi/3)]
+color_lst = ['red', 'orange', 'yellow', 'green', 'blue', 'purple']
+color_lst += color_lst
+
+for i in range(6):
+    rad = i*math.pi/3
+    next_point = [0, 100*math.cos(rad), 100*math.sin(rad)]
+    point_h2 = [0, 150*math.cos(rad), 150*math.sin(rad)]
+    t3d.Line(space, last_point, next_point, width=3, fill=color_lst[i])
+    t3d.Line(space, next_point, point_h2, width=3, fill=color_lst[i+1])
+    t3d.Point(space, last_point, size=20, fill=color_lst[i+2])
+    t3d.Point(space, point_h2, size=10, fill=color_lst[i+3])
+    last_point = next_point
 
-for a in -100, 0, 100:
-    for b in -100, 0, 100:
-        for c in -100, 0, 100:
-            t3d.Cuboid(space, a-50, b-50, c-50, 100, 100, 100,  # 创建正方体
-                       color_up='white', color_down='yellow', color_left='red',
-                       color_right='orange', color_front='blue', color_back='green')
-
-
-def spin():
-    """ 自动旋转 """
-    for geo in space.geos():
-        geo.rotate(dz=0.01)
-
-
-def floating(value):
-    """ 上下浮动 """
-    for geo in space.geos():
-        geo.translate(dz=math.sin(value))
-
-
-def animation(value=0):
-    """ 形成动画 """
-    spin()
-    floating(value)
-    space.space_sort()  # 给它们的空间位置排序以正确显示
-    for geo in space.geos():
-        geo.update()
-    space.after(10, animation, value+math.pi/60)
-
-
-def scale(event):
-    """ 缩放事件 """
-    k = 1.05 if event.keysym == 'equal' else 0.95 if event.keysym == 'minus' else 1  # 缩放比率
-    for geo in space.geos():  # 遍历所有的几何体（不包括基本 3D 对象）
-        geo.scale(k, k, k)  # 缩放
-        geo.update()  # 更新改对象的实际画面
-    space.space_sort()  # 空间前后位置排序
-
-
-animation()
-root.bind('<Key-equal>', scale)  # 绑定等号按键
-root.bind('<Key-minus>', scale)  # 绑定减号按键
+space.space_sort()  # 给它们的空间位置排序以正确显示
 root.mainloop()  # 消息事件循环
 ```
 
 </details>
 
 More/更多👇
 -----------
```

### Comparing `tkintertools-2.6.6/README.md` & `tkintertools-2.6.6.dev0/tkintertools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,79 @@
+Metadata-Version: 2.1
+Name: tkintertools
+Version: 2.6.6.dev0
+Summary: An auxiliary module of the tkinter module.
+Home-page: https://github.com/Xiaokang2022/tkintertools
+Author: Xiaokang2022
+Author-email: 2951256653@qq.com
+Maintainer: Xiaokang2022
+Maintainer-email: 2951256653@qq.com
+License: MulanPSL-2.0
+Keywords: tkinter,tkintertools,GUI
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 <div align="center">
 
 # 🚀tkintertools🚀
 
 <img src="tkt.png" style="height: 128px" alt="Logo" />
 
 `tkintertools` 模块是 `tkinter` 模块的一个辅助模块\
 The `tkintertools` module is an auxiliary module of the `tkinter` module
 
 [![Version](https://img.shields.io/pypi/v/tkintertools?label=Version)](.)
 [![License](https://img.shields.io/pypi/l/tkintertools?label=License)](LICENSE.txt)
-[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/07/01-orange)](CHANGELOG.md)
+[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/06/29-orange)](CHANGELOG.md)
 [![ToDo](https://img.shields.io/badge/ToDo-16-yellow)](TODO.md)
 [![Size](https://img.shields.io/github/languages/code-size/Xiaokang2022/tkintertools?label=Size)](tkintertools)
-[![Wiki](https://img.shields.io/badge/Wiki-14-purple)](https://github.com/Xiaokang2022/tkintertools/wiki)\
+[![Wiki](https://img.shields.io/badge/Wiki-15-purple)](https://github.com/Xiaokang2022/tkintertools/wiki)\
 [![Downloads](https://img.shields.io/pypi/dm/tkintertools?label=Downloads&logo=pypi)](https://pypistats.org/packages/tkintertools)
 [![Owner](https://img.shields.io/badge/Owner-Xiaokang2022-white?logo=about.me)](https://github.com/Xiaokang2022)
 [![Blog](https://img.shields.io/badge/Blog-小康2022@CSDN-red)](https://xiaokang2022.blog.csdn.net)
 [![Email](https://img.shields.io/badge/Email-2951256653@qq.com-cyan)](mailto:2951256653@qq.com)
 
 [![Insights](https://repobeats.axiom.co/api/embed/ab8fae686a5a96f91fa71c40c53c189310924f5e.svg)](https://github.com/Xiaokang2022/tkintertools/pulse)
 
 </div>
 
 Install/模块安装👇
 -----------------
 
 ### Stable Version/稳定版本
 
-* Version/最新版本 : `2.6.6`
-* Release/发布日期 : 2023/07/01 (UTC+08)
+* Version/最新版本 : `2.6.5`
+* Release/发布日期 : 2023/06/17 (UTC+08)
 
 这个是目前的最新稳定版，相对于开发版本而言比较稳定，bug 大体上是没有那么多的，推荐使用这个。  
 稳定版和开发版相比，它在发布之前有个测试的步骤，经过测试之后（各项功能正常运行，多平台兼容）才会发布。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.6
+pip install tkintertools==2.6.5
 ```
 
 ### Development Version/开发版本
 
-* Version/最新版本 : `2.6.6.dev0`
+* Version/最新版本 : `2.6.6.dev`
 * Release/发布日期 : 2023/06/29 (UTC+08)
 
 这个是我正在开发的版本，可能有新功能，bug 可能会比较多，但也可能会比原来的版本更加稳定。  
 开发版没有经过多操作系统的测试，仅能保证在 Windows 系统下运行所有功能，在其他的操作系统上，可能有部分功能无法正常运行。  
 大家可以在 Issues 中提出一些建议，我可能会适当采纳一些并在开发版本中更改或实现。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.6.dev0
+pip install tkintertools==2.6.6.dev
 ```
 
 > **Warning**  
 > 开发版仅作示例，各函数或类的 API 并非最终确定结果，直接使用开发版可能导致后续无法与稳定版兼容！  
 > 若不指定具体的版本号，则会下载最新的稳定版本，也就是说，开发版本只能通过指定的版本号获取！
 
 ### Requirements/环境需求
@@ -74,97 +92,66 @@
 ![Python3.10.*](https://img.shields.io/badge/Python-3.10.*-blue?logo=python)
 ![Python3.11.*](https://img.shields.io/badge/Python-3.11.*-blue?logo=python)
 ![Python3.12.*](https://img.shields.io/badge/Python-3.12.*-blue?logo=python)
 
 News/最新功能👇
 --------------
 
-**最新版本: tkintertools-v2.6.6**
+**最新版本: tkintertools-2.6.6.dev 开发版**
 
 > **Note**  
-> 现将开发版（`tkintertools-dev`）合并到稳定版（`tkintertools`）中，版本号格式变为 `*.*.*.dev*`，大家在通过 pip 工具进行下载时请注意！近段时间内将删除 PyPi 上的 tkintertools-dev！
+> 现将开发版（`tkintertools-dev`）合并到稳定版（`tkintertools`）中，版本号格式变为 `*.*.*.dev`，大家在通过 pip 工具进行下载时请注意！近段时间内将删除 PyPi 上的 tkintertools-dev！
 
 下面是本次版本更新内容条目：
 
-- [X] 3D 子模块的类 `_Point`、`_Line`、`_Side` 和 `Geometry` 都新增一个方法 `center` 返回该 3D 对象的几何中心；
 - [X] 新增抽象类 `_3D_Object` 来作为类 `_Point`、`_Line` 和 `_Side` 的元基类；
 - [X] 优化了 3D 子模块中的参数传递，使用者不需要时刻保证 `list` 的传递性，且原来只能使用 `list` 类型的参数现在为 `Iterable` 类型；
 - [X] 3D 子模块中 3D 对象居中方式改变，相比原来性能提升了不少，代码量也减少了；
 - [X] 改正了部分错误的类型提示，完善了部分缺少的方法注释；
 - [X] 3D 子模块中原来用函数 `hypot` 计算两点间距离，现在直接用函数 `dist` 计算两点间欧几里得距离，提高性能；
 - [X] 3D 子模块中优化了类 `Point` 的控件位置显示，让其始终保持在最前；
-- [X] 3D 子模块中相机距离的计算公式优化，提高了一点性能；
 - [X] 3D 子模块的类 `Point` 及其父类 `_Point` 的参数 `point1` 和 `point2` 分别被重命名为 `point_start` 和 `point_end`；
 - [X] 3D 子模块的类 `Space` 的参数 `origin_color` 被更改为四个新的参数，分别是 `origin_size`、`origin_width`、`origin_fill` 和 `origin_outline`；
 - [X] 3D 子模块的类 `Canvas_3D` 和 `Space` 移除参数 `dx` 和 `dy`，画布默认视野保持居中，也就是说，现在它们的中心位置才是原来的左上角顶点；
 
 下面是一个主要新功能的示例程序，运行下面的示例程序时，其拥有以下功能：
 
 * 按住鼠标左键拖动可以旋转这多个几何体；
 * 按住鼠标右键拖动可以移动这些几何体在空间中的位置；
 * 滚动鼠标中键可以放大和缩小画面；
-* 这多个几何体会自动地旋转以及上下浮动；
 
 下面是示例程序的效果图（运行环境为 Windows11-Python3.11.4）：
 
-![news](news.gif)
+![news](news.png)
 
 <details><summary><b>点击查看源代码</b></summary>
 
 ```python
 import math  # 数学支持
 
 import tkintertools as tkt  # 引入基础模块
 from tkintertools import tools_3d as t3d  # 引入 3d 子模块
 
 root = tkt.Tk('3D', 1280, 720)  # 创建窗口
 space = t3d.Space(root, 1280, 720, 0, 0)  # 创建空间
+last_point = [0, 100*math.cos(-math.pi/3), 100*math.sin(-math.pi/3)]
+color_lst = ['red', 'orange', 'yellow', 'green', 'blue', 'purple']
+color_lst += color_lst
+
+for i in range(6):
+    rad = i*math.pi/3
+    next_point = [0, 100*math.cos(rad), 100*math.sin(rad)]
+    point_h2 = [0, 150*math.cos(rad), 150*math.sin(rad)]
+    t3d.Line(space, last_point, next_point, width=3, fill=color_lst[i])
+    t3d.Line(space, next_point, point_h2, width=3, fill=color_lst[i+1])
+    t3d.Point(space, last_point, size=20, fill=color_lst[i+2])
+    t3d.Point(space, point_h2, size=10, fill=color_lst[i+3])
+    last_point = next_point
 
-for a in -100, 0, 100:
-    for b in -100, 0, 100:
-        for c in -100, 0, 100:
-            t3d.Cuboid(space, a-50, b-50, c-50, 100, 100, 100,  # 创建正方体
-                       color_up='white', color_down='yellow', color_left='red',
-                       color_right='orange', color_front='blue', color_back='green')
-
-
-def spin():
-    """ 自动旋转 """
-    for geo in space.geos():
-        geo.rotate(dz=0.01)
-
-
-def floating(value):
-    """ 上下浮动 """
-    for geo in space.geos():
-        geo.translate(dz=math.sin(value))
-
-
-def animation(value=0):
-    """ 形成动画 """
-    spin()
-    floating(value)
-    space.space_sort()  # 给它们的空间位置排序以正确显示
-    for geo in space.geos():
-        geo.update()
-    space.after(10, animation, value+math.pi/60)
-
-
-def scale(event):
-    """ 缩放事件 """
-    k = 1.05 if event.keysym == 'equal' else 0.95 if event.keysym == 'minus' else 1  # 缩放比率
-    for geo in space.geos():  # 遍历所有的几何体（不包括基本 3D 对象）
-        geo.scale(k, k, k)  # 缩放
-        geo.update()  # 更新改对象的实际画面
-    space.space_sort()  # 空间前后位置排序
-
-
-animation()
-root.bind('<Key-equal>', scale)  # 绑定等号按键
-root.bind('<Key-minus>', scale)  # 绑定减号按键
+space.space_sort()  # 给它们的空间位置排序以正确显示
 root.mainloop()  # 消息事件循环
 ```
 
 </details>
 
 More/更多👇
 -----------
```

### Comparing `tkintertools-2.6.6/setup.py` & `tkintertools-2.6.6.dev0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,14 @@
-"""
-上传 PyPi
----------
-1. __init__.py 的版本号
-2. setup.py 的版本号
-3. CHANGELOG.md 日志文件
-4. README.md 自述文件
-5. Wiki 仓库文件
-6. Python3.8.* 兼容性测试
-7. Ubuntu22.04 跨平台测试
-8. 确认上传文件
-"""
+""" 上传 PyPi """
 
 import setuptools
 
 setuptools.setup(
     name='tkintertools',
-    version='2.6.6',
+    version='2.6.6.dev',
     description='An auxiliary module of the tkinter module.',
     long_description=open('README.md', encoding='utf-8').read(),
     author='Xiaokang2022',
     author_email='2951256653@qq.com',
     maintainer='Xiaokang2022',
     maintainer_email='2951256653@qq.com',
     url='https://github.com/Xiaokang2022/tkintertools',
@@ -44,7 +33,9 @@
 # pip install socksio [数据分析]
 
 # pypistats overall tkintertools [数据分析]
 # pypistats recent tkintertools
 # pypistats system tkintertools
 # pypistats python_minor tkintertools
 # pypistats python_major tkintertools
+
+# https://pypistats.org/packages/tkintertools [数据分析]
```

### Comparing `tkintertools-2.6.6/tkintertools/__init__.py` & `tkintertools-2.6.6.dev0/tkintertools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 from .__main__ import (Button, Canvas, CheckButton, Entry, Label, PhotoImage,
                        Progressbar, SetProcessDpiAwareness, Singleton, Text,
                        Tk, Toplevel, askfont, color, move, text)
 from .constants import *
 
 __author__ = 'Xiaokang2022<2951256653@qq.com>'
-__version__ = '2.6.6'
+__version__ = '2.6.6.dev'
 __all__ = [
     # Container Widgets
     'Tk', 'Toplevel', 'Canvas',
     # Virtual Canvas Widgets
     'Label', 'Button', 'CheckButton', 'Entry', 'Text', 'Progressbar',
     # Tool Classes
     'PhotoImage', 'Singleton',
```

### Comparing `tkintertools-2.6.6/tkintertools/__main__.py` & `tkintertools-2.6.6.dev0/tkintertools/__main__.py`

 * *Files identical despite different names*

### Comparing `tkintertools-2.6.6/tkintertools/constants.py` & `tkintertools-2.6.6.dev0/tkintertools/constants.py`

 * *Files identical despite different names*

### Comparing `tkintertools-2.6.6/tkintertools/tools_3d.py` & `tkintertools-2.6.6.dev0/tkintertools/tools_3d.py`

 * *Files 5% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         return tuple(self._items_3d)
 
     def geos(self):  # type: () -> tuple[Geometry]
         """ 返回 `Canvas_3d` 类的 `geos` 元组 """
         return tuple(self._geos)
 
     def space_sort(self):  # type: () -> None
-        """ 空间位置排序 """  # BUG: 在距离比较近的两个对象时，仍会显示不正确
+        """ 空间位置排序 """
         self._items_3d.sort(key=lambda item: (
             not isinstance(item, Point), item.camera_distance()))
         for item in self._items_3d:
             self.lower(item.item)
 
 
 class Space(Canvas_3D):
@@ -255,18 +255,14 @@
         `kx`: x 轴方向缩放比例\n
         `ky`: y 轴方向缩放比例\n
         `kz`: z 轴方向缩放比例\n
         `center`: 缩放中心，默认为几何中心\n
         """
 
     @abstractmethod
-    def center(self):
-        """ 几何中心 """
-
-    @abstractmethod
     def project(self, distance):
         """
         投影\n
         `distance`: 对象与观察者的距离\n
         """
 
 
@@ -283,21 +279,18 @@
         # type: (float, float, float, ..., Iterable[float]) -> None
         rotate(self.coords, dx, dy, dz, center=center)
 
     def scale(self, kx=1, ky=1, kz=1, *, center=None):
         # type: (float, float, float, ..., Iterable[float] | None) -> None
         scale(self.coords, kx, ky, kz, center=center)
 
-    def center(self):  # type: () -> tuple[float, float, float]
-        return tuple(self.coords)
-
     def project(self, distance):  # type: (float) -> list[float]
         relative_dis = distance - self.coords[0]
         if relative_dis <= 1e-16:
-            return [float('inf')]*2  # BUG: 目前超出范围只能让其消失
+            return [float('INF')]*2  # BUG: 目前超出范围只能让其消失
         k = distance/relative_dis
         return [self.coords[1]*k, self.coords[2]*k]
 
 
 class _Line(_3D_Object):
     """ 线 """
 
@@ -321,17 +314,14 @@
     def scale(self, kx=1, ky=1, kz=1, *, center=None):
         # type: (float, float, float, ..., Iterable[float] | None) -> None
         if center is None:
             center = [statistics.mean(axis) for axis in zip(*self.coords)]
         for coord in self.coords:
             scale(coord, kx, ky, kz, center=center)
 
-    def center(self):  # type: () -> tuple[float, float, float]
-        return tuple(statistics.mean(coords) for coords in zip(*self.coords))
-
     def project(self, distance):  # type: (float) -> list[list[float]]
         return [point.project(distance) for point in self.points]
 
 
 class _Side(_3D_Object):
     """ 面 """
 
@@ -352,17 +342,14 @@
     def scale(self, kx=1, ky=1, kz=1, *, center=None):
         # type: (float, float, float, ..., Iterable[float] | None) -> None
         if center is None:
             center = [statistics.mean(axis) for axis in zip(*self.coords)]
         for coord in self.coords:
             scale(coord, kx, ky, kz, center=center)
 
-    def center(self):  # type: () -> tuple[float, float, float]
-        return tuple(statistics.mean(coords) for coords in zip(*self.coords))
-
     def project(self, distance):  # type: (float) -> list[list[list[float]]]
         return [line.project(distance) for line in self.lines]
 
 
 class Point(_Point):
     """ 点 """
 
@@ -398,16 +385,15 @@
         """ 更新 """
         x, y = self.project(self.canvas.distance)
         self.canvas.coords(self.item, (x-self.size)*self.canvas.rx, (y-self.size) *
                            self.canvas.ry, (x+self.size)*self.canvas.rx, (y+self.size)*self.canvas.ry)
 
     def camera_distance(self):  # type: () -> float
         """ 与相机距离 """
-        sign = math.copysign(1, self.canvas.distance - self.coords[0])
-        return sign*math.dist([self.canvas.distance, 0, 0], self.coords)
+        return math.dist([self.canvas.distance, 0, 0], self.coords)
 
 
 class Line(_Line):
     """ 线 """
 
     def __init__(
         self,
@@ -436,17 +422,15 @@
     def update(self) -> None:
         """ 更新 """
         self.canvas.coords(self.item, *[coord*(self.canvas.ry if i else self.canvas.rx)
                            for point in self.project(self.canvas.distance) for i, coord in enumerate(point)])
 
     def camera_distance(self):  # type: () -> float
         """ 与相机距离 """
-        center = self.center()
-        sign = math.copysign(1, self.canvas.distance - center[0])
-        return sign*math.dist([self.canvas.distance, 0, 0], center)
+        return statistics.mean(math.dist([self.canvas.distance, 0, 0], coord) for coord in self.coords)
 
 
 class Side(_Side):
     """ 面 """
 
     def __init__(
         self,
@@ -476,17 +460,15 @@
     def update(self) -> None:
         """ 更新 """
         self.canvas.coords(self.item, *[coord*(self.canvas.ry if i else self.canvas.rx)
                            for line in self.project(self.canvas.distance) for point in line for i, coord in enumerate(point)])
 
     def camera_distance(self):  # type: () -> float
         """ 与相机距离 """
-        center = self.center()
-        sign = math.copysign(1, self.canvas.distance - center[0])
-        return sign*math.dist([self.canvas.distance, 0, 0], center)
+        return statistics.mean(math.dist([self.canvas.distance, 0, 0], coord) for coord in self.coords)
 
 
 class Geometry:
     """ 几何体 """
 
     def __init__(
         self,
@@ -498,54 +480,30 @@
         `sides`: 组成几何体的面\n
         """
         canvas._geos.append(self)
         self.canvas = canvas
         self.sides = list(sides)
 
     def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
-        """
-        平移\n
-        `dx`: x 轴方向位移距离\n
-        `dy`: y 轴方向位移距离\n
-        `dz`: z 轴方向位移距离\n
-        """
         for side in self.sides:
             side.translate(dx, dy, dz)
 
     def rotate(self, dx=0, dy=0, dz=0, *, center=[0, 0, 0]):
         # type: (float, float, float, ..., Iterable[float]) -> None
-        """
-        旋转\n
-        `dx`: 绕x 轴方向旋转弧度\n
-        `dy`: 绕y 轴方向旋转弧度\n
-        `dz`: 绕z 轴方向旋转弧度\n
-        `center`: 旋转中心\n
-        """
         for side in self.sides:
             side.rotate(dx, dy, dz, center=center)
 
     def scale(self, kx=1, ky=1, kz=1, *, center=None):
         # type: (float, float, float, ..., Iterable[float] | None) -> None
-        """
-        缩放\n
-        `kx`: x 轴方向缩放比例\n
-        `ky`: y 轴方向缩放比例\n
-        `kz`: z 轴方向缩放比例\n
-        `center`: 缩放中心，默认为几何中心\n
-        """
-        if center is None:
-            center = self.center()
+        if center is None:  # BUG: 公式对凹面几何体不成立
+            center = [statistics.mean(axis) for axis in zip(
+                *set(tuple(coord) for side in self.sides for coord in side.coords))]
         for side in self.sides:
             side.scale(kx, ky, kz, center=center)
 
-    def center(self):  # type: () -> tuple[float, float, float]
-        """ 几何中心 """
-        # BUG: 公式对凹面几何体不成立
-        return tuple(statistics.mean(axis) for axis in zip(*set(tuple(coord) for side in self.sides for coord in side.coords)))
-
     def update(self):  # type: () -> None
         """ 更新几何体 """
         for side in self.sides:
             side.update()
 
     def append(self, *sides):  # type: (Side) -> None
         """
```

