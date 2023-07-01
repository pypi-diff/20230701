# Comparing `tmp/irc_api-0.0.4.tar.gz` & `tmp/irc_api-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irc_api-0.0.4.tar", last modified: Sat Jul  1 15:58:05 2023, max compression
+gzip compressed data, was "irc_api-0.0.5.tar", last modified: Sat Jul  1 16:31:57 2023, max compression
```

## Comparing `irc_api-0.0.4.tar` & `irc_api-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:58:05.456746 irc_api-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 15:57:55.000000 irc_api-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-01 15:58:05.456746 irc_api-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-01 15:57:55.000000 irc_api-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-01 15:57:55.000000 irc_api-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 15:58:05.456746 irc_api-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:58:05.452746 irc_api-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:58:05.452746 irc_api-0.0.4/src/irc_api/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-01 15:57:55.000000 irc_api-0.0.4/src/irc_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-07-01 15:57:55.000000 irc_api-0.0.4/src/irc_api/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    11279 2023-07-01 15:57:55.000000 irc_api-0.0.4/src/irc_api/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-01 15:57:55.000000 irc_api-0.0.4/src/irc_api/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-01 15:57:55.000000 irc_api-0.0.4/src/irc_api/irc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-01 15:57:55.000000 irc_api-0.0.4/src/irc_api/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:58:05.456746 irc_api-0.0.4/src/irc_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-01 15:58:05.000000 irc_api-0.0.4/src/irc_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-01 15:58:05.000000 irc_api-0.0.4/src/irc_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 15:58:05.000000 irc_api-0.0.4/src/irc_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-01 15:58:05.000000 irc_api-0.0.4/src/irc_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-01 15:58:05.000000 irc_api-0.0.4/src/irc_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:31:57.844179 irc_api-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 16:31:42.000000 irc_api-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-01 16:31:57.844179 irc_api-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-01 16:31:42.000000 irc_api-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-01 16:31:42.000000 irc_api-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 16:31:57.844179 irc_api-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:31:57.844179 irc_api-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:31:57.844179 irc_api-0.0.5/src/irc_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-01 16:31:42.000000 irc_api-0.0.5/src/irc_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-07-01 16:31:42.000000 irc_api-0.0.5/src/irc_api/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11279 2023-07-01 16:31:42.000000 irc_api-0.0.5/src/irc_api/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-01 16:31:42.000000 irc_api-0.0.5/src/irc_api/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-01 16:31:42.000000 irc_api-0.0.5/src/irc_api/irc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-01 16:31:42.000000 irc_api-0.0.5/src/irc_api/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:31:57.844179 irc_api-0.0.5/src/irc_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-01 16:31:57.000000 irc_api-0.0.5/src/irc_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-01 16:31:57.000000 irc_api-0.0.5/src/irc_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 16:31:57.000000 irc_api-0.0.5/src/irc_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-01 16:31:57.000000 irc_api-0.0.5/src/irc_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-01 16:31:57.000000 irc_api-0.0.5/src/irc_api.egg-info/top_level.txt
```

### Comparing `irc_api-0.0.4/LICENSE` & `irc_api-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `irc_api-0.0.4/PKG-INFO` & `irc_api-0.0.5/src/irc_api.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: irc_api
-Version: 0.0.4
+Name: irc-api
+Version: 0.0.5
 Summary: An API written in Python to make IRC bots.
 Author: Sha-chan
 Project-URL: Homepage, https://github.com/Shadow15510/irc_api
 Project-URL: Documentation, https://irc-api.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `irc_api-0.0.4/pyproject.toml` & `irc_api-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `irc_api-0.0.4/src/irc_api/bot.py` & `irc_api-0.0.5/src/irc_api/bot.py`

 * *Files identical despite different names*

### Comparing `irc_api-0.0.4/src/irc_api/commands.py` & `irc_api-0.0.5/src/irc_api/commands.py`

 * *Files identical despite different names*

### Comparing `irc_api-0.0.4/src/irc_api/history.py` & `irc_api-0.0.5/src/irc_api/history.py`

 * *Files identical despite different names*

### Comparing `irc_api-0.0.4/src/irc_api/irc.py` & `irc_api-0.0.5/src/irc_api/irc.py`

 * *Files identical despite different names*

### Comparing `irc_api-0.0.4/src/irc_api/message.py` & `irc_api-0.0.5/src/irc_api/message.py`

 * *Files identical despite different names*

