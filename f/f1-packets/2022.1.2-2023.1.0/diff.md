# Comparing `tmp/f1-packets-2022.1.2.tar.gz` & `tmp/f1_packets-2023.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f1-packets-2022.1.2.tar", max compression
+gzip compressed data, was "f1_packets-2023.1.0.tar", max compression
```

## Comparing `f1-packets-2022.1.2.tar` & `f1_packets-2023.1.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1077 2022-07-11 14:26:31.847470 f1-packets-2022.1.2/LICENSE
--rw-r--r--   0        0        0      540 2022-07-11 14:26:31.847470 f1-packets-2022.1.2/README.md
--rw-r--r--   0        0        0        0 2022-07-11 14:26:31.847470 f1-packets-2022.1.2/f1/__init__.py
--rw-r--r--   0        0        0      545 2022-07-11 14:26:31.847470 f1-packets-2022.1.2/f1/handler.py
--rw-r--r--   0        0        0      680 2022-07-11 14:26:31.847470 f1-packets-2022.1.2/f1/listener.py
--rw-r--r--   0        0        0    19710 2022-07-11 14:26:31.847470 f1-packets-2022.1.2/f1/packets.py
--rw-r--r--   0        0        0      840 2022-07-11 14:26:41.107787 f1-packets-2022.1.2/pyproject.toml
--rw-r--r--   0        0        0     1156 2022-07-11 14:26:41.576232 f1-packets-2022.1.2/setup.py
--rw-r--r--   0        0        0     1291 2022-07-11 14:26:41.576531 f1-packets-2022.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-01 17:36:25.470852 f1_packets-2023.1.0/LICENSE
+-rw-r--r--   0        0        0      540 2023-07-01 17:36:25.470852 f1_packets-2023.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-01 17:36:25.470852 f1_packets-2023.1.0/f1/__init__.py
+-rw-r--r--   0        0        0      545 2023-07-01 17:36:25.470852 f1_packets-2023.1.0/f1/handler.py
+-rw-r--r--   0        0        0      680 2023-07-01 17:36:25.470852 f1_packets-2023.1.0/f1/listener.py
+-rw-r--r--   0        0        0    22150 2023-07-01 17:36:25.470852 f1_packets-2023.1.0/f1/packets.py
+-rw-r--r--   0        0        0      840 2023-07-01 17:36:38.291159 f1_packets-2023.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1342 1970-01-01 00:00:00.000000 f1_packets-2023.1.0/PKG-INFO
```

### Comparing `f1-packets-2022.1.2/LICENSE` & `f1_packets-2023.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `f1-packets-2022.1.2/README.md` & `f1_packets-2023.1.0/README.md`

 * *Files identical despite different names*

### Comparing `f1-packets-2022.1.2/f1/handler.py` & `f1_packets-2023.1.0/f1/handler.py`

 * *Files identical despite different names*

### Comparing `f1-packets-2022.1.2/f1/listener.py` & `f1_packets-2023.1.0/f1/listener.py`

 * *Files identical despite different names*

