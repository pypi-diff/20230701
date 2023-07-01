# Comparing `tmp/lingam-1.7.1.tar.gz` & `tmp/lingam-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lingam-1.7.1.tar", last modified: Fri Feb 17 02:21:01 2023, max compression
+gzip compressed data, was "lingam-1.8.0.tar", last modified: Sat Jul  1 08:37:54 2023, max compression
```

## Comparing `lingam-1.7.1.tar` & `lingam-1.8.0.tar`

### file list

```diff
@@ -1,50 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 02:21:01.040711 lingam-1.7.1/
--rw-r--r--   0 root         (0) root         (0)     1110 2023-02-17 00:51:39.000000 lingam-1.7.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8876 2023-02-17 02:21:01.040711 lingam-1.7.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8631 2023-02-17 00:51:39.000000 lingam-1.7.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 02:21:01.030711 lingam-1.7.1/lingam/
--rw-r--r--   0 root         (0) root         (0)     1279 2023-02-17 00:51:39.000000 lingam-1.7.1/lingam/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5843 2023-02-17 00:51:39.000000 lingam-1.7.1/lingam/base.py
--rw-r--r--   0 root         (0) root         (0)    14836 2023-02-17 00:51:39.000000 lingam-1.7.1/lingam/bootstrap.py
--rw-r--r--   0 root         (0) root         (0)    18716 2023-02-17 00:51:39.000000 lingam-1.7.1/lingam/bottom_up_parce_lingam.py
--rw-r--r--   0 root         (0) root         (0)     7460 2023-02-17 00:51:39.000000 lingam-1.7.1/lingam/camuv.py
--rw-r--r--   0 root         (0) root         (0)    24236 2023-02-17 00:51:39.000000 lingam-1.7.1/lingam/causal_based_simulator.py
--rw-r--r--   0 root         (0) root         (0)     9697 2023-02-17 00:51:39.000000 lingam-1.7.1/lingam/causal_effect.py
--rw-r--r--   0 root         (0) root         (0)    10632 2023-02-17 00:51:39.000000 lingam-1.7.1/lingam/direct_lingam.py
--rw-r--r--   0 root         (0) root         (0)     4660 2023-02-17 00:51:39.000000 lingam-1.7.1/lingam/hsic.py
--rw-r--r--   0 root         (0) root         (0)     4632 2023-02-17 00:51:39.000000 lingam-1.7.1/lingam/ica_lingam.py
--rw-r--r--   0 root         (0) root         (0)    13361 2023-02-17 00:51:39.000000 lingam-1.7.1/lingam/lim.py
--rw-r--r--   0 root         (0) root         (0)    24644 2023-02-17 00:51:39.000000 lingam-1.7.1/lingam/lina.py
--rw-r--r--   0 root         (0) root         (0)    27629 2023-02-17 00:51:39.000000 lingam-1.7.1/lingam/longitudinal_lingam.py
--rw-r--r--   0 root         (0) root         (0)    11025 2023-02-17 00:51:39.000000 lingam-1.7.1/lingam/multi_group_direct_lingam.py
--rw-r--r--   0 root         (0) root         (0)    17954 2023-02-17 00:51:39.000000 lingam-1.7.1/lingam/rcd.py
--rw-r--r--   0 root         (0) root         (0)     6028 2023-02-17 00:51:39.000000 lingam-1.7.1/lingam/resit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 02:21:01.030711 lingam-1.7.1/lingam/utils/
--rw-r--r--   0 root         (0) root         (0)    29526 2023-02-17 00:51:39.000000 lingam-1.7.1/lingam/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17324 2023-02-17 00:51:39.000000 lingam-1.7.1/lingam/var_lingam.py
--rw-r--r--   0 root         (0) root         (0)    20353 2023-02-17 00:51:39.000000 lingam-1.7.1/lingam/varma_lingam.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 02:21:01.030711 lingam-1.7.1/lingam.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8876 2023-02-17 02:21:00.000000 lingam-1.7.1/lingam.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1009 2023-02-17 02:21:00.000000 lingam-1.7.1/lingam.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-17 02:21:00.000000 lingam-1.7.1/lingam.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       98 2023-02-17 02:21:00.000000 lingam-1.7.1/lingam.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-02-17 02:21:00.000000 lingam-1.7.1/lingam.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-17 02:21:01.040711 lingam-1.7.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      926 2023-02-17 00:51:39.000000 lingam-1.7.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 02:21:01.030711 lingam-1.7.1/tests/
--rw-r--r--   0 root         (0) root         (0)    14293 2023-02-17 00:51:39.000000 lingam-1.7.1/tests/test_bootstrap.py
--rw-r--r--   0 root         (0) root         (0)    10832 2023-02-17 00:51:39.000000 lingam-1.7.1/tests/test_bottom_up_parce_lingam.py
--rw-r--r--   0 root         (0) root         (0)     2615 2023-02-17 00:51:39.000000 lingam-1.7.1/tests/test_camuv.py
--rw-r--r--   0 root         (0) root         (0)    27130 2023-02-17 00:51:39.000000 lingam-1.7.1/tests/test_causal_based_simulator.py
--rw-r--r--   0 root         (0) root         (0)    10044 2023-02-17 00:51:39.000000 lingam-1.7.1/tests/test_causal_effect.py
--rw-r--r--   0 root         (0) root         (0)     8599 2023-02-17 00:51:39.000000 lingam-1.7.1/tests/test_direct_lingam.py
--rw-r--r--   0 root         (0) root         (0)     2304 2023-02-17 00:51:39.000000 lingam-1.7.1/tests/test_ica_lingam.py
--rw-r--r--   0 root         (0) root         (0)     1792 2023-02-17 00:51:39.000000 lingam-1.7.1/tests/test_lim.py
--rw-r--r--   0 root         (0) root         (0)     6637 2023-02-17 00:51:39.000000 lingam-1.7.1/tests/test_lina.py
--rw-r--r--   0 root         (0) root         (0)    19896 2023-02-17 00:51:39.000000 lingam-1.7.1/tests/test_longitudinal_lingam.py
--rw-r--r--   0 root         (0) root         (0)    12304 2023-02-17 00:51:39.000000 lingam-1.7.1/tests/test_multi_group_direct_lingam.py
--rw-r--r--   0 root         (0) root         (0)     9689 2023-02-17 00:51:39.000000 lingam-1.7.1/tests/test_rcd.py
--rw-r--r--   0 root         (0) root         (0)     2017 2023-02-17 00:51:39.000000 lingam-1.7.1/tests/test_resit.py
--rw-r--r--   0 root         (0) root         (0)     4626 2023-02-17 00:51:39.000000 lingam-1.7.1/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     5375 2023-02-17 00:51:39.000000 lingam-1.7.1/tests/test_var_lingam.py
--rw-r--r--   0 root         (0) root         (0)     8381 2023-02-17 00:51:39.000000 lingam-1.7.1/tests/test_varma_lingam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 08:37:54.449583 lingam-1.8.0/
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-07-01 08:11:10.000000 lingam-1.8.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8876 2023-07-01 08:37:54.449583 lingam-1.8.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8631 2023-07-01 08:11:10.000000 lingam-1.8.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 08:37:54.449583 lingam-1.8.0/lingam/
+-rw-r--r--   0 root         (0) root         (0)     1329 2023-07-01 08:11:10.000000 lingam-1.8.0/lingam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5843 2023-07-01 08:11:10.000000 lingam-1.8.0/lingam/base.py
+-rw-r--r--   0 root         (0) root         (0)    14836 2023-07-01 08:11:10.000000 lingam-1.8.0/lingam/bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)    18716 2023-07-01 08:11:10.000000 lingam-1.8.0/lingam/bottom_up_parce_lingam.py
+-rw-r--r--   0 root         (0) root         (0)     7504 2023-07-01 08:11:10.000000 lingam-1.8.0/lingam/camuv.py
+-rw-r--r--   0 root         (0) root         (0)    25558 2023-07-01 08:11:10.000000 lingam-1.8.0/lingam/causal_based_simulator.py
+-rw-r--r--   0 root         (0) root         (0)     9697 2023-07-01 08:11:10.000000 lingam-1.8.0/lingam/causal_effect.py
+-rw-r--r--   0 root         (0) root         (0)    10632 2023-07-01 08:11:10.000000 lingam-1.8.0/lingam/direct_lingam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 08:37:54.449583 lingam-1.8.0/lingam/experimental/
+-rw-r--r--   0 root         (0) root         (0)      276 2023-07-01 08:11:10.000000 lingam-1.8.0/lingam/experimental/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13123 2023-07-01 08:22:05.000000 lingam-1.8.0/lingam/experimental/cdg.py
+-rw-r--r--   0 root         (0) root         (0)    11932 2023-07-01 08:11:10.000000 lingam-1.8.0/lingam/experimental/oct.py
+-rw-r--r--   0 root         (0) root         (0)     4440 2023-07-01 08:24:13.000000 lingam-1.8.0/lingam/hsic.py
+-rw-r--r--   0 root         (0) root         (0)     4632 2023-07-01 08:11:10.000000 lingam-1.8.0/lingam/ica_lingam.py
+-rw-r--r--   0 root         (0) root         (0)    13735 2023-07-01 08:11:10.000000 lingam-1.8.0/lingam/lim.py
+-rw-r--r--   0 root         (0) root         (0)    24644 2023-07-01 08:11:10.000000 lingam-1.8.0/lingam/lina.py
+-rw-r--r--   0 root         (0) root         (0)    27629 2023-07-01 08:11:10.000000 lingam-1.8.0/lingam/longitudinal_lingam.py
+-rw-r--r--   0 root         (0) root         (0)    11025 2023-07-01 08:11:10.000000 lingam-1.8.0/lingam/multi_group_direct_lingam.py
+-rw-r--r--   0 root         (0) root         (0)    21277 2023-07-01 08:11:10.000000 lingam-1.8.0/lingam/multi_group_rcd.py
+-rw-r--r--   0 root         (0) root         (0)    17954 2023-07-01 08:11:10.000000 lingam-1.8.0/lingam/rcd.py
+-rw-r--r--   0 root         (0) root         (0)     6028 2023-07-01 08:11:10.000000 lingam-1.8.0/lingam/resit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 08:37:54.449583 lingam-1.8.0/lingam/utils/
+-rw-r--r--   0 root         (0) root         (0)    43275 2023-07-01 08:25:11.000000 lingam-1.8.0/lingam/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7670 2023-07-01 08:11:10.000000 lingam-1.8.0/lingam/utils/_rcd.py
+-rw-r--r--   0 root         (0) root         (0)    17322 2023-07-01 08:11:10.000000 lingam-1.8.0/lingam/var_lingam.py
+-rw-r--r--   0 root         (0) root         (0)    20353 2023-07-01 08:11:10.000000 lingam-1.8.0/lingam/varma_lingam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 08:37:54.449583 lingam-1.8.0/lingam.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8876 2023-07-01 08:37:54.000000 lingam-1.8.0/lingam.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      722 2023-07-01 08:37:54.000000 lingam-1.8.0/lingam.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-01 08:37:54.000000 lingam-1.8.0/lingam.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-01 08:37:54.000000 lingam-1.8.0/lingam.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-01 08:37:54.000000 lingam-1.8.0/lingam.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-01 08:37:54.449583 lingam-1.8.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      948 2023-07-01 08:11:10.000000 lingam-1.8.0/setup.py
```

### Comparing `lingam-1.7.1/LICENSE` & `lingam-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lingam-1.7.1/PKG-INFO` & `lingam-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lingam
-Version: 1.7.1
+Version: 1.8.0
 Summary: LiNGAM Python Package
 Home-page: https://github.com/cdt15/lingam
 Author: T.Ikeuchi, G.Haraoka, M.Ide, W.Kurebayashi, S.Shimizu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `lingam-1.7.1/README.md` & `lingam-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `lingam-1.7.1/lingam/__init__.py` & `lingam-1.8.0/lingam/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """
 The lingam module includes implementation of the LiNGAM algorithms.
 The LiNGAM Project: https://sites.google.com/view/sshimizu06/lingam
 """
 
 from .bootstrap import BootstrapResult
 from .bottom_up_parce_lingam import BottomUpParceLiNGAM
