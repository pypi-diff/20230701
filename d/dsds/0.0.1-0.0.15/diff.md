# Comparing `tmp/dsds-0.0.1.tar.gz` & `tmp/dsds-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsds-0.0.1.tar", last modified: Wed Jun 21 01:13:10 2023, max compression
+gzip compressed data, was "dsds-0.0.15.tar", last modified: Sat Jul  1 02:14:18 2023, max compression
```

## Comparing `dsds-0.0.1.tar` & `dsds-0.0.15.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 01:13:10.299490 dsds-0.0.1/
--rw-rw-rw-   0        0        0     1076 2023-06-20 22:59:11.000000 dsds-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     8690 2023-06-21 01:13:10.298490 dsds-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6352 2023-06-21 01:08:29.000000 dsds-0.0.1/README.md
--rw-rw-rw-   0        0        0     1380 2023-06-21 00:35:21.000000 dsds-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-21 01:13:10.299490 dsds-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-21 01:13:10.275300 dsds-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-21 01:13:10.286428 dsds-0.0.1/src/dsds/
--rw-rw-rw-   0        0        0       86 2023-06-20 22:44:35.000000 dsds-0.0.1/src/dsds/__init__.py
--rw-rw-rw-   0        0        0    32532 2023-06-20 22:45:44.000000 dsds-0.0.1/src/dsds/builder.py
--rw-rw-rw-   0        0        0     3766 2023-06-20 23:18:47.000000 dsds-0.0.1/src/dsds/eda_text.py
--rw-rw-rw-   0        0        0    23724 2023-06-20 18:09:46.000000 dsds-0.0.1/src/dsds/fs.py
--rw-rw-rw-   0        0        0    12723 2023-06-20 18:31:58.000000 dsds-0.0.1/src/dsds/prescreen.py
--rw-rw-rw-   0        0        0      141 2023-06-16 03:14:56.000000 dsds-0.0.1/src/dsds/sample.py
--rw-rw-rw-   0        0        0      323 2023-06-20 18:16:12.000000 dsds-0.0.1/src/dsds/split.py
--rw-rw-rw-   0        0        0    28111 2023-06-20 22:22:56.000000 dsds-0.0.1/src/dsds/transform.py
--rw-rw-rw-   0        0        0     1811 2023-06-16 03:00:16.000000 dsds-0.0.1/src/dsds/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-21 01:13:10.297489 dsds-0.0.1/src/dsds.egg-info/
--rw-rw-rw-   0        0        0     8690 2023-06-21 01:13:10.000000 dsds-0.0.1/src/dsds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2023-06-21 01:13:10.000000 dsds-0.0.1/src/dsds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 01:13:10.000000 dsds-0.0.1/src/dsds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      157 2023-06-21 01:13:10.000000 dsds-0.0.1/src/dsds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-21 01:13:10.000000 dsds-0.0.1/src/dsds.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 02:14:18.342856 dsds-0.0.15/
+-rw-rw-rw-   0        0        0     1079 2023-06-23 04:44:14.000000 dsds-0.0.15/LICENSE
+-rw-rw-rw-   0        0        0     5284 2023-07-01 02:14:18.342856 dsds-0.0.15/PKG-INFO
+-rw-rw-rw-   0        0        0     2912 2023-07-01 01:54:50.000000 dsds-0.0.15/README.md
+-rw-rw-rw-   0        0        0     1398 2023-07-01 01:17:46.000000 dsds-0.0.15/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-01 02:14:18.342856 dsds-0.0.15/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-01 02:14:18.305847 dsds-0.0.15/src/
+drwxrwxrwx   0        0        0        0 2023-07-01 02:14:18.321851 dsds-0.0.15/src/dsds/
+-rw-rw-rw-   0        0        0       87 2023-07-01 01:17:22.000000 dsds-0.0.15/src/dsds/__init__.py
+-rw-rw-rw-   0        0        0    36129 2023-06-25 20:43:42.000000 dsds-0.0.15/src/dsds/_builder.py
+-rw-rw-rw-   0        0        0     8493 2023-06-25 20:43:52.000000 dsds-0.0.15/src/dsds/_transform.py
+-rw-rw-rw-   0        0        0     4528 2023-06-28 04:17:12.000000 dsds-0.0.15/src/dsds/blueprint.py
+-rw-rw-rw-   0        0        0     3766 2023-06-20 23:18:47.000000 dsds-0.0.15/src/dsds/eda_text.py
+-rw-rw-rw-   0        0        0    24398 2023-06-28 04:24:18.000000 dsds-0.0.15/src/dsds/fs.py
+-rw-rw-rw-   0        0        0     2983 2023-06-30 23:24:11.000000 dsds-0.0.15/src/dsds/metrics.py
+-rw-rw-rw-   0        0        0    27096 2023-07-01 01:37:28.000000 dsds-0.0.15/src/dsds/prescreen.py
+-rw-rw-rw-   0        0        0      141 2023-06-16 03:14:56.000000 dsds-0.0.15/src/dsds/sample.py
+-rw-rw-rw-   0        0        0     1957 2023-06-29 03:48:38.000000 dsds-0.0.15/src/dsds/split.py
+-rw-rw-rw-   0        0        0    23534 2023-07-01 01:41:03.000000 dsds-0.0.15/src/dsds/transform.py
+-rw-rw-rw-   0        0        0     1484 2023-06-29 03:20:17.000000 dsds-0.0.15/src/dsds/type_alias.py
+-rw-rw-rw-   0        0        0     1811 2023-06-16 03:00:16.000000 dsds-0.0.15/src/dsds/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-01 02:14:18.340855 dsds-0.0.15/src/dsds.egg-info/
+-rw-rw-rw-   0        0        0     5284 2023-07-01 02:14:18.000000 dsds-0.0.15/src/dsds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-07-01 02:14:18.000000 dsds-0.0.15/src/dsds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 02:14:18.000000 dsds-0.0.15/src/dsds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2023-07-01 02:14:18.000000 dsds-0.0.15/src/dsds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-01 02:14:18.000000 dsds-0.0.15/src/dsds.egg-info/top_level.txt
```

### Comparing `dsds-0.0.1/LICENSE` & `dsds-0.0.15/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 
+Copyright (c) 2023 T.Q
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `dsds-0.0.1/pyproject.toml` & `dsds-0.0.15/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 [build-system]
 requires = ["setuptools"]
 
 [project]
 name = "dsds"
-version = "0.0.1"
+version = "0.0.15"
 requires-python = ">=3.9"
 readme = "README.md"
-description = "A feature screening, selection, EDA, pipeline building and management tool centered around Polars dataframes."
+description = "A feature screening, selection, EDA, pipeline building and management tool centered around Polars dataframe."
 authors = [
     {name = "Tianren Qin", email = "tq9695@gmail.com"}
 ]
 license = {file = "LICENSE"}
 dependencies = [
-    "polars >= 0.18.3",
-    "scipy >= 1.10.1",
-    "orjson >= 3.9.1",
+    "polars >= 0.18.4",
+    "scipy >= 1.11.1",
     "pandas",
     "numpy",
     "typing_extensions >= 4.0.1"
 ]
 
-keywords = ["pipeline", "EDA", "feature-screening", "feature-selection"]
+keywords = ["data pipeline", "EDA", "feature-screening", "feature-selection"]
 
 classifiers = [
   "Development Status :: 2 - Pre-Alpha",
   "Environment :: Console",
   "Intended Audience :: Science/Research",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
@@ -36,15 +35,16 @@
   "Programming Language :: Python :: 3.11",
   "Topic :: Scientific/Engineering",
 ]
 
 [project.optional-dependencies]
 scikit-learn = ["scikit-learn"]
 xgboost = ["xgboost"]
-all = ["scikit-learn", "xgboost"]
+lightgbm = ["lightgbm"]
+all = ["scikit-learn", "xgboost", "lightgbm"]
 
 [project.urls]
 "Homepage" = "https://github.com/abstractqqq/dsds"
 
 [tool.ruff]
 line-length = 120
 fix = true
```

### Comparing `dsds-0.0.1/src/dsds/builder.py` & `dsds-0.0.15/src/dsds/_builder.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,867 +1,920 @@
-from __future__ import annotations
+# from __future__ import annotations
 
