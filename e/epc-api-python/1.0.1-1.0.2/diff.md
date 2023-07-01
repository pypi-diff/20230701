# Comparing `tmp/epc-api-python-1.0.1.tar.gz` & `tmp/epc-api-python-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epc-api-python-1.0.1.tar", last modified: Mon Apr 17 12:22:56 2023, max compression
+gzip compressed data, was "epc-api-python-1.0.2.tar", last modified: Sat Jul  1 14:49:19 2023, max compression
```

## Comparing `epc-api-python-1.0.1.tar` & `epc-api-python-1.0.2.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 khalimconn-kowlessar   (501) staff       (20)        0 2023-04-17 12:22:56.899850 epc-api-python-1.0.1/
--rw-rw-r--   0 khalimconn-kowlessar   (501) staff       (20)     1064 2023-04-14 15:59:56.000000 epc-api-python-1.0.1/LICENSE
--rw-rw-r--   0 khalimconn-kowlessar   (501) staff       (20)       79 2023-04-17 12:02:18.000000 epc-api-python-1.0.1/MANIFEST.in
--rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)     4292 2023-04-17 12:22:56.899665 epc-api-python-1.0.1/PKG-INFO
--rw-rw-r--   0 khalimconn-kowlessar   (501) staff       (20)     2610 2023-04-17 12:15:56.000000 epc-api-python-1.0.1/README.md
-drwxr-xr-x   0 khalimconn-kowlessar   (501) staff       (20)        0 2023-04-17 12:22:56.896993 epc-api-python-1.0.1/epc_api/
--rw-rw-r--   0 khalimconn-kowlessar   (501) staff       (20)       22 2023-04-17 12:17:35.000000 epc-api-python-1.0.1/epc_api/__init__.py
--rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)     8870 2023-04-17 11:33:36.000000 epc-api-python-1.0.1/epc_api/client.py
--rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)      626 2023-04-17 11:33:36.000000 epc-api-python-1.0.1/epc_api/exceptions.py
--rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)     1282 2023-04-14 11:22:21.000000 epc-api-python-1.0.1/epc_api/schemas.py
-drwxr-xr-x   0 khalimconn-kowlessar   (501) staff       (20)        0 2023-04-17 12:22:56.897917 epc-api-python-1.0.1/epc_api_python.egg-info/
--rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)     4292 2023-04-17 12:22:56.000000 epc-api-python-1.0.1/epc_api_python.egg-info/PKG-INFO
--rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)      488 2023-04-17 12:22:56.000000 epc-api-python-1.0.1/epc_api_python.egg-info/SOURCES.txt
--rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)        1 2023-04-17 12:22:56.000000 epc-api-python-1.0.1/epc_api_python.egg-info/dependency_links.txt
--rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)      117 2023-04-17 12:22:56.000000 epc-api-python-1.0.1/epc_api_python.egg-info/requires.txt
--rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)        8 2023-04-17 12:22:56.000000 epc-api-python-1.0.1/epc_api_python.egg-info/top_level.txt
-drwxr-xr-x   0 khalimconn-kowlessar   (501) staff       (20)        0 2023-04-17 12:22:56.898535 epc-api-python-1.0.1/examples/
--rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)      546 2023-04-17 11:33:36.000000 epc-api-python-1.0.1/examples/basic_example.py
--rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)      411 2023-04-17 11:33:36.000000 epc-api-python-1.0.1/examples/csv_example.py
--rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)      473 2023-04-17 11:33:36.000000 epc-api-python-1.0.1/examples/zip_example.py
--rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)     1127 2023-04-17 12:22:23.000000 epc-api-python-1.0.1/pyproject.toml
-drwxr-xr-x   0 khalimconn-kowlessar   (501) staff       (20)        0 2023-04-17 12:22:56.898782 epc-api-python-1.0.1/requirements/
--rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)       45 2023-04-17 10:55:17.000000 epc-api-python-1.0.1/requirements/prod.txt
--rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)       38 2023-04-17 12:22:56.899896 epc-api-python-1.0.1/setup.cfg
--rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)       50 2023-04-17 11:24:27.000000 epc-api-python-1.0.1/setup.py
-drwxr-xr-x   0 khalimconn-kowlessar   (501) staff       (20)        0 2023-04-17 12:22:56.899380 epc-api-python-1.0.1/tests/
--rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)     2462 2023-04-17 11:33:36.000000 epc-api-python-1.0.1/tests/test_client_init.py
--rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)     3223 2023-04-17 11:33:36.000000 epc-api-python-1.0.1/tests/test_endpoints.py
--rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)     2186 2023-04-17 11:33:36.000000 epc-api-python-1.0.1/tests/test_schema.py
+drwxr-xr-x   0 khalimconn-kowlessar   (501) staff       (20)        0 2023-07-01 14:49:19.353803 epc-api-python-1.0.2/
+-rw-rw-r--   0 khalimconn-kowlessar   (501) staff       (20)     1064 2023-04-14 15:59:56.000000 epc-api-python-1.0.2/LICENSE
+-rw-rw-r--   0 khalimconn-kowlessar   (501) staff       (20)       79 2023-04-17 12:02:18.000000 epc-api-python-1.0.2/MANIFEST.in
+-rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)     4292 2023-07-01 14:49:19.353639 epc-api-python-1.0.2/PKG-INFO
+-rw-rw-r--   0 khalimconn-kowlessar   (501) staff       (20)     2610 2023-04-17 12:15:56.000000 epc-api-python-1.0.2/README.md
+drwxr-xr-x   0 khalimconn-kowlessar   (501) staff       (20)        0 2023-07-01 14:49:19.349796 epc-api-python-1.0.2/epc_api/
+-rw-rw-r--   0 khalimconn-kowlessar   (501) staff       (20)       22 2023-04-17 12:17:35.000000 epc-api-python-1.0.2/epc_api/__init__.py
+-rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)     9003 2023-07-01 14:28:41.000000 epc-api-python-1.0.2/epc_api/client.py
+-rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)      626 2023-04-17 11:33:36.000000 epc-api-python-1.0.2/epc_api/exceptions.py
+-rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)     1282 2023-04-14 11:22:21.000000 epc-api-python-1.0.2/epc_api/schemas.py
+drwxr-xr-x   0 khalimconn-kowlessar   (501) staff       (20)        0 2023-07-01 14:49:19.350654 epc-api-python-1.0.2/epc_api_python.egg-info/
+-rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)     4292 2023-07-01 14:49:19.000000 epc-api-python-1.0.2/epc_api_python.egg-info/PKG-INFO
+-rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)      554 2023-07-01 14:49:19.000000 epc-api-python-1.0.2/epc_api_python.egg-info/SOURCES.txt
+-rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)        1 2023-07-01 14:49:19.000000 epc-api-python-1.0.2/epc_api_python.egg-info/dependency_links.txt
+-rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)      117 2023-07-01 14:49:19.000000 epc-api-python-1.0.2/epc_api_python.egg-info/requires.txt
+-rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)        8 2023-07-01 14:49:19.000000 epc-api-python-1.0.2/epc_api_python.egg-info/top_level.txt
+drwxr-xr-x   0 khalimconn-kowlessar   (501) staff       (20)        0 2023-07-01 14:49:19.352119 epc-api-python-1.0.2/examples/
+-rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)      546 2023-05-10 15:11:57.000000 epc-api-python-1.0.2/examples/basic_example.py
+-rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)      411 2023-05-10 13:47:00.000000 epc-api-python-1.0.2/examples/csv_example.py
+-rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)     8744 2023-07-01 14:29:25.000000 epc-api-python-1.0.2/examples/investigating_recommendations.py
+-rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)     1880 2023-06-16 09:35:57.000000 epc-api-python-1.0.2/examples/test_script.py
+-rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)      473 2023-04-17 11:33:36.000000 epc-api-python-1.0.2/examples/zip_example.py
+-rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)     1127 2023-07-01 14:49:13.000000 epc-api-python-1.0.2/pyproject.toml
+drwxr-xr-x   0 khalimconn-kowlessar   (501) staff       (20)        0 2023-07-01 14:49:19.352405 epc-api-python-1.0.2/requirements/
+-rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)       45 2023-04-17 10:55:17.000000 epc-api-python-1.0.2/requirements/prod.txt
+-rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)       38 2023-07-01 14:49:19.353852 epc-api-python-1.0.2/setup.cfg
+-rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)       50 2023-04-17 11:24:27.000000 epc-api-python-1.0.2/setup.py
+drwxr-xr-x   0 khalimconn-kowlessar   (501) staff       (20)        0 2023-07-01 14:49:19.353147 epc-api-python-1.0.2/tests/
+-rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)     2462 2023-04-17 11:33:36.000000 epc-api-python-1.0.2/tests/test_client_init.py
+-rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)     3223 2023-04-17 11:33:36.000000 epc-api-python-1.0.2/tests/test_endpoints.py
+-rw-r--r--   0 khalimconn-kowlessar   (501) staff       (20)     2186 2023-04-17 11:33:36.000000 epc-api-python-1.0.2/tests/test_schema.py
```

### Comparing `epc-api-python-1.0.1/LICENSE` & `epc-api-python-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `epc-api-python-1.0.1/PKG-INFO` & `epc-api-python-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epc-api-python
-Version: 1.0.1
+Version: 1.0.2
 Summary: Interface the UK Govenment EPC api
 Author: Khalim Conn-Kowlessar
 License: Copyright (c) 2023 Khalim Conn-Kowlessar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `epc-api-python-1.0.1/README.md` & `epc-api-python-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `epc-api-python-1.0.1/epc_api/client.py` & `epc-api-python-1.0.2/epc_api/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,14 +145,17 @@
         self.headers = headers
 
     def _parse_response(self, response):
         """
         Given a successful response, this function parses the returned values
         """
         if self.headers["Accept"] == "application/json":
+            if not response.text:
+                # If we get an empty response, we return an empty object
+                return {}
             return response.json()
 
         # For other headers, we take the simple approach and allow the user to parse as they wish
         return response.content
 
     def call(self, method, url, params):
         response = getattr(requests, method)(
```