### Comparing `f1-packets-2022.1.2/f1/packets.py` & `f1_packets-2023.1.0/f1/packets.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,21 +85,23 @@
 
 # [[[cog
 # import sys; sys.path.append("./scripts"); import genspec
 # ]]]
 class PacketHeader(Packet):
     _fields_ = [
         ("packet_format", ctypes.c_uint16),
+        ("game_year", ctypes.c_uint8),
         ("game_major_version", ctypes.c_uint8),
         ("game_minor_version", ctypes.c_uint8),
         ("packet_version", ctypes.c_uint8),
         ("packet_id", ctypes.c_uint8),
         ("session_uid", ctypes.c_uint64),
         ("session_time", ctypes.c_float),
         ("frame_identifier", ctypes.c_uint32),
+        ("overall_frame_identifier", ctypes.c_uint32),
         ("player_car_index", ctypes.c_uint8),
         ("secondary_player_car_index", ctypes.c_uint8),
     ]
 
 
 class CarMotionData(Packet):
     _fields_ = [
@@ -124,29 +126,14 @@
     ]
 
 
 class PacketMotionData(Packet):
     _fields_ = [
         ("header", PacketHeader),
         ("car_motion_data", CarMotionData * 22),
-        ("suspension_position", ctypes.c_float * 4),
-        ("suspension_velocity", ctypes.c_float * 4),
-        ("suspension_acceleration", ctypes.c_float * 4),
-        ("wheel_speed", ctypes.c_float * 4),
-        ("wheel_slip", ctypes.c_float * 4),
-        ("local_velocity_x", ctypes.c_float),
-        ("local_velocity_y", ctypes.c_float),
-        ("local_velocity_z", ctypes.c_float),
-        ("angular_velocity_x", ctypes.c_float),
-        ("angular_velocity_y", ctypes.c_float),
-        ("angular_velocity_z", ctypes.c_float),
-        ("angular_acceleration_x", ctypes.c_float),
-        ("angular_acceleration_y", ctypes.c_float),
-        ("angular_acceleration_z", ctypes.c_float),
-        ("front_wheels_angle", ctypes.c_float),
     ]
 
 
 class MarshalZone(Packet):
     _fields_ = [
         ("zone_start", ctypes.c_float),
         ("zone_flag", ctypes.c_int8),
@@ -207,34 +194,46 @@
         ("drs_assist", ctypes.c_uint8),
         ("dynamic_racing_line", ctypes.c_uint8),
         ("dynamic_racing_line_type", ctypes.c_uint8),
         ("game_mode", ctypes.c_uint8),
         ("rule_set", ctypes.c_uint8),
         ("time_of_day", ctypes.c_uint32),
         ("session_length", ctypes.c_uint8),
+        ("speed_units_lead_player", ctypes.c_uint8),
+        ("temperature_units_lead_player", ctypes.c_uint8),
+        ("speed_units_secondary_player", ctypes.c_uint8),
+        ("temperature_units_secondary_player", ctypes.c_uint8),
+        ("num_safety_car_periods", ctypes.c_uint8),
+        ("num_virtual_safety_car_periods", ctypes.c_uint8),
+        ("num_red_flag_periods", ctypes.c_uint8),
     ]
 
 
 class LapData(Packet):
     _fields_ = [
         ("last_lap_time_in_ms", ctypes.c_uint32),
         ("current_lap_time_in_ms", ctypes.c_uint32),
         ("sector1_time_in_ms", ctypes.c_uint16),
+        ("sector1_time_minutes", ctypes.c_uint8),
         ("sector2_time_in_ms", ctypes.c_uint16),
+        ("sector2_time_minutes", ctypes.c_uint8),
+        ("delta_to_car_in_front_in_ms", ctypes.c_uint16),
+        ("delta_to_race_leader_in_ms", ctypes.c_uint16),
         ("lap_distance", ctypes.c_float),
         ("total_distance", ctypes.c_float),
         ("safety_car_delta", ctypes.c_float),
         ("car_position", ctypes.c_uint8),
         ("current_lap_num", ctypes.c_uint8),
         ("pit_status", ctypes.c_uint8),
         ("num_pit_stops", ctypes.c_uint8),
         ("sector", ctypes.c_uint8),
         ("current_lap_invalid", ctypes.c_uint8),
         ("penalties", ctypes.c_uint8),
-        ("warnings", ctypes.c_uint8),
+        ("total_warnings", ctypes.c_uint8),
+        ("corner_cutting_warnings", ctypes.c_uint8),
         ("num_unserved_drive_through_pens", ctypes.c_uint8),
         ("num_unserved_stop_go_pens", ctypes.c_uint8),
         ("grid_position", ctypes.c_uint8),
         ("driver_status", ctypes.c_uint8),
         ("result_status", ctypes.c_uint8),
         ("pit_lane_timer_active", ctypes.c_uint8),
         ("pit_lane_time_in_lane_in_ms", ctypes.c_uint16),
@@ -327,27 +326,35 @@
 
 class Buttons(Packet):
     _fields_ = [
         ("button_status", ctypes.c_uint32),
     ]
 
 
+class Overtake(Packet):
+    _fields_ = [
+        ("overtaking_vehicle_idx", ctypes.c_uint8),
+        ("being_overtaken_vehicle_idx", ctypes.c_uint8),
+    ]
+
+
 class EventDataDetails(ctypes.Union, PacketMixin):
     _fields_ = [
         ("fastest_lap", FastestLap),
         ("retirement", Retirement),
         ("team_mate_in_pits", TeamMateInPits),
         ("race_winner", RaceWinner),
         ("penalty", Penalty),
         ("speed_trap", SpeedTrap),
         ("start_l_ights", StartLIghts),
         ("drive_through_penalty_served", DriveThroughPenaltyServed),
         ("stop_go_penalty_served", StopGoPenaltyServed),
         ("flashback", Flashback),
         ("buttons", Buttons),
+        ("overtake", Overtake),
     ]
 
 
 class PacketEventData(Packet):
     _fields_ = [
         ("header", PacketHeader),
         ("event_string_code", ctypes.c_uint8 * 4),
@@ -362,14 +369,16 @@
         ("network_id", ctypes.c_uint8),
         ("team_id", ctypes.c_uint8),
         ("my_team", ctypes.c_uint8),
         ("race_number", ctypes.c_uint8),
         ("nationality", ctypes.c_uint8),
         ("name", ctypes.c_char * 48),
         ("your_telemetry", ctypes.c_uint8),
+        ("show_online_names", ctypes.c_uint8),
+        ("platform", ctypes.c_uint8),
     ]
 
 
 class PacketParticipantsData(Packet):
     _fields_ = [
         ("header", PacketHeader),
         ("num_active_cars", ctypes.c_uint8),
@@ -457,14 +466,16 @@
         ("max_gears", ctypes.c_uint8),
         ("drs_allowed", ctypes.c_uint8),
         ("drs_activation_distance", ctypes.c_uint16),
         ("actual_tyre_compound", ctypes.c_uint8),
         ("visual_tyre_compound", ctypes.c_uint8),
         ("tyres_age_laps", ctypes.c_uint8),
         ("vehicle_fia_flags", ctypes.c_int8),
+        ("engine_power_ice", ctypes.c_float),
+        ("engine_power_mguk", ctypes.c_float),
         ("ers_store_energy", ctypes.c_float),
         ("ers_deploy_mode", ctypes.c_uint8),
         ("ers_harvested_this_lap_mguk", ctypes.c_float),
         ("ers_harvested_this_lap_mguh", ctypes.c_float),
         ("ers_deployed_this_lap", ctypes.c_float),
         ("network_paused", ctypes.c_uint8),
     ]
@@ -505,14 +516,15 @@
 
 
 class LobbyInfoData(Packet):
     _fields_ = [
         ("ai_controlled", ctypes.c_uint8),
         ("team_id", ctypes.c_uint8),
         ("nationality", ctypes.c_uint8),
+        ("platform", ctypes.c_uint8),
         ("name", ctypes.c_char * 48),
         ("car_number", ctypes.c_uint8),
         ("ready_status", ctypes.c_uint8),
     ]
 
 
 class PacketLobbyInfoData(Packet):
@@ -556,16 +568,19 @@
     ]
 
 
 class LapHistoryData(Packet):
     _fields_ = [
         ("lap_time_in_ms", ctypes.c_uint32),
         ("sector1_time_in_ms", ctypes.c_uint16),
+        ("sector1_time_minutes", ctypes.c_uint8),
         ("sector2_time_in_ms", ctypes.c_uint16),
+        ("sector1_time_minutes", ctypes.c_uint8),
         ("sector3_time_in_ms", ctypes.c_uint16),
+        ("sector3_time_minutes", ctypes.c_uint8),
         ("lap_valid_bit_flags", ctypes.c_uint8),
     ]
 
 
 class TyreStintHistoryData(Packet):
     _fields_ = [
         ("end_lap", ctypes.c_uint8),
@@ -585,27 +600,78 @@
         ("best_sector2_lap_num", ctypes.c_uint8),
         ("best_sector3_lap_num", ctypes.c_uint8),
         ("lap_history_data", LapHistoryData * 100),
         ("tyre_stints_history_data", TyreStintHistoryData * 8),
     ]
 
 
