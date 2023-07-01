# Comparing `tmp/sscred_fork-0.2.1.tar.gz` & `tmp/sscred_fork-0.2.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sscred_fork-0.2.1.tar", last modified: Thu Jun 29 18:43:00 2023, max compression
+gzip compressed data, was "/Users/benjaminK/Desktop/SSCred_fork/SSCred_fork/dist/.tmp-1zk1qy0k/sscred_fork-0.2.11.tar", last modified: Sat Jul  1 01:50:55 2023, max compression
```

## Comparing `sscred_fork-0.2.1.tar` & `sscred_fork-0.2.11.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-06-29 18:43:00.000000 sscred_fork-0.2.1/
--rw-r--r--   0 benjaminK   (501) staff       (20)     1537 2023-06-29 18:39:09.000000 sscred_fork-0.2.1/LICENSE
--rw-r--r--   0 benjaminK   (501) staff       (20)     9225 2023-06-29 18:43:00.000000 sscred_fork-0.2.1/PKG-INFO
--rw-r--r--   0 benjaminK   (501) staff       (20)     8328 2023-06-29 18:39:09.000000 sscred_fork-0.2.1/README.md
--rw-r--r--   0 benjaminK   (501) staff       (20)      877 2023-06-29 18:43:00.000000 sscred_fork-0.2.1/setup.cfg
--rw-r--r--   0 benjaminK   (501) staff       (20)     1565 2023-06-29 18:42:57.000000 sscred_fork-0.2.1/setup.py
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-06-29 18:43:00.000000 sscred_fork-0.2.1/sscred/
--rw-r--r--   0 benjaminK   (501) staff       (20)      502 2023-06-29 18:39:09.000000 sscred_fork-0.2.1/sscred/__init__.py
--rw-r--r--   0 benjaminK   (501) staff       (20)    12885 2023-06-29 18:39:09.000000 sscred_fork-0.2.1/sscred/acl.py
--rw-r--r--   0 benjaminK   (501) staff       (20)    12248 2023-06-29 18:39:09.000000 sscred_fork-0.2.1/sscred/blind_pedersen.py
--rw-r--r--   0 benjaminK   (501) staff       (20)    16436 2023-06-29 18:39:09.000000 sscred_fork-0.2.1/sscred/blind_signature.py
--rw-r--r--   0 benjaminK   (501) staff       (20)     6771 2023-06-29 18:39:09.000000 sscred_fork-0.2.1/sscred/commitment.py
--rw-r--r--   0 benjaminK   (501) staff       (20)       31 2023-06-29 18:39:09.000000 sscred_fork-0.2.1/sscred/config.py
--rw-r--r--   0 benjaminK   (501) staff       (20)     6280 2023-06-29 18:39:09.000000 sscred_fork-0.2.1/sscred/pack.py
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-06-29 18:43:00.000000 sscred_fork-0.2.1/sscred_fork.egg-info/
--rw-r--r--   0 benjaminK   (501) staff       (20)     9225 2023-06-29 18:43:00.000000 sscred_fork-0.2.1/sscred_fork.egg-info/PKG-INFO
--rw-r--r--   0 benjaminK   (501) staff       (20)      367 2023-06-29 18:43:00.000000 sscred_fork-0.2.1/sscred_fork.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminK   (501) staff       (20)        1 2023-06-29 18:43:00.000000 sscred_fork-0.2.1/sscred_fork.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminK   (501) staff       (20)       38 2023-06-29 18:43:00.000000 sscred_fork-0.2.1/sscred_fork.egg-info/requires.txt
--rw-r--r--   0 benjaminK   (501) staff       (20)        7 2023-06-29 18:43:00.000000 sscred_fork-0.2.1/sscred_fork.egg-info/top_level.txt
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-06-29 18:43:00.000000 sscred_fork-0.2.1/test/
--rw-r--r--   0 benjaminK   (501) staff       (20)    11039 2023-06-29 18:39:09.000000 sscred_fork-0.2.1/test/test_sscred.py
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-01 01:50:55.000000 sscred_fork-0.2.11/
+-rw-r--r--   0 benjaminK   (501) staff       (20)     1537 2023-06-29 18:39:09.000000 sscred_fork-0.2.11/LICENSE
+-rw-r--r--   0 benjaminK   (501) staff       (20)     9226 2023-07-01 01:50:55.000000 sscred_fork-0.2.11/PKG-INFO
+-rw-r--r--   0 benjaminK   (501) staff       (20)     8328 2023-06-29 18:39:09.000000 sscred_fork-0.2.11/README.md
+-rw-r--r--   0 benjaminK   (501) staff       (20)      878 2023-07-01 01:50:55.000000 sscred_fork-0.2.11/setup.cfg
+-rw-r--r--   0 benjaminK   (501) staff       (20)     1565 2023-06-29 18:42:57.000000 sscred_fork-0.2.11/setup.py
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-01 01:50:55.000000 sscred_fork-0.2.11/sscred/
+-rw-r--r--   0 benjaminK   (501) staff       (20)      502 2023-06-29 18:39:09.000000 sscred_fork-0.2.11/sscred/__init__.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)    12885 2023-06-29 18:39:09.000000 sscred_fork-0.2.11/sscred/acl.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)    12248 2023-06-29 18:39:09.000000 sscred_fork-0.2.11/sscred/blind_pedersen.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)    16436 2023-06-29 18:39:09.000000 sscred_fork-0.2.11/sscred/blind_signature.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)     6771 2023-06-29 18:39:09.000000 sscred_fork-0.2.11/sscred/commitment.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)       31 2023-06-29 18:39:09.000000 sscred_fork-0.2.11/sscred/config.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)     6481 2023-07-01 01:46:16.000000 sscred_fork-0.2.11/sscred/pack.py
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-01 01:50:55.000000 sscred_fork-0.2.11/sscred_fork.egg-info/
+-rw-r--r--   0 benjaminK   (501) staff       (20)     9226 2023-07-01 01:50:55.000000 sscred_fork-0.2.11/sscred_fork.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminK   (501) staff       (20)      367 2023-07-01 01:50:55.000000 sscred_fork-0.2.11/sscred_fork.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminK   (501) staff       (20)        1 2023-07-01 01:50:55.000000 sscred_fork-0.2.11/sscred_fork.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminK   (501) staff       (20)       38 2023-07-01 01:50:55.000000 sscred_fork-0.2.11/sscred_fork.egg-info/requires.txt
+-rw-r--r--   0 benjaminK   (501) staff       (20)        7 2023-07-01 01:50:55.000000 sscred_fork-0.2.11/sscred_fork.egg-info/top_level.txt
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-07-01 01:50:55.000000 sscred_fork-0.2.11/test/
+-rw-r--r--   0 benjaminK   (501) staff       (20)    11039 2023-06-29 18:39:09.000000 sscred_fork-0.2.11/test/test_sscred.py
```

### Comparing `sscred_fork-0.2.1/LICENSE` & `sscred_fork-0.2.11/LICENSE`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.1/PKG-INFO` & `sscred_fork-0.2.11/sscred_fork.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sscred_fork
-Version: 0.2.1
+Name: sscred-fork
+Version: 0.2.11
 Summary: Single Show Credentials: A Python library for anonymous authentication.
 Home-page: https://github.com/spring-epfl/SSCred
 Author: Kasra EdalatNejad
 Author-email: kasra.edalat@epfl.ch
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `sscred_fork-0.2.1/README.md` & `sscred_fork-0.2.11/README.md`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.1/setup.cfg` & `sscred_fork-0.2.11/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sscred
-version = 0.2.1
+version = 0.2.11
 license = BSD-3-Clause
 author = Kasra EdalatNejad
 author_email = kasra.edalat@epfl.ch
 description = Single Show Credentials: A Python library for anonymous authentication.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/spring-epfl/SSCred
```