-import inspect
-from .prescreen import (
-    remove_if_exists
-    , regex_removal
-    , var_removal
-    , null_removal
-    , unique_removal
-    , constant_removal
-    , date_removal
-)
-# from .eda_selection import *
-from .transform import (
-    FitRecord
-    , FitTransform
-    , ScalingStrategy
-    , ImputationStartegy
-    , scale
-    , impute
-    , binary_encode
-    , one_hot_encode
-    , percentile_encode
-    , smooth_target_encode
-    , ordinal_encode
-    , ordinal_auto_encode
-)
-
-from dataclasses import dataclass
-import polars as pl
-import pandas as pd
-from typing import ParamSpec, Self, TypeVar, Optional, Any, Callable, Iterable, Concatenate
-from enum import Enum
-from pathlib import Path
-from time import perf_counter
-import orjson
-import logging
-import importlib
-import os
-
-T = TypeVar("T")
-P = ParamSpec("P")
-
-logger = logging.getLogger(__name__)
-
-################################################################################################
-# WORK IN PROGRESS
-# 
-# For everyone who is reading this, my coding style is primarily influenced by the Primeagen,
-# some Rust conventions, and a little bit of functional style, although unfortunately we have to 
-# work with classes in Python.
-#
-# Terminologies: 
-# A ExecStep/transformation is canonical if the transformation on the dataset does not require
-# any information about the dataset to be performed or repeated.
-# e.g. raise the value of a column to the power of 2
-# e.g. remove columns with names a, b, c
-# They should be ExecSteps with is_fit = False and is_selector = False.
-# A canonical transformation should have the following signature:
-# Concatenate[pl.DataFrame, P] ---> pl.DataFrame, where
-# the output is just the transformed dataframe.
-# 
-# A non-canonical transformation is a transformation that requires information about the data to
-# be repeated.
-# e.g. impute (because we might need the mean/median of columns), scale, encoding... 
-# They should be ExecSteps with is_fit = True and is_selector = False.
-# A non-canonical transfromation should have the signature:
-# Concatenate[pl.DataFrame, P] ---> FitTransform, where
-# P = placeholder for other parameters
-# FitTransform is a data container that contains 
-# 1. transformed: the transformed dataframe
-# 2. mapping: a FitRecord that contains the necessary info about the data to repeat this fit
-#
-# A selector is a function that has the following signature:
-# Concatenate[pl.DataFrame, P] ---> list[str], where
-# P = placeholder for other parameters
-#
-################################################################################################
-
-
-# This is just a builtin mapping for desc.
-class BuiltinExecs(Enum):
-    NULL_REMOVAL = "Remove columns with more than {:.2f}% nulls."
-    VAR_REMOVAL = "Remove columns with less than {} variance. (Not recommended.)"
-    CONST_REMOVAL = "Remove columns that are constants."
-    UNIQUE_REMOVAL = "Remove columns that are like unique identifiers, e.g. with more than {:.2f}% unique values."
-    COL_REMOVAL = "Remove given if they exist in dataframe."
-    DATE_REMOVAL = "Remove columns that are inferred to be dates."
-    REGX_REMOVAL = "Remove all columns whose names satisfy the regex rule {}."
-    BINARY_ENCODE = "Encode given into binary [0,1] values."
-    ORDINAL_ENCODE = "Encode string values of given columns into numbers with given mapping."
-    ORDINAL_AUTO_ENCODE = "Encode string values of given columns into numbers with inferred ordering."
-    TARGET_ENCODE = "Encode string values using the target encoding algorithm."
-    ONE_HOT_ENCODE = "Encode string values of given columns by the one-hot-encoding technique. (No drop first option)."
-    PERCENTILE_ENCODE = "Encode a continuous column by percentiles."
-    SCALE = "Scale using specified the {} scaling method."
-    IMPUTE = "Impute using specified the {} imputation method."
-    CHECKPOINT = "Unavailable for now."
-    SELECT = "Select only the given columns."
-    LOWER = "Lower all column names in the incoming dataframe."
-
-@dataclass
-class ExecStep():
-    name:str
-    module:str|Path
-    desc:str = ""
-    args:Optional[dict[str, Any]] = None # None if it is record.
-    is_fit:bool = False
-    # Is this a function that produces a FitTransform output? 
-    # If so, the output is expected to be of type FitRecord (pl.DataFrame, FitRecord).
-    # If not, the output is expected to be of type pl.DataFrame. (Normal, natural output)
-
-    fit_name:Optional[str] = None # name of the FitRecord class (The class that inherits from FitRecord)
-    fit_module:Optional[str] = None # module where this FitRecord class belongs to
-    fit_record: Optional[FitRecord] = None # The actual content of the Record, will only be not none in blueprints.
-    is_selector:bool = False
-    is_custom:bool = False 
-
-    def get_args(self) -> str:
-        return self.args
-    
-    def drop_args(self) -> Self:
-        self.args = None
-    
-    def __str__(self) -> str:
-        text = f"Function: {self.name} | Module: {self.module} | Arguments:\n{self.args}\n"
-        text += f"Brief description: {self.desc}"
-        if self.is_fit:
-            text += "\nThis step is will fit and transform the data."
-        if self.is_custom:
-            text += "\nThis step is a user defined function."
-        return text
-
-@dataclass
-class ExecPlan():
-    steps:list[ExecStep]
-    target:str = ""
-
-    def __iter__(self) -> Iterable[ExecStep]:
-        return iter(self.steps)
-
-    def __str__(self) -> str:
-        if len(self.steps) > 0:
-            text = ""
-            for i, item in enumerate(self.steps):
-                text += f"--- Step {i+1}: ---\n"
-                text += str(item)
-                text += "\n"
-            return text
-        else:
-            return "No step has been set."
-        
-    def __len__(self) -> int:
-        return len(self.steps)
-    
-    def clear(self) -> None:
-        self.steps.clear()
-
-    def is_empty(self) -> bool:
-        return len(self.steps) == 0
-
-    def add(self, step:ExecStep) -> None:
-        self.steps.append(step)
-
-    def popleft(self) -> Optional[ExecStep]:
-        return self.steps.pop(0)
-
-    def add_step(self
-        , func:Callable[Concatenate[pl.DataFrame, P], pl.DataFrame|FitTransform]
-        , desc:str
-        , args:dict[str, Any] # Technically is not Any, but Anything that can be serialized by orjson..
-        , is_fit:bool=False
-        ) -> None:
-
-        self.steps.append(
-            ExecStep(func.__name__, func.__module__, desc = desc, args = args
-                    , is_fit = is_fit, is_selector = False, is_custom = False)
-        )
-
-    def add_selector_step(self
-        , func:Callable[Concatenate[pl.DataFrame, P], list[str]]
-        , desc:str
-        , args:dict[str, Any]
-        ) -> None:
-        
-        self.steps.append(
-            ExecStep(func.__name__, func.__module__, desc = desc, args = args, 
-                    is_fit = False, is_selector = True, is_custom = False)
-        )
-
-    def add_custom_step(self
-        , func:Callable[[pl.DataFrame, T], pl.DataFrame|FitTransform]
-        , desc:str
-        , args:dict[str, Any]
-        , is_fit:bool=False) -> None:
-        
-        self.steps.append(
-            ExecStep(func.__name__, func.__module__, desc = desc, args = args, 
-                    is_fit = is_fit, is_selector = False, is_custom = True)
-        )
-
-    def add_custom_selector_step(self
-        , func:Callable[[pl.DataFrame, T], list[str]]
-        , desc:str
-        , args:dict[str, Any]
-        ) -> None:
-        
-        self.steps.append(
-            ExecStep(func.__name__, func.__module__, desc = desc, args = args, 
-                    is_fit = False, is_selector = True, is_custom = True)
-        )
-
-def _select_cols(df:pl.DataFrame, cols:list[str], target:str) -> pl.DataFrame:
-
-    # Whether to select target or not depends on if df has a target column.
-    if target in df.columns and target not in cols:
-        cols.append(target)
-    elif target not in df.columns and target in cols:
-        cols.remove(target)
-
-    # don't check if c in cols belongs to df. Let it error.
-    return df.select(cols)
-
-def _lower_columns(df:pl.DataFrame) -> pl.DataFrame:
-    return df.rename({c: c.lower() for c in df.columns})
-
-
-# 1. The exact logic 
-# Pipebuilder -> ExecPlan (as execution_plan)
-#             -> ExecPlan (as _blueprint)
-# can be improved. Especially in execution_plan, we can totally just use the callable,
-# instead of importing it in the build process.
-# 
-# 2. Can we make output json smaller (slim down ExecStep)? Do we really need all the fields?
-# I want to avoid nesting. So it is flatter. Can we be more precise?
-#
-# 3. Better text representation
-#
-
-class PipeBuilder:
-
-    def __init__(self, project_name:str="my_project"):
-
-        self.target:str = ""
-        self.data:Optional[pl.DataFrame] = None
-        self.project_name:str = project_name
-        self._built:bool = False
-        self._execution_plan:ExecPlan = ExecPlan(steps=[])
-        self._blueprint:ExecPlan = ExecPlan(steps=[])
-    
-    def __len__(self) -> int: # positive int
-        return len(self._execution_plan)
-    
-    def __str__(self) -> str:
-        if not self._execution_plan.is_empty():
-            text = f"Project name: {self.project_name}\nTotal steps: {len(self)} | Ready to build: {self._is_ready()} |"
-            if self.target != "":
-                text += f" Target variable: {self.target}"
-            text += "\n"
-            text += str(self._execution_plan)
-            return text
-        return "The current builder has no execution plan."
-    
-    ### I/O
-    def set_target(self, target:str) -> Self:
-        if target == "":
-            raise ValueError("Target cannot be empty string.")
-        
-        if self.data is not None:
-            if target not in self.data.columns:
-                raise ValueError("Target is not found in the dataframe.")
+# #######################################################################
+# # ALL CODE HERE ARE FOR ARCHIVE PURPOSE 
+# # WILL BE REMOVED ONCE THE NEW DEVELOPMENT BECOMES MORE STABLE
+# #######################################################################
+
+# from .type_alias import (
+#     PolarsFrame
+# )
+
+# from .prescreen import (
+#     remove_if_exists
+#     , regex_removal
+#     , var_removal
+#     , null_removal
+#     , unique_removal
+#     , constant_removal
+#     , date_removal
+#     , non_numeric_removal
+# )
+# # from .eda_selection import *
+# from .transform import (
+#     FitRecord
+#     , FitTransform
+#     , ScalingStrategy
+#     , ImputationStartegy
+#     , scale
+#     , impute
+#     , binary_encode
+#     , one_hot_encode
+#     # , percentile_encode
+#     , smooth_target_encode
+#     , ordinal_encode
+#     , ordinal_auto_encode
+# )
+
+# from dataclasses import dataclass
+# import polars as pl
+# from polars.type_aliases import FrameInitTypes
+# import pandas as pd
+# from typing import ParamSpec, Self, TypeVar, Optional, Any, Callable, Iterable, Concatenate
+# from enum import Enum
+# from pathlib import Path
+# from time import perf_counter
+# import orjson
+# import inspect
+# import re
+# import logging
+# import importlib
+# import os
+
+# T = TypeVar("T")
+# P = ParamSpec("P")
+
+# logger = logging.getLogger(__name__)
+
+# ################################################################################################
+# # WORK IN PROGRESS
+# # 
+# # For everyone who is reading this, my coding style is primarily influenced by the Primeagen,
+# # some Rust conventions, and a little bit of functional style, although unfortunately we have to 
+# # work with classes in Python.
+# #
+# # Terminologies: 
+# # A ExecStep/transformation is canonical if the transformation on the dataset does not require
+# # any information about the dataset to be performed or repeated.
+# # e.g. raise the value of a column to the power of 2
+# # e.g. remove columns with names a, b, c
+# # They should be ExecSteps with is_fit = False and is_selector = False.
+# # A canonical transformation should have the following signature:
+# # Concatenate[pl.DataFrame, P] ---> pl.DataFrame, where
+# # the output is just the transformed dataframe.
+# # 
+# # A non-canonical transformation is a transformation that requires information about the data to
+# # be repeated.
+# # e.g. impute (because we might need the mean/median of columns), scale, encoding... 
+# # They should be ExecSteps with is_fit = True and is_selector = False.
+# # A non-canonical transfromation should have the signature:
+# # Concatenate[pl.DataFrame, P] ---> FitTransform, where
+# # P = placeholder for other parameters
+# # FitTransform is a data container that contains 
+# # 1. transformed: the transformed dataframe
+# # 2. mapping: a FitRecord that contains the necessary info about the data to repeat this fit
+# #
+# # A selector is a function that has the following signature:
+# # Concatenate[pl.DataFrame, P] ---> list[str], where
+# # P = placeholder for other parameters
+# #
+# ################################################################################################
+
+
+# # This is just a builtin mapping for desc.
+# class BuiltinExecs(Enum):
+#     NULL_REMOVAL = "Remove columns with more than {:.2f}% nulls."
+#     VAR_REMOVAL = "Remove columns with less than {} variance. (Not recommended.)"
+#     CONST_REMOVAL = "Remove columns that are constants."
+#     NON_NUMERIC_REMOVAL = "Remove all non-numeric columns."
+#     UNIQUE_REMOVAL = "Remove columns that are like unique identifiers, e.g. with more than {:.2f}% unique values."
+#     COL_REMOVAL = "Remove given if they exist in dataframe."
+#     DATE_REMOVAL = "Remove columns that are inferred to be dates."
+#     REGX_REMOVAL = "Remove all columns whose names satisfy the regex rule {}."
+#     BINARY_ENCODE = "Encode given into binary [0,1] values."
+#     ORDINAL_ENCODE = "Encode string values of given columns into numbers with given mapping."
+#     ORDINAL_AUTO_ENCODE = "Encode string values of given columns into numbers with inferred ordering."
+#     TARGET_ENCODE = "Encode string values using the target encoding algorithm."
+#     ONE_HOT_ENCODE = "Encode string values of given columns by the one-hot-encoding technique. (No drop first option)."
+#     PERCENTILE_ENCODE = "Encode a continuous column by percentiles."
+#     SCALE = "Scale using specified the {} scaling method."
+#     IMPUTE = "Impute using specified the {} imputation method."
+#     CHECKPOINT = "Unavailable for now."
+#     SELECT = "Select only the given columns."
+#     LOWER = "Lower all column names in the incoming dataframe."
+
+# @dataclass
+# class ExecStep():
+#     name:str
+#     module:str|Path
+#     desc:str = ""
+#     args:Optional[dict[str, Any]] = None # None if it is record.
+#     is_fit:bool = False
+#     # Is this a function that produces a FitTransform output? 
+#     # If so, the output is expected to be of type FitRecord (pl.DataFrame, FitRecord).
+#     # If not, the output is expected to be of type pl.DataFrame. (Normal, natural output)
+
+#     fit_name:Optional[str] = None # name of the FitRecord class (The class that inherits from FitRecord)
+#     fit_module:Optional[str] = None # module where this FitRecord class belongs to
+#     fit_record: Optional[FitRecord] = None # The actual content of the Record, will only be not none in blueprints.
+#     is_selector:bool = False
+#     is_custom:bool = False 
+
+#     def get_args(self) -> str:
+#         return self.args
+    
+#     def drop_args(self) -> Self:
+#         self.args = None
+    
+#     def __str__(self) -> str:
+#         text = f"Function: {self.name} | Module: {self.module} | Arguments:\n{self.args}\n"
+#         text += f"Brief description: {self.desc}"
+#         if self.is_fit:
+#             text += "\nThis step is will fit and transform the data."
+#         if self.is_custom:
+#             text += "\nThis step is a user defined function."
+#         return text
+
+# @dataclass
+# class ExecPlan():
+#     steps:list[ExecStep]
+#     target:str = ""
+
+#     def __iter__(self) -> Iterable[ExecStep]:
+#         return iter(self.steps)
+
+#     def __str__(self) -> str:
+#         if len(self.steps) > 0:
+#             text = ""
+#             for i, item in enumerate(self.steps):
+#                 text += f"--- Step {i+1}: ---\n"
+#                 text += str(item)
+#                 text += "\n"
+#             return text
+#         else:
+#             return "No step has been set."
+        
+#     def __len__(self) -> int:
+#         return len(self.steps)
+    
+#     def clear(self) -> None:
+#         self.steps.clear()
+
+#     def is_empty(self) -> bool:
+#         return len(self.steps) == 0
+
+#     def add(self, step:ExecStep) -> None:
+#         self.steps.append(step)
+
+#     def popleft(self) -> Optional[ExecStep]:
+#         return self.steps.pop(0)
+    
+#     def find(self, name:str) -> list[int]:
+#         found:list[int] = []
+#         regex = re.compile(name)
+#         for i,step in enumerate(self.steps):
+#             if regex.search(step.name) or regex.search(step.desc):
+#                 found.append(i)
+
+#         return found
+
+#     def add_step(self
+#         , func:Callable[Concatenate[pl.DataFrame, P], pl.DataFrame|FitTransform]
+#         , desc:str
+#         , args:dict[str, Any] # Technically is not Any, but Anything that can be serialized by orjson..
+#         , is_fit:bool=False
+#     ) -> None:
+
+#         self.steps.append(
+#             ExecStep(func.__name__, func.__module__, desc = desc, args = args
+#                     , is_fit = is_fit, is_selector = False, is_custom = False)
+#         )
+
+#     def add_selector_step(self
+#         , func:Callable[Concatenate[pl.DataFrame, P], list[str]]
+#         , desc:str
+#         , args:dict[str, Any]
+#     ) -> None:
+        
+#         self.steps.append(
+#             ExecStep(func.__name__, func.__module__, desc = desc, args = args, 
+#                     is_fit = False, is_selector = True, is_custom = False)
+#         )
+
+#     def add_custom_step(self
+#         , func:Callable[[pl.DataFrame, T], pl.DataFrame|FitTransform]
+#         , desc:str
+#         , args:dict[str, Any]
+#         , is_fit:bool=False
+#     ) -> None:
+        
+#         self.steps.append(
+#             ExecStep(func.__name__, func.__module__, desc = desc, args = args, 
+#                     is_fit = is_fit, is_selector = False, is_custom = True)
+#         )
+
+#     def add_custom_selector_step(self
+#         , func:Callable[[pl.DataFrame, T], list[str]]
+#         , desc:str
+#         , args:dict[str, Any]
+#     ) -> None:
+        
+#         self.steps.append(
+#             ExecStep(func.__name__, func.__module__, desc = desc, args = args, 
+#                     is_fit = False, is_selector = True, is_custom = True)
+#         )
+
+# def _select_cols(df:PolarsFrame, cols:list[str], target:str) -> PolarsFrame:
+
+#     # Whether to select target or not depends on if df has a target column.
+#     if target in df.columns and target not in cols:
+#         cols.append(target)
+#     elif target not in df.columns and target in cols:
+#         cols.remove(target)
+
+#     # don't check if c in cols belongs to df. Let it error.
+#     return df.select(cols)
+
+# def _lower_columns(df:PolarsFrame) -> PolarsFrame:
+#     return df.rename({c: c.lower() for c in df.columns})
+
+# def _rename(df:PolarsFrame, rename_dict:dict[str, str]) -> PolarsFrame:
+#     return df.rename(rename_dict)
+
+# # 1. The exact logic 
+# # Pipebuilder -> ExecPlan (as execution_plan)
+# #             -> ExecPlan (as _blueprint)
+# # can be improved. Especially in execution_plan, we can totally just use the callable,
+# # instead of importing it in the build process.
+# # 
+# # 2. Can we make output json smaller (slim down ExecStep)? Do we really need all the fields?
+# # I want to avoid nesting. So it is flatter. Can we be more precise?
+# #
+# # 3. Better text representation
+# #
+
+# class PipeBuilder:
+
+#     def __init__(self, target:str="", project_name:str="my_project"):
+
+#         self.target:str = target
+#         self.data:Optional[pl.LazyFrame] = None # This is always lazy
+#         self.project_name:str = project_name
+#         self._built:bool = False
+#         self._execution_plan:ExecPlan = ExecPlan(steps=[])
+#         self._blueprint:ExecPlan = ExecPlan(steps=[])
+    
+#     def __len__(self) -> int: # positive int
+#         return len(self._execution_plan)
+    
+#     def __str__(self) -> str:
+#         text = f"Project name: {self.project_name}\nTotal steps: {len(self)} |"
+#         if self.target != "":
+#             text += f" Target variable: {self.target}"
+#         text += "\n"
+#         if not self._execution_plan.is_empty() and not self._built:
+#             text += str(self._execution_plan)
+#             return text
+#         elif self._built:
+#             text += str(self._blueprint)
+#             return text
+#         return "Nothing to print."
+    
+#     ### I/O
+#     def set_target(self, target:str) -> Self:
+#         if target == "":
+#             raise ValueError("Target cannot be empty string.")
+        
+#         if self.data is not None:
+#             if target not in self.data.columns:
+#                 raise ValueError("Target is not found in the dataframe.")
             
-        self.target = target
-        self._blueprint.target = target
-        return self
-        
-    def set_data(self, df:pl.DataFrame|pd.DataFrame) -> Self:
-        '''Set the data on which to "fit" the pipeline.'''
-        try:
-            if isinstance(df, pd.DataFrame):
-                logger.warning("Found input to be a Pandas Dataframe. It will be converted to a Polars dataframe, "
-                            "and the original Pandas dataframe will be erased.")
+#         self.target = target
+#         self._blueprint.target = target
+#         return self
+        
+#     def set_data(self, df: FrameInitTypes|PolarsFrame) -> Self:
+#         '''Set the data on which to "fit" the pipeline.'''
+#         try:
+#             if isinstance(df, pd.DataFrame):
+#                 logger.warning("Found input to be a Pandas Dataframe. It will be converted to a Polars dataframe, "
+#                             "and the original Pandas dataframe will be erased.")
                 
