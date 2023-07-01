# Comparing `tmp/fileaccess-0.2.13.tar.gz` & `tmp/fileaccess-0.2.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fileaccess-0.2.13.tar", last modified: Fri Jun 23 19:36:19 2023, max compression
+gzip compressed data, was "fileaccess-0.2.16.tar", last modified: Sat Jul  1 04:27:26 2023, max compression
```

## Comparing `fileaccess-0.2.13.tar` & `fileaccess-0.2.16.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 joehacobian   (501) staff       (20)        0 2023-06-23 19:36:19.373391 fileaccess-0.2.13/
--rw-r--r--   0 joehacobian   (501) staff       (20)     1060 2023-04-26 23:34:23.000000 fileaccess-0.2.13/LICENSE
--rw-r--r--   0 joehacobian   (501) staff       (20)     3858 2023-06-23 19:36:19.373134 fileaccess-0.2.13/PKG-INFO
--rw-r--r--   0 joehacobian   (501) staff       (20)     3015 2023-06-23 19:25:55.000000 fileaccess-0.2.13/README.md
-drwxr-xr-x   0 joehacobian   (501) staff       (20)        0 2023-06-23 19:36:19.371045 fileaccess-0.2.13/fileaccess/
--rw-r--r--   0 joehacobian   (501) staff       (20)     4375 2023-04-26 22:46:58.000000 fileaccess-0.2.13/fileaccess/__init__.py
-drwxr-xr-x   0 joehacobian   (501) staff       (20)        0 2023-06-23 19:36:19.372786 fileaccess-0.2.13/fileaccess.egg-info/
--rw-r--r--   0 joehacobian   (501) staff       (20)     3858 2023-06-23 19:36:19.000000 fileaccess-0.2.13/fileaccess.egg-info/PKG-INFO
--rw-r--r--   0 joehacobian   (501) staff       (20)      218 2023-06-23 19:36:19.000000 fileaccess-0.2.13/fileaccess.egg-info/SOURCES.txt
--rw-r--r--   0 joehacobian   (501) staff       (20)        1 2023-06-23 19:36:19.000000 fileaccess-0.2.13/fileaccess.egg-info/dependency_links.txt
--rw-r--r--   0 joehacobian   (501) staff       (20)        3 2023-06-23 19:36:19.000000 fileaccess-0.2.13/fileaccess.egg-info/requires.txt
--rw-r--r--   0 joehacobian   (501) staff       (20)       11 2023-06-23 19:36:19.000000 fileaccess-0.2.13/fileaccess.egg-info/top_level.txt
--rw-r--r--   0 joehacobian   (501) staff       (20)       38 2023-06-23 19:36:19.373468 fileaccess-0.2.13/setup.cfg
--rw-r--r--   0 joehacobian   (501) staff       (20)     1032 2023-06-23 19:25:51.000000 fileaccess-0.2.13/setup.py
+drwxr-xr-x   0 joehacobian   (501) staff       (20)        0 2023-07-01 04:27:26.909960 fileaccess-0.2.16/
+-rw-r--r--   0 joehacobian   (501) staff       (20)     1060 2023-04-26 23:34:23.000000 fileaccess-0.2.16/LICENSE
+-rw-r--r--   0 joehacobian   (501) staff       (20)     3896 2023-07-01 04:27:26.909734 fileaccess-0.2.16/PKG-INFO
+-rw-r--r--   0 joehacobian   (501) staff       (20)     3054 2023-07-01 04:10:04.000000 fileaccess-0.2.16/README.md
+drwxr-xr-x   0 joehacobian   (501) staff       (20)        0 2023-07-01 04:27:26.908136 fileaccess-0.2.16/fileaccess/
+-rw-r--r--   0 joehacobian   (501) staff       (20)     4494 2023-07-01 04:00:59.000000 fileaccess-0.2.16/fileaccess/__init__.py
+drwxr-xr-x   0 joehacobian   (501) staff       (20)        0 2023-07-01 04:27:26.909450 fileaccess-0.2.16/fileaccess.egg-info/
+-rw-r--r--   0 joehacobian   (501) staff       (20)     3896 2023-07-01 04:27:26.000000 fileaccess-0.2.16/fileaccess.egg-info/PKG-INFO
+-rw-r--r--   0 joehacobian   (501) staff       (20)      218 2023-07-01 04:27:26.000000 fileaccess-0.2.16/fileaccess.egg-info/SOURCES.txt
+-rw-r--r--   0 joehacobian   (501) staff       (20)        1 2023-07-01 04:27:26.000000 fileaccess-0.2.16/fileaccess.egg-info/dependency_links.txt
+-rw-r--r--   0 joehacobian   (501) staff       (20)        3 2023-07-01 04:27:26.000000 fileaccess-0.2.16/fileaccess.egg-info/requires.txt
+-rw-r--r--   0 joehacobian   (501) staff       (20)       11 2023-07-01 04:27:26.000000 fileaccess-0.2.16/fileaccess.egg-info/top_level.txt
+-rw-r--r--   0 joehacobian   (501) staff       (20)       38 2023-07-01 04:27:26.910023 fileaccess-0.2.16/setup.cfg
+-rw-r--r--   0 joehacobian   (501) staff       (20)     1031 2023-07-01 04:13:06.000000 fileaccess-0.2.16/setup.py
```

### Comparing `fileaccess-0.2.13/LICENSE` & `fileaccess-0.2.16/LICENSE`

 * *Files identical despite different names*

### Comparing `fileaccess-0.2.13/PKG-INFO` & `fileaccess-0.2.16/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: fileaccess
-Version: 0.2.13
+Version: 0.2.16
 Summary: A package for easier file access, automatically closes opened file handles, & provides for simple file/directory creation.
 Home-page: https://github.com/node0/Fileaccess
 Author: Joe Hacobian
 Author-email: joehacobian@gmail.com
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -19,50 +19,52 @@
 License-File: LICENSE
 
 # Fileaccess Utility Class
 
 ## Introduction
 `Fileaccess` is a utility class for safely dealing with files. This class can be used to read, write, or append to a file, as well as create a file or directory. A nice benefit of using it is the automatic file handle management it provides.  
 
