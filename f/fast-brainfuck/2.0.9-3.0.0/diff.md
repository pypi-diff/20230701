# Comparing `tmp/fast-brainfuck-2.0.9.tar.gz` & `tmp/fast-brainfuck-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\fast-brainfuck-2.0.9.tar", last modified: Thu Jun 29 02:54:03 2023, max compression
+gzip compressed data, was "dist\fast-brainfuck-3.0.0.tar", last modified: Sat Jul  1 07:06:18 2023, max compression
```

## Comparing `fast-brainfuck-2.0.9.tar` & `fast-brainfuck-3.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 02:54:03.634377 fast-brainfuck-2.0.9/
--rw-rw-rw-   0        0        0     3753 2023-06-29 02:54:03.634377 fast-brainfuck-2.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     2428 2023-06-29 02:53:38.000000 fast-brainfuck-2.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 02:54:03.634377 fast-brainfuck-2.0.9/fast_brainfuck.egg-info/
--rw-rw-rw-   0        0        0     3753 2023-06-29 02:54:03.000000 fast-brainfuck-2.0.9/fast_brainfuck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-06-29 02:54:03.000000 fast-brainfuck-2.0.9/fast_brainfuck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 02:54:03.000000 fast-brainfuck-2.0.9/fast_brainfuck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-29 02:54:03.000000 fast-brainfuck-2.0.9/fast_brainfuck.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-06-29 02:54:03.000000 fast-brainfuck-2.0.9/fast_brainfuck.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-29 02:54:03.000000 fast-brainfuck-2.0.9/fast_brainfuck.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4720 2023-06-29 02:53:58.000000 fast-brainfuck-2.0.9/fastbf.py
--rw-rw-rw-   0        0        0       42 2023-06-29 02:54:03.634377 fast-brainfuck-2.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1189 2023-06-29 02:53:52.000000 fast-brainfuck-2.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 07:06:18.077971 fast-brainfuck-3.0.0/
+-rw-rw-rw-   0        0        0     4255 2023-07-01 07:06:18.076969 fast-brainfuck-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2898 2023-07-01 07:05:46.000000 fast-brainfuck-3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 07:06:18.076464 fast-brainfuck-3.0.0/fast_brainfuck.egg-info/
+-rw-rw-rw-   0        0        0     4255 2023-07-01 07:06:18.000000 fast-brainfuck-3.0.0/fast_brainfuck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-07-01 07:06:18.000000 fast-brainfuck-3.0.0/fast_brainfuck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 07:06:18.000000 fast-brainfuck-3.0.0/fast_brainfuck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-01 07:06:18.000000 fast-brainfuck-3.0.0/fast_brainfuck.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-07-01 07:06:18.000000 fast-brainfuck-3.0.0/fast_brainfuck.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-01 07:06:18.000000 fast-brainfuck-3.0.0/fast_brainfuck.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4733 2023-07-01 06:58:47.000000 fast-brainfuck-3.0.0/fastbf.py
+-rw-rw-rw-   0        0        0       42 2023-07-01 07:06:18.077971 fast-brainfuck-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1189 2023-07-01 07:01:06.000000 fast-brainfuck-3.0.0/setup.py
```

### Comparing `fast-brainfuck-2.0.9/PKG-INFO` & `fast-brainfuck-3.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: fast-brainfuck
-Version: 2.0.9
+Version: 3.0.0
 Summary: Brainfuck "compiler" for Python (fast)
 Home-page: https://github.com/none-None1/fast-bf
 License: UNKNOWN
 Description: <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
         
