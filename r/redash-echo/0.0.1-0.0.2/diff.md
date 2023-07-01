# Comparing `tmp/redash-echo-0.0.1.tar.gz` & `tmp/redash-echo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redash-echo-0.0.1.tar", last modified: Fri Jun 30 23:44:09 2023, max compression
+gzip compressed data, was "redash-echo-0.0.2.tar", last modified: Sat Jul  1 00:09:55 2023, max compression
```

## Comparing `redash-echo-0.0.1.tar` & `redash-echo-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 23:44:09.567905 redash-echo-0.0.1/
--rw-rw-rw-   0        0        0      357 2023-06-30 23:44:09.567905 redash-echo-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-24 05:58:23.000000 redash-echo-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 23:44:09.456861 redash-echo-0.0.1/redash-echo/
--rw-rw-rw-   0        0        0       21 2023-06-28 05:55:42.000000 redash-echo-0.0.1/redash-echo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 23:44:09.464875 redash-echo-0.0.1/redash-echo/config/
--rw-rw-rw-   0        0        0        0 2023-06-28 01:29:08.000000 redash-echo-0.0.1/redash-echo/config/__init__.py
--rw-rw-rw-   0        0        0      546 2023-06-28 02:42:15.000000 redash-echo-0.0.1/redash-echo/config/yaml.py
--rw-rw-rw-   0        0        0     4671 2023-06-29 09:59:24.000000 redash-echo-0.0.1/redash-echo/main.py
-drwxrwxrwx   0        0        0        0 2023-06-30 23:44:09.475860 redash-echo-0.0.1/redash-echo/redash/
--rw-rw-rw-   0        0        0        0 2023-06-24 05:59:03.000000 redash-echo-0.0.1/redash-echo/redash/__init__.py
--rw-rw-rw-   0        0        0     2919 2023-06-29 09:37:22.000000 redash-echo-0.0.1/redash-echo/redash/data.py
-drwxrwxrwx   0        0        0        0 2023-06-30 23:44:09.540392 redash-echo-0.0.1/redash-echo/slack/
--rw-rw-rw-   0        0        0        0 2023-06-24 07:43:43.000000 redash-echo-0.0.1/redash-echo/slack/__init__.py
--rw-rw-rw-   0        0        0     1066 2023-06-28 05:31:00.000000 redash-echo-0.0.1/redash-echo/slack/messages.py
-drwxrwxrwx   0        0        0        0 2023-06-30 23:44:09.565910 redash-echo-0.0.1/redash_echo.egg-info/
--rw-rw-rw-   0        0        0      357 2023-06-30 23:44:09.000000 redash-echo-0.0.1/redash_echo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      446 2023-06-30 23:44:09.000000 redash-echo-0.0.1/redash_echo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 23:44:09.000000 redash-echo-0.0.1/redash_echo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-30 23:44:09.000000 redash-echo-0.0.1/redash_echo.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       34 2023-06-30 23:44:09.000000 redash-echo-0.0.1/redash_echo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-30 23:44:09.000000 redash-echo-0.0.1/redash_echo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 23:44:09.567905 redash-echo-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      569 2023-06-28 05:55:26.000000 redash-echo-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 00:09:55.978524 redash-echo-0.0.2/
+-rw-rw-rw-   0        0        0      357 2023-07-01 00:09:55.978524 redash-echo-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-24 05:58:23.000000 redash-echo-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 00:09:55.941763 redash-echo-0.0.2/redash-echo/
+-rw-rw-rw-   0        0        0      115 2023-07-01 00:08:29.000000 redash-echo-0.0.2/redash-echo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 00:09:55.945763 redash-echo-0.0.2/redash-echo/config/
+-rw-rw-rw-   0        0        0        0 2023-06-28 01:29:08.000000 redash-echo-0.0.2/redash-echo/config/__init__.py
+-rw-rw-rw-   0        0        0      546 2023-06-28 02:42:15.000000 redash-echo-0.0.2/redash-echo/config/yaml.py
+-rw-rw-rw-   0        0        0     4671 2023-06-29 09:59:24.000000 redash-echo-0.0.2/redash-echo/main.py
+drwxrwxrwx   0        0        0        0 2023-07-01 00:09:55.948763 redash-echo-0.0.2/redash-echo/redash/
+-rw-rw-rw-   0        0        0        0 2023-06-24 05:59:03.000000 redash-echo-0.0.2/redash-echo/redash/__init__.py
+-rw-rw-rw-   0        0        0     2919 2023-06-29 09:37:22.000000 redash-echo-0.0.2/redash-echo/redash/data.py
+drwxrwxrwx   0        0        0        0 2023-07-01 00:09:55.951763 redash-echo-0.0.2/redash-echo/slack/
+-rw-rw-rw-   0        0        0        0 2023-06-24 07:43:43.000000 redash-echo-0.0.2/redash-echo/slack/__init__.py
+-rw-rw-rw-   0        0        0     1066 2023-06-28 05:31:00.000000 redash-echo-0.0.2/redash-echo/slack/messages.py
+drwxrwxrwx   0        0        0        0 2023-07-01 00:09:55.976947 redash-echo-0.0.2/redash_echo.egg-info/
+-rw-rw-rw-   0        0        0      357 2023-07-01 00:09:55.000000 redash-echo-0.0.2/redash_echo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      446 2023-07-01 00:09:55.000000 redash-echo-0.0.2/redash_echo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 00:09:55.000000 redash-echo-0.0.2/redash_echo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-30 23:44:09.000000 redash-echo-0.0.2/redash_echo.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       34 2023-07-01 00:09:55.000000 redash-echo-0.0.2/redash_echo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-01 00:09:55.000000 redash-echo-0.0.2/redash_echo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 00:09:55.979521 redash-echo-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      569 2023-06-30 23:59:58.000000 redash-echo-0.0.2/setup.py
```

### Comparing `redash-echo-0.0.1/redash-echo/config/yaml.py` & `redash-echo-0.0.2/redash-echo/config/yaml.py`

 * *Files identical despite different names*

### Comparing `redash-echo-0.0.1/redash-echo/main.py` & `redash-echo-0.0.2/redash-echo/main.py`

 * *Files identical despite different names*

### Comparing `redash-echo-0.0.1/redash-echo/redash/data.py` & `redash-echo-0.0.2/redash-echo/redash/data.py`

 * *Files identical despite different names*

### Comparing `redash-echo-0.0.1/redash-echo/slack/messages.py` & `redash-echo-0.0.2/redash-echo/slack/messages.py`

 * *Files identical despite different names*

### Comparing `redash-echo-0.0.1/setup.py` & `redash-echo-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='redash-echo',
-    version='0.0.1',
+    version='0.0.2',
     description='A tool integrating Redash with Slack',
     author='Yun',
     author_email='ysjhmtb@gmail.com',
     url='https://github.com/yunseokjeon/redash-echo',
     install_requires=['PyYAML', 'requests', 'seaborn', 'slack_sdk'],
     packages=find_packages(exclude=[]),
     keywords=['Redash', 'Slack'],
```

