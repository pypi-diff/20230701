# Comparing `tmp/parcoords-0.1.1.tar.gz` & `tmp/parcoords-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parcoords-0.1.1.tar", last modified: Sat Jul  1 15:22:03 2023, max compression
+gzip compressed data, was "parcoords-0.1.2.tar", last modified: Sat Jul  1 15:35:55 2023, max compression
```

## Comparing `parcoords-0.1.1.tar` & `parcoords-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:22:03.113590 parcoords-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-01 15:21:49.000000 parcoords-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-01 15:22:03.109590 parcoords-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-01 15:21:49.000000 parcoords-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:22:03.109590 parcoords-0.1.1/parcoords/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-01 15:21:49.000000 parcoords-0.1.1/parcoords/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-07-01 15:21:49.000000 parcoords-0.1.1/parcoords/parcoords.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:22:03.109590 parcoords-0.1.1/parcoords.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-01 15:22:03.000000 parcoords-0.1.1/parcoords.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-01 15:22:03.000000 parcoords-0.1.1/parcoords.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 15:22:03.000000 parcoords-0.1.1/parcoords.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-01 15:22:03.000000 parcoords-0.1.1/parcoords.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 15:22:03.000000 parcoords-0.1.1/parcoords.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 15:22:03.113590 parcoords-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-01 15:21:49.000000 parcoords-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:35:55.377490 parcoords-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-01 15:35:46.000000 parcoords-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-01 15:35:55.377490 parcoords-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-01 15:35:46.000000 parcoords-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:35:55.377490 parcoords-0.1.2/parcoords/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-01 15:35:46.000000 parcoords-0.1.2/parcoords/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-07-01 15:35:46.000000 parcoords-0.1.2/parcoords/parcoords.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:35:55.377490 parcoords-0.1.2/parcoords.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-01 15:35:55.000000 parcoords-0.1.2/parcoords.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-01 15:35:55.000000 parcoords-0.1.2/parcoords.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 15:35:55.000000 parcoords-0.1.2/parcoords.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-01 15:35:55.000000 parcoords-0.1.2/parcoords.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 15:35:55.000000 parcoords-0.1.2/parcoords.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 15:35:55.377490 parcoords-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-01 15:35:46.000000 parcoords-0.1.2/setup.py
```

### Comparing `parcoords-0.1.1/LICENSE.txt` & `parcoords-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `parcoords-0.1.1/PKG-INFO` & `parcoords-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: parcoords
-Version: 0.1.1
+Version: 0.1.2
 Summary: Parallel coordinates plotting
+Home-page: https://github.com/VoigtPeter/parcoords
 Author: Peter Voigt
 License: MIT
 Keywords: parallel coordinates,parallel-coordinates,plot,hyperparameter,visualization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -13,28 +14,29 @@
 License-File: LICENSE.txt
 
 # Parallel Coordinates Plotting for Python `parcoords`
 
 This package implements a parallel-coordinate plot, commonly used in machine learning, i.e. for hyperparameter visualization.
 
 <p align="center">
-  <img alt="Example parallel-coordinate plot" src="img/example_plot.png">
+  <img alt="Example parallel-coordinate plot" src="https://raw.githubusercontent.com/VoigtPeter/parcoords/main/img/example_plot.png">
 </p>
 
 ## Installation
 The `parcoords` package can be installed with pip:
 ```
-pip install <package name>
+pip install parcoords
 ```
+You can also view the package on [PyPI](https://pypi.org/project/parcoords/).
 
 ## Usage
 The following code produces the sample plot at the beginning of this page.
 ```python
 import matplotlib.pyplot as plt
-from parcoords.parcoords import plot_parcoords
+from parcoords import plot_parcoords
 
 # let's define some data to plot
 values = [
     [0.1, 10, "smote", 0.78],
     [0.15, 9, "none", 0.46],
     [0.18, 8, "rand_over", 0.67],
     [0.01, 16, "rand_over", 0.84],
@@ -55,8 +57,8 @@
     title="Parallel-Coordinates of the Hyperparameters",
 )
 
 plt.show()
 ```
 
 ## License
-This repository is licensed under the [MIT-License](./LICENSE.txt).
+This repository is licensed under the [MIT-License](https://github.com/VoigtPeter/parcoords/blob/main/LICENSE.txt).
```

### Comparing `parcoords-0.1.1/README.md` & `parcoords-0.1.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # Parallel Coordinates Plotting for Python `parcoords`
 
 This package implements a parallel-coordinate plot, commonly used in machine learning, i.e. for hyperparameter visualization.
 
 <p align="center">
