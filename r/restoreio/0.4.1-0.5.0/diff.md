# Comparing `tmp/restoreio-0.4.1.tar.gz` & `tmp/restoreio-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "restoreio-0.4.1.tar", last modified: Wed Jun 14 02:30:43 2023, max compression
+gzip compressed data, was "restoreio-0.5.0.tar", last modified: Sat Jul  1 20:06:58 2023, max compression
```

## Comparing `restoreio-0.4.1.tar` & `restoreio-0.5.0.tar`

### file list

```diff
@@ -1,190 +1,191 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.935131 restoreio-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-14 02:30:14.000000 restoreio-0.4.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-14 02:30:14.000000 restoreio-0.4.1/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-14 02:30:14.000000 restoreio-0.4.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-14 02:30:14.000000 restoreio-0.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-14 02:30:14.000000 restoreio-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-06-14 02:30:43.935131 restoreio-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-06-14 02:30:14.000000 restoreio-0.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.915131 restoreio-0.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.919131 restoreio-0.4.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_inspect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.915131 restoreio-0.4.1/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.915131 restoreio-0.4.1/docs/source/_static/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.919131 restoreio-0.4.1/docs/source/_static/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   108412 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/assets/fonts/synconew.regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    65432 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/assets/fonts/syncopate.bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   141308 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/assets/fonts/syncopate.regular.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.919131 restoreio-0.4.1/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/css/custom-anaconda-doc.css
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/css/custom-pydata.css
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.915131 restoreio-0.4.1/docs/source/_static/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.919131 restoreio-0.4.1/docs/source/_static/images/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/images/icons/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/images/icons/logo-anaconda.ico
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/images/icons/logo-anaconda.png
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/images/icons/logo-anaconda.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/images/icons/logo-pypi.ico
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/images/icons/logo-pypi.png
--rw-r--r--   0 runner    (1001) docker     (123)    70855 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/images/icons/logo-pypi.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/images/icons/logo-restoreio-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    26103 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/images/icons/logo-restoreio-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14098 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/images/icons/logo-restoreio-light.png
--rw-r--r--   0 runner    (1001) docker     (123)    26102 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/images/icons/logo-restoreio-light.svg
--rw-r--r--   0 runner    (1001) docker     (123)    22771 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/images/icons/logo-traceflows-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    23221 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/images/icons/logo-traceflows-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)    23601 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/images/icons/logo-traceflows-light.png
--rw-r--r--   0 runner    (1001) docker     (123)    23223 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/images/icons/logo-traceflows-light.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.923131 restoreio-0.4.1/docs/source/_static/images/plots/
--rw-r--r--   0 runner    (1001) docker     (123)  1078579 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/images/plots/cor_cov.png
--rw-r--r--   0 runner    (1001) docker     (123)   386357 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/images/plots/deviation.png
--rw-r--r--   0 runner    (1001) docker     (123)   419634 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/images/plots/ensembles.png
--rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/images/plots/ensembles_js_distance.png
--rw-r--r--   0 runner    (1001) docker     (123)   792928 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/images/plots/gdop_coverage.png
--rw-r--r--   0 runner    (1001) docker     (123)   130012 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/images/plots/js_distance.png
--rw-r--r--   0 runner    (1001) docker     (123)   107758 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/images/plots/kl_eigenvalues.png
--rw-r--r--   0 runner    (1001) docker     (123)   541932 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/images/plots/kl_eigenvectors.png
--rw-r--r--   0 runner    (1001) docker     (123)   290207 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/images/plots/orig_vel_and_error.png
--rw-r--r--   0 runner    (1001) docker     (123)   267216 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/images/plots/rbf_kernel_2d.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.927131 restoreio-0.4.1/docs/source/_static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_static/js/custom-pydata.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.927131 restoreio-0.4.1/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.927131 restoreio-0.4.1/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_templates/autosummary/attribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_templates/autosummary/method.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_templates/autosummary/ndarray_subclass.rst
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_templates/autosummary/property.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_templates/sidebar-nav-bs.html
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/_templates/version.html
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/cite.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/cli_restore.rst
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/cli_scan.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/contents.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/custom_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.927131 restoreio-0.4.1/docs/source/generated/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/generated/restoreio.restore.rst
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/generated/restoreio.scan.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/install.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.927131 restoreio-0.4.1/docs/source/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/notebooks/quick_start.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-14 02:30:14.000000 restoreio-0.4.1/docs/source/recursive_glob.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-14 02:30:14.000000 restoreio-0.4.1/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.915131 restoreio-0.4.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.927131 restoreio-0.4.1/examples/restore/
--rwxr-xr-x   0 runner    (1001) docker     (123)    30256 2023-06-14 02:30:14.000000 restoreio-0.4.1/examples/restore/main_VaryingNumModes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7838 2023-06-14 02:30:14.000000 restoreio-0.4.1/examples/restore/plot_coverage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21626 2023-06-14 02:30:14.000000 restoreio-0.4.1/examples/restore/plot_fixed_size_artificial_mask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23405 2023-06-14 02:30:14.000000 restoreio-0.4.1/examples/restore/plot_variable_d_artificial_masks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21770 2023-06-14 02:30:14.000000 restoreio-0.4.1/examples/restore/plot_variable_size_artificial_masks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.927131 restoreio-0.4.1/examples/uncertainty_quant/
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-14 02:30:14.000000 restoreio-0.4.1/examples/uncertainty_quant/_display_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-06-14 02:30:14.000000 restoreio-0.4.1/examples/uncertainty_quant/_draw_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-06-14 02:30:14.000000 restoreio-0.4.1/examples/uncertainty_quant/_plot_utilities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16132 2023-06-14 02:30:14.000000 restoreio-0.4.1/examples/uncertainty_quant/plot_gdop_coverage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6715 2023-06-14 02:30:14.000000 restoreio-0.4.1/examples/uncertainty_quant/plot_js_divergence.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-14 02:30:14.000000 restoreio-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-14 02:30:14.000000 restoreio-0.4.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.927131 restoreio-0.4.1/restoreio/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24450 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.927131 restoreio-0.4.1/restoreio/_file_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_file_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_file_utilities/file_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.927131 restoreio-0.4.1/restoreio/_geography/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_geography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_geography/_find_alpha_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_geography/create_mask_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_geography/detect_land_ocean.py
--rw-r--r--   0 runner    (1001) docker     (123)    24845 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_geography/locate_missing_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.931131 restoreio-0.4.1/restoreio/_inpaint/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_inpaint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_inpaint/_cast_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_inpaint/_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_inpaint/_plot_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_inpaint/inpaint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.931131 restoreio-0.4.1/restoreio/_input_output/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_input_output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_input_output/get_datetime_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_input_output/load_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_input_output/load_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_input_output/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.931131 restoreio-0.4.1/restoreio/_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_parser/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_parser/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16625 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_parser/parse_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.931131 restoreio-0.4.1/restoreio/_plots/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_plots/_display_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_plots/_draw_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_plots/_plot_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_plots/_plot_quiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_plots/_plot_streamlines.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_plots/_plot_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_plots/_plot_velocities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_plots/plot_results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.931131 restoreio-0.4.1/restoreio/_plots_uq/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_plots_uq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_plots_uq/_refine_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_plots_uq/_shifted_colormap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_plots_uq/plot_auto_correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_plots_uq/plot_convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_plots_uq/plot_cor_cov.py
--rw-r--r--   0 runner    (1001) docker     (123)    26594 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_plots_uq/plot_ensembles_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_plots_uq/plot_kl_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_plots_uq/plot_rbf_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.931131 restoreio-0.4.1/restoreio/_restore/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_restore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_restore/_make_array_masked.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_restore/refine_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    15310 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_restore/restore_generated_ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)     9359 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_restore/restore_main_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.931131 restoreio-0.4.1/restoreio/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_scripts/examples.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    44295 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_scripts/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.931131 restoreio-0.4.1/restoreio/_server_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_server_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_server_utils/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_server_utils/terminate_with_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.935131 restoreio-0.4.1/restoreio/_subset/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_subset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_subset/_array_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_subset/subset_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_subset/subset_domain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.935131 restoreio-0.4.1/restoreio/_uncertainty_quant/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_uncertainty_quant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_uncertainty_quant/_compute_correlation_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    18404 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_uncertainty_quant/_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_uncertainty_quant/_statistical_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)    17915 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_uncertainty_quant/generate_image_ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)    11072 2023-06-14 02:30:14.000000 restoreio-0.4.1/restoreio/_uncertainty_quant/get_ensembles_stat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.927131 restoreio-0.4.1/restoreio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-06-14 02:30:43.000000 restoreio-0.4.1/restoreio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-14 02:30:43.000000 restoreio-0.4.1/restoreio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 02:30:43.000000 restoreio-0.4.1/restoreio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-14 02:30:43.000000 restoreio-0.4.1/restoreio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 02:30:43.000000 restoreio-0.4.1/restoreio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-14 02:30:43.000000 restoreio-0.4.1/restoreio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-14 02:30:43.000000 restoreio-0.4.1/restoreio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-14 02:30:43.935131 restoreio-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-06-14 02:30:14.000000 restoreio-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:30:43.935131 restoreio-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-14 02:30:14.000000 restoreio-0.4.1/tests/test_restore_local_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-14 02:30:14.000000 restoreio-0.4.1/tests/test_restore_remote_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-14 02:30:14.000000 restoreio-0.4.1/tests/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-14 02:30:14.000000 restoreio-0.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.984282 restoreio-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-01 20:06:40.000000 restoreio-0.5.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-01 20:06:40.000000 restoreio-0.5.0/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-01 20:06:40.000000 restoreio-0.5.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-01 20:06:40.000000 restoreio-0.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-01 20:06:40.000000 restoreio-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-07-01 20:06:58.984282 restoreio-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-07-01 20:06:40.000000 restoreio-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.968282 restoreio-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.968282 restoreio-0.5.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_inspect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.968282 restoreio-0.5.0/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.968282 restoreio-0.5.0/docs/source/_static/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.972282 restoreio-0.5.0/docs/source/_static/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   108412 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/assets/fonts/synconew.regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    65432 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/assets/fonts/syncopate.bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   141308 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/assets/fonts/syncopate.regular.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.972282 restoreio-0.5.0/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/css/custom-anaconda-doc.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/css/custom-pydata.css
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.968282 restoreio-0.5.0/docs/source/_static/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.972282 restoreio-0.5.0/docs/source/_static/images/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/logo-anaconda.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/logo-anaconda.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/logo-anaconda.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/logo-pypi.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/logo-pypi.png
+-rw-r--r--   0 runner    (1001) docker     (123)    70855 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/logo-pypi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/logo-restoreio-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26103 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/logo-restoreio-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14098 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/logo-restoreio-light.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26102 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/logo-restoreio-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22771 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/logo-traceflows-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23221 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/logo-traceflows-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    23601 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/logo-traceflows-light.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23223 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/logo-traceflows-light.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.976282 restoreio-0.5.0/docs/source/_static/images/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)  1078579 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/plots/cor_cov.png
+-rw-r--r--   0 runner    (1001) docker     (123)   386357 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/plots/deviation.png
+-rw-r--r--   0 runner    (1001) docker     (123)   419634 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/plots/ensembles.png
+-rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/plots/ensembles_js_distance.png
+-rw-r--r--   0 runner    (1001) docker     (123)   792928 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/plots/gdop_coverage.png
+-rw-r--r--   0 runner    (1001) docker     (123)   130012 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/plots/js_distance.png
+-rw-r--r--   0 runner    (1001) docker     (123)   107758 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/plots/kl_eigenvalues.png
+-rw-r--r--   0 runner    (1001) docker     (123)   541932 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/plots/kl_eigenvectors.png
+-rw-r--r--   0 runner    (1001) docker     (123)   290207 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/plots/orig_vel_and_error.png
+-rw-r--r--   0 runner    (1001) docker     (123)   267216 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/plots/rbf_kernel_2d.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.976282 restoreio-0.5.0/docs/source/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/js/custom-pydata.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.976282 restoreio-0.5.0/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.976282 restoreio-0.5.0/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_templates/autosummary/attribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_templates/autosummary/method.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_templates/autosummary/ndarray_subclass.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_templates/autosummary/property.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_templates/sidebar-nav-bs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_templates/version.html
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/cite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/cli_restore.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/cli_scan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/contents.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/custom_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.976282 restoreio-0.5.0/docs/source/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/generated/restoreio.restore.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/generated/restoreio.scan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/install.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.976282 restoreio-0.5.0/docs/source/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/notebooks/quick_start.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/recursive_glob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-01 20:06:40.000000 restoreio-0.5.0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.968282 restoreio-0.5.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.980282 restoreio-0.5.0/examples/restore/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30256 2023-07-01 20:06:40.000000 restoreio-0.5.0/examples/restore/main_VaryingNumModes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7838 2023-07-01 20:06:40.000000 restoreio-0.5.0/examples/restore/plot_coverage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21626 2023-07-01 20:06:40.000000 restoreio-0.5.0/examples/restore/plot_fixed_size_artificial_mask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23405 2023-07-01 20:06:40.000000 restoreio-0.5.0/examples/restore/plot_variable_d_artificial_masks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21771 2023-07-01 20:06:40.000000 restoreio-0.5.0/examples/restore/plot_variable_size_artificial_masks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.980282 restoreio-0.5.0/examples/uncertainty_quant/
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-01 20:06:40.000000 restoreio-0.5.0/examples/uncertainty_quant/_display_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-07-01 20:06:40.000000 restoreio-0.5.0/examples/uncertainty_quant/_draw_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-07-01 20:06:40.000000 restoreio-0.5.0/examples/uncertainty_quant/_plot_utilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16132 2023-07-01 20:06:40.000000 restoreio-0.5.0/examples/uncertainty_quant/plot_gdop_coverage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6715 2023-07-01 20:06:40.000000 restoreio-0.5.0/examples/uncertainty_quant/plot_js_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-01 20:06:40.000000 restoreio-0.5.0/examples/uncertainty_quant/restoreio_mwe.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-01 20:06:40.000000 restoreio-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-01 20:06:40.000000 restoreio-0.5.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.980282 restoreio-0.5.0/restoreio/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24450 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.980282 restoreio-0.5.0/restoreio/_file_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_file_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_file_utilities/file_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.980282 restoreio-0.5.0/restoreio/_geography/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_geography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_geography/_find_alpha_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_geography/create_mask_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_geography/detect_land_ocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24845 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_geography/locate_missing_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.980282 restoreio-0.5.0/restoreio/_inpaint/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_inpaint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_inpaint/_cast_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_inpaint/_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_inpaint/_plot_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_inpaint/inpaint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.980282 restoreio-0.5.0/restoreio/_input_output/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_input_output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_input_output/get_datetime_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_input_output/load_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_input_output/load_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_input_output/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.980282 restoreio-0.5.0/restoreio/_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_parser/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_parser/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16639 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_parser/parse_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.980282 restoreio-0.5.0/restoreio/_plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots/_display_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots/_draw_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots/_plot_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots/_plot_quiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots/_plot_streamlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots/_plot_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots/_plot_velocities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots/plot_results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.984282 restoreio-0.5.0/restoreio/_plots_uq/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots_uq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots_uq/_refine_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots_uq/_shifted_colormap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots_uq/plot_auto_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots_uq/plot_convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots_uq/plot_cor_cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26594 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots_uq/plot_ensembles_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots_uq/plot_kl_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots_uq/plot_rbf_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.984282 restoreio-0.5.0/restoreio/_restore/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_restore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_restore/_make_array_masked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_restore/refine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_restore/restore_generated_ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9359 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_restore/restore_main_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.984282 restoreio-0.5.0/restoreio/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_scripts/examples.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    44360 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_scripts/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.984282 restoreio-0.5.0/restoreio/_server_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_server_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_server_utils/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_server_utils/terminate_with_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.984282 restoreio-0.5.0/restoreio/_subset/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_subset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_subset/_array_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_subset/subset_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_subset/subset_domain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.984282 restoreio-0.5.0/restoreio/_uncertainty_quant/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_uncertainty_quant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_uncertainty_quant/_compute_correlation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18404 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_uncertainty_quant/_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_uncertainty_quant/_statistical_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17931 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_uncertainty_quant/generate_image_ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11072 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_uncertainty_quant/get_ensembles_stat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.980282 restoreio-0.5.0/restoreio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-07-01 20:06:58.000000 restoreio-0.5.0/restoreio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-07-01 20:06:58.000000 restoreio-0.5.0/restoreio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 20:06:58.000000 restoreio-0.5.0/restoreio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-01 20:06:58.000000 restoreio-0.5.0/restoreio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 20:06:58.000000 restoreio-0.5.0/restoreio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-01 20:06:58.000000 restoreio-0.5.0/restoreio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 20:06:58.000000 restoreio-0.5.0/restoreio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-01 20:06:58.984282 restoreio-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-07-01 20:06:40.000000 restoreio-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.984282 restoreio-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-07-01 20:06:40.000000 restoreio-0.5.0/tests/test_restore_local_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-01 20:06:40.000000 restoreio-0.5.0/tests/test_restore_remote_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-01 20:06:40.000000 restoreio-0.5.0/tests/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-01 20:06:40.000000 restoreio-0.5.0/tox.ini
```

### Comparing `restoreio-0.4.1/LICENSE.txt` & `restoreio-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/MANIFEST.in` & `restoreio-0.5.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/PKG-INFO` & `restoreio-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restoreio
-Version: 0.4.1
+Version: 0.5.0
 Summary: Reconstruct incomplete oceanographic dataset
 Home-page: https://github.com/ameli/restoreio
 Download-URL: https://github.com/ameli/restoreio/archive/main.zip
 Author: Siavash Ameli
 Author-email: sameli@berkeley.edu
 Project-URL: Documentation, https://github.com/ameli/restoreio/blob/main/README.rst
 Project-URL: Source, https://github.com/ameli/restoreio
