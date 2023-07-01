# Comparing `tmp/gecs-0.28.0.tar.gz` & `tmp/gecs-0.28.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gecs-0.28.0.tar", max compression
+gzip compressed data, was "gecs-0.28.1.tar", max compression
```

## Comparing `gecs-0.28.0.tar` & `gecs-0.28.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1060 2023-04-06 09:38:20.465352 gecs-0.28.0/LICENSE
--rw-r--r--   0        0        0     2041 2023-07-01 14:45:06.152875 gecs-0.28.0/README.md
--rw-r--r--   0        0        0      697 2023-07-01 13:58:58.563506 gecs-0.28.0/pyproject.toml
--rw-r--r--   0        0        0    43189 2023-07-01 14:46:26.156284 gecs-0.28.0/src/gecs/gec.py
--rw-r--r--   0        0        0     2112 2023-06-19 14:54:28.150721 gecs-0.28.0/src/gecs/utils/gaussian_process_visualisation.py
--rw-r--r--   0        0        0     3029 1970-01-01 00:00:00.000000 gecs-0.28.0/setup.py
--rw-r--r--   0        0        0     3005 1970-01-01 00:00:00.000000 gecs-0.28.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-06 09:38:20.465352 gecs-0.28.1/LICENSE
+-rw-r--r--   0        0        0     2041 2023-07-01 15:06:46.565047 gecs-0.28.1/README.md
+-rw-r--r--   0        0        0      697 2023-07-01 15:07:22.368832 gecs-0.28.1/pyproject.toml
+-rw-r--r--   0        0        0    43189 2023-07-01 14:46:26.156284 gecs-0.28.1/src/gecs/gec.py
+-rw-r--r--   0        0        0     2112 2023-06-19 14:54:28.150721 gecs-0.28.1/src/gecs/utils/gaussian_process_visualisation.py
+-rw-r--r--   0        0        0     3029 1970-01-01 00:00:00.000000 gecs-0.28.1/setup.py
+-rw-r--r--   0        0        0     3005 1970-01-01 00:00:00.000000 gecs-0.28.1/PKG-INFO
```

### Comparing `gecs-0.28.0/LICENSE` & `gecs-0.28.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gecs-0.28.0/README.md` & `gecs-0.28.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     from gecs.gec import GEC
 
     gec.fit(X, y)
 
     gec.serialize(path) # stores gec data and settings, but not underlying LGBMClassifier attributes
 
-    gec2 = GEC.deserialize(path, X, y) # X and z are necessary to fit the underlying LGBMClassifier
+    gec2 = GEC.deserialize(path, X, y) # X and y are necessary to fit the underlying LGBMClassifier
 
 
 ## Contributing
 
 If you want to contribute, please reach out and I'll design a process around it.
 
 ## License
