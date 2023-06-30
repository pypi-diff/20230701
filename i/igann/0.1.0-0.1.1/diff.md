# Comparing `tmp/igann-0.1.0.tar.gz` & `tmp/igann-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igann-0.1.0.tar", last modified: Fri Jun 30 20:37:49 2023, max compression
+gzip compressed data, was "igann-0.1.1.tar", last modified: Fri Jun 30 21:59:26 2023, max compression
```

## Comparing `igann-0.1.0.tar` & `igann-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 makraus   (1000) makraus   (1000)        0 2023-06-30 20:37:49.863980 igann-0.1.0/
--rw-rw-r--   0 makraus   (1000) makraus   (1000)     1069 2023-06-30 20:26:12.000000 igann-0.1.0/LICENSE
--rw-rw-r--   0 makraus   (1000) makraus   (1000)     5464 2023-06-30 20:37:49.863980 igann-0.1.0/PKG-INFO
--rw-rw-r--   0 makraus   (1000) makraus   (1000)     5142 2023-06-30 20:26:12.000000 igann-0.1.0/README.md
-drwxrwxr-x   0 makraus   (1000) makraus   (1000)        0 2023-06-30 20:37:49.863980 igann-0.1.0/igann/
--rw-rw-r--   0 makraus   (1000) makraus   (1000)       57 2023-06-30 20:26:12.000000 igann-0.1.0/igann/__init__.py
--rw-rw-r--   0 makraus   (1000) makraus   (1000)    53255 2023-06-30 20:26:12.000000 igann-0.1.0/igann/igann.py
-drwxrwxr-x   0 makraus   (1000) makraus   (1000)        0 2023-06-30 20:37:49.863980 igann-0.1.0/igann.egg-info/
--rw-rw-r--   0 makraus   (1000) makraus   (1000)     5464 2023-06-30 20:37:49.000000 igann-0.1.0/igann.egg-info/PKG-INFO
--rw-rw-r--   0 makraus   (1000) makraus   (1000)      231 2023-06-30 20:37:49.000000 igann-0.1.0/igann.egg-info/SOURCES.txt
--rw-rw-r--   0 makraus   (1000) makraus   (1000)        1 2023-06-30 20:37:49.000000 igann-0.1.0/igann.egg-info/dependency_links.txt
--rw-rw-r--   0 makraus   (1000) makraus   (1000)        1 2023-06-30 20:32:10.000000 igann-0.1.0/igann.egg-info/not-zip-safe
--rw-rw-r--   0 makraus   (1000) makraus   (1000)       71 2023-06-30 20:37:49.000000 igann-0.1.0/igann.egg-info/requires.txt
--rw-rw-r--   0 makraus   (1000) makraus   (1000)        6 2023-06-30 20:37:49.000000 igann-0.1.0/igann.egg-info/top_level.txt
--rw-rw-r--   0 makraus   (1000) makraus   (1000)       38 2023-06-30 20:37:49.863980 igann-0.1.0/setup.cfg
--rw-rw-r--   0 makraus   (1000) makraus   (1000)      714 2023-06-30 20:36:45.000000 igann-0.1.0/setup.py
+drwxrwxr-x   0 makraus   (1000) makraus   (1000)        0 2023-06-30 21:59:26.923055 igann-0.1.1/
+-rw-rw-r--   0 makraus   (1000) makraus   (1000)     1069 2023-06-30 21:54:58.000000 igann-0.1.1/LICENSE
+-rw-rw-r--   0 makraus   (1000) makraus   (1000)     5513 2023-06-30 21:59:26.923055 igann-0.1.1/PKG-INFO
+-rw-rw-r--   0 makraus   (1000) makraus   (1000)     5191 2023-06-30 21:54:58.000000 igann-0.1.1/README.md
+drwxrwxr-x   0 makraus   (1000) makraus   (1000)        0 2023-06-30 21:59:26.923055 igann-0.1.1/igann/
+-rw-rw-r--   0 makraus   (1000) makraus   (1000)       57 2023-06-30 21:54:58.000000 igann-0.1.1/igann/__init__.py
+-rw-rw-r--   0 makraus   (1000) makraus   (1000)    53282 2023-06-30 21:54:58.000000 igann-0.1.1/igann/igann.py
+drwxrwxr-x   0 makraus   (1000) makraus   (1000)        0 2023-06-30 21:59:26.923055 igann-0.1.1/igann.egg-info/
+-rw-rw-r--   0 makraus   (1000) makraus   (1000)     5513 2023-06-30 21:59:26.000000 igann-0.1.1/igann.egg-info/PKG-INFO
+-rw-rw-r--   0 makraus   (1000) makraus   (1000)      231 2023-06-30 21:59:26.000000 igann-0.1.1/igann.egg-info/SOURCES.txt
+-rw-rw-r--   0 makraus   (1000) makraus   (1000)        1 2023-06-30 21:59:26.000000 igann-0.1.1/igann.egg-info/dependency_links.txt
+-rw-rw-r--   0 makraus   (1000) makraus   (1000)        1 2023-06-30 21:55:11.000000 igann-0.1.1/igann.egg-info/not-zip-safe
+-rw-rw-r--   0 makraus   (1000) makraus   (1000)       71 2023-06-30 21:59:26.000000 igann-0.1.1/igann.egg-info/requires.txt
+-rw-rw-r--   0 makraus   (1000) makraus   (1000)        6 2023-06-30 21:59:26.000000 igann-0.1.1/igann.egg-info/top_level.txt
+-rw-rw-r--   0 makraus   (1000) makraus   (1000)       38 2023-06-30 21:59:26.923055 igann-0.1.1/setup.cfg
+-rw-rw-r--   0 makraus   (1000) makraus   (1000)      714 2023-06-30 21:58:11.000000 igann-0.1.1/setup.py
```

### Comparing `igann-0.1.0/LICENSE` & `igann-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `igann-0.1.0/PKG-INFO` & `igann-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igann
-Version: 0.1.0
+Version: 0.1.1
 Summary: Implementation of Interpretable Generalized Additive Neural Networks
 Home-page: https://github.com/MathiasKraus/igann
 Author: Mathias Kraus
 Author-email: mathias.sebastian.kraus@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -67,14 +67,15 @@
 - verbose: verbosity level. Can be 0 for no information, 1 for printing losses, and 2 for plotting shape functions every 5 iterations.
 
 ## Examples
 ### Basic regression example
 
 In the following, we use the common diabetes dataset from sklearn (https://scikit-learn.org/0.16/modules/generated/sklearn.datasets.load_diabetes.html). After loading the dataset via
 
+
 ```
 X, y = load_diabetes(return_X_y=True, as_frame=True)
 scaler = StandardScaler()
 X_names = X.columns
 
 X = scaler.fit_transform(X)
 X = pd.DataFrame(X, columns=X_names)
