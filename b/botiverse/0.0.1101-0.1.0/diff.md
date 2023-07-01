# Comparing `tmp/botiverse-0.0.1101.tar.gz` & `tmp/botiverse-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botiverse-0.0.1101.tar", last modified: Tue Jan 31 14:38:39 2023, max compression
+gzip compressed data, was "botiverse-0.1.0.tar", last modified: Sat Jul  1 14:09:51 2023, max compression
```

## Comparing `botiverse-0.0.1101.tar` & `botiverse-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-01-31 14:38:39.390851 botiverse-0.0.1101/
--rw-r--r--   0 essam      (501) staff       (20)     1252 2023-01-31 14:38:39.390606 botiverse-0.0.1101/PKG-INFO
--rw-r--r--   0 essam      (501) staff       (20)      437 2023-01-31 14:27:35.000000 botiverse-0.0.1101/README.md
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-01-31 14:38:39.387543 botiverse-0.0.1101/botiverse/
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-01-31 14:38:39.389596 botiverse-0.0.1101/botiverse/TODS/
--rw-r--r--   0 essam      (501) staff       (20)     1057 2023-01-31 12:49:51.000000 botiverse-0.0.1101/botiverse/TODS/TODS.py
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-01-31 14:19:19.000000 botiverse-0.0.1101/botiverse/TODS/__init__.py
--rw-r--r--   0 essam      (501) staff       (20)      101 2023-01-31 13:20:06.000000 botiverse-0.0.1101/botiverse/__init__.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-01-31 14:38:39.390322 botiverse-0.0.1101/botiverse/basic_chatbot/
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-01-31 14:19:10.000000 botiverse-0.0.1101/botiverse/basic_chatbot/__init__.py
--rw-r--r--   0 essam      (501) staff       (20)     1053 2023-01-31 13:18:31.000000 botiverse-0.0.1101/botiverse/basic_chatbot/basic_chatbot.py
--rw-r--r--   0 essam      (501) staff       (20)        0 2023-01-31 12:37:58.000000 botiverse-0.0.1101/botiverse/basic_chatbot/utils.py
-drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-01-31 14:38:39.388982 botiverse-0.0.1101/botiverse.egg-info/
--rw-r--r--   0 essam      (501) staff       (20)     1252 2023-01-31 14:38:38.000000 botiverse-0.0.1101/botiverse.egg-info/PKG-INFO
--rw-r--r--   0 essam      (501) staff       (20)      364 2023-01-31 14:38:39.000000 botiverse-0.0.1101/botiverse.egg-info/SOURCES.txt
--rw-r--r--   0 essam      (501) staff       (20)        1 2023-01-31 14:38:38.000000 botiverse-0.0.1101/botiverse.egg-info/dependency_links.txt
--rw-r--r--   0 essam      (501) staff       (20)       12 2023-01-31 14:38:39.000000 botiverse-0.0.1101/botiverse.egg-info/requires.txt
--rw-r--r--   0 essam      (501) staff       (20)       10 2023-01-31 14:38:39.000000 botiverse-0.0.1101/botiverse.egg-info/top_level.txt
--rw-r--r--   0 essam      (501) staff       (20)       38 2023-01-31 14:38:39.390937 botiverse-0.0.1101/setup.cfg
--rw-r--r--   0 essam      (501) staff       (20)     1751 2023-01-31 14:38:33.000000 botiverse-0.0.1101/setup.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-01 14:09:51.829900 botiverse-0.1.0/
+-rw-r--r--   0 essam      (501) staff       (20)     1192 2023-07-01 14:09:51.829734 botiverse-0.1.0/PKG-INFO
+-rw-r--r--   0 essam      (501) staff       (20)      440 2023-01-31 16:00:25.000000 botiverse-0.1.0/README.md
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-01 14:09:51.826509 botiverse-0.1.0/botiverse/
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-01 14:09:51.828760 botiverse-0.1.0/botiverse/TODS/
+-rw-r--r--   0 essam      (501) staff       (20)      977 2023-07-01 06:07:26.000000 botiverse-0.1.0/botiverse/TODS/DNN_TODS.py
+-rw-r--r--   0 essam      (501) staff       (20)     4080 2023-07-01 06:07:26.000000 botiverse-0.1.0/botiverse/TODS/TODS.py
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-01-31 14:19:19.000000 botiverse-0.1.0/botiverse/TODS/__init__.py
+-rw-r--r--   0 essam      (501) staff       (20)     1345 2023-07-01 06:07:26.000000 botiverse-0.1.0/botiverse/TODS/tods_example.py
+-rw-r--r--   0 essam      (501) staff       (20)     7362 2023-07-01 06:07:26.000000 botiverse-0.1.0/botiverse/TODS/utils.py
+-rw-r--r--   0 essam      (501) staff       (20)      762 2023-07-01 06:07:26.000000 botiverse-0.1.0/botiverse/TODS/utils2.py
+-rw-r--r--   0 essam      (501) staff       (20)      241 2023-07-01 10:10:18.000000 botiverse-0.1.0/botiverse/__init__.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-01 14:09:51.829485 botiverse-0.1.0/botiverse/basic_chatbot/
+-rw-r--r--   0 essam      (501) staff       (20)        0 2023-01-31 14:19:10.000000 botiverse-0.1.0/botiverse/basic_chatbot/__init__.py
+-rw-r--r--   0 essam      (501) staff       (20)     1099 2023-02-06 15:33:14.000000 botiverse-0.1.0/botiverse/basic_chatbot/basic_chatbot.py
+-rw-r--r--   0 essam      (501) staff       (20)       35 2023-02-06 15:31:49.000000 botiverse-0.1.0/botiverse/basic_chatbot/utils.py
+drwxr-xr-x   0 essam      (501) staff       (20)        0 2023-07-01 14:09:51.827394 botiverse-0.1.0/botiverse.egg-info/
+-rw-r--r--   0 essam      (501) staff       (20)     1192 2023-07-01 14:09:51.000000 botiverse-0.1.0/botiverse.egg-info/PKG-INFO
+-rw-r--r--   0 essam      (501) staff       (20)      471 2023-07-01 14:09:51.000000 botiverse-0.1.0/botiverse.egg-info/SOURCES.txt
+-rw-r--r--   0 essam      (501) staff       (20)        1 2023-07-01 14:09:51.000000 botiverse-0.1.0/botiverse.egg-info/dependency_links.txt
+-rw-r--r--   0 essam      (501) staff       (20)       12 2023-07-01 14:09:51.000000 botiverse-0.1.0/botiverse.egg-info/requires.txt
+-rw-r--r--   0 essam      (501) staff       (20)       10 2023-07-01 14:09:51.000000 botiverse-0.1.0/botiverse.egg-info/top_level.txt
+-rw-r--r--   0 essam      (501) staff       (20)       38 2023-07-01 14:09:51.829951 botiverse-0.1.0/setup.cfg
+-rw-r--r--   0 essam      (501) staff       (20)     1958 2023-07-01 14:07:32.000000 botiverse-0.1.0/setup.py
```

### Comparing `botiverse-0.0.1101/PKG-INFO` & `botiverse-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: botiverse
-Version: 0.0.1101
-Summary: botiverse is a chatbot library that offers a high-level API to access a diverse set of chatbot models.
+Version: 0.1.0
+Summary: botiverse is a chatbot library that offers a high-level API to
 Home-page: https://botiverse.readthedocs.io/
 Author: Essam W., Mohamed Saad, Yousef Atef, Karim Taha
 Author-email: essamwisam@outlook.com
 License: GPLv3
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -30,15 +29,16 @@
 Try to import and playaround with the Basic Chat Bot:
 
 ```Python
 from botiverse import basic_chatbot
 
 # Make a new chatbot and give it a name
 Max = basic_chatbot("Max")
+
 # Train the chatbot
 Max.train("abcdefgh")
+
 # Ask the chatbot a question
 response = Max.infer("Can you tell me a joke?")
+
 print(response)
 ```
