# Comparing `tmp/add_trailing_comma-2.5.1.tar.gz` & `tmp/add_trailing_comma-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "add_trailing_comma-2.5.1.tar", last modified: Sat Jun 10 21:05:03 2023, max compression
+gzip compressed data, was "add_trailing_comma-3.0.0.tar", last modified: Sat Jul  1 17:57:01 2023, max compression
```

## Comparing `add_trailing_comma-2.5.1.tar` & `add_trailing_comma-3.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 21:05:03.163805 add_trailing_comma-2.5.1/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.1/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4669 2023-06-10 21:05:03.167805 add_trailing_comma-2.5.1/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4032 2023-06-10 21:05:02.000000 add_trailing_comma-2.5.1/README.md
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 21:05:03.163805 add_trailing_comma-2.5.1/add_trailing_comma/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.1/add_trailing_comma/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      135 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.1/add_trailing_comma/__main__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      733 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.1/add_trailing_comma/_ast_helpers.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2307 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.1/add_trailing_comma/_data.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3228 2023-06-10 21:05:02.000000 add_trailing_comma-2.5.1/add_trailing_comma/_main.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 21:05:03.163805 add_trailing_comma-2.5.1/add_trailing_comma/_plugins/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.1/add_trailing_comma/_plugins/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1129 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.1/add_trailing_comma/_plugins/_with.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1887 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.1/add_trailing_comma/_plugins/calls.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1254 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.1/add_trailing_comma/_plugins/classes.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1645 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.1/add_trailing_comma/_plugins/functions.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1256 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.1/add_trailing_comma/_plugins/imports.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3058 2023-06-10 20:30:39.000000 add_trailing_comma-2.5.1/add_trailing_comma/_plugins/literals.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2451 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.1/add_trailing_comma/_plugins/match.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6613 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.1/add_trailing_comma/_token_helpers.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 21:05:03.163805 add_trailing_comma-2.5.1/add_trailing_comma.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4669 2023-06-10 21:05:03.000000 add_trailing_comma-2.5.1/add_trailing_comma.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      790 2023-06-10 21:05:03.000000 add_trailing_comma-2.5.1/add_trailing_comma.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-10 21:05:03.000000 add_trailing_comma-2.5.1/add_trailing_comma.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       69 2023-06-10 21:05:03.000000 add_trailing_comma-2.5.1/add_trailing_comma.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       19 2023-06-10 21:05:03.000000 add_trailing_comma-2.5.1/add_trailing_comma.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       19 2023-06-10 21:05:03.000000 add_trailing_comma-2.5.1/add_trailing_comma.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1233 2023-06-10 21:05:03.167805 add_trailing_comma-2.5.1/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-06-10 20:24:15.000000 add_trailing_comma-2.5.1/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-01 17:57:01.880476 add_trailing_comma-3.0.0/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4669 2023-07-01 17:57:01.880476 add_trailing_comma-3.0.0/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4032 2023-07-01 17:57:01.000000 add_trailing_comma-3.0.0/README.md
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-01 17:57:01.880476 add_trailing_comma-3.0.0/add_trailing_comma/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/add_trailing_comma/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      135 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/add_trailing_comma/__main__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      733 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/add_trailing_comma/_ast_helpers.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2126 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/add_trailing_comma/_data.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2991 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/add_trailing_comma/_main.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-01 17:57:01.880476 add_trailing_comma-3.0.0/add_trailing_comma/_plugins/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/add_trailing_comma/_plugins/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1129 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/add_trailing_comma/_plugins/_with.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1582 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/add_trailing_comma/_plugins/calls.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1254 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/add_trailing_comma/_plugins/classes.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1384 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/add_trailing_comma/_plugins/functions.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1256 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/add_trailing_comma/_plugins/imports.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3058 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/add_trailing_comma/_plugins/literals.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2451 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/add_trailing_comma/_plugins/match.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     6613 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/add_trailing_comma/_token_helpers.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-01 17:57:01.880476 add_trailing_comma-3.0.0/add_trailing_comma.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4669 2023-07-01 17:57:01.000000 add_trailing_comma-3.0.0/add_trailing_comma.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      790 2023-07-01 17:57:01.000000 add_trailing_comma-3.0.0/add_trailing_comma.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-07-01 17:57:01.000000 add_trailing_comma-3.0.0/add_trailing_comma.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       69 2023-07-01 17:57:01.000000 add_trailing_comma-3.0.0/add_trailing_comma.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       19 2023-07-01 17:57:01.000000 add_trailing_comma-3.0.0/add_trailing_comma.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       19 2023-07-01 17:57:01.000000 add_trailing_comma-3.0.0/add_trailing_comma.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1233 2023-07-01 17:57:01.880476 add_trailing_comma-3.0.0/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-07-01 17:56:56.000000 add_trailing_comma-3.0.0/setup.py
```

### Comparing `add_trailing_comma-2.5.1/LICENSE` & `add_trailing_comma-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.5.1/PKG-INFO` & `add_trailing_comma-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: add_trailing_comma
-Version: 2.5.1
+Version: 3.0.0
 Summary: Automatically add trailing commas to calls and literals
 Home-page: https://github.com/asottile/add-trailing-comma
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -34,15 +34,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/add-trailing-comma
-    rev: v2.5.1
+    rev: v3.0.0
     hooks:
     -   id: add-trailing-comma
 ```
 
 ## multi-line method invocation style -- why?
 
 ```python
