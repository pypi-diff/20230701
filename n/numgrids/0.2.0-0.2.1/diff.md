# Comparing `tmp/numgrids-0.2.0.tar.gz` & `tmp/numgrids-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numgrids-0.2.0.tar", last modified: Fri Jun 30 17:01:22 2023, max compression
+gzip compressed data, was "numgrids-0.2.1.tar", last modified: Sat Jul  1 06:20:50 2023, max compression
```

## Comparing `numgrids-0.2.0.tar` & `numgrids-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-06-30 17:01:22.091494 numgrids-0.2.0/
--rw-r--r--   0 mbaer    (671849960) 579947404     1069 2023-06-30 04:56:35.000000 numgrids-0.2.0/LICENSE
--rw-r--r--   0 mbaer    (671849960) 579947404     3789 2023-06-30 17:01:22.090686 numgrids-0.2.0/PKG-INFO
--rw-r--r--   0 mbaer    (671849960) 579947404     3397 2023-06-30 16:56:43.000000 numgrids-0.2.0/README.md
-drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-06-30 17:01:22.087443 numgrids-0.2.0/numgrids/
--rw-r--r--   0 mbaer    (671849960) 579947404      110 2023-06-30 04:50:47.000000 numgrids-0.2.0/numgrids/__init__.py
--rw-r--r--   0 mbaer    (671849960) 579947404     4547 2023-06-30 12:56:50.000000 numgrids-0.2.0/numgrids/api.py
--rw-r--r--   0 mbaer    (671849960) 579947404     7127 2023-06-30 13:37:54.000000 numgrids-0.2.0/numgrids/axes.py
--rw-r--r--   0 mbaer    (671849960) 579947404     5157 2023-06-28 14:34:51.000000 numgrids-0.2.0/numgrids/diff.py
--rw-r--r--   0 mbaer    (671849960) 579947404     1929 2023-06-30 13:36:37.000000 numgrids-0.2.0/numgrids/grids.py
--rw-r--r--   0 mbaer    (671849960) 579947404     1995 2023-06-30 04:55:14.000000 numgrids-0.2.0/numgrids/integration.py
--rw-r--r--   0 mbaer    (671849960) 579947404      426 2023-06-30 16:47:26.000000 numgrids-0.2.0/numgrids/interpol.py
--rw-r--r--   0 mbaer    (671849960) 579947404      163 2023-06-30 06:18:32.000000 numgrids-0.2.0/numgrids/utils.py
-drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-06-30 17:01:22.089881 numgrids-0.2.0/numgrids.egg-info/
--rw-r--r--   0 mbaer    (671849960) 579947404     3789 2023-06-30 17:01:22.000000 numgrids-0.2.0/numgrids.egg-info/PKG-INFO
--rw-r--r--   0 mbaer    (671849960) 579947404      337 2023-06-30 17:01:22.000000 numgrids-0.2.0/numgrids.egg-info/SOURCES.txt
--rw-r--r--   0 mbaer    (671849960) 579947404        1 2023-06-30 17:01:22.000000 numgrids-0.2.0/numgrids.egg-info/dependency_links.txt
--rw-r--r--   0 mbaer    (671849960) 579947404       31 2023-06-30 17:01:22.000000 numgrids-0.2.0/numgrids.egg-info/requires.txt
--rw-r--r--   0 mbaer    (671849960) 579947404        9 2023-06-30 17:01:22.000000 numgrids-0.2.0/numgrids.egg-info/top_level.txt
--rw-r--r--   0 mbaer    (671849960) 579947404       38 2023-06-30 17:01:22.091733 numgrids-0.2.0/setup.cfg
--rw-r--r--   0 mbaer    (671849960) 579947404      936 2023-06-30 16:57:52.000000 numgrids-0.2.0/setup.py
+drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-07-01 06:20:50.345287 numgrids-0.2.1/
+-rw-r--r--   0 mbaer    (671849960) 579947404     1069 2023-06-30 04:56:35.000000 numgrids-0.2.1/LICENSE
+-rw-r--r--   0 mbaer    (671849960) 579947404     3773 2023-07-01 06:20:50.344972 numgrids-0.2.1/PKG-INFO
+-rw-r--r--   0 mbaer    (671849960) 579947404     3381 2023-07-01 06:16:40.000000 numgrids-0.2.1/README.md
+drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-07-01 06:20:50.343011 numgrids-0.2.1/numgrids/
+-rw-r--r--   0 mbaer    (671849960) 579947404      146 2023-07-01 06:15:06.000000 numgrids-0.2.1/numgrids/__init__.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     4402 2023-07-01 06:16:12.000000 numgrids-0.2.1/numgrids/api.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     7127 2023-06-30 13:37:54.000000 numgrids-0.2.1/numgrids/axes.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     5157 2023-06-28 14:34:51.000000 numgrids-0.2.1/numgrids/diff.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     1929 2023-06-30 13:36:37.000000 numgrids-0.2.1/numgrids/grids.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     1995 2023-06-30 04:55:14.000000 numgrids-0.2.1/numgrids/integration.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     1294 2023-07-01 06:03:13.000000 numgrids-0.2.1/numgrids/interpol.py
+-rw-r--r--   0 mbaer    (671849960) 579947404      163 2023-06-30 06:18:32.000000 numgrids-0.2.1/numgrids/utils.py
+drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2023-07-01 06:20:50.344498 numgrids-0.2.1/numgrids.egg-info/
+-rw-r--r--   0 mbaer    (671849960) 579947404     3773 2023-07-01 06:20:50.000000 numgrids-0.2.1/numgrids.egg-info/PKG-INFO
+-rw-r--r--   0 mbaer    (671849960) 579947404      337 2023-07-01 06:20:50.000000 numgrids-0.2.1/numgrids.egg-info/SOURCES.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404        1 2023-07-01 06:20:50.000000 numgrids-0.2.1/numgrids.egg-info/dependency_links.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404       39 2023-07-01 06:20:50.000000 numgrids-0.2.1/numgrids.egg-info/requires.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404        9 2023-07-01 06:20:50.000000 numgrids-0.2.1/numgrids.egg-info/top_level.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404       38 2023-07-01 06:20:50.345421 numgrids-0.2.1/setup.cfg
+-rw-r--r--   0 mbaer    (671849960) 579947404      944 2023-07-01 06:20:44.000000 numgrids-0.2.1/setup.py
```

### Comparing `numgrids-0.2.0/LICENSE` & `numgrids-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `numgrids-0.2.0/PKG-INFO` & `numgrids-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: numgrids
-Version: 0.2.0
+Version: 0.2.1
 Summary: UNKNOWN
 Home-page: https://github.com/maroba/numgrids
 Author: Matthias Baer
 Author-email: matthias.r.baer@googlemail.com
 License: MIT
 Platform: ALL
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">numgrids</h1>
 <p align="center"> Working with numerical grids made easy.</p>
 
 <p align="center"><a href="https://badge.fury.io/py/numgrids"> <img src="https://badge.fury.io/py/numgrids.svg" alt="PyPI version"></a><a href=""> <img src="https://github.com/maroba/numgrids/actions/workflows/checks.yml/badge.svg" alt="build"></a><a href="https://codecov.io/gh/maroba/numgrids"> <img src="https://codecov.io/gh/maroba/numgrids/branch/main/graph/badge.svg?token=JNH9SP7BRG" alt=""></a></p>
@@ -40,23 +40,23 @@
 As a quick example, here is how you define a grid on the unit disk using polar coordinates.
 Along the azimuthal (angular) direction, choose an equidistant spacing with periodic boundary conditions:
 
 ```python
 from numgrids import *
 from numpy import pi
 
