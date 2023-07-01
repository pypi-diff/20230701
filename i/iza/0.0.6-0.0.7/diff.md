# Comparing `tmp/iza-0.0.6.tar.gz` & `tmp/iza-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iza-0.0.6.tar", last modified: Tue Jun 27 21:51:41 2023, max compression
+gzip compressed data, was "iza-0.0.7.tar", last modified: Sat Jul  1 14:54:34 2023, max compression
```

## Comparing `iza-0.0.6.tar` & `iza-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 21:51:41.388938 iza-0.0.6/
--rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 iza-0.0.6/LICENSE
--rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 iza-0.0.6/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     1969 2023-06-27 21:51:41.388823 iza-0.0.6/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     1348 2023-06-24 20:51:36.000000 iza-0.0.6/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 21:51:41.387495 iza-0.0.6/iza/
--rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-27 21:51:25.000000 iza-0.0.6/iza/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)    20748 2023-06-27 21:51:25.000000 iza-0.0.6/iza/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     2046 2023-06-27 21:51:25.000000 iza-0.0.6/iza/commands.py
--rw-r--r--   0 solst      (501) staff       (20)     2264 2023-06-27 21:51:25.000000 iza-0.0.6/iza/imp.py
--rw-r--r--   0 solst      (501) staff       (20)    14824 2023-06-27 21:51:25.000000 iza-0.0.6/iza/nbs.py
--rw-r--r--   0 solst      (501) staff       (20)     4983 2023-06-27 21:51:25.000000 iza-0.0.6/iza/plots.py
--rw-r--r--   0 solst      (501) staff       (20)      448 2023-06-27 21:51:25.000000 iza-0.0.6/iza/rich.py
--rw-r--r--   0 solst      (501) staff       (20)     8171 2023-06-27 21:51:25.000000 iza-0.0.6/iza/static.py
--rw-r--r--   0 solst      (501) staff       (20)      191 2023-06-27 21:51:25.000000 iza-0.0.6/iza/typer.py
--rw-r--r--   0 solst      (501) staff       (20)     4383 2023-06-27 21:51:25.000000 iza-0.0.6/iza/types.py
--rw-r--r--   0 solst      (501) staff       (20)    54404 2023-06-27 21:51:25.000000 iza-0.0.6/iza/utils.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-27 21:51:41.388635 iza-0.0.6/iza.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     1969 2023-06-27 21:51:41.000000 iza-0.0.6/iza.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      388 2023-06-27 21:51:41.000000 iza-0.0.6/iza.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-27 21:51:41.000000 iza-0.0.6/iza.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       70 2023-06-27 21:51:41.000000 iza-0.0.6/iza.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-24 20:04:21.000000 iza-0.0.6/iza.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)       75 2023-06-27 21:51:41.000000 iza-0.0.6/iza.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        4 2023-06-27 21:51:41.000000 iza-0.0.6/iza.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      900 2023-06-27 21:49:34.000000 iza-0.0.6/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-27 21:51:41.388977 iza-0.0.6/setup.cfg
--rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-06-27 21:50:00.000000 iza-0.0.6/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-07-01 14:54:34.453100 iza-0.0.7/
+-rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 iza-0.0.7/LICENSE
+-rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 iza-0.0.7/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     1969 2023-07-01 14:54:34.452969 iza-0.0.7/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     1348 2023-06-24 20:51:36.000000 iza-0.0.7/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-07-01 14:54:34.451694 iza-0.0.7/iza/
+-rw-r--r--   0 solst      (501) staff       (20)       22 2023-07-01 14:53:52.000000 iza-0.0.7/iza/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)    20856 2023-07-01 14:53:52.000000 iza-0.0.7/iza/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     2046 2023-07-01 14:53:52.000000 iza-0.0.7/iza/commands.py
+-rw-r--r--   0 solst      (501) staff       (20)     2264 2023-07-01 14:53:52.000000 iza-0.0.7/iza/imp.py
+-rw-r--r--   0 solst      (501) staff       (20)    14824 2023-07-01 14:53:52.000000 iza-0.0.7/iza/nbs.py
+-rw-r--r--   0 solst      (501) staff       (20)     4983 2023-07-01 14:53:52.000000 iza-0.0.7/iza/plots.py
+-rw-r--r--   0 solst      (501) staff       (20)      448 2023-07-01 14:53:52.000000 iza-0.0.7/iza/rich.py
+-rw-r--r--   0 solst      (501) staff       (20)     8199 2023-07-01 14:53:52.000000 iza-0.0.7/iza/static.py
+-rw-r--r--   0 solst      (501) staff       (20)      191 2023-07-01 14:53:52.000000 iza-0.0.7/iza/typer.py
+-rw-r--r--   0 solst      (501) staff       (20)     4395 2023-07-01 14:53:52.000000 iza-0.0.7/iza/types.py
+-rw-r--r--   0 solst      (501) staff       (20)    54797 2023-07-01 14:53:52.000000 iza-0.0.7/iza/utils.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-07-01 14:54:34.452751 iza-0.0.7/iza.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     1969 2023-07-01 14:54:34.000000 iza-0.0.7/iza.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      388 2023-07-01 14:54:34.000000 iza-0.0.7/iza.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-07-01 14:54:34.000000 iza-0.0.7/iza.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       70 2023-07-01 14:54:34.000000 iza-0.0.7/iza.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-24 20:04:21.000000 iza-0.0.7/iza.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)       80 2023-07-01 14:54:34.000000 iza-0.0.7/iza.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        4 2023-07-01 14:54:34.000000 iza-0.0.7/iza.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      905 2023-07-01 14:53:49.000000 iza-0.0.7/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-07-01 14:54:34.453143 iza-0.0.7/setup.cfg
+-rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-06-27 21:50:00.000000 iza-0.0.7/setup.py
```

### Comparing `iza-0.0.6/LICENSE` & `iza-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `iza-0.0.6/PKG-INFO` & `iza-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iza
-Version: 0.0.6
+Version: 0.0.7
 Summary: chaos package of utilities; a nod to izalith
 Home-page: https://github.com/dsm-72/iza
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `iza-0.0.6/README.md` & `iza-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `iza-0.0.6/iza/_modidx.py` & `iza-0.0.7/iza/_modidx.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,14 +127,15 @@
                            'iza.utils.allsametype': ('utils.html#allsametype', 'iza/utils.py'),
                            'iza.utils.arein': ('utils.html#arein', 'iza/utils.py'),
                            'iza.utils.base_entry_fn': ('utils.html#base_entry_fn', 'iza/utils.py'),
                            'iza.utils.base_init_tree': ('utils.html#base_init_tree', 'iza/utils.py'),
                            'iza.utils.check_ext': ('utils.html#check_ext', 'iza/utils.py'),
                            'iza.utils.collapse_user': ('utils.html#collapse_user', 'iza/utils.py'),
                            'iza.utils.config_exp_logger': ('utils.html#config_exp_logger', 'iza/utils.py'),
+                           'iza.utils.copy_to_clipboard': ('utils.html#copy_to_clipboard', 'iza/utils.py'),
                            'iza.utils.decompress_directory_of_gunzipped_files': ( 'utils.html#decompress_directory_of_gunzipped_files',
                                                                                   'iza/utils.py'),
                            'iza.utils.decompress_gunzip': ('utils.html#decompress_gunzip', 'iza/utils.py'),
                            'iza.utils.decompress_tarball': ('utils.html#decompress_tarball', 'iza/utils.py'),
                            'iza.utils.decompress_tarball_of_gunzipped_files': ( 'utils.html#decompress_tarball_of_gunzipped_files',
                                                                                 'iza/utils.py'),
                            'iza.utils.dir_dirs': ('utils.html#dir_dirs', 'iza/utils.py'),
```

