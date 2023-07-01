# Comparing `tmp/zeugvars-0.1.0.tar.gz` & `tmp/zeugvars-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeugvars-0.1.0.tar", max compression
+gzip compressed data, was "zeugvars-0.1.1.tar", max compression
```

## Comparing `zeugvars-0.1.0.tar` & `zeugvars-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1083 2023-06-29 20:37:00.152930 zeugvars-0.1.0/LICENSE
--rw-r--r--   0        0        0      389 2023-07-01 08:25:42.317874 zeugvars-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       86 2023-06-29 20:37:00.154924 zeugvars-0.1.0/README.md
--rw-r--r--   0        0        0    10817 2023-07-01 09:30:32.668712 zeugvars-0.1.0/zeugvars.py
--rw-r--r--   0        0        0      415 1970-01-01 00:00:00.000000 zeugvars-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-29 20:37:00.152930 zeugvars-0.1.1/LICENSE
+-rw-r--r--   0        0        0      438 2023-07-01 10:17:58.043297 zeugvars-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       86 2023-06-29 20:37:00.154924 zeugvars-0.1.1/README.md
+-rw-r--r--   0        0        0    10817 2023-07-01 10:01:32.143374 zeugvars-0.1.1/zeugvars.py
+-rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 zeugvars-0.1.1/PKG-INFO
```

### Comparing `zeugvars-0.1.0/LICENSE` & `zeugvars-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zeugvars-0.1.0/zeugvars.py` & `zeugvars-0.1.1/zeugvars.py`

 * *Files identical despite different names*

