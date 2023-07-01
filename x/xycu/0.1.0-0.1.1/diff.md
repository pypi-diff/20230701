# Comparing `tmp/xycu-0.1.0.tar.gz` & `tmp/xycu-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xycu-0.1.0.tar", max compression
+gzip compressed data, was "xycu-0.1.1.tar", max compression
```

## Comparing `xycu-0.1.0.tar` & `xycu-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1086 2023-07-01 17:03:03.878769 xycu-0.1.0/LICENSE
--rw-r--r--   0        0        0      519 2023-07-01 19:09:23.615651 xycu-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        6 2023-07-01 17:02:57.856184 xycu-0.1.0/README.md
--rw-r--r--   0        0        0      272 2023-07-01 19:07:33.238896 xycu-0.1.0/src/xycu/__init__.py
--rw-r--r--   0        0        0      491 2023-07-01 19:18:53.252663 xycu-0.1.0/src/xycu/clients.py
--rw-r--r--   0        0        0       19 2023-07-01 19:10:19.351552 xycu-0.1.0/src/xycu/managers/__init__.py
--rw-r--r--   0        0        0      494 2023-07-01 19:23:15.032817 xycu-0.1.0/src/xycu/managers/nsfw.py
--rw-r--r--   0        0        0      485 2023-07-01 19:23:22.239378 xycu-0.1.0/src/xycu/managers/sfw.py
--rw-r--r--   0        0        0       19 2023-07-01 19:04:08.843430 xycu-0.1.0/src/xycu/models/__init__.py
--rw-r--r--   0        0        0       19 2023-07-01 19:09:52.336652 xycu-0.1.0/src/xycu/models/enums/__init__.py
--rw-r--r--   0        0        0       19 2023-07-01 19:10:09.772425 xycu-0.1.0/src/xycu/models/enums/categories/__init__.py
--rw-r--r--   0        0        0      211 2023-07-01 19:10:02.374449 xycu-0.1.0/src/xycu/models/enums/categories/nsfw.py
--rw-r--r--   0        0        0      755 2023-07-01 19:14:46.560219 xycu-0.1.0/src/xycu/models/enums/categories/sfw.py
--rw-r--r--   0        0        0      103 2023-07-01 19:13:02.936202 xycu-0.1.0/src/xycu/models/images.py
--rw-r--r--   0        0        0      633 1970-01-01 00:00:00.000000 xycu-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-07-01 17:03:03.878769 xycu-0.1.1/LICENSE
+-rw-r--r--   0        0        0      876 2023-07-01 19:55:40.591410 xycu-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      721 2023-07-01 19:54:10.975278 xycu-0.1.1/README.md
+-rw-r--r--   0        0        0      304 2023-07-01 19:37:51.695752 xycu-0.1.1/src/xycu/__init__.py
+-rw-r--r--   0        0        0      491 2023-07-01 19:18:53.252663 xycu-0.1.1/src/xycu/clients.py
+-rw-r--r--   0        0        0       19 2023-07-01 19:10:19.351552 xycu-0.1.1/src/xycu/managers/__init__.py
+-rw-r--r--   0        0        0      494 2023-07-01 19:28:13.555575 xycu-0.1.1/src/xycu/managers/nsfw.py
+-rw-r--r--   0        0        0      485 2023-07-01 19:23:22.239378 xycu-0.1.1/src/xycu/managers/sfw.py
+-rw-r--r--   0        0        0       19 2023-07-01 19:04:08.843430 xycu-0.1.1/src/xycu/models/__init__.py
+-rw-r--r--   0        0        0       19 2023-07-01 19:09:52.336652 xycu-0.1.1/src/xycu/models/enums/__init__.py
+-rw-r--r--   0        0        0       19 2023-07-01 19:10:09.772425 xycu-0.1.1/src/xycu/models/enums/categories/__init__.py
+-rw-r--r--   0        0        0      211 2023-07-01 19:10:02.374449 xycu-0.1.1/src/xycu/models/enums/categories/nsfw.py
+-rw-r--r--   0        0        0      755 2023-07-01 19:14:46.560219 xycu-0.1.1/src/xycu/models/enums/categories/sfw.py
+-rw-r--r--   0        0        0      103 2023-07-01 19:13:02.936202 xycu-0.1.1/src/xycu/models/images.py
+-rw-r--r--   0        0        0     1526 1970-01-01 00:00:00.000000 xycu-0.1.1/PKG-INFO
```

### Comparing `xycu-0.1.0/LICENSE` & `xycu-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xycu-0.1.0/src/xycu/models/enums/categories/sfw.py` & `xycu-0.1.1/src/xycu/models/enums/categories/sfw.py`

 * *Files identical despite different names*

