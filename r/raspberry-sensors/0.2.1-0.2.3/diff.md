# Comparing `tmp/raspberry-sensors-0.2.1.tar.gz` & `tmp/raspberry-sensors-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspberry-sensors-0.2.1.tar", last modified: Wed Jun 28 11:19:28 2023, max compression
+gzip compressed data, was "raspberry-sensors-0.2.3.tar", last modified: Sat Jul  1 18:16:37 2023, max compression
```

## Comparing `raspberry-sensors-0.2.1.tar` & `raspberry-sensors-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 pip       (1000) pip       (1000)        0 2023-06-28 11:19:28.927540 raspberry-sensors-0.2.1/
--rwxrwxrwx   0 pip       (1000) pip       (1000)     1091 2023-06-28 10:47:28.000000 raspberry-sensors-0.2.1/LICENSE
--rw-r--r--   0 pip       (1000) pip       (1000)      500 2023-06-28 11:19:28.927540 raspberry-sensors-0.2.1/PKG-INFO
--rwxrwxrwx   0 pip       (1000) pip       (1000)       90 2023-06-28 10:56:28.000000 raspberry-sensors-0.2.1/README.md
--rwxrwxrwx   0 pip       (1000) pip       (1000)      583 2023-06-28 10:56:18.000000 raspberry-sensors-0.2.1/pyproject.toml
--rw-r--r--   0 pip       (1000) pip       (1000)       38 2023-06-28 11:19:28.927540 raspberry-sensors-0.2.1/setup.cfg
-drwxr-xr-x   0 pip       (1000) pip       (1000)        0 2023-06-28 11:19:28.903541 raspberry-sensors-0.2.1/src/
-drwxr-xr-x   0 pip       (1000) pip       (1000)        0 2023-06-28 11:19:28.915541 raspberry-sensors-0.2.1/src/raspberry-sensors/
--rwxrwxrwx   0 pip       (1000) pip       (1000)        0 2023-06-28 10:37:28.000000 raspberry-sensors-0.2.1/src/raspberry-sensors/__init__.py
--rwxrwxrwx   0 pip       (1000) pip       (1000)     3315 2023-06-28 10:26:16.000000 raspberry-sensors-0.2.1/src/raspberry-sensors/sensors.py
-drwxr-xr-x   0 pip       (1000) pip       (1000)        0 2023-06-28 11:19:28.923540 raspberry-sensors-0.2.1/src/raspberry_sensors.egg-info/
--rw-r--r--   0 pip       (1000) pip       (1000)      500 2023-06-28 11:19:28.000000 raspberry-sensors-0.2.1/src/raspberry_sensors.egg-info/PKG-INFO
--rw-r--r--   0 pip       (1000) pip       (1000)      321 2023-06-28 11:19:28.000000 raspberry-sensors-0.2.1/src/raspberry_sensors.egg-info/SOURCES.txt
--rw-r--r--   0 pip       (1000) pip       (1000)        1 2023-06-28 11:19:28.000000 raspberry-sensors-0.2.1/src/raspberry_sensors.egg-info/dependency_links.txt
--rw-r--r--   0 pip       (1000) pip       (1000)       45 2023-06-28 11:19:28.000000 raspberry-sensors-0.2.1/src/raspberry_sensors.egg-info/top_level.txt
-drwxr-xr-x   0 pip       (1000) pip       (1000)        0 2023-06-28 11:19:28.923540 raspberry-sensors-0.2.1/src/raspberry_sensors_Develper/
--rwxrwxrwx   0 pip       (1000) pip       (1000)     3329 2023-06-28 10:53:18.000000 raspberry-sensors-0.2.1/src/raspberry_sensors_Develper/sensors.py
+drwxrwxrwx   0        0        0        0 2023-07-01 18:16:37.871609 raspberry-sensors-0.2.3/
+-rw-rw-rw-   0        0        0     1091 2023-06-28 10:47:29.000000 raspberry-sensors-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     1763 2023-07-01 18:16:37.871609 raspberry-sensors-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1338 2023-07-01 16:02:47.000000 raspberry-sensors-0.2.3/README.md
+-rw-rw-rw-   0        0        0      501 2023-07-01 18:16:23.000000 raspberry-sensors-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-01 18:16:37.871609 raspberry-sensors-0.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-01 18:16:37.840273 raspberry-sensors-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-01 18:16:37.840273 raspberry-sensors-0.2.3/src/raspberry-sensors/
+-rw-rw-rw-   0        0        0        0 2023-06-28 10:37:28.000000 raspberry-sensors-0.2.3/src/raspberry-sensors/__init__.py
+-rw-rw-rw-   0        0        0     3315 2023-06-28 10:26:16.000000 raspberry-sensors-0.2.3/src/raspberry-sensors/sensors.py
+drwxrwxrwx   0        0        0        0 2023-07-01 18:16:37.855900 raspberry-sensors-0.2.3/src/raspberry_sensors.egg-info/
+-rw-rw-rw-   0        0        0     1763 2023-07-01 18:16:37.000000 raspberry-sensors-0.2.3/src/raspberry_sensors.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-07-01 18:16:37.000000 raspberry-sensors-0.2.3/src/raspberry_sensors.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 18:16:37.000000 raspberry-sensors-0.2.3/src/raspberry_sensors.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-01 18:16:37.000000 raspberry-sensors-0.2.3/src/raspberry_sensors.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 18:16:37.871609 raspberry-sensors-0.2.3/src/raspberry_sensors_Develper/
+-rw-rw-rw-   0        0        0     3340 2023-07-01 18:16:16.000000 raspberry-sensors-0.2.3/src/raspberry_sensors_Develper/sensors.py
```

### Comparing `raspberry-sensors-0.2.1/LICENSE` & `raspberry-sensors-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `raspberry-sensors-0.2.1/src/raspberry-sensors/sensors.py` & `raspberry-sensors-0.2.3/src/raspberry-sensors/sensors.py`

 * *Files identical despite different names*

### Comparing `raspberry-sensors-0.2.1/src/raspberry_sensors_Develper/sensors.py` & `raspberry-sensors-0.2.3/src/raspberry_sensors_Develper/sensors.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,21 +33,21 @@
                 analog_in.AnalogIn(self.ads, 3)
             ]
         except Exception as ex:
             ads = 1
             if self.loging_error:
                 print(f"ADS init error -> {ex}")
 
-    def get_dht(self, _type=22, pin=4):
+    def get_dht(self, _type=22, gpio=4):
         if dht:
             if self.loging_error:
                 print("DHT not available")
             return {"humidity": self.cache["humidity"], "temperature": self.cache["temperature"]}
         try:
-            h, t = read(DHT22 if _type==22 else DHT11, pin)
+            h, t = read(DHT22 if _type==22 else DHT11, gpio)
             if h and t:
                 self.cache["humidity"], self.cache["temperature"] = round(h, 2), round(t, 2)
             else:
                 if self.loging_error:
                     print(f"DHT error, used cache")
         except Exception as ex:
             if self.loging_error:
@@ -81,8 +81,8 @@
             if pwm:
                 self.cache["co2"] = read_from_pwm(gpio=gpio, range=_range)["co2"]
             else:
                 self.cache["co2"] = mhz_read()["co2"]
         except Exception as ex:
             if self.loging_error:
                 print(f"MHZ19 error ({ex}), used cache")
-        return self.cache["co2"]
+        return {"co2": self.cache["co2"]}
```

