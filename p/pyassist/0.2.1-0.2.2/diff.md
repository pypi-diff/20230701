# Comparing `tmp/pyassist-0.2.1.tar.gz` & `tmp/pyassist-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyassist-0.2.1.tar", last modified: Sat Jul  1 21:17:42 2023, max compression
+gzip compressed data, was "pyassist-0.2.2.tar", last modified: Sat Jul  1 21:37:32 2023, max compression
```

## Comparing `pyassist-0.2.1.tar` & `pyassist-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 21:17:42.193514 pyassist-0.2.1/
--rw-rw-rw-   0        0        0     1063 2023-06-28 16:14:31.000000 pyassist-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      871 2023-07-01 21:17:42.194513 pyassist-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       52 2023-06-28 16:30:47.000000 pyassist-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 21:17:42.181516 pyassist-0.2.1/pyassist/
--rw-rw-rw-   0        0        0      102 2023-07-01 21:15:26.000000 pyassist-0.2.1/pyassist/__init__.py
--rw-rw-rw-   0        0        0     1834 2023-06-29 10:33:09.000000 pyassist-0.2.1/pyassist/process.py
--rw-rw-rw-   0        0        0     1961 2023-06-29 10:33:04.000000 pyassist-0.2.1/pyassist/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-01 21:17:42.193514 pyassist-0.2.1/pyassist.egg-info/
--rw-rw-rw-   0        0        0      871 2023-07-01 21:17:42.000000 pyassist-0.2.1/pyassist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-07-01 21:17:42.000000 pyassist-0.2.1/pyassist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 21:17:42.000000 pyassist-0.2.1/pyassist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-07-01 21:17:42.000000 pyassist-0.2.1/pyassist.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-01 21:17:42.000000 pyassist-0.2.1/pyassist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-01 21:17:42.195515 pyassist-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1980 2023-07-01 20:15:27.000000 pyassist-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 21:37:32.106194 pyassist-0.2.2/
+-rw-rw-rw-   0        0        0     1063 2023-06-28 16:14:31.000000 pyassist-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      871 2023-07-01 21:37:32.106194 pyassist-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2023-06-28 16:30:47.000000 pyassist-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 21:37:32.077686 pyassist-0.2.2/pyassist/
+drwxrwxrwx   0        0        0        0 2023-07-01 21:37:32.103195 pyassist-0.2.2/pyassist/Network/
+-rw-rw-rw-   0        0        0       54 2023-06-29 10:38:20.000000 pyassist-0.2.2/pyassist/Network/__init__.py
+-rw-rw-rw-   0        0        0     7013 2023-06-29 10:36:06.000000 pyassist-0.2.2/pyassist/Network/network.py
+-rw-rw-rw-   0        0        0     8704 2023-06-29 10:57:47.000000 pyassist-0.2.2/pyassist/Network/proxy.py
+drwxrwxrwx   0        0        0        0 2023-07-01 21:37:32.105196 pyassist-0.2.2/pyassist/Scraper/
+-rw-rw-rw-   0        0        0       52 2023-06-29 11:24:12.000000 pyassist-0.2.2/pyassist/Scraper/__init__.py
+-rw-rw-rw-   0        0        0     1821 2023-06-29 11:22:50.000000 pyassist-0.2.2/pyassist/Scraper/bs4.py
+-rw-rw-rw-   0        0        0     3960 2023-06-30 17:19:32.000000 pyassist-0.2.2/pyassist/Scraper/selenium.py
+-rw-rw-rw-   0        0        0      102 2023-07-01 21:15:26.000000 pyassist-0.2.2/pyassist/__init__.py
+-rw-rw-rw-   0        0        0     1834 2023-06-29 10:33:09.000000 pyassist-0.2.2/pyassist/process.py
+-rw-rw-rw-   0        0        0     1961 2023-06-29 10:33:04.000000 pyassist-0.2.2/pyassist/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-01 21:37:32.091194 pyassist-0.2.2/pyassist.egg-info/
+-rw-rw-rw-   0        0        0      871 2023-07-01 21:37:32.000000 pyassist-0.2.2/pyassist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      419 2023-07-01 21:37:32.000000 pyassist-0.2.2/pyassist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 21:37:32.000000 pyassist-0.2.2/pyassist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-07-01 21:37:32.000000 pyassist-0.2.2/pyassist.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-01 21:37:32.000000 pyassist-0.2.2/pyassist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-01 21:37:32.110194 pyassist-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     2050 2023-07-01 21:35:10.000000 pyassist-0.2.2/setup.py
```

### Comparing `pyassist-0.2.1/LICENSE` & `pyassist-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyassist-0.2.1/PKG-INFO` & `pyassist-0.2.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyassist
-Version: 0.2.1
+Version: 0.2.2
 Summary: This is Python Utility
 Home-page: https://github.com/ISabariRajan
-Download-URL: https://github.com/ISabariRajan/Utilities/archive/refs/tags/v-0.2.1.tar.gz
+Download-URL: https://github.com/ISabariRajan/Utilities/archive/refs/tags/v-0.2.2.tar.gz
 Author: Sabari Rajan
 Author-email: mailme@isbarirajan.com
 License: MIT
 Keywords: Utility,utils,pyutils,assist,easy,service
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `pyassist-0.2.1/pyassist/process.py` & `pyassist-0.2.2/pyassist/process.py`

 * *Files identical despite different names*

### Comparing `pyassist-0.2.1/pyassist/utils.py` & `pyassist-0.2.2/pyassist/utils.py`

 * *Files identical despite different names*

### Comparing `pyassist-0.2.1/pyassist.egg-info/PKG-INFO` & `pyassist-0.2.2/pyassist.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyassist
-Version: 0.2.1
+Version: 0.2.2
 Summary: This is Python Utility
 Home-page: https://github.com/ISabariRajan
-Download-URL: https://github.com/ISabariRajan/Utilities/archive/refs/tags/v-0.2.1.tar.gz
+Download-URL: https://github.com/ISabariRajan/Utilities/archive/refs/tags/v-0.2.2.tar.gz
 Author: Sabari Rajan
 Author-email: mailme@isbarirajan.com
 License: MIT
 Keywords: Utility,utils,pyutils,assist,easy,service
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `pyassist-0.2.1/setup.py` & `pyassist-0.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from setuptools import setup
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setup(
   name = 'pyassist',         # How you named your package folder (MyLib)
-  packages = ['pyassist'],   # Chose the same as "name"
-  version = '0.2.1',      # Start with a small number and increase it with every change you make
+  packages = [
+      'pyassist',
+      'pyassist.Network',
+      'pyassist.Scraper'
+      ],   # Chose the same as "name"
+  version = '0.2.2',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = """This is Python Utility""",   # Give a short description about your library
   author = 'Sabari Rajan',                   # Type in your name
   author_email = 'mailme@isbarirajan.com',      # Type in your E-Mail
   url = 'https://github.com/ISabariRajan',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/ISabariRajan/Utilities/archive/refs/tags/v-0.2.1.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/ISabariRajan/Utilities/archive/refs/tags/v-0.2.2.tar.gz',    # I explain this later on
   keywords = ['Utility', 'utils', 'pyutils', 'assist', 'easy', 'service'],   # Keywords that define your package best
   install_requires=[
       "lxml", "pyloggerutils", "requests", "urllib3", "BeautifulSoup4", "webdriver_manager", "selenium"
   ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
```

