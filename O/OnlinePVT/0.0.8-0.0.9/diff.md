# Comparing `tmp/onlinepvt-0.0.8.tar.gz` & `tmp/onlinepvt-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onlinepvt-0.0.8.tar", last modified: Thu Mar 16 13:50:34 2023, max compression
+gzip compressed data, was "onlinepvt-0.0.9.tar", last modified: Sat Mar 18 12:13:24 2023, max compression
```

## Comparing `onlinepvt-0.0.8.tar` & `onlinepvt-0.0.9.tar`

### file list

```diff
@@ -1,90 +1,94 @@
-drwxrwxrwx   0        0        0        0 2023-03-16 13:50:34.402177 onlinepvt-0.0.8/
--rw-rw-rw-   0        0        0     1087 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1942 2023-03-16 13:50:34.402177 onlinepvt-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1403 2023-03-12 19:51:44.000000 onlinepvt-0.0.8/README.md
--rw-rw-rw-   0        0        0      108 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      678 2023-03-16 13:50:34.404173 onlinepvt-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-16 13:50:34.199419 onlinepvt-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-03-16 13:50:34.226706 onlinepvt-0.0.8/src/onlinepvt/
--rw-rw-rw-   0        0        0       57 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 13:50:34.397175 onlinepvt-0.0.8/src/onlinepvt/models/
--rw-rw-rw-   0        0        0     5619 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/__init__.py
--rw-rw-rw-   0        0        0      203 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_call_result.py
--rw-rw-rw-   0        0        0     7085 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_fluid.py
--rw-rw-rw-   0        0        0    16791 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_fluid_component_block.py
--rw-rw-rw-   0        0        0     2971 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_fluid_distribution_moment.py
--rw-rw-rw-   0        0        0     1410 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_fluid_kij.py
--rw-rw-rw-   0        0        0     4095 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_fluid_polymer_component.py
--rw-rw-rw-   0        0        0     1994 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_fluid_pseudo_component.py
--rw-rw-rw-   0        0        0    16948 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_fluid_standard_component.py
--rw-rw-rw-   0        0        0    11247 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_output_calculation_result_phase.py
--rw-rw-rw-   0        0        0     2082 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_output_calculation_result_phase_composition.py
--rw-rw-rw-   0        0        0     1529 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_output_calculation_result_phase_polymer_moment.py
--rw-rw-rw-   0        0        0     2006 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_output_calculation_result_phase_polymer_moments.py
--rw-rw-rw-   0        0        0     2887 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_output_calculation_result_point.py
--rw-rw-rw-   0        0        0     5432 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_output_phasediagram.py
--rw-rw-rw-   0        0        0     1342 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_output_phasediagram_point.py
--rw-rw-rw-   0        0        0     4001 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_output_unflashed_property_result.py
--rw-rw-rw-   0        0        0     5594 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_output_unflashed_property_result_ideal.py
--rw-rw-rw-   0        0        0     5609 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_output_unflashed_property_result_residual.py
--rw-rw-rw-   0        0        0     2080 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_profile_information.py
--rw-rw-rw-   0        0        0     1898 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_profile_time_information.py
--rw-rw-rw-   0        0        0     2124 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_value_component_composition.py
--rw-rw-rw-   0        0        0     1627 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_value_composition_array.py
--rw-rw-rw-   0        0        0      827 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_value_compressibility.py
--rw-rw-rw-   0        0        0     1005 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_value_density.py
--rw-rw-rw-   0        0        0     1010 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_value_enthalpy.py
--rw-rw-rw-   0        0        0     1005 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_value_entropy.py
--rw-rw-rw-   0        0        0      856 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_value_floating_with_out_units.py
--rw-rw-rw-   0        0        0     1325 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_value_floating_with_out_units_name.py
--rw-rw-rw-   0        0        0     1055 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_value_floating_with_units.py
--rw-rw-rw-   0        0        0      810 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_value_mole_percent.py
--rw-rw-rw-   0        0        0     1004 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_value_pressure.py
--rw-rw-rw-   0        0        0     1019 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_value_temperature.py
--rw-rw-rw-   0        0        0     1000 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_value_volume.py
--rw-rw-rw-   0        0        0      821 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/api_value_weight_percent.py
--rw-rw-rw-   0        0        0      601 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/association_scheme.py
--rw-rw-rw-   0        0        0     1777 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/calculation_block_info.py
--rw-rw-rw-   0        0        0     4018 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/calculation_composition.py
--rw-rw-rw-   0        0        0     3188 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/cloud_point_calculation_input.py
--rw-rw-rw-   0        0        0     3602 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/cloud_point_calculation_result.py
--rw-rw-rw-   0        0        0      251 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/cloud_point_calculation_type.py
--rw-rw-rw-   0        0        0      252 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/component_type.py
--rw-rw-rw-   0        0        0      201 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/cp_model.py
--rw-rw-rw-   0        0        0      287 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/distribution_model.py
--rw-rw-rw-   0        0        0      203 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/eos_model.py
--rw-rw-rw-   0        0        0     1905 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/exception_info.py
--rw-rw-rw-   0        0        0     3726 2023-03-16 13:49:35.000000 onlinepvt-0.0.8/src/onlinepvt/models/flash_calculation_input.py
--rw-rw-rw-   0        0        0     3580 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/flash_calculation_result.py
--rw-rw-rw-   0        0        0      281 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/flash_calculation_type.py
--rw-rw-rw-   0        0        0     3449 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/flashed_property_calculation_input.py
--rw-rw-rw-   0        0        0     3624 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/flashed_property_calculation_result.py
--rw-rw-rw-   0        0        0      182 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/is_alkane.py
--rw-rw-rw-   0        0        0     1522 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/new_fluid_input.py
--rw-rw-rw-   0        0        0     2179 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/new_fluid_result.py
--rw-rw-rw-   0        0        0      276 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/phase_type.py
--rw-rw-rw-   0        0        0     3326 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/phasediagram_fixed_temperature_pressure_calculation_input.py
--rw-rw-rw-   0        0        0     3660 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/phasediagram_fixed_temperature_pressure_calculation_result.py
--rw-rw-rw-   0        0        0      208 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/polymer_type.py
--rw-rw-rw-   0        0        0     2360 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/problem_details.py
--rw-rw-rw-   0        0        0      284 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/properties_calculation_type.py
--rw-rw-rw-   0        0        0      274 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/property_reference_point.py
--rw-rw-rw-   0        0        0     1235 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/request_fluid_input.py
--rw-rw-rw-   0        0        0     2492 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/request_fluid_result.py
--rw-rw-rw-   0        0        0     3171 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/sle_point_calculation_input.py
--rw-rw-rw-   0        0        0     3596 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/sle_point_calculation_result.py
--rw-rw-rw-   0        0        0      249 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/sle_point_calculation_type.py
--rw-rw-rw-   0        0        0     3484 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/unflashed_property_calculation_input.py
--rw-rw-rw-   0        0        0     3637 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/unflashed_property_calculation_result.py
--rw-rw-rw-   0        0        0     3418 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/units.py
--rw-rw-rw-   0        0        0      932 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/models/units_item.py
--rw-rw-rw-   0        0        0     7044 2023-03-12 19:53:59.000000 onlinepvt-0.0.8/src/onlinepvt/online_pvt_client.py
--rw-rw-rw-   0        0        0     1027 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/src/onlinepvt/types.py
-drwxrwxrwx   0        0        0        0 2023-03-16 13:50:34.242707 onlinepvt-0.0.8/src/onlinepvt.egg-info/
--rw-rw-rw-   0        0        0     1942 2023-03-16 13:50:34.000000 onlinepvt-0.0.8/src/onlinepvt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3838 2023-03-16 13:50:34.000000 onlinepvt-0.0.8/src/onlinepvt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-16 13:50:34.000000 onlinepvt-0.0.8/src/onlinepvt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-03-16 13:50:34.000000 onlinepvt-0.0.8/src/onlinepvt.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-16 13:50:34.400172 onlinepvt-0.0.8/tests/
--rw-rw-rw-   0        0        0      856 2023-03-16 13:41:47.000000 onlinepvt-0.0.8/tests/test_call_flash.py
--rw-rw-rw-   0        0        0     1504 2023-03-12 19:13:52.000000 onlinepvt-0.0.8/tests/test_json_mapping.py
+drwxrwxrwx   0        0        0        0 2023-03-18 12:13:24.630027 onlinepvt-0.0.9/
+-rw-rw-rw-   0        0        0     1087 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1942 2023-03-18 12:13:24.630027 onlinepvt-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1403 2023-03-12 19:51:44.000000 onlinepvt-0.0.9/README.md
+-rw-rw-rw-   0        0        0      108 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      678 2023-03-18 12:13:24.637547 onlinepvt-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-03-18 12:13:24.469223 onlinepvt-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-03-18 12:13:24.485357 onlinepvt-0.0.9/src/onlinepvt/
+-rw-rw-rw-   0        0        0       57 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-18 12:13:24.500375 onlinepvt-0.0.9/src/onlinepvt/demofluids/
+-rw-rw-rw-   0        0        0       64 2023-03-18 11:57:06.000000 onlinepvt-0.0.9/src/onlinepvt/demofluids/__init__.py
+-rw-rw-rw-   0        0        0     2703 2023-03-18 11:57:06.000000 onlinepvt-0.0.9/src/onlinepvt/demofluids/fluids.py
+drwxrwxrwx   0        0        0        0 2023-03-18 12:13:24.624025 onlinepvt-0.0.9/src/onlinepvt/models/
+-rw-rw-rw-   0        0        0     5619 2023-03-17 17:21:06.000000 onlinepvt-0.0.9/src/onlinepvt/models/__init__.py
+-rw-rw-rw-   0        0        0      203 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_call_result.py
+-rw-rw-rw-   0        0        0     7085 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_fluid.py
+-rw-rw-rw-   0        0        0    16791 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_fluid_component_block.py
+-rw-rw-rw-   0        0        0     2971 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_fluid_distribution_moment.py
+-rw-rw-rw-   0        0        0     1410 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_fluid_kij.py
+-rw-rw-rw-   0        0        0     4095 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_fluid_polymer_component.py
+-rw-rw-rw-   0        0        0     1994 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_fluid_pseudo_component.py
+-rw-rw-rw-   0        0        0    16948 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_fluid_standard_component.py
+-rw-rw-rw-   0        0        0    11281 2023-03-18 11:57:06.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_output_calculation_result_phase.py
+-rw-rw-rw-   0        0        0     2082 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_output_calculation_result_phase_composition.py
+-rw-rw-rw-   0        0        0     1529 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_output_calculation_result_phase_polymer_moment.py
+-rw-rw-rw-   0        0        0     2006 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_output_calculation_result_phase_polymer_moments.py
+-rw-rw-rw-   0        0        0     2887 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_output_calculation_result_point.py
+-rw-rw-rw-   0        0        0     5432 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_output_phasediagram.py
+-rw-rw-rw-   0        0        0     1342 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_output_phasediagram_point.py
+-rw-rw-rw-   0        0        0     4001 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_output_unflashed_property_result.py
+-rw-rw-rw-   0        0        0     5594 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_output_unflashed_property_result_ideal.py
+-rw-rw-rw-   0        0        0     5609 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_output_unflashed_property_result_residual.py
+-rw-rw-rw-   0        0        0     2080 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_profile_information.py
+-rw-rw-rw-   0        0        0     1898 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_profile_time_information.py
+-rw-rw-rw-   0        0        0     2124 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_value_component_composition.py
+-rw-rw-rw-   0        0        0     1627 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_value_composition_array.py
+-rw-rw-rw-   0        0        0      827 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_value_compressibility.py
+-rw-rw-rw-   0        0        0     1005 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_value_density.py
+-rw-rw-rw-   0        0        0     1010 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_value_enthalpy.py
+-rw-rw-rw-   0        0        0     1005 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_value_entropy.py
+-rw-rw-rw-   0        0        0      856 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_value_floating_with_out_units.py
+-rw-rw-rw-   0        0        0     1325 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_value_floating_with_out_units_name.py
+-rw-rw-rw-   0        0        0     1055 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_value_floating_with_units.py
+-rw-rw-rw-   0        0        0      810 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_value_mole_percent.py
+-rw-rw-rw-   0        0        0     1004 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_value_pressure.py
+-rw-rw-rw-   0        0        0     1019 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_value_temperature.py
+-rw-rw-rw-   0        0        0     1000 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_value_volume.py
+-rw-rw-rw-   0        0        0      821 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/api_value_weight_percent.py
+-rw-rw-rw-   0        0        0      601 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/association_scheme.py
+-rw-rw-rw-   0        0        0     1777 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/calculation_block_info.py
+-rw-rw-rw-   0        0        0     4018 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/calculation_composition.py
+-rw-rw-rw-   0        0        0     3707 2023-03-18 11:57:06.000000 onlinepvt-0.0.9/src/onlinepvt/models/cloud_point_calculation_input.py
+-rw-rw-rw-   0        0        0     3602 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/cloud_point_calculation_result.py
+-rw-rw-rw-   0        0        0      251 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/cloud_point_calculation_type.py
+-rw-rw-rw-   0        0        0      252 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/component_type.py
+-rw-rw-rw-   0        0        0      201 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/cp_model.py
+-rw-rw-rw-   0        0        0      287 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/distribution_model.py
+-rw-rw-rw-   0        0        0      203 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/eos_model.py
+-rw-rw-rw-   0        0        0     1905 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/exception_info.py
+-rw-rw-rw-   0        0        0     4139 2023-03-18 11:57:06.000000 onlinepvt-0.0.9/src/onlinepvt/models/flash_calculation_input.py
+-rw-rw-rw-   0        0        0     3580 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/flash_calculation_result.py
+-rw-rw-rw-   0        0        0      281 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/flash_calculation_type.py
+-rw-rw-rw-   0        0        0     3449 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/flashed_property_calculation_input.py
+-rw-rw-rw-   0        0        0     3624 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/flashed_property_calculation_result.py
+-rw-rw-rw-   0        0        0      182 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/is_alkane.py
+-rw-rw-rw-   0        0        0     1522 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/new_fluid_input.py
+-rw-rw-rw-   0        0        0     2179 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/new_fluid_result.py
+-rw-rw-rw-   0        0        0      276 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/phase_type.py
+-rw-rw-rw-   0        0        0     3326 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/phasediagram_fixed_temperature_pressure_calculation_input.py
+-rw-rw-rw-   0        0        0     3660 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/phasediagram_fixed_temperature_pressure_calculation_result.py
+-rw-rw-rw-   0        0        0      208 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/polymer_type.py
+-rw-rw-rw-   0        0        0     2360 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/problem_details.py
+-rw-rw-rw-   0        0        0      284 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/properties_calculation_type.py
+-rw-rw-rw-   0        0        0      274 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/property_reference_point.py
+-rw-rw-rw-   0        0        0     1235 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/request_fluid_input.py
+-rw-rw-rw-   0        0        0     2492 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/request_fluid_result.py
+-rw-rw-rw-   0        0        0     3171 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/sle_point_calculation_input.py
+-rw-rw-rw-   0        0        0     3596 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/sle_point_calculation_result.py
+-rw-rw-rw-   0        0        0      249 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/sle_point_calculation_type.py
+-rw-rw-rw-   0        0        0     3484 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/unflashed_property_calculation_input.py
+-rw-rw-rw-   0        0        0     3637 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/unflashed_property_calculation_result.py
+-rw-rw-rw-   0        0        0     3418 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/units.py
+-rw-rw-rw-   0        0        0      932 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/models/units_item.py
+-rw-rw-rw-   0        0        0     7044 2023-03-12 19:53:59.000000 onlinepvt-0.0.9/src/onlinepvt/online_pvt_client.py
+-rw-rw-rw-   0        0        0     1027 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/src/onlinepvt/types.py
+drwxrwxrwx   0        0        0        0 2023-03-18 12:13:24.498372 onlinepvt-0.0.9/src/onlinepvt.egg-info/
+-rw-rw-rw-   0        0        0     1942 2023-03-18 12:13:24.000000 onlinepvt-0.0.9/src/onlinepvt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3940 2023-03-18 12:13:24.000000 onlinepvt-0.0.9/src/onlinepvt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-18 12:13:24.000000 onlinepvt-0.0.9/src/onlinepvt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-03-18 12:13:24.000000 onlinepvt-0.0.9/src/onlinepvt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-18 12:13:24.630027 onlinepvt-0.0.9/tests/
+-rw-rw-rw-   0        0        0     1398 2023-03-18 11:57:06.000000 onlinepvt-0.0.9/tests/test_call_cloudpoint.py
+-rw-rw-rw-   0        0        0     1388 2023-03-18 11:57:06.000000 onlinepvt-0.0.9/tests/test_call_flash.py
+-rw-rw-rw-   0        0        0     1504 2023-03-12 19:13:52.000000 onlinepvt-0.0.9/tests/test_json_mapping.py
```

### Comparing `onlinepvt-0.0.8/LICENSE` & `onlinepvt-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/PKG-INFO` & `onlinepvt-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onlinepvt
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python SDK for accessing OnlinePVT API
 Home-page: https://github.com/OnlinePVT/onlinepvt-python-sdk
 Author: VLXE A/S
 Author-email: author@vlxe.com
 Project-URL: Bug Tracker, https://github.com/OnlinePVT/onlinepvt-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `onlinepvt-0.0.8/README.md` & `onlinepvt-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/setup.cfg` & `onlinepvt-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206f 6e6c 696e 6570 7674 0d0a 7665   = onlinepvt..ve
