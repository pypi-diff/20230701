# Comparing `tmp/cdict-1.0.0.tar.gz` & `tmp/cdict-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdict-1.0.0.tar", last modified: Thu Jun  8 23:50:25 2023, max compression
+gzip compressed data, was "cdict-1.0.1.tar", last modified: Sat Jul  1 06:35:02 2023, max compression
```

## Comparing `cdict-1.0.0.tar` & `cdict-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jeffwu     (503) staff       (20)        0 2023-06-08 23:50:25.678567 cdict-1.0.0/
--rw-r--r--   0 jeffwu     (503) staff       (20)       42 2022-05-24 14:35:55.000000 cdict-1.0.0/.gitignore
--rw-r--r--   0 jeffwu     (503) staff       (20)     1080 2022-05-24 14:35:55.000000 cdict-1.0.0/LICENSE
--rw-r--r--   0 jeffwu     (503) staff       (20)      199 2023-06-08 23:50:25.678171 cdict-1.0.0/PKG-INFO
--rw-r--r--   0 jeffwu     (503) staff       (20)     2469 2023-06-08 23:45:51.000000 cdict-1.0.0/README.md
-drwxr-xr-x   0 jeffwu     (503) staff       (20)        0 2023-06-08 23:50:25.652008 cdict-1.0.0/cdict/
--rw-r--r--   0 jeffwu     (503) staff       (20)       29 2023-02-07 17:31:36.000000 cdict-1.0.0/cdict/__init__.py
--rw-r--r--   0 jeffwu     (503) staff       (20)     4078 2023-06-08 23:39:41.000000 cdict-1.0.0/cdict/main.py
-drwxr-xr-x   0 jeffwu     (503) staff       (20)        0 2023-06-08 23:50:25.676838 cdict-1.0.0/cdict.egg-info/
--rw-r--r--   0 jeffwu     (503) staff       (20)      199 2023-06-08 23:50:25.000000 cdict-1.0.0/cdict.egg-info/PKG-INFO
--rw-r--r--   0 jeffwu     (503) staff       (20)      204 2023-06-08 23:50:25.000000 cdict-1.0.0/cdict.egg-info/SOURCES.txt
--rw-r--r--   0 jeffwu     (503) staff       (20)        1 2023-06-08 23:50:25.000000 cdict-1.0.0/cdict.egg-info/dependency_links.txt
--rw-r--r--   0 jeffwu     (503) staff       (20)        6 2023-06-08 23:50:25.000000 cdict-1.0.0/cdict.egg-info/top_level.txt
--rw-r--r--   0 jeffwu     (503) staff       (20)       38 2023-06-08 23:50:25.678630 cdict-1.0.0/setup.cfg
--rw-r--r--   0 jeffwu     (503) staff       (20)      282 2023-06-08 23:47:51.000000 cdict-1.0.0/setup.py
-drwxr-xr-x   0 jeffwu     (503) staff       (20)        0 2023-06-08 23:50:25.677534 cdict-1.0.0/tests/
--rw-r--r--   0 jeffwu     (503) staff       (20)     4674 2023-06-08 23:44:41.000000 cdict-1.0.0/tests/test_main.py
+drwxr-xr-x   0 jeffwu     (503) staff       (20)        0 2023-07-01 06:35:02.570132 cdict-1.0.1/
+-rw-r--r--   0 jeffwu     (503) staff       (20)       42 2022-05-24 14:35:55.000000 cdict-1.0.1/.gitignore
+-rw-r--r--   0 jeffwu     (503) staff       (20)     1080 2022-05-24 14:35:55.000000 cdict-1.0.1/LICENSE
+-rw-r--r--   0 jeffwu     (503) staff       (20)      199 2023-07-01 06:35:02.569545 cdict-1.0.1/PKG-INFO
+-rw-r--r--   0 jeffwu     (503) staff       (20)     2599 2023-06-09 16:03:29.000000 cdict-1.0.1/README.md
+drwxr-xr-x   0 jeffwu     (503) staff       (20)        0 2023-07-01 06:35:02.546092 cdict-1.0.1/cdict/
+-rw-r--r--   0 jeffwu     (503) staff       (20)       29 2023-02-07 17:31:36.000000 cdict-1.0.1/cdict/__init__.py
+-rw-r--r--   0 jeffwu     (503) staff       (20)     4176 2023-07-01 06:26:23.000000 cdict-1.0.1/cdict/main.py
+drwxr-xr-x   0 jeffwu     (503) staff       (20)        0 2023-07-01 06:35:02.560096 cdict-1.0.1/cdict.egg-info/
+-rw-r--r--   0 jeffwu     (503) staff       (20)      199 2023-07-01 06:35:01.000000 cdict-1.0.1/cdict.egg-info/PKG-INFO
+-rw-r--r--   0 jeffwu     (503) staff       (20)      204 2023-07-01 06:35:01.000000 cdict-1.0.1/cdict.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffwu     (503) staff       (20)        1 2023-07-01 06:35:01.000000 cdict-1.0.1/cdict.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffwu     (503) staff       (20)        6 2023-07-01 06:35:01.000000 cdict-1.0.1/cdict.egg-info/top_level.txt
+-rw-r--r--   0 jeffwu     (503) staff       (20)       38 2023-07-01 06:35:02.570216 cdict-1.0.1/setup.cfg
+-rw-r--r--   0 jeffwu     (503) staff       (20)      282 2023-07-01 06:34:54.000000 cdict-1.0.1/setup.py
+drwxr-xr-x   0 jeffwu     (503) staff       (20)        0 2023-07-01 06:35:02.568448 cdict-1.0.1/tests/
+-rw-r--r--   0 jeffwu     (503) staff       (20)     5070 2023-06-09 16:03:25.000000 cdict-1.0.1/tests/test_main.py
```

### Comparing `cdict-1.0.0/LICENSE` & `cdict-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdict-1.0.0/README.md` & `cdict-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 `pip install cdict`
 
 ## Usage
 
 It's most easily understood by example!
 
 ```python
+import pytest
 from cdict import C
 
 # create very simple values
 # cdicts always represent a list of dictionaries
 a1 = C.dict(a=1, aa=1)
 a2 = C.dict(a=2, aa=4)
 assert list(a1) == [dict(a=1, aa=1)]
@@ -34,62 +35,65 @@
 assert list(sweep_a * sweep_b) == [
     dict(a=1, aa=1, b=1),
     dict(a=1, aa=1, b=2),
     dict(a=2, aa=4, b=1),
     dict(a=2, aa=4, b=2),
 ]
 
-# conflicting keys errors by default
-with pytest.raises(ValueError):
-    list(b1 * b2)
-
-# implementing a cdict_combine lets you override that behavior
-class summing_number(int):
-    def cdict_combine(self, other):
-        return summing_number(self + other)
-b1 = C.dict(b=1)
-b2 = C.dict(b=2)
-asserrt list(b1 * b2) == [
-    dict(b=3)
+# you can also nest
+nested_sweep = C.dict(nested_a=sweep_a, nested_b=sweep_b)
+assert list(nested_sweep) == [
+    dict(nested_a=dict(a=1, aa=1), nested_b=dict(b=1)),
+    dict(nested_a=dict(a=1, aa=1), nested_b=dict(b=2)),
+    dict(nested_a=dict(a=2, aa=4), nested_b=dict(b=1)),
+    dict(nested_a=dict(a=2, aa=4), nested_b=dict(b=2)),
 ]
 
-# also some convenience ways to union
+# a more convenient way to union
 sweep_concise = C.dict(a=C.list(1, 2), b=C.list(1, 2))
 assert list(sweep_concise) == [
     dict(a=1, b=1),
     dict(a=1, b=2),
     dict(a=2, b=1),
     dict(a=2, b=2),
 ]
 
-# nesting as well
-nested_sweep = C.dict(nested_a=sweep_a, nested_b=sweep_b)
-assert list(nested_sweep) == [
-    dict(nested_a=dict(a=1, aa=1), nested_b=dict(b=1)),
-    dict(nested_a=dict(a=1, aa=1), nested_b=dict(b=2)),
-    dict(nested_a=dict(a=2, aa=4), nested_b=dict(b=1)),
-    dict(nested_a=dict(a=2, aa=4), nested_b=dict(b=2)),
-]
+# and transform
+def square_a(x):
+    x['aa'] = x['a']**2
+    return x
 
-# zipping of equal length things
-nested_sweep = sweep_a | sweep_b
-assert list(nested_sweep) == [
+sweep_concise = sweep_concise.map(square_a)
+assert list(sweep_concise) == [
     dict(a=1, aa=1, b=1),
+    dict(a=1, aa=1, b=2),
+    dict(a=2, aa=4, b=1),
     dict(a=2, aa=4, b=2),
 ]
 
-# transform dicts on the fly
-a3 = C.dict(a=3)
+# conflicting keys errors by default
+with pytest.raises(ValueError):
+    list(b1 * b2)
 
-def square_a(x):
-    x['aa'] = x['a']**2
-    return x
+# implementing a cdict_combine lets you override that behavior
+class summing_number(int):
+    def cdict_combine(self, other):
+        return summing_number(self + other)
+b1 = C.dict(b=summing_number(1))
+b2 = C.dict(b=summing_number(2))
+assert list(b1 * b2) == [
+    dict(b=3)
+]
 
-a3 = a3.map(square_a)
-assert list(a3) == [dict(a=3, aa=9)]
+# zipping of equal length things
+diag_sweep = sweep_a | sweep_b
+assert list(diag_sweep) == [
+    dict(a=1, aa=1, b=1),
+    dict(a=2, aa=4, b=2),
+]
 ```
 
 ## Properties
 
 - `*` `+` and `|` are associative
 - `*` is left-distributive over `+`, that is `a * c + b * c = (a + b) * c`.  It is right-distributive if ignoring order of the resulting items.
 - `+`  is commutative if you don’t care about order of the resulting items
