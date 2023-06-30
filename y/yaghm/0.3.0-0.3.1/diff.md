# Comparing `tmp/yaghm-0.3.0.tar.gz` & `tmp/yaghm-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaghm-0.3.0.tar", last modified: Tue Oct 26 04:37:46 2021, max compression
+gzip compressed data, was "yaghm-0.3.1.tar", last modified: Fri Jun 30 23:24:50 2023, max compression
```

## Comparing `yaghm-0.3.0.tar` & `yaghm-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,30 @@
-drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2021-10-26 04:37:46.941320 yaghm-0.3.0/
--rw-r--r--   0 chaim     (1000) chaim     (1000)     1057 2021-09-17 07:57:32.000000 yaghm-0.3.0/LICENSE
--rw-r--r--   0 chaim     (1000) chaim     (1000)     2366 2021-10-26 04:37:46.941320 yaghm-0.3.0/PKG-INFO
--rw-r--r--   0 chaim     (1000) chaim     (1000)     1916 2021-09-17 05:03:00.000000 yaghm-0.3.0/README.md
--rw-r--r--   0 chaim     (1000) chaim     (1000)       38 2021-10-26 04:37:46.941320 yaghm-0.3.0/setup.cfg
--rw-r--r--   0 chaim     (1000) chaim     (1000)      957 2021-10-26 04:37:37.000000 yaghm-0.3.0/setup.py
-drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2021-10-26 04:37:46.941320 yaghm-0.3.0/src/
-drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2021-10-26 04:37:46.941320 yaghm-0.3.0/src/yaghm/
--rw-r--r--   0 chaim     (1000) chaim     (1000)      317 2021-06-29 02:45:48.000000 yaghm-0.3.0/src/yaghm/__init__.py
--rw-r--r--   0 chaim     (1000) chaim     (1000)     1422 2021-10-26 04:37:37.000000 yaghm-0.3.0/src/yaghm/custom_command.py
--rw-r--r--   0 chaim     (1000) chaim     (1000)     1367 2021-06-29 02:45:48.000000 yaghm-0.3.0/src/yaghm/disable.py
--rw-r--r--   0 chaim     (1000) chaim     (1000)     3789 2021-10-26 04:37:37.000000 yaghm-0.3.0/src/yaghm/enable.py
--rw-r--r--   0 chaim     (1000) chaim     (1000)     1292 2021-09-17 07:35:40.000000 yaghm-0.3.0/src/yaghm/lib.py
--rw-r--r--   0 chaim     (1000) chaim     (1000)     1128 2021-06-29 02:45:48.000000 yaghm-0.3.0/src/yaghm/list_hooks.py
--rw-r--r--   0 chaim     (1000) chaim     (1000)      909 2021-09-17 07:35:40.000000 yaghm-0.3.0/src/yaghm/main.py
-drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2021-10-26 04:37:46.941320 yaghm-0.3.0/src/yaghm/templates/
--rw-r--r--   0 chaim     (1000) chaim     (1000)      504 2021-07-03 07:20:08.000000 yaghm-0.3.0/src/yaghm/templates/wrapper.jinja2
-drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2021-10-26 04:37:46.941320 yaghm-0.3.0/src/yaghm.egg-info/
--rw-r--r--   0 chaim     (1000) chaim     (1000)     2366 2021-10-26 04:37:46.000000 yaghm-0.3.0/src/yaghm.egg-info/PKG-INFO
--rw-r--r--   0 chaim     (1000) chaim     (1000)      411 2021-10-26 04:37:46.000000 yaghm-0.3.0/src/yaghm.egg-info/SOURCES.txt
--rw-r--r--   0 chaim     (1000) chaim     (1000)        1 2021-10-26 04:37:46.000000 yaghm-0.3.0/src/yaghm.egg-info/dependency_links.txt
--rw-r--r--   0 chaim     (1000) chaim     (1000)       43 2021-10-26 04:37:46.000000 yaghm-0.3.0/src/yaghm.egg-info/entry_points.txt
--rw-r--r--   0 chaim     (1000) chaim     (1000)       55 2021-10-26 04:37:46.000000 yaghm-0.3.0/src/yaghm.egg-info/requires.txt
--rw-r--r--   0 chaim     (1000) chaim     (1000)        6 2021-10-26 04:37:46.000000 yaghm-0.3.0/src/yaghm.egg-info/top_level.txt
+drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2023-06-30 23:24:50.912946 yaghm-0.3.1/
+-rw-r--r--   0 chaim     (1000) chaim     (1000)       38 2021-06-29 02:55:56.000000 yaghm-0.3.1/.gitignore
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     1057 2021-09-17 07:57:32.000000 yaghm-0.3.1/LICENSE
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     2329 2023-06-30 23:24:50.912946 yaghm-0.3.1/PKG-INFO
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     1916 2021-09-17 05:03:00.000000 yaghm-0.3.1/README.md
+drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2023-06-30 23:24:50.909613 yaghm-0.3.1/doc/
+-rw-r--r--   0 chaim     (1000) chaim     (1000)      902 2021-10-26 04:37:37.000000 yaghm-0.3.1/doc/config.md
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     1658 2021-06-29 02:45:48.000000 yaghm-0.3.1/doc/custom-hooks.md
+-rw-r--r--   0 chaim     (1000) chaim     (1000)      414 2021-09-17 07:35:40.000000 yaghm-0.3.1/doc/technical.md
+-rw-r--r--   0 chaim     (1000) chaim     (1000)       38 2023-06-30 23:24:50.912946 yaghm-0.3.1/setup.cfg
+-rw-r--r--   0 chaim     (1000) chaim     (1000)      980 2023-06-30 23:20:57.000000 yaghm-0.3.1/setup.py
+drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2023-06-30 23:24:50.909613 yaghm-0.3.1/src/
+drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2023-06-30 23:24:50.909613 yaghm-0.3.1/src/yaghm/
+-rw-r--r--   0 chaim     (1000) chaim     (1000)      317 2023-06-30 22:42:17.000000 yaghm-0.3.1/src/yaghm/__init__.py
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     1422 2023-06-30 22:42:17.000000 yaghm-0.3.1/src/yaghm/custom_command.py
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     1367 2023-06-30 22:42:17.000000 yaghm-0.3.1/src/yaghm/disable.py
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     3789 2023-06-30 22:42:17.000000 yaghm-0.3.1/src/yaghm/enable.py
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     1292 2023-06-30 22:42:17.000000 yaghm-0.3.1/src/yaghm/lib.py
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     1128 2023-06-30 22:42:17.000000 yaghm-0.3.1/src/yaghm/list_hooks.py
+-rw-r--r--   0 chaim     (1000) chaim     (1000)      909 2023-06-30 22:42:17.000000 yaghm-0.3.1/src/yaghm/main.py
+drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2023-06-30 23:24:50.912946 yaghm-0.3.1/src/yaghm/templates/
+-rw-r--r--   0 chaim     (1000) chaim     (1000)      504 2023-06-30 22:42:16.000000 yaghm-0.3.1/src/yaghm/templates/wrapper.jinja2
+drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2023-06-30 23:24:50.912946 yaghm-0.3.1/src/yaghm.egg-info/
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     2329 2023-06-30 23:24:50.000000 yaghm-0.3.1/src/yaghm.egg-info/PKG-INFO
+-rw-r--r--   0 chaim     (1000) chaim     (1000)      483 2023-06-30 23:24:50.000000 yaghm-0.3.1/src/yaghm.egg-info/SOURCES.txt
+-rw-r--r--   0 chaim     (1000) chaim     (1000)        1 2023-06-30 23:24:50.000000 yaghm-0.3.1/src/yaghm.egg-info/dependency_links.txt
+-rw-r--r--   0 chaim     (1000) chaim     (1000)       42 2023-06-30 23:24:50.000000 yaghm-0.3.1/src/yaghm.egg-info/entry_points.txt
+-rw-r--r--   0 chaim     (1000) chaim     (1000)       67 2023-06-30 23:24:50.000000 yaghm-0.3.1/src/yaghm.egg-info/requires.txt
+-rw-r--r--   0 chaim     (1000) chaim     (1000)        6 2023-06-30 23:24:50.000000 yaghm-0.3.1/src/yaghm.egg-info/top_level.txt
+-rw-r--r--   0 chaim     (1000) chaim     (1000)      602 2021-10-26 04:37:37.000000 yaghm-0.3.1/yaghm.yml
```

### Comparing `yaghm-0.3.0/LICENSE` & `yaghm-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yaghm-0.3.0/PKG-INFO` & `yaghm-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: yaghm
-Version: 0.3.0
+Version: 0.3.1
 Summary: Minimal git hook manager for the command line.
 Home-page: https://www.github.com/metov/yaghm
 Author: Azat Akhmetov
 Author-email: azatinfo@yandex.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Yet Another Git Hook Manager
