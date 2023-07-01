# Comparing `tmp/aiovantage-0.4.0.tar.gz` & `tmp/aiovantage-0.5.0.tar.gz`

## Comparing `aiovantage-0.4.0.tar` & `aiovantage-0.5.0.tar`

### file list

```diff
@@ -1,153 +1,156 @@
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 aiovantage-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 aiovantage-0.4.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 aiovantage-0.4.0/testrgbw.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 aiovantage-0.4.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.4.0/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 aiovantage-0.4.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 aiovantage-0.4.0/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 aiovantage-0.4.0/.vscode/settings.json
--rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/dump_system.py
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/monitor_all.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/anemo_sensors/dump_anemo_sensors.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/anemo_sensors/monitor_anemo_sensors.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/areas/dump_areas.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/blind_groups/dump_blind_groups.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/blinds/dump_blinds.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/blinds/monitor_blinds.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/buttons/dump_buttons.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/buttons/monitor_buttons.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/command_client/event_log.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/command_client/status_load.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/config_client/dump_objects.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/config_client/get_version.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/dry_contacts/dump_dry_contacts.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/dry_contacts/monitor_dry_contacts.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/gmem/dump_gmem.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/gmem/monitor_gmem.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/gmem/set_gmem.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/light_sensors/dump_light_sensors.py
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/light_sensors/monitor_light_sensors.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/load_groups/dump_load_groups.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/loads/control_load.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/loads/dump_loads.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/loads/monitor_loads.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/loads/poll_on_loads.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/loads/toggle_load.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/omni_sensors/dump_omni_sensors.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/omni_sensors/monitor_omni_sensors.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/rgb_loads/dump_rgb_loads.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/rgb_loads/monitor_rgb_loads.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/stations/dump_stations.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/stations/jingle_bells.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/tasks/dump_tasks.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/tasks/run_task.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/temperature_sensors/dump_temperature_sensors.py
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 aiovantage-0.4.0/examples/temperature_sensors/monitor_temperature_sensors.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/__about__.py
--rw-r--r--   0        0        0     9122 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/__init__.py
--rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/connection.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/errors.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/events.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/py.typed
--rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/query.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/README.md
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/__init__.py
--rw-r--r--   0        0        0     6308 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/commands.py
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/events.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/utils.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/__init__.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/anemo_sensor.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/base.py
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/blind.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/button.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/color_temperature.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/gmem.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/introspection.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/light_sensor.py
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/load.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/object.py
--rw-r--r--   0        0        0     9678 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/rgb_load.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/sensor.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/sounder.py
--rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/task.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/command_client/interfaces/temperature.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/README.md
--rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/__init__.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/helpers.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/xml_dataclass.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/methods/__init__.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/methods/types.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/methods/configuration/__init__.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/methods/configuration/close_filter.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/methods/configuration/get_filter_results.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/methods/configuration/get_object.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/methods/configuration/open_filter.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/methods/introspection/__init__.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/methods/introspection/get_version.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/methods/login/__init__.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/methods/login/login.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/__init__.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/anemo_sensor.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/area.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/blind.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/blind_group.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/button.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/dc_power_profile.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/ddg_color_load.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/dg_color_load.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/dimmer.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/dry_contact.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/dual_relay_station.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/eq_ctrl.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/eq_ux.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/gmem.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/keypad.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/light_sensor.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/load.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/load_group.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/location_object.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/master.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/module.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/module_gen2.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/omni_sensor.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/power_profile.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/pwm_power_profile.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/qis_blind.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/qube_blind.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/relay_blind.py
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/rgb_load.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/scene_point_relay.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/sensor.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/station_bus.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/station_object.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/system_object.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/task.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/temperature.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/somfy/rs485_group.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/somfy/rs485_shade.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/somfy/urtsi_2_group.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/config_client/objects/somfy/urtsi_2_shade.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/__init__.py
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/anemo_sensors.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/areas.py
--rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/base.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/blind_groups.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/blinds.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/buttons.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/dry_contacts.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/gmem.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/light_sensors.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/load_groups.py
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/loads.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/masters.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/modules.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/omni_sensors.py
--rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/rgb_loads.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/stations.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/tasks.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 aiovantage-0.4.0/src/aiovantage/controllers/temperature_sensors.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 aiovantage-0.4.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.4.0/LICENSE
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 aiovantage-0.4.0/README.md
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 aiovantage-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 aiovantage-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 aiovantage-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 aiovantage-0.5.0/.pylintrc
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 aiovantage-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aiovantage-0.5.0/TODO
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 aiovantage-0.5.0/test.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 aiovantage-0.5.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.5.0/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 aiovantage-0.5.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 aiovantage-0.5.0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 aiovantage-0.5.0/.vscode/settings.json
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/dump_system.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/monitor_all.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/anemo_sensors/dump_anemo_sensors.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/anemo_sensors/monitor_anemo_sensors.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/areas/dump_areas.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/blind_groups/dump_blind_groups.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/blinds/dump_blinds.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/blinds/monitor_blinds.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/buttons/dump_buttons.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/buttons/monitor_buttons.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/command_client/event_log.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/command_client/status_load.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/config_client/dump_objects.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/config_client/get_version.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/dry_contacts/dump_dry_contacts.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/dry_contacts/monitor_dry_contacts.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/gmem/dump_gmem.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/gmem/monitor_gmem.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/gmem/set_gmem.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/light_sensors/dump_light_sensors.py
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/light_sensors/monitor_light_sensors.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/load_groups/dump_load_groups.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/loads/control_load.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/loads/dump_loads.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/loads/monitor_loads.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/loads/poll_on_loads.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/loads/toggle_load.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/omni_sensors/dump_omni_sensors.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/omni_sensors/monitor_omni_sensors.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/rgb_loads/dump_rgb_loads.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/rgb_loads/monitor_rgb_loads.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/stations/dump_stations.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/stations/jingle_bells.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/tasks/dump_tasks.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/tasks/run_task.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/temperature_sensors/dump_temperature_sensors.py
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/temperature_sensors/monitor_temperature_sensors.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/__about__.py
+-rw-r--r--   0        0        0     9851 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/__init__.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/connection.py
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/discovery.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/errors.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/events.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/py.typed
+-rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/query.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/README.md
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/__init__.py
+-rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/commands.py
+-rw-r--r--   0        0        0    14769 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/events.py
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/utils.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/__init__.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/anemo_sensor.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/base.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/blind.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/button.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/color_temperature.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/gmem.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/introspection.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/light_sensor.py
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/load.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/object.py
+-rw-r--r--   0        0        0     9652 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/rgb_load.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/sensor.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/sounder.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/task.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/temperature.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/README.md
+-rw-r--r--   0        0        0     7178 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/__init__.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/helpers.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/xml_dataclass.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/methods/__init__.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/methods/types.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/methods/configuration/__init__.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/methods/configuration/close_filter.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/methods/configuration/get_filter_results.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/methods/configuration/get_object.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/methods/configuration/open_filter.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/methods/introspection/__init__.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/methods/introspection/get_version.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/methods/login/__init__.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/methods/login/login.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/__init__.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/anemo_sensor.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/area.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/blind.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/blind_group.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/button.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/dc_power_profile.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/ddg_color_load.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/dg_color_load.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/dimmer.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/dry_contact.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/dual_relay_station.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/eq_ctrl.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/eq_ux.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/gmem.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/keypad.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/light_sensor.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/load.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/load_group.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/location_object.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/master.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/module.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/module_gen2.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/omni_sensor.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/power_profile.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/pwm_power_profile.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/qis_blind.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/qube_blind.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/relay_blind.py
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/rgb_load.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/scene_point_relay.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/sensor.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/station_bus.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/station_object.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/system_object.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/task.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/temperature.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/somfy/rs485_group.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/somfy/rs485_shade.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/somfy/urtsi_2_group.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/somfy/urtsi_2_shade.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/__init__.py
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/anemo_sensors.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/areas.py
+-rw-r--r--   0        0        0    12714 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/base.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/blind_groups.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/blinds.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/buttons.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/dry_contacts.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/gmem.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/light_sensors.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/load_groups.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/loads.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/masters.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/modules.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/omni_sensors.py
+-rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/rgb_loads.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/stations.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/tasks.py
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/temperature_sensors.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 aiovantage-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.5.0/LICENSE
+-rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 aiovantage-0.5.0/README.md
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 aiovantage-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 aiovantage-0.5.0/PKG-INFO
```

### Comparing `aiovantage-0.4.0/.pre-commit-config.yaml` & `aiovantage-0.5.0/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -18,9 +18,8 @@
           - xsdata==23.6
         args: []
 
   - repo: https://github.com/thlorenz/doctoc
     rev: v2.2.0
     hooks:
       - id: doctoc
-        args: ["--github", "--notitle", "--maxlevel=2"]
-        files: CONTRIBUTING.md
+        args: ["--github", "--notitle", "--maxlevel=2", "--update-only"]
```

### Comparing `aiovantage-0.4.0/CONTRIBUTING.md` & `aiovantage-0.5.0/CONTRIBUTING.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Contributing
 
 First off, thanks for taking the time to contribute!
 
