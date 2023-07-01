# Comparing `tmp/maroon-0.1.0.tar.gz` & `tmp/maroon-0.1.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maroon-0.1.0.tar", max compression
+gzip compressed data, was "maroon-0.1.41.tar", max compression
```

## Comparing `maroon-0.1.0.tar` & `maroon-0.1.41.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0    35823 2023-07-01 06:02:26.934625 maroon-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2023-07-01 06:03:50.190151 maroon-0.1.0/maroon/__init__.py
--rw-r--r--   0        0        0      275 2023-07-01 06:14:20.622906 maroon-0.1.0/maroon/cli.py
--rw-r--r--   0        0        0      144 2023-07-01 06:14:20.617905 maroon-0.1.0/maroon/do_format.py
--rw-r--r--   0        0        0      394 2023-07-01 06:20:00.905889 maroon-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       59 2023-07-01 06:02:26.934625 maroon-0.1.0/README.md
--rw-r--r--   0        0        0      550 1970-01-01 00:00:00.000000 maroon-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-07-01 06:02:26.934625 maroon-0.1.41/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-01 06:03:50.190151 maroon-0.1.41/maroon/__init__.py
+-rw-r--r--   0        0        0      764 2023-07-01 08:15:28.879222 maroon-0.1.41/maroon/cli.py
+-rw-r--r--   0        0        0     2009 2023-07-01 07:53:25.527573 maroon-0.1.41/maroon/cue_parser.py
+-rw-r--r--   0        0        0      900 2023-07-01 07:36:46.611307 maroon-0.1.41/maroon/format.py
+-rw-r--r--   0        0        0     3714 2023-07-01 08:15:28.868221 maroon-0.1.41/maroon/transform.py
+-rw-r--r--   0        0        0      486 2023-07-01 08:23:34.070454 maroon-0.1.41/pyproject.toml
+-rw-r--r--   0        0        0      499 2023-07-01 08:22:59.818046 maroon-0.1.41/README.md
+-rw-r--r--   0        0        0     1142 1970-01-01 00:00:00.000000 maroon-0.1.41/PKG-INFO
```

### Comparing `maroon-0.1.0/LICENSE` & `maroon-0.1.41/LICENSE`

 * *Files identical despite different names*