-The main productivity benefit of using this class is the createFile() method which creates file and directory paths automatically for a given file or directory asset, as well as allowing the writing of file contents together in a single method call. If you find yourself writing out a directory tree or a lot of files, this can save you frustration.  
+The main productivity benefit of using this class is the createFile() method which creates file & directory paths automatically for a given file or directory asset, as well as allowing the writing of file contents together in a single method call.  
+
+If you find yourself writing out a directory tree or a lot of files, this can save you time *(binary bytes or text are auto-detected & correctly written)*.  
 
 ## Usage
 ### Reading a File
-To read a file, use the `with` statement and specify the file name and mode as the `Fileaccess` class parameters. Here's an example:
+To read a file, use the `with` statement & specify the file name & mode as the `Fileaccess` class parameters. Here's an example:
 
 ```python
 with Fileaccess("filename.txt", "r") as file:
     for line in file:
         print(line)
 ```
 
 ### Writing to a File
-To write to a file, use the `with` statement and specify the file name and mode as the `Fileaccess` class parameters. Here's an example:
+To write to a file, use the `with` statement & specify the file name & mode as the `Fileaccess` class parameters. Here's an example:
 
 ```python
 with Fileaccess("filename.txt", "w") as file:
     file.write("Hello World")
 ```
 
 ### Appending to a File
-To append to a file, use the `with` statement and specify the file name and mode as the `Fileaccess` class parameters. Here's an example:
+To append to a file, use the `with` statement & specify the file name & mode as the `Fileaccess` class parameters. Here's an example:
 
 ```python
 with Fileaccess("filename.txt", "a") as file:
     file.write("Hello World")
 ```
 
 ### Creating a File or Directory
 To create a file or directory, use the `createFile` method of the `Fileaccess` class. Here's an example:
 
 ```python
 Fileaccess.createFile(assetType="f", targetPath="/path/to/file.txt", fileContents="File contents")
 ```
 
