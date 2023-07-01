# Comparing `tmp/fabrics-0.7.3.tar.gz` & `tmp/fabrics-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrics-0.7.3.tar", max compression
+gzip compressed data, was "fabrics-0.7.4.tar", max compression
```

## Comparing `fabrics-0.7.3.tar` & `fabrics-0.7.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    35306 2023-06-01 01:03:50.659173 fabrics-0.7.3/LICENSE
--rw-r--r--   0        0        0     4831 2023-06-01 01:04:18.409175 fabrics-0.7.3/README.md
--rw-r--r--   0        0        0       40 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/.gitignore
--rw-r--r--   0        0        0       71 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/__init__.py
--rw-r--r--   0        0        0      249 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/components/energies/execution_energies.py
--rw-r--r--   0        0        0     3048 2023-06-01 01:04:18.517182 fabrics-0.7.3/fabrics/components/leaves/attractor.py
--rw-r--r--   0        0        0     2453 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/components/leaves/dynamic_attractor.py
--rw-r--r--   0        0        0     4365 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/components/leaves/dynamic_geometry.py
--rw-r--r--   0        0        0     2915 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/components/leaves/dynamic_leaf.py
--rw-r--r--   0        0        0     8399 2023-06-01 01:04:18.517182 fabrics-0.7.3/fabrics/components/leaves/geometry.py
--rw-r--r--   0        0        0     2307 2023-06-01 01:04:18.517182 fabrics-0.7.3/fabrics/components/leaves/leaf.py
--rw-r--r--   0        0        0     1171 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/components/maps/parameterized_maps.py
--rw-r--r--   0        0        0     1319 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/defaults/default_energies.py
--rw-r--r--   0        0        0     1609 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/defaults/default_geometries.py
--rw-r--r--   0        0        0      918 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/defaults/default_leaves.py
--rw-r--r--   0        0        0     1852 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/defaults/default_maps.py
--rw-r--r--   0        0        0      260 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/diffGeometry/casadi_helpers.py
--rw-r--r--   0        0        0     3605 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/diffGeometry/diffMap.py
--rw-r--r--   0        0        0     4016 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/diffGeometry/energized_geometry.py
--rw-r--r--   0        0        0     6868 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/diffGeometry/energy.py
--rw-r--r--   0        0        0     3416 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/diffGeometry/geometry.py
--rw-r--r--   0        0        0     6927 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/diffGeometry/spec.py
--rw-r--r--   0        0        0     2818 2023-06-01 01:03:50.815185 fabrics-0.7.3/fabrics/diffGeometry/speedControl.py
--rw-r--r--   0        0        0     6194 2023-06-01 01:04:18.517182 fabrics-0.7.3/fabrics/helpers/casadiFunctionWrapper.py
--rw-r--r--   0        0        0       75 2023-06-01 01:03:50.819185 fabrics-0.7.3/fabrics/helpers/constants.py
--rw-r--r--   0        0        0      273 2023-06-01 01:03:50.819185 fabrics-0.7.3/fabrics/helpers/exceptions.py
--rw-r--r--   0        0        0     2461 2023-06-01 01:03:50.819185 fabrics-0.7.3/fabrics/helpers/functions.py
--rw-r--r--   0        0        0     3940 2023-06-01 01:03:50.819185 fabrics-0.7.3/fabrics/helpers/variables.py
--rw-r--r--   0        0        0     6592 2023-06-01 01:04:18.517182 fabrics-0.7.3/fabrics/planner/non_holonomic_parameterized_planner.py
--rw-r--r--   0        0        0    21854 2023-06-01 01:04:18.517182 fabrics-0.7.3/fabrics/planner/parameterized_planner.py
--rw-r--r--   0        0        0     1548 2023-06-01 01:03:50.819185 fabrics-0.7.3/fabrics/planner/serialized_planner.py
--rw-r--r--   0        0        0     1045 2023-06-01 01:04:18.521183 fabrics-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     5837 1970-01-01 00:00:00.000000 fabrics-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0    35306 2023-07-01 00:59:42.639427 fabrics-0.7.4/LICENSE
+-rw-r--r--   0        0        0     4831 2023-07-01 00:59:42.639427 fabrics-0.7.4/README.md
+-rw-r--r--   0        0        0       40 2023-07-01 00:59:42.795428 fabrics-0.7.4/fabrics/.gitignore
+-rw-r--r--   0        0        0       71 2023-07-01 00:59:42.795428 fabrics-0.7.4/fabrics/__init__.py
+-rw-r--r--   0        0        0      249 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/components/energies/execution_energies.py
+-rw-r--r--   0        0        0     3048 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/components/leaves/attractor.py
+-rw-r--r--   0        0        0     2453 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/components/leaves/dynamic_attractor.py
+-rw-r--r--   0        0        0     4365 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/components/leaves/dynamic_geometry.py
+-rw-r--r--   0        0        0     2915 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/components/leaves/dynamic_leaf.py
+-rw-r--r--   0        0        0    10097 2023-07-01 01:00:11.675667 fabrics-0.7.4/fabrics/components/leaves/geometry.py
+-rw-r--r--   0        0        0     2307 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/components/leaves/leaf.py
+-rw-r--r--   0        0        0     1369 2023-07-01 01:00:11.675667 fabrics-0.7.4/fabrics/components/maps/parameterized_maps.py
+-rw-r--r--   0        0        0     1319 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/defaults/default_energies.py
+-rw-r--r--   0        0        0     1609 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/defaults/default_geometries.py
+-rw-r--r--   0        0        0      918 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/defaults/default_leaves.py
+-rw-r--r--   0        0        0     1852 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/defaults/default_maps.py
+-rw-r--r--   0        0        0      260 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/diffGeometry/casadi_helpers.py
+-rw-r--r--   0        0        0     3605 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/diffGeometry/diffMap.py
+-rw-r--r--   0        0        0     4016 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/diffGeometry/energized_geometry.py
+-rw-r--r--   0        0        0     6868 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/diffGeometry/energy.py
+-rw-r--r--   0        0        0     3364 2023-07-01 01:00:11.675667 fabrics-0.7.4/fabrics/diffGeometry/geometry.py
+-rw-r--r--   0        0        0     6934 2023-07-01 01:00:11.675667 fabrics-0.7.4/fabrics/diffGeometry/spec.py
+-rw-r--r--   0        0        0     2818 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/diffGeometry/speedControl.py
+-rw-r--r--   0        0        0     6194 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/helpers/casadiFunctionWrapper.py
+-rw-r--r--   0        0        0       75 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/helpers/constants.py
+-rw-r--r--   0        0        0      273 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/helpers/exceptions.py
+-rw-r--r--   0        0        0     2068 2023-07-01 01:00:11.675667 fabrics-0.7.4/fabrics/helpers/functions.py
+-rw-r--r--   0        0        0     3940 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/helpers/variables.py
+-rw-r--r--   0        0        0     6592 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/planner/non_holonomic_parameterized_planner.py
+-rw-r--r--   0        0        0    22532 2023-07-01 01:00:11.675667 fabrics-0.7.4/fabrics/planner/parameterized_planner.py
+-rw-r--r--   0        0        0     1548 2023-07-01 00:59:42.799428 fabrics-0.7.4/fabrics/planner/serialized_planner.py
+-rw-r--r--   0        0        0     1074 2023-07-01 01:00:11.679667 fabrics-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     5844 1970-01-01 00:00:00.000000 fabrics-0.7.4/PKG-INFO
```

### Comparing `fabrics-0.7.3/LICENSE` & `fabrics-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.3/README.md` & `fabrics-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.3/fabrics/components/leaves/attractor.py` & `fabrics-0.7.4/fabrics/components/leaves/attractor.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.3/fabrics/components/leaves/dynamic_attractor.py` & `fabrics-0.7.4/fabrics/components/leaves/dynamic_attractor.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.3/fabrics/components/leaves/dynamic_geometry.py` & `fabrics-0.7.4/fabrics/components/leaves/dynamic_geometry.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.3/fabrics/components/leaves/dynamic_leaf.py` & `fabrics-0.7.4/fabrics/components/leaves/dynamic_leaf.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.3/fabrics/components/leaves/geometry.py` & `fabrics-0.7.4/fabrics/components/leaves/geometry.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import casadi as ca
 import numpy as np
 
 from fabrics.components.maps.parameterized_maps import (
     ParameterizedObstacleMap,
+    ParameterizedPlaneConstraintMap,
 )
 from fabrics.diffGeometry.diffMap import DifferentialMap, ExplicitDifferentialMap
 from fabrics.diffGeometry.geometry import Geometry
 from fabrics.diffGeometry.energy import Lagrangian
 from fabrics.components.leaves.leaf import Leaf
 from fabrics.helpers.variables import Variables
 from fabrics.helpers.functions import parse_symbolic_input
