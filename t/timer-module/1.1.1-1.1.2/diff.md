# Comparing `tmp/timer-module-1.1.1.tar.gz` & `tmp/timer-module-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timer-module-1.1.1.tar", last modified: Sat Jul  1 11:18:57 2023, max compression
+gzip compressed data, was "timer-module-1.1.2.tar", last modified: Sat Jul  1 15:23:35 2023, max compression
```

## Comparing `timer-module-1.1.1.tar` & `timer-module-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 11:18:57.905384 timer-module-1.1.1/
--rw-rw-rw-   0        0        0     1091 2023-02-11 02:09:32.000000 timer-module-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     2428 2023-07-01 11:18:57.904380 timer-module-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1859 2023-05-20 04:26:53.000000 timer-module-1.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-01 11:18:57.905384 timer-module-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      902 2023-07-01 11:18:09.000000 timer-module-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 11:18:57.882837 timer-module-1.1.1/timer_module/
--rw-rw-rw-   0        0        0      127 2023-05-20 04:38:26.000000 timer-module-1.1.1/timer_module/__init__.py
--rw-rw-rw-   0        0        0     5838 2023-07-01 10:58:41.000000 timer-module-1.1.1/timer_module/metrics.py
--rw-rw-rw-   0        0        0     7178 2023-07-01 10:42:41.000000 timer-module-1.1.1/timer_module/profiler.py
--rw-rw-rw-   0        0        0     1358 2023-06-29 22:39:56.000000 timer-module-1.1.1/timer_module/terminal.py
--rw-rw-rw-   0        0        0     1459 2023-05-20 04:38:26.000000 timer-module-1.1.1/timer_module/timer.py
-drwxrwxrwx   0        0        0        0 2023-07-01 11:18:57.903378 timer-module-1.1.1/timer_module.egg-info/
--rw-rw-rw-   0        0        0     2428 2023-07-01 11:18:57.000000 timer-module-1.1.1/timer_module.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-07-01 11:18:57.000000 timer-module-1.1.1/timer_module.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 11:18:57.000000 timer-module-1.1.1/timer_module.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-01 11:18:57.000000 timer-module-1.1.1/timer_module.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-01 11:18:57.000000 timer-module-1.1.1/timer_module.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 15:23:35.509932 timer-module-1.1.2/
+-rw-rw-rw-   0        0        0     1091 2023-02-11 02:09:32.000000 timer-module-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2428 2023-07-01 15:23:35.508931 timer-module-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1859 2023-05-20 04:26:53.000000 timer-module-1.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-01 15:23:35.509932 timer-module-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      902 2023-07-01 15:20:34.000000 timer-module-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 15:23:35.501899 timer-module-1.1.2/timer_module/
+-rw-rw-rw-   0        0        0      127 2023-05-20 04:38:26.000000 timer-module-1.1.2/timer_module/__init__.py
+-rw-rw-rw-   0        0        0     6004 2023-07-01 15:20:18.000000 timer-module-1.1.2/timer_module/metrics.py
+-rw-rw-rw-   0        0        0     7178 2023-07-01 10:42:41.000000 timer-module-1.1.2/timer_module/profiler.py
+-rw-rw-rw-   0        0        0     1358 2023-06-29 22:39:56.000000 timer-module-1.1.2/timer_module/terminal.py
+-rw-rw-rw-   0        0        0     1459 2023-05-20 04:38:26.000000 timer-module-1.1.2/timer_module/timer.py
+drwxrwxrwx   0        0        0        0 2023-07-01 15:23:35.507925 timer-module-1.1.2/timer_module.egg-info/
+-rw-rw-rw-   0        0        0     2428 2023-07-01 15:23:35.000000 timer-module-1.1.2/timer_module.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-07-01 15:23:35.000000 timer-module-1.1.2/timer_module.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 15:23:35.000000 timer-module-1.1.2/timer_module.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-01 15:23:35.000000 timer-module-1.1.2/timer_module.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-01 15:23:35.000000 timer-module-1.1.2/timer_module.egg-info/top_level.txt
```

### Comparing `timer-module-1.1.1/LICENSE` & `timer-module-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `timer-module-1.1.1/PKG-INFO` & `timer-module-1.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timer-module
-Version: 1.1.1
+Version: 1.1.2
 Summary: Timer Module with performance profiling features
 Home-page: https://github.com/syn-chromatic/timer-module
 Author: syn-chromatic
 Author-email: synchromatic.github@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `timer-module-1.1.1/README.md` & `timer-module-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `timer-module-1.1.1/setup.py` & `timer-module-1.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 from setuptools import setup, find_packages
 
-VERSION = "1.1.1"
+VERSION = "1.1.2"
 DESCRIPTION = "Timer Module with performance profiling features"
 
 root = Path(__file__).parent
 long_description = (root / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="timer-module",
```

### Comparing `timer-module-1.1.1/timer_module/metrics.py` & `timer-module-1.1.2/timer_module/metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,26 +69,31 @@
 
 class ProfileMetricsReport:
     def __init__(self, realtime: bool = False):
         self.realtime = realtime
         self.terminal = Terminal()
         self.header_color = self.get_header_color()
         self.call_color = self.get_call_color()
-        self.total_color = CyanANSI()
+        self.total_time_color = self.get_total_time_color()
 
     def get_header_color(self) -> ANSICode:
         if self.realtime:
             return YellowANSI()
         return GreenANSI()
 
     def get_call_color(self) -> ANSICode:
         if self.realtime:
             return CyanANSI()
         return WhiteANSI()
 
+    def get_total_time_color(self) -> ANSICode:
+        if self.realtime:
+            return YellowANSI()
+        return GreenANSI()
+
     def get_relative_percentage(self, pcall_ns: float, call_ns: float) -> float:
         percentage = 0.0
         if pcall_ns > 0.0 and call_ns > 0.0:
             percentage = (call_ns / pcall_ns) * 100
         return percentage
 
     def write_primary_call_header(self, call_metrics: CallableMetrics):
@@ -155,9 +160,9 @@
             self.write_primary_call_report(pcall_metrics)
 
         total_time_ns = self.get_total_time(callable_refs, timing_refs)
         total_time = TimeFormatterNs(total_time_ns).auto_format()
 
         string = "――― Total Time: [{}] ―――\n\n\n"
         string = string.format(f"{total_time}")
-        self.terminal.set_ansi_color(self.total_color)
+        self.terminal.set_ansi_color(self.total_time_color)
         self.terminal.write(string)
```

### Comparing `timer-module-1.1.1/timer_module/profiler.py` & `timer-module-1.1.2/timer_module/profiler.py`

 * *Files identical despite different names*

### Comparing `timer-module-1.1.1/timer_module/terminal.py` & `timer-module-1.1.2/timer_module/terminal.py`

 * *Files identical despite different names*

### Comparing `timer-module-1.1.1/timer_module/timer.py` & `timer-module-1.1.2/timer_module/timer.py`

 * *Files identical despite different names*

### Comparing `timer-module-1.1.1/timer_module.egg-info/PKG-INFO` & `timer-module-1.1.2/timer_module.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timer-module
-Version: 1.1.1
+Version: 1.1.2
 Summary: Timer Module with performance profiling features
 Home-page: https://github.com/syn-chromatic/timer-module
 Author: syn-chromatic
 Author-email: synchromatic.github@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

