# Comparing `tmp/igorwriter-0.3.0.tar.gz` & `tmp/igorwriter-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/igorwriter-0.3.0.tar", last modified: Sat Nov 16 05:33:38 2019, max compression
+gzip compressed data, was "igorwriter-0.4.0.tar", last modified: Sat Jul  1 17:44:56 2023, max compression
```

## Comparing `igorwriter-0.3.0.tar` & `igorwriter-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,27 @@
-drwxr-xr-x   0 tomoya    (1000) tomoya    (1000)        0 2019-11-16 05:33:38.001721 igorwriter-0.3.0/
--rw-r--r--   0 tomoya    (1000) tomoya    (1000)     4580 2019-11-16 05:33:38.001721 igorwriter-0.3.0/PKG-INFO
--rw-r--r--   0 tomoya    (1000) tomoya    (1000)     3121 2019-11-16 05:32:31.000000 igorwriter-0.3.0/README.rst
-drwxr-xr-x   0 tomoya    (1000) tomoya    (1000)        0 2019-11-16 05:33:38.001721 igorwriter-0.3.0/igorwriter/
--rw-r--r--   0 tomoya    (1000) tomoya    (1000)    12958 2019-11-16 05:32:31.000000 igorwriter-0.3.0/igorwriter/__init__.py
--rw-r--r--   0 tomoya    (1000) tomoya    (1000)      433 2019-11-16 04:29:14.000000 igorwriter-0.3.0/igorwriter/builtin_names.py
-drwxr-xr-x   0 tomoya    (1000) tomoya    (1000)        0 2019-11-16 05:33:38.001721 igorwriter-0.3.0/igorwriter/builtins/
--rw-r--r--   0 tomoya    (1000) tomoya    (1000)     5805 2019-11-16 04:29:14.000000 igorwriter-0.3.0/igorwriter/builtins/functions.txt
--rw-r--r--   0 tomoya    (1000) tomoya    (1000)      104 2019-11-16 04:29:14.000000 igorwriter-0.3.0/igorwriter/builtins/keywords.txt
--rw-r--r--   0 tomoya    (1000) tomoya    (1000)     6175 2019-11-16 04:29:14.000000 igorwriter-0.3.0/igorwriter/builtins/operations.txt
--rw-r--r--   0 tomoya    (1000) tomoya    (1000)     1511 2019-11-16 05:32:31.000000 igorwriter-0.3.0/igorwriter/utils.py
--rw-r--r--   0 tomoya    (1000) tomoya    (1000)     2760 2019-11-16 04:29:14.000000 igorwriter-0.3.0/igorwriter/validator.py
-drwxr-xr-x   0 tomoya    (1000) tomoya    (1000)        0 2019-11-16 05:33:38.001721 igorwriter-0.3.0/igorwriter.egg-info/
--rw-r--r--   0 tomoya    (1000) tomoya    (1000)     4580 2019-11-16 05:33:37.000000 igorwriter-0.3.0/igorwriter.egg-info/PKG-INFO
--rw-r--r--   0 tomoya    (1000) tomoya    (1000)      395 2019-11-16 05:33:37.000000 igorwriter-0.3.0/igorwriter.egg-info/SOURCES.txt
--rw-r--r--   0 tomoya    (1000) tomoya    (1000)        1 2019-11-16 05:33:37.000000 igorwriter-0.3.0/igorwriter.egg-info/dependency_links.txt
--rw-r--r--   0 tomoya    (1000) tomoya    (1000)        6 2019-11-16 05:33:37.000000 igorwriter-0.3.0/igorwriter.egg-info/requires.txt
--rw-r--r--   0 tomoya    (1000) tomoya    (1000)       11 2019-11-16 05:33:37.000000 igorwriter-0.3.0/igorwriter.egg-info/top_level.txt
--rw-r--r--   0 tomoya    (1000) tomoya    (1000)       67 2019-11-16 05:33:38.001721 igorwriter-0.3.0/setup.cfg
--rw-r--r--   0 tomoya    (1000) tomoya    (1000)     1577 2019-11-16 05:32:31.000000 igorwriter-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 17:44:56.121068 igorwriter-0.4.0/
+-rw-rw-rw-   0        0        0     1062 2019-11-16 04:29:14.000000 igorwriter-0.4.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     3594 2023-07-01 17:44:56.121068 igorwriter-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3121 2019-11-16 05:32:31.000000 igorwriter-0.4.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-01 17:44:56.096041 igorwriter-0.4.0/igorwriter/
+-rw-rw-rw-   0        0        0       53 2023-07-01 17:36:50.000000 igorwriter-0.4.0/igorwriter/__init__.py
+-rw-rw-rw-   0        0        0      433 2019-11-16 04:29:14.000000 igorwriter-0.4.0/igorwriter/builtin_names.py
+drwxrwxrwx   0        0        0        0 2023-07-01 17:44:56.106042 igorwriter-0.4.0/igorwriter/builtins/
+-rw-rw-rw-   0        0        0     5805 2019-11-16 04:29:14.000000 igorwriter-0.4.0/igorwriter/builtins/functions.txt
+-rw-rw-rw-   0        0        0      104 2019-11-16 04:29:14.000000 igorwriter-0.4.0/igorwriter/builtins/keywords.txt
+-rw-rw-rw-   0        0        0     6175 2019-11-16 04:29:14.000000 igorwriter-0.4.0/igorwriter/builtins/operations.txt
+-rw-rw-rw-   0        0        0      213 2023-07-01 17:22:58.000000 igorwriter-0.4.0/igorwriter/errors.py
+-rw-rw-rw-   0        0        0    18287 2023-07-01 17:36:50.000000 igorwriter-0.4.0/igorwriter/igorwave.py
+-rw-rw-rw-   0        0        0     1511 2019-11-16 05:32:31.000000 igorwriter-0.4.0/igorwriter/utils.py
+-rw-rw-rw-   0        0        0     2807 2023-07-01 17:22:58.000000 igorwriter-0.4.0/igorwriter/validator.py
+drwxrwxrwx   0        0        0        0 2023-07-01 17:44:56.104042 igorwriter-0.4.0/igorwriter.egg-info/
+-rw-rw-rw-   0        0        0     3594 2023-07-01 17:44:56.000000 igorwriter-0.4.0/igorwriter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-07-01 17:44:56.000000 igorwriter-0.4.0/igorwriter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 17:44:56.000000 igorwriter-0.4.0/igorwriter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-01 17:44:56.000000 igorwriter-0.4.0/igorwriter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-01 17:44:56.000000 igorwriter-0.4.0/igorwriter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2023-07-01 17:44:56.125067 igorwriter-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1278 2023-07-01 17:38:27.000000 igorwriter-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 17:44:56.120068 igorwriter-0.4.0/tests/
+-rw-rw-rw-   0        0        0     4191 2023-07-01 17:22:58.000000 igorwriter-0.4.0/tests/test_names.py
+-rw-rw-rw-   0        0        0     1256 2019-11-16 04:29:14.000000 igorwriter-0.4.0/tests/test_utils.py
+-rw-rw-rw-   0        0        0    12984 2023-07-01 17:36:50.000000 igorwriter-0.4.0/tests/test_wave.py
```

### Comparing `igorwriter-0.3.0/README.rst` & `igorwriter-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `igorwriter-0.3.0/igorwriter/builtins/functions.txt` & `igorwriter-0.4.0/igorwriter/builtins/functions.txt`

 * *Files identical despite different names*

