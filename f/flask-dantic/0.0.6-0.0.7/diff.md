# Comparing `tmp/flask-dantic-0.0.6.tar.gz` & `tmp/flask-dantic-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-dantic-0.0.6.tar", last modified: Thu Aug 11 08:43:01 2022, max compression
+gzip compressed data, was "flask-dantic-0.0.7.tar", last modified: Sat Jul  1 19:45:14 2023, max compression
```

## Comparing `flask-dantic-0.0.6.tar` & `flask-dantic-0.0.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 seneca    (1000) seneca    (1000)        0 2022-08-11 08:43:01.160313 flask-dantic-0.0.6/
--rw-rw-r--   0 seneca    (1000) seneca    (1000)       28 2022-06-23 11:36:35.000000 flask-dantic-0.0.6/MANIFEST.in
--rw-rw-r--   0 seneca    (1000) seneca    (1000)    10165 2022-08-11 08:43:01.160313 flask-dantic-0.0.6/PKG-INFO
--rw-rw-r--   0 seneca    (1000) seneca    (1000)     6982 2022-07-02 20:13:01.000000 flask-dantic-0.0.6/README.md
-drwxrwxr-x   0 seneca    (1000) seneca    (1000)        0 2022-08-11 08:43:01.156313 flask-dantic-0.0.6/flask_dantic/
--rw-rw-r--   0 seneca    (1000) seneca    (1000)        5 2022-08-11 08:40:49.000000 flask-dantic-0.0.6/flask_dantic/VERSION
--rw-rw-r--   0 seneca    (1000) seneca    (1000)      320 2022-06-23 15:18:59.000000 flask-dantic-0.0.6/flask_dantic/__init__.py
-drwxrwxr-x   0 seneca    (1000) seneca    (1000)        0 2022-08-11 08:43:01.156313 flask-dantic-0.0.6/flask_dantic/pydantic_serializer/
--rw-rw-r--   0 seneca    (1000) seneca    (1000)      157 2022-06-23 11:57:04.000000 flask-dantic-0.0.6/flask_dantic/pydantic_serializer/__init__.py
--rw-rw-r--   0 seneca    (1000) seneca    (1000)     5474 2022-06-21 23:00:02.000000 flask-dantic-0.0.6/flask_dantic/pydantic_serializer/encoders.py
--rw-rw-r--   0 seneca    (1000) seneca    (1000)     2233 2022-08-11 08:36:25.000000 flask-dantic-0.0.6/flask_dantic/pydantic_serializer/serializer.py
-drwxrwxr-x   0 seneca    (1000) seneca    (1000)        0 2022-08-11 08:43:01.156313 flask-dantic-0.0.6/flask_dantic/request_validator/
--rw-rw-r--   0 seneca    (1000) seneca    (1000)       72 2022-06-23 15:18:38.000000 flask-dantic-0.0.6/flask_dantic/request_validator/__init__.py
--rw-rw-r--   0 seneca    (1000) seneca    (1000)      136 2022-06-24 11:34:11.000000 flask-dantic-0.0.6/flask_dantic/request_validator/exceptions.py
--rw-rw-r--   0 seneca    (1000) seneca    (1000)     2965 2022-06-24 11:34:11.000000 flask-dantic-0.0.6/flask_dantic/request_validator/validator.py
-drwxrwxr-x   0 seneca    (1000) seneca    (1000)        0 2022-08-11 08:43:01.156313 flask-dantic-0.0.6/flask_dantic.egg-info/
--rw-rw-r--   0 seneca    (1000) seneca    (1000)    10165 2022-08-11 08:43:01.000000 flask-dantic-0.0.6/flask_dantic.egg-info/PKG-INFO
--rw-rw-r--   0 seneca    (1000) seneca    (1000)      670 2022-08-11 08:43:01.000000 flask-dantic-0.0.6/flask_dantic.egg-info/SOURCES.txt
--rw-rw-r--   0 seneca    (1000) seneca    (1000)        1 2022-08-11 08:43:01.000000 flask-dantic-0.0.6/flask_dantic.egg-info/dependency_links.txt
--rw-rw-r--   0 seneca    (1000) seneca    (1000)       42 2022-08-11 08:43:01.000000 flask-dantic-0.0.6/flask_dantic.egg-info/requires.txt
--rw-rw-r--   0 seneca    (1000) seneca    (1000)       19 2022-08-11 08:43:01.000000 flask-dantic-0.0.6/flask_dantic.egg-info/top_level.txt
--rw-rw-r--   0 seneca    (1000) seneca    (1000)      269 2022-08-11 08:43:01.160313 flask-dantic-0.0.6/setup.cfg
--rw-rw-r--   0 seneca    (1000) seneca    (1000)     1917 2022-06-23 11:53:28.000000 flask-dantic-0.0.6/setup.py
-drwxrwxr-x   0 seneca    (1000) seneca    (1000)        0 2022-08-11 08:43:01.160313 flask-dantic-0.0.6/tests/
--rw-rw-r--   0 seneca    (1000) seneca    (1000)        0 2022-06-22 00:49:11.000000 flask-dantic-0.0.6/tests/__init__.py
--rw-rw-r--   0 seneca    (1000) seneca    (1000)      175 2022-06-23 18:26:37.000000 flask-dantic-0.0.6/tests/conftest.py
--rw-rw-r--   0 seneca    (1000) seneca    (1000)      626 2022-06-22 09:13:51.000000 flask-dantic-0.0.6/tests/create_test_db.py
--rw-rw-r--   0 seneca    (1000) seneca    (1000)     4553 2022-06-23 11:56:42.000000 flask-dantic-0.0.6/tests/test_json_encoder.py
--rw-rw-r--   0 seneca    (1000) seneca    (1000)     3845 2022-08-11 08:40:16.000000 flask-dantic-0.0.6/tests/test_serializer.py
--rw-rw-r--   0 seneca    (1000) seneca    (1000)    15446 2022-06-24 11:34:11.000000 flask-dantic-0.0.6/tests/test_validator.py
+drwxr-xr-x   0 vivekkeshore   (502) staff       (20)        0 2023-07-01 19:45:14.786934 flask-dantic-0.0.7/
+-rw-r--r--   0 vivekkeshore   (502) staff       (20)       28 2023-05-28 19:20:55.000000 flask-dantic-0.0.7/MANIFEST.in
+-rw-r--r--   0 vivekkeshore   (502) staff       (20)    10165 2023-07-01 19:45:14.787102 flask-dantic-0.0.7/PKG-INFO
+-rw-r--r--   0 vivekkeshore   (502) staff       (20)     6982 2023-05-28 19:20:55.000000 flask-dantic-0.0.7/README.md
+drwxr-xr-x   0 vivekkeshore   (502) staff       (20)        0 2023-07-01 19:45:14.783217 flask-dantic-0.0.7/flask_dantic/
+-rw-r--r--   0 vivekkeshore   (502) staff       (20)        5 2023-07-01 19:43:58.000000 flask-dantic-0.0.7/flask_dantic/VERSION
+-rw-r--r--   0 vivekkeshore   (502) staff       (20)      320 2023-05-28 19:20:55.000000 flask-dantic-0.0.7/flask_dantic/__init__.py
+drwxr-xr-x   0 vivekkeshore   (502) staff       (20)        0 2023-07-01 19:45:14.784843 flask-dantic-0.0.7/flask_dantic/pydantic_serializer/
+-rw-r--r--   0 vivekkeshore   (502) staff       (20)      157 2023-05-28 19:20:55.000000 flask-dantic-0.0.7/flask_dantic/pydantic_serializer/__init__.py
+-rw-r--r--   0 vivekkeshore   (502) staff       (20)     5474 2023-07-01 19:37:45.000000 flask-dantic-0.0.7/flask_dantic/pydantic_serializer/encoders.py
+-rw-r--r--   0 vivekkeshore   (502) staff       (20)     2233 2023-07-01 19:37:49.000000 flask-dantic-0.0.7/flask_dantic/pydantic_serializer/serializer.py
+drwxr-xr-x   0 vivekkeshore   (502) staff       (20)        0 2023-07-01 19:45:14.785405 flask-dantic-0.0.7/flask_dantic/request_validator/
+-rw-r--r--   0 vivekkeshore   (502) staff       (20)       72 2023-05-28 19:20:55.000000 flask-dantic-0.0.7/flask_dantic/request_validator/__init__.py
+-rw-r--r--   0 vivekkeshore   (502) staff       (20)      136 2023-05-28 19:20:55.000000 flask-dantic-0.0.7/flask_dantic/request_validator/exceptions.py
+-rw-r--r--   0 vivekkeshore   (502) staff       (20)     2965 2023-05-28 19:20:55.000000 flask-dantic-0.0.7/flask_dantic/request_validator/validator.py
+drwxr-xr-x   0 vivekkeshore   (502) staff       (20)        0 2023-07-01 19:45:14.784190 flask-dantic-0.0.7/flask_dantic.egg-info/
+-rw-r--r--   0 vivekkeshore   (502) staff       (20)    10165 2023-07-01 19:45:14.000000 flask-dantic-0.0.7/flask_dantic.egg-info/PKG-INFO
+-rw-r--r--   0 vivekkeshore   (502) staff       (20)      670 2023-07-01 19:45:14.000000 flask-dantic-0.0.7/flask_dantic.egg-info/SOURCES.txt
+-rw-r--r--   0 vivekkeshore   (502) staff       (20)        1 2023-07-01 19:45:14.000000 flask-dantic-0.0.7/flask_dantic.egg-info/dependency_links.txt
+-rw-r--r--   0 vivekkeshore   (502) staff       (20)       42 2023-07-01 19:45:14.000000 flask-dantic-0.0.7/flask_dantic.egg-info/requires.txt
+-rw-r--r--   0 vivekkeshore   (502) staff       (20)       19 2023-07-01 19:45:14.000000 flask-dantic-0.0.7/flask_dantic.egg-info/top_level.txt
+-rw-r--r--   0 vivekkeshore   (502) staff       (20)      269 2023-07-01 19:45:14.787795 flask-dantic-0.0.7/setup.cfg
+-rw-r--r--   0 vivekkeshore   (502) staff       (20)     1917 2023-05-28 19:20:55.000000 flask-dantic-0.0.7/setup.py
+drwxr-xr-x   0 vivekkeshore   (502) staff       (20)        0 2023-07-01 19:45:14.786643 flask-dantic-0.0.7/tests/
+-rw-r--r--   0 vivekkeshore   (502) staff       (20)        0 2023-05-28 19:20:54.000000 flask-dantic-0.0.7/tests/__init__.py
+-rw-r--r--   0 vivekkeshore   (502) staff       (20)      175 2023-05-28 19:20:54.000000 flask-dantic-0.0.7/tests/conftest.py
+-rw-r--r--   0 vivekkeshore   (502) staff       (20)      626 2023-05-28 19:20:54.000000 flask-dantic-0.0.7/tests/create_test_db.py
+-rw-r--r--   0 vivekkeshore   (502) staff       (20)     4553 2023-07-01 19:37:41.000000 flask-dantic-0.0.7/tests/test_json_encoder.py
+-rw-r--r--   0 vivekkeshore   (502) staff       (20)     3845 2023-07-01 19:37:32.000000 flask-dantic-0.0.7/tests/test_serializer.py
+-rw-r--r--   0 vivekkeshore   (502) staff       (20)    15446 2023-05-28 19:20:54.000000 flask-dantic-0.0.7/tests/test_validator.py
```

### Comparing `flask-dantic-0.0.6/PKG-INFO` & `flask-dantic-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-dantic
-Version: 0.0.6
+Version: 0.0.7
 Summary: This package provides a utility to validate pydantic request models and also serialize db object using pydantic models.
 Home-page: https://github.com/vivekkeshore/flask-dantic
 Author: Vivek Keshore
 Author-email: vivek.keshore@gmail.com
 License: MIT
 Description: # 🅕🅛🅐🅢🅚-🅓🅐🅝🅣🅘🅒
