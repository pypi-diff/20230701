# Comparing `tmp/archtool-0.1.0.tar.gz` & `tmp/archtool-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archtool-0.1.0.tar", last modified: Fri Jun 30 17:10:36 2023, max compression
+gzip compressed data, was "archtool-0.1.5.tar", last modified: Sat Jul  1 11:31:13 2023, max compression
```

## Comparing `archtool-0.1.0.tar` & `archtool-0.1.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 godmod    (1000) godmod    (1000)        0 2023-06-30 17:10:36.966595 archtool-0.1.0/
--rw-rw-r--   0 godmod    (1000) godmod    (1000)      692 2023-06-30 17:10:36.966595 archtool-0.1.0/PKG-INFO
--rw-rw-r--   0 godmod    (1000) godmod    (1000)      984 2023-06-30 16:42:50.000000 archtool-0.1.0/README.md
-drwxrwxr-x   0 godmod    (1000) godmod    (1000)        0 2023-06-30 17:10:36.958598 archtool-0.1.0/archtool.egg-info/
--rw-rw-r--   0 godmod    (1000) godmod    (1000)      692 2023-06-30 17:10:36.000000 archtool-0.1.0/archtool.egg-info/PKG-INFO
--rw-rw-r--   0 godmod    (1000) godmod    (1000)      668 2023-06-30 17:10:36.000000 archtool-0.1.0/archtool.egg-info/SOURCES.txt
--rw-rw-r--   0 godmod    (1000) godmod    (1000)        1 2023-06-30 17:10:36.000000 archtool-0.1.0/archtool.egg-info/dependency_links.txt
--rw-rw-r--   0 godmod    (1000) godmod    (1000)        1 2023-06-30 17:09:53.000000 archtool-0.1.0/archtool.egg-info/not-zip-safe
--rw-rw-r--   0 godmod    (1000) godmod    (1000)        9 2023-06-30 17:10:36.000000 archtool-0.1.0/archtool.egg-info/top_level.txt
-drwxrwxr-x   0 godmod    (1000) godmod    (1000)        0 2023-06-30 17:10:36.958598 archtool-0.1.0/injector/
--rw-rw-r--   0 godmod    (1000) godmod    (1000)        0 2023-06-10 11:21:50.000000 archtool-0.1.0/injector/__init__.py
-drwxrwxr-x   0 godmod    (1000) godmod    (1000)        0 2023-06-30 17:10:36.962596 archtool-0.1.0/injector/components/
--rw-rw-r--   0 godmod    (1000) godmod    (1000)        0 2023-06-27 12:15:15.000000 archtool-0.1.0/injector/components/__init__.py
--rw-rw-r--   0 godmod    (1000) godmod    (1000)      653 2023-06-27 12:15:15.000000 archtool-0.1.0/injector/components/default_component.py
--rw-rw-r--   0 godmod    (1000) godmod    (1000)     4778 2023-06-27 12:15:15.000000 archtool-0.1.0/injector/dependecy_injector.py
--rw-rw-r--   0 godmod    (1000) godmod    (1000)      358 2023-06-15 20:16:42.000000 archtool-0.1.0/injector/exceptions.py
--rw-rw-r--   0 godmod    (1000) godmod    (1000)     2245 2023-06-23 10:36:36.000000 archtool-0.1.0/injector/global_types.py
-drwxrwxr-x   0 godmod    (1000) godmod    (1000)        0 2023-06-30 17:10:36.962596 archtool-0.1.0/injector/interfaces/
--rw-rw-r--   0 godmod    (1000) godmod    (1000)       93 2023-06-27 12:15:15.000000 archtool-0.1.0/injector/interfaces/__init__.py
--rw-rw-r--   0 godmod    (1000) godmod    (1000)      851 2023-06-27 12:15:15.000000 archtool-0.1.0/injector/interfaces/dependecy_injector.py
--rw-rw-r--   0 godmod    (1000) godmod    (1000)      464 2023-06-27 12:15:15.000000 archtool-0.1.0/injector/interfaces/di_layer.py
--rw-rw-r--   0 godmod    (1000) godmod    (1000)      761 2023-06-13 13:21:42.000000 archtool-0.1.0/injector/interfaces/layer.py
-drwxrwxr-x   0 godmod    (1000) godmod    (1000)        0 2023-06-30 17:10:36.966595 archtool-0.1.0/injector/layers/
--rw-rw-r--   0 godmod    (1000) godmod    (1000)       34 2023-06-27 12:15:15.000000 archtool-0.1.0/injector/layers/__init__.py
--rw-rw-r--   0 godmod    (1000) godmod    (1000)      509 2023-06-29 10:42:15.000000 archtool-0.1.0/injector/layers/default_layer_interfaces.py
--rw-rw-r--   0 godmod    (1000) godmod    (1000)     2065 2023-06-27 12:15:15.000000 archtool-0.1.0/injector/layers/default_layers.py
--rw-rw-r--   0 godmod    (1000) godmod    (1000)     3601 2023-06-27 12:15:15.000000 archtool-0.1.0/injector/layers/di_basic_layer.py
--rw-rw-r--   0 godmod    (1000) godmod    (1000)     9125 2023-06-27 12:15:15.000000 archtool-0.1.0/injector/utils.py
--rw-rw-r--   0 godmod    (1000) godmod    (1000)       84 2023-06-15 21:49:35.000000 archtool-0.1.0/pyproject.toml
--rw-rw-r--   0 godmod    (1000) godmod    (1000)      768 2023-06-30 17:10:36.966595 archtool-0.1.0/setup.cfg
--rw-rw-r--   0 godmod    (1000) godmod    (1000)     1639 2023-06-21 11:41:25.000000 archtool-0.1.0/setup.py
+drwxrwxr-x   0 godmod    (1000) godmod    (1000)        0 2023-07-01 11:31:13.672704 archtool-0.1.5/
+-rw-rw-r--   0 godmod    (1000) godmod    (1000)      692 2023-07-01 11:31:13.672704 archtool-0.1.5/PKG-INFO
+-rw-rw-r--   0 godmod    (1000) godmod    (1000)      420 2023-07-01 11:28:08.000000 archtool-0.1.5/README.md
+drwxrwxr-x   0 godmod    (1000) godmod    (1000)        0 2023-07-01 11:31:13.668704 archtool-0.1.5/archtool/
+-rw-rw-r--   0 godmod    (1000) godmod    (1000)        0 2023-07-01 11:22:17.000000 archtool-0.1.5/archtool/__init__.py
+drwxrwxr-x   0 godmod    (1000) godmod    (1000)        0 2023-07-01 11:31:13.672704 archtool-0.1.5/archtool/components/
+-rw-rw-r--   0 godmod    (1000) godmod    (1000)        0 2023-07-01 11:22:17.000000 archtool-0.1.5/archtool/components/__init__.py
+-rw-rw-r--   0 godmod    (1000) godmod    (1000)      653 2023-07-01 11:22:17.000000 archtool-0.1.5/archtool/components/default_component.py
+-rw-rw-r--   0 godmod    (1000) godmod    (1000)     5281 2023-07-01 11:22:17.000000 archtool-0.1.5/archtool/dependecy_injector.py
+-rw-rw-r--   0 godmod    (1000) godmod    (1000)      358 2023-07-01 11:22:17.000000 archtool-0.1.5/archtool/exceptions.py
+-rw-rw-r--   0 godmod    (1000) godmod    (1000)     1984 2023-07-01 11:22:17.000000 archtool-0.1.5/archtool/global_types.py
+drwxrwxr-x   0 godmod    (1000) godmod    (1000)        0 2023-07-01 11:31:13.672704 archtool-0.1.5/archtool/interfaces/
+-rw-rw-r--   0 godmod    (1000) godmod    (1000)       93 2023-07-01 11:22:17.000000 archtool-0.1.5/archtool/interfaces/__init__.py
+-rw-rw-r--   0 godmod    (1000) godmod    (1000)      851 2023-07-01 11:22:17.000000 archtool-0.1.5/archtool/interfaces/dependecy_injector.py
+-rw-rw-r--   0 godmod    (1000) godmod    (1000)      464 2023-07-01 11:22:17.000000 archtool-0.1.5/archtool/interfaces/di_layer.py
+-rw-rw-r--   0 godmod    (1000) godmod    (1000)      761 2023-07-01 11:22:17.000000 archtool-0.1.5/archtool/interfaces/layer.py
+drwxrwxr-x   0 godmod    (1000) godmod    (1000)        0 2023-07-01 11:31:13.672704 archtool-0.1.5/archtool/layers/
+-rw-rw-r--   0 godmod    (1000) godmod    (1000)       34 2023-07-01 11:22:17.000000 archtool-0.1.5/archtool/layers/__init__.py
+-rw-rw-r--   0 godmod    (1000) godmod    (1000)      509 2023-07-01 11:22:17.000000 archtool-0.1.5/archtool/layers/default_layer_interfaces.py
+-rw-rw-r--   0 godmod    (1000) godmod    (1000)     2065 2023-07-01 11:22:17.000000 archtool-0.1.5/archtool/layers/default_layers.py
+-rw-rw-r--   0 godmod    (1000) godmod    (1000)     3654 2023-07-01 11:22:17.000000 archtool-0.1.5/archtool/layers/di_basic_layer.py
+-rw-rw-r--   0 godmod    (1000) godmod    (1000)     9125 2023-07-01 11:22:17.000000 archtool-0.1.5/archtool/utils.py
+drwxrwxr-x   0 godmod    (1000) godmod    (1000)        0 2023-07-01 11:31:13.672704 archtool-0.1.5/archtool.egg-info/
+-rw-rw-r--   0 godmod    (1000) godmod    (1000)      692 2023-07-01 11:31:13.000000 archtool-0.1.5/archtool.egg-info/PKG-INFO
+-rw-rw-r--   0 godmod    (1000) godmod    (1000)      668 2023-07-01 11:31:13.000000 archtool-0.1.5/archtool.egg-info/SOURCES.txt
+-rw-rw-r--   0 godmod    (1000) godmod    (1000)        1 2023-07-01 11:31:13.000000 archtool-0.1.5/archtool.egg-info/dependency_links.txt
+-rw-rw-r--   0 godmod    (1000) godmod    (1000)        1 2023-07-01 11:22:17.000000 archtool-0.1.5/archtool.egg-info/not-zip-safe
+-rw-rw-r--   0 godmod    (1000) godmod    (1000)        9 2023-07-01 11:31:13.000000 archtool-0.1.5/archtool.egg-info/top_level.txt
+-rw-rw-r--   0 godmod    (1000) godmod    (1000)       84 2023-06-15 21:49:35.000000 archtool-0.1.5/pyproject.toml
+-rw-rw-r--   0 godmod    (1000) godmod    (1000)      768 2023-07-01 11:31:13.676704 archtool-0.1.5/setup.cfg
+-rw-rw-r--   0 godmod    (1000) godmod    (1000)     1639 2023-06-21 11:41:25.000000 archtool-0.1.5/setup.py
```

### Comparing `archtool-0.1.0/PKG-INFO` & `archtool-0.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: archtool
-Version: 0.1.0
-Home-page: https://github.com/0nliner/injector
+Version: 0.1.5
+Home-page: https://github.com/0nliner/archtool
 Author: Aleksandr Chudaikin
 Author-email: aleksandrchudaikindev@gmail.com
 License: MIT
 Keywords: ''
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `archtool-0.1.0/archtool.egg-info/PKG-INFO` & `archtool-0.1.5/archtool.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: archtool
-Version: 0.1.0
-Home-page: https://github.com/0nliner/injector
+Version: 0.1.5
+Home-page: https://github.com/0nliner/archtool
 Author: Aleksandr Chudaikin
 Author-email: aleksandrchudaikindev@gmail.com
 License: MIT
 Keywords: ''
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `archtool-0.1.0/injector/components/default_component.py` & `archtool-0.1.5/archtool/components/default_component.py`

 * *Files identical despite different names*

### Comparing `archtool-0.1.0/injector/dependecy_injector.py` & `archtool-0.1.5/archtool/dependecy_injector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,80 @@
 from typing import List, Dict
 
 from .exceptions import (DependecyDuplicate,
                          DependecyDoesNotRegistred
                          )
 
