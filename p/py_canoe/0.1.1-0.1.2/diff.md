# Comparing `tmp/py_canoe-0.1.1.tar.gz` & `tmp/py_canoe-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_canoe-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "py_canoe-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `py_canoe-0.1.1.tar` & `py_canoe-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     3699 2023-06-21 03:21:26.026953 py_canoe-0.1.1/.gitignore
--rw-r--r--   0        0        0     5330 2023-06-21 02:44:58.263085 py_canoe-0.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1095 2023-06-21 02:44:58.263085 py_canoe-0.1.1/LICENSE
--rw-r--r--   0        0        0     1919 2023-06-21 02:44:58.263085 py_canoe-0.1.1/README.md
--rw-r--r--   0        0        0      147 2023-06-21 02:44:58.263085 py_canoe-0.1.1/_config.yml
--rw-r--r--   0        0        0     1852 2023-06-21 02:44:58.273095 py_canoe-0.1.1/docs/index.md
--rw-r--r--   0        0        0      507 2023-06-21 02:44:58.273095 py_canoe-0.1.1/mkdocs.yml
--rw-r--r--   0        0        0      668 2023-06-21 02:44:58.273095 py_canoe-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       60 2023-06-21 02:44:58.273095 py_canoe-0.1.1/requirements.txt
--rwxr-xr-x   0        0        0      635 2023-06-29 17:56:00.911096 py_canoe-0.1.1/scripts/deploy_docs_to_github.bat
--rwxr-xr-x   0        0        0     1526 2023-06-29 17:56:00.911096 py_canoe-0.1.1/scripts/install_dependencies.bat
--rwxr-xr-x   0        0        0      589 2023-06-21 02:44:58.273095 py_canoe-0.1.1/scripts/run_pytests.bat
--rwxr-xr-x   0        0        0      608 2023-06-21 02:44:58.273095 py_canoe-0.1.1/scripts/upload_package_to_pypi.bat
--rw-r--r--   0        0        0        0 2023-06-29 17:34:50.054974 py_canoe-0.1.1/src/__int__.py
--rw-r--r--   0        0        0    47393 2023-06-29 17:34:50.054974 py_canoe-0.1.1/src/py_canoe.py
--rw-r--r--   0        0        0       31 2023-06-21 02:44:58.283091 py_canoe-0.1.1/tests/__int__.py
--rw-r--r--   0        0        0     2192 2023-06-21 02:44:58.283091 py_canoe-0.1.1/tests/demo_cfg/CANdb/easy.dbc
--rw-r--r--   0        0        0  1106768 2023-06-21 02:44:58.293092 py_canoe-0.1.1/tests/demo_cfg/CDD/UDS-ExampleEcu-5.0.2.cdd
--rw-r--r--   0        0        0    11560 2023-06-29 17:34:50.054974 py_canoe-0.1.1/tests/demo_cfg/Logs/demo_log.blf
--rw-r--r--   0        0        0     3708 2023-06-21 02:44:58.293092 py_canoe-0.1.1/tests/demo_cfg/Nodes/SimDiagECU.can
--rw-r--r--   0        0        0      928 2023-06-21 02:44:58.293092 py_canoe-0.1.1/tests/demo_cfg/Nodes/system_events.can
--rw-r--r--   0        0        0      256 2023-06-21 02:44:58.293092 py_canoe-0.1.1/tests/demo_cfg/Nodes/system_variables.can
--rw-r--r--   0        0        0     5436 2023-06-21 02:44:58.303089 py_canoe-0.1.1/tests/demo_cfg/Panels/sys_var_demo_panel.xvp
--rw-r--r--   0        0        0   203010 2023-06-29 17:34:50.064968 py_canoe-0.1.1/tests/demo_cfg/demo.cfg
--rw-r--r--   0        0        0   194788 2023-06-29 17:34:50.064968 py_canoe-0.1.1/tests/demo_cfg/demo_offline.cfg
--rw-r--r--   0        0        0     3627 2023-06-29 17:38:24.013024 py_canoe-0.1.1/tests/test_canoe.py
--rw-r--r--   0        0        0     2401 1970-01-01 00:00:00.000000 py_canoe-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3699 2023-06-21 03:21:26.026953 py_canoe-0.1.2/.gitignore
+-rw-r--r--   0        0        0     5330 2023-06-21 02:44:58.263085 py_canoe-0.1.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1095 2023-06-21 02:44:58.263085 py_canoe-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1919 2023-06-21 02:44:58.263085 py_canoe-0.1.2/README.md
+-rw-r--r--   0        0        0      147 2023-06-21 02:44:58.263085 py_canoe-0.1.2/_config.yml
+-rw-r--r--   0        0        0     1852 2023-06-21 02:44:58.273095 py_canoe-0.1.2/docs/index.md
+-rw-r--r--   0        0        0      507 2023-06-21 02:44:58.273095 py_canoe-0.1.2/mkdocs.yml
+-rw-r--r--   0        0        0      668 2023-06-21 02:44:58.273095 py_canoe-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       60 2023-06-21 02:44:58.273095 py_canoe-0.1.2/requirements.txt
+-rwxr-xr-x   0        0        0      635 2023-06-29 17:56:00.911096 py_canoe-0.1.2/scripts/deploy_docs_to_github.bat
+-rwxr-xr-x   0        0        0     1526 2023-06-29 17:56:00.911096 py_canoe-0.1.2/scripts/install_dependencies.bat
+-rwxr-xr-x   0        0        0      589 2023-06-21 02:44:58.273095 py_canoe-0.1.2/scripts/run_pytests.bat
+-rwxr-xr-x   0        0        0      608 2023-06-21 02:44:58.273095 py_canoe-0.1.2/scripts/upload_package_to_pypi.bat
+-rw-r--r--   0        0        0        0 2023-06-29 17:34:50.054974 py_canoe-0.1.2/src/__int__.py
+-rw-r--r--   0        0        0    47414 2023-07-01 18:10:39.507550 py_canoe-0.1.2/src/py_canoe.py
+-rw-r--r--   0        0        0       31 2023-06-21 02:44:58.283091 py_canoe-0.1.2/tests/__int__.py
+-rw-r--r--   0        0        0     2192 2023-06-21 02:44:58.283091 py_canoe-0.1.2/tests/demo_cfg/CANdb/easy.dbc
+-rw-r--r--   0        0        0  1106768 2023-06-21 02:44:58.293092 py_canoe-0.1.2/tests/demo_cfg/CDD/UDS-ExampleEcu-5.0.2.cdd
+-rw-r--r--   0        0        0    11560 2023-06-29 17:34:50.054974 py_canoe-0.1.2/tests/demo_cfg/Logs/demo_log.blf
+-rw-r--r--   0        0        0     3708 2023-06-21 02:44:58.293092 py_canoe-0.1.2/tests/demo_cfg/Nodes/SimDiagECU.can
+-rw-r--r--   0        0        0      928 2023-06-21 02:44:58.293092 py_canoe-0.1.2/tests/demo_cfg/Nodes/system_events.can
+-rw-r--r--   0        0        0      256 2023-06-21 02:44:58.293092 py_canoe-0.1.2/tests/demo_cfg/Nodes/system_variables.can
+-rw-r--r--   0        0        0     5436 2023-06-21 02:44:58.303089 py_canoe-0.1.2/tests/demo_cfg/Panels/sys_var_demo_panel.xvp
+-rw-r--r--   0        0        0   203010 2023-06-29 17:34:50.064968 py_canoe-0.1.2/tests/demo_cfg/demo.cfg
+-rw-r--r--   0        0        0   194788 2023-06-29 17:34:50.064968 py_canoe-0.1.2/tests/demo_cfg/demo_offline.cfg
+-rw-r--r--   0        0        0     3925 2023-07-01 18:13:10.224114 py_canoe-0.1.2/tests/test_canoe.py
+-rw-r--r--   0        0        0     2401 1970-01-01 00:00:00.000000 py_canoe-0.1.2/PKG-INFO
```

### Comparing `py_canoe-0.1.1/.gitignore` & `py_canoe-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.1/CODE_OF_CONDUCT.md` & `py_canoe-0.1.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.1/LICENSE` & `py_canoe-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.1/README.md` & `py_canoe-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.1/docs/index.md` & `py_canoe-0.1.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.1/pyproject.toml` & `py_canoe-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.1/scripts/deploy_docs_to_github.bat` & `py_canoe-0.1.2/scripts/deploy_docs_to_github.bat`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.1/scripts/install_dependencies.bat` & `py_canoe-0.1.2/scripts/install_dependencies.bat`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.1/scripts/run_pytests.bat` & `py_canoe-0.1.2/scripts/run_pytests.bat`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.1/scripts/upload_package_to_pypi.bat` & `py_canoe-0.1.2/scripts/upload_package_to_pypi.bat`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.1/src/py_canoe.py` & `py_canoe-0.1.2/src/py_canoe.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,56 @@
 """Python package for controlling Vector CANoe tool"""
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 # Import Python Libraries here
 import os