```

### Comparing `add_trailing_comma-2.5.1/README.md` & `add_trailing_comma-3.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/add-trailing-comma
-    rev: v2.5.1
+    rev: v3.0.0
     hooks:
     -   id: add-trailing-comma
 ```
 
 ## multi-line method invocation style -- why?
 
 ```python
```

### Comparing `add_trailing_comma-2.5.1/add_trailing_comma/_ast_helpers.py` & `add_trailing_comma-3.0.0/add_trailing_comma/_ast_helpers.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.5.1/add_trailing_comma/_data.py` & `add_trailing_comma-3.0.0/add_trailing_comma/_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,33 +3,25 @@
 import ast
 import collections
 import pkgutil
 from typing import Callable
 from typing import Iterable
 from typing import List
 from typing import NamedTuple
+from typing import Protocol
 from typing import Tuple
-from typing import TYPE_CHECKING
 from typing import TypeVar
 
 from tokenize_rt import Offset
 from tokenize_rt import Token
 
 from add_trailing_comma import _plugins
 
-if TYPE_CHECKING:
-    from typing import Protocol
-else:
-    Protocol = object
-
-Version = Tuple[int, ...]
-
 
 class State(NamedTuple):
-    min_version: Version
     in_fstring: bool = False
 
 
 AST_T = TypeVar('AST_T', bound=ast.AST)
 TokenFunc = Callable[[int, List[Token]], None]
 ASTFunc = Callable[[State, AST_T], Iterable[Tuple[Offset, TokenFunc]]]
 
@@ -46,17 +38,16 @@
 class ASTCallbackMapping(Protocol):
     def __getitem__(self, tp: type[AST_T]) -> list[ASTFunc[AST_T]]: ...
 
 
 def visit(
         funcs: ASTCallbackMapping,
         tree: ast.AST,
-        version: Version,
 ) -> dict[Offset, list[TokenFunc]]:
-    nodes = [(tree, State(min_version=version))]
+    nodes = [(tree, State())]
 
     ret = collections.defaultdict(list)
     while nodes:
         node, state = nodes.pop()
 
         tp = type(node)
         for ast_func in funcs[tp]:
```

### Comparing `add_trailing_comma-2.5.1/add_trailing_comma/_main.py` & `add_trailing_comma-3.0.0/add_trailing_comma/_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,21 +20,21 @@
 def _changing_list(lst: list[Token]) -> Iterable[tuple[int, Token]]:
     i = 0
     while i < len(lst):
         yield i, lst[i]
         i += 1
 
 