```

### Comparing `cdict-1.0.0/cdict/main.py` & `cdict-1.0.1/cdict/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,18 @@
         return _cdict_sum([dict(**kwargs)])
 
     @classmethod
     def list(cls, *args: Any) -> cdict:
         return cls.iter(list(args))
 
     @classmethod
+    def sum(cls, args: Iterable) -> cdict:
+        return sum(args, cls.list())
+
+    @classmethod
     def iter(cls, it: Any) -> cdict:
         return _cdict_sum(it)
 
     def apply(self, fn: Callable[[Any], Any]) -> cdict:
         return _cdict_apply(fn, self)
 
     def map(self, fn: Callable[[Any], Any]) -> cdict:
```

### Comparing `cdict-1.0.0/tests/test_main.py` & `cdict-1.0.1/tests/test_main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import time
 import pytest
+import re
+import os
 
 from cdict import C
 
 def assert_dicts(c, expected):
     print(c)
     dicts = list(iter(c))
     assert len(dicts) == len(expected), f"Expected equal lengths, got {len(expected)} instead of {len(dicts)}"
@@ -151,13 +153,26 @@
 
 def test_commutative_mult():
     a0 = C.dict(a=C.list(1,2))
     a1 = C.dict(b=C.list(3,4))
     assert_equivalent_sets(a0 * a1, a1 * a0)
 
 
+def test_readme_code():
+    readme_file = os.path.join(os.path.dirname(__file__), '..', 'README.md')
+    with open(readme_file) as f:
+        text = f.read()
+    m = re.search('```(.+?)```', text, flags=re.DOTALL)
+    assert m
+    code = m.group(1)
+    assert code.startswith('python')
+    code = code[6:].strip()
+    exec(code, globals(), globals())
+
+
 if __name__ == "__main__":
     test_simple()
     test_overwriting()
     test_or()
     test_distributive()
     test_commutative_mult()
+    test_readme_code()
```