+## Table of contents
+
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
 - [🔨 Set up Development Environment](#-set-up-development-environment)
 - [✨ Submit your work](#-submit-your-work)
 - [🎨 Style guidelines](#-style-guidelines)
 - [📦️ Build a package](#%EF%B8%8F-build-a-package)
```

### Comparing `aiovantage-0.4.0/.github/ISSUE_TEMPLATE/bug.yml` & `aiovantage-0.5.0/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/.github/ISSUE_TEMPLATE/feature_request.yml` & `aiovantage-0.5.0/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/dump_system.py` & `aiovantage-0.5.0/examples/dump_system.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/monitor_all.py` & `aiovantage-0.5.0/examples/monitor_all.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/anemo_sensors/dump_anemo_sensors.py` & `aiovantage-0.5.0/examples/anemo_sensors/dump_anemo_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/anemo_sensors/monitor_anemo_sensors.py` & `aiovantage-0.5.0/examples/anemo_sensors/monitor_anemo_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/areas/dump_areas.py` & `aiovantage-0.5.0/examples/areas/dump_areas.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/blind_groups/dump_blind_groups.py` & `aiovantage-0.5.0/examples/blind_groups/dump_blind_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/blinds/dump_blinds.py` & `aiovantage-0.5.0/examples/blinds/dump_blinds.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/blinds/monitor_blinds.py` & `aiovantage-0.5.0/examples/blinds/monitor_blinds.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/buttons/dump_buttons.py` & `aiovantage-0.5.0/examples/buttons/dump_buttons.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/buttons/monitor_buttons.py` & `aiovantage-0.5.0/examples/buttons/monitor_buttons.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/command_client/event_log.py` & `aiovantage-0.5.0/examples/command_client/event_log.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/command_client/status_load.py` & `aiovantage-0.5.0/examples/command_client/status_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/config_client/dump_objects.py` & `aiovantage-0.5.0/examples/config_client/dump_objects.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/config_client/get_version.py` & `aiovantage-0.5.0/examples/config_client/get_version.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/dry_contacts/dump_dry_contacts.py` & `aiovantage-0.5.0/examples/dry_contacts/dump_dry_contacts.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/dry_contacts/monitor_dry_contacts.py` & `aiovantage-0.5.0/examples/dry_contacts/monitor_dry_contacts.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/gmem/dump_gmem.py` & `aiovantage-0.5.0/examples/gmem/dump_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/gmem/monitor_gmem.py` & `aiovantage-0.5.0/examples/gmem/monitor_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/gmem/set_gmem.py` & `aiovantage-0.5.0/examples/gmem/set_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/light_sensors/dump_light_sensors.py` & `aiovantage-0.5.0/examples/light_sensors/dump_light_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/light_sensors/monitor_light_sensors.py` & `aiovantage-0.5.0/examples/light_sensors/monitor_light_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/load_groups/dump_load_groups.py` & `aiovantage-0.5.0/examples/load_groups/dump_load_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/loads/control_load.py` & `aiovantage-0.5.0/examples/loads/control_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/loads/dump_loads.py` & `aiovantage-0.5.0/examples/loads/dump_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/loads/monitor_loads.py` & `aiovantage-0.5.0/examples/loads/monitor_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/loads/poll_on_loads.py` & `aiovantage-0.5.0/examples/loads/poll_on_loads.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     async with Vantage(args.host, args.username, args.password) as vantage:
         # Preload the loads from the controller
         await vantage.loads.initialize()
 
         # Print a list of all loads that are currently on every 5 seconds
         while True:
-            on_loads = list(vantage.loads.on)
+            on_loads = list(vantage.loads.is_on)
             print(f"{len(on_loads)} loads are ON")
             for load in on_loads:
                 print(f"- {load.name}")
             print()
 
             await asyncio.sleep(5)
```

### Comparing `aiovantage-0.4.0/examples/loads/toggle_load.py` & `aiovantage-0.5.0/examples/loads/toggle_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/omni_sensors/dump_omni_sensors.py` & `aiovantage-0.5.0/examples/omni_sensors/dump_omni_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/omni_sensors/monitor_omni_sensors.py` & `aiovantage-0.5.0/examples/omni_sensors/monitor_omni_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/rgb_loads/dump_rgb_loads.py` & `aiovantage-0.5.0/examples/rgb_loads/dump_rgb_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/rgb_loads/monitor_rgb_loads.py` & `aiovantage-0.5.0/examples/rgb_loads/monitor_rgb_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/stations/dump_stations.py` & `aiovantage-0.5.0/examples/stations/dump_stations.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/stations/jingle_bells.py` & `aiovantage-0.5.0/examples/stations/jingle_bells.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/tasks/dump_tasks.py` & `aiovantage-0.5.0/examples/tasks/dump_tasks.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/tasks/run_task.py` & `aiovantage-0.5.0/examples/tasks/run_task.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/temperature_sensors/dump_temperature_sensors.py` & `aiovantage-0.5.0/examples/temperature_sensors/dump_temperature_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/examples/temperature_sensors/monitor_temperature_sensors.py` & `aiovantage-0.5.0/examples/temperature_sensors/monitor_temperature_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/src/aiovantage/__init__.py` & `aiovantage-0.5.0/src/aiovantage/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -42,16 +42,24 @@
         username: Optional[str] = None,
         password: Optional[str] = None,
         *,
         use_ssl: bool = True,
         config_port: Optional[int] = None,
         command_port: Optional[int] = None,
     ) -> None:
-        """Initialize the Vantage instance."""
+        """Initialize the Vantage instance.
 
+        Args:
+            host: The hostname or IP address of the Vantage controller.
+            username: The username to use for authentication.
+            password: The password to use for authentication.
+            use_ssl: Whether to use SSL for the connection.
+            config_port: The port to use for the config client.
+            command_port: The port to use for the command client.
+        """
         # Set up clients
         self._config_client = ConfigClient(
             host, username, password, ssl=use_ssl, port=config_port
         )
 
         self._command_client = CommandClient(
             host, username, password, ssl=use_ssl, port=command_port
@@ -78,25 +86,24 @@
         self._omni_sensors = OmniSensorsController(self)
         self._stations = StationsController(self)
         self._tasks = TasksController(self)
         self._temperature_sensors = TemperatureSensorsController(self)
 
     async def __aenter__(self) -> Self:
         """Return context manager."""
-        await self.event_stream.start()
         return self
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> None:
         """Exit context manager."""
-        await self.close()
+        self.close()
         if exc_val:
             raise exc_val
 
     @property
     def config_client(self) -> ConfigClient:
         """Return the config client."""
         return self._config_client
@@ -192,50 +199,54 @@
         return self._tasks
 
     @property
     def temperature_sensors(self) -> TemperatureSensorsController:
         """Return the TemperatureSensors controller for managing temperature sensors."""
         return self._temperature_sensors
 
-    async def close(self) -> None:
+    def close(self) -> None:
         """Close the clients."""
-
         self.config_client.close()
         self.command_client.close()
-        await self.event_stream.stop()
+        self.event_stream.stop()
 
-    async def initialize(self) -> None:
-        """Fetch all objects from the controllers."""
+    async def initialize(self, fetch_state: bool = True) -> None:
+        """Fetch all objects from the controllers.
 
+        Args:
+            fetch_state: Whether to also fetch the state of each object.
+        """
         await asyncio.gather(
-            self._anemo_sensors.initialize(),
-            self._areas.initialize(),
-            self._blinds.initialize(),
-            self._blind_groups.initialize(),
-            self._buttons.initialize(),
-            self._dry_contacts.initialize(),
-            self._gmem.initialize(),
-            self._light_sensors.initialize(),
-            self._loads.initialize(),
-            self._masters.initialize(),
-            self._modules.initialize(),
-            self._rgb_loads.initialize(),
-            self._omni_sensors.initialize(),
-            self._stations.initialize(),
-            self._tasks.initialize(),
-            self._temperature_sensors.initialize(),
+            self._anemo_sensors.initialize(fetch_state),
+            self._areas.initialize(fetch_state),
+            self._blinds.initialize(fetch_state),
+            self._blind_groups.initialize(fetch_state),
+            self._buttons.initialize(fetch_state),
+            self._dry_contacts.initialize(fetch_state),
+            self._gmem.initialize(fetch_state),
+            self._light_sensors.initialize(fetch_state),
+            self._loads.initialize(fetch_state),
+            self._masters.initialize(fetch_state),
+            self._modules.initialize(fetch_state),
+            self._rgb_loads.initialize(fetch_state),
+            self._omni_sensors.initialize(fetch_state),
+            self._stations.initialize(fetch_state),
+            self._tasks.initialize(fetch_state),
+            self._temperature_sensors.initialize(fetch_state),
         )
 
     def subscribe(self, callback: EventCallback[SystemObject]) -> Callable[[], None]:
         """Subscribe to state changes for all objects.
 
+        Args:
+            callback: The callback to call when an object changes.
+
         Returns:
             A function to unsubscribe.
         """
-
         unsubscribes = [
             self.anemo_sensors.subscribe(callback),
             self.areas.subscribe(callback),
             self.blinds.subscribe(callback),
             self.blind_groups.subscribe(callback),
             self.buttons.subscribe(callback),
             self.dry_contacts.subscribe(callback),
```

### Comparing `aiovantage-0.4.0/src/aiovantage/connection.py` & `aiovantage-0.5.0/src/aiovantage/connection.py`

 * *Files identical despite different names*

```diff
@@ -45,15 +45,14 @@
         if port is None:
             self._port = self.default_ssl_port if ssl else self.default_port
         else:
             self._port = port
 
     async def open(self) -> None:
         """Open the connection."""
-
         # If we're already connected, do nothing
         if self._writer is not None and not self._writer.is_closing():
             return
 
         # Create the connection
         try:
             self._reader, self._writer = await asyncio.wait_for(
@@ -97,15 +96,14 @@
 
     async def write(self, message: str) -> None:
         """Send a plaintext message.
 
         Args:
             message: The message to send, as a string.
         """
-
         # Make sure we're connected
         if self._writer is None or self._writer.is_closing():
             raise ClientConnectionError("Client not connected.")
 
         # Send the request
         try:
             self._writer.write(message.encode())
@@ -119,15 +117,14 @@
         Args:
             separator: The separator to read until.
             timeout: The optional timeout in seconds.
 
         Returns:
             The data read, as a string.
         """
-
         # Make sure we're connected
         if self._reader is None or self.closed:
             raise ClientConnectionError("Client not connected.")
 
         # Read the response, with optional timeout
         try:
             data = await asyncio.wait_for(self._reader.readuntil(separator), timeout)
```

### Comparing `aiovantage-0.4.0/src/aiovantage/errors.py` & `aiovantage-0.5.0/src/aiovantage/errors.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,18 @@
     """Exception for client connection errors."""
 
 
 class ClientTimeoutError(asyncio.TimeoutError, ClientConnectionError):
     """Exception for client connection errors caused by timeouts."""
 
 
+class ClientResponseError(ClientError):
+    """Exception for client response errors."""
+
+
 class CommandError(ClientError):
     """Base exception for errors caused by sending commands or requests."""
 
 
 class LoginFailedError(CommandError):
     """Login failed."""
```

### Comparing `aiovantage-0.4.0/src/aiovantage/query.py` & `aiovantage-0.5.0/src/aiovantage/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 
         Args:
             data: The data dictionary to query.
             populate: A coroutine to populate the data so we don't have a complete
                       dataset before using "async for" loops.
             filters: A list of filters to apply to the queryset.
         """
-
         self.__data = data
         self.__populate = populate
         self.__iterator: Optional[Iterator[T]] = None
 
         if filters is None:
             self.__filters: List[Callable[[T], Any]] = []
         else:
@@ -115,15 +114,14 @@
 
     @overload
     def get(self, **kwargs: Any) -> Optional[T]:
         ...
 
     def get(self, *args: Any, **kwargs: Any) -> Optional[T]:
         """Get the first object that matches the given filter."""
-
         # Handle the case where we're getting an object by key
         if len(args) == 1 and isinstance(args[0], int):
             return self.__data.get(args[0], kwargs.get("default", None))
 
         # Otherwise, pass through to filter and return the first object
         return next(iter(self.filter(*args, **kwargs)), None)
```

### Comparing `aiovantage-0.4.0/src/aiovantage/command_client/README.md` & `aiovantage-0.5.0/src/aiovantage/command_client/README.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/src/aiovantage/command_client/__init__.py` & `aiovantage-0.5.0/src/aiovantage/command_client/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/src/aiovantage/command_client/commands.py` & `aiovantage-0.5.0/src/aiovantage/command_client/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     """The arguments of the "R:" line of the response."""
 
     data: List[str]
     """The data lines of the response, before the "R:" line."""
 
     def __init__(self, data: List[str]) -> None:
         """Initialize a CommandResponse."""
-
         # Extract "data" lines from the response. These are any lines before the
         # "R:" line, from commands such as "HELP" and "LISTSTATUS".
         self.data, return_line = data[:-1], data[-1]
 
         # Split the "R:" line into the command and arguments
         command, *self.args = tokenize_response(return_line)
 
@@ -109,15 +108,14 @@
             params: The parameters to send with the command.
             force_quotes: Whether to force string params to be wrapped in double quotes.
             connection: The connection to use, if not the default.
 
         Returns:
             A CommandResponse instance.
         """
-
         # Get a connection to the Host Command service
         conn = connection or await self.get_connection()
 
         # Build the request string, encoding the parameters if necessary
         if params:
             request = f"{command} {encode_params(*params, force_quotes=force_quotes)}"
         else:
```

### Comparing `aiovantage-0.4.0/src/aiovantage/command_client/events.py` & `aiovantage-0.5.0/src/aiovantage/command_client/events.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,53 +26,63 @@
 from typing_extensions import Self
 
 from aiovantage.errors import ClientConnectionError, ClientError
 
 from .commands import CommandConnection
 from .utils import tokenize_response
 
+# The interval between keepalive messages, in seconds.
 KEEPALIVE_INTERVAL = 60
 
 
-# Typing for events
 class EventType(Enum):
     """Enumeration of event types."""
 
     CONNECTED = "connect"
     DISCONNECTED = "disconnect"
     RECONNECTED = "reconnect"
     STATUS = "status"
     ENHANCED_LOG = "enhanced_log"
 
 
-# Typed dictionaries for events
 class ConnectEvent(TypedDict):
+    """Event emitted when the connection is established."""
+
     type: Literal[EventType.CONNECTED]
 
 
 class DisconnectEvent(TypedDict):
+    """Event emitted when the connection is lost."""
+
     type: Literal[EventType.DISCONNECTED]
 
 
 class ReconnectEvent(TypedDict):
+    """Event emitted when the connection is re-established."""
+
     type: Literal[EventType.RECONNECTED]
 
 
 class StatusEvent(TypedDict):
+    """Event emitted when a "S:" status is received."""
+
     type: Literal[EventType.STATUS]
     id: int
     status_type: str
     args: Sequence[str]
 
 
 class EnhancedLogEvent(TypedDict):
+    """Event emitted when an "EL:" enhanced log is received."""
+
     type: Literal[EventType.ENHANCED_LOG]
     log: str
 
 
+# Type alias for any event type
 Event = Union[
     ConnectEvent, DisconnectEvent, ReconnectEvent, StatusEvent, EnhancedLogEvent
 ]
 
 # Type aliases for callbacks for event subscriptions
 EventCallback = Callable[[Event], Union[None, Coroutine]]
 EventFilter = Callable[[Event], bool]
@@ -114,39 +124,41 @@
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> None:
         """Exit context manager."""
-        await self.stop()
+        self.stop()
         if exc_val:
             raise exc_val
 
     async def start(self) -> None:
         """Initialize the event stream."""
         async with self._start_lock:
             if self._started:
                 return
 
             await self.get_connection()
             self._tasks.append(asyncio.create_task(self._message_handler()))
             self._tasks.append(asyncio.create_task(self._command_handler()))
             self._tasks.append(asyncio.create_task(self._keepalive()))
 
+            self._logger.debug("Started the event stream")
             self._started = True
 
-    async def stop(self) -> None:
+    def stop(self) -> None:
         """Stop the event stream."""
-        async with self._start_lock:
-            for task in self._tasks:
-                task.cancel()
-            self._tasks.clear()
-            self._connection.close()
-            self._started = False
+        for task in self._tasks:
+            task.cancel()
+        self._tasks.clear()
+        self._connection.close()
+
+        self._logger.debug("Stopped the event stream")
+        self._started = False
 
     async def get_connection(self) -> CommandConnection:
         """Get a connection to the Host Command service."""
         async with self._connection_lock:
             if self._connection.closed:
                 # Open a new connection
                 await self._connection.open()
@@ -167,15 +179,14 @@
         Args:
             callback: The callback to invoke when an event is received.
             event_filter: A filter to apply to events before invoking the callback.
 
         Returns:
             A function that can be used to unsubscribe from events.
         """
-
         # Support filtering by event type, a list of event types, or a predicate
         subscription: EventSubscription
         if isinstance(event_filter, EventType):
             subscription = (callback, lambda event: event["type"] == event_filter)
         elif isinstance(event_filter, Iterable):
             subscription = (callback, lambda event: event["type"] in event_filter)  # type: ignore[operator]
         else:
@@ -197,15 +208,14 @@
         Args:
             callback: The callback to invoke when an event is received.
             status_types: The status types to subscribe to status events for.
 
         Returns:
             A coroutine that can be used to unsubscribe from status events.
         """
-
         # Support both a single status type and a list of status types
         if isinstance(status_types, str):
             status_types = (status_types,)
 
         # Enable this status type if it's not already enabled
         for status_type in status_types:
             self._status_subscribers[status_type] += 1
@@ -233,21 +243,19 @@
     def subscribe_enhanced_log(
         self, callback: EventCallback, log_types: Union[str, Iterable[str]]
     ) -> Callable[[], None]:
         """Subscribe to "Enhanced Log" events from the Host Command service.
 
         Args:
             callback: The callback to invoke when an event is received.
-            log_types: The event log types to subscribe to.
+            log_types: The event log type or types to subscribe to.
 
         Returns:
             A coroutine that can be used to unsubscribe from log events.
         """
-
-        # Support both a single log type and a list of log types
         if isinstance(log_types, str):
             log_types = (log_types,)
 
         # Enable this log type if it's not already enabled
         for log_type in log_types:
             self._enhanced_log_subscribers[log_type] += 1
             if self._enhanced_log_subscribers[log_type] == 1:
@@ -380,16 +388,17 @@
         # Queue a command to be sent to the Host Command service.
         self._command_queue.put_nowait(command)
 
     def _enable_status(self, status_type: str) -> None:
         # Enable status updates on the controller for a particular status type.
         self._queue_command(f"STATUS {status_type}")
 
-    def _disable_status(self, status_type: str) -> None:
+    def _disable_status(self, _status_type: str) -> None:
         # Disable status updates on the controller for a particular status type.
+        # Note: This assumes the count has already been decremented.
         self._queue_command("STATUS NONE")
         for status_type, count in self._status_subscribers.items():
             if count > 0:
                 self._queue_command(f"STATUS {status_type}")
 
     def _enable_enhanced_log(self, log_type: str) -> None:
         # Enable enhanced logging on the controller for a particular log type.
```

### Comparing `aiovantage-0.4.0/src/aiovantage/command_client/utils.py` & `aiovantage-0.5.0/src/aiovantage/command_client/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
     Args:
         string: The response string to tokenize.
 
     Returns:
         A list of string tokens.
     """
-
     tokens = []
     for match in TOKEN_PATTERN.finditer(string):
         token = match.group(0)
 
         # Remove quotes from quoted strings, and unescape quotes
         if token.startswith('"') and token.endswith('"'):
             token = token[1:-1].replace('""', '"')
@@ -43,15 +42,14 @@
     Args:
         params: The parameters to encode.
         force_quotes: Whether to force string params to be wrapped in double quotes.
 
     Returns:
         The encoded parameters, joined by spaces.
     """
-
     encoded_params = []
 
     for value in params:
         if isinstance(value, str):
             if '"' in value or " " in value or force_quotes:
                 value = value.replace('"', '""')
                 encoded_params.append(f'"{value}"')
```

### Comparing `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/__init__.py` & `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/anemo_sensor.py` & `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/anemo_sensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
     async def get_speed(self, vid: int) -> Decimal:
         """Get the value of an anemo sensor, in mph.
 
         Args:
             vid: The Vantage ID of the anemo sensor.
         """
-
         # INVOKE <id> AnemoSensor.GetSpeed
         # -> R:INVOKE <id> <speed> AnemoSensor.GetSpeed
         response = await self.invoke(vid, "AnemoSensor.GetSpeed")
         level = Decimal(response.args[1])
 
         return level
 
@@ -29,14 +28,12 @@
 
         Args:
             args: The arguments of the event.
 
         Returns:
             The value of the anemo sensor, in mph.
         """
-
         # ELLOG STATUS ON
         # -> EL: <id> AnemoSensor.GetSpeed <speed>
-
         # STATUS ADD <id>
         # -> S:STATUS <id> AnemoSensor.GetSpeed <speed>
         return Decimal(args[0]) / 1000
```

### Comparing `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/base.py` & `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/blind.py` & `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/blind.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,105 +17,95 @@
 
     async def open(self, vid: int) -> None:
         """Open a blind.
 
         Args:
             vid: The Vantage ID of the blind.
         """
-
         # INVOKE <id> Blind.Open
         # -> R:INVOKE <id> <rcode> Blind.Open
         await self.invoke(vid, "Blind.Open")
 
     async def close(self, vid: int) -> None:
         """Close a blind.
 
         Args:
             vid: The Vantage ID of the blind.
         """
-
         # INVOKE <id> Blind.Close
         # -> R:INVOKE <id> <rcode> Blind.Close
         await self.invoke(vid, "Blind.Close")
 
     async def stop(self, vid: int) -> None:
         """Stop a blind.
 
         Args:
             vid: The Vantage ID of the blind.
         """
-
         # INVOKE <id> Blind.Stop
         # -> R:INVOKE <id> <rcode> Blind.Stop
         await self.invoke(vid, "Blind.Stop")
 
     async def get_position(self, vid: int) -> Decimal:
         """Get the position of a blind.
 
         Args:
             vid: The Vantage ID of the blind.
 
         Returns:
             The position of the blind, as a percentage.
         """
-
         # INVOKE <id> Blind.GetPosition
         # -> R:INVOKE <id> <position (0-100.000)> Blind.GetPosition
         response = await self.invoke(vid, "Blind.GetPosition")
         position = Decimal(response.args[1])
 
         return position
 
     async def set_position(self, vid: int, position: float) -> None:
         """Set the position of a blind.
 
         Args:
             vid: The Vantage ID of the blind.
             position: The position to set the blind to, as a percentage.
         """
-
         # INVOKE <id> Blind.SetPosition <position>
         # -> R:INVOKE <id> <rcode> Blind.SetPosition <position>
         await self.invoke(vid, "Blind.SetPosition", position)
 
     @classmethod
     def parse_blind_status(cls, args: Sequence[str]) -> Decimal:
         """Parse a simple 'S:BLIND' event.
 
         Args:
             args: The arguments of the event.
 
         Returns:
             The position of the blind, as a percentage.
         """
-
         # STATUS BLIND
         # -> S:BLIND <id> <position (0-100.000)>
         return Decimal(args[0])
 
     @classmethod
     def parse_get_position_status(cls, args: Sequence[str]) -> Decimal:
         """Parse a 'Blind.GetPosition' event."""
-
         # ELLOG STATUS ON
         # -> EL: <id> Blind.GetPosition <position (0-100000)>
-
         # ADDSTATUS <id>
         # -> S:STATUS <id> Blind.GetPosition <position (0-100000)>
         position = Decimal(args[0]) / 1000
 
         return position
 
     @classmethod
     def parse_get_state_status(cls, args: Sequence[str]) -> BlindState:
         """Parse a 'Blind.GetBlindState' event."""
-
         # ADDSTATUS <id>
         # -> S:STATUS <id> Blind.GetBlindState <moving> <start> <end> <transitionTime> <startTime>
-
         # ELLOG STATUSEX ON
         # -> EL: <id> Blind.GetBlindState <moving> <start> <end> <transitionTime> <startTime>
         return cls.BlindState(
             # Is the blind currently moving?
             is_moving=bool(int(args[0])),
             # Position the blind is moving from (as a percentage)
             start_pos=Decimal(args[1]) / 1000,
```

### Comparing `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/button.py` & `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/button.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
         Args:
             vid: The Vantage ID of the button.
 
         Returns:
             The pressed state of the button, True if pressed, False if not.
         """
-
         # INVOKE <id> Button.GetState
         # -> R:INVOKE <id> <state (Up/Down)> Button.GetState
         response = await self.invoke(vid, "Button.GetState")
         state = response.args[1]
         if state == "Up":
             return False
         if state == "Down":
@@ -32,58 +31,53 @@
     async def set_state(self, vid: int, pressed: bool) -> None:
         """Set the state of a button.
 
         Args:
             vid: The Vantage ID of the button.
             pressed: The state to set the button to, either a State.UP or State.DOWN.
         """
-
         # INVOKE <id> Button.SetState <state (0/1/Up/Down)>
         # -> R:INVOKE <id> Button.SetState <state (Up/Down)>
         await self.invoke(vid, "Button.SetState", pressed)
 
     async def press(self, vid: int) -> None:
         """Press a button.
 
         Args:
             vid: The Vantage ID of the button.
         """
-
         await self.set_state(vid, True)
 
     async def release(self, vid: int) -> None:
         """Release a button.
 
         Args:
             vid: The Vantage ID of the button.
         """
-
         await self.set_state(vid, False)
 
     async def press_and_release(self, vid: int) -> None:
         """Press and release a button.
 
         Args:
             vid: The Vantage ID of the button.
         """
-
         await self.press(vid)
         await self.release(vid)
 
     @classmethod
     def parse_btn_status(cls, args: Sequence[str]) -> bool:
         """Parse a simple 'S:BTN' event.
 
         Args:
             args: The arguments of the event.
 
         Returns:
             The state of the button, either a State.UP or State.DOWN.
         """
-
         # STATUS BTN
         # -> S:BTN <id> <state (PRESS/RELEASE)>
         state = args[0]
         if state == "RELEASE":
             return False
         if state == "PRESS":
             return True
@@ -96,14 +90,12 @@
 
         Args:
             args: The arguments of the event.
 
         Returns:
             The state of the button, either a State.UP or State.DOWN.
         """
-
         # ELLOG STATUS ON
         # -> EL: <id> Button.GetState <state (0/1)>
-
         # STATUS ADD <id>
         # -> S:STATUS <id> Button.GetState <state (0/1)>
         return bool(int(args[0]))
```

### Comparing `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/color_temperature.py` & `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/color_temperature.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
         Args:
             vid: The Vantage ID of the light.
 
         Returns:
             The color temperature of the light, in Kelvin.
         """
-
         # INVOKE <id> ColorTemperature.Get
         # -> R:INVOKE <id> <temp> ColorTemperature.Get
         response = await self.invoke(vid, "ColorTemperature.Get")
         color_temp = int(response.args[1])
 
         return color_temp
 
@@ -29,15 +28,14 @@
         """Set the color temperature of a light.
 
         Args:
             vid: The Vantage ID of the light.
             temp: The color temperature to set the light to, in Kelvin.
             transition: The time in seconds to transition to the new color
         """
-
         # Ensure the temperature is an integer
         temp = int(temp)
 
         # INVOKE <id> ColorTemperature.Set <temp> <seconds>
         # -> R:INVOKE <id> <rcode> ColorTemperature.Set <temp>
         await self.invoke(vid, "ColorTemperature.Set", temp, transition)
 
@@ -49,13 +47,12 @@
             args: The arguments of the event.
 
         Returns:
             The color temperature, in Kelvin.
         """
         # ELLOG STATUS ON
         # -> EL: <id> ColorTemperature.Get <temp>
-
         # STATUS ADD <id>
         # -> S:STATUS <id> ColorTemperature.Get <temp>
         color_temp = int(args[0])
 
         return color_temp
```

### Comparing `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/gmem.py` & `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/gmem.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,41 +13,38 @@
 
         Args:
             vid: The Vantage ID of the variable.
 
         Returns:
             The value of the variable, as a raw string.
         """
-
         # GETVARIABLE {id}
         # -> R:GETVARIABLE {id} {value}
         response = await self.command_client.command("GETVARIABLE", vid)
         value = response.args[1]
 
         return value
 
     async def set_value(self, vid: int, value: Union[int, str, bool]) -> None:
         """Set the value of a variable.
 
         Args:
             vid: The Vantage ID of the variable.
             value: The value to set, either a bool, int, or str.
         """
-
         # SETVARIABLE {id} {value}
         # -> R:SETVARIABLE {id} {value}
         await self.command_client.command("VARIABLE", vid, value, force_quotes=True)
 
     @classmethod
     def parse_variable_status(cls, args: Sequence[str]) -> str:
         """Parse a simple 'S:VARIABLE' event.
 
         Args:
             args: The arguments of the event.
 
         Returns:
             The level of the load.
         """
-
         # STATUS VARIABLE
         # -> S:VARIABLE <id> <value>
         return args[0]
```

### Comparing `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/introspection.py` & `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/introspection.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,13 +18,12 @@
     async def get_firmware_version(self, vid: int, image: Firmware) -> str:
         """Get the firmware version.
 
         Args:
             vid: The Vantage ID of the controller.
             image: The firmware image to get the version of.
         """
-
         # INVOKE <id> IntroSpection.GetFirmwareVersion <image>
         # -> R:INVOKE <id> <rcode> IntroSpection.GetFirmwareVersion <image> <version>
         response = await self.invoke(vid, "IntroSpection.GetFirmwareVersion", image)
 
         return response.args[4].rstrip()
```

### Comparing `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/light_sensor.py` & `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/light_sensor.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,20 +6,19 @@
 from .base import Interface
 
 
 class LightSensorInterface(Interface):
     """Interface for querying and controlling light sensors."""
 
     async def get_level(self, vid: int) -> Decimal:
-        """Get the level of a light sensor, in foot-candles
+        """Get the level of a light sensor, in foot-candles.
 
         Args:
             vid: The Vantage ID of the light sensor.
         """
-
         # INVOKE <id> LightSensor.GetLevel
         # -> R:INVOKE <id> <level> LightSensor.GetLevel
         response = await self.invoke(vid, "LightSensor.GetLevel")
         level = Decimal(response.args[1])
 
         return level
 
@@ -29,14 +28,12 @@
 
         Args:
             args: The arguments of the event.
 
         Returns:
             The level of the light sensor, in foot-candles.
         """
-
         # ELLOG STATUS ON
         # -> EL: <id> LightSensor.GetLevel <level>
-
         # STATUS ADD <id>
         # -> S:STATUS <id> LightSensor.GetLevel <level>
         return Decimal(args[0]) / 1000
```

### Comparing `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/load.py` & `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/load.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,58 +26,54 @@
         """Turn on a load.
 
         Args:
             vid: The Vantage ID of the load.
             transition: The time in seconds to transition to the new level.
             level: The level to set the load to (0-100).
         """
-
         if transition:
             await self.ramp(vid, level, transition)
         else:
             await self.set_level(vid, level)
 
     async def turn_off(self, vid: int, transition: float = 0) -> None:
         """Turn off a load.
 
         Args:
             vid: The Vantage ID of the load.
             transition: The time in seconds to ramp the load down.
         """
-
         if transition:
             await self.ramp(vid, 0, transition)
         else:
             await self.set_level(vid, 0)
 
     async def get_level(self, vid: int) -> float:
         """Get the level of a load.
 
         Args:
             vid: The Vantage ID of the load.
 
         Returns:
             The level of the load, as a percentage (0-100).
         """
-
         # INVOKE <id> Load.GetLevel
         # -> R:INVOKE <id> <level (0-100)> Load.GetLevel
         response = await self.invoke(vid, "Load.GetLevel")
         level = float(response.args[1])
 
         return level
 
     async def set_level(self, vid: int, level: float) -> None:
         """Set the level of a load.
 
         Args:
             vid: The Vantage ID of the load.
             level: The level to set the load to (0-100).
         """
-
         # Clamp level to 0-100
         level = max(min(level, 100), 0)
 
         # INVOKE <id> Load.SetLevel <level (0-100)>
         # -> R:INVOKE <id> <rcode> Load.SetLevel <level (0-100)>
         await self.invoke(vid, "Load.SetLevel", level)
 
@@ -92,44 +88,40 @@
 
         Args:
             vid: The Vantage ID of the load.
             level: The level to ramp the load to (0-100).
             seconds: The number of seconds to ramp the load over.
             ramp_type: The type of ramp to perform.
         """
-
         # INVOKE <id> Load.Ramp <type> <seconds> <level>
         # -> R:INVOKE <id> <rcode> Load.Ramp <type> <seconds> <level>
         await self.invoke(vid, "Load.Ramp", ramp_type, seconds, level)
 
     @classmethod
     def parse_load_status(cls, args: Sequence[str]) -> float:
         """Parse a simple 'S:LOAD' event.
 
         Args:
             args: The arguments of the event.
 
         Returns:
             The level of the load.
         """
-
         # STATUS LOAD
         # -> S:LOAD <id> <level (0-100)>
         return float(args[0])
 
     @classmethod
     def parse_get_level_status(cls, args: Sequence[str]) -> float:
         """Parse a 'Load.GetLevel' event.
 
         Args:
             args: The arguments of the event.
 
         Returns:
             The level of the load.
         """
-
         # ELLOG STATUS ON
         # -> EL: <id> Load.GetLevel <level (0-100000)>
-
         # ADDSTATUS <id>
         # -> S:STATUS <id> Load.GetLevel <level (0-100000)>
         return float(args[0]) / 1000
```

### Comparing `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/object.py` & `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/object.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
         Args:
             vid: The Vantage ID of the object.
 
         Returns:
             The modification time of the object, as a datetime object.
         """
-
         # INVOKE <id> Object.GetMTime
         # -> R:INVOKE <id> <mtime> Object.GetMTime
         response = await self.invoke(vid, "Object.GetMTime")
         mtime = datetime.fromtimestamp(int(response.args[1]))
 
         return mtime
 
@@ -32,14 +31,12 @@
 
         Args:
             args: The arguments of the event.
 
         Returns:
             The modification time of the object, as a datetime object.
         """
-
         # ELLOG STATUS ON
         # -> EL: <id> Object.GetMTime <mtime>
-
         # STATUS ADD <id>
         # -> S:STATUS <id> Object.GetMTime <mtime>
         return datetime.fromtimestamp(int(args[0]))
```

### Comparing `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/rgb_load.py` & `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/rgb_load.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,55 +14,51 @@
 
         Args:
             vid: The Vantage ID of the RGB load.
 
         Returns:
             The value of the RGB color as a tuple of (red, green, blue).
         """
-
         return (await self.get_color(vid))[:3]
 
     async def get_rgbw(self, vid: int) -> Tuple[int, ...]:
         """Get the RGBW color of a load from the controller.
 
         Args:
             vid: The Vantage ID of the RGB load.
 
         Returns:
             The value of the RGBW color as a tuple of (red, green, blue, white).
         """
-
         return tuple(
             [await self.get_rgbw_channel(vid, channel) for channel in range(4)]
         )
 
     async def get_hsl(self, vid: int) -> Tuple[int, ...]:
         """Get the HSL color of a load from the controller.
 
         Args:
             vid: The Vantage ID of the RGB load.
 
         Returns:
             The value of the HSL color as a tuple of (hue, saturation, lightness).
         """
-
         return tuple(
             [await self.get_hsl_attribute(vid, attribute) for attribute in range(3)]
         )
 
     async def get_color(self, vid: int) -> Tuple[int, ...]:
         """Get the RGB/RGBW color of a load from the controller.
 
         Args:
             vid: The Vantage ID of the RGB load.
 
         Returns:
             The value of the RGB/RGBW color as a bytearray.
         """
-
         # INVOKE <id> RGBLoad.GetColor
         # -> R:INVOKE <id> <color> RGBLoad.GetColor
         response = await self.invoke(vid, "RGBLoad.GetColor")
         color = int(response.args[1])
 
         return tuple(struct.pack(">i", color))
 
@@ -72,15 +68,14 @@
         Args:
             vid: The Vantage ID of the RGB load.
             channel: The channel to get the color of.
 
         Returns:
             The value of the RGB channel, 0-255.
         """
-
         # INVOKE <id> RGBLoad.GetRGB <channel>
         # -> R:INVOKE <id> <value> RGBLoad.GetRGB <channel>
         response = await self.invoke(vid, "RGBLoad.GetRGB", channel)
         color = int(response.args[1])
 
         return color
 
@@ -90,15 +85,14 @@
         Args:
             vid: The Vantage ID of the RGB load.
             channel: The channel to get the color of.
 
         Returns:
             The value of the RGBW channel, 0-255.
         """
-
         # INVOKE <id> RGBLoad.GetRGB <channel>
         # -> R:INVOKE <id> <value> RGBLoad.GetRGB <channel>
         response = await self.invoke(vid, "RGBLoad.GetRGBW", channel)
         color = int(response.args[1])
 
         return color
 
@@ -109,15 +103,14 @@
             vid: The Vantage ID of the RGB load.
             attribute: The attribute to get the value of.
 
         Returns:
             The value of the HSL attribute, 0-360 for hue, 0-100 for saturation and
             lightness.
         """
-
         # INVOKE <id> RGBLoad.GetHSL <channel>
         # -> R:INVOKE <id> <value> RGBLoad.GetHSL <channel>
         response = await self.invoke(vid, "RGBLoad.GetHSL", attribute)
         color = int(response.args[1])
 
         return color
 
@@ -126,15 +119,14 @@
 
         Args:
             vid: The Vantage ID of the RGB load.
             red: The red value of the color, (0-255)
             green: The green value of the color, (0-255)
             blue: The blue value of the color, (0-255)
         """
-
         # Clamp levels to 0-255, ensure they're integers
         red = int(max(min(red, 255), 0))
         green = int(max(min(green, 255), 0))
         blue = int(max(min(blue, 255), 0))
 
         # INVOKE <id> RGBLoad.SetRGB <red> <green> <blue>
         # -> R:INVOKE <id> <rcode> RGBLoad.SetRGB <red> <green> <blue>
@@ -148,15 +140,14 @@
         Args:
             vid: The Vantage ID of the RGB load.
             red: The red value of the color, (0-255)
             green: The green value of the color, (0-255)
             blue: The blue value of the color, (0-255)
             white: The white value of the color, (0-255)
         """
-
         # Clamp levels to 0-255
         red = int(max(min(red, 255), 0))
         green = int(max(min(green, 255), 0))
         blue = int(max(min(blue, 255), 0))
         white = int(max(min(white, 255), 0))
 
         # INVOKE <id> RGBLoad.SetRGBW <red> <green> <blue> <white>
@@ -170,15 +161,14 @@
 
         Args:
             vid: The Vantage ID of the RGB load.
             hue: The hue value of the color, in degrees (0-360).
             saturation: The saturation value of the color, in percent (0-100).
             lightness: The lightness value of the color, in percent (0-100).
         """
-
         # Clamp levels to 0-360, 0-100, ensure they're integers
         hue = int(max(min(hue, 360), 0))
         saturation = int(max(min(saturation, 100), 0))
         lightness = int(max(min(lightness, 100), 0))
 
         # INVOKE <id> RGBLoad.SetHSL <hue> <saturation> <lightness>
         # -> R:INVOKE <id> <rcode> RGBLoad.SetHSL <hue> <saturation> <lightness>
@@ -192,34 +182,31 @@
         Args:
             vid: The Vantage ID of the RGB load.
             red: The new red value of the color, (0-255)
             green: The new green value of the color, (0-255)
             blue: The new blue value of the color, (0-255)
             seconds: The number of seconds the transition should take.
         """
-
         # Clamp levels to 0-255, ensure they're integers
         red = int(max(min(red, 255), 0))
         green = int(max(min(green, 255), 0))
         blue = int(max(min(blue, 255), 0))
 
         # INVOKE <id> RGBLoad.DissolveRGB <red> <green> <blue>
         # -> R:INVOKE <id> <rcode> RGBLoad.DissolveRGB <red> <green> <blue>
         await self.invoke(vid, "RGBLoad.DissolveRGB", red, green, blue, seconds)
 
     async def set_rgb_component(self, vid: int, channel: int, value: float) -> None:
-        """
-        Set a single RGB(W) color channel of a load.
+        """Set a single RGB(W) color channel of a load.
 
         Args:
             vid: The Vantage ID of the RGB load.
             channel: The channel to set the color of.
             value: The value to set the channel to, 0-255.
         """
-
         # Clamp levels to 0-255, ensure they're integers
         value = int(max(min(value, 255), 0))
 
         # INVOKE <id> RGBLoad.SetRGBComponent <channel> <value>
         # -> R:INVOKE <id> <rcode> RGBLoad.SetRGBComponent <channel> <value>
         await self.invoke(vid, "RGBLoad.SetRGBComponent", channel, value)
 
@@ -231,45 +218,40 @@
         Args:
             vid: The Vantage ID of the RGB load.
             hue: The new hue value of the color, in degrees (0-360).
             saturation: The new saturation value of the color, in percent (0-100).
             lightness: The new lightness value of the color, in percent (0-100).
             seconds: The number of seconds the transition should take.
         """
-
         # Clamp levels to 0-360, 0-100, ensure they're integers
         hue = int(max(min(hue, 360), 0))
         saturation = int(max(min(saturation, 100), 0))
         lightness = int(max(min(lightness, 100), 0))
 
         # INVOKE <id> RGBLoad.DissolveHSL <hue> <saturation> <lightness>
         # -> R:INVOKE <id> <rcode> RGBLoad.DissolveHSL <hue> <saturation> <lightness>
         await self.invoke(
             vid, "RGBLoad.DissolveHSL", hue, saturation, lightness, seconds
         )
 
     @classmethod
     def parse_color_channel_status(cls, args: Sequence[str]) -> Tuple[int, int]:
         """Parse an 'RGBLoad.GetRGB' event."""
-
         # ELLOG STATUSEX ON
         # -> EL: <id> RGBLoad.GetRGB <value> <channel>
-
         # STATUS ADD <id>
         # -> S:STATUS <id> RGBLoad.GetRGB <value> <channel>
         value = int(args[0])
         channel = int(args[1])
 
         return channel, value
 
     @classmethod
     def parse_get_color_status(cls, args: Sequence[str]) -> bytearray:
         """Parse an 'RGBLoad.GetColor' event."""
-
         # ELLOG STATUS ON
         # -> EL: <id> RGBLoad.GetColor <color>
-
         # STATUS ADD <id>
         # -> S:STATUS <id> RGBLoad.GetColor <color>
         color = int(args[0])
 
         return bytearray(struct.pack(">i", color))
```

### Comparing `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/sensor.py` & `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/sensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
     async def get_level(self, vid: int) -> int:
         """Get the level of a sensor.
 
         Args:
             vid: The Vantage ID of the sensor.
         """
-
         # INVOKE <id> Sensor.GetLevel
         # -> R:INVOKE <id> <level (0-100)> Sensor.GetLevel
         response = await self.invoke(vid, "Sensor.GetLevel")
         level = int(response.args[1])
 
         return level
 
@@ -28,14 +27,12 @@
 
         Args:
             args: The arguments of the event.
 
         Returns:
             The level of the sensor.
         """
-
         # ELLOG STATUS ON
         # -> EL: <id> Sensor.GetLevel <level>
-
         # STATUS ADD <id>
         # -> S:STATUS <id> Sensor.GetLevel <level>
         return int(args[0])
```

### Comparing `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/sounder.py` & `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/sounder.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,66 +8,62 @@
 
     async def turn_on(self, vid: int) -> None:
         """Turn on the keypad speaker.
 
         Args:
             vid: The Vantage ID of the keypad.
         """
-
         # INVOKE <id> Sounder.TurnOn
         # -> R:INVOKE <id> <rcode> Sounder.SetStatus
         await self.invoke(vid, "Sounder.SetStatus", "On")
 
     async def turn_off(self, vid: int) -> None:
         """Turn off the keypad speaker.
 
         Args:
             vid: The Vantage ID of the keypad.
         """
-
         # INVOKE <id> Sounder.TurnOff
         # -> R:INVOKE <id> <rcode> Sounder.SetStatus
         await self.invoke(vid, "Sounder.SetStatus", "Off")
 
     async def get_frequency(self, vid: int) -> float:
         """Get the frequency of the keypad speaker.
 
         Args:
             vid: The Vantage ID of the keypad.
 
         Returns:
             The frequency of the keypad speaker.
         """
-
         # INVOKE <id> Sounder.GetFrequency
         # -> R:INVOKE <id> <frequency> Sounder.GetFrequency
         response = await self.invoke(vid, "Sounder.GetFrequency")
         frequency = float(response.args[0])
 
         return frequency
 
     async def set_frequency(self, vid: int, frequency: float) -> None:
         """Set the frequency of the keypad speaker.
 
         Args:
             vid: The Vantage ID of the keypad.
             frequency: The frequency to set.
         """
-
         # INVOKE <id> Sounder.SetFrequency <frequency>
         # -> R:INVOKE <id> <rcode> Sounder.SetFrequency
         await self.invoke(vid, "Sounder.SetFrequency", frequency)
 
     async def play_fx(
         self, vid: int, fx: int, duration: float = 0, volume: float = 0
     ) -> None:
         """Play an FX on the keypad speaker.
 
         Args:
+            vid: The Vantage ID of the keypad.
             fx: The FX to play.
             duration: The duration to play the FX for, in seconds, 0 for default.
             volume: The volume to play the FX at, as a percentage, 0 for default.
         """
-
         # INVOKE <id> Sounder.PlayFX <fx> <duration> <volume>
         # -> R:INVOKE <id> <rcode> Sounder.PlayFX
         await self.invoke(vid, "Sounder.PlayFX", fx, duration, volume)
```

### Comparing `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/task.py` & `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,101 +10,92 @@
 
     async def is_running(self, vid: int) -> bool:
         """Get the running state of a task.
 
         Args:
             vid: The Vantage ID of the task.
         """
-
         # INVOKE <id> Task.IsRunning
         # -> R:INVOKE <id> <running (0/1)> Task.IsRunning
         response = await self.invoke(vid, "Task.IsRunning")
         is_running = bool(int(response.args[1]))
 
         return is_running
 
     async def get_state(self, vid: int) -> bool:
         """Get the state of a task.
 
         Args:
             vid: The Vantage ID of the task.
         """
-
         # INVOKE <id> Task.GetState
         # -> R:INVOKE <id> <state (0/1)> Task.GetState
         response = await self.invoke(vid, "Task.GetState")
         task_state = bool(int(response.args[1]))
 
         return task_state
 
     async def start(self, vid: int) -> None:
         """Start a task.
 
         Args:
             vid: The Vantage ID of the task.
         """
-
         # INVOKE <id> Task.Start <source> <event> <param1> <param2>
         # -> R:INVOKE <id> <rcode (0/1)> Task.Start <source> <event> <param1> <param2>
         await self.invoke(vid, "Task.Start")
 
     async def stop(self, vid: int) -> None:
         """Stop a running task.
 
         Args:
             vid: The Vantage ID of the task.
         """
-
         # INVOKE <id> Task.Stop
         # -> R:INVOKE <id> <rcode> Task.Stop
         await self.invoke(vid, "Task.Stop")
 
     @classmethod
     def parse_task_status(cls, args: Sequence[str]) -> bool:
         """Parse a simple 'S:TASK' event.
 
         Args:
             args: The arguments of the event.
 
         Returns:
             The state of the task.
         """
-
         # STATUS TASK
         # -> S:TASK <id> <state (0/1)>
         return bool(int(args[0]))
 
     @classmethod
     def parse_get_state_status(cls, args: Sequence[str]) -> bool:
         """Parse a 'Task.GetState' event.
 
         Args:
             args: The arguments of the event.
 
         Returns:
             The state of the task.
         """
-
         # ELLOG STATUS ON
         # -> EL: <id> Task.GetState <state (0/1)>
-
         # STATUS ADD <id>
         # -> S:STATUS <id> Task.GetState <state (0/1)>
         return bool(int(args[0]))
 
     @classmethod
     def parse_is_running_status(cls, args: Sequence[str]) -> bool:
         """Parse a 'Task.IsRunning' event.
 
         Args:
             args: The arguments of the event.
 
         Returns:
             The running state of the task.
         """
-
         # ELLOG STATUS ON
         # -> EL: <id> Task.IsRunning <running (0/1)>
-
         # STATUS ADD <id>
         # -> S:STATUS <id> Task.IsRunning <running (0/1)>
         return bool(int(args[0]))
```

### Comparing `aiovantage-0.4.0/src/aiovantage/command_client/interfaces/temperature.py` & `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/temperature.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
     async def get_value(self, vid: int) -> Decimal:
         """Get the value of a temperature sensor.
 
         Args:
             vid: The Vantage ID of the temperature sensor.
         """
-
         # INVOKE <id> Temperature.GetValue
         # -> R:INVOKE <id> <temp> Temperature.GetValue
         response = await self.invoke(vid, "Temperature.GetValue")
         level = Decimal(response.args[1])
 
         return level
 
@@ -29,14 +28,12 @@
 
         Args:
             args: The arguments of the event.
 
         Returns:
             The level of the sensor.
         """
-
         # ELLOG STATUS ON
         # -> EL: <id> Temperature.GetValue <temp>
-
         # STATUS ADD <id>
         # -> S:STATUS <id> Temperature.GetValue <temp>
         return Decimal(args[0]) / 1000
```

### Comparing `aiovantage-0.4.0/src/aiovantage/config_client/README.md` & `aiovantage-0.5.0/src/aiovantage/config_client/README.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/src/aiovantage/config_client/__init__.py` & `aiovantage-0.5.0/src/aiovantage/config_client/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,17 +26,18 @@
 from xsdata.formats.dataclass.parsers import XmlParser
 from xsdata.formats.dataclass.parsers.config import ParserConfig
 from xsdata.formats.dataclass.parsers.handlers import XmlEventHandler
 from xsdata.formats.dataclass.serializers import XmlSerializer
 from xsdata.formats.dataclass.serializers.config import SerializerConfig
 
 from aiovantage.config_client.methods import Call, Method, Return
+from aiovantage.config_client.methods.introspection import GetVersion
 from aiovantage.config_client.methods.login import Login
 from aiovantage.connection import BaseConnection
-from aiovantage.errors import LoginFailedError
+from aiovantage.errors import ClientResponseError, LoginFailedError, LoginRequiredError
 
 
 class ConfigConnection(BaseConnection):
     """Connection to a Vantage ACI server."""
 
     default_port = 2001
     default_ssl_port = 2010
@@ -99,75 +100,99 @@
         self._connection.close()
 
     async def request(
         self,
         method_cls: Type[Method[Call, Return]],
         params: Optional[Call] = None,
         connection: Optional[ConfigConnection] = None,
-    ) -> Return:
+    ) -> Optional[Return]:
         """Marshall a request, send it to the ACI service, and return a parsed object.
 
         Args:
             method_cls: The request method class to use.
             params: The parameters to pass to the method.
             connection: The connection to use, if not the default.
 
         Returns:
             The parsed response object
         """
-
         # Open the connection if it's closed
         conn = connection or await self.get_connection()
 
         # Build the method object
         method = method_cls()
         method.call = params
-        method_name = f"{method_cls.interface}.{method_cls.__name__}"
 
         # Render the method object to XML with xsdata
-        request = self._serializer.render(method)
-        self._logger.debug(request)
+        request = (
+            f"<{method.interface}>"
+            + self._serializer.render(method)
+            + f"</{method.interface}>"
+        )
+        self._logger.debug("Sending request: %s", request)
 
         # Send the request and read the response
         async with self._request_lock:
-            await conn.write(f"<{method.interface}>{request}</{method.interface}>")
+            await conn.write(request)
             response = await conn.readuntil(
-                f"</{method.interface}>".encode(), timeout=self._read_timeout
+                f"</{method.interface}>\n".encode(), timeout=self._read_timeout
             )
-        self._logger.debug(response)
+        self._logger.debug("Received response: %s", response)
 
-        # Parse the XML doc and extract the method element
-        tree = ElementTree.fromstring(response)
-        method_el = tree.find(f"{method_cls.__name__}")
-        if method_el is None:
-            raise ValueError(f"<{method_cls.__name__}> element missing from response")
-
-        # Validate there is a non-empty return value
-        return_el = method_el.find("return")
-        if return_el is None:
-            raise ValueError(f"{method_name} response did not contain a return value")
+        # Parse the XML doc
+        root = ElementTree.fromstring(response)
+
+        # Response root must match the tag of the request
+        if root.tag != method.interface:
+            raise ClientResponseError(
+                f"Response '{root.tag}' does not match request '{method.interface}'"
+            )
+
+        # Responses must contain the method element and a return element
+        method_el = root.find(f"./{method_cls.__name__}")
+        return_el = root.find(f"./{method_cls.__name__}/return")
+        if method_el is None or return_el is None:
+            raise ClientResponseError("Response is missing method or return element")
+
+        # Return None if the method has empty return element.
+        # This can happen when the client is not logged in, or when the method returns
+        # no results, eg. IConfiguration.GetFilterResults.
+        if return_el.text is None and len(return_el) == 0:
+            return None
 
         # Parse the method element with xsdata
         method = self._parser.parse(method_el, method_cls)
         if method.return_value is None:
-            raise ValueError(f"{method_name} response did not contain a return value")
+            return None
 
         return method.return_value
 
     async def get_connection(self) -> ConfigConnection:
         """Get a connection to the ACI service."""
         async with self._connection_lock:
             if self._connection.closed:
                 await self._connection.open()
 
-                # Log in if we have credentials
+                # Ensure the connection is authenticated, if required
                 if self._username is not None and self._password is not None:
+                    # Log in if we have credentials
                     success = await self.request(
                         Login,
                         Login.Params(self._username, self._password),
                         self._connection,
                     )
 
                     if not success:
                         raise LoginFailedError("Login failed, bad username or password")
+                else:
+                    # Check if login is required if we don't have credentials
+                    version = await self.request(
+                        GetVersion,
+                        connection=self._connection,
+                    )
+
+                    if version is None:
+                        raise LoginRequiredError(
+                            "Login required, but no credentials were provided"
+                        )
 
             return self._connection
```

### Comparing `aiovantage-0.4.0/src/aiovantage/config_client/helpers.py` & `aiovantage-0.5.0/src/aiovantage/config_client/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Helper functions for fetching system objects."""
 
+from contextlib import suppress
 from typing import Any, AsyncIterator, Optional, Sequence
 
 from aiovantage.config_client import ConfigClient
 from aiovantage.config_client.methods.configuration import (
     CloseFilter,
     GetFilterResults,
     GetObject,
     OpenFilter,
 )
+from aiovantage.errors import ClientError, ClientResponseError
 
 
 async def get_objects(
     client: ConfigClient,
     *,
     types: Optional[Sequence[str]] = None,
     xpath: Optional[str] = None,
@@ -23,65 +25,67 @@
         client: The ACI client instance
         types: An optional string, or list of strings of object types to fetch
         xpath: An optional xpath to filter the results by, eg. "/Load", "/*[@VID='12']"
 
     Yields:
         The objects of the specified types
     """
-
     # Support both a single object type and a list of status types
     if isinstance(types, str):
         types = [types]
     elif types is not None:
         types = list(types)
 
     # Open the filter
     handle = await client.request(
         OpenFilter, OpenFilter.Params(object_types=types, xpath=xpath)
     )
 
+    if handle is None:
+        raise ClientResponseError("Failed to open filter")
+
     try:
         # Get the results
         while True:
             response = await client.request(
                 GetFilterResults, GetFilterResults.Params(h_filter=handle)
             )
 
-            if not response.objects:
+            if not response:
                 break
 
-            for obj in response.objects:
+            for obj in response:
                 if obj.choice is None:
                     continue
 
                 yield obj.choice
     finally:
         # Close the filter
-        await client.request(CloseFilter, handle)
+        with suppress(ClientError):
+            await client.request(CloseFilter, handle)
 
 
 async def get_objects_by_id(
     client: ConfigClient, vids: Sequence[int]
 ) -> AsyncIterator[Any]:
     """Get all vantage system objects of the specified ids.
 
     Args:
         client: The ACI client instance
         vids: A list of Vantage IDs for object to fetch
 
     Yields:
         The objects of the specified ids
     """
-
     # Open the filter
     response = await client.request(GetObject, GetObject.Params(vids=list(vids)))
-    if not response.objects:
+    if not response:
         return
 
-    for obj in response.objects:
+    for obj in response:
         if obj.choice is None:
             continue
 
         yield obj.choice
 
 
 async def get_object_by_id(client: ConfigClient, vid: int) -> Any:
@@ -90,12 +94,11 @@
     Args:
         client: The ACI client instance
         vid: The Vantage ID of the object to fetch
 
     Returns:
         The object matching the specified id, or None if not found
     """
-
     try:
         return await get_objects_by_id(client, [vid]).__anext__()
     except StopAsyncIteration:
         return None
```

### Comparing `aiovantage-0.4.0/src/aiovantage/config_client/xml_dataclass.py` & `aiovantage-0.5.0/src/aiovantage/config_client/xml_dataclass.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,12 +32,11 @@
     metadata.update({"type": "Text"})
 
     return field(metadata=metadata, **kwargs)
 
 
 def xml_tag_from_class(cls: Type[Any]) -> str:
     """Get the XML tag name for a class."""
-
     meta = getattr(cls, "Meta", None)
     name = getattr(meta, "name", cls.__qualname__)
 
     return name
```

### Comparing `aiovantage-0.4.0/src/aiovantage/config_client/methods/types.py` & `aiovantage-0.5.0/src/aiovantage/config_client/methods/types.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ObjectChoice type definition."""
 
 import inspect
 from dataclasses import dataclass, field
 from typing import Optional
 
 import aiovantage.config_client.objects
-from aiovantage.config_client.xml_dataclass import xml_attribute, xml_tag_from_class
+from aiovantage.config_client.xml_dataclass import xml_tag_from_class
 
 # Get all Vantage object from aiovantage.config_client.objects
 ALL_OBJECT_TYPES = [
     item
     for _, item in inspect.getmembers(aiovantage.config_client.objects, inspect.isclass)
 ]
 
@@ -17,15 +17,17 @@
 @dataclass
 class ObjectChoice:
     """ObjectChoice type definition.
 
     Wildcard type that can be used to represent any object type.
     """
 
-    id: Optional[int] = xml_attribute("VID", default=None)
+    id: Optional[int] = field(
+        default=None, metadata={"name": "VID", "type": "Attribute"}
+    )
     choice: Optional[object] = field(
         default=None,
         metadata={
             "type": "Wildcard",
             "choices": [
                 {
                     "name": xml_tag_from_class(cls),
```

### Comparing `aiovantage-0.4.0/src/aiovantage/config_client/methods/configuration/get_object.py` & `aiovantage-0.5.0/src/aiovantage/config_client/methods/configuration/get_object.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 """IConfiguration.GetObject method definition."""
 
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import ClassVar, List, Optional
 
 from aiovantage.config_client.methods.types import ObjectChoice
-from aiovantage.config_client.xml_dataclass import xml_element
 
 
 @dataclass
 class GetObject:
     """IConfiguration.GetObject method definition."""
 
     interface: ClassVar[str] = "IConfiguration"
-    call: Optional["GetObject.Params"] = xml_element("call", default=None)
-    return_value: Optional["GetObject.Return"] = xml_element("return", default=None)
+    call: Optional["GetObject.Params"] = field(default=None)
+    return_value: Optional[List[ObjectChoice]] = field(
+        default=None, metadata={"name": "Object", "wrapper": "return"}
+    )
 
     @dataclass
     class Params:
         """IConfiguration.GetObject method parameters."""
 
-        vids: List[int] = xml_element("VID")
-
-    @dataclass
-    class Return:
-        """IConfiguration.GetObject method return value."""
-
-        objects: List[ObjectChoice] = xml_element("Object", default_factory=list)
+        vids: List[int] = field(metadata={"name": "VID"})
```

### Comparing `aiovantage-0.4.0/src/aiovantage/config_client/objects/__init__.py` & `aiovantage-0.5.0/src/aiovantage/config_client/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/src/aiovantage/config_client/objects/blind.py` & `aiovantage-0.5.0/src/aiovantage/config_client/objects/blind.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,9 +14,9 @@
     """Blind object."""
 
     parent_id: Optional[int] = xml_element("Parent", default=None)
     orientation: Optional[str] = xml_attribute("ShadeOrientation", default=None)
     type: Optional[str] = xml_attribute("ShadeType", default=None)
 
     def __post_init__(self) -> None:
-        """Post init."""
+        """Declare state attributes in post init."""
         self.position: Optional[Decimal] = None
```

### Comparing `aiovantage-0.4.0/src/aiovantage/config_client/objects/button.py` & `aiovantage-0.5.0/src/aiovantage/config_client/objects/button.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,9 +27,9 @@
                 self.up_task_id,
                 self.down_task_id,
                 self.hold_task_id,
             )
         )
 
     def __post_init__(self) -> None:
-        """Post init."""
+        """Declare state attributes in post init."""
         self.pressed: bool = False
```

### Comparing `aiovantage-0.4.0/src/aiovantage/config_client/objects/gmem.py` & `aiovantage-0.5.0/src/aiovantage/config_client/objects/gmem.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         fixed: bool = xml_attribute("Fixed", default=False)
 
     data: Data = xml_element("data")
     persistent: bool = xml_element("Persistent")
     tag: Tag = xml_element("Tag")
 
     def __post_init__(self) -> None:
-        """Post init."""
+        """Declare state attributes in post init."""
         self.value: Union[int, str, bool, None] = None
 
     @property
     def is_bool(self) -> bool:
         """Return True if GMem is boolean type."""
         return self.tag.type == "bool"
```

### Comparing `aiovantage-0.4.0/src/aiovantage/config_client/objects/load.py` & `aiovantage-0.5.0/src/aiovantage/config_client/objects/load.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class Load(LocationObject):
     """Load object."""
 
     load_type: str = xml_element("LoadType")
     power_profile_id: int = xml_element("PowerProfile")
 
     def __post_init__(self) -> None:
-        """Post init."""
+        """Declare state attributes in post init."""
         self.level: Optional[float] = None
 
     @property
     def is_relay(self) -> bool:
         """Return True if the load is a relay."""
         return self.load_type in (
             "High Voltage Relay",
```

### Comparing `aiovantage-0.4.0/src/aiovantage/config_client/objects/omni_sensor.py` & `aiovantage-0.5.0/src/aiovantage/config_client/objects/omni_sensor.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         method: str = xml_element("Method")
         method_hw: str = xml_element("MethodHW")
 
     get: GetMethodType = xml_element("Get")
     parent_id: int = xml_element("Parent")
 
     def __post_init__(self) -> None:
-        """Post init."""
+        """Declare state attributes in post init."""
         self.level: Union[int, Decimal, None] = None
 
     @property
     def is_current_sensor(self) -> bool:
         """Return True if the sensor is a current sensor."""
         return self.model == "Current"
```

### Comparing `aiovantage-0.4.0/src/aiovantage/config_client/objects/rgb_load.py` & `aiovantage-0.5.0/src/aiovantage/config_client/objects/rgb_load.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,16 +42,15 @@
         COLOR_CHANNEL = "Color Channel"
 
     color_type: ColorType = xml_element("ColorType")
     min_temp: int = xml_element("MinTemp")
     max_temp: int = xml_element("MaxTemp")
 
     def __post_init__(self) -> None:
-        """Post init."""
-
+        """Declare state attributes in post init."""
         self.hsl: Optional[Tuple[int, int, int]] = None
         self.rgb: Optional[Tuple[int, int, int]] = None
         self.rgbw: Optional[Tuple[int, int, int, int]] = None
         self.level: Optional[int] = None
         self.color_temp: Optional[int] = None
 
     @property
```

### Comparing `aiovantage-0.4.0/src/aiovantage/config_client/objects/system_object.py` & `aiovantage-0.5.0/src/aiovantage/config_client/objects/system_object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/src/aiovantage/controllers/anemo_sensors.py` & `aiovantage-0.5.0/src/aiovantage/controllers/tasks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,43 @@
-"""Controller holding and managing Vantage anemo (wind) sensors."""
+"""Controller holding and managing Vantage tasks."""
 
-from typing import Any, Dict, Sequence
+from typing import Sequence
 
 from typing_extensions import override
 
-from aiovantage.command_client.interfaces import AnemoSensorInterface
-from aiovantage.config_client.objects import AnemoSensor
+from aiovantage.command_client.interfaces import TaskInterface
+from aiovantage.config_client.objects import Task
 
-from .base import StatefulController
+from .base import BaseController, State
 
 
-class AnemoSensorsController(StatefulController[AnemoSensor], AnemoSensorInterface):
-    """Controller holding and managing Vantage anemo (wind) sensors."""
+class TasksController(BaseController[Task], TaskInterface):
+    """Controller holding and managing Vantage tasks."""
 
-    # Fetch the following object types from Vantage
-    vantage_types = ("AnemoSensor",)
+    vantage_types = ("Task",)
+    """The Vantage object types that this controller will fetch."""
 
-    # Subscribe to status updates from the Enhanced Log for the following methods
-    enhanced_log_status = True
-    enhanced_log_status_methods = ("AnemoSensor.GetSpeed",)
+    enhanced_log_status_methods = ("Task.IsRunning", "Task.GetState")
+    """Which status methods this controller handles from the Enhanced Log."""
 
     @override
-    async def fetch_object_state(self, vid: int) -> None:
-        """Fetch the initial state of an anemo sensor."""
-
-        state: Dict[str, Any] = {
-            "speed": await AnemoSensorInterface.get_speed(self, vid),
+    async def fetch_object_state(self, vid: int) -> State:
+        """Fetch the state properties of a task."""
+        return {
+            "is_running": await TaskInterface.is_running(self, vid),
+            "state": await TaskInterface.get_state(self, vid),
         }
 
-        self.update_state(vid, state)
-
     @override
-    def handle_object_update(self, vid: int, status: str, args: Sequence[str]) -> None:
-        """Handle state changes for an anemo sensor."""
-
-        state: Dict[str, Any] = {}
-        if status == "AnemoSensor.GetSpeed":
-            state["speed"] = AnemoSensorInterface.parse_get_speed_status(args)
+    def parse_object_update(self, _vid: int, status: str, args: Sequence[str]) -> State:
+        """Handle state changes for a task."""
+        if status == "Task.IsRunning":
+            return {
+                "is_running": TaskInterface.parse_is_running_status(args),
+            }
+
+        if status == "Task.GetState":
+            return {
+                "state": TaskInterface.parse_get_state_status(args),
+            }
 
-        self.update_state(vid, state)
+        return None
```

### Comparing `aiovantage-0.4.0/src/aiovantage/controllers/base.py` & `aiovantage-0.5.0/src/aiovantage/controllers/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Base controller for Vantage objects."""
 
 import asyncio
 import logging
-from abc import abstractmethod
+from dataclasses import fields
 from inspect import iscoroutinefunction
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterable,
     List,
+    Literal,
     Optional,
     Sequence,
     Tuple,
     TypeVar,
     Union,
-    cast,
 )
 
 from aiovantage.command_client import CommandClient, Event, EventStream, EventType
 from aiovantage.command_client.utils import tokenize_response
 from aiovantage.config_client import ConfigClient
 from aiovantage.config_client.helpers import get_objects
 from aiovantage.config_client.objects import SystemObject
@@ -33,36 +33,46 @@
 T = TypeVar("T", bound=SystemObject)
 
 
 # Types for callbacks for event subscriptions
 EventCallback = Callable[[VantageEvent, T, Dict[str, Any]], None]
 EventSubscription = Tuple[EventCallback[T], Optional[Iterable[VantageEvent]]]
 
+# Type for state updates
+State = Optional[Dict[str, Any]]
+
 
 class BaseController(QuerySet[T]):
     """Base controller for Vantage objects."""
 
     vantage_types: Tuple[str, ...]
     """The Vantage object types that this controller handles."""
 
+    status_types: Optional[Tuple[str, ...]] = None
+    """Which Vantage 'STATUS' types this controller handles, if any."""
+
+    enhanced_log_status_methods: Optional[Union[Tuple[str, ...], Literal["*"]]] = None
+    """Which status methods this controller handles from the Enhanced Log."""
+
     def __init__(self, vantage: "Vantage") -> None:
         """Initialize instance."""
         self._vantage = vantage
         self._items: Dict[int, T] = {}
         self._logger = logging.getLogger(__package__)
+        self._subscribed_to_event_stream = False
         self._subscriptions: List[EventSubscription[T]] = []
         self._id_subscriptions: Dict[int, List[EventSubscription[T]]] = {}
         self._initialized = False
 
-        QuerySet.__init__(self, self._items, self.initialize)
+        QuerySet.__init__(self, self._items, self._lazy_initialize)
 
         self.__post_init__()
 
     def __post_init__(self) -> None:
-        """Post initialization hook."""
+        """Post initialization hook for subclasses."""
 
     def __getitem__(self, vid: int) -> T:
         """Return the object with the given Vantage ID."""
         return self._items[vid]
 
     def __contains__(self, vid: int) -> bool:
         """Return True if the object with the given Vantage ID exists."""
@@ -79,32 +89,92 @@
         return self._vantage.command_client
 
     @property
     def event_stream(self) -> EventStream:
         """Return the event stream instance."""
         return self._vantage.event_stream
 
-    async def initialize(self) -> None:
-        """Initialize a stateless controller by populating the objects it manages."""
+    @property
+    def stateful(self) -> bool:
+        """Return True if this controller manages stateful objects."""
+        return bool(self.status_types or self.enhanced_log_status_methods)
+
+    async def fetch_object_state(self, _vid: int) -> State:
+        """Fetch the full state of an object, should be overridden by subclasses."""
+        return None
+
+    def parse_object_update(
+        self, _vid: int, _status: str, _args: Sequence[str]
+    ) -> State:
+        """Parse updates from the event stream for an object, should be overridden by subclasses."""
+        return None
+
+    async def initialize(self, fetch_state: bool = True) -> None:
+        """Populate objects and fetch their initial state."""
+        prev_ids = set(self._items.keys())
+        cur_ids = set()
 
-        if self._initialized:
-            return
+        # Fetch all objects managed by this controller
+        async for obj in get_objects(self.config_client, types=self.vantage_types):
+            if obj.id not in prev_ids:
+                # This is a new object, add it to the controller
+                self._items[obj.id] = obj
+
+                # Fetch the state of the object
+                if self.stateful and fetch_state:
+                    self._set_state(obj, await self.fetch_object_state(obj.id))
 
-        await self.fetch_objects()
+                # Notify subscribers that a new object was added
+                self.emit(VantageEvent.OBJECT_ADDED, obj)
+            else:
+                # This is an existing object, check if any attributes have changed
+                prev_obj = self._items[obj.id]
+                attrs_changed = [
+                    field.name
+                    for field in fields(prev_obj)
+                    if getattr(prev_obj, field.name) != getattr(obj, field.name)
+                    and field.name != "mtime"
+                ]
+
+                # If any attributes changed, update the object and notify subscribers
+                if attrs_changed:
+                    self._items[obj.id] = obj
+                    self.emit(
+                        VantageEvent.OBJECT_UPDATED,
+                        obj,
+                        {"attrs_changed": attrs_changed},
+                    )
+
+            # Keep track of which objects we've seen
+            cur_ids.add(obj.id)
+
+        # Handle objects that were removed
+        for vid in prev_ids - cur_ids:
+            obj = self._items.pop(vid)
+            self.emit(VantageEvent.OBJECT_REMOVED, obj)
+
+        # Subscribe to the event stream if this is the first subscription
+        if self.stateful and fetch_state and not self._subscribed_to_event_stream:
+            await self._subscribe_to_event_stream()
 
         self._initialized = True
+        self._logger.info("%s initialized", self.__class__.__name__)
 
-    async def fetch_objects(self) -> None:
-        """Fetch all objects managed by this controller."""
+    async def fetch_full_state(self, subscribe: bool = True) -> None:
+        """Fetch the full state of all objects managed by this controller."""
+        if not self.stateful:
+            return
 
-        async for obj in get_objects(self.config_client, types=self.vantage_types):
-            self._items[obj.id] = cast(T, obj)
-            self.emit(VantageEvent.OBJECT_ADDED, cast(T, obj))
+        for obj in self._items.values():
+            self._update_state(obj.id, await self.fetch_object_state(obj.id))
+
+        if subscribe and not self._subscribed_to_event_stream:
+            await self._subscribe_to_event_stream()
 
-        self._logger.info("%s fetched objects", self.__class__.__name__)
+        self._logger.info("%s fetched state", self.__class__.__name__)
 
     def subscribe(
         self,
         callback: EventCallback[T],
         id_filter: Union[int, Tuple[int], None] = None,
         event_filter: Union[VantageEvent, Tuple[VantageEvent], None] = None,
     ) -> Callable[[], None]:
@@ -114,20 +184,18 @@
             callback: The callback to call when an object changes.
             id_filter: The Vantage IDs to subscribe to, all objects if None.
             event_filter: The event types to subscribe to, all events if None.
 
         Returns:
             A function to unsubscribe from the callback.
         """
-
-        # Handle single ID filter
+        # Handle single ID filter or single event filter
         if isinstance(id_filter, int):
             id_filter = (id_filter,)
 
-        # Handle single event filter
         if isinstance(event_filter, VantageEvent):
             event_filter = (event_filter,)
 
         # Create the subscription
         subscription = (callback, event_filter)
 
         # Add the subscription to the list of subscriptions
@@ -148,121 +216,55 @@
                     if vid not in self._id_subscriptions:
                         continue
                     self._id_subscriptions[vid].remove(subscription)
 
         return unsubscribe
 
     def emit(
-        self,
-        event_type: VantageEvent,
-        obj: T,
-        data: Optional[Dict[str, Any]] = None,
+        self, event_type: VantageEvent, obj: T, data: Optional[Dict[str, Any]] = None
     ) -> None:
         """Emit an event to subscribers of this controller.
 
         Args:
             event_type: The type of event to emit.
             obj: The object that the event relates to.
             data: Data to pass to the callback.
         """
-
         if data is None:
             data = {}
 
         # Grab a list of subscribers that care about this object
         subscribers = self._subscriptions + self._id_subscriptions.get(obj.id, [])
         for callback, event_filter in subscribers:
             if event_filter is not None and event_type not in event_filter:
                 continue
 
             if iscoroutinefunction(callback):
                 asyncio.create_task(callback(event_type, obj, data))  # noqa: RUF006
             else:
                 callback(event_type, obj, data)
 
-
-class StatefulController(BaseController[T]):
-    """Base controller for Vantage objects that have state."""
-
-    status_types: Optional[Tuple[str, ...]] = None
-    """Which Vantage status types this controller handles, if any."""
-
-    enhanced_log_status: bool = False
-    """Should this controller subscribe to updates from the Enhanced Log."""
-
-    enhanced_log_status_methods: Optional[Tuple[str, ...]] = None
-    """Which status methods this controller handles from the Enhanced Log."""
-
-    @abstractmethod
-    async def fetch_object_state(self, vid: int) -> None:
-        """Fetch the initial state of an object."""
-
-    @abstractmethod
-    def handle_object_update(self, vid: int, status: str, args: Sequence[str]) -> None:
-        """Handle state changes for an object."""
-
-    async def initialize(self) -> None:
-        """Initialize a stateful controller.
-
-        Populates the objects it manages, fetches their initial state, and subscribes
-        to state updates.
-        """
-
-        if self._initialized:
+    def _set_state(self, obj: T, state: State) -> None:
+        # Set the state properties of an object.
+        if state is None:
             return
 
-        await self.fetch_objects()
-        await self.fetch_full_state()
-        await self.subscribe_to_updates()
-
-        self.event_stream.subscribe(self._handle_event, EventType.RECONNECTED)
-
-        self._initialized = True
-
-    async def fetch_full_state(self) -> None:
-        """Fetch the full state of all objects managed by this controller."""
-
-        await asyncio.gather(
-            *[self.fetch_object_state(obj.id) for obj in self._items.values()]
-        )
-
-        self._logger.info("%s fetched full state", self.__class__.__name__)
-
-    async def subscribe_to_updates(self) -> None:
-        """Subscribe to state updates for objects managed by this controller."""
+        for key, value in state.items():
+            try:
+                setattr(obj, key, value)
+            except AttributeError:
+                self._logger.warning("Object '%d' has no attribute '%s'", obj.id, key)
 
-        if not self._items:
+    def _update_state(self, vid: int, state: State) -> None:
+        """Update the state of an object and notify subscribers if it changed."""
+        if state is None:
             return
 
-        # Ensure that the event stream is running
-        await self.event_stream.start()
-
-        # Subscribe to "STATUS {type}" updates, if this controller cares about them
-        if self.status_types:
-            self.event_stream.subscribe_status(self._handle_event, self.status_types)
-
-        # Subscribe to object status events from the "Enhanced Log"
-        if self.enhanced_log_status:
-            self.event_stream.subscribe_enhanced_log(
-                self._handle_event, ("STATUS", "STATUSEX")
-            )
-
-        self._logger.info("%s subscribed to updates", self.__class__.__name__)
-
-    def update_state(self, vid: int, state: Dict[str, Any]) -> None:
-        """Update the state of an object and notify subscribers if it changed.
-
-        Args:
-            vid: The Vantage ID of the object to update.
-            state: A dictionary of attributes to update.
-        """
-
-        # Get the object, skip if it doesn't exist
-        obj = self.get(vid)
-        if obj is None:
+        # Ignore updates for objects that this controller doesn't manage
+        if (obj := self._items.get(vid)) is None:
             return
 
         # Check if any of the attributes changed and update them
         attrs_changed = []
         for key, value in state.items():
             try:
                 if getattr(obj, key) != value:
@@ -275,39 +277,72 @@
         if len(attrs_changed) > 0:
             self.emit(
                 VantageEvent.OBJECT_UPDATED,
                 obj,
                 {"attrs_changed": attrs_changed},
             )
 
+    async def _subscribe_to_event_stream(self) -> None:
+        # Ensure that the event stream is running
+        await self.event_stream.start()
+
+        # Re-fetch the full state of all objects after reconnecting
+        self.event_stream.subscribe(self._handle_event, EventType.RECONNECTED)
+
+        # Subscribe to "STATUS {type}" updates, if this controller cares about them
+        if self.status_types:
+            self.event_stream.subscribe_status(self._handle_event, self.status_types)
+
+        # Subscribe to object status events from the "Enhanced Log"
+        if self.enhanced_log_status_methods:
+            self.event_stream.subscribe_enhanced_log(
+                self._handle_event, ("STATUS", "STATUSEX")
+            )
+
+        self._subscribed_to_event_stream = True
+        self._logger.info("%s subscribed to event stream", self.__class__.__name__)
+
     async def _handle_event(self, event: Event) -> None:
         # Handle events from the event stream
+        # pylint: disable=assignment-from-none
+
         if event["type"] == EventType.STATUS:
             # Ignore events for objects that this controller doesn't manage
             if event["id"] not in self._items:
                 return
 
             # Pass the event to the controller
-            self.handle_object_update(event["id"], event["status_type"], event["args"])
+            state = self.parse_object_update(
+                event["id"], event["status_type"], event["args"]
+            )
+            self._update_state(event["id"], state)
 
         elif event["type"] == EventType.ENHANCED_LOG:
             # STATUS/STATUSEX logs can be tokenized the same as command responses
             id_str, method, *args = tokenize_response(event["log"])
 
             # Ignore events with methods that this controller doesn't care about
-            if (
+            if not (
                 self.enhanced_log_status_methods
-                and method not in self.enhanced_log_status_methods
+                and (
+                    self.enhanced_log_status_methods == "*"
+                    or method in self.enhanced_log_status_methods
+                )
             ):
                 return
 
             # Ignore events for objects that this controller doesn't manage
             vid = int(id_str)
             if vid not in self._items:
                 return
 
             # Pass the event to the controller
-            self.handle_object_update(vid, method, args)
+            state = self.parse_object_update(vid, method, args)
+            self._update_state(vid, state)
 
         elif event["type"] == EventType.RECONNECTED:
             # Fetch the full state of all objects after reconnecting
             await self.fetch_full_state()
+
+    async def _lazy_initialize(self) -> None:
+        if not self._initialized:
+            await self.initialize()
```

### Comparing `aiovantage-0.4.0/src/aiovantage/controllers/blind_groups.py` & `aiovantage-0.5.0/src/aiovantage/controllers/blind_groups.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,24 +6,23 @@
 
 from .base import BaseController
 
 
 class BlindGroupsController(BaseController[BlindGroup], BlindInterface):
     """Controller holding and managing Vantage blind groups."""
 
-    # Fetch the following object types from Vantage
     vantage_types = (
         "BlindGroup",
         "Somfy.RS-485_Group_CHILD",
         "Somfy.URTSI_2_Group_CHILD",
     )
+    """The Vantage object types that this controller will fetch."""
 
     def blinds(self, vid: int) -> QuerySet[Blind]:
         """Return a queryset of all blinds in this blind group."""
-
         blind_group = self[vid]
         if blind_group.blind_ids is not None:
             # Some blind groups have a list of blind ids, use that to filter
             return self._vantage.blinds.filter(
                 lambda blind: blind.id in blind_group.blind_ids  # type: ignore[operator]
             )
```

### Comparing `aiovantage-0.4.0/src/aiovantage/controllers/blinds.py` & `aiovantage-0.5.0/src/aiovantage/controllers/blinds.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 """Controller holding and managing Vantage blinds."""
 
-from typing import Any, Dict, Sequence
+from typing import Sequence
 
 from typing_extensions import override
 
 from aiovantage.command_client.interfaces import BlindInterface
 from aiovantage.config_client.objects import Blind
 
-from .base import StatefulController
+from .base import BaseController, State
 
 
-class BlindsController(StatefulController[Blind], BlindInterface):
+class BlindsController(BaseController[Blind], BlindInterface):
     """Controller holding and managing Vantage blinds."""
 
-    # Fetch the following object types from Vantage
     vantage_types = (
         "QISBlind",
         "QubeBlind",
         "RelayBlind",
         "Somfy.RS-485_Shade_CHILD",
         "Somfy.URTSI_2_Shade_CHILD",
     )
+    """The Vantage object types that this controller will fetch."""
 
-    # Subscribe to status updates from the Enhanced Log for the following methods
-    enhanced_log_status = True
     enhanced_log_status_methods = ("Blind.GetPosition",)
+    """Which status methods this controller handles from the Enhanced Log."""
 
     @override
-    async def fetch_object_state(self, vid: int) -> None:
-        """Fetch the initial state of a blind."""
-
-        state: Dict[str, Any] = {
-            "position": await BlindInterface.get_position(self, vid)
+    async def fetch_object_state(self, vid: int) -> State:
+        """Fetch the state properties of a blind."""
+        return {
+            "position": await BlindInterface.get_position(self, vid),
         }
 
-        self.update_state(vid, state)
-
     @override
-    def handle_object_update(self, vid: int, status: str, args: Sequence[str]) -> None:
+    def parse_object_update(self, _vid: int, status: str, args: Sequence[str]) -> State:
         """Handle state changes for a blind."""
+        if status != "Blind.GetPosition":
+            return None
 
-        state: Dict[str, Any] = {}
-        if status == "Blind.GetPosition":
-            state["position"] = BlindInterface.parse_get_position_status(args)
-
-        self.update_state(vid, state)
+        return {
+            "position": BlindInterface.parse_get_position_status(args),
+        }
```

### Comparing `aiovantage-0.4.0/src/aiovantage/controllers/buttons.py` & `aiovantage-0.5.0/src/aiovantage/controllers/anemo_sensors.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,37 @@
-"""Controller holding and managing Vantage buttons."""
+"""Controller holding and managing Vantage anemo (wind) sensors."""
 
-from typing import Any, Dict, Sequence
+from typing import Sequence
 
 from typing_extensions import override
 
-from aiovantage.command_client.interfaces import ButtonInterface
-from aiovantage.config_client.objects import Button
+from aiovantage.command_client.interfaces import AnemoSensorInterface
+from aiovantage.config_client.objects import AnemoSensor
 
-from .base import StatefulController
+from .base import BaseController, State
 
 
-class ButtonsController(StatefulController[Button], ButtonInterface):
-    """Controller holding and managing Vantage buttons."""
+class AnemoSensorsController(BaseController[AnemoSensor], AnemoSensorInterface):
+    """Controller holding and managing Vantage anemo (wind) sensors."""
 
-    # Fetch the following object types from Vantage
-    vantage_types = ("Button",)
+    vantage_types = ("AnemoSensor",)
+    """The Vantage object types that this controller will fetch."""
 
-    # Get status updates from "STATUS BTN"
-    status_types = ("BTN",)
+    enhanced_log_status_methods = ("AnemoSensor.GetSpeed",)
+    """Which status methods this controller handles from the Enhanced Log."""
 
     @override
-    async def fetch_object_state(self, vid: int) -> None:
-        """Fetch the initial state of a button."""
+    async def fetch_object_state(self, vid: int) -> State:
+        """Fetch the state properties of an anemo sensor."""
+        return {
+            "speed": await AnemoSensorInterface.get_speed(self, vid),
+        }
 
     @override
-    def handle_object_update(self, vid: int, status: str, args: Sequence[str]) -> None:
-        """Handle state changes for a button."""
-
-        state: Dict[str, Any] = {}
-        if status == "BTN":
-            state["pressed"] = ButtonInterface.parse_btn_status(args)
-
-        self.update_state(vid, state)
+    def parse_object_update(self, _vid: int, status: str, args: Sequence[str]) -> State:
+        """Handle state changes for an anemo sensor."""
+        if status != "AnemoSensor.GetSpeed":
+            return None
+
+        return {
+            "speed": AnemoSensorInterface.parse_get_speed_status(args),
+        }
```

### Comparing `aiovantage-0.4.0/src/aiovantage/controllers/light_sensors.py` & `aiovantage-0.5.0/src/aiovantage/controllers/light_sensors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 """Controller holding and managing Vantage light sensors."""
 
-from typing import Any, Dict, Sequence
+from typing import Sequence
 
 from typing_extensions import override
 
 from aiovantage.command_client.interfaces import LightSensorInterface
 from aiovantage.config_client.objects import LightSensor
 
-from .base import StatefulController
+from .base import BaseController, State
 
 
-class LightSensorsController(StatefulController[LightSensor], LightSensorInterface):
+class LightSensorsController(BaseController[LightSensor], LightSensorInterface):
     """Controller holding and managing Vantage light sensors."""
 
-    # Fetch the following object types from Vantage
     vantage_types = ("LightSensor",)
+    """The Vantage object types that this controller will fetch."""
 
-    # Subscribe to status updates from the Enhanced Log for the following methods
-    enhanced_log_status = True
     enhanced_log_status_methods = ("LightSensor.GetLevel",)
+    """Which status methods this controller handles from the Enhanced Log."""
 
     @override
-    async def fetch_object_state(self, vid: int) -> None:
-        """Fetch the initial state of a light sensor."""
-
-        state: Dict[str, Any] = {
+    async def fetch_object_state(self, vid: int) -> State:
+        """Fetch the state properties of a light sensor."""
+        return {
             "level": await LightSensorInterface.get_level(self, vid),
         }
 
-        self.update_state(vid, state)
-
     @override
-    def handle_object_update(self, vid: int, status: str, args: Sequence[str]) -> None:
+    def parse_object_update(self, _vid: int, status: str, args: Sequence[str]) -> State:
         """Handle state changes for a light sensor."""
+        if status != "LightSensor.GetLevel":
+            return None
 
-        state: Dict[str, Any] = {}
-        if status == "LightSensor.GetLevel":
-            state["level"] = LightSensorInterface.parse_get_level_status(args)
-
-        self.update_state(vid, state)
+        return {
+            "level": LightSensorInterface.parse_get_level_status(args),
+        }
```

### Comparing `aiovantage-0.4.0/src/aiovantage/controllers/loads.py` & `aiovantage-0.5.0/src/aiovantage/controllers/loads.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,71 +1,63 @@
 """Controller holding and managing Vantage loads."""
 
-from typing import Any, Dict, Sequence
+from typing import Sequence
 
 from typing_extensions import override
 
 from aiovantage.command_client.interfaces import LoadInterface
 from aiovantage.config_client.objects import Load
 from aiovantage.query import QuerySet
 
-from .base import StatefulController
+from .base import BaseController, State
 
 
-class LoadsController(StatefulController[Load], LoadInterface):
+class LoadsController(BaseController[Load], LoadInterface):
     """Controller holding and managing Vantage loads."""
 
-    # Fetch the following object types from Vantage
     vantage_types = ("Load",)
+    """The Vantage object types that this controller will fetch."""
 
-    # Get status updates from "STATUS LOAD"
     status_types = ("LOAD",)
+    """Which Vantage 'STATUS' types this controller handles, if any."""
 
     @override
-    async def fetch_object_state(self, vid: int) -> None:
-        """Fetch the initial state of a load."""
-
-        state: Dict[str, Any] = {
+    async def fetch_object_state(self, vid: int) -> State:
+        """Fetch the state properties of a load."""
+        return {
             "level": await LoadInterface.get_level(self, vid),
         }
 
-        self.update_state(vid, state)
-
     @override
-    def handle_object_update(self, vid: int, status: str, args: Sequence[str]) -> None:
+    def parse_object_update(self, _vid: int, status: str, args: Sequence[str]) -> State:
         """Handle state changes for a load."""
+        if status != "LOAD":
+            return None
 
-        state: Dict[str, Any] = {}
-        if status == "LOAD":
-            state["level"] = LoadInterface.parse_load_status(args)
-
-        self.update_state(vid, state)
+        return {
+            "level": LoadInterface.parse_load_status(args),
+        }
 
     @property
-    def on(self) -> QuerySet[Load]:
+    def is_on(self) -> QuerySet[Load]:
         """Return a queryset of all loads that are turned on."""
-
         return self.filter(lambda load: load.is_on)
 
     @property
-    def off(self) -> QuerySet[Load]:
+    def is_off(self) -> QuerySet[Load]:
         """Return a queryset of all loads that are turned off."""
-
         return self.filter(lambda load: not load.is_on)
 
     @property
     def relays(self) -> QuerySet[Load]:
         """Return a queryset of all loads that are relays."""
-
         return self.filter(lambda load: load.is_relay)
 
     @property
     def motors(self) -> QuerySet[Load]:
         """Return a queryset of all loads that are motors."""
-
         return self.filter(lambda load: load.is_motor)
 
     @property
     def lights(self) -> QuerySet[Load]:
         """Return a queryset of all loads that are lights."""
-
         return self.filter(lambda load: load.is_light)
```

### Comparing `aiovantage-0.4.0/src/aiovantage/controllers/omni_sensors.py` & `aiovantage-0.5.0/src/aiovantage/controllers/omni_sensors.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,93 +1,87 @@
 """Controller holding and managing Vantage omni sensors."""
 
 from decimal import Decimal
-from typing import Any, Dict, Sequence, Union
+from typing import Sequence, Union
 
 from typing_extensions import override
 
 from aiovantage.config_client.objects import OmniSensor
-from aiovantage.controllers.base import StatefulController
+from aiovantage.controllers.base import BaseController, State
 
 
-class OmniSensorsController(StatefulController[OmniSensor]):
+class OmniSensorsController(BaseController[OmniSensor]):
     """Controller holding and managing Vantage omni sensors."""
 
-    # Fetch the following object types from Vantage
     vantage_types = ("OmniSensor",)
+    """The Vantage object types that this controller will fetch."""
 
-    # Subscribe to status updates from the Enhanced Log
-    enhanced_log_status = True
+    enhanced_log_status_methods = "*"
+    """Which status methods this controller handles from the Enhanced Log."""
 
     @override
-    async def fetch_object_state(self, vid: int) -> None:
-        """Fetch the initial state of an omni sensor."""
-
-        state: Dict[str, Any] = {
+    async def fetch_object_state(self, vid: int) -> State:
+        """Fetch the state properties of an omni sensor."""
+        return {
             "level": await self.get_level(vid),
         }
 
-        self.update_state(vid, state)
-
     @override
-    def handle_object_update(self, vid: int, status: str, args: Sequence[str]) -> None:
+    def parse_object_update(self, vid: int, status: str, args: Sequence[str]) -> State:
         """Handle state changes for an omni sensor."""
-
-        omni_sensor: OmniSensor = self[vid]
+        omni_sensor = self[vid]
         if status != omni_sensor.get.method:
-            return
+            return None
 
-        state: Dict[str, Any] = {
+        return {
             "level": self.parse_get_level_status(omni_sensor, args),
         }
 
-        self.update_state(vid, state)
-
     async def get_level(self, vid: int, cached: bool = False) -> Union[int, Decimal]:
         """Get the level of an OmniSensor.
 
         Args:
             vid: The ID of the sensor.
             cached: Whether to use the cached value or fetch a new one.
 
         Returns:
             The level of the sensor.
         """
-
-        omni_sensor: OmniSensor = self[vid]
-
         # Figure out which get method to use, hardware or software (cached)
+        omni_sensor = self[vid]
         method = omni_sensor.get.method if cached else omni_sensor.get.method_hw
 
         # INVOKE <id> <method>
         # -> R:INVOKE <id> <value> <method>
         response = await self.command_client.command("INVOKE", vid, method)
 
         # Convert the level to the correct type
         if omni_sensor.get.formula.return_type == "fixed":
             level = Decimal(response.args[1])
-            if omni_sensor.get.formula.level_type == "fixed":
-                return level
-            else:
+            if omni_sensor.get.formula.level_type == "int":
                 return int(level)
-        else:
+
+            return level
+
+        if omni_sensor.get.formula.return_type == "int":
             level = Decimal(response.args[1]) / 1000
-            if omni_sensor.get.formula.level_type == "fixed":
-                return level
-            else:
+            if omni_sensor.get.formula.level_type == "int":
                 return int(level)
 
+            return level
+
+        raise ValueError(f"Unknown return type {omni_sensor.get.formula.return_type}")
+
     @classmethod
     def parse_get_level_status(
         cls, omni_sensor: OmniSensor, args: Sequence[str]
     ) -> Union[int, Decimal]:
         """Parse an OmniSensor 'GetLevel' event, eg. 'PowerSensor.GetPower'."""
-
         # ELLOG STATUS ON
         # -> EL: <id> <method> <value>
         # STATUS ADD <id>
         # -> S:STATUS <id> <method> <value>
         level = Decimal(args[0]) / 1000
-        if omni_sensor.get.formula.level_type == "fixed":
-            return level
-        else:
+        if omni_sensor.get.formula.level_type == "int":
             return int(level)
+
+        return level
```

### Comparing `aiovantage-0.4.0/src/aiovantage/controllers/rgb_loads.py` & `aiovantage-0.5.0/src/aiovantage/controllers/rgb_loads.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,46 +8,44 @@
     ColorTemperatureInterface,
     LoadInterface,
     RGBLoadInterface,
 )
 from aiovantage.config_client.objects import RGBLoad
 from aiovantage.query import QuerySet
 
-from .base import StatefulController
+from .base import BaseController, State
 
 
 class RGBLoadsController(
-    StatefulController[RGBLoad],
+    BaseController[RGBLoad],
     LoadInterface,
     RGBLoadInterface,
     ColorTemperatureInterface,
 ):
     """Controller holding and managing Vantage RGB loads."""
 
-    # Fetch the following object types from Vantage
     vantage_types = ("Vantage.DGColorLoad", "Vantage.DDGColorLoad")
+    """The Vantage object types that this controller will fetch."""
 
-    # Subscribe to status updates from the Enhanced Log for the following methods
-    enhanced_log_status = True
     enhanced_log_status_methods = (
         "RGBLoad.GetHSL",
         "RGBLoad.GetRGB",
         "RGBLoad.GetRGBW",
         "ColorTemperature.Get",
         "Load.GetLevel",
     )
+    """Which status methods this controller handles from the Enhanced Log."""
 
     def __post_init__(self) -> None:
-        """Post initialization hook."""
+        """Initialize the map for building colors."""
         self._temp_color_map: Dict[int, List[int]] = {}
 
     @override
-    async def fetch_object_state(self, vid: int) -> None:
-        """Fetch the initial state of an RGB load."""
-
+    async def fetch_object_state(self, vid: int) -> State:
+        """Fetch the state properties of an RGB load."""
         state: Dict[str, Any] = {
             "level": await LoadInterface.get_level(self, vid),
         }
 
         rgb_load: RGBLoad = self[vid]
         if rgb_load.is_rgb:
             state["hsl"] = await RGBLoadInterface.get_hsl(self, vid)
@@ -55,55 +53,58 @@
             state["rgbw"] = await RGBLoadInterface.get_rgbw(self, vid)
 
         if rgb_load.is_cct:
             state["color_temp"] = await ColorTemperatureInterface.get_color_temp(
                 self, vid
             )
 
-        self.update_state(vid, state)
+        return state
 
     @override
-    def handle_object_update(self, vid: int, status: str, args: Sequence[str]) -> None:
+    def parse_object_update(self, vid: int, status: str, args: Sequence[str]) -> State:
         """Handle state changes for an RGB load."""
-
         rgb_load: RGBLoad = self[vid]
-        state: Dict[str, Any] = {}
         if status == "Load.GetLevel":
-            state["level"] = LoadInterface.parse_get_level_status(args)
+            return {
+                "level": LoadInterface.parse_get_level_status(args),
+            }
 
-        elif status == "RGBLoad.GetHSL" and rgb_load.is_rgb:
+        if status == "RGBLoad.GetHSL" and rgb_load.is_rgb:
             channel, value = RGBLoadInterface.parse_color_channel_status(args)
             if hsl := self._build_color_from_channels(vid, channel, value, 3):
-                state["hsl"] = hsl
+                return {"hsl": hsl}
+            return None
 
-        elif status == "RGBLoad.GetRGB" and rgb_load.is_rgb:
+        if status == "RGBLoad.GetRGB" and rgb_load.is_rgb:
             channel, value = RGBLoadInterface.parse_color_channel_status(args)
             if rgb := self._build_color_from_channels(vid, channel, value, 3):
-                state["rgb"] = rgb
+                return {"rgb": rgb}
+            return None
 
-        elif status == "RGBLoad.GetRGBW" and rgb_load.is_rgb:
+        if status == "RGBLoad.GetRGBW" and rgb_load.is_rgb:
             channel, value = RGBLoadInterface.parse_color_channel_status(args)
             if rgbw := self._build_color_from_channels(vid, channel, value, 4):
-                state["rgbw"] = rgbw
+                return {"rgbw": rgbw}
+            return None
 
-        elif status == "ColorTemperature.Get" and rgb_load.is_cct:
-            state["color_temp"] = ColorTemperatureInterface.parse_get_status(args)
+        if status == "ColorTemperature.Get" and rgb_load.is_cct:
+            return {
+                "color_temp": ColorTemperatureInterface.parse_get_status(args),
+            }
 
-        self.update_state(vid, state)
+        return None
 
     @property
-    def on(self) -> QuerySet[RGBLoad]:
+    def is_on(self) -> QuerySet[RGBLoad]:
         """Return a queryset of all RGB loads that are turned on."""
-
         return self.filter(lambda load: load.is_on)
 
     @property
-    def off(self) -> QuerySet[RGBLoad]:
+    def is_off(self) -> QuerySet[RGBLoad]:
         """Return a queryset of all RGB loads that are turned off."""
-
         return self.filter(lambda load: not load.is_on)
 
     def _build_color_from_channels(
         self, vid: int, channel: int, value: int, num_channels: int
     ) -> Optional[Tuple[int, ...]]:
         # Build a color from a series of channel value events. We need to store
         # partially constructed colors in memory, since updates come separately for
```

### Comparing `aiovantage-0.4.0/src/aiovantage/controllers/temperature_sensors.py` & `aiovantage-0.5.0/src/aiovantage/controllers/temperature_sensors.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 """Controller holding and managing Vantage temperature sensors."""
 
-from typing import Any, Dict, Sequence
+from typing import Sequence
 
 from typing_extensions import override
 
 from aiovantage.command_client.interfaces import TemperatureInterface
 from aiovantage.config_client.objects import Temperature
 
-from .base import StatefulController
+from .base import BaseController, State
 
 
-class TemperatureSensorsController(
-    StatefulController[Temperature], TemperatureInterface
-):
+class TemperatureSensorsController(BaseController[Temperature], TemperatureInterface):
     """Controller holding and managing Vantage temperature sensors."""
 
-    # Fetch the following object types from Vantage
     vantage_types = ("Temperature",)
+    """The Vantage object types that this controller will fetch."""
 
-    # Subscribe to status updates from the Enhanced Log for the following methods
-    enhanced_log_status = True
     enhanced_log_status_methods = ("Temperature.GetValue",)
+    """Which status methods this controller handles from the Enhanced Log."""
 
     @override
-    async def fetch_object_state(self, vid: int) -> None:
-        """Fetch the initial state of a temperature sensor."""
-
-        state: Dict[str, Any] = {
+    async def fetch_object_state(self, vid: int) -> State:
+        """Fetch the state properties of a temperature sensor."""
+        return {
             "value": await TemperatureInterface.get_value(self, vid),
         }
 
-        self.update_state(vid, state)
-
     @override
-    def handle_object_update(self, vid: int, status: str, args: Sequence[str]) -> None:
+    def parse_object_update(self, _vid: int, status: str, args: Sequence[str]) -> State:
         """Handle state changes for a temperature sensor."""
+        if status != "Temperature.GetValue":
+            return None
 
-        state: Dict[str, Any] = {}
-        if status == "Temperature.GetValue":
-            state["value"] = TemperatureInterface.parse_get_value_status(args)
-
-        self.update_state(vid, state)
+        return {
+            "value": TemperatureInterface.parse_get_value_status(args),
+        }
```

### Comparing `aiovantage-0.4.0/LICENSE` & `aiovantage-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiovantage-0.4.0/pyproject.toml` & `aiovantage-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -66,26 +66,31 @@
 [tool.black]
 target-version = ["py38"]
 skip-string-normalization = true
 
 [tool.ruff]
 target-version = "py38"
 select = [
+    "F",    # pyflakes
     "E",    # pycodestyle errors
     "W",    # pycodestyle warnings
-    "F",    # pyflakes
     "I",    # isort
+    "N",    # pep8-naming
+    "UP",   # pyupgrade
+    "D",    # pydocstyle
     "C",    # flake8-comprehensions
     "B",    # flake8-bugbear
     "Q",    # flake8-quotes
-    "UP",   # pyupgrade
     "C90",  # mccabe
 ]
 ignore = [
     "E501",  # line too long, handled by black
 ]
 
 [tool.ruff.isort]
 known-first-party = ["aiovantage"]
 
 [tool.ruff.mccabe]
-max-complexity = 15
+max-complexity = 15
+
+[tool.ruff.pydocstyle]
+convention = "google"
```

