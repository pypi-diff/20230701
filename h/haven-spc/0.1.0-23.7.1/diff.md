# Comparing `tmp/haven-spc-0.1.0.tar.gz` & `tmp/haven-spc-23.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haven-spc-0.1.0.tar", last modified: Sat Jul  1 17:55:28 2023, max compression
+gzip compressed data, was "haven-spc-23.7.1.tar", last modified: Sat Jul  1 18:20:47 2023, max compression
```

## Comparing `haven-spc-0.1.0.tar` & `haven-spc-23.7.1.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-01 17:55:28.397106 haven-spc-0.1.0/
--rw-------   0 b268176   (2319) xsdspc    (1117)     1702 2023-07-01 17:55:28.397106 haven-spc-0.1.0/PKG-INFO
--rw-------   0 b268176   (2319) xsdspc    (1117)      993 2023-04-10 22:19:31.000000 haven-spc-0.1.0/README.md
--rw-------   0 b268176   (2319) xsdspc    (1117)     2533 2023-07-01 17:43:25.000000 haven-spc-0.1.0/pyproject.toml
--rw-------   0 b268176   (2319) xsdspc    (1117)       38 2023-07-01 17:55:28.397106 haven-spc-0.1.0/setup.cfg
-drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-01 17:55:28.383106 haven-spc-0.1.0/src/
-drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-01 17:55:28.384106 haven-spc-0.1.0/src/firefly/
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)       67 2023-04-10 22:19:31.000000 haven-spc-0.1.0/src/firefly/__init__.py
--rw-------   0 b268176   (2319) xsdspc    (1117)    16757 2023-06-23 02:06:13.000000 haven-spc-0.1.0/src/firefly/application.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     2467 2023-06-23 01:30:52.000000 haven-spc-0.1.0/src/firefly/area_detector_viewer.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     5569 2023-06-01 22:20:45.000000 haven-spc-0.1.0/src/firefly/bss.py
--rw-------   0 b268176   (2319) xsdspc    (1117)      538 2023-06-23 01:30:52.000000 haven-spc-0.1.0/src/firefly/button.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     3588 2023-06-23 01:30:52.000000 haven-spc-0.1.0/src/firefly/camera.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     1448 2023-06-23 01:09:32.000000 haven-spc-0.1.0/src/firefly/cameras.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     1716 2023-06-23 01:09:32.000000 haven-spc-0.1.0/src/firefly/display.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     4270 2023-06-01 22:20:45.000000 haven-spc-0.1.0/src/firefly/energy.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     6112 2023-06-23 01:30:52.000000 haven-spc-0.1.0/src/firefly/launcher.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     8639 2023-06-23 01:30:52.000000 haven-spc-0.1.0/src/firefly/main_window.py
--rw-------   0 b268176   (2319) xsdspc    (1117)      560 2023-06-23 02:42:38.000000 haven-spc-0.1.0/src/firefly/motor.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     1782 2023-06-23 01:30:52.000000 haven-spc-0.1.0/src/firefly/ophyd_plugin.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     3359 2023-06-23 01:30:52.000000 haven-spc-0.1.0/src/firefly/queue_client.py
--rw-------   0 b268176   (2319) xsdspc    (1117)    18767 2023-06-23 02:42:38.000000 haven-spc-0.1.0/src/firefly/run_browser.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     5845 2023-06-23 02:42:38.000000 haven-spc-0.1.0/src/firefly/run_client.py
--rw-------   0 b268176   (2319) xsdspc    (1117)      373 2023-06-01 22:20:45.000000 haven-spc-0.1.0/src/firefly/status.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     3541 2023-06-01 22:20:45.000000 haven-spc-0.1.0/src/firefly/voltmeter.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     1780 2023-06-23 01:30:52.000000 haven-spc-0.1.0/src/firefly/voltmeters.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     2582 2023-04-10 22:19:31.000000 haven-spc-0.1.0/src/firefly/xafs_scan.py
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)      240 2023-04-10 22:19:31.000000 haven-spc-0.1.0/src/firefly/xafs_scan_region.py
--rw-------   0 b268176   (2319) xsdspc    (1117)    27385 2023-06-23 02:42:39.000000 haven-spc-0.1.0/src/firefly/xrf_detector.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     1162 2023-06-23 01:30:52.000000 haven-spc-0.1.0/src/firefly/xrf_roi.py
-drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-01 17:55:28.385106 haven-spc-0.1.0/src/haven/
--rw-------   0 b268176   (2319) xsdspc    (1117)     1941 2023-06-23 01:09:32.000000 haven-spc-0.1.0/src/haven/__init__.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     2350 2023-06-01 22:20:45.000000 haven-spc-0.1.0/src/haven/_iconfig.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     2401 2023-06-23 01:30:52.000000 haven-spc-0.1.0/src/haven/catalog.py
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)      114 2022-12-04 22:26:31.000000 haven-spc-0.1.0/src/haven/constants.py
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     4337 2022-12-04 22:26:31.000000 haven-spc-0.1.0/src/haven/energy_ranges.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     1782 2023-06-23 01:30:52.000000 haven-spc-0.1.0/src/haven/exceptions.py
-drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-01 17:55:28.386106 haven-spc-0.1.0/src/haven/instrument/
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)      225 2022-12-04 22:26:31.000000 haven-spc-0.1.0/src/haven/instrument/__init__.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     1339 2023-06-23 01:09:32.000000 haven-spc-0.1.0/src/haven/instrument/aps.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     6763 2023-06-23 01:30:52.000000 haven-spc-0.1.0/src/haven/instrument/area_detector.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     3034 2023-06-23 02:42:36.000000 haven-spc-0.1.0/src/haven/instrument/camera.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     2413 2023-06-23 02:42:35.000000 haven-spc-0.1.0/src/haven/instrument/device.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     4364 2023-06-01 22:20:45.000000 haven-spc-0.1.0/src/haven/instrument/energy_positioner.py
--rw-------   0 b268176   (2319) xsdspc    (1117)    11264 2023-06-23 01:30:52.000000 haven-spc-0.1.0/src/haven/instrument/fluorescence_detector.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     1163 2023-06-23 02:42:35.000000 haven-spc-0.1.0/src/haven/instrument/heater.py
--rw-------   0 b268176   (2319) xsdspc    (1117)    11264 2023-06-23 02:08:27.000000 haven-spc-0.1.0/src/haven/instrument/instrument_registry.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     9915 2023-06-23 01:30:52.000000 haven-spc-0.1.0/src/haven/instrument/ion_chamber.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     5700 2023-06-01 22:20:45.000000 haven-spc-0.1.0/src/haven/instrument/lerix.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     2749 2023-06-23 02:27:42.000000 haven-spc-0.1.0/src/haven/instrument/load_instrument.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     2135 2023-06-01 22:20:45.000000 haven-spc-0.1.0/src/haven/instrument/monochromator.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     2543 2023-06-01 22:20:45.000000 haven-spc-0.1.0/src/haven/instrument/motor.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     1654 2023-04-10 22:19:31.000000 haven-spc-0.1.0/src/haven/instrument/power_supply.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     1796 2023-06-01 22:20:45.000000 haven-spc-0.1.0/src/haven/instrument/scaler_triggered.py
--rw-------   0 b268176   (2319) xsdspc    (1117)      932 2023-06-23 02:42:36.000000 haven-spc-0.1.0/src/haven/instrument/shutter.py
--rw-------   0 b268176   (2319) xsdspc    (1117)      442 2023-06-01 22:20:45.000000 haven-spc-0.1.0/src/haven/instrument/slits.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     1324 2023-06-01 22:20:45.000000 haven-spc-0.1.0/src/haven/instrument/stage.py
--rw-------   0 b268176   (2319) xsdspc    (1117)      480 2023-04-10 22:19:31.000000 haven-spc-0.1.0/src/haven/instrument/xray_source.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     9122 2023-06-01 22:20:45.000000 haven-spc-0.1.0/src/haven/motor_position.py
-drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-01 17:55:28.386106 haven-spc-0.1.0/src/haven/plans/
--rw-------   0 b268176   (2319) xsdspc    (1117)       46 2023-04-10 22:19:31.000000 haven-spc-0.1.0/src/haven/plans/__init__.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     4225 2023-06-01 22:20:45.000000 haven-spc-0.1.0/src/haven/plans/align_motor.py
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     1759 2022-12-04 22:26:31.000000 haven-spc-0.1.0/src/haven/plans/align_slits.py
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     3770 2022-12-04 22:26:31.000000 haven-spc-0.1.0/src/haven/plans/auto_gain.py
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     4902 2022-12-04 22:26:31.000000 haven-spc-0.1.0/src/haven/plans/beam_properties.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     4445 2023-06-01 22:20:45.000000 haven-spc-0.1.0/src/haven/plans/energy_scan.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     3787 2023-06-23 01:30:52.000000 haven-spc-0.1.0/src/haven/plans/mono_ID_calibration.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     5214 2023-04-10 22:19:31.000000 haven-spc-0.1.0/src/haven/plans/mono_gap_calibration.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     1300 2023-06-01 22:20:45.000000 haven-spc-0.1.0/src/haven/plans/record_dark_current.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     2319 2023-06-23 01:30:52.000000 haven-spc-0.1.0/src/haven/plans/set_energy.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     1791 2023-06-01 22:20:45.000000 haven-spc-0.1.0/src/haven/plans/shutters.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     5401 2023-06-01 22:20:45.000000 haven-spc-0.1.0/src/haven/plans/xafs_scan.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     5919 2023-07-01 17:44:42.000000 haven-spc-0.1.0/src/haven/preprocessors.py
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)      516 2022-12-04 22:26:31.000000 haven-spc-0.1.0/src/haven/progress_bar.py
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     2145 2023-06-07 19:55:42.000000 haven-spc-0.1.0/src/haven/run_engine.py
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     6262 2023-06-07 19:55:42.000000 haven-spc-0.1.0/src/haven/simulated_ioc.py
-drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-01 17:55:28.387106 haven-spc-0.1.0/src/haven/tests/
--rw-------   0 b268176   (2319) xsdspc    (1117)        0 2023-06-01 22:20:45.000000 haven-spc-0.1.0/src/haven/tests/__init__.py
--rw-------   0 b268176   (2319) xsdspc    (1117)    11922 2023-06-01 22:20:45.000000 haven-spc-0.1.0/src/haven/tests/ioc_apsbss.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     1093 2023-06-23 01:30:52.000000 haven-spc-0.1.0/src/haven/tests/ioc_area_detector.py
--rwx------   0 b268176   (2319) xsdspc    (1117)     6568 2023-06-23 02:42:36.000000 haven-spc-0.1.0/src/haven/tests/ioc_dxp.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     1939 2023-06-01 22:20:45.000000 haven-spc-0.1.0/src/haven/tests/ioc_mono.py
--rw-------   0 b268176   (2319) xsdspc    (1117)      891 2023-06-01 22:20:45.000000 haven-spc-0.1.0/src/haven/tests/ioc_motor.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     1843 2023-06-01 22:20:45.000000 haven-spc-0.1.0/src/haven/tests/ioc_preamp.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     2867 2023-06-01 22:20:45.000000 haven-spc-0.1.0/src/haven/tests/ioc_ptc10.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     6020 2023-06-01 22:20:45.000000 haven-spc-0.1.0/src/haven/tests/ioc_scaler.py
--rw-------   0 b268176   (2319) xsdspc    (1117)      896 2023-06-01 22:20:45.000000 haven-spc-0.1.0/src/haven/tests/ioc_simple.py
--rw-------   0 b268176   (2319) xsdspc    (1117)      963 2023-06-01 22:20:45.000000 haven-spc-0.1.0/src/haven/tests/ioc_undulator.py
--rw-------   0 b268176   (2319) xsdspc    (1117)      387 2023-06-23 01:30:52.000000 haven-spc-0.1.0/src/haven/tests/test_catalogs.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     7159 2023-06-23 01:30:52.000000 haven-spc-0.1.0/src/haven/tests/tiled_example.py
--rw-------   0 b268176   (2319) xsdspc    (1117)      227 2023-04-10 22:19:31.000000 haven-spc-0.1.0/src/haven/typing.py
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     7188 2023-04-10 22:19:31.000000 haven-spc-0.1.0/src/haven/xdi_writer.py
-drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-01 17:55:28.387106 haven-spc-0.1.0/src/haven_spc.egg-info/
--rw-------   0 b268176   (2319) xsdspc    (1117)     1702 2023-07-01 17:55:28.000000 haven-spc-0.1.0/src/haven_spc.egg-info/PKG-INFO
--rw-------   0 b268176   (2319) xsdspc    (1117)     3786 2023-07-01 17:55:28.000000 haven-spc-0.1.0/src/haven_spc.egg-info/SOURCES.txt
--rw-------   0 b268176   (2319) xsdspc    (1117)        1 2023-07-01 17:55:28.000000 haven-spc-0.1.0/src/haven_spc.egg-info/dependency_links.txt
--rw-------   0 b268176   (2319) xsdspc    (1117)      157 2023-07-01 17:55:28.000000 haven-spc-0.1.0/src/haven_spc.egg-info/entry_points.txt
--rw-------   0 b268176   (2319) xsdspc    (1117)      246 2023-07-01 17:55:28.000000 haven-spc-0.1.0/src/haven_spc.egg-info/requires.txt
--rw-------   0 b268176   (2319) xsdspc    (1117)       14 2023-07-01 17:55:28.000000 haven-spc-0.1.0/src/haven_spc.egg-info/top_level.txt
-drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-01 17:55:28.397106 haven-spc-0.1.0/tests/
--rw-------   0 b268176   (2319) xsdspc    (1117)     2103 2023-04-10 22:19:31.000000 haven-spc-0.1.0/tests/test_align_motor.py
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)      814 2023-04-10 22:19:31.000000 haven-spc-0.1.0/tests/test_application.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     1023 2023-06-01 22:21:34.000000 haven-spc-0.1.0/tests/test_aps.py
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)      317 2023-06-07 19:55:42.000000 haven-spc-0.1.0/tests/test_area_detector.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     2668 2023-06-23 02:09:01.000000 haven-spc-0.1.0/tests/test_area_detector_display.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     3500 2023-04-10 22:19:31.000000 haven-spc-0.1.0/tests/test_beam_properties.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     9553 2023-06-01 22:21:12.000000 haven-spc-0.1.0/tests/test_bss_display.py
--rw-------   0 b268176   (2319) xsdspc    (1117)      917 2023-06-01 22:20:45.000000 haven-spc-0.1.0/tests/test_camera.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     3458 2023-06-23 02:42:41.000000 haven-spc-0.1.0/tests/test_cameras_display.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     5173 2023-06-01 22:20:45.000000 haven-spc-0.1.0/tests/test_energy_display.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     1873 2023-06-01 22:20:45.000000 haven-spc-0.1.0/tests/test_energy_positioner.py
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     1646 2023-04-12 20:07:31.000000 haven-spc-0.1.0/tests/test_energy_ranges.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     6214 2023-06-23 02:42:41.000000 haven-spc-0.1.0/tests/test_fluorescence.py
--rw-------   0 b268176   (2319) xsdspc    (1117)      793 2023-06-23 02:31:03.000000 haven-spc-0.1.0/tests/test_heater.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     1566 2023-06-01 22:20:45.000000 haven-spc-0.1.0/tests/test_iconfig.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     7013 2023-06-23 01:30:52.000000 haven-spc-0.1.0/tests/test_instrument_registry.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     5450 2023-06-01 22:20:45.000000 haven-spc-0.1.0/tests/test_ion_chamber.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     5100 2023-06-01 22:20:45.000000 haven-spc-0.1.0/tests/test_lerix.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     1996 2023-06-01 22:20:45.000000 haven-spc-0.1.0/tests/test_main_window.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     2837 2023-04-10 22:19:31.000000 haven-spc-0.1.0/tests/test_mono_ID_calibration_plan.py
--rw-------   0 b268176   (2319) xsdspc    (1117)      394 2023-06-01 22:20:45.000000 haven-spc-0.1.0/tests/test_monochromator.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     1511 2023-06-01 22:20:45.000000 haven-spc-0.1.0/tests/test_motor.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     1549 2023-06-01 22:20:45.000000 haven-spc-0.1.0/tests/test_motor_menu.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     2554 2023-06-01 22:20:45.000000 haven-spc-0.1.0/tests/test_ophyd_connection.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     9709 2023-06-23 01:30:52.000000 haven-spc-0.1.0/tests/test_plans.py
--rw-------   0 b268176   (2319) xsdspc    (1117)      473 2023-06-01 22:20:45.000000 haven-spc-0.1.0/tests/test_power_supply.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     9424 2023-06-01 22:20:45.000000 haven-spc-0.1.0/tests/test_preprocessors.py
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     3190 2023-06-07 19:55:42.000000 haven-spc-0.1.0/tests/test_queue_client.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     9430 2023-06-23 02:42:42.000000 haven-spc-0.1.0/tests/test_run_browser.py
--rw-------   0 b268176   (2319) xsdspc    (1117)      866 2023-06-01 22:20:45.000000 haven-spc-0.1.0/tests/test_run_engine.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     8241 2023-06-01 22:20:45.000000 haven-spc-0.1.0/tests/test_save_motor_positions.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     1394 2023-04-10 22:19:31.000000 haven-spc-0.1.0/tests/test_scaler_triggering.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     1788 2023-06-23 01:30:52.000000 haven-spc-0.1.0/tests/test_set_energy.py
--rw-------   0 b268176   (2319) xsdspc    (1117)      828 2023-06-01 22:20:45.000000 haven-spc-0.1.0/tests/test_shutter.py
--rw-------   0 b268176   (2319) xsdspc    (1117)      289 2023-04-29 19:01:19.000000 haven-spc-0.1.0/tests/test_simulated_devices.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     5966 2023-06-23 01:30:52.000000 haven-spc-0.1.0/tests/test_simulated_ioc.py
--rw-------   0 b268176   (2319) xsdspc    (1117)      304 2023-04-10 22:19:31.000000 haven-spc-0.1.0/tests/test_slits.py
--rw-------   0 b268176   (2319) xsdspc    (1117)      985 2023-06-01 22:20:45.000000 haven-spc-0.1.0/tests/test_stages.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     3538 2023-06-01 22:20:45.000000 haven-spc-0.1.0/tests/test_voltmeters.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     1806 2023-04-10 22:19:31.000000 haven-spc-0.1.0/tests/test_xafs_scan.py
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     8691 2023-04-10 22:19:31.000000 haven-spc-0.1.0/tests/test_xdi_writer.py
--rw-------   0 b268176   (2319) xsdspc    (1117)      309 2023-06-01 22:20:45.000000 haven-spc-0.1.0/tests/test_xray_source.py
--rw-------   0 b268176   (2319) xsdspc    (1117)    14369 2023-06-23 02:42:42.000000 haven-spc-0.1.0/tests/test_xrf_detector_display.py
+drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-01 18:20:47.700168 haven-spc-23.7.1/
+-rw-------   0 b268176   (2319) xsdspc    (1117)     2192 2023-07-01 18:20:47.700168 haven-spc-23.7.1/PKG-INFO
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1490 2023-07-01 18:20:19.000000 haven-spc-23.7.1/README.md
+-rw-------   0 b268176   (2319) xsdspc    (1117)     2531 2023-07-01 18:18:02.000000 haven-spc-23.7.1/pyproject.toml
+-rw-------   0 b268176   (2319) xsdspc    (1117)       38 2023-07-01 18:20:47.700168 haven-spc-23.7.1/setup.cfg
+drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-01 18:20:47.694168 haven-spc-23.7.1/src/
+drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-01 18:20:47.695168 haven-spc-23.7.1/src/firefly/
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)       67 2023-04-10 22:19:31.000000 haven-spc-23.7.1/src/firefly/__init__.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)    16757 2023-06-23 02:06:13.000000 haven-spc-23.7.1/src/firefly/application.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     2467 2023-06-23 01:30:52.000000 haven-spc-23.7.1/src/firefly/area_detector_viewer.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     5569 2023-06-01 22:20:45.000000 haven-spc-23.7.1/src/firefly/bss.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)      538 2023-06-23 01:30:52.000000 haven-spc-23.7.1/src/firefly/button.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     3588 2023-06-23 01:30:52.000000 haven-spc-23.7.1/src/firefly/camera.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1448 2023-06-23 01:09:32.000000 haven-spc-23.7.1/src/firefly/cameras.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1716 2023-06-23 01:09:32.000000 haven-spc-23.7.1/src/firefly/display.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     4270 2023-06-01 22:20:45.000000 haven-spc-23.7.1/src/firefly/energy.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     6112 2023-06-23 01:30:52.000000 haven-spc-23.7.1/src/firefly/launcher.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     8639 2023-06-23 01:30:52.000000 haven-spc-23.7.1/src/firefly/main_window.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)      560 2023-06-23 02:42:38.000000 haven-spc-23.7.1/src/firefly/motor.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1782 2023-06-23 01:30:52.000000 haven-spc-23.7.1/src/firefly/ophyd_plugin.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     3359 2023-06-23 01:30:52.000000 haven-spc-23.7.1/src/firefly/queue_client.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)    18767 2023-06-23 02:42:38.000000 haven-spc-23.7.1/src/firefly/run_browser.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     5845 2023-06-23 02:42:38.000000 haven-spc-23.7.1/src/firefly/run_client.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)      373 2023-06-01 22:20:45.000000 haven-spc-23.7.1/src/firefly/status.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     3541 2023-06-01 22:20:45.000000 haven-spc-23.7.1/src/firefly/voltmeter.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1780 2023-06-23 01:30:52.000000 haven-spc-23.7.1/src/firefly/voltmeters.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     2582 2023-04-10 22:19:31.000000 haven-spc-23.7.1/src/firefly/xafs_scan.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      240 2023-04-10 22:19:31.000000 haven-spc-23.7.1/src/firefly/xafs_scan_region.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)    27385 2023-06-23 02:42:39.000000 haven-spc-23.7.1/src/firefly/xrf_detector.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1162 2023-06-23 01:30:52.000000 haven-spc-23.7.1/src/firefly/xrf_roi.py
+drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-01 18:20:47.696168 haven-spc-23.7.1/src/haven/
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1941 2023-06-23 01:09:32.000000 haven-spc-23.7.1/src/haven/__init__.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     2350 2023-06-01 22:20:45.000000 haven-spc-23.7.1/src/haven/_iconfig.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     2401 2023-06-23 01:30:52.000000 haven-spc-23.7.1/src/haven/catalog.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      114 2022-12-04 22:26:31.000000 haven-spc-23.7.1/src/haven/constants.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     4337 2022-12-04 22:26:31.000000 haven-spc-23.7.1/src/haven/energy_ranges.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1782 2023-06-23 01:30:52.000000 haven-spc-23.7.1/src/haven/exceptions.py
+drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-01 18:20:47.697168 haven-spc-23.7.1/src/haven/instrument/
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      225 2022-12-04 22:26:31.000000 haven-spc-23.7.1/src/haven/instrument/__init__.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1339 2023-06-23 01:09:32.000000 haven-spc-23.7.1/src/haven/instrument/aps.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     6763 2023-06-23 01:30:52.000000 haven-spc-23.7.1/src/haven/instrument/area_detector.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     3034 2023-06-23 02:42:36.000000 haven-spc-23.7.1/src/haven/instrument/camera.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     2413 2023-06-23 02:42:35.000000 haven-spc-23.7.1/src/haven/instrument/device.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     4364 2023-06-01 22:20:45.000000 haven-spc-23.7.1/src/haven/instrument/energy_positioner.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)    11264 2023-06-23 01:30:52.000000 haven-spc-23.7.1/src/haven/instrument/fluorescence_detector.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1163 2023-06-23 02:42:35.000000 haven-spc-23.7.1/src/haven/instrument/heater.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)    11264 2023-06-23 02:08:27.000000 haven-spc-23.7.1/src/haven/instrument/instrument_registry.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     9915 2023-06-23 01:30:52.000000 haven-spc-23.7.1/src/haven/instrument/ion_chamber.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     5700 2023-06-01 22:20:45.000000 haven-spc-23.7.1/src/haven/instrument/lerix.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     2749 2023-06-23 02:27:42.000000 haven-spc-23.7.1/src/haven/instrument/load_instrument.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     2135 2023-06-01 22:20:45.000000 haven-spc-23.7.1/src/haven/instrument/monochromator.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     2543 2023-06-01 22:20:45.000000 haven-spc-23.7.1/src/haven/instrument/motor.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1654 2023-04-10 22:19:31.000000 haven-spc-23.7.1/src/haven/instrument/power_supply.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1796 2023-06-01 22:20:45.000000 haven-spc-23.7.1/src/haven/instrument/scaler_triggered.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)      932 2023-06-23 02:42:36.000000 haven-spc-23.7.1/src/haven/instrument/shutter.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)      442 2023-06-01 22:20:45.000000 haven-spc-23.7.1/src/haven/instrument/slits.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1324 2023-06-01 22:20:45.000000 haven-spc-23.7.1/src/haven/instrument/stage.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)      480 2023-04-10 22:19:31.000000 haven-spc-23.7.1/src/haven/instrument/xray_source.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     9122 2023-06-01 22:20:45.000000 haven-spc-23.7.1/src/haven/motor_position.py
+drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-01 18:20:47.697168 haven-spc-23.7.1/src/haven/plans/
+-rw-------   0 b268176   (2319) xsdspc    (1117)       46 2023-04-10 22:19:31.000000 haven-spc-23.7.1/src/haven/plans/__init__.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     4225 2023-06-01 22:20:45.000000 haven-spc-23.7.1/src/haven/plans/align_motor.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     1759 2022-12-04 22:26:31.000000 haven-spc-23.7.1/src/haven/plans/align_slits.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     3770 2022-12-04 22:26:31.000000 haven-spc-23.7.1/src/haven/plans/auto_gain.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     4902 2022-12-04 22:26:31.000000 haven-spc-23.7.1/src/haven/plans/beam_properties.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     4445 2023-06-01 22:20:45.000000 haven-spc-23.7.1/src/haven/plans/energy_scan.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     3787 2023-06-23 01:30:52.000000 haven-spc-23.7.1/src/haven/plans/mono_ID_calibration.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     5214 2023-04-10 22:19:31.000000 haven-spc-23.7.1/src/haven/plans/mono_gap_calibration.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1300 2023-06-01 22:20:45.000000 haven-spc-23.7.1/src/haven/plans/record_dark_current.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     2319 2023-06-23 01:30:52.000000 haven-spc-23.7.1/src/haven/plans/set_energy.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1791 2023-06-01 22:20:45.000000 haven-spc-23.7.1/src/haven/plans/shutters.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     5401 2023-06-01 22:20:45.000000 haven-spc-23.7.1/src/haven/plans/xafs_scan.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     5919 2023-07-01 17:44:42.000000 haven-spc-23.7.1/src/haven/preprocessors.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      516 2022-12-04 22:26:31.000000 haven-spc-23.7.1/src/haven/progress_bar.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     2145 2023-06-07 19:55:42.000000 haven-spc-23.7.1/src/haven/run_engine.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     6262 2023-06-07 19:55:42.000000 haven-spc-23.7.1/src/haven/simulated_ioc.py
+drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-01 18:20:47.698168 haven-spc-23.7.1/src/haven/tests/
+-rw-------   0 b268176   (2319) xsdspc    (1117)        0 2023-06-01 22:20:45.000000 haven-spc-23.7.1/src/haven/tests/__init__.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)    11922 2023-06-01 22:20:45.000000 haven-spc-23.7.1/src/haven/tests/ioc_apsbss.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1093 2023-06-23 01:30:52.000000 haven-spc-23.7.1/src/haven/tests/ioc_area_detector.py
+-rwx------   0 b268176   (2319) xsdspc    (1117)     6568 2023-06-23 02:42:36.000000 haven-spc-23.7.1/src/haven/tests/ioc_dxp.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1939 2023-06-01 22:20:45.000000 haven-spc-23.7.1/src/haven/tests/ioc_mono.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)      891 2023-06-01 22:20:45.000000 haven-spc-23.7.1/src/haven/tests/ioc_motor.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1843 2023-06-01 22:20:45.000000 haven-spc-23.7.1/src/haven/tests/ioc_preamp.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     2867 2023-06-01 22:20:45.000000 haven-spc-23.7.1/src/haven/tests/ioc_ptc10.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     6020 2023-06-01 22:20:45.000000 haven-spc-23.7.1/src/haven/tests/ioc_scaler.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)      896 2023-06-01 22:20:45.000000 haven-spc-23.7.1/src/haven/tests/ioc_simple.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)      963 2023-06-01 22:20:45.000000 haven-spc-23.7.1/src/haven/tests/ioc_undulator.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)      387 2023-06-23 01:30:52.000000 haven-spc-23.7.1/src/haven/tests/test_catalogs.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     7159 2023-06-23 01:30:52.000000 haven-spc-23.7.1/src/haven/tests/tiled_example.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)      227 2023-04-10 22:19:31.000000 haven-spc-23.7.1/src/haven/typing.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     7188 2023-04-10 22:19:31.000000 haven-spc-23.7.1/src/haven/xdi_writer.py
+drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-01 18:20:47.698168 haven-spc-23.7.1/src/haven_spc.egg-info/
+-rw-------   0 b268176   (2319) xsdspc    (1117)     2192 2023-07-01 18:20:47.000000 haven-spc-23.7.1/src/haven_spc.egg-info/PKG-INFO
+-rw-------   0 b268176   (2319) xsdspc    (1117)     3786 2023-07-01 18:20:47.000000 haven-spc-23.7.1/src/haven_spc.egg-info/SOURCES.txt
+-rw-------   0 b268176   (2319) xsdspc    (1117)        1 2023-07-01 18:20:47.000000 haven-spc-23.7.1/src/haven_spc.egg-info/dependency_links.txt
+-rw-------   0 b268176   (2319) xsdspc    (1117)      157 2023-07-01 18:20:47.000000 haven-spc-23.7.1/src/haven_spc.egg-info/entry_points.txt
+-rw-------   0 b268176   (2319) xsdspc    (1117)      252 2023-07-01 18:20:47.000000 haven-spc-23.7.1/src/haven_spc.egg-info/requires.txt
+-rw-------   0 b268176   (2319) xsdspc    (1117)       14 2023-07-01 18:20:47.000000 haven-spc-23.7.1/src/haven_spc.egg-info/top_level.txt
+drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-01 18:20:47.700168 haven-spc-23.7.1/tests/
+-rw-------   0 b268176   (2319) xsdspc    (1117)     2103 2023-04-10 22:19:31.000000 haven-spc-23.7.1/tests/test_align_motor.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      814 2023-04-10 22:19:31.000000 haven-spc-23.7.1/tests/test_application.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1023 2023-06-01 22:21:34.000000 haven-spc-23.7.1/tests/test_aps.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      317 2023-06-07 19:55:42.000000 haven-spc-23.7.1/tests/test_area_detector.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     2668 2023-06-23 02:09:01.000000 haven-spc-23.7.1/tests/test_area_detector_display.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     3500 2023-04-10 22:19:31.000000 haven-spc-23.7.1/tests/test_beam_properties.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     9553 2023-06-01 22:21:12.000000 haven-spc-23.7.1/tests/test_bss_display.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)      917 2023-06-01 22:20:45.000000 haven-spc-23.7.1/tests/test_camera.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     3458 2023-06-23 02:42:41.000000 haven-spc-23.7.1/tests/test_cameras_display.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     5173 2023-06-01 22:20:45.000000 haven-spc-23.7.1/tests/test_energy_display.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1873 2023-06-01 22:20:45.000000 haven-spc-23.7.1/tests/test_energy_positioner.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     1646 2023-04-12 20:07:31.000000 haven-spc-23.7.1/tests/test_energy_ranges.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     6214 2023-06-23 02:42:41.000000 haven-spc-23.7.1/tests/test_fluorescence.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)      793 2023-06-23 02:31:03.000000 haven-spc-23.7.1/tests/test_heater.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1566 2023-06-01 22:20:45.000000 haven-spc-23.7.1/tests/test_iconfig.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     7013 2023-06-23 01:30:52.000000 haven-spc-23.7.1/tests/test_instrument_registry.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     5450 2023-06-01 22:20:45.000000 haven-spc-23.7.1/tests/test_ion_chamber.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     5100 2023-06-01 22:20:45.000000 haven-spc-23.7.1/tests/test_lerix.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1996 2023-06-01 22:20:45.000000 haven-spc-23.7.1/tests/test_main_window.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     2837 2023-04-10 22:19:31.000000 haven-spc-23.7.1/tests/test_mono_ID_calibration_plan.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)      394 2023-06-01 22:20:45.000000 haven-spc-23.7.1/tests/test_monochromator.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1511 2023-06-01 22:20:45.000000 haven-spc-23.7.1/tests/test_motor.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1549 2023-06-01 22:20:45.000000 haven-spc-23.7.1/tests/test_motor_menu.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     2554 2023-06-01 22:20:45.000000 haven-spc-23.7.1/tests/test_ophyd_connection.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     9709 2023-06-23 01:30:52.000000 haven-spc-23.7.1/tests/test_plans.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)      473 2023-06-01 22:20:45.000000 haven-spc-23.7.1/tests/test_power_supply.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     9424 2023-06-01 22:20:45.000000 haven-spc-23.7.1/tests/test_preprocessors.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     3190 2023-06-07 19:55:42.000000 haven-spc-23.7.1/tests/test_queue_client.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     9430 2023-06-23 02:42:42.000000 haven-spc-23.7.1/tests/test_run_browser.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)      866 2023-06-01 22:20:45.000000 haven-spc-23.7.1/tests/test_run_engine.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     8241 2023-06-01 22:20:45.000000 haven-spc-23.7.1/tests/test_save_motor_positions.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1394 2023-04-10 22:19:31.000000 haven-spc-23.7.1/tests/test_scaler_triggering.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1788 2023-06-23 01:30:52.000000 haven-spc-23.7.1/tests/test_set_energy.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)      828 2023-06-01 22:20:45.000000 haven-spc-23.7.1/tests/test_shutter.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)      289 2023-04-29 19:01:19.000000 haven-spc-23.7.1/tests/test_simulated_devices.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     5966 2023-06-23 01:30:52.000000 haven-spc-23.7.1/tests/test_simulated_ioc.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)      304 2023-04-10 22:19:31.000000 haven-spc-23.7.1/tests/test_slits.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)      985 2023-06-01 22:20:45.000000 haven-spc-23.7.1/tests/test_stages.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     3538 2023-06-01 22:20:45.000000 haven-spc-23.7.1/tests/test_voltmeters.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1806 2023-04-10 22:19:31.000000 haven-spc-23.7.1/tests/test_xafs_scan.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     8691 2023-04-10 22:19:31.000000 haven-spc-23.7.1/tests/test_xdi_writer.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)      309 2023-06-01 22:20:45.000000 haven-spc-23.7.1/tests/test_xray_source.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)    14369 2023-06-23 02:42:42.000000 haven-spc-23.7.1/tests/test_xrf_detector_display.py
```

### Comparing `haven-spc-0.1.0/PKG-INFO` & `haven-spc-23.7.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: haven-spc
-Version: 0.1.0
-Summary: Tools and applicatrion for running the spectroscopy group beamlines at the Advanced Photon Source.
+Version: 23.7.1
+Summary: Tools and GUI for running the spectroscopy group beamlines at the Advanced Photon Source.
 Author-email: Mark Wolfman <wolfman@anl.gov>
 Project-URL: Homepage, https://haven-spc.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/spc-group/haven/issues
 Keywords: synchrotron,xray,bluesky
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
@@ -26,32 +26,57 @@
 
 "Don't fly in anything with a Capissen 38 engine, they fall right out
 of the sky."
 
 
 ## Installation
 