+import sys
 import logging
+import pythoncom
+import win32com.client
 from typing import Union
 from logging import handlers
-from win32com.client import *
-from win32com.client.connect import *
 from time import sleep as wait
 
-
 def DoEvents():
     pythoncom.PumpWaitingMessages()
     wait(.1)
 
+def DoEventsUntil(cond):
+    while not cond():
+        DoEvents()
+
+class CanoeApplicationEvents:
+    """Handler for CANoe Application events"""
+
+    @staticmethod
+    def OnOpen():
+        print('canoe opened')
+        CANoe.CANOE_APP_OPENED = True
+        CANoe.CANOE_APP_CLOSED = False
+
+    @staticmethod
+    def OnQuit():
+        print('canoe closed')
+        CANoe.CANOE_APP_OPENED = False
+        CANoe.CANOE_APP_CLOSED = True
+
+class CanoeMeasurementEvents:
+    """Handler for CANoe Measurement events"""
+
+    @staticmethod
+    def OnStart():
+        CANoe.CANOE_MEAS_STARTED = True
+        CANoe.CANOE_MEAS_STOPPED = False
+
+    @staticmethod
+    def OnStop():
+        CANoe.CANOE_MEAS_STARTED = False
+        CANoe.CANOE_MEAS_STOPPED = True
 
 class CANoe:
     r"""The CANoe class represents the CANoe application.
     The CANoe class is the foundation for the object hierarchy.
     You can reach all other methods from the CANoe class instance.
 
     Examples:
@@ -27,245 +58,242 @@
         >>> canoe_inst = CANoe(py_canoe_log_dir=r'D:\.py_canoe')
         >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
         >>> canoe_inst.start_measurement()
         >>> wait(10)
         >>> canoe_inst.stop_measurement()
         >>> canoe_inst.quit()
     """
-    Started = False
-    Stopped = False
+    CANOE_APP_OPENED = False
+    CANOE_APP_CLOSED = False
+    CANOE_MEAS_STARTED = False
+    CANOE_MEAS_STOPPED = False
 
