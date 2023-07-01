# Comparing `tmp/cfg-param-wrapper-1.0.0.post2.tar.gz` & `tmp/cfg-param-wrapper-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfg-param-wrapper-1.0.0.post2.tar", last modified: Sun Jun 11 22:59:07 2023, max compression
+gzip compressed data, was "cfg-param-wrapper-1.0.1.tar", last modified: Sat Jul  1 05:28:08 2023, max compression
```

## Comparing `cfg-param-wrapper-1.0.0.post2.tar` & `cfg-param-wrapper-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-11 22:59:07.486929 cfg-param-wrapper-1.0.0.post2/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1071 2023-04-12 20:40:08.000000 cfg-param-wrapper-1.0.0.post2/LICENSE
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1587 2023-06-11 22:59:07.486929 cfg-param-wrapper-1.0.0.post2/PKG-INFO
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      748 2023-06-11 22:58:44.000000 cfg-param-wrapper-1.0.0.post2/README.md
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      959 2023-06-11 22:58:36.000000 cfg-param-wrapper-1.0.0.post2/pyproject.toml
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       38 2023-06-11 22:59:07.486929 cfg-param-wrapper-1.0.0.post2/setup.cfg
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-11 22:59:07.486929 cfg-param-wrapper-1.0.0.post2/src/
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-11 22:59:07.486929 cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      316 2023-06-07 03:20:42.000000 cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper/__init__.py
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     9978 2023-06-07 01:13:05.000000 cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper/argparse_config.py
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2966 2023-06-11 22:56:57.000000 cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper/cfg_dict.py
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2258 2023-06-11 22:57:11.000000 cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper/function_config_wrapper.py
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1934 2023-06-11 22:55:59.000000 cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper/save_handlers.py
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-11 22:59:07.486929 cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper.egg-info/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1587 2023-06-11 22:59:07.000000 cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      453 2023-06-11 22:59:07.000000 cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)        1 2023-06-11 22:59:07.000000 cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       25 2023-06-11 22:59:07.000000 cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper.egg-info/requires.txt
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       18 2023-06-11 22:59:07.000000 cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 zepto     (1000) zepto     (1000)        0 2023-07-01 05:28:08.830288 cfg-param-wrapper-1.0.1/
+-rw-r--r--   0 zepto     (1000) zepto     (1000)     1071 2023-04-12 20:40:08.000000 cfg-param-wrapper-1.0.1/LICENSE
+-rw-r--r--   0 zepto     (1000) zepto     (1000)     2272 2023-07-01 05:28:08.830288 cfg-param-wrapper-1.0.1/PKG-INFO
+-rw-r--r--   0 zepto     (1000) zepto     (1000)     1440 2023-07-01 05:27:50.000000 cfg-param-wrapper-1.0.1/README.md
+-rw-r--r--   0 zepto     (1000) zepto     (1000)      957 2023-07-01 05:27:56.000000 cfg-param-wrapper-1.0.1/pyproject.toml
+-rw-r--r--   0 zepto     (1000) zepto     (1000)       38 2023-07-01 05:28:08.830288 cfg-param-wrapper-1.0.1/setup.cfg
+drwxr-xr-x   0 zepto     (1000) zepto     (1000)        0 2023-07-01 05:28:08.828288 cfg-param-wrapper-1.0.1/src/
+drwxr-xr-x   0 zepto     (1000) zepto     (1000)        0 2023-07-01 05:28:08.829288 cfg-param-wrapper-1.0.1/src/cfg_param_wrapper/
+-rw-r--r--   0 zepto     (1000) zepto     (1000)      316 2023-06-07 03:20:42.000000 cfg-param-wrapper-1.0.1/src/cfg_param_wrapper/__init__.py
+-rw-r--r--   0 zepto     (1000) zepto     (1000)     9978 2023-06-07 01:13:05.000000 cfg-param-wrapper-1.0.1/src/cfg_param_wrapper/argparse_config.py
+-rw-r--r--   0 zepto     (1000) zepto     (1000)     3073 2023-07-01 05:22:43.000000 cfg-param-wrapper-1.0.1/src/cfg_param_wrapper/cfg_dict.py
+-rw-r--r--   0 zepto     (1000) zepto     (1000)     2456 2023-06-20 06:23:06.000000 cfg-param-wrapper-1.0.1/src/cfg_param_wrapper/function_config_wrapper.py
+-rw-r--r--   0 zepto     (1000) zepto     (1000)     2166 2023-07-01 05:27:21.000000 cfg-param-wrapper-1.0.1/src/cfg_param_wrapper/save_handlers.py
+drwxr-xr-x   0 zepto     (1000) zepto     (1000)        0 2023-07-01 05:28:08.830288 cfg-param-wrapper-1.0.1/src/cfg_param_wrapper.egg-info/
+-rw-r--r--   0 zepto     (1000) zepto     (1000)     2272 2023-07-01 05:28:08.000000 cfg-param-wrapper-1.0.1/src/cfg_param_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 zepto     (1000) zepto     (1000)      453 2023-07-01 05:28:08.000000 cfg-param-wrapper-1.0.1/src/cfg_param_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 zepto     (1000) zepto     (1000)        1 2023-07-01 05:28:08.000000 cfg-param-wrapper-1.0.1/src/cfg_param_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 zepto     (1000) zepto     (1000)       25 2023-07-01 05:28:08.000000 cfg-param-wrapper-1.0.1/src/cfg_param_wrapper.egg-info/requires.txt
+-rw-r--r--   0 zepto     (1000) zepto     (1000)       18 2023-07-01 05:28:08.000000 cfg-param-wrapper-1.0.1/src/cfg_param_wrapper.egg-info/top_level.txt
```

### Comparing `cfg-param-wrapper-1.0.0.post2/LICENSE` & `cfg-param-wrapper-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cfg-param-wrapper-1.0.0.post2/PKG-INFO` & `cfg-param-wrapper-1.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfg-param-wrapper
-Version: 1.0.0.post2
+Version: 1.0.1
 Summary: A package designed to simplify defaults.
 Author-email: Zeptofine <zeptofine@gmail.com>
 Project-URL: Homepage, https://github.com/zeptofine/cfg-argparser
 Project-URL: Bug Tracker, https://github.com/zeptofine/cfg-argparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -14,39 +14,52 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: typer
 License-File: LICENSE
 