-from .interfaces import (DependecyInjectorInterface,
-                         LayerInterface
-                         )
+from .interfaces import DependecyInjectorInterface
 
-from injector.layers.default_layers import default_layers
-from injector.layers import Layer
-from injector.global_types import (AppModules,
+from archtool.layers.default_layers import default_layers
+from archtool.layers.di_basic_layer import Layer
+from archtool.components.default_component import ComponentPattern
+from archtool.global_types import (AppModules,
                                    ContainerT,
                                    DEPENDENCY_KEY)
 
-from injector.utils import (get_dependencies,
+from archtool.utils import (get_dependencies,
                             serialize_dep_key,
                             get_all_interfaces_and_realizations)
 
 
 # TODO: нахерачить документацию по тому как этим пользоваться
 # TODO: валидации:
 #       однонаправленность импортов
 
 class DependecyInjector(DependecyInjectorInterface):
     def __init__(self,
                  modules_list: AppModules,
-                 layers: List[LayerInterface] = None):
+                 layers: List[Layer] = None):
 
         self.modules_list = modules_list
-        self.layers = layers if layers else default_layers
         # инициализируем классы слоёв
         # TODO: позже нужно вынести инициализацию.
         #       Это должен делать пользователь
-        self.layers = [layer() for layer in self.layers]
         self._dependencies: Dict[DEPENDENCY_KEY, object] = {}
 
+        self.layers = layers if layers else default_layers
+        self._layers = []
+        for layer in self.layers:
+            initialized_layer = layer()
+            self._layers.append(initialized_layer)
+        self.layers = self._layers
+
     def inject(self):
         for layer in self.layers:
             if issubclass(type(layer), Layer):
-                # TODO: сделать аннотирование на components
-                # TODO: добавить __iter__ на Components класс
-                for component_group in layer.component_groups:
+                for component_pattern in layer.component_groups:
+                    # достаём модули, которые не игнорируют слой
+                    modules_to_interact = self._exclude_ignored_modules(
+                        component_pattern=component_pattern)
+
                     component_group_deps = get_all_interfaces_and_realizations(
-                        app_modules=self.modules_list,
-                        name_pattern=component_group.module_name_regex,
-                        superclass=component_group.superclass)
+                        app_modules=modules_to_interact,
+                        name_pattern=component_pattern.module_name_regex,
+                        superclass=component_pattern.superclass)
 
                     # добавляем зависимости слоя в глобальные зависимости
                     for dep_key, dep_class in component_group_deps.items():
                         # инициализируем классы, подставляем как зависимость
                         dep_instance = dep_class()
                         self._reg_dependecy(key=dep_key,
                                             value=dep_instance)
 
         # инжектим
         for dep_interface, dep_instance in self._dependencies.items():
             self._inject_dependencies(container=dep_instance)
 
