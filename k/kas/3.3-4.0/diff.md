# Comparing `tmp/kas-3.3.tar.gz` & `tmp/kas-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kas-3.3.tar", last modified: Tue Jun 20 19:26:55 2023, max compression
+gzip compressed data, was "dist/kas-4.0.tar", last modified: Sat Jul  1 11:36:50 2023, max compression
```

## Comparing `kas-3.3.tar` & `kas-4.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 jan       (1000) users      (100)        0 2023-06-20 19:26:55.000000 kas-3.3/
--rw-r--r--   0 jan       (1000) users      (100)     2878 2023-06-20 19:26:55.000000 kas-3.3/PKG-INFO
--rw-r--r--   0 jan       (1000) users      (100)     1624 2023-04-08 06:54:12.000000 kas-3.3/README.rst
-drwxr-xr-x   0 jan       (1000) users      (100)        0 2023-06-20 19:26:55.000000 kas-3.3/kas/
--rw-r--r--   0 jan       (1000) users      (100)     1527 2020-12-06 06:22:49.000000 kas-3.3/kas/__init__.py
--rw-r--r--   0 jan       (1000) users      (100)     1330 2021-09-13 11:52:25.000000 kas-3.3/kas/__main__.py
--rw-r--r--   0 jan       (1000) users      (100)     1420 2023-06-20 19:26:48.000000 kas-3.3/kas/__version__.py
--rw-r--r--   0 jan       (1000) users      (100)     7155 2023-06-10 06:39:22.000000 kas-3.3/kas/config.py
--rw-r--r--   0 jan       (1000) users      (100)     1455 2021-10-08 09:03:16.000000 kas-3.3/kas/configschema.py
--rw-r--r--   0 jan       (1000) users      (100)     4525 2022-10-28 05:38:25.000000 kas-3.3/kas/context.py
--rw-r--r--   0 jan       (1000) users      (100)    12259 2023-06-10 06:39:22.000000 kas-3.3/kas/includehandler.py
--rw-r--r--   0 jan       (1000) users      (100)     6574 2023-05-28 10:39:04.000000 kas-3.3/kas/kas.py
--rw-r--r--   0 jan       (1000) users      (100)     2872 2023-05-19 05:17:03.000000 kas-3.3/kas/kasusererror.py
--rw-r--r--   0 jan       (1000) users      (100)    12663 2023-05-19 05:17:03.000000 kas-3.3/kas/libcmds.py
--rw-r--r--   0 jan       (1000) users      (100)    13670 2023-06-10 06:39:22.000000 kas-3.3/kas/libkas.py
-drwxr-xr-x   0 jan       (1000) users      (100)        0 2023-06-20 19:26:55.000000 kas-3.3/kas/plugins/
--rw-r--r--   0 jan       (1000) users      (100)     2014 2023-01-05 17:10:45.000000 kas-3.3/kas/plugins/__init__.py
--rw-r--r--   0 jan       (1000) users      (100)     4276 2023-05-19 05:17:03.000000 kas-3.3/kas/plugins/build.py
--rw-r--r--   0 jan       (1000) users      (100)     2352 2021-10-19 08:31:44.000000 kas-3.3/kas/plugins/checkout.py
--rw-r--r--   0 jan       (1000) users      (100)     8728 2023-06-10 06:39:22.000000 kas-3.3/kas/plugins/dump.py
--rw-r--r--   0 jan       (1000) users      (100)     5140 2023-06-10 06:39:22.000000 kas-3.3/kas/plugins/for_all_repos.py
--rw-r--r--   0 jan       (1000) users      (100)    18530 2023-06-10 06:39:22.000000 kas-3.3/kas/plugins/menu.py
--rw-r--r--   0 jan       (1000) users      (100)     4451 2023-05-19 05:17:03.000000 kas-3.3/kas/plugins/shell.py
--rw-r--r--   0 jan       (1000) users      (100)    20545 2023-06-10 06:39:22.000000 kas-3.3/kas/repos.py
--rw-r--r--   0 jan       (1000) users      (100)     9741 2023-06-10 06:39:22.000000 kas-3.3/kas/schema-kas.json
--rwxr-xr-x   0 jan       (1000) users      (100)    16587 2023-06-20 19:26:48.000000 kas-3.3/kas-container
-drwxr-xr-x   0 jan       (1000) users      (100)        0 2023-06-20 19:26:55.000000 kas-3.3/kas.egg-info/
--rw-r--r--   0 jan       (1000) users      (100)     2878 2023-06-20 19:26:55.000000 kas-3.3/kas.egg-info/PKG-INFO
--rw-r--r--   0 jan       (1000) users      (100)      586 2023-06-20 19:26:55.000000 kas-3.3/kas.egg-info/SOURCES.txt
--rw-r--r--   0 jan       (1000) users      (100)        1 2023-06-20 19:26:55.000000 kas-3.3/kas.egg-info/dependency_links.txt
--rw-r--r--   0 jan       (1000) users      (100)       38 2023-06-20 19:26:55.000000 kas-3.3/kas.egg-info/entry_points.txt
--rw-r--r--   0 jan       (1000) users      (100)       76 2023-06-20 19:26:55.000000 kas-3.3/kas.egg-info/requires.txt
--rw-r--r--   0 jan       (1000) users      (100)        4 2023-06-20 19:26:55.000000 kas-3.3/kas.egg-info/top_level.txt
--rw-r--r--   0 jan       (1000) users      (100)       58 2021-11-29 10:53:59.000000 kas-3.3/pyproject.toml
--rw-r--r--   0 jan       (1000) users      (100)       38 2023-06-20 19:26:55.000000 kas-3.3/setup.cfg
--rw-r--r--   0 jan       (1000) users      (100)     3286 2023-05-26 16:25:25.000000 kas-3.3/setup.py
+drwxr-xr-x   0 jan       (1000) users      (100)        0 2023-07-01 11:36:50.000000 kas-4.0/
+-rw-r--r--   0 jan       (1000) users      (100)     2878 2023-07-01 11:36:50.000000 kas-4.0/PKG-INFO
+-rw-r--r--   0 jan       (1000) users      (100)     1624 2023-04-08 06:54:12.000000 kas-4.0/README.rst
+drwxr-xr-x   0 jan       (1000) users      (100)        0 2023-07-01 11:36:50.000000 kas-4.0/kas/
+-rw-r--r--   0 jan       (1000) users      (100)     1527 2020-12-06 06:22:49.000000 kas-4.0/kas/__init__.py
+-rw-r--r--   0 jan       (1000) users      (100)     1330 2021-09-13 11:52:25.000000 kas-4.0/kas/__main__.py
+-rw-r--r--   0 jan       (1000) users      (100)     1420 2023-06-26 09:56:15.000000 kas-4.0/kas/__version__.py
+-rw-r--r--   0 jan       (1000) users      (100)     7155 2023-06-10 06:39:22.000000 kas-4.0/kas/config.py
+-rw-r--r--   0 jan       (1000) users      (100)     1455 2021-10-08 09:03:16.000000 kas-4.0/kas/configschema.py
+-rw-r--r--   0 jan       (1000) users      (100)     4525 2022-10-28 05:38:25.000000 kas-4.0/kas/context.py
+-rw-r--r--   0 jan       (1000) users      (100)    12259 2023-07-01 11:36:17.000000 kas-4.0/kas/includehandler.py
+-rw-r--r--   0 jan       (1000) users      (100)     6574 2023-05-28 10:39:04.000000 kas-4.0/kas/kas.py
+-rw-r--r--   0 jan       (1000) users      (100)     2872 2023-05-19 05:17:03.000000 kas-4.0/kas/kasusererror.py
+-rw-r--r--   0 jan       (1000) users      (100)    12663 2023-05-19 05:17:03.000000 kas-4.0/kas/libcmds.py
+-rw-r--r--   0 jan       (1000) users      (100)    13670 2023-06-10 06:39:22.000000 kas-4.0/kas/libkas.py
+drwxr-xr-x   0 jan       (1000) users      (100)        0 2023-07-01 11:36:50.000000 kas-4.0/kas/plugins/
+-rw-r--r--   0 jan       (1000) users      (100)     2014 2023-01-05 17:10:45.000000 kas-4.0/kas/plugins/__init__.py
+-rw-r--r--   0 jan       (1000) users      (100)     4276 2023-05-19 05:17:03.000000 kas-4.0/kas/plugins/build.py
+-rw-r--r--   0 jan       (1000) users      (100)     2352 2021-10-19 08:31:44.000000 kas-4.0/kas/plugins/checkout.py
+-rw-r--r--   0 jan       (1000) users      (100)     8728 2023-06-10 06:39:22.000000 kas-4.0/kas/plugins/dump.py
+-rw-r--r--   0 jan       (1000) users      (100)     5140 2023-06-10 06:39:22.000000 kas-4.0/kas/plugins/for_all_repos.py
+-rw-r--r--   0 jan       (1000) users      (100)    18530 2023-06-10 06:39:22.000000 kas-4.0/kas/plugins/menu.py
+-rw-r--r--   0 jan       (1000) users      (100)     4451 2023-05-19 05:17:03.000000 kas-4.0/kas/plugins/shell.py
+-rw-r--r--   0 jan       (1000) users      (100)    20545 2023-06-10 06:39:22.000000 kas-4.0/kas/repos.py
+-rw-r--r--   0 jan       (1000) users      (100)     9741 2023-06-10 06:39:22.000000 kas-4.0/kas/schema-kas.json
+-rwxr-xr-x   0 jan       (1000) users      (100)    16587 2023-06-26 09:56:15.000000 kas-4.0/kas-container
+drwxr-xr-x   0 jan       (1000) users      (100)        0 2023-07-01 11:36:50.000000 kas-4.0/kas.egg-info/
+-rw-r--r--   0 jan       (1000) users      (100)     2878 2023-07-01 11:36:49.000000 kas-4.0/kas.egg-info/PKG-INFO
+-rw-r--r--   0 jan       (1000) users      (100)      586 2023-07-01 11:36:49.000000 kas-4.0/kas.egg-info/SOURCES.txt
+-rw-r--r--   0 jan       (1000) users      (100)        1 2023-07-01 11:36:49.000000 kas-4.0/kas.egg-info/dependency_links.txt
+-rw-r--r--   0 jan       (1000) users      (100)       38 2023-07-01 11:36:49.000000 kas-4.0/kas.egg-info/entry_points.txt
+-rw-r--r--   0 jan       (1000) users      (100)       76 2023-07-01 11:36:49.000000 kas-4.0/kas.egg-info/requires.txt
+-rw-r--r--   0 jan       (1000) users      (100)        4 2023-07-01 11:36:49.000000 kas-4.0/kas.egg-info/top_level.txt
+-rw-r--r--   0 jan       (1000) users      (100)       58 2021-11-29 10:53:59.000000 kas-4.0/pyproject.toml
+-rw-r--r--   0 jan       (1000) users      (100)       38 2023-07-01 11:36:50.000000 kas-4.0/setup.cfg
+-rw-r--r--   0 jan       (1000) users      (100)     3286 2023-05-26 16:25:25.000000 kas-4.0/setup.py
```

### Comparing `kas-3.3/PKG-INFO` & `kas-4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.2
 Name: kas