### Comparing `iza-0.0.6/iza/commands.py` & `iza-0.0.7/iza/commands.py`

 * *Files identical despite different names*

### Comparing `iza-0.0.6/iza/imp.py` & `iza-0.0.7/iza/imp.py`

 * *Files identical despite different names*

### Comparing `iza-0.0.6/iza/nbs.py` & `iza-0.0.7/iza/nbs.py`

 * *Files identical despite different names*

### Comparing `iza-0.0.6/iza/plots.py` & `iza-0.0.7/iza/plots.py`

 * *Files identical despite different names*

### Comparing `iza-0.0.6/iza/static.py` & `iza-0.0.7/iza/static.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/01_static.ipynb.
 
 # %% auto 0
 __all__ = ['NBKS_DIR', 'ROOT_DIR', 'EXPL_DIR', 'DATA_DIR', 'RESULTS_DIR', 'FIGURES_DIR', 'IZALITH_DATA_DIR', 'GIBBS_DATA_DIR',
            'PERIOD', 'GZ', 'H5', 'CSV', 'MTX', 'TAR', 'TSV', 'PY', 'NPY', 'NPZ', 'TXT', 'JSON', 'ZIP', 'IPYNB',
            'EXT_GZ', 'EXT_H5', 'EXT_CSV', 'EXT_MTX', 'EXT_TAR', 'EXT_TSV', 'EXT_TAR_GZ', 'EXT_PY', 'EXT_NPY', 'EXT_NPZ',
-           'EXT_TXT', 'EXT_JSON', 'EXT_ZIP', 'EXT_IPYNB', 'SEED', 'ITEM', 'TIME', 'LABEL', 'SERIES', 'SAMPLES',
-           'CONDITION', 'CONDITIONS', 'HVG', 'PCA', 'UMAP', 'TSNE', 'PHATE', 'MAGIC', 'CELL', 'BARCODE', 'BARCODES',
-           'ID', 'MITO', 'RIBO', 'GENE', 'GENE_ID', 'GENE_IDS', 'GENE_SYMBOL', 'HIGHLY_VARIABLE', 'ENSEMBL',
+           'EXT_TXT', 'EXT_JSON', 'EXT_ZIP', 'EXT_IPYNB', 'SEED', 'ITEM', 'TIME', 'LABEL', 'SERIES', 'SAMPLE',
+           'SAMPLES', 'CONDITION', 'CONDITIONS', 'HVG', 'PCA', 'UMAP', 'TSNE', 'PHATE', 'MAGIC', 'CELL', 'BARCODE',
+           'BARCODES', 'ID', 'MITO', 'RIBO', 'GENE', 'GENE_ID', 'GENE_IDS', 'GENE_SYMBOL', 'HIGHLY_VARIABLE', 'ENSEMBL',
            'ENSEMBL_ID', 'HUMAN', 'MOUSE', 'HUMAN_TF', 'MOUSE_TF', 'HUMAN_GENE_SYMBOL', 'HUMAN_ENSEMBLE_ID',
            'MOUSE_ENSEMBLE_ID', 'BATCH', 'TIMEPOINT', 'TOTAL_COUNTS', 'DOUBLET', 'DOUBLET_SCORES', 'PREDICTED_DOUBLETS',
            'PRENORM', 'DETECTED', 'SCALED_NORMALIZED', 'COUNTS', 'PCT', 'PERCENT', 'PCT_COUNTS', 'PCT_COUNTS_MITO',
            'PCT_COUNTS_RIBO', 'X', 'X_', 'X_PRENORM', 'X_DETECTED', 'X_SCALED_NORMALIZED', 'X_MAGIC', 'X_PCA',
            'X_PCA_HVG', 'X_PHATE', 'X_PHATE_HVG', 'ADATA', 'MATRIX', 'FEATURES', 'SENSITIVITY',
            'AMAZON_BUCKET_FLUENTBIO', 'LINEAGE_ESC', 'LINEAGE_PREGERM', 'LINEAGE_NEURAL_CREST', 'LINEAGE_NEURAL_PROG',
            'LINEAGE_ENDO', 'LINEAGE_MESO', 'LINEAGE_CARDIAC', 'LINEAGE_HEMA', 'LINEAGE_SOMITES', 'LINEAGE_TROPHOBLAST',
@@ -84,14 +84,15 @@
 
 # %% ../nbs/01_static.ipynb 15
 SEED = 'seed'
 ITEM = 'item'
 TIME = 'time'
 LABEL = 'label'
 SERIES = 'series'
+SAMPLE = 'sample'
 SAMPLES = 'samples'
 CONDITION = 'condition'
 CONDITIONS = f'{CONDITION}s'
 
 # %% ../nbs/01_static.ipynb 19
 HVG = 'hvg'
```

### Comparing `iza-0.0.6/iza/types.py` & `iza-0.0.7/iza/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 # %% ../nbs/03_types.ipynb 6
 import numpy as np, pandas as pd
 import pathlib
 
 # %% ../nbs/03_types.ipynb 9
 try:
     import torch
-    Tensor:TypeAlias = torch.Tensor
+    Tensor: TypeAlias = torch.Tensor
     Device: TypeAlias = torch.device
 except ImportError:
     # Define a placeholder type if torch is not installed
-    Tensor = Union[Iterable[Number], Any]
+    Tensor: TypeAlias = Union[Iterable[Number], Any]
     Device: TypeAlias = Union[str, None, Any]
     pass
 
 # %% ../nbs/03_types.ipynb 11
 try:
     import anndata as ad    
     AnnData: TypeAlias = ad.AnnData
```

### Comparing `iza-0.0.6/iza/utils.py` & `iza-0.0.7/iza/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/02_utils.ipynb.
 
 # %% auto 0
 __all__ = ['DecompressFunc', 'isiter', 'allinstance', 'allsametype', 'isin', 'arein', 'str_just_alpha', 'str_just_numeric',
            'strip_punc', 'filter_kwargs_for_func', 'filter_kwargs_for_class', 'wrangle_kwargs_for_func',
-           'wrangle_kwargs_for_class', 'is_pathlib', 'is_pathlike', 'is_path', 'str_to_path', 'path_to_str',
-           'to_abs_expanded', 'sort_file_first', 'sort_directory_first', 'get_user', 'collapse_user', 'check_ext',
-           'drop_ext', 'is_tar', 'is_gz', 'is_targz', 'is_tarball', 'filter_for_gz_files', 'get_gz_files_in_dir',
-           'decompress_tarball', 'decompress_gunzip', 'undo_gz', 'RecursiveDecompressor', 'make_missing_dirs',
-           'dir_dirs', 'decompress_directory_of_gunzipped_files', 'decompress_tarball_of_gunzipped_files',
-           'stream_file', 'download_and_decompress_tarball_of_gunzipped_files', 'make_temp_file', 'urljoin', 'Slice',
-           'base_init_tree', 'rich_init_tree', 'init_tree', 'base_entry_fn', 'rich_entry_fn', 'entry_fn',
-           'walk_dir_tree', 'DirectoryTree', 'RichDirectory', 'Directory', 'is_matrix', 'undo_npmatrix', 'is_series',
-           'is_series_like', 'is_np', 'is_device', 'is_cpu', 'is_mps', 'is_tensor', 'is_torch', 'undo_sparse',
-           'to_ndarray', 'AdataExtractor', 'config_exp_logger', 'exp_log_filename', 'exp_param_filename', 'list_exps',
-           'gen_exp_name', 'load_exp_params', 'save_exp_params', 'setup_exp', 'is_config_subset', 'find_exps',
-           'ArchiveDownloader']
+           'wrangle_kwargs_for_class', 'copy_to_clipboard', 'is_pathlib', 'is_pathlike', 'is_path', 'str_to_path',
+           'path_to_str', 'to_abs_expanded', 'sort_file_first', 'sort_directory_first', 'get_user', 'collapse_user',
+           'check_ext', 'drop_ext', 'is_tar', 'is_gz', 'is_targz', 'is_tarball', 'filter_for_gz_files',
+           'get_gz_files_in_dir', 'decompress_tarball', 'decompress_gunzip', 'undo_gz', 'RecursiveDecompressor',
+           'make_missing_dirs', 'dir_dirs', 'decompress_directory_of_gunzipped_files',
+           'decompress_tarball_of_gunzipped_files', 'stream_file', 'download_and_decompress_tarball_of_gunzipped_files',
+           'make_temp_file', 'urljoin', 'Slice', 'base_init_tree', 'rich_init_tree', 'init_tree', 'base_entry_fn',
+           'rich_entry_fn', 'entry_fn', 'walk_dir_tree', 'DirectoryTree', 'RichDirectory', 'Directory', 'is_matrix',
+           'undo_npmatrix', 'is_series', 'is_series_like', 'is_np', 'is_device', 'is_cpu', 'is_mps', 'is_tensor',
+           'is_torch', 'undo_sparse', 'to_ndarray', 'AdataExtractor', 'config_exp_logger', 'exp_log_filename',
+           'exp_param_filename', 'list_exps', 'gen_exp_name', 'load_exp_params', 'save_exp_params', 'setup_exp',
+           'is_config_subset', 'find_exps', 'ArchiveDownloader']
 
 # %% ../nbs/02_utils.ipynb 5