@@ -39,20 +39,20 @@
 
 ******
 |logo|
 ******
 
 ``restoreio`` is a Python package to **Restore** **I**\ ncomplete **O**\ ceanographic dataset.
 
-``restoreio`` can be installed and used as a standalone Python package or in your browser through the `online gateway interface <http://transport.me.berkeley.edu/restore>`__.
+``restoreio`` can be installed and used as a standalone Python package or in your browser through the `online gateway interface <https://transport.me.berkeley.edu/restore>`__.
 
 Links
 =====
 
-* `Online Gateway <http://transport.me.berkeley.edu/restore>`_
+* `Online Gateway <https://transport.me.berkeley.edu/restore>`_
 * `Documentation <https://ameli.github.io/restoreio>`_
 * `PyPI <https://pypi.org/project/restoreio/>`_
 * `Anaconda <https://anaconda.org/s-ameli/restoreio>`_
 * `Git Hub <https://github.com/ameli/restoreio>`_
 
 Install
 =======
```

### Comparing `restoreio-0.4.1/README.rst` & `restoreio-0.5.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ******
 |logo|
 ******
 
 ``restoreio`` is a Python package to **Restore** **I**\ ncomplete **O**\ ceanographic dataset.
 
-``restoreio`` can be installed and used as a standalone Python package or in your browser through the `online gateway interface <http://transport.me.berkeley.edu/restore>`__.
+``restoreio`` can be installed and used as a standalone Python package or in your browser through the `online gateway interface <https://transport.me.berkeley.edu/restore>`__.
 
 Links
 =====
 
