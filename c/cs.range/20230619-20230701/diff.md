# Comparing `tmp/cs.range-20230619.tar.gz` & `tmp/cs.range-20230701.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.range-20230619.tar", last modified: Mon Jun 19 03:48:01 2023, max compression
+gzip compressed data, was "cs.range-20230701.tar", last modified: Sat Jul  1 02:30:54 2023, max compression
```

## Comparing `cs.range-20230619.tar` & `cs.range-20230701.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-19 03:48:01.028716 cs.range-20230619/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-06-19 03:47:45.000000 cs.range-20230619/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     2875 2023-06-19 03:48:01.028853 cs.range-20230619/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)     6506 2023-06-19 03:47:46.000000 cs.range-20230619/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-19 03:48:01.023417 cs.range-20230619/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-19 03:48:01.023842 cs.range-20230619/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-19 03:48:01.026347 cs.range-20230619/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    18190 2023-06-19 03:46:43.000000 cs.range-20230619/lib/python/cs/range.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-19 03:48:01.028418 cs.range-20230619/lib/python/cs.range.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     2875 2023-06-19 03:48:01.000000 cs.range-20230619/lib/python/cs.range.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      292 2023-06-19 03:48:01.000000 cs.range-20230619/lib/python/cs.range.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-06-19 03:48:01.000000 cs.range-20230619/lib/python/cs.range.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)       39 2023-06-19 03:48:01.000000 cs.range-20230619/lib/python/cs.range.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-06-19 03:48:01.000000 cs.range-20230619/lib/python/cs.range.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)     3069 2023-06-19 03:47:52.000000 cs.range-20230619/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)      937 2023-06-19 03:48:01.029580 cs.range-20230619/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-06-19 03:47:46.000000 cs.range-20230619/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-01 02:30:54.785742 cs.range-20230701/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-07-01 02:30:36.000000 cs.range-20230701/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)     2819 2023-07-01 02:30:54.785858 cs.range-20230701/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)     6450 2023-07-01 02:30:38.000000 cs.range-20230701/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-01 02:30:54.781288 cs.range-20230701/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-01 02:30:54.781634 cs.range-20230701/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-01 02:30:54.783691 cs.range-20230701/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    18206 2023-07-01 02:30:24.000000 cs.range-20230701/lib/python/cs/range.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-07-01 02:30:54.785472 cs.range-20230701/lib/python/cs.range.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)     2819 2023-07-01 02:30:54.000000 cs.range-20230701/lib/python/cs.range.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      292 2023-07-01 02:30:54.000000 cs.range-20230701/lib/python/cs.range.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-07-01 02:30:54.000000 cs.range-20230701/lib/python/cs.range.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)       39 2023-07-01 02:30:54.000000 cs.range-20230701/lib/python/cs.range.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-07-01 02:30:54.000000 cs.range-20230701/lib/python/cs.range.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)     3013 2023-07-01 02:30:44.000000 cs.range-20230701/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)      937 2023-07-01 02:30:54.786441 cs.range-20230701/setup.cfg
+-rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-07-01 02:30:38.000000 cs.range-20230701/setup.py
```

### Comparing `cs.range-20230619/PKG-INFO` & `cs.range-20230701/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.range
-Version: 20230619
+Version: 20230701
 Summary: a Range class implementing compact integer ranges with a set-like API, and associated functions
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
@@ -17,17 +17,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 A Range is an object resembling a set but optimised for contiguous
 ranges of int members.
 
-*Latest release 20230619*:
-* Span: sanity check .start and .end.
-* Range.issubset: efficient comparison with another Range, also .issuperset.
+*Latest release 20230701*:
+Assorted bugfixes.
 
 ## Function `overlap(span1, span2)`
 
 Return a list `[start,end]` denoting the overlap of two spans.
 
 Example:
 
@@ -68,14 +67,17 @@
     >>> list(spans([1,2,3,7,8,11,5]))
     [1:4, 7:9, 11:12, 5:6]
 
 # Release Log
 
 
 
+*Release 20230701*:
+Assorted bugfixes.
+
 *Release 20230619*:
 * Span: sanity check .start and .end.
 * Range.issubset: efficient comparison with another Range, also .issuperset.
 
 *Release 20230518*:
 Span,Range: new as_list() methods.
```

### Comparing `cs.range-20230619/README.md` & `cs.range-20230701/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 A Range is an object resembling a set but optimised for contiguous
 ranges of int members.
 
-*Latest release 20230619*:
-* Span: sanity check .start and .end.
-* Range.issubset: efficient comparison with another Range, also .issuperset.
+*Latest release 20230701*:
+Assorted bugfixes.
 
 ## Function `overlap(span1, span2)`
 
 Return a list `[start,end]` denoting the overlap of two spans.
 
 Example:
 
@@ -199,14 +198,17 @@
     >>> list(spans([1,2,3,7,8,11,5]))
     [1:4, 7:9, 11:12, 5:6]
 
 # Release Log
 
 
 
+*Release 20230701*:
+Assorted bugfixes.
+
 *Release 20230619*:
 * Span: sanity check .start and .end.
 * Range.issubset: efficient comparison with another Range, also .issuperset.
 
 *Release 20230518*:
 Span,Range: new as_list() methods.
