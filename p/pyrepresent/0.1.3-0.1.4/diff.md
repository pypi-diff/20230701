# Comparing `tmp/pyrepresent-0.1.3.tar.gz` & `tmp/pyrepresent-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrepresent-0.1.3.tar", last modified: Fri Jun 30 19:49:51 2023, max compression
+gzip compressed data, was "pyrepresent-0.1.4.tar", last modified: Sat Jul  1 08:08:55 2023, max compression
```

## Comparing `pyrepresent-0.1.3.tar` & `pyrepresent-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 19:49:51.980747 pyrepresent-0.1.3/
--rw-rw-rw-   0        0        0      115 2023-06-30 19:49:51.000000 pyrepresent-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     5268 2023-06-30 19:49:51.979775 pyrepresent-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4389 2023-03-21 18:58:55.000000 pyrepresent-0.1.3/README.md
--rw-rw-rw-   0        0        0    12965 2023-03-21 19:21:52.000000 pyrepresent-0.1.3/build.py
--rw-rw-rw-   0        0        0      715 2023-06-30 18:38:22.000000 pyrepresent-0.1.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-30 19:49:51.973760 pyrepresent-0.1.3/pyrepresent.egg-info/
--rw-rw-rw-   0        0        0     5268 2023-06-30 19:49:51.000000 pyrepresent-0.1.3/pyrepresent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-06-30 19:49:51.000000 pyrepresent-0.1.3/pyrepresent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 19:49:51.000000 pyrepresent-0.1.3/pyrepresent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-06-30 19:49:51.000000 pyrepresent-0.1.3/pyrepresent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-30 19:49:51.000000 pyrepresent-0.1.3/pyrepresent.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-30 19:49:51.978749 pyrepresent-0.1.3/represent/
--rw-rw-rw-   0        0        0       85 2023-03-09 09:17:11.000000 pyrepresent-0.1.3/represent/__init__.py
--rw-rw-rw-   0        0        0     5875 2023-03-09 09:10:13.000000 pyrepresent-0.1.3/represent/base.py
--rw-rw-rw-   0        0        0      202 2023-03-09 09:18:08.000000 pyrepresent-0.1.3/represent/document.py
--rw-rw-rw-   0        0        0     2133 2023-05-15 13:38:04.000000 pyrepresent-0.1.3/represent/indentation.py
--rw-rw-rw-   0        0        0    19907 2023-06-30 19:49:10.000000 pyrepresent-0.1.3/represent/object.py
--rw-rw-rw-   0        0        0    20997 2023-06-30 19:26:36.000000 pyrepresent-0.1.3/represent/structures.py
--rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.1.3/requirements-dev.txt
--rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.1.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 19:49:51.980747 pyrepresent-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-06-30 18:38:17.000000 pyrepresent-0.1.3/setup.py
--rw-rw-rw-   0        0        0     1028 2023-06-30 19:49:35.000000 pyrepresent-0.1.3/test.py
+drwxrwxrwx   0        0        0        0 2023-07-01 08:08:55.463804 pyrepresent-0.1.4/
+-rw-rw-rw-   0        0        0      115 2023-07-01 08:08:55.000000 pyrepresent-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     5268 2023-07-01 08:08:55.463804 pyrepresent-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4389 2023-03-21 18:58:55.000000 pyrepresent-0.1.4/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pyrepresent-0.1.4/build.py
+-rw-rw-rw-   0        0        0      715 2023-07-01 08:08:45.000000 pyrepresent-0.1.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-01 08:08:55.459803 pyrepresent-0.1.4/pyrepresent.egg-info/
+-rw-rw-rw-   0        0        0     5268 2023-07-01 08:08:55.000000 pyrepresent-0.1.4/pyrepresent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2023-07-01 08:08:55.000000 pyrepresent-0.1.4/pyrepresent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 08:08:55.000000 pyrepresent-0.1.4/pyrepresent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-01 08:08:55.000000 pyrepresent-0.1.4/pyrepresent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-01 08:08:55.000000 pyrepresent-0.1.4/pyrepresent.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 08:08:55.462804 pyrepresent-0.1.4/represent/
+-rw-rw-rw-   0        0        0       85 2023-03-09 09:17:11.000000 pyrepresent-0.1.4/represent/__init__.py
+-rw-rw-rw-   0        0        0     2133 2023-05-15 13:38:04.000000 pyrepresent-0.1.4/represent/indentation.py
+-rw-rw-rw-   0        0        0    20230 2023-07-01 08:07:33.000000 pyrepresent-0.1.4/represent/object.py
+-rw-rw-rw-   0        0        0    21509 2023-07-01 08:08:23.000000 pyrepresent-0.1.4/represent/structures.py
+-rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.1.4/requirements-dev.txt
+-rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.1.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 08:08:55.464804 pyrepresent-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-07-01 08:08:41.000000 pyrepresent-0.1.4/setup.py
+-rw-rw-rw-   0        0        0     1028 2023-06-30 19:49:35.000000 pyrepresent-0.1.4/test.py
```

### Comparing `pyrepresent-0.1.3/PKG-INFO` & `pyrepresent-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.1.3
+Version: 0.1.4
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.1.3/README.md` & `pyrepresent-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.1.3/build.py` & `pyrepresent-0.1.4/build.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,16 +88,14 @@
                     continue
                 # end if
 
                 if (
                     (len(parts) > 2) and
                     (part in ("--extra-index-url", "--index-url", "--find-links"))
                 ):