-    def __init__(self, py_canoe_log_dir='') -> None:
+    def __init__(self, py_canoe_log_dir=''):
         """
         Args:
             py_canoe_log_dir (str): directory to store py_canoe log. example 'D:\\.py_canoe'
         """
         self.log = logging.getLogger('CANOE_LOG')
         self.__py_canoe_log_initialisation(py_canoe_log_dir)
-        self.__canoe_objects = {}
-        self.__dispatch_canoe()
-        self.wait_for_start = lambda: DoEventsUntil(lambda: CANoe.Started)
-        self.wait_for_stop = lambda: DoEventsUntil(lambda: CANoe.Stopped)
-        self.__triggered_canoe_quit = False
-        self.__BUS_TYPES = {'CAN': 1, 'J1939': 2, 'TTP': 4, 'LIN': 5, 'MOST': 6, 'Kline': 14}
-        self.__diag_ecu_qualifiers_dictionary = {}
-        self.__replay_blocks_obj_dictionary = {}
+        self.wait_for_canoe_app_to_open = None
+        self.wait_for_canoe_meas_to_start = None
+        self.wait_for_canoe_meas_to_stop = None
+        self.wait_for_canoe_app_to_close = None
+        self.__diag_ecu_qualifiers_dictionary = dict()
+        self.__replay_blocks_obj_dictionary = dict()
+        self.__canoe_objects = dict()
+        self.__canoe_info = dict()
 
     def __py_canoe_log_initialisation(self, py_canoe_log_dir):
         self.log.setLevel(logging.DEBUG)
         log_format = logging.Formatter("%(asctime)s [CANOE_LOG] [%(levelname)-5.5s]  %(message)s")
         ch = logging.StreamHandler(sys.stdout)
         ch.setFormatter(log_format)
         self.log.addHandler(ch)
         if py_canoe_log_dir != '' and not os.path.exists(py_canoe_log_dir):
             os.makedirs(py_canoe_log_dir, exist_ok=True)
         if os.path.exists(py_canoe_log_dir):
             fh = handlers.RotatingFileHandler(fr'{py_canoe_log_dir}\py_canoe.log', maxBytes=(1024 * 50), backupCount=20)
             fh.setFormatter(log_format)
             self.log.addHandler(fh)
 
-    def __dispatch_canoe(self):
-        app = DispatchEx('CANoe.Application')
-        app.Configuration.Modified = False
-        ver = app.Version
-        self.log.info(f'Dispatched CANoe Application {ver.major}.{ver.minor}.{ver.Build}...')
-        self.__canoe_objects['Application'] = app
-        self.__canoe_objects['Application.Configuration'] = self.__canoe_objects['Application'].Configuration
-        self.__canoe_objects['Application.Measurement'] = self.__canoe_objects['Application'].Measurement
-        self.__canoe_objects['Application.Measurement.Running'] = self.__canoe_objects['Application.Measurement'].Running
-        self.wait_for_start = lambda: DoEventsUntil(lambda: CANoe.Started)
-        self.wait_for_stop = lambda: DoEventsUntil(lambda: CANoe.Stopped)
-        WithEvents(self.__canoe_objects['Application.Measurement'], CanoeMeasurementEvents)
-
     def __fetch_canoe_networks_data(self) -> dict:
-        self.__canoe_objects['Application.Networks'] = self.__canoe_objects['Application'].Networks
         canoe_networks_dict = {}
-        for network in self.__canoe_objects['Application.Networks']:
+        for network in self.__canoe_objects['Networks']:
             network_name = network.Name
             canoe_networks_dict[network_name] = {}
             canoe_networks_dict[network_name]['network_obj'] = network
-            # canoe_networks_dict[network_name]['BusType'] = network.BusType
             canoe_networks_dict[network_name]['Devices'] = {}
             for device in network.Devices:
                 device_name = device.Name
                 canoe_networks_dict[network_name]['Devices'][device_name] = {}
                 canoe_networks_dict[network_name]['Devices'][device_name]['device_obj'] = device
                 try:
                     canoe_networks_dict[network_name]['Devices'][device_name]['diagnostic_obj'] = device.Diagnostic
                     self.__diag_ecu_qualifiers_dictionary[device_name] = canoe_networks_dict[network_name]['Devices'][device_name]['diagnostic_obj']
                 except pythoncom.com_error:
                     canoe_networks_dict[network_name]['Devices'][device_name]['diagnostic_obj'] = None
         return canoe_networks_dict
 
+    def __fetch_canoe_bus_data(self) -> dict:
+        self.__canoe_objects['ReplayCollection'] = self.__canoe_objects['Bus'].ReplayCollection
+        self.__canoe_objects['Nodes'] = self.__canoe_objects['Bus'].Nodes
+        canoe_bus_dict = {}
+        replay_blocks_dict = {}
+        nodes_dict = {}
+        for replay_block in self.__canoe_objects['ReplayCollection']:
+            replay_blocks_dict[replay_block.Name] = replay_block
+        for node in self.__canoe_objects['Nodes']:
+            nodes_dict[node.Name] = node
+        canoe_bus_dict['replay_block_objs'] = self.__replay_blocks_obj_dictionary = replay_blocks_dict
+        canoe_bus_dict['node_objs'] = nodes_dict
+        return canoe_bus_dict
+
     def __fetch_canoe_system_data(self) -> dict:
-        self.__canoe_objects['Application.System'] = self.__canoe_objects['Application'].System
-        self.__canoe_objects['Application.System.Namespaces'] = self.__canoe_objects['Application.System'].Namespaces
-        self.__canoe_objects['Application.System.VariablesFiles'] = self.__canoe_objects['Application.System'].VariablesFiles
         canoe_system_dict = {'Namespaces': {},
                              'VariablesFiles': {}}
         namespaces_dict = {}
