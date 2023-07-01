# Comparing `tmp/pycatalicism-2.0.1.tar.gz` & `tmp/pycatalicism-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycatalicism-2.0.1.tar", last modified: Sun Jun 25 17:08:41 2023, max compression
+gzip compressed data, was "pycatalicism-2.0.2.tar", last modified: Sat Jul  1 11:10:21 2023, max compression
```

## Comparing `pycatalicism-2.0.1.tar` & `pycatalicism-2.0.2.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-06-25 17:08:41.781925 pycatalicism-2.0.1/
--rw-rw-r--   0 d         (1000) d         (1000)    33826 2023-06-25 17:08:41.781925 pycatalicism-2.0.1/PKG-INFO
--rw-rw-r--   0 d         (1000) d         (1000)    33353 2023-06-25 16:59:43.000000 pycatalicism-2.0.1/README.md
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-06-25 17:08:41.769925 pycatalicism-2.0.1/pycatalicism/
--rw-rw-r--   0 d         (1000) d         (1000)        0 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/__init__.py
--rw-rw-r--   0 d         (1000) d         (1000)     3167 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/activation_config.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-06-25 17:08:41.777925 pycatalicism-2.0.1/pycatalicism/calc/
--rw-rw-r--   0 d         (1000) d         (1000)        0 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/__init__.py
--rw-rw-r--   0 d         (1000) d         (1000)      255 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/activity.py
--rw-rw-r--   0 d         (1000) d         (1000)     3994 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/calc.py
--rw-rw-r--   0 d         (1000) d         (1000)     2423 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/calculator.py
--rw-rw-r--   0 d         (1000) d         (1000)     1458 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/calculator_factory.py
--rw-rw-r--   0 d         (1000) d         (1000)       97 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/calculatorexception.py
--rw-rw-r--   0 d         (1000) d         (1000)     8320 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/chromatec_crystal_composition_copy_paste_parser.py
--rw-rw-r--   0 d         (1000) d         (1000)     3348 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/co2_hydrogenation_exporter.py
--rw-rw-r--   0 d         (1000) d         (1000)     6353 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/co2_hydrogenation_plotter.py
--rw-rw-r--   0 d         (1000) d         (1000)     5972 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/co2hydrogenationcalculator.py
--rw-rw-r--   0 d         (1000) d         (1000)     4311 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/co2hydrogenationproductsbasiscalculator.py
--rw-rw-r--   0 d         (1000) d         (1000)     2468 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/co_oxidation_exporter.py
--rw-rw-r--   0 d         (1000) d         (1000)     2662 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/co_oxidation_plotter.py
--rw-rw-r--   0 d         (1000) d         (1000)     2541 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/conversion.py
--rw-rw-r--   0 d         (1000) d         (1000)     3412 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/cooxidationcalculator.py
--rw-rw-r--   0 d         (1000) d         (1000)     1027 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/exporter.py
--rw-rw-r--   0 d         (1000) d         (1000)     1013 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/exporter_factory.py
--rw-rw-r--   0 d         (1000) d         (1000)      103 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/exporterexception.py
--rw-rw-r--   0 d         (1000) d         (1000)      903 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/parser.py
--rw-rw-r--   0 d         (1000) d         (1000)      837 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/parser_factory.py
--rw-rw-r--   0 d         (1000) d         (1000)       98 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/parserexception.py
--rw-rw-r--   0 d         (1000) d         (1000)     1117 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/plotter.py
--rw-rw-r--   0 d         (1000) d         (1000)      970 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/plotter_factory.py
--rw-rw-r--   0 d         (1000) d         (1000)       84 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/plotterexception.py
--rw-rw-r--   0 d         (1000) d         (1000)     8075 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/rawdata.py
--rw-rw-r--   0 d         (1000) d         (1000)     4674 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/calc/selectivity.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-06-25 17:08:41.777925 pycatalicism-2.0.1/pycatalicism/chromatograph/
--rw-rw-r--   0 d         (1000) d         (1000)        0 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/chromatograph/__init__.py
--rw-rw-r--   0 d         (1000) d         (1000)     6738 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/chromatograph/chromatec_analytic_modbus.py
--rw-rw-r--   0 d         (1000) d         (1000)     8950 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/chromatograph/chromatec_control_panel_modbus.py
--rw-rw-r--   0 d         (1000) d         (1000)    10008 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/chromatograph/chromatec_crystal_5000.py
--rw-rw-r--   0 d         (1000) d         (1000)      214 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/chromatograph/chromatograph_exceptions.py
--rw-rw-r--   0 d         (1000) d         (1000)      817 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/chromatograph/chromatograph_logging.py
--rw-rw-r--   0 d         (1000) d         (1000)      392 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/chromatograph/logging_config.py
--rw-rw-r--   0 d         (1000) d         (1000)     3679 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/chromatograph/modbus_converter.py
--rw-rw-r--   0 d         (1000) d         (1000)     6211 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/config.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-06-25 17:08:41.777925 pycatalicism-2.0.1/pycatalicism/furnace/
--rw-rw-r--   0 d         (1000) d         (1000)        0 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/furnace/__init__.py
--rw-rw-r--   0 d         (1000) d         (1000)      317 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/furnace/furnace_exceptions.py
--rw-rw-r--   0 d         (1000) d         (1000)      814 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/furnace/furnace_logging.py
--rw-rw-r--   0 d         (1000) d         (1000)      201 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/furnace/logging_config.py
--rw-rw-r--   0 d         (1000) d         (1000)    27681 2023-06-25 16:59:43.000000 pycatalicism-2.0.1/pycatalicism/furnace/owen_protocol.py
--rw-rw-r--   0 d         (1000) d         (1000)     3566 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/furnace/owen_tmp101.py
--rw-rw-r--   0 d         (1000) d         (1000)     1884 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/init_conc_config.py
--rw-rw-r--   0 d         (1000) d         (1000)     3453 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/logging_decorator.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-06-25 17:08:41.777925 pycatalicism-2.0.1/pycatalicism/mass_flow_controller/
--rw-rw-r--   0 d         (1000) d         (1000)        0 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/mass_flow_controller/__init__.py
--rw-rw-r--   0 d         (1000) d         (1000)     6373 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/mass_flow_controller/bronkhorst_f201cv.py
--rw-rw-r--   0 d         (1000) d         (1000)     1385 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/mass_flow_controller/bronkhorst_mfc_calibration.py
--rw-rw-r--   0 d         (1000) d         (1000)      160 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/mass_flow_controller/logging_config.py
--rw-rw-r--   0 d         (1000) d         (1000)      874 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/mass_flow_controller/mass_flow_controller_logging.py
--rw-rw-r--   0 d         (1000) d         (1000)      240 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/mass_flow_controller/mfc_exceptions.py
--rw-rw-r--   0 d         (1000) d         (1000)     2124 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/measurement_config.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-06-25 17:08:41.781925 pycatalicism-2.0.1/pycatalicism/plotters/
--rw-rw-r--   0 d         (1000) d         (1000)        0 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/plotters/__init__.py
--rw-rw-r--   0 d         (1000) d         (1000)     1764 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/plotters/data.py
--rw-rw-r--   0 d         (1000) d         (1000)     4662 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/plotters/non_blocking_plotter.py
--rw-rw-r--   0 d         (1000) d         (1000)     1124 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/plotters/point.py
--rw-rw-r--   0 d         (1000) d         (1000)     4261 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/plotters/process_plotter.py
--rw-rw-r--   0 d         (1000) d         (1000)    36180 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/pycat.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-06-25 17:08:41.781925 pycatalicism-2.0.1/pycatalicism/valves/
--rw-rw-r--   0 d         (1000) d         (1000)        0 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/valves/__init__.py
--rw-rw-r--   0 d         (1000) d         (1000)     7381 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/valves/arduino_valve_controller.py
--rw-rw-r--   0 d         (1000) d         (1000)      155 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/valves/logging_config.py
--rw-rw-r--   0 d         (1000) d         (1000)     1163 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/valves/valves_exceptions.py
--rw-rw-r--   0 d         (1000) d         (1000)      860 2023-06-20 09:38:25.000000 pycatalicism-2.0.1/pycatalicism/valves/valves_logging.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-06-25 17:08:41.769925 pycatalicism-2.0.1/pycatalicism.egg-info/
--rw-rw-r--   0 d         (1000) d         (1000)    33826 2023-06-25 17:08:41.000000 pycatalicism-2.0.1/pycatalicism.egg-info/PKG-INFO
--rw-rw-r--   0 d         (1000) d         (1000)     2799 2023-06-25 17:08:41.000000 pycatalicism-2.0.1/pycatalicism.egg-info/SOURCES.txt
--rw-rw-r--   0 d         (1000) d         (1000)        1 2023-06-25 17:08:41.000000 pycatalicism-2.0.1/pycatalicism.egg-info/dependency_links.txt
--rw-rw-r--   0 d         (1000) d         (1000)       50 2023-06-25 17:08:41.000000 pycatalicism-2.0.1/pycatalicism.egg-info/entry_points.txt
--rw-rw-r--   0 d         (1000) d         (1000)       90 2023-06-25 17:08:41.000000 pycatalicism-2.0.1/pycatalicism.egg-info/requires.txt
--rw-rw-r--   0 d         (1000) d         (1000)       13 2023-06-25 17:08:41.000000 pycatalicism-2.0.1/pycatalicism.egg-info/top_level.txt
--rw-rw-r--   0 d         (1000) d         (1000)       38 2023-06-25 17:08:41.781925 pycatalicism-2.0.1/setup.cfg
--rw-rw-r--   0 d         (1000) d         (1000)     1099 2023-06-25 16:59:43.000000 pycatalicism-2.0.1/setup.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-07-01 11:10:21.689416 pycatalicism-2.0.2/
+-rw-rw-r--   0 d         (1000) d         (1000)    34124 2023-07-01 11:10:21.689416 pycatalicism-2.0.2/PKG-INFO
+-rw-rw-r--   0 d         (1000) d         (1000)    33651 2023-07-01 11:07:09.000000 pycatalicism-2.0.2/README.md
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-07-01 11:10:21.673416 pycatalicism-2.0.2/pycatalicism/
+-rw-rw-r--   0 d         (1000) d         (1000)        0 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)     3167 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/activation_config.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-07-01 11:10:21.681416 pycatalicism-2.0.2/pycatalicism/calc/
+-rw-rw-r--   0 d         (1000) d         (1000)        0 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/calc/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)      255 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/calc/activity.py
+-rw-rw-r--   0 d         (1000) d         (1000)     3994 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/calc/calc.py
+-rw-rw-r--   0 d         (1000) d         (1000)     2423 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/calc/calculator.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1458 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/calc/calculator_factory.py
+-rw-rw-r--   0 d         (1000) d         (1000)       97 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/calc/calculatorexception.py
+-rw-rw-r--   0 d         (1000) d         (1000)     8558 2023-07-01 11:07:09.000000 pycatalicism-2.0.2/pycatalicism/calc/chromatec_crystal_composition_copy_paste_parser.py
+-rw-rw-r--   0 d         (1000) d         (1000)     3348 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/calc/co2_hydrogenation_exporter.py
+-rw-rw-r--   0 d         (1000) d         (1000)     6353 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/calc/co2_hydrogenation_plotter.py
+-rw-rw-r--   0 d         (1000) d         (1000)     5972 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/calc/co2hydrogenationcalculator.py
+-rw-rw-r--   0 d         (1000) d         (1000)     4311 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/calc/co2hydrogenationproductsbasiscalculator.py
+-rw-rw-r--   0 d         (1000) d         (1000)     2468 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/calc/co_oxidation_exporter.py
+-rw-rw-r--   0 d         (1000) d         (1000)     2662 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/calc/co_oxidation_plotter.py
+-rw-rw-r--   0 d         (1000) d         (1000)     2541 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/calc/conversion.py
+-rw-rw-r--   0 d         (1000) d         (1000)     3412 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/calc/cooxidationcalculator.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1027 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/calc/exporter.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1013 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/calc/exporter_factory.py
+-rw-rw-r--   0 d         (1000) d         (1000)      103 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/calc/exporterexception.py
+-rw-rw-r--   0 d         (1000) d         (1000)      903 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/calc/parser.py
+-rw-rw-r--   0 d         (1000) d         (1000)      837 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/calc/parser_factory.py
+-rw-rw-r--   0 d         (1000) d         (1000)       98 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/calc/parserexception.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1117 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/calc/plotter.py
+-rw-rw-r--   0 d         (1000) d         (1000)      970 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/calc/plotter_factory.py
+-rw-rw-r--   0 d         (1000) d         (1000)       84 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/calc/plotterexception.py
+-rw-rw-r--   0 d         (1000) d         (1000)     8075 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/calc/rawdata.py
+-rw-rw-r--   0 d         (1000) d         (1000)     4674 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/calc/selectivity.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-07-01 11:10:21.681416 pycatalicism-2.0.2/pycatalicism/chromatograph/
+-rw-rw-r--   0 d         (1000) d         (1000)        0 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/chromatograph/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)     6738 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/chromatograph/chromatec_analytic_modbus.py
+-rw-rw-r--   0 d         (1000) d         (1000)     8950 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/chromatograph/chromatec_control_panel_modbus.py
+-rw-rw-r--   0 d         (1000) d         (1000)    10008 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/chromatograph/chromatec_crystal_5000.py
+-rw-rw-r--   0 d         (1000) d         (1000)      214 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/chromatograph/chromatograph_exceptions.py
+-rw-rw-r--   0 d         (1000) d         (1000)      817 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/chromatograph/chromatograph_logging.py
+-rw-rw-r--   0 d         (1000) d         (1000)      392 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/chromatograph/logging_config.py
+-rw-rw-r--   0 d         (1000) d         (1000)     3679 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/chromatograph/modbus_converter.py
+-rw-rw-r--   0 d         (1000) d         (1000)     6211 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/config.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-07-01 11:10:21.685416 pycatalicism-2.0.2/pycatalicism/furnace/
+-rw-rw-r--   0 d         (1000) d         (1000)        0 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/furnace/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)      317 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/furnace/furnace_exceptions.py
+-rw-rw-r--   0 d         (1000) d         (1000)      814 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/furnace/furnace_logging.py
+-rw-rw-r--   0 d         (1000) d         (1000)      201 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/furnace/logging_config.py
+-rw-rw-r--   0 d         (1000) d         (1000)    27681 2023-06-25 16:59:43.000000 pycatalicism-2.0.2/pycatalicism/furnace/owen_protocol.py
+-rw-rw-r--   0 d         (1000) d         (1000)     3566 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/furnace/owen_tmp101.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1884 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/init_conc_config.py
+-rw-rw-r--   0 d         (1000) d         (1000)     3453 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/logging_decorator.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-07-01 11:10:21.685416 pycatalicism-2.0.2/pycatalicism/mass_flow_controller/
+-rw-rw-r--   0 d         (1000) d         (1000)        0 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/mass_flow_controller/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)     6373 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/mass_flow_controller/bronkhorst_f201cv.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1385 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/mass_flow_controller/bronkhorst_mfc_calibration.py
+-rw-rw-r--   0 d         (1000) d         (1000)      160 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/mass_flow_controller/logging_config.py
+-rw-rw-r--   0 d         (1000) d         (1000)      874 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/mass_flow_controller/mass_flow_controller_logging.py
+-rw-rw-r--   0 d         (1000) d         (1000)      240 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/mass_flow_controller/mfc_exceptions.py
+-rw-rw-r--   0 d         (1000) d         (1000)     2124 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/measurement_config.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-07-01 11:10:21.685416 pycatalicism-2.0.2/pycatalicism/plotters/
+-rw-rw-r--   0 d         (1000) d         (1000)        0 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/plotters/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1764 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/plotters/data.py
+-rw-rw-r--   0 d         (1000) d         (1000)     4662 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/plotters/non_blocking_plotter.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1124 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/plotters/point.py
+-rw-rw-r--   0 d         (1000) d         (1000)     4261 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/plotters/process_plotter.py
+-rw-rw-r--   0 d         (1000) d         (1000)    36180 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/pycat.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-07-01 11:10:21.689416 pycatalicism-2.0.2/pycatalicism/valves/
+-rw-rw-r--   0 d         (1000) d         (1000)        0 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/valves/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)     7381 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/valves/arduino_valve_controller.py
+-rw-rw-r--   0 d         (1000) d         (1000)      155 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/valves/logging_config.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1163 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/valves/valves_exceptions.py
+-rw-rw-r--   0 d         (1000) d         (1000)      860 2023-06-20 09:38:25.000000 pycatalicism-2.0.2/pycatalicism/valves/valves_logging.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-07-01 11:10:21.673416 pycatalicism-2.0.2/pycatalicism.egg-info/
+-rw-rw-r--   0 d         (1000) d         (1000)    34124 2023-07-01 11:10:21.000000 pycatalicism-2.0.2/pycatalicism.egg-info/PKG-INFO
+-rw-rw-r--   0 d         (1000) d         (1000)     2799 2023-07-01 11:10:21.000000 pycatalicism-2.0.2/pycatalicism.egg-info/SOURCES.txt
+-rw-rw-r--   0 d         (1000) d         (1000)        1 2023-07-01 11:10:21.000000 pycatalicism-2.0.2/pycatalicism.egg-info/dependency_links.txt
+-rw-rw-r--   0 d         (1000) d         (1000)       50 2023-07-01 11:10:21.000000 pycatalicism-2.0.2/pycatalicism.egg-info/entry_points.txt
+-rw-rw-r--   0 d         (1000) d         (1000)       90 2023-07-01 11:10:21.000000 pycatalicism-2.0.2/pycatalicism.egg-info/requires.txt
+-rw-rw-r--   0 d         (1000) d         (1000)       13 2023-07-01 11:10:21.000000 pycatalicism-2.0.2/pycatalicism.egg-info/top_level.txt
+-rw-rw-r--   0 d         (1000) d         (1000)       38 2023-07-01 11:10:21.689416 pycatalicism-2.0.2/setup.cfg
+-rw-rw-r--   0 d         (1000) d         (1000)     1099 2023-07-01 11:07:09.000000 pycatalicism-2.0.2/setup.py
```

### Comparing `pycatalicism-2.0.1/PKG-INFO` & `pycatalicism-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycatalicism
-Version: 2.0.1
+Version: 2.0.2
 Summary: Program controls catalytic activity of materials measurement equipment as well as calculations
 Home-page: https://github.com/leybodv/pycatalicism
 Author: Denis Leybo
 Author-email: denis@leybo.xyz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,14 +30,15 @@
     <h3>Arch Linux</h3>
       <p>Установить python:</p>
       <p><code>pacman -S python</code></p>
       <p>Установить программу:</p>
       <p><code>pip install pycatalicism</code></p>
     <h3>Windows</h3>
       <p>Установить python отсюда: <a href="python.org">python.org</a></p>
