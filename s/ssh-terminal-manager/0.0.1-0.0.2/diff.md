# Comparing `tmp/ssh_terminal_manager-0.0.1.tar.gz` & `tmp/ssh_terminal_manager-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_terminal_manager-0.0.1.tar", last modified: Sat Jul  1 07:11:45 2023, max compression
+gzip compressed data, was "ssh_terminal_manager-0.0.2.tar", last modified: Sat Jul  1 07:49:17 2023, max compression
```

## Comparing `ssh_terminal_manager-0.0.1.tar` & `ssh_terminal_manager-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 07:11:45.763793 ssh_terminal_manager-0.0.1/
--rw-rw-rw-   0        0        0     1084 2023-06-24 10:20:33.000000 ssh_terminal_manager-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      689 2023-07-01 07:11:45.763793 ssh_terminal_manager-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-07-01 07:07:29.000000 ssh_terminal_manager-0.0.1/README.md
--rw-rw-rw-   0        0        0      703 2023-07-01 07:10:47.000000 ssh_terminal_manager-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-01 07:11:45.763793 ssh_terminal_manager-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-01 07:11:45.619149 ssh_terminal_manager-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-01 07:11:45.662285 ssh_terminal_manager-0.0.1/src/ssh_terminal_manager/
--rw-rw-rw-   0        0        0    10360 2023-07-01 05:12:13.000000 ssh_terminal_manager-0.0.1/src/ssh_terminal_manager/__init__.py
--rw-rw-rw-   0        0        0     3503 2023-07-01 05:12:13.000000 ssh_terminal_manager-0.0.1/src/ssh_terminal_manager/collection.py
--rw-rw-rw-   0        0        0     5199 2023-07-01 05:12:14.000000 ssh_terminal_manager-0.0.1/src/ssh_terminal_manager/command.py
-drwxrwxrwx   0        0        0        0 2023-07-01 07:11:45.759482 ssh_terminal_manager-0.0.1/src/ssh_terminal_manager/default_collections/
--rw-rw-rw-   0        0        0      161 2023-07-01 05:12:15.000000 ssh_terminal_manager-0.0.1/src/ssh_terminal_manager/default_collections/__init__.py
--rw-rw-rw-   0        0        0     1004 2023-07-01 05:12:15.000000 ssh_terminal_manager-0.0.1/src/ssh_terminal_manager/default_collections/const.py
--rw-rw-rw-   0        0        0     3825 2023-07-01 05:12:15.000000 ssh_terminal_manager-0.0.1/src/ssh_terminal_manager/default_collections/linux.py
--rw-rw-rw-   0        0        0     3720 2023-07-01 05:12:15.000000 ssh_terminal_manager-0.0.1/src/ssh_terminal_manager/default_collections/windows_cmd.py
--rw-rw-rw-   0        0        0     3961 2023-07-01 05:12:15.000000 ssh_terminal_manager-0.0.1/src/ssh_terminal_manager/default_collections/windows_ps.py
--rw-rw-rw-   0        0        0      405 2023-07-01 05:12:14.000000 ssh_terminal_manager-0.0.1/src/ssh_terminal_manager/errors.py
--rw-rw-rw-   0        0        0      645 2023-07-01 05:12:14.000000 ssh_terminal_manager-0.0.1/src/ssh_terminal_manager/event.py
--rw-rw-rw-   0        0        0      222 2023-07-01 05:12:14.000000 ssh_terminal_manager-0.0.1/src/ssh_terminal_manager/helpers.py
--rw-rw-rw-   0        0        0     1346 2023-07-01 05:12:14.000000 ssh_terminal_manager-0.0.1/src/ssh_terminal_manager/locker.py
--rw-rw-rw-   0        0        0     4133 2023-07-01 05:12:14.000000 ssh_terminal_manager-0.0.1/src/ssh_terminal_manager/manager.py
--rw-rw-rw-   0        0        0     8606 2023-07-01 05:12:14.000000 ssh_terminal_manager-0.0.1/src/ssh_terminal_manager/sensor.py
-drwxrwxrwx   0        0        0        0 2023-07-01 07:11:45.731544 ssh_terminal_manager-0.0.1/src/ssh_terminal_manager.egg-info/
--rw-rw-rw-   0        0        0      689 2023-07-01 07:11:45.000000 ssh_terminal_manager-0.0.1/src/ssh_terminal_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      878 2023-07-01 07:11:45.000000 ssh_terminal_manager-0.0.1/src/ssh_terminal_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 07:11:45.000000 ssh_terminal_manager-0.0.1/src/ssh_terminal_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-07-01 07:11:45.000000 ssh_terminal_manager-0.0.1/src/ssh_terminal_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-01 07:11:45.000000 ssh_terminal_manager-0.0.1/src/ssh_terminal_manager.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 07:49:17.697689 ssh_terminal_manager-0.0.2/
+-rw-rw-rw-   0        0        0     1084 2023-06-24 10:20:33.000000 ssh_terminal_manager-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      689 2023-07-01 07:49:17.696056 ssh_terminal_manager-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-07-01 07:07:29.000000 ssh_terminal_manager-0.0.2/README.md
+-rw-rw-rw-   0        0        0      674 2023-07-01 07:48:07.000000 ssh_terminal_manager-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-01 07:49:17.698691 ssh_terminal_manager-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-01 07:49:17.552478 ssh_terminal_manager-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-01 07:49:17.610433 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/
+-rw-rw-rw-   0        0        0    10338 2023-07-01 07:37:03.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/__init__.py
+-rw-rw-rw-   0        0        0     3503 2023-07-01 05:12:13.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/collection.py
+-rw-rw-rw-   0        0        0     5199 2023-07-01 05:12:14.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/command.py
+drwxrwxrwx   0        0        0        0 2023-07-01 07:49:17.693748 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/default_collections/
+-rw-rw-rw-   0        0        0      161 2023-07-01 05:12:15.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/default_collections/__init__.py
+-rw-rw-rw-   0        0        0     1004 2023-07-01 05:12:15.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/default_collections/const.py
+-rw-rw-rw-   0        0        0     3825 2023-07-01 05:12:15.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/default_collections/linux.py
+-rw-rw-rw-   0        0        0     3720 2023-07-01 05:12:15.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/default_collections/windows_cmd.py
+-rw-rw-rw-   0        0        0     3961 2023-07-01 05:12:15.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/default_collections/windows_ps.py
+-rw-rw-rw-   0        0        0      405 2023-07-01 05:12:14.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/errors.py
+-rw-rw-rw-   0        0        0      645 2023-07-01 05:12:14.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/event.py
+-rw-rw-rw-   0        0        0      222 2023-07-01 05:12:14.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/helpers.py
+-rw-rw-rw-   0        0        0     1346 2023-07-01 05:12:14.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/locker.py
+-rw-rw-rw-   0        0        0     4133 2023-07-01 05:12:14.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/manager.py
+-rw-rw-rw-   0        0        0     8606 2023-07-01 05:12:14.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/sensor.py
+drwxrwxrwx   0        0        0        0 2023-07-01 07:49:17.668184 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager.egg-info/
+-rw-rw-rw-   0        0        0      689 2023-07-01 07:49:17.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      878 2023-07-01 07:49:17.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 07:49:17.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-07-01 07:49:17.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-01 07:49:17.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager.egg-info/top_level.txt
```

### Comparing `ssh_terminal_manager-0.0.1/LICENSE` & `ssh_terminal_manager-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ssh_terminal_manager-0.0.1/PKG-INFO` & `ssh_terminal_manager-0.0.2/src/ssh_terminal_manager.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ssh_terminal_manager
-Version: 0.0.1
+Name: ssh-terminal-manager
+Version: 0.0.2
 Summary: Control and monitor devices with SSH terminal commands
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Keywords: ssh,terminal,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `ssh_terminal_manager-0.0.1/pyproject.toml` & `ssh_terminal_manager-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ssh_terminal_manager"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Control and monitor devices with SSH terminal commands"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -18,13 +18,12 @@
 ]
 keywords = [
   "ssh", 
   "terminal", 
   "command line",
 ]
 dependencies = [
-  "async-timeout >= 4.0.2",
   "icmplib >= 3.0",
   "paramiko >= 3.2.0",
   "python-slugify >= 4.0.1",
   "wakeonlan >= 3.0.0",
 ]
```

