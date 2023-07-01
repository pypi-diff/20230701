# Comparing `tmp/f_dpi-0.0.1.tar.gz` & `tmp/f_dpi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f_dpi-0.0.1.tar", last modified: Sat Jul  1 06:27:46 2023, max compression
+gzip compressed data, was "f_dpi-0.0.2.tar", last modified: Sat Jul  1 06:30:40 2023, max compression
```

## Comparing `f_dpi-0.0.1.tar` & `f_dpi-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 06:27:46.980937 f_dpi-0.0.1/
--rw-rw-rw-   0        0        0      147 2023-07-01 06:27:46.981946 f_dpi-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-04-17 20:39:54.000000 f_dpi-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 06:27:46.969824 f_dpi-0.0.1/f_dpi/
--rw-rw-rw-   0        0        0       62 2023-07-01 06:26:53.000000 f_dpi-0.0.1/f_dpi/__init__.py
--rw-rw-rw-   0        0        0       21 2023-04-17 20:49:44.000000 f_dpi-0.0.1/f_dpi/__version__.py
--rw-rw-rw-   0        0        0     1407 2023-06-02 02:16:18.000000 f_dpi-0.0.1/f_dpi/f_dpi.py
-drwxrwxrwx   0        0        0        0 2023-07-01 06:27:46.980937 f_dpi-0.0.1/f_dpi.egg-info/
--rw-rw-rw-   0        0        0      147 2023-07-01 06:27:46.000000 f_dpi-0.0.1/f_dpi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-07-01 06:27:46.000000 f_dpi-0.0.1/f_dpi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 06:27:46.000000 f_dpi-0.0.1/f_dpi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-01 06:27:46.000000 f_dpi-0.0.1/f_dpi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-01 06:27:46.982948 f_dpi-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      432 2023-07-01 06:27:38.000000 f_dpi-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 06:30:40.564767 f_dpi-0.0.2/
+-rw-rw-rw-   0        0        0      147 2023-07-01 06:30:40.564767 f_dpi-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-04-17 20:39:54.000000 f_dpi-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 06:30:40.550089 f_dpi-0.0.2/f_dpi/
+-rw-rw-rw-   0        0        0       62 2023-07-01 06:26:53.000000 f_dpi-0.0.2/f_dpi/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-07-01 06:30:13.000000 f_dpi-0.0.2/f_dpi/__version__.py
+-rw-rw-rw-   0        0        0     1407 2023-06-02 02:16:18.000000 f_dpi-0.0.2/f_dpi/f_dpi.py
+drwxrwxrwx   0        0        0        0 2023-07-01 06:30:40.563767 f_dpi-0.0.2/f_dpi.egg-info/
+-rw-rw-rw-   0        0        0      147 2023-07-01 06:30:40.000000 f_dpi-0.0.2/f_dpi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-07-01 06:30:40.000000 f_dpi-0.0.2/f_dpi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 06:30:40.000000 f_dpi-0.0.2/f_dpi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-07-01 06:30:40.000000 f_dpi-0.0.2/f_dpi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-01 06:30:40.000000 f_dpi-0.0.2/f_dpi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-01 06:30:40.565767 f_dpi-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      457 2023-07-01 06:30:22.000000 f_dpi-0.0.2/setup.py
```

### Comparing `f_dpi-0.0.1/f_dpi/f_dpi.py` & `f_dpi-0.0.2/f_dpi/f_dpi.py`

 * *Files identical despite different names*

