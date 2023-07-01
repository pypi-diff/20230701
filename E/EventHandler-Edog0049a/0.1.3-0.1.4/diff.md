# Comparing `tmp/eventhandler_edog0049a-0.1.3.tar.gz` & `tmp/eventhandler_edog0049a-0.1.4.tar.gz`

## Comparing `eventhandler_edog0049a-0.1.3.tar` & `eventhandler_edog0049a-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.3/.secret
--rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.3/distbackup/eventhandler_edog0049a-0.1.2-py3-none-any.whl
--rw-r--r--   0        0        0     8920 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.3/distbackup/eventhandler_edog0049a-0.1.2.tar.gz
--rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.3/src/EventHandler/EventHandler.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.3/src/EventHandler/__init__.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.3/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.3/README.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.4/.secret
+-rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.4/distbackup/eventhandler_edog0049a-0.1.2-py3-none-any.whl
+-rw-r--r--   0        0        0     8920 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.4/distbackup/eventhandler_edog0049a-0.1.2.tar.gz
+-rw-r--r--   0        0        0     3834 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.4/distbackup/eventhandler_edog0049a-0.1.3-py3-none-any.whl
+-rw-r--r--   0        0        0    15290 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.4/distbackup/eventhandler_edog0049a-0.1.3.tar.gz
+-rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.4/src/EventHandler/EventHandler.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.4/src/EventHandler/__init__.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.4/README.md
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 eventhandler_edog0049a-0.1.4/PKG-INFO
```

### Comparing `eventhandler_edog0049a-0.1.3/distbackup/eventhandler_edog0049a-0.1.2-py3-none-any.whl` & `eventhandler_edog0049a-0.1.4/distbackup/eventhandler_edog0049a-0.1.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `eventhandler_edog0049a-0.1.3/distbackup/eventhandler_edog0049a-0.1.2.tar.gz` & `eventhandler_edog0049a-0.1.4/distbackup/eventhandler_edog0049a-0.1.2.tar.gz`

 * *Files identical despite different names*

### Comparing `eventhandler_edog0049a-0.1.3/src/EventHandler/EventHandler.py` & `eventhandler_edog0049a-0.1.4/src/EventHandler/EventHandler.py`

 * *Files identical despite different names*

### Comparing `eventhandler_edog0049a-0.1.3/LICENSE.txt` & `eventhandler_edog0049a-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eventhandler_edog0049a-0.1.3/pyproject.toml` & `eventhandler_edog0049a-0.1.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EventHandler_Edog0049a"
-version = "0.1.3"
+version = "0.1.4"
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
-EventHandler= "EventHandler"
+EventHandler= "Events"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/EventHandler"]
```