+from .camuv import CAMUV
+from .causal_based_simulator import CausalBasedSimulator
 from .causal_effect import CausalEffect
 from .direct_lingam import DirectLiNGAM
 from .ica_lingam import ICALiNGAM
-from .longitudinal_lingam import LongitudinalLiNGAM, LongitudinalBootstrapResult
+from .lim import LiM
+from .lina import LiNA, MDLiNA
+from .longitudinal_lingam import LongitudinalBootstrapResult, LongitudinalLiNGAM
 from .multi_group_direct_lingam import MultiGroupDirectLiNGAM
+from .multi_group_rcd import MultiGroupRCD
 from .rcd import RCD
-from .camuv import CAMUV
-from .var_lingam import VARLiNGAM, VARBootstrapResult
-from .varma_lingam import VARMALiNGAM, VARMABootstrapResult
-from .lina import LiNA
-from .lina import MDLiNA
 from .resit import RESIT
-from .lim import LiM
-from .causal_based_simulator import CausalBasedSimulator
+from .var_lingam import VARBootstrapResult, VARLiNGAM
+from .varma_lingam import VARMABootstrapResult, VARMALiNGAM
+
 __all__ = [
     "ICALiNGAM",
     "DirectLiNGAM",
     "BootstrapResult",
     "MultiGroupDirectLiNGAM",
     "CausalEffect",
     "VARLiNGAM",
@@ -35,10 +36,11 @@
     "RCD",
     "CAMUV",
     "LiNA",
     "MDLiNA",
     "RESIT",
     "LiM",
     "CausalBasedSimulator",
+    "MultiGroupRCD",
 ]
 
-__version__ = "1.7.1"
+__version__ = "1.8.0"
```

### Comparing `lingam-1.7.1/lingam/base.py` & `lingam-1.8.0/lingam/base.py`

 * *Files identical despite different names*

### Comparing `lingam-1.7.1/lingam/bootstrap.py` & `lingam-1.8.0/lingam/bootstrap.py`

 * *Files identical despite different names*

### Comparing `lingam-1.7.1/lingam/bottom_up_parce_lingam.py` & `lingam-1.8.0/lingam/bottom_up_parce_lingam.py`

 * *Files identical despite different names*

### Comparing `lingam-1.7.1/lingam/camuv.py` & `lingam-1.8.0/lingam/camuv.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 """
 Python implementation of the LiNGAM algorithms.
 The LiNGAM Project: https://sites.google.com/view/sshimizu06/lingam
 """
 
 
-from .hsic import hsic_test_gamma
-import numpy as np
+import copy
 import itertools
+
+import numpy as np
 from pygam import LinearGAM
-import copy
 from sklearn.utils import check_array
 
+from .hsic import hsic_test_gamma
+
 
 class CAMUV:
     """Implementation of CAM-UV Algorithm [1]_
 
     References
     ----------
     .. [1] T.N.Maeda and S.Shimizu. Causal additive models with unobserved variables.
        In Proc. Thirty-Seventh Conference on Uncertainty in Artificial Intelligence (UAI). PMLR  161:97-106, 2021.
     """
 
-    def __init__(
-            self,
-            alpha=0.01,
-            num_explanatory_vals=2
-    ):
-
+    def __init__(self, alpha=0.01, num_explanatory_vals=2):
         """Construct a CAM-UV model.
 
         Parameters
         ----------
          alpha : float, optional (default=0.01)
              Alpha level.
          num_explanatory_vals : int, optional (default=2)
@@ -54,15 +51,15 @@
         d = X.shape[1]
         N = self._get_neighborhoods(X, self._alpha)
         P = self._find_parents(X, self._alpha, self._num_explanatory_vals, N)
 
         U = []
 
         for i in range(d):
-            for j in range(d)[i+1:]:
+            for j in range(d)[i + 1 :]:
                 if (i in P[j]) or (j in P[i]):
                     continue
                 if (i not in N[j]) or (j not in N[i]):
                     continue
                 i_residual = self._get_residual(X, i, P[i])
                 j_residual = self._get_residual(X, j, P[j])
                 in_X = np.reshape(i_residual, [n, 1])
@@ -71,30 +68,29 @@
                 if independence < self._alpha:
                     if not set([i, j]) in U:
                         U.append(set([i, j]))
 
         return self._estimate_adjacency_matrix(X, P, U)
 
     def _get_residual(self, X, explained_i, explanatory_ids):
-
         explanatory_ids = list(explanatory_ids)
 
         if len(explanatory_ids) == 0:
             residual = X[:, explained_i]
         else:
             gam = LinearGAM().fit(X[:, explanatory_ids], X[:, explained_i])
             residual = X[:, explained_i] - gam.predict(X[:, explanatory_ids])
         return residual
 
     def _get_neighborhoods(self, X, alpha):
         n = X.shape[0]
         d = X.shape[1]
         N = [set() for i in range(d)]
         for i in range(d):
-            for j in range(d)[i+1:]:
+            for j in range(d)[i + 1 :]:
                 in_X = np.reshape(X[:, i], [n, 1])
                 in_Y = np.reshape(X[:, j], [n, 1])
                 independence = hsic_test_gamma(X=in_X, Y=in_Y)[1]
                 if independence < self._alpha:
                     N[i].add(j)
                     N[j].add(i)
         return N
@@ -102,29 +98,33 @@
     def _find_parents(self, X, alpha, maxnum_vals, N):
         n = X.shape[0]
         d = X.shape[1]
         P = [set() for i in range(d)]  # Parents
         t = 2
         Y = copy.deepcopy(X)
 
-        while (True):
+        while True:
             changed = False
             variables_set_list = list(itertools.combinations(set(range(d)), t))
             for variables_set in variables_set_list:
                 variables_set = set(variables_set)
 
                 if not self._check_identified_causality(variables_set, P):
                     continue
 
-                child, independence_with_K = self._get_child(X, variables_set, P, N, Y, alpha)
+                child, independence_with_K = self._get_child(
+                    X, variables_set, P, N, Y, alpha
+                )
                 if not independence_with_K > alpha:
                     continue
 
-                parents = variables_set-{child}
-                if not self._check_independence_withou_K(parents, child, P, N, Y, alpha):
+                parents = variables_set - {child}
+                if not self._check_independence_withou_K(
+                    parents, child, P, N, Y, alpha
+                ):
                     continue
 
                 for parent in parents:
                     P[child].add(parent)
                     changed = True
                     Y = self._get_residuals_matrix(X, Y, P, child)
 
@@ -134,27 +134,26 @@
                 t += 1
                 if t > maxnum_vals:
                     break
 
         for i in range(d):
             non_parents = set()
             for j in P[i]:
-                residual_i = self._get_residual(X, i, P[i]-{j})
+                residual_i = self._get_residual(X, i, P[i] - {j})
                 residual_j = self._get_residual(X, j, P[j])
                 in_X = np.reshape(residual_i, [n, 1])
                 in_Y = np.reshape(residual_j, [n, 1])
                 independence = hsic_test_gamma(X=in_X, Y=in_Y)[1]
                 if independence > alpha:
                     non_parents.add(j)
             P[i] = P[i] - non_parents
 
         return P
 
     def _get_residuals_matrix(self, X, Y_old, P, child):
-
         Y = copy.deepcopy(Y_old)
         Y[:, child] = self._get_residual(X, child, P[child])
         return Y
 
     def _get_child(self, X, variables_set, P, N, Y, alpha):
         n = X.shape[0]
 
@@ -186,15 +185,15 @@
             if alpha < independence:
                 return False
         return True
 
     def _check_identified_causality(self, variables_set, P):
         variables_list = list(variables_set)
         for i in variables_list:
-            for j in variables_list[variables_list.index(i)+1:]:
+            for j in variables_list[variables_list.index(i) + 1 :]:
                 if (j in P[i]) or (i in P[j]):
                     return False
         return True
 
     def _check_correlation(self, child, parents, N):
         for parent in parents:
             if parent not in N[child]:
```

### Comparing `lingam-1.7.1/lingam/causal_based_simulator.py` & `lingam-1.8.0/lingam/causal_based_simulator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,407 +1,540 @@
 from collections import namedtuple
 
 import numpy as np
 import pandas as pd
 
-from sklearn.base import BaseEstimator, RegressorMixin, ClassifierMixin, clone
+from sklearn.base import RegressorMixin, ClassifierMixin, clone
+from sklearn.dummy import DummyClassifier, DummyRegressor
 from sklearn.model_selection._search import BaseSearchCV
 from sklearn.utils import check_array
 from sklearn.linear_model import LinearRegression, LogisticRegression
 from sklearn.pipeline import Pipeline
 
-TrainData = namedtuple("TrainData", ("condition", "X", "y"))
-TrainResult = namedtuple("TrainResult", ("condition", "model", "exp_columns", "predicted", "residual"))
-ChangingModels = namedtuple("ChangingModels", ("name", "condition", "model"))
+TrainData = namedtuple(
+    "TrainData",
+    ("condition", "X", "y")
+)
+TrainResult = namedtuple(
+    "TrainResult",
+    ("condition", "model", "exp_columns", "predicted", "residual")
+)
+ChangingModels = namedtuple(
+    "ChangingModels",
+    ("name", "condition", "model")
+)
 
 
 class CausalBasedSimulator:
     """
     Causal based simulator.
 
     Attributes
     ----------
     train_result_ : dict of string -> list of dict
         information about trained models.