-import inspect, string
+import os, inspect, string
 from dataclasses import dataclass, field
 
 import numpy as np, pandas as pd
 
 from typing import List, Any, Optional, Callable, Union, Tuple, Iterable, Set, TypeAlias, Type
 
 # %% ../nbs/02_utils.ipynb 7
@@ -85,32 +85,49 @@
     params = (defaults or {}).copy()
     # update with kwargs of our class
     params.update(kwargs or {})
     # filter for only the params that other class accepts
     params = filter_kwargs_for_class(cls, **params)
     return params
 
-# %% ../nbs/02_utils.ipynb 12
+# %% ../nbs/02_utils.ipynb 11
+def copy_to_clipboard(text: str):
+    command = ""
+    
+    # macOS and Linux
+    if os.name == 'posix':  
+        command = 'echo "' + text + '" | pbcopy'
+    
+    # Windows
+    elif os.name == 'nt':  
+        command = 'echo ' + text + ' | clip'
+
+    else:
+        raise OSError("Unsupported operating system")
+
+    os.system(command)
+
+# %% ../nbs/02_utils.ipynb 13
 import os, sys, pwd, atexit, tempfile, inspect, pathlib
 import requests, tarfile, gzip, shutil
 from dataclasses import dataclass, field
 from tqdm.auto import tqdm
 
 from typing import Optional, List, Union, Iterable, Tuple, Any, Callable
 