-                self.data = pl.from_pandas(df)
-                df = df.iloc[0:0]
-            elif isinstance(df, pl.DataFrame):
-                self.data = df.clone()
-            else:
-                raise TypeError("Input df must either be Pandas or Polars dataframe.")
-        except Exception as e:
-            logger.error(e)
-
-        return Self
-    
-    def set_data_and_target(self, df:pl.DataFrame|pd.DataFrame, target:str) -> Self:
-        _ = self.set_target(target)        
-        _ = self.set_data(df)
-        if target not in self.data.columns:
-            raise ValueError("Target is not found in the dataframe.")
-        
-        self.target = target
-        return self 
-
-    def from_csv(self, path:str|Path, **csv_args) -> Self:
-        '''
-        
-        '''
-        try:
-            self.data = pl.read_csv(path, **csv_args)
-            return Self
-        except Exception as e:
-            logger.error(e)
-
-    def from_parquet(self, path:str|Path, **parquet_args) -> Self:
-        '''
-        
-        '''
-        try:
-            self.data = pl.read_parquet(path, **parquet_args)
-            return Self
-        except Exception as e:
-            logger.error(e)
-    
-    def from_json(self, path:str|Path, **json_args) -> Self:
-        '''
-        
-        '''
-        try:
-            self.data = pl.read_json(path, **json_args)
-            return Self
-        except Exception as e:
-            logger.error(e)
-
-    def from_excel(self, path:str|Path, **excel_args) -> Self:
-        '''
-        
-        '''
-        try:
-            self.data = pl.read_json(path, **excel_args)
-            return Self
-        except Exception as e:
-            logger.error(e)
-    ### End of I/O
-    
-    ### Miscellaneous
-    def show(self):
-        print(self)
-
-    def clear(self):
-        self.data = self.data.clear()
-        self._execution_plan.clear()
-        self._blueprint.clear()
-        self._built = False
-
-    def select_cols(self, cols:list[str]) -> Self:
-        if self._is_ready():
-            self._execution_plan.add_step(
-                func = _select_cols,
-                desc = BuiltinExecs.SELECT.value,
-                args = {"cols":cols, "target":self.target}
-            )
-            return self
-        else:
-            raise ValueError("Target must be set before setting column selections.")
-    
-    def set_lower_cols(self) -> Self:
-        self._execution_plan.add_step(
-            func = _lower_columns,
-            desc = BuiltinExecs.LOWER.value,
-            args = {}
-        )
-        return self
-
-    ### End of Miscellaneous
-
-    ### Checks
-    def _is_ready(self) -> bool:
-        if self.data is None:
-            return False
-        
-        return self.target != "" and self.target in self.data.columns
-    
-    ### End of Checks.
-
-    ### Project meta data section
-    def set_project_name(self, project_name:str) -> Self:
-        if project_name == "":
-            raise ValueError("Project name cannot be empty.")
-        self.project_name = project_name
-        return self
-
-    ### End of project meta data section
-    
-    ### Column removal section
-    def set_null_removal(self, threshold:float) -> Self:
-        if threshold > 1 or threshold <= 0:
-            raise ValueError("Threshold for null removal must be between 0 and 1.")
-
-        self._execution_plan.add_step(
-            func = null_removal ,
-            desc = BuiltinExecs.NULL_REMOVAL.value.format(threshold*100),
-            args = {"threshold":threshold}  
-        )
-        return self 
-    
-    def set_var_removal(self, threshold:float) -> Self:
-        if threshold <= 0:
-            raise ValueError("Threshold for var removal must be positive.")
-        
-        if self._is_ready():
-            self._execution_plan.add_step(
-                func = var_removal,
-                desc = BuiltinExecs.VAR_REMOVAL.value.format(threshold),
-                args = {"threshold":threshold, "target":self.target},
-            )
-            return self
-        else:
-            raise ValueError("Target must be set before setting var removal.")
-    
-    def set_const_removal(self, include_null:bool=True) -> Self:
-        
-        self._execution_plan.add_step(
-            func = constant_removal,
-            desc = BuiltinExecs.CONST_REMOVAL.value,
-            args = {"include_null":include_null},
-        )
-        return self
-    
-    def set_unique_removal(self, threshold:float=0.9) -> Self:
-        if threshold > 1 or threshold <= 0:
-            raise ValueError("Threshold for unique removal must be between 0 and 1.")
-
-        self._execution_plan.add_step(
-            func = unique_removal ,
-            desc = BuiltinExecs.UNIQUE_REMOVAL.value.format(threshold*100),
-            args = {"threshold":threshold}  
-        )
-        return self 
-    
-    def set_regex_removal(self, pat:str, lowercase:bool=False) -> Self:
-        '''Removes columns that satisfies the regex rule. May optionally only check on lowercased column names.'''
-        description = BuiltinExecs.REGX_REMOVAL.value.format(pat)
-        if lowercase:
-            description += ". Everything will be lowercased."
-
-        self._execution_plan.add_step(
-            func = regex_removal,
-            desc = description,
-            args = {"pat":pat, "lowercase": lowercase},
-        )
-        return self
-    
-    def set_col_removal(self, cols:list[str]) -> Self:
-        '''Removes the given columns.'''
-        self._execution_plan.add_step(
-            func = remove_if_exists,
-            desc = BuiltinExecs.COL_REMOVAL.value,
-            args = {"to_drop":cols},
-        )
-        return self
-    
-    def set_date_removal(self) -> Self:
-        '''Removes columns that are inferred to be dates.'''
-        self._execution_plan.add_step(
-            func = date_removal ,
-            desc = BuiltinExecs.DATE_REMOVAL.value,
-            args = {}
-        )
-        return self 
-        
-    ### End of column removal section
-
-    ### Scaling and Imputation
-    def set_scaling(self, cols:list[str]
-        , strategy:ScalingStrategy=ScalingStrategy.NORMALIZE
-        , const:int=1) -> Self:
-        # const only matters if startegy is constant
-        self._execution_plan.add_step(
-            func = scale,
-            desc = BuiltinExecs.SCALE.value.format(strategy),
-            args = {"cols":cols, "strategy": strategy, "const":const},
-            is_fit = True
-        )
-        return self
-    
-    def set_impute(self, cols:list[str]
-        , strategy:ImputationStartegy=ImputationStartegy.MEDIAN
-        , const:int=1) -> Self:
-        
-        # const only matters if startegy is constant
-        self._execution_plan.add_step(
-            func = impute,
-            desc = BuiltinExecs.IMPUTE.value.format(strategy),
-            args = {"cols":cols, "strategy": strategy, "const":const},
-            is_fit = True
-        )
-        return self
-    
-    ### End of Scaling and Imputation
-
-    ### Encoding
-    def set_binary_encoding(self, cols:Optional[list[str]]=None) -> Self:
-        
-        if cols:
-            description = BuiltinExecs.BINARY_ENCODE.value
-        else:
-            description = "Automatically detect binary columns and turn them into [0,1] values by their order."
-
-        self._execution_plan.add_step(
-            func = binary_encode,
-            desc = description,
-            args = {"cols":cols},
-            is_fit = True
-        )
-        return self
-
-    def set_ordinal_encoding(self, mapping:dict[str, dict[str,int]], default:Optional[int]=None) -> Self:
-        
-        self._execution_plan.add_step(
-            func = ordinal_encode,
-            desc = BuiltinExecs.ORDINAL_ENCODE.value,
-            args = {"ordinal_mapping":mapping, "default": default},
-            is_fit = True
-        )
-        return self
-    
-    def set_ordinal_auto_encoding(self, cols:list[str], default:Optional[int]=None) -> Self:
-        
-        self._execution_plan.add_step(
-            func = ordinal_auto_encode,
-            desc = BuiltinExecs.ORDINAL_AUTO_ENCODE.value,
-            args = {"cols":cols, "default": default},
-            is_fit = True
-        )
-        return self
-    
-    def set_target_encoding(self, cols:list[str], min_samples_leaf:int=20, smoothing:int=10) -> Self:
-        
-        if self._is_ready():
-            self._execution_plan.add_step(
-                func = smooth_target_encode,
-                desc = BuiltinExecs.TARGET_ENCODE.value,
-                args = {"target":self.target, "cols": cols, "min_samples_leaf":min_samples_leaf
-                        , "smoothing":smoothing},
-                is_fit = True
-            )
-            return self
-        else:
-            raise ValueError("The target must be set before target encoding.")
-        
-    def set_one_hot_encoding(self, cols:Optional[list[str]]=None, separator:str="_") -> Self:
-        
-        if cols:
-            description = BuiltinExecs.ORDINAL_AUTO_ENCODE.value
-        else:
-            description = "Automatically detect string columns and one-hot encode them."
-
-        self._execution_plan.add_step(
-            func = one_hot_encode,
-            desc = description,
-            args = {"cols":cols, "separator": separator},
-            is_fit = True
-        )
-        return self
-    
-    def set_percentile_encoding(self, cols:list[str]) -> Self:
-
-        self._execution_plan.add_step(
-            func = percentile_encode,
-            desc = BuiltinExecs.PERCENTILE_ENCODE.value,
-            args = {"cols":cols},
-            is_fit = True
-        )
-        return self
-    
-    ### End of Encoding Section
-
-    ### Custom Actions
-
-    # Step and FitTransforms are differentiated in order to prevent error.
-    # A normal step is a function that takes in a dataframe, some other args, and 
-    # outputs a dataframe. Use add_custom_step for this case.
-    #
-    # A FitTransform is essentially a function that outputs the type FitTransform.
-    # This means that the transformation is dependent on information about the dataset (self.data),
-    # If this is the case, use add_custom_fit_transform
-
-    def add_custom_step(self
-        , func:Callable[Concatenate[pl.DataFrame, P], pl.DataFrame]
-        , desc:str
-        , args:dict[str, Any]
-        ) -> Self:
-        '''A normal step is a function that takes in a dataframe, some other args, and outputs a dataframe.'''
-        if "return" not in func.__annotations__:
-            logger.info("It is highly recommended that the custom step returns " 
-                        "a Polars dataframe. If this returns a TransformationResult, use add_custom_transform instead.")
-
-        self._execution_plan.add_custom_step(
-            func = func,
-            desc = desc,
-            args = args,
-            is_fit = False
-        )
-
-        return self
-    
-    def add_selector(self
-        , func:Callable[Concatenate[pl.DataFrame, P], list[str]]
-        , desc:str
-        , args:dict[str, Any]
-        ) -> Self:
-
-        if str(inspect.signature(func).return_annotation) != "list[str]":
-            raise TypeError("A selector function must explicitly provide a list[str] return type.")
-
-        if self._is_ready():
-            if "target" not in args:
-                args["target"] = self.target
-            self._execution_plan.add_selector_step(
-                func = func,
-                desc = desc,
-                args = args
-            )
-            return self
-        else:
-            raise ValueError("Selectors can only be queued after df and target are set.")
-    
-    def add_custom_selector(self
-        , func:Callable[Concatenate[pl.DataFrame, P], list[str]]
-        , desc:str
-        , args:dict[str, Any]
-        ) -> Self:
-        '''A normal step is a function that takes in a dataframe, some other args, and outputs a dataframe.'''
-        if str(inspect.signature(func).return_annotation) != "list[str]":
-            raise TypeError("A selector function must explicitly provide a list[str] return type.")
-
-        if self._is_ready():
-            if "target" not in args:
-                args["target"] = self.target
-            self._execution_plan.add_custom_selector_step(
-                func = func,
-                desc = desc,
-                args = args
-            )
-            return self
-        else:
-            raise ValueError("Selectors can only be queued after df and target are set.")
-
-        return self
-
-    def add_custom_fit_transform(self
-        , func:Callable[Concatenate[pl.DataFrame, P], FitTransform]
-        , desc:str
-        , args:dict[str, Any]
-        ) -> Self:
-        '''A FitTransform is essentially a function that outputs the type FitTransform.
-        This means that the transformation is dependent on information about the dataset (self.data),
-        '''
-
-        if "return" not in func.__annotations__:
-            logger.info("It is highly recommended that the custom transform returns "
-                        "a type that inherits from FitTransform in the transform.py module."
-                        "If this returns a pl.DataFrame, use add_custom_step instead.")
-
-        self._execution_plan.add_custom_step(
-            func = func,
-            desc = desc,
-            args = args,
-            is_fit = True
-        )
-
-        return self
-
-    ### End of Custom Actions
-
-
-    def _process_fit_in_build(self, step:ExecStep) -> None:
-
-        apply_transf:Callable[Concatenate[pl.DataFrame, P], FitTransform] 
-        apply_transf = getattr(importlib.import_module(step.module), step.name)
-        rec: FitRecord
-        self.data, rec = apply_transf(self.data, **step.args)
-        new_step = ExecStep(
-            name = step.name,
-            module = "N/A",
-            desc = step.desc, # 
-            # args = step.args, # don't need this when applying
-            is_fit = True,
-            fit_name = type(rec).__name__,
-            fit_module = rec.__module__,
-            fit_record = rec,
-            is_custom = step.is_custom
-        )
-        self._blueprint.add(new_step)
-
-    def _process_selector_in_build(self, step:ExecStep) -> None:
-
-        selector:Callable[Concatenate[pl.DataFrame, P], list[str]]
-        selector = getattr(importlib.import_module(step.module), step.name)
-        selected_cols:list[str] = selector(self.data, **step.args)
-        if self.target in selected_cols:
-            self.data = self.data.select(selected_cols)
-        else:
-            self.data = self.data.select(selected_cols + [self.target])
-
-        logger.info(f"The following features are kept: {selected_cols[:10]} + ... Only showing top 10.")
-        self._blueprint.add_step(
-            func = _select_cols,
-            desc = step.desc,
-            args = {"cols": selected_cols, "target": self.target}
-        )
-
-    def build(self) -> pl.DataFrame:
-        '''Build according to the steps.
-            Arguments:
-                df: Another chance to set input df if it has not been set.
-
-            Returns:
-                A dataframe.
-        
-        '''
-        n = len(self._execution_plan)
-        logger.info(f"Starting to build. Total steps: {n}.")
-        if not self._is_ready():
-            raise ValueError(f"Dataframe is not set properly, or the target {self.target} is not found "
-                             "in the dataframe. Cannot build without target.")
-        
-        if self._built:
-            logger.warning("The PipeBuilder is built once already. It is not intended to be built again. "
-                           "To avoid unexpected behavior, construct a new pipe only after calling .clear().")
-        
-        i = 0
-        # Todo! If something failed, save a backup dataframe to a temp folder.
-        while not self._execution_plan.is_empty():
-            i += 1
-            step = self._execution_plan.popleft()
-            logger.info(f"|{i}/{n}|: Step: {step.name} | is_fit: {step.is_fit} | is_selector: {step.is_selector}")
-            start = perf_counter()
-            success = True
-
-            if step.is_selector:
-                self._process_selector_in_build(step)
-            elif step.is_fit:
-                self._process_fit_in_build(step)
-            else: # Regular, canonical steps.
-                apply_func:Callable[Concatenate[pl.DataFrame, P], pl.DataFrame]  
-                apply_func = getattr(importlib.import_module(step.module), step.name)
-                self.data = self.data.pipe(apply_func, **step.args)
-                self._blueprint.add(step)
-
-            end = perf_counter()
-            logger.info(f"|{i}/{n}|: Finished in {end-start:.2f}s | Success: {success}")
-
-        logger.info("Build success. A blueprint has been built and can be viewed by calling .blueprint(), "
-                    "and can be saved as a json by calling .write()")
-
-        self._built = True
-        return self.data
-    
-    def get_final_data(self) -> Optional[pl.DataFrame]:
-        if self._built:
-            return self.data.clone()
-        else:
-            logger.info("Pipeline has not been built. There cannot be any final data.")
-            return None
-    
-    # Rename this in the future?
-    def apply(self, df:pl.DataFrame|pd.DataFrame) -> pl.DataFrame:
-        if not self._built:
-            raise ValueError("The builder must be built before applying it to new datasets.")
-        
-        if isinstance(df, pd.DataFrame):
-            logger.warning("Found input to be a Pandas dataframe. Turning it into a Polars dataframe.")
-            try:
-                input_df:pl.DataFrame = pl.from_pandas(df)
-            except Exception as e:
-                logger.error(e)
-        else:
-            input_df:pl.DataFrame = df
-
-        n = len(self._blueprint)
-        step:ExecStep
-        for i, step in enumerate(self._blueprint):
-            logger.info(f"|{i+1}/{n}|: Performing Step: {step.name} | is_fit: {step.is_fit}")
-            start = perf_counter()
-            success = True
-            if step.is_fit:
-                try:
-                    rec:FitRecord = step.fit_record
-                    input_df = input_df.pipe(rec.transform)
-                except Exception as e:
-                    success = False
-                    logger.error(e)
-            else:
-                apply_func:Callable[Concatenate[pl.DataFrame, P], pl.DataFrame] 
-                apply_func = getattr(importlib.import_module(step.module), step.name)
-                input_df = input_df.pipe(apply_func, **step.args)
-
-            end = perf_counter()
-            logger.info(f"|{i+1}/{n}|: Finished in {end-start:.2f}s | Success: {success}")
-        
-        return input_df
-
-    def blueprint(self):
-        return print(self._blueprint)
-        
-    def write(self, name:str="") -> None:
-        if self._blueprint.is_empty():
-            logger.warning("Blueprint is empty. Nothing is done.")
-            return
-
-        directory = "./blueprints/"
-        if name == "":
-            name += self.project_name + ".json"
-            logger.info(f"No name is specified, using project name ({name}) as default.")
-        else:
-            if not name.endswith(".json"):
-                name += ".json"
-
-        if not os.path.isdir(directory):
-            logger.info("Local ./blueprints/ directory is not found. It will be created.")
-            os.mkdir(directory)
-        try:
-            destination = directory+name
-            with open(destination, "wb") as f:
-                data = orjson.dumps(self._blueprint, option=orjson.OPT_NON_STR_KEYS|orjson.OPT_SERIALIZE_NUMPY)
-                f.write(data)
-
-            logger.info(f"Successfully saved to {destination}.")
-        except Exception as e:
-            logger.error(e)
-
-    def from_blueprint(self, path:str|Path):
-        logger.info("Reading from a blueprint. The builder will reset itself.")
-        self.clear()
-        try:
-            f = open(path, "rb")
-            data = orjson.loads(f.read())
-            f.close()
-            steps:list[dict[str, Any]] = data["steps"]
-            self.target = data["target"]
-            for s in steps:
-                if s["is_fit"]: # Need to recreate TransformRecord objects from dict
-                    name = s.get("fit_name", None)
-                    module = s.get("fit_module", None)
-                    record = s.get("fit_record", None)
-                    if (name is not None) or (module is not None) or (record is not None):
-                        if (name is None) or (module is None) or (record is None):
-                            raise ValueError(f"Something went wrong with the FitRecord: {s['name']}. "
-                                             "All of fit_name, fit_module and fit_record fields must not be null.")
-                    # Get the class the FitRecord belongs to.
-                    c = getattr(importlib.import_module(module), name)
-                    # Create an instance of c
-                    rec = c(**record) # Turn this json into a real Python object.
-                    s["fit_record"] = rec # Set "fit_record" field to be the object, not the dict.
-
-                self._blueprint.add(ExecStep(**s))
-
-            self._built = True
-            logger.info("Successfully read from a blueprint.")
-        except Exception as e:
-            logger.error(e)
-
-    ### End of Building section
-
-
+#                 self.data = pl.from_pandas(df).lazy() # Keep it lazy for internal stuff.
+#                 df = df.iloc[0:0]
+#             elif isinstance(df, pl.DataFrame, pl.LazyFrame):
+#                 self.data = df # Keep it lazy for internal stuff
+#             else: # Try this..
+#                 self.data = pl.DataFrame(df).lazy() # Keep it lazy for internal stuff
+#         except Exception as e:
+#             logger.error(e)
+
+#         return Self
+    
+#     def set_data_and_target(self, df:Any, target:str) -> Self:
+#         '''
+#             df: Any data that is p
+#         '''
+#         _ = self.set_target(target)        
+#         _ = self.set_data(df)
+#         if target not in self.data.columns:
+#             raise ValueError("Target is not found in the dataframe.")
+        
+#         self.target = target
+#         return self 
+
+#     # def from_csv(self, path:str|Path, **csv_args) -> Self:
+#     #     '''
+        
+#     #     '''
+#     #     try:
+#     #         self.data = pl.read_csv(path, **csv_args)
+#     #         return Self
+#     #     except Exception as e:
+#     #         logger.error(e)
+
+#     # def from_parquet(self, path:str|Path, **parquet_args) -> Self:
+#     #     '''
+        
+#     #     '''
+#     #     try:
+#     #         self.data = pl.read_parquet(path, **parquet_args)
+#     #         return Self
+#     #     except Exception as e:
+#     #         logger.error(e)
+    
+#     # def from_json(self, path:str|Path, **json_args) -> Self:
+#     #     '''
+        
+#     #     '''
+#     #     try:
+#     #         self.data = pl.read_json(path, **json_args)
+#     #         return Self
+#     #     except Exception as e:
+#     #         logger.error(e)
+
+#     # def from_excel(self, path:str|Path, **excel_args) -> Self:
+#     #     '''
+        
+#     #     '''
+#     #     try:
+#     #         self.data = pl.read_json(path, **excel_args)
+#     #         return Self
+#     #     except Exception as e:
+#     #         logger.error(e)
+#     ### End of I/O
+    
+#     ### Miscellaneous
+#     def show(self):
+#         print(self)
+
+#     def find(self, name:str) -> None:
+#         found = self._execution_plan.find(name)
+#         for i in found:
+#             print(f"Step at index {i}:")
+#             print(self._execution_plan.steps[i])
+
+#     # Set, Remove, in a safe way.
+
+#     def clear(self):
+#         if self.data is not None:
+#             self.data = self.data.clear()
+#         self._execution_plan.clear()
+#         self._blueprint.clear()
+#         self._built = False
+
+#     def select_cols(self, cols:list[str]) -> Self:
+#         if self._is_ready():
+#             self._execution_plan.add_step(
+#                 func = _select_cols,
+#                 desc = BuiltinExecs.SELECT.value,
+#                 args = {"cols":cols, "target":self.target}
+#             )
+#             return self
+#         else:
+#             raise ValueError("Target must be set before setting column selections.")
+    
+#     def set_lower_cols(self) -> Self:
+#         self._execution_plan.add_step(
+#             func = _lower_columns,
+#             desc = BuiltinExecs.LOWER.value,
+#             args = {}
+#         )
+#         return self
+
+#     ### End of Miscellaneous
+
+#     ### Checks
+#     def _is_ready(self) -> bool:
+#         if self.data is None:
+#             return False
+        
+#         return self.target != "" and self.target in self.data.columns
+    
+#     ### End of Checks.
+
+#     ### Project meta data section
+#     def set_project_name(self, project_name:str) -> Self:
+#         if project_name == "":
+#             raise ValueError("Project name cannot be empty.")
+#         self.project_name = project_name
+#         return self
+
+#     ### End of project meta data section
+    
+#     ### Column removal section
+#     def set_null_removal(self, threshold:float) -> Self:
+#         if threshold > 1 or threshold <= 0:
+#             raise ValueError("Threshold for null removal must be between 0 and 1.")
+
+#         self._execution_plan.add_step(
+#             func = null_removal ,
+#             desc = BuiltinExecs.NULL_REMOVAL.value.format(threshold*100),
+#             args = {"threshold":threshold}  
+#         )
+#         return self
+    
+#     def set_var_removal(self, threshold:float) -> Self:
+#         if threshold <= 0:
+#             raise ValueError("Threshold for var removal must be positive.")
+        
+#         if self._is_ready():
+#             self._execution_plan.add_step(
+#                 func = var_removal,
+#                 desc = BuiltinExecs.VAR_REMOVAL.value.format(threshold),
+#                 args = {"threshold":threshold, "target":self.target},
+#             )
+#             return self
+#         else:
+#             raise ValueError("Target must be set before setting var removal.")
+    
+#     def set_const_removal(self, include_null:bool=True) -> Self:
+        
+#         self._execution_plan.add_step(
+#             func = constant_removal,
+#             desc = BuiltinExecs.CONST_REMOVAL.value,
+#             args = {"include_null":include_null},
+#         )
+#         return self
+    
+#     def set_unique_removal(self, threshold:float=0.9) -> Self:
+#         if threshold > 1 or threshold <= 0:
+#             raise ValueError("Threshold for unique removal must be between 0 and 1.")
+
+#         self._execution_plan.add_step(
+#             func = unique_removal ,
+#             desc = BuiltinExecs.UNIQUE_REMOVAL.value.format(threshold*100),
+#             args = {"threshold":threshold}  
+#         )
+#         return self 
+    
+#     def set_regex_removal(self, pat:str, lowercase:bool=False) -> Self:
+#         '''Removes columns that satisfies the regex rule. May optionally only check on lowercased column names.'''
+#         description = BuiltinExecs.REGX_REMOVAL.value.format(pat)
+#         if lowercase:
+#             description += ". Everything will be lowercased."
+
+#         self._execution_plan.add_step(
+#             func = regex_removal,
+#             desc = description,
+#             args = {"pat":pat, "lowercase": lowercase},
+#         )
+#         return self
+    
+#     def set_col_removal(self, cols:list[str]) -> Self:
+#         '''Removes the given columns.'''
+#         self._execution_plan.add_step(
+#             func = remove_if_exists,
+#             desc = BuiltinExecs.COL_REMOVAL.value,
+#             args = {"to_drop":cols},
+#         )
+#         return self
+    
+#     def set_date_removal(self) -> Self:
+#         '''Removes columns that are inferred to be dates.'''
+#         self._execution_plan.add_step(
+#             func = date_removal,
+#             desc = BuiltinExecs.DATE_REMOVAL.value,
+#             args = {}
+#         )
+#         return self
+    
+#     def set_non_numeric_removal(self) -> Self:
+#         self._execution_plan.add_step(
+#             func = non_numeric_removal ,
+#             desc = BuiltinExecs.NON_NUMERIC_REMOVAL.value,
+#             args = {}
+#         )
+#         return self 
+        
+#     ### End of column removal section
+
+#     ### Scaling and Imputation
+#     def set_scaling(self, cols:list[str]
+#         , strategy:ScalingStrategy=ScalingStrategy.NORMALIZE
+#         , const:int=1) -> Self:
+#         # const only matters if startegy is constant
+#         self._execution_plan.add_step(
+#             func = scale,
+#             desc = BuiltinExecs.SCALE.value.format(strategy),
+#             args = {"cols":cols, "strategy": strategy, "const":const},
+#             is_fit = True
+#         )
+#         return self
+    
+#     def set_impute(self, cols:list[str]
+#         , strategy:ImputationStartegy=ImputationStartegy.MEDIAN
+#         , const:int=1) -> Self:
+        
+#         # const only matters if startegy is constant
+#         self._execution_plan.add_step(
+#             func = impute,
+#             desc = BuiltinExecs.IMPUTE.value.format(strategy),
+#             args = {"cols":cols, "strategy": strategy, "const":const},
+#             is_fit = True
+#         )
+#         return self
+    
+#     ### End of Scaling and Imputation
+
+#     ### Encoding
+#     def set_binary_encoding(self, cols:Optional[list[str]]=None) -> Self:
+        
+#         if cols:
+#             description = BuiltinExecs.BINARY_ENCODE.value
+#         else:
+#             description = "Automatically detect binary columns and turn them into [0,1] values by their order."
+
+#         self._execution_plan.add_step(
+#             func = binary_encode,
+#             desc = description,
+#             args = {"cols":cols},
+#             is_fit = True
+#         )
+#         return self
+
+#     def set_ordinal_encoding(self, mapping:dict[str, dict[str,int]], default:Optional[int]=None) -> Self:
+        
+#         self._execution_plan.add_step(
+#             func = ordinal_encode,
+#             desc = BuiltinExecs.ORDINAL_ENCODE.value,
+#             args = {"ordinal_mapping":mapping, "default": default},
+#             is_fit = True
+#         )
+#         return self
+    
+#     def set_ordinal_auto_encoding(self, cols:list[str], default:Optional[int]=None) -> Self:
+        
+#         self._execution_plan.add_step(
+#             func = ordinal_auto_encode,
+#             desc = BuiltinExecs.ORDINAL_AUTO_ENCODE.value,
+#             args = {"cols":cols, "default": default},
+#             is_fit = True
+#         )
+#         return self
+    
+#     def set_target_encoding(self, cols:list[str], min_samples_leaf:int=20, smoothing:int=10) -> Self:
+        
+#         if self._is_ready():
+#             self._execution_plan.add_step(
+#                 func = smooth_target_encode,
+#                 desc = BuiltinExecs.TARGET_ENCODE.value,
+#                 args = {"target":self.target, "cols": cols, "min_samples_leaf":min_samples_leaf
+#                         , "smoothing":smoothing},
+#                 is_fit = True
+#             )
+#             return self
+#         else:
+#             raise ValueError("The target must be set before target encoding.")
+        
+#     def set_one_hot_encoding(self, cols:Optional[list[str]]=None, separator:str="_") -> Self:
+        
+#         if cols:
+#             description = BuiltinExecs.ORDINAL_AUTO_ENCODE.value
+#         else:
+#             description = "Automatically detect string columns and one-hot encode them."
+
+#         self._execution_plan.add_step(
+#             func = one_hot_encode,
+#             desc = description,
+#             args = {"cols":cols, "separator": separator},
+#             is_fit = True
+#         )
+#         return self
+    
+#     # def set_percentile_encoding(self, cols:list[str]) -> Self:
+
+#     #     self._execution_plan.add_step(
+#     #         func = percentile_encode,
+#     #         desc = BuiltinExecs.PERCENTILE_ENCODE.value,
+#     #         args = {"cols":cols},
+#     #         is_fit = True
+#     #     )
+#     #     return self
+    
+#     ### End of Encoding Section
+
+#     ### Custom Actions
+
+#     # Step and FitTransforms are differentiated in order to prevent error.
+#     # A normal step is a function that takes in a dataframe, some other args, and 
+#     # outputs a dataframe. Use add_custom_step for this case.
+#     #
+#     # A FitTransform is essentially a function that outputs the type FitTransform.
+#     # This means that the transformation is dependent on information about the dataset (self.data),
+#     # If this is the case, use add_custom_fit_transform
+
+#     def add_custom_step(self
+#         , func:Callable[Concatenate[PolarsFrame, P], PolarsFrame]
+#         , desc:str
+#         , args:dict[str, Any]
+#         ) -> Self:
+#         '''A normal step is a function that takes in a dataframe, some other args, and outputs a dataframe.'''
+#         if "return" not in func.__annotations__:
+#             logger.info("It is highly recommended that the custom step returns " 
+#                         "a Polars dataframe. If this returns a TransformationResult, use add_custom_transform instead.")
+
+#         self._execution_plan.add_custom_step(
+#             func = func,
+#             desc = desc,
+#             args = args,
+#             is_fit = False
+#         )
+
+#         return self
+    
+#     def add_selector(self
+#         , func:Callable[Concatenate[PolarsFrame, P], list[str]]
+#         , desc:str
+#         , args:dict[str, Any]
+#         ) -> Self:
+
+#         if str(inspect.signature(func).return_annotation) != "list[str]":
+#             raise TypeError("A selector function must explicitly provide a list[str] return type.")
+
+#         if self._is_ready():
+#             if "target" not in args:
+#                 args["target"] = self.target
+#             self._execution_plan.add_selector_step(
+#                 func = func,
+#                 desc = desc,
+#                 args = args
+#             )
+#             return self
+#         else:
+#             raise ValueError("Selectors can only be queued after df and target are set.")
+    
+#     def add_custom_selector(self
+#         , func:Callable[Concatenate[PolarsFrame, P], list[str]]
+#         , desc:str
+#         , args:dict[str, Any]
+#         ) -> Self:
+#         '''A normal step is a function that takes in a dataframe, some other args, and outputs a dataframe.'''
+#         if str(inspect.signature(func).return_annotation) != "list[str]":
+#             raise TypeError("A selector function must explicitly provide a list[str] return type.")
+
+#         if self._is_ready():
+#             if "target" not in args:
+#                 args["target"] = self.target
+#             self._execution_plan.add_custom_selector_step(
+#                 func = func,
+#                 desc = desc,
+#                 args = args
+#             )
+#             return self
+#         else:
+#             raise ValueError("Selectors can only be queued after df and target are set.")
+
+#     def add_custom_fit_transform(self
+#         , func:Callable[Concatenate[PolarsFrame, P], FitTransform]
+#         , desc:str
+#         , args:dict[str, Any]
+#         ) -> Self:
+#         '''A FitTransform is essentially a function that outputs the type FitTransform.
+#         This means that the transformation is dependent on information about the dataset (self.data),
+#         '''
+
+#         if "return" not in func.__annotations__:
+#             logger.info("It is highly recommended that the custom transform returns "
+#                         "a type that inherits from FitTransform in the transform.py module."
+#                         "If this returns a pl.DataFrame, use add_custom_step instead.")
+
+#         self._execution_plan.add_custom_step(
+#             func = func,
+#             desc = desc,
+#             args = args,
+#             is_fit = True
+#         )
+
+#         return self
+
+#     ### End of Custom Actions
+
+
+#     def _process_fit_in_build(self, step:ExecStep) -> None:
+
+#         apply_transf:Callable[Concatenate[PolarsFrame, P], FitTransform] 
+#         apply_transf = getattr(importlib.import_module(step.module), step.name)
+#         rec: FitRecord
+#         self.data, rec = self.data.pipe(apply_transf, **step.args)
+#         new_step = ExecStep(
+#             name = step.name,
+#             module = "N/A",
+#             desc = step.desc, # 
+#             # args = step.args, # don't need args when we apply (transform)
+#             is_fit = True,
+#             fit_name = type(rec).__name__,
+#             fit_module = rec.__module__,
+#             fit_record = rec,
+#             is_custom = step.is_custom
+#         )
+#         self._blueprint.add(new_step)
+
+#     def _process_selector_in_build(self, step:ExecStep) -> None:
+
+#         selector:Callable[Concatenate[pl.DataFrame, P], list[str]]
+#         selector = getattr(importlib.import_module(step.module), step.name)
+#         selected_cols:list[str] = selector(self.data, **step.args)
+#         to_select = selected_cols.copy()
+#         if self.target not in selected_cols:
+#             to_select.append(self.target)
+        
+#         # In this stage, target should be in to_select and in df.columns.
+#         self.data = self.data.pipe(_select_cols, to_select, self.target)
+
+#         logger.info(f"The following features are kept: {selected_cols[:10]} + ... Only showing top 10.")
+#         self._blueprint.add_step(
+#             func = _select_cols,
+#             desc = step.desc,
+#             args = {"cols": selected_cols, "target": self.target}
+#         )
+
+
+#     # RETHINK how to build.
+#     # Maybe we should cast df to lazy, then use Polars's Pipe. But how to save Polars's Pipe?
+#     def build_2(self) -> pl.DataFrame:
+#         pass
+
+#     def build(self) -> pl.DataFrame:
+#         '''Build according to the steps.
+#             Arguments:
+#                 df: Another chance to set input df if it has not been set.
+
+#             Returns:
+#                 A dataframe.
+        
+#         '''
+#         n = len(self._execution_plan)
+#         logger.info(f"Starting to build. Total steps: {n}.")
+#         if not self._is_ready():
+#             raise ValueError(f"Dataframe is not set properly, or the target {self.target} is not found "
+#                              "in the dataframe. Cannot build without target.")
+        
+#         if self._built:
+#             logger.warning("The PipeBuilder is built once already. It is not intended to be built again. "
+#                            "To avoid unexpected behavior, construct a new pipe only after calling .clear().")
+        
+#         i = 0
+#         # Todo! If something failed, save a backup dataframe to a temp folder.
+#         while not self._execution_plan.is_empty():
+#             i += 1
+#             step = self._execution_plan.popleft()
+#             logger.info(f"|{i}/{n}|: Step: {step.name} | is_fit: {step.is_fit} | is_selector: {step.is_selector}")
+#             start = perf_counter()
+#             success = True
+
+#             if step.is_selector:
+#                 self._process_selector_in_build(step)
+#             elif step.is_fit:
+#                 self._process_fit_in_build(step)
+#             else: # Regular, canonical steps.
+#                 apply_func:Callable[Concatenate[PolarsFrame, P], PolarsFrame]  
+#                 apply_func = getattr(importlib.import_module(step.module), step.name)
+#                 self.data = self.data.pipe(apply_func, **step.args)
+#                 self._blueprint.add(step)
+
+#             end = perf_counter()
+#             logger.info(f"|{i}/{n}|: Finished in {end-start:.2f}s | Success: {success}")
+
+#         logger.info("Build success. A blueprint has been built and can be viewed by calling .blueprint(), "
+#                     "and can be saved as a json by calling .write()")
+
+#         self._built = True
+#         return self.data
+    
+#     # Rename this in the future?
+#     def apply(self, df:pl.DataFrame|pd.DataFrame) -> pl.DataFrame:
+#         if not self._built:
+#             raise ValueError("The builder must be built before applying it to new datasets.")
+#         try:
+#             if isinstance(df, pd.DataFrame):
+#                 logger.warning("Found input to be a Pandas dataframe. Turning it into a Polars dataframe.")
+#                 try:
+#                     input_df:pl.DataFrame = pl.from_pandas(df)
+#                 except Exception as e:
+#                     logger.error(e)
+#             elif isinstance(df, pl.DataFrame):
+#                 input_df:pl.DataFrame = df
+#             else:
+#                 input_df:pl.DataFrame = pl.DataFrame(df)
+#         except Exception as e:
+#             logger.error(e)
+
+#         n = len(self._blueprint)
+#         step:ExecStep
+#         for i, step in enumerate(self._blueprint):
+#             logger.info(f"|{i+1}/{n}|: Performing Step: {step.name} | is_fit: {step.is_fit}")
+#             start = perf_counter()
+#             success = True
+#             if step.is_fit:
+#                 try:
+#                     rec:FitRecord = step.fit_record
+#                     input_df = input_df.pipe(rec.transform)
+#                 except Exception as e:
+#                     success = False
+#                     logger.error(e)
+#             else:
+#                 apply_func:Callable[Concatenate[pl.DataFrame, P], pl.DataFrame] 
+#                 apply_func = getattr(importlib.import_module(step.module), step.name)
+#                 input_df = input_df.pipe(apply_func, **step.args)
+
+#             end = perf_counter()
+#             logger.info(f"|{i+1}/{n}|: Finished in {end-start:.2f}s | Success: {success}")
+        
+#         return input_df
+
+#     def blueprint(self):
+#         return print(self._blueprint)
+        
+#     def write(self, name:str="") -> None:
+#         if self._blueprint.is_empty():
+#             logger.warning("Blueprint is empty. Nothing is done.")
+#             return
+
+#         directory = "./blueprints/"
+#         if name == "":
+#             name += self.project_name + ".json"
+#             logger.info(f"No name is specified, using project name ({name}) as default.")
+#         else:
+#             if not name.endswith(".json"):
+#                 name += ".json"
+
+#         if not os.path.isdir(directory):
+#             logger.info("Local ./blueprints/ directory is not found. It will be created.")
+#             os.mkdir(directory)
+#         try:
+#             destination = directory+name
+#             with open(destination, "wb") as f:
+#                 data = orjson.dumps(self._blueprint, option=orjson.OPT_NON_STR_KEYS|orjson.OPT_SERIALIZE_NUMPY)
+#                 f.write(data)
+
+#             logger.info(f"Successfully saved to {destination}.")
+#         except Exception as e:
+#             logger.error(e)
+
+#     def from_blueprint(self, input_file:str|Path|bytes) -> Self:
+#         logger.info("Reading from a blueprint. The builder will reset itself.")
+#         self.clear()
+#         try:
+#             if isinstance(input_file, bytes):
+#                 data = orjson.loads(input_file)
+#             else:
+#                 f = open(input_file, "rb")
+#                 data = orjson.loads(f.read())
+#                 f.close()
+            
+#             steps:list[dict[str, Any]] = data["steps"]
+#             self.target = data["target"]
+#             for s in steps:
+#                 if s["is_fit"]: # Need to recreate TransformRecord objects from dict
+#                     name = s.get("fit_name", None)
+#                     module = s.get("fit_module", None)
+#                     record = s.get("fit_record", None)
+#                     if (name is not None) or (module is not None) or (record is not None):
+#                         if (name is None) or (module is None) or (record is None):
+#                             raise ValueError(f"Something went wrong with the FitRecord: {s['name']}. "
+#                                              "All of fit_name, fit_module and fit_record fields must not be null.")
+#                     # Get the class the FitRecord belongs to.
+#                     c = getattr(importlib.import_module(module), name)
+#                     # Create an instance of c
+#                     rec = c(**record) # Turn this json into a real Python object.
+#                     s["fit_record"] = rec # Set "fit_record" field to be the object, not the dict.
+
+#                 self._blueprint.add(ExecStep(**s))
+
+#             self._built = True
+#             logger.info("Successfully read from a blueprint.")
+#         except Exception as e:
+#             logger.error(e)
 
