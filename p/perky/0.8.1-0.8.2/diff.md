# Comparing `tmp/perky-0.8.1.tar.gz` & `tmp/perky-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perky-0.8.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "perky-0.8.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `perky-0.8.1.tar` & `perky-0.8.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       39 2023-06-26 00:34:27.020388 perky-0.8.1/.gitignore
--rw-r--r--   0        0        0     1089 2023-06-26 00:34:27.028388 perky-0.8.1/LICENSE
--rw-r--r--   0        0        0    13977 2023-06-26 11:20:38.108383 perky-0.8.1/README.md
--rwxr-xr-x   0        0        0    13785 2023-06-26 11:19:51.155981 perky-0.8.1/perky/__init__.py
--rw-r--r--   0        0        0    13071 2023-06-26 00:34:27.028388 perky-0.8.1/perky/tokenize.py
--rw-r--r--   0        0        0     7146 2023-06-26 00:34:27.028388 perky-0.8.1/perky/transform.py
--rw-r--r--   0        0        0     4422 2023-06-26 00:34:27.028388 perky-0.8.1/perky/utility.py
--rw-r--r--   0        0        0      437 2018-12-04 18:40:09.175851 perky-0.8.1/pyproject.toml
--rw-r--r--   0        0        0        0 2018-12-04 18:40:09.175851 perky-0.8.1/tests/__init__.py
--rw-r--r--   0        0        0        3 2020-08-28 04:00:24.788890 perky-0.8.1/tests/include_dict/included.pky
--rw-r--r--   0        0        0       33 2020-08-28 04:00:24.788890 perky-0.8.1/tests/include_dict/main.pky
--rw-r--r--   0        0        0        1 2020-08-28 04:00:24.788890 perky-0.8.1/tests/include_list/included.pky
--rw-r--r--   0        0        0       27 2020-08-28 04:00:24.788890 perky-0.8.1/tests/include_list/main.pky
--rw-r--r--   0        0        0      106 2020-08-28 04:00:24.788890 perky-0.8.1/tests/include_nested/included.pky
--rw-r--r--   0        0        0      190 2020-08-28 04:00:24.788890 perky-0.8.1/tests/include_nested/main.pky
--rw-r--r--   0        0        0       30 2020-08-28 04:00:24.788890 perky-0.8.1/tests/include_path/dir1/main.pky
--rw-r--r--   0        0        0        3 2020-08-28 04:00:24.788890 perky-0.8.1/tests/include_path/dir2/included.pky
--rw-r--r--   0        0        0      766 2023-06-26 00:34:27.028388 perky-0.8.1/tests/perkytestlib.py
--rw-r--r--   0        0        0      657 2023-06-26 00:34:27.028388 perky-0.8.1/tests/test_all.py
--rw-r--r--   0        0        0      214 2018-12-04 18:40:09.175851 perky-0.8.1/tests/test_input.txt
--rw-r--r--   0        0        0    13636 2023-06-26 11:19:25.427761 perky-0.8.1/tests/test_perky.py
--rw-r--r--   0        0        0     8086 2023-06-26 00:34:27.028388 perky-0.8.1/tests/test_tokenize.py
--rw-r--r--   0        0        0     1263 2023-06-26 00:34:27.028388 perky-0.8.1/tests/test_transform.py
--rw-r--r--   0        0        0     1773 2023-06-26 00:34:27.028388 perky-0.8.1/tests/test_utility.py
--rw-r--r--   0        0        0    14413 1970-01-01 00:00:00.000000 perky-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0       39 2023-07-01 02:47:29.152522 perky-0.8.2/.gitignore
+-rw-r--r--   0        0        0     1089 2023-07-01 02:47:29.152522 perky-0.8.2/LICENSE
+-rw-r--r--   0        0        0    15157 2023-07-01 02:49:14.953392 perky-0.8.2/README.md
+-rwxr-xr-x   0        0        0    13692 2023-07-01 02:49:14.953392 perky-0.8.2/perky/__init__.py
+-rw-r--r--   0        0        0    13071 2023-07-01 02:47:29.152522 perky-0.8.2/perky/tokenize.py
+-rw-r--r--   0        0        0     7146 2023-07-01 02:47:29.152522 perky-0.8.2/perky/transform.py
+-rw-r--r--   0        0        0     4422 2023-07-01 02:47:29.152522 perky-0.8.2/perky/utility.py
+-rw-r--r--   0        0        0      437 2023-07-01 02:47:29.152522 perky-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-01 02:47:29.156522 perky-0.8.2/tests/__init__.py
+-rw-r--r--   0        0        0        3 2023-07-01 02:47:29.156522 perky-0.8.2/tests/include_dict/included.pky
+-rw-r--r--   0        0        0       33 2023-07-01 02:47:29.156522 perky-0.8.2/tests/include_dict/main.pky
+-rw-r--r--   0        0        0        1 2023-07-01 02:47:29.156522 perky-0.8.2/tests/include_list/included.pky
+-rw-r--r--   0        0        0       27 2023-07-01 02:47:29.156522 perky-0.8.2/tests/include_list/main.pky
+-rw-r--r--   0        0        0      106 2023-07-01 02:47:29.156522 perky-0.8.2/tests/include_nested/included.pky
+-rw-r--r--   0        0        0      190 2023-07-01 02:47:29.156522 perky-0.8.2/tests/include_nested/main.pky
+-rw-r--r--   0        0        0       30 2023-07-01 02:47:29.156522 perky-0.8.2/tests/include_path/dir1/main.pky
+-rw-r--r--   0        0        0        3 2023-07-01 02:47:29.156522 perky-0.8.2/tests/include_path/dir2/included.pky
+-rw-r--r--   0        0        0      766 2023-07-01 02:47:29.156522 perky-0.8.2/tests/perkytestlib.py
+-rw-r--r--   0        0        0      669 2023-07-01 02:49:14.953392 perky-0.8.2/tests/test_all.py
+-rw-r--r--   0        0        0      214 2023-07-01 02:47:29.156522 perky-0.8.2/tests/test_input.txt
+-rw-r--r--   0        0        0    13636 2023-07-01 02:47:29.156522 perky-0.8.2/tests/test_perky.py
+-rw-r--r--   0        0        0     8086 2023-07-01 02:47:29.156522 perky-0.8.2/tests/test_tokenize.py
+-rw-r--r--   0        0        0     1263 2023-07-01 02:47:29.156522 perky-0.8.2/tests/test_transform.py
+-rw-r--r--   0        0        0     1773 2023-07-01 02:47:29.156522 perky-0.8.2/tests/test_utility.py
+-rw-r--r--   0        0        0    15593 1970-01-01 00:00:00.000000 perky-0.8.2/PKG-INFO
```

### Comparing `perky-0.8.1/LICENSE` & `perky-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `perky-0.8.1/README.md` & `perky-0.8.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -17,27 +17,27 @@
 * Explicit minimal data type support.  Rather than guess at the types
   of your data, Perky lets you handle the final transformation.
 * Lightweight, simple, and fast.  Perky's implementation is small
   and straightforward.  Ignoring comments and test code, it's about
   1k lines of Python.  Fewer lines means fewer bugs!  (Hopefully!)
 * Flexible and extensible.  Perky permits extending the semantics of
   Perky files through a "pragma" mechanism.
-* Perky supports Python 3.6+, and its supported code passes its
-  unit test suite with 100% coverage.
+* Perky supports Python 3.6+, and passes its unit test suite with
+  100% coverage (excluding the deprecated portions).
 
 #### Perky syntax
 
 Perky configuration files look something like JSON without the
 quoting.  It supports only a surprisingly small set of value
 types:
 
 * strings, including quoted strings and
   "triple-quoted strings" (multi-line strings),
-* "lists" (arrays),
-* and "dicts" (associative arrays).
+* "mappings" (dicts), and
+* "sequences" (lists).
 
 Perky is line-oriented; individual values go on a single
 line.  Container objects use one line per internal value.
 
 You may nest lists and dicts as deeply as memory permits.
 
 Unlike Python itself, leading whitespace is ignored.  You
@@ -127,21 +127,21 @@
 rather than guess and be wrong, Perky keeps things simple:
 just lists, dicts, and strings.  For any other type,
 it's up to you to transform it from a string into the type
 you want, and back again.
 
 Note that Perky doesn't care how or if you transform your
 data.  You can use the strings as-is or transform them
-however you like.  You can transform them by hand
+however you like.  You can transform them by hand,
 or with a third-party data transformation library like
 [Marshmallow.](https://marshmallow.readthedocs.io/)
 
-(Perky used to support an experimental API for transforming
-data yourself.  But this was never fully fleshed-out, and
-there are better versions of that technology out there.
+(Perky used to support an experimental API for automated
+data transformation.  But this was never fully fleshed-out,
+and there are better versions of that technology out there.
 I've deprecated the "transformation" submodule and will
 remove it before 1.0.)
 
 
 ### Pragmas
 
 A *pragma* is a metadata directive for the Perky parser.
@@ -211,43 +211,56 @@
   we don't want to let errors pass silently.
 * Using an undefined pragma.
 * Using one of Perky's special tokens as a pragma argument, like
   `{`, `[`, `'''`, `"""`, `[]`, or `{}`.
 
 ### API
 
-`def loads(s, *, pragmas=None, encoding='utf-8', root=None) -> o`
+#### `def loads(s, *, pragmas=None, root=None) -> o`
 
 Parses a Perky-format string, and returns a container filled
 with the values parsed from that string.
 
-If `root` is not `None`,
-it should be a container
+If `root` is `None`, `loads` behaves as if you passed in an
+empty `dict`.
 
-If `root` is `None`, returns a new dict.
+If `root` is not `None`, it should be a container, either
+a mutable mapping (`dict`) or a mutable sequence (`list`).
+This affects how the data is parsed; if `root` is a
+mutable mapping, the top level of the Perky file must be
+a "mapping context" (a series of `name=value` lines);
+if `root` is a mutable sequence, the top level of the Perky
+file is assumed to be a "sequence context"
+(a series of `value` lines).
 
-`def loads(s, *, pragmas=None, encoding='utf-8', root=None) -> o`
+#### `def load(s, *, pragmas=None, encoding='utf-8', root=None) -> o`
 
 Parses a file containing Perky-file-format settings.
 Returns a dict.
 
-`perky.dumps(d) -> s`
+`encoding` specifies the encoding used to decode the
+data read from the file.
+
+#### `perky.dumps(d) -> s`
 
 Converts a dictionary to a Perky-file-format string.
 Keys in the dictionary must all be strings.  Values
 that are not dicts, lists, or strings will be converted
 to strings using str.
 Returns a string.
 
-`perky.dump(filename, d, *, pragmas=None, encoding="utf-8")`
+#### `perky.dump(filename, d, *, pragmas=None, encoding="utf-8")`
 
 Converts a dictionary to a Perky-file-format string
 using `perky.dump`, then writes it to *filename*.
 
-`perky.pragma_include(include_path=(".",))`
+`encoding` specifies the encoding used to encode the
+data written to the file.
+
+#### `perky.pragma_include(include_path=(".",), *, encoding='utf-8')`
 
 This function generates a pragma handler that adds "include"
 functionality.  "Including" means lexically inserting one Perky
 file inside another, contextually at the spot where the pragma
 exists.
 
 For example:
@@ -272,21 +285,24 @@
     include_dirs = [appdirs.user_data_dir(myapp_name)]
     config_dirs = [appdirs.user_config_dir(myapp_name)]
     pragmas = {
         'include': perky.pragma_include(include_dirs),
         'config': perky.pragma_include(config_dirs),
     }
 
+`encoding` specifies the encoding used to decode the
+data read in from the included files.
+
 Notes:
 
 * The pragma handler is context-sensitive; the included
 file will be included as if it was copied-and-pasted replacing
 the pragma line.  Among other things, this means that if the pragma
-is invoked inside a list context, the included file must *start*
-in a list context.
+is invoked inside a sequence context, the included file must *start*
+in a sequence context.
 
 * When loading the file, the pragma handler will pass in the
 current pragma handlers into `perky.load()`.  Among other things,
 this allows for recursive includes.
 
 * When including inside a dict context, you're explicitly permitted
 to re-define existing keys if they were previously defined in
@@ -296,16 +312,16 @@
 current directory (`"."`).  If you override the default
 and pass in your own include path, the pragma handler
 won't search the current directory unless you add `"."`
 to the include path yourself.
 
 #### Deprecated API
 
-Perky currently has a "transformation" submodule.
-The idea is, you'd load a Perky file,
+Perky has a "transformation" submodule.
+The idea is, you load a Perky file,
 then run `perky.transform` on that dictionary to
 convert the strings into native values.
 
 These functions are no longer maintained or supported,
 and will be removed before 1.0.
 Why?  This part of Perky was always
 an experiment... and the experiment never really paid
@@ -319,17 +335,17 @@
 For posterity's sakes, here's documentation of the
 now-deprecated API.
 
 `perky.map(d, fn) -> o`
 
 Iterates over a dictionary.  Returns a new dictionary where,
 for every *value*:
-  * if it is a dict, replace with a new dict.
-  * if it is a list, replace with a new list.
-  * if it is neither a dict nor a list, replace with
+  * if it's a dict, replace with a new dict.
+  * if it's a list, replace with a new list.
+  * if it's neither a dict nor a list, replace with
     `fn(value)`.
 
 The function passed in is called a *conversion function*.
 
 `perky.transform(d, schema, default=None) -> o`
 
 Recursively transforms a Perky dict into some other
@@ -364,14 +380,29 @@
 
 ### TODO
 
 * Backslash quoting currently does "whatever your version of Python does".  Perhaps this should be explicit, and parsed by Perky itself?
 
 ### Changelog
 
+**0.8.2** *2023/06/30*
+
+* Minor API changes:
+
+  - You can now pass an `encoding` keyword argument
+    into `pragma_include`.  This is now the only way
+    to specify the encoding used to decode files
+    loaded from disk by `pragma_include`.
+  - Removed the (undocumented) `encoding` attribute
+    of the `perky.Parser` object.
+  - Removed the `encoding` parameter for `loads`.
+  - The `encoding` parameter for `load` is now only
+    used by `load` itself when loading the top-level
+    Perky file.
+
 **0.8.1** *2023/06/26*
 
 * Whoops!  A major regression: I inadveretently changed the default
   conversion of non-string values from `str` to `repr`.  Bad move!
   `str` is much better.  Added a test so I don't do this again.
 
 **0.8** *2023/06/25*
```

### Comparing `perky-0.8.1/perky/__init__.py` & `perky-0.8.2/perky/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
 TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE
 OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
 
-__version__ = "0.8.1"
+__version__ = "0.8.2"
 
 import ast
 from collections.abc import MutableMapping, MutableSequence, Sequence
 import os.path
 from os.path import isfile, join, normpath
 import re
 import shlex
@@ -145,20 +145,19 @@
 def export(fn):
     __all__.append(fn.__name__)
     return fn
 
 
 class Parser:
 
-    def __init__(self, s, *, pragmas=None, encoding='utf-8', root=None):
+    def __init__(self, s, *, pragmas=None, root=None):
         if not isinstance(s, str):
             raise TypeError('s must be str, not {type(s)}')
         self.lt = LineTokenizer(s)
         self.pragmas = pragmas or {}
-        self.encoding = encoding
         self.root = root if root is not None else {}
         self.breadcrumbs = []
 
     def _parse_pragma(self, line):
         original_line = line
         line = line.strip()
         assert line[0] == '='
@@ -400,56 +399,56 @@
         if value == value.strip() and "".join(value.split()).isalnum():
             self.newline(value)
             return
         return self.serialize_quoted_string(value)
 
 
 @export
-def loads(s, *, pragmas=None, encoding='utf-8', root=None):
-    p = Parser(s, pragmas=pragmas, encoding=encoding, root=root)
+def loads(s, *, pragmas=None, root=None):
+    p = Parser(s, pragmas=pragmas, root=root)
     d = p.parse()
     return d
 
 @export
 def dumps(d):
     s = Serializer()
     s.serialize(d)
     return s.dumps()
 
 
 @export
 def load(filename, *, pragmas=None, encoding="utf-8", root=None):
     with open(filename, "rt", encoding=encoding) as f:
-        return loads(f.read(), pragmas=pragmas, encoding=encoding, root=root)
+        return loads(f.read(), pragmas=pragmas, root=root)
 
 @export
 def dump(filename, d, *, encoding="utf-8"):
     s = Serializer()
     s.serialize(d)
     with open(filename, "wt", encoding=encoding) as f:
         f.write(s.dumps())
 
 
 @export
-def pragma_include(include_path=(".",)):
+def pragma_include(include_path=(".",), *, encoding='utf-8'):
     assert isinstance(include_path, Sequence)
     assert not isinstance(include_path, str)
     assert all(isinstance(s, str) for s in include_path)
     include_path = tuple(include_path)
     def pragma_include(parser, filename):
         leaf = parser.breadcrumbs[-1]
         leaf_is_list = isinstance(parser.breadcrumbs[-1], list)
         subroot = [] if leaf_is_list else {}
         for directory in include_path:
             path = normpath(join(directory, filename))
             if isfile(path):
                 break
         else:
             raise FileNotFoundError(filename)
-        load(path, pragmas=parser.pragmas, encoding=parser.encoding, root=subroot)
+        load(path, pragmas=parser.pragmas, encoding=encoding, root=subroot)
         merged = merge_dicts_and_lists(leaf, subroot)
         # print(f"\n\nXXX merge_dicts_and_lists({leaf=}, {subroot=}) -> {merged=}\n\n")
         leaf.clear()
         if isinstance(leaf, list):
             leaf.extend(merged)
         else:
             leaf.update(merged)
```

### Comparing `perky-0.8.1/perky/tokenize.py` & `perky-0.8.2/perky/tokenize.py`

 * *Files identical despite different names*

### Comparing `perky-0.8.1/perky/transform.py` & `perky-0.8.2/perky/transform.py`

 * *Files identical despite different names*

### Comparing `perky-0.8.1/perky/utility.py` & `perky-0.8.2/perky/utility.py`

 * *Files identical despite different names*

### Comparing `perky-0.8.1/tests/perkytestlib.py` & `perky-0.8.2/tests/perkytestlib.py`

 * *Files identical despite different names*

### Comparing `perky-0.8.1/tests/test_all.py` & `perky-0.8.2/tests/test_all.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,13 +16,13 @@
         module = __import__(test_module)
         result = unittest.main(module=module, exit=False)
         modules += 1
         successes += result.result.wasSuccessful()
 
     print()
     if successes == modules:
-        print("Unit tests passed.")
+        print("OK")
     else: # pragma: nocover
-        print("Unit tests failed.")
+        print(f"FAILED (failed modules={modules - successes})")
 
 if __name__ == '__main__':
     run_tests()
```

### Comparing `perky-0.8.1/tests/test_perky.py` & `perky-0.8.2/tests/test_perky.py`

 * *Files identical despite different names*

### Comparing `perky-0.8.1/tests/test_tokenize.py` & `perky-0.8.2/tests/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `perky-0.8.1/tests/test_transform.py` & `perky-0.8.2/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `perky-0.8.1/tests/test_utility.py` & `perky-0.8.2/tests/test_utility.py`

 * *Files identical despite different names*

### Comparing `perky-0.8.1/PKG-INFO` & `perky-0.8.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perky
-Version: 0.8.1
+Version: 0.8.2
 Summary: A simple, Pythonic file format.  Same interface as the
 Home-page: https://github.com/larryhastings/perky/
 Author: Larry Hastings
 Author-email: larry@hastings.org
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
@@ -30,27 +30,27 @@
 * Explicit minimal data type support.  Rather than guess at the types
   of your data, Perky lets you handle the final transformation.
 * Lightweight, simple, and fast.  Perky's implementation is small
   and straightforward.  Ignoring comments and test code, it's about
   1k lines of Python.  Fewer lines means fewer bugs!  (Hopefully!)
 * Flexible and extensible.  Perky permits extending the semantics of
   Perky files through a "pragma" mechanism.
-* Perky supports Python 3.6+, and its supported code passes its
-  unit test suite with 100% coverage.
+* Perky supports Python 3.6+, and passes its unit test suite with
+  100% coverage (excluding the deprecated portions).
 
 #### Perky syntax
 
 Perky configuration files look something like JSON without the
 quoting.  It supports only a surprisingly small set of value
 types:
 
 * strings, including quoted strings and
   "triple-quoted strings" (multi-line strings),
-* "lists" (arrays),
-* and "dicts" (associative arrays).
+* "mappings" (dicts), and
+* "sequences" (lists).
 
 Perky is line-oriented; individual values go on a single
 line.  Container objects use one line per internal value.
 
 You may nest lists and dicts as deeply as memory permits.
 
 Unlike Python itself, leading whitespace is ignored.  You
@@ -140,21 +140,21 @@
 rather than guess and be wrong, Perky keeps things simple:
 just lists, dicts, and strings.  For any other type,
 it's up to you to transform it from a string into the type
 you want, and back again.
 
 Note that Perky doesn't care how or if you transform your
 data.  You can use the strings as-is or transform them
-however you like.  You can transform them by hand
+however you like.  You can transform them by hand,
 or with a third-party data transformation library like
 [Marshmallow.](https://marshmallow.readthedocs.io/)
 
-(Perky used to support an experimental API for transforming
-data yourself.  But this was never fully fleshed-out, and
-there are better versions of that technology out there.
+(Perky used to support an experimental API for automated
+data transformation.  But this was never fully fleshed-out,
+and there are better versions of that technology out there.
 I've deprecated the "transformation" submodule and will
 remove it before 1.0.)
 
 
 ### Pragmas
 
 A *pragma* is a metadata directive for the Perky parser.
@@ -224,43 +224,56 @@
   we don't want to let errors pass silently.
 * Using an undefined pragma.
 * Using one of Perky's special tokens as a pragma argument, like
   `{`, `[`, `'''`, `"""`, `[]`, or `{}`.
 
 ### API
 
-`def loads(s, *, pragmas=None, encoding='utf-8', root=None) -> o`
+#### `def loads(s, *, pragmas=None, root=None) -> o`
 
 Parses a Perky-format string, and returns a container filled
 with the values parsed from that string.
 
-If `root` is not `None`,
-it should be a container
+If `root` is `None`, `loads` behaves as if you passed in an
+empty `dict`.
 
-If `root` is `None`, returns a new dict.
+If `root` is not `None`, it should be a container, either
+a mutable mapping (`dict`) or a mutable sequence (`list`).
+This affects how the data is parsed; if `root` is a
+mutable mapping, the top level of the Perky file must be
+a "mapping context" (a series of `name=value` lines);
+if `root` is a mutable sequence, the top level of the Perky
+file is assumed to be a "sequence context"
+(a series of `value` lines).
 
-`def loads(s, *, pragmas=None, encoding='utf-8', root=None) -> o`
+#### `def load(s, *, pragmas=None, encoding='utf-8', root=None) -> o`
 
 Parses a file containing Perky-file-format settings.
 Returns a dict.
 
-`perky.dumps(d) -> s`
+`encoding` specifies the encoding used to decode the
+data read from the file.
+
+#### `perky.dumps(d) -> s`
 
 Converts a dictionary to a Perky-file-format string.
 Keys in the dictionary must all be strings.  Values
 that are not dicts, lists, or strings will be converted
 to strings using str.
 Returns a string.
 
-`perky.dump(filename, d, *, pragmas=None, encoding="utf-8")`
+#### `perky.dump(filename, d, *, pragmas=None, encoding="utf-8")`
 
 Converts a dictionary to a Perky-file-format string
 using `perky.dump`, then writes it to *filename*.
 
-`perky.pragma_include(include_path=(".",))`
+`encoding` specifies the encoding used to encode the
+data written to the file.
+
+#### `perky.pragma_include(include_path=(".",), *, encoding='utf-8')`
 
 This function generates a pragma handler that adds "include"
 functionality.  "Including" means lexically inserting one Perky
 file inside another, contextually at the spot where the pragma
 exists.
 
 For example:
@@ -285,21 +298,24 @@
     include_dirs = [appdirs.user_data_dir(myapp_name)]
     config_dirs = [appdirs.user_config_dir(myapp_name)]
     pragmas = {
         'include': perky.pragma_include(include_dirs),
         'config': perky.pragma_include(config_dirs),
     }
 
+`encoding` specifies the encoding used to decode the
+data read in from the included files.
+
 Notes:
 
 * The pragma handler is context-sensitive; the included
 file will be included as if it was copied-and-pasted replacing
 the pragma line.  Among other things, this means that if the pragma
-is invoked inside a list context, the included file must *start*
-in a list context.
+is invoked inside a sequence context, the included file must *start*
+in a sequence context.
 
 * When loading the file, the pragma handler will pass in the
 current pragma handlers into `perky.load()`.  Among other things,
 this allows for recursive includes.
 
 * When including inside a dict context, you're explicitly permitted
 to re-define existing keys if they were previously defined in
@@ -309,16 +325,16 @@
 current directory (`"."`).  If you override the default
 and pass in your own include path, the pragma handler
 won't search the current directory unless you add `"."`
 to the include path yourself.
 
 #### Deprecated API
 
-Perky currently has a "transformation" submodule.
-The idea is, you'd load a Perky file,
+Perky has a "transformation" submodule.
+The idea is, you load a Perky file,
 then run `perky.transform` on that dictionary to
 convert the strings into native values.
 
 These functions are no longer maintained or supported,
 and will be removed before 1.0.
 Why?  This part of Perky was always
 an experiment... and the experiment never really paid
@@ -332,17 +348,17 @@
 For posterity's sakes, here's documentation of the
 now-deprecated API.
 
 `perky.map(d, fn) -> o`
 
 Iterates over a dictionary.  Returns a new dictionary where,
 for every *value*:
-  * if it is a dict, replace with a new dict.
-  * if it is a list, replace with a new list.
-  * if it is neither a dict nor a list, replace with
+  * if it's a dict, replace with a new dict.
+  * if it's a list, replace with a new list.
+  * if it's neither a dict nor a list, replace with
     `fn(value)`.
 
 The function passed in is called a *conversion function*.
 
 `perky.transform(d, schema, default=None) -> o`
 
 Recursively transforms a Perky dict into some other
@@ -377,14 +393,29 @@
 
 ### TODO
 
 * Backslash quoting currently does "whatever your version of Python does".  Perhaps this should be explicit, and parsed by Perky itself?
 
 ### Changelog
 
+**0.8.2** *2023/06/30*
+
+* Minor API changes:
+
+  - You can now pass an `encoding` keyword argument
+    into `pragma_include`.  This is now the only way
+    to specify the encoding used to decode files
+    loaded from disk by `pragma_include`.
+  - Removed the (undocumented) `encoding` attribute
+    of the `perky.Parser` object.
+  - Removed the `encoding` parameter for `loads`.
+  - The `encoding` parameter for `load` is now only
+    used by `load` itself when loading the top-level
+    Perky file.
+
 **0.8.1** *2023/06/26*
 
 * Whoops!  A major regression: I inadveretently changed the default
   conversion of non-string values from `str` to `repr`.  Bad move!
   `str` is much better.  Added a test so I don't do this again.
 
 **0.8** *2023/06/25*
```

