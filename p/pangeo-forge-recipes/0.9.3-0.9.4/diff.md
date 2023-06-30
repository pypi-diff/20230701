# Comparing `tmp/pangeo-forge-recipes-0.9.3.tar.gz` & `tmp/pangeo-forge-recipes-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pangeo-forge-recipes-0.9.3.tar", last modified: Tue Jan  3 21:43:10 2023, max compression
+gzip compressed data, was "pangeo-forge-recipes-0.9.4.tar", last modified: Fri Jan  6 20:44:22 2023, max compression
```

## Comparing `pangeo-forge-recipes-0.9.3.tar` & `pangeo-forge-recipes-0.9.4.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 21:43:10.455632 pangeo-forge-recipes-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 21:43:10.435631 pangeo-forge-recipes-0.9.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 21:43:10.439632 pangeo-forge-recipes-0.9.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/.github/workflows/main.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/.github/workflows/slash-command-dispatch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/.github/workflows/tutorials.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-01-03 21:43:10.455632 pangeo-forge-recipes-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 21:43:10.439632 pangeo-forge-recipes-0.9.3/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/ci/py3.8.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/ci/py3.9.yml
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/ci/upstream-dev.yml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 21:43:10.439632 pangeo-forge-recipes-0.9.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 21:43:10.439632 pangeo-forge-recipes-0.9.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/_static/human-maintainer.png
--rw-r--r--   0 runner    (1001) docker     (123)    21218 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/_static/pangeo-forge-bot.png
--rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/_static/pangeo-forge-logo-blue.png
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/_static/recipe-contributor.png
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 21:43:10.439632 pangeo-forge-recipes-0.9.3/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/images/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)    13105 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/images/Format_function.png
--rw-r--r--   0 runner    (1001) docker     (123)    21287 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/images/OISST_URL_structure.png
--rw-r--r--   0 runner    (1001) docker     (123)    38382 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/images/OISST_structure_conversion.png
--rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/images/SLA_Format_function.png
--rw-r--r--   0 runner    (1001) docker     (123)    40461 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/images/SLA_URL_structure.png
--rw-r--r--   0 runner    (1001) docker     (123)    21513 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/images/SLA_structure_conversion.png
--rw-r--r--   0 runner    (1001) docker     (123)    15093 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/images/SSS_Format_function.png
--rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/images/SSS_URL_structure.png
--rw-r--r--   0 runner    (1001) docker     (123)    52683 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/images/SSS_structure_conversion.png
--rw-r--r--   0 runner    (1001) docker     (123)    20496 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/images/XarrayZarrRecipe Syntax Recap.png
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 21:43:10.439632 pangeo-forge-recipes-0.9.3/docs/introduction_tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/introduction_tutorial/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/introduction_tutorial/intro_tutorial_part1.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   159887 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/introduction_tutorial/intro_tutorial_part2.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    16970 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/introduction_tutorial/intro_tutorial_part3.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 21:43:10.443632 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_cloud/core_concepts.md
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_cloud/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    23351 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_cloud/pr_checks_reference.md
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_cloud/recipe_contribution.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 21:43:10.443632 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/api_reference.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 21:43:10.443632 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/development/
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/development/coordination.md
--rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/development/development_guide.md
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/development/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/development/release_notes.md
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 21:43:10.443632 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/recipe_user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/recipe_user_guide/execution.md
--rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/recipe_user_guide/file_patterns.md
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/recipe_user_guide/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/recipe_user_guide/recipes.md
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/recipe_user_guide/storage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 21:43:10.443632 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 21:43:10.443632 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/tutorials/hdf_reference/
--rw-r--r--   0 runner    (1001) docker     (123)   355841 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/tutorials/hdf_reference/reference_cmip6.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/tutorials/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 21:43:10.447631 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/tutorials/xarray_zarr/
--rwxr-xr-x   0 runner    (1001) docker     (123)   255746 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/tutorials/xarray_zarr/cmip6-recipe.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (123)   280613 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/tutorials/xarray_zarr/multi_variable_recipe.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   389413 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/tutorials/xarray_zarr/ncei-woa-screenshot.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    16881 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/tutorials/xarray_zarr/netcdf_zarr_sequential.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  1240212 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/tutorials/xarray_zarr/opendap_subset_recipe.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (123)  2791167 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/tutorials/xarray_zarr/terraclimate.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/docs/what_is_pangeo_forge.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 21:43:10.451632 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-03 21:43:10.000000 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/chunk_grid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 21:43:10.451632 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/executors/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/executors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/executors/beam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/executors/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/executors/prefect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/executors/python.py
--rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 21:43:10.451632 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/recipes/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/recipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/recipes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/recipes/reference_hdf_zarr.py
--rw-r--r--   0 runner    (1001) docker     (123)    40907 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/recipes/xarray_zarr.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 21:43:10.451632 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-01-03 21:43:10.000000 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-01-03 21:43:10.000000 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-03 21:43:10.000000 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-03 21:43:10.000000 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-01-03 21:43:10.000000 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-03 21:43:10.000000 pangeo-forge-recipes-0.9.3/pangeo_forge_recipes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-01-03 21:43:10.455632 pangeo-forge-recipes-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 21:43:10.455632 pangeo-forge-recipes-0.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18361 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/tests/http_auth_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 21:43:10.455632 pangeo-forge-recipes-0.9.3/tests/recipe_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/tests/recipe_tests/test_HDFReferenceRecipe.py
--rw-r--r--   0 runner    (1001) docker     (123)    20926 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/tests/recipe_tests/test_XarrayZarrRecipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/tests/recipe_tests/test_execution_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/tests/recipe_tests/test_graph_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/tests/test_chunk_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/tests/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/tests/test_locking.py
--rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/tests/test_patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/tests/test_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/tests/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-01-03 21:43:01.000000 pangeo-forge-recipes-0.9.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:44:22.445115 pangeo-forge-recipes-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:44:22.425114 pangeo-forge-recipes-0.9.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:44:22.425114 pangeo-forge-recipes-0.9.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/.github/workflows/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/.github/workflows/slash-command-dispatch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/.github/workflows/tutorials.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-01-06 20:44:22.445115 pangeo-forge-recipes-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:44:22.425114 pangeo-forge-recipes-0.9.4/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/ci/py3.8.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/ci/py3.9.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/ci/upstream-dev.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:44:22.425114 pangeo-forge-recipes-0.9.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:44:22.425114 pangeo-forge-recipes-0.9.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/_static/human-maintainer.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21218 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/_static/pangeo-forge-bot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/_static/pangeo-forge-logo-blue.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/_static/recipe-contributor.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:44:22.429114 pangeo-forge-recipes-0.9.4/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/images/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)    13105 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/images/Format_function.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21287 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/images/OISST_URL_structure.png
+-rw-r--r--   0 runner    (1001) docker     (123)    38382 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/images/OISST_structure_conversion.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/images/SLA_Format_function.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40461 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/images/SLA_URL_structure.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21513 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/images/SLA_structure_conversion.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15093 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/images/SSS_Format_function.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/images/SSS_URL_structure.png
+-rw-r--r--   0 runner    (1001) docker     (123)    52683 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/images/SSS_structure_conversion.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20496 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/images/XarrayZarrRecipe Syntax Recap.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:44:22.429114 pangeo-forge-recipes-0.9.4/docs/introduction_tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/introduction_tutorial/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/introduction_tutorial/intro_tutorial_part1.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   159887 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/introduction_tutorial/intro_tutorial_part2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    16970 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/introduction_tutorial/intro_tutorial_part3.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:44:22.429114 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_cloud/core_concepts.md
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_cloud/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    23351 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_cloud/pr_checks_reference.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_cloud/recipe_contribution.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:44:22.429114 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/api_reference.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:44:22.429114 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/development/
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/development/coordination.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/development/development_guide.md
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/development/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/development/release_notes.md
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:44:22.429114 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/recipe_user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/recipe_user_guide/execution.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/recipe_user_guide/file_patterns.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/recipe_user_guide/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/recipe_user_guide/recipes.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/recipe_user_guide/storage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:44:22.429114 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:44:22.429114 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/tutorials/hdf_reference/
+-rw-r--r--   0 runner    (1001) docker     (123)   355841 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/tutorials/hdf_reference/reference_cmip6.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/tutorials/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:44:22.433114 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/tutorials/xarray_zarr/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   255746 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/tutorials/xarray_zarr/cmip6-recipe.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (123)   280613 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/tutorials/xarray_zarr/multi_variable_recipe.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   389413 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/tutorials/xarray_zarr/ncei-woa-screenshot.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16881 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/tutorials/xarray_zarr/netcdf_zarr_sequential.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1240212 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/tutorials/xarray_zarr/opendap_subset_recipe.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (123)  2791167 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/tutorials/xarray_zarr/terraclimate.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/docs/what_is_pangeo_forge.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:44:22.437115 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-06 20:44:22.000000 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/chunk_grid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:44:22.441115 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/executors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/executors/beam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/executors/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/executors/prefect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/executors/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:44:22.441115 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/recipes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/recipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/recipes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/recipes/reference_hdf_zarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40906 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/recipes/xarray_zarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:44:22.441115 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-01-06 20:44:22.000000 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-01-06 20:44:22.000000 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 20:44:22.000000 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 20:44:22.000000 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-01-06 20:44:22.000000 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-06 20:44:22.000000 pangeo-forge-recipes-0.9.4/pangeo_forge_recipes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-01-06 20:44:22.445115 pangeo-forge-recipes-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:44:22.441115 pangeo-forge-recipes-0.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18361 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/tests/http_auth_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 20:44:22.445115 pangeo-forge-recipes-0.9.4/tests/recipe_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/tests/recipe_tests/test_HDFReferenceRecipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20926 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/tests/recipe_tests/test_XarrayZarrRecipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/tests/recipe_tests/test_execution_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/tests/recipe_tests/test_graph_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/tests/test_chunk_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/tests/test_locking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/tests/test_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-01-06 20:44:13.000000 pangeo-forge-recipes-0.9.4/tests/test_utils.py
```

### Comparing `pangeo-forge-recipes-0.9.3/.github/workflows/main.yaml` & `pangeo-forge-recipes-0.9.4/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/.github/workflows/release.yaml` & `pangeo-forge-recipes-0.9.4/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/.github/workflows/tutorials.yaml` & `pangeo-forge-recipes-0.9.4/.github/workflows/tutorials.yaml`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/.gitignore` & `pangeo-forge-recipes-0.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/.pre-commit-config.yaml` & `pangeo-forge-recipes-0.9.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/LICENSE` & `pangeo-forge-recipes-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/PKG-INFO` & `pangeo-forge-recipes-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangeo-forge-recipes
-Version: 0.9.3
+Version: 0.9.4
 Summary: Pipeline tools for building and publishing analysis ready datasets.
 Home-page: https://github.com/pangeo-forge/pangeo-forge-recipes
 Maintainer: Ryan Abernathey
 Maintainer-email: rpa@ldeo.columbia.edu
 License: Apache
 Keywords: pangeo,data
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pangeo-forge-recipes-0.9.3/README.md` & `pangeo-forge-recipes-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/ci/py3.8.yml` & `pangeo-forge-recipes-0.9.4/ci/py3.8.yml`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/ci/py3.9.yml` & `pangeo-forge-recipes-0.9.4/ci/py3.9.yml`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/Makefile` & `pangeo-forge-recipes-0.9.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/_static/human-maintainer.png` & `pangeo-forge-recipes-0.9.4/docs/_static/human-maintainer.png`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/_static/pangeo-forge-bot.png` & `pangeo-forge-recipes-0.9.4/docs/_static/pangeo-forge-bot.png`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/_static/pangeo-forge-logo-blue.png` & `pangeo-forge-recipes-0.9.4/docs/_static/pangeo-forge-logo-blue.png`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/_static/recipe-contributor.png` & `pangeo-forge-recipes-0.9.4/docs/_static/recipe-contributor.png`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/conf.py` & `pangeo-forge-recipes-0.9.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/images/.DS_Store` & `pangeo-forge-recipes-0.9.4/docs/images/.DS_Store`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/images/Format_function.png` & `pangeo-forge-recipes-0.9.4/docs/images/Format_function.png`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/images/OISST_URL_structure.png` & `pangeo-forge-recipes-0.9.4/docs/images/OISST_URL_structure.png`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/images/OISST_structure_conversion.png` & `pangeo-forge-recipes-0.9.4/docs/images/OISST_structure_conversion.png`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/images/SLA_Format_function.png` & `pangeo-forge-recipes-0.9.4/docs/images/SLA_Format_function.png`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/images/SLA_URL_structure.png` & `pangeo-forge-recipes-0.9.4/docs/images/SLA_URL_structure.png`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/images/SLA_structure_conversion.png` & `pangeo-forge-recipes-0.9.4/docs/images/SLA_structure_conversion.png`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/images/SSS_Format_function.png` & `pangeo-forge-recipes-0.9.4/docs/images/SSS_Format_function.png`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/images/SSS_URL_structure.png` & `pangeo-forge-recipes-0.9.4/docs/images/SSS_URL_structure.png`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/images/SSS_structure_conversion.png` & `pangeo-forge-recipes-0.9.4/docs/images/SSS_structure_conversion.png`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/images/XarrayZarrRecipe Syntax Recap.png` & `pangeo-forge-recipes-0.9.4/docs/images/XarrayZarrRecipe Syntax Recap.png`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/index.md` & `pangeo-forge-recipes-0.9.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/introduction_tutorial/index.md` & `pangeo-forge-recipes-0.9.4/docs/introduction_tutorial/index.md`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/introduction_tutorial/intro_tutorial_part1.ipynb` & `pangeo-forge-recipes-0.9.4/docs/introduction_tutorial/intro_tutorial_part1.ipynb`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/introduction_tutorial/intro_tutorial_part2.ipynb` & `pangeo-forge-recipes-0.9.4/docs/introduction_tutorial/intro_tutorial_part2.ipynb`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/introduction_tutorial/intro_tutorial_part3.ipynb` & `pangeo-forge-recipes-0.9.4/docs/introduction_tutorial/intro_tutorial_part3.ipynb`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/make.bat` & `pangeo-forge-recipes-0.9.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/pangeo_forge_cloud/core_concepts.md` & `pangeo-forge-recipes-0.9.4/docs/pangeo_forge_cloud/core_concepts.md`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/pangeo_forge_cloud/index.md` & `pangeo-forge-recipes-0.9.4/docs/pangeo_forge_cloud/index.md`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/pangeo_forge_cloud/pr_checks_reference.md` & `pangeo-forge-recipes-0.9.4/docs/pangeo_forge_cloud/pr_checks_reference.md`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/pangeo_forge_cloud/recipe_contribution.md` & `pangeo-forge-recipes-0.9.4/docs/pangeo_forge_cloud/recipe_contribution.md`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/api_reference.md` & `pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/api_reference.md`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/development/coordination.md` & `pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/development/coordination.md`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/development/development_guide.md` & `pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/development/development_guide.md`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/development/release_notes.md` & `pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/development/release_notes.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 # Release Notes
 
+## v0.9.4 - 2023-01-06
+
+- Fixed bug in `0.9.3` which broke all recipe object imports if `scipy` (an optional
+dependency) was missing from environment. {pull}`466`
+
 ## v0.9.3 - 2023-01-03
 
+```{warning}
+Yanked due to presence of a bug. Please use `0.9.4` instead.
+```
+
 - Bugfix to allow opening of zarr files. This fix allows using Zarr stores as an input
 source for recipes. {pull}`462`
 - Add netcdf3 support for opening source files with kerchunk. Resolves a long-standing
 issue wherein netcdf3 source files could not be loaded lazily, which effectively
 blocked the use of large netcdf3 files as recipe sources. {pull}`383`
 - Fix zarr reference bug {pull}`455`
 - Add `dataset_type` class attribute for recipe classes {pull}`437`
```

