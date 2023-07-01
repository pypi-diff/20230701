# Comparing `tmp/performancetest-0.0.7.tar.gz` & `tmp/performancetest-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "performancetest-0.0.7.tar", last modified: Wed Jun 28 04:58:50 2023, max compression
+gzip compressed data, was "performancetest-0.0.9.tar", last modified: Sat Jul  1 15:20:41 2023, max compression
```

## Comparing `performancetest-0.0.7.tar` & `performancetest-0.0.9.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 04:58:50.794276 performancetest-0.0.7/
--rw-rw-rw-   0        0        0      515 2023-06-28 04:58:50.794101 performancetest-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     4346 2023-06-27 05:36:55.000000 performancetest-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-28 04:58:50.749647 performancetest-0.0.7/performancetest/
--rw-rw-rw-   0        0        0       49 2023-06-21 09:23:31.000000 performancetest-0.0.7/performancetest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-28 04:58:50.782127 performancetest-0.0.7/performancetest/core/
--rw-rw-rw-   0        0        0       25 2023-05-04 05:59:55.000000 performancetest-0.0.7/performancetest/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-28 04:58:50.785591 performancetest-0.0.7/performancetest/core/base/
--rw-rw-rw-   0        0        0       25 2023-05-04 05:59:55.000000 performancetest-0.0.7/performancetest/core/base/__init__.py
--rw-rw-rw-   0        0        0      289 2023-05-04 05:59:55.000000 performancetest-0.0.7/performancetest/core/base/actuator.py
--rw-rw-rw-   0        0        0      325 2023-05-04 05:59:55.000000 performancetest-0.0.7/performancetest/core/base/monitor.py
--rw-rw-rw-   0        0        0     3562 2023-06-21 12:46:09.000000 performancetest-0.0.7/performancetest/core/command.py
--rw-rw-rw-   0        0        0     4277 2023-06-27 06:56:49.000000 performancetest-0.0.7/performancetest/core/cpu.py
--rw-rw-rw-   0        0        0     6413 2023-06-23 08:54:45.000000 performancetest-0.0.7/performancetest/core/device.py
--rw-rw-rw-   0        0        0     4268 2023-06-21 12:46:09.000000 performancetest-0.0.7/performancetest/core/devicebattery.py
--rw-rw-rw-   0        0        0    18842 2023-06-25 06:05:19.000000 performancetest-0.0.7/performancetest/core/fps.py
--rw-rw-rw-   0        0        0      678 2023-06-21 12:46:09.000000 performancetest-0.0.7/performancetest/core/global_data.py
--rw-rw-rw-   0        0        0     3882 2023-06-27 06:56:49.000000 performancetest-0.0.7/performancetest/core/gpu.py
--rw-rw-rw-   0        0        0     6646 2023-06-21 12:47:53.000000 performancetest-0.0.7/performancetest/core/iosperf.py
--rw-rw-rw-   0        0        0     3928 2023-06-27 06:56:49.000000 performancetest-0.0.7/performancetest/core/memory.py
--rw-rw-rw-   0        0        0     4315 2023-06-23 08:54:45.000000 performancetest-0.0.7/performancetest/core/snapshot.py
--rw-rw-rw-   0        0        0     4254 2023-06-27 06:56:49.000000 performancetest-0.0.7/performancetest/core/task_handle.py
-drwxrwxrwx   0        0        0        0 2023-06-28 04:58:50.787631 performancetest-0.0.7/performancetest/test/
--rw-rw-rw-   0        0        0       25 2023-05-04 05:59:55.000000 performancetest-0.0.7/performancetest/test/__init__.py
--rw-rw-rw-   0        0        0     1133 2023-05-04 05:59:55.000000 performancetest-0.0.7/performancetest/test/all_property_test.py
-drwxrwxrwx   0        0        0        0 2023-06-28 04:58:50.792801 performancetest-0.0.7/performancetest/web/
--rw-rw-rw-   0        0        0       25 2023-05-05 12:26:54.000000 performancetest-0.0.7/performancetest/web/__init__.py
--rw-rw-rw-   0        0        0     1852 2023-06-21 12:46:09.000000 performancetest-0.0.7/performancetest/web/dao.py
--rw-rw-rw-   0        0        0      408 2023-06-21 10:25:13.000000 performancetest-0.0.7/performancetest/web/entity.py
--rw-rw-rw-   0        0        0     9205 2023-06-28 04:58:38.000000 performancetest-0.0.7/performancetest/web/main.py
--rw-rw-rw-   0        0        0    11864 2023-06-25 06:05:19.000000 performancetest-0.0.7/performancetest/web/util.py
-drwxrwxrwx   0        0        0        0 2023-06-28 04:58:50.765737 performancetest-0.0.7/performancetest.egg-info/
--rw-rw-rw-   0        0        0      515 2023-06-28 04:58:50.000000 performancetest-0.0.7/performancetest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      921 2023-06-28 04:58:50.000000 performancetest-0.0.7/performancetest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 04:58:50.000000 performancetest-0.0.7/performancetest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-28 04:58:50.000000 performancetest-0.0.7/performancetest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-28 04:58:50.794831 performancetest-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      843 2023-06-28 04:58:38.000000 performancetest-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 15:20:41.408991 performancetest-0.0.9/
+-rw-rw-rw-   0        0        0      515 2023-07-01 15:20:41.408991 performancetest-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4957 2023-07-01 12:21:28.000000 performancetest-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 15:20:41.381991 performancetest-0.0.9/performancetest/
+-rw-rw-rw-   0        0        0       49 2023-06-22 08:15:17.000000 performancetest-0.0.9/performancetest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 15:20:41.399991 performancetest-0.0.9/performancetest/core/
+-rw-rw-rw-   0        0        0      715 2023-07-01 13:53:47.000000 performancetest-0.0.9/performancetest/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 15:20:41.401991 performancetest-0.0.9/performancetest/core/base/
+-rw-rw-rw-   0        0        0      767 2023-07-01 13:55:25.000000 performancetest-0.0.9/performancetest/core/base/__init__.py
+-rw-rw-rw-   0        0        0     5614 2023-07-01 13:55:25.000000 performancetest-0.0.9/performancetest/core/base/actuator.py
+-rw-rw-rw-   0        0        0     5714 2023-07-01 13:55:25.000000 performancetest-0.0.9/performancetest/core/base/monitor.py
+-rw-rw-rw-   0        0        0    17115 2023-07-01 13:53:47.000000 performancetest-0.0.9/performancetest/core/command.py
+-rw-rw-rw-   0        0        0    18820 2023-07-01 13:53:47.000000 performancetest-0.0.9/performancetest/core/cpu.py
+-rw-rw-rw-   0        0        0    33907 2023-07-01 13:53:47.000000 performancetest-0.0.9/performancetest/core/device.py
+-rw-rw-rw-   0        0        0    23641 2023-07-01 13:53:47.000000 performancetest-0.0.9/performancetest/core/devicebattery.py
+-rw-rw-rw-   0        0        0    41533 2023-07-01 13:53:47.000000 performancetest-0.0.9/performancetest/core/fps.py
+-rw-rw-rw-   0        0        0     3796 2023-07-01 13:53:47.000000 performancetest-0.0.9/performancetest/core/global_data.py
+-rw-rw-rw-   0        0        0    18007 2023-07-01 13:53:47.000000 performancetest-0.0.9/performancetest/core/gpu.py
+-rw-rw-rw-   0        0        0    22000 2023-07-01 13:53:47.000000 performancetest-0.0.9/performancetest/core/iosperf.py
+-rw-rw-rw-   0        0        0    18284 2023-07-01 13:53:47.000000 performancetest-0.0.9/performancetest/core/memory.py
+-rw-rw-rw-   0        0        0    23596 2023-07-01 13:53:47.000000 performancetest-0.0.9/performancetest/core/snapshot.py
+-rw-rw-rw-   0        0        0    15097 2023-07-01 13:53:47.000000 performancetest-0.0.9/performancetest/core/task_handle.py
+drwxrwxrwx   0        0        0        0 2023-07-01 15:20:41.402991 performancetest-0.0.9/performancetest/pyarmor_runtime_000000/
+-rw-rw-rw-   0        0        0      103 2023-07-01 13:52:15.000000 performancetest-0.0.9/performancetest/pyarmor_runtime_000000/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 15:20:41.403990 performancetest-0.0.9/performancetest/test/
+-rw-rw-rw-   0        0        0       25 2023-05-01 16:15:41.000000 performancetest-0.0.9/performancetest/test/__init__.py
+-rw-rw-rw-   0        0        0     1133 2023-06-15 15:11:01.000000 performancetest-0.0.9/performancetest/test/all_property_test.py
+drwxrwxrwx   0        0        0        0 2023-07-01 15:20:41.407990 performancetest-0.0.9/performancetest/web/
+-rw-rw-rw-   0        0        0       25 2023-05-07 12:34:19.000000 performancetest-0.0.9/performancetest/web/__init__.py
+-rw-rw-rw-   0        0        0     1852 2023-06-22 08:15:17.000000 performancetest-0.0.9/performancetest/web/dao.py
+-rw-rw-rw-   0        0        0      408 2023-06-10 10:20:09.000000 performancetest-0.0.9/performancetest/web/entity.py
+-rw-rw-rw-   0        0        0     9205 2023-07-01 12:18:21.000000 performancetest-0.0.9/performancetest/web/main.py
+-rw-rw-rw-   0        0        0    11864 2023-06-24 11:48:14.000000 performancetest-0.0.9/performancetest/web/util.py
+drwxrwxrwx   0        0        0        0 2023-07-01 15:20:41.389990 performancetest-0.0.9/performancetest.egg-info/
+-rw-rw-rw-   0        0        0      515 2023-07-01 15:20:41.000000 performancetest-0.0.9/performancetest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      972 2023-07-01 15:20:41.000000 performancetest-0.0.9/performancetest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 15:20:41.000000 performancetest-0.0.9/performancetest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-01 15:20:41.000000 performancetest-0.0.9/performancetest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 15:20:41.408991 performancetest-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      873 2023-07-01 15:20:38.000000 performancetest-0.0.9/setup.py
```

### Comparing `performancetest-0.0.7/PKG-INFO` & `performancetest-0.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: performancetest
-Version: 0.0.7
+Version: 0.0.9
 Summary: Android, IOS app_performance
 Home-page: https://github.com/1033866383/perf-orange-cat
 Author: bozhou.fan
 Author-email: 15525730080@163.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `performancetest-0.0.7/README.md` & `performancetest-0.0.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,65 @@
 <h1>perf-orange-cat</h1>
 <br/>
-<h1>客户端性能测试平台 https://github.com/1033866383/perf-orange-cat/releases </h1>
+<h1>客户端性能测试平台</h1>
 
 ![微信图片_20230624120931](https://github.com/1033866383/perf-orange-cat/assets/56209295/ce1d47eb-01bb-41d8-88d4-e07828aea825)
 
 <h2>演示地址：http://112.126.75.188/</h2>
 
+<h2>源码地址：
+    https://github.com/1033866383/perf-orange-cat
+    <br/>
+    or 
+    <br/>
+    https://github.com/1033866383/app_performance_private/tree/perf-orange-cat</h2>
+    <h2>
+        安装：pip install -U performancetest 
+        <br/><br/>
+            启动：python -m performancetest.web.main   
+        <br/><br/>
+        启动后访问：http://localhost/ 即可开始Android/IOS性能测试 
+        <br/><br/>
+        API文档访问：http://localhost/redoc/
+        <br/><br/>
+        环境要求：python3.9+ 如果python版本有问题可以使用pyenv:https://github.com/pyenv/pyenv 
+        去做环境隔离<br/><br/>
+    </h2>
 <h2>简介</h2>
 <ul>
     <li>替代perfdog等客户端性能测试工具</li>
     <li>支持Android/IOS平台上应用的性能数据测试，包含游戏和视频类app的性能测试</li>
     <li>支持指标包含:cpu,memory,fps,gpu,温度,电量，以及他们的最大值，最小值，平均值</li>
-    <li>fps指标中包含：，卡顿（jank），强卡顿（big jank），卡顿率等指标,等指标</li>
+    <li>fps指标中包含：卡顿（jank），强卡顿（big jank），卡顿率等指标,等指标</li>
     <li>数据结果准确，与perfdog一致</li>
     <li>可用实时记录设备画面，点击图片或者点击图标上的点可用跳转到对对应的场景。</li>
     <li>支持局域网内使用，此平台部署服务后整个局域网访问服务页面就可以直接对本机设备进行性能测试</li>
     <li>提供可执行文件直接执行部署即可，提供api详情</li>
 </ul>
 
 <h2>目录介绍</h2>
 <ul>
 <li>test_result/ 包含前端页面和测试结果。</li>
 <li>log.log 为项目运行日志。</li>
 <li>task.sqlite 为sqllite数据库，包含了每个任务的基本详情也是唯一的dao对象。</li>
-<li>其他可执行文件为不同平台的可执行文件。</li>
 </ul>
 
 ![image](https://github.com/1033866383/perf-orange-cat/assets/56209295/852cda82-058b-4832-9daf-8074c1a7bb6b)
 
 <h2>使用教程</h2>
-1.运行exe， Pyinstaller打包的项目首次启动时可能会稍微慢一点。
+建议使用上方的 pip install 的方式装包启动。 
+<br/>
+1.pip install -U performancetest 
+
+![image](https://github.com/1033866383/perf-orange-cat/assets/56209295/b0d566fd-cf1e-4fd2-85eb-21f1e3762619)
 
-![image](https://github.com/1033866383/perf-orange-cat/assets/56209295/fc99180b-1e26-47e4-87a6-cc3db7d9b9e8)
 
-2.此时项目已经启动了。
+2.python -m performancetest.web.main  此时项目已经启动了。
 
-![image](https://github.com/1033866383/perf-orange-cat/assets/56209295/baae938d-bf01-4f3b-a5e6-0309a718cf2d)
+![image](https://github.com/1033866383/perf-orange-cat/assets/56209295/38f32ab0-a967-4cc4-963a-e57320e9da11)
 
 3.访问http://localhost/。
 
 默认页面：
 
 ![image](https://github.com/1033866383/perf-orange-cat/assets/56209295/100c40ee-499f-437f-8f98-e4469f946e6e)
```

