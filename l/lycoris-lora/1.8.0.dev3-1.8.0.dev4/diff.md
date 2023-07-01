# Comparing `tmp/lycoris_lora-1.8.0.dev3.tar.gz` & `tmp/lycoris_lora-1.8.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lycoris_lora-1.8.0.dev3.tar", last modified: Sat Jul  1 07:45:27 2023, max compression
+gzip compressed data, was "lycoris_lora-1.8.0.dev4.tar", last modified: Sat Jul  1 11:58:09 2023, max compression
```

## Comparing `lycoris_lora-1.8.0.dev3.tar` & `lycoris_lora-1.8.0.dev4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 07:45:27.889606 lycoris_lora-1.8.0.dev3/
--rw-rw-rw-   0        0        0    11545 2023-06-04 13:36:43.000000 lycoris_lora-1.8.0.dev3/LICENSE.md
--rw-rw-rw-   0        0        0      353 2023-07-01 07:45:27.888605 lycoris_lora-1.8.0.dev3/PKG-INFO
--rw-rw-rw-   0        0        0     7677 2023-06-28 12:51:02.000000 lycoris_lora-1.8.0.dev3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 07:45:27.873571 lycoris_lora-1.8.0.dev3/lycoris/
--rw-rw-rw-   0        0        0       62 2023-06-29 04:44:57.000000 lycoris_lora-1.8.0.dev3/lycoris/__init__.py
--rw-rw-rw-   0        0        0    20963 2023-06-04 13:36:43.000000 lycoris_lora-1.8.0.dev3/lycoris/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-01 07:45:27.888605 lycoris_lora-1.8.0.dev3/lycoris_lora.egg-info/
--rw-rw-rw-   0        0        0      353 2023-07-01 07:45:27.000000 lycoris_lora-1.8.0.dev3/lycoris_lora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-07-01 07:45:27.000000 lycoris_lora-1.8.0.dev3/lycoris_lora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 07:45:27.000000 lycoris_lora-1.8.0.dev3/lycoris_lora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-04 13:39:16.000000 lycoris_lora-1.8.0.dev3/lycoris_lora.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-07-01 07:45:27.000000 lycoris_lora-1.8.0.dev3/lycoris_lora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-01 07:45:27.000000 lycoris_lora-1.8.0.dev3/lycoris_lora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 07:45:27.889606 lycoris_lora-1.8.0.dev3/setup.cfg
--rw-rw-rw-   0        0        0      547 2023-07-01 07:45:06.000000 lycoris_lora-1.8.0.dev3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 11:58:09.219053 lycoris_lora-1.8.0.dev4/
+-rw-rw-rw-   0        0        0    11545 2023-06-04 13:36:43.000000 lycoris_lora-1.8.0.dev4/LICENSE.md
+-rw-rw-rw-   0        0        0      353 2023-07-01 11:58:09.218056 lycoris_lora-1.8.0.dev4/PKG-INFO
+-rw-rw-rw-   0        0        0     7677 2023-06-28 12:51:02.000000 lycoris_lora-1.8.0.dev4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 11:58:09.201043 lycoris_lora-1.8.0.dev4/lycoris/
+-rw-rw-rw-   0        0        0        0 2023-07-01 11:57:57.000000 lycoris_lora-1.8.0.dev4/lycoris/__init__.py
+-rw-rw-rw-   0        0        0    20963 2023-06-04 13:36:43.000000 lycoris_lora-1.8.0.dev4/lycoris/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-01 11:58:09.218056 lycoris_lora-1.8.0.dev4/lycoris_lora.egg-info/
+-rw-rw-rw-   0        0        0      353 2023-07-01 11:58:09.000000 lycoris_lora-1.8.0.dev4/lycoris_lora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-07-01 11:58:09.000000 lycoris_lora-1.8.0.dev4/lycoris_lora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 11:58:09.000000 lycoris_lora-1.8.0.dev4/lycoris_lora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-04 13:39:16.000000 lycoris_lora-1.8.0.dev4/lycoris_lora.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-07-01 11:58:09.000000 lycoris_lora-1.8.0.dev4/lycoris_lora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-01 11:58:09.000000 lycoris_lora-1.8.0.dev4/lycoris_lora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 11:58:09.219053 lycoris_lora-1.8.0.dev4/setup.cfg
+-rw-rw-rw-   0        0        0      547 2023-07-01 11:58:02.000000 lycoris_lora-1.8.0.dev4/setup.py
```

### Comparing `lycoris_lora-1.8.0.dev3/LICENSE.md` & `lycoris_lora-1.8.0.dev4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev3/README.md` & `lycoris_lora-1.8.0.dev4/README.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev3/lycoris/utils.py` & `lycoris_lora-1.8.0.dev4/lycoris/utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev3/setup.py` & `lycoris_lora-1.8.0.dev4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='lycoris_lora',
     packages=['lycoris'],
-    version='1.8.0.dev3',
+    version='1.8.0.dev4',
     url='https://github.com/KohakuBlueleaf/LyCORIS',
     description='Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion',
     author='Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao',
     author_email='apolloyeh0123@gmail.com',
     zip_safe=False,
     install_requires=[
         'torch',
```

