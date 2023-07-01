# Comparing `tmp/spectrochempy-0.6.6.tar.gz` & `tmp/spectrochempy-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrochempy-0.6.6.tar", last modified: Sat Jun 17 10:08:33 2023, max compression
+gzip compressed data, was "spectrochempy-0.6.7.tar", last modified: Sat Jul  1 08:03:41 2023, max compression
```

## Comparing `spectrochempy-0.6.6.tar` & `spectrochempy-0.6.7.tar`

### file list

```diff
@@ -1,360 +1,368 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.265452 spectrochempy-0.6.6/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/.codeclimate.yml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/.codespellrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.217447 spectrochempy-0.6.6/.conda/
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/.conda/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    18144 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    21393 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.221448 spectrochempy-0.6.6/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/LICENSES/NMRGLUE_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/LICENSES/NNMF_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/LICENSES/PACKAGING_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/LICENSES/PANDAS_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/LICENSES/TRAITTYPES_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/LICENSES/WHITTAKER_SMOOTH_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-17 10:08:33.265452 spectrochempy-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/environment_dev.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/environment_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.221448 spectrochempy-0.6.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/requirements/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/requirements/requirements_test.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.221448 spectrochempy-0.6.6/scp_data/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.221448 spectrochempy-0.6.6/scp_data/databases/
--rw-r--r--   0 runner    (1001) docker     (123)    26810 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/databases/isotopes.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.229449 spectrochempy-0.6.6/scp_data/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    38040 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/Felipa-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    25832 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/Humor-Sans.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/LICENSE_felipa.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/LICENSE_victormono.txt
--rw-r--r--   0 runner    (1001) docker     (123)   157048 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   197120 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   164392 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-BoldOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150324 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-ExtraLight.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   184764 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-ExtraLightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   156852 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-ExtraLightOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188172 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150888 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188268 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   157596 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-LightOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   153808 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   194336 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161360 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-MediumOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   158228 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-Oblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   151576 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   155276 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   193176 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161200 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-SemiBoldOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150284 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188288 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-ThinItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   157184 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-ThinOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   105316 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/comic-sans-ms.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.229449 spectrochempy-0.6.6/scp_data/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/stylesheets/grayscale.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/stylesheets/notebook.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/stylesheets/paper.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/stylesheets/poster.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/stylesheets/sans.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/stylesheets/scpy.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/stylesheets/serif.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/stylesheets/talk.mplstyle
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.229449 spectrochempy-0.6.6/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scripts/checkindex.py
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scripts/validate_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-17 10:08:33.265452 spectrochempy-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.229449 spectrochempy-0.6.6/spectrochempy/
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.233449 spectrochempy-0.6.6/spectrochempy/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.233449 spectrochempy-0.6.6/spectrochempy/analysis/_base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53764 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/_base/_analysisbase.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.233449 spectrochempy-0.6.6/spectrochempy/analysis/baseline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/baseline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/baseline/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    39539 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/baseline/baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/baseline/baseline_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/baseline/baselineutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.233449 spectrochempy-0.6.6/spectrochempy/analysis/crossdecomposition/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/crossdecomposition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/crossdecomposition/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/crossdecomposition/pls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.233449 spectrochempy-0.6.6/spectrochempy/analysis/curvefitting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/curvefitting/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9926 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/curvefitting/_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/curvefitting/_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/curvefitting/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/curvefitting/linearregression.py
--rw-r--r--   0 runner    (1001) docker     (123)    36742 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/curvefitting/optimize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.237450 spectrochempy-0.6.6/spectrochempy/analysis/decomposition/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/decomposition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/decomposition/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/decomposition/efa.py
--rw-r--r--   0 runner    (1001) docker     (123)    11441 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/decomposition/fast_ica.py
--rw-r--r--   0 runner    (1001) docker     (123)    35222 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/decomposition/iris.py
--rw-r--r--   0 runner    (1001) docker     (123)    49037 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/decomposition/mcrals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/decomposition/nmf.py
--rw-r--r--   0 runner    (1001) docker     (123)    22562 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/decomposition/pca.py
--rw-r--r--   0 runner    (1001) docker     (123)    21127 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/decomposition/simplisma.py
--rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/decomposition/svd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.237450 spectrochempy-0.6.6/spectrochempy/analysis/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/integration/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/integration/integrate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.237450 spectrochempy-0.6.6/spectrochempy/analysis/kinetic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/kinetic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/kinetic/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    59505 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/kinetic/kineticutilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.237450 spectrochempy-0.6.6/spectrochempy/analysis/peakfinding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/peakfinding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/peakfinding/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13470 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/peakfinding/peakfinding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.237450 spectrochempy-0.6.6/spectrochempy/application/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/application/_check_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    32609 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/application/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/application/datadir.py
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/application/general_preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)    47037 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/application/plot_preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/application/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.237450 spectrochempy-0.6.6/spectrochempy/core/
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.237450 spectrochempy-0.6.6/spectrochempy/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/common/dialogs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.241450 spectrochempy-0.6.6/spectrochempy/core/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/dataset/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.241450 spectrochempy-0.6.6/spectrochempy/core/dataset/arraymixins/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/dataset/arraymixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15237 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/dataset/arraymixins/ndio.py
--rw-r--r--   0 runner    (1001) docker     (123)   119944 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/dataset/arraymixins/ndmath.py
--rw-r--r--   0 runner    (1001) docker     (123)    27604 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/dataset/arraymixins/ndplot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.241450 spectrochempy-0.6.6/spectrochempy/core/dataset/baseobjects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/dataset/baseobjects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/dataset/baseobjects/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    75007 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/dataset/baseobjects/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)    22940 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/dataset/baseobjects/ndcomplex.py
--rw-r--r--   0 runner    (1001) docker     (123)    30311 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/dataset/coord.py
--rw-r--r--   0 runner    (1001) docker     (123)    37757 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/dataset/coordset.py
--rw-r--r--   0 runner    (1001) docker     (123)    53490 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/dataset/nddataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.241450 spectrochempy-0.6.6/spectrochempy/core/plotters/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/plotters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/plotters/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/plotters/multiplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    21204 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/plotters/plot1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    26223 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/plotters/plot2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/plotters/plot3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/plotters/plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.241450 spectrochempy-0.6.6/spectrochempy/core/project/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/project/abstractproject.py
--rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/project/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.245450 spectrochempy-0.6.6/spectrochempy/core/readers/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    29953 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/read_carroucell.py
--rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/read_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    11381 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/read_jcamp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/read_labspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/read_matlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    39331 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/read_omnic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/read_opus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/read_quadera.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/read_soc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17013 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/read_spc.py
--rw-r--r--   0 runner    (1001) docker     (123)    45425 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/read_topspin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/read_zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.245450 spectrochempy-0.6.6/spectrochempy/core/script/
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.245450 spectrochempy-0.6.6/spectrochempy/core/units/
--rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/units/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.245450 spectrochempy-0.6.6/spectrochempy/core/writers/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/writers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/writers/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/writers/write_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/writers/write_excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/writers/write_jcamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/writers/write_matlab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.245450 spectrochempy-0.6.6/spectrochempy/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.245450 spectrochempy-0.6.6/spectrochempy/examples/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.249451 spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_efa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_efa_keller_massart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_fast_ica.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_iris.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_mcrals_chrom1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_mcrals_kinetics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_nmf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_pca_iris.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_pca_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_simplisma.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.249451 spectrochempy-0.6.6/spectrochempy/examples/analysis/b_crossdecomposition/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/b_crossdecomposition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/b_crossdecomposition/plot_pls.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/b_crossdecomposition/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.249451 spectrochempy-0.6.6/spectrochempy/examples/analysis/c_curvefitting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/c_curvefitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/c_curvefitting/plot_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/c_curvefitting/plot_lstsq_single_equation.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/c_curvefitting/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.249451 spectrochempy-0.6.6/spectrochempy/examples/analysis/d_baseline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/d_baseline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/d_baseline/plot_baseline_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/d_baseline/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.249451 spectrochempy-0.6.6/spectrochempy/examples/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.249451 spectrochempy-0.6.6/spectrochempy/examples/core/a_nddataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/a_nddataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/a_nddataset/plot_a_create_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/a_nddataset/plot_b_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/a_nddataset/plot_c_units.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/a_nddataset/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.249451 spectrochempy-0.6.6/spectrochempy/examples/core/b_units/
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/b_units/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.253451 spectrochempy-0.6.6/spectrochempy/examples/core/c_importer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/c_importer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/c_importer/plot_generic_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/c_importer/plot_read_IR_from_omnic.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/c_importer/plot_read_IR_from_opus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/c_importer/plot_read_nmr_from_bruker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/c_importer/plot_read_raman_from_labspec.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/c_importer/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.253451 spectrochempy-0.6.6/spectrochempy/examples/core/d_plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/d_plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/d_plotting/plot_plot_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/d_plotting/plot_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/d_plotting/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.253451 spectrochempy-0.6.6/spectrochempy/examples/core/e_project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/e_project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/e_project/plot_project.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/e_project/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.253451 spectrochempy-0.6.6/spectrochempy/examples/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.253451 spectrochempy-0.6.6/spectrochempy/examples/processing/apodization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/apodization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/apodization/plot_proc_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/apodization/plot_proc_sp.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/apodization/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.253451 spectrochempy-0.6.6/spectrochempy/examples/processing/denoising/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/denoising/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/denoising/plot_denoising.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/denoising/plot_despike.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/denoising/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.253451 spectrochempy-0.6.6/spectrochempy/examples/processing/filtering/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/filtering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/filtering/plot_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/filtering/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.257452 spectrochempy-0.6.6/spectrochempy/examples/processing/raman/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/raman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/raman/plot_raman_process.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/raman/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.257452 spectrochempy-0.6.6/spectrochempy/extern/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/extern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64415 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/extern/nmrglue.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/extern/traittypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/extern/traittypes_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/extern/whittaker_smooth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.257452 spectrochempy-0.6.6/spectrochempy/ipython/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/ipython/magics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.257452 spectrochempy-0.6.6/spectrochempy/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.257452 spectrochempy-0.6.6/spectrochempy/processing/_base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/_base/_processingbase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.257452 spectrochempy-0.6.6/spectrochempy/processing/alignement/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/alignement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15773 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/alignement/align.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/alignement/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.257452 spectrochempy-0.6.6/spectrochempy/processing/fft/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/fft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/fft/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24702 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/fft/apodization.py
--rw-r--r--   0 runner    (1001) docker     (123)    19382 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/fft/fft.py
--rw-r--r--   0 runner    (1001) docker     (123)    23167 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/fft/phasing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/fft/shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/fft/zero_filling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.257452 spectrochempy-0.6.6/spectrochempy/processing/filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/filter/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/filter/denoise.py
--rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/filter/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.261452 spectrochempy-0.6.6/spectrochempy/processing/interpolation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/interpolation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/interpolation/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/interpolation/interpolate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.261452 spectrochempy-0.6.6/spectrochempy/processing/transformation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/transformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/transformation/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/transformation/autosub.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/transformation/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/transformation/npy.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/structure.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.265452 spectrochempy-0.6.6/spectrochempy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14466 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/baseconfigurable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/citation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/coordrange.py
--rw-r--r--   0 runner    (1001) docker     (123)    18013 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/decorators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14507 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/fake.py
--rw-r--r--   0 runner    (1001) docker     (123)    23764 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/jsonutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/metaconfigurable.py
--rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/numutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/optional.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/orderedset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/packages.py
--rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/print.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3422 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/print_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (123)    33071 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/timeutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/traits.py
--rw-r--r--   0 runner    (1001) docker     (123)    16115 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.265452 spectrochempy-0.6.6/spectrochempy/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/widgets/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/widgets/baselinecorrector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/widgets/fileselector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.233449 spectrochempy-0.6.6/spectrochempy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-17 10:08:32.000000 spectrochempy-0.6.6/spectrochempy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12463 2023-06-17 10:08:33.000000 spectrochempy-0.6.6/spectrochempy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 10:08:32.000000 spectrochempy-0.6.6/spectrochempy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 10:08:32.000000 spectrochempy-0.6.6/spectrochempy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-17 10:08:32.000000 spectrochempy-0.6.6/spectrochempy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-17 10:08:32.000000 spectrochempy-0.6.6/spectrochempy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.450460 spectrochempy-0.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/.codeclimate.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/.codespellrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.410459 spectrochempy-0.6.7/.conda/
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/.conda/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    18144 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    21393 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.410459 spectrochempy-0.6.7/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/LICENSES/NMRGLUE_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/LICENSES/NNMF_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/LICENSES/PACKAGING_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/LICENSES/PANDAS_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/LICENSES/PY_WDF_READER_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/LICENSES/TRAITTYPES_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/LICENSES/WHITTAKER_SMOOTH_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-07-01 08:03:41.450460 spectrochempy-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/environment_dev.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/environment_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.410459 spectrochempy-0.6.7/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/requirements/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/requirements/requirements_test.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.410459 spectrochempy-0.6.7/scp_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.410459 spectrochempy-0.6.7/scp_data/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)    26810 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/databases/isotopes.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.418460 spectrochempy-0.6.7/scp_data/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    38040 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/fonts/Felipa-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    25832 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/fonts/Humor-Sans.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/fonts/LICENSE_felipa.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/fonts/LICENSE_victormono.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   157048 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/fonts/VictorMono-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   197120 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/fonts/VictorMono-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   164392 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/fonts/VictorMono-BoldOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150324 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/fonts/VictorMono-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   184764 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/fonts/VictorMono-ExtraLightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   156852 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/fonts/VictorMono-ExtraLightOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188172 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/fonts/VictorMono-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150888 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/fonts/VictorMono-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188268 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/fonts/VictorMono-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   157596 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/fonts/VictorMono-LightOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   153808 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/fonts/VictorMono-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   194336 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/fonts/VictorMono-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161360 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/fonts/VictorMono-MediumOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   158228 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/fonts/VictorMono-Oblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   151576 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/fonts/VictorMono-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   155276 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/fonts/VictorMono-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   193176 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/fonts/VictorMono-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161200 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/fonts/VictorMono-SemiBoldOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150284 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/fonts/VictorMono-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188288 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/fonts/VictorMono-ThinItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   157184 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/fonts/VictorMono-ThinOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   105316 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/fonts/comic-sans-ms.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.418460 spectrochempy-0.6.7/scp_data/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/stylesheets/grayscale.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/stylesheets/notebook.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/stylesheets/paper.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/stylesheets/poster.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/stylesheets/sans.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/stylesheets/scpy.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/stylesheets/serif.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scp_data/stylesheets/talk.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.418460 spectrochempy-0.6.7/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scripts/checkindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/scripts/validate_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-01 08:03:41.450460 spectrochempy-0.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.418460 spectrochempy-0.6.7/spectrochempy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.418460 spectrochempy-0.6.7/spectrochempy/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.418460 spectrochempy-0.6.7/spectrochempy/analysis/_base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53764 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/_base/_analysisbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.422459 spectrochempy-0.6.7/spectrochempy/analysis/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/baseline/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39540 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/baseline/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/baseline/baseline_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/baseline/baselineutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.422459 spectrochempy-0.6.7/spectrochempy/analysis/crossdecomposition/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/crossdecomposition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/crossdecomposition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/crossdecomposition/pls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.422459 spectrochempy-0.6.7/spectrochempy/analysis/curvefitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/curvefitting/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9926 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/curvefitting/_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/curvefitting/_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/curvefitting/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/curvefitting/linearregression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36916 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/curvefitting/optimize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.422459 spectrochempy-0.6.7/spectrochempy/analysis/decomposition/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/decomposition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/decomposition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/decomposition/efa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11441 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/decomposition/fast_ica.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35222 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/decomposition/iris.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49184 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/decomposition/mcrals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/decomposition/nmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22562 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/decomposition/pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21127 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/decomposition/simplisma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/decomposition/svd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.422459 spectrochempy-0.6.7/spectrochempy/analysis/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/integration/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/integration/integrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.422459 spectrochempy-0.6.7/spectrochempy/analysis/kinetic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/kinetic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/kinetic/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59505 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/kinetic/kineticutilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.426460 spectrochempy-0.6.7/spectrochempy/analysis/peakfinding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/peakfinding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/peakfinding/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14224 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/peakfinding/peakfinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/analysis/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.426460 spectrochempy-0.6.7/spectrochempy/application/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/application/_check_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32609 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/application/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/application/datadir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/application/general_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47037 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/application/plot_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/application/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.426460 spectrochempy-0.6.7/spectrochempy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.426460 spectrochempy-0.6.7/spectrochempy/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/common/dialogs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.426460 spectrochempy-0.6.7/spectrochempy/core/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/dataset/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.426460 spectrochempy-0.6.7/spectrochempy/core/dataset/arraymixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/dataset/arraymixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15237 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/dataset/arraymixins/ndio.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119944 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/dataset/arraymixins/ndmath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27604 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/dataset/arraymixins/ndplot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.426460 spectrochempy-0.6.7/spectrochempy/core/dataset/baseobjects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/dataset/baseobjects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/dataset/baseobjects/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75007 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/dataset/baseobjects/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22940 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/dataset/baseobjects/ndcomplex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30306 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/dataset/coord.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37782 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/dataset/coordset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53079 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/dataset/nddataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.430460 spectrochempy-0.6.7/spectrochempy/core/plotters/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/plotters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/plotters/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/plotters/multiplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21204 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/plotters/plot1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26223 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/plotters/plot2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/plotters/plot3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/plotters/plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.430460 spectrochempy-0.6.7/spectrochempy/core/project/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/project/abstractproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/project/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.430460 spectrochempy-0.6.7/spectrochempy/core/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/readers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/readers/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30076 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/readers/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/readers/read_carroucell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/readers/read_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11381 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/readers/read_jcamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/readers/read_labspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/readers/read_matlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38766 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/readers/read_omnic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/readers/read_opus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/readers/read_quadera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/readers/read_soc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17013 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/readers/read_spc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45425 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/readers/read_topspin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29565 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/readers/read_wire.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/readers/read_zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.430460 spectrochempy-0.6.7/spectrochempy/core/script/
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.430460 spectrochempy-0.6.7/spectrochempy/core/units/
+-rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/units/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.434460 spectrochempy-0.6.7/spectrochempy/core/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/writers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/writers/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/writers/write_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/writers/write_excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/writers/write_jcamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/core/writers/write_matlab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.434460 spectrochempy-0.6.7/spectrochempy/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.434460 spectrochempy-0.6.7/spectrochempy/examples/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.434460 spectrochempy-0.6.7/spectrochempy/examples/analysis/a_decomposition/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/analysis/a_decomposition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/analysis/a_decomposition/plot_efa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/analysis/a_decomposition/plot_efa_keller_massart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/analysis/a_decomposition/plot_fast_ica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/analysis/a_decomposition/plot_iris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/analysis/a_decomposition/plot_mcrals_chrom1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/analysis/a_decomposition/plot_mcrals_kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/analysis/a_decomposition/plot_nmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/analysis/a_decomposition/plot_pca_iris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/analysis/a_decomposition/plot_pca_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/analysis/a_decomposition/plot_simplisma.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/analysis/a_decomposition/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.434460 spectrochempy-0.6.7/spectrochempy/examples/analysis/b_crossdecomposition/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/analysis/b_crossdecomposition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/analysis/b_crossdecomposition/plot_pls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/analysis/b_crossdecomposition/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.434460 spectrochempy-0.6.7/spectrochempy/examples/analysis/c_curvefitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/analysis/c_curvefitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/analysis/c_curvefitting/plot_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/analysis/c_curvefitting/plot_lstsq_single_equation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/analysis/c_curvefitting/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.434460 spectrochempy-0.6.7/spectrochempy/examples/analysis/d_baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/analysis/d_baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/analysis/d_baseline/plot_baseline_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/analysis/d_baseline/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/analysis/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.434460 spectrochempy-0.6.7/spectrochempy/examples/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.438460 spectrochempy-0.6.7/spectrochempy/examples/core/a_nddataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/core/a_nddataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/core/a_nddataset/plot_a_create_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/core/a_nddataset/plot_b_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/core/a_nddataset/plot_c_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/core/a_nddataset/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.438460 spectrochempy-0.6.7/spectrochempy/examples/core/b_units/
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/core/b_units/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.438460 spectrochempy-0.6.7/spectrochempy/examples/core/c_importer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/core/c_importer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/core/c_importer/plot_generic_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/core/c_importer/plot_read_IR_from_omnic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/core/c_importer/plot_read_IR_from_opus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/core/c_importer/plot_read_nmr_from_bruker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/core/c_importer/plot_read_raman_from_labspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/core/c_importer/plot_read_renishaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/core/c_importer/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.438460 spectrochempy-0.6.7/spectrochempy/examples/core/d_plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/core/d_plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/core/d_plotting/plot_plot_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/core/d_plotting/plot_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/core/d_plotting/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.438460 spectrochempy-0.6.7/spectrochempy/examples/core/e_project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/core/e_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/core/e_project/plot_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/core/e_project/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/core/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.438460 spectrochempy-0.6.7/spectrochempy/examples/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.438460 spectrochempy-0.6.7/spectrochempy/examples/processing/apodization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/processing/apodization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/processing/apodization/plot_proc_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/processing/apodization/plot_proc_sp.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/processing/apodization/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.438460 spectrochempy-0.6.7/spectrochempy/examples/processing/denoising/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/processing/denoising/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/processing/denoising/plot_denoising.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/processing/denoising/plot_despike.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/processing/denoising/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.438460 spectrochempy-0.6.7/spectrochempy/examples/processing/filtering/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/processing/filtering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/processing/filtering/plot_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/processing/filtering/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.442460 spectrochempy-0.6.7/spectrochempy/examples/processing/nmr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/processing/nmr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/processing/nmr/plot_processing_nmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/processing/nmr/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.442460 spectrochempy-0.6.7/spectrochempy/examples/processing/raman/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/processing/raman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/processing/raman/plot_processing_raman.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/processing/raman/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/examples/processing/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.442460 spectrochempy-0.6.7/spectrochempy/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/extern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66123 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/extern/nmrglue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/extern/traittypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/extern/traittypes_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/extern/whittaker_smooth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.442460 spectrochempy-0.6.7/spectrochempy/ipython/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/ipython/magics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.442460 spectrochempy-0.6.7/spectrochempy/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.442460 spectrochempy-0.6.7/spectrochempy/processing/_base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/processing/_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/processing/_base/_processingbase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.442460 spectrochempy-0.6.7/spectrochempy/processing/alignement/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/processing/alignement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15773 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/processing/alignement/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/processing/alignement/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/processing/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.442460 spectrochempy-0.6.7/spectrochempy/processing/fft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/processing/fft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/processing/fft/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24702 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/processing/fft/apodization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19382 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/processing/fft/fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23167 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/processing/fft/phasing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/processing/fft/shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/processing/fft/zero_filling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.442460 spectrochempy-0.6.7/spectrochempy/processing/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/processing/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/processing/filter/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/processing/filter/denoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/processing/filter/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.446460 spectrochempy-0.6.7/spectrochempy/processing/interpolation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/processing/interpolation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/processing/interpolation/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/processing/interpolation/interpolate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.446460 spectrochempy-0.6.7/spectrochempy/processing/transformation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/processing/transformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/processing/transformation/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/processing/transformation/autosub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/processing/transformation/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/processing/transformation/npy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/structure.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.450460 spectrochempy-0.6.7/spectrochempy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14610 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/baseconfigurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/citation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/coordrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/datetimeutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18013 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/decorators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14507 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24356 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/jsonutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/metaconfigurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/numutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/optional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/orderedset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/print.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3422 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/print_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33111 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/timeutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16115 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/utils/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.450460 spectrochempy-0.6.7/spectrochempy/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/widgets/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/widgets/baselinecorrector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-01 08:03:23.000000 spectrochempy-0.6.7/spectrochempy/widgets/fileselector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:03:41.418460 spectrochempy-0.6.7/spectrochempy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-07-01 08:03:41.000000 spectrochempy-0.6.7/spectrochempy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-07-01 08:03:41.000000 spectrochempy-0.6.7/spectrochempy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 08:03:41.000000 spectrochempy-0.6.7/spectrochempy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 08:03:41.000000 spectrochempy-0.6.7/spectrochempy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-01 08:03:41.000000 spectrochempy-0.6.7/spectrochempy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-01 08:03:41.000000 spectrochempy-0.6.7/spectrochempy.egg-info/top_level.txt
```

### Comparing `spectrochempy-0.6.6/.codeclimate.yml` & `spectrochempy-0.6.7/.codeclimate.yml`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/.conda/meta.yaml` & `spectrochempy-0.6.7/.conda/meta.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   script:
     - export SETUPTOOLS_SCM_PRETEND_VERSION={{ version }}
     - {{ PYTHON }} -m pip install .
 
 requirements:
   host:
     - pip
-    - python >=3.8
+    - python >=3.9
     - setuptools
     - setuptools_scm
   run:
     - python
 
     # specific dependencies
     - brukeropusreader
@@ -44,19 +44,19 @@
     - ipython
     - jinja2
     - matplotlib
     - numba
     - numpy
     - numpydoc>=1.2
     - pint>=0.20
-    - pytz
     - requests
     - scipy
     - tqdm
     - traitlets
+    - tzlocal
     - scikit-learn
     - xlrd
     - pyyaml
 
     # dependencies needed mainly for install and a bit more ...
     - setuptools
     - setuptools_scm
```

