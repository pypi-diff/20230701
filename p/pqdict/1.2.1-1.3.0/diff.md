# Comparing `tmp/pqdict-1.2.1.tar.gz` & `tmp/pqdict-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqdict-1.2.1.tar", last modified: Mon Jun 26 20:08:13 2023, max compression
+gzip compressed data, was "pqdict-1.3.0.tar", last modified: Sat Jul  1 20:50:29 2023, max compression
```

## Comparing `pqdict-1.2.1.tar` & `pqdict-1.3.0.tar`

### file list

```diff
@@ -1,31 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:08:13.009665 pqdict-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-06-26 20:08:03.000000 pqdict-1.2.1/CHANGES
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-26 20:08:03.000000 pqdict-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-26 20:08:03.000000 pqdict-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-26 20:08:13.009665 pqdict-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-26 20:08:03.000000 pqdict-1.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:08:13.005665 pqdict-1.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-06-26 20:08:03.000000 pqdict-1.2.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-06-26 20:08:03.000000 pqdict-1.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-26 20:08:03.000000 pqdict-1.2.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)    62591 2023-06-26 20:08:03.000000 pqdict-1.2.1/docs/gillespie-output.png
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-26 20:08:03.000000 pqdict-1.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-06-26 20:08:03.000000 pqdict-1.2.1/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-26 20:08:03.000000 pqdict-1.2.1/docs/pqdict.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-06-26 20:08:03.000000 pqdict-1.2.1/docs/release.rst
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-26 20:08:03.000000 pqdict-1.2.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:08:13.009665 pqdict-1.2.1/pqdict/
--rw-r--r--   0 runner    (1001) docker     (123)    19638 2023-06-26 20:08:03.000000 pqdict-1.2.1/pqdict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-26 20:08:03.000000 pqdict-1.2.1/pqdict/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:08:03.000000 pqdict-1.2.1/pqdict/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:08:13.009665 pqdict-1.2.1/pqdict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-26 20:08:12.000000 pqdict-1.2.1/pqdict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-26 20:08:13.000000 pqdict-1.2.1/pqdict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:08:12.000000 pqdict-1.2.1/pqdict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:08:12.000000 pqdict-1.2.1/pqdict.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 20:08:12.000000 pqdict-1.2.1/pqdict.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 20:08:12.000000 pqdict-1.2.1/pqdict.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-26 20:08:13.009665 pqdict-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-26 20:08:03.000000 pqdict-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:08:13.009665 pqdict-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    14721 2023-06-26 20:08:03.000000 pqdict-1.2.1/tests/test_pqdict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:50:29.590369 pqdict-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-01 20:50:18.000000 pqdict-1.3.0/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-01 20:50:18.000000 pqdict-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-01 20:50:18.000000 pqdict-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-01 20:50:29.590369 pqdict-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-01 20:50:18.000000 pqdict-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:50:29.590369 pqdict-1.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-07-01 20:50:18.000000 pqdict-1.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-07-01 20:50:18.000000 pqdict-1.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-01 20:50:18.000000 pqdict-1.3.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    62591 2023-07-01 20:50:18.000000 pqdict-1.3.0/docs/gillespie-output.png
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-01 20:50:18.000000 pqdict-1.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-01 20:50:18.000000 pqdict-1.3.0/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-01 20:50:18.000000 pqdict-1.3.0/docs/pqdict.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-01 20:50:18.000000 pqdict-1.3.0/docs/release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 20:50:18.000000 pqdict-1.3.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:50:29.590369 pqdict-1.3.0/pqdict/
+-rw-r--r--   0 runner    (1001) docker     (123)    22812 2023-07-01 20:50:18.000000 pqdict-1.3.0/pqdict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 20:50:18.000000 pqdict-1.3.0/pqdict/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:50:29.590369 pqdict-1.3.0/pqdict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-01 20:50:29.000000 pqdict-1.3.0/pqdict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-01 20:50:29.000000 pqdict-1.3.0/pqdict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 20:50:29.000000 pqdict-1.3.0/pqdict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-01 20:50:29.000000 pqdict-1.3.0/pqdict.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-01 20:50:29.000000 pqdict-1.3.0/pqdict.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-01 20:50:18.000000 pqdict-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 20:50:29.590369 pqdict-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:50:29.590369 pqdict-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    15585 2023-07-01 20:50:18.000000 pqdict-1.3.0/tests/test_pqdict.py
```

### Comparing `pqdict-1.2.1/CHANGES` & `pqdict-1.3.0/CHANGES`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,35 @@
 Release Notes
 =============
 
+1.3.0 (2023-07-01)
+++++++++++++++++++
+
+This release drops support for Python versions below 3.7
+
+* API changes:
+	- Added ``popvalue`` method to mirror recent ``topvalue`` addition.
+	- Added ``default`` argument to ``top`` and support for ``default`` using ``pop`` with PQ semantics. This value is returned when the collection is empty.
+
+* Maintenance:
+	- Dropped support for Python 2.7, 3.4, 3.5, and 3.6 (#22).
+	- Inlined type annotations and removed stub file. Thanks for advice from `@aqeelat <https://github.com/aqeelat>_`.
+	- Migrate to pyproject.toml
+	- Linting and static type checking in CI
+
+
 1.2.1 (2023-06-26)
 ++++++++++++++++++
 
 * Typing:
 	- Provided typing support (#19) applying stub generated by `@noamraph <https://github.com/noamraph>`_
 
 * Maintenance:
 	- Replaced CI badge.
-	- Dropped Python 2.7, no longer supported in CI. Next minor release will no longer support Python 2.
+	- Dropped Python 2.7 from CI, no longer supported there. Next minor release of pqdict will no longer support Python 2.
 
 
 1.2.0 (2022-10-14)
 ++++++++++++++++++
 
 * API changes:
 	- Added ``topvalue`` method (#17). By `@ShivKJ <https://github.com/ShivKJ>`_
```

### Comparing `pqdict-1.2.1/LICENSE` & `pqdict-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pqdict-1.2.1/README.rst` & `pqdict-1.3.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 Priority Queue Dictionary (pqdict)
 ==================================
 
 A priority queue dictionary maps hashable objects (keys) to priority-determining values. It provides a hybrid dictionary/priority queue API. 
 
-Works with Python 2.7+, 3.4+, and PyPy.
-
 .. image:: https://github.com/nvictus/priority-queue-dictionary/actions/workflows/package_lint-test.yml/badge.svg
     :target: https://github.com/nvictus/priority-queue-dictionary/actions/workflows/package_lint-test.yml
     :alt: CI
 
 .. image:: https://readthedocs.org/projects/pqdict/badge/?version=latest
     :target: https://readthedocs.org/projects/pqdict/
     :alt: Documentation Status
```

### Comparing `pqdict-1.2.1/docs/Makefile` & `pqdict-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pqdict-1.2.1/docs/conf.py` & `pqdict-1.3.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #!/usr/bin/env python3
-# -*- coding: utf-8 -*-
 #
 # pqdict documentation build configuration file, created by
 # sphinx-quickstart on Sat Aug 29 16:46:59 2015.
 #
 # This file is execfile()d with the current directory set to its
 # containing dir.
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
-import sys
 import os
-import shlex
 import re
+import sys
+from datetime import datetime
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #sys.path.insert(0, os.path.abspath('.'))
 sys.path.insert(0, os.path.abspath('..'))
 
@@ -54,15 +53,16 @@
 #source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = 'pqdict'
-copyright = '2015, Nezar Abdennur'
+year = datetime.now().year
+copyright = f'2012-{year}, Nezar Abdennur'
 author = 'Nezar Abdennur'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 def _get_version():
     init = os.path.join("..", "pqdict", "__init__.py")
@@ -80,15 +80,15 @@
 version = release.rsplit(".", maxsplit=1)[0]
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 #today = ''
 # Else, today_fmt is used as the format for a strftime call.
 #today_fmt = '%B %d, %Y'
```

### Comparing `pqdict-1.2.1/docs/gillespie-output.png` & `pqdict-1.3.0/docs/gillespie-output.png`

 * *Files identical despite different names*

### Comparing `pqdict-1.2.1/docs/intro.rst` & `pqdict-1.3.0/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `pqdict-1.2.1/docs/pqdict.rst` & `pqdict-1.3.0/docs/pqdict.rst`

 * *Files 8% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 
 
 pqdict class
 ------------
 .. autoclass:: pqdict
     :no-members:
 
-    .. automethod:: fromkeys
+    .. automethod:: minpq
 
-    .. automethod:: heapify([key])
+    .. automethod:: maxpq
+    
+    .. automethod:: fromkeys
 
     |
 
     **Properties**
 
     .. autoattribute:: keyfn
 
@@ -40,86 +42,96 @@
 
     .. method:: key in pq
     
     .. automethod:: get(key[, default])
 
     .. method:: pop([key[, default]])
 
-        If ``key`` is in the pqdict, remove it and return its priority value,
-        else return ``default``. If ``default`` is not provided and ``key`` is
-        not in the pqdict, raise a ``KeyError``.
+        Hybrid pop method.
+
+        With ``key``, perform a dictionary pop:
+        
+        * If ``key`` is in the pqdict, remove the item and return its
+          **value**.
+        * If ``key`` is not in the pqdict, return ``default`` if provided,
+          otherwise raise a ``KeyError``.
 
     .. automethod:: clear 
     
     .. automethod:: update([other]) 
 
     .. automethod:: setdefault(key[, default]) 
 
     .. automethod:: copy()
 
     Iterators and Views
 
     .. warning:: 
-        For the following sequences, order is arbitrary.
+        For the sequences returned by the following methods, the **iteration order is arbitrary**.
+
+        See further below for sorted iterators :meth:`popkeys`, :meth:`popvalues`, and :meth:`popitems`.
 
     .. method:: iter(pq)
 
     .. automethod:: keys
 
     .. automethod:: values 
 
     .. automethod:: items
 
-    .. note::
-        In Python 2, the above methods return lists rather than views and ``pqdict`` includes additional iterator methods ``iterkeys()``, ``itervalues()`` and ``iteritems()``.
-
     |
 
     **Priority Queue API**
 
     .. automethod:: top
 
     .. automethod:: topvalue
+
+    .. automethod:: topitem
     
-    .. method:: pop([key[, default]])
+    .. method:: pop(*, [default])
 
-        If ``key`` is not provided, remove the top item and return its key, or
-        raise ``KeyError`` if the pqdict is empty.
+        Hybrid pop method.
 
-    .. automethod:: additem
+        Without ``key``, perform a priority queue pop:
 
-    .. automethod:: updateitem
-
-    .. automethod:: topitem
+        * Remove the top item and return its **key**.
+        * If the pqdict is empty, return ``default`` if provided, otherwise
+          raise a ``KeyError``.
 
+    .. automethod:: popvalue
+    
     .. automethod:: popitem
 
+    .. automethod:: additem
+
+    .. automethod:: updateitem
+
     .. automethod:: pushpopitem(key, value)
 
     .. automethod:: replace_key
 
     .. automethod:: swap_priority
 
-    Heapsort Iterators
+    .. automethod:: heapify([key])
+
+    Sorted Iterators
 
     .. note::
         Iteration is in descending order of priority.
 
-    .. danger::
-        Heapsort iterators are destructive: they are generators that pop items out of the heap, which amounts to performing a heapsort.
+    .. warning::
+        Sorted iterators are destructive: they are generators that pop items out of the heap, which amounts to performing a heapsort.
 
     .. automethod:: popkeys
 
     .. automethod:: popvalues 
 
     .. automethod:: popitems
 
-    .. warning::
-        The names of the heapsort iterators in v0.5 (iterkeys, itervalues, iteritems) were changed in v0.6 to be more transparent: These names are not provided at all in Python 3, and in Python 2 they are now part of the dictionary API.
-
 
 Functions
 ---------
 .. autofunction:: pqdict.nsmallest
 
 .. autofunction:: pqdict.nlargest
```

### Comparing `pqdict-1.2.1/docs/release.rst` & `pqdict-1.3.0/docs/release.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,35 @@
 Release Notes
 =============
 
+1.3.0 (2023-07-01)
+++++++++++++++++++
+
+This release drops support for Python versions below 3.7
+
+* API changes:
+	- Added ``popvalue`` method to mirror recent ``topvalue`` addition.
+	- Added ``default`` argument to ``top`` and support for ``default`` using ``pop`` with PQ semantics. This value is returned when the collection is empty.
+
+* Maintenance:
+	- Dropped support for Python 2.7, 3.4, 3.5, and 3.6 (#22).
+	- Inlined type annotations and removed stub file. Thanks for advice from `@aqeelat <https://github.com/aqeelat>_`.
+	- Migrate to pyproject.toml
+	- Linting and static type checking in CI
+
+
 1.2.1 (2023-06-26)
 ++++++++++++++++++
 
 * Typing:
 	- Provided typing support (#19) applying stub generated by `@noamraph <https://github.com/noamraph>`_
 
 * Maintenance:
 	- Replaced CI badge.
-	- Dropped Python 2.7, no longer supported in CI. Next minor release will no longer support Python 2.
+	- Dropped Python 2.7 from CI, no longer supported there. Next minor release of pqdict will no longer support Python 2.
 
 
 1.2.0 (2022-10-14)
 ++++++++++++++++++
 
 * API changes:
 	- Added ``topvalue`` method (#17). By `@ShivKJ <https://github.com/ShivKJ>`_
```

### Comparing `pqdict-1.2.1/pqdict/__init__.py` & `pqdict-1.3.0/pqdict/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 Priority Queue Dictionary (pqdict)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 A Pythonic indexed priority queue.
 
 A dict-like heap queue to prioritize hashable objects while providing random
@@ -26,241 +25,284 @@
 
 - O(log n) removal of any item
 
 - O(log n) updating of any item's priority level
 
 Documentation at <http://pqdict.readthedocs.org/en/latest>.
 
-:copyright: (c) 2012-2015 by Nezar Abdennur.
+:copyright: (c) 2012-2023 by Nezar Abdennur.
 :license: MIT, see LICENSE for more details.
 
 """
-try:
-    from collections.abc import MutableMapping as _MutableMapping
-except ImportError:
-    # 2.7 compatability
-    from collections import MutableMapping as _MutableMapping  # type: ignore
+from collections.abc import MutableMapping
+from operator import gt, lt
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    Iterator,
+    List,
+    Mapping,
+    Optional,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+)
+from warnings import warn
 
-from six.moves import range
-from operator import lt, gt
+__version__ = "1.3.0"
+__all__ = ["pqdict", "nlargest", "nsmallest"]
 
+DictInputs = Union[Mapping[Any, Any], Iterable[Tuple[Any, Any]]]
+Tpqdict = TypeVar("Tpqdict", bound="pqdict")
 
-__version__ = "1.2.1"
-__all__ = ["pqdict", "PQDict", "minpq", "maxpq", "nlargest", "nsmallest"]
 
-
-class _Node(object):
+class Node:
     __slots__ = ("key", "value", "prio")
 
-    def __init__(self, key, value, prio):
+    key: Any
+    value: Any
+    prio: Any
+
+    def __init__(self, key: Any, value: Any, prio: Any) -> None:
         self.key = key
         self.value = value
         self.prio = prio
 
-    def __repr__(self):
-        return self.__class__.__name__ + "(%s, %s, %s)" % (
-            repr(self.key),
-            repr(self.value),
-            repr(self.prio),
-        )
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}({self.key}, {self.value}, {self.prio})"
 
 
-class pqdict(_MutableMapping):  # pyright: ignore # Argument to class must be a base class (reportGeneralTypeIssues
+class pqdict(MutableMapping):
     """
     A collection that maps hashable objects (keys) to priority-determining
     values. The mapping is mutable so items may be added, removed and have
     their priority level updated.
 
+    The default behavior is that of a min-priority queue, i.e. the item with
+    the *smallest* priority value is given *highest* priority. This behavior
+    can be reversed by specifying ``reverse=True`` or by providing a custom
+    precedence function via the ``precedes`` keyword argument. Alternatively,
+    use the explicit :meth:`pqdict.minpq` or :meth:`pqdict.maxpq` class methods.
+
     Parameters
     ----------
     data : mapping or iterable, optional
         Input data, e.g. a dictionary or a sequence of items.
     key : callable, optional
         Optional priority key function to transform values into priority keys
-        for sorting. By default, the values are not transformed.
-    reverse : bool, optional
+        for comparison. By default, the values are used directly as priority
+        keys and are not transformed.
+    reverse : bool, optional [default: ``False``]
         If ``True``, *larger* priority keys give items *higher* priority.
         Default is ``False``.
-    precedes : callable, optional (overrides ``reverse``)
+    precedes : callable, optional [default: ``operator.lt``]
         Function that determines precedence of a pair of priority keys. The
         default comparator is ``operator.lt``, meaning *smaller* priority keys
-        give items *higher* priority.
-
+        give items *higher* priority. The callable must have the form
+        ``precedes(prio1, prio2) -> bool`` and return ``True`` if ``prio1``
+        has higher priority than ``prio2``. Overrides ``reverse``.
     """
 
-    def __init__(self, data=None, key=None, reverse=False, precedes=lt):
+    _heap: List[Node]
+    _position: Dict[Any, int]
+
+    def __init__(
+        self,
+        data: Optional[DictInputs] = None,
+        key: Optional[Callable[[Any], Any]] = None,
+        reverse: bool = False,
+        precedes: Callable[[Any, Any], bool] = lt,
+    ) -> None:
         if reverse:
             if precedes == lt:
                 precedes = gt
             else:
                 raise ValueError("Got both `reverse=True` and a custom `precedes`.")
 
         if key is None or callable(key):
             self._keyfn = key
         else:
-            raise ValueError(
-                "`key` function must be a callable; got {}".format(type(key))
-            )
+            raise ValueError(f"`key` function must be a callable; got {key}")
 
         if callable(precedes):
             self._precedes = precedes
         else:
-            raise ValueError(
-                "`precedes` function must be a callable; got {}".format(type(precedes))
-            )
+            raise ValueError(f"`precedes` function must be a callable; got {precedes}")
 
         # The heap
         self._heap = []
 
         # The index
         self._position = {}
 
         if data is not None:
             self.update(data)
 
     @property
-    def precedes(self):
+    def precedes(self) -> Callable[[Any, Any], bool]:
         """Priority key precedence function"""
         return self._precedes
 
     @property
-    def keyfn(self):
+    def keyfn(self) -> Callable[[Any], Any]:
         """Priority key function"""
         return self._keyfn if self._keyfn is not None else lambda x: x
 
-    def __repr__(self):
-        things = ", ".join(
-            ["%s: %s" % (repr(node.key), repr(node.value)) for node in self._heap]
-        )
-        return self.__class__.__name__ + "({" + things + "})"
+    def __repr__(self) -> str:
+        things = ", ".join([f"{node.key}: {node.value}" for node in self._heap])
+        return f"{self.__class__.__name__}({things})"
+
+    @classmethod
+    def minpq(cls: Type[Tpqdict], *args: Any, **kwargs: Any) -> Tpqdict:
+        """Create a pqdict with min-priority semantics: smallest is highest."""
+        return cls(dict(*args, **kwargs), precedes=lt)
+
+    @classmethod
+    def maxpq(cls: Type[Tpqdict], *args: Any, **kwargs: Any) -> Tpqdict:
+        """Create a pqdict with max-priority semantics: largest is highest."""
+        return cls(dict(*args, **kwargs), precedes=gt)
 
     ############
     # dict API #
     ############
-    __marker = object()
-    __eq__ = _MutableMapping.__eq__
-    __ne__ = _MutableMapping.__ne__
-    keys = _MutableMapping.keys
-    values = _MutableMapping.values
-    items = _MutableMapping.items
-    get = _MutableMapping.get
-    clear = _MutableMapping.clear
-    update = _MutableMapping.update
-    setdefault = _MutableMapping.setdefault
+    __marker: object = object()
+    # __eq__ = MutableMapping.__eq__
+    # __ne__ = MutableMapping.__ne__
+    # keys = MutableMapping.keys
+    # values = MutableMapping.values
+    # items = MutableMapping.items
+    # get = MutableMapping.get
+    # clear = MutableMapping.clear
+    # update = MutableMapping.update
+    # setdefault = MutableMapping.setdefault
 
     @classmethod
-    def fromkeys(cls, iterable, value, **kwargs):
+    def fromkeys(
+        cls: Type[Tpqdict], iterable: Iterable, value: Any, **kwargs: Any
+    ) -> Tpqdict:
         """
-        Return a new pqict mapping keys from an iterable to the same value.
-
+        Return a new pqdict mapping keys from an iterable to the same value.
         """
         return cls(((k, value) for k in iterable), **kwargs)
 
-    def __len__(self):
+    def __len__(self) -> int:
         """
         Return number of items in the pqdict.
-
         """
         return len(self._heap)
 
-    def __contains__(self, key):
+    def __contains__(self, key: Any) -> bool:
         """
         Return ``True`` if key is in the pqdict.
-
         """
         return key in self._position
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[Any]:
         """
         Return an iterator over the keys of the pqdict. The order of iteration
         is arbitrary! Use ``popkeys`` to iterate over keys in priority order.
-
         """
         for node in self._heap:
             yield node.key
 
-    def __getitem__(self, key):
+    def __getitem__(self, key: Any) -> Any:
         """
         Return the priority value of ``key``. Raises a ``KeyError`` if not in
         the pqdict.
-
         """
         return self._heap[self._position[key]].value  # raises KeyError
 
-    def __setitem__(self, key, value):
+    def __setitem__(self, key: Any, value: Any) -> None:
         """
-        Assign a priority value to ``key``.
-
+        Assign a priority value to ``key``. If ``key`` is already in the
+        pqdict, its priority value is updated.
         """
         heap = self._heap
         position = self._position
         keygen = self._keyfn
         try:
             pos = position[key]
         except KeyError:
             # add
             n = len(heap)
             prio = keygen(value) if keygen is not None else value
-            heap.append(_Node(key, value, prio))
+            heap.append(Node(key, value, prio))
             position[key] = n
             self._swim(n)
         else:
             # update
             prio = keygen(value) if keygen is not None else value
             heap[pos].value = value
             heap[pos].prio = prio
             self._reheapify(pos)
 
-    def __delitem__(self, key):
+    def __delitem__(self, key: Any) -> None:
         """
         Remove item. Raises a ``KeyError`` if key is not in the pqdict.
-
         """
         heap = self._heap
         position = self._position
         pos = position.pop(key)  # raises KeyError
         node_to_delete = heap[pos]
         # Take the very last node and place it in the vacated spot. Let it
         # sink or swim until it reaches its new resting place.
         end = heap.pop(-1)
         if end is not node_to_delete:
             heap[pos] = end
             position[end.key] = pos
             self._reheapify(pos)
         del node_to_delete
 
-    def copy(self):
+    def copy(self: Tpqdict) -> Tpqdict:
         """
         Return a shallow copy of a pqdict.
-
         """
         other = self.__class__(key=self._keyfn, precedes=self._precedes)
         other._position = self._position.copy()
-        other._heap = [_Node(node.key, node.value, node.prio) for node in self._heap]
+        other._heap = [Node(node.key, node.value, node.prio) for node in self._heap]
         return other
 
-    def pop(self, key=__marker, default=__marker):
-        """
-        If ``key`` is in the pqdict, remove it and return its priority value,
-        else return ``default``. If ``default`` is not provided and ``key`` is
-        not in the pqdict, raise a ``KeyError``.
-
-        If ``key`` is not provided, remove the top item and return its key, or
-        raise ``KeyError`` if the pqdict is empty.
-
+    def pop(
+        self,
+        key: Any = __marker,
+        default: Any = __marker,
+    ) -> Any:
+        """
+        Hybrid pop method.
+
+        With ``key``, perform a dictionary pop:
+
+        * If ``key`` is in the pqdict, remove the item and return its
+          **value**.
+        * If ``key`` is not in the pqdict, return ``default`` if provided,
+          otherwise raise a ``KeyError``.
+
+        Without ``key``, perform a priority queue pop:
+
+        * Remove the top item and return its **key**.
+        * If the pqdict is empty, return ``default`` if provided, otherwise
+          raise a ``KeyError``.
         """
         heap = self._heap
         position = self._position
+
         # pq semantics: remove and return top *key* (value is discarded)
         if key is self.__marker:
             if not heap:
-                raise KeyError("pqdict is empty")
+                if default is self.__marker:
+                    raise KeyError("pqdict is empty")
+                else:
+                    return default
             key = heap[0].key
             del self[key]
             return key
+
         # dict semantics: remove and return *value* mapped from key
         try:
             pos = position.pop(key)  # raises KeyError
         except KeyError:
             if default is self.__marker:
                 raise
             return default
@@ -274,31 +316,77 @@
             value = node_to_delete.value
             del node_to_delete
             return value
 
     ######################
     # Priority Queue API #
     ######################
-    def top(self):
+    def top(self, default: Any = __marker) -> Any:
         """
-        Return the key of the item with highest priority. Raises ``KeyError``
-        if pqdict is empty.
+        Return the key of the item with highest priority. If ``default`` is
+        provided and pqdict is empty, then return``default``, otherwise raise
+        ``KeyError``.
+        """
+        try:
+            node = self._heap[0]
+        except IndexError:
+            if default is self.__marker:
+                raise KeyError("pqdict is empty")
+            else:
+                return default
+        return node.key
+
+    def topvalue(self, default: Any = __marker) -> Any:
+        """
+        Return the value of the item with highest priority. If ``default`` is
+        provided and pqdict is empty, then return``default``, otherwise raise
+        ``KeyError``.
+        """
+        try:
+            node = self._heap[0]
+        except IndexError:
+            if default is self.__marker:
+                raise KeyError("pqdict is empty")
+            else:
+                return default
+        return node.value
 
+    def topitem(self) -> Tuple[Any, Any]:
+        """
+        Return the item with highest priority. Raises ``KeyError`` if pqdict is
+        empty.
         """
         try:
             node = self._heap[0]
         except IndexError:
             raise KeyError("pqdict is empty")
-        return node.key
+        return node.key, node.value
+
+    def popvalue(self, default: Any = __marker) -> Any:
+        """
+        Remove and return the value of the item with highest priority. If
+        ``default`` is provided and pqdict is empty, then return``default``,
+        otherwise raise ``KeyError``.
+        """
+        heap = self._heap
+
+        if not heap:
+            if default is self.__marker:
+                raise KeyError("pqdict is empty")
+            else:
+                return default
+
+        value = heap[0].value
+        del self[heap[0].key]
+        return value
 
-    def popitem(self):
+    def popitem(self) -> Tuple[Any, Any]:
         """
         Remove and return the item with highest priority. Raises ``KeyError``
         if pqdict is empty.
-
         """
         heap = self._heap
         position = self._position
 
         try:
             end = heap.pop(-1)
         except IndexError:
@@ -310,155 +398,136 @@
             position[end.key] = 0
             self._sink(0)
         else:
             node = end
         del position[node.key]
         return node.key, node.value
 
-    def topitem(self):
-        """
-        Return the item with highest priority. Raises ``KeyError`` if pqdict is
-        empty.
-
-        """
-        try:
-            node = self._heap[0]
-        except IndexError:
-            raise KeyError("pqdict is empty")
-        return node.key, node.value
-
-    def additem(self, key, value):
+    def additem(self, key: Any, value: Any) -> None:
         """
         Add a new item. Raises ``KeyError`` if key is already in the pqdict.
-
         """
         if key in self._position:
-            raise KeyError("%s is already in the queue" % repr(key))
+            raise KeyError(f"{key} is already in the queue")
         self[key] = value
 
-    def pushpopitem(self, key, value):
+    def pushpopitem(self, key: Any, value: Any) -> Tuple[Any, Any]:
         """
         Equivalent to inserting a new item followed by removing the top
         priority item, but faster. Raises ``KeyError`` if the new key is
         already in the pqdict.
-
         """
         heap = self._heap
         position = self._position
         precedes = self._precedes
         prio = self._keyfn(value) if self._keyfn else value
-        node = _Node(key, value, prio)
+        node = Node(key, value, prio)
         if key in self:
-            raise KeyError("%s is already in the queue" % repr(key))
+            raise KeyError(f"{key} is already in the queue")
         if heap and precedes(heap[0].prio, node.prio):
             node, heap[0] = heap[0], node
             position[key] = 0
             del position[node.key]
             self._sink(0)
         return node.key, node.value
 
-    def updateitem(self, key, new_val):
+    def updateitem(self, key: Any, new_val: Any) -> None:
         """
         Update the priority value of an existing item. Raises ``KeyError`` if
         key is not in the pqdict.
-
         """
         if key not in self._position:
             raise KeyError(key)
         self[key] = new_val
 
-    def replace_key(self, key, new_key):
+    def replace_key(self, key: Any, new_key: Any) -> None:
         """
         Replace the key of an existing heap node in place. Raises ``KeyError``
         if the key to replace does not exist or if the new key is already in
         the pqdict.
-
         """
         heap = self._heap
         position = self._position
         if new_key in self:
-            raise KeyError("%s is already in the queue" % repr(new_key))
+            raise KeyError(f"{new_key} is already in the queue")
         pos = position.pop(key)  # raises appropriate KeyError
         position[new_key] = pos
         heap[pos].key = new_key
 
-    def swap_priority(self, key1, key2):
+    def swap_priority(self, key1: Any, key2: Any) -> None:
         """
         Fast way to swap the priority level of two items in the pqdict. Raises
         ``KeyError`` if either key does not exist.
-
         """
         heap = self._heap
         position = self._position
         if key1 not in self or key2 not in self:
             raise KeyError
         pos1, pos2 = position[key1], position[key2]
         heap[pos1].key, heap[pos2].key = key2, key1
         position[key1], position[key2] = pos2, pos1
 
-    def popkeys(self):
+    def popkeys(self) -> Iterator[Any]:
         """
-        Heapsort iterator over keys in descending order of priority level.
-
+        Remove items, returning keys in descending order of priority rank.
         """
         try:
             while True:
                 yield self.popitem()[0]
         except KeyError:
             return
 
-    def popvalues(self):
+    def popvalues(self) -> Iterator[Any]:
         """
-        Heapsort iterator over values in descending order of priority level.
-
+        Remove items, returning values in descending order of priority rank.
         """
         try:
             while True:
                 yield self.popitem()[1]
         except KeyError:
             return
 
-    def popitems(self):
+    def popitems(self) -> Iterator[Tuple[Any, Any]]:
         """
-        Heapsort iterator over items in descending order of priority level.
-
+        Remove and return items in descending order of priority rank.
         """
         try:
             while True:
                 yield self.popitem()
         except KeyError:
             return
 
-    def heapify(self, key=__marker):
+    def heapify(self, key: Any = __marker) -> None:
         """
         Repair a broken heap. If the state of an item's priority value changes
         you can re-sort the relevant item only by providing ``key``.
-
         """
         if key is self.__marker:
             n = len(self._heap)
             # No need to look at any node without a child.
             for pos in reversed(range(n // 2)):
                 self._sink(pos)
         else:
             try:
                 pos = self._position[key]
             except KeyError:
                 raise KeyError(key)
             self._reheapify(pos)
 
-    # Heap algorithms
+    ###################
+    # Heap algorithms #
+    ###################
     # The names of the heap operations in `heapq` (sift up/down) refer to the
     # motion of the nodes being compared to, rather than the node being
     # operated on as is usually done in textbooks (i.e. bubble down/up,
     # instead). Here I use the sink/swim nomenclature from
     # http://algs4.cs.princeton.edu/24pq/. The way I like to think of it, an
     # item that is too "heavy" (low-priority) should sink down the tree, while
     # one that is too "light" should float or swim up.
-    def _reheapify(self, pos):
+    def _reheapify(self, pos: int) -> None:
         # update existing node:
         # bubble up or down depending on values of parent and children
         heap = self._heap
         precedes = self._precedes
         parent_pos = (pos - 1) >> 1
         child_pos = 2 * pos + 1
         if parent_pos > -1 and precedes(heap[pos].prio, heap[parent_pos].prio):
@@ -468,15 +537,15 @@
             if other_pos < len(heap) and not precedes(
                 heap[child_pos].prio, heap[other_pos].prio
             ):
                 child_pos = other_pos
             if precedes(heap[child_pos].prio, heap[pos].prio):
                 self._sink(pos)
 
-    def _sink(self, top=0):
+    def _sink(self, top: int = 0) -> None:
         # "Sink-to-the-bottom-then-swim" algorithm (Floyd, 1964)
         # Tends to reduce the number of comparisons when inserting "heavy"
         # items at the top, e.g. during a heap pop. See heapq for more details.
         heap = self._heap
         position = self._position
         precedes = self._precedes
         endpos = len(heap)
@@ -501,15 +570,15 @@
             child_pos = 2 * pos + 1
         # We are left with a "vacant" leaf. Put our node there and let it swim
         # until it reaches its new resting place.
         heap[pos] = node
         position[node.key] = pos
         self._swim(pos, top)
 
-    def _swim(self, pos, top=0):
+    def _swim(self, pos: int, top: int = 0) -> None:
         heap = self._heap
         position = self._position
         precedes = self._precedes
         # Grab the node from its place
         node = heap[pos]
         # Sift parents down until we find a place where the node fits.
         while pos > top:
@@ -521,128 +590,120 @@
                 pos = parent_pos
                 continue
             break
         # Put node in its new place
         heap[pos] = node
         position[node.key] = pos
 
-    def topvalue(self, default=__marker):
-        """
-        :param default: if provided, then returning it when priority queue is empty.
-                        If default is not provided and priority queue is empty,
-                        then raising KeyError (as returned by ".topitem()")
-        :return: the top value from priority queue
-        """
-        try:
-            _, v = self.topitem()
-            return v
-        except KeyError:
-            if default is self.__marker:
-                raise  # no default value provided so raising the KeyError
-            else:
-                return default
 
 ###########
 # Aliases #
 ###########
 
 
-PQDict = pqdict  # deprecated
-
-
-def minpq(*args, **kwargs):
+def minpq(*args: Any, **kwargs: Any) -> pqdict:
+    warn(
+        "The `minpq` module function is deprecated and will be removed in v1.4. "
+        "Use the classmethod `pqdict.minpq()` instead.",
+        DeprecationWarning,
+        stacklevel=2
+    )
     return pqdict(dict(*args, **kwargs), precedes=lt)
 
 
-def maxpq(*args, **kwargs):
+def maxpq(*args: Any, **kwargs: Any) -> pqdict:
+    warn(
+        "The `maxpq` module function is deprecated and will be removed in v1.4. "
+        "Use the classmethod `pqdict.maxpq()` instead.",
+        DeprecationWarning,
+        stacklevel=2
+    )
     return pqdict(dict(*args, **kwargs), precedes=gt)
 
 
 #############
 # Functions #
 #############
 
 
-def nlargest(n, mapping, key=None):
+def nlargest(n: int, mapping: Mapping, key: Optional[Callable[[Any], Any]] = None):
     """
     Takes a mapping and returns the n keys associated with the largest values
     in descending order. If the mapping has fewer than n items, all its keys
     are returned.
 
-    Equivalent to:
-        ``next(zip(*heapq.nlargest(mapping.items(), key=lambda x: x[1])))``
-
     Parameters
     ----------
     n : int
         The number of keys associated with the largest values
         in descending order
     mapping : Mapping
         A mapping object
     key : callable, optional
         Optional priority key function to transform values into priority keys
         for sorting. By default, the values are not transformed.
 
     Returns
     -------
-    list of up to n keys from the mapping
+    list of up to n keys from the mapping associated with the largest values
 
+    Notes
+    -----
+    This function is equivalent to:
+
+    >>> [item[0] for item in heapq.nlargest(n, mapping.items(), lambda x: x[1])]
     """
-    try:
-        it = mapping.iteritems()
-    except AttributeError:
-        it = iter(mapping.items())
+    it = iter(mapping.items())
     pq = pqdict(key=key, precedes=lt)
     try:
-        for i in range(n):
+        for _ in range(n):
             pq.additem(*next(it))
     except StopIteration:
         pass
     try:
         while it:
             pq.pushpopitem(*next(it))
     except StopIteration:
         pass
     out = list(pq.popkeys())
     out.reverse()
     return out
 
 
-def nsmallest(n, mapping, key=None):
+def nsmallest(n: int, mapping: Mapping, key: Optional[Callable[[Any], Any]] = None):
     """
     Takes a mapping and returns the n keys associated with the smallest values
     in ascending order. If the mapping has fewer than n items, all its keys are
     returned.
 
-    Equivalent to:
-        ``next(zip(*heapq.nsmallest(mapping.items(), key=lambda x: x[1])))``
-
     Parameters
     ----------
     n : int
         The number of keys associated with the smallest values
         in ascending order
     mapping : Mapping
         A mapping object
     key : callable, optional
         Optional priority key function to transform values into priority keys
         for sorting. By default, the values are not transformed.
 
     Returns
     -------
-    list of up to n keys from the mapping
+    list of up to n keys from the mapping associated with the smallest values
 
+    Notes
+    -----
+    This function is equivalent to:
+
+    >>> [item[0] for item in heapq.nsmallest(n, mapping.items(), lambda x: x[1])]
     """
-    try:
-        it = mapping.iteritems()
-    except AttributeError:
-        it = iter(mapping.items())
+    it = iter(mapping.items())
     pq = pqdict(key=key, precedes=gt)
     try:
-        for i in range(n):
+        for _ in range(n):
             pq.additem(*next(it))
     except StopIteration:
         pass
     try:
         while it:
             pq.pushpopitem(*next(it))
     except StopIteration:
```

### Comparing `pqdict-1.2.1/setup.py` & `pqdict-1.3.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,82 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-import io
-import os
-import re
-
-try:
-    from setuptools import setup
-except ImportError:
-    from distutils.core import setup
-
-
-classifiers = """\
-    Development Status :: 5 - Production/Stable
-    Operating System :: OS Independent
-    License :: OSI Approved :: MIT License
-    Programming Language :: Python
-    Programming Language :: Python :: 2
-    Programming Language :: Python :: 2.7
-    Programming Language :: Python :: 3
-    Programming Language :: Python :: 3.4
-    Programming Language :: Python :: 3.5
-    Programming Language :: Python :: 3.6
-    Programming Language :: Python :: 3.7
-    Programming Language :: Python :: 3.8
-    Programming Language :: Python :: 3.9
-    Programming Language :: Python :: 3.10
-    Programming Language :: Python :: 3.11
-    Programming Language :: Python :: Implementation :: CPython
-    Programming Language :: Python :: Implementation :: PyPy
-"""
-
-
-def _read(*parts, **kwargs):
-    filepath = os.path.join(os.path.dirname(__file__), *parts)
-    encoding = kwargs.pop('encoding', 'utf-8')
-    with io.open(filepath, encoding=encoding) as fh:
-        text = fh.read()
-    return text
-
-
-def get_version():
-    version = re.search(
-        r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]',
-        _read('pqdict', '__init__.py'),
-        re.MULTILINE).group(1)
-    return version
-
-
-def get_long_description():
-    return _read('README.rst')
-
-
-setup(
-    name='pqdict',
-    version=get_version(),
-    license='MIT',
-    description='A Pythonic indexed priority queue',
-    long_description=get_long_description(),
-    keywords=['dict', 'priority queue', 'heap', 'scheduler', 'data structures'],
-    author='Nezar Abdennur',
-    author_email='nabdennur@gmail.com',
-    url='https://github.com/nvictus/priority-queue-dictionary',
-    packages=['pqdict'],
-    package_data={
-        'pqdict': ['py.typed', '*.pyi'],
-    },
-    zip_safe=False,
-    classifiers=[s.strip() for s in classifiers.split('\n') if s],
-    install_requires=['six'],
-    tests_require=['pytest'],
-    extras_require={'docs': ['Sphinx>=1.1', 'numpydoc']},
-)
+[build-system]
+requires = ["setuptools>=43.0.0", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "pqdict"
+description = "A Pythonic indexed priority queue."
+requires-python = ">=3.7"
+license = {text = "MIT"}
+authors = [
+  {name = "Nezar Abdennur", email = "nabdennur@gmail.com"},
+]
+keywords = [
+    "dict", 
+    "priority queue", 
+    "heap", 
+    "scheduler", 
+    "data structures",
+]
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Operating System :: OS Independent",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: Implementation :: CPython",
+    "Programming Language :: Python :: Implementation :: PyPy",
+]
+
+dynamic = ["readme", "version"]
+dependencies = []
+
+[project.optional-dependencies]
+test = [
+    "isort",
+    "mypy",
+    "pytest",
+    "pyupgrade",
+    "ruff",
+]
+docs = [
+    "numpydoc",
+    "Sphinx<7.0.0",
+    "sphinx-autobuild",
+    "sphinx_rtd_theme",
+]
+
+[project.urls]
+homepage = "https://github.com/nvictus/priority-queue-dictionary"
+documentation = "https://pqdict.readthedocs.io"
+repository = "https://github.com/nvictus/priority-queue-dictionary"
+changelog = "https://github.com/nvictus/priority-queue-dictionary/blob/master/CHANGES"
+
+[tool.setuptools.dynamic]
+readme = { file = ["README.rst"] }
+version = { attr = "pqdict.__version__" }
+
+[tool.setuptools.package-data]
+pqdict = ['py.typed']
+
+[tool.distutils.bdist_wheel]
+universal = true
+
+[tool.isort]
+profile = "black"
+skip_gitignore = true
+
+[tool.ruff]
+extend-select = [
+    "E",  # style errors
+    # "D",  # pydocstyle
+    "F",  # pyflakes
+    "I",  # isort
+    "RUF", # ruff-specific rules
+    "UP", # pyupgrade
+    "W",  # style  warnings
+]
```

### Comparing `pqdict-1.2.1/tests/test_pqdict.py` & `pqdict-1.3.0/tests/test_pqdict.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-# -*- coding: utf-8 -*-
-from datetime import datetime, timedelta
-from itertools import combinations
 import operator
-import sys
 import random
+import sys
+from datetime import datetime, timedelta
+from itertools import combinations
 
 import pytest
 
-from pqdict import pqdict, minpq, maxpq, nlargest, nsmallest
-
+from pqdict import maxpq, minpq, nlargest, nsmallest, pqdict
 
 sample_keys = ["A", "B", "C", "D", "E", "F", "G"]
 sample_values = [5, 8, 7, 3, 9, 12, 1]
 sample_tuple_values = [
     ("a", 5), ("b", 8), (None, 7), (2.5, 3), ("e", 9), ("f", 12), ("g", 1)
 ]
 sample_items = list(zip(sample_keys, sample_values))
@@ -56,27 +54,28 @@
     assert list(range(n)) == sorted(nodes)
     # All heap entries map back to the correct dictionary key
     for key in pq._position:
         node = pq._heap[pq._position[key]]
         assert key == node.key
 
 
-# The next group of tests were originally in class TestNew
-
+##########
+# Creation
+##########
 
 def test_constructor():
     # sequence of pairs
     pq0 = pqdict(
         [("A", 5), ("B", 8), ("C", 7), ("D", 3), ("E", 9), ("F", 12), ("G", 1)]
     )
     pq1 = pqdict(zip(["A", "B", "C", "D", "E", "F", "G"], [5, 8, 7, 3, 9, 12, 1]))
     # dictionary
     pq2 = pqdict({"A": 5, "B": 8, "C": 7, "D": 3, "E": 9, "F": 12, "G": 1})
     # keyword arguments
-    pq3 = minpq(A=5, B=8, C=7, D=3, E=9, F=12, G=1)
+    pq3 = pqdict.minpq(A=5, B=8, C=7, D=3, E=9, F=12, G=1)
     assert pq0 == pq1 == pq2 == pq3
 
 
 def test_equality():
     # eq
     pq1 = pqdict(sample_items)
     pq2 = pqdict(sample_items)
@@ -85,29 +84,31 @@
     # ne
     pq2[random.choice(sample_keys)] += 1
     assert not pq1 == pq2
     assert pq1 != pq2
     # pqdict == regular dict if they have same key/value pairs
     adict = dict(sample_items)
     assert pq1 == adict
+
     # TODO: FIX?
     # pqdicts evaluate as equal even if they have different
     # key functions and/or precedence functions
-    pq3 = maxpq(sample_items)
+    pq3 = pqdict.maxpq(sample_items)
+
     assert pq1 == pq3
 
 
 def test_minpq():
-    pq = minpq(A=5, B=8, C=7, D=3, E=9, F=12, G=1)
+    pq = pqdict.minpq(A=5, B=8, C=7, D=3, E=9, F=12, G=1)
     assert list(pq.popvalues()) == [1, 3, 5, 7, 8, 9, 12]
     assert pq.precedes == operator.lt
 
 
 def test_maxpq():
-    pq = maxpq(A=5, B=8, C=7, D=3, E=9, F=12, G=1)
+    pq = pqdict.maxpq(A=5, B=8, C=7, D=3, E=9, F=12, G=1)
     assert list(pq.popvalues()) == [12, 9, 8, 7, 5, 3, 1]
     assert pq.precedes == operator.gt
 
 
 def test_fromkeys():
     # assign same value to all
     seq = ["foo", "bar", "baz"]
@@ -125,16 +126,27 @@
     pq = pqdict.fromkeys(seq, float("-inf"), precedes=operator.gt)
     for k in seq:
         assert pq[k] == float("-inf")
     pq["spam"] = 10
     assert pq.pop() == "spam"
 
 
-# The next group of tests were originally in class TestDictAPI
+def test_factory_functions():
+    pq = minpq(A=5, B=8, C=7, D=3, E=9, F=12, G=1)
+    assert list(pq.popvalues()) == [1, 3, 5, 7, 8, 9, 12]
+    assert pq.precedes == operator.lt
 
+    pq = maxpq(A=5, B=8, C=7, D=3, E=9, F=12, G=1)
+    assert list(pq.popvalues()) == [12, 9, 8, 7, 5, 3, 1]
+    assert pq.precedes == operator.gt
+
+
+################
+# Dictionary API
+################
 
 def test_len():
     pq = pqdict()
     assert len(pq) == 0
     pq = pqdict(sample_items)
     assert len(pq) == len(sample_items)
 
@@ -243,15 +255,18 @@
 
 def test_items():
     pq = pqdict(sample_items)
     assert sorted(sample_items) == sorted(pq.items())
     assert sorted(sample_values) == [item[1] for item in pq.popitems()]
 
 
-# The next group of tests were originally inclass TestPQAPI
+####################
+# Priority Queue API
+####################
+
 def test_keyfn():
     pq = pqdict()
     assert pq.keyfn(5) == 5
     pq = pqdict(key=lambda x: len(x))
     assert pq.keyfn([1, 2, 3]) == 3
 
 
@@ -266,46 +281,52 @@
     pq["b"] = (1,)
     pq["c"] = (1, 2)
     pq["d"] = (1, 2, 3)
     assert list(pq.popvalues()) == [(), (1,), (1, 2), (1, 2, 3)]
 
 
 def test_pop():
+    # Dict-pop
     # pop selected item - return value
-    pq = minpq(A=5, B=8, C=1)
+    pq = pqdict.minpq(A=5, B=8, C=1)
     value = pq.pop("B")
     assert value == 8
     pq.pop("A")
     pq.pop("C")
     with pytest.raises(KeyError):
         pq.pop("A")
     with pytest.raises(KeyError):
         pq.pop("does_not_exist")
+    assert pq.pop("does_not_exist", "default") == "default"
+
+    # PQ-pop
     # no args and empty - throws
     with pytest.raises(KeyError):
         pq.pop()  # pq is now empty
+    assert pq.pop(default="default") == "default"
     # no args - return top key
-    pq = minpq(A=5, B=8, C=1)
+    pq = pqdict.minpq(A=5, B=8, C=1)
     assert pq.pop() == "C"
 
 
 def test_top():
     # empty
     pq = pqdict()
     with pytest.raises(KeyError):
         pq.top()
+    assert pq.top("default") == "default"
     # non-empty
     for num_items in range(1, 30):
         items = generate_data("float", num_items)
         pq = pqdict(items)
         assert pq.top() == min(items, key=lambda x: x[1])[0]
 
 
 def test_popitem():
-    pq = minpq(A=5, B=8, C=1)
+    pq = pqdict.minpq(A=5, B=8, C=1)
     # pop top item
     key, value = pq.popitem()
     assert key == "C"
     assert value == 1
 
 
 def test_topitem():
@@ -339,38 +360,38 @@
     assert pq[key] == value + 1.0
     # can only update existing keys
     with pytest.raises(KeyError):
         pq.updateitem("does_not_exist", 99.0)
 
 
 def test_pushpopitem():
-    pq = minpq(A=5, B=8, C=1)
+    pq = pqdict.minpq(A=5, B=8, C=1)
     assert pq.pushpopitem("D", 10) == ("C", 1)
     assert pq.pushpopitem("E", 5) == ("E", 5)
     with pytest.raises(KeyError):
         pq.pushpopitem("A", 99)
 
 
 def test_replace_key():
-    pq = minpq(A=5, B=8, C=1)
+    pq = pqdict.minpq(A=5, B=8, C=1)
     pq.replace_key("A", "Alice")
     pq.replace_key("B", "Bob")
     _check_index(pq)
     assert pq["Alice"] == 5
     assert pq["Bob"] == 8
     with pytest.raises(KeyError):
         pq.__getitem__("A")
     with pytest.raises(KeyError):
         pq.__getitem__("B")
     with pytest.raises(KeyError):
         pq.replace_key("C", "Bob")
 
 
 def test_swap_priority():
-    pq = minpq(A=5, B=8, C=1)
+    pq = pqdict.minpq(A=5, B=8, C=1)
     pq.swap_priority("A", "C")
     _check_index(pq)
     assert pq["A"] == 1
     assert pq["C"] == 5
     assert pq.top() == "A"
     with pytest.raises(KeyError):
         pq.swap_priority("A", "Z")
@@ -390,26 +411,15 @@
         # NOTE: heapsort is NOT a stable sorting method, so keys with equal
         # priority keys are not guaranteed to have the same order as in the
         # original sequence.
         values_heapsorted = list(pq.popvalues())
         assert values_heapsorted == sorted(values)
 
 
-# The next group of tests were originally in class TestOperations
-
-
-@pytest.mark.skipif("sys.version_info <= (3,0)")
-def test_uncomparable():
-    # non-comparable priority keys (Python 3 only)
-    # Python 3 has stricter comparison than Python 2
-    pq = pqdict()
-    pq.additem("a", [])
-    with pytest.raises(TypeError):
-        pq.additem("b", 5)
-
+# Heap invariant tests and key/value types
 
 def test_heapify():
     for size in range(30):
         items = generate_data("int", size)
         pq = pqdict(items)
         _check_heap_invariant(pq)
         assert len(pq._heap) == size
@@ -465,15 +475,15 @@
             del pq[key]
             assert key not in pq
         _check_heap_invariant(pq)
         _check_index(pq)
 
 
 def test_topvalue1():
-    pq = maxpq()
+    pq = pqdict.maxpq()
     pq['a'] = 10
     pq['b'] = 20
     pq['c'] = 5
 
     assert pq.topvalue() == 20
 
     pq.pop()
@@ -491,34 +501,62 @@
 
 
 def test_topvalue2():
     rnd = random.Random(0)
 
     n = 1000
     low, high = 0, 1000000
-
     vals = []
-
-    pq = minpq()
+    pq = pqdict.minpq()
 
     for i in range(n):
         v = rnd.randint(low, high)
-
         pq[i] = v
         vals.append(v)
 
     popped_values = []
-
     while pq:
         popped_values.append(pq.topvalue())
         pq.pop()
 
     assert sorted(vals) == popped_values
 
 
+def test_popvalue1():
+    pq = pqdict.maxpq()
+    pq['a'] = 10
+    pq['b'] = 20
+    pq['c'] = 5
+    assert pq.popvalue() == 20
+    assert pq.popvalue() == 10
+    assert pq.popvalue() == 5
+    assert pq.popvalue(-1) == -1
+    assert pq.popvalue(default=-10) == -10
+
+
+def test_popvalue2():
+    rnd = random.Random(0)
+
+    n = 1000
+    low, high = 0, 1000000
+    vals = []
+    pq = pqdict.minpq()
+
+    for i in range(n):
+        v = rnd.randint(low, high)
+        pq[i] = v
+        vals.append(v)
+
+    popped_values = []
+    while pq:
+        popped_values.append(pq.popvalue())
+
+    assert sorted(vals) == popped_values
+
+
 def test_edgecases():
     keys = ["A", "B", "C", "D", "E", "F", "G"]
     values = [1, 1, 1, 1, 1, 1, 1]
     pq = pqdict(zip(keys, values))
     pq["B"] = 2
     _check_heap_invariant(pq)
     pq = pqdict(zip(keys, values))
@@ -544,23 +582,26 @@
     pq["b"] = dt + timedelta(days=5)
     pq["c"] = dt + timedelta(seconds=5)
     assert list(pq.popkeys()) == ["a", "c", "b"]
 
 
 def test_repair():
     mutable_value = [3]
-    pq = minpq(A=[1], B=[2], C=mutable_value)
+    pq = pqdict.minpq(A=[1], B=[2], C=mutable_value)
     assert pq[pq.top()] == [1]
     mutable_value[0] = 0
     assert pq[pq.top()] == [1]
     pq.heapify("C")
     assert pq[pq.top()] == [0]
 
 
-# The next test was originally in class TestModuleFunctions
+########################
+# Module-level functions
+########################
+
 def test_nbest():
     top3 = nlargest(3, dict(sample_items))
     assert list(top3) == ["F", "E", "B"]
     bot3 = nsmallest(3, dict(sample_items))
     assert list(bot3) == ["G", "D", "A"]
```