-                    print(i, parts, line)
-
                     if i == 0:
                         name = parts[-1]
 
                     else:
                         name = parts[0]
                     # end if
```

### Comparing `pyrepresent-0.1.3/pyproject.toml` & `pyrepresent-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pyrepresent'
-version = '0.1.3'
+version = '0.1.4'
 description = 'A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pyrepresent-0.1.3/pyrepresent.egg-info/PKG-INFO` & `pyrepresent-0.1.4/pyrepresent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.1.3
+Version: 0.1.4
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.1.3/represent/indentation.py` & `pyrepresent-0.1.4/represent/indentation.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.1.3/represent/object.py` & `pyrepresent-0.1.4/represent/object.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,59 @@
 # object.py
 
 import inspect
 import builtins
 import types
+import six
 import datetime as dt
 from itertools import chain
 from typing import (
     Any, Optional, Union, Iterable, Type, Dict, Tuple
 )
 
-from represent.base import is_bound_method
+import pandas as pd
+import numpy as np
+
 from represent.indentation import indent
 from represent.structures import (
     structures, HiddenStructure, StringWrapper, colorize,
     CircularReferenceStructure, DataStructure, TypeStructure,
     ObjectStructure, FunctionStructure, SetStructure,
     ListStructure, DictStructure
 )
 
-import pandas as pd
-import numpy as np
-
 __all__ = [
     "to_string",
     "BaseModel",
     "Modifiers",
     "unwrap",
     "DataContainer",
     "HashableDict",
     "HashableSet",
     "HashableList",
     "FrozenHashable"
 ]
 
+def is_bound_method(value: Any, /) -> bool:
+    """
+    Checks whether an object is a bound method or not.
+
+    :param value: The object to check.
+
+    :return: The boolean value.
+    """
+
+    try:
+        return six.get_method_self(value) is not None
+
+    except AttributeError:
+        return False
+    # end try
+# end is_bound_method
+
 class DataContainer(dict):
     """A class to represent a data container."""
 
     def __setattr__(self, key: str, value: Any) -> None:
         """
         Sets the attribute.
```

### Comparing `pyrepresent-0.1.3/represent/structures.py` & `pyrepresent-0.1.4/represent/structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # structures.py
 
 import datetime as dt
 import types
+import subprocess
+import os
 from typing import Union, Any, Optional, Callable
 from functools import wraps
 
 from colorama import Fore, Style
 
 import pandas as pd
 import numpy as np
 
-from represent.base import is_proxy_process
-
 __all__ = [
     "Colors",
     "DataStructure",
     "DataStructureMeta",
     "DictStructure",
     "HiddenStructure",
     "SetStructure",
@@ -28,15 +28,37 @@
     "colorize",
     "decolorize",
     "TypeStructure",
     "ObjectStructure",
     "FunctionStructure"
 ]
 
-Args = Kwargs = Any
+def is_proxy_process() -> bool:
+    """
+    Returns True if the process is running from an IDE.
+
+    :return: The boolean value.
+    """
+
+    shells = {
+        "bash.exe", "cmd.exe", "powershell.exe",
+        "WindowsTerminal.exe"
+    }
+
+    s = subprocess.check_output(
+        [
+            "tasklist", "/v", "/fo", "csv",
+            "/nh", "/fi", f"PID eq {os.getppid()}"
+        ]
+    )
+
+    entry = str(s).strip().strip('"').strip('b\'"').split('","')
+
+    return not (entry and (entry[0] in shells))
+# end is_proxy_process
 
 class Colors:
     """A class to represent colors."""
 
     RED = "$RED$"
     BLACK = "$BLACK$"
     GREEN = "$GREEN$"
@@ -323,15 +345,15 @@
 
     :param constructor: The init method of the class.
 
     :return: The wrapped init method.
     """
 
     @wraps(constructor)
-    def __str__(*args: Args, **kwargs: Kwargs) -> str:
+    def __str__(*args: Any, **kwargs: Any) -> str:
         """
         Defines the class attributes to wrap the init method.
 
         :param args: Any positional arguments.
         :param kwargs: Any keyword arguments
 
         :returns: The model object.
```

### Comparing `pyrepresent-0.1.3/setup.py` & `pyrepresent-0.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "test.py"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='pyrepresent',
-        version='0.1.3',
+        version='0.1.4',
         description=(
             "A module for object and model representations as strings, "
             "with vast configurations, colors, hidden and protected values, "
             "assignment operations, memory addresses and more."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `pyrepresent-0.1.3/test.py` & `pyrepresent-0.1.4/test.py`

 * *Files identical despite different names*

