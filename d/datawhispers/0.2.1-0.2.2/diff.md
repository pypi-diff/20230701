# Comparing `tmp/datawhispers-0.2.1.tar.gz` & `tmp/datawhispers-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawhispers-0.2.1.tar", last modified: Sat Jul  1 11:20:37 2023, max compression
+gzip compressed data, was "datawhispers-0.2.2.tar", last modified: Sat Jul  1 12:58:33 2023, max compression
```

## Comparing `datawhispers-0.2.1.tar` & `datawhispers-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-01 11:20:37.775925 datawhispers-0.2.1/
--rw-r--r--   0 german     (501) staff       (20)     1061 2023-07-01 09:46:39.000000 datawhispers-0.2.1/LICENSE
--rw-r--r--   0 german     (501) staff       (20)     1079 2023-07-01 11:20:37.775777 datawhispers-0.2.1/PKG-INFO
--rw-r--r--   0 german     (501) staff       (20)      436 2023-07-01 11:20:15.000000 datawhispers-0.2.1/README.md
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-01 11:20:37.774752 datawhispers-0.2.1/datawhispers/
--rw-r--r--   0 german     (501) staff       (20)       75 2023-07-01 10:41:44.000000 datawhispers-0.2.1/datawhispers/__init__.py
--rw-r--r--   0 german     (501) staff       (20)     6015 2023-07-01 11:19:29.000000 datawhispers-0.2.1/datawhispers/advanced_prog.py
--rw-r--r--   0 german     (501) staff       (20)     7569 2023-07-01 09:48:05.000000 datawhispers-0.2.1/datawhispers/datavis.py
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-01 11:20:37.775545 datawhispers-0.2.1/datawhispers.egg-info/
--rw-r--r--   0 german     (501) staff       (20)     1079 2023-07-01 11:20:37.000000 datawhispers-0.2.1/datawhispers.egg-info/PKG-INFO
--rw-r--r--   0 german     (501) staff       (20)      284 2023-07-01 11:20:37.000000 datawhispers-0.2.1/datawhispers.egg-info/SOURCES.txt
--rw-r--r--   0 german     (501) staff       (20)        1 2023-07-01 11:20:37.000000 datawhispers-0.2.1/datawhispers.egg-info/dependency_links.txt
--rw-r--r--   0 german     (501) staff       (20)       38 2023-07-01 11:20:37.000000 datawhispers-0.2.1/datawhispers.egg-info/requires.txt
--rw-r--r--   0 german     (501) staff       (20)       13 2023-07-01 11:20:37.000000 datawhispers-0.2.1/datawhispers.egg-info/top_level.txt
--rw-r--r--   0 german     (501) staff       (20)       38 2023-07-01 11:20:37.775970 datawhispers-0.2.1/setup.cfg
--rw-r--r--   0 german     (501) staff       (20)     2059 2023-07-01 11:20:27.000000 datawhispers-0.2.1/setup.py
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-01 12:58:33.884387 datawhispers-0.2.2/
+-rw-r--r--   0 german     (501) staff       (20)     1061 2023-07-01 09:46:39.000000 datawhispers-0.2.2/LICENSE
+-rw-r--r--   0 german     (501) staff       (20)     1079 2023-07-01 12:58:33.884261 datawhispers-0.2.2/PKG-INFO
+-rw-r--r--   0 german     (501) staff       (20)      436 2023-07-01 11:20:15.000000 datawhispers-0.2.2/README.md
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-01 12:58:33.883200 datawhispers-0.2.2/datawhispers/
+-rw-r--r--   0 german     (501) staff       (20)       75 2023-07-01 10:41:44.000000 datawhispers-0.2.2/datawhispers/__init__.py
+-rw-r--r--   0 german     (501) staff       (20)     7688 2023-07-01 12:58:12.000000 datawhispers-0.2.2/datawhispers/advanced_prog.py
+-rw-r--r--   0 german     (501) staff       (20)     7569 2023-07-01 09:48:05.000000 datawhispers-0.2.2/datawhispers/datavis.py
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-01 12:58:33.884046 datawhispers-0.2.2/datawhispers.egg-info/
+-rw-r--r--   0 german     (501) staff       (20)     1079 2023-07-01 12:58:33.000000 datawhispers-0.2.2/datawhispers.egg-info/PKG-INFO
+-rw-r--r--   0 german     (501) staff       (20)      284 2023-07-01 12:58:33.000000 datawhispers-0.2.2/datawhispers.egg-info/SOURCES.txt
+-rw-r--r--   0 german     (501) staff       (20)        1 2023-07-01 12:58:33.000000 datawhispers-0.2.2/datawhispers.egg-info/dependency_links.txt
+-rw-r--r--   0 german     (501) staff       (20)       38 2023-07-01 12:58:33.000000 datawhispers-0.2.2/datawhispers.egg-info/requires.txt
+-rw-r--r--   0 german     (501) staff       (20)       13 2023-07-01 12:58:33.000000 datawhispers-0.2.2/datawhispers.egg-info/top_level.txt
+-rw-r--r--   0 german     (501) staff       (20)       38 2023-07-01 12:58:33.884434 datawhispers-0.2.2/setup.cfg
+-rw-r--r--   0 german     (501) staff       (20)     2059 2023-07-01 12:58:25.000000 datawhispers-0.2.2/setup.py
```

### Comparing `datawhispers-0.2.1/LICENSE` & `datawhispers-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datawhispers-0.2.1/PKG-INFO` & `datawhispers-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawhispers
-Version: 0.2.1
+Version: 0.2.2
 Summary: This is a library to solve regression problems or statistical analysis for the DHBW Mannheim courses Advanced Programming and Data Visualisation
 Home-page: https://github.com/GermanPaul12/datawhispers
 Download-URL: https://github.com/GermanPaul12/datawhispers/archive/v_01.tar.gz
 Author: German Paul
 Author-email: motets-rosiest-0r@icloud.com
 License: MIT
 Keywords: Python3,Data Visualisation,Statistical Analysis,Regression,Advanced Programming
