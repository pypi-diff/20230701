# Comparing `tmp/setup_cfg_fmt-2.3.0.tar.gz` & `tmp/setup_cfg_fmt-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setup_cfg_fmt-2.3.0.tar", last modified: Thu Jun  1 23:40:41 2023, max compression
+gzip compressed data, was "setup_cfg_fmt-2.4.0.tar", last modified: Sat Jul  1 17:47:56 2023, max compression
```

## Comparing `setup_cfg_fmt-2.3.0.tar` & `setup_cfg_fmt-2.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-01 23:40:41.347571 setup_cfg_fmt-2.3.0/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-06-01 21:59:49.000000 setup_cfg_fmt-2.3.0/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4739 2023-06-01 23:40:41.347571 setup_cfg_fmt-2.3.0/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4121 2023-06-01 23:40:41.000000 setup_cfg_fmt-2.3.0/README.md
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1158 2023-06-01 23:40:41.351571 setup_cfg_fmt-2.3.0/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-06-01 21:59:49.000000 setup_cfg_fmt-2.3.0/setup.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-01 23:40:41.347571 setup_cfg_fmt-2.3.0/setup_cfg_fmt.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4739 2023-06-01 23:40:41.000000 setup_cfg_fmt-2.3.0/setup_cfg_fmt.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      277 2023-06-01 23:40:41.000000 setup_cfg_fmt-2.3.0/setup_cfg_fmt.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-01 23:40:41.000000 setup_cfg_fmt-2.3.0/setup_cfg_fmt.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       53 2023-06-01 23:40:41.000000 setup_cfg_fmt-2.3.0/setup_cfg_fmt.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       25 2023-06-01 23:40:41.000000 setup_cfg_fmt-2.3.0/setup_cfg_fmt.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       14 2023-06-01 23:40:41.000000 setup_cfg_fmt-2.3.0/setup_cfg_fmt.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)    17808 2023-06-01 23:40:38.000000 setup_cfg_fmt-2.3.0/setup_cfg_fmt.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-01 17:47:56.560463 setup_cfg_fmt-2.4.0/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-06-01 21:59:49.000000 setup_cfg_fmt-2.4.0/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4739 2023-07-01 17:47:56.560463 setup_cfg_fmt-2.4.0/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4121 2023-07-01 17:47:56.000000 setup_cfg_fmt-2.4.0/README.md
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1158 2023-07-01 17:47:56.564463 setup_cfg_fmt-2.4.0/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-06-01 21:59:49.000000 setup_cfg_fmt-2.4.0/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-01 17:47:56.560463 setup_cfg_fmt-2.4.0/setup_cfg_fmt.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4739 2023-07-01 17:47:56.000000 setup_cfg_fmt-2.4.0/setup_cfg_fmt.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      277 2023-07-01 17:47:56.000000 setup_cfg_fmt-2.4.0/setup_cfg_fmt.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-07-01 17:47:56.000000 setup_cfg_fmt-2.4.0/setup_cfg_fmt.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       53 2023-07-01 17:47:56.000000 setup_cfg_fmt-2.4.0/setup_cfg_fmt.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       25 2023-07-01 17:47:56.000000 setup_cfg_fmt-2.4.0/setup_cfg_fmt.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       14 2023-07-01 17:47:56.000000 setup_cfg_fmt-2.4.0/setup_cfg_fmt.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    17739 2023-07-01 17:47:56.000000 setup_cfg_fmt-2.4.0/setup_cfg_fmt.py
```

### Comparing `setup_cfg_fmt-2.3.0/LICENSE` & `setup_cfg_fmt-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `setup_cfg_fmt-2.3.0/PKG-INFO` & `setup_cfg_fmt-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: setup_cfg_fmt
-Version: 2.3.0
+Version: 2.4.0
 Summary: apply a consistent format to `setup.cfg` files
 Home-page: https://github.com/asottile/setup-cfg-fmt
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![build status](https://github.com/asottile/setup-cfg-fmt/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/setup-cfg-fmt/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/setup-cfg-fmt/main.svg)](https://results.pre-commit.ci/latest/github/asottile/setup-cfg-fmt/main)
 
 setup-cfg-fmt
@@ -33,15 +33,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/setup-cfg-fmt
-    rev: v2.3.0
+    rev: v2.4.0
     hooks:
     -   id: setup-cfg-fmt
 ```
 
 ## cli
 
 Consult the help for the latest usage:
```

### Comparing `setup_cfg_fmt-2.3.0/README.md` & `setup_cfg_fmt-2.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/setup-cfg-fmt
-    rev: v2.3.0
+    rev: v2.4.0
     hooks:
     -   id: setup-cfg-fmt
 ```
 
 ## cli
 
 Consult the help for the latest usage:
```

