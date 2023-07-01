# Comparing `tmp/BeeDrive-0.3.7.1.tar.gz` & `tmp/BeeDrive-0.4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BeeDrive-0.3.7.1.tar", last modified: Fri Jun 30 01:03:18 2023, max compression
+gzip compressed data, was "dist\BeeDrive-0.4.0.0.tar", last modified: Sat Jul  1 04:53:33 2023, max compression
```

## Comparing `BeeDrive-0.3.7.1.tar` & `BeeDrive-0.4.0.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 01:03:18.346788 BeeDrive-0.3.7.1/
--rw-rw-rw-   0        0        0     9719 2023-06-30 01:03:18.346788 BeeDrive-0.3.7.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-30 01:03:18.346788 BeeDrive-0.3.7.1/setup.cfg
--rw-rw-rw-   0        0        0     1439 2022-02-08 18:45:13.000000 BeeDrive-0.3.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 04:53:33.000000 BeeDrive-0.4.0.0/
+-rw-rw-rw-   0        0        0     9719 2023-07-01 04:53:33.000000 BeeDrive-0.4.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-01 04:53:33.000000 BeeDrive-0.4.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1439 2022-02-22 04:49:08.000000 BeeDrive-0.4.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `BeeDrive-0.3.7.1/PKG-INFO` & `BeeDrive-0.4.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BeeDrive
-Version: 0.3.7.1
+Version: 0.4.0.0
 Summary: BeeDrive: Open Source Privacy File Transfering System for Teams and Individual Developers
 Home-page: https://github.com/JacksonWuxs/BeeDrive
 Author: Xuansheng Wu
 Maintainer: Xuansheng Wu
 License: GPL v3
 Platform: all
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `BeeDrive-0.3.7.1/setup.py` & `BeeDrive-0.4.0.0/setup.py`

 * *Files identical despite different names*

