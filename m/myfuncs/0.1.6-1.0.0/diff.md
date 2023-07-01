# Comparing `tmp/myfuncs-0.1.6.tar.gz` & `tmp/myfuncs-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myfuncs-0.1.6.tar", last modified: Sat May 20 09:17:28 2023, max compression
+gzip compressed data, was "myfuncs-1.0.0.tar", last modified: Sat Jul  1 04:55:09 2023, max compression
```

## Comparing `myfuncs-0.1.6.tar` & `myfuncs-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-05-20 09:17:28.530643 myfuncs-0.1.6/
--rw-r--r--   0 work       (501) staff       (20)     1068 2023-05-13 16:42:37.000000 myfuncs-0.1.6/LICENSE
--rw-r--r--   0 work       (501) staff       (20)     2426 2023-05-20 09:17:28.530526 myfuncs-0.1.6/PKG-INFO
--rw-r--r--   0 work       (501) staff       (20)     1687 2023-05-13 21:07:45.000000 myfuncs-0.1.6/README.md
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-05-20 09:17:28.529927 myfuncs-0.1.6/myfuncs/
--rw-r--r--   0 work       (501) staff       (20)       21 2023-05-13 18:23:34.000000 myfuncs-0.1.6/myfuncs/__init__.py
--rw-r--r--   0 work       (501) staff       (20)     4331 2023-05-20 09:12:09.000000 myfuncs-0.1.6/myfuncs/funcs.py
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-05-20 09:17:28.530368 myfuncs-0.1.6/myfuncs.egg-info/
--rw-r--r--   0 work       (501) staff       (20)     2426 2023-05-20 09:17:28.000000 myfuncs-0.1.6/myfuncs.egg-info/PKG-INFO
--rw-r--r--   0 work       (501) staff       (20)      187 2023-05-20 09:17:28.000000 myfuncs-0.1.6/myfuncs.egg-info/SOURCES.txt
--rw-r--r--   0 work       (501) staff       (20)        1 2023-05-20 09:17:28.000000 myfuncs-0.1.6/myfuncs.egg-info/dependency_links.txt
--rw-r--r--   0 work       (501) staff       (20)        8 2023-05-20 09:17:28.000000 myfuncs-0.1.6/myfuncs.egg-info/top_level.txt
--rw-r--r--   0 work       (501) staff       (20)       38 2023-05-20 09:17:28.530681 myfuncs-0.1.6/setup.cfg
--rw-r--r--   0 work       (501) staff       (20)      916 2023-05-20 09:17:23.000000 myfuncs-0.1.6/setup.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-07-01 04:55:09.318271 myfuncs-1.0.0/
+-rw-r--r--   0 work       (501) staff       (20)     1068 2023-05-13 16:42:37.000000 myfuncs-1.0.0/LICENSE
+-rw-r--r--   0 work       (501) staff       (20)     2728 2023-07-01 04:55:09.318161 myfuncs-1.0.0/PKG-INFO
+-rw-r--r--   0 work       (501) staff       (20)     1989 2023-07-01 04:54:48.000000 myfuncs-1.0.0/README.md
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-07-01 04:55:09.317033 myfuncs-1.0.0/myfuncs/
+-rw-r--r--   0 work       (501) staff       (20)     1153 2023-07-01 04:37:50.000000 myfuncs-1.0.0/myfuncs/__init__.py
+-rw-r--r--   0 work       (501) staff       (20)     4470 2023-07-01 03:35:53.000000 myfuncs-1.0.0/myfuncs/funcs.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-07-01 04:55:09.317535 myfuncs-1.0.0/myfuncs.egg-info/
+-rw-r--r--   0 work       (501) staff       (20)     2728 2023-07-01 04:55:09.000000 myfuncs-1.0.0/myfuncs.egg-info/PKG-INFO
+-rw-r--r--   0 work       (501) staff       (20)      248 2023-07-01 04:55:09.000000 myfuncs-1.0.0/myfuncs.egg-info/SOURCES.txt
+-rw-r--r--   0 work       (501) staff       (20)        1 2023-07-01 04:55:09.000000 myfuncs-1.0.0/myfuncs.egg-info/dependency_links.txt
+-rw-r--r--   0 work       (501) staff       (20)       14 2023-07-01 04:55:09.000000 myfuncs-1.0.0/myfuncs.egg-info/top_level.txt
+-rw-r--r--   0 work       (501) staff       (20)       38 2023-07-01 04:55:09.318307 myfuncs-1.0.0/setup.cfg
+-rw-r--r--   0 work       (501) staff       (20)      916 2023-07-01 04:33:42.000000 myfuncs-1.0.0/setup.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-07-01 04:55:09.317904 myfuncs-1.0.0/tests/
+-rw-r--r--   0 work       (501) staff       (20)        0 2023-07-01 04:44:58.000000 myfuncs-1.0.0/tests/__init__.py
+-rwxr-xr-x   0 work       (501) staff       (20)     4015 2023-07-01 03:41:29.000000 myfuncs-1.0.0/tests/funcspy_tests.py
+-rw-r--r--   0 work       (501) staff       (20)      985 2023-07-01 04:40:15.000000 myfuncs-1.0.0/tests/main_tests.py
```

### Comparing `myfuncs-0.1.6/LICENSE` & `myfuncs-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `myfuncs-0.1.6/PKG-INFO` & `myfuncs-1.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfuncs
-Version: 0.1.6
+Version: 1.0.0
 Summary: Personal utility functions that I use across different codebases.
 Home-page: https://github.com/cc-d/myfuncs
 Author: Cary Carter
 Author-email: ccarterdev@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -16,83 +16,66 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # myfuncs
 
-This Python package, `myfuncs`, is a collection of personal utility functions created by myself. It is primarily intended for my personal use, providing easy access to frequently used functions across different projects and systems.
+`myfuncs` is a Python package that provides a set of utility functions designed to streamline your code and enhance efficiency across various projects and platforms.
 
 ## Installation
 
-You can install the package via pip:
+You can install `myfuncs` using pip:
 
 ```bash
 pip install myfuncs
 ```
 
-
 ## Usage
 
-Here's an example of how to use the functions provided by the `myfuncs` package:
-
-```python
-from myfuncs import valid_uuid, logf
 
