# Comparing `tmp/lokzzpylibrary-0.1.dev14.tar.gz` & `tmp/lokzzpylibrary-0.1.dev15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lokzzpylibrary-0.1.dev14.tar", last modified: Sat Jul  1 14:50:47 2023, max compression
+gzip compressed data, was "lokzzpylibrary-0.1.dev15.tar", last modified: Sat Jul  1 15:13:02 2023, max compression
```

## Comparing `lokzzpylibrary-0.1.dev14.tar` & `lokzzpylibrary-0.1.dev15.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 14:50:47.440094 lokzzpylibrary-0.1.dev14/
--rw-rw-rw-   0        0        0       67 2023-07-01 14:48:17.000000 lokzzpylibrary-0.1.dev14/.gitignore
--rw-rw-rw-   0        0        0      418 2023-07-01 14:50:47.439096 lokzzpylibrary-0.1.dev14/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-01 06:13:01.000000 lokzzpylibrary-0.1.dev14/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 14:50:47.432095 lokzzpylibrary-0.1.dev14/lib/
--rw-rw-rw-   0        0        0        0 2023-07-01 03:21:24.000000 lokzzpylibrary-0.1.dev14/lib/__init__.py
--rw-rw-rw-   0        0        0     1428 2023-07-01 03:05:38.000000 lokzzpylibrary-0.1.dev14/lib/library.py
-drwxrwxrwx   0        0        0        0 2023-07-01 14:50:47.438098 lokzzpylibrary-0.1.dev14/lokzzpylibrary.egg-info/
--rw-rw-rw-   0        0        0      418 2023-07-01 14:50:47.000000 lokzzpylibrary-0.1.dev14/lokzzpylibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-07-01 14:50:47.000000 lokzzpylibrary-0.1.dev14/lokzzpylibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 14:50:47.000000 lokzzpylibrary-0.1.dev14/lokzzpylibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-01 14:50:47.000000 lokzzpylibrary-0.1.dev14/lokzzpylibrary.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-01 14:50:47.000000 lokzzpylibrary-0.1.dev14/lokzzpylibrary.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      635 2023-07-01 14:50:36.000000 lokzzpylibrary-0.1.dev14/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-01 14:50:47.440094 lokzzpylibrary-0.1.dev14/setup.cfg
--rwxrwxrwx   0        0        0      108 2023-07-01 14:27:44.000000 lokzzpylibrary-0.1.dev14/upload.bat
+drwxrwxrwx   0        0        0        0 2023-07-01 15:13:02.516797 lokzzpylibrary-0.1.dev15/
+-rw-rw-rw-   0        0        0       67 2023-07-01 14:48:17.000000 lokzzpylibrary-0.1.dev15/.gitignore
+-rw-rw-rw-   0        0        0      418 2023-07-01 15:13:02.515798 lokzzpylibrary-0.1.dev15/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-01 06:13:01.000000 lokzzpylibrary-0.1.dev15/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 15:13:02.506797 lokzzpylibrary-0.1.dev15/lib/
+-rw-rw-rw-   0        0        0        0 2023-07-01 03:21:24.000000 lokzzpylibrary-0.1.dev15/lib/__init__.py
+-rw-rw-rw-   0        0        0     1428 2023-07-01 03:05:38.000000 lokzzpylibrary-0.1.dev15/lib/library.py
+drwxrwxrwx   0        0        0        0 2023-07-01 15:13:02.513796 lokzzpylibrary-0.1.dev15/lokzzpylibrary.egg-info/
+-rw-rw-rw-   0        0        0      418 2023-07-01 15:13:02.000000 lokzzpylibrary-0.1.dev15/lokzzpylibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-07-01 15:13:02.000000 lokzzpylibrary-0.1.dev15/lokzzpylibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 15:13:02.000000 lokzzpylibrary-0.1.dev15/lokzzpylibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-01 15:13:02.000000 lokzzpylibrary-0.1.dev15/lokzzpylibrary.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-01 15:13:02.000000 lokzzpylibrary-0.1.dev15/lokzzpylibrary.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      635 2023-07-01 14:50:36.000000 lokzzpylibrary-0.1.dev15/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-01 15:13:02.516797 lokzzpylibrary-0.1.dev15/setup.cfg
+-rwxrwxrwx   0        0        0      108 2023-07-01 14:27:44.000000 lokzzpylibrary-0.1.dev15/upload.bat
```

### Comparing `lokzzpylibrary-0.1.dev14/lib/library.py` & `lokzzpylibrary-0.1.dev15/lib/library.py`

 * *Files identical despite different names*

### Comparing `lokzzpylibrary-0.1.dev14/pyproject.toml` & `lokzzpylibrary-0.1.dev15/pyproject.toml`

 * *Files identical despite different names*

