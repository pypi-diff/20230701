# Comparing `tmp/pyhdtoolkit-1.3.2.tar.gz` & `tmp/pyhdtoolkit-1.4.0.tar.gz`

## Comparing `pyhdtoolkit-1.3.2.tar` & `pyhdtoolkit-1.4.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/.codeclimate.yml
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/.zenodo.json
--rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/Makefile
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/__init__.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/version.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/__init__.py
--rw-r--r--   0        0        0    15024 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/_generators.py
--rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/constants.py
--rw-r--r--   0        0        0    14165 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/coupling.py
--rw-r--r--   0        0        0    17934 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/matching.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/parameters.py
--rw-r--r--   0        0        0    20681 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/ptc.py
--rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/track.py
--rw-r--r--   0        0        0    15424 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/tune.py
--rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/twiss.py
--rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/utils.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/lhc/__init__.py
--rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/lhc/_coupling.py
--rw-r--r--   0        0        0    12988 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/lhc/_elements.py
--rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/lhc/_errors.py
--rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/lhc/_misc.py
--rw-r--r--   0        0        0    17925 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/lhc/_powering.py
--rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/lhc/_queries.py
--rw-r--r--   0        0        0     7821 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/lhc/_routines.py
--rw-r--r--   0        0        0    21324 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/lhc/_setup.py
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/lhc/_twiss.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/maths/__init__.py
--rw-r--r--   0        0        0     8912 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/maths/nonconvex_phase_sync.py
--rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/maths/stats_fitting.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/maths/utils.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/models/__init__.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/models/beam.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/models/htc.py
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/models/madx.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/optics/__init__.py
--rw-r--r--   0        0        0     4937 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/optics/beam.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/optics/ripken.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/optics/twiss.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/plotting/__init__.py
--rw-r--r--   0        0        0    15656 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/plotting/aperture.py
--rw-r--r--   0        0        0    10336 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/plotting/crossing.py
--rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/plotting/envelope.py
--rw-r--r--   0        0        0    13071 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/plotting/lattice.py
--rw-r--r--   0        0        0    20361 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/plotting/layout.py
--rw-r--r--   0        0        0     7463 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/plotting/phasespace.py
--rw-r--r--   0        0        0     7052 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/plotting/tune.py
--rw-r--r--   0        0        0    19836 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/plotting/utils.py
--rw-r--r--   0        0        0    11454 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/plotting/sbs/coupling.py
--rw-r--r--   0        0        0     8931 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/plotting/sbs/phase.py
--rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/plotting/styles/__init__.py
--rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/plotting/styles/paper.py
--rw-r--r--   0        0        0     8629 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/plotting/styles/thesis.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/utils/__init__.py
--rw-r--r--   0        0        0     9811 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/utils/_misc.py
--rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/utils/cmdline.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/utils/contexts.py
--rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/utils/executors.py
--rw-r--r--   0        0        0    10703 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/utils/htc_monitor.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/utils/logging.py
--rw-r--r--   0        0        0    32032 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/utils/operations.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyhdtoolkit/utils/printutil.py
--rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/LICENSE
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/README.md
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     5280 2020-02-02 00:00:00.000000 pyhdtoolkit-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/.codeclimate.yml
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/.zenodo.json
+-rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/Makefile
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/__init__.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/version.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/__init__.py
+-rw-r--r--   0        0        0    15024 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/_generators.py
+-rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/constants.py
+-rw-r--r--   0        0        0    14165 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/coupling.py
+-rw-r--r--   0        0        0    17934 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/matching.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/parameters.py
+-rw-r--r--   0        0        0    20681 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/ptc.py
+-rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/track.py
+-rw-r--r--   0        0        0    15424 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/tune.py
+-rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/twiss.py
+-rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/utils.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/lhc/__init__.py
+-rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/lhc/_coupling.py
+-rw-r--r--   0        0        0    12988 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/lhc/_elements.py
+-rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/lhc/_errors.py
+-rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/lhc/_misc.py
+-rw-r--r--   0        0        0    17925 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/lhc/_powering.py
+-rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/lhc/_queries.py
+-rw-r--r--   0        0        0     7821 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/lhc/_routines.py
+-rw-r--r--   0        0        0    21324 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/lhc/_setup.py
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/lhc/_twiss.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/maths/__init__.py
+-rw-r--r--   0        0        0     8912 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/maths/nonconvex_phase_sync.py
+-rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/maths/stats_fitting.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/maths/utils.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/models/__init__.py
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/models/beam.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/models/htc.py
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/models/madx.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/optics/__init__.py
+-rw-r--r--   0        0        0     4937 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/optics/beam.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/optics/ripken.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/optics/twiss.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/plotting/__init__.py
+-rw-r--r--   0        0        0    15656 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/plotting/aperture.py
+-rw-r--r--   0        0        0    10336 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/plotting/crossing.py
+-rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/plotting/envelope.py
+-rw-r--r--   0        0        0    13071 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/plotting/lattice.py
+-rw-r--r--   0        0        0    20361 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/plotting/layout.py
+-rw-r--r--   0        0        0     7463 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/plotting/phasespace.py
+-rw-r--r--   0        0        0     7052 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/plotting/tune.py
+-rw-r--r--   0        0        0    19836 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/plotting/utils.py
+-rw-r--r--   0        0        0    11454 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/plotting/sbs/coupling.py
+-rw-r--r--   0        0        0     8931 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/plotting/sbs/phase.py
+-rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/plotting/styles/__init__.py
+-rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/plotting/styles/paper.py
+-rw-r--r--   0        0        0     8629 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/plotting/styles/thesis.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/utils/__init__.py
+-rw-r--r--   0        0        0     9811 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/utils/_misc.py
+-rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/utils/cmdline.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/utils/contexts.py
+-rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/utils/executors.py
+-rw-r--r--   0        0        0    10745 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/utils/htc_monitor.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/utils/logging.py
+-rw-r--r--   0        0        0    32032 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/utils/operations.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyhdtoolkit/utils/printutil.py
+-rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/LICENSE
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/README.md
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 pyhdtoolkit-1.4.0/PKG-INFO
```

### Comparing `pyhdtoolkit-1.3.2/.codeclimate.yml` & `pyhdtoolkit-1.4.0/.codeclimate.yml`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/Makefile` & `pyhdtoolkit-1.4.0/Makefile`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/__init__.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/version.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = "1.3.2"
+VERSION = "1.4.0"
 
 
 def version_info() -> str:
     """Debug convenience function to give version, platform and runtime information."""
     import platform
     import sys
