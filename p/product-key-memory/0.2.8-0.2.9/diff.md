# Comparing `tmp/product_key_memory-0.2.8.tar.gz` & `tmp/product_key_memory-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "product_key_memory-0.2.8.tar", last modified: Fri Jun 30 21:49:37 2023, max compression
+gzip compressed data, was "product_key_memory-0.2.9.tar", last modified: Sat Jul  1 17:12:38 2023, max compression
```

## Comparing `product_key_memory-0.2.8.tar` & `product_key_memory-0.2.9.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:37.983594 product_key_memory-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-30 21:49:28.000000 product_key_memory-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-30 21:49:37.983594 product_key_memory-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-30 21:49:28.000000 product_key_memory-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:37.983594 product_key_memory-0.2.8/product_key_memory/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-30 21:49:28.000000 product_key_memory-0.2.8/product_key_memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-06-30 21:49:28.000000 product_key_memory-0.2.8/product_key_memory/product_key_memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:37.983594 product_key_memory-0.2.8/product_key_memory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-30 21:49:37.000000 product_key_memory-0.2.8/product_key_memory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-30 21:49:37.000000 product_key_memory-0.2.8/product_key_memory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 21:49:37.000000 product_key_memory-0.2.8/product_key_memory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-30 21:49:37.000000 product_key_memory-0.2.8/product_key_memory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-30 21:49:37.000000 product_key_memory-0.2.8/product_key_memory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 21:49:37.983594 product_key_memory-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-30 21:49:28.000000 product_key_memory-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:12:38.873859 product_key_memory-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-01 17:12:26.000000 product_key_memory-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-01 17:12:38.873859 product_key_memory-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-01 17:12:26.000000 product_key_memory-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:12:38.873859 product_key_memory-0.2.9/product_key_memory/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-01 17:12:26.000000 product_key_memory-0.2.9/product_key_memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-07-01 17:12:26.000000 product_key_memory-0.2.9/product_key_memory/product_key_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-01 17:12:26.000000 product_key_memory-0.2.9/product_key_memory/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:12:38.873859 product_key_memory-0.2.9/product_key_memory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-01 17:12:38.000000 product_key_memory-0.2.9/product_key_memory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-01 17:12:38.000000 product_key_memory-0.2.9/product_key_memory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 17:12:38.000000 product_key_memory-0.2.9/product_key_memory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-01 17:12:38.000000 product_key_memory-0.2.9/product_key_memory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-01 17:12:38.000000 product_key_memory-0.2.9/product_key_memory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 17:12:38.873859 product_key_memory-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-01 17:12:26.000000 product_key_memory-0.2.9/setup.py
```

### Comparing `product_key_memory-0.2.8/LICENSE` & `product_key_memory-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `product_key_memory-0.2.8/PKG-INFO` & `product_key_memory-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: product_key_memory
-Version: 0.2.8
+Version: 0.2.9
 Summary: Product Key Memory
 Home-page: https://github.com/lucidrains/product-key-memory
 Author: Aran Komatsuzaki, Phil Wang
 Author-email: aran1234321@gmail.com, lucidrains@gmail.com
 License: MIT
 Keywords: transformers,artificial intelligence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `product_key_memory-0.2.8/README.md` & `product_key_memory-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `product_key_memory-0.2.8/product_key_memory/product_key_memory.py` & `product_key_memory-0.2.9/product_key_memory/product_key_memory.py`

 * *Files identical despite different names*

### Comparing `product_key_memory-0.2.8/product_key_memory.egg-info/PKG-INFO` & `product_key_memory-0.2.9/product_key_memory.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: product-key-memory
-Version: 0.2.8
+Version: 0.2.9
 Summary: Product Key Memory
 Home-page: https://github.com/lucidrains/product-key-memory
 Author: Aran Komatsuzaki, Phil Wang
 Author-email: aran1234321@gmail.com, lucidrains@gmail.com
 License: MIT
 Keywords: transformers,artificial intelligence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `product_key_memory-0.2.8/setup.py` & `product_key_memory-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'product_key_memory',
     packages = find_packages(),
-    version = '0.2.8',
+    version = '0.2.9',
     license = 'MIT',
     description = 'Product Key Memory',
     long_description_content_type = 'text/markdown',
     author = 'Aran Komatsuzaki, Phil Wang',
     author_email = 'aran1234321@gmail.com, lucidrains@gmail.com',
     url = 'https://github.com/lucidrains/product-key-memory',
     keywords = [
```

