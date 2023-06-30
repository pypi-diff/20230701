# Comparing `tmp/summo-0.0.1.tar.gz` & `tmp/summo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "summo-0.0.1.tar", last modified: Thu Jun 29 03:44:17 2023, max compression
+gzip compressed data, was "summo-0.0.2.tar", last modified: Fri Jun 30 23:28:18 2023, max compression
```

## Comparing `summo-0.0.1.tar` & `summo-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-29 03:44:17.126051 summo-0.0.1/
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)        0 2023-06-29 03:20:24.000000 summo-0.0.1/LICENSE
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      212 2023-06-29 03:44:17.126051 summo-0.0.1/PKG-INFO
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)       39 2023-06-29 03:43:34.000000 summo-0.0.1/README.md
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      331 2023-06-29 03:20:24.000000 summo-0.0.1/pyproject.toml
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)       38 2023-06-29 03:44:17.126051 summo-0.0.1/setup.cfg
-drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-29 03:44:17.126051 summo-0.0.1/src/
-drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-29 03:44:17.126051 summo-0.0.1/src/summo/
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      140 2023-06-29 03:33:27.000000 summo-0.0.1/src/summo/__init__.py
-drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-29 03:44:17.126051 summo-0.0.1/src/summo.egg-info/
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      212 2023-06-29 03:44:17.000000 summo-0.0.1/src/summo.egg-info/PKG-INFO
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      186 2023-06-29 03:44:17.000000 summo-0.0.1/src/summo.egg-info/SOURCES.txt
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)        1 2023-06-29 03:44:17.000000 summo-0.0.1/src/summo.egg-info/dependency_links.txt
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)        6 2023-06-29 03:44:17.000000 summo-0.0.1/src/summo.egg-info/top_level.txt
+drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-30 23:28:18.217963 summo-0.0.2/
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)     1071 2023-06-29 18:44:42.000000 summo-0.0.2/LICENSE
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      417 2023-06-30 23:28:18.217963 summo-0.0.2/PKG-INFO
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      202 2023-06-29 21:36:53.000000 summo-0.0.2/README.md
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      605 2023-06-30 23:28:10.000000 summo-0.0.2/pyproject.toml
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)       38 2023-06-30 23:28:18.217963 summo-0.0.2/setup.cfg
+drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-30 23:28:18.217963 summo-0.0.2/src/
+drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-30 23:28:18.217963 summo-0.0.2/src/summo/
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)       34 2023-06-30 17:04:57.000000 summo-0.0.2/src/summo/__init__.py
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      611 2023-06-30 18:08:00.000000 summo-0.0.2/src/summo/summary.py
+drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-30 23:28:18.217963 summo-0.0.2/src/summo.egg-info/
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      417 2023-06-30 23:28:18.000000 summo-0.0.2/src/summo.egg-info/PKG-INFO
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      261 2023-06-30 23:28:18.000000 summo-0.0.2/src/summo.egg-info/SOURCES.txt
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)        1 2023-06-30 23:28:18.000000 summo-0.0.2/src/summo.egg-info/dependency_links.txt
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)       34 2023-06-30 23:28:18.000000 summo-0.0.2/src/summo.egg-info/requires.txt
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)        6 2023-06-30 23:28:18.000000 summo-0.0.2/src/summo.egg-info/top_level.txt
+drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-30 23:28:18.217963 summo-0.0.2/tests/
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)     1233 2023-06-30 18:09:22.000000 summo-0.0.2/tests/test_summary.py
```

