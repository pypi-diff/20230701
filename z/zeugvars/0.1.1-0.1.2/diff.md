# Comparing `tmp/zeugvars-0.1.1.tar.gz` & `tmp/zeugvars-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeugvars-0.1.1.tar", max compression
+gzip compressed data, was "zeugvars-0.1.2.tar", max compression
```

## Comparing `zeugvars-0.1.1.tar` & `zeugvars-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1083 2023-06-29 20:37:00.152930 zeugvars-0.1.1/LICENSE
--rw-r--r--   0        0        0      438 2023-07-01 10:17:58.043297 zeugvars-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       86 2023-06-29 20:37:00.154924 zeugvars-0.1.1/README.md
--rw-r--r--   0        0        0    10817 2023-07-01 10:01:32.143374 zeugvars-0.1.1/zeugvars.py
--rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 zeugvars-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-29 20:37:00.152930 zeugvars-0.1.2/LICENSE
+-rw-r--r--   0        0        0      524 2023-07-01 10:22:26.461939 zeugvars-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2491 2023-07-01 10:30:54.698962 zeugvars-0.1.2/README.md
+-rw-r--r--   0        0        0    10864 2023-07-01 10:30:54.691960 zeugvars-0.1.2/zeugvars.py
+-rw-r--r--   0        0        0     2894 1970-01-01 00:00:00.000000 zeugvars-0.1.2/PKG-INFO
```

### Comparing `zeugvars-0.1.1/LICENSE` & `zeugvars-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zeugvars-0.1.1/zeugvars.py` & `zeugvars-0.1.2/zeugvars.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 ZeugVars
 ~~~~~~~~
 A simple & straight-forward Python module for creating context-dependent proxy objects.
 
 (C) bswck, 2023
 
-Short Description
------------------
+What is this?
+-------------
 `zeugvars` is a Python module for creating context-dependent proxy objects.
 
 By 'proxy' we mean any object that forwards attribute access to another
 object.  By 'context-dependent' we mean that the object to which the proxy
 forwards attribute access can change depending on the context in which the
 proxy is used.
 
@@ -24,16 +24,16 @@
 the object to which `flask.request` forwards attribute access is stored
 in a `werkzeug.local.LocalProxy` object. The functionality of `zeugvars.zeugvar()`
 is roughly equivalent to `werkzeug.local.LocalProxy`. The `zeugvar` function
 creates a proxy object that forwards attribute access to an object stored
 in the provided manager, which could be any object that implements the
 `Manager` protocol; for example, a `contextvars.ContextVar` object.
 
-Usage
------
+Description
+-----------
 The `zeugvar` function takes a `Manager` object and class (optional) as arguments.
 The `Manager` object must have `get` and `set` methods.  The `get` method returns
 the object to which the proxy forwards attribute access.  The `set` method sets
 the object to which the proxy forwards attribute access.  `set` is called when
 the proxy is being inplace modified.  The class is optional unless the `Manager`
 is bound, i.e. `Manager.get` returns an instance of a class.
 The user might provide custom `getter` and `setter` functions.
@@ -54,15 +54,15 @@
 >>> count += 1
 >>> count
 1
 >>> count -= 1
 >>> count
 0
 >>> counter.set(1000)
-<Token...>
+<Token var=<ContextVar name='counter' at ...> at ...>
 >>> count
 1000
 """
 
 import contextlib
 import functools
 from collections.abc import Callable
```