```

### Comparing `cs.range-20230619/lib/python/cs/range.py` & `cs.range-20230701/lib/python/cs/range.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from bisect import bisect_left
 from collections import namedtuple
 import sys
 
 from cs.logutils import ifdebug
 from cs.seq import first
 
-__version__ = '20230619'
+__version__ = '20230701'
 
 DISTINFO = {
     'description':
     "a Range class implementing compact integer ranges with a set-like API,"
     " and associated functions",
     'keywords': ["python2", "python3"],
     'classifiers': [
@@ -58,16 +58,16 @@
   try:
     item_spans = items.spans
   except AttributeError:
     # fall through to span locator below
     pass
   else:
     # trust the .spans() method
-    for span in item_spans:
-      yield Span(*span)
+    for span in item_spans():
+      yield span
     return
 
   # otherwise compute by examination
   prev = None
   for i in items:
     if prev is None:
       prev = [i, i + 1]
@@ -173,16 +173,15 @@
     ''' Clear the `Range`: remove all elements.
     '''
     self._spans = []
 
   def spans(self):
     ''' Return an iterable of `Spans` covering the `Range`.
     '''
-    for span in self._spans:
-      yield Span(*span)
+    return list(self._spans)
 
   @property
   def span0(self):
     ''' Return the first `Span`; raises `IndexError` if there are no spans.
     '''
     return first(self.spans())
 
@@ -506,37 +505,37 @@
   def add(self, start, end=None):
     ''' Like `set.add` but with an extended signature.
     '''
     if end is not None:
       self.add_span(start, end)
     elif isinstance(start, Range):
       for span in start.spans():
-        self.add_span(*span)
+        self.add_span(span.start, span.end)
     else:
       self.add_span(start, start + 1)
 
   def discard(self, start, end=None):
     ''' Like `set.discard` but with an extended signature.
     '''
     if end is not None:
       self.discard_span(start, end)
     elif isinstance(start, Range):
       for span in start.spans():
-        self.discard_span(*span)
+        self.discard_span(span.start, span.end)
     else:
       self.discard_span(start, start + 1)
 
   def remove(self, start, end=None):
     ''' Like `set.remove` but with an extended signature.
     '''
     if end is not None:
       self.discard_span(start, end, remove_mode=True)
     elif isinstance(start, Range):
       for span in start.spans():
-        self.discard_span(*span, remove_mode=True)
+        self.discard_span(span.start, span.end, remove_mode=True)
     else:
       self.discard_span(start, start + 1, remove_mode=True)
 
   def update(self, iterable):
     ''' Update the `Range` to include the values from `iterable`.
     '''
     start = None
```

### Comparing `cs.range-20230619/lib/python/cs.range.egg-info/PKG-INFO` & `cs.range-20230701/lib/python/cs.range.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.range
-Version: 20230619
+Version: 20230701
 Summary: a Range class implementing compact integer ranges with a set-like API, and associated functions
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
@@ -17,17 +17,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 A Range is an object resembling a set but optimised for contiguous
 ranges of int members.
 
-*Latest release 20230619*:
-* Span: sanity check .start and .end.
-* Range.issubset: efficient comparison with another Range, also .issuperset.
+*Latest release 20230701*:
+Assorted bugfixes.
 
 ## Function `overlap(span1, span2)`
 
 Return a list `[start,end]` denoting the overlap of two spans.
 
 Example:
 
@@ -68,14 +67,17 @@
     >>> list(spans([1,2,3,7,8,11,5]))
     [1:4, 7:9, 11:12, 5:6]
 
 # Release Log
 
 
 
+*Release 20230701*:
+Assorted bugfixes.
+
 *Release 20230619*:
 * Span: sanity check .start and .end.
 * Range.issubset: efficient comparison with another Range, also .issuperset.
 
 *Release 20230518*:
 Span,Range: new as_list() methods.
```

### Comparing `cs.range-20230619/pyproject.toml` & `cs.range-20230701/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -18,30 +18,29 @@
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20230619"
+version = "20230701"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 A Range is an object resembling a set but optimised for contiguous
 ranges of int members.
 
-*Latest release 20230619*:
-* Span: sanity check .start and .end.
-* Range.issubset: efficient comparison with another Range, also .issuperset.
+*Latest release 20230701*:
+Assorted bugfixes.
 
 ## Function `overlap(span1, span2)`
 
 Return a list `[start,end]` denoting the overlap of two spans.
 
 Example:
 
@@ -82,14 +81,17 @@
     >>> list(spans([1,2,3,7,8,11,5]))
     [1:4, 7:9, 11:12, 5:6]
 
 # Release Log
 
 
 
+*Release 20230701*:
+Assorted bugfixes.
+
 *Release 20230619*:
 * Span: sanity check .start and .end.
 * Range.issubset: efficient comparison with another Range, also .issuperset.
 
 *Release 20230518*:
 Span,Range: new as_list() methods.
```

### Comparing `cs.range-20230619/setup.cfg` & `cs.range-20230701/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cs.range
-version = 20230619
+version = 20230701
 author = Cameron Simpson
 author_email = cs@cskk.id.au
 license = GNU General Public License v3 or later (GPLv3+)
 description = a Range class implementing compact integer ranges with a set-like API, and associated functions
 keywords = python2, python3
 url = https://bitbucket.org/cameron_simpson/css/commits/all
 classifiers =
```

