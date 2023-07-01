# Comparing `tmp/zeugvars-0.1.2.tar.gz` & `tmp/zeugvars-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeugvars-0.1.2.tar", max compression
+gzip compressed data, was "zeugvars-0.1.3.tar", max compression
```

## Comparing `zeugvars-0.1.2.tar` & `zeugvars-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1083 2023-06-29 20:37:00.152930 zeugvars-0.1.2/LICENSE
--rw-r--r--   0        0        0      524 2023-07-01 10:22:26.461939 zeugvars-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2491 2023-07-01 10:30:54.698962 zeugvars-0.1.2/README.md
--rw-r--r--   0        0        0    10864 2023-07-01 10:30:54.691960 zeugvars-0.1.2/zeugvars.py
--rw-r--r--   0        0        0     2894 1970-01-01 00:00:00.000000 zeugvars-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-29 20:37:00.152930 zeugvars-0.1.3/LICENSE
+-rw-r--r--   0        0        0      524 2023-07-01 11:10:05.294301 zeugvars-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2474 2023-07-01 11:09:48.290088 zeugvars-0.1.3/README.md
+-rw-r--r--   0        0        0    11260 2023-07-01 11:09:48.282092 zeugvars-0.1.3/zeugvars.py
+-rw-r--r--   0        0        0     2877 1970-01-01 00:00:00.000000 zeugvars-0.1.3/PKG-INFO
```

### Comparing `zeugvars-0.1.2/LICENSE` & `zeugvars-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zeugvars-0.1.2/pyproject.toml` & `zeugvars-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zeugvars"
-version = "0.1.2"
+version = "0.1.3"
 description = "A simple & straight-forward Python module for creating context-dependent proxy objects."
 authors = ["bswck <bswck.dev@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/bswck/zeugvars"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `zeugvars-0.1.2/README.md` & `zeugvars-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
 ## Description
 
 The `zeugvar` function takes a `Manager` object and class (optional) as arguments.
 The `Manager` object must have `get` and `set` methods. The `get` method returns
 the object to which the proxy forwards attribute access. The `set` method sets
 the object to which the proxy forwards attribute access.  `set` is called when
-the proxy is being inplace modified. The class is optional unless the `Manager`
-is bound, i.e. `Manager.get` returns an instance of a class.
+the proxy is being inplace modified. The class parameter is optional,
+but it is strongly recommended for some corner-cases.
 The user might provide custom `getter` and `setter` functions.
 This might be useful when there is the need to keep track of the tokens
 returned by `ContextVar.set()`, if using `ContextVar` as the manager.
 
 ## Example
 
 The following example shows how to use `zeugvar` with `contextvars.ContextVar`:
```

### Comparing `zeugvars-0.1.2/zeugvars.py` & `zeugvars-0.1.3/zeugvars.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 creates a proxy object that forwards attribute access to an object stored
 in the provided manager, which could be any object that implements the
 `Manager` protocol; for example, a `contextvars.ContextVar` object.
 
 Description
 -----------
 The `zeugvar` function takes a `Manager` object and class (optional) as arguments.
-The `Manager` object must have `get` and `set` methods.  The `get` method returns
-the object to which the proxy forwards attribute access.  The `set` method sets
-the object to which the proxy forwards attribute access.  `set` is called when
-the proxy is being inplace modified.  The class is optional unless the `Manager`
-is bound, i.e. `Manager.get` returns an instance of a class.
+The `Manager` object must have `get` and `set` methods. The `get` method returns
+the object to which the proxy forwards attribute access. The `set` method sets
+the object to which the proxy forwards attribute access. `set` is called when
+the proxy is being inplace modified. The class parameter is optional,
+but it is strongly recommended for some corner-cases.
 The user might provide custom `getter` and `setter` functions.
 This might be useful when there is the need to keep track of the tokens
 returned by `ContextVar.set()`, if using `ContextVar` as the manager.
 
 Example
 -------
 The following example shows how to use `zeugvar` with `contextvars.ContextVar`:
@@ -59,33 +59,35 @@
 0
 >>> counter.set(1000)
 <Token var=<ContextVar name='counter' at ...> at ...>
 >>> count
 1000
 """
 
-import contextlib
-import functools
+from contextlib import suppress
+from functools import partial
 from collections.abc import Callable
 from typing import TypeVar, Any, cast, Protocol, runtime_checkable
 
+__all__ = ("zeugvar",)
+
 _T = TypeVar("_T")
 
 
 @runtime_checkable
 class Manager(Protocol[_T]):
     def get(self) -> _T:
         ...
 
     def set(self, value: _T) -> Any:
         ...
 
 
 def zeugvar_descriptor(
-    cls: type[_T],
+    cls: type[_T] | None,
     mgr: Manager[_T],
     getter: Callable[[Manager[_T]], _T],
     setter: Callable[[Manager[_T], _T], None],
     *,
     undefined: Callable[..., Any] | None = None,
     fallback: Callable[..., Any] | None = None,
     custom_mro: bool = False,
@@ -105,18 +107,20 @@
         def __get__(self, instance: _T, owner: type[_T] | None) -> Any:
             if self.attr_name == "__getattr__":
 
                 def attribute(name: str) -> Any:
                     return getattr(getter(mgr), name)
 
             elif self.attr_name in ("__repr__", "__str__"):
-                with contextlib.suppress(RuntimeError):
+                with suppress(RuntimeError):
                     return getattr(getter(mgr), self.attr_name)
 
                 def attribute() -> str:  # type: ignore[misc]
+                    if cls is None:
+                        return "<unbound zeugvar>"
                     return f"<unbound {cls.__name__!r} object>"
 
             else:
                 try:
                     obj = getter(mgr)
                 except RuntimeError:
                     if self.attr_name == "__dir__" and not custom_mro:
@@ -132,15 +136,15 @@
                 else:
                     try:
                         attribute = getattr(obj, self.attr_name)
                     except AttributeError:
                         if not callable(fallback):
                             raise
 
-                        attribute = functools.partial(fallback, obj)
+                        attribute = partial(fallback, obj)
 
             if inplace:
                 def _apply_inplace(*args: Any, **kwargs: Any) -> _T:
                     ret = attribute(*args, **kwargs)
                     setter(mgr, ret)
                     return instance
 
@@ -170,32 +174,37 @@
 
 def _cv_setter(mgr: Manager[_T], value: _T) -> None:
     mgr.set(value)
 
 
 def zeugvar(
     mgr: Manager[_T],
-    cls: type[_T] = None,  # type: ignore[assignment]
+    cls: type[_T] | None = None,
     getter: Callable[[Manager[_T]], _T] = None,  # type: ignore[assignment]
     setter: Callable[[Manager[_T], _T], None] = None,  # type: ignore[assignment]
 ) -> _T:
     """See `zeugvars` module docstring for usage and example."""
 
     if getter is None:
         getter = _cv_getter
 
     if setter is None:
         setter = _cv_setter
 
     if cls is None:
-        cls = type(getter(mgr))
+        with suppress(RuntimeError):
+            cls = type(getter(mgr))
+
+    if cls is None:
+        custom_mro = False
+    else:
+        mro: Callable[[], tuple[type[Any], ...]] = object.__getattribute__(cls, "mro")
+        custom_mro = not hasattr(mro, "__self__")
 
-    mro: Callable[[], tuple[type[Any], ...]] = object.__getattribute__(cls, "mro")
-    custom_mro = not hasattr(mro, "__self__")
-    descriptor = functools.partial(
+    descriptor = partial(
         zeugvar_descriptor, cls, mgr, getter, setter, custom_mro=custom_mro
     )
 
     class _ZeugVarMeta(type):
         __doc__ = descriptor()
         __wrapped__ = descriptor()
         __repr__ = descriptor()
@@ -209,16 +218,20 @@
         __gt__ = descriptor()
         __ge__ = descriptor()
         __hash__ = descriptor()
         __bool__ = descriptor(undefined=lambda: False)
         __getattr__ = descriptor()
         __setattr__ = descriptor()
         __delattr__ = descriptor()
-        __dir__ = descriptor(undefined=lambda: dir(cls))
-        __class__ = descriptor(undefined=lambda: cls)
+        if cls is None:
+            __dir__ = descriptor()
+            __class__ = descriptor()
+        else:
+            __dir__ = descriptor(undefined=lambda: dir(cls))
+            __class__ = descriptor(undefined=lambda: cls)
         __instancecheck__ = descriptor()
         __subclasscheck__ = descriptor()
         __call__ = descriptor()
         __len__ = descriptor()
         __length_hint__ = descriptor()
         __getitem__ = descriptor()
         __setitem__ = descriptor()
@@ -286,22 +299,24 @@
         __aiter__ = descriptor()
         __anext__ = descriptor()
         __aenter__ = descriptor()
         __aexit__ = descriptor()
         __copy__ = descriptor()
         __deepcopy__ = descriptor()
 
-    zv = cast(_T, _ZeugVarMeta(cls.__name__, (), {}))
+    cls_name = cls.__name__ if cls is not None else f"zeugvar_{id(mgr):x}"
+
+    zv = cast(_T, _ZeugVarMeta(cls_name, (), {}))
     if not custom_mro:
 
         def _mro_wrapper() -> tuple[type[Any], ...]:
             try:
-                getter(mgr)
+                obj = getter(mgr)
             except RuntimeError:
                 return mro()
             else:
                 raise AttributeError(
-                    f"{cls.__name__!r} object has no attribute 'mro'"
+                    f"{type(obj).__name__!r} object has no attribute 'mro'"
                 ) from None
 
         type.__setattr__(zv, "mro", _mro_wrapper)
     return zv
```

### Comparing `zeugvars-0.1.2/PKG-INFO` & `zeugvars-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeugvars
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple & straight-forward Python module for creating context-dependent proxy objects.
 Home-page: https://github.com/bswck/zeugvars
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -39,16 +39,16 @@
 
 ## Description
 
 The `zeugvar` function takes a `Manager` object and class (optional) as arguments.
 The `Manager` object must have `get` and `set` methods. The `get` method returns
 the object to which the proxy forwards attribute access. The `set` method sets
 the object to which the proxy forwards attribute access.  `set` is called when
-the proxy is being inplace modified. The class is optional unless the `Manager`
-is bound, i.e. `Manager.get` returns an instance of a class.
+the proxy is being inplace modified. The class parameter is optional,
+but it is strongly recommended for some corner-cases.
 The user might provide custom `getter` and `setter` functions.
 This might be useful when there is the need to keep track of the tokens
 returned by `ContextVar.set()`, if using `ContextVar` as the manager.
 
 ## Example
 
 The following example shows how to use `zeugvar` with `contextvars.ContextVar`:
```

