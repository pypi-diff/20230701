# Comparing `tmp/sincfold-0.1.1.tar.gz` & `tmp/sincfold-0.2.tar.gz`

## Comparing `sincfold-0.1.1.tar` & `sincfold-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 sincfold-0.1.1/hubconf.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 sincfold-0.1.1/setup.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 sincfold-0.1.1/splits.py
--rw-r--r--   0        0        0     7934 2020-02-02 00:00:00.000000 sincfold-0.1.1/src/sincfold/__init__.py
--rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 sincfold-0.1.1/src/sincfold/dataset.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 sincfold-0.1.1/src/sincfold/embeddings.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 sincfold-0.1.1/src/sincfold/metrics.py
--rw-r--r--   0        0        0    10483 2020-02-02 00:00:00.000000 sincfold-0.1.1/src/sincfold/model.py
--rw-r--r--   0        0        0     9338 2020-02-02 00:00:00.000000 sincfold-0.1.1/src/sincfold/utils.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 sincfold-0.1.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sincfold-0.1.1/LICENSE
--rw-r--r--   0        0        0     3883 2020-02-02 00:00:00.000000 sincfold-0.1.1/README.md
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 sincfold-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 sincfold-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0   160805 2020-02-02 00:00:00.000000 sincfold-0.2/abstract.png
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 sincfold-0.2/hubconf.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 sincfold-0.2/setup.py
+-rw-r--r--   0        0        0     7934 2020-02-02 00:00:00.000000 sincfold-0.2/src/sincfold/__init__.py
+-rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 sincfold-0.2/src/sincfold/dataset.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 sincfold-0.2/src/sincfold/embeddings.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 sincfold-0.2/src/sincfold/metrics.py
+-rw-r--r--   0        0        0    10483 2020-02-02 00:00:00.000000 sincfold-0.2/src/sincfold/model.py
+-rw-r--r--   0        0        0     9338 2020-02-02 00:00:00.000000 sincfold-0.2/src/sincfold/utils.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 sincfold-0.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sincfold-0.2/LICENSE
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 sincfold-0.2/README.md
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 sincfold-0.2/pyproject.toml
+-rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 sincfold-0.2/PKG-INFO
```

### Comparing `sincfold-0.1.1/src/sincfold/__init__.py` & `sincfold-0.2/src/sincfold/__init__.py`

 * *Files identical despite different names*

### Comparing `sincfold-0.1.1/src/sincfold/dataset.py` & `sincfold-0.2/src/sincfold/dataset.py`

 * *Files identical despite different names*

### Comparing `sincfold-0.1.1/src/sincfold/embeddings.py` & `sincfold-0.2/src/sincfold/embeddings.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import torch as tr
 
 # Mapping of nucleotide symbols
