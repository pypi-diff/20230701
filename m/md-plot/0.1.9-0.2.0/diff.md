# Comparing `tmp/md_plot-0.1.9.tar.gz` & `tmp/md_plot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md_plot-0.1.9.tar", last modified: Wed Mar  9 13:00:40 2022, max compression
+gzip compressed data, was "md_plot-0.2.0.tar", last modified: Sat Jul  1 11:53:50 2023, max compression
```

## Comparing `md_plot-0.1.9.tar` & `md_plot-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,120 @@
-drwxrwxrwx   0        0        0        0 2022-03-09 13:00:40.725706 md_plot-0.1.9/
--rw-rw-rw-   0        0        0      423 2022-03-09 11:37:12.000000 md_plot-0.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1803 2022-03-09 13:00:40.720720 md_plot-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     1617 2022-03-09 11:37:12.000000 md_plot-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2022-03-09 13:00:40.486144 md_plot-0.1.9/md_plot/
--rw-rw-rw-   0        0        0       94 2022-03-09 12:48:49.000000 md_plot-0.1.9/md_plot/__init__.py
-drwxrwxrwx   0        0        0        0 2022-03-09 13:00:40.627969 md_plot-0.1.9/md_plot/examples/
--rw-rw-rw-   0        0        0   713264 2022-03-09 11:37:12.000000 md_plot-0.1.9/md_plot/examples/BimodalArtificial.gz.pkl
--rw-rw-rw-   0        0        0    40107 2022-03-09 11:37:12.000000 md_plot-0.1.9/md_plot/examples/MTY_Clipped.gz.pkl
--rw-rw-rw-   0        0        0    74065 2022-03-09 11:37:12.000000 md_plot-0.1.9/md_plot/examples/MuncipalIncomeTaxYield_IncomeTaxShare.gz.pkl
--rw-rw-rw-   0        0        0     4255 2022-03-09 11:37:12.000000 md_plot-0.1.9/md_plot/examples/SampleLogInome.gz.pkl
--rw-rw-rw-   0        0        0   461683 2022-03-09 11:37:12.000000 md_plot-0.1.9/md_plot/examples/SkewedDistribution.gz.pkl
--rw-rw-rw-   0        0        0   462122 2022-03-09 11:37:12.000000 md_plot-0.1.9/md_plot/examples/SkewedDistributionLongTable.gz.pkl
--rw-rw-rw-   0        0        0    51719 2022-03-09 11:37:12.000000 md_plot-0.1.9/md_plot/examples/StocksData2018Q1.gz.pkl
--rw-rw-rw-   0        0        0     6840 2022-03-09 11:37:12.000000 md_plot-0.1.9/md_plot/examples/UniformSample.gz.pkl
-drwxrwxrwx   0        0        0        0 2022-03-09 13:00:40.711744 md_plot-0.1.9/md_plot/helper/
--rw-rw-rw-   0        0        0      350 2022-03-09 11:37:12.000000 md_plot-0.1.9/md_plot/helper/__init__.py
--rw-rw-rw-   0        0        0     6141 2022-03-09 11:37:12.000000 md_plot-0.1.9/md_plot/helper/bimodal.py
--rw-rw-rw-   0        0        0     1285 2022-03-09 11:37:12.000000 md_plot-0.1.9/md_plot/helper/optimal_no_bins.py
--rw-rw-rw-   0        0        0     5897 2022-03-09 11:38:44.000000 md_plot-0.1.9/md_plot/helper/pareto_density_estimation.py
--rw-rw-rw-   0        0        0     3473 2022-03-09 11:37:12.000000 md_plot-0.1.9/md_plot/helper/pareto_radius.py
--rw-rw-rw-   0        0        0     1892 2022-03-09 11:37:12.000000 md_plot-0.1.9/md_plot/helper/pretty.py
--rw-rw-rw-   0        0        0     4394 2022-03-09 11:37:12.000000 md_plot-0.1.9/md_plot/helper/robust_normalization.py
--rw-rw-rw-   0        0        0     1232 2022-03-09 11:37:12.000000 md_plot-0.1.9/md_plot/helper/signed_log.py
--rw-rw-rw-   0        0        0     3539 2022-03-09 11:37:12.000000 md_plot-0.1.9/md_plot/helper/stat_pde_density.py
--rw-rw-rw-   0        0        0     1453 2022-03-09 11:37:12.000000 md_plot-0.1.9/md_plot/load_examples.py
--rw-rw-rw-   0        0        0    17761 2022-03-09 11:54:27.000000 md_plot-0.1.9/md_plot/md_plot.py
-drwxrwxrwx   0        0        0        0 2022-03-09 13:00:40.530040 md_plot-0.1.9/md_plot.egg-info/
--rw-rw-rw-   0        0        0     1803 2022-03-09 13:00:39.000000 md_plot-0.1.9/md_plot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      922 2022-03-09 13:00:40.000000 md_plot-0.1.9/md_plot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-09 13:00:39.000000 md_plot-0.1.9/md_plot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-03-09 13:00:39.000000 md_plot-0.1.9/md_plot.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       88 2022-03-09 13:00:39.000000 md_plot-0.1.9/md_plot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-03-09 13:00:40.000000 md_plot-0.1.9/md_plot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-03-09 13:00:40.725706 md_plot-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1423 2022-03-09 12:51:26.000000 md_plot-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 11:53:50.888298 md_plot-0.2.0/
+-rw-rw-rw-   0        0        0      437 2020-05-11 05:25:01.000000 md_plot-0.2.0/.gitignore
+-rw-rw-rw-   0        0        0    35821 2020-05-11 05:25:01.000000 md_plot-0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      448 2023-07-01 09:25:19.000000 md_plot-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1642 2023-07-01 11:53:50.887299 md_plot-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1617 2020-05-11 05:25:01.000000 md_plot-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 11:53:50.274478 md_plot-0.2.0/doc/
+drwxrwxrwx   0        0        0        0 2023-07-01 11:53:50.312479 md_plot-0.2.0/doc/images/
+-rw-rw-rw-   0        0        0    29408 2020-05-11 05:25:01.000000 md_plot-0.2.0/doc/images/bimodal_artificial.png
+drwxrwxrwx   0        0        0        0 2023-07-01 11:53:50.328436 md_plot-0.2.0/docs/
+-rw-rw-rw-   0        0        0      623 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-07-01 11:53:50.278470 md_plot-0.2.0/docs/_build/
+drwxrwxrwx   0        0        0        0 2023-07-01 11:53:50.278470 md_plot-0.2.0/docs/_build/html/
+drwxrwxrwx   0        0        0        0 2023-07-01 11:53:50.499058 md_plot-0.2.0/docs/_build/html/_static/
+-rw-rw-rw-   0        0        0      673 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/_build/html/_static/ajax-loader.gif
+-rw-rw-rw-   0        0        0    11380 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/_build/html/_static/basic.css
+-rw-rw-rw-   0        0        0      756 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/_build/html/_static/comment-bright.png
+-rw-rw-rw-   0        0        0      829 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/_build/html/_static/comment-close.png
+-rw-rw-rw-   0        0        0      641 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/_build/html/_static/comment.png
+-rw-rw-rw-   0        0        0     9536 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/_build/html/_static/doctools.js
+-rw-rw-rw-   0        0        0      212 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/_build/html/_static/documentation_options.js
+-rw-rw-rw-   0        0        0      222 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/_build/html/_static/down-pressed.png
+-rw-rw-rw-   0        0        0      202 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/_build/html/_static/down.png
+-rw-rw-rw-   0        0        0      286 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/_build/html/_static/file.png
+-rw-rw-rw-   0        0        0   278292 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/_build/html/_static/jquery-3.2.1.js
+-rw-rw-rw-   0        0        0    86663 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/_build/html/_static/jquery.js
+-rw-rw-rw-   0        0        0       90 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/_build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/_build/html/_static/plus.png
+-rw-rw-rw-   0        0        0     4463 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/_build/html/_static/pygments.css
+-rw-rw-rw-   0        0        0    26209 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/_build/html/_static/searchtools.js
+-rw-rw-rw-   0        0        0    36167 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/_build/html/_static/underscore-1.3.1.js
+-rw-rw-rw-   0        0        0    12171 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/_build/html/_static/underscore.js
+-rw-rw-rw-   0        0        0      214 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/_build/html/_static/up-pressed.png
+-rw-rw-rw-   0        0        0      203 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/_build/html/_static/up.png
+-rw-rw-rw-   0        0        0    26163 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/_build/html/_static/websupport.js
+drwxrwxrwx   0        0        0        0 2023-07-01 11:53:50.503046 md_plot-0.2.0/docs/application/
+drwxrwxrwx   0        0        0        0 2023-07-01 11:53:50.576848 md_plot-0.2.0/docs/application/FuerDoku/
+-rw-rw-rw-   0        0        0    35591 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/application/FuerDoku/CD20.png
+-rw-rw-rw-   0        0        0    36277 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/application/FuerDoku/CD23.png
+-rw-rw-rw-   0        0        0    35129 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/application/FuerDoku/CD5.png
+-rw-rw-rw-   0        0        0    36250 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/application/FuerDoku/CD7lambda.png
+-rw-rw-rw-   0        0        0    35954 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/application/FuerDoku/CD8kappa.png
+-rw-rw-rw-   0        0        0    32867 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/application/FuerDoku/CashAndCashEquivalents.png
+-rw-rw-rw-   0        0        0   142079 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/application/FuerDoku/FlowCyotometry.jpeg
+-rw-rw-rw-   0        0        0    31085 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/application/FuerDoku/IncomeBeforeTax.png
+-rw-rw-rw-   0        0        0    33397 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/application/FuerDoku/NetIncomeFromContinuingOps.png
+-rw-rw-rw-   0        0        0    32152 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/application/FuerDoku/OperatingIncomeorLoss.png
+-rw-rw-rw-   0        0        0     6561 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/application/example_application.md
+-rw-rw-rw-   0        0        0     5008 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/conf.py
+-rw-rw-rw-   0        0        0      573 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/index.rst
+-rwxrwxrwx   0        0        0      811 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-07-01 11:53:50.593803 md_plot-0.2.0/docs/user_guide/
+-rw-rw-rw-   0        0        0     2428 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/13FlowCytometry.md
+drwxrwxrwx   0        0        0        0 2023-07-01 11:53:50.780445 md_plot-0.2.0/docs/user_guide/images/
+-rw-rw-rw-   0        0        0   142079 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/images/FlowCyotometry.jpeg
+-rw-rw-rw-   0        0        0    49924 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/images/MDplot_stocksdata.png
+-rw-rw-rw-   0        0        0    89073 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/images/MDplot_stocksdata_ordered.png
+-rw-rw-rw-   0        0        0    53990 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/images/Multimodal.jpeg
+-rw-rw-rw-   0        0        0    25197 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/images/RobustMDplot.png
+-rw-rw-rw-   0        0        0    23503 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/images/beanplotuniform.jpeg
+-rw-rw-rw-   0        0        0    29408 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/images/bimodal_artificial.png
+-rw-rw-rw-   0        0        0    27800 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/images/bimodal_with_green_gaussian.png
+-rw-rw-rw-   0        0        0    22306 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/images/bimodal_without_gaussian.png
+-rw-rw-rw-   0        0        0    15887 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/images/box_plot.png
+-rw-rw-rw-   0        0        0    52296 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/images/ggplot1_stocksdata.png
+-rw-rw-rw-   0        0        0    60181 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/images/ggplot2_stocksdata.png
+-rw-rw-rw-   0        0        0    58672 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/images/ggplot3_stocksdata.png
+-rw-rw-rw-   0        0        0    25372 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/images/ggplot_fails.png
+-rw-rw-rw-   0        0        0    16152 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/images/its_mty.png
+-rw-rw-rw-   0        0        0    17891 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/images/its_mty_scaled.png
+-rw-rw-rw-   0        0        0    48261 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/images/itsboxplot.jpeg
+-rw-rw-rw-   0        0        0    15356 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/images/load_examples.png
+-rw-rw-rw-   0        0        0    33534 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/images/mdplotuniform.jpeg
+-rw-rw-rw-   0        0        0    45705 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/images/mty.jpeg
+-rw-rw-rw-   0        0        0    17178 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/images/mty_clipped.png
+-rw-rw-rw-   0        0        0    18133 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/images/mty_clipped_layout.png
+-rw-rw-rw-   0        0        0    17257 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/images/mty_clipped_sample.png
+-rw-rw-rw-   0        0        0    56621 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/images/stocks_alphabetical.png
+-rw-rw-rw-   0        0        0    56609 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/images/stocks_statistics.png
+-rw-rw-rw-   0        0        0     1257 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/python_package.md
+-rw-rw-rw-   0        0        0     8300 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/python_tutorial.md
+-rw-rw-rw-   0        0        0      435 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/r_package.md
+-rw-rw-rw-   0        0        0     8543 2020-05-11 05:25:01.000000 md_plot-0.2.0/docs/user_guide/r_tutorial.md
+drwxrwxrwx   0        0        0        0 2023-07-01 11:53:50.791416 md_plot-0.2.0/md_plot/
+-rw-rw-rw-   0        0        0       94 2023-07-01 11:45:20.000000 md_plot-0.2.0/md_plot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 11:53:50.846268 md_plot-0.2.0/md_plot/examples/
+-rw-rw-rw-   0        0        0   713264 2020-05-11 05:25:01.000000 md_plot-0.2.0/md_plot/examples/BimodalArtificial.gz.pkl
+-rw-rw-rw-   0        0        0    40107 2020-05-11 05:25:01.000000 md_plot-0.2.0/md_plot/examples/MTY_Clipped.gz.pkl
+-rw-rw-rw-   0        0        0    74065 2020-05-11 05:25:01.000000 md_plot-0.2.0/md_plot/examples/MuncipalIncomeTaxYield_IncomeTaxShare.gz.pkl
+-rw-rw-rw-   0        0        0     4255 2020-05-11 05:25:01.000000 md_plot-0.2.0/md_plot/examples/SampleLogInome.gz.pkl
+-rw-rw-rw-   0        0        0   461683 2020-05-11 05:25:01.000000 md_plot-0.2.0/md_plot/examples/SkewedDistribution.gz.pkl
+-rw-rw-rw-   0        0        0   462122 2020-05-11 05:25:01.000000 md_plot-0.2.0/md_plot/examples/SkewedDistributionLongTable.gz.pkl
+-rw-rw-rw-   0        0        0    51719 2020-05-11 05:25:01.000000 md_plot-0.2.0/md_plot/examples/StocksData2018Q1.gz.pkl
+-rw-rw-rw-   0        0        0     6840 2020-05-11 05:25:01.000000 md_plot-0.2.0/md_plot/examples/UniformSample.gz.pkl
+drwxrwxrwx   0        0        0        0 2023-07-01 11:53:50.875191 md_plot-0.2.0/md_plot/helper/
+-rw-rw-rw-   0        0        0      350 2020-05-15 08:21:02.000000 md_plot-0.2.0/md_plot/helper/__init__.py
+-rw-rw-rw-   0        0        0     6169 2023-07-01 09:41:06.000000 md_plot-0.2.0/md_plot/helper/bimodal.py
+-rw-rw-rw-   0        0        0     1285 2020-05-11 05:25:01.000000 md_plot-0.2.0/md_plot/helper/optimal_no_bins.py
+-rw-rw-rw-   0        0        0     5896 2023-07-01 09:37:57.000000 md_plot-0.2.0/md_plot/helper/pareto_density_estimation.py
+-rw-rw-rw-   0        0        0     3473 2020-05-11 05:25:01.000000 md_plot-0.2.0/md_plot/helper/pareto_radius.py
+-rw-rw-rw-   0        0        0     1892 2020-05-11 05:25:01.000000 md_plot-0.2.0/md_plot/helper/pretty.py
+-rw-rw-rw-   0        0        0     4394 2020-05-11 05:25:01.000000 md_plot-0.2.0/md_plot/helper/robust_normalization.py
+-rw-rw-rw-   0        0        0     1232 2020-05-11 05:25:01.000000 md_plot-0.2.0/md_plot/helper/signed_log.py
+-rw-rw-rw-   0        0        0     3539 2020-05-11 05:25:01.000000 md_plot-0.2.0/md_plot/helper/stat_pde_density.py
+-rw-rw-rw-   0        0        0     1453 2020-05-11 05:25:01.000000 md_plot-0.2.0/md_plot/load_examples.py
+-rw-rw-rw-   0        0        0    17796 2023-07-01 11:35:21.000000 md_plot-0.2.0/md_plot/md_plot.py
+drwxrwxrwx   0        0        0        0 2023-07-01 11:53:50.883171 md_plot-0.2.0/md_plot/unidip/
+-rw-rw-rw-   0        0        0        0 2023-07-01 11:41:26.000000 md_plot-0.2.0/md_plot/unidip/__init__.py
+-rw-rw-rw-   0        0        0     4747 2023-07-01 11:33:11.000000 md_plot-0.2.0/md_plot/unidip/dip.py
+-rw-rw-rw-   0        0        0     9393 2023-07-01 11:29:36.000000 md_plot-0.2.0/md_plot/unidip/unidip.py
+drwxrwxrwx   0        0        0        0 2023-07-01 11:53:50.812359 md_plot-0.2.0/md_plot.egg-info/
+-rw-rw-rw-   0        0        0     1642 2023-07-01 11:53:50.000000 md_plot-0.2.0/md_plot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3665 2023-07-01 11:53:50.000000 md_plot-0.2.0/md_plot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 11:53:50.000000 md_plot-0.2.0/md_plot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2020-05-15 10:01:02.000000 md_plot-0.2.0/md_plot.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       74 2023-07-01 11:53:50.000000 md_plot-0.2.0/md_plot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-01 11:53:50.000000 md_plot-0.2.0/md_plot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      698 2020-05-11 05:25:01.000000 md_plot-0.2.0/readme_pypi.rst
+-rw-rw-rw-   0        0        0       42 2023-07-01 11:53:50.889294 md_plot-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1396 2023-07-01 11:47:12.000000 md_plot-0.2.0/setup.py
```

### Comparing `md_plot-0.1.9/PKG-INFO` & `md_plot-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: md_plot
-Version: 0.1.9
+Version: 0.2.0
 Summary: Draws a mirrored density plot for each input column