+      <p>Установить <a href="https://www.microsoft.com/en-us/download/details.aspx?id=48145">Visual C++ Redistributable for Visual Studio 2015</a></p>
       <p>Установить программу:</p>
       <p><code>pip install pycatalicism</code></p>
       <p>Скачать и установить драйвер usb -> com отсюда: <a href="https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers">silabs.com</a></p>
   <h2 id="calc">Рассчёт характеристик катализаторов</h2>
     <p><code>pycat calc --conversion|--selectivity [--output-data OUTPUT_DATA] [--show-plot] [--output-plot OUPUT_PLOT] [--products-basis] [--sample-name SAMPLE_NAME] input-data-path initial-data-path {co-oxidation|co2-hydrogenation}</code></p>
     <p>Аргументы:</p>
     <table>
@@ -335,12 +336,14 @@
     </table>
   </p>
   <h2>ТуДу</h2>
     <ul>
       <li>переписать модуль calc: селективность должна рассчитываться автоматически, если это имеет смысл; должно быть 2 команды <code>calculate activity</code> и <code>calculate conversion</code></li>
       <li>автоматически конвертировать данные с газовых часов в СИ при рассчёте</li>
     </ul>
-    <h2 id="changes">Изменения в новых версиях</h2>
+  <h2 id="changes">Изменения в новых версиях</h2>
     <ul>
       <li>2.0.1</li>
       <p>Исправлена ошибка <a href="https://github.com/leybodv/pycatalicism/issues/19">issue 19</a></p>
