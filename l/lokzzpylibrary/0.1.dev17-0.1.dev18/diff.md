# Comparing `tmp/lokzzpylibrary-0.1.dev17.tar.gz` & `tmp/lokzzpylibrary-0.1.dev18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lokzzpylibrary-0.1.dev17.tar", last modified: Sat Jul  1 15:32:10 2023, max compression
+gzip compressed data, was "lokzzpylibrary-0.1.dev18.tar", last modified: Sat Jul  1 15:50:23 2023, max compression
```

## Comparing `lokzzpylibrary-0.1.dev17.tar` & `lokzzpylibrary-0.1.dev18.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 15:32:10.898737 lokzzpylibrary-0.1.dev17/
--rw-rw-rw-   0        0        0       67 2023-07-01 14:48:17.000000 lokzzpylibrary-0.1.dev17/.gitignore
--rw-rw-rw-   0        0        0        9 2023-07-01 15:31:36.000000 lokzzpylibrary-0.1.dev17/MANIFEST.in
--rw-rw-rw-   0        0        0      418 2023-07-01 15:32:10.897736 lokzzpylibrary-0.1.dev17/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-01 06:13:01.000000 lokzzpylibrary-0.1.dev17/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 15:32:10.891737 lokzzpylibrary-0.1.dev17/lib/
--rw-rw-rw-   0        0        0        0 2023-07-01 03:21:24.000000 lokzzpylibrary-0.1.dev17/lib/__init__.py
--rw-rw-rw-   0        0        0     1428 2023-07-01 03:05:38.000000 lokzzpylibrary-0.1.dev17/lib/library.py
-drwxrwxrwx   0        0        0        0 2023-07-01 15:32:10.897736 lokzzpylibrary-0.1.dev17/lokzzpylibrary.egg-info/
--rw-rw-rw-   0        0        0      418 2023-07-01 15:32:10.000000 lokzzpylibrary-0.1.dev17/lokzzpylibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-07-01 15:32:10.000000 lokzzpylibrary-0.1.dev17/lokzzpylibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 15:32:10.000000 lokzzpylibrary-0.1.dev17/lokzzpylibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-01 15:32:10.000000 lokzzpylibrary-0.1.dev17/lokzzpylibrary.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-01 15:32:10.000000 lokzzpylibrary-0.1.dev17/lokzzpylibrary.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      635 2023-07-01 15:18:31.000000 lokzzpylibrary-0.1.dev17/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-01 15:32:10.898737 lokzzpylibrary-0.1.dev17/setup.cfg
--rwxrwxrwx   0        0        0      108 2023-07-01 14:27:44.000000 lokzzpylibrary-0.1.dev17/upload.bat
+drwxrwxrwx   0        0        0        0 2023-07-01 15:50:23.397061 lokzzpylibrary-0.1.dev18/
+-rw-rw-rw-   0        0        0       67 2023-07-01 14:48:17.000000 lokzzpylibrary-0.1.dev18/.gitignore
+-rw-rw-rw-   0        0        0       24 2023-07-01 15:36:20.000000 lokzzpylibrary-0.1.dev18/MANIFEST.in
+-rw-rw-rw-   0        0        0      418 2023-07-01 15:50:23.396062 lokzzpylibrary-0.1.dev18/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-01 06:13:01.000000 lokzzpylibrary-0.1.dev18/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 15:50:23.390060 lokzzpylibrary-0.1.dev18/lib/
+-rw-rw-rw-   0        0        0        0 2023-07-01 03:21:24.000000 lokzzpylibrary-0.1.dev18/lib/__init__.py
+-rw-rw-rw-   0        0        0     1428 2023-07-01 03:05:38.000000 lokzzpylibrary-0.1.dev18/lib/library.py
+drwxrwxrwx   0        0        0        0 2023-07-01 15:50:23.395060 lokzzpylibrary-0.1.dev18/lokzzpylibrary.egg-info/
+-rw-rw-rw-   0        0        0      418 2023-07-01 15:50:23.000000 lokzzpylibrary-0.1.dev18/lokzzpylibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-07-01 15:50:23.000000 lokzzpylibrary-0.1.dev18/lokzzpylibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 15:50:23.000000 lokzzpylibrary-0.1.dev18/lokzzpylibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-01 15:50:23.000000 lokzzpylibrary-0.1.dev18/lokzzpylibrary.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-01 15:50:23.000000 lokzzpylibrary-0.1.dev18/lokzzpylibrary.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      635 2023-07-01 15:38:44.000000 lokzzpylibrary-0.1.dev18/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-01 15:50:23.397061 lokzzpylibrary-0.1.dev18/setup.cfg
+-rwxrwxrwx   0        0        0      108 2023-07-01 14:27:44.000000 lokzzpylibrary-0.1.dev18/upload.bat
```

### Comparing `lokzzpylibrary-0.1.dev17/lib/library.py` & `lokzzpylibrary-0.1.dev18/lib/library.py`

 * *Files identical despite different names*

### Comparing `lokzzpylibrary-0.1.dev17/pyproject.toml` & `lokzzpylibrary-0.1.dev18/pyproject.toml`

 * *Files identical despite different names*

