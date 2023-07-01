# Comparing `tmp/sax-0.8.7.tar.gz` & `tmp/sax-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sax-0.8.7.tar", last modified: Thu Jun  1 21:42:36 2023, max compression
+gzip compressed data, was "sax-0.8.8.tar", last modified: Sat Jul  1 03:26:02 2023, max compression
```

## Comparing `sax-0.8.7.tar` & `sax-0.8.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 21:42:36.600096 sax-0.8.7/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-01 21:41:56.000000 sax-0.8.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      838 2023-06-01 21:42:36.600096 sax-0.8.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4864 2023-06-01 21:41:56.000000 sax-0.8.7/README.md
--rw-r--r--   0 root         (0) root         (0)     2010 2023-06-01 21:41:56.000000 sax-0.8.7/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 21:42:36.596096 sax-0.8.7/sax/
--rw-r--r--   0 root         (0) root         (0)     2699 2023-06-01 21:41:56.000000 sax-0.8.7/sax/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6517 2023-06-01 21:41:56.000000 sax-0.8.7/sax/_nbdev.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 21:42:36.600096 sax-0.8.7/sax/backends/
--rw-r--r--   0 root         (0) root         (0)      774 2023-06-01 21:41:56.000000 sax-0.8.7/sax/backends/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3871 2023-06-01 21:41:56.000000 sax-0.8.7/sax/backends/additive.py
--rw-r--r--   0 root         (0) root         (0)     4333 2023-06-01 21:41:56.000000 sax-0.8.7/sax/backends/default.py
--rw-r--r--   0 root         (0) root         (0)     3945 2023-06-01 21:41:56.000000 sax-0.8.7/sax/backends/klu.py
--rw-r--r--   0 root         (0) root         (0)    10676 2023-06-01 21:41:56.000000 sax-0.8.7/sax/circuit.py
--rw-r--r--   0 root         (0) root         (0)     8000 2023-06-01 21:41:56.000000 sax-0.8.7/sax/make_docs.py
--rw-r--r--   0 root         (0) root         (0)     8813 2023-06-01 21:41:56.000000 sax-0.8.7/sax/models.py
--rw-r--r--   0 root         (0) root         (0)     5770 2023-06-01 21:41:56.000000 sax-0.8.7/sax/multimode.py
--rw-r--r--   0 root         (0) root         (0)     6964 2023-06-01 21:41:56.000000 sax-0.8.7/sax/netlist.py
--rw-r--r--   0 root         (0) root         (0)     2751 2023-06-01 21:41:56.000000 sax-0.8.7/sax/netlist_cleaning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 21:42:36.600096 sax-0.8.7/sax/nn/
--rw-r--r--   0 root         (0) root         (0)      971 2023-06-01 21:41:56.000000 sax-0.8.7/sax/nn/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2749 2023-06-01 21:41:56.000000 sax-0.8.7/sax/nn/core.py
--rw-r--r--   0 root         (0) root         (0)     6965 2023-06-01 21:41:56.000000 sax-0.8.7/sax/nn/io.py
--rw-r--r--   0 root         (0) root         (0)      925 2023-06-01 21:41:56.000000 sax-0.8.7/sax/nn/loss.py
--rw-r--r--   0 root         (0) root         (0)     2000 2023-06-01 21:41:56.000000 sax-0.8.7/sax/nn/utils.py
--rw-r--r--   0 root         (0) root         (0)     1775 2023-06-01 21:41:56.000000 sax-0.8.7/sax/patched.py
--rw-r--r--   0 root         (0) root         (0)    10223 2023-06-01 21:41:56.000000 sax-0.8.7/sax/typing_.py
--rw-r--r--   0 root         (0) root         (0)    18468 2023-06-01 21:41:56.000000 sax-0.8.7/sax/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 21:42:36.600096 sax-0.8.7/sax.egg-info/
--rw-r--r--   0 root         (0) root         (0)      838 2023-06-01 21:42:36.000000 sax-0.8.7/sax.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      513 2023-06-01 21:42:36.000000 sax-0.8.7/sax.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 21:42:36.000000 sax-0.8.7/sax.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      519 2023-06-01 21:42:36.000000 sax-0.8.7/sax.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-01 21:42:36.000000 sax-0.8.7/sax.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 21:42:36.600096 sax-0.8.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 03:26:02.363851 sax-0.8.8/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-01 03:25:20.000000 sax-0.8.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      838 2023-07-01 03:26:02.363851 sax-0.8.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4864 2023-07-01 03:25:20.000000 sax-0.8.8/README.md
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-07-01 03:25:20.000000 sax-0.8.8/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 03:26:02.359851 sax-0.8.8/sax/
+-rw-r--r--   0 root         (0) root         (0)     2779 2023-07-01 03:25:20.000000 sax-0.8.8/sax/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6577 2023-07-01 03:25:20.000000 sax-0.8.8/sax/_nbdev.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 03:26:02.363851 sax-0.8.8/sax/backends/
+-rw-r--r--   0 root         (0) root         (0)      774 2023-07-01 03:25:20.000000 sax-0.8.8/sax/backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3871 2023-07-01 03:25:20.000000 sax-0.8.8/sax/backends/additive.py
+-rw-r--r--   0 root         (0) root         (0)     4333 2023-07-01 03:25:20.000000 sax-0.8.8/sax/backends/default.py
+-rw-r--r--   0 root         (0) root         (0)     3945 2023-07-01 03:25:20.000000 sax-0.8.8/sax/backends/klu.py
+-rw-r--r--   0 root         (0) root         (0)    12018 2023-07-01 03:25:20.000000 sax-0.8.8/sax/circuit.py
+-rw-r--r--   0 root         (0) root         (0)     8000 2023-07-01 03:25:20.000000 sax-0.8.8/sax/make_docs.py
+-rw-r--r--   0 root         (0) root         (0)     8813 2023-07-01 03:25:20.000000 sax-0.8.8/sax/models.py
+-rw-r--r--   0 root         (0) root         (0)     5770 2023-07-01 03:25:20.000000 sax-0.8.8/sax/multimode.py
+-rw-r--r--   0 root         (0) root         (0)     6964 2023-07-01 03:25:20.000000 sax-0.8.8/sax/netlist.py
+-rw-r--r--   0 root         (0) root         (0)     2751 2023-07-01 03:25:20.000000 sax-0.8.8/sax/netlist_cleaning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 03:26:02.363851 sax-0.8.8/sax/nn/
+-rw-r--r--   0 root         (0) root         (0)      971 2023-07-01 03:25:20.000000 sax-0.8.8/sax/nn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2749 2023-07-01 03:25:20.000000 sax-0.8.8/sax/nn/core.py
+-rw-r--r--   0 root         (0) root         (0)     6965 2023-07-01 03:25:20.000000 sax-0.8.8/sax/nn/io.py
+-rw-r--r--   0 root         (0) root         (0)      925 2023-07-01 03:25:20.000000 sax-0.8.8/sax/nn/loss.py
+-rw-r--r--   0 root         (0) root         (0)     2000 2023-07-01 03:25:20.000000 sax-0.8.8/sax/nn/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1775 2023-07-01 03:25:20.000000 sax-0.8.8/sax/patched.py
+-rw-r--r--   0 root         (0) root         (0)    10223 2023-07-01 03:25:20.000000 sax-0.8.8/sax/typing_.py
+-rw-r--r--   0 root         (0) root         (0)    18468 2023-07-01 03:25:20.000000 sax-0.8.8/sax/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 03:26:02.359851 sax-0.8.8/sax.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      838 2023-07-01 03:26:02.000000 sax-0.8.8/sax.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      513 2023-07-01 03:26:02.000000 sax-0.8.8/sax.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-01 03:26:02.000000 sax-0.8.8/sax.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      519 2023-07-01 03:26:02.000000 sax-0.8.8/sax.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-01 03:26:02.000000 sax-0.8.8/sax.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-01 03:26:02.363851 sax-0.8.8/setup.cfg
```

### Comparing `sax-0.8.7/LICENSE` & `sax-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sax-0.8.7/PKG-INFO` & `sax-0.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sax
-Version: 0.8.7
+Version: 0.8.8
 Summary: Autograd and XLA for S-parameters
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `sax-0.8.7/README.md` & `sax-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `sax-0.8.7/pyproject.toml` & `sax-0.8.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "pip", "build", "wheel", "pybind11"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sax"
-version = "0.8.7"
+version = "0.8.8"
 authors = [
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Autograd and XLA for S-parameters"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Science/Research",
```

### Comparing `sax-0.8.7/sax/__init__.py` & `sax-0.8.8/sax/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 __all__ = []
 
 # Internal Cell
 #nbdev_comment from __future__ import annotations
 
 __author__ = "Floris Laporte"
-__version__ = "0.8.7"
+__version__ = "0.8.8"
 
 # Cell
 from functools import partial as partial
 from math import pi as pi
 
 from scipy.constants import c as c
 
@@ -101,14 +101,15 @@
 from .netlist import netlist as netlist
 from .netlist import load_netlist as load_netlist
 from .netlist import load_recursive_netlist as load_recursive_netlist
 
 # Cell
 
 from .circuit import circuit as circuit
+from .circuit import get_required_circuit_models as get_required_circuit_models
 
 # Cell
 
 from sax import backends as backends
 
 # Cell
```

### Comparing `sax-0.8.7/sax/_nbdev.py` & `sax-0.8.8/sax/_nbdev.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,14 +77,15 @@
          "draw_dag": "07_circuit.ipynb",
          "find_root": "07_circuit.ipynb",
          "find_leaves": "07_circuit.ipynb",
          "circuit": "07_circuit.ipynb",
          "NetlistDict": "07_circuit.ipynb",
          "CircuitInfo": "07_circuit.ipynb",
          "RecursiveNetlistDict": "07_circuit.ipynb",
+         "get_required_circuit_models": "07_circuit.ipynb",
          "circuit_backends": "08_backends.ipynb",
          "evaluate_circuit": "08a_backends_default.ipynb",
          "solve_klu": "08b_backends_klu.ipynb",
          "mul_coo": "08b_backends_klu.ipynb",
          "evaluate_circuit_klu": "08b_backends_klu.ipynb",
          "split_port": "08c_backends_additive.ipynb",
          "graph_edges": "08c_backends_additive.ipynb",
```

### Comparing `sax-0.8.7/sax/backends/__init__.py` & `sax-0.8.8/sax/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.7/sax/backends/additive.py` & `sax-0.8.8/sax/backends/additive.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.7/sax/backends/default.py` & `sax-0.8.8/sax/backends/default.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.7/sax/backends/klu.py` & `sax-0.8.8/sax/backends/klu.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.7/sax/circuit.py` & `sax-0.8.8/sax/circuit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: nbs/07_circuit.ipynb (unless otherwise specified).
 
 
 from __future__ import annotations
 
 
 __all__ = ['create_dag', 'draw_dag', 'find_root', 'find_leaves', 'circuit', 'NetlistDict', 'CircuitInfo',
-           'RecursiveNetlistDict']
+           'RecursiveNetlistDict', 'get_required_circuit_models']
 
 # Cell
 #nbdev_comment from __future__ import annotations
 
 import os
 import shutil
 import sys
