# Comparing `tmp/dispatches-1.2.0rc1.tar.gz` & `tmp/dispatches-1.3.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dispatches-1.2.0rc1.tar", last modified: Wed Apr  5 15:38:31 2023, max compression
+gzip compressed data, was "dispatches-1.3.0rc0.tar", last modified: Sat Jul  1 01:16:15 2023, max compression
```

## Comparing `dispatches-1.2.0rc1.tar` & `dispatches-1.3.0rc0.tar`

### file list

```diff
@@ -1,140 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:38:31.619723 dispatches-1.2.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-05 15:38:31.619723 dispatches-1.2.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:38:31.579721 dispatches-1.2.0rc1/dispatches/
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:38:31.579721 dispatches-1.2.0rc1/dispatches/case_studies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:38:31.579721 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:38:31.579721 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/supercritical_plant/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/supercritical_plant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46868 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/supercritical_plant/supercritical_powerplant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:38:31.579721 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/supercritical_plant/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/supercritical_plant/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/supercritical_plant/tests/test_scpc_flowsheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:38:31.579721 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   298229 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/pfd_ultra_supercritical_pc.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:38:31.583721 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   111391 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/charge_design_ultra_supercritical_power_plant.py
--rw-r--r--   0 runner    (1001) docker     (123)    50372 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/discharge_design_ultra_supercritical_power_plant.py
--rw-r--r--   0 runner    (1001) docker     (123)  2330804 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/initialized_integrated_storage_usc.json
--rw-r--r--   0 runner    (1001) docker     (123)    54649 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/integrated_storage_with_ultrasupercritical_power_plant.py
--rw-r--r--   0 runner    (1001) docker     (123)    14951 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/multiperiod_double_loop_usc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12754 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/multiperiod_integrated_storage_usc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16166 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/pricetaker_with_multiperiod_integrated_storage_usc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:38:31.587721 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/tests/test_charge_usc_powerplant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/tests/test_discharge_usc_powerplant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/tests/test_integrated_storage_with_ultrasupercritical_power_plant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/tests/test_multiperiod_integrated_storage_usc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:38:31.587721 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/tests/test_usc_powerplant.py
--rw-r--r--   0 runner    (1001) docker     (123)    51228 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/ultra_supercritical_powerplant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:38:31.591721 dispatches-1.2.0rc1/dispatches/case_studies/nuclear_case/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/nuclear_case/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  2921488 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/nuclear_case/lmp_signal.json
--rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/nuclear_case/nuclear_flowsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11459 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/nuclear_case/nuclear_flowsheet_multiperiod_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:38:31.591721 dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/
--rw-r--r--   0 runner    (1001) docker     (123)    20939 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/RE_flowsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:38:31.603722 dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1819947 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/data/309_WIND_1-SimulationOutputs.csv
--rw-r--r--   0 runner    (1001) docker     (123)   191554 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/data/44.21_-101.94_windtoolkit_2012_60min_80m.srw
--rw-r--r--   0 runner    (1001) docker     (123)  7076855 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/data/Wind_Thermal_Dispatch.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10869 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/double_loop_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/load_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/run_double_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:38:31.603722 dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   140032 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/tests/rts_results_all_prices.npy
--rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/tests/test_RE_flowsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/tests/test_multiperiod_wind_battery_doubleloop.py
--rw-r--r--   0 runner    (1001) docker     (123)    14883 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/wind_battery_LMP.py
--rw-r--r--   0 runner    (1001) docker     (123)    17388 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/wind_battery_PEM_LMP.py
--rw-r--r--   0 runner    (1001) docker     (123)    27433 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/wind_battery_PEM_tank_turbine_LMP.py
--rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/wind_battery_double_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:38:31.603722 dispatches-1.2.0rc1/dispatches/properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/properties/h2_ideal_vap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/properties/h2_reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    16153 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/properties/hitecsalt_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/properties/hturbine_ideal_vap.py
--rw-r--r--   0 runner    (1001) docker     (123)    16216 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/properties/solarsalt_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:38:31.603722 dispatches-1.2.0rc1/dispatches/properties/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/properties/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/properties/tests/test_h2_ideal_vap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/properties/tests/test_hitecsalt_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/properties/tests/test_solarsalt_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/properties/tests/test_thermaloil_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/properties/thermaloil_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:38:31.603722 dispatches-1.2.0rc1/dispatches/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:38:31.603722 dispatches-1.2.0rc1/dispatches/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/tests/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:38:31.615723 dispatches-1.2.0rc1/dispatches/tests/data/prescient_5bus/
--rw-r--r--   0 runner    (1001) docker     (123)   231999 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/tests/data/prescient_5bus/DAY_AHEAD_load.csv
--rw-r--r--   0 runner    (1001) docker     (123)   269139 2023-04-05 15:37:11.000000 dispatches-1.2.0rc1/dispatches/tests/data/prescient_5bus/DAY_AHEAD_renewables.csv
--rw-r--r--   0 runner    (1001) docker     (123)  2888100 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/tests/data/prescient_5bus/REAL_TIME_load.csv
--rw-r--r--   0 runner    (1001) docker     (123)  3641364 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/tests/data/prescient_5bus/REAL_TIME_renewables.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/tests/data/prescient_5bus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/tests/data/prescient_5bus/branch.csv
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/tests/data/prescient_5bus/bus.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/tests/data/prescient_5bus/gen.csv
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/tests/data/prescient_5bus/initial_status.csv
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/tests/data/prescient_5bus/reserves.csv
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/tests/data/prescient_5bus/simulation_objects.csv
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/tests/data/prescient_5bus/timeseries_pointers.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/tests/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/tests/test_prescient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:38:31.615723 dispatches-1.2.0rc1/dispatches/unit_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/unit_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10778 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/unit_models/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)    39163 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/unit_models/concrete_tes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/unit_models/elec_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16798 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/unit_models/heat_exchanger_tube.py
--rw-r--r--   0 runner    (1001) docker     (123)    26308 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/unit_models/hydrogen_tank.py
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/unit_models/hydrogen_tank_simplified.py
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/unit_models/hydrogen_turbine_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/unit_models/pem_electrolyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:38:31.615723 dispatches-1.2.0rc1/dispatches/unit_models/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/unit_models/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/unit_models/tests/test_battery.py
--rw-r--r--   0 runner    (1001) docker     (123)    26496 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/unit_models/tests/test_concrete_tes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/unit_models/tests/test_elec_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/unit_models/tests/test_heat_exchanger_tube.py
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/unit_models/tests/test_hydrogen_tank.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/unit_models/tests/test_hydrogen_tank_simplified.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/unit_models/tests/test_hydrogen_turbine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/unit_models/tests/test_pem_electrolyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/unit_models/tests/test_wind_power.py
--rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/unit_models/wind_power.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:38:31.615723 dispatches-1.2.0rc1/dispatches/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/util/syn_hist_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/util/syn_hist_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/util/teal_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:38:31.619723 dispatches-1.2.0rc1/dispatches/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/workflow/coordinator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/workflow/rts_gmlc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:38:31.619723 dispatches-1.2.0rc1/dispatches/workflow/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/workflow/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/workflow/tests/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/dispatches/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:38:31.579721 dispatches-1.2.0rc1/dispatches.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-05 15:38:31.000000 dispatches-1.2.0rc1/dispatches.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-04-05 15:38:31.000000 dispatches-1.2.0rc1/dispatches.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 15:38:31.000000 dispatches-1.2.0rc1/dispatches.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-05 15:38:31.000000 dispatches-1.2.0rc1/dispatches.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-05 15:38:31.000000 dispatches-1.2.0rc1/dispatches.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 15:38:31.619723 dispatches-1.2.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-04-05 15:37:12.000000 dispatches-1.2.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:16:15.481856 dispatches-1.3.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-01 01:14:49.000000 dispatches-1.3.0rc0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-01 01:16:15.481856 dispatches-1.3.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-07-01 01:14:49.000000 dispatches-1.3.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:16:15.441856 dispatches-1.3.0rc0/dispatches/
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-01 01:14:49.000000 dispatches-1.3.0rc0/dispatches/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:16:15.441856 dispatches-1.3.0rc0/dispatches/case_studies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 01:14:49.000000 dispatches-1.3.0rc0/dispatches/case_studies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:16:15.445856 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 01:14:49.000000 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:16:15.445856 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/supercritical_plant/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 01:14:49.000000 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/supercritical_plant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46868 2023-07-01 01:14:49.000000 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/supercritical_plant/supercritical_powerplant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:16:15.445856 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/supercritical_plant/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 01:14:49.000000 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/supercritical_plant/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-01 01:14:49.000000 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/supercritical_plant/tests/test_scpc_flowsheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:16:15.445856 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 01:14:49.000000 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   298229 2023-07-01 01:14:49.000000 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/pfd_ultra_supercritical_pc.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:16:15.449856 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 01:14:49.000000 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   111391 2023-07-01 01:14:49.000000 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/charge_design_ultra_supercritical_power_plant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50372 2023-07-01 01:14:49.000000 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/discharge_design_ultra_supercritical_power_plant.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2330804 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/initialized_integrated_storage_usc.json
+-rw-r--r--   0 runner    (1001) docker     (123)    54649 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/integrated_storage_with_ultrasupercritical_power_plant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14951 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/multiperiod_double_loop_usc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12754 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/multiperiod_integrated_storage_usc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16166 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/pricetaker_with_multiperiod_integrated_storage_usc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:16:15.449856 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/tests/test_charge_usc_powerplant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/tests/test_discharge_usc_powerplant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/tests/test_integrated_storage_with_ultrasupercritical_power_plant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/tests/test_multiperiod_integrated_storage_usc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:16:15.449856 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/tests/test_usc_powerplant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51228 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/ultra_supercritical_powerplant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:16:15.453856 dispatches-1.3.0rc0/dispatches/case_studies/nuclear_case/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/nuclear_case/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2921488 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/nuclear_case/lmp_signal.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/nuclear_case/nuclear_flowsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11459 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/nuclear_case/nuclear_flowsheet_multiperiod_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:16:15.453856 dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/PEM_parametrized_bidder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21792 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/RE_flowsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16259 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/RE_surrogate_optimization_steadystate.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:16:15.465856 dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1819947 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/data/309_WIND_1-SimulationOutputs.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   191554 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/data/44.21_-101.94_windtoolkit_2012_60min_80m.srw
+-rw-r--r--   0 runner    (1001) docker     (123)  7076863 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/data/Wind_Thermal_Dispatch.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/double_loop_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/load_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/run_double_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/run_double_loop_PEM.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:16:15.465856 dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   140032 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/tests/rts_results_all_prices.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/tests/test_RE_flowsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/tests/test_multiperiod_wind_battery_doubleloop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/tests/test_surrogate_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/tests/test_surrogate_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/tests/test_wind_PEM_double_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12284 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/wind_PEM_double_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/wind_battery_LMP.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17565 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/wind_battery_PEM_LMP.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27433 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/wind_battery_PEM_tank_turbine_LMP.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/wind_battery_double_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:16:15.465856 dispatches-1.3.0rc0/dispatches/case_studies/simple_rankine_cycle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/simple_rankine_cycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27406 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/simple_rankine_cycle/simple_rankine_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14031 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/simple_rankine_cycle/surrogate_design_alamo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11264 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/simple_rankine_cycle/surrogate_design_scikit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/simple_rankine_cycle/train_alamo_surrogates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/simple_rankine_cycle/train_keras_surrogates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/case_studies/simple_rankine_cycle/train_scikit_surrogates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:16:15.465856 dispatches-1.3.0rc0/dispatches/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/properties/h2_ideal_vap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/properties/h2_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16153 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/properties/hitecsalt_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/properties/hturbine_ideal_vap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16216 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/properties/solarsalt_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:16:15.469856 dispatches-1.3.0rc0/dispatches/properties/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/properties/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/properties/tests/test_h2_ideal_vap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/properties/tests/test_hitecsalt_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/properties/tests/test_solarsalt_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/properties/tests/test_thermaloil_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/properties/thermaloil_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:16:15.469856 dispatches-1.3.0rc0/dispatches/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:16:15.469856 dispatches-1.3.0rc0/dispatches/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/tests/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:16:15.477856 dispatches-1.3.0rc0/dispatches/tests/data/prescient_5bus/
+-rw-r--r--   0 runner    (1001) docker     (123)   231999 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/tests/data/prescient_5bus/DAY_AHEAD_load.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   269139 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/tests/data/prescient_5bus/DAY_AHEAD_renewables.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  2888100 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/tests/data/prescient_5bus/REAL_TIME_load.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  3641364 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/tests/data/prescient_5bus/REAL_TIME_renewables.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/tests/data/prescient_5bus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/tests/data/prescient_5bus/branch.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/tests/data/prescient_5bus/bus.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/tests/data/prescient_5bus/gen.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/tests/data/prescient_5bus/initial_status.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/tests/data/prescient_5bus/reserves.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/tests/data/prescient_5bus/simulation_objects.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/tests/data/prescient_5bus/timeseries_pointers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/tests/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/tests/test_prescient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:16:15.477856 dispatches-1.3.0rc0/dispatches/unit_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/unit_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10778 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/unit_models/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39163 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/unit_models/concrete_tes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/unit_models/elec_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16798 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/unit_models/heat_exchanger_tube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26308 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/unit_models/hydrogen_tank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/unit_models/hydrogen_tank_simplified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/unit_models/hydrogen_turbine_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/unit_models/pem_electrolyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/unit_models/solar_pv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:16:15.481856 dispatches-1.3.0rc0/dispatches/unit_models/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/unit_models/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/unit_models/tests/test_battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26496 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/unit_models/tests/test_concrete_tes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/unit_models/tests/test_elec_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/unit_models/tests/test_heat_exchanger_tube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/unit_models/tests/test_hydrogen_tank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/unit_models/tests/test_hydrogen_tank_simplified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/unit_models/tests/test_hydrogen_turbine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/unit_models/tests/test_pem_electrolyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/unit_models/tests/test_solar_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/unit_models/tests/test_wind_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/unit_models/wind_power.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:16:15.481856 dispatches-1.3.0rc0/dispatches/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/util/surrogates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/util/syn_hist_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/util/syn_hist_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/util/teal_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:16:15.481856 dispatches-1.3.0rc0/dispatches/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/workflow/coordinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/workflow/parametrized_bidder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/workflow/rts_gmlc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:16:15.481856 dispatches-1.3.0rc0/dispatches/workflow/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/workflow/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/workflow/tests/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/dispatches/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:16:15.441856 dispatches-1.3.0rc0/dispatches.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-01 01:16:15.000000 dispatches-1.3.0rc0/dispatches.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-07-01 01:16:15.000000 dispatches-1.3.0rc0/dispatches.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 01:16:15.000000 dispatches-1.3.0rc0/dispatches.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-01 01:16:15.000000 dispatches-1.3.0rc0/dispatches.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-01 01:16:15.000000 dispatches-1.3.0rc0/dispatches.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 01:16:15.481856 dispatches-1.3.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-07-01 01:14:50.000000 dispatches-1.3.0rc0/setup.py
```

### Comparing `dispatches-1.2.0rc1/LICENSE.md` & `dispatches-1.3.0rc0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/PKG-INFO` & `dispatches-1.3.0rc0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dispatches
-Version: 1.2.0rc1
+Version: 1.3.0rc0
 Summary: GMLC DISPATCHES software tools
 Home-page: https://github.com/gmlc-dispatches/dispatches
 Author: DISPATCHES team
 Keywords: market simulation,chemical engineering,process modeling,hybrid power systems
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dispatches-1.2.0rc1/README.md` & `dispatches-1.3.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/__init__.py` & `dispatches-1.3.0rc0/dispatches/__init__.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/supercritical_plant/supercritical_powerplant.py` & `dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/supercritical_plant/supercritical_powerplant.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/supercritical_plant/tests/test_scpc_flowsheet.py` & `dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/supercritical_plant/tests/test_scpc_flowsheet.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/pfd_ultra_supercritical_pc.svg` & `dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/pfd_ultra_supercritical_pc.svg`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/charge_design_ultra_supercritical_power_plant.py` & `dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/charge_design_ultra_supercritical_power_plant.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/discharge_design_ultra_supercritical_power_plant.py` & `dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/discharge_design_ultra_supercritical_power_plant.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/initialized_integrated_storage_usc.json` & `dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/initialized_integrated_storage_usc.json`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/integrated_storage_with_ultrasupercritical_power_plant.py` & `dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/integrated_storage_with_ultrasupercritical_power_plant.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/multiperiod_double_loop_usc.py` & `dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/multiperiod_double_loop_usc.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/multiperiod_integrated_storage_usc.py` & `dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/multiperiod_integrated_storage_usc.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/pricetaker_with_multiperiod_integrated_storage_usc.py` & `dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/pricetaker_with_multiperiod_integrated_storage_usc.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/tests/test_charge_usc_powerplant.py` & `dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/tests/test_charge_usc_powerplant.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/tests/test_discharge_usc_powerplant.py` & `dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/tests/test_discharge_usc_powerplant.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/tests/test_integrated_storage_with_ultrasupercritical_power_plant.py` & `dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/tests/test_integrated_storage_with_ultrasupercritical_power_plant.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/tests/test_multiperiod_integrated_storage_usc.py` & `dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/tests/test_multiperiod_integrated_storage_usc.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/tests/test_usc_powerplant.py` & `dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/tests/test_usc_powerplant.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/fossil_case/ultra_supercritical_plant/ultra_supercritical_powerplant.py` & `dispatches-1.3.0rc0/dispatches/case_studies/fossil_case/ultra_supercritical_plant/ultra_supercritical_powerplant.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/nuclear_case/lmp_signal.json` & `dispatches-1.3.0rc0/dispatches/case_studies/nuclear_case/lmp_signal.json`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/nuclear_case/nuclear_flowsheet.py` & `dispatches-1.3.0rc0/dispatches/case_studies/nuclear_case/nuclear_flowsheet.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/nuclear_case/nuclear_flowsheet_multiperiod_class.py` & `dispatches-1.3.0rc0/dispatches/case_studies/nuclear_case/nuclear_flowsheet_multiperiod_class.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/RE_flowsheet.py` & `dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/RE_flowsheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,16 @@
 from dispatches.unit_models import (
     HydrogenTurbine,
     HydrogenTank,
     SimpleHydrogenTank,
     PEM_Electrolyzer,
     ElectricalSplitter,
     BatteryStorage,
-    Wind_Power
+    Wind_Power,
+    SolarPV
 )
 
 from idaes.models.unit_models.separator import Separator
 from dispatches.case_studies.renewables_case.load_parameters import *
 import matplotlib as mpl
 mpl.use(mpl.rcParams['backend'])
 import logging
@@ -82,14 +83,30 @@
         wind unit model in the flowsheet
     """
     m.fs.windpower = Wind_Power(**wind_resource_config)
     m.fs.windpower.system_capacity.fix(wind_mw * 1e3)   # kW
     return m.fs.windpower
 
 
+def add_pv(m, pv_mw, pv_resource_config):
+    """
+    Adds a solar pv unit to the flowsheet with a fixed system capacity and that uses resource data to determine the capacity factors
+
+    Args:
+        m: existing ConcreteModel with a flowsheet `fs`
+        pv_mw: capacity of PV model to be fixed
+        pv_resource_config: dictionary of Config keys `capacity_factors` and ConfigValues
+    Returns:
+        pv unit model in the flowsheet
+    """
+    m.fs.pv = SolarPV(**pv_resource_config)
+    m.fs.pv.system_capacity.fix(pv_mw * 1e3)   # kW
+    return m.fs.pv
+
+
 def add_pem(m, outlet_pressure_bar):
     """
     Adds a PEM electrolyzer unit to the flowsheet with a fixed outlet pressure and conversion rate. The properties package is h2_ideal_vap.
 
     The operating temperature and maximum pressure of the PEM are pulled from load_parameters.py
 
     Args:
@@ -313,15 +330,15 @@
         source=m.fs.mixer.outlet,
         destination=m.fs.h2_turbine.compressor.inlet
     )
 
     return m.fs.h2_turbine, m.fs.mixer, m.fs.translator
 
 
-def create_model(wind_mw, pem_bar, batt_mw, tank_type, tank_length_m, turb_inlet_bar, wind_resource_config=None):
+def create_model(re_mw, pem_bar, batt_mw, tank_type, tank_length_m, turb_inlet_bar, resource_config, re_type='wind'):
     """
     Creates a Flowsheet Pyomo model that puts together the Wind unit model with optional PEM, Hydrogen Tank, and Hydrogen Turbine unit models.
 
     The input parameters determine the size of the technologies by fixing the appropriate variable. If the size parameter is None, the technology
     will not be added.
 
     The wind is first split among its output destinations: grid, battery and PEM with an ElectricalSplitter unit model. 
@@ -332,45 +349,53 @@
         wind_mw: wind farm capacity
         pem_bar: operating pressure of the PEM  
         batt_mw: nameplate power
         tank_type: `simple`, `detailed`, or `detailed-valve`. See `add_h2_tank` for descriptions
         tank_length_m: required if using `detailed` tank type, length of tank
         turb_inlet_bar: operating inlet pressure of hydrogen to turbine
         wind_resource_config: dictionary of Windpower Config keys (`resource_speed`, `resource_probability_density`) and ConfigValues. See `add_wind` for description
+        re_type: 'wind' or 'pv'
     
     """
     m = ConcreteModel()
 
     m.fs = FlowsheetBlock(dynamic=False)
 
-    wind = add_wind(m, wind_mw, wind_resource_config)
-    wind_output_dests = ["grid"]
+    if re_type == "wind":
+        re = add_wind(m, re_mw, resource_config)
+    elif re_type == 'pv':
+        re = add_pv(m, re_mw, resource_config)
+        
+    re_output_dests = ["grid"]
 
     if pem_bar is not None:
         pem, _ = add_pem(m, pem_bar)
-        wind_output_dests.append("pem")
+        re_output_dests.append("pem")
 
     if batt_mw is not None:
         battery = add_battery(m, batt_mw)
-        wind_output_dests.append("battery")
+        re_output_dests.append("battery")
 
     if tank_length_m is not None:
         h2_tank = add_h2_tank(m, tank_type, pem_bar, tank_length_m)
 
     if turb_inlet_bar is not None and tank_length_m is not None:
         add_h2_turbine(m, turb_inlet_bar)
 
     # Set up where wind output flows to
-    if len(wind_output_dests) > 1:
-        m.fs.splitter = ElectricalSplitter(outlet_list=wind_output_dests)
-        m.fs.wind_to_splitter = Arc(source=wind.electricity_out, dest=m.fs.splitter.electricity_in)
+    if len(re_output_dests) > 1:
+        m.fs.splitter = ElectricalSplitter(outlet_list=re_output_dests)
+        if re_type == "wind":
+            m.fs.wind_to_splitter = Arc(source=re.electricity_out, dest=m.fs.splitter.electricity_in)
+        elif re_type == 'pv':
+            m.fs.pv_to_splitter = Arc(source=re.electricity_out, dest=m.fs.splitter.electricity_in)
 
-    if "pem" in wind_output_dests:
+    if "pem" in re_output_dests:
         m.fs.splitter_to_pem = Arc(source=m.fs.splitter.pem_port, dest=pem.electricity_in)
-    if "battery" in wind_output_dests:
+    if "battery" in re_output_dests:
         m.fs.splitter_to_battery = Arc(source=m.fs.splitter.battery_port, dest=battery.power_in)
 
     if hasattr(m.fs, "h2_tank"):
         m.fs.pem_to_tank = Arc(source=pem.outlet, dest=h2_tank.inlet)
 
     if hasattr(m.fs, "h2_turbine"):
         if tank_type == 'simple':
@@ -391,15 +416,15 @@
             m.fs.h2_splitter_to_turb = Arc(source=m.fs.h2_splitter.turbine,
                                         destination=m.fs.translator.inlet)
 
     TransformationFactory("network.expand_arcs").apply_to(m)
 
     # Scaling factors, set mostly to 1 for now
     elec_sf = 1
-    iscale.set_scaling_factor(m.fs.windpower.electricity, elec_sf)
+    iscale.set_scaling_factor(re.electricity, elec_sf)
     if hasattr(m.fs, "splitter"):
         iscale.set_scaling_factor(m.fs.splitter.electricity, elec_sf)
         iscale.set_scaling_factor(m.fs.splitter.grid_elec, elec_sf)
 
     if hasattr(m.fs, "battery"):
         iscale.set_scaling_factor(m.fs.splitter.battery_elec, elec_sf)
         iscale.set_scaling_factor(m.fs.battery.elec_in, elec_sf)
```

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/data/309_WIND_1-SimulationOutputs.csv` & `dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/data/309_WIND_1-SimulationOutputs.csv`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/data/44.21_-101.94_windtoolkit_2012_60min_80m.srw` & `dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/data/44.21_-101.94_windtoolkit_2012_60min_80m.srw`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/data/Wind_Thermal_Dispatch.csv` & `dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/data/Wind_Thermal_Dispatch.csv`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-,122_RTLMP,122_DALMP,303_RTLMP,303_DALMP,309_RTLMP,309_DALMP,317_RTLMP,317_DALMP,101_CT_1-DADispatch,101_CT_1-RTDispatch,101_CT_2-DADispatch,101_CT_2-RTDispatch,102_CT_1-DADispatch,102_CT_1-RTDispatch,102_CT_2-DADispatch,102_CT_2-RTDispatch,107_CC_1-DADispatch,107_CC_1-RTDispatch,113_CT_1-DADispatch,113_CT_1-RTDispatch,113_CT_2-DADispatch,113_CT_2-RTDispatch,113_CT_3-DADispatch,113_CT_3-RTDispatch,113_CT_4-DADispatch,113_CT_4-RTDispatch,118_CC_1-DADispatch,118_CC_1-RTDispatch,123_CT_1-DADispatch,123_CT_1-RTDispatch,123_CT_4-DADispatch,123_CT_4-RTDispatch,123_CT_5-DADispatch,123_CT_5-RTDispatch,201_CT_1-DADispatch,201_CT_1-RTDispatch,201_CT_2-DADispatch,201_CT_2-RTDispatch,202_CT_1-DADispatch,202_CT_1-RTDispatch,202_CT_2-DADispatch,202_CT_2-RTDispatch,207_CT_1-DADispatch,207_CT_1-RTDispatch,207_CT_2-DADispatch,207_CT_2-RTDispatch,213_CC_3-DADispatch,213_CC_3-RTDispatch,213_CT_1-DADispatch,213_CT_1-RTDispatch,213_CT_2-DADispatch,213_CT_2-RTDispatch,215_CT_4-DADispatch,215_CT_4-RTDispatch,215_CT_5-DADispatch,215_CT_5-RTDispatch,218_CC_1-DADispatch,218_CC_1-RTDispatch,221_CC_1-DADispatch,221_CC_1-RTDispatch,223_CT_4-DADispatch,223_CT_4-RTDispatch,223_CT_5-DADispatch,223_CT_5-RTDispatch,223_CT_6-DADispatch,223_CT_6-RTDispatch,301_CT_1-DADispatch,301_CT_1-RTDispatch,301_CT_2-DADispatch,301_CT_2-RTDispatch,301_CT_3-DADispatch,301_CT_3-RTDispatch,301_CT_4-DADispatch,301_CT_4-RTDispatch,302_CT_1-DADispatch,302_CT_1-RTDispatch,302_CT_2-DADispatch,302_CT_2-RTDispatch,302_CT_3-DADispatch,302_CT_3-RTDispatch,302_CT_4-DADispatch,302_CT_4-RTDispatch,307_CT_1-DADispatch,307_CT_1-RTDispatch,307_CT_2-DADispatch,307_CT_2-RTDispatch,313_CC_1-DADispatch,313_CC_1-RTDispatch,315_CT_6-DADispatch,315_CT_6-RTDispatch,315_CT_7-DADispatch,315_CT_7-RTDispatch,315_CT_8-DADispatch,315_CT_8-RTDispatch,318_CC_1-DADispatch,318_CC_1-RTDispatch,321_CC_1-DADispatch,321_CC_1-RTDispatch,322_CT_5-DADispatch,322_CT_5-RTDispatch,322_CT_6-DADispatch,322_CT_6-RTDispatch,323_CC_1-DADispatch,323_CC_1-RTDispatch,323_CC_2-DADispatch,323_CC_2-RTDispatch,122_WIND_1-DADispatch,122_WIND_1-RTDispatch,122_WIND_1-Curtailed,303_WIND_1-DADispatch,303_WIND_1-RTDispatch,303_WIND_1-Curtailed,309_WIND_1-DADispatch,309_WIND_1-RTDispatch,309_WIND_1-Curtailed,317_WIND_1-DADispatch,317_WIND_1-RTDispatch,317_WIND_1-Curtailed,309_WIND_1-RTPower,317_WIND_1-RTPower,303_WIND_1-RTPower,122_WIND_1-RTPower,309_WIND_1-DAPower,317_WIND_1-DAPower,303_WIND_1-DAPower,122_WIND_1-DAPower,122_WIND_1-RTCF,122_WIND_1-DACF,303_WIND_1-RTCF,303_WIND_1-DACF,309_WIND_1-RTCF,309_WIND_1-DACF,317_WIND_1-RTCF,317_WIND_1-DACF
+DateTime,122_RTLMP,122_DALMP,303_RTLMP,303_DALMP,309_RTLMP,309_DALMP,317_RTLMP,317_DALMP,101_CT_1-DADispatch,101_CT_1-RTDispatch,101_CT_2-DADispatch,101_CT_2-RTDispatch,102_CT_1-DADispatch,102_CT_1-RTDispatch,102_CT_2-DADispatch,102_CT_2-RTDispatch,107_CC_1-DADispatch,107_CC_1-RTDispatch,113_CT_1-DADispatch,113_CT_1-RTDispatch,113_CT_2-DADispatch,113_CT_2-RTDispatch,113_CT_3-DADispatch,113_CT_3-RTDispatch,113_CT_4-DADispatch,113_CT_4-RTDispatch,118_CC_1-DADispatch,118_CC_1-RTDispatch,123_CT_1-DADispatch,123_CT_1-RTDispatch,123_CT_4-DADispatch,123_CT_4-RTDispatch,123_CT_5-DADispatch,123_CT_5-RTDispatch,201_CT_1-DADispatch,201_CT_1-RTDispatch,201_CT_2-DADispatch,201_CT_2-RTDispatch,202_CT_1-DADispatch,202_CT_1-RTDispatch,202_CT_2-DADispatch,202_CT_2-RTDispatch,207_CT_1-DADispatch,207_CT_1-RTDispatch,207_CT_2-DADispatch,207_CT_2-RTDispatch,213_CC_3-DADispatch,213_CC_3-RTDispatch,213_CT_1-DADispatch,213_CT_1-RTDispatch,213_CT_2-DADispatch,213_CT_2-RTDispatch,215_CT_4-DADispatch,215_CT_4-RTDispatch,215_CT_5-DADispatch,215_CT_5-RTDispatch,218_CC_1-DADispatch,218_CC_1-RTDispatch,221_CC_1-DADispatch,221_CC_1-RTDispatch,223_CT_4-DADispatch,223_CT_4-RTDispatch,223_CT_5-DADispatch,223_CT_5-RTDispatch,223_CT_6-DADispatch,223_CT_6-RTDispatch,301_CT_1-DADispatch,301_CT_1-RTDispatch,301_CT_2-DADispatch,301_CT_2-RTDispatch,301_CT_3-DADispatch,301_CT_3-RTDispatch,301_CT_4-DADispatch,301_CT_4-RTDispatch,302_CT_1-DADispatch,302_CT_1-RTDispatch,302_CT_2-DADispatch,302_CT_2-RTDispatch,302_CT_3-DADispatch,302_CT_3-RTDispatch,302_CT_4-DADispatch,302_CT_4-RTDispatch,307_CT_1-DADispatch,307_CT_1-RTDispatch,307_CT_2-DADispatch,307_CT_2-RTDispatch,313_CC_1-DADispatch,313_CC_1-RTDispatch,315_CT_6-DADispatch,315_CT_6-RTDispatch,315_CT_7-DADispatch,315_CT_7-RTDispatch,315_CT_8-DADispatch,315_CT_8-RTDispatch,318_CC_1-DADispatch,318_CC_1-RTDispatch,321_CC_1-DADispatch,321_CC_1-RTDispatch,322_CT_5-DADispatch,322_CT_5-RTDispatch,322_CT_6-DADispatch,322_CT_6-RTDispatch,323_CC_1-DADispatch,323_CC_1-RTDispatch,323_CC_2-DADispatch,323_CC_2-RTDispatch,122_WIND_1-DADispatch,122_WIND_1-RTDispatch,122_WIND_1-Curtailed,303_WIND_1-DADispatch,303_WIND_1-RTDispatch,303_WIND_1-Curtailed,309_WIND_1-DADispatch,309_WIND_1-RTDispatch,309_WIND_1-Curtailed,317_WIND_1-DADispatch,317_WIND_1-RTDispatch,317_WIND_1-Curtailed,309_WIND_1-RTPower,317_WIND_1-RTPower,303_WIND_1-RTPower,122_WIND_1-RTPower,309_WIND_1-DAPower,317_WIND_1-DAPower,303_WIND_1-DAPower,122_WIND_1-DAPower,122_WIND_1-RTCF,122_WIND_1-DACF,303_WIND_1-RTCF,303_WIND_1-DACF,309_WIND_1-RTCF,309_WIND_1-DACF,317_WIND_1-RTCF,317_WIND_1-DACF
 2020-01-02 00:00:00,23.07,21.288312,23.07,21.288312,23.07,21.288312,23.07,21.288312,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,568.4,527.183333,0.0,141.1,54.333333,0.0,0.1,0.833333,0.0,729.1,494.966667,0.0,0.8333333333333334,494.9666666666667,54.333333333333336,527.1833333333334,0.1,729.1,141.1,568.4,0.738869423032002,0.7966362999299229,0.06414797323888233,0.1665879574970484,0.005619240278714317,0.0006743088334457181,0.6194051641429942,0.9124014516330873
 2020-01-02 01:00:00,22.968387,20.419032,22.968387,20.419032,22.968387,20.419032,22.968387,20.419032,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,630.0,582.15,0.0,52.6,14.7,0.0,0.8,1.166667,0.0,757.1,416.625,0.0,1.1666666666666667,416.625,14.700000000000001,582.15,0.8,757.1,52.6,630.0,0.8159074982480728,0.8829712683952348,0.017355371900826446,0.06210153482880756,0.007866936390200046,0.005394470667565745,0.5213677887623577,0.9474408709798523
 2020-01-02 02:00:00,24.617429,19.689677,24.617429,19.689677,24.617429,19.689677,24.617429,19.689677,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,672.3,462.466667,0.0,17.4,7.716667,0.0,2.7,15.208333,0.0,753.4,233.875,0.0,15.20833333333333,233.875,7.716666666666666,462.4666666666667,2.7,753.4,17.4,672.3,0.6481663162812428,0.9422564821303433,0.009110586383313656,0.020543093270365995,0.10255113508653627,0.01820633850303439,0.29267300713302463,0.9428106619947441
 2020-01-02 03:00:00,24.617429,19.983571,24.617429,19.983571,24.617429,19.983571,24.617429,19.983571,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,661.3,402.816667,0.0,8.9,13.7,0.0,11.4,19.233333,0.0,734.3,200.866667,0.0,19.233333333333334,200.86666666666667,13.699999999999998,402.81666666666666,11.4,734.3,8.9,661.3,0.5645643541228684,0.9268395234758233,0.016174734356552537,0.010507674144037782,0.12969206563272645,0.07687120701281186,0.25136612021857924,0.918908772368915
 2020-01-02 04:00:00,27.050323,19.983571,27.050323,19.983571,27.050323,19.983571,27.050323,19.983571,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,654.0,402.341667,0.0,7.0,18.491667,0.0,18.3,26.016667,0.0,724.2,179.416667,0.0,26.016666666666666,179.41666666666666,18.491666666666667,402.34166666666664,18.3,724.2,7.0,654.0,0.5638986218173324,0.9166082690960056,0.021831955922865014,0.008264462809917356,0.175432681501461,0.12339851652056641,0.22452342218328952,0.9062695532474033
 2020-01-02 05:00:00,22.51634,20.419032,22.51634,20.419032,22.51634,20.419032,22.51634,20.419032,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,654.4,554.716667,0.0,11.6,27.55,0.0,23.6,23.966667,0.0,725.7,437.175,0.0,23.966666666666665,437.175,27.55,554.7166666666667,23.6,725.7,11.6,654.4,0.7774585377248306,0.9171688857743517,0.03252656434474616,0.01369539551357733,0.16160935041582375,0.15913688469318948,0.5470842197472157,0.9081466649981229
 2020-01-02 06:00:00,22.492903,21.843871,22.492903,21.843871,22.492903,21.843871,22.492903,21.843871,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,666.4,672.733333,0.0,23.3,22.108333,0.0,24.6,8.841667,0.0,748.0,593.241667,0.0,8.841666666666667,593.2416666666667,22.108333333333334,672.7333333333333,24.6,748.0,23.3,666.4,0.9428638168652185,0.9339873861247372,0.02610192837465565,0.027508854781582055,0.05962013935715891,0.16587997302764665,0.7423872690109706,0.9360530596921537
```

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/load_parameters.py` & `dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/load_parameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,18 +20,19 @@
 
 re_case_dir = Path(this_file_dir())
 
 timestep_hrs = 1                            # timestep [hr]
 # constants
 h2_mols_per_kg = 500
 H2_mass = 2.016 / 1000
