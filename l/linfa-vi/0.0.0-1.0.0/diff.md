# Comparing `tmp/linfa_vi-0.0.0.tar.gz` & `tmp/linfa_vi-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linfa_vi-0.0.0.tar", last modified: Sat Jul  1 12:23:33 2023, max compression
+gzip compressed data, was "linfa_vi-1.0.0.tar", last modified: Sat Jul  1 16:07:09 2023, max compression
```

## Comparing `linfa_vi-0.0.0.tar` & `linfa_vi-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 dschiava  (1000) dschiava  (1000)        0 2023-07-01 12:23:33.115355 linfa_vi-0.0.0/
--rw-rw-r--   0 dschiava  (1000) dschiava  (1000)     1069 2023-05-29 22:46:19.000000 linfa_vi-0.0.0/LICENSE
--rw-rw-r--   0 dschiava  (1000) dschiava  (1000)     6338 2023-07-01 12:23:33.115355 linfa_vi-0.0.0/PKG-INFO
--rw-rw-r--   0 dschiava  (1000) dschiava  (1000)     4630 2023-07-01 10:23:13.000000 linfa_vi-0.0.0/README.md
-drwxrwxr-x   0 dschiava  (1000) dschiava  (1000)        0 2023-07-01 12:23:33.115355 linfa_vi-0.0.0/linfa/
--rw-rw-r--   0 dschiava  (1000) dschiava  (1000)        0 2023-05-29 22:46:19.000000 linfa_vi-0.0.0/linfa/__init__.py
--rw-rw-r--   0 dschiava  (1000) dschiava  (1000)    13040 2023-07-01 10:23:13.000000 linfa_vi-0.0.0/linfa/maf.py
--rw-rw-r--   0 dschiava  (1000) dschiava  (1000)    13517 2023-07-01 10:23:13.000000 linfa_vi-0.0.0/linfa/nofas.py
--rw-rw-r--   0 dschiava  (1000) dschiava  (1000)    13030 2023-07-01 10:23:13.000000 linfa_vi-0.0.0/linfa/run_experiment.py
--rw-rw-r--   0 dschiava  (1000) dschiava  (1000)     4331 2023-07-01 10:23:13.000000 linfa_vi-0.0.0/linfa/transform.py
-drwxrwxr-x   0 dschiava  (1000) dschiava  (1000)        0 2023-07-01 12:23:33.115355 linfa_vi-0.0.0/linfa_vi.egg-info/
--rw-rw-r--   0 dschiava  (1000) dschiava  (1000)     6338 2023-07-01 12:23:33.000000 linfa_vi-0.0.0/linfa_vi.egg-info/PKG-INFO
--rw-rw-r--   0 dschiava  (1000) dschiava  (1000)      309 2023-07-01 12:23:33.000000 linfa_vi-0.0.0/linfa_vi.egg-info/SOURCES.txt
--rw-rw-r--   0 dschiava  (1000) dschiava  (1000)        1 2023-07-01 12:23:33.000000 linfa_vi-0.0.0/linfa_vi.egg-info/dependency_links.txt
--rw-rw-r--   0 dschiava  (1000) dschiava  (1000)      117 2023-07-01 12:23:33.000000 linfa_vi-0.0.0/linfa_vi.egg-info/requires.txt
--rw-rw-r--   0 dschiava  (1000) dschiava  (1000)        6 2023-07-01 12:23:33.000000 linfa_vi-0.0.0/linfa_vi.egg-info/top_level.txt
--rw-rw-r--   0 dschiava  (1000) dschiava  (1000)     1310 2023-07-01 12:18:03.000000 linfa_vi-0.0.0/pyproject.toml
--rw-rw-r--   0 dschiava  (1000) dschiava  (1000)       38 2023-07-01 12:23:33.115355 linfa_vi-0.0.0/setup.cfg
--rw-rw-r--   0 dschiava  (1000) dschiava  (1000)       38 2023-05-29 22:46:19.000000 linfa_vi-0.0.0/setup.py
-drwxrwxr-x   0 dschiava  (1000) dschiava  (1000)        0 2023-07-01 12:23:33.115355 linfa_vi-0.0.0/tests/
--rw-rw-r--   0 dschiava  (1000) dschiava  (1000)    29771 2023-07-01 10:35:40.000000 linfa_vi-0.0.0/tests/test_linfa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:07:09.685803 linfa_vi-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-01 16:05:08.000000 linfa_vi-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-07-01 16:07:09.685803 linfa_vi-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-07-01 16:05:08.000000 linfa_vi-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:07:09.681803 linfa_vi-1.0.0/linfa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 16:05:08.000000 linfa_vi-1.0.0/linfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-07-01 16:05:08.000000 linfa_vi-1.0.0/linfa/maf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-07-01 16:05:08.000000 linfa_vi-1.0.0/linfa/nofas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13555 2023-07-01 16:05:08.000000 linfa_vi-1.0.0/linfa/run_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-01 16:05:08.000000 linfa_vi-1.0.0/linfa/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:07:09.685803 linfa_vi-1.0.0/linfa_vi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-07-01 16:07:09.000000 linfa_vi-1.0.0/linfa_vi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-01 16:07:09.000000 linfa_vi-1.0.0/linfa_vi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 16:07:09.000000 linfa_vi-1.0.0/linfa_vi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-01 16:07:09.000000 linfa_vi-1.0.0/linfa_vi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-01 16:07:09.000000 linfa_vi-1.0.0/linfa_vi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-01 16:05:08.000000 linfa_vi-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 16:07:09.685803 linfa_vi-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 16:05:08.000000 linfa_vi-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:07:09.685803 linfa_vi-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    30715 2023-07-01 16:05:08.000000 linfa_vi-1.0.0/tests/test_linfa.py
```

### Comparing `linfa_vi-0.0.0/LICENSE` & `linfa_vi-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `linfa_vi-0.0.0/PKG-INFO` & `linfa_vi-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linfa_vi
-Version: 0.0.0
+Version: 1.0.0
 Summary: A Python library for inference with normalizing flow and annealing
 Author-email: resDesLab  <daniele.schiavazzi@gmail.com>
 License: Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -26,14 +26,21 @@
 
 ## LINFA
 
 LINFA is a library for variational inference with normalizing flow and adaptive annealing. It is designed to accommodate computationally expensive models and difficult-to-sample posterior distributions with dependent parameters.
 
 The code for the masked autoencoders for density estimation (MADE), masked autoregressive flow (MAF) and real non volume-preserving transformation (RealNVP) is based on the implementation provided by [Kamen Bliznashki](https://github.com/kamenbliznashki/normalizing_flows). 
 
+### Installation
+
+To install LINFA type
+
+```
+pip install linfa-vi
+```
 
 ### Documentation 
 
 The documentation can be found on [readmydocs]()
 
 ### References
```