### Comparing `epc-api-python-1.0.1/epc_api/exceptions.py` & `epc-api-python-1.0.2/epc_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `epc-api-python-1.0.1/epc_api/schemas.py` & `epc-api-python-1.0.2/epc_api/schemas.py`

 * *Files identical despite different names*

### Comparing `epc-api-python-1.0.1/epc_api_python.egg-info/PKG-INFO` & `epc-api-python-1.0.2/epc_api_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epc-api-python
-Version: 1.0.1
+Version: 1.0.2
 Summary: Interface the UK Govenment EPC api
 Author: Khalim Conn-Kowlessar
 License: Copyright (c) 2023 Khalim Conn-Kowlessar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `epc-api-python-1.0.1/examples/basic_example.py` & `epc-api-python-1.0.2/examples/basic_example.py`

 * *Files identical despite different names*

### Comparing `epc-api-python-1.0.1/pyproject.toml` & `epc-api-python-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "epc-api-python"
-version = "1.0.1"
+version = "1.0.2"
 description = "Interface the UK Govenment EPC api"
 readme = "README.md"
 authors = [{ name = "Khalim Conn-Kowlessar" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -30,15 +30,15 @@
 dev = ["pytest>=6.2.3", "pytest-cov>=4.0.0", "black>=19.10b0", "isort", "prospector"]
 
 [project.urls]
 Homepage = "https://github.com/KhalimCK/epc-api-python"
 
 
 [tool.bumpver]
-current_version = "1.0.1"
+current_version = "1.0.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `epc-api-python-1.0.1/tests/test_client_init.py` & `epc-api-python-1.0.2/tests/test_client_init.py`

 * *Files identical despite different names*

### Comparing `epc-api-python-1.0.1/tests/test_endpoints.py` & `epc-api-python-1.0.2/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `epc-api-python-1.0.1/tests/test_schema.py` & `epc-api-python-1.0.2/tests/test_schema.py`

 * *Files identical despite different names*

