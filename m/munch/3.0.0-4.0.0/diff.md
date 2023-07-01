# Comparing `tmp/munch-3.0.0.tar.gz` & `tmp/munch-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "munch-3.0.0.tar", last modified: Sun May 14 12:28:55 2023, max compression
+gzip compressed data, was "munch-4.0.0.tar", last modified: Sat Jul  1 09:49:23 2023, max compression
```

## Comparing `munch-3.0.0.tar` & `munch-4.0.0.tar`

### file list

```diff
@@ -1,38 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:28:55.100046 munch-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-14 12:28:32.000000 munch-3.0.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:28:55.096045 munch-3.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:28:55.096045 munch-3.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-14 12:28:32.000000 munch-3.0.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-14 12:28:32.000000 munch-3.0.0/.github/workflows/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-14 12:28:32.000000 munch-3.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-14 12:28:32.000000 munch-3.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-14 12:28:32.000000 munch-3.0.0/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 12:28:55.000000 munch-3.0.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-05-14 12:28:32.000000 munch-3.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-14 12:28:55.000000 munch-3.0.0/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-14 12:28:32.000000 munch-3.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 12:28:32.000000 munch-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-14 12:28:32.000000 munch-3.0.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-05-14 12:28:55.100046 munch-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-14 12:28:32.000000 munch-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:28:55.096045 munch-3.0.0/munch/
--rw-r--r--   0 runner    (1001) docker     (123)    22544 2023-05-14 12:28:32.000000 munch-3.0.0/munch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-14 12:28:32.000000 munch-3.0.0/munch/python3_compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:28:55.100046 munch-3.0.0/munch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-05-14 12:28:55.000000 munch-3.0.0/munch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-14 12:28:55.000000 munch-3.0.0/munch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 12:28:55.000000 munch-3.0.0/munch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 12:28:55.000000 munch-3.0.0/munch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-14 12:28:55.000000 munch-3.0.0/munch.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-14 12:28:55.000000 munch-3.0.0/munch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 12:28:55.000000 munch-3.0.0/munch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-14 12:28:32.000000 munch-3.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-14 12:28:55.100046 munch-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-14 12:28:32.000000 munch-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:28:55.100046 munch-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:28:32.000000 munch-3.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-14 12:28:32.000000 munch-3.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    16017 2023-05-14 12:28:32.000000 munch-3.0.0/tests/test_munch.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-14 12:28:32.000000 munch-3.0.0/tests/test_readme.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-14 12:28:32.000000 munch-3.0.0/tests/test_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-14 12:28:32.000000 munch-3.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:49:23.618900 munch-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-01 09:49:11.000000 munch-4.0.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:49:23.614900 munch-4.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:49:23.614900 munch-4.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-01 09:49:11.000000 munch-4.0.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-01 09:49:11.000000 munch-4.0.0/.github/workflows/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-01 09:49:11.000000 munch-4.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-01 09:49:11.000000 munch-4.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-01 09:49:11.000000 munch-4.0.0/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 09:49:23.000000 munch-4.0.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-01 09:49:11.000000 munch-4.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-01 09:49:23.000000 munch-4.0.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-01 09:49:11.000000 munch-4.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 09:49:11.000000 munch-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-01 09:49:11.000000 munch-4.0.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-07-01 09:49:23.618900 munch-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-07-01 09:49:11.000000 munch-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:49:23.614900 munch-4.0.0/munch/
+-rw-r--r--   0 runner    (1001) docker     (123)    22499 2023-07-01 09:49:11.000000 munch-4.0.0/munch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:49:23.618900 munch-4.0.0/munch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-07-01 09:49:23.000000 munch-4.0.0/munch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-01 09:49:23.000000 munch-4.0.0/munch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 09:49:23.000000 munch-4.0.0/munch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 09:49:23.000000 munch-4.0.0/munch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-01 09:49:23.000000 munch-4.0.0/munch.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-01 09:49:23.000000 munch-4.0.0/munch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-01 09:49:23.000000 munch-4.0.0/munch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-01 09:49:11.000000 munch-4.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-01 09:49:23.618900 munch-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-01 09:49:11.000000 munch-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:49:23.618900 munch-4.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 09:49:11.000000 munch-4.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-01 09:49:11.000000 munch-4.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16017 2023-07-01 09:49:11.000000 munch-4.0.0/tests/test_munch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-01 09:49:11.000000 munch-4.0.0/tests/test_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-01 09:49:11.000000 munch-4.0.0/tests/test_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-01 09:49:11.000000 munch-4.0.0/tox.ini
```

### Comparing `munch-3.0.0/.github/workflows/ci.yml` & `munch-4.0.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `munch-3.0.0/.github/workflows/python-publish.yml` & `munch-4.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `munch-3.0.0/.travis.yml` & `munch-4.0.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `munch-3.0.0/CHANGELOG.md` & `munch-4.0.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 Changelog
 =========
 
 Next Version
 ------------
 
+4.0.0 (2023-07-01)
+------------------
+
+* Remove six dependency
+
 3.0.0 (2023-05-14)
 ------------------
 
 * Fix munchify for tuples of lists  
 * Require Python >=3.6 and upgrade syntax - thanks @EwoutH
 * Update __init__.py  to work with non standard version - thanks @mboisson
 * Allow importing even when VERSION read fails - thanks @mdornseif and @dangillet
```

