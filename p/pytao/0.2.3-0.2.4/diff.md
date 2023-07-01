# Comparing `tmp/pytao-0.2.3.tar.gz` & `tmp/pytao-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pytao/pytao/dist/.tmp-ei_eaipr/pytao-0.2.3.tar", last modified: Fri Mar  3 16:02:46 2023, max compression
+gzip compressed data, was "/home/runner/work/pytao/pytao/dist/.tmp-wkqdkud6/pytao-0.2.4.tar", last modified: Sat Jul  1 21:42:57 2023, max compression
```

## Comparing `pytao-0.2.3.tar` & `pytao-0.2.4.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 16:02:46.000000 pytao-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-03 16:02:35.000000 pytao-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-03 16:02:35.000000 pytao-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-03-03 16:02:46.000000 pytao-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-03-03 16:02:35.000000 pytao-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 16:02:46.000000 pytao-0.2.3/pytao/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-03 16:02:46.000000 pytao-0.2.3/pytao/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 16:02:46.000000 pytao-0.2.3/pytao/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/gui/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8970 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/gui/data_type_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    34616 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/gui/module_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    63664 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/gui/tao_base_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/gui/tao_beam_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/gui/tao_console.py
--rw-r--r--   0 runner    (1001) docker     (123)    50559 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/gui/tao_data_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/gui/tao_ele_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/gui/tao_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    62214 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/gui/tao_lat_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/gui/tao_misc_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/gui/tao_mpl_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/gui/tao_plot_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    95292 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/gui/tao_plot_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/gui/tao_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    40433 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/gui/tao_var_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)    42615 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/gui/tao_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    65690 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/gui/taoplot.py
--rw-r--r--   0 runner    (1001) docker     (123)   112592 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/interface_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 16:02:46.000000 pytao-0.2.3/pytao/misc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/misc/csr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/misc/csr_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/misc/markers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 16:02:46.000000 pytao-0.2.3/pytao/tao_ctypes/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/tao_ctypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/tao_ctypes/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/tao_ctypes/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/tao_ctypes/extra_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/tao_ctypes/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/tao_ctypes/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/tao_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 16:02:46.000000 pytao-0.2.3/pytao/tao_pexpect/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/tao_pexpect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/tao_pexpect/tao_pipe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 16:02:46.000000 pytao-0.2.3/pytao/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    27630 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/tests/test_interface_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 16:02:46.000000 pytao-0.2.3/pytao/util/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/util/evaluate_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/util/lattice_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/util/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-03-03 16:02:35.000000 pytao-0.2.3/pytao/util/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 16:02:46.000000 pytao-0.2.3/pytao.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-03-03 16:02:46.000000 pytao-0.2.3/pytao.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-03-03 16:02:46.000000 pytao-0.2.3/pytao.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 16:02:46.000000 pytao-0.2.3/pytao.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-03 16:02:46.000000 pytao-0.2.3/pytao.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-03 16:02:46.000000 pytao-0.2.3/pytao.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-03 16:02:35.000000 pytao-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-03 16:02:46.000000 pytao-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-03-03 16:02:35.000000 pytao-0.2.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-03-03 16:02:35.000000 pytao-0.2.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:42:57.000000 pytao-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 21:42:46.000000 pytao-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-01 21:42:46.000000 pytao-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-01 21:42:57.000000 pytao-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-01 21:42:46.000000 pytao-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:42:57.000000 pytao-0.2.4/pytao/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-01 21:42:57.000000 pytao-0.2.4/pytao/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:42:57.000000 pytao-0.2.4/pytao/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8970 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/data_type_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34616 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/module_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63664 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/tao_base_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/tao_beam_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/tao_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50559 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/tao_data_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/tao_ele_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/tao_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62214 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/tao_lat_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/tao_misc_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/tao_mpl_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/tao_plot_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95292 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/tao_plot_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/tao_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40433 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/tao_var_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42615 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/tao_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65690 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/gui/taoplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114650 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/interface_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:42:57.000000 pytao-0.2.4/pytao/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/misc/csr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/misc/csr_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/misc/markers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:42:57.000000 pytao-0.2.4/pytao/tao_ctypes/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/tao_ctypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/tao_ctypes/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/tao_ctypes/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/tao_ctypes/extra_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/tao_ctypes/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/tao_ctypes/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/tao_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:42:57.000000 pytao-0.2.4/pytao/tao_pexpect/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/tao_pexpect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/tao_pexpect/tao_pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:42:57.000000 pytao-0.2.4/pytao/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28283 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/tests/test_interface_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:42:57.000000 pytao-0.2.4/pytao/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/util/evaluate_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/util/lattice_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/util/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-07-01 21:42:46.000000 pytao-0.2.4/pytao/util/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:42:57.000000 pytao-0.2.4/pytao.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-01 21:42:57.000000 pytao-0.2.4/pytao.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-01 21:42:57.000000 pytao-0.2.4/pytao.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 21:42:57.000000 pytao-0.2.4/pytao.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-01 21:42:57.000000 pytao-0.2.4/pytao.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-01 21:42:57.000000 pytao-0.2.4/pytao.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-01 21:42:46.000000 pytao-0.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-01 21:42:57.000000 pytao-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-01 21:42:46.000000 pytao-0.2.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-07-01 21:42:46.000000 pytao-0.2.4/versioneer.py
```

### Comparing `pytao-0.2.3/LICENSE` & `pytao-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/PKG-INFO` & `pytao-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytao
-Version: 0.2.3
+Version: 0.2.4
 Home-page: https://www.classe.cornell.edu/bmad/tao.html
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyTao
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytao Version: 0.2.3 Home-page: https://
+Metadata-Version: 2.1 Name: pytao Version: 0.2.4 Home-page: https://
 www.classe.cornell.edu/bmad/tao.html Requires-Python: >=3.6 Description-
 Content-Type: text/markdown License-File: LICENSE # PyTao [PyTao]((https://
 bmad-sim.github.io/pytao/index.html)) is Python interface for [Tao](https://
 www.classe.cornell.edu/bmad/tao.html), which is based on the Bmad subroutine
 library for relativistic chargedâparticle and X-ray simulations in
 accelerators and storage rings. Documentation for Bmad and Tao, as well as
 information for downloading the code if needed is given on the [Bmad website]
