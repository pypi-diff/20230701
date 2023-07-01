# Comparing `tmp/cocoserver-1.0.8.tar.gz` & `tmp/cocoserver-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cocoserver-1.0.8.tar", last modified: Thu Jun 29 23:28:16 2023, max compression
+gzip compressed data, was "cocoserver-1.0.9.tar", last modified: Sat Jul  1 12:13:51 2023, max compression
```

## Comparing `cocoserver-1.0.8.tar` & `cocoserver-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-06-29 23:28:16.250645 cocoserver-1.0.8/
--rw-r--r--   0 culler     (501) staff       (20)    18092 2023-06-26 20:10:54.000000 cocoserver-1.0.8/LICENSE
--rw-r--r--   0 culler     (501) staff       (20)     2964 2023-06-29 23:28:16.250441 cocoserver-1.0.8/PKG-INFO
--rw-r--r--   0 culler     (501) staff       (20)     1977 2023-06-26 20:10:54.000000 cocoserver-1.0.8/README.rst
--rw-r--r--   0 culler     (501) staff       (20)     1287 2023-06-28 01:52:55.000000 cocoserver-1.0.8/pyproject.toml
--rw-r--r--   0 culler     (501) staff       (20)       38 2023-06-29 23:28:16.250703 cocoserver-1.0.8/setup.cfg
-drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-06-29 23:28:16.248308 cocoserver-1.0.8/src/
-drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-06-29 23:28:16.249223 cocoserver-1.0.8/src/cocoserver/
--rw-r--r--   0 culler     (501) staff       (20)     7565 2023-06-29 23:23:16.000000 cocoserver-1.0.8/src/cocoserver/__init__.py
-drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-06-29 23:28:16.250159 cocoserver-1.0.8/src/cocoserver.egg-info/
--rw-r--r--   0 culler     (501) staff       (20)     2964 2023-06-29 23:28:16.000000 cocoserver-1.0.8/src/cocoserver.egg-info/PKG-INFO
--rw-r--r--   0 culler     (501) staff       (20)      212 2023-06-29 23:28:16.000000 cocoserver-1.0.8/src/cocoserver.egg-info/SOURCES.txt
--rw-r--r--   0 culler     (501) staff       (20)        1 2023-06-29 23:28:16.000000 cocoserver-1.0.8/src/cocoserver.egg-info/dependency_links.txt
--rw-r--r--   0 culler     (501) staff       (20)       11 2023-06-29 23:28:16.000000 cocoserver-1.0.8/src/cocoserver.egg-info/top_level.txt
+drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-07-01 12:13:51.739628 cocoserver-1.0.9/
+-rw-r--r--   0 culler     (501) staff       (20)    18092 2023-06-24 13:34:32.000000 cocoserver-1.0.9/LICENSE
+-rw-r--r--   0 culler     (501) staff       (20)     3133 2023-07-01 12:13:51.739005 cocoserver-1.0.9/PKG-INFO
+-rw-r--r--   0 culler     (501) staff       (20)     2146 2023-07-01 11:51:38.000000 cocoserver-1.0.9/README.rst
+-rw-r--r--   0 culler     (501) staff       (20)     1331 2023-07-01 11:31:11.000000 cocoserver-1.0.9/pyproject.toml
+-rw-r--r--   0 culler     (501) staff       (20)       38 2023-07-01 12:13:51.739799 cocoserver-1.0.9/setup.cfg
+drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-07-01 12:13:51.733182 cocoserver-1.0.9/src/
+drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-07-01 12:13:51.735723 cocoserver-1.0.9/src/cocoserver/
+-rw-r--r--   0 culler     (501) staff       (20)     7862 2023-07-01 12:12:46.000000 cocoserver-1.0.9/src/cocoserver/__init__.py
+-rw-r--r--   0 culler     (501) staff       (20)       38 2023-07-01 11:27:55.000000 cocoserver-1.0.9/src/cocoserver/__main__.py
+drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-07-01 12:13:51.738284 cocoserver-1.0.9/src/cocoserver.egg-info/
+-rw-r--r--   0 culler     (501) staff       (20)     3133 2023-07-01 12:13:51.000000 cocoserver-1.0.9/src/cocoserver.egg-info/PKG-INFO
+-rw-r--r--   0 culler     (501) staff       (20)      280 2023-07-01 12:13:51.000000 cocoserver-1.0.9/src/cocoserver.egg-info/SOURCES.txt
+-rw-r--r--   0 culler     (501) staff       (20)        1 2023-07-01 12:13:51.000000 cocoserver-1.0.9/src/cocoserver.egg-info/dependency_links.txt
+-rw-r--r--   0 culler     (501) staff       (20)       41 2023-07-01 12:13:51.000000 cocoserver-1.0.9/src/cocoserver.egg-info/entry_points.txt
+-rw-r--r--   0 culler     (501) staff       (20)       11 2023-07-01 12:13:51.000000 cocoserver-1.0.9/src/cocoserver.egg-info/top_level.txt
```

### Comparing `cocoserver-1.0.8/LICENSE` & `cocoserver-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cocoserver-1.0.8/PKG-INFO` & `cocoserver-1.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocoserver
-Version: 1.0.8
+Version: 1.0.9
 Summary: A local HTTP server for compressed content.
 Author-email: Marc Culler <culler@users.noreply.github.com>, "Nathan M. Dunfield" <nathan@dunfield.info>, Matthias Görner <enischte@gmail.com>
 Maintainer-email: Marc Culler <culler@users.noreply.github.com>, "Nathan M. Dunfield" <nathan@dunfield.info>, Matthias Görner <enischte@gmail.com>
 Project-URL: Homepage, https://github.com/3-manifolds/cocoserver
 Project-URL: Bug Tracker, https://github.com/3-manifolds/cocoserver/issues
 Keywords: http,server,gzip,documentation
 Classifier: Development Status :: 3 - Alpha