+
     residual_ : pandas.DataFrame
         residuals of trained models.
-    categorical_info_ : dict of strig -> list of str
-        information about categorical variables.
-        the key of its dictioary is variable name, the value is the list of classes.
+
+    cat_map_ : dict of strig -> list of str
+        information about categorical variables. the key of its dictioary is
+        variable name, the value is the list of classes.
+
     simulated_data_ : pandas.DataFrame
         result of simulation.
     """
 
-    def __init__(self):
-        # input of train()
-        self._data = None
-        self._causal_graph = None
-
-        # result of train()
-        self._train_results = None
-
-        # input of run()
-        self._changing_exog = None
-        self._changing_models = None
-
-        # result of run()
-        self._causal_order = None
-        self._simulated_result = None
-
     def train(self, X, causal_graph, models=None):
         """
-        Estimate functional relations between variables and variable distributions based on
-        the training data ``X`` and the causal graph ``G``. The functional relations represents
-        by sklearn.linear_model.LinearRegression if the object variable is numeric,
-        and represents by sklearn.linear_model.LogisticRegression if the object variable is categorical by default.
-        ``train_result_`` and ``residual_`` will be exposed after executing train().
+        Estimate functional relations between variables and variable
+        distributions based on the training data ``X`` and the causal graph
+        ``G``. The functional relations represents by
+        sklearn.linear_model.LinearRegression if the object variable is
+        numeric, and represents by sklearn.linear_model.LogisticRegression
+        if the object variable is categorical by default. ``train_result_``
+        and ``residual_`` will be exposed after executing train().
 
         Parameters
         ----------
         X : pandas.DataFrame
             Training data.
+
         causal_graph : array-like of shape (n_features, _features)
             Causal graph.
+
         models : dict of string -> object, default=None
-            Dictionary about models of variables.
-            Models are cloned internaly and are trained to infer functioal relations.
-            Given instances of the model are cloned to estimate the functional relation between variables.
+            Dictionary about models of variables. Models are cloned internaly
+            and are trained to infer functioal relations. Given instances of
+            the model are cloned to estimate the functional relation between
+            variables.
 
         Returns
         -------
         self : Object
         """
 
-        data, categorical_info = self._check_data(X)
+        # checking inputs
+        data, cat_map = self._check_data(X)
 
         causal_graph = self._check_causal_graph(causal_graph, data.shape[1])
-        train_models = self._check_models(models, data.index, data.columns, categorical_info)
 
-        train_results = self._train(data, categorical_info, causal_graph, train_models)
+        train_models = self._check_models(
+            models,
+            data.index,
+            data.columns,
+            cat_map
+        )
+
+        # training
+        train_results = self._train(
+            data,
+            cat_map,
+            causal_graph,
+            train_models
+        )
 
         residual_df = {}
-        for column in X.columns:
-            if len(train_results[column]) > 0:
-                series = self._concat_residuals(train_results, column, data.index)
+        for col_name in X.columns:
+            if len(train_results[col_name]) > 0:
+                series = self._concat_residuals(
+                    train_results,
+                    col_name,
+                    data.index
+                )
             else:
+                # node with no parent nodes
                 series = np.ones(data.shape[0]) * np.nan
-            residual_df[column] = series
-        residual_df = pd.DataFrame(residual_df)
 
-        train_result = self._prepare_to_expose_train(train_results, categorical_info)
+            residual_df[col_name] = series
+
+        residual_df = pd.DataFrame(residual_df)
 
-        self.train_result_ = train_result
+        # setting attributes
+        self.train_result_ = self._prep_to_expose_train(
+            train_results,
+            cat_map
+        )
         self.residual_ = residual_df
+        self.categorical_info_ = cat_map
 
+        # setting information
         self._data = data
-        self.categorical_info_ = categorical_info
         self._train_results = train_results
         self._causal_graph = causal_graph
+        self._causal_order = None
 
         return self
 
-    def run(self, changing_exog=None, changing_models=None, shuffle_residual=False, random_state=None):
+    def run(
+        self,
+        changing_exog=None,
+        changing_models=None,
+        shuffle_residual=False,
+        random_state=None
+    ):
         """
-        Generate simulated data using trained models and the given causal graph with given exogenous data and models.
-        Specifying environmental changes to ``changing_exog`` or specifiyig changes in fucitonal relation to ``change_models``
+        Generate simulated data using trained models and the given
+        causal graph with given exogenous data and models.
+        Specifying environmental changes to ``changing_exog`` or
+        specifiyig changes in fucitonal relation to ``change_models``
         effects simulated data.
-        Residuals to simulate variables are shuffled using radom_state if ``shuffle_residual`` is True.
-        ``simulated_data_`` will be expose after excuting train().
+        Residuals to simulate variables are shuffled using radom_state
+        if ``shuffle_residual`` is True. ``simulated_data_`` will be
+        expose after excuting train().
 
         Parameters
         ----------
         changing_exog : dict of string -> array-like, default=None
-            Dictioary about exogeous variables which keys are variable names and values are data of variables.
-            That variable name should be a one of column names of X and the length should be same as X.
+            Dictioary about exogeous variables which keys are variable
+            names and values are data of variables. That variable name
+            should be a one of column names of X and the length should
+            be same as X.
+
         changing_model : list of dict, default=None
-            List of the changing models which elements are dictionary. that keys should be name, condition, and model.
-            For name and condition, refer to ``train_result_`` and set the values corresponding to
-            the conditions you wish to change. For model, you must provide a trained machine learning instance.
+            List of the changing models which elements are dictionary. that
+            keys should be name, condition, and model. For name and
+            condition, refer to ``train_result_`` and set the values
+            corresponding to the conditions you wish to change. For model,
+            you must provide a trained machine learning instance.
+
         shuffle_residual : bool, default=True
             If True, residuals are shuffled.
