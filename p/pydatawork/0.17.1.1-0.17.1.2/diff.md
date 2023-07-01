# Comparing `tmp/pydatawork-0.17.1.1.tar.gz` & `tmp/pydatawork-0.17.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.17.1.1.tar", last modified: Sat Jul  1 17:18:52 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.17.1.2.tar", last modified: Sat Jul  1 17:22:18 2023, max compression
```

## Comparing `pydatawork-0.17.1.1.tar` & `pydatawork-0.17.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-01 17:18:52.000000 pydatawork-0.17.1.1/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    15536 2023-07-01 17:18:52.000000 pydatawork-0.17.1.1/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    12025 2023-07-01 17:17:45.000000 pydatawork-0.17.1.1/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-01 17:18:52.000000 pydatawork-0.17.1.1/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    15536 2023-07-01 17:18:52.000000 pydatawork-0.17.1.1/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-01 17:18:52.000000 pydatawork-0.17.1.1/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-01 17:18:52.000000 pydatawork-0.17.1.1/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-01 17:18:52.000000 pydatawork-0.17.1.1/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    32580 2023-07-01 17:10:17.000000 pydatawork-0.17.1.1/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-01 17:18:52.000000 pydatawork-0.17.1.1/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-01 16:36:42.000000 pydatawork-0.17.1.1/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-01 17:22:18.000000 pydatawork-0.17.1.2/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    15522 2023-07-01 17:22:18.000000 pydatawork-0.17.1.2/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    12011 2023-07-01 17:20:59.000000 pydatawork-0.17.1.2/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-01 17:22:18.000000 pydatawork-0.17.1.2/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    15522 2023-07-01 17:22:18.000000 pydatawork-0.17.1.2/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-01 17:22:18.000000 pydatawork-0.17.1.2/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-01 17:22:18.000000 pydatawork-0.17.1.2/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-01 17:22:18.000000 pydatawork-0.17.1.2/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    32580 2023-07-01 17:10:17.000000 pydatawork-0.17.1.2/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-01 17:22:18.000000 pydatawork-0.17.1.2/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-01 17:22:12.000000 pydatawork-0.17.1.2/setup.py
```

### Comparing `pydatawork-0.17.1.1/PKG-INFO` & `pydatawork-0.17.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.1.1
+Version: 0.17.1.2
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
         https://docs.qq.com/form/page/DZVNabWlkRUtldWtJ
         
         
         # functions and description
         
         
         
-        ## move_files_by_keyword() 按文件名中的关键词移动文件，灵活提取文件 （v 0.17.1.1）
+        ## move_files_by_keyword() 按文件名中关键词移动文件，灵活提取文件 (v 0.17.1.2)
         
         ###### Sun Jul 2 24:35:12 CST 2023
         
         ```python
         def move_files_by_keyword(raw_data_path,working_path):
             """
             raw_data_path：原始数据所在路径。（不会移动子文件夹，也不会遍历子文件夹）
@@ -27,15 +27,15 @@
             keyword（不是参数）：指文件名中包含的关键词，不是参数，程序运行后，在命令行中根据提示按需输入。
             目标：根据文件名中的关键词移动文件。
             """
         ```
         
         
         
-        ## copy_files_by_keyword() 按文件名中的关键词复制文件，灵活提取文件 （v 0.17.1.1）
+        ## copy_files_by_keyword() 按文件名中关键词复制文件，灵活提取文件 (v 0.17.1.2)
         
         ###### Sun Jul 2 24:28:40 CST 2023
         
         ```python
         def copy_files_by_keyword(raw_data_path,working_path):
             """
             raw_data_path：原始数据所在路径。（不会复制子文件夹，也不会遍历子文件夹）
```

### Comparing `pydatawork-0.17.1.1/README.md` & `pydatawork-0.17.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 https://docs.qq.com/form/page/DZVNabWlkRUtldWtJ
 
 
 # functions and description
 
 
 
-## move_files_by_keyword() 按文件名中的关键词移动文件，灵活提取文件 （v 0.17.1.1）
+## move_files_by_keyword() 按文件名中关键词移动文件，灵活提取文件 (v 0.17.1.2)
 
 ###### Sun Jul 2 24:35:12 CST 2023
 
 ```python
 def move_files_by_keyword(raw_data_path,working_path):
     """
     raw_data_path：原始数据所在路径。（不会移动子文件夹，也不会遍历子文件夹）
@@ -19,15 +19,15 @@
     keyword（不是参数）：指文件名中包含的关键词，不是参数，程序运行后，在命令行中根据提示按需输入。
     目标：根据文件名中的关键词移动文件。
     """
 ```
 
 
 
-## copy_files_by_keyword() 按文件名中的关键词复制文件，灵活提取文件 （v 0.17.1.1）
+## copy_files_by_keyword() 按文件名中关键词复制文件，灵活提取文件 (v 0.17.1.2)
 
 ###### Sun Jul 2 24:28:40 CST 2023
 
 ```python
 def copy_files_by_keyword(raw_data_path,working_path):
     """
     raw_data_path：原始数据所在路径。（不会复制子文件夹，也不会遍历子文件夹）
```

### Comparing `pydatawork-0.17.1.1/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.17.1.2/pydatawork.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.1.1
+Version: 0.17.1.2
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
         https://docs.qq.com/form/page/DZVNabWlkRUtldWtJ
         
         
         # functions and description
         
         
         
-        ## move_files_by_keyword() 按文件名中的关键词移动文件，灵活提取文件 （v 0.17.1.1）
+        ## move_files_by_keyword() 按文件名中关键词移动文件，灵活提取文件 (v 0.17.1.2)
         
         ###### Sun Jul 2 24:35:12 CST 2023
         
         ```python
         def move_files_by_keyword(raw_data_path,working_path):
             """
             raw_data_path：原始数据所在路径。（不会移动子文件夹，也不会遍历子文件夹）
@@ -27,15 +27,15 @@
             keyword（不是参数）：指文件名中包含的关键词，不是参数，程序运行后，在命令行中根据提示按需输入。
             目标：根据文件名中的关键词移动文件。
             """
         ```
         
         
         
-        ## copy_files_by_keyword() 按文件名中的关键词复制文件，灵活提取文件 （v 0.17.1.1）
+        ## copy_files_by_keyword() 按文件名中关键词复制文件，灵活提取文件 (v 0.17.1.2)
         
         ###### Sun Jul 2 24:28:40 CST 2023
         
         ```python
         def copy_files_by_keyword(raw_data_path,working_path):
             """
             raw_data_path：原始数据所在路径。（不会复制子文件夹，也不会遍历子文件夹）
```

### Comparing `pydatawork-0.17.1.1/pydatawork.py` & `pydatawork-0.17.1.2/pydatawork.py`

 * *Files identical despite different names*

### Comparing `pydatawork-0.17.1.1/setup.py` & `pydatawork-0.17.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.17.1.1',
+    version='0.17.1.2',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

