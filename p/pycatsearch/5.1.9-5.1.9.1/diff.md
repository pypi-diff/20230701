# Comparing `tmp/pycatsearch-5.1.9.tar.gz` & `tmp/pycatsearch-5.1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycatsearch-5.1.9.tar", last modified: Sat Jul  1 14:59:34 2023, max compression
+gzip compressed data, was "pycatsearch-5.1.9.1.tar", last modified: Sat Jul  1 17:53:04 2023, max compression
```

## Comparing `pycatsearch-5.1.9.tar` & `pycatsearch-5.1.9.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:59:34.842588 pycatsearch-5.1.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:59:34.834588 pycatsearch-5.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:59:34.838588 pycatsearch-5.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    10587 2023-07-01 14:59:34.842588 pycatsearch-5.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9047 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 14:59:34.842588 pycatsearch-5.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:59:34.834588 pycatsearch-5.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:59:34.838588 pycatsearch-5.1.9/src/pycatsearch/
--rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/src/pycatsearch/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      109 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/src/pycatsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-01 14:59:34.000000 pycatsearch-5.1.9/src/pycatsearch/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/src/pycatsearch/async_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/src/pycatsearch/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/src/pycatsearch/catalog_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/src/pycatsearch/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:59:34.842588 pycatsearch-5.1.9/src/pycatsearch/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/src/pycatsearch/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/src/pycatsearch/gui/catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/src/pycatsearch/gui/download_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/src/pycatsearch/gui/float_spinbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/src/pycatsearch/gui/frequency_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/src/pycatsearch/gui/html_style_delegate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/src/pycatsearch/gui/menu_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/src/pycatsearch/gui/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/src/pycatsearch/gui/selectable_label.py
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/src/pycatsearch/gui/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/src/pycatsearch/gui/substance_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/src/pycatsearch/gui/substances_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/src/pycatsearch/gui/titled_list_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    44013 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/src/pycatsearch/gui/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/src/pycatsearch/gui/url_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/src/pycatsearch/gui/waiting_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)    24484 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/src/pycatsearch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:59:34.842588 pycatsearch-5.1.9/src/pycatsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10587 2023-07-01 14:59:34.000000 pycatsearch-5.1.9/src/pycatsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-01 14:59:34.000000 pycatsearch-5.1.9/src/pycatsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 14:59:34.000000 pycatsearch-5.1.9/src/pycatsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-01 14:59:34.000000 pycatsearch-5.1.9/src/pycatsearch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 14:59:34.000000 pycatsearch-5.1.9/src/pycatsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-01 14:59:34.000000 pycatsearch-5.1.9/src/pycatsearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-07-01 14:59:19.000000 pycatsearch-5.1.9/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:53:04.082080 pycatsearch-5.1.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:53:04.070080 pycatsearch-5.1.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:53:04.074080 pycatsearch-5.1.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-07-01 17:53:04.082080 pycatsearch-5.1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9066 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 17:53:04.082080 pycatsearch-5.1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:53:04.070080 pycatsearch-5.1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:53:04.074080 pycatsearch-5.1.9.1/src/pycatsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/src/pycatsearch/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      109 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/src/pycatsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-01 17:53:03.000000 pycatsearch-5.1.9.1/src/pycatsearch/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/src/pycatsearch/async_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/src/pycatsearch/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/src/pycatsearch/catalog_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/src/pycatsearch/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:53:04.082080 pycatsearch-5.1.9.1/src/pycatsearch/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/src/pycatsearch/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/src/pycatsearch/gui/catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/src/pycatsearch/gui/download_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/src/pycatsearch/gui/float_spinbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/src/pycatsearch/gui/frequency_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/src/pycatsearch/gui/html_style_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/src/pycatsearch/gui/menu_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/src/pycatsearch/gui/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/src/pycatsearch/gui/selectable_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/src/pycatsearch/gui/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/src/pycatsearch/gui/substance_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14347 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/src/pycatsearch/gui/substances_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/src/pycatsearch/gui/titled_list_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43920 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/src/pycatsearch/gui/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/src/pycatsearch/gui/url_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/src/pycatsearch/gui/waiting_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24484 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/src/pycatsearch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:53:04.078080 pycatsearch-5.1.9.1/src/pycatsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-07-01 17:53:04.000000 pycatsearch-5.1.9.1/src/pycatsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-01 17:53:04.000000 pycatsearch-5.1.9.1/src/pycatsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 17:53:04.000000 pycatsearch-5.1.9.1/src/pycatsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-01 17:53:04.000000 pycatsearch-5.1.9.1/src/pycatsearch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 17:53:04.000000 pycatsearch-5.1.9.1/src/pycatsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-01 17:53:04.000000 pycatsearch-5.1.9.1/src/pycatsearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-07-01 17:52:53.000000 pycatsearch-5.1.9.1/updater.py
```

### Comparing `pycatsearch-5.1.9/.github/workflows/publish-to-pypi.yml` & `pycatsearch-5.1.9.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.9/LICENSE.md` & `pycatsearch-5.1.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.9/PKG-INFO` & `pycatsearch-5.1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycatsearch
-Version: 5.1.9
+Version: 5.1.9.1
 Summary: Yet another implementation of JPL and CDMS spectroscopy catalogs offline search
 Author-email: StSav012 <stsav012@gmail.com>
 License: LGPL-3.0-only
 Project-URL: Source Code, https://github.com/StSav012/pycatsearch
 Project-URL: Bug Tracker, https://github.com/StSav012/pycatsearch/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Win32 (MS Windows)
