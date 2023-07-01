# Comparing `tmp/PyCompGeomAlgorithms-1.0.7.tar.gz` & `tmp/PyCompGeomAlgorithms-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCompGeomAlgorithms-1.0.7.tar", last modified: Thu Jun 29 09:03:12 2023, max compression
+gzip compressed data, was "PyCompGeomAlgorithms-1.0.8.tar", last modified: Sat Jul  1 09:14:26 2023, max compression
```

## Comparing `PyCompGeomAlgorithms-1.0.7.tar` & `PyCompGeomAlgorithms-1.0.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 09:03:12.029963 PyCompGeomAlgorithms-1.0.7/
--rw-rw-rw-   0        0        0     1104 2023-06-22 11:36:14.000000 PyCompGeomAlgorithms-1.0.7/LICENSE
--rw-rw-rw-   0        0        0      480 2023-06-29 09:03:12.028966 PyCompGeomAlgorithms-1.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-29 09:03:11.982122 PyCompGeomAlgorithms-1.0.7/PyCompGeomAlgorithms/
--rw-rw-rw-   0        0        0        0 2023-06-22 07:54:06.000000 PyCompGeomAlgorithms-1.0.7/PyCompGeomAlgorithms/__init__.py
--rw-rw-rw-   0        0        0    11303 2023-06-27 08:22:07.000000 PyCompGeomAlgorithms-1.0.7/PyCompGeomAlgorithms/core.py
--rw-rw-rw-   0        0        0     2916 2023-06-29 08:57:40.000000 PyCompGeomAlgorithms-1.0.7/PyCompGeomAlgorithms/graham.py
--rw-rw-rw-   0        0        0      920 2023-06-22 10:15:40.000000 PyCompGeomAlgorithms-1.0.7/PyCompGeomAlgorithms/jarvis.py
--rw-rw-rw-   0        0        0     2536 2023-06-22 08:22:43.000000 PyCompGeomAlgorithms-1.0.7/PyCompGeomAlgorithms/kd_tree.py
--rw-rw-rw-   0        0        0     2762 2023-06-27 08:36:35.000000 PyCompGeomAlgorithms-1.0.7/PyCompGeomAlgorithms/preparata.py
--rw-rw-rw-   0        0        0     2359 2023-06-27 08:34:18.000000 PyCompGeomAlgorithms-1.0.7/PyCompGeomAlgorithms/quickhull.py
-drwxrwxrwx   0        0        0        0 2023-06-29 09:03:12.010028 PyCompGeomAlgorithms-1.0.7/PyCompGeomAlgorithms.egg-info/
--rw-rw-rw-   0        0        0      480 2023-06-29 09:03:11.000000 PyCompGeomAlgorithms-1.0.7/PyCompGeomAlgorithms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      714 2023-06-29 09:03:11.000000 PyCompGeomAlgorithms-1.0.7/PyCompGeomAlgorithms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 09:03:11.000000 PyCompGeomAlgorithms-1.0.7/PyCompGeomAlgorithms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-29 09:03:11.000000 PyCompGeomAlgorithms-1.0.7/PyCompGeomAlgorithms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2199 2023-06-22 12:13:13.000000 PyCompGeomAlgorithms-1.0.7/README.md
--rw-rw-rw-   0        0        0       88 2023-06-22 19:12:11.000000 PyCompGeomAlgorithms-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-29 09:03:12.029963 PyCompGeomAlgorithms-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      702 2023-06-29 09:02:15.000000 PyCompGeomAlgorithms-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 09:03:12.012022 PyCompGeomAlgorithms-1.0.7/tests/
--rw-rw-rw-   0        0        0        0 2023-06-22 07:57:15.000000 PyCompGeomAlgorithms-1.0.7/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 09:03:12.024979 PyCompGeomAlgorithms-1.0.7/tests/algorithms/
--rw-rw-rw-   0        0        0        0 2023-06-22 07:57:09.000000 PyCompGeomAlgorithms-1.0.7/tests/algorithms/__init__.py
--rw-rw-rw-   0        0        0     5326 2023-06-29 09:02:05.000000 PyCompGeomAlgorithms-1.0.7/tests/algorithms/test_graham.py
--rw-rw-rw-   0        0        0      605 2023-06-26 14:33:11.000000 PyCompGeomAlgorithms-1.0.7/tests/algorithms/test_jarvis.py
--rw-rw-rw-   0        0        0     2521 2023-06-27 08:19:04.000000 PyCompGeomAlgorithms-1.0.7/tests/algorithms/test_kd_tree.py
--rw-rw-rw-   0        0        0     3424 2023-06-27 08:19:50.000000 PyCompGeomAlgorithms-1.0.7/tests/algorithms/test_preparata.py
--rw-rw-rw-   0        0        0     3304 2023-06-27 08:34:51.000000 PyCompGeomAlgorithms-1.0.7/tests/algorithms/test_quickhull.py
-drwxrwxrwx   0        0        0        0 2023-06-29 09:03:12.027968 PyCompGeomAlgorithms-1.0.7/tests/entities/
--rw-rw-rw-   0        0        0        0 2023-06-26 14:32:45.000000 PyCompGeomAlgorithms-1.0.7/tests/entities/__init__.py
--rw-rw-rw-   0        0        0     1866 2023-06-26 14:32:52.000000 PyCompGeomAlgorithms-1.0.7/tests/entities/test_entities.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:14:26.666850 PyCompGeomAlgorithms-1.0.8/
+-rw-rw-rw-   0        0        0     1104 2023-06-22 11:36:14.000000 PyCompGeomAlgorithms-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0      480 2023-07-01 09:14:26.665854 PyCompGeomAlgorithms-1.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-01 09:14:26.622000 PyCompGeomAlgorithms-1.0.8/PyCompGeomAlgorithms/
+-rw-rw-rw-   0        0        0        0 2023-06-22 07:54:06.000000 PyCompGeomAlgorithms-1.0.8/PyCompGeomAlgorithms/__init__.py
+-rw-rw-rw-   0        0        0    12246 2023-07-01 09:13:28.000000 PyCompGeomAlgorithms-1.0.8/PyCompGeomAlgorithms/core.py
+-rw-rw-rw-   0        0        0     2916 2023-07-01 09:06:52.000000 PyCompGeomAlgorithms-1.0.8/PyCompGeomAlgorithms/graham.py
+-rw-rw-rw-   0        0        0      920 2023-06-22 10:15:40.000000 PyCompGeomAlgorithms-1.0.8/PyCompGeomAlgorithms/jarvis.py
+-rw-rw-rw-   0        0        0     2536 2023-06-22 08:22:43.000000 PyCompGeomAlgorithms-1.0.8/PyCompGeomAlgorithms/kd_tree.py
+-rw-rw-rw-   0        0        0     2762 2023-06-27 08:36:35.000000 PyCompGeomAlgorithms-1.0.8/PyCompGeomAlgorithms/preparata.py
+-rw-rw-rw-   0        0        0     2359 2023-06-27 08:34:18.000000 PyCompGeomAlgorithms-1.0.8/PyCompGeomAlgorithms/quickhull.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:14:26.648918 PyCompGeomAlgorithms-1.0.8/PyCompGeomAlgorithms.egg-info/
+-rw-rw-rw-   0        0        0      480 2023-07-01 09:14:26.000000 PyCompGeomAlgorithms-1.0.8/PyCompGeomAlgorithms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      714 2023-07-01 09:14:26.000000 PyCompGeomAlgorithms-1.0.8/PyCompGeomAlgorithms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 09:14:26.000000 PyCompGeomAlgorithms-1.0.8/PyCompGeomAlgorithms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-01 09:14:26.000000 PyCompGeomAlgorithms-1.0.8/PyCompGeomAlgorithms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2199 2023-06-22 12:13:13.000000 PyCompGeomAlgorithms-1.0.8/README.md
+-rw-rw-rw-   0        0        0       88 2023-06-22 19:12:11.000000 PyCompGeomAlgorithms-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-01 09:14:26.666850 PyCompGeomAlgorithms-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      702 2023-07-01 09:13:34.000000 PyCompGeomAlgorithms-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:14:26.649907 PyCompGeomAlgorithms-1.0.8/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-22 07:57:15.000000 PyCompGeomAlgorithms-1.0.8/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:14:26.656885 PyCompGeomAlgorithms-1.0.8/tests/algorithms/
+-rw-rw-rw-   0        0        0        0 2023-06-22 07:57:09.000000 PyCompGeomAlgorithms-1.0.8/tests/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     5326 2023-06-29 09:02:05.000000 PyCompGeomAlgorithms-1.0.8/tests/algorithms/test_graham.py
+-rw-rw-rw-   0        0        0      605 2023-06-26 14:33:11.000000 PyCompGeomAlgorithms-1.0.8/tests/algorithms/test_jarvis.py
+-rw-rw-rw-   0        0        0     2521 2023-06-27 08:19:04.000000 PyCompGeomAlgorithms-1.0.8/tests/algorithms/test_kd_tree.py
+-rw-rw-rw-   0        0        0     3424 2023-06-27 08:19:50.000000 PyCompGeomAlgorithms-1.0.8/tests/algorithms/test_preparata.py
+-rw-rw-rw-   0        0        0     3304 2023-06-27 08:34:51.000000 PyCompGeomAlgorithms-1.0.8/tests/algorithms/test_quickhull.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:14:26.664859 PyCompGeomAlgorithms-1.0.8/tests/entities/
+-rw-rw-rw-   0        0        0        0 2023-06-26 14:32:45.000000 PyCompGeomAlgorithms-1.0.8/tests/entities/__init__.py
+-rw-rw-rw-   0        0        0     1866 2023-06-26 14:32:52.000000 PyCompGeomAlgorithms-1.0.8/tests/entities/test_entities.py
```

### Comparing `PyCompGeomAlgorithms-1.0.7/LICENSE` & `PyCompGeomAlgorithms-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCompGeomAlgorithms-1.0.7/PyCompGeomAlgorithms/core.py` & `PyCompGeomAlgorithms-1.0.8/PyCompGeomAlgorithms/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -204,25 +204,39 @@
         return -inf if self.b == 0 else -self.a / self.b
     
     @property
     def y_intercept(self):
         return -inf if self.b == 0 else -self.c / self.b
 
 