-# %% ../nbs/02_utils.ipynb 13
+# %% ../nbs/02_utils.ipynb 14
 from iza.static import (
     EXT_GZ, EXT_TAR, EXT_TAR_GZ,
 )
 
 from iza.types import (
     PathType, PathLike
 )
 
-# %% ../nbs/02_utils.ipynb 15
+# %% ../nbs/02_utils.ipynb 16
 def is_pathlib(path:Any) -> bool:
     """Check if the input is a path"""
     return isinstance(path, PathType)
 
 def is_pathlike(path:Any) -> bool:
     """Check if the input is a path"""
     return isinstance(path, (PathLike))
@@ -143,24 +160,24 @@
 def sort_file_first(path: PathType):
     return (not path.is_file(), path.name.lower())
 
 def sort_directory_first(path: PathType):
     return (path.is_file(), path.name.lower())
 
 
-# %% ../nbs/02_utils.ipynb 17
+# %% ../nbs/02_utils.ipynb 18
 def get_user() -> str:
     user = pwd.getpwuid(os.getuid())[0]
     return user
 
 def collapse_user(path: str) -> str:
     _, rest = path.split(get_user())    
     return '~' + rest
 
-# %% ../nbs/02_utils.ipynb 19
+# %% ../nbs/02_utils.ipynb 20
 def check_ext(filename:str, extension:str) -> bool:
     if is_pathlib(filename):
         filename = path_to_str(filename)
     has_extension = extension in filename 
     splits = filename.split(extension)
     is_end_of_str = len(splits) >= 2 and splits[-1] == ''
     is_end_of_str = filename.endswith(extension)
