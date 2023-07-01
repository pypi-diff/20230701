# Comparing `tmp/rvtools-0.1.5.tar.gz` & `tmp/rvtools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rvtools-0.1.5.tar", max compression
+gzip compressed data, was "rvtools-0.1.6.tar", max compression
```

## Comparing `rvtools-0.1.5.tar` & `rvtools-0.1.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1571 2023-06-30 18:44:54.787213 rvtools-0.1.5/README.md
--rw-r--r--   0        0        0      950 2023-06-30 18:55:08.005404 rvtools-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      150 2023-06-30 17:26:45.549942 rvtools-0.1.5/rvtools/__init__.py
--rw-r--r--   0        0        0      408 2023-06-30 18:31:20.324526 rvtools-0.1.5/rvtools/construct/__init__.py
--rw-r--r--   0        0        0      793 2023-06-30 18:31:21.355889 rvtools-0.1.5/rvtools/construct/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2573 2023-06-25 22:21:36.090266 rvtools-0.1.5/rvtools/construct/__pycache__/_helpers.cpython-311.pyc
--rw-r--r--   0        0        0     3390 2023-06-30 17:10:00.426276 rvtools-0.1.5/rvtools/construct/__pycache__/beta.cpython-311.pyc
--rw-r--r--   0        0        0     4740 2023-06-30 18:19:29.450911 rvtools-0.1.5/rvtools/construct/__pycache__/lognorm.cpython-311.pyc
--rw-r--r--   0        0        0     3133 2023-06-30 17:16:00.201884 rvtools-0.1.5/rvtools/construct/__pycache__/loguniform.cpython-311.pyc
--rw-r--r--   0        0        0     3376 2023-06-30 17:14:17.612857 rvtools-0.1.5/rvtools/construct/__pycache__/norm.cpython-311.pyc
--rw-r--r--   0        0        0     1136 2023-06-30 18:49:53.018755 rvtools-0.1.5/rvtools/construct/__pycache__/pert.cpython-311.pyc
--rw-r--r--   0        0        0     1236 2023-06-30 18:49:53.019105 rvtools-0.1.5/rvtools/construct/__pycache__/tp_uniform.cpython-311.pyc
--rw-r--r--   0        0        0     3424 2023-06-30 17:16:00.201337 rvtools-0.1.5/rvtools/construct/__pycache__/uniform.cpython-311.pyc
--rw-r--r--   0        0        0     1535 2023-06-25 22:20:41.612198 rvtools-0.1.5/rvtools/construct/_helpers.py
--rw-r--r--   0        0        0     2103 2023-06-30 17:09:58.826501 rvtools-0.1.5/rvtools/construct/beta.py
--rw-r--r--   0        0        0     3073 2023-06-30 18:08:07.135992 rvtools-0.1.5/rvtools/construct/lognorm.py
--rw-r--r--   0        0        0     1965 2023-06-30 17:15:58.797323 rvtools-0.1.5/rvtools/construct/loguniform.py
--rw-r--r--   0        0        0     1880 2023-06-30 17:13:21.148678 rvtools-0.1.5/rvtools/construct/norm.py
--rw-r--r--   0        0        0      785 2023-06-30 18:36:45.614328 rvtools-0.1.5/rvtools/construct/pert.py
--rw-r--r--   0        0        0      837 2023-06-30 18:36:45.610762 rvtools-0.1.5/rvtools/construct/tp_uniform.py
--rw-r--r--   0        0        0     2224 2023-06-30 17:15:58.794493 rvtools-0.1.5/rvtools/construct/uniform.py
--rw-r--r--   0        0        0      628 2023-06-30 18:22:52.877475 rvtools-0.1.5/rvtools/dists/__init__.py
--rw-r--r--   0        0        0      611 2023-06-30 18:24:18.881448 rvtools-0.1.5/rvtools/dists/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0        0 2023-06-30 14:37:51.404420 rvtools-0.1.5/rvtools/dists/gen/__init__.py
--rw-r--r--   0        0        0      169 2023-06-30 14:37:52.815093 rvtools-0.1.5/rvtools/dists/gen/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2123 2023-06-30 17:34:43.838362 rvtools-0.1.5/rvtools/dists/gen/__pycache__/certainty.cpython-311.pyc
--rw-r--r--   0        0        0     2766 2023-06-30 17:34:43.837781 rvtools-0.1.5/rvtools/dists/gen/__pycache__/halves_uniform.cpython-311.pyc
--rw-r--r--   0        0        0     7374 2023-06-30 17:34:43.837034 rvtools-0.1.5/rvtools/dists/gen/__pycache__/tp_uniform.cpython-311.pyc
--rw-r--r--   0        0        0     1243 2023-06-30 17:26:45.575234 rvtools-0.1.5/rvtools/dists/gen/certainty.py
--rw-r--r--   0        0        0     1350 2023-06-30 17:26:45.578709 rvtools-0.1.5/rvtools/dists/gen/halves_uniform.py
--rw-r--r--   0        0        0     5244 2023-06-30 17:26:45.610428 rvtools-0.1.5/rvtools/dists/gen/tp_uniform.py
--rw-r--r--   0        0        0     1257 2023-06-30 17:26:45.575868 rvtools-0.1.5/rvtools/fam.py
--rw-r--r--   0        0        0        0 2023-06-25 18:12:13.995575 rvtools-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0      499 2023-06-30 16:50:57.527151 rvtools-0.1.5/tests/conftest.py
--rw-r--r--   0        0        0      345 2023-06-30 17:22:10.404617 rvtools-0.1.5/tests/test_certainty.py
--rw-r--r--   0        0        0     5745 2023-06-29 15:12:37.194609 rvtools-0.1.5/tests/test_constructors.py
--rw-r--r--   0        0        0     2159 2023-06-26 22:48:01.912458 rvtools-0.1.5/tests/test_parse_spec.py
--rw-r--r--   0        0        0      256 2023-06-30 17:25:47.032459 rvtools-0.1.5/tests/test_readme_does_not_raise.py
--rw-r--r--   0        0        0     4440 2023-06-30 17:21:54.412641 rvtools-0.1.5/tests/test_tp_uniform.py
--rw-r--r--   0        0        0      943 2023-06-30 17:26:45.583827 rvtools-0.1.5/tests/test_types.py
--rw-r--r--   0        0        0     2217 1970-01-01 00:00:00.000000 rvtools-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1623 2023-06-30 19:02:53.518689 rvtools-0.1.6/README.md
+-rw-r--r--   0        0        0      950 2023-07-01 13:53:11.589524 rvtools-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      150 2023-06-30 17:26:45.549942 rvtools-0.1.6/rvtools/__init__.py
+-rw-r--r--   0        0        0      408 2023-06-30 18:31:20.324526 rvtools-0.1.6/rvtools/construct/__init__.py
+-rw-r--r--   0        0        0      793 2023-06-30 18:31:21.355889 rvtools-0.1.6/rvtools/construct/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2573 2023-06-25 22:21:36.090266 rvtools-0.1.6/rvtools/construct/__pycache__/_helpers.cpython-311.pyc
+-rw-r--r--   0        0        0     3390 2023-06-30 17:10:00.426276 rvtools-0.1.6/rvtools/construct/__pycache__/beta.cpython-311.pyc
+-rw-r--r--   0        0        0     4740 2023-06-30 18:19:29.450911 rvtools-0.1.6/rvtools/construct/__pycache__/lognorm.cpython-311.pyc
+-rw-r--r--   0        0        0     3133 2023-06-30 17:16:00.201884 rvtools-0.1.6/rvtools/construct/__pycache__/loguniform.cpython-311.pyc
+-rw-r--r--   0        0        0     3376 2023-06-30 17:14:17.612857 rvtools-0.1.6/rvtools/construct/__pycache__/norm.cpython-311.pyc
+-rw-r--r--   0        0        0     1136 2023-06-30 18:49:53.018755 rvtools-0.1.6/rvtools/construct/__pycache__/pert.cpython-311.pyc
+-rw-r--r--   0        0        0     1236 2023-06-30 18:49:53.019105 rvtools-0.1.6/rvtools/construct/__pycache__/tp_uniform.cpython-311.pyc
+-rw-r--r--   0        0        0     3424 2023-06-30 17:16:00.201337 rvtools-0.1.6/rvtools/construct/__pycache__/uniform.cpython-311.pyc
+-rw-r--r--   0        0        0     1535 2023-06-25 22:20:41.612198 rvtools-0.1.6/rvtools/construct/_helpers.py
+-rw-r--r--   0        0        0     2103 2023-06-30 17:09:58.826501 rvtools-0.1.6/rvtools/construct/beta.py
+-rw-r--r--   0        0        0     3073 2023-06-30 18:08:07.135992 rvtools-0.1.6/rvtools/construct/lognorm.py
+-rw-r--r--   0        0        0     1965 2023-06-30 17:15:58.797323 rvtools-0.1.6/rvtools/construct/loguniform.py
+-rw-r--r--   0        0        0     1880 2023-06-30 17:13:21.148678 rvtools-0.1.6/rvtools/construct/norm.py
+-rw-r--r--   0        0        0      785 2023-06-30 18:36:45.614328 rvtools-0.1.6/rvtools/construct/pert.py
+-rw-r--r--   0        0        0      837 2023-06-30 18:36:45.610762 rvtools-0.1.6/rvtools/construct/tp_uniform.py
+-rw-r--r--   0        0        0     2224 2023-06-30 17:15:58.794493 rvtools-0.1.6/rvtools/construct/uniform.py
+-rw-r--r--   0        0        0      628 2023-06-30 18:22:52.877475 rvtools-0.1.6/rvtools/dists/__init__.py
+-rw-r--r--   0        0        0      611 2023-06-30 18:24:18.881448 rvtools-0.1.6/rvtools/dists/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2023-06-30 14:37:51.404420 rvtools-0.1.6/rvtools/dists/gen/__init__.py
+-rw-r--r--   0        0        0      169 2023-06-30 14:37:52.815093 rvtools-0.1.6/rvtools/dists/gen/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2123 2023-06-30 17:34:43.838362 rvtools-0.1.6/rvtools/dists/gen/__pycache__/certainty.cpython-311.pyc
+-rw-r--r--   0        0        0     2766 2023-06-30 17:34:43.837781 rvtools-0.1.6/rvtools/dists/gen/__pycache__/halves_uniform.cpython-311.pyc
+-rw-r--r--   0        0        0     7374 2023-06-30 17:34:43.837034 rvtools-0.1.6/rvtools/dists/gen/__pycache__/tp_uniform.cpython-311.pyc
+-rw-r--r--   0        0        0     1243 2023-06-30 17:26:45.575234 rvtools-0.1.6/rvtools/dists/gen/certainty.py
+-rw-r--r--   0        0        0     1350 2023-06-30 17:26:45.578709 rvtools-0.1.6/rvtools/dists/gen/halves_uniform.py
+-rw-r--r--   0        0        0     5244 2023-06-30 17:26:45.610428 rvtools-0.1.6/rvtools/dists/gen/tp_uniform.py
+-rw-r--r--   0        0        0     1257 2023-06-30 17:26:45.575868 rvtools-0.1.6/rvtools/fam.py
+-rw-r--r--   0        0        0        0 2023-06-25 18:12:13.995575 rvtools-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0      499 2023-06-30 16:50:57.527151 rvtools-0.1.6/tests/conftest.py
+-rw-r--r--   0        0        0      345 2023-06-30 17:22:10.404617 rvtools-0.1.6/tests/test_certainty.py
+-rw-r--r--   0        0        0     5745 2023-06-29 15:12:37.194609 rvtools-0.1.6/tests/test_constructors.py
+-rw-r--r--   0        0        0     2159 2023-06-26 22:48:01.912458 rvtools-0.1.6/tests/test_parse_spec.py
+-rw-r--r--   0        0        0      256 2023-06-30 17:25:47.032459 rvtools-0.1.6/tests/test_readme_does_not_raise.py
+-rw-r--r--   0        0        0     4440 2023-06-30 17:21:54.412641 rvtools-0.1.6/tests/test_tp_uniform.py
+-rw-r--r--   0        0        0      943 2023-06-30 17:26:45.583827 rvtools-0.1.6/tests/test_types.py
+-rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 rvtools-0.1.6/PKG-INFO
```

### Comparing `rvtools-0.1.5/README.md` & `rvtools-0.1.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -4,28 +4,29 @@
 ```shell
 pip install rvtools  # or `poetry add rvtools`
 ```
 # [Documentation](https://tadamcz.com/rvtools/)
 
 # Sample usage
 ```python
-from rvtools.construct import lognorm, uniform, loguniform, CopulaJoint, beta
-from rvtools.dists import pert, certainty
+from rvtools.construct import lognorm, uniform, loguniform, CopulaJoint, beta, pert, certainty
 # PERT distribution: (min, mode, max) like triangular, but smoother shape
 pert(1, 2, 4)
 
 lognorm(mu=1, sigma=2) # SciPy equivalent: lognorm(scale=np.exp(mu), s=sigma). Hard to remember.
 lognorm(mean=3, sd=4)  # Would need explicit calculation in SciPy
 lognorm(p50=1, p95=2)  # Percentiles. Would need explicit calculation in SciPy
 
 uniform(1, 2)  # SciPy equivalent: uniform(1, scale=2-1). Can trip you up.
 uniform(2, 1)  # Not possible to invert the order in SciPy even though it's mathematically equivalent
 
 loguniform(p10=42, p90=100)  # Percentiles. Would need explicit calculation in SciPy
 
+certainty(42)  # 100% probability of 42, but as a _continuous_ distribution
+
 # Arbitrary quantiles (not just integer percentiles)
 lognorm(quantiles={0.0123: 1, 999/1000: 2})
 
 # Copula
 # Specify a joint probability distribution from arbitrary marginal distributions
 # and pairwise rank correlations.
 marginals = {
```

