# Comparing `tmp/couchbed-0.1.2.tar.gz` & `tmp/couchbed-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "couchbed-0.1.2.tar", last modified: Sat Jul  1 14:48:06 2023, max compression
+gzip compressed data, was "couchbed-0.1.4.tar", last modified: Sat Jul  1 21:36:43 2023, max compression
```

## Comparing `couchbed-0.1.2.tar` & `couchbed-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-01 14:48:06.691670 couchbed-0.1.2/
--rw-r--r--   0 shuntaro   (501) staff       (20)     1075 2023-01-22 05:52:37.000000 couchbed-0.1.2/LICENSE.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        0 2023-07-01 01:19:19.000000 couchbed-0.1.2/MANIFEST.in
--rw-r--r--   0 shuntaro   (501) staff       (20)     2396 2023-07-01 14:48:06.691714 couchbed-0.1.2/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)     1930 2023-07-01 14:47:48.000000 couchbed-0.1.2/README.md
--rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 couchbed-0.1.2/pyproject.toml
--rw-r--r--   0 shuntaro   (501) staff       (20)      564 2023-07-01 14:48:06.691933 couchbed-0.1.2/setup.cfg
--rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 couchbed-0.1.2/setup.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-01 14:48:06.690993 couchbed-0.1.2/src/
--rw-r--r--   0 shuntaro   (501) staff       (20)       30 2023-07-01 02:56:33.000000 couchbed-0.1.2/src/__init__.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-01 14:48:06.691570 couchbed-0.1.2/src/couchbed.egg-info/
--rw-r--r--   0 shuntaro   (501) staff       (20)     2396 2023-07-01 14:48:06.000000 couchbed-0.1.2/src/couchbed.egg-info/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)      278 2023-07-01 14:48:06.000000 couchbed-0.1.2/src/couchbed.egg-info/SOURCES.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        1 2023-07-01 14:48:06.000000 couchbed-0.1.2/src/couchbed.egg-info/dependency_links.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       13 2023-07-01 14:48:06.000000 couchbed-0.1.2/src/couchbed.egg-info/requires.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       18 2023-07-01 14:48:06.000000 couchbed-0.1.2/src/couchbed.egg-info/top_level.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)     4047 2023-07-01 14:41:22.000000 couchbed-0.1.2/src/couchbed.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-01 21:36:43.374519 couchbed-0.1.4/
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1075 2023-01-22 05:52:37.000000 couchbed-0.1.4/LICENSE.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        0 2023-07-01 01:19:19.000000 couchbed-0.1.4/MANIFEST.in
+-rw-r--r--   0 shuntaro   (501) staff       (20)     2396 2023-07-01 21:36:43.374567 couchbed-0.1.4/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1930 2023-07-01 14:47:48.000000 couchbed-0.1.4/README.md
+-rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 couchbed-0.1.4/pyproject.toml
+-rw-r--r--   0 shuntaro   (501) staff       (20)      564 2023-07-01 21:36:43.374807 couchbed-0.1.4/setup.cfg
+-rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 couchbed-0.1.4/setup.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-01 21:36:43.373799 couchbed-0.1.4/src/
+-rw-r--r--   0 shuntaro   (501) staff       (20)       30 2023-07-01 02:56:33.000000 couchbed-0.1.4/src/__init__.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-01 21:36:43.374424 couchbed-0.1.4/src/couchbed.egg-info/
+-rw-r--r--   0 shuntaro   (501) staff       (20)     2396 2023-07-01 21:36:43.000000 couchbed-0.1.4/src/couchbed.egg-info/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)      278 2023-07-01 21:36:43.000000 couchbed-0.1.4/src/couchbed.egg-info/SOURCES.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        1 2023-07-01 21:36:43.000000 couchbed-0.1.4/src/couchbed.egg-info/dependency_links.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       13 2023-07-01 21:36:43.000000 couchbed-0.1.4/src/couchbed.egg-info/requires.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       18 2023-07-01 21:36:43.000000 couchbed-0.1.4/src/couchbed.egg-info/top_level.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)     4364 2023-07-01 21:36:24.000000 couchbed-0.1.4/src/couchbed.py
```

### Comparing `couchbed-0.1.2/LICENSE.txt` & `couchbed-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `couchbed-0.1.2/PKG-INFO` & `couchbed-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: couchbed
-Version: 0.1.2
+Version: 0.1.4
 Summary: Logging into CouchDB.
 Author: chocolate-icecream
 Keywords: CouchDB
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
```

### Comparing `couchbed-0.1.2/README.md` & `couchbed-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `couchbed-0.1.2/setup.cfg` & `couchbed-0.1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = couchbed
-version = 0.1.2
+version = 0.1.4
 author = chocolate-icecream
 description = Logging into CouchDB.
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
```

### Comparing `couchbed-0.1.2/src/couchbed.egg-info/PKG-INFO` & `couchbed-0.1.4/src/couchbed.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: couchbed
-Version: 0.1.2
+Version: 0.1.4
 Summary: Logging into CouchDB.
 Author: chocolate-icecream
 Keywords: CouchDB
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
```

### Comparing `couchbed-0.1.2/src/couchbed.py` & `couchbed-0.1.4/src/couchbed.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 class CBBook:
     def __init__(self, cbed, book_id):
         self.cbed = cbed
         self.book_id = book_id
         self.stopwatch_dict = {"startup": time.time()}
         self.log_dict = {}
         self.write_flag = False
-        self.content = {"msg": [], "log": [], "setting": {}, "created": self.cbed.iso_time_str, "last_updated": self.cbed.iso_time_str}
+        self.content = {"msg": [], "log": [], "setting": {}, "created": self.cbed.iso_time_str, "last_updated": self.cbed.iso_time_str, "results": {}}
 
     def __call__(self, *args):
         self.message(" ".join([f"{x}" for x in args]))
 
     def message(self, msg):
         time_stamped_msg = self.cbed.time_str +": "+ msg
         self.content["msg"].append(time_stamped_msg)
@@ -102,17 +102,26 @@
         return None
 
     def log(self, log_dict):
         log_dict = self.sanitize(log_dict)
         log_dict["_time"] = self.cbed.iso_time_str
         self.content["log"].append(log_dict)
         print(", ".join([f"{key}:{value}" for key, value in log_dict.items()]))
-        self.write_flag = True
         self.content["last_updated"] = self.cbed.iso_time_str
+        self.write_flag = True
+        
     
+    def result(self, result_dict):
+        result_dict = self.sanitize(result_dict)
+        result_dict["_time"] = self.cbed.iso_time_str
+        self.content["results"].update(result_dict)
+        self.content["last_updated"] = self.cbed.iso_time_str
+        self.write_flag = True
+        
+
     def save(self):
         self.cbed.save()
 
     def sanitize(self, value):
         if isinstance(value, (str, float, int)):
             return value
         elif isinstance(value, dict):
```