### Comparing `pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/installation.md` & `pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/installation.md`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/recipe_user_guide/execution.md` & `pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/recipe_user_guide/execution.md`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/recipe_user_guide/file_patterns.md` & `pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/recipe_user_guide/file_patterns.md`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/recipe_user_guide/index.md` & `pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/recipe_user_guide/index.md`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/recipe_user_guide/recipes.md` & `pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/recipe_user_guide/recipes.md`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/recipe_user_guide/storage.md` & `pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/recipe_user_guide/storage.md`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/tutorials/hdf_reference/reference_cmip6.ipynb` & `pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/tutorials/hdf_reference/reference_cmip6.ipynb`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/tutorials/index.md` & `pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/tutorials/index.md`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/tutorials/xarray_zarr/cmip6-recipe.ipynb` & `pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/tutorials/xarray_zarr/cmip6-recipe.ipynb`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/tutorials/xarray_zarr/multi_variable_recipe.ipynb` & `pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/tutorials/xarray_zarr/multi_variable_recipe.ipynb`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/tutorials/xarray_zarr/ncei-woa-screenshot.png` & `pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/tutorials/xarray_zarr/ncei-woa-screenshot.png`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/tutorials/xarray_zarr/netcdf_zarr_sequential.ipynb` & `pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/tutorials/xarray_zarr/netcdf_zarr_sequential.ipynb`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/tutorials/xarray_zarr/opendap_subset_recipe.ipynb` & `pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/tutorials/xarray_zarr/opendap_subset_recipe.ipynb`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/pangeo_forge_recipes/tutorials/xarray_zarr/terraclimate.ipynb` & `pangeo-forge-recipes-0.9.4/docs/pangeo_forge_recipes/tutorials/xarray_zarr/terraclimate.ipynb`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/docs/what_is_pangeo_forge.md` & `pangeo-forge-recipes-0.9.4/docs/what_is_pangeo_forge.md`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/chunk_grid.py` & `pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/chunk_grid.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/executors/__init__.py` & `pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/executors/base.py` & `pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/executors/base.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/executors/beam.py` & `pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/executors/beam.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/executors/dask.py` & `pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/executors/dask.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/executors/prefect.py` & `pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/executors/prefect.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/executors/python.py` & `pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/executors/python.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/patterns.py` & `pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/patterns.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/recipes/__init__.py` & `pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/recipes/__init__.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/recipes/base.py` & `pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/recipes/base.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/recipes/reference_hdf_zarr.py` & `pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/recipes/reference_hdf_zarr.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/recipes/xarray_zarr.py` & `pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/recipes/xarray_zarr.py`

 * *Files 0% similar despite different names*

