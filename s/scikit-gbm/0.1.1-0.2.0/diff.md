# Comparing `tmp/scikit-gbm-0.1.1.tar.gz` & `tmp/scikit-gbm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-gbm-0.1.1.tar", last modified: Sat Jun 17 20:01:29 2023, max compression
+gzip compressed data, was "scikit-gbm-0.2.0.tar", last modified: Sat Jul  1 16:19:34 2023, max compression
```

## Comparing `scikit-gbm-0.1.1.tar` & `scikit-gbm-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,41 @@
-drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-06-17 20:01:29.534784 scikit-gbm-0.1.1/
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     1077 2023-04-15 14:39:04.000000 scikit-gbm-0.1.1/LICENSE
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     2141 2023-06-17 20:01:29.534784 scikit-gbm-0.1.1/PKG-INFO
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     1594 2023-06-16 22:11:35.000000 scikit-gbm-0.1.1/README.md
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)      720 2023-06-17 20:00:24.000000 scikit-gbm-0.1.1/pyproject.toml
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)       97 2023-06-16 21:48:45.000000 scikit-gbm-0.1.1/requirements.txt
-drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-06-17 20:01:29.502785 scikit-gbm-0.1.1/scikit_gbm.egg-info/
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     2141 2023-06-17 20:01:29.000000 scikit-gbm-0.1.1/scikit_gbm.egg-info/PKG-INFO
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)      465 2023-06-17 20:01:29.000000 scikit-gbm-0.1.1/scikit_gbm.egg-info/SOURCES.txt
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)        1 2023-06-17 20:01:29.000000 scikit-gbm-0.1.1/scikit_gbm.egg-info/dependency_links.txt
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)       97 2023-06-17 20:01:29.000000 scikit-gbm-0.1.1/scikit_gbm.egg-info/requires.txt
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)        6 2023-06-17 20:01:29.000000 scikit-gbm-0.1.1/scikit_gbm.egg-info/top_level.txt
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)       38 2023-06-17 20:01:29.534784 scikit-gbm-0.1.1/setup.cfg
-drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-06-17 20:01:29.502785 scikit-gbm-0.1.1/skgbm/
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)       48 2023-06-09 20:23:00.000000 scikit-gbm-0.1.1/skgbm/__init__.py
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     4073 2023-06-10 20:23:41.000000 scikit-gbm-0.1.1/skgbm/base.py
-drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-06-17 20:01:29.502785 scikit-gbm-0.1.1/skgbm/preprocessing/
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)      126 2023-06-16 21:48:45.000000 scikit-gbm-0.1.1/skgbm/preprocessing/__init__.py
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     8592 2023-06-17 18:31:13.000000 scikit-gbm-0.1.1/skgbm/preprocessing/discretizer.py
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     3693 2023-06-17 18:06:40.000000 scikit-gbm-0.1.1/skgbm/preprocessing/featurizer.py
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     3662 2023-06-16 21:48:45.000000 scikit-gbm-0.1.1/skgbm/tools.py
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     5348 2023-06-09 20:23:00.000000 scikit-gbm-0.1.1/skgbm/tree.py
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     8165 2023-06-16 21:48:45.000000 scikit-gbm-0.1.1/skgbm/trees_extraction.py
-drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-06-17 20:01:29.518784 scikit-gbm-0.1.1/tests/
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     2587 2023-04-15 16:16:57.000000 scikit-gbm-0.1.1/tests/test_gbm_wrapper.py
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     1574 2023-06-09 20:23:00.000000 scikit-gbm-0.1.1/tests/test_trees_to_dataframe.py
+drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-07-01 16:19:34.605100 scikit-gbm-0.2.0/
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     1077 2023-04-15 14:39:04.000000 scikit-gbm-0.2.0/LICENSE
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     2150 2023-07-01 16:19:34.605100 scikit-gbm-0.2.0/PKG-INFO
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     1603 2023-06-20 21:46:26.000000 scikit-gbm-0.2.0/README.md
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)      720 2023-07-01 16:19:06.000000 scikit-gbm-0.2.0/pyproject.toml
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)       97 2023-06-16 21:48:45.000000 scikit-gbm-0.2.0/requirements.txt
+drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-07-01 16:19:34.585101 scikit-gbm-0.2.0/scikit_gbm.egg-info/
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     2150 2023-07-01 16:19:34.000000 scikit-gbm-0.2.0/scikit_gbm.egg-info/PKG-INFO
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)      775 2023-07-01 16:19:34.000000 scikit-gbm-0.2.0/scikit_gbm.egg-info/SOURCES.txt
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)        1 2023-07-01 16:19:34.000000 scikit-gbm-0.2.0/scikit_gbm.egg-info/dependency_links.txt
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)       97 2023-07-01 16:19:34.000000 scikit-gbm-0.2.0/scikit_gbm.egg-info/requires.txt
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)        6 2023-07-01 16:19:34.000000 scikit-gbm-0.2.0/scikit_gbm.egg-info/top_level.txt
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)       38 2023-07-01 16:19:34.605100 scikit-gbm-0.2.0/setup.cfg
+drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-07-01 16:19:34.585101 scikit-gbm-0.2.0/skgbm/
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)       48 2023-06-09 20:23:00.000000 scikit-gbm-0.2.0/skgbm/__init__.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     2289 2023-07-01 14:08:53.000000 scikit-gbm-0.2.0/skgbm/base.py
+drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-07-01 16:19:34.585101 scikit-gbm-0.2.0/skgbm/preprocessing/
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)      126 2023-06-16 21:48:45.000000 scikit-gbm-0.2.0/skgbm/preprocessing/__init__.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     8578 2023-07-01 14:08:53.000000 scikit-gbm-0.2.0/skgbm/preprocessing/discretizer.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     3679 2023-07-01 14:08:53.000000 scikit-gbm-0.2.0/skgbm/preprocessing/featurizer.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     3662 2023-06-16 21:48:45.000000 scikit-gbm-0.2.0/skgbm/tools.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     5348 2023-06-09 20:23:00.000000 scikit-gbm-0.2.0/skgbm/tree.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     8165 2023-06-16 21:48:45.000000 scikit-gbm-0.2.0/skgbm/trees_extraction.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     2999 2023-06-26 20:22:45.000000 scikit-gbm-0.2.0/skgbm/utils.py
+drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-07-01 16:19:34.585101 scikit-gbm-0.2.0/skgbm/viz/
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)      188 2023-06-26 20:51:11.000000 scikit-gbm-0.2.0/skgbm/viz/__init__.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     1964 2023-06-26 20:52:16.000000 scikit-gbm-0.2.0/skgbm/viz/axil.py
+drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-07-01 16:19:34.585101 scikit-gbm-0.2.0/skgbm/wrappers/
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)      895 2023-07-01 14:08:53.000000 scikit-gbm-0.2.0/skgbm/wrappers/__init__.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)      524 2023-07-01 14:08:53.000000 scikit-gbm-0.2.0/skgbm/wrappers/base_wrapper.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)      778 2023-07-01 14:08:53.000000 scikit-gbm-0.2.0/skgbm/wrappers/catboost_wrapper.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)      650 2023-07-01 14:08:53.000000 scikit-gbm-0.2.0/skgbm/wrappers/lightgbm_wrapper.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)      622 2023-07-01 14:08:53.000000 scikit-gbm-0.2.0/skgbm/wrappers/sklearn_wrapper.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     1241 2023-07-01 15:03:47.000000 scikit-gbm-0.2.0/skgbm/wrappers/xgboost_wrapper.py
+drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-07-01 16:19:34.585101 scikit-gbm-0.2.0/skgbm/xai/
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)      122 2023-06-20 21:46:26.000000 scikit-gbm-0.2.0/skgbm/xai/__init__.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     9995 2023-07-01 15:02:40.000000 scikit-gbm-0.2.0/skgbm/xai/axil.py
+drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-07-01 16:19:34.597101 scikit-gbm-0.2.0/tests/
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     2233 2023-07-01 14:08:53.000000 scikit-gbm-0.2.0/tests/test_axil.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     2587 2023-04-15 16:16:57.000000 scikit-gbm-0.2.0/tests/test_gbm_wrapper.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     1569 2023-06-20 21:46:26.000000 scikit-gbm-0.2.0/tests/test_trees_to_dataframe.py
```

### Comparing `scikit-gbm-0.1.1/LICENSE` & `scikit-gbm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-gbm-0.1.1/PKG-INFO` & `scikit-gbm-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-gbm
-Version: 0.1.1
+Version: 0.2.0
 Summary: scikit-learn compatible tools to work with GBM models
 Author-email: Krzysztof Joachimiak <joachimiak.krzysztof@gmail.com>
 Project-URL: Homepage, https://github.com/krzjoa/scikit-gbm
 Project-URL: Bug Tracker, https://github.com/krzjoa/scikit-gbm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,14 +32,15 @@
 ## Usage
 
 Fo the moment, you can find the following tools in the library:
 
 * `GBMFeaturizer`
 * `GBMDiscretizer`
 * `trees_to_dataframe`
