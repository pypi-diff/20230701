# Comparing `tmp/keras_pbar-0.0.1.tar.gz` & `tmp/keras_pbar-0.0.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras_pbar-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "keras_pbar-0.0.1.dev1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `keras_pbar-0.0.1.tar` & `keras_pbar-0.0.1.dev1.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0      678 2023-06-04 17:59:30.949708 keras_pbar-0.0.1/Readme.md
--rw-r--r--   0        0        0       45 2023-06-04 17:59:30.949708 keras_pbar-0.0.1/keras_pbar/__init__.py
--rw-r--r--   0        0        0     1117 2023-06-04 17:59:30.949708 keras_pbar-0.0.1/keras_pbar/keras_pbar.py
--rw-r--r--   0        0        0      727 2023-06-04 17:59:30.949708 keras_pbar-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 keras_pbar-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      502 2023-06-30 22:14:48.630884 keras_pbar-0.0.1.dev1/Readme.md
+-rw-r--r--   0        0        0       49 2023-06-30 22:14:48.630884 keras_pbar-0.0.1.dev1/keras_pbar/__init__.py
+-rw-r--r--   0        0        0       64 2023-06-30 22:14:48.630884 keras_pbar-0.0.1.dev1/keras_pbar/py.typed
+-rw-r--r--   0        0        0        0 2023-06-30 22:14:48.630884 keras_pbar-0.0.1.dev1/keras_pbar/src/__init__.py
+-rw-r--r--   0        0        0     1125 2023-06-30 22:14:48.630884 keras_pbar-0.0.1.dev1/keras_pbar/src/keras_pbar.py
+-rw-r--r--   0        0        0     8954 2023-06-30 22:14:48.630884 keras_pbar-0.0.1.dev1/keras_pbar/src/pbar.py
+-rw-r--r--   0        0        0      653 2023-06-30 22:14:48.630884 keras_pbar-0.0.1.dev1/pyproject.toml
+-rw-r--r--   0        0        0     1070 1970-01-01 00:00:00.000000 keras_pbar-0.0.1.dev1/PKG-INFO
```

### Comparing `keras_pbar-0.0.1/keras_pbar/keras_pbar.py` & `keras_pbar-0.0.1.dev1/keras_pbar/src/keras_pbar.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from typing import Sized, Iterable, TypeVar
-from keras.utils import Progbar
+from keras_pbar.src.pbar import Progbar
 
 T = TypeVar("T")
 
 
 def keras_pbar(iterable: Iterable[T], n: int | None = None) -> Iterable[T]:
     """
     Prints Keras progress bar to stdout and updates it on every iteration.
```

### Comparing `keras_pbar-0.0.1/PKG-INFO` & `keras_pbar-0.0.1.dev1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: keras_pbar
-Version: 0.0.1
+Version: 0.0.1.dev1
 Summary: TQDM-like API for Keras Progressbar.
 Author-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Maintainer-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
-Requires-Dist: keras
-Requires-Dist: tensorflow ; extra == "dev" and ( sys_platform == 'linux')
-Requires-Dist: tensorflow_macos ; extra == "dev" and ( sys_platform == 'darwin')
+Requires-Dist: numpy
+Requires-Dist: absl_py
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: tox ; extra == "dev"
 Project-URL: Homepage, https://github.com/aaarrti/keras_pbar
 Provides-Extra: dev
 
 # Keras Progressbar with TQDM-like API.
@@ -29,11 +28,8 @@
 from keras_pbar import keras_pbar
 
 df = pd.read_csv("data.csv")
 for identifier, sliced in keras_pbar(df.group_by("id")):
     # Do some time consuming processing.
     time.sleep(2)
 ```
-### Notes
-It does not directly depend on `tensorflow`, so you can install it without.
-But probably during import time, it will fail, when `keras` tries to import `tensorlfow`.
```