-In the above example, `assetType` can be either `"f"` to create a file or `"d"` to create a directory. The `targetPath` parameter specifies the path where the file or directory will be created. The `fileContents` parameter is optional and can be used to specify the contents of the file.
+In the above example, `assetType` can be either `"f"` to create a file or `"d"` to create a directory. The `targetPath` parameter specifies the path where the file or directory will be created. The `fileContents` parameter is optional & can be used to specify the contents of the file.
   
 Note: You do NOT need to first create the directory path for a file if the directory path doesn't exist (all you need are access permissions for the user python is running as). The full directory path will automatically be create for you simply by you providing a full file path.
   
 
 ## File Access Modes
 The `mode` parameter in the `Fileaccess` class specifies the file access mode. Here's a table of the available modes:
 
@@ -70,14 +72,14 @@
 | --- | --- |
 | `r` | Open for reading (default) |
 | `w` | Open for writing, truncating the file first |
 | `x` | Open for exclusive creation, failing if the file already exists |
 | `a` | Open for writing, appending to the end of file if it exists |
 | `b` | Binary mode |
 | `t` | Text mode (default) |
-| `+` | Open for updating (reading and writing) |
+| `+` | Open for updating (reading & writing) |
 
 ## Error Handling
-If an error occurs while using the `Fileaccess` class, it will be caught and printed to the console. This can be useful for debugging purposes.
+If an error occurs while using the `Fileaccess` class, it will be caught & printed to the console. This can be useful for debugging purposes.
 
 ## License
 This code is licensed under the MIT License. See the `LICENSE` file for more information.
```

### Comparing `fileaccess-0.2.13/README.md` & `fileaccess-0.2.16/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 # Fileaccess Utility Class
 
 ## Introduction
 `Fileaccess` is a utility class for safely dealing with files. This class can be used to read, write, or append to a file, as well as create a file or directory. A nice benefit of using it is the automatic file handle management it provides.  
 
-The main productivity benefit of using this class is the createFile() method which creates file and directory paths automatically for a given file or directory asset, as well as allowing the writing of file contents together in a single method call. If you find yourself writing out a directory tree or a lot of files, this can save you frustration.  
+The main productivity benefit of using this class is the createFile() method which creates file & directory paths automatically for a given file or directory asset, as well as allowing the writing of file contents together in a single method call.  
+
+If you find yourself writing out a directory tree or a lot of files, this can save you time *(binary bytes or text are auto-detected & correctly written)*.  
 
 ## Usage
 ### Reading a File
-To read a file, use the `with` statement and specify the file name and mode as the `Fileaccess` class parameters. Here's an example:
+To read a file, use the `with` statement & specify the file name & mode as the `Fileaccess` class parameters. Here's an example:
 
 ```python
 with Fileaccess("filename.txt", "r") as file:
     for line in file:
         print(line)
 ```
 
 ### Writing to a File
-To write to a file, use the `with` statement and specify the file name and mode as the `Fileaccess` class parameters. Here's an example:
+To write to a file, use the `with` statement & specify the file name & mode as the `Fileaccess` class parameters. Here's an example:
 
 ```python
 with Fileaccess("filename.txt", "w") as file:
     file.write("Hello World")
 ```
 
 ### Appending to a File
-To append to a file, use the `with` statement and specify the file name and mode as the `Fileaccess` class parameters. Here's an example:
+To append to a file, use the `with` statement & specify the file name & mode as the `Fileaccess` class parameters. Here's an example:
 
 ```python
 with Fileaccess("filename.txt", "a") as file:
     file.write("Hello World")
 ```
 
 ### Creating a File or Directory
 To create a file or directory, use the `createFile` method of the `Fileaccess` class. Here's an example:
 
 ```python
 Fileaccess.createFile(assetType="f", targetPath="/path/to/file.txt", fileContents="File contents")
 ```
 
