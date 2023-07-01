# Comparing `tmp/flake8_numba-0.1.0.tar.gz` & `tmp/flake8_numba-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_numba-0.1.0.tar", max compression
+gzip compressed data, was "flake8_numba-0.2.0.tar", max compression
```

## Comparing `flake8_numba-0.1.0.tar` & `flake8_numba-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      201 2023-06-24 11:52:21.698322 flake8_numba-0.1.0/flake8_numba/__init__.py
--rw-r--r--   0        0        0      843 2023-06-25 14:21:05.857971 flake8_numba-0.1.0/flake8_numba/plugin.py
--rw-r--r--   0        0        0     1750 2023-06-25 16:29:47.518837 flake8_numba-0.1.0/flake8_numba/rule.py
--rw-r--r--   0        0        0        0 2023-06-23 19:35:21.903653 flake8_numba-0.1.0/flake8_numba/rules/__init__.py
--rw-r--r--   0        0        0     5565 2023-06-25 19:48:43.376303 flake8_numba-0.1.0/flake8_numba/rules/nba0.py
--rw-r--r--   0        0        0      925 2023-06-25 14:51:48.142394 flake8_numba-0.1.0/flake8_numba/rules/nba1.py
--rw-r--r--   0        0        0     9801 2023-06-25 16:47:28.537600 flake8_numba-0.1.0/flake8_numba/rules/nba2.py
--rw-r--r--   0        0        0     8509 2023-06-25 16:53:55.966188 flake8_numba-0.1.0/flake8_numba/utils.py
--rw-r--r--   0        0        0     2404 2023-06-25 16:29:47.522473 flake8_numba-0.1.0/flake8_numba/visitor.py
--rw-r--r--   0        0        0     3069 2023-06-25 16:29:47.522473 flake8_numba-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      747 2023-06-24 18:31:42.168344 flake8_numba-0.1.0/README.md
--rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 flake8_numba-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      201 2023-06-24 11:52:21.698322 flake8_numba-0.2.0/flake8_numba/__init__.py
+-rw-r--r--   0        0        0      843 2023-06-25 14:21:05.857971 flake8_numba-0.2.0/flake8_numba/plugin.py
+-rw-r--r--   0        0        0     1750 2023-06-25 16:29:47.518837 flake8_numba-0.2.0/flake8_numba/rule.py
+-rw-r--r--   0        0        0        0 2023-06-23 19:35:21.903653 flake8_numba-0.2.0/flake8_numba/rules/__init__.py
+-rw-r--r--   0        0        0     5565 2023-06-25 19:48:43.376303 flake8_numba-0.2.0/flake8_numba/rules/nba0.py
+-rw-r--r--   0        0        0      925 2023-06-25 14:51:48.142394 flake8_numba-0.2.0/flake8_numba/rules/nba1.py
+-rw-r--r--   0        0        0    13002 2023-07-01 11:08:24.532910 flake8_numba-0.2.0/flake8_numba/rules/nba2.py
+-rw-r--r--   0        0        0     8509 2023-06-25 16:53:55.966188 flake8_numba-0.2.0/flake8_numba/utils.py
+-rw-r--r--   0        0        0     2404 2023-06-25 16:29:47.522473 flake8_numba-0.2.0/flake8_numba/visitor.py
+-rw-r--r--   0        0        0     3069 2023-07-01 11:12:07.454856 flake8_numba-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      747 2023-06-24 18:31:42.168344 flake8_numba-0.2.0/README.md
+-rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 flake8_numba-0.2.0/PKG-INFO
```

### Comparing `flake8_numba-0.1.0/flake8_numba/plugin.py` & `flake8_numba-0.2.0/flake8_numba/plugin.py`

 * *Files identical despite different names*

### Comparing `flake8_numba-0.1.0/flake8_numba/rule.py` & `flake8_numba-0.2.0/flake8_numba/rule.py`

 * *Files identical despite different names*

### Comparing `flake8_numba-0.1.0/flake8_numba/rules/nba0.py` & `flake8_numba-0.2.0/flake8_numba/rules/nba0.py`

 * *Files identical despite different names*

### Comparing `flake8_numba-0.1.0/flake8_numba/rules/nba1.py` & `flake8_numba-0.2.0/flake8_numba/rules/nba1.py`

 * *Files identical despite different names*

### Comparing `flake8_numba-0.1.0/flake8_numba/rules/nba2.py` & `flake8_numba-0.2.0/flake8_numba/rules/nba2.py`

 * *Files 18% similar despite different names*

```diff
@@ -222,14 +222,57 @@
         return None
 
     @property
     def depends_on(self) -> set[type[Rule]]:
         return {nba0.NBA007}
 
 