-* `Online Gateway <http://transport.me.berkeley.edu/restore>`_
+* `Online Gateway <https://transport.me.berkeley.edu/restore>`_
 * `Documentation <https://ameli.github.io/restoreio>`_
 * `PyPI <https://pypi.org/project/restoreio/>`_
 * `Anaconda <https://anaconda.org/s-ameli/restoreio>`_
 * `Git Hub <https://github.com/ameli/restoreio>`_
 
 Install
 =======
```

### Comparing `restoreio-0.4.1/docs/Makefile` & `restoreio-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/make.bat` & `restoreio-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_inspect.py` & `restoreio-0.5.0/docs/source/_inspect.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/assets/fonts/synconew.regular.ttf` & `restoreio-0.5.0/docs/source/_static/assets/fonts/synconew.regular.ttf`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/assets/fonts/syncopate.bold.ttf` & `restoreio-0.5.0/docs/source/_static/assets/fonts/syncopate.bold.ttf`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/assets/fonts/syncopate.regular.ttf` & `restoreio-0.5.0/docs/source/_static/assets/fonts/syncopate.regular.ttf`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/css/custom-anaconda-doc.css` & `restoreio-0.5.0/docs/source/_static/css/custom-anaconda-doc.css`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/css/custom-pydata.css` & `restoreio-0.5.0/docs/source/_static/css/custom-pydata.css`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/css/custom.css` & `restoreio-0.5.0/docs/source/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/images/icons/favicon.ico` & `restoreio-0.5.0/docs/source/_static/images/icons/favicon.ico`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/images/icons/logo-anaconda.ico` & `restoreio-0.5.0/docs/source/_static/images/icons/logo-anaconda.ico`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/images/icons/logo-anaconda.png` & `restoreio-0.5.0/docs/source/_static/images/icons/logo-anaconda.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/images/icons/logo-anaconda.svg` & `restoreio-0.5.0/docs/source/_static/images/icons/logo-anaconda.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/images/icons/logo-pypi.ico` & `restoreio-0.5.0/docs/source/_static/images/icons/logo-pypi.ico`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/images/icons/logo-pypi.png` & `restoreio-0.5.0/docs/source/_static/images/icons/logo-pypi.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/images/icons/logo-pypi.svg` & `restoreio-0.5.0/docs/source/_static/images/icons/logo-pypi.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/images/icons/logo-restoreio-dark.png` & `restoreio-0.5.0/docs/source/_static/images/icons/logo-restoreio-dark.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/images/icons/logo-restoreio-dark.svg` & `restoreio-0.5.0/docs/source/_static/images/icons/logo-restoreio-dark.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/images/icons/logo-restoreio-light.png` & `restoreio-0.5.0/docs/source/_static/images/icons/logo-restoreio-light.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/images/icons/logo-restoreio-light.svg` & `restoreio-0.5.0/docs/source/_static/images/icons/logo-restoreio-light.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/images/icons/logo-traceflows-dark.png` & `restoreio-0.5.0/docs/source/_static/images/icons/logo-traceflows-dark.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/images/icons/logo-traceflows-dark.svg` & `restoreio-0.5.0/docs/source/_static/images/icons/logo-traceflows-dark.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/images/icons/logo-traceflows-light.png` & `restoreio-0.5.0/docs/source/_static/images/icons/logo-traceflows-light.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/images/icons/logo-traceflows-light.svg` & `restoreio-0.5.0/docs/source/_static/images/icons/logo-traceflows-light.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/images/plots/cor_cov.png` & `restoreio-0.5.0/docs/source/_static/images/plots/cor_cov.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/images/plots/deviation.png` & `restoreio-0.5.0/docs/source/_static/images/plots/deviation.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/images/plots/ensembles.png` & `restoreio-0.5.0/docs/source/_static/images/plots/ensembles.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/images/plots/ensembles_js_distance.png` & `restoreio-0.5.0/docs/source/_static/images/plots/ensembles_js_distance.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/images/plots/gdop_coverage.png` & `restoreio-0.5.0/docs/source/_static/images/plots/gdop_coverage.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/images/plots/js_distance.png` & `restoreio-0.5.0/docs/source/_static/images/plots/js_distance.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/images/plots/kl_eigenvalues.png` & `restoreio-0.5.0/docs/source/_static/images/plots/kl_eigenvalues.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/images/plots/kl_eigenvectors.png` & `restoreio-0.5.0/docs/source/_static/images/plots/kl_eigenvectors.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/images/plots/orig_vel_and_error.png` & `restoreio-0.5.0/docs/source/_static/images/plots/orig_vel_and_error.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/images/plots/rbf_kernel_2d.png` & `restoreio-0.5.0/docs/source/_static/images/plots/rbf_kernel_2d.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_static/js/custom-pydata.js` & `restoreio-0.5.0/docs/source/_static/js/custom-pydata.js`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_templates/autosummary/class.rst` & `restoreio-0.5.0/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_templates/layout.html` & `restoreio-0.5.0/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/_templates/version.html` & `restoreio-0.5.0/docs/source/_templates/version.html`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/cite.rst` & `restoreio-0.5.0/docs/source/cite.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/conf.py` & `restoreio-0.5.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/custom_domain.py` & `restoreio-0.5.0/docs/source/custom_domain.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/examples.rst` & `restoreio-0.5.0/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/index.rst` & `restoreio-0.5.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/install.rst` & `restoreio-0.5.0/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/notebooks/quick_start.ipynb` & `restoreio-0.5.0/docs/source/notebooks/quick_start.ipynb`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/docs/source/recursive_glob.py` & `restoreio-0.5.0/docs/source/recursive_glob.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/examples/restore/main_VaryingNumModes.py` & `restoreio-0.5.0/examples/restore/main_VaryingNumModes.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/examples/restore/plot_coverage.py` & `restoreio-0.5.0/examples/restore/plot_coverage.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/examples/restore/plot_fixed_size_artificial_mask.py` & `restoreio-0.5.0/examples/restore/plot_fixed_size_artificial_mask.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/examples/restore/plot_variable_d_artificial_masks.py` & `restoreio-0.5.0/examples/restore/plot_variable_d_artificial_masks.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/examples/restore/plot_variable_size_artificial_masks.py` & `restoreio-0.5.0/examples/restore/plot_variable_size_artificial_masks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python
 
 """
 Example:
-./plot_variable_size_artificial_masks.py -i http://transport.me.berkeley.edu/thredds/dodsC/root/WHOI-HFR/WHOI_HFR_2014_original.nc -o ~/Desktop/output.nc -L 0 -d 5 -s -c -t 46
+./plot_variable_size_artificial_masks.py -i https://transport.me.berkeley.edu/thredds/dodsC/root/WHOI-HFR/WHOI_HFR_2014_original.nc -o ~/Desktop/output.nc -L 0 -d 5 -s -c -t 46
 """
 
 # =======
 # Imports
 # =======
 
 import numpy
```

