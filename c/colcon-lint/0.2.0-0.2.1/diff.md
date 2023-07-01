# Comparing `tmp/colcon-lint-0.2.0.tar.gz` & `tmp/colcon-lint-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colcon-lint-0.2.0.tar", last modified: Thu Jun  1 15:00:38 2023, max compression
+gzip compressed data, was "colcon-lint-0.2.1.tar", last modified: Sat Jul  1 04:37:50 2023, max compression
```

## Comparing `colcon-lint-0.2.0.tar` & `colcon-lint-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 15:00:38.446222 colcon-lint-0.2.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-01 15:00:15.000000 colcon-lint-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1547 2023-06-01 15:00:38.446222 colcon-lint-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1082 2023-06-01 15:00:15.000000 colcon-lint-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 15:00:38.446222 colcon-lint-0.2.0/colcon_lint/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-01 15:00:15.000000 colcon-lint-0.2.0/colcon_lint/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 15:00:38.446222 colcon-lint-0.2.0/colcon_lint/verb/
--rw-r--r--   0 root         (0) root         (0)      581 2023-06-01 15:00:15.000000 colcon-lint-0.2.0/colcon_lint/verb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14921 2023-06-01 15:00:15.000000 colcon-lint-0.2.0/colcon_lint/verb/lint_depends.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 15:00:38.446222 colcon-lint-0.2.0/colcon_lint.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1547 2023-06-01 15:00:38.000000 colcon-lint-0.2.0/colcon_lint.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      412 2023-06-01 15:00:38.000000 colcon-lint-0.2.0/colcon_lint.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 15:00:38.000000 colcon-lint-0.2.0/colcon_lint.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-06-01 15:00:38.000000 colcon-lint-0.2.0/colcon_lint.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-06-01 15:00:38.000000 colcon-lint-0.2.0/colcon_lint.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-01 15:00:38.000000 colcon-lint-0.2.0/colcon_lint.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      773 2023-06-01 15:00:38.446222 colcon-lint-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      620 2023-06-01 15:00:15.000000 colcon-lint-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 15:00:38.446222 colcon-lint-0.2.0/test/
--rw-r--r--   0 root         (0) root         (0)     1577 2023-06-01 15:00:15.000000 colcon-lint-0.2.0/test/test_cmake.py
--rw-r--r--   0 root         (0) root         (0)     1070 2023-06-01 15:00:15.000000 colcon-lint-0.2.0/test/test_import.py
--rw-r--r--   0 root         (0) root         (0)     2093 2023-06-01 15:00:15.000000 colcon-lint-0.2.0/test/test_launch.py
--rw-r--r--   0 root         (0) root         (0)      902 2023-06-01 15:00:15.000000 colcon-lint-0.2.0/test/test_setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 04:37:50.683274 colcon-lint-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-01 04:37:43.000000 colcon-lint-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-07-01 04:37:50.683274 colcon-lint-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-07-01 04:37:43.000000 colcon-lint-0.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 04:37:50.683274 colcon-lint-0.2.1/colcon_lint/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-07-01 04:37:43.000000 colcon-lint-0.2.1/colcon_lint/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 04:37:50.683274 colcon-lint-0.2.1/colcon_lint/verb/
+-rw-r--r--   0 root         (0) root         (0)      581 2023-07-01 04:37:43.000000 colcon-lint-0.2.1/colcon_lint/verb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15415 2023-07-01 04:37:43.000000 colcon-lint-0.2.1/colcon_lint/verb/lint_depends.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 04:37:50.683274 colcon-lint-0.2.1/colcon_lint.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-07-01 04:37:50.000000 colcon-lint-0.2.1/colcon_lint.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      412 2023-07-01 04:37:50.000000 colcon-lint-0.2.1/colcon_lint.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-01 04:37:50.000000 colcon-lint-0.2.1/colcon_lint.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-01 04:37:50.000000 colcon-lint-0.2.1/colcon_lint.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-07-01 04:37:50.000000 colcon-lint-0.2.1/colcon_lint.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-01 04:37:50.000000 colcon-lint-0.2.1/colcon_lint.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      773 2023-07-01 04:37:50.683274 colcon-lint-0.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      620 2023-07-01 04:37:43.000000 colcon-lint-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 04:37:50.683274 colcon-lint-0.2.1/test/
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-07-01 04:37:43.000000 colcon-lint-0.2.1/test/test_cmake.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-07-01 04:37:43.000000 colcon-lint-0.2.1/test/test_import.py
+-rw-r--r--   0 root         (0) root         (0)     2093 2023-07-01 04:37:43.000000 colcon-lint-0.2.1/test/test_launch.py
+-rw-r--r--   0 root         (0) root         (0)      902 2023-07-01 04:37:43.000000 colcon-lint-0.2.1/test/test_setup.py
```

### Comparing `colcon-lint-0.2.0/LICENSE` & `colcon-lint-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `colcon-lint-0.2.0/PKG-INFO` & `colcon-lint-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colcon-lint
-Version: 0.2.0
+Version: 0.2.1
 Summary: Colcon extension for linting ROS package dependencies
 Home-page: UNKNOWN
 Author: Tatsuro Sakaguchi
 Author-email: tacchan.mello.ioiq@gmail.com
 Maintainer: Tatsuro Sakaguchi
 Maintainer-email: tacchan.mello.ioiq@gmail.com
 License: Apache License, Version 2.0
```