### Comparing `munch-3.0.0/LICENSE.txt` & `munch-4.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `munch-3.0.0/PKG-INFO` & `munch-4.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: munch
-Version: 3.0.0
+Version: 4.0.0
 Summary: A dot-accessible dictionary (a la JavaScript objects)
 Home-page: https://github.com/Infinidat/munch
 Author: Rotem Yaari
 Author-email: vmalloc@gmail.com
 License: MIT
 Keywords: munch,dict,mapping,container,collection
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,22 +23,31 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 Provides-Extra: yaml
 License-File: LICENSE.txt
 
-[![Build Status](https://travis-ci.org/Infinidat/munch.svg?branch=master)](https://travis-ci.org/Infinidat/munch)
 [![Latest Version](https://img.shields.io/pypi/v/munch.svg)](https://pypi.python.org/pypi/munch/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/munch.svg)](https://pypi.python.org/pypi/munch/)
 [![Downloads](https://img.shields.io/pypi/dm/munch.svg)](https://pypi.python.org/pypi/munch/)
 
 munch
 ==========
 
+Installation
+-------------
+
+```
+pip install munch
+```
+
+Usage
+-----
+
 munch is a fork of David Schoonover's **Bunch** package, providing similar functionality. 99% of the work was done by him, and the fork was made mainly for lack of responsiveness for fixes and maintenance on the original code.
 
 Munch is a dictionary that supports attribute-style access, a la JavaScript:
 
 ```python
 
 >>> from munch import Munch
```

### Comparing `munch-3.0.0/README.md` & `munch-4.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,24 @@
-[![Build Status](https://travis-ci.org/Infinidat/munch.svg?branch=master)](https://travis-ci.org/Infinidat/munch)
 [![Latest Version](https://img.shields.io/pypi/v/munch.svg)](https://pypi.python.org/pypi/munch/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/munch.svg)](https://pypi.python.org/pypi/munch/)
 [![Downloads](https://img.shields.io/pypi/dm/munch.svg)](https://pypi.python.org/pypi/munch/)
 
 munch
 ==========
 
+Installation
+-------------
+
+```
+pip install munch
+```
+
+Usage
+-----
+
 munch is a fork of David Schoonover's **Bunch** package, providing similar functionality. 99% of the work was done by him, and the fork was made mainly for lack of responsiveness for fixes and maintenance on the original code.
 
 Munch is a dictionary that supports attribute-style access, a la JavaScript:
 
 ```python
 
 >>> from munch import Munch
```

### Comparing `munch-3.0.0/munch/__init__.py` & `munch-4.0.0/munch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
         __all__ = ('Munch', 'munchify','unmunchify')
 
     un/munchify provide dictionary conversion; Munches can also be
     converted via Munch.to/fromDict().
 """
 
-from .python3_compat import iterkeys, iteritems, Mapping, u
+from collections.abc import Mapping
 
 try:
     # For python 3.8 and later
     import importlib.metadata as importlib_metadata
 except ImportError:
     # For everyone else
     import importlib_metadata
@@ -201,15 +201,15 @@
             Munch({'a b': 9, 1: 2, 'c': Munch({'simple': 5})})
 
             (*) Invertible so long as collection contents are each repr-invertible.
         """
         return f'{self.__class__.__name__}({dict.__repr__(self)})'
 
     def __dir__(self):
-        return list(iterkeys(self))
+        return list(self.keys())
 
     def __getstate__(self):
         """ Implement a serializable interface used for pickling.
 
         See https://docs.python.org/3.6/library/pickle.html.
         """
         return {k: v for k, v in self.items()}
@@ -240,15 +240,15 @@
         return type(self).fromDict(self)
 
     def update(self, *args, **kwargs):
         """
         Override built-in method to call custom __setitem__ method that may
         be defined in subclasses.
         """
-        for k, v in iteritems(dict(*args, **kwargs)):
+        for k, v in dict(*args, **kwargs).items():
             self[k] = v
 
     def get(self, k, d=None):
         """
         D.get(k[,d]) -> D[k] if k in D, else d.  d defaults to None.
         """
         if k not in self:
@@ -471,15 +471,15 @@
         else:
             return obj
 
     def post_munchify(partial, obj):
         # Here we finish munchifying the parts of obj that were deferred by pre_munchify because they
         # might be involved in a cycle
         if isinstance(obj, Mapping):
-            partial.update((k, munchify_cycles(obj[k])) for k in iterkeys(obj))
+            partial.update((k, munchify_cycles(obj[k])) for k in obj.keys())
         elif isinstance(obj, list):
             partial.extend(munchify_cycles(item) for item in obj)
         elif isinstance(obj, tuple):
             for (item_partial, item) in zip(partial, obj):
                 post_munchify(item_partial, item)
 
         return partial
@@ -533,15 +533,15 @@
         else:
             return obj
 
     def post_unmunchify(partial, obj):
         # Here we finish unmunchifying the parts of obj that were deferred by pre_unmunchify because they
         # might be involved in a cycle
         if isinstance(obj, Mapping):
-            partial.update((k, unmunchify_cycles(obj[k])) for k in iterkeys(obj))
+            partial.update((k, unmunchify_cycles(obj[k])) for k in obj.keys())
         elif isinstance(obj, list):
             partial.extend(unmunchify_cycles(v) for v in obj)
         elif isinstance(obj, tuple):
             for (value_partial, value) in zip(partial, obj):
                 post_unmunchify(value_partial, value)
 
         return partial
@@ -622,23 +622,23 @@
         """ Converts Munch to a representation node.
 
             >>> b = Munch(foo=['bar', Munch(lol=True)], hello=42)
             >>> import yaml
             >>> yaml.dump(b, default_flow_style=True)
             '!munch.Munch {foo: [bar, !munch.Munch {lol: true}], hello: 42}\\n'
         """
-        return dumper.represent_mapping(u('!munch.Munch'), data)
+        return dumper.represent_mapping('!munch.Munch', data)
 
     for loader_name in ("BaseLoader", "FullLoader", "SafeLoader", "Loader", "UnsafeLoader", "DangerLoader"):
         LoaderCls = getattr(yaml, loader_name, None)
         if LoaderCls is None:
             # This code supports both PyYAML 4.x and 5.x versions
             continue
-        yaml.add_constructor(u('!munch'), from_yaml, Loader=LoaderCls)
-        yaml.add_constructor(u('!munch.Munch'), from_yaml, Loader=LoaderCls)
+        yaml.add_constructor('!munch', from_yaml, Loader=LoaderCls)
+        yaml.add_constructor('!munch.Munch', from_yaml, Loader=LoaderCls)
 
     SafeRepresenter.add_representer(Munch, to_yaml_safe)
     SafeRepresenter.add_multi_representer(Munch, to_yaml_safe)
 
     Representer.add_representer(Munch, to_yaml)
     Representer.add_multi_representer(Munch, to_yaml)
```

### Comparing `munch-3.0.0/munch.egg-info/PKG-INFO` & `munch-4.0.0/munch.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: munch
-Version: 3.0.0
+Version: 4.0.0
 Summary: A dot-accessible dictionary (a la JavaScript objects)
 Home-page: https://github.com/Infinidat/munch
 Author: Rotem Yaari
 Author-email: vmalloc@gmail.com
 License: MIT
 Keywords: munch,dict,mapping,container,collection
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,22 +23,31 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 Provides-Extra: yaml
 License-File: LICENSE.txt
 
-[![Build Status](https://travis-ci.org/Infinidat/munch.svg?branch=master)](https://travis-ci.org/Infinidat/munch)
 [![Latest Version](https://img.shields.io/pypi/v/munch.svg)](https://pypi.python.org/pypi/munch/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/munch.svg)](https://pypi.python.org/pypi/munch/)
 [![Downloads](https://img.shields.io/pypi/dm/munch.svg)](https://pypi.python.org/pypi/munch/)
 
 munch
 ==========
 
+Installation
+-------------
+
+```
+pip install munch
+```
+
+Usage
+-----
+
 munch is a fork of David Schoonover's **Bunch** package, providing similar functionality. 99% of the work was done by him, and the fork was made mainly for lack of responsiveness for fixes and maintenance on the original code.
 
 Munch is a dictionary that supports attribute-style access, a la JavaScript:
 
 ```python
 
 >>> from munch import Munch
```

### Comparing `munch-3.0.0/setup.cfg` & `munch-4.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `munch-3.0.0/tests/conftest.py` & `munch-4.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `munch-3.0.0/tests/test_munch.py` & `munch-4.0.0/tests/test_munch.py`

 * *Files identical despite different names*

### Comparing `munch-3.0.0/tests/test_yaml.py` & `munch-4.0.0/tests/test_yaml.py`

 * *Files identical despite different names*