### Comparing `performancetest-0.0.7/performancetest/test/all_property_test.py` & `performancetest-0.0.9/performancetest/test/all_property_test.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.7/performancetest/web/dao.py` & `performancetest-0.0.9/performancetest/web/dao.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.7/performancetest/web/main.py` & `performancetest-0.0.9/performancetest/web/main.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.7/performancetest/web/util.py` & `performancetest-0.0.9/performancetest/web/util.py`

 * *Files identical despite different names*

### Comparing `performancetest-0.0.7/performancetest.egg-info/PKG-INFO` & `performancetest-0.0.9/performancetest.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: performancetest
-Version: 0.0.7
+Version: 0.0.9
 Summary: Android, IOS app_performance
 Home-page: https://github.com/1033866383/perf-orange-cat
 Author: bozhou.fan
 Author-email: 15525730080@163.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `performancetest-0.0.7/performancetest.egg-info/SOURCES.txt` & `performancetest-0.0.9/performancetest.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 performancetest/core/iosperf.py
 performancetest/core/memory.py
 performancetest/core/snapshot.py
 performancetest/core/task_handle.py
 performancetest/core/base/__init__.py
 performancetest/core/base/actuator.py
 performancetest/core/base/monitor.py
+performancetest/pyarmor_runtime_000000/__init__.py
 performancetest/test/__init__.py
 performancetest/test/all_property_test.py
 performancetest/web/__init__.py
 performancetest/web/dao.py
 performancetest/web/entity.py
 performancetest/web/main.py
 performancetest/web/util.py
```

### Comparing `performancetest-0.0.7/setup.py` & `performancetest-0.0.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # # _*_ coding: utf-8 _*_
 from setuptools import setup, find_packages
 
 setup(
        name='performancetest',
-       version='0.0.7',
+       version='0.0.9',
        url='https://github.com/1033866383/perf-orange-cat',
        author='bozhou.fan',
        author_email='15525730080@163.com',
        description='Android, IOS app_performance',
        packages=find_packages(),
        install_requires=[],
        include_package_data=True,  # 这里添加 include_package_data 参数
        package_data={
-           'performancetest': ['web/test_result/*']
+           'performancetest': ['web/test_result/*', 'pyarmor_runtime_000000/*']
        },
        classifiers=[
            'Development Status :: 3 - Alpha',
            'Intended Audience :: Developers',
            'License :: OSI Approved :: MIT License',
            'Programming Language :: Python :: 3',
            'Programming Language :: Python :: 3.9',
        ],
-   )
+   )
```