-# cfg_param_wrapper 1.0.0-2
+# cfg_param_wrapper 1.0.1
 
 a config wrapper I made. It's made to wrap simple functions, and intercept configurations in tandem with a CfgDict object.
 
+Check the [Github](https://github.com/zeptofine/cfg-param_wrapper/) README! It's likely more up to date.
+
 ## Installation
 
 ```bash
 # from pypi:
 pip install cfg-param-wrapper
 
 # from github:
 git clone "https://github.com/zeptofine/cfg-param-wrapper"
 cd cfg-param-wrapper
 pip install -e .
-
 ```
 
+## @wrap_config
+
+The `wrap_config` decorator is meant to wrap a function, take their parameters and create a config file from it. Once a function is wrapped using `@wrap_config`, either the cfg can change and the function's default parameters are updated according to the argument names and such.
+
+This is very useful in `Typer` and `Click` commands (wrap it before declaring a command).
+
+## CfgDict
+
+This is a dictionary subclass that takes a filename, and saves all the changes to the file using `json` or `toml`.
+
+It allows custom encoders and decoders for the file formats it supports.
+
 ## Example
 
 ```python
 from cfg_param_wrapper import wrap_config, CfgDict
 
 cfg = CfgDict("test.json")
 @wrap_config(cfg)
-def test_function(s: str, is_real: bool = True): # I'd advise only wrapping functions all having default methods
+def test_function(s: str, is_real: bool = True): # I'd advise only wrapping functions with default parameters
     return f"{s} is {'real' if is_real else 'fake'}"
 
 if __name__ == "__main__":
   print(test_function("We"))
   cfg['s'] = "us"
   print(test_function()) # Linters hate him!
 ```
```

### Comparing `cfg-param-wrapper-1.0.0.post2/pyproject.toml` & `cfg-param-wrapper-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cfg-param-wrapper"
-version = "1.0.0-2"
+version = "1.0.1"
 authors = [{ name = "Zeptofine", email = "zeptofine@gmail.com" }]
 description = "A package designed to simplify defaults."
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
```

### Comparing `cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper/argparse_config.py` & `cfg-param-wrapper-1.0.1/src/cfg_param_wrapper/argparse_config.py`

 * *Files identical despite different names*

### Comparing `cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper/cfg_dict.py` & `cfg-param-wrapper-1.0.1/src/cfg_param_wrapper/cfg_dict.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,24 +19,27 @@
         cfg_path: str | Path,
         config: dict | None = None,
         autofill: bool = False,
         save_on_change: bool = False,
         sort_on_save: bool = False,
         start_empty: bool = False,
         save_mode: Literal["json", "toml"] = "json",
+        encoder=None,
+        decoder=None,
     ) -> None:
         config = config or {}
         super().__init__(config)
         self.cfg_path: str | Path = cfg_path
         self.save_on_change: bool = save_on_change
         self.sort_on_save: bool = sort_on_save
 
         assert save_mode in HANDLERS
         self.save_handler: SaveHandler = HANDLERS[save_mode](cfg_path)