### Comparing `linfa_vi-0.0.0/README.md` & `linfa_vi-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 
 ## LINFA
 
 LINFA is a library for variational inference with normalizing flow and adaptive annealing. It is designed to accommodate computationally expensive models and difficult-to-sample posterior distributions with dependent parameters.
 
 The code for the masked autoencoders for density estimation (MADE), masked autoregressive flow (MAF) and real non volume-preserving transformation (RealNVP) is based on the implementation provided by [Kamen Bliznashki](https://github.com/kamenbliznashki/normalizing_flows). 
 
+### Installation
+
+To install LINFA type
+
+```
+pip install linfa-vi
+```
 
 ### Documentation 
 
 The documentation can be found on [readmydocs]()
 
 ### References
```

### Comparing `linfa_vi-0.0.0/linfa/maf.py` & `linfa_vi-1.0.0/linfa/maf.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-0.0.0/linfa/nofas.py` & `linfa_vi-1.0.0/linfa/nofas.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-0.0.0/linfa/run_experiment.py` & `linfa_vi-1.0.0/linfa/run_experiment.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,66 +1,76 @@
 import os
 import torch
 import numpy as np
-import scipy as sp
-from maf import MAF, RealNVP
+from linfa.maf import MAF, RealNVP
 
 torch.set_default_tensor_type(torch.DoubleTensor)
 
 class experiment:
     """Defines an instance of variational inference
 
     This class is the core class of the LINFA library
     and defines all the default hyperparameter values and 
     and functions used for inference. 
     """
     def __init__(self):
+
+        # NF ARCHITECTURE parameters
         self.name              = "Experiment"
+        self.input_size        = 3             #:int:  Number of input parameters
         self.flow_type         = 'maf'         #:str:  Type of flow ('maf' or 'realnvp')
         self.n_blocks          = 15            #:int:  Number of layers
         self.hidden_size       = 100           #:int:  Hidden layer size for MADE in each layer
         self.n_hidden          = 1             #:int:  Number of hidden layers in each MADE
         self.activation_fn     = 'relu'        #:str:  Actication function used (either 'relu','tanh' or 'sigmoid')
         self.input_order       = 'sequential'  #:str:  Input order for create_mask (either 'sequential' or 'random')
         self.batch_norm_order  = True          #:bool: Uses decide if batch_norm is used
-        self.save_interval     = 200           #:int:  Save interval for all results
-        self.store_nf_interval = 1000          #:int:  Save interval for normalizing flow parameters
 
-        self.input_size    = 3      #:int:    Number of input parameters
-        self.batch_size    = 500    #:int:    Number of batch samples generated at every iteration from the base distribution
-        self.true_data_num = 2      #:double: Number of true model evaluated at each surrogate update
-        self.n_iter        = 25001  #:int:    Total number of iterations
-        self.lr            = 0.003  #:double: Learning rate
-        self.lr_decay      = 0.9999 #:double: Learning rate decay
-
-        self.run_nofas          = True #:bool: Activate NoFAS and the use of a surrogate model
-        self.log_interval       = 10   #:int:  How often the loss statistics are printed
-        self.calibrate_interval = 300  #:int:  How often the surrogate model is updated
-        self.budget             = 216  #:int:  Maximum number of allowed evaluations of the true model
+        # NOFAS parameters
+        self.run_nofas          = True  #:bool:   Activate NoFAS and the use of a surrogate model
+        self.log_interval       = 10    #:int:    How often the loss statistics are printed
+        self.calibrate_interval = 300   #:int:    How often the surrogate model is updated
+        self.true_data_num      = 2     #:double: Number of true model evaluated at each surrogate update
+        self.budget             = 216   #:int:    Maximum number of allowed evaluations of the true model
+        self.surr_pre_it        = 40000 #:int:    Number of pre-training iterations for surrogate model
+        self.surr_upd_it        = 6000  #:int:    Number of iterations for the surrogate model update
 
+        # OPTIMIZER parameters
         self.optimizer    = 'Adam'   #:str:    Type of optimizer used (either 'Adam' or 'RMSprop')
+        self.lr           = 0.003    #:double: Learning rate
+        self.lr_decay     = 0.9999   #:double: Learning rate decay
         self.lr_scheduler = 'StepLR' #:str:    type of lr scheduler used (either 'StepLR' or 'ExponentialLR')
         self.lr_step      = 1000     #:int:    Number of steps for StepLR learning rate scheduler 
+        self.batch_size   = 500      #:int:    Number of batch samples generated at every iteration from the base distribution        
+        self.n_iter       = 25001    #:int:    Total number of iterations
+
+        # ANNEALING parameters
+        self.annealing    = True     #:bool:   Flag to activate an annealing scheduler
+        self.scheduler    = 'AdaAnn' #:str:    Type of annealing scheduler (either 'AdaAnn' or 'Linear')
+        # AdaAnn
         self.tol          = 0.001    #:double: KL tolerance for AdaAnn scheduler
         self.t0           = 0.01     #:double: Initial value for the inverse temperature
         self.N            = 100      #:int:    Number of batch samples generated for $t<1$ at each iteration
         self.N_1          = 1000     #:int:    number of batch samples generated for $t=1$ at each iteration
         self.T_0          = 500      #:int:    Number of parameter updates at the initial inverse temperature $t_0$
         self.T            = 5        #:int:    Number of parameter updates for each temperature for $t<1$
         self.T_1          = 5001     #:int:    Number of parameter updates at $t=1$
-        self.M            = 1000     #:int:    Number of Monte Carlo  samples use to compute the denominator of the AdaAnn formula
-        self.annealing    = True     #:boo:    Flag to activate an annealing scheduler
-        self.scheduler    = 'AdaAnn' #:str:    Type of annealing scheduler (either 'AdaAnn' or 'Linear')
+        self.M            = 1000     #:int:    Number of Monte Carlo  samples use to compute the denominator of the AdaAnn formula        
+        # Linear scheduler
         self.linear_step  = 0.0001   #:double: Fixed step size for the Linear annealing scheduler
 
-        self.output_dir = './results/' + self.name #:str: Name of the output folder
-        self.log_file   = 'log.txt'                #:str: File name where the log profile stats are written
-        self.seed       = 35435                    #:int: Random seed
-        self.n_sample   = 5000                     #:int: Number of batch samples used to print results at save_interval
+        # OUTPUT parameters
+        self.output_dir        = './results/' + self.name #:str: Name of the output folder
+        self.log_file          = 'log.txt'                #:str: File name where the log profile stats are written
+        self.seed              = 35435                    #:int: Random seed
+        self.n_sample          = 5000                     #:int: Number of batch samples used to print results at save_interval
+        self.save_interval     = 200                      #:int: Save interval for all results
+        self.store_nf_interval = 1000                     #:int: Save interval for normalizing flow parameters
 
+        # DEVICE parameters
         self.no_cuda = True #:bool: Flag to use CPU
 
         # Set device
         self.device = torch.device('cuda:0' if torch.cuda.is_available() and not self.no_cuda else 'cpu')
 
         # Local pointer to the main components for inference
         self.transform        = None
@@ -230,15 +240,15 @@
 
         # updating surrogate model
         if self.run_nofas and iteration % self.calibrate_interval == 0 and self.surrogate.grid_record.size(0) < self.budget:
             xk0 = xk[:self.true_data_num, :].data.clone()            
             # print("\n")
             # print(list(self.surrogate.grid_record.size())[0])
             # print(xk0)
-            self.surrogate.update(xk0, max_iters=6000)
+            self.surrogate.update(xk0, max_iters=self.surr_upd_it)
 
         # Free energy bound
         loss = (- torch.sum(sum_log_abs_det_jacobians, 1) - t * self.model_logdensity(xk)).mean()
         optimizer.zero_grad()
         loss.backward()
         optimizer.step()
         if iteration % self.log_interval == 0:
```

### Comparing `linfa_vi-0.0.0/linfa/transform.py` & `linfa_vi-1.0.0/linfa/transform.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-0.0.0/linfa_vi.egg-info/PKG-INFO` & `linfa_vi-1.0.0/linfa_vi.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linfa-vi
-Version: 0.0.0
+Version: 1.0.0
 Summary: A Python library for inference with normalizing flow and annealing
 Author-email: resDesLab  <daniele.schiavazzi@gmail.com>
 License: Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -26,14 +26,21 @@
 
 ## LINFA
 
 LINFA is a library for variational inference with normalizing flow and adaptive annealing. It is designed to accommodate computationally expensive models and difficult-to-sample posterior distributions with dependent parameters.
 
 The code for the masked autoencoders for density estimation (MADE), masked autoregressive flow (MAF) and real non volume-preserving transformation (RealNVP) is based on the implementation provided by [Kamen Bliznashki](https://github.com/kamenbliznashki/normalizing_flows). 
 
+### Installation
+
+To install LINFA type
+
+```
+pip install linfa-vi
+```
 
 ### Documentation 
 
 The documentation can be found on [readmydocs]()
 
 ### References
```

### Comparing `linfa_vi-0.0.0/pyproject.toml` & `linfa_vi-1.0.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "linfa_vi"
-version = "0.0.0"
+version = "1.0.0"
 description = "A Python library for inference with normalizing flow and annealing"
 readme = "README.md"
 authors = [{ name = "resDesLab ", email = "daniele.schiavazzi@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -29,25 +29,7 @@
 packages = ["linfa"]
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/desResLab/LINFA"
-
-[tool.bumpver]
-current_version = "2023.1001-alpha"
-version_pattern = "YYYY.BUILD[-TAG]"
-commit_message = "bump version {old_version} -> {new_version}"
-commit = true
-tag = true
-push = true
-
-[tool.bumpver.file_patterns]
-"pyproject.toml" = [
-    'current_version = "{version}"',
-]
-"README.md" = [
-    "{version}",
-    "{pep440_version}",
-]
-
```

### Comparing `linfa_vi-0.0.0/tests/test_linfa.py` & `linfa_vi-1.0.0/tests/test_linfa.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import unittest
-import os,sys,argparse
+import os
 from linfa.run_experiment import experiment
 from linfa.transform import Transformation
 from linfa.nofas import Surrogate
 import torch
 import random
 import numpy as np
-import math
 
 class linfa_test_suite(unittest.TestCase):
 
     def trivial_example(self):
 
         if "it" in os.environ:
           max_it  = int(os.environ["it"])
+          max_pre = 1000
         else:
           max_it  = 25001
+          max_pre = 40000
 
         print('')
         print('--- TEST 1: TRIVIAL FUNCTION - NOFAS')
         print('')
 
         # Import trivial model
         from linfa.models.TrivialModels import Trivial
@@ -41,14 +42,16 @@
         # exp.n_iter      = 25001
         exp.n_iter        = max_it  # int: Number of iterations (default 25001)
         exp.lr            = 0.002   # float: Learning rate (default 0.003)
         exp.lr_decay      = 0.9999  # float: Learning rate decay (default 0.9999)
         exp.log_interval  = 10      # int: How often to show loss stat (default 10)
 
         exp.run_nofas          = True
+        exp.surr_pre_it        = max_pre #:int: Number of pre-training iterations for surrogate model
+        exp.surr_upd_it        = 6000  #:int: Number of iterations for the surrogate model update
         exp.annealing          = False
         exp.calibrate_interval = 1000  # int: How often to update surrogate model (default 1000)
         exp.budget             = 64    # int: Total number of true model evaluation
 
         exp.output_dir   = './results/' + exp.name
         exp.log_file     = 'log.txt'
         exp.seed         = random.randint(0, 10 ** 9)  # int: Random seed used
@@ -77,15 +80,15 @@
         # Define surrogate
         exp.surrogate = Surrogate(exp.name, lambda x: model.solve_t(trsf.forward(x)), 2, 2, [[0, 6], [0, 6]], 20, device=exp.device)
         if exp.run_nofas:
             if not os.path.isfile(exp.name + ".sur") or not os.path.isfile(exp.name + ".npz"):
                 print("Warning: Surrogate model files: {0}.npz and {0}.npz could not be found. ".format(exp.name))
                 # 4 samples for each dimension: pre-grid size = 16
                 exp.surrogate.gen_grid(gridnum=4)
-                exp.surrogate.pre_train(40000, 0.03, 0.9999, 500, store=True)
+                exp.surrogate.pre_train(exp.surr_pre_it, 0.03, 0.9999, 500, store=True)
         exp.surrogate.surrogate_load()
 
         # Define log density
         def log_density(x, model, surrogate, transform):
             # x contains the original, untransformed inputs
 
             # Compute transformation log Jacobian
@@ -117,16 +120,18 @@
         exp.run()
 
 
     def highdim_example(self):
 
         if "it" in os.environ:
           max_it  = int(os.environ["it"])
+          max_pre = 1000
         else:
           max_it  = 25001
+          max_pre = 100000
 
         print('')
         print('--- TEST 2: HIGH DIMENSIONAL SOBOL FUNCTION - NOFAS')
         print('')
 
         from linfa.models.highdimModels import Highdim
         
@@ -147,14 +152,17 @@
         # exp.n_iter      = 25001
         exp.n_iter        = max_it  # int: Number of iterations (default 25001)
         exp.lr            = 0.003   # float: Learning rate (default 0.003)
         exp.lr_decay      = 0.9999  # float: Learning rate decay (default 0.9999)
         exp.log_interval  = 10      # int: How often to show loss stat (default 10)
 
         exp.run_nofas          = True
+        self.surr_pre_it       = max_pre #:int: Number of pre-training iterations for surrogate model
+        self.surr_upd_it       = 6000   #:int: Number of iterations for the surrogate model update
+
         exp.annealing          = False
         exp.calibrate_interval = 200   # int: How often to update surrogate model (default 1000)
         exp.budget             = 1023  # int: Total number of true model evaluation
 
         exp.output_dir   = './results/' + exp.name
         exp.log_file     = 'log.txt'
         exp.seed         = random.randint(0, 10 ** 9)  # int: Random seed used
@@ -186,15 +194,15 @@
         # Define the surrogate
         exp.surrogate = Surrogate(exp.name, lambda x: model.solve_t(trsf.forward(x)), model.input_num, model.output_num,
                                   torch.Tensor([[-3.0, 3.0], [-3.0, 3.0], [-3.0, 3.0], [-3.0, 3.0], [-3.0, 3.0]]), 20, device=exp.device)
         if exp.run_nofas:
             if not os.path.isfile(exp.name + ".sur") or not os.path.isfile(exp.name + ".npz"):
                 print("Warning: Surrogate model files: {0}.npz and {0}.npz could not be found. ".format(exp.name))
                 exp.surrogate.gen_grid(gridnum=3)
-                exp.surrogate.pre_train(100000, 0.03, 0.9999, 500, store=True)
+                exp.surrogate.pre_train(self.surr_pre_it, 0.03, 0.9999, 500, store=True)
         exp.surrogate.surrogate_load()
 
         # Define the log density        
         def log_density(x, model, surrogate, transform):
 
             # Compute transformation log Jacobian
             adjust = transform.compute_log_jacob_func(x)
@@ -226,16 +234,18 @@
         exp.run()
 
 
     def rc_example(self):
 
         if "it" in os.environ:
           max_it  = int(os.environ["it"])
+          max_pre = 1000
         else:
           max_it  = 25001
+          max_pre = 40000
 
         print('')
         print('--- TEST 3: RC MODEL - NOFAS')
         print('')
 
         # Import model
         from linfa.models.circuitModels import rcModel
@@ -257,14 +267,17 @@
         # exp.n_iter        = 25001   # int: Number of iterations (default 25001)
         exp.n_iter        = max_it
         exp.lr            = 0.005   # float: Learning rate (default 0.003)
         exp.lr_decay      = 0.9999  # float: Learning rate decay (default 0.9999)
         exp.log_interval  = 10      # int: How often to show loss stat (default 10)
 
         exp.run_nofas          = True
+        self.surr_pre_it       = max_pre #:int: Number of pre-training iterations for surrogate model
+        self.surr_upd_it       = 6000  #:int: Number of iterations for the surrogate model update
+
         exp.annealing          = False
         exp.calibrate_interval = 1000  # int: How often to update surrogate model (default 1000)
         exp.budget             = 64    # int: Total number of true model evaluation
 
         exp.output_dir   = './results/' + exp.name
         exp.log_file     = 'log.txt'
         exp.seed         = random.randint(0, 10 ** 9)  # int: Random seed used
@@ -296,15 +309,15 @@
         # Define surrogate model
         exp.surrogate = Surrogate(exp.name, lambda x: model.solve_t(trsf.forward(x)), exp.input_size, 3,
                                   torch.Tensor([[-7, 7], [-7, 7]]), 20, device=exp.device)
         if exp.run_nofas:
             if not os.path.isfile(exp.name + ".sur") or not os.path.isfile(exp.name + ".npz"):
                 print("Warning: Surrogate model files: {0}.npz and {0}.npz could not be found. ".format(exp.name))
                 exp.surrogate.gen_grid(gridnum=4)
-                exp.surrogate.pre_train(40000, 0.03, 0.9999, 500, store=True)
+                exp.surrogate.pre_train(self.surr_pre_it, 0.03, 0.9999, 500, store=True)
         exp.surrogate.surrogate_load()
 
         # Define log density
         def log_density(x, model, surrogate, transform):
             
             # Compute transformation log Jacobian
             adjust = transform.compute_log_jacob_func(x)
@@ -336,16 +349,18 @@
         # Run VI
         exp.run()
 
     def rcr_example(self):
 
         if "it" in os.environ:
           max_it  = int(os.environ["it"])
+          max_pre = 1000
         else:
           max_it  = 25001
+          max_pre = 50000
 
         print('')
         print('--- TEST 4: RCR MODEL - NOFAS')
         print('')
 
         # Import rcr model
         from linfa.models.circuitModels import rcrModel
@@ -367,14 +382,17 @@
         # exp.n_iter        = 25001   # int: Number of iterations (default 25001)
         exp.n_iter        = max_it
         exp.lr            = 0.003   # float: Learning rate (default 0.003)
         exp.lr_decay      = 0.9999  # float: Learning rate decay (default 0.9999)
         exp.log_interval  = 10      # int: How often to show loss stat (default 10)
 
         exp.run_nofas          = True
+        self.surr_pre_it       = max_pre #:int: Number of pre-training iterations for surrogate model
+        self.surr_upd_it       = 6000  #:int: Number of iterations for the surrogate model update
+
         exp.annealing          = False
         exp.calibrate_interval = 300  # int: How often to update surrogate model (default 1000)
         exp.budget             = 216  # int: Total number of true model evaluation
 
         exp.output_dir = './results/' + exp.name
         exp.log_file = 'log.txt'
         exp.seed = random.randint(0, 10 ** 9)  # int: Random seed used
@@ -407,15 +425,15 @@
         # Define surrogate
         exp.surrogate = Surrogate(exp.name, lambda x: model.solve_t(trsf.forward(x)), exp.input_size, 3,
                                   torch.Tensor([[-7, 7], [-7, 7], [-7, 7]]), 20, device=exp.device)
         if exp.run_nofas:
             if not os.path.isfile(exp.name + ".sur") or not os.path.isfile(exp.name + ".npz"):
                 print("Warning: Surrogate model files: {0}.npz and {0}.npz could not be found. ".format(exp.name))
                 exp.surrogate.gen_grid(gridnum=4)
-                exp.surrogate.pre_train(50000, 0.03, 0.9999, 500, store=True)
+                exp.surrogate.pre_train(self.surr_pre_it, 0.03, 0.9999, 500, store=True)
         exp.surrogate.surrogate_load()
 
         # Define log density
         def log_density(x, model, surrogate, transform):
 
             # Compute transformation log Jacobian
             adjust = transform.compute_log_jacob_func(x)
@@ -457,24 +475,19 @@
           run_t0   = 0.99          
         else:
           run_T_1  = 10000
           run_T    = 3
           run_T_0  = 500
           run_t0   = 0.001          
 
-
         print('')
         print('--- TEST 5: FRIEDMAN 1 MODEL - ADAANN')
         print('')
 
         from linfa.run_experiment import experiment
-        import torch
-        import random
-        import numpy as np
-        import pandas as pd
 
         # Experiment Setting
         exp = experiment()
         exp.name              = "adaann"
         exp.flow_type         = 'realnvp'     # str: Type of flow (default 'realnvp')
         exp.n_blocks          = 10            # int: Number of layers (default 5)
         exp.hidden_size       = 20            # int: Hidden layer size for MADE in each layer (default 100)
@@ -516,16 +529,16 @@
         exp.seed         = random.randint(0, 10 ** 9)  # int: Random seed used
         exp.n_sample     = 5000                        # int: Batch size to generate final results/plots
         exp.no_cuda      = True                        # Running on CPU by default but tested on CUDA
 
         exp.device = torch.device('cuda:0' if torch.cuda.is_available() and not exp.no_cuda else 'cpu')
 
         # Model Setting
-        data_set = pd.read_csv('../resource/data/D1000.csv')
-        data = torch.tensor(data_set.values).to(exp.device)
+        data_set = np.loadtxt('../resource/data/D1000.csv',delimiter=',',skiprows=1)
+        data = torch.tensor(data_set).to(exp.device)
 
         def log_density(params, d):
 
             # Compute Model
             # Modified bimodal version of the Friedman model
             def targetPosterior(b, x):
                 return b[0] * torch.sin(np.pi * x[:, 0] * x[:, 1]) + \
```