### Comparing `rvtools-0.1.5/pyproject.toml` & `rvtools-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "rvtools"
-version = "0.1.5"
+version = "0.1.6"
 homepage = "https://github.com/tadamcz/rvtools"
 description = "Top-level package for Probability distribution and random variable tools."
 authors = ["Tom Adamczewski <tadamczewskipublic@gmail.com>"]
 readme = "README.md"
 classifiers=[
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
```

### Comparing `rvtools-0.1.5/rvtools/construct/__pycache__/__init__.cpython-311.pyc` & `rvtools-0.1.6/rvtools/construct/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/rvtools/construct/__pycache__/_helpers.cpython-311.pyc` & `rvtools-0.1.6/rvtools/construct/__pycache__/_helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/rvtools/construct/__pycache__/beta.cpython-311.pyc` & `rvtools-0.1.6/rvtools/construct/__pycache__/beta.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/rvtools/construct/__pycache__/lognorm.cpython-311.pyc` & `rvtools-0.1.6/rvtools/construct/__pycache__/lognorm.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/rvtools/construct/__pycache__/loguniform.cpython-311.pyc` & `rvtools-0.1.6/rvtools/construct/__pycache__/loguniform.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/rvtools/construct/__pycache__/norm.cpython-311.pyc` & `rvtools-0.1.6/rvtools/construct/__pycache__/norm.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/rvtools/construct/__pycache__/pert.cpython-311.pyc` & `rvtools-0.1.6/rvtools/construct/__pycache__/pert.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/rvtools/construct/__pycache__/tp_uniform.cpython-311.pyc` & `rvtools-0.1.6/rvtools/construct/__pycache__/tp_uniform.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/rvtools/construct/__pycache__/uniform.cpython-311.pyc` & `rvtools-0.1.6/rvtools/construct/__pycache__/uniform.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/rvtools/construct/_helpers.py` & `rvtools-0.1.6/rvtools/construct/_helpers.py`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/rvtools/construct/beta.py` & `rvtools-0.1.6/rvtools/construct/beta.py`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/rvtools/construct/lognorm.py` & `rvtools-0.1.6/rvtools/construct/lognorm.py`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/rvtools/construct/loguniform.py` & `rvtools-0.1.6/rvtools/construct/loguniform.py`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/rvtools/construct/norm.py` & `rvtools-0.1.6/rvtools/construct/norm.py`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/rvtools/construct/pert.py` & `rvtools-0.1.6/rvtools/construct/pert.py`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/rvtools/construct/tp_uniform.py` & `rvtools-0.1.6/rvtools/construct/tp_uniform.py`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/rvtools/construct/uniform.py` & `rvtools-0.1.6/rvtools/construct/uniform.py`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/rvtools/dists/__init__.py` & `rvtools-0.1.6/rvtools/dists/__init__.py`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/rvtools/dists/__pycache__/__init__.cpython-311.pyc` & `rvtools-0.1.6/rvtools/dists/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/rvtools/dists/gen/__pycache__/certainty.cpython-311.pyc` & `rvtools-0.1.6/rvtools/dists/gen/__pycache__/certainty.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/rvtools/dists/gen/__pycache__/halves_uniform.cpython-311.pyc` & `rvtools-0.1.6/rvtools/dists/gen/__pycache__/halves_uniform.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/rvtools/dists/gen/__pycache__/tp_uniform.cpython-311.pyc` & `rvtools-0.1.6/rvtools/dists/gen/__pycache__/tp_uniform.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/rvtools/dists/gen/certainty.py` & `rvtools-0.1.6/rvtools/dists/gen/certainty.py`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/rvtools/dists/gen/halves_uniform.py` & `rvtools-0.1.6/rvtools/dists/gen/halves_uniform.py`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/rvtools/dists/gen/tp_uniform.py` & `rvtools-0.1.6/rvtools/dists/gen/tp_uniform.py`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/rvtools/fam.py` & `rvtools-0.1.6/rvtools/fam.py`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/tests/test_constructors.py` & `rvtools-0.1.6/tests/test_constructors.py`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/tests/test_parse_spec.py` & `rvtools-0.1.6/tests/test_parse_spec.py`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/tests/test_tp_uniform.py` & `rvtools-0.1.6/tests/test_tp_uniform.py`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/tests/test_types.py` & `rvtools-0.1.6/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.5/PKG-INFO` & `rvtools-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rvtools
-Version: 0.1.5
+Version: 0.1.6
 Summary: Top-level package for Probability distribution and random variable tools.
 Home-page: https://github.com/tadamcz/rvtools
 Author: Tom Adamczewski
 Author-email: tadamczewskipublic@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
@@ -21,28 +21,29 @@
 ```shell
 pip install rvtools  # or `poetry add rvtools`
 ```
 # [Documentation](https://tadamcz.com/rvtools/)
 
 # Sample usage
 ```python
-from rvtools.construct import lognorm, uniform, loguniform, CopulaJoint, beta
-from rvtools.dists import pert, certainty
+from rvtools.construct import lognorm, uniform, loguniform, CopulaJoint, beta, pert, certainty
 # PERT distribution: (min, mode, max) like triangular, but smoother shape
 pert(1, 2, 4)
 
 lognorm(mu=1, sigma=2) # SciPy equivalent: lognorm(scale=np.exp(mu), s=sigma). Hard to remember.
 lognorm(mean=3, sd=4)  # Would need explicit calculation in SciPy
 lognorm(p50=1, p95=2)  # Percentiles. Would need explicit calculation in SciPy
 
 uniform(1, 2)  # SciPy equivalent: uniform(1, scale=2-1). Can trip you up.
 uniform(2, 1)  # Not possible to invert the order in SciPy even though it's mathematically equivalent
 
 loguniform(p10=42, p90=100)  # Percentiles. Would need explicit calculation in SciPy
 
+certainty(42)  # 100% probability of 42, but as a _continuous_ distribution
+
 # Arbitrary quantiles (not just integer percentiles)
 lognorm(quantiles={0.0123: 1, 999/1000: 2})
 
 # Copula
 # Specify a joint probability distribution from arbitrary marginal distributions
 # and pairwise rank correlations.
 marginals = {
```

