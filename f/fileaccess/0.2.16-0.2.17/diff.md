# Comparing `tmp/fileaccess-0.2.16.tar.gz` & `tmp/fileaccess-0.2.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fileaccess-0.2.16.tar", last modified: Sat Jul  1 04:27:26 2023, max compression
+gzip compressed data, was "fileaccess-0.2.17.tar", last modified: Sat Jul  1 04:35:37 2023, max compression
```

## Comparing `fileaccess-0.2.16.tar` & `fileaccess-0.2.17.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 joehacobian   (501) staff       (20)        0 2023-07-01 04:27:26.909960 fileaccess-0.2.16/
--rw-r--r--   0 joehacobian   (501) staff       (20)     1060 2023-04-26 23:34:23.000000 fileaccess-0.2.16/LICENSE
--rw-r--r--   0 joehacobian   (501) staff       (20)     3896 2023-07-01 04:27:26.909734 fileaccess-0.2.16/PKG-INFO
--rw-r--r--   0 joehacobian   (501) staff       (20)     3054 2023-07-01 04:10:04.000000 fileaccess-0.2.16/README.md
-drwxr-xr-x   0 joehacobian   (501) staff       (20)        0 2023-07-01 04:27:26.908136 fileaccess-0.2.16/fileaccess/
--rw-r--r--   0 joehacobian   (501) staff       (20)     4494 2023-07-01 04:00:59.000000 fileaccess-0.2.16/fileaccess/__init__.py
-drwxr-xr-x   0 joehacobian   (501) staff       (20)        0 2023-07-01 04:27:26.909450 fileaccess-0.2.16/fileaccess.egg-info/
--rw-r--r--   0 joehacobian   (501) staff       (20)     3896 2023-07-01 04:27:26.000000 fileaccess-0.2.16/fileaccess.egg-info/PKG-INFO
--rw-r--r--   0 joehacobian   (501) staff       (20)      218 2023-07-01 04:27:26.000000 fileaccess-0.2.16/fileaccess.egg-info/SOURCES.txt
--rw-r--r--   0 joehacobian   (501) staff       (20)        1 2023-07-01 04:27:26.000000 fileaccess-0.2.16/fileaccess.egg-info/dependency_links.txt
--rw-r--r--   0 joehacobian   (501) staff       (20)        3 2023-07-01 04:27:26.000000 fileaccess-0.2.16/fileaccess.egg-info/requires.txt
--rw-r--r--   0 joehacobian   (501) staff       (20)       11 2023-07-01 04:27:26.000000 fileaccess-0.2.16/fileaccess.egg-info/top_level.txt
--rw-r--r--   0 joehacobian   (501) staff       (20)       38 2023-07-01 04:27:26.910023 fileaccess-0.2.16/setup.cfg
--rw-r--r--   0 joehacobian   (501) staff       (20)     1031 2023-07-01 04:13:06.000000 fileaccess-0.2.16/setup.py
+drwxr-xr-x   0 joehacobian   (501) staff       (20)        0 2023-07-01 04:35:36.998139 fileaccess-0.2.17/
+-rw-r--r--   0 joehacobian   (501) staff       (20)     1060 2023-04-26 23:34:23.000000 fileaccess-0.2.17/LICENSE
+-rw-r--r--   0 joehacobian   (501) staff       (20)     4247 2023-07-01 04:35:36.997749 fileaccess-0.2.17/PKG-INFO
+-rw-r--r--   0 joehacobian   (501) staff       (20)     3405 2023-07-01 04:35:00.000000 fileaccess-0.2.17/README.md
+drwxr-xr-x   0 joehacobian   (501) staff       (20)        0 2023-07-01 04:35:36.994211 fileaccess-0.2.17/fileaccess/
+-rw-r--r--   0 joehacobian   (501) staff       (20)     4494 2023-07-01 04:00:59.000000 fileaccess-0.2.17/fileaccess/__init__.py
+drwxr-xr-x   0 joehacobian   (501) staff       (20)        0 2023-07-01 04:35:36.997244 fileaccess-0.2.17/fileaccess.egg-info/
+-rw-r--r--   0 joehacobian   (501) staff       (20)     4247 2023-07-01 04:35:36.000000 fileaccess-0.2.17/fileaccess.egg-info/PKG-INFO
+-rw-r--r--   0 joehacobian   (501) staff       (20)      218 2023-07-01 04:35:36.000000 fileaccess-0.2.17/fileaccess.egg-info/SOURCES.txt
+-rw-r--r--   0 joehacobian   (501) staff       (20)        1 2023-07-01 04:35:36.000000 fileaccess-0.2.17/fileaccess.egg-info/dependency_links.txt
+-rw-r--r--   0 joehacobian   (501) staff       (20)        3 2023-07-01 04:35:36.000000 fileaccess-0.2.17/fileaccess.egg-info/requires.txt
+-rw-r--r--   0 joehacobian   (501) staff       (20)       11 2023-07-01 04:35:36.000000 fileaccess-0.2.17/fileaccess.egg-info/top_level.txt
+-rw-r--r--   0 joehacobian   (501) staff       (20)       38 2023-07-01 04:35:36.998226 fileaccess-0.2.17/setup.cfg
+-rw-r--r--   0 joehacobian   (501) staff       (20)     1031 2023-07-01 04:35:16.000000 fileaccess-0.2.17/setup.py
```

### Comparing `fileaccess-0.2.16/LICENSE` & `fileaccess-0.2.17/LICENSE`

 * *Files identical despite different names*

### Comparing `fileaccess-0.2.16/PKG-INFO` & `fileaccess-0.2.17/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileaccess
-Version: 0.2.16
+Version: 0.2.17
 Summary: A package for easier file access, automatically closes opened file handles, & provides for simple file/directory creation.
 Home-page: https://github.com/node0/Fileaccess
 Author: Joe Hacobian
 Author-email: joehacobian@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -60,14 +60,20 @@
 Fileaccess.createFile(assetType="f", targetPath="/path/to/file.txt", fileContents="File contents")
 ```
 
 In the above example, `assetType` can be either `"f"` to create a file or `"d"` to create a directory. The `targetPath` parameter specifies the path where the file or directory will be created. The `fileContents` parameter is optional & can be used to specify the contents of the file.
   
 Note: You do NOT need to first create the directory path for a file if the directory path doesn't exist (all you need are access permissions for the user python is running as). The full directory path will automatically be create for you simply by you providing a full file path.
   
+Note 2: If you wish to exercise more granluar control over file and folder permissions at creation time there are two parameters you may use: `filePermissions` & `folderPermissions`  
+
+Below are the assumed default values if one or both of these paramters is not given specific other values:  
+`filePermissions="0644"`  
+`folderPermissions="0755"`  
+
 
 ## File Access Modes
 The `mode` parameter in the `Fileaccess` class specifies the file access mode. Here's a table of the available modes:
 
 | Mode | Meaning |
 | --- | --- |
 | `r` | Open for reading (default) |
```

