# Comparing `tmp/linfa_vi-1.0.3.tar.gz` & `tmp/linfa_vi-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linfa_vi-1.0.3.tar", last modified: Sat Jul  1 17:22:25 2023, max compression
+gzip compressed data, was "linfa_vi-1.0.4.tar", last modified: Sat Jul  1 19:37:24 2023, max compression
```

## Comparing `linfa_vi-1.0.3.tar` & `linfa_vi-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:22:25.904546 linfa_vi-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-01 17:22:15.000000 linfa_vi-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-01 17:22:25.904546 linfa_vi-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-07-01 17:22:15.000000 linfa_vi-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:22:25.904546 linfa_vi-1.0.3/linfa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:22:15.000000 linfa_vi-1.0.3/linfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-07-01 17:22:15.000000 linfa_vi-1.0.3/linfa/maf.py
--rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-07-01 17:22:15.000000 linfa_vi-1.0.3/linfa/nofas.py
--rw-r--r--   0 runner    (1001) docker     (123)    13555 2023-07-01 17:22:15.000000 linfa_vi-1.0.3/linfa/run_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-01 17:22:15.000000 linfa_vi-1.0.3/linfa/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:22:25.904546 linfa_vi-1.0.3/linfa_vi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-01 17:22:25.000000 linfa_vi-1.0.3/linfa_vi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-01 17:22:25.000000 linfa_vi-1.0.3/linfa_vi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 17:22:25.000000 linfa_vi-1.0.3/linfa_vi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-01 17:22:25.000000 linfa_vi-1.0.3/linfa_vi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-01 17:22:25.000000 linfa_vi-1.0.3/linfa_vi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-01 17:22:15.000000 linfa_vi-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 17:22:25.904546 linfa_vi-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 17:22:15.000000 linfa_vi-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:22:25.904546 linfa_vi-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    30715 2023-07-01 17:22:15.000000 linfa_vi-1.0.3/tests/test_linfa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:37:24.229439 linfa_vi-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-01 19:37:13.000000 linfa_vi-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-01 19:37:24.229439 linfa_vi-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-07-01 19:37:13.000000 linfa_vi-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:37:24.229439 linfa_vi-1.0.4/linfa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 19:37:13.000000 linfa_vi-1.0.4/linfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-07-01 19:37:13.000000 linfa_vi-1.0.4/linfa/maf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-07-01 19:37:13.000000 linfa_vi-1.0.4/linfa/nofas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13555 2023-07-01 19:37:13.000000 linfa_vi-1.0.4/linfa/run_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-01 19:37:13.000000 linfa_vi-1.0.4/linfa/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:37:24.229439 linfa_vi-1.0.4/linfa_vi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-01 19:37:24.000000 linfa_vi-1.0.4/linfa_vi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-01 19:37:24.000000 linfa_vi-1.0.4/linfa_vi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 19:37:24.000000 linfa_vi-1.0.4/linfa_vi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-01 19:37:24.000000 linfa_vi-1.0.4/linfa_vi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-01 19:37:24.000000 linfa_vi-1.0.4/linfa_vi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-01 19:37:13.000000 linfa_vi-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 19:37:24.229439 linfa_vi-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 19:37:13.000000 linfa_vi-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:37:24.229439 linfa_vi-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    30715 2023-07-01 19:37:13.000000 linfa_vi-1.0.4/tests/test_linfa.py
```

### Comparing `linfa_vi-1.0.3/LICENSE` & `linfa_vi-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.0.3/PKG-INFO` & `linfa_vi-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linfa_vi
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python library for inference with normalizing flow and annealing
 Author-email: resDesLab  <daniele.schiavazzi@gmail.com>
 License: Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `linfa_vi-1.0.3/README.md` & `linfa_vi-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.0.3/linfa/maf.py` & `linfa_vi-1.0.4/linfa/maf.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.0.3/linfa/nofas.py` & `linfa_vi-1.0.4/linfa/nofas.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.0.3/linfa/run_experiment.py` & `linfa_vi-1.0.4/linfa/run_experiment.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.0.3/linfa/transform.py` & `linfa_vi-1.0.4/linfa/transform.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.0.3/linfa_vi.egg-info/PKG-INFO` & `linfa_vi-1.0.4/linfa_vi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linfa-vi
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python library for inference with normalizing flow and annealing
 Author-email: resDesLab  <daniele.schiavazzi@gmail.com>
 License: Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `linfa_vi-1.0.3/pyproject.toml` & `linfa_vi-1.0.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "linfa_vi"
-version = "1.0.3"
+version = "1.0.4"
 description = "A Python library for inference with normalizing flow and annealing"
 readme = "README.md"
 authors = [{ name = "resDesLab ", email = "daniele.schiavazzi@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["variational inference", "normalizig flow", "adaptive annealing", "physics-based modeling"]
 dependencies = [
     "torch==1.13.1",
-    "numpy==1.22",
+    "numpy==1.19.5",
     'tomli; python_version < "3.11"',    
 ]
 requires-python = ">=3.7"
 
 [tool.setuptools]
 packages = ["linfa"]
```

### Comparing `linfa_vi-1.0.3/tests/test_linfa.py` & `linfa_vi-1.0.4/tests/test_linfa.py`

 * *Files identical despite different names*