+
         random_state : int, default=None
             If shuffle_residual is True, random_state is used as seed.
 
         Returns
         -------
         simulated_data : pandas.DataFrame
             simulated data.
         """
 
         if self._train_results is None:
-            raise RuntimeError("train() should be executed before run() is executed.")
+            raise RuntimeError(
+                "run() shall be executed after train() is executed"
+            )
 
+        # checking inputs
         changing_exog_df = self._check_changing_exog(
-            changing_exog, self._data.index, self._data.columns, self.categorical_info_)
-        changing_models2 = self._check_changing_models(changing_models, self.categorical_info_, self._train_results)
+            changing_exog,
+            self._data.index,
+            self._data.columns,
+            self.categorical_info_
+        )
+        changing_models2 = self._check_changing_models(
+            changing_models,
+            self.categorical_info_,
+            self._train_results
+        )
 
+        # calculating causal_order if it has not been calculated
         if self._causal_order is not None:
             causal_order = self._causal_order
         else:
             causal_order = self._get_causal_order(self._causal_graph)
 
-        simulated_df = self._simulate(self._data, self._causal_graph, causal_order, self.categorical_info_,
-                                      changing_exog_df, changing_models2, self._train_results, shuffle_residual, random_state)
+        simulated_df = self._simulate(
+            self._data,
+            self._causal_graph,
+            causal_order,
+            self.categorical_info_,
+            changing_exog_df,
+            changing_models2,
+            self._train_results,
+            shuffle_residual,
+            random_state
+        )
 
+        # set attributes
         self.simulated_data_ = simulated_df
 
+        # set information
         self._changing_exog = changing_exog_df
         self._changing_models = changing_models2
         if self._causal_order is None:
             self._causal_order = causal_order
 
         return self.simulated_data_
 
     def _check_data(self, X):
         if not isinstance(X, pd.DataFrame):
-            raise RuntimeError("X must be a pandas.DataFrame.")
+            raise RuntimeError("X shall be a pandas.DataFrame.")
 
-        # copy to replace values of categorical variables.
-        X = X.copy()
+        cat_map = {}
+        for c, is_cat in zip(X.columns, X.dtypes.values == "category"):
+            if not is_cat:
+                continue
 
-        is_categorical = {c: is_categorical for c, is_categorical in zip(X.columns, X.dtypes.values == "category")}
+            cat_map[c] = np.unique(X[c]).tolist()
+            X[c] = X[c].apply(lambda x: cat_map[c].index(x))
 
-        categorical_info = {}
-        for column, is_categorical_ in is_categorical.items():
-            if not is_categorical_:
-                continue
+        return X, cat_map
+
+    def _check_causal_graph(self, causal_graph, col_num):
+        graph = check_array(causal_graph)
+
+        if graph.shape[0] != col_num or graph.shape[1] != col_num:
+            raise RuntimeError("causal_graph.shape shall be square.")
 
-            # replace values of the categorical variable
-            categorical_info[column] = np.unique(X[column]).tolist()
-            X[column] = X[column].apply(lambda x: categorical_info[column].index(x))
-
-        return X, categorical_info
-
-    def _check_causal_graph(self, causal_graph, column_num):
-        causal_graph_ = check_array(causal_graph)
-        if causal_graph_.shape[0] != column_num or causal_graph_.shape[1] != column_num:
-            raise RuntimeError("The height and width of the causal_graph must be the same length.")
-        return causal_graph_
+        return graph
+
+    def _check_model_instance(self, model, col_name, cat_map):
+        if col_name not in cat_map.keys():
+            model_type = RegressorMixin
+        else:
+            model_type = ClassifierMixin
 
-    def _check_model_instance(self, model, column, categorical_info):
-        model_type = RegressorMixin if column not in categorical_info.keys() else ClassifierMixin
         if isinstance(model, Pipeline):
             if not isinstance(model.steps[-1][-1], model_type):
                 raise RuntimeError(
-                    "The final step in the Pipeline should be an instance of the regression/classification model.")
+                    "The last step in Pipeline should be an "
+                    + "instance of a regression/classification model."
+                )
         elif isinstance(model, BaseSearchCV):
             if not isinstance(model.get_params()["estimator"], model_type):
-                raise RuntimeError("Must be an instance of a regression/classification model.")
+                raise RuntimeError(
+                    "The type of the estimator shall be an "
+                    + "instance of a regression/classification model."
+                )
         else:
             if not isinstance(model, model_type):
-                raise RuntimeError("Must be an instance of a regression/classification model.")
+                raise RuntimeError(
+                    "The type of the estimator shall be an "
+                    + "instance of a regression/classification model."
+                )
 
         if model_type == ClassifierMixin:
             try:
                 func = getattr(model, "predict_proba")
                 if not callable(func):
                     raise Exception
             except Exception:
-                raise RuntimeError("Classification models without predict_proba() cannot be used.")
+                raise RuntimeError(
+                    "Classification models shall have "
+                    + "predict_proba()."
+                )
 
-    def _check_models(self, models, index, columns, categorical_info):
+    def _check_models(self, models, index, columns, cat_map):
         if models is None:
             return {}
 
         if not isinstance(models, dict):
-            raise RuntimeError("models must be a dictionary.")
+            raise RuntimeError("models shall be a dictionary.")
 
-        for column, model in models.items():
-            if column not in columns:
-                raise RuntimeError("The key of models must be a variable name that exists in X.")
+        for col_name, model in models.items():
+            if col_name not in columns:
+                raise RuntimeError(f"Unknown column name ({col_name})")
 
-            self._check_model_instance(model, column, categorical_info)
+            self._check_model_instance(model, col_name, cat_map)
 
         return models
 
-    def _check_changing_exog(self, changing_exog, index, columns, categorical_info):
+    def _check_changing_exog(self, changing_exog, index, columns, cat_map):
         if changing_exog is None:
             return pd.DataFrame()
 
         if not isinstance(changing_exog, dict):
-            raise RuntimeError("changing_exog must be a dictionary.")
+            raise RuntimeError("changing_exog shall be a dictionary.")
 
         changing_exog_df = {}
-        for column, values in changing_exog.items():
-            if column not in columns:
-                raise RuntimeError("The key of changing_exog must be a variable name that exists in X.")
+        for col_name, values in changing_exog.items():
+            if col_name not in columns:
+                raise RuntimeError(
+                    f"Unknown key in changing_exog. ({col_name})"
+                )
 
-            if column in categorical_info.keys():
-                raise RuntimeError("You cannot set changig_exog for a column of category variables.")
+            if col_name in cat_map.keys():
+                raise RuntimeError(
+                    f"Category variables shall not be specified. ({col_name})"
+                )
 
             s = check_array(values, ensure_2d=False, dtype=None).flatten()
             if s.shape[0] != len(index):
-                raise RuntimeError("The data sequence of changing_exog values must be the same length as X.")
+                raise RuntimeError(
+                    f"Wrong length. ({s.shape[0]} != {len(index)})"
+                )
 
-            changing_exog_df[column] = pd.Series(values, index=index)
+            changing_exog_df[col_name] = pd.Series(values, index=index)
         changing_exog_df = pd.DataFrame(changing_exog_df).loc[index, :]
 
         return changing_exog_df
 
-    def _check_changing_models(self, changing_models, categorical_info, train_results):
+    def _check_changing_models(self, changing_models, cat_map, train_results):
         if changing_models is None:
             return {}
 
         if not isinstance(changing_models, list):
-            raise RuntimeError("changing_models must be a list.")
+            raise RuntimeError("changing_models shall be a list.")
 
         changing_models_ = []
         for model_info in changing_models:
             if not isinstance(model_info, dict):
-                raise RuntimeError("The elements of changing_models must be dict.")
+                raise RuntimeError(
+                    "changing_models shall be a list of dictionaries."
+                )
 
-            if len(set(ChangingModels._fields) - set(model_info.keys())) > 0:
-                raise RuntimeError("The models element is missing a key.")
+            missing_keys = set(ChangingModels._fields) - set(model_info.keys())
+            if len(missing_keys) > 0:
+                raise RuntimeError(
+                    "Missing key on model_info. " + str(missing_keys)
+                )
 
             name = model_info["name"]
             if name not in train_results.keys():
-                raise RuntimeError("A variable name that does not exist.")
+                raise RuntimeError(f"Unknown name. ({name})")
 
             condition = model_info["condition"]
-            conditions = [cond_result.condition for cond_result in train_results[name]]
+            conditions = [
+                cond_result.condition for cond_result in train_results[name]
+            ]
             if condition not in conditions:
-                raise RuntimeError("This is a condition that does not exist in the training results.")
+                raise RuntimeError("Not-exsitent consition. " + str(condition))
 
             model = model_info["model"]
-            self._check_model_instance(model, name, categorical_info)
+            self._check_model_instance(model, name, cat_map)
 
-            changing_models_.append(ChangingModels(name=name, condition=condition, model=model))
+            changing_models_.append(
+                ChangingModels(name=name, condition=condition, model=model)
+            )
         return changing_models_
 
     def _get_causal_order(self, causal_graph):
         causal_order = []
 
         row_num = causal_graph.shape[0]
         original_index = np.arange(row_num)
 
         while 0 < len(causal_graph):
-            # find a row all of which elements are zero
-            row_index_list = np.where(np.sum(np.abs(causal_graph), axis=1) == 0)[0]
+            # finding rows where the elements are all zeros
+            row_index_list = np.where(
+                np.sum(np.abs(causal_graph), axis=1) == 0
+            )[0]
             if len(row_index_list) == 0:
                 break
 
             target_index = row_index_list[0]
 
             # append i to the end of the list
             causal_order.append(original_index[target_index])
             original_index = np.delete(original_index, target_index, axis=0)
 
-            # remove the i-th row and the i-th column from matrix
-            mask = np.delete(np.arange(len(causal_graph)), target_index, axis=0)
+            # remove i-th row and i-th column from matrix
+            mask = np.delete(
+                np.arange(len(causal_graph)),
+                target_index,
+                axis=0
+            )
             causal_graph = causal_graph[mask][:, mask]
 
         if len(causal_order) != row_num:
             causal_order = None
 
         return np.array(causal_order)
 
-    def _get_train_data(self, data, X_columns, y_column, categorical_info, changing_exog_df=None):
+    def _get_train_data(
+        self,
+        data,
+        X_cols,
+        y_col,
+        cat_map,
+        changing_exog_df=None
+    ):
         train_data_list = []
 
-        # column names of categorical varialbes in X_columns
-        X_columns_cat = set(X_columns) & set(categorical_info.keys())
-        X_columns_cat = sorted(X_columns_cat, key=lambda x: list(X_columns).index(x))
-
-        if len(X_columns_cat) == 0:
-            X = data.loc[:, X_columns].copy()
-            y = data.loc[:, y_column].copy()
+        # column names of categorical variables in X_columns
+        X_cols_cat = set(X_cols) & set(cat_map.keys())
+        X_cols_cat = sorted(X_cols_cat, key=lambda x: list(X_cols).index(x))
+
+        # no categorical variable in X
+        if len(X_cols_cat) == 0:
+            X = data.loc[:, X_cols].copy()
+            y = data.loc[:, y_col].copy()
 
-            # apply exogeous
+            # overwrite with exogenous
             if changing_exog_df is not None:
                 for col, series in changing_exog_df.items():
                     if col in X.columns.tolist():
                         X[col] = series
 
             train_data_list.append(TrainData(condition=None, X=X, y=y))
             return train_data_list
 
-        # column names of non-ategorical variables
-        X_columns_num = set(X_columns) - set(categorical_info.keys())
-        X_columns_num = sorted(X_columns_num, key=lambda x: list(X_columns).index(x))
+        # column names of non-categorical variables in X_columns
+        X_cols_num = set(X_cols) - set(cat_map.keys())
+        X_cols_num = sorted(X_cols_num, key=lambda x: list(X_cols).index(x))
+
+        # unique conditions by categorical parent nodes
+        uniq_conds = np.unique(
+            data.loc[:, X_cols_cat].values.tolist(),
+            axis=0
+        )
 
-        # unique conditions by parent nodes
-        uniq_conds = np.unique(data.loc[:, X_columns_cat].values.tolist(), axis=0)
         for uniq_cond in uniq_conds:
-            # filter X by the condition
-            target_index = np.argwhere(np.all(data.loc[:, X_columns_cat].values == uniq_cond, axis=1)).flatten()
-            X_filtered = data.iloc[target_index, :].loc[:, X_columns_num].copy()
-            y_filtered = data.iloc[target_index, :].loc[:, y_column].copy()
+            # filter by the condition
+            target_index = np.argwhere(
+                np.all(data.loc[:, X_cols_cat].values == uniq_cond, axis=1)
+            ).flatten()
 
-            # apply exogeous
+            X_filtered = data.iloc[target_index, :].loc[:, X_cols_num].copy()
+            y_filtered = data.iloc[target_index, :].loc[:, y_col].copy()
+
+            # overwrite with exogenous
             if changing_exog_df is not None:
                 for col, series in changing_exog_df.items():
                     if col in X.columns.tolist():
                         X_filtered[col] = series.loc[target_index]
 
             condition = {}
-            for column, value in zip(X_columns_cat, uniq_cond):
-                condition[column] = categorical_info[column][value]
+            for col_name, value in zip(X_cols_cat, uniq_cond):
+                condition[col_name] = cat_map[col_name][value]
 
-            train_data_list.append(TrainData(condition=condition, X=X_filtered, y=y_filtered))
+            train_data_list.append(
+                TrainData(condition=condition, X=X_filtered, y=y_filtered)
+            )
 
         return train_data_list
 
     def _predict_reg_model(self, X, model):
         try:
             predicted = model.predict(X.values)
         except Exception as e:
-            raise RuntimeError("An exception occurred during predict() of the model.:" + str(e))
+            raise RuntimeError(
+                "An exception occurred during predict() of the model. "
+                + str(e)
+            )
 
         return np.array(predicted)
 
     def _train_reg_model(self, X, y, model):
         try:
             model.fit(X.values, y.values)
         except Exception as e:
-            raise RuntimeError("An exception occurred during fit() of the model.:" + str(e))
+            raise RuntimeError(
+                "An exception occurred during fit() of the model. "
+                + str(e)
+            )
 
         predicted = self._predict_reg_model(X, model)
         predicted = pd.Series(predicted, index=X.index, dtype=y.dtype)
 
         resid = y - predicted
 
         return model, predicted, resid
 
     def _predict_clf_model(self, X, model):
         try:
             proba = model.predict_proba(X.values)
         except Exception as e:
-            raise RuntimeError("An exception occurred during predict_proba() of the model.:" + str(e))
+            raise RuntimeError(
+                "An exception occurred during predict_proba() of the model. "
+                + str(e)
+            )
 
         # sampling values based on predicted probability
         predicted = []
         for proba_ in proba:
             predicted.append(np.random.choice(model.classes_, p=proba_))
 
         return np.array(predicted)
 
-    def _train_clf_model(self, X, y, model, categorical_info):
+    def _train_clf_model(self, X, y, model, cat_map):
         try:
             model.fit(X.values, y.values)
         except Exception as e:
-            raise RuntimeError("An exception occurred during fit() of the model.:" + str(e))
+            raise RuntimeError(
+                "An exception occurred during fit() of the model. "
+                + str(e)
+            )
 
         predicted = self._predict_clf_model(X, model)
         predicted = pd.Series(predicted, index=X.index, dtype=y.dtype)
 
         # classifier doesn't have residuals
         resid = None
-
         return model, predicted, resid
 
     def _concat_residuals(self, train_results, to_name, index):
         ret = []
 
         cond_results = train_results[to_name]
+
         for cond_result in cond_results:
             series = getattr(cond_result, "residual")
+
             if series is None:
                 predicted = getattr(cond_result, "predicted")
-                series = pd.Series(np.ones(predicted.shape[0]) * np.nan, index=predicted.index)
+                series = pd.Series(
+                    np.ones(predicted.shape[0]) * np.nan,
+                    index=predicted.index
+                )
+
             ret.append(series)
+
+        # concat and sort by original index
         ret = pd.concat(ret, axis=0).loc[index]
 
         return ret
 
     def _concat_predicts(self, train_results, to_name, index):
         ret = []
 
@@ -409,187 +542,233 @@
         for cond_result in cond_results:
             series = getattr(cond_result, "predicted")
             ret.append(series)
         ret = pd.concat(ret, axis=0).loc[index]
 
         return ret
 
-    def _prepare_to_expose_train(self, train_results, categorical_info):
+    def _prep_to_expose_train(self, train_results, cat_map):
         train_results_ = {}
+
         for to_name, cond_results in train_results.items():
             train_result_ = []
+
             for result in cond_results:
                 result_ = {}
+
                 if result.condition is None:
                     result_["condition"] = None
                 else:
-                    result_["condition"] = {k: v for k, v in result.condition.items()}
+                    result_["condition"] = {
+                        k: v for k, v in result.condition.items()
+                    }
+
                 result_["model"] = result.model
+
                 result_["exp_columns"] = result.exp_columns
 
-                if to_name not in categorical_info.keys():
+                if to_name not in cat_map.keys():
                     # non categorical
                     result_["predicted"] = result.predicted
                 else:
                     # categorical
-                    result_["predicted"] = result.predicted.map(lambda x: categorical_info[to_name][x])
+                    result_["predicted"] = result.predicted.map(
+                        lambda x: cat_map[to_name][x]
+                    )
 
                 result_["residual"] = result.residual
 
                 train_result_.append(result_)
             train_results_[to_name] = train_result_
+
         return train_results_
 
-    def _train(self, data, categorical_info, causal_graph, models):
+    def _train(self, data, cat_map, graph, models):
         train_results = {}
 
-        for to_index, graph_row in enumerate(causal_graph):
+        for to_index, graph_row in enumerate(graph):
             cond_results = []
 
-            to_name = data.columns[to_index]
+            from_indices = np.argwhere(
+                ~np.isclose(graph_row, 0)
+            ).flatten()
 
-            from_indices = np.argwhere(~np.isclose(graph_row, 0)).flatten()
+            # get column names
+            to_name = data.columns[to_index]
             from_names = data.columns[from_indices]
+            from_names_num = sorted(
+                set(from_names) - set(cat_map.keys()),
+                key=lambda x: list(data.columns).index(x)
+            )
 
             # making data list splitted by conditions
-            train_data_list = self._get_train_data(data, from_names, to_name, categorical_info)
-
-            from_names_num = sorted(set(from_names) - set(categorical_info.keys()), key=lambda x: list(data.columns).index(x))
+            cond_tr_data = self._get_train_data(
+                data,
+                from_names,
+                to_name,
+                cat_map
+            )
 
-            # most topstream
+            # node with no parents
             if len(from_names) == 0:
                 train_results[to_name] = []
                 continue
 
-            for train_data in train_data_list:
+            # node with parents
+            for tr_data in cond_tr_data:
+                # selecting a model to train
                 if to_name in models.keys():
-                    # given model
                     model = clone(models[to_name])
                 else:
-                    # default model
                     if len(from_names_num) > 0:
-                        if to_name in categorical_info.keys():
+                        # default
+                        if to_name in cat_map.keys():
                             model = LogisticRegression()
                         else:
                             model = LinearRegression()
                     else:
-                        # no explanatory (only categorical variables)
-                        if to_name in categorical_info.keys():
-                            model = CbsCategoricalClassifier()
+                        # no non-categorical parents
+                        if to_name in cat_map.keys():
+                            model = DummyClassifier(strategy="uniform")
                         else:
-                            model = CbsExpectedValueRegressor()
+                            model = DummyRegressor()
 
-                if to_name in categorical_info.keys():
-                    model, predicted, resid = self._train_clf_model(train_data.X, train_data.y, model, categorical_info)
+                # train model
+                if to_name in cat_map.keys():
+                    model, predicted, resid = self._train_clf_model(
+                        tr_data.X,
+                        tr_data.y,
+                        model,
+                        cat_map
+                    )
                 else:
-                    model, predicted, resid = self._train_reg_model(train_data.X, train_data.y, model)
-
-                cond_results.append(TrainResult(condition=train_data.condition,
-                                                model=model, exp_columns=from_names_num, predicted=predicted, residual=resid))
+                    model, predicted, resid = self._train_reg_model(
+                        tr_data.X,
+                        tr_data.y,
+                        model
+                    )
+
+                cond_results.append(TrainResult(
+                    condition=tr_data.condition,
+                    model=model,
+                    exp_columns=from_names_num,
+                    predicted=predicted,
+                    residual=resid
+                ))
             train_results[to_name] = cond_results
+
         return train_results
 
-    def _select_changing_model(self, changing_models, to_name, condition):
+    def _select_changing_model(
+        self,
+        changing_models,
+        to_name,
+        condition
+    ):
         for model_info in changing_models:
             if model_info.name != to_name:
                 continue
             elif model_info.condition != condition:
                 continue
+
             return model_info.model
         return None
 
-    def _simulate(self, data, causal_graph, causal_order, categorical_info, changing_exog_df,
-                  changing_models, train_results, shuffle_residual, random_state):
+    def _simulate(
+        self,
+        data,
+        causal_graph,
+        causal_order,
+        cat_map,
+        changing_exog_df,
+        changing_models,
+        train_results,
+        shuffle_residual,
+        random_state
+    ):
         sim_df = pd.DataFrame(index=data.index)
 
-        # predict from upstream to downstream
+        # predicting from upstream to downstream
         for to_index in causal_order:
-            # input column of node i is the nonzero column of row i of the adjacency matrix.
+            # input nodes of node i are nonzero variables of i-th row of graph
             from_indices = causal_graph[to_index, :]
             from_indices = np.argwhere(~np.isclose(from_indices, 0)).flatten()
 
             to_name = data.columns[to_index]
-            from_names = [data.columns[from_index] for from_index in from_indices]
+            from_names = [
+                data.columns[from_index] for from_index in from_indices
+            ]
 
-            # no predictions by model for root node. The data is same as X.
+            # assigning values without predicting if to_name has no parents.
             if len(from_names) == 0:
                 sim_df[to_name] = data[to_name].copy()
                 continue
 
             if to_name in changing_exog_df.columns:
                 error = changing_exog_df[to_name]
-            elif to_name not in categorical_info.keys():
-                error = self._concat_residuals(train_results, to_name, data.index)
+            elif to_name not in cat_map.keys():
+                error = self._concat_residuals(
+                    train_results,
+                    to_name,
+                    data.index
+                )
 
             X = sim_df[from_names]
 
-            # simulate for each conditions
+            # simulation for each conditions
             y_sim = []
             for cond_result in train_results[to_name]:
                 X_ = X
 
                 if cond_result.condition is not None:
-                    # filter rows by condition
+                    # filter rows by a condition
                     filter_ = []
                     for key, value in cond_result.condition.items():
-                        filter_.append(X_[key] == categorical_info[key].index(value))
+                        filter_.append(X_[key] == cat_map[key].index(value))
                     filter_ = np.all(filter_, axis=0)
                     X_ = X_.loc[filter_, :]
 
-                # filter columns by explanatory
+                # filter columns by explanatories
                 if len(cond_result.exp_columns) > 0:
                     X_ = X_.loc[:, cond_result.exp_columns]
                 else:
                     # dummy data when all parent nodes are categorical
-                    X_ = pd.DataFrame(np.ones(X_.shape[0]).reshape(X_.shape[0]) * np.nan, index=X_.index, columns=[to_name])
-
-                # select a model to simulate
-                model = self._select_changing_model(changing_models, to_name, cond_result.condition)
+                    X_ = pd.DataFrame(
+                        np.ones(X_.shape[0]).reshape(X_.shape[0]) * np.nan,
+                        index=X_.index,
+                        columns=[to_name]
+                    )
+
+                # selecting a model for the simulation
+                model = self._select_changing_model(
+                    changing_models,
+                    to_name,
+                    cond_result.condition
+                )
                 if model is None:
                     model = cond_result.model
 
-                if to_name in categorical_info.keys():
+                if to_name in cat_map.keys():
                     y_hat = self._predict_clf_model(X_, model)
                 else:
                     y_hat = self._predict_reg_model(X_, model)
 
                     cond_error = error.loc[X_.index]
                     if shuffle_residual is True:
-                        cond_error = cond_error.sample(frac=1, random_state=random_state)
+                        cond_error = cond_error.sample(
+                            frac=1,
+                            random_state=random_state
+                        )
                     y_hat += cond_error
 
                 y_sim.append(pd.Series(y_hat, index=X_.index))
             sim_df[to_name] = pd.concat(y_sim, axis=0).loc[data.index]
         sim_df = sim_df.loc[data.index, data.columns]
 
-        # decode categorical values
-        for column, categories in categorical_info.items():
-            sim_df[column] = sim_df[column].map(lambda idx: categories[idx])
-            sim_df[column] = sim_df[column].astype("category")
+        # decoding categorical values
+        for col_name, categories in cat_map.items():
+            sim_df[col_name] = sim_df[col_name].map(
+                lambda idx: categories[idx]
+            )
+            sim_df[col_name] = sim_df[col_name].astype("category")
 
         return sim_df
-
-
-class CbsExpectedValueRegressor(BaseEstimator, RegressorMixin):
-    # Regression model to be used when there is no explanatory variable.
-
-    def fit(self, X, y):
-        self.expected_value_ = np.mean(y)
-
-    def predict(self, X):
-        y_hat = self.expected_value_ * np.ones(X.shape[0])
-        return y_hat
-
-
-class CbsCategoricalClassifier(BaseEstimator, ClassifierMixin):
-    # classification model to be used when there is no explanatory variable.
-
-    def fit(self, X, y):
-        values, counts = np.unique(y, return_counts=True)
-        p = np.array([c / y.shape[0] for c in counts])
-
-        self.p_ = p
-        self.classes_ = values
-        return self
-
-    def predict_proba(self, X):
-        return [self.p_] * X.shape[0]
```

### Comparing `lingam-1.7.1/lingam/causal_effect.py` & `lingam-1.8.0/lingam/causal_effect.py`

 * *Files identical despite different names*

### Comparing `lingam-1.7.1/lingam/direct_lingam.py` & `lingam-1.8.0/lingam/direct_lingam.py`

 * *Files identical despite different names*

### Comparing `lingam-1.7.1/lingam/hsic.py` & `lingam-1.8.0/lingam/hsic.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 import numpy as np
 from scipy.stats import gamma
 from statsmodels.nonparametric import bandwidths
 
 __all__ = ["get_kernel_width", "get_gram_matrix", "hsic_teststat", "hsic_test_gamma"]
 
+# Modify hsic with reference to causal-learn:
+# causallearn/search/FCMBased/lingam/hsic.py
+
 
 def get_kernel_width(X):
     """Calculate the bandwidth to median distance between points.
     Use at most 100 points (since median is only a heuristic,
     and 100 points is sufficient for a robust estimate).
 
     Parameters
