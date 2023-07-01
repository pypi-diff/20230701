# Comparing `tmp/lcmtools-0.1.3.tar.gz` & `tmp/lcmtools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcmtools-0.1.3.tar", last modified: Sat Apr  1 15:03:21 2023, max compression
+gzip compressed data, was "lcmtools-0.1.5.tar", last modified: Sat Jul  1 14:53:30 2023, max compression
```

## Comparing `lcmtools-0.1.3.tar` & `lcmtools-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-01 15:03:21.657561 lcmtools-0.1.3/
--rw-rw-rw-   0        0        0     1086 2023-02-23 06:51:28.000000 lcmtools-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     1965 2023-04-01 15:03:21.656561 lcmtools-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-01 15:03:21.647558 lcmtools-0.1.3/lcmtools/
--rw-rw-rw-   0        0        0       42 2023-02-23 14:29:02.000000 lcmtools-0.1.3/lcmtools/__init__.py
--rw-rw-rw-   0        0        0      336 2023-04-01 15:03:19.000000 lcmtools-0.1.3/lcmtools/__version__.py
--rw-rw-rw-   0        0        0    11955 2023-04-01 15:02:49.000000 lcmtools-0.1.3/lcmtools/lcmtools.py
-drwxrwxrwx   0        0        0        0 2023-04-01 15:03:21.655561 lcmtools-0.1.3/lcmtools.egg-info/
--rw-rw-rw-   0        0        0     1965 2023-04-01 15:03:21.000000 lcmtools-0.1.3/lcmtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-04-01 15:03:21.000000 lcmtools-0.1.3/lcmtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-01 15:03:21.000000 lcmtools-0.1.3/lcmtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-01 15:03:21.000000 lcmtools-0.1.3/lcmtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-01 15:03:21.000000 lcmtools-0.1.3/lcmtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-01 15:03:21.657561 lcmtools-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     3924 2023-04-01 15:01:45.000000 lcmtools-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 14:53:30.111605 lcmtools-0.1.5/
+-rw-rw-rw-   0        0        0     1086 2023-02-23 06:51:28.000000 lcmtools-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     1965 2023-07-01 14:53:30.110601 lcmtools-0.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-01 14:53:30.104724 lcmtools-0.1.5/lcmtools/
+-rw-rw-rw-   0        0        0       42 2023-02-23 14:29:02.000000 lcmtools-0.1.5/lcmtools/__init__.py
+-rw-rw-rw-   0        0        0      336 2023-07-01 14:44:31.000000 lcmtools-0.1.5/lcmtools/__version__.py
+-rw-rw-rw-   0        0        0    13332 2023-07-01 14:33:16.000000 lcmtools-0.1.5/lcmtools/lcmtools.py
+drwxrwxrwx   0        0        0        0 2023-07-01 14:53:30.110097 lcmtools-0.1.5/lcmtools.egg-info/
+-rw-rw-rw-   0        0        0     1965 2023-07-01 14:53:30.000000 lcmtools-0.1.5/lcmtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-07-01 14:53:30.000000 lcmtools-0.1.5/lcmtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 14:53:30.000000 lcmtools-0.1.5/lcmtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-01 14:53:30.000000 lcmtools-0.1.5/lcmtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-01 14:53:30.000000 lcmtools-0.1.5/lcmtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 14:53:30.111605 lcmtools-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     3924 2023-07-01 14:44:39.000000 lcmtools-0.1.5/setup.py
```

### Comparing `lcmtools-0.1.3/LICENSE` & `lcmtools-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lcmtools-0.1.3/PKG-INFO` & `lcmtools-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcmtools
-Version: 0.1.3
+Version: 0.1.5
 Summary: A script that calls LCModel through Python.
 Home-page: https://github.com/luodeb/lcmtools
 Author: Luo Debin
 Author-email: luodeb@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lcmtools Version: 0.1.3 Summary: A script that
+Metadata-Version: 2.1 Name: lcmtools Version: 0.1.5 Summary: A script that
 calls LCModel through Python. Home-page: https://github.com/luodeb/lcmtools
 Author: Luo Debin Author-email: luodeb@qq.com License: MIT Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Requires-Python: >=3.6.0 Description-Content-Type: text/
```

### Comparing `lcmtools-0.1.3/lcmtools/lcmtools.py` & `lcmtools-0.1.5/lcmtools/lcmtools.py`

 * *Files 13% similar despite different names*

```diff
@@ -123,17 +123,42 @@
         self.filctrl = self.baseFile + ".control"
         self.filbas = basisFile
 
         # output
         self.filps = self.baseFile + ".ps"
         self.filcsv = self.baseFile + ".csv"
         self.filpdf = self.baseFile + ".pdf"
