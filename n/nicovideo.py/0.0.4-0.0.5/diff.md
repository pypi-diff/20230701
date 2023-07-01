# Comparing `tmp/nicovideo.py-0.0.4.tar.gz` & `tmp/nicovideo.py-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nicovideo.py-0.0.4.tar", last modified: Sat Jul  1 05:48:46 2023, max compression
+gzip compressed data, was "nicovideo.py-0.0.5.tar", last modified: Sat Jul  1 07:09:59 2023, max compression
```

## Comparing `nicovideo.py-0.0.4.tar` & `nicovideo.py-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-07-01 05:48:46.563040 nicovideo.py-0.0.4/
--rw-rw-r--   0 okaits    (1000) okaits    (1000)     7559 2023-06-24 05:49:10.000000 nicovideo.py-0.0.4/LICENSE.md
--rw-rw-r--   0 okaits    (1000) okaits    (1000)     3557 2023-07-01 05:48:46.563040 nicovideo.py-0.0.4/PKG-INFO
--rw-rw-r--   0 okaits    (1000) okaits    (1000)     2802 2023-06-24 15:54:52.000000 nicovideo.py-0.0.4/README.md
-drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-07-01 05:48:46.563040 nicovideo.py-0.0.4/nicovideo/
--rw-rw-r--   0 okaits    (1000) okaits    (1000)     4784 2023-07-01 05:47:03.000000 nicovideo.py-0.0.4/nicovideo/__init__.py
-drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-07-01 05:48:46.563040 nicovideo.py-0.0.4/nicovideo.py.egg-info/
--rw-rw-r--   0 okaits    (1000) okaits    (1000)     3557 2023-07-01 05:48:46.000000 nicovideo.py-0.0.4/nicovideo.py.egg-info/PKG-INFO
--rw-rw-r--   0 okaits    (1000) okaits    (1000)      195 2023-07-01 05:48:46.000000 nicovideo.py-0.0.4/nicovideo.py.egg-info/SOURCES.txt
--rw-rw-r--   0 okaits    (1000) okaits    (1000)        1 2023-07-01 05:48:46.000000 nicovideo.py-0.0.4/nicovideo.py.egg-info/dependency_links.txt
--rw-rw-r--   0 okaits    (1000) okaits    (1000)       10 2023-07-01 05:48:46.000000 nicovideo.py-0.0.4/nicovideo.py.egg-info/top_level.txt
--rw-rw-r--   0 okaits    (1000) okaits    (1000)       38 2023-07-01 05:48:46.563040 nicovideo.py-0.0.4/setup.cfg
--rw-rw-r--   0 okaits    (1000) okaits    (1000)      993 2023-07-01 05:47:08.000000 nicovideo.py-0.0.4/setup.py
+drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-07-01 07:09:59.785252 nicovideo.py-0.0.5/
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)     7559 2023-06-24 05:49:10.000000 nicovideo.py-0.0.5/LICENSE.md
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)     3557 2023-07-01 07:09:59.785252 nicovideo.py-0.0.5/PKG-INFO
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)     2802 2023-06-24 15:54:52.000000 nicovideo.py-0.0.5/README.md
+drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-07-01 07:09:59.785252 nicovideo.py-0.0.5/nicovideo/
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)    10894 2023-07-01 07:08:21.000000 nicovideo.py-0.0.5/nicovideo/__init__.py
+drwxrwxr-x   0 okaits    (1000) okaits    (1000)        0 2023-07-01 07:09:59.785252 nicovideo.py-0.0.5/nicovideo.py.egg-info/
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)     3557 2023-07-01 07:09:59.000000 nicovideo.py-0.0.5/nicovideo.py.egg-info/PKG-INFO
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)      195 2023-07-01 07:09:59.000000 nicovideo.py-0.0.5/nicovideo.py.egg-info/SOURCES.txt
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)        1 2023-07-01 07:09:59.000000 nicovideo.py-0.0.5/nicovideo.py.egg-info/dependency_links.txt
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)       10 2023-07-01 07:09:59.000000 nicovideo.py-0.0.5/nicovideo.py.egg-info/top_level.txt
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)       38 2023-07-01 07:09:59.785252 nicovideo.py-0.0.5/setup.cfg
+-rw-rw-r--   0 okaits    (1000) okaits    (1000)      993 2023-07-01 07:08:25.000000 nicovideo.py-0.0.5/setup.py
```

### Comparing `nicovideo.py-0.0.4/LICENSE.md` & `nicovideo.py-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nicovideo.py-0.0.4/PKG-INFO` & `nicovideo.py-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nicovideo.py
-Version: 0.0.4
+Version: 0.0.5
 Summary: Get nicovideo's video metadata.
 Home-page: https://github.com/okaits/nicovideo.py
 Author: okaits#7534
 Author-email: okaits@okaits7534.mydns.jp
 License: GNU Lesser General Public License 3.0
 Keywords: nicovideo
 Platform: UNKNOWN
```

### Comparing `nicovideo.py-0.0.4/README.md` & `nicovideo.py-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nicovideo.py-0.0.4/nicovideo.py.egg-info/PKG-INFO` & `nicovideo.py-0.0.5/nicovideo.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nicovideo.py
-Version: 0.0.4
+Version: 0.0.5
 Summary: Get nicovideo's video metadata.
 Home-page: https://github.com/okaits/nicovideo.py
 Author: okaits#7534
 Author-email: okaits@okaits7534.mydns.jp
 License: GNU Lesser General Public License 3.0
 Keywords: nicovideo
 Platform: UNKNOWN
```

### Comparing `nicovideo.py-0.0.4/setup.py` & `nicovideo.py-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import find_packages, setup
 
 readme = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name='nicovideo.py',
-    version='0.0.4',
+    version='0.0.5',
     description='Get nicovideo\'s video metadata.',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='okaits#7534',
     author_email='okaits@okaits7534.mydns.jp',
     url='https://github.com/okaits/nicovideo.py',
     classifiers=[
```