### Comparing `colcon-lint-0.2.0/README.md` & `colcon-lint-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `colcon-lint-0.2.0/colcon_lint/__init__.py` & `colcon-lint-0.2.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,8 +8,10 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = '0.2.0'
+from setuptools import setup
+
+setup()
```

### Comparing `colcon-lint-0.2.0/colcon_lint/verb/__init__.py` & `colcon-lint-0.2.1/colcon_lint/verb/__init__.py`

 * *Files identical despite different names*

### Comparing `colcon-lint-0.2.0/colcon_lint/verb/lint_depends.py` & `colcon-lint-0.2.1/colcon_lint/verb/lint_depends.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,31 +69,40 @@
             pkg = decorator.descriptor
             pkg_path = pathlib.Path(FindPackageShare(pkg.name).find(pkg.name)) / 'launch'
             launch_depends = set()
             for file in pkg_path.glob('**/*.py'):
                 launch_depends |= self.resolve_launch_depends(file)
 
             pkg_lib_path = pathlib.Path(FindPackagePrefix(pkg.name).find(pkg.name)) / 'lib'
-            egg_link = list(pkg_lib_path.glob('**/site-packages/*egg-link'))
+            site_packages_path = list(pkg_lib_path.glob('**/site-packages'))
             import_depends = set()
             setup_py_depends = set()
             build_depends = set()
             build_export_depends = set()
             buildtool_depends = set()
             test_depends = set()
             pkg_build_path = pkg_path.parents[4] / 'build' / pkg.name
-            if egg_link:
-                with open(egg_link[0]) as f:
-                    python_sources = pathlib.Path(f.read().split('\n')[0]) / pkg.name
-                for file in python_sources.glob('**/*.py'):
-                    import_depends |= self.resolve_import_depends(file)
+            if site_packages_path:
+                egg_link = list(site_packages_path[0].glob('*egg-link'))
+                if egg_link:
+                    with open(egg_link[0]) as f:
+                        python_sources = pathlib.Path(f.read().split('\n')[0]) / pkg.name
+                    for file in python_sources.glob('**/*.py'):
+                        import_depends |= self.resolve_import_depends(file)
 
-                setup_py = python_sources.parent / 'setup.py'
-                if setup_py.exists():
-                    setup_py_depends = self.resolve_setup_py_depends(setup_py)
+                    setup_py = python_sources.parent / 'setup.py'
+                    if setup_py.exists():
+                        setup_py_depends = self.resolve_setup_py_depends(setup_py)
+                else:
+                    for file in site_packages_path[0].glob('**/*.py'):
+                        import_depends |= self.resolve_import_depends(file)
+
+                    setup_py = pkg_build_path / 'setup.py'
+                    if setup_py.exists():
+                        setup_py_depends = self.resolve_setup_py_depends(setup_py)
             elif (pkg_build_path / 'Makefile').exists():
                 trace_file = pkg_build_path / 'trace.log'
                 if trace_file.exists():
                     with open(trace_file) as f:
                         trace_log = f.readlines()
                 else:
                     with open(pkg_build_path / 'Makefile') as f:
```

### Comparing `colcon-lint-0.2.0/colcon_lint.egg-info/PKG-INFO` & `colcon-lint-0.2.1/colcon_lint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colcon-lint
-Version: 0.2.0
+Version: 0.2.1
 Summary: Colcon extension for linting ROS package dependencies
 Home-page: UNKNOWN
 Author: Tatsuro Sakaguchi
 Author-email: tacchan.mello.ioiq@gmail.com
 Maintainer: Tatsuro Sakaguchi
 Maintainer-email: tacchan.mello.ioiq@gmail.com
 License: Apache License, Version 2.0
```

### Comparing `colcon-lint-0.2.0/setup.cfg` & `colcon-lint-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `colcon-lint-0.2.0/setup.py` & `colcon-lint-0.2.1/colcon_lint/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,10 +8,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-from setuptools import setup
-
-setup()
+__version__ = '0.2.1'
```

### Comparing `colcon-lint-0.2.0/test/test_cmake.py` & `colcon-lint-0.2.1/test/test_cmake.py`

 * *Files identical despite different names*

### Comparing `colcon-lint-0.2.0/test/test_import.py` & `colcon-lint-0.2.1/test/test_import.py`

 * *Files identical despite different names*

### Comparing `colcon-lint-0.2.0/test/test_launch.py` & `colcon-lint-0.2.1/test/test_launch.py`

 * *Files identical despite different names*

### Comparing `colcon-lint-0.2.0/test/test_setup.py` & `colcon-lint-0.2.1/test/test_setup.py`

 * *Files identical despite different names*

