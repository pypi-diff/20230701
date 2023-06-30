# Comparing `tmp/flasc-1.3.tar.gz` & `tmp/flasc-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flasc-1.3.tar", last modified: Thu Jun  1 20:36:46 2023, max compression
+gzip compressed data, was "flasc-1.3.1.tar", last modified: Fri Jun 30 22:32:39 2023, max compression
```

## Comparing `flasc-1.3.tar` & `flasc-1.3.1.tar`

### file list

```diff
@@ -1,25 +1,56 @@
-drwxr-xr-x   0 rmudafor (1974918542) NREL_NT\Domain Users (18434217)        0 2023-06-01 20:36:46.699920 flasc-1.3/
--rw-r--r--   0 rmudafor (1974918542) NREL_NT\Domain Users (18434217)      258 2023-06-01 20:15:30.000000 flasc-1.3/AUTHORS.rst
--rw-r--r--   0 rmudafor (1974918542) NREL_NT\Domain Users (18434217)    11356 2023-06-01 20:15:30.000000 flasc-1.3/LICENSE.txt
--rw-r--r--   0 rmudafor (1974918542) NREL_NT\Domain Users (18434217)      620 2023-06-01 20:15:30.000000 flasc-1.3/NOTICE.txt
--rw-r--r--   0 rmudafor (1974918542) NREL_NT\Domain Users (18434217)      758 2023-06-01 20:36:46.699519 flasc-1.3/PKG-INFO
--rw-r--r--   0 rmudafor (1974918542) NREL_NT\Domain Users (18434217)     6397 2023-06-01 20:35:47.000000 flasc-1.3/README.rst
-drwxr-xr-x   0 rmudafor (1974918542) NREL_NT\Domain Users (18434217)        0 2023-06-01 20:36:46.695198 flasc-1.3/flasc/
--rw-r--r--   0 rmudafor (1974918542) NREL_NT\Domain Users (18434217)      475 2023-06-01 20:15:30.000000 flasc-1.3/flasc/__init__.py
--rw-r--r--   0 rmudafor (1974918542) NREL_NT\Domain Users (18434217)     4419 2023-06-01 20:15:30.000000 flasc-1.3/flasc/circular_statistics.py
--rw-r--r--   0 rmudafor (1974918542) NREL_NT\Domain Users (18434217)    38165 2023-06-01 20:15:30.000000 flasc-1.3/flasc/floris_tools.py
--rw-r--r--   0 rmudafor (1974918542) NREL_NT\Domain Users (18434217)     9951 2023-06-01 20:15:30.000000 flasc-1.3/flasc/optimization.py
--rw-r--r--   0 rmudafor (1974918542) NREL_NT\Domain Users (18434217)    14584 2023-06-01 20:15:30.000000 flasc-1.3/flasc/time_operations.py
--rw-r--r--   0 rmudafor (1974918542) NREL_NT\Domain Users (18434217)     6870 2023-06-01 20:15:30.000000 flasc-1.3/flasc/utilities.py
--rw-r--r--   0 rmudafor (1974918542) NREL_NT\Domain Users (18434217)        3 2023-06-01 20:15:30.000000 flasc-1.3/flasc/version.py
--rw-r--r--   0 rmudafor (1974918542) NREL_NT\Domain Users (18434217)    28151 2023-06-01 20:15:30.000000 flasc-1.3/flasc/visualization.py
-drwxr-xr-x   0 rmudafor (1974918542) NREL_NT\Domain Users (18434217)        0 2023-06-01 20:36:46.698898 flasc-1.3/flasc.egg-info/
--rw-r--r--   0 rmudafor (1974918542) NREL_NT\Domain Users (18434217)      758 2023-06-01 20:36:46.000000 flasc-1.3/flasc.egg-info/PKG-INFO
--rw-r--r--   0 rmudafor (1974918542) NREL_NT\Domain Users (18434217)      433 2023-06-01 20:36:46.000000 flasc-1.3/flasc.egg-info/SOURCES.txt
--rw-r--r--   0 rmudafor (1974918542) NREL_NT\Domain Users (18434217)        1 2023-06-01 20:36:46.000000 flasc-1.3/flasc.egg-info/dependency_links.txt
--rw-r--r--   0 rmudafor (1974918542) NREL_NT\Domain Users (18434217)       41 2023-06-01 20:36:46.000000 flasc-1.3/flasc.egg-info/entry_points.txt
--rw-r--r--   0 rmudafor (1974918542) NREL_NT\Domain Users (18434217)        1 2023-06-01 20:27:05.000000 flasc-1.3/flasc.egg-info/not-zip-safe
--rw-r--r--   0 rmudafor (1974918542) NREL_NT\Domain Users (18434217)      142 2023-06-01 20:36:46.000000 flasc-1.3/flasc.egg-info/requires.txt
--rw-r--r--   0 rmudafor (1974918542) NREL_NT\Domain Users (18434217)        6 2023-06-01 20:36:46.000000 flasc-1.3/flasc.egg-info/top_level.txt
--rw-r--r--   0 rmudafor (1974918542) NREL_NT\Domain Users (18434217)       38 2023-06-01 20:36:46.700074 flasc-1.3/setup.cfg
--rw-r--r--   0 rmudafor (1974918542) NREL_NT\Domain Users (18434217)     1876 2023-06-01 20:36:43.000000 flasc-1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:32:39.848386 flasc-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-30 22:32:25.000000 flasc-1.3.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-30 22:32:25.000000 flasc-1.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-30 22:32:25.000000 flasc-1.3.1/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-06-30 22:32:39.848386 flasc-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-06-30 22:32:25.000000 flasc-1.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:32:39.844385 flasc-1.3.1/flasc/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/circular_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:32:39.844385 flasc-1.3.1/flasc/dataframe_operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/dataframe_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/dataframe_operations/dataframe_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37601 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/dataframe_operations/dataframe_manipulations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/dataframe_operations/df_reader_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:32:39.844385 flasc-1.3.1/flasc/energy_ratio/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/energy_ratio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42675 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/energy_ratio/energy_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47208 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/energy_ratio/energy_ratio_gain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49150 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/energy_ratio/energy_ratio_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25949 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/energy_ratio/energy_ratio_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19741 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/energy_ratio/energy_ratio_wd_bias_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38165 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/floris_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:32:39.844385 flasc-1.3.1/flasc/model_estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/model_estimation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/model_estimation/floris_sensitivity_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/model_estimation/turbulence_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10052 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:32:39.844385 flasc-1.3.1/flasc/raw_data_handling/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/raw_data_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/raw_data_handling/raw_data_importing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28413 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/raw_data_handling/sqldatabase_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14584 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/time_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:32:39.844385 flasc-1.3.1/flasc/turbine_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/turbine_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/turbine_analysis/find_sensor_faults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/turbine_analysis/northing_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40581 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/turbine_analysis/ws_pow_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/turbine_analysis/yaw_pow_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28151 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:32:39.848386 flasc-1.3.1/flasc/wake_steering/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/wake_steering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/wake_steering/lookup_table_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-06-30 22:32:25.000000 flasc-1.3.1/flasc/wake_steering/yaw_optimizer_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:32:39.844385 flasc-1.3.1/flasc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-06-30 22:32:39.000000 flasc-1.3.1/flasc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-30 22:32:39.000000 flasc-1.3.1/flasc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:32:39.000000 flasc-1.3.1/flasc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 22:32:39.000000 flasc-1.3.1/flasc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:32:39.000000 flasc-1.3.1/flasc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-30 22:32:39.000000 flasc-1.3.1/flasc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 22:32:39.000000 flasc-1.3.1/flasc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-06-30 22:32:25.000000 flasc-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 22:32:39.848386 flasc-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-30 22:32:25.000000 flasc-1.3.1/setup.py
```

### Comparing `flasc-1.3/LICENSE.txt` & `flasc-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flasc-1.3/NOTICE.txt` & `flasc-1.3.1/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `flasc-1.3/README.rst` & `flasc-1.3.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-==========
+=============================================
 FLORIS-based Analysis for SCADA data (FLASC)
-==========
+=============================================
 
 **Further documentation is available at http://flasc.readthedocs.io/.**
 
 FLASC provides a rich suite of analysis tools for SCADA data
 filtering & analysis, wind farm model validation, field experiment design,
 and field experiment monitoring. The repository is centrally built around
 NRELs in-house `floris` wind farm model, available at
@@ -23,27 +23,27 @@
    :alt: Automated tests success
 
 .. image:: https://codecov.io/gh/nrel/flasc/branch/main/graph/badge.svg
    :target: https://app.codecov.io/gh/nrel/flasc/
    :alt: Code coverage
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Code formatting style
+    :target: https://github.com/psf/black
+    :alt: Code formatting style
 
 .. image:: https://img.shields.io/badge/License-Apache_2.0-blue.svg
-   :target: https://opensource.org/licenses/Apache-2.0
-   :alt: Apache 2.0 License
+    :target: https://opensource.org/licenses/Apache-2.0
+    :alt: Apache 2.0 License
 
 Installation
 ------------
 We recommend installing this repository in a separate virtual environment.
 After creating a new virtual environment, clone this repository to your local
 system and install it locally using ``pip``. The command for this is ``pip install -e flasc``.
-
+    
 Features
 --------
 FLASC consists of multiple modules, including:
 
 * *flasc.dataframe_operations*: This module includes functionality to easily manipulate pandas data frames. Functions include filtering data by wind direction, wind speed an/or TI, deriving the ambient conditions from the upstream turbines, all the while dealing with angle wrapping for angular variables.
 * *flasc.energy_ratio*: this module contains classes to calculate and visualize the energy ratio as defined by Fleming et al. (2019). The energy ratio is a very useful quantity in SCADA data analysis and related model	validation. It represents the amount of energy produced by a turbine relative to what that turbine would have produced if no wakes were present. Various classes are included in this model, from classes used to calculate and plot the energy ratio for a single dataset, a class for multiple datasets, and a class that calculates the wind direction bias for every turbine by maximizing the energy ratio fit between FLORIS and SCADA data. Various visualization methods are included such as energy ratio plots and automated generation of detailed excel spreadsheets to determine where and which turbines performed differently than expected. These methods	can be used both for model validation and for processing field campaign data, e.g. baseline vs optimized operation.
 * *flasc.floris_tools*: this module contains functions that leverage the floris model directly. This includes functions to calculate a large set of floris simulations (with MPI, optionally) for different atmospheric conditions, yaw misalignments and/or model parameters. It also includes two functions	to precalculate and respectively interpolate from a large set of model solutions to speed up further postprocessing.
```

