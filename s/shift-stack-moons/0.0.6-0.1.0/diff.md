# Comparing `tmp/shift_stack_moons-0.0.6.tar.gz` & `tmp/shift_stack_moons-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shift_stack_moons-0.0.6.tar", last modified: Mon Feb  6 02:35:03 2023, max compression
+gzip compressed data, was "shift_stack_moons-0.1.0.tar", last modified: Sat Jul  1 03:37:57 2023, max compression
```

## Comparing `shift_stack_moons-0.0.6.tar` & `shift_stack_moons-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxr-xr-x   0 emolter    (501) staff       (20)        0 2023-02-06 02:35:03.659556 shift_stack_moons-0.0.6/
--rw-r--r--   0 emolter    (501) staff       (20)     1500 2022-02-11 20:32:50.000000 shift_stack_moons-0.0.6/LICENSE.txt
--rw-r--r--   0 emolter    (501) staff       (20)     1097 2023-02-06 02:35:03.659609 shift_stack_moons-0.0.6/PKG-INFO
--rw-r--r--   0 emolter    (501) staff       (20)     2069 2023-02-06 02:31:17.000000 shift_stack_moons-0.0.6/README.md
--rw-r--r--   0 emolter    (501) staff       (20)     2053 2022-04-07 00:51:29.000000 shift_stack_moons-0.0.6/image.py
--rw-r--r--   0 emolter    (501) staff       (20)       98 2023-02-06 02:35:03.659834 shift_stack_moons-0.0.6/setup.cfg
--rwxr-xr-x   0 emolter    (501) staff       (20)     1381 2023-02-06 02:34:30.000000 shift_stack_moons-0.0.6/setup.py
-drwxr-xr-x   0 emolter    (501) staff       (20)        0 2023-02-06 02:35:03.659471 shift_stack_moons-0.0.6/shift_stack_moons.egg-info/
--rw-r--r--   0 emolter    (501) staff       (20)     1097 2023-02-06 02:35:03.000000 shift_stack_moons-0.0.6/shift_stack_moons.egg-info/PKG-INFO
--rw-r--r--   0 emolter    (501) staff       (20)      234 2023-02-06 02:35:03.000000 shift_stack_moons-0.0.6/shift_stack_moons.egg-info/SOURCES.txt
--rw-r--r--   0 emolter    (501) staff       (20)        1 2023-02-06 02:35:03.000000 shift_stack_moons-0.0.6/shift_stack_moons.egg-info/dependency_links.txt
--rw-r--r--   0 emolter    (501) staff       (20)       24 2023-02-06 02:35:03.000000 shift_stack_moons-0.0.6/shift_stack_moons.egg-info/top_level.txt
--rwxr-xr-x   0 emolter    (501) staff       (20)    10578 2023-02-06 02:27:04.000000 shift_stack_moons-0.0.6/shift_stack_moons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 03:37:57.431966 shift_stack_moons-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-01 03:37:46.000000 shift_stack_moons-0.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-01 03:37:57.431966 shift_stack_moons-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-01 03:37:46.000000 shift_stack_moons-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 03:37:57.431966 shift_stack_moons-0.1.0/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 03:37:46.000000 shift_stack_moons-0.1.0/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-01 03:37:57.431966 shift_stack_moons-0.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1316 2023-07-01 03:37:46.000000 shift_stack_moons-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 03:37:57.431966 shift_stack_moons-0.1.0/shift_stack_moons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-01 03:37:57.000000 shift_stack_moons-0.1.0/shift_stack_moons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-01 03:37:57.000000 shift_stack_moons-0.1.0/shift_stack_moons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 03:37:57.000000 shift_stack_moons-0.1.0/shift_stack_moons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-01 03:37:57.000000 shift_stack_moons-0.1.0/shift_stack_moons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 03:37:57.431966 shift_stack_moons-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 03:37:46.000000 shift_stack_moons-0.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 03:37:57.431966 shift_stack_moons-0.1.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 03:37:46.000000 shift_stack_moons-0.1.0/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-01 03:37:46.000000 shift_stack_moons-0.1.0/tests/test_shift_and_stack.py
```

### Comparing `shift_stack_moons-0.0.6/LICENSE.txt` & `shift_stack_moons-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shift_stack_moons-0.0.6/PKG-INFO` & `shift_stack_moons-0.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: shift_stack_moons
-Version: 0.0.6
-Summary: Find small moons around planets using shift-and-stack based on JPL Horizons ephemeris
+Version: 0.1.0
+Summary: Find small moons around planets     using shift-and-stack based on JPL Horizons ephemeris
 Home-page: https://github.com/emolter/shift_stack_moons
 Author: Ned Molter
 Author-email: emolter@berkeley.edu
 License: BSD
 Keywords: planetary astronomy moons jpl ephemeris
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
-Find small moons around planets using shift-and-stack based on JPL Horizons ephemeris
+Find small moons around planets     using shift-and-stack based on JPL Horizons ephemeris
```

### Comparing `shift_stack_moons-0.0.6/README.md` & `shift_stack_moons-0.1.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,38 @@
-# installation
+[![DOI](https://zenodo.org/badge/415108491.svg)](https://zenodo.org/badge/latestdoi/415108491)
+[![codecov.io Code Coverage](https://codecov.io/gh/emolter/shift_stack_moons/branch/main/graph/badge.svg)](https://codecov.io/gh/emolter/shift_stack_moons)
 
-Use `pip install shift_stack_moons` to install. Tested in Python 3.9 but might work on other versions.
+# Installation
 
-# description
-find small moons around planets using shift-and-stack based on JPL Horizons ephemeris, save as fits
+1. Ensure Python version in your environment is >=3.7
+2. pip install -r requirements.txt
+3. pip install shift-stack-moons
 
-At present, Keck NIRC2 fits header keywords are hard-coded in. 
+# Usage
+
+See `example-run.ipynb`
+
+# Description
+Increase signal-to-noise ratio on small moons around planets in multi-frame observations according to the expected position of the moon from JPL Horizons.
 
 ![alt text](https://github.com/emolter/shift_stack_moons/blob/main/despina_pretty_picture.jpeg?raw=true)
 
-This image shows the utility of the software. Thirty images of Neptune from Keck's NIRC2 instrument, each separated by 1-2 minutes, have been shifted according to the orbit of Despina to increase the signal-to-noise of that moon.  Despina appears as a point source, whereas all the other labeled moonlets appear as streaks. If you look closely you can see the individual images that make up Proteus's streak. Neptune is a streak, too, but it's so overexposed you can't tell. The sidelobes of the PSF can be seen on Despina. I compared this stacked PSF to a calibration star PSF and the match is pretty close, so the shift-and-stack is quite accurate.
+This image shows the utility of the software. Thirty images of Neptune from Keck's NIRC2 instrument, each separated by 1-2 minutes, have been shifted according to the orbit of Despina to increase the signal-to-noise of that moon.  Despina appears as a point source, whereas all the other labeled moonlets appear as streaks. If you look closely, you can see the individual images that make up Proteus's streak. Neptune is a streak, too, but it's so overexposed you can't tell. The sidelobes of the PSF can be seen on Despina. I compared this stacked PSF to a calibration star PSF and the match is pretty close, so the shift-and-stack is quite accurate.
+
+# Caveats
+shift_and_stack.py scrapes the FITS header of input images for relevant information like the rotator angle, instrument angle, observation date and time, integration time, etc. The keywords are included in a .yaml file (data/kw\_instrument.yaml) to (in theory) support ease-of-use for different fits header conventions.  
 
-# usage
-command-line application: "python shift_and_stack.py -h" for help
+However, this has only been tested for Keck's NIRC2 instrument. If you are using any instrument other than Keck NIRC2, you will need to make a .yaml file for your instrument.
 
-as a Python import: the preferred method. see the docstring of shift\_stack\_moons
+# Dependencies
+See requirements.txt.
 
-# caveats
-shift_and_stack.py scrapes the FITS header of input images for the following keywords: ROTPOSN, DATE-OBS, EXPSTART, NAXIS1, NAXIS2, ITIME, COADDS
-if you are using any instrument other than Keck NIRC2, you will likely need to replace these hard-coded keywords.
-I plan to make this more generic eventually, but I'm paid to do science, not code. If you want to help out, make a pull request!
+Note that the most recent (officially unreleased) version of Astropy-affiliated package image\_registration is required, so it is installed directly from the GitHub page instead of from pypi.
 
-# dependencies
-requires the Astropy-affiliated package image\_registration: https://pypi.org/project/image_registration/
+The other dependencies should be included with a usual Python Anaconda install.
 
-all other dependencies should be included with a usual Python Anaconda release
+# Contributing
 
-# how to cite
-if you use this for research, please cite it in some way.  I'm no expert on how to do this right, but there are plenty of resources, e.g.: https://journals.aas.org/news/software-citation-suggestions/
+I welcome contributions! Please submit an issue first, explaining what you'd like to change/add.  I'll comment on that, and then you can submit a PR when your improvement/addition is ready!
 
-written by Ned Molter 2021-Oct-08.
+# Cite
+If you use this for research, please cite it using the DOI above. Please also cite Molter et al. 2023 (in review)
```

### Comparing `shift_stack_moons-0.0.6/setup.py` & `shift_stack_moons-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 #!/usr/bin/env python
 
-import sys
 from setuptools import setup, find_packages
 
-VERSION = '0.0.6'
-DESCRIPTION = "Find small moons around planets using shift-and-stack based on JPL Horizons ephemeris"
+VERSION = '0.1.0'
+DESCRIPTION = "Find small moons around planets \
+    using shift-and-stack based on JPL Horizons ephemeris"
 
 CLASSIFIERS = list(filter(None, map(str.strip,
-"""
+                                    """
 Development Status :: 3 - Alpha
 Intended Audience :: Science/Research
 License :: OSI Approved :: BSD License
 Programming Language :: Python
-Programming Language :: Python :: 3.5
 Programming Language :: Python :: 3.6
 Programming Language :: Python :: 3.7
 Programming Language :: Python :: 3.8
 Programming Language :: Python :: 3.9
-Programming Language :: Python :: Implementation :: CPython
+Programming Language :: Python :: 3.10
+Programming Language :: Python :: 3.11
 Topic :: Software Development :: Libraries :: Python Modules
 """.splitlines())))
 
 setup(
-        name="shift_stack_moons",
-        version=VERSION,
-        description=DESCRIPTION,
-        long_description=DESCRIPTION,
-        long_description_content_type="text/x-rst",
-        classifiers=CLASSIFIERS,
-        author="Ned Molter",
-        author_email="emolter@berkeley.edu",
-        url="https://github.com/emolter/shift_stack_moons",
-        python_requires='>=3',
-        license="BSD",
-        keywords='planetary astronomy moons jpl ephemeris',
-        packages=find_packages(),
-        py_modules=['shift_stack_moons', 'image'],
-        platforms=['any'],
-        setup_requires=['pytest-runner'],
-        tests_require=['pytest']
-)
+    name="shift_stack_moons",
+    version=VERSION,
+    description=DESCRIPTION,
+    long_description=DESCRIPTION,
+    long_description_content_type="text/x-rst",
+    classifiers=CLASSIFIERS,
+    author="Ned Molter",
+    author_email="emolter@berkeley.edu",
+    url="https://github.com/emolter/shift_stack_moons",
+    python_requires='>=3',
+    license="BSD",
+    keywords='planetary astronomy moons jpl ephemeris',
+    packages=find_packages(),
+    py_modules=['shift_stack_moons'],
+    platforms=['any'],
+    setup_requires=['pytest-runner'],
+    tests_require=['pytest']
+)
```

### Comparing `shift_stack_moons-0.0.6/shift_stack_moons.egg-info/PKG-INFO` & `shift_stack_moons-0.1.0/shift_stack_moons.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: shift-stack-moons
-Version: 0.0.6
-Summary: Find small moons around planets using shift-and-stack based on JPL Horizons ephemeris
+Version: 0.1.0
+Summary: Find small moons around planets     using shift-and-stack based on JPL Horizons ephemeris
 Home-page: https://github.com/emolter/shift_stack_moons
 Author: Ned Molter
 Author-email: emolter@berkeley.edu
 License: BSD
 Keywords: planetary astronomy moons jpl ephemeris
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
-Find small moons around planets using shift-and-stack based on JPL Horizons ephemeris
+Find small moons around planets     using shift-and-stack based on JPL Horizons ephemeris
```