-def _fix_src(contents_text: str, min_version: tuple[int, ...]) -> str:
+def _fix_src(contents_text: str) -> str:
     try:
         ast_obj = ast_parse(contents_text)
     except SyntaxError:
         return contents_text
 
-    callbacks = visit(FUNCS, ast_obj, min_version)
+    callbacks = visit(FUNCS, ast_obj)
 
     tokens = src_to_tokens(contents_text)
     for i, token in _changing_list(tokens):
         # DEDENT is a zero length token
         if not token.src:
             continue
 
@@ -63,15 +63,15 @@
     try:
         contents_text_orig = contents_text = contents_bytes.decode()
     except UnicodeDecodeError:
         msg = f'{filename} is non-utf-8 (not supported)'
         print(msg, file=sys.stderr)
         return 1
 
-    contents_text = _fix_src(contents_text, args.min_version)
+    contents_text = _fix_src(contents_text)
 
     if filename == '-':
         print(contents_text, end='')
     elif contents_text != contents_text_orig:
         print(f'Rewriting {filename}', file=sys.stderr)
         with open(filename, 'wb') as f:
             f.write(contents_text.encode())
@@ -82,29 +82,20 @@
         return contents_text != contents_text_orig
 
 
 def main(argv: Sequence[str] | None = None) -> int:
     parser = argparse.ArgumentParser()
     parser.add_argument('filenames', nargs='*')
     parser.add_argument('--exit-zero-even-if-changed', action='store_true')
-    parser.add_argument(
-        '--py35-plus',
-        action='store_const', dest='min_version', const=(3, 5), default=(2, 7),
-    )
-    parser.add_argument(
-        '--py36-plus',
-        action='store_const', dest='min_version', const=(3, 6),
-    )
+    parser.add_argument('--py35-plus', action='store_true')
+    parser.add_argument('--py36-plus', action='store_true')
     args = parser.parse_args(argv)
 
-    if args.min_version < (3, 6):
-        print(
-            'WARNING: add-trailing-comma will only use 3.6+ mode after 3.0',
-            file=sys.stderr,
-        )
+    if args.py35_plus or args.py36_plus:
+        print('WARNING: --py35-plus / --py36-plus do nothing', file=sys.stderr)
 
     ret = 0
     for filename in args.filenames:
         ret |= fix_file(filename, args)
     return ret
```

### Comparing `add_trailing_comma-2.5.1/add_trailing_comma/_plugins/_with.py` & `add_trailing_comma-3.0.0/add_trailing_comma/_plugins/_with.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.5.1/add_trailing_comma/_plugins/calls.py` & `add_trailing_comma-3.0.0/add_trailing_comma/_plugins/calls.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,50 +15,42 @@
 from add_trailing_comma._token_helpers import fix_brace
 
 
 def _fix_call(
         i: int,
         tokens: list[Token],
         *,
-        add_comma: bool,
         arg_offsets: set[Offset],
 ) -> None:
     return fix_brace(
         tokens,
         find_call(arg_offsets, i, tokens),
-        add_comma=add_comma,
+        add_comma=True,
         remove_comma=True,
     )
 
 
 @register(ast.Call)
 def visit_Call(
         state: State,
         node: ast.Call,
 ) -> Iterable[tuple[Offset, TokenFunc]]:
     argnodes = [*node.args, *node.keywords]
     arg_offsets = set()
-    has_starargs = False
     for argnode in argnodes:
-        if isinstance(argnode, ast.Starred):
-            has_starargs = True
-        if isinstance(argnode, ast.keyword) and argnode.arg is None:
-            has_starargs = True
-
         offset = ast_to_offset(argnode)
         # multiline strings have invalid position, ignore them
         if offset.utf8_byte_offset != -1:  # pragma: no branch (cpy bug)
             arg_offsets.add(offset)
 
     # If the sole argument is a generator, don't add a trailing comma as
     # this breaks lib2to3 based tools
     only_a_generator = (
         len(argnodes) == 1 and isinstance(argnodes[0], ast.GeneratorExp)
     )
 
     if arg_offsets and not only_a_generator and not state.in_fstring:
         func = functools.partial(
             _fix_call,
-            add_comma=not has_starargs or state.min_version >= (3, 5),
             arg_offsets=arg_offsets,
         )
         yield ast_to_offset(node), func
