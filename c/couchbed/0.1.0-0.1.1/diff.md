# Comparing `tmp/couchbed-0.1.0.tar.gz` & `tmp/couchbed-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "couchbed-0.1.0.tar", last modified: Sat Jul  1 03:01:32 2023, max compression
+gzip compressed data, was "couchbed-0.1.1.tar", last modified: Sat Jul  1 14:42:48 2023, max compression
```

## Comparing `couchbed-0.1.0.tar` & `couchbed-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-01 03:01:32.891462 couchbed-0.1.0/
--rw-r--r--   0 shuntaro   (501) staff       (20)     1075 2023-01-22 05:52:37.000000 couchbed-0.1.0/LICENSE.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        0 2023-07-01 01:19:19.000000 couchbed-0.1.0/MANIFEST.in
--rw-r--r--   0 shuntaro   (501) staff       (20)     2617 2023-07-01 03:01:32.891510 couchbed-0.1.0/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)     1851 2023-07-01 02:58:14.000000 couchbed-0.1.0/README.md
--rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 couchbed-0.1.0/pyproject.toml
--rw-r--r--   0 shuntaro   (501) staff       (20)      798 2023-07-01 03:01:32.891744 couchbed-0.1.0/setup.cfg
--rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 couchbed-0.1.0/setup.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-01 03:01:32.890718 couchbed-0.1.0/src/
--rw-r--r--   0 shuntaro   (501) staff       (20)       30 2023-07-01 02:56:33.000000 couchbed-0.1.0/src/__init__.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-01 03:01:32.891356 couchbed-0.1.0/src/couchbed.egg-info/
--rw-r--r--   0 shuntaro   (501) staff       (20)     2617 2023-07-01 03:01:32.000000 couchbed-0.1.0/src/couchbed.egg-info/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)      278 2023-07-01 03:01:32.000000 couchbed-0.1.0/src/couchbed.egg-info/SOURCES.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        1 2023-07-01 03:01:32.000000 couchbed-0.1.0/src/couchbed.egg-info/dependency_links.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       13 2023-07-01 03:01:32.000000 couchbed-0.1.0/src/couchbed.egg-info/requires.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       18 2023-07-01 03:01:32.000000 couchbed-0.1.0/src/couchbed.egg-info/top_level.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)     3662 2023-07-01 02:56:40.000000 couchbed-0.1.0/src/couchbed.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-01 14:42:48.556151 couchbed-0.1.1/
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1075 2023-01-22 05:52:37.000000 couchbed-0.1.1/LICENSE.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        0 2023-07-01 01:19:19.000000 couchbed-0.1.1/MANIFEST.in
+-rw-r--r--   0 shuntaro   (501) staff       (20)     2317 2023-07-01 14:42:48.556222 couchbed-0.1.1/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1851 2023-07-01 02:58:14.000000 couchbed-0.1.1/README.md
+-rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 couchbed-0.1.1/pyproject.toml
+-rw-r--r--   0 shuntaro   (501) staff       (20)      564 2023-07-01 14:42:48.556452 couchbed-0.1.1/setup.cfg
+-rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 couchbed-0.1.1/setup.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-01 14:42:48.555466 couchbed-0.1.1/src/
+-rw-r--r--   0 shuntaro   (501) staff       (20)       30 2023-07-01 02:56:33.000000 couchbed-0.1.1/src/__init__.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-01 14:42:48.556023 couchbed-0.1.1/src/couchbed.egg-info/
+-rw-r--r--   0 shuntaro   (501) staff       (20)     2317 2023-07-01 14:42:48.000000 couchbed-0.1.1/src/couchbed.egg-info/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)      278 2023-07-01 14:42:48.000000 couchbed-0.1.1/src/couchbed.egg-info/SOURCES.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        1 2023-07-01 14:42:48.000000 couchbed-0.1.1/src/couchbed.egg-info/dependency_links.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       13 2023-07-01 14:42:48.000000 couchbed-0.1.1/src/couchbed.egg-info/requires.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       18 2023-07-01 14:42:48.000000 couchbed-0.1.1/src/couchbed.egg-info/top_level.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)     4047 2023-07-01 14:41:22.000000 couchbed-0.1.1/src/couchbed.py
```

### Comparing `couchbed-0.1.0/LICENSE.txt` & `couchbed-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `couchbed-0.1.0/PKG-INFO` & `couchbed-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 Metadata-Version: 2.1
 Name: couchbed
-Version: 0.1.0
+Version: 0.1.1
 Summary: Logging into CouchDB.
 Author: chocolate-icecream
 Keywords: CouchDB
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # CouchBed
```

### Comparing `couchbed-0.1.0/README.md` & `couchbed-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `couchbed-0.1.0/src/couchbed.egg-info/PKG-INFO` & `couchbed-0.1.1/src/couchbed.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 Metadata-Version: 2.1
 Name: couchbed
-Version: 0.1.0
+Version: 0.1.1
 Summary: Logging into CouchDB.
 Author: chocolate-icecream
 Keywords: CouchDB
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # CouchBed
```

### Comparing `couchbed-0.1.0/src/couchbed.py` & `couchbed-0.1.1/src/couchbed.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,106 +11,114 @@
             return
         self.couch = couchdb.Server(uri)
         if db_name in self.couch:
             self.db = self.couch[db_name]
         else:
             self.db = self.couch.create(db_name)
         self.db_name = db_name