@@ -218,7 +219,53 @@
         self._map = ExplicitDifferentialMap(
             phi_reduced,
             self._parent_variables,
             J=J,
             Jdot=Jdot,
         )
 
+class PlaneConstraintGeometryLeaf(GenericGeometryLeaf):
+    def __init__(
+            self,
+            parent_variables: Variables,
+            constraint_name: str,
+            collision_link: str,
+            collision_fk: ca.SX,
+    ):
+        self._collision_link = collision_link
+        self._collision_fk = collision_fk
+        self._constraint_name = constraint_name
+        super().__init__(
+            parent_variables,
+            f"{collision_link}_{constraint_name}",
+            collision_fk,
+        )
+        self.set_forward_map()
+
+    def set_forward_map(self):
+        q = self._parent_variables.position_variable()
+        radius_body_name = f"radius_body_{self._collision_link}"
+        if radius_body_name in self._parent_variables.parameters():
+            radius_body_variable = self._parent_variables.parameters()[
+                radius_body_name
+            ]
+        else:
+            radius_body_variable = ca.SX.sym(radius_body_name, 1)
+        if self._constraint_name in self._parent_variables.parameters():
+            constraint_variable = self._parent_variables.parameters()[
+                self._constraint_name
+            ]
+        else:
+            constraint_variable = ca.SX.sym(self._constraint_name, 4)
+        geo_parameters = {
+            radius_body_name: radius_body_variable,
+            self._constraint_name: constraint_variable,
+        }
+        self._parent_variables.add_parameters(geo_parameters)
+        self._map = ParameterizedPlaneConstraintMap(
+            self._parent_variables,
+            self._forward_kinematics,
+            constraint_variable,
+            radius_body_variable
+        )
+
+
```

### Comparing `fabrics-0.7.3/fabrics/components/leaves/leaf.py` & `fabrics-0.7.4/fabrics/components/leaves/leaf.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.3/fabrics/components/maps/parameterized_maps.py` & `fabrics-0.7.4/fabrics/components/maps/parameterized_maps.py`

 * *Files 26% similar despite different names*

```diff
@@ -25,25 +25,26 @@
         phi = (
             ca.norm_2(fk - reference_variable)
             / (radius_variable + radius_body_variable)
             - 1
         )
         super().__init__(phi, var)
 
