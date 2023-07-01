# Comparing `tmp/lokzz--pylibrary-1.0.tar.gz` & `tmp/lokzz-pylibrary-1.0.0.0.0.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lokzz--pylibrary-1.0.tar", last modified: Sat Jul  1 06:05:30 2023, max compression
+gzip compressed data, was "lokzz-pylibrary-1.0.0.0.0.0.0.1.tar", last modified: Sat Jul  1 14:28:54 2023, max compression
```

## Comparing `lokzz--pylibrary-1.0.tar` & `lokzz-pylibrary-1.0.0.0.0.0.0.1.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 06:05:30.816876 lokzz--pylibrary-1.0/
--rw-rw-rw-   0        0        0       35 2023-07-01 06:02:41.000000 lokzz--pylibrary-1.0/.gitignore
--rw-rw-rw-   0        0        0      490 2023-07-01 06:05:30.816876 lokzz--pylibrary-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      118 2023-07-01 05:58:38.000000 lokzz--pylibrary-1.0/README.md
--rw-rw-rw-   0        0        0        0 2023-07-01 04:25:02.000000 lokzz--pylibrary-1.0/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 06:05:30.810875 lokzz--pylibrary-1.0/lib/
--rw-rw-rw-   0        0        0        0 2023-07-01 03:21:24.000000 lokzz--pylibrary-1.0/lib/__init__.py
--rw-rw-rw-   0        0        0     1428 2023-07-01 03:05:38.000000 lokzz--pylibrary-1.0/lib/library.py
-drwxrwxrwx   0        0        0        0 2023-07-01 06:05:30.815876 lokzz--pylibrary-1.0/lokzz_pylibrary.egg-info/
--rw-rw-rw-   0        0        0      489 2023-07-01 06:05:30.000000 lokzz--pylibrary-1.0/lokzz_pylibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-07-01 06:05:30.000000 lokzz--pylibrary-1.0/lokzz_pylibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 06:05:30.000000 lokzz--pylibrary-1.0/lokzz_pylibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-01 06:05:30.000000 lokzz--pylibrary-1.0/lokzz_pylibrary.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-01 06:05:30.000000 lokzz--pylibrary-1.0/lokzz_pylibrary.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      545 2023-07-01 05:28:11.000000 lokzz--pylibrary-1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-01 06:05:30.817875 lokzz--pylibrary-1.0/setup.cfg
--rwxrwxrwx   0        0        0       88 2023-07-01 06:05:30.000000 lokzz--pylibrary-1.0/upload.bat
+drwxrwxrwx   0        0        0        0 2023-07-01 14:28:54.842692 lokzz-pylibrary-1.0.0.0.0.0.0.1/
+-rw-rw-rw-   0        0        0       56 2023-07-01 06:24:03.000000 lokzz-pylibrary-1.0.0.0.0.0.0.1/.gitignore
+-rw-rw-rw-   0        0        0      425 2023-07-01 14:28:54.842692 lokzz-pylibrary-1.0.0.0.0.0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-01 06:13:01.000000 lokzz-pylibrary-1.0.0.0.0.0.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 14:28:54.835692 lokzz-pylibrary-1.0.0.0.0.0.0.1/lib/
+-rw-rw-rw-   0        0        0        0 2023-07-01 03:21:24.000000 lokzz-pylibrary-1.0.0.0.0.0.0.1/lib/__init__.py
+-rw-rw-rw-   0        0        0     1428 2023-07-01 03:05:38.000000 lokzz-pylibrary-1.0.0.0.0.0.0.1/lib/library.py
+drwxrwxrwx   0        0        0        0 2023-07-01 14:28:54.841693 lokzz-pylibrary-1.0.0.0.0.0.0.1/lokzz_pylibrary.egg-info/
+-rw-rw-rw-   0        0        0      425 2023-07-01 14:28:54.000000 lokzz-pylibrary-1.0.0.0.0.0.0.1/lokzz_pylibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-07-01 14:28:54.000000 lokzz-pylibrary-1.0.0.0.0.0.0.1/lokzz_pylibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 14:28:54.000000 lokzz-pylibrary-1.0.0.0.0.0.0.1/lokzz_pylibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-01 14:28:54.000000 lokzz-pylibrary-1.0.0.0.0.0.0.1/lokzz_pylibrary.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-01 14:28:54.000000 lokzz-pylibrary-1.0.0.0.0.0.0.1/lokzz_pylibrary.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      556 2023-07-01 14:28:44.000000 lokzz-pylibrary-1.0.0.0.0.0.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-01 14:28:54.842692 lokzz-pylibrary-1.0.0.0.0.0.0.1/setup.cfg
+-rwxrwxrwx   0        0        0      108 2023-07-01 14:27:44.000000 lokzz-pylibrary-1.0.0.0.0.0.0.1/upload.bat
```

### Comparing `lokzz--pylibrary-1.0/lib/library.py` & `lokzz-pylibrary-1.0.0.0.0.0.0.1/lib/library.py`

 * *Files identical despite different names*

### Comparing `lokzz--pylibrary-1.0/pyproject.toml` & `lokzz-pylibrary-1.0.0.0.0.0.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
-name = "lokzz--pylibrary"
-version = "1.0"
+name = "lokzz-pylibrary"
+version = "1.0.0.0.0.0.0.1"
 authors = [
     { name="lokzz", email="lokzz@github.com" },
 ]
 description = "personal library"
 readme = "README.md"
 license = {text = "BSD-3-Clause"}
 requires-python = ">=3.10.7"
```

