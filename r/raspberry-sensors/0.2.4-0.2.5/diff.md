# Comparing `tmp/raspberry-sensors-0.2.4.tar.gz` & `tmp/raspberry-sensors-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspberry-sensors-0.2.4.tar", last modified: Sat Jul  1 18:29:49 2023, max compression
+gzip compressed data, was "raspberry-sensors-0.2.5.tar", last modified: Sat Jul  1 18:34:28 2023, max compression
```

## Comparing `raspberry-sensors-0.2.4.tar` & `raspberry-sensors-0.2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 18:29:49.645820 raspberry-sensors-0.2.4/
--rw-rw-rw-   0        0        0     1091 2023-06-28 10:47:29.000000 raspberry-sensors-0.2.4/LICENSE
--rw-rw-rw-   0        0        0     1763 2023-07-01 18:29:49.643828 raspberry-sensors-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1338 2023-07-01 16:02:47.000000 raspberry-sensors-0.2.4/README.md
--rw-rw-rw-   0        0        0      501 2023-07-01 18:27:54.000000 raspberry-sensors-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-01 18:29:49.645820 raspberry-sensors-0.2.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-01 18:29:49.611848 raspberry-sensors-0.2.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-01 18:29:49.621253 raspberry-sensors-0.2.4/src/raspberry-sensors/
--rw-rw-rw-   0        0        0        0 2023-06-28 10:37:28.000000 raspberry-sensors-0.2.4/src/raspberry-sensors/__init__.py
--rw-rw-rw-   0        0        0     3315 2023-06-28 10:26:16.000000 raspberry-sensors-0.2.4/src/raspberry-sensors/sensors.py
-drwxrwxrwx   0        0        0        0 2023-07-01 18:29:49.640835 raspberry-sensors-0.2.4/src/raspberry_sensors.egg-info/
--rw-rw-rw-   0        0        0     1763 2023-07-01 18:29:49.000000 raspberry-sensors-0.2.4/src/raspberry_sensors.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2023-07-01 18:29:49.000000 raspberry-sensors-0.2.4/src/raspberry_sensors.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 18:29:49.000000 raspberry-sensors-0.2.4/src/raspberry_sensors.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-01 18:29:49.000000 raspberry-sensors-0.2.4/src/raspberry_sensors.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-01 18:29:49.641832 raspberry-sensors-0.2.4/src/raspberry_sensors_Develper/
--rw-rw-rw-   0        0        0     3400 2023-07-01 18:27:02.000000 raspberry-sensors-0.2.4/src/raspberry_sensors_Develper/sensors.py
+drwxrwxrwx   0        0        0        0 2023-07-01 18:34:28.617002 raspberry-sensors-0.2.5/
+-rw-rw-rw-   0        0        0     1091 2023-06-28 10:47:29.000000 raspberry-sensors-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0     1787 2023-07-01 18:34:28.617002 raspberry-sensors-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1362 2023-07-01 18:34:08.000000 raspberry-sensors-0.2.5/README.md
+-rw-rw-rw-   0        0        0      501 2023-07-01 18:34:14.000000 raspberry-sensors-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-01 18:34:28.617002 raspberry-sensors-0.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-01 18:34:28.586895 raspberry-sensors-0.2.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-01 18:34:28.596843 raspberry-sensors-0.2.5/src/raspberry-sensors/
+-rw-rw-rw-   0        0        0        0 2023-06-28 10:37:28.000000 raspberry-sensors-0.2.5/src/raspberry-sensors/__init__.py
+-rw-rw-rw-   0        0        0     3315 2023-06-28 10:26:16.000000 raspberry-sensors-0.2.5/src/raspberry-sensors/sensors.py
+drwxrwxrwx   0        0        0        0 2023-07-01 18:34:28.608452 raspberry-sensors-0.2.5/src/raspberry_sensors.egg-info/
+-rw-rw-rw-   0        0        0     1787 2023-07-01 18:34:28.000000 raspberry-sensors-0.2.5/src/raspberry_sensors.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-07-01 18:34:28.000000 raspberry-sensors-0.2.5/src/raspberry_sensors.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 18:34:28.000000 raspberry-sensors-0.2.5/src/raspberry_sensors.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-01 18:34:28.000000 raspberry-sensors-0.2.5/src/raspberry_sensors.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 18:34:28.608452 raspberry-sensors-0.2.5/src/raspberry_sensors_Develper/
+-rw-rw-rw-   0        0        0     3400 2023-07-01 18:27:02.000000 raspberry-sensors-0.2.5/src/raspberry_sensors_Develper/sensors.py
```

### Comparing `raspberry-sensors-0.2.4/LICENSE` & `raspberry-sensors-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `raspberry-sensors-0.2.4/PKG-INFO` & `raspberry-sensors-0.2.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 Metadata-Version: 2.1
 Name: raspberry-sensors
-Version: 0.2.4
+Version: 0.2.5
 Summary: This package for getting values from sensors mh_z19, DHT, ads1015
 Author-email: Develper <testerlzt@mail.ru>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RaspberryPi sensors
 
 The library for getting values from sensors mh_z19, DHT, ads1015.
-Does not cause exceptions in case of errors, the cached value of sensors is also returned in case of an error
+*Does not cause exceptions in case of errors, the cached value of sensors is also returned in case of an error*
 
-*Examples*
+# Examples
 
 
-start
+### start
 
 ```
 from raspberry_sensors import sensors
 sensors = sensors.Sensors()
 ```
 
 
-disabling error logging
+### disabling error logging
 
 ```
 sensors = sensors.Sensors(loging_error=False)
 ```
 
 
-get the value of DHT
+### get the value of DHT
 
 ```
 sensors.get_dht(_type=22, gpio=4)
 # _type=22 - DHT22
 # _type=11 - DHT11
 # gpio - GPIO pin
 
 # return data ( dict )