### Comparing `spectrochempy-0.6.6/.gitignore` & `spectrochempy-0.6.7/.gitignore`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/.pre-commit-config.yaml` & `spectrochempy-0.6.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/.pylintrc` & `spectrochempy-0.6.7/.pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 load-plugins=
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Minimum Python version to use for version dependent checks. Will default to
 # the version used to run pylint.
-py-version=3.8
+py-version=3.9
 
 # When enabled, pylint would attempt to guess common misconfiguration and emit
 # user-friendly hints instead of false-positive error messages.
 suggestion-mode=yes
 
 # Allow loading of arbitrary C extensions. Extensions are imported into the
 # active Python interpreter and may run arbitrary code.
```

### Comparing `spectrochempy-0.6.6/.zenodo.json` & `spectrochempy-0.6.7/.zenodo.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'publication_date'": "'2023-07-01'", "'version'": "'0.6.7'"}*

```diff
@@ -50,12 +50,12 @@
         "raman",
         "raman-spectra",
         "raman-spectroscopy",
         "spectroscopy",
         "uv-vis"
     ],
     "license": "CECILL-B",
-    "publication_date": "2023-06-17",
+    "publication_date": "2023-07-01",
     "title": "SpectroChemPy",
     "upload_type": "software",
-    "version": "0.6.6"
+    "version": "0.6.7"
 }
```

### Comparing `spectrochempy-0.6.6/CITATION.cff` & `spectrochempy-0.6.7/CITATION.cff`

 * *Files 12% similar despite different names*

```diff
@@ -11,20 +11,20 @@
   orcid: https://orcid.org/0000-0002-9579-8910
 - affiliation: "ENSICAEN, Universit\xE9 de Caen, CNRS (Laboratoire Catalyse et Spectrochimie)"
   email: christian.fernandez@ensicaen.fr
   family-names: Fernandez
   given-names: Christian
   orcid: https://orcid.org/0000-0002-5476-3148
 cff-version: 1.2.0
-date-released: '2023-06-17'
+date-released: '2023-07-01'
 identifiers:
 - description: Persistent identifier for all versions of SpectroChemPy
   type: doi
   value: 10.5281/zenodo.3823841
 license: CECILL-B
 message: If you use this software, please cite it using the metadata from this file.
 repository-code: https://github.com/spectrochempy/spectrochempy
 title: SpectroChemPy, a framework for processing, analyzing and modeling spectroscopic
   data for chemistry with Python
 type: software
 url: https://www.spectrochempy.fr
-version: 0.6.6
+version: 0.6.7
```

### Comparing `spectrochempy-0.6.6/Dockerfile` & `spectrochempy-0.6.7/Dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 USER root
 
 RUN sudo apt-get update -y && \
     sudo apt-get install -y libx11-6
 
 USER $NB_UID
 
-# Choose python 3.8 version
-ARG PY_VERSION=3.8
+# Choose python 3.9 version
+ARG PY_VERSION=3.9
 ARG DEV=''
 ARG DASH=''
 ARG CANTERA=''
 ARG BRANCH=''
 
 # ENV CONDA_ENV scpy$PY_VERSION
```

### Comparing `spectrochempy-0.6.6/LICENSE` & `spectrochempy-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/LICENSES/NMRGLUE_LICENSE.rst` & `spectrochempy-0.6.7/LICENSES/NMRGLUE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/LICENSES/NNMF_LICENSE.rst` & `spectrochempy-0.6.7/LICENSES/NNMF_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/LICENSES/PACKAGING_LICENSE.rst` & `spectrochempy-0.6.7/LICENSES/PACKAGING_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/LICENSES/PANDAS_LICENSE.rst` & `spectrochempy-0.6.7/LICENSES/PANDAS_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/LICENSES/TRAITTYPES_LICENSE.rst` & `spectrochempy-0.6.7/LICENSES/TRAITTYPES_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/LICENSES/WHITTAKER_SMOOTH_LICENSE.rst` & `spectrochempy-0.6.7/LICENSES/WHITTAKER_SMOOTH_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/PKG-INFO` & `spectrochempy-0.6.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrochempy
-Version: 0.6.6
+Version: 0.6.7
 Summary: Processing, analysis and modelling Spectroscopic data for Chemistry with Python
 Home-page: https://www.spectrochempy.fr
 Author: Arnaud Travert & Christian Fernandez
 Author-email: contact@spectrochempy.fr
 Maintainer: C. Fernandez
 Maintainer-email: christian.fernandez@ensicaen.fr
 License: CECILL-B
