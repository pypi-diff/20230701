# Comparing `tmp/eventhandler_edog0049a-0.1.0.tar.gz` & `tmp/eventhandler_edog0049a-0.1.1.tar.gz`

## Comparing `eventhandler_edog0049a-0.1.0.tar` & `eventhandler_edog0049a-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.0/.secret
--rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.0/src/EventHandler/EventHandler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.0/src/EventHandler/__init__.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.0/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.0/README.md
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.1/.secret
+-rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.1/src/EventHandler/EventHandler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.1/src/EventHandler/__init__.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.1/README.md
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.1/PKG-INFO
```

### Comparing `eventhandler_edog0049a-0.1.0/src/EventHandler/EventHandler.py` & `eventhandler_edog0049a-0.1.1/src/EventHandler/EventHandler.py`

 * *Files identical despite different names*

### Comparing `eventhandler_edog0049a-0.1.0/LICENSE.txt` & `eventhandler_edog0049a-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eventhandler_edog0049a-0.1.0/pyproject.toml` & `eventhandler_edog0049a-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EventHandler_Edog0049a"
-version = "0.1.0"
+version = "0.1.1"
 description = 'A simple event handler'
 readme = {"file" = "README.md", "content-type" = "text/markdown"}
 requires-python = ">=3.8"
 license = "Apache-2.0 OR MIT"
 authors = [
   { name = "Eli Reid", email = "Elir@elireid.com" },
 ]
 
 [project.urls]
 "Source code" = "https://github.com/eli-reid/EventHandler"
 
 [project.entry-points.plugin-namespace]
-TEventHandler = "EventHandler"
+EventHandler = "EventHandler"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/EventHandler"]
```