-00000020: 7273 696f 6e20 3d20 302e 302e 380d 0a61  rsion = 0.0.8..a
+00000020: 7273 696f 6e20 3d20 302e 302e 390d 0a61  rsion = 0.0.9..a
 00000030: 7574 686f 7220 3d20 564c 5845 2041 2f53  uthor = VLXE A/S
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 2061 7574 686f 7240 766c 7865 2e63 6f6d   author@vlxe.com
 00000060: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000070: 5079 7468 6f6e 2053 444b 2066 6f72 2061  Python SDK for a
 00000080: 6363 6573 7369 6e67 204f 6e6c 696e 6550  ccessing OnlineP
 00000090: 5654 2041 5049 0d0a 6c6f 6e67 5f64 6573  VT API..long_des
```

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/__init__.py` & `onlinepvt-0.0.9/src/onlinepvt/models/__init__.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_fluid.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_fluid.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_fluid_component_block.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_fluid_component_block.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_fluid_distribution_moment.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_fluid_distribution_moment.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_fluid_kij.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_fluid_kij.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_fluid_polymer_component.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_fluid_polymer_component.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_fluid_pseudo_component.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_fluid_pseudo_component.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_fluid_standard_component.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_fluid_standard_component.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_output_calculation_result_phase.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_output_calculation_result_phase.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     phase_label: Union[Unset, None, str] = UNSET
     volume: Union[Unset, ApiValueVolume] = UNSET
     density: Union[Unset, ApiValueDensity] = UNSET
     entropy: Union[Unset, ApiValueEntropy] = UNSET
     enthalpy: Union[Unset, ApiValueEnthalpy] = UNSET
     cp: Union[Unset, ApiValueFloatingWithUnits] = UNSET
     cv: Union[Unset, ApiValueFloatingWithUnits] = UNSET
-    jt_coeffient: Union[Unset, ApiValueFloatingWithUnits] = UNSET
+    jt_coefficient: Union[Unset, ApiValueFloatingWithUnits] = UNSET
     speed_of_sound: Union[Unset, ApiValueFloatingWithUnits] = UNSET
     molecular_weight: Union[Unset, ApiValueFloatingWithUnits] = UNSET
     compressibility: Union[Unset, ApiValueCompressibility] = UNSET
     mole_percent: Union[Unset, ApiValueMolePercent] = UNSET
     weight_percent: Union[Unset, ApiValueWeightPercent] = UNSET
     polymer_moments: Union[Unset,
                            ApiOutputCalculationResultPhasePolymerMoments] = UNSET
@@ -66,17 +66,17 @@
         if not isinstance(self.cp, Unset):
             cp = self.cp.to_dict()
 
         cv: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.cv, Unset):
             cv = self.cv.to_dict()
 
-        jt_coeffient: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.jt_coeffient, Unset):
-            jt_coeffient = self.jt_coeffient.to_dict()
+        jt_coefficient: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.jt_coefficient, Unset):
+            jt_coefficient = self.jt_coefficient.to_dict()
 
         speed_of_sound: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.speed_of_sound, Unset):
             speed_of_sound = self.speed_of_sound.to_dict()
 
         molecular_weight: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.molecular_weight, Unset):
@@ -116,16 +116,16 @@
             field_dict["entropy"] = entropy
         if enthalpy is not UNSET:
             field_dict["enthalpy"] = enthalpy
         if cp is not UNSET:
             field_dict["cp"] = cp
         if cv is not UNSET:
             field_dict["cv"] = cv
-        if jt_coeffient is not UNSET:
-            field_dict["jtCoeffient"] = jt_coeffient
+        if jt_coefficient is not UNSET:
+            field_dict["jtcoefficient"] = jt_coefficient
         if speed_of_sound is not UNSET:
             field_dict["speedOfSound"] = speed_of_sound
         if molecular_weight is not UNSET:
             field_dict["molecularWeight"] = molecular_weight
         if compressibility is not UNSET:
             field_dict["compressibility"] = compressibility
         if mole_percent is not UNSET:
@@ -189,20 +189,20 @@
         _cv = d.pop("cv", UNSET)
         cv: Union[Unset, ApiValueFloatingWithUnits]
         if isinstance(_cv, Unset):
             cv = UNSET
         else:
             cv = ApiValueFloatingWithUnits.from_dict(_cv)
 
-        _jt_coeffient = d.pop("jtCoeffient", UNSET)
-        jt_coeffient: Union[Unset, ApiValueFloatingWithUnits]
-        if isinstance(_jt_coeffient, Unset):
-            jt_coeffient = UNSET
+        _jt_coefficient = d.pop("jtCoefficient", UNSET)
+        jt_coefficient: Union[Unset, ApiValueFloatingWithUnits]
+        if isinstance(_jt_coefficient, Unset):
+            jt_coefficient = UNSET
         else:
-            jt_coeffient = ApiValueFloatingWithUnits.from_dict(_jt_coeffient)
+            jt_coefficient = ApiValueFloatingWithUnits.from_dict(_jt_coefficient)
 
         _speed_of_sound = d.pop("speedOfSound", UNSET)
         speed_of_sound: Union[Unset, ApiValueFloatingWithUnits]
         if isinstance(_speed_of_sound, Unset):
             speed_of_sound = UNSET
         else:
             speed_of_sound = ApiValueFloatingWithUnits.from_dict(
@@ -260,15 +260,15 @@
             phase_label=phase_label,
             volume=volume,
             density=density,
             entropy=entropy,
             enthalpy=enthalpy,
             cp=cp,
             cv=cv,
-            jt_coeffient=jt_coeffient,
+            jt_coefficient=jt_coefficient,
             speed_of_sound=speed_of_sound,
             molecular_weight=molecular_weight,
             compressibility=compressibility,
             mole_percent=mole_percent,
             weight_percent=weight_percent,
             polymer_moments=polymer_moments,
             composition=composition,
```

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_output_calculation_result_phase_composition.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_output_calculation_result_phase_composition.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_output_calculation_result_phase_polymer_moment.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_output_calculation_result_phase_polymer_moment.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_output_calculation_result_phase_polymer_moments.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_output_calculation_result_phase_polymer_moments.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_output_calculation_result_point.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_output_calculation_result_point.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_output_phasediagram.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_output_phasediagram.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_output_phasediagram_point.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_output_phasediagram_point.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_output_unflashed_property_result.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_output_unflashed_property_result.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_output_unflashed_property_result_ideal.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_output_unflashed_property_result_ideal.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_output_unflashed_property_result_residual.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_output_unflashed_property_result_residual.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_profile_information.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_profile_information.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_profile_time_information.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_profile_time_information.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_value_component_composition.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_value_component_composition.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_value_composition_array.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_value_composition_array.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_value_compressibility.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_value_compressibility.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_value_density.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_value_density.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_value_enthalpy.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_value_enthalpy.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_value_entropy.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_value_entropy.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_value_floating_with_out_units.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_value_floating_with_out_units.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_value_floating_with_out_units_name.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_value_floating_with_out_units_name.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_value_floating_with_units.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_value_floating_with_units.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_value_mole_percent.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_value_mole_percent.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_value_pressure.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_value_pressure.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_value_temperature.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_value_temperature.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_value_volume.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_value_volume.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/api_value_weight_percent.py` & `onlinepvt-0.0.9/src/onlinepvt/models/api_value_weight_percent.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/association_scheme.py` & `onlinepvt-0.0.9/src/onlinepvt/models/association_scheme.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/calculation_block_info.py` & `onlinepvt-0.0.9/src/onlinepvt/models/calculation_block_info.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/calculation_composition.py` & `onlinepvt-0.0.9/src/onlinepvt/models/calculation_composition.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/cloud_point_calculation_input.py` & `onlinepvt-0.0.9/src/onlinepvt/models/sle_point_calculation_input.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.calculation_composition import CalculationComposition
-from ..models.cloud_point_calculation_type import CloudPointCalculationType
+from ..models.sle_point_calculation_type import SlePointCalculationType
 from ..models.units import Units
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CloudPointCalculationInput")
+T = TypeVar("T", bound="SlePointCalculationInput")
 
 
 @attr.s(auto_attribs=True)