@@ -52,9 +50,7 @@
 Install with `pip install yaghm`
 
 ## Further reading
 
 * [How it works](doc/technical.md)
 * [Config syntax](doc/config.md)
 * [Developing hooks](doc/custom-hooks.md)
-
-
```

### Comparing `yaghm-0.3.0/README.md` & `yaghm-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `yaghm-0.3.0/setup.py` & `yaghm-0.3.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from pathlib import Path
 
 from setuptools import find_packages
 
 setup(
     name="yaghm",
-    version="0.3.0",
+    version="0.3.1",
     description="Minimal git hook manager for the command line.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://www.github.com/metov/yaghm",
     author="Azat Akhmetov",
     author_email="azatinfo@yandex.com",
     classifiers=[
@@ -23,14 +23,15 @@
     install_requires=[
         "coloredlogs",
         "docopt",
         "GitPython",
         "Jinja2",
         "PyYAML",
         "questionary",
+        "ruamel.yaml",
     ],
     entry_points={
         "console_scripts": [
             "yaghm=yaghm.main:main",
         ],
     },
 )
```

### Comparing `yaghm-0.3.0/src/yaghm/custom_command.py` & `yaghm-0.3.1/src/yaghm/custom_command.py`

 * *Files identical despite different names*

### Comparing `yaghm-0.3.0/src/yaghm/disable.py` & `yaghm-0.3.1/src/yaghm/disable.py`

 * *Files identical despite different names*