```

### Comparing `datawhispers-0.2.1/datawhispers/advanced_prog.py` & `datawhispers-0.2.2/datawhispers/advanced_prog.py`

 * *Files 22% similar despite different names*

```diff
@@ -103,45 +103,60 @@
     o = len(coeffs)
     print(f'# This is a polynomial of order {o}.')
     y = 0
     for i in range(o):
         y += coeffs[i]*x**i
     return y
 
-def make_plot(x,y,y_reg, xticks=[], yticks=[],xlabel="x", ylabel="y", colors=["lightblue", "black"]):
+def make_plot(x,y,y_reg, xticks=[], yticks=[],xlabel="x", ylabel="y", colors=["lightblue", "black"], name="fig_reg.png"):
     '''
     Outputs a graph for (x and y) and (x and y_reg) and saves it as fig_reg.png
     x: array with x-values
     y: array with y-values
     y_reg: array with regression y_values
     '''
     plt.plot(x,y_reg,color=colors[1]);
     plt.scatter(x,y, color=colors[0]);
     plt.xlabel(xlabel) 
     plt.ylabel(ylabel)
     if xticks: plt.xticks(xticks);
     if yticks: plt.yticks(yticks);
-    plt.savefig("fig_reg.png");    
+    plt.savefig(f"{name}");  
     plt.show()
 
 
 def show_mnist_from_array(arr):    
     """
     Returns the image of the mnist number and saves it as mnist_num.png
     arr: array of shape (784,) or (28,28)
     """
     if arr.shape == (784,):   
         arr = arr.reshape((28, 28))
     # Plot
     plt.imshow(arr, cmap='gray')
-    plt.show()
     plt.savefig("mnist_num.png")
