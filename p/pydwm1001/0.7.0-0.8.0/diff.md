# Comparing `tmp/pydwm1001-0.7.0.tar.gz` & `tmp/pydwm1001-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydwm1001-0.7.0.tar", last modified: Fri Jun 30 00:13:35 2023, max compression
+gzip compressed data, was "pydwm1001-0.8.0.tar", last modified: Sat Jul  1 01:26:25 2023, max compression
```

## Comparing `pydwm1001-0.7.0.tar` & `pydwm1001-0.8.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-30 00:13:35.812601 pydwm1001-0.7.0/
--rw-r--r--   0 adam       (501) staff       (20)     1111 2023-06-21 00:05:54.000000 pydwm1001-0.7.0/LICENSE
--rw-r--r--   0 adam       (501) staff       (20)      637 2023-06-30 00:13:35.812494 pydwm1001-0.7.0/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)      103 2023-06-21 00:05:43.000000 pydwm1001-0.7.0/README.md
--rw-r--r--   0 adam       (501) staff       (20)     4488 2023-06-30 00:12:46.000000 pydwm1001-0.7.0/dwm1001.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-30 00:13:35.812237 pydwm1001-0.7.0/pydwm1001.egg-info/
--rw-r--r--   0 adam       (501) staff       (20)      637 2023-06-30 00:13:35.000000 pydwm1001-0.7.0/pydwm1001.egg-info/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)      229 2023-06-30 00:13:35.000000 pydwm1001-0.7.0/pydwm1001.egg-info/SOURCES.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2023-06-30 00:13:35.000000 pydwm1001-0.7.0/pydwm1001.egg-info/dependency_links.txt
--rw-r--r--   0 adam       (501) staff       (20)        9 2023-06-30 00:13:35.000000 pydwm1001-0.7.0/pydwm1001.egg-info/requires.txt
--rw-r--r--   0 adam       (501) staff       (20)        8 2023-06-30 00:13:35.000000 pydwm1001-0.7.0/pydwm1001.egg-info/top_level.txt
--rw-r--r--   0 adam       (501) staff       (20)      640 2023-06-30 00:12:46.000000 pydwm1001-0.7.0/pyproject.toml
--rw-r--r--   0 adam       (501) staff       (20)       38 2023-06-30 00:13:35.812638 pydwm1001-0.7.0/setup.cfg
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-30 00:13:35.812335 pydwm1001-0.7.0/tests/
--rw-r--r--   0 adam       (501) staff       (20)     2788 2023-06-30 00:12:46.000000 pydwm1001-0.7.0/tests/test_dwm1001.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-01 01:26:25.701798 pydwm1001-0.8.0/
+-rw-r--r--   0 adam       (501) staff       (20)     1111 2023-06-21 00:05:54.000000 pydwm1001-0.8.0/LICENSE
+-rw-r--r--   0 adam       (501) staff       (20)      637 2023-07-01 01:26:25.701659 pydwm1001-0.8.0/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)      103 2023-06-21 00:05:43.000000 pydwm1001-0.8.0/README.md
+-rw-r--r--   0 adam       (501) staff       (20)     4672 2023-07-01 01:24:35.000000 pydwm1001-0.8.0/dwm1001.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-01 01:26:25.701221 pydwm1001-0.8.0/pydwm1001.egg-info/
+-rw-r--r--   0 adam       (501) staff       (20)      637 2023-07-01 01:26:25.000000 pydwm1001-0.8.0/pydwm1001.egg-info/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)      229 2023-07-01 01:26:25.000000 pydwm1001-0.8.0/pydwm1001.egg-info/SOURCES.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2023-07-01 01:26:25.000000 pydwm1001-0.8.0/pydwm1001.egg-info/dependency_links.txt
+-rw-r--r--   0 adam       (501) staff       (20)        9 2023-07-01 01:26:25.000000 pydwm1001-0.8.0/pydwm1001.egg-info/requires.txt
+-rw-r--r--   0 adam       (501) staff       (20)        8 2023-07-01 01:26:25.000000 pydwm1001-0.8.0/pydwm1001.egg-info/top_level.txt
+-rw-r--r--   0 adam       (501) staff       (20)      640 2023-07-01 01:24:35.000000 pydwm1001-0.8.0/pyproject.toml
+-rw-r--r--   0 adam       (501) staff       (20)       38 2023-07-01 01:26:25.701840 pydwm1001-0.8.0/setup.cfg
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-01 01:26:25.701316 pydwm1001-0.8.0/tests/
+-rw-r--r--   0 adam       (501) staff       (20)     2788 2023-06-30 00:12:46.000000 pydwm1001-0.8.0/tests/test_dwm1001.py
```

### Comparing `pydwm1001-0.7.0/LICENSE` & `pydwm1001-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydwm1001-0.7.0/PKG-INFO` & `pydwm1001-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydwm1001
-Version: 0.7.0
+Version: 0.8.0
 Summary: A Python library for interfacing with DWM1001
 Author-email: Adam Morrissett <morrissettal2@vcu.edu>
 Project-URL: Homepage, https://github.com/the-hive-lab/pydwm1001
 Project-URL: Bug Tracker, https://github.com/the-hive-lab/pydwm1001/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pydwm1001-0.7.0/dwm1001.py` & `pydwm1001-0.8.0/dwm1001.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 from serial import Serial
 
 
 class TagId(str):
     pass
 
 
