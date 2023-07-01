# Comparing `tmp/redash-echo-0.0.3.tar.gz` & `tmp/redash-echo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redash-echo-0.0.3.tar", last modified: Sat Jul  1 02:22:19 2023, max compression
+gzip compressed data, was "redash-echo-0.0.4.tar", last modified: Sat Jul  1 02:55:44 2023, max compression
```

## Comparing `redash-echo-0.0.3.tar` & `redash-echo-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 02:22:19.764335 redash-echo-0.0.3/
--rw-rw-rw-   0        0        0      357 2023-07-01 02:22:19.764335 redash-echo-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-24 05:58:23.000000 redash-echo-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 02:22:19.676720 redash-echo-0.0.3/redash-echo/
--rw-rw-rw-   0        0        0      124 2023-07-01 02:17:39.000000 redash-echo-0.0.3/redash-echo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 02:22:19.680721 redash-echo-0.0.3/redash-echo/config/
--rw-rw-rw-   0        0        0        0 2023-07-01 00:52:33.000000 redash-echo-0.0.3/redash-echo/config/__init__.py
--rw-rw-rw-   0        0        0      546 2023-07-01 00:52:33.000000 redash-echo-0.0.3/redash-echo/config/yaml.py
--rw-rw-rw-   0        0        0     4671 2023-07-01 00:52:34.000000 redash-echo-0.0.3/redash-echo/main.py
-drwxrwxrwx   0        0        0        0 2023-07-01 02:22:19.693191 redash-echo-0.0.3/redash-echo/redash/
--rw-rw-rw-   0        0        0        0 2023-07-01 00:52:34.000000 redash-echo-0.0.3/redash-echo/redash/__init__.py
--rw-rw-rw-   0        0        0     2919 2023-07-01 00:52:34.000000 redash-echo-0.0.3/redash-echo/redash/data.py
-drwxrwxrwx   0        0        0        0 2023-07-01 02:22:19.727777 redash-echo-0.0.3/redash-echo/slack/
--rw-rw-rw-   0        0        0        0 2023-07-01 00:52:34.000000 redash-echo-0.0.3/redash-echo/slack/__init__.py
--rw-rw-rw-   0        0        0     1066 2023-07-01 00:52:34.000000 redash-echo-0.0.3/redash-echo/slack/messages.py
-drwxrwxrwx   0        0        0        0 2023-07-01 02:22:19.762350 redash-echo-0.0.3/redash_echo.egg-info/
--rw-rw-rw-   0        0        0      357 2023-07-01 02:22:19.000000 redash-echo-0.0.3/redash_echo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      622 2023-07-01 02:22:19.000000 redash-echo-0.0.3/redash_echo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 02:22:19.000000 redash-echo-0.0.3/redash_echo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-30 23:44:09.000000 redash-echo-0.0.3/redash_echo.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       49 2023-07-01 02:22:19.000000 redash-echo-0.0.3/redash_echo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       68 2023-07-01 02:22:19.000000 redash-echo-0.0.3/redash_echo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 02:22:19.765335 redash-echo-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      642 2023-07-01 02:21:17.000000 redash-echo-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 02:55:44.442627 redash-echo-0.0.4/
+-rw-rw-rw-   0        0        0      357 2023-07-01 02:55:44.442627 redash-echo-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-24 05:58:23.000000 redash-echo-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 02:55:44.424635 redash-echo-0.0.4/redash_echo.egg-info/
+-rw-rw-rw-   0        0        0      357 2023-07-01 02:55:44.000000 redash-echo-0.0.4/redash_echo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      438 2023-07-01 02:55:44.000000 redash-echo-0.0.4/redash_echo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 02:55:44.000000 redash-echo-0.0.4/redash_echo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-30 23:44:09.000000 redash-echo-0.0.4/redash_echo.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       49 2023-07-01 02:55:44.000000 redash-echo-0.0.4/redash_echo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-01 02:55:44.000000 redash-echo-0.0.4/redash_echo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 02:55:44.427753 redash-echo-0.0.4/redashecho/
+-rw-rw-rw-   0        0        0      124 2023-07-01 02:54:59.000000 redash-echo-0.0.4/redashecho/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 02:55:44.431755 redash-echo-0.0.4/redashecho/config/
+-rw-rw-rw-   0        0        0        0 2023-07-01 00:52:33.000000 redash-echo-0.0.4/redashecho/config/__init__.py
+-rw-rw-rw-   0        0        0      546 2023-07-01 00:52:33.000000 redash-echo-0.0.4/redashecho/config/yaml.py
+-rw-rw-rw-   0        0        0     4671 2023-07-01 00:52:34.000000 redash-echo-0.0.4/redashecho/main.py
+drwxrwxrwx   0        0        0        0 2023-07-01 02:55:44.435755 redash-echo-0.0.4/redashecho/redash/
+-rw-rw-rw-   0        0        0        0 2023-07-01 00:52:34.000000 redash-echo-0.0.4/redashecho/redash/__init__.py
+-rw-rw-rw-   0        0        0     2919 2023-07-01 00:52:34.000000 redash-echo-0.0.4/redashecho/redash/data.py
+drwxrwxrwx   0        0        0        0 2023-07-01 02:55:44.439754 redash-echo-0.0.4/redashecho/slack/
+-rw-rw-rw-   0        0        0        0 2023-07-01 00:52:34.000000 redash-echo-0.0.4/redashecho/slack/__init__.py
+-rw-rw-rw-   0        0        0     1066 2023-07-01 00:52:34.000000 redash-echo-0.0.4/redashecho/slack/messages.py
+-rw-rw-rw-   0        0        0       42 2023-07-01 02:55:44.443633 redash-echo-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      587 2023-07-01 02:54:58.000000 redash-echo-0.0.4/setup.py
```

### Comparing `redash-echo-0.0.3/redash-echo/config/yaml.py` & `redash-echo-0.0.4/redashecho/config/yaml.py`

 * *Files identical despite different names*

### Comparing `redash-echo-0.0.3/redash-echo/main.py` & `redash-echo-0.0.4/redashecho/main.py`

 * *Files identical despite different names*

### Comparing `redash-echo-0.0.3/redash-echo/redash/data.py` & `redash-echo-0.0.4/redashecho/redash/data.py`

 * *Files identical despite different names*

### Comparing `redash-echo-0.0.3/redash-echo/slack/messages.py` & `redash-echo-0.0.4/redashecho/slack/messages.py`

 * *Files identical despite different names*

### Comparing `redash-echo-0.0.3/setup.py` & `redash-echo-0.0.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='redash-echo',
-    version='0.0.3',
+    version='0.0.4',
     description='A tool integrating Redash with Slack',
     author='Yun',
     author_email='ysjhmtb@gmail.com',
     url='https://github.com/yunseokjeon/redash-echo',
     install_requires=['PyYAML', 'requests', 'seaborn', 'slack_sdk', 'cron_converter'],
-    packages=['redash-echo', 'redash-echo/config', 'redash-echo/redash', 'redash-echo/slack'],
+    packages=find_packages(exclude=[]),
     keywords=['Redash', 'Slack'],
     python_requires='>=3.11',
     package_data={},
     zip_safe=False,
     classifiers=[
         'Programming Language :: Python :: 3.11'
     ]
```