-
-"""
-class ParameterizedObstacleMap(ParameterizedGeometryMap):
+class ParameterizedPlaneConstraintMap(ParameterizedGeometryMap):
     def __init__(
         self,
         var: Variables,
         fk,
-        reference_variable,
-        radius_variable,
+        constraint_variable,
         radius_body_variable,
     ):
-        phi = (
-            ca.norm_2(fk - reference_variable)
-            / (radius_variable + radius_body_variable)
-            - 1
-        )
-        super().__init__(phi, var=var)
-"""
+        phi = ca.fabs(ca.dot(constraint_variable[0:3], fk) + constraint_variable[3]) / ca.norm_2(constraint_variable[0:3]) - radius_body_variable
+
+        #phi = ca.fabs(a*x + b*y + c*z + d) / ((a**2 + b**2 + c**2)**0.5)
+        #phi = (
+        #    ca.norm_2(fk - reference_variable)
+        #    / (radius_variable + radius_body_variable)
+        #    - 1
+        #)
+        super().__init__(phi, var)
+
+
```

### Comparing `fabrics-0.7.3/fabrics/defaults/default_energies.py` & `fabrics-0.7.4/fabrics/defaults/default_energies.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.3/fabrics/defaults/default_geometries.py` & `fabrics-0.7.4/fabrics/defaults/default_geometries.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.3/fabrics/defaults/default_leaves.py` & `fabrics-0.7.4/fabrics/defaults/default_leaves.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.3/fabrics/defaults/default_maps.py` & `fabrics-0.7.4/fabrics/defaults/default_maps.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.3/fabrics/diffGeometry/diffMap.py` & `fabrics-0.7.4/fabrics/diffGeometry/diffMap.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.3/fabrics/diffGeometry/energized_geometry.py` & `fabrics-0.7.4/fabrics/diffGeometry/energized_geometry.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.3/fabrics/diffGeometry/energy.py` & `fabrics-0.7.4/fabrics/diffGeometry/energy.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.3/fabrics/diffGeometry/geometry.py` & `fabrics-0.7.4/fabrics/diffGeometry/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import casadi as ca
 import numpy as np
 from copy import deepcopy
 
 from fabrics.diffGeometry.diffMap import DifferentialMap, DynamicDifferentialMap
