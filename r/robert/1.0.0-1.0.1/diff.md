# Comparing `tmp/robert-1.0.0.tar.gz` & `tmp/robert-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robert-1.0.0.tar", last modified: Fri Jun 30 17:37:09 2023, max compression
+gzip compressed data, was "robert-1.0.1.tar", last modified: Sat Jul  1 07:56:06 2023, max compression
```

## Comparing `robert-1.0.0.tar` & `robert-1.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 17:37:09.083404 robert-1.0.0/
--rw-rw-rw-   0        0        0     1099 2023-05-23 09:25:43.000000 robert-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      992 2023-06-30 17:37:09.085836 robert-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2392 2023-06-18 10:39:36.000000 robert-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 17:37:09.038152 robert-1.0.0/robert/
--rw-rw-rw-   0        0        0        0 2023-05-23 09:25:43.000000 robert-1.0.0/robert/__init__.py
--rw-rw-rw-   0        0        0      583 2023-05-23 09:25:43.000000 robert-1.0.0/robert/__main__.py
--rw-rw-rw-   0        0        0     5020 2023-06-17 18:18:26.000000 robert-1.0.0/robert/aqme.py
--rw-rw-rw-   0        0        0     2017 2023-06-20 18:14:41.000000 robert-1.0.0/robert/argument_parser.py
--rw-rw-rw-   0        0        0    15344 2023-06-30 11:54:20.000000 robert-1.0.0/robert/curate.py
--rw-rw-rw-   0        0        0     7529 2023-06-20 18:11:53.000000 robert-1.0.0/robert/generate.py
--rw-rw-rw-   0        0        0    29733 2023-06-30 16:53:53.000000 robert-1.0.0/robert/generate_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-30 17:37:09.064396 robert-1.0.0/robert/model_params/
--rw-rw-rw-   0        0        0      211 2023-05-23 09:25:43.000000 robert-1.0.0/robert/model_params/ADAB_params.yaml
--rw-rw-rw-   0        0        0      775 2023-06-30 17:01:38.000000 robert-1.0.0/robert/model_params/GB_params.yaml
--rw-rw-rw-   0        0        0       91 2023-06-19 12:21:08.000000 robert-1.0.0/robert/model_params/GP_params.yaml
--rw-rw-rw-   0        0        0       88 2023-06-07 12:49:19.000000 robert-1.0.0/robert/model_params/MVL_params.yaml
--rw-rw-rw-   0        0        0      808 2023-06-07 12:43:39.000000 robert-1.0.0/robert/model_params/NN_params.yaml
--rw-rw-rw-   0        0        0      576 2023-06-30 17:01:41.000000 robert-1.0.0/robert/model_params/RF_params.yaml
--rw-rw-rw-   0        0        0      732 2023-06-30 17:01:45.000000 robert-1.0.0/robert/model_params/VR_params.yaml
--rw-rw-rw-   0        0        0     4374 2023-06-20 17:35:36.000000 robert-1.0.0/robert/predict.py
--rw-rw-rw-   0        0        0    26483 2023-06-21 06:22:51.000000 robert-1.0.0/robert/predict_utils.py
--rw-rw-rw-   0        0        0     5745 2023-05-23 09:25:43.000000 robert-1.0.0/robert/report.py
--rw-rw-rw-   0        0        0     5875 2023-06-20 15:37:54.000000 robert-1.0.0/robert/robert.py
--rw-rw-rw-   0        0        0    37329 2023-06-30 16:54:00.000000 robert-1.0.0/robert/utils.py
--rw-rw-rw-   0        0        0    19418 2023-06-20 15:37:54.000000 robert-1.0.0/robert/verify.py
-drwxrwxrwx   0        0        0        0 2023-06-30 17:37:09.048620 robert-1.0.0/robert.egg-info/
--rw-rw-rw-   0        0        0      992 2023-06-30 17:37:08.000000 robert-1.0.0/robert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      800 2023-06-30 17:37:08.000000 robert-1.0.0/robert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 17:37:08.000000 robert-1.0.0/robert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      158 2023-06-30 17:37:08.000000 robert-1.0.0/robert.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-30 17:37:08.000000 robert-1.0.0/robert.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      118 2023-06-30 17:37:09.085836 robert-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2035 2023-06-30 17:01:03.000000 robert-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 17:37:09.083404 robert-1.0.0/tests/
--rw-rw-rw-   0        0        0     6529 2023-06-19 15:13:27.000000 robert-1.0.0/tests/test_1curate.py
--rw-rw-rw-   0        0        0     6379 2023-06-20 18:16:46.000000 robert-1.0.0/tests/test_2generate.py
--rw-rw-rw-   0        0        0     4289 2023-06-20 19:38:53.000000 robert-1.0.0/tests/test_3verify.py
--rw-rw-rw-   0        0        0     5019 2023-06-20 19:47:48.000000 robert-1.0.0/tests/test_4predict.py
--rw-rw-rw-   0        0        0     4142 2023-06-20 18:05:57.000000 robert-1.0.0/tests/test_5aqme_n_full.py
+drwxrwxrwx   0        0        0        0 2023-07-01 07:56:06.123300 robert-1.0.1/
+-rw-rw-rw-   0        0        0     1099 2023-05-23 09:25:43.000000 robert-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      992 2023-07-01 07:56:06.123300 robert-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2392 2023-06-18 10:39:36.000000 robert-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 07:56:06.104071 robert-1.0.1/robert/
+-rw-rw-rw-   0        0        0        0 2023-05-23 09:25:43.000000 robert-1.0.1/robert/__init__.py
+-rw-rw-rw-   0        0        0      583 2023-05-23 09:25:43.000000 robert-1.0.1/robert/__main__.py
+-rw-rw-rw-   0        0        0     5020 2023-06-17 18:18:26.000000 robert-1.0.1/robert/aqme.py
+-rw-rw-rw-   0        0        0     2017 2023-06-20 18:14:41.000000 robert-1.0.1/robert/argument_parser.py
+-rw-rw-rw-   0        0        0    15344 2023-06-30 11:54:20.000000 robert-1.0.1/robert/curate.py
+-rw-rw-rw-   0        0        0     7529 2023-06-20 18:11:53.000000 robert-1.0.1/robert/generate.py
+-rw-rw-rw-   0        0        0    29733 2023-06-30 16:53:53.000000 robert-1.0.1/robert/generate_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-01 07:56:06.111490 robert-1.0.1/robert/model_params/
+-rw-rw-rw-   0        0        0      211 2023-05-23 09:25:43.000000 robert-1.0.1/robert/model_params/ADAB_params.yaml
+-rw-rw-rw-   0        0        0      775 2023-06-30 17:01:38.000000 robert-1.0.1/robert/model_params/GB_params.yaml
+-rw-rw-rw-   0        0        0       91 2023-06-19 12:21:08.000000 robert-1.0.1/robert/model_params/GP_params.yaml
+-rw-rw-rw-   0        0        0       88 2023-06-07 12:49:19.000000 robert-1.0.1/robert/model_params/MVL_params.yaml
+-rw-rw-rw-   0        0        0      808 2023-06-07 12:43:39.000000 robert-1.0.1/robert/model_params/NN_params.yaml
+-rw-rw-rw-   0        0        0      576 2023-06-30 17:01:41.000000 robert-1.0.1/robert/model_params/RF_params.yaml
+-rw-rw-rw-   0        0        0      732 2023-06-30 17:01:45.000000 robert-1.0.1/robert/model_params/VR_params.yaml
+-rw-rw-rw-   0        0        0     4374 2023-06-20 17:35:36.000000 robert-1.0.1/robert/predict.py
+-rw-rw-rw-   0        0        0    26483 2023-06-21 06:22:51.000000 robert-1.0.1/robert/predict_utils.py
+-rw-rw-rw-   0        0        0     5792 2023-07-01 07:20:39.000000 robert-1.0.1/robert/report.py
+-rw-rw-rw-   0        0        0     5875 2023-06-20 15:37:54.000000 robert-1.0.1/robert/robert.py
+-rw-rw-rw-   0        0        0    37329 2023-07-01 06:59:03.000000 robert-1.0.1/robert/utils.py
+-rw-rw-rw-   0        0        0    19418 2023-06-20 15:37:54.000000 robert-1.0.1/robert/verify.py
+drwxrwxrwx   0        0        0        0 2023-07-01 07:56:06.106828 robert-1.0.1/robert.egg-info/
+-rw-rw-rw-   0        0        0      992 2023-07-01 07:56:06.000000 robert-1.0.1/robert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      800 2023-07-01 07:56:06.000000 robert-1.0.1/robert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 07:56:06.000000 robert-1.0.1/robert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      142 2023-07-01 07:56:06.000000 robert-1.0.1/robert.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-01 07:56:06.000000 robert-1.0.1/robert.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      118 2023-07-01 07:56:06.123300 robert-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1953 2023-07-01 06:58:37.000000 robert-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 07:56:06.122798 robert-1.0.1/tests/
+-rw-rw-rw-   0        0        0     6529 2023-06-19 15:13:27.000000 robert-1.0.1/tests/test_1curate.py
+-rw-rw-rw-   0        0        0     6379 2023-06-20 18:16:46.000000 robert-1.0.1/tests/test_2generate.py
+-rw-rw-rw-   0        0        0     4289 2023-06-20 19:38:53.000000 robert-1.0.1/tests/test_3verify.py
+-rw-rw-rw-   0        0        0     5019 2023-06-20 19:47:48.000000 robert-1.0.1/tests/test_4predict.py
+-rw-rw-rw-   0        0        0     4142 2023-06-20 18:05:57.000000 robert-1.0.1/tests/test_5aqme_n_full.py
```

### Comparing `robert-1.0.0/LICENSE` & `robert-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robert-1.0.0/PKG-INFO` & `robert-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: robert
-Version: 1.0.0
+Version: 1.0.1
 Summary: Refiner and Optimizer of a Bunch of Existing Regression Tools
 Home-page: https://github.com/jvalegre/robert