@@ -173,43 +190,43 @@
     file = os.path.basename(filename)
     if extension is None:
         file, *_ = file.split('.')
     else:
         file = filename.replace(extension, '')
     return os.path.join(os.path.dirname(filename), file)
 
-# %% ../nbs/02_utils.ipynb 20
+# %% ../nbs/02_utils.ipynb 21
 def is_tar(filename:str) -> bool:
     return check_ext(filename, EXT_TAR)
 
 def is_gz(filename:str) -> bool:
     return check_ext(filename, EXT_GZ)
 
 def is_targz(filename:str) -> bool:
     return check_ext(filename, EXT_TAR_GZ)
 
 def is_tarball(filename:str) -> bool:
     return is_tar(filename) or is_targz(filename)
 
 
-# %% ../nbs/02_utils.ipynb 21
+# %% ../nbs/02_utils.ipynb 22
 def filter_for_gz_files(files:List[str]) -> List[str]:
     return list(filter(lambda f: is_gz(f), files))
 
 def get_gz_files_in_dir(dirname:str) -> List[str]:
     all_files = []
 
     for (root, dirs, files) in os.walk(dirname):   
         fullpaths = [os.path.join(root, file) for file in files]
         all_files.extend(fullpaths)
     
     gz_files = filter_for_gz_files(all_files)
     return gz_files
 
-# %% ../nbs/02_utils.ipynb 23
+# %% ../nbs/02_utils.ipynb 24
 def decompress_tarball(filename:str, remove:bool=False) -> Tuple[str, Optional[EOFError]]:
     '''
     Returns
     -------
         dirname : str
             The name of the archive e.g. `~/Downloads/fluentbio.tar.gz` would
             yield `~/Downloads/fluentbio`
@@ -274,15 +291,15 @@
         filename, _ = decompress_gunzip(filename, remove)
     elif is_tar(filename):
         pass
     elif is_tarball(filename):
         filename, _ = decompress_tarball(filename, remove)
     return filename
 
-# %% ../nbs/02_utils.ipynb 24
+# %% ../nbs/02_utils.ipynb 25
 DecompressFunc = Callable[[str, bool], str]
 
 @dataclass
 class RecursiveDecompressor:
     dirname: PathType
     entries: Optional[List[str]] = field(default_factory=list, repr=False)
     strategy: Optional[DecompressFunc] = field(default=undo_gz, repr=False)
@@ -352,15 +369,15 @@
                     
         elif self.remove:
             if filename in self.entries:
                 self.entries.remove(filename)
             self.decrease_total()
 
 
-# %% ../nbs/02_utils.ipynb 26
+# %% ../nbs/02_utils.ipynb 27
 def make_missing_dirs(dirs:List[str]):
     if isinstance(dirs, str):
         dirs = [dirs]
         
     elif is_pathlib(dirs):
         dirs = [dirs]
         
@@ -369,15 +386,15 @@
             os.makedirs(d)
             
 def dir_dirs(dirname:str) -> List[str]:
     entries = os.listdir(dirname)
     is_subdir = lambda e : os.path.isdir(os.path.join(dirname, e))
     return list(filter(is_subdir, entries))
 
-# %% ../nbs/02_utils.ipynb 27
+# %% ../nbs/02_utils.ipynb 28
 def decompress_directory_of_gunzipped_files(
     dirname:str, desc:Optional[str]=None, remove:Optional[bool]=False
 ) -> None:
     if desc is None:
         desc = dirname.split('/')[-1]
 
     gz_files = get_gz_files_in_dir(dirname)
@@ -393,15 +410,15 @@
 
     if desc is None:
         desc = dirname.split('/')[-1]
 
     # NOTE: decompress all internal .gz files
     decompress_directory_of_gunzipped_files(dirname, desc, remove)
 
-# %% ../nbs/02_utils.ipynb 29
+# %% ../nbs/02_utils.ipynb 30
 def stream_file(uri:str, filename:Optional[str]=None, desc:Optional[str]=None) -> None:
     '''
     Parameters
     ----------
     uri : str
         The URI to download
 
