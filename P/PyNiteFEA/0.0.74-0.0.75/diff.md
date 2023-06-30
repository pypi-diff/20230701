# Comparing `tmp/PyNiteFEA-0.0.74.tar.gz` & `tmp/PyNiteFEA-0.0.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNiteFEA-0.0.74.tar", last modified: Mon Apr 24 16:34:10 2023, max compression
+gzip compressed data, was "PyNiteFEA-0.0.75.tar", last modified: Fri Jun 30 23:37:28 2023, max compression
```

## Comparing `PyNiteFEA-0.0.74.tar` & `PyNiteFEA-0.0.75.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:34:10.288179 PyNiteFEA-0.0.74/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-04-24 16:34:10.288179 PyNiteFEA-0.0.74/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:34:10.288179 PyNiteFEA-0.0.74/PyNite/
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/BeamSegY.py
--rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/BeamSegZ.py
--rw-r--r--   0 runner    (1001) docker     (123)   152953 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/FEModel3D.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/FixedEndReactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/LoadCombo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/MainStyleSheet.css
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/Material.py
--rw-r--r--   0 runner    (1001) docker     (123)    78215 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/Member3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    67808 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/Mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/Node3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/PhysMember.py
--rw-r--r--   0 runner    (1001) docker     (123)    35570 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/Plate3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    32588 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/Quad3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    26019 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/Report_Template.html
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/Reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/Spring3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    88489 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/Visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/PyNite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:34:10.288179 PyNiteFEA-0.0.74/PyNiteFEA.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-04-24 16:34:10.000000 PyNiteFEA-0.0.74/PyNiteFEA.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-24 16:34:10.000000 PyNiteFEA-0.0.74/PyNiteFEA.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 16:34:10.000000 PyNiteFEA-0.0.74/PyNiteFEA.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-24 16:34:10.000000 PyNiteFEA-0.0.74/PyNiteFEA.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 16:34:10.000000 PyNiteFEA-0.0.74/PyNiteFEA.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 16:34:10.288179 PyNiteFEA-0.0.74/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-24 16:34:00.000000 PyNiteFEA-0.0.74/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:37:28.447581 PyNiteFEA-0.0.75/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-06-30 23:37:28.447581 PyNiteFEA-0.0.75/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:37:28.439580 PyNiteFEA-0.0.75/PyNite/
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/BeamSegY.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/BeamSegZ.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154824 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/FEModel3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/FixedEndReactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/LoadCombo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/MainStyleSheet.css
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/Material.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78215 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/Member3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67835 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/Mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/Node3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/PhysMember.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35570 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/Plate3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32588 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/Quad3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26019 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/Report_Template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/Reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/Spring3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88489 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/Visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/PyNite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:37:28.447581 PyNiteFEA-0.0.75/PyNiteFEA.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-06-30 23:37:28.000000 PyNiteFEA-0.0.75/PyNiteFEA.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-30 23:37:28.000000 PyNiteFEA-0.0.75/PyNiteFEA.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 23:37:28.000000 PyNiteFEA-0.0.75/PyNiteFEA.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-30 23:37:28.000000 PyNiteFEA-0.0.75/PyNiteFEA.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 23:37:28.000000 PyNiteFEA-0.0.75/PyNiteFEA.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 23:37:28.447581 PyNiteFEA-0.0.75/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-30 23:37:17.000000 PyNiteFEA-0.0.75/setup.py
```

### Comparing `PyNiteFEA-0.0.74/LICENSE` & `PyNiteFEA-0.0.75/LICENSE`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.74/PKG-INFO` & `PyNiteFEA-0.0.75/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNiteFEA
-Version: 0.0.74
+Version: 0.0.75
 Summary: A simple elastic 3D structural finite element library for Python.
 Home-page: https://github.com/JWock82/PyNite.git
 Author: D. Craig Brinck, PE, SE
 Author-email: Building.Code@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -57,15 +57,15 @@
 
 1. Accuracy: There are no guarantees PyNite is error free, but accuracy and correctness are a priority. When bugs or errors are identified, top priority will be given to eliminate them. PyNite's code is frequently reviewed, and its output is tested against a suite of textbook problems with known solutions using continuous integration (CI) anytime a change to the code base is made. If you do happen to find an error, please report it as an issue.
 
 2. Simplicity: There are other finite element alternatives out there with many more capabilities, but they are often lacking in documentation, written in difficult languages, or require extensive knowledge of finite element theory and/or element formulations to use. PyNite is not intended to be the most technically advanced solver out there. Rather, the goal is to provide a robust yet simple general purpose package.
 
 4. Improvement: PyNite is getting better at what it does. Each new feature provides leverage to build upon previous features in more elaborate ways. Key to improvement is (a) maintaining the core features that other features rely on, and (b) adding new features that are solid stepping stones to other features. Improvement most often happens by getting the small and simple things right incrementally, rather than with sweeping overhauls all at once.
 
-5. Collaboration: The intent is to keep PyNite free and open source. This will encourage future development and contributions. Keeping it open source will allow anyone to inspect and improve the code it runs on. If you see an area you can help PyNite improve in you are encouraged to contribute. Please follow the contributing guidelines given in this repository.
+5. Collaboration: If you see a way to improve Pynite, you are encouraged to contribute. There are many simple ways to contribute that don't take much effort. Issue reports and pull requests can be very helpful. One easy way to contribute is to add to or improve the library of simple example problems in the `Examples` folder. Please keep them relatively simple. Most users learn Pynite from following these simple examples. Another way to help Pynite without having to know too much about its internal workings is to help with the documentation files in the `docs\source` folder of this repository. These files help new users learn Pynite. If you are able to make a bigger commitment, and would like to become a regular contributor to the project, please reach out about becoming a collaborator.
 
 # Support
 Whether you just need help getting started with PyNite, or are looking to build something more complex, there are a few resources available:
 * The examples in the "Examples" folder in this repository cover a variety of simple problems. The comments in the examples provide additional guidance on how PyNite works.
 * Documentation is a work in progress and can be found on readthedocs here: https://pynite.readthedocs.io/en/latest/index.html.
 * If you're looking for more direct guidance on using PyNite, or for help coding a project, I am available on a private consulting basis. You can reach out to me directly at Building.Code@outlook.com to discuss options.
 
@@ -89,14 +89,17 @@
 Here's a list of projects that run on PyNite:
 
 * Building Code (https://building-code.herokuapp.com/) - This one is my personal side project.
 * Standard Solver (https://www.standardsolver.com/)
 * Phaenotyp (https://github.com/bewegende-Architektur/Phaenotyp) (https://youtu.be/shloSw9HjVI)
 
 # What's New?
+v0.0.75
+* Bug fix & improvements for PDF printing capabilities. Methods used to print PDF's had fallen behind updates to the rest of the program. It should be fixed now. The way PDF's are printed has changed slightly. Examples have been updated to demonstrate this and the documentation on readthedocs has been updated as well: (https://pynite.readthedocs.io/en/latest/reporting.html).
+
 v0.0.74
 * Bug fix for rectangular meshes with very close control points. The program now checks for mesh
 control points that are for all practical purposes the same and eliminates the duplicates.
 
 v0.0.73
 * Bug fix for merging duplicated plate names when using models with multiple meshes.
```

