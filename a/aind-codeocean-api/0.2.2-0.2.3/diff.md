# Comparing `tmp/aind_codeocean_api-0.2.2.tar.gz` & `tmp/aind_codeocean_api-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_codeocean_api-0.2.2.tar", last modified: Mon May  8 18:36:09 2023, max compression
+gzip compressed data, was "aind_codeocean_api-0.2.3.tar", last modified: Fri Jun 30 23:24:53 2023, max compression
```

## Comparing `aind_codeocean_api-0.2.2.tar` & `aind_codeocean_api-0.2.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:36:09.468292 aind_codeocean_api-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-08 18:35:50.000000 aind_codeocean_api-0.2.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:36:09.460291 aind_codeocean_api-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:36:09.460291 aind_codeocean_api-0.2.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-08 18:35:50.000000 aind_codeocean_api-0.2.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-08 18:35:50.000000 aind_codeocean_api-0.2.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-08 18:35:50.000000 aind_codeocean_api-0.2.2/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:36:09.460291 aind_codeocean_api-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-08 18:35:50.000000 aind_codeocean_api-0.2.2/.github/workflows/lint_and_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-08 18:35:50.000000 aind_codeocean_api-0.2.2/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-08 18:35:50.000000 aind_codeocean_api-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-08 18:35:50.000000 aind_codeocean_api-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-08 18:36:09.464292 aind_codeocean_api-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-08 18:35:50.000000 aind_codeocean_api-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:36:09.464292 aind_codeocean_api-0.2.2/doc_template/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-08 18:35:50.000000 aind_codeocean_api-0.2.2/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-08 18:35:50.000000 aind_codeocean_api-0.2.2/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:36:09.464292 aind_codeocean_api-0.2.2/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:36:09.464292 aind_codeocean_api-0.2.2/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-05-08 18:35:50.000000 aind_codeocean_api-0.2.2/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)   259838 2023-05-08 18:35:50.000000 aind_codeocean_api-0.2.2/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-05-08 18:35:50.000000 aind_codeocean_api-0.2.2/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-08 18:35:50.000000 aind_codeocean_api-0.2.2/doc_template/source/aind_codeocean_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-08 18:35:50.000000 aind_codeocean_api-0.2.2/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-08 18:35:50.000000 aind_codeocean_api-0.2.2/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-08 18:35:50.000000 aind_codeocean_api-0.2.2/doc_template/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-08 18:35:50.000000 aind_codeocean_api-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 18:36:09.468292 aind_codeocean_api-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-08 18:35:50.000000 aind_codeocean_api-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:36:09.460291 aind_codeocean_api-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:36:09.464292 aind_codeocean_api-0.2.2/src/aind_codeocean_api/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-08 18:35:50.000000 aind_codeocean_api-0.2.2/src/aind_codeocean_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20746 2023-05-08 18:35:50.000000 aind_codeocean_api-0.2.2/src/aind_codeocean_api/codeocean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-08 18:35:50.000000 aind_codeocean_api-0.2.2/src/aind_codeocean_api/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:36:09.464292 aind_codeocean_api-0.2.2/src/aind_codeocean_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-08 18:36:09.000000 aind_codeocean_api-0.2.2/src/aind_codeocean_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-08 18:36:09.000000 aind_codeocean_api-0.2.2/src/aind_codeocean_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 18:36:09.000000 aind_codeocean_api-0.2.2/src/aind_codeocean_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-08 18:36:09.000000 aind_codeocean_api-0.2.2/src/aind_codeocean_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-08 18:36:09.000000 aind_codeocean_api-0.2.2/src/aind_codeocean_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:36:09.464292 aind_codeocean_api-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 18:35:50.000000 aind_codeocean_api-0.2.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:36:09.464292 aind_codeocean_api-0.2.2/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-08 18:35:50.000000 aind_codeocean_api-0.2.2/tests/resources/fake_credentials.json
--rw-r--r--   0 runner    (1001) docker     (123)    28173 2023-05-08 18:35:50.000000 aind_codeocean_api-0.2.2/tests/test_codeocean_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-08 18:35:50.000000 aind_codeocean_api-0.2.2/tests/test_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:24:53.215109 aind_codeocean_api-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:24:53.207109 aind_codeocean_api-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:24:53.211109 aind_codeocean_api-0.2.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:24:53.211109 aind_codeocean_api-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/.github/workflows/lint_and_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-30 23:24:53.215109 aind_codeocean_api-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:24:53.211109 aind_codeocean_api-0.2.3/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:24:53.215109 aind_codeocean_api-0.2.3/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:24:53.215109 aind_codeocean_api-0.2.3/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   259838 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/doc_template/source/aind_codeocean_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/doc_template/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 23:24:53.215109 aind_codeocean_api-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:24:53.207109 aind_codeocean_api-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:24:53.215109 aind_codeocean_api-0.2.3/src/aind_codeocean_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-30 23:24:38.000000 aind_codeocean_api-0.2.3/src/aind_codeocean_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20676 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/src/aind_codeocean_api/codeocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/src/aind_codeocean_api/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:24:53.215109 aind_codeocean_api-0.2.3/src/aind_codeocean_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-30 23:24:53.000000 aind_codeocean_api-0.2.3/src/aind_codeocean_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-30 23:24:53.000000 aind_codeocean_api-0.2.3/src/aind_codeocean_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 23:24:53.000000 aind_codeocean_api-0.2.3/src/aind_codeocean_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-30 23:24:53.000000 aind_codeocean_api-0.2.3/src/aind_codeocean_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-30 23:24:53.000000 aind_codeocean_api-0.2.3/src/aind_codeocean_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:24:53.215109 aind_codeocean_api-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:24:53.215109 aind_codeocean_api-0.2.3/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/tests/resources/fake_credentials.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28173 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/tests/test_codeocean_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/tests/test_credentials.py
```

### Comparing `aind_codeocean_api-0.2.2/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_codeocean_api-0.2.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.2/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_codeocean_api-0.2.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.2/.github/ISSUE_TEMPLATE/user-story.md` & `aind_codeocean_api-0.2.3/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.2/.github/workflows/lint_and_test.yml` & `aind_codeocean_api-0.2.3/.github/workflows/lint_and_test.yml`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.2/.github/workflows/tag_and_publish.yml` & `aind_codeocean_api-0.2.3/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.2/.gitignore` & `aind_codeocean_api-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.2/LICENSE` & `aind_codeocean_api-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.2/PKG-INFO` & `aind_codeocean_api-0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind_codeocean_api
-Version: 0.2.2
+Version: 0.2.3
 Summary: CodeOcean API manager in Python
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `aind_codeocean_api-0.2.2/README.md` & `aind_codeocean_api-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.2/doc_template/Makefile` & `aind_codeocean_api-0.2.3/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.2/doc_template/make.bat` & `aind_codeocean_api-0.2.3/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.2/doc_template/source/_static/dark-logo.svg` & `aind_codeocean_api-0.2.3/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.2/doc_template/source/_static/favicon.ico` & `aind_codeocean_api-0.2.3/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.2/doc_template/source/_static/light-logo.svg` & `aind_codeocean_api-0.2.3/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.2/doc_template/source/aind_codeocean_api.rst` & `aind_codeocean_api-0.2.3/doc_template/source/aind_codeocean_api.rst`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.2/doc_template/source/conf.py` & `aind_codeocean_api-0.2.3/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.2/pyproject.toml` & `aind_codeocean_api-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.2/src/aind_codeocean_api/codeocean.py` & `aind_codeocean_api-0.2.3/src/aind_codeocean_api/codeocean.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,18 +345,14 @@
         asset_description : Optional[str]
             A description of the data asset. Default blanks.
         mount : string
             Mount point. Default None (Mount point equal to the asset name)
         tags : Optional[List[str]]
             A list of tags to attach to the data asset.
             Default None (empty list).
-        keep_on_external_storage : Optional[bool]
-            Keep data asset on external storage. Defaults to True.
-        index_data : Optional[bool]
-            Whether to index the data asset. Defaults to True.
         custom_metadata : Optional[dict]
             What key:value metadata tags to apply to the asset.
         Returns
         ---------------
         requests.models.Response
         """
 
@@ -606,39 +602,42 @@
         self.logger.info(response.url)
 
         return response
 
     def update_permissions(
         self,
         data_asset_id: str,
-        users: List[Dict] = [],
-        groups: List[Dict] = [],
+        users: Optional[List[Dict]] = None,
+        groups: Optional[List[Dict]] = None,
         everyone: Optional[str] = None,
     ) -> requests.models.Response:
         """
         This will update permissions of a data asset from a POST request to
         Code Ocean API.
 
         Parameters
         ---------------
         data_asset_id : string
             ID of the data asset
-        users: List[Dict] (optional, default [])
+        users: Optional[List[Dict]] (optional, default None)
             list of dictionaries containing keys 'email' and 'role'
-        groups: List[Dict] (optional, default [])
+        groups: Optional[List[Dict]] (optional, default None)
             list of dictionaries containing keys 'group' and 'role'
           'role' is 'owner' or 'viewer'
         everyone: str (optional, default None)
             'none': revoke global perms. 'viewer': grant viewer globally
 
         Returns
         ---------------
         requests.models.Response
         """
 
+        users = [] if users is None else users
+        groups = [] if groups is None else groups
+
         permissions = {
             self._Fields.USERS.value: users,
             self._Fields.GROUPS.value: groups,
         }
 
         if everyone is not None:
             permissions[self._Fields.EVERYONE.value] = everyone
```

### Comparing `aind_codeocean_api-0.2.2/src/aind_codeocean_api/credentials.py` & `aind_codeocean_api-0.2.3/src/aind_codeocean_api/credentials.py`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.2/src/aind_codeocean_api.egg-info/PKG-INFO` & `aind_codeocean_api-0.2.3/src/aind_codeocean_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-codeocean-api
-Version: 0.2.2
+Version: 0.2.3
 Summary: CodeOcean API manager in Python
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `aind_codeocean_api-0.2.2/src/aind_codeocean_api.egg-info/SOURCES.txt` & `aind_codeocean_api-0.2.3/src/aind_codeocean_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.2/tests/test_codeocean_requests.py` & `aind_codeocean_api-0.2.3/tests/test_codeocean_requests.py`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.2/tests/test_credentials.py` & `aind_codeocean_api-0.2.3/tests/test_credentials.py`

 * *Files identical despite different names*

