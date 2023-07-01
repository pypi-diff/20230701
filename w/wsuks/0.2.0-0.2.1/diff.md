# Comparing `tmp/wsuks-0.2.0.tar.gz` & `tmp/wsuks-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsuks-0.2.0.tar", max compression
+gzip compressed data, was "wsuks-0.2.1.tar", max compression
```

## Comparing `wsuks-0.2.0.tar` & `wsuks-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1301 2023-04-06 19:28:11.193610 wsuks-0.2.0/LICENSE
--rw-r--r--   0        0        0       12 2023-04-01 15:37:24.878272 wsuks-0.2.0/README.md
--rw-r--r--   0        0        0      507 2023-07-01 17:17:13.477618 wsuks-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-01 15:16:02.001468 wsuks-0.2.0/wsuks/__init__.py
--rw-r--r--   0        0        0   717232 2023-03-30 14:57:14.000000 wsuks-0.2.0/wsuks/executables/PsExec.exe
--rw-r--r--   0        0        0   831888 2023-03-30 14:57:14.000000 wsuks-0.2.0/wsuks/executables/PsExec64.exe
--rw-r--r--   0        0        0        0 2023-03-19 17:44:56.143981 wsuks-0.2.0/wsuks/helpers/__init__.py
--rw-r--r--   0        0        0     3056 2023-07-01 16:04:00.893527 wsuks-0.2.0/wsuks/helpers/argparser.py
--rw-r--r--   0        0        0     3080 2023-07-01 16:14:59.221541 wsuks-0.2.0/wsuks/helpers/arpspoofer.py
--rw-r--r--   0        0        0     1697 2023-04-02 21:07:58.692346 wsuks-0.2.0/wsuks/helpers/logger.py
--rw-r--r--   0        0        0     3354 2023-07-01 16:23:15.421551 wsuks-0.2.0/wsuks/helpers/sysvolparser.py
--rw-r--r--   0        0        0    10679 2023-07-01 16:14:34.285540 wsuks-0.2.0/wsuks/helpers/wsusserver.py
--rw-r--r--   0        0        0     2845 2023-07-01 16:22:47.865551 wsuks-0.2.0/wsuks/wsuks.py
--rw-r--r--   0        0        0      583 2023-04-06 19:28:41.085610 wsuks-0.2.0/wsuks/xml_files/get-authorization-cookie.xml
--rw-r--r--   0        0        0      838 2023-04-06 19:28:44.697610 wsuks-0.2.0/wsuks/xml_files/get-config.xml
--rw-r--r--   0        0        0      526 2023-04-06 19:28:47.697610 wsuks-0.2.0/wsuks/xml_files/get-cookie.xml
--rw-r--r--   0        0        0     4247 2023-04-06 19:28:51.417611 wsuks-0.2.0/wsuks/xml_files/get-extended-update-info.xml
--rw-r--r--   0        0        0      469 2023-04-06 19:28:58.353611 wsuks-0.2.0/wsuks/xml_files/internal-error.xml
--rw-r--r--   0        0        0      364 2023-04-06 19:29:04.397611 wsuks-0.2.0/wsuks/xml_files/register-computer.xml
--rw-r--r--   0        0        0      418 2023-04-06 19:29:08.141611 wsuks-0.2.0/wsuks/xml_files/report-event-batch.xml
--rw-r--r--   0        0        0     3295 2023-04-06 19:29:12.273611 wsuks-0.2.0/wsuks/xml_files/sync-updates.xml
--rw-r--r--   0        0        0      899 1970-01-01 00:00:00.000000 wsuks-0.2.0/setup.py
--rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 wsuks-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1301 2023-04-06 19:28:11.193610 wsuks-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1858 2023-07-01 17:32:37.749637 wsuks-0.2.1/README.md
+-rw-r--r--   0        0        0      507 2023-07-01 17:34:10.469639 wsuks-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-01 15:16:02.001468 wsuks-0.2.1/wsuks/__init__.py
+-rw-r--r--   0        0        0   717232 2023-03-30 14:57:14.000000 wsuks-0.2.1/wsuks/executables/PsExec.exe
+-rw-r--r--   0        0        0   831888 2023-03-30 14:57:14.000000 wsuks-0.2.1/wsuks/executables/PsExec64.exe
+-rw-r--r--   0        0        0        0 2023-03-19 17:44:56.143981 wsuks-0.2.1/wsuks/helpers/__init__.py
+-rw-r--r--   0        0        0     3056 2023-07-01 16:04:00.893527 wsuks-0.2.1/wsuks/helpers/argparser.py
+-rw-r--r--   0        0        0     3080 2023-07-01 16:14:59.221541 wsuks-0.2.1/wsuks/helpers/arpspoofer.py
+-rw-r--r--   0        0        0     1697 2023-04-02 21:07:58.692346 wsuks-0.2.1/wsuks/helpers/logger.py
+-rw-r--r--   0        0        0     3354 2023-07-01 16:23:15.421551 wsuks-0.2.1/wsuks/helpers/sysvolparser.py
+-rw-r--r--   0        0        0    10679 2023-07-01 16:14:34.285540 wsuks-0.2.1/wsuks/helpers/wsusserver.py
+-rw-r--r--   0        0        0     2945 2023-07-01 17:30:58.501635 wsuks-0.2.1/wsuks/wsuks.py
+-rw-r--r--   0        0        0      583 2023-04-06 19:28:41.085610 wsuks-0.2.1/wsuks/xml_files/get-authorization-cookie.xml
+-rw-r--r--   0        0        0      838 2023-04-06 19:28:44.697610 wsuks-0.2.1/wsuks/xml_files/get-config.xml
+-rw-r--r--   0        0        0      526 2023-04-06 19:28:47.697610 wsuks-0.2.1/wsuks/xml_files/get-cookie.xml
+-rw-r--r--   0        0        0     4247 2023-04-06 19:28:51.417611 wsuks-0.2.1/wsuks/xml_files/get-extended-update-info.xml
+-rw-r--r--   0        0        0      469 2023-04-06 19:28:58.353611 wsuks-0.2.1/wsuks/xml_files/internal-error.xml
+-rw-r--r--   0        0        0      364 2023-04-06 19:29:04.397611 wsuks-0.2.1/wsuks/xml_files/register-computer.xml
+-rw-r--r--   0        0        0      418 2023-04-06 19:29:08.141611 wsuks-0.2.1/wsuks/xml_files/report-event-batch.xml
+-rw-r--r--   0        0        0     3295 2023-04-06 19:29:12.273611 wsuks-0.2.1/wsuks/xml_files/sync-updates.xml
+-rw-r--r--   0        0        0     2792 1970-01-01 00:00:00.000000 wsuks-0.2.1/setup.py
+-rw-r--r--   0        0        0     2477 1970-01-01 00:00:00.000000 wsuks-0.2.1/PKG-INFO
```

### Comparing `wsuks-0.2.0/LICENSE` & `wsuks-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.0/wsuks/executables/PsExec.exe` & `wsuks-0.2.1/wsuks/executables/PsExec.exe`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.0/wsuks/executables/PsExec64.exe` & `wsuks-0.2.1/wsuks/executables/PsExec64.exe`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.0/wsuks/helpers/argparser.py` & `wsuks-0.2.1/wsuks/helpers/argparser.py`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.0/wsuks/helpers/arpspoofer.py` & `wsuks-0.2.1/wsuks/helpers/arpspoofer.py`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.0/wsuks/helpers/logger.py` & `wsuks-0.2.1/wsuks/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.0/wsuks/helpers/sysvolparser.py` & `wsuks-0.2.1/wsuks/helpers/sysvolparser.py`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.0/wsuks/helpers/wsusserver.py` & `wsuks-0.2.1/wsuks/helpers/wsusserver.py`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.0/wsuks/wsuks.py` & `wsuks-0.2.1/wsuks/wsuks.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,13 +75,17 @@
     logger = logging.getLogger('wsuks')
     logger.debug(args)
     
     # Prevent scapy from logging to console
     scapyLogger = logging.getLogger('scapy')
     scapyLogger.handlers.clear()
 
+    if os.geteuid() != 0:
+        logger.error("This script must be run as root!")
+        exit(1)
+
     wsuks = Wsuks(args)
     wsuks.run()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `wsuks-0.2.0/wsuks/xml_files/get-authorization-cookie.xml` & `wsuks-0.2.1/wsuks/xml_files/get-authorization-cookie.xml`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.0/wsuks/xml_files/get-config.xml` & `wsuks-0.2.1/wsuks/xml_files/get-config.xml`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.0/wsuks/xml_files/get-cookie.xml` & `wsuks-0.2.1/wsuks/xml_files/get-cookie.xml`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.0/wsuks/xml_files/get-extended-update-info.xml` & `wsuks-0.2.1/wsuks/xml_files/get-extended-update-info.xml`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.0/wsuks/xml_files/sync-updates.xml` & `wsuks-0.2.1/wsuks/xml_files/sync-updates.xml`

 * *Files identical despite different names*