### Comparing `yaghm-0.3.0/src/yaghm/enable.py` & `yaghm-0.3.1/src/yaghm/enable.py`

 * *Files identical despite different names*

### Comparing `yaghm-0.3.0/src/yaghm/lib.py` & `yaghm-0.3.1/src/yaghm/lib.py`

 * *Files identical despite different names*

### Comparing `yaghm-0.3.0/src/yaghm/list_hooks.py` & `yaghm-0.3.1/src/yaghm/list_hooks.py`

 * *Files identical despite different names*

### Comparing `yaghm-0.3.0/src/yaghm/main.py` & `yaghm-0.3.1/src/yaghm/main.py`

 * *Files identical despite different names*

### Comparing `yaghm-0.3.0/src/yaghm.egg-info/PKG-INFO` & `yaghm-0.3.1/src/yaghm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: yaghm
-Version: 0.3.0
+Version: 0.3.1
 Summary: Minimal git hook manager for the command line.
 Home-page: https://www.github.com/metov/yaghm
 Author: Azat Akhmetov
 Author-email: azatinfo@yandex.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Yet Another Git Hook Manager
@@ -52,9 +50,7 @@
 Install with `pip install yaghm`
 
 ## Further reading
 
 * [How it works](doc/technical.md)
 * [Config syntax](doc/config.md)
 * [Developing hooks](doc/custom-hooks.md)
-
-
```