-from fabrics.helpers.functions import joinVariables
 from fabrics.helpers.variables import Variables
 from fabrics.helpers.casadiFunctionWrapper import CasadiFunctionWrapper
 
 
 class Geometry:
     """description"""
```

### Comparing `fabrics-0.7.3/fabrics/diffGeometry/spec.py` & `fabrics-0.7.4/fabrics/diffGeometry/spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import casadi as ca
 import numpy as np
 import logging
 from copy import deepcopy
 
 from fabrics.diffGeometry.diffMap import DifferentialMap, DynamicDifferentialMap
 from fabrics.helpers.constants import eps
-from fabrics.helpers.functions import joinVariables, checkCompatability
+from fabrics.helpers.functions import checkCompatability
 
 from fabrics.helpers.casadiFunctionWrapper import CasadiFunctionWrapper
 from fabrics.helpers.variables import Variables
 
 class Spec:
     """description"""
 
+    _vars: Variables
+
     def __init__(self, M: ca.SX, **kwargs):
         self._x_ref_name = "x_ref"
         self._xdot_ref_name = "xdot_ref"
         self._xddot_ref_name = "xddot_ref"
         if 'ref_names' in kwargs:
             ref_names = kwargs.get('ref_names')
             self._x_ref_name = ref_names[0]
```

### Comparing `fabrics-0.7.3/fabrics/diffGeometry/speedControl.py` & `fabrics-0.7.4/fabrics/diffGeometry/speedControl.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.3/fabrics/helpers/casadiFunctionWrapper.py` & `fabrics-0.7.4/fabrics/helpers/casadiFunctionWrapper.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.3/fabrics/helpers/functions.py` & `fabrics-0.7.4/fabrics/helpers/functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,28 +43,14 @@
         all_variables = []
     for variable in all_variables:
         if variable.name() in parameters:
             new_parameters[variable.name()] = variable
     return new_parameters, symbolic_expression
 
 
-def joinVariables(var1, var2):
-    var = var1 + var2
-    unique_items = []
-    for item in var:
-        already_exists = False
-        for u_item in unique_items:
-            if u_item.size() == item.size() and ca.is_equal(u_item, item):
-                already_exists = True
-                break
-        if not already_exists:
-            unique_items.append(item)
-    return unique_items
-
-
 def joinRefTrajs(refTrajs1, refTrajs2):
     refTrajs = refTrajs1 + refTrajs2
     unique_items = []
     for item in refTrajs:
         already_exists = False
         for u_item in unique_items:
             parameter_list_1 = list(u_item._vars.parameters().values())
