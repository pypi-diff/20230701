# Comparing `tmp/couchbed-0.1.1.tar.gz` & `tmp/couchbed-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "couchbed-0.1.1.tar", last modified: Sat Jul  1 14:42:48 2023, max compression
+gzip compressed data, was "couchbed-0.1.2.tar", last modified: Sat Jul  1 14:48:06 2023, max compression
```

## Comparing `couchbed-0.1.1.tar` & `couchbed-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-01 14:42:48.556151 couchbed-0.1.1/
--rw-r--r--   0 shuntaro   (501) staff       (20)     1075 2023-01-22 05:52:37.000000 couchbed-0.1.1/LICENSE.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        0 2023-07-01 01:19:19.000000 couchbed-0.1.1/MANIFEST.in
--rw-r--r--   0 shuntaro   (501) staff       (20)     2317 2023-07-01 14:42:48.556222 couchbed-0.1.1/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)     1851 2023-07-01 02:58:14.000000 couchbed-0.1.1/README.md
--rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 couchbed-0.1.1/pyproject.toml
--rw-r--r--   0 shuntaro   (501) staff       (20)      564 2023-07-01 14:42:48.556452 couchbed-0.1.1/setup.cfg
--rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 couchbed-0.1.1/setup.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-01 14:42:48.555466 couchbed-0.1.1/src/
--rw-r--r--   0 shuntaro   (501) staff       (20)       30 2023-07-01 02:56:33.000000 couchbed-0.1.1/src/__init__.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-01 14:42:48.556023 couchbed-0.1.1/src/couchbed.egg-info/
--rw-r--r--   0 shuntaro   (501) staff       (20)     2317 2023-07-01 14:42:48.000000 couchbed-0.1.1/src/couchbed.egg-info/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)      278 2023-07-01 14:42:48.000000 couchbed-0.1.1/src/couchbed.egg-info/SOURCES.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        1 2023-07-01 14:42:48.000000 couchbed-0.1.1/src/couchbed.egg-info/dependency_links.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       13 2023-07-01 14:42:48.000000 couchbed-0.1.1/src/couchbed.egg-info/requires.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       18 2023-07-01 14:42:48.000000 couchbed-0.1.1/src/couchbed.egg-info/top_level.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)     4047 2023-07-01 14:41:22.000000 couchbed-0.1.1/src/couchbed.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-01 14:48:06.691670 couchbed-0.1.2/
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1075 2023-01-22 05:52:37.000000 couchbed-0.1.2/LICENSE.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        0 2023-07-01 01:19:19.000000 couchbed-0.1.2/MANIFEST.in
+-rw-r--r--   0 shuntaro   (501) staff       (20)     2396 2023-07-01 14:48:06.691714 couchbed-0.1.2/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1930 2023-07-01 14:47:48.000000 couchbed-0.1.2/README.md
+-rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 couchbed-0.1.2/pyproject.toml
+-rw-r--r--   0 shuntaro   (501) staff       (20)      564 2023-07-01 14:48:06.691933 couchbed-0.1.2/setup.cfg
+-rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 couchbed-0.1.2/setup.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-01 14:48:06.690993 couchbed-0.1.2/src/
+-rw-r--r--   0 shuntaro   (501) staff       (20)       30 2023-07-01 02:56:33.000000 couchbed-0.1.2/src/__init__.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-01 14:48:06.691570 couchbed-0.1.2/src/couchbed.egg-info/
+-rw-r--r--   0 shuntaro   (501) staff       (20)     2396 2023-07-01 14:48:06.000000 couchbed-0.1.2/src/couchbed.egg-info/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)      278 2023-07-01 14:48:06.000000 couchbed-0.1.2/src/couchbed.egg-info/SOURCES.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        1 2023-07-01 14:48:06.000000 couchbed-0.1.2/src/couchbed.egg-info/dependency_links.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       13 2023-07-01 14:48:06.000000 couchbed-0.1.2/src/couchbed.egg-info/requires.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       18 2023-07-01 14:48:06.000000 couchbed-0.1.2/src/couchbed.egg-info/top_level.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)     4047 2023-07-01 14:41:22.000000 couchbed-0.1.2/src/couchbed.py
```

### Comparing `couchbed-0.1.1/LICENSE.txt` & `couchbed-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `couchbed-0.1.1/PKG-INFO` & `couchbed-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: couchbed
-Version: 0.1.1
+Version: 0.1.2
 Summary: Logging into CouchDB.
 Author: chocolate-icecream
 Keywords: CouchDB
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
@@ -29,58 +29,61 @@
 
 First, import the `CouchBed` class from the `couchbed` module:
 
 ```python
 from couchbed import CouchBed
 ```
 
-Create an instance of the `CouchBed` class, specifying the name of the CouchDB database as a parameter. By default, CouchBed uses the CouchDB URI provided by the `PYTHON_COUCHBED` environment variable. Alternatively, you can pass the URI as a parameter when creating the `CouchBed` instance.
+Create an instance of the `CouchBed` class, specifying the name of the CouchDB database as a parameter. By default, CouchBed uses the CouchDB URI provided by the `PYTHON_COUCHBED` environment variable. Alternatively, you can pass the URI as a parameter when creating the `CouchBed` instance. For each trial, you prepare a new book (CBBook).
 
 ```python
 couch = CouchBed("__DATABASE_NAME__")