@@ -30,36 +33,26 @@
     if n_samples > 100:
         X_med = X[:100, :]
         n_samples = 100
     else:
         X_med = X
 
     G = np.sum(X_med * X_med, 1).reshape(n_samples, 1)
-    Q = np.tile(G, (1, n_samples))
-    R = np.tile(G.T, (n_samples, 1))
-
-    dists = Q + R - 2 * np.dot(X_med, X_med.T)
+    dists = G + G.T - 2 * np.dot(X_med, X_med.T)
     dists = dists - np.tril(dists)
-    dists = dists.reshape(n_samples ** 2, 1)
+    dists = dists.reshape(n_samples**2, 1)
 
     return np.sqrt(0.5 * np.median(dists[dists > 0]))
 
 
-def _rbf_dot(X, Y, width):
-    """Compute the inner product of radial basis functions."""
-    n_samples_X = X.shape[0]
-    n_samples_Y = Y.shape[0]
-
-    G = np.sum(X * X, 1).reshape(n_samples_X, 1)
-    H = np.sum(Y * Y, 1).reshape(n_samples_Y, 1)
-    Q = np.tile(G, (1, n_samples_Y))
-    R = np.tile(H.T, (n_samples_X, 1))
-    H = Q + R - 2 * np.dot(X, Y.T)
-
-    return np.exp(-H / 2 / (width ** 2))
+def _rbf_dot(X, width):
+    """rbf dot, in special case with X dot X"""
+    G = np.sum(X * X, axis=1)
+    H = G[None, :] + G[:, None] - 2 * np.dot(X, X.T)
+    return np.exp(-H / 2 / (width**2))
 
 
 def get_gram_matrix(X, width):
     """Get the centered gram matrices.
 
     Parameters
     ----------
@@ -72,19 +65,20 @@
 
     Returns
     -------
     K, Kc : array
         the centered gram matrices.
     """
     n = X.shape[0]