@@ -427,15 +444,15 @@
     with tqdm.wrapattr(
         open(filename, 'wb'), 'write', 
         miniters=1, desc=desc, total=total
     ) as fout:
         for chunk in response.iter_content(chunk_size=4096):
             fout.write(chunk)
 
-# %% ../nbs/02_utils.ipynb 31
+# %% ../nbs/02_utils.ipynb 32
 def download_and_decompress_tarball_of_gunzipped_files(
     uri:str, download_dir:str=None, desc:Optional[str]=None, remove:Optional[bool]=False
 ):
     filename = os.path.basename(uri)
     fullpath = os.path.join(download_dir, filename)
 
     if desc is None:
@@ -447,36 +464,36 @@
 
     if desc is None:
         description = f'Decompressing {filename}'
     # NOTE: filtered_matrix.tar.gz --> filtered_matrix/**/file.tsv
     decompress_tarball_of_gunzipped_files(fullpath, desc, remove)
 
 
-# %% ../nbs/02_utils.ipynb 33
+# %% ../nbs/02_utils.ipynb 34
 def make_temp_file(**kwargs: Any) -> tempfile.NamedTemporaryFile:
     temp = tempfile.NamedTemporaryFile(**kwargs)
     @atexit.register
     def delete_temp() -> None:
         temp.close()
     return temp
 
-# %% ../nbs/02_utils.ipynb 35
+# %% ../nbs/02_utils.ipynb 36
 from urllib3.util.url import parse_url
 
-# %% ../nbs/02_utils.ipynb 36
+# %% ../nbs/02_utils.ipynb 37
 def urljoin(*parts: str) -> str:
     return parse_url('/'.join(s.strip('/') for s in parts)).url
 
-# %% ../nbs/02_utils.ipynb 38
+# %% ../nbs/02_utils.ipynb 39
 from dataclasses import dataclass, field
 import numpy as np, pandas as pd
 
 from typing import List, Union, Tuple
 
-# %% ../nbs/02_utils.ipynb 41
+# %% ../nbs/02_utils.ipynb 42
 @dataclass
 class Slice:
     """A class for representing a slice and providing conversion to other formats."""
     slc: slice = field(default_factory=slice)
 
     @property
     def start(self):
@@ -563,61 +580,61 @@
             return self.totuple()
         elif dtype in {'dict', dict}:
             return self.todict()
         elif dtype in {'slice', slice}:
             return self.toslice()
         return self
 
-# %% ../nbs/02_utils.ipynb 43
+# %% ../nbs/02_utils.ipynb 44
 import os, pathlib 
 from pathlib import Path
 from dataclasses import dataclass, field, KW_ONLY
 from typing import Optional, List, ClassVar, Any, TypeAlias, Callable
 from enum import StrEnum
 
-# %% ../nbs/02_utils.ipynb 44
+# %% ../nbs/02_utils.ipynb 45
 from iza.types import (
     PathLike, PathType,
     DirectoryTreeStrings, TreeEntryFunc,
     RichTree, RichText, RichConsole, RichProgress
 )
 from .static import EXT_PY
 
 #| export
 from .imp import RichImp
 from ipos.imp import is_mod, is_var_imp, Module, Imp
 
-# %% ../nbs/02_utils.ipynb 45
+# %% ../nbs/02_utils.ipynb 46
 try:    
     from rich.tree import Tree
     from rich.text import Text    
     from rich.filesize import decimal
     from rich import get_console
     from rich.console import Console
     from rich.progress import Progress
 
 except ImportError:
     Tree = None
     Text = None 
     Progress = None
 
-# %% ../nbs/02_utils.ipynb 49
+# %% ../nbs/02_utils.ipynb 50
 def base_init_tree(dirname: str):
     return None
 
 def rich_init_tree(dirname):
     return Tree(f'[link file://{dirname}]{dirname}', guide_style='bold bright_blue')
 
 def init_tree(dirname):
     try:
         return rich_init_tree(dirname)
     except:
         return base_init_tree(dirname)
 