+        self.filtab = self.baseFile + ".table"
+        self.filcoo = self.baseFile + ".coord"
+        self.filpri = self.baseFile + ".print"
 
         self.title = self.baseFile.split('/')[-1]
 
+    def load_result(self):
+        # 读取结果
+        with open(self.filcoo, 'rb') as f:
+            text = f.read().decode().replace('\n','')
+        sdata = text.split()
+        ppm_index = sdata.index('ppm-axis')
+        phase_index = sdata.index('phased')
+        fit_index = sdata.index('fit')
+        background_index = sdata.index('background')
+        data_len = int(sdata[ppm_index-3])
+        ppm = np.zeros(data_len)
+        phase = np.zeros(data_len)
+        fit = np.zeros(data_len)
+        background = np.zeros(data_len)
+        for i in range(data_len):
+            ppm[i] = float(sdata[ppm_index+3+i])
+            phase[i] = float(sdata[phase_index+4+i])
+            fit[i] = float(sdata[fit_index+5+i])
+            background[i] = float(sdata[background_index+3+i])
+
+        return ppm, phase, fit, background
+
     def __read_rda(self,rdaFile: str ):
         # 将rda文件转换为raw文件，并且读取配置信息
         with open(rdaFile, 'rb') as file:
             rdaText = file.read()
 
         headtext = rdaText[rdaText.find(b'>>> Begin of header <<<') + len(
             b'>>> Begin of header <<<') + 2: rdaText.find(b'>>> End of header <<<') - 2].decode()
@@ -243,19 +268,28 @@
             return self.spec_data
         else:
             assert False, 'dtype must be time or spec'
 
     def __gen_control(self):
         # 生成control文件
         # control file
-        control_text = (f" $LCMODL\n title= '{self.title}'\n "
-                        f"ppmst= {self.ctl_dict['ppmst']}\n ppmend= {self.ctl_dict['ppmend']}\n "
-                        f"nunfil= {self.ctl_dict['nunfil']}\n key= 210387309\n hzpppm= {self.ctl_dict['hzpppm']}\n "
-                        f"filraw= '{self.filraw}'\n filps= '{self.filps}'\n filbas= '{self.filbas}'\n filcsv= '{self.filcsv}'\n "
-                        f"lcsv = 11\n echot= {self.ctl_dict['echot']}\n deltat= {self.ctl_dict['deltat']}\n $END")
+        control_text = (f" $LCMODL\n "
+                        f"title= '{self.title}'\n "
+                        f"ppmst= {self.ctl_dict['ppmst']}\n "
+                        f"ppmend= {self.ctl_dict['ppmend']}\n "
+                        f"nunfil= {self.ctl_dict['nunfil']}\n "
+                        f"key= 210387309\n "
+                        f"hzpppm= {self.ctl_dict['hzpppm']}\n "
+                        f"filraw= '{self.filraw}'\n filps= '{self.filps}'\n "
+                        f"filbas= '{self.filbas}'\n filcsv= '{self.filcsv}'\n "
+                        f"filtab= '{self.filtab}'\n filcoo= '{self.filcoo}'\n "
+                        f"filpri= '{self.filpri}'\n "
+                        f"lcsv = 11\n lprint = 6\n lcoord = 9\n ltable = 7\n "
+                        f"echot= {self.ctl_dict['echot']}\n "
+                        f"deltat= {self.ctl_dict['deltat']}\n $END")
 
         with open(self.filctrl, 'w') as control:
             control.write(control_text)
 
     def __convert_ps_pdf(self):
         # 将PostScript文件转换为pdf文件
         args = [
```

### Comparing `lcmtools-0.1.3/lcmtools.egg-info/PKG-INFO` & `lcmtools-0.1.5/lcmtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcmtools
-Version: 0.1.3
+Version: 0.1.5
 Summary: A script that calls LCModel through Python.
 Home-page: https://github.com/luodeb/lcmtools
 Author: Luo Debin
 Author-email: luodeb@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lcmtools Version: 0.1.3 Summary: A script that
+Metadata-Version: 2.1 Name: lcmtools Version: 0.1.5 Summary: A script that
 calls LCModel through Python. Home-page: https://github.com/luodeb/lcmtools
 Author: Luo Debin Author-email: luodeb@qq.com License: MIT Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Requires-Python: >=3.6.0 Description-Content-Type: text/
```

### Comparing `lcmtools-0.1.3/setup.py` & `lcmtools-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'lcmtools'
 DESCRIPTION = 'A script that calls LCModel through Python.'
 URL = 'https://github.com/luodeb/lcmtools'
 EMAIL = 'luodeb@qq.com'
 AUTHOR = 'Luo Debin'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.3'
+VERSION = '0.1.5'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'python3-ghostscript', 'numpy', 'scipy',
 ]
 
 # What packages are optional?
```

