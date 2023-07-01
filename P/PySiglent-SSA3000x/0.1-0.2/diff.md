# Comparing `tmp/PySiglent_SSA3000x-0.1.tar.gz` & `tmp/PySiglent_SSA3000x-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySiglent_SSA3000x-0.1.tar", last modified: Sun Jun 25 20:22:58 2023, max compression
+gzip compressed data, was "PySiglent_SSA3000x-0.2.tar", last modified: Sat Jul  1 16:47:32 2023, max compression
```

## Comparing `PySiglent_SSA3000x-0.1.tar` & `PySiglent_SSA3000x-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 20:22:58.146383 PySiglent_SSA3000x-0.1/
--rw-rw-rw-   0        0        0     1091 2023-06-25 20:17:12.000000 PySiglent_SSA3000x-0.1/LICENSE
--rw-rw-rw-   0        0        0      413 2023-06-25 20:22:58.146383 PySiglent_SSA3000x-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-25 20:22:58.136775 PySiglent_SSA3000x-0.1/PySiglent_SSA3000x/
--rw-rw-rw-   0        0        0    26105 2023-06-25 20:19:04.000000 PySiglent_SSA3000x-0.1/PySiglent_SSA3000x/PySiglent_SSA3000x.py
--rw-rw-rw-   0        0        0       54 2023-06-25 20:17:12.000000 PySiglent_SSA3000x-0.1/PySiglent_SSA3000x/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 20:22:58.145383 PySiglent_SSA3000x-0.1/PySiglent_SSA3000x.egg-info/
--rw-rw-rw-   0        0        0      413 2023-06-25 20:22:58.000000 PySiglent_SSA3000x-0.1/PySiglent_SSA3000x.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-06-25 20:22:58.000000 PySiglent_SSA3000x-0.1/PySiglent_SSA3000x.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 20:22:58.000000 PySiglent_SSA3000x-0.1/PySiglent_SSA3000x.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-25 20:22:58.000000 PySiglent_SSA3000x-0.1/PySiglent_SSA3000x.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-25 20:22:58.000000 PySiglent_SSA3000x-0.1/PySiglent_SSA3000x.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-25 20:22:58.146383 PySiglent_SSA3000x-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1076 2023-06-25 20:19:33.000000 PySiglent_SSA3000x-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 16:47:31.986064 PySiglent_SSA3000x-0.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-25 20:17:12.000000 PySiglent_SSA3000x-0.2/LICENSE
+-rw-rw-rw-   0        0        0      413 2023-07-01 16:47:31.984063 PySiglent_SSA3000x-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-01 16:47:31.943064 PySiglent_SSA3000x-0.2/PySiglent_SSA3000x/
+-rw-rw-rw-   0        0        0    26168 2023-07-01 16:45:44.000000 PySiglent_SSA3000x-0.2/PySiglent_SSA3000x/PySiglent_SSA3000x.py
+-rw-rw-rw-   0        0        0       54 2023-06-25 20:17:12.000000 PySiglent_SSA3000x-0.2/PySiglent_SSA3000x/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 16:47:31.978065 PySiglent_SSA3000x-0.2/PySiglent_SSA3000x.egg-info/
+-rw-rw-rw-   0        0        0      413 2023-07-01 16:47:31.000000 PySiglent_SSA3000x-0.2/PySiglent_SSA3000x.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-07-01 16:47:31.000000 PySiglent_SSA3000x-0.2/PySiglent_SSA3000x.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 16:47:31.000000 PySiglent_SSA3000x-0.2/PySiglent_SSA3000x.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-01 16:47:31.000000 PySiglent_SSA3000x-0.2/PySiglent_SSA3000x.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-01 16:47:31.000000 PySiglent_SSA3000x-0.2/PySiglent_SSA3000x.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 16:47:31.987065 PySiglent_SSA3000x-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1076 2023-06-25 20:19:33.000000 PySiglent_SSA3000x-0.2/setup.py
```

### Comparing `PySiglent_SSA3000x-0.1/LICENSE` & `PySiglent_SSA3000x-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PySiglent_SSA3000x-0.1/PySiglent_SSA3000x/PySiglent_SSA3000x.py` & `PySiglent_SSA3000x-0.2/PySiglent_SSA3000x/PySiglent_SSA3000x.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+import pyvisa
+from numpy import linspace
 
 class PySiglent_SSA3000x:
-    import pyvisa
-    from numpy import linspace
 
     # exceptions
     class Exceptions:
         class NotConnected(Exception):
             def __init__(self) -> None:
                 super().__init__('instrument connection not implemented')
 
@@ -283,17 +283,19 @@
             return True
         return False
     
     # custom fuinctions ---------------
     
     def get_spectrum(self, trace:Trace):
         """used to gwet the spectrum data in a format like [ [freq_1, level_1], [freq_2, level_2], ...]"""
-        level_data:list = trace.get_data()
-        frequency_points = self.linspace(self.start_frequency, self.stop_frequency, len(level_data))
-        return zip(frequency_points, level_data)
+        level_points = trace.get_data()
+        start_freq = self.start_frequency()
+        stop_freq  = self.stop_frequency()
+        frequency_points = linspace(start_freq, stop_freq, len(level_points))
+        return list(zip(frequency_points, level_points))
 
     # function from manual ------------
 
     def center_freqency(self, frequency: int = None):
         """Sets the center frequency of the spectrum analyzer. [Hz]
         Gets the center frequency."""
         if frequency is not None and not self.frequency_min <= frequency <= self.frequency_max:
```

### Comparing `PySiglent_SSA3000x-0.1/setup.py` & `PySiglent_SSA3000x-0.2/setup.py`

 * *Files identical despite different names*

