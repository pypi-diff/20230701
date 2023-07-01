# Comparing `tmp/mafese-0.1.5.tar.gz` & `tmp/mafese-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mafese-0.1.5.tar", last modified: Thu Jun 15 09:52:38 2023, max compression
+gzip compressed data, was "mafese-0.1.6.tar", last modified: Sat Jul  1 09:51:10 2023, max compression
```

## Comparing `mafese-0.1.5.tar` & `mafese-0.1.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:52:38.781912 mafese-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-15 09:51:23.000000 mafese-0.1.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-15 09:51:23.000000 mafese-0.1.5/ChangeLog.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-15 09:51:23.000000 mafese-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-15 09:51:23.000000 mafese-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16001 2023-06-15 09:52:38.781912 mafese-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-06-15 09:51:23.000000 mafese-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:52:38.773912 mafese-0.1.5/mafese/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-15 09:51:23.000000 mafese-0.1.5/mafese/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:52:38.777912 mafese-0.1.5/mafese/embedded/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/embedded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/embedded/lasso.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/embedded/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/unsupervised.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:52:38.777912 mafese-0.1.5/mafese/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/utils/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/utils/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/utils/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/utils/estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/utils/mealpy_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/utils/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:52:38.777912 mafese-0.1.5/mafese/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/wrapper/mha.py
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/wrapper/recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-06-15 09:51:24.000000 mafese-0.1.5/mafese/wrapper/sequential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:52:38.777912 mafese-0.1.5/mafese.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16001 2023-06-15 09:52:38.000000 mafese-0.1.5/mafese.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-15 09:52:38.000000 mafese-0.1.5/mafese.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:52:38.000000 mafese-0.1.5/mafese.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-15 09:52:38.000000 mafese-0.1.5/mafese.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 09:52:38.000000 mafese-0.1.5/mafese.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 09:52:38.781912 mafese-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-15 09:51:24.000000 mafese-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:52:38.777912 mafese-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-15 09:51:24.000000 mafese-0.1.5/tests/test_embedded.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-15 09:51:24.000000 mafese-0.1.5/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-15 09:51:24.000000 mafese-0.1.5/tests/test_unsupervised.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-15 09:51:24.000000 mafese-0.1.5/tests/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:51:10.820963 mafese-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-01 09:50:03.000000 mafese-0.1.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-01 09:50:03.000000 mafese-0.1.6/ChangeLog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 09:50:03.000000 mafese-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-01 09:50:03.000000 mafese-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13007 2023-07-01 09:51:10.820963 mafese-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-07-01 09:50:03.000000 mafese-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:51:10.816963 mafese-0.1.6/mafese/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:51:10.816963 mafese-0.1.6/mafese/embedded/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/embedded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/embedded/lasso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/embedded/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/unsupervised.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:51:10.820963 mafese-0.1.6/mafese/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/utils/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/utils/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/utils/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/utils/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/utils/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/utils/mealpy_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/utils/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:51:10.820963 mafese-0.1.6/mafese/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34491 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/wrapper/mha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/wrapper/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/wrapper/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:51:10.816963 mafese-0.1.6/mafese.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13007 2023-07-01 09:51:10.000000 mafese-0.1.6/mafese.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-01 09:51:10.000000 mafese-0.1.6/mafese.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 09:51:10.000000 mafese-0.1.6/mafese.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-01 09:51:10.000000 mafese-0.1.6/mafese.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-01 09:51:10.000000 mafese-0.1.6/mafese.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 09:51:10.820963 mafese-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-01 09:50:03.000000 mafese-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:51:10.820963 mafese-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-01 09:50:03.000000 mafese-0.1.6/tests/test_embedded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-01 09:50:03.000000 mafese-0.1.6/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-01 09:50:03.000000 mafese-0.1.6/tests/test_unsupervised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-01 09:50:03.000000 mafese-0.1.6/tests/test_wrapper.py
```

### Comparing `mafese-0.1.5/CODE_OF_CONDUCT.md` & `mafese-0.1.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `mafese-0.1.5/ChangeLog.md` & `mafese-0.1.6/ChangeLog.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+# Version 0.1.6
+
++ Rename some public functions to private functions
++ Add MultiMhaSelector class
++ Add Matplotlib library and support visualization for MultiMhaSelector class
++ Add dependency plotly>=5.10.0 and kaleido >=0.2.1
++ Update examples for some Selector class
++ Replace evaluator module by evaluate method in Selector class.
+
+---------------------------------------------------------------------
+
 # Version 0.1.5
 
 + Add more regression and classification datasets
 + Update documents, examples, test
 + Remove matplotlib dependency
 
 ---------------------------------------------------------------------
```

