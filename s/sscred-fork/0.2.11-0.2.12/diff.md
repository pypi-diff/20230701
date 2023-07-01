# Comparing `tmp/sscred_fork-0.2.11.tar.gz` & `tmp/sscred_fork-0.2.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/benjaminK/Desktop/SSCred_fork/SSCred_fork/dist/.tmp-1zk1qy0k/sscred_fork-0.2.11.tar", last modified: Sat Jul  1 01:50:55 2023, max compression
+gzip compressed data, was "/Users/benjaminK/Desktop/SSCred_fork/SSCred_fork/dist/.tmp-af47a3o1/sscred_fork-0.2.12.tar", last modified: Sat Jul  1 02:04:22 2023, max compression
```

## Comparing `sscred_fork-0.2.11.tar` & `sscred_fork-0.2.12.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-01 01:50:55.000000 sscred_fork-0.2.11/
--rw-r--r--   0 benjaminK   (501) staff       (20)     1537 2023-06-29 18:39:09.000000 sscred_fork-0.2.11/LICENSE
--rw-r--r--   0 benjaminK   (501) staff       (20)     9226 2023-07-01 01:50:55.000000 sscred_fork-0.2.11/PKG-INFO
--rw-r--r--   0 benjaminK   (501) staff       (20)     8328 2023-06-29 18:39:09.000000 sscred_fork-0.2.11/README.md
--rw-r--r--   0 benjaminK   (501) staff       (20)      878 2023-07-01 01:50:55.000000 sscred_fork-0.2.11/setup.cfg
--rw-r--r--   0 benjaminK   (501) staff       (20)     1565 2023-06-29 18:42:57.000000 sscred_fork-0.2.11/setup.py
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-01 01:50:55.000000 sscred_fork-0.2.11/sscred/
--rw-r--r--   0 benjaminK   (501) staff       (20)      502 2023-06-29 18:39:09.000000 sscred_fork-0.2.11/sscred/__init__.py
--rw-r--r--   0 benjaminK   (501) staff       (20)    12885 2023-06-29 18:39:09.000000 sscred_fork-0.2.11/sscred/acl.py
--rw-r--r--   0 benjaminK   (501) staff       (20)    12248 2023-06-29 18:39:09.000000 sscred_fork-0.2.11/sscred/blind_pedersen.py
--rw-r--r--   0 benjaminK   (501) staff       (20)    16436 2023-06-29 18:39:09.000000 sscred_fork-0.2.11/sscred/blind_signature.py
--rw-r--r--   0 benjaminK   (501) staff       (20)     6771 2023-06-29 18:39:09.000000 sscred_fork-0.2.11/sscred/commitment.py
--rw-r--r--   0 benjaminK   (501) staff       (20)       31 2023-06-29 18:39:09.000000 sscred_fork-0.2.11/sscred/config.py
--rw-r--r--   0 benjaminK   (501) staff       (20)     6481 2023-07-01 01:46:16.000000 sscred_fork-0.2.11/sscred/pack.py
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-01 01:50:55.000000 sscred_fork-0.2.11/sscred_fork.egg-info/
--rw-r--r--   0 benjaminK   (501) staff       (20)     9226 2023-07-01 01:50:55.000000 sscred_fork-0.2.11/sscred_fork.egg-info/PKG-INFO
--rw-r--r--   0 benjaminK   (501) staff       (20)      367 2023-07-01 01:50:55.000000 sscred_fork-0.2.11/sscred_fork.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminK   (501) staff       (20)        1 2023-07-01 01:50:55.000000 sscred_fork-0.2.11/sscred_fork.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminK   (501) staff       (20)       38 2023-07-01 01:50:55.000000 sscred_fork-0.2.11/sscred_fork.egg-info/requires.txt
--rw-r--r--   0 benjaminK   (501) staff       (20)        7 2023-07-01 01:50:55.000000 sscred_fork-0.2.11/sscred_fork.egg-info/top_level.txt
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-01 01:50:55.000000 sscred_fork-0.2.11/test/
--rw-r--r--   0 benjaminK   (501) staff       (20)    11039 2023-06-29 18:39:09.000000 sscred_fork-0.2.11/test/test_sscred.py
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-01 02:04:22.000000 sscred_fork-0.2.12/
+-rw-r--r--   0 benjaminK   (501) staff       (20)     1537 2023-06-29 18:39:09.000000 sscred_fork-0.2.12/LICENSE
+-rw-r--r--   0 benjaminK   (501) staff       (20)     9226 2023-07-01 02:04:22.000000 sscred_fork-0.2.12/PKG-INFO
+-rw-r--r--   0 benjaminK   (501) staff       (20)     8328 2023-06-29 18:39:09.000000 sscred_fork-0.2.12/README.md
+-rw-r--r--   0 benjaminK   (501) staff       (20)      878 2023-07-01 02:04:22.000000 sscred_fork-0.2.12/setup.cfg
+-rw-r--r--   0 benjaminK   (501) staff       (20)     1565 2023-06-29 18:42:57.000000 sscred_fork-0.2.12/setup.py
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-01 02:04:22.000000 sscred_fork-0.2.12/sscred/
+-rw-r--r--   0 benjaminK   (501) staff       (20)      502 2023-06-29 18:39:09.000000 sscred_fork-0.2.12/sscred/__init__.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)    12885 2023-06-29 18:39:09.000000 sscred_fork-0.2.12/sscred/acl.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)    12248 2023-06-29 18:39:09.000000 sscred_fork-0.2.12/sscred/blind_pedersen.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)    16436 2023-06-29 18:39:09.000000 sscred_fork-0.2.12/sscred/blind_signature.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)     6771 2023-06-29 18:39:09.000000 sscred_fork-0.2.12/sscred/commitment.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)       31 2023-06-29 18:39:09.000000 sscred_fork-0.2.12/sscred/config.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)     7266 2023-07-01 02:03:59.000000 sscred_fork-0.2.12/sscred/pack.py
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-01 02:04:22.000000 sscred_fork-0.2.12/sscred_fork.egg-info/
+-rw-r--r--   0 benjaminK   (501) staff       (20)     9226 2023-07-01 02:04:22.000000 sscred_fork-0.2.12/sscred_fork.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminK   (501) staff       (20)      367 2023-07-01 02:04:22.000000 sscred_fork-0.2.12/sscred_fork.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminK   (501) staff       (20)        1 2023-07-01 02:04:22.000000 sscred_fork-0.2.12/sscred_fork.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminK   (501) staff       (20)       38 2023-07-01 02:04:22.000000 sscred_fork-0.2.12/sscred_fork.egg-info/requires.txt
+-rw-r--r--   0 benjaminK   (501) staff       (20)        7 2023-07-01 02:04:22.000000 sscred_fork-0.2.12/sscred_fork.egg-info/top_level.txt
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-01 02:04:22.000000 sscred_fork-0.2.12/test/
+-rw-r--r--   0 benjaminK   (501) staff       (20)    11039 2023-06-29 18:39:09.000000 sscred_fork-0.2.12/test/test_sscred.py
```

### Comparing `sscred_fork-0.2.11/LICENSE` & `sscred_fork-0.2.12/LICENSE`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.11/PKG-INFO` & `sscred_fork-0.2.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sscred_fork
-Version: 0.2.11
+Version: 0.2.12
 Summary: Single Show Credentials: A Python library for anonymous authentication.
 Home-page: https://github.com/spring-epfl/SSCred
 Author: Kasra EdalatNejad
 Author-email: kasra.edalat@epfl.ch
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `sscred_fork-0.2.11/README.md` & `sscred_fork-0.2.12/README.md`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.11/setup.cfg` & `sscred_fork-0.2.12/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sscred
-version = 0.2.11
+version = 0.2.12
 license = BSD-3-Clause
 author = Kasra EdalatNejad
 author_email = kasra.edalat@epfl.ch
 description = Single Show Credentials: A Python library for anonymous authentication.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/spring-epfl/SSCred
```