```

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/_generators.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/_generators.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/constants.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/constants.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/coupling.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/coupling.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/matching.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/matching.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/parameters.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/parameters.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/ptc.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/ptc.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/track.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/track.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/tune.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/tune.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/twiss.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/twiss.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/utils.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/utils.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/lhc/__init__.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/lhc/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/lhc/_coupling.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/lhc/_coupling.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/lhc/_elements.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/lhc/_elements.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/lhc/_errors.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/lhc/_errors.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/lhc/_misc.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/lhc/_misc.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/lhc/_powering.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/lhc/_powering.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/lhc/_queries.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/lhc/_queries.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/lhc/_routines.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/lhc/_routines.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/lhc/_setup.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/lhc/_setup.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/cpymadtools/lhc/_twiss.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/cpymadtools/lhc/_twiss.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/maths/nonconvex_phase_sync.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/maths/nonconvex_phase_sync.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/maths/stats_fitting.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/maths/stats_fitting.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/maths/utils.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/maths/utils.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/models/beam.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/models/beam.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,20 +16,20 @@
     """
     .. versionadded:: 0.12.0
 
     Class to encompass, validate and manipulate properties of a particle beam.
     One can find a usage example in the :ref:`beam enveloppe demo <demo-beam-enveloppe>`.
     """
 
-    pc_GeV: Optional[float]  # Beam momentum [GeV]
+    pc_GeV: Optional[float] = None  # Beam momentum [GeV]
     E_0_GeV: Optional[float] = 0.9382720813  # Particle rest mass energy [GeV], defaults to that of a proton
     charge: Optional[float] = 1  # Particle charge in [e], defaults to that of a proton
-    en_x_m: Optional[float]  # Horizontal normalized emittance [m]
-    en_y_m: Optional[float]  # Vertical normalized emittance [m]
-    deltap_p: Optional[float]  # Momentum deviation
+    en_x_m: Optional[float] = None  # Horizontal normalized emittance [m]
+    en_y_m: Optional[float] = None  # Vertical normalized emittance [m]
+    deltap_p: Optional[float] = None  # Momentum deviation
 
     @property
     def B_rho_Tm(self) -> float:
         """Beam rigidity [T/m]"""
         return self.pc_GeV / 0.3
 
     @property
```

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/models/htc.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/models/htc.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ---------------
 
 Module with ``pydantic`` models to validate and store data obtained by querying the ``HTCondor`` queue.
 """
 from typing import Union
 
 from pendulum import DateTime
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict
 
 
 class BaseSummary(BaseModel):
     """
     .. versionadded:: 0.12.0
 
     Class to encompass and validate the cluster's summary line in the ``condor_q`` output.
