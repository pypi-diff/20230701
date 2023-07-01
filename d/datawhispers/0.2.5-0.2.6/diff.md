# Comparing `tmp/datawhispers-0.2.5.tar.gz` & `tmp/datawhispers-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawhispers-0.2.5.tar", last modified: Sat Jul  1 13:33:43 2023, max compression
+gzip compressed data, was "datawhispers-0.2.6.tar", last modified: Sat Jul  1 13:49:58 2023, max compression
```

## Comparing `datawhispers-0.2.5.tar` & `datawhispers-0.2.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-01 13:33:43.948496 datawhispers-0.2.5/
--rw-r--r--   0 german     (501) staff       (20)     1061 2023-07-01 09:46:39.000000 datawhispers-0.2.5/LICENSE
--rw-r--r--   0 german     (501) staff       (20)     1079 2023-07-01 13:33:43.948370 datawhispers-0.2.5/PKG-INFO
--rw-r--r--   0 german     (501) staff       (20)      436 2023-07-01 11:20:15.000000 datawhispers-0.2.5/README.md
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-01 13:33:43.947333 datawhispers-0.2.5/datawhispers/
--rw-r--r--   0 german     (501) staff       (20)       75 2023-07-01 10:41:44.000000 datawhispers-0.2.5/datawhispers/__init__.py
--rw-r--r--   0 german     (501) staff       (20)     7949 2023-07-01 13:33:20.000000 datawhispers-0.2.5/datawhispers/advanced_prog.py
--rw-r--r--   0 german     (501) staff       (20)     7569 2023-07-01 09:48:05.000000 datawhispers-0.2.5/datawhispers/datavis.py
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-01 13:33:43.948128 datawhispers-0.2.5/datawhispers.egg-info/
--rw-r--r--   0 german     (501) staff       (20)     1079 2023-07-01 13:33:43.000000 datawhispers-0.2.5/datawhispers.egg-info/PKG-INFO
--rw-r--r--   0 german     (501) staff       (20)      284 2023-07-01 13:33:43.000000 datawhispers-0.2.5/datawhispers.egg-info/SOURCES.txt
--rw-r--r--   0 german     (501) staff       (20)        1 2023-07-01 13:33:43.000000 datawhispers-0.2.5/datawhispers.egg-info/dependency_links.txt
--rw-r--r--   0 german     (501) staff       (20)       38 2023-07-01 13:33:43.000000 datawhispers-0.2.5/datawhispers.egg-info/requires.txt
--rw-r--r--   0 german     (501) staff       (20)       13 2023-07-01 13:33:43.000000 datawhispers-0.2.5/datawhispers.egg-info/top_level.txt
--rw-r--r--   0 german     (501) staff       (20)       38 2023-07-01 13:33:43.948541 datawhispers-0.2.5/setup.cfg
--rw-r--r--   0 german     (501) staff       (20)     2059 2023-07-01 13:33:32.000000 datawhispers-0.2.5/setup.py
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-01 13:49:58.376687 datawhispers-0.2.6/
+-rw-r--r--   0 german     (501) staff       (20)     1061 2023-07-01 09:46:39.000000 datawhispers-0.2.6/LICENSE
+-rw-r--r--   0 german     (501) staff       (20)     1079 2023-07-01 13:49:58.376561 datawhispers-0.2.6/PKG-INFO
+-rw-r--r--   0 german     (501) staff       (20)      436 2023-07-01 11:20:15.000000 datawhispers-0.2.6/README.md
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-01 13:49:58.375457 datawhispers-0.2.6/datawhispers/
+-rw-r--r--   0 german     (501) staff       (20)       75 2023-07-01 10:41:44.000000 datawhispers-0.2.6/datawhispers/__init__.py
+-rw-r--r--   0 german     (501) staff       (20)     8342 2023-07-01 13:49:41.000000 datawhispers-0.2.6/datawhispers/advanced_prog.py
+-rw-r--r--   0 german     (501) staff       (20)     7569 2023-07-01 09:48:05.000000 datawhispers-0.2.6/datawhispers/datavis.py
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-01 13:49:58.376356 datawhispers-0.2.6/datawhispers.egg-info/
+-rw-r--r--   0 german     (501) staff       (20)     1079 2023-07-01 13:49:58.000000 datawhispers-0.2.6/datawhispers.egg-info/PKG-INFO
+-rw-r--r--   0 german     (501) staff       (20)      284 2023-07-01 13:49:58.000000 datawhispers-0.2.6/datawhispers.egg-info/SOURCES.txt
+-rw-r--r--   0 german     (501) staff       (20)        1 2023-07-01 13:49:58.000000 datawhispers-0.2.6/datawhispers.egg-info/dependency_links.txt
+-rw-r--r--   0 german     (501) staff       (20)       38 2023-07-01 13:49:58.000000 datawhispers-0.2.6/datawhispers.egg-info/requires.txt
+-rw-r--r--   0 german     (501) staff       (20)       13 2023-07-01 13:49:58.000000 datawhispers-0.2.6/datawhispers.egg-info/top_level.txt
+-rw-r--r--   0 german     (501) staff       (20)       38 2023-07-01 13:49:58.376729 datawhispers-0.2.6/setup.cfg
+-rw-r--r--   0 german     (501) staff       (20)     2059 2023-07-01 13:49:51.000000 datawhispers-0.2.6/setup.py
```

### Comparing `datawhispers-0.2.5/LICENSE` & `datawhispers-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `datawhispers-0.2.5/PKG-INFO` & `datawhispers-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawhispers
-Version: 0.2.5
+Version: 0.2.6
 Summary: This is a library to solve regression problems or statistical analysis for the DHBW Mannheim courses Advanced Programming and Data Visualisation
 Home-page: https://github.com/GermanPaul12/datawhispers
 Download-URL: https://github.com/GermanPaul12/datawhispers/archive/v_01.tar.gz
 Author: German Paul
 Author-email: motets-rosiest-0r@icloud.com
 License: MIT
 Keywords: Python3,Data Visualisation,Statistical Analysis,Regression,Advanced Programming
```