+      <li>2.0.2</li>
+      <p>Исправлена ошибка <a href="https://github.com/leybodv/pycatalicism/issues/1">issue 1</a></p>
     </ul>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycatalicism Version: 2.0.1 Summary: Program
+Metadata-Version: 2.1 Name: pycatalicism Version: 2.0.2 Summary: Program
 controls catalytic activity of materials measurement equipment as well as
 calculations Home-page: https://github.com/leybodv/pycatalicism Author: Denis
 Leybo Author-email: denis@leybo.xyz Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >3.10.0 Description-Content-Type:
 text/markdown
 ****** pycatalicism ******
@@ -35,14 +35,15 @@
 **** Arch Linux ****
 Ð£ÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÑ python:
 pacman -S python
 Ð£ÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÑ Ð¿ÑÐ¾Ð³ÑÐ°Ð¼Ð¼Ñ:
 pip install pycatalicism
 **** Windows ****
 Ð£ÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÑ python Ð¾ÑÑÑÐ´Ð°: python.org
+Ð£ÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÑ Visual_C++_Redistributable_for_Visual_Studio_2015
 Ð£ÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÑ Ð¿ÑÐ¾Ð³ÑÐ°Ð¼Ð¼Ñ:
 pip install pycatalicism
 Ð¡ÐºÐ°ÑÐ°ÑÑ Ð¸ ÑÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÑ Ð´ÑÐ°Ð¹Ð²ÐµÑ usb -> com Ð¾ÑÑÑÐ´Ð°:
 silabs.com
 ***** Ð Ð°ÑÑÑÑÑ ÑÐ°ÑÐ°ÐºÑÐµÑÐ¸ÑÑÐ¸Ðº ÐºÐ°ÑÐ°Ð»Ð¸Ð·Ð°ÑÐ¾ÑÐ¾Ð²
 *****
 pycat calc --conversion|--selectivity [--output-data OUTPUT_DATA] [--show-plot]