+class NBA209(Rule):
+    """Output value is not assigned with guvectorize."""
+
+    def _check(self, node: ast.FunctionDef) -> Optional[Error]:
+        str_signature, location = get_pos_arg_from_decorator(1, node)
+        if not isinstance(str_signature, str):
+            return None
+
+        parts = str_signature.split("->")
+        right_of_arrow = parts[1].strip()
+        n_outputs = Counter(right_of_arrow)["("]
+
+        # Get the function body
+        func_body = node.body
+
+        # Get the names of the last N positional arguments of the function
+        outputs_to_be_modified = {
+            arg.arg for arg in node.args.args[-n_outputs:] if arg.annotation is None
+        }
+
+        # Traverse each node in the function body
+        for sub_node in func_body:
+            # If it is an assignment and the target is a name argument
+            if isinstance(sub_node, ast.Assign) and isinstance(
+                sub_node.targets[0], ast.Subscript
+            ):
+                value = sub_node.targets[0].value
+                if isinstance(value, ast.Name) and value.id in outputs_to_be_modified:
+                    outputs_to_be_modified.remove(value.id)
+
+        if outputs_to_be_modified:
+            msg = (
+                "NBA209: Not all output variables are assigned "
+                f"{list(outputs_to_be_modified)}"
+            )
+            return Error(location.line, location.column, message=msg)
+        return None
+
+    @property
+    def depends_on(self) -> set[type[Rule]]:
+        return {NBA201, NBA202, NBA203, NBA204, NBA205, nba0.NBA005}
+
+
 class NBA211(Rule):
     """Arrays in second pos argument must be separated by commas."""
 
     def _check(self, node: ast.FunctionDef) -> Optional[Error]:
         second_arg, location = get_pos_arg_from_decorator(1, node)
         if not isinstance(second_arg, str):
             return None
@@ -255,7 +298,44 @@
                 comma_detected = False
                 arrow_detected = False
         return None
 
     @property
     def depends_on(self) -> set[type[Rule]]:
         return {nba0.NBA007, NBA203, NBA204}  # First two positional arguments are ok
+
+
+class NBA212(Rule):
+    """Do not assign en input variables."""
+
+    def _check(self, node: ast.FunctionDef) -> Optional[Error]:
+        str_signature, location = get_pos_arg_from_decorator(1, node)
+        if not isinstance(str_signature, str):
+            return None
+
+        parts = str_signature.split("->")
+        right_of_arrow = parts[0].strip()
+        n_inputs = Counter(right_of_arrow)["("]
+
+        # Get the function body
+        func_body = node.body
+
+        # Get the names of the first N positional arguments of the function
+        input_names = {
+            arg.arg for arg in node.args.args[:n_inputs] if arg.annotation is None
+        }
+
+        # Traverse each node in the function body
+        for sub_node in func_body:
+            # If it is an assignment and the target is a name argument
+            if isinstance(sub_node, ast.Assign):
+                targets = sub_node.targets
+                if isinstance(targets[0], ast.Name) and targets[0].id in input_names:
+                    msg = f"NBA212: Do not modify input value: {targets[0].id}"
+                    return Error(location.line, location.column, message=msg)
+                if isinstance(targets[0], ast.Subscript) and isinstance(
+                    targets[0].value, ast.Name
+                ):
+                    if targets[0].value.id in input_names:
+                        msg = f"NBA212: Do not modify input value: {targets[0].value.id}"
+                        return Error(location.line, location.column, message=msg)
+        return None
```

### Comparing `flake8_numba-0.1.0/flake8_numba/utils.py` & `flake8_numba-0.2.0/flake8_numba/utils.py`

 * *Files identical despite different names*

### Comparing `flake8_numba-0.1.0/flake8_numba/visitor.py` & `flake8_numba-0.2.0/flake8_numba/visitor.py`

 * *Files identical despite different names*

### Comparing `flake8_numba-0.1.0/pyproject.toml` & `flake8_numba-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flake8_numba"
-version = "0.1.0"
+version = "0.2.0"
 description = "Perform checks over numba usage"
 authors = ["Manuel Floriano Vázquez <mflovaa@gmail.com>"]
 readme = "README.md"
 packages = [{include = "flake8_numba"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `flake8_numba-0.1.0/README.md` & `flake8_numba-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `flake8_numba-0.1.0/PKG-INFO` & `flake8_numba-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-numba
-Version: 0.1.0
+Version: 0.2.0
 Summary: Perform checks over numba usage
 Author: Manuel Floriano Vázquez
 Author-email: mflovaa@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

