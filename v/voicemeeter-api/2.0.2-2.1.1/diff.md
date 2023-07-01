# Comparing `tmp/voicemeeter-api-2.0.2.tar.gz` & `tmp/voicemeeter_api-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicemeeter-api-2.0.2.tar", max compression
+gzip compressed data, was "voicemeeter_api-2.1.1.tar", max compression
```

## Comparing `voicemeeter-api-2.0.2.tar` & `voicemeeter_api-2.1.1.tar`

### file list

```diff
@@ -1,27 +1,26 @@
--rw-r--r--   0        0        0     1091 2022-06-16 12:51:04.818279 voicemeeter-api-2.0.2/LICENSE
--rw-r--r--   0        0        0     1111 2023-06-29 17:04:50.006953 voicemeeter-api-2.0.2/pyproject.toml
--rw-r--r--   0        0        0    16567 2023-06-25 12:44:09.209061 voicemeeter-api-2.0.2/README.md
--rw-r--r--   0        0        0       69 2022-07-31 06:38:44.483821 voicemeeter-api-2.0.2/voicemeeterlib/__init__.py
--rw-r--r--   0        0        0     8226 2023-06-23 19:51:19.906407 voicemeeter-api-2.0.2/voicemeeterlib/bus.py
--rw-r--r--   0        0        0     4239 2023-06-22 23:20:33.622570 voicemeeter-api-2.0.2/voicemeeterlib/cbindings.py
--rw-r--r--   0        0        0     1194 2023-06-22 23:31:24.097081 voicemeeter-api-2.0.2/voicemeeterlib/command.py
--rw-r--r--   0        0        0     5819 2023-06-22 09:43:14.446510 voicemeeter-api-2.0.2/voicemeeterlib/config.py
--rw-r--r--   0        0        0     1748 2022-07-07 14:44:58.387087 voicemeeter-api-2.0.2/voicemeeterlib/device.py
--rw-r--r--   0        0        0      273 2023-06-23 00:41:14.485078 voicemeeter-api-2.0.2/voicemeeterlib/error.py
--rw-r--r--   0        0        0     2099 2023-06-22 08:38:58.271443 voicemeeter-api-2.0.2/voicemeeterlib/event.py
--rw-r--r--   0        0        0     7792 2023-06-29 15:52:06.128626 voicemeeter-api-2.0.2/voicemeeterlib/factory.py
--rw-r--r--   0        0        0     1091 2023-06-22 23:31:40.238138 voicemeeter-api-2.0.2/voicemeeterlib/inst.py
--rw-r--r--   0        0        0     1800 2023-06-23 20:52:02.185334 voicemeeter-api-2.0.2/voicemeeterlib/iremote.py
--rw-r--r--   0        0        0     2352 2023-06-22 02:21:02.337418 voicemeeter-api-2.0.2/voicemeeterlib/kinds.py
--rw-r--r--   0        0        0     1063 2023-06-22 23:31:57.569332 voicemeeter-api-2.0.2/voicemeeterlib/macrobutton.py
--rw-r--r--   0        0        0     1130 2023-06-21 12:24:03.433043 voicemeeter-api-2.0.2/voicemeeterlib/meta.py
--rw-r--r--   0        0        0     6486 2023-06-29 16:53:17.199263 voicemeeter-api-2.0.2/voicemeeterlib/misc.py
--rw-r--r--   0        0        0     1968 2023-06-21 12:25:36.590976 voicemeeter-api-2.0.2/voicemeeterlib/recorder.py
--rw-r--r--   0        0        0    11082 2023-06-29 17:03:12.450592 voicemeeter-api-2.0.2/voicemeeterlib/remote.py
--rw-r--r--   0        0        0    15325 2023-06-23 19:51:13.562428 voicemeeter-api-2.0.2/voicemeeterlib/strip.py
--rw-r--r--   0        0        0     2277 2023-06-23 16:22:05.659320 voicemeeter-api-2.0.2/voicemeeterlib/subject.py
--rw-r--r--   0        0        0     2978 2023-06-25 02:33:59.383974 voicemeeter-api-2.0.2/voicemeeterlib/updater.py
--rw-r--r--   0        0        0     1971 2023-06-29 16:15:53.063554 voicemeeter-api-2.0.2/voicemeeterlib/util.py
--rw-r--r--   0        0        0     4470 2022-08-08 13:33:38.448073 voicemeeter-api-2.0.2/voicemeeterlib/vban.py
--rw-r--r--   0        0        0    17744 2023-06-29 17:05:54.081464 voicemeeter-api-2.0.2/setup.py
--rw-r--r--   0        0        0    16380 2023-06-29 17:05:54.126598 voicemeeter-api-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-06-16 12:51:04.818279 voicemeeter_api-2.1.1/LICENSE
+-rw-r--r--   0        0        0     1111 2023-07-01 18:51:25.724767 voicemeeter_api-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0    17394 2023-07-01 18:51:25.723761 voicemeeter_api-2.1.1/README.md
+-rw-r--r--   0        0        0       69 2022-07-31 06:38:44.483821 voicemeeter_api-2.1.1/voicemeeterlib/__init__.py
+-rw-r--r--   0        0        0     8226 2023-06-23 19:51:19.906407 voicemeeter_api-2.1.1/voicemeeterlib/bus.py
+-rw-r--r--   0        0        0     4239 2023-06-22 23:20:33.622570 voicemeeter_api-2.1.1/voicemeeterlib/cbindings.py
+-rw-r--r--   0        0        0     1194 2023-06-22 23:31:24.097081 voicemeeter_api-2.1.1/voicemeeterlib/command.py
+-rw-r--r--   0        0        0     5819 2023-06-22 09:43:14.446510 voicemeeter_api-2.1.1/voicemeeterlib/config.py
+-rw-r--r--   0        0        0     1748 2022-07-07 14:44:58.387087 voicemeeter_api-2.1.1/voicemeeterlib/device.py
+-rw-r--r--   0        0        0      273 2023-06-23 00:41:14.485078 voicemeeter_api-2.1.1/voicemeeterlib/error.py
+-rw-r--r--   0        0        0     2099 2023-06-22 08:38:58.271443 voicemeeter_api-2.1.1/voicemeeterlib/event.py
+-rw-r--r--   0        0        0     7792 2023-06-29 15:52:06.128626 voicemeeter_api-2.1.1/voicemeeterlib/factory.py
+-rw-r--r--   0        0        0     1091 2023-06-22 23:31:40.238138 voicemeeter_api-2.1.1/voicemeeterlib/inst.py
+-rw-r--r--   0        0        0     1800 2023-06-23 20:52:02.185334 voicemeeter_api-2.1.1/voicemeeterlib/iremote.py
+-rw-r--r--   0        0        0     2352 2023-06-22 02:21:02.337418 voicemeeter_api-2.1.1/voicemeeterlib/kinds.py
+-rw-r--r--   0        0        0     1063 2023-06-22 23:31:57.569332 voicemeeter_api-2.1.1/voicemeeterlib/macrobutton.py
+-rw-r--r--   0        0        0     1130 2023-06-21 12:24:03.433043 voicemeeter_api-2.1.1/voicemeeterlib/meta.py
+-rw-r--r--   0        0        0     6485 2023-07-01 18:51:25.725768 voicemeeter_api-2.1.1/voicemeeterlib/misc.py
+-rw-r--r--   0        0        0     6739 2023-07-01 18:30:01.004734 voicemeeter_api-2.1.1/voicemeeterlib/recorder.py
+-rw-r--r--   0        0        0    11082 2023-06-29 17:03:12.450592 voicemeeter_api-2.1.1/voicemeeterlib/remote.py
+-rw-r--r--   0        0        0    15325 2023-06-23 19:51:13.562428 voicemeeter_api-2.1.1/voicemeeterlib/strip.py
+-rw-r--r--   0        0        0     2277 2023-06-23 16:22:05.659320 voicemeeter_api-2.1.1/voicemeeterlib/subject.py
+-rw-r--r--   0        0        0     2978 2023-06-25 02:33:59.383974 voicemeeter_api-2.1.1/voicemeeterlib/updater.py
+-rw-r--r--   0        0        0     1971 2023-06-30 17:58:26.046029 voicemeeter_api-2.1.1/voicemeeterlib/util.py
+-rw-r--r--   0        0        0     4650 2023-07-01 18:51:25.726767 voicemeeter_api-2.1.1/voicemeeterlib/vban.py
+-rw-r--r--   0        0        0    17226 1970-01-01 00:00:00.000000 voicemeeter_api-2.1.1/PKG-INFO
```

### Comparing `voicemeeter-api-2.0.2/LICENSE` & `voicemeeter_api-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-2.0.2/pyproject.toml` & `voicemeeter_api-2.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "voicemeeter-api"
-version = "2.0.2"
+version = "2.1.1"
 description = "A Python wrapper for the Voiceemeter API"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/voicemeeter-api-python"
 
 packages = [
```

### Comparing `voicemeeter-api-2.0.2/README.md` & `voicemeeter_api-2.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -394,39 +394,74 @@
 
 -   `play()`
 -   `stop()`
 -   `pause()`
 -   `record()`
 -   `ff()`
 -   `rew()`
--   `load(<filepath>)`: string
+-   `load(filepath)`: raw string
+-   `goto(time_string)`: time string in format `hh:mm:ss`
+-   `filetype(filetype)`: string, ("wav", "aiff", "bwf", "mp3")
 
 The following properties are available
 
--   `loop`: boolean
 -   `A1 - A5`: boolean
 -   `B1 - A3`: boolean
+-   `samplerate`: int, (22050, 24000, 32000, 44100, 48000, 88200, 96000, 176400, 192000)
+-   `bitresolution`: int, (8, 16, 24, 32)
+-   `channel`: int, from 1 to 8
+-   `kbps`: int, (32, 40, 48, 56, 64, 80, 96, 112, 128, 160, 192, 224, 256, 320)
+-   `gain`: float, from -60.0 to 12.0
 
 example:
 
 ```python
 vm.recorder.play()
 vm.recorder.stop()
 
-# Enable loop play
-vm.recorder.loop = True
-
 # Disable recorder out channel B2
 vm.recorder.B2 = False
 
 # filepath as raw string
 vm.recorder.load(r'C:\music\mytune.mp3')
+
+# set the goto time to 1m 30s
+vm.recorder.goto("00:01:30")
 ```
 
-Recorder properties are defined as write only.
+#### Recorder.Mode
+
+The following properties are available
+
+-   `recbus`: boolean
+-   `playonload`: boolean
+-   `loop`: boolean
+-   `multitrack`: boolean
+
+example:
+
+```python
+# Enable loop play
+vm.recorder.mode.loop = True
+```
+
+#### Recorder.ArmStrip[i]|ArmBus[i]
+
+The following method is available
+
+-   `set(val)`: boolean
+
+example:
+
+```python
+# Arm strip 3
+vm.recorder.armstrip[3].set(True)
+# Arm bus 0
+vm.recorder.armbus[0].set(True)
+```
 
 ### VBAN
 
 -   `vm.vban.enable()` `vm.vban.disable()` Turn VBAN on or off
 
 ##### Instream | Outstream
 
@@ -590,26 +625,24 @@
 
 ```python
 vm.option.sr = 48000
 ```
 
 The following methods are available:
 
--   `buffer(driver, buffer)` : Set buffer size for particular audio driver.
+-   `buffer(driver, buf)` : Set buffer size for particular audio driver.
+    -   buf: int, from 128 to 2048
+    -   driver:str, ("mme", "wdm", "ks", "asio")
 
 example:
 
 ```python
 vm.option.buffer("wdm", 512)
 ```
 
-driver defined as one of ("mme", "wdm", "ks", "asio")
-
-buffer, from 128 to 2048
-
 ##### delay[i]
 
 -   `get()`: int
 -   `set(delay)`: int, from 0 to 500
 
 example:
 
@@ -660,15 +693,15 @@
 ```python
 vm.strip[0].apply(mute: True, gain: 3.2, A1: True)
 vm.vban.outstream[0].apply(on: True, name: 'streamname', bit: 24)
 ```
 
 ## Config Files
 
-`vm.apply_config(<configname>)`
+`vm.apply_config(configname)`
 
 You may load config files in TOML format.
 Three example configs have been included with the package. Remember to save
 current settings before loading a user config. To set one you may do:
 
 ```python
 import voicemeeterlib
```

### Comparing `voicemeeter-api-2.0.2/voicemeeterlib/bus.py` & `voicemeeter_api-2.1.1/voicemeeterlib/bus.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-2.0.2/voicemeeterlib/cbindings.py` & `voicemeeter_api-2.1.1/voicemeeterlib/cbindings.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-2.0.2/voicemeeterlib/command.py` & `voicemeeter_api-2.1.1/voicemeeterlib/command.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-2.0.2/voicemeeterlib/config.py` & `voicemeeter_api-2.1.1/voicemeeterlib/config.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-2.0.2/voicemeeterlib/device.py` & `voicemeeter_api-2.1.1/voicemeeterlib/device.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-2.0.2/voicemeeterlib/event.py` & `voicemeeter_api-2.1.1/voicemeeterlib/event.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-2.0.2/voicemeeterlib/factory.py` & `voicemeeter_api-2.1.1/voicemeeterlib/factory.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-2.0.2/voicemeeterlib/inst.py` & `voicemeeter_api-2.1.1/voicemeeterlib/inst.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-2.0.2/voicemeeterlib/iremote.py` & `voicemeeter_api-2.1.1/voicemeeterlib/iremote.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-2.0.2/voicemeeterlib/kinds.py` & `voicemeeter_api-2.1.1/voicemeeterlib/kinds.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-2.0.2/voicemeeterlib/macrobutton.py` & `voicemeeter_api-2.1.1/voicemeeterlib/macrobutton.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-2.0.2/voicemeeterlib/meta.py` & `voicemeeter_api-2.1.1/voicemeeterlib/meta.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-2.0.2/voicemeeterlib/misc.py` & `voicemeeter_api-2.1.1/voicemeeterlib/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import Optional
 
-from .error import VMError
 from .iremote import IRemote
 from .kinds import kinds_all
 
 
 class FX(IRemote):
     def __str__(self):
         return f"{type(self).__name__}"
@@ -192,15 +191,15 @@
     def sr(self) -> int:
         return int(self.getter("sr"))
 
     @sr.setter
     def sr(self, val: int):
         opts = (44100, 48000, 88200, 96000, 176400, 192000)
         if val not in opts:
-            raise VMError(f"Expected one of: {opts}")
+            self.logger.warning(f"sr got: {val} but expected a value in {opts}")
         self.setter("sr", val)
 
     @property
     def asiosr(self) -> bool:
         return self.getter("asiosr") == 1
 
     @asiosr.setter
```

### Comparing `voicemeeter-api-2.0.2/voicemeeterlib/remote.py` & `voicemeeter_api-2.1.1/voicemeeterlib/remote.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-2.0.2/voicemeeterlib/strip.py` & `voicemeeter_api-2.1.1/voicemeeterlib/strip.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-2.0.2/voicemeeterlib/subject.py` & `voicemeeter_api-2.1.1/voicemeeterlib/subject.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-2.0.2/voicemeeterlib/updater.py` & `voicemeeter_api-2.1.1/voicemeeterlib/updater.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-2.0.2/voicemeeterlib/util.py` & `voicemeeter_api-2.1.1/voicemeeterlib/util.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-2.0.2/voicemeeterlib/vban.py` & `voicemeeter_api-2.1.1/voicemeeterlib/vban.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from abc import abstractmethod
 
-from .error import VMError
 from .iremote import IRemote
 
 
 class VbanStream(IRemote):
     """
     Implements the common interface
 
@@ -46,66 +45,68 @@
     @property
     def port(self) -> int:
         return int(self.getter("port"))
 
     @port.setter
     def port(self, val: int):
         if not 1024 <= val <= 65535:
-            raise VMError("Expected value from 1024 to 65535")
+            self.logger.warning(
+                f"port got: {val} but expected a value from 1024 to 65535"
+            )
         self.setter("port", val)
 
     @property
     def sr(self) -> int:
         return int(self.getter("sr"))
 
     @sr.setter
     def sr(self, val: int):
         opts = (11025, 16000, 22050, 24000, 32000, 44100, 48000, 64000, 88200, 96000)
         if val not in opts:
-            raise VMError(f"Expected one of: {opts}")
+            self.logger.warning(f"sr got: {val} but expected a value in {opts}")
         self.setter("sr", val)
 
     @property
     def channel(self) -> int:
         return int(self.getter("channel"))
 
     @channel.setter
     def channel(self, val: int):
         if not 1 <= val <= 8:
-            raise VMError("Expected value from 1 to 8")
+            self.logger.warning(f"channel got: {val} but expected a value from 1 to 8")
         self.setter("channel", val)
 
     @property
     def bit(self) -> int:
         return 16 if (int(self.getter("bit") == 1)) else 24
 
     @bit.setter
     def bit(self, val: int):
         if val not in (16, 24):
-            raise VMError("Expected value 16 or 24")
+            self.logger.warning(f"bit got: {val} but expected value 16 or 24")
         self.setter("bit", 1 if (val == 16) else 2)
 
     @property
     def quality(self) -> int:
         return int(self.getter("quality"))
 
     @quality.setter
     def quality(self, val: int):
         if not 0 <= val <= 4:
-            raise VMError("Expected value from 0 to 4")
+            self.logger.warning(f"quality got: {val} but expected a value from 0 to 4")
         self.setter("quality", val)
 
     @property
     def route(self) -> int:
         return int(self.getter("route"))
 
     @route.setter
     def route(self, val: int):
         if not 0 <= val <= 8:
-            raise VMError("Expected value from 0 to 8")
+            self.logger.warning(f"route got: {val} but expected a value from 0 to 8")
         self.setter("route", val)
 
 
 class VbanInstream(VbanStream):
     """
     class representing a vban instream
```

### Comparing `voicemeeter-api-2.0.2/setup.py` & `voicemeeter_api-2.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,852 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: voicemeeter-api
+Version: 2.1.1
+Summary: A Python wrapper for the Voiceemeter API
+Home-page: https://github.com/onyx-and-iris/voicemeeter-api-python
+License: MIT
+Author: onyx-and-iris
+Author-email: code@onyxandiris.online
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
+Project-URL: Repository, https://github.com/onyx-and-iris/voicemeeter-api-python
+Description-Content-Type: text/markdown
 
-packages = \
-['voicemeeterlib']
+[![PyPI version](https://badge.fury.io/py/voicemeeter-api.svg)](https://badge.fury.io/py/voicemeeter-api)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/onyx-and-iris/voicemeeter-api-python/blob/dev/LICENSE)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+![Tests Status](./tests/basic.svg?dummy=8484744)
+![Tests Status](./tests/banana.svg?dummy=8484744)
+![Tests Status](./tests/potato.svg?dummy=8484744)
 
-package_data = \
-{'': ['*']}
+# Python Wrapper for Voicemeeter API
 
-extras_require = \
-{':python_version < "3.11"': ['tomli>=2.0.1,<3.0.0']}
-
-entry_points = \
-{'console_scripts': ['dsl = scripts:ex_dsl',
-                     'events = scripts:ex_events',
-                     'gui = scripts:ex_gui',
-                     'levels = scripts:ex_levels',
-                     'midi = scripts:ex_midi',
-                     'obs = scripts:ex_obs',
-                     'observer = scripts:ex_observer',
-                     'test = scripts:test']}
-
-setup_kwargs = {
-    'name': 'voicemeeter-api',
-    'version': '2.0.2',
-    'description': 'A Python wrapper for the Voiceemeter API',
-    'long_description': '[![PyPI version](https://badge.fury.io/py/voicemeeter-api.svg)](https://badge.fury.io/py/voicemeeter-api)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/onyx-and-iris/voicemeeter-api-python/blob/dev/LICENSE)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)\n![Tests Status](./tests/basic.svg?dummy=8484744)\n![Tests Status](./tests/banana.svg?dummy=8484744)\n![Tests Status](./tests/potato.svg?dummy=8484744)\n\n# Python Wrapper for Voicemeeter API\n\nThis package offers a Python interface for the Voicemeeter Remote C API.\n\nFor an outline of past/future changes refer to: [CHANGELOG](CHANGELOG.md)\n\n## Tested against\n\n-   Basic 1.0.8.8\n-   Banana 2.0.6.8\n-   Potato 3.0.2.8\n\n## Requirements\n\n-   [Voicemeeter](https://voicemeeter.com/)\n-   Python 3.10 or greater\n\n## Installation\n\n`pip install voicemeeter-api`\n\n## `Use`\n\nSimplest use case, use a context manager to request a Remote class of a kind.\n\nLogin and logout are handled for you in this scenario.\n\n#### `__main__.py`\n\n```python\nimport voicemeeterlib\n\n\nclass ManyThings:\n    def __init__(self, vm):\n        self.vm = vm\n\n    def things(self):\n        self.vm.strip[0].label = "podmic"\n        self.vm.strip[0].mute = True\n        print(\n            f"strip 0 ({self.vm.strip[0].label}) mute has been set to {self.vm.strip[0].mute}"\n        )\n\n    def other_things(self):\n        self.vm.bus[3].gain = -6.3\n        self.vm.bus[4].eq.on = True\n        info = (\n            f"bus 3 gain has been set to {self.vm.bus[3].gain}",\n            f"bus 4 eq has been set to {self.vm.bus[4].eq.on}",\n        )\n        print("\\n".join(info))\n\n\ndef main():\n    KIND_ID = "banana"\n\n    with voicemeeterlib.api(KIND_ID) as vm:\n        do = ManyThings(vm)\n        do.things()\n        do.other_things()\n\n        # set many parameters at once\n        vm.apply(\n            {\n                "strip-2": {"A1": True, "B1": True, "gain": -6.0},\n                "bus-2": {"mute": True, "eq": {"on": True}},\n                "button-0": {"state": True},\n                "vban-in-0": {"on": True},\n                "vban-out-1": {"name": "streamname"},\n            }\n        )\n\n\nif __name__ == "__main__":\n    main()\n\n```\n\nOtherwise you must remember to call `vm.login()`, `vm.logout()` at the start/end of your code.\n\n## `KIND_ID`\n\nPass the kind of Voicemeeter as an argument. KIND_ID may be:\n\n-   `basic`\n-   `banana`\n-   `potato`\n\n## `Available commands`\n\n### Strip\n\nThe following properties are available.\n\n-   `mono`: boolean\n-   `solo`: boolean\n-   `mute`: boolean\n-   `gain`: float, from -60.0 to 12.0\n-   `audibility`: float, from 0.0 to 10.0\n-   `limit`: int, from -40 to 12\n-   `A1 - A5`, `B1 - B3`: boolean\n-   `label`: string\n-   `mc`: boolean\n-   `k`: int, from 0 to 4\n-   `bass`: float, from -12.0 to 12.0\n-   `mid`: float, from -12.0 to 12.0\n-   `treble`: float, from -12.0 to 12.0\n-   `reverb`: float, from 0.0 to 10.0\n-   `delay`: float, from 0.0 to 10.0\n-   `fx1`: float, from 0.0 to 10.0\n-   `fx2`: float, from 0.0 to 10.0\n-   `pan_x`: float, from -0.5 to 0.5\n-   `pan_y`: float, from 0.0 to 1.0\n-   `color_x`: float, from -0.5 to 0.5\n-   `color_y`: float, from 0.0 to 1.0\n-   `fx_x`: float, from -0.5 to 0.5\n-   `fx_y`: float, from 0.0 to 1.0\n-   `postreverb`: boolean\n-   `postdelay`: boolean\n-   `postfx1`: boolean\n-   `postfx2`: boolean\n\nexample:\n\n```python\nvm.strip[3].gain = 3.7\nprint(vm.strip[0].label)\n```\n\nThe following methods are available.\n\n-   `appgain(name, value)`: string, float, from 0.0 to 1.0\n\nSet the gain in db by value for the app matching name.\n\n-   `appmute(name, value)`: string, bool\n\nSet mute state as value for the app matching name.\n\nexample:\n\n```python\nvm.strip[5].appmute("Spotify", True)\nvm.strip[5].appgain("Spotify", 0.5)\n```\n\n#### Strip.Comp\n\nThe following properties are available.\n\n-   `knob`: float, from 0.0 to 10.0\n-   `gainin`: float, from -24.0 to 24.0\n-   `ratio`: float, from 1.0 to 8.0\n-   `threshold`: float, from -40.0 to -3.0\n-   `attack`: float, from 0.0 to 200.0\n-   `release`: float, from 0.0 to 5000.0\n-   `knee`: float, from 0.0 to 1.0\n-   `gainout`: float, from -24.0 to 24.0\n-   `makeup`: boolean\n\nexample:\n\n```python\nprint(vm.strip[4].comp.knob)\n```\n\nStrip Comp parameters are defined for PhysicalStrips.\n\n`knob` defined for all versions, all other parameters potato only.\n\n#### Strip.Gate\n\nThe following properties are available.\n\n-   `knob`: float, from 0.0 to 10.0\n-   `threshold`: float, from -60.0 to -10.0\n-   `damping`: float, from -60.0 to -10.0\n-   `bpsidechain`: int, from 100 to 4000\n-   `attack`: float, from 0.0 to 1000.0\n-   `hold`: float, from 0.0 to 5000.0\n-   `release`: float, from 0.0 to 5000.0\n\nexample:\n\n```python\nvm.strip[2].gate.attack = 300.8\n```\n\nStrip Gate parameters are defined for PhysicalStrips.\n\n`knob` defined for all versions, all other parameters potato only.\n\n#### Strip.Denoiser\n\nThe following properties are available.\n\n-   `knob`: float, from 0.0 to 10.0\n\nexample:\n\n```python\nvm.strip[0].denoiser.knob = 0.5\n```\n\nStrip Denoiser parameters are defined for PhysicalStrips, potato version only.\n\n#### Strip.EQ\n\nThe following properties are available.\n\n-   `on`: boolean\n-   `ab`: boolean\n\nexample:\n\n```python\nvm.strip[0].eq.ab = True\n```\n\nStrip EQ parameters are defined for PhysicalStrips, potato version only.\n\n##### Strip.Gainlayers\n\n-   `gain`: float, from -60.0 to 12.0\n\nexample:\n\n```python\nvm.strip[3].gainlayer[3].gain = 3.7\n```\n\nGainlayers are defined for potato version only.\n\n##### Strip.Levels\n\nThe following properties are available.\n\n-   `prefader`\n-   `postfader`\n-   `postmute`\n\nexample:\n\n```python\nprint(vm.strip[3].levels.prefader)\n```\n\nLevel properties will return -200.0 if no audio detected.\n\n### Bus\n\nThe following properties are available.\n\n-   `mono`: boolean\n-   `mute`: boolean\n-   `sel`: boolean\n-   `gain`: float, from -60.0 to 12.0\n-   `label`: string\n-   `returnreverb`: float, from 0.0 to 10.0\n-   `returndelay`: float, from 0.0 to 10.0\n-   `returnfx1`: float, from 0.0 to 10.0\n-   `returnfx2`: float, from 0.0 to 10.0\n-   `monitor`: boolean\n\nexample:\n\n```python\nvm.bus[3].gain = 3.7\nprint(vm.bus[0].label)\n\nvm.bus[4].mono = True\n```\n\n##### Bus.EQ\n\nThe following properties are available.\n\n-   `on`: boolean\n-   `ab`: boolean\n\nexample:\n\n```python\nvm.bus[3].eq.on = True\n```\n\n##### Bus.Modes\n\nThe following properties are available.\n\n-   `normal`: boolean\n-   `amix`: boolean\n-   `bmix`: boolean\n-   `composite`: boolean\n-   `tvmix`: boolean\n-   `upmix21`: boolean\n-   `upmix41`: boolean\n-   `upmix61`: boolean\n-   `centeronly`: boolean\n-   `lfeonly`: boolean\n-   `rearonly`: boolean\n\nThe following methods are available.\n\n-   `get()`: Returns the current bus mode\n\nexample:\n\n```python\nvm.bus[4].mode.amix = True\n\nprint(vm.bus[2].mode.get())\n```\n\n##### Bus.Levels\n\nThe following properties are available.\n\n-   `all`\n\nexample:\n\n```python\nprint(vm.bus[0].levels.all)\n```\n\n`levels.all` will return -200.0 if no audio detected.\n\n### Strip | Bus\n\nThe following methods are available.\n\n-   `fadeto(amount, time)`: float, int\n-   `fadeby(amount, time)`: float, int\n\nModify gain to or by the selected amount in db over a time interval in ms.\n\nexample:\n\n```python\nvm.strip[0].fadeto(-10.3, 1000)\nvm.bus[3].fadeby(-5.6, 500)\n```\n\n#### Strip.Device | Bus.Device\n\nThe following properties are available\n\n-   `name`: str\n-   `sr`: int\n-   `wdm`: str\n-   `ks`: str\n-   `mme`: str\n-   `asio`: str\n\nexample:\n\n```python\nprint(vm.strip[0].device.name)\nvm.bus[0].device.asio = "Audient USB Audio ASIO Driver"\n```\n\nstrip|bus device parameters are defined for physical channels only.\n\nname, sr are read only. wdm, ks, mme, asio are write only.\n\n### Macrobuttons\n\nThe following properties are available.\n\n-   `state`: boolean\n-   `stateonly`: boolean\n-   `trigger`: boolean\n\nexample:\n\n```python\nvm.button[37].state = True\nvm.button[55].trigger = False\n```\n\n### Recorder\n\nThe following methods are available\n\n-   `play()`\n-   `stop()`\n-   `pause()`\n-   `record()`\n-   `ff()`\n-   `rew()`\n-   `load(<filepath>)`: string\n\nThe following properties are available\n\n-   `loop`: boolean\n-   `A1 - A5`: boolean\n-   `B1 - A3`: boolean\n\nexample:\n\n```python\nvm.recorder.play()\nvm.recorder.stop()\n\n# Enable loop play\nvm.recorder.loop = True\n\n# Disable recorder out channel B2\nvm.recorder.B2 = False\n\n# filepath as raw string\nvm.recorder.load(r\'C:\\music\\mytune.mp3\')\n```\n\nRecorder properties are defined as write only.\n\n### VBAN\n\n-   `vm.vban.enable()` `vm.vban.disable()` Turn VBAN on or off\n\n##### Instream | Outstream\n\nThe following properties are available.\n\n-   `on`: boolean\n-   `name`: string\n-   `ip`: string\n-   `port`: int, range from 1024 to 65535\n-   `sr`: int, (11025, 16000, 22050, 24000, 32000, 44100, 48000, 64000, 88200, 96000)\n-   `channel`: int, from 1 to 8\n-   `bit`: int, 16 or 24\n-   `quality`: int, from 0 to 4\n-   `route`: int, from 0 to 8\n\n`SR`, `channel` and `bit` are defined as:\n\n-   readonly for instreams.\n-   read and write for outstreams.\n\nexample:\n\n```python\n# turn VBAN on\nvm.vban.enable()\n\n# turn on vban instream 0\nvm.vban.instream[0].on = True\n\n# set bit property for outstream 3 to 24\nvm.vban.outstream[3].bit = 24\n```\n\n### Command\n\nCertain \'special\' commands are defined by the API as performing actions rather than setting values.\n\nThe following methods are available:\n\n-   `show()` : Bring Voiceemeter GUI to the front\n-   `shutdown()` : Shuts down the GUI\n-   `restart()` : Restart the audio engine\n-   `reset()`: Applies the `reset` config. (phys strip B1, virt strip A1, gains, comp, gate 0.0, mute, mono, solo, eq false)\n\nThe following properties are available.\n\n-   `showvbanchat`: boolean\n-   `lock`: boolean\n\nexample:\n\n```python\nvm.command.restart()\nvm.command.showvbanchat = True\n```\n\n`showvbanchat` and `lock` are write only.\n\n### Device\n\n-   `ins` `outs` : Returns the number of input/output devices\n-   `input(i)` `output(i)` : Returns a dict of device properties for device[i]\n\nexample:\n\n```python\nimport voicemeeterlib\nwith voicemeeterlib.api(KIND_ID) as vm:\n    for i in range(vm.device.ins):\n        print(vm.device.input(i))\n```\n\n### FX\n\nThe following properties are available:\n\n-   `reverb`: boolean\n-   `reverb_ab`: boolean\n-   `delay`: boolean\n-   `delay_ab`: boolean\n\nexample:\n\n```python\nvm.fx.reverb_ab = True\n```\n\n### Patch\n\nThe following properties are available:\n\n-   `postfadercomposite`: boolean\n-   `postfxinsert`: boolean\n\nexample:\n\n```python\nvm.patch.postfxinsert = False\n```\n\n##### asio[i]\n\n-   `get()`: int\n-   `set(patch_in)`: int, valid range determined by connected device.\n\nexample:\n\n```python\nvm.patch.asio[3].set(4)\n```\n\ni, from 0 to 10\n\n##### A2[i] - A5[i]\n\n-   `get()`: int\n-   `set(patch_out)`: int, valid range determined by connected device.\n\nexample:\n\n```python\nvm.patch.A3[5].set(3)\n```\n\ni, from 0 to 8.\n\n##### composite[i]\n\n-   `get()`: int\n-   `set(channel)`: int, from 0 up to number of channels depending on version.\n\nexample:\n\n```python\nvm.patch.composite[7].set(4)\n```\n\ni, from 0 to 8.\n\n##### insert[i]\n\n-   `on`: boolean\n\nexample:\n\n```python\nvm.patch.insert[18].on = True\n```\n\ni, from 0 up to number of channels depending on version.\n\n### Option\n\nThe following properties are available:\n\n-   `sr`: int\n-   `asiosr`: boolean\n-   `monitoronsel`: boolean\n\nexample:\n\n```python\nvm.option.sr = 48000\n```\n\nThe following methods are available:\n\n-   `buffer(driver, buffer)` : Set buffer size for particular audio driver.\n\nexample:\n\n```python\nvm.option.buffer("wdm", 512)\n```\n\ndriver defined as one of ("mme", "wdm", "ks", "asio")\n\nbuffer, from 128 to 2048\n\n##### delay[i]\n\n-   `get()`: int\n-   `set(delay)`: int, from 0 to 500\n\nexample:\n\n```python\nvm.option.delay[4].set(30)\n```\n\ni, from 0 up to 4.\n\n### Midi\n\nThe following properties are available:\n\n-   `channel`: int, returns the midi channel\n-   `current`: int, returns the current (or most recently pressed) key\n\nThe following methods are available:\n\n-   `get(key)`: int, returns most recent velocity value for a key\n\nexample:\n\n```python\nprint(vm.midi.get(12))\n```\n\nget() may return None if no value for requested key in midi cache\n\n### Multiple parameters\n\n-   `apply`\n    Set many strip/bus/macrobutton/vban parameters at once, for example:\n\n```python\nvm.apply(\n    {\n        "strip-2": {"A1": True, "B1": True, "gain": -6.0},\n        "bus-2": {"mute": True, "eq": {"on": True}},\n        "button-0": {"state": True},\n        "vban-in-0": {"on": True},\n        "vban-out-1": {"name": "streamname"},\n    }\n)\n```\n\nOr for each class you may do:\n\n```python\nvm.strip[0].apply(mute: True, gain: 3.2, A1: True)\nvm.vban.outstream[0].apply(on: True, name: \'streamname\', bit: 24)\n```\n\n## Config Files\n\n`vm.apply_config(<configname>)`\n\nYou may load config files in TOML format.\nThree example configs have been included with the package. Remember to save\ncurrent settings before loading a user config. To set one you may do:\n\n```python\nimport voicemeeterlib\nwith voicemeeterlib.api(\'banana\') as vm:\n    vm.apply_config(\'example\')\n```\n\nwill load a user config file at configs/banana/example.toml for Voicemeeter Banana.\n\n## Events\n\nBy default, NO events are listened for. Use events kwargs to enable specific event types.\n\nexample:\n\n```python\nimport voicemeeterlib\n# Set event updates to occur every 50ms\n# Listen for level updates only\nwith voicemeeterlib.api(\'banana\', ratelimit=0.05, ldirty=True}) as vm:\n    ...\n```\n\n#### `vm.observer`\n\nUse the Subject class to register an app as event observer.\n\nThe following methods are available:\n\n-   `add`: registers an app as an event observer\n-   `remove`: deregisters an app as an event observer\n\nexample:\n\n```python\n# register an app to receive updates\nclass App():\n    def __init__(self, vm):\n        vm.observer.add(self)\n        ...\n```\n\n#### `vm.event`\n\nUse the event class to toggle updates as necessary.\n\nThe following properties are available:\n\n-   `pdirty`: boolean\n-   `mdirty`: boolean\n-   `midi`: boolean\n-   `ldirty`: boolean\n\nexample:\n\n```python\nvm.event.ldirty = True\n\nvm.event.pdirty = False\n```\n\nOr add, remove a list of events.\n\nThe following methods are available:\n\n-   `add()`\n-   `remove()`\n-   `get()`\n\nexample:\n\n```python\nvm.event.remove(["pdirty", "mdirty", "midi"])\n\n# get a list of currently subscribed\nprint(vm.event.get())\n```\n\n## Remote class\n\n`voicemeeterlib.api(KIND_ID: str)`\n\nYou may pass the following optional keyword arguments:\n\n-   `sync`: boolean=False, force the getters to wait for dirty parameters to clear. For most cases leave this as False.\n-   `ratelimit`: float=0.033, how often to check for updates in ms.\n-   `pdirty`: boolean=False, parameter updates\n-   `mdirty`: boolean=False, macrobutton updates\n-   `midi`: boolean=False, midi updates\n-   `ldirty`: boolean=False, level updates\n\nAccess to lower level Getters and Setters are provided with these functions:\n\n-   `vm.get(param, is_string=False)`: For getting the value of any parameter. Set string to True if getting a property value expected to return a string.\n-   `vm.set(param, value)`: For setting the value of any parameter.\n\nexample:\n\n```python\nvm.get(\'Strip[2].Mute\')\nvm.set(\'Strip[4].Label\', \'stripname\')\nvm.set(\'Strip[0].Gain\', -3.6)\n```\n\nAccess to lower level polling functions are provided with the following property objects:\n\n#### `vm.pdirty`\n\nTrue iff a parameter has been updated.\n\n#### `vm.mdirty`\n\nTrue iff a macrobutton has been updated.\n\n#### `vm.ldirty`\n\nTrue iff a level has been updated.\n\n\n### Run tests\n\nTo run all tests:\n\n```\npytest -v\n```\n\n### Official Documentation\n\n-   [Voicemeeter Remote C API](https://github.com/onyx-and-iris/Voicemeeter-SDK/blob/update-docs/VoicemeeterRemoteAPI.pdf)\n',
-    'author': 'onyx-and-iris',
-    'author_email': 'code@onyxandiris.online',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/onyx-and-iris/voicemeeter-api-python',
-    'packages': packages,
-    'package_data': package_data,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
+This package offers a Python interface for the Voicemeeter Remote C API.
 
+For an outline of past/future changes refer to: [CHANGELOG](CHANGELOG.md)
+
+## Tested against
+
+-   Basic 1.0.8.8
+-   Banana 2.0.6.8
+-   Potato 3.0.2.8
+
+## Requirements
+
+-   [Voicemeeter](https://voicemeeter.com/)
+-   Python 3.10 or greater
+
+## Installation
+
+`pip install voicemeeter-api`
+
+## `Use`
+
+Simplest use case, use a context manager to request a Remote class of a kind.
+
+Login and logout are handled for you in this scenario.
+
+#### `__main__.py`
+
+```python
+import voicemeeterlib
+
+
+class ManyThings:
+    def __init__(self, vm):
+        self.vm = vm
+
+    def things(self):
+        self.vm.strip[0].label = "podmic"
+        self.vm.strip[0].mute = True
+        print(
+            f"strip 0 ({self.vm.strip[0].label}) mute has been set to {self.vm.strip[0].mute}"
+        )
+
+    def other_things(self):
+        self.vm.bus[3].gain = -6.3
+        self.vm.bus[4].eq.on = True
+        info = (
+            f"bus 3 gain has been set to {self.vm.bus[3].gain}",
+            f"bus 4 eq has been set to {self.vm.bus[4].eq.on}",
+        )
+        print("\n".join(info))
+
+
+def main():
+    KIND_ID = "banana"
+
+    with voicemeeterlib.api(KIND_ID) as vm:
+        do = ManyThings(vm)
+        do.things()
+        do.other_things()
+
+        # set many parameters at once
+        vm.apply(
+            {
+                "strip-2": {"A1": True, "B1": True, "gain": -6.0},
+                "bus-2": {"mute": True, "eq": {"on": True}},
+                "button-0": {"state": True},
+                "vban-in-0": {"on": True},
+                "vban-out-1": {"name": "streamname"},
+            }
+        )
+
+
+if __name__ == "__main__":
+    main()
+
+```
+
+Otherwise you must remember to call `vm.login()`, `vm.logout()` at the start/end of your code.
+
+## `KIND_ID`
+
+Pass the kind of Voicemeeter as an argument. KIND_ID may be:
+
+-   `basic`
+-   `banana`
+-   `potato`
+
+## `Available commands`
+
+### Strip
+
+The following properties are available.
+
+-   `mono`: boolean
+-   `solo`: boolean
+-   `mute`: boolean
+-   `gain`: float, from -60.0 to 12.0
+-   `audibility`: float, from 0.0 to 10.0
+-   `limit`: int, from -40 to 12
+-   `A1 - A5`, `B1 - B3`: boolean
+-   `label`: string
+-   `mc`: boolean
+-   `k`: int, from 0 to 4
+-   `bass`: float, from -12.0 to 12.0
+-   `mid`: float, from -12.0 to 12.0
+-   `treble`: float, from -12.0 to 12.0
+-   `reverb`: float, from 0.0 to 10.0
+-   `delay`: float, from 0.0 to 10.0
+-   `fx1`: float, from 0.0 to 10.0
+-   `fx2`: float, from 0.0 to 10.0
+-   `pan_x`: float, from -0.5 to 0.5
+-   `pan_y`: float, from 0.0 to 1.0
+-   `color_x`: float, from -0.5 to 0.5
+-   `color_y`: float, from 0.0 to 1.0
+-   `fx_x`: float, from -0.5 to 0.5
+-   `fx_y`: float, from 0.0 to 1.0
+-   `postreverb`: boolean
+-   `postdelay`: boolean
+-   `postfx1`: boolean
+-   `postfx2`: boolean
+
+example:
+
+```python
+vm.strip[3].gain = 3.7
+print(vm.strip[0].label)
+```
+
+The following methods are available.
+
+-   `appgain(name, value)`: string, float, from 0.0 to 1.0
+
+Set the gain in db by value for the app matching name.
+
+-   `appmute(name, value)`: string, bool
+
+Set mute state as value for the app matching name.
+
+example:
+
+```python
+vm.strip[5].appmute("Spotify", True)
+vm.strip[5].appgain("Spotify", 0.5)
+```
+
+#### Strip.Comp
+
+The following properties are available.
+
+-   `knob`: float, from 0.0 to 10.0
+-   `gainin`: float, from -24.0 to 24.0
+-   `ratio`: float, from 1.0 to 8.0
+-   `threshold`: float, from -40.0 to -3.0
+-   `attack`: float, from 0.0 to 200.0
+-   `release`: float, from 0.0 to 5000.0
+-   `knee`: float, from 0.0 to 1.0
+-   `gainout`: float, from -24.0 to 24.0
+-   `makeup`: boolean
+
+example:
+
+```python
+print(vm.strip[4].comp.knob)
+```
+
+Strip Comp parameters are defined for PhysicalStrips.
+
+`knob` defined for all versions, all other parameters potato only.
+
+#### Strip.Gate
+
+The following properties are available.
+
+-   `knob`: float, from 0.0 to 10.0
+-   `threshold`: float, from -60.0 to -10.0
+-   `damping`: float, from -60.0 to -10.0
+-   `bpsidechain`: int, from 100 to 4000
+-   `attack`: float, from 0.0 to 1000.0
+-   `hold`: float, from 0.0 to 5000.0
+-   `release`: float, from 0.0 to 5000.0
+
+example:
+
+```python
+vm.strip[2].gate.attack = 300.8
+```
+
+Strip Gate parameters are defined for PhysicalStrips.
+
+`knob` defined for all versions, all other parameters potato only.
+
+#### Strip.Denoiser
+
+The following properties are available.
+
+-   `knob`: float, from 0.0 to 10.0
+
+example:
+
+```python
+vm.strip[0].denoiser.knob = 0.5
+```
+
+Strip Denoiser parameters are defined for PhysicalStrips, potato version only.
+
+#### Strip.EQ
+
+The following properties are available.
+
+-   `on`: boolean
+-   `ab`: boolean
+
+example:
+
+```python
+vm.strip[0].eq.ab = True
+```
+
+Strip EQ parameters are defined for PhysicalStrips, potato version only.
+
+##### Strip.Gainlayers
+
+-   `gain`: float, from -60.0 to 12.0
+
+example:
+
+```python
+vm.strip[3].gainlayer[3].gain = 3.7
+```
+
+Gainlayers are defined for potato version only.
+
+##### Strip.Levels
+
+The following properties are available.
+
+-   `prefader`
+-   `postfader`
+-   `postmute`
+
+example:
+
+```python
+print(vm.strip[3].levels.prefader)
+```
+
+Level properties will return -200.0 if no audio detected.
+
+### Bus
+
+The following properties are available.
+
+-   `mono`: boolean
+-   `mute`: boolean
+-   `sel`: boolean
+-   `gain`: float, from -60.0 to 12.0
+-   `label`: string
+-   `returnreverb`: float, from 0.0 to 10.0
+-   `returndelay`: float, from 0.0 to 10.0
+-   `returnfx1`: float, from 0.0 to 10.0
+-   `returnfx2`: float, from 0.0 to 10.0
+-   `monitor`: boolean
+
+example:
+
+```python
+vm.bus[3].gain = 3.7
+print(vm.bus[0].label)
+
+vm.bus[4].mono = True
+```
+
+##### Bus.EQ
+
+The following properties are available.
+
+-   `on`: boolean
+-   `ab`: boolean
+
+example:
+
+```python
+vm.bus[3].eq.on = True
+```
+
+##### Bus.Modes
+
+The following properties are available.
+
+-   `normal`: boolean
+-   `amix`: boolean
+-   `bmix`: boolean
+-   `composite`: boolean
+-   `tvmix`: boolean
+-   `upmix21`: boolean
+-   `upmix41`: boolean
+-   `upmix61`: boolean
+-   `centeronly`: boolean
+-   `lfeonly`: boolean
+-   `rearonly`: boolean
+
+The following methods are available.
+
+-   `get()`: Returns the current bus mode
+
+example:
+
+```python
+vm.bus[4].mode.amix = True
+
+print(vm.bus[2].mode.get())
+```
+
+##### Bus.Levels
+
+The following properties are available.
+
+-   `all`
+
+example:
+
+```python
+print(vm.bus[0].levels.all)
+```
+
+`levels.all` will return -200.0 if no audio detected.
+
+### Strip | Bus
+
+The following methods are available.
+
+-   `fadeto(amount, time)`: float, int
+-   `fadeby(amount, time)`: float, int
+
+Modify gain to or by the selected amount in db over a time interval in ms.
+
+example:
+
+```python
+vm.strip[0].fadeto(-10.3, 1000)
+vm.bus[3].fadeby(-5.6, 500)
+```
+
+#### Strip.Device | Bus.Device
+
+The following properties are available
+
+-   `name`: str
+-   `sr`: int
+-   `wdm`: str
+-   `ks`: str
+-   `mme`: str
+-   `asio`: str
+
+example:
+
+```python
+print(vm.strip[0].device.name)
+vm.bus[0].device.asio = "Audient USB Audio ASIO Driver"
+```
+
+strip|bus device parameters are defined for physical channels only.
+
+name, sr are read only. wdm, ks, mme, asio are write only.
+
+### Macrobuttons
+
+The following properties are available.
+
+-   `state`: boolean
+-   `stateonly`: boolean
+-   `trigger`: boolean
+
+example:
+
+```python
+vm.button[37].state = True
+vm.button[55].trigger = False
+```
+
+### Recorder
+
+The following methods are available
+
+-   `play()`
+-   `stop()`
+-   `pause()`
+-   `record()`
+-   `ff()`
+-   `rew()`
+-   `load(filepath)`: raw string
+-   `goto(time_string)`: time string in format `hh:mm:ss`
+-   `filetype(filetype)`: string, ("wav", "aiff", "bwf", "mp3")
+
+The following properties are available
+
+-   `A1 - A5`: boolean
+-   `B1 - A3`: boolean
+-   `samplerate`: int, (22050, 24000, 32000, 44100, 48000, 88200, 96000, 176400, 192000)
+-   `bitresolution`: int, (8, 16, 24, 32)
+-   `channel`: int, from 1 to 8
+-   `kbps`: int, (32, 40, 48, 56, 64, 80, 96, 112, 128, 160, 192, 224, 256, 320)
+-   `gain`: float, from -60.0 to 12.0
+
+example:
+
+```python
+vm.recorder.play()
+vm.recorder.stop()
+
+# Disable recorder out channel B2
+vm.recorder.B2 = False
+
+# filepath as raw string
+vm.recorder.load(r'C:\music\mytune.mp3')
+
+# set the goto time to 1m 30s
+vm.recorder.goto("00:01:30")
+```
+
+#### Recorder.Mode
+
+The following properties are available
+
+-   `recbus`: boolean
+-   `playonload`: boolean
+-   `loop`: boolean
+-   `multitrack`: boolean
+
+example:
+
+```python
+# Enable loop play
+vm.recorder.mode.loop = True
+```
+
+#### Recorder.ArmStrip[i]|ArmBus[i]
+
+The following method is available
+
+-   `set(val)`: boolean
+
+example:
+
+```python
+# Arm strip 3
+vm.recorder.armstrip[3].set(True)
+# Arm bus 0
+vm.recorder.armbus[0].set(True)
+```
+
+### VBAN
+
+-   `vm.vban.enable()` `vm.vban.disable()` Turn VBAN on or off
+
+##### Instream | Outstream
+
+The following properties are available.
+
+-   `on`: boolean
+-   `name`: string
+-   `ip`: string
+-   `port`: int, range from 1024 to 65535
+-   `sr`: int, (11025, 16000, 22050, 24000, 32000, 44100, 48000, 64000, 88200, 96000)
+-   `channel`: int, from 1 to 8
+-   `bit`: int, 16 or 24
+-   `quality`: int, from 0 to 4
+-   `route`: int, from 0 to 8
+
+`SR`, `channel` and `bit` are defined as:
+
+-   readonly for instreams.
+-   read and write for outstreams.
+
+example:
+
+```python
+# turn VBAN on
+vm.vban.enable()
+
+# turn on vban instream 0
+vm.vban.instream[0].on = True
+
+# set bit property for outstream 3 to 24
+vm.vban.outstream[3].bit = 24
+```
+
+### Command
+
+Certain 'special' commands are defined by the API as performing actions rather than setting values.
+
+The following methods are available:
+
+-   `show()` : Bring Voiceemeter GUI to the front
+-   `shutdown()` : Shuts down the GUI
+-   `restart()` : Restart the audio engine
+-   `reset()`: Applies the `reset` config. (phys strip B1, virt strip A1, gains, comp, gate 0.0, mute, mono, solo, eq false)
+
+The following properties are available.
+
+-   `showvbanchat`: boolean
+-   `lock`: boolean
+
+example:
+
+```python
+vm.command.restart()
+vm.command.showvbanchat = True
+```
+
+`showvbanchat` and `lock` are write only.
+
+### Device
+
+-   `ins` `outs` : Returns the number of input/output devices
+-   `input(i)` `output(i)` : Returns a dict of device properties for device[i]
+
+example:
+
+```python
+import voicemeeterlib
+with voicemeeterlib.api(KIND_ID) as vm:
+    for i in range(vm.device.ins):
+        print(vm.device.input(i))
+```
+
+### FX
+
+The following properties are available:
+
+-   `reverb`: boolean
+-   `reverb_ab`: boolean
+-   `delay`: boolean
+-   `delay_ab`: boolean
+
+example:
+
+```python
+vm.fx.reverb_ab = True
+```
+
+### Patch
+
+The following properties are available:
+
+-   `postfadercomposite`: boolean
+-   `postfxinsert`: boolean
+
+example:
+
+```python
+vm.patch.postfxinsert = False
+```
+
+##### asio[i]
+
+-   `get()`: int
+-   `set(patch_in)`: int, valid range determined by connected device.
+
+example:
+
+```python
+vm.patch.asio[3].set(4)
+```
+
+i, from 0 to 10
+
+##### A2[i] - A5[i]
+
+-   `get()`: int
+-   `set(patch_out)`: int, valid range determined by connected device.
+
+example:
+
+```python
+vm.patch.A3[5].set(3)
+```
+
+i, from 0 to 8.
+
+##### composite[i]
+
+-   `get()`: int
+-   `set(channel)`: int, from 0 up to number of channels depending on version.
+
+example:
+
+```python
+vm.patch.composite[7].set(4)
+```
+
+i, from 0 to 8.
+
+##### insert[i]
+
+-   `on`: boolean
+
+example:
+
+```python
+vm.patch.insert[18].on = True
+```
+
+i, from 0 up to number of channels depending on version.
+
+### Option
+
+The following properties are available:
+
+-   `sr`: int
+-   `asiosr`: boolean
+-   `monitoronsel`: boolean
+
+example:
+
+```python
+vm.option.sr = 48000
+```
+
+The following methods are available:
+
+-   `buffer(driver, buf)` : Set buffer size for particular audio driver.
+    -   buf: int, from 128 to 2048
+    -   driver:str, ("mme", "wdm", "ks", "asio")
+
+example:
+
+```python
+vm.option.buffer("wdm", 512)
+```
+
+##### delay[i]
+
+-   `get()`: int
+-   `set(delay)`: int, from 0 to 500
+
+example:
+
+```python
+vm.option.delay[4].set(30)
+```
+
+i, from 0 up to 4.
+
+### Midi
+
+The following properties are available:
+
+-   `channel`: int, returns the midi channel
+-   `current`: int, returns the current (or most recently pressed) key
+
+The following methods are available:
+
+-   `get(key)`: int, returns most recent velocity value for a key
+
+example:
+
+```python
+print(vm.midi.get(12))
+```
+
+get() may return None if no value for requested key in midi cache
+
+### Multiple parameters
+
+-   `apply`
+    Set many strip/bus/macrobutton/vban parameters at once, for example:
+
+```python
+vm.apply(
+    {
+        "strip-2": {"A1": True, "B1": True, "gain": -6.0},
+        "bus-2": {"mute": True, "eq": {"on": True}},
+        "button-0": {"state": True},
+        "vban-in-0": {"on": True},
+        "vban-out-1": {"name": "streamname"},
+    }
+)
+```
+
+Or for each class you may do:
+
+```python
+vm.strip[0].apply(mute: True, gain: 3.2, A1: True)
+vm.vban.outstream[0].apply(on: True, name: 'streamname', bit: 24)
+```
+
+## Config Files
+
+`vm.apply_config(configname)`
+
+You may load config files in TOML format.
+Three example configs have been included with the package. Remember to save
+current settings before loading a user config. To set one you may do:
+
+```python
+import voicemeeterlib
+with voicemeeterlib.api('banana') as vm:
+    vm.apply_config('example')
+```
+
+will load a user config file at configs/banana/example.toml for Voicemeeter Banana.
+
+## Events
+
+By default, NO events are listened for. Use events kwargs to enable specific event types.
+
+example:
+
+```python
+import voicemeeterlib
+# Set event updates to occur every 50ms
+# Listen for level updates only
+with voicemeeterlib.api('banana', ratelimit=0.05, ldirty=True}) as vm:
+    ...
+```
+
+#### `vm.observer`
+
+Use the Subject class to register an app as event observer.
+
+The following methods are available:
+
+-   `add`: registers an app as an event observer
+-   `remove`: deregisters an app as an event observer
+
+example:
+
+```python
+# register an app to receive updates
+class App():
+    def __init__(self, vm):
+        vm.observer.add(self)
+        ...
+```
+
+#### `vm.event`
+
+Use the event class to toggle updates as necessary.
+
+The following properties are available:
+
+-   `pdirty`: boolean
+-   `mdirty`: boolean
+-   `midi`: boolean
+-   `ldirty`: boolean
+
+example:
+
+```python
+vm.event.ldirty = True
+
+vm.event.pdirty = False
+```
+
+Or add, remove a list of events.
+
+The following methods are available:
+
+-   `add()`
+-   `remove()`
+-   `get()`
+
+example:
+
+```python
+vm.event.remove(["pdirty", "mdirty", "midi"])
+
+# get a list of currently subscribed
+print(vm.event.get())
+```
+
+## Remote class
+
+`voicemeeterlib.api(KIND_ID: str)`
+
+You may pass the following optional keyword arguments:
+
+-   `sync`: boolean=False, force the getters to wait for dirty parameters to clear. For most cases leave this as False.
+-   `ratelimit`: float=0.033, how often to check for updates in ms.
+-   `pdirty`: boolean=False, parameter updates
+-   `mdirty`: boolean=False, macrobutton updates
+-   `midi`: boolean=False, midi updates
+-   `ldirty`: boolean=False, level updates
+
+Access to lower level Getters and Setters are provided with these functions:
+
+-   `vm.get(param, is_string=False)`: For getting the value of any parameter. Set string to True if getting a property value expected to return a string.
+-   `vm.set(param, value)`: For setting the value of any parameter.
+
+example:
+
+```python
+vm.get('Strip[2].Mute')
+vm.set('Strip[4].Label', 'stripname')
+vm.set('Strip[0].Gain', -3.6)
+```
+
+Access to lower level polling functions are provided with the following property objects:
+
+#### `vm.pdirty`
+
+True iff a parameter has been updated.
+
+#### `vm.mdirty`
+
+True iff a macrobutton has been updated.
+
+#### `vm.ldirty`
+
+True iff a level has been updated.
+
+
+### Run tests
+
+To run all tests:
+
+```
+pytest -v
+```
+
+### Official Documentation
+
+-   [Voicemeeter Remote C API](https://github.com/onyx-and-iris/Voicemeeter-SDK/blob/update-docs/VoicemeeterRemoteAPI.pdf)
 
-setup(**setup_kwargs)
```

