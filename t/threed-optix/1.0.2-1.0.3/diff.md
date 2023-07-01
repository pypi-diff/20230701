# Comparing `tmp/threed_optix-1.0.2.tar.gz` & `tmp/threed_optix-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threed_optix-1.0.2.tar", last modified: Sat Jul  1 09:29:36 2023, max compression
+gzip compressed data, was "threed_optix-1.0.3.tar", last modified: Sat Jul  1 10:07:14 2023, max compression
```

## Comparing `threed_optix-1.0.2.tar` & `threed_optix-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-01 09:29:36.458083 threed_optix-1.0.2/
--rw-rw-r--   0 elika     (1000) elika     (1000)      166 2023-07-01 09:29:36.458083 threed_optix-1.0.2/PKG-INFO
--rw-rw-r--   0 elika     (1000) elika     (1000)        0 2023-06-29 16:13:36.000000 threed_optix-1.0.2/README.rst
--rw-rw-r--   0 elika     (1000) elika     (1000)      107 2023-07-01 09:29:36.458083 threed_optix-1.0.2/setup.cfg
--rw-rw-r--   0 elika     (1000) elika     (1000)      386 2023-07-01 09:17:23.000000 threed_optix-1.0.2/setup.py
-drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-01 09:29:36.458083 threed_optix-1.0.2/src/
-drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-01 09:29:36.458083 threed_optix-1.0.2/src/threed_optix/
--rw-rw-r--   0 elika     (1000) elika     (1000)       22 2023-06-26 17:19:19.000000 threed_optix-1.0.2/src/threed_optix/__init__.py
--rw-rw-r--   0 elika     (1000) elika     (1000)     5755 2023-06-30 12:46:37.000000 threed_optix-1.0.2/src/threed_optix/api.py
-drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-01 09:29:36.458083 threed_optix-1.0.2/src/threed_optix/examples/
--rw-rw-r--   0 elika     (1000) elika     (1000)        0 2023-06-24 18:01:59.000000 threed_optix-1.0.2/src/threed_optix/examples/__init__.py
--rw-rw-r--   0 elika     (1000) elika     (1000)     1017 2023-07-01 09:12:49.000000 threed_optix-1.0.2/src/threed_optix/examples/example_0.py
--rwxrwxr-x   0 elika     (1000) elika     (1000)      813 2023-07-01 09:12:49.000000 threed_optix-1.0.2/src/threed_optix/examples/simple.py
-drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-01 09:29:36.458083 threed_optix-1.0.2/src/threed_optix.egg-info/
--rw-rw-r--   0 elika     (1000) elika     (1000)      166 2023-07-01 09:29:36.000000 threed_optix-1.0.2/src/threed_optix.egg-info/PKG-INFO
--rw-rw-r--   0 elika     (1000) elika     (1000)      394 2023-07-01 09:29:36.000000 threed_optix-1.0.2/src/threed_optix.egg-info/SOURCES.txt
--rw-rw-r--   0 elika     (1000) elika     (1000)        1 2023-07-01 09:29:36.000000 threed_optix-1.0.2/src/threed_optix.egg-info/dependency_links.txt
--rw-rw-r--   0 elika     (1000) elika     (1000)       16 2023-07-01 09:29:36.000000 threed_optix-1.0.2/src/threed_optix.egg-info/requires.txt
--rw-rw-r--   0 elika     (1000) elika     (1000)       13 2023-07-01 09:29:36.000000 threed_optix-1.0.2/src/threed_optix.egg-info/top_level.txt
+drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-01 10:07:14.933181 threed_optix-1.0.3/
+-rw-rw-r--   0 elika     (1000) elika     (1000)      166 2023-07-01 10:07:14.933181 threed_optix-1.0.3/PKG-INFO
+-rw-rw-r--   0 elika     (1000) elika     (1000)        0 2023-06-29 16:13:36.000000 threed_optix-1.0.3/README.rst
+-rw-rw-r--   0 elika     (1000) elika     (1000)      107 2023-07-01 10:07:14.933181 threed_optix-1.0.3/setup.cfg
+-rw-rw-r--   0 elika     (1000) elika     (1000)      408 2023-07-01 10:07:00.000000 threed_optix-1.0.3/setup.py
+drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-01 10:07:14.933181 threed_optix-1.0.3/src/
+drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-01 10:07:14.933181 threed_optix-1.0.3/src/threed_optix/
+-rw-rw-r--   0 elika     (1000) elika     (1000)       22 2023-06-26 17:19:19.000000 threed_optix-1.0.3/src/threed_optix/__init__.py
+-rw-rw-r--   0 elika     (1000) elika     (1000)     5755 2023-06-30 12:46:37.000000 threed_optix-1.0.3/src/threed_optix/api.py
+drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-01 10:07:14.933181 threed_optix-1.0.3/src/threed_optix/examples/
+-rw-rw-r--   0 elika     (1000) elika     (1000)        0 2023-06-24 18:01:59.000000 threed_optix-1.0.3/src/threed_optix/examples/__init__.py
+-rw-rw-r--   0 elika     (1000) elika     (1000)     1017 2023-07-01 09:12:49.000000 threed_optix-1.0.3/src/threed_optix/examples/example_0.py
+-rwxrwxr-x   0 elika     (1000) elika     (1000)      813 2023-07-01 09:12:49.000000 threed_optix-1.0.3/src/threed_optix/examples/simple.py
+drwxrwxr-x   0 elika     (1000) elika     (1000)        0 2023-07-01 10:07:14.933181 threed_optix-1.0.3/src/threed_optix.egg-info/
+-rw-rw-r--   0 elika     (1000) elika     (1000)      166 2023-07-01 10:07:14.000000 threed_optix-1.0.3/src/threed_optix.egg-info/PKG-INFO
+-rw-rw-r--   0 elika     (1000) elika     (1000)      394 2023-07-01 10:07:14.000000 threed_optix-1.0.3/src/threed_optix.egg-info/SOURCES.txt
+-rw-rw-r--   0 elika     (1000) elika     (1000)        1 2023-07-01 10:07:14.000000 threed_optix-1.0.3/src/threed_optix.egg-info/dependency_links.txt
+-rw-rw-r--   0 elika     (1000) elika     (1000)       27 2023-07-01 10:07:14.000000 threed_optix-1.0.3/src/threed_optix.egg-info/requires.txt
+-rw-rw-r--   0 elika     (1000) elika     (1000)       13 2023-07-01 10:07:14.000000 threed_optix-1.0.3/src/threed_optix.egg-info/top_level.txt
```

### Comparing `threed_optix-1.0.2/src/threed_optix/api.py` & `threed_optix-1.0.3/src/threed_optix/api.py`

 * *Files identical despite different names*

### Comparing `threed_optix-1.0.2/src/threed_optix/examples/example_0.py` & `threed_optix-1.0.3/src/threed_optix/examples/example_0.py`

 * *Files identical despite different names*

### Comparing `threed_optix-1.0.2/src/threed_optix/examples/simple.py` & `threed_optix-1.0.3/src/threed_optix/examples/simple.py`

 * *Files identical despite different names*

