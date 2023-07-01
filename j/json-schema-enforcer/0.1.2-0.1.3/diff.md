# Comparing `tmp/json_schema_enforcer-0.1.2.tar.gz` & `tmp/json_schema_enforcer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_schema_enforcer-0.1.2.tar", max compression
+gzip compressed data, was "json_schema_enforcer-0.1.3.tar", max compression
```

## Comparing `json_schema_enforcer-0.1.2.tar` & `json_schema_enforcer-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2650 2023-06-27 19:15:35.843509 json_schema_enforcer-0.1.2/README.md
--rw-r--r--   0        0        0      138 2023-06-27 19:29:56.058279 json_schema_enforcer-0.1.2/json_schema_enforcer/__init__.py
--rw-r--r--   0        0        0    29552 2023-06-26 12:22:06.870156 json_schema_enforcer-0.1.2/json_schema_enforcer/schema.py
--rw-r--r--   0        0        0      382 2023-06-27 19:30:09.818194 json_schema_enforcer-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 json_schema_enforcer-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2650 2023-06-27 19:15:35.843509 json_schema_enforcer-0.1.3/README.md
+-rw-r--r--   0        0        0      138 2023-06-27 19:29:56.058279 json_schema_enforcer-0.1.3/json_schema_enforcer/__init__.py
+-rw-r--r--   0        0        0    29865 2023-07-01 10:52:06.073669 json_schema_enforcer-0.1.3/json_schema_enforcer/schema.py
+-rw-r--r--   0        0        0      382 2023-07-01 10:45:45.977058 json_schema_enforcer-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 json_schema_enforcer-0.1.3/PKG-INFO
```

### Comparing `json_schema_enforcer-0.1.2/README.md` & `json_schema_enforcer-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `json_schema_enforcer-0.1.2/json_schema_enforcer/schema.py` & `json_schema_enforcer-0.1.3/json_schema_enforcer/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,16 @@
         _style_config: StyleConfig | None = None,
     ) -> ValidationResult:
         if data[start_index:] == "-":
             return ValidationResult(True, None)
         regex = r"^-?([1-9][0-9]*|0)(\.0*)?"
         match = re.match(regex, data[start_index:])
         if match:
-            return ValidationResult(True, start_index + match.end())
+            # TODO: limit the actual number, not just the length
+            return ValidationResult(True, start_index + min(match.end(), 10))
         return ValidationResult(False, None)
 
 
 class NumberSchemaParser(JsonSchemaParser):
     """A schema parser for number values"""
 
     def __init__(
@@ -161,23 +162,25 @@
             return number <= self.minimum
         return number < self.minimum
 
     def all_multiples_in_range(self, number: float) -> Iterator[int]:
         """Return all multiples between the maximum and minimum"""
         if self.multiple_of is None:
             return []
-        maximum = (
+        maximum = min(
             self.maximum
             or number * (10 * 10 ** int(math.log10(self.multiple_of)))
-            + self.multiple_of
-        )
-        minimum = (
+            + self.multiple_of,
+            1000000000000000000000000,
+        )  # We are limiting it to 16 digits because of floating point precision
+        minimum = min(
             self.minimum
             or number * (10 * 10 ** int(math.log10(self.multiple_of)))
-            - self.multiple_of
+            - self.multiple_of,
+            -1000000000000000000000000,
         )
         if maximum is None or minimum is None:
             return
         if not minimum < maximum:
             return
         for multiple in range(
             int(minimum / self.multiple_of),
@@ -258,17 +261,18 @@
         self,
         data: str,
         start_index: int = 0,
         _indent_level: int = 0,
         _style_config: StyleConfig | None = None,
     ) -> ValidationResult:
         # I'm going to restrict scientific notation for now because it's a pain
+        # TODO: scientific notation + proper non-length-based limiting
         if data[start_index:] == "-":
             return ValidationResult(self.allowed_negative(), None)
-        regex = r"-?([1-9][0-9]*|0)(\.[0-9]*)?"
+        regex = r"-?([1-9][0-9]{0,16}|0)(\.[0-9]{1,16})?"
         match = re.match(regex, data[start_index:])
         if not match:
             return ValidationResult(False, None)
         string_segment = data[start_index : start_index + match.end()]
 
         valid_partial, valid_full = self.partial_validate(string_segment)
         if not valid_partial:
```

### Comparing `json_schema_enforcer-0.1.2/PKG-INFO` & `json_schema_enforcer-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-schema-enforcer
-Version: 0.1.2
+Version: 0.1.3
 Summary: A progressive JSON schema validator
 Author: rizerphe
 Author-email: 44440399+rizerphe@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

