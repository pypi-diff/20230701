# Comparing `tmp/libsodium-2.5.1.tar.gz` & `tmp/libsodium-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsodium-2.5.1.tar", last modified: Sat Jul  1 18:29:57 2023, max compression
+gzip compressed data, was "libsodium-2.5.2.tar", last modified: Sat Jul  1 21:50:17 2023, max compression
```

## Comparing `libsodium-2.5.1.tar` & `libsodium-2.5.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:29:57.102473 libsodium-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-01 18:29:26.000000 libsodium-2.5.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-01 18:29:57.102473 libsodium-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-01 18:29:26.000000 libsodium-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-01 18:29:26.000000 libsodium-2.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-01 18:29:57.102473 libsodium-2.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:29:57.098473 libsodium-2.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:29:57.098473 libsodium-2.5.1/src/libsodium/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-01 18:29:26.000000 libsodium-2.5.1/src/libsodium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26876 2023-07-01 18:29:26.000000 libsodium-2.5.1/src/libsodium/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-01 18:29:26.000000 libsodium-2.5.1/src/libsodium/classes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:29:57.102473 libsodium-2.5.1/src/libsodium/db/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-01 18:29:26.000000 libsodium-2.5.1/src/libsodium/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-01 18:29:26.000000 libsodium-2.5.1/src/libsodium/db/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-01 18:29:26.000000 libsodium-2.5.1/src/libsodium/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-07-01 18:29:26.000000 libsodium-2.5.1/src/libsodium/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:29:57.102473 libsodium-2.5.1/src/libsodium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-01 18:29:57.000000 libsodium-2.5.1/src/libsodium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-01 18:29:57.000000 libsodium-2.5.1/src/libsodium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 18:29:57.000000 libsodium-2.5.1/src/libsodium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 18:29:57.000000 libsodium-2.5.1/src/libsodium.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:50:17.896142 libsodium-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-01 21:49:52.000000 libsodium-2.5.2/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-01 21:50:17.896142 libsodium-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-01 21:49:52.000000 libsodium-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-01 21:49:52.000000 libsodium-2.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-01 21:50:17.896142 libsodium-2.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:50:17.892142 libsodium-2.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:50:17.892142 libsodium-2.5.2/src/libsodium/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-01 21:49:52.000000 libsodium-2.5.2/src/libsodium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27113 2023-07-01 21:49:52.000000 libsodium-2.5.2/src/libsodium/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-01 21:49:52.000000 libsodium-2.5.2/src/libsodium/classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:50:17.896142 libsodium-2.5.2/src/libsodium/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-01 21:49:52.000000 libsodium-2.5.2/src/libsodium/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-01 21:49:52.000000 libsodium-2.5.2/src/libsodium/db/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-01 21:49:52.000000 libsodium-2.5.2/src/libsodium/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-07-01 21:49:52.000000 libsodium-2.5.2/src/libsodium/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 21:50:17.896142 libsodium-2.5.2/src/libsodium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-01 21:50:17.000000 libsodium-2.5.2/src/libsodium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-01 21:50:17.000000 libsodium-2.5.2/src/libsodium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 21:50:17.000000 libsodium-2.5.2/src/libsodium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 21:50:17.000000 libsodium-2.5.2/src/libsodium.egg-info/top_level.txt
```

### Comparing `libsodium-2.5.1/LICENCE` & `libsodium-2.5.2/LICENCE`

 * *Files identical despite different names*

### Comparing `libsodium-2.5.1/PKG-INFO` & `libsodium-2.5.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: libsodium
-Version: 2.5.1
+Version: 2.5.2
 Summary: A simple web framework
 Home-page: https://libsodium.readthedocs.io/en/latest/
 Author: Ahsan Ahmed
 Author-email: ahsan.ahmed3246@gmail.com
 Project-URL: Docs, https://libsodium.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