@@ -335,8 +335,42 @@
         for mode in modes
     }
     ports = {
         f"{p1}@{mode}": f"{p2}@{mode}"
         for p1, p2 in netlist.ports.items()
         for mode in modes
     }
-    return connections, ports, models
+    return connections, ports, models
+
+# Cell
+
+def get_required_circuit_models(
+        netlist: Union[Netlist, NetlistDict, RecursiveNetlist, RecursiveNetlistDict],
+        models: Optional[Dict[str, Model]] = None,
+) -> List:
+    if models is None:
+        models = {}
+    assert isinstance(models, dict)
+    netlist = _ensure_recursive_netlist_dict(netlist)
+    # TODO: do the following two steps *after* recursive netlist parsing.
+    netlist = remove_unused_instances(netlist)
+    netlist, instance_models = _extract_instance_models(netlist)
+    recnet: RecursiveNetlist = _validate_net(netlist)
+
+    missing_models = {}
+    missing_model_names = []
+    g = nx.DiGraph()
+
+    for model_name, subnetlist in recnet.dict()["__root__"].items():
+        if not model_name in missing_models:
+            missing_models[model_name] = models.get(model_name, subnetlist)
+            g.add_node(model_name)
+        if model_name in models:
+            continue
+        for instance in subnetlist["instances"].values():
+            component = instance["component"]
+            if not component in missing_models:
+                missing_models[component] = models.get(component, None)
+                missing_model_names.append(component)
+                g.add_node(component)
+            g.add_edge(model_name, component)
+    return missing_model_names
```

### Comparing `sax-0.8.7/sax/make_docs.py` & `sax-0.8.8/sax/make_docs.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.7/sax/models.py` & `sax-0.8.8/sax/models.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.7/sax/multimode.py` & `sax-0.8.8/sax/multimode.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.7/sax/netlist.py` & `sax-0.8.8/sax/netlist.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.7/sax/netlist_cleaning.py` & `sax-0.8.8/sax/netlist_cleaning.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.7/sax/nn/__init__.py` & `sax-0.8.8/sax/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.7/sax/nn/core.py` & `sax-0.8.8/sax/nn/core.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.7/sax/nn/io.py` & `sax-0.8.8/sax/nn/io.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.7/sax/nn/loss.py` & `sax-0.8.8/sax/nn/loss.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.7/sax/nn/utils.py` & `sax-0.8.8/sax/nn/utils.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.7/sax/patched.py` & `sax-0.8.8/sax/patched.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.7/sax/typing_.py` & `sax-0.8.8/sax/typing_.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.7/sax/utils.py` & `sax-0.8.8/sax/utils.py`

 * *Files identical despite different names*

### Comparing `sax-0.8.7/sax.egg-info/PKG-INFO` & `sax-0.8.8/sax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sax
-Version: 0.8.7
+Version: 0.8.8
 Summary: Autograd and XLA for S-parameters
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `sax-0.8.7/sax.egg-info/SOURCES.txt` & `sax-0.8.8/sax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sax-0.8.7/sax.egg-info/requires.txt` & `sax-0.8.8/sax.egg-info/requires.txt`

 * *Files identical despite different names*