+book = couch.new_book()
 ```
 
 ### Recording Settings
 
-You can record settings by using the `set` method or by directly assigning values to keys in the `CouchBed` instance.
+You can record settings by using the `set` method or by directly assigning values to keys in the `CBBook` instance.
 
 ```python
-couch.set({"a": 1, "b": 2})
+book.set({"a": 1, "b": 2})
 # or
-couch["key"] = "value"
+book["key"] = "value"
 ```
 
 ### Accessing Settings
 
-You can access the recorded settings by using the `CouchBed` instance as a dictionary.
+You can access the recorded settings by using the `CBBook` instance as a dictionary.
 
 ```python
-print(couch["a"])
+print(book["a"])
 ```
 
 ### Recording Messages
 
-You can record messages by calling the `CouchBed` instance as a function and passing the desired message as arguments.
+You can record messages by calling the `CBBook` instance as a function and passing the desired message as arguments.
 
 ```python
-couch("Hello", 1, 2, 3)
+book("Hello", 1, 2, 3)
 ```
 
 ### Recording Logs
 
 You can record logs by using the `log` method and passing a dictionary containing the log information.
 
 ```python
-couch.log({"epoch": 1, "train_loss": 0.1, "val_loss": 0.15})
+book.log({"epoch": 1, "train_loss": 0.1, "val_loss": 0.15})
 ```
 
 ### Saving Data
 
 CouchBed automatically saves the data every 5 seconds if there are any changes. However, it's recommended to explicitly call the `save` method at the end of your program to ensure all the data is saved. Otherwise, the last 5-second data may be lost.
 
 ```python
+book.save()
+# or
 couch.save()
 ```
 
 ## License
 
 CouchBed is licensed under the MIT License.
```

### Comparing `couchbed-0.1.1/README.md` & `couchbed-0.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -14,58 +14,61 @@
 
 First, import the `CouchBed` class from the `couchbed` module:
 
 ```python
 from couchbed import CouchBed
 ```
 
-Create an instance of the `CouchBed` class, specifying the name of the CouchDB database as a parameter. By default, CouchBed uses the CouchDB URI provided by the `PYTHON_COUCHBED` environment variable. Alternatively, you can pass the URI as a parameter when creating the `CouchBed` instance.
+Create an instance of the `CouchBed` class, specifying the name of the CouchDB database as a parameter. By default, CouchBed uses the CouchDB URI provided by the `PYTHON_COUCHBED` environment variable. Alternatively, you can pass the URI as a parameter when creating the `CouchBed` instance. For each trial, you prepare a new book (CBBook).
 
 ```python
 couch = CouchBed("__DATABASE_NAME__")
+book = couch.new_book()
 ```
 
 ### Recording Settings
 
-You can record settings by using the `set` method or by directly assigning values to keys in the `CouchBed` instance.
+You can record settings by using the `set` method or by directly assigning values to keys in the `CBBook` instance.
 
 ```python
-couch.set({"a": 1, "b": 2})
+book.set({"a": 1, "b": 2})
 # or
-couch["key"] = "value"
+book["key"] = "value"
 ```
 
 ### Accessing Settings
 
-You can access the recorded settings by using the `CouchBed` instance as a dictionary.
+You can access the recorded settings by using the `CBBook` instance as a dictionary.
 
 ```python
-print(couch["a"])
+print(book["a"])
 ```
 
 ### Recording Messages
 
