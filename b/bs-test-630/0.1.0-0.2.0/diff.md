# Comparing `tmp/bs_test_630-0.1.0.tar.gz` & `tmp/bs_test_630-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_test_630-0.1.0.tar", max compression
+gzip compressed data, was "bs_test_630-0.2.0.tar", max compression
```

## Comparing `bs_test_630-0.1.0.tar` & `bs_test_630-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        5 2023-06-26 21:55:07.746361 bs_test_630-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-23 22:46:21.760508 bs_test_630-0.1.0/blacksmith/__init__.py
--rw-r--r--   0        0        0     3546 2023-06-30 23:30:09.809113 bs_test_630-0.1.0/blacksmith/agents.py
--rw-r--r--   0        0        0      553 2023-06-28 03:04:51.693365 bs_test_630-0.1.0/blacksmith/defaults/__pycache__/prompts.cpython-311.pyc
--rw-r--r--   0        0        0      843 2023-06-30 22:48:59.357216 bs_test_630-0.1.0/blacksmith/defaults/prompts.py
--rw-r--r--   0        0        0      368 2023-06-29 10:21:48.331464 bs_test_630-0.1.0/blacksmith/llm.py
--rw-r--r--   0        0        0        0 2023-06-26 22:06:00.728175 bs_test_630-0.1.0/blacksmith/scripts/__init__.py
--rw-r--r--   0        0        0      151 2023-06-26 22:06:03.377477 bs_test_630-0.1.0/blacksmith/scripts/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4315 2023-06-30 22:15:46.655686 bs_test_630-0.1.0/blacksmith/scripts/__pycache__/cli.cpython-311.pyc
--rw-r--r--   0        0        0     4392 2023-06-30 22:05:31.984149 bs_test_630-0.1.0/blacksmith/scripts/__pycache__/images.cpython-311.pyc
--rw-r--r--   0        0        0     5879 2023-06-30 21:42:18.409842 bs_test_630-0.1.0/blacksmith/scripts/__pycache__/k8s.cpython-311.pyc
--rw-r--r--   0        0        0     2976 2023-06-26 22:05:41.831425 bs_test_630-0.1.0/blacksmith/scripts/__pycache__/main.cpython-311.pyc
--rw-r--r--   0        0        0     2318 2023-06-30 22:15:42.101952 bs_test_630-0.1.0/blacksmith/scripts/cli.py
--rw-r--r--   0        0        0     3806 2023-06-30 22:05:27.946280 bs_test_630-0.1.0/blacksmith/scripts/images.py
--rw-r--r--   0        0        0     5351 2023-06-30 21:01:20.188340 bs_test_630-0.1.0/blacksmith/scripts/k8s.py
--rw-r--r--   0        0        0     2406 2023-06-28 23:45:12.797321 bs_test_630-0.1.0/blacksmith/tools.py
--rw-r--r--   0        0        0      515 2023-06-30 23:30:25.517756 bs_test_630-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      607 1970-01-01 00:00:00.000000 bs_test_630-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        5 2023-06-26 21:55:07.746361 bs_test_630-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-23 22:46:21.760508 bs_test_630-0.2.0/blacksmith/__init__.py
+-rw-r--r--   0        0        0     3550 2023-06-30 23:36:29.343312 bs_test_630-0.2.0/blacksmith/agents.py
+-rw-r--r--   0        0        0      553 2023-06-28 03:04:51.693365 bs_test_630-0.2.0/blacksmith/defaults/__pycache__/prompts.cpython-311.pyc
+-rw-r--r--   0        0        0      843 2023-06-30 22:48:59.357216 bs_test_630-0.2.0/blacksmith/defaults/prompts.py
+-rw-r--r--   0        0        0      368 2023-06-29 10:21:48.331464 bs_test_630-0.2.0/blacksmith/llm.py
+-rw-r--r--   0        0        0        0 2023-06-26 22:06:00.728175 bs_test_630-0.2.0/blacksmith/scripts/__init__.py
+-rw-r--r--   0        0        0      151 2023-06-26 22:06:03.377477 bs_test_630-0.2.0/blacksmith/scripts/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4315 2023-06-30 22:15:46.655686 bs_test_630-0.2.0/blacksmith/scripts/__pycache__/cli.cpython-311.pyc
+-rw-r--r--   0        0        0     4392 2023-06-30 22:05:31.984149 bs_test_630-0.2.0/blacksmith/scripts/__pycache__/images.cpython-311.pyc
+-rw-r--r--   0        0        0     5879 2023-06-30 21:42:18.409842 bs_test_630-0.2.0/blacksmith/scripts/__pycache__/k8s.cpython-311.pyc
+-rw-r--r--   0        0        0     2976 2023-06-26 22:05:41.831425 bs_test_630-0.2.0/blacksmith/scripts/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0        0        0     2318 2023-06-30 22:15:42.101952 bs_test_630-0.2.0/blacksmith/scripts/cli.py
+-rw-r--r--   0        0        0     3806 2023-06-30 22:05:27.946280 bs_test_630-0.2.0/blacksmith/scripts/images.py
+-rw-r--r--   0        0        0     5351 2023-06-30 21:01:20.188340 bs_test_630-0.2.0/blacksmith/scripts/k8s.py
+-rw-r--r--   0        0        0     2406 2023-06-28 23:45:12.797321 bs_test_630-0.2.0/blacksmith/tools.py
+-rw-r--r--   0        0        0      515 2023-06-30 23:36:35.886355 bs_test_630-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      607 1970-01-01 00:00:00.000000 bs_test_630-0.2.0/PKG-INFO
```

### Comparing `bs_test_630-0.1.0/blacksmith/agents.py` & `bs_test_630-0.2.0/blacksmith/agents.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                     tool_res = requests.get(url=url, json=args)
                     data = tool_res.json()
                     print(f"Executed function {service_name}. Result: {data}")
                     func_calls.append(
                         {
                             "execution_order": iterations,
                             "function_name": {service_name},
-                            "function_params": {args},
+                            "params": {func["arguments"]},
                             "result": {data},
                         }
                     )
                     messages.append(
                         {
                             "role": "user",
                             "content": f"""
```

### Comparing `bs_test_630-0.1.0/blacksmith/defaults/__pycache__/prompts.cpython-311.pyc` & `bs_test_630-0.2.0/blacksmith/defaults/__pycache__/prompts.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bs_test_630-0.1.0/blacksmith/defaults/prompts.py` & `bs_test_630-0.2.0/blacksmith/defaults/prompts.py`

 * *Files identical despite different names*

### Comparing `bs_test_630-0.1.0/blacksmith/scripts/__pycache__/cli.cpython-311.pyc` & `bs_test_630-0.2.0/blacksmith/scripts/__pycache__/cli.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bs_test_630-0.1.0/blacksmith/scripts/__pycache__/images.cpython-311.pyc` & `bs_test_630-0.2.0/blacksmith/scripts/__pycache__/images.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bs_test_630-0.1.0/blacksmith/scripts/__pycache__/k8s.cpython-311.pyc` & `bs_test_630-0.2.0/blacksmith/scripts/__pycache__/k8s.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bs_test_630-0.1.0/blacksmith/scripts/__pycache__/main.cpython-311.pyc` & `bs_test_630-0.2.0/blacksmith/scripts/__pycache__/main.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bs_test_630-0.1.0/blacksmith/scripts/cli.py` & `bs_test_630-0.2.0/blacksmith/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `bs_test_630-0.1.0/blacksmith/scripts/images.py` & `bs_test_630-0.2.0/blacksmith/scripts/images.py`

 * *Files identical despite different names*

### Comparing `bs_test_630-0.1.0/blacksmith/scripts/k8s.py` & `bs_test_630-0.2.0/blacksmith/scripts/k8s.py`

 * *Files identical despite different names*

### Comparing `bs_test_630-0.1.0/blacksmith/tools.py` & `bs_test_630-0.2.0/blacksmith/tools.py`

 * *Files identical despite different names*

### Comparing `bs_test_630-0.1.0/pyproject.toml` & `bs_test_630-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bs-test-630"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["alec <fkalec@gmail.com>"]
 readme = "README.md"
 packages = [{include = "blacksmith"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `bs_test_630-0.1.0/PKG-INFO` & `bs_test_630-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bs-test-630
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: alec
 Author-email: fkalec@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: docker (>=6.1.3,<7.0.0)
```

