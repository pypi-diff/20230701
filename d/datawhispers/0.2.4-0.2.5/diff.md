# Comparing `tmp/datawhispers-0.2.4.tar.gz` & `tmp/datawhispers-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawhispers-0.2.4.tar", last modified: Sat Jul  1 13:17:38 2023, max compression
+gzip compressed data, was "datawhispers-0.2.5.tar", last modified: Sat Jul  1 13:33:43 2023, max compression
```

## Comparing `datawhispers-0.2.4.tar` & `datawhispers-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-01 13:17:38.642042 datawhispers-0.2.4/
--rw-r--r--   0 german     (501) staff       (20)     1061 2023-07-01 09:46:39.000000 datawhispers-0.2.4/LICENSE
--rw-r--r--   0 german     (501) staff       (20)     1079 2023-07-01 13:17:38.641924 datawhispers-0.2.4/PKG-INFO
--rw-r--r--   0 german     (501) staff       (20)      436 2023-07-01 11:20:15.000000 datawhispers-0.2.4/README.md
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-01 13:17:38.640890 datawhispers-0.2.4/datawhispers/
--rw-r--r--   0 german     (501) staff       (20)       75 2023-07-01 10:41:44.000000 datawhispers-0.2.4/datawhispers/__init__.py
--rw-r--r--   0 german     (501) staff       (20)     7938 2023-07-01 13:17:01.000000 datawhispers-0.2.4/datawhispers/advanced_prog.py
--rw-r--r--   0 german     (501) staff       (20)     7569 2023-07-01 09:48:05.000000 datawhispers-0.2.4/datawhispers/datavis.py
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-01 13:17:38.641739 datawhispers-0.2.4/datawhispers.egg-info/
--rw-r--r--   0 german     (501) staff       (20)     1079 2023-07-01 13:17:38.000000 datawhispers-0.2.4/datawhispers.egg-info/PKG-INFO
--rw-r--r--   0 german     (501) staff       (20)      284 2023-07-01 13:17:38.000000 datawhispers-0.2.4/datawhispers.egg-info/SOURCES.txt
--rw-r--r--   0 german     (501) staff       (20)        1 2023-07-01 13:17:38.000000 datawhispers-0.2.4/datawhispers.egg-info/dependency_links.txt
--rw-r--r--   0 german     (501) staff       (20)       38 2023-07-01 13:17:38.000000 datawhispers-0.2.4/datawhispers.egg-info/requires.txt
--rw-r--r--   0 german     (501) staff       (20)       13 2023-07-01 13:17:38.000000 datawhispers-0.2.4/datawhispers.egg-info/top_level.txt
--rw-r--r--   0 german     (501) staff       (20)       38 2023-07-01 13:17:38.642090 datawhispers-0.2.4/setup.cfg
--rw-r--r--   0 german     (501) staff       (20)     2059 2023-07-01 13:17:18.000000 datawhispers-0.2.4/setup.py
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-01 13:33:43.948496 datawhispers-0.2.5/
+-rw-r--r--   0 german     (501) staff       (20)     1061 2023-07-01 09:46:39.000000 datawhispers-0.2.5/LICENSE
+-rw-r--r--   0 german     (501) staff       (20)     1079 2023-07-01 13:33:43.948370 datawhispers-0.2.5/PKG-INFO
+-rw-r--r--   0 german     (501) staff       (20)      436 2023-07-01 11:20:15.000000 datawhispers-0.2.5/README.md
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-01 13:33:43.947333 datawhispers-0.2.5/datawhispers/
+-rw-r--r--   0 german     (501) staff       (20)       75 2023-07-01 10:41:44.000000 datawhispers-0.2.5/datawhispers/__init__.py
+-rw-r--r--   0 german     (501) staff       (20)     7949 2023-07-01 13:33:20.000000 datawhispers-0.2.5/datawhispers/advanced_prog.py
+-rw-r--r--   0 german     (501) staff       (20)     7569 2023-07-01 09:48:05.000000 datawhispers-0.2.5/datawhispers/datavis.py
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-01 13:33:43.948128 datawhispers-0.2.5/datawhispers.egg-info/
+-rw-r--r--   0 german     (501) staff       (20)     1079 2023-07-01 13:33:43.000000 datawhispers-0.2.5/datawhispers.egg-info/PKG-INFO
+-rw-r--r--   0 german     (501) staff       (20)      284 2023-07-01 13:33:43.000000 datawhispers-0.2.5/datawhispers.egg-info/SOURCES.txt
+-rw-r--r--   0 german     (501) staff       (20)        1 2023-07-01 13:33:43.000000 datawhispers-0.2.5/datawhispers.egg-info/dependency_links.txt
+-rw-r--r--   0 german     (501) staff       (20)       38 2023-07-01 13:33:43.000000 datawhispers-0.2.5/datawhispers.egg-info/requires.txt
+-rw-r--r--   0 german     (501) staff       (20)       13 2023-07-01 13:33:43.000000 datawhispers-0.2.5/datawhispers.egg-info/top_level.txt
+-rw-r--r--   0 german     (501) staff       (20)       38 2023-07-01 13:33:43.948541 datawhispers-0.2.5/setup.cfg
+-rw-r--r--   0 german     (501) staff       (20)     2059 2023-07-01 13:33:32.000000 datawhispers-0.2.5/setup.py
```

### Comparing `datawhispers-0.2.4/LICENSE` & `datawhispers-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `datawhispers-0.2.4/PKG-INFO` & `datawhispers-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawhispers
-Version: 0.2.4
+Version: 0.2.5
 Summary: This is a library to solve regression problems or statistical analysis for the DHBW Mannheim courses Advanced Programming and Data Visualisation
 Home-page: https://github.com/GermanPaul12/datawhispers
 Download-URL: https://github.com/GermanPaul12/datawhispers/archive/v_01.tar.gz
 Author: German Paul
 Author-email: motets-rosiest-0r@icloud.com
 License: MIT
 Keywords: Python3,Data Visualisation,Statistical Analysis,Regression,Advanced Programming
```