-
 class BinTreeNode:
     def __init__(self, data, left=None, right=None):
         self.data = data
         self.left = left
         self.right = right
     
     @property
     def is_leaf(self):
         return self.left is None and self.right is None
     
+    def traverse_preorder(self, node=None, nodes=None):
+        if node is None:
+            node = self
+        if nodes is None:
+            nodes = []
+        
+        nodes.append(node)
+
+        if node.left:
+            self.traverse_preorder(node.left, nodes)
+        if node.right:
+            self.traverse_preorder(node.right, nodes)
+        
+        return nodes
+
     def traverse_inorder(self, node=None, nodes=None):
         if node is None:
             node = self
         if nodes is None:
             nodes = []
         
         if node.left:
@@ -230,15 +244,29 @@
         
         nodes.append(node)
 
         if node.right:
             self.traverse_inorder(node.right, nodes)
         
         return nodes
-    
+
+    def traverse_postorder(self, node=None, nodes=None):
+        if node is None:
+            node = self
+        if nodes is None:
+            nodes = []
+        
+        if node.left:
+            self.traverse_postorder(node.left, nodes)
+        if node.right:
+            self.traverse_postorder(node.right, nodes)
+        
+        nodes.append(node)
+        return nodes
+
     def __eq__(self, other):
         return (
             isinstance(other, self.__class__)
             and self.data == other.data
             and self.left == other.left
             and self.right == other.right
         )
