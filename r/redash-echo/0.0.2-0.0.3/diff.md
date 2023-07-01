# Comparing `tmp/redash-echo-0.0.2.tar.gz` & `tmp/redash-echo-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redash-echo-0.0.2.tar", last modified: Sat Jul  1 00:09:55 2023, max compression
+gzip compressed data, was "redash-echo-0.0.3.tar", last modified: Sat Jul  1 02:22:19 2023, max compression
```

## Comparing `redash-echo-0.0.2.tar` & `redash-echo-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 00:09:55.978524 redash-echo-0.0.2/
--rw-rw-rw-   0        0        0      357 2023-07-01 00:09:55.978524 redash-echo-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-24 05:58:23.000000 redash-echo-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 00:09:55.941763 redash-echo-0.0.2/redash-echo/
--rw-rw-rw-   0        0        0      115 2023-07-01 00:08:29.000000 redash-echo-0.0.2/redash-echo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 00:09:55.945763 redash-echo-0.0.2/redash-echo/config/
--rw-rw-rw-   0        0        0        0 2023-06-28 01:29:08.000000 redash-echo-0.0.2/redash-echo/config/__init__.py
--rw-rw-rw-   0        0        0      546 2023-06-28 02:42:15.000000 redash-echo-0.0.2/redash-echo/config/yaml.py
--rw-rw-rw-   0        0        0     4671 2023-06-29 09:59:24.000000 redash-echo-0.0.2/redash-echo/main.py
-drwxrwxrwx   0        0        0        0 2023-07-01 00:09:55.948763 redash-echo-0.0.2/redash-echo/redash/
--rw-rw-rw-   0        0        0        0 2023-06-24 05:59:03.000000 redash-echo-0.0.2/redash-echo/redash/__init__.py
--rw-rw-rw-   0        0        0     2919 2023-06-29 09:37:22.000000 redash-echo-0.0.2/redash-echo/redash/data.py
-drwxrwxrwx   0        0        0        0 2023-07-01 00:09:55.951763 redash-echo-0.0.2/redash-echo/slack/
--rw-rw-rw-   0        0        0        0 2023-06-24 07:43:43.000000 redash-echo-0.0.2/redash-echo/slack/__init__.py
--rw-rw-rw-   0        0        0     1066 2023-06-28 05:31:00.000000 redash-echo-0.0.2/redash-echo/slack/messages.py
-drwxrwxrwx   0        0        0        0 2023-07-01 00:09:55.976947 redash-echo-0.0.2/redash_echo.egg-info/
--rw-rw-rw-   0        0        0      357 2023-07-01 00:09:55.000000 redash-echo-0.0.2/redash_echo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      446 2023-07-01 00:09:55.000000 redash-echo-0.0.2/redash_echo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 00:09:55.000000 redash-echo-0.0.2/redash_echo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-30 23:44:09.000000 redash-echo-0.0.2/redash_echo.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       34 2023-07-01 00:09:55.000000 redash-echo-0.0.2/redash_echo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-01 00:09:55.000000 redash-echo-0.0.2/redash_echo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 00:09:55.979521 redash-echo-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      569 2023-06-30 23:59:58.000000 redash-echo-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 02:22:19.764335 redash-echo-0.0.3/
+-rw-rw-rw-   0        0        0      357 2023-07-01 02:22:19.764335 redash-echo-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-24 05:58:23.000000 redash-echo-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 02:22:19.676720 redash-echo-0.0.3/redash-echo/
+-rw-rw-rw-   0        0        0      124 2023-07-01 02:17:39.000000 redash-echo-0.0.3/redash-echo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 02:22:19.680721 redash-echo-0.0.3/redash-echo/config/
+-rw-rw-rw-   0        0        0        0 2023-07-01 00:52:33.000000 redash-echo-0.0.3/redash-echo/config/__init__.py
+-rw-rw-rw-   0        0        0      546 2023-07-01 00:52:33.000000 redash-echo-0.0.3/redash-echo/config/yaml.py
+-rw-rw-rw-   0        0        0     4671 2023-07-01 00:52:34.000000 redash-echo-0.0.3/redash-echo/main.py
+drwxrwxrwx   0        0        0        0 2023-07-01 02:22:19.693191 redash-echo-0.0.3/redash-echo/redash/
+-rw-rw-rw-   0        0        0        0 2023-07-01 00:52:34.000000 redash-echo-0.0.3/redash-echo/redash/__init__.py
+-rw-rw-rw-   0        0        0     2919 2023-07-01 00:52:34.000000 redash-echo-0.0.3/redash-echo/redash/data.py
+drwxrwxrwx   0        0        0        0 2023-07-01 02:22:19.727777 redash-echo-0.0.3/redash-echo/slack/
+-rw-rw-rw-   0        0        0        0 2023-07-01 00:52:34.000000 redash-echo-0.0.3/redash-echo/slack/__init__.py
+-rw-rw-rw-   0        0        0     1066 2023-07-01 00:52:34.000000 redash-echo-0.0.3/redash-echo/slack/messages.py
+drwxrwxrwx   0        0        0        0 2023-07-01 02:22:19.762350 redash-echo-0.0.3/redash_echo.egg-info/
+-rw-rw-rw-   0        0        0      357 2023-07-01 02:22:19.000000 redash-echo-0.0.3/redash_echo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      622 2023-07-01 02:22:19.000000 redash-echo-0.0.3/redash_echo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 02:22:19.000000 redash-echo-0.0.3/redash_echo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-30 23:44:09.000000 redash-echo-0.0.3/redash_echo.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       49 2023-07-01 02:22:19.000000 redash-echo-0.0.3/redash_echo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       68 2023-07-01 02:22:19.000000 redash-echo-0.0.3/redash_echo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 02:22:19.765335 redash-echo-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      642 2023-07-01 02:21:17.000000 redash-echo-0.0.3/setup.py
```

### Comparing `redash-echo-0.0.2/redash-echo/config/yaml.py` & `redash-echo-0.0.3/redash-echo/config/yaml.py`

 * *Files identical despite different names*

### Comparing `redash-echo-0.0.2/redash-echo/main.py` & `redash-echo-0.0.3/redash-echo/main.py`

 * *Files identical despite different names*

### Comparing `redash-echo-0.0.2/redash-echo/redash/data.py` & `redash-echo-0.0.3/redash-echo/redash/data.py`

 * *Files identical despite different names*

### Comparing `redash-echo-0.0.2/redash-echo/slack/messages.py` & `redash-echo-0.0.3/redash-echo/slack/messages.py`

 * *Files identical despite different names*

### Comparing `redash-echo-0.0.2/setup.py` & `redash-echo-0.0.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='redash-echo',
-    version='0.0.2',
+    version='0.0.3',
     description='A tool integrating Redash with Slack',
     author='Yun',
     author_email='ysjhmtb@gmail.com',
     url='https://github.com/yunseokjeon/redash-echo',
-    install_requires=['PyYAML', 'requests', 'seaborn', 'slack_sdk'],
-    packages=find_packages(exclude=[]),
+    install_requires=['PyYAML', 'requests', 'seaborn', 'slack_sdk', 'cron_converter'],
+    packages=['redash-echo', 'redash-echo/config', 'redash-echo/redash', 'redash-echo/slack'],
     keywords=['Redash', 'Slack'],
     python_requires='>=3.11',
     package_data={},
     zip_safe=False,
     classifiers=[
         'Programming Language :: Python :: 3.11'
     ]
```

