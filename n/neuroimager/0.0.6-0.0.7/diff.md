# Comparing `tmp/neuroimager-0.0.6.tar.gz` & `tmp/neuroimager-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroimager-0.0.6.tar", last modified: Sat Jun 10 10:19:01 2023, max compression
+gzip compressed data, was "neuroimager-0.0.7.tar", last modified: Sat Jul  1 04:32:47 2023, max compression
```

## Comparing `neuroimager-0.0.6.tar` & `neuroimager-0.0.7.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:19:01.428394 neuroimager-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-10 10:18:45.000000 neuroimager-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-10 10:19:01.428394 neuroimager-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-10 10:18:45.000000 neuroimager-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:19:01.424394 neuroimager-0.0.6/neuroimager/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-10 10:18:45.000000 neuroimager-0.0.6/neuroimager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:19:01.428394 neuroimager-0.0.6/neuroimager/pipes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 10:18:45.000000 neuroimager-0.0.6/neuroimager/pipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-10 10:18:45.000000 neuroimager-0.0.6/neuroimager/pipes/bipartite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-10 10:18:45.000000 neuroimager-0.0.6/neuroimager/pipes/brainage.py
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-06-10 10:18:45.000000 neuroimager-0.0.6/neuroimager/pipes/cca.py
--rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-06-10 10:18:45.000000 neuroimager-0.0.6/neuroimager/pipes/hmm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:19:01.428394 neuroimager-0.0.6/neuroimager/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-10 10:18:45.000000 neuroimager-0.0.6/neuroimager/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-10 10:18:45.000000 neuroimager-0.0.6/neuroimager/plotting/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:19:01.428394 neuroimager-0.0.6/neuroimager/stats/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-10 10:18:45.000000 neuroimager-0.0.6/neuroimager/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-06-10 10:18:45.000000 neuroimager-0.0.6/neuroimager/stats/correlation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:19:01.428394 neuroimager-0.0.6/neuroimager/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-10 10:18:45.000000 neuroimager-0.0.6/neuroimager/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9900 2023-06-10 10:18:45.000000 neuroimager-0.0.6/neuroimager/utils/atlas.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-10 10:18:45.000000 neuroimager-0.0.6/neuroimager/utils/fc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 10:19:01.424394 neuroimager-0.0.6/neuroimager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-10 10:19:01.000000 neuroimager-0.0.6/neuroimager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-10 10:19:01.000000 neuroimager-0.0.6/neuroimager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 10:19:01.000000 neuroimager-0.0.6/neuroimager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-10 10:19:01.000000 neuroimager-0.0.6/neuroimager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-10 10:19:01.000000 neuroimager-0.0.6/neuroimager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 10:19:01.428394 neuroimager-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-10 10:18:45.000000 neuroimager-0.0.6/setup.py
+drwxr-xr-x   0 nij       (1000) nij       (1000)        0 2023-07-01 04:32:47.119986 neuroimager-0.0.7/
+-rw-r--r--   0 nij       (1000) nij       (1000)    35149 2023-06-05 13:40:29.000000 neuroimager-0.0.7/LICENSE
+-rw-r--r--   0 nij       (1000) nij       (1000)     2458 2023-07-01 04:32:47.119986 neuroimager-0.0.7/PKG-INFO
+-rw-r--r--   0 nij       (1000) nij       (1000)     1832 2023-07-01 04:30:46.000000 neuroimager-0.0.7/README.md
+drwxr-xr-x   0 nij       (1000) nij       (1000)        0 2023-07-01 04:32:47.117986 neuroimager-0.0.7/neuroimager/
+-rw-r--r--   0 nij       (1000) nij       (1000)      149 2023-06-05 13:02:03.000000 neuroimager-0.0.7/neuroimager/__init__.py
+drwxr-xr-x   0 nij       (1000) nij       (1000)        0 2023-07-01 04:32:47.117986 neuroimager-0.0.7/neuroimager/pipes/
+-rw-r--r--   0 nij       (1000) nij       (1000)        0 2023-06-05 13:00:13.000000 neuroimager-0.0.7/neuroimager/pipes/__init__.py
+-rw-r--r--   0 nij       (1000) nij       (1000)     3188 2023-06-10 05:11:31.000000 neuroimager-0.0.7/neuroimager/pipes/bipartite.py
+-rw-r--r--   0 nij       (1000) nij       (1000)     1400 2023-06-13 06:38:35.000000 neuroimager-0.0.7/neuroimager/pipes/brainage.py
+-rw-r--r--   0 nij       (1000) nij       (1000)     7097 2023-06-08 17:19:10.000000 neuroimager-0.0.7/neuroimager/pipes/cca.py
+-rw-r--r--   0 nij       (1000) nij       (1000)    15711 2023-06-13 06:49:44.000000 neuroimager-0.0.7/neuroimager/pipes/explore.py
+-rw-r--r--   0 nij       (1000) nij       (1000)    39138 2023-07-01 03:39:37.000000 neuroimager-0.0.7/neuroimager/pipes/hmm.py
+drwxr-xr-x   0 nij       (1000) nij       (1000)        0 2023-07-01 04:32:47.118986 neuroimager-0.0.7/neuroimager/plotting/
+-rw-r--r--   0 nij       (1000) nij       (1000)      338 2023-06-30 10:01:02.000000 neuroimager-0.0.7/neuroimager/plotting/__init__.py
+-rw-r--r--   0 nij       (1000) nij       (1000)     4034 2023-06-30 09:51:04.000000 neuroimager-0.0.7/neuroimager/plotting/plot.py
+-rw-r--r--   0 nij       (1000) nij       (1000)      786 2023-06-30 13:44:07.000000 neuroimager-0.0.7/neuroimager/plotting/styler.py
+drwxr-xr-x   0 nij       (1000) nij       (1000)        0 2023-07-01 04:32:47.118986 neuroimager-0.0.7/neuroimager/stats/
+-rw-r--r--   0 nij       (1000) nij       (1000)      159 2023-06-13 07:01:27.000000 neuroimager-0.0.7/neuroimager/stats/__init__.py
+-rw-r--r--   0 nij       (1000) nij       (1000)     5558 2023-06-09 10:11:35.000000 neuroimager-0.0.7/neuroimager/stats/correlation.py
+-rw-r--r--   0 nij       (1000) nij       (1000)     1715 2023-06-13 06:59:17.000000 neuroimager-0.0.7/neuroimager/stats/perm_ttest.py
+drwxr-xr-x   0 nij       (1000) nij       (1000)        0 2023-07-01 04:32:47.118986 neuroimager-0.0.7/neuroimager/utils/
+-rw-r--r--   0 nij       (1000) nij       (1000)      560 2023-06-09 06:04:17.000000 neuroimager-0.0.7/neuroimager/utils/__init__.py
+-rw-r--r--   0 nij       (1000) nij       (1000)     9900 2023-06-09 14:51:06.000000 neuroimager-0.0.7/neuroimager/utils/atlas.py
+-rw-r--r--   0 nij       (1000) nij       (1000)     6704 2023-06-09 10:11:35.000000 neuroimager-0.0.7/neuroimager/utils/fc.py
+drwxr-xr-x   0 nij       (1000) nij       (1000)        0 2023-07-01 04:32:47.117986 neuroimager-0.0.7/neuroimager.egg-info/
+-rw-r--r--   0 nij       (1000) nij       (1000)     2458 2023-07-01 04:32:47.000000 neuroimager-0.0.7/neuroimager.egg-info/PKG-INFO
+-rw-r--r--   0 nij       (1000) nij       (1000)      663 2023-07-01 04:32:47.000000 neuroimager-0.0.7/neuroimager.egg-info/SOURCES.txt
+-rw-r--r--   0 nij       (1000) nij       (1000)        1 2023-07-01 04:32:47.000000 neuroimager-0.0.7/neuroimager.egg-info/dependency_links.txt
+-rw-r--r--   0 nij       (1000) nij       (1000)      110 2023-07-01 04:32:47.000000 neuroimager-0.0.7/neuroimager.egg-info/requires.txt
+-rw-r--r--   0 nij       (1000) nij       (1000)       12 2023-07-01 04:32:47.000000 neuroimager-0.0.7/neuroimager.egg-info/top_level.txt
+-rw-r--r--   0 nij       (1000) nij       (1000)       38 2023-07-01 04:32:47.119986 neuroimager-0.0.7/setup.cfg
+-rw-r--r--   0 nij       (1000) nij       (1000)     1241 2023-07-01 04:32:00.000000 neuroimager-0.0.7/setup.py
```

### Comparing `neuroimager-0.0.6/LICENSE` & `neuroimager-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.6/PKG-INFO` & `neuroimager-0.0.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuroimager
-Version: 0.0.6
+Version: 0.0.7
 Summary: A collection of utilities used for MRI data analysis
 Home-page: https://github.com/Wetiqe/neuroimager
 Author: Wetiqe
 Author-email: jzni132134@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -15,15 +15,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # neuroimager
 
 A collection of utilities used for MRI data analysis
 