@@ -395,7 +396,9 @@
       ÐµÑÐ»Ð¸ ÑÑÐ¾ Ð¸Ð¼ÐµÐµÑ ÑÐ¼ÑÑÐ»; Ð´Ð¾Ð»Ð¶Ð½Ð¾ Ð±ÑÑÑ 2
       ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ calculate activity Ð¸ calculate conversion
     * Ð°Ð²ÑÐ¾Ð¼Ð°ÑÐ¸ÑÐµÑÐºÐ¸ ÐºÐ¾Ð½Ð²ÐµÑÑÐ¸ÑÐ¾Ð²Ð°ÑÑ Ð´Ð°Ð½Ð½ÑÐµ Ñ
       Ð³Ð°Ð·Ð¾Ð²ÑÑ ÑÐ°ÑÐ¾Ð² Ð² Ð¡Ð Ð¿ÑÐ¸ ÑÐ°ÑÑÑÑÑÐµ
 ***** ÐÐ·Ð¼ÐµÐ½ÐµÐ½Ð¸Ñ Ð² Ð½Ð¾Ð²ÑÑ Ð²ÐµÑÑÐ¸ÑÑ *****
     * 2.0.1
       ÐÑÐ¿ÑÐ°Ð²Ð»ÐµÐ½Ð° Ð¾ÑÐ¸Ð±ÐºÐ° issue_19