-        for namespace in self.__canoe_objects['Application.System.Namespaces']:
+        for namespace in self.__canoe_objects['Namespaces']:
             namespaces_dict[namespace.Name] = namespace
         canoe_system_dict['Namespaces'] = namespaces_dict
         variable_files_dict = {}
-        for variables_file in self.__canoe_objects['Application.System.VariablesFiles']:
+        for variables_file in self.__canoe_objects['VariablesFiles']:
             variable_files_dict[variables_file.Name] = variables_file
         canoe_system_dict['VariablesFiles'] = variable_files_dict
         return canoe_system_dict
 
-    def __fetch_canoe_bus_data(self) -> dict:
-        self.__canoe_objects['Application.Bus'] = self.__canoe_objects['Application'].Bus
-        self.__canoe_objects['Application.Bus.ReplayCollection'] = self.__canoe_objects['Application.Bus'].ReplayCollection
-        self.__canoe_objects['Application.Bus.Nodes'] = self.__canoe_objects['Application.Bus'].Nodes
-        canoe_bus_dict = {}
-        replay_blocks_dict = {}
-        nodes_dict = {}
-        for replay_block in self.__canoe_objects['Application.Bus.ReplayCollection']:
-            replay_blocks_dict[replay_block.Name] = replay_block
-        for node in self.__canoe_objects['Application.Bus.Nodes']:
-            nodes_dict[node.Name] = node
-        canoe_bus_dict['replay_block_objs'] = self.__replay_blocks_obj_dictionary = replay_blocks_dict
-        canoe_bus_dict['node_objs'] = nodes_dict
-        return canoe_bus_dict
-
     def open(self, canoe_cfg: str, visible=True, auto_save=False, prompt_user=False) -> None:
         r"""Loads CANoe configuration.
 
         Args:
             canoe_cfg (str): The complete path for the CANoe configuration.
             visible (bool): True if you want to see CANoe UI. Defaults to True.
             auto_save (bool, optional): A boolean value that indicates whether the active configuration should be saved if it has been changed. Defaults to False.
             prompt_user (bool, optional): A boolean value that indicates whether the user should intervene in error situations. Defaults to False.
 
         Examples:
             >>> # The following example opens a configuration
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
         """
-        if self.__triggered_canoe_quit:
-            self.__dispatch_canoe()
+        pythoncom.CoInitialize()
+        self.__canoe_objects['Application'] = win32com.client.Dispatch('CANoe.Application')
+        cav = self.__canoe_objects['Application'].Version
+        self.log.info(f'Dispatched Vector CANoe Application {cav.major}.{cav.minor}.{cav.Build}')
+        self.__canoe_objects['Application'].Visible = visible
+        self.__canoe_objects['Application'].Configuration.Modified = False
         if os.path.isfile(canoe_cfg):
             self.log.info(f'CANoe cfg "{canoe_cfg}" found.')
-            self.__canoe_objects['Application'].Visible = visible
             self.__canoe_objects['Application'].Open(canoe_cfg, auto_save, prompt_user)
             self.log.info(f'loaded CANoe config "{canoe_cfg}"')
-            self.__fetch_canoe_networks_data()
-            self.__fetch_canoe_system_data()
-            self.__fetch_canoe_bus_data()
+            self.__canoe_objects['Bus'] = win32com.client.Dispatch(self.__canoe_objects['Application'].Bus)
+            self.__canoe_objects['Configuration'] = win32com.client.Dispatch(self.__canoe_objects['Application'].Configuration)
+            self.__canoe_objects['Environment'] = win32com.client.Dispatch(self.__canoe_objects['Application'].Environment)
+            self.__canoe_objects['Measurement'] = win32com.client.Dispatch(self.__canoe_objects['Application'].Measurement)
+            self.__canoe_objects['Networks'] = win32com.client.Dispatch(self.__canoe_objects['Application'].Networks)
+            self.__canoe_objects['System'] = win32com.client.Dispatch(self.__canoe_objects['Application'].System)
+            self.__canoe_objects['Namespaces'] = win32com.client.Dispatch(self.__canoe_objects['System'].Namespaces)
+            self.__canoe_objects['VariablesFiles'] = win32com.client.Dispatch(self.__canoe_objects['System'].VariablesFiles)
+            self.__canoe_objects['UI'] = win32com.client.Dispatch(self.__canoe_objects['Application'].UI)
+            self.wait_for_canoe_meas_to_start = lambda: DoEventsUntil(lambda: CANoe.CANOE_MEAS_STARTED)
+            self.wait_for_canoe_meas_to_stop = lambda: DoEventsUntil(lambda: CANoe.CANOE_MEAS_STOPPED)
+            win32com.client.WithEvents(self.__canoe_objects['Measurement'], CanoeMeasurementEvents)
+            self.__canoe_info['networks'] = self.__fetch_canoe_networks_data()
+            self.__canoe_info['bus'] = self.__fetch_canoe_bus_data()
+            self.__canoe_info['system'] = self.__fetch_canoe_system_data()
         else:
             self.log.info(f'CANoe cfg "{canoe_cfg}" not found.')
-        self.__triggered_canoe_quit = False
+            raise FileNotFoundError(f'CANoe cfg file "{canoe_cfg}" not found!')
 
     def new(self, auto_save=False, prompt_user=False) -> None:
         """Creates a new configuration.
 
         Args:
             auto_save (bool, optional): A boolean value that indicates whether the active configuration should be saved if it has been changed. Defaults to False.
             prompt_user (bool, optional): A boolean value that indicates whether the user should intervene in error situations. Defaults to False.
 
         Examples:
             >>> # The following example creates a new configuration
             >>> canoe_inst = CANoe()
             >>> canoe_inst.new()
         """