### Comparing `flasc-1.3/flasc/circular_statistics.py` & `flasc-1.3.1/flasc/circular_statistics.py`

 * *Files identical despite different names*

### Comparing `flasc-1.3/flasc/floris_tools.py` & `flasc-1.3.1/flasc/floris_tools.py`

 * *Files identical despite different names*

### Comparing `flasc-1.3/flasc/optimization.py` & `flasc-1.3.1/flasc/optimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,15 +255,19 @@
         if angle_wrapping:
             ytest_cor = wrap_360(ytest - dy)
             y_error = np.abs(wrap_180(yref-ytest_cor))
         else:
             ytest_cor = ytest - dy
             y_error = np.abs(yref-ytest_cor)
 
-        J = np.nanmean(y_error**2.0)
+        if np.all(np.isnan(y_error)) | (len(y_error) < 1):
+            J = np.nan
+        else:
+            J = np.nanmean(y_error**2.0)
+
         if np.isnan(J_opt):
             if not np.isnan(J):
                 J_opt = J
                 dwd_opt = dy
         elif J < J_opt:
             J_opt = J
             dwd_opt = dy
```

### Comparing `flasc-1.3/flasc/time_operations.py` & `flasc-1.3.1/flasc/time_operations.py`

 * *Files identical despite different names*

### Comparing `flasc-1.3/flasc/utilities.py` & `flasc-1.3.1/flasc/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations under
 # the License.
 
 
 import datetime
 
