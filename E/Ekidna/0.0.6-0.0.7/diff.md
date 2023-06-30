# Comparing `tmp/Ekidna-0.0.6.tar.gz` & `tmp/Ekidna-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Ekidna-0.0.6.tar", last modified: Thu Jun 29 21:13:23 2023, max compression
+gzip compressed data, was "Ekidna-0.0.7.tar", last modified: Fri Jun 30 22:55:03 2023, max compression
```

## Comparing `Ekidna-0.0.6.tar` & `Ekidna-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 21:13:23.861999 Ekidna-0.0.6/
--rw-rw-rw-   0        0        0      630 2023-06-29 19:54:15.000000 Ekidna-0.0.6/CHANGELOG.txt
-drwxrwxrwx   0        0        0        0 2023-06-29 21:13:23.823647 Ekidna-0.0.6/Ekidna/
--rw-rw-rw-   0        0        0    33166 2023-06-29 21:11:59.000000 Ekidna-0.0.6/Ekidna/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 21:13:23.859009 Ekidna-0.0.6/Ekidna.egg-info/
--rw-rw-rw-   0        0        0     1523 2023-06-29 21:13:23.000000 Ekidna-0.0.6/Ekidna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-06-29 21:13:23.000000 Ekidna-0.0.6/Ekidna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 21:13:23.000000 Ekidna-0.0.6/Ekidna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-29 21:13:23.000000 Ekidna-0.0.6/Ekidna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1059 2023-06-29 21:10:14.000000 Ekidna-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-06-29 18:41:11.000000 Ekidna-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0    13206 2023-06-29 21:10:17.000000 Ekidna-0.0.6/Module Contents.txt
--rw-rw-rw-   0        0        0     1523 2023-06-29 21:13:23.861020 Ekidna-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      378 2023-06-29 21:10:51.000000 Ekidna-0.0.6/README.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 21:13:23.862998 Ekidna-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      734 2023-06-29 21:11:55.000000 Ekidna-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 22:55:03.743853 Ekidna-0.0.7/
+-rw-rw-rw-   0        0        0      639 2023-06-30 21:48:21.000000 Ekidna-0.0.7/CHANGELOG.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 22:55:03.686032 Ekidna-0.0.7/Ekidna/
+-rw-rw-rw-   0        0        0    86635 2023-06-30 22:54:12.000000 Ekidna-0.0.7/Ekidna/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 22:55:03.740769 Ekidna-0.0.7/Ekidna.egg-info/
+-rw-rw-rw-   0        0        0     1532 2023-06-30 22:55:03.000000 Ekidna-0.0.7/Ekidna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-06-30 22:55:03.000000 Ekidna-0.0.7/Ekidna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 22:55:03.000000 Ekidna-0.0.7/Ekidna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-30 22:55:03.000000 Ekidna-0.0.7/Ekidna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1059 2023-06-29 21:10:14.000000 Ekidna-0.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-06-29 18:41:11.000000 Ekidna-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0    36509 2023-06-30 21:51:21.000000 Ekidna-0.0.7/Module Contents.txt
+-rw-rw-rw-   0        0        0     1532 2023-06-30 22:55:03.743166 Ekidna-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-06-29 21:10:51.000000 Ekidna-0.0.7/README.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 22:55:03.744355 Ekidna-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      734 2023-06-30 21:48:32.000000 Ekidna-0.0.7/setup.py
```

### Comparing `Ekidna-0.0.6/Ekidna.egg-info/PKG-INFO` & `Ekidna-0.0.7/Ekidna.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Ekidna
-Version: 0.0.6
+Version: 0.0.7
 Summary: Electrochemistry data analysis tools
 Home-page: 
 Author: OzymandiasTheDead
 Author-email: jacob@ekidnasensing.com
 License: MIT
 Keywords: Ekidna
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -21,21 +21,20 @@
 
 The code is developed by researchers at Ekidna Sensing.
 
 
 
 Change Log
 ===========
-0.0.6 (June 29, 2023)
+0.0.7 (June 30, 2023)
 -------------------------
-- Sixth Release
+- Seventh Release
 
 Notes:
 ------
-Added a class called linear_std_curve
+Added standard curve classes: parabolic_QR, linear_QR, power_std_curve, parabolic_std_curve
 
-The class can be used to fit a linear model to data. The class goes beyond standard coefficient determination, as it also
-determines estimation limits for inverse regression. Information such as smoothing, baseline subtraction, calibration procedures 
-employed to process the data prior to fitting can also be stored.
+The classes can be used to fit models to data. The classes also contain attriburtes such as estimation limits for inverse regression.
+Information such as smoothing, baseline subtraction, calibration procedures employed to process the data prior to fitting can also be stored.
 
-The prediction band edges of the standard curve are also callable as methods within the object. See documentation for full list of methods
+The prediction band edges of the standard curve are callable as methods within the objects. See documentation for full list of methods
 and attributes.
```

### Comparing `Ekidna-0.0.6/LICENSE.txt` & `Ekidna-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Ekidna-0.0.6/PKG-INFO` & `Ekidna-0.0.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Ekidna
-Version: 0.0.6
+Version: 0.0.7
 Summary: Electrochemistry data analysis tools
 Home-page: 
 Author: OzymandiasTheDead
 Author-email: jacob@ekidnasensing.com
 License: MIT
 Keywords: Ekidna
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -21,21 +21,20 @@
 
 The code is developed by researchers at Ekidna Sensing.
 
 
 
 Change Log
 ===========
-0.0.6 (June 29, 2023)
+0.0.7 (June 30, 2023)
 -------------------------
-- Sixth Release
+- Seventh Release
 
 Notes:
 ------
-Added a class called linear_std_curve
+Added standard curve classes: parabolic_QR, linear_QR, power_std_curve, parabolic_std_curve
 
-The class can be used to fit a linear model to data. The class goes beyond standard coefficient determination, as it also
-determines estimation limits for inverse regression. Information such as smoothing, baseline subtraction, calibration procedures 
-employed to process the data prior to fitting can also be stored.
+The classes can be used to fit models to data. The classes also contain attriburtes such as estimation limits for inverse regression.
+Information such as smoothing, baseline subtraction, calibration procedures employed to process the data prior to fitting can also be stored.
 
-The prediction band edges of the standard curve are also callable as methods within the object. See documentation for full list of methods
+The prediction band edges of the standard curve are callable as methods within the objects. See documentation for full list of methods
 and attributes.
```

### Comparing `Ekidna-0.0.6/setup.py` & `Ekidna-0.0.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='Ekidna',
-    version='0.0.6',
+    version='0.0.7',
     description='Electrochemistry data analysis tools',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='OzymandiasTheDead',
     author_email='jacob@ekidnasensing.com',
     license='MIT',
     classifiers=classifiers,
```