-        self.doc_id = self.time_str + " " + ''.join(random.choices(string.ascii_lowercase, k=3))
-        self.stopwatch_dict = {"startup": time.time()}
-        self.log_dict = {}
-        self.write_flag = False
-        self.doc = {"msg": [], "log": [], "setting": {}}
+        self.books = {}
+
         self.periodic_task()
-            
     
-    def __call__(self, *args):
+    def new_book(self):
+        if self.couch is None:
+            return dict()
+        book_id = self.time_str + " " + ''.join(random.choices(string.ascii_lowercase, k=3))
+        book = CBBook(self, book_id=book_id)
+        self.books[book_id] = book
+        return book
+    
+    def get_list(self):
+        pass
+
+    def periodic_task(self):
         if self.couch is None:
             return
-        self.message(" ".join([f"{x}" for x in args]))
+        t = threading.Timer(self.SAVE_PERIOD, self.periodic_task)
+        t.daemon = True
+        t.start()
+        try:
+            self.save()
+        except:
+            pass
 
-    def message(self, msg):
+    def save(self):
         if self.couch is None:
             return
-        time_stamped_msg = self.time_str +": "+ msg
-        self.doc["msg"].append(time_stamped_msg)
+        for book_id, book in self.books.items():
+            if not book.write_flag:
+                continue
+            self.db[book_id] = book.content
+            self.db.save(self.content)
+            book.write_flag = False
+
+    @property
+    def time_str(self):
+        return datetime.datetime.now().strftime("%y-%m-%d %H-%M-%S")
+    
+    @property
+    def iso_time_str(self):
+        return datetime.datetime.now().isoformat()
+
+class CBBook:
+    def __init__(self, cbed, book_id):
+        self.cbed = cbed
+        self.book_id = book_id
+        self.stopwatch_dict = {"startup": time.time()}
+        self.log_dict = {}
+        self.write_flag = False
+        self.content = {"msg": [], "log": [], "setting": {}, "created": self.cbed.iso_time_str, "last_updated": self.cbed.iso_time_str}
+
+    def __call__(self, *args):
+        self.message(" ".join([f"{x}" for x in args]))
+
+    def message(self, msg):
+        time_stamped_msg = self.cbed.time_str +": "+ msg
+        self.content["msg"].append(time_stamped_msg)
         self.write_flag = True
+        self.content["last_updated"] = self.cbed.iso_time_str
         print(time_stamped_msg)
     
     def start_stopwatch(self, watch_name):
-        if self.couch is None:
-            return
         self.stopwatch_dict[watch_name] = time.time()
 
     def record_stopwatch(self, watch_name="startup", msg=None):
-        if self.couch is None:
-            return
         if watch_name in self.stopwatch_dict:
             dt = time.time() - self.stopwatch_dict[watch_name]
             self.message(f"{watch_name} -> {dt} {f'({msg})' if msg is not None else ''}")
     
     def set(self, setting_dict):
-        if self.couch is None:
-            return
-        self.doc["setting"].update(self.sanitize(setting_dict))
+        self.content["setting"].update(self.sanitize(setting_dict))
         self.write_flag = True
+        self.content["last_updated"] = self.cbed.iso_time_str
 
     def __setitem__(self, key, value):
-        if self.couch is None:
-            return
-        self.doc["setting"][key] = self.sanitize(value)
+        self.content["setting"][key] = self.sanitize(value)
         self.write_flag = True
+        self.content["last_updated"] = self.cbed.iso_time_str
 
     def __getitem__(self, key):
-        if self.couch is None:
-            return
-        if key in self.doc["setting"]:
-            return self.doc["setting"][key]
+        if key in self.content["setting"]:
+            return self.content["setting"][key]
         return None
 
     def log(self, log_dict):
-        if self.couch is None:
-            return
         log_dict = self.sanitize(log_dict)
-        log_dict["_time"] = self.time_str
-        self.doc["log"].append(log_dict)
+        log_dict["_time"] = self.cbed.iso_time_str
+        self.content["log"].append(log_dict)
         print(", ".join([f"{key}:{value}" for key, value in log_dict.items()]))
         self.write_flag = True
-
-    def periodic_task(self):
-        if self.couch is None:
-            return
-        t = threading.Timer(self.SAVE_PERIOD, self.periodic_task)
-        t.daemon = True
-        t.start()
-        if self.write_flag:
-            try:
-                self.save()
-            except:
-                pass
+        self.content["last_updated"] = self.cbed.iso_time_str
     
+    def save(self):
+        self.cbed.save()
+
     def sanitize(self, value):
         if isinstance(value, (str, float, int)):
             return value
         elif isinstance(value, dict):
             result_dict = {}
             for k, v in value.items():
                 result_dict[k] = self.sanitize(v)
             return result_dict
         else:
             return ast.literal_eval(f"{value}")
-            
-
-    def save(self):
-        if self.couch is None:
-            return
-        if not self.write_flag:
-            pass
-        if isinstance(self.doc, dict):
-            self.db[self.doc_id] = self.doc
-            self.doc = self.db[self.doc_id]
-        self.db.save(self.doc)
-        self.write_flag = False
-
-    @property
-    def time_str(self):
-        return datetime.datetime.now().strftime("%y-%m-%d %H:%M:%S")
```

