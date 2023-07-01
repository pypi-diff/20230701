# Comparing `tmp/eventhandler_edog0049a-0.1.1.tar.gz` & `tmp/eventhandler_edog0049a-0.1.2.tar.gz`

## Comparing `eventhandler_edog0049a-0.1.1.tar` & `eventhandler_edog0049a-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.1/.secret
--rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.1/src/EventHandler/EventHandler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.1/src/EventHandler/__init__.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.1/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.1/README.md
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.2/.secret
+-rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.2/distbackup/eventhandler_edog0049a-0.1.2-py3-none-any.whl
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.2/distbackup/eventhandler_edog0049a-0.1.2.tar.gz
+-rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.2/src/EventHandler/EventHandler.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.2/src/EventHandler/__init__.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.2/README.md
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.2/PKG-INFO
```

### Comparing `eventhandler_edog0049a-0.1.1/src/EventHandler/EventHandler.py` & `eventhandler_edog0049a-0.1.2/src/EventHandler/EventHandler.py`

 * *Files identical despite different names*

### Comparing `eventhandler_edog0049a-0.1.1/LICENSE.txt` & `eventhandler_edog0049a-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eventhandler_edog0049a-0.1.1/pyproject.toml` & `eventhandler_edog0049a-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EventHandler_Edog0049a"
-version = "0.1.1"
+version = "0.1.2"
 description = 'A simple event handler'
 readme = {"file" = "README.md", "content-type" = "text/markdown"}
 requires-python = ">=3.8"
 license = "Apache-2.0 OR MIT"
 authors = [
   { name = "Eli Reid", email = "Elir@elireid.com" },
 ]
```

