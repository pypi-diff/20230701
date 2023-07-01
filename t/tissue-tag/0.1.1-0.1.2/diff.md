# Comparing `tmp/tissue-tag-0.1.1.tar.gz` & `tmp/tissue-tag-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tissue-tag-0.1.1.tar", last modified: Sat Jul  1 11:43:47 2023, max compression
+gzip compressed data, was "tissue-tag-0.1.2.tar", last modified: Sat Jul  1 12:01:01 2023, max compression
```

## Comparing `tissue-tag-0.1.1.tar` & `tissue-tag-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 amsalem   (1000) amsalem   (1000)        0 2023-07-01 11:43:47.315556 tissue-tag-0.1.1/
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     1497 2023-06-30 14:25:56.000000 tissue-tag-0.1.1/LICENSE
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     2105 2023-07-01 11:43:47.315556 tissue-tag-0.1.1/PKG-INFO
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     1721 2023-06-30 14:25:56.000000 tissue-tag-0.1.1/README.md
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)       38 2023-07-01 11:43:47.315556 tissue-tag-0.1.1/setup.cfg
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)      812 2023-07-01 11:43:23.000000 tissue-tag-0.1.1/setup.py
-drwxrwxr-x   0 amsalem   (1000) amsalem   (1000)        0 2023-07-01 11:43:47.315556 tissue-tag-0.1.1/tissue_tag.egg-info/
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     2105 2023-07-01 11:43:47.000000 tissue-tag-0.1.1/tissue_tag.egg-info/PKG-INFO
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)      195 2023-07-01 11:43:47.000000 tissue-tag-0.1.1/tissue_tag.egg-info/SOURCES.txt
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)        1 2023-07-01 11:43:47.000000 tissue-tag-0.1.1/tissue_tag.egg-info/dependency_links.txt
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)       83 2023-07-01 11:43:47.000000 tissue-tag-0.1.1/tissue_tag.egg-info/requires.txt
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)        1 2023-07-01 11:43:47.000000 tissue-tag-0.1.1/tissue_tag.egg-info/top_level.txt
+drwxrwxr-x   0 amsalem   (1000) amsalem   (1000)        0 2023-07-01 12:01:01.612068 tissue-tag-0.1.2/
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     1497 2023-06-30 14:25:56.000000 tissue-tag-0.1.2/LICENSE
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     1034 2023-07-01 12:01:01.612068 tissue-tag-0.1.2/PKG-INFO
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)      650 2023-07-01 12:00:11.000000 tissue-tag-0.1.2/README.md
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)       38 2023-07-01 12:01:01.612068 tissue-tag-0.1.2/setup.cfg
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)      813 2023-07-01 11:59:22.000000 tissue-tag-0.1.2/setup.py
+drwxrwxr-x   0 amsalem   (1000) amsalem   (1000)        0 2023-07-01 12:01:01.612068 tissue-tag-0.1.2/tissue_tag.egg-info/
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     1034 2023-07-01 12:01:01.000000 tissue-tag-0.1.2/tissue_tag.egg-info/PKG-INFO
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)      195 2023-07-01 12:01:01.000000 tissue-tag-0.1.2/tissue_tag.egg-info/SOURCES.txt
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)        1 2023-07-01 12:01:01.000000 tissue-tag-0.1.2/tissue_tag.egg-info/dependency_links.txt
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)       84 2023-07-01 12:01:01.000000 tissue-tag-0.1.2/tissue_tag.egg-info/requires.txt
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)        1 2023-07-01 12:01:01.000000 tissue-tag-0.1.2/tissue_tag.egg-info/top_level.txt
```

### Comparing `tissue-tag-0.1.1/LICENSE` & `tissue-tag-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tissue-tag-0.1.1/setup.py` & `tissue-tag-0.1.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='tissue-tag',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     install_requires=[
-        'opencv-python'
+        'opencv-python',
         'Pillow',
         'bokeh',
         'jupyter-bokeh',
         'matplotlib',
         'seaborn',
         'scipy',
         'scikit-image',
```

