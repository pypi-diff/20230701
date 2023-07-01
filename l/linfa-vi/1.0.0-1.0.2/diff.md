# Comparing `tmp/linfa_vi-1.0.0.tar.gz` & `tmp/linfa_vi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linfa_vi-1.0.0.tar", last modified: Sat Jul  1 16:07:09 2023, max compression
+gzip compressed data, was "linfa_vi-1.0.2.tar", last modified: Sat Jul  1 16:36:54 2023, max compression
```

## Comparing `linfa_vi-1.0.0.tar` & `linfa_vi-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:07:09.685803 linfa_vi-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-01 16:05:08.000000 linfa_vi-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-07-01 16:07:09.685803 linfa_vi-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-07-01 16:05:08.000000 linfa_vi-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:07:09.681803 linfa_vi-1.0.0/linfa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:05:08.000000 linfa_vi-1.0.0/linfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-07-01 16:05:08.000000 linfa_vi-1.0.0/linfa/maf.py
--rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-07-01 16:05:08.000000 linfa_vi-1.0.0/linfa/nofas.py
--rw-r--r--   0 runner    (1001) docker     (123)    13555 2023-07-01 16:05:08.000000 linfa_vi-1.0.0/linfa/run_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-01 16:05:08.000000 linfa_vi-1.0.0/linfa/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:07:09.685803 linfa_vi-1.0.0/linfa_vi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-07-01 16:07:09.000000 linfa_vi-1.0.0/linfa_vi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-01 16:07:09.000000 linfa_vi-1.0.0/linfa_vi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 16:07:09.000000 linfa_vi-1.0.0/linfa_vi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-01 16:07:09.000000 linfa_vi-1.0.0/linfa_vi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-01 16:07:09.000000 linfa_vi-1.0.0/linfa_vi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-01 16:05:08.000000 linfa_vi-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 16:07:09.685803 linfa_vi-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 16:05:08.000000 linfa_vi-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:07:09.685803 linfa_vi-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    30715 2023-07-01 16:05:08.000000 linfa_vi-1.0.0/tests/test_linfa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:36:54.044263 linfa_vi-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-01 16:36:42.000000 linfa_vi-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-07-01 16:36:54.044263 linfa_vi-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-07-01 16:36:42.000000 linfa_vi-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:36:54.044263 linfa_vi-1.0.2/linfa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:36:42.000000 linfa_vi-1.0.2/linfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-07-01 16:36:42.000000 linfa_vi-1.0.2/linfa/maf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-07-01 16:36:42.000000 linfa_vi-1.0.2/linfa/nofas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13555 2023-07-01 16:36:42.000000 linfa_vi-1.0.2/linfa/run_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-01 16:36:42.000000 linfa_vi-1.0.2/linfa/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:36:54.044263 linfa_vi-1.0.2/linfa_vi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-07-01 16:36:54.000000 linfa_vi-1.0.2/linfa_vi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-01 16:36:54.000000 linfa_vi-1.0.2/linfa_vi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 16:36:54.000000 linfa_vi-1.0.2/linfa_vi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-01 16:36:54.000000 linfa_vi-1.0.2/linfa_vi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-01 16:36:54.000000 linfa_vi-1.0.2/linfa_vi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-01 16:36:42.000000 linfa_vi-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 16:36:54.044263 linfa_vi-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 16:36:42.000000 linfa_vi-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:36:54.044263 linfa_vi-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    30715 2023-07-01 16:36:42.000000 linfa_vi-1.0.2/tests/test_linfa.py
```

### Comparing `linfa_vi-1.0.0/LICENSE` & `linfa_vi-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.0.0/PKG-INFO` & `linfa_vi-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linfa_vi
-Version: 1.0.0
+Version: 1.0.2
 Summary: A Python library for inference with normalizing flow and annealing
 Author-email: resDesLab  <daniele.schiavazzi@gmail.com>
 License: Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -18,15 +18,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
  ![example workflow](https://github.com/desResLab/LINFA/actions/workflows/test_publish_pypi.yml/badge.svg) 
-[![Documentation Status](https://readthedocs.org/projects/mrina/badge/?version=latest)](https://mrina.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/linfa-vi/badge/?version=latest)](https://linfa-vi.readthedocs.io/en/latest/?badge=latest)
 
 ## LINFA
 
 LINFA is a library for variational inference with normalizing flow and adaptive annealing. It is designed to accommodate computationally expensive models and difficult-to-sample posterior distributions with dependent parameters.
 
 The code for the masked autoencoders for density estimation (MADE), masked autoregressive flow (MAF) and real non volume-preserving transformation (RealNVP) is based on the implementation provided by [Kamen Bliznashki](https://github.com/kamenbliznashki/normalizing_flows). 
 
@@ -47,17 +47,16 @@
 Background theory and examples for LINFA are discussed in the two papers: 
 
 - Y. Wang, F. Liu and D.E. Schiavazzi, *[Variational Inference with NoFAS: Normalizing Flow with Adaptive Surrogate for Computationally Expensive Models](https://www.sciencedirect.com/science/article/abs/pii/S0021999122005162)*
 - E.R. Cobian, J.D. Hauenstein, F. Liu and D.E. Schiavazzi, *[AdaAnn: Adaptive Annealing Scheduler for Probability Density Approximation](https://www.dl.begellhouse.com/journals/52034eb04b657aea,796f39cb1acf1296,6f85fe1149ff41d9.html?sgstd=1)*
 
 ### Requirements
 
-* PyTorch 1.4.0
-* Numpy 1.19.2
-* Scipy 1.6.1
+* PyTorch 1.13.1
+* Numpy 1.22
 
 ### Numerical Benchmarks
 
 LINFA includes five numerical benchmarks:
 
 * Trivial example.
 * High dimensional example (Sobol' function).
```

### Comparing `linfa_vi-1.0.0/README.md` & `linfa_vi-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
  ![example workflow](https://github.com/desResLab/LINFA/actions/workflows/test_publish_pypi.yml/badge.svg) 
-[![Documentation Status](https://readthedocs.org/projects/mrina/badge/?version=latest)](https://mrina.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/linfa-vi/badge/?version=latest)](https://linfa-vi.readthedocs.io/en/latest/?badge=latest)
 
 ## LINFA
 
 LINFA is a library for variational inference with normalizing flow and adaptive annealing. It is designed to accommodate computationally expensive models and difficult-to-sample posterior distributions with dependent parameters.
 
 The code for the masked autoencoders for density estimation (MADE), masked autoregressive flow (MAF) and real non volume-preserving transformation (RealNVP) is based on the implementation provided by [Kamen Bliznashki](https://github.com/kamenbliznashki/normalizing_flows). 
 
@@ -25,17 +25,16 @@
 Background theory and examples for LINFA are discussed in the two papers: 
 
 - Y. Wang, F. Liu and D.E. Schiavazzi, *[Variational Inference with NoFAS: Normalizing Flow with Adaptive Surrogate for Computationally Expensive Models](https://www.sciencedirect.com/science/article/abs/pii/S0021999122005162)*
 - E.R. Cobian, J.D. Hauenstein, F. Liu and D.E. Schiavazzi, *[AdaAnn: Adaptive Annealing Scheduler for Probability Density Approximation](https://www.dl.begellhouse.com/journals/52034eb04b657aea,796f39cb1acf1296,6f85fe1149ff41d9.html?sgstd=1)*
 
 ### Requirements
 
-* PyTorch 1.4.0
-* Numpy 1.19.2
-* Scipy 1.6.1
+* PyTorch 1.13.1
+* Numpy 1.22
 
 ### Numerical Benchmarks
 
 LINFA includes five numerical benchmarks:
 
 * Trivial example.
 * High dimensional example (Sobol' function).
```

### Comparing `linfa_vi-1.0.0/linfa/maf.py` & `linfa_vi-1.0.2/linfa/maf.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.0.0/linfa/nofas.py` & `linfa_vi-1.0.2/linfa/nofas.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.0.0/linfa/run_experiment.py` & `linfa_vi-1.0.2/linfa/run_experiment.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.0.0/linfa/transform.py` & `linfa_vi-1.0.2/linfa/transform.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.0.0/linfa_vi.egg-info/PKG-INFO` & `linfa_vi-1.0.2/linfa_vi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linfa-vi
-Version: 1.0.0
+Version: 1.0.2
 Summary: A Python library for inference with normalizing flow and annealing
 Author-email: resDesLab  <daniele.schiavazzi@gmail.com>
 License: Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -18,15 +18,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
  ![example workflow](https://github.com/desResLab/LINFA/actions/workflows/test_publish_pypi.yml/badge.svg) 
-[![Documentation Status](https://readthedocs.org/projects/mrina/badge/?version=latest)](https://mrina.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/linfa-vi/badge/?version=latest)](https://linfa-vi.readthedocs.io/en/latest/?badge=latest)
 
 ## LINFA
 
 LINFA is a library for variational inference with normalizing flow and adaptive annealing. It is designed to accommodate computationally expensive models and difficult-to-sample posterior distributions with dependent parameters.
 
 The code for the masked autoencoders for density estimation (MADE), masked autoregressive flow (MAF) and real non volume-preserving transformation (RealNVP) is based on the implementation provided by [Kamen Bliznashki](https://github.com/kamenbliznashki/normalizing_flows). 
 
@@ -47,17 +47,16 @@
 Background theory and examples for LINFA are discussed in the two papers: 
 
 - Y. Wang, F. Liu and D.E. Schiavazzi, *[Variational Inference with NoFAS: Normalizing Flow with Adaptive Surrogate for Computationally Expensive Models](https://www.sciencedirect.com/science/article/abs/pii/S0021999122005162)*
 - E.R. Cobian, J.D. Hauenstein, F. Liu and D.E. Schiavazzi, *[AdaAnn: Adaptive Annealing Scheduler for Probability Density Approximation](https://www.dl.begellhouse.com/journals/52034eb04b657aea,796f39cb1acf1296,6f85fe1149ff41d9.html?sgstd=1)*
 
 ### Requirements
 
-* PyTorch 1.4.0
-* Numpy 1.19.2
-* Scipy 1.6.1
+* PyTorch 1.13.1
+* Numpy 1.22
 
 ### Numerical Benchmarks
 
 LINFA includes five numerical benchmarks:
 
 * Trivial example.
 * High dimensional example (Sobol' function).
```

### Comparing `linfa_vi-1.0.0/pyproject.toml` & `linfa_vi-1.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,29 +2,28 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "linfa_vi"
-version = "1.0.0"
+version = "1.0.2"
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
     "numpy==1.22",
-    "scipy==1.7.3",
     'tomli; python_version < "3.11"',    
 ]
 requires-python = ">=3.7"
 
 [tool.setuptools]
 packages = ["linfa"]
```

### Comparing `linfa_vi-1.0.0/tests/test_linfa.py` & `linfa_vi-1.0.2/tests/test_linfa.py`

 * *Files identical despite different names*