### Comparing `datawhispers-0.2.5/datawhispers/advanced_prog.py` & `datawhispers-0.2.6/datawhispers/advanced_prog.py`

 * *Files 5% similar despite different names*

```diff
@@ -125,32 +125,39 @@
 
 
 def show_mnist_from_array(arr):    
     """
     Returns the image of the mnist number and saves it as mnist_num.png
     arr: array of shape (784,) or (28,28)
     """
+    label = ''
+    if arr.shape == (785,): label,arr = arr[0],arr[1:].reshape((28, 28))
     if arr.shape == (784,):   
         arr = arr.reshape((28, 28))
     # Plot
+    plt.title(f"MNIST Number {label}")
     plt.imshow(arr, cmap='gray')
-    plt.savefig("mnist_num.png")
+    plt.savefig("mnist_num.png", dpi=1200)
     plt.show()
     
 
 def show_mnist_from_file(filepath):    
     with open(filepath) as f: 
         try:
+            label = ""
             for i in f:
                 if "," in i:   
                     arr = np.array([int(num) for num in i.split(",")])
+                    if arr.shape == (785,): label,arr = arr[0],arr[1:].reshape((28, 28))
                     if arr.shape == (784,): arr = arr.reshape((28, 28))
                 else:    
                     arr = np.array([int(num) for num in i.split(";")])
+                    if arr.shape == (785,): label,arr = arr[0],arr[1:].reshape((28, 28))
                     if arr.shape == (784,): arr = arr.reshape((28, 28))
+                plt.title(f"MNIST Number {label}")    
                 plt.imshow(arr, cmap="gray")
                 plt.show()   
         except Exception as e:
             print("Sorry try the func 'show_mnist_from_array' because your file does not seem to work with this method")         
 
 
 def add_mnist_num_arrays(num1,num2):
```

### Comparing `datawhispers-0.2.5/datawhispers/datavis.py` & `datawhispers-0.2.6/datawhispers/datavis.py`

 * *Files identical despite different names*

### Comparing `datawhispers-0.2.5/datawhispers.egg-info/PKG-INFO` & `datawhispers-0.2.6/datawhispers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawhispers
-Version: 0.2.5
+Version: 0.2.6
 Summary: This is a library to solve regression problems or statistical analysis for the DHBW Mannheim courses Advanced Programming and Data Visualisation
 Home-page: https://github.com/GermanPaul12/datawhispers
 Download-URL: https://github.com/GermanPaul12/datawhispers/archive/v_01.tar.gz
 Author: German Paul
 Author-email: motets-rosiest-0r@icloud.com
 License: MIT
 Keywords: Python3,Data Visualisation,Statistical Analysis,Regression,Advanced Programming
```

### Comparing `datawhispers-0.2.5/setup.py` & `datawhispers-0.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'datawhispers',         # How you named your package folder (MyLib)
   packages = ["datawhispers"],   # Chose the same as "name"
-  version = '0.2.5',      # Start with a small number and increase it with every change you make
+  version = '0.2.6',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'This is a library to solve regression problems or statistical analysis for the DHBW Mannheim courses Advanced Programming and Data Visualisation',   # Give a short description about your library
   author = 'German Paul',                   # Type in your name
   author_email = 'motets-rosiest-0r@icloud.com',      # Type in your E-Mail
   url = 'https://github.com/GermanPaul12/datawhispers',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/GermanPaul12/datawhispers/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['Python3', 'Data Visualisation', 'Statistical Analysis', "Regression", "Advanced Programming"],   # Keywords that define your package best
```