```diff
@@ -725,15 +725,15 @@
     The organization of the source files is described by the ``file_pattern``.
     Currently this recipe supports at most one ``MergeDim`` and one ``ConcatDim``
     in the File Pattern.
 
     :param file_pattern: An object which describes the organization of the input files.
     :param inputs_per_chunk: The number of inputs to use in each chunk along the concat dim.
        Must be an integer >= 1.
-    :param target_chunks: Desired chunk structure for the targret dataset. This is a dictionary
+    :param target_chunks: Desired chunk structure for the target dataset. This is a dictionary
        mapping dimension names to chunk size. When using a :class:`patterns.FilePattern` with
        a :class:`patterns.ConcatDim` that specifies ``n_items_per_file``, then you don't need
        to include the concat dim in ``target_chunks``.
     :param storage_config: Defines locations for writing the output dataset, caching temporary data,
       and for caching metadata for inputs and chunks. All three locations default to
       ``tempdir.TemporaryDirectory``; this default config can be used for testing and debugging the
       recipe. In an actual execution context, the default config is re-assigned to point to the
```

### Comparing `pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/reference.py` & `pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/reference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 Functions related to creating fsspec references.
 """
 
 from typing import Dict, Tuple, Union
 
 from kerchunk.hdf import SingleHdf5ToZarr
-from kerchunk.netCDF3 import NetCDF3ToZarr
 
 from .patterns import FileType
 
 
 def create_kerchunk_reference(
     fp, url: str, file_type: FileType, inline_threshold: int = 300
 ) -> Dict:
     if file_type == FileType.netcdf4:
         chunks = SingleHdf5ToZarr(fp, url, inline_threshold=inline_threshold)
     elif file_type == FileType.netcdf3:
+        from kerchunk.netCDF3 import NetCDF3ToZarr
+
         chunks = NetCDF3ToZarr(url, max_chunk_size=100_000_000)
     return chunks.translate()
 
 
 def unstrip_protocol(name: str, protocol: Union[str, Tuple[str, ...]]) -> str:
     # should be upstreamed into fsspec and maybe also
     # be a method on an OpenFile
```

### Comparing `pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/serialization.py` & `pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/serialization.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/storage.py` & `pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/storage.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/pangeo_forge_recipes/utils.py` & `pangeo-forge-recipes-0.9.4/pangeo_forge_recipes/utils.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/pangeo_forge_recipes.egg-info/PKG-INFO` & `pangeo-forge-recipes-0.9.4/pangeo_forge_recipes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangeo-forge-recipes
-Version: 0.9.3
+Version: 0.9.4
 Summary: Pipeline tools for building and publishing analysis ready datasets.
 Home-page: https://github.com/pangeo-forge/pangeo-forge-recipes
 Maintainer: Ryan Abernathey
 Maintainer-email: rpa@ldeo.columbia.edu
 License: Apache
 Keywords: pangeo,data
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pangeo-forge-recipes-0.9.3/pangeo_forge_recipes.egg-info/SOURCES.txt` & `pangeo-forge-recipes-0.9.4/pangeo_forge_recipes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/setup.cfg` & `pangeo-forge-recipes-0.9.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/tests/conftest.py` & `pangeo-forge-recipes-0.9.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/tests/http_auth_server.py` & `pangeo-forge-recipes-0.9.4/tests/http_auth_server.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/tests/recipe_tests/test_HDFReferenceRecipe.py` & `pangeo-forge-recipes-0.9.4/tests/recipe_tests/test_HDFReferenceRecipe.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/tests/recipe_tests/test_XarrayZarrRecipe.py` & `pangeo-forge-recipes-0.9.4/tests/recipe_tests/test_XarrayZarrRecipe.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/tests/recipe_tests/test_execution_context.py` & `pangeo-forge-recipes-0.9.4/tests/recipe_tests/test_execution_context.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/tests/recipe_tests/test_graph_memory.py` & `pangeo-forge-recipes-0.9.4/tests/recipe_tests/test_graph_memory.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/tests/test_chunk_grid.py` & `pangeo-forge-recipes-0.9.4/tests/test_chunk_grid.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/tests/test_fixtures.py` & `pangeo-forge-recipes-0.9.4/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/tests/test_locking.py` & `pangeo-forge-recipes-0.9.4/tests/test_locking.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/tests/test_patterns.py` & `pangeo-forge-recipes-0.9.4/tests/test_patterns.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/tests/test_pipelines.py` & `pangeo-forge-recipes-0.9.4/tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/tests/test_serialization.py` & `pangeo-forge-recipes-0.9.4/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/tests/test_storage.py` & `pangeo-forge-recipes-0.9.4/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-recipes-0.9.3/tests/test_utils.py` & `pangeo-forge-recipes-0.9.4/tests/test_utils.py`

 * *Files identical despite different names*