+* `AXIL`
 
 Take a look at the [documentation](https://scikit-gbm.readthedocs.io/en/latest/?badge=latest) to learn more.
 A simple example, how to use `GBMFeaturizer` in a classification task.
 
 ```python
 
 # Classification
```

### Comparing `scikit-gbm-0.1.1/README.md` & `scikit-gbm-0.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 ## Usage
 
 Fo the moment, you can find the following tools in the library:
 
 * `GBMFeaturizer`
 * `GBMDiscretizer`
 * `trees_to_dataframe`
+* `AXIL`
 
 Take a look at the [documentation](https://scikit-gbm.readthedocs.io/en/latest/?badge=latest) to learn more.
 A simple example, how to use `GBMFeaturizer` in a classification task.
 
 ```python
 
 # Classification
```

### Comparing `scikit-gbm-0.1.1/pyproject.toml` & `scikit-gbm-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "scikit-gbm"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
   { name="Krzysztof Joachimiak", email="joachimiak.krzysztof@gmail.com" },
 ]
 description = "scikit-learn compatible tools to work with GBM models"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `scikit-gbm-0.1.1/scikit_gbm.egg-info/PKG-INFO` & `scikit-gbm-0.2.0/scikit_gbm.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-gbm
-Version: 0.1.1
+Version: 0.2.0
 Summary: scikit-learn compatible tools to work with GBM models
 Author-email: Krzysztof Joachimiak <joachimiak.krzysztof@gmail.com>
 Project-URL: Homepage, https://github.com/krzjoa/scikit-gbm
 Project-URL: Bug Tracker, https://github.com/krzjoa/scikit-gbm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,14 +32,15 @@
 ## Usage
 
 Fo the moment, you can find the following tools in the library:
 
 * `GBMFeaturizer`
 * `GBMDiscretizer`
 * `trees_to_dataframe`
+* `AXIL`
 
 Take a look at the [documentation](https://scikit-gbm.readthedocs.io/en/latest/?badge=latest) to learn more.
 A simple example, how to use `GBMFeaturizer` in a classification task.
 
 ```python
 
 # Classification
```

### Comparing `scikit-gbm-0.1.1/skgbm/preprocessing/discretizer.py` & `scikit-gbm-0.2.0/skgbm/preprocessing/discretizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import numpy as np
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.preprocessing import OneHotEncoder
 from sklearn.base import clone
 
 from feature_engine.discretisation import ArbitraryDiscretiser
 
-from ..base import GBMWrapper
+from ..base import GBM
 from ..tools import trees_to_dataframe
 from ..trees_extraction import _catboost_raw_trees, _catboost_get_splits
 
 try:
     import catboost
     CATBOOST_CLASSES = [
         catboost.CatBoostRegressor,
@@ -23,15 +23,15 @@
     ]
 except:
     # If there is no CatBoost, any CatBoost model can't be passed anyway
     CATBOOST_CLASSES = []
 
 
 
-class GBMDiscretizer(BaseEstimator, TransformerMixin, GBMWrapper):
+class GBMDiscretizer(BaseEstimator, TransformerMixin, GBM):
     """
     Feature discretizer based on GBDT.
     
     Internally, it uses `ArbitraryDiscretiser <https://feature-engine.trainindata.com/en/1.0.x/discretisation/ArbitraryDiscretiser.html>`_
     to handle discretization step after finding the optimal thresholds.
     
     Parameters
```

### Comparing `scikit-gbm-0.1.1/skgbm/preprocessing/featurizer.py` & `scikit-gbm-0.2.0/skgbm/preprocessing/featurizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import scipy
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.preprocessing import OneHotEncoder
 
-from ..base import GBMWrapper
+from ..base import GBM
 
 
-class GBMFeaturizer(BaseEstimator, TransformerMixin, GBMWrapper):
+class GBMFeaturizer(BaseEstimator, TransformerMixin, GBM):
     """
     Feature generator for any GBDT model.
     
     Parameters
     ----------
     estimator: object
         A gradient boosting model from scikit-learn, XGBoost, LightGBM or CatBoost library
```

### Comparing `scikit-gbm-0.1.1/skgbm/tools.py` & `scikit-gbm-0.2.0/skgbm/tools.py`

 * *Files identical despite different names*

### Comparing `scikit-gbm-0.1.1/skgbm/tree.py` & `scikit-gbm-0.2.0/skgbm/tree.py`

 * *Files identical despite different names*

### Comparing `scikit-gbm-0.1.1/skgbm/trees_extraction.py` & `scikit-gbm-0.2.0/skgbm/trees_extraction.py`

 * *Files identical despite different names*

### Comparing `scikit-gbm-0.1.1/tests/test_gbm_wrapper.py` & `scikit-gbm-0.2.0/tests/test_gbm_wrapper.py`

 * *Files identical despite different names*

### Comparing `scikit-gbm-0.1.1/tests/test_trees_to_dataframe.py` & `scikit-gbm-0.2.0/tests/test_trees_to_dataframe.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import pandas as pd
 from sklearn.datasets import make_classification, make_regression
 from sklearn.ensemble import GradientBoostingClassifier, GradientBoostingRegressor
 from xgboost import XGBClassifier, XGBRegressor, XGBRanker
 from lightgbm import LGBMClassifier, LGBMRegressor, LGBMRanker
 from catboost import CatBoostClassifier, CatBoostRegressor, CatBoostRanker
 
-from skgbm.functional import trees_to_dataframe
+from skgbm.tools import trees_to_dataframe
 
 make_classification = pytest.fixture(make_classification)
 make_regression = pytest.fixture(make_regression)
 
 
 def test_gbm_wrapper_classification(make_classification):
```

