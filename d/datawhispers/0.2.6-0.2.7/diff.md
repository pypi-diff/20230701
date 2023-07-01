# Comparing `tmp/datawhispers-0.2.6.tar.gz` & `tmp/datawhispers-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawhispers-0.2.6.tar", last modified: Sat Jul  1 13:49:58 2023, max compression
+gzip compressed data, was "datawhispers-0.2.7.tar", last modified: Sat Jul  1 16:58:48 2023, max compression
```

## Comparing `datawhispers-0.2.6.tar` & `datawhispers-0.2.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-01 13:49:58.376687 datawhispers-0.2.6/
--rw-r--r--   0 german     (501) staff       (20)     1061 2023-07-01 09:46:39.000000 datawhispers-0.2.6/LICENSE
--rw-r--r--   0 german     (501) staff       (20)     1079 2023-07-01 13:49:58.376561 datawhispers-0.2.6/PKG-INFO
--rw-r--r--   0 german     (501) staff       (20)      436 2023-07-01 11:20:15.000000 datawhispers-0.2.6/README.md
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-01 13:49:58.375457 datawhispers-0.2.6/datawhispers/
--rw-r--r--   0 german     (501) staff       (20)       75 2023-07-01 10:41:44.000000 datawhispers-0.2.6/datawhispers/__init__.py
--rw-r--r--   0 german     (501) staff       (20)     8342 2023-07-01 13:49:41.000000 datawhispers-0.2.6/datawhispers/advanced_prog.py
--rw-r--r--   0 german     (501) staff       (20)     7569 2023-07-01 09:48:05.000000 datawhispers-0.2.6/datawhispers/datavis.py
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-01 13:49:58.376356 datawhispers-0.2.6/datawhispers.egg-info/
--rw-r--r--   0 german     (501) staff       (20)     1079 2023-07-01 13:49:58.000000 datawhispers-0.2.6/datawhispers.egg-info/PKG-INFO
--rw-r--r--   0 german     (501) staff       (20)      284 2023-07-01 13:49:58.000000 datawhispers-0.2.6/datawhispers.egg-info/SOURCES.txt
--rw-r--r--   0 german     (501) staff       (20)        1 2023-07-01 13:49:58.000000 datawhispers-0.2.6/datawhispers.egg-info/dependency_links.txt
--rw-r--r--   0 german     (501) staff       (20)       38 2023-07-01 13:49:58.000000 datawhispers-0.2.6/datawhispers.egg-info/requires.txt
--rw-r--r--   0 german     (501) staff       (20)       13 2023-07-01 13:49:58.000000 datawhispers-0.2.6/datawhispers.egg-info/top_level.txt
--rw-r--r--   0 german     (501) staff       (20)       38 2023-07-01 13:49:58.376729 datawhispers-0.2.6/setup.cfg
--rw-r--r--   0 german     (501) staff       (20)     2059 2023-07-01 13:49:51.000000 datawhispers-0.2.6/setup.py
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-01 16:58:48.038656 datawhispers-0.2.7/
+-rw-r--r--   0 german     (501) staff       (20)     1061 2023-07-01 09:46:39.000000 datawhispers-0.2.7/LICENSE
+-rw-r--r--   0 german     (501) staff       (20)     1556 2023-07-01 16:58:48.038536 datawhispers-0.2.7/PKG-INFO
+-rw-r--r--   0 german     (501) staff       (20)      436 2023-07-01 11:20:15.000000 datawhispers-0.2.7/README.md
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-01 16:58:48.037542 datawhispers-0.2.7/datawhispers/
+-rw-r--r--   0 german     (501) staff       (20)       75 2023-07-01 10:41:44.000000 datawhispers-0.2.7/datawhispers/__init__.py
+-rw-r--r--   0 german     (501) staff       (20)     8342 2023-07-01 13:49:41.000000 datawhispers-0.2.7/datawhispers/advanced_prog.py
+-rw-r--r--   0 german     (501) staff       (20)     7569 2023-07-01 09:48:05.000000 datawhispers-0.2.7/datawhispers/datavis.py
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-01 16:58:48.038323 datawhispers-0.2.7/datawhispers.egg-info/
+-rw-r--r--   0 german     (501) staff       (20)     1556 2023-07-01 16:58:48.000000 datawhispers-0.2.7/datawhispers.egg-info/PKG-INFO
+-rw-r--r--   0 german     (501) staff       (20)      284 2023-07-01 16:58:48.000000 datawhispers-0.2.7/datawhispers.egg-info/SOURCES.txt
+-rw-r--r--   0 german     (501) staff       (20)        1 2023-07-01 16:58:48.000000 datawhispers-0.2.7/datawhispers.egg-info/dependency_links.txt
+-rw-r--r--   0 german     (501) staff       (20)       38 2023-07-01 16:58:48.000000 datawhispers-0.2.7/datawhispers.egg-info/requires.txt
+-rw-r--r--   0 german     (501) staff       (20)       13 2023-07-01 16:58:48.000000 datawhispers-0.2.7/datawhispers.egg-info/top_level.txt
+-rw-r--r--   0 german     (501) staff       (20)       38 2023-07-01 16:58:48.038703 datawhispers-0.2.7/setup.cfg
+-rw-r--r--   0 german     (501) staff       (20)     2271 2023-07-01 16:58:42.000000 datawhispers-0.2.7/setup.py
```

### Comparing `datawhispers-0.2.6/LICENSE` & `datawhispers-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `datawhispers-0.2.6/datawhispers/advanced_prog.py` & `datawhispers-0.2.7/datawhispers/advanced_prog.py`

 * *Files identical despite different names*

### Comparing `datawhispers-0.2.6/datawhispers/datavis.py` & `datawhispers-0.2.7/datawhispers/datavis.py`

 * *Files identical despite different names*

### Comparing `datawhispers-0.2.6/setup.py` & `datawhispers-0.2.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from distutils.core import setup
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 setup(
   name = 'datawhispers',         # How you named your package folder (MyLib)
   packages = ["datawhispers"],   # Chose the same as "name"
-  version = '0.2.6',      # Start with a small number and increase it with every change you make
+  version = '0.2.7',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'This is a library to solve regression problems or statistical analysis for the DHBW Mannheim courses Advanced Programming and Data Visualisation',   # Give a short description about your library
   author = 'German Paul',                   # Type in your name
   author_email = 'motets-rosiest-0r@icloud.com',      # Type in your E-Mail
   url = 'https://github.com/GermanPaul12/datawhispers',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/GermanPaul12/datawhispers/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['Python3', 'Data Visualisation', 'Statistical Analysis', "Regression", "Advanced Programming"],   # Keywords that define your package best
@@ -14,14 +17,16 @@
           'pandas',
           'matplotlib',
           'numpy',
           'seaborn',
           'scipy',
           
       ],
+  long_description=long_description,
+  long_description_content_type='text/markdown',
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
     'Programming Language :: Python :: 3.4',
```