```

### Comparing `pytao-0.2.3/README.md` & `pytao-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/__init__.py` & `pytao-0.2.4/pytao/__init__.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/gui/__init__.py` & `pytao-0.2.4/pytao/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/gui/data_type_list.py` & `pytao-0.2.4/pytao/gui/data_type_list.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/gui/main.py` & `pytao-0.2.4/pytao/gui/main.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/gui/module_check.py` & `pytao-0.2.4/pytao/gui/module_check.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/gui/tao_base_windows.py` & `pytao-0.2.4/pytao/gui/tao_base_windows.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/gui/tao_beam_windows.py` & `pytao-0.2.4/pytao/gui/tao_beam_windows.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/gui/tao_console.py` & `pytao-0.2.4/pytao/gui/tao_console.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/gui/tao_data_windows.py` & `pytao-0.2.4/pytao/gui/tao_data_windows.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/gui/tao_ele_location.py` & `pytao-0.2.4/pytao/gui/tao_ele_location.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/gui/tao_interface.py` & `pytao-0.2.4/pytao/gui/tao_interface.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/gui/tao_lat_windows.py` & `pytao-0.2.4/pytao/gui/tao_lat_windows.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/gui/tao_misc_windows.py` & `pytao-0.2.4/pytao/gui/tao_misc_windows.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/gui/tao_mpl_toolbar.py` & `pytao-0.2.4/pytao/gui/tao_mpl_toolbar.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/gui/tao_plot_dict.py` & `pytao-0.2.4/pytao/gui/tao_plot_dict.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/gui/tao_plot_windows.py` & `pytao-0.2.4/pytao/gui/tao_plot_windows.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/gui/tao_set.py` & `pytao-0.2.4/pytao/gui/tao_set.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/gui/tao_var_windows.py` & `pytao-0.2.4/pytao/gui/tao_var_windows.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/gui/tao_widget.py` & `pytao-0.2.4/pytao/gui/tao_widget.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/gui/taoplot.py` & `pytao-0.2.4/pytao/gui/taoplot.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/interface_commands.py` & `pytao-0.2.4/pytao/interface_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1278,15 +1278,15 @@
     Parameters
     ----------
     ele_id
     which : default=model
     
     Returns
     -------
-    string_list
+    dict of attributes and values
     
     Notes
     -----
     Command syntax:
       python ele:control_var {ele_id}|{which}
     
     Where:
@@ -2376,14 +2376,71 @@
     
     """
     cmd = f'python global'
     if verbose: print(cmd)
     return __execute(tao, cmd, as_dict, raises, method_name='tao_global', cmd_type='string_list')
 
 
+def global_optimization(tao, *, verbose=False, as_dict=True, raises=True):
+    """
+    
+    Output optimization parameters.
+    Also see global:opti_de.
+    
+    Returns
+    -------
+    string_list
+    
+    Notes
+    -----
+    Command syntax:
+      python global:optimization
+    
+    Output syntax is parameter list form. See documentation at the beginning of this file.
+    
+    Examples
+    --------
+    Example: 1
+     init: -init $ACC_ROOT_DIR/regression_tests/python_test/cesr/tao.init
+     args:
+    
+    """
+    cmd = f'python global:optimization'
+    if verbose: print(cmd)
+    return __execute(tao, cmd, as_dict, raises, method_name='global_optimization', cmd_type='string_list')
+
+
+def global_opti_de(tao, *, verbose=False, as_dict=True, raises=True):
+    """
+    
+    Output DE optimization parameters.
+    
+    Returns
+    -------
+    string_list
+    
+    Notes
+    -----
+    Command syntax:
+      python global:opti_de
+    
+    Output syntax is parameter list form. See documentation at the beginning of this file.
+    
+    Examples
+    --------
+    Example: 1
+     init: -init $ACC_ROOT_DIR/regression_tests/python_test/cesr/tao.init
+     args:
+    
+    """
+    cmd = f'python global:opti_de'
+    if verbose: print(cmd)
+    return __execute(tao, cmd, as_dict, raises, method_name='global_opti_de', cmd_type='string_list')
+
+
 def help(tao, *, verbose=False, as_dict=True, raises=True):
     """
     
     Output list of "help xxx" topics
     
     Returns
     -------
@@ -2716,15 +2773,16 @@
 def merit(tao, *, verbose=False, as_dict=True, raises=True):
     """
     
     Output merit value.
     
     Returns
     -------
-    string_list
+    merit: float
+        Value of the merit function
     
     Notes
     -----
     Command syntax:
       python merit
     
     Examples
@@ -3670,14 +3728,42 @@
     
     """
     cmd = f'python show {line}'
     if verbose: print(cmd)
     return __execute(tao, cmd, as_dict, raises, method_name='show', cmd_type='string_list')
 
 
+def space_charge_com(tao, *, verbose=False, as_dict=True, raises=True):
+    """
+    
+    Output space_charge_com structure parameters.
+    
+    Returns
+    -------
+    string_list
+    
+    Notes
+    -----
+    Command syntax:
+      python space_charge_com
+    
+    Output syntax is parameter list form. See documentation at the beginning of this file.
+    
+    Examples
+    --------
+    Example: 1
+     init: -init $ACC_ROOT_DIR/regression_tests/python_test/cesr/tao.init
+     args:
+    
+    """
+    cmd = f'python space_charge_com'
+    if verbose: print(cmd)
+    return __execute(tao, cmd, as_dict, raises, method_name='space_charge_com', cmd_type='string_list')
+
+
 def species_to_int(tao, species_str, *, verbose=False, as_dict=True, raises=True):
     """
     
     Convert species name to corresponding integer
     
     Parameters
     ----------
```

### Comparing `pytao-0.2.3/pytao/misc/csr.py` & `pytao-0.2.4/pytao/misc/csr.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/misc/csr_plot.py` & `pytao-0.2.4/pytao/misc/csr_plot.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/misc/markers.py` & `pytao-0.2.4/pytao/misc/markers.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/tao_ctypes/core.py` & `pytao-0.2.4/pytao/tao_ctypes/core.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/tao_ctypes/evaluate.py` & `pytao-0.2.4/pytao/tao_ctypes/evaluate.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/tao_ctypes/extra_commands.py` & `pytao-0.2.4/pytao/tao_ctypes/extra_commands.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/tao_ctypes/tools.py` & `pytao-0.2.4/pytao/tao_ctypes/tools.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/tao_ctypes/util.py` & `pytao-0.2.4/pytao/tao_ctypes/util.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/tao_interface.py` & `pytao-0.2.4/pytao/tao_interface.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/tao_pexpect/tao_pipe.py` & `pytao-0.2.4/pytao/tao_pexpect/tao_pipe.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/tests/test_interface_commands.py` & `pytao-0.2.4/pytao/tests/test_interface_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -342,14 +342,26 @@
         
 def test_tao_global_1():
     
     tao = Tao(os.path.expandvars('-init $ACC_ROOT_DIR/regression_tests/python_test/cesr/tao.init -noplot'))
     ret = interface_commands.tao_global(tao)
             
         
+def test_global_optimization_1():
+    
+    tao = Tao(os.path.expandvars('-init $ACC_ROOT_DIR/regression_tests/python_test/cesr/tao.init -noplot'))
+    ret = interface_commands.global_optimization(tao)
+            
+        
+def test_global_opti_de_1():
+    
+    tao = Tao(os.path.expandvars('-init $ACC_ROOT_DIR/regression_tests/python_test/cesr/tao.init -noplot'))
+    ret = interface_commands.global_opti_de(tao)
+            
+        
 def test_help_1():
     
     tao = Tao(os.path.expandvars('-init $ACC_ROOT_DIR/regression_tests/python_test/cesr/tao.init -noplot'))
     ret = interface_commands.help(tao)
             
         
 def test_inum_1():
@@ -552,14 +564,20 @@
         
 def test_show_1():
     
     tao = Tao(os.path.expandvars('-init $ACC_ROOT_DIR/regression_tests/python_test/cesr/tao.init -noplot'))
     ret = interface_commands.show(tao, line='-python')
             
         
+def test_space_charge_com_1():
+    
+    tao = Tao(os.path.expandvars('-init $ACC_ROOT_DIR/regression_tests/python_test/cesr/tao.init -noplot'))
+    ret = interface_commands.space_charge_com(tao)
+            
+        
 def test_species_to_int_1():
     
     tao = Tao(os.path.expandvars('-init $ACC_ROOT_DIR/regression_tests/python_test/cesr/tao.init -noplot'))
     ret = interface_commands.species_to_int(tao, species_str='electron')
             
         
 def test_species_to_str_1():
```

### Comparing `pytao-0.2.3/pytao/util/data.py` & `pytao-0.2.4/pytao/util/data.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/util/evaluate_expression.py` & `pytao-0.2.4/pytao/util/evaluate_expression.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/util/lattice_element.py` & `pytao-0.2.4/pytao/util/lattice_element.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/util/parameters.py` & `pytao-0.2.4/pytao/util/parameters.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/pytao/util/parsers.py` & `pytao-0.2.4/pytao/util/parsers.py`

 * *Files 9% similar despite different names*

```diff
@@ -122,14 +122,34 @@
     for iu, vals in universes.items():
         out[iu] = np.array(vals).astype(float)
         
     return out
 
 
 
+def parse_ele_control_var(lines):
+    """
+    Parses the output of tao python ele_control_var
+    
+    Parameters
+    ----------
+    lines : list of str
+        The output of the 'python ele_control_var' command to parse
+    
+    Returns
+    -------
+    dict of attributes and values
+    
+    """
+    d = {}
+    for line in lines:
+        ix, name, value = line.split(';')
+        d[name] = float(value)    
+    return d
+
 def parse_lat_ele_list(lines):
     """
     Parses the output of tao python lat_ele_list
     
     Parameters
     ----------
     lines : list of str
