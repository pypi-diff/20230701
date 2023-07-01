# Comparing `tmp/mltrainer-0.1.4.tar.gz` & `tmp/mltrainer-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mltrainer-0.1.4.tar", last modified: Fri Jun 30 10:32:19 2023, max compression
+gzip compressed data, was "mltrainer-0.1.5.tar", last modified: Sat Jul  1 19:39:33 2023, max compression
```

## Comparing `mltrainer-0.1.4.tar` & `mltrainer-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       50 2023-06-30 09:29:35.989842 mltrainer-0.1.4/README.md
--rw-r--r--   0        0        0      177 2023-06-30 10:32:00.627743 mltrainer-0.1.4/mltrainer/__init__.py
--rw-r--r--   0        0        0     1653 2023-06-29 21:12:27.729107 mltrainer-0.1.4/mltrainer/imagemodels.py
--rw-r--r--   0        0        0     1653 2023-06-29 21:14:56.380151 mltrainer-0.1.4/mltrainer/metrics.py
--rw-r--r--   0        0        0     4285 2023-06-29 21:14:36.526642 mltrainer-0.1.4/mltrainer/rnn_models.py
--rw-r--r--   0        0        0     1543 2023-06-29 21:25:52.147263 mltrainer-0.1.4/mltrainer/settings.py
--rw-r--r--   0        0        0     2388 2023-06-29 21:22:50.605098 mltrainer-0.1.4/mltrainer/tokenizer.py
--rw-r--r--   0        0        0     8797 2023-06-30 09:47:07.147102 mltrainer-0.1.4/mltrainer/trainer.py
--rw-r--r--   0        0        0     2489 2023-06-30 09:47:13.271722 mltrainer-0.1.4/mltrainer/vae.py
--rw-r--r--   0        0        0     1643 2023-06-30 10:32:19.126916 mltrainer-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 mltrainer-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       50 2023-06-30 09:29:35.989842 mltrainer-0.1.5/README.md
+-rw-r--r--   0        0        0      177 2023-07-01 19:38:48.061403 mltrainer-0.1.5/mltrainer/__init__.py
+-rw-r--r--   0        0        0     1653 2023-06-29 21:12:27.729107 mltrainer-0.1.5/mltrainer/imagemodels.py
+-rw-r--r--   0        0        0     1653 2023-06-29 21:14:56.380151 mltrainer-0.1.5/mltrainer/metrics.py
+-rw-r--r--   0        0        0     4285 2023-06-29 21:14:36.526642 mltrainer-0.1.5/mltrainer/rnn_models.py
+-rw-r--r--   0        0        0     1543 2023-06-29 21:25:52.147263 mltrainer-0.1.5/mltrainer/settings.py
+-rw-r--r--   0        0        0     2388 2023-06-29 21:22:50.605098 mltrainer-0.1.5/mltrainer/tokenizer.py
+-rw-r--r--   0        0        0     8797 2023-06-30 09:47:07.147102 mltrainer-0.1.5/mltrainer/trainer.py
+-rw-r--r--   0        0        0     2489 2023-06-30 09:47:13.271722 mltrainer-0.1.5/mltrainer/vae.py
+-rw-r--r--   0        0        0     1643 2023-07-01 19:39:33.290727 mltrainer-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      916 1970-01-01 00:00:00.000000 mltrainer-0.1.5/PKG-INFO
```

### Comparing `mltrainer-0.1.4/mltrainer/imagemodels.py` & `mltrainer-0.1.5/mltrainer/imagemodels.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.4/mltrainer/metrics.py` & `mltrainer-0.1.5/mltrainer/metrics.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.4/mltrainer/rnn_models.py` & `mltrainer-0.1.5/mltrainer/rnn_models.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.4/mltrainer/settings.py` & `mltrainer-0.1.5/mltrainer/settings.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.4/mltrainer/tokenizer.py` & `mltrainer-0.1.5/mltrainer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.4/mltrainer/trainer.py` & `mltrainer-0.1.5/mltrainer/trainer.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.4/mltrainer/vae.py` & `mltrainer-0.1.5/mltrainer/vae.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.4/pyproject.toml` & `mltrainer-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 [project]
 name = "mltrainer"
-version = "0.1.4"
+version = "0.1.5"
 description = "toolkit for training pytorch models"
 authors = [
     { name = "R.Grouls", email = "Raoul.Grouls@han.nl" },
 ]
 requires-python = ">=3.10"
 readme = "README.md"
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Topic :: Scientific/Engineering :: Artificial Intelligence",
+    "Programming Language :: Python",
+    "Typing :: Typed",
+]
 dependencies = [
     "gin-config>=0.5.0",
     "numpy>=1.25.0",
     "torch>=2.0.1",
     "loguru>=0.7.0",
     "ray[tune]>=2.5.1",
     "tqdm>=4.65.0",
@@ -34,29 +40,23 @@
     "flake8-annotations>=3.0.1",
     "black>=23.3.0",
     "flake8>=6.0.0",
     "isort>=5.12.0",
     "mypy>=1.4.1",
 ]
 
-[tools.urls]
-GitHub = "https://github.com/raoulg/mltrainer"
-classifiers = [
-    "Development Status :: 3 - Alpha",
-    "Topic :: Scientific/Engineering :: Artificial Intelligence",
-    "Programming Language :: Python",
-    "Typing :: Typed",
-]
-
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
+[tools.urls]
+GitHub = "https://github.com/raoulg/mltrainer"
+
 [tool.flake8]
 ignore = [
     "W503",
     "ANN101",
     "ANN002",
     "ANN003",
 ]
```