### Comparing `PyNiteFEA-0.0.74/PyNite/BeamSegY.py` & `PyNiteFEA-0.0.75/PyNite/BeamSegY.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.74/PyNite/BeamSegZ.py` & `PyNiteFEA-0.0.75/PyNite/BeamSegZ.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.74/PyNite/FEModel3D.py` & `PyNiteFEA-0.0.75/PyNite/FEModel3D.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 from PyNite.Quad3D import Quad3D
 from PyNite.Plate3D import Plate3D
 from PyNite.LoadCombo import LoadCombo
 from PyNite.Mesh import Mesh, RectangleMesh, AnnulusMesh, FrustrumMesh, CylinderMesh
 
 # %%
 class FEModel3D():
-    """A 3D finite element model.
+    """A 3D finite element model object. This object has methods and dictionaries to create, store,
+       and retrieve results from a finite element model.
     """
 
     def __init__(self):
         """Creates a new 3D finite element model.
         """
         
         # Initialize the model's various dictionaries. The dictionaries will be prepopulated with
@@ -260,16 +261,15 @@
         # Return the spring name
         return name
 
     def add_member(self, name, i_node, j_node, material, Iy, Iz, J, A, auxNode=None,
                    tension_only=False, comp_only=False):
         """Adds a new physical member to the model.
 
-        :param name: A unique user-defined name for the member. If None or "", a name will be
-                    automatically assigned
+        :param name: A unique user-defined name for the member. If ``None`` or ``""``, a name will be automatically assigned
         :type name: str
         :param i_node: The name of the i-node (start node).
         :type i_node: str
         :param j_node: The name of the j-node (end node).
         :type j_node: str
         :param material: The name of the material of the member.
         :type material: str
@@ -277,17 +277,15 @@
         :type Iy: number
         :param Iz: The moment of inertia of the member about its local z-axis.
         :type Iz: number
         :param J: The polar moment of inertia of the member.
         :type J: number
         :param A: The cross-sectional area of the member.
         :type A: number
-        :param auxNode: The name of the auxiliary node used to define the local z-axis. The default
-                        is None, in which case the program defines the axis instead of using an
-                        auxiliary node.
+        :param auxNode: The name of the auxiliary node used to define the local z-axis. The default is ``None``, in which case the program defines the axis instead of using an auxiliary node.
         :type auxNode: str, optional
         :param tension_only: Indicates if the member is tension-only, defaults to False
         :type tension_only: bool, optional
         :param comp_only: Indicates if the member is compression-only, defaults to False
         :type comp_only: bool, optional
         :raises NameError: Occurs if the specified name already exists.
         :return: The name of the member added to the model.
@@ -303,20 +301,17 @@
             count = 1
             while name in self.Members: 
                 name = "M" + str(len(self.Members)+count)
                 count += 1
                 
         # Create a new member
         if auxNode == None:
-            new_member = PhysMember(name, self.Nodes[i_node], self.Nodes[j_node], material, Iy, Iz, J,
-                                    A, model=self, tension_only=tension_only, comp_only=comp_only)
+            new_member = PhysMember(name, self.Nodes[i_node], self.Nodes[j_node], material, Iy, Iz, J, A, model=self, tension_only=tension_only, comp_only=comp_only)
         else:
-            new_member = PhysMember(name, self.Nodes[i_node], self.Nodes[j_node], material, Iy, Iz, J,
-                                    A, model=self, auxnode=self.GetAuxNode(auxNode),
-                                    tension_only=tension_only, comp_only=comp_only)
+            new_member = PhysMember(name, self.Nodes[i_node], self.Nodes[j_node], material, Iy, Iz, J, A, model=self, auxnode=self.AuxNodes[auxNode], tension_only=tension_only, comp_only=comp_only)
         
         # Add the new member to the list
         self.Members[name] = new_member
         
         # Flag the model as unsolved
         self.solution = None
 
@@ -435,56 +430,46 @@
 
         # Flag the model as unsolved
         self.solution = None
         
         #Return the quad name
         return name
 
-    def add_rectangle_mesh(self, name, mesh_size, width, height, thickness, material, kx_mod=1.0, 
-            ky_mod=1.0, origin=[0, 0, 0], plane='XY', x_control=None, y_control=None, start_node=None,
-            start_element = None, element_type='Quad'):
+    def add_rectangle_mesh(self, name, mesh_size, width, height, thickness, material, kx_mod=1.0, ky_mod=1.0, origin=[0, 0, 0], plane='XY', x_control=None, y_control=None, start_node=None, start_element = None, element_type='Quad'):
         """Adds a rectangular mesh of elements to the model.
 
         :param name: A unique name for the mesh.
         :type name: str
         :param mesh_size: The desired mesh size.
         :type mesh_size: number
         :param width: The overall width of the rectangular mesh measured along its local x-axis.
         :type width: number
         :param height: The overall height of the rectangular mesh measured along its local y-axis.
         :type height: number
         :param thickness: The thickness of each element in the mesh.
         :type thickness: number
         :param material: The name of the material for elements in the mesh.
         :type material: str
-        :param kx_mod: Stiffness modification factor for in-plane stiffness in the element's local
-                       x-direction. Defaults to 1.0 (no modification).
+        :param kx_mod: Stiffness modification factor for in-plane stiffness in the element's local x-direction. Defaults to 1.0 (no modification).
         :type kx_mod: float, optional
-        :param ky_mod: Stiffness modification factor for in-plane stiffness in the element's local
-                       y-direction. Defaults to 1.0 (no modification).
+        :param ky_mod: Stiffness modification factor for in-plane stiffness in the element's local y-direction. Defaults to 1.0 (no modification).
         :type ky_mod: float, optional
         :param origin: The origin of the regtangular mesh's local coordinate system. Defaults to [0, 0, 0]
         :type origin: list, optional
-        :param plane: The plane the mesh will be parallel to. Options are 'XY', 'YZ', and 'XZ'.
-                      Defaults to 'XY'.
+        :param plane: The plane the mesh will be parallel to. Options are 'XY', 'YZ', and 'XZ'. Defaults to 'XY'.
         :type plane: str, optional
-        :param x_control: A list of control points along the mesh's local x-axis to work into the
-                          mesh. Defaults to `None`.
+        :param x_control: A list of control points along the mesh's local x-axis to work into the mesh. Defaults to `None`.
         :type x_control: list, optional
-        :param y_control: A list of control points along the mesh's local y-axis to work into the
-                          mesh. Defaults to None.
+        :param y_control: A list of control points along the mesh's local y-axis to work into the mesh. Defaults to None.
         :type y_control: list, optional
-        :param start_node: The name of the first node in the mesh. If set to `None` the program
-                           will use the next available node name. Default is `None`.
+        :param start_node: The name of the first node in the mesh. If set to `None` the program will use the next available node name. Default is `None`.
         :type start_node: str, optional
-        :param start_element: The name of the first element in the mesh. If set to `None` the
-                              program will use the next available element name. Default is `None`.
+        :param start_element: The name of the first element in the mesh. If set to `None` the program will use the next available element name. Default is `None`.
         :type start_element: str, optional
-        :param element_type: They type of element to make the mesh out of. Either 'Quad' or 'Rect'.
-                             Defaults to 'Quad'.
+        :param element_type: They type of element to make the mesh out of. Either 'Quad' or 'Rect'. Defaults to 'Quad'.
         :type element_type: str, optional
         :raises NameError: Occurs when the specified name already exists in the model.
         :return: The name of the mesh added to the model.
         :rtype: str
         """
         
         # Check if a mesh name has been provided