-    H = np.eye(n) - 1 / n * np.ones((n, n))
-
-    K = _rbf_dot(X, X, width)
-    Kc = np.dot(np.dot(H, K), H)
 
+    K = _rbf_dot(X, width)
+    K_colsums = K.sum(axis=0)
+    K_rowsums = K.sum(axis=1)
+    K_allsum = K_rowsums.sum()
+    Kc = K - (K_colsums[None, :] + K_rowsums[:, None]) / n + (K_allsum / n**2)
     return K, Kc
 
 
 def hsic_teststat(Kc, Lc, n):
     """get the HSIC statistic.
 
     Parameters
@@ -97,15 +91,15 @@
 
     Returns
     -------
     float
         the HSIC statistic.
     """
     # test statistic m*HSICb under H1
-    return 1 / n * np.sum(np.sum(Kc.T * Lc))
+    return 1 / n * np.sum(Kc.T * Lc)
 
 
 def hsic_test_gamma(X, Y, bw_method="mdbs"):
     """get the HSIC statistic.
 
     Parameters
     ----------
@@ -144,29 +138,28 @@
 
     # these are slightly biased estimates of centered gram matrices
     K, Kc = get_gram_matrix(X, width_x)
     L, Lc = get_gram_matrix(Y, width_y)
 
     # test statistic m*HSICb under H1
     n = X.shape[0]
-    bone = np.ones((n, 1))
     test_stat = hsic_teststat(Kc, Lc, n)
 
     var = (1 / 6 * Kc * Lc) ** 2
     # second subtracted term is bias correction
-    var = 1 / n / (n - 1) * (np.sum(np.sum(var)) - np.sum(np.diag(var)))
+    var = 1 / n / (n - 1) * (np.sum(var) - np.trace(var))
     # variance under H0
     var = 72 * (n - 4) * (n - 5) / n / (n - 1) / (n - 2) / (n - 3) * var
 
-    K = K - np.diag(np.diag(K))
-    L = L - np.diag(np.diag(L))
-    mu_X = 1 / n / (n - 1) * np.dot(bone.T, np.dot(K, bone))
-    mu_Y = 1 / n / (n - 1) * np.dot(bone.T, np.dot(L, bone))
+    K[np.diag_indices(n)] = 0
+    L[np.diag_indices(n)] = 0
+    mu_X = 1 / n / (n - 1) * K.sum()
+    mu_Y = 1 / n / (n - 1) * L.sum()
     # mean under H0
     mean = 1 / n * (1 + mu_X * mu_Y - mu_X - mu_Y)
 
-    alpha = mean ** 2 / var
+    alpha = mean**2 / var
     # threshold for hsicArr*m
-    beta = np.dot(var, n) / mean
-    p = 1 - gamma.cdf(test_stat, alpha, scale=beta)[0][0]
+    beta = var * n / mean
+    p = gamma.sf(test_stat, alpha, scale=beta)
 
     return test_stat, p
```

### Comparing `lingam-1.7.1/lingam/ica_lingam.py` & `lingam-1.8.0/lingam/ica_lingam.py`

 * *Files identical despite different names*

### Comparing `lingam-1.7.1/lingam/lim.py` & `lingam-1.8.0/lingam/lim.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 """
 Python implementation of the LiNGAM algorithms.
 The LiNGAM Project: https://sites.google.com/view/sshimizu06/lingam
 """
 
+from itertools import product
+
+import networkx as nx
 import numpy as np
+import pandas as pd
 import scipy.optimize as sopt
 from scipy.special import expit as sigmoid
-# import time
-import pandas as pd
-import networkx as nx
 from sklearn.linear_model import LinearRegression, LogisticRegression
 from sklearn.metrics import log_loss
-# from Combining import likelihood
-# import random
-# import itertools
-from itertools import product # , combinations, chain
+
 import lingam.utils as ut
 
 
 class LiM:
     """Implementation of LiM Algorithm [1]_
 
     References
     ----------
     .. [1] Zeng Y, Shimizu S, Matsui H, et al. Causal discovery for
        linear mixed data[C]//Conference on Causal Learning and Rea-
        soning. PMLR, 2022: 994-1009.
     """
 
     def __init__(
-            self,
-            lambda1=0.1,
-            loss_type='mixed',
-            max_iter=150,
-            h_tol=1e-8,
-            rho_max=1e+16,
-            w_threshold=0.1,
+        self,
+        lambda1=0.1,
+        loss_type="mixed",
+        max_iter=150,
+        h_tol=1e-8,
+        rho_max=1e16,
+        w_threshold=0.1,
     ):
         """Construct a LiM model.
 
         Parameters
         ----------
         lambda1 : float, optional (default=0.1)
              L1 penalty parameter.