### Comparing `datawhispers-0.2.4/datawhispers/advanced_prog.py` & `datawhispers-0.2.5/datawhispers/advanced_prog.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     '''Time series exponential regression. 
     '''
     coef_first_step = linReg(x_in,np.log(y))
     b = coef_first_step[0]
     a = np.exp(coef_first_step[1])
     return [a,b]
 
-def pred(ansatz, coef, x_in, freeRegAnsatz=None):
+def predict(ansatz, coef, x_in, freeRegAnsatz=None):
     '''Computes the predction for input x_in and the computed corresponding
        coefficients
     ''' 
         
     if ansatz == 'linReg' or ansatz == 'polReg':
         values = np.poly1d(coef)(x_in)     
             
@@ -215,15 +215,15 @@
     
     
     def pred(self, x):
         '''Computes the predction for input x and the computed corresponding
            coefficients
         ''' 
         
-        values = pred(self.ansatz, self.coef, x)            
+        values = predict(self.ansatz, self.coef, x)            
         
     
         return  values      
 
     
     def r2(self):
         '''Computes the coefficient of determination for the training input
@@ -231,15 +231,15 @@
         wert=r2(self.y, self.pred(self.x))
         return round(wert, 4)        
     
     
     def make_easy_plot(self, file_name):
         '''Shows a plot of the data, the regression and saves the plot
         '''
-        make_plot(self.x, self.y, self.pred(x), name=file_name)
+        make_plot(x=self.x, y=self.y, y_reg=predict(self.ansatz, self.coef, self.x), name=file_name)
         print(f"r2: {self.r2}, coefs: {self.coef}")
     
     
 def plot_all_regs(x,y, xticks=None, yticks=None):
     model = Trend(x,y,"linReg")
     plt.title("Linear Regression");
     y_reg = model.pred(x)
@@ -260,12 +260,8 @@
     print(f"Coefs: {model.coef}, r2: {model.r2}")   
     
     model = Trend(x,y,"expReg")
     plt.title("Exponential Regression");
     y_reg = model.pred(x)
     make_plot(x,y,y_reg, name="exp_reg.png");
     print(f"Coefs: {model.coef}, r2: {model.r2}")   
-        
-        
-    
-
```

### Comparing `datawhispers-0.2.4/datawhispers/datavis.py` & `datawhispers-0.2.5/datawhispers/datavis.py`

 * *Files identical despite different names*

### Comparing `datawhispers-0.2.4/datawhispers.egg-info/PKG-INFO` & `datawhispers-0.2.5/datawhispers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawhispers
-Version: 0.2.4
+Version: 0.2.5
 Summary: This is a library to solve regression problems or statistical analysis for the DHBW Mannheim courses Advanced Programming and Data Visualisation
 Home-page: https://github.com/GermanPaul12/datawhispers
 Download-URL: https://github.com/GermanPaul12/datawhispers/archive/v_01.tar.gz
 Author: German Paul
 Author-email: motets-rosiest-0r@icloud.com
 License: MIT
 Keywords: Python3,Data Visualisation,Statistical Analysis,Regression,Advanced Programming
```

### Comparing `datawhispers-0.2.4/setup.py` & `datawhispers-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'datawhispers',         # How you named your package folder (MyLib)
   packages = ["datawhispers"],   # Chose the same as "name"
-  version = '0.2.4',      # Start with a small number and increase it with every change you make
+  version = '0.2.5',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'This is a library to solve regression problems or statistical analysis for the DHBW Mannheim courses Advanced Programming and Data Visualisation',   # Give a short description about your library
   author = 'German Paul',                   # Type in your name
   author_email = 'motets-rosiest-0r@icloud.com',      # Type in your E-Mail
   url = 'https://github.com/GermanPaul12/datawhispers',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/GermanPaul12/datawhispers/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['Python3', 'Data Visualisation', 'Statistical Analysis', "Regression", "Advanced Programming"],   # Keywords that define your package best
```