-*haven* uses *mamba* for dependency management, and *poetry* for
-installation and development. First create the conda environment with
-mamba:
+### Python Packing Index
+
+Easiest way to install haven is using pip.
+
+```
+$ python -m pip install 'haven-spc'
+```
+
+### Development (Conda)
+
+*haven* can also use *mamba* for dependency management, and
+*setuptools* for installation and development. First create the conda
+environment with mamba:
 
 ```
 $ mamba env create -f environment.yml -n haven
 ```
 
-then install the package, with dependencies, in developer mode:
+then install the package, in developer mode:
 
 ```
 $ conda activate haven
-$ poetry install
+$ pip install -e .
 ```
 
 ## Running Tests
 
 To run tests, run
 
 ```
 $ pytest
 ```
 
 # firefly
-User-facing applications for controlling the beamlines managed by the spectroscopy group
+
+User-facing applications for controlling the beamlines managed by the
+spectroscopy group. Be sure to include the [gui] extras if you plan
+to use the GUI.
+
+```
+$ python -m pip install 'haven-spc[gui]'
+$ firefly
+```
+
+# Versioning
+
+Haven/Firefly uses calendar versioning, with short year and short
+month for the MAJOR and MINOR versions, then a incremental MICRO
+version. For example, version *23.7.2* is the 2nd (*2*) release in
+July (*7*) 2023 (*23*).
```

### Comparing `haven-spc-0.1.0/README.md` & `haven-spc-23.7.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -8,32 +8,57 @@
 
 "Don't fly in anything with a Capissen 38 engine, they fall right out
 of the sky."
 
 
 ## Installation
 