+#         return self
+#     ### End of Building section
```

### Comparing `dsds-0.0.1/src/dsds/eda_text.py` & `dsds-0.0.15/src/dsds/eda_text.py`

 * *Files identical despite different names*

### Comparing `dsds-0.0.1/src/dsds/fs.py` & `dsds-0.0.15/src/dsds/fs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,158 +1,161 @@
 from .prescreen import (
     discrete_inferral
     , get_numeric_cols
     , get_unique_count
 )
 
-import os
+from .type_alias import (
+    PolarsFrame
+    , MRMRStrategy
+    , CPU_COUNT
+    , clean_strategy_str
+)
+from .blueprint import( # Need this for Polars extension to work
+    Blueprint
+)
+
 import polars as pl
 import numpy as np
-from enum import Enum
-from typing import Final, Any, Optional, Tuple
+from typing import Any, Optional, Tuple
 from scipy.spatial import KDTree
 from scipy.special import fdtrc, psi
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from tqdm import tqdm
 
-# Everything named as a selector must return a list of str
-
-CPU_COUNT:Final[int] = os.cpu_count()
-# Some will return dataframe as output, some list of str
-
 def _conditional_entropy(
     df:pl.DataFrame
     , target:str
     , predictive:str
 ) -> Tuple[str, float]:
-    
-    # temp = df.groupby(predictive).agg(
-    #     pl.count().alias("prob(predictive)")
-    # ).with_columns(
-    #     pl.col("prob(predictive)") / len(df)
-    # )
 
     cond_entropy = df.groupby((target, predictive)).agg(
         pl.count()
     ).with_columns(
         (pl.col("count").sum().over(predictive) / len(df)).alias("prob(predictive)"),
         (pl.col("count") / pl.col("count").sum()).alias("prob(target,predictive)")
     ).select(
         (-((pl.col("prob(target,predictive)")/pl.col("prob(predictive)")).log() 
            * pl.col("prob(target,predictive)")).sum()) # This is the conditional entropy.
-    ).to_numpy()[0,0]
+    ).row(0)[0]
 
     return (predictive, cond_entropy)
 
-# NEED REVIEW FOR CORRECTNESS
+# !!!NEED REVIEW FOR CORRECTNESS
 def discrete_ig(
     df:pl.DataFrame
     , target:str
     , discrete_cols:Optional[list[str]] = None
     , n_threads:int = CPU_COUNT
 ) -> pl.DataFrame:
     '''The entropy here is "discrete entropy".
 
-        Computes the information gain: Entropy(target) - Conditional_Entropy(target|c), where c is a column in discrete_cols.
-        For more information, please take a look at https://en.wikipedia.org/wiki/Entropy_(information_theory)
+        Computes the information gain: Entropy(target) - Conditional_Entropy(target|c), where c is a column in 
+        discrete_cols. For more information, please take a look at https://en.wikipedia.org/wiki/Entropy_(information_theory)
 
-        Information gain defined in this way suffers from high cardinality (high uniqueness), and therefore a weighted information
-        gain is provided, weighted by (1 - unique_pct), where unique_pct represents the percentage of unique values in feature.
+        Information gain defined in this way suffers from high cardinality (high uniqueness), and therefore a weighted 
+        information gain is provided, weighted by (1 - unique_pct), where unique_pct represents the percentage of unique
+         values in feature.
 
-        Currently this only works for discrete columns and no method for continuous column is implemented yet.
+        Currently this only works for discrete columns. For continuous features vs discrete target, use mutual_info.
 
         Arguments:
-            df:
+            df: Eager frame only.
             target:
             discrete_cols: list of discrete columns.
             top_k: must be >= 0. If <= 0, the entire DataFrame will be returned.
             n_threads: 4, 8 ,16 will not make any real difference. But there is a difference between 0 and 4 threads. 
             
         Returns:
             a poalrs dataframe with information gain computed for each categorical column. 
     '''
     output = []
     discretes = []
     if isinstance(discrete_cols, list):
         discretes.extend(discrete_cols)
     else: # If discrete_cols is not passed, infer it
         discretes.extend(discrete_inferral(df, exclude=[target]))
-    
+
     # Compute target entropy. This only needs to be done once.
     target_entropy = df.groupby(target).agg(
                         (pl.count()).alias("prob(target)") / len(df)
                     ).get_column("prob(target)").entropy()
 
     # Get unique count for selected columns. This is because higher unique percentage may skew information gain
     unique_count = get_unique_count(df.select(discretes)).with_columns(
         (pl.col("n_unique") / len(df)).alias("unique_pct")
     ).rename({"column":"feature"})
 
-    with ThreadPoolExecutor(max_workers=n_threads) as ex: # 10% gain actually. Small but ok.
-        futures = (ex.submit(_conditional_entropy, df, target, predictive) for predictive in discretes)
-        with tqdm(total=len(discretes)) as pbar:
-            for res in as_completed(futures):
-                ig = res.result()
-                output.append(ig)
-                pbar.update(1)
+    with ThreadPoolExecutor(max_workers=n_threads) as ex: # 10% speed gain ? Need to retest this..
+        pbar = tqdm(total=len(discretes), desc = "discrete_ig")
+        for future in as_completed(ex.submit(_conditional_entropy, df, target, pred) for pred in discretes):
+            ig = future.result()
+            output.append(ig)
+            pbar.update(1)
+
+        pbar.close()
 
-    output_df = pl.from_records(output, schema=["feature", "conditional_entropy"])\
+    return pl.from_records(output, schema=["feature", "conditional_entropy"])\
         .with_columns(
             pl.lit(target_entropy).alias("target_entropy"),
             (pl.lit(target_entropy) - pl.col("conditional_entropy")).alias("information_gain")
         ).join(unique_count, on="feature")\
         .select("feature", "target_entropy", "conditional_entropy", "unique_pct", "information_gain")\
         .with_columns(
             ((1 - pl.col("unique_pct")) * pl.col("information_gain")).alias("weighted_information_gain")
         )
 
-    return output_df
-
 discrete_mi = discrete_ig
 
 def discrete_ig_selector(
-    df:pl.DataFrame
+    df:PolarsFrame
     , target:str
     , top_k:int
     , n_threads:int = CPU_COUNT
-) -> list[str]:
+) -> PolarsFrame:
     discrete_cols = discrete_inferral(df, exclude=[target])
-    # They are not examined by this feature selection method. So keep them.
-    complement = [f for f in df.columns if f not in discrete_cols and f != target] 
-    ig = discrete_ig(df, target, discrete_cols, n_threads)\
+
+    is_lazy = isinstance(df, pl.LazyFrame)
+    if is_lazy:
+        input_data:pl.DataFrame = df.collect()
+    else:
+        input_data:pl.DataFrame = df
+
+    ig = discrete_ig(input_data, target, discrete_cols, n_threads)\
             .top_k(by="information_gain", k = top_k)
 
+    complement = [f for f in input_data.columns if f not in discrete_cols]
     selected = ig.get_column("feature").to_list()
-    print(f"Selected {len(selected)} features. There are {len(complement)} features the algorithm "
+    print(f"Selected {len(selected)} features. There are {len(complement)} columns the algorithm "
         "cannot process. They are also returned.")
 
-    return selected + complement
-
+    if is_lazy:
+        return df.blueprint.select(selected + complement)
+    return df.select(selected + complement)
 
 def mutual_info(
     df:pl.DataFrame
-    , conti_cols:list[str]
     , target:str
+    , conti_cols:list[str]
     , n_neighbors:int=3
     , random_state:int=42
     , n_threads:int=CPU_COUNT
 ) -> pl.DataFrame:
     '''Approximates mutual information (information gain) between the continuous variables and the target.
 
         This is essentially a "copy-and-paste" of the mutual_info_classif call in sklearn library. 
         There are a few important distinctions:
 
         1. This uses Scipy library's kdtree, instead of sklearn's kdtree and nearneighbors. 
         2. The use of Scipy enables us to use more cores. 
         3. There are less "checks" and "safeguards", meaning input data quality is expected to be "good".
-        4. Conti_cols are supposed to be "continuous" variables. In sklearn's mutual_info_classif, if you input a dense matrix X,
-            it will always be treated as continuous, and if X is sparse, it will be treated as discrete.
-        5. The method here is sklearn's method in the case of continous variable and discrete target, which is based on the method
-            described in sources.
-   
+        4. Conti_cols are supposed to be "continuous" variables. In sklearn's mutual_info_classif, if you input a dense 
+            matrix X, it will always be treated as continuous, and if X is sparse, it will be treated as discrete.
+        5. This method is based on method described the sources.
+
         Arguments:
             df:
             conti_cols: 
             target: list of discrete columns.
             n_neighbors:
             random_state: a random seed to generate small noise.
             n_threads: 
@@ -162,75 +165,87 @@
         Sources:
             (1). B. C. Ross “Mutual Information between Discrete and Continuous Data Sets”. PLoS ONE 9(2), 2014.\n
             (2). A. Kraskov, H. Stogbauer and P. Grassberger, “Estimating mutual information”. Phys. Rev. E 69, 2004.
             
     '''
     n = len(df)
     rng = np.random.default_rng(random_state)
-    target_col = df[target].to_numpy().ravel()
+    target_col = df.get_column(target).to_numpy().ravel()
     unique_targets = np.unique(target_col)
-    # parts = {t:df.filter((pl.col(target) == t)) for t in df[target].unique()}
     all_masks = {}
     for t in unique_targets:
         all_masks[t] = target_col == t
-        if len(df.filter(pl.col(target) == t)) <= n_neighbors:
+        if np.sum(all_masks[t]) <= n_neighbors:
             raise ValueError(f"The target class {t} must have more than {n_neighbors} values in the dataset.")        
 
     estimates = []
     psi_n_and_k = psi(n) + psi(n_neighbors)
     for col in tqdm(conti_cols, desc = "Mutual Info"):
-        c = df[col].to_numpy().reshape(-1,1)
-        c = c + (1e-10 * np.mean(c) * rng.standard_normal(size=c.shape))
+        c = df.get_column(col).cast(pl.Float64).to_numpy().reshape(-1,1)
+        # Add random noise here because if inpute data is too big, then adding
+        # a random matrix of the same size will require a lot of memory upfront.
+        c = c + (1e-10 * np.mean(c) * rng.standard_normal(size=c.shape)) 
         radius = np.empty(n)
         label_counts = np.empty(n)
         for t in unique_targets:
             mask = all_masks[t]
             c_masked = c[mask]
             kd1 = KDTree(data=c_masked, leafsize=40)
-            # dd = distances from the points the the k nearest points. +1 because this starts from 0. It is 1 off from sklearn's kdtree.
+            # dd = distances from the points the the k nearest points. +1 because this starts from 0. It is 1 off from 
+            # sklearn's kdtree.
             dd, _ = kd1.query(c_masked, k = n_neighbors + 1, workers=n_threads)
             radius[mask] = np.nextafter(dd[:, -1], 0)
             label_counts[mask] = np.sum(mask)
 
         kd2 = KDTree(data=c, leafsize=40) 
         m_all = kd2.query_ball_point(c, r = radius, return_length=True, workers=n_threads)
         estimates.append(
             max(0, psi_n_and_k - np.mean(psi(label_counts) + psi(m_all)))
         ) # smallest is 0
 
-    output = pl.from_records([conti_cols, estimates], schema=["feature", "estimated_mi"])
-    return output
+    return pl.from_records([conti_cols, estimates], schema=["feature", "estimated_mi"])
 
+# Selectors should always return target
 def mutual_info_selector(
-    df:pl.DataFrame
+    df:PolarsFrame
     , target:str
     , n_neighbors:int=3
     , random_state:int=42
     , n_threads:int=CPU_COUNT
     , top_k:int = 50
-) -> list[str]:
+) -> PolarsFrame:
     
-    nums = get_numeric_cols(df, exclude=[target])
-    complement = [f for f in df.columns if f not in nums and f != target]
-    mi_scores = mutual_info(df, nums, target, n_neighbors, random_state, n_threads)\
+    is_lazy = isinstance(df, pl.LazyFrame)
+    if is_lazy:
+        input_data:pl.DataFrame = df.collect()
+    else:
+        input_data:pl.DataFrame = df
+
+    nums = get_numeric_cols(input_data, exclude=[target])
+    complement = [f for f in input_data.columns if f not in nums]
+
+    mi_scores = mutual_info(input_data, target, nums, n_neighbors, random_state, n_threads)\
                 .top_k(by="estimated_mi", k = top_k)
 
     selected = mi_scores.get_column("feature").to_list()