### Comparing `setup_cfg_fmt-2.3.0/setup.cfg` & `setup_cfg_fmt-2.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = setup_cfg_fmt
-version = 2.3.0
+version = 2.4.0
 description = apply a consistent format to `setup.cfg` files
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/setup-cfg-fmt
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
@@ -16,15 +16,15 @@
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 
 [options]
 py_modules = setup_cfg_fmt
 install_requires = 
 	identify[license]>=2.4.0
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.entry_points]
 console_scripts = 
 	setup-cfg-fmt=setup_cfg_fmt:main
 
 [bdist_wheel]
 universal = True
```

### Comparing `setup_cfg_fmt-2.3.0/setup_cfg_fmt.egg-info/PKG-INFO` & `setup_cfg_fmt-2.4.0/setup_cfg_fmt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: setup-cfg-fmt
-Version: 2.3.0
+Version: 2.4.0
 Summary: apply a consistent format to `setup.cfg` files
 Home-page: https://github.com/asottile/setup-cfg-fmt
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![build status](https://github.com/asottile/setup-cfg-fmt/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/setup-cfg-fmt/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/setup-cfg-fmt/main.svg)](https://results.pre-commit.ci/latest/github/asottile/setup-cfg-fmt/main)
 
 setup-cfg-fmt
@@ -33,15 +33,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/setup-cfg-fmt
-    rev: v2.3.0
+    rev: v2.4.0
     hooks:
     -   id: setup-cfg-fmt
 ```
 
 ## cli
 
 Consult the help for the latest usage:
```

### Comparing `setup_cfg_fmt-2.3.0/setup_cfg_fmt.py` & `setup_cfg_fmt-2.4.0/setup_cfg_fmt.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
 
 GLOB_PART = re.compile(r'(\[[^]]+\]|.)')
 
 
 def _case_insensitive_glob(s: str) -> str:
     def cb(match: Match[str]) -> str:
-        match_s = match.group()
+        match_s = match[0]
         if len(match_s) == 1:
             return f'[{match_s.upper()}{match_s.lower()}]'
         else:
             inner = ''.join(f'{c.upper()}{c.lower()}' for c in match_s[1:-1])
             return f'[{inner}]'
 
     return GLOB_PART.sub(cb, s)
@@ -118,15 +118,15 @@
 
 
 def _parse_list(s: str) -> list[str]:
     return s.strip().splitlines()
 
 
 def _fmt_list_always(items: list[str]) -> str:
-    return '\n'.join(['', *items])
+    return '\n'.join(('', *items))
 
 
 def _fmt_list(items: list[str]) -> str:
     if len(items) == 1:
         return items[0]
     else:
         return _fmt_list_always(items)
@@ -257,30 +257,27 @@
 
 
 def _normalize_lib(lib: str) -> str:
     base = _req_base(lib)
 
     conditions = ','.join(
         sorted(
-            (
-                f'{m.group(1)}{m.group(2)}'
-                for m in REQ_REGEX.finditer(lib)
-            ),
+            (f'{m[1]}{m[2]}' for m in REQ_REGEX.finditer(lib)),
             key=lambda c: ('<' in c, '>' in 'c', c),
         ),
     )
 
     return f'{base}{conditions}'
 
 
 def _req_base(lib: str) -> str:
     basem = re.match(BASE_NAME_REGEX, lib)
     assert basem
     # pip replaces _ with - in package names
-    return basem.group(0).replace('_', '-')
+    return basem[0].replace('_', '-')
 
 
 def _py_classifiers(
         python_requires: str | None, *, max_py_version: tuple[int, int],
 ) -> list[str]:
     try:
         minimum, exclude = _parse_python_requires(python_requires)
@@ -517,15 +514,15 @@
     parser = argparse.ArgumentParser()
     parser.add_argument('filenames', nargs='*')
     parser.add_argument('--include-version-classifiers', action='store_true')
     parser.add_argument(
         '--min-py3-version', type=_ver_type, default=None,
         help=argparse.SUPPRESS,
     )
-    parser.add_argument('--min-py-version', type=_ver_type, default=(3, 7))
+    parser.add_argument('--min-py-version', type=_ver_type, default=(3, 8))
     parser.add_argument('--max-py-version', type=_ver_type, default=(3, 11))
     args = parser.parse_args(argv)
 
     if args.min_py3_version:
         print(
             'WARNING: setup-cfg-fmt will replace --min-py3-version '
             'with --min-py-version in a future release',
```

