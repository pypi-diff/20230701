# Comparing `tmp/lvm_read-1.20.tar.gz` & `tmp/lvm_read-1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\lvm_read-1.20.tar", last modified: Sun Nov 29 07:10:35 2020, max compression
+gzip compressed data, was "lvm_read-1.21.tar", last modified: Sat Jul  1 05:22:08 2023, max compression
```

## Comparing `lvm_read-1.20.tar` & `lvm_read-1.21.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2020-11-29 07:10:35.462014 lvm_read-1.20/
--rw-rw-rw-   0        0        0      568 2020-11-29 07:10:35.462014 lvm_read-1.20/PKG-INFO
-drwxrwxrwx   0        0        0        0 2020-11-29 07:10:35.460020 lvm_read-1.20/lvm_read.egg-info/
--rw-rw-rw-   0        0        0      568 2020-11-29 07:10:35.000000 lvm_read-1.20/lvm_read.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      179 2020-11-29 07:10:35.000000 lvm_read-1.20/lvm_read.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-11-29 07:10:35.000000 lvm_read-1.20/lvm_read.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2020-11-29 07:10:35.000000 lvm_read-1.20/lvm_read.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2020-11-29 07:10:35.000000 lvm_read-1.20/lvm_read.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7795 2020-11-29 07:07:48.000000 lvm_read-1.20/lvm_read.py
--rw-rw-rw-   0        0        0       42 2020-11-29 07:10:35.462014 lvm_read-1.20/setup.cfg
--rw-rw-rw-   0        0        0     1494 2020-11-29 07:07:37.000000 lvm_read-1.20/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 05:22:08.727992 lvm_read-1.21/
+-rw-rw-rw-   0        0        0     1091 2023-07-01 04:57:49.000000 lvm_read-1.21/LICENSE
+-rw-rw-rw-   0        0        0      520 2023-07-01 05:22:08.727992 lvm_read-1.21/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-01 05:22:08.727992 lvm_read-1.21/lvm_read.egg-info/
+-rw-rw-rw-   0        0        0      520 2023-07-01 05:22:08.000000 lvm_read-1.21/lvm_read.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-07-01 05:22:08.000000 lvm_read-1.21/lvm_read.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 05:22:08.000000 lvm_read-1.21/lvm_read.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-01 05:22:08.000000 lvm_read-1.21/lvm_read.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-01 05:22:08.000000 lvm_read-1.21/lvm_read.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6816 2023-07-01 05:13:12.000000 lvm_read-1.21/lvm_read.py
+-rw-rw-rw-   0        0        0       42 2023-07-01 05:22:08.727992 lvm_read-1.21/setup.cfg
+-rw-rw-rw-   0        0        0      724 2023-07-01 05:21:06.000000 lvm_read-1.21/setup.py
```

### Comparing `lvm_read-1.20/lvm_read.py` & `lvm_read-1.21/lvm_read.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,17 @@
-# -*- coding: utf-8 -*-
-
-# Copyright (C) 2014-2017 Matjaž Mršnik, Miha Pirnat, Janko Slavič, Blaž Starc (in alphabetic order)
-#
-# This file is part of lvm_read.
-#
-# lvm_read is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, version 3 of the License.
-#
-# lvm_read is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with lvm_read.  If not, see <http://www.gnu.org/licenses/>.
-
-
-
 """
-This module is part of the www.openmodal.com project and is used for the 
-reading LabView Measurement File
+This module is used for the reading LabView Measurement File
 
 Author: Janko Slavič et al. (janko.slavic@fs.uni-lj.si)
 """
 from os import path
 import pickle
 import numpy as np
 
-__version__ = '1.20'
+__version__ = '1.21'
 
 def _lvm_pickle(filename):
     """ Reads pickle file (for local use)
 
     :param filename: filename of lvm file
     :return lvm_data: dict with lvm data
     """
@@ -82,14 +61,15 @@
     :return lvm_data: lvm dict
     """
     lvm_data = dict()
     lvm_data['Decimal_Separator'] = '.'
     data_channels_comment_reading = False
     data_reading = False
     segment = None
+    seg_data = []
     first_column = 0
     nr_of_columns = 0
     segment_nr = 0
     def to_float(a):
         try:
             return float(a.replace(lvm_data['Decimal_Separator'], '.'))
         except:
@@ -157,42 +137,39 @@
     :return:      dictionary with lvm data
 
     Examples
     --------
     >>> import numpy as np
     >>> import urllib
     >>> filename = 'short.lvm' #download a sample file from github
-    >>> sample_file = urllib.request.urlopen('https://raw.githubusercontent.com/openmodal/lvm_read/master/data/'+filename).read()
+    >>> sample_file = urllib.request.urlopen('https://github.com/ladisk/lvm_read/blob/master/data/'+filename).read()
     >>> str = sample_file.decode('utf-8') # convert to string
     >>> lvm = lvm_read.read_str(str) #read the string as lvm file content
     >>> lvm.keys() #explore the dictionary
     dict_keys(['', 'Date', 'X_Columns', 'Time_Pref', 'Time', 'Writer_Version',...
     """
     return read_lines(str.splitlines(keepends=True))
 
 
 def read(filename, read_from_pickle=True, dump_file=True):
     """Read from .lvm file and by default for faster reading save to pickle.
 
-    This module is part of the www.openmodal.com project
-
-    For a showcase see: https://github.com/openmodal/lvm_read/blob/master/Showcase%20lvm_read.ipynb
     See also specifications: http://www.ni.com/tutorial/4139/en/
 
     :param filename:            file which should be read
     :param read_from_pickle:    if True, it tries to read from pickle
     :param dump_file:           dump file to pickle (significantly increases performance)
     :return:                    dictionary with lvm data
 
     Examples
     --------
     >>> import numpy as np
     >>> import urllib
     >>> filename = 'short.lvm' #download a sample file from github
-    >>> sample_file = urllib.request.urlopen('https://raw.githubusercontent.com/openmodal/lvm_read/master/data/'+filename).read()
+    >>> sample_file = urllib.request.urlopen('https://github.com/ladisk/lvm_read/blob/master/data/'+filename).read()
     >>> with open(filename, 'wb') as f: # save the file locally
             f.write(sample_file)
     >>> lvm = lvm_read.read('short.lvm') #read the file
     >>> lvm.keys() #explore the dictionary
     dict_keys(['', 'Date', 'X_Columns', 'Time_Pref', 'Time', 'Writer_Version',...
     """
     lvm_data = _lvm_pickle(filename)
```