-import numba
+# import numba
 import numpy as np
 # import scipy.interpolate as interp
 
 from floris.utilities import wrap_360
 
 
 def printnow(text, flush=True):
@@ -75,15 +75,15 @@
         y = _interpolate_with_max_gap(x, xp, fp, max_gap, False, kind)
 
     return y
 
 
 # Credits to 'np8', from https://stackoverflow.com/questions/64045034/interpolate-values-and-replace-with-nans-within-a-long-gap
 # Adapted to include nearest-neighbor interpolation
-@numba.njit()
+# @numba.njit()
 def _interpolate_with_max_gap(
     x, xp, fp, max_gap, assume_sorted=False, kind="linear", extrapolate=True,
 ):
     """
     Interpolate data linearly or using nearest-neighbor with maximum gap.
     If there is larger gap in data than `max_gap`, the gap will be filled
     with np.nan.
```

### Comparing `flasc-1.3/flasc/visualization.py` & `flasc-1.3.1/flasc/visualization.py`

 * *Files identical despite different names*

### Comparing `flasc-1.3/setup.py` & `flasc-1.3.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """The setup script."""
 
 from pathlib import Path
 from setuptools import setup, find_packages
 
 # Package meta-data.
 NAME = "flasc"
-DESCRIPTION = "FLASC provides a rich suite of analysis tools for SCADA data filtering and analysis, wind farm model validation, field experiment design, and field experiment monitoring."
+DESCRIPTION = "FLASC provides a rich suite of analysis tools for SCADA data filtering & analysis, wind farm model validation, field experiment design, and field experiment monitoring."
 URL = "https://github.com/NREL/flasc"
 EMAIL = "paul.fleming@nrel.gov"
 AUTHOR = "NREL National Wind Technology Center"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'floris>=3.4',
     'feather-format',
     'matplotlib>=3.6.3',
     'numpy',
-    'numba',
-    'openoa',
     'pandas>=1.5',
     'pyproj',
     'pytest',
     'SALib',
     'scipy',
     'sqlalchemy',
     'streamlit',
@@ -44,19 +42,19 @@
     # Placeholder
 ]
 
 setup(
     name=NAME,
     version=VERSION,
     description=DESCRIPTION,
-    # long_description=README,
+    long_description=README,
     author=AUTHOR,
     author_email=EMAIL,
     url=URL,
-    packages=find_packages(include=['flasc']),
+    packages=find_packages(include=['flasc*']),
     entry_points={
         'console_scripts': [
             'flasc=flasc.cli:main'
         ]
     },
     include_package_data=True,
     install_requires=REQUIRED,
```

