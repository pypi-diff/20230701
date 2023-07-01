# Comparing `tmp/pyezviz-0.2.1.6.tar.gz` & `tmp/pyezviz-0.2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyezviz-0.2.1.6.tar", last modified: Mon Jun 26 05:50:06 2023, max compression
+gzip compressed data, was "pyezviz-0.2.1.7.tar", last modified: Sat Jul  1 18:05:02 2023, max compression
```

## Comparing `pyezviz-0.2.1.6.tar` & `pyezviz-0.2.1.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:50:06.358931 pyezviz-0.2.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-26 05:50:06.358931 pyezviz-0.2.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:50:06.358931 pyezviz-0.2.1.6/pyezviz/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/pyezviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/pyezviz/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/pyezviz/api_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/pyezviz/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/pyezviz/cas.py
--rw-r--r--   0 runner    (1001) docker     (123)    60024 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/pyezviz/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/pyezviz/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/pyezviz/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/pyezviz/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/pyezviz/test_cam_rtsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/pyezviz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:50:06.358931 pyezviz-0.2.1.6/pyezviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-26 05:50:06.000000 pyezviz-0.2.1.6/pyezviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-26 05:50:06.000000 pyezviz-0.2.1.6/pyezviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 05:50:06.000000 pyezviz-0.2.1.6/pyezviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 05:50:06.000000 pyezviz-0.2.1.6/pyezviz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 05:50:06.000000 pyezviz-0.2.1.6/pyezviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 05:50:06.000000 pyezviz-0.2.1.6/pyezviz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 05:50:06.358931 pyezviz-0.2.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:05:02.278302 pyezviz-0.2.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-01 18:05:02.278302 pyezviz-0.2.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:05:02.278302 pyezviz-0.2.1.7/pyezviz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/pyezviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/pyezviz/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/pyezviz/api_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/pyezviz/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/pyezviz/cas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61784 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/pyezviz/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/pyezviz/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/pyezviz/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/pyezviz/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/pyezviz/test_cam_rtsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/pyezviz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:05:02.278302 pyezviz-0.2.1.7/pyezviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-01 18:05:02.000000 pyezviz-0.2.1.7/pyezviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-01 18:05:02.000000 pyezviz-0.2.1.7/pyezviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 18:05:02.000000 pyezviz-0.2.1.7/pyezviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-01 18:05:02.000000 pyezviz-0.2.1.7/pyezviz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-01 18:05:02.000000 pyezviz-0.2.1.7/pyezviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-01 18:05:02.000000 pyezviz-0.2.1.7/pyezviz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 18:05:02.278302 pyezviz-0.2.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-01 18:04:52.000000 pyezviz-0.2.1.7/setup.py
```

### Comparing `pyezviz-0.2.1.6/LICENSE.md` & `pyezviz-0.2.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.6/README.md` & `pyezviz-0.2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.6/pyezviz/__init__.py` & `pyezviz-0.2.1.7/pyezviz/__init__.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.6/pyezviz/__main__.py` & `pyezviz-0.2.1.7/pyezviz/__main__.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.6/pyezviz/api_endpoints.py` & `pyezviz-0.2.1.7/pyezviz/api_endpoints.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.6/pyezviz/camera.py` & `pyezviz-0.2.1.7/pyezviz/camera.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.6/pyezviz/cas.py` & `pyezviz-0.2.1.7/pyezviz/cas.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.6/pyezviz/client.py` & `pyezviz-0.2.1.7/pyezviz/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -728,14 +728,17 @@
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["resultCode"] != "0":
+            if json_output["resultCode"] == "-1":
+                _LOGGER.warning("Server busy, retrying %s", max_retries)
+                return self.get_storage_status(serial, max_retries + 1)
             raise PyEzvizError(
                 f"Could not get device storage status: Got {json_output})"
             )
 
         return json_output["storageStatus"]
 
     def sound_alarm(self, serial: str, enable: int = 1, max_retries: int = 0) -> bool:
@@ -940,14 +943,17 @@
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["resultCode"] != "0":
+            if json_output["resultCode"] == "-1":
+                _LOGGER.warning("Server busy, retrying %s", max_retries)
+                return self.reboot_camera(serial, delay, operation, max_retries + 1)
             raise PyEzvizError(f"Could not reboot device {json_output})")
 
         return True
 
     def get_group_defence_mode(self, max_retries: int = 0) -> Any:
         """Get group arm status. The alarm arm/disarm concept on 1st page of app."""
 