@@ -264,17 +292,23 @@
         mid = (left + right) // 2
         node = cls.node_class(iterable[mid])
         node.left = cls._from_iterable(iterable, left, mid-1)
         node.right = cls._from_iterable(iterable, mid+1, right)
 
         return node
     
+    def traverse_preorder(self):
+        return self.root.traverse_preorder()
+
     def traverse_inorder(self):
         return self.root.traverse_inorder()
     
+    def traverse_postorder(self):
+        return self.root.traverse_postorder()
+    
     def __eq__(self, other):
         return isinstance(other, self.__class__) and self.root == other.root
 
 
 class ThreadedBinTreeNode(BinTreeNode):
     def __init__(self, data):
         super().__init__(data)
```

### Comparing `PyCompGeomAlgorithms-1.0.7/PyCompGeomAlgorithms/graham.py` & `PyCompGeomAlgorithms-1.0.8/PyCompGeomAlgorithms/graham.py`

 * *Files identical despite different names*

### Comparing `PyCompGeomAlgorithms-1.0.7/PyCompGeomAlgorithms/jarvis.py` & `PyCompGeomAlgorithms-1.0.8/PyCompGeomAlgorithms/jarvis.py`

 * *Files identical despite different names*

### Comparing `PyCompGeomAlgorithms-1.0.7/PyCompGeomAlgorithms/kd_tree.py` & `PyCompGeomAlgorithms-1.0.8/PyCompGeomAlgorithms/kd_tree.py`

 * *Files identical despite different names*

### Comparing `PyCompGeomAlgorithms-1.0.7/PyCompGeomAlgorithms/preparata.py` & `PyCompGeomAlgorithms-1.0.8/PyCompGeomAlgorithms/preparata.py`

 * *Files identical despite different names*

### Comparing `PyCompGeomAlgorithms-1.0.7/PyCompGeomAlgorithms/quickhull.py` & `PyCompGeomAlgorithms-1.0.8/PyCompGeomAlgorithms/quickhull.py`

 * *Files identical despite different names*

### Comparing `PyCompGeomAlgorithms-1.0.7/PyCompGeomAlgorithms.egg-info/SOURCES.txt` & `PyCompGeomAlgorithms-1.0.8/PyCompGeomAlgorithms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyCompGeomAlgorithms-1.0.7/README.md` & `PyCompGeomAlgorithms-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `PyCompGeomAlgorithms-1.0.7/setup.py` & `PyCompGeomAlgorithms-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="PyCompGeomAlgorithms",
-    version="1.0.7",
+    version="1.0.8",
     author="artandfi (Artem Fisunenko)",
     author_email="artyom.fisunenko@gmail.com",
     description="An implementation of computational geometry algorithms in Python3.",
     packages=find_packages(),
     keywords=[
         "Python3",
         "computational geometry",
```

