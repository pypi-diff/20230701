# Comparing `tmp/tensorlearn-1.1.8.tar.gz` & `tmp/tensorlearn-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorlearn-1.1.8.tar", last modified: Wed Feb 15 03:20:37 2023, max compression
+gzip compressed data, was "tensorlearn-1.1.9.tar", last modified: Wed Feb 15 05:59:08 2023, max compression
```

## Comparing `tensorlearn-1.1.8.tar` & `tensorlearn-1.1.9.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-02-15 03:20:37.872589 tensorlearn-1.1.8/
--rw-r--r--   0 ryan       (501) staff       (20)     1061 2022-11-17 10:04:43.000000 tensorlearn-1.1.8/LICENSE
--rw-r--r--   0 ryan       (501) staff       (20)     8338 2023-02-15 03:20:37.872211 tensorlearn-1.1.8/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)     7727 2022-12-04 04:47:53.000000 tensorlearn-1.1.8/README.md
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-02-15 03:20:37.872750 tensorlearn-1.1.8/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)     2087 2023-02-15 03:17:47.000000 tensorlearn-1.1.8/setup.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-02-15 03:20:37.862970 tensorlearn-1.1.8/tensorlearn/
--rw-r--r--   0 ryan       (501) staff       (20)     1395 2023-02-08 00:10:39.000000 tensorlearn-1.1.8/tensorlearn/__init__.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-02-15 03:20:37.867651 tensorlearn-1.1.8/tensorlearn/decomposition/
--rw-r--r--   0 ryan       (501) staff       (20)     1100 2022-11-17 10:04:13.000000 tensorlearn-1.1.8/tensorlearn/decomposition/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     2042 2022-11-20 00:09:51.000000 tensorlearn-1.1.8/tensorlearn/decomposition/candecomp_parafac.py
--rw-r--r--   0 ryan       (501) staff       (20)     2899 2023-02-15 03:18:14.000000 tensorlearn-1.1.8/tensorlearn/decomposition/tensor_train.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-02-15 03:20:37.870366 tensorlearn-1.1.8/tensorlearn/operations/
--rw-r--r--   0 ryan       (501) staff       (20)     1127 2022-11-17 10:04:02.000000 tensorlearn-1.1.8/tensorlearn/operations/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     1896 2022-11-18 22:05:17.000000 tensorlearn-1.1.8/tensorlearn/operations/matrix_operations.py
--rw-r--r--   0 ryan       (501) staff       (20)     5648 2023-02-08 03:50:09.000000 tensorlearn-1.1.8/tensorlearn/operations/tensor_operations.py
--rw-r--r--   0 ryan       (501) staff       (20)     1828 2023-02-08 00:18:39.000000 tensorlearn-1.1.8/tensorlearn/tl_methods.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-02-15 03:20:37.865226 tensorlearn-1.1.8/tensorlearn.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)     8338 2023-02-15 03:20:37.000000 tensorlearn-1.1.8/tensorlearn.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      516 2023-02-15 03:20:37.000000 tensorlearn-1.1.8/tensorlearn.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-02-15 03:20:37.000000 tensorlearn-1.1.8/tensorlearn.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)        6 2023-02-15 03:20:37.000000 tensorlearn-1.1.8/tensorlearn.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)       12 2023-02-15 03:20:37.000000 tensorlearn-1.1.8/tensorlearn.egg-info/top_level.txt
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-02-15 03:20:37.871349 tensorlearn-1.1.8/tests/
--rw-r--r--   0 ryan       (501) staff       (20)      152 2022-11-17 03:13:25.000000 tensorlearn-1.1.8/tests/test_1.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-02-15 05:59:08.457554 tensorlearn-1.1.9/
+-rw-r--r--   0 ryan       (501) staff       (20)     1061 2022-11-17 10:04:43.000000 tensorlearn-1.1.9/LICENSE
+-rw-r--r--   0 ryan       (501) staff       (20)     8338 2023-02-15 05:59:08.457144 tensorlearn-1.1.9/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)     7727 2022-12-04 04:47:53.000000 tensorlearn-1.1.9/README.md
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-02-15 05:59:08.457694 tensorlearn-1.1.9/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)     2087 2023-02-15 05:58:31.000000 tensorlearn-1.1.9/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-02-15 05:59:08.447842 tensorlearn-1.1.9/tensorlearn/
+-rw-r--r--   0 ryan       (501) staff       (20)     1453 2023-02-15 05:47:45.000000 tensorlearn-1.1.9/tensorlearn/__init__.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-02-15 05:59:08.453197 tensorlearn-1.1.9/tensorlearn/decomposition/
+-rw-r--r--   0 ryan       (501) staff       (20)     1100 2022-11-17 10:04:13.000000 tensorlearn-1.1.9/tensorlearn/decomposition/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     2042 2022-11-20 00:09:51.000000 tensorlearn-1.1.9/tensorlearn/decomposition/candecomp_parafac.py
+-rw-r--r--   0 ryan       (501) staff       (20)     2899 2023-02-15 05:47:56.000000 tensorlearn-1.1.9/tensorlearn/decomposition/tensor_train.py
+-rw-r--r--   0 ryan       (501) staff       (20)      940 2023-02-15 05:27:27.000000 tensorlearn-1.1.9/tensorlearn/decomposition/tucker.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-02-15 05:59:08.455674 tensorlearn-1.1.9/tensorlearn/operations/
+-rw-r--r--   0 ryan       (501) staff       (20)     1127 2022-11-17 10:04:02.000000 tensorlearn-1.1.9/tensorlearn/operations/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     1896 2022-11-18 22:05:17.000000 tensorlearn-1.1.9/tensorlearn/operations/matrix_operations.py
+-rw-r--r--   0 ryan       (501) staff       (20)     6901 2023-02-15 05:35:14.000000 tensorlearn-1.1.9/tensorlearn/operations/tensor_operations.py
+-rw-r--r--   0 ryan       (501) staff       (20)     2230 2023-02-15 05:47:51.000000 tensorlearn-1.1.9/tensorlearn/tl_methods.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-02-15 05:59:08.450395 tensorlearn-1.1.9/tensorlearn.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)     8338 2023-02-15 05:59:08.000000 tensorlearn-1.1.9/tensorlearn.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      552 2023-02-15 05:59:08.000000 tensorlearn-1.1.9/tensorlearn.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-02-15 05:59:08.000000 tensorlearn-1.1.9/tensorlearn.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        6 2023-02-15 05:59:08.000000 tensorlearn-1.1.9/tensorlearn.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       12 2023-02-15 05:59:08.000000 tensorlearn-1.1.9/tensorlearn.egg-info/top_level.txt
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-02-15 05:59:08.456274 tensorlearn-1.1.9/tests/
+-rw-r--r--   0 ryan       (501) staff       (20)      152 2022-11-17 03:13:25.000000 tensorlearn-1.1.9/tests/test_1.py
```

### Comparing `tensorlearn-1.1.8/LICENSE` & `tensorlearn-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorlearn-1.1.8/PKG-INFO` & `tensorlearn-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorlearn
-Version: 1.1.8
+Version: 1.1.9
 Summary: A Python Package for Advanced Tensor Learning Methods
 Home-page: https://github.com/rmsolgi/tensorlearn.git
 Author: Ryan Solgi
 Author-email: ryan.solgi@gmail.com
 Maintainer: Ryan Solgi
 Keywords: tensor,decomposition,tensor-train,rank,auto-rank,CANDECOMP,PARAFAC,CP
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tensorlearn-1.1.8/README.md` & `tensorlearn-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `tensorlearn-1.1.8/setup.py` & `tensorlearn-1.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tensorlearn", 
-    version="1.1.8",
+    version="1.1.9",
     author="Ryan Solgi",
     author_email="ryan.solgi@gmail.com",
     maintainer='Ryan Solgi',
     description="A Python Package for Advanced Tensor Learning Methods",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rmsolgi/tensorlearn.git",
```