-axis_phi = Axis.of_type(AxisType.EQUIDISTANT, 50, 0, 2*pi, periodic=True)
+axis_phi = Axis(AxisType.EQUIDISTANT, 50, 0, 2*pi, periodic=True)
 ```
 
 <img src="docs/assets/equi_periodic.png" height="326">
 
 Along the radial axis, let's choose a non-equidistant spacing:
 
 ```python
-axis_radial = Axis.of_type(AxisType.CHEBYSHEV, 20, 0, 1)
+axis_radial = Axis(AxisType.CHEBYSHEV, 20, 0, 1)
 ```
 
 <img src="docs/assets/cheby.png" height="91">
 
 Now combine the axes to a grid:
 
 ```python
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: numgrids Version: 0.2.0 Summary: UNKNOWN Home-page:
+Metadata-Version: 2.1 Name: numgrids Version: 0.2.1 Summary: UNKNOWN Home-page:
 https://github.com/maroba/numgrids Author: Matthias Baer Author-email:
 matthias.r.baer@googlemail.com License: MIT Platform: ALL Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE
                             ****** numgrids ******
                     Working with numerical grids made easy.
                              [PyPI_version][build]
    [docs/assets/torus.png] [docs/assets/disk320.png] [docs/assets/cubic.png]
 **Main Features** - Quickly define numerical grids for any rectangular or
 curvilinear coordinate system - Differentiation and integration - Interpolation
 - Easy manipulation of meshed functions - Using high precision spectral methods
 (FFT + Chebyshev) wherever possible - Fully compatible with *numpy* ##
 Installation ```shell pip install numgrids ``` ## Quick Start As a quick
 example, here is how you define a grid on the unit disk using polar
 coordinates. Along the azimuthal (angular) direction, choose an equidistant
 spacing with periodic boundary conditions: ```python from numgrids import *
-from numpy import pi axis_phi = Axis.of_type(AxisType.EQUIDISTANT, 50, 0, 2*pi,
+from numpy import pi axis_phi = Axis(AxisType.EQUIDISTANT, 50, 0, 2*pi,
 periodic=True) ``` [docs/assets/equi_periodic.png] Along the radial axis, let's
