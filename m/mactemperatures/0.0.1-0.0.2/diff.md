# Comparing `tmp/mactemperatures-0.0.1.tar.gz` & `tmp/mactemperatures-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/joshua/Developer/MacTemperatures/dist/tmpm8i4izxf/mactemperatures-0.0.1.tar", last modified: Sun Jun  5 19:06:51 2022, max compression
+gzip compressed data, was "mactemperatures-0.0.2.tar", last modified: Sat Jul  1 16:29:59 2023, max compression
```

## Comparing `mactemperatures-0.0.1.tar` & `mactemperatures-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2022-06-05 19:06:51.000000 mactemperatures-0.0.1/
--rw-r--r--   0 joshua     (501) staff       (20)     1069 2022-06-05 17:58:03.000000 mactemperatures-0.0.1/LICENSE
--rw-r--r--   0 joshua     (501) staff       (20)      991 2022-06-05 19:06:51.000000 mactemperatures-0.0.1/PKG-INFO
--rw-r--r--   0 joshua     (501) staff       (20)      400 2022-06-05 18:47:53.000000 mactemperatures-0.0.1/README.md
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2022-06-05 19:06:51.000000 mactemperatures-0.0.1/mactemperatures/
--rw-r--r--   0 joshua     (501) staff       (20)       38 2022-06-05 18:30:15.000000 mactemperatures-0.0.1/mactemperatures/__init__.py
--rw-r--r--   0 joshua     (501) staff       (20)      538 2022-06-05 18:31:40.000000 mactemperatures-0.0.1/mactemperatures/core.py
--rw-r--r--   0 joshua     (501) staff       (20)      166 2022-06-05 18:14:57.000000 mactemperatures-0.0.1/mactemperatures/exceptions.py
--rw-r--r--   0 joshua     (501) staff       (20)     5228 2022-06-05 19:06:06.000000 mactemperatures-0.0.1/mactemperatures/sensors.c
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2022-06-05 19:06:51.000000 mactemperatures-0.0.1/mactemperatures.egg-info/
--rw-r--r--   0 joshua     (501) staff       (20)      991 2022-06-05 19:06:50.000000 mactemperatures-0.0.1/mactemperatures.egg-info/PKG-INFO
--rw-r--r--   0 joshua     (501) staff       (20)      290 2022-06-05 19:06:51.000000 mactemperatures-0.0.1/mactemperatures.egg-info/SOURCES.txt
--rw-r--r--   0 joshua     (501) staff       (20)        1 2022-06-05 19:06:50.000000 mactemperatures-0.0.1/mactemperatures.egg-info/dependency_links.txt
--rw-r--r--   0 joshua     (501) staff       (20)       27 2022-06-05 19:06:51.000000 mactemperatures-0.0.1/mactemperatures.egg-info/top_level.txt
--rw-r--r--   0 joshua     (501) staff       (20)       38 2022-06-05 19:06:51.000000 mactemperatures-0.0.1/setup.cfg
--rw-r--r--   0 joshua     (501) staff       (20)     1349 2022-06-05 19:06:17.000000 mactemperatures-0.0.1/setup.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-07-01 16:29:59.505423 mactemperatures-0.0.2/
+-rw-r--r--   0 joshua     (501) staff       (20)     1069 2023-07-01 16:21:52.000000 mactemperatures-0.0.2/LICENSE
+-rw-r--r--   0 joshua     (501) staff       (20)     1043 2023-07-01 16:29:59.505282 mactemperatures-0.0.2/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)      450 2023-07-01 16:22:51.000000 mactemperatures-0.0.2/README.md
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-07-01 16:29:59.504371 mactemperatures-0.0.2/mactemperatures/
+-rw-r--r--   0 joshua     (501) staff       (20)       38 2023-07-01 16:21:52.000000 mactemperatures-0.0.2/mactemperatures/__init__.py
+-rw-r--r--   0 joshua     (501) staff       (20)      538 2023-07-01 16:21:52.000000 mactemperatures-0.0.2/mactemperatures/core.py
+-rw-r--r--   0 joshua     (501) staff       (20)      166 2023-07-01 16:21:52.000000 mactemperatures-0.0.2/mactemperatures/exceptions.py
+-rw-r--r--   0 joshua     (501) staff       (20)     5228 2023-07-01 16:21:52.000000 mactemperatures-0.0.2/mactemperatures/sensors.c
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2023-07-01 16:29:59.505084 mactemperatures-0.0.2/mactemperatures.egg-info/
+-rw-r--r--   0 joshua     (501) staff       (20)     1043 2023-07-01 16:29:59.000000 mactemperatures-0.0.2/mactemperatures.egg-info/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)      290 2023-07-01 16:29:59.000000 mactemperatures-0.0.2/mactemperatures.egg-info/SOURCES.txt
+-rw-r--r--   0 joshua     (501) staff       (20)        1 2023-07-01 16:29:59.000000 mactemperatures-0.0.2/mactemperatures.egg-info/dependency_links.txt
+-rw-r--r--   0 joshua     (501) staff       (20)       27 2023-07-01 16:29:59.000000 mactemperatures-0.0.2/mactemperatures.egg-info/top_level.txt
+-rw-r--r--   0 joshua     (501) staff       (20)       38 2023-07-01 16:29:59.505466 mactemperatures-0.0.2/setup.cfg
+-rw-r--r--   0 joshua     (501) staff       (20)     1120 2023-07-01 16:29:49.000000 mactemperatures-0.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mactemperatures-0.0.1/LICENSE` & `mactemperatures-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mactemperatures-0.0.1/mactemperatures/core.py` & `mactemperatures-0.0.2/mactemperatures/core.py`

 * *Files identical despite different names*

### Comparing `mactemperatures-0.0.1/mactemperatures/sensors.c` & `mactemperatures-0.0.2/mactemperatures/sensors.c`

 * *Files identical despite different names*

### Comparing `mactemperatures-0.0.1/setup.py` & `mactemperatures-0.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,37 +4,34 @@
 os.environ['LDFLAGS'] = '-framework IOKit -framework Foundation'
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 setuptools.setup(
     name = "mactemperatures",
-    version = "0.0.1",
+    version = "0.0.2",
     author="Joshua Unrau",
     author_email="contact@joshuaunrau.com",
     description="Python Package for Obtaining Temperature Sensor Readings on M1 Macs",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/joshunrau/MacTemperatures",
+    url="https://github.com/joshunrau/mac-temperatures",
     project_urls={
-        "Bug Tracker": "https://github.com/joshunrau/MacTemperatures/issues",
+        "Bug Tracker": "https://github.com/joshunrau/mac-temperatures/issues",
     },
     classifiers=[
         "Programming Language :: C",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: MacOS",
     ],
     packages=setuptools.find_packages(where="."),
     python_requires=">=3.7",
     ext_modules = [
         setuptools.Extension(
             name="macsensors", 
             sources=[
                 os.path.join('mactemperatures', 'sensors.c')
-                #os.path.join('mactemperatures', "macsensors", 'bindings.c'),
-                #os.path.join('mactemperatures', "macsensors", 'sensors.c'),
-                #os.path.join('mactemperatures', "macsensors", 'sensors.h')
             ]
         )
     ]
 )
```