+    def _exclude_ignored_modules(self, component_pattern: ComponentPattern):
+        filtered_modules = []
+        for module in self.modules_list:
+            if component_pattern not in module.ignore:
+                filtered_modules.append(module)
+        return filtered_modules
+
     def _inject_dependencies(self, container: ContainerT) -> None:
         """
         Внедряет зависимости
 
         ARGS:
         container - объект, в который встраиваем зависимости
         """
```

### Comparing `archtool-0.1.0/injector/global_types.py` & `archtool-0.1.5/archtool/global_types.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,20 +32,15 @@
 class AppModule:
     """
     ARGS:
     - import_path: питонячий импорт модуля относительно BASE_DIR
     """
     import_path: str
     # TODO: перенести логику игнора слоёв
-    ignore_views: bool = field(default=False)
-    ignore_service_interfaces: bool = field(default=False)
-    ignore_repositories_interfaces: bool = field(default=False)
-    ignore_repositories: bool = field(default=False)
-    ignore_services: bool = field(default=False)
-    is_legacy: bool = field(default=True)
+    ignore: List[Any] = field(default_factory=list)
 
     # TODO: написать отдельную функцию валидации модуля,
     # вынести её отдельно
     def _validate_module(self):
         """
         Производит проверки:
             - существует ли модуль
```

### Comparing `archtool-0.1.0/injector/interfaces/dependecy_injector.py` & `archtool-0.1.5/archtool/interfaces/dependecy_injector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from injector.global_types import AppModules, DEPENDENCY_KEY
+from archtool.global_types import AppModules, DEPENDENCY_KEY
 
 
 class DependecyInjectorInterface(ABC):
     @abstractmethod
     def __init__(self,
                  modules_list: AppModules):
         """