### Comparing `sscred_fork-0.2.11/setup.py` & `sscred_fork-0.2.12/setup.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.11/sscred/acl.py` & `sscred_fork-0.2.12/sscred/acl.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.11/sscred/blind_pedersen.py` & `sscred_fork-0.2.12/sscred/blind_pedersen.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.11/sscred/blind_signature.py` & `sscred_fork-0.2.12/sscred/blind_signature.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.11/sscred/commitment.py` & `sscred_fork-0.2.12/sscred/commitment.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.11/sscred/pack.py` & `sscred_fork-0.2.12/sscred/pack.py`

 * *Files 17% similar despite different names*

```diff
@@ -73,25 +73,46 @@
         boolean <- obj1 == obj2
 
     Args:
         cls: class
         ext: an unique code for the msgpack's Ext hook
     """
     def enc(obj):
-        # data = {key: getattr(obj, key) for key in obj.__slots__}
-        # data['pk'] = obj.pk
-        # return packb(data)
-        return packb({key: getattr(obj, key) for key in obj.__slots__})
+        data = {key: getattr(obj, key) for key in obj.__slots__}
+        kv = {}
+
+        if hasattr(obj, 'bc_param'):
+            kv['bc_param'] = obj.bc_param
+        if hasattr(obj, 'pk'):
+            kv['pk'] = obj.pk
+        if hasattr(obj, 'z'):
+            kv['z'] = obj.z
+        if hasattr(obj, 'param'):
+            kv['param'] = obj.param
+            # if hasattr(obj, 'to_bytes'):
+            #     kv['to_bytes'] = obj.to_bytes
+            # if hasattr(obj, 'from_bytes'):
+            #     kv['from_bytes'] = obj.from_bytes
+            # if hasattr(obj, 'verify_signature'):
+            #     kv['verify_signature'] = obj.verify_signature
+            # if hasattr(obj, 'verify_parameters'):
+            #     kv['verify_parameters'] = obj.verify_parameters
+            # if hasattr(obj, '_compute_z_param'):
+            #     kv['_compute_z_param'] = obj._compute_z_param
+
+        data.update(kv)
+
+        return packb(data)
+        # return packb({key: getattr(obj, key) for key in obj.__slots__})
 
     def dec(data):
         obj = cls.__new__(cls)
         for key, value in unpackb(data).items():
             if key != "__weakref__":
                 setattr(obj, key, value)
-        # obj.pk = data['pk']
         return obj
 
     def eq(a, b):
         if type(a) != type(b):
             return NotImplemented
         for ka, kb in zip(a.__slots__, b.__slots__):
             if getattr(a, ka) != getattr(b, kb):
```

### Comparing `sscred_fork-0.2.11/sscred_fork.egg-info/PKG-INFO` & `sscred_fork-0.2.12/sscred_fork.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sscred-fork
-Version: 0.2.11
+Version: 0.2.12
 Summary: Single Show Credentials: A Python library for anonymous authentication.
 Home-page: https://github.com/spring-epfl/SSCred
 Author: Kasra EdalatNejad
 Author-email: kasra.edalat@epfl.ch
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `sscred_fork-0.2.11/test/test_sscred.py` & `sscred_fork-0.2.12/test/test_sscred.py`

 * *Files identical despite different names*

