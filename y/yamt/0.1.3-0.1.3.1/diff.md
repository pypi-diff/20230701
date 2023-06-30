# Comparing `tmp/yamt-0.1.3.tar.gz` & `tmp/yamt-0.1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamt-0.1.3.tar", max compression
+gzip compressed data, was "yamt-0.1.3.1.tar", max compression
```

## Comparing `yamt-0.1.3.tar` & `yamt-0.1.3.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1098 2022-07-09 20:34:21.759651 yamt-0.1.3/LICENSE
--rw-r--r--   0        0        0      546 2023-06-30 22:09:54.280636 yamt-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      327 2022-07-09 20:34:21.759651 yamt-0.1.3/README.md
--rw-r--r--   0        0        0      641 2023-02-24 00:04:48.443064 yamt-0.1.3/yamt/__init__.py
--rw-r--r--   0        0        0     4782 2022-11-14 20:24:48.298437 yamt-0.1.3/yamt/asyncio_misc.py
--rw-r--r--   0        0        0     2810 2023-02-17 19:27:48.444386 yamt-0.1.3/yamt/asyncio_sync_primitives.py
--rw-r--r--   0        0        0     8513 2023-03-28 05:21:29.388039 yamt-0.1.3/yamt/collections.py
--rw-r--r--   0        0        0     2012 2022-11-12 16:33:43.019509 yamt-0.1.3/yamt/enum.py
--rw-r--r--   0        0        0     5609 2023-06-30 22:01:34.485430 yamt-0.1.3/yamt/misc.py
--rw-r--r--   0        0        0      193 2022-07-09 20:34:21.763604 yamt-0.1.3/yamt/typing.py
--rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 yamt-0.1.3/setup.py
--rw-r--r--   0        0        0      819 1970-01-01 00:00:00.000000 yamt-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1098 2022-07-09 20:34:21.759651 yamt-0.1.3.1/LICENSE
+-rw-r--r--   0        0        0      548 2023-06-30 22:28:17.999881 yamt-0.1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      327 2022-07-09 20:34:21.759651 yamt-0.1.3.1/README.md
+-rw-r--r--   0        0        0      641 2023-02-24 00:04:48.443064 yamt-0.1.3.1/yamt/__init__.py
+-rw-r--r--   0        0        0     4782 2022-11-14 20:24:48.298437 yamt-0.1.3.1/yamt/asyncio_misc.py
+-rw-r--r--   0        0        0     2810 2023-02-17 19:27:48.444386 yamt-0.1.3.1/yamt/asyncio_sync_primitives.py
+-rw-r--r--   0        0        0     8513 2023-03-28 05:21:29.388039 yamt-0.1.3.1/yamt/collections.py
+-rw-r--r--   0        0        0     2012 2022-11-12 16:33:43.019509 yamt-0.1.3.1/yamt/enum.py
+-rw-r--r--   0        0        0     5624 2023-06-30 22:27:06.701506 yamt-0.1.3.1/yamt/misc.py
+-rw-r--r--   0        0        0      193 2022-07-09 20:34:21.763604 yamt-0.1.3.1/yamt/typing.py
+-rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 yamt-0.1.3.1/setup.py
+-rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 yamt-0.1.3.1/PKG-INFO
```

### Comparing `yamt-0.1.3/LICENSE` & `yamt-0.1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yamt-0.1.3/pyproject.toml` & `yamt-0.1.3.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yamt"
-version = "0.1.3"
+version = "0.1.3.1"
 description = "yet another monkey toolkit"
 authors = ["lightmanLP <liteman1000@gmail.com>", "mikk357 <mikk357@yandex.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["utils", "tools", "misc"]
 
 [tool.poetry.urls]
```

### Comparing `yamt-0.1.3/yamt/__init__.py` & `yamt-0.1.3.1/yamt/__init__.py`

 * *Files identical despite different names*

### Comparing `yamt-0.1.3/yamt/asyncio_misc.py` & `yamt-0.1.3.1/yamt/asyncio_misc.py`

 * *Files identical despite different names*

### Comparing `yamt-0.1.3/yamt/asyncio_sync_primitives.py` & `yamt-0.1.3.1/yamt/asyncio_sync_primitives.py`

 * *Files identical despite different names*

### Comparing `yamt-0.1.3/yamt/collections.py` & `yamt-0.1.3.1/yamt/collections.py`

 * *Files identical despite different names*

### Comparing `yamt-0.1.3/yamt/enum.py` & `yamt-0.1.3.1/yamt/enum.py`

 * *Files identical despite different names*

### Comparing `yamt-0.1.3/yamt/misc.py` & `yamt-0.1.3.1/yamt/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,17 +189,18 @@
     __instance: SingletonT | None = None
 
     def __call__(cls: type[SingletonT], *args, **kwargs) -> SingletonT:
         if cls.__instance is None:
             cls.__instance = super().__call__(*args, **kwargs)
         return cls.__instance
 
-    def _wipe_singleton(self):
-        del self.__instance
-        self.__instance = None
+    @classmethod
+    def _wipe_singleton(cls):
+        del cls.__instance
+        cls.__instance = None
 
 
 class IterativeRandomizer(Generic[T]):
     data: list[T]
 
     def __init__(self, data: Iterable[T]) -> None:
         self.data = list(data)
```

### Comparing `yamt-0.1.3/setup.py` & `yamt-0.1.3.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['yamt']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'yamt',
-    'version': '0.1.3',
+    'version': '0.1.3.1',
     'description': 'yet another monkey toolkit',
     'long_description': '# yamt (yet another monkey toolkit)\n[![PyPI version](https://badge.fury.io/py/yamt.svg)](https://badge.fury.io/py/yamt)\n![PyPI downloads per mounth](https://img.shields.io/pypi/dm/yamt)\n![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/UT1C/yamt)\n\n## Installation\n```\npip install yamt\n```\n',
     'author': 'lightmanLP',
     'author_email': 'liteman1000@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `yamt-0.1.3/PKG-INFO` & `yamt-0.1.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamt
-Version: 0.1.3
+Version: 0.1.3.1
 Summary: yet another monkey toolkit
 License: MIT
 Keywords: utils,tools,misc
 Author: lightmanLP
 Author-email: liteman1000@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

