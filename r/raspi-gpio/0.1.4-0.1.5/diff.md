# Comparing `tmp/raspi_gpio-0.1.4.tar.gz` & `tmp/raspi_gpio-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspi_gpio-0.1.4.tar", max compression
+gzip compressed data, was "raspi_gpio-0.1.5.tar", max compression
```

## Comparing `raspi_gpio-0.1.4.tar` & `raspi_gpio-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2023-07-01 01:57:44.646492 raspi_gpio-0.1.4/LICENSE
--rw-r--r--   0        0        0      270 2023-07-01 01:57:44.646492 raspi_gpio-0.1.4/README.md
--rw-r--r--   0        0        0      741 2023-07-01 01:58:03.494485 raspi_gpio-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1127 2023-07-01 01:57:44.646492 raspi_gpio-0.1.4/raspi_gpio/GPIO.py
--rw-r--r--   0        0        0      240 2023-07-01 01:57:44.646492 raspi_gpio-0.1.4/raspi_gpio/__init__.py
--rw-r--r--   0        0        0      715 2023-07-01 01:57:44.646492 raspi_gpio-0.1.4/raspi_gpio/spidev.py
--rw-r--r--   0        0        0     1121 1970-01-01 00:00:00.000000 raspi_gpio-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-01 02:15:24.817355 raspi_gpio-0.1.5/LICENSE
+-rw-r--r--   0        0        0      270 2023-07-01 02:15:24.817355 raspi_gpio-0.1.5/README.md
+-rw-r--r--   0        0        0      741 2023-07-01 02:15:49.250790 raspi_gpio-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1174 2023-07-01 02:15:24.817355 raspi_gpio-0.1.5/raspi_gpio/GPIO.py
+-rw-r--r--   0        0        0      240 2023-07-01 02:15:24.817355 raspi_gpio-0.1.5/raspi_gpio/__init__.py
+-rw-r--r--   0        0        0      715 2023-07-01 02:15:24.817355 raspi_gpio-0.1.5/raspi_gpio/spidev.py
+-rw-r--r--   0        0        0     1121 1970-01-01 00:00:00.000000 raspi_gpio-0.1.5/PKG-INFO
```

### Comparing `raspi_gpio-0.1.4/LICENSE` & `raspi_gpio-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `raspi_gpio-0.1.4/pyproject.toml` & `raspi_gpio-0.1.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "raspi-gpio"
-version = "0.1.4"
+version = "0.1.5"
 description = "RPi.GPIO wrapper with mocks for developmennt on any platform"
 authors = ["Mark Parker <mark@parker-programs.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "raspi_gpio"}]
 homepage = "https://pypi.org/project/raspi-gpio/"
 repository = "https://github.com/MarkParker5/raspi-gpio"
```

### Comparing `raspi_gpio-0.1.4/raspi_gpio/GPIO.py` & `raspi_gpio-0.1.5/raspi_gpio/GPIO.py`

 * *Files 10% similar despite different names*

```diff
@@ -71,7 +71,10 @@
     pass
 
 def gpio_function(channel):
     return OUT
 
 def setwarnings(state):
     pass
+
+def pulseOut(ce_pin, value, period):
+    pass
```

### Comparing `raspi_gpio-0.1.4/raspi_gpio/spidev.py` & `raspi_gpio-0.1.5/raspi_gpio/spidev.py`

 * *Files identical despite different names*

### Comparing `raspi_gpio-0.1.4/PKG-INFO` & `raspi_gpio-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspi-gpio
-Version: 0.1.4
+Version: 0.1.5
 Summary: RPi.GPIO wrapper with mocks for developmennt on any platform
 Home-page: https://pypi.org/project/raspi-gpio/
 License: MIT
 Keywords: raspberry-pi,gpio,rpi,rpi-gpio,RPi.GPIO
 Author: Mark Parker
 Author-email: mark@parker-programs.com
 Requires-Python: >=3.10,<4.0
```

