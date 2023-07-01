# Comparing `tmp/igem-uploads-0.1.0.tar.gz` & `tmp/igem-uploads-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igem-uploads-0.1.0.tar", last modified: Sat Jul  1 18:43:18 2023, max compression
+gzip compressed data, was "igem-uploads-0.1.1.tar", last modified: Sat Jul  1 18:46:23 2023, max compression
```

## Comparing `igem-uploads-0.1.0.tar` & `igem-uploads-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 liang      (501) staff       (20)        0 2023-07-01 18:43:18.017032 igem-uploads-0.1.0/
--rw-r--r--   0 liang      (501) staff       (20)    18715 2023-07-01 18:14:41.000000 igem-uploads-0.1.0/LICENSE
--rw-r--r--   0 liang      (501) staff       (20)     1240 2023-07-01 18:43:18.016881 igem-uploads-0.1.0/PKG-INFO
--rw-r--r--   0 liang      (501) staff       (20)      856 2023-07-01 18:37:34.000000 igem-uploads-0.1.0/README.md
-drwxr-xr-x   0 liang      (501) staff       (20)        0 2023-07-01 18:43:18.016089 igem-uploads-0.1.0/igem_uploads.egg-info/
--rw-r--r--   0 liang      (501) staff       (20)     1240 2023-07-01 18:43:17.000000 igem-uploads-0.1.0/igem_uploads.egg-info/PKG-INFO
--rw-r--r--   0 liang      (501) staff       (20)      244 2023-07-01 18:43:17.000000 igem-uploads-0.1.0/igem_uploads.egg-info/SOURCES.txt
--rw-r--r--   0 liang      (501) staff       (20)        1 2023-07-01 18:43:17.000000 igem-uploads-0.1.0/igem_uploads.egg-info/dependency_links.txt
--rw-r--r--   0 liang      (501) staff       (20)        6 2023-07-01 18:43:17.000000 igem-uploads-0.1.0/igem_uploads.egg-info/requires.txt
--rw-r--r--   0 liang      (501) staff       (20)        8 2023-07-01 18:43:17.000000 igem-uploads-0.1.0/igem_uploads.egg-info/top_level.txt
--rw-r--r--   0 liang      (501) staff       (20)       38 2023-07-01 18:43:18.017079 igem-uploads-0.1.0/setup.cfg
--rw-r--r--   0 liang      (501) staff       (20)      658 2023-07-01 18:42:46.000000 igem-uploads-0.1.0/setup.py
-drwxr-xr-x   0 liang      (501) staff       (20)        0 2023-07-01 18:43:18.016553 igem-uploads-0.1.0/uploads/
--rw-r--r--   0 liang      (501) staff       (20)       29 2023-06-30 17:37:36.000000 igem-uploads-0.1.0/uploads/__init__.py
--rw-r--r--   0 liang      (501) staff       (20)     7357 2023-07-01 18:33:27.000000 igem-uploads-0.1.0/uploads/session.py
+drwxr-xr-x   0 liang      (501) staff       (20)        0 2023-07-01 18:46:23.315511 igem-uploads-0.1.1/
+-rw-r--r--   0 liang      (501) staff       (20)    18715 2023-07-01 18:14:41.000000 igem-uploads-0.1.1/LICENSE
+-rw-r--r--   0 liang      (501) staff       (20)     1248 2023-07-01 18:46:23.315381 igem-uploads-0.1.1/PKG-INFO
+-rw-r--r--   0 liang      (501) staff       (20)      856 2023-07-01 18:37:34.000000 igem-uploads-0.1.1/README.md
+drwxr-xr-x   0 liang      (501) staff       (20)        0 2023-07-01 18:46:23.314970 igem-uploads-0.1.1/igem_uploads.egg-info/
+-rw-r--r--   0 liang      (501) staff       (20)     1248 2023-07-01 18:46:23.000000 igem-uploads-0.1.1/igem_uploads.egg-info/PKG-INFO
+-rw-r--r--   0 liang      (501) staff       (20)      244 2023-07-01 18:46:23.000000 igem-uploads-0.1.1/igem_uploads.egg-info/SOURCES.txt
+-rw-r--r--   0 liang      (501) staff       (20)        1 2023-07-01 18:46:23.000000 igem-uploads-0.1.1/igem_uploads.egg-info/dependency_links.txt
+-rw-r--r--   0 liang      (501) staff       (20)        6 2023-07-01 18:46:23.000000 igem-uploads-0.1.1/igem_uploads.egg-info/requires.txt
+-rw-r--r--   0 liang      (501) staff       (20)        8 2023-07-01 18:46:23.000000 igem-uploads-0.1.1/igem_uploads.egg-info/top_level.txt
+-rw-r--r--   0 liang      (501) staff       (20)       38 2023-07-01 18:46:23.315551 igem-uploads-0.1.1/setup.cfg
+-rw-r--r--   0 liang      (501) staff       (20)      666 2023-07-01 18:46:13.000000 igem-uploads-0.1.1/setup.py
+drwxr-xr-x   0 liang      (501) staff       (20)        0 2023-07-01 18:46:23.315212 igem-uploads-0.1.1/uploads/
+-rw-r--r--   0 liang      (501) staff       (20)       29 2023-06-30 17:37:36.000000 igem-uploads-0.1.1/uploads/__init__.py
+-rw-r--r--   0 liang      (501) staff       (20)     7357 2023-07-01 18:33:27.000000 igem-uploads-0.1.1/uploads/session.py
```

### Comparing `igem-uploads-0.1.0/LICENSE` & `igem-uploads-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `igem-uploads-0.1.0/PKG-INFO` & `igem-uploads-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: igem-uploads
-Version: 0.1.0
+Version: 0.1.1
 Summary: Helps iGEMers upload their files to the iGEM server.
 Home-page: https://github.com/iGEM-HBUT-China/igem-uploads
-Author: lty2002
+Author: iGEM-HBUT-China
 Author-email: liangtianyi2002@outlook.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # igem-uploads
```

### Comparing `igem-uploads-0.1.0/README.md` & `igem-uploads-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `igem-uploads-0.1.0/igem_uploads.egg-info/PKG-INFO` & `igem-uploads-0.1.1/igem_uploads.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: igem-uploads
-Version: 0.1.0
+Version: 0.1.1
 Summary: Helps iGEMers upload their files to the iGEM server.
 Home-page: https://github.com/iGEM-HBUT-China/igem-uploads
-Author: lty2002
+Author: iGEM-HBUT-China
 Author-email: liangtianyi2002@outlook.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # igem-uploads
```

### Comparing `igem-uploads-0.1.0/setup.py` & `igem-uploads-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = ["wheel"]
 
 setup(
     name="igem-uploads",
-    version="0.1.0",
-    author="lty2002",
+    version="0.1.1",
+    author="iGEM-HBUT-China",
     author_email="liangtianyi2002@outlook.com",
     description="Helps iGEMers upload their files to the iGEM server.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/iGEM-HBUT-China/igem-uploads",
     packages=find_packages(),
     install_requires=requirements,
```

### Comparing `igem-uploads-0.1.0/uploads/session.py` & `igem-uploads-0.1.1/uploads/session.py`

 * *Files identical despite different names*