@@ -43,14 +43,16 @@
 
 class HTCTaskSummary(BaseModel):
     """
     .. versionadded:: 0.12.0
 
     Class to encompass and validate a specific job's line in the ``condor_q`` output.
     """
+    # This is so pydantic accepts pendulum.DateTime as a validated type
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
     owner: str
     batch_name: int
     submitted: DateTime
     done: Union[int, str]
     run: Union[int, str]
     idle: Union[int, str]
```

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/models/madx.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/models/madx.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/optics/beam.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/optics/beam.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/optics/ripken.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/optics/ripken.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/optics/twiss.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/optics/twiss.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/plotting/aperture.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/plotting/aperture.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/plotting/crossing.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/plotting/crossing.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/plotting/envelope.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/plotting/envelope.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/plotting/lattice.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/plotting/lattice.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/plotting/layout.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/plotting/layout.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/plotting/phasespace.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/plotting/phasespace.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/plotting/tune.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/plotting/tune.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/plotting/utils.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/plotting/utils.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/plotting/sbs/coupling.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/plotting/sbs/coupling.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/plotting/sbs/phase.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/plotting/sbs/phase.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/plotting/styles/__init__.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/plotting/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/plotting/styles/paper.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/plotting/styles/paper.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/plotting/styles/thesis.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/plotting/styles/thesis.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/utils/__init__.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/utils/_misc.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/utils/_misc.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/utils/cmdline.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/utils/cmdline.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/utils/contexts.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/utils/executors.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/utils/executors.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/utils/htc_monitor.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/utils/htc_monitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -148,21 +148,21 @@
 
 
 def _make_cluster_table(owner_name: str, cluster: ClusterSummary) -> Table:
     table = _default_cluster_table()
     for i, source in enumerate(["query", "user", "cluster"]):
         table.add_row(
             "Query" if i == 0 else ("All Users" if i == 2 else owner_name),
-            str(cluster.dict()[source]["jobs"]),
-            str(cluster.dict()[source]["completed"]),
-            str(cluster.dict()[source]["running"]),
-            str(cluster.dict()[source]["idle"]),
-            str(cluster.dict()[source]["held"]),
-            str(cluster.dict()[source]["suspended"]),
-            str(cluster.dict()[source]["removed"]),
+            str(cluster.model_dump()[source]["jobs"]),
+            str(cluster.model_dump()[source]["completed"]),
+            str(cluster.model_dump()[source]["running"]),
+            str(cluster.model_dump()[source]["idle"]),
+            str(cluster.model_dump()[source]["held"]),
+            str(cluster.model_dump()[source]["suspended"]),
+            str(cluster.model_dump()[source]["removed"]),
         )
     return table
 
 
 # ----- Helpers ----- #
```

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/utils/logging.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/utils/operations.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/utils/operations.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyhdtoolkit/utils/printutil.py` & `pyhdtoolkit-1.4.0/pyhdtoolkit/utils/printutil.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/.gitignore` & `pyhdtoolkit-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/LICENSE` & `pyhdtoolkit-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/README.md` & `pyhdtoolkit-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.3.2/pyproject.toml` & `pyhdtoolkit-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Scientific/Engineering :: Visualization",
     "Topic :: Utilities",
 ]
 
@@ -57,15 +58,15 @@
   "pandas >= 1.4",
   "matplotlib >=3.3",
   "scipy >= 1.6",
   "tfs-pandas >= 3.2",
   "loguru < 1.0",
   "cpymad >= 1.9",
   "rich >= 12.0",