-choose a non-equidistant spacing: ```python axis_radial = Axis.of_type
+choose a non-equidistant spacing: ```python axis_radial = Axis
 (AxisType.CHEBYSHEV, 20, 0, 1) ``` [docs/assets/cheby.png] Now combine the axes
 to a grid: ```python grid = Grid(axis_radial, axis_phi) ``` [docs/assets/
 disk320.png] Sample a meshed function on this grid: ```python from numpy import
 exp, sin R, Phi = grid.meshed_coords f = R**2 * sin(Phi)**2 ``` Define partial
 derivatives $\partial/\partial r$ and $\partial/\partial \varphi$ and apply
 them: ```python # second argument means derivative order, third argument means
 axis index: d_dr = Diff(grid, 1, 0) d_dphi = Diff(grid, 1, 1) df_dr = d_dr(f)
```

### Comparing `numgrids-0.2.0/README.md` & `numgrids-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -25,23 +25,23 @@
 As a quick example, here is how you define a grid on the unit disk using polar coordinates.
 Along the azimuthal (angular) direction, choose an equidistant spacing with periodic boundary conditions:
 
 ```python
 from numgrids import *
 from numpy import pi
 
-axis_phi = Axis.of_type(AxisType.EQUIDISTANT, 50, 0, 2*pi, periodic=True)
+axis_phi = Axis(AxisType.EQUIDISTANT, 50, 0, 2*pi, periodic=True)
 ```
 
 <img src="docs/assets/equi_periodic.png" height="326">
 
 Along the radial axis, let's choose a non-equidistant spacing:
 
 ```python
-axis_radial = Axis.of_type(AxisType.CHEBYSHEV, 20, 0, 1)
+axis_radial = Axis(AxisType.CHEBYSHEV, 20, 0, 1)
 ```
 
 <img src="docs/assets/cheby.png" height="91">
 
 Now combine the axes to a grid:
 
 ```python
```

#### html2text {}

```diff
@@ -6,17 +6,17 @@
 curvilinear coordinate system - Differentiation and integration - Interpolation
 - Easy manipulation of meshed functions - Using high precision spectral methods
 (FFT + Chebyshev) wherever possible - Fully compatible with *numpy* ##
 Installation ```shell pip install numgrids ``` ## Quick Start As a quick
 example, here is how you define a grid on the unit disk using polar
 coordinates. Along the azimuthal (angular) direction, choose an equidistant
 spacing with periodic boundary conditions: ```python from numgrids import *
