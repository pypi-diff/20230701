# Comparing `tmp/DetaMetrics-0.0.4.tar.gz` & `tmp/DetaMetrics-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DetaMetrics-0.0.4.tar", last modified: Sat Jul  1 10:01:38 2023, max compression
+gzip compressed data, was "DetaMetrics-0.0.5.tar", last modified: Sat Jul  1 10:12:52 2023, max compression
```

## Comparing `DetaMetrics-0.0.4.tar` & `DetaMetrics-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 10:01:38.415649 DetaMetrics-0.0.4/
-drwxrwxrwx   0        0        0        0 2023-07-01 10:01:38.407149 DetaMetrics-0.0.4/DetaMetrics.egg-info/
--rw-rw-rw-   0        0        0     1301 2023-07-01 10:01:38.000000 DetaMetrics-0.0.4/DetaMetrics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-07-01 10:01:38.000000 DetaMetrics-0.0.4/DetaMetrics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 10:01:38.000000 DetaMetrics-0.0.4/DetaMetrics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-01 10:01:38.000000 DetaMetrics-0.0.4/DetaMetrics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-01 10:01:38.000000 DetaMetrics-0.0.4/DetaMetrics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1075 2023-06-30 12:12:35.000000 DetaMetrics-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1301 2023-07-01 10:01:38.414647 DetaMetrics-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      923 2023-06-30 14:06:48.000000 DetaMetrics-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 10:01:38.412640 DetaMetrics-0.0.4/detametrics/
--rw-rw-rw-   0        0        0       28 2023-06-30 12:00:58.000000 DetaMetrics-0.0.4/detametrics/__init__.py
--rw-rw-rw-   0        0        0      781 2023-07-01 09:58:35.000000 DetaMetrics-0.0.4/detametrics/sdk.py
--rw-rw-rw-   0        0        0      502 2023-06-30 12:00:54.000000 DetaMetrics-0.0.4/detametrics/tf.py
--rw-rw-rw-   0        0        0      497 2023-07-01 09:57:08.000000 DetaMetrics-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-01 10:01:38.415649 DetaMetrics-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-01 10:12:52.219591 DetaMetrics-0.0.5/
+drwxrwxrwx   0        0        0        0 2023-07-01 10:12:52.209479 DetaMetrics-0.0.5/DetaMetrics.egg-info/
+-rw-rw-rw-   0        0        0     1301 2023-07-01 10:12:52.000000 DetaMetrics-0.0.5/DetaMetrics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-07-01 10:12:52.000000 DetaMetrics-0.0.5/DetaMetrics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 10:12:52.000000 DetaMetrics-0.0.5/DetaMetrics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-01 10:12:52.000000 DetaMetrics-0.0.5/DetaMetrics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-01 10:12:52.000000 DetaMetrics-0.0.5/DetaMetrics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1075 2023-06-30 12:12:35.000000 DetaMetrics-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1301 2023-07-01 10:12:52.218579 DetaMetrics-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      923 2023-06-30 14:06:48.000000 DetaMetrics-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 10:12:52.216478 DetaMetrics-0.0.5/detametrics/
+-rw-rw-rw-   0        0        0       28 2023-06-30 12:00:58.000000 DetaMetrics-0.0.5/detametrics/__init__.py
+-rw-rw-rw-   0        0        0      781 2023-07-01 09:58:35.000000 DetaMetrics-0.0.5/detametrics/sdk.py
+-rw-rw-rw-   0        0        0      523 2023-07-01 10:12:27.000000 DetaMetrics-0.0.5/detametrics/tf.py
+-rw-rw-rw-   0        0        0      497 2023-07-01 10:12:36.000000 DetaMetrics-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-01 10:12:52.219591 DetaMetrics-0.0.5/setup.cfg
```

### Comparing `DetaMetrics-0.0.4/DetaMetrics.egg-info/PKG-INFO` & `DetaMetrics-0.0.5/DetaMetrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DetaMetrics
-Version: 0.0.4
+Version: 0.0.5
 Summary: SDK for DetaMetrics TensorBoard alternative.
 Author: SamTheProgrammer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `DetaMetrics-0.0.4/LICENSE` & `DetaMetrics-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `DetaMetrics-0.0.4/PKG-INFO` & `DetaMetrics-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DetaMetrics
-Version: 0.0.4
+Version: 0.0.5
 Summary: SDK for DetaMetrics TensorBoard alternative.
 Author: SamTheProgrammer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `DetaMetrics-0.0.4/README.md` & `DetaMetrics-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `DetaMetrics-0.0.4/detametrics/sdk.py` & `DetaMetrics-0.0.5/detametrics/sdk.py`

 * *Files identical despite different names*