### Comparing `sscred_fork-0.2.1/setup.py` & `sscred_fork-0.2.11/setup.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.1/sscred/acl.py` & `sscred_fork-0.2.11/sscred/acl.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.1/sscred/blind_pedersen.py` & `sscred_fork-0.2.11/sscred/blind_pedersen.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.1/sscred/blind_signature.py` & `sscred_fork-0.2.11/sscred/blind_signature.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.1/sscred/commitment.py` & `sscred_fork-0.2.11/sscred/commitment.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.1/sscred/pack.py` & `sscred_fork-0.2.11/sscred/pack.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,14 @@
             if isinstance(obj, T):
                 num, enc = _pack_reg[T]
                 return msgpack.ExtType(num, enc(obj))
 
     return petlib.pack.default(obj)
 
 
-
 def add_msgpack_support_slots(cls, ext, add_cls_methods=True):
     """Adds serialization support,
 
     Enables packing and unpacking with msgpack with 'pack.packb' and
     'pack.unpackb' methods.
 
     If add_method then enables equality, reading and writing for the classs.
@@ -74,21 +73,25 @@
         boolean <- obj1 == obj2
 
     Args:
         cls: class
         ext: an unique code for the msgpack's Ext hook
     """
     def enc(obj):
+        # data = {key: getattr(obj, key) for key in obj.__slots__}
+        # data['pk'] = obj.pk
+        # return packb(data)
         return packb({key: getattr(obj, key) for key in obj.__slots__})
 
     def dec(data):
         obj = cls.__new__(cls)
         for key, value in unpackb(data).items():
             if key != "__weakref__":
                 setattr(obj, key, value)