+    * 2.0.2
+      ÐÑÐ¿ÑÐ°Ð²Ð»ÐµÐ½Ð° Ð¾ÑÐ¸Ð±ÐºÐ° issue_1
```

### Comparing `pycatalicism-2.0.1/README.md` & `pycatalicism-2.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     <h3>Arch Linux</h3>
       <p>Установить python:</p>
       <p><code>pacman -S python</code></p>
       <p>Установить программу:</p>
       <p><code>pip install pycatalicism</code></p>
     <h3>Windows</h3>
       <p>Установить python отсюда: <a href="python.org">python.org</a></p>
+      <p>Установить <a href="https://www.microsoft.com/en-us/download/details.aspx?id=48145">Visual C++ Redistributable for Visual Studio 2015</a></p>
       <p>Установить программу:</p>
       <p><code>pip install pycatalicism</code></p>
       <p>Скачать и установить драйвер usb -> com отсюда: <a href="https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers">silabs.com</a></p>
   <h2 id="calc">Рассчёт характеристик катализаторов</h2>
     <p><code>pycat calc --conversion|--selectivity [--output-data OUTPUT_DATA] [--show-plot] [--output-plot OUPUT_PLOT] [--products-basis] [--sample-name SAMPLE_NAME] input-data-path initial-data-path {co-oxidation|co2-hydrogenation}</code></p>
     <p>Аргументы:</p>
     <table>
@@ -322,12 +323,14 @@
     </table>
   </p>
   <h2>ТуДу</h2>
     <ul>
       <li>переписать модуль calc: селективность должна рассчитываться автоматически, если это имеет смысл; должно быть 2 команды <code>calculate activity</code> и <code>calculate conversion</code></li>
       <li>автоматически конвертировать данные с газовых часов в СИ при рассчёте</li>
     </ul>
-    <h2 id="changes">Изменения в новых версиях</h2>
+  <h2 id="changes">Изменения в новых версиях</h2>
     <ul>
       <li>2.0.1</li>
       <p>Исправлена ошибка <a href="https://github.com/leybodv/pycatalicism/issues/19">issue 19</a></p>
+      <li>2.0.2</li>
+      <p>Исправлена ошибка <a href="https://github.com/leybodv/pycatalicism/issues/1">issue 1</a></p>
     </ul>
```

#### html2text {}

```diff
@@ -28,14 +28,15 @@
 **** Arch Linux ****
 Ð£ÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÑ python:
 pacman -S python
 Ð£ÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÑ Ð¿ÑÐ¾Ð³ÑÐ°Ð¼Ð¼Ñ:
 pip install pycatalicism
 **** Windows ****
 Ð£ÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÑ python Ð¾ÑÑÑÐ´Ð°: python.org