```

### Comparing `gecs-0.28.0/pyproject.toml` & `gecs-0.28.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gecs"
-version = "0.28.0"
+version = "0.28.1"
 authors = ["Leon Luithlen <leontimnaluithlen@gmail.com>"]
 description = "LightGBM Classifier with integrated bayesian hyperparameter optimization"
 keywords = ["lightgbm", "classification", "machine learning", "hyperparameter optimization", "classifier"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/0xideas/sequifier"
 repository = "https://github.com/0xideas/sequifier"
```

### Comparing `gecs-0.28.0/src/gecs/gec.py` & `gecs-0.28.1/src/gecs/gec.py`

 * *Files identical despite different names*

### Comparing `gecs-0.28.0/src/gecs/utils/gaussian_process_visualisation.py` & `gecs-0.28.1/src/gecs/utils/gaussian_process_visualisation.py`

 * *Files identical despite different names*

### Comparing `gecs-0.28.0/setup.py` & `gecs-0.28.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,17 +20,17 @@
  'scikit-learn==1.2.2',
  'scipy==1.10.1',
  'tqdm==4.65.0',
  'typer==0.9.0']
 
 setup_kwargs = {
     'name': 'gecs',
-    'version': '0.28.0',
+    'version': '0.28.1',
     'description': 'LightGBM Classifier with integrated bayesian hyperparameter optimization',
-    'long_description': "![a gecko looking at the camera with bayesian math in white on a pink and green background](documentation/assets/header.png)\n\n\n# (100)gecs\n\nBayesian hyperparameter tuning for LGBMClassifier with a scikit-learn API\n\n## Table of Contents\n\n- [Project Overview](#project-overview)\n- [Installation](#installation)\n- [Usage](#usage)\n- [Contributing](#contributing)\n- [License](#license)\n\n## Project Overview\n\nThe package `gecs` provides the class `GEC`, which is a child class of the class `LGBMClassifier` from the package `lightgbm`. It can be imported from `gecs.gec` and then used in place of `LGBMClassifier`, with the same API. The difference to `LGBMClassifier` lies in the fact that `GEC`automatically does bayesian hyperparameter optimization of the parameters `learning_rate`, `reg_alpha`, `reg_lambda`, `min_child_samples`, `min_child_weight`, `colsample_bytree` and optionally also of `num_leaves` and `n_estimators`.\n\nThe fit method has two new parameters: `n_iter`, which sets the number of hyperparameter combinations that will be tried (the higher `n_iter` the higher the expected accuracy, but at a cost of compute) and `fixed_hyperparameters`, which determines which hyperparameters of the LGBM classifier won't get optimized. By default, these are `n_estimators` and `num_leaves`, as the highest possible value for these hyperparameters is almost always optimal. The idea then is to set these as high as makes sense in a specific context and then optimize the other hyperparameters.\n\n\n## Installation\n\n    pip install gecs\n\n## Usage\n\n    from gecs.gec import GEC\n\n    gec.fit(X, y)\n\n    gec.serialize(path) # stores gec data and settings, but not underlying LGBMClassifier attributes\n\n    gec2 = GEC.deserialize(path, X, y) # X and z are necessary to fit the underlying LGBMClassifier\n\n\n## Contributing\n\nIf you want to contribute, please reach out and I'll design a process around it.\n\n## License\n\nMIT\n\n## Contact Information\n\nYou can find my contact information on my website: [https://leonluithlen.eu](https://leonluithlen.eu)",
+    'long_description': "![a gecko looking at the camera with bayesian math in white on a pink and green background](documentation/assets/header.png)\n\n\n# (100)gecs\n\nBayesian hyperparameter tuning for LGBMClassifier with a scikit-learn API\n\n## Table of Contents\n\n- [Project Overview](#project-overview)\n- [Installation](#installation)\n- [Usage](#usage)\n- [Contributing](#contributing)\n- [License](#license)\n\n## Project Overview\n\nThe package `gecs` provides the class `GEC`, which is a child class of the class `LGBMClassifier` from the package `lightgbm`. It can be imported from `gecs.gec` and then used in place of `LGBMClassifier`, with the same API. The difference to `LGBMClassifier` lies in the fact that `GEC`automatically does bayesian hyperparameter optimization of the parameters `learning_rate`, `reg_alpha`, `reg_lambda`, `min_child_samples`, `min_child_weight`, `colsample_bytree` and optionally also of `num_leaves` and `n_estimators`.\n\nThe fit method has two new parameters: `n_iter`, which sets the number of hyperparameter combinations that will be tried (the higher `n_iter` the higher the expected accuracy, but at a cost of compute) and `fixed_hyperparameters`, which determines which hyperparameters of the LGBM classifier won't get optimized. By default, these are `n_estimators` and `num_leaves`, as the highest possible value for these hyperparameters is almost always optimal. The idea then is to set these as high as makes sense in a specific context and then optimize the other hyperparameters.\n\n\n## Installation\n\n    pip install gecs\n\n## Usage\n\n    from gecs.gec import GEC\n\n    gec.fit(X, y)\n\n    gec.serialize(path) # stores gec data and settings, but not underlying LGBMClassifier attributes\n\n    gec2 = GEC.deserialize(path, X, y) # X and y are necessary to fit the underlying LGBMClassifier\n\n\n## Contributing\n\nIf you want to contribute, please reach out and I'll design a process around it.\n\n## License\n\nMIT\n\n## Contact Information\n\nYou can find my contact information on my website: [https://leonluithlen.eu](https://leonluithlen.eu)",
     'author': 'Leon Luithlen',
     'author_email': 'leontimnaluithlen@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/0xideas/sequifier',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `gecs-0.28.0/PKG-INFO` & `gecs-0.28.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gecs
-Version: 0.28.0
+Version: 0.28.1
 Summary: LightGBM Classifier with integrated bayesian hyperparameter optimization
 Home-page: https://github.com/0xideas/sequifier
 License: MIT
 Keywords: lightgbm,classification,machine learning,hyperparameter optimization,classifier
 Author: Leon Luithlen
 Author-email: leontimnaluithlen@gmail.com
 Requires-Python: >=3.10.0,<3.11.0
@@ -54,15 +54,15 @@
 
     from gecs.gec import GEC
 
     gec.fit(X, y)
 
     gec.serialize(path) # stores gec data and settings, but not underlying LGBMClassifier attributes
 
-    gec2 = GEC.deserialize(path, X, y) # X and z are necessary to fit the underlying LGBMClassifier
+    gec2 = GEC.deserialize(path, X, y) # X and y are necessary to fit the underlying LGBMClassifier
 
 
 ## Contributing
 
 If you want to contribute, please reach out and I'll design a process around it.
 
 ## License
```