-  "pydantic >= 1.0,<2.0",
+  "pydantic >= 2.0",
   "pendulum >= 2.0",
   "optics-functions >= 0.1",
 ]
 
 [project.optional-dependencies]
 test = [
   "pytest >= 6.0",
```

### Comparing `pyhdtoolkit-1.3.2/PKG-INFO` & `pyhdtoolkit-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhdtoolkit
-Version: 1.3.2
+Version: 1.4.0
 Summary: An all-in-one toolkit package to ease my Python work in my PhD.
 Project-URL: homepage, https://github.com/fsoubelet/PyhDToolkit
 Project-URL: repository, https://github.com/fsoubelet/PyhDToolkit
 Project-URL: documentation, https://fsoubelet.github.io/PyhDToolkit
 Project-URL: changelog, https://fsoubelet.github.io/PyhDToolkit/release.html
 Author-email: Felix Soubelet <felix.soubelet@cern.ch>
 License-Expression: MIT
@@ -15,28 +15,29 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Requires-Dist: cpymad>=1.9
 Requires-Dist: loguru<1.0
 Requires-Dist: matplotlib>=3.3
 Requires-Dist: numpy!=1.24,>=1.21
 Requires-Dist: optics-functions>=0.1
 Requires-Dist: pandas>=1.4
 Requires-Dist: pendulum>=2.0
-Requires-Dist: pydantic<2.0,>=1.0
+Requires-Dist: pydantic>=2.0
 Requires-Dist: rich>=12.0
 Requires-Dist: scipy>=1.6
 Requires-Dist: tfs-pandas>=3.2
 Provides-Extra: dev
 Requires-Dist: black>=22.1; extra == 'dev'
 Requires-Dist: isort>=5.10; extra == 'dev'
 Requires-Dist: ruff>=0.0.250; extra == 'dev'
```

#### html2text {}

```diff
@@ -1,28 +1,29 @@
-Metadata-Version: 2.1 Name: pyhdtoolkit Version: 1.3.2 Summary: An all-in-one
+Metadata-Version: 2.1 Name: pyhdtoolkit Version: 1.4.0 Summary: An all-in-one
 toolkit package to ease my Python work in my PhD. Project-URL: homepage, https:
 //github.com/fsoubelet/PyhDToolkit Project-URL: repository, https://github.com/
 fsoubelet/PyhDToolkit Project-URL: documentation, https://fsoubelet.github.io/
 PyhDToolkit Project-URL: changelog, https://fsoubelet.github.io/PyhDToolkit/
 release.html Author-email: Felix Soubelet
 soubelet@cern.ch> License-Expression: MIT License-File: LICENSE Keywords:
 Accelerator Physics,Docker,PHD,Physics Simulation,Visualisation Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: MIT License Classifier: Natural
 Language :: English Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: Implementation :: CPython Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Physics Classifier: Topic ::
-Scientific/Engineering :: Visualization Classifier: Topic :: Utilities
-Requires-Python: >=3.8 Requires-Dist: cpymad>=1.9 Requires-Dist: loguru<1.0
-Requires-Dist: matplotlib>=3.3 Requires-Dist: numpy!=1.24,>=1.21 Requires-Dist:
-optics-functions>=0.1 Requires-Dist: pandas>=1.4 Requires-Dist: pendulum>=2.0
-Requires-Dist: pydantic<2.0,>=1.0 Requires-Dist: rich>=12.0 Requires-Dist:
+Python :: 3.11 Classifier: Programming Language :: Python :: Implementation ::
+CPython Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
+Scientific/Engineering :: Physics Classifier: Topic :: Scientific/Engineering
+:: Visualization Classifier: Topic :: Utilities Requires-Python: >=3.8
+Requires-Dist: cpymad>=1.9 Requires-Dist: loguru<1.0 Requires-Dist:
+matplotlib>=3.3 Requires-Dist: numpy!=1.24,>=1.21 Requires-Dist: optics-
+functions>=0.1 Requires-Dist: pandas>=1.4 Requires-Dist: pendulum>=2.0
+Requires-Dist: pydantic>=2.0 Requires-Dist: rich>=12.0 Requires-Dist:
 scipy>=1.6 Requires-Dist: tfs-pandas>=3.2 Provides-Extra: dev Requires-Dist:
 black>=22.1; extra == 'dev' Requires-Dist: isort>=5.10; extra == 'dev'
 Requires-Dist: ruff>=0.0.250; extra == 'dev' Provides-Extra: docs Requires-
 Dist: sphinx-codeautolink>=0.14; extra == 'docs' Requires-Dist: sphinx-
 copybutton<1.0; extra == 'docs' Requires-Dist: sphinx-gallery<1.0; extra ==
 'docs' Requires-Dist: sphinx-issues>=3.0; extra == 'docs' Requires-Dist:
 sphinx-panels<1.0; extra == 'docs' Requires-Dist: sphinx-prompt>=1.5; extra ==
```