-In the above example, `assetType` can be either `"f"` to create a file or `"d"` to create a directory. The `targetPath` parameter specifies the path where the file or directory will be created. The `fileContents` parameter is optional and can be used to specify the contents of the file.
+In the above example, `assetType` can be either `"f"` to create a file or `"d"` to create a directory. The `targetPath` parameter specifies the path where the file or directory will be created. The `fileContents` parameter is optional & can be used to specify the contents of the file.
   
 Note: You do NOT need to first create the directory path for a file if the directory path doesn't exist (all you need are access permissions for the user python is running as). The full directory path will automatically be create for you simply by you providing a full file path.
   
 
 ## File Access Modes
 The `mode` parameter in the `Fileaccess` class specifies the file access mode. Here's a table of the available modes:
 
@@ -50,14 +52,14 @@
 | --- | --- |
 | `r` | Open for reading (default) |
 | `w` | Open for writing, truncating the file first |
 | `x` | Open for exclusive creation, failing if the file already exists |
 | `a` | Open for writing, appending to the end of file if it exists |
 | `b` | Binary mode |
 | `t` | Text mode (default) |
-| `+` | Open for updating (reading and writing) |
+| `+` | Open for updating (reading & writing) |
 
 ## Error Handling
-If an error occurs while using the `Fileaccess` class, it will be caught and printed to the console. This can be useful for debugging purposes.
+If an error occurs while using the `Fileaccess` class, it will be caught & printed to the console. This can be useful for debugging purposes.
 
 ## License
 This code is licensed under the MIT License. See the `LICENSE` file for more information.
```

### Comparing `fileaccess-0.2.13/fileaccess/__init__.py` & `fileaccess-0.2.16/fileaccess/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         if os.path.exists(file_name):
             self.file_name = file_name
         else:
             raise Exception(f"Filename parameter must be a valid file path")
         if mode in ['r', 'w', 'a']:
             self.mode = mode
         else:
-            raise Exception(f"Passed mode must be one of r = read, w = write, a = append, instead found: {mode}")
+            raise Exception(f"Passed mode must be commonly one of r = read, w = write, a = append, or one of [r,w,x,a,b,t,+]. Instead found: {mode}")
 
     def __enter__(self):
         self.file = open(self.file_name, self.mode)
         return self.file
 
     def __exit__(self, exc_type, exc_value, tb):
         self.file.close()
@@ -92,9 +92,10 @@
             targetPathArray = fileAsset.split("/")
             targetPathArray.pop()
             fileAssetContainingDir = "/".join(targetPathArray)
             sh.mkdir("-p", fileAssetContainingDir)
             sh.touch(fileAsset)
             sh.chmod(filePermissions, fileAsset)
             if os.path.exists(fileAsset) and fileContents is not None:
-                with open(fileAsset, "wt") as fileHandle:
+                writeMode = 'wb' if isinstance(fileContents, bytes) else 'wt'
+                with open(fileAsset, writeMode) as fileHandle:
                     fileHandle.write(fileContents)
```

### Comparing `fileaccess-0.2.13/fileaccess.egg-info/PKG-INFO` & `fileaccess-0.2.16/fileaccess.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: fileaccess
-Version: 0.2.13
+Version: 0.2.16
 Summary: A package for easier file access, automatically closes opened file handles, & provides for simple file/directory creation.
 Home-page: https://github.com/node0/Fileaccess
 Author: Joe Hacobian
 Author-email: joehacobian@gmail.com
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -19,50 +19,52 @@
 License-File: LICENSE
 
 # Fileaccess Utility Class
 
 ## Introduction
 `Fileaccess` is a utility class for safely dealing with files. This class can be used to read, write, or append to a file, as well as create a file or directory. A nice benefit of using it is the automatic file handle management it provides.  
 