@@ -577,19 +562,16 @@
 
         # Flag the model as unsolved
         self.solution = None
         
         #Return the mesh's name
         return name
 
-    def add_frustrum_mesh(self, name, mesh_size, large_radius, small_radius, height, thickness,
-                          material, kx_mod=1.0, ky_mod=1.0, origin=[0, 0, 0], axis='Y',
-                          start_node=None, start_element=None):
-        """Adds a mesh of quadrilaterals forming a frustrum (a cone intersected by a horizontal
-        plane).
+    def add_frustrum_mesh(self, name, mesh_size, large_radius, small_radius, height, thickness,material, kx_mod=1.0, ky_mod=1.0, origin=[0, 0, 0], axis='Y', start_node=None, start_element=None):
+        """Adds a mesh of quadrilaterals forming a frustrum (a cone intersected by a horizontal plane).
 
         :param name: A unique name for the mesh.
         :type name: str
         :param mesh_size: The target mesh size
         :type mesh_size: number
         :param large_radius: The larger of the two end radii.
         :type large_radius: number
@@ -597,26 +579,23 @@
         :type small_radius: number
         :param height: The height of the frustrum.
         :type height: number
         :param thickness: The thickness of the elements.
         :type thickness: number
         :param material: The name of the element material.
         :type material: str
-        :param kx_mod: Stiffness modification factor for radial stiffness in each element's local
-                       x-direction, defaults to 1 (no modification).
+        :param kx_mod: Stiffness modification factor for radial stiffness in each element's local x-direction, defaults to 1 (no modification).
         :type kx_mod: number, optional
-        :param ky_mod: Stiffness modification factor for meridional stiffness in each
-                       element's local y-direction, defaults to 1 (no modification).
+        :param ky_mod: Stiffness modification factor for meridional stiffness in each element's local y-direction, defaults to 1 (no modification).
         :type ky_mod: number, optional
         :param origin: The origin of the mesh, defaults to [0, 0, 0].
         :type origin: list, optional
         :param axis: The global axis about which the mesh will be generated, defaults to 'Y'.
         :type axis: str, optional
-        :param start_node: The name of the first node in the mesh. If set to None the program
-                           will use the next available node name, defaults to None.
+        :param start_node: The name of the first node in the mesh. If set to None the program will use the next available node name, defaults to None.
         :type start_node: str, optional
         :param start_element: The name of the first element in the mesh. If set to `None` the
                               program will use the next available element name, defaults to None
         :type start_element: str, optional
         :raises NameError: Occurs if the specified name already exists.
         :return: The name of the mesh added to the model.
         :rtype: str
@@ -648,59 +627,57 @@
         
         #Return the mesh's name
         return name
     
     def add_cylinder_mesh(self, name, mesh_size, radius, height, thickness, material, kx_mod=1,
                           ky_mod=1, origin=[0, 0, 0], axis='Y', num_elements=None, start_node=None,
                           start_element=None, element_type='Quad'):
-        """
-        Adds a mesh of elements forming a cylinder.
-
-        Parameters
-        ----------
-        name : str
-            A unique name for the mesh.
-        mesh_size : number
-            The target mesh size
-        radius : number
-            The radius of the cylinder.
-        height : number
-            The height of the cylinder.
-        thickness : number
-            Element thickness.
-        material : str
-            The name of the element material.
-        kx_mod : number
-            Stiffness modification factor for hoop stiffness in each
-            element's local x-direction. Default value is 1.0 (no
-            modification).
-        ky_mod : number
-            Stiffness modification factor for meridional stiffness in each
-            element's local y-direction. Default value is 1.0 (no
-            modification).
-        origin : list, optional
-            The origin of the mesh. The default is [0, 0, 0].
-        axis : str, optional
-            The global axis about which the mesh will be generated. The default is 'Y'.
-        num_elements : number
-            The number of elements to use to form the perimeter of each course. This is typically
-            only used if you are trying to match the nodes to another mesh's nodes. If set to
-            `None` the program will automatically calculate the number of elements to use based on
-            the mesh size. The default is None.
-        start_node : str
-            The name of the first node in the mesh. If set to `None` the program will use the next
-            available node name. Default is `None`
-        start_element : str
-            The name of the first element in the mesh. If set to `None` the program will use the
-            next available element name. Default is `None`
-        element_type : str, optional
-            The type of element to make the mesh out of. Either 'Quad' or 'Rect'. The default is
-            'Quad'.
+        """Adds a mesh of elements forming a cylinder.
 
-        """
+        :param name: A unique name for the mesh.
+        :type name: str
+        :param mesh_size: The target mesh size.
+        :type mesh_size: float
+        :param radius: The radius of the cylinder.
+        :type radius: float
+        :param height: The height of the cylinder.
+        :type height: float
+        :param thickness: Element thickness.
+        :type thickness: float
+        :param material: The name of the element material.
+        :type material: str
+        :param kx_mod: Stiffness modification factor for hoop stiffness in each element's local
+                       x-direction. Defaults to 1.0 (no modification).
+        :type kx_mod: int, optional
+        :param ky_mod: Stiffness modification factor for meridional stiffness in each element's
+                       local y-direction. Defaults to 1.0 (no modification).
+        :type ky_mod: int, optional
+        :param origin: The origin [X, Y, Z] of the mesh. Defaults to [0, 0, 0].
+        :type origin: list, optional
+        :param axis: The global axis about which the mesh will be generated. Defaults to 'Y'.
+        :type axis: str, optional
+        :param num_elements: The number of elements to use to form each course of elements. This
+                             is typically only used if you are trying to match the nodes to another
+                             mesh's nodes. If set to `None` the program will automatically
+                             calculate the number of elements to use based on the mesh size.
+                             Defaults to None.
+        :type num_elements: int, optional
+        :param start_node: The name of the first node in the mesh. If set to `None` the program
+                           will use the next available node name. Defaults to `None`.
+        :type start_node: str, optional
+        :param start_element: The name of the first element in the mesh. If set to `None` the
+                              program will use the next available element name. Defaults to `None`.
+        :type start_element: str, optional
+        :param element_type: The type of element to make the mesh out of. Either 'Quad' or 'Rect'.
+                             Defaults to 'Quad'.
+        :type element_type: str, optional
+        :raises NameError: Occurs when the specified mesh name is already being used in the model.
+        :return: The name of the mesh added to the model
+        :rtype: str
+        """            
         
         # Check if a name has been provided
         if name:
             # Check that the mesh name doesn't already exist
             if name in self.Meshes: raise NameError(f"Mesh name '{name}' already exists")
         # Give the mesh a new name if necessary
         else:
@@ -725,26 +702,19 @@
         # Flag the model as unsolved
         self.solution = None
         
         #Return the mesh's name
         return name
 
     def merge_duplicate_nodes(self, tolerance=0.001):
-        """
-        Removes duplicate nodes from the model and returns a list of the removed node names.
+        """Removes duplicate nodes from the model and returns a list of the removed node names.
 