-# Example usage of valid_uuid
-print(valid_uuid("550e8400-e29b-41d4-a716-446655440000"))  # True
+The functions in `myfuncs` can be imported as follows:
 
-# Example usage of logf
-import logging
-
-@logf(level=logging.DEBUG)
-def example_function(x):
-    return x * 2
+```python
+from myfuncs import runcmd
 
-print(example_function(4))  # 8
+# Example usage of the runcmd function
+result = runcmd("ls -l")
+print("Output:", result)
 ```
 
-You can update your `README.md` file to include information about the tests as follows:
-
----
-
-## Running Tests
-
-To run the tests for the `myfuncs` package, follow these steps:
+# Functions
 
-1\. Navigate to the root directory of the `myfuncs` package in your terminal.
+## `runcmd()`
 
-2\. Make sure you have the necessary dependencies installed in your virtual environment.
+Here, `runcmd` is a utility function that runs shell commands with optional output capture. It accepts additional arguments to customize the command execution process. This function is just one example of the utilities provided by `myfuncs`.
 
-3\. Run the tests by executing the following command:
+The `runcmd` function's parameters are:
 
-```bash
+- `cmd` (str): The command to be executed.
+- `output` (bool, optional): Specifies whether to capture and return the output of the command. Defaults to True.
+- `*args`: Additional positional arguments passed to `subprocess.run()`.
+- `**kwargs`: Additional keyword arguments passed to `subprocess.run()`.
 
-python -m unittest tests.myfuncs_tests
+----
 
-```
+## Running Tests
 
-If the tests run successfully, you should see output similar to the following:
+The `myfuncs` package includes a test suite to verify the operation of its functions. To run the tests:
 
+```bash
+python -m unittest tests/*.py
 ```
 
-..DEBUG:myfuncs.funcs:valid_uuid() | ('123e4567-e89b-12d3-a456-426614174000',) {}
-
-DEBUG:myfuncs.funcs:valid_uuid() 0.00018s | True
+This command executes all Python files (`*.py`) in the `tests` directory. Successful completion signifies that the functions are working as intended.
 
-DEBUG:myfuncs.funcs:valid_uuid() | ('123e4567-e89b-12d3-a456-42661417400',) {}
+## Documentation
 
