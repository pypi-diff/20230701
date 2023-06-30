# Comparing `tmp/electricalsim-0.0.6.9.tar.gz` & `tmp/electricalsim-0.0.7.0.tar.gz`

## Comparing `electricalsim-0.0.6.9.tar` & `electricalsim-0.0.7.0.tar`

### file list

```diff
@@ -1,83 +1,84 @@
--rw-r--r--   0        0        0    17549 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/README.md
--rw-r--r--   0        0        0    84223 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/10_PF4.png
--rw-r--r--   0        0        0    54206 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/11_PF_tooltips.png
--rw-r--r--   0        0        0    88072 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/12_App_settings.png
--rw-r--r--   0        0        0    50389 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/13_Disabling_nodes.png
--rw-r--r--   0        0        0    69759 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/14_Context_menu.png
--rw-r--r--   0        0        0    97038 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/1_Main_Window.png
--rw-r--r--   0        0        0    95822 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/1_Main_Window_dark.png
--rw-r--r--   0        0        0   136326 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/2_Dialogs.png
--rw-r--r--   0        0        0    25172 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/3_Widgets.png
--rw-r--r--   0        0        0    84286 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/4_Pandapower_DataFrames.png
--rw-r--r--   0        0        0    16870 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/5_Connections_angle_b.png
--rw-r--r--   0        0        0    21425 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/5_Connections_curved_b.png
--rw-r--r--   0        0        0    21864 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/5_Connections_straight_b.png
--rw-r--r--   0        0        0    13193 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/6_Line_and_transformer_nodes.png
--rw-r--r--   0        0        0   136386 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/7_PF1.png
--rw-r--r--   0        0        0   144782 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/8_PF2.png
--rw-r--r--   0        0        0    83704 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/9_PF3.png
--rwxr-xr-x   0        0        0    51862 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/Logo_CIESE_2021 y UTN_Sta_Fe.png
--rw-r--r--   0        0        0    33067 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/app_icon.png
--rw-r--r--   0        0        0    22462 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/Electrical_Grid_Simulator.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/__init__.py
--rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/config.ini
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/egs_create_shortcut.py
--rwxr-xr-x   0        0        0       98 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/egs_run.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/version.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/.idea/electricalsim.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/.idea/misc.xml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/.idea/modules.xml
--rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/.idea/workspace.xml
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/extensions/extension_classes.py
--rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/hotkeys/hotkey_functions.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/hotkeys/hotkeys.json
--rwxr-xr-x   0        0        0    82539 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/icons/CIESE_UTN_Sta_Fe.png
--rw-r--r--   0        0        0    33031 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/icons/app_icon.ico
--rw-r--r--   0        0        0    33067 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/icons/app_icon.png
--rwxr-xr-x   0        0        0    14363 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/icons/app_icon.svg
--rw-r--r--   0        0        0    30015 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/lib/auxiliary.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/lib/calculations.py
--rw-r--r--   0        0        0   208285 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/lib/electricalGraph.py
--rw-r--r--   0        0        0    83266 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/lib/main_components.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/lib/table_widget.py
--rw-r--r--   0        0        0    11797 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/about_dialog.ui
--rw-r--r--   0        0        0    17328 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/aload_dialog.ui
--rw-r--r--   0        0        0    17419 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/asgen_dialog.ui
--rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/bus_dialog.ui
--rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/choose_bus_switch.ui
--rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/choose_generator_type.ui
--rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/choose_line_type.ui
--rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/choose_load_type.ui
--rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/choose_transformer_type.ui
--rw-r--r--   0        0        0    23084 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/dcline_dialog.ui
--rw-r--r--   0        0        0   138693 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/dialogs.py
--rw-r--r--   0        0        0    35106 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/ext_grid_dialog.ui
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/extension.ui
--rw-r--r--   0        0        0    33034 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/gen_dialog.ui
--rw-r--r--   0        0        0    16772 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/impedance_dialog.ui
--rw-r--r--   0        0        0    31104 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/line_dialog.ui
--rw-r--r--   0        0        0    25616 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/load_dialog.ui
--rw-r--r--   0        0        0    12940 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/main_window.ui
--rw-r--r--   0        0        0    12741 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/main_window_backup.ui
--rw-r--r--   0        0        0    23184 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/motor_dialog.ui
--rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/network_settings_dialog.ui
--rw-r--r--   0        0        0    34604 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/pf_settings_widget.ui
--rw-r--r--   0        0        0    50076 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/power_flow_dialog.ui
--rw-r--r--   0        0        0    14082 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/settings_dialog.ui
--rw-r--r--   0        0        0    38654 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/sgen_dialog.ui
--rw-r--r--   0        0        0    11331 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/shunt_dialog.ui
--rw-r--r--   0        0        0    10554 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/stdline_dialog.ui
--rw-r--r--   0        0        0    10807 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/stdtransformer3w_dialog.ui
--rw-r--r--   0        0        0    30234 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/stdtransformer_dialog.ui
--rw-r--r--   0        0        0    26339 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/storage_dialog.ui
--rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/switch_dialog.ui
--rw-r--r--   0        0        0    65860 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/transformer3w_dialog.ui
--rw-r--r--   0        0        0    56751 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/transformer_dialog.ui
--rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/ward_dialog.ui
--rw-r--r--   0        0        0    15494 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/xward_dialog.ui
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/LICENSE
--rw-r--r--   0        0        0    12030 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/README_PyPI.md
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/pyproject.toml
--rw-r--r--   0        0        0    13259 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/PKG-INFO
+-rw-r--r--   0        0        0    18506 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/README.md
+-rw-r--r--   0        0        0    84223 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/10_PF4.png
+-rw-r--r--   0        0        0    54206 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/11_PF_tooltips.png
+-rw-r--r--   0        0        0    88072 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/12_App_settings.png
+-rw-r--r--   0        0        0    50389 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/13_Disabling_nodes.png
+-rw-r--r--   0        0        0    69759 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/14_Context_menu.png
+-rw-r--r--   0        0        0    10969 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/15_Extension_manager.png
+-rw-r--r--   0        0        0   124772 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/1_Main_Window.png
+-rw-r--r--   0        0        0   122916 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/1_Main_Window_dark.png
+-rw-r--r--   0        0        0   149680 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/2_Dialogs.png
+-rw-r--r--   0        0        0    25172 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/3_Widgets.png
+-rw-r--r--   0        0        0   134645 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/4_Pandapower_DataFrames.png
+-rw-r--r--   0        0        0    16870 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/5_Connections_angle_b.png
+-rw-r--r--   0        0        0    21425 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/5_Connections_curved_b.png
+-rw-r--r--   0        0        0    21864 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/5_Connections_straight_b.png
+-rw-r--r--   0        0        0    13193 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/6_Line_and_transformer_nodes.png
+-rw-r--r--   0        0        0   136386 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/7_PF1.png
+-rw-r--r--   0        0        0   144782 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/8_PF2.png
+-rw-r--r--   0        0        0    83704 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/9_PF3.png
+-rwxr-xr-x   0        0        0    51862 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/Logo_CIESE_2021 y UTN_Sta_Fe.png
+-rw-r--r--   0        0        0    33067 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/img/app_icon.png
+-rw-r--r--   0        0        0    22462 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/Electrical_Grid_Simulator.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/__init__.py
+-rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/config.ini
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/egs_create_shortcut.py
+-rwxr-xr-x   0        0        0       98 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/egs_run.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/version.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/.idea/electricalsim.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/.idea/misc.xml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/.idea/modules.xml
+-rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/.idea/workspace.xml
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/extensions/extension_classes.py
+-rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/hotkeys/hotkey_functions.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/hotkeys/hotkeys.json
+-rwxr-xr-x   0        0        0    82539 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/icons/CIESE_UTN_Sta_Fe.png
+-rw-r--r--   0        0        0    33031 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/icons/app_icon.ico
+-rw-r--r--   0        0        0    33067 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/icons/app_icon.png
+-rwxr-xr-x   0        0        0    14363 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/icons/app_icon.svg
+-rw-r--r--   0        0        0    30015 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/lib/auxiliary.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/lib/calculations.py
+-rw-r--r--   0        0        0   208285 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/lib/electricalGraph.py
+-rw-r--r--   0        0        0    83266 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/lib/main_components.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/lib/table_widget.py
+-rw-r--r--   0        0        0    11797 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/about_dialog.ui
+-rw-r--r--   0        0        0    17328 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/aload_dialog.ui
+-rw-r--r--   0        0        0    17419 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/asgen_dialog.ui
+-rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/bus_dialog.ui
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/choose_bus_switch.ui
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/choose_generator_type.ui
+-rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/choose_line_type.ui
+-rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/choose_load_type.ui
+-rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/choose_transformer_type.ui
+-rw-r--r--   0        0        0    23084 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/dcline_dialog.ui
+-rw-r--r--   0        0        0   138693 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/dialogs.py
+-rw-r--r--   0        0        0    35106 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/ext_grid_dialog.ui
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/extension.ui
+-rw-r--r--   0        0        0    33034 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/gen_dialog.ui
+-rw-r--r--   0        0        0    16772 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/impedance_dialog.ui
+-rw-r--r--   0        0        0    31104 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/line_dialog.ui
+-rw-r--r--   0        0        0    25616 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/load_dialog.ui
+-rw-r--r--   0        0        0    12940 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/main_window.ui
+-rw-r--r--   0        0        0    12741 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/main_window_backup.ui
+-rw-r--r--   0        0        0    23184 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/motor_dialog.ui
+-rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/network_settings_dialog.ui
+-rw-r--r--   0        0        0    34604 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/pf_settings_widget.ui
+-rw-r--r--   0        0        0    50076 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/power_flow_dialog.ui
+-rw-r--r--   0        0        0    14082 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/settings_dialog.ui
+-rw-r--r--   0        0        0    38654 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/sgen_dialog.ui
+-rw-r--r--   0        0        0    11331 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/shunt_dialog.ui
+-rw-r--r--   0        0        0    10554 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/stdline_dialog.ui
+-rw-r--r--   0        0        0    10807 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/stdtransformer3w_dialog.ui
+-rw-r--r--   0        0        0    30234 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/stdtransformer_dialog.ui
+-rw-r--r--   0        0        0    26339 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/storage_dialog.ui
+-rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/switch_dialog.ui
+-rw-r--r--   0        0        0    65860 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/transformer3w_dialog.ui
+-rw-r--r--   0        0        0    56751 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/transformer_dialog.ui
+-rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/ward_dialog.ui
+-rw-r--r--   0        0        0    15494 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/src/electricalsim/ui/xward_dialog.ui
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/LICENSE
+-rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/README_PyPI.md
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 electricalsim-0.0.7.0/PKG-INFO
```

