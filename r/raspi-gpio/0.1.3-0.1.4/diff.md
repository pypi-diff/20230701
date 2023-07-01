# Comparing `tmp/raspi_gpio-0.1.3.tar.gz` & `tmp/raspi_gpio-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspi_gpio-0.1.3.tar", max compression
+gzip compressed data, was "raspi_gpio-0.1.4.tar", max compression
```

## Comparing `raspi_gpio-0.1.3.tar` & `raspi_gpio-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2023-07-01 01:51:06.677988 raspi_gpio-0.1.3/LICENSE
--rw-r--r--   0        0        0      270 2023-07-01 01:51:06.677988 raspi_gpio-0.1.3/README.md
--rw-r--r--   0        0        0      741 2023-07-01 01:51:25.534106 raspi_gpio-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1110 2023-07-01 01:51:06.677988 raspi_gpio-0.1.3/raspi_gpio/GPIO.py
--rw-r--r--   0        0        0      240 2023-07-01 01:51:06.677988 raspi_gpio-0.1.3/raspi_gpio/__init__.py
--rw-r--r--   0        0        0      715 2023-07-01 01:51:06.677988 raspi_gpio-0.1.3/raspi_gpio/spidev.py
--rw-r--r--   0        0        0     1121 1970-01-01 00:00:00.000000 raspi_gpio-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-01 01:57:44.646492 raspi_gpio-0.1.4/LICENSE
+-rw-r--r--   0        0        0      270 2023-07-01 01:57:44.646492 raspi_gpio-0.1.4/README.md
+-rw-r--r--   0        0        0      741 2023-07-01 01:58:03.494485 raspi_gpio-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1127 2023-07-01 01:57:44.646492 raspi_gpio-0.1.4/raspi_gpio/GPIO.py
+-rw-r--r--   0        0        0      240 2023-07-01 01:57:44.646492 raspi_gpio-0.1.4/raspi_gpio/__init__.py
+-rw-r--r--   0        0        0      715 2023-07-01 01:57:44.646492 raspi_gpio-0.1.4/raspi_gpio/spidev.py
+-rw-r--r--   0        0        0     1121 1970-01-01 00:00:00.000000 raspi_gpio-0.1.4/PKG-INFO
```

### Comparing `raspi_gpio-0.1.3/LICENSE` & `raspi_gpio-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `raspi_gpio-0.1.3/pyproject.toml` & `raspi_gpio-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "raspi-gpio"
-version = "0.1.3"
+version = "0.1.4"
 description = "RPi.GPIO wrapper with mocks for developmennt on any platform"
 authors = ["Mark Parker <mark@parker-programs.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "raspi_gpio"}]
 homepage = "https://pypi.org/project/raspi-gpio/"
 repository = "https://github.com/MarkParker5/raspi-gpio"
```

### Comparing `raspi_gpio-0.1.3/raspi_gpio/GPIO.py` & `raspi_gpio-0.1.4/raspi_gpio/GPIO.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 BCM = 11
 PUD_OFF = 0
 PUD_UP = 2
 PUD_DOWN = 1
 RISING = 0
 FALLING = 0
 BOTH = 0
+RPI_REVISION = 0
 
 class PWM(object):
 
     def __init__(self, channel, frequency):
         pass
 
     def start(self, dutycycle):
```

### Comparing `raspi_gpio-0.1.3/raspi_gpio/spidev.py` & `raspi_gpio-0.1.4/raspi_gpio/spidev.py`

 * *Files identical despite different names*

### Comparing `raspi_gpio-0.1.3/PKG-INFO` & `raspi_gpio-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspi-gpio
-Version: 0.1.3
+Version: 0.1.4
 Summary: RPi.GPIO wrapper with mocks for developmennt on any platform
 Home-page: https://pypi.org/project/raspi-gpio/
 License: MIT
 Keywords: raspberry-pi,gpio,rpi,rpi-gpio,RPi.GPIO
 Author: Mark Parker
 Author-email: mark@parker-programs.com
 Requires-Python: >=3.10,<4.0
```