-The main productivity benefit of using this class is the createFile() method which creates file and directory paths automatically for a given file or directory asset, as well as allowing the writing of file contents together in a single method call. If you find yourself writing out a directory tree or a lot of files, this can save you frustration.  
+The main productivity benefit of using this class is the createFile() method which creates file & directory paths automatically for a given file or directory asset, as well as allowing the writing of file contents together in a single method call.  
+
+If you find yourself writing out a directory tree or a lot of files, this can save you time *(binary bytes or text are auto-detected & correctly written)*.  
 
 ## Usage
 ### Reading a File
-To read a file, use the `with` statement and specify the file name and mode as the `Fileaccess` class parameters. Here's an example:
+To read a file, use the `with` statement & specify the file name & mode as the `Fileaccess` class parameters. Here's an example:
 
 ```python
 with Fileaccess("filename.txt", "r") as file:
     for line in file:
         print(line)
 ```
 
 ### Writing to a File
-To write to a file, use the `with` statement and specify the file name and mode as the `Fileaccess` class parameters. Here's an example:
+To write to a file, use the `with` statement & specify the file name & mode as the `Fileaccess` class parameters. Here's an example:
 
 ```python
 with Fileaccess("filename.txt", "w") as file:
     file.write("Hello World")
 ```
 
 ### Appending to a File
-To append to a file, use the `with` statement and specify the file name and mode as the `Fileaccess` class parameters. Here's an example:
+To append to a file, use the `with` statement & specify the file name & mode as the `Fileaccess` class parameters. Here's an example:
 
 ```python
 with Fileaccess("filename.txt", "a") as file:
     file.write("Hello World")
 ```
 
 ### Creating a File or Directory
 To create a file or directory, use the `createFile` method of the `Fileaccess` class. Here's an example:
 
 ```python
 Fileaccess.createFile(assetType="f", targetPath="/path/to/file.txt", fileContents="File contents")
 ```
 
-In the above example, `assetType` can be either `"f"` to create a file or `"d"` to create a directory. The `targetPath` parameter specifies the path where the file or directory will be created. The `fileContents` parameter is optional and can be used to specify the contents of the file.
+In the above example, `assetType` can be either `"f"` to create a file or `"d"` to create a directory. The `targetPath` parameter specifies the path where the file or directory will be created. The `fileContents` parameter is optional & can be used to specify the contents of the file.
   
 Note: You do NOT need to first create the directory path for a file if the directory path doesn't exist (all you need are access permissions for the user python is running as). The full directory path will automatically be create for you simply by you providing a full file path.
   
 
 ## File Access Modes
 The `mode` parameter in the `Fileaccess` class specifies the file access mode. Here's a table of the available modes:
 
@@ -70,14 +72,14 @@
 | --- | --- |
 | `r` | Open for reading (default) |
 | `w` | Open for writing, truncating the file first |
 | `x` | Open for exclusive creation, failing if the file already exists |
 | `a` | Open for writing, appending to the end of file if it exists |
 | `b` | Binary mode |
 | `t` | Text mode (default) |
-| `+` | Open for updating (reading and writing) |
+| `+` | Open for updating (reading & writing) |
 
 ## Error Handling
-If an error occurs while using the `Fileaccess` class, it will be caught and printed to the console. This can be useful for debugging purposes.
+If an error occurs while using the `Fileaccess` class, it will be caught & printed to the console. This can be useful for debugging purposes.
 
 ## License
 This code is licensed under the MIT License. See the `LICENSE` file for more information.
```

### Comparing `fileaccess-0.2.13/setup.py` & `fileaccess-0.2.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fileaccess",
-    version="0.2.13",
+    version="0.2.16",
     packages=find_packages(),
     install_requires=[
         "sh"
     ],
     author="Joe Hacobian",
     author_email="joehacobian@gmail.com",
     description="A package for easier file access, automatically closes opened file handles, & provides for simple file/directory creation.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/node0/Fileaccess",
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