@@ -70,15 +70,15 @@
 - `entries_count` is the number of the substances loaded by `__init__`.
 - `sources` contains a list of files that have been loaded successfully by `__init__`.
 - `sources_info` returns a list of the files and the timestamps recorded there (if any).
 - `min_frequency` and `max_frequency` are the extreme values of `frequency_limits`.
 
 ###### Functions:
 
-- `__init__(self, *catalog_file_names: str)` accepts names of JSON or GZipped JSON files.
+- `__init__(self, *catalog_file_names: str)` accepts names of JSON or GZip/BZip2/LZMA-compressed JSON files.
   It loads them into memory joined.
 - `filter(self, *,
   min_frequency: float = 0.0,
   max_frequency: float = math.inf,
   min_intensity: float = -math.inf,
   max_intensity: float = math.inf,
   temperature: float = -math.inf,
```

### Comparing `pycatsearch-5.1.9/README.md` & `pycatsearch-5.1.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 - `entries_count` is the number of the substances loaded by `__init__`.
 - `sources` contains a list of files that have been loaded successfully by `__init__`.
 - `sources_info` returns a list of the files and the timestamps recorded there (if any).
 - `min_frequency` and `max_frequency` are the extreme values of `frequency_limits`.
 
 ###### Functions:
 
-- `__init__(self, *catalog_file_names: str)` accepts names of JSON or GZipped JSON files.
+- `__init__(self, *catalog_file_names: str)` accepts names of JSON or GZip/BZip2/LZMA-compressed JSON files.
   It loads them into memory joined.
 - `filter(self, *,
   min_frequency: float = 0.0,
   max_frequency: float = math.inf,
   min_intensity: float = -math.inf,
   max_intensity: float = math.inf,
   temperature: float = -math.inf,
```

