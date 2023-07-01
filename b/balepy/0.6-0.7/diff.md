# Comparing `tmp/balepy-0.6.tar.gz` & `tmp/balepy-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balepy-0.6.tar", last modified: Tue Jun 27 19:57:54 2023, max compression
+gzip compressed data, was "balepy-0.7.tar", last modified: Sat Jul  1 14:43:26 2023, max compression
```

## Comparing `balepy-0.6.tar` & `balepy-0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-27 19:57:54.150265 balepy-0.6/
--rw-r--r--   0 themamad  (1000) themamad  (1000)     1077 2023-06-20 12:51:32.000000 balepy-0.6/LICENSE
--rw-r--r--   0 themamad  (1000) themamad  (1000)      990 2023-06-27 19:57:54.150265 balepy-0.6/PKG-INFO
--rw-r--r--   0 themamad  (1000) themamad  (1000)      238 2023-06-26 14:07:46.000000 balepy-0.6/README.md
-drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-27 19:57:54.150265 balepy-0.6/balepy/
--rw-r--r--   0 themamad  (1000) themamad  (1000)     2109 2023-06-27 19:57:31.000000 balepy-0.6/balepy/__init__.py
-drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-27 19:57:54.150265 balepy-0.6/balepy.egg-info/
--rw-r--r--   0 themamad  (1000) themamad  (1000)      990 2023-06-27 19:57:54.000000 balepy-0.6/balepy.egg-info/PKG-INFO
--rw-r--r--   0 themamad  (1000) themamad  (1000)      165 2023-06-27 19:57:54.000000 balepy-0.6/balepy.egg-info/SOURCES.txt
--rw-r--r--   0 themamad  (1000) themamad  (1000)        1 2023-06-27 19:57:54.000000 balepy-0.6/balepy.egg-info/dependency_links.txt
--rw-r--r--   0 themamad  (1000) themamad  (1000)        7 2023-06-27 19:57:54.000000 balepy-0.6/balepy.egg-info/top_level.txt
--rw-r--r--   0 themamad  (1000) themamad  (1000)       38 2023-06-27 19:57:54.150265 balepy-0.6/setup.cfg
--rw-r--r--   0 themamad  (1000) themamad  (1000)      987 2023-06-27 19:57:15.000000 balepy-0.6/setup.py
+drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-07-01 14:43:26.358563 balepy-0.7/
+-rw-r--r--   0 themamad  (1000) themamad  (1000)     1077 2023-06-20 12:51:32.000000 balepy-0.7/LICENSE
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      997 2023-07-01 14:43:26.358563 balepy-0.7/PKG-INFO
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      245 2023-07-01 14:42:36.000000 balepy-0.7/README.md
+drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-07-01 14:43:26.358563 balepy-0.7/balepy/
+-rw-r--r--   0 themamad  (1000) themamad  (1000)     4400 2023-07-01 14:42:59.000000 balepy-0.7/balepy/__init__.py
+drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-07-01 14:43:26.358563 balepy-0.7/balepy.egg-info/
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      997 2023-07-01 14:43:26.000000 balepy-0.7/balepy.egg-info/PKG-INFO
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      165 2023-07-01 14:43:26.000000 balepy-0.7/balepy.egg-info/SOURCES.txt
+-rw-r--r--   0 themamad  (1000) themamad  (1000)        1 2023-07-01 14:43:26.000000 balepy-0.7/balepy.egg-info/dependency_links.txt
+-rw-r--r--   0 themamad  (1000) themamad  (1000)        7 2023-07-01 14:43:26.000000 balepy-0.7/balepy.egg-info/top_level.txt
+-rw-r--r--   0 themamad  (1000) themamad  (1000)       38 2023-07-01 14:43:26.358563 balepy-0.7/setup.cfg
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      987 2023-07-01 14:42:17.000000 balepy-0.7/setup.py
```

### Comparing `balepy-0.6/LICENSE` & `balepy-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `balepy-0.6/PKG-INFO` & `balepy-0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balepy
-Version: 0.6
+Version: 0.7
 Summary: balepy a Library Python for create bot API in bale application
 Home-page: https://github.com/OnlyRad/bale
 Author: Mohammad and Erfan
 Author-email: mohammadmehrabi175@gmail.com
 Keywords: bot,Bot,bale,robot
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -26,14 +26,14 @@
 
 ```python
 pip install -U balepy
 ```
 
 => START
 
-> doc: github.com/onlyrad
+> doc: github.com/onlyrad/balepy
 
 <hr>
 
 # Social Media:
 ### Rubika: @TheLinux
 ### Rubika: @Tommy969
```

### Comparing `balepy-0.6/balepy.egg-info/PKG-INFO` & `balepy-0.7/balepy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balepy
-Version: 0.6
+Version: 0.7
 Summary: balepy a Library Python for create bot API in bale application
 Home-page: https://github.com/OnlyRad/bale
 Author: Mohammad and Erfan
 Author-email: mohammadmehrabi175@gmail.com
 Keywords: bot,Bot,bale,robot
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -26,14 +26,14 @@
 
 ```python
 pip install -U balepy
 ```
 
 => START
 
-> doc: github.com/onlyrad
+> doc: github.com/onlyrad/balepy
 
 <hr>
 
 # Social Media:
 ### Rubika: @TheLinux
 ### Rubika: @Tommy969
```

### Comparing `balepy-0.6/setup.py` & `balepy-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'balepy',
-    version = '0.6',
+    version = '0.7',
     author='Mohammad and Erfan',
     author_email = 'mohammadmehrabi175@gmail.com',
     description = 'balepy a Library Python for create bot API in bale application',
     keywords = ['bot' , 'Bot' , 'bale' , 'robot'],
     long_description = open("README.md", encoding="utf-8").read(),
     python_requires="~=3.6",
     long_description_content_type = 'text/markdown',
```