+# Automatic Analysis of HMM model estimated by HMM-MAR
 
+To be done
 
 # Atlas Operation
 Suggest you have two probability atlas:
 ```python
 from nilearn import plotting
 import nibabel as nib
 import os
```

### Comparing `neuroimager-0.0.6/README.md` & `neuroimager-0.0.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # neuroimager
 
 A collection of utilities used for MRI data analysis
 
+# Automatic Analysis of HMM model estimated by HMM-MAR
 
+To be done
 
 # Atlas Operation
 Suggest you have two probability atlas:
 ```python
 from nilearn import plotting
 import nibabel as nib
 import os
```

### Comparing `neuroimager-0.0.6/neuroimager/pipes/bipartite.py` & `neuroimager-0.0.7/neuroimager/pipes/bipartite.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.6/neuroimager/pipes/brainage.py` & `neuroimager-0.0.7/neuroimager/pipes/brainage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import numpy as np
 from sklearn.linear_model import LinearRegression
 from sklearn.preprocessing import PolynomialFeatures
 
 
-def BAG(train_pred, test_pred, train_y, test_y):
+def BAG(train_pred, test_pred, train_y, test_y, line_reg_order=1):
     """
     Brain Age Gap Correction
 
     Parameters:
-    train_pred (numpy array): Predicted age on the training set.
-    test_pred (numpy array): Predicted age on the test set.
-    train_y (numpy array): Actual age in the training set.
-    test_y (numpy array): Actual age in the test set.
+    train_pred (1D numpy array): Predicted age on the training set.
+    test_pred (1D numpy array): Predicted age on the test set.
+    train_y (1D numpy array): Actual age in the training set.
+    test_y (1D numpy array): Actual age in the test set.
 
     Returns:
     corrected_age (numpy array): Corrected predicted age on the test set.
     train_delta_age (numpy array): Difference between predicted and actual age on the training set.
     line_reg (LinearRegression object): Trained regression model.
+
+    References:
+    Bias-adjustment in neuroimaging-based brain age frameworks: A robust scheme
     """
 
     line_reg = LinearRegression()
