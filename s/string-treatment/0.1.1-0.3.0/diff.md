# Comparing `tmp/string_treatment-0.1.1.tar.gz` & `tmp/string_treatment-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "string_treatment-0.1.1.tar", last modified: Fri Jun 30 15:52:01 2023, max compression
+gzip compressed data, was "string_treatment-0.3.0.tar", last modified: Sat Jul  1 00:04:28 2023, max compression
```

## Comparing `string_treatment-0.1.1.tar` & `string_treatment-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 15:52:01.778163 string_treatment-0.1.1/
--rw-rw-rw-   0        0        0      478 2023-06-30 15:52:01.774645 string_treatment-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1042 2023-06-30 15:26:14.000000 string_treatment-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-30 15:52:01.778678 string_treatment-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      881 2023-06-30 15:51:50.000000 string_treatment-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 15:52:01.768055 string_treatment-0.1.1/string_treatment.egg-info/
--rw-rw-rw-   0        0        0      478 2023-06-30 15:52:01.000000 string_treatment-0.1.1/string_treatment.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-30 15:52:01.000000 string_treatment-0.1.1/string_treatment.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 15:52:01.000000 string_treatment-0.1.1/string_treatment.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-30 15:52:01.000000 string_treatment-0.1.1/string_treatment.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 15:52:01.000000 string_treatment-0.1.1/string_treatment.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4111 2023-06-30 15:37:14.000000 string_treatment-0.1.1/string_treatment.py
+drwxrwxrwx   0        0        0        0 2023-07-01 00:04:28.200965 string_treatment-0.3.0/
+-rw-rw-rw-   0        0        0     1091 2023-06-30 17:16:02.000000 string_treatment-0.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      539 2023-07-01 00:04:28.202998 string_treatment-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1086 2023-07-01 00:02:37.000000 string_treatment-0.3.0/README.md
+-rw-rw-rw-   0        0        0      169 2023-06-30 16:32:03.000000 string_treatment-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0      651 2023-07-01 00:04:28.207284 string_treatment-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-01 00:04:28.093943 string_treatment-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-01 00:04:28.141130 string_treatment-0.3.0/src/string_treatment/
+-rw-rw-rw-   0        0        0        0 2023-06-30 16:48:39.000000 string_treatment-0.3.0/src/string_treatment/__init__.py
+-rw-rw-rw-   0        0        0     3472 2023-07-01 00:00:50.000000 string_treatment-0.3.0/src/string_treatment/string_treatment.py
+drwxrwxrwx   0        0        0        0 2023-07-01 00:04:28.196240 string_treatment-0.3.0/src/string_treatment.egg-info/
+-rw-rw-rw-   0        0        0      539 2023-07-01 00:04:28.000000 string_treatment-0.3.0/src/string_treatment.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-07-01 00:04:28.000000 string_treatment-0.3.0/src/string_treatment.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 00:04:28.000000 string_treatment-0.3.0/src/string_treatment.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-01 00:04:28.000000 string_treatment-0.3.0/src/string_treatment.egg-info/top_level.txt
```

### Comparing `string_treatment-0.1.1/README.md` & `string_treatment-0.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 ```shell
 pip install string-treatment
 ```
 
 # Quick start
 #### With reference list
 ``` python
->>> import string_treatment as st
+>>> from string_treatment import string_treatment as st
 >>> list_of_reference = ['João Pessoa/PB']
 >>> data_with_inconsistency = ['João Pessoa PB', 'Joao pessoa--PB', 'joa pssoa(pb)']
 >>> st.treat_referenced(data_with_inconsistency, list_of_reference)
 ['João Pessoa PB', 'João Pessoa PB', 'João Pessoa PB']
 ```
 
 #### Without reference list
 ``` python
->>> import string_treatment as st
+>>> from string_treatment import string_treatment as st
 >>> data_with_inconsistency = ['João Pessoa PB', 'Joao pessoa--PB', 'joa pssoa(pb)']
 >>> st.treat_unreferenced(data_with_inconsistency)
 ['João Pessoa PB', 'João Pessoa PB', 'João Pessoa PB']
 ```
 
 # Usage
 To learn about how to use this library and examples,
```

