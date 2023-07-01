# Comparing `tmp/pynamer-2.1.7.tar.gz` & `tmp/pynamer-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamer-2.1.7.tar", last modified: Mon Jun 19 19:04:55 2023, max compression
+gzip compressed data, was "pynamer-2.1.8.tar", last modified: Sat Jul  1 15:01:58 2023, max compression
```

## Comparing `pynamer-2.1.7.tar` & `pynamer-2.1.8.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 19:04:55.234025 pynamer-2.1.7/
--rw-rw-rw-   0        0        0      172 2023-05-21 12:10:39.000000 pynamer-2.1.7/AUTHORS.md
--rw-rw-rw-   0        0        0    11947 2023-06-19 19:04:40.000000 pynamer-2.1.7/CHANGELOG.md
--rw-rw-rw-   0        0        0     1095 2023-05-21 12:10:39.000000 pynamer-2.1.7/LICENSE
--rw-rw-rw-   0        0        0      237 2023-05-21 12:10:39.000000 pynamer-2.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0    19784 2023-06-19 19:04:55.234025 pynamer-2.1.7/PKG-INFO
--rw-rw-rw-   0        0        0    17816 2023-06-19 12:49:30.000000 pynamer-2.1.7/README.md
--rw-rw-rw-   0        0        0     2183 2023-06-11 20:09:06.000000 pynamer-2.1.7/pyproject.toml
--rw-rw-rw-   0        0        0     2288 2023-06-19 19:04:55.236026 pynamer-2.1.7/setup.cfg
--rw-rw-rw-   0        0        0      109 2023-04-21 12:29:15.000000 pynamer-2.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 19:04:54.788031 pynamer-2.1.7/src/
-drwxrwxrwx   0        0        0        0 2023-06-19 19:04:54.886027 pynamer-2.1.7/src/pynamer/
--rw-rw-rw-   0        0        0       11 2023-05-21 12:10:39.000000 pynamer-2.1.7/src/pynamer/README.md
--rw-rw-rw-   0        0        0     1989 2023-06-19 19:04:40.000000 pynamer-2.1.7/src/pynamer/__init__.py
--rw-rw-rw-   0        0        0     9736 2023-05-29 10:07:59.000000 pynamer-2.1.7/src/pynamer/builder.py
--rw-rw-rw-   0        0        0     2462 2023-06-12 20:06:37.000000 pynamer-2.1.7/src/pynamer/cli.py
--rw-rw-rw-   0        0        0      863 2023-06-12 20:04:32.000000 pynamer-2.1.7/src/pynamer/config.py
-drwxrwxrwx   0        0        0        0 2023-06-19 19:04:54.901026 pynamer-2.1.7/src/pynamer/project_name/
--rw-rw-rw-   0        0        0        0 2023-05-21 12:10:39.000000 pynamer-2.1.7/src/pynamer/project_name/__init__.py
--rw-rw-rw-   0        0        0     7935 2023-06-17 17:24:20.000000 pynamer-2.1.7/src/pynamer/pynamer.py
--rw-rw-rw-   0        0        0      386 2023-06-04 12:15:11.000000 pynamer-2.1.7/src/pynamer/setup.txt
--rw-rw-rw-   0        0        0      401 2023-05-21 12:10:39.000000 pynamer-2.1.7/src/pynamer/setup_base.txt
--rw-rw-rw-   0        0        0    11098 2023-06-14 17:55:57.000000 pynamer-2.1.7/src/pynamer/utils.py
--rw-rw-rw-   0        0        0    11922 2023-06-19 18:58:14.000000 pynamer-2.1.7/src/pynamer/validators.py
-drwxrwxrwx   0        0        0        0 2023-06-19 19:04:54.898025 pynamer-2.1.7/src/pynamer.egg-info/
--rw-rw-rw-   0        0        0    19784 2023-06-19 19:04:54.000000 pynamer-2.1.7/src/pynamer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1215 2023-06-19 19:04:54.000000 pynamer-2.1.7/src/pynamer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 19:04:54.000000 pynamer-2.1.7/src/pynamer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-19 19:04:54.000000 pynamer-2.1.7/src/pynamer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      188 2023-06-19 19:04:54.000000 pynamer-2.1.7/src/pynamer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-19 19:04:54.000000 pynamer-2.1.7/src/pynamer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 19:04:55.231044 pynamer-2.1.7/tests/
--rw-rw-rw-   0        0        0     2159 2023-06-12 20:06:37.000000 pynamer-2.1.7/tests/test_args.py
--rw-rw-rw-   0        0        0     2000 2023-05-24 15:55:39.000000 pynamer-2.1.7/tests/test_build_dist.py
--rw-rw-rw-   0        0        0     1102 2023-05-24 15:55:39.000000 pynamer-2.1.7/tests/test_cleanup.py
--rw-rw-rw-   0        0        0     1222 2023-05-24 15:55:39.000000 pynamer-2.1.7/tests/test_create_setup_file.py
--rw-rw-rw-   0        0        0     1617 2023-06-04 12:01:20.000000 pynamer-2.1.7/tests/test_defaults.py
--rw-rw-rw-   0        0        0      529 2023-05-24 15:55:39.000000 pynamer-2.1.7/tests/test_delete_director.py
--rw-rw-rw-   0        0        0     1289 2023-05-21 12:10:39.000000 pynamer-2.1.7/tests/test_feedback.py
--rw-rw-rw-   0        0        0     2900 2023-06-15 11:28:35.000000 pynamer-2.1.7/tests/test_final_analysis.py
--rw-rw-rw-   0        0        0      738 2023-05-21 12:10:39.000000 pynamer-2.1.7/tests/test_find_pypirc_file.py
--rw-rw-rw-   0        0        0     1484 2023-06-14 19:03:12.000000 pynamer-2.1.7/tests/test_generate_pypi_index.py
--rw-rw-rw-   0        0        0     1712 2023-06-06 13:17:16.000000 pynamer-2.1.7/tests/test_get_homepage.py
--rw-rw-rw-   0        0        0     2025 2023-06-12 20:09:06.000000 pynamer-2.1.7/tests/test_github_meta.py
--rw-rw-rw-   0        0        0      329 2023-06-07 13:07:48.000000 pynamer-2.1.7/tests/test_is_valid_package_name.py
--rw-rw-rw-   0        0        0     2568 2023-06-06 13:17:15.000000 pynamer-2.1.7/tests/test_ping_json.py
--rw-rw-rw-   0        0        0     1547 2023-05-21 12:10:39.000000 pynamer-2.1.7/tests/test_ping_project.py
--rw-rw-rw-   0        0        0      522 2023-05-21 12:10:39.000000 pynamer-2.1.7/tests/test_process_input_file.py
--rw-rw-rw-   0        0        0     1129 2023-05-21 12:10:39.000000 pynamer-2.1.7/tests/test_pypi_search.py
--rw-rw-rw-   0        0        0      515 2023-05-24 15:55:39.000000 pynamer-2.1.7/tests/test_pypi_search_index.py
--rw-rw-rw-   0        0        0      746 2023-05-24 15:55:39.000000 pynamer-2.1.7/tests/test_rename_project_dir.py
--rw-rw-rw-   0        0        0      914 2023-05-24 15:55:39.000000 pynamer-2.1.7/tests/test_upload_dist.py
--rw-rw-rw-   0        0        0     1325 2023-06-14 17:55:57.000000 pynamer-2.1.7/tests/test_utils_search_json.py
--rw-rw-rw-   0        0        0     1707 2023-05-31 14:17:44.000000 pynamer-2.1.7/tests/test_utils_version.py
--rw-rw-rw-   0        0        0      647 2023-05-21 12:10:39.000000 pynamer-2.1.7/tests/test_write_output_file.py
+drwxrwxrwx   0        0        0        0 2023-07-01 15:01:58.358193 pynamer-2.1.8/
+-rw-rw-rw-   0        0        0      172 2023-05-21 12:10:39.000000 pynamer-2.1.8/AUTHORS.md
+-rw-rw-rw-   0        0        0    12777 2023-07-01 15:01:42.000000 pynamer-2.1.8/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1095 2023-05-21 12:10:39.000000 pynamer-2.1.8/LICENSE
+-rw-rw-rw-   0        0        0      237 2023-05-21 12:10:39.000000 pynamer-2.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0    20867 2023-07-01 15:01:58.358193 pynamer-2.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0    18805 2023-07-01 10:24:32.000000 pynamer-2.1.8/README.md
+-rw-rw-rw-   0        0        0     2183 2023-06-11 20:09:06.000000 pynamer-2.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0     2344 2023-07-01 15:01:58.361188 pynamer-2.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      109 2023-04-21 12:29:15.000000 pynamer-2.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 15:01:58.235612 pynamer-2.1.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-01 15:01:58.297197 pynamer-2.1.8/src/pynamer/
+-rw-rw-rw-   0        0        0       11 2023-05-21 12:10:39.000000 pynamer-2.1.8/src/pynamer/README.md
+-rw-rw-rw-   0        0        0     1989 2023-07-01 15:01:43.000000 pynamer-2.1.8/src/pynamer/__init__.py
+-rw-rw-rw-   0        0        0       54 2023-06-24 19:33:38.000000 pynamer-2.1.8/src/pynamer/__main__.py
+-rw-rw-rw-   0        0        0     9736 2023-05-29 10:07:59.000000 pynamer-2.1.8/src/pynamer/builder.py
+-rw-rw-rw-   0        0        0     2462 2023-06-12 20:06:37.000000 pynamer-2.1.8/src/pynamer/cli.py
+-rw-rw-rw-   0        0        0      863 2023-06-12 20:04:32.000000 pynamer-2.1.8/src/pynamer/config.py
+drwxrwxrwx   0        0        0        0 2023-07-01 15:01:58.310190 pynamer-2.1.8/src/pynamer/project_name/
+-rw-rw-rw-   0        0        0        0 2023-05-21 12:10:39.000000 pynamer-2.1.8/src/pynamer/project_name/__init__.py
+-rw-rw-rw-   0        0        0     7935 2023-06-17 17:24:20.000000 pynamer-2.1.8/src/pynamer/pynamer.py
+-rw-rw-rw-   0        0        0      386 2023-06-04 12:15:11.000000 pynamer-2.1.8/src/pynamer/setup.txt
+-rw-rw-rw-   0        0        0      401 2023-05-21 12:10:39.000000 pynamer-2.1.8/src/pynamer/setup_base.txt
+-rw-rw-rw-   0        0        0    11098 2023-06-14 17:55:57.000000 pynamer-2.1.8/src/pynamer/utils.py
+-rw-rw-rw-   0        0        0    12061 2023-06-30 16:49:28.000000 pynamer-2.1.8/src/pynamer/validators.py
+drwxrwxrwx   0        0        0        0 2023-07-01 15:01:58.308193 pynamer-2.1.8/src/pynamer.egg-info/
+-rw-rw-rw-   0        0        0    20867 2023-07-01 15:01:58.000000 pynamer-2.1.8/src/pynamer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1239 2023-07-01 15:01:58.000000 pynamer-2.1.8/src/pynamer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 15:01:58.000000 pynamer-2.1.8/src/pynamer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-01 15:01:58.000000 pynamer-2.1.8/src/pynamer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      188 2023-07-01 15:01:58.000000 pynamer-2.1.8/src/pynamer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-01 15:01:58.000000 pynamer-2.1.8/src/pynamer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 15:01:58.355189 pynamer-2.1.8/tests/
+-rw-rw-rw-   0        0        0     2159 2023-06-12 20:06:37.000000 pynamer-2.1.8/tests/test_args.py
+-rw-rw-rw-   0        0        0     2000 2023-05-24 15:55:39.000000 pynamer-2.1.8/tests/test_build_dist.py
+-rw-rw-rw-   0        0        0     1102 2023-05-24 15:55:39.000000 pynamer-2.1.8/tests/test_cleanup.py
+-rw-rw-rw-   0        0        0     1222 2023-05-24 15:55:39.000000 pynamer-2.1.8/tests/test_create_setup_file.py
+-rw-rw-rw-   0        0        0     1617 2023-06-04 12:01:20.000000 pynamer-2.1.8/tests/test_defaults.py
+-rw-rw-rw-   0        0        0      529 2023-05-24 15:55:39.000000 pynamer-2.1.8/tests/test_delete_director.py
+-rw-rw-rw-   0        0        0     1289 2023-05-21 12:10:39.000000 pynamer-2.1.8/tests/test_feedback.py
+-rw-rw-rw-   0        0        0     2900 2023-06-15 11:28:35.000000 pynamer-2.1.8/tests/test_final_analysis.py
+-rw-rw-rw-   0        0        0      738 2023-05-21 12:10:39.000000 pynamer-2.1.8/tests/test_find_pypirc_file.py
+-rw-rw-rw-   0        0        0     1484 2023-06-14 19:03:12.000000 pynamer-2.1.8/tests/test_generate_pypi_index.py
+-rw-rw-rw-   0        0        0     1712 2023-06-06 13:17:16.000000 pynamer-2.1.8/tests/test_get_homepage.py
+-rw-rw-rw-   0        0        0     1987 2023-07-01 14:49:34.000000 pynamer-2.1.8/tests/test_github_meta.py
+-rw-rw-rw-   0        0        0      329 2023-06-07 13:07:48.000000 pynamer-2.1.8/tests/test_is_valid_package_name.py
+-rw-rw-rw-   0        0        0     2568 2023-06-06 13:17:15.000000 pynamer-2.1.8/tests/test_ping_json.py
+-rw-rw-rw-   0        0        0     1547 2023-05-21 12:10:39.000000 pynamer-2.1.8/tests/test_ping_project.py
+-rw-rw-rw-   0        0        0      522 2023-05-21 12:10:39.000000 pynamer-2.1.8/tests/test_process_input_file.py
+-rw-rw-rw-   0        0        0     1129 2023-05-21 12:10:39.000000 pynamer-2.1.8/tests/test_pypi_search.py
+-rw-rw-rw-   0        0        0      515 2023-05-24 15:55:39.000000 pynamer-2.1.8/tests/test_pypi_search_index.py
+-rw-rw-rw-   0        0        0      746 2023-05-24 15:55:39.000000 pynamer-2.1.8/tests/test_rename_project_dir.py
+-rw-rw-rw-   0        0        0      914 2023-05-24 15:55:39.000000 pynamer-2.1.8/tests/test_upload_dist.py
+-rw-rw-rw-   0        0        0     1325 2023-06-14 17:55:57.000000 pynamer-2.1.8/tests/test_utils_search_json.py
+-rw-rw-rw-   0        0        0     1707 2023-05-31 14:17:44.000000 pynamer-2.1.8/tests/test_utils_version.py
+-rw-rw-rw-   0        0        0      647 2023-05-21 12:10:39.000000 pynamer-2.1.8/tests/test_write_output_file.py
```

### Comparing `pynamer-2.1.7/CHANGELOG.md` & `pynamer-2.1.8/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.1.8 (2023-07-01)
+### Documentation
+* Update hyperlinks ([`68a4f66`](https://github.com/Stephen-RA-King/pynamer/commit/68a4f665b642795589c354bc3e192ff8038e19c6))
+* Update docker image usage ([`9637e54`](https://github.com/Stephen-RA-King/pynamer/commit/9637e54529e1113daea1e6c1ce6b8bf785d16aa0))
+* Minor case change ([`5c0535d`](https://github.com/Stephen-RA-King/pynamer/commit/5c0535d78b48a2efdaede61ff675359c78df135b))
+* Add openssf badge scorecard ([`779a9fe`](https://github.com/Stephen-RA-King/pynamer/commit/779a9fec1e400cfd3400ad5dcace6f9121de5bc3))
+* Update openssf badge ([`d196617`](https://github.com/Stephen-RA-King/pynamer/commit/d1966179c7dcec1ac872595b8278ad5501bafd2e))
+* Add openssf details ([`6fe62f8`](https://github.com/Stephen-RA-King/pynamer/commit/6fe62f8f5450949f4e37638f293457052061de61))
+
 ## v2.1.7 (2023-06-19)
 ### Fix
 * Account for hompepoage beginning with http: ([`d9dcb50`](https://github.com/Stephen-RA-King/pynamer/commit/d9dcb50b4e6321d681a16aeba88bc2a2908f1005))
 
 ## v2.1.6 (2023-06-17)
 ### Fix
 * Error message regarding pypirc file before registration ([`ded4143`](https://github.com/Stephen-RA-King/pynamer/commit/ded4143062a1e2fb5cf74c2912dea692d64fac17))
```

### Comparing `pynamer-2.1.7/LICENSE` & `pynamer-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.7/PKG-INFO` & `pynamer-2.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 2.1.7
+Version: 2.1.8
 Summary: Utility to find an available package name in the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
 License: MIT
-Project-URL: documentation, https://pynamer.readthedocs.io/en/latest/
+Project-URL: Bug Tracker, https://github.com/Stephen-RA-King/pynamer/issues
+Project-URL: CI, https://github.com/Stephen-RA-King/pynamer/actions
+Project-URL: Documentation, https://pynamer.readthedocs.io/en/latest/
 Project-URL: Release Notes, https://github.com/Stephen-RA-King/pynamer/releases
 Project-URL: Source Code, https://github.com/Stephen-RA-King/pynamer/
-Project-URL: Issue Tracker, https://github.com/Stephen-RA-King/pynamer/issues
 Keywords: available-on-pypi,pip-search,packaging,naming,name-generation,names,pypi,packaging,naming-conventions
 Platform: Any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -48,14 +49,16 @@
 [![Code style: black][black-image]][black-url]
 [![Checked with mypy][mypy-image]][mypy-url]
 [![security: bandit][bandit-image]][bandit-url]
 [![Commitizen friendly][commitizen-image]][commitizen-url]
 [![Conventional Commits][conventional-commits-image]][conventional-commits-url]
 [![DeepSource][deepsource-image]][deepsource-url]
 [![license][license-image]][license-url]
+[![pydough][pydough-image]][pydough-url]
+<!-- [![OpenSSFScorecard][openssf-image]][openssf-url] -->
 
 As a pseudo replacement for pip search, pynamer will quickly ascertain if a project name is 'available' in PyPI.
 
 ![](assets/pynamer1.png)
 
 # Contents
 
@@ -412,14 +415,36 @@
 ```
 
 Using a name similar to to an existing package name is a security issue.
 
 Malicious players will try to create project names that are frequently mistyped for large popular projects, thereby facilitating installation of a malicious project.
 e.g. replacing "L" / "l" with the number 1 or "o" / "O" with 0. The Software utilized by PyPI can be found on GitHub: [warehouse](https://github.com/pypi/warehouse).
 
+## Using the Docker Image
+
+Pull the latest image from the Hub.
+```bash
+~ $ docker pull sraking/pynamer
+```
+Run the image.
+```bash
+~ $ docker run -it sraking/pynamer /bin/bash
+```
+Use the command line as normal in the container.
+
+```bash
+root@4d315992ca28:/app# pynamer
+usage: pynamer [-h] [-r] [-v] [-g] [-m] [-s] [-w] [-f FILENAME] [-o FILENAME] [--version] [projects ...]
+
+Determine if project name is available on pypi with the option to 'register' it for future use if available
+...
+```
+
+
+
 ## Documentation
 
 ---
 
 [**Read the Docs**](https://pynamer.readthedocs.io/en/latest/)
 
 -   [**Credits**](https://pynamer.readthedocs.io/en/latest/example.html)
@@ -436,24 +461,24 @@
 
 ---
 
 [![Linkedin](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
 [![PyPI repository](assets/pypi.png)](https://pypi.org/project/pynamer)
 [![Docker](assets/docker.png)](https://hub.docker.com/r/sraking/pynamer)
-[![](assets/www.png)](https://www.justpython.tech)
+[![](assets/www.png)](https://stephen-ra-king.github.io/justpython/)
 [![](assets/email.png)](mailto:sking.github@gmail.com)
 
-Stephen R A King : [sking.github@gmail.com](mailto:sking.github@gmail.com)
+Author: Stephen King ([sking.github@gmail.com](mailto:sking.github@gmail.com))
 
 Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
-Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.2
+Created with Cookiecutter template: [![pydough][pydough-image]][pydough-url] version 1.2.2
 
-[![DOI](https://zenodo.org/badge/631029310.svg)](https://zenodo.org/badge/latestdoi/631029310)
+Digital object identifier: [![DOI](https://zenodo.org/badge/631029310.svg)](https://zenodo.org/badge/latestdoi/631029310)
 
 <!-- Markdown link & img dfn's -->
 
 [bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
 [bandit-url]: https://github.com/PyCQA/bandit
 [black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-url]: https://github.com/psf/black
@@ -466,16 +491,16 @@
 [codefactor-url]: https://www.codefactor.io/repository/github/Stephen-RA-King/pynamer
 [codeql-image]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/github-code-scanning/codeql/badge.svg
 [codeql-url]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/github-code-scanning/codeql
 [commitizen-image]: https://img.shields.io/badge/commitizen-friendly-brightgreen.svg
 [commitizen-url]: http://commitizen.github.io/cz-cli/
 [conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?style=flat-square
 [conventional-commits-url]: https://conventionalcommits.org
-[deepsource-image]: https://static.deepsource.io/deepsource-badge-light-mini.svg
-[deepsource-url]: https://deepsource.io/gh/Stephen-RA-King/pynamer/?ref=repository-badge
+[deepsource-image]: https://app.deepsource.com/gh/Stephen-RA-King/pynamer.svg/?label=active+issues&show_trend=true&token=SGo-Vr17NUYVQaEWkU9rBb6Y
+[deepsource-url]: https://app.deepsource.com/gh/Stephen-RA-King/pynamer/?ref=repository-badge
 [docker-image]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/docker-image.yml/badge.svg
 [docker-url]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/docker-image.yml
 [downloads-image]: https://static.pepy.tech/personalized-badge/pynamer?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads
 [downloads-url]: https://pepy.tech/project/pynamer
 [format-image]: https://img.shields.io/pypi/format/pynamer
 [isort-image]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
 [isort-url]: https://github.com/pycqa/isort/
@@ -483,19 +508,22 @@
 [lgtm-alerts-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynamer/alerts/
 [lgtm-quality-image]: https://img.shields.io/lgtm/grade/python/g/Stephen-RA-King/pynamer.svg?logo=lgtm&logoWidth=18
 [lgtm-quality-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynamer/context:python
 [license-image]: https://img.shields.io/pypi/l/pynamer
 [license-url]: https://github.com/Stephen-RA-King/pynamer/blob/main/LICENSE
 [mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
 [mypy-url]: http://mypy-lang.org/
+[openssf-image]: https://api.securityscorecards.dev/projects/github.com/Stephen-RA-King/pynamer/badge
+[openssf-url]: https://api.securityscorecards.dev/projects/github.com/Stephen-RA-King/pynamer
 [pipx-url]: https://pypa.github.io/pipx/
 [pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
 [pre-commit-url]: https://github.com/pre-commit/pre-commit
 [pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/pynamer/main.svg
 [pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/pynamer/main
+[pydough-image]: https://img.shields.io/badge/pydough-2023-orange
 [pydough-url]: https://github.com/Stephen-RA-King/pydough
 [pypi-image]: https://img.shields.io/pypi/v/pynamer.svg
 [pypi-url]: https://pypi.org/project/pynamer/
 [python-version-image]: https://img.shields.io/pypi/pyversions/pynamer
 [readthedocs-image]: https://readthedocs.org/projects/pynamer/badge/?version=latest
 [readthedocs-url]: https://pynamer.readthedocs.io/en/latest/?badge=latest
 [status-image]: https://img.shields.io/pypi/status/pynamer.svg
```

### Comparing `pynamer-2.1.7/README.md` & `pynamer-2.1.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 [![Code style: black][black-image]][black-url]
 [![Checked with mypy][mypy-image]][mypy-url]
 [![security: bandit][bandit-image]][bandit-url]
 [![Commitizen friendly][commitizen-image]][commitizen-url]
 [![Conventional Commits][conventional-commits-image]][conventional-commits-url]
 [![DeepSource][deepsource-image]][deepsource-url]
 [![license][license-image]][license-url]
+[![pydough][pydough-image]][pydough-url]
+<!-- [![OpenSSFScorecard][openssf-image]][openssf-url] -->
 
 As a pseudo replacement for pip search, pynamer will quickly ascertain if a project name is 'available' in PyPI.
 
 ![](assets/pynamer1.png)
 
 # Contents
 
@@ -380,14 +382,36 @@
 ```
 
 Using a name similar to to an existing package name is a security issue.
 
 Malicious players will try to create project names that are frequently mistyped for large popular projects, thereby facilitating installation of a malicious project.
 e.g. replacing "L" / "l" with the number 1 or "o" / "O" with 0. The Software utilized by PyPI can be found on GitHub: [warehouse](https://github.com/pypi/warehouse).
 
+## Using the Docker Image
+
+Pull the latest image from the Hub.
+```bash
+~ $ docker pull sraking/pynamer
+```
+Run the image.
+```bash
+~ $ docker run -it sraking/pynamer /bin/bash
+```
+Use the command line as normal in the container.
+
+```bash
+root@4d315992ca28:/app# pynamer
+usage: pynamer [-h] [-r] [-v] [-g] [-m] [-s] [-w] [-f FILENAME] [-o FILENAME] [--version] [projects ...]
+
+Determine if project name is available on pypi with the option to 'register' it for future use if available
+...
+```
+
+
+
 ## Documentation
 
 ---
 
 [**Read the Docs**](https://pynamer.readthedocs.io/en/latest/)
 
 -   [**Credits**](https://pynamer.readthedocs.io/en/latest/example.html)
@@ -404,24 +428,24 @@
 
 ---
 
 [![Linkedin](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
 [![PyPI repository](assets/pypi.png)](https://pypi.org/project/pynamer)
 [![Docker](assets/docker.png)](https://hub.docker.com/r/sraking/pynamer)
-[![](assets/www.png)](https://www.justpython.tech)
+[![](assets/www.png)](https://stephen-ra-king.github.io/justpython/)
 [![](assets/email.png)](mailto:sking.github@gmail.com)
 
-Stephen R A King : [sking.github@gmail.com](mailto:sking.github@gmail.com)
+Author: Stephen King ([sking.github@gmail.com](mailto:sking.github@gmail.com))
 
 Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
-Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.2
+Created with Cookiecutter template: [![pydough][pydough-image]][pydough-url] version 1.2.2
 
-[![DOI](https://zenodo.org/badge/631029310.svg)](https://zenodo.org/badge/latestdoi/631029310)
+Digital object identifier: [![DOI](https://zenodo.org/badge/631029310.svg)](https://zenodo.org/badge/latestdoi/631029310)
 
 <!-- Markdown link & img dfn's -->
 
 [bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
 [bandit-url]: https://github.com/PyCQA/bandit
 [black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-url]: https://github.com/psf/black
@@ -434,16 +458,16 @@
 [codefactor-url]: https://www.codefactor.io/repository/github/Stephen-RA-King/pynamer
 [codeql-image]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/github-code-scanning/codeql/badge.svg
 [codeql-url]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/github-code-scanning/codeql
 [commitizen-image]: https://img.shields.io/badge/commitizen-friendly-brightgreen.svg
 [commitizen-url]: http://commitizen.github.io/cz-cli/
 [conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?style=flat-square
 [conventional-commits-url]: https://conventionalcommits.org
-[deepsource-image]: https://static.deepsource.io/deepsource-badge-light-mini.svg
-[deepsource-url]: https://deepsource.io/gh/Stephen-RA-King/pynamer/?ref=repository-badge
+[deepsource-image]: https://app.deepsource.com/gh/Stephen-RA-King/pynamer.svg/?label=active+issues&show_trend=true&token=SGo-Vr17NUYVQaEWkU9rBb6Y
+[deepsource-url]: https://app.deepsource.com/gh/Stephen-RA-King/pynamer/?ref=repository-badge
 [docker-image]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/docker-image.yml/badge.svg
 [docker-url]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/docker-image.yml
 [downloads-image]: https://static.pepy.tech/personalized-badge/pynamer?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads
 [downloads-url]: https://pepy.tech/project/pynamer
 [format-image]: https://img.shields.io/pypi/format/pynamer
 [isort-image]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
 [isort-url]: https://github.com/pycqa/isort/
@@ -451,19 +475,22 @@
 [lgtm-alerts-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynamer/alerts/
 [lgtm-quality-image]: https://img.shields.io/lgtm/grade/python/g/Stephen-RA-King/pynamer.svg?logo=lgtm&logoWidth=18
 [lgtm-quality-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynamer/context:python
 [license-image]: https://img.shields.io/pypi/l/pynamer
 [license-url]: https://github.com/Stephen-RA-King/pynamer/blob/main/LICENSE
 [mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
 [mypy-url]: http://mypy-lang.org/
+[openssf-image]: https://api.securityscorecards.dev/projects/github.com/Stephen-RA-King/pynamer/badge
+[openssf-url]: https://api.securityscorecards.dev/projects/github.com/Stephen-RA-King/pynamer
 [pipx-url]: https://pypa.github.io/pipx/
 [pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
 [pre-commit-url]: https://github.com/pre-commit/pre-commit
 [pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/pynamer/main.svg
 [pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/pynamer/main
+[pydough-image]: https://img.shields.io/badge/pydough-2023-orange
 [pydough-url]: https://github.com/Stephen-RA-King/pydough
 [pypi-image]: https://img.shields.io/pypi/v/pynamer.svg
 [pypi-url]: https://pypi.org/project/pynamer/
 [python-version-image]: https://img.shields.io/pypi/pyversions/pynamer
 [readthedocs-image]: https://readthedocs.org/projects/pynamer/badge/?version=latest
 [readthedocs-url]: https://pynamer.readthedocs.io/en/latest/?badge=latest
 [status-image]: https://img.shields.io/pypi/status/pynamer.svg
```

### Comparing `pynamer-2.1.7/pyproject.toml` & `pynamer-2.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.7/setup.cfg` & `pynamer-2.1.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -38,106 +38,110 @@
 00000250: 6875 622e 636f 6d2f 5374 6570 6865 6e2d  hub.com/Stephen-
 00000260: 5241 2d4b 696e 672f 7079 6e61 6d65 722f  RA-King/pynamer/
 00000270: 6172 6368 6976 652f 7265 6673 2f68 6561  archive/refs/hea
 00000280: 6473 2f6d 6169 6e2e 7a69 700d 0a6c 6963  ds/main.zip..lic
 00000290: 656e 7365 203d 204d 4954 0d0a 6c69 6365  ense = MIT..lice
 000002a0: 6e73 655f 6669 6c65 7320 3d20 4c49 4345  nse_files = LICE
 000002b0: 4e53 450d 0a70 726f 6a65 6374 5f75 726c  NSE..project_url
-000002c0: 7320 3d20 0d0a 0964 6f63 756d 656e 7461  s = ...documenta
-000002d0: 7469 6f6e 203d 2068 7474 7073 3a2f 2f70  tion = https://p
-000002e0: 796e 616d 6572 2e72 6561 6474 6865 646f  ynamer.readthedo
-000002f0: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-00000300: 0d0a 0952 656c 6561 7365 204e 6f74 6573  ...Release Notes
-00000310: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
-00000320: 622e 636f 6d2f 5374 6570 6865 6e2d 5241  b.com/Stephen-RA
-00000330: 2d4b 696e 672f 7079 6e61 6d65 722f 7265  -King/pynamer/re
-00000340: 6c65 6173 6573 0d0a 0953 6f75 7263 6520  leases...Source 
-00000350: 436f 6465 203d 2068 7474 7073 3a2f 2f67  Code = https://g
-00000360: 6974 6875 622e 636f 6d2f 5374 6570 6865  ithub.com/Stephe
-00000370: 6e2d 5241 2d4b 696e 672f 7079 6e61 6d65  n-RA-King/pyname
-00000380: 722f 0d0a 0949 7373 7565 2054 7261 636b  r/...Issue Track
-00000390: 6572 203d 2068 7474 7073 3a2f 2f67 6974  er = https://git
-000003a0: 6875 622e 636f 6d2f 5374 6570 6865 6e2d  hub.com/Stephen-
-000003b0: 5241 2d4b 696e 672f 7079 6e61 6d65 722f  RA-King/pynamer/
-000003c0: 6973 7375 6573 0d0a 636c 6173 7369 6669  issues..classifi
-000003d0: 6572 7320 3d20 0d0a 0944 6576 656c 6f70  ers = ...Develop
-000003e0: 6d65 6e74 2053 7461 7475 7320 3a3a 2035  ment Status :: 5
-000003f0: 202d 2050 726f 6475 6374 696f 6e2f 5374   - Production/St
-00000400: 6162 6c65 0d0a 0945 6e76 6972 6f6e 6d65  able...Environme
-00000410: 6e74 203a 3a20 436f 6e73 6f6c 650d 0a09  nt :: Console...
-00000420: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
-00000430: 6520 3a3a 2044 6576 656c 6f70 6572 730d  e :: Developers.
-00000440: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
-00000450: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
-00000460: 204c 6963 656e 7365 0d0a 094f 7065 7261   License...Opera
-00000470: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
-00000480: 5320 496e 6465 7065 6e64 656e 740d 0a09  S Independent...
-00000490: 4e61 7475 7261 6c20 4c61 6e67 7561 6765  Natural Language
-000004a0: 203a 3a20 456e 676c 6973 680d 0a09 5072   :: English...Pr
-000004b0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000004c0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000004d0: 330d 0a09 5072 6f67 7261 6d6d 696e 6720  3...Programming 
-000004e0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000004f0: 6f6e 203a 3a20 3320 3a3a 204f 6e6c 790d  on :: 3 :: Only.
-00000500: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000510: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000520: 203a 3a20 332e 390d 0a09 5072 6f67 7261   :: 3.9...Progra
-00000530: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000540: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
-00000550: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-00000560: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000570: 6e20 3a3a 2033 2e31 310d 0a0d 0a5b 6f70  n :: 3.11....[op
-00000580: 7469 6f6e 735d 0d0a 7061 636b 6167 655f  tions]..package_
-00000590: 6469 7220 3d20 0d0a 093d 7372 630d 0a70  dir = ...=src..p
-000005a0: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
-000005b0: 0a69 6e63 6c75 6465 5f70 6163 6b61 6765  .include_package
-000005c0: 5f64 6174 6120 3d20 5472 7565 0d0a 7079  _data = True..py
-000005d0: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
-000005e0: 3e3d 332e 390d 0a69 6e73 7461 6c6c 5f72  >=3.9..install_r
-000005f0: 6571 7569 7265 7320 3d20 0d0a 0962 6561  equires = ...bea
-00000600: 7574 6966 756c 736f 7570 343e 3d34 2e31  utifulsoup4>=4.1
-00000610: 322e 320d 0a09 6275 696c 643e 3d30 2e31  2.2...build>=0.1
-00000620: 302e 300d 0a09 636f 6c6f 7261 6d61 3e3d  0.0...colorama>=
-00000630: 302e 342e 360d 0a09 6a69 6e6a 6132 3e3d  0.4.6...jinja2>=
-00000640: 332e 312e 320d 0a09 7061 636b 6167 696e  3.1.2...packagin
-00000650: 673e 3d32 332e 310d 0a09 7079 7468 6f6e  g>=23.1...python
-00000660: 2d64 6174 6575 7469 6c3e 3d32 2e38 2e32  -dateutil>=2.8.2
-00000670: 0d0a 0970 7979 616d 6c3e 3d36 2e30 0d0a  ...pyyaml>=6.0..
-00000680: 0972 6571 7565 7374 733e 3d32 2e33 302e  .requests>=2.30.
-00000690: 300d 0a09 7269 6368 3e3d 3133 2e33 2e35  0...rich>=13.3.5
-000006a0: 0d0a 0974 7164 6d3e 3d34 2e36 352e 300d  ...tqdm>=4.65.0.
-000006b0: 0a09 7477 696e 653e 3d33 2e38 2e30 0d0a  ..twine>=3.8.0..
-000006c0: 0977 6865 656c 3e3d 302e 3430 2e30 0d0a  .wheel>=0.40.0..
-000006d0: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
-000006e0: 6765 732e 6669 6e64 5d0d 0a77 6865 7265  ges.find]..where
-000006f0: 203d 2073 7263 0d0a 0d0a 5b6f 7074 696f   = src....[optio
-00000700: 6e73 2e70 6163 6b61 6765 5f64 6174 615d  ns.package_data]
-00000710: 0d0a 7079 6e61 6d65 7220 3d20 0d0a 0952  ..pynamer = ...R
-00000720: 4541 444d 452e 6d64 0d0a 0970 726f 6a65  EADME.md...proje
-00000730: 6374 5f6e 616d 650d 0a09 7072 6f6a 6563  ct_name...projec
-00000740: 745f 6e61 6d65 2f5f 5f69 6e69 745f 5f2e  t_name/__init__.
-00000750: 7079 0d0a 0973 6574 7570 2e74 7874 0d0a  py...setup.txt..
-00000760: 0973 6574 7570 5f62 6173 652e 7478 740d  .setup_base.txt.
-00000770: 0a0d 0a5b 6f70 7469 6f6e 732e 656e 7472  ...[options.entr
-00000780: 795f 706f 696e 7473 5d0d 0a63 6f6e 736f  y_points]..conso
-00000790: 6c65 5f73 6372 6970 7473 203d 200d 0a09  le_scripts = ...
-000007a0: 7079 6e61 6d65 7220 3d20 7079 6e61 6d65  pynamer = pyname
-000007b0: 722e 7079 6e61 6d65 723a 6d61 696e 0d0a  r.pynamer:main..
-000007c0: 0d0a 5b66 6c61 6b65 385d 0d0a 646f 6373  ..[flake8]..docs
-000007d0: 7472 696e 672d 636f 6e76 656e 7469 6f6e  tring-convention
-000007e0: 203d 206e 756d 7079 0d0a 6d61 782d 636f   = numpy..max-co
-000007f0: 6d70 6c65 7869 7479 203d 2031 380d 0a6d  mplexity = 18..m
-00000800: 6178 2d6c 696e 652d 6c65 6e67 7468 203d  ax-line-length =
-00000810: 2038 380d 0a73 656c 6563 7420 3d20 422c   88..select = B,
-00000820: 2042 392c 2043 2c20 442c 2045 2c20 462c   B9, C, D, E, F,
-00000830: 204e 2c20 570d 0a65 7863 6c75 6465 203d   N, W..exclude =
-00000840: 2074 6573 7473 2f2a 2c2e 746f 782f 2a2c   tests/*,.tox/*,
-00000850: 2e6e 6f78 2f2a 2c64 6f63 732f 2a2c 2e67  .nox/*,docs/*,.g
-00000860: 6974 2f2a 2c2e 6769 7468 7562 2f2a 0d0a  it/*,.github/*..
-00000870: 6967 6e6f 7265 203d 200d 0a09 4532 3033  ignore = ...E203
-00000880: 2c0d 0a09 5735 3033 2c0d 0a70 6572 2d66  ,...W503,..per-f
-00000890: 696c 652d 6967 6e6f 7265 7320 3d20 0d0a  ile-ignores = ..
-000008a0: 0970 796e 616d 6572 2e70 793a 4339 3031  .pynamer.py:C901
-000008b0: 0d0a 0962 7569 6c64 6572 2e70 793a 4339  ...builder.py:C9
-000008c0: 3031 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  01....[egg_info]
-000008d0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-000008e0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+000002c0: 7320 3d20 0d0a 0942 7567 2054 7261 636b  s = ...Bug Track
+000002d0: 6572 203d 2068 7474 7073 3a2f 2f67 6974  er = https://git
+000002e0: 6875 622e 636f 6d2f 5374 6570 6865 6e2d  hub.com/Stephen-
+000002f0: 5241 2d4b 696e 672f 7079 6e61 6d65 722f  RA-King/pynamer/
+00000300: 6973 7375 6573 0d0a 0943 4920 3d20 6874  issues...CI = ht
+00000310: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000320: 2f53 7465 7068 656e 2d52 412d 4b69 6e67  /Stephen-RA-King
+00000330: 2f70 796e 616d 6572 2f61 6374 696f 6e73  /pynamer/actions
+00000340: 0d0a 0944 6f63 756d 656e 7461 7469 6f6e  ...Documentation
+00000350: 203d 2068 7474 7073 3a2f 2f70 796e 616d   = https://pynam
+00000360: 6572 2e72 6561 6474 6865 646f 6373 2e69  er.readthedocs.i
+00000370: 6f2f 656e 2f6c 6174 6573 742f 0d0a 0952  o/en/latest/...R
+00000380: 656c 6561 7365 204e 6f74 6573 203d 2068  elease Notes = h
+00000390: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000003a0: 6d2f 5374 6570 6865 6e2d 5241 2d4b 696e  m/Stephen-RA-Kin
+000003b0: 672f 7079 6e61 6d65 722f 7265 6c65 6173  g/pynamer/releas
+000003c0: 6573 0d0a 0953 6f75 7263 6520 436f 6465  es...Source Code
+000003d0: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
+000003e0: 622e 636f 6d2f 5374 6570 6865 6e2d 5241  b.com/Stephen-RA
+000003f0: 2d4b 696e 672f 7079 6e61 6d65 722f 0d0a  -King/pynamer/..
+00000400: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
+00000410: 0944 6576 656c 6f70 6d65 6e74 2053 7461  .Development Sta
+00000420: 7475 7320 3a3a 2035 202d 2050 726f 6475  tus :: 5 - Produ
+00000430: 6374 696f 6e2f 5374 6162 6c65 0d0a 0945  ction/Stable...E
+00000440: 6e76 6972 6f6e 6d65 6e74 203a 3a20 436f  nvironment :: Co
+00000450: 6e73 6f6c 650d 0a09 496e 7465 6e64 6564  nsole...Intended
+00000460: 2041 7564 6965 6e63 6520 3a3a 2044 6576   Audience :: Dev
+00000470: 656c 6f70 6572 730d 0a09 4c69 6365 6e73  elopers...Licens
+00000480: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+00000490: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
+000004a0: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
+000004b0: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+000004c0: 6e64 656e 740d 0a09 4e61 7475 7261 6c20  ndent...Natural 
+000004d0: 4c61 6e67 7561 6765 203a 3a20 456e 676c  Language :: Engl
+000004e0: 6973 680d 0a09 5072 6f67 7261 6d6d 696e  ish...Programmin
+000004f0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000500: 7468 6f6e 203a 3a20 330d 0a09 5072 6f67  thon :: 3...Prog
+00000510: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000520: 203a 3a20 5079 7468 6f6e 203a 3a20 3320   :: Python :: 3 
+00000530: 3a3a 204f 6e6c 790d 0a09 5072 6f67 7261  :: Only...Progra
+00000540: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000550: 3a20 5079 7468 6f6e 203a 3a20 332e 390d  : Python :: 3.9.
+00000560: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000570: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000580: 203a 3a20 332e 3130 0d0a 0950 726f 6772   :: 3.10...Progr
+00000590: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000005a0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
+000005b0: 310d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  1....[options]..
+000005c0: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
+000005d0: 093d 7372 630d 0a70 6163 6b61 6765 7320  .=src..packages 
+000005e0: 3d20 6669 6e64 3a0d 0a69 6e63 6c75 6465  = find:..include
+000005f0: 5f70 6163 6b61 6765 5f64 6174 6120 3d20  _package_data = 
+00000600: 5472 7565 0d0a 7079 7468 6f6e 5f72 6571  True..python_req
+00000610: 7569 7265 7320 3d20 3e3d 332e 390d 0a69  uires = >=3.9..i
+00000620: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
+00000630: 3d20 0d0a 0962 6561 7574 6966 756c 736f  = ...beautifulso
+00000640: 7570 343e 3d34 2e31 322e 320d 0a09 6275  up4>=4.12.2...bu
+00000650: 696c 643e 3d30 2e31 302e 300d 0a09 636f  ild>=0.10.0...co
+00000660: 6c6f 7261 6d61 3e3d 302e 342e 360d 0a09  lorama>=0.4.6...
+00000670: 6a69 6e6a 6132 3e3d 332e 312e 320d 0a09  jinja2>=3.1.2...
+00000680: 7061 636b 6167 696e 673e 3d32 332e 310d  packaging>=23.1.
+00000690: 0a09 7079 7468 6f6e 2d64 6174 6575 7469  ..python-dateuti
+000006a0: 6c3e 3d32 2e38 2e32 0d0a 0970 7979 616d  l>=2.8.2...pyyam
+000006b0: 6c3e 3d36 2e30 0d0a 0972 6571 7565 7374  l>=6.0...request
+000006c0: 733e 3d32 2e33 302e 300d 0a09 7269 6368  s>=2.30.0...rich
+000006d0: 3e3d 3133 2e33 2e35 0d0a 0974 7164 6d3e  >=13.3.5...tqdm>
+000006e0: 3d34 2e36 352e 300d 0a09 7477 696e 653e  =4.65.0...twine>
+000006f0: 3d33 2e38 2e30 0d0a 0977 6865 656c 3e3d  =3.8.0...wheel>=
+00000700: 302e 3430 2e30 0d0a 0d0a 5b6f 7074 696f  0.40.0....[optio
+00000710: 6e73 2e70 6163 6b61 6765 732e 6669 6e64  ns.packages.find
+00000720: 5d0d 0a77 6865 7265 203d 2073 7263 0d0a  ]..where = src..
+00000730: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
+00000740: 6765 5f64 6174 615d 0d0a 7079 6e61 6d65  ge_data]..pyname
+00000750: 7220 3d20 0d0a 0952 4541 444d 452e 6d64  r = ...README.md
+00000760: 0d0a 0970 726f 6a65 6374 5f6e 616d 650d  ...project_name.
+00000770: 0a09 7072 6f6a 6563 745f 6e61 6d65 2f5f  ..project_name/_
+00000780: 5f69 6e69 745f 5f2e 7079 0d0a 0973 6574  _init__.py...set
+00000790: 7570 2e74 7874 0d0a 0973 6574 7570 5f62  up.txt...setup_b
+000007a0: 6173 652e 7478 740d 0a0d 0a5b 6f70 7469  ase.txt....[opti
+000007b0: 6f6e 732e 656e 7472 795f 706f 696e 7473  ons.entry_points
+000007c0: 5d0d 0a63 6f6e 736f 6c65 5f73 6372 6970  ]..console_scrip
+000007d0: 7473 203d 200d 0a09 7079 6e61 6d65 7220  ts = ...pynamer 
+000007e0: 3d20 7079 6e61 6d65 722e 7079 6e61 6d65  = pynamer.pyname
+000007f0: 723a 6d61 696e 0d0a 0d0a 5b66 6c61 6b65  r:main....[flake
+00000800: 385d 0d0a 646f 6373 7472 696e 672d 636f  8]..docstring-co
+00000810: 6e76 656e 7469 6f6e 203d 206e 756d 7079  nvention = numpy
+00000820: 0d0a 6d61 782d 636f 6d70 6c65 7869 7479  ..max-complexity
+00000830: 203d 2031 380d 0a6d 6178 2d6c 696e 652d   = 18..max-line-
+00000840: 6c65 6e67 7468 203d 2038 380d 0a73 656c  length = 88..sel
+00000850: 6563 7420 3d20 422c 2042 392c 2043 2c20  ect = B, B9, C, 
+00000860: 442c 2045 2c20 462c 204e 2c20 570d 0a65  D, E, F, N, W..e
+00000870: 7863 6c75 6465 203d 2074 6573 7473 2f2a  xclude = tests/*
+00000880: 2c2e 746f 782f 2a2c 2e6e 6f78 2f2a 2c64  ,.tox/*,.nox/*,d
+00000890: 6f63 732f 2a2c 2e67 6974 2f2a 2c2e 6769  ocs/*,.git/*,.gi
+000008a0: 7468 7562 2f2a 0d0a 6967 6e6f 7265 203d  thub/*..ignore =
+000008b0: 200d 0a09 4532 3033 2c0d 0a09 5735 3033   ...E203,...W503
+000008c0: 2c0d 0a70 6572 2d66 696c 652d 6967 6e6f  ,..per-file-igno
+000008d0: 7265 7320 3d20 0d0a 0970 796e 616d 6572  res = ...pynamer
+000008e0: 2e70 793a 4339 3031 0d0a 0962 7569 6c64  .py:C901...build
+000008f0: 6572 2e70 793a 4339 3031 0d0a 0d0a 5b65  er.py:C901....[e
+00000900: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+00000910: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+00000920: 203d 2030 0d0a 0d0a                       = 0....
```

### Comparing `pynamer-2.1.7/src/pynamer/__init__.py` & `pynamer-2.1.8/src/pynamer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pickle
 from importlib.resources import files
 
 # Third party modules
 import yaml
 
 __title__ = "pynamer"
-__version__ = "2.1.7"
+__version__ = "2.1.8"
 __author__ = "Stephen R A King"
 __description__ = (
     "Utility to find an available package name in the PyPI repository and register it "
 )
 __email__ = "sking.github@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Stephen R A King"
```

### Comparing `pynamer-2.1.7/src/pynamer/builder.py` & `pynamer-2.1.8/src/pynamer/builder.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.7/src/pynamer/cli.py` & `pynamer-2.1.8/src/pynamer/cli.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.7/src/pynamer/config.py` & `pynamer-2.1.8/src/pynamer/config.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.7/src/pynamer/pynamer.py` & `pynamer-2.1.8/src/pynamer/pynamer.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.7/src/pynamer/utils.py` & `pynamer-2.1.8/src/pynamer/utils.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.7/src/pynamer/validators.py` & `pynamer-2.1.8/src/pynamer/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,21 @@
                 "\n",
                 f"created:  {isoparse(repo_json['created_at']).date()}",
                 "\n",
                 f"updated:  {isoparse(repo_json['updated_at']).date()}",
             ]
         )
     if json_raw.status_code == 404:
-        return "".join([return_text, "repository does not exist"])
+        return "".join(
+            [
+                return_text,
+                "JSON API Does not exist.\n"
+                "This usually indicates a very old repository.",
+            ]
+        )
     return ""
 
 
 def _ping_project(project_name: str) -> bool:
     """Determines if the URL to the project exists in PyPIs project area.
 
     Args:
@@ -146,15 +152,15 @@
         logger.debug("%s FOUND in the project area of PyPI", project_name)
         return True
     logger.debug("%s NOT FOUND in the project area of PyPI", project_name)
     return False
 
 
 def _ping_json(project_name: str, stats: bool = False) -> str:
-    """Collects some details about the project if it exists.
+    """Collects some PyPI details about the project if it exists.
 
     Args:
         project_name:   the name of the project to test.
 
     Raises:
         SystemExit:     if any requests.RequestException occurs.
     """
```

### Comparing `pynamer-2.1.7/src/pynamer.egg-info/PKG-INFO` & `pynamer-2.1.8/src/pynamer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 2.1.7
+Version: 2.1.8
 Summary: Utility to find an available package name in the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
 License: MIT
-Project-URL: documentation, https://pynamer.readthedocs.io/en/latest/
+Project-URL: Bug Tracker, https://github.com/Stephen-RA-King/pynamer/issues
+Project-URL: CI, https://github.com/Stephen-RA-King/pynamer/actions
+Project-URL: Documentation, https://pynamer.readthedocs.io/en/latest/
 Project-URL: Release Notes, https://github.com/Stephen-RA-King/pynamer/releases
 Project-URL: Source Code, https://github.com/Stephen-RA-King/pynamer/
-Project-URL: Issue Tracker, https://github.com/Stephen-RA-King/pynamer/issues
 Keywords: available-on-pypi,pip-search,packaging,naming,name-generation,names,pypi,packaging,naming-conventions
 Platform: Any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -48,14 +49,16 @@
 [![Code style: black][black-image]][black-url]
 [![Checked with mypy][mypy-image]][mypy-url]
 [![security: bandit][bandit-image]][bandit-url]
 [![Commitizen friendly][commitizen-image]][commitizen-url]
 [![Conventional Commits][conventional-commits-image]][conventional-commits-url]
 [![DeepSource][deepsource-image]][deepsource-url]
 [![license][license-image]][license-url]
+[![pydough][pydough-image]][pydough-url]
+<!-- [![OpenSSFScorecard][openssf-image]][openssf-url] -->
 
 As a pseudo replacement for pip search, pynamer will quickly ascertain if a project name is 'available' in PyPI.
 
 ![](assets/pynamer1.png)
 
 # Contents
 
@@ -412,14 +415,36 @@
 ```
 
 Using a name similar to to an existing package name is a security issue.
 
 Malicious players will try to create project names that are frequently mistyped for large popular projects, thereby facilitating installation of a malicious project.
 e.g. replacing "L" / "l" with the number 1 or "o" / "O" with 0. The Software utilized by PyPI can be found on GitHub: [warehouse](https://github.com/pypi/warehouse).
 
+## Using the Docker Image
+
+Pull the latest image from the Hub.
+```bash
+~ $ docker pull sraking/pynamer
+```
+Run the image.
+```bash
+~ $ docker run -it sraking/pynamer /bin/bash
+```
+Use the command line as normal in the container.
+
+```bash
+root@4d315992ca28:/app# pynamer
+usage: pynamer [-h] [-r] [-v] [-g] [-m] [-s] [-w] [-f FILENAME] [-o FILENAME] [--version] [projects ...]
+
+Determine if project name is available on pypi with the option to 'register' it for future use if available
+...
+```
+
+
+
 ## Documentation
 
 ---
 
 [**Read the Docs**](https://pynamer.readthedocs.io/en/latest/)
 
 -   [**Credits**](https://pynamer.readthedocs.io/en/latest/example.html)
@@ -436,24 +461,24 @@
 
 ---
 
 [![Linkedin](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
 [![PyPI repository](assets/pypi.png)](https://pypi.org/project/pynamer)
 [![Docker](assets/docker.png)](https://hub.docker.com/r/sraking/pynamer)
-[![](assets/www.png)](https://www.justpython.tech)
+[![](assets/www.png)](https://stephen-ra-king.github.io/justpython/)
 [![](assets/email.png)](mailto:sking.github@gmail.com)
 
-Stephen R A King : [sking.github@gmail.com](mailto:sking.github@gmail.com)
+Author: Stephen King ([sking.github@gmail.com](mailto:sking.github@gmail.com))
 
 Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
-Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.2
+Created with Cookiecutter template: [![pydough][pydough-image]][pydough-url] version 1.2.2
 
-[![DOI](https://zenodo.org/badge/631029310.svg)](https://zenodo.org/badge/latestdoi/631029310)
+Digital object identifier: [![DOI](https://zenodo.org/badge/631029310.svg)](https://zenodo.org/badge/latestdoi/631029310)
 
 <!-- Markdown link & img dfn's -->
 
 [bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
 [bandit-url]: https://github.com/PyCQA/bandit
 [black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-url]: https://github.com/psf/black
@@ -466,16 +491,16 @@
 [codefactor-url]: https://www.codefactor.io/repository/github/Stephen-RA-King/pynamer
 [codeql-image]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/github-code-scanning/codeql/badge.svg
 [codeql-url]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/github-code-scanning/codeql
 [commitizen-image]: https://img.shields.io/badge/commitizen-friendly-brightgreen.svg
 [commitizen-url]: http://commitizen.github.io/cz-cli/
 [conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?style=flat-square
 [conventional-commits-url]: https://conventionalcommits.org
-[deepsource-image]: https://static.deepsource.io/deepsource-badge-light-mini.svg
-[deepsource-url]: https://deepsource.io/gh/Stephen-RA-King/pynamer/?ref=repository-badge
+[deepsource-image]: https://app.deepsource.com/gh/Stephen-RA-King/pynamer.svg/?label=active+issues&show_trend=true&token=SGo-Vr17NUYVQaEWkU9rBb6Y
+[deepsource-url]: https://app.deepsource.com/gh/Stephen-RA-King/pynamer/?ref=repository-badge
 [docker-image]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/docker-image.yml/badge.svg
 [docker-url]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/docker-image.yml
 [downloads-image]: https://static.pepy.tech/personalized-badge/pynamer?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads
 [downloads-url]: https://pepy.tech/project/pynamer
 [format-image]: https://img.shields.io/pypi/format/pynamer
 [isort-image]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
 [isort-url]: https://github.com/pycqa/isort/
@@ -483,19 +508,22 @@
 [lgtm-alerts-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynamer/alerts/
 [lgtm-quality-image]: https://img.shields.io/lgtm/grade/python/g/Stephen-RA-King/pynamer.svg?logo=lgtm&logoWidth=18
 [lgtm-quality-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynamer/context:python
 [license-image]: https://img.shields.io/pypi/l/pynamer
 [license-url]: https://github.com/Stephen-RA-King/pynamer/blob/main/LICENSE
 [mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
 [mypy-url]: http://mypy-lang.org/
+[openssf-image]: https://api.securityscorecards.dev/projects/github.com/Stephen-RA-King/pynamer/badge
+[openssf-url]: https://api.securityscorecards.dev/projects/github.com/Stephen-RA-King/pynamer
 [pipx-url]: https://pypa.github.io/pipx/
 [pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
 [pre-commit-url]: https://github.com/pre-commit/pre-commit
 [pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/pynamer/main.svg
 [pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/pynamer/main
+[pydough-image]: https://img.shields.io/badge/pydough-2023-orange
 [pydough-url]: https://github.com/Stephen-RA-King/pydough
 [pypi-image]: https://img.shields.io/pypi/v/pynamer.svg
 [pypi-url]: https://pypi.org/project/pynamer/
 [python-version-image]: https://img.shields.io/pypi/pyversions/pynamer
 [readthedocs-image]: https://readthedocs.org/projects/pynamer/badge/?version=latest
 [readthedocs-url]: https://pynamer.readthedocs.io/en/latest/?badge=latest
 [status-image]: https://img.shields.io/pypi/status/pynamer.svg
```

### Comparing `pynamer-2.1.7/src/pynamer.egg-info/SOURCES.txt` & `pynamer-2.1.8/src/pynamer.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/pynamer/README.md
 src/pynamer/__init__.py
+src/pynamer/__main__.py
 src/pynamer/builder.py
 src/pynamer/cli.py
 src/pynamer/config.py
 src/pynamer/pynamer.py
 src/pynamer/setup.txt
 src/pynamer/setup_base.txt
 src/pynamer/utils.py
```

### Comparing `pynamer-2.1.7/tests/test_args.py` & `pynamer-2.1.8/tests/test_args.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.7/tests/test_build_dist.py` & `pynamer-2.1.8/tests/test_build_dist.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.7/tests/test_cleanup.py` & `pynamer-2.1.8/tests/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.7/tests/test_create_setup_file.py` & `pynamer-2.1.8/tests/test_create_setup_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.7/tests/test_defaults.py` & `pynamer-2.1.8/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.7/tests/test_delete_director.py` & `pynamer-2.1.8/tests/test_delete_director.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.7/tests/test_feedback.py` & `pynamer-2.1.8/tests/test_feedback.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.7/tests/test_final_analysis.py` & `pynamer-2.1.8/tests/test_final_analysis.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.7/tests/test_find_pypirc_file.py` & `pynamer-2.1.8/tests/test_find_pypirc_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.7/tests/test_generate_pypi_index.py` & `pynamer-2.1.8/tests/test_generate_pypi_index.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.7/tests/test_get_homepage.py` & `pynamer-2.1.8/tests/test_get_homepage.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.7/tests/test_github_meta.py` & `pynamer-2.1.8/tests/test_github_meta.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-#!/usr/bin/env python3
-# Core Library modules
-import pickle
-from pathlib import Path
-
-# Third party modules
-import pytest
-import requests
-from requests.exceptions import ConnectTimeout
-
-# First party modules
-import pynamer
-
-BASE_DIR = Path(__file__).parents[0]
-
-
-expected_response_found = """
-
-GitHub Stats
-------------
-stars:    32616
-forks:    2102
-issues:   405
-license:  MIT License
-watching: 229
-created:  2018-03-14
-updated:  2023-06-12"""
-
-
-expected_response_http_error = """
-
-GitHub Stats
-------------
-GitHub can not be contacted"""
-
-
-expected_response_404_error = """
-
-GitHub Stats
-------------
-repository does not exist"""
-
-
-@pytest.fixture
-def mock_response_404(monkeypatch):
-    def mock_get(*args, **kwargs):
-        class MockResponse:
-            def __init__(self):
-                self.status_code = 404
-
-            def json(self):
-                return {}
-
-        return MockResponse()
-
-    monkeypatch.setattr(requests, "get", mock_get)
-
-
-def my_custom_get_found(url, **kwargs):
-    _pickle_file = BASE_DIR / "resources" / "requests_get_github_json_black.pickle"
-    _pickle_bytes = _pickle_file.read_bytes()
-    pickle_content = pickle.loads(_pickle_bytes)
-    return pickle_content
-
-
-def test_github_meta_black(monkeypatch):
-    monkeypatch.setattr(requests, "get", my_custom_get_found)
-    result = pynamer.validators._github_meta("https://github.com/psf/black")
-    assert result == expected_response_found
-
-
-def test_ping_json_error(monkeypatch):
-    def mock_requests_error(*args, **kwargs):
-        raise ConnectTimeout("Connection timed out")
-
-    monkeypatch.setattr(requests, "get", mock_requests_error)
-
-    result = pynamer.validators._github_meta("https://github.com/psf/black")
-    assert result == expected_response_http_error
-
-
-def test_ping_json_not_exist(mock_response_404):
-    result = pynamer.validators._github_meta("https://github.com/psf/black")
-    assert result == expected_response_404_error
+#!/usr/bin/env python3
+# Core Library modules
+import pickle
+from pathlib import Path
+
+# Third party modules
+import pytest
+import requests
+from requests.exceptions import ConnectTimeout
+
+# First party modules
+import pynamer
+
+BASE_DIR = Path(__file__).parents[0]
+
+
+expected_response_found = """
+
+GitHub Stats
+------------
+stars:    32616
+forks:    2102
+issues:   405
+license:  MIT License
+watching: 229
+created:  2018-03-14
+updated:  2023-06-12"""
+
+
+expected_response_http_error = """
+
+GitHub Stats
+------------
+GitHub can not be contacted"""
+
+
+expected_response_404_error = """
+
+GitHub Stats
+------------
+JSON API Does not exist.\nThis usually indicates a very old repository."""
+
+
+@pytest.fixture
+def mock_response_404(monkeypatch):
+    def mock_get(*args, **kwargs):
+        class MockResponse:
+            def __init__(self):
+                self.status_code = 404
+
+            def json(self):
+                return {}
+
+        return MockResponse()
+
+    monkeypatch.setattr(requests, "get", mock_get)
+
+
+def my_custom_get_found(url, **kwargs):
+    _pickle_file = BASE_DIR / "resources" / "requests_get_github_json_black.pickle"
+    _pickle_bytes = _pickle_file.read_bytes()
+    pickle_content = pickle.loads(_pickle_bytes)
+    return pickle_content
+
+
+def test_github_meta_black(monkeypatch):
+    monkeypatch.setattr(requests, "get", my_custom_get_found)
+    result = pynamer.validators._github_meta("https://github.com/psf/black")
+    assert result == expected_response_found
+
+
+def test_ping_json_error(monkeypatch):
+    def mock_requests_error(*args, **kwargs):
+        raise ConnectTimeout("Connection timed out")
+
+    monkeypatch.setattr(requests, "get", mock_requests_error)
+
+    result = pynamer.validators._github_meta("https://github.com/psf/black")
+    assert result == expected_response_http_error
+
+
+def test_ping_json_not_exist(mock_response_404):
+    result = pynamer.validators._github_meta("https://github.com/psf/black")
+    assert result == expected_response_404_error
```

### Comparing `pynamer-2.1.7/tests/test_ping_json.py` & `pynamer-2.1.8/tests/test_ping_json.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.7/tests/test_ping_project.py` & `pynamer-2.1.8/tests/test_ping_project.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.7/tests/test_process_input_file.py` & `pynamer-2.1.8/tests/test_process_input_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.7/tests/test_pypi_search.py` & `pynamer-2.1.8/tests/test_pypi_search.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.7/tests/test_pypi_search_index.py` & `pynamer-2.1.8/tests/test_pypi_search_index.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.7/tests/test_rename_project_dir.py` & `pynamer-2.1.8/tests/test_rename_project_dir.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.7/tests/test_upload_dist.py` & `pynamer-2.1.8/tests/test_upload_dist.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.7/tests/test_utils_search_json.py` & `pynamer-2.1.8/tests/test_utils_search_json.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.7/tests/test_utils_version.py` & `pynamer-2.1.8/tests/test_utils_version.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.7/tests/test_write_output_file.py` & `pynamer-2.1.8/tests/test_write_output_file.py`

 * *Files identical despite different names*