-        Parameters
-        ----------
-        tolerance : number
-            The maximum distance between two nodes in order to consider them duplicates.
-
-        Returns
-        -------
-        remove_list : list
-            A list of th enames of the nodes that were removed.
+        :param tolerance: The maximum distance between two nodes in order to consider them
+                          duplicates. Defaults to 0.001.
+        :type tolerance: float, optional
         """
 
         # Initialize a dictionary marking where each node is used
         node_lookup = {node_name: [] for node_name in self.Nodes.keys()}
         element_dicts = ('Springs', 'Members', 'Plates', 'Quads')
         node_types = ('i_node', 'j_node', 'm_node', 'n_node')
 
@@ -836,83 +806,70 @@
         for node_name in remove_list:
             self.Nodes.pop(node_name)
         
         # Flag the model as unsolved
         self.solution = None
 
     def delete_node(self, node_name):
-        '''
-        Removes a node from the model. All nodal loads associated with the
-        node and elements attached to the node will also be removed.
-        
-        Parameters
-        ----------
-        node_name : str
-            The name of the node to be removed.
-        '''
-        
+        """Removes a node from the model. All nodal loads associated with the node and elements attached to the node will also be removed.
+
+        :param node_name: The name of the node to be removed.
+        :type node_name: str
+        """
+            
         # Remove the node. Nodal loads are stored within the node, so they
         # will be deleted automatically when the node is deleted.
         self.Nodes.pop(node_name)
         
         # Find any elements attached to the node and remove them
         self.Members = {name: member for name, member in self.Members.items() if member.i_node.name != node_name and member.j_node.name != node_name}
         self.Plates = {name: plate for name, plate in self.Plates.items() if plate.i_node.name != node_name and plate.j_node.name != node_name and plate.m_node.name != node_name and plate.n_node.name != node_name}
         self.Quads = {name: quad for name, quad in self.Quads.items() if quad.i_node.name != node_name and quad.j_node.name != node_name and quad.m_node.name != node_name and quad.n_node.name != node_name}
 
         # Flag the model as unsolved
         self.solution = None
 
     def delete_auxnode(self, auxnode_name):
-        '''
-        Removes an auxiliary node from the model.
+        """Removes an auxiliary node from the model.
 
-        Parameters
-        ----------
-        auxnode_name : str
-            The name of the auxiliary node to be removed
-        '''
+        :param auxnode_name: The name of the auxiliary node to be removed.
+        :type auxnode_name: str
+        """
 
         # Remove the auxiliary node
         self.AuxNodes.pop(auxnode_name)
 
         # Remove the auxiliary node from any members that were using it
         for member in self.Members.values():
             if member.auxNode == auxnode_name:
                 member.auxNode = None
         
         # Flag the model as unsolved
         self.solution = None
 
     def delete_spring(self, spring_name):
-        '''
-        Removes a spring from the model.
-        
-        Parameters
-        ----------
-        spring_name : str
-            The name of the spring to be removed.
-        '''
+        """Removes a spring from the model.
+
+        :param spring_name: The name of the spring to be removed.
+        :type spring_name: str
+        """
         
         # Remove the spring
         self.Springs.pop(spring_name)
 
         # Flag the model as unsolved
         self.solution = None
 
     def delete_member(self, member_name):
-        '''
-        Removes a member from the model. All member loads associated with the
-        member will also be removed.
-        
-        Parameters
-        ----------
-        member_name : str
-            The name of the member to be removed.
-        '''
+        """Removes a member from the model. All member loads associated with the member will also
+           be removed.
+
+        :param member_name: The name of the member to be removed.
+        :type member_name: str
+        """
         
         # Remove the member. Member loads are stored within the member, so they
         # will be deleted automatically when the member is deleted.
         self.Members.pop(member_name)
 
         # Flag the model as unsolved
         self.solution = None
@@ -1028,156 +985,150 @@
         if direction == 'RZ':
             node.EnforcedRZ = magnitude
         
         # Flag the model as unsolved
         self.solution = None
 
     def def_releases(self, Member, Dxi=False, Dyi=False, Dzi=False, Rxi=False, Ryi=False, Rzi=False, Dxj=False, Dyj=False, Dzj=False, Rxj=False, Ryj=False, Rzj=False):
-        '''
-        Defines member end releases.
-        
-        All member end releases will default to unreleased unless specified otherwise.
-        
-        Parameters
-        ----------
-        Member : str
-            The name of the member to have its releases modified.
-        Dxi : boolean
-            Indicates whether the member is released axially at its start.
-        Dyi : boolean
-            Indicates whether the member is released for shear in the local y-axis at its start.
-        Dzi : boolean
-            Indicates whether the member is released for shear in the local z-axis at its start.
-        Rxi : boolean
-            Indicates whether the member is released for torsion at its start.
-        Ryi : boolean
-            Indicates whether the member is released for moment about the local y-axis at its start.
-        Rzi : boolean
-            Indicates whether the member is released for moment about the local z-axis at its start.
-        Dxj : boolean
-            Indicates whether the member is released axially at its end.
-        Dyj : boolean
-            Indicates whether the member is released for shear in the local y-axis at its end.
-        Dzj : boolean
-            Indicates whether the member is released for shear in the local z-axis.
-        Rxj : boolean
-            Indicates whether the member is released for torsion at its end.
-        Ryj : boolean
-            Indicates whether the member is released for moment about the local y-axis at its end.
-        Rzj : boolean
-            Indicates whether the member is released for moment about the local z-axis at its end.
-        '''
+        """Defines member end realeses for a member. All member end releases will default to unreleased unless specified otherwise.
+
+        :param Member: The name of the member to have its releases modified.
+        :type Member: str
+        :param Dxi: Indicates whether the member is released axially at its start. Defaults to False.
+        :type Dxi: bool, optional
+        :param Dyi: Indicates whether the member is released for shear in the local y-axis at its start. Defaults to False.
+        :type Dyi: bool, optional
+        :param Dzi: Indicates whether the member is released for shear in the local z-axis at its start. Defaults to False.
+        :type Dzi: bool, optional
+        :param Rxi: Indicates whether the member is released for torsion at its start. Defaults to False.
+        :type Rxi: bool, optional
+        :param Ryi: Indicates whether the member is released for moment about the local y-axis at its start. Defaults to False.
+        :type Ryi: bool, optional
+        :param Rzi: Indicates whether the member is released for moment about the local z-axis at its start. Defaults to False.
+        :type Rzi: bool, optional
+        :param Dxj: Indicates whether the member is released axially at its end. Defaults to False.
+        :type Dxj: bool, optional
+        :param Dyj: Indicates whether the member is released for shear in the local y-axis at its end. Defaults to False.
+        :type Dyj: bool, optional
+        :param Dzj: Indicates whether the member is released for shear in the local z-axis. Defaults to False.
+        :type Dzj: bool, optional
+        :param Rxj: Indicates whether the member is released for torsion at its end. Defaults to False.
+        :type Rxj: bool, optional
+        :param Ryj: Indicates whether the member is released for moment about the local y-axis at its end. Defaults to False.
+        :type Ryj: bool, optional
+        :param Rzj: Indicates whether the member is released for moment about the local z-axis at its end. Defaults to False.
+        :type Rzj: bool, optional
+        """
         
         # Apply the end releases to the member
         self.Members[Member].Releases = [Dxi, Dyi, Dzi, Rxi, Ryi, Rzi, Dxj, Dyj, Dzj, Rxj, Ryj, Rzj]     
 
         # Flag the model as unsolved
         self.solution = None
 
     def add_load_combo(self, name, factors, combo_type='strength'):
-        '''
-        Adds a load combination to the model
+        """Adds a load combination to the model.
 
-        Parameters
-        ----------
-        name : str
-            A unique name for the load combination (e.g. '1.2D+1.6L+0.5S' or 'Gravity Combo').
-        factors : dictionary
-            A dictionary containing load cases and their corresponding factors (e.g. {'D':1.2, 'L':1.6, 'S':0.5}).
-        combo_type : str
-            A description of the type of load combination (e.g. 'strength', 'service'). Currently
-            this does nothing in the program, and is a placeholder for future features.
-        '''
+        :param name: A unique name for the load combination (e.g. '1.2D+1.6L+0.5S' or 'Gravity Combo').
+        :type name: str
+        :param factors: A dictionary containing load cases and their corresponding factors (e.g. {'D':1.2, 'L':1.6, 'S':0.5}).
+        :type factors: dict
+        :param combo_type: A description of the type of load combination (e.g. 'strength', 'service'). This has no effect on the analysis. It can be used to mark special combinations for easier filtering through them later on. Defaults to 'service'.
+        :type combo_type: str, optional
+        """            
 
         # Create a new load combination object
         new_combo = LoadCombo(name, combo_type, factors)
 
         # Add the load combination to the dictionary of load combinations
         self.LoadCombos[name] = new_combo
 
         # Flag the model as solved
         self.solution = None
 
     def add_node_load(self, Node, Direction, P, case='Case 1'):
