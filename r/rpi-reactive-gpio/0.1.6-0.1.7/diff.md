# Comparing `tmp/rpi_reactive_gpio-0.1.6.tar.gz` & `tmp/rpi_reactive_gpio-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpi_reactive_gpio-0.1.6.tar", max compression
+gzip compressed data, was "rpi_reactive_gpio-0.1.7.tar", max compression
```

## Comparing `rpi_reactive_gpio-0.1.6.tar` & `rpi_reactive_gpio-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1068 2023-06-30 17:51:17.829130 rpi_reactive_gpio-0.1.6/LICENSE
--rw-r--r--   0        0        0       80 2023-06-30 17:51:17.829130 rpi_reactive_gpio-0.1.6/README.md
--rw-r--r--   0        0        0      766 2023-06-30 17:51:48.325478 rpi_reactive_gpio-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      207 2023-06-30 17:51:17.829130 rpi_reactive_gpio-0.1.6/rpi_reactive_gpio/__init__.py
--rw-r--r--   0        0        0     1607 2023-06-30 17:51:17.829130 rpi_reactive_gpio-0.1.6/rpi_reactive_gpio/buttons.py
--rw-r--r--   0        0        0     3508 2023-06-30 17:51:17.829130 rpi_reactive_gpio-0.1.6/rpi_reactive_gpio/leds.py
--rw-r--r--   0        0        0      482 2023-06-30 17:51:17.829130 rpi_reactive_gpio-0.1.6/rpi_reactive_gpio/main.py
--rw-r--r--   0        0        0      850 2023-06-30 17:51:17.829130 rpi_reactive_gpio-0.1.6/rpi_reactive_gpio/pin_manager.py
--rw-r--r--   0        0        0     1263 2023-06-30 17:51:17.829130 rpi_reactive_gpio-0.1.6/rpi_reactive_gpio/scene.py
--rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 rpi_reactive_gpio-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-30 22:30:56.638390 rpi_reactive_gpio-0.1.7/LICENSE
+-rw-r--r--   0        0        0       80 2023-06-30 22:30:56.638390 rpi_reactive_gpio-0.1.7/README.md
+-rw-r--r--   0        0        0      766 2023-06-30 22:31:14.886377 rpi_reactive_gpio-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      207 2023-06-30 22:30:56.638390 rpi_reactive_gpio-0.1.7/rpi_reactive_gpio/__init__.py
+-rw-r--r--   0        0        0     1607 2023-06-30 22:30:56.638390 rpi_reactive_gpio-0.1.7/rpi_reactive_gpio/buttons.py
+-rw-r--r--   0        0        0     3534 2023-06-30 22:30:56.638390 rpi_reactive_gpio-0.1.7/rpi_reactive_gpio/leds.py
+-rw-r--r--   0        0        0      482 2023-06-30 22:30:56.638390 rpi_reactive_gpio-0.1.7/rpi_reactive_gpio/main.py
+-rw-r--r--   0        0        0      850 2023-06-30 22:30:56.638390 rpi_reactive_gpio-0.1.7/rpi_reactive_gpio/pin_manager.py
+-rw-r--r--   0        0        0     1263 2023-06-30 22:30:56.638390 rpi_reactive_gpio-0.1.7/rpi_reactive_gpio/scene.py
+-rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 rpi_reactive_gpio-0.1.7/PKG-INFO
```

### Comparing `rpi_reactive_gpio-0.1.6/LICENSE` & `rpi_reactive_gpio-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rpi_reactive_gpio-0.1.6/pyproject.toml` & `rpi_reactive_gpio-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rpi-reactive-gpio"
-version = "0.1.6"
+version = "0.1.7"
 description = "Syntax sugar for controlling RPi.GPIO with reactive design."
 authors = ["MarkParker5 <markparker.it@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rpi_reactive_gpio"}]
 homepage = "https://pypi.org/project/rpi-reactive-gpio/"
 repository = "https://github.com/MarkParker5/rpi-reactive-gpio"
```

### Comparing `rpi_reactive_gpio-0.1.6/rpi_reactive_gpio/buttons.py` & `rpi_reactive_gpio-0.1.7/rpi_reactive_gpio/buttons.py`

 * *Files identical despite different names*

### Comparing `rpi_reactive_gpio-0.1.6/rpi_reactive_gpio/leds.py` & `rpi_reactive_gpio-0.1.7/rpi_reactive_gpio/leds.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,16 +87,16 @@
                 GPIO.output(self.green_pin, GPIO.HIGH)
                 GPIO.output(self.blue_pin, GPIO.LOW)
             case RGBLedState.blue:
                 GPIO.output(self.red_pin, GPIO.LOW)
                 GPIO.output(self.green_pin, GPIO.LOW)
                 GPIO.output(self.blue_pin, GPIO.HIGH)
               
-    def update(self):
-        self._last_led_state = self._get_pin_state()      
+    def update(self, *args, **kwargs):
+        self._last_led_state = self._get_pin_state(*args, **kwargs)
           
     # decorator
     def __call__(self, get_pin_state: Callable[..., RGBLedState]) -> RGBLedManager:
         global managers
         self._get_pin_state = get_pin_state
         managers.append(self)
         return self
```

### Comparing `rpi_reactive_gpio-0.1.6/rpi_reactive_gpio/pin_manager.py` & `rpi_reactive_gpio-0.1.7/rpi_reactive_gpio/pin_manager.py`

 * *Files identical despite different names*

### Comparing `rpi_reactive_gpio-0.1.6/rpi_reactive_gpio/scene.py` & `rpi_reactive_gpio-0.1.7/rpi_reactive_gpio/scene.py`

 * *Files identical despite different names*

### Comparing `rpi_reactive_gpio-0.1.6/PKG-INFO` & `rpi_reactive_gpio-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpi-reactive-gpio
-Version: 0.1.6
+Version: 0.1.7
 Summary: Syntax sugar for controlling RPi.GPIO with reactive design.
 Home-page: https://pypi.org/project/rpi-reactive-gpio/
 License: MIT
 Keywords: raspberry-pi,gpio,reactive,rxpy,rx,rpi,rpi-gpio,RPi.GPIO
 Author: MarkParker5
 Author-email: markparker.it@gmail.com
 Requires-Python: >=3.10,<4.0
```