### Comparing `pycatsearch-5.1.9/main.py` & `pycatsearch-5.1.9.1/main.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.9/pyproject.toml` & `pycatsearch-5.1.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.9/setup.py` & `pycatsearch-5.1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.9/src/pycatsearch/__init__.py` & `pycatsearch-5.1.9.1/src/pycatsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.9/src/pycatsearch/async_downloader.py` & `pycatsearch-5.1.9.1/src/pycatsearch/async_downloader.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.9/src/pycatsearch/catalog.py` & `pycatsearch-5.1.9.1/src/pycatsearch/catalog.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.9/src/pycatsearch/catalog_entry.py` & `pycatsearch-5.1.9.1/src/pycatsearch/catalog_entry.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.9/src/pycatsearch/downloader.py` & `pycatsearch-5.1.9.1/src/pycatsearch/downloader.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.9/src/pycatsearch/gui/catalog_info.py` & `pycatsearch-5.1.9.1/src/pycatsearch/gui/catalog_info.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.9/src/pycatsearch/gui/download_dialog.py` & `pycatsearch-5.1.9.1/src/pycatsearch/gui/download_dialog.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.9/src/pycatsearch/gui/float_spinbox.py` & `pycatsearch-5.1.9.1/src/pycatsearch/gui/float_spinbox.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.9/src/pycatsearch/gui/frequency_box.py` & `pycatsearch-5.1.9.1/src/pycatsearch/gui/frequency_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,25 +50,25 @@
         self._page_by_center: QWidget = QWidget()
         self._layout_by_center: QFormLayout = QFormLayout(self._page_by_center)
         self._spin_frequency_center: FrequencySpinBox = FrequencySpinBox(self._page_by_center)
         self._spin_frequency_deviation: FrequencySpinBox = FrequencySpinBox(self._page_by_center)
 
         self._layout_by_range.setLabelAlignment(Qt.AlignmentFlag.AlignLeft)
         self._spin_frequency_from.setValue(118747.341)
-        self._layout_by_range.addRow(self._layout_by_range.tr('From:'), self._spin_frequency_from)
+        self._layout_by_range.addRow(self.tr('From:'), self._spin_frequency_from)
         self._spin_frequency_to.setValue(118753.341)
-        self._layout_by_range.addRow(self._layout_by_range.tr('To:'), self._spin_frequency_to)
+        self._layout_by_range.addRow(self.tr('To:'), self._spin_frequency_to)
         self.addTab(self._page_by_range, icon('mdi6.arrow-expand-horizontal'), self.tr('Range'))
 
         self._spin_frequency_center.setValue(118750.341)
-        self._layout_by_center.addRow(self._layout_by_center.tr('Center:'), self._spin_frequency_center)
+        self._layout_by_center.addRow(self.tr('Center:'), self._spin_frequency_center)
         self._spin_frequency_deviation.setMaximum(99.9999)
         self._spin_frequency_deviation.setSingleStep(0.1)
         self._spin_frequency_deviation.setValue(0.4)
-        self._layout_by_center.addRow(self._layout_by_center.tr('Deviation:'), self._spin_frequency_deviation)
+        self._layout_by_center.addRow(self.tr('Deviation:'), self._spin_frequency_deviation)
         self.addTab(self._page_by_center, icon('mdi6.format-horizontal-align-center'), self.tr('Center'))
 
         self.load_settings()
 
         self._spin_frequency_from.valueChanged.connect(self._on_spin_frequency_from_edited)
         self._spin_frequency_to.valueChanged.connect(self._on_spin_frequency_to_edited)
         self._spin_frequency_center.valueChanged.connect(self._on_spin_frequency_center_edited)
```

### Comparing `pycatsearch-5.1.9/src/pycatsearch/gui/html_style_delegate.py` & `pycatsearch-5.1.9.1/src/pycatsearch/gui/html_style_delegate.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.9/src/pycatsearch/gui/menu_bar.py` & `pycatsearch-5.1.9.1/src/pycatsearch/gui/menu_bar.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,15 @@
         self.menu_edit.addSeparator()
         self.menu_copy_only: QMenu = self.menu_edit.addMenu(self.tr('Copy &Only'))
         self.action_copy_current: QAction = self.menu_copy_only.addAction(self.tr('Active &Cell'))
         self.menu_copy_only.addSeparator()
         self.action_copy_name: QAction = self.menu_copy_only.addAction(self.tr('&Substance Name'))
         self.action_copy_frequency: QAction = self.menu_copy_only.addAction(self.tr('&Frequency'))
         self.action_copy_intensity: QAction = self.menu_copy_only.addAction(self.tr('&Intensity'))