-from numpy import pi axis_phi = Axis.of_type(AxisType.EQUIDISTANT, 50, 0, 2*pi,
+from numpy import pi axis_phi = Axis(AxisType.EQUIDISTANT, 50, 0, 2*pi,
 periodic=True) ``` [docs/assets/equi_periodic.png] Along the radial axis, let's
-choose a non-equidistant spacing: ```python axis_radial = Axis.of_type
+choose a non-equidistant spacing: ```python axis_radial = Axis
 (AxisType.CHEBYSHEV, 20, 0, 1) ``` [docs/assets/cheby.png] Now combine the axes
 to a grid: ```python grid = Grid(axis_radial, axis_phi) ``` [docs/assets/
 disk320.png] Sample a meshed function on this grid: ```python from numpy import
 exp, sin R, Phi = grid.meshed_coords f = R**2 * sin(Phi)**2 ``` Define partial
 derivatives $\partial/\partial r$ and $\partial/\partial \varphi$ and apply
 them: ```python # second argument means derivative order, third argument means
 axis index: d_dr = Diff(grid, 1, 0) d_dphi = Diff(grid, 1, 1) df_dr = d_dr(f)
```

### Comparing `numgrids-0.2.0/numgrids/api.py` & `numgrids-0.2.1/numgrids/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,20 +69,16 @@
     """
     EQUIDISTANT = "equidistant"
     EQUIDISTANT_PERIODIC = "equidistant_periodic"
     CHEBYSHEV = "chebyshev"
     LOGARITHMIC = "log"
 
 
-class Axis:
-    """Interface for creating axis objects of any kind."""
-
-    @classmethod
-    def of_type(self, axis_type, num_points, low, high, **kwargs):
-        """Creates an Axis object of a given type.
+def Axis(axis_type, num_points, low, high, **kwargs):
+    """Creates an Axis object of a given type.
 
         Parameters
         ----------
         axis_type: AxisType
             The type of axis (equidistant, periodic, logarithmic, Chebyshev, etc.)
         num_points: positive int
             Number of grid points along this axis.
@@ -92,24 +88,25 @@
             The highest coordinate value on the axis.
 
         Returns
         -------
         Axis object of specified type.
 
         """
-        if axis_type == AxisType.EQUIDISTANT:
-            return EquidistantAxis(num_points, low, high, **kwargs)
-        elif axis_type == AxisType.EQUIDISTANT_PERIODIC:
-            return EquidistantAxis(num_points, low, high, periodic=True, **kwargs)
-        elif axis_type == AxisType.CHEBYSHEV:
-            return ChebyshevAxis(num_points, low, high, **kwargs)
-        elif axis_type == AxisType.LOGARITHMIC:
-            return LogAxis(num_points, low, high, **kwargs)
-        else:
-            raise NotImplementedError(f"No such axis type: {axis_type}")
+
+    if axis_type == AxisType.EQUIDISTANT:
+        return EquidistantAxis(num_points, low, high, **kwargs)
+    elif axis_type == AxisType.EQUIDISTANT_PERIODIC:
+        return EquidistantAxis(num_points, low, high, periodic=True, **kwargs)
+    elif axis_type == AxisType.CHEBYSHEV:
+        return ChebyshevAxis(num_points, low, high, **kwargs)
+    elif axis_type == AxisType.LOGARITHMIC:
+        return LogAxis(num_points, low, high, **kwargs)
+    else:
+        raise NotImplementedError(f"No such axis type: {axis_type}")
 
 
 class SphericalGrid(Grid):
     """A spherical grid in spherical coordinates (r, theta, phi)."""
 
     def __init__(self, raxis, theta_axis, phi_axis):
         """
```

### Comparing `numgrids-0.2.0/numgrids/axes.py` & `numgrids-0.2.1/numgrids/axes.py`

 * *Files identical despite different names*

### Comparing `numgrids-0.2.0/numgrids/diff.py` & `numgrids-0.2.1/numgrids/diff.py`

 * *Files identical despite different names*

### Comparing `numgrids-0.2.0/numgrids/grids.py` & `numgrids-0.2.1/numgrids/grids.py`

 * *Files identical despite different names*

### Comparing `numgrids-0.2.0/numgrids/integration.py` & `numgrids-0.2.1/numgrids/integration.py`

 * *Files identical despite different names*

### Comparing `numgrids-0.2.0/numgrids.egg-info/PKG-INFO` & `numgrids-0.2.1/numgrids.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: numgrids
-Version: 0.2.0
+Version: 0.2.1
 Summary: UNKNOWN
 Home-page: https://github.com/maroba/numgrids
 Author: Matthias Baer
 Author-email: matthias.r.baer@googlemail.com
 License: MIT
 Platform: ALL
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">numgrids</h1>
 <p align="center"> Working with numerical grids made easy.</p>
 
 <p align="center"><a href="https://badge.fury.io/py/numgrids"> <img src="https://badge.fury.io/py/numgrids.svg" alt="PyPI version"></a><a href=""> <img src="https://github.com/maroba/numgrids/actions/workflows/checks.yml/badge.svg" alt="build"></a><a href="https://codecov.io/gh/maroba/numgrids"> <img src="https://codecov.io/gh/maroba/numgrids/branch/main/graph/badge.svg?token=JNH9SP7BRG" alt=""></a></p>
@@ -40,23 +40,23 @@
 As a quick example, here is how you define a grid on the unit disk using polar coordinates.
 Along the azimuthal (angular) direction, choose an equidistant spacing with periodic boundary conditions:
 
 ```python
 from numgrids import *
 from numpy import pi
 
-axis_phi = Axis.of_type(AxisType.EQUIDISTANT, 50, 0, 2*pi, periodic=True)
+axis_phi = Axis(AxisType.EQUIDISTANT, 50, 0, 2*pi, periodic=True)
 ```
 
 <img src="docs/assets/equi_periodic.png" height="326">
 
 Along the radial axis, let's choose a non-equidistant spacing:
 
 ```python
-axis_radial = Axis.of_type(AxisType.CHEBYSHEV, 20, 0, 1)
+axis_radial = Axis(AxisType.CHEBYSHEV, 20, 0, 1)
 ```
 
 <img src="docs/assets/cheby.png" height="91">
 
 Now combine the axes to a grid:
 
 ```python
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: numgrids Version: 0.2.0 Summary: UNKNOWN Home-page:
+Metadata-Version: 2.1 Name: numgrids Version: 0.2.1 Summary: UNKNOWN Home-page:
 https://github.com/maroba/numgrids Author: Matthias Baer Author-email:
 matthias.r.baer@googlemail.com License: MIT Platform: ALL Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE
                             ****** numgrids ******
                     Working with numerical grids made easy.
                              [PyPI_version][build]
    [docs/assets/torus.png] [docs/assets/disk320.png] [docs/assets/cubic.png]
 **Main Features** - Quickly define numerical grids for any rectangular or
 curvilinear coordinate system - Differentiation and integration - Interpolation
 - Easy manipulation of meshed functions - Using high precision spectral methods
 (FFT + Chebyshev) wherever possible - Fully compatible with *numpy* ##
 Installation ```shell pip install numgrids ``` ## Quick Start As a quick
 example, here is how you define a grid on the unit disk using polar
 coordinates. Along the azimuthal (angular) direction, choose an equidistant
 spacing with periodic boundary conditions: ```python from numgrids import *
-from numpy import pi axis_phi = Axis.of_type(AxisType.EQUIDISTANT, 50, 0, 2*pi,
+from numpy import pi axis_phi = Axis(AxisType.EQUIDISTANT, 50, 0, 2*pi,
 periodic=True) ``` [docs/assets/equi_periodic.png] Along the radial axis, let's
-choose a non-equidistant spacing: ```python axis_radial = Axis.of_type
+choose a non-equidistant spacing: ```python axis_radial = Axis
 (AxisType.CHEBYSHEV, 20, 0, 1) ``` [docs/assets/cheby.png] Now combine the axes
 to a grid: ```python grid = Grid(axis_radial, axis_phi) ``` [docs/assets/
 disk320.png] Sample a meshed function on this grid: ```python from numpy import
 exp, sin R, Phi = grid.meshed_coords f = R**2 * sin(Phi)**2 ``` Define partial
 derivatives $\partial/\partial r$ and $\partial/\partial \varphi$ and apply
 them: ```python # second argument means derivative order, third argument means
 axis index: d_dr = Diff(grid, 1, 0) d_dphi = Diff(grid, 1, 1) df_dr = d_dr(f)
```

### Comparing `numgrids-0.2.0/setup.py` & `numgrids-0.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 
 author = 'Matthias Baer'
 email = 'matthias.r.baer@googlemail.com'
 description = ''
 name = 'numgrids'
 year = '2023'
 url = 'https://github.com/maroba/numgrids'
-version = '0.2.0'
+version = '0.2.1'
 
 setup(
     name=name,
     author=author,
     author_email=email,
     url=url,
     version=version,
     packages=find_packages(),
     package_dir={name: name},
     include_package_data=True,
     license='MIT',
     description=description,
     long_description=open('README.md').read() if exists('README.md') else '',
     long_description_content_type="text/markdown",
-    install_requires=['numpy', 'scipy', 'matplotlib', 'findiff'
+    install_requires=['numpy', 'scipy>=1.10.1', 'matplotlib', 'findiff'
                       ],
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     classifiers=['Operating System :: OS Independent',
                  'Programming Language :: Python :: 3',
                  ],
     platforms=['ALL'],
 )
```