-    poly = PolynomialFeatures(degree=1, include_bias=True)
+    poly = PolynomialFeatures(degree=line_reg_order, include_bias=True)
     line_reg_features = poly.fit_transform(train_y.reshape(-1, 1))
-    line_reg.fit(line_reg_features, train_pred.reshape(-1, 1))
-
+    offset_train = train_pred - train_y
+    line_reg.fit(line_reg_features, offset_train.reshape(-1, 1))
     test_features = poly.transform(test_y.reshape(-1, 1))
-    corrected_delta_age = (
-        test_pred - np.array(line_reg.predict(test_features)).flatten()
-    )
-    corrected_age = test_y + corrected_delta_age
-
+    offset_test = np.array(line_reg.predict(test_features)).flatten()
+    corrected_age = test_pred - offset_test
+    corrected_delta_age = corrected_age - test_y
     return corrected_age, corrected_delta_age
```

### Comparing `neuroimager-0.0.6/neuroimager/pipes/cca.py` & `neuroimager-0.0.7/neuroimager/pipes/cca.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.6/neuroimager/plotting/plot.py` & `neuroimager-0.0.7/neuroimager/plotting/plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,13 @@
 import numpy as np
 from matplotlib import pyplot as plt
 import seaborn as sns
 from scipy.stats import gaussian_kde
 
 