@@ -14,18 +14,17 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: CeCILL-B Free Software License Agreement (CECILL-B)
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align ="center">
 <img src='https://github.com/spectrochempy/spectrochempy/raw/master/docs/_static/scpy.png' width="150">
 <br>
 SpectroChemPy
```

### Comparing `spectrochempy-0.6.6/README.md` & `spectrochempy-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/environment.yml` & `spectrochempy-0.6.7/environment.yml`

 * *Files 18% similar despite different names*

```diff
@@ -33,19 +33,19 @@
     - ipython
     - jinja2
     - matplotlib
     - numba
     - numpy
     - numpydoc>=1.2
     - pint>=0.20
-    - pytz
     - requests
     - scipy
     - tqdm
     - traitlets
+    - tzlocal
     - scikit-learn
     - xlrd
     - pyyaml
 
     # dependencies needed mainly for install and a bit more ...
     - setuptools
     - setuptools_scm
```

### Comparing `spectrochempy-0.6.6/environment_dev.yml` & `spectrochempy-0.6.7/environment_dev.yml`

 * *Files 2% similar despite different names*

```diff
@@ -33,19 +33,19 @@
     - ipython
     - jinja2
     - matplotlib
     - numba
     - numpy
     - numpydoc>=1.2
     - pint>=0.20
-    - pytz
     - requests
     - scipy
     - tqdm
     - traitlets
+    - tzlocal
     - scikit-learn
     - xlrd
     - pyyaml
 
     # dependencies needed mainly for install and a bit more ...
     - setuptools
     - setuptools_scm
```

### Comparing `spectrochempy-0.6.6/environment_test.yml` & `spectrochempy-0.6.7/environment_test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -33,19 +33,19 @@
     - ipython
     - jinja2
     - matplotlib
     - numba
     - numpy
     - numpydoc>=1.2
     - pint>=0.20
-    - pytz
     - requests
     - scipy
     - tqdm
     - traitlets
+    - tzlocal
     - scikit-learn
     - xlrd
     - pyyaml
 
     # dependencies needed mainly for install and a bit more ...
     - setuptools
     - setuptools_scm
```

### Comparing `spectrochempy-0.6.6/requirements/requirements.txt` & `spectrochempy-0.6.7/requirements/requirements.txt`

 * *Files 26% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 ipython
 jinja2
 matplotlib
 numba
 numpy
 numpydoc>=1.2
 pint>=0.20
-pytz
 requests
 scipy
 tqdm
 traitlets
+tzlocal
 scikit-learn
 xlrd
 pyyaml
 setuptools
 setuptools_scm
 gitpython
 ipywidgets==8.0.4
```

### Comparing `spectrochempy-0.6.6/requirements/requirements_dev.txt` & `spectrochempy-0.6.7/requirements/requirements_dev.txt`

 * *Files 16% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 ipython
 jinja2
 matplotlib
 numba
 numpy
 numpydoc>=1.2
 pint>=0.20
-pytz
 requests
 scipy
 tqdm
 traitlets
+tzlocal
 scikit-learn
 xlrd
 pyyaml
 setuptools
 setuptools_scm
 gitpython
 ipywidgets==8.0.4
```

### Comparing `spectrochempy-0.6.6/requirements/requirements_test.txt` & `spectrochempy-0.6.7/requirements/requirements_test.txt`

 * *Files 19% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 ipython
 jinja2
 matplotlib
 numba
 numpy
 numpydoc>=1.2
 pint>=0.20
-pytz
 requests
 scipy
 tqdm
 traitlets
+tzlocal
 scikit-learn
 xlrd
 pyyaml
 setuptools
 setuptools_scm
 gitpython
 ipywidgets==8.0.4
```

### Comparing `spectrochempy-0.6.6/scp_data/databases/isotopes.csv` & `spectrochempy-0.6.7/scp_data/databases/isotopes.csv`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/fonts/Felipa-Regular.ttf` & `spectrochempy-0.6.7/scp_data/fonts/Felipa-Regular.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/fonts/Humor-Sans.ttf` & `spectrochempy-0.6.7/scp_data/fonts/Humor-Sans.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/fonts/LICENSE_felipa.txt` & `spectrochempy-0.6.7/scp_data/fonts/LICENSE_felipa.txt`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/fonts/LICENSE_victormono.txt` & `spectrochempy-0.6.7/scp_data/fonts/LICENSE_victormono.txt`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/fonts/VictorMono-Bold.ttf` & `spectrochempy-0.6.7/scp_data/fonts/VictorMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/fonts/VictorMono-BoldItalic.ttf` & `spectrochempy-0.6.7/scp_data/fonts/VictorMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/fonts/VictorMono-BoldOblique.ttf` & `spectrochempy-0.6.7/scp_data/fonts/VictorMono-BoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/fonts/VictorMono-ExtraLight.ttf` & `spectrochempy-0.6.7/scp_data/fonts/VictorMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/fonts/VictorMono-ExtraLightItalic.ttf` & `spectrochempy-0.6.7/scp_data/fonts/VictorMono-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/fonts/VictorMono-ExtraLightOblique.ttf` & `spectrochempy-0.6.7/scp_data/fonts/VictorMono-ExtraLightOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/fonts/VictorMono-Italic.ttf` & `spectrochempy-0.6.7/scp_data/fonts/VictorMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/fonts/VictorMono-Light.ttf` & `spectrochempy-0.6.7/scp_data/fonts/VictorMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/fonts/VictorMono-LightItalic.ttf` & `spectrochempy-0.6.7/scp_data/fonts/VictorMono-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/fonts/VictorMono-LightOblique.ttf` & `spectrochempy-0.6.7/scp_data/fonts/VictorMono-LightOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/fonts/VictorMono-Medium.ttf` & `spectrochempy-0.6.7/scp_data/fonts/VictorMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/fonts/VictorMono-MediumItalic.ttf` & `spectrochempy-0.6.7/scp_data/fonts/VictorMono-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/fonts/VictorMono-MediumOblique.ttf` & `spectrochempy-0.6.7/scp_data/fonts/VictorMono-MediumOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/fonts/VictorMono-Oblique.ttf` & `spectrochempy-0.6.7/scp_data/fonts/VictorMono-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/fonts/VictorMono-Regular.ttf` & `spectrochempy-0.6.7/scp_data/fonts/VictorMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/fonts/VictorMono-SemiBold.ttf` & `spectrochempy-0.6.7/scp_data/fonts/VictorMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/fonts/VictorMono-SemiBoldItalic.ttf` & `spectrochempy-0.6.7/scp_data/fonts/VictorMono-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/fonts/VictorMono-SemiBoldOblique.ttf` & `spectrochempy-0.6.7/scp_data/fonts/VictorMono-SemiBoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/fonts/VictorMono-Thin.ttf` & `spectrochempy-0.6.7/scp_data/fonts/VictorMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/fonts/VictorMono-ThinItalic.ttf` & `spectrochempy-0.6.7/scp_data/fonts/VictorMono-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/fonts/VictorMono-ThinOblique.ttf` & `spectrochempy-0.6.7/scp_data/fonts/VictorMono-ThinOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/fonts/comic-sans-ms.ttf` & `spectrochempy-0.6.7/scp_data/fonts/comic-sans-ms.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/stylesheets/grayscale.mplstyle` & `spectrochempy-0.6.7/scp_data/stylesheets/grayscale.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/stylesheets/notebook.mplstyle` & `spectrochempy-0.6.7/scp_data/stylesheets/notebook.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/stylesheets/sans.mplstyle` & `spectrochempy-0.6.7/scp_data/stylesheets/sans.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/stylesheets/scpy.mplstyle` & `spectrochempy-0.6.7/scp_data/stylesheets/scpy.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scp_data/stylesheets/serif.mplstyle` & `spectrochempy-0.6.7/scp_data/stylesheets/serif.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scripts/checkindex.py` & `spectrochempy-0.6.7/scripts/checkindex.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/scripts/validate_docstrings.py` & `spectrochempy-0.6.7/scripts/validate_docstrings.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/setup.cfg` & `spectrochempy-0.6.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/setup.py` & `spectrochempy-0.6.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,24 +138,23 @@
         "Development Status :: 3 - Alpha",
         "Topic :: Utilities",
         "Topic :: Scientific/Engineering",
         "Topic :: Software Development :: Libraries",
         "Intended Audience :: Science/Research",
         "License :: CeCILL-B Free Software License Agreement (CECILL-B)",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     platforms=["Windows", "Mac OS X", "Linux"],
     # packages discovery
     zip_safe=False,
     packages=find_packages() + packages,
     include_package_data=True,  # requirements
-    python_requires=">=3.8",
+    python_requires=">=3.9",
     setup_requires=["setuptools_scm>=6.3.2", "matplotlib>=3.5.1"],
     install_requires=read_requirements(),
     # post-commands
     cmdclass={
         "develop": PostDevelopCommand,
         "install": PostInstallCommand,
     },
```

### Comparing `spectrochempy-0.6.6/spectrochempy/__init__.py` & `spectrochempy-0.6.7/spectrochempy/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/_base/_analysisbase.py` & `spectrochempy-0.6.7/spectrochempy/analysis/_base/_analysisbase.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/api.py` & `spectrochempy-0.6.7/spectrochempy/analysis/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/baseline/api.py` & `spectrochempy-0.6.7/spectrochempy/analysis/baseline/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/baseline/baseline.py` & `spectrochempy-0.6.7/spectrochempy/analysis/baseline/baseline.py`

 * *Files 0% similar despite different names*

```diff
@@ -596,14 +596,15 @@
         %(analysis_fit.returns)s
         """
         self._fitted = False  # reinit this flag
 
         # Set X
         # -----
         X = X.copy()
+
         if (
             self.model == "asls"
         ):  # AsLS doesn't work for now with masked data (see _fit)
             # so we will remove the mask and restore it after the fit
             self.Xmasked = X.copy()
             X.remove_masks()
```

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/baseline/baseline_deprecated.py` & `spectrochempy-0.6.7/spectrochempy/analysis/baseline/baseline_deprecated.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/baseline/baselineutils.py` & `spectrochempy-0.6.7/spectrochempy/analysis/baseline/baselineutils.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/crossdecomposition/api.py` & `spectrochempy-0.6.7/spectrochempy/analysis/crossdecomposition/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/crossdecomposition/pls.py` & `spectrochempy-0.6.7/spectrochempy/analysis/crossdecomposition/pls.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/curvefitting/_models.py` & `spectrochempy-0.6.7/spectrochempy/analysis/curvefitting/_models.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/curvefitting/_parameters.py` & `spectrochempy-0.6.7/spectrochempy/analysis/curvefitting/_parameters.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/curvefitting/api.py` & `spectrochempy-0.6.7/spectrochempy/analysis/curvefitting/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/curvefitting/linearregression.py` & `spectrochempy-0.6.7/spectrochempy/analysis/curvefitting/linearregression.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/curvefitting/optimize.py` & `spectrochempy-0.6.7/spectrochempy/analysis/curvefitting/optimize.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,19 +118,22 @@
             **kwargs,
         )
 
     # ----------------------------------------------------------------------------------
     # Private methods ( overriding abstract methods)
     # ----------------------------------------------------------------------------------
     def _fit(self, X, Y=None):
-
         # NMR
         # sequence = kargs.get('sequence', 'ideal_pulse')
         # self.sequence = PulseSequence(type=sequence)
 
+        # for now, we only work with 1D data
+        if X.ndim > 1 and all(np.array(X.shape) > 1):
+            raise NotImplementedError("Only 1D data are supported for now")
+
         # create model data
         modeldata, modelnames, model_A, model_a, model_b = self._get_modeldata(X)
 
         info_("*" * 50)
         info_("  Entering fitting procedure")
         info_("*" * 50)
 
@@ -575,15 +578,14 @@
         # This function is needed for the script related to modelfunction
         #
         # exp_idx: int, contains the index of the experiment
 
         new_param = param.copy()
 
         for key in param:
-
             if param.reference[key]:
                 new_param.reference[key] = False
                 # important to put it here
                 # before other instruction
                 # try to interpret the given refpar expression
                 refpar = param[key]
                 while True:
```

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/decomposition/api.py` & `spectrochempy-0.6.7/spectrochempy/analysis/decomposition/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/decomposition/efa.py` & `spectrochempy-0.6.7/spectrochempy/analysis/decomposition/efa.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/decomposition/fast_ica.py` & `spectrochempy-0.6.7/spectrochempy/analysis/decomposition/fast_ica.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/decomposition/iris.py` & `spectrochempy-0.6.7/spectrochempy/analysis/decomposition/iris.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/decomposition/mcrals.py` & `spectrochempy-0.6.7/spectrochempy/analysis/decomposition/mcrals.py`

 * *Files 1% similar despite different names*

```diff
@@ -955,22 +955,27 @@
 
                 C[:, self.hardConc] = fixedC[:, self.getC_to_C_idx]
 
             # stores C in C_constrained
             # ------------------------------------------
             C_constrained = C.copy()
 
-            # Compute St taking into account non-negativity
-            # --------------------------------------------
+            # Compute St
+            # -----------
             St = self._solve_St(C)
 
             # stores St in St_unconstrained
             # ------------------------------------------
             St_unconstrained = St.copy()
 
+            # Force non-negative spectra
+            # ------------------------------------------
+            if np.any(self.nonnegSpec):
+                St[self.nonnegSpec, :] = St[self.nonnegSpec, :].clip(min=0)
+
             # Force unimodal spectra
             # ------------------------------------------
             if np.any(self.unimodSpec):
                 St = _unimodal_2D(
                     St,
                     idxes=self.unimodSpec,
                     axis=1,
```

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/decomposition/nmf.py` & `spectrochempy-0.6.7/spectrochempy/analysis/decomposition/nmf.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/decomposition/pca.py` & `spectrochempy-0.6.7/spectrochempy/analysis/decomposition/pca.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/decomposition/simplisma.py` & `spectrochempy-0.6.7/spectrochempy/analysis/decomposition/simplisma.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/decomposition/svd.py` & `spectrochempy-0.6.7/spectrochempy/analysis/decomposition/svd.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/integration/api.py` & `spectrochempy-0.6.7/spectrochempy/analysis/integration/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/integration/integrate.py` & `spectrochempy-0.6.7/spectrochempy/analysis/integration/integrate.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/kinetic/api.py` & `spectrochempy-0.6.7/spectrochempy/analysis/kinetic/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/kinetic/kineticutilities.py` & `spectrochempy-0.6.7/spectrochempy/analysis/kinetic/kineticutilities.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/peakfinding/api.py` & `spectrochempy-0.6.7/spectrochempy/analysis/peakfinding/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/peakfinding/peakfinding.py` & `spectrochempy-0.6.7/spectrochempy/analysis/peakfinding/peakfinding.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,20 +10,18 @@
 Contains wrappers of `scipy.signal` peak finding functions.
 """
 
 __all__ = ["find_peaks"]
 
 __dataset_methods__ = ["find_peaks"]
 