-class CloudPointCalculationInput:
-    """Input to cloud point calculation"""
+class SlePointCalculationInput:
+    """Input for SLE point calculation"""
 
     user_id: str
     access_secret: str
     components: List[CalculationComposition]
     fluid_id: str
-    point_type: CloudPointCalculationType
+    point_type: SlePointCalculationType
     units: Union[Unset, Units] = UNSET
     temperature: Union[Unset, float] = UNSET
     pressure: Union[Unset, float] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         user_id = self.user_id
         access_secret = self.access_secret
@@ -73,32 +73,32 @@
         for components_item_data in _components:
             components_item = CalculationComposition.from_dict(components_item_data)
 
             components.append(components_item)
 
         fluid_id = d.pop("fluidId")
 
-        point_type = CloudPointCalculationType(d.pop("pointType"))
+        point_type = SlePointCalculationType(d.pop("pointType"))
 
         _units = d.pop("units", UNSET)
         units: Union[Unset, Units]
         if isinstance(_units, Unset):
             units = UNSET
         else:
             units = Units.from_dict(_units)
 
         temperature = d.pop("temperature", UNSET)
 
         pressure = d.pop("pressure", UNSET)
 
-        cloud_point_calculation_input = cls(
+        sle_point_calculation_input = cls(
             user_id=user_id,
             access_secret=access_secret,
             components=components,
             fluid_id=fluid_id,
             point_type=point_type,
             units=units,
             temperature=temperature,
             pressure=pressure,
         )
 
-        return cloud_point_calculation_input
+        return sle_point_calculation_input
```

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/cloud_point_calculation_result.py` & `onlinepvt-0.0.9/src/onlinepvt/models/cloud_point_calculation_result.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/exception_info.py` & `onlinepvt-0.0.9/src/onlinepvt/models/exception_info.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/flash_calculation_input.py` & `onlinepvt-0.0.9/src/onlinepvt/models/cloud_point_calculation_input.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,122 +1,115 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.calculation_composition import CalculationComposition
-from ..models.flash_calculation_type import FlashCalculationType
-from ..models.units import Units
+from ..models.cloud_point_calculation_type import CloudPointCalculationType
+from ..models.api_fluid import ApiFluid
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="FlashCalculationInput")
+T = TypeVar("T", bound="CloudPointCalculationInput")
 
 
 @attr.s(auto_attribs=True)
-class FlashCalculationInput:
-    """Input for flash calculation"""
+class CloudPointCalculationInput:
+    """Input to cloud point calculation"""
 
     user_id: str
     access_secret: str
     components: List[CalculationComposition]
-    flash_type: FlashCalculationType
-    fluid_id: str
+    point_type: CloudPointCalculationType
     units: str
+    fluid_id: Union[Unset, str] = UNSET
+    fluid: Union[Unset, ApiFluid] = UNSET
     temperature: Union[Unset, float] = UNSET
     pressure: Union[Unset, float] = UNSET
-    enthalpy: Union[Unset, float] = UNSET
-    entropy: Union[Unset, float] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         user_id = self.user_id
         access_secret = self.access_secret
         components = []
         for components_item_data in self.components:
             components_item = components_item_data.to_dict()
 
             components.append(components_item)
 
-        flash_type = self.flash_type.value
-
-        #units: Union[Unset, Dict[str, Any]] = UNSET
-        #if not isinstance(self.units, Unset):
-        #    units = self.units.to_dict()
-        units = self.units
-        fluid_id = self.fluid_id
+        point_type = self.point_type.value
         temperature = self.temperature
         pressure = self.pressure
-        enthalpy = self.enthalpy
-        entropy = self.entropy
+        units = self.units
+
+        fluid_id: Union[Unset, str] = UNSET
+        if not isinstance(self.fluid_id, Unset):
+            fluid = self.fluid_id
+
+        fluid: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.fluid, Unset):
+            fluid = self.fluid.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(
             {
                 "userId": user_id,
                 "accessSecret": access_secret,
                 "components": components,
-                "flashType": flash_type,
+                "pointType": point_type,
             }
         )
         if units is not UNSET:
             field_dict["units"] = units
         if fluid_id is not UNSET:
             field_dict["fluidId"] = fluid_id
+        if fluid is not UNSET:
+            field_dict["fluid"] = fluid
         if temperature is not UNSET:
             field_dict["temperature"] = temperature
         if pressure is not UNSET:
             field_dict["pressure"] = pressure
-        if enthalpy is not UNSET:
-            field_dict["enthalpy"] = enthalpy
-        if entropy is not UNSET:
-            field_dict["entropy"] = entropy
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         user_id = d.pop("userId")
-
         access_secret = d.pop("accessSecret")
+        point_type = CloudPointCalculationType(d.pop("pointType"))
+        units = d.pop("units", UNSET)
 
         components = []
         _components = d.pop("components")
         for components_item_data in _components:
-            components_item = CalculationComposition.from_dict(
-                components_item_data)
+            components_item = CalculationComposition.from_dict(components_item_data)
 
             components.append(components_item)
 
-        flash_type = FlashCalculationType(d.pop("flashType"))
-
-        #_units = d.pop("units", UNSET)
-        #units: Union[Unset, Units]
-        #if isinstance(_units, Unset):
-        #    units = UNSET
-        #else:
-        #    units = Units.from_dict(_units)
-
-        units = d.pop("units", UNSET)
-
-        fluid_id = d.pop("fluidId", UNSET)
+        _fluid_id = d.pop("fluidId", UNSET)
+        fluid_id: Union[Unset, str]
+        if isinstance(_fluid_id, Unset):
+            fluid_id = UNSET
+        else:
+            fluid_id = _fluid_id
+
+        _fluid = d.pop("fluid", UNSET)
+        fluid: Union[Unset, ApiFluid]
+        if isinstance(_fluid, Unset):
+            fluid = UNSET
+        else:
+            fluid = ApiFluid.from_dict(_fluid)
 
         temperature = d.pop("temperature", UNSET)
-
         pressure = d.pop("pressure", UNSET)
 
-        enthalpy = d.pop("enthalpy", UNSET)
-
-        entropy = d.pop("entropy", UNSET)
-
-        flash_calculation_input = cls(
+        cloud_point_calculation_input = cls(
             user_id=user_id,
             access_secret=access_secret,
             components=components,
-            flash_type=flash_type,
-            units=units,
             fluid_id=fluid_id,
+            fluid=fluid,
+            point_type=point_type,
+            units=units,
             temperature=temperature,
             pressure=pressure,
-            enthalpy=enthalpy,
-            entropy=entropy,
         )
 
-        return flash_calculation_input
+        return cloud_point_calculation_input
```

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/flash_calculation_result.py` & `onlinepvt-0.0.9/src/onlinepvt/models/flash_calculation_result.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/flashed_property_calculation_input.py` & `onlinepvt-0.0.9/src/onlinepvt/models/flashed_property_calculation_input.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/flashed_property_calculation_result.py` & `onlinepvt-0.0.9/src/onlinepvt/models/flashed_property_calculation_result.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/new_fluid_input.py` & `onlinepvt-0.0.9/src/onlinepvt/models/new_fluid_input.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/new_fluid_result.py` & `onlinepvt-0.0.9/src/onlinepvt/models/new_fluid_result.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/phasediagram_fixed_temperature_pressure_calculation_input.py` & `onlinepvt-0.0.9/src/onlinepvt/models/phasediagram_fixed_temperature_pressure_calculation_input.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/phasediagram_fixed_temperature_pressure_calculation_result.py` & `onlinepvt-0.0.9/src/onlinepvt/models/phasediagram_fixed_temperature_pressure_calculation_result.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/problem_details.py` & `onlinepvt-0.0.9/src/onlinepvt/models/problem_details.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/request_fluid_input.py` & `onlinepvt-0.0.9/src/onlinepvt/models/request_fluid_input.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/request_fluid_result.py` & `onlinepvt-0.0.9/src/onlinepvt/models/request_fluid_result.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/sle_point_calculation_input.py` & `onlinepvt-0.0.9/src/onlinepvt/models/unflashed_property_calculation_input.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,71 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.calculation_composition import CalculationComposition
-from ..models.sle_point_calculation_type import SlePointCalculationType
+from ..models.properties_calculation_type import PropertiesCalculationType
 from ..models.units import Units
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="SlePointCalculationInput")
+T = TypeVar("T", bound="UnflashedPropertyCalculationInput")
 
 
 @attr.s(auto_attribs=True)