```

### Comparing `fabrics-0.7.3/fabrics/helpers/variables.py` & `fabrics-0.7.4/fabrics/helpers/variables.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.3/fabrics/planner/non_holonomic_parameterized_planner.py` & `fabrics-0.7.4/fabrics/planner/non_holonomic_parameterized_planner.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.3/fabrics/planner/parameterized_planner.py` & `fabrics-0.7.4/fabrics/planner/parameterized_planner.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from fabrics.helpers.casadiFunctionWrapper import CasadiFunctionWrapper
 
 from fabrics.components.energies.execution_energies import ExecutionLagrangian
 from fabrics.components.leaves.leaf import Leaf
 from fabrics.components.leaves.attractor import GenericAttractor
 from fabrics.components.leaves.dynamic_attractor import GenericDynamicAttractor
 from fabrics.components.leaves.dynamic_geometry import DynamicObstacleLeaf, GenericDynamicGeometryLeaf
-from fabrics.components.leaves.geometry import ObstacleLeaf, LimitLeaf, SelfCollisionLeaf, GenericGeometryLeaf, ESDFGeometryLeaf
+from fabrics.components.leaves.geometry import ObstacleLeaf, LimitLeaf, PlaneConstraintGeometryLeaf, SelfCollisionLeaf, GenericGeometryLeaf, ESDFGeometryLeaf
 
 from mpscenes.goals.goal_composition import GoalComposition
 from mpscenes.goals.sub_goal import SubGoal
 
 from forwardkinematics.fksCommon.fk_creator import FkCreator
 from forwardkinematics.urdfFks.generic_urdf_fk import GenericURDFFk
 
@@ -74,14 +74,20 @@
     )
     self_collision_geometry: str = (
         "-0.5 / (x ** 1) * (-0.5 * (ca.sign(xdot) - 1)) * xdot ** 2"
     )
     self_collision_finsler: str = (
         "0.1/(x**1) * xdot**2"
     )
+    geometry_plane_constraint: str = (
+        "-0.5 / (x ** 5) * (-0.5 * (ca.sign(xdot) - 1)) * xdot ** 2"
+    )
+    finsler_plane_constraint: str = (
+        "0.1/(x**1) * xdot**2"
+    )
     attractor_potential: str = (
         "5.0 * (ca.norm_2(x) + 1 / 10 * ca.log(1 + ca.exp(-2 * 10 * ca.norm_2(x))))"
     )
     attractor_metric: str = (
         "((2.0 - 0.3) * ca.exp(-1 * (0.75 * ca.norm_2(x))**2) + 0.3) * ca.SX(np.identity(x.size()[0]))"
     )
     damper_beta: str = (
@@ -308,14 +314,15 @@
         collision_links: list = None,
         self_collision_pairs: dict = None,
         collision_links_esdf: list = None,
         goal: GoalComposition = None,
         limits: list = None,
         number_obstacles: int = 1,
         number_dynamic_obstacles: int = 0,
+        number_plane_constraints: int = 0,
         dynamic_obstacle_dimension: int = 3,
     ):
         if collision_links is None:
             collision_links = []
         if collision_links_esdf is None:
             collision_links_esdf = []
         if self_collision_pairs is None:
@@ -341,14 +348,20 @@
                 self.add_leaf(geometry)
             for i in range(number_dynamic_obstacles):
                 obstacle_name = f"obst_dynamic_{i}"
                 geometry = DynamicObstacleLeaf(self._variables, fk, obstacle_name, collision_link, reference_parameters=reference_parameter_list[i])
                 geometry.set_geometry(self.config.collision_geometry)
                 geometry.set_finsler_structure(self.config.collision_finsler)
                 self.add_leaf(geometry)