-    
+    plt.show()
     
 
+def show_mnist_from_file(filepath):    
+    with open(filepath) as f: 
+        try:
+            for i in f:
+                if "," in i:   
+                    arr = np.array([int(num) for num in i.split(",")])
+                    if arr.shape == (784,): arr = arr.reshape((28, 28))
+                else:    
+                    arr = np.array([int(num) for num in i.split(";")])
+                    if arr.shape == (784,): arr = arr.reshape((28, 28))
+                plt.imshow(arr, cmap="gray")
+                plt.show()   
+        except Exception as e:
+            print("Sorry try the func 'show_mnist_from_array' because your file does not seem to work with this method")         
+
+
 def add_mnist_num_arrays(num1,num2):
     """
     Returns the image of the result and saves it as mnist_result.png
     arr: np.array of shape (784,) or (28,28)
     """        
     if num1.shape == (784,):
         num1 = num1.reshape((28,28))
@@ -210,8 +225,40 @@
         return  values      
 
     
     def r2(self):
         '''Computes the coefficient of determination for the training input
         ''' 
         wert=r2(self.y, self.pred(self.x))
-        return round(wert, 3)        
+        return round(wert, 4)        
+    
+    
+def plot_all_regs(x,y, xticks=None, yticks=None):
+    model = Trend(x,y,"linReg")
+    plt.title("Linear Regression");
+    y_reg = model.pred(x)
+    make_plot(x,y,y_reg, name="lin_reg_plot.png");
+    print(f"Coefs: {model.coef}, r2: {model.r2}")
+    
+    for i in range(2,10):
+        model = Trend(x,y,"polReg", deg=i)
+        plt.title(f"Polynomial Regression {i} degree");
+        y_reg = model.pred(x)
+        make_plot(x,y,y_reg, name=f"pol_reg{i}.png");
+        print(f"Coefs: {model.coef}, r2: {model.r2}")
+    
+    model = Trend(x,y,"trigReg")
+    plt.title("Trigonometric Regression");
+    y_reg = model.pred(x)
+    make_plot(x,y,y_reg, name="trig_reg.png");
+    print(f"Coefs: {model.coef}, r2: {model.r2}")   
+    
+    model = Trend(x,y,"expReg")
+    plt.title("Exponential Regression");
+    y_reg = model.pred(x)
+    make_plot(x,y,y_reg, name="exp_reg.png");
+    print(f"Coefs: {model.coef}, r2: {model.r2}")   
+        
+        
+    
+        
+
```

### Comparing `datawhispers-0.2.1/datawhispers/datavis.py` & `datawhispers-0.2.2/datawhispers/datavis.py`

 * *Files identical despite different names*

### Comparing `datawhispers-0.2.1/datawhispers.egg-info/PKG-INFO` & `datawhispers-0.2.2/datawhispers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawhispers
-Version: 0.2.1
+Version: 0.2.2
 Summary: This is a library to solve regression problems or statistical analysis for the DHBW Mannheim courses Advanced Programming and Data Visualisation
 Home-page: https://github.com/GermanPaul12/datawhispers
 Download-URL: https://github.com/GermanPaul12/datawhispers/archive/v_01.tar.gz
 Author: German Paul
 Author-email: motets-rosiest-0r@icloud.com
 License: MIT
 Keywords: Python3,Data Visualisation,Statistical Analysis,Regression,Advanced Programming
```

### Comparing `datawhispers-0.2.1/setup.py` & `datawhispers-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'datawhispers',         # How you named your package folder (MyLib)
   packages = ["datawhispers"],   # Chose the same as "name"
-  version = '0.2.1',      # Start with a small number and increase it with every change you make
+  version = '0.2.2',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'This is a library to solve regression problems or statistical analysis for the DHBW Mannheim courses Advanced Programming and Data Visualisation',   # Give a short description about your library
   author = 'German Paul',                   # Type in your name
   author_email = 'motets-rosiest-0r@icloud.com',      # Type in your E-Mail
   url = 'https://github.com/GermanPaul12/datawhispers',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/GermanPaul12/datawhispers/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['Python3', 'Data Visualisation', 'Statistical Analysis', "Regression", "Advanced Programming"],   # Keywords that define your package best
```