-*haven* uses *mamba* for dependency management, and *poetry* for
-installation and development. First create the conda environment with
-mamba:
+### Python Packing Index
+
+Easiest way to install haven is using pip.
+
+```
+$ python -m pip install 'haven-spc'
+```
+
+### Development (Conda)
+
+*haven* can also use *mamba* for dependency management, and
+*setuptools* for installation and development. First create the conda
+environment with mamba:
 
 ```
 $ mamba env create -f environment.yml -n haven
 ```
 
-then install the package, with dependencies, in developer mode:
+then install the package, in developer mode:
 
 ```
 $ conda activate haven
-$ poetry install
+$ pip install -e .
 ```
 
 ## Running Tests
 
 To run tests, run
 
 ```
 $ pytest
 ```
 
 # firefly
-User-facing applications for controlling the beamlines managed by the spectroscopy group
+
+User-facing applications for controlling the beamlines managed by the
+spectroscopy group. Be sure to include the [gui] extras if you plan
+to use the GUI.
+
+```
+$ python -m pip install 'haven-spc[gui]'
+$ firefly
+```
+
+# Versioning
+
+Haven/Firefly uses calendar versioning, with short year and short
+month for the MAJOR and MINOR versions, then a incremental MICRO
+version. For example, version *23.7.2* is the 2nd (*2*) release in
+July (*7*) 2023 (*23*).
```

### Comparing `haven-spc-0.1.0/pyproject.toml` & `haven-spc-23.7.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "haven-spc"
-version = "0.1.0"
+version = "23.7.1"
 authors = [
   { name="Mark Wolfman", email="wolfman@anl.gov" },
 ]
