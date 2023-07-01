# Comparing `tmp/sessypy-0.0.9.tar.gz` & `tmp/sessypy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sessypy-0.0.9.tar", last modified: Fri Jun  2 21:02:28 2023, max compression
+gzip compressed data, was "sessypy-0.1.0.tar", last modified: Sat Jul  1 15:05:02 2023, max compression
```

## Comparing `sessypy-0.0.9.tar` & `sessypy-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:02:28.013666 sessypy-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-02 21:02:14.000000 sessypy-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-02 21:02:28.013666 sessypy-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-02 21:02:14.000000 sessypy-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-02 21:02:14.000000 sessypy-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-02 21:02:28.013666 sessypy-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:02:28.005665 sessypy-0.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:02:28.009666 sessypy-0.0.9/src/sessypy/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-02 21:02:14.000000 sessypy-0.0.9/src/sessypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-02 21:02:14.000000 sessypy-0.0.9/src/sessypy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-02 21:02:14.000000 sessypy-0.0.9/src/sessypy/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-06-02 21:02:14.000000 sessypy-0.0.9/src/sessypy/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-02 21:02:14.000000 sessypy-0.0.9/src/sessypy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:02:28.013666 sessypy-0.0.9/src/sessypy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-02 21:02:27.000000 sessypy-0.0.9/src/sessypy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-02 21:02:28.000000 sessypy-0.0.9/src/sessypy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 21:02:27.000000 sessypy-0.0.9/src/sessypy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 21:02:27.000000 sessypy-0.0.9/src/sessypy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 21:02:27.000000 sessypy-0.0.9/src/sessypy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:05:02.806926 sessypy-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-01 15:04:48.000000 sessypy-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-01 15:05:02.806926 sessypy-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-01 15:04:48.000000 sessypy-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-01 15:04:48.000000 sessypy-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-01 15:05:02.806926 sessypy-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:05:02.806926 sessypy-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:05:02.806926 sessypy-0.1.0/src/sessypy/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-01 15:04:48.000000 sessypy-0.1.0/src/sessypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-01 15:04:48.000000 sessypy-0.1.0/src/sessypy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-01 15:04:48.000000 sessypy-0.1.0/src/sessypy/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-07-01 15:04:48.000000 sessypy-0.1.0/src/sessypy/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-01 15:04:48.000000 sessypy-0.1.0/src/sessypy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:05:02.806926 sessypy-0.1.0/src/sessypy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-01 15:05:02.000000 sessypy-0.1.0/src/sessypy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-01 15:05:02.000000 sessypy-0.1.0/src/sessypy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 15:05:02.000000 sessypy-0.1.0/src/sessypy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-01 15:05:02.000000 sessypy-0.1.0/src/sessypy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-01 15:05:02.000000 sessypy-0.1.0/src/sessypy.egg-info/top_level.txt
```

### Comparing `sessypy-0.0.9/LICENSE` & `sessypy-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sessypy-0.0.9/PKG-INFO` & `sessypy-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sessypy
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python wrapper for Sessy REST API
 Home-page: https://github.com/PimDoos/sessypy
 Author: PimDoos
 License: GNU GPLv3
 Project-URL: Homepage, https://github.com/PimDoos/sessypy
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sessypy-0.0.9/src/sessypy/api.py` & `sessypy-0.1.0/src/sessypy/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         self.session = aiohttp.ClientSession(
             auth=BasicAuth(username, password),
             raise_for_status = True
         )
     
     async def get(self, command):
         return await self.request("GET", command)
-    async def post(self, command: SessyApiCommand, data: dict):
+    async def post(self, command: SessyApiCommand, data: dict = None):
         return await self.request("POST", command, data)
     
     async def request(self, method: str, command: SessyApiCommand, data = None):
         try:
             url = self._command_url(command)
             response = await self.session.request(method, url, json = data)
             return await response.json()