@@ -86,49 +84,53 @@
 
     def _estimate_LiM(self, X, dis_con):
         """Estimate the adjacency matrix btw. mixed variables"""
 
         def _loss(W):
             """Evaluate value and gradient of loss."""
             M = X @ W
-            if self._loss_type == 'logistic':
+            if self._loss_type == "logistic":
                 loss = 1.0 / X.shape[0] * (np.logaddexp(0, M) - X * M).sum()
                 G_loss = 1.0 / X.shape[0] * X.T @ (sigmoid(M) - X)
-            elif self._loss_type == 'laplace':
+            elif self._loss_type == "laplace":
                 R = X - M
-                loss = - 1.0 / X.shape[0] * np.sum(- np.log(np.cosh(R)))
+                loss = -1.0 / X.shape[0] * np.sum(-np.log(np.cosh(R)))
                 G_loss = 1.0 / X.shape[0] * X.T @ np.tanh(R)
-            elif self._loss_type == 'mixed':
+            elif self._loss_type == "mixed":
                 R = X - M
                 a1, a2 = 1, 1
-                loss_dis = ((np.logaddexp(0, M) - X * M) * np.absolute(dis_con - 1)).sum()
+                loss_dis = (
+                    (np.logaddexp(0, M) - X * M) * np.absolute(dis_con - 1)
+                ).sum()
                 loss_con = np.sum(-np.log(np.cosh(R)) * dis_con)
                 loss = -1.0 / X.shape[0] * (a1 * loss_dis + a2 * loss_con)
                 W_dis = np.zeros([d, d])
                 W_con = np.zeros([d, d])
                 for ii in np.where(dis_con[0, :] == 0):
                     W_dis[[ii], :] = 1
                     W_dis[:, [ii]] = 1
                 for jj in np.where(dis_con[0, :] == 1):
                     W_con[[jj], :] = 1
                     W_con[:, [jj]] = 1
                 G_dis = X.T @ (sigmoid(M) - X) * W_dis
-                G_con = - X.T @ np.tanh(R) * W_con
+                G_con = -X.T @ np.tanh(R) * W_con
                 G_loss = 1.0 / X.shape[0] * (G_dis + G_con)
-            elif self._loss_type == 'mixed_dag':
+            elif self._loss_type == "mixed_dag":
                 dag = nx.DiGraph(W)
                 lingam_data = np.transpose(X)
                 df = pd.DataFrame(X)
                 is_continuous = dis_con[0, :].astype(bool)
                 is_discrete = np.invert(is_continuous)
-                loss = - _bic_scoring(dag, is_discrete, df, lingam_data)  # lingam_data:dims*samples
+                loss = -_bic_scoring(
+                    dag, is_discrete, df, lingam_data
+                )  # lingam_data:dims*samples
                 R = X - M
                 G_loss = 1.0 / X.shape[0] * (X.T @ (sigmoid(M) - X) - X.T @ np.tanh(R))
             else:
-                raise ValueError('unknown loss type')
+                raise ValueError("unknown loss type")
             return loss, G_loss
 
         def _bic_scoring(dag: nx.DiGraph, is_discrete, df, lingam_data):
             """Evaluate value of loss given the DAG."""
             sample_size = df.shape[0]
             K = dag.number_of_edges() + dag.number_of_nodes()
             # K = dag.number_of_edges() + np.sum(is_discrete)
@@ -141,27 +143,33 @@
                 # 離散
                 if is_discrete[i]:
                     if not parents_i:
                         # Bernoulli binary variable, likelihood using Bernoulli model with MLE parameters
                         frequency_table = df[i].value_counts()
                         likekihood_bernoulli = 0.0
                         for count_k in frequency_table:
-                            likekihood_bernoulli += count_k * (np.log(count_k) - np.log(frequency_table.sum()))
+                            likekihood_bernoulli += count_k * (
+                                np.log(count_k) - np.log(frequency_table.sum())
+                            )
                         total_score += likekihood_bernoulli
 
                     elif parents_i:
                         # Logistic binary variable, likelihood using logistic regression model.
                         X = df[parents_i]
                         y = df[i]
-                        logistic = LogisticRegression(solver='lbfgs')  # or solver='liblinear'
+                        logistic = LogisticRegression(
+                            solver="lbfgs"
+                        )  # or solver='liblinear'
                         logistic.fit(X, y)
                         predict_prob = logistic.predict_proba(X)
 
                         # Negative cross-entropy loss a.k.a log-likelihood
-                        likekihood_logistic = -log_loss(y_true=y, y_pred=predict_prob, normalize=False)
+                        likekihood_logistic = -log_loss(
+                            y_true=y, y_pred=predict_prob, normalize=False
+                        )
                         total_score += likekihood_logistic
                     pass
                 # 連続
                 elif not is_discrete[i]:
                     b_i = np.zeros(dag.number_of_nodes())
 
                     if parents_i:  # estimate b_i
@@ -189,90 +197,108 @@
             M = np.eye(d) + W * W / d  # (Yu et al. 2019)
             G_h = np.linalg.matrix_power(M, d - 1)
             h = (G_h.T * M).sum() - d
             return h, G_h
 
         def _adj(w):
             """Convert doubled variables ([2 d^2] array) back to original variables ([d, d] matrix)."""
