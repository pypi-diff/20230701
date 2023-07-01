# Comparing `tmp/nanorequests-0.2.tar.gz` & `tmp/nanorequests-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanorequests-0.2.tar", last modified: Sat Jul  1 06:22:40 2023, max compression
+gzip compressed data, was "nanorequests-0.3.tar", last modified: Sat Jul  1 06:52:27 2023, max compression
```

## Comparing `nanorequests-0.2.tar` & `nanorequests-0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 06:22:40.081094 nanorequests-0.2/
--rw-r--r--   0 viral      (501) staff       (20)     1070 2023-06-26 15:52:46.000000 nanorequests-0.2/LICENSE.txt
--rw-r--r--   0 viral      (501) staff       (20)      356 2023-07-01 06:22:40.081159 nanorequests-0.2/PKG-INFO
--rw-r--r--   0 viral      (501) staff       (20)      136 2023-06-26 15:52:46.000000 nanorequests-0.2/README.md
-drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 06:22:40.080502 nanorequests-0.2/nanorequests.egg-info/
--rw-r--r--   0 viral      (501) staff       (20)      356 2023-07-01 06:22:40.000000 nanorequests-0.2/nanorequests.egg-info/PKG-INFO
--rw-r--r--   0 viral      (501) staff       (20)      251 2023-07-01 06:22:40.000000 nanorequests-0.2/nanorequests.egg-info/SOURCES.txt
--rw-r--r--   0 viral      (501) staff       (20)        1 2023-07-01 06:22:40.000000 nanorequests-0.2/nanorequests.egg-info/dependency_links.txt
--rw-r--r--   0 viral      (501) staff       (20)        9 2023-07-01 06:22:40.000000 nanorequests-0.2/nanorequests.egg-info/requires.txt
--rw-r--r--   0 viral      (501) staff       (20)        6 2023-07-01 06:22:40.000000 nanorequests-0.2/nanorequests.egg-info/top_level.txt
--rw-r--r--   0 viral      (501) staff       (20)      107 2023-07-01 06:22:40.081404 nanorequests-0.2/setup.cfg
--rw-r--r--   0 viral      (501) staff       (20)      460 2023-07-01 06:01:04.000000 nanorequests-0.2/setup.py
-drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 06:22:40.080692 nanorequests-0.2/tests/
--rw-r--r--   0 viral      (501) staff       (20)        0 2023-07-01 05:12:27.000000 nanorequests-0.2/tests/__init__.py
--rw-r--r--   0 viral      (501) staff       (20)     3180 2023-07-01 06:03:28.000000 nanorequests-0.2/tests/main.py
+drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 06:52:27.004095 nanorequests-0.3/
+-rw-r--r--   0 viral      (501) staff       (20)     1070 2023-06-26 15:52:46.000000 nanorequests-0.3/LICENSE.txt
+-rw-r--r--   0 viral      (501) staff       (20)      356 2023-07-01 06:52:27.004170 nanorequests-0.3/PKG-INFO
+-rw-r--r--   0 viral      (501) staff       (20)      136 2023-06-26 15:52:46.000000 nanorequests-0.3/README.md
+drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 06:52:27.003644 nanorequests-0.3/nanorequests.egg-info/
+-rw-r--r--   0 viral      (501) staff       (20)      356 2023-07-01 06:52:26.000000 nanorequests-0.3/nanorequests.egg-info/PKG-INFO
+-rw-r--r--   0 viral      (501) staff       (20)      267 2023-07-01 06:52:26.000000 nanorequests-0.3/nanorequests.egg-info/SOURCES.txt
+-rw-r--r--   0 viral      (501) staff       (20)        1 2023-07-01 06:52:26.000000 nanorequests-0.3/nanorequests.egg-info/dependency_links.txt
+-rw-r--r--   0 viral      (501) staff       (20)        9 2023-07-01 06:52:26.000000 nanorequests-0.3/nanorequests.egg-info/requires.txt
+-rw-r--r--   0 viral      (501) staff       (20)       13 2023-07-01 06:52:26.000000 nanorequests-0.3/nanorequests.egg-info/top_level.txt
+-rw-r--r--   0 viral      (501) staff       (20)     3844 2023-07-01 06:03:28.000000 nanorequests-0.3/nanorequests.py
+-rw-r--r--   0 viral      (501) staff       (20)      107 2023-07-01 06:52:27.004463 nanorequests-0.3/setup.cfg
+-rw-r--r--   0 viral      (501) staff       (20)      463 2023-07-01 06:52:07.000000 nanorequests-0.3/setup.py
+drwxr-xr-x   0 viral      (501) staff       (20)        0 2023-07-01 06:52:27.003834 nanorequests-0.3/tests/
+-rw-r--r--   0 viral      (501) staff       (20)        0 2023-07-01 05:12:27.000000 nanorequests-0.3/tests/__init__.py
+-rw-r--r--   0 viral      (501) staff       (20)     3180 2023-07-01 06:03:28.000000 nanorequests-0.3/tests/main.py
```

### Comparing `nanorequests-0.2/LICENSE.txt` & `nanorequests-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nanorequests-0.2/tests/main.py` & `nanorequests-0.3/tests/main.py`

 * *Files identical despite different names*