-Version: 3.3
+Version: 4.0
 Summary: Setup tool for bitbake based projects
 Home-page: https://github.com/siemens/kas
 Maintainer: Jan Kiszka
 Maintainer-email: jan.kiszka@siemens.com
 License: MIT
-Download-URL: https://github.com/siemens/kas/archive/3.3.tar.gz
+Download-URL: https://github.com/siemens/kas/archive/4.0.tar.gz
 Description: Setup tool for bitbake based projects
         =====================================
         
         +--------------------+
         |    Build Status    |
         +====================+
         | |workflow-master|_ |
```

### Comparing `kas-3.3/README.rst` & `kas-4.0/README.rst`

 * *Files identical despite different names*

### Comparing `kas-3.3/kas/__init__.py` & `kas-4.0/kas/__init__.py`

 * *Files identical despite different names*

### Comparing `kas-3.3/kas/__main__.py` & `kas-4.0/kas/__main__.py`

 * *Files identical despite different names*

### Comparing `kas-3.3/kas/__version__.py` & `kas-4.0/kas/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,12 +21,12 @@
 # SOFTWARE.
 """
     This module contains the version of kas.
 """
 __license__ = 'MIT'
 __copyright__ = 'Copyright (c) Siemens AG, 2017-2020'
 
-__version__ = '3.3'
+__version__ = '4.0'
 
 # Please update docs/format-changelog.rst when changing the file version.
 __file_version__ = 14
 __compatible_file_version__ = 1