### Comparing `mafese-0.1.5/LICENSE` & `mafese-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mafese-0.1.5/mafese/__init__.py` & `mafese-0.1.6/mafese/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 15:23, 06/03/2022 ----------%                                                                               
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 
 from mafese.utils.data_loader import Data, get_dataset
 from mafese.filter import FilterSelector
 from mafese.wrapper.recursive import RecursiveSelector
 from mafese.wrapper.sequential import SequentialSelector
-from mafese.wrapper.mha import MhaSelector
+from mafese.wrapper.mha import MhaSelector, MultiMhaSelector
 from mafese.embedded.lasso import LassoSelector
 from mafese.embedded.tree import TreeSelector
 from mafese.unsupervised import UnsupervisedSelector
```

### Comparing `mafese-0.1.5/mafese/embedded/lasso.py` & `mafese-0.1.6/mafese/embedded/lasso.py`

 * *Files 11% similar despite different names*

```diff
@@ -73,29 +73,31 @@
     >>> # check the index of selected features
     >>> print(feat_selector.selected_feature_indexes)
     array([ 0, 1, 2, 5, 9])
     >>> # call transform() on X to filter it down to selected features
     >>> X_filtered = feat_selector.transform(X)
     """
 
-    SUPPORTED_REG_ESTIMATORS = ["lasso"]
-    SUPPORTED_CLS_ESTIMATORS = ["lasso", "lr", "svm"]
+    SUPPORT = {
+        "classification": ["lasso", "lr", "svm"],
+        "regression": ["lasso"]
+    }
 
     def __init__(self, problem="classification", estimator="lasso", estimator_paras=None, threshold=None, norm_order=1, max_features=None):
         super().__init__(problem)
-        self.estimator = self.set_estimator(estimator, estimator_paras)
+        self.estimator = self._set_estimator(estimator, estimator_paras)
         self.threshold = threshold
         self.norm_order = norm_order
         self.max_features = max_features
         self.selector = SelectFromModel(estimator=self.estimator, threshold=self.threshold, prefit=False,
                                         norm_order=self.norm_order, max_features=self.max_features)
 
-    def set_estimator(self, estimator=None, paras=None):
+    def _set_estimator(self, estimator=None, paras=None):
         if type(estimator) is str:
-            estimator_name = validator.check_str("estimator", estimator, self.SUPPORTED_CLS_ESTIMATORS + self.SUPPORTED_REG_ESTIMATORS)
+            estimator_name = validator.check_str("estimator", estimator, self.SUPPORT[self.problem])
             return get_lasso_based_estimator(self.problem, estimator_name, paras)
         else:
             raise TypeError("Estimator should be a string.")
 
     def fit(self, X, y=None):
         self.selector.fit(X, y)
         self.selected_feature_masks = self.selector.get_support()
```

### Comparing `mafese-0.1.5/mafese/embedded/tree.py` & `mafese-0.1.6/mafese/embedded/tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,15 @@
           features allowed by using the output of `max_feaures(X)`.
         - If `None`, then all features are kept.
 
         To only select based on ``max_features``, set ``threshold=-np.inf``.
 
     Examples
     --------
-    The following example shows how to retrieve the most informative features in the Lasso-based FS method
+    The following example shows how to retrieve the most informative features in the Tree-based FS method
 
     >>> import pandas as pd
     >>> from mafese.embedded.tree import TreeSelector
     >>> # load dataset
     >>> dataset = pd.read_csv('your_path/dataset.csv', index_col=0).values
     >>> X, y = dataset[:, 0:-1], dataset[:, -1]     # Assumption that the last column is label column
     >>> # define mafese feature selection method
@@ -74,29 +74,29 @@
     >>> # check the index of selected features
     >>> print(feat_selector.selected_feature_indexes)
     array([ 0, 1, 2, 5, 9])
     >>> # call transform() on X to filter it down to selected features
     >>> X_filtered = feat_selector.transform(X)
     """
 
-    SUPPORTED_ESTIMATORS = ["rf", "adaboost", "xgb", "tree"]
+    SUPPORTED = ["rf", "adaboost", "xgb", "tree"]
 
     def __init__(self, problem="classification", estimator="tree", estimator_paras=None, threshold=None, norm_order=1, max_features=None):
         super().__init__(problem)
