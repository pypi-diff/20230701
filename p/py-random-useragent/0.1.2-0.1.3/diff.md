# Comparing `tmp/py_random_useragent-0.1.2.tar.gz` & `tmp/py_random_useragent-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_random_useragent-0.1.2.tar", max compression
+gzip compressed data, was "py_random_useragent-0.1.3.tar", max compression
```

## Comparing `py_random_useragent-0.1.2.tar` & `py_random_useragent-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      248 2023-07-01 06:06:38.669241 py_random_useragent-0.1.2/README.md
--rw-r--r--   0        0        0      295 2023-07-01 06:15:49.435485 py_random_useragent-0.1.2/py_random_useragent/__init__.py
--rw-r--r--   0        0        0      203 2023-05-14 06:24:47.700344 py_random_useragent-0.1.2/py_random_useragent/__main__.py
--rw-r--r--   0        0        0      296 2023-07-01 06:14:48.185698 py_random_useragent-0.1.2/py_random_useragent/main.py
--rw-r--r--   0        0        0     2063 2023-07-01 06:15:38.931165 py_random_useragent-0.1.2/py_random_useragent/user_agent.py
--rw-r--r--   0        0        0     5165 2023-07-01 06:16:15.020285 py_random_useragent-0.1.2/py_random_useragent/useragents.txt
--rw-r--r--   0        0        0      524 2023-07-01 06:15:54.591644 py_random_useragent-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      869 1970-01-01 00:00:00.000000 py_random_useragent-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      248 2023-07-01 06:22:16.810097 py_random_useragent-0.1.3/README.md
+-rw-r--r--   0        0        0      295 2023-07-01 06:23:00.970888 py_random_useragent-0.1.3/py_random_useragent/__init__.py
+-rw-r--r--   0        0        0      203 2023-05-14 06:24:47.700344 py_random_useragent-0.1.3/py_random_useragent/__main__.py
+-rw-r--r--   0        0        0      296 2023-07-01 06:14:48.185698 py_random_useragent-0.1.3/py_random_useragent/main.py
+-rw-r--r--   0        0        0     2063 2023-07-01 06:15:38.931165 py_random_useragent-0.1.3/py_random_useragent/user_agent.py
+-rw-r--r--   0        0        0     5165 2023-07-01 06:23:43.839748 py_random_useragent-0.1.3/py_random_useragent/useragents.txt
+-rw-r--r--   0        0        0      524 2023-07-01 06:23:10.787078 py_random_useragent-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      869 1970-01-01 00:00:00.000000 py_random_useragent-0.1.3/PKG-INFO
```

### Comparing `py_random_useragent-0.1.2/py_random_useragent/user_agent.py` & `py_random_useragent-0.1.3/py_random_useragent/user_agent.py`

 * *Files identical despite different names*

### Comparing `py_random_useragent-0.1.2/py_random_useragent/useragents.txt` & `py_random_useragent-0.1.3/py_random_useragent/useragents.txt`

 * *Files identical despite different names*

### Comparing `py_random_useragent-0.1.2/pyproject.toml` & `py_random_useragent-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-random-useragent"
-version = "0.1.2"
+version = "0.1.3"
 description = "Generate a random User Agent"
 authors = ["Oleg Suvorinov <suvorinovoleg@yandex.ru>"]
 readme = "README.md"
 homepage = "https://github.com/suvorinov/py-random-useragent"
 packages = [{include = "py_random_useragent"}]
 
 [tool.poetry.dependencies]
```

### Comparing `py_random_useragent-0.1.2/PKG-INFO` & `py_random_useragent-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-random-useragent
-Version: 0.1.2
+Version: 0.1.3
 Summary: Generate a random User Agent
 Home-page: https://github.com/suvorinov/py-random-useragent
 Author: Oleg Suvorinov
 Author-email: suvorinovoleg@yandex.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -27,11 +27,11 @@
 
 ### Usage
 
 ``` python
 from py_random_useragent import UserAgent
 
 # Получение UserAgent
-ua = UserAgent().get_ua()
-print(ua)
+UA = UserAgent()
+print(UA.get_ua())
 ```
```