+        # obj.pk = data['pk']
         return obj
 
     def eq(a, b):
         if type(a) != type(b):
             return NotImplemented
         for ka, kb in zip(a.__slots__, b.__slots__):
             if getattr(a, ka) != getattr(b, kb):
@@ -156,35 +159,41 @@
     add_msgpack_support(blind_pedersen.BlindedPedersenParam, COUNTER_BASE+6)
     add_msgpack_support(blind_pedersen.BlPedersenCommitment, COUNTER_BASE+7)
     # Abe's signature
     add_msgpack_support_slots(blind_signature.AbeParam, COUNTER_BASE+8)
     add_msgpack_support_slots(blind_signature.AbePublicKey, COUNTER_BASE+9)
     add_msgpack_support_slots(blind_signature.AbePrivateKey, COUNTER_BASE+10)
     add_msgpack_support_slots(blind_signature.AbeSignature, COUNTER_BASE+11)
-    add_msgpack_support_slots(blind_signature.SignerCommitMessage, COUNTER_BASE+12)
-    add_msgpack_support_slots(blind_signature.SignerResponseMessage, COUNTER_BASE+13)
+    add_msgpack_support_slots(
+        blind_signature.SignerCommitMessage, COUNTER_BASE+12)
+    add_msgpack_support_slots(
+        blind_signature.SignerResponseMessage, COUNTER_BASE+13)
     # ACL
     add_msgpack_support_slots(acl.ACLParam, COUNTER_BASE+14)
     add_msgpack_support_slots(acl.ACLIssuerPrivateKey, COUNTER_BASE+15)
     add_msgpack_support_slots(acl.ACLIssuerPublicKey, COUNTER_BASE+16)
     add_msgpack_support_slots(acl.ProveAttrKnowledgeMessage, COUNTER_BASE+17)
     add_msgpack_support_slots(acl.ACLCredential, COUNTER_BASE+18)
     add_msgpack_support_slots(acl.ACLCredentialPrivate, COUNTER_BASE+19)
     # zksk
     add_msgpack_support(Secret, COUNTER_BASE+20, add_cls_methods=False)
     add_msgpack_support(NIZK, COUNTER_BASE+21, add_cls_methods=False)
 
     # Added later
-    add_msgpack_support_slots(blind_signature.SignerCommitmentInternalState, COUNTER_BASE+22)
-    add_msgpack_support_slots(blind_signature.UserBlindedChallengeInternalState, COUNTER_BASE+23)
-    add_msgpack_support_slots(blind_signature.BlindedChallengeMessage, COUNTER_BASE+24)
+    add_msgpack_support_slots(
+        blind_signature.SignerCommitmentInternalState, COUNTER_BASE+22)
+    add_msgpack_support_slots(
+        blind_signature.UserBlindedChallengeInternalState, COUNTER_BASE+23)
+    add_msgpack_support_slots(
+        blind_signature.BlindedChallengeMessage, COUNTER_BASE+24)
+
 
 register_all_classes()
 
 
 def main():
     import doctest
     doctest.testmod(verbose=True)
 
+
 if __name__ == '__main__':
     main()
-
```

### Comparing `sscred_fork-0.2.1/sscred_fork.egg-info/PKG-INFO` & `sscred_fork-0.2.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sscred-fork
-Version: 0.2.1
+Name: sscred_fork
+Version: 0.2.11
 Summary: Single Show Credentials: A Python library for anonymous authentication.
 Home-page: https://github.com/spring-epfl/SSCred
 Author: Kasra EdalatNejad
 Author-email: kasra.edalat@epfl.ch
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `sscred_fork-0.2.1/test/test_sscred.py` & `sscred_fork-0.2.11/test/test_sscred.py`

 * *Files identical despite different names*