-        self.action_copy_lower_state_energy: QAction = self.menu_copy_only.addAction(
-            self.menu_copy_only.tr('&Lower State Energy'))
+        self.action_copy_lower_state_energy: QAction = self.menu_copy_only.addAction(self.tr('&Lower State Energy'))
         self.action_copy: QAction = self.menu_edit.addAction(
             self._icon('edit-copy', 'mdi6.content-copy'),
             self.tr('Co&py Selection'))
         self.menu_edit.addSeparator()
         self.action_select_all: QAction = self.menu_edit.addAction(
             self._icon('edit-select-all', 'mdi6.select-all'),
             self.tr('&Select All'))
```

### Comparing `pycatsearch-5.1.9/src/pycatsearch/gui/preferences.py` & `pycatsearch-5.1.9.1/src/pycatsearch/gui/preferences.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.9/src/pycatsearch/gui/settings.py` & `pycatsearch-5.1.9.1/src/pycatsearch/gui/settings.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.9/src/pycatsearch/gui/substance_info.py` & `pycatsearch-5.1.9.1/src/pycatsearch/gui/substance_info.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.9/src/pycatsearch/gui/substances_box.py` & `pycatsearch-5.1.9.1/src/pycatsearch/gui/substances_box.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
-from typing import Callable, cast
+from typing import Callable
 
 from qtpy.QtCore import QModelIndex, Qt, Signal, Slot
 from qtpy.QtWidgets import (QAbstractItemView, QAbstractScrollArea, QCheckBox, QGroupBox, QLineEdit, QListWidget,
                             QListWidgetItem, QPushButton, QVBoxLayout, QWidget)
 
 from .html_style_delegate import HTMLDelegate
 from .settings import Settings
@@ -34,31 +34,30 @@
         self._list_substance: QListWidget = QListWidget(self)
         self._check_keep_selection: QCheckBox = QCheckBox(self)
         self._button_select_none: QPushButton = QPushButton(self)
 
         self.setCheckable(True)
         self.setTitle(self.tr('Search Only For…'))
         self._text_substance.setClearButtonEnabled(True)
-        self._text_substance.setPlaceholderText(self._text_substance.tr('Filter'))
+        self._text_substance.setPlaceholderText(self.tr('Filter'))
         self._layout_substance.addWidget(self._text_substance)
         self._list_substance.setEditTriggers(QAbstractItemView.EditTrigger.NoEditTriggers)
         self._list_substance.setDropIndicatorShown(False)
         self._list_substance.setAlternatingRowColors(True)
         self._list_substance.setSelectionMode(QAbstractItemView.SelectionMode.ExtendedSelection)
         self._list_substance.setSelectionBehavior(QAbstractItemView.SelectionBehavior.SelectRows)
         self._list_substance.setSortingEnabled(False)
         self._list_substance.setSizeAdjustPolicy(QAbstractScrollArea.SizeAdjustPolicy.AdjustToContents)
         self._list_substance.setItemDelegateForColumn(0, HTMLDelegate())
         self._layout_substance.addWidget(self._list_substance)
-        self._check_keep_selection.setStatusTip(
-            self._check_keep_selection.tr('Keep substances list selection through filter changes'))
-        self._check_keep_selection.setText(self._check_keep_selection.tr('Persistent Selection'))
+        self._check_keep_selection.setStatusTip(self.tr('Keep substances list selection through filter changes'))
+        self._check_keep_selection.setText(self.tr('Persistent Selection'))
         self._layout_substance.addWidget(self._check_keep_selection)
-        self._button_select_none.setStatusTip(self._button_select_none.tr('Clear substances list selection'))
-        self._button_select_none.setText(self._button_select_none.tr('Select None'))
+        self._button_select_none.setStatusTip(self.tr('Clear substances list selection'))
+        self._button_select_none.setText(self.tr('Select None'))
         self._layout_substance.addWidget(self._button_select_none)
 
         self._button_select_none.setIcon(icon('mdi6.checkbox-blank-off-outline'))
 
         self._text_substance.textChanged.connect(self._on_text_changed)
         self._check_keep_selection.toggled.connect(self._on_check_save_selection_toggled)
         self._button_select_none.clicked.connect(self._on_button_select_none_clicked)