-  <img alt="Example parallel-coordinate plot" src="img/example_plot.png">
+  <img alt="Example parallel-coordinate plot" src="https://raw.githubusercontent.com/VoigtPeter/parcoords/main/img/example_plot.png">
 </p>
 
 ## Installation
 The `parcoords` package can be installed with pip:
 ```
-pip install <package name>
+pip install parcoords
 ```
+You can also view the package on [PyPI](https://pypi.org/project/parcoords/).
 
 ## Usage
 The following code produces the sample plot at the beginning of this page.
 ```python
 import matplotlib.pyplot as plt
-from parcoords.parcoords import plot_parcoords
+from parcoords import plot_parcoords
 
 # let's define some data to plot
 values = [
     [0.1, 10, "smote", 0.78],
     [0.15, 9, "none", 0.46],
     [0.18, 8, "rand_over", 0.67],
     [0.01, 16, "rand_over", 0.84],
@@ -41,8 +42,8 @@
     title="Parallel-Coordinates of the Hyperparameters",
 )
 
 plt.show()
 ```
 
 ## License
-This repository is licensed under the [MIT-License](./LICENSE.txt).
+This repository is licensed under the [MIT-License](https://github.com/VoigtPeter/parcoords/blob/main/LICENSE.txt).
```

### Comparing `parcoords-0.1.1/parcoords/parcoords.py` & `parcoords-0.1.2/parcoords/parcoords.py`

 * *Files identical despite different names*

### Comparing `parcoords-0.1.1/parcoords.egg-info/PKG-INFO` & `parcoords-0.1.2/parcoords.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: parcoords
-Version: 0.1.1
+Version: 0.1.2
 Summary: Parallel coordinates plotting
+Home-page: https://github.com/VoigtPeter/parcoords
 Author: Peter Voigt
 License: MIT
 Keywords: parallel coordinates,parallel-coordinates,plot,hyperparameter,visualization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -13,28 +14,29 @@
 License-File: LICENSE.txt
 
 # Parallel Coordinates Plotting for Python `parcoords`
 
 This package implements a parallel-coordinate plot, commonly used in machine learning, i.e. for hyperparameter visualization.
 
 <p align="center">
-  <img alt="Example parallel-coordinate plot" src="img/example_plot.png">
+  <img alt="Example parallel-coordinate plot" src="https://raw.githubusercontent.com/VoigtPeter/parcoords/main/img/example_plot.png">
 </p>
 
 ## Installation
 The `parcoords` package can be installed with pip:
 ```
-pip install <package name>
+pip install parcoords
 ```
+You can also view the package on [PyPI](https://pypi.org/project/parcoords/).
 
 ## Usage
 The following code produces the sample plot at the beginning of this page.
 ```python
 import matplotlib.pyplot as plt
-from parcoords.parcoords import plot_parcoords
+from parcoords import plot_parcoords
 
 # let's define some data to plot
 values = [
     [0.1, 10, "smote", 0.78],
     [0.15, 9, "none", 0.46],
     [0.18, 8, "rand_over", 0.67],
     [0.01, 16, "rand_over", 0.84],
@@ -55,8 +57,8 @@
     title="Parallel-Coordinates of the Hyperparameters",
 )
 
 plt.show()
 ```
 
 ## License
-This repository is licensed under the [MIT-License](./LICENSE.txt).
+This repository is licensed under the [MIT-License](https://github.com/VoigtPeter/parcoords/blob/main/LICENSE.txt).
```

### Comparing `parcoords-0.1.1/setup.py` & `parcoords-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 import os
 import setuptools
 
 
 setuptools.setup(
     name="parcoords",
-    version="0.1.1",
+    version="0.1.2",
     author="Peter Voigt",
+    url="https://github.com/VoigtPeter/parcoords",
     packages=["parcoords"],
     license="MIT",
     description="Parallel coordinates plotting",
-    long_description=open(os.path.join(os.path.dirname(__file__), "README.md")).read(),
+    long_description=open(
+        os.path.join(os.path.dirname(__file__), "README.md")
+    ).read(),
     long_description_content_type="text/markdown",
-    keywords=["parallel coordinates", "parallel-coordinates", "plot", "hyperparameter", "visualization"],
+    keywords=[
+        "parallel coordinates",
+        "parallel-coordinates",
+        "plot",
+        "hyperparameter",
+        "visualization",
+    ],
     python_requires=">=3.6",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    install_requires=["matplotlib", "numpy"]
+    install_requires=["matplotlib", "numpy"],
 )
```

