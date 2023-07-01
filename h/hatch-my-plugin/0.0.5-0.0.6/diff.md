# Comparing `tmp/hatch_my_plugin-0.0.5.tar.gz` & `tmp/hatch_my_plugin-0.0.6.tar.gz`

## Comparing `hatch_my_plugin-0.0.5.tar` & `hatch_my_plugin-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rwxr-xr-x   0        0        0      121 2020-02-02 00:00:00.000000 hatch_my_plugin-0.0.5/hatch_my_plugin/__about__.py
--rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 hatch_my_plugin-0.0.5/hatch_my_plugin/__init__.py
--rwxr-xr-x   0        0        0      182 2020-02-02 00:00:00.000000 hatch_my_plugin-0.0.5/hatch_my_plugin/hooks.py
--rwxr-xr-x   0        0        0      415 2020-02-02 00:00:00.000000 hatch_my_plugin-0.0.5/hatch_my_plugin/plugin.py
--rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 hatch_my_plugin-0.0.5/plugin-test/LICENSE.txt
--rwxr-xr-x   0        0        0      499 2020-02-02 00:00:00.000000 hatch_my_plugin-0.0.5/plugin-test/README.md
--rwxr-xr-x   0        0        0      983 2020-02-02 00:00:00.000000 hatch_my_plugin-0.0.5/plugin-test/pyproject.toml
--rwxr-xr-x   0        0        0      121 2020-02-02 00:00:00.000000 hatch_my_plugin-0.0.5/plugin-test/plugin_test/__about__.py
--rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 hatch_my_plugin-0.0.5/plugin-test/plugin_test/__init__.py
--rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 hatch_my_plugin-0.0.5/LICENSE.txt
--rwxr-xr-x   0        0        0      527 2020-02-02 00:00:00.000000 hatch_my_plugin-0.0.5/README.md
--rwxr-xr-x   0        0        0     1090 2020-02-02 00:00:00.000000 hatch_my_plugin-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 hatch_my_plugin-0.0.5/PKG-INFO
+-rwxr-xr-x   0        0        0      121 2020-02-02 00:00:00.000000 hatch_my_plugin-0.0.6/hatch_my_plugin/__about__.py
+-rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 hatch_my_plugin-0.0.6/hatch_my_plugin/__init__.py
+-rwxr-xr-x   0        0        0      182 2020-02-02 00:00:00.000000 hatch_my_plugin-0.0.6/hatch_my_plugin/hooks.py
+-rwxr-xr-x   0        0        0      449 2020-02-02 00:00:00.000000 hatch_my_plugin-0.0.6/hatch_my_plugin/plugin.py
+-rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 hatch_my_plugin-0.0.6/plugin-test/LICENSE.txt
+-rwxr-xr-x   0        0        0      499 2020-02-02 00:00:00.000000 hatch_my_plugin-0.0.6/plugin-test/README.md
+-rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 hatch_my_plugin-0.0.6/plugin-test/pyproject.toml
+-rwxr-xr-x   0        0        0      121 2020-02-02 00:00:00.000000 hatch_my_plugin-0.0.6/plugin-test/plugin_test/__about__.py
+-rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 hatch_my_plugin-0.0.6/plugin-test/plugin_test/__init__.py
+-rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 hatch_my_plugin-0.0.6/LICENSE.txt
+-rwxr-xr-x   0        0        0      527 2020-02-02 00:00:00.000000 hatch_my_plugin-0.0.6/README.md
+-rwxr-xr-x   0        0        0     1090 2020-02-02 00:00:00.000000 hatch_my_plugin-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 hatch_my_plugin-0.0.6/PKG-INFO
```

### Comparing `hatch_my_plugin-0.0.5/plugin-test/LICENSE.txt` & `hatch_my_plugin-0.0.6/plugin-test/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_my_plugin-0.0.5/plugin-test/pyproject.toml` & `hatch_my_plugin-0.0.6/plugin-test/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -29,7 +29,13 @@
 [project.urls]
 Documentation = "https://github.com/unknown/plugin-test#readme"
 Issues = "https://github.com/unknown/plugin-test/issues"
 Source = "https://github.com/unknown/plugin-test"
 
 [tool.hatch.version]
 path = "plugin_test/__about__.py"
+
+[tool.hatch.envs.default]
+dependencies = []
+
+[tool.hatch.envs.default.scripts]
+test = "echo hello default"
```

### Comparing `hatch_my_plugin-0.0.5/LICENSE.txt` & `hatch_my_plugin-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_my_plugin-0.0.5/README.md` & `hatch_my_plugin-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `hatch_my_plugin-0.0.5/pyproject.toml` & `hatch_my_plugin-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hatch_my_plugin-0.0.5/PKG-INFO` & `hatch_my_plugin-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-my-plugin
-Version: 0.0.5
+Version: 0.0.6
 Project-URL: Documentation, https://github.com/unknown/hatch-my-plugin#readme
 Project-URL: Issues, https://github.com/unknown/hatch-my-plugin/issues
 Project-URL: Source, https://github.com/unknown/hatch-my-plugin
 Author-email: warise <example@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