@@ -161,14 +181,32 @@
         
     
     """
     m7 = np.array([[float(x) for x in line.split(';')[1:]] for line in lines])
     return {'mat6':m7[:,0:6], 'vec0':m7[:,6]}
 
 
+def parse_merit(lines):
+    """
+    Parses the output of a tao python merit
+    
+    Parameters
+    ----------
+    lines : list of str
+        The output of the 'python matrix' command to parse
+    
+    Returns
+    -------
+    merit: float
+        Value of the merit function
+    """
+    assert len(lines) == 1
+    return float(lines[0])
+
+
 def parse_plot_list(lines):
     """
     Parses the output of the `python plot_list` command.
     
     This could be region or template data.
```

### Comparing `pytao-0.2.3/pytao.egg-info/PKG-INFO` & `pytao-0.2.4/pytao.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytao
-Version: 0.2.3
+Version: 0.2.4
 Home-page: https://www.classe.cornell.edu/bmad/tao.html
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyTao
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytao Version: 0.2.3 Home-page: https://
+Metadata-Version: 2.1 Name: pytao Version: 0.2.4 Home-page: https://
 www.classe.cornell.edu/bmad/tao.html Requires-Python: >=3.6 Description-
 Content-Type: text/markdown License-File: LICENSE # PyTao [PyTao]((https://
 bmad-sim.github.io/pytao/index.html)) is Python interface for [Tao](https://
 www.classe.cornell.edu/bmad/tao.html), which is based on the Bmad subroutine
 library for relativistic chargedâparticle and X-ray simulations in
 accelerators and storage rings. Documentation for Bmad and Tao, as well as
 information for downloading the code if needed is given on the [Bmad website]
```

### Comparing `pytao-0.2.3/pytao.egg-info/SOURCES.txt` & `pytao-0.2.4/pytao.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/setup.py` & `pytao-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `pytao-0.2.3/versioneer.py` & `pytao-0.2.4/versioneer.py`

 * *Files identical despite different names*