-Download-URL: https://github.com/jvalegre/robert/archive/refs/tags/1.0.0.tar.gz
+Download-URL: https://github.com/jvalegre/robert/archive/refs/tags/1.0.1.tar.gz
 Author: Juan V. Alegre Requena, David Dalmau
 Author-email: jv.alegre@csic.es
 License: MIT
 Keywords: workflows,machine learning,cheminformatics,data curation,prediction,automated
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `robert-1.0.0/README.md` & `robert-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `robert-1.0.0/robert/__main__.py` & `robert-1.0.1/robert/__main__.py`

 * *Files identical despite different names*

### Comparing `robert-1.0.0/robert/aqme.py` & `robert-1.0.1/robert/aqme.py`

 * *Files identical despite different names*

### Comparing `robert-1.0.0/robert/argument_parser.py` & `robert-1.0.1/robert/argument_parser.py`

 * *Files identical despite different names*

### Comparing `robert-1.0.0/robert/curate.py` & `robert-1.0.1/robert/curate.py`

 * *Files identical despite different names*

### Comparing `robert-1.0.0/robert/generate.py` & `robert-1.0.1/robert/generate.py`

 * *Files identical despite different names*

### Comparing `robert-1.0.0/robert/generate_utils.py` & `robert-1.0.1/robert/generate_utils.py`

 * *Files identical despite different names*

### Comparing `robert-1.0.0/robert/model_params/GB_params.yaml` & `robert-1.0.1/robert/model_params/GB_params.yaml`

 * *Files identical despite different names*

### Comparing `robert-1.0.0/robert/model_params/NN_params.yaml` & `robert-1.0.1/robert/model_params/NN_params.yaml`

 * *Files identical despite different names*

### Comparing `robert-1.0.0/robert/model_params/RF_params.yaml` & `robert-1.0.1/robert/model_params/RF_params.yaml`

 * *Files identical despite different names*

### Comparing `robert-1.0.0/robert/model_params/VR_params.yaml` & `robert-1.0.1/robert/model_params/VR_params.yaml`

 * *Files identical despite different names*

### Comparing `robert-1.0.0/robert/predict.py` & `robert-1.0.1/robert/predict.py`

 * *Files identical despite different names*

### Comparing `robert-1.0.0/robert/predict_utils.py` & `robert-1.0.1/robert/predict_utils.py`

 * *Files identical despite different names*

### Comparing `robert-1.0.0/robert/report.py` & `robert-1.0.1/robert/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 
 """
 #####################################################.
 #        This file stores the REPORT class          #
 #    used for generating the final PDF report       #
 #####################################################.
 
-from robert.utils import (load_variables,
-)
+from robert.utils import (load_variables)
 
 class report:
     """
     Class containing all the functions from the REPORT module.
 
     Parameters
     ----------