+# R	Guanine / Adenine (purine)
 # Y	Cytosine / Uracil (pyrimidine)
 # K	Guanine / Uracil
 # M	Adenine / Cytosine
 # S	Guanine / Cytosine
 # W	Adenine / Uracil
 # B	Guanine / Uracil / Cytosine
 # D	Guanine / Adenine / Uracil
 # H	Adenine / Cytosine / Uracil
 # V	Guanine / Cytosine / Adenine
 # N	Adenine / Guanine / Cytosine / Uracil
 NT_DICT = {
+    "R": ["G", "A"],
     "Y": ["C", "U"],
     "K": ["G", "U"],
     "M": ["A", "C"],
     "S": ["G", "C"],
     "W": ["A", "U"],
     "B": ["G", "U", "C"],
     "D": ["G", "A", "U"],
```

### Comparing `sincfold-0.1.1/src/sincfold/metrics.py` & `sincfold-0.2/src/sincfold/metrics.py`

 * *Files identical despite different names*

### Comparing `sincfold-0.1.1/src/sincfold/model.py` & `sincfold-0.2/src/sincfold/model.py`

 * *Files identical despite different names*

### Comparing `sincfold-0.1.1/src/sincfold/utils.py` & `sincfold-0.2/src/sincfold/utils.py`

 * *Files identical despite different names*

### Comparing `sincfold-0.1.1/.gitignore` & `sincfold-0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sincfold-0.1.1/LICENSE` & `sincfold-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sincfold-0.1.1/README.md` & `sincfold-0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-# sincFold
+# **sincFold**: a RNA folding prediction tool based on deep learning.
 
-This is the repository for sincFold, a new RNA folding prediction tool based on deep learning.
+<p align="center">
+<img src="abstract.png" alt="abstract">
+</p>
 
 ```bibtex
 @article{sincFold2023,
-  title={sincFold: a fast end-to-end method to accurately fold RNA sequences with deep learning},
-  author={Leandro A. Bugnon and Leandro Di Persia and Matias Gerard and Jonathan Raad and Santiago Prochetto and Emilio Fenoy and  Georgina Stegmayer and Diego H. Milone},
+  title={sincFold: an end-to-end method to accurately fold RNA sequences with compressed short-long context encodings and binding restrictions},
+  author={Leandro A. Bugnon and Leandro Di Persia and Matias Gerard and Jonathan Raad and Santiago Prochetto and Emilio Fenoy and Uciel Chorostecki and Georgina Stegmayer and Diego H. Milone},
   journal={under review},
   year={2023}
 }
 ```
-<p align="center">
-<img src="abstract.png" alt="abstract">
-</p>
 
 sincFold is a fast and accurate RNA secondary structure prediction method. It is an end-to-end approach that predict the nucleotides contact matrix using only the RNA sequence as input. The model is based on a residual neural network that can learn short and long context features from a small dataset, it can incorporate base-pair constraints and can guarantee the output structure to be valid.  Extensive experiments on several benchmark datasets were made, comparing sincFold against classical methods and new models based on deep learning. We demonstrate that sincFold achieves a very competitive performance in comparison with state-of-the-art methods.
 
 A summary of results can be seen in [this notebook](results/summary.ipynb).
 
 ## Folding RNA sequences
 
 We have a [webserver](https://sinc.unl.edu.ar/web-demo/sincfold/) running with the lattest version. This server admits one sequence at a time. Please follow the next
-instructions if you want to run the model locally. We provide a model pretrained with validated  RNA datasets (archiveII, RNAstralign, urs-pdb). At the end you can find the instructions to replicate our results from scratch.
+instructions if you want to run the model locally. We provide a model pretrained with validated  RNA datasets (archiveII, RNAstralign, urs-pdb). At the end you can find the instructions to replicate our cross-validation results from scratch.
 
 ## Install
 
 This is a Python package. It is recommended to use virtualenv or conda to create a new enviroment and avoid breaking system packages.
 
 To install the package, run:
 
@@ -87,8 +86,8 @@
 then call the training and testing functions
 
 
     sincFold train working_path/train.csv --valid_file working_path/valid.csv -o working_path/output/
 
     sincFold test working_path/test.csv -m working_path/output/weights.pmt
 
-The complete process may take about 4hs using a RTX A5000.
+The complete process may take about 3hs using a RTX A5000.
```

### Comparing `sincfold-0.1.1/pyproject.toml` & `sincfold-0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sincfold"
-version = "0.1.1"
+version = "0.2"
 authors = [
   {name="Leandro Bugnon", email="lbugnon@sinc.unl.edu.ar"}]
 description = "An end-to-end method to predict RNA secondary structure based on deep learning"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "torch",
@@ -24,8 +24,8 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/sinc-lab/sincfold"
 "Bug Tracker" = "https://github.com/sinc-lab/sincfold/issues"
 
 [project.scripts]
-sincFold = "sincfold:main"
+sincFold = "sincfold:main"
```

### Comparing `sincfold-0.1.1/PKG-INFO` & `sincfold-0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 Metadata-Version: 2.1
 Name: sincfold
-Version: 0.1.1
+Version: 0.2
 Summary: An end-to-end method to predict RNA secondary structure based on deep learning
 Project-URL: Homepage, https://github.com/sinc-lab/sincfold
 Project-URL: Bug Tracker, https://github.com/sinc-lab/sincfold/issues
 Author-email: Leandro Bugnon <lbugnon@sinc.unl.edu.ar>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
 Requires-Dist: torch
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
-# sincFold
+# **sincFold**: a RNA folding prediction tool based on deep learning.
 
-This is the repository for sincFold, a new RNA folding prediction tool based on deep learning.
+<p align="center">
+<img src="abstract.png" alt="abstract">
+</p>
 
 ```bibtex
 @article{sincFold2023,
-  title={sincFold: a fast end-to-end method to accurately fold RNA sequences with deep learning},
-  author={Leandro A. Bugnon and Leandro Di Persia and Matias Gerard and Jonathan Raad and Santiago Prochetto and Emilio Fenoy and  Georgina Stegmayer and Diego H. Milone},
+  title={sincFold: an end-to-end method to accurately fold RNA sequences with compressed short-long context encodings and binding restrictions},
+  author={Leandro A. Bugnon and Leandro Di Persia and Matias Gerard and Jonathan Raad and Santiago Prochetto and Emilio Fenoy and Uciel Chorostecki and Georgina Stegmayer and Diego H. Milone},
   journal={under review},
   year={2023}
 }
 ```
-<p align="center">
-<img src="abstract.png" alt="abstract">
-</p>
 
 sincFold is a fast and accurate RNA secondary structure prediction method. It is an end-to-end approach that predict the nucleotides contact matrix using only the RNA sequence as input. The model is based on a residual neural network that can learn short and long context features from a small dataset, it can incorporate base-pair constraints and can guarantee the output structure to be valid.  Extensive experiments on several benchmark datasets were made, comparing sincFold against classical methods and new models based on deep learning. We demonstrate that sincFold achieves a very competitive performance in comparison with state-of-the-art methods.
 
 A summary of results can be seen in [this notebook](results/summary.ipynb).
 
 ## Folding RNA sequences
 
 We have a [webserver](https://sinc.unl.edu.ar/web-demo/sincfold/) running with the lattest version. This server admits one sequence at a time. Please follow the next
-instructions if you want to run the model locally. We provide a model pretrained with validated  RNA datasets (archiveII, RNAstralign, urs-pdb). At the end you can find the instructions to replicate our results from scratch.
+instructions if you want to run the model locally. We provide a model pretrained with validated  RNA datasets (archiveII, RNAstralign, urs-pdb). At the end you can find the instructions to replicate our cross-validation results from scratch.
 
 ## Install
 
 This is a Python package. It is recommended to use virtualenv or conda to create a new enviroment and avoid breaking system packages.
 
 To install the package, run:
 
@@ -106,8 +105,8 @@
 then call the training and testing functions
 
 
     sincFold train working_path/train.csv --valid_file working_path/valid.csv -o working_path/output/
 
     sincFold test working_path/test.csv -m working_path/output/weights.pmt
 
-The complete process may take about 4hs using a RTX A5000.
+The complete process may take about 3hs using a RTX A5000.
```

