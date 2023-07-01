# Comparing `tmp/gptconsole-0.1.tar.gz` & `tmp/gptconsole-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptconsole-0.1.tar", last modified: Sat Jul  1 03:07:28 2023, max compression
+gzip compressed data, was "gptconsole-0.2.tar", last modified: Sat Jul  1 03:22:35 2023, max compression
```

## Comparing `gptconsole-0.1.tar` & `gptconsole-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2023-07-01 03:07:28.418737 gptconsole-0.1/
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)    18092 2023-06-29 01:49:35.000000 gptconsole-0.1/LICENSE
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      226 2023-07-01 03:07:28.418737 gptconsole-0.1/PKG-INFO
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      687 2023-06-29 03:19:48.000000 gptconsole-0.1/README.md
-drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2023-07-01 03:07:28.418737 gptconsole-0.1/gptconsole.egg-info/
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      226 2023-07-01 03:07:28.000000 gptconsole-0.1/gptconsole.egg-info/PKG-INFO
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      199 2023-07-01 03:07:28.000000 gptconsole-0.1/gptconsole.egg-info/SOURCES.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)        1 2023-07-01 03:07:28.000000 gptconsole-0.1/gptconsole.egg-info/dependency_links.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)       44 2023-07-01 03:07:28.000000 gptconsole-0.1/gptconsole.egg-info/entry_points.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)       11 2023-07-01 03:07:28.000000 gptconsole-0.1/gptconsole.egg-info/top_level.txt
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)       38 2023-07-01 03:07:28.418737 gptconsole-0.1/setup.cfg
--rw-r--r--   0 john_vm   (1000) john_vm   (1000)      393 2023-07-01 03:07:10.000000 gptconsole-0.1/setup.py
+drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2023-07-01 03:22:35.888775 gptconsole-0.2/
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)    18092 2023-06-29 01:49:35.000000 gptconsole-0.2/LICENSE
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      226 2023-07-01 03:22:35.888775 gptconsole-0.2/PKG-INFO
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      687 2023-06-29 03:19:48.000000 gptconsole-0.2/README.md
+drwxr-xr-x   0 john_vm   (1000) john_vm   (1000)        0 2023-07-01 03:22:35.888775 gptconsole-0.2/gptconsole.egg-info/
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      226 2023-07-01 03:22:35.000000 gptconsole-0.2/gptconsole.egg-info/PKG-INFO
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      199 2023-07-01 03:22:35.000000 gptconsole-0.2/gptconsole.egg-info/SOURCES.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)        1 2023-07-01 03:22:35.000000 gptconsole-0.2/gptconsole.egg-info/dependency_links.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)       49 2023-07-01 03:22:35.000000 gptconsole-0.2/gptconsole.egg-info/entry_points.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)       11 2023-07-01 03:22:35.000000 gptconsole-0.2/gptconsole.egg-info/top_level.txt
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)       38 2023-07-01 03:22:35.888775 gptconsole-0.2/setup.cfg
+-rw-r--r--   0 john_vm   (1000) john_vm   (1000)      398 2023-07-01 03:22:00.000000 gptconsole-0.2/setup.py
```

### Comparing `gptconsole-0.1/LICENSE` & `gptconsole-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gptconsole-0.1/README.md` & `gptconsole-0.2/README.md`

 * *Files identical despite different names*