-        '''
-        Adds a nodal load to the model.
+        """Adds a nodal load to the model.
+
+        :param Node: The name of the node where the load is being applied.
+        :type Node: str
+        :param Direction: The global direction the load is being applied in. Forces are `'FX'`,
+                          `'FY'`, and `'FZ'`. Moments are `'MX'`, `'MY'`, and `'MZ'`.
+        :type Direction: str
+        :param P: The numeric value (magnitude) of the load.
+        :type P: float
+        :param case: The name of the load case the load belongs to. Defaults to 'Case 1'.
+        :type case: str, optional
+        :raises ValueError: Occurs when an invalid load direction was specified.
+        """
         
-        Parameters
-        ----------
-        Node : str
-            The name of the node where the load is being applied.
-        Direction : {'FX', 'FY', 'FZ', 'MX', 'MY', 'MZ'}
-            The global direction the load is being applied in. Forces are 'FX', 'FY', and 'FZ'. Moments are 'MX', 'MY', and 'MZ'.
-        P : number
-            The numeric value (magnitude) of the load.
-        case : str
-            The name of the load case the load belongs to.
-        '''
         # Validate the value of Direction
         if Direction not in ('FX', 'FY', 'FZ', 'MX', 'MY', 'MZ'):
             raise ValueError(f"Direction must be 'FX', 'FY', 'FZ', 'MX', 'MY', or 'MZ'. {Direction} was given.")
         # Add the node load to the model
         self.Nodes[Node].NodeLoads.append((Direction, P, case))
 
         # Flag the model as unsolved
         self.solution = None
 
     def add_member_pt_load(self, Member, Direction, P, x, case='Case 1'):
-        '''
-        Adds a member point load to the model.
-        
-        Parameters
-        ----------
-        Member : str
-            The name of the member the load is being applied to.
-        Direction : {'Fx', 'Fy', 'Fz', 'Mx', 'My', 'Mz'}
-            The direction in which the force is to be applied. Note that
-            typical beam sign convention is used. Transverse forces acting
-            toward the beam are positive. Moments are positive if they act
-            counter-clockwise relative to the beam's local coordinate system.
-            Torsional point loads follow the right hand rule for sign convention.
-        P : number
-            The numeric value (magnitude) of the load.
-        x : number
-            The load's location along the member's local x-axis.
-        '''
+        """Adds a member point load to the model.
+
+        :param Member: The name of the member the load is being applied to.
+        :type Member: str
+        :param Direction: The direction in which the load is to be applied. Valid values are `'Fx'`,
+                          `'Fy'`, `'Fz'`, `'Mx'`, `'My'`, `'Mz'`, `'FX'`, `'FY'`, `'FZ'`, `'MX'`, `'MY'`, or `'MZ'`.
+                          Note that lower-case notation indicates use of the beam's local
+                          coordinate system, while upper-case indicates use of the model's globl
+                          coordinate system.
+        :type Direction: str
+        :param P: The numeric value (magnitude) of the load.
+        :type P: float
+        :param x: The load's location along the member's local x-axis.
+        :type x: float
+        :param case: The load case to categorize the load under. Defaults to 'Case 1'.
+        :type case: str, optional
+        :raises ValueError: Occurs when an invalid load direction has been specified.
+        """            
 
         # Validate the value of Direction
         if Direction not in ('Fx', 'Fy', 'Fz', 'FX', 'FY', 'FZ', 'Mx', 'My', 'Mz', 'MX', 'MY', 'MZ'):
             raise ValueError(f"Direction must be 'Fx', 'Fy', 'Fz', 'FX', 'FY', FZ', 'Mx', 'My', 'Mz', 'MX', 'MY', or 'MZ'. {Direction} was given.")
         
         # Add the point load to the member
         self.Members[Member].PtLoads.append((Direction, P, x, case))
         
         # Flag the model as unsolved
         self.solution = None
 
     def add_member_dist_load(self, Member, Direction, w1, w2, x1=None, x2=None, case='Case 1'):
-        '''
-        Adds a member distributed load to the model.
-        
-        Parameters
-        ----------
-        Member : str
-            The name of the member the load is being appied to
-        Direction : {'Fx', 'Fy', 'Fz'}
-            The direction in which the load is to be applied. Note that
-            typical beam sign convention is used. Forces acting toward the beam
-            are positive.
-        w1 : number
-            The starting value (magnitude) of the load.
-        w2 : number
-            The ending value (magnitude) of the load.
-        x1 : number
-            The load's start location along the member's local x-axis. If this argument
-            is not specified, the start of the member will be used.
-        x2 : number
-            The load's end location along the member's local x-axis. If this argument
-            is not specified, the end of the member will be used.
-        '''
+        """Adds a member distributed load to the model.
+
+        :param Member: The name of the member the load is being appied to.
+        :type Member: str
+        :param Direction: The direction in which the load is to be applied. Valid values are `'Fx'`,
+                          `'Fy'`, `'Fz'`, `'FX'`, `'FY'`, or `'FZ'`.
+                          Note that lower-case notation indicates use of the beam's local
+                          coordinate system, while upper-case indicates use of the model's globl
+                          coordinate system.
+        :type Direction: str
+        :param w1: The starting value (magnitude) of the load.
+        :type w1: float
+        :param w2: The ending value (magnitude) of the load.
+        :type w2: float
+        :param x1: The load's start location along the member's local x-axis. If this argument is
+                   not specified, the start of the member will be used. Defaults to `None`
+        :type x1: float, optional
+        :param x2: The load's end location along the member's local x-axis. If this argument is not
+                   specified, the end of the member will be used. Defaults to `None`.
+        :type x2: float, optional
+        :param case: _description_, defaults to 'Case 1'
+        :type case: str, optional
+        :raises ValueError: Occurs when an invalid load direction has been specified.
+        """
+       
         # Validate the value of Direction
         if Direction not in ('Fx', 'Fy', 'Fz', 'FX', 'FY', 'FZ'):
             raise ValueError(f"Direction must be 'Fx', 'Fy', 'Fz', 'FX', 'FY', or 'FZ'. {Direction} was given.")
         # Determine if a starting and ending points for the load have been specified.
         # If not, use the member start and end as defaults
         if x1 == None:
             start = 0