### Comparing `restoreio-0.4.1/examples/uncertainty_quant/_display_utilities.py` & `restoreio-0.5.0/examples/uncertainty_quant/_display_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/examples/uncertainty_quant/_draw_map.py` & `restoreio-0.5.0/examples/uncertainty_quant/_draw_map.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/examples/uncertainty_quant/_plot_utilities.py` & `restoreio-0.5.0/examples/uncertainty_quant/_plot_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/examples/uncertainty_quant/plot_gdop_coverage.py` & `restoreio-0.5.0/examples/uncertainty_quant/plot_gdop_coverage.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/examples/uncertainty_quant/plot_js_divergence.py` & `restoreio-0.5.0/examples/uncertainty_quant/plot_js_divergence.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/__main__.py` & `restoreio-0.5.0/restoreio/__main__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_file_utilities/__init__.py` & `restoreio-0.5.0/restoreio/_file_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_file_utilities/file_utilities.py` & `restoreio-0.5.0/restoreio/_file_utilities/file_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_geography/__init__.py` & `restoreio-0.5.0/restoreio/_geography/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_geography/_find_alpha_shapes.py` & `restoreio-0.5.0/restoreio/_geography/_find_alpha_shapes.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_geography/create_mask_info.py` & `restoreio-0.5.0/restoreio/_geography/create_mask_info.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_geography/detect_land_ocean.py` & `restoreio-0.5.0/restoreio/_geography/detect_land_ocean.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_geography/locate_missing_data.py` & `restoreio-0.5.0/restoreio/_geography/locate_missing_data.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_inpaint/_cast_types.py` & `restoreio-0.5.0/restoreio/_inpaint/_cast_types.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_inpaint/_image.py` & `restoreio-0.5.0/restoreio/_inpaint/_image.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_inpaint/_plot_image.py` & `restoreio-0.5.0/restoreio/_inpaint/_plot_image.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_inpaint/inpaint.py` & `restoreio-0.5.0/restoreio/_inpaint/inpaint.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_input_output/__init__.py` & `restoreio-0.5.0/restoreio/_input_output/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_input_output/get_datetime_info.py` & `restoreio-0.5.0/restoreio/_input_output/get_datetime_info.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_input_output/load_dataset.py` & `restoreio-0.5.0/restoreio/_input_output/load_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
         except BaseException as error:
             print('ERROR: Can not read local ncml file: ' + filename)
             raise error
 
         return agg
 