@@ -52,7 +52,9 @@
 
 To use the server::
   
   >>> from cocoserver import StaticServer
   >>> s = StaticServer('my/site/root')
   >>> s.visit('mypage')
 
+The pip package also installs a console script named *coco* which can
+be used to view your static site, for example by running: ``coco /usr/local/share/doc/myproject``.
```

### Comparing `cocoserver-1.0.8/README.rst` & `cocoserver-1.0.9/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -33,7 +33,9 @@
 
 To use the server::
   
   >>> from cocoserver import StaticServer
   >>> s = StaticServer('my/site/root')
   >>> s.visit('mypage')
 
+The pip package also installs a console script named *coco* which can
+be used to view your static site, for example by running: ``coco /usr/local/share/doc/myproject``.
```

### Comparing `cocoserver-1.0.8/pyproject.toml` & `cocoserver-1.0.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -24,13 +24,16 @@
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Topic :: Software Development :: Documentation"
 ]
 
+[project.scripts]
+coco = "cocoserver:main"
+
 [project.urls]
 "Homepage" = "https://github.com/3-manifolds/cocoserver"
 "Bug Tracker" = "https://github.com/3-manifolds/cocoserver/issues"
 
 [tool.setuptools.dynamic]
 version = {attr = "cocoserver.__version__"}
```

### Comparing `cocoserver-1.0.8/src/cocoserver/__init__.py` & `cocoserver-1.0.9/src/cocoserver/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import email
 import shutil
 import datetime
 import webbrowser
 import urllib.parse
 import importlib.metadata
 
-__version__ = '1.0.8'
+__version__ = '1.0.9'
 
 class GzipHTTPRequestHandler(SimpleHTTPRequestHandler):
     def __init__(self, *args, **kwargs):
         self.logfile = kwargs.pop('logfile', None)
         super().__init__(*args, **kwargs)
 
     def log_message(self, format, *args):
@@ -174,7 +174,17 @@
         webbrowser.open_new_tab(url)
 
     def address(self):
         """Return the ip address of this server."""
         if not self.httpd or not self.server_thread.is_alive():
             raise ValueError('Server is not running')
         return self.httpd.server_address
+
+def main():
+    if len(sys.argv) != 2:
+        print('Provide the path of a site root as an argument.')
+        sys.exit(1)
+    StaticServer(sys.argv[1]).visit()
+    while True:
+        response = input('Type "stop" to stop the server:\n> ')
+        if response == 'stop':
+            sys.exit()
```

### Comparing `cocoserver-1.0.8/src/cocoserver.egg-info/PKG-INFO` & `cocoserver-1.0.9/src/cocoserver.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocoserver
-Version: 1.0.8
+Version: 1.0.9
 Summary: A local HTTP server for compressed content.
 Author-email: Marc Culler <culler@users.noreply.github.com>, "Nathan M. Dunfield" <nathan@dunfield.info>, Matthias Görner <enischte@gmail.com>
 Maintainer-email: Marc Culler <culler@users.noreply.github.com>, "Nathan M. Dunfield" <nathan@dunfield.info>, Matthias Görner <enischte@gmail.com>
 Project-URL: Homepage, https://github.com/3-manifolds/cocoserver
 Project-URL: Bug Tracker, https://github.com/3-manifolds/cocoserver/issues
 Keywords: http,server,gzip,documentation
 Classifier: Development Status :: 3 - Alpha
@@ -52,7 +52,9 @@
 
 To use the server::
   
   >>> from cocoserver import StaticServer
   >>> s = StaticServer('my/site/root')
   >>> s.visit('mypage')
 
+The pip package also installs a console script named *coco* which can
+be used to view your static site, for example by running: ``coco /usr/local/share/doc/myproject``.
```