-def update_matplotlib_fontsize():
-    parameters = {
-        "axes.labelsize": 20,
-        "axes.titlesize": 20,
-        "figure.titlesize": 20,
-        "xtick.labelsize": 20,
-        "ytick.labelsize": 20,
-        "legend.fontsize": 15,
-        "legend.title_fontsize": 16,
-        "axes.titleweight": "bold",
-        "axes.labelweight": "bold",
-        "figure.titleweight": "bold",
-        "font.weight": "bold",
-        "font.sans-serif": "Arial",
-    }
-    plt.rcParams.update(parameters)
-
-
 def get_sig(sig):
     symbol = ""
     if 0.01 < sig < 0.05:
         symbol = "*"
     elif 0.001 < sig <= 0.01:
         symbol = "**"
     elif sig <= 0.001:
```

### Comparing `neuroimager-0.0.6/neuroimager/stats/correlation.py` & `neuroimager-0.0.7/neuroimager/stats/correlation.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.6/neuroimager/utils/__init__.py` & `neuroimager-0.0.7/neuroimager/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.6/neuroimager/utils/atlas.py` & `neuroimager-0.0.7/neuroimager/utils/atlas.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.6/neuroimager/utils/fc.py` & `neuroimager-0.0.7/neuroimager/utils/fc.py`

 * *Files identical despite different names*

### Comparing `neuroimager-0.0.6/neuroimager.egg-info/PKG-INFO` & `neuroimager-0.0.7/neuroimager.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuroimager
-Version: 0.0.6
+Version: 0.0.7
 Summary: A collection of utilities used for MRI data analysis
 Home-page: https://github.com/Wetiqe/neuroimager
 Author: Wetiqe
 Author-email: jzni132134@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -15,15 +15,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # neuroimager
 
 A collection of utilities used for MRI data analysis
 
+# Automatic Analysis of HMM model estimated by HMM-MAR
 
+To be done
 
 # Atlas Operation
 Suggest you have two probability atlas:
 ```python
 from nilearn import plotting
 import nibabel as nib
 import os
```

### Comparing `neuroimager-0.0.6/neuroimager.egg-info/SOURCES.txt` & `neuroimager-0.0.7/neuroimager.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 neuroimager.egg-info/dependency_links.txt
 neuroimager.egg-info/requires.txt
 neuroimager.egg-info/top_level.txt
 neuroimager/pipes/__init__.py
 neuroimager/pipes/bipartite.py
 neuroimager/pipes/brainage.py
 neuroimager/pipes/cca.py
+neuroimager/pipes/explore.py
 neuroimager/pipes/hmm.py
 neuroimager/plotting/__init__.py
 neuroimager/plotting/plot.py
+neuroimager/plotting/styler.py
 neuroimager/stats/__init__.py
 neuroimager/stats/correlation.py
+neuroimager/stats/perm_ttest.py
 neuroimager/utils/__init__.py
 neuroimager/utils/atlas.py
 neuroimager/utils/fc.py
```

### Comparing `neuroimager-0.0.6/setup.py` & `neuroimager-0.0.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 current_dir = os.path.abspath(os.path.dirname(__file__))
 # Read the contents of your README file
 with open(os.path.join(current_dir, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="neuroimager",
-    version="0.0.6",
+    version="0.0.7",
     description="A collection of utilities used for MRI data analysis",
     author="Wetiqe",
     author_email="jzni132134@gmail.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Wetiqe/neuroimager",
     packages=find_packages(),
@@ -22,14 +22,16 @@
         "pandas==1.5.3",
         "scipy==1.10.1",
         "pingouin",
         "seaborn",
         "sklearn",
         "nilearn",
         "networkx",
+        "munkres",
+        "scikit-network",
     ],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