-description = "Tools and applicatrion for running the spectroscopy group beamlines at the Advanced Photon Source."
+description = "Tools and GUI for running the spectroscopy group beamlines at the Advanced Photon Source."
 readme = "README.md"
 requires-python = ">=3.7,<3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "Development Status :: 3 - Alpha",
     "Topic :: Scientific/Engineering",
@@ -17,15 +17,15 @@
 keywords = ["synchrotron", "xray", "bluesky"]
 dependencies = ["bluesky", "ophyd", "databroker", "apsbss", "xraydb", "mergedeep", "xrayutilities", "bluesky-queueserver-api", "apstools", "databroker"]
 
 [project.optional-dependencies]
 
 dev = ["black", "pytest", "pytest-mongodb", "build", "twine",
        "time-machine", "pytest-mock", "pytest-qt", "flake8"]
-gui = ["pyqt", "tiled-client", "qtawesome", "pydm", "pyqtgraph"]
+gui = ["pyqt>=5.12", "tiled-client", "qtawesome", "pydm", "pyqtgraph"]
 
 [project.urls]
 "Homepage" = "https://haven-spc.readthedocs.io/en/latest/"
 "Bug Tracker" = "https://github.com/spc-group/haven/issues"
 
 [project.scripts]
 haven_config = "haven._iconfig:print_config_value"