-        self.__dispatch_canoe()
         self.__canoe_objects['Application'].New(auto_save, prompt_user)
-        self.log.info('created a new configuration')
+        self.log.info('created a new configuration...')
 
-    def quit(self) -> None:
+    def quit(self):
         r"""Quits CANoe without saving changes in the configuration.
 
         Examples:
             >>> # The following example quits CANoe
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.quit()
         """
-        if self.__canoe_objects['Application'].Measurement.Running:
-            self.stop_measurement()
-        self.__canoe_objects['Application'].Configuration.Modified = False
+        if self.__canoe_objects['Measurement'].Running:
+            self.__canoe_objects['Measurement'].Stop()
+            self.wait_for_canoe_meas_to_stop()
         self.__canoe_objects['Application'].Quit()
-        self.__triggered_canoe_quit = True
-        self.log.info('CANoe Application Closed without saving configuration.')
+        self.log.info('CANoe Application Closed.')
 
     def start_measurement_in_animation_mode(self, animation_delay=100) -> None:
         r"""Starts the measurement in Animation mode.
 
         Args:
             animation_delay (int): The animation delay during the measurement in Offline Mode.
 
         Examples:
             >>> # The following example starts the measurement in Animation mode
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement_in_animation_mode()
         """
-        if not self.__canoe_objects['Application'].Measurement.Running:
-            self.__canoe_objects['Application'].Measurement.AnimationDelay = animation_delay
-            self.__canoe_objects['Application'].Measurement.Animate()
+        if not self.__canoe_objects['Measurement'].Running:
+            self.__canoe_objects['Measurement'].AnimationDelay = animation_delay
+            self.__canoe_objects['Measurement'].Animate()
+            self.wait_for_canoe_meas_to_start()
             self.log.info(f'Started the measurement in Animation mode with animation delay = {animation_delay}.')
 
     def break_measurement_in_offline_mode(self) -> None:
         r"""Interrupts the playback in Offline mode.
 
         Examples:
             >>> # The following example interrupts the playback in Offline mode
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.break_measurement_in_offline_mode()
         """
-        if self.__canoe_objects['Application'].Measurement.Running:
-            self.__canoe_objects['Application'].Measurement.Break()
+        if self.__canoe_objects['Measurement'].Running:
+            self.__canoe_objects['Measurement'].Break()
             self.log.info('Interrupted the playback in Offline mode.')
 
     def reset_measurement_in_offline_mode(self) -> None:
         r"""Resets the measurement in Offline mode.
 
         Examples:
             >>> # The following example resets the measurement in Offline mode
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.reset_measurement_in_offline_mode()
         """
-        self.__canoe_objects['Application'].Measurement.Reset()
+        self.__canoe_objects['Measurement'].Reset()
         self.log.info('resetted measurement in offline mode.')
 
     def start_measurement(self) -> bool:
         r"""Starts the measurement.
 
         Returns:
             True if measurement started. else Flase.
 
         Examples:
             >>> # The following example starts the measurement
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
         """
-        if not self.__canoe_objects['Application'].Measurement.Running:
-            self.__canoe_objects['Application'].Measurement.Start()
-            if not self.__canoe_objects['Application'].Measurement.Running:
+        if not self.__canoe_objects['Measurement'].Running:
+            self.__canoe_objects['Measurement'].Start()
+            if not self.__canoe_objects['Measurement'].Running:
                 self.log.info(f'waiting for measurement to start...')
-                self.wait_for_start()
-            self.log.info(f'CANoe Measurement Started. Measurement running status = {self.__canoe_objects["Application"].Measurement.Running}')
+                self.wait_for_canoe_meas_to_start()
+            self.log.info(f'CANoe Measurement Started. Measurement running status = {self.__canoe_objects["Measurement"].Running}')
         else:
-            self.log.info(f'CANoe Measurement Already Running. Measurement running status = {self.__canoe_objects["Application"].Measurement.Running}')
-        return self.__canoe_objects['Application'].Measurement.Running
+            self.log.info(f'CANoe Measurement Already Running. Measurement running status = {self.__canoe_objects["Measurement"].Running}')
+        return self.__canoe_objects['Measurement'].Running
 
     def step_measurement_event_in_single_step(self) -> None:
         r"""Processes a measurement event in single step.
 
         Examples:
             >>> # The following example processes a measurement event in single step
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.step_measurement_event_in_single_step()
         """
-        if not self.__canoe_objects['Application'].Measurement.Running:
-            self.__canoe_objects['Application'].Measurement.Step()
+        if not self.__canoe_objects['Measurement'].Running:
+            self.__canoe_objects['Measurement'].Step()
             self.log.info('processed a measurement event in single step')
 
     def stop_measurement(self) -> bool:
         r"""Stops the measurement.
 
         Returns:
             True if measurement stopped. else Flase.
@@ -273,54 +301,54 @@
         Examples:
             >>> # The following example stops the measurement
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
             >>> canoe_inst.stop_measurement()
         """
-        if self.__canoe_objects['Application'].Measurement.Running:
-            self.__canoe_objects['Application'].Measurement.Stop()
-            self.wait_for_stop()
-            self.log.info(f'CANoe Measurement Stopped. Measurement running status = {self.__canoe_objects["Application"].Measurement.Running}')
+        if self.__canoe_objects['Measurement'].Running:
+            self.__canoe_objects['Measurement'].Stop()
+            self.wait_for_canoe_meas_to_stop()
+            self.log.info(f'CANoe Measurement Stopped. Measurement running status = {self.__canoe_objects["Measurement"].Running}')
         else:
-            self.log.info(f'CANoe Measurement Already Stopped. Measurement running status = {self.__canoe_objects["Application"].Measurement.Running}')
-        return not self.__canoe_objects['Application'].Measurement.Running
+            self.log.info(f'CANoe Measurement Already Stopped. Measurement running status = {self.__canoe_objects["Measurement"].Running}')
+        return not self.__canoe_objects['Measurement'].Running
 
     def reset_measurement(self) -> bool:
         r"""reset the measurement.
 
         Returns:
             Measurement running status(True/False).
 
         Examples:
             >>> # The following example resets the measurement
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
             >>> canoe_inst.reset_measurement()
         """
-        if self.__canoe_objects['Application'].Measurement.Running:
+        if self.__canoe_objects['Measurement'].Running:
             self.stop_measurement()
         self.start_measurement()
-        self.log.info(f'Resetted measurement. Measurement running status = {self.__canoe_objects["Application"].Measurement.Running}')
-        return self.__canoe_objects['Application'].Measurement.Running
+        self.log.info(f'Resetted measurement. Measurement running status = {self.__canoe_objects["Measurement"].Running}')
+        return self.__canoe_objects['Measurement'].Running
 
     def stop_ex_measurement(self) -> None:
         r"""StopEx repairs differences in the behavior of the Stop method on deferred stops concerning simulated and real mode in CANoe.
 
         Examples:
             >>> # The following example full stops the measurement
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
             >>> canoe_inst.stop_ex_measurement()
         """
-        if self.__canoe_objects['Application'].Measurement.Running:
-            self.__canoe_objects['Application'].Measurement.StopEx()
-            self.log.info(f'Stopped measurement. Measurement running status = {self.__canoe_objects["Application"].Measurement.Running}')
+        if self.__canoe_objects['Measurement'].Running:
+            self.__canoe_objects['Measurement'].StopEx()
+            self.log.info(f'Stopped measurement. Measurement running status = {self.__canoe_objects["Measurement"].Running}')
 
     def get_measurement_index(self) -> int:
         r"""gets the measurement index for the next measurement.
 
         Returns:
             Measurement Index.
 
@@ -328,15 +356,15 @@
             >>> # The following example gets the measurement index measurement
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
             >>> canoe_inst.stop_measurement()
             >>> canoe_inst.get_measurement_index()
         """
-        measurement_index = self.__canoe_objects['Application'].Measurement.MeasurementIndex
+        measurement_index = self.__canoe_objects['Measurement'].MeasurementIndex
         self.log.info(f'measurement_index value = {measurement_index}')
         return measurement_index
 
     def set_measurement_index(self, index: int) -> int:
         r"""sets the measurement index for the next measurement.
 
         Args:
@@ -349,17 +377,17 @@
             >>> # The following example sets the measurement index for the next measurement to 15
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
             >>> canoe_inst.stop_measurement()
             >>> canoe_inst.set_measurement_index(15)
         """
-        self.__canoe_objects['Application'].Measurement.MeasurementIndex = index
+        self.__canoe_objects['Measurement'].MeasurementIndex = index
         self.log.info(f'CANoe measurement index set to {index}')
-        return self.__canoe_objects['Application'].Measurement.MeasurementIndex
+        return self.__canoe_objects['Measurement'].MeasurementIndex
 
     def get_measurement_running_status(self) -> bool:
         r"""Returns the running state of the measurement.
 
         Returns:
             True if The measurement is running.
             False if The measurement is not running.
@@ -367,35 +395,35 @@
         Examples:
             >>> # The following example returns measurement running status (True/False)
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
             >>> canoe_inst.get_measurement_running_status()
         """
-        self.log.info(f'CANoe Measurement Running Status = {self.__canoe_objects["Application"].Measurement.Running}')
-        return self.__canoe_objects['Application'].Measurement.Running
+        self.log.info(f'CANoe Measurement Running Status = {self.__canoe_objects["Measurement"].Running}')
+        return self.__canoe_objects['Measurement'].Running
 
     def save_configuration(self) -> bool:
         r"""Saves the configuration.
 
         Returns:
             True if configuration saved. else False.
 
         Examples:
             >>> # The following example saves the configuration if necessary
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.save_configuration()
         """
-        if not self.__canoe_objects['Application'].Configuration.Saved:
-            self.__canoe_objects['Application'].Configuration.Save()
+        if not self.__canoe_objects['Configuration'].Saved:
+            self.__canoe_objects['Configuration'].Save()
             self.log.info('CANoe Configuration saved.')
         else:
             self.log.info('CANoe Configuration already in saved state.')
-        return self.__canoe_objects['Application'].Configuration.Saved
+        return self.__canoe_objects['Configuration'].Saved
 
     def save_configuration_as(self, path: str, major: int, minor: int, create_dir=True) -> bool:
         r"""Saves the configuration as a different CANoe version.
 
         Args:
             path (str): The complete file name.
             major (int): The major version number of the target version.
@@ -410,17 +438,17 @@
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.save_configuration_as(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo_v12.cfg', 10, 0)"""
         config_path = '\\'.join(path.split('\\')[:-1])
         if not os.path.exists(config_path) and create_dir:
             os.makedirs(config_path, exist_ok=True)
         if os.path.exists(config_path):
-            self.__canoe_objects['Application'].Configuration.SaveAs(path, major, minor)
+            self.__canoe_objects['Configuration'].SaveAs(path, major, minor)
             self.log.info(f'CANoe Configuration saved as {path}.')