@@ -34,15 +33,15 @@
     def __init__(self, **kwargs):
 
         # check if there is a problem with weasyprint (required for this module)
         _ = self.init_report()
 
         # load default and user-specified variables
         self.args = load_variables(kwargs, "report")
-            
+
         # # load data from DAT files
         # def data_content(self):
         #     """
         #     Reads a file and returns a formatted string between two markers
         #     """
 
         #     start_str = X
@@ -76,16 +75,16 @@
     def init_report(self):
         '''
         Checks whether weasyprint works to make the report
         '''
 
         try:
             from weasyprint import HTML
-        except OSError:
-            print(f"\n  x The REPORT module requires weasyprint, and it is not compatible with your installation. Try installing ROBERT with 'conda install -c conda-forge robert'")
+        except (OSError,ModuleNotFoundError):
+            print(f"\n  x The REPORT module requires weasyprint but this module is missing, the PDF with the summary of the results has not been created. Try installing ROBERT with 'conda install -c conda-forge robert'")
 
 
 # def css_content_fun():
 #     '''
 #     Create content for css
 #     '''
```

### Comparing `robert-1.0.0/robert/robert.py` & `robert-1.0.1/robert/robert.py`

 * *Files identical despite different names*

### Comparing `robert-1.0.0/robert/utils.py` & `robert-1.0.1/robert/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     VotingClassifier)
 from sklearn.gaussian_process import GaussianProcessRegressor, GaussianProcessClassifier
 from sklearn.neural_network import MLPRegressor, MLPClassifier
 from sklearn.linear_model import LinearRegression
 import warnings # this avoids warnings from sklearn
 warnings.filterwarnings("ignore")
 
