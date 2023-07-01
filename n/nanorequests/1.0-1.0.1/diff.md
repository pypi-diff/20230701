# Comparing `tmp/nanorequests-1.0.tar.gz` & `tmp/nanorequests-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanorequests-1.0.tar", last modified: Sat Jul  1 07:53:57 2023, max compression
+gzip compressed data, was "nanorequests-1.0.1.tar", last modified: Sat Jul  1 08:52:23 2023, max compression
```

## Comparing `nanorequests-1.0.tar` & `nanorequests-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 07:53:57.407052 nanorequests-1.0/
--rw-r--r--   0 viral      (501) staff       (20)     1070 2023-06-26 15:52:46.000000 nanorequests-1.0/LICENSE.txt
--rw-r--r--   0 viral      (501) staff       (20)      518 2023-07-01 07:53:57.407113 nanorequests-1.0/PKG-INFO
--rw-r--r--   0 viral      (501) staff       (20)      129 2023-07-01 07:48:19.000000 nanorequests-1.0/README.md
-drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 07:53:57.405921 nanorequests-1.0/nanorequests/
--rw-r--r--   0 viral      (501) staff       (20)     3862 2023-07-01 07:51:39.000000 nanorequests-1.0/nanorequests/__init__.py
--rw-r--r--   0 viral      (501) staff       (20)     4164 2023-07-01 05:31:42.000000 nanorequests-1.0/nanorequests/nanoexceptions.py
-drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 07:53:57.406656 nanorequests-1.0/nanorequests.egg-info/
--rw-r--r--   0 viral      (501) staff       (20)      518 2023-07-01 07:53:57.000000 nanorequests-1.0/nanorequests.egg-info/PKG-INFO
--rw-r--r--   0 viral      (501) staff       (20)      307 2023-07-01 07:53:57.000000 nanorequests-1.0/nanorequests.egg-info/SOURCES.txt
--rw-r--r--   0 viral      (501) staff       (20)        1 2023-07-01 07:53:57.000000 nanorequests-1.0/nanorequests.egg-info/dependency_links.txt
--rw-r--r--   0 viral      (501) staff       (20)        9 2023-07-01 07:53:57.000000 nanorequests-1.0/nanorequests.egg-info/requires.txt
--rw-r--r--   0 viral      (501) staff       (20)       24 2023-07-01 07:53:57.000000 nanorequests-1.0/nanorequests.egg-info/top_level.txt
--rw-r--r--   0 viral      (501) staff       (20)      188 2023-07-01 07:53:57.407297 nanorequests-1.0/setup.cfg
--rw-r--r--   0 viral      (501) staff       (20)      492 2023-07-01 07:53:33.000000 nanorequests-1.0/setup.py
-drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 07:53:57.406832 nanorequests-1.0/tests/
--rw-r--r--   0 viral      (501) staff       (20)        0 2023-07-01 05:12:27.000000 nanorequests-1.0/tests/__init__.py
--rw-r--r--   0 viral      (501) staff       (20)     3197 2023-07-01 07:52:57.000000 nanorequests-1.0/tests/main.py
+drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 08:52:23.844569 nanorequests-1.0.1/
+-rw-r--r--   0 viral      (501) staff       (20)     1070 2023-07-01 08:51:01.000000 nanorequests-1.0.1/LICENSE.txt
+-rw-r--r--   0 viral      (501) staff       (20)     4187 2023-07-01 08:52:23.844626 nanorequests-1.0.1/PKG-INFO
+-rw-r--r--   0 viral      (501) staff       (20)     3796 2023-07-01 08:51:01.000000 nanorequests-1.0.1/README.md
+drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 08:52:23.843324 nanorequests-1.0.1/nanorequests/
+-rw-r--r--   0 viral      (501) staff       (20)     3862 2023-07-01 07:51:39.000000 nanorequests-1.0.1/nanorequests/__init__.py
+-rw-r--r--   0 viral      (501) staff       (20)     4164 2023-07-01 05:31:42.000000 nanorequests-1.0.1/nanorequests/nanoexceptions.py
+drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 08:52:23.844146 nanorequests-1.0.1/nanorequests.egg-info/
+-rw-r--r--   0 viral      (501) staff       (20)     4187 2023-07-01 08:52:23.000000 nanorequests-1.0.1/nanorequests.egg-info/PKG-INFO
+-rw-r--r--   0 viral      (501) staff       (20)      307 2023-07-01 08:52:23.000000 nanorequests-1.0.1/nanorequests.egg-info/SOURCES.txt
+-rw-r--r--   0 viral      (501) staff       (20)        1 2023-07-01 08:52:23.000000 nanorequests-1.0.1/nanorequests.egg-info/dependency_links.txt
+-rw-r--r--   0 viral      (501) staff       (20)        9 2023-07-01 08:52:23.000000 nanorequests-1.0.1/nanorequests.egg-info/requires.txt
+-rw-r--r--   0 viral      (501) staff       (20)       24 2023-07-01 08:52:23.000000 nanorequests-1.0.1/nanorequests.egg-info/top_level.txt
+-rw-r--r--   0 viral      (501) staff       (20)      188 2023-07-01 08:52:23.844818 nanorequests-1.0.1/setup.cfg
+-rw-r--r--   0 viral      (501) staff       (20)      494 2023-07-01 08:51:54.000000 nanorequests-1.0.1/setup.py
+drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 08:52:23.844362 nanorequests-1.0.1/tests/
+-rw-r--r--   0 viral      (501) staff       (20)        0 2023-07-01 05:12:27.000000 nanorequests-1.0.1/tests/__init__.py
+-rw-r--r--   0 viral      (501) staff       (20)     3197 2023-07-01 07:52:57.000000 nanorequests-1.0.1/tests/main.py
```

### Comparing `nanorequests-1.0/LICENSE.txt` & `nanorequests-1.0.1/LICENSE.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) [year] [fullname]
+Copyright (c) 2023 Viral Parmar
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `nanorequests-1.0/nanorequests/__init__.py` & `nanorequests-1.0.1/nanorequests/__init__.py`

 * *Files identical despite different names*

### Comparing `nanorequests-1.0/nanorequests/nanoexceptions.py` & `nanorequests-1.0.1/nanorequests/nanoexceptions.py`

 * *Files identical despite different names*

### Comparing `nanorequests-1.0/tests/main.py` & `nanorequests-1.0.1/tests/main.py`

 * *Files identical despite different names*