```

### Comparing `kas-3.3/kas/config.py` & `kas-4.0/kas/config.py`

 * *Files identical despite different names*

### Comparing `kas-3.3/kas/configschema.py` & `kas-4.0/kas/configschema.py`

 * *Files identical despite different names*

### Comparing `kas-3.3/kas/context.py` & `kas-4.0/kas/context.py`

 * *Files identical despite different names*

### Comparing `kas-3.3/kas/includehandler.py` & `kas-4.0/kas/includehandler.py`

 * *Files identical despite different names*

### Comparing `kas-3.3/kas/kas.py` & `kas-4.0/kas/kas.py`

 * *Files identical despite different names*

### Comparing `kas-3.3/kas/kasusererror.py` & `kas-4.0/kas/kasusererror.py`

 * *Files identical despite different names*

### Comparing `kas-3.3/kas/libcmds.py` & `kas-4.0/kas/libcmds.py`

 * *Files identical despite different names*

### Comparing `kas-3.3/kas/libkas.py` & `kas-4.0/kas/libkas.py`

 * *Files identical despite different names*

### Comparing `kas-3.3/kas/plugins/__init__.py` & `kas-4.0/kas/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `kas-3.3/kas/plugins/build.py` & `kas-4.0/kas/plugins/build.py`

 * *Files identical despite different names*