-{"humidity": 36.0, "temperature": 21.0}
+# {"humidity": 36.0, "temperature": 21.0}
 ```
 
 
-get the value of ads
+### get the value of ads
 
 ```
 sensors.get_ads(chanel, interpolate=False, interpolate_min=0, interpolate_max=0)
 # chanel - the channel that you want to get the voltage from
 # interpolate - getting the normal value using interpolation
 # interpolate_min (use if interpolate True) - minimum value at 0 V
 # interpolate_max (use if interpolate True) - maximum value at 0 V
 
 # return data ( float )
 # if interpolate=False - voltage
 # if interpolate=True - the voltage value to which the interpolation formula is applied 
 ```
 
 
-get the value of mh_z19
+### get the value of mh_z19
 
 ```
 sensors.get_mhz(gpio=12, pwm=False)
 # gpio - GPIO pin
 # pwm - if pwm is True it will be read using pwm otherwise it is default
 
 # return data ( dict )
```

### Comparing `raspberry-sensors-0.2.4/README.md` & `raspberry-sensors-0.2.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 # RaspberryPi sensors
 
 The library for getting values from sensors mh_z19, DHT, ads1015.
-Does not cause exceptions in case of errors, the cached value of sensors is also returned in case of an error
+*Does not cause exceptions in case of errors, the cached value of sensors is also returned in case of an error*
 
-*Examples*
+# Examples
 
 
-start
+### start
 
 ```
 from raspberry_sensors import sensors
 sensors = sensors.Sensors()
 ```
 
 
-disabling error logging
+### disabling error logging
 
 ```
 sensors = sensors.Sensors(loging_error=False)
 ```
 
 
-get the value of DHT
+### get the value of DHT
 
 ```
 sensors.get_dht(_type=22, gpio=4)
 # _type=22 - DHT22
 # _type=11 - DHT11
 # gpio - GPIO pin
 
 # return data ( dict )
-{"humidity": 36.0, "temperature": 21.0}
+# {"humidity": 36.0, "temperature": 21.0}
 ```
 
 
-get the value of ads
+### get the value of ads
 
 ```
 sensors.get_ads(chanel, interpolate=False, interpolate_min=0, interpolate_max=0)
 # chanel - the channel that you want to get the voltage from
 # interpolate - getting the normal value using interpolation
 # interpolate_min (use if interpolate True) - minimum value at 0 V
 # interpolate_max (use if interpolate True) - maximum value at 0 V
 
 # return data ( float )
 # if interpolate=False - voltage
 # if interpolate=True - the voltage value to which the interpolation formula is applied 
 ```
 
 
-get the value of mh_z19
+### get the value of mh_z19
 
 ```
 sensors.get_mhz(gpio=12, pwm=False)
 # gpio - GPIO pin
 # pwm - if pwm is True it will be read using pwm otherwise it is default
 
 # return data ( dict )
```

### Comparing `raspberry-sensors-0.2.4/src/raspberry-sensors/sensors.py` & `raspberry-sensors-0.2.5/src/raspberry-sensors/sensors.py`

 * *Files identical despite different names*

### Comparing `raspberry-sensors-0.2.4/src/raspberry_sensors.egg-info/PKG-INFO` & `raspberry-sensors-0.2.5/src/raspberry_sensors.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 Metadata-Version: 2.1
 Name: raspberry-sensors
-Version: 0.2.4
+Version: 0.2.5
 Summary: This package for getting values from sensors mh_z19, DHT, ads1015
 Author-email: Develper <testerlzt@mail.ru>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RaspberryPi sensors
 
 The library for getting values from sensors mh_z19, DHT, ads1015.
-Does not cause exceptions in case of errors, the cached value of sensors is also returned in case of an error
+*Does not cause exceptions in case of errors, the cached value of sensors is also returned in case of an error*
 
-*Examples*
+# Examples
 
 
-start
+### start
 
 ```
 from raspberry_sensors import sensors
 sensors = sensors.Sensors()
 ```
 
 
-disabling error logging
+### disabling error logging
 
 ```
 sensors = sensors.Sensors(loging_error=False)
 ```
 
 
-get the value of DHT
+### get the value of DHT
 
 ```
 sensors.get_dht(_type=22, gpio=4)
 # _type=22 - DHT22
 # _type=11 - DHT11
 # gpio - GPIO pin
 
 # return data ( dict )
-{"humidity": 36.0, "temperature": 21.0}
+# {"humidity": 36.0, "temperature": 21.0}
 ```
 
 
-get the value of ads
+### get the value of ads
 
 ```
 sensors.get_ads(chanel, interpolate=False, interpolate_min=0, interpolate_max=0)
 # chanel - the channel that you want to get the voltage from
 # interpolate - getting the normal value using interpolation
 # interpolate_min (use if interpolate True) - minimum value at 0 V
 # interpolate_max (use if interpolate True) - maximum value at 0 V
 
 # return data ( float )
 # if interpolate=False - voltage
 # if interpolate=True - the voltage value to which the interpolation formula is applied 
 ```
 
 
-get the value of mh_z19
+### get the value of mh_z19
 
 ```
 sensors.get_mhz(gpio=12, pwm=False)
 # gpio - GPIO pin
 # pwm - if pwm is True it will be read using pwm otherwise it is default
 
 # return data ( dict )
```

### Comparing `raspberry-sensors-0.2.4/src/raspberry_sensors_Develper/sensors.py` & `raspberry-sensors-0.2.5/src/raspberry_sensors_Develper/sensors.py`

 * *Files identical despite different names*