-
+        self.encoder = encoder
+        self.decoder = decoder
         if not os.path.exists(self.cfg_path) and autofill:
             self.save(config)
         if not start_empty:
             self.load()
 
     def set_path(self, path):
         """sets a new path to follow"""
@@ -46,16 +49,15 @@
 
     def save(self, out_dict=None):
         """saves the dict to the file"""
         if not isinstance(out_dict, dict):
             out_dict = self
         if self.sort_on_save:
             out_dict = dict(sorted(out_dict.items()))
-        print(out_dict)
-        self.save_handler.save(dict(out_dict))
+        self.save_handler.save(dict(out_dict), self.encoder)
         return self
 
     def _save_on_change(self) -> bool:
         if self.save_on_change:
             self.save()
             return True
         return False
@@ -74,15 +76,15 @@
         super().clear()
         return self
 
     def load(self):
         """Loads the data from the file"""
         if os.path.exists(self.cfg_path):
             try:
-                self.update(self.save_handler.load())
+                self.update(self.save_handler.load(self.decoder))
             except Exception:
                 print(f"[!] failed to load config from {self.cfg_path}")
         else:
             self.save({})
         return self
 
     def is_serializable(self, obj: Any) -> bool:
```

### Comparing `cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper/function_config_wrapper.py` & `cfg-param-wrapper-1.0.1/src/cfg_param_wrapper/function_config_wrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,19 +17,29 @@
     fn.__dict__.update(f.__dict__)
     fn.__annotations__ = f.__annotations__
     fn.__doc__ = f.__doc__
     return fn
 
 
 def wrap_config(cfg_dict: CfgDict) -> Callable[..., Callable]:
-    """Wraps a function with a CfgDict file to make an easy config configuration"""
+    '''Wraps a function with a CfgDict to make an easy config setup.
 
+    Parameters
+    ----------
+    cfg_dict : CfgDict
+        The file to write to. Must be a CfgDict.
+
+    Returns
+    -------
+    Callable[..., Callable]
+        a function that takes a wrapped function.
+    '''
     def _wrapper(func: Callable) -> Callable:
-        # get parameters and defaults
 
+        # get parameters and defaults
         parameters: dict[str, inspect.Parameter] = dict(inspect.signature(func).parameters)
         save_after = False
         for name, param in parameters.items():
             if name not in cfg_dict:
                 if cfg_dict.is_serializable(param.default):
                     save_after = True
                     cfg_dict[name] = param.default
```

### Comparing `cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper/save_handlers.py` & `cfg-param-wrapper-1.0.1/src/cfg_param_wrapper/save_handlers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from __future__ import annotations
 
 import json
 from abc import abstractmethod
-from collections.abc import Callable
+from collections.abc import Callable, Mapping
 from pathlib import Path
 from typing import Any
 
 import toml
 
 
 class SaveHandler:
     def __init__(self, path: str | Path):
         self.path: Path = Path(path)
 
     @abstractmethod
-    def save(self, dct: dict) -> None:
+    def save(self, dct: dict, encoder=None) -> None:
         """saves the given dict to self.path"""
 
     @abstractmethod
-    def load(self) -> dict:
+    def load(self, decoder=None) -> dict:
         """loads a dictionary from self.path"""
 
     @abstractmethod
     def try_serialize(self, object: object) -> bool:
         """Tries to serialize the item and returns whether it is successful"""
 
     def _write(self, func: Callable, mode="w") -> None:
@@ -33,37 +33,42 @@
         with open(self.path, mode, encoding="utf-8") as file:
             return func(file)
 
 
 class JsonSaveHandler(SaveHandler):
     """A save handler made to save and load .json files"""
 
-    def save(self, dct: dict) -> None:
-        self._write(lambda file: json.dump(dct, file, indent=4))
+    def save(self, dct: dict, encoder=None) -> None:
+        self._write(lambda file: json.dump(dct, file, indent=4, cls=encoder))
 
-    def load(self) -> dict:
-        return self._read(json.load)
+    def load(self, decoder=None) -> dict:
+        return self._read(lambda file: json.load(file, cls=decoder))
 
     def try_serialize(self, object: object) -> bool:
         try:
             json.dumps(object)
             return True
         except (TypeError, OverflowError):
             return False
 
+
 class TomlSaveHandler(SaveHandler):
     """A save handler made to save and load .toml files"""
 
-    def save(self, dct: dict) -> None:
-        self._write(lambda file: toml.dump(dct, file))
+    def save(self, dct: dict, encoder: toml.TomlEncoder | None = None) -> None:
+        self._write(lambda file: toml.dump(dct, file, encoder=encoder))
 
-    def load(self) -> dict:
-        return self._read(toml.load)
+    def load(self, decoder=None) -> dict:
+        return self._read(lambda file: toml.load(file, decoder=decoder))
 
-    def try_serialize(self, object: object) -> bool:
+    def try_serialize(self, object: Mapping) -> bool:
         try:
             toml.dumps(object)
             return True
         except (TypeError, OverflowError, ValueError):
             return False
 
-HANDLERS: dict[str, type[SaveHandler]] = {"json": JsonSaveHandler, "toml": TomlSaveHandler}
+
+HANDLERS: dict[str, type[SaveHandler]] = {
+    "json": JsonSaveHandler,
+    "toml": TomlSaveHandler,
+}
```

### Comparing `cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper.egg-info/PKG-INFO` & `cfg-param-wrapper-1.0.1/src/cfg_param_wrapper.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfg-param-wrapper
-Version: 1.0.0.post2
+Version: 1.0.1
 Summary: A package designed to simplify defaults.
 Author-email: Zeptofine <zeptofine@gmail.com>
 Project-URL: Homepage, https://github.com/zeptofine/cfg-argparser
 Project-URL: Bug Tracker, https://github.com/zeptofine/cfg-argparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -14,39 +14,52 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: typer
 License-File: LICENSE
 
-# cfg_param_wrapper 1.0.0-2
+# cfg_param_wrapper 1.0.1
 
 a config wrapper I made. It's made to wrap simple functions, and intercept configurations in tandem with a CfgDict object.
 
+Check the [Github](https://github.com/zeptofine/cfg-param_wrapper/) README! It's likely more up to date.
+
 ## Installation
 
 ```bash
 # from pypi:
 pip install cfg-param-wrapper
 
 # from github:
 git clone "https://github.com/zeptofine/cfg-param-wrapper"
 cd cfg-param-wrapper
 pip install -e .
-
 ```
 
+## @wrap_config
+
+The `wrap_config` decorator is meant to wrap a function, take their parameters and create a config file from it. Once a function is wrapped using `@wrap_config`, either the cfg can change and the function's default parameters are updated according to the argument names and such.
+
+This is very useful in `Typer` and `Click` commands (wrap it before declaring a command).
+
+## CfgDict
+
+This is a dictionary subclass that takes a filename, and saves all the changes to the file using `json` or `toml`.
+
+It allows custom encoders and decoders for the file formats it supports.
+
 ## Example
 
 ```python
 from cfg_param_wrapper import wrap_config, CfgDict
 
 cfg = CfgDict("test.json")
 @wrap_config(cfg)
-def test_function(s: str, is_real: bool = True): # I'd advise only wrapping functions all having default methods
+def test_function(s: str, is_real: bool = True): # I'd advise only wrapping functions with default parameters
     return f"{s} is {'real' if is_real else 'fake'}"
 
 if __name__ == "__main__":
   print(test_function("We"))
   cfg['s'] = "us"
   print(test_function()) # Linters hate him!
 ```
```