-class SlePointCalculationInput:
-    """Input for SLE point calculation"""
+class UnflashedPropertyCalculationInput:
+    """Input to property calculation"""
 
     user_id: str
     access_secret: str
     components: List[CalculationComposition]
     fluid_id: str
-    point_type: SlePointCalculationType
+    calculation_type: PropertiesCalculationType
     units: Union[Unset, Units] = UNSET
     temperature: Union[Unset, float] = UNSET
     pressure: Union[Unset, float] = UNSET
+    volume: Union[Unset, float] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         user_id = self.user_id
         access_secret = self.access_secret
         components = []
         for components_item_data in self.components:
             components_item = components_item_data.to_dict()
 
             components.append(components_item)
 
         fluid_id = self.fluid_id
-        point_type = self.point_type.value
+        calculation_type = self.calculation_type.value
 
         units: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.units, Unset):
             units = self.units.to_dict()
 
         temperature = self.temperature
         pressure = self.pressure
+        volume = self.volume
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(
             {
                 "userId": user_id,
                 "accessSecret": access_secret,
                 "components": components,
                 "fluidId": fluid_id,
-                "pointType": point_type,
+                "calculationType": calculation_type,
             }
         )
         if units is not UNSET:
             field_dict["units"] = units
         if temperature is not UNSET:
             field_dict["temperature"] = temperature
         if pressure is not UNSET:
             field_dict["pressure"] = pressure
