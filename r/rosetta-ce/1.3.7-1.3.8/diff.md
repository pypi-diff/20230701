# Comparing `tmp/rosetta-ce-1.3.7.tar.gz` & `tmp/rosetta-ce-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosetta-ce-1.3.7.tar", last modified: Fri Jun 30 12:44:34 2023, max compression
+gzip compressed data, was "rosetta-ce-1.3.8.tar", last modified: Sat Jul  1 06:29:57 2023, max compression
```

## Comparing `rosetta-ce-1.3.7.tar` & `rosetta-ce-1.3.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 12:44:34.274760 rosetta-ce-1.3.7/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.3.7/LICENSE
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-06-30 12:44:34.274489 rosetta-ce-1.3.7/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.3.7/README.md
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 12:44:34.266565 rosetta-ce-1.3.7/rosetta/
--rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.3.7/rosetta/__init__.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 12:44:34.269954 rosetta-ce-1.3.7/rosetta/constants/
--rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.3.7/rosetta/constants/__init__.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.3.7/rosetta/constants/sensors.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.3.7/rosetta/constants/sources.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.3.7/rosetta/constants/systems.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.3.7/rosetta/rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)    43792 2023-06-30 12:42:30.000000 rosetta-ce-1.3.7/rosetta/rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     8572 2023-06-29 15:55:20.000000 rosetta-ce-1.3.7/rosetta/rsender.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 12:44:34.272625 rosetta-ce-1.3.7/rosetta_ce.egg-info/
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-06-30 12:44:34.000000 rosetta-ce-1.3.7/rosetta_ce.egg-info/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-06-30 12:44:34.000000 rosetta-ce-1.3.7/rosetta_ce.egg-info/SOURCES.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-06-30 12:44:34.000000 rosetta-ce-1.3.7/rosetta_ce.egg-info/dependency_links.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-06-30 12:44:34.000000 rosetta-ce-1.3.7/rosetta_ce.egg-info/requires.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-06-30 12:44:34.000000 rosetta-ce-1.3.7/rosetta_ce.egg-info/top_level.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-06-30 12:44:34.274799 rosetta-ce-1.3.7/setup.cfg
--rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-06-30 12:43:23.000000 rosetta-ce-1.3.7/setup.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 12:44:34.273919 rosetta-ce-1.3.7/tests/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.3.7/tests/test_rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.3.7/tests/test_rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.3.7/tests/test_rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-01 06:29:57.602789 rosetta-ce-1.3.8/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.3.8/LICENSE
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-01 06:29:57.602452 rosetta-ce-1.3.8/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.3.8/README.md
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-01 06:29:57.596905 rosetta-ce-1.3.8/rosetta/
+-rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.3.8/rosetta/__init__.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-01 06:29:57.598717 rosetta-ce-1.3.8/rosetta/constants/
+-rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.3.8/rosetta/constants/__init__.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.3.8/rosetta/constants/sensors.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.3.8/rosetta/constants/sources.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.3.8/rosetta/constants/systems.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.3.8/rosetta/rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)    43790 2023-07-01 06:28:28.000000 rosetta-ce-1.3.8/rosetta/rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     8572 2023-06-29 15:55:20.000000 rosetta-ce-1.3.8/rosetta/rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-01 06:29:57.600552 rosetta-ce-1.3.8/rosetta_ce.egg-info/
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-01 06:29:57.000000 rosetta-ce-1.3.8/rosetta_ce.egg-info/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-07-01 06:29:57.000000 rosetta-ce-1.3.8/rosetta_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-07-01 06:29:57.000000 rosetta-ce-1.3.8/rosetta_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-07-01 06:29:57.000000 rosetta-ce-1.3.8/rosetta_ce.egg-info/requires.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-07-01 06:29:57.000000 rosetta-ce-1.3.8/rosetta_ce.egg-info/top_level.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-07-01 06:29:57.602830 rosetta-ce-1.3.8/setup.cfg
+-rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-07-01 06:28:46.000000 rosetta-ce-1.3.8/setup.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-01 06:29:57.601922 rosetta-ce-1.3.8/tests/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.3.8/tests/test_rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.3.8/tests/test_rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.3.8/tests/test_rsender.py
```

### Comparing `rosetta-ce-1.3.7/LICENSE` & `rosetta-ce-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.7/PKG-INFO` & `rosetta-ce-1.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.3.7
+Version: 1.3.8
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.3.7/README.md` & `rosetta-ce-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.7/rosetta/constants/sensors.py` & `rosetta-ce-1.3.8/rosetta/constants/sensors.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.7/rosetta/constants/sources.py` & `rosetta-ce-1.3.8/rosetta/constants/sources.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.7/rosetta/constants/systems.py` & `rosetta-ce-1.3.8/rosetta/constants/systems.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.7/rosetta/rconverter.py` & `rosetta-ce-1.3.8/rosetta/rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.7/rosetta/rfaker.py` & `rosetta-ce-1.3.8/rosetta/rfaker.py`

 * *Files 0% similar despite different names*

```diff
@@ -687,15 +687,15 @@
                     'severity': severity,
                     'host': host,
                     'user': user
                 }
                 if observables:
                     for observable, observable_value in vars(observables).items():
                         if observable_value:
-                            event['observable'] = random.choice(observable_value)
+                            event[observable] = random.choice(observable_value)
                 json_messages.append(event)
         return json_messages
 
     @classmethod
     def incidents(cls, count, fields: Optional[str] = None, timestamp: Optional[datetime] = None,
                   vendor: Optional[str] = None, product: Optional[str] = None, version: Optional[str] = None,
                   observables: Optional[Observables] = None) -> List[dict]:
```

### Comparing `rosetta-ce-1.3.7/rosetta/rsender.py` & `rosetta-ce-1.3.8/rosetta/rsender.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.7/rosetta_ce.egg-info/PKG-INFO` & `rosetta-ce-1.3.8/rosetta_ce.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.3.7
+Version: 1.3.8
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.3.7/setup.py` & `rosetta-ce-1.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rosetta-ce",
-    version="1.3.7",
+    version="1.3.8",
     author="Ayman Mahmoud",
     author_email="content@ayman.online",
     description="Rosetta is a Python package that can be used to fake security logs and alerts for testing different "
                 "detection and response use cases.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ayman-m/rosetta",
```

### Comparing `rosetta-ce-1.3.7/tests/test_rconverter.py` & `rosetta-ce-1.3.8/tests/test_rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.7/tests/test_rfaker.py` & `rosetta-ce-1.3.8/tests/test_rfaker.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.7/tests/test_rsender.py` & `rosetta-ce-1.3.8/tests/test_rsender.py`

 * *Files identical despite different names*