-    elif file_extension in ['.nc', '.ncd', '.nc.gz']:
+    elif file_extension in ['.nc', '.nc4', '.ncd', '.nc.gz']:
 
         try:
             nc = netCDF4.Dataset(filename)
         except BaseException as error:
             print('ERROR: Can not read local netcdf file: ' + filename)
             raise error
 
@@ -114,19 +114,19 @@
         file_extension = os.path.splitext(url[:-3])[1]
 
     # Note that some opendap urls do not even have a file extension
     if file_extension != "":
 
         # If a file extension exists, check if it is a standard netcdf file
         if file_extension not in \
-                ['.nc', '.ncd', '.nc.gz', '.ncml', '.ncml.gz']:
+                ['.nc', '.nc4', '.ncd', '.nc.gz', '.ncml', '.ncml.gz']:
             terminate_with_error(
                 'The input data URL is not an netcdf file. The URL should ' +
-                'end with ".nc", ".ncd", ".nc.gz", ".ncml", ".ncml.gz", or ' +
-                'without file extension.')
+                'end with ".nc", ".nc4", ".ncd", ".nc.gz", ".ncml", ' +
+                '".ncml.gz", or without file extension.')
 
     try:
 
         # nc = open_url(url)
         nc = netCDF4.Dataset(url)
 
     except OSError:
```

### Comparing `restoreio-0.4.1/restoreio/_input_output/load_variables.py` & `restoreio-0.5.0/restoreio/_input_output/load_variables.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_input_output/writer.py` & `restoreio-0.5.0/restoreio/_input_output/writer.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_parser/examples.py` & `restoreio-0.5.0/restoreio/_parser/examples.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_parser/formatter.py` & `restoreio-0.5.0/restoreio/_parser/formatter.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_parser/parse_arguments.py` & `restoreio-0.5.0/restoreio/_parser/parse_arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,16 @@
                           help='show this help message and exit')
 
     # Input filename
     help_input = """
     Input filename. This can be either the path to a local file or the URL to
     a remote dataset. The file or URL may or may not have a file extension.
     However, if the file does have an extension, the file extension should be
-    either ``.nc``, ``.ncd``, ``.nc.gz``, ``.ncml``, or ``*.ncml.gz`` only.
+    either ``.nc``, ``.nc4``, ``.ncd``, ``.nc.gz``, ``.ncml``, or ``*.ncml.gz``
+    only.
     """
     required.add_argument('-i', type=str, help=help_input, metavar='INPUT',
                           required=True)
 
     # Output filename
     help_output = """
     Output filename. This can be either the path to a local file or the URL to
```

### Comparing `restoreio-0.4.1/restoreio/_plots/_display_utilities.py` & `restoreio-0.5.0/restoreio/_plots/_display_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_plots/_draw_map.py` & `restoreio-0.5.0/restoreio/_plots/_draw_map.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_plots/_plot_grid.py` & `restoreio-0.5.0/restoreio/_plots/_plot_grid.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_plots/_plot_quiver.py` & `restoreio-0.5.0/restoreio/_plots/_plot_quiver.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_plots/_plot_streamlines.py` & `restoreio-0.5.0/restoreio/_plots/_plot_streamlines.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_plots/_plot_utilities.py` & `restoreio-0.5.0/restoreio/_plots/_plot_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_plots/_plot_velocities.py` & `restoreio-0.5.0/restoreio/_plots/_plot_velocities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_plots/plot_results.py` & `restoreio-0.5.0/restoreio/_plots/plot_results.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_plots_uq/__init__.py` & `restoreio-0.5.0/restoreio/_plots_uq/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_plots_uq/_refine_mask.py` & `restoreio-0.5.0/restoreio/_plots_uq/_refine_mask.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_plots_uq/_shifted_colormap.py` & `restoreio-0.5.0/restoreio/_plots_uq/_shifted_colormap.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_plots_uq/plot_auto_correlation.py` & `restoreio-0.5.0/restoreio/_plots_uq/plot_auto_correlation.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_plots_uq/plot_convergence.py` & `restoreio-0.5.0/restoreio/_plots_uq/plot_convergence.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_plots_uq/plot_cor_cov.py` & `restoreio-0.5.0/restoreio/_plots_uq/plot_cor_cov.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_plots_uq/plot_ensembles_stat.py` & `restoreio-0.5.0/restoreio/_plots_uq/plot_ensembles_stat.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_plots_uq/plot_kl_transform.py` & `restoreio-0.5.0/restoreio/_plots_uq/plot_kl_transform.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_plots_uq/plot_rbf_kernel.py` & `restoreio-0.5.0/restoreio/_plots_uq/plot_rbf_kernel.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py` & `restoreio-0.5.0/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_restore/__init__.py` & `restoreio-0.5.0/restoreio/_restore/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_restore/_make_array_masked.py` & `restoreio-0.5.0/restoreio/_restore/_make_array_masked.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_restore/refine_grid.py` & `restoreio-0.5.0/restoreio/_restore/refine_grid.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_restore/restore_generated_ensembles.py` & `restoreio-0.5.0/restoreio/_restore/restore_generated_ensembles.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,14 +374,15 @@
                 V_one_time,
                 U_error_one_time,
                 V_error_one_time,
                 U_all_ensembles_inpainted,
                 V_all_ensembles_inpainted,
                 U_all_ensembles_inpainted_stats,
                 V_all_ensembles_inpainted_stats,
+                save=save,
                 verbose=verbose)
 
     U_all_ensembles_inpainted_mean = U_all_ensembles_inpainted_stats['Mean']
     V_all_ensembles_inpainted_mean = V_all_ensembles_inpainted_stats['Mean']
     U_all_ensembles_inpainted_std = U_all_ensembles_inpainted_stats['STD']
     V_all_ensembles_inpainted_std = V_all_ensembles_inpainted_stats['STD']
```

### Comparing `restoreio-0.4.1/restoreio/_restore/restore_main_ensemble.py` & `restoreio-0.5.0/restoreio/_restore/restore_main_ensemble.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_scripts/examples.py` & `restoreio-0.5.0/restoreio/_scripts/examples.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_scripts/scan.py` & `restoreio-0.5.0/restoreio/_scripts/scan.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,16 @@
                           help='show this help message and exit')
 
     # Input filename
     help_input = """
     Input filename. This can be either the path to a local file or the URL to
     a remote dataset. The file or URL may or may not have a file extension.
     However, if the file does have an extension, the file extension should be
