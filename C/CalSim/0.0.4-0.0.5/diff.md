# Comparing `tmp/calsim-0.0.4.tar.gz` & `tmp/calsim-0.0.5.tar.gz`

## Comparing `calsim-0.0.4.tar` & `calsim-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 calsim-0.0.4/src/CalSim/__init__.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 calsim-0.0.4/src/CalSim/core/__init__.py
--rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 calsim-0.0.4/src/CalSim/core/control.py
--rwxr-xr-x   0        0        0     4852 2020-02-02 00:00:00.000000 calsim-0.0.4/src/CalSim/core/controller.py
--rwxr-xr-x   0        0        0    13617 2020-02-02 00:00:00.000000 calsim-0.0.4/src/CalSim/core/dynamics.py
--rwxr-xr-x   0        0        0     6073 2020-02-02 00:00:00.000000 calsim-0.0.4/src/CalSim/core/environment.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 calsim-0.0.4/src/CalSim/core/exceptions.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 calsim-0.0.4/src/CalSim/core/manipulator.py
--rwxr-xr-x   0        0        0      483 2020-02-02 00:00:00.000000 calsim-0.0.4/src/CalSim/core/run_simulation.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 calsim-0.0.4/src/CalSim/core/sim_utils.py
--rwxr-xr-x   0        0        0     4475 2020-02-02 00:00:00.000000 calsim-0.0.4/src/CalSim/core/state_estimation.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 calsim-0.0.4/src/CalSim/core/tests.py
--rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 calsim-0.0.4/src/CalSim/core/transforms.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 calsim-0.0.4/src/CalSim/core/twist.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 calsim-0.0.4/tests/test_simulation_simple.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 calsim-0.0.4/LICENSE
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 calsim-0.0.4/README.md
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 calsim-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 calsim-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 calsim-0.0.5/src/CalSim/__init__.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 calsim-0.0.5/src/CalSim/core/__init__.py
+-rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 calsim-0.0.5/src/CalSim/core/control.py
+-rwxr-xr-x   0        0        0     4852 2020-02-02 00:00:00.000000 calsim-0.0.5/src/CalSim/core/controller.py
+-rwxr-xr-x   0        0        0    13617 2020-02-02 00:00:00.000000 calsim-0.0.5/src/CalSim/core/dynamics.py
+-rwxr-xr-x   0        0        0     6073 2020-02-02 00:00:00.000000 calsim-0.0.5/src/CalSim/core/environment.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 calsim-0.0.5/src/CalSim/core/exceptions.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 calsim-0.0.5/src/CalSim/core/manipulator.py
+-rwxr-xr-x   0        0        0      483 2020-02-02 00:00:00.000000 calsim-0.0.5/src/CalSim/core/run_simulation.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 calsim-0.0.5/src/CalSim/core/sim_utils.py
+-rwxr-xr-x   0        0        0     4475 2020-02-02 00:00:00.000000 calsim-0.0.5/src/CalSim/core/state_estimation.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 calsim-0.0.5/src/CalSim/core/tests.py
+-rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 calsim-0.0.5/src/CalSim/core/transforms.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 calsim-0.0.5/src/CalSim/core/twist.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 calsim-0.0.5/tests/test_simulation_simple.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 calsim-0.0.5/LICENSE
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 calsim-0.0.5/README.md
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 calsim-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 calsim-0.0.5/PKG-INFO
```

### Comparing `calsim-0.0.4/src/CalSim/core/control.py` & `calsim-0.0.5/src/CalSim/core/control.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.4/src/CalSim/core/controller.py` & `calsim-0.0.5/src/CalSim/core/controller.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.4/src/CalSim/core/dynamics.py` & `calsim-0.0.5/src/CalSim/core/dynamics.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.4/src/CalSim/core/environment.py` & `calsim-0.0.5/src/CalSim/core/environment.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.4/src/CalSim/core/manipulator.py` & `calsim-0.0.5/src/CalSim/core/manipulator.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.4/src/CalSim/core/sim_utils.py` & `calsim-0.0.5/src/CalSim/core/sim_utils.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.4/src/CalSim/core/state_estimation.py` & `calsim-0.0.5/src/CalSim/core/state_estimation.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.4/src/CalSim/core/transforms.py` & `calsim-0.0.5/src/CalSim/core/transforms.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.4/src/CalSim/core/twist.py` & `calsim-0.0.5/src/CalSim/core/twist.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.4/LICENSE` & `calsim-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `calsim-0.0.4/pyproject.toml` & `calsim-0.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "CalSim"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Massimiliano de Sa", email="mz.desa@berkeley.edu" },
 ]
 description = "Simulator package for Berkeley robotics course."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "numpy>=1.24.0",
-  "matplotlib>=3.7.0",
-  "seaborn>=0.12.0",
+  "numpy>=1.20.0",
+  "matplotlib>=3.5.0",
+  "seaborn>=0.10.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/mzdesa/CalSim"
 "Bug Tracker" = "https://github.com/mzdesa/CalSim"
```

### Comparing `calsim-0.0.4/PKG-INFO` & `calsim-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: CalSim
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simulator package for Berkeley robotics course.
 Project-URL: Homepage, https://github.com/mzdesa/CalSim
 Project-URL: Bug Tracker, https://github.com/mzdesa/CalSim
 Author-email: Massimiliano de Sa <mz.desa@berkeley.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: matplotlib>=3.7.0
-Requires-Dist: numpy>=1.24.0
-Requires-Dist: seaborn>=0.12.0
+Requires-Dist: matplotlib>=3.5.0
+Requires-Dist: numpy>=1.20.0
+Requires-Dist: seaborn>=0.10.0
 Description-Content-Type: text/markdown
 
 # CalSim
 Multi-purpose educational robotics simulator built for the Berkeley courses 106/206 AB.
```