-            return self.__canoe_objects['Application'].Configuration.Saved
+            return self.__canoe_objects['Configuration'].Saved
         else:
             self.log.info(f'tried creating {path}. but {config_path} directory not found.')
             return False
 
     def get_signal_value(self, bus: str, channel: int, message: str, signal: str, raw_value=False) -> Union[float, int]:
         r"""get_signal_value Returns a Signal value.
 
@@ -591,29 +619,29 @@
         Examples:
             >>> # The following example switches to the desktop with the name "Configuration"
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
             >>> canoe_inst.ui_activate_desktop("Configuration")
         """
-        self.__canoe_objects['Application'].UI.ActivateDesktop(name)
+        self.__canoe_objects['UI'].ActivateDesktop(name)
         self.log.info(f'Activated / switched to "{name}" Desktop')
 
     def ui_open_baudrate_dialog(self) -> None:
         r"""opens the dialog for configuring the bus parameters. Make sure Measurement stopped when using this method.
 
         Examples:
             >>> # The following example opens the dialog for configuring the bus parameters
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.stop_measurement()
             >>> canoe_inst.ui_open_baudrate_dialog()
         """
         self.log.info('opened the dialog for configuring the bus parameters')
-        self.__canoe_objects['Application'].UI.OpenBaudrateDialog()
+        self.__canoe_objects['UI'].OpenBaudrateDialog()
 
     def write_text_in_write_window(self, text: str) -> None:
         r"""Outputs a line of text in the Write Window.
         Args:
             text (str): The text.
 
         Examples:
@@ -622,15 +650,15 @@
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
             >>> wait(1)
             >>> canoe_inst.write_text_in_write_window("hello from python!")
             >>> wait(1)
             >>> print(canoe_inst.read_text_from_write_window())
         """
-        self.__canoe_objects['Application'].UI.Write.Output(text)
+        self.__canoe_objects['UI'].Write.Output(text)
         self.log.info(f'written "{text}" to Write Window')
 
     def read_text_from_write_window(self) -> str:
         r"""read the text contents from Write Window.
 
         Returns:
             The text content.
@@ -641,30 +669,30 @@
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
             >>> wait(1)
             >>> canoe_inst.write_text_in_write_window("hello from python!")
             >>> wait(1)
             >>> print(canoe_inst.read_text_from_write_window())
         """
-        return self.__canoe_objects['Application'].UI.Write.Text
+        return self.__canoe_objects['UI'].Write.Text
 
     def clear_write_window_content(self) -> None:
         r"""Clears the contents of the Write Window.
 
         Examples:
             >>> # The following example clears content from Write Window.
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
             >>> wait(1)
             >>> canoe_inst.write_text_in_write_window("hello from python!")
             >>> wait(1)
             >>> canoe_inst.clear_write_window_content()
         """
-        self.__canoe_objects['Application'].UI.Write.Clear()
+        self.__canoe_objects['UI'].Write.Clear()
         self.log.info(f'Cleared Write Window Content.')
 
     def enable_write_window_output_file(self, output_file: str) -> None:
         r"""Enables logging of all outputs of the Write Window in the output file.
 
         Args:
             output_file (str): The complete path of the output file.
@@ -676,27 +704,27 @@
             >>> canoe_inst.enable_write_window_output_file(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\write_out.txt')
             >>> canoe_inst.start_measurement()
             >>> wait(1)
             >>> canoe_inst.write_text_in_write_window("hello from python!")
             >>> wait(1)
             >>> canoe_inst.stop_measurement()
         """
-        self.__canoe_objects['Application'].UI.Write.EnableOutputFile(output_file)
+        self.__canoe_objects['UI'].Write.EnableOutputFile(output_file)
         self.log.info(f'Enabled Write Window logging. file path --> {output_file}')
 
     def disable_write_window_output_file(self) -> None:
         r"""Disables logging of all outputs of the Write Window.
 
         Examples:
             >>> # The following example Disables logging of all outputs of the Write Window.
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.disable_write_window_output_file()
         """
-        self.__canoe_objects['Application'].UI.Write.DisableOutputFile()
+        self.__canoe_objects['UI'].Write.DisableOutputFile()
         self.log.info(f'Disabled Write Window logging.')
 
     def get_can_bus_statistics(self, channel: int) -> dict:
         r"""Returns CAN Bus Statistics.
 
         Args:
             channel (int): The channel of the statistic that is to be returned.
@@ -706,15 +734,16 @@
 
         Examples:
             >>> # The following example prints CAN channel 1 statistics
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> print(canoe_inst.get_can_bus_statistics(channel=1))
         """
