# Comparing `tmp/local_llm_function_calling-0.1.2.tar.gz` & `tmp/local_llm_function_calling-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local_llm_function_calling-0.1.2.tar", max compression
+gzip compressed data, was "local_llm_function_calling-0.1.3.tar", max compression
```

## Comparing `local_llm_function_calling-0.1.2.tar` & `local_llm_function_calling-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3105 2023-06-27 19:54:06.411406 local_llm_function_calling-0.1.2/README.md
--rw-r--r--   0        0        0      555 2023-06-27 19:57:49.091938 local_llm_function_calling-0.1.2/local_llm_function_calling/__init__.py
--rw-r--r--   0        0        0     5386 2023-06-27 19:57:39.016004 local_llm_function_calling-0.1.2/local_llm_function_calling/constrainer.py
--rw-r--r--   0        0        0     5256 2023-06-27 19:57:01.459251 local_llm_function_calling-0.1.2/local_llm_function_calling/generator.py
--rw-r--r--   0        0        0     3950 2023-06-27 09:38:19.333497 local_llm_function_calling-0.1.2/local_llm_function_calling/prompter.py
--rw-r--r--   0        0        0      433 2023-06-27 19:59:48.920153 local_llm_function_calling-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3566 1970-01-01 00:00:00.000000 local_llm_function_calling-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3105 2023-06-27 19:54:06.411406 local_llm_function_calling-0.1.3/README.md
+-rw-r--r--   0        0        0      555 2023-06-27 19:57:49.091938 local_llm_function_calling-0.1.3/local_llm_function_calling/__init__.py
+-rw-r--r--   0        0        0     5386 2023-06-27 19:57:39.016004 local_llm_function_calling-0.1.3/local_llm_function_calling/constrainer.py
+-rw-r--r--   0        0        0     5256 2023-06-27 19:57:01.459251 local_llm_function_calling-0.1.3/local_llm_function_calling/generator.py
+-rw-r--r--   0        0        0     3950 2023-06-27 09:38:19.333497 local_llm_function_calling-0.1.3/local_llm_function_calling/prompter.py
+-rw-r--r--   0        0        0      433 2023-07-01 10:56:36.554955 local_llm_function_calling-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3566 1970-01-01 00:00:00.000000 local_llm_function_calling-0.1.3/PKG-INFO
```

### Comparing `local_llm_function_calling-0.1.2/README.md` & `local_llm_function_calling-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `local_llm_function_calling-0.1.2/local_llm_function_calling/__init__.py` & `local_llm_function_calling-0.1.3/local_llm_function_calling/__init__.py`

 * *Files identical despite different names*

### Comparing `local_llm_function_calling-0.1.2/local_llm_function_calling/constrainer.py` & `local_llm_function_calling-0.1.3/local_llm_function_calling/constrainer.py`

 * *Files identical despite different names*

### Comparing `local_llm_function_calling-0.1.2/local_llm_function_calling/generator.py` & `local_llm_function_calling-0.1.3/local_llm_function_calling/generator.py`

 * *Files identical despite different names*

### Comparing `local_llm_function_calling-0.1.2/local_llm_function_calling/prompter.py` & `local_llm_function_calling-0.1.3/local_llm_function_calling/prompter.py`

 * *Files identical despite different names*

### Comparing `local_llm_function_calling-0.1.2/PKG-INFO` & `local_llm_function_calling-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: local-llm-function-calling
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: rizerphe
 Author-email: 44440399+rizerphe@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: json-schema-enforcer (>=0.1.2,<0.2.0)
+Requires-Dist: json-schema-enforcer (>=0.1.3,<0.2.0)
 Requires-Dist: torch (>=2.0.1,<3.0.0)
 Requires-Dist: transformers (>=4.30.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Local LLM function calling
 
 ## Overview
```