-
-
```

### Comparing `botiverse-0.0.1101/botiverse/TODS/TODS.py` & `botiverse-0.1.0/botiverse/basic_chatbot/basic_chatbot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
-import torch
+from botiverse.basic_chatbot.utils import meh
 
-class TODS:
+class basic_chatbot:
     """
     Instantiate a basic chat bot model that uses a classic feedforward neural network.
     Data can be then used to train the chatbot model.
     
     :param name: The chatbot's name.
     :type name: string
     """
```

### Comparing `botiverse-0.0.1101/botiverse.egg-info/PKG-INFO` & `botiverse-0.1.0/botiverse.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: botiverse
-Version: 0.0.1101
-Summary: botiverse is a chatbot library that offers a high-level API to access a diverse set of chatbot models.
+Version: 0.1.0
+Summary: botiverse is a chatbot library that offers a high-level API to
 Home-page: https://botiverse.readthedocs.io/
 Author: Essam W., Mohamed Saad, Yousef Atef, Karim Taha
 Author-email: essamwisam@outlook.com
 License: GPLv3
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -30,15 +29,16 @@
 Try to import and playaround with the Basic Chat Bot:
 
 ```Python
 from botiverse import basic_chatbot
 
 # Make a new chatbot and give it a name
 Max = basic_chatbot("Max")
+
 # Train the chatbot
 Max.train("abcdefgh")
+
 # Ask the chatbot a question
 response = Max.infer("Can you tell me a joke?")
+
 print(response)
 ```
-
-
```

### Comparing `botiverse-0.0.1101/setup.py` & `botiverse-0.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,33 @@
-# Any library uses this setup.py file:
-
-# Always prefer setuptools over distutils
-from setuptools import setup, find_packages
+"""
+This file is used to build the package and upload it to PyPI
+"""
+# pylint: skip-file  (PyLint is not happy with importing the already built-in open)
+from os import path
 
 # To use a consistent encoding
 from codecs import open
-from os import path
+
+# Always prefer setuptools over distutils
+from setuptools import setup
+
 
 # The directory containing this file
 HERE = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     readme = f.read()
 
 # This call to setup() does all the work
 setup(
     name="botiverse",
-    version="0.0.1101",
-    description="botiverse is a chatbot library that offers a high-level API to access a diverse set of chatbot models.",
+    version="0.1.0",
+    description='''botiverse is a chatbot library that offers a high-level API to
+    access a diverse set of chatbot models''',
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://botiverse.readthedocs.io/",
     author="Essam W., Mohamed Saad, Yousef Atef, Karim Taha",
     author_email="essamwisam@outlook.com",
     license="GPLv3",
     classifiers=[                               # https://pypi.org/classifiers/
@@ -38,9 +43,14 @@
     ],
     packages=["botiverse", "botiverse.basic_chatbot", "botiverse.TODS"],
     include_package_data=True,
     install_requires=["numpy", "torch"]            # just as was in requirements.txt
 )
 
 
-# TODO: upload to test PyPI by running: twine upload --repository-url https://test.pypi.org/legacy/ dist/*
-# DONE: upload to PyPI by running: twine upload dist/*
+# Steps to upload to PyPI
+# 0 - Increment the version number in setup.py
+# 1 - Remove the dist folder
+# 2- python3 setup.py sdist bdist_wheel  
+# 3 - twine upload dist/*
+
+# To upload to test PyPI: twine upload --repository-url https://test.pypi.org/legacy/ dist/*
```