-DEBUG:myfuncs.funcs:valid_uuid() 0.00002s | False
+In-depth documentation can be accessed in the source code within docstrings. For future developments and detailed examples, please refer to the `myfuncs` [GitHub repository](https://github.com/cc-d/myfuncs).
 
-.
+## Contributing
 
-----------------------------------------------------------------------
-
-Ran 3 tests in 0.001s
-
-OK
-
-```
+Contributions to `myfuncs` are welcomed. If you encounter any issues or have suggestions for improvements, please open an issue on the [GitHub repository](https://github.com/cc-d/myfuncs).
 
-This output indicates that all the tests have passed.
+## License
 
----
+This project is licensed under the MIT License. See the [LICENSE](https://github.com/cc-d/myfuncs/blob/main/LICENSE) file for more details.
```

### Comparing `myfuncs-0.1.6/myfuncs/funcs.py` & `myfuncs-1.0.0/myfuncs/funcs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+legacy file, kept around for off chance somebody is relying
+on backwards compatability, all functionality should go in __init__.py
+"""
 import os
 import re
 import time
 import inspect
 import random
 import string
 from datetime import datetime
```

### Comparing `myfuncs-0.1.6/myfuncs.egg-info/PKG-INFO` & `myfuncs-1.0.0/myfuncs.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfuncs
-Version: 0.1.6
+Version: 1.0.0
 Summary: Personal utility functions that I use across different codebases.
 Home-page: https://github.com/cc-d/myfuncs
 Author: Cary Carter
 Author-email: ccarterdev@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -16,83 +16,66 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # myfuncs
 
-This Python package, `myfuncs`, is a collection of personal utility functions created by myself. It is primarily intended for my personal use, providing easy access to frequently used functions across different projects and systems.
+`myfuncs` is a Python package that provides a set of utility functions designed to streamline your code and enhance efficiency across various projects and platforms.
 
 ## Installation
 
-You can install the package via pip:
+You can install `myfuncs` using pip:
 
 ```bash
 pip install myfuncs
 ```
 
-
 ## Usage
 
-Here's an example of how to use the functions provided by the `myfuncs` package:
-
-```python
-from myfuncs import valid_uuid, logf
 
-# Example usage of valid_uuid
-print(valid_uuid("550e8400-e29b-41d4-a716-446655440000"))  # True
+The functions in `myfuncs` can be imported as follows:
 
-# Example usage of logf
-import logging
-
-@logf(level=logging.DEBUG)
-def example_function(x):
-    return x * 2
+```python
+from myfuncs import runcmd
 
-print(example_function(4))  # 8
+# Example usage of the runcmd function
+result = runcmd("ls -l")
+print("Output:", result)
 ```
 
-You can update your `README.md` file to include information about the tests as follows:
-
----
-
-## Running Tests
-
-To run the tests for the `myfuncs` package, follow these steps:
+# Functions
 
-1\. Navigate to the root directory of the `myfuncs` package in your terminal.
+## `runcmd()`
 
-2\. Make sure you have the necessary dependencies installed in your virtual environment.
+Here, `runcmd` is a utility function that runs shell commands with optional output capture. It accepts additional arguments to customize the command execution process. This function is just one example of the utilities provided by `myfuncs`.
 
-3\. Run the tests by executing the following command:
+The `runcmd` function's parameters are:
 
-```bash
+- `cmd` (str): The command to be executed.
+- `output` (bool, optional): Specifies whether to capture and return the output of the command. Defaults to True.
+- `*args`: Additional positional arguments passed to `subprocess.run()`.
+- `**kwargs`: Additional keyword arguments passed to `subprocess.run()`.
 
-python -m unittest tests.myfuncs_tests
+----
 
-```
+## Running Tests
 
-If the tests run successfully, you should see output similar to the following:
+The `myfuncs` package includes a test suite to verify the operation of its functions. To run the tests:
 
+```bash
+python -m unittest tests/*.py
 ```
 
-..DEBUG:myfuncs.funcs:valid_uuid() | ('123e4567-e89b-12d3-a456-426614174000',) {}
-
-DEBUG:myfuncs.funcs:valid_uuid() 0.00018s | True
+This command executes all Python files (`*.py`) in the `tests` directory. Successful completion signifies that the functions are working as intended.
 
-DEBUG:myfuncs.funcs:valid_uuid() | ('123e4567-e89b-12d3-a456-42661417400',) {}
+## Documentation
 
-DEBUG:myfuncs.funcs:valid_uuid() 0.00002s | False
+In-depth documentation can be accessed in the source code within docstrings. For future developments and detailed examples, please refer to the `myfuncs` [GitHub repository](https://github.com/cc-d/myfuncs).
 
-.
+## Contributing
 
-----------------------------------------------------------------------
-
-Ran 3 tests in 0.001s
-
-OK
-
-```
+Contributions to `myfuncs` are welcomed. If you encounter any issues or have suggestions for improvements, please open an issue on the [GitHub repository](https://github.com/cc-d/myfuncs).
 
-This output indicates that all the tests have passed.
+## License
 
----
+This project is licensed under the MIT License. See the [LICENSE](https://github.com/cc-d/myfuncs/blob/main/LICENSE) file for more details.
```

### Comparing `myfuncs-0.1.6/setup.py` & `myfuncs-1.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfuncs',
-    version='0.1.6',
+    version='1.0.0',
     packages=find_packages(),
     install_requires=[],
     author='Cary Carter',
     author_email='ccarterdev@gmail.com',
     description='Personal utility functions that I use across different codebases.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