+Ð£ÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÑ Visual_C++_Redistributable_for_Visual_Studio_2015
 Ð£ÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÑ Ð¿ÑÐ¾Ð³ÑÐ°Ð¼Ð¼Ñ:
 pip install pycatalicism
 Ð¡ÐºÐ°ÑÐ°ÑÑ Ð¸ ÑÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÑ Ð´ÑÐ°Ð¹Ð²ÐµÑ usb -> com Ð¾ÑÑÑÐ´Ð°:
 silabs.com
 ***** Ð Ð°ÑÑÑÑÑ ÑÐ°ÑÐ°ÐºÑÐµÑÐ¸ÑÑÐ¸Ðº ÐºÐ°ÑÐ°Ð»Ð¸Ð·Ð°ÑÐ¾ÑÐ¾Ð²
 *****
 pycat calc --conversion|--selectivity [--output-data OUTPUT_DATA] [--show-plot]
@@ -388,7 +389,9 @@
       ÐµÑÐ»Ð¸ ÑÑÐ¾ Ð¸Ð¼ÐµÐµÑ ÑÐ¼ÑÑÐ»; Ð´Ð¾Ð»Ð¶Ð½Ð¾ Ð±ÑÑÑ 2
       ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ calculate activity Ð¸ calculate conversion
     * Ð°Ð²ÑÐ¾Ð¼Ð°ÑÐ¸ÑÐµÑÐºÐ¸ ÐºÐ¾Ð½Ð²ÐµÑÑÐ¸ÑÐ¾Ð²Ð°ÑÑ Ð´Ð°Ð½Ð½ÑÐµ Ñ
       Ð³Ð°Ð·Ð¾Ð²ÑÑ ÑÐ°ÑÐ¾Ð² Ð² Ð¡Ð Ð¿ÑÐ¸ ÑÐ°ÑÑÑÑÑÐµ
 ***** ÐÐ·Ð¼ÐµÐ½ÐµÐ½Ð¸Ñ Ð² Ð½Ð¾Ð²ÑÑ Ð²ÐµÑÑÐ¸ÑÑ *****
     * 2.0.1
       ÐÑÐ¿ÑÐ°Ð²Ð»ÐµÐ½Ð° Ð¾ÑÐ¸Ð±ÐºÐ° issue_19
+    * 2.0.2
+      ÐÑÐ¿ÑÐ°Ð²Ð»ÐµÐ½Ð° Ð¾ÑÐ¸Ð±ÐºÐ° issue_1
```

### Comparing `pycatalicism-2.0.1/pycatalicism/activation_config.py` & `pycatalicism-2.0.2/pycatalicism/activation_config.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/calc/calc.py` & `pycatalicism-2.0.2/pycatalicism/calc/calc.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/calc/calculator.py` & `pycatalicism-2.0.2/pycatalicism/calc/calculator.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/calc/calculator_factory.py` & `pycatalicism-2.0.2/pycatalicism/calc/calculator_factory.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/calc/chromatec_crystal_composition_copy_paste_parser.py` & `pycatalicism-2.0.2/pycatalicism/calc/chromatec_crystal_composition_copy_paste_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,28 +62,30 @@
         exception:ParserException
             if initial_data_path is not file or if input_data_path is not directory
         """
         if not initial_data_path.is_file():
             raise ParserException(f'initial data path {initial_data_path} must be a file')
         if not input_data_path.is_dir():
             raise ParserException(f'input data path {input_data_path} must be a directory')
+        self.logger.info(f'Parsing file with initial data: {initial_data_path}')
         _, Cs_i, Ta_i, Pa_i, f_i = self._parse_file(initial_data_path)
         flow_is_measured = Ta_i and Pa_i and f_i
         Ts = []
         Cs_f = []
         Ta_f = [] if flow_is_measured else None
         Pa_f = [] if flow_is_measured else None
         f_f = [] if flow_is_measured else None
         for file in input_data_path.iterdir():
             if file == initial_data_path:
                 continue
             if file.is_dir():
                 self.logger.warning(f'Found directory {file} in input data path')
                 continue
             try:
+                self.logger.info(f'Parsing data file: {file}')
                 T, C, Ta, Pa, f = self._parse_file(file)
             except ParserException:
                 self.logger.warning(f'Wrong data format in file {file}. Skipping.')
                 continue
             Ts.append(T)
             Cs_f.append(C)
             if Ta_f is not None and Pa_f is not None and f_f is not None:
@@ -129,14 +131,15 @@
 
         raises
         ------
         exception:ParserException
             if data format is wrong
         """
         try:
+            self.logger.debug(f'Replacing commas with dots in file: {path}')
             file_contents = self._replace_commas_with_dots(path)
         except UnicodeDecodeError:
             raise ParserException(f'Non unicode file {path}')
         T = None
         C = {}
         Ta = None
         Pa = None