@@ -1192,65 +1143,59 @@
         # Add the distributed load to the member
         self.Members[Member].DistLoads.append((Direction, w1, w2, start, end, case))
         
         # Flag the model as unsolved
         self.solution = None
 
     def add_plate_surface_pressure(self, plate_name, pressure, case='Case 1'):
-        """
-        Adds a surface pressure to the rectangular plate element.
-
-        Parameters
-        ----------
-        plate_name : str
-            The name for the rectangular plate to add the surface pressure to.
-        pressure : number
-            The value for the surface pressure.
-        case : str, optional
-            The load case to add the surface pressure to. Default is 'Case 1'.
+        """Adds a surface pressure to the rectangular plate element.
         
-        """
+
+        :param plate_name: The name for the rectangular plate to add the surface pressure to.
+        :type plate_name: str
+        :param pressure: The value (magnitude) for the surface pressure.
+        :type pressure: float
+        :param case: The load case to add the surface pressure to. Defaults to 'Case 1'.
+        :type case: str, optional
+        :raises Exception: Occurs when an invalid plate name has been specified.
+        """   
 
         # Add the surface pressure to the rectangle
         if plate_name in self.Plates.keys():
             self.Plates[plate_name].pressures.append([pressure, case])
         else:
             raise Exception('Invalid plate name specified for plate surface pressure.')
         
         # Flag the model as unsolved
         self.solution = None
 
     def add_quad_surface_pressure(self, quad_name, pressure, case='Case 1'):
-        """
-        Adds a surface pressure to the quadrilateral element.
+        """Adds a surface pressure to the quadrilateral element.
 
-        Parameters
-        ----------
-        quad_name : str
-            The name for the quad to add the surface pressure to.
-        pressure : number
-            The value for the surface pressure.
-        case : str, optional
-            The load case to add the surface pressure to. Default is 'Case 1'.
-        
+        :param quad_name: The name for the quad to add the surface pressure to.
+        :type quad_name: str
+        :param pressure: The value (magnitude) for the surface pressure.
+        :type pressure: float
+        :param case: The load case to add the surface pressure to. Defaults to 'Case 1'.
+        :type case: str, optional
+        :raises Exception: Occurs when an invalid quad name has been specified.
         """
 
         # Add the surface pressure to the quadrilateral
         if quad_name in self.Quads.keys():
             self.Quads[quad_name].pressures.append([pressure, case])
         else:
             raise Exception('Invalid quad name specified for quad surface pressure.')
         
         # Flag the model as unsolved
         self.solution = None
 
     def delete_loads(self):
-        '''
-        Deletes all loads from the model along with any results based on the loads.
-        '''
+        """Deletes all loads from the model along with any results based on the loads.
+        """
 
         # Delete the member loads and the calculated internal forces
         for member in self.Members.values():
             member.DistLoads = []
             member.PtLoads = []
             member.SegmentsZ = []
             member.SegmentsY = []
@@ -1693,34 +1638,28 @@
             if sparse: self._check_stability(K.tocsr())
             else: self._check_stability(K)
 
         # Return the global stiffness matrix
         return K    
    
     def Kg(self, combo_name='Combo 1', log=False, sparse=True):
-        """
-        Returns the model's global geometric stiffness matrix.
+        """Returns the model's global geometric stiffness matrix. The model must have a static
+           solution prior to obtaining the geometric stiffness matrix. Stiffness of plates is not
+           included.
 
-        The model must have a static solution prior to obtaining the geometric stiffness matrix.
-        Stiffness of plates is not included.
-
-        Parameters
-        ----------
-        combo_name : str, optional.
-            The name of the load combination to derive the matrix for (not the load combination itself).
-        log : bool, optional
-            Prints updates to the console if set to True. Default is False.
-        sparse : bool, optional
-            Returns a sparse matrix if set to True, and a dense matrix
-            otherwise. Default is True.
-                
-        Returns
-        -------
-        Kg : ndarray or coo_matrix
-            The global geometric stiffness matrix for the structure.
+        :param combo_name: The name of the load combination to derive the matrix for. Defaults to
+                           'Combo 1'.
+        :type combo_name: str, optional
+        :param log: Prints updates to the console if set to `True`. Defaults to `False`.
+        :type log: bool, optional
+        :param sparse: Returns a sparse matrix if set to `True`, and a dense matrix otherwise.
+                       Defaults to `True`.
+        :type sparse: bool, optional
+        :return: The global geometric stiffness matrix for the structure.
+        :rtype: ndarray or coo_matrix
         """
         
         if sparse == True:
             # Initialize a zero matrix to hold all the stiffness terms. The matrix will be stored as a
             # scipy sparse `lil_matrix`. This matrix format has several advantages. It uses less memory
             # if the matrix is sparse, supports slicing, and can be converted to other formats (sparse
             # or dense) later on for mathematical operations.
@@ -1876,22 +1815,22 @@
                 # Now that 'm' is known, place the term in the global fixed end reaction vector
                 FER[m, 0] += quad_FER[a, 0]
 
         # Return the global fixed end reaction vector
         return FER
     
     def P(self, combo_name='Combo 1'):
-        '''
-        Assembles and returns the global nodal force vector.
+        """Assembles and returns the global nodal force vector.
 
-        Parameters
-        ----------
-        combo_name : str
-            The name of the load combination to get the force vector for (not the load combination itself).
-        '''
+        :param combo_name: The name of the load combination to get the force vector for. Defaults
+                           to 'Combo 1'.
+        :type combo_name: str, optional
+        :return: The global nodal force vector.
+        :rtype: array
+        """
             
         # Initialize a zero vector to hold all the terms
         P = zeros((len(self.Nodes)*6, 1))
         
         # Get the load combination for the given 'combo_name'
         combo = self.LoadCombos[combo_name]
 
@@ -1935,27 +1874,25 @@
         :rtype: array
         """
  
         # Return the global displacement vector
         return self._D[combo_name]
 
     def _partition(self, unp_matrix, D1_indices, D2_indices):