-# Sodium v2.51
+# Sodium v2.52
 [![Documentation Status](https://readthedocs.org/projects/libsodium/badge/?version=latest)](https://libsodium.readthedocs.io/en/latest/?badge=latest)
 ![PyPI](https://img.shields.io/pypi/v/libsodium)
 
 Sodium is a WSGI web framework(like django) that is built for creating API's.
 # Instalation
 Linux/MacOS:
 ```
```

### Comparing `libsodium-2.5.1/setup.cfg` & `libsodium-2.5.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = libsodium
-version = 2.5.1
+version = 2.5.2
 author = Ahsan Ahmed
 author_email = ahsan.ahmed3246@gmail.com
 description = A simple web framework
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://libsodium.readthedocs.io/en/latest/
 project_urls =
```

### Comparing `libsodium-2.5.1/src/libsodium/__main__.py` & `libsodium-2.5.2/src/libsodium/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             S:::::So::::o     o::::od:::::d     d:::::d  i::::i u:::::uuuu:::::u  m::::m   m::::m   m::::m
 SSSSSSS     S:::::So:::::ooooo:::::od::::::ddddd::::::ddi::::::iu:::::::::::::::uum::::m   m::::m   m::::m
 S::::::SSSSSS:::::So:::::::::::::::o d:::::::::::::::::di::::::i u:::::::::::::::um::::m   m::::m   m::::m
 S:::::::::::::::SS  oo:::::::::::oo   d:::::::::ddd::::di::::::i  uu::::::::uu:::um::::m   m::::m   m::::m
  SSSSSSSSSSSSSSS      ooooooooooo      ddddddddd   dddddiiiiiiii    uuuuuuuu  uuuummmmmm   mmmmmm   mmmmmm
 """
     print("\x1b[32m"+x+"\x1b[0m")
-    print("v2.50\nMade by ahsan")
+    print("v2.52\nMade by ahsan")
     exit()
 
 if args[0] == "init":
     print("\033[93m"+"Name for project(leave blank to use current directory):"+"\x1b[0m")
     project_name = input("\x1b[32m"+"> ")
     print("\033[93m"+"What is your interpreter(ex. python3, python, py)"+"\x1b[0m")
     interpreter = input("\x1b[32m"+"> ")
@@ -180,14 +180,19 @@
     return server
 
 if __name__ == "__main__":
     import grpc
     from concurrent import futures
     addAll(grpc.server(futures.ThreadPoolExecutor(max_workers=10)))""")
 
+    os.mkdir("src/templates")
+    x = open(prefix+"src/templates/.sodium", "w")
+    x.write(os.getcwd()+f"/{project_name}")
+    x.close()
+
     x = open(prefix+"start.py", 'w')
     x.write('''from libsodium import Deamon
 from sonora.wsgi import grpcWSGI
 from socketio import WSGIApp
 import eventlet
 import json
 import importlib
@@ -247,15 +252,15 @@
 SSSSSSS     S:::::So:::::ooooo:::::od::::::ddddd::::::ddi::::::iu:::::::::::::::uum::::m   m::::m   m::::m
 S::::::SSSSSS:::::So:::::::::::::::o d:::::::::::::::::di::::::i u:::::::::::::::um::::m   m::::m   m::::m
 S:::::::::::::::SS  oo:::::::::::oo   d:::::::::ddd::::di::::::i  uu::::::::uu:::um::::m   m::::m   m::::m
  SSSSSSSSSSSSSSS      ooooooooooo      ddddddddd   dddddiiiiiiii    uuuuuuuu  uuuummmmmm   mmmmmm   mmmmmm
 
     """
     print(F_Green+x+F_End)
-    print("v2.50")
+    print("v2.52")
     print(f"{getCurrentTime()} [{F_Magenta}INFO{F_End}] Creating Deamon... ")
     MainDeamon = Deamon()
 
     print(f"{getCurrentTime()} [{F_LightCyan}SocketIO{F_End}] Loading SocketIO app...")
     from src.websockets.app import sio
     from os import listdir
     from os.path import isfile
@@ -586,15 +591,15 @@
         except Exception as e:
             return False""")
             f.close()
         else:
             print(f"The utility {args[2]} is not creatable")
             exit()
     elif args[1] == "gRPC":
-        if not len(args) == 3:
+        if not len(args) >= 3:
             print("Invalid amount of arugments please check out the code below\npython3 -m libsodium create gRPC example.proto")
             exit(1)
         try:
             config = open('sodiumconfig.json', 'r')
         except:
             print("The sodiumconfig.json file was not found")
             exit()
@@ -626,17 +631,21 @@
         except FileExistsError:
             pass
         
         exit_code = os.system(f"{interpreter} -m grpc_tools.protoc -I src/gRPC/protobufs --python_out=src/gRPC/{args[2][:len(args[2])-6]} --grpc_python_out=src/gRPC/{args[2][:len(args[2])-6]} src/gRPC/protobufs/{args[2]}")
 
         if not exit_code == 0:
             print("Process is shutting down")
-            os.rmdir(f"src/gRPC/{args[2][:len(args[2])-6]}")
+            if not args[3] == "--regen":
+                os.rmdir(f"src/gRPC/{args[2][:len(args[2])-6]}")
             exit(1)
 
+        if args[3] == "--regen":
+            exit()
+
         f = open(f"src/gRPC/{args[2][:len(args[2])-6]}/{args[2][:len(args[2])-6]}.py", "w")
         f.write(f"""import src.gRPC.{args[2][:len(args[2])-6]}.{args[2][:len(args[2])-6]}_pb2_grpc as {args[2][:len(args[2])-6]}_pb2_grpc 
 
 def serve(server):
     {args[2][:len(args[2])-6]}_pb2_grpc.add_ExampleServicer_to_server(
         AppServicerHere(), server
     )""")
```

### Comparing `libsodium-2.5.1/src/libsodium/classes.py` & `libsodium-2.5.2/src/libsodium/classes.py`

 * *Files identical despite different names*

### Comparing `libsodium-2.5.1/src/libsodium/wsgi.py` & `libsodium-2.5.2/src/libsodium/wsgi.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
             if hasattr(controler, "blueprint"):
                 blueprint = controler.blueprint()
                 targetMimetypes = blueprint[1]
                 blueprint = blueprint[0]
                 blueprint = blueprint.blueprint
                 if not request.mimetype in targetMimetypes:
-                    rsp = Response("<h1>Incorrect mimetype.</h1><p>Sodium v2.50</p>")
+                    rsp = Response("<h1>Incorrect mimetype.</h1><p>Sodium v2.52</p>")
                     rsp.headers['Content-Type'] = 'text/html' 
                     return rsp(environ, start_response)
                 if request.mimetype == "application/x-www-form-urlencoded":
                     target = request.form
                 elif request.mimetype == "multipart/form":
                         target = request.form
                 elif request.mimetype == "application/json":
```

### Comparing `libsodium-2.5.1/src/libsodium.egg-info/PKG-INFO` & `libsodium-2.5.2/src/libsodium.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: libsodium
-Version: 2.5.1
+Version: 2.5.2
 Summary: A simple web framework
 Home-page: https://libsodium.readthedocs.io/en/latest/
 Author: Ahsan Ahmed
 Author-email: ahsan.ahmed3246@gmail.com
 Project-URL: Docs, https://libsodium.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
-# Sodium v2.51
+# Sodium v2.52
 [![Documentation Status](https://readthedocs.org/projects/libsodium/badge/?version=latest)](https://libsodium.readthedocs.io/en/latest/?badge=latest)
 ![PyPI](https://img.shields.io/pypi/v/libsodium)
 
 Sodium is a WSGI web framework(like django) that is built for creating API's.
 # Instalation
 Linux/MacOS:
 ```
```