### Comparing `fileaccess-0.2.16/README.md` & `fileaccess-0.2.17/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -40,14 +40,20 @@
 Fileaccess.createFile(assetType="f", targetPath="/path/to/file.txt", fileContents="File contents")
 ```
 
 In the above example, `assetType` can be either `"f"` to create a file or `"d"` to create a directory. The `targetPath` parameter specifies the path where the file or directory will be created. The `fileContents` parameter is optional & can be used to specify the contents of the file.
   
 Note: You do NOT need to first create the directory path for a file if the directory path doesn't exist (all you need are access permissions for the user python is running as). The full directory path will automatically be create for you simply by you providing a full file path.
   
+Note 2: If you wish to exercise more granluar control over file and folder permissions at creation time there are two parameters you may use: `filePermissions` & `folderPermissions`  
+
+Below are the assumed default values if one or both of these paramters is not given specific other values:  
+`filePermissions="0644"`  
+`folderPermissions="0755"`  
+
 
 ## File Access Modes
 The `mode` parameter in the `Fileaccess` class specifies the file access mode. Here's a table of the available modes:
 
 | Mode | Meaning |
 | --- | --- |
 | `r` | Open for reading (default) |
```

### Comparing `fileaccess-0.2.16/fileaccess/__init__.py` & `fileaccess-0.2.17/fileaccess/__init__.py`

 * *Files identical despite different names*

### Comparing `fileaccess-0.2.16/fileaccess.egg-info/PKG-INFO` & `fileaccess-0.2.17/fileaccess.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileaccess
-Version: 0.2.16
+Version: 0.2.17
 Summary: A package for easier file access, automatically closes opened file handles, & provides for simple file/directory creation.
 Home-page: https://github.com/node0/Fileaccess
 Author: Joe Hacobian
 Author-email: joehacobian@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -60,14 +60,20 @@
 Fileaccess.createFile(assetType="f", targetPath="/path/to/file.txt", fileContents="File contents")
 ```
 
 In the above example, `assetType` can be either `"f"` to create a file or `"d"` to create a directory. The `targetPath` parameter specifies the path where the file or directory will be created. The `fileContents` parameter is optional & can be used to specify the contents of the file.
   
 Note: You do NOT need to first create the directory path for a file if the directory path doesn't exist (all you need are access permissions for the user python is running as). The full directory path will automatically be create for you simply by you providing a full file path.
   
+Note 2: If you wish to exercise more granluar control over file and folder permissions at creation time there are two parameters you may use: `filePermissions` & `folderPermissions`  
+
+Below are the assumed default values if one or both of these paramters is not given specific other values:  
+`filePermissions="0644"`  
+`folderPermissions="0755"`  
+
 
 ## File Access Modes
 The `mode` parameter in the `Fileaccess` class specifies the file access mode. Here's a table of the available modes:
 
 | Mode | Meaning |
 | --- | --- |
 | `r` | Open for reading (default) |
```

### Comparing `fileaccess-0.2.16/setup.py` & `fileaccess-0.2.17/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fileaccess",
-    version="0.2.16",
+    version="0.2.17",
     packages=find_packages(),
     install_requires=[
         "sh"
     ],
     author="Joe Hacobian",
     author_email="joehacobian@gmail.com",
     description="A package for easier file access, automatically closes opened file handles, & provides for simple file/directory creation.",
```

