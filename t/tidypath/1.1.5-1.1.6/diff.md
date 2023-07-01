# Comparing `tmp/tidypath-1.1.5.tar.gz` & `tmp/tidypath-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidypath-1.1.5.tar", last modified: Fri Jun 30 17:42:16 2023, max compression
+gzip compressed data, was "tidypath-1.1.6.tar", last modified: Sat Jul  1 08:02:22 2023, max compression
```

## Comparing `tidypath-1.1.5.tar` & `tidypath-1.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-06-30 17:42:16.603755 tidypath-1.1.5/
--rwxr-xr-x   0 userx     (1000) wheel      (998)    35149 2023-06-08 21:46:44.000000 tidypath-1.1.5/LICENSE.md
--rw-r--r--   0 userx     (1000) wheel      (998)     3682 2023-06-30 17:42:16.603755 tidypath-1.1.5/PKG-INFO
--rwxr-xr-x   0 userx     (1000) wheel      (998)     2804 2023-06-08 21:46:44.000000 tidypath-1.1.5/README.md
--rwxr-xr-x   0 userx     (1000) wheel      (998)      106 2023-06-30 17:42:16.603755 tidypath-1.1.5/setup.cfg
--rwxr-xr-x   0 userx     (1000) wheel      (998)     1161 2023-06-30 17:41:03.000000 tidypath-1.1.5/setup.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-06-30 17:42:16.600421 tidypath-1.1.5/tidypath/
--rwxr-xr-x   0 userx     (1000) wheel      (998)      302 2023-06-08 21:46:44.000000 tidypath-1.1.5/tidypath/__init__.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     1629 2023-06-08 21:46:44.000000 tidypath-1.1.5/tidypath/_helper.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     5054 2023-06-08 21:46:44.000000 tidypath-1.1.5/tidypath/config.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)    11943 2023-06-30 17:38:34.000000 tidypath-1.1.5/tidypath/decorators.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     6130 2023-06-30 17:36:32.000000 tidypath-1.1.5/tidypath/fmt.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     5197 2023-06-08 21:46:44.000000 tidypath-1.1.5/tidypath/inspection.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)    13171 2023-06-30 17:40:49.000000 tidypath-1.1.5/tidypath/paths.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     9844 2023-06-08 21:46:44.000000 tidypath-1.1.5/tidypath/storage.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-06-30 17:42:16.603755 tidypath-1.1.5/tidypath.egg-info/
--rwxr-xr-x   0 userx     (1000) wheel      (998)     3682 2023-06-30 17:42:16.000000 tidypath-1.1.5/tidypath.egg-info/PKG-INFO
--rwxr-xr-x   0 userx     (1000) wheel      (998)      358 2023-06-30 17:42:16.000000 tidypath-1.1.5/tidypath.egg-info/SOURCES.txt
--rwxr-xr-x   0 userx     (1000) wheel      (998)        1 2023-06-30 17:42:16.000000 tidypath-1.1.5/tidypath.egg-info/dependency_links.txt
--rwxr-xr-x   0 userx     (1000) wheel      (998)       63 2023-06-30 17:42:16.000000 tidypath-1.1.5/tidypath.egg-info/requires.txt
--rwxr-xr-x   0 userx     (1000) wheel      (998)        9 2023-06-30 17:42:16.000000 tidypath-1.1.5/tidypath.egg-info/top_level.txt
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-07-01 08:02:22.864847 tidypath-1.1.6/
+-rwxr-xr-x   0 userx     (1000) wheel      (998)    35149 2023-06-08 21:46:44.000000 tidypath-1.1.6/LICENSE.md
+-rw-r--r--   0 userx     (1000) wheel      (998)     3682 2023-07-01 08:02:22.864847 tidypath-1.1.6/PKG-INFO
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     2804 2023-06-08 21:46:44.000000 tidypath-1.1.6/README.md
+-rwxr-xr-x   0 userx     (1000) wheel      (998)      106 2023-07-01 08:02:22.864847 tidypath-1.1.6/setup.cfg
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     1161 2023-07-01 08:02:13.000000 tidypath-1.1.6/setup.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-07-01 08:02:22.861513 tidypath-1.1.6/tidypath/
+-rwxr-xr-x   0 userx     (1000) wheel      (998)      302 2023-06-08 21:46:44.000000 tidypath-1.1.6/tidypath/__init__.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     1629 2023-06-08 21:46:44.000000 tidypath-1.1.6/tidypath/_helper.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     5054 2023-06-08 21:46:44.000000 tidypath-1.1.6/tidypath/config.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)    11948 2023-07-01 08:01:59.000000 tidypath-1.1.6/tidypath/decorators.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     6165 2023-07-01 08:01:27.000000 tidypath-1.1.6/tidypath/fmt.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     5197 2023-06-08 21:46:44.000000 tidypath-1.1.6/tidypath/inspection.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)    13171 2023-06-30 17:40:49.000000 tidypath-1.1.6/tidypath/paths.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     9844 2023-06-08 21:46:44.000000 tidypath-1.1.6/tidypath/storage.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-07-01 08:02:22.864847 tidypath-1.1.6/tidypath.egg-info/
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     3682 2023-07-01 08:02:22.000000 tidypath-1.1.6/tidypath.egg-info/PKG-INFO
+-rwxr-xr-x   0 userx     (1000) wheel      (998)      358 2023-07-01 08:02:22.000000 tidypath-1.1.6/tidypath.egg-info/SOURCES.txt
+-rwxr-xr-x   0 userx     (1000) wheel      (998)        1 2023-07-01 08:02:22.000000 tidypath-1.1.6/tidypath.egg-info/dependency_links.txt
+-rwxr-xr-x   0 userx     (1000) wheel      (998)       63 2023-07-01 08:02:22.000000 tidypath-1.1.6/tidypath.egg-info/requires.txt
+-rwxr-xr-x   0 userx     (1000) wheel      (998)        9 2023-07-01 08:02:22.000000 tidypath-1.1.6/tidypath.egg-info/top_level.txt
```

### Comparing `tidypath-1.1.5/LICENSE.md` & `tidypath-1.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.5/PKG-INFO` & `tidypath-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidypath
-Version: 1.1.5
+Version: 1.1.6
 Summary: Automatically store/load data in a tidy, efficient way.
 Home-page: https://github.com/medinajorge/tidypath
 Download-URL: https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tidypath-1.1.5/README.md` & `tidypath-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.5/setup.py` & `tidypath-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tidypath',
