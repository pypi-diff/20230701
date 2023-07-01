# Comparing `tmp/timer-module-1.1.0.tar.gz` & `tmp/timer-module-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timer-module-1.1.0.tar", last modified: Sat May 20 04:32:06 2023, max compression
+gzip compressed data, was "timer-module-1.1.1.tar", last modified: Sat Jul  1 11:18:57 2023, max compression
```

## Comparing `timer-module-1.1.0.tar` & `timer-module-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 04:32:06.229749 timer-module-1.1.0/
--rw-rw-rw-   0        0        0     1091 2023-02-11 02:09:32.000000 timer-module-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     2428 2023-05-20 04:32:06.228748 timer-module-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1859 2023-05-20 04:26:53.000000 timer-module-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-20 04:32:06.229749 timer-module-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      922 2023-05-20 04:31:19.000000 timer-module-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-20 04:32:06.202187 timer-module-1.1.0/timer_module/
--rw-rw-rw-   0        0        0      127 2023-05-20 02:26:45.000000 timer-module-1.1.0/timer_module/__init__.py
--rw-rw-rw-   0        0        0      494 2023-05-20 04:26:53.000000 timer-module-1.1.0/timer_module/converters.py
--rw-rw-rw-   0        0        0    10558 2023-05-20 04:26:53.000000 timer-module-1.1.0/timer_module/profiler.py
--rw-rw-rw-   0        0        0     1356 2023-05-20 04:26:53.000000 timer-module-1.1.0/timer_module/stdio.py
--rw-rw-rw-   0        0        0     1459 2023-02-11 01:27:34.000000 timer-module-1.1.0/timer_module/timer.py
-drwxrwxrwx   0        0        0        0 2023-05-20 04:32:06.227747 timer-module-1.1.0/timer_module.egg-info/
--rw-rw-rw-   0        0        0     2428 2023-05-20 04:32:06.000000 timer-module-1.1.0/timer_module.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-05-20 04:32:06.000000 timer-module-1.1.0/timer_module.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 04:32:06.000000 timer-module-1.1.0/timer_module.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-20 04:32:06.000000 timer-module-1.1.0/timer_module.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-20 04:32:06.000000 timer-module-1.1.0/timer_module.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 11:18:57.905384 timer-module-1.1.1/
+-rw-rw-rw-   0        0        0     1091 2023-02-11 02:09:32.000000 timer-module-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2428 2023-07-01 11:18:57.904380 timer-module-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1859 2023-05-20 04:26:53.000000 timer-module-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-01 11:18:57.905384 timer-module-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      902 2023-07-01 11:18:09.000000 timer-module-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 11:18:57.882837 timer-module-1.1.1/timer_module/
+-rw-rw-rw-   0        0        0      127 2023-05-20 04:38:26.000000 timer-module-1.1.1/timer_module/__init__.py
+-rw-rw-rw-   0        0        0     5838 2023-07-01 10:58:41.000000 timer-module-1.1.1/timer_module/metrics.py
+-rw-rw-rw-   0        0        0     7178 2023-07-01 10:42:41.000000 timer-module-1.1.1/timer_module/profiler.py
+-rw-rw-rw-   0        0        0     1358 2023-06-29 22:39:56.000000 timer-module-1.1.1/timer_module/terminal.py
+-rw-rw-rw-   0        0        0     1459 2023-05-20 04:38:26.000000 timer-module-1.1.1/timer_module/timer.py
+drwxrwxrwx   0        0        0        0 2023-07-01 11:18:57.903378 timer-module-1.1.1/timer_module.egg-info/
+-rw-rw-rw-   0        0        0     2428 2023-07-01 11:18:57.000000 timer-module-1.1.1/timer_module.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-07-01 11:18:57.000000 timer-module-1.1.1/timer_module.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 11:18:57.000000 timer-module-1.1.1/timer_module.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-01 11:18:57.000000 timer-module-1.1.1/timer_module.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-01 11:18:57.000000 timer-module-1.1.1/timer_module.egg-info/top_level.txt
```

### Comparing `timer-module-1.1.0/LICENSE` & `timer-module-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `timer-module-1.1.0/PKG-INFO` & `timer-module-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timer-module
-Version: 1.1.0
+Version: 1.1.1
 Summary: Timer Module with performance profiling features
 Home-page: https://github.com/syn-chromatic/timer-module
 Author: syn-chromatic
 Author-email: synchromatic.github@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `timer-module-1.1.0/README.md` & `timer-module-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `timer-module-1.1.0/setup.py` & `timer-module-1.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from pathlib import Path
 from setuptools import setup, find_packages
 
-VERSION = "1.1.0"
+VERSION = "1.1.1"
 DESCRIPTION = "Timer Module with performance profiling features"
 
 root = Path(__file__).parent
 long_description = (root / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="timer-module",
     author="syn-chromatic",
     author_email="synchromatic.github@gmail.com",
     url="https://github.com/syn-chromatic/timer-module",
     version=VERSION,
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
-    packages=find_packages(exclude=["examples"]),
+    packages=find_packages(),
     python_requires=">=3.10",
     install_requires=["setuptools>=45.0"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.10",
         "Topic :: Utilities",
```

### Comparing `timer-module-1.1.0/timer_module/stdio.py` & `timer-module-1.1.1/timer_module/terminal.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,20 +42,20 @@
 
 
 class WhiteANSI(ANSICode):
     def __init__(self):
         self.value: str = "\033[37m"
 
 
-class Stdio:
+class Terminal:
     def __init__(self, ansi_color: ANSICode = WhiteANSI()):
         self.ansi_color = ansi_color
         self.ansi_reset = ResetANSI()
 
-    def stdout(self, text: str):
+    def write(self, text: str):
         string = "{}{}{}"
         ansi_color_val = self.ansi_color.value
         ansi_reset_val = self.ansi_reset.value
         string = string.format(ansi_color_val, text, ansi_reset_val)
         print(string)
 
     def set_ansi_color(self, ansi_color: ANSICode):
```

### Comparing `timer-module-1.1.0/timer_module/timer.py` & `timer-module-1.1.1/timer_module/timer.py`

 * *Files identical despite different names*

### Comparing `timer-module-1.1.0/timer_module.egg-info/PKG-INFO` & `timer-module-1.1.1/timer_module.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timer-module
-Version: 1.1.0
+Version: 1.1.1
 Summary: Timer Module with performance profiling features
 Home-page: https://github.com/syn-chromatic/timer-module
 Author: syn-chromatic
 Author-email: synchromatic.github@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