```

### Comparing `haven-spc-0.1.0/src/firefly/application.py` & `haven-spc-23.7.1/src/firefly/application.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/firefly/area_detector_viewer.py` & `haven-spc-23.7.1/src/firefly/area_detector_viewer.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/firefly/bss.py` & `haven-spc-23.7.1/src/firefly/bss.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/firefly/button.py` & `haven-spc-23.7.1/src/firefly/button.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/firefly/camera.py` & `haven-spc-23.7.1/src/firefly/camera.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/firefly/cameras.py` & `haven-spc-23.7.1/src/firefly/cameras.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/firefly/display.py` & `haven-spc-23.7.1/src/firefly/display.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/firefly/energy.py` & `haven-spc-23.7.1/src/firefly/energy.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/firefly/launcher.py` & `haven-spc-23.7.1/src/firefly/launcher.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/firefly/main_window.py` & `haven-spc-23.7.1/src/firefly/main_window.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/firefly/motor.py` & `haven-spc-23.7.1/src/firefly/motor.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/firefly/ophyd_plugin.py` & `haven-spc-23.7.1/src/firefly/ophyd_plugin.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/firefly/queue_client.py` & `haven-spc-23.7.1/src/firefly/queue_client.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/firefly/run_browser.py` & `haven-spc-23.7.1/src/firefly/run_browser.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/firefly/run_client.py` & `haven-spc-23.7.1/src/firefly/run_client.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/firefly/voltmeter.py` & `haven-spc-23.7.1/src/firefly/voltmeter.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/firefly/voltmeters.py` & `haven-spc-23.7.1/src/firefly/voltmeters.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/firefly/xafs_scan.py` & `haven-spc-23.7.1/src/firefly/xafs_scan.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/firefly/xrf_detector.py` & `haven-spc-23.7.1/src/firefly/xrf_detector.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/firefly/xrf_roi.py` & `haven-spc-23.7.1/src/firefly/xrf_roi.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/__init__.py` & `haven-spc-23.7.1/src/haven/__init__.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/_iconfig.py` & `haven-spc-23.7.1/src/haven/_iconfig.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/catalog.py` & `haven-spc-23.7.1/src/haven/catalog.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/energy_ranges.py` & `haven-spc-23.7.1/src/haven/energy_ranges.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/exceptions.py` & `haven-spc-23.7.1/src/haven/exceptions.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/instrument/aps.py` & `haven-spc-23.7.1/src/haven/instrument/aps.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/instrument/area_detector.py` & `haven-spc-23.7.1/src/haven/instrument/area_detector.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/instrument/camera.py` & `haven-spc-23.7.1/src/haven/instrument/camera.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/instrument/device.py` & `haven-spc-23.7.1/src/haven/instrument/device.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/instrument/energy_positioner.py` & `haven-spc-23.7.1/src/haven/instrument/energy_positioner.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/instrument/fluorescence_detector.py` & `haven-spc-23.7.1/src/haven/instrument/fluorescence_detector.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/instrument/heater.py` & `haven-spc-23.7.1/src/haven/instrument/heater.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/instrument/instrument_registry.py` & `haven-spc-23.7.1/src/haven/instrument/instrument_registry.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/instrument/ion_chamber.py` & `haven-spc-23.7.1/src/haven/instrument/ion_chamber.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/instrument/lerix.py` & `haven-spc-23.7.1/src/haven/instrument/lerix.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/instrument/load_instrument.py` & `haven-spc-23.7.1/src/haven/instrument/load_instrument.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/instrument/monochromator.py` & `haven-spc-23.7.1/src/haven/instrument/monochromator.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/instrument/motor.py` & `haven-spc-23.7.1/src/haven/instrument/motor.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/instrument/power_supply.py` & `haven-spc-23.7.1/src/haven/instrument/power_supply.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/instrument/scaler_triggered.py` & `haven-spc-23.7.1/src/haven/instrument/scaler_triggered.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/instrument/shutter.py` & `haven-spc-23.7.1/src/haven/instrument/shutter.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/instrument/stage.py` & `haven-spc-23.7.1/src/haven/instrument/stage.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/motor_position.py` & `haven-spc-23.7.1/src/haven/motor_position.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/plans/align_motor.py` & `haven-spc-23.7.1/src/haven/plans/align_motor.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/plans/align_slits.py` & `haven-spc-23.7.1/src/haven/plans/align_slits.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/plans/auto_gain.py` & `haven-spc-23.7.1/src/haven/plans/auto_gain.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/plans/beam_properties.py` & `haven-spc-23.7.1/src/haven/plans/beam_properties.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/plans/energy_scan.py` & `haven-spc-23.7.1/src/haven/plans/energy_scan.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/plans/mono_ID_calibration.py` & `haven-spc-23.7.1/src/haven/plans/mono_ID_calibration.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/plans/mono_gap_calibration.py` & `haven-spc-23.7.1/src/haven/plans/mono_gap_calibration.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/plans/record_dark_current.py` & `haven-spc-23.7.1/src/haven/plans/record_dark_current.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/plans/set_energy.py` & `haven-spc-23.7.1/src/haven/plans/set_energy.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/plans/shutters.py` & `haven-spc-23.7.1/src/haven/plans/shutters.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/plans/xafs_scan.py` & `haven-spc-23.7.1/src/haven/plans/xafs_scan.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/preprocessors.py` & `haven-spc-23.7.1/src/haven/preprocessors.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/progress_bar.py` & `haven-spc-23.7.1/src/haven/progress_bar.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/run_engine.py` & `haven-spc-23.7.1/src/haven/run_engine.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/simulated_ioc.py` & `haven-spc-23.7.1/src/haven/simulated_ioc.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/tests/ioc_apsbss.py` & `haven-spc-23.7.1/src/haven/tests/ioc_apsbss.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/tests/ioc_area_detector.py` & `haven-spc-23.7.1/src/haven/tests/ioc_area_detector.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/tests/ioc_dxp.py` & `haven-spc-23.7.1/src/haven/tests/ioc_dxp.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/tests/ioc_mono.py` & `haven-spc-23.7.1/src/haven/tests/ioc_mono.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/tests/ioc_motor.py` & `haven-spc-23.7.1/src/haven/tests/ioc_motor.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/tests/ioc_preamp.py` & `haven-spc-23.7.1/src/haven/tests/ioc_preamp.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/tests/ioc_ptc10.py` & `haven-spc-23.7.1/src/haven/tests/ioc_ptc10.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/tests/ioc_scaler.py` & `haven-spc-23.7.1/src/haven/tests/ioc_scaler.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/tests/ioc_simple.py` & `haven-spc-23.7.1/src/haven/tests/ioc_simple.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/tests/ioc_undulator.py` & `haven-spc-23.7.1/src/haven/tests/ioc_undulator.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/tests/tiled_example.py` & `haven-spc-23.7.1/src/haven/tests/tiled_example.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven/xdi_writer.py` & `haven-spc-23.7.1/src/haven/xdi_writer.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/src/haven_spc.egg-info/PKG-INFO` & `haven-spc-23.7.1/src/haven_spc.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: haven-spc
-Version: 0.1.0
-Summary: Tools and applicatrion for running the spectroscopy group beamlines at the Advanced Photon Source.
+Version: 23.7.1
+Summary: Tools and GUI for running the spectroscopy group beamlines at the Advanced Photon Source.
 Author-email: Mark Wolfman <wolfman@anl.gov>
 Project-URL: Homepage, https://haven-spc.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/spc-group/haven/issues
 Keywords: synchrotron,xray,bluesky
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
@@ -26,32 +26,57 @@
 
 "Don't fly in anything with a Capissen 38 engine, they fall right out
 of the sky."
 
 
 ## Installation
 