+class TyreSetData(Packet):
+    _fields_ = [
+        ("actual_tyre_compound", ctypes.c_uint8),
+        ("visual_tyre_compound", ctypes.c_uint8),
+        ("wear", ctypes.c_uint8),
+        ("available", ctypes.c_uint8),
+        ("recommended_session", ctypes.c_uint8),
+        ("life_span", ctypes.c_uint8),
+        ("usable_life", ctypes.c_uint8),
+        ("lap_delta_time", ctypes.c_int16),
+        ("fitted", ctypes.c_uint8),
+    ]
+
+
+class PacketTyreSetsData(Packet):
+    _fields_ = [
+        ("header", PacketHeader),
+        ("car_idx", ctypes.c_uint8),
+        ("tyre_set_data", TyreSetData * 20),
+        ("fitted_idx", ctypes.c_uint8),
+    ]
+
+
+class PacketMotionExData(Packet):
+    _fields_ = [
+        ("header", PacketHeader),
+        ("suspension_position", ctypes.c_float * 4),
+        ("suspension_velocity", ctypes.c_float * 4),
+        ("suspension_acceleration", ctypes.c_float * 4),
+        ("wheel_speed", ctypes.c_float * 4),
+        ("wheel_slip_ratio", ctypes.c_float * 4),
+        ("wheel_slip_angle", ctypes.c_float * 4),
+        ("wheel_lat_force", ctypes.c_float * 4),
+        ("wheel_long_force", ctypes.c_float * 4),
+        ("height_of_cog_above_ground", ctypes.c_float),
+        ("local_velocity_x", ctypes.c_float),
+        ("local_velocity_y", ctypes.c_float),
+        ("local_velocity_z", ctypes.c_float),
+        ("angular_velocity_x", ctypes.c_float),
+        ("angular_velocity_y", ctypes.c_float),
+        ("angular_velocity_z", ctypes.c_float),
+        ("angular_acceleration_x", ctypes.c_float),
+        ("angular_acceleration_y", ctypes.c_float),
+        ("angular_acceleration_z", ctypes.c_float),
+        ("front_wheels_angle", ctypes.c_float),
+        ("wheel_vert_force", ctypes.c_float * 4),
+    ]
+
+
 HEADER_FIELD_TO_PACKET_TYPE = {
-    (2022, 1, 0): PacketMotionData,
-    (2022, 1, 1): PacketSessionData,
-    (2022, 1, 2): PacketLapData,
-    (2022, 1, 3): PacketEventData,
-    (2022, 1, 4): PacketParticipantsData,
-    (2022, 1, 5): PacketCarSetupData,
-    (2022, 1, 6): PacketCarTelemetryData,
-    (2022, 1, 7): PacketCarStatusData,
-    (2022, 1, 8): PacketFinalClassificationData,
-    (2022, 1, 9): PacketLobbyInfoData,
-    (2022, 1, 10): PacketCarDamageData,
-    (2022, 1, 11): PacketSessionHistoryData,
+    (2023, 1, 0): PacketMotionData,
+    (2023, 1, 1): PacketSessionData,
+    (2023, 1, 2): PacketLapData,
+    (2023, 1, 3): PacketEventData,
+    (2023, 1, 4): PacketParticipantsData,
+    (2023, 1, 5): PacketCarSetupData,
+    (2023, 1, 6): PacketCarTelemetryData,
+    (2023, 1, 7): PacketCarStatusData,
+    (2023, 1, 8): PacketFinalClassificationData,
+    (2023, 1, 9): PacketLobbyInfoData,
+    (2023, 1, 10): PacketCarDamageData,
+    (2023, 1, 11): PacketSessionHistoryData,
+    (2023, 1, 12): PacketTyreSetsData,
+    (2023, 1, 13): PacketMotionExData,
 }
 # [[[end]]]
 
 
 def resolve(packet):
     header = PacketHeader.from_buffer_copy(packet)
     key = (header.packet_format, header.packet_version, header.packet_id)