+class TagName(str):
+    pass
+
+
 @dataclass
 class TagPosition:
     x_m: float
     y_m: float
     z_m: float
     quality: int
 
@@ -52,28 +56,32 @@
     SHELL_STARTUP_DELAY_PERIOD = 1.0
     SHELL_COMMAND_DELAY_PERIOD = 0.5
 
     def __init__(self, serial_handle: Serial) -> None:
         self.serial_handle = serial_handle
 
     @property
-    def tag_id(self) -> str:
+    def tag_name(self) -> TagName:
+        # We only use the last four characters in the address
+        return TagName("DW" + self.tag_id[-4:])
+
+    @property
+    def tag_id(self) -> TagId:
         self.send_shell_command(ShellCommand.SI)
 
-        report = []
+        response = []
         for _ in range(9):
-            report.append(self.serial_handle.readline().decode())
+            response.append(self.serial_handle.readline().decode())
 
-        # System info has a lot of lines, but we only care about the address
-        address_line = report[2]
+        # System info response has several lines, but we only care about the address
+        address_line = response[2]
         address_text_start = address_line.find("addr=")
-        address_string = address_line[address_text_start:-1].strip()
+        address_string = address_line[address_text_start:].strip()
 
-        # We only use the last four characters in the address
-        return address_string[-4:]
+        return TagId("0" + address_string.removeprefix("addr="))
 
     def send_shell_command(self, command: ShellCommand) -> None:
         self.serial_handle.write(command.value)
         self.serial_handle.write(ShellCommand.ENTER.value)
         self.serial_handle.flush()
 
         time.sleep(self.SHELL_COMMAND_DELAY_PERIOD)
@@ -113,27 +121,27 @@
     def __init__(self, serial_handle: Serial) -> None:
         super().__init__(serial_handle)
 
         # Device may not have shutdown properly previously
         self.reset()
         self.enter_shell_mode()
 
-    def wait_for_position_report(self) -> Tuple[TagId, TagPosition]:
+    def wait_for_position_report(self) -> Tuple[TagName, TagPosition]:
         report = self.serial_handle.readline().decode().split(",")
 
         if len(report) != 8:
             raise ParsingError("Position report has unexpected length.")
 
         if report[0] != "POS":
             raise ParsingError("Position report has incorrect tag.")
 
         position_data = [float(substr) for substr in report[3:6]]
         position_data.append(int(report[6]))
 
-        return TagId(report[2]), TagPosition(*position_data)
+        return TagName("DW" + report[2]), TagPosition(*position_data)
 
 
 class ActiveTag(UartDwm1001):
     def __init__(self, serial_handle) -> None:
         self.serial_handle = serial_handle
 
         # Device may not have shutdown properly previously
```

### Comparing `pydwm1001-0.7.0/pydwm1001.egg-info/PKG-INFO` & `pydwm1001-0.8.0/pydwm1001.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydwm1001
-Version: 0.7.0
+Version: 0.8.0
 Summary: A Python library for interfacing with DWM1001
 Author-email: Adam Morrissett <morrissettal2@vcu.edu>
 Project-URL: Homepage, https://github.com/the-hive-lab/pydwm1001
 Project-URL: Bug Tracker, https://github.com/the-hive-lab/pydwm1001/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pydwm1001-0.7.0/pyproject.toml` & `pydwm1001-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pydwm1001"
-version = "0.7.0"
+version = "0.8.0"
 authors = [
   { name="Adam Morrissett", email="morrissettal2@vcu.edu" },
 ]
 description = "A Python library for interfacing with DWM1001"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pydwm1001-0.7.0/tests/test_dwm1001.py` & `pydwm1001-0.8.0/tests/test_dwm1001.py`

 * *Files identical despite different names*

