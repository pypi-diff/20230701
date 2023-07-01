# Comparing `tmp/openplugincore-0.3.1.tar.gz` & `tmp/openplugincore-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openplugincore-0.3.1.tar", last modified: Sat Jul  1 18:01:43 2023, max compression
+gzip compressed data, was "openplugincore-0.3.2.tar", last modified: Sat Jul  1 18:06:11 2023, max compression
```

## Comparing `openplugincore-0.3.1.tar` & `openplugincore-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 18:01:43.170945 openplugincore-0.3.1/
--rw-rw-rw-   0        0        0      826 2023-07-01 18:01:43.169943 openplugincore-0.3.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-01 18:01:43.140945 openplugincore-0.3.1/openplugincore/
--rw-rw-rw-   0        0        0       61 2023-07-01 15:22:26.000000 openplugincore-0.3.1/openplugincore/__init__.py
--rw-rw-rw-   0        0        0     9291 2023-07-01 15:16:30.000000 openplugincore-0.3.1/openplugincore/openplugincore.py
--rw-rw-rw-   0        0        0      696 2023-06-27 03:28:44.000000 openplugincore-0.3.1/openplugincore/types.py
-drwxrwxrwx   0        0        0        0 2023-07-01 18:01:43.161945 openplugincore-0.3.1/openplugincore.egg-info/
--rw-rw-rw-   0        0        0      826 2023-07-01 18:01:43.000000 openplugincore-0.3.1/openplugincore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-07-01 18:01:43.000000 openplugincore-0.3.1/openplugincore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 18:01:43.000000 openplugincore-0.3.1/openplugincore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-07-01 18:01:43.000000 openplugincore-0.3.1/openplugincore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-01 18:01:43.000000 openplugincore-0.3.1/openplugincore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 18:01:43.170945 openplugincore-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1511 2023-07-01 18:01:41.000000 openplugincore-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 18:01:43.167943 openplugincore-0.3.1/tests/
--rw-rw-rw-   0        0        0        0 2023-06-30 23:02:19.000000 openplugincore-0.3.1/tests/__init__.py
--rw-rw-rw-   0        0        0     1589 2023-07-01 01:03:27.000000 openplugincore-0.3.1/tests/mock_data.py
--rw-rw-rw-   0        0        0     2491 2023-07-01 15:22:55.000000 openplugincore-0.3.1/tests/test_basicTest.py
--rw-rw-rw-   0        0        0    13215 2023-07-01 15:23:05.000000 openplugincore-0.3.1/tests/test_e2e.py
+drwxrwxrwx   0        0        0        0 2023-07-01 18:06:11.184897 openplugincore-0.3.2/
+-rw-rw-rw-   0        0        0      826 2023-07-01 18:06:11.183899 openplugincore-0.3.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-01 18:06:11.150898 openplugincore-0.3.2/openplugincore/
+-rw-rw-rw-   0        0        0       61 2023-07-01 15:22:26.000000 openplugincore-0.3.2/openplugincore/__init__.py
+-rw-rw-rw-   0        0        0     9291 2023-07-01 15:16:30.000000 openplugincore-0.3.2/openplugincore/openplugincore.py
+-rw-rw-rw-   0        0        0    19151 2023-07-01 05:38:42.000000 openplugincore-0.3.2/openplugincore/plugins.json
+-rw-rw-rw-   0        0        0      696 2023-06-27 03:28:44.000000 openplugincore-0.3.2/openplugincore/types.py
+drwxrwxrwx   0        0        0        0 2023-07-01 18:06:11.175898 openplugincore-0.3.2/openplugincore.egg-info/
+-rw-rw-rw-   0        0        0      826 2023-07-01 18:06:11.000000 openplugincore-0.3.2/openplugincore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2023-07-01 18:06:11.000000 openplugincore-0.3.2/openplugincore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 18:06:11.000000 openplugincore-0.3.2/openplugincore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-07-01 18:06:11.000000 openplugincore-0.3.2/openplugincore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-01 18:06:11.000000 openplugincore-0.3.2/openplugincore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 18:06:11.184897 openplugincore-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1515 2023-07-01 18:06:08.000000 openplugincore-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 18:06:11.181901 openplugincore-0.3.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-30 23:02:19.000000 openplugincore-0.3.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     1589 2023-07-01 01:03:27.000000 openplugincore-0.3.2/tests/mock_data.py
+-rw-rw-rw-   0        0        0     2491 2023-07-01 15:22:55.000000 openplugincore-0.3.2/tests/test_basicTest.py
+-rw-rw-rw-   0        0        0    13215 2023-07-01 15:23:05.000000 openplugincore-0.3.2/tests/test_e2e.py
```

### Comparing `openplugincore-0.3.1/PKG-INFO` & `openplugincore-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openplugincore
-Version: 0.3.1
+Version: 0.3.2
 Summary: Seamlessly integrate with OpenAI ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!
 Home-page: UNKNOWN
 Author: Sebastian Sosa
 Author-email: 1sebastian1sosa1@gmail.com
 License: UNKNOWN
 Keywords: python,openai,chatgpt,chat,plugin
 Platform: UNKNOWN
```

### Comparing `openplugincore-0.3.1/openplugincore/openplugincore.py` & `openplugincore-0.3.2/openplugincore/openplugincore.py`

 * *Files identical despite different names*

### Comparing `openplugincore-0.3.1/openplugincore/types.py` & `openplugincore-0.3.2/openplugincore/types.py`

 * *Files identical despite different names*

### Comparing `openplugincore-0.3.1/openplugincore.egg-info/PKG-INFO` & `openplugincore-0.3.2/openplugincore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openplugincore
-Version: 0.3.1
+Version: 0.3.2
 Summary: Seamlessly integrate with OpenAI ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!
 Home-page: UNKNOWN
 Author: Sebastian Sosa
 Author-email: 1sebastian1sosa1@gmail.com
 License: UNKNOWN
 Keywords: python,openai,chatgpt,chat,plugin
 Platform: UNKNOWN
```

### Comparing `openplugincore-0.3.1/setup.py` & `openplugincore-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name='openplugincore', 
-        version="0.3.1",
+        version="0.3.2",
         author="Sebastian Sosa",
         author_email="1sebastian1sosa1@gmail.com",
         description='Seamlessly integrate with OpenAI ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!',
         long_description='Seamlessly integrate with OpenAIs ChatGPT plugins via API (or client), offering the same powerful functionality as the ChatGPT api + plugins!',
         packages=find_packages(),
         package_data={
-            "openplugin": ["*.json"],  # include all .json files in the openplugin package
+            "openplugincore": ["*.json"],  # include all .json files in the openplugin package
         },
         exclude=['tests'],
         install_requires=[
             'pyyaml',
             'requests',
             'openai',
             'langchain',
```

### Comparing `openplugincore-0.3.1/tests/mock_data.py` & `openplugincore-0.3.2/tests/mock_data.py`

 * *Files identical despite different names*

### Comparing `openplugincore-0.3.1/tests/test_basicTest.py` & `openplugincore-0.3.2/tests/test_basicTest.py`

 * *Files identical despite different names*

### Comparing `openplugincore-0.3.1/tests/test_e2e.py` & `openplugincore-0.3.2/tests/test_e2e.py`

 * *Files identical despite different names*

