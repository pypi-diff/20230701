# Comparing `tmp/raspi_gpio-0.1.2.tar.gz` & `tmp/raspi_gpio-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspi_gpio-0.1.2.tar", max compression
+gzip compressed data, was "raspi_gpio-0.1.3.tar", max compression
```

## Comparing `raspi_gpio-0.1.2.tar` & `raspi_gpio-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2023-06-30 22:00:13.107397 raspi_gpio-0.1.2/LICENSE
--rw-r--r--   0        0        0      270 2023-06-30 22:00:13.107397 raspi_gpio-0.1.2/README.md
--rw-r--r--   0        0        0      741 2023-06-30 22:00:33.523945 raspi_gpio-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1110 2023-06-30 22:00:13.107397 raspi_gpio-0.1.2/raspi_gpio/GPIO.py
--rw-r--r--   0        0        0      240 2023-06-30 22:00:13.107397 raspi_gpio-0.1.2/raspi_gpio/__init__.py
--rw-r--r--   0        0        0      703 2023-06-30 22:00:13.107397 raspi_gpio-0.1.2/raspi_gpio/spidev.py
--rw-r--r--   0        0        0     1121 1970-01-01 00:00:00.000000 raspi_gpio-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-01 01:51:06.677988 raspi_gpio-0.1.3/LICENSE
+-rw-r--r--   0        0        0      270 2023-07-01 01:51:06.677988 raspi_gpio-0.1.3/README.md
+-rw-r--r--   0        0        0      741 2023-07-01 01:51:25.534106 raspi_gpio-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1110 2023-07-01 01:51:06.677988 raspi_gpio-0.1.3/raspi_gpio/GPIO.py
+-rw-r--r--   0        0        0      240 2023-07-01 01:51:06.677988 raspi_gpio-0.1.3/raspi_gpio/__init__.py
+-rw-r--r--   0        0        0      715 2023-07-01 01:51:06.677988 raspi_gpio-0.1.3/raspi_gpio/spidev.py
+-rw-r--r--   0        0        0     1121 1970-01-01 00:00:00.000000 raspi_gpio-0.1.3/PKG-INFO
```

### Comparing `raspi_gpio-0.1.2/LICENSE` & `raspi_gpio-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `raspi_gpio-0.1.2/raspi_gpio/GPIO.py` & `raspi_gpio-0.1.3/raspi_gpio/GPIO.py`

 * *Files identical despite different names*

### Comparing `raspi_gpio-0.1.2/raspi_gpio/spidev.py` & `raspi_gpio-0.1.3/raspi_gpio/spidev.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,11 +30,11 @@
     def writebytes2(self,values):
         pass
 
     def xfer(self, values, speed=4096, delay=0, bits=8):
         pass
 
     def xfer2(self, values, speed=4096, delay=0, bits=8):
-        pass
+        return [0] * 255
 
     def xfer3(self, values, speed=4096, delay=0, bits=8):
         pass
```

### Comparing `raspi_gpio-0.1.2/PKG-INFO` & `raspi_gpio-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspi-gpio
-Version: 0.1.2
+Version: 0.1.3
 Summary: RPi.GPIO wrapper with mocks for developmennt on any platform
 Home-page: https://pypi.org/project/raspi-gpio/
 License: MIT
 Keywords: raspberry-pi,gpio,rpi,rpi-gpio,RPi.GPIO
 Author: Mark Parker
 Author-email: mark@parker-programs.com
 Requires-Python: >=3.10,<4.0
```