+            for i in range(number_plane_constraints):
+                constraint_name = f"constraint_{i}"
+                geometry = PlaneConstraintGeometryLeaf(self._variables, constraint_name, collision_link, fk)
+                geometry.set_geometry(self.config.geometry_plane_constraint)
+                geometry.set_finsler_structure(self.config.finsler_plane_constraint)
+                self.add_leaf(geometry)
 
 
         for collision_link in collision_links_esdf:
             fk = self.get_forward_kinematics(collision_link)
             geometry = ESDFGeometryLeaf(self._variables, collision_link, fk)
             geometry.set_geometry(self.config.collision_geometry)
             geometry.set_finsler_structure(self.config.collision_finsler)
```

### Comparing `fabrics-0.7.3/fabrics/planner/serialized_planner.py` & `fabrics-0.7.4/fabrics/planner/serialized_planner.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.7.3/pyproject.toml` & `fabrics-0.7.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "fabrics"
-version = "0.7.3"
+version = "0.7.4"
 description = "Optimization fabrics in python."
 authors = ["Max Spahn <m.spahn@tudelft.nl>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 repository = "https://tud-amr/fabrics"
 keywords = ["robotics", "motion-planning", "geometry"]
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.10"
-casadi = "^3.5.4,!=3.5.5.post1,!=3.5.5.post1"
+casadi = "^3.5.4,!=3.5.5.post1,!=3.5.5.post1,<3.6.0"
 numpy = "^1.15.3"
 geomdl = "^5.3.1"
 pyquaternion = "^0.9.9"
 pickle-mixin = "^1.0.2"
 quaternionic = "^1.0.0"
 forwardkinematics = "^1.0"
 mpscenes = "^0.3"
@@ -29,14 +29,15 @@
 pytest-cov = "^4.0.0"
 
 [tool.poetry.group.tutorials]
 optional = true
 
 [tool.poetry.group.tutorials.dependencies]
 planarenvs = "^1.3.2"
+matplotlib = "^3.7.0"
 jupyterlab = "^3.6.1"
 
 [tool.poetry.group.agents]
 optional = true
 
 [tool.poetry.group.agents.dependencies]
 urdfenvs = "^0.7.6"
```

### Comparing `fabrics-0.7.3/PKG-INFO` & `fabrics-0.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: fabrics
-Version: 0.7.3
+Version: 0.7.4
 Summary: Optimization fabrics in python.
 Home-page: https://tud-amr/fabrics
 License: GPL-3.0-or-later
 Keywords: robotics,motion-planning,geometry
 Author: Max Spahn
 Author-email: m.spahn@tudelft.nl
 Requires-Python: >=3.8,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: casadi (>=3.5.4,<4.0.0,!=3.5.5.post1,!=3.5.5.post1)
+Requires-Dist: casadi (>=3.5.4,<4.0.0,!=3.5.5.post1,!=3.5.5.post1,<3.6.0)
 Requires-Dist: forwardkinematics (>=1.0,<2.0)
 Requires-Dist: geomdl (>=5.3.1,<6.0.0)
 Requires-Dist: mpscenes (>=0.3,<0.4)
 Requires-Dist: numpy (>=1.15.3,<2.0.0)
 Requires-Dist: pickle-mixin (>=1.0.2,<2.0.0)
 Requires-Dist: pynput (>=1.7.6,<2.0.0)
 Requires-Dist: pyquaternion (>=0.9.9,<0.10.0)
```

#### html2text {}

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 2.1 Name: fabrics Version: 0.7.3 Summary: Optimization
+Metadata-Version: 2.1 Name: fabrics Version: 0.7.4 Summary: Optimization
 fabrics in python. Home-page: https://tud-amr/fabrics License: GPL-3.0-or-later
 Keywords: robotics,motion-planning,geometry Author: Max Spahn Author-email:
 m.spahn@tudelft.nl Requires-Python: >=3.8,<3.10 Classifier: License :: OSI
 Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Requires-Dist: casadi
-(>=3.5.4,<4.0.0,!=3.5.5.post1,!=3.5.5.post1) Requires-Dist: forwardkinematics
-(>=1.0,<2.0) Requires-Dist: geomdl (>=5.3.1,<6.0.0) Requires-Dist: mpscenes
-(>=0.3,<0.4) Requires-Dist: numpy (>=1.15.3,<2.0.0) Requires-Dist: pickle-mixin
-(>=1.0.2,<2.0.0) Requires-Dist: pynput (>=1.7.6,<2.0.0) Requires-Dist:
-pyquaternion (>=0.9.9,<0.10.0) Requires-Dist: quaternionic (>=1.0.0,<2.0.0)
-Project-URL: Repository, https://tud-amr/fabrics Description-Content-Type:
-text/markdown # (Geometric) Fabrics [![Build and Agents](https://github.com/
-maxspahn/fabrics/actions/workflows/diffGeo_agents.yml/badge.svg)](https://
-github.com/maxspahn/fabrics/actions/workflows/diffGeo_agents.yml) [![Build and
-Unittest](https://github.com/maxspahn/fabrics/actions/workflows/unitTest.yml/
-badge.svg)](https://github.com/maxspahn/fabrics/actions/workflows/unitTest.yml)
-**Note on development** > This project is still under heavy development and
-there is a lack of > documentation. I, @maxspahn, am committed to improve and
-maintain that package. > However, I rely on people like you to point me to
-issues and unclear sections of > the code. So feel free to leave issues
-whenever something bugs you. **Fabrics ros-wrapper** > The fabrics-ros wrapper
-will be released very shortly when compatibility is > verified. Geometric
-Fabrics represent a geometric approach to motion generation for various robot
-structures. The idea is a next development step after Riemannian Motion
-Policies and offers increased stability and accessibility.
+(>=3.5.4,<4.0.0,!=3.5.5.post1,!=3.5.5.post1,<3.6.0) Requires-Dist:
+forwardkinematics (>=1.0,<2.0) Requires-Dist: geomdl (>=5.3.1,<6.0.0) Requires-
+Dist: mpscenes (>=0.3,<0.4) Requires-Dist: numpy (>=1.15.3,<2.0.0) Requires-
+Dist: pickle-mixin (>=1.0.2,<2.0.0) Requires-Dist: pynput (>=1.7.6,<2.0.0)
+Requires-Dist: pyquaternion (>=0.9.9,<0.10.0) Requires-Dist: quaternionic
+(>=1.0.0,<2.0.0) Project-URL: Repository, https://tud-amr/fabrics Description-
+Content-Type: text/markdown # (Geometric) Fabrics [![Build and Agents](https://
+github.com/maxspahn/fabrics/actions/workflows/diffGeo_agents.yml/badge.svg)]
+(https://github.com/maxspahn/fabrics/actions/workflows/diffGeo_agents.yml) [!
+[Build and Unittest](https://github.com/maxspahn/fabrics/actions/workflows/
+unitTest.yml/badge.svg)](https://github.com/maxspahn/fabrics/actions/workflows/
+unitTest.yml) **Note on development** > This project is still under heavy
+development and there is a lack of > documentation. I, @maxspahn, am committed
+to improve and maintain that package. > However, I rely on people like you to
+point me to issues and unclear sections of > the code. So feel free to leave
+issues whenever something bugs you. **Fabrics ros-wrapper** > The fabrics-ros
+wrapper will be released very shortly when compatibility is > verified.
+Geometric Fabrics represent a geometric approach to motion generation for
+various robot structures. The idea is a next development step after Riemannian
+Motion Policies and offers increased stability and accessibility.
 Holonomic robots Non-Holonomic robots
 [1]              [1]
 [1]              [1]
 [1]
 ## Installation Install the package through pip, using ```bash pip3 install "."
 ``` or from PyPI using ```bash pip3 install fabrics ``` Options are [agents]
 and [tutorials]. Those can be installed using ``` pip3 install ".[agents]" pip3
```