+        if volume is not UNSET:
+            field_dict["volume"] = volume
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         user_id = d.pop("userId")
@@ -73,32 +77,35 @@
         for components_item_data in _components:
             components_item = CalculationComposition.from_dict(components_item_data)
 
             components.append(components_item)
 
         fluid_id = d.pop("fluidId")
 
-        point_type = SlePointCalculationType(d.pop("pointType"))
+        calculation_type = PropertiesCalculationType(d.pop("calculationType"))
 
         _units = d.pop("units", UNSET)
         units: Union[Unset, Units]
         if isinstance(_units, Unset):
             units = UNSET
         else:
             units = Units.from_dict(_units)
 
         temperature = d.pop("temperature", UNSET)
 
         pressure = d.pop("pressure", UNSET)
 
-        sle_point_calculation_input = cls(
+        volume = d.pop("volume", UNSET)
+
+        unflashed_property_calculation_input = cls(
             user_id=user_id,
             access_secret=access_secret,
             components=components,
             fluid_id=fluid_id,
-            point_type=point_type,
+            calculation_type=calculation_type,
             units=units,
             temperature=temperature,
             pressure=pressure,
+            volume=volume,
         )
 
-        return sle_point_calculation_input
+        return unflashed_property_calculation_input
```

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/sle_point_calculation_result.py` & `onlinepvt-0.0.9/src/onlinepvt/models/sle_point_calculation_result.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/unflashed_property_calculation_input.py` & `onlinepvt-0.0.9/src/onlinepvt/models/flash_calculation_input.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,111 +1,128 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.calculation_composition import CalculationComposition
-from ..models.properties_calculation_type import PropertiesCalculationType
-from ..models.units import Units
+from ..models.flash_calculation_type import FlashCalculationType
+from ..models.api_fluid import ApiFluid
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnflashedPropertyCalculationInput")
+T = TypeVar("T", bound="FlashCalculationInput")
 
 
 @attr.s(auto_attribs=True)
-class UnflashedPropertyCalculationInput:
-    """Input to property calculation"""
+class FlashCalculationInput:
+    """Input for flash calculation"""
 
     user_id: str
     access_secret: str
     components: List[CalculationComposition]
-    fluid_id: str
-    calculation_type: PropertiesCalculationType
-    units: Union[Unset, Units] = UNSET
+    flash_type: FlashCalculationType
+    units: str
+    fluid_id: Union[Unset, str] = UNSET
+    fluid: Union[Unset, ApiFluid] = UNSET
     temperature: Union[Unset, float] = UNSET
     pressure: Union[Unset, float] = UNSET
-    volume: Union[Unset, float] = UNSET
+    enthalpy: Union[Unset, float] = UNSET
+    entropy: Union[Unset, float] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         user_id = self.user_id
         access_secret = self.access_secret
         components = []
         for components_item_data in self.components:
             components_item = components_item_data.to_dict()
 
             components.append(components_item)
 
-        fluid_id = self.fluid_id
-        calculation_type = self.calculation_type.value
-
-        units: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.units, Unset):
-            units = self.units.to_dict()
-
+        flash_type = self.flash_type.value
+        units = self.units
         temperature = self.temperature
         pressure = self.pressure
-        volume = self.volume
+        enthalpy = self.enthalpy
+        entropy = self.entropy
+
+        fluid_id: Union[Unset, str] = UNSET
+        if not isinstance(self.fluid_id, Unset):
+            fluid = self.fluid_id
+
+        fluid: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.fluid, Unset):
+            fluid = self.fluid.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(
             {
                 "userId": user_id,
                 "accessSecret": access_secret,
                 "components": components,
-                "fluidId": fluid_id,
-                "calculationType": calculation_type,
+                "flashType": flash_type,
             }
         )
         if units is not UNSET:
             field_dict["units"] = units
+        if fluid_id is not UNSET:
+            field_dict["fluidId"] = fluid_id
+        if fluid is not UNSET:
+            field_dict["fluid"] = fluid
         if temperature is not UNSET:
             field_dict["temperature"] = temperature
         if pressure is not UNSET:
             field_dict["pressure"] = pressure
-        if volume is not UNSET:
-            field_dict["volume"] = volume
+        if enthalpy is not UNSET:
+            field_dict["enthalpy"] = enthalpy
+        if entropy is not UNSET:
+            field_dict["entropy"] = entropy
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         user_id = d.pop("userId")
-
         access_secret = d.pop("accessSecret")
+        flash_type = FlashCalculationType(d.pop("flashType"))
+        units = d.pop("units", UNSET)
 
         components = []
         _components = d.pop("components")
         for components_item_data in _components:
-            components_item = CalculationComposition.from_dict(components_item_data)
+            components_item = CalculationComposition.from_dict(
+                components_item_data)
 
             components.append(components_item)
 
-        fluid_id = d.pop("fluidId")
-
-        calculation_type = PropertiesCalculationType(d.pop("calculationType"))
+        _fluid_id = d.pop("fluidId", UNSET)
+        fluid_id: Union[Unset, str]
+        if isinstance(_fluid_id, Unset):
+            fluid_id = UNSET
+        else:
+            fluid_id = _fluid_id
 
-        _units = d.pop("units", UNSET)
-        units: Union[Unset, Units]
-        if isinstance(_units, Unset):
-            units = UNSET
+        _fluid = d.pop("fluid", UNSET)
+        fluid: Union[Unset, ApiFluid]
+        if isinstance(_fluid, Unset):
+            fluid = UNSET
         else:
-            units = Units.from_dict(_units)
+            fluid = ApiFluid.from_dict(_fluid)
 
         temperature = d.pop("temperature", UNSET)
-
         pressure = d.pop("pressure", UNSET)
+        enthalpy = d.pop("enthalpy", UNSET)
+        entropy = d.pop("entropy", UNSET)
 
-        volume = d.pop("volume", UNSET)
-
-        unflashed_property_calculation_input = cls(
+        flash_calculation_input = cls(
             user_id=user_id,
             access_secret=access_secret,
             components=components,
-            fluid_id=fluid_id,
-            calculation_type=calculation_type,
+            flash_type=flash_type,
             units=units,
+            fluid_id=fluid_id,
+            fluid=fluid,
             temperature=temperature,
             pressure=pressure,
-            volume=volume,
+            enthalpy=enthalpy,
+            entropy=entropy,
         )
 
-        return unflashed_property_calculation_input
+        return flash_calculation_input
```

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/unflashed_property_calculation_result.py` & `onlinepvt-0.0.9/src/onlinepvt/models/unflashed_property_calculation_result.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/units.py` & `onlinepvt-0.0.9/src/onlinepvt/models/units.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/models/units_item.py` & `onlinepvt-0.0.9/src/onlinepvt/models/units_item.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/online_pvt_client.py` & `onlinepvt-0.0.9/src/onlinepvt/online_pvt_client.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt/types.py` & `onlinepvt-0.0.9/src/onlinepvt/types.py`

 * *Files identical despite different names*

### Comparing `onlinepvt-0.0.8/src/onlinepvt.egg-info/PKG-INFO` & `onlinepvt-0.0.9/src/onlinepvt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onlinepvt
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python SDK for accessing OnlinePVT API
 Home-page: https://github.com/OnlinePVT/onlinepvt-python-sdk
 Author: VLXE A/S
 Author-email: author@vlxe.com
 Project-URL: Bug Tracker, https://github.com/OnlinePVT/onlinepvt-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `onlinepvt-0.0.8/src/onlinepvt.egg-info/SOURCES.txt` & `onlinepvt-0.0.9/src/onlinepvt.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 src/onlinepvt/__init__.py
 src/onlinepvt/online_pvt_client.py
 src/onlinepvt/types.py
 src/onlinepvt.egg-info/PKG-INFO
 src/onlinepvt.egg-info/SOURCES.txt
 src/onlinepvt.egg-info/dependency_links.txt
 src/onlinepvt.egg-info/top_level.txt
+src/onlinepvt/demofluids/__init__.py
+src/onlinepvt/demofluids/fluids.py
 src/onlinepvt/models/__init__.py
 src/onlinepvt/models/api_call_result.py
 src/onlinepvt/models/api_fluid.py
 src/onlinepvt/models/api_fluid_component_block.py
 src/onlinepvt/models/api_fluid_distribution_moment.py
 src/onlinepvt/models/api_fluid_kij.py
 src/onlinepvt/models/api_fluid_polymer_component.py
@@ -75,9 +77,10 @@
 src/onlinepvt/models/sle_point_calculation_input.py
 src/onlinepvt/models/sle_point_calculation_result.py
 src/onlinepvt/models/sle_point_calculation_type.py
 src/onlinepvt/models/unflashed_property_calculation_input.py
 src/onlinepvt/models/unflashed_property_calculation_result.py
 src/onlinepvt/models/units.py
 src/onlinepvt/models/units_item.py
+tests/test_call_cloudpoint.py
 tests/test_call_flash.py
 tests/test_json_mapping.py
```

### Comparing `onlinepvt-0.0.8/tests/test_json_mapping.py` & `onlinepvt-0.0.9/tests/test_json_mapping.py`

 * *Files identical despite different names*