-# %% ../nbs/02_utils.ipynb 51
+# %% ../nbs/02_utils.ipynb 52
 def base_entry_fn(path:Path, prefix:str='', pointer:str='', suffix:str='') -> str:
     name = path.name
     return f'{prefix}{pointer}{name}{suffix}'
 
 def rich_entry_fn(path:Path, prefix:str='', pointer:str='', suffix:str='') -> str:
     text = Text(path.name)
     size = decimal(path.stat().st_size)
@@ -628,15 +645,15 @@
 def entry_fn(path:Path, prefix:str='', pointer:str='', suffix:str='') -> str:
     try:
         return rich_entry_fn(path, prefix, pointer, suffix)
     except:
         return base_entry_fn(path, prefix, pointer, suffix)
 
 
-# %% ../nbs/02_utils.ipynb 53
+# %% ../nbs/02_utils.ipynb 54
 def walk_dir_tree(
     dirname: PathLike, 
     prefix: str = '',
     hidden: Optional[bool] = False, 
     tree: Optional[RichTree] = None,
     entry_fn: TreeEntryFunc = entry_fn,
 ):    
@@ -668,15 +685,15 @@
             branch = tree.add(entry_fn(path))
     
         if path.is_dir():
             # NOTE: space because last, └── , above so no more |
             extension = BRANCH if pointer == TEE else SPACE
             yield from walk_dir_tree(path, prefix=f'{prefix}{extension}', hidden=hidden, tree=branch, entry_fn=entry_fn)
 
-# %% ../nbs/02_utils.ipynb 55
+# %% ../nbs/02_utils.ipynb 56
 @dataclass
 class DirectoryTree:
     dirname: str
     
     hidden: Optional[bool] = False
     entry_fn: Optional[TreeEntryFunc] = field(default=entry_fn)
     tree: Optional[RichTree] = field(init=False, default=None)
@@ -708,15 +725,15 @@
         print(tree_str)
         return
 
     def __repr__(self):        
         tree_str = self.make_tree_str()        
         return tree_str  
 
-# %% ../nbs/02_utils.ipynb 56
+# %% ../nbs/02_utils.ipynb 57
 @dataclass
 class RichDirectory(DirectoryTree):
     _: KW_ONLY
     console: Optional[RichConsole] = field(default_factory=Console, init=True, repr=False)    
     _imp: Imp = field(default_factory=RichImp, init=False, repr=False)
     def __post_init__(self):
         super().__post_init__()
@@ -725,40 +742,40 @@
         if self.console is None and is_mod(self._imp._module):
             self.console = get_console()
 
     def print_rich(self) -> None:    
         lines = self.get_tree_lines()
         self.console.print(self.tree)
 
-# %% ../nbs/02_utils.ipynb 57
+# %% ../nbs/02_utils.ipynb 58
 @dataclass
 class Directory(DirectoryTree):
     dirname: PathLike
     pass
 
-# %% ../nbs/02_utils.ipynb 59
+# %% ../nbs/02_utils.ipynb 60
 import os
 from pathlib import Path
 from dataclasses import dataclass, field, KW_ONLY
 from typing import Optional, List, ClassVar
 
-# %% ../nbs/02_utils.ipynb 61
+# %% ../nbs/02_utils.ipynb 62
 import pandas as pd
 
-# %% ../nbs/02_utils.ipynb 62
+# %% ../nbs/02_utils.ipynb 63
 from iza.static import (
     ADATA, MATRIX, BARCODES, FEATURES, EXT_H5, EXT_MTX, EXT_TSV,
     GENE_SYMBOL, ENSEMBL_ID
 )
 from iza.types import (
     AnnData
 )
 from tqdm.auto import tqdm
 
-# %% ../nbs/02_utils.ipynb 63
+# %% ../nbs/02_utils.ipynb 64
 try: 
     import scanpy as sc, scprep
 
     # NOTE: Directory defined in _02_utils/_02_directory.ipynb
     @dataclass
     class FilterMatrixDirectory(Directory):
         _: KW_ONLY
@@ -873,23 +890,23 @@
         
 
         def __post_init__(self):    
             raise ImportError('FilterMatrixDirectory requires scprep and scanpy to be installed')
         
     pass
 
-# %% ../nbs/02_utils.ipynb 65
+# %% ../nbs/02_utils.ipynb 66
 import os
 import numpy as np, pandas as pd
 from typing import Optional, List, ClassVar, Any
 
-# %% ../nbs/02_utils.ipynb 66
+# %% ../nbs/02_utils.ipynb 67
 from .types import Tensor, Device, SeriesLike, ndarray
 
