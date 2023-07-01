# Comparing `tmp/enigmacrypt-0.0.4.tar.gz` & `tmp/enigmacrypt-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enigmacrypt-0.0.4.tar", last modified: Fri Jun 30 20:35:53 2023, max compression
+gzip compressed data, was "enigmacrypt-0.0.5.tar", last modified: Sat Jul  1 21:39:58 2023, max compression
```

## Comparing `enigmacrypt-0.0.4.tar` & `enigmacrypt-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 20:35:53.879362 enigmacrypt-0.0.4/
--rw-rw-rw-   0        0        0     1096 2023-06-29 20:42:14.000000 enigmacrypt-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     2511 2023-06-30 20:35:53.879362 enigmacrypt-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1771 2023-06-29 20:42:14.000000 enigmacrypt-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 20:35:53.870651 enigmacrypt-0.0.4/app/
--rw-rw-rw-   0        0        0       23 2023-06-30 20:35:52.000000 enigmacrypt-0.0.4/app/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 20:35:53.872157 enigmacrypt-0.0.4/app/enigmacrypt/
--rw-rw-rw-   0        0        0      119 2023-06-30 18:25:58.000000 enigmacrypt-0.0.4/app/enigmacrypt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 20:35:53.878328 enigmacrypt-0.0.4/enigmacrypt.egg-info/
--rw-rw-rw-   0        0        0     2511 2023-06-30 20:35:53.000000 enigmacrypt-0.0.4/enigmacrypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-06-30 20:35:53.000000 enigmacrypt-0.0.4/enigmacrypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 20:35:53.000000 enigmacrypt-0.0.4/enigmacrypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-30 20:35:53.000000 enigmacrypt-0.0.4/enigmacrypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-30 20:35:53.000000 enigmacrypt-0.0.4/enigmacrypt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 20:35:53.879362 enigmacrypt-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1128 2023-06-30 20:35:52.000000 enigmacrypt-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 21:39:58.078067 enigmacrypt-0.0.5/
+-rw-rw-rw-   0        0        0     1096 2023-06-29 20:42:16.000000 enigmacrypt-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2530 2023-07-01 21:39:58.076076 enigmacrypt-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1771 2023-06-29 20:42:16.000000 enigmacrypt-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 21:39:58.058122 enigmacrypt-0.0.5/app/
+-rw-rw-rw-   0        0        0       23 2023-07-01 21:39:56.000000 enigmacrypt-0.0.5/app/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 21:39:58.061112 enigmacrypt-0.0.5/app/enigmacrypt/
+-rw-rw-rw-   0        0        0      119 2023-06-30 18:26:00.000000 enigmacrypt-0.0.5/app/enigmacrypt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 21:39:58.074079 enigmacrypt-0.0.5/enigmacrypt.egg-info/
+-rw-rw-rw-   0        0        0     2530 2023-07-01 21:39:57.000000 enigmacrypt-0.0.5/enigmacrypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-07-01 21:39:57.000000 enigmacrypt-0.0.5/enigmacrypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 21:39:57.000000 enigmacrypt-0.0.5/enigmacrypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-01 21:39:57.000000 enigmacrypt-0.0.5/enigmacrypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-01 21:39:57.000000 enigmacrypt-0.0.5/enigmacrypt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 21:39:58.078067 enigmacrypt-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1124 2023-07-01 21:39:56.000000 enigmacrypt-0.0.5/setup.py
```

### Comparing `enigmacrypt-0.0.4/LICENSE` & `enigmacrypt-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `enigmacrypt-0.0.4/PKG-INFO` & `enigmacrypt-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: enigmacrypt
-Version: 0.0.4
+Version: 0.0.5
 Summary: Encoding and decoding strings using keys
 Home-page: https://github.com/Wooks08/EnigmaCrypt
 Author: WooksCode (Wojciech Karwowski)
 Author-email: <wookscode.kontakt@gmail.com>
 License: MIT
 Keywords: python,encode,decode,decoder,encoder,string encryption,string decryption
-Classifier: Development Status :: 2 - Pre-Alpha
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.07
 Description-Content-Type: text/markdown
@@ -57,7 +58,9 @@
 If you have any questions or need support, you can reach out to the project maintainer at wookscode.kontakt@gmail.com.
 
 ## Acknowledgments
 EnigmaCrypt works by shuffling the alphabet and digits in random order and then generating quite complex key to show crucial information for decryption process
 
 ## Disclaimer
 Please note that EnigmaCrypt is provided as-is and is not responsible for any security breaches or issues that may arise from its usage. It is always recommended to use additional security measures and best practices when handling sensitive information.
+
+
```

### Comparing `enigmacrypt-0.0.4/README.md` & `enigmacrypt-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `enigmacrypt-0.0.4/enigmacrypt.egg-info/PKG-INFO` & `enigmacrypt-0.0.5/enigmacrypt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: enigmacrypt
-Version: 0.0.4
+Version: 0.0.5
 Summary: Encoding and decoding strings using keys
 Home-page: https://github.com/Wooks08/EnigmaCrypt
 Author: WooksCode (Wojciech Karwowski)
 Author-email: <wookscode.kontakt@gmail.com>
 License: MIT
 Keywords: python,encode,decode,decoder,encoder,string encryption,string decryption
-Classifier: Development Status :: 2 - Pre-Alpha
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.07
 Description-Content-Type: text/markdown
@@ -57,7 +58,9 @@
 If you have any questions or need support, you can reach out to the project maintainer at wookscode.kontakt@gmail.com.
 
 ## Acknowledgments
 EnigmaCrypt works by shuffling the alphabet and digits in random order and then generating quite complex key to show crucial information for decryption process
 
 ## Disclaimer
 Please note that EnigmaCrypt is provided as-is and is not responsible for any security breaches or issues that may arise from its usage. It is always recommended to use additional security measures and best practices when handling sensitive information.
+
+
```

### Comparing `enigmacrypt-0.0.4/setup.py` & `enigmacrypt-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", 'r') as f:
     LONG_DESCRIPTION = f.read()
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Encoding and decoding strings using keys'
 
 # Setting up
 setup(
     name="enigmacrypt",
     version=VERSION,
     author="WooksCode (Wojciech Karwowski)",
@@ -21,15 +21,15 @@
     python_requires=">=3.07",
     extras_require={
         "dev": ["pytest>=7.0", "twine>=4.0.2"]
     },
     keywords=['python', 'encode', 'decode', 'decoder',
               'encoder', 'string encryption', 'string decryption'],
     classifiers=[
-        "Development Status :: 2 - Pre-Alpha",
+        "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
 )
```