-        self.estimator = self.set_estimator(estimator, estimator_paras)
+        self.estimator = self._set_estimator(estimator, estimator_paras)
         self.estimator_paras = estimator_paras
         self.threshold = threshold
         self.norm_order = norm_order
         self.max_features = max_features
         self.selector = SelectFromModel(estimator=self.estimator, threshold=self.threshold, prefit=False,
                                         norm_order=self.norm_order, max_features=self.max_features)
 
-    def set_estimator(self, estimator=None, paras=None):
+    def _set_estimator(self, estimator=None, paras=None):
         if type(estimator) is str:
-            estimator_name = validator.check_str("estimator", estimator, self.SUPPORTED_ESTIMATORS)
+            estimator_name = validator.check_str("estimator", estimator, self.SUPPORTED)
             return get_tree_based_estimator(self.problem, estimator_name, paras)
         else:
             raise TypeError("Estimator should be a string.")
 
     def fit(self, X, y=None):
         self.selector.fit(X, y)
         self.selected_feature_masks = self.selector.get_support()
```

### Comparing `mafese-0.1.5/mafese/filter.py` & `mafese-0.1.6/mafese/filter.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,33 +72,35 @@
     >>> # check the index of selected features
     >>> print(feat_selector.selected_feature_indexes)
     array([ 0, 1, 2, 5, 9])
     >>> # call transform() on X to filter it down to selected features
     >>> X_filtered = feat_selector.transform(X)
     """
 
+    SUPPORT = {
+        "classification": {"CHI": "chi2", "ANOVA": "f_classif", "MI": "mutual_info_classif",
+                            "KENDALL": "kendall_func", "SPEARMAN": "spearman_func", "POINT": "point_func"},
+        "regression": {"PEARSON": "r_regression", "ANOVA": "f_regression", "MI": "mutual_info_regression",
+                        "KENDALL": "kendall_func", "SPEARMAN": "spearman_func", "POINT": "point_func"}
+    }
+
     def __init__(self, problem="classification", method="ANOVA", n_features=3):
         super().__init__(problem)
-        if self.problem == "classification":
-            self.supported_methods = {"CHI": "chi2", "ANOVA": "f_classif", "MI": "mutual_info_classif",
-                                      "KENDALL": "kendall_func", "SPEARMAN": "spearman_func", "POINT": "point_func"}
-        else:
-            self.supported_methods = {"PEARSON": "r_regression", "ANOVA": "f_regression", "MI": "mutual_info_regression",
-                                      "KENDALL": "kendall_func", "SPEARMAN": "spearman_func", "POINT": "point_func"}
-        self.method = self.set_method(method)
-        self.set_selector(n_features)
+        self.supported_methods = self.SUPPORT[self.problem]
+        self.method = self._set_method(method)
+        self._set_selector(n_features)
 
-    def set_method(self, method=None):
+    def _set_method(self, method=None):
         if type(method) is str:
             method_name = validator.check_str("method", method, list(self.supported_methods.keys()))
             return getattr(correlation, self.supported_methods[method_name])
         else:
             raise TypeError(f"Your method needs to be a string.")
 
-    def set_selector(self, n_features):
+    def _set_selector(self, n_features):
         self.n_features = n_features
         if type(n_features) is int:
             self.selector = correlation.SelectKBest(score_func=self.method, k=n_features)
         elif type(n_features) is float and 0 < n_features < 1:
             self.selector = correlation.SelectPercentile(score_func=self.method, percentile=self.n_features*100)
         else:
             raise TypeError(f"Type of n_features parameter is int or float. If int, 1 <= n_features <= max_features. If float, 0 < n_features < 1")
```

### Comparing `mafese-0.1.5/mafese/unsupervised.py` & `mafese-0.1.6/mafese/unsupervised.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,31 +57,31 @@
     >>> # check the index of selected features
     >>> print(feat_selector.selected_feature_indexes)
     array([ 0, 1, 2, 5, 9])
     >>> # call transform() on X to filter it down to selected features
     >>> X_filtered = feat_selector.transform(X)
     """
 