### Comparing `PyCompGeomAlgorithms-1.0.7/tests/algorithms/test_graham.py` & `PyCompGeomAlgorithms-1.0.8/tests/algorithms/test_graham.py`

 * *Files identical despite different names*

### Comparing `PyCompGeomAlgorithms-1.0.7/tests/algorithms/test_jarvis.py` & `PyCompGeomAlgorithms-1.0.8/tests/algorithms/test_jarvis.py`

 * *Files identical despite different names*

### Comparing `PyCompGeomAlgorithms-1.0.7/tests/algorithms/test_kd_tree.py` & `PyCompGeomAlgorithms-1.0.8/tests/algorithms/test_kd_tree.py`

 * *Files identical despite different names*

### Comparing `PyCompGeomAlgorithms-1.0.7/tests/algorithms/test_preparata.py` & `PyCompGeomAlgorithms-1.0.8/tests/algorithms/test_preparata.py`

 * *Files identical despite different names*

### Comparing `PyCompGeomAlgorithms-1.0.7/tests/algorithms/test_quickhull.py` & `PyCompGeomAlgorithms-1.0.8/tests/algorithms/test_quickhull.py`

 * *Files identical despite different names*

### Comparing `PyCompGeomAlgorithms-1.0.7/tests/entities/test_entities.py` & `PyCompGeomAlgorithms-1.0.8/tests/entities/test_entities.py`

 * *Files identical despite different names*