```

### Comparing `flask-dantic-0.0.6/README.md` & `flask-dantic-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `flask-dantic-0.0.6/flask_dantic/pydantic_serializer/encoders.py` & `flask-dantic-0.0.7/flask_dantic/pydantic_serializer/encoders.py`

 * *Files identical despite different names*

### Comparing `flask-dantic-0.0.6/flask_dantic/pydantic_serializer/serializer.py` & `flask-dantic-0.0.7/flask_dantic/pydantic_serializer/serializer.py`

 * *Files identical despite different names*

### Comparing `flask-dantic-0.0.6/flask_dantic/request_validator/validator.py` & `flask-dantic-0.0.7/flask_dantic/request_validator/validator.py`

 * *Files identical despite different names*

### Comparing `flask-dantic-0.0.6/flask_dantic.egg-info/PKG-INFO` & `flask-dantic-0.0.7/flask_dantic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-dantic
-Version: 0.0.6
+Version: 0.0.7
 Summary: This package provides a utility to validate pydantic request models and also serialize db object using pydantic models.
 Home-page: https://github.com/vivekkeshore/flask-dantic
 Author: Vivek Keshore
 Author-email: vivek.keshore@gmail.com
 License: MIT
 Description: # 🅕🅛🅐🅢🅚-🅓🅐🅝🅣🅘🅒
```

### Comparing `flask-dantic-0.0.6/flask_dantic.egg-info/SOURCES.txt` & `flask-dantic-0.0.7/flask_dantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask-dantic-0.0.6/setup.py` & `flask-dantic-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `flask-dantic-0.0.6/tests/create_test_db.py` & `flask-dantic-0.0.7/tests/create_test_db.py`

 * *Files identical despite different names*

### Comparing `flask-dantic-0.0.6/tests/test_json_encoder.py` & `flask-dantic-0.0.7/tests/test_json_encoder.py`

 * *Files identical despite different names*

### Comparing `flask-dantic-0.0.6/tests/test_serializer.py` & `flask-dantic-0.0.7/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `flask-dantic-0.0.6/tests/test_validator.py` & `flask-dantic-0.0.7/tests/test_validator.py`

 * *Files identical despite different names*