-            return (w[:d * d] - w[d * d:]).reshape([d, d])
+            return (w[: d * d] - w[d * d :]).reshape([d, d])
 
         def _func(w):
             """Evaluate value and gradient of augmented Lagrangian for doubled variables ([2 d^2] array)."""
             W = _adj(w)
             loss, G_loss = _loss(W)
             h, G_h = _h(W)
             obj = loss + 0.5 * rho * h * h + alpha * h + self._lambda1 * w.sum()
             # G_smooth = G_loss + (rho * h + alpha) * G_h # Zheng Xun Dag 2018
             G_smooth = G_loss + (rho * h + alpha) * G_h.T * W * 2  # 2019
-            g_obj = np.concatenate((G_smooth + self._lambda1, - G_smooth + self._lambda1), axis=None)
+            g_obj = np.concatenate(
+                (G_smooth + self._lambda1, -G_smooth + self._lambda1), axis=None
+            )
             return obj, g_obj
 
         n, d = X.shape
-        w_est, rho, alpha, h = np.random.random(2 * d * d), 1.0, 0.0, np.inf  # double w_est into (w_pos, w_neg)
-        bnds = [(0, 0) if i == j else (0, None) for _ in range(2) for i in range(d) for j in range(d)]
+        w_est, rho, alpha, h = (
+            np.random.random(2 * d * d),
+            1.0,
+            0.0,
+            np.inf,
+        )  # double w_est into (w_pos, w_neg)
+        bnds = [
+            (0, 0) if i == j else (0, None)
+            for _ in range(2)
+            for i in range(d)
+            for j in range(d)
+        ]
 
         # if self._loss_type == 'l2':
         #     X = X - np.mean(X, axis=0, keepdims=True)
         for _ in range(self._max_iter):
             w_new, h_new = None, None
             while rho < self._rho_max:
-                sol = sopt.minimize(_func, w_est, method='L-BFGS-B', jac=True, bounds=bnds)
+                sol = sopt.minimize(
+                    _func, w_est, method="L-BFGS-B", jac=True, bounds=bnds
+                )
                 # print('--- One iteration passed.....', sol.fun)
                 w_new = sol.x
                 h_new, _ = _h(_adj(w_new))
                 if h_new >= 0.25 * h:
                     rho *= 10
                 else:
                     break
             w_est, h = w_new, h_new
             alpha += rho * h
             # print('------- rho  is:', rho)
             if h <= self._h_tol and h != 0:
                 break
-            if rho >= self._rho_max * 1e-6 and h > 1e+05:  # avoid the full graph
+            if rho >= self._rho_max * 1e-6 and h > 1e05:  # avoid the full graph
                 w_est = np.random.random(2 * d * d)
                 rho = 1.0
             elif rho >= self._rho_max:
                 break
             if np.sum(np.absolute(_adj(w_est))) < 0.09:  # avoid the zero matrix
                 w_est = np.random.random(2 * d * d)
         W_est = _adj(w_est)
         W_est[np.abs(W_est) < self._w_threshold] = 0
         # print('W_est (without the 2nd phase) is: \n', W_est)
 
-        self._loss_type = 'mixed_dag'
+        self._loss_type = "mixed_dag"
         aa, aaa = _loss(W_est)  # loss
         I = np.where(W_est != 0)
         # check directions
         W_min_lss = np.copy(W_est)
-        candi_setting = list(product(range(2), repeat=len(I[0])))  # 1:reverse the direction； 0:unchanged
+        candi_setting = list(
+            product(range(2), repeat=len(I[0]))
+        )  # 1:reverse the direction； 0:unchanged
         for candi_setting_i in range(1, len(candi_setting)):
             W_tmp = np.copy(W_est)
             for iii in range(len(I[0])):  # transform to W_tmp
                 if candi_setting[candi_setting_i][iii] == 1:
                     W_tmp[I[0][iii], I[1][iii]] = 0
                     W_tmp[I[1][iii], I[0][iii]] = 1
             lss, lss_G = _loss(W_tmp)
             if lss < aa and _h(W_tmp)[0] < self._h_tol:
                 W_min_lss = np.copy(W_tmp)
                 aa = lss
 
         # prune process
-        if d > 2 and len(I[0]) > (d - 1):     # > min_edge
+        if d > 2 and len(I[0]) > (d - 1):  # > min_edge
             W0 = np.copy(W_min_lss)
             I_delete = np.where(W_min_lss != 0)
             for delete_i in range(len(I_delete[0])):
                 W_tmp = np.copy(W0)
                 W_tmp[I_delete[0][delete_i], I_delete[1][delete_i]] = 0
                 lss, lss_G = _loss(W_tmp)
                 if lss < aa and _h(W_tmp)[0] < self._h_tol:
                     W_min_lss = np.copy(W_tmp)
                     aa = lss
             #
-            if not np.all(W_est.astype(bool) == W_min_lss.astype(bool)):  # if they are different
+            if not np.all(
+                W_est.astype(bool) == W_min_lss.astype(bool)
+            ):  # if they are different
                 W0 = np.copy(W_est)
                 for delete_i in range(len(I[0])):
                     W_tmp = np.copy(W0)
                     W_tmp[I[0][delete_i], I[1][delete_i]] = 0
                     lss, lss_G = _loss(W_tmp)
                     if lss < aa and _h(W_tmp)[0] < self._h_tol:
                         W_min_lss = np.copy(W_tmp)
@@ -286,15 +312,17 @@
                 W_tmp = np.copy(W0)
                 W_tmp[I_add[0][add_i], I_add[1][add_i]] = 1
                 lss, lss_G = _loss(W_tmp)
                 if lss < aa and _h(W_tmp)[0] < self._h_tol:
                     W_min_lss = np.copy(W_tmp)
                     aa = lss
             #
-            if not np.all(W_est.astype(bool) == W_min_lss.astype(bool)):  # if they are different
+            if not np.all(
+                W_est.astype(bool) == W_min_lss.astype(bool)
+            ):  # if they are different
                 W0 = np.copy(W_est)
                 W_edges = W0 + W0.T + np.eye(d)
                 I_add = np.where(W_edges == 0)  # add undirected edges' indices
                 for add_i in range(len(I_add[0])):
                     W_tmp = np.copy(W0)
                     W_tmp[I_add[0][add_i], I_add[1][add_i]] = 1
                     lss, lss_G = _loss(W_tmp)
@@ -312,8 +340,8 @@
 
         Returns
         -------
         adjacency_matrix_ : array-like, shape (n_features, n_features)
             The adjacency matrix of variables, where
             ``n_features`` is the number of observed variables.
         """
-        return self._adjacency_matrix
+        return self._adjacency_matrix
```

### Comparing `lingam-1.7.1/lingam/lina.py` & `lingam-1.8.0/lingam/lina.py`

 * *Files identical despite different names*

### Comparing `lingam-1.7.1/lingam/longitudinal_lingam.py` & `lingam-1.8.0/lingam/longitudinal_lingam.py`

 * *Files identical despite different names*

### Comparing `lingam-1.7.1/lingam/multi_group_direct_lingam.py` & `lingam-1.8.0/lingam/multi_group_direct_lingam.py`

 * *Files identical despite different names*

### Comparing `lingam-1.7.1/lingam/rcd.py` & `lingam-1.8.0/lingam/rcd.py`

 * *Files identical despite different names*

### Comparing `lingam-1.7.1/lingam/resit.py` & `lingam-1.8.0/lingam/resit.py`

 * *Files identical despite different names*

### Comparing `lingam-1.7.1/lingam/var_lingam.py` & `lingam-1.8.0/lingam/var_lingam.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,22 +265,22 @@
         return p_values
 
     def _estimate_var_coefs(self, X):
         """Estimate coefficients of VAR"""
         # XXX: VAR.fit() is not searching lags correctly
         if self._criterion not in ["aic", "fpe", "hqic", "bic"]:
             var = VAR(X)
-            result = var.fit(maxlags=self._lags, trend="nc")
+            result = var.fit(maxlags=self._lags, trend="n")
         else:
             min_value = float("Inf")
             result = None
 
             for lag in range(1, self._lags + 1):
                 var = VAR(X)
-                fitted = var.fit(maxlags=lag, ic=None, trend="nc")
+                fitted = var.fit(maxlags=lag, ic=None, trend="n")
 
                 value = getattr(fitted, self._criterion)
                 if value < min_value:
                     min_value = value
                     result = fitted
 
         return result.coefs, result.k_ar, result.resid
```

### Comparing `lingam-1.7.1/lingam/varma_lingam.py` & `lingam-1.8.0/lingam/varma_lingam.py`

 * *Files identical despite different names*

### Comparing `lingam-1.7.1/lingam.egg-info/PKG-INFO` & `lingam-1.8.0/lingam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lingam
-Version: 1.7.1
+Version: 1.8.0
 Summary: LiNGAM Python Package
 Home-page: https://github.com/cdt15/lingam
 Author: T.Ikeuchi, G.Haraoka, M.Ide, W.Kurebayashi, S.Shimizu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `lingam-1.7.1/setup.py` & `lingam-1.8.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         'graphviz',
         'statsmodels',
         'factor_analyzer',
         'igraph',
         'networkx',
         'pandas',
         'pygam',
+        'matplotlib',
     ],
     url='https://github.com/cdt15/lingam',
     packages=setuptools.find_packages(exclude=['tests']),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
```