-You can record messages by calling the `CouchBed` instance as a function and passing the desired message as arguments.
+You can record messages by calling the `CBBook` instance as a function and passing the desired message as arguments.
 
 ```python
-couch("Hello", 1, 2, 3)
+book("Hello", 1, 2, 3)
 ```
 
 ### Recording Logs
 
 You can record logs by using the `log` method and passing a dictionary containing the log information.
 
 ```python
-couch.log({"epoch": 1, "train_loss": 0.1, "val_loss": 0.15})
+book.log({"epoch": 1, "train_loss": 0.1, "val_loss": 0.15})
 ```
 
 ### Saving Data
 
 CouchBed automatically saves the data every 5 seconds if there are any changes. However, it's recommended to explicitly call the `save` method at the end of your program to ensure all the data is saved. Otherwise, the last 5-second data may be lost.
 
 ```python
+book.save()
+# or
 couch.save()
 ```
 
 ## License
 
 CouchBed is licensed under the MIT License.
```

### Comparing `couchbed-0.1.1/setup.cfg` & `couchbed-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = couchbed
-version = 0.1.1
+version = 0.1.2
 author = chocolate-icecream
 description = Logging into CouchDB.
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
```

### Comparing `couchbed-0.1.1/src/couchbed.egg-info/PKG-INFO` & `couchbed-0.1.2/src/couchbed.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: couchbed
-Version: 0.1.1
+Version: 0.1.2
 Summary: Logging into CouchDB.
 Author: chocolate-icecream
 Keywords: CouchDB
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
@@ -29,58 +29,61 @@
 
 First, import the `CouchBed` class from the `couchbed` module:
 
 ```python
 from couchbed import CouchBed
 ```
 
-Create an instance of the `CouchBed` class, specifying the name of the CouchDB database as a parameter. By default, CouchBed uses the CouchDB URI provided by the `PYTHON_COUCHBED` environment variable. Alternatively, you can pass the URI as a parameter when creating the `CouchBed` instance.
+Create an instance of the `CouchBed` class, specifying the name of the CouchDB database as a parameter. By default, CouchBed uses the CouchDB URI provided by the `PYTHON_COUCHBED` environment variable. Alternatively, you can pass the URI as a parameter when creating the `CouchBed` instance. For each trial, you prepare a new book (CBBook).
 
 ```python
 couch = CouchBed("__DATABASE_NAME__")
+book = couch.new_book()
 ```
 
 ### Recording Settings
 
-You can record settings by using the `set` method or by directly assigning values to keys in the `CouchBed` instance.
+You can record settings by using the `set` method or by directly assigning values to keys in the `CBBook` instance.
 
 ```python
-couch.set({"a": 1, "b": 2})
+book.set({"a": 1, "b": 2})
 # or
-couch["key"] = "value"
+book["key"] = "value"
 ```
 
 ### Accessing Settings
 
-You can access the recorded settings by using the `CouchBed` instance as a dictionary.
+You can access the recorded settings by using the `CBBook` instance as a dictionary.
 
 ```python
-print(couch["a"])
+print(book["a"])
 ```
 
 ### Recording Messages
 
-You can record messages by calling the `CouchBed` instance as a function and passing the desired message as arguments.
+You can record messages by calling the `CBBook` instance as a function and passing the desired message as arguments.
 
 ```python
-couch("Hello", 1, 2, 3)
+book("Hello", 1, 2, 3)
 ```
 
 ### Recording Logs
 
 You can record logs by using the `log` method and passing a dictionary containing the log information.
 
 ```python
-couch.log({"epoch": 1, "train_loss": 0.1, "val_loss": 0.15})
+book.log({"epoch": 1, "train_loss": 0.1, "val_loss": 0.15})
 ```
 
 ### Saving Data
 
 CouchBed automatically saves the data every 5 seconds if there are any changes. However, it's recommended to explicitly call the `save` method at the end of your program to ensure all the data is saved. Otherwise, the last 5-second data may be lost.
 
 ```python
+book.save()
+# or
 couch.save()
 ```
 
 ## License
 
 CouchBed is licensed under the MIT License.
```

### Comparing `couchbed-0.1.1/src/couchbed.py` & `couchbed-0.1.2/src/couchbed.py`

 * *Files identical despite different names*