@@ -649,8 +715,10 @@
     24: "Suzuka Short",
     25: "Hanoi",
     26: "Zandvoort",
     27: "Imola",
     28: "Portimão",
     29: "Jeddah",
     30: "Miami",
+    31: "Las Vegas",
+    32: "Losail",
 }
```

### Comparing `f1-packets-2022.1.2/pyproject.toml` & `f1_packets-2023.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 authors = ["Gabriele N. Tornetta <phoenix1987@gmail.com>"]
 license = "MIT"
 packages = [
   {include = "f1"},
 ]
 readme = "README.md"
 repository = "https://github.com/P403n1x87/f1-packets"
-version = "2022.1.2"
+version = "2023.1.0"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 [tool.poetry.urls]
 issues = "https://github.com/P403n1x87/f1-packets/issues"
```

### Comparing `f1-packets-2022.1.2/PKG-INFO` & `f1_packets-2023.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: f1-packets
-Version: 2022.1.2
+Version: 2023.1.0
 Summary: Python library for the official F1 game UDP telemetry data
 Home-page: https://github.com/P403n1x87/f1-packets
 License: MIT
 Author: Gabriele N. Tornetta
 Author-email: phoenix1987@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/P403n1x87/f1-packets
 Project-URL: issues, https://github.com/P403n1x87/f1-packets/issues
 Description-Content-Type: text/markdown
 
 # F1 Packets
 
 Python library for the official F1 game UDP telemetry data
```