```

### Comparing `archtool-0.1.0/injector/interfaces/layer.py` & `archtool-0.1.5/archtool/interfaces/layer.py`

 * *Files identical despite different names*

### Comparing `archtool-0.1.0/injector/layers/default_layers.py` & `archtool-0.1.5/archtool/layers/default_layers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from injector.components.default_component import ComponentPattern
-from injector.layers import Layer
+from archtool.components.default_component import ComponentPattern
+from archtool.layers import Layer
 
-from injector.layers.default_layer_interfaces import (ABCView,
+from archtool.layers.default_layer_interfaces import (ABCView,
                                                       ABCService,
                                                       ABCRepo,
                                                       ABCController)
 
 # TODO:
 # class ComponentsModule:
 #     """
```

### Comparing `archtool-0.1.0/injector/layers/di_basic_layer.py` & `archtool-0.1.5/archtool/layers/di_basic_layer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import abstractmethod
 from typing import List, Generator
 from inspect import isclass
 
-from injector.components.default_component import ComponentPatternBase
+from archtool.components.default_component import ComponentPatternBase
 
 
 class ValidationError(Exception):
     ...
 
 
 def is_component_pattern_base(obj):
@@ -75,14 +75,15 @@
         components_instance = components_class()
 
         module = attrs.pop("__module__")
         depends_on = attrs.pop("depends_on")
 
         new_attrs = {"__module__": module,
                      "component_groups": components_instance,
+                     "Components": components_class,
                      "depends_on": depends_on}
 
         new_layer_class = super_new(cls, name, bases, new_attrs)
         new_layer_class.__new__ = super(object).__new__
         return new_layer_class
 
     @classmethod
```

### Comparing `archtool-0.1.0/injector/utils.py` & `archtool-0.1.5/archtool/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from inspect import isclass, isabstract, getfile, getmro
 from importlib import import_module
 from typing import List, Callable
 from functools import singledispatch
 from re import sub
 
 from pathlib import Path
-from injector.exceptions import (CheckFailedException,
+from archtool.exceptions import (CheckFailedException,
                                  MultipleRealizationsException,
                                  RealizationNotFount)
-from injector.global_types import (
+from archtool.global_types import (
         Dependecy,
         ContainerT,
         DependeciesT,
         AppModule,
         AppModules,
         DEPENDENCY_KEY,
         InterfaceT)
```

### Comparing `archtool-0.1.0/setup.cfg` & `archtool-0.1.5/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 name = archtool
-version = 0.1.0
+version = 0.1.5
 license = MIT
 author = Aleksandr Chudaikin
 author_email = aleksandrchudaikindev@gmail.com
 description_file = file: README.md
-url = https://github.com/0nliner/injector
+url = https://github.com/0nliner/archtool
 keywords = ''
 install_requires = []
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3 :: Only
```

### Comparing `archtool-0.1.0/setup.py` & `archtool-0.1.5/setup.py`

 * *Files identical despite different names*