### Comparing `electricalsim-0.0.6.9/README.md` & `electricalsim-0.0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,73 +1,77 @@
 # Electrical Grid Simulator (EGS)
-The *Electrical Grid Simulator* (abbreviated as **EGS**) is a graphical user interface application for simulating electrical networks based on the [pandapower](https://www.pandapower.org/) library. The main objective is to allow the creation of mathematical models for steady-state electrical grids from a user-friendly interface.
+The *Electrical Grid Simulator* (abbreviated as **EGS**) is a graphical user interface application for simulating electrical networks based on the [pandapower](https://www.pandapower.org/) library. The main objective is to allow the creation of mathematical models for steady-state electrical grids from a user-friendly interface. It adds an extensions system for including new calculation or simulation algorithms. Extensions are implemented as standard Python packages, so they can be distributed through the [PyPI repository](https://pypi.org/).
 
 <p align = "center">
 <img src="./img/app_icon.png" alt="EGS logo" width="200">
 </p>
 
 EGS is developed at the *National Technological University, Santa Fe Regional Faculty* ([UTN-FRSF](https://www.frsf.utn.edu.ar/)), at the *Center for Research and Development in Electrical Engineering and Energy Systems* ([CIESE](https://www.frsf.utn.edu.ar/investigacion-y-vinculacion/investigacion-y-vinculacion/centros-y-grupos/ciese)), Argentina.
 
 <p align = "center">
 <img src="./img/Logo_CIESE_2021 y UTN_Sta_Fe.png" alt="" width="450">
 </p>
 
 > __Warning__ <br>
 > <span style="color:red">
-<b>This application is considered in alpha stage. So you can expect incomplete sections and some (or many) bugs. New changes may cause incompatibilities with older versions (old files that no longer work with newer versions of the program).</b>
+<b>This application is in an early stage of development. So you can expect incomplete sections and some (or many) bugs. New changes may cause incompatibilities with older versions (old files that no longer work with newer versions of the program).</b>
 </span>
 
 ## Goals
 - Providing a minimalistic, modern and good-looking interface.
 - Multiplatform: GNU/Linux, MS Windows and Apple MacOS (not tested on MacOS).
-- Providing an extension system to expand its capabilities **(WIP, not available yet)**.
+- Providing an extensions system to expand its capabilities **(new, starting in versión 0.0.6.9)**.
 
 ## How it is built
 EGS is built in Python and entirely from open source and free software. The main core components are:
 
+* The [pandapower](https://www.pandapower.org/) modeling and calculation library for electrical power systems.
 * The [Qt](https://www.qt.io/) toolkit with [PySide2](https://wiki.qt.io/Qt_for_Python) and [Qt.py](https://github.com/mottosso/Qt.py) bindings for the UI.
 * The [NodeGraphQt](https://github.com/jchanvfx/NodeGraphQt) library for building the graph (schematic network graphic).
 * The [PyQtDarkTheme](https://github.com/5yutan5/PyQtDarkTheme) package for applying modern themes (light and dark themes).
 * The [QtAwesome](https://github.com/spyder-ide/qtawesome) package for modern flat monochromatic icons.
 * The [matplotlib](https://matplotlib.org/) package for plotting calculation results.
 * Other scientific Python packages, mainly [NumPy](https://numpy.org/) and [pandas](https://pandas.pydata.org/).
 
 EGS is implemented as a Python package uploaded to the [PyPI repository](https://pypi.org/). ```pandapower``` and other packages listed above are set as dependencies.
 
-> __Note__ <br>
-> The ```NodeGraphQt``` is not available in PyPI. Hence, a copy of it is included within the EGS package.
-
 
 ## How it works
 Every time the user inserts and connects an element to the grid, the application replicates the addition in a ```pandapower``` network. Thus, the parameters of a component are updated in the ```pandapower``` network when they are modified from the graphical interface.
 
 The network configured from the interface is designated as **Graph**, while the corresponding ```pandapower``` model is denoted as **Data model**. This synchronization works in the **Graph -> Data model** direction, i.e. changes in the **Graph** are automatically registered into the **Data model**, and not the other way around. However, the contents of the **Data model** can be consulted at any time. 
 
 According to the structure proposed by the ```pandapower``` library, the **Data model** consists of a set of tables ([pandas DataFrame type objects](https://en.wikipedia.org/wiki/Pandas_(software))). Each table (**DataFrame**) contains the parameters of a certain type of component. The types of components supported by ```pandapower``` are those indicated in [this documentation link](https://pandapower.readthedocs.io/en/latest/elements.html). At this moment, most of these components are also supported by EGS.
 
 ![Main window: Graph view](img/1_Main_Window.png)
 <p align = "center">
 <i>Main window: Graph view</i>
 </p>
 
 
+![Main window: Data model view](img/15_Extension_manager.png)
+<p align = "center">
+<i>Extension manager: Select and execute extensions</i>
+</p>
+
+
 ![Main window: Data model view](img/4_Pandapower_DataFrames.png)
 <p align = "center">
 <i>Main window: Data model view - Tables arranged in tabs</i>
 </p>
 </br></br>
 
 The EGS main window is organized as follows:
 
 *  The main work area can display either the **Graph** or the **Data model**. The **Data model** is shown as a set of tables arranged in tabs. For more information about this data (including the meaning of column names), see the [pandapower documentation](https://pandapower.readthedocs.io/).
 * The side toolbar lists the supported components. An element is added to the **Graph** by clicking on the corresponding icon. In some cases, an icon may represent a category (e.g., loads).  In such cases, a dialog allows you to choose the required type within that category. For example, in the loads category, six different types are available.
 Switches work in a different way. According to ```pandapower```, switches can be added between two buses or between a bus and a line (AC line) or transformer. Thus, if you want to do the first, just select two buses and then click the switch button. On the contrary, if you want to add a switch next to a line (or transformer), select only the corresponding element and then click the switch button. In this case, a new dialog will allow you to select the bus.
-* The upper toolbar is divided into two parts. The left part contains the file functions and the calculation options. Here it is possible to open/save files, export only the **Data model** to JSON, or simply delete the network and start a new one. The *"play"* button opens the dialog for a power flow calculation. Meanwhile, the right side gives access to the basic network configuration (name, base system power and rated frequency) and to the application settings dialog.
+* The upper toolbar is divided into three parts. The left part contains the file functions and the calculation options. Here it is possible to open/save files, export only the **Data model** to JSON, or simply delete the network and start a new one. The *"play"* button opens the dialog for a power flow calculation. Meanwhile, the right side gives access to the basic network configuration (name, base system power and rated frequency) and to the application settings dialog. The extension manager is displayed at the center. In order to run an extensión, just select one of them and click the run button.
 * The status bar at the bottom will notify when the grid has been modified and has not been saved.
-* The menu bar includes the same options as the toolbars.
+* The menu bar includes most of the options available in the toolbars.
 
 ## Main features
 
 ### Nodes and ports
 A **node** element is a component added to the **Graph**. A **node** should not be mistaken for a network **bus**. Any component of the grid is represented by a **node** in the **Graph**. For this reason, there is a *node type* for each type of component supported by EGS.
 
 <p align = "center">
@@ -105,21 +109,21 @@
 When a bus node is added to the **Graph**, it is immediately inserted also into the **Data model**. But this is not the case with other components, which are included in the **Data model** only when they are connected. This behavior is due to the fact that ```pandapower``` requires the connection points to insert a new element into the grid (with the only exception of the bus component). But this has an advantage: you can disconnect an element and connect it again in a different place, without losing the parameters configured in the node, which remain stored in the **Graph**. EGS will take care of maintaining the synchronization with the **Data model**.
 
 ### Simulations and calculations
 With EGS you can build and set up the model of an electrical grid in a graphical way. The application also allows you to perform *AC balanced power flow* calculations (other calculations supported by ```pandapower``` may be added in the future). For other types of simulations and calculations, you can proceed according to two alternatives:
 
 1. Export the **Data model** and the last power flow results to a JSON format file ready to be imported from a Python script through ```pandapower```. Then, any calculation or processing can be done from the script. The export is done from the graphical interface, while the subsequent import is done as indicated [in the pandapower documentation](https://pandapower.readthedocs.io/en/latest/file_io.html#pandapower.from_json), using the ```pandapower.from_json()``` function.
 
-2. Incorporate the required calculation functionality from an extension developed in Python. This way, the calculation is executed from within EGS. **Note that this feature is one of the main goals of EGS, but is not yet available in this early stage of development.**
+2. Incorporate the required calculation functionality from an extension developed in Python. This way, the calculation is executed from within EGS. Extensions are implemented as regular Python packages. An Optimal Power Flow (OPF) extension is available in the PyPI repository (package name: **electricalsim-opf-quadratic**). **Instructions and a template for creating extensions will be available soon.**
 
 Models generated by EGS can be saved in a file containing both the **Graph** and the **Data model** (**.egs** file extension). You can then reopen the file whenever you need it and retrieve even the results of the last power flow run.
 
 
 ### Running an AC balanced power flow
-In order to run a power flow, click on the *"play"* button at the upper toolbar. A new dialog gets opened. The first tab allows you to configure the parameters of the numerical method (solver) and other model settings. Then, execute the calculation using the ***Run power flow*** button.
+In order to run a power flow, click on the ***play*** button at the upper toolbar. A new dialog gets opened. The first tab allows you to configure the parameters of the numerical method (solver) and other model settings. Then, execute the calculation using the ***Run power flow*** button.
 
 ![Power flow dialog - First tab (settings)](img/7_PF1.png)
 <p align = "center">
 <i>Power flow dialog - First tab (settings)</i>
 </p>
 </br>
 
@@ -299,10 +303,23 @@
 On MS Windows:
 ```bash
 python -m pip uninstall electricalsim
 ```
 
 Note that shortcuts added with the ```egs-create-shortcut``` command are not removed. So you must delete them manually.
 
+## Installing extensions
+
+Extensions available in the PyPI repository can be installed using ```pip```. For example, the Optimal Power Flow extension is installed with:
+
+```bash
+pip install electricalsim-opf-quadratic
+```
+
+On MS Windows:
+```bash
+python -m pip install electricalsim-opf-quadratic
+```
+
 # License
 
 This project uses the [MIT license](https://github.com/aloytag/electrical-grid-simulator/blob/main/LICENSE).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `electricalsim-0.0.6.9/img/10_PF4.png` & `electricalsim-0.0.7.0/img/10_PF4.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/img/11_PF_tooltips.png` & `electricalsim-0.0.7.0/img/11_PF_tooltips.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/img/12_App_settings.png` & `electricalsim-0.0.7.0/img/12_App_settings.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/img/13_Disabling_nodes.png` & `electricalsim-0.0.7.0/img/13_Disabling_nodes.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/img/14_Context_menu.png` & `electricalsim-0.0.7.0/img/14_Context_menu.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/img/3_Widgets.png` & `electricalsim-0.0.7.0/img/3_Widgets.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/img/5_Connections_angle_b.png` & `electricalsim-0.0.7.0/img/5_Connections_angle_b.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/img/5_Connections_curved_b.png` & `electricalsim-0.0.7.0/img/5_Connections_curved_b.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/img/5_Connections_straight_b.png` & `electricalsim-0.0.7.0/img/5_Connections_straight_b.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/img/6_Line_and_transformer_nodes.png` & `electricalsim-0.0.7.0/img/6_Line_and_transformer_nodes.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/img/7_PF1.png` & `electricalsim-0.0.7.0/img/7_PF1.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/img/8_PF2.png` & `electricalsim-0.0.7.0/img/8_PF2.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/img/9_PF3.png` & `electricalsim-0.0.7.0/img/9_PF3.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/img/Logo_CIESE_2021 y UTN_Sta_Fe.png` & `electricalsim-0.0.7.0/img/Logo_CIESE_2021 y UTN_Sta_Fe.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/img/app_icon.png` & `electricalsim-0.0.7.0/img/app_icon.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/Electrical_Grid_Simulator.py` & `electricalsim-0.0.7.0/src/electricalsim/Electrical_Grid_Simulator.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/config.ini` & `electricalsim-0.0.7.0/src/electricalsim/config.ini`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/egs_create_shortcut.py` & `electricalsim-0.0.7.0/src/electricalsim/egs_create_shortcut.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/.idea/workspace.xml` & `electricalsim-0.0.7.0/src/electricalsim/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/.idea/inspectionProfiles/Project_Default.xml` & `electricalsim-0.0.7.0/src/electricalsim/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/extensions/extension_classes.py` & `electricalsim-0.0.7.0/src/electricalsim/extensions/extension_classes.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/hotkeys/hotkey_functions.py` & `electricalsim-0.0.7.0/src/electricalsim/hotkeys/hotkey_functions.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/hotkeys/hotkeys.json` & `electricalsim-0.0.7.0/src/electricalsim/hotkeys/hotkeys.json`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/icons/CIESE_UTN_Sta_Fe.png` & `electricalsim-0.0.7.0/src/electricalsim/icons/CIESE_UTN_Sta_Fe.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/icons/app_icon.ico` & `electricalsim-0.0.7.0/src/electricalsim/icons/app_icon.ico`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/icons/app_icon.png` & `electricalsim-0.0.7.0/src/electricalsim/icons/app_icon.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/icons/app_icon.svg` & `electricalsim-0.0.7.0/src/electricalsim/icons/app_icon.svg`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/lib/auxiliary.py` & `electricalsim-0.0.7.0/src/electricalsim/lib/auxiliary.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/lib/electricalGraph.py` & `electricalsim-0.0.7.0/src/electricalsim/lib/electricalGraph.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/lib/main_components.py` & `electricalsim-0.0.7.0/src/electricalsim/lib/main_components.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/lib/table_widget.py` & `electricalsim-0.0.7.0/src/electricalsim/lib/table_widget.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/about_dialog.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/about_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/aload_dialog.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/aload_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/asgen_dialog.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/asgen_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/bus_dialog.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/bus_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/choose_bus_switch.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/choose_bus_switch.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/choose_generator_type.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/choose_generator_type.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/choose_line_type.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/choose_line_type.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/choose_load_type.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/choose_load_type.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/choose_transformer_type.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/choose_transformer_type.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/dcline_dialog.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/dcline_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/dialogs.py` & `electricalsim-0.0.7.0/src/electricalsim/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/ext_grid_dialog.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/ext_grid_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/extension.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/extension.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/gen_dialog.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/gen_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/impedance_dialog.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/impedance_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/line_dialog.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/line_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/load_dialog.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/load_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/main_window.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/main_window.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/main_window_backup.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/main_window_backup.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/motor_dialog.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/motor_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/network_settings_dialog.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/network_settings_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/pf_settings_widget.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/pf_settings_widget.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/power_flow_dialog.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/power_flow_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/settings_dialog.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/settings_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/sgen_dialog.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/sgen_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/shunt_dialog.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/shunt_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/stdline_dialog.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/stdline_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/stdtransformer3w_dialog.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/stdtransformer3w_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/stdtransformer_dialog.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/stdtransformer_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/storage_dialog.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/storage_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/switch_dialog.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/switch_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/transformer3w_dialog.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/transformer3w_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/transformer_dialog.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/transformer_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/ward_dialog.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/ward_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/src/electricalsim/ui/xward_dialog.ui` & `electricalsim-0.0.7.0/src/electricalsim/ui/xward_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/LICENSE` & `electricalsim-0.0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.9/pyproject.toml` & `electricalsim-0.0.7.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "electricalsim"
-version = "0.0.6.9"
+version = "0.0.7.0"
 author = "PhD Ariel S. Loyarte"
 authors = [
   { name="PhD Ariel S. Loyarte", email="aloyarte@frsf.utn.edu.ar" },
 ]
 description = "Graphical user interface for simulating electrical networks based on the pandapower library"
 readme = "README_PyPI.md"
 requires-python = ">=3.8"
```

