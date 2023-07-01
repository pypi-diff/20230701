# Comparing `tmp/nanorequests-0.8.tar.gz` & `tmp/nanorequests-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanorequests-0.8.tar", last modified: Sat Jul  1 07:37:16 2023, max compression
+gzip compressed data, was "nanorequests-0.9.tar", last modified: Sat Jul  1 07:46:57 2023, max compression
```

## Comparing `nanorequests-0.8.tar` & `nanorequests-0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 07:37:16.601730 nanorequests-0.8/
--rw-r--r--   0 viral      (501) staff       (20)     1070 2023-06-26 15:52:46.000000 nanorequests-0.8/LICENSE.txt
--rw-r--r--   0 viral      (501) staff       (20)      356 2023-07-01 07:37:16.601869 nanorequests-0.8/PKG-INFO
--rw-r--r--   0 viral      (501) staff       (20)      136 2023-06-26 15:52:46.000000 nanorequests-0.8/README.md
-drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 07:37:16.600550 nanorequests-0.8/nanorequests/
--rw-r--r--   0 viral      (501) staff       (20)        0 2023-07-01 07:24:40.000000 nanorequests-0.8/nanorequests/__init__.py
--rw-r--r--   0 viral      (501) staff       (20)     4164 2023-07-01 05:31:42.000000 nanorequests-0.8/nanorequests/nanoexceptions.py
--rw-r--r--   0 viral      (501) staff       (20)     3862 2023-07-01 07:33:53.000000 nanorequests-0.8/nanorequests/nanorequests.py
-drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 07:37:16.601299 nanorequests-0.8/nanorequests.egg-info/
--rw-r--r--   0 viral      (501) staff       (20)      356 2023-07-01 07:37:16.000000 nanorequests-0.8/nanorequests.egg-info/PKG-INFO
--rw-r--r--   0 viral      (501) staff       (20)      336 2023-07-01 07:37:16.000000 nanorequests-0.8/nanorequests.egg-info/SOURCES.txt
--rw-r--r--   0 viral      (501) staff       (20)        1 2023-07-01 07:37:16.000000 nanorequests-0.8/nanorequests.egg-info/dependency_links.txt
--rw-r--r--   0 viral      (501) staff       (20)        9 2023-07-01 07:37:16.000000 nanorequests-0.8/nanorequests.egg-info/requires.txt
--rw-r--r--   0 viral      (501) staff       (20)       24 2023-07-01 07:37:16.000000 nanorequests-0.8/nanorequests.egg-info/top_level.txt
--rw-r--r--   0 viral      (501) staff       (20)      107 2023-07-01 07:37:16.602419 nanorequests-0.8/setup.cfg
--rw-r--r--   0 viral      (501) staff       (20)      508 2023-07-01 07:36:57.000000 nanorequests-0.8/setup.py
-drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 07:37:16.601507 nanorequests-0.8/tests/
--rw-r--r--   0 viral      (501) staff       (20)        0 2023-07-01 05:12:27.000000 nanorequests-0.8/tests/__init__.py
--rw-r--r--   0 viral      (501) staff       (20)     3223 2023-07-01 07:34:19.000000 nanorequests-0.8/tests/main.py
+drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 07:46:57.309786 nanorequests-0.9/
+-rw-r--r--   0 viral      (501) staff       (20)     1070 2023-06-26 15:52:46.000000 nanorequests-0.9/LICENSE.txt
+-rw-r--r--   0 viral      (501) staff       (20)      398 2023-07-01 07:46:57.309889 nanorequests-0.9/PKG-INFO
+-rw-r--r--   0 viral      (501) staff       (20)      136 2023-06-26 15:52:46.000000 nanorequests-0.9/README.md
+drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 07:46:57.308421 nanorequests-0.9/nanorequests/
+-rw-r--r--   0 viral      (501) staff       (20)       27 2023-07-01 07:42:39.000000 nanorequests-0.9/nanorequests/__init__.py
+-rw-r--r--   0 viral      (501) staff       (20)     4164 2023-07-01 05:31:42.000000 nanorequests-0.9/nanorequests/nanoexceptions.py
+-rw-r--r--   0 viral      (501) staff       (20)     3862 2023-07-01 07:33:53.000000 nanorequests-0.9/nanorequests/nanorequests.py
+drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 07:46:57.309324 nanorequests-0.9/nanorequests.egg-info/
+-rw-r--r--   0 viral      (501) staff       (20)      398 2023-07-01 07:46:57.000000 nanorequests-0.9/nanorequests.egg-info/PKG-INFO
+-rw-r--r--   0 viral      (501) staff       (20)      336 2023-07-01 07:46:57.000000 nanorequests-0.9/nanorequests.egg-info/SOURCES.txt
+-rw-r--r--   0 viral      (501) staff       (20)        1 2023-07-01 07:46:57.000000 nanorequests-0.9/nanorequests.egg-info/dependency_links.txt
+-rw-r--r--   0 viral      (501) staff       (20)        9 2023-07-01 07:46:57.000000 nanorequests-0.9/nanorequests.egg-info/requires.txt
+-rw-r--r--   0 viral      (501) staff       (20)       24 2023-07-01 07:46:57.000000 nanorequests-0.9/nanorequests.egg-info/top_level.txt
+-rw-r--r--   0 viral      (501) staff       (20)      107 2023-07-01 07:46:57.310180 nanorequests-0.9/setup.cfg
+-rw-r--r--   0 viral      (501) staff       (20)      593 2023-07-01 07:45:39.000000 nanorequests-0.9/setup.py
+drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 07:46:57.309530 nanorequests-0.9/tests/
+-rw-r--r--   0 viral      (501) staff       (20)        0 2023-07-01 05:12:27.000000 nanorequests-0.9/tests/__init__.py
+-rw-r--r--   0 viral      (501) staff       (20)     3223 2023-07-01 07:34:19.000000 nanorequests-0.9/tests/main.py
```

### Comparing `nanorequests-0.8/LICENSE.txt` & `nanorequests-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nanorequests-0.8/nanorequests/nanoexceptions.py` & `nanorequests-0.9/nanorequests/nanoexceptions.py`

 * *Files identical despite different names*

### Comparing `nanorequests-0.8/nanorequests/nanorequests.py` & `nanorequests-0.9/nanorequests/nanorequests.py`

 * *Files identical despite different names*

### Comparing `nanorequests-0.8/tests/main.py` & `nanorequests-0.9/tests/main.py`

 * *Files identical despite different names*

