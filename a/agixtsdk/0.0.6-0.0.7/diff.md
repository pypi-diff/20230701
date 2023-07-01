# Comparing `tmp/agixtsdk-0.0.6.tar.gz` & `tmp/agixtsdk-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixtsdk-0.0.6.tar", last modified: Fri Jun 30 04:29:39 2023, max compression
+gzip compressed data, was "agixtsdk-0.0.7.tar", last modified: Sat Jul  1 05:25:04 2023, max compression
```

## Comparing `agixtsdk-0.0.6.tar` & `agixtsdk-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:29:39.323001 agixtsdk-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-30 04:29:26.000000 agixtsdk-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-30 04:29:26.000000 agixtsdk-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-30 04:29:39.323001 agixtsdk-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-30 04:29:26.000000 agixtsdk-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:29:39.319001 agixtsdk-0.0.6/agixtsdk/
--rw-r--r--   0 runner    (1001) docker     (123)    16671 2023-06-30 04:29:26.000000 agixtsdk-0.0.6/agixtsdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 04:29:39.323001 agixtsdk-0.0.6/agixtsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-30 04:29:39.000000 agixtsdk-0.0.6/agixtsdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-30 04:29:39.000000 agixtsdk-0.0.6/agixtsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 04:29:39.000000 agixtsdk-0.0.6/agixtsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 04:29:39.000000 agixtsdk-0.0.6/agixtsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 04:29:39.000000 agixtsdk-0.0.6/agixtsdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-30 04:29:26.000000 agixtsdk-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 04:29:39.323001 agixtsdk-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-30 04:29:26.000000 agixtsdk-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:25:04.790227 agixtsdk-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-01 05:24:52.000000 agixtsdk-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-01 05:24:52.000000 agixtsdk-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-01 05:25:04.790227 agixtsdk-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-01 05:24:52.000000 agixtsdk-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:25:04.786227 agixtsdk-0.0.7/agixtsdk/
+-rw-r--r--   0 runner    (1001) docker     (123)    16656 2023-07-01 05:24:52.000000 agixtsdk-0.0.7/agixtsdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:25:04.790227 agixtsdk-0.0.7/agixtsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-01 05:25:04.000000 agixtsdk-0.0.7/agixtsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-01 05:25:04.000000 agixtsdk-0.0.7/agixtsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 05:25:04.000000 agixtsdk-0.0.7/agixtsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-01 05:25:04.000000 agixtsdk-0.0.7/agixtsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-01 05:25:04.000000 agixtsdk-0.0.7/agixtsdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-01 05:24:52.000000 agixtsdk-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 05:25:04.790227 agixtsdk-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-01 05:24:52.000000 agixtsdk-0.0.7/setup.py
```

### Comparing `agixtsdk-0.0.6/LICENSE` & `agixtsdk-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `agixtsdk-0.0.6/PKG-INFO` & `agixtsdk-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixtsdk
-Version: 0.0.6
+Version: 0.0.7
 Summary: The AGiXT SDK for Python.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixtsdk-0.0.6/README.md` & `agixtsdk-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `agixtsdk-0.0.6/agixtsdk/__init__.py` & `agixtsdk-0.0.7/agixtsdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -420,15 +420,15 @@
     def get_extension_settings(self) -> Dict[str, Any]:
         try:
             response = requests.get(f"{self.base_uri}/api/extensions/settings")
             return response.json()["extension_settings"]
         except requests.RequestException:
             return self.handle_error(response)
 
-    def get_extensions(self) -> List[tuple]:
+    def get_extensions(self):
         try:
             response = requests.get(f"{self.base_uri}/api/extensions")
             return response.json()["extensions"]
         except requests.RequestException:
             return self.handle_error(response)
 
     def get_command_args(self, command_name: str) -> Dict[str, Any]:
```

### Comparing `agixtsdk-0.0.6/agixtsdk.egg-info/PKG-INFO` & `agixtsdk-0.0.7/agixtsdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixtsdk
-Version: 0.0.6
+Version: 0.0.7
 Summary: The AGiXT SDK for Python.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixtsdk-0.0.6/setup.py` & `agixtsdk-0.0.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Read the contents of your README file
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="agixtsdk",
-    version="0.0.6",
+    version="0.0.7",
     description="The AGiXT SDK for Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Josh XT",
     author_email="josh@devxt.com",
     packages=find_packages(),
     python_requires=">=3.10",
```