```

### Comparing `add_trailing_comma-2.5.1/add_trailing_comma/_plugins/classes.py` & `add_trailing_comma-3.0.0/add_trailing_comma/_plugins/classes.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.5.1/add_trailing_comma/_plugins/functions.py` & `add_trailing_comma-3.0.0/add_trailing_comma/_plugins/functions.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,48 +15,39 @@
 from add_trailing_comma._token_helpers import fix_brace
 
 
 def _fix_func(
         i: int,
         tokens: list[Token],
         *,
-        add_comma: bool,
         arg_offsets: set[Offset],
 ) -> None:
     fix_brace(
         tokens,
         find_call(arg_offsets, i, tokens),
-        add_comma=add_comma,
+        add_comma=True,
         remove_comma=True,
     )
 
 
 def visit_FunctionDef(
         state: State,
         node: ast.AsyncFunctionDef | ast.FunctionDef,
 ) -> Iterable[tuple[Offset, TokenFunc]]:
-    has_starargs = False
-    args = [*getattr(node.args, 'posonlyargs', ()), *node.args.args]
+    args = [*node.args.posonlyargs, *node.args.args]
 
     if node.args.vararg:
         args.append(node.args.vararg)
-        has_starargs = True
     if node.args.kwarg:
         args.append(node.args.kwarg)
-        has_starargs = True
     if node.args.kwonlyargs:
         args.extend(node.args.kwonlyargs)
-        has_starargs = True
 
     arg_offsets = {ast_to_offset(arg) for arg in args}
 
     if arg_offsets:
-        func = functools.partial(
-            _fix_func,
-            add_comma=not has_starargs or state.min_version >= (3, 6),
-            arg_offsets=arg_offsets,
-        )
+        func = functools.partial(_fix_func, arg_offsets=arg_offsets)
         yield ast_to_offset(node), func
 
 
 register(ast.AsyncFunctionDef)(visit_FunctionDef)
 register(ast.FunctionDef)(visit_FunctionDef)
```

### Comparing `add_trailing_comma-2.5.1/add_trailing_comma/_plugins/imports.py` & `add_trailing_comma-3.0.0/add_trailing_comma/_plugins/imports.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.5.1/add_trailing_comma/_plugins/literals.py` & `add_trailing_comma-3.0.0/add_trailing_comma/_plugins/literals.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.5.1/add_trailing_comma/_plugins/match.py` & `add_trailing_comma-3.0.0/add_trailing_comma/_plugins/match.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.5.1/add_trailing_comma/_token_helpers.py` & `add_trailing_comma-3.0.0/add_trailing_comma/_token_helpers.py`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.5.1/add_trailing_comma.egg-info/PKG-INFO` & `add_trailing_comma-3.0.0/add_trailing_comma.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: add-trailing-comma
-Version: 2.5.1
+Version: 3.0.0
 Summary: Automatically add trailing commas to calls and literals
 Home-page: https://github.com/asottile/add-trailing-comma
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -34,15 +34,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/add-trailing-comma
-    rev: v2.5.1
+    rev: v3.0.0
     hooks:
     -   id: add-trailing-comma
 ```
 
 ## multi-line method invocation style -- why?
 
 ```python
```

### Comparing `add_trailing_comma-2.5.1/add_trailing_comma.egg-info/SOURCES.txt` & `add_trailing_comma-3.0.0/add_trailing_comma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `add_trailing_comma-2.5.1/setup.cfg` & `add_trailing_comma-3.0.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = add_trailing_comma
-version = 2.5.1
+version = 3.0.0
 description = Automatically add trailing commas to calls and literals
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/add-trailing-comma
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
```