@@ -1203,14 +1209,17 @@
                 + str(req.text)
             ) from err
 
         if json_output["resultCode"] == "20002":
             raise EzvizAuthVerificationCode(f"MFA code required: Got {json_output})")
 
         if json_output["resultCode"] != "0":
+            if json_output["resultCode"] == "-1":
+                _LOGGER.warning("Server busy, retrying %s", max_retries)
+                return self.get_cam_key(serial, smscode, max_retries + 1)
             raise PyEzvizError(
                 f"Could not get camera encryption key: Got {json_output})"
             )
 
         return json_output
 
     def create_panoramic(self, serial: str, max_retries: int = 0) -> Any:
@@ -1244,14 +1253,17 @@
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["resultCode"] != "0":
+            if json_output["resultCode"] == "-1":
+                _LOGGER.warning("Server busy, retrying %s", max_retries)
+                return self.create_panoramic(serial, max_retries + 1)
             raise PyEzvizError(
                 f"Could not send command to create panoramic photo: Got {json_output})"
             )
 
         return json_output
 
     def return_panoramic(self, serial: str, max_retries: int = 0) -> Any:
@@ -1285,14 +1297,17 @@
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["resultCode"] != "0":
+            if json_output["resultCode"] == "-1":
+                _LOGGER.warning("Server busy, retrying %s", max_retries)
+                return self.return_panoramic(serial, max_retries + 1)
             raise PyEzvizError(f"Could retrieve panoramic photo: Got {json_output})")
 
         return json_output
 
     def ptz_control_coordinates(
         self, serial: str, x_axis: float, y_axis: float
     ) -> bool:
@@ -1487,14 +1502,19 @@
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["resultCode"] != "0":
+            if json_output["resultCode"] == "-1":
+                _LOGGER.warning("Server busy, retrying %s", max_retries)
+                return self.api_set_defence_schedule(
+                    serial, schedule, enable, max_retries + 1
+                )
             raise PyEzvizError(f"Could not set the schedule: Got {json_output})")
 
         return True
 
     def api_set_defence_mode(self, mode: DefenseModeType, max_retries: int = 0) -> bool:
         """Set defence mode for all devices. The alarm panel from main page is used."""
         if max_retries > MAX_RETRIES:
@@ -1679,14 +1699,19 @@
         try:
             response_json = req.json()
 
         except ValueError as err:
             raise PyEzvizError("Could not decode response:" + str(err)) from err
 
         if response_json["resultCode"] != "0":
+            if response_json["resultCode"] == "-1":
+                _LOGGER.warning("Server busy, retrying %s", max_retries)
+                return self.detection_sensibility(
+                    serial, sensibility, type_value, max_retries + 1
+                )
             raise PyEzvizError(
                 f"Unable to set detection sensibility. Got: {response_json}"
             )
 
         return True
 
     def get_detection_sensibility(
@@ -1722,14 +1747,19 @@
         try:
             response_json = req.json()
 
         except ValueError as err:
             raise PyEzvizError("Could not decode response:" + str(err)) from err
 
         if response_json["resultCode"] != "0":
+            if response_json["resultCode"] == "-1":
+                _LOGGER.warning("Server busy, retrying %s", max_retries)
+                return self.get_detection_sensibility(
+                    serial, type_value, max_retries + 1
+                )
             raise PyEzvizError(
                 f"Unable to get detection sensibility. Got: {response_json}"
             )
 
         if response_json["algorithmConfig"]["algorithmList"]:
             for idx in response_json["algorithmConfig"]["algorithmList"]:
                 if idx["type"] == type_value:
```

### Comparing `pyezviz-0.2.1.6/pyezviz/constants.py` & `pyezviz-0.2.1.7/pyezviz/constants.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.6/pyezviz/exceptions.py` & `pyezviz-0.2.1.7/pyezviz/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.6/pyezviz/mqtt.py` & `pyezviz-0.2.1.7/pyezviz/mqtt.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.6/pyezviz/test_cam_rtsp.py` & `pyezviz-0.2.1.7/pyezviz/test_cam_rtsp.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.6/pyezviz/utils.py` & `pyezviz-0.2.1.7/pyezviz/utils.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.6/setup.py` & `pyezviz-0.2.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyezviz',
-    version="0.2.1.6",
+    version="0.2.1.7",
     license='Apache Software License 2.0',
     author='Pierre Ourdouille',
     author_email='baqs@users.github.com',
     description='Pilot your Ezviz cameras',
     long_description="Pilot your Ezviz cameras with this module. Please view readme on github",
     url='http://github.com/baqs/pyEzviz/',
     packages=setuptools.find_packages(),
```