-        '''
-        Partitions a matrix (or vector) into submatrices (or subvectors) based on degree of freedom
-        boundary conditions.
+        """Partitions a matrix (or vector) into submatrices (or subvectors) based on degree of freedom boundary conditions.
 
-        Parameters
-        ----------
-        unp_matrix : ndarray or lil_matrix
-            The unpartitioned matrix (or vector) to be partitioned.
-        D1_indices : list
-            A list of the indices for degrees of freedom that have unknown displacements.
-        D2_indices : list
-            A list of the indices for degrees of freedom that have known displacements.
-        '''
+        :param unp_matrix: The unpartitioned matrix (or vector) to be partitioned.
+        :type unp_matrix: ndarray or lil_matrix
+        :param D1_indices: A list of the indices for degrees of freedom that have unknown displacements.
+        :type D1_indices: list
+        :param D2_indices: A list of the indices for degrees of freedom that have known displacements.
+        :type D2_indices: list
+        :return: Partitioned submatrices (or subvectors) based on degree of freedom boundary conditions.
+        :rtype: array, array, array, array
+        """
 
         # Determine if this is a 1D vector or a 2D matrix
 
         # 1D vectors
         if unp_matrix.shape[1] == 1:
             # Partition the vector into 2 subvectors
             m1 = unp_matrix[D1_indices, :]
@@ -1967,36 +1904,28 @@
             m11 = unp_matrix[D1_indices, :][:, D1_indices]
             m12 = unp_matrix[D1_indices, :][:, D2_indices]
             m21 = unp_matrix[D2_indices, :][:, D1_indices]
             m22 = unp_matrix[D2_indices, :][:, D2_indices]
             return m11, m12, m21, m22
 
     def analyze(self, log=False, check_stability=True, check_statics=False, max_iter=30, sparse=True):
-        """
-        Performs first-order static analysis.
-        
-        Iterations are performed if tension-only members or
-        compression-only members are present.
+        """Performs first-order static analysis. Iterations are performed if tension-only members or compression-only members are present.
 
-
-        Parameters
-        ----------
-        log : bool, optional
-            Prints the analysis log to the console if set to True. Default is False.
-        check_statics : bool, optional
-            When set to True, causes a statics check to be performed
-        max_iter : number, optional
-            The maximum number of iterations to try to get convergence
-            for tension/compression-only analysis.
-        sparse : bool, optional
-            Indicates whether the sparse matrix solver should be used. A matrix can be considered
-            sparse or dense depening on how many zero terms there are. Structural stiffness
-            matrices often contain many zero terms. The sparse solver can offer faster solutions
-            for such matrices. Using the sparse solver on dense matrices may lead to slower
-            solution times.
+        :param log: Prints the analysis log to the console if set to True. Default is False.
+        :type log: bool, optional
+        :param check_stability: When set to `True`, checks for nodal instabilities. This slows down analysis a little. Default is `True`.
+        :type check_stability: bool, optional
+        :param check_statics: When set to `True`, causes a statics check to be performed
+        :type check_statics: bool, optional
+        :param max_iter: The maximum number of iterations to try to get convergence for tension/compression-only analysis. Defaults to 30.
+        :type max_iter: int, optional
+        :param sparse: Indicates whether the sparse matrix solver should be used. A matrix can be considered sparse or dense depening on how many zero terms there are. Structural stiffness matrices often contain many zero terms. The sparse solver can offer faster solutions for such matrices. Using the sparse solver on dense matrices may lead to slower solution times.
+        :type sparse: bool, optional
+        :raises Exception: _description_
+        :raises Exception: _description_
         """
 
         if log:
             print('+-----------+')
             print('| Analyzing |')
             print('+-----------+')
```

### Comparing `PyNiteFEA-0.0.74/PyNite/FixedEndReactions.py` & `PyNiteFEA-0.0.75/PyNite/FixedEndReactions.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.74/PyNite/MainStyleSheet.css` & `PyNiteFEA-0.0.75/PyNite/MainStyleSheet.css`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.74/PyNite/Member3D.py` & `PyNiteFEA-0.0.75/PyNite/Member3D.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.74/PyNite/Mesh.py` & `PyNiteFEA-0.0.75/PyNite/Mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -444,31 +444,31 @@
 
         # Add the mesh's boundaries to the list of control points
         x_control.append(0)
         x_control.append(width)
         y_control.append(0)
         y_control.append(height)
 
-        # Sort the control points and remove duplicate values
+        # Sort the control points in ascending order
         x_control = sorted(x_control)
         y_control = sorted(y_control)
 
         # Remove any values that are duplicates or near duplicates from `x_control`
         unique_list = []
         for i in range(len(x_control) - 1):
-            # Only keep the value at `i` if it's not a duplicate or near duplicate
+            # Only keep the value at `i` if it's not a duplicate or near duplicate of the next value
             if not isclose(x_control[i], x_control[i+1]):
                 unique_list.append(x_control[i])
         unique_list.append(x_control[-1])
         x_control = unique_list
 
         # Remove any values that are duplicates or near duplicates from `y_control`
         unique_list = []
         for i in range(len(y_control) - 1):
-            # Only keep the value at `i` if it's not a duplicate or near duplicate
+            # Only keep the value at `i` if it's not a duplicate or near duplicate of the next value
             if not isclose(y_control[i], y_control[i+1]):
                 unique_list.append(y_control[i])
         unique_list.append(y_control[-1])
         y_control = unique_list
     
         # Each node number will be increased by the offset calculated below
         node_offset = int(self.start_node[1:]) - 1
```

### Comparing `PyNiteFEA-0.0.74/PyNite/Node3D.py` & `PyNiteFEA-0.0.75/PyNite/Node3D.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.74/PyNite/PhysMember.py` & `PyNiteFEA-0.0.75/PyNite/PhysMember.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.74/PyNite/Plate3D.py` & `PyNiteFEA-0.0.75/PyNite/Plate3D.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.74/PyNite/Quad3D.py` & `PyNiteFEA-0.0.75/PyNite/Quad3D.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.74/PyNite/Report_Template.html` & `PyNiteFEA-0.0.75/PyNite/Report_Template.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <!DOCTYPE html>
 <html>
 
     <head>
-        <h1>PyNite Analysis Report</h1>
+        <h1>Pynite Analysis Report</h1>
     </head>
 
     <body>
 
         {% if node_table == True %}
         <h3>Nodes & Supports</h3>     
         <table>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-****** PyNite Analysis Report ******
