# Comparing `tmp/gaitalytics-0.1.0b0.tar.gz` & `tmp/gaitalytics-0.1.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaitalytics-0.1.0b0.tar", last modified: Thu Jun 29 09:25:02 2023, max compression
+gzip compressed data, was "gaitalytics-0.1.1b0.tar", last modified: Sat Jul  1 09:07:16 2023, max compression
```

## Comparing `gaitalytics-0.1.0b0.tar` & `gaitalytics-0.1.1b0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 09:25:02.038627 gaitalytics-0.1.0b0/
--rw-rw-rw-   0        0        0     1096 2023-04-25 17:34:59.000000 gaitalytics-0.1.0b0/LICENSE
--rw-rw-rw-   0        0        0     5555 2023-06-29 09:25:02.038627 gaitalytics-0.1.0b0/PKG-INFO
--rw-rw-rw-   0        0        0     5031 2023-06-29 08:31:56.000000 gaitalytics-0.1.0b0/README.md
--rw-rw-rw-   0        0        0       84 2023-06-21 07:51:06.000000 gaitalytics-0.1.0b0/pyproject.toml
--rw-rw-rw-   0        0        0      728 2023-06-29 09:25:02.038627 gaitalytics-0.1.0b0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-29 09:25:02.003369 gaitalytics-0.1.0b0/src/
-drwxrwxrwx   0        0        0        0 2023-06-29 09:25:02.019876 gaitalytics-0.1.0b0/src/gaitalytics/
--rw-rw-rw-   0        0        0        0 2023-06-21 08:57:09.000000 gaitalytics-0.1.0b0/src/gaitalytics/__init__.py
--rw-rw-rw-   0        0        0    27232 2023-06-29 07:53:14.000000 gaitalytics-0.1.0b0/src/gaitalytics/analysis.py
--rw-rw-rw-   0        0        0    12671 2023-06-29 07:53:14.000000 gaitalytics-0.1.0b0/src/gaitalytics/api.py
--rw-rw-rw-   0        0        0     3226 2023-06-28 07:52:44.000000 gaitalytics-0.1.0b0/src/gaitalytics/c3d.py
--rw-rw-rw-   0        0        0    13086 2023-06-28 07:52:44.000000 gaitalytics-0.1.0b0/src/gaitalytics/cycle.py
--rw-rw-rw-   0        0        0     3340 2023-06-20 15:51:04.000000 gaitalytics-0.1.0b0/src/gaitalytics/emg.py
--rw-rw-rw-   0        0        0    15989 2023-06-28 13:09:43.000000 gaitalytics-0.1.0b0/src/gaitalytics/events.py
--rw-rw-rw-   0        0        0     8394 2023-06-29 09:07:44.000000 gaitalytics-0.1.0b0/src/gaitalytics/modelling.py
--rw-rw-rw-   0        0        0     6139 2023-06-28 07:52:44.000000 gaitalytics-0.1.0b0/src/gaitalytics/plot.py
--rw-rw-rw-   0        0        0    14514 2023-06-28 14:05:27.000000 gaitalytics-0.1.0b0/src/gaitalytics/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-29 09:25:02.034889 gaitalytics-0.1.0b0/src/gaitalytics.egg-info/
--rw-rw-rw-   0        0        0     5555 2023-06-29 09:25:01.000000 gaitalytics-0.1.0b0/src/gaitalytics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      490 2023-06-29 09:25:01.000000 gaitalytics-0.1.0b0/src/gaitalytics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 09:25:01.000000 gaitalytics-0.1.0b0/src/gaitalytics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-06-29 09:25:01.000000 gaitalytics-0.1.0b0/src/gaitalytics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-29 09:25:01.000000 gaitalytics-0.1.0b0/src/gaitalytics.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 09:07:16.913475 gaitalytics-0.1.1b0/
+-rw-rw-rw-   0        0        0     1096 2023-04-25 17:34:59.000000 gaitalytics-0.1.1b0/LICENSE
+-rw-rw-rw-   0        0        0     7028 2023-07-01 09:07:16.913475 gaitalytics-0.1.1b0/PKG-INFO
+-rw-rw-rw-   0        0        0     6504 2023-07-01 09:06:44.000000 gaitalytics-0.1.1b0/README.md
+-rw-rw-rw-   0        0        0       84 2023-06-21 07:51:06.000000 gaitalytics-0.1.1b0/pyproject.toml
+-rw-rw-rw-   0        0        0      728 2023-07-01 09:07:16.913475 gaitalytics-0.1.1b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-01 09:07:16.893073 gaitalytics-0.1.1b0/src/
+drwxrwxrwx   0        0        0        0 2023-07-01 09:07:16.903344 gaitalytics-0.1.1b0/src/gaitalytics/
+-rw-rw-rw-   0        0        0        0 2023-06-21 08:57:09.000000 gaitalytics-0.1.1b0/src/gaitalytics/__init__.py
+-rw-rw-rw-   0        0        0    27232 2023-07-01 08:08:36.000000 gaitalytics-0.1.1b0/src/gaitalytics/analysis.py
+-rw-rw-rw-   0        0        0    14931 2023-07-01 08:19:58.000000 gaitalytics-0.1.1b0/src/gaitalytics/api.py
+-rw-rw-rw-   0        0        0     3226 2023-06-28 07:52:44.000000 gaitalytics-0.1.1b0/src/gaitalytics/c3d.py
+-rw-rw-rw-   0        0        0    13160 2023-07-01 08:19:58.000000 gaitalytics-0.1.1b0/src/gaitalytics/cycle.py
+-rw-rw-rw-   0        0        0     3340 2023-06-20 15:51:04.000000 gaitalytics-0.1.1b0/src/gaitalytics/emg.py
+-rw-rw-rw-   0        0        0    15989 2023-06-28 13:09:43.000000 gaitalytics-0.1.1b0/src/gaitalytics/events.py
+-rw-rw-rw-   0        0        0     8727 2023-07-01 07:03:06.000000 gaitalytics-0.1.1b0/src/gaitalytics/modelling.py
+-rw-rw-rw-   0        0        0     6139 2023-07-01 08:19:58.000000 gaitalytics-0.1.1b0/src/gaitalytics/plot.py
+-rw-rw-rw-   0        0        0    14514 2023-07-01 08:19:58.000000 gaitalytics-0.1.1b0/src/gaitalytics/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-01 09:07:16.913475 gaitalytics-0.1.1b0/src/gaitalytics.egg-info/
+-rw-rw-rw-   0        0        0     7028 2023-07-01 09:07:16.000000 gaitalytics-0.1.1b0/src/gaitalytics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2023-07-01 09:07:16.000000 gaitalytics-0.1.1b0/src/gaitalytics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 09:07:16.000000 gaitalytics-0.1.1b0/src/gaitalytics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-01 09:07:16.000000 gaitalytics-0.1.1b0/src/gaitalytics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-01 09:07:16.000000 gaitalytics-0.1.1b0/src/gaitalytics.egg-info/top_level.txt
```

### Comparing `gaitalytics-0.1.0b0/LICENSE` & `gaitalytics-0.1.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.0b0/PKG-INFO` & `gaitalytics-0.1.1b0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,20 @@
-Metadata-Version: 2.1
-Name: gaitalytics
-Version: 0.1.0b0
-Summary: Library to analyse gait data captured with a mocap system
-Home-page: https://github.com/cereneo-foundation/gaitalytics
-Author: André Böni
-Author-email: andre.boeni@cereneo.foundation
-License: MIT
-Keywords: gait,analysis,c3d,mocap
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
 # Gaitalytics