@@ -219,28 +218,28 @@
                 self.catalog, species_tags.pop(),
                 inchi_key_search_url_template=self._settings.inchi_key_search_url_template,
                 parent=self)
             syn.exec()
 
     @Slot(QListWidgetItem)
     def _on_list_substance_item_changed(self, item: QListWidgetItem) -> None:
-        species_tags: set[int] = cast(set[int], item.data(Qt.ItemDataRole.UserRole))
+        species_tags: set[int] = item.data(Qt.ItemDataRole.UserRole)
         if item.checkState() == Qt.CheckState.Checked:
             if not self._selected_substances.issuperset(species_tags):
                 self._selected_substances |= species_tags
                 self.selectedSubstancesChanged.emit()
         else:
             if self._selected_substances.intersection(species_tags):
                 self._selected_substances -= species_tags
                 self.selectedSubstancesChanged.emit()
         self._list_substance.blockSignals(True)
         another_item: QListWidgetItem
         for i in range(self._list_substance.count()):
             another_item = self._list_substance.item(i)
-            another_item_species_tags: set[int] = cast(set[int], another_item.data(Qt.ItemDataRole.UserRole))
+            another_item_species_tags: set[int] = another_item.data(Qt.ItemDataRole.UserRole)
             if another_item_species_tags <= self._selected_substances:
                 another_item.setCheckState(Qt.CheckState.Checked)
             elif another_item_species_tags & self._selected_substances:
                 another_item.setCheckState(Qt.CheckState.PartiallyChecked)
             else:
                 another_item.setCheckState(Qt.CheckState.Unchecked)
         self._list_substance.blockSignals(False)
```

### Comparing `pycatsearch-5.1.9/src/pycatsearch/gui/titled_list_widget.py` & `pycatsearch-5.1.9.1/src/pycatsearch/gui/titled_list_widget.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.9/src/pycatsearch/gui/ui.py` & `pycatsearch-5.1.9.1/src/pycatsearch/gui/ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,28 +320,28 @@
                                              | Qt.AlignmentFlag.AlignTrailing
                                              | Qt.AlignmentFlag.AlignVCenter)
             self.spin_intensity.setButtonSymbols(QAbstractSpinBox.ButtonSymbols.NoButtons)
             self.spin_intensity.setDecimals(2)
             self.spin_intensity.setRange(-inf, inf)
             self.spin_intensity.setSingleStep(0.1)
             self.spin_intensity.setValue(-6.54)
-            self.spin_intensity.setStatusTip(self.spin_intensity.tr('Limit shown spectral lines'))
-            layout_options.addRow(layout_options.tr('Minimal Intensity:'), self.spin_intensity)
+            self.spin_intensity.setStatusTip(self.tr('Limit shown spectral lines'))
+            layout_options.addRow(self.tr('Minimal Intensity:'), self.spin_intensity)
             self.spin_temperature.setAlignment(Qt.AlignmentFlag.AlignRight
                                                | Qt.AlignmentFlag.AlignTrailing
                                                | Qt.AlignmentFlag.AlignVCenter)
             self.spin_temperature.setButtonSymbols(QAbstractSpinBox.ButtonSymbols.NoButtons)
             self.spin_temperature.setMaximum(999.99)
             self.spin_temperature.setValue(300.0)
-            self.spin_temperature.setStatusTip(self.spin_temperature.tr('Temperature to calculate intensity'))
-            self.spin_temperature.setSuffix(self.spin_temperature.tr(' K'))
-            layout_options.addRow(layout_options.tr('Temperature:'), self.spin_temperature)
+            self.spin_temperature.setStatusTip(self.tr('Temperature to calculate intensity'))
+            self.spin_temperature.setSuffix(self.tr(' K'))
+            layout_options.addRow(self.tr('Temperature:'), self.spin_temperature)
             layout_right.addLayout(layout_options, 0)
 