-    print(f"Selected {len(selected)} features. There are {len(complement)} features the algorithm "
+    print(f"Selected {len(selected)} features. There are {len(complement)} columns the algorithm "
         "cannot process. They are also returned.")
-    return selected + complement
+    
+    if is_lazy:
+        return df.blueprint.select(selected + complement)
+    return df.select(selected + complement)
 
 def _f_score(
     df:pl.DataFrame
     , target:str
     , num_list:list[str]
 ) -> np.ndarray:
-    '''Same as f_classification, but returns a numpy array of f scores only.'''
+    '''Same as f_classif, but returns a numpy array of f scores only.'''
     
-    # See comments in f_classification
+    # See comments in f_classif
     step_one_expr:list[pl.Expr] = [pl.count().alias("cnt")]
     step_two_expr:list[pl.Expr] = []
     step_three_expr:list[pl.Expr] = []
     for n in num_list:
         n_avg:str = n + "_avg"
         n_tavg:str = n + "_tavg"
         n_var:str = n + "_var"
@@ -252,15 +267,15 @@
     n_classes = len(ref)
     df_btw_class = n_classes - 1 
     df_in_class = n_samples - n_classes
     # This is f-score, score in the order of num_list
     return ref.with_columns(step_two_expr).select(step_three_expr)\
             .to_numpy().ravel() * (df_in_class / df_btw_class)
 
-def f_classification(
+def f_classif(
     df:pl.DataFrame
     , target:str
     , num_cols:Optional[list[str]]=None
 ) -> pl.DataFrame:
     '''Computes ANOVA one way test, the f value/score and the p value. 
         Equivalent to f_classif in sklearn.feature_selection, but is more dataframe-friendly, 
         and performs better on bigger data.
@@ -316,96 +331,95 @@
     f_values = ref.with_columns(step_two_expr).select(step_three_expr)\
             .to_numpy().ravel() * (df_in_class / df_btw_class)
     # We should scale this by (df_in_class / df_btw_class) because we did not do this earlier
     # At this point, f_values should be a pretty small dataframe. 
     # Cast to numpy, so that fdtrc can process it properly.
 
     p_values = fdtrc(df_btw_class, df_in_class, f_values) # get p values 
-    return pl.from_records([num_list, f_values, p_values], schema=["feature","f_value","p_value"])
+    return pl.from_records((num_list, f_values, p_values), schema=["feature","f_value","p_value"])
 
 def f_score_selector(
-    df:pl.DataFrame
+    df:PolarsFrame
     , target:str
     , top_k:int
-) -> list[str]:
+) -> PolarsFrame:
     
-    nums = get_numeric_cols(df, exclude=[target])
+    is_lazy = isinstance(df, pl.LazyFrame)
+    if is_lazy:
+        input_data:pl.DataFrame = df.collect()
+    else:
+        input_data:pl.DataFrame = df
+
+    nums = get_numeric_cols(input_data, exclude=[target])
     # Non-numerical columns cannot be analyzed by mrmr. So add back in the end.
-    complement = [f for f in df.columns if f not in nums and f != target]
-    scores = _f_score(df, target, nums)
+    complement = [f for f in input_data.columns if f not in nums]
+
+    scores = _f_score(input_data, target, nums)
     temp_df = pl.DataFrame({"feature":nums, "fscore":scores}).top_k(
         by = "fscore", k = top_k
     )
     selected = temp_df.get_column("feature").to_list()
     
-    print(f"Selected {len(selected)} features. There are {len(complement)} features the algorithm "
+    print(f"Selected {len(selected)} features. There are {len(complement)} columns the algorithm "
     "cannot process. They are also returned.")
 
-    return selected + complement
-
+    if is_lazy:
+        return df.blueprint.select(selected + complement)
+    return df.select(selected + complement)
 
-class MRMR_STRATEGY(Enum):
-    F_SCORE = "F-SCORE"
-    RF = "RF"
-    XGB = "XGB"
-    MIS = "MIS"
-
-    def info(self) -> str:
-        if self.name == self.F_SCORE:
-            return "F Score"
-        elif self.name == self.RF:
-            return "Random Forest"
-        elif self.name == self.XGB:
-            return "XGBoost"
-        elif self.name == self.MIS:
-            return "Mutual Information Score"
-        else:
-            return "Unknown"
+#---- Below is MRMR
 
 def _mrmr_underlying_score(
     df:pl.DataFrame
     , target:str
     , num_list:list[str]
-    , strategy:MRMR_STRATEGY
+    , strategy:MRMRStrategy
     , params:dict[str,Any]
 ) -> np.ndarray:
     
-    print(f"Running {strategy.info()} to determine feature relevance...")
-    if strategy == MRMR_STRATEGY.F_SCORE:
+    print(f"Running {strategy} to determine feature relevance...")
+    s = clean_strategy_str(strategy)
+    if s in ("fscore", "f", "f_score"):
         scores = _f_score(df, target, num_list)
-    elif strategy == MRMR_STRATEGY.RF:
+    elif s in ("rf", "random_forest"):
         from sklearn.ensemble import RandomForestClassifier
         print("Random forest is not deterministic by default. Results may vary.")
         rf = RandomForestClassifier(**params)
         rf.fit(df[num_list].to_numpy(), df[target].to_numpy().ravel())
         scores = rf.feature_importances_
-    elif strategy == MRMR_STRATEGY.XGB:
+    elif s in ("xgb", "xgboost"):
         from xgboost import XGBClassifier
         print("XGB is not deterministic by default. Results may vary.")
         xgb = XGBClassifier(**params)
         xgb.fit(df[num_list].to_numpy(), df[target].to_numpy().ravel())
         scores = xgb.feature_importances_
-    elif strategy == MRMR_STRATEGY.MIS:
+    elif s in ("mis", "mutual_info_score"):
         scores = mutual_info(df, conti_cols=num_list, target=target).get_column("estimated_mi").to_numpy().ravel()
+    elif s in ("lgbm", "lightgbm"):
+        from lightgbm import LGBMClassifier
+        print("LightGBM is not deterministic by default. Results may vary.")
+        lgbm = LGBMClassifier(**params)
+        lgbm.fit(df[num_list].to_numpy(), df[target].to_numpy().ravel())
+        scores = lgbm.feature_importances_
     else: # Pythonic nonsense
         raise ValueError(f"The strategy {strategy} is not a valid MRMR Strategy.")
     
     return scores
 
 def mrmr(
     df:pl.DataFrame
     , target:str
     , k:int
     , num_cols:Optional[list[str]] = None
-    , strategy:MRMR_STRATEGY|str = MRMR_STRATEGY.F_SCORE
+    , strategy: MRMRStrategy = "fscore"
     , params:Optional[dict[str,Any]] = None
     , low_memory:bool=False
 ) -> list[str]:
-    '''Implements MRMR. Will add a few more strategies in the future. (Likely only strategies for numerators
-        , aka relevance)
+    '''Implements MRMR. Will add a few more strategies in the future. Likely only strategies for numerators
+        , aka relevance. Right now xgb, lgbm and rf strategies only work for classification problems.
 
         Currently this only supports classification.
 
         Arguments:
             df:
             target:
             k:
@@ -421,15 +435,15 @@
 
     num_list = []
     if isinstance(num_cols, list):
         num_list.extend(num_cols)
     else:
         num_list.extend(get_numeric_cols(df, exclude=[target]))
 
-    s = MRMR_STRATEGY(strategy) if isinstance(strategy, str) else strategy
+    s = clean_strategy_str(strategy)
     scores = _mrmr_underlying_score(df
                                     , target = target
                                     , num_list = num_list
                                     , strategy = s
                                     , params = {} if params is None else params
                                     )
 
@@ -439,17 +453,17 @@
         df_local = df.select(num_list).with_columns(
             (pl.col(f) - pl.col(f).mean())/pl.col(f).std() for f in num_list
         ) # Note that if we get a const column, the entire column will be NaN
 
     output_size = min(k, len(num_list))
     print(f"Found {len(num_list)} total features to select from. Proceeding to select top {output_size} features.")
     cumulating_abs_corr = np.zeros(len(num_list)) # For each feature at index i, we keep a cumulating sum
-    pbar = tqdm(total=output_size, desc = f"MRMR, {s}")
     top_idx = np.argmax(scores)
     selected = [num_list[top_idx]]
+    pbar = tqdm(total=output_size, desc = f"MRMR, {s}")
     pbar.update(1)
     for j in range(1, output_size): 
         argmax = -1
         current_max = -1
         last_selected_col = df_local.drop_in_place(selected[-1])
         if low_memory: # normalize if in low memory mode.
             last_selected_col = (last_selected_col - last_selected_col.mean())/last_selected_col.std()
@@ -472,42 +486,52 @@
                     current_max = new_score
                     argmax = i
 
         selected.append(num_list[argmax])
         pbar.update(1)
 
     pbar.close()
-    print("Output is sorted in order of selection. (The 1st feature selected is most important, the 2nd the 2nd most important, etc.)")
+    print("Output is sorted in order of selection (relevance).")
     return selected
 
 def mrmr_selector(
-    df:pl.DataFrame
+    df:PolarsFrame
     , target:str
     , top_k:int
-    , strategy:MRMR_STRATEGY|str = MRMR_STRATEGY.F_SCORE
+    , strategy:MRMRStrategy = "fscore"
     , params:Optional[dict[str,Any]] = None
     , low_memory:bool=False
-) -> list[str]:
+) -> PolarsFrame:
 
-    num_cols = get_numeric_cols(df, exclude=[target])
+    is_lazy = isinstance(df, pl.LazyFrame)
+    if is_lazy:
+        input_data:pl.DataFrame = df.collect()
+    else:
+        input_data:pl.DataFrame = df
+
+    num_cols = get_numeric_cols(input_data, exclude=[target])
     # Non-numerical columns cannot be analyzed by mrmr. So add back in the end.
-    complement = [f for f in df.columns if f not in num_cols and f != target]
-    s = MRMR_STRATEGY(strategy) if isinstance(strategy, str) else strategy
-    selected = mrmr(df, target, top_k, num_cols, s, params, low_memory)
+    complement = [f for f in input_data.columns if f not in num_cols]
+
+    s = clean_strategy_str(strategy)
+    selected = mrmr(input_data, target, top_k, num_cols, s, params, low_memory)
 
-    print(f"Selected {len(selected)} features. There are {len(complement)} features the algorithm "
+    print(f"Selected {len(selected)} features. There are {len(complement)} columns the algorithm "
           "cannot process. They are also returned.")
-    return selected + complement
+    
+    if is_lazy:
+        return df.blueprint.select(selected + complement)
+    return df.select(selected + complement)
 
 def knock_out_mrmr(
     df:pl.DataFrame
     , target:str
     , k:int 
     , num_cols:Optional[list[str]] = None
-    , strategy:MRMR_STRATEGY|str = MRMR_STRATEGY.F_SCORE
+    , strategy:MRMRStrategy = "fscore"
     , corr_threshold:float = 0.7
     , params:Optional[dict[str,Any]] = None
 ) -> list[str]:
     '''
         Essentially the same as vanilla MRMR. Instead of using sum(abs(corr)) to "weigh down" correlated 
         variables, here we use a simpler knock out rule based on absolute correlation.
 
@@ -517,15 +541,15 @@
     
     num_list = []
     if isinstance(num_cols, list):
         num_list.extend(num_cols)
     else:
         num_list.extend(get_numeric_cols(df, exclude=[target]))
 
-    s = MRMR_STRATEGY(strategy) if isinstance(strategy, str) else strategy
+    s = clean_strategy_str(strategy)
     scores = _mrmr_underlying_score(df
                                     , target = target
                                     , num_list = num_list
                                     , strategy = s
                                     , params = {} if params is None else params)
 
     # Set up
@@ -545,34 +569,45 @@
             count += 1
             pbar.update(1)
         if count >= output_size:
             break
 
     pbar.close()
     if count < k:
-        print(f"Found only {count}/{k} number of values because most of them are highly correlated and the knock out rule eliminates most of them.")
+        print(f"Found only {count}/{k} number of values because most of them are highly correlated and the knock out "
+              "rule eliminates most of them.")
 
-    print("Output is sorted in order of selection. (The 1st feature selected is most important, the 2nd the 2nd most important, etc.)")
+    print("Output is sorted in order of selection (relevance).")
     return selected
 
 def knock_out_mrmr_selector(
-    df:pl.DataFrame
+    df:PolarsFrame
     , target:str
     , top_k:int 
-    , strategy:MRMR_STRATEGY|str = MRMR_STRATEGY.F_SCORE
+    , strategy:MRMRStrategy = "fscore"
     , corr_threshold:float = 0.7
     , params:Optional[dict[str,Any]] = None
-) -> list[str]:
+) -> PolarsFrame:
+
+    is_lazy = isinstance(df, pl.LazyFrame)
+    if isinstance(df, pl.LazyFrame):
+        input_data:pl.DataFrame = df.collect()
+    else:
+        input_data:pl.DataFrame = df
 
     num_cols = get_numeric_cols(df, exclude=[target])
     # Non-numerical columns cannot be analyzed by mrmr. So add back in the end.
-    complement = [f for f in df.columns if f not in num_cols and f != target]
-    s = MRMR_STRATEGY(strategy) if isinstance(strategy, str) else strategy
-    selected = knock_out_mrmr(df, target, top_k, num_cols, s, corr_threshold, params)
-    print(f"Selected {len(selected)} features. There are {len(complement)} features the algorithm "
+    complement = [f for f in df.columns if f not in num_cols]
+
+    s = clean_strategy_str(strategy)
+    selected = knock_out_mrmr(input_data, target, top_k, num_cols, s, corr_threshold, params)
+    print(f"Selected {len(selected)} features. There are {len(complement)} columns the algorithm "
         "cannot process. They are also returned.")
-    return selected + complement
+    
+    if is_lazy:
+        return df.blueprint.select(selected + complement)
+    return df.select(selected + complement)
```

### Comparing `dsds-0.0.1/src/dsds/transform.py` & `dsds-0.0.15/src/dsds/transform.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,538 +1,342 @@
 from __future__ import annotations
 
+from .type_alias import (
+    PolarsFrame
+    , ImputationStrategy
+    , ScalingStrategy
+    , PowerTransformStrategy
+    , clean_strategy_str
+    , CPU_COUNT
+)
 from .prescreen import (
     get_bool_cols
     , get_numeric_cols
     , get_string_cols
     , get_unique_count
     , dtype_mapping
 )
-
-from abc import ABC, abstractmethod
-from dataclasses import dataclass
+from .blueprint import( # Need this for Polars extension to work
+    Blueprint
+)
 import logging
-import orjson
 import polars as pl
-import numpy as np 
-from enum import Enum
-from typing import Any, Tuple, Iterable, Optional
+from typing import Optional, Tuple
+from scipy.stats._morestats import (
+    yeojohnson_normmax
+    , boxcox_normmax
+)
+from concurrent.futures import as_completed, ThreadPoolExecutor
+from tqdm import tqdm
 
 # A lot of companies are still using Python < 3.10
 # So I am not using match statements
 # Well, it does say in project description that we need Python 3.10.
 
 logger = logging.getLogger(__name__)
 
-class ImputationStartegy(Enum):
-    CONST = "CONST"
-    MEDIAN = 'MEDIAN'
-    MEAN = "MEAN"
-    MODE = "MODE"
-
-class ScalingStrategy(Enum):
-    NORMALIZE = "NORMALIZE"
-    MIN_MAX = "MIN-MAX"
-    CONST = "CONST"
-
-class EncodingStrategy(Enum):
-    ORDINAL = "ORDINAL"
-    ORDINAL_AUTO = "ORDINAL-AUTO"
-    TARGET = "TARGET"
-    ONE_HOT = "ONE-HOT"
-    BINARY = "BINARY"
-    PERCENTILE = "PERCENTILE"
-
-# It is highly recommended that this should be a dataclass and serializable by orjson.
-class FitRecord(ABC):
-
-    @abstractmethod
-    def materialize(self) -> pl.DataFrame | str:
-        # A pretty way to print or visualize itself, 
-        # or organize self to something more useful than a data structure.
-        pass 
-
-    @abstractmethod
-    def transform(self, df:pl.DataFrame) -> pl.DataFrame:
-        # Transform according to the record.
-        pass
-
-@dataclass
-class ImputationRecord(FitRecord):
-    features:list[str]
-    strategy:ImputationStartegy
-    values:list[float]|np.ndarray
-
-    def __init__(self, features:list[str], strategy:EncodingStrategy|str, values:list[float]|np.ndarray):
-        self.features = features
-        self.strategy = ImputationStartegy(strategy) if isinstance(strategy, str) else strategy
-        self.values = values
-
-    def __iter__(self) -> Iterable:
-        return zip(self.features, [self.strategy]*len(self.features), self.values)
-    
-    def __str__(self) -> str:
-        return orjson.dumps(self, option=orjson.OPT_SERIALIZE_NUMPY).decode()
-    
-    def materialize(self) -> pl.DataFrame:
-        return pl.from_records(list(self), schema=["feature", "imputation_strategy", "value_used"])
-    
-    def transform(self, df:pl.DataFrame) -> pl.DataFrame:
-        return df.with_columns(
-            pl.col(f).fill_null(v) for f, v in zip(self.features, self.values)
-        )
-    
-@dataclass
-class ScalingRecord(FitRecord):
-    features:list[str]
-    strategy:ScalingStrategy
-    values:list[dict[str, float]]
-
-    def __init__(self, features:list[str], strategy:EncodingStrategy|str, values:list[dict[str, float]]):
-        self.features = features
-        self.strategy = ScalingStrategy(strategy) if isinstance(strategy, str) else strategy
-        self.values = values
-
-    def __iter__(self) -> Iterable:
-        return zip(self.features, [self.strategy]*len(self.features), self.values)
-    
-    def __str__(self) -> str:
-        return orjson.dumps(self, option=orjson.OPT_SERIALIZE_NUMPY).decode()
-    
-    def materialize(self) -> pl.DataFrame:
-        vals = (orjson.dumps(v, option=orjson.OPT_SERIALIZE_NUMPY).decode() for v in self.values)
-        presentable =  zip(self.features, [self.strategy]*len(self.features), vals)
-        return pl.from_records(list(presentable), schema=["feature", "scaling_strategy", "scaling_meta_data"])
-    
-    def transform(self, df:pl.DataFrame) -> pl.DataFrame:
-
-        if self.strategy == ScalingStrategy.NORMALIZE:
-            return df.with_columns(
-                (pl.col(f)-pl.lit(v["mean"]))/pl.lit(v["std"]) for f, v in zip(self.features, self.values)
-            )
-        elif self.strategy == ScalingStrategy.MIN_MAX:
-            return df.with_columns(
-                (pl.col(f)-pl.lit(v["min"]))/(pl.lit(v["max"] - v["min"])) for f, v in zip(self.features, self.values)
-            )
-        elif self.strategy == ScalingStrategy.CONST:
-            return df.with_columns(
-                pl.col(f)/v['const'] for f, v in zip(self.features, self.values)
-            )    
-        else:
-            raise ValueError(f"Unknown scaling strategy: {self.strategy}")
-
-@dataclass
-class EncoderRecord(FitRecord):
-    features:list[str]
-    strategy:EncodingStrategy
-    mappings:list[dict]
-
-    ### FOR str encoders, mapping looks like "dict[str, float]", except one-hot. See one-hot for more info.
-    ### For numeric encoder, like percentile encoder, the key of the mapping is of type str despite the fact that
-    ### it is a number. This is because json has to have str as keys. See percentile_encode for more info.
-
-    def __init__(self, features:list[str], strategy:EncodingStrategy|str, mappings:list[dict[Any, Any]]):
-        self.features = features
-        self.strategy = EncodingStrategy(strategy) if isinstance(strategy, str) else strategy
-        self.mappings = mappings
-
-    def __iter__(self) -> Iterable:
-        return zip(self.features, [self.strategy]*len(self.features), self.mappings)
-    
-    def __str__(self) -> str:
-        return orjson.dumps(self, option=orjson.OPT_SERIALIZE_NUMPY|orjson.OPT_NON_STR_KEYS).decode()
-    
-    def materialize(self) -> pl.DataFrame:
-        vals = (orjson.dumps(v, option=orjson.OPT_SERIALIZE_NUMPY|orjson.OPT_NON_STR_KEYS).decode() for v in self.mappings)
-        presentable =  zip(self.features, [self.strategy]*len(self.features), vals)
-        return pl.from_records(list(presentable), schema=["feature", "encoding_strategy", "maps"])
-    
-    ###
-    # NEED TO FIND WAYS TO OPTIMIZE ENCODINGS FOR Numeric values...
-    ###
-
-    @staticmethod
-    def _find_first_index_of_smaller(u:float, order:list[Tuple[float, int]]) -> int:
-        order.sort(key=lambda x: x[1])
-        for v, i in order: # order looks like [(18.21, 1), (22.32, 2), ...]
-            if u <= v:
-                return i
-        # percentile max out at 100. It is possible that in future data, there will be some
-        # that is > existing max. So assign all that to 101
-        return 101 
-
-    def transform(self, df:pl.DataFrame) -> pl.DataFrame:
-        # Special cases first
-        if self.strategy == EncodingStrategy.PERCENTILE:
-            for i,f in enumerate(self.features):
-                # Construct a new series for each column. SLOW SLOW SLOW...
-
-                # If this comes from a blue_print, then we will get a dict with str keys
-                # because JSON KEY IS ALWAYS A STR.
-                # If we are running this after generating this record, the original key is 
-                # numeric. So either way, this works.
-                order = [(float(v), p) for v, p in self.mappings[i].items()] 
-                percentiles = []
-                already_mapped = {}
-                for v in df.get_column(f):
-                    if v is None or np.isnan(v) or np.isneginf(v): # To 0
-                        percentiles.append(0) 
-                    else:
-                        if v in already_mapped:
-                            percentiles.append(already_mapped[v])
-                        else:
-                            percentile = self._find_first_index_of_smaller(v, order)
-                            already_mapped[v] = percentile
-                            percentiles.append(percentile)
-                
-                new_f = pl.Series(f, percentiles).cast(pl.UInt8)
-                df.replace_at_idx(df.find_idx_by_name(f), new_f)
-                
-            return df
-        
-        elif self.strategy == EncodingStrategy.ONE_HOT:
-            one_hot_cols = self.features
-            one_hot_map = self.mappings[0] # One hot mapping only has 1 mapping in the list.
-            key:str = list(one_hot_map.keys())[0]
-            value:str = one_hot_map[key] # must be a string
-            separator = value[value.rfind(key) - 1]
-            return df.to_dummies(columns=one_hot_cols, separator=separator)
-
-        # Normal case 
-        return df.with_columns(
-            pl.col(f).map_dict(d) for f,d in zip(self.features, self.mappings)
-        )
-
-class FitTransform:
-
-    def __init__(self, transformed:pl.DataFrame, mapping: FitRecord):
-        self.transformed = transformed
-        self.mapping = mapping
-        
-    def __iter__(self) -> Iterable[Tuple[pl.DataFrame, FitRecord]]:
-        return iter((self.transformed, self.mapping))
-    
-    def materialize(self) -> pl.DataFrame | str:
-        return self.mapping.materialize()
-
-
-def check_columns_types(df:pl.DataFrame, cols:Optional[list[str]]=None) -> str:
+def check_columns_types(df:PolarsFrame, cols:Optional[list[str]]=None) -> str:
     '''Returns the unique types of given columns in a single string. If multiple types are present
     they are joined by a |. If cols is not given, automatically uses all df's columns.'''
-    types = set()
     if cols is None:
         check_cols:list[str] = df.columns
     else:
         check_cols:list[str] = cols 
 
-    temp = df.select(check_cols)
-    for t in temp.dtypes:
-        types.add(dtype_mapping(t))
-    
-    if len(types) > 0:
-        return "|".join(types)
-    else:
-        return "unknown"
+    types = set(dtype_mapping(t) for t in df.select(check_cols).dtypes)
+    return "|".join(types) if len(types) > 0 else "unknown"
 
 
-def impute(df:pl.DataFrame
+def impute(
+    df:PolarsFrame
     , cols:list[str]
-    , strategy:ImputationStartegy|str = ImputationStartegy.MEDIAN
-    , const:int = 1
-) -> FitTransform:
+    , strategy:ImputationStrategy = 'median'
+    , const:float = 1.
+) -> PolarsFrame:
     '''
         Arguments:
-            df:
-            cols:
-            strategy:
-            const: only uses this value if strategy = ImputationStartegy.CONST
+            df: Either a eager/lazy Polars dataframe
+            cols: cols to impute
+            strategy: one of 'mean', 'avg', 'average', 'median', 'const', 'constant', 'mode', 'most_frequent'. Some are 
+            just alternative names for the same strategy.
+            const: only uses this value if strategy = const
     
     '''
-
-    s = ImputationStartegy(strategy.replace("-","_")) if isinstance(strategy, str) else strategy
+    s = clean_strategy_str(strategy)
     # Given Strategy, define expressions
-    if s == ImputationStartegy.MEDIAN:
-        all_medians = df[cols].median().to_numpy().ravel()
+    if s == "median":
+        all_medians = df.lazy().select(cols).median().collect().row(0)
         exprs = (pl.col(c).fill_null(all_medians[i]) for i,c in enumerate(cols))
-        impute_record = ImputationRecord(cols, strategy, all_medians)
-
-    elif s == ImputationStartegy.MEAN:
-        all_means = df[cols].mean().to_numpy().ravel()
+    elif s in ("mean", "avg", "average"):
+        all_means = df.lazy().select(cols).mean().collect().row(0)
         exprs = (pl.col(c).fill_null(all_means[i]) for i,c in enumerate(cols))
-        impute_record = ImputationRecord(cols, strategy, all_means)
-
-    elif s == ImputationStartegy.CONST:
+    elif s in ("const", "constant"):
         exprs = (pl.col(c).fill_null(const) for c in cols)
-        impute_record = ImputationRecord(cols, strategy, np.full(shape=len(cols), fill_value=const))
-
-    elif s == ImputationStartegy.MODE:
-        all_modes = df.select(pl.col(c).mode() for c in cols).to_numpy().ravel()
+    elif s in ("mode", "most_frequent"):
+        all_modes = df.lazy().select(pl.col(c).mode().first() for c in cols).collect().row(0)
         exprs = (pl.col(c).fill_null(all_modes[i]) for i,c in enumerate(cols))
-        impute_record = ImputationRecord(cols, strategy, all_modes)
-
     else:
-        raise ValueError(f"Unknown imputation strategy: {s}")
+        raise TypeError(f"Unknown imputation strategy: {strategy}")
 
-    transformed = df.with_columns(exprs)
-    return FitTransform(transformed=transformed, mapping=impute_record)
+    # Need to cast to list so that pickle can work with it
+    # This is unfortunate because we will be looping over this list twice... Whatever...
+    if isinstance(df, pl.LazyFrame):
+        return df.blueprint.with_columns(list(exprs)) 
+    return df.with_columns(exprs)
 
-def scale(df:pl.DataFrame
+def scale(
+    df:PolarsFrame
     , cols:list[str]
-    , strategy:ScalingStrategy=ScalingStrategy.NORMALIZE
-    , const:int = 1
-) -> FitTransform:
+    , strategy:ScalingStrategy="normal"
+    , const:float = 1.0
+) -> PolarsFrame:
     
     '''
         Arguments:
             df:
             cols:
             strategy:
             const: only uses this value if strategy = ImputationStartegy.CONST
     
     '''
     types = check_columns_types(df, cols)
     if types != "numeric":
         raise ValueError(f"Scaling can only be used on numeric columns, not {types} types.")
-    
-    s = ScalingStrategy(strategy.replace("-","_")) if isinstance(strategy, str) else strategy
-    if s == ScalingStrategy.NORMALIZE:
-        all_means = df[cols].mean().to_numpy().ravel()
-        all_stds = df[cols].std().to_numpy().ravel()
-        exprs = (((pl.col(c) - pl.lit(all_means[i]))/(pl.lit(all_stds[i])) for i,c in enumerate(cols)))
-        scale_data = [{"mean":m, "std":s} for m,s in zip(all_means, all_stds)]
-        scaling_records = ScalingRecord(cols, strategy, scale_data)
-
-    elif s == ScalingStrategy.MIN_MAX:
-        all_mins = df[cols].min().to_numpy().ravel()
-        all_maxs = df[cols].max().to_numpy().ravel()
-        exprs = ((pl.col(c) - pl.lit(all_mins[i]))/(pl.lit(all_maxs[i] - all_mins[i])) for i,c in enumerate(cols))
-        scale_data = [{"min":m, "max":mm} for m, mm in zip(all_mins, all_maxs)]
-        scaling_records = ScalingRecord(cols, strategy, scale_data)
 
-    elif s == ScalingStrategy.CONST:
+    s = clean_strategy_str(strategy)
+    if s in ("normal", "standard", "normalize"):
+        mean_std = df.select(cols).lazy().select(
+            pl.all().mean().prefix("mean:")
+            , pl.all().std().prefix("std:")
+        ).collect().row(0)
+        exprs = ( (pl.col(c) - mean_std[i])/(mean_std[i + len(cols)]) for i,c in enumerate(cols) )
+    elif s == "min_max":
+        min_max = df.select(cols).lazy().select(
+            pl.all().min().prefix("min:"),
+            pl.all().max().prefix("max:")
+        ).collect().row(0) # All mins come first, then maxs
+        exprs = ( (pl.col(c) - min_max[i])/((min_max[i + len(cols)] - min_max[i])) for i,c in enumerate(cols) )
+    elif s in ("const", "constant"):
         exprs = (pl.col(c)/const for c in cols)
-        scale_data = [{"const":const} for _ in cols]
-        scaling_records = ScalingRecord(cols, strategy, scale_data)
-
     else:
-        raise ValueError(f"Unknown scaling strategy: {strategy}")
+        raise TypeError(f"Unknown scaling strategy: {strategy}")
 
-    transformed = df.with_columns(exprs)
-    return FitTransform(transformed=transformed, mapping=scaling_records)
+    if isinstance(df, pl.LazyFrame):
+        return df.blueprint.with_columns(list(exprs))
+    return df.with_columns(exprs)
 
-def boolean_transform(df:pl.DataFrame, keep_null:bool=True) -> pl.DataFrame:
+def boolean_transform(df:PolarsFrame, keep_null:bool=True) -> PolarsFrame:
     '''
         Converts all boolean columns into binary columns.
         Arguments:
             df:
             keep_null: if true, null will be kept. If false, null will be mapped to 0.
 
     '''
     bool_cols = get_bool_cols(df)
     if keep_null: # Directly cast. If null, then cast will also return null
         exprs = (pl.col(c).cast(pl.UInt8) for c in bool_cols)
     else: # Cast. Then fill null to 0s.
         exprs = (pl.col(c).cast(pl.UInt8).fill_null(0) for c in bool_cols)
 
+    if isinstance(df, pl.LazyFrame):
+        return df.blueprint.with_columns(list(exprs))
     return df.with_columns(exprs)
 
-def one_hot_encode(df:pl.DataFrame, cols:Optional[list[str]]=None, separator:str="_") -> FitTransform:
+def one_hot_encode(
+    df:PolarsFrame
+    , cols:Optional[list[str]]=None
+    , separator:str="_"
+    , drop_first:bool=False
+) -> PolarsFrame:
     '''One hot encoding. The separator must be a single character.'''
-
-    # Here is a rule: Separator must be a single char
-    # This is enforced because we want to be able to extract separator from EncoderRecord
-    if len(separator) != 1:
-        raise ValueError(f"Separator must be a single character for the system to work, not {separator}")
     
-    str_cols = []
     if isinstance(cols, list):
         types = check_columns_types(df, cols)
         if types != "string":
             raise ValueError(f"One-hot encoding can only be used on string columns, not {types} types.")
-        str_cols.extend(cols)
+        str_cols = cols
     else:
         str_cols = get_string_cols(df)
 
-    res = df.to_dummies(columns=str_cols, separator=separator)
-    all_mappings = []
-    for c in str_cols:
-        mapping = {}
-        for cc in filter(lambda name: c in name, res.columns):
-            # c is original column_name, cc is one-hot created name
-            val = cc.replace(c + separator, "") # get original value
-            mapping[val] = cc
-
-        all_mappings.append(mapping)
-
-    encoder_rec = EncoderRecord(features=str_cols, strategy=EncodingStrategy.ONE_HOT, mappings=all_mappings)
-    return FitTransform(transformed = res, mapping = encoder_rec)
+    if isinstance(df, pl.LazyFrame):
+        temp = df.lazy().groupby(1).agg(
+            pl.col(s).unique().sort() for s in str_cols
+        ).select(str_cols)
+        exprs:list[pl.Expr] = []
+        one = pl.lit(1, dtype=pl.UInt8) # Avoid casting 
+        zero = pl.lit(0, dtype=pl.UInt8) # Avoid casting
+        for t in temp.collect().get_columns():
+            u:pl.List = t[0] # t is a Series which contains a single series/list, so u is a series/list
+            if len(u) > 1:
+                exprs.extend(
+                    pl.when(pl.col(t.name) == u[i]).then(one).otherwise(zero).alias(t.name + separator + u[i])
+                    for i in range(int(drop_first), len(u)) 
+                )
+            else:
+                logger.info(f"During one-hot-encoding, the column {t.name} is found to have 1 unique value. Dropped.")
+        
+        return df.blueprint.with_columns(exprs).blueprint.drop(str_cols)
+    else:
+        return df.to_dummies(columns=str_cols, separator=separator, drop_first=drop_first)
 
 # def fixed_sized_encode(df:pl.DataFrame, num_cols:list[str], bin_size:int=50) -> TransformationResult:
 #     '''Given a continuous variable, take the smallest `bin_size` of them, and call them bin 1, take the next
 #     smallest `bin_size` of them and call them bin 2, etc...
     
 #     '''
 #     pass
 
-# Try to generalize this.
-def percentile_encode(df:pl.DataFrame
-    , cols:list[str]=None
-    , exclude:list[str]=None
-) -> FitTransform:
-    '''
-        Bin your continuous variable X into X_percentiles. This will create at most 100 + 1 bins, where each percentile could
-        potentially be a bin and null will be mapped to bin = 0. Bin 1 means percentile 0 to 1. Generally, bin X groups the
-        population from bin X-1 to bin X into one bucket.
 
-        I see some potential optimization opportunities here.
+# REWRITE THIS
+# def percentile_encode(df:pl.DataFrame
+#     , cols:list[str]=None
+#     , exclude:list[str]=None
+# ) -> FitTransform:
+#     '''Bin your continuous variable X into X_percentiles. This will create at most 100 + 1 bins, 
+#         where each percentile could potentially be a bin and null will be mapped to bin = 0. 
+#         Bin 1 means percentile 0 to 1. Generally, bin X groups the population from bin X-1 to 
+#         bin X into one bucket.
+
+#         I see some potential optimization opportunities here.
+
+#         Arguments:
+#             df:
+#             num_cols: 
+#             exclude:
 
-        Arguments:
-            df:
-            num_cols: 
-            exclude:
-
-        Returns:
-            (A transformed dataframe, a mapping table (value to percentile))
+#         Returns:
+#             (A transformed dataframe, a mapping table (value to percentile))
     
-    '''
-
-    # Percentile Binning
+#     '''
 
-    num_list:list[str] = []
-    exclude_list:list[str] = [] if exclude is None else exclude
-    if isinstance(cols, list):
-        types = check_columns_types(df, cols)
-        if types != "numeric":
-            raise ValueError(f"Percentile encoding can only be used on numeric columns, not {types} types.")
-        num_list.extend(cols)
-    else:
-        num_list.extend(get_numeric_cols(df, exclude=exclude_list))
+#     # Percentile Binning
 
-    exprs:list[pl.Expr] = []
-    all_mappings = []
-    for c in num_list:
-        percentile = df.groupby(c).agg(pl.count().alias("cnt"))\
-            .sort(c)\
-            .with_columns(
-                ((pl.col("cnt").cumsum()*100)/len(df)).ceil().alias("percentile")
-            ).groupby("percentile")\
-            .agg((
-                pl.col(c).min().alias("min"),
-                pl.col(c).max().alias("max"),
-                pl.col("cnt").sum().alias("cnt"),
-            )).sort("percentile").select((
-                pl.lit(c).alias("feature"),
-                pl.col("percentile").cast(pl.UInt8),
-                "min",
-                "max",
-                "cnt",
-            ))
+#     num_list:list[str] = []
+#     exclude_list:list[str] = [] if exclude is None else exclude
+#     if isinstance(cols, list):
+#         types = check_columns_types(df, cols)
+#         if types != "numeric":
+#             raise ValueError(f"Percentile encoding can only be used on numeric columns, not {types} types.")
+#         num_list.extend(cols)
+#     else:
+#         num_list.extend(get_numeric_cols(df, exclude=exclude_list))
+
+#     exprs:list[pl.Expr] = []
+#     all_mappings = []
+#     for c in num_list:
+#         percentile = df.groupby(c).agg(pl.count().alias("cnt"))\
+#             .sort(c)\
+#             .with_columns(
+#                 ((pl.col("cnt").cumsum()*100)/len(df)).ceil().alias("percentile")
+#             ).groupby("percentile")\
+#             .agg(
+#                 pl.col(c).min().alias("min"),
+#                 pl.col(c).max().alias("max"),
+#                 pl.col("cnt").sum().alias("cnt"),
+#             ).sort("percentile").select(
+#                 pl.lit(c).alias("feature"),
+#                 pl.col("percentile").cast(pl.UInt8),
+#                 "min",
+#                 "max",
+#                 "cnt",
+#             )
         
-        first_row = percentile.select(["percentile","min", "max"]).to_numpy()[0, :] # First row
-        # Need to handle an extreme case when percentile looks like 
-        # percentile   min   max
-        #  p1         null  null
-        #  p2          ...   ...
-        # This happens when there are so many nulls in the column.
-        if np.isnan(first_row[2]):
-            # Discard the first row if this is the case. 
-            percentile = percentile.slice(1, length = None)
-
-        temp_df = df.lazy().filter(pl.col(c).is_not_null()).sort(c).set_sorted(c)\
-            .join_asof(other=percentile.lazy().set_sorted("max"), left_on=c, right_on="max", strategy="forward")\
-            .select((c, "percentile"))\
-            .unique().collect()
+#         first_row = percentile.select("percentile","min", "max").to_numpy()[0, :] # First row
+#         # Need to handle an extreme case when percentile looks like 
+#         # percentile   min   max
+#         #  p1         null  null
+#         #  p2          ...   ...
+#         # This happens when there are so many nulls in the column.
+#         if np.isnan(first_row[2]):
+#             # Discard the first row if this is the case. 
+#             percentile = percentile.slice(1, length = None)
+
+#         # Only work on non null values. Null will be mapped to default value anyway.
+#         temp_df = df.lazy().filter(pl.col(c).is_not_null()).sort(c).set_sorted(c)\
+#             .join_asof(other=percentile.lazy().set_sorted("max"), left_on=c, right_on="max", strategy="forward")\
+#             .select(c, "percentile")\
+#             .unique().collect()
         
-        real_mapping = dict(zip(temp_df[c], temp_df["percentile"]))
-        # a representation of the mapping.
-        repr_mapping = dict(zip(percentile["max"], percentile["percentile"]))
-        all_mappings.append(repr_mapping)
-        exprs.append(
-            pl.col(c).map_dict(real_mapping, default=0).cast(pl.UInt8)
-        )
-        percentile = percentile.with_columns((
-            pl.col("min").cast(pl.Float32),
-            pl.col("max").cast(pl.Float32),
-            pl.col("cnt").cast(pl.UInt32)
-        )) # Need to do this because we need a uniform format in order to stack these columns.
-
-    res = df.with_columns(exprs)
-    encoder_rec = EncoderRecord(features=num_list, strategy=EncodingStrategy.PERCENTILE, mappings=all_mappings)
-    return FitTransform(transformed=res, mapping=encoder_rec)
+#         real_mapping = dict(zip(temp_df[c], temp_df["percentile"]))
+#         # a representation of the mapping, needed for recreating this.
+#         repr_mapping = dict(zip(percentile["max"], percentile["percentile"]))
+#         all_mappings.append(repr_mapping)
+#         exprs.append(
+#             pl.col(c).map_dict(real_mapping, default=0).cast(pl.UInt8)
+#         )
+
+#     res = df.with_columns(exprs)
+#     encoder_rec = EncoderRecord(features=num_list, strategy=EncodingStrategy.PERCENTILE, mappings=all_mappings)
+#     return FitTransform(transformed=res, mapping=encoder_rec)
 
-def binary_encode(df:pl.DataFrame
+def binary_encode(
+    df:PolarsFrame
     , cols:Optional[list[str]]=None
     , exclude:Optional[list[str]]=None
-) -> FitTransform:
-    
-    '''Encode the given columns as binary values.
-
-        The goal of this function is to map binary string values into [0, 1], therefore reducing the amount of encoding
-        you will have to do later. The values will be mapped to [0, 1] by the following rule:
-            if value_1 < value_2, value_1 --> 0, value_2 --> 1. E.g. 'N' < 'Y' ==> 'N' --> 0 and 'Y' --> 1
-        
-        In case the two distinct values are [None, value_1], and you decide to treat this variable as a binary category
-        , then None --> 0 and value_1 --> 1. 
-        
-        Using one-hot-encoding will map binary categorical values to 2 columns (except when you specify drop_first=True 
-        in pd.get_dummies), therefore introducing unnecessary dimension. So it is better to prevent it.
-
-        If case the distinct values are [null, value_1, value_2], then this is not currently considered as a 
-        binary column.
+) -> PolarsFrame:
+    '''Encode the given columns as binary values. Only hands string binaries at this moment. Just a short-hand for 
+        one-hot-encoding for binary string columns.
 
         Arguments:
             df:
             binary_cols: the binary_cols you wish to convert. If no input, will infer.
             exclude: the columns you wish to exclude in this transformation. 
 
         Returns: 
             (the transformed dataframe, mapping table between old values to [0,1])
     '''
 
-    exprs = []
-    mappings = []
-    binary_list = []
-    if isinstance(cols, list):
-        binary_list.extend(cols)
-    else:
+    if cols is None:
         str_cols = get_string_cols(df)
         exclude = [] if exclude is None else exclude
-        binary_columns = get_unique_count(df)\
-            .filter( # Binary + Not Exclude + String
+        binary_list = get_unique_count(df)\
+            .filter( # Binary + Not Exclude + Only String
                 (pl.col("n_unique") == 2) & (~pl.col("column").is_in(exclude)) & (pl.col("column").is_in(str_cols))
-            ).get_column("column")
+            ).get_column("column").to_list()
 
-        # Binary numericals are kept the way they are.
-        binary_list.extend(binary_columns)     
+    else: # No need to do all that type checking steps because we are gonna do that in one-hot anyways
+        binary_list = cols
     
-    # Doing some repetitive operations here, but I am not sure how I can get all the data in one go.
-    for b in binary_list:
-        vals = df.get_column(b).unique().to_list()
-        logger.info(f"Transforming {b} into a binary column with [0, 1] ...")
-        if len(vals) != 2:
-            logger.warning(f"Found {b} has {len(vals)} unique values instead of 2. Not a binary variable. Ignored.")
-            continue
-        if vals[0] is None: # Weird code, but we need this case.
-            pass
-        elif vals[1] is None:
-            vals[0], vals[1] = vals[1], vals[0]
-        else:
-            vals.sort()
+    return one_hot_encode(df, cols=binary_list, drop_first=True)
 
-        # In Python, None can be a dictionary key.
-        mappings.append({vals[0]: 0, vals[1]: 1})
-        exprs.append(
-            pl.when(pl.col(b).is_null()).then(0).otherwise(
-                pl.when(pl.col(b) < vals[1]).then(0).otherwise(1)
-            ).cast(pl.UInt8).alias(b) 
-        )
-
-    res = df.with_columns(exprs)
-    encoder_rec = EncoderRecord(features=binary_list, strategy=EncodingStrategy.BINARY, mappings=mappings)
-    return FitTransform(transformed = res, mapping = encoder_rec)
+def force_binary(
+    df:PolarsFrame
+    , cols:Optional[list[str]]=None
+):
+    '''
+    Force every binary column, no matter what data type, to be turned into 0s and 1s by the order of the elements. If a 
+    column has two unique values like [null, "haha"], then null will be mapped to 0 and "haha" to 1.
+    '''
+    if cols is None:
+        binary_list = get_unique_count(df)\
+            .filter(pl.col("n_unique") == 2)\
+            .get_column("column").to_list()
+    else:
+        binary_list = cols
+
+    temp = df.lazy().groupby(1).agg(
+            pl.col(s).unique().sort() for s in binary_list
+        ).select(binary_list)
+    
+    exprs:list[pl.Expr] = []
+    one = pl.lit(1, dtype=pl.UInt8) # Avoid casting 
+    zero = pl.lit(0, dtype=pl.UInt8) # Avoid casting
+    for t in temp.collect().get_columns():
+        u:pl.List = t[0] # t is a Series which contains a single list which contains the 2 unique values 
+        if len(u) == 2:
+            exprs.append(
+                pl.when(pl.col(t.name) == u[0]).then(zero).otherwise(one).alias(t.name)
+            )
+        else:
+            logger.info(f"During force_binary, the column {t.name} is found to have != 2 unique values. Ignored.")
+    
+    if isinstance(df, pl.LazyFrame):
+        return df.blueprint.with_columns(exprs)
+    return df.with_columns(exprs)    
 
 def get_mapping_table(ordinal_mapping:dict[str, dict[str,int]]) -> pl.DataFrame:
     '''
         Helper function to get a table from an ordinal_mapping dict.
 
         >>> {
         >>> "a": 
@@ -549,65 +353,70 @@
             A table with feature name, value, and mapped_to
     
     '''
     mapping_tables:list[pl.DataFrame] = []
     for feature, mapping in ordinal_mapping.items():
         table = pl.from_records(list(mapping.items()), schema=["value", "mapped_to"]).with_columns(
             pl.lit(feature).alias("feature")
-        ).select(("feature", "value", "mapped_to"))
+        ).select("feature", "value", "mapped_to")
         mapping_tables.append(table)
 
     return pl.concat(mapping_tables)
 
-def ordinal_auto_encode(df:pl.DataFrame
-    , cols:list[str]=None
-    , default:int|None=None
+def ordinal_auto_encode(
+    df:PolarsFrame
+    , cols:Optional[list[str]]=None
     , exclude:Optional[list[str]]=None
-) -> FitTransform:
+) -> PolarsFrame:
     '''
         Automatically applies ordinal encoding to the provided columns by the following logic:
             Sort the column, smallest value will be assigned to 0, second smallest will be assigned to 1...
 
         This will automatically detect string columns and apply this operation if ordinal_cols is not provided. 
         This method is great for string columns like age ranges, with values like ["10-20", "20-30"], etc...
         
         Arguments:
             df:
             default:
             ordinal_cols:
-            exclude: the columns you wish to exclude in this transformation. (Only applies if you are letting the system auto-detecting columns.)
+            exclude: the columns you wish to exclude in this transformation.
         
         Returns:
             (encoded df, mapping table)
     '''
-    ordinal_list:list[str] = []
     if isinstance(cols, list):
         types = check_columns_types(df, cols)
         if types != "string":
             raise ValueError(f"Ordinal encoding can only be used on string columns, not {types} types.")
-        ordinal_list.extend(cols)
+        ordinal_list = cols
     else:
-        ordinal_list.extend(get_string_cols(df, exclude=exclude))
+        ordinal_list = get_string_cols(df, exclude=exclude)
 
-    exprs:list[pl.Expr] = []
-    all_mappings = []
-    for c in ordinal_list:
-        sorted_uniques = df.get_column(c).unique().sort()
-        mapping:dict[str, int] = dict(zip(sorted_uniques, range(len(sorted_uniques))))
-        all_mappings.append(mapping)
-        exprs.append(pl.col(c).map_dict(mapping, default=default).cast(pl.UInt32))
-
-    res = df.with_columns(exprs)
-    encoder_rec = EncoderRecord(features=ordinal_list, strategy=EncodingStrategy.ORDINAL_AUTO, mappings=all_mappings)
-    return FitTransform(transformed=res, mapping=encoder_rec)
+    temp = df.lazy().groupby(1).agg(
+        pl.col(c).unique().sort() for c in ordinal_list
+    ).select(ordinal_list)
+    for t in temp.collect().get_columns():
+        uniques:pl.Series = t[0]
+        mapping = {t.name: uniques, "to": list(range(len(uniques)))} 
+        if isinstance(df, pl.LazyFrame):
+            # Use a list here because Python cannot pickle a generator
+            df = df.blueprint.map_dict(t.name, mapping, "to", None)
+        else:
+            map_tb = pl.DataFrame(mapping)
+            df = df.join(map_tb, on = t.name).with_columns(
+                pl.col("to").alias(t.name)
+            ).drop("to")
+
+    return df
 
-def ordinal_encode(df:pl.DataFrame
+def ordinal_encode(
+    df:PolarsFrame
     , ordinal_mapping:dict[str, dict[str,int]]
     , default:int|None=None
-) -> FitTransform:
+) -> PolarsFrame:
     '''
         Ordinal encode the data with given mapping.
 
         Notice that this function assumes that you already have the mapping, in correct mapping format.
         since you have to supply the ordinal_mapping argument. If you still want the tabular output format,
         please call get_ordinal_mapping_table with ordinal_mapping, which will create a table from this.
 
@@ -615,81 +424,167 @@
             df:
             ordinal_mapping:
             default: if a value for a feature does not exist in ordinal_mapping, use default.
 
         Returns:
             encoded df
     '''
-    
-    exprs:list[pl.Expr] = []
-    f:list[str] = []
-    all_mappings:list[dict[Any, Any]] = []
+
     for c in ordinal_mapping:
         if c in df.columns:
             mapping = ordinal_mapping[c]
-            all_mappings.append(mapping)
-            exprs.append(pl.col(c).map_dict(mapping, default=default).cast(pl.UInt32))
+            if isinstance(df, pl.LazyFrame):
+                # This relies on the fact that dicts in Python is ordered
+                mapping = {c: mapping.keys(), "to": mapping.values()}
+                df = df.blueprint.map_dict(c, mapping, "to", default)
+            else:
+                mapping = pl.DataFrame((mapping.keys(), mapping.values()), schema=[c, "to"])
+                df = df.join(mapping, on = c, how="left").with_columns(
+                    pl.col("to").fill_null(default).alias(c)
+                ).drop("to")
         else:
             logger.warning(f"Found that column {c} is not in df. Skipped.")
 
-    res = df.with_columns(exprs)
-    encoder_rec = EncoderRecord(features=f, strategy=EncodingStrategy.ORDINAL, mappings=all_mappings)
-    return FitTransform(transformed=res, mapping=encoder_rec)
+    return df
 
 def smooth_target_encode(
-    df:pl.DataFrame
+    df:PolarsFrame
     , target:str
     , cols:list[str]
     , min_samples_leaf:int
     , smoothing:float
     , check_binary:bool=True
-) -> FitTransform:
+) -> PolarsFrame:
     '''Smooth target encoding for binary classification. Currently only implemented for binary target.
 
         See https://towardsdatascience.com/dealing-with-categorical-variables-by-using-target-encoder-a0f1733a4c69
 
         Arguments:
             df:
             target:
             cat_cols:
             min_samples_leaf:
             smoothing:
             check_binary:
-    
     '''
-    str_cols:list[str] = []
     if isinstance(cols, list):
         types = check_columns_types(df, cols)
         if types != "string":
             raise ValueError(f"Target encoding can only be used on string columns, not {types} types.")
-        str_cols.extend(cols)
+        str_cols = cols
     else:
         str_cols = get_string_cols(df)
     
     # Only works for binary target for now 
     # Check if it is binary or not.
     if check_binary:
-        target_uniques = df.get_column(target).unique()
+        target_uniques = df.lazy().select(pl.col(target).unique()).collect().get_column(target)
         if len(target_uniques) != 2 or (not (0 in target_uniques and 1 in target_uniques)):
             raise ValueError(f"The target column {target} must be a binary target with 0s and 1s.")
 
-    p = df.get_column(target).mean() # probability of target = 1
-    all_mappings:list[dict[Any, Any]] = []
-    exprs:list[pl.Expr] = []
+    p = df.lazy().select(pl.col(target).mean()).collect().row(0)[0] # probability of target = 1
     # If c has null, null will become a group when we group by.
     for c in str_cols:
         ref = df.groupby(c).agg(
-            pl.col(target).sum().alias("cnt"),
+            pl.count().alias("cnt"),
             pl.col(target).mean().alias("cond_p")
         ).with_columns(
-            (1/(1 + ((-(pl.col("cnt") - pl.lit(min_samples_leaf)))/pl.lit(smoothing)).exp())).alias("alpha")
-        ).with_columns(
+            (1./(1. + ((-(pl.col("cnt").cast(pl.Float64) - min_samples_leaf))/smoothing).exp())).alias("alpha")
+        ).select(
+            pl.col(c).alias(c),
             (pl.col("alpha") * pl.col("cond_p") + (pl.lit(1) - pl.col("alpha")) * pl.lit(p)).alias("encoded_as")
-        )
-        
-        mapping = dict(zip(ref[c], ref["encoded_as"]))
-        all_mappings.append(mapping)
-        exprs.append(pl.col(c).map_dict(mapping))
+        ) # If df is lazy, ref is lazy. If df is eager, ref is eager
+        if isinstance(df, pl.LazyFrame):
+            df = df.blueprint.map_dict(c, ref.collect().to_dict(), "encoded_as", None)
+        else: # It is ok to do inner join because all values of c are present in ref.
+            df = df.join(ref, on = c).with_columns(
+                pl.col("encoded_as").alias(c)
+            ).drop("encoded_as")
+
+    return df
+
+def _lmax_estimate_step(df:PolarsFrame, c:str, s:PowerTransformStrategy) -> Tuple[str, float]:
+    np_col = df.lazy().select(pl.col(c).cast(pl.Float64)).collect().get_column(c).view()
+    if s in ("yeo_johnson", "yeojohnson"):
+        lmax:float = yeojohnson_normmax(np_col)
+    else:
+        lmax:float = boxcox_normmax(np_col, method="mle")
+    
+    return (c, lmax)
+
+def power_transform(
+    df: PolarsFrame
+    , cols: list[str]
+    , strategy: PowerTransformStrategy = "yeo_johnson"
+    , n_threads:int = CPU_COUNT
+    # , lmbda: Optional[float] = None
+) -> PolarsFrame:
+    '''Performs power transform on the data.
+
+    df: either a lazy or eager Polars dataframe
+    cols: a list of numerical columns to perform the transform.
+    strategy: either yeo_johnson or box_cox
+    n_threads: max number of threads you want to use. Default = CPU_COUNT
+
+    returns:
+        the transformed dataframe. If input is lazy, output is lazy. If input is eager, output is eager.
+    
+    '''
+    
+
+    types = check_columns_types(df, cols)
+    if types != "numeric":
+        raise ValueError(f"Power Transform can only be used on numeric columns, not {types} types.")
+
+    s = clean_strategy_str(strategy)
+    exprs:list[pl.Expr] = []
+    # Ensure columns do not have missing values
+    exclude_columns_w_nulls = df.lazy().select(cols).null_count().collect().transpose(
+        include_header=True, column_names=["null_count"]
+    ).filter(pl.col("null_count") > 0).get_column("column").to_list()
+
+    if len(exclude_columns_w_nulls) > 0:
+        logger.info("The following columns will not be processed by power_transform because they contain missing "
+                    f"values. Please impute them.\n{exclude_columns_w_nulls}")
         
-    res = df.with_columns(exprs)
-    encoder_rec = EncoderRecord(features=str_cols, strategy=EncodingStrategy.TARGET, mappings=all_mappings)
-    return FitTransform(transformed=res, mapping=encoder_rec)
+    non_null_list = [c for c in cols if c not in exclude_columns_w_nulls]
+    pbar = tqdm(non_null_list, desc = "Inferring best paramters")
+    if s in ("yeo_johnson", "yeojohnson"):
+        with ThreadPoolExecutor(max_workers=n_threads) as ex:
+            for future in as_completed(ex.submit(_lmax_estimate_step, df, c, s) for c in non_null_list):
+                c, lmax = future.result()
+                if lmax == 0: # log(x + 1)
+                    x_ge_0_sub_expr = (pl.col(c).add(1)).log()
+                else: # ((x + 1)**lmbda - 1) / lmbda
+                    x_ge_0_sub_expr = ((pl.col(c).add(1)).pow(lmax) - 1) / lmax
+
+                if lmax == 2: # -log(-x + 1)
+                    x_lt_0_sub_expr = pl.lit(-1) * (1 - pl.col(c)).log()
+                else: #  -((-x + 1)**(2 - lmbda) - 1) / (2 - lmbda)
+                    t = 2 - lmax
+                    x_lt_0_sub_expr = pl.lit(-1/t) * ((1 - pl.col(c)).pow(t) - 1)
+
+                exprs.append(
+                    pl.when(pl.col(c).ge(0)).then(x_ge_0_sub_expr).otherwise(x_lt_0_sub_expr).alias(c)
+                )
+                pbar.update(1)
+
+    elif s in ("box_cox", "boxcox"):
+        with ThreadPoolExecutor(max_workers=n_threads) as ex:
+            for future in as_completed(ex.submit(_lmax_estimate_step, df, c, s) for c in non_null_list):
+                c, lmax = future.result()
+                if lmax == 0: # log(x)
+                    exprs.append(pl.col(c).log())
+                else: # (x**lmbda - 1) / lmbda
+                    exprs.append(
+                        (pl.col(c).pow(lmax) - 1) / lmax
+                    )
+                pbar.update(1)
+    else:
+        raise TypeError(f"The input strategy {strategy} is not a valid strategy. Valid strategies are: yeo_johnson "
+                        "or box_cox")
+    pbar.close()
+    if isinstance(df, pl.LazyFrame): # Lazy
+        return df.lazy().blueprint.with_columns(exprs)
+    return df.with_columns(exprs) # Eager
+
+
```

### Comparing `dsds-0.0.1/src/dsds/utils.py` & `dsds-0.0.15/src/dsds/utils.py`

 * *Files identical despite different names*