+kg_to_tons = 0.00110231
 
 # costs in per kW unless specified otherwise
 wind_cap_cost = 1550
-wind_op_cost = 43
+wind_op_cost = 10
 batt_cap_cost = 300 * 4                     # per kW for 4 hour battery
 batt_rep_cost_kwh = batt_cap_cost * 0.5 / 4 # assume 50% price w/ discounting and 4 hour battery
 pem_cap_cost = 1630
 pem_op_cost = 47.9
 pem_var_cost = 1.3/1000                     # per kWh
 tank_cap_cost_per_m3 = 29 * 0.8 * 1000      # per m^3
 tank_cap_cost_per_kg = 29 * 33.5            # per kg
@@ -60,30 +61,28 @@
 h2_turb_min_flow = 1e-3
 air_h2_ratio = 10.76
 compressor_dp = 24.01
 max_pressure_bar = 700
 
 # load pre-compiled RTS-GMLC output data
 df = pd.read_csv(re_case_dir / "data" / "Wind_Thermal_Dispatch.csv")
-df["DateTime"] = df['Unnamed: 0']
-df.drop('Unnamed: 0', inplace=True, axis=1)
 df.index = pd.to_datetime(df["DateTime"])
 
 # drop indices not in original data set
 start_date = pd.Timestamp('2020-01-02 00:00:00')
 ix = pd.date_range(start=start_date, 
                     end=start_date
                     + pd.offsets.DateOffset(days=365)
                     - pd.offsets.DateOffset(hours=1),
                     freq='1H')
 ix = ix[(ix.day != 29) | (ix.month != 2)]
 
 df = df[df.index.isin(ix)]
 
