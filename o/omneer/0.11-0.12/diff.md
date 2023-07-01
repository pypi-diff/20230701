# Comparing `tmp/omneer-0.11.tar.gz` & `tmp/omneer-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omneer-0.11.tar", last modified: Sat Jul  1 05:51:24 2023, max compression
+gzip compressed data, was "omneer-0.12.tar", last modified: Sat Jul  1 07:13:31 2023, max compression
```

## Comparing `omneer-0.11.tar` & `omneer-0.12.tar`

### file list

```diff
@@ -1,12 +1,25 @@
-drwxr-xr-x   0 willblair   (502) staff       (20)        0 2023-07-01 05:51:24.072288 omneer-0.11/
--rw-r--r--   0 willblair   (502) staff       (20)     3579 2023-07-01 05:51:24.071828 omneer-0.11/PKG-INFO
--rw-r--r--   0 willblair   (502) staff       (20)     3299 2023-07-01 03:48:24.000000 omneer-0.11/README.md
-drwxr-xr-x   0 willblair   (502) staff       (20)        0 2023-07-01 05:51:24.071138 omneer-0.11/omneer.egg-info/
--rw-r--r--   0 willblair   (502) staff       (20)     3579 2023-07-01 05:51:23.000000 omneer-0.11/omneer.egg-info/PKG-INFO
--rw-r--r--   0 willblair   (502) staff       (20)      200 2023-07-01 05:51:24.000000 omneer-0.11/omneer.egg-info/SOURCES.txt
--rw-r--r--   0 willblair   (502) staff       (20)        1 2023-07-01 05:51:23.000000 omneer-0.11/omneer.egg-info/dependency_links.txt
--rw-r--r--   0 willblair   (502) staff       (20)       47 2023-07-01 05:51:23.000000 omneer-0.11/omneer.egg-info/entry_points.txt
--rw-r--r--   0 willblair   (502) staff       (20)      216 2023-07-01 05:51:23.000000 omneer-0.11/omneer.egg-info/requires.txt
--rw-r--r--   0 willblair   (502) staff       (20)        1 2023-07-01 05:51:24.000000 omneer-0.11/omneer.egg-info/top_level.txt
--rw-r--r--   0 willblair   (502) staff       (20)       38 2023-07-01 05:51:24.072443 omneer-0.11/setup.cfg
--rw-r--r--   0 willblair   (502) staff       (20)      977 2023-07-01 05:48:04.000000 omneer-0.11/setup.py
+drwxr-xr-x   0 willblair   (502) staff       (20)        0 2023-07-01 07:13:31.846172 omneer-0.12/
+-rw-r--r--   0 willblair   (502) staff       (20)     3579 2023-07-01 07:13:31.845714 omneer-0.12/PKG-INFO
+-rw-r--r--   0 willblair   (502) staff       (20)     3299 2023-07-01 03:48:24.000000 omneer-0.12/README.md
+drwxr-xr-x   0 willblair   (502) staff       (20)        0 2023-07-01 07:13:31.833123 omneer-0.12/omneer/
+-rw-r--r--   0 willblair   (502) staff       (20)        0 2023-07-01 04:10:27.000000 omneer-0.12/omneer/__init__.py
+drwxr-xr-x   0 willblair   (502) staff       (20)        0 2023-07-01 07:13:31.844735 omneer-0.12/omneer/lc/
+-rw-r--r--   0 willblair   (502) staff       (20)        0 2023-07-01 06:49:34.000000 omneer-0.12/omneer/lc/__init__.py
+-rw-r--r--   0 willblair   (502) staff       (20)     2036 2023-07-01 03:49:19.000000 omneer-0.12/omneer/lc/bootstrap.py
+-rw-r--r--   0 willblair   (502) staff       (20)     2001 2023-07-01 06:01:35.000000 omneer-0.12/omneer/lc/dataloader.py
+-rw-r--r--   0 willblair   (502) staff       (20)     2719 2023-07-01 06:01:40.000000 omneer-0.12/omneer/lc/dataset.py
+-rw-r--r--   0 willblair   (502) staff       (20)     2939 2023-07-01 07:07:40.000000 omneer-0.12/omneer/lc/main.py
+-rw-r--r--   0 willblair   (502) staff       (20)     4540 2023-07-01 04:06:37.000000 omneer-0.12/omneer/lc/misc.py
+-rw-r--r--   0 willblair   (502) staff       (20)     8230 2023-07-01 07:08:43.000000 omneer-0.12/omneer/lc/mlp.py
+-rw-r--r--   0 willblair   (502) staff       (20)     2938 2023-07-01 07:08:02.000000 omneer-0.12/omneer/lc/plot.py
+-rw-r--r--   0 willblair   (502) staff       (20)     1576 2023-07-01 03:58:50.000000 omneer-0.12/omneer/lc/shap_analysis__.py
+-rw-r--r--   0 willblair   (502) staff       (20)     3447 2023-07-01 07:08:09.000000 omneer-0.12/omneer/lc/train.py
+drwxr-xr-x   0 willblair   (502) staff       (20)        0 2023-07-01 07:13:31.836174 omneer-0.12/omneer.egg-info/
+-rw-r--r--   0 willblair   (502) staff       (20)     3579 2023-07-01 07:13:31.000000 omneer-0.12/omneer.egg-info/PKG-INFO
+-rw-r--r--   0 willblair   (502) staff       (20)      428 2023-07-01 07:13:31.000000 omneer-0.12/omneer.egg-info/SOURCES.txt
+-rw-r--r--   0 willblair   (502) staff       (20)        1 2023-07-01 07:13:31.000000 omneer-0.12/omneer.egg-info/dependency_links.txt
+-rw-r--r--   0 willblair   (502) staff       (20)       46 2023-07-01 07:13:31.000000 omneer-0.12/omneer.egg-info/entry_points.txt
+-rw-r--r--   0 willblair   (502) staff       (20)      216 2023-07-01 07:13:31.000000 omneer-0.12/omneer.egg-info/requires.txt
+-rw-r--r--   0 willblair   (502) staff       (20)        7 2023-07-01 07:13:31.000000 omneer-0.12/omneer.egg-info/top_level.txt
+-rw-r--r--   0 willblair   (502) staff       (20)       38 2023-07-01 07:13:31.846415 omneer-0.12/setup.cfg
+-rw-r--r--   0 willblair   (502) staff       (20)      968 2023-07-01 07:13:25.000000 omneer-0.12/setup.py
```

### Comparing `omneer-0.11/PKG-INFO` & `omneer-0.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omneer
-Version: 0.11
+Version: 0.12
 Summary: Advanced personalized medicine diagnostics for neurodegenerative disorders
 Home-page: http://omneer.xyz
 Author: William Blair
 Author-email: william.blair0708@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `omneer-0.11/README.md` & `omneer-0.12/README.md`

 * *Files identical despite different names*

### Comparing `omneer-0.11/omneer.egg-info/PKG-INFO` & `omneer-0.12/omneer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omneer
-Version: 0.11
+Version: 0.12
 Summary: Advanced personalized medicine diagnostics for neurodegenerative disorders
 Home-page: http://omneer.xyz
 Author: William Blair
 Author-email: william.blair0708@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `omneer-0.11/setup.py` & `omneer-0.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='omneer',
-    version='0.11',
+    version='0.12',
     packages=find_packages(include=['omneer', 'omneer.*']),
     url='http://omneer.xyz',
     license='MIT',
     author='William Blair',
     author_email='william.blair0708@gmail.com',
     description='Advanced personalized medicine diagnostics for neurodegenerative disorders',
     long_description=open('README.md').read(),
@@ -24,12 +24,12 @@
         'scikit-learn>=0.24.0',
         'torch>=1.9.0',
         'tqdm>=4.62.0',
         'xgboost>=1.4.0',
         'joblib>=1.0.0',
     ],
     entry_points={
-        'console_scripts': [
-            'omneer=omneer.lc.main:main',
+    'console_scripts': [
+        'omneer=omneer.lc.main:cli',
         ],
     },
 )
```

