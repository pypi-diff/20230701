# Comparing `tmp/drmmsdk-0.0.2.tar.gz` & `tmp/drmmsdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drmmsdk-0.0.2.tar", last modified: Fri Jun 30 22:53:02 2023, max compression
+gzip compressed data, was "drmmsdk-0.0.3.tar", last modified: Fri Jun 30 22:58:11 2023, max compression
```

## Comparing `drmmsdk-0.0.2.tar` & `drmmsdk-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:53:02.181232 drmmsdk-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-30 22:52:51.000000 drmmsdk-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-30 22:52:51.000000 drmmsdk-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-30 22:53:02.181232 drmmsdk-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-30 22:52:51.000000 drmmsdk-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:53:02.177232 drmmsdk-0.0.2/drmmsdk/
--rw-r--r--   0 runner    (1001) docker     (123)    36639 2023-06-30 22:52:51.000000 drmmsdk-0.0.2/drmmsdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:53:02.181232 drmmsdk-0.0.2/drmmsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-30 22:53:02.000000 drmmsdk-0.0.2/drmmsdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-30 22:53:02.000000 drmmsdk-0.0.2/drmmsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:53:02.000000 drmmsdk-0.0.2/drmmsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-30 22:53:02.000000 drmmsdk-0.0.2/drmmsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 22:53:02.000000 drmmsdk-0.0.2/drmmsdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-30 22:52:51.000000 drmmsdk-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 22:52:51.000000 drmmsdk-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 22:53:02.181232 drmmsdk-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-30 22:52:51.000000 drmmsdk-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:58:11.520136 drmmsdk-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-30 22:58:01.000000 drmmsdk-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-30 22:58:01.000000 drmmsdk-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-30 22:58:11.520136 drmmsdk-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-30 22:58:01.000000 drmmsdk-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:58:11.520136 drmmsdk-0.0.3/drmmsdk/
+-rw-r--r--   0 runner    (1001) docker     (123)    36639 2023-06-30 22:58:01.000000 drmmsdk-0.0.3/drmmsdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:58:11.520136 drmmsdk-0.0.3/drmmsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-30 22:58:11.000000 drmmsdk-0.0.3/drmmsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-30 22:58:11.000000 drmmsdk-0.0.3/drmmsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:58:11.000000 drmmsdk-0.0.3/drmmsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-30 22:58:11.000000 drmmsdk-0.0.3/drmmsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 22:58:11.000000 drmmsdk-0.0.3/drmmsdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-30 22:58:01.000000 drmmsdk-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 22:58:01.000000 drmmsdk-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 22:58:11.520136 drmmsdk-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-30 22:58:01.000000 drmmsdk-0.0.3/setup.py
```

### Comparing `drmmsdk-0.0.2/LICENSE` & `drmmsdk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `drmmsdk-0.0.2/PKG-INFO` & `drmmsdk-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drmmsdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: Datto RMM Unofficial Python SDK
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -22,14 +22,16 @@
 
 ## Usage
 
 Import the package in your Python script as follows:
 
 ```python
 import drmmsdk
+
+drmm = drmmsdk(api_key="your_api_key", api_secret="your_api_secret", server="your_server")
 ```
 
 ## Methods
 
 The SDK currently supports the following methods:
 
 1. `create_site()`: Creates a new site.
```

### Comparing `drmmsdk-0.0.2/README.md` & `drmmsdk-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 ## Usage
 
 Import the package in your Python script as follows:
 
 ```python
 import drmmsdk
+
+drmm = drmmsdk(api_key="your_api_key", api_secret="your_api_secret", server="your_server")
 ```
 
 ## Methods
 
 The SDK currently supports the following methods:
 
 1. `create_site()`: Creates a new site.
```

### Comparing `drmmsdk-0.0.2/drmmsdk/__init__.py` & `drmmsdk-0.0.3/drmmsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `drmmsdk-0.0.2/drmmsdk.egg-info/PKG-INFO` & `drmmsdk-0.0.3/drmmsdk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drmmsdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: Datto RMM Unofficial Python SDK
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -22,14 +22,16 @@
 
 ## Usage
 
 Import the package in your Python script as follows:
 
 ```python
 import drmmsdk
+
+drmm = drmmsdk(api_key="your_api_key", api_secret="your_api_secret", server="your_server")
 ```
 
 ## Methods
 
 The SDK currently supports the following methods:
 
 1. `create_site()`: Creates a new site.
```

### Comparing `drmmsdk-0.0.2/setup.py` & `drmmsdk-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 with open(os.path.join(this_directory, "requirements.txt")) as f:
     requirements = f.read().splitlines()
 
 
 setup(
     name="drmmsdk",
-    version="0.0.2",
+    version="0.0.3",
     description="Datto RMM Unofficial Python SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Josh XT",
     author_email="josh@devxt.com",
     packages=find_packages(),
     python_requires=">=3.10",
```