### Comparing `ssh_terminal_manager-0.0.1/src/ssh_terminal_manager/__init__.py` & `ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """SSH terminal manager."""
 from __future__ import annotations
 
 import asyncio
 import logging
 from time import time
 
-import async_timeout
 import icmplib
 import paramiko
 import wakeonlan
 
 from .collection import Collection
 from .command import ActionCommand, Command, SensorCommand
 from .default_collections import ActionKey, SensorKey
```

### Comparing `ssh_terminal_manager-0.0.1/src/ssh_terminal_manager/collection.py` & `ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/collection.py`

 * *Files identical despite different names*

### Comparing `ssh_terminal_manager-0.0.1/src/ssh_terminal_manager/command.py` & `ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/command.py`

 * *Files identical despite different names*

### Comparing `ssh_terminal_manager-0.0.1/src/ssh_terminal_manager/default_collections/const.py` & `ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/default_collections/const.py`

 * *Files identical despite different names*

### Comparing `ssh_terminal_manager-0.0.1/src/ssh_terminal_manager/default_collections/linux.py` & `ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/default_collections/linux.py`

 * *Files identical despite different names*

### Comparing `ssh_terminal_manager-0.0.1/src/ssh_terminal_manager/default_collections/windows_cmd.py` & `ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/default_collections/windows_cmd.py`

 * *Files identical despite different names*

### Comparing `ssh_terminal_manager-0.0.1/src/ssh_terminal_manager/default_collections/windows_ps.py` & `ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/default_collections/windows_ps.py`

 * *Files identical despite different names*

### Comparing `ssh_terminal_manager-0.0.1/src/ssh_terminal_manager/event.py` & `ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/event.py`

 * *Files identical despite different names*

### Comparing `ssh_terminal_manager-0.0.1/src/ssh_terminal_manager/locker.py` & `ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/locker.py`

 * *Files identical despite different names*

### Comparing `ssh_terminal_manager-0.0.1/src/ssh_terminal_manager/manager.py` & `ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/manager.py`

 * *Files identical despite different names*

### Comparing `ssh_terminal_manager-0.0.1/src/ssh_terminal_manager/sensor.py` & `ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/sensor.py`

 * *Files identical despite different names*

### Comparing `ssh_terminal_manager-0.0.1/src/ssh_terminal_manager.egg-info/PKG-INFO` & `ssh_terminal_manager-0.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ssh-terminal-manager
-Version: 0.0.1
+Name: ssh_terminal_manager
+Version: 0.0.2
 Summary: Control and monitor devices with SSH terminal commands
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Keywords: ssh,terminal,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `ssh_terminal_manager-0.0.1/src/ssh_terminal_manager.egg-info/SOURCES.txt` & `ssh_terminal_manager-0.0.2/src/ssh_terminal_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