### Comparing `kas-3.3/kas/plugins/checkout.py` & `kas-4.0/kas/plugins/checkout.py`

 * *Files identical despite different names*

### Comparing `kas-3.3/kas/plugins/dump.py` & `kas-4.0/kas/plugins/dump.py`

 * *Files identical despite different names*

### Comparing `kas-3.3/kas/plugins/for_all_repos.py` & `kas-4.0/kas/plugins/for_all_repos.py`

 * *Files identical despite different names*

### Comparing `kas-3.3/kas/plugins/menu.py` & `kas-4.0/kas/plugins/menu.py`

 * *Files identical despite different names*

### Comparing `kas-3.3/kas/plugins/shell.py` & `kas-4.0/kas/plugins/shell.py`

 * *Files identical despite different names*

### Comparing `kas-3.3/kas/repos.py` & `kas-4.0/kas/repos.py`

 * *Files identical despite different names*

### Comparing `kas-3.3/kas/schema-kas.json` & `kas-4.0/kas/schema-kas.json`

 * *Files identical despite different names*

### Comparing `kas-3.3/kas-container` & `kas-4.0/kas-container`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 		if [ "$1" = "cleanall" ]; then
 			DL_DIR=${DL_DIR:-${KAS_BUILD_DIR}/downloads}
 			trace rm -rf "${DL_DIR}"
 		fi
 	fi
 }
 
-KAS_IMAGE_VERSION_DEFAULT="3.3"
+KAS_IMAGE_VERSION_DEFAULT="4.0"
 KAS_CONTAINER_IMAGE_PATH_DEFAULT="ghcr.io/siemens/kas"
 KAS_CONTAINER_IMAGE_NAME_DEFAULT="kas"
 
 set_container_image_var() {
 	KAS_IMAGE_VERSION="${KAS_IMAGE_VERSION:-${KAS_IMAGE_VERSION_DEFAULT}}"
 	KAS_CONTAINER_IMAGE_NAME="${KAS_CONTAINER_IMAGE_NAME:-${KAS_CONTAINER_IMAGE_NAME_DEFAULT}}"
 	KAS_CONTAINER_IMAGE_PATH="${KAS_CONTAINER_IMAGE_PATH:-${KAS_CONTAINER_IMAGE_PATH_DEFAULT}}"
```

### Comparing `kas-3.3/kas.egg-info/PKG-INFO` & `kas-4.0/kas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.2
 Name: kas
-Version: 3.3
+Version: 4.0
 Summary: Setup tool for bitbake based projects
 Home-page: https://github.com/siemens/kas
 Maintainer: Jan Kiszka
 Maintainer-email: jan.kiszka@siemens.com
 License: MIT
-Download-URL: https://github.com/siemens/kas/archive/3.3.tar.gz
+Download-URL: https://github.com/siemens/kas/archive/4.0.tar.gz
 Description: Setup tool for bitbake based projects
         =====================================
         
         +--------------------+
         |    Build Status    |
         +====================+
         | |workflow-master|_ |
```

### Comparing `kas-3.3/kas.egg-info/SOURCES.txt` & `kas-4.0/kas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kas-3.3/setup.py` & `kas-4.0/setup.py`

 * *Files identical despite different names*