-    version='1.1.5',
+    version='1.1.6',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=['tidypath'],
     url='https://github.com/medinajorge/tidypath',
     download_url='https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz',
     description="Automatically store/load data in a tidy, efficient way.",
     long_description=open('README.md').read(),
```

### Comparing `tidypath-1.1.5/tidypath/_helper.py` & `tidypath-1.1.6/tidypath/_helper.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.5/tidypath/config.py` & `tidypath-1.1.6/tidypath/config.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.5/tidypath/decorators.py` & `tidypath-1.1.6/tidypath/decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from ._helper import merge_nested_dict
 
 
 def savedata(keys_or_function=None, include_classes="file",
              ext=config.EXT_DEFAULT_DATA, keys=config.KEYS_DEFAULT_DATA, funcname_in_filename=config.FUNCNAME_IN_FILENAME_DEFAULT_DATA,
              overwrite=False, save=True, load_opts_default_save=True,  #defaults for extra arguments
              max_str_length=255,
-             iterable_maxsize=3,
+             iterable_maxsize=np.inf,
              load_opts={}, **save_opts):
     """
     Decorator for automatically saving output and then loading cached data.
     Default behavior:
         1st function call:   stores the data with extension 'ext'.
         rest:                loads stored data if the key args passed to the function coincide.
```

### Comparing `tidypath-1.1.5/tidypath/fmt.py` & `tidypath-1.1.6/tidypath/fmt.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         return str(x)
     elif callable(x):
         return x.__name__
     elif isinstance(x, dict):
         if len(x) >= iterable_maxsize:
             return "{}-values".format(str(len(x)))
         else:
-            return dict_to_id(x, ndigits=ndigits, join_char="-")
+            return dict_to_id(x, ndigits=ndigits, join_char="-", iterable_maxsize=iterable_maxsize)
     elif isinstance(x, iterables):
         if len(x) >= iterable_maxsize:
             return "{}-values".format(str(len(x)))
         else:
             return '-'.join([encoder(sub_x) for sub_x in x])
     else:
         return str(x)
```

### Comparing `tidypath-1.1.5/tidypath/inspection.py` & `tidypath-1.1.6/tidypath/inspection.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.5/tidypath/paths.py` & `tidypath-1.1.6/tidypath/paths.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.5/tidypath/storage.py` & `tidypath-1.1.6/tidypath/storage.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.5/tidypath.egg-info/PKG-INFO` & `tidypath-1.1.6/tidypath.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidypath
-Version: 1.1.5
+Version: 1.1.6
 Summary: Automatically store/load data in a tidy, efficient way.
 Home-page: https://github.com/medinajorge/tidypath
 Download-URL: https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