@@ -84,14 +85,15 @@
 
 ```
 y = (y - y.mean()) / y.std()
 ```
 
 we can simply initialize and fit IGANN with
 ```
+from igann import IGANN
 model = IGANN(task='regression')
 model.fit(X, y)
 ```
 
 With 
 ```
 model.plot_single(plot_by_list=['age', 'bmi', 'bp', 'sex', 's1', 's2'])
@@ -102,14 +104,15 @@
 
 
 ### Sparse regression example
 
 In many cases, it makes sense to train a sparse IGANN model, i.e., a model which only basis its output on few features. This generally increases the ease of understanding the model behavior.
 
 ```
+from igann import IGANN
 model = IGANN(task='regression', sparse=5)
 model.fit(X, y)
 model.plot_single()
 ```
 
 yields (note that the sparse parameters denotes the max number of features)
```

### Comparing `igann-0.1.0/README.md` & `igann-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 - verbose: verbosity level. Can be 0 for no information, 1 for printing losses, and 2 for plotting shape functions every 5 iterations.
 
 ## Examples
 ### Basic regression example
 
 In the following, we use the common diabetes dataset from sklearn (https://scikit-learn.org/0.16/modules/generated/sklearn.datasets.load_diabetes.html). After loading the dataset via
 
+
 ```
 X, y = load_diabetes(return_X_y=True, as_frame=True)
 scaler = StandardScaler()
 X_names = X.columns
 
 X = scaler.fit_transform(X)
 X = pd.DataFrame(X, columns=X_names)
@@ -73,14 +74,15 @@
 
 ```
 y = (y - y.mean()) / y.std()
 ```
 
 we can simply initialize and fit IGANN with
 ```
+from igann import IGANN
 model = IGANN(task='regression')
 model.fit(X, y)
 ```
 
 With 
 ```
 model.plot_single(plot_by_list=['age', 'bmi', 'bp', 'sex', 's1', 's2'])
@@ -91,14 +93,15 @@
 
 
 ### Sparse regression example
 
 In many cases, it makes sense to train a sparse IGANN model, i.e., a model which only basis its output on few features. This generally increases the ease of understanding the model behavior.
 
 ```
+from igann import IGANN
 model = IGANN(task='regression', sparse=5)
 model.fit(X, y)
 model.plot_single()
 ```
 
 yields (note that the sparse parameters denotes the max number of features)
```

### Comparing `igann-0.1.0/igann/igann.py` & `igann-0.1.1/igann/igann.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,15 +347,15 @@
         if fitted_dummies != None:
             self.get_dummies = fitted_dummies
             X = self._preprocess_feature_matrix(X, fit_dummies=False)
 
         else:
             X = self._preprocess_feature_matrix(X, fit_dummies=True)
 
-        if type(y) == pd.Series:
+        if type(y) == pd.Series or type(y) == pd.DataFrame:
             y = y.values
 
         y = torch.from_numpy(y.squeeze()).float()
 
         if self.task == 'classification':
             # In the case of targets in {0,1}, transform them to {-1,1} for optimization purposes
             if torch.min(y) != -1:
```

### Comparing `igann-0.1.0/igann.egg-info/PKG-INFO` & `igann-0.1.1/igann.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igann
-Version: 0.1.0
+Version: 0.1.1
 Summary: Implementation of Interpretable Generalized Additive Neural Networks
 Home-page: https://github.com/MathiasKraus/igann
 Author: Mathias Kraus
 Author-email: mathias.sebastian.kraus@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -67,14 +67,15 @@
 - verbose: verbosity level. Can be 0 for no information, 1 for printing losses, and 2 for plotting shape functions every 5 iterations.
 
 ## Examples
 ### Basic regression example
 
 In the following, we use the common diabetes dataset from sklearn (https://scikit-learn.org/0.16/modules/generated/sklearn.datasets.load_diabetes.html). After loading the dataset via
 
+
 ```
 X, y = load_diabetes(return_X_y=True, as_frame=True)
 scaler = StandardScaler()
 X_names = X.columns
 
 X = scaler.fit_transform(X)
 X = pd.DataFrame(X, columns=X_names)
@@ -84,14 +85,15 @@
 
 ```
 y = (y - y.mean()) / y.std()
 ```
 
 we can simply initialize and fit IGANN with
 ```
+from igann import IGANN
 model = IGANN(task='regression')
 model.fit(X, y)
 ```
 
 With 
 ```
 model.plot_single(plot_by_list=['age', 'bmi', 'bp', 'sex', 's1', 's2'])
@@ -102,14 +104,15 @@
 
 
 ### Sparse regression example
 
 In many cases, it makes sense to train a sparse IGANN model, i.e., a model which only basis its output on few features. This generally increases the ease of understanding the model behavior.
 
 ```
+from igann import IGANN
 model = IGANN(task='regression', sparse=5)
 model.fit(X, y)
 model.plot_single()
 ```
 
 yields (note that the sparse parameters denotes the max number of features)
```

### Comparing `igann-0.1.0/setup.py` & `igann-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='igann',
-    version='0.1.0',
+    version='0.1.1',
     author='Mathias Kraus',
     author_email='mathias.sebastian.kraus@gmail.com',
     description='Implementation of Interpretable Generalized Additive Neural Networks',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/MathiasKraus/igann',
     license='MIT',
```

