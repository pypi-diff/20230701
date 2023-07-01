# Comparing `tmp/gptconsole-0.5.tar.gz` & `tmp/gptconsole-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptconsole-0.5.tar", last modified: Sat Jul  1 03:39:26 2023, max compression
+gzip compressed data, was "gptconsole-0.7.tar", last modified: Sat Jul  1 03:47:21 2023, max compression
```

## Comparing `gptconsole-0.5.tar` & `gptconsole-0.7.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2023-07-01 03:39:26.878818 gptconsole-0.5/
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)    18092 2023-06-29 01:49:35.000000 gptconsole-0.5/LICENSE
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      226 2023-07-01 03:39:26.878818 gptconsole-0.5/PKG-INFO
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      687 2023-06-29 03:19:48.000000 gptconsole-0.5/README.md
-drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2023-07-01 03:39:26.878818 gptconsole-0.5/gptconsole.egg-info/
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      226 2023-07-01 03:39:26.000000 gptconsole-0.5/gptconsole.egg-info/PKG-INFO
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      199 2023-07-01 03:39:26.000000 gptconsole-0.5/gptconsole.egg-info/SOURCES.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)        1 2023-07-01 03:39:26.000000 gptconsole-0.5/gptconsole.egg-info/dependency_links.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)       45 2023-07-01 03:39:26.000000 gptconsole-0.5/gptconsole.egg-info/entry_points.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)        5 2023-07-01 03:39:26.000000 gptconsole-0.5/gptconsole.egg-info/top_level.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)       38 2023-07-01 03:39:26.878818 gptconsole-0.5/setup.cfg
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      388 2023-07-01 03:39:21.000000 gptconsole-0.5/setup.py
+drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2023-07-01 03:47:21.575505 gptconsole-0.7/
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)    18092 2023-06-29 01:49:35.000000 gptconsole-0.7/LICENSE
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      226 2023-07-01 03:47:21.575505 gptconsole-0.7/PKG-INFO
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      687 2023-06-29 03:19:48.000000 gptconsole-0.7/README.md
+drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2023-07-01 03:47:21.575505 gptconsole-0.7/gptconsole.egg-info/
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      226 2023-07-01 03:47:21.000000 gptconsole-0.7/gptconsole.egg-info/PKG-INFO
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      213 2023-07-01 03:47:21.000000 gptconsole-0.7/gptconsole.egg-info/SOURCES.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)        1 2023-07-01 03:47:21.000000 gptconsole-0.7/gptconsole.egg-info/dependency_links.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)       40 2023-07-01 03:47:21.000000 gptconsole-0.7/gptconsole.egg-info/entry_points.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)       11 2023-07-01 03:47:21.000000 gptconsole-0.7/gptconsole.egg-info/top_level.txt
+-rwxr-xr-x   0 john_vm   (1000) john_vm   (1000)     9176 2023-07-01 03:36:39.000000 gptconsole-0.7/gptconsole.py
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)       38 2023-07-01 03:47:21.575505 gptconsole-0.7/setup.cfg
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      389 2023-07-01 03:47:04.000000 gptconsole-0.7/setup.py
```

### Comparing `gptconsole-0.5/LICENSE` & `gptconsole-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gptconsole-0.5/README.md` & `gptconsole-0.7/README.md`

 * *Files identical despite different names*