### Comparing `tensorlearn-1.1.8/tensorlearn/__init__.py` & `tensorlearn-1.1.9/tensorlearn/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE 
 SOFTWARE.
 '''
 
 from . import decomposition
 from . import operations
 from . import tl_methods
-from .tl_methods import auto_rank_tt, unfold, mode_n_product, tt_to_tensor, tensor_resize, tensor_frobenius_norm, error_truncated_svd, tt_compression_ratio, cp_als_rand_init, cp_to_tensor, cp_compression_ratio, column_wise_kronecker
+from .tl_methods import auto_rank_tt, unfold, mode_n_product, tt_to_tensor, tensor_resize, tensor_frobenius_norm, error_truncated_svd, tt_compression_ratio, cp_als_rand_init, cp_to_tensor, cp_compression_ratio, column_wise_kronecker, tucker_hosvd, tucker_to_tensor, tucker_compression_ratio
```

### Comparing `tensorlearn-1.1.8/tensorlearn/decomposition/__init__.py` & `tensorlearn-1.1.9/tensorlearn/decomposition/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorlearn-1.1.8/tensorlearn/decomposition/candecomp_parafac.py` & `tensorlearn-1.1.9/tensorlearn/decomposition/candecomp_parafac.py`

 * *Files identical despite different names*

### Comparing `tensorlearn-1.1.8/tensorlearn/decomposition/tensor_train.py` & `tensorlearn-1.1.9/tensorlearn/decomposition/tensor_train.py`

 * *Files identical despite different names*

### Comparing `tensorlearn-1.1.8/tensorlearn/operations/__init__.py` & `tensorlearn-1.1.9/tensorlearn/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorlearn-1.1.8/tensorlearn/operations/matrix_operations.py` & `tensorlearn-1.1.9/tensorlearn/operations/matrix_operations.py`

 * *Files identical despite different names*

### Comparing `tensorlearn-1.1.8/tensorlearn/operations/tensor_operations.py` & `tensorlearn-1.1.9/tensorlearn/operations/tensor_operations.py`

 * *Files 17% similar despite different names*

```diff
@@ -166,17 +166,59 @@
     t_shape_array=np.array(t_shape)
     
     tensor_size=np.prod(t_shape_array)
     
     compression_ratio=tensor_size/factors_size
     
     return compression_ratio    
+
+
+    ###################### Tucker tensor shape
+    ###################### ###################### ###################### ###################
+
+
+def tucker_tensor_shape(factor_matrices):
+    
+    t_shape=[f.shape[0] for f in factor_matrices]
+    
+    return t_shape
+
+
+    ###################### Tuckers factors to tensor
+    ###################### ###################### ###################### ###################
+
+
+def tucker_to_tensor(core_factor,factor_matrices):
     
     
+    tensor=core_factor
+    counter=0
+    for factor in factor_matrices:
+        tensor=tensor_operations.mode_n_product(tensor,factor,counter)
+        counter+=1
+    return tensor    
+    
+    ###################### Tucker Compression Ratio ccounting lambda (weights) too
+    ###################### ###################### ###################### ######################      
+def tucker_compression_ratio(core_factor,factor_matrices):
 
+    
+    factors_size=core_factor.size
+    for item in factor_matrices:
+        factors_size+=item.size
+        
+    t_shape=tensor_operations.tucker_tensor_shape(factor_matrices)
+    
+    t_shape_array=np.array(t_shape)
+    
+    tensor_size=np.prod(t_shape_array)
+    
+    compression_ratio=tensor_size/factors_size
+    
+    return compression_ratio
```

### Comparing `tensorlearn-1.1.8/tensorlearn/tl_methods.py` & `tensorlearn-1.1.9/tensorlearn/tl_methods.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 
     
 
 from tensorlearn.decomposition import tensor_train
 from tensorlearn.decomposition import candecomp_parafac
+from tensorlearn.decomposition import tucker
 from tensorlearn.operations import tensor_operations as top
 from tensorlearn.operations import matrix_operations as mop
 
 
 ############################################################
 ############################################################
 #####               decompositions
 def auto_rank_tt(tensor,epsilon):
     return tensor_train.auto_rank_tt(tensor,epsilon)
     
 def cp_als_rand_init(tensor, rank, iteration, random_seed=None):
     return candecomp_parafac.cp_als_rand_init(tensor, rank, iteration, random_seed)
     
+def tucker_hosvd(tensor, epsilon):
+    return tucker.tucker_hosvd(tensor, epsilon)
+    
 ############################################################
 ############################################################
 ####               tensor operations
 
 #### TT
 def tt_to_tensor(factors):
     return top.tt_to_tensor(factors)
@@ -45,14 +49,25 @@
 ### CP
 
 def cp_to_tensor(weights, factors):
     return top.cp_to_tensor(weights, factors)
     
 def cp_compression_ratio(weights, factors):
     return top.cp_compression_ratio(weights,factors)
+    
+    
+### Tucker
+
+def tucker_to_tensor(core_factor,factor_matrices):
+    return top.tucker_to_tensor(core_factor,factor_matrices)
+
+def tucker_compression_ratio(core_factor,factor_matrices):
+    return top.tucker_compression_ratio(core_factor,factor_matrices)
+    
+
 
 ############################################################
 ############################################################
 ######              matrix operations
 
 def error_truncated_svd(x, error):
     return mop.error_truncated_svd(x,error)
```

### Comparing `tensorlearn-1.1.8/tensorlearn.egg-info/PKG-INFO` & `tensorlearn-1.1.9/tensorlearn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorlearn
-Version: 1.1.8
+Version: 1.1.9
 Summary: A Python Package for Advanced Tensor Learning Methods
 Home-page: https://github.com/rmsolgi/tensorlearn.git
 Author: Ryan Solgi
 Author-email: ryan.solgi@gmail.com
 Maintainer: Ryan Solgi
 Keywords: tensor,decomposition,tensor-train,rank,auto-rank,CANDECOMP,PARAFAC,CP
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tensorlearn-1.1.8/tensorlearn.egg-info/SOURCES.txt` & `tensorlearn-1.1.9/tensorlearn.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -7,11 +7,12 @@
 tensorlearn.egg-info/SOURCES.txt
 tensorlearn.egg-info/dependency_links.txt
 tensorlearn.egg-info/requires.txt
 tensorlearn.egg-info/top_level.txt
 tensorlearn/decomposition/__init__.py
 tensorlearn/decomposition/candecomp_parafac.py
 tensorlearn/decomposition/tensor_train.py
+tensorlearn/decomposition/tucker.py
 tensorlearn/operations/__init__.py
 tensorlearn/operations/matrix_operations.py
 tensorlearn/operations/tensor_operations.py
 tests/test_1.py
```

