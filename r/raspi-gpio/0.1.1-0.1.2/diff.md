# Comparing `tmp/raspi_gpio-0.1.1.tar.gz` & `tmp/raspi_gpio-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspi_gpio-0.1.1.tar", max compression
+gzip compressed data, was "raspi_gpio-0.1.2.tar", max compression
```

## Comparing `raspi_gpio-0.1.1.tar` & `raspi_gpio-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2023-06-30 18:14:16.775162 raspi_gpio-0.1.1/LICENSE
--rw-r--r--   0        0        0       85 2023-06-30 18:14:16.775162 raspi_gpio-0.1.1/README.md
--rw-r--r--   0        0        0      741 2023-06-30 18:14:37.606896 raspi_gpio-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1110 2023-06-30 18:14:16.775162 raspi_gpio-0.1.1/raspi_gpio/GPIO.py
--rw-r--r--   0        0        0      233 2023-06-30 18:14:16.775162 raspi_gpio-0.1.1/raspi_gpio/__init__.py
--rw-r--r--   0        0        0      703 2023-06-30 18:14:16.775162 raspi_gpio-0.1.1/raspi_gpio/spidev.py
--rw-r--r--   0        0        0      936 1970-01-01 00:00:00.000000 raspi_gpio-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-30 22:00:13.107397 raspi_gpio-0.1.2/LICENSE
+-rw-r--r--   0        0        0      270 2023-06-30 22:00:13.107397 raspi_gpio-0.1.2/README.md
+-rw-r--r--   0        0        0      741 2023-06-30 22:00:33.523945 raspi_gpio-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1110 2023-06-30 22:00:13.107397 raspi_gpio-0.1.2/raspi_gpio/GPIO.py
+-rw-r--r--   0        0        0      240 2023-06-30 22:00:13.107397 raspi_gpio-0.1.2/raspi_gpio/__init__.py
+-rw-r--r--   0        0        0      703 2023-06-30 22:00:13.107397 raspi_gpio-0.1.2/raspi_gpio/spidev.py
+-rw-r--r--   0        0        0     1121 1970-01-01 00:00:00.000000 raspi_gpio-0.1.2/PKG-INFO
```

### Comparing `raspi_gpio-0.1.1/LICENSE` & `raspi_gpio-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `raspi_gpio-0.1.1/pyproject.toml` & `raspi_gpio-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "raspi-gpio"
-version = "0.1.1"
+version = "0.1.2"
 description = "RPi.GPIO wrapper with mocks for developmennt on any platform"
 authors = ["Mark Parker <mark@parker-programs.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "raspi_gpio"}]
 homepage = "https://pypi.org/project/raspi-gpio/"
 repository = "https://github.com/MarkParker5/raspi-gpio"
```

### Comparing `raspi_gpio-0.1.1/raspi_gpio/GPIO.py` & `raspi_gpio-0.1.2/raspi_gpio/GPIO.py`

 * *Files identical despite different names*

### Comparing `raspi_gpio-0.1.1/raspi_gpio/spidev.py` & `raspi_gpio-0.1.2/raspi_gpio/spidev.py`

 * *Files identical despite different names*

### Comparing `raspi_gpio-0.1.1/PKG-INFO` & `raspi_gpio-0.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspi-gpio
-Version: 0.1.1
+Version: 0.1.2
 Summary: RPi.GPIO wrapper with mocks for developmennt on any platform
 Home-page: https://pypi.org/project/raspi-gpio/
 License: MIT
 Keywords: raspberry-pi,gpio,rpi,rpi-gpio,RPi.GPIO
 Author: Mark Parker
 Author-email: mark@parker-programs.com
 Requires-Python: >=3.10,<4.0
@@ -17,7 +17,23 @@
 Project-URL: Documentation, https://github.com/MarkParker5/raspi-gpio/blob/main/README.md
 Project-URL: Repository, https://github.com/MarkParker5/raspi-gpio
 Description-Content-Type: text/markdown
 
 # raspi-gpio
 RPi.GPIO and spidev wrapper with mocks for developmennt on any platform
 
+# Installation
+```sh
+pip install raspi-gpio
+```
+
+# Usage
+Replace
+```python
+import RPi.GPIO as GPIO
+from spidev import SpiDev
+```
+with
+```python
+from raspi_gpio import GPIO, SpiDev
+```
+
```

