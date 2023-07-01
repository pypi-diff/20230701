# Comparing `tmp/tissue-tag-0.1.0.tar.gz` & `tmp/tissue-tag-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tissue-tag-0.1.0.tar", last modified: Fri Jun 30 14:29:06 2023, max compression
+gzip compressed data, was "tissue-tag-0.1.1.tar", last modified: Sat Jul  1 11:43:47 2023, max compression
```

## Comparing `tissue-tag-0.1.0.tar` & `tissue-tag-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 amsalem   (1000) amsalem   (1000)        0 2023-06-30 14:29:06.153731 tissue-tag-0.1.0/
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     1497 2023-06-30 14:25:56.000000 tissue-tag-0.1.0/LICENSE
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)      336 2023-06-30 14:29:06.153731 tissue-tag-0.1.0/PKG-INFO
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     1721 2023-06-30 14:25:56.000000 tissue-tag-0.1.0/README.md
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)       38 2023-06-30 14:29:06.157731 tissue-tag-0.1.0/setup.cfg
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)      616 2023-06-30 14:28:17.000000 tissue-tag-0.1.0/setup.py
-drwxrwxr-x   0 amsalem   (1000) amsalem   (1000)        0 2023-06-30 14:29:06.153731 tissue-tag-0.1.0/tissue_tag.egg-info/
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)      336 2023-06-30 14:29:06.000000 tissue-tag-0.1.0/tissue_tag.egg-info/PKG-INFO
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)      195 2023-06-30 14:29:06.000000 tissue-tag-0.1.0/tissue_tag.egg-info/SOURCES.txt
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)        1 2023-06-30 14:29:06.000000 tissue-tag-0.1.0/tissue_tag.egg-info/dependency_links.txt
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)       67 2023-06-30 14:29:06.000000 tissue-tag-0.1.0/tissue_tag.egg-info/requires.txt
--rw-rw-r--   0 amsalem   (1000) amsalem   (1000)        1 2023-06-30 14:29:06.000000 tissue-tag-0.1.0/tissue_tag.egg-info/top_level.txt
+drwxrwxr-x   0 amsalem   (1000) amsalem   (1000)        0 2023-07-01 11:43:47.315556 tissue-tag-0.1.1/
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     1497 2023-06-30 14:25:56.000000 tissue-tag-0.1.1/LICENSE
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     2105 2023-07-01 11:43:47.315556 tissue-tag-0.1.1/PKG-INFO
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     1721 2023-06-30 14:25:56.000000 tissue-tag-0.1.1/README.md
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)       38 2023-07-01 11:43:47.315556 tissue-tag-0.1.1/setup.cfg
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)      812 2023-07-01 11:43:23.000000 tissue-tag-0.1.1/setup.py
+drwxrwxr-x   0 amsalem   (1000) amsalem   (1000)        0 2023-07-01 11:43:47.315556 tissue-tag-0.1.1/tissue_tag.egg-info/
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)     2105 2023-07-01 11:43:47.000000 tissue-tag-0.1.1/tissue_tag.egg-info/PKG-INFO
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)      195 2023-07-01 11:43:47.000000 tissue-tag-0.1.1/tissue_tag.egg-info/SOURCES.txt
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)        1 2023-07-01 11:43:47.000000 tissue-tag-0.1.1/tissue_tag.egg-info/dependency_links.txt
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)       83 2023-07-01 11:43:47.000000 tissue-tag-0.1.1/tissue_tag.egg-info/requires.txt
+-rw-rw-r--   0 amsalem   (1000) amsalem   (1000)        1 2023-07-01 11:43:47.000000 tissue-tag-0.1.1/tissue_tag.egg-info/top_level.txt
```

### Comparing `tissue-tag-0.1.0/LICENSE` & `tissue-tag-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tissue-tag-0.1.0/README.md` & `tissue-tag-0.1.1/README.md`

 * *Files identical despite different names*