```

### Comparing `sessypy-0.0.9/src/sessypy/const.py` & `sessypy-0.1.0/src/sessypy/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     POWER_STRATEGY = f"{API_VERSION_1}/power/active_strategy"
 
     P1_DETAILS = f"{API_VERSION_1}/p1/details"
     P1_STATUS = f"{API_VERSION_1}/p1/status"
     
     SYSTEM_SETTINGS = f"{API_VERSION_1}/system/settings"
     SYSTEM_INFO = f"{API_VERSION_1}/system/info"
+    SYSTEM_RESTART = f"{API_VERSION_1}/system/restart"
     WIFI_STA_CREDENTIALS = f"{API_VERSION_1}/wifi_sta/credentials"
 
 
 class SessyPowerStrategy(str, Enum):
     API = "POWER_STRATEGY_API"
     NOM = "POWER_STRATEGY_NOM"
     ROI = "POWER_STRATEGY_ROI"
```

### Comparing `sessypy-0.0.9/src/sessypy/devices.py` & `sessypy-0.1.0/src/sessypy/devices.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,14 +39,20 @@
         return await self.api.post(SessyApiCommand.OTA_START, {"target": target.value})
     
     async def get_network_scan(self):
         return await self.api.get(SessyApiCommand.NETWORK_SCAN)
     
     async def get_network_status(self):
         return await self.api.get(SessyApiCommand.NETWORK_STATUS)
+    
+    async def get_system_info(self):
+        return await self.api.get(SessyApiCommand.SYSTEM_INFO)
+    
+    async def restart(self):
+        return await self.api.post(SessyApiCommand.SYSTEM_RESTART)
 
     async def set_wifi_credentials(self, ssid: str, password: str):
         return await self.api.post(SessyApiCommand.WIFI_STA_CREDENTIALS, {"ssid":ssid, "pass":password})
 
     async def close(self):
         await self.api.close()
     
@@ -70,29 +76,38 @@
     async def get_p1_status(self):
         return await self.api.get(SessyApiCommand.P1_STATUS)
 
     async def get_p1_details(self):
         return await self.api.get(SessyApiCommand.P1_DETAILS)
 
 class SessyCTMeter(SessyDevice):
-    pass    
+    async def get_ct_status(self):
+        return await self.api.get(SessyApiCommand.P1_STATUS)
+    
+    async def get_ct_details(self):
+        return await self.api.get(SessyApiCommand.P1_DETAILS)
 	
 
 """Connect to the API and determine the device type"""
 async def get_sessy_device(host: str, username: str, password: str) -> SessyDevice:
+    # Assume username == serial number, which is mostly correct
+    serial_number = username
 
+    # Identify devices by API call and first letter of serial number
     device_profiles = [
-        (SessyBattery, SessyApiCommand.POWER_STRATEGY),
-        (SessyP1Meter, SessyApiCommand.P1_STATUS),
-        #(SessyDevice, SessyApiCommand.NETWORK_STATUS),
+        (SessyBattery, SessyApiCommand.POWER_STRATEGY, "D"),
+        (SessyP1Meter, SessyApiCommand.P1_STATUS, "P"),
+        (SessyCTMeter, SessyApiCommand.P1_STATUS, "C"),
     ]
 
     api = SessyApi(host, username, password)
 
     for device_profile in device_profiles:
+        if serial_number[0].upper() != device_profile[2]:
+            continue
         try:
             await api.get(device_profile[1])
             return device_profile[0](api)
         except SessyConnectionException:
             pass
         except SessyNotSupportedException:
             pass
```

### Comparing `sessypy-0.0.9/src/sessypy.egg-info/PKG-INFO` & `sessypy-0.1.0/src/sessypy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sessypy
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python wrapper for Sessy REST API
 Home-page: https://github.com/PimDoos/sessypy
 Author: PimDoos
 License: GNU GPLv3
 Project-URL: Homepage, https://github.com/PimDoos/sessypy
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