-robert_version = "1.1.0"
+robert_version = "1.0.1"
 time_run = time.strftime("%Y/%m/%d %H:%M:%S", time.localtime())
 robert_ref = f"ROBERT v {robert_version}, Dalmau, D.; Alegre-Requena, J. V., 2023. https://github.com/jvalegre/robert"
 
 
 # load paramters from yaml file
 def load_from_yaml(self):
     """
```

### Comparing `robert-1.0.0/robert/verify.py` & `robert-1.0.1/robert/verify.py`

 * *Files identical despite different names*

### Comparing `robert-1.0.0/robert.egg-info/PKG-INFO` & `robert-1.0.1/robert.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: robert
-Version: 1.0.0
+Version: 1.0.1
 Summary: Refiner and Optimizer of a Bunch of Existing Regression Tools
 Home-page: https://github.com/jvalegre/robert
-Download-URL: https://github.com/jvalegre/robert/archive/refs/tags/1.0.0.tar.gz
+Download-URL: https://github.com/jvalegre/robert/archive/refs/tags/1.0.1.tar.gz
 Author: Juan V. Alegre Requena, David Dalmau
 Author-email: jv.alegre@csic.es
 License: MIT
 Keywords: workflows,machine learning,cheminformatics,data curation,prediction,automated
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `robert-1.0.0/robert.egg-info/SOURCES.txt` & `robert-1.0.1/robert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robert-1.0.0/setup.py` & `robert-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
-version="1.0.0"
+version="1.0.1"
 setup(
     name="robert",
     packages=find_packages(exclude=["tests"]),
     package_data={"robert": ["model_params/*"]},
     version=version,
     license="MIT",
     description="Refiner and Optimizer of a Bunch of Existing Regression Tools",
@@ -39,16 +39,13 @@
         "matplotlib>=3.7.1",
         "seaborn",
         "scipy",
         "scikit-learn>=1.2,<1.3",
         "hyperopt",
         "numba",
         "shap",
-        "glib",
-        "weasyprint",
         "scikit-learn-intelex",
-        # requires also "conda install -c conda-forge gtk3" in Windows
-        # requires also "conda install -c conda-forge shap"
+        # requires also "conda install -c conda-forge gtk3 glib weasyprint" for report.py
     ],
     python_requires=">=3.0",
     include_package_data=True,
 )
```

### Comparing `robert-1.0.0/tests/test_1curate.py` & `robert-1.0.1/tests/test_1curate.py`

 * *Files identical despite different names*

### Comparing `robert-1.0.0/tests/test_2generate.py` & `robert-1.0.1/tests/test_2generate.py`

 * *Files identical despite different names*

### Comparing `robert-1.0.0/tests/test_3verify.py` & `robert-1.0.1/tests/test_3verify.py`

 * *Files identical despite different names*

### Comparing `robert-1.0.0/tests/test_4predict.py` & `robert-1.0.1/tests/test_4predict.py`

 * *Files identical despite different names*

### Comparing `robert-1.0.0/tests/test_5aqme_n_full.py` & `robert-1.0.1/tests/test_5aqme_n_full.py`

 * *Files identical despite different names*