-*haven* uses *mamba* for dependency management, and *poetry* for
-installation and development. First create the conda environment with
-mamba:
+### Python Packing Index
+
+Easiest way to install haven is using pip.
+
+```
+$ python -m pip install 'haven-spc'
+```
+
+### Development (Conda)
+
+*haven* can also use *mamba* for dependency management, and
+*setuptools* for installation and development. First create the conda
+environment with mamba:
 
 ```
 $ mamba env create -f environment.yml -n haven
 ```
 
-then install the package, with dependencies, in developer mode:
+then install the package, in developer mode:
 
 ```
 $ conda activate haven
-$ poetry install
+$ pip install -e .
 ```
 
 ## Running Tests
 
 To run tests, run
 
 ```
 $ pytest
 ```
 
 # firefly
-User-facing applications for controlling the beamlines managed by the spectroscopy group
+
+User-facing applications for controlling the beamlines managed by the
+spectroscopy group. Be sure to include the [gui] extras if you plan
+to use the GUI.
+
+```
+$ python -m pip install 'haven-spc[gui]'
+$ firefly
+```
+
+# Versioning
+
+Haven/Firefly uses calendar versioning, with short year and short
+month for the MAJOR and MINOR versions, then a incremental MICRO
+version. For example, version *23.7.2* is the 2nd (*2*) release in
+July (*7*) 2023 (*23*).
```

### Comparing `haven-spc-0.1.0/src/haven_spc.egg-info/SOURCES.txt` & `haven-spc-23.7.1/src/haven_spc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_align_motor.py` & `haven-spc-23.7.1/tests/test_align_motor.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_application.py` & `haven-spc-23.7.1/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_aps.py` & `haven-spc-23.7.1/tests/test_aps.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_area_detector_display.py` & `haven-spc-23.7.1/tests/test_area_detector_display.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_beam_properties.py` & `haven-spc-23.7.1/tests/test_beam_properties.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_bss_display.py` & `haven-spc-23.7.1/tests/test_bss_display.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_camera.py` & `haven-spc-23.7.1/tests/test_camera.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_cameras_display.py` & `haven-spc-23.7.1/tests/test_cameras_display.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_energy_display.py` & `haven-spc-23.7.1/tests/test_energy_display.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_energy_positioner.py` & `haven-spc-23.7.1/tests/test_energy_positioner.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_energy_ranges.py` & `haven-spc-23.7.1/tests/test_energy_ranges.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_fluorescence.py` & `haven-spc-23.7.1/tests/test_fluorescence.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_heater.py` & `haven-spc-23.7.1/tests/test_heater.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_iconfig.py` & `haven-spc-23.7.1/tests/test_iconfig.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_instrument_registry.py` & `haven-spc-23.7.1/tests/test_instrument_registry.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_ion_chamber.py` & `haven-spc-23.7.1/tests/test_ion_chamber.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_lerix.py` & `haven-spc-23.7.1/tests/test_lerix.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_main_window.py` & `haven-spc-23.7.1/tests/test_main_window.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_mono_ID_calibration_plan.py` & `haven-spc-23.7.1/tests/test_mono_ID_calibration_plan.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_motor.py` & `haven-spc-23.7.1/tests/test_motor.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_motor_menu.py` & `haven-spc-23.7.1/tests/test_motor_menu.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_ophyd_connection.py` & `haven-spc-23.7.1/tests/test_ophyd_connection.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_plans.py` & `haven-spc-23.7.1/tests/test_plans.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_preprocessors.py` & `haven-spc-23.7.1/tests/test_preprocessors.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_queue_client.py` & `haven-spc-23.7.1/tests/test_queue_client.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_run_browser.py` & `haven-spc-23.7.1/tests/test_run_browser.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_run_engine.py` & `haven-spc-23.7.1/tests/test_run_engine.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_save_motor_positions.py` & `haven-spc-23.7.1/tests/test_save_motor_positions.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_scaler_triggering.py` & `haven-spc-23.7.1/tests/test_scaler_triggering.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_set_energy.py` & `haven-spc-23.7.1/tests/test_set_energy.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_shutter.py` & `haven-spc-23.7.1/tests/test_shutter.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_simulated_ioc.py` & `haven-spc-23.7.1/tests/test_simulated_ioc.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_stages.py` & `haven-spc-23.7.1/tests/test_stages.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_voltmeters.py` & `haven-spc-23.7.1/tests/test_voltmeters.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_xafs_scan.py` & `haven-spc-23.7.1/tests/test_xafs_scan.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_xdi_writer.py` & `haven-spc-23.7.1/tests/test_xdi_writer.py`

 * *Files identical despite different names*

### Comparing `haven-spc-0.1.0/tests/test_xrf_detector_display.py` & `haven-spc-23.7.1/tests/test_xrf_detector_display.py`

 * *Files identical despite different names*

