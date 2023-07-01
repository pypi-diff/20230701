# Comparing `tmp/SecureMessaging-3.8.8.tar.gz` & `tmp/SecureMessaging-3.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SecureMessaging-3.8.8.tar", last modified: Fri Jun 30 06:49:04 2023, max compression
+gzip compressed data, was "SecureMessaging-3.8.9.tar", last modified: Sat Jul  1 02:42:01 2023, max compression
```

## Comparing `SecureMessaging-3.8.8.tar` & `SecureMessaging-3.8.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-30 06:49:04.498813 SecureMessaging-3.8.8/
--rw-r--r--   0 user      (1000) user      (1000)     2861 2023-06-30 06:49:04.498813 SecureMessaging-3.8.8/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     2310 2023-06-30 06:11:32.000000 SecureMessaging-3.8.8/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-30 06:49:04.498813 SecureMessaging-3.8.8/SecureMessaging.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     2861 2023-06-30 06:49:04.000000 SecureMessaging-3.8.8/SecureMessaging.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      260 2023-06-30 06:49:04.000000 SecureMessaging-3.8.8/SecureMessaging.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-06-30 06:49:04.000000 SecureMessaging-3.8.8/SecureMessaging.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       28 2023-06-30 06:49:04.000000 SecureMessaging-3.8.8/SecureMessaging.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-06-30 06:49:04.000000 SecureMessaging-3.8.8/SecureMessaging.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)    12557 2023-06-30 06:31:56.000000 SecureMessaging-3.8.8/SecureMessaging.py
--rw-r--r--   0 user      (1000) user      (1000)     1479 2023-06-30 06:11:32.000000 SecureMessaging-3.8.8/license.txt
--rw-r--r--   0 user      (1000) user      (1000)       28 2023-06-30 06:11:32.000000 SecureMessaging-3.8.8/requirements.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-06-30 06:49:04.498813 SecureMessaging-3.8.8/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     1002 2023-06-30 06:48:20.000000 SecureMessaging-3.8.8/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-07-01 02:42:01.785062 SecureMessaging-3.8.9/
+-rw-r--r--   0 user      (1000) user      (1000)     3013 2023-07-01 02:42:01.785062 SecureMessaging-3.8.9/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     2310 2023-06-30 06:11:32.000000 SecureMessaging-3.8.9/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-07-01 02:42:01.785062 SecureMessaging-3.8.9/SecureMessaging.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     3013 2023-07-01 02:42:01.000000 SecureMessaging-3.8.9/SecureMessaging.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      260 2023-07-01 02:42:01.000000 SecureMessaging-3.8.9/SecureMessaging.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-07-01 02:42:01.000000 SecureMessaging-3.8.9/SecureMessaging.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       28 2023-07-01 02:42:01.000000 SecureMessaging-3.8.9/SecureMessaging.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-07-01 02:42:01.000000 SecureMessaging-3.8.9/SecureMessaging.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)    12557 2023-06-30 06:31:56.000000 SecureMessaging-3.8.9/SecureMessaging.py
+-rw-r--r--   0 user      (1000) user      (1000)     1479 2023-06-30 06:11:32.000000 SecureMessaging-3.8.9/license.txt
+-rw-r--r--   0 user      (1000) user      (1000)       28 2023-06-30 06:11:32.000000 SecureMessaging-3.8.9/requirements.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-07-01 02:42:01.785062 SecureMessaging-3.8.9/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)     1159 2023-07-01 02:41:42.000000 SecureMessaging-3.8.9/setup.py
```

### Comparing `SecureMessaging-3.8.8/PKG-INFO` & `SecureMessaging-3.8.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: SecureMessaging
-Version: 3.8.8
+Version: 3.8.9
 Summary: Secure Messaging
 Home-page: https://github.com/ethicalhacker7192/SecureMessaging
 Author: Guinea_Pig_Lord
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # OTP-MAC-online
 a One Time Pad encryption program called GuineaSend that also encrypts the key in MAC SHA-256 bit hash.
 
 
 ## to install and run on linux(python3 required):
```

### Comparing `SecureMessaging-3.8.8/README.md` & `SecureMessaging-3.8.9/README.md`

 * *Files identical despite different names*

### Comparing `SecureMessaging-3.8.8/SecureMessaging.egg-info/PKG-INFO` & `SecureMessaging-3.8.9/SecureMessaging.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: SecureMessaging
-Version: 3.8.8
+Version: 3.8.9
 Summary: Secure Messaging
 Home-page: https://github.com/ethicalhacker7192/SecureMessaging
 Author: Guinea_Pig_Lord
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # OTP-MAC-online
 a One Time Pad encryption program called GuineaSend that also encrypts the key in MAC SHA-256 bit hash.
 
 
 ## to install and run on linux(python3 required):
```

### Comparing `SecureMessaging-3.8.8/SecureMessaging.py` & `SecureMessaging-3.8.9/SecureMessaging.py`

 * *Files identical despite different names*

### Comparing `SecureMessaging-3.8.8/license.txt` & `SecureMessaging-3.8.9/license.txt`

 * *Files identical despite different names*