-    SUPPORTED_METHODS = {
+    SUPPORT = {
         "VAR": "Variance Threshold",
         "DR": "Dispersion Ratio",
         "MAD": "Mean Absolute Difference",
         "MCL": "Multicollinearity",
     }
 
     def __init__(self, problem="classification", method="MCL", n_features=None, threshold=10):
         super().__init__(problem)
-        self.method = self.set_method(method)
+        self.method = self._set_method(method)
         self.n_features = n_features
         self.threshold = threshold
         self.support_values = None
 
-    def set_method(self, method=None):
+    def _set_method(self, method=None):
         if type(method) is str:
-            return validator.check_str("method", method, list(self.SUPPORTED_METHODS.keys()))
+            return validator.check_str("method", method, list(self.SUPPORT.keys()))
         else:
             raise TypeError(f"Your method needs to be a string.")
 
     def transform(self, X):
         return X[:, self.selected_feature_indexes]
 
     def fit_transform(self, X, y=None, **fit_params):
```

### Comparing `mafese-0.1.5/mafese/utils/correlation.py` & `mafese-0.1.6/mafese/utils/correlation.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.5/mafese/utils/data_loader.py` & `mafese-0.1.6/mafese/utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.5/mafese/utils/encoder.py` & `mafese-0.1.6/mafese/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.5/mafese/utils/estimator.py` & `mafese-0.1.6/mafese/utils/estimator.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.5/mafese/utils/mealpy_util.py` & `mafese-0.1.6/mafese/utils/mealpy_util.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.5/mafese/utils/transfer.py` & `mafese-0.1.6/mafese/utils/transfer.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.5/mafese/utils/validator.py` & `mafese-0.1.6/mafese/utils/validator.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.5/mafese/wrapper/recursive.py` & `mafese-0.1.6/mafese/wrapper/recursive.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,33 +78,32 @@
     >>> # check the index of selected features
     >>> print(feat_selector.selected_feature_indexes)
     array([ 0, 1, 2, 5, 9])
     >>> # call transform() on X to filter it down to selected features
     >>> X_filtered = feat_selector.transform(X)
     """
 
-    SUPPORTED_ESTIMATORS = ["svm", "rf", "adaboost", "xgb", "tree"]
+    SUPPORT = ["svm", "rf", "adaboost", "xgb", "tree"]
 
     def __init__(self, problem="classification", estimator="knn", estimator_paras=None, n_features=3, step=1, verbose=0, importance_getter="auto"):
         super().__init__(problem)
-        self.estimator = self.set_estimator(estimator, estimator_paras)
+        self.estimator = self._set_estimator(estimator, estimator_paras)
         self.estimator_paras = estimator_paras
         self.n_features = n_features
         self.step = step
         self.verbose = verbose
         self.importance_getter = importance_getter
         self.selector = RFE(estimator=self.estimator, n_features_to_select=self.n_features,
                             step=self.step, verbose=self.verbose, importance_getter=self.importance_getter)
 
-    def set_estimator(self, estimator=None, paras=None):
+    def _set_estimator(self, estimator=None, paras=None):
         if type(estimator) is str:
-            estimator_name = validator.check_str("estimator", estimator, self.SUPPORTED_ESTIMATORS)
+            estimator_name = validator.check_str("estimator", estimator, self.SUPPORT)
             return get_recursive_estimator(self.problem, estimator_name, paras)
-        elif (hasattr(estimator, 'fit') and hasattr(estimator, 'predict')) and \
-                (callable(estimator.fit) and callable(estimator.predict)):
+        elif (hasattr(estimator, 'fit') and hasattr(estimator, 'predict')) and (callable(estimator.fit) and callable(estimator.predict)):
             return estimator
         else:
             raise NotImplementedError(f"Your estimator needs to implement at least 'fit' and 'predict' functions.")
 
     def fit(self, X, y=None):
         self.selector = self.selector.fit(X, y)
         self.selected_feature_masks = self.selector.support_.copy()
```

### Comparing `mafese-0.1.5/mafese/wrapper/sequential.py` & `mafese-0.1.6/mafese/wrapper/sequential.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,35 +93,34 @@
     >>> # check the index of selected features
     >>> print(feat_selector.selected_feature_indexes)
     array([ 0, 1, 2, 5, 9])
     >>> # call transform() on X to filter it down to selected features
     >>> X_filtered = feat_selector.transform(X)
     """
 
-    SUPPORTED_ESTIMATORS = ["knn", "svm", "rf", "adaboost", "xgb", "tree", "ann"]
+    SUPPORT = ["knn", "svm", "rf", "adaboost", "xgb", "tree", "ann"]
 
     def __init__(self, problem="classification", estimator="knn", estimator_paras=None, n_features=3,
                  direction="forward", tol=None, scoring=None, cv=5, n_jobs=None):
         super().__init__(problem)
-        self.estimator = self.set_estimator(estimator, estimator_paras)
+        self.estimator = self._set_estimator(estimator, estimator_paras)
         self.estimator_paras = estimator_paras
         self.n_features = n_features
         self.direction = direction
         self.tol = tol
         self.scoring = scoring
         self.cv = cv
         self.n_jobs = n_jobs
         self.selector = SFS(estimator=self.estimator, n_features_to_select=self.n_features, direction=self.direction)
 
-    def set_estimator(self, estimator=None, paras=None):
+    def _set_estimator(self, estimator=None, paras=None):
         if type(estimator) is str:
-            estimator_name = validator.check_str("estimator", estimator, self.SUPPORTED_ESTIMATORS)
+            estimator_name = validator.check_str("estimator", estimator, self.SUPPORT)
             return get_general_estimator(self.problem, estimator_name, paras)
-        elif (hasattr(estimator, 'fit') and hasattr(estimator, 'predict')) and \
-                (callable(estimator.fit) and callable(estimator.predict)):
+        elif (hasattr(estimator, 'fit') and hasattr(estimator, 'predict')) and (callable(estimator.fit) and callable(estimator.predict)):
             return estimator
         else:
             raise NotImplementedError(f"Your estimator needs to implement at least 'fit' and 'predict' functions.")
 
     def fit(self, X, y=None):
         self.selector = self.selector.fit(X, y)
         self.selected_feature_masks = self.selector.support_.copy()
```

### Comparing `mafese-0.1.5/mafese.egg-info/SOURCES.txt` & `mafese-0.1.6/mafese.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 CODE_OF_CONDUCT.md
 ChangeLog.md
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 mafese/__init__.py
-mafese/evaluator.py
 mafese/filter.py
 mafese/selector.py
 mafese/unsupervised.py
 mafese.egg-info/PKG-INFO
 mafese.egg-info/SOURCES.txt
 mafese.egg-info/dependency_links.txt
 mafese.egg-info/requires.txt
@@ -18,14 +17,15 @@
 mafese/embedded/lasso.py
 mafese/embedded/tree.py
 mafese/utils/__init__.py
 mafese/utils/correlation.py
 mafese/utils/data_loader.py
 mafese/utils/encoder.py
 mafese/utils/estimator.py
+mafese/utils/evaluator.py
 mafese/utils/mealpy_util.py
 mafese/utils/transfer.py
 mafese/utils/validator.py
 mafese/wrapper/__init__.py
 mafese/wrapper/mha.py
 mafese/wrapper/recursive.py
 mafese/wrapper/sequential.py
```

### Comparing `mafese-0.1.5/setup.py` & `mafese-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     with open('README.md', encoding='utf-8') as f:
         README = f.read()
     return README
 
 
 setup(
     name="mafese",
-    version="0.1.5",
+    version="0.1.6",
     author="Thieu",
     author_email="nguyenthieu2102@gmail.com",
     description="MAFESE: Metaheuristic Algorithm for Feature Selection - An Open Source Python Library",
     long_description=readme(),
     long_description_content_type="text/markdown",
     keywords=["engineering optimization problems", "mathematical optimization",
               "feature selection", "classification problem",
@@ -67,13 +67,14 @@
         "Topic :: Scientific/Engineering :: Bio-Informatics",
         "Topic :: Software Development :: Build Tools",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Utilities",
     ],
     install_requires=["numpy>=1.17.1", "scipy>=1.7.1", "scikit-learn>=1.0.2",
-                      "pandas>=1.3.5", "mealpy>=2.5.3", "permetrics>=1.3.3"],
+                      "pandas>=1.3.5", "mealpy>=2.5.3", "permetrics>=1.3.3",
+                      "plotly>=5.10.0", "kaleido>=0.2.1"],
     extras_require={
         "dev": ["pytest>=7.0", "pytest-cov==4.0.0", "flake8>=4.0.1"],
     },
     python_requires='>=3.7',
 )
```

### Comparing `mafese-0.1.5/tests/test_embedded.py` & `mafese-0.1.6/tests/test_embedded.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.5/tests/test_filter.py` & `mafese-0.1.6/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.5/tests/test_unsupervised.py` & `mafese-0.1.6/tests/test_unsupervised.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.5/tests/test_wrapper.py` & `mafese-0.1.6/tests/test_wrapper.py`

 * *Files identical despite different names*