-# %% ../nbs/02_utils.ipynb 69
+# %% ../nbs/02_utils.ipynb 70
 def is_matrix(arr: SeriesLike) -> bool:
     '''
     Checks whether or not `arr` is a np.matrix
     
     Parameters
     ----------    
     arr : SeriesLike
@@ -969,15 +986,15 @@
     Returns
     -------
     result : bool
     '''
     return isinstance(arr_q, ndarray)
 
 
-# %% ../nbs/02_utils.ipynb 70
+# %% ../nbs/02_utils.ipynb 71
 def is_device(device_q: Device) -> bool:
     '''
     Checks whether or not `device_q` is a valid
     pytorch device type.
     
     Parameters
     ----------    
@@ -1064,15 +1081,15 @@
     
     See Also
     --------
     is_tensor
     '''
     return is_tensor(tensor_q)
 
-# %% ../nbs/02_utils.ipynb 71
+# %% ../nbs/02_utils.ipynb 72
 def undo_sparse(arr: SeriesLike) -> SeriesLike:  
     '''
     Given a arr tries to make it a dense array
     
     Parameters
     ----------    
     arr : SeriesLike
@@ -1099,25 +1116,25 @@
     arr = undo_sparse(arr)
 
     if not is_np(arr):
         arr = np.array(arr)
 
     return arr
 
-# %% ../nbs/02_utils.ipynb 73
+# %% ../nbs/02_utils.ipynb 74
 import os, random
 import numpy as np
 
 from dataclasses import dataclass, field, KW_ONLY
 from typing import Optional, List, ClassVar, Any
 
-# %% ../nbs/02_utils.ipynb 74
+# %% ../nbs/02_utils.ipynb 75
 from .types import Tensor, Device, SeriesLike, ndarray
 
-# %% ../nbs/02_utils.ipynb 76
+# %% ../nbs/02_utils.ipynb 77
 try:
     import torch
     def ensure_device(device: Device) -> Device:
         '''
         Given a valid device type attempts to instantiant 
         a pytorch device object i.e. `device='cpu'` will
         return `torch.device('cpu')`.
@@ -1387,15 +1404,15 @@
     coerce_mps_dtype = lambda dtype, device, assume_on_mps: dtype
     ensure_mps_dtype = identity
     move_to = lambda tensor, other, dtype, do_dtype: tensor
     pass
 
 
 
-# %% ../nbs/02_utils.ipynb 77
+# %% ../nbs/02_utils.ipynb 78
 try:
     import torch, pytorch_lightning as pl
     def set_seeds(seed: int) -> None:
         '''
         Calls a bunch of seed functions with `seed`
         
         Parameters
@@ -1407,25 +1424,25 @@
         np.random.seed(seed)    
         pl.seed_everything(seed)
 except ImportError as err:
      def set_seeds(seed: int) -> None:
          random.seed(seed)
          np.random.seed(seed)
 
-# %% ../nbs/02_utils.ipynb 79
+# %% ../nbs/02_utils.ipynb 80
 from dataclasses import dataclass, field
 import numpy as np, pandas as pd
 
 from typing import List, Any, Optional
 
-# %% ../nbs/02_utils.ipynb 80
+# %% ../nbs/02_utils.ipynb 81
 from .types import AnnData, ndarray, DataFrame
 from .static import X_MAGIC, PHATE, X_PHATE
 
-# %% ../nbs/02_utils.ipynb 82
+# %% ../nbs/02_utils.ipynb 83
 @dataclass
 class AdataExtractor:
     adata: AnnData
     layer: Optional[str] = X_MAGIC
     x_emb: Optional[str] = X_PHATE
 
     dim_str: Optional[str] = None
```

### Comparing `iza-0.0.6/iza.egg-info/PKG-INFO` & `iza-0.0.7/iza.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iza
-Version: 0.0.6
+Version: 0.0.7
 Summary: chaos package of utilities; a nod to izalith
 Home-page: https://github.com/dsm-72/iza
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `iza-0.0.6/settings.ini` & `iza-0.0.7/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = iza
 lib_name = iza
-version = 0.0.6
+version = 0.0.7
 min_python = 3.10
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = iza
 nbs_path = nbs
 recursive = True
@@ -30,9 +30,9 @@
 console_scripts = iza=iza.commands:app
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
-requirements = pandas seaborn scikit-learn numpy nbformat rich typer requests tqdm
+requirements = pandas seaborn scikit-learn numpy nbformat rich typer requests tqdm ipos
```

### Comparing `iza-0.0.6/setup.py` & `iza-0.0.7/setup.py`

 * *Files identical despite different names*