-        bus_statistics_obj = self.__canoe_objects['Application'].Configuration.OnlineSetup.BusStatistics.BusStatistic(self.__BUS_TYPES['CAN'], channel)
+        bus_types = {'CAN': 1, 'J1939': 2, 'TTP': 4, 'LIN': 5, 'MOST': 6, 'Kline': 14}
+        bus_statistics_obj = self.__canoe_objects['Configuration'].OnlineSetup.BusStatistics.BusStatistic(bus_types['CAN'], channel)
         statistics_info = {
             # The bus load
             'bus_load': bus_statistics_obj.BusLoad,
             # The controller status
             'chip_state': bus_statistics_obj.ChipState,
             # The number of Error Frames per second
             'error': bus_statistics_obj.Error,
@@ -792,15 +821,15 @@
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
             >>> sys_var_val = canoe_inst.get_system_variable_value('sys_var_demo::speed')
             >>>print(sys_var_val)
         """
         namespace = '::'.join(sys_var_name.split('::')[:-1])
         variable_name = sys_var_name.split('::')[-1]
-        namespace_object = self.__canoe_objects['Application'].System.Namespaces(namespace)
+        namespace_object = self.__canoe_objects['Namespaces'](namespace)
         variable_value = namespace_object.Variables(variable_name).Value
         self.log.info(f'system variable({sys_var_name}) value = {variable_value}.')
         return variable_value
 
     def set_system_variable_value(self, sys_var_name: str, value: Union[int, float, str]) -> None:
         r"""set_system_variable_value sets a value to system variable.
 
@@ -813,15 +842,15 @@
             >>> canoe_inst = CANoe()
             >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
             >>> canoe_inst.start_measurement()
             >>> canoe_inst.set_system_variable_value('sys_var_demo::speed', 1)
         """
         namespace = '::'.join(sys_var_name.split('::')[:-1])
         variable_name = sys_var_name.split('::')[-1]
-        namespace_object = self.__canoe_objects['Application'].System.Namespaces(namespace)
+        namespace_object = self.__canoe_objects['Namespaces'](namespace)
         namespace_object.Variables(variable_name).Value = value
         self.log.info(f'system variable({sys_var_name}) value set to {value}.')
 
     def send_diag_request(self, diag_ecu_qualifier_name: str, request: str, request_in_bytes=True) -> str:
         r"""The send_diag_request method represents the query of a diagnostic tester (client) to an ECU (server) in CANoe.
 
         Args:
@@ -918,25 +947,7 @@
             if start_stop:
                 self.__replay_blocks_obj_dictionary[block_name].Start()
             else:
                 self.__replay_blocks_obj_dictionary[block_name].Stop()
             self.log.info(f'Replay block "{block_name}" {"Started" if start_stop else "Stopped"}.')
         else:
             self.log.warning(f'Replay block "{block_name}" not available.')
-
-class CanoeMeasurementEvents:
-    """Handler for CANoe measurement events"""
-
-    @staticmethod
-    def OnStart():
-        CANoe.Started = True
-        CANoe.Stopped = False
-
-    @staticmethod
-    def OnStop():
-        CANoe.Started = False
-        CANoe.Stopped = True
-
-
-def DoEventsUntil(cond):
-    while not cond():
-        DoEvents()
```

### Comparing `py_canoe-0.1.1/tests/demo_cfg/CANdb/easy.dbc` & `py_canoe-0.1.2/tests/demo_cfg/CANdb/easy.dbc`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.1/tests/demo_cfg/CDD/UDS-ExampleEcu-5.0.2.cdd` & `py_canoe-0.1.2/tests/demo_cfg/CDD/UDS-ExampleEcu-5.0.2.cdd`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.1/tests/demo_cfg/Logs/demo_log.blf` & `py_canoe-0.1.2/tests/demo_cfg/Logs/demo_log.blf`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.1/tests/demo_cfg/Nodes/SimDiagECU.can` & `py_canoe-0.1.2/tests/demo_cfg/Nodes/SimDiagECU.can`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.1/tests/demo_cfg/Nodes/system_events.can` & `py_canoe-0.1.2/tests/demo_cfg/Nodes/system_events.can`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.1/tests/demo_cfg/Panels/sys_var_demo_panel.xvp` & `py_canoe-0.1.2/tests/demo_cfg/Panels/sys_var_demo_panel.xvp`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.1/tests/demo_cfg/demo.cfg` & `py_canoe-0.1.2/tests/demo_cfg/demo.cfg`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.1/tests/demo_cfg/demo_offline.cfg` & `py_canoe-0.1.2/tests/demo_cfg/demo_offline.cfg`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.1/tests/test_canoe.py` & `py_canoe-0.1.2/tests/test_canoe.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 sys.path.extend([file_path, fr'{root_path}\src'])
 
 from py_canoe import CANoe
 canoe_inst = CANoe()
 
 def test_canoe_open_new_save_methods():
     canoe_inst.open(fr'{file_path}\demo_cfg\demo.cfg')
+    canoe_inst.quit()
+    wait(1)
+    canoe_inst.open(fr'{file_path}\demo_cfg\demo.cfg')
+    wait(1)
     canoe_inst.new(auto_save=True)
     assert canoe_inst.save_configuration_as(fr'{file_path}\demo_cfg\demo_v10.cfg', 10, 0)
     wait(2)
 
 def test_canoe_basic_measurement_methods():
     canoe_inst.open(fr'{file_path}\demo_cfg\demo.cfg')
     meas_index = canoe_inst.get_measurement_index()
@@ -81,17 +85,24 @@
     assert canoe_inst.stop_measurement()
     canoe_inst.disable_write_window_output_file()
     assert "hello from python!" in text
     wait(2)
 
 def test_canoe_animation_mode_methods():
     canoe_inst.open(fr'{file_path}\demo_cfg\demo_offline.cfg')
-    canoe_inst.step_measurement_event_in_single_step()
-    wait(2)
     canoe_inst.start_measurement_in_animation_mode()
-    wait(2)
+    wait(1)
     canoe_inst.break_measurement_in_offline_mode()
-    wait(2)
+    wait(1)
+    canoe_inst.step_measurement_event_in_single_step()
+    wait(1)
     canoe_inst.reset_measurement_in_offline_mode()
-    wait(2)
+    wait(1)
     assert canoe_inst.stop_measurement()
-    wait(2)
+    wait(1)
+    canoe_inst.open(fr'{file_path}\demo_cfg\demo.cfg')
+
+def test_quit_canoe():
+    canoe_inst.open(fr'{file_path}\demo_cfg\demo_offline.cfg')
+    wait(1)
+    canoe_inst.quit()
+    wait(5)
```

### Comparing `py_canoe-0.1.1/PKG-INFO` & `py_canoe-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_canoe
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python package for controlling Vector CANoe tool
 Author-email: chaitu-ycr <chaitu.ycr@gmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.9
```