+****** Pynite Analysis Report ******
 {% if node_table == True %}
 **** Nodes & Supports ****
 Node      X        Y        Z        Support X       Support Y       Support Z       Support RX      Support RY      Support RZ
 {         {        {        {        {               {               {               {               {               {
 {         { "%.4g" { "%.4g" { "%.4g" {               {               {               {               {               {
 node.name | format | format | format node.support_DX node.support_DY node.support_DZ node.support_RX node.support_RY node.support_RZ
 }}        (node.X) (node.Y) (node.Z) }}              }}              }}              }}              }}              }}
```

### Comparing `PyNiteFEA-0.0.74/PyNite/Spring3D.py` & `PyNiteFEA-0.0.75/PyNite/Spring3D.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.74/PyNite/Visualization.py` & `PyNiteFEA-0.0.75/PyNite/Visualization.py`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.74/PyNiteFEA.egg-info/PKG-INFO` & `PyNiteFEA-0.0.75/PyNiteFEA.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNiteFEA
-Version: 0.0.74
+Version: 0.0.75
 Summary: A simple elastic 3D structural finite element library for Python.
 Home-page: https://github.com/JWock82/PyNite.git
 Author: D. Craig Brinck, PE, SE
 Author-email: Building.Code@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -57,15 +57,15 @@
 
 1. Accuracy: There are no guarantees PyNite is error free, but accuracy and correctness are a priority. When bugs or errors are identified, top priority will be given to eliminate them. PyNite's code is frequently reviewed, and its output is tested against a suite of textbook problems with known solutions using continuous integration (CI) anytime a change to the code base is made. If you do happen to find an error, please report it as an issue.
 
 2. Simplicity: There are other finite element alternatives out there with many more capabilities, but they are often lacking in documentation, written in difficult languages, or require extensive knowledge of finite element theory and/or element formulations to use. PyNite is not intended to be the most technically advanced solver out there. Rather, the goal is to provide a robust yet simple general purpose package.
 
 4. Improvement: PyNite is getting better at what it does. Each new feature provides leverage to build upon previous features in more elaborate ways. Key to improvement is (a) maintaining the core features that other features rely on, and (b) adding new features that are solid stepping stones to other features. Improvement most often happens by getting the small and simple things right incrementally, rather than with sweeping overhauls all at once.
 
-5. Collaboration: The intent is to keep PyNite free and open source. This will encourage future development and contributions. Keeping it open source will allow anyone to inspect and improve the code it runs on. If you see an area you can help PyNite improve in you are encouraged to contribute. Please follow the contributing guidelines given in this repository.
+5. Collaboration: If you see a way to improve Pynite, you are encouraged to contribute. There are many simple ways to contribute that don't take much effort. Issue reports and pull requests can be very helpful. One easy way to contribute is to add to or improve the library of simple example problems in the `Examples` folder. Please keep them relatively simple. Most users learn Pynite from following these simple examples. Another way to help Pynite without having to know too much about its internal workings is to help with the documentation files in the `docs\source` folder of this repository. These files help new users learn Pynite. If you are able to make a bigger commitment, and would like to become a regular contributor to the project, please reach out about becoming a collaborator.
 
 # Support
 Whether you just need help getting started with PyNite, or are looking to build something more complex, there are a few resources available:
 * The examples in the "Examples" folder in this repository cover a variety of simple problems. The comments in the examples provide additional guidance on how PyNite works.
 * Documentation is a work in progress and can be found on readthedocs here: https://pynite.readthedocs.io/en/latest/index.html.
 * If you're looking for more direct guidance on using PyNite, or for help coding a project, I am available on a private consulting basis. You can reach out to me directly at Building.Code@outlook.com to discuss options.
 
@@ -89,14 +89,17 @@
 Here's a list of projects that run on PyNite:
 
 * Building Code (https://building-code.herokuapp.com/) - This one is my personal side project.
 * Standard Solver (https://www.standardsolver.com/)
 * Phaenotyp (https://github.com/bewegende-Architektur/Phaenotyp) (https://youtu.be/shloSw9HjVI)
 
 # What's New?
+v0.0.75
+* Bug fix & improvements for PDF printing capabilities. Methods used to print PDF's had fallen behind updates to the rest of the program. It should be fixed now. The way PDF's are printed has changed slightly. Examples have been updated to demonstrate this and the documentation on readthedocs has been updated as well: (https://pynite.readthedocs.io/en/latest/reporting.html).
+
 v0.0.74
 * Bug fix for rectangular meshes with very close control points. The program now checks for mesh
 control points that are for all practical purposes the same and eliminates the duplicates.
 
 v0.0.73
 * Bug fix for merging duplicated plate names when using models with multiple meshes.
```

### Comparing `PyNiteFEA-0.0.74/PyNiteFEA.egg-info/SOURCES.txt` & `PyNiteFEA-0.0.75/PyNiteFEA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyNiteFEA-0.0.74/README.md` & `PyNiteFEA-0.0.75/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 1. Accuracy: There are no guarantees PyNite is error free, but accuracy and correctness are a priority. When bugs or errors are identified, top priority will be given to eliminate them. PyNite's code is frequently reviewed, and its output is tested against a suite of textbook problems with known solutions using continuous integration (CI) anytime a change to the code base is made. If you do happen to find an error, please report it as an issue.
 
 2. Simplicity: There are other finite element alternatives out there with many more capabilities, but they are often lacking in documentation, written in difficult languages, or require extensive knowledge of finite element theory and/or element formulations to use. PyNite is not intended to be the most technically advanced solver out there. Rather, the goal is to provide a robust yet simple general purpose package.
 
 4. Improvement: PyNite is getting better at what it does. Each new feature provides leverage to build upon previous features in more elaborate ways. Key to improvement is (a) maintaining the core features that other features rely on, and (b) adding new features that are solid stepping stones to other features. Improvement most often happens by getting the small and simple things right incrementally, rather than with sweeping overhauls all at once.
 
-5. Collaboration: The intent is to keep PyNite free and open source. This will encourage future development and contributions. Keeping it open source will allow anyone to inspect and improve the code it runs on. If you see an area you can help PyNite improve in you are encouraged to contribute. Please follow the contributing guidelines given in this repository.
+5. Collaboration: If you see a way to improve Pynite, you are encouraged to contribute. There are many simple ways to contribute that don't take much effort. Issue reports and pull requests can be very helpful. One easy way to contribute is to add to or improve the library of simple example problems in the `Examples` folder. Please keep them relatively simple. Most users learn Pynite from following these simple examples. Another way to help Pynite without having to know too much about its internal workings is to help with the documentation files in the `docs\source` folder of this repository. These files help new users learn Pynite. If you are able to make a bigger commitment, and would like to become a regular contributor to the project, please reach out about becoming a collaborator.
 
 # Support
 Whether you just need help getting started with PyNite, or are looking to build something more complex, there are a few resources available:
 * The examples in the "Examples" folder in this repository cover a variety of simple problems. The comments in the examples provide additional guidance on how PyNite works.
 * Documentation is a work in progress and can be found on readthedocs here: https://pynite.readthedocs.io/en/latest/index.html.
 * If you're looking for more direct guidance on using PyNite, or for help coding a project, I am available on a private consulting basis. You can reach out to me directly at Building.Code@outlook.com to discuss options.
 
@@ -70,14 +70,17 @@
 Here's a list of projects that run on PyNite:
 
 * Building Code (https://building-code.herokuapp.com/) - This one is my personal side project.
 * Standard Solver (https://www.standardsolver.com/)
 * Phaenotyp (https://github.com/bewegende-Architektur/Phaenotyp) (https://youtu.be/shloSw9HjVI)
 
 # What's New?
+v0.0.75
+* Bug fix & improvements for PDF printing capabilities. Methods used to print PDF's had fallen behind updates to the rest of the program. It should be fixed now. The way PDF's are printed has changed slightly. Examples have been updated to demonstrate this and the documentation on readthedocs has been updated as well: (https://pynite.readthedocs.io/en/latest/reporting.html).
+
 v0.0.74
 * Bug fix for rectangular meshes with very close control points. The program now checks for mesh
 control points that are for all practical purposes the same and eliminates the duplicates.
 
 v0.0.73
 * Bug fix for merging duplicated plate names when using models with multiple meshes.
```

### Comparing `PyNiteFEA-0.0.74/setup.py` & `PyNiteFEA-0.0.75/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PyNiteFEA",
-    version="0.0.74",
+    version="0.0.75",
     author="D. Craig Brinck, PE, SE",
     author_email="Building.Code@outlook.com",
     description="A simple elastic 3D structural finite element library for Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JWock82/PyNite.git",
     packages=setuptools.find_packages(include=['PyNite', 'Pynite.*']),
```

