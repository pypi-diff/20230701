# Comparing `tmp/dark-gateway-0.0.1b0.tar.gz` & `tmp/dark-gateway-0.0.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dark-gateway-0.0.1b0.tar", last modified: Sat Jul  1 14:24:08 2023, max compression
+gzip compressed data, was "dark-gateway-0.0.1rc0.tar", last modified: Sat Jul  1 14:41:01 2023, max compression
```

## Comparing `dark-gateway-0.0.1b0.tar` & `dark-gateway-0.0.1rc0.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:08.165066 dark-gateway-0.0.1b0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 14:24:00.000000 dark-gateway-0.0.1b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-01 14:24:08.165066 dark-gateway-0.0.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 14:24:00.000000 dark-gateway-0.0.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:08.165066 dark-gateway-0.0.1b0/dark_gateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-01 14:24:08.000000 dark-gateway-0.0.1b0/dark_gateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-01 14:24:08.000000 dark-gateway-0.0.1b0/dark_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 14:24:08.000000 dark-gateway-0.0.1b0/dark_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-01 14:24:08.000000 dark-gateway-0.0.1b0/dark_gateway.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 14:24:08.165066 dark-gateway-0.0.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-01 14:24:06.000000 dark-gateway-0.0.1b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:08.165066 dark-gateway-0.0.1b0/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 14:24:00.000000 dark-gateway-0.0.1b0/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-07-01 14:24:00.000000 dark-gateway-0.0.1b0/util/libs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13540 2023-07-01 14:24:00.000000 dark-gateway-0.0.1b0/util/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:41:01.017794 dark-gateway-0.0.1rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 14:40:58.000000 dark-gateway-0.0.1rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-01 14:41:01.017794 dark-gateway-0.0.1rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 14:40:58.000000 dark-gateway-0.0.1rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:41:01.017794 dark-gateway-0.0.1rc0/dark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 14:40:58.000000 dark-gateway-0.0.1rc0/dark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:41:01.017794 dark-gateway-0.0.1rc0/dark/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-01 14:40:58.000000 dark-gateway-0.0.1rc0/dark/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-01 14:40:58.000000 dark-gateway-0.0.1rc0/dark/gateway/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:41:01.017794 dark-gateway-0.0.1rc0/dark/gateway/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 14:40:58.000000 dark-gateway-0.0.1rc0/dark/gateway/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-07-01 14:40:58.000000 dark-gateway-0.0.1rc0/dark/gateway/util/libs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13540 2023-07-01 14:40:58.000000 dark-gateway-0.0.1rc0/dark/gateway/util/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:41:01.017794 dark-gateway-0.0.1rc0/dark_gateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-01 14:41:00.000000 dark-gateway-0.0.1rc0/dark_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-01 14:41:01.000000 dark-gateway-0.0.1rc0/dark_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 14:41:00.000000 dark-gateway-0.0.1rc0/dark_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-01 14:41:00.000000 dark-gateway-0.0.1rc0/dark_gateway.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 14:41:01.017794 dark-gateway-0.0.1rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-01 14:41:00.000000 dark-gateway-0.0.1rc0/setup.py
```

### Comparing `dark-gateway-0.0.1b0/LICENSE` & `dark-gateway-0.0.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dark-gateway-0.0.1b0/setup.py` & `dark-gateway-0.0.1rc0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 local = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(local, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 
 # This gets deployed when a new release is made by github actions
-VERSION = '0.0.1b'
+VERSION = '0.0.1c'
 # VERSION = '0.0.1'
 
 # CHANGEME VARS
 PACKAGE_NAME = "dark-gateway"
 DESCRIPTION = 'dARK Gateway libs'
 LONG_DESCRIPTION = 'dARK web3 libs to connect applications to the dARK'
 AUTHOR_NAME = "Thiago Nóbrega"
```

### Comparing `dark-gateway-0.0.1b0/util/libs.py` & `dark-gateway-0.0.1rc0/dark/gateway/util/libs.py`

 * *Files identical despite different names*

### Comparing `dark-gateway-0.0.1b0/util/setup.py` & `dark-gateway-0.0.1rc0/dark/gateway/util/setup.py`

 * *Files identical despite different names*