-from datetime import datetime, timezone
-
 import numpy as np
 import scipy
 
-from spectrochempy.core.dataset.coord import Coord
+from spectrochempy.application import warning_
 from spectrochempy.core.units import Quantity
 
 # Todo:
 # find_peaks_cwt(vector, widths[, wavelet, ...]) Attempt to find the peaks in a 1-D array.
 # argrelmin(data[, axis, order, mode]) 	Calculate the relative minima of data.
 # argrelmax(data[, axis, order, mode]) 	Calculate the relative maxima of data.
 # argrelextrema(data, comparator[, axis, ...]) 	Calculate the relative extrema of data.
@@ -200,38 +198,55 @@
     <Quantity([    1644     1455], 'centimeter^-1')>
     >>> properties["peak_heights"][0]
     <Quantity(2.26663446, 'absorbance')>
     >>> properties["widths"][0]
     <Quantity(38.729003, 'centimeter^-1')>
     """
 
+    # get the dataset
     X = dataset.squeeze()
-
     if X.ndim > 1:
         raise ValueError(
             "Works only for 1D NDDataset or a 2D NDdataset with `len(X.y) <= 1`"
         )
+    # TODO: implement for 2D datasets (would be useful e.g., for NMR)
+    # be sure that data are real (NMR case for instance)
+    if X.is_complex or X.is_quaternion:
+        X = X.real
 
-    window_length = window_length if window_length % 2 == 0 else window_length - 1
-
-    # if the following parameters are entered as floats, the coordinates are used.
-    # Else, they will be treated as indices as in scipy.signal.find_peak()
-
+    # Check if we can work with the coordinates
     use_coord = use_coord and X.coordset is not None
 
-    # units
-    xunits = X.x.units if use_coord else 1
-    dunits = X.units if use_coord else 1
-
-    # assume linear x coordinates when use_coord is True!
-    # TODO: what if the coordinates are not linear?
-    spacing = X.x.spacing
-    if isinstance(spacing, Quantity):
-        spacing = spacing.magnitude
-    step = np.abs(spacing) if use_coord else 1
+    # init variable in case we do not use coordinates
+    lastcoord = None
+    xunits = 1
+    dunits = 1
+    step = 1
+
+    if use_coord:
+        # We will use the last coordinates (but if the data were transposed or sliced,
+        # the name can be something else than 'x')
+        lastcoord = X.coordset[X.dims[-1]]
+
+        # units
+        xunits = lastcoord.units if lastcoord.units is not None else 1
+        dunits = X.units if X.units is not None else 1
+
+        # assume linear x coordinates
+        # TODO: what if the coordinates are not linear?
+        if not lastcoord.linear:
+            warning_(
+                "The x coordinates are not linear. " "The peak finding might be wrong."
+            )
+            spacing = np.mean(lastcoord.spacing)
+        else:
+            spacing = lastcoord.spacing
+        if isinstance(spacing, Quantity):
+            spacing = spacing.magnitude
+        step = np.abs(spacing)
 
     # transform coord (if exists) to index
     # TODO: allow units for distance, width, wlen, plateau_size
     distance = int(round(distance / step)) if distance is not None else None
     width = int(round(width / step)) if width is not None else None
     wlen = int(round(wlen / step)) if wlen is not None else None
     plateau_size = int(round(plateau_size / step)) if plateau_size is not None else None
@@ -248,66 +263,66 @@
         rel_height=rel_height,
         plateau_size=plateau_size,
     )
 
     out = X[peaks]
 
     if not use_coord:
-        out.coordset = None
+        out.coordset = None  # remove the coordinates
 
+    # quadratic interpolation to find the maximum
+    window_length = window_length if window_length % 2 == 0 else window_length - 1
+    x_pos = []
     if window_length > 1:
-        # quadratic interpolation to find the maximum
-        x_pos = []
         for i, peak in enumerate(peaks):
-
             start = peak - window_length // 2
             end = peak + window_length // 2 + 1
             sle = slice(start, end)
 
-            Xp = X[sle]
-
-            y = Xp.data
-            x = Xp.x.data if use_coord else range(start, end)
+            y = X.data[sle]
+            x = lastcoord.data[sle] if use_coord else range(start, end)
 
             coef = np.polyfit(x, y, 2)
 
             x_at_max = -coef[1] / (2 * coef[0])
             y_at_max = np.poly1d(coef)(x_at_max)
 
             out[i] = y_at_max
-            x_pos.append(x_at_max)
+            if not use_coord:
+                x_pos.append(x_at_max)
+            else:
+                out.coordset(out.dims[-1])[i] = x_at_max
+    if x_pos and not use_coord:
+        from spectrochempy.core.dataset.coord import Coord
 
-        out.x = Coord(x_pos)
-        out.x.units = X.x.units if use_coord else None
+        out.coordset = Coord(x_pos)
 
     # transform back index to coord
     if use_coord:
-
         for key in ["peak_heights", "width_heights", "prominences"]:
             if key in properties:
                 properties[key] = [height * dunits for height in properties[key]]
 
         for key in (
             "left_bases",
             "right_bases",
             "left_edges",
             "right_edges",
         ):  # values are initially of int type
-
             if key in properties:
                 properties[key] = [
-                    X.x.values[int(index)]
+                    lastcoord.values[int(index)]
                     for index in properties[key].astype("float64")
                 ]
 
         def _prop(ips):
             # interpolate coord
             floor = int(np.floor(ips))
-            return X.x.values[floor] + (ips - floor) * (
-                X.x.values[floor + 1] - X.x.values[floor]
+            return lastcoord.values[floor] + (ips - floor) * (
+                lastcoord.values[floor + 1] - lastcoord.values[floor]
             )
 
         for key in ("left_ips", "right_ips"):  # values are float type
             if key in properties:
                 properties[key] = [_prop(ips) for ips in properties[key]]
 
         if "widths" in properties:
@@ -317,12 +332,10 @@
 
         if "plateau_sizes" in properties:
             properties["plateau_sizes"] = [
                 np.abs(sizes * step) * xunits for sizes in properties["plateau_sizes"]
             ]
 
     out.name = "peaks of " + X.name
-    out.history = (
-        f"{str(datetime.now(timezone.utc))}: find_peaks(): {len(peaks)} peak(s) found"
-    )
+    out.history = f"find_peaks(): {len(peaks)} peak(s) found"
 
     return out, properties
```

### Comparing `spectrochempy-0.6.6/spectrochempy/analysis/readme.rst` & `spectrochempy-0.6.7/spectrochempy/analysis/readme.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/api.py` & `spectrochempy-0.6.7/spectrochempy/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/application/_check_update.py` & `spectrochempy-0.6.7/spectrochempy/application/_check_update.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/application/application.py` & `spectrochempy-0.6.7/spectrochempy/application/application.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/application/datadir.py` & `spectrochempy-0.6.7/spectrochempy/application/datadir.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/application/general_preferences.py` & `spectrochempy-0.6.7/spectrochempy/application/general_preferences.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/application/plot_preferences.py` & `spectrochempy-0.6.7/spectrochempy/application/plot_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -451,15 +451,15 @@
     axes3d_grid = Bool(True, help=r"""display grid on 3d axes""").tag(
         config=True, kind=""
     )
     #
     # DATE
     #
     timezone = Unicode(
-        "UTC", help=r"""a pytz timezone string, e.g., US/Central or Europe/Paris"""
+        "UTC", help=r"""a IANA timezone string, e.g., US/Central or Europe/Paris"""
     ).tag(config=True, kind="")
     date_autoformatter_year = Unicode("%Y").tag(config=True, kind="")
     date_autoformatter_month = Unicode("%b %Y").tag(config=True, kind="")
     date_autoformatter_day = Unicode("%b %d %Y").tag(config=True, kind="")
     date_autoformatter_hour = Unicode("%H:%M:%S").tag(config=True, kind="")
     date_autoformatter_minute = Unicode("%H:%M:%S.%f").tag(config=True, kind="")
     date_autoformatter_second = Unicode("%H:%M:%S.%f").tag(config=True, kind="")
```

### Comparing `spectrochempy-0.6.6/spectrochempy/application/view.py` & `spectrochempy-0.6.7/spectrochempy/application/view.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/__init__.py` & `spectrochempy-0.6.7/spectrochempy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/common/dialogs.py` & `spectrochempy-0.6.7/spectrochempy/core/common/dialogs.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/dataset/api.py` & `spectrochempy-0.6.7/spectrochempy/core/dataset/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/dataset/arraymixins/__init__.py` & `spectrochempy-0.6.7/spectrochempy/core/dataset/arraymixins/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/dataset/arraymixins/ndio.py` & `spectrochempy-0.6.7/spectrochempy/core/dataset/arraymixins/ndio.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/dataset/arraymixins/ndmath.py` & `spectrochempy-0.6.7/spectrochempy/core/dataset/arraymixins/ndmath.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/dataset/arraymixins/ndplot.py` & `spectrochempy-0.6.7/spectrochempy/core/dataset/arraymixins/ndplot.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/dataset/baseobjects/meta.py` & `spectrochempy-0.6.7/spectrochempy/core/dataset/baseobjects/meta.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/dataset/baseobjects/ndarray.py` & `spectrochempy-0.6.7/spectrochempy/core/dataset/baseobjects/ndarray.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/dataset/baseobjects/ndcomplex.py` & `spectrochempy-0.6.7/spectrochempy/core/dataset/baseobjects/ndcomplex.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/dataset/coord.py` & `spectrochempy-0.6.7/spectrochempy/core/dataset/coord.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,14 @@
     # specific to NMR
     _larmor = tr.Instance(Quantity, allow_none=True)
 
     # ----------------------------------------------------------------------------------
     # initialization
     # ----------------------------------------------------------------------------------
     def __init__(self, data=None, **kwargs):
-
         # check if data is iterable
         if data is not None and not is_iterable(data):
             raise ValueError("Data for coordinates must be an iterable or None")
 
         # in case Coord replace old LinearCoord object
         # without changing the arguments
         _offset = kwargs.pop("offset", 0)
@@ -178,15 +177,15 @@
 
         if data is None and _size is not None and _increment is not None:
             data = np.arange(_size) * _increment + _offset
 
         # specific case of NMR (initialize unit context NMR)
         larmor = kwargs.pop("larmor", None)
 
-        self._linearize_below = kwargs.pop("linearize_below", 0.1)
+        self._linearize_below = kwargs.pop("linearize_below", 1.0)
 
         # extract parameters for linearization and data rounding
         self._sigdigits = kwargs.pop("sigdigits", 4)
 
         # if data is a Coord, rounding may have been set already
         if isinstance(data, Coord):
             self._rounding = data._rounding
@@ -253,15 +252,14 @@
         if self.has_data and len(self.shape) > 1:
             raise ValueError("Only one 1D arrays can be used to define coordinates")
 
         # linearize the data if possible or at least round it
         # to the number of significant digits
 
         if self.has_data and self.dtype.kind not in "M":
-
             # First try to linearize the data if it is not a datetime
             self._linear = False
             self.linearize(self._sigdigits)
             if self._linear:
                 return
 
     @property
@@ -649,15 +647,14 @@
     #     if self.units == "ppm":
     #         return True
     #     if self.units == "1 / centimeter" and "raman" not in self.title.lower():
     #         return True
     #     return False
 
     def _cstr(self, header="  coordinates: ... \n", print_size=True, **kwargs):
-
         indent = kwargs.get("indent", 0)
 
         out = ""
         if not self.is_empty and print_size:
             out += f"{self._str_shape().rstrip()}\n"
         out += f"        title: {self.title}\n" if self.title else ""
         if self.has_data:
@@ -765,15 +762,14 @@
         # private property
         # True if timescale must be used for interferogram axis. Else it
         # will be set to optical path difference.
         return self._use_time
 
     @_use_time_axis.setter
     def _use_time_axis(self, val):
-
         self._use_time = val
         if "laser_frequency" in self.meta:
             self.set_laser_frequency(self.meta.laser_frequency)
 
     @property
     def show_datapoints(self):
         """
@@ -785,15 +781,14 @@
         ]:
             return False
 
         return self._show_datapoints
 
     @show_datapoints.setter
     def show_datapoints(self, val):
-
         self._show_datapoints = val
 
     @property
     def larmor(self):
         """
         Return larmor frequency in NMR spectroscopy context.
         """
```

### Comparing `spectrochempy-0.6.6/spectrochempy/core/dataset/coordset.py` & `spectrochempy-0.6.7/spectrochempy/core/dataset/coordset.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,14 @@
     # default coord index
     _default = Int(0)
 
     # ----------------------------------------------------------------------------------
     # initialization
     # ----------------------------------------------------------------------------------
     def __init__(self, *coords, **kwargs):
-
         self._copy = kwargs.pop("copy", True)
         self._sorted = kwargs.pop("sorted", True)
 
         keepnames = kwargs.pop("keepnames", False)
         # if keepnames is false and the names of the dimensions are not passed in kwargs, then use dims if not none
         dims = kwargs.pop("dims", None)
 
@@ -141,15 +140,14 @@
         # initialise the coordinate list
         self._coords = []
 
         # First evaluate passed args
         # --------------------------
         # some cleaning
         if coords:
-
             if all(
                 [
                     (
                         isinstance(coords[i], (np.ndarray, NDArray, list, CoordSet))
                         or coords[i] is None
                     )
                     for i in range(len(coords))
@@ -770,26 +768,24 @@
             try:
                 return self.__delitem__(item)
             except (IndexError, KeyError):
                 raise AttributeError
 
     def __getattr__(self, item):
         # when the attribute was not found
-        if "_validate" in item or "_changed" in item:
+        if "_validate" in item or "_changed" in item or item in ["strip", "__iter__"]:
             raise AttributeError
 
         try:
             return self.__getitem__(item)
         except (IndexError, KeyError):
             raise AttributeError
 
     def __getitem__(self, index):
-
         if isinstance(index, str):
-
             # find by name
             if index in self.names:
                 idx = self.names.index(index)
                 return self._coords.__getitem__(idx)
 
             # ok we did not find it!
             # let's try in references
@@ -958,17 +954,15 @@
                 raise KeyError(
                     f"Could not find `{index}` in coordinates names or titles"
                 )
 
         self._coords[index] = coord
 
     def __delitem__(self, index):
-
         if isinstance(index, str):
-
             # find by name
             if index in self.names:
                 idx = self.names.index(index)
                 del self._coords[idx]
                 return
 
             # let's try in the title
@@ -1009,21 +1003,19 @@
         out = out.format(*s)
         return out
 
     def __str__(self):
         return repr(self)
 
     def _cstr(self, header="  coordinates: ... \n", print_size=True):
-
         txt = ""
         for idx, dim in enumerate(self.names):
             coord = getattr(self, dim)
 
             if coord:
-
                 dimension = f"     DIMENSION `{dim}`"
                 for k, v in self.references.items():
                     if dim == v:
                         # reference to this dimension
                         dimension += f"=`{k}`"
                 txt += dimension + "\n"
```

### Comparing `spectrochempy-0.6.6/spectrochempy/core/dataset/nddataset.py` & `spectrochempy-0.6.7/spectrochempy/core/dataset/nddataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,36 +9,36 @@
 """
 
 __all__ = ["NDDataset"]
 # import signal
 import sys
 import textwrap
 from datetime import datetime, tzinfo
+from zoneinfo import ZoneInfo, ZoneInfoNotFoundError
 
 import numpy as np
-import pytz  # TODO: for py>=3.9, we could use builtin zoneinfo library instead of pyt
 import traitlets as tr
+from tzlocal import get_localzone
 
 from spectrochempy.application import error_, warning_
 from spectrochempy.core.dataset.arraymixins.ndio import NDIO
 from spectrochempy.core.dataset.arraymixins.ndmath import NDMath  # _set_ufuncs,
 from spectrochempy.core.dataset.arraymixins.ndmath import _set_operators
 from spectrochempy.core.dataset.arraymixins.ndplot import NDPlot
 from spectrochempy.core.dataset.baseobjects.ndarray import DEFAULT_DIM_NAME, NDArray
 from spectrochempy.core.dataset.baseobjects.ndcomplex import NDComplexArray
 from spectrochempy.core.dataset.coord import Coord
 from spectrochempy.core.dataset.coordset import CoordSet
 from spectrochempy.extern.traittypes import Array
-from spectrochempy.utils.exceptions import SpectroChemPyError, UnknownTimeZoneError
+from spectrochempy.utils.datetimeutils import utcnow
+from spectrochempy.utils.exceptions import SpectroChemPyError
 from spectrochempy.utils.optional import import_optional_dependency
 from spectrochempy.utils.print import colored_output
 from spectrochempy.utils.system import get_user_and_node
 
-#       but we need compatibility with 3.7 (Colab).
-
 
 # ======================================================================================
 # NDDataset class definition
 # ======================================================================================
 @tr.signature_has_traits
 class NDDataset(NDMath, NDIO, NDPlot, NDComplexArray):
     r"""
@@ -222,15 +222,15 @@
     # Initialisation
     # ----------------------------------------------------------------------------------
     def __init__(
         self, data=None, coordset=None, coordunits=None, coordtitles=None, **kwargs
     ):
         super().__init__(data, **kwargs)
 
-        self._created = datetime.utcnow()
+        self._created = utcnow()
         self.description = kwargs.pop("description", "")
         self.author = kwargs.pop("author", get_user_and_node())
 
         history = kwargs.pop("history", None)
         if history is not None:
             self.history = history
 
@@ -343,15 +343,15 @@
             for i, item in enumerate(items):
                 # get the corresponding dimension name in the dims list
                 name = self.dims[i]
                 # get the corresponding index in the coordinate's names list
                 idx = names.index(name)
                 if self._coordset[idx].is_empty:
                     new_coords[idx] = Coord(None, name=name)
-                elif isinstance(item, slice):
+                else:  # if isinstance(item, slice):
                     # add the slice on the corresponding coordinates on the dim to the
                     # new list of coordinates
                     if not isinstance(self._coordset[idx], CoordSet):
                         new_coords[idx] = self._coordset[idx][item]
                     else:
                         # we must slice all internal coordinates
                         newc = []
@@ -361,16 +361,16 @@
                         # we reverse to be sure
                         # the order will be  kept for internal coordinates
                         new_coords[idx]._default = self._coordset[
                             idx
                         ]._default  # set the same default coord
                         new_coords[idx]._is_same_dim = self._coordset[idx]._is_same_dim
 
-                elif isinstance(item, (np.ndarray, list)):
-                    new_coords[idx] = self._coordset[idx][item]
+                # elif isinstance(item, (np.ndarray, list)):
+                #    new_coords[idx] = self._coordset[idx][item]
 
             new.set_coordset(*new_coords, keepnames=True)
 
         new.history = f"Slice extracted: ({saveditems})"
         return new
 
     def __getattr__(self, item):
@@ -537,40 +537,40 @@
     #     ranges = Meta()
     #     for dim in self.dims:
     #         ranges[dim] = dict(masks={}, baselines={}, integrals={}, others={})
     #     return ranges
 
     @tr.default("_timezone")
     def _timezone_default(self):
-        # Return the default timezone (UTC)
-        return datetime.utcnow().astimezone().tzinfo
+        # Return the default timezone (local timezone)
+        return get_localzone()
 
-    @tr.validate("_created")
-    def _created_validate(self, proposal):
-        date = proposal["value"]
-        if date.tzinfo is not None:
-            # make the date utc naive
-            date = date.replace(tzinfo=None)
-        return date
+    # @tr.validate("_created")
+    # def _created_validate(self, proposal):
+    #     date = proposal["value"]
+    #     if date.tzinfo is not None:
+    #         # make the date utc naive
+    #         date = date.replace(tzinfo=None)
+    #     return date
 
     @tr.validate("_history")
     def _history_validate(self, proposal):
         history = proposal["value"]
         if isinstance(history, list) or history is None:
             # reset
             self._history = None
         return history
 
-    @tr.validate("_modified")
-    def _modified_validate(self, proposal):
-        date = proposal["value"]
-        if date.tzinfo is not None:
-            # make the date utc naive
-            date = date.replace(tzinfo=None)
-        return date
+    # @tr.validate("_modified")
+    # def _modified_validate(self, proposal):
+    #     date = proposal["value"]
+    #     if date.tzinfo is not None:
+    #         # make the date utc naive
+    #         date = date.replace(tzinfo=None)
+    #     return date
 
     @tr.observe(tr.All)
     def _anytrait_changed(self, change):
         # ex: change {
         #   'owner': object, # The HasTraits instance
         #   'new': 6, # The new value
         #   'old': 5, # The old value
@@ -578,15 +578,15 @@
         #   'type': 'change', # The event type of the notification, usually 'change'
         # }
 
         if change["name"] in ["_created", "_modified", "trait_added"]:
             return
 
         # all the time -> update modified date
-        self._modified = datetime.utcnow()
+        self._modified = utcnow()
         return
 
     def _cstr(self):
         # Display the metadata of the object and partially the data
         out = ""
         out += "         name: {}\n".format(self.name)
         out += "       author: {}\n".format(self.author)
@@ -816,16 +816,17 @@
     def history(self):
         """
         Describes the history of actions made on this array (List of strings).
         """
 
         history = []
         for date, value in self._history:
-            date = pytz.utc.localize(date)
-            date = date.astimezone(self.timezone).isoformat(sep=" ", timespec="seconds")
+            date = date.astimezone(self._timezone).isoformat(
+                sep=" ", timespec="seconds"
+            )
             value = value[0].capitalize() + value[1:]
             history.append(f"{date}> {value}")
         return history
 
     @history.setter
     def history(self, value):
         if value is None:
@@ -923,16 +924,16 @@
             return self._coordset.units
 
     @property
     def created(self):
         """
         Creation date object (Datetime).
         """
-        created = pytz.utc.localize(self._created)
-        return created.astimezone(self.timezone).isoformat(sep=" ", timespec="seconds")
+        created = self._created.astimezone(self._timezone)
+        return created.isoformat(sep=" ", timespec="seconds")
 
     @property
     def data(self):
         """
         The `data` array.
 
         If there is no data but labels, then the labels are returned instead of data.
@@ -968,15 +969,15 @@
         self._description = value
 
     @property
     def local_timezone(self):
         """
         Return the local timezone.
         """
-        return str(datetime.utcnow().astimezone().tzinfo)
+        return str(get_localzone())
 
     @property
     def modeldata(self):
         """
         `~numpy.ndarray` - models data.
 
         Data eventually generated by modelling of the data.
@@ -988,16 +989,16 @@
         self._modeldata = data
 
     @property
     def modified(self):
         """
         Date of modification (readonly property).
         """
-        modified = pytz.utc.localize(self._modified)
-        return modified.astimezone(self.timezone).isoformat(sep=" ", timespec="seconds")
+        modified = self._modified.astimezone(self._timezone)
+        return modified.isoformat(sep=" ", timespec="seconds")
 
     @property
     def origin(self):
         """
         Origin of the data.
 
         e.g. spectrometer or software
@@ -1275,35 +1276,28 @@
     def timezone(self):
         """
         Return the timezone information.
 
         A timezone's offset refers to how many hours the timezone
         is from Coordinated Universal Time (UTC).
 
-        A `naive` datetime object contains no timezone information. The
-        easiest way to tell if a datetime object is naive is by checking
-        tzinfo.  will be set to None of the object is naive.
-
-        A naive datetime object is limited in that it cannot locate itself
-        in relation to offset-aware datetime objects.
-
         In spectrochempy, all datetimes are stored in UTC, so that conversion
         must be done during the display of these datetimes using tzinfo.
         """
-        return self._timezone
+        return str(self._timezone)
 
     @timezone.setter
     def timezone(self, val):
         try:
-            self._timezone = pytz.timezone(val)
-        except pytz.UnknownTimeZoneError:
-            raise UnknownTimeZoneError(
+            self._timezone = ZoneInfo(val)
+        except ZoneInfoNotFoundError as e:
+            raise ZoneInfoNotFoundError(
                 "You can get a list of valid timezones in "
                 "https://en.wikipedia.org/wiki/tr.List_of_tz_database_time_zones ",
-            )
+            ) from e
 
     def to_array(self):
         """
         Return a numpy masked array.
 
         Other NDDataset attributes are lost.
```

### Comparing `spectrochempy-0.6.6/spectrochempy/core/plotters/multiplot.py` & `spectrochempy-0.6.7/spectrochempy/core/plotters/multiplot.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/plotters/plot1d.py` & `spectrochempy-0.6.7/spectrochempy/core/plotters/plot1d.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/plotters/plot2d.py` & `spectrochempy-0.6.7/spectrochempy/core/plotters/plot2d.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/plotters/plot3d.py` & `spectrochempy-0.6.7/spectrochempy/core/plotters/plot3d.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/plotters/plotly.py` & `spectrochempy-0.6.7/spectrochempy/core/plotters/plotly.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/project/abstractproject.py` & `spectrochempy-0.6.7/spectrochempy/core/project/abstractproject.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/project/project.py` & `spectrochempy-0.6.7/spectrochempy/core/project/project.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/readers/download.py` & `spectrochempy-0.6.7/spectrochempy/core/readers/download.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/readers/importer.py` & `spectrochempy-0.6.7/spectrochempy/core/readers/importer.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,16 @@
     ("dso", "Data Set Object files (*.dso)"),
     ("jcamp", "JCAMP-DX files (*.jdx *.dx)"),
     ("csv", "CSV files (*.csv)"),
     ("excel", "Microsoft Excel files (*.xls)"),
     ("zip", "Compressed folder of data files (*.zip)"),
     ("quadera", "Quadera ascii files (*.asc)"),
     ("carroucell", "Carroucell files (*spa)"),
-    ("galactic", "GRAMS/Thermo Galactic files (*.spc)")
+    ("galactic", "GRAMS/Thermo Galactic files (*.spc)"),
+    ("wire", "Renishaw WiRE files (*.wdf)"),
     #  ('all', 'All files (*.*)')
 ]
 ALIAS = [
     ("spg", "omnic"),
     ("spa", "omnic"),
     ("ddr", "soc"),
     ("hdr", "soc"),
@@ -61,14 +62,15 @@
     ("srs", "omnic"),
     ("mat", "matlab"),
     ("txt", "labspec"),
     ("jdx", "jcamp"),
     ("dx", "jcamp"),
     ("xls", "excel"),
     ("asc", "quadera"),
+    ("wdf", "wire"),
 ]
 
 
 # --------------------------------------------------------------------------------------
 class Importer(HasTraits):
     # Private Importer class
 
@@ -307,14 +309,15 @@
 read_galactic : Read Galactic files (:file:`.spc`\ ).
 read_quadera : Read a Pfeiffer Vacuum's QUADERA mass spectrometer software file.
 read_topspin : Read TopSpin Bruker NMR spectra.
 read_csv : Read CSV files (:file:`.csv`\ ).
 read_jcamp : Read Infrared JCAMP-DX files (:file:`.jdx`\ , :file:`.dx`\ ).
 read_matlab : Read Matlab files (:file:`.mat`\ , :file:`.dso`\ ).
 read_carroucell : Read files in a directory after a carroucell experiment.
+read_wire : Read REnishaw Wire files (:file:`.wdf`\ ).
 """,
     sections=["See Also"],
     base="Importer",
 )
 
 _docstring.delete_params("Importer.see_also", "read")
 
@@ -682,15 +685,15 @@
     # Check if Content has been passed?
     content = kwargs.get("content", False)
 
     # default encoding
     encoding = "utf-8"
 
     if _is_url(filename):
-        # by default we set the read_only flag to True when reading remote url
+        # by default, we set the read_only flag to True when reading remote url
         kwargs["read_only"] = kwargs.get("read_only", True)
 
         # use request to read the remote content
         r = requests.get(filename, allow_redirects=True)
         r.raise_for_status()
         content = r.content
         encoding = r.encoding
```

### Comparing `spectrochempy-0.6.6/spectrochempy/core/readers/read_carroucell.py` & `spectrochempy-0.6.7/spectrochempy/core/readers/read_carroucell.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/readers/read_csv.py` & `spectrochempy-0.6.7/spectrochempy/core/readers/read_csv.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/readers/read_jcamp.py` & `spectrochempy-0.6.7/spectrochempy/core/readers/read_jcamp.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/readers/read_labspec.py` & `spectrochempy-0.6.7/spectrochempy/core/readers/read_labspec.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     See Also
     ---------
     %(Importer.see_also.no_read_labspec)s
 
     Examples
     --------
-    >>> A = scp.read_labspec('ramandata/Activation.txt')
+    >>> A = scp.read_labspec('ramandata/labspec/Activation.txt')
     """
 
     kwargs["filetypes"] = ["LABSPEC exported files (*.txt)"]
     kwargs["protocol"] = ["labspec", "txt"]
     importer = Importer()
     return importer(*paths, **kwargs)
```

### Comparing `spectrochempy-0.6.6/spectrochempy/core/readers/read_matlab.py` & `spectrochempy-0.6.7/spectrochempy/core/readers/read_matlab.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/readers/read_omnic.py` & `spectrochempy-0.6.7/spectrochempy/core/readers/read_omnic.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 files.
 """
 __all__ = ["read_omnic", "read_spg", "read_spa", "read_srs"]
 __dataset_methods__ = __all__
 
 import io
 import re
-import struct
 from datetime import datetime, timedelta, timezone
 
 import numpy as np
 
 from spectrochempy.application import info_
 from spectrochempy.core.dataset.coord import Coord
 from spectrochempy.core.dataset.nddataset import NDDataset
 from spectrochempy.core.readers.importer import Importer, _importer_method, _openfid
 from spectrochempy.core.units import ur
 from spectrochempy.utils.docstrings import _docstring
+from spectrochempy.utils.file import fromfile
 
 # ======================================================================================
 # Public functions
 # ======================================================================================
 _docstring.delete_params("Importer.see_also", "read_omnic")
 
 
@@ -332,22 +332,22 @@
     #
     # the number of line per block may change from file to file but the total
     # number of lines is given at hex 294, hence allowing counting the
     # number of spectra:
 
     # read total number of lines
     fid.seek(294)
-    nlines = _fromfile(fid, "uint16", count=1)
+    nlines = fromfile(fid, "uint16", count=1)
 
     # read "key values"
     pos = 304
     keys = np.zeros(nlines)
     for i in range(nlines):
         fid.seek(pos)
-        keys[i] = _fromfile(fid, dtype="uint8", count=1)
+        keys[i] = fromfile(fid, dtype="uint8", count=1)
         pos += 16
 
     # the number of occurrences of the key '02' is number of spectra
     nspec = np.count_nonzero((keys == 2))
 
     if nspec == 0:  # pragma: no cover
         raise IOError(
@@ -371,15 +371,15 @@
     position02 = (
         304 * np.ones(len(indices02[0]), dtype="int") + 16 * indices02[0]
     )  # ex: [304 432 ...]
 
     for i in range(nspec):
         # read the position of the header
         fid.seek(position02[i] + 2)
-        pos_header = _fromfile(fid, dtype="uint32", count=1)
+        pos_header = fromfile(fid, dtype="uint32", count=1)
         # get infos
         info = _read_header(fid, pos_header)
         nx[i] = info["nx"]
         firstx[i] = info["firstx"]
         lastx[i] = info["lastx"]
         xunits.append(info["xunits"])
         xtitles.append(info["xtitle"])
@@ -431,23 +431,23 @@
     indices6B = np.nonzero(key_is_6B)
     position6B = 304 * np.ones(len(indices6B[0]), dtype="int") + 16 * indices6B[0]
 
     # Read spectra titles and acquisition date
     for i in range(nspec):
         # determines the position of informatioon
         fid.seek(position6B[i] + 2)  # go to line and skip 2 bytes
-        spa_title_pos = _fromfile(fid, "uint32", 1)
+        spa_title_pos = fromfile(fid, "uint32", 1)
 
         # read omnic filename
         spa_title = _readbtext(fid, spa_title_pos, 256)
         spectitles.append(spa_title)
 
         # and the acquisition date
         fid.seek(spa_title_pos + 256)
-        timestamp = _fromfile(fid, dtype="uint32", count=1)
+        timestamp = fromfile(fid, dtype="uint32", count=1)
         # since 31/12/1899, 00:00
         acqdate = datetime(1899, 12, 31, 0, 0, tzinfo=timezone.utc) + timedelta(
             seconds=int(timestamp)
         )
         acquisitiondates.append(acqdate)
         timestamp = acqdate.timestamp()
         # Transform back to timestamp for storage in the Coord object
@@ -462,15 +462,15 @@
         # e.g. peakresolve)
         #  key_is_1B = (keys == 27)
         #  indices1B =  # np.nonzero(key_is_1B)
         #  position1B = 304 * np.ones(len(indices1B[0]), dtype='int') + 16 * indices6B[0]
         #  if len(position1B) != 0:  # read history texts
         #     for j in range(nspec):  determine the position of information
         #        f.seek(position1B[j] + 2)  #
-        #        history_pos = _fromfile(f,  'uint32', 1)
+        #        history_pos = fromfile(f,  'uint32', 1)
         #        history =  _readbtext(f, history_pos[0])
         #        allhistories.append(history)
 
     fid.close()
 
     # Create Dataset Object of spectral content
     dataset.data = data
@@ -530,15 +530,15 @@
     # been saved: it won't match with the actual filename if a subsequent
     # renaming has been done in the OS.
     spa_name = _readbtext(fid, 30, 256)
 
     # The acquisition date (GMT) is at hex 128 = decimal 296.
     # Second since 31/12/1899, 00:00
     fid.seek(296)
-    timestamp = _fromfile(fid, dtype="uint32", count=1)
+    timestamp = fromfile(fid, dtype="uint32", count=1)
     acqdate = datetime(1899, 12, 31, 0, 0, tzinfo=timezone.utc) + timedelta(
         seconds=int(timestamp)
     )
     acquisitiondate = acqdate
 
     # Transform back to timestamp for storage in the Coord object
     # use datetime.fromtimestamp(d, timezone.utc)) to transform back to datetime object
@@ -575,40 +575,40 @@
     # (before the '1B').
 
     # scan "key values"
     pos = 304
     spa_comments = []  # several custom comments can be present
     while "continue":
         fid.seek(pos)
-        key = _fromfile(fid, dtype="uint8", count=1)
+        key = fromfile(fid, dtype="uint8", count=1)
 
         # print(key, end=' ; ')
 
         if key == 2:
             # read the position of the header
             fid.seek(pos + 2)
-            pos_header = _fromfile(fid, dtype="uint32", count=1)
+            pos_header = fromfile(fid, dtype="uint32", count=1)
             info = _read_header(fid, pos_header)
 
         elif key == 3 and return_ifg is None:
             intensities = _getintensities(fid, pos)
 
         elif key == 4:
             fid.seek(pos + 2)
-            comments_pos = _fromfile(fid, "uint32", 1)
+            comments_pos = fromfile(fid, "uint32", 1)
             fid.seek(pos + 6)
-            comments_len = _fromfile(fid, "uint32", 1)
+            comments_len = fromfile(fid, "uint32", 1)
             fid.seek(comments_pos)
             spa_comments.append(fid.read(comments_len).decode("latin-1", "replace"))
 
         elif key == 27:
             fid.seek(pos + 2)
-            history_pos = _fromfile(fid, "uint32", 1)
+            history_pos = fromfile(fid, "uint32", 1)
             fid.seek(pos + 6)
-            history_len = _fromfile(fid, "uint32", 1)
+            history_len = fromfile(fid, "uint32", 1)
             spa_history = _readbtext(fid, history_pos, history_len)
 
         elif key == 102 and return_ifg == "sample":
             s_ifg_intensities = _getintensities(fid, pos)
 
         elif key == 103 and return_ifg == "background":
             b_ifg_intensities = _getintensities(fid, pos)
@@ -737,15 +737,15 @@
         fid = io.BytesIO(filename)  # pragma: no cover
     else:
         fid = open(filename, "rb")
 
     # determine whether the srs is reprocessed. At pos=292 (hex:124) appears a difference between
     # and reprocessed series
     fid.seek(292)
-    key = _fromfile(fid, dtype="uint8", count=16)[0]
+    key = fromfile(fid, dtype="uint8", count=16)[0]
     if key == 39:  # (hex: 27)
         is_reprocessed = False
     elif key == 15:  # (hex = 0F)
         is_reprocessed = True
     # if key == 72 (hex:48), could be TGA
 
     """ At pos=304 (hex:130) is the position of the '02' key for series. Herte we don't use it.
@@ -788,23 +788,23 @@
 
         # now read the spectra/interferogram names and data
         # the first one....
         pos = index[2]
         names.append(_readbtext(fid, pos, 256))
         pos += 84
         fid.seek(pos)
-        data[0, :] = _fromfile(fid, dtype="float32", count=info["nx"])[:]
+        data[0, :] = fromfile(fid, dtype="float32", count=info["nx"])[:]
         pos += info["nx"] * 4
         # ... and the remaining ones:
         for i in np.arange(info["ny"])[1:]:
             pos += 16
             names.append(_readbtext(fid, pos, 256))
             pos += 84
             fid.seek(pos)
-            data[i, :] = _fromfile(fid, dtype="float32", count=info["nx"])[:]
+            data[i, :] = fromfile(fid, dtype="float32", count=info["nx"])[:]
             pos += info["nx"] * 4
 
         # now get series history
         if not is_reprocessed:
             history = info["history"]
         else:
             # In reprocessed series the updated "DATA PROCESSING HISTORY" is located right after
@@ -818,15 +818,15 @@
 
         # First get background info
         info = _read_header(fid, index[1])
 
         if "background_name" not in info.keys():
             # it is a short header
             fid.seek(index[1] + 208)
-            data = _fromfile(fid, dtype="float32", count=info["nx"])
+            data = fromfile(fid, dtype="float32", count=info["nx"])
         else:
             # longer header, in such case the header indicates a spectrum
             # but the data are those of an ifg... For now need more examples
             return None
 
     # Create NDDataset Object for the series
     if not return_bg:
@@ -896,19 +896,19 @@
         # its function is not known. related to Grams-schmidt ?
 
         # pos = _nextline(pos)
         # found = False
         # while not found:
         #     pos += 16
         #     f.seek(pos)
-        #     key = _fromfile(f, dtype='uint8', count=1)
+        #     key = fromfile(f, dtype='uint8', count=1)
         #     if key == 1:
         #         pos += 4
         #         f.seek(pos)
-        #         X = _fromfile(f, dtype='float32', count=info['ny'])
+        #         X = fromfile(f, dtype='float32', count=info['ny'])
         #         found = True
         #
         # X = NDDataset(X)
         # _x = Coord(np.around(np.linspace(0, info['ny']-1, info['ny']), 0),
         #            title='time',
         #            units='minutes')
         # X.set_coordset(x=_x)
@@ -918,39 +918,14 @@
         # X.history = str(datetime.now(timezone.utc)) + ':imported from srs
 
     fid.close()
 
     return dataset
 
 
-def _fromfile(fid, dtype, count):
-    # to replace np.fromfile in case of io.BytesIO object instead of byte
-    # object
-    t = {
-        "uint8": "B",
-        "int8": "b",
-        "uint16": "H",
-        "int16": "h",
-        "uint32": "I",
-        "int32": "i",
-        "float32": "f",
-        "char8": "c",
-    }
-    typ = t[dtype] * count
-    if dtype.endswith("16"):
-        count *= 2
-    elif dtype.endswith("32"):
-        count *= 4
-
-    out = struct.unpack(typ, fid.read(count))
-    if len(out) == 1:
-        return out[0]
-    return np.array(out)
-
-
 def _readbtext(fid, pos, size):
     # Read some text in binary file of given size. If size is None, the etxt is read
     # until b\0\ is encountered.
     # Returns utf-8 string
     fid.seek(pos)
     if size is None:
         btext = b""
@@ -1060,19 +1035,19 @@
     if bytes == b"Spectral Data File":
         filetype = "spa, spg"
     elif bytes == b"Spectral Exte File":
         filetype = "srs"
 
     # nx
     fid.seek(pos + 4)
-    out["nx"] = _fromfile(fid, "uint32", count=1)
+    out["nx"] = fromfile(fid, "uint32", count=1)
 
     # xunits
     fid.seek(pos + 8)
-    key = _fromfile(fid, dtype="uint8", count=1)
+    key = fromfile(fid, dtype="uint8", count=1)
     if key == 1:
         out["xunits"] = "cm^-1"
         out["xtitle"] = "wavenumbers"
     elif key == 2:
         out["xunits"] = None
         out["xtitle"] = "data points"
     elif key == 3:  # pragma: no cover
@@ -1087,15 +1062,15 @@
     else:  # pragma: no cover
         out["xunits"] = None
         out["xtitle"] = "xaxis"
         info_("The nature of x data is not recognized, xtitle is set to 'xaxis'")
 
     # data units
     fid.seek(pos + 12)
-    key = _fromfile(fid, dtype="uint8", count=1)
+    key = fromfile(fid, dtype="uint8", count=1)
     if key == 17:
         out["units"] = "absorbance"
         out["title"] = "absorbance"
     elif key == 16:  # pragma: no cover
         out["units"] = "percent"
         out["title"] = "transmittance"
     elif key == 11:  # pragma: no cover
@@ -1122,51 +1097,51 @@
     else:  # pragma: no cover
         out["units"] = None
         out["title"] = "intensity"
         info_("The nature of data is not recognized, title set to 'Intensity'")
 
     # firstx, lastx
     fid.seek(pos + 16)
-    out["firstx"] = _fromfile(fid, "float32", 1)
+    out["firstx"] = fromfile(fid, "float32", 1)
     fid.seek(pos + 20)
-    out["lastx"] = _fromfile(fid, "float32", 1)
+    out["lastx"] = fromfile(fid, "float32", 1)
     fid.seek(pos + 28)
 
-    out["scan_pts"] = _fromfile(fid, "uint32", 1)
+    out["scan_pts"] = fromfile(fid, "uint32", 1)
     fid.seek(pos + 32)
-    out["zpd"] = _fromfile(fid, "uint32", 1)
+    out["zpd"] = fromfile(fid, "uint32", 1)
     fid.seek(pos + 36)
-    out["nscan"] = _fromfile(fid, "uint32", 1)
+    out["nscan"] = fromfile(fid, "uint32", 1)
     fid.seek(pos + 52)
-    out["nbkgscan"] = _fromfile(fid, "uint32", 1)
+    out["nbkgscan"] = fromfile(fid, "uint32", 1)
     fid.seek(pos + 68)
-    out["collection_length"] = _fromfile(fid, "uint32", 1)
+    out["collection_length"] = fromfile(fid, "uint32", 1)
     fid.seek(pos + 80)
-    out["reference_frequency"] = _fromfile(fid, "float32", 1)
+    out["reference_frequency"] = fromfile(fid, "float32", 1)
     fid.seek(pos + 188)
-    out["optical_velocity"] = _fromfile(fid, "float32", 1)
+    out["optical_velocity"] = fromfile(fid, "float32", 1)
 
     if filetype == "spa, spg":
         out["history"] = _readbtext(fid, pos + 208, None)
 
     if filetype == "srs":
         if out["nbkgscan"] == 0:
             # an interferogram in rapid scan mode
             if out["firstx"] > out["lastx"]:
                 out["firstx"], out["lastx"] = out["lastx"], out["firstx"]
 
         out["name"] = _readbtext(fid, pos + 938, 256)
         fid.seek(pos + 1002)
-        out["collection_length"] = _fromfile(fid, "float32", 1) * 60
+        out["collection_length"] = fromfile(fid, "float32", 1) * 60
         fid.seek(pos + 1006)
-        out["lasty"] = _fromfile(fid, "float32", 1)
+        out["lasty"] = fromfile(fid, "float32", 1)
         fid.seek(pos + 1010)
-        out["firsty"] = _fromfile(fid, "float32", 1)
+        out["firsty"] = fromfile(fid, "float32", 1)
         fid.seek(pos + 1026)
-        out["ny"] = _fromfile(fid, "uint32", 1)
+        out["ny"] = fromfile(fid, "uint32", 1)
         #  y unit could be at pos+1030 with 01 = minutes ?
         out["history"] = _readbtext(fid, pos + 1200, None)
 
         if _readbtext(fid, pos + 208, 256)[:10] == "Background":
             # it is the header of a background
             out["background_name"] = _readbtext(fid, pos + 208, 256)[10:]
 
@@ -1175,15 +1150,15 @@
 
 def _getintensities(fid, pos):
     # get intensities from the 03 (spectrum)
     # or 66 (sample ifg) or 67 (bg ifg) key,
     # returns a ndarray
 
     fid.seek(pos + 2)  # skip 2 bytes
-    intensity_pos = _fromfile(fid, "uint32", 1)
+    intensity_pos = fromfile(fid, "uint32", 1)
     fid.seek(pos + 6)
-    intensity_size = _fromfile(fid, "uint32", 1)
+    intensity_size = fromfile(fid, "uint32", 1)
     nintensities = int(intensity_size / 4)
 
     # Read and return spectral intensities
     fid.seek(intensity_pos)
-    return _fromfile(fid, "float32", int(nintensities))
+    return fromfile(fid, "float32", int(nintensities))
```

### Comparing `spectrochempy-0.6.6/spectrochempy/core/readers/read_opus.py` & `spectrochempy-0.6.7/spectrochempy/core/readers/read_opus.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/readers/read_quadera.py` & `spectrochempy-0.6.7/spectrochempy/core/readers/read_quadera.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/readers/read_soc.py` & `spectrochempy-0.6.7/spectrochempy/core/readers/read_soc.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/readers/read_spc.py` & `spectrochempy-0.6.7/spectrochempy/core/readers/read_spc.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/readers/read_topspin.py` & `spectrochempy-0.6.7/spectrochempy/core/readers/read_topspin.py`

 * *Files 0% similar despite different names*

```diff
@@ -844,15 +844,15 @@
                 data = data + dataI * 1.0j
 
             else:
                 return None
         else:
             data = datalist
 
-    # we now make some rearrangement of the dic to have something more user friendly
+    # we now make some rearrangement of the dic to have something more user-friendly
     # we assume that all experiments have similar (important) parameters so that the experiments are compatibles
 
     meta = Meta()  # This is the parameter dictionary
     datatype = path.name.upper() if not processed else f"{data.ndim}D"
 
     keys = sorted(dic.keys())
```

### Comparing `spectrochempy-0.6.6/spectrochempy/core/readers/read_zip.py` & `spectrochempy-0.6.7/spectrochempy/core/readers/read_zip.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/script/__init__.py` & `spectrochempy-0.6.7/spectrochempy/core/script/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/units/__init__.py` & `spectrochempy-0.6.7/spectrochempy/core/units/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/writers/exporter.py` & `spectrochempy-0.6.7/spectrochempy/core/writers/exporter.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/writers/write_csv.py` & `spectrochempy-0.6.7/spectrochempy/core/writers/write_csv.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/writers/write_excel.py` & `spectrochempy-0.6.7/spectrochempy/core/writers/write_excel.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/writers/write_jcamp.py` & `spectrochempy-0.6.7/spectrochempy/core/writers/write_jcamp.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/core/writers/write_matlab.py` & `spectrochempy-0.6.7/spectrochempy/core/writers/write_matlab.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_efa.py` & `spectrochempy-0.6.7/spectrochempy/examples/analysis/a_decomposition/plot_efa.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_efa_keller_massart.py` & `spectrochempy-0.6.7/spectrochempy/examples/analysis/a_decomposition/plot_efa_keller_massart.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_fast_ica.py` & `spectrochempy-0.6.7/spectrochempy/examples/analysis/a_decomposition/plot_fast_ica.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_iris.py` & `spectrochempy-0.6.7/spectrochempy/examples/analysis/a_decomposition/plot_iris.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_mcrals_chrom1.py` & `spectrochempy-0.6.7/spectrochempy/examples/analysis/a_decomposition/plot_mcrals_chrom1.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_mcrals_kinetics.py` & `spectrochempy-0.6.7/spectrochempy/examples/analysis/a_decomposition/plot_mcrals_kinetics.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_nmf.py` & `spectrochempy-0.6.7/spectrochempy/examples/analysis/a_decomposition/plot_nmf.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_pca_iris.py` & `spectrochempy-0.6.7/spectrochempy/examples/analysis/a_decomposition/plot_pca_iris.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_pca_spec.py` & `spectrochempy-0.6.7/spectrochempy/examples/analysis/a_decomposition/plot_pca_spec.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_simplisma.py` & `spectrochempy-0.6.7/spectrochempy/examples/analysis/a_decomposition/plot_simplisma.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/analysis/b_crossdecomposition/plot_pls.py` & `spectrochempy-0.6.7/spectrochempy/examples/analysis/b_crossdecomposition/plot_pls.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/analysis/c_curvefitting/plot_fit.py` & `spectrochempy-0.6.7/spectrochempy/examples/analysis/c_curvefitting/plot_fit.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/analysis/c_curvefitting/plot_lstsq_single_equation.py` & `spectrochempy-0.6.7/spectrochempy/examples/analysis/c_curvefitting/plot_lstsq_single_equation.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/analysis/d_baseline/plot_baseline_correction.py` & `spectrochempy-0.6.7/spectrochempy/examples/analysis/d_baseline/plot_baseline_correction.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/core/a_nddataset/plot_a_create_dataset.py` & `spectrochempy-0.6.7/spectrochempy/examples/core/a_nddataset/plot_a_create_dataset.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/core/a_nddataset/plot_b_coordinates.py` & `spectrochempy-0.6.7/spectrochempy/examples/core/a_nddataset/plot_b_coordinates.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/core/a_nddataset/plot_c_units.py` & `spectrochempy-0.6.7/spectrochempy/examples/core/a_nddataset/plot_c_units.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/core/b_units/units.py` & `spectrochempy-0.6.7/spectrochempy/examples/core/b_units/units.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/core/c_importer/plot_generic_read.py` & `spectrochempy-0.6.7/spectrochempy/examples/core/c_importer/plot_generic_read.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/core/c_importer/plot_read_IR_from_omnic.py` & `spectrochempy-0.6.7/spectrochempy/examples/core/c_importer/plot_read_IR_from_omnic.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/core/c_importer/plot_read_IR_from_opus.py` & `spectrochempy-0.6.7/spectrochempy/examples/core/c_importer/plot_read_IR_from_opus.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/core/c_importer/plot_read_nmr_from_bruker.py` & `spectrochempy-0.6.7/spectrochempy/examples/core/c_importer/plot_read_nmr_from_bruker.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/core/c_importer/plot_read_raman_from_labspec.py` & `spectrochempy-0.6.7/spectrochempy/examples/core/c_importer/plot_read_raman_from_labspec.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 """
 # %%
 import spectrochempy as scp
 
 # %%
 # define the folder where are the spectra
 datadir = scp.preferences.datadir
-ramandir = datadir / "ramandata"
+ramandir = datadir / "ramandata/labspec"
 
 # %%
 
 A = scp.read_labspec("Activation.txt", directory=ramandir)
 A.plot()
 
 A = scp.read_labspec("532nm-191216-Si_200mu.txt", directory=ramandir)
```

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/core/d_plotting/plot_plot_multiple.py` & `spectrochempy-0.6.7/spectrochempy/examples/core/d_plotting/plot_plot_multiple.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 """
 # %%
 # Import spectrochempy as usual
 import spectrochempy as scp
 
 # %%
 # Load the data (here 2D spectrum made from a list of 1D spectra):
-B1 = scp.read("ramandata/serie190214-1.txt")
+B1 = scp.read("ramandata/labspec/serie190214-1.txt")
 
 # %%
 # First we show the basic plot (note here the use of the `cmap=None` option to
 # display the spectra with rotating colors. cmap can be of course set to any other
 # available matplotlib colormap. The second parameter `lw` is used to set the line
 # width. In addition, we fix the figsize to have a better view of the spectra.
 prefs = B1.preferences
```

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/core/d_plotting/plot_plotting.py` & `spectrochempy-0.6.7/spectrochempy/examples/core/d_plotting/plot_plotting.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/core/e_project/plot_project.py` & `spectrochempy-0.6.7/spectrochempy/examples/core/e_project/plot_project.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/processing/apodization/plot_proc_em.py` & `spectrochempy-0.6.7/spectrochempy/examples/processing/apodization/plot_proc_em.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/processing/apodization/plot_proc_sp.py` & `spectrochempy-0.6.7/spectrochempy/examples/processing/apodization/plot_proc_sp.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/processing/denoising/plot_denoising.py` & `spectrochempy-0.6.7/spectrochempy/examples/processing/denoising/plot_denoising.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import spectrochempy as scp
 
 scp.set_loglevel("INFO")  # to see information
 
 # %%
 # Load the data (should be a 2D spectrum or a list of datasets that can be merged):
 
-dataset = scp.read("ramandata/serie190214-1.txt")
+dataset = scp.read("ramandata/labspec/serie190214-1.txt")
 
 # %%
 # select the useful region
 
 nd = dataset[:, 60.0:]
 
 # %%
```

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/processing/denoising/plot_despike.py` & `spectrochempy-0.6.7/spectrochempy/examples/processing/denoising/plot_despike.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
 In this example, we use the `despike` method to remove the noise from a Raman
 spectrum.
 """
 import spectrochempy as scp
 
 # %%
-# Load the data  ( )
+# Load the data
 
-dataset = scp.read("ramandata/serie190214-1.txt")
+dataset = scp.read("ramandata/labspec/serie190214-1.txt")
 
 # %%
 # Keep only one spectrum in this series
 # and select the useful region
 
 X = dataset[0, 70.0:]
 
@@ -35,32 +35,30 @@
 
 prefs = X.preferences
 prefs.figure.figsize = (8, 4)
 _ = X1.plot()
 
 # %%
 # Now let's use the `~spectrochempy.despike` method.
-# Only two parameters needs to be tuned: the `size`of the filter
-# (actually a savitsky-golay filter of order 2), and `delta`, the threshold for the
+# Only two parameters needs to be tuned: the `size` of the filter
+# (actually a Savitsky-Golay filter of order 2), and `delta`, the threshold for the
 # detection of spikes (outliers).
 # A spike is detected if its value is greater than `delta` times the standard deviation
 # of the difference between the original and the smoothed data.
 
-# sphinx_gallery_thumbnail_number = 2
-
 X2 = scp.despike(X1, size=11, delta=5)
 _ = X1.plot()
 _ = X2.plot(clear=False, ls="-", c="r")
 
-# %% [markdown]
+# %%
 # Getting the desired results require the tuning of size and delta parameters.
 # And sometimes may need to repeat the procedure on a previously filtered spectra.
 #
 # For example, if size or delta are badly chosen, valid peaks could be removed.
-# So carefull inspection of the results is crucial.
+# So careful inspection of the results is crucial.
 
 X3 = scp.despike(X1, size=21, delta=2)
 _ = X1.plot()
 _ = X3.plot(clear=False, ls="-", c="r")
 
 # %%
 # This ends the example ! The following line can be uncommented if no plot shows when
```

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/processing/filtering/plot_filter.py` & `spectrochempy-0.6.7/spectrochempy/examples/processing/filtering/plot_filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 # %%
 # First, we import a sample raman spectrum and plot it:
 
 # use the generic read function.
 # Note that read_labspec would be equivalent for this file format.
 
-X = scp.read("ramandata/SMC1-Initial_RT.txt")
+X = scp.read("ramandata/labspec/SMC1-Initial_RT.txt")
 prefs = X.preferences
 prefs.figure.figsize = (8, 4)
 _ = X.plot()
 
 # %%
 # here `Filter` processor is used to apply a Savitzky-Golay filter to the
 # spectrum.
```

### Comparing `spectrochempy-0.6.6/spectrochempy/examples/processing/raman/plot_raman_process.py` & `spectrochempy-0.6.7/spectrochempy/examples/processing/raman/plot_processing_raman.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import spectrochempy as scp
 
 # %%
 # Importing a 1D spectra
 # ----------------------
 # Define the folder where are the spectra
 datadir = scp.preferences.datadir
-ramandir = datadir / "ramandata"
+ramandir = datadir / "ramandata/labspec"
 
 # %%
 # Read a single spectrum
 A = scp.read_labspec("SMC1-Initial_RT.txt", directory=ramandir)
 
 # %%
 # Plot the spectrum
```

### Comparing `spectrochempy-0.6.6/spectrochempy/extern/nmrglue.py` & `spectrochempy-0.6.7/spectrochempy/extern/nmrglue.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,46 @@
+# Copyright Notice and Statement for the nmrglue Project
+# https://github.com/jjhelmus/nmrglue (BSD 3-Clause License)
+#
+# Copyright (c) 2010-2015 Jonathan J. Helmus
+# All rights reserved.
+#
+#
+# Redistribution and use in source and binary forms, with or without
+# modification, are permitted provided that the following conditions are
+# met:
+#
+#
+# 	a. Redistributions of source code must retain the above copyright
+#        notice, this list of conditions and the following disclaimer.
+#
+#
+# 	b. Redistributions in binary form must reproduce the above copyright
+#        notice, this list of conditions and the following disclaimer in the
+#        documentation and/or other materials provided with the
+#        distribution.
+#
+# 	c. Neither the name of the author nor the names of contributors may
+#        be used to endorse or promote products derived from this software
+#        without specific prior written permission.
+#
+#
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
+# "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
+# LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
+# A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
+# OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
+# SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
+# LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
+# DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
+# THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+# (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+
 """
 Functions for reading and writing Bruker binary (ser/fid) files, Bruker
 JCAMP-DX parameter (acqus) files, and Bruker pulse program (pulseprogram)
 files.
 
 Copied and adapted from NMRGLUE (See NMRGLUE_LICENCES in root folder LICENSES)
 """
```

### Comparing `spectrochempy-0.6.6/spectrochempy/extern/traittypes.py` & `spectrochempy-0.6.7/spectrochempy/extern/traittypes.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/extern/traittypes_utils.py` & `spectrochempy-0.6.7/spectrochempy/extern/traittypes_utils.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/extern/whittaker_smooth.py` & `spectrochempy-0.6.7/spectrochempy/extern/whittaker_smooth.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/ipython/magics.py` & `spectrochempy-0.6.7/spectrochempy/ipython/magics.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/processing/_base/_processingbase.py` & `spectrochempy-0.6.7/spectrochempy/processing/_base/_processingbase.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/processing/alignement/align.py` & `spectrochempy-0.6.7/spectrochempy/processing/alignement/align.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/processing/alignement/api.py` & `spectrochempy-0.6.7/spectrochempy/processing/alignement/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/processing/api.py` & `spectrochempy-0.6.7/spectrochempy/processing/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/processing/fft/api.py` & `spectrochempy-0.6.7/spectrochempy/processing/fft/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/processing/fft/apodization.py` & `spectrochempy-0.6.7/spectrochempy/processing/fft/apodization.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/processing/fft/fft.py` & `spectrochempy-0.6.7/spectrochempy/processing/fft/fft.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/processing/fft/phasing.py` & `spectrochempy-0.6.7/spectrochempy/processing/fft/phasing.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/processing/fft/shift.py` & `spectrochempy-0.6.7/spectrochempy/processing/fft/shift.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/processing/fft/zero_filling.py` & `spectrochempy-0.6.7/spectrochempy/processing/fft/zero_filling.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/processing/filter/api.py` & `spectrochempy-0.6.7/spectrochempy/processing/filter/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/processing/filter/denoise.py` & `spectrochempy-0.6.7/spectrochempy/processing/filter/denoise.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/processing/filter/filter.py` & `spectrochempy-0.6.7/spectrochempy/processing/filter/filter.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/processing/interpolation/api.py` & `spectrochempy-0.6.7/spectrochempy/processing/interpolation/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/processing/interpolation/interpolate.py` & `spectrochempy-0.6.7/spectrochempy/processing/interpolation/interpolate.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/processing/transformation/api.py` & `spectrochempy-0.6.7/spectrochempy/processing/transformation/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/processing/transformation/autosub.py` & `spectrochempy-0.6.7/spectrochempy/processing/transformation/autosub.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/processing/transformation/concatenate.py` & `spectrochempy-0.6.7/spectrochempy/processing/transformation/concatenate.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 __all__ = ["concatenate", "stack"]
 
 __dataset_methods__ = __all__
 
-import datetime as datetime
 from warnings import warn
 
 import numpy as np
 
 from spectrochempy.core.dataset.baseobjects.ndarray import DEFAULT_DIM_NAME
 from spectrochempy.core.dataset.coord import Coord
 from spectrochempy.utils import exceptions
+from spectrochempy.utils.datetimeutils import utcnow
 from spectrochempy.utils.decorators import deprecated
 from spectrochempy.utils.orderedset import OrderedSet
 
 
 def concatenate(*datasets, **kwargs):
     """
     Concatenation of `NDDataset` objects along a given axis.
@@ -178,15 +178,15 @@
             authortuple = authortuple + (dataset.author,)
 
         out.author = " & ".join([str(author) for author in authortuple])
 
         out.description += ", {}".format(dataset.name)
 
     out.description += " )"
-    out._date = out._modified = datetime.datetime.now(datetime.timezone.utc)
+    out._date = out._modified = utcnow()
     out.history = ["Created by concatenate"]
 
     return out
 
 
 def stack(*datasets):
     """
```

### Comparing `spectrochempy-0.6.6/spectrochempy/processing/transformation/npy.py` & `spectrochempy-0.6.7/spectrochempy/processing/transformation/npy.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/structure.md` & `spectrochempy-0.6.7/spectrochempy/structure.md`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/__init__.py` & `spectrochempy-0.6.7/spectrochempy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/baseconfigurable.py` & `spectrochempy-0.6.7/spectrochempy/utils/baseconfigurable.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,14 +292,18 @@
         # validation fired when self._X is assigned
         X = proposal.value
 
         # for the following we need X with two dimensions
         # So let's generate the un-squeezed X
         X = self._make_unsqueezed_dataset(X)
 
+        # if X is complex or quaternion, we will work on the real part only
+        if X.is_complex or X.is_quaternion:
+            X = X.real
+
         # as in fit methods we often use np.linalg library, we cannot handle directly
         # masked data (so we remove them here and they will be restored at the end of
         # the process during transform or inverse transform methods
         # store the original shape as it will be eventually modified as welle- as the
         # original coordset
         self._X_shape = X.shape
```

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/citation.py` & `spectrochempy-0.6.7/spectrochempy/utils/citation.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/compare.py` & `spectrochempy-0.6.7/spectrochempy/utils/compare.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/constants.py` & `spectrochempy-0.6.7/spectrochempy/utils/constants.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/coordrange.py` & `spectrochempy-0.6.7/spectrochempy/utils/coordrange.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/decorators.py` & `spectrochempy-0.6.7/spectrochempy/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/docstrings.py` & `spectrochempy-0.6.7/spectrochempy/utils/docstrings.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/exceptions.py` & `spectrochempy-0.6.7/spectrochempy/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/fake.py` & `spectrochempy-0.6.7/spectrochempy/utils/fake.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/file.py` & `spectrochempy-0.6.7/spectrochempy/utils/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,21 @@
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
 File utilities.
 """
 import re
+import struct
 import warnings
 from os import environ
 from pathlib import Path, PosixPath, WindowsPath
 
+import numpy as np
+
 
 # ======================================================================================
 # Utility functions
 # ======================================================================================
 def download_testdata():
     from spectrochempy.core import preferences
     from spectrochempy.core.readers.importer import read
@@ -25,14 +28,39 @@
     # this process is relatively long, so we do not want to do it several time:
     downloaded = datadir / "__downloaded__"
     if not downloaded.exists():
         read(datadir, download_only=True)
         downloaded.touch(exist_ok=True)
 
 
+def fromfile(fid, dtype, count):
+    # to replace np.fromfile in case of io.BytesIO object instead of byte
+    # object
+    t = {
+        "uint8": "B",
+        "int8": "b",
+        "uint16": "H",
+        "int16": "h",
+        "uint32": "I",
+        "int32": "i",
+        "float32": "f",
+        "char8": "c",
+    }
+    typ = t[dtype] * count
+    if dtype.endswith("16"):
+        count *= 2
+    elif dtype.endswith("32"):
+        count *= 4
+
+    out = struct.unpack(typ, fid.read(count))
+    if len(out) == 1:
+        return out[0]
+    return np.array(out)
+
+
 def _insensitive_case_glob(pattern):
     def either(c):
         return f"[{c.lower()}{c.upper()}]" if c.isalpha() else c
 
     return "".join(map(either, pattern))
```

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/jsonutils.py` & `spectrochempy-0.6.7/spectrochempy/utils/jsonutils.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/metaconfigurable.py` & `spectrochempy-0.6.7/spectrochempy/utils/metaconfigurable.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/misc.py` & `spectrochempy-0.6.7/spectrochempy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/numutils.py` & `spectrochempy-0.6.7/spectrochempy/utils/numutils.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/objects.py` & `spectrochempy-0.6.7/spectrochempy/utils/objects.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/optional.py` & `spectrochempy-0.6.7/spectrochempy/utils/optional.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/orderedset.py` & `spectrochempy-0.6.7/spectrochempy/utils/orderedset.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/packages.py` & `spectrochempy-0.6.7/spectrochempy/utils/packages.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/plots.py` & `spectrochempy-0.6.7/spectrochempy/utils/plots.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/print.py` & `spectrochempy-0.6.7/spectrochempy/utils/print.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/print_versions.py` & `spectrochempy-0.6.7/spectrochempy/utils/print_versions.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/system.py` & `spectrochempy-0.6.7/spectrochempy/utils/system.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/testing.py` & `spectrochempy-0.6.7/spectrochempy/utils/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,14 @@
     if not issubdtype(z.dtype, number):
         z = z.astype(float_)  # handle object arrays
 
     return z < 1.5 * 10.0 ** (-decimal)
 
 
 def compare_ndarrays(this, other, approx=False, decimal=6, data_only=False):
-
     # Comparison based on attributes:
     #        data, dims, mask, labels, units, meta
 
     from spectrochempy.core.units import ur
 
     def compare(x, y):
         return _compare(x, y, decimal)
@@ -203,15 +202,14 @@
             else:
                 raise AssertionError(f"{other} has no units")
 
     return True
 
 
 def compare_coords(this, other, approx=False, decimal=3, data_only=False):
-
     # TODO: compare base on signficant digit for coordinate instead of decimals
     #  (that may not work for very small coordinates numbers)
     from spectrochempy.core.units import ur
 
     def compare(x, y):
         return _compare(x, y, decimal)
 
@@ -240,15 +238,15 @@
                 if (
                     hasattr(oattr, "size")
                     and hasattr(sattr, "size")
                     and oattr.size != sattr.size
                 ):
                     raise AssertionError(f"{thistype}.{attr} sizes are different.")
 
-                if attr == "data":
+                if attr == "data" and not (sattr is None and oattr is None):
                     if approx:
                         assert_array_compare(
                             compare,
                             sattr,
                             oattr,
                             header=(
                                 f"{thistype}.{attr} attributes ar"
@@ -569,15 +567,15 @@
 
         random.set_state(self.startstate)
 
 
 # ======================================================================================
 # raises and assertions (mostly copied from astropy)
 # ======================================================================================
-def assert_equal_units(unit1, unit2, strict=False):
+def assert_units_equal(unit1, unit2, strict=False):
     """
     Compare units.
 
     Parameters
     ----------
     unit1 : units
         Units to be compared.
```

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/timeutils.py` & `spectrochempy-0.6.7/spectrochempy/utils/timeutils.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/traits.py` & `spectrochempy-0.6.7/spectrochempy/utils/traits.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/version.py` & `spectrochempy-0.6.7/spectrochempy/utils/version.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/warnings.py` & `spectrochempy-0.6.7/spectrochempy/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/utils/zip.py` & `spectrochempy-0.6.7/spectrochempy/utils/zip.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/widgets/baselinecorrector.py` & `spectrochempy-0.6.7/spectrochempy/widgets/baselinecorrector.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy/widgets/fileselector.py` & `spectrochempy-0.6.7/spectrochempy/widgets/fileselector.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.6/spectrochempy.egg-info/PKG-INFO` & `spectrochempy-0.6.7/spectrochempy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrochempy
-Version: 0.6.6
+Version: 0.6.7
 Summary: Processing, analysis and modelling Spectroscopic data for Chemistry with Python
 Home-page: https://www.spectrochempy.fr
 Author: Arnaud Travert & Christian Fernandez
 Author-email: contact@spectrochempy.fr
 Maintainer: C. Fernandez
 Maintainer-email: christian.fernandez@ensicaen.fr
 License: CECILL-B
@@ -14,18 +14,17 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: CeCILL-B Free Software License Agreement (CECILL-B)
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align ="center">
 <img src='https://github.com/spectrochempy/spectrochempy/raw/master/docs/_static/scpy.png' width="150">
 <br>
 SpectroChemPy
```

### Comparing `spectrochempy-0.6.6/spectrochempy.egg-info/SOURCES.txt` & `spectrochempy-0.6.7/spectrochempy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 setup.cfg
 setup.py
 .conda/meta.yaml
 LICENSES/NMRGLUE_LICENSE.rst
 LICENSES/NNMF_LICENSE.rst
 LICENSES/PACKAGING_LICENSE.rst
 LICENSES/PANDAS_LICENSE.rst
+LICENSES/PY_WDF_READER_LICENSE.rst
 LICENSES/TRAITTYPES_LICENSE.rst
 LICENSES/WHITTAKER_SMOOTH_LICENSE.rst
 requirements/requirements.txt
 requirements/requirements_dev.txt
 requirements/requirements_test.txt
 scp_data/__init__.py
 scp_data/databases/isotopes.csv
@@ -154,14 +155,15 @@
 spectrochempy/core/readers/read_matlab.py
 spectrochempy/core/readers/read_omnic.py
 spectrochempy/core/readers/read_opus.py
 spectrochempy/core/readers/read_quadera.py
 spectrochempy/core/readers/read_soc.py
 spectrochempy/core/readers/read_spc.py
 spectrochempy/core/readers/read_topspin.py
+spectrochempy/core/readers/read_wire.py
 spectrochempy/core/readers/read_zip.py
 spectrochempy/core/script/__init__.py
 spectrochempy/core/units/__init__.py
 spectrochempy/core/writers/__init__.py
 spectrochempy/core/writers/api.py
 spectrochempy/core/writers/exporter.py
 spectrochempy/core/writers/write_csv.py
@@ -203,14 +205,15 @@
 spectrochempy/examples/core/b_units/units.py
 spectrochempy/examples/core/c_importer/__init__.py
 spectrochempy/examples/core/c_importer/plot_generic_read.py
 spectrochempy/examples/core/c_importer/plot_read_IR_from_omnic.py
 spectrochempy/examples/core/c_importer/plot_read_IR_from_opus.py
 spectrochempy/examples/core/c_importer/plot_read_nmr_from_bruker.py
 spectrochempy/examples/core/c_importer/plot_read_raman_from_labspec.py
+spectrochempy/examples/core/c_importer/plot_read_renishaw.py
 spectrochempy/examples/core/c_importer/readme.rst
 spectrochempy/examples/core/d_plotting/__init__.py
 spectrochempy/examples/core/d_plotting/plot_plot_multiple.py
 spectrochempy/examples/core/d_plotting/plot_plotting.py
 spectrochempy/examples/core/d_plotting/readme.rst
 spectrochempy/examples/core/e_project/__init__.py
 spectrochempy/examples/core/e_project/plot_project.py
@@ -224,16 +227,19 @@
 spectrochempy/examples/processing/denoising/__init__.py
 spectrochempy/examples/processing/denoising/plot_denoising.py
 spectrochempy/examples/processing/denoising/plot_despike.py
 spectrochempy/examples/processing/denoising/readme.rst
 spectrochempy/examples/processing/filtering/__init__.py
 spectrochempy/examples/processing/filtering/plot_filter.py
 spectrochempy/examples/processing/filtering/readme.rst
+spectrochempy/examples/processing/nmr/__init__.py
+spectrochempy/examples/processing/nmr/plot_processing_nmr.py
+spectrochempy/examples/processing/nmr/readme.rst
 spectrochempy/examples/processing/raman/__init__.py
-spectrochempy/examples/processing/raman/plot_raman_process.py
+spectrochempy/examples/processing/raman/plot_processing_raman.py
 spectrochempy/examples/processing/raman/readme.rst
 spectrochempy/extern/__init__.py
 spectrochempy/extern/nmrglue.py
 spectrochempy/extern/traittypes.py
 spectrochempy/extern/traittypes_utils.py
 spectrochempy/extern/whittaker_smooth.py
 spectrochempy/ipython/__init__.py
@@ -266,14 +272,15 @@
 spectrochempy/processing/transformation/npy.py
 spectrochempy/utils/__init__.py
 spectrochempy/utils/baseconfigurable.py
 spectrochempy/utils/citation.py
 spectrochempy/utils/compare.py
 spectrochempy/utils/constants.py
 spectrochempy/utils/coordrange.py
+spectrochempy/utils/datetimeutils.py
 spectrochempy/utils/decorators.py
 spectrochempy/utils/docstrings.py
 spectrochempy/utils/exceptions.py
 spectrochempy/utils/fake.py
 spectrochempy/utils/file.py
 spectrochempy/utils/jsonutils.py
 spectrochempy/utils/metaconfigurable.py
```

