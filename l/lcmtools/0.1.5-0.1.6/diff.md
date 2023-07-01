# Comparing `tmp/lcmtools-0.1.5.tar.gz` & `tmp/lcmtools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcmtools-0.1.5.tar", last modified: Sat Jul  1 14:53:30 2023, max compression
+gzip compressed data, was "lcmtools-0.1.6.tar", last modified: Sat Jul  1 17:45:11 2023, max compression
```

## Comparing `lcmtools-0.1.5.tar` & `lcmtools-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 14:53:30.111605 lcmtools-0.1.5/
--rw-rw-rw-   0        0        0     1086 2023-02-23 06:51:28.000000 lcmtools-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     1965 2023-07-01 14:53:30.110601 lcmtools-0.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-01 14:53:30.104724 lcmtools-0.1.5/lcmtools/
--rw-rw-rw-   0        0        0       42 2023-02-23 14:29:02.000000 lcmtools-0.1.5/lcmtools/__init__.py
--rw-rw-rw-   0        0        0      336 2023-07-01 14:44:31.000000 lcmtools-0.1.5/lcmtools/__version__.py
--rw-rw-rw-   0        0        0    13332 2023-07-01 14:33:16.000000 lcmtools-0.1.5/lcmtools/lcmtools.py
-drwxrwxrwx   0        0        0        0 2023-07-01 14:53:30.110097 lcmtools-0.1.5/lcmtools.egg-info/
--rw-rw-rw-   0        0        0     1965 2023-07-01 14:53:30.000000 lcmtools-0.1.5/lcmtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-07-01 14:53:30.000000 lcmtools-0.1.5/lcmtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 14:53:30.000000 lcmtools-0.1.5/lcmtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-01 14:53:30.000000 lcmtools-0.1.5/lcmtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-01 14:53:30.000000 lcmtools-0.1.5/lcmtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 14:53:30.111605 lcmtools-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     3924 2023-07-01 14:44:39.000000 lcmtools-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 17:45:11.204542 lcmtools-0.1.6/
+-rw-rw-rw-   0        0        0     1086 2023-02-23 06:51:28.000000 lcmtools-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     1965 2023-07-01 17:45:11.201252 lcmtools-0.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-01 17:45:11.191470 lcmtools-0.1.6/lcmtools/
+-rw-rw-rw-   0        0        0       42 2023-02-23 14:29:02.000000 lcmtools-0.1.6/lcmtools/__init__.py
+-rw-rw-rw-   0        0        0      336 2023-07-01 17:44:43.000000 lcmtools-0.1.6/lcmtools/__version__.py
+-rw-rw-rw-   0        0        0    13585 2023-07-01 15:00:49.000000 lcmtools-0.1.6/lcmtools/lcmtools.py
+drwxrwxrwx   0        0        0        0 2023-07-01 17:45:11.200252 lcmtools-0.1.6/lcmtools.egg-info/
+-rw-rw-rw-   0        0        0     1965 2023-07-01 17:45:11.000000 lcmtools-0.1.6/lcmtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-07-01 17:45:11.000000 lcmtools-0.1.6/lcmtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 17:45:11.000000 lcmtools-0.1.6/lcmtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-01 17:45:11.000000 lcmtools-0.1.6/lcmtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-01 17:45:11.000000 lcmtools-0.1.6/lcmtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 17:45:11.204542 lcmtools-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     3924 2023-07-01 17:44:53.000000 lcmtools-0.1.6/setup.py
```

### Comparing `lcmtools-0.1.5/LICENSE` & `lcmtools-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lcmtools-0.1.5/PKG-INFO` & `lcmtools-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcmtools
-Version: 0.1.5
+Version: 0.1.6
 Summary: A script that calls LCModel through Python.
 Home-page: https://github.com/luodeb/lcmtools
 Author: Luo Debin
 Author-email: luodeb@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lcmtools Version: 0.1.5 Summary: A script that
+Metadata-Version: 2.1 Name: lcmtools Version: 0.1.6 Summary: A script that
 calls LCModel through Python. Home-page: https://github.com/luodeb/lcmtools
 Author: Luo Debin Author-email: luodeb@qq.com License: MIT Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Requires-Python: >=3.6.0 Description-Content-Type: text/
```

### Comparing `lcmtools-0.1.5/lcmtools/lcmtools.py` & `lcmtools-0.1.6/lcmtools/lcmtools.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,28 @@
 import numpy as np
 import locale
 import ghostscript
 from scipy import signal
 import time
 
 class LCMConfig(object):
+    '''
+    echot = "30"
+    hzpppm = "1.27731e+02"
+    nsize = "2048"
+
+    ppmst = "4.0"
+    ppmend = "0.2"
+    deltat = '2.500e-04'
+    B0 = '3.0'
+    seq = 'PRESS'
+    # 输入文件方式配置信息
+    filraw:str = None
+    '''
+    
     # 输入data方式配置信息
     echot = "30"
     hzpppm = "1.27731e+02"
     nsize = "2048"
 
     ppmst = "4.0"
     ppmend = "0.2"
```

### Comparing `lcmtools-0.1.5/lcmtools.egg-info/PKG-INFO` & `lcmtools-0.1.6/lcmtools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcmtools
-Version: 0.1.5
+Version: 0.1.6
 Summary: A script that calls LCModel through Python.
 Home-page: https://github.com/luodeb/lcmtools
 Author: Luo Debin
 Author-email: luodeb@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lcmtools Version: 0.1.5 Summary: A script that
+Metadata-Version: 2.1 Name: lcmtools Version: 0.1.6 Summary: A script that
 calls LCModel through Python. Home-page: https://github.com/luodeb/lcmtools
 Author: Luo Debin Author-email: luodeb@qq.com License: MIT Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Requires-Python: >=3.6.0 Description-Content-Type: text/
```

### Comparing `lcmtools-0.1.5/setup.py` & `lcmtools-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'lcmtools'
 DESCRIPTION = 'A script that calls LCModel through Python.'
 URL = 'https://github.com/luodeb/lcmtools'
 EMAIL = 'luodeb@qq.com'
 AUTHOR = 'Luo Debin'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.5'
+VERSION = '0.1.6'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'python3-ghostscript', 'numpy', 'scipy',
 ]
 
 # What packages are optional?
```

