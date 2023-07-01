# Comparing `tmp/calsim-0.0.3.tar.gz` & `tmp/calsim-0.0.4.tar.gz`

## Comparing `calsim-0.0.3.tar` & `calsim-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 calsim-0.0.3/src/CalSim/__init__.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 calsim-0.0.3/src/CalSim/core/__init__.py
--rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 calsim-0.0.3/src/CalSim/core/control.py
--rwxr-xr-x   0        0        0     4852 2020-02-02 00:00:00.000000 calsim-0.0.3/src/CalSim/core/controller.py
--rwxr-xr-x   0        0        0    13617 2020-02-02 00:00:00.000000 calsim-0.0.3/src/CalSim/core/dynamics.py
--rwxr-xr-x   0        0        0     5815 2020-02-02 00:00:00.000000 calsim-0.0.3/src/CalSim/core/environment.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 calsim-0.0.3/src/CalSim/core/exceptions.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 calsim-0.0.3/src/CalSim/core/manipulator.py
--rwxr-xr-x   0        0        0      483 2020-02-02 00:00:00.000000 calsim-0.0.3/src/CalSim/core/run_simulation.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 calsim-0.0.3/src/CalSim/core/sim_utils.py
--rwxr-xr-x   0        0        0     4475 2020-02-02 00:00:00.000000 calsim-0.0.3/src/CalSim/core/state_estimation.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 calsim-0.0.3/src/CalSim/core/tests.py
--rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 calsim-0.0.3/src/CalSim/core/transforms.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 calsim-0.0.3/src/CalSim/core/twist.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 calsim-0.0.3/LICENSE
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 calsim-0.0.3/README.md
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 calsim-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 calsim-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 calsim-0.0.4/src/CalSim/__init__.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 calsim-0.0.4/src/CalSim/core/__init__.py
+-rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 calsim-0.0.4/src/CalSim/core/control.py
+-rwxr-xr-x   0        0        0     4852 2020-02-02 00:00:00.000000 calsim-0.0.4/src/CalSim/core/controller.py
+-rwxr-xr-x   0        0        0    13617 2020-02-02 00:00:00.000000 calsim-0.0.4/src/CalSim/core/dynamics.py
+-rwxr-xr-x   0        0        0     6073 2020-02-02 00:00:00.000000 calsim-0.0.4/src/CalSim/core/environment.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 calsim-0.0.4/src/CalSim/core/exceptions.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 calsim-0.0.4/src/CalSim/core/manipulator.py
+-rwxr-xr-x   0        0        0      483 2020-02-02 00:00:00.000000 calsim-0.0.4/src/CalSim/core/run_simulation.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 calsim-0.0.4/src/CalSim/core/sim_utils.py
+-rwxr-xr-x   0        0        0     4475 2020-02-02 00:00:00.000000 calsim-0.0.4/src/CalSim/core/state_estimation.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 calsim-0.0.4/src/CalSim/core/tests.py
+-rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 calsim-0.0.4/src/CalSim/core/transforms.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 calsim-0.0.4/src/CalSim/core/twist.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 calsim-0.0.4/tests/test_simulation_simple.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 calsim-0.0.4/LICENSE
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 calsim-0.0.4/README.md
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 calsim-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 calsim-0.0.4/PKG-INFO
```

### Comparing `calsim-0.0.3/src/CalSim/core/control.py` & `calsim-0.0.4/src/CalSim/core/control.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.3/src/CalSim/core/controller.py` & `calsim-0.0.4/src/CalSim/core/controller.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.3/src/CalSim/core/dynamics.py` & `calsim-0.0.4/src/CalSim/core/dynamics.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.3/src/CalSim/core/environment.py` & `calsim-0.0.4/src/CalSim/core/environment.py`

 * *Files 7% similar despite different names*

```diff
@@ -122,27 +122,33 @@
             boolean: whether or not the time has exceeded the total simulation time
         """
         #check current time with respect to simulation time
         if self.t >= self.TOTAL_SIM_TIME:
             return True
         return False
     
-    def run(self, N = 1):
+    def run(self, N = 1, run_vis = True):
         """
         Function to run the simulation N times
         Inputs:
             N (int): number of simulation examples to run
+            run_vis (bool): run the visualization of the results
+        Returns:
+            self.xHist, self.uHist, self.tHist
         """
         #loop over an overall simulation N times
         for i in range(N):
             self.reset()
             while not self._is_done():
                 print("Simulation Time Remaining: ", self.TOTAL_SIM_TIME - self.t)
                 self.step() #step the environment while not done
-            self.visualize() #render the result
+            if run_vis:
+                self.visualize() #render the result
+        #return the history arrays
+        return self.xHist, self.uHist, self.tHist
             
     def visualize(self):
         """
         Provide visualization of the environment
         """
         self.dynamics.show_animation(self.xHist, self.uHist, self.tHist)
         self.dynamics.show_plots(self.xHist, self.uHist, self.tHist)
```

### Comparing `calsim-0.0.3/src/CalSim/core/manipulator.py` & `calsim-0.0.4/src/CalSim/core/manipulator.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.3/src/CalSim/core/sim_utils.py` & `calsim-0.0.4/src/CalSim/core/sim_utils.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.3/src/CalSim/core/state_estimation.py` & `calsim-0.0.4/src/CalSim/core/state_estimation.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.3/src/CalSim/core/transforms.py` & `calsim-0.0.4/src/CalSim/core/transforms.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.3/src/CalSim/core/twist.py` & `calsim-0.0.4/src/CalSim/core/twist.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.3/LICENSE` & `calsim-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `calsim-0.0.3/pyproject.toml` & `calsim-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "CalSim"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Massimiliano de Sa", email="mz.desa@berkeley.edu" },
 ]
 description = "Simulator package for Berkeley robotics course."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `calsim-0.0.3/PKG-INFO` & `calsim-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalSim
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simulator package for Berkeley robotics course.
 Project-URL: Homepage, https://github.com/mzdesa/CalSim
 Project-URL: Bug Tracker, https://github.com/mzdesa/CalSim
 Author-email: Massimiliano de Sa <mz.desa@berkeley.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