-            self.button_search.setText(self.button_search.tr('Show'))
+            self.button_search.setText(self.tr('Show'))
             layout_right.addWidget(self.button_search, 0)
 
             self._right_matter.setLayout(layout_right)
             self._top_matter.addWidget(self._right_matter)
             self._top_matter.setStretchFactor(0, 1)
             self._top_matter.setChildrenCollapsible(False)
 
@@ -710,20 +710,20 @@
                           self.tr("About CatSearch"),
                           "<html><p>"
                           + self.tr("CatSearch is a means of searching through spectroscopy lines catalogs. "
                                     "It's an offline application.")
                           + "</p><p>"
                           + self.tr("It relies on the data stored in JSON files.")
                           + "</p><p>"
-                          + self.tr("One can write his own catalogs as well as convert data from "
+                          + self.tr("One can write their own catalogs as well as download data from "
                                     "<a href='https://spec.jpl.nasa.gov/'>JPL</a> and "
                                     "<a href='https://astro.uni-koeln.de/'>CDMS</a> spectroscopy databases "
-                                    "freely available in the Internet or other sources.")
+                                    "available in the Internet.")
                           + "</p><p>"
-                          + self.tr("Both plain text JSON and GZip compressed JSON are supported.")
+                          + self.tr("Both plain text JSON and GZip/BZip2/LZMA-compressed JSON are supported.")
                           + "</p><p>"
                           + self.tr('See {0} for more info.')
                           .format('<a href="https://github.com/StSav012/pycatsearch/blob/master/README.md">{0}</a>')
                           .format(self.tr('readme'))
                           + "</p><br><p>"
                           + self.tr("CatSearch is licensed under the {0}.")
                           .format("<a href='https://www.gnu.org/copyleft/lesser.html'>{0}</a>"
```

### Comparing `pycatsearch-5.1.9/src/pycatsearch/gui/waiting_screen.py` & `pycatsearch-5.1.9.1/src/pycatsearch/gui/waiting_screen.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.9/src/pycatsearch/utils.py` & `pycatsearch-5.1.9.1/src/pycatsearch/utils.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.9/src/pycatsearch.egg-info/PKG-INFO` & `pycatsearch-5.1.9.1/src/pycatsearch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycatsearch
-Version: 5.1.9
+Version: 5.1.9.1
 Summary: Yet another implementation of JPL and CDMS spectroscopy catalogs offline search
 Author-email: StSav012 <stsav012@gmail.com>
 License: LGPL-3.0-only
 Project-URL: Source Code, https://github.com/StSav012/pycatsearch
 Project-URL: Bug Tracker, https://github.com/StSav012/pycatsearch/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Win32 (MS Windows)
@@ -70,15 +70,15 @@
 - `entries_count` is the number of the substances loaded by `__init__`.
 - `sources` contains a list of files that have been loaded successfully by `__init__`.
 - `sources_info` returns a list of the files and the timestamps recorded there (if any).
 - `min_frequency` and `max_frequency` are the extreme values of `frequency_limits`.
 
 ###### Functions:
 
-- `__init__(self, *catalog_file_names: str)` accepts names of JSON or GZipped JSON files.
+- `__init__(self, *catalog_file_names: str)` accepts names of JSON or GZip/BZip2/LZMA-compressed JSON files.
   It loads them into memory joined.
 - `filter(self, *,
   min_frequency: float = 0.0,
   max_frequency: float = math.inf,
   min_intensity: float = -math.inf,
   max_intensity: float = math.inf,
   temperature: float = -math.inf,
```

### Comparing `pycatsearch-5.1.9/src/pycatsearch.egg-info/SOURCES.txt` & `pycatsearch-5.1.9.1/src/pycatsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.9/updater.py` & `pycatsearch-5.1.9.1/updater.py`

 * *Files identical despite different names*