-    either ``.nc``, ``.ncd``, ``.nc.gz``, ``.ncml``, or ``*.ncml.gz`` only.
+    either ``.nc``, ``.nc4``, ``.ncd``, ``.nc.gz``, ``.ncml``, or ``*.ncml.gz``
+    only.
     """
     required.add_argument('-i', type=str, help=help_input, metavar='INPUT',
                           required=True)
 
     # Scan velocity
     help_scan_velocity = """
     Scans the velocity arrays of the file. This is useful to find the min and
@@ -201,15 +202,15 @@
         files_list = [f.path for f in nc.members]
         os.chdir(current_directory)
 
         # Aggregate
         agg = netCDF4.MFDataset(files_list, aggdim='t')
         return agg
 
-    elif file_extension in ['.nc', '.ncd', '.nc.gz']:
+    elif file_extension in ['.nc', '.nc4', '.ncd', '.nc.gz']:
 
         nc = netCDF4.Dataset(filename)
         return nc
 
     else:
         _terminate_with_error(
             "File format %s is not recognized." % file_extension)
@@ -248,21 +249,21 @@
         file_extension = os.path.splitext(url[:-3])[1]
 
     # Note that some opendap urls do not even have a file extension
     if file_extension != "":
 
         # If a file extension exists, check if it is a standard netcdf file
         if file_extension not in \
-                ['.nc', '.ncd', '.nc.gz', '.ncml', '.ncml.gz']:
+                ['.nc', '.nc4', '.ncd', '.nc.gz', '.ncml', '.ncml.gz']:
             _terminate_with_error(
                 'The input data URL is not an <i>netcdf</i> file. The URL ' +
-                'should end with <code>.nc</code>, <code>.ncd</code>, ' +
-                '<code>.nc.gz</code>, <code>.ncml</code>, ' +
-                '<code>.ncml.gz</code>, or without file extension.',
-                terminate)
+                'should end with <code>.nc</code>, <code>.nc4</code>, ' +
+                '<code>.ncd</code>, <code>.nc.gz</code>, ' +
+                '<code>.ncml</code>, <code>.ncml.gz</code>, or without file ' +
+                'extension.', terminate)
 
     try:
         # nc = open_url(url)
         nc = netCDF4.Dataset(url)
 
     except OSError:
         _terminate_with_error('Unable to read %s.' % url, terminate)
@@ -1092,16 +1093,16 @@
 
     Parameters
     ----------
 
     input : str
         The input netcdf file URL (if remote file) or file name (if local
         data). The URL should either have no extension, if it does have an
-        extension, the file extension should be either of ``.nc``, ``.nc.gz``,
-        ``.ncd``, ``.ncml``, or ``.ncml.gz``.
+        extension, the file extension should be either of ``.nc``, ``.nc4``,
+        ``.ncd``, ``.nc.gz``, ``.ncml``, or ``.ncml.gz``.
 
     scan_velocity : bool, default=False
         Scans the velocity arrays of the file. This is useful to find the min
         and max range of the velocity data to adjust the color bar for
         plotting.
 
     terminate : bool, default=False
@@ -1137,15 +1138,15 @@
 
     Examples
     --------
 
     .. code-block:: python
 
         >>> from restoreio import scan
