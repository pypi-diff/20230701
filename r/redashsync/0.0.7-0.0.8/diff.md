# Comparing `tmp/redashsync-0.0.7.tar.gz` & `tmp/redashsync-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redashsync-0.0.7.tar", last modified: Sat Jul  1 03:19:50 2023, max compression
+gzip compressed data, was "redashsync-0.0.8.tar", last modified: Sat Jul  1 06:19:20 2023, max compression
```

## Comparing `redashsync-0.0.7.tar` & `redashsync-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 03:19:50.336788 redashsync-0.0.7/
--rw-rw-rw-   0        0        0      321 2023-07-01 03:19:50.335752 redashsync-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-01 03:19:50.301822 redashsync-0.0.7/redashsync/
--rw-rw-rw-   0        0        0      124 2023-07-01 03:19:02.000000 redashsync-0.0.7/redashsync/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 03:19:50.325454 redashsync-0.0.7/redashsync/config/
--rw-rw-rw-   0        0        0        0 2023-07-01 03:10:23.000000 redashsync-0.0.7/redashsync/config/__init__.py
--rw-rw-rw-   0        0        0      552 2023-07-01 03:10:37.000000 redashsync-0.0.7/redashsync/config/yaml.py
--rw-rw-rw-   0        0        0     4662 2023-07-01 03:12:08.000000 redashsync-0.0.7/redashsync/main.py
-drwxrwxrwx   0        0        0        0 2023-07-01 03:19:50.329452 redashsync-0.0.7/redashsync/redash/
--rw-rw-rw-   0        0        0        0 2023-07-01 03:10:51.000000 redashsync-0.0.7/redashsync/redash/__init__.py
--rw-rw-rw-   0        0        0     2919 2023-07-01 03:11:11.000000 redashsync-0.0.7/redashsync/redash/data.py
-drwxrwxrwx   0        0        0        0 2023-07-01 03:19:50.333421 redashsync-0.0.7/redashsync/slack/
--rw-rw-rw-   0        0        0        0 2023-07-01 03:11:26.000000 redashsync-0.0.7/redashsync/slack/__init__.py
--rw-rw-rw-   0        0        0     1068 2023-07-01 03:11:42.000000 redashsync-0.0.7/redashsync/slack/messages.py
-drwxrwxrwx   0        0        0        0 2023-07-01 03:19:50.322417 redashsync-0.0.7/redashsync.egg-info/
--rw-rw-rw-   0        0        0      321 2023-07-01 03:19:50.000000 redashsync-0.0.7/redashsync.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      422 2023-07-01 03:19:50.000000 redashsync-0.0.7/redashsync.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 03:19:50.000000 redashsync-0.0.7/redashsync.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-01 03:15:55.000000 redashsync-0.0.7/redashsync.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       49 2023-07-01 03:19:50.000000 redashsync-0.0.7/redashsync.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-01 03:19:50.000000 redashsync-0.0.7/redashsync.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 03:19:50.336788 redashsync-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      544 2023-07-01 03:19:03.000000 redashsync-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 06:19:20.762883 redashsync-0.0.8/
+-rw-rw-rw-   0        0        0     4103 2023-07-01 06:19:20.762883 redashsync-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3748 2023-07-01 06:11:16.000000 redashsync-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 06:19:20.715654 redashsync-0.0.8/redashsync/
+-rw-rw-rw-   0        0        0      124 2023-07-01 06:18:48.000000 redashsync-0.0.8/redashsync/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 06:19:20.752792 redashsync-0.0.8/redashsync/config/
+-rw-rw-rw-   0        0        0        0 2023-07-01 03:10:23.000000 redashsync-0.0.8/redashsync/config/__init__.py
+-rw-rw-rw-   0        0        0      552 2023-07-01 03:10:37.000000 redashsync-0.0.8/redashsync/config/yaml.py
+-rw-rw-rw-   0        0        0     4662 2023-07-01 03:12:08.000000 redashsync-0.0.8/redashsync/main.py
+drwxrwxrwx   0        0        0        0 2023-07-01 06:19:20.756796 redashsync-0.0.8/redashsync/redash/
+-rw-rw-rw-   0        0        0        0 2023-07-01 03:10:51.000000 redashsync-0.0.8/redashsync/redash/__init__.py
+-rw-rw-rw-   0        0        0     2919 2023-07-01 03:11:11.000000 redashsync-0.0.8/redashsync/redash/data.py
+drwxrwxrwx   0        0        0        0 2023-07-01 06:19:20.760879 redashsync-0.0.8/redashsync/slack/
+-rw-rw-rw-   0        0        0        0 2023-07-01 03:11:26.000000 redashsync-0.0.8/redashsync/slack/__init__.py
+-rw-rw-rw-   0        0        0     1068 2023-07-01 03:11:42.000000 redashsync-0.0.8/redashsync/slack/messages.py
+drwxrwxrwx   0        0        0        0 2023-07-01 06:19:20.748597 redashsync-0.0.8/redashsync.egg-info/
+-rw-rw-rw-   0        0        0     4103 2023-07-01 06:19:20.000000 redashsync-0.0.8/redashsync.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2023-07-01 06:19:20.000000 redashsync-0.0.8/redashsync.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 06:19:20.000000 redashsync-0.0.8/redashsync.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-01 03:15:55.000000 redashsync-0.0.8/redashsync.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       49 2023-07-01 06:19:20.000000 redashsync-0.0.8/redashsync.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-01 06:19:20.000000 redashsync-0.0.8/redashsync.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 06:19:20.763885 redashsync-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      721 2023-07-01 06:18:48.000000 redashsync-0.0.8/setup.py
```

### Comparing `redashsync-0.0.7/redashsync/config/yaml.py` & `redashsync-0.0.8/redashsync/config/yaml.py`

 * *Files identical despite different names*

### Comparing `redashsync-0.0.7/redashsync/main.py` & `redashsync-0.0.8/redashsync/main.py`

 * *Files identical despite different names*

### Comparing `redashsync-0.0.7/redashsync/redash/data.py` & `redashsync-0.0.8/redashsync/redash/data.py`

 * *Files identical despite different names*

### Comparing `redashsync-0.0.7/redashsync/slack/messages.py` & `redashsync-0.0.8/redashsync/slack/messages.py`

 * *Files identical despite different names*

### Comparing `redashsync-0.0.7/setup.py` & `redashsync-0.0.8/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from setuptools import setup, find_packages
 
+with open('README.md', encoding='utf-8') as f:
+    long_description = f.read()
+
 setup(
     name='redashsync',
-    version='0.0.7',
+    version='0.0.8',
     description='A tool integrating Redash with Slack',
+    long_description = long_description,
+    long_description_content_type='text/markdown',
     author='Yun',
     author_email='ysjhmtb@gmail.com',
     url='',
     install_requires=['PyYAML', 'requests', 'seaborn', 'slack_sdk', 'cron_converter'],
     packages=find_packages(exclude=[]),
     keywords=['Redash', 'Slack'],
     python_requires='>=3.11',
```

