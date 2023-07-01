# Comparing `tmp/bark_monitor-0.0.2.tar.gz` & `tmp/bark_monitor-0.0.3.tar.gz`

## Comparing `bark_monitor-0.0.2.tar` & `bark_monitor-0.0.3.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/.flake8
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/.github/workflows/snap.yaml
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/.vscode/launch.json
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/.vscode/settings.json
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/bark_monitor/__init__.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/bark_monitor/chats.py
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/bark_monitor/config.py
--rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/bark_monitor/google_sync.py
--rw-r--r--   0        0        0    15214 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/bark_monitor/very_bark_bot.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/bark_monitor/cli/get_param.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/bark_monitor/cli/record.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/bark_monitor/cli/yamnet_lite_record.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/bark_monitor/cli/yamnet_record.py
--rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/bark_monitor/recorders/base_recorder.py
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/bark_monitor/recorders/recorder.py
--rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/bark_monitor/recorders/recording.py
--rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/bark_monitor/recorders/wave_recorder.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/bark_monitor/recorders/yamnet_lite_recorder.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/bark_monitor/recorders/yamnet_recorder.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/config_test/chats.json
--rw-r--r--   0        0        0    39622 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/images/dashboard.png
--rw-r--r--   0        0        0   175097 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/images/watson.jpg
--rw-r--r--   0        0        0    72959 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/images/watson_icon.jpg
--rw-r--r--   0        0        0  4126810 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/models/lite-model_yamnet_classification_tflite_1.tflite
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/recording_test/recording.json
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/recording_test/19-06-2023/recording.json
--rw-r--r--   0        0        0   131116 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/recording_test/audio/01-07-2023/01-07-2023_13-46-50.wav
--rw-r--r--   0        0        0    65580 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/recording_test/audio/01-07-2023/01-07-2023_13-48-33.wav
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/scripts/audio_device_info.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/snap/snapcraft.yaml
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/tests/test_recording.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/tests/data/recording.json
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/.gitignore
--rw-r--r--   0        0        0    34235 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/LICENSE.md
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/README.md
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    42616 2020-02-02 00:00:00.000000 bark_monitor-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/.flake8
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/pypi_token
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/.github/workflows/snap.yaml
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/.vscode/launch.json
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/.vscode/settings.json
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/bark_monitor/__init__.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/bark_monitor/chats.py
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/bark_monitor/config.py
+-rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/bark_monitor/google_sync.py
+-rw-r--r--   0        0        0    15214 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/bark_monitor/very_bark_bot.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/bark_monitor/cli/get_param.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/bark_monitor/cli/record.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/bark_monitor/cli/yamnet_lite_record.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/bark_monitor/cli/yamnet_record.py
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/bark_monitor/recorders/base_recorder.py
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/bark_monitor/recorders/recorder.py
+-rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/bark_monitor/recorders/recording.py
+-rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/bark_monitor/recorders/wave_recorder.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/bark_monitor/recorders/yamnet_lite_recorder.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/bark_monitor/recorders/yamnet_recorder.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/config_test/chats.json
+-rw-r--r--   0        0        0    39622 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/images/dashboard.png
+-rw-r--r--   0        0        0   175097 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/images/watson.jpg
+-rw-r--r--   0        0        0    72959 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/images/watson_icon.jpg
+-rw-r--r--   0        0        0  4126810 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/models/lite-model_yamnet_classification_tflite_1.tflite
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/recording_test/recording.json
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/recording_test/19-06-2023/recording.json
+-rw-r--r--   0        0        0   131116 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/recording_test/audio/01-07-2023/01-07-2023_13-46-50.wav
+-rw-r--r--   0        0        0    65580 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/recording_test/audio/01-07-2023/01-07-2023_13-48-33.wav
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/scripts/audio_device_info.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/snap/snapcraft.yaml
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/tests/test_recording.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/tests/data/recording.json
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/.gitignore
+-rw-r--r--   0        0        0    34235 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/LICENSE.md
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/README.md
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    42718 2020-02-02 00:00:00.000000 bark_monitor-0.0.3/PKG-INFO
```

### Comparing `bark_monitor-0.0.2/.github/workflows/snap.yaml` & `bark_monitor-0.0.3/.github/workflows/snap.yaml`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/.vscode/launch.json` & `bark_monitor-0.0.3/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/bark_monitor/chats.py` & `bark_monitor-0.0.3/bark_monitor/chats.py`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/bark_monitor/config.py` & `bark_monitor-0.0.3/bark_monitor/config.py`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/bark_monitor/google_sync.py` & `bark_monitor-0.0.3/bark_monitor/google_sync.py`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/bark_monitor/very_bark_bot.py` & `bark_monitor-0.0.3/bark_monitor/very_bark_bot.py`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/bark_monitor/cli/get_param.py` & `bark_monitor-0.0.3/bark_monitor/cli/get_param.py`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/bark_monitor/cli/record.py` & `bark_monitor-0.0.3/bark_monitor/cli/record.py`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/bark_monitor/cli/yamnet_lite_record.py` & `bark_monitor-0.0.3/bark_monitor/cli/yamnet_lite_record.py`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/bark_monitor/cli/yamnet_record.py` & `bark_monitor-0.0.3/bark_monitor/cli/yamnet_record.py`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/bark_monitor/recorders/base_recorder.py` & `bark_monitor-0.0.3/bark_monitor/recorders/base_recorder.py`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/bark_monitor/recorders/recorder.py` & `bark_monitor-0.0.3/bark_monitor/recorders/recorder.py`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/bark_monitor/recorders/recording.py` & `bark_monitor-0.0.3/bark_monitor/recorders/recording.py`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/bark_monitor/recorders/wave_recorder.py` & `bark_monitor-0.0.3/bark_monitor/recorders/wave_recorder.py`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/bark_monitor/recorders/yamnet_lite_recorder.py` & `bark_monitor-0.0.3/bark_monitor/recorders/yamnet_lite_recorder.py`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/bark_monitor/recorders/yamnet_recorder.py` & `bark_monitor-0.0.3/bark_monitor/recorders/yamnet_recorder.py`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/images/dashboard.png` & `bark_monitor-0.0.3/images/dashboard.png`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/images/watson.jpg` & `bark_monitor-0.0.3/images/watson.jpg`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/images/watson_icon.jpg` & `bark_monitor-0.0.3/images/watson_icon.jpg`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/models/lite-model_yamnet_classification_tflite_1.tflite` & `bark_monitor-0.0.3/models/lite-model_yamnet_classification_tflite_1.tflite`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/recording_test/recording.json` & `bark_monitor-0.0.3/recording_test/recording.json`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/recording_test/audio/01-07-2023/01-07-2023_13-46-50.wav` & `bark_monitor-0.0.3/recording_test/audio/01-07-2023/01-07-2023_13-46-50.wav`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/recording_test/audio/01-07-2023/01-07-2023_13-48-33.wav` & `bark_monitor-0.0.3/recording_test/audio/01-07-2023/01-07-2023_13-48-33.wav`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/scripts/audio_device_info.py` & `bark_monitor-0.0.3/scripts/audio_device_info.py`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/snap/snapcraft.yaml` & `bark_monitor-0.0.3/snap/snapcraft.yaml`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/tests/test_recording.py` & `bark_monitor-0.0.3/tests/test_recording.py`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/tests/data/recording.json` & `bark_monitor-0.0.3/tests/data/recording.json`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/.gitignore` & `bark_monitor-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/LICENSE.md` & `bark_monitor-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bark_monitor-0.0.2/README.md` & `bark_monitor-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Bark monitor
 
 <!-- [![Get it from the Snap Store](https://snapcraft.io/static/images/badges/en/snap-store-black.svg)](https://snapcraft.io/bark-monitor) -->
 
-Get it from pipy: `pip install bark-monitor`.
-
-![](images/watson.jpg)
+![my dog](https://codeberg.org/MalcolmMielle/bark_monitor/raw/commit/990ab48c7e4f3110a8f10b4d4eed4c209d43b81b/images/watson.jpg)
 
 Showing my neighbor my dog doesn't bark!
 
+Get it today: `pip install bark-monitor`.
+
 ## Introduction
 
 Do you also have neighbor who accuses your dog of barking all the time, want to kick you out of your flat because of it, even though you know _it's not true_?
 Do you want to know if your dog is actually noisy when you are gone but you don't (and don't want to buy) a baby cam?
 
 Then this project is for you!
```

### Comparing `bark_monitor-0.0.2/pyproject.toml` & `bark_monitor-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bark_monitor"
-version = "0.0.2"
+version = "0.0.3"
 description = "A package to monitor your dog's barks"
 authors = [
   { name = "Malcolm Mielle", email = "malcolm.mielle@gmail.com" },
 ]
 readme = "README.md"
 dependencies = [
   "Wave>=0.0.2",
```

### Comparing `bark_monitor-0.0.2/PKG-INFO` & `bark_monitor-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bark_monitor
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package to monitor your dog's barks
 Project-URL: repository, https://codeberg.org/MalcolmMielle/bark_monitor
 Project-URL: documentation, https://malcolmmielle.codeberg.page/bark_monitor/@pages/
 Author-email: Malcolm Mielle <malcolm.mielle@gmail.com>
 License: ### GNU AFFERO GENERAL PUBLIC LICENSE
         
         Version 3, 19 November 2007
@@ -690,20 +690,20 @@
 Requires-Dist: mkdocs>=1.4.3; extra == 'docs'
 Description-Content-Type: text/markdown
 
 # Bark monitor
 
 <!-- [![Get it from the Snap Store](https://snapcraft.io/static/images/badges/en/snap-store-black.svg)](https://snapcraft.io/bark-monitor) -->
 
-Get it from pipy: `pip install bark-monitor`.
-
-![](images/watson.jpg)
+![my dog](https://codeberg.org/MalcolmMielle/bark_monitor/raw/commit/990ab48c7e4f3110a8f10b4d4eed4c209d43b81b/images/watson.jpg)
 
 Showing my neighbor my dog doesn't bark!
 
+Get it today: `pip install bark-monitor`.
+
 ## Introduction
 
 Do you also have neighbor who accuses your dog of barking all the time, want to kick you out of your flat because of it, even though you know _it's not true_?
 Do you want to know if your dog is actually noisy when you are gone but you don't (and don't want to buy) a baby cam?
 
 Then this project is for you!
```