### Comparing `igorwriter-0.3.0/igorwriter/builtins/operations.txt` & `igorwriter-0.4.0/igorwriter/builtins/operations.txt`

 * *Files identical despite different names*

### Comparing `igorwriter-0.3.0/igorwriter/utils.py` & `igorwriter-0.4.0/igorwriter/utils.py`

 * *Files identical despite different names*

### Comparing `igorwriter-0.3.0/setup.py` & `igorwriter-0.4.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,42 @@
-# -*- coding: utf-8 -*-
-# Always prefer setuptools over distutils
-from setuptools import setup, find_packages
-# To use a consistent encoding
-from codecs import open
-from os import path
-
-here = path.abspath(path.dirname(__file__))
-
-# Get the long description from the README file
-with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
-    long_description = f.read()
-
-setup(
-    name='igorwriter',
-    version='0.3.0',
-    description='Write IGOR binary (.ibw) or text (.itx) files from numpy array',
-    long_description=long_description,
-    url='https://github.com/t-onoz/igorwriter',
-    author='t-onoz',
-    license='MIT',
-    classifiers=[
-        # How mature is this project? Common values are
-        #   3 - Alpha
-        #   4 - Beta
-        #   5 - Production/Stable
-        'Development Status :: 3 - Alpha',
-
-        'License :: OSI Approved :: MIT License',
-
-        # Specify the Python versions you support here. In particular, ensure
-        # that you indicate whether you support Python 2, Python 3 or both.
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-    ],
-
-    packages=find_packages(),
-    package_data={
-        'igorwriter': ['builtins/*.txt']
-    },
-
-    install_requires=['numpy'],  # Optional
-)
+# -*- coding: utf-8 -*-
+# Always prefer setuptools over distutils
+from setuptools import setup, find_packages
+# To use a consistent encoding
+from codecs import open
+from os import path
+
+here = path.abspath(path.dirname(__file__))
+
+# Get the long description from the README file
+with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
+    long_description = f.read()
+
+setup(
+    name='igorwriter',
+    version='0.4.0',
+    description='Write IGOR binary (.ibw) or text (.itx) files from numpy array',
+    long_description=long_description,
+    url='https://github.com/t-onoz/igorwriter',
+    author='t-onoz',
+    license='MIT',
+    classifiers=[
+        # How mature is this project? Common values are
+        #   3 - Alpha
+        #   4 - Beta
+        #   5 - Production/Stable
+        'Development Status :: 3 - Alpha',
+
+        'License :: OSI Approved :: MIT License',
+
+        # Specify the Python versions you support here. In particular, ensure
+        # that you indicate whether you support Python 2, Python 3 or both.
+        'Programming Language :: Python :: 3',
+    ],
+
+    packages=find_packages(),
+    package_data={
+        'igorwriter': ['builtins/*.txt']
+    },
+
+    install_requires=['numpy'],  # Optional
+)
```