-<img src="resources/logos/Gaitalytics_noBackground.png" alt="Gaitalytics logo" width="200"/>
+
+[<img src="https://github.com/cereneo-foundation/gaitalytics/blob/6d88443708bab2dbe300534bd52262d973397bcb/resources/logos/Gaitalytics_noBackground.png" alt="Gaitalytics logo" width="200"/>](https://github.com/cereneo-foundation/gaitalytics)
 
 This Python package provides a comprehensive set of tools and advanced algorithms for analyzing 3D motion capture data.
 It is specifically designed to process gait data stored in c3d format. Prior to utilizing the features of gaitalytics,
-it is necessary to perform data labeling, modeling, and filtering procedures. The library's versatility allows it to be
-adaptable to various marker sets and modeling algorithms, offering high configurability.
+it is necessary to perform data labeling, modeling, and filtering procedures.
+
+The library's versatility allows it to be adaptable to various marker sets and modeling algorithms,
+offering high configurability.
+
+> **Note**
+> Current pre-release is only tested with data acquired with Motek Caren, HBM2 Lower Body Trunk and PIG. 
 
 ## Functionalities
 
 ### Event Detection
 
 | Method     | Description      | options                                                                                                                                                                                                  |
 |:-----------|:-----------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
@@ -70,10 +60,52 @@
 ````shell
 pip install gaitalytics
 conda install -c conda-forge btk
 ````
 
 ## Usage
 
-Please take the resources in the example folder for advice.
+### Configuration
+
+Gaitalytics can be used with any marker set, which at least includes four hip markers (left front/back, right
+front/back)
+and four foot markers (left heel/toe, right heel/toe) and four ankle makers (left medial/lateral, right medial lateral).
+
+All functionalities in the libraries only take points into account which are configured in as specific yaml file. 
+Working example file can be found [here](https://github.com/cereneo-foundation/gaitalytics/blob/94bbc73072535d7f1e53ea935b6145194b137f09/settings/hbm_pig.yaml)
+
+
+
+Minimal requirements would look like this:
+````yaml
+marker_set_mapping:
+  left_back_hip: LASIS
+  right_back_hip: RASIS
+  left_front_hip: LPSIS
+  right_front_hip: RPSIS
+  
+  left_lat_malleoli: LLM
+  right_lat_malleoli: RLM
+  left_med_malleoli: LMM
+  right_med_malleoli: RMM
+
+  right_heel: RHEE
+  left_heel: LHEE
+  right_meta_2: RMT2
+  left_meta_2: LMT2
+  
+  com: COM
+  left_cmos: cmos_left
+  right_cmos: cmos_right
+  
+model_mapping:
+````
+> **Warning**
+> Do not rename keys of the minimal setting
+
+### Pipline
+
+Please take the resources in
+the [example folder](https://github.com/cereneo-foundation/gaitalytics/tree/94bbc73072535d7f1e53ea935b6145194b137f09/examples)
+for advice.
 
-###
+###
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gaitalytics-0.1.0b0/setup.cfg` & `gaitalytics-0.1.1b0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 6169 7461 6c79 7469 6373 0d0a   = gaitalytics..
-00000020: 7665 7273 696f 6e20 3d20 302e 312e 3062  version = 0.1.0b
+00000020: 7665 7273 696f 6e20 3d20 302e 312e 3162  version = 0.1.1b
 00000030: 6574 610d 0a61 7574 686f 7220 3d20 416e  eta..author = An
 00000040: 6472 c3a9 2042 c3b6 6e69 0d0a 6175 7468  dr.. B..ni..auth
 00000050: 6f72 5f65 6d61 696c 203d 2061 6e64 7265  or_email = andre
 00000060: 2e62 6f65 6e69 4063 6572 656e 656f 2e66  .boeni@cereneo.f
 00000070: 6f75 6e64 6174 696f 6e0d 0a75 726c 203d  oundation..url =
 00000080: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000090: 636f 6d2f 6365 7265 6e65 6f2d 666f 756e  com/cereneo-foun
```

### Comparing `gaitalytics-0.1.0b0/src/gaitalytics/analysis.py` & `gaitalytics-0.1.1b0/src/gaitalytics/analysis.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.0b0/src/gaitalytics/api.py` & `gaitalytics-0.1.1b0/src/gaitalytics/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from pandas import DataFrame
 
 import gaitalytics.analysis
 import gaitalytics.c3d
 import gaitalytics.cycle
 import gaitalytics.events
+import gaitalytics.modelling
 import gaitalytics.utils
 
 # constants
 CYCLE_METHOD_HEEL_STRIKE = "HS"
 CYCLE_METHOD_TOE_OFF = "TO"
 
 NORMALISE_METHODE_LINEAR = "linear"
@@ -39,14 +40,19 @@
                  ANALYSIS_POWERS,
                  ANALYSIS_FORCES,
                  ANALYSIS_SPATIO_TEMP,
                  ANALYSIS_TOE_CLEARANCE,
                  ANALYSIS_CMOS,
                  ANALYSIS_MOS)
 
+MODELLING_COM = "com"
+MODELLING_CMOS = "cmos"
+MODELLING_LIST = [MODELLING_COM,
+                  MODELLING_CMOS]
+
 
 def analyse_data(cycle_data: Dict[str, gaitalytics.utils.BasicCyclePoint],
                  config: gaitalytics.utils.ConfigProvider,
                  methode: List[str] = ANALYSIS_LIST, **kwargs) -> DataFrame:
     """
     runs specified analysis and concatenates into one frame
     :param cycle_data: unnormalised cycle data
@@ -283,13 +289,54 @@
     if buffer_output_path:
         prefix = os.path.basename(c3d_file_path).replace(".4.c3d", "")
         _cycle_points_to_csv(normalised_data, buffer_output_path, prefix)
 
     return normalised_data
 
 
+def model_data(c3d_file_path: str,
+               output_path: str,
+               configs: gaitalytics.utils.ConfigProvider,
+               methode: str,
+               **kwargs):
+    """
+    Models data according to chosen method and saves new c3d file in output path with '.5.c3d extension'
+
+    :param c3d_file_path: path of c3d file with modelled filtered data '.3.c3d'
+    :param output_path: path to dir to store c3d file with events
+    :param configs: configs from marker and model mapping
+    :param methode: methode to detect events 'Marker' api.GAIT_EVENT_METHODE_MARKER or
+        'Forceplate' api.GAIT_EVENT_METHODE_FP
+    :keyword belt_speed: belt speed
+    """
+    if not methode in MODELLING_LIST:
+        raise KeyError(f"{methode} is not a valid modelling methode")
+    methods: List[gaitalytics.modelling.BaseOutputModeller] = []
+    acq = gaitalytics.c3d.read_btk(c3d_file_path)
+    subject = gaitalytics.utils.extract_subject(acq)
+    if methode == MODELLING_CMOS:
+        methods.append(gaitalytics.modelling.COMModeller(configs))
+        methods.append(gaitalytics.modelling.CMoSModeller(gaitalytics.utils.GaitEventContext.LEFT,
+                                                          configs,
+                                                          subject.left_leg_length,
+                                                          **kwargs))
+        methods.append(gaitalytics.modelling.CMoSModeller(gaitalytics.utils.GaitEventContext.RIGHT,
+                                                          configs,
+                                                          subject.right_leg_length,
+                                                          **kwargs))
+    elif methode == MODELLING_COM:
+        methods.append(gaitalytics.modelling.COMModeller(configs))
+
+    for methode in methods:
+        methode.create_point(acq, **kwargs)
+    filename = os.path.basename(c3d_file_path)
+    filename = filename.replace(".4.c3d", ".5.c3d")
+    output_path = os.path.join(output_path, filename)
+    gaitalytics.c3d.write_btk(acq, output_path)
+
+
 def _cycle_points_to_csv(cycle_data: Dict[str, gaitalytics.utils.BasicCyclePoint], dir_path: str, prefix: str):
     subject_saved = False
     for key in cycle_data:
         cycle_data[key].to_csv(dir_path, prefix)
         if not subject_saved:
             cycle_data[key].subject.to_file(dir_path)
```

### Comparing `gaitalytics-0.1.0b0/src/gaitalytics/c3d.py` & `gaitalytics-0.1.1b0/src/gaitalytics/c3d.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.0b0/src/gaitalytics/cycle.py` & `gaitalytics-0.1.1b0/src/gaitalytics/cycle.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,16 @@
 
 
 # Normalisation
 class TimeNormalisationAlgorithm(ABC):
 
     def __init__(self, number_frames: int = 100):
         self._number_frames = number_frames
-        self._data_type_fiter = {gaitalytics.utils.PointDataType.Angles,
+        self._data_type_fiter = {gaitalytics.utils.PointDataType.Marker,
+                                 gaitalytics.utils.PointDataType.Angles,
                                  gaitalytics.utils.PointDataType.Forces,
                                  gaitalytics.utils.PointDataType.Moments,
                                  gaitalytics.utils.PointDataType.Power,
                                  gaitalytics.utils.PointDataType.Scalar,
                                  gaitalytics.utils.PointDataType.Reaction}
 
     def normalise(self,
```

### Comparing `gaitalytics-0.1.0b0/src/gaitalytics/emg.py` & `gaitalytics-0.1.1b0/src/gaitalytics/emg.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.0b0/src/gaitalytics/events.py` & `gaitalytics-0.1.1b0/src/gaitalytics/events.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.0b0/src/gaitalytics/modelling.py` & `gaitalytics-0.1.1b0/src/gaitalytics/modelling.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,179 +9,187 @@
 
 class BaseOutputModeller(ABC):
 
     def __init__(self, label: str, point_type: gaitalytics.utils.PointDataType):
         self._label = label
         self._type = point_type
 
-    def create_point(self, acq: btkAcquisition):
-        result = self._calculate_point(acq)
+    def create_point(self, acq: btkAcquisition, **kwargs):
+        result = self._calculate_point(acq , **kwargs)
         point = btkPoint(self._type.value)
         point.SetValues(result)
         point.SetLabel(self._label)
         acq.AppendPoint(point)
 
     @abstractmethod
-    def _calculate_point(self, acq: btkAcquisition) -> np.ndarray:
+    def _calculate_point(self, acq: btkAcquisition, **kwargs) -> np.ndarray:
         pass
 
 
 class COMModeller(BaseOutputModeller):
 
     def __init__(self, configs: gaitalytics.utils.ConfigProvider):
         super().__init__(configs.MARKER_MAPPING.com.value, gaitalytics.utils.PointDataType.Scalar)
         self._configs = configs
 
-    def _calculate_point(self, acq: btkAcquisition):
+    def _calculate_point(self, acq: btkAcquisition, **kwargs):
         l_hip_b = acq.GetPoint(self._configs.MARKER_MAPPING.left_back_hip.value).GetValues()
         r_hip_b = acq.GetPoint(self._configs.MARKER_MAPPING.right_back_hip.value).GetValues()
         l_hip_f = acq.GetPoint(self._configs.MARKER_MAPPING.left_front_hip.value).GetValues()
         r_hip_f = acq.GetPoint(self._configs.MARKER_MAPPING.right_front_hip.value).GetValues()
         return (l_hip_b + r_hip_b + l_hip_f + r_hip_f) / 4
 
 
 class CMoSModeller(BaseOutputModeller):
 
-    def __init__(self, side: str, configs: gaitalytics.utils.ConfigProvider,
-                 dominant_leg_length: float, belt_speed: float):
+    def __init__(self, side: gaitalytics.utils.GaitEventContext, configs: gaitalytics.utils.ConfigProvider,
+                 dominant_leg_length: float, **kwargs):
+        belt_speed = kwargs.get("belt_speed", 0)
         self._configs = configs
         self._dominant_leg_length = dominant_leg_length
         self._belt_speed = belt_speed
         self._side = side
-        if side == "Left":
+        if side == gaitalytics.utils.GaitEventContext.LEFT:
             label = self._configs.MARKER_MAPPING.left_cmos.value
         else:
             label = self._configs.MARKER_MAPPING.right_cmos.value
         super().__init__(label, gaitalytics.utils.PointDataType.Marker)
 
-    def _calculate_point(self, acq: btkAcquisition) -> np.ndarray:
+    def _calculate_point(self, acq: btkAcquisition, **kwargs) -> np.ndarray:
         com = acq.GetPoint(self._configs.MARKER_MAPPING.com.value).GetValues()
-        if self._side == "Left":
+        if self._side == gaitalytics.utils.GaitEventContext.LEFT:
             lat_malleoli = acq.GetPoint(self._configs.MARKER_MAPPING.left_lat_malleoli.value).GetValues()
             contra_lat_malleoli = acq.GetPoint(self._configs.MARKER_MAPPING.right_lat_malleoli.value).GetValues()
             meta_2 = acq.GetPoint(self._configs.MARKER_MAPPING.left_meta_2.value).GetValues()
             contra_meta_2 = acq.GetPoint(self._configs.MARKER_MAPPING.right_meta_2.value).GetValues()
         else:
             lat_malleoli = acq.GetPoint(self._configs.MARKER_MAPPING.right_lat_malleoli.value).GetValues()
             contra_lat_malleoli = acq.GetPoint(self._configs.MARKER_MAPPING.left_lat_malleoli.value).GetValues()
             meta_2 = acq.GetPoint(self._configs.MARKER_MAPPING.right_meta_2.value).GetValues()
             contra_meta_2 = acq.GetPoint(self._configs.MARKER_MAPPING.left_meta_2.value).GetValues()
         return self.cMoS(com, lat_malleoli, contra_lat_malleoli, meta_2, contra_meta_2, self._dominant_leg_length,
-                         self._belt_speed, acq, self._side)
+                         self._belt_speed, acq, self._side, **kwargs)
 
     def cMoS(self, com: np.ndarray,
              lat_malleoli_marker: np.ndarray,
              lat_malleoli_marker_contra: np.ndarray,
              second_meta_head_marker: np.ndarray,
              second_meta_head_marker_contra: np.ndarray,
              dominant_leg_length: float,
              belt_speed: float,
              acq: btkAcquisition,
-             side: str,
-             show: bool = True) -> np.ndarray:
+             side: gaitalytics.utils.GaitEventContext,
+             **kwargs) -> np.ndarray:
+
+        show_plot = kwargs.get("show_plot", False)
         # AP axis is inverted
         com[:, 1] *= -1
         second_meta_head_marker[:, 1] *= -1
         second_meta_head_marker_contra[:, 1] *= -1
 
-        if side == "Left":
-            contra_side = "Right"
+        if side == gaitalytics.utils.GaitEventContext.LEFT:
+            contra_side = gaitalytics.utils.GaitEventContext.RIGHT
         else:
-            contra_side = "Left"
+            contra_side = gaitalytics.utils.GaitEventContext.LEFT
         distance_from_x_com_to_bos = np.zeros((len(com), 3))
 
         # preparing events for the MOS calculation
         events_labels = []
         events_frames = []
         events_foot = []
         for k in range(acq.GetEventNumber()):
             event = acq.GetEvent(k)
             events_labels.append(event.GetLabel())
             events_frames.append(event.GetFrame())
             events_foot.append(event.GetContext())
 
-        minute_flag = False
-        mos = []
         itr = 0
         cycle_event = None
-        com_v = np.diff(com, axis=0)
-        sqrt_leg_speed = np.sqrt(9.81 / dominant_leg_length)
+        com_v = calculate_point_velocity(com)
+        x_com = calculate_xcom(belt_speed, com, com_v, dominant_leg_length)
         # data route
         for i in range(0, len(com)):
             if itr < acq.GetEventNumber():
                 if events_frames[itr] == i:
                     type_of_event = events_labels[itr]
                     foot = events_foot[itr]
                     cycle_event = f"{foot} {type_of_event}"
                     # determining the event to know the base of support we have to use for the calculation
                     itr += 1
             else:
                 break
 
-            # calculating the x_com
-            x_com = [com[i, 0] + (com_v[i, 0]/sqrt_leg_speed), com[i, 1] + (belt_speed+com_v[i, 1]) / sqrt_leg_speed]
-            # still miss the treadmill speed (need velocity of belt in AP and ML axis too)
-            # x_com = [COM[i, 0], COM[i, 1]]
-            # calculating the distance between the x_com and the BOS
             # 4 cases : Left Heel Strike, Left Toe Off, Right Heel Strike, Right Toe Off
             """
                         MOSant
                             ^
                             |
                 MOSlat <-- COM --> MOSmed       (for left foot ahead, invert lat and med otherwise)
                             |
                         MOSpost
 
             """
             ## AP
-            if cycle_event == f"{contra_side} Foot Off":
-                mos = [x_com[0] - lat_malleoli_marker[i, 0],
-                       second_meta_head_marker[i, 1] - x_com[1]]
-            elif cycle_event == f"{side} Foot Off":
-                mos = [lat_malleoli_marker_contra[i, 0] - x_com[0],
-                       second_meta_head_marker_contra[i, 1] - x_com[1]]
-            elif cycle_event == f"{side} Foot Strike":
-                mos = [x_com[0] - lat_malleoli_marker[i, 0],
-                       second_meta_head_marker[i, 1] - x_com[1]]
-            elif cycle_event == f"{contra_side} Foot Strike":
-                mos = [lat_malleoli_marker_contra[i, 0] - x_com[0],
-                       second_meta_head_marker_contra[i, 1] - x_com[1]]
+            if cycle_event == f"{contra_side.value} Foot Off":
+                mos = [x_com[i, 0] - lat_malleoli_marker[i, 0],
+                       second_meta_head_marker[i, 1] - x_com[i, 1]]
+            elif cycle_event == f"{side.value} Foot Off":
+                mos = [lat_malleoli_marker_contra[i, 0] - x_com[i, 0],
+                       second_meta_head_marker_contra[i, 1] - x_com[i, 1]]
+            elif cycle_event == f"{side.value} Foot Strike":
+                mos = [x_com[i, 0] - lat_malleoli_marker[i, 0],
+                       second_meta_head_marker[i, 1] - x_com[i, 1]]
+            elif cycle_event == f"{contra_side.value} Foot Strike":
+                mos = [lat_malleoli_marker_contra[i, 0] - x_com[i, 0],
+                       second_meta_head_marker_contra[i, 1] - x_com[i, 1]]
             else:
                 mos = [0, 0]
 
-            if side == "Left":
+            if side == gaitalytics.utils.GaitEventContext.LEFT:
                 mos[0] = mos[0] * -1
+
             distance_from_x_com_to_bos[i, 0] = mos[0]
             distance_from_x_com_to_bos[i, 1] = mos[1]
-        if show:
-            self._show(distance_from_x_com_to_bos, side)
+        if show_plot:
+            self._show(distance_from_x_com_to_bos, side.value)
         return distance_from_x_com_to_bos
 
     def _show(self, distance_from_xCOM_to_BOS, side):
         # if show==True:
         # fig, ax1 = plt.subplots()
         freq = 100
         index_minute = 60 * freq
         time = np.arange(0, len(distance_from_xCOM_to_BOS) / freq, 1 / freq)
         fig, axs = plt.subplots(1, 2, figsize=(8, 6))
         fig.suptitle(side)
         (ax1, ax2) = axs  # Unpack the subplots axes
-        # ax1.plot(distance_from_xCOM_to_BOS[:, 0])
-        # ax1.plot(time, Lat_Malleoli_Marker_Right[:, 0])
-        # ax1.plot(time, Lat_Malleoli_Marker_Left[:, 0])
-        # ax1.plot(time, COM[:, 0])
+
         ax1.plot(time[0:index_minute], distance_from_xCOM_to_BOS[0:index_minute, 0], color='orange', label='MOSlat')
         ax1.plot(time[index_minute:], distance_from_xCOM_to_BOS[index_minute:, 0], color='green', label='MOSlat>1min')
 
         ax2.plot(time[0:index_minute], distance_from_xCOM_to_BOS[0:index_minute, 1], color='orange', label='MOSap')
         ax2.plot(time[index_minute:], distance_from_xCOM_to_BOS[index_minute:, 1], color='green', label='MOSap>1min')
 
-        # ax2.plot(distance_from_xCOM_to_BOS[:, 1])
-        # ax2.plot(time, Second_Meta_Head_Marker_Right[:, 1])
-        # ax2.plot(time, Second_Meta_Head_Marker_Left[:, 1])
-        # ax2.plot(time, COM[:, 1])
-
         ax1.legend()
         ax2.legend()
         # Adjust the spacing between subplots
         plt.tight_layout()
         plt.show()
+
+
+def calculate_point_velocity(com: np.ndarray):
+    com_v = np.diff(com, axis=0)
+    com_v = np.insert(com_v, 0, 0, axis=0)
+    for c in range(len(com_v[0])):
+        com_v[0, c] = com_v[1, c]
+    return com_v
+
+
+def calculate_xcom(belt_speed: float, com: np.ndarray, com_v: np.ndarray, dominant_leg_length: float):
+    sqrt_leg_speed = np.sqrt(9.81 / dominant_leg_length)
+    com_x_v = com[:, 0] + (com_v[:, 0] / sqrt_leg_speed)
+    com_y_v = com[:, 1] + (belt_speed + com_v[:, 1]) / sqrt_leg_speed
+    com_z_v = com[:, 2] + (com_v[:, 2] / sqrt_leg_speed)
+    x_com = np.array([com_x_v, com_y_v, com_z_v]).T
+    # calculating the x_com
+
+    return x_com
```

### Comparing `gaitalytics-0.1.0b0/src/gaitalytics/plot.py` & `gaitalytics-0.1.1b0/src/gaitalytics/plot.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.1.0b0/src/gaitalytics/utils.py` & `gaitalytics-0.1.1b0/src/gaitalytics/utils.py`

 * *Files identical despite different names*