-bus = "309"
+bus = "303"
 market = "DA"
 prices = df[f"{bus}_{market}LMP"].values
 prices_used = copy.copy(prices)
 prices_used[prices_used > 200] = 200
 weekly_prices = prices_used.reshape(52, 168)
 # n_time_points = 7 * 24
 
@@ -92,17 +91,17 @@
 wind_cfs = df[f"{bus}_WIND_1-{market}CF"].values
 
 wind_capacity_factors = {t:
                             {'wind_resource_config': {
                                 'capacity_factor': 
                                     [wind_cfs[t]]}} for t in range(n_timesteps)}
 # simple financial assumptions
-i = 0.05                                    # discount rate
+discount_rate = 0.05                                    # discount rate
 N = 30                                      # years
-PA = ((1+i)**N - 1)/(i*(1+i)**N)            # present value / annuity = 1 / CRF
+PA = ((1+discount_rate)**N - 1)/(discount_rate*(1+discount_rate)**N)            # present value / annuity = 1 / CRF
 
 # wind resource data from example Wind Toolkit file
 wind_data = SRW_to_wind_data(re_case_dir / 'data' / '44.21_-101.94_windtoolkit_2012_60min_80m.srw')
 wind_speeds = [wind_data['data'][i][2] for i in range(8760)]
 
 wind_resource = {t:
                     {'wind_resource_config': {
```

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/run_double_loop.py` & `dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/run_double_loop.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,16 @@
     ThermalGeneratorModelData,
 )
 from idaes import __version__
 import pyomo.environ as pyo
 from pyomo.common.fileutils import this_file_dir
 import pandas as pd
 from pathlib import Path
-from dispatches_sample_data import rts_gmlc
+
+from dispatches_data.api import path
 
 this_file_path = Path(this_file_dir())
 
 usage = "Run double loop simulation with RE model."
 parser = ArgumentParser(usage)
 
 parser.add_argument(
@@ -126,15 +127,15 @@
 
 prescient_outputs_df = pd.read_csv(this_file_path / "data" / "Wind_Thermal_Dispatch.csv")
 prescient_outputs_df.index = pd.to_datetime(prescient_outputs_df['Unnamed: 0'])
 prescient_outputs_df = prescient_outputs_df[prescient_outputs_df.index >= pd.Timestamp(f'{start_date} 00:00:00')]
 gen_capacity_factor = prescient_outputs_df[f"{wind_generator}-RTCF"].values.tolist()
 
 # NOTE: `rts_gmlc_data_dir` should point to a directory containing RTS-GMLC scenarios
-rts_gmlc_data_dir = rts_gmlc.source_data_path
+rts_gmlc_data_dir = path("rts_gmlc") / "SourceData"
 output_dir = Path(f"sim_{sim_id}_results")
 
 solver = pyo.SolverFactory("xpress_direct")
 
 if participation_mode == "Bid":
     thermal_generator_params = {
         "gen_name": wind_generator,
@@ -145,15 +146,16 @@
         "min_up_time": 0,
         "ramp_up_60min": wind_pmax + battery_pmax,
         "ramp_down_60min": wind_pmax + battery_pmax,
         "shutdown_capacity": wind_pmax + battery_pmax,
         "startup_capacity": 0,
         "initial_status": 1,
         "initial_p_output": 0,
-        "production_cost_bid_pairs": [(p_min, 0), (wind_pmax, 0)],
+        "production_cost_bid_pairs": [(p_min, 0), (wind_pmax + battery_pmax, 0)],
+        "include_default_p_cost": False,
         "startup_cost_pairs": [(0, 0)],
         "fixed_commitment": None,
     }
     model_data = ThermalGeneratorModelData(**thermal_generator_params)
 elif participation_mode == "SelfSchedule":
     generator_params = {
         "gen_name": wind_generator,
```

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/tests/rts_results_all_prices.npy` & `dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/tests/rts_results_all_prices.npy`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/tests/test_RE_flowsheet.py` & `dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/tests/test_RE_flowsheet.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,21 +43,21 @@
     params["wind_resource"] = wind_resource
     return params
 
 
 def test_create_model(input_params):
     tank_type = "simple"
     m = create_model(
-        wind_mw=fixed_wind_mw,
+        re_mw=fixed_wind_mw,
         pem_bar=pem_bar,
         batt_mw=fixed_batt_mw,
         tank_type=tank_type,
         tank_length_m=fixed_tank_size,
         turb_inlet_bar=pem_bar,
-        wind_resource_config=input_params['wind_resource'][0]['wind_resource_config']
+        resource_config=input_params['wind_resource'][0]['wind_resource_config']
     )
 
     assert hasattr(m.fs, "windpower")
     assert hasattr(m.fs, "splitter")
     assert hasattr(m.fs, "battery")
     assert hasattr(m.fs, "pem")
     assert hasattr(m.fs, "h2_tank")
@@ -79,53 +79,89 @@
     assert value(m.fs.h2_turbine.turbine.deltaP[0]) == -2401000.0
     assert value(m.fs.mixer.air_feed.mole_frac_comp[0, "hydrogen"]) == 2e-4
 
     dof = degrees_of_freedom(m)
     assert dof == 10
 
 
+def test_create_model_PV():
+    pv_capacity_factors = {'capacity_factor': [0.5]}
+
+    tank_type = "simple"
+    m = create_model(
+        re_mw=800,
+        pem_bar=pem_bar,
+        batt_mw=fixed_batt_mw,
+        tank_type=tank_type,
+        tank_length_m=fixed_tank_size,
+        turb_inlet_bar=pem_bar,
+        resource_config=pv_capacity_factors,
+        re_type='pv'
+    )
+
+    assert hasattr(m.fs, "pv")
+    assert hasattr(m.fs, "splitter")
+    assert hasattr(m.fs, "battery")
+    assert hasattr(m.fs, "pem")
+    assert hasattr(m.fs, "h2_tank")
+    assert hasattr(m.fs, "translator")
+    assert hasattr(m.fs, "mixer")
+    assert hasattr(m.fs, "h2_turbine")
+    assert hasattr(m.fs.mixer, "purchased_hydrogen_feed")
+
+    assert m.fs.pv.system_capacity.fixed
+    assert m.fs.battery.nameplate_power.fixed
+    assert m.fs.mixer.air_h2_ratio.active
+    assert m.fs.mixer.purchased_hydrogen_feed.flow_mol[0].lb
+    assert value(m.fs.h2_turbine.turbine.deltaP[0]) == -2401000.0
+    assert value(m.fs.mixer.air_feed.mole_frac_comp[0, "hydrogen"]) == 2e-4
+
+    dof = degrees_of_freedom(m)
+    assert dof == 10
+
+
 def test_wind_battery_optimize(input_params):
     mp = wind_battery_optimize(n_time_points=7 * 24, input_params=input_params, verbose=True)
-    assert value(mp.pyomo_model.NPV) == pytest.approx(1001068228, rel=1e-3)
-    assert value(mp.pyomo_model.annual_revenue) == pytest.approx(168691601, rel=1e-3)
+    assert value(mp.pyomo_model.NPV) == pytest.approx(1429566414, rel=1e-3)
+    assert value(mp.pyomo_model.annual_revenue) == pytest.approx(196566023, rel=1e-3)
     blks = mp.get_active_process_blocks()
     assert value(blks[0].fs.battery.nameplate_power) == pytest.approx(1326779, rel=1e-3)
     plot_results(*record_results(mp))
 
 
 def test_wind_battery_pem_optimize(input_params):
     input_params['h2_price_per_kg'] = 2.5
     design_res, _ = wind_battery_pem_optimize(time_points=6 * 24, input_params=input_params, verbose=True)
     assert design_res['batt_mw'] == pytest.approx(4874, rel=1e-3)
     assert design_res['pem_mw'] == pytest.approx(0, abs=1e-1)
     assert design_res['annual_rev_h2'] == pytest.approx(0.055, abs=1e-1)
-    assert design_res['annual_rev_E'] == pytest.approx(531576401, rel=1e-2)
-    assert design_res['NPV'] == pytest.approx(2322131921, rel=1e-2)
+    assert design_res['annual_rev_E'] == pytest.approx(559530360, rel=1e-2)
+    assert design_res['NPV'] == pytest.approx(2750726183, rel=1e-2)
 
 
 def test_wind_battery_pem_tank_turb_optimize_simple(input_params):
     input_params['h2_price_per_kg'] = 2.0
     design_res = wind_battery_pem_tank_turb_optimize(6 * 24, input_params, verbose=True, plot=False)
     assert design_res['batt_mw'] == pytest.approx(4874, rel=1e-2)
     assert design_res['pem_mw'] == pytest.approx(0, abs=3)
     assert design_res['tank_kgH2'] == pytest.approx(0, abs=3)
     assert design_res['turb_mw'] == pytest.approx(0, abs=3)
     assert design_res['avg_turb_eff'] == pytest.approx(1.51, rel=1e-1)
     assert design_res['annual_rev_h2'] == pytest.approx(2634, abs=5e3)
-    assert design_res['annual_rev_E'] == pytest.approx(531566543, rel=1e-2)
-    assert design_res['NPV'] == pytest.approx(2344545889, rel=1e-2)
+    assert design_res['annual_rev_E'] == pytest.approx(559530220, rel=1e-2)
+    assert design_res['NPV'] == pytest.approx(2774377851, rel=1e-2)
 
 
 @pytest.mark.skipif(platform.system() == "Windows", reason="Platform differences in IPOPT solve")
 def test_wind_battery_pem_tank_turb_optimize_detailed(input_params):
     input_params['h2_price_per_kg'] = 2.0
     input_params['tank_type'] = 'detailed'
     input_params['pem_mw'] = 0
     design_res = wind_battery_pem_tank_turb_optimize(6 * 24, input_params=input_params, verbose=True, plot=False)
     assert design_res['batt_mw'] == pytest.approx(4874, rel=1e-2)
     assert design_res['pem_mw'] == pytest.approx(0, abs=3)
     assert design_res['tank_kgH2'] == pytest.approx(0, abs=3)
     assert design_res['turb_mw'] == pytest.approx(0, abs=3)
     assert design_res['avg_turb_eff'] == pytest.approx(1.51, rel=1e-1)
     assert design_res['annual_rev_h2'] == pytest.approx(2634, abs=5e3)
-    assert design_res['annual_rev_E'] == pytest.approx(531566543, rel=1e-2)
-    assert design_res['NPV'] == pytest.approx(2344545889, rel=1e-2)
+    assert design_res['annual_rev_E'] == pytest.approx(559530220, rel=1e-2)
+    assert design_res['NPV'] == pytest.approx(2774377851, rel=1e-2)
```

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/tests/test_multiperiod_wind_battery_doubleloop.py` & `dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/tests/test_multiperiod_wind_battery_doubleloop.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,14 @@
 from dispatches.case_studies.renewables_case.wind_battery_double_loop import MultiPeriodWindBattery
 
 
 @pytest.fixture
 def wind_thermal_dispatch_data():
     re_case_dir = Path(this_file_dir()).parent
     df = pd.read_csv(re_case_dir / "data" / "Wind_Thermal_Dispatch.csv")
-    df["DateTime"] = df['Unnamed: 0']
-    df.drop('Unnamed: 0', inplace=True, axis=1)
     df.index = pd.to_datetime(df["DateTime"])
     return df
 
 
 @pytest.mark.component
 def test_track_market_dispatch(wind_thermal_dispatch_data):
 
@@ -204,14 +202,15 @@
         "ramp_up_60min": wind_pmax + battery_pmax,
         "ramp_down_60min": wind_pmax + battery_pmax,
         "shutdown_capacity": wind_pmax + battery_pmax,
         "startup_capacity": 0,
         "initial_status": 1,
         "initial_p_output": 0,
         "production_cost_bid_pairs": [(pmin, 0), (wind_pmax, 0)],
+        "include_default_p_cost": False,
         "startup_cost_pairs": [(0, 0)],
         "fixed_commitment": None,
     }
     model_data = ThermalGeneratorModelData(**thermal_generator_params)
 
     solver = pyo.SolverFactory("cbc")
 
@@ -240,13 +239,15 @@
 
     blks = bidder_object.day_ahead_model.fs[0].windBattery.get_active_process_blocks(
     )
     assert len(blks) == day_ahead_horizon
     assert len(bidder_object.day_ahead_model.fs.index_set()) == n_scenario
 
     known_solution = [
-        0.0, 6188.0, 0.0, 0.0, 5270.0, 6132.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 
-        0.0, 0.0, 0.0, 7502.0, 7224.0, 6750.000000000001, 5358.0, 0.0, 0.0, 0.0, 0.0, 
-        0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 
-        3772.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 3938.0]
+        0.0, 48.5758, 0.0, 0.0, 265.8715, 942.4884, 0.0, 0.0, 0.0, 0.0,
+        0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 448.9947, 49.4844, 161.6625,
+        550.2666, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0,
+        0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0,
+        1623.0916, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 704.3113,
+        ]
 
     assertStructuredAlmostEqual(bid_prices, known_solution, reltol=1e-2)
```

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/wind_battery_LMP.py` & `dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/wind_battery_LMP.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     m = create_model(
         input_params['wind_mw'],
         None,
         input_params['batt_mw'],
         None,
         None,
         None,
-        wind_resource_config=wind_resource_config
+        resource_config=wind_resource_config
     )
 
     m.fs.battery.initial_state_of_charge.fix(0)
     m.fs.battery.initial_energy_throughput.fix(0)
     initialize_mp(m, verbose=verbose)
 
     wind_battery_om_costs(m)
```

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/wind_battery_PEM_LMP.py` & `dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/wind_battery_PEM_LMP.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     Third, battery ramp constraints and operating cost components are added
 
     Args:
         wind_resource_config: wind resource for the time step
         input_params: size and operation parameters. Required keys: `wind_mw`, `pem_bar`, `batt_mw`
         verbose:
     """
-    m = create_model(input_params['wind_mw'], input_params['pem_bar'], input_params['batt_mw'], None, None, None, wind_resource_config=wind_resource_config)
+    m = create_model(input_params['wind_mw'], input_params['pem_bar'], input_params['batt_mw'], None, None, None, resource_config=wind_resource_config)
 
     m.fs.pem.outlet_state[0].sum_mole_frac_out.deactivate()
     m.fs.pem.outlet_state[0].component_flow_balances.deactivate()
     m.fs.pem.outlet_state[0].phase_fraction_constraint.deactivate()
 
     m.fs.battery.initial_state_of_charge.fix(0)
     m.fs.battery.initial_energy_throughput.fix(0)
@@ -216,30 +216,34 @@
     m.pem_system_capacity = Var(domain=NonNegativeReals, initialize=input_params['pem_mw'] * 1e3, units=pyunits.kW)
 
     # sizing constraints
     if input_params['design_opt']:
         for blk in blks:
             if not input_params['extant_wind']:
                 blk.fs.windpower.system_capacity.unfix()
+            else:
+                m.wind_system_capacity.fix(input_params['wind_mw'] * 1e3)
             blk.fs.battery.nameplate_power.unfix()
     else:
         m.pem_system_capacity.fix(input_params['pem_mw'] * 1e3)
 
     m.wind_max_p = Constraint(mp_battery_wind_pem.pyomo_model.TIME, rule=lambda b, t: blks[t].fs.windpower.system_capacity <= m.wind_system_capacity)
     m.battery_max_p = Constraint(mp_battery_wind_pem.pyomo_model.TIME, rule=lambda b, t: blks[t].fs.battery.nameplate_power <= m.battery_system_capacity)
     m.pem_max_p = Constraint(mp_battery_wind_pem.pyomo_model.TIME, rule=lambda b, t: blks[t].fs.pem.electricity[0] <= m.pem_system_capacity)
 
     m.h2_price_per_kg = pyo.Param(default=input_params['h2_price_per_kg'], mutable=True)
 
     m.wind_cap_cost = pyo.Param(default=wind_cap_cost, mutable=True)
-    if input_params['extant_wind']:
-        m.wind_cap_cost.set_value(0.)
     m.pem_cap_cost = pyo.Param(default=pem_cap_cost, mutable=True)
     m.batt_cap_cost = pyo.Param(default=batt_cap_cost, mutable=True)
 
+    # if wind farm exist already, size is fixed and don't charge the capital cost
+    if input_params['extant_wind']:
+        m.wind_cap_cost.set_value(0.)
+
     # add market data for each block
     for blk in blks:
         blk_wind = blk.fs.windpower
         blk_battery = blk.fs.battery
         blk_pem = blk.fs.pem
 
         # add operating costs
@@ -374,8 +378,8 @@
     }
     print(design_res)
 
     return design_res, ipopt_res
 
 
 if __name__ == "__main__":
-    wind_battery_pem_optimize(6*24, default_input_params, verbose=False, plot=False)
+    wind_battery_pem_optimize(len(prices), default_input_params, verbose=False, plot=False)
```

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/wind_battery_PEM_tank_turbine_LMP.py` & `dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/wind_battery_PEM_tank_turbine_LMP.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/case_studies/renewables_case/wind_battery_double_loop.py` & `dispatches-1.3.0rc0/dispatches/case_studies/renewables_case/wind_battery_double_loop.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/conftest.py` & `dispatches-1.3.0rc0/dispatches/conftest.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/properties/h2_ideal_vap.py` & `dispatches-1.3.0rc0/dispatches/properties/h2_ideal_vap.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/properties/h2_reaction.py` & `dispatches-1.3.0rc0/dispatches/properties/h2_reaction.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/properties/hitecsalt_properties.py` & `dispatches-1.3.0rc0/dispatches/properties/hitecsalt_properties.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/properties/hturbine_ideal_vap.py` & `dispatches-1.3.0rc0/dispatches/properties/hturbine_ideal_vap.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/properties/solarsalt_properties.py` & `dispatches-1.3.0rc0/dispatches/properties/solarsalt_properties.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/properties/tests/test_h2_ideal_vap.py` & `dispatches-1.3.0rc0/dispatches/properties/tests/test_h2_ideal_vap.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/properties/tests/test_hitecsalt_properties.py` & `dispatches-1.3.0rc0/dispatches/properties/tests/test_hitecsalt_properties.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/properties/tests/test_solarsalt_properties.py` & `dispatches-1.3.0rc0/dispatches/properties/tests/test_solarsalt_properties.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/properties/tests/test_thermaloil_properties.py` & `dispatches-1.3.0rc0/dispatches/properties/tests/test_thermaloil_properties.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/properties/thermaloil_properties.py` & `dispatches-1.3.0rc0/dispatches/properties/thermaloil_properties.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/tests/data/prescient_5bus/DAY_AHEAD_load.csv` & `dispatches-1.3.0rc0/dispatches/tests/data/prescient_5bus/DAY_AHEAD_load.csv`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/tests/data/prescient_5bus/DAY_AHEAD_renewables.csv` & `dispatches-1.3.0rc0/dispatches/tests/data/prescient_5bus/DAY_AHEAD_renewables.csv`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/tests/data/prescient_5bus/REAL_TIME_load.csv` & `dispatches-1.3.0rc0/dispatches/tests/data/prescient_5bus/REAL_TIME_load.csv`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/tests/data/prescient_5bus/REAL_TIME_renewables.csv` & `dispatches-1.3.0rc0/dispatches/tests/data/prescient_5bus/REAL_TIME_renewables.csv`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/tests/data/prescient_5bus/gen.csv` & `dispatches-1.3.0rc0/dispatches/tests/data/prescient_5bus/gen.csv`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/tests/data/prescient_5bus/simulation_objects.csv` & `dispatches-1.3.0rc0/dispatches/tests/data/prescient_5bus/simulation_objects.csv`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/tests/data/prescient_5bus/timeseries_pointers.csv` & `dispatches-1.3.0rc0/dispatches/tests/data/prescient_5bus/timeseries_pointers.csv`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/tests/test_headers.py` & `dispatches-1.3.0rc0/dispatches/tests/test_headers.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/tests/test_prescient.py` & `dispatches-1.3.0rc0/dispatches/tests/test_prescient.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/unit_models/__init__.py` & `dispatches-1.3.0rc0/dispatches/unit_models/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 from .elec_splitter import ElectricalSplitter
 from .heat_exchanger_tube import ConcreteTubeSide
 from .hydrogen_tank import HydrogenTank
 from .hydrogen_tank_simplified import SimpleHydrogenTank
 from .hydrogen_turbine_unit import HydrogenTurbine
 from .pem_electrolyzer import PEM_Electrolyzer
 from .wind_power import Wind_Power
+from .solar_pv import SolarPV
 from .concrete_tes import ConcreteTES
```

### Comparing `dispatches-1.2.0rc1/dispatches/unit_models/battery.py` & `dispatches-1.3.0rc0/dispatches/unit_models/battery.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/unit_models/concrete_tes.py` & `dispatches-1.3.0rc0/dispatches/unit_models/concrete_tes.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/unit_models/elec_splitter.py` & `dispatches-1.3.0rc0/dispatches/unit_models/elec_splitter.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/unit_models/heat_exchanger_tube.py` & `dispatches-1.3.0rc0/dispatches/unit_models/heat_exchanger_tube.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/unit_models/hydrogen_tank.py` & `dispatches-1.3.0rc0/dispatches/unit_models/hydrogen_tank.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/unit_models/hydrogen_tank_simplified.py` & `dispatches-1.3.0rc0/dispatches/unit_models/hydrogen_tank_simplified.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/unit_models/hydrogen_turbine_unit.py` & `dispatches-1.3.0rc0/dispatches/unit_models/hydrogen_turbine_unit.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/unit_models/pem_electrolyzer.py` & `dispatches-1.3.0rc0/dispatches/unit_models/pem_electrolyzer.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/unit_models/tests/test_battery.py` & `dispatches-1.3.0rc0/dispatches/unit_models/tests/test_battery.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/unit_models/tests/test_concrete_tes.py` & `dispatches-1.3.0rc0/dispatches/unit_models/tests/test_concrete_tes.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/unit_models/tests/test_elec_splitter.py` & `dispatches-1.3.0rc0/dispatches/unit_models/tests/test_elec_splitter.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/unit_models/tests/test_heat_exchanger_tube.py` & `dispatches-1.3.0rc0/dispatches/unit_models/tests/test_heat_exchanger_tube.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/unit_models/tests/test_hydrogen_tank.py` & `dispatches-1.3.0rc0/dispatches/unit_models/tests/test_hydrogen_tank.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/unit_models/tests/test_hydrogen_tank_simplified.py` & `dispatches-1.3.0rc0/dispatches/unit_models/tests/test_hydrogen_tank_simplified.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/unit_models/tests/test_hydrogen_turbine.py` & `dispatches-1.3.0rc0/dispatches/unit_models/tests/test_hydrogen_turbine.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/unit_models/tests/test_pem_electrolyzer.py` & `dispatches-1.3.0rc0/dispatches/unit_models/tests/test_pem_electrolyzer.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/unit_models/tests/test_wind_power.py` & `dispatches-1.3.0rc0/dispatches/unit_models/tests/test_wind_power.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/unit_models/wind_power.py` & `dispatches-1.3.0rc0/dispatches/unit_models/wind_power.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/util/__init__.py` & `dispatches-1.3.0rc0/dispatches/util/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 #################################################################################
-# DISPATCHES was produced under the DOE Design Integration and Synthesis
-# Platform to Advance Tightly Coupled Hybrid Energy Systems program (DISPATCHES),
-# and is copyright (c) 2022 by the software owners: The Regents of the University
+# DISPATCHES was produced under the DOE Design Integration and Synthesis Platform
+# to Advance Tightly Coupled Hybrid Energy Systems program (DISPATCHES), and is
+# copyright (c) 2020-2023 by the software owners: The Regents of the University
 # of California, through Lawrence Berkeley National Laboratory, National
 # Technology & Engineering Solutions of Sandia, LLC, Alliance for Sustainable
 # Energy, LLC, Battelle Energy Alliance, LLC, University of Notre Dame du Lac, et
 # al. All rights reserved.
 #
 # Please see the files COPYRIGHT.md and LICENSE.md for full copyright and license
 # information, respectively. Both files are also available online at the URL:
 # "https://github.com/gmlc-dispatches/dispatches".
-#
 #################################################################################
 
-
+from .surrogates import train_surrogate_model
 from .teal_integration import (
     build_econ_settings,
     build_TEAL_Component,
     calculate_TEAL_metrics,
 )
 from .syn_hist_integration import SynHist_integration
 from .syn_hist_generation import generate_syn_realizations
```

### Comparing `dispatches-1.2.0rc1/dispatches/util/syn_hist_generation.py` & `dispatches-1.3.0rc0/dispatches/util/syn_hist_generation.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/util/syn_hist_integration.py` & `dispatches-1.3.0rc0/dispatches/util/syn_hist_integration.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/util/teal_integration.py` & `dispatches-1.3.0rc0/dispatches/util/teal_integration.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/workflow/__init__.py` & `dispatches-1.3.0rc0/dispatches/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/workflow/coordinator.py` & `dispatches-1.3.0rc0/dispatches/workflow/coordinator.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/workflow/rts_gmlc.py` & `dispatches-1.3.0rc0/dispatches/workflow/rts_gmlc.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/workflow/tests/test_workflow.py` & `dispatches-1.3.0rc0/dispatches/workflow/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches/workflow/workflow.py` & `dispatches-1.3.0rc0/dispatches/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `dispatches-1.2.0rc1/dispatches.egg-info/PKG-INFO` & `dispatches-1.3.0rc0/dispatches.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dispatches
-Version: 1.2.0rc1
+Version: 1.3.0rc0
 Summary: GMLC DISPATCHES software tools
 Home-page: https://github.com/gmlc-dispatches/dispatches
 Author: DISPATCHES team
 Keywords: market simulation,chemical engineering,process modeling,hybrid power systems
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dispatches-1.2.0rc1/dispatches.egg-info/SOURCES.txt` & `dispatches-1.3.0rc0/dispatches.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -32,31 +32,45 @@
 dispatches/case_studies/fossil_case/ultra_supercritical_plant/storage/tests/test_multiperiod_integrated_storage_usc.py
 dispatches/case_studies/fossil_case/ultra_supercritical_plant/tests/__init__.py
 dispatches/case_studies/fossil_case/ultra_supercritical_plant/tests/test_usc_powerplant.py
 dispatches/case_studies/nuclear_case/__init__.py
 dispatches/case_studies/nuclear_case/lmp_signal.json
 dispatches/case_studies/nuclear_case/nuclear_flowsheet.py
 dispatches/case_studies/nuclear_case/nuclear_flowsheet_multiperiod_class.py
+dispatches/case_studies/renewables_case/PEM_parametrized_bidder.py
 dispatches/case_studies/renewables_case/RE_flowsheet.py
+dispatches/case_studies/renewables_case/RE_surrogate_optimization_steadystate.py
 dispatches/case_studies/renewables_case/__init__.py
 dispatches/case_studies/renewables_case/double_loop_utils.py
 dispatches/case_studies/renewables_case/load_parameters.py
 dispatches/case_studies/renewables_case/run_double_loop.py
+dispatches/case_studies/renewables_case/run_double_loop_PEM.py
+dispatches/case_studies/renewables_case/wind_PEM_double_loop.py
 dispatches/case_studies/renewables_case/wind_battery_LMP.py
 dispatches/case_studies/renewables_case/wind_battery_PEM_LMP.py
 dispatches/case_studies/renewables_case/wind_battery_PEM_tank_turbine_LMP.py
 dispatches/case_studies/renewables_case/wind_battery_double_loop.py
 dispatches/case_studies/renewables_case/data/309_WIND_1-SimulationOutputs.csv
 dispatches/case_studies/renewables_case/data/44.21_-101.94_windtoolkit_2012_60min_80m.srw
 dispatches/case_studies/renewables_case/data/Wind_Thermal_Dispatch.csv
 dispatches/case_studies/renewables_case/data/__init__.py
 dispatches/case_studies/renewables_case/tests/__init__.py
 dispatches/case_studies/renewables_case/tests/rts_results_all_prices.npy
 dispatches/case_studies/renewables_case/tests/test_RE_flowsheet.py
 dispatches/case_studies/renewables_case/tests/test_multiperiod_wind_battery_doubleloop.py
+dispatches/case_studies/renewables_case/tests/test_surrogate_models.py
+dispatches/case_studies/renewables_case/tests/test_surrogate_opt.py
+dispatches/case_studies/renewables_case/tests/test_wind_PEM_double_loop.py
+dispatches/case_studies/simple_rankine_cycle/__init__.py
+dispatches/case_studies/simple_rankine_cycle/simple_rankine_cycle.py
+dispatches/case_studies/simple_rankine_cycle/surrogate_design_alamo.py
+dispatches/case_studies/simple_rankine_cycle/surrogate_design_scikit.py
+dispatches/case_studies/simple_rankine_cycle/train_alamo_surrogates.py
+dispatches/case_studies/simple_rankine_cycle/train_keras_surrogates.py
+dispatches/case_studies/simple_rankine_cycle/train_scikit_surrogates.py
 dispatches/properties/__init__.py
 dispatches/properties/h2_ideal_vap.py
 dispatches/properties/h2_reaction.py
 dispatches/properties/hitecsalt_properties.py
 dispatches/properties/hturbine_ideal_vap.py
 dispatches/properties/solarsalt_properties.py
 dispatches/properties/thermaloil_properties.py
@@ -86,28 +100,32 @@
 dispatches/unit_models/concrete_tes.py
 dispatches/unit_models/elec_splitter.py
 dispatches/unit_models/heat_exchanger_tube.py
 dispatches/unit_models/hydrogen_tank.py
 dispatches/unit_models/hydrogen_tank_simplified.py
 dispatches/unit_models/hydrogen_turbine_unit.py
 dispatches/unit_models/pem_electrolyzer.py
+dispatches/unit_models/solar_pv.py
 dispatches/unit_models/wind_power.py
 dispatches/unit_models/tests/__init__.py
 dispatches/unit_models/tests/test_battery.py
 dispatches/unit_models/tests/test_concrete_tes.py
 dispatches/unit_models/tests/test_elec_splitter.py
 dispatches/unit_models/tests/test_heat_exchanger_tube.py
 dispatches/unit_models/tests/test_hydrogen_tank.py
 dispatches/unit_models/tests/test_hydrogen_tank_simplified.py
 dispatches/unit_models/tests/test_hydrogen_turbine.py
 dispatches/unit_models/tests/test_pem_electrolyzer.py
+dispatches/unit_models/tests/test_solar_pv.py
 dispatches/unit_models/tests/test_wind_power.py
 dispatches/util/__init__.py
+dispatches/util/surrogates.py
 dispatches/util/syn_hist_generation.py
 dispatches/util/syn_hist_integration.py
 dispatches/util/teal_integration.py
 dispatches/workflow/__init__.py
 dispatches/workflow/coordinator.py
+dispatches/workflow/parametrized_bidder.py
 dispatches/workflow/rts_gmlc.py
 dispatches/workflow/workflow.py
 dispatches/workflow/tests/__init__.py
 dispatches/workflow/tests/test_workflow.py
```

### Comparing `dispatches-1.2.0rc1/setup.py` & `dispatches-1.3.0rc0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -61,29 +61,31 @@
     - for_release: to be used when cutting a release of DISPATCHES
     - for_prerelease: to be used for the prerelease version of DISPATCHES (i.e. the `main` branch, and all PRs targeting it)
     """
     # idaes-pse: for IDAES DMF -dang 12/2020
     for_release = [
         # NOTE: this will fail until this idaes-pse version is available on PyPI
         "idaes-pse==2.0.*",
+        "pyomo==6.5.*",
     ]
     for_prerelease = [
         "idaes-pse==2.0.*",
+        "pyomo==6.5.*",
     ]
 
 
 SPECIAL_DEPENDENCIES = SpecialDependencies.for_release
 
 
 ########################################################################################
 
 setup(
     name="dispatches",
     url="https://github.com/gmlc-dispatches/dispatches",
-    version="1.2.0rc1",
+    version="1.3.0rc0",
     description="GMLC DISPATCHES software tools",
     long_description=long_description,
     long_description_content_type="text/plain",
     author="DISPATCHES team",
     # Classifiers help users find your project by categorizing it.
     #
     # For a list of valid classifiers, see https://pypi.org/classifiers/
@@ -115,27 +117,30 @@
     install_requires=[
         "pytest",
         # we use jupyter notebooks
         "jupyter",
         # for visualizing DMF provenance
         "graphviz",
         "gridx-prescient>=2.2.2",
-        "nrel-pysam>=3.0.1",
+        "nrel-pysam",
+        "utm",
         "dispatches-data-packages >= 23.3.19",
+        "dispatches-rts-gmlc-data",
         *SPECIAL_DEPENDENCIES
     ],
     extras_require={
         "teal": [
-            "raven-framework == 2.2 ; python_version <= '3.8' and platform_system != 'Linux'",
-            "teal-ravenframework == 0.3 ; python_version <= '3.8' and platform_system != 'Linux'",
+            "raven-framework == 2.3 ; python_version <= '3.9' and platform_system != 'Linux'",
+            "teal-ravenframework == 0.4 ; python_version <= '3.9' and platform_system != 'Linux'",
             "dispatches-synthetic-price-data >= 23.4.4",
         ],
         "surrogates": [
-            "tslearn >= 0.5.2",
-            "tensorflow >= 2.9.1",
+            "tslearn >= 0.5.2",  # not needed for steady-state surrogates
+            "scikit-learn == 1.2.1",  # used by RE steady-state surrogate (static_clustering_wind_pmax.pkl)
+            "tensorflow == 2.10.0",  # to match Tensorflow version used to train RE steady-state surrogates Keras models
             "tables >= 3.6.1",
             "matplotlib",
             "dispatches-dynamic-sweep-data >= 23.4.4",
         ],
     },
     package_data={
         "": ["*.json"],
@@ -144,14 +149,37 @@
             "rts_results_all_prices.npy",
         ],
         "dispatches.case_studies.renewables_case.data": [
            "Wind_Thermal_Dispatch.csv",
            "309_WIND_1-SimulationOutputs.csv",
             "44.21_-101.94_windtoolkit_2012_60min_80m.srw"
         ],
+        "dispatches.case_studies.renewables_case.data.steady_state_surrogate.dispatch_frequency":[
+            "ss_surrogate_param_wind_pmax.json",
+            "static_clustering_wind_pmax.pkl"
+        ],
+        "dispatches.case_studies.renewables_case.data.steady_state_surrogate.dispatch_frequency.ss_surrogate_model_wind_pmax":[
+            "keras_metadata.pb",
+            "saved_model.pb"
+        ],
+        "dispatches.case_studies.renewables_case.data.steady_state_surrogate.dispatch_frequency.ss_surrogate_model_wind_pmax.variables":[
+            "variables.data-00000-of-00001",
+            "variables.index"
+        ],
+        "dispatches.case_studies.renewables_case.data.steady_state_surrogate.revenue":[
+            "RE_revenue_params_2_25.json"
+        ],
+        "dispatches.case_studies.renewables_case.data.steady_state_surrogate.revenue.RE_revenue_2_25":[
+            "keras_metadata.pb",
+            "saved_model.pb"
+        ],
+        "dispatches.case_studies.renewables_case.data.steady_state_surrogate.revenue.RE_revenue_2_25.variables":[
+            "variables.data-00000-of-00001",
+            "variables.index"
+        ],
         "dispatches.case_studies.fossil_case.ultra_supercritical_plant": [
             "pfd_ultra_supercritical_pc.svg",
         ],
         "dispatches.workflow.train_market_surrogates.dynamic.tests.data":[
             "inputdatatest.h5",
             "revdatatest.csv",
             "simdatatest.csv",
```