-        [git repo](https://github.com/none-None1/fast-bf)
+        # A big bugfix is applied to this package due to the technique Python uses to import modules.
+        
+        In previous versions, when brainfuck_to_function is called, it creates a module named _foo, which is imported. But Python also stores it into a cache, that means when you call brainfuck_to_function again, the new module would not be imported, which causes a function the same as the previous function is returned.
+        
+        However, in this version and higher, a module with a random name is created instead, which fixed the bug.
         
         ### This is a very fast brainfuck "compiler".
         
         When used, it builds brainfuck code into Python extension modules, and imports it.
         
         Requires:
         1. Python>=3.6
```

### Comparing `fast-brainfuck-2.0.9/README.md` & `fast-brainfuck-3.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
 
-[git repo](https://github.com/none-None1/fast-bf)
+# A big bugfix is applied to this package due to the technique Python uses to import modules.
+
+In previous versions, when brainfuck_to_function is called, it creates a module named _foo, which is imported. But Python also stores it into a cache, that means when you call brainfuck_to_function again, the new module would not be imported, which causes a function the same as the previous function is returned.
+
+However, in this version and higher, a module with a random name is created instead, which fixed the bug.
 
 ### This is a very fast brainfuck "compiler".
 
 When used, it builds brainfuck code into Python extension modules, and imports it.
 
 Requires:
 1. Python>=3.6
```

### Comparing `fast-brainfuck-2.0.9/fast_brainfuck.egg-info/PKG-INFO` & `fast-brainfuck-3.0.0/fast_brainfuck.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: fast-brainfuck
-Version: 2.0.9
+Version: 3.0.0
 Summary: Brainfuck "compiler" for Python (fast)
 Home-page: https://github.com/none-None1/fast-bf
 License: UNKNOWN
 Description: <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
         
-        [git repo](https://github.com/none-None1/fast-bf)
+        # A big bugfix is applied to this package due to the technique Python uses to import modules.
+        
+        In previous versions, when brainfuck_to_function is called, it creates a module named _foo, which is imported. But Python also stores it into a cache, that means when you call brainfuck_to_function again, the new module would not be imported, which causes a function the same as the previous function is returned.
+        
+        However, in this version and higher, a module with a random name is created instead, which fixed the bug.
         
         ### This is a very fast brainfuck "compiler".
         
         When used, it builds brainfuck code into Python extension modules, and imports it.
         
         Requires:
         1. Python>=3.6
```

### Comparing `fast-brainfuck-2.0.9/fastbf.py` & `fast-brainfuck-3.0.0/fastbf.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,32 +31,32 @@
     code+='    unsigned char *cell=new unsigned char['+str(cellsize)+'];\n    int p=0;\nfor(int i=0;i<'+str(cellsize)+';i++) cell[i]=0;\n'
     translate={'>':'p++;','<':'p--;',',':'cell[p]=getchar();','.':'putchar(cell[p]);','[':'while(cell[p]){',']':'}','+':'++cell[p];','-':'--cell[p];'}
     for i in brainfuck:
         if i in translate:
             code += '    '+translate[i]+'\n'
     code+='}'
     return code
-def wrap_cpp(cpp):
+def wrap_cpp(cpp,dn='_foo'):
     """
     Wrap C++ code into code usable by Python.
     :param cpp: C++ code
     :return: Wrapped code
     """
     code='''
 #include<pybind11/pybind11.h>
 #include<cstdio>
 #include<cstring>
 namespace py=pybind11;
     '''
     code+=cpp
     code+='''
-PYBIND11_MODULE(_foo,self){
+PYBIND11_MODULE(%s,self){
     self.def("run",&run);
 }
-    '''
+    '''%dn
     return code
 def dist_cpp(cpp):
     """
     Distribute C++ code into Python module.
     :param cpp: C++ code
     :return: None
     """
@@ -80,51 +80,51 @@
     :return: A function, call it with no arguments to run the brainfuck code
     """
     cwd=os.getcwd()
     os.chdir(_tmp())
     dn=random_string()
     os.mkdir(dn)
     os.chdir(dn)
-    distcode='''
+    distcode=f'''
 from setuptools import setup,Extension
 from pybind11 import get_include
 _foo=Extension(
-    name='_foo',
+    name='{dn}',
     sources=['_foo.cpp'],
     language='c++',
     include_dirs=[get_include()],
     extra_compile_args=['-std=c++11']
 )
 setup(
     ext_modules=[_foo]
 )
     '''
     cpp=brainfuck_to_cpp(brainfuck,cellsize)
-    wrap=wrap_cpp(cpp)
+    wrap=wrap_cpp(cpp,dn)
     with open('_foo.cpp','w') as f:
         f.write(wrap)
     with open('setup.py','w') as f:
         f.write(distcode)
     python=sys.executable
     if platform.system()!='Windows':
         os.chmod(os.path.join(_tmp(),dn),0o777)
         run(
-            f'{python} setup.py build_ext --inplace',shell=True,stdout=PIPE,stderr=PIPE # Finally! I've fixed Linux support!
+            f'{python} setup.py build_ext --inplace',shell=True, stdout=PIPE, stderr=PIPE # Finally! I've fixed Linux support!
         )
     else:
         run(
             [
                 python,
                 'setup.py',
                 'build_ext',
                 '--inplace'
             ], shell=True, stdout=PIPE, stderr=PIPE
         )
     sys.path.append(os.path.join(_tmp(),dn))
-    foo=__import__('_foo')
+    foo=__import__(dn)
     os.chdir(cwd)
     sys.path.pop()
     return foo.run
 def dist_brainfuck(brainfuck,modulename='foo',cellsize=300000):
     """
     Distribute brainfuck code into a python module.
     :param brainfuck: Brainfuck code
```

### Comparing `fast-brainfuck-2.0.9/setup.py` & `fast-brainfuck-3.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 def readme():
     with open('README.md','r') as f:
         return f.read()
 setup(
     name='fast-brainfuck',
     py_modules=['fastbf'],
-    version='2.0.9',
+    version='3.0.0',
     entry_points={
         'console_scripts':[
             'fastbf=fastbf:_fastbf_inter'
         ]
     },
     description='Brainfuck "compiler" for Python (fast)',
     long_description=readme(),
```