@@ -183,11 +186,11 @@
                 path to file for processing
 
         returns
         -------
             new_contents:str
                 string with file contents in which commas were replaced with dots
         """
-        with path.open(mode='r') as file:
+        with path.open(mode='r', encoding='utf8') as file:
             contents = file.read()
             new_contents = contents.replace(',', '.')
         return new_contents
```

### Comparing `pycatalicism-2.0.1/pycatalicism/calc/co2_hydrogenation_exporter.py` & `pycatalicism-2.0.2/pycatalicism/calc/co2_hydrogenation_exporter.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/calc/co2_hydrogenation_plotter.py` & `pycatalicism-2.0.2/pycatalicism/calc/co2_hydrogenation_plotter.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/calc/co2hydrogenationcalculator.py` & `pycatalicism-2.0.2/pycatalicism/calc/co2hydrogenationcalculator.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/calc/co2hydrogenationproductsbasiscalculator.py` & `pycatalicism-2.0.2/pycatalicism/calc/co2hydrogenationproductsbasiscalculator.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/calc/co_oxidation_exporter.py` & `pycatalicism-2.0.2/pycatalicism/calc/co_oxidation_exporter.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/calc/co_oxidation_plotter.py` & `pycatalicism-2.0.2/pycatalicism/calc/co_oxidation_plotter.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/calc/conversion.py` & `pycatalicism-2.0.2/pycatalicism/calc/conversion.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/calc/cooxidationcalculator.py` & `pycatalicism-2.0.2/pycatalicism/calc/cooxidationcalculator.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/calc/exporter.py` & `pycatalicism-2.0.2/pycatalicism/calc/exporter.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/calc/exporter_factory.py` & `pycatalicism-2.0.2/pycatalicism/calc/exporter_factory.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/calc/parser.py` & `pycatalicism-2.0.2/pycatalicism/calc/parser.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/calc/parser_factory.py` & `pycatalicism-2.0.2/pycatalicism/calc/parser_factory.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/calc/plotter.py` & `pycatalicism-2.0.2/pycatalicism/calc/plotter.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/calc/plotter_factory.py` & `pycatalicism-2.0.2/pycatalicism/calc/plotter_factory.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/calc/rawdata.py` & `pycatalicism-2.0.2/pycatalicism/calc/rawdata.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/calc/selectivity.py` & `pycatalicism-2.0.2/pycatalicism/calc/selectivity.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/chromatograph/chromatec_analytic_modbus.py` & `pycatalicism-2.0.2/pycatalicism/chromatograph/chromatec_analytic_modbus.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/chromatograph/chromatec_control_panel_modbus.py` & `pycatalicism-2.0.2/pycatalicism/chromatograph/chromatec_control_panel_modbus.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/chromatograph/chromatec_crystal_5000.py` & `pycatalicism-2.0.2/pycatalicism/chromatograph/chromatec_crystal_5000.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/chromatograph/chromatograph_logging.py` & `pycatalicism-2.0.2/pycatalicism/chromatograph/chromatograph_logging.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/chromatograph/modbus_converter.py` & `pycatalicism-2.0.2/pycatalicism/chromatograph/modbus_converter.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/config.py` & `pycatalicism-2.0.2/pycatalicism/config.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/furnace/furnace_logging.py` & `pycatalicism-2.0.2/pycatalicism/furnace/furnace_logging.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/furnace/owen_protocol.py` & `pycatalicism-2.0.2/pycatalicism/furnace/owen_protocol.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/furnace/owen_tmp101.py` & `pycatalicism-2.0.2/pycatalicism/furnace/owen_tmp101.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/init_conc_config.py` & `pycatalicism-2.0.2/pycatalicism/init_conc_config.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/logging_decorator.py` & `pycatalicism-2.0.2/pycatalicism/logging_decorator.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/mass_flow_controller/bronkhorst_f201cv.py` & `pycatalicism-2.0.2/pycatalicism/mass_flow_controller/bronkhorst_f201cv.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/mass_flow_controller/bronkhorst_mfc_calibration.py` & `pycatalicism-2.0.2/pycatalicism/mass_flow_controller/bronkhorst_mfc_calibration.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/mass_flow_controller/mass_flow_controller_logging.py` & `pycatalicism-2.0.2/pycatalicism/mass_flow_controller/mass_flow_controller_logging.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/measurement_config.py` & `pycatalicism-2.0.2/pycatalicism/measurement_config.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/plotters/data.py` & `pycatalicism-2.0.2/pycatalicism/plotters/data.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/plotters/non_blocking_plotter.py` & `pycatalicism-2.0.2/pycatalicism/plotters/non_blocking_plotter.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/plotters/point.py` & `pycatalicism-2.0.2/pycatalicism/plotters/point.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/plotters/process_plotter.py` & `pycatalicism-2.0.2/pycatalicism/plotters/process_plotter.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/pycat.py` & `pycatalicism-2.0.2/pycatalicism/pycat.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/valves/arduino_valve_controller.py` & `pycatalicism-2.0.2/pycatalicism/valves/arduino_valve_controller.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/valves/valves_exceptions.py` & `pycatalicism-2.0.2/pycatalicism/valves/valves_exceptions.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism/valves/valves_logging.py` & `pycatalicism-2.0.2/pycatalicism/valves/valves_logging.py`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/pycatalicism.egg-info/PKG-INFO` & `pycatalicism-2.0.2/pycatalicism.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycatalicism
-Version: 2.0.1
+Version: 2.0.2
 Summary: Program controls catalytic activity of materials measurement equipment as well as calculations
 Home-page: https://github.com/leybodv/pycatalicism
 Author: Denis Leybo
 Author-email: denis@leybo.xyz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,14 +30,15 @@
     <h3>Arch Linux</h3>
       <p>Установить python:</p>
       <p><code>pacman -S python</code></p>
       <p>Установить программу:</p>
       <p><code>pip install pycatalicism</code></p>
     <h3>Windows</h3>
       <p>Установить python отсюда: <a href="python.org">python.org</a></p>
+      <p>Установить <a href="https://www.microsoft.com/en-us/download/details.aspx?id=48145">Visual C++ Redistributable for Visual Studio 2015</a></p>
       <p>Установить программу:</p>
       <p><code>pip install pycatalicism</code></p>
       <p>Скачать и установить драйвер usb -> com отсюда: <a href="https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers">silabs.com</a></p>
   <h2 id="calc">Рассчёт характеристик катализаторов</h2>
     <p><code>pycat calc --conversion|--selectivity [--output-data OUTPUT_DATA] [--show-plot] [--output-plot OUPUT_PLOT] [--products-basis] [--sample-name SAMPLE_NAME] input-data-path initial-data-path {co-oxidation|co2-hydrogenation}</code></p>
     <p>Аргументы:</p>
     <table>
@@ -335,12 +336,14 @@
     </table>
   </p>
   <h2>ТуДу</h2>
     <ul>
       <li>переписать модуль calc: селективность должна рассчитываться автоматически, если это имеет смысл; должно быть 2 команды <code>calculate activity</code> и <code>calculate conversion</code></li>
       <li>автоматически конвертировать данные с газовых часов в СИ при рассчёте</li>
     </ul>
-    <h2 id="changes">Изменения в новых версиях</h2>
+  <h2 id="changes">Изменения в новых версиях</h2>
     <ul>
       <li>2.0.1</li>
       <p>Исправлена ошибка <a href="https://github.com/leybodv/pycatalicism/issues/19">issue 19</a></p>
+      <li>2.0.2</li>
+      <p>Исправлена ошибка <a href="https://github.com/leybodv/pycatalicism/issues/1">issue 1</a></p>
     </ul>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycatalicism Version: 2.0.1 Summary: Program
+Metadata-Version: 2.1 Name: pycatalicism Version: 2.0.2 Summary: Program
 controls catalytic activity of materials measurement equipment as well as
 calculations Home-page: https://github.com/leybodv/pycatalicism Author: Denis
 Leybo Author-email: denis@leybo.xyz Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >3.10.0 Description-Content-Type:
 text/markdown
 ****** pycatalicism ******
@@ -35,14 +35,15 @@
 **** Arch Linux ****
 Ð£ÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÑ python:
 pacman -S python
 Ð£ÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÑ Ð¿ÑÐ¾Ð³ÑÐ°Ð¼Ð¼Ñ:
 pip install pycatalicism
 **** Windows ****
 Ð£ÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÑ python Ð¾ÑÑÑÐ´Ð°: python.org
+Ð£ÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÑ Visual_C++_Redistributable_for_Visual_Studio_2015
 Ð£ÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÑ Ð¿ÑÐ¾Ð³ÑÐ°Ð¼Ð¼Ñ:
 pip install pycatalicism
 Ð¡ÐºÐ°ÑÐ°ÑÑ Ð¸ ÑÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÑ Ð´ÑÐ°Ð¹Ð²ÐµÑ usb -> com Ð¾ÑÑÑÐ´Ð°:
 silabs.com
 ***** Ð Ð°ÑÑÑÑÑ ÑÐ°ÑÐ°ÐºÑÐµÑÐ¸ÑÑÐ¸Ðº ÐºÐ°ÑÐ°Ð»Ð¸Ð·Ð°ÑÐ¾ÑÐ¾Ð²
 *****
 pycat calc --conversion|--selectivity [--output-data OUTPUT_DATA] [--show-plot]
@@ -395,7 +396,9 @@
       ÐµÑÐ»Ð¸ ÑÑÐ¾ Ð¸Ð¼ÐµÐµÑ ÑÐ¼ÑÑÐ»; Ð´Ð¾Ð»Ð¶Ð½Ð¾ Ð±ÑÑÑ 2
       ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ calculate activity Ð¸ calculate conversion
     * Ð°Ð²ÑÐ¾Ð¼Ð°ÑÐ¸ÑÐµÑÐºÐ¸ ÐºÐ¾Ð½Ð²ÐµÑÑÐ¸ÑÐ¾Ð²Ð°ÑÑ Ð´Ð°Ð½Ð½ÑÐµ Ñ
       Ð³Ð°Ð·Ð¾Ð²ÑÑ ÑÐ°ÑÐ¾Ð² Ð² Ð¡Ð Ð¿ÑÐ¸ ÑÐ°ÑÑÑÑÑÐµ
 ***** ÐÐ·Ð¼ÐµÐ½ÐµÐ½Ð¸Ñ Ð² Ð½Ð¾Ð²ÑÑ Ð²ÐµÑÑÐ¸ÑÑ *****
     * 2.0.1
       ÐÑÐ¿ÑÐ°Ð²Ð»ÐµÐ½Ð° Ð¾ÑÐ¸Ð±ÐºÐ° issue_19
+    * 2.0.2
+      ÐÑÐ¿ÑÐ°Ð²Ð»ÐµÐ½Ð° Ð¾ÑÐ¸Ð±ÐºÐ° issue_1
```

### Comparing `pycatalicism-2.0.1/pycatalicism.egg-info/SOURCES.txt` & `pycatalicism-2.0.2/pycatalicism.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycatalicism-2.0.1/setup.py` & `pycatalicism-2.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "pyserial>=3.5",
     "pymodbus>=2.5.3,<2.6",
     "bronkhorst-propar>=1.0",
     ]
 
 setuptools.setup(
      name='pycatalicism',
-     version='2.0.1',
+     version='2.0.2',
      author="Denis Leybo",
      author_email="denis@leybo.xyz",
      description="Program controls catalytic activity of materials measurement equipment as well as calculations",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/leybodv/pycatalicism",
      packages=setuptools.find_packages(),
```