-Home-page: UNKNOWN
+Download-URL: https://github.com/TinoGehlert/md_plot/archive/v0.2.0.tar.gz
 Author: TinoGehlert
 Author-email: tinogehlert@aol.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/TinoGehlert/md_plot/archive/v0.1.9.tar.gz
 Project-URL: R-Version, https://cran.r-project.org/web/packages/DataVisualizations/index.html
 Project-URL: Source, https://github.com/TinoGehlert/md_plot
 Project-URL: Docs, https://md-plot.readthedocs.io
-Description: Mirrored Density Plot
-        =====================
-        
-        This function creates a MD-plot for each column of the dataframe. The MD-plot is a visualization
-        for a boxplot-like Shape of the PDF published in [Thrun/Ultsch, 2019]. It is an improvement of
-        violin or so-called bean plots and posses advantages in comparison to the conventional well-known
-        box plot [Thrun/Ultsch, 2019]. This is the Python implementation of the function MD-Plot contained 
-        in R package [DataVisualizations](https://cran.r-project.org/web/packages/DataVisualizations/index.html)
-        
-        Basic Usage
-        ^^^^^^^^^^^
-        
-        from md_plot import MDplot, load_examples
-        
-        dctExamples = load_examples()
-        
-        MDplot(dctExamples["BimodalArtificial"])
-        
 Keywords: data_science violin density_plot
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
+License-File: LICENSE.txt
+
+Mirrored Density Plot
+=====================
+
+This function creates a MD-plot for each column of the dataframe. The MD-plot is a visualization
+for a boxplot-like Shape of the PDF published in [Thrun/Ultsch, 2019]. It is an improvement of
+violin or so-called bean plots and posses advantages in comparison to the conventional well-known
+box plot [Thrun/Ultsch, 2019]. This is the Python implementation of the function MD-Plot contained 
+in R package [DataVisualizations](https://cran.r-project.org/web/packages/DataVisualizations/index.html)
+
+Basic Usage
+^^^^^^^^^^^
+
+from md_plot import MDplot, load_examples
+
+dctExamples = load_examples()
+
+MDplot(dctExamples["BimodalArtificial"])
```

### Comparing `md_plot-0.1.9/README.md` & `md_plot-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `md_plot-0.1.9/md_plot/examples/BimodalArtificial.gz.pkl` & `md_plot-0.2.0/md_plot/examples/BimodalArtificial.gz.pkl`

 * *Files identical despite different names*

### Comparing `md_plot-0.1.9/md_plot/examples/MTY_Clipped.gz.pkl` & `md_plot-0.2.0/md_plot/examples/MTY_Clipped.gz.pkl`

 * *Files identical despite different names*

### Comparing `md_plot-0.1.9/md_plot/examples/MuncipalIncomeTaxYield_IncomeTaxShare.gz.pkl` & `md_plot-0.2.0/md_plot/examples/MuncipalIncomeTaxYield_IncomeTaxShare.gz.pkl`

 * *Files identical despite different names*

### Comparing `md_plot-0.1.9/md_plot/examples/SampleLogInome.gz.pkl` & `md_plot-0.2.0/md_plot/examples/SampleLogInome.gz.pkl`

 * *Files identical despite different names*

### Comparing `md_plot-0.1.9/md_plot/examples/SkewedDistribution.gz.pkl` & `md_plot-0.2.0/md_plot/examples/SkewedDistribution.gz.pkl`

 * *Files identical despite different names*

### Comparing `md_plot-0.1.9/md_plot/examples/SkewedDistributionLongTable.gz.pkl` & `md_plot-0.2.0/md_plot/examples/SkewedDistributionLongTable.gz.pkl`

 * *Files identical despite different names*

### Comparing `md_plot-0.1.9/md_plot/examples/StocksData2018Q1.gz.pkl` & `md_plot-0.2.0/md_plot/examples/StocksData2018Q1.gz.pkl`

 * *Files identical despite different names*

### Comparing `md_plot-0.1.9/md_plot/examples/UniformSample.gz.pkl` & `md_plot-0.2.0/md_plot/examples/UniformSample.gz.pkl`

 * *Files identical despite different names*

### Comparing `md_plot-0.1.9/md_plot/helper/bimodal.py` & `md_plot-0.2.0/md_plot/helper/bimodal.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,28 +62,29 @@
         
         # constants
         EPS = 1.5  # minimal Kruemmung > 0
         
         anz = len(x)
         
         ersteAbleitung = fx.diff().dropna() / x.diff().dropna()
-        ersteAbleitung = pd.Series([0]).append(ersteAbleitung)
+        ersteAbleitung = pd.concat([pd.Series([0]), ersteAbleitung])
         windowSize = 13
         ersteAbleitung = pd.Series(lfilter(np.repeat(1.0/windowSize, 
                                                      windowSize), 
                                            1, ersteAbleitung))
         
         secondDerivative = ersteAbleitung.diff().dropna() / x.diff().dropna()
-        secondDerivative = pd.Series([0]).append(secondDerivative)
+        
+        secondDerivative = pd.concat([pd.Series([0]), secondDerivative])
         windowSize = 15
         secondDerivative = pd.Series(lfilter(np.repeat(1.0/windowSize, 
                                                        windowSize), 
                                              1, secondDerivative))
         
-        Next = pd.Series([x for x in range(1, anz)]).append(pd.Series([anz-1]))
+        Next = pd.concat([pd.Series([x for x in range(1, anz)]), pd.Series([anz-1])])
         posOrNeg = x * 0
         posOrNeg[secondDerivative >  EPS] = 1
         posOrNeg[secondDerivative < -1 * EPS] = -1
         # NextIdentical is true if the next is on the same side
         nextIdentical = posOrNeg == posOrNeg[Next].reset_index(drop=True)
         posRuns = nextIdentical & (secondDerivative > EPS)
         negRuns =  nextIdentical & (secondDerivative < -1 * EPS)
```

### Comparing `md_plot-0.1.9/md_plot/helper/optimal_no_bins.py` & `md_plot-0.2.0/md_plot/helper/optimal_no_bins.py`

 * *Files identical despite different names*

### Comparing `md_plot-0.1.9/md_plot/helper/pareto_density_estimation.py` & `md_plot-0.2.0/md_plot/helper/pareto_density_estimation.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     # this data is at the lower edge
     lowData = data[data < (minData + paretoRadius)]
     lowR = 2 * minData - lowData
     # this data is at the upper edge
     upData = data[data > (maxData - paretoRadius)]
     upR = 2 * maxData - upData
     # extend data by mirrowing
-    dataPlus = data.append(lowR).append(upR)
+    dataPlus = pd.concat([data, lowR, upR])
     
     paretoDensity = []
     for fltKernel in kernels:
         lb = fltKernel - paretoRadius
         ub = fltKernel + paretoRadius
         dataTemp = dataPlus[(dataPlus >= lb) & (dataPlus <= ub)]
         paretoDensity.append(len(dataTemp))
```

### Comparing `md_plot-0.1.9/md_plot/helper/pareto_radius.py` & `md_plot-0.2.0/md_plot/helper/pareto_radius.py`

 * *Files identical despite different names*

### Comparing `md_plot-0.1.9/md_plot/helper/pretty.py` & `md_plot-0.2.0/md_plot/helper/pretty.py`

 * *Files identical despite different names*

### Comparing `md_plot-0.1.9/md_plot/helper/robust_normalization.py` & `md_plot-0.2.0/md_plot/helper/robust_normalization.py`

 * *Files identical despite different names*

### Comparing `md_plot-0.1.9/md_plot/helper/signed_log.py` & `md_plot-0.2.0/md_plot/helper/signed_log.py`

 * *Files identical despite different names*

### Comparing `md_plot-0.1.9/md_plot/helper/stat_pde_density.py` & `md_plot-0.2.0/md_plot/helper/stat_pde_density.py`

 * *Files identical despite different names*

### Comparing `md_plot-0.1.9/md_plot/load_examples.py` & `md_plot-0.2.0/md_plot/load_examples.py`

 * *Files identical despite different names*

### Comparing `md_plot-0.1.9/md_plot/md_plot.py` & `md_plot-0.2.0/md_plot/md_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 @author: tinog_000
 """
 
 import warnings
 import pandas as pd
 import numpy as np
 import plotnine as p9
-import unidip.dip as dip
 from pandas.api.types import is_numeric_dtype
 from scipy.stats.mstats import mquantiles
 from scipy.stats import norm, trim_mean, skewtest, kstest
 from .helper.robust_normalization import robust_normalization
 from .helper.signed_log import signed_log
 from .helper.bimodal import bimodal
 from .helper.stat_pde_density import stat_pde_density
+from .unidip import dip
 
 
 def MDplot(Data, Names=None, Ordering='Default', Scaling=None, 
            Fill='darkblue', RobustGaussian=True, GaussianColor='magenta', 
            Gaussian_lwd=1.5, BoxPlot=False, BoxColor='darkred', 
            MDscaling='width', LineColor='black', LineSize=0.01, 
            QuantityThreshold=40, UniqueValuesThreshold=12, 
@@ -164,16 +164,17 @@
         
         factor = pd.Series([0.25, 0.75]).apply(lambda x: abs(norm.ppf(x)))\
         .sum()
         std = Data.std()
         
         dfQuartile = Data.apply(lambda x: mquantiles(x, [0.25, 0.75], 
                                                      alphap=0.5, betap=0.5))
-        dfQuartile = dfQuartile.append(dfQuartile.loc[1] - dfQuartile.loc[0], 
-                                       ignore_index=True)
+        psIQR = dfQuartile.loc[1] - dfQuartile.loc[0]
+        dfIQR = pd.DataFrame([psIQR.values], columns=psIQR.index)
+        dfQuartile = pd.concat([dfQuartile, dfIQR])
         dfQuartile.index = ["low", "hi", "iqr"]
         dfMinMax = Data.apply(lambda x: mquantiles(x, [0.001, 0.999], 
                                                    alphap=0.5, betap=0.5))
         dfMinMax.index = ["min", "max"]
         
         shat = pd.Series()
         mhat = pd.Series()
```

### Comparing `md_plot-0.1.9/md_plot.egg-info/PKG-INFO` & `md_plot-0.2.0/md_plot.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: md-plot
-Version: 0.1.9
+Version: 0.2.0
 Summary: Draws a mirrored density plot for each input column
-Home-page: UNKNOWN
+Download-URL: https://github.com/TinoGehlert/md_plot/archive/v0.2.0.tar.gz
 Author: TinoGehlert
 Author-email: tinogehlert@aol.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/TinoGehlert/md_plot/archive/v0.1.9.tar.gz
 Project-URL: R-Version, https://cran.r-project.org/web/packages/DataVisualizations/index.html
 Project-URL: Source, https://github.com/TinoGehlert/md_plot
 Project-URL: Docs, https://md-plot.readthedocs.io
-Description: Mirrored Density Plot
-        =====================
-        
-        This function creates a MD-plot for each column of the dataframe. The MD-plot is a visualization
-        for a boxplot-like Shape of the PDF published in [Thrun/Ultsch, 2019]. It is an improvement of
-        violin or so-called bean plots and posses advantages in comparison to the conventional well-known
-        box plot [Thrun/Ultsch, 2019]. This is the Python implementation of the function MD-Plot contained 
-        in R package [DataVisualizations](https://cran.r-project.org/web/packages/DataVisualizations/index.html)
-        
-        Basic Usage
-        ^^^^^^^^^^^
-        
-        from md_plot import MDplot, load_examples
-        
-        dctExamples = load_examples()
-        
-        MDplot(dctExamples["BimodalArtificial"])
-        
 Keywords: data_science violin density_plot
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
+License-File: LICENSE.txt
+
+Mirrored Density Plot
+=====================
+
+This function creates a MD-plot for each column of the dataframe. The MD-plot is a visualization
+for a boxplot-like Shape of the PDF published in [Thrun/Ultsch, 2019]. It is an improvement of
+violin or so-called bean plots and posses advantages in comparison to the conventional well-known
+box plot [Thrun/Ultsch, 2019]. This is the Python implementation of the function MD-Plot contained 
+in R package [DataVisualizations](https://cran.r-project.org/web/packages/DataVisualizations/index.html)
+
+Basic Usage
+^^^^^^^^^^^
+
+from md_plot import MDplot, load_examples
+
+dctExamples = load_examples()
+
+MDplot(dctExamples["BimodalArtificial"])
```

### Comparing `md_plot-0.1.9/setup.py` & `md_plot-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 
 setup(name='md_plot',
-      version='0.1.9',
+      version='0.2.0',
       project_urls={'R-Version': 'https://cran.r-project.org/web/packages/DataVisualizations/index.html', 
                     'Source': 'https://github.com/TinoGehlert/md_plot', 
                     'Docs': 'https://md-plot.readthedocs.io'},
       description='Draws a mirrored density plot for each input column',
       long_description=open('readme_pypi.rst').read(),
-      download_url='https://github.com/TinoGehlert/md_plot/archive/v0.1.9.tar.gz',
+      download_url='https://github.com/TinoGehlert/md_plot/archive/v0.2.0.tar.gz',
       classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
@@ -25,11 +25,10 @@
       packages=find_packages(),
       install_requires=[
           'pandas>=0.24.2',
           'numpy>=1.16',
           'scipy>=1.1.0',
           'matplotlib>=3.1.0',
           'plotnine>=0.5.1',
-          'unidip>=0.1.1'
       ],
       include_package_data=True,
       zip_safe=False)
```

