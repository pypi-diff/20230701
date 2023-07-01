# Comparing `tmp/tech-ninja-tistory-api-1.0.2.tar.gz` & `tmp/tech-ninja-tistory-api-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tech-ninja-tistory-api-1.0.2.tar", last modified: Sat Jul  1 13:55:52 2023, max compression
+gzip compressed data, was "dist\tech-ninja-tistory-api-1.0.3.tar", last modified: Sat Jul  1 13:59:35 2023, max compression
```

## Comparing `tech-ninja-tistory-api-1.0.2.tar` & `tech-ninja-tistory-api-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 13:55:52.000000 tech-ninja-tistory-api-1.0.2/
--rw-rw-rw-   0        0        0     1542 2023-07-01 13:55:52.000000 tech-ninja-tistory-api-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      183 2023-07-01 05:46:37.000000 tech-ninja-tistory-api-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      707 2023-07-01 06:24:29.000000 tech-ninja-tistory-api-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-01 13:55:52.000000 tech-ninja-tistory-api-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      975 2023-07-01 13:55:42.000000 tech-ninja-tistory-api-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 13:55:52.000000 tech-ninja-tistory-api-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-01 13:55:52.000000 tech-ninja-tistory-api-1.0.2/src/tech_ninja_tistory_api/
--rw-rw-rw-   0        0        0     7960 2023-07-01 06:22:48.000000 tech-ninja-tistory-api-1.0.2/src/tech_ninja_tistory_api/tistory_api.py
--rw-rw-rw-   0        0        0       35 2023-07-01 06:21:35.000000 tech-ninja-tistory-api-1.0.2/src/tech_ninja_tistory_api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 13:55:52.000000 tech-ninja-tistory-api-1.0.2/src/tech_ninja_tistory_api.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-01 13:55:52.000000 tech-ninja-tistory-api-1.0.2/src/tech_ninja_tistory_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1542 2023-07-01 13:55:52.000000 tech-ninja-tistory-api-1.0.2/src/tech_ninja_tistory_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       35 2023-07-01 13:55:52.000000 tech-ninja-tistory-api-1.0.2/src/tech_ninja_tistory_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0      363 2023-07-01 13:55:52.000000 tech-ninja-tistory-api-1.0.2/src/tech_ninja_tistory_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       23 2023-07-01 13:55:52.000000 tech-ninja-tistory-api-1.0.2/src/tech_ninja_tistory_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 13:59:35.000000 tech-ninja-tistory-api-1.0.3/
+-rw-rw-rw-   0        0        0     1542 2023-07-01 13:59:35.000000 tech-ninja-tistory-api-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2023-07-01 05:46:37.000000 tech-ninja-tistory-api-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      707 2023-07-01 06:24:29.000000 tech-ninja-tistory-api-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-01 13:59:35.000000 tech-ninja-tistory-api-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      968 2023-07-01 13:59:04.000000 tech-ninja-tistory-api-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 13:59:35.000000 tech-ninja-tistory-api-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-01 13:59:35.000000 tech-ninja-tistory-api-1.0.3/src/tech_ninja_tistory_api/
+-rw-rw-rw-   0        0        0     7960 2023-07-01 06:22:48.000000 tech-ninja-tistory-api-1.0.3/src/tech_ninja_tistory_api/tistory_api.py
+-rw-rw-rw-   0        0        0       35 2023-07-01 06:21:35.000000 tech-ninja-tistory-api-1.0.3/src/tech_ninja_tistory_api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 13:59:35.000000 tech-ninja-tistory-api-1.0.3/src/tech_ninja_tistory_api.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-01 13:59:35.000000 tech-ninja-tistory-api-1.0.3/src/tech_ninja_tistory_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1542 2023-07-01 13:59:35.000000 tech-ninja-tistory-api-1.0.3/src/tech_ninja_tistory_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-07-01 13:59:35.000000 tech-ninja-tistory-api-1.0.3/src/tech_ninja_tistory_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      363 2023-07-01 13:59:35.000000 tech-ninja-tistory-api-1.0.3/src/tech_ninja_tistory_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       23 2023-07-01 13:59:35.000000 tech-ninja-tistory-api-1.0.3/src/tech_ninja_tistory_api.egg-info/top_level.txt
```

### Comparing `tech-ninja-tistory-api-1.0.2/PKG-INFO` & `tech-ninja-tistory-api-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tech-ninja-tistory-api
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tistory API Wrapper
 Home-page: https://github.com/yscho03/tech-ninja-tistory-api
 Author: yscho03
 Author-email: yscho03.developer@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/yscho03/tech-ninja-tistory-api/issues
 Description: # Tistory API Wrapper
```

### Comparing `tech-ninja-tistory-api-1.0.2/README.md` & `tech-ninja-tistory-api-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tech-ninja-tistory-api-1.0.2/setup.py` & `tech-ninja-tistory-api-1.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tech-ninja-tistory-api",
-    version="1.0.2",
+    version="1.0.3",
     author="yscho03",
     author_email="yscho03.developer@gmail.com",
     description="Tistory API Wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yscho03/tech-ninja-tistory-api",
     project_urls={
@@ -20,12 +20,12 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
     install_requires=[
-        "requests>=2.13, <2.20",
+        "requests>=2.24",
         "urllib3>=1.26",
     ],    
     dist_dir='dist',    
 )
```

### Comparing `tech-ninja-tistory-api-1.0.2/src/tech_ninja_tistory_api/tistory_api.py` & `tech-ninja-tistory-api-1.0.3/src/tech_ninja_tistory_api/tistory_api.py`

 * *Files identical despite different names*

### Comparing `tech-ninja-tistory-api-1.0.2/src/tech_ninja_tistory_api.egg-info/PKG-INFO` & `tech-ninja-tistory-api-1.0.3/src/tech_ninja_tistory_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tech-ninja-tistory-api
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tistory API Wrapper
 Home-page: https://github.com/yscho03/tech-ninja-tistory-api
 Author: yscho03
 Author-email: yscho03.developer@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/yscho03/tech-ninja-tistory-api/issues
 Description: # Tistory API Wrapper
```