-        >>> input = 'http://transport.me.berkeley.edu/thredds/dodsC/root/' + \
+        >>> input = 'https://transport.me.berkeley.edu/thredds/dodsC/root/' + \
         ...         'WHOI-HFR/WHOI_HFR_2014_original.nc'
 
         >>> # Run script
         >>> info = scan(input, scan_velocity=True, terminate=False,
         ...             verbose=True)
         {
             "Scan": {
```

### Comparing `restoreio-0.4.1/restoreio/_server_utils/globals.py` & `restoreio-0.5.0/restoreio/_server_utils/globals.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_server_utils/terminate_with_error.py` & `restoreio-0.5.0/restoreio/_server_utils/terminate_with_error.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_subset/_array_utilities.py` & `restoreio-0.5.0/restoreio/_subset/_array_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_subset/subset_datetime.py` & `restoreio-0.5.0/restoreio/_subset/subset_datetime.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_subset/subset_domain.py` & `restoreio-0.5.0/restoreio/_subset/subset_domain.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_uncertainty_quant/_compute_correlation_matrix.py` & `restoreio-0.5.0/restoreio/_uncertainty_quant/_compute_correlation_matrix.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py` & `restoreio-0.5.0/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_uncertainty_quant/_image_utils.py` & `restoreio-0.5.0/restoreio/_uncertainty_quant/_image_utils.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_uncertainty_quant/_statistical_distances.py` & `restoreio-0.5.0/restoreio/_uncertainty_quant/_statistical_distances.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio/_uncertainty_quant/generate_image_ensembles.py` & `restoreio-0.5.0/restoreio/_uncertainty_quant/generate_image_ensembles.py`

 * *Files 0% similar despite different names*

```diff
@@ -449,15 +449,15 @@
                               verbose=verbose)
 
     # window of kernel
     window_lon = kernel_width
     window_lat = kernel_width
     quadratic_form = _estimate_autocorrelation_rbf_kernel(
             masked_image_data, valid_indices_lon, ids_lon, window_lon,
-            window_lat, vel_component, plot, verbose=verbose)
+            window_lat, vel_component, plot=plot, save=save, verbose=verbose)
 
     # Generate ensembles for vector (Note: eigenvalues and eigenvectors are
     # only needed for plotting them)
     valid_vector_ensembles, eigenvalues, eigenvectors = \
         generate_valid_vector_ensembles(
                 valid_vector, valid_vector_error, valid_indices, num_ensembles,
                 ratio_num_modes, acf_length_scale_lon, acf_length_scale_lat,
```

### Comparing `restoreio-0.4.1/restoreio/_uncertainty_quant/get_ensembles_stat.py` & `restoreio-0.5.0/restoreio/_uncertainty_quant/get_ensembles_stat.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/restoreio.egg-info/PKG-INFO` & `restoreio-0.5.0/restoreio.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restoreio
-Version: 0.4.1
+Version: 0.5.0
 Summary: Reconstruct incomplete oceanographic dataset
 Home-page: https://github.com/ameli/restoreio
 Download-URL: https://github.com/ameli/restoreio/archive/main.zip
 Author: Siavash Ameli
 Author-email: sameli@berkeley.edu
 Project-URL: Documentation, https://github.com/ameli/restoreio/blob/main/README.rst
 Project-URL: Source, https://github.com/ameli/restoreio
@@ -39,20 +39,20 @@
 
 ******
 |logo|
 ******
 
 ``restoreio`` is a Python package to **Restore** **I**\ ncomplete **O**\ ceanographic dataset.
 
-``restoreio`` can be installed and used as a standalone Python package or in your browser through the `online gateway interface <http://transport.me.berkeley.edu/restore>`__.
+``restoreio`` can be installed and used as a standalone Python package or in your browser through the `online gateway interface <https://transport.me.berkeley.edu/restore>`__.
 
 Links
 =====
 
-* `Online Gateway <http://transport.me.berkeley.edu/restore>`_
+* `Online Gateway <https://transport.me.berkeley.edu/restore>`_
 * `Documentation <https://ameli.github.io/restoreio>`_
 * `PyPI <https://pypi.org/project/restoreio/>`_
 * `Anaconda <https://anaconda.org/s-ameli/restoreio>`_
 * `Git Hub <https://github.com/ameli/restoreio>`_
 
 Install
 =======
```

### Comparing `restoreio-0.4.1/restoreio.egg-info/SOURCES.txt` & `restoreio-0.5.0/restoreio.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 examples/restore/plot_variable_d_artificial_masks.py
 examples/restore/plot_variable_size_artificial_masks.py
 examples/uncertainty_quant/_display_utilities.py
 examples/uncertainty_quant/_draw_map.py
 examples/uncertainty_quant/_plot_utilities.py
 examples/uncertainty_quant/plot_gdop_coverage.py
 examples/uncertainty_quant/plot_js_divergence.py
+examples/uncertainty_quant/restoreio_mwe.py
 restoreio/__init__.py
 restoreio/__main__.py
 restoreio/__version__.py
 restoreio.egg-info/PKG-INFO
 restoreio.egg-info/SOURCES.txt
 restoreio.egg-info/dependency_links.txt
 restoreio.egg-info/entry_points.txt
```

### Comparing `restoreio-0.4.1/setup.py` & `restoreio-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.4.1/tests/test_restore_local_data.py` & `restoreio-0.5.0/tests/test_restore_local_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -78,17 +78,17 @@
             min_lon=min_lon, max_lon=max_lon, min_lat=min_lat, max_lat=max_lat,
             time=time, sweep=False, detect_land=True, fill_coast=False,
             convex_hull=False, alpha=20, refine_grid=1, uncertainty_quant=True,
             num_ensembles=200, ratio_num_modes=1, kernel_width=5,
             scale_error=0.08, plot=True, verbose=True, terminate=False)
 
     # Remove outputs
-    remove_file('*.svg')
-    remove_file('*.pdf')
-    remove_file(output)
+    # remove_file('*.svg')
+    # remove_file('*.pdf')
+    # remove_file(output)
 
 
 # ===========
 # Script main
 # ===========
 
 if __name__ == "__main__":
```

### Comparing `restoreio-0.4.1/tests/test_restore_remote_data.py` & `restoreio-0.5.0/tests/test_restore_remote_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     # min_lon = -122.344
     # max_lon = -121.781
     # min_lat = 36.507
     # max_lat = 36.9925
     # time = '2017-01-25T03:00:00'
 
     # Martha's Vineyard
-    input = 'http://transport.me.berkeley.edu/thredds/dodsC/root/' + \
+    input = 'https://transport.me.berkeley.edu/thredds/dodsC/root/' + \
             'WHOI-HFR/WHOI_HFR_2014_original.nc'
     min_lon = -70.7
     max_lon = -70.5
     min_lat = 41.2
     max_lat = 41.3
     min_time = '2014-07-01T20:00:00'
     max_time = '2014-07-03T20:00:00'
```

### Comparing `restoreio-0.4.1/tests/test_scan.py` & `restoreio-0.5.0/tests/test_scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 def test_scan():
     """
     Test for `scan` function.
     """
 
     # Martha's Vineyard
-    input = 'http://transport.me.berkeley.edu/thredds/dodsC/root/' + \
+    input = 'https://transport.me.berkeley.edu/thredds/dodsC/root/' + \
             'WHOI-HFR/WHOI_HFR_2014_original.nc'
 
     # Run script
     scan(input, scan_velocity=True, terminate=False, verbose=True)
 
 
 # ===========
```

### Comparing `restoreio-0.4.1/tox.ini` & `restoreio-0.5.0/tox.ini`

 * *Files identical despite different names*

