# Comparing `tmp/lino_react-23.6.2.tar.gz` & `tmp/lino_react-23.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lino_react-23.6.2.tar", last modified: Wed Jun 21 08:42:00 2023, max compression
+gzip compressed data, was "lino_react-23.7.0.tar", last modified: Sat Jul  1 13:35:51 2023, max compression
```

## Comparing `lino_react-23.6.2.tar` & `lino_react-23.7.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-21 08:42:00.007061 lino_react-23.6.2/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    34523 2023-02-28 05:23:19.000000 lino_react-23.6.2/COPYING
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      157 2023-02-28 05:23:19.000000 lino_react-23.6.2/MANIFEST.in
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1032 2023-06-21 08:42:00.007061 lino_react-23.6.2/PKG-INFO
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      178 2023-02-28 05:23:19.000000 lino_react-23.6.2/README.rst
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-21 08:41:59.995061 lino_react-23.6.2/lino_react/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      283 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-21 08:41:59.999061 lino_react-23.6.2/lino_react/react/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     4628 2023-06-13 10:46:31.000000 lino_react-23.6.2/lino_react/react/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-21 08:41:59.999061 lino_react-23.6.2/lino_react/react/__pycache__/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3382 2023-06-15 05:49:26.000000 lino_react-23.6.2/lino_react/react/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2980 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     4013 2023-04-27 06:42:41.000000 lino_react-23.6.2/lino_react/react/__pycache__/icons.cpython-310.pyc
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3793 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/__pycache__/icons.cpython-38.pyc
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      160 2023-03-30 05:54:52.000000 lino_react-23.6.2/lino_react/react/__pycache__/models.cpython-310.pyc
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1412 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/__pycache__/models.cpython-38.pyc
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    18341 2023-05-03 06:16:14.000000 lino_react-23.6.2/lino_react/react/__pycache__/renderer.cpython-310.pyc
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    18127 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/__pycache__/renderer.cpython-38.pyc
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    20615 2023-06-12 10:17:24.000000 lino_react-23.6.2/lino_react/react/__pycache__/views.cpython-310.pyc
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    20473 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/__pycache__/views.cpython-38.pyc
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-21 08:41:59.995061 lino_react-23.6.2/lino_react/react/config/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-21 08:41:59.999061 lino_react-23.6.2/lino_react/react/config/react/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/config/react/linoweb.json
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1910 2023-06-11 06:54:48.000000 lino_react-23.6.2/lino_react/react/config/react/main.html
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    16246 2023-06-21 07:51:55.000000 lino_react-23.6.2/lino_react/react/config/react/service-worker.js
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3893 2023-04-27 06:29:15.000000 lino_react-23.6.2/lino_react/react/icons.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       36 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/index.js
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-03-30 05:51:42.000000 lino_react-23.6.2/lino_react/react/models.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    29204 2023-05-03 06:10:54.000000 lino_react-23.6.2/lino_react/react/renderer.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-21 08:41:59.995061 lino_react-23.6.2/lino_react/react/static/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-21 08:42:00.003061 lino_react-23.6.2/lino_react/react/static/media/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    10355 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/static/media/color.6441e63a.png
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    10355 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/static/media/color.c7a33805.png
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    13112 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/static/media/line.567f5738.gif
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    39748 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/static/media/primeicons.2d2afb27.eot
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    57384 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/static/media/primeicons.3a0d4a58.ttf
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    39648 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/static/media/primeicons.66ee0deb.woff
--rw-rw-r--   0 blurry    (1000) blurry    (1000)   234640 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/static/media/primeicons.c55d94a2.svg
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    39572 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/static/media/primeicons.df0140f8.ttf
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    57560 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/static/media/primeicons.dfbfef2d.eot
--rw-rw-r--   0 blurry    (1000) blurry    (1000)   163568 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/static/media/primeicons.e5e0e944.svg
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    57460 2023-02-28 05:23:19.000000 lino_react-23.6.2/lino_react/react/static/media/primeicons.e61f3495.woff
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-21 08:42:00.007061 lino_react-23.6.2/lino_react/react/static/react/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)  1777129 2023-06-21 07:51:55.000000 lino_react-23.6.2/lino_react/react/static/react/main.js
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2437 2023-06-21 07:51:55.000000 lino_react-23.6.2/lino_react/react/static/react/main.js.LICENSE.txt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    28705 2023-06-11 15:16:59.000000 lino_react-23.6.2/lino_react/react/views.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1431 2023-06-21 08:41:02.000000 lino_react-23.6.2/lino_react/setup_info.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-21 08:41:59.995061 lino_react-23.6.2/lino_react.egg-info/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1032 2023-06-21 08:41:59.000000 lino_react-23.6.2/lino_react.egg-info/PKG-INFO
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1770 2023-06-21 08:41:59.000000 lino_react-23.6.2/lino_react.egg-info/SOURCES.txt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        1 2023-06-21 08:41:59.000000 lino_react-23.6.2/lino_react.egg-info/dependency_links.txt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        1 2023-02-28 05:23:26.000000 lino_react-23.6.2/lino_react.egg-info/not-zip-safe
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        5 2023-06-21 08:41:59.000000 lino_react-23.6.2/lino_react.egg-info/requires.txt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       11 2023-06-21 08:41:59.000000 lino_react-23.6.2/lino_react.egg-info/top_level.txt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       38 2023-06-21 08:42:00.007061 lino_react-23.6.2/setup.cfg
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      183 2023-02-28 05:23:19.000000 lino_react-23.6.2/setup.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-01 13:35:51.604881 lino_react-23.7.0/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    34523 2023-02-28 05:23:19.000000 lino_react-23.7.0/COPYING
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      157 2023-02-28 05:23:19.000000 lino_react-23.7.0/MANIFEST.in
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1032 2023-07-01 13:35:51.604881 lino_react-23.7.0/PKG-INFO
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      178 2023-02-28 05:23:19.000000 lino_react-23.7.0/README.rst
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-01 13:35:51.596881 lino_react-23.7.0/lino_react/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      283 2023-02-28 05:23:19.000000 lino_react-23.7.0/lino_react/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-01 13:35:51.596881 lino_react-23.7.0/lino_react/react/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     4628 2023-06-13 10:46:31.000000 lino_react-23.7.0/lino_react/react/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-01 13:35:51.596881 lino_react-23.7.0/lino_react/react/__pycache__/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3382 2023-06-15 05:49:26.000000 lino_react-23.7.0/lino_react/react/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2980 2023-02-28 05:23:19.000000 lino_react-23.7.0/lino_react/react/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     4013 2023-04-27 06:42:41.000000 lino_react-23.7.0/lino_react/react/__pycache__/icons.cpython-310.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3793 2023-02-28 05:23:19.000000 lino_react-23.7.0/lino_react/react/__pycache__/icons.cpython-38.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      160 2023-03-30 05:54:52.000000 lino_react-23.7.0/lino_react/react/__pycache__/models.cpython-310.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1412 2023-02-28 05:23:19.000000 lino_react-23.7.0/lino_react/react/__pycache__/models.cpython-38.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    18457 2023-07-01 13:29:48.000000 lino_react-23.7.0/lino_react/react/__pycache__/renderer.cpython-310.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    18127 2023-02-28 05:23:19.000000 lino_react-23.7.0/lino_react/react/__pycache__/renderer.cpython-38.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    20615 2023-06-12 10:17:24.000000 lino_react-23.7.0/lino_react/react/__pycache__/views.cpython-310.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    20473 2023-02-28 05:23:19.000000 lino_react-23.7.0/lino_react/react/__pycache__/views.cpython-38.pyc
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-01 13:35:51.596881 lino_react-23.7.0/lino_react/react/config/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-01 13:35:51.596881 lino_react-23.7.0/lino_react/react/config/react/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:19.000000 lino_react-23.7.0/lino_react/react/config/react/linoweb.json
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1910 2023-06-11 06:54:48.000000 lino_react-23.7.0/lino_react/react/config/react/main.html
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    16246 2023-07-01 13:31:06.000000 lino_react-23.7.0/lino_react/react/config/react/service-worker.js
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3893 2023-04-27 06:29:15.000000 lino_react-23.7.0/lino_react/react/icons.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       36 2023-02-28 05:23:19.000000 lino_react-23.7.0/lino_react/react/index.js
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-03-30 05:51:42.000000 lino_react-23.7.0/lino_react/react/models.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    29357 2023-07-01 13:29:44.000000 lino_react-23.7.0/lino_react/react/renderer.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-01 13:35:51.596881 lino_react-23.7.0/lino_react/react/static/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-01 13:35:51.600881 lino_react-23.7.0/lino_react/react/static/media/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    10355 2023-02-28 05:23:19.000000 lino_react-23.7.0/lino_react/react/static/media/color.6441e63a.png
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    10355 2023-02-28 05:23:19.000000 lino_react-23.7.0/lino_react/react/static/media/color.c7a33805.png
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    13112 2023-02-28 05:23:19.000000 lino_react-23.7.0/lino_react/react/static/media/line.567f5738.gif
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    39748 2023-02-28 05:23:19.000000 lino_react-23.7.0/lino_react/react/static/media/primeicons.2d2afb27.eot
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    57384 2023-02-28 05:23:19.000000 lino_react-23.7.0/lino_react/react/static/media/primeicons.3a0d4a58.ttf
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    39648 2023-02-28 05:23:19.000000 lino_react-23.7.0/lino_react/react/static/media/primeicons.66ee0deb.woff
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)   234640 2023-02-28 05:23:19.000000 lino_react-23.7.0/lino_react/react/static/media/primeicons.c55d94a2.svg
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    39572 2023-02-28 05:23:19.000000 lino_react-23.7.0/lino_react/react/static/media/primeicons.df0140f8.ttf
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    57560 2023-02-28 05:23:19.000000 lino_react-23.7.0/lino_react/react/static/media/primeicons.dfbfef2d.eot
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)   163568 2023-02-28 05:23:19.000000 lino_react-23.7.0/lino_react/react/static/media/primeicons.e5e0e944.svg
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    57460 2023-02-28 05:23:19.000000 lino_react-23.7.0/lino_react/react/static/media/primeicons.e61f3495.woff
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-01 13:35:51.604881 lino_react-23.7.0/lino_react/react/static/react/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)  1776344 2023-07-01 13:31:06.000000 lino_react-23.7.0/lino_react/react/static/react/main.js
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2437 2023-07-01 13:31:06.000000 lino_react-23.7.0/lino_react/react/static/react/main.js.LICENSE.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    28705 2023-06-11 15:16:59.000000 lino_react-23.7.0/lino_react/react/views.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1431 2023-07-01 13:34:24.000000 lino_react-23.7.0/lino_react/setup_info.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-01 13:35:51.596881 lino_react-23.7.0/lino_react.egg-info/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1032 2023-07-01 13:35:51.000000 lino_react-23.7.0/lino_react.egg-info/PKG-INFO
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1770 2023-07-01 13:35:51.000000 lino_react-23.7.0/lino_react.egg-info/SOURCES.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        1 2023-07-01 13:35:51.000000 lino_react-23.7.0/lino_react.egg-info/dependency_links.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        1 2023-02-28 05:23:26.000000 lino_react-23.7.0/lino_react.egg-info/not-zip-safe
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        5 2023-07-01 13:35:51.000000 lino_react-23.7.0/lino_react.egg-info/requires.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       11 2023-07-01 13:35:51.000000 lino_react-23.7.0/lino_react.egg-info/top_level.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       38 2023-07-01 13:35:51.604881 lino_react-23.7.0/setup.cfg
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      183 2023-02-28 05:23:19.000000 lino_react-23.7.0/setup.py
```

### Comparing `lino_react-23.6.2/COPYING` & `lino_react-23.7.0/COPYING`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.2/PKG-INFO` & `lino_react-23.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lino_react
-Version: 23.6.2
+Version: 23.7.0
 Summary: The React front end for Lino
 Home-page: https://gitlab.com/lino-framework/react
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 Classifier:   Programming Language :: Python
 Classifier:   Programming Language :: Python :: 3
 Classifier:   Development Status :: 5 - Production/Stable
```

### Comparing `lino_react-23.6.2/lino_react/react/__init__.py` & `lino_react-23.7.0/lino_react/react/__init__.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.2/lino_react/react/__pycache__/__init__.cpython-310.pyc` & `lino_react-23.7.0/lino_react/react/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.2/lino_react/react/__pycache__/__init__.cpython-38.pyc` & `lino_react-23.7.0/lino_react/react/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.2/lino_react/react/__pycache__/icons.cpython-310.pyc` & `lino_react-23.7.0/lino_react/react/__pycache__/icons.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.2/lino_react/react/__pycache__/icons.cpython-38.pyc` & `lino_react-23.7.0/lino_react/react/__pycache__/icons.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.2/lino_react/react/__pycache__/models.cpython-38.pyc` & `lino_react-23.7.0/lino_react/react/__pycache__/models.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.2/lino_react/react/__pycache__/renderer.cpython-310.pyc` & `lino_react-23.7.0/lino_react/react/__pycache__/renderer.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May  3 06:10:54 2023 UTC, .py size: 29204 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 6f0d 0d0a 0000 0000 eefa 5164 1472 0000  o.........Qd.r..
+00000000: 6f0d 0d0a 0000 0000 482a a064 ad72 0000  o.......H*.d.r..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 a201 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 ae01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6400 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6407 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
 00000080: 6408 6c0d 6d0e 5a0e 6d0f 5a0f 0100 6400  d.l.m.Z.m.Z...d.
 00000090: 6409 6c10 6d11 5a11 6d12 5a12 0100 6400  d.l.m.Z.m.Z...d.
@@ -20,1128 +20,1135 @@
 00000130: 6d2d 5a2d 0100 6400 6414 6c2e 6d2f 5a2f  m-Z-..d.d.l.m/Z/
 00000140: 6d30 5a30 6d31 5a31 6d32 5a32 6d33 5a33  m0Z0m1Z1m2Z2m3Z3
 00000150: 0100 6400 6415 6c13 6d34 5a34 0100 6400  ..d.d.l.m4Z4..d.
 00000160: 6416 6c35 6d36 5a36 0100 6400 6417 6c37  d.l5m6Z6..d.d.l7
 00000170: 6d38 5a38 0100 6400 6418 6c39 6d3a 5a3a  m8Z8..d.d.l9m:Z:
 00000180: 6d3b 5a3b 6d3c 5a3c 0100 6400 6419 6c3d  m;Z;m<Z<..d.d.l=
 00000190: 6d3e 5a3e 6d3f 5a3f 0100 6400 641a 6c40  m>Z>m?Z?..d.d.l@
-000001a0: 6d41 5a41 0100 641b 641c 6c42 6d43 5a43  mAZA..d.d.lBmCZC
-000001b0: 0100 6421 641d 641e 8401 5a44 4700 641f  ..d!d.d...ZDG.d.
-000001c0: 6420 8400 6420 650f 8303 5a45 6401 5300  d ..d e...ZEd.S.
-000001d0: 2922 e900 0000 004e 2901 da04 5061 7468  )".....N)...Path
-000001e0: 2901 da06 6573 6361 7065 2901 da08 7365  )...escape)...se
-000001f0: 7474 696e 6773 2901 da06 6d6f 6465 6c73  ttings)...models
-00000200: 2901 da0b 666f 726d 6174 5f6c 617a 7929  )...format_lazy)
-00000210: 01da 0b74 7261 6e73 6c61 7469 6f6e 2902  ...translation).
-00000220: da11 6164 645f 7573 6572 5f6c 616e 6775  ..add_user_langu
-00000230: 6167 65da 0f4a 7343 6163 6865 5265 6e64  age..JsCacheRend
-00000240: 6572 6572 2902 da04 4d65 6e75 da08 4d65  erer)...Menu..Me
-00000250: 6e75 4974 656d 2901 da09 636f 6e73 7461  nuItem)...consta
-00000260: 6e74 7329 01da 0b63 686f 6963 656c 6973  nts)...choicelis
-00000270: 7473 2901 da0b 436f 6e74 656e 7454 7970  ts)...ContentTyp
-00000280: 6529 01da 0b45 7874 5265 6e64 6572 6572  e)...ExtRenderer
-00000290: 2908 da0e 5368 6f77 456d 7074 7954 6162  )...ShowEmptyTab
-000002a0: 6c65 da0a 5368 6f77 4465 7461 696c da0d  le..ShowDetail..
-000002b0: 5772 6170 7065 6441 6374 696f 6eda 0a53  WrappedAction..S
-000002c0: 686f 7749 6e73 6572 74da 0953 686f 7754  howInsert..ShowT
-000002d0: 6162 6c65 da0c 5375 626d 6974 4465 7461  able..SubmitDeta
-000002e0: 696c da0c 5375 626d 6974 496e 7365 7274  il..SubmitInsert
-000002f0: da06 4163 7469 6f6e 2901 da0b 426f 756e  ..Action)...Boun
-00000300: 6441 6374 696f 6e29 01da 0e43 686f 6963  dAction)...Choic
-00000310: 654c 6973 744d 6574 6129 01da 1044 6173  eListMeta)...Das
-00000320: 6862 6f61 7264 4c61 796f 7574 7329 01da  hboardLayouts)..
-00000330: 0541 6374 6f72 2902 da0c 4c61 796f 7574  .Actor)...Layout
-00000340: 4861 6e64 6c65 da0a 4261 7365 4c61 796f  Handle..BaseLayo
-00000350: 7574 2905 da0d 4c61 796f 7574 456c 656d  ut)...LayoutElem
-00000360: 656e 74da 1143 6f6d 626f 4669 656c 6445  ent..ComboFieldE
-00000370: 6c65 6d65 6e74 da1d 5369 6d70 6c65 5265  lement..SimpleRe
-00000380: 6d6f 7465 436f 6d62 6f46 6965 6c64 456c  moteComboFieldEl
-00000390: 656d 656e 74da 0c46 6965 6c64 456c 656d  ement..FieldElem
-000003a0: 656e 74da 1750 7265 7669 6577 5465 7874  ent..PreviewText
-000003b0: 4669 656c 6445 6c65 6d65 6e74 2901 da06  FieldElement)...
-000003c0: 6b65 726e 656c 2901 da01 4529 01da 056a  kernel)...E)...j
-000003d0: 7367 656e 2903 da05 7079 326a 73da 076a  sgen)...py2js..j
-000003e0: 735f 636f 6465 da08 6f62 6a32 6469 6374  s_code..obj2dict
-000003f0: 2902 da10 6765 745f 7573 6572 5f70 726f  )...get_user_pro
-00000400: 6669 6c65 da11 7769 7468 5f75 7365 725f  file..with_user_
-00000410: 7072 6f66 696c 6529 01da 0769 7363 6c61  profile)...iscla
-00000420: 7373 e901 0000 0029 01da 1252 4541 4354  ss.....)...REACT
-00000430: 5f49 434f 4e5f 4d41 5050 494e 4763 0300  _ICON_MAPPINGc..
-00000440: 0000 0000 0000 0000 0000 0500 0000 0300  ................
-00000450: 0000 4300 0000 734a 0000 007c 0264 016b  ..C...sJ...|.d.k
-00000460: 0273 0c74 007c 0283 0173 0c4a 0064 0283  .s.t.|...s.J.d..
-00000470: 0182 0174 017c 0083 0144 005d 125c 027d  ...t.|...D.].\.}
-00000480: 037d 047c 0272 1a7c 027c 0483 017d 047c  .}.|.r.|.|...}.|
-00000490: 047c 016b 0272 227c 0302 0001 0053 0071  .|.k.r"|.....S.q
-000004a0: 1064 0353 0029 047a 4d52 6574 7572 6e73  .d.S.).zMReturns
-000004b0: 2074 6865 2069 6e64 6578 206f 6620 616e   the index of an
-000004c0: 2065 6c65 6d65 6e74 2069 6e20 6120 6361   element in a ca
-000004d0: 6c6c 6162 6c65 2077 6869 6368 2063 616e  llable which can
-000004e0: 2062 6520 7573 6520 6120 6b65 7920 6675   be use a key fu
-000004f0: 6e63 7469 6f6e 4e7a 586b 6579 2073 686f  nctionNzXkey sho
-00000500: 6c64 2062 6520 6120 6675 6e63 7469 6f6e  ld be a function
-00000510: 2074 6861 7420 7461 6b65 7320 7468 6520   that takes the 
-00000520: 6974 7465 7227 7320 6974 656d 2061 6e64  itter's item and
-00000530: 2072 6574 7572 6e73 2074 6861 7420 7761   returns that wa
-00000540: 6e74 6564 206d 6174 6368 6564 2069 7465  nted matched ite
-00000550: 6de9 ffff ffff 2902 da08 6361 6c6c 6162  m.....)...callab
-00000560: 6c65 da09 656e 756d 6572 6174 6529 05da  le..enumerate)..
-00000570: 0569 7474 6572 da06 7461 7267 6574 da03  .itter..target..
-00000580: 6b65 79da 0169 da01 78a9 0072 3600 0000  key..i..x..r6...
-00000590: fa45 2f68 6f6d 652f 626c 7572 7279 2f6c  .E/home/blurry/l
-000005a0: 696e 6f2f 656e 762f 7265 706f 7369 746f  ino/env/reposito
-000005b0: 7269 6573 2f72 6561 6374 2f6c 696e 6f5f  ries/react/lino_
-000005c0: 7265 6163 742f 7265 6163 742f 7265 6e64  react/react/rend
-000005d0: 6572 6572 2e70 79da 0466 696e 642d 0000  erer.py..find-..
-000005e0: 0073 1000 0000 1802 1002 0401 0801 0801  .s..............
-000005f0: 0801 02ff 0403 7238 0000 0063 0000 0000  ......r8...c....
-00000600: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00000610: 0000 0000 73e6 0000 0065 005a 0164 005a  ....s....e.Z.d.Z
-00000620: 0264 015a 0364 025a 0464 025a 0564 035a  .d.Z.d.Z.d.Z.d.Z
-00000630: 0664 045a 0764 025a 0887 0066 0164 0564  .d.Z.d.Z...f.d.d
-00000640: 0684 085a 0964 0764 0884 005a 0a64 0964  ...Z.d.d...Z.d.d
-00000650: 0a84 005a 0b64 0b64 0c84 005a 0c64 0d64  ...Z.d.d...Z.d.d
-00000660: 0e84 005a 0d64 0f64 1084 005a 0e64 1164  ...Z.d.d...Z.d.d
-00000670: 1284 005a 0f64 3264 1464 1584 015a 1069  ...Z.d2d.d...Z.i
-00000680: 0066 0164 1664 1784 015a 1164 1864 1984  .f.d.d...Z.d.d..
-00000690: 005a 1264 1a64 1b84 005a 1364 1c64 1d84  .Z.d.d...Z.d.d..
-000006a0: 005a 1464 1e64 1f84 005a 1564 2064 2184  .Z.d.d...Z.d d!.
-000006b0: 005a 1664 2264 2384 005a 1764 2464 2584  .Z.d"d#..Z.d$d%.
-000006c0: 005a 1864 2664 2784 005a 1964 2864 2984  .Z.d&d'..Z.d(d).
-000006d0: 005a 1a64 2a64 2b84 005a 1b64 2c64 2d84  .Z.d*d+..Z.d,d-.
-000006e0: 005a 1c64 2e64 2f84 005a 1d87 0066 0164  .Z.d.d/..Z...f.d
-000006f0: 3064 3184 085a 1e87 0004 005a 1f53 0029  0d1..Z.....Z.S.)
-00000700: 33da 0852 656e 6465 7265 727a 480a 2020  3..RendererzH.  
-00000710: 2020 4120 6672 6f6e 742d 656e 6420 7265    A front-end re
-00000720: 6e64 6572 6572 2074 6861 7420 7573 6573  nderer that uses
-00000730: 2074 6865 2052 6561 6374 204a 6176 6173   the React Javas
-00000740: 6372 6970 7420 6672 616d 6577 6f72 6b2e  cript framework.
-00000750: 0a20 2020 2054 7a12 7265 6163 742f 6c69  .    Tz.react/li
-00000760: 6e6f 7765 622e 6a73 6f6e 7a05 2e6a 736f  noweb.jsonz..jso
-00000770: 6e63 0200 0000 0000 0000 0000 0000 0200  nc..............
-00000780: 0000 0300 0000 0300 0000 731c 0000 0074  ..........s....t
-00000790: 0083 00a0 017c 01a1 0101 0074 02a0 037c  .....|.....t...|
-000007a0: 006a 04a1 0101 0064 0053 00a9 014e 2905  .j.....d.S...N).
-000007b0: da05 7375 7065 72da 085f 5f69 6e69 745f  ..super..__init_
-000007c0: 5f72 2500 0000 da12 7265 6769 7374 6572  _r%.....register
-000007d0: 5f63 6f6e 7665 7274 6572 da0f 7079 326a  _converter..py2j
-000007e0: 735f 636f 6e76 6572 7465 7229 02da 0473  s_converter)...s
-000007f0: 656c 66da 0966 726f 6e74 5f65 6e64 a901  elf..front_end..
-00000800: da09 5f5f 636c 6173 735f 5f72 3600 0000  ..__class__r6...
-00000810: 7237 0000 0072 3c00 0000 4500 0000 7304  r7...r<...E...s.
-00000820: 0000 000c 0110 017a 1152 656e 6465 7265  .......z.Rendere
-00000830: 722e 5f5f 696e 6974 5f5f 6302 0000 0000  r.__init__c.....
-00000840: 0000 0000 0000 000c 0000 0008 0000 0003  ................
-00000850: 0000 0073 7202 0000 6401 6402 8400 7400  ...sr...d.d...t.
-00000860: 6a01 a002 a100 4400 8301 7d02 7403 8300  j.....D...}.t...
-00000870: 7d03 8800 6a04 4400 5d14 7d04 7c04 a005  }...j.D.].}.|...
-00000880: a100 4400 5d0d 7d05 7c05 6a06 7c03 7601  ..D.].}.|.j.|.v.
-00000890: 7223 7c03 a007 7c05 6a06 a101 0100 7116  r#|...|.j.....q.
-000008a0: 7110 6403 8800 5f08 7409 6a0a 6a0b 7d06  q.d..._.t.j.j.}.
-000008b0: 740c 8700 6601 6404 6402 8408 7c03 4400  t...f.d.d...|.D.
-000008c0: 8301 7409 6a0a a00d 740e 8300 a101 7c06  ..t.j...t.....|.
-000008d0: 6a0f 6a10 7409 6a0a 6a11 8800 6a12 6a13  j.j.t.j.j...j.j.
-000008e0: 6405 7501 6406 6402 8400 7409 6a0a 6a14  d.u.d.d...t.j.j.
-000008f0: 4400 8301 6407 8d06 7d07 7409 6a0a a015  D...d...}.t.j...
-00000900: 6408 a101 7264 7c07 6a16 7417 7c06 6a18  d...rd|.j.t.|.j.
-00000910: 6a19 6a1a a01b a100 8301 6409 8d01 0100  j.j.......d.....
-00000920: 7c07 6a16 7409 6a0a 6a00 6a1c 640a 8d01  |.j.t.j.j.j.d...
-00000930: 0100 7a13 7c07 6a16 741d a01e 741f 7409  ..z.|.j.t...t.t.
-00000940: 6a20 8301 640b 1b00 640c 1b00 a101 6a21  j ..d...d.....j!
-00000950: 640d 8d01 0100 5700 6e09 0400 7422 7989  d.....W.n...t"y.
-00000960: 0100 0100 0100 5900 6e01 7700 7423 7409  ......Y.n.w.t#t.
-00000970: 6a0a 640e 8302 7298 7c07 6a16 7409 6a0a  j.d...r.|.j.t.j.
-00000980: 6a24 640f 8d01 0100 7409 6a0a 6a25 6405  j$d.....t.j.j%d.
-00000990: 6b02 72a5 7c07 6a16 6403 6410 8d01 0100  k.r.|.j.d.d.....
-000009a0: 6e0e 7423 7c06 6a26 6411 8302 72b3 7c07  n.t#|.j&d...r.|.
-000009b0: 6a16 7c06 6a26 6a27 6412 8d01 0100 7409  j.|.j&j'd.....t.
-000009c0: 6a0a a015 6413 a101 72c5 7c07 6a16 7c06  j...d...r.|.j.|.
-000009d0: 6a28 6a29 6fc2 7409 6a0a 6a2a 6414 8d01  j(j)o.t.j.j*d...
-000009e0: 0100 6900 7d08 8800 6a2b 4400 5d2f 7d09  ..i.}...j+D.]/}.
-000009f0: 8800 a02c 7c09 a101 7c08 7c09 6a2d 3c00  ...,|...|.|.j-<.
-00000a00: 7423 7c09 6415 8302 72f9 6416 7c09 6a2d  t#|.d...r.d.|.j-
-00000a10: 7600 72f9 742e 7c02 6417 1900 8301 4400  v.r.t.|.d.....D.
-00000a20: 5d14 5c02 7d0a 7d0b 7c0b 6418 1900 7c09  ].\.}.}.|.d...|.
-00000a30: 6a2f 6b02 72f8 7c09 6a2d 7c02 6417 1900  j/k.r.|.j-|.d...
-00000a40: 7c0a 1900 6419 3c00 71e4 71ca 8800 6a30  |...d.<.q.q...j0
-00000a50: 4400 5d0a 7d09 8800 a02c 7c09 a101 7c08  D.].}....,|...|.
-00000a60: 7c09 6a2d 3c00 71fd 8800 6a31 4400 5d0b  |.j-<.q...j1D.].
-00000a70: 7d09 8800 a02c 7c09 a101 7c08 7c09 6a2d  }....,|...|.|.j-
-00000a80: 3c00 9001 710b 8800 6a32 4400 5d0b 7d09  <...q...j2D.].}.
-00000a90: 8800 a02c 7c09 a101 7c08 7c09 6a2d 3c00  ...,|...|.|.j-<.
-00000aa0: 9001 711a 7c07 6a16 7c08 7c02 641a 8d02  ..q.|.j.|.|.d...
-00000ab0: 0100 7c01 a033 7434 7c07 8301 a101 0100  ..|..3t4|.......
-00000ac0: 641b 8800 5f08 641c 5300 291d 7a86 0a20  d..._.d.S.).z.. 
-00000ad0: 2020 2020 2020 2043 7265 6174 6573 2077         Creates w
-00000ae0: 6861 7420 6973 206b 6e6f 776e 2061 7320  hat is known as 
-00000af0: 7769 6e64 6f77 2e41 7070 2e73 7461 7465  window.App.state
-00000b00: 2e73 6974 655f 6461 7461 2069 6e20 5265  .site_data in Re
-00000b10: 6163 7420 636f 6465 2e0a 0a20 2020 2020  act code...     
-00000b20: 2020 203a 7061 7261 6d20 663a 2046 696c     :param f: Fil
-00000b30: 6520 6f62 6a65 6374 0a20 2020 2020 2020  e object.       
-00000b40: 203a 7265 7475 726e 3a20 310a 2020 2020   :return: 1.    
-00000b50: 2020 2020 6301 0000 0000 0000 0000 0000      c...........
-00000b60: 0003 0000 0006 0000 0053 0000 0073 2400  .........S...s$.
-00000b70: 0000 6900 7c00 5d0e 5c02 7d01 7d02 7c01  ..i.|.].\.}.}.|.
-00000b80: 6400 6401 8400 7c02 a000 a100 4400 8301  d.d...|.....D...
-00000b90: 9302 7102 5300 2902 6301 0000 0000 0000  ..q.S.).c.......
-00000ba0: 0000 0000 0002 0000 0006 0000 0053 0000  .............S..
-00000bb0: 0073 2400 0000 6700 7c00 5d0e 7d01 7c01  .s$...g.|.].}.|.
-00000bc0: 6400 1900 6a00 7401 7c01 6401 1900 8301  d...j.t.|.d.....
-00000bd0: 6402 9c02 9102 7102 5300 2903 7201 0000  d.....q.S.).r...
-00000be0: 0072 2c00 0000 2902 da05 7661 6c75 65da  .r,...)...value.
-00000bf0: 0474 6578 7429 0272 4300 0000 da03 7374  .text).rC.....st
-00000c00: 7229 02da 022e 30da 0163 7236 0000 0072  r)....0..cr6...r
-00000c10: 3600 0000 7237 0000 00da 0a3c 6c69 7374  6...r7.....<list
-00000c20: 636f 6d70 3e52 0000 0073 0200 0000 2400  comp>R...s....$.
-00000c30: 7a35 5265 6e64 6572 6572 2e77 7269 7465  z5Renderer.write
-00000c40: 5f6c 696e 6f5f 6a73 2e3c 6c6f 6361 6c73  _lino_js.<locals
-00000c50: 3e2e 3c64 6963 7463 6f6d 703e 2e3c 6c69  >.<dictcomp>.<li
-00000c60: 7374 636f 6d70 3e29 01da 0b67 6574 5f63  stcomp>)...get_c
-00000c70: 686f 6963 6573 2903 7246 0000 00da 0249  hoices).rF.....I
-00000c80: 44da 0263 6c72 3600 0000 7236 0000 0072  D..clr6...r6...r
-00000c90: 3700 0000 da0a 3c64 6963 7463 6f6d 703e  7.....<dictcomp>
-00000ca0: 5000 0000 7308 0000 0006 0006 0312 ff06  P...s...........
-00000cb0: fe7a 2a52 656e 6465 7265 722e 7772 6974  .z*Renderer.writ
-00000cc0: 655f 6c69 6e6f 5f6a 732e 3c6c 6f63 616c  e_lino_js.<local
-00000cd0: 733e 2e3c 6469 6374 636f 6d70 3e54 6301  s>.<dictcomp>Tc.
-00000ce0: 0000 0000 0000 0000 0000 0002 0000 0006  ................
-00000cf0: 0000 0013 0000 0073 1a00 0000 6900 7c00  .......s....i.|.
-00000d00: 5d09 7d01 7c01 6a00 8800 a001 7c01 a101  ].}.|.j.....|...
-00000d10: 9302 7102 5300 7236 0000 0029 02da 0b61  ..q.S.r6...)...a
-00000d20: 6374 696f 6e5f 6e61 6d65 da0b 6163 7469  ction_name..acti
-00000d30: 6f6e 326a 736f 6e29 0272 4600 0000 da01  on2json).rF.....
-00000d40: 61a9 0172 3f00 0000 7236 0000 0072 3700  a..r?...r6...r7.
-00000d50: 0000 724c 0000 005f 0000 0073 0200 0000  ..rL..._...s....
-00000d60: 1a00 4e63 0100 0000 0000 0000 0000 0000  ..Nc............
-00000d70: 0200 0000 0400 0000 5300 0000 7316 0000  ........S...s...
-00000d80: 0069 007c 005d 077d 017c 016a 007c 016a  .i.|.].}.|.j.|.j
-00000d90: 0193 0271 0253 0072 3600 0000 2902 da0b  ...q.S.r6...)...
-00000da0: 646a 616e 676f 5f63 6f64 65da 046e 616d  django_code..nam
-00000db0: 6529 0272 4600 0000 da04 6c61 6e67 7236  e).rF.....langr6
-00000dc0: 0000 0072 3600 0000 7237 0000 0072 4c00  ...r6...r7...rL.
-00000dd0: 0000 6500 0000 7302 0000 0016 0029 06da  ..e...s......)..
-00000de0: 0761 6374 696f 6e73 da04 6d65 6e75 da15  .actions..menu..
-00000df0: 7573 655f 6461 7368 626f 6172 645f 6c61  use_dashboard_la
-00000e00: 796f 7574 73da 0a73 6974 655f 7469 746c  youts..site_titl
-00000e10: 65da 1065 6469 7469 6e67 5f66 726f 6e74  e..editing_front
-00000e20: 656e 64da 096c 616e 6775 6167 6573 da04  end..languages..
-00000e30: 6d65 6d6f 2901 da0a 7375 6767 6573 746f  memo)...suggesto
-00000e40: 7273 2901 da0f 7265 7669 7369 6f6e 5f6e  rs)...revision_n
-00000e50: 756d 6265 72da 0572 6561 6374 7a07 6d61  umber..reactz.ma
-00000e60: 696e 2e6a 7329 01da 0d6d 6a73 5f74 696d  in.js)...mjs_tim
-00000e70: 6573 7461 6d70 da0a 7468 656d 655f 6e61  estamp..theme_na
-00000e80: 6d65 2901 725f 0000 0029 01da 0d6e 6f5f  me).r_...)...no_
-00000e90: 7573 6572 5f6d 6f64 656c da19 616c 6c6f  user_model..allo
-00000ea0: 775f 6f6e 6c69 6e65 5f72 6567 6973 7472  w_online_registr
-00000eb0: 6174 696f 6e29 0172 6100 0000 da06 6e6f  ation).ra.....no
-00000ec0: 7469 6679 2901 da0c 7573 655f 7075 7368  tify)...use_push
-00000ed0: 5f61 7069 da0b 6368 6f69 6365 5f6e 616d  _api..choice_nam
-00000ee0: 657a 1073 7973 7465 6d2e 4461 7368 626f  ez.system.Dashbo
-00000ef0: 6172 647a 1773 7973 7465 6d2e 4461 7368  ardz.system.Dash
-00000f00: 626f 6172 644c 6179 6f75 7473 7243 0000  boardLayoutsrC..
-00000f10: 00da 0d77 696e 646f 775f 6c61 796f 7574  ...window_layout
-00000f20: 2902 da0b 666f 726d 5f70 616e 656c 7372  )...form_panelsr
-00000f30: 0d00 0000 4672 2c00 0000 2935 7223 0000  ....Fr,...)5r#..
-00000f40: 00da 0b43 484f 4943 454c 4953 5453 da05  ...CHOICELISTS..
-00000f50: 6974 656d 73da 0373 6574 da0b 6163 746f  items..set..acto
-00000f60: 7273 5f6c 6973 74da 0b67 6574 5f61 6374  rs_list..get_act
-00000f70: 696f 6e73 da06 6163 7469 6f6e da03 6164  ions..action..ad
-00000f80: 64da 1173 6572 6961 6c69 7365 5f6a 735f  d..serialise_js_
-00000f90: 636f 6465 7204 0000 00da 0453 4954 45da  coder......SITE.
-00000fa0: 0770 6c75 6769 6e73 da04 6469 6374 da0d  .plugins..dict..
-00000fb0: 6765 745f 7369 7465 5f6d 656e 7572 2900  get_site_menur).
-00000fc0: 0000 da06 7379 7374 656d 7256 0000 00da  ....systemrV....
-00000fd0: 0574 6974 6c65 7240 0000 00da 0a75 726c  .titler@.....url
-00000fe0: 5f70 7265 6669 7872 5900 0000 da0c 6973  _prefixrY.....is
-00000ff0: 5f69 6e73 7461 6c6c 6564 da06 7570 6461  _installed..upda
-00001000: 7465 da04 6c69 7374 725a 0000 00da 0670  te..listrZ.....p
-00001010: 6172 7365 72da 0a73 7567 6765 7374 6572  arser..suggester
-00001020: 73da 046b 6579 73da 0a63 6f64 655f 6d74  s..keys..code_mt
-00001030: 696d 65da 026f 73da 0473 7461 7472 0200  ime..os..statr..
-00001040: 0000 da0b 5354 4154 4943 5f52 4f4f 54da  ....STATIC_ROOT.
-00001050: 0873 745f 6d74 696d 65da 1146 696c 654e  .st_mtime..FileN
-00001060: 6f74 466f 756e 6445 7272 6f72 da07 6861  otFoundError..ha
-00001070: 7361 7474 7272 5f00 0000 da0a 7573 6572  sattrr_.....user
-00001080: 5f6d 6f64 656c da05 7573 6572 7372 6100  _model..usersra.
-00001090: 0000 7262 0000 0072 6300 0000 da09 7573  ..rb...rc.....us
-000010a0: 655f 6c69 6e6f 6472 6600 0000 da0a 7061  e_linodrf.....pa
-000010b0: 6e65 6c32 6a73 6f6e da0f 5f66 6f72 6d70  nel2json.._formp
-000010c0: 616e 656c 5f6e 616d 6572 3000 0000 7264  anel_namer0...rd
-000010d0: 0000 00da 0c70 6172 616d 5f70 616e 656c  .....param_panel
-000010e0: 73da 1361 6374 696f 6e5f 7061 7261 6d5f  s..action_param_
-000010f0: 7061 6e65 6c73 da0c 6f74 6865 725f 7061  panels..other_pa
-00001100: 6e65 6c73 da05 7772 6974 6572 2600 0000  nels..writer&...
-00001110: 290c 723f 0000 00da 0166 da10 6368 6f69  ).r?.....f..choi
-00001120: 6365 6c69 7374 735f 6461 7461 7254 0000  celists_datarT..
-00001130: 00da 0372 7074 da02 6261 7270 0000 00da  ...rpt..barp....
-00001140: 0464 6174 6172 6600 0000 da01 7072 3400  .datarf.....pr4.
-00001150: 0000 da04 6974 656d 7236 0000 0072 5000  ....itemr6...rP.
-00001160: 0000 7237 0000 00da 0d77 7269 7465 5f6c  ..r7.....write_l
-00001170: 696e 6f5f 6a73 4900 0000 7370 0000 0006  ino_jsI...sp....
-00001180: 0708 0306 fd06 050a 010c 020a 010c 0102  ................
-00001190: 8002 fe06 0408 0102 0110 010c 0206 0106  ................
-000011a0: 010a 0110 0106 f90c 0904 0210 0106 ff12  ................
-000011b0: 0602 0126 010c 0104 0102 ff0c 0310 010c  ...&............
-000011c0: 020e 010c 0110 010c 0218 0104 090a 0110  ................
-000011d0: 0114 0114 010e 0112 0104 800a 0112 010a  ................
-000011e0: 0114 010a 0114 010e 010e 0506 0204 017a  ...............z
-000011f0: 1652 656e 6465 7265 722e 7772 6974 655f  .Renderer.write_
-00001200: 6c69 6e6f 5f6a 7363 0200 0000 0000 0000  lino_jsc........
-00001210: 0000 0000 0400 0000 0600 0000 4300 0000  ............C...
-00001220: 73c6 0000 0074 007c 0174 0183 0273 074a  s....t.|.t...s.J
-00001230: 0082 0174 027c 016a 037c 01a0 04a1 007c  ...t.|.j.|.....|
-00001240: 01a0 05a1 007c 016a 0664 018d 047d 0274  .....|.j.d...}.t
-00001250: 007c 0174 0783 0272 297c 016a 086a 096a  .|.t...r)|.j.j.j
-00001260: 037c 0264 023c 0074 0a7c 016a 086a 0b83  .|.d.<.t.|.j.j..
-00001270: 017c 0264 033c 007c 016a 0c72 317c 016a  .|.d.<.|.j.r1|.j
-00001280: 0c7c 0264 043c 007c 016a 0d72 397c 016a  .|.d.<.|.j.r9|.j
-00001290: 0d7c 0264 053c 007c 016a 0e72 4064 067c  .|.d.<.|.j.r@d.|
-000012a0: 0264 073c 007c 016a 0f72 487c 016a 0f7c  .d.<.|.j.rH|.j.|
-000012b0: 0264 083c 007c 016a 1072 4f64 067c 0264  .d.<.|.j.rOd.|.d
-000012c0: 093c 007c 016a 1172 5664 067c 0264 0a3c  .<.|.j.rVd.|.d.<
-000012d0: 007c 00a0 127c 01a1 017d 037c 0372 617c  .|...|...}.|.ra|
-000012e0: 037c 0264 0b3c 007c 0253 0029 0c7a 3343  .|.d.<.|.S.).z3C
-000012f0: 6f6e 7665 7274 7320 676c 6f62 616c 206c  onverts global l
-00001300: 6973 7420 6f66 2061 6c6c 2061 6374 696f  ist of all actio
-00001310: 6e73 2074 6f20 6a73 6f6e 2066 6f72 6d61  ns to json forma
-00001320: 742e 2904 da02 616e da05 6c61 6265 6cda  t.)...an..label.
-00001330: 0d77 696e 646f 775f 6163 7469 6f6e da0b  .window_action..
-00001340: 6874 7470 5f6d 6574 686f 6472 9400 0000  http_methodr....
-00001350: da05 6163 746f 72da 0c70 7265 7072 6f63  ..actor..preproc
-00001360: 6573 736f 72da 0b73 656c 6563 745f 726f  essor..select_ro
-00001370: 7773 54da 1073 7562 6d69 745f 666f 726d  wsT..submit_form
-00001380: 5f64 6174 61da 0b62 7574 746f 6e5f 7465  _data..button_te
-00001390: 7874 da14 7368 6f77 5f69 6e5f 7369 6465  xt..show_in_side
-000013a0: 5f74 6f6f 6c62 6172 da0e 6e65 7665 725f  _toolbar..never_
-000013b0: 636f 6c6c 6170 7365 da04 6963 6f6e 2913  collapse..icon).
-000013c0: da0a 6973 696e 7374 616e 6365 7217 0000  ..isinstancer...
-000013d0: 0072 7100 0000 724d 0000 00da 0967 6574  .rq...rM.....get
-000013e0: 5f6c 6162 656c da10 6973 5f77 696e 646f  _label..is_windo
-000013f0: 775f 6163 7469 6f6e 7297 0000 0072 1200  w_actionr....r..
-00001400: 0000 da0c 626f 756e 645f 6163 7469 6f6e  ....bound_action
-00001410: 726c 0000 0072 4500 0000 7298 0000 0072  rl...rE...r....r
-00001420: 9900 0000 729a 0000 0072 9b00 0000 729c  ....r....r....r.
-00001430: 0000 0072 9d00 0000 729e 0000 00da 0f67  ...r....r......g
-00001440: 6574 5f61 6374 696f 6e5f 6963 6f6e 2904  et_action_icon).
-00001450: 723f 0000 00da 0176 da06 7265 7375 6c74  r?.....v..result
-00001460: 729f 0000 0072 3600 0000 7236 0000 0072  r....r6...r6...r
-00001470: 3700 0000 724e 0000 009e 0000 0073 2400  7...rN.......s$.
-00001480: 0000 0e02 0604 0601 0601 0401 06fd 0a06  ................
-00001490: 0e01 1001 1002 1002 0e01 1001 0e01 0e01  ................
-000014a0: 0a02 0c01 0402 7a14 5265 6e64 6572 6572  ......z.Renderer
-000014b0: 2e61 6374 696f 6e32 6a73 6f6e 6302 0000  .action2jsonc...
-000014c0: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-000014d0: 0043 0000 0073 2e00 0000 7400 7c01 7401  .C...s....t.|.t.
-000014e0: 8302 7307 4a00 8201 7c01 a002 a100 7d02  ..s.J...|.....}.
-000014f0: 7403 7c00 a004 7c02 6a05 a101 7c02 6a06  t.|...|.j...|.j.
-00001500: 6a07 6401 8d02 5300 2902 4e29 02da 046d  j.d...S.).N)...m
-00001510: 6169 6eda 0b77 696e 646f 775f 7369 7a65  ain..window_size
-00001520: 2908 72a0 0000 0072 1d00 0000 da11 6765  ).r....r......ge
-00001530: 745f 6c61 796f 7574 5f68 616e 646c 6572  t_layout_handler
-00001540: 7100 0000 da09 656c 656d 326a 736f 6e72  q.....elem2jsonr
-00001550: a700 0000 da06 6c61 796f 7574 72a8 0000  ......layoutr...
-00001560: 0029 0372 3f00 0000 7291 0000 0072 a500  .).r?...r....r..
-00001570: 0000 7236 0000 0072 3600 0000 7237 0000  ..r6...r6...r7..
-00001580: 0072 8600 0000 bb00 0000 730a 0000 000e  .r........s.....
-00001590: 0108 030c 0106 0106 ff7a 1352 656e 6465  .........z.Rende
-000015a0: 7265 722e 7061 6e65 6c32 6a73 6f6e 6302  rer.panel2jsonc.
-000015b0: 0000 0000 0000 0000 0000 0004 0000 0005  ................
-000015c0: 0000 0003 0000 0073 d600 0000 7400 7c01  .......s....t.|.
-000015d0: 7401 8302 7307 4a00 8201 7402 7c01 a003  t...s.J...t.|...
-000015e0: a100 7c01 6a04 6a05 6401 8d02 7d02 7406  ..|.j.j.d...}.t.
-000015f0: 7c01 6402 8302 7222 8700 6601 6403 6404  |.d...r"..f.d.d.
-00001600: 8408 7c01 6a07 4400 8301 7c02 6405 3c00  ..|.j.D...|.d.<.
-00001610: 7c02 a008 7409 7c01 6406 8302 a101 0100  |...t.|.d.......
-00001620: 7406 7c01 6407 8302 7253 7c02 a008 7409  t.|.d...rS|...t.
-00001630: 7c01 6a0a 6408 8302 a101 0100 7406 7c01  |.j.d.......t.|.
-00001640: 6409 8302 7253 7c01 6a0b 6400 7501 7253  d...rS|.j.d.u.rS
-00001650: 7c01 6a0b a00c a100 4400 5d0b 5c02 7d03  |.j.....D.].\.}.
-00001660: 7d01 8800 a00d 7c01 a101 7c02 7c03 3c00  }.....|...|.|.<.
-00001670: 7147 740e 7c01 6a04 740f 8302 7269 7c02  qGt.|.j.t...ri|.
-00001680: 6a08 7c01 a010 a100 640a 8d01 0100 7c02  j.|.....d.....|.
-00001690: 6a08 7c01 6a11 6a12 640b 8d01 0100 7c02  j.|.j.j.d.....|.
-000016a0: 5300 290c 4e29 0272 9500 0000 da0a 7265  S.).N).r......re
-000016b0: 6163 745f 6e61 6d65 da08 656c 656d 656e  act_name..elemen
-000016c0: 7473 6301 0000 0000 0000 0000 0000 0002  tsc.............
-000016d0: 0000 0005 0000 0013 0000 0073 1e00 0000  ...........s....
-000016e0: 6700 7c00 5d0b 7d01 7c01 a000 a100 7202  g.|.].}.|.....r.
-000016f0: 8800 a001 7c01 a101 9102 7102 5300 7236  ....|.....q.S.r6
-00001700: 0000 0029 02da 0a69 735f 7669 7369 626c  ...)...is_visibl
-00001710: 6572 aa00 0000 2902 7246 0000 00da 0165  er....).rF.....e
-00001720: 7250 0000 0072 3600 0000 7237 0000 0072  rP...r6...r7...r
-00001730: 4800 0000 ca00 0000 7302 0000 001e 007a  H.......s......z
-00001740: 2652 656e 6465 7265 722e 656c 656d 326a  &Renderer.elem2j
-00001750: 736f 6e2e 3c6c 6f63 616c 733e 2e3c 6c69  son.<locals>.<li
-00001760: 7374 636f 6d70 3e72 6800 0000 7a98 6669  stcomp>rh...z.fi
-00001770: 656c 6473 5f69 6e64 6578 2066 6965 6c64  elds_index field
-00001780: 735f 696e 6465 785f 6869 6464 656e 2065  s_index_hidden e
-00001790: 6469 7461 626c 6520 7665 7274 6963 616c  ditable vertical
-000017a0: 2068 7061 6420 6973 5f66 6965 6c64 7365   hpad is_fieldse
-000017b0: 7420 6e61 6d65 2077 6964 7468 2070 7265  t name width pre
-000017c0: 6665 7272 6564 5f77 6964 7468 2020 2020  ferred_width    
-000017d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017e0: 2020 2020 2020 2020 2020 2020 2020 6869                hi
-000017f0: 6464 656e 2076 616c 7565 2068 666c 6578  dden value hflex
-00001800: 2076 666c 6578 7298 0000 007a 1561 6374   vflexr....z.act
-00001810: 6f72 5f69 6420 6469 7370 6c61 795f 6d6f  or_id display_mo
-00001820: 6465 da06 736c 6176 6573 2901 da0d 6669  de..slaves)...fi
-00001830: 656c 645f 6f70 7469 6f6e 7329 01da 0968  eld_options)...h
-00001840: 656c 705f 7465 7874 2913 72a0 0000 0072  elp_text).r....r
-00001850: 1e00 0000 7271 0000 0072 a100 0000 7242  ....rq...r....rB
-00001860: 0000 00da 085f 5f6e 616d 655f 5f72 8200  .....__name__r..
-00001870: 0000 72ad 0000 0072 7700 0000 7228 0000  ..r....rw...r(..
-00001880: 0072 9800 0000 72b0 0000 0072 6800 0000  .r....r....rh...
-00001890: 72aa 0000 00da 0a69 7373 7562 636c 6173  r......issubclas
-000018a0: 7372 2100 0000 da11 6765 745f 6669 656c  sr!.....get_fiel
-000018b0: 645f 6f70 7469 6f6e 73da 0566 6965 6c64  d_options..field
-000018c0: 72b2 0000 0029 0472 3f00 0000 72a5 0000  r....).r?...r...
-000018d0: 0072 a600 0000 da01 6b72 3600 0000 7250  .r......kr6...rP
-000018e0: 0000 0072 3700 0000 72aa 0000 00c3 0000  ...r7...r.......
-000018f0: 0073 2000 0000 0e01 0802 0602 06fe 0a03  .s .............
-00001900: 1801 1002 0a04 1202 1403 1201 1001 0c03  ................
-00001910: 1001 1001 0402 7a12 5265 6e64 6572 6572  ......z.Renderer
-00001920: 2e65 6c65 6d32 6a73 6f6e 6301 0000 0000  .elem2jsonc.....
-00001930: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-00001940: 0000 0073 0400 0000 6401 5300 2902 4e7a  ...s....d.S.).Nz
-00001950: 1e77 696e 646f 772e 4170 702e 6461 7368  .window.App.dash
-00001960: 626f 6172 642e 7265 6c6f 6164 2829 3b72  board.reload();r
-00001970: 3600 0000 7250 0000 0072 3600 0000 7236  6...rP...r6...r6
-00001980: 0000 0072 3700 0000 da09 7265 6c6f 6164  ...r7.....reload
-00001990: 5f6a 73e2 0000 0073 0200 0000 0401 7a12  _js....s......z.
-000019a0: 5265 6e64 6572 6572 2e72 656c 6f61 645f  Renderer.reload_
-000019b0: 6a73 6302 0000 0000 0000 0000 0000 0006  jsc.............
-000019c0: 0000 0004 0000 004f 0000 0073 dc00 0000  .......O...s....
-000019d0: 7c01 6a00 6a01 6401 6b02 720f 7c00 6a02  |.j.j.d.k.r.|.j.
-000019e0: 6a03 7c02 6900 7c03 a401 8e01 5300 7c01  j.|.i.|.....S.|.
-000019f0: a004 a100 7d04 7c03 a005 7c04 6402 1900  ....}.|...|.d...
-00001a00: a101 0100 7406 7c03 7c01 8302 0100 7c01  ....t.|.|.....|.
-00001a10: 6a07 6403 7501 722c 7c03 a008 7409 6a0a  j.d.u.r,|...t.j.
-00001a20: 7c01 6a07 a102 0100 7c01 6a0b 6403 7501  |.j.....|.j.d.u.
-00001a30: 7239 7c03 a008 7409 6a0c 7c01 6a0b a102  r9|...t.j.|.j...
-00001a40: 0100 7c01 6a0d 6403 7501 725c 7c01 6a0d  ..|.j.d.u.r\|.j.
-00001a50: 6404 1900 7d05 7c05 a00e 6405 a101 7255  d...}.|...d...rU
-00001a60: 7c05 6406 6403 8502 1900 7d05 7c03 a008  |.d.d.....}.|...
-00001a70: 7409 6a0f 6407 a102 0100 7c03 a008 7409  t.j.d.....|...t.
-00001a80: 6a10 7c05 a102 0100 7c00 6a02 6a03 7c01  j.|.....|.j.j.|.
-00001a90: 6a00 6a11 7c01 6a00 6a01 6702 7c02 a201  j.j.|.j.j.g.|...
-00001aa0: 5200 6900 7c03 a401 8e01 5300 2908 7a20  R.i.|.....S.).z 
-00001ab0: 5573 6564 2066 6f72 2074 7572 6e20 7265  Used for turn re
-00001ac0: 7175 6573 7473 2069 6e74 6f20 7572 6c73  quests into urls
-00001ad0: da04 4d61 696e da0b 6261 7365 5f70 6172  ..Main..base_par
-00001ae0: 616d 734e 7201 0000 00da 012d 722c 0000  amsNr......-r,..
-00001af0: 00da 0444 4553 4329 1272 9800 0000 72b3  ...DESC).r....r.
-00001b00: 0000 0072 4000 0000 da0f 6275 696c 645f  ...r@.....build_
-00001b10: 706c 6169 6e5f 7572 6cda 0a67 6574 5f73  plain_url..get_s
-00001b20: 7461 7475 7372 7700 0000 7208 0000 00da  tatusrw...r.....
-00001b30: 066f 6666 7365 74da 0a73 6574 6465 6661  .offset..setdefa
-00001b40: 756c 7472 0c00 0000 da0f 5552 4c5f 5041  ultr......URL_PA
-00001b50: 5241 4d5f 5354 4152 54da 056c 696d 6974  RAM_START..limit
-00001b60: da0f 5552 4c5f 5041 5241 4d5f 4c49 4d49  ..URL_PARAM_LIMI
-00001b70: 54da 086f 7264 6572 5f62 79da 0a73 7461  T..order_by..sta
-00001b80: 7274 7377 6974 68da 1155 524c 5f50 4152  rtswith..URL_PAR
-00001b90: 414d 5f53 4f52 5444 4952 da0e 5552 4c5f  AM_SORTDIR..URL_
-00001ba0: 5041 5241 4d5f 534f 5254 da09 6170 705f  PARAM_SORT..app_
-00001bb0: 6c61 6265 6c29 0672 3f00 0000 da02 6172  label).r?.....ar
-00001bc0: da04 6172 6773 da02 6b77 da02 7374 da02  ..args..kw..st..
-00001bd0: 7363 7236 0000 0072 3600 0000 7237 0000  scr6...r6...r7..
-00001be0: 00da 0f67 6574 5f72 6571 7565 7374 5f75  ...get_request_u
-00001bf0: 726c e500 0000 732c 0000 000c 0212 0108  rl....s,........
-00001c00: 020e 010a 010a 0110 010a 0110 010a 010a  ................
-00001c10: 010a 010c 010e 010e 0106 030c 0102 ff02  ................
-00001c20: 0106 ff02 0106 ff7a 1852 656e 6465 7265  .......z.Rendere
-00001c30: 722e 6765 745f 7265 7175 6573 745f 7572  r.get_request_ur
-00001c40: 6c4e 6305 0000 0000 0000 0000 0000 0007  lNc.............
-00001c50: 0000 0005 0000 004b 0000 0073 ae00 0000  .......K...s....
-00001c60: 7c04 7005 7c03 a000 a100 7d04 7401 7c04  |.p.|.....}.t.|.
-00001c70: 8301 6401 6b02 7211 6402 a002 7c04 a101  ..d.k.r.d...|...
-00001c80: 7d04 7c03 6a03 6a04 722c 7c03 6a03 6a05  }.|.j.j.r,|.j.j.
-00001c90: 732c 7c00 a006 7c02 7c03 7c01 a103 7d06  s,|...|.|.|...}.
-00001ca0: 7c00 6a07 7c02 7c03 7c06 7c04 6604 6900  |.j.|.|.|.|.f.i.
-00001cb0: 7c05 a401 8e01 5300 7c03 6a03 6a08 724b  |.....S.|.j.j.rK
-00001cc0: 7c02 a009 a100 7d06 7c01 6400 7501 723f  |.....}.|.d.u.r?
-00001cd0: 7c06 6a0a 7c01 6a0b 6403 8d01 0100 7c00  |.j.|.j.d.....|.
-00001ce0: 6a07 7c02 7c03 7c06 7c04 6604 6900 7c05  j.|.|.|.|.f.i.|.
-00001cf0: a401 8e01 5300 7c00 6a0c 7c01 7c02 7c03  ....S.|.j.|.|.|.
-00001d00: 7c04 6604 6900 7c05 a401 8e01 5300 2904  |.f.i.|.....S.).
-00001d10: 4e72 2c00 0000 7506 0000 00c2 a07b 7dc2  Nr,...u......{}.
-00001d20: a029 01da 0972 6563 6f72 645f 6964 290d  .)...record_id).
-00001d30: da10 6765 745f 6275 7474 6f6e 5f6c 6162  ..get_button_lab
-00001d40: 656c da03 6c65 6eda 0666 6f72 6d61 7472  el..len..formatr
-00001d50: 6c00 0000 da0a 7061 7261 6d65 7465 7273  l.....parameters
-00001d60: da10 6e6f 5f70 6172 616d 735f 7769 6e64  ..no_params_wind
-00001d70: 6f77 da11 6765 745f 6163 7469 6f6e 5f73  ow..get_action_s
-00001d80: 7461 7475 73da 1477 696e 646f 775f 6163  tatus..window_ac
-00001d90: 7469 6f6e 5f62 7574 746f 6eda 0e6f 7065  tion_button..ope
-00001da0: 6e73 5f61 5f77 696e 646f 7772 be00 0000  ns_a_windowr....
-00001db0: 7277 0000 00da 0270 6bda 1172 6f77 5f61  rw.....pk..row_a
-00001dc0: 6374 696f 6e5f 6275 7474 6f6e 2907 723f  ction_button).r?
-00001dd0: 0000 00da 036f 626a 72c9 0000 0072 8f00  .....objr....r..
-00001de0: 0000 7295 0000 0072 cb00 0000 72cc 0000  ..r....r....r...
-00001df0: 0072 3600 0000 7236 0000 0072 3700 0000  .r6...r6...r7...
-00001e00: da0d 6163 7469 6f6e 5f62 7574 746f 6efd  ..action_button.
-00001e10: 0000 0073 2000 0000 0c01 0c01 0a01 1002  ...s ...........
-00001e20: 0e01 0401 0801 04ff 0201 06ff 0802 0801  ................
-00001e30: 0801 0e01 1801 1801 7a16 5265 6e64 6572  ........z.Render
-00001e40: 6572 2e61 6374 696f 6e5f 6275 7474 6f6e  er.action_button
-00001e50: 6305 0000 0000 0000 0000 0000 0007 0000  c...............
-00001e60: 0004 0000 004b 0000 0073 4000 0000 7c02  .....K...s@...|.
-00001e70: 6401 7500 720d 7c03 6a00 6402 6900 7c04  d.u.r.|.j.d.i.|.
-00001e80: a401 8e01 7d06 6e09 7c02 6a01 7c03 6601  ....}.n.|.j.|.f.
-00001e90: 6900 7c04 a401 8e01 7d06 7c00 6a02 7c06  i.|.....}.|.j.|.
-00001ea0: 7c01 6602 6900 7c05 a401 8e01 5300 2903  |.f.i.|.....S.).
-00001eb0: 61cf 0100 004e 6f74 6520 7468 6174 2060  a....Note that `
-00001ec0: 6261 2e61 6374 6f72 6020 6d61 7920 6469  ba.actor` may di
-00001ed0: 6666 6572 2066 726f 6d20 6061 722e 6163  ffer from `ar.ac
-00001ee0: 746f 7260 2077 6865 6e20 6465 6669 6e65  tor` when define
-00001ef0: 6420 6f6e 2061 0a20 2020 2020 2020 2064  d on a.        d
-00001f00: 6966 6665 7265 6e74 2061 6374 6f72 2e20  ifferent actor. 
-00001f10: 5265 6d65 6d62 6572 2065 2e67 2e20 7468  Remember e.g. th
-00001f20: 6520 224d 7573 7420 7265 6164 2065 4944  e "Must read eID
-00001f30: 2063 6172 6422 2061 6374 696f 6e0a 2020   card" action.  
-00001f40: 2020 2020 2020 6275 7474 6f6e 2069 6e20        button in 
-00001f50: 6569 645f 696e 666f 206f 6620 6e65 7763  eid_info of newc
-00001f60: 6f6d 6572 732e 4e65 7743 6c69 656e 7473  omers.NewClients
-00001f70: 2028 3230 3134 3034 3232 292e 0a0a 2020   (20140422)...  
-00001f80: 2020 2020 2020 3a6f 626a 3a20 2054 6865        :obj:  The
-00001f90: 2064 6174 6162 6173 6520 6f62 6a65 6374   database object
-00001fa0: 0a20 2020 2020 2020 203a 6172 3a20 2020  .        :ar:   
-00001fb0: 5468 6520 6163 7469 6f6e 2072 6571 7565  The action reque
-00001fc0: 7374 0a20 2020 2020 2020 203a 6261 3a20  st.        :ba: 
-00001fd0: 2054 6865 2062 6f75 6e64 2061 6374 696f   The bound actio
-00001fe0: 6e0a 2020 2020 2020 2020 3a72 6571 7565  n.        :reque
-00001ff0: 7374 5f6b 7761 7267 733a 206b 6579 776f  st_kwargs: keywo
-00002000: 7264 2061 7267 756d 656e 7473 2074 6f20  rd arguments to 
-00002010: 666f 7277 6172 6465 6420 746f 2074 6865  forwarded to the
-00002020: 2063 6869 6c64 2061 6374 696f 6e20 7265   child action re
-00002030: 7175 6573 740a 0a20 2020 2020 2020 2041  quest..        A
-00002040: 6e79 206b 6579 776f 7264 206f 7468 6572  ny keyword other
-00002050: 2061 7267 756d 656e 7473 2061 7265 2066   arguments are f
-00002060: 6f72 7761 7264 6564 2074 6f20 3a6d 6574  orwarded to :met
-00002070: 683a 6061 7232 6a73 602e 0a0a 2020 2020  h:`ar2js`...    
-00002080: 2020 2020 4e72 3600 0000 2903 da07 7265      Nr6...)...re
-00002090: 7175 6573 74da 0573 7061 776e da05 6172  quest..spawn..ar
-000020a0: 326a 7329 0772 3f00 0000 72da 0000 0072  2js).r?...r....r
-000020b0: c900 0000 728f 0000 00da 0e72 6571 7565  ....r......reque
-000020c0: 7374 5f6b 7761 7267 73da 0673 7461 7475  st_kwargs..statu
-000020d0: 73da 0373 6172 7236 0000 0072 3600 0000  s..sarr6...r6...
-000020e0: 7237 0000 00da 1761 6374 696f 6e5f 6361  r7.....action_ca
-000020f0: 6c6c 5f6f 6e5f 696e 7374 616e 6365 0e01  ll_on_instance..
-00002100: 0000 7308 0000 0008 0e12 0112 0314 017a  ..s............z
-00002110: 2052 656e 6465 7265 722e 6163 7469 6f6e   Renderer.action
-00002120: 5f63 616c 6c5f 6f6e 5f69 6e73 7461 6e63  _call_on_instanc
-00002130: 6563 0200 0000 0000 0000 0000 0000 0400  ec..............
-00002140: 0000 0400 0000 4300 0000 732c 0000 007c  ......C...s,...|
-00002150: 016a 0070 057c 016a 017d 0274 02a0 037c  .j.p.|.j.}.t...|
-00002160: 0264 01a1 027d 037c 0364 0175 0072 1264  .d...}.|.d.u.r.d
-00002170: 0153 0064 027c 0316 0053 0029 037a bf0a  .S.d.|...S.).z..
-00002180: 2020 2020 2020 2020 5573 6573 2061 6e20          Uses an 
-00002190: 696e 7465 726e 616c 206d 6170 7069 6e67  internal mapping
-000021a0: 2066 6f72 2069 636f 6e20 6e61 6d65 7320   for icon names 
-000021b0: 746f 2063 6f6e 7665 7274 2065 7869 7374  to convert exist
-000021c0: 696e 6720 6963 6f6e 7320 696e 746f 2072  ing icons into r
-000021d0: 6561 6374 2d75 7361 626c 652e 0a20 2020  eact-usable..   
-000021e0: 2020 2020 203a 7061 7261 6d20 6163 7469       :param acti
-000021f0: 6f6e 3a0a 2020 2020 2020 2020 3a72 6574  on:.        :ret
-00002200: 7572 6e3a 2073 7472 3a20 6120 6963 6f6e  urn: str: a icon
-00002210: 206e 616d 6520 666f 7220 6569 7468 6572   name for either
-00002220: 2070 7269 6d65 2d72 6561 6374 206f 7220   prime-react or 
-00002230: 6963 6f6e 380a 2020 2020 2020 2020 4e7a  icon8.        Nz
-00002240: 0570 6920 2573 2904 da0f 7265 6163 745f  .pi %s)...react_
-00002250: 6963 6f6e 5f6e 616d 65da 0969 636f 6e5f  icon_name..icon_
-00002260: 6e61 6d65 722d 0000 00da 0367 6574 2904  namer-.....get).
-00002270: 723f 0000 0072 6c00 0000 729f 0000 00da  r?...rl...r.....
-00002280: 0a72 6561 6374 5f69 636f 6e72 3600 0000  .react_iconr6...
-00002290: 7236 0000 0072 3700 0000 72a4 0000 0023  r6...r7...r....#
-000022a0: 0100 0073 0a00 0000 0c07 0c01 0801 0401  ...s............
-000022b0: 0802 7a18 5265 6e64 6572 6572 2e67 6574  ..z.Renderer.get
-000022c0: 5f61 6374 696f 6e5f 6963 6f6e 6303 0000  _action_iconc...
-000022d0: 0000 0000 0000 0000 0008 0000 0007 0000  ................
-000022e0: 004b 0000 0073 a400 0000 7c01 6a00 7d04  .K...s....|.j.}.
-000022f0: 7c01 6a01 7d05 6900 7d06 7c05 6a02 a003  |.j.}.i.}.|.j...
-00002300: a100 721c 7c03 a004 7c00 a005 7c01 7c05  ..r.|...|...|.|.
-00002310: 7c02 a103 a101 0100 7c06 a004 7c03 a101  |.......|...|...
-00002320: 0100 7c06 a004 7c00 a006 7c01 7c05 7c02  ..|...|...|.|.|.
-00002330: a103 a101 0100 7c06 a004 7c03 a101 0100  ......|...|.....
-00002340: 7c04 7c05 6a02 6a07 7c01 6a08 7c05 6a09  |.|.j.j.|.j.|.j.
-00002350: 6a0a 7c06 6401 9c05 7d07 740b 7c02 6402  j.|.d...}.t.|.d.
-00002360: 8302 7243 7c02 6a0c 7c07 6403 3c00 6e09  ..rC|.j.|.d.<.n.
-00002370: 740d 7c02 740e 8302 724c 7c02 7c07 6403  t.|.t...rL|.|.d.
-00002380: 3c00 6404 740f 7c07 8301 1600 5300 2905  <.d.t.|.....S.).
-00002390: 7a43 496d 706c 656d 656e 7473 203a 6d65  zCImplements :me
-000023a0: 7468 3a60 6c69 6e6f 2e63 6f72 652e 7265  th:`lino.core.re
-000023b0: 6e64 6572 6572 2e48 746d 6c52 656e 6465  nderer.HtmlRende
-000023c0: 7265 722e 6172 326a 7360 2e0a 0a20 2020  rer.ar2js`...   
-000023d0: 2020 2020 2029 05da 0272 7072 9400 0000       )...rpr....
-000023e0: da06 6f6e 4d61 696e da07 6163 746f 7249  ..onMain..actorI
-000023f0: 6472 e000 0000 72d8 0000 00da 0273 72fa  dr....r......sr.
-00002400: 1877 696e 646f 772e 4170 702e 7275 6e41  .window.App.runA
-00002410: 6374 696f 6e28 2573 2929 10da 1072 6571  ction(%s))...req
-00002420: 7565 7374 696e 675f 7061 6e65 6c72 a300  uesting_panelr..
-00002430: 0000 726c 0000 0072 a200 0000 7277 0000  ..rl...r....rw..
-00002440: 0072 d500 0000 da11 6765 745f 6163 7469  .r......get_acti
-00002450: 6f6e 5f70 6172 616d 7372 4d00 0000 da10  on_paramsrM.....
-00002460: 6973 5f6f 6e5f 6d61 696e 5f61 6374 6f72  is_on_main_actor
-00002470: 7298 0000 00da 0861 6374 6f72 5f69 6472  r......actor_idr
-00002480: 8200 0000 72d8 0000 0072 a000 0000 7278  ....r....r....rx
-00002490: 0000 0072 2600 0000 2908 723f 0000 0072  ...r&...).r?...r
-000024a0: c900 0000 72da 0000 0072 e000 0000 72e7  ....r....r....r.
-000024b0: 0000 0072 8f00 0000 da06 7061 7261 6d73  ...r......params
-000024c0: da06 6a73 5f6f 626a 7236 0000 0072 3600  ..js_objr6...r6.
-000024d0: 0000 7237 0000 0072 de00 0000 3101 0000  ..r7...r....1...
-000024e0: 732a 0000 0006 0406 0104 010a 0114 040a  s*..............
-000024f0: 0114 010a 0102 0306 0104 0106 0102 0106  ................
-00002500: fb0a 070c 010a 0208 0102 0206 0104 ff7a  ...............z
-00002510: 0e52 656e 6465 7265 722e 6172 326a 7363  .Renderer.ar2jsc
-00002520: 0200 0000 0000 0000 0000 0000 0600 0000  ................
-00002530: 0600 0000 4300 0000 73bc 0100 007c 0174  ....C...s....|.t
-00002540: 006a 016a 0275 0072 0a74 0364 0183 0153  .j.j.u.r.t.d...S
-00002550: 0074 047c 0174 0583 0272 1674 0664 02a0  .t.|.t...r.t.d..
-00002560: 077c 01a1 0183 0182 0174 047c 0174 086a  .|.......t.|.t.j
-00002570: 0983 0272 2009 007c 016a 0a53 0074 047c  ...r ..|.j.S.t.|
-00002580: 0174 0b6a 0c83 0272 297c 016a 0d53 0074  .t.j...r)|.j.S.t
-00002590: 047c 0174 0683 0272 3274 0e7c 0183 0153  .|.t...r2t.|...S
-000025a0: 0074 047c 0174 0f83 0272 4a7c 016a 1064  .t.|.t...rJ|.j.d
-000025b0: 0375 0072 3f7c 016a 1153 0074 127c 016a  .u.r?|.j.S.t.|.j
-000025c0: 1374 127c 016a 1164 048d 0164 058d 0253  .t.|.j.d...d...S
-000025d0: 0074 047c 0174 1483 0272 cc7c 016a 1564  .t.|.t...r.|.j.d
-000025e0: 0375 0172 6d7c 00a0 1664 037c 016a 1564  .u.rm|...d.|.j.d
-000025f0: 03a1 037d 027c 0264 0375 0173 624a 0082  ...}.|.d.u.sbJ..
-00002600: 0164 067c 0216 007d 037c 00a0 177c 017c  .d.|...}.|...|.|
-00002610: 0264 03a1 0353 007c 016a 1864 0375 0172  .d...S.|.j.d.u.r
-00002620: 957c 016a 1972 857c 016a 186a 1a64 0d69  .|.j.r.|.j.j.d.i
-00002630: 007c 016a 19a4 018e 017d 047c 00a0 1b7c  .|.j.....}.|...|
-00002640: 04a1 017d 036e 087c 00a0 1c64 037c 016a  ...}.n.|...d.|.j
-00002650: 1869 00a1 037d 037c 00a0 177c 017c 037c  .i...}.|...|.|.|
-00002660: 016a 1da1 0353 007c 016a 1e64 0375 0172  .j...S.|.j.d.u.r
-00002670: a764 067c 016a 1e16 007d 037c 00a0 177c  .d.|.j...}.|...|
-00002680: 017c 037c 016a 1da1 0353 007c 016a 1f64  .|.|.j...S.|.j.d
-00002690: 0375 0172 b07c 016a 1f7d 056e 037c 016a  .u.r.|.j.}.n.|.j
-000026a0: 1353 007c 016a 106a 1064 0375 0072 c574  .S.|.j.j.d.u.r.t
-000026b0: 1264 077c 016a 1374 0364 087c 0516 0083  .d.|.j.t.d.|....
-000026c0: 0164 098d 0353 0074 127c 016a 137c 0564  .d...S.t.|.j.|.d
-000026d0: 0a8d 0253 0074 047c 0174 0383 0272 dc74  ...S.t.|.t...r.t
-000026e0: 207c 0064 0b64 0c83 0372 dc74 0e7c 016a   |.d.d...r.t.|.j
-000026f0: 2183 0153 007c 0153 0029 0e7a 540a 2020  !..S.|.S.).zT.  
-00002700: 2020 2020 2020 4164 6469 7469 6f6e 616c        Additional
-00002710: 2063 6f6e 7665 7274 696e 6720 6c6f 6769   converting logi
-00002720: 6320 666f 7220 7365 7269 616c 697a 696e  c for serializin
-00002730: 6720 5079 7468 6f6e 2076 616c 7565 7320  g Python values 
-00002740: 746f 206a 736f 6e2e 0a20 2020 2020 2020  to json..       
-00002750: 20da 104c 414e 4755 4147 455f 4348 4f49   ..LANGUAGE_CHOI
-00002760: 4345 537a 0b32 3032 3130 3531 3720 7b7d  CESz.20210517 {}
-00002770: 4e29 0172 6800 0000 2902 7244 0000 0072  N).rh...).rD...r
-00002780: 5500 0000 7a02 2573 da06 6275 7474 6f6e  U...z.%s..button
-00002790: 7a23 6675 6e63 7469 6f6e 2829 207b 204c  z#function() { L
-000027a0: 696e 6f2e 6c6f 6164 5f75 726c 2827 2573  ino.load_url('%s
-000027b0: 2729 3b20 7d29 03da 0578 7479 7065 7244  '); })...xtyperD
-000027c0: 0000 00da 0768 616e 646c 6572 2902 7244  .....handler).rD
-000027d0: 0000 00da 0468 7265 6672 6e00 0000 4672  .....hrefrn...Fr
-000027e0: 3600 0000 2922 7204 0000 0072 6f00 0000  6...)"r....ro...
-000027f0: 72f2 0000 0072 2700 0000 72a0 0000 0072  r....r'...r....r
-00002800: 1c00 0000 da09 4578 6365 7074 696f 6e72  ......Exceptionr
-00002810: d200 0000 720d 0000 00da 0643 686f 6963  ....r......Choic
-00002820: 6572 4300 0000 7205 0000 00da 054d 6f64  erC...r......Mod
-00002830: 656c 72d8 0000 0072 4500 0000 720a 0000  elr....rE...r...
-00002840: 00da 0670 6172 656e 7472 6800 0000 7271  ...parentrh...rq
-00002850: 0000 0072 9500 0000 720b 0000 00da 0869  ...r....r......i
-00002860: 6e73 7461 6e63 65da 1069 6e73 7461 6e63  nstance..instanc
-00002870: 655f 6861 6e64 6c65 72da 0c68 616e 646c  e_handler..handl
-00002880: 6572 5f69 7465 6d72 a300 0000 72f0 0000  er_itemr....r...
-00002890: 0072 dc00 0000 da0f 7265 7175 6573 745f  .r......request_
-000028a0: 6861 6e64 6c65 72da 0b61 6374 696f 6e5f  handler..action_
-000028b0: 6361 6c6c 72b2 0000 00da 0a6a 6176 6173  callr......javas
-000028c0: 6372 6970 7472 f600 0000 da07 6765 7461  criptr......geta
-000028d0: 7474 72da 0173 2906 723f 0000 0072 a500  ttr..s).r?...r..
-000028e0: 0000 da01 68da 026a 7372 c900 0000 da03  ....h..jsr......
-000028f0: 7572 6c72 3600 0000 7236 0000 0072 3700  urlr6...r6...r7.
-00002900: 0000 723e 0000 0052 0100 0073 5400 0000  ..r>...R...sT...
-00002910: 0c04 0801 0a01 0e01 0c01 0201 0603 0c01  ................
-00002920: 0601 0a01 0801 0a01 0a01 0601 1603 0a02  ................
-00002930: 0a01 1001 0c01 0801 0e01 0a01 0601 1401  ................
-00002940: 0c01 1002 1001 0a02 0a01 1001 0a01 0801  ................
-00002950: 0607 0c02 0202 0601 0a02 06fd 0e04 1602  ................
-00002960: 0a02 0402 7a18 5265 6e64 6572 6572 2e70  ....z.Renderer.p
-00002970: 7932 6a73 5f63 6f6e 7665 7274 6572 6304  y2js_converterc.
-00002980: 0000 0000 0000 0000 0000 0005 0000 0004  ................
-00002990: 0000 0043 0000 0073 5000 0000 7400 7c01  ...C...sP...t.|.
-000029a0: 6a01 7c02 6401 8d02 7d04 7c01 6a02 721a  j.|.d...}.|.j.r.
-000029b0: 7c01 6a02 6a03 6a04 721a 7c04 6a05 6402  |.j.j.j.r.|.j.d.
-000029c0: 7c01 6a02 6a03 6a04 1700 6403 8d01 0100  |.j.j.j...d.....
-000029d0: 7406 6a07 6a08 7226 7c03 7226 7c04 6a05  t.j.j.r&|.r&|.j.
-000029e0: 7c03 6404 8d01 0100 7c04 5300 2905 da00  |.d.....|.S.)...
-000029f0: 2902 7244 0000 0072 f500 0000 7a07 782d  ).rD...r....z.x-
-00002a00: 7462 6172 2d29 01da 0769 636f 6e43 6c73  tbar-)...iconCls
-00002a10: 2901 da07 746f 6f6c 5469 7029 0972 7100  )...toolTip).rq.
-00002a20: 0000 7295 0000 0072 a300 0000 726c 0000  ..r....r....rl..
-00002a30: 0072 e400 0000 7277 0000 0072 0400 0000  .r....rw...r....
-00002a40: 726f 0000 00da 0d75 7365 5f71 7569 636b  ro.....use_quick
-00002a50: 7469 7073 2905 723f 0000 00da 026d 6972  tips).r?.....mir
-00002a60: f500 0000 72b2 0000 00da 0164 7236 0000  ....r......dr6..
-00002a70: 0072 3600 0000 7237 0000 0072 fd00 0000  .r6...r7...r....
-00002a80: a001 0000 730c 0000 000e 0410 0116 010c  ....s...........
-00002a90: 010c 0304 017a 1552 656e 6465 7265 722e  .....z.Renderer.
-00002aa0: 6861 6e64 6c65 725f 6974 656d 6302 0000  handler_itemc...
-00002ab0: 0000 0000 0000 0000 0005 0000 0005 0000  ................
-00002ac0: 004f 0000 0073 2000 0000 7c01 6a00 6402  .O...s ...|.j.d.
-00002ad0: 6900 7c03 a401 8e01 7d04 7c00 a001 7c01  i.|.....}.|...|.
-00002ae0: 7c01 6a02 7c04 a103 5300 2903 7a36 2047  |.j.|...S.).z6 G
-00002af0: 656e 6572 6174 6573 206a 7320 7374 7269  enerates js stri
-00002b00: 6e67 2066 6f72 2061 6374 696f 6e20 6275  ng for action bu
-00002b10: 7474 6f6e 2063 616c 6c73 2e0a 2020 2020  tton calls..    
-00002b20: 2020 2020 4e72 3600 0000 2903 72be 0000      Nr6...).r...
-00002b30: 0072 ff00 0000 72a3 0000 0029 0572 3f00  .r....r....).r?.
-00002b40: 0000 72c9 0000 0072 ca00 0000 72cb 0000  ..r....r....r...
-00002b50: 0072 cc00 0000 7236 0000 0072 3600 0000  .r....r6...r6...
-00002b60: 7237 0000 0072 fe00 0000 ae01 0000 7304  r7...r........s.
-00002b70: 0000 0010 0410 017a 1852 656e 6465 7265  .......z.Rendere
-00002b80: 722e 7265 7175 6573 745f 6861 6e64 6c65  r.request_handle
-00002b90: 7263 0400 0000 0000 0000 0000 0000 0800  rc..............
-00002ba0: 0000 0800 0000 4300 0000 739c 0000 007c  ......C...s....|
-00002bb0: 026a 007d 047c 02a0 01a1 00a0 0264 0164  .j.}.|.......d.d
-00002bc0: 02a1 025c 027d 057d 067c 0373 1169 007d  ...\.}.}.|.s.i.}
-00002bd0: 037c 0164 0075 0172 2274 037c 0164 0383  .|.d.u.r"t.|.d..
-00002be0: 0272 227c 016a 0464 0869 007c 03a4 018e  .r"|.j.d.i.|....
-00002bf0: 017d 037c 0172 2d7c 016a 0572 2d7c 016a  .}.|.r-|.j.r-|.j
-00002c00: 057c 0374 066a 073c 007c 0664 046b 0272  .|.t.j.<.|.d.k.r
-00002c10: 3974 037c 0364 0583 0272 397c 0364 053d  9t.|.d...r9|.d.=
-00002c20: 007c 0164 0075 0072 3f64 006e 027c 016a  .|.d.u.r?d.n.|.j
-00002c30: 087d 0764 0674 0974 0a7c 067c 057c 037c  .}.d.t.t.|.|.|.|
-00002c40: 0764 078d 0483 0116 0053 0029 094e da01  .d.......S.).N..
-00002c50: 2e72 2c00 0000 72be 0000 00da 0467 7269  .r,...r......gri
-00002c60: 6472 cf00 0000 72eb 0000 0029 0472 9400  dr....r....).r..
-00002c70: 0000 72e9 0000 0072 e000 0000 72e7 0000  ..r....r....r...
-00002c80: 0072 3600 0000 290b 726c 0000 00da 0966  .r6...).rl.....f
-00002c90: 756c 6c5f 6e61 6d65 da06 7273 706c 6974  ull_name..rsplit
-00002ca0: 7282 0000 0072 be00 0000 da0a 7375 6273  r....r......subs
-00002cb0: 745f 7573 6572 720c 0000 00da 1455 524c  t_userr......URL
-00002cc0: 5f50 4152 414d 5f53 5542 5354 5f55 5345  _PARAM_SUBST_USE
-00002cd0: 5272 ec00 0000 7226 0000 0072 7100 0000  Rr....r&...rq...
-00002ce0: 2908 723f 0000 0072 c900 0000 72a3 0000  ).r?...r....r...
-00002cf0: 0072 e000 0000 724f 0000 0072 e900 0000  .r....rO...r....
-00002d00: 7294 0000 0072 e700 0000 7236 0000 0072  r....r....r6...r
-00002d10: 3600 0000 7237 0000 0072 ff00 0000 b801  6...r7...r......
-00002d20: 0000 7322 0000 0006 0214 0204 0204 0112  ..s"............
-00002d30: 0210 010a 020c 0112 1106 0112 0206 0202  ................
-00002d40: 0102 0102 0102 010a fc7a 1452 656e 6465  .........z.Rende
-00002d50: 7265 722e 6163 7469 6f6e 5f63 616c 6c63  rer.action_callc
-00002d60: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00002d70: 0400 0000 4300 0000 732e 0000 007c 0173  ....C...s....|.s
-00002d80: 0464 0053 0074 007c 0174 0183 0273 0d74  .d.S.t.|.t...s.t
-00002d90: 017c 0183 017d 0174 027c 0164 0164 028d  .|...}.t.|.d.d..
-00002da0: 027d 0164 037c 0117 0053 0029 044e 4629  .}.d.|...S.).NF)
-00002db0: 01da 0571 756f 7465 7a0b 6a61 7661 7363  ...quotez.javasc
-00002dc0: 7269 7074 3a29 0372 a000 0000 7245 0000  ript:).r....rE..
-00002dd0: 0072 0300 0000 2902 723f 0000 0072 0401  .r....).r?...r..
-00002de0: 0000 7236 0000 0072 3600 0000 7237 0000  ..r6...r6...r7..
-00002df0: 00da 066a 7332 7572 6ce2 0100 0073 0c00  ...js2url....s..
-00002e00: 0000 0401 0401 0a02 0801 0c01 0801 7a0f  ..............z.
-00002e10: 5265 6e64 6572 6572 2e6a 7332 7572 6c63  Renderer.js2urlc
-00002e20: 0600 0000 0000 0000 0000 0000 0700 0000  ................
-00002e30: 0400 0000 4300 0000 7356 0000 0074 006a  ....C...sV...t.j
-00002e40: 016a 0272 2774 006a 016a 0372 0f64 017c  .j.r't.j.j.r.d.|
-00002e50: 047c 0566 0216 007d 066e 0264 027d 067c  .|.f...}.n.d.}.|
-00002e60: 0272 1974 0464 037c 067c 0283 037d 067c  .r.t.d.|.|...}.|
-00002e70: 0672 297c 016a 0564 047c 037c 0666 0216  .r)|.j.d.|.|.f..
-00002e80: 0064 058d 0101 0064 0053 0064 0053 0064  .d.....d.S.d.S.d
-00002e90: 0053 0029 064e 7a08 2825 732e 2573 2920  .S.).Nz.(%s.%s) 
-00002ea0: 7206 0100 007a 047b 7d7b 7d7a 0728 2573  r....z.{}{}z.(%s
-00002eb0: 2c25 7329 2901 da08 7175 6963 6b74 6970  ,%s))...quicktip
-00002ec0: 2906 7204 0000 0072 6f00 0000 7209 0100  ).r....ro...r...
-00002ed0: 00da 1973 686f 775f 696e 7465 726e 616c  ...show_internal
-00002ee0: 5f66 6965 6c64 5f6e 616d 6573 7206 0000  _field_namesr...
-00002ef0: 0072 7700 0000 2907 723f 0000 0072 cb00  .rw...).r?...r..
-00002f00: 0000 72b2 0000 0072 7400 0000 da0a 6461  ..r....rt.....da
-00002f10: 7461 736f 7572 6365 da09 6669 656c 646e  tasource..fieldn
-00002f20: 616d 65da 0374 7474 7236 0000 0072 3600  ame..tttr6...r6.
-00002f30: 0000 7237 0000 00da 0d61 6464 5f68 656c  ..r7.....add_hel
-00002f40: 705f 7465 7874 eb01 0000 7318 0000 0008  p_text....s.....
-00002f50: 0108 010e 0104 0204 010c 0104 0108 0402  ................
-00002f60: 010e ff04 f504 077a 1652 656e 6465 7265  .......z.Rendere
-00002f70: 722e 6164 645f 6865 6c70 5f74 6578 7463  r.add_help_textc
-00002f80: 0200 0000 0000 0000 0000 0000 0500 0000  ................
-00002f90: 0300 0000 4300 0000 7356 0000 0074 0083  ....C...sV...t..
-00002fa0: 007d 0264 017c 0117 0064 0217 007d 037c  .}.d.|...d...}.|
-00002fb0: 006a 01a0 0264 03a1 0164 0419 007d 047c  .j...d...d...}.|
-00002fc0: 0264 0575 0172 1c7c 037c 026a 0364 0217  .d.u.r.|.|.j.d..
-00002fd0: 0037 007d 037c 0374 04a0 05a1 0064 0317  .7.}.|.t.....d..
-00002fe0: 007c 0417 0037 007d 0364 067c 047c 0366  .|...7.}.d.|.|.f
-00002ff0: 0353 0029 077a 2c4c 696b 6520 6c69 6e6f  .S.).z,Like lino
-00003000: 5f6a 735f 7061 7274 732c 2062 7574 2066  _js_parts, but f
-00003010: 6f72 2061 6374 6f72 5f6c 6576 656c 2064  or actor_level d
-00003020: 6174 61da 054c 696e 6f5f da01 5f72 0c01  ata..Lino_.._r..
-00003030: 0000 722e 0000 004e da05 6361 6368 6529  ..r....N..cache)
-00003040: 0672 2900 0000 da11 6c69 6e6f 5f77 6562  .r).....lino_web
-00003050: 5f74 656d 706c 6174 6572 0f01 0000 7243  _templater....rC
-00003060: 0000 0072 0700 0000 da0c 6765 745f 6c61  ...r......get_la
-00003070: 6e67 7561 6765 2905 723f 0000 0072 e900  nguage).r?...r..
-00003080: 0000 da09 7573 6572 5f74 7970 65da 0866  ....user_type..f
-00003090: 696c 656e 616d 65da 0966 696c 655f 7479  ilename..file_ty
-000030a0: 7065 7236 0000 0072 3600 0000 7237 0000  per6...r6...r7..
-000030b0: 00da 156c 696e 6f5f 6a73 5f70 6172 7473  ...lino_js_parts
-000030c0: 5f63 6875 6e6b 6564 fa01 0000 730e 0000  _chunked....s...
-000030d0: 0006 020c 0110 0108 010e 0114 010a 017a  ...............z
-000030e0: 1e52 656e 6465 7265 722e 6c69 6e6f 5f6a  .Renderer.lino_j
-000030f0: 735f 7061 7274 735f 6368 756e 6b65 6463  s_parts_chunkedc
-00003100: 0200 0000 0000 0000 0000 0000 1100 0000  ................
-00003110: 0600 0000 4300 0000 73de 0100 0067 007d  ....C...s....g.}
-00003120: 0267 007d 037c 0144 005d e47d 047c 04a0  .g.}.|.D.].}.|..
-00003130: 00a1 007d 057c 0573 127c 046a 016a 0272  ...}.|.s.|.j.j.r
-00003140: cc74 036a 047c 046a 016a 0569 017d 067c  .t.j.|.j.j.i.}.|
-00003150: 0572 237c 066a 067c 056a 076a 0864 018d  .r#|.j.|.j.j.d..
-00003160: 0101 007c 046a 016a 0272 c767 007d 0774  ...|.j.j.r.g.}.t
-00003170: 0983 007d 087c 046a 0aa0 0b7c 046a 0174  ...}.|.j...|.j.t
-00003180: 0c83 00a1 0244 005d 727d 0974 097c 096a  .....D.]r}.t.|.j
-00003190: 016a 0564 028d 017d 0a7c 096a 016a 0d7d  .j.d...}.|.j.j.}
-000031a0: 0b7c 0b72 487c 0b7c 0a64 033c 007c 096a  .|.rH|.|.d.<.|.j
-000031b0: 016a 0e7d 0c7c 0c72 5e74 0f7c 0c83 0172  .j.}.|.r^t.|...r
-000031c0: 5a7c 0c7c 096a 0a83 017c 0a64 043c 006e  Z|.|.j...|.d.<.n
-000031d0: 047c 0c7c 0a64 043c 007c 096a 016a 1064  .|.|.d.<.|.j.j.d
-000031e0: 0575 0172 847c 096a 016a 107d 0d7c 0d7c  .u.r.|.j.j.}.|.|
-000031f0: 0876 0072 747c 087c 0d19 00a0 117c 0aa1  .v.rt|.|.....|..
-00003200: 0101 006e 1574 097c 0d64 068d 017d 0e7c  ...n.t.|.d...}.|
-00003210: 0a67 017c 087c 0d3c 007c 07a0 117c 0ea1  .g.|.|.<.|...|..
-00003220: 0101 006e 057c 07a0 117c 0aa1 0101 007c  ...n.|...|.....|
-00003230: 096a 016a 1272 a774 137c 096a 016a 1283  .j.j.r.t.|.j.j..
-00003240: 017d 0f74 147c 0f64 0783 0273 9e7c 096a  .}.t.|.d...s.|.j
-00003250: 016a 057c 0f64 073c 007c 0f7c 0376 0172  .j.|.d.<.|.|.v.r
-00003260: a77c 03a0 117c 0fa1 0101 0071 357c 0872  .|...|.....q5|.r
-00003270: c374 157c 0783 0144 005d 145c 027d 107d  .t.|...D.].\.}.}
-00003280: 0a7c 0aa0 1664 0864 09a1 0272 c27c 087c  .|...d.d...r.|.|
-00003290: 0a64 0819 0019 007c 077c 1019 0064 0a3c  .d.....|.|...d.<
-000032a0: 0071 ae7c 077c 0664 0b3c 007c 02a0 117c  .q.|.|.d.<.|...|
-000032b0: 06a1 0101 007c 046a 016a 1272 ea74 137c  .....|.j.j.r.t.|
-000032c0: 046a 016a 1283 017d 0f74 147c 0f64 0783  .j.j...}.t.|.d..
-000032d0: 0273 e17c 046a 016a 057c 0f64 073c 007c  .s.|.j.j.|.d.<.|
-000032e0: 0f7c 0376 0172 ea7c 03a0 117c 0fa1 0101  .|.v.r.|...|....
-000032f0: 0071 067c 027c 0366 0253 0029 0c7a 4543  .q.|.|.f.S.).zEC
-00003300: 6f6e 7665 7274 7320 6f66 2061 6c6c 2074  onverts of all t
-00003310: 6865 2062 6f75 6e64 6163 7469 6f6e 7320  he boundactions 
-00003320: 6f66 2061 6e20 6163 746f 7220 746f 206a  of an actor to j
-00003330: 736f 6e20 666f 726d 6174 2e0a 2020 2020  son format..    
-00003340: 2020 2020 a901 7265 0000 0029 0172 9400      ..re...).r..
-00003350: 0000 72b2 0000 00da 0a6a 735f 6861 6e64  ..r......js_hand
-00003360: 6c65 724e 2901 da05 636f 6d62 6f72 8f00  lerN)...combor..
-00003370: 0000 7225 0100 0046 7255 0000 00da 0e74  ..r%...FrU.....t
-00003380: 6f6f 6c62 6172 4163 7469 6f6e 7329 17da  oolbarActions)..
-00003390: 1167 6574 5f6c 6179 6f75 745f 6861 6e64  .get_layout_hand
-000033a0: 656c 726c 0000 00da 0b77 696e 646f 775f  elrl.....window_
-000033b0: 7479 7065 720c 0000 00da 1555 524c 5f50  typer......URL_P
-000033c0: 4152 414d 5f41 4354 494f 4e5f 4e41 4d45  ARAM_ACTION_NAME
-000033d0: 724d 0000 0072 7700 0000 72ab 0000 0072  rM...rw...r....r
-000033e0: 8700 0000 7271 0000 0072 9800 0000 da13  ....rq...r......
-000033f0: 6765 745f 746f 6f6c 6261 725f 6163 7469  get_toolbar_acti
-00003400: 6f6e 7372 2900 0000 72b2 0000 0072 2401  onsr)...r....r$.
-00003410: 0000 722f 0000 00da 0b63 6f6d 626f 5f67  ..r/.....combo_g
-00003420: 726f 7570 da06 6170 7065 6e64 da06 686f  roup..append..ho
-00003430: 746b 6579 da04 7661 7273 7282 0000 0072  tkey..varsr....r
-00003440: 3000 0000 72e5 0000 0029 1172 3f00 0000  0...r....).r?...
-00003450: da0c 6163 7469 6f6e 735f 6c69 7374 72a6  ..actions_listr.
-00003460: 0000 00da 0768 6f74 6b65 7973 728f 0000  .....hotkeysr...
-00003470: 00da 026c 68da 1161 6374 696f 6e5f 6465  ...lh..action_de
-00003480: 7363 7269 7074 6f72 da04 7462 6173 da09  scriptor..tbas..
-00003490: 636f 6d62 6f5f 6d61 7072 4f00 0000 da03  combo_maprO.....
-000034a0: 7462 6172 b200 0000 7224 0100 0072 2b01  tbar....r$...r+.
-000034b0: 0000 7225 0100 0072 2d01 0000 7234 0000  ..r%...r-...r4..
-000034c0: 0072 3600 0000 7236 0000 0072 3700 0000  .r6...r6...r7...
-000034d0: da0c 6163 7469 6f6e 7332 6a73 6f6e 0402  ..actions2json..
-000034e0: 0000 7368 0000 0004 0404 0108 0208 010c  ..sh............
-000034f0: 010e 0204 0110 0108 0104 0106 0106 0208  ................
-00003500: 0108 ff0e 0308 010c 0108 0104 0108 0110  ................
-00003510: 0108 020c 0208 0108 0210 010a 020a 010c  ................
-00003520: 010a 0208 020c 010a 010c 0108 010a 0102  ................
-00003530: 8004 0210 010c 0114 0102 8008 020a 0208  ................
-00003540: 020c 010a 010c 0108 010a 0102 8008 027a  ...............z
-00003550: 1552 656e 6465 7265 722e 6163 7469 6f6e  .Renderer.action
-00003560: 7332 6a73 6f6e 6302 0000 0000 0000 0000  s2jsonc.........
-00003570: 0000 0005 0000 0005 0000 0043 0000 0073  ...........C...s
-00003580: 5800 0000 6700 7d02 6400 7d03 7c01 4400  X...g.}.d.}.|.D.
-00003590: 5d14 7d04 7c04 6401 1900 6400 7500 7213  ].}.|.d...d.u.r.
-000035a0: 7c04 6402 1900 7d03 7106 7c02 a000 7401  |.d...}.q.|...t.
-000035b0: 7c04 8301 a101 0100 7106 7402 7c02 6403  |.......q.t.|.d.
-000035c0: 6404 8400 6405 8d02 7d02 7c02 a000 6400  d...d...}.|...d.
-000035d0: 7c03 6702 a101 0100 7c02 5300 2906 4e72  |.g.....|.S.).Nr
-000035e0: 0100 0000 722c 0000 0063 0100 0000 0000  ....r,...c......
-000035f0: 0000 0000 0000 0100 0000 0200 0000 5300  ..............S.
-00003600: 0000 7308 0000 007c 0064 0119 0053 0029  ..s....|.d...S.)
-00003610: 024e 7201 0000 0072 3600 0000 2901 7235  .Nr....r6...).r5
-00003620: 0000 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
-00003630: 0000 da08 3c6c 616d 6264 613e 5002 0000  ....<lambda>P...
-00003640: 7302 0000 0008 007a 2c52 656e 6465 7265  s......z,Rendere
-00003650: 722e 6469 7370 6c61 795f 6d6f 6465 326a  r.display_mode2j
-00003660: 736f 6e2e 3c6c 6f63 616c 733e 2e3c 6c61  son.<locals>.<la
-00003670: 6d62 6461 3ea9 0172 3300 0000 2903 722c  mbda>..r3...).r,
-00003680: 0100 0072 7800 0000 da06 736f 7274 6564  ...rx.....sorted
-00003690: 2905 723f 0000 00da 0c64 6973 706c 6179  ).r?.....display
-000036a0: 5f6d 6f64 65da 0364 6d73 da03 646d 6472  _mode..dms..dmdr
-000036b0: 9200 0000 7236 0000 0072 3600 0000 7237  ....r6...r6...r7
-000036c0: 0000 00da 1164 6973 706c 6179 5f6d 6f64  .....display_mod
-000036d0: 6532 6a73 6f6e 4802 0000 7312 0000 0004  e2jsonH...s.....
-000036e0: 0104 0108 010c 010a 0110 0210 010e 0104  ................
-000036f0: 017a 1a52 656e 6465 7265 722e 6469 7370  .z.Renderer.disp
-00003700: 6c61 795f 6d6f 6465 326a 736f 6e63 0200  lay_mode2jsonc..
-00003710: 0000 0000 0000 0000 0000 1100 0000 0800  ................
-00003720: 0000 4300 0000 73fe 0200 0074 007c 0183  ..C...s....t.|..
-00003730: 0172 0974 017c 0174 0283 0273 0b4a 0082  .r.t.|.t...s.J..
-00003740: 017c 00a0 037c 016a 04a1 015c 027d 027d  .|...|.j...\.}.}
-00003750: 0374 057c 016a 067c 027c 01a0 07a1 0074  .t.|.j.|.|.....t
-00003760: 087c 016a 0983 017c 01a0 0a74 0b83 00a1  .|.j...|...t....
-00003770: 010c 0064 018d 057d 0474 0c7c 0383 0172  ...d...}.t.|...r
-00003780: 317c 046a 0d7c 0364 028d 0101 007c 01a0  1|.j.|.d.....|..
-00003790: 0ea1 007d 057c 056a 0f64 0075 0072 4374  ...}.|.j.d.u.rCt
-000037a0: 106a 116a 12a0 1364 037c 01a1 0201 006e  .j.j...d.|.....n
-000037b0: 5d74 147c 0564 0483 0272 9767 007d 0664  ]t.|.d...r.g.}.d
-000037c0: 057d 077c 05a0 15a1 007d 087c 0844 005d  .}.|.....}.|.D.]
-000037d0: 407d 097c 00a0 167c 09a1 017d 0a7c 0a6a  @}.|...|...}.|.j
-000037e0: 0d74 177c 056a 0f6a 187c 096a 196a 1a64  .t.|.j.j.|.j.j.d
-000037f0: 0664 0784 0064 088d 037c 0717 0064 098d  .d...d...|...d..
-00003800: 0101 0074 1b7c 0974 1c83 0272 8474 1b7c  ...t.|.t...r.t.|
-00003810: 0974 1d83 0273 847c 0a6a 0d7c 0a64 0a19  .t...s.|.j.|.d..
-00003820: 0064 0b17 0064 0c8d 0101 007c 0764 0b37  .d...d.....|.d.7
-00003830: 007d 0774 1b7c 0974 1e83 0272 8d7c 0764  .}.t.|.t...r.|.d
-00003840: 0d37 007d 077c 06a0 1f7c 0aa1 0101 0071  .7.}.|...|.....q
-00003850: 527c 067c 0464 0e3c 007c 04a0 0d74 207c  R|.|.d.<.|...t |
-00003860: 056a 0f64 0f83 02a1 0101 007c 04a0 0d74  .j.d.......|...t
-00003870: 207c 0164 1083 02a1 0101 0074 147c 016a   |.d.......t.|.j
-00003880: 2164 1183 0272 b47c 046a 0d64 1264 138d  !d...r.|.j.d.d..
-00003890: 0101 007c 016a 2264 0075 0172 c17c 00a0  ...|.j"d.u.r.|..
-000038a0: 237c 016a 22a1 017c 0464 143c 007c 016a  #|.j"..|.d.<.|.j
-000038b0: 2464 0075 0172 d67c 016a 24a0 25a1 007d  $d.u.r.|.j$.%..}
-000038c0: 0b7c 0b64 0075 0172 d67c 046a 0d7c 0b6a  .|.d.u.r.|.j.|.j
-000038d0: 2664 158d 0101 007c 016a 2772 e27c 046a  &d.....|.j'r.|.j
-000038e0: 0d74 287c 016a 2783 0164 168d 0101 0074  .t(|.j'..d.....t
-000038f0: 297c 0164 1764 0083 037d 0c7c 0c64 0075  )|.d.d...}.|.d.u
-00003900: 0172 f37c 046a 0d7c 0c6a 2664 188d 0101  .r.|.j.|.j&d....
-00003910: 0074 297c 0164 1964 0083 037d 0d7c 0d64  .t)|.d.d...}.|.d
-00003920: 0075 0190 0172 057c 046a 0d7c 0d6a 2664  .u...r.|.j.|.j&d
-00003930: 1a8d 0101 0074 297c 016a 2164 1b69 0083  .....t)|.j!d.i..
-00003940: 037d 0e7c 0e90 0172 1c7c 046a 0d64 1c64  .}.|...r.|.j.d.d
-00003950: 1d84 007c 0ea0 2aa1 0044 0083 0164 1e8d  ...|..*..D...d..
-00003960: 0101 0074 106a 11a0 2b64 1fa1 0190 0172  ...t.j..+d.....r
-00003970: 3f74 297c 0164 2064 0083 0364 0075 0190  ?t)|.d d...d.u..
-00003980: 0172 3f74 147c 016a 2164 2183 0290 0172  .r?t.|.j!d!....r
-00003990: 3f7c 046a 0d74 2c6a 2da0 2e7c 016a 21a1  ?|.j.t,j-..|.j!.
-000039a0: 016a 2f64 228d 0101 0064 2344 005d 177d  .j/d"....d#D.].}
-000039b0: 0f74 297c 017c 0f64 0083 037d 107c 1064  .t)|.|.d...}.|.d
-000039c0: 0075 0190 0172 577c 04a0 0d7c 0f7c 106a  .u...rW|...|.|.j
-000039d0: 306a 3169 01a1 0101 0090 0171 417c 016a  0j1i.......qA|.j
-000039e0: 3264 0075 0190 0172 7d7c 046a 0d7c 016a  2d.u...r}|.j.|.j
-000039f0: 326a 2664 2464 2584 007c 016a 326a 336a  2j&d$d%..|.j2j3j
-00003a00: 3444 0083 0164 268d 0201 0074 147c 0164  4D...d&....t.|.d
-00003a10: 2783 0290 0172 7d7c 046a 0d7c 016a 3564  '....r}|.j.|.j5d
-00003a20: 288d 0101 007c 0453 0029 294e 2905 da02  (....|.S.))N)...
-00003a30: 6964 722f 0100 0072 9500 0000 da05 736c  idr/...r......sl
-00003a40: 6176 65da 0865 6469 7461 626c 6529 0172  ave..editable).r
-00003a50: 3001 0000 7a0f 2573 2068 6173 206e 6f20  0...z.%s has no 
-00003a60: 7374 6f72 65da 0b67 6574 5f63 6f6c 756d  store..get_colum
-00003a70: 6e73 7201 0000 0063 0100 0000 0000 0000  nsr....c........
-00003a80: 0000 0000 0100 0000 0100 0000 5300 0000  ............S...
-00003a90: 7306 0000 007c 006a 0053 0072 3a00 0000  s....|.j.S.r:...
-00003aa0: a901 7252 0000 00a9 0172 8c00 0000 7236  ..rR.....r....r6
-00003ab0: 0000 0072 3600 0000 7237 0000 0072 3701  ...r6...r7...r7.
-00003ac0: 0000 6d02 0000 7302 0000 0006 007a 2552  ..m...s......z%R
-00003ad0: 656e 6465 7265 722e 6163 746f 7232 6a73  enderer.actor2js
-00003ae0: 6f6e 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  on.<locals>.<lam
-00003af0: 6264 613e 7238 0100 0029 01da 0c66 6965  bda>r8...)...fie
-00003b00: 6c64 735f 696e 6465 7872 4401 0000 722c  lds_indexrD...r,
-00003b10: 0000 0029 01da 1366 6965 6c64 735f 696e  ...)...fields_in
-00003b20: 6465 785f 6869 6464 656e e902 0000 00da  dex_hidden......
-00003b30: 0363 6f6c da08 706b 5f69 6e64 6578 7ad0  .col..pk_indexz.
-00003b40: 7072 6576 6965 775f 6c69 6d69 7420 7573  preview_limit us
-00003b50: 655f 6465 7461 696c 5f70 6172 616d 5f70  e_detail_param_p
-00003b60: 616e 656c 2075 7365 5f64 6574 6169 6c5f  anel use_detail_
-00003b70: 7061 7261 6d73 5f76 616c 7565 2068 6964  params_value hid
-00003b80: 655f 6e61 7669 6761 746f 7220 7573 655f  e_navigator use_
-00003b90: 6465 7461 696c 5f70 6172 616d 735f 7661  detail_params_va
-00003ba0: 6c75 6520 7265 6163 745f 7265 7370 6f6e  lue react_respon
-00003bb0: 7369 7665 206d 6178 5f72 656e 6465 725f  sive max_render_
-00003bc0: 6465 7074 6820 7369 6d70 6c65 5f73 6c61  depth simple_sla
-00003bd0: 7665 6772 6964 5f68 6561 6465 7220 7061  vegrid_header pa
-00003be0: 6769 6e61 746f 725f 7465 6d70 6c61 7465  ginator_template
-00003bf0: 2068 6964 655f 746f 705f 746f 6f6c 6261   hide_top_toolba
-00003c00: 7220 6869 6465 5f69 665f 656d 7074 7920  r hide_if_empty 
-00003c10: da04 6669 6c65 5429 01da 0d63 6f6e 7461  ..fileT)...conta
-00003c20: 696e 5f6d 6564 6961 723a 0100 0072 2301  in_mediar:...r#.
-00003c30: 0000 2901 da0d 6163 7469 7665 5f66 6965  ..)...active_fie
-00003c40: 6c64 73da 0b63 6172 645f 6c61 796f 7574  lds..card_layout
-00003c50: 2901 724c 0100 00da 0b6c 6973 745f 6c61  ).rL.....list_la
-00003c60: 796f 7574 2901 724d 0100 00da 0e5f 6368  yout).rM....._ch
-00003c70: 6f6f 7365 7273 5f64 6963 7463 0100 0000  oosers_dictc....
-00003c80: 0000 0000 0000 0000 0300 0000 0500 0000  ................
-00003c90: 5300 0000 7322 0000 0069 007c 005d 0d5c  S...s"...i.|.].\
-00003ca0: 027d 017d 027c 0164 0064 0184 007c 026a  .}.}.|.d.d...|.j
-00003cb0: 0044 0083 0193 0271 0253 0029 0263 0100  .D.....q.S.).c..
-00003cc0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00003cd0: 0000 5300 0000 f312 0000 0067 007c 005d  ..S........g.|.]
-00003ce0: 057d 017c 016a 0091 0271 0253 0072 3600  .}.|.j...q.S.r6.
-00003cf0: 0000 7242 0100 0029 0272 4600 0000 da02  ..rB...).rF.....
-00003d00: 6366 7236 0000 0072 3600 0000 7237 0000  cfr6...r6...r7..
-00003d10: 0072 4800 0000 a302 0000 f302 0000 0012  .rH.............
-00003d20: 007a 3252 656e 6465 7265 722e 6163 746f  .z2Renderer.acto
-00003d30: 7232 6a73 6f6e 2e3c 6c6f 6361 6c73 3e2e  r2json.<locals>.
-00003d40: 3c64 6963 7463 6f6d 703e 2e3c 6c69 7374  <dictcomp>.<list
-00003d50: 636f 6d70 3e29 01da 0e63 6f6e 7465 7874  comp>)...context
-00003d60: 5f66 6965 6c64 7329 0372 4600 0000 da02  _fields).rF.....
-00003d70: 666e 7247 0000 0072 3600 0000 7236 0000  fnrG...r6...r6..
-00003d80: 0072 3700 0000 724c 0000 00a3 0200 0073  .r7...rL.......s
-00003d90: 0600 0000 0600 0601 16ff 7a27 5265 6e64  ..........z'Rend
-00003da0: 6572 6572 2e61 6374 6f72 326a 736f 6e2e  erer.actor2json.
-00003db0: 3c6c 6f63 616c 733e 2e3c 6469 6374 636f  <locals>.<dictco
-00003dc0: 6d70 3e29 01da 0c63 686f 6f73 6572 5f64  mp>)...chooser_d
-00003dd0: 6963 74da 0c63 6f6e 7465 6e74 7479 7065  ict..contenttype
-00003de0: 73da 056d 6f64 656c da05 5f6d 6574 6129  s..model.._meta)
-00003df0: 01da 0c63 6f6e 7465 6e74 5f74 7970 6529  ...content_type)
-00003e00: 03da 0d64 6574 6169 6c5f 6163 7469 6f6e  ...detail_action
-00003e10: da0d 696e 7365 7274 5f61 6374 696f 6eda  ..insert_action.
-00003e20: 0e64 6566 6175 6c74 5f61 6374 696f 6e63  .default_actionc
-00003e30: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00003e40: 0300 0000 5300 0000 724f 0100 0072 3600  ....S...rO...r6.
-00003e50: 0000 7242 0100 0029 0272 4600 0000 728c  ..rB...).rF...r.
-00003e60: 0000 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
-00003e70: 0000 7248 0000 00b3 0200 0072 5101 0000  ..rH.......rQ...
-00003e80: 7a27 5265 6e64 6572 6572 2e61 6374 6f72  z'Renderer.actor
-00003e90: 326a 736f 6e2e 3c6c 6f63 616c 733e 2e3c  2json.<locals>.<
-00003ea0: 6c69 7374 636f 6d70 3e29 02da 0d70 6172  listcomp>)...par
-00003eb0: 616d 735f 6c61 796f 7574 da0d 7061 7261  ams_layout..para
-00003ec0: 6d73 5f66 6965 6c64 73da 1070 6172 616d  ms_fields..param
-00003ed0: 735f 7061 6e65 6c5f 706f 7329 0172 5e01  s_panel_pos).r^.
-00003ee0: 0000 2936 722b 0000 0072 b400 0000 721b  ..)6r+...r....r.
-00003ef0: 0000 0072 3601 0000 da0d 5f61 6374 696f  ...r6....._actio
-00003f00: 6e73 5f6c 6973 7472 7100 0000 72ef 0000  ns_listrq...r...
-00003f10: 00da 0f67 6574 5f61 6374 6f72 5f6c 6162  ...get_actor_lab
-00003f20: 656c da04 626f 6f6c da06 6d61 7374 6572  el..bool..master
-00003f30: da0c 6869 6465 5f65 6469 7469 6e67 7229  ..hide_editingr)
-00003f40: 0000 0072 d100 0000 7277 0000 00da 0a67  ...r....rw.....g
-00003f50: 6574 5f68 616e 646c 65da 0573 746f 7265  et_handle..store
-00003f60: 7204 0000 0072 6f00 0000 da06 6c6f 6767  r....ro.....logg
-00003f70: 6572 da07 7761 726e 696e 6772 8200 0000  er..warningr....
-00003f80: 7241 0100 0072 aa00 0000 7238 0000 00da  rA...r....r8....
-00003f90: 0b6c 6973 745f 6669 656c 6473 72b6 0000  .list_fieldsr...
-00003fa0: 0072 5200 0000 72a0 0000 0072 1f00 0000  .rR...r....r....
-00003fb0: 7220 0000 0072 2200 0000 722c 0100 0072  r ...r"...r,...r
-00003fc0: 2800 0000 7256 0100 0072 3a01 0000 723d  (...rV...r:...r=
-00003fd0: 0100 0072 5901 0000 da11 6765 745f 7769  ...rY.....get_wi
-00003fe0: 6e64 6f77 5f6c 6179 6f75 7472 8700 0000  ndow_layoutr....
-00003ff0: 724b 0100 0072 7800 0000 7201 0100 0072  rK...rx...r....r
-00004000: 6800 0000 7276 0000 0072 0e00 0000 da07  h...rv...r......
-00004010: 6f62 6a65 6374 73da 0d67 6574 5f66 6f72  objects..get_for
-00004020: 5f6d 6f64 656c 72d8 0000 0072 6c00 0000  _modelr....rl...
-00004030: 724d 0000 0072 5c01 0000 da0c 7061 7261  rM...r\.....para
-00004040: 6d73 5f73 746f 7265 da0c 7061 7261 6d5f  ms_store..param_
-00004050: 6669 656c 6473 725e 0100 0029 1172 3f00  fieldsr^...).r?.
-00004060: 0000 72a5 0000 00da 0261 6cda 0268 6b72  ..r......al..hkr
-00004070: a600 0000 da02 6168 da07 636f 6c75 6d6e  ......ah..column
-00004080: 73da 0969 6e64 6578 5f6d 6f64 da09 636f  s..index_mod..co
-00004090: 6c5f 656c 656d 7372 4701 0000 720b 0100  l_elemsrG...r...
-000040a0: 00da 0277 6c72 4c01 0000 724d 0100 0072  ...wlrL...rM...r
-000040b0: 5401 0000 72b7 0000 0072 8f00 0000 7236  T...r....r....r6
-000040c0: 0000 0072 3600 0000 7237 0000 00da 0a61  ...r6...r7.....a
-000040d0: 6374 6f72 326a 736f 6e54 0200 0073 8e00  ctor2jsonT...s..
-000040e0: 0000 1601 1001 0601 0201 0601 0801 0c01  ................
-000040f0: 06fc 0807 0c01 0802 0a01 1201 0a03 0401  ................
-00004100: 0401 0801 0801 0a01 1201 0601 04ff 0201  ................
-00004110: 08ff 1402 1403 0801 0a01 0801 0c01 0801  ................
-00004120: 1205 1001 0c0d 0c01 0a02 1001 0a02 0a01  ................
-00004130: 0801 0e01 0602 1201 0c02 0801 0e01 0c02  ................
-00004140: 0a01 0e02 0e03 0601 0a01 0601 0aff 2603  ..............&.
-00004150: 0201 06ff 1803 0801 0c01 0a01 1201 0480  ................
-00004160: 0c02 0402 0601 1201 06fe 0c04 0e01 0401  ................
-00004170: 7a13 5265 6e64 6572 6572 2e61 6374 6f72  z.Renderer.actor
-00004180: 326a 736f 6e63 0200 0000 0000 0000 0000  2jsonc..........
-00004190: 0000 0400 0000 0600 0000 0300 0000 7364  ..............sd
-000041a0: 0000 0064 0188 015f 0088 016a 0144 005d  ...d..._...j.D.]
-000041b0: 2289 0088 006a 0264 0075 0172 0e71 0674  "....j.d.u.r.q.t
-000041c0: 036a 046a 0588 01a0 0688 006a 07a1 018e  .j.j.......j....
-000041d0: 007d 0287 0087 0166 0264 0264 0384 087d  .}.....f.d.d...}
-000041e0: 0374 086a 096a 0aa0 0b7c 027c 037c 01a1  .t.j.j...|.|.|..
-000041f0: 0301 0071 0664 0488 015f 0074 0c83 00a0  ...q.d..._.t....
-00004200: 0d7c 01a1 0153 0029 054e 5463 0100 0000  .|...S.).NTc....
-00004210: 0000 0000 0000 0000 0100 0000 0600 0000  ................
-00004220: 1300 0000 7318 0000 007c 00a0 0074 0188  ....s....|...t..
-00004230: 01a0 0288 00a1 0183 01a1 0101 0064 0053  .............d.S
-00004240: 0072 3a00 0000 2903 728b 0000 0072 2600  .r:...).r....r&.
-00004250: 0000 7275 0100 0072 4301 0000 a902 7298  ..ru...rC.....r.
-00004260: 0000 0072 3f00 0000 7236 0000 0072 3700  ...r?...r6...r7.
-00004270: 0000 728b 0000 00c2 0200 0073 0200 0000  ..r........s....
-00004280: 1801 7a26 5265 6e64 6572 6572 2e62 7569  ..z&Renderer.bui
-00004290: 6c64 5f6a 735f 6361 6368 652e 3c6c 6f63  ld_js_cache.<loc
-000042a0: 616c 733e 2e77 7269 7465 4629 0e72 6e00  als>.writeF).rn.
-000042b0: 0000 726a 0000 00da 0f67 6574 5f68 616e  ..rj.....get_han
-000042c0: 646c 655f 6e61 6d65 727d 0000 00da 0470  dle_namer}.....p
-000042d0: 6174 68da 046a 6f69 6e72 2201 0000 72ef  ath..joinr"...r.
-000042e0: 0000 0072 0400 0000 726f 0000 0072 2300  ...r....ro...r#.
-000042f0: 0000 da0f 6d61 6b65 5f63 6163 6865 5f66  ....make_cache_f
-00004300: 696c 6572 3b00 0000 da0e 6275 696c 645f  iler;.....build_
-00004310: 6a73 5f63 6163 6865 2904 723f 0000 00da  js_cache).r?....
-00004320: 0566 6f72 6365 7253 0100 0072 8b00 0000  .forcerS...r....
-00004330: 7241 0000 0072 7601 0000 7237 0000 0072  rA...rv...r7...r
-00004340: 7b01 0000 b902 0000 7312 0000 0006 020a  {.......s.......
-00004350: 020a 0102 0114 010e 0214 0306 020c 017a  ...............z
-00004360: 1752 656e 6465 7265 722e 6275 696c 645f  .Renderer.build_
-00004370: 6a73 5f63 6163 6865 723a 0000 0029 2072  js_cacher:...) r
-00004380: b300 0000 da0a 5f5f 6d6f 6475 6c65 5f5f  ......__module__
-00004390: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
-000043a0: 5f5f 646f 635f 5fda 0e69 735f 696e 7465  __doc__..is_inte
-000043b0: 7261 6374 6976 65da 0863 616e 5f61 7574  ractive..can_aut
-000043c0: 6872 1d01 0000 7221 0100 00da 1873 7570  hr....r!.....sup
-000043d0: 706f 7274 5f64 6173 6862 6f61 7264 5f6c  port_dashboard_l
-000043e0: 6179 6f75 7472 3c00 0000 7293 0000 0072  ayoutr<...r....r
-000043f0: 4e00 0000 7286 0000 0072 aa00 0000 72b8  N...r....r....r.
-00004400: 0000 0072 ce00 0000 72db 0000 0072 e200  ...r....r....r..
-00004410: 0000 72a4 0000 0072 de00 0000 723e 0000  ..r....r....r>..
-00004420: 0072 fd00 0000 72fe 0000 0072 ff00 0000  .r....r....r....
-00004430: 7213 0100 0072 1901 0000 7222 0100 0072  r....r....r"...r
-00004440: 3601 0000 723d 0100 0072 7501 0000 727b  6...r=...ru...r{
-00004450: 0100 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
-00004460: 5f5f 7236 0000 0072 3600 0000 7241 0000  __r6...r6...rA..
-00004470: 0072 3700 0000 7239 0000 003a 0000 0073  .r7...r9...:...s
-00004480: 3c00 0000 0800 0401 0403 0401 0402 0401  <...............
-00004490: 0401 0c02 0804 0855 081d 0808 081f 0803  .......U........
-000044a0: 0a18 0212 0aff 0815 080e 0821 084e 080e  ...........!.N..
-000044b0: 080a 082a 0809 080f 080a 0844 080c 1465  ...*.......D...e
-000044c0: 7239 0000 0072 3a00 0000 2946 727d 0000  r9...r:...)Fr}..
-000044d0: 00da 0770 6174 686c 6962 7202 0000 00da  ...pathlibr.....
-000044e0: 0468 746d 6c72 0300 0000 da0b 646a 616e  .htmlr......djan
-000044f0: 676f 2e63 6f6e 6672 0400 0000 da09 646a  go.confr......dj
-00004500: 616e 676f 2e64 6272 0500 0000 da11 646a  ango.dbr......dj
-00004510: 616e 676f 2e75 7469 6c73 2e74 6578 7472  ango.utils.textr
-00004520: 0600 0000 da0c 646a 616e 676f 2e75 7469  ......django.uti
-00004530: 6c73 7207 0000 00da 126c 696e 6f2e 636f  lsr......lino.co
-00004540: 7265 2e72 656e 6465 7265 7272 0800 0000  re.rendererr....
-00004550: 7209 0000 00da 0f6c 696e 6f2e 636f 7265  r......lino.core
-00004560: 2e6d 656e 7573 720a 0000 0072 0b00 0000  .menusr....r....
-00004570: da09 6c69 6e6f 2e63 6f72 6572 0c00 0000  ..lino.corer....
-00004580: 720d 0000 00da 0e6c 696e 6f2e 636f 7265  r......lino.core
-00004590: 2e67 666b 7372 0e00 0000 da1e 6c69 6e6f  .gfksr......lino
-000045a0: 2e6d 6f64 6c69 622e 6578 746a 732e 6578  .modlib.extjs.ex
-000045b0: 745f 7265 6e64 6572 6572 720f 0000 00da  t_rendererr.....
-000045c0: 116c 696e 6f2e 636f 7265 2e61 6374 696f  .lino.core.actio
-000045d0: 6e73 7210 0000 0072 1100 0000 7212 0000  nsr....r....r...
-000045e0: 0072 1300 0000 7214 0000 0072 1500 0000  .r....r....r....
-000045f0: 7216 0000 0072 1700 0000 da15 6c69 6e6f  r....r......lino
-00004600: 2e63 6f72 652e 626f 756e 6461 6374 696f  .core.boundactio
-00004610: 6e72 1800 0000 da15 6c69 6e6f 2e63 6f72  nr......lino.cor
-00004620: 652e 6368 6f69 6365 6c69 7374 7372 1900  e.choicelistsr..
-00004630: 0000 da1e 6c69 6e6f 2e6d 6f64 6c69 622e  ....lino.modlib.
-00004640: 7379 7374 656d 2e63 686f 6963 656c 6973  system.choicelis
-00004650: 7473 721a 0000 00da 106c 696e 6f2e 636f  tsr......lino.co
-00004660: 7265 2e61 6374 6f72 7372 1b00 0000 da11  re.actorsr......
-00004670: 6c69 6e6f 2e63 6f72 652e 6c61 796f 7574  lino.core.layout
-00004680: 7372 1c00 0000 721d 0000 00da 0f6c 696e  sr....r......lin
-00004690: 6f2e 636f 7265 2e65 6c65 6d73 721e 0000  o.core.elemsr...
-000046a0: 0072 1f00 0000 7220 0000 0072 2100 0000  .r....r ...r!...
-000046b0: 7222 0000 0072 2300 0000 da0a 6574 6765  r"...r#.....etge
-000046c0: 6e2e 6874 6d6c 7224 0000 00da 0a6c 696e  n.htmlr$.....lin
-000046d0: 6f2e 7574 696c 7372 2500 0000 da10 6c69  o.utilsr%.....li
-000046e0: 6e6f 2e75 7469 6c73 2e6a 7367 656e 7226  no.utils.jsgenr&
-000046f0: 0000 0072 2700 0000 7228 0000 00da 176c  ...r'...r(.....l
-00004700: 696e 6f2e 6d6f 646c 6962 2e75 7365 7273  ino.modlib.users
-00004710: 2e75 7469 6c73 7229 0000 0072 2a00 0000  .utilsr)...r*...
-00004720: da07 696e 7370 6563 7472 2b00 0000 da05  ..inspectr+.....
-00004730: 6963 6f6e 7372 2d00 0000 7238 0000 0072  iconsr-...r8...r
-00004740: 3900 0000 7236 0000 0072 3600 0000 7236  9...r6...r6...r6
-00004750: 0000 0072 3700 0000 da08 3c6d 6f64 756c  ...r7.....<modul
-00004760: 653e 0100 0000 733a 0000 0008 040c 010c  e>....s:........
-00004770: 010c 010c 010c 010c 0110 0210 020c 010c  ................
-00004780: 010c 010c 0128 020c 030c 010c 010c 0110  .....(..........
-00004790: 011c 010c 020c 020c 0214 0110 020c 020c  ................
-000047a0: 020a 0314 0d                             .....
+000001a0: 6d41 5a41 0100 6400 641b 6c42 6d43 5a43  mAZA..d.d.lBmCZC
+000001b0: 0100 641c 641d 6c44 6d45 5a45 0100 6422  ..d.d.lDmEZE..d"
+000001c0: 641e 641f 8401 5a46 4700 6420 6421 8400  d.d...ZFG.d d!..
+000001d0: 6421 650f 8303 5a47 6401 5300 2923 e900  d!e...ZGd.S.)#..
+000001e0: 0000 004e 2901 da04 5061 7468 2901 da06  ...N)...Path)...
+000001f0: 6573 6361 7065 2901 da08 7365 7474 696e  escape)...settin
+00000200: 6773 2901 da06 6d6f 6465 6c73 2901 da0b  gs)...models)...
+00000210: 666f 726d 6174 5f6c 617a 7929 01da 0b74  format_lazy)...t
+00000220: 7261 6e73 6c61 7469 6f6e 2902 da11 6164  ranslation)...ad
+00000230: 645f 7573 6572 5f6c 616e 6775 6167 65da  d_user_language.
+00000240: 0f4a 7343 6163 6865 5265 6e64 6572 6572  .JsCacheRenderer
+00000250: 2902 da04 4d65 6e75 da08 4d65 6e75 4974  )...Menu..MenuIt
+00000260: 656d 2901 da09 636f 6e73 7461 6e74 7329  em)...constants)
+00000270: 01da 0b63 686f 6963 656c 6973 7473 2901  ...choicelists).
+00000280: da0b 436f 6e74 656e 7454 7970 6529 01da  ..ContentType)..
+00000290: 0b45 7874 5265 6e64 6572 6572 2908 da0e  .ExtRenderer)...
+000002a0: 5368 6f77 456d 7074 7954 6162 6c65 da0a  ShowEmptyTable..
+000002b0: 5368 6f77 4465 7461 696c da0d 5772 6170  ShowDetail..Wrap
+000002c0: 7065 6441 6374 696f 6eda 0a53 686f 7749  pedAction..ShowI
+000002d0: 6e73 6572 74da 0953 686f 7754 6162 6c65  nsert..ShowTable
+000002e0: da0c 5375 626d 6974 4465 7461 696c da0c  ..SubmitDetail..
+000002f0: 5375 626d 6974 496e 7365 7274 da06 4163  SubmitInsert..Ac
+00000300: 7469 6f6e 2901 da0b 426f 756e 6441 6374  tion)...BoundAct
+00000310: 696f 6e29 01da 0e43 686f 6963 654c 6973  ion)...ChoiceLis
+00000320: 744d 6574 6129 01da 1044 6173 6862 6f61  tMeta)...Dashboa
+00000330: 7264 4c61 796f 7574 7329 01da 0541 6374  rdLayouts)...Act
+00000340: 6f72 2902 da0c 4c61 796f 7574 4861 6e64  or)...LayoutHand
+00000350: 6c65 da0a 4261 7365 4c61 796f 7574 2905  le..BaseLayout).
+00000360: da0d 4c61 796f 7574 456c 656d 656e 74da  ..LayoutElement.
+00000370: 1143 6f6d 626f 4669 656c 6445 6c65 6d65  .ComboFieldEleme
+00000380: 6e74 da1d 5369 6d70 6c65 5265 6d6f 7465  nt..SimpleRemote
+00000390: 436f 6d62 6f46 6965 6c64 456c 656d 656e  ComboFieldElemen
+000003a0: 74da 0c46 6965 6c64 456c 656d 656e 74da  t..FieldElement.
+000003b0: 1750 7265 7669 6577 5465 7874 4669 656c  .PreviewTextFiel
+000003c0: 6445 6c65 6d65 6e74 2901 da06 6b65 726e  dElement)...kern
+000003d0: 656c 2901 da01 4529 01da 056a 7367 656e  el)...E)...jsgen
+000003e0: 2903 da05 7079 326a 73da 076a 735f 636f  )...py2js..js_co
+000003f0: 6465 da08 6f62 6a32 6469 6374 2902 da10  de..obj2dict)...
+00000400: 6765 745f 7573 6572 5f70 726f 6669 6c65  get_user_profile
+00000410: da11 7769 7468 5f75 7365 725f 7072 6f66  ..with_user_prof
+00000420: 696c 6529 01da 0845 6469 7453 6166 6529  ile)...EditSafe)
+00000430: 01da 0769 7363 6c61 7373 e901 0000 0029  ...isclass.....)
+00000440: 01da 1252 4541 4354 5f49 434f 4e5f 4d41  ...REACT_ICON_MA
+00000450: 5050 494e 4763 0300 0000 0000 0000 0000  PPINGc..........
+00000460: 0000 0500 0000 0300 0000 4300 0000 734a  ..........C...sJ
+00000470: 0000 007c 0264 016b 0273 0c74 007c 0283  ...|.d.k.s.t.|..
+00000480: 0173 0c4a 0064 0283 0182 0174 017c 0083  .s.J.d.....t.|..
+00000490: 0144 005d 125c 027d 037d 047c 0272 1a7c  .D.].\.}.}.|.r.|
+000004a0: 027c 0483 017d 047c 047c 016b 0272 227c  .|...}.|.|.k.r"|
+000004b0: 0302 0001 0053 0071 1064 0353 0029 047a  .....S.q.d.S.).z
+000004c0: 4d52 6574 7572 6e73 2074 6865 2069 6e64  MReturns the ind
+000004d0: 6578 206f 6620 616e 2065 6c65 6d65 6e74  ex of an element
+000004e0: 2069 6e20 6120 6361 6c6c 6162 6c65 2077   in a callable w
+000004f0: 6869 6368 2063 616e 2062 6520 7573 6520  hich can be use 
+00000500: 6120 6b65 7920 6675 6e63 7469 6f6e 4e7a  a key functionNz
+00000510: 586b 6579 2073 686f 6c64 2062 6520 6120  Xkey shold be a 
+00000520: 6675 6e63 7469 6f6e 2074 6861 7420 7461  function that ta
+00000530: 6b65 7320 7468 6520 6974 7465 7227 7320  kes the itter's 
+00000540: 6974 656d 2061 6e64 2072 6574 7572 6e73  item and returns
+00000550: 2074 6861 7420 7761 6e74 6564 206d 6174   that wanted mat
+00000560: 6368 6564 2069 7465 6de9 ffff ffff 2902  ched item.....).
+00000570: da08 6361 6c6c 6162 6c65 da09 656e 756d  ..callable..enum
+00000580: 6572 6174 6529 05da 0569 7474 6572 da06  erate)...itter..
+00000590: 7461 7267 6574 da03 6b65 79da 0169 da01  target..key..i..
+000005a0: 78a9 0072 3700 0000 fa45 2f68 6f6d 652f  x..r7....E/home/
+000005b0: 626c 7572 7279 2f6c 696e 6f2f 656e 762f  blurry/lino/env/
+000005c0: 7265 706f 7369 746f 7269 6573 2f72 6561  repositories/rea
+000005d0: 6374 2f6c 696e 6f5f 7265 6163 742f 7265  ct/lino_react/re
+000005e0: 6163 742f 7265 6e64 6572 6572 2e70 79da  act/renderer.py.
+000005f0: 0466 696e 642e 0000 0073 1000 0000 1802  .find....s......
+00000600: 1002 0401 0801 0801 0801 02ff 0403 7239  ..............r9
+00000610: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000620: 0000 0000 0300 0000 0000 0000 73e6 0000  ............s...
+00000630: 0065 005a 0164 005a 0264 015a 0364 025a  .e.Z.d.Z.d.Z.d.Z
+00000640: 0464 025a 0564 035a 0664 045a 0764 025a  .d.Z.d.Z.d.Z.d.Z
+00000650: 0887 0066 0164 0564 0684 085a 0964 0764  ...f.d.d...Z.d.d
+00000660: 0884 005a 0a64 0964 0a84 005a 0b64 0b64  ...Z.d.d...Z.d.d
+00000670: 0c84 005a 0c64 0d64 0e84 005a 0d64 0f64  ...Z.d.d...Z.d.d
+00000680: 1084 005a 0e64 1164 1284 005a 0f64 3264  ...Z.d.d...Z.d2d
+00000690: 1464 1584 015a 1069 0066 0164 1664 1784  .d...Z.i.f.d.d..
+000006a0: 015a 1164 1864 1984 005a 1264 1a64 1b84  .Z.d.d...Z.d.d..
+000006b0: 005a 1364 1c64 1d84 005a 1464 1e64 1f84  .Z.d.d...Z.d.d..
+000006c0: 005a 1564 2064 2184 005a 1664 2264 2384  .Z.d d!..Z.d"d#.
+000006d0: 005a 1764 2464 2584 005a 1864 2664 2784  .Z.d$d%..Z.d&d'.
+000006e0: 005a 1964 2864 2984 005a 1a64 2a64 2b84  .Z.d(d)..Z.d*d+.
+000006f0: 005a 1b64 2c64 2d84 005a 1c64 2e64 2f84  .Z.d,d-..Z.d.d/.
+00000700: 005a 1d87 0066 0164 3064 3184 085a 1e87  .Z...f.d0d1..Z..
+00000710: 0004 005a 1f53 0029 33da 0852 656e 6465  ...Z.S.)3..Rende
+00000720: 7265 727a 480a 2020 2020 4120 6672 6f6e  rerzH.    A fron
+00000730: 742d 656e 6420 7265 6e64 6572 6572 2074  t-end renderer t
+00000740: 6861 7420 7573 6573 2074 6865 2052 6561  hat uses the Rea
+00000750: 6374 204a 6176 6173 6372 6970 7420 6672  ct Javascript fr
+00000760: 616d 6577 6f72 6b2e 0a20 2020 2054 7a12  amework..    Tz.
+00000770: 7265 6163 742f 6c69 6e6f 7765 622e 6a73  react/linoweb.js
+00000780: 6f6e 7a05 2e6a 736f 6e63 0200 0000 0000  onz..jsonc......
+00000790: 0000 0000 0000 0200 0000 0300 0000 0300  ................
+000007a0: 0000 731c 0000 0074 0083 00a0 017c 01a1  ..s....t.....|..
+000007b0: 0101 0074 02a0 037c 006a 04a1 0101 0064  ...t...|.j.....d
+000007c0: 0053 00a9 014e 2905 da05 7375 7065 72da  .S...N)...super.
+000007d0: 085f 5f69 6e69 745f 5f72 2500 0000 da12  .__init__r%.....
+000007e0: 7265 6769 7374 6572 5f63 6f6e 7665 7274  register_convert
+000007f0: 6572 da0f 7079 326a 735f 636f 6e76 6572  er..py2js_conver
+00000800: 7465 7229 02da 0473 656c 66da 0966 726f  ter)...self..fro
+00000810: 6e74 5f65 6e64 a901 da09 5f5f 636c 6173  nt_end....__clas
+00000820: 735f 5f72 3700 0000 7238 0000 0072 3d00  s__r7...r8...r=.
+00000830: 0000 4600 0000 7304 0000 000c 0110 017a  ..F...s........z
+00000840: 1152 656e 6465 7265 722e 5f5f 696e 6974  .Renderer.__init
+00000850: 5f5f 6302 0000 0000 0000 0000 0000 000c  __c.............
+00000860: 0000 0008 0000 0003 0000 0073 7202 0000  ...........sr...
+00000870: 6401 6402 8400 7400 6a01 a002 a100 4400  d.d...t.j.....D.
+00000880: 8301 7d02 7403 8300 7d03 8800 6a04 4400  ..}.t...}...j.D.
+00000890: 5d14 7d04 7c04 a005 a100 4400 5d0d 7d05  ].}.|.....D.].}.
+000008a0: 7c05 6a06 7c03 7601 7223 7c03 a007 7c05  |.j.|.v.r#|...|.
+000008b0: 6a06 a101 0100 7116 7110 6403 8800 5f08  j.....q.q.d..._.
+000008c0: 7409 6a0a 6a0b 7d06 740c 8700 6601 6404  t.j.j.}.t...f.d.
+000008d0: 6402 8408 7c03 4400 8301 7409 6a0a a00d  d...|.D...t.j...
+000008e0: 740e 8300 a101 7c06 6a0f 6a10 7409 6a0a  t.....|.j.j.t.j.
+000008f0: 6a11 8800 6a12 6a13 6405 7501 6406 6402  j...j.j.d.u.d.d.
+00000900: 8400 7409 6a0a 6a14 4400 8301 6407 8d06  ..t.j.j.D...d...
+00000910: 7d07 7409 6a0a a015 6408 a101 7264 7c07  }.t.j...d...rd|.
+00000920: 6a16 7417 7c06 6a18 6a19 6a1a a01b a100  j.t.|.j.j.j.....
+00000930: 8301 6409 8d01 0100 7c07 6a16 7409 6a0a  ..d.....|.j.t.j.
+00000940: 6a00 6a1c 640a 8d01 0100 7a13 7c07 6a16  j.j.d.....z.|.j.
+00000950: 741d a01e 741f 7409 6a20 8301 640b 1b00  t...t.t.j ..d...
+00000960: 640c 1b00 a101 6a21 640d 8d01 0100 5700  d.....j!d.....W.
+00000970: 6e09 0400 7422 7989 0100 0100 0100 5900  n...t"y.......Y.
+00000980: 6e01 7700 7423 7409 6a0a 640e 8302 7298  n.w.t#t.j.d...r.
+00000990: 7c07 6a16 7409 6a0a 6a24 640f 8d01 0100  |.j.t.j.j$d.....
+000009a0: 7409 6a0a 6a25 6405 6b02 72a5 7c07 6a16  t.j.j%d.k.r.|.j.
+000009b0: 6403 6410 8d01 0100 6e0e 7423 7c06 6a26  d.d.....n.t#|.j&
+000009c0: 6411 8302 72b3 7c07 6a16 7c06 6a26 6a27  d...r.|.j.|.j&j'
+000009d0: 6412 8d01 0100 7409 6a0a a015 6413 a101  d.....t.j...d...
+000009e0: 72c5 7c07 6a16 7c06 6a28 6a29 6fc2 7409  r.|.j.|.j(j)o.t.
+000009f0: 6a0a 6a2a 6414 8d01 0100 6900 7d08 8800  j.j*d.....i.}...
+00000a00: 6a2b 4400 5d2f 7d09 8800 a02c 7c09 a101  j+D.]/}....,|...
+00000a10: 7c08 7c09 6a2d 3c00 7423 7c09 6415 8302  |.|.j-<.t#|.d...
+00000a20: 72f9 6416 7c09 6a2d 7600 72f9 742e 7c02  r.d.|.j-v.r.t.|.
+00000a30: 6417 1900 8301 4400 5d14 5c02 7d0a 7d0b  d.....D.].\.}.}.
+00000a40: 7c0b 6418 1900 7c09 6a2f 6b02 72f8 7c09  |.d...|.j/k.r.|.
+00000a50: 6a2d 7c02 6417 1900 7c0a 1900 6419 3c00  j-|.d...|...d.<.
+00000a60: 71e4 71ca 8800 6a30 4400 5d0a 7d09 8800  q.q...j0D.].}...
+00000a70: a02c 7c09 a101 7c08 7c09 6a2d 3c00 71fd  .,|...|.|.j-<.q.
+00000a80: 8800 6a31 4400 5d0b 7d09 8800 a02c 7c09  ..j1D.].}....,|.
+00000a90: a101 7c08 7c09 6a2d 3c00 9001 710b 8800  ..|.|.j-<...q...
+00000aa0: 6a32 4400 5d0b 7d09 8800 a02c 7c09 a101  j2D.].}....,|...
+00000ab0: 7c08 7c09 6a2d 3c00 9001 711a 7c07 6a16  |.|.j-<...q.|.j.
+00000ac0: 7c08 7c02 641a 8d02 0100 7c01 a033 7434  |.|.d.....|..3t4
+00000ad0: 7c07 8301 a101 0100 641b 8800 5f08 641c  |.......d..._.d.
+00000ae0: 5300 291d 7a86 0a20 2020 2020 2020 2043  S.).z..        C
+00000af0: 7265 6174 6573 2077 6861 7420 6973 206b  reates what is k
+00000b00: 6e6f 776e 2061 7320 7769 6e64 6f77 2e41  nown as window.A
+00000b10: 7070 2e73 7461 7465 2e73 6974 655f 6461  pp.state.site_da
+00000b20: 7461 2069 6e20 5265 6163 7420 636f 6465  ta in React code
+00000b30: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
+00000b40: 6d20 663a 2046 696c 6520 6f62 6a65 6374  m f: File object
+00000b50: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00000b60: 3a20 310a 2020 2020 2020 2020 6301 0000  : 1.        c...
+00000b70: 0000 0000 0000 0000 0003 0000 0006 0000  ................
+00000b80: 0053 0000 0073 2400 0000 6900 7c00 5d0e  .S...s$...i.|.].
+00000b90: 5c02 7d01 7d02 7c01 6400 6401 8400 7c02  \.}.}.|.d.d...|.
+00000ba0: a000 a100 4400 8301 9302 7102 5300 2902  ....D.....q.S.).
+00000bb0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000bc0: 0006 0000 0053 0000 0073 2400 0000 6700  .....S...s$...g.
+00000bd0: 7c00 5d0e 7d01 7c01 6400 1900 6a00 7401  |.].}.|.d...j.t.
+00000be0: 7c01 6401 1900 8301 6402 9c02 9102 7102  |.d.....d.....q.
+00000bf0: 5300 2903 7201 0000 0072 2d00 0000 2902  S.).r....r-...).
+00000c00: da05 7661 6c75 65da 0474 6578 7429 0272  ..value..text).r
+00000c10: 4400 0000 da03 7374 7229 02da 022e 30da  D.....str)....0.
+00000c20: 0163 7237 0000 0072 3700 0000 7238 0000  .cr7...r7...r8..
+00000c30: 00da 0a3c 6c69 7374 636f 6d70 3e53 0000  ...<listcomp>S..
+00000c40: 0073 0200 0000 2400 7a35 5265 6e64 6572  .s....$.z5Render
+00000c50: 6572 2e77 7269 7465 5f6c 696e 6f5f 6a73  er.write_lino_js
+00000c60: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
+00000c70: 6f6d 703e 2e3c 6c69 7374 636f 6d70 3e29  omp>.<listcomp>)
+00000c80: 01da 0b67 6574 5f63 686f 6963 6573 2903  ...get_choices).
+00000c90: 7247 0000 00da 0249 44da 0263 6c72 3700  rG.....ID..clr7.
+00000ca0: 0000 7237 0000 0072 3800 0000 da0a 3c64  ..r7...r8.....<d
+00000cb0: 6963 7463 6f6d 703e 5100 0000 7308 0000  ictcomp>Q...s...
+00000cc0: 0006 0006 0312 ff06 fe7a 2a52 656e 6465  .........z*Rende
+00000cd0: 7265 722e 7772 6974 655f 6c69 6e6f 5f6a  rer.write_lino_j
+00000ce0: 732e 3c6c 6f63 616c 733e 2e3c 6469 6374  s.<locals>.<dict
+00000cf0: 636f 6d70 3e54 6301 0000 0000 0000 0000  comp>Tc.........
+00000d00: 0000 0002 0000 0006 0000 0013 0000 0073  ...............s
+00000d10: 1a00 0000 6900 7c00 5d09 7d01 7c01 6a00  ....i.|.].}.|.j.
+00000d20: 8800 a001 7c01 a101 9302 7102 5300 7237  ....|.....q.S.r7
+00000d30: 0000 0029 02da 0b61 6374 696f 6e5f 6e61  ...)...action_na
+00000d40: 6d65 da0b 6163 7469 6f6e 326a 736f 6e29  me..action2json)
+00000d50: 0272 4700 0000 da01 61a9 0172 4000 0000  .rG.....a..r@...
+00000d60: 7237 0000 0072 3800 0000 724d 0000 0060  r7...r8...rM...`
+00000d70: 0000 0073 0200 0000 1a00 4e63 0100 0000  ...s......Nc....
+00000d80: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00000d90: 5300 0000 7316 0000 0069 007c 005d 077d  S...s....i.|.].}
+00000da0: 017c 016a 007c 016a 0193 0271 0253 0072  .|.j.|.j...q.S.r
+00000db0: 3700 0000 2902 da0b 646a 616e 676f 5f63  7...)...django_c
+00000dc0: 6f64 65da 046e 616d 6529 0272 4700 0000  ode..name).rG...
+00000dd0: da04 6c61 6e67 7237 0000 0072 3700 0000  ..langr7...r7...
+00000de0: 7238 0000 0072 4d00 0000 6600 0000 7302  r8...rM...f...s.
+00000df0: 0000 0016 0029 06da 0761 6374 696f 6e73  .....)...actions
+00000e00: da04 6d65 6e75 da15 7573 655f 6461 7368  ..menu..use_dash
+00000e10: 626f 6172 645f 6c61 796f 7574 73da 0a73  board_layouts..s
+00000e20: 6974 655f 7469 746c 65da 1065 6469 7469  ite_title..editi
+00000e30: 6e67 5f66 726f 6e74 656e 64da 096c 616e  ng_frontend..lan
+00000e40: 6775 6167 6573 da04 6d65 6d6f 2901 da0a  guages..memo)...
+00000e50: 7375 6767 6573 746f 7273 2901 da0f 7265  suggestors)...re
+00000e60: 7669 7369 6f6e 5f6e 756d 6265 72da 0572  vision_number..r
+00000e70: 6561 6374 7a07 6d61 696e 2e6a 7329 01da  eactz.main.js)..
+00000e80: 0d6d 6a73 5f74 696d 6573 7461 6d70 da0a  .mjs_timestamp..
+00000e90: 7468 656d 655f 6e61 6d65 2901 7260 0000  theme_name).r`..
+00000ea0: 0029 01da 0d6e 6f5f 7573 6572 5f6d 6f64  .)...no_user_mod
+00000eb0: 656c da19 616c 6c6f 775f 6f6e 6c69 6e65  el..allow_online
+00000ec0: 5f72 6567 6973 7472 6174 696f 6e29 0172  _registration).r
+00000ed0: 6200 0000 da06 6e6f 7469 6679 2901 da0c  b.....notify)...
+00000ee0: 7573 655f 7075 7368 5f61 7069 da0b 6368  use_push_api..ch
+00000ef0: 6f69 6365 5f6e 616d 657a 1073 7973 7465  oice_namez.syste
+00000f00: 6d2e 4461 7368 626f 6172 647a 1773 7973  m.Dashboardz.sys
+00000f10: 7465 6d2e 4461 7368 626f 6172 644c 6179  tem.DashboardLay
+00000f20: 6f75 7473 7244 0000 00da 0d77 696e 646f  outsrD.....windo
+00000f30: 775f 6c61 796f 7574 2902 da0b 666f 726d  w_layout)...form
+00000f40: 5f70 616e 656c 7372 0d00 0000 4672 2d00  _panelsr....Fr-.
+00000f50: 0000 2935 7223 0000 00da 0b43 484f 4943  ..)5r#.....CHOIC
+00000f60: 454c 4953 5453 da05 6974 656d 73da 0373  ELISTS..items..s
+00000f70: 6574 da0b 6163 746f 7273 5f6c 6973 74da  et..actors_list.
+00000f80: 0b67 6574 5f61 6374 696f 6e73 da06 6163  .get_actions..ac
+00000f90: 7469 6f6e da03 6164 64da 1173 6572 6961  tion..add..seria
+00000fa0: 6c69 7365 5f6a 735f 636f 6465 7204 0000  lise_js_coder...
+00000fb0: 00da 0453 4954 45da 0770 6c75 6769 6e73  ...SITE..plugins
+00000fc0: da04 6469 6374 da0d 6765 745f 7369 7465  ..dict..get_site
+00000fd0: 5f6d 656e 7572 2900 0000 da06 7379 7374  _menur).....syst
+00000fe0: 656d 7257 0000 00da 0574 6974 6c65 7241  emrW.....titlerA
+00000ff0: 0000 00da 0a75 726c 5f70 7265 6669 7872  .....url_prefixr
+00001000: 5a00 0000 da0c 6973 5f69 6e73 7461 6c6c  Z.....is_install
+00001010: 6564 da06 7570 6461 7465 da04 6c69 7374  ed..update..list
+00001020: 725b 0000 00da 0670 6172 7365 72da 0a73  r[.....parser..s
+00001030: 7567 6765 7374 6572 73da 046b 6579 73da  uggesters..keys.
+00001040: 0a63 6f64 655f 6d74 696d 65da 026f 73da  .code_mtime..os.
+00001050: 0473 7461 7472 0200 0000 da0b 5354 4154  .statr......STAT
+00001060: 4943 5f52 4f4f 54da 0873 745f 6d74 696d  IC_ROOT..st_mtim
+00001070: 65da 1146 696c 654e 6f74 466f 756e 6445  e..FileNotFoundE
+00001080: 7272 6f72 da07 6861 7361 7474 7272 6000  rror..hasattrr`.
+00001090: 0000 da0a 7573 6572 5f6d 6f64 656c da05  ....user_model..
+000010a0: 7573 6572 7372 6200 0000 7263 0000 0072  usersrb...rc...r
+000010b0: 6400 0000 da09 7573 655f 6c69 6e6f 6472  d.....use_linodr
+000010c0: 6700 0000 da0a 7061 6e65 6c32 6a73 6f6e  g.....panel2json
+000010d0: da0f 5f66 6f72 6d70 616e 656c 5f6e 616d  .._formpanel_nam
+000010e0: 6572 3100 0000 7265 0000 00da 0c70 6172  er1...re.....par
+000010f0: 616d 5f70 616e 656c 73da 1361 6374 696f  am_panels..actio
+00001100: 6e5f 7061 7261 6d5f 7061 6e65 6c73 da0c  n_param_panels..
+00001110: 6f74 6865 725f 7061 6e65 6c73 da05 7772  other_panels..wr
+00001120: 6974 6572 2600 0000 290c 7240 0000 00da  iter&...).r@....
+00001130: 0166 da10 6368 6f69 6365 6c69 7374 735f  .f..choicelists_
+00001140: 6461 7461 7255 0000 00da 0372 7074 da02  datarU.....rpt..
+00001150: 6261 7271 0000 00da 0464 6174 6172 6700  barq.....datarg.
+00001160: 0000 da01 7072 3500 0000 da04 6974 656d  ....pr5.....item
+00001170: 7237 0000 0072 5100 0000 7238 0000 00da  r7...rQ...r8....
+00001180: 0d77 7269 7465 5f6c 696e 6f5f 6a73 4a00  .write_lino_jsJ.
+00001190: 0000 7370 0000 0006 0708 0306 fd06 050a  ..sp............
+000011a0: 010c 020a 010c 0102 8002 fe06 0408 0102  ................
+000011b0: 0110 010c 0206 0106 010a 0110 0106 f90c  ................
+000011c0: 0904 0210 0106 ff12 0602 0126 010c 0104  ...........&....
+000011d0: 0102 ff0c 0310 010c 020e 010c 0110 010c  ................
+000011e0: 0218 0104 090a 0110 0114 0114 010e 0112  ................
+000011f0: 0104 800a 0112 010a 0114 010a 0114 010e  ................
+00001200: 010e 0506 0204 017a 1652 656e 6465 7265  .......z.Rendere
+00001210: 722e 7772 6974 655f 6c69 6e6f 5f6a 7363  r.write_lino_jsc
+00001220: 0200 0000 0000 0000 0000 0000 0400 0000  ................
+00001230: 0600 0000 4300 0000 73c6 0000 0074 007c  ....C...s....t.|
+00001240: 0174 0183 0273 074a 0082 0174 027c 016a  .t...s.J...t.|.j
+00001250: 037c 01a0 04a1 007c 01a0 05a1 007c 016a  .|.....|.....|.j
+00001260: 0664 018d 047d 0274 007c 0174 0783 0272  .d...}.t.|.t...r
+00001270: 297c 016a 086a 096a 037c 0264 023c 0074  )|.j.j.j.|.d.<.t
+00001280: 0a7c 016a 086a 0b83 017c 0264 033c 007c  .|.j.j...|.d.<.|
+00001290: 016a 0c72 317c 016a 0c7c 0264 043c 007c  .j.r1|.j.|.d.<.|
+000012a0: 016a 0d72 397c 016a 0d7c 0264 053c 007c  .j.r9|.j.|.d.<.|
+000012b0: 016a 0e72 4064 067c 0264 073c 007c 016a  .j.r@d.|.d.<.|.j
+000012c0: 0f72 487c 016a 0f7c 0264 083c 007c 016a  .rH|.j.|.d.<.|.j
+000012d0: 1072 4f64 067c 0264 093c 007c 016a 1172  .rOd.|.d.<.|.j.r
+000012e0: 5664 067c 0264 0a3c 007c 00a0 127c 01a1  Vd.|.d.<.|...|..
+000012f0: 017d 037c 0372 617c 037c 0264 0b3c 007c  .}.|.ra|.|.d.<.|
+00001300: 0253 0029 0c7a 3343 6f6e 7665 7274 7320  .S.).z3Converts 
+00001310: 676c 6f62 616c 206c 6973 7420 6f66 2061  global list of a
+00001320: 6c6c 2061 6374 696f 6e73 2074 6f20 6a73  ll actions to js
+00001330: 6f6e 2066 6f72 6d61 742e 2904 da02 616e  on format.)...an
+00001340: da05 6c61 6265 6cda 0d77 696e 646f 775f  ..label..window_
+00001350: 6163 7469 6f6e da0b 6874 7470 5f6d 6574  action..http_met
+00001360: 686f 6472 9500 0000 da05 6163 746f 72da  hodr......actor.
+00001370: 0c70 7265 7072 6f63 6573 736f 72da 0b73  .preprocessor..s
+00001380: 656c 6563 745f 726f 7773 54da 1073 7562  elect_rowsT..sub
+00001390: 6d69 745f 666f 726d 5f64 6174 61da 0b62  mit_form_data..b
+000013a0: 7574 746f 6e5f 7465 7874 da14 7368 6f77  utton_text..show
+000013b0: 5f69 6e5f 7369 6465 5f74 6f6f 6c62 6172  _in_side_toolbar
+000013c0: da0e 6e65 7665 725f 636f 6c6c 6170 7365  ..never_collapse
+000013d0: da04 6963 6f6e 2913 da0a 6973 696e 7374  ..icon)...isinst
+000013e0: 616e 6365 7217 0000 0072 7200 0000 724e  ancer....rr...rN
+000013f0: 0000 00da 0967 6574 5f6c 6162 656c da10  .....get_label..
+00001400: 6973 5f77 696e 646f 775f 6163 7469 6f6e  is_window_action
+00001410: 7298 0000 0072 1200 0000 da0c 626f 756e  r....r......boun
+00001420: 645f 6163 7469 6f6e 726d 0000 0072 4600  d_actionrm...rF.
+00001430: 0000 7299 0000 0072 9a00 0000 729b 0000  ..r....r....r...
+00001440: 0072 9c00 0000 729d 0000 0072 9e00 0000  .r....r....r....
+00001450: 729f 0000 00da 0f67 6574 5f61 6374 696f  r......get_actio
+00001460: 6e5f 6963 6f6e 2904 7240 0000 00da 0176  n_icon).r@.....v
+00001470: da06 7265 7375 6c74 72a0 0000 0072 3700  ..resultr....r7.
+00001480: 0000 7237 0000 0072 3800 0000 724f 0000  ..r7...r8...rO..
+00001490: 009f 0000 0073 2400 0000 0e02 0604 0601  .....s$.........
+000014a0: 0601 0401 06fd 0a06 0e01 1001 1002 1002  ................
+000014b0: 0e01 1001 0e01 0e01 0a02 0c01 0402 7a14  ..............z.
+000014c0: 5265 6e64 6572 6572 2e61 6374 696f 6e32  Renderer.action2
+000014d0: 6a73 6f6e 6302 0000 0000 0000 0000 0000  jsonc...........
+000014e0: 0003 0000 0004 0000 0043 0000 0073 2e00  .........C...s..
+000014f0: 0000 7400 7c01 7401 8302 7307 4a00 8201  ..t.|.t...s.J...
+00001500: 7c01 a002 a100 7d02 7403 7c00 a004 7c02  |.....}.t.|...|.
+00001510: 6a05 a101 7c02 6a06 6a07 6401 8d02 5300  j...|.j.j.d...S.
+00001520: 2902 4e29 02da 046d 6169 6eda 0b77 696e  ).N)...main..win
+00001530: 646f 775f 7369 7a65 2908 72a1 0000 0072  dow_size).r....r
+00001540: 1d00 0000 da11 6765 745f 6c61 796f 7574  ......get_layout
+00001550: 5f68 616e 646c 6572 7200 0000 da09 656c  _handlerr.....el
+00001560: 656d 326a 736f 6e72 a800 0000 da06 6c61  em2jsonr......la
+00001570: 796f 7574 72a9 0000 0029 0372 4000 0000  youtr....).r@...
+00001580: 7292 0000 0072 a600 0000 7237 0000 0072  r....r....r7...r
+00001590: 3700 0000 7238 0000 0072 8700 0000 bc00  7...r8...r......
+000015a0: 0000 730a 0000 000e 0108 030c 0106 0106  ..s.............
+000015b0: ff7a 1352 656e 6465 7265 722e 7061 6e65  .z.Renderer.pane
+000015c0: 6c32 6a73 6f6e 6302 0000 0000 0000 0000  l2jsonc.........
+000015d0: 0000 0004 0000 0005 0000 0003 0000 0073  ...............s
+000015e0: d600 0000 7400 7c01 7401 8302 7307 4a00  ....t.|.t...s.J.
+000015f0: 8201 7402 7c01 a003 a100 7c01 6a04 6a05  ..t.|.....|.j.j.
+00001600: 6401 8d02 7d02 7406 7c01 6402 8302 7222  d...}.t.|.d...r"
+00001610: 8700 6601 6403 6404 8408 7c01 6a07 4400  ..f.d.d...|.j.D.
+00001620: 8301 7c02 6405 3c00 7c02 a008 7409 7c01  ..|.d.<.|...t.|.
+00001630: 6406 8302 a101 0100 7406 7c01 6407 8302  d.......t.|.d...
+00001640: 7253 7c02 a008 7409 7c01 6a0a 6408 8302  rS|...t.|.j.d...
+00001650: a101 0100 7406 7c01 6409 8302 7253 7c01  ....t.|.d...rS|.
+00001660: 6a0b 6400 7501 7253 7c01 6a0b a00c a100  j.d.u.rS|.j.....
+00001670: 4400 5d0b 5c02 7d03 7d01 8800 a00d 7c01  D.].\.}.}.....|.
+00001680: a101 7c02 7c03 3c00 7147 740e 7c01 6a04  ..|.|.<.qGt.|.j.
+00001690: 740f 8302 7269 7c02 6a08 7c01 a010 a100  t...ri|.j.|.....
+000016a0: 640a 8d01 0100 7c02 6a08 7c01 6a11 6a12  d.....|.j.|.j.j.
+000016b0: 640b 8d01 0100 7c02 5300 290c 4e29 0272  d.....|.S.).N).r
+000016c0: 9600 0000 da0a 7265 6163 745f 6e61 6d65  ......react_name
+000016d0: da08 656c 656d 656e 7473 6301 0000 0000  ..elementsc.....
+000016e0: 0000 0000 0000 0002 0000 0005 0000 0013  ................
+000016f0: 0000 0073 1e00 0000 6700 7c00 5d0b 7d01  ...s....g.|.].}.
+00001700: 7c01 a000 a100 7202 8800 a001 7c01 a101  |.....r.....|...
+00001710: 9102 7102 5300 7237 0000 0029 02da 0a69  ..q.S.r7...)...i
+00001720: 735f 7669 7369 626c 6572 ab00 0000 2902  s_visibler....).
+00001730: 7247 0000 00da 0165 7251 0000 0072 3700  rG.....erQ...r7.
+00001740: 0000 7238 0000 0072 4900 0000 cb00 0000  ..r8...rI.......
+00001750: 7302 0000 001e 007a 2652 656e 6465 7265  s......z&Rendere
+00001760: 722e 656c 656d 326a 736f 6e2e 3c6c 6f63  r.elem2json.<loc
+00001770: 616c 733e 2e3c 6c69 7374 636f 6d70 3e72  als>.<listcomp>r
+00001780: 6900 0000 7a98 6669 656c 6473 5f69 6e64  i...z.fields_ind
+00001790: 6578 2066 6965 6c64 735f 696e 6465 785f  ex fields_index_
+000017a0: 6869 6464 656e 2065 6469 7461 626c 6520  hidden editable 
+000017b0: 7665 7274 6963 616c 2068 7061 6420 6973  vertical hpad is
+000017c0: 5f66 6965 6c64 7365 7420 6e61 6d65 2077  _fieldset name w
+000017d0: 6964 7468 2070 7265 6665 7272 6564 5f77  idth preferred_w
+000017e0: 6964 7468 2020 2020 2020 2020 2020 2020  idth            
+000017f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001800: 2020 2020 2020 6869 6464 656e 2076 616c        hidden val
+00001810: 7565 2068 666c 6578 2076 666c 6578 7299  ue hflex vflexr.
+00001820: 0000 007a 1561 6374 6f72 5f69 6420 6469  ...z.actor_id di
+00001830: 7370 6c61 795f 6d6f 6465 da06 736c 6176  splay_mode..slav
+00001840: 6573 2901 da0d 6669 656c 645f 6f70 7469  es)...field_opti
+00001850: 6f6e 7329 01da 0968 656c 705f 7465 7874  ons)...help_text
+00001860: 2913 72a1 0000 0072 1e00 0000 7272 0000  ).r....r....rr..
+00001870: 0072 a200 0000 7243 0000 00da 085f 5f6e  .r....rC.....__n
+00001880: 616d 655f 5f72 8300 0000 72ae 0000 0072  ame__r....r....r
+00001890: 7800 0000 7228 0000 0072 9900 0000 72b1  x...r(...r....r.
+000018a0: 0000 0072 6900 0000 72ab 0000 00da 0a69  ...ri...r......i
+000018b0: 7373 7562 636c 6173 7372 2100 0000 da11  ssubclassr!.....
+000018c0: 6765 745f 6669 656c 645f 6f70 7469 6f6e  get_field_option
+000018d0: 73da 0566 6965 6c64 72b3 0000 0029 0472  s..fieldr....).r
+000018e0: 4000 0000 72a6 0000 0072 a700 0000 da01  @...r....r......
+000018f0: 6b72 3700 0000 7251 0000 0072 3800 0000  kr7...rQ...r8...
+00001900: 72ab 0000 00c4 0000 0073 2000 0000 0e01  r........s .....
+00001910: 0802 0602 06fe 0a03 1801 1002 0a04 1202  ................
+00001920: 1403 1201 1001 0c03 1001 1001 0402 7a12  ..............z.
+00001930: 5265 6e64 6572 6572 2e65 6c65 6d32 6a73  Renderer.elem2js
+00001940: 6f6e 6301 0000 0000 0000 0000 0000 0001  onc.............
+00001950: 0000 0001 0000 0043 0000 0073 0400 0000  .......C...s....
+00001960: 6401 5300 2902 4e7a 1e77 696e 646f 772e  d.S.).Nz.window.
+00001970: 4170 702e 6461 7368 626f 6172 642e 7265  App.dashboard.re
+00001980: 6c6f 6164 2829 3b72 3700 0000 7251 0000  load();r7...rQ..
+00001990: 0072 3700 0000 7237 0000 0072 3800 0000  .r7...r7...r8...
+000019a0: da09 7265 6c6f 6164 5f6a 73e3 0000 0073  ..reload_js....s
+000019b0: 0200 0000 0401 7a12 5265 6e64 6572 6572  ......z.Renderer
+000019c0: 2e72 656c 6f61 645f 6a73 6302 0000 0000  .reload_jsc.....
+000019d0: 0000 0000 0000 0006 0000 0004 0000 004f  ...............O
+000019e0: 0000 0073 dc00 0000 7c01 6a00 6a01 6401  ...s....|.j.j.d.
+000019f0: 6b02 720f 7c00 6a02 6a03 7c02 6900 7c03  k.r.|.j.j.|.i.|.
+00001a00: a401 8e01 5300 7c01 a004 a100 7d04 7c03  ....S.|.....}.|.
+00001a10: a005 7c04 6402 1900 a101 0100 7406 7c03  ..|.d.......t.|.
+00001a20: 7c01 8302 0100 7c01 6a07 6403 7501 722c  |.....|.j.d.u.r,
+00001a30: 7c03 a008 7409 6a0a 7c01 6a07 a102 0100  |...t.j.|.j.....
+00001a40: 7c01 6a0b 6403 7501 7239 7c03 a008 7409  |.j.d.u.r9|...t.
+00001a50: 6a0c 7c01 6a0b a102 0100 7c01 6a0d 6403  j.|.j.....|.j.d.
+00001a60: 7501 725c 7c01 6a0d 6404 1900 7d05 7c05  u.r\|.j.d...}.|.
+00001a70: a00e 6405 a101 7255 7c05 6406 6403 8502  ..d...rU|.d.d...
+00001a80: 1900 7d05 7c03 a008 7409 6a0f 6407 a102  ..}.|...t.j.d...
+00001a90: 0100 7c03 a008 7409 6a10 7c05 a102 0100  ..|...t.j.|.....
+00001aa0: 7c00 6a02 6a03 7c01 6a00 6a11 7c01 6a00  |.j.j.|.j.j.|.j.
+00001ab0: 6a01 6702 7c02 a201 5200 6900 7c03 a401  j.g.|...R.i.|...
+00001ac0: 8e01 5300 2908 7a20 5573 6564 2066 6f72  ..S.).z Used for
+00001ad0: 2074 7572 6e20 7265 7175 6573 7473 2069   turn requests i
+00001ae0: 6e74 6f20 7572 6c73 da04 4d61 696e da0b  nto urls..Main..
+00001af0: 6261 7365 5f70 6172 616d 734e 7201 0000  base_paramsNr...
+00001b00: 00da 012d 722d 0000 00da 0444 4553 4329  ...-r-.....DESC)
+00001b10: 1272 9900 0000 72b4 0000 0072 4100 0000  .r....r....rA...
+00001b20: da0f 6275 696c 645f 706c 6169 6e5f 7572  ..build_plain_ur
+00001b30: 6cda 0a67 6574 5f73 7461 7475 7372 7800  l..get_statusrx.
+00001b40: 0000 7208 0000 00da 066f 6666 7365 74da  ..r......offset.
+00001b50: 0a73 6574 6465 6661 756c 7472 0c00 0000  .setdefaultr....
+00001b60: da0f 5552 4c5f 5041 5241 4d5f 5354 4152  ..URL_PARAM_STAR
+00001b70: 54da 056c 696d 6974 da0f 5552 4c5f 5041  T..limit..URL_PA
+00001b80: 5241 4d5f 4c49 4d49 54da 086f 7264 6572  RAM_LIMIT..order
+00001b90: 5f62 79da 0a73 7461 7274 7377 6974 68da  _by..startswith.
+00001ba0: 1155 524c 5f50 4152 414d 5f53 4f52 5444  .URL_PARAM_SORTD
+00001bb0: 4952 da0e 5552 4c5f 5041 5241 4d5f 534f  IR..URL_PARAM_SO
+00001bc0: 5254 da09 6170 705f 6c61 6265 6c29 0672  RT..app_label).r
+00001bd0: 4000 0000 da02 6172 da04 6172 6773 da02  @.....ar..args..
+00001be0: 6b77 da02 7374 da02 7363 7237 0000 0072  kw..st..scr7...r
+00001bf0: 3700 0000 7238 0000 00da 0f67 6574 5f72  7...r8.....get_r
+00001c00: 6571 7565 7374 5f75 726c e600 0000 732c  equest_url....s,
+00001c10: 0000 000c 0212 0108 020e 010a 010a 0110  ................
+00001c20: 010a 0110 010a 010a 010a 010c 010e 010e  ................
+00001c30: 0106 030c 0102 ff02 0106 ff02 0106 ff7a  ...............z
+00001c40: 1852 656e 6465 7265 722e 6765 745f 7265  .Renderer.get_re
+00001c50: 7175 6573 745f 7572 6c4e 6305 0000 0000  quest_urlNc.....
+00001c60: 0000 0000 0000 0007 0000 0005 0000 004b  ...............K
+00001c70: 0000 0073 ae00 0000 7c04 7005 7c03 a000  ...s....|.p.|...
+00001c80: a100 7d04 7401 7c04 8301 6401 6b02 7211  ..}.t.|...d.k.r.
+00001c90: 6402 a002 7c04 a101 7d04 7c03 6a03 6a04  d...|...}.|.j.j.
+00001ca0: 722c 7c03 6a03 6a05 732c 7c00 a006 7c02  r,|.j.j.s,|...|.
+00001cb0: 7c03 7c01 a103 7d06 7c00 6a07 7c02 7c03  |.|...}.|.j.|.|.
+00001cc0: 7c06 7c04 6604 6900 7c05 a401 8e01 5300  |.|.f.i.|.....S.
+00001cd0: 7c03 6a03 6a08 724b 7c02 a009 a100 7d06  |.j.j.rK|.....}.
+00001ce0: 7c01 6400 7501 723f 7c06 6a0a 7c01 6a0b  |.d.u.r?|.j.|.j.
+00001cf0: 6403 8d01 0100 7c00 6a07 7c02 7c03 7c06  d.....|.j.|.|.|.
+00001d00: 7c04 6604 6900 7c05 a401 8e01 5300 7c00  |.f.i.|.....S.|.
+00001d10: 6a0c 7c01 7c02 7c03 7c04 6604 6900 7c05  j.|.|.|.|.f.i.|.
+00001d20: a401 8e01 5300 2904 4e72 2d00 0000 7506  ....S.).Nr-...u.
+00001d30: 0000 00c2 a07b 7dc2 a029 01da 0972 6563  .....{}..)...rec
+00001d40: 6f72 645f 6964 290d da10 6765 745f 6275  ord_id)...get_bu
+00001d50: 7474 6f6e 5f6c 6162 656c da03 6c65 6eda  tton_label..len.
+00001d60: 0666 6f72 6d61 7472 6d00 0000 da0a 7061  .formatrm.....pa
+00001d70: 7261 6d65 7465 7273 da10 6e6f 5f70 6172  rameters..no_par
+00001d80: 616d 735f 7769 6e64 6f77 da11 6765 745f  ams_window..get_
+00001d90: 6163 7469 6f6e 5f73 7461 7475 73da 1477  action_status..w
+00001da0: 696e 646f 775f 6163 7469 6f6e 5f62 7574  indow_action_but
+00001db0: 746f 6eda 0e6f 7065 6e73 5f61 5f77 696e  ton..opens_a_win
+00001dc0: 646f 7772 bf00 0000 7278 0000 00da 0270  dowr....rx.....p
+00001dd0: 6bda 1172 6f77 5f61 6374 696f 6e5f 6275  k..row_action_bu
+00001de0: 7474 6f6e 2907 7240 0000 00da 036f 626a  tton).r@.....obj
+00001df0: 72ca 0000 0072 9000 0000 7296 0000 0072  r....r....r....r
+00001e00: cc00 0000 72cd 0000 0072 3700 0000 7237  ....r....r7...r7
+00001e10: 0000 0072 3800 0000 da0d 6163 7469 6f6e  ...r8.....action
+00001e20: 5f62 7574 746f 6efe 0000 0073 2000 0000  _button....s ...
+00001e30: 0c01 0c01 0a01 1002 0e01 0401 0801 04ff  ................
+00001e40: 0201 06ff 0802 0801 0801 0e01 1801 1801  ................
+00001e50: 7a16 5265 6e64 6572 6572 2e61 6374 696f  z.Renderer.actio
+00001e60: 6e5f 6275 7474 6f6e 6305 0000 0000 0000  n_buttonc.......
+00001e70: 0000 0000 0007 0000 0004 0000 004b 0000  .............K..
+00001e80: 0073 4000 0000 7c02 6401 7500 720d 7c03  .s@...|.d.u.r.|.
+00001e90: 6a00 6402 6900 7c04 a401 8e01 7d06 6e09  j.d.i.|.....}.n.
+00001ea0: 7c02 6a01 7c03 6601 6900 7c04 a401 8e01  |.j.|.f.i.|.....
+00001eb0: 7d06 7c00 6a02 7c06 7c01 6602 6900 7c05  }.|.j.|.|.f.i.|.
+00001ec0: a401 8e01 5300 2903 61cf 0100 004e 6f74  ....S.).a....Not
+00001ed0: 6520 7468 6174 2060 6261 2e61 6374 6f72  e that `ba.actor
+00001ee0: 6020 6d61 7920 6469 6666 6572 2066 726f  ` may differ fro
+00001ef0: 6d20 6061 722e 6163 746f 7260 2077 6865  m `ar.actor` whe
+00001f00: 6e20 6465 6669 6e65 6420 6f6e 2061 0a20  n defined on a. 
+00001f10: 2020 2020 2020 2064 6966 6665 7265 6e74         different
+00001f20: 2061 6374 6f72 2e20 5265 6d65 6d62 6572   actor. Remember
+00001f30: 2065 2e67 2e20 7468 6520 224d 7573 7420   e.g. the "Must 
+00001f40: 7265 6164 2065 4944 2063 6172 6422 2061  read eID card" a
+00001f50: 6374 696f 6e0a 2020 2020 2020 2020 6275  ction.        bu
+00001f60: 7474 6f6e 2069 6e20 6569 645f 696e 666f  tton in eid_info
+00001f70: 206f 6620 6e65 7763 6f6d 6572 732e 4e65   of newcomers.Ne
+00001f80: 7743 6c69 656e 7473 2028 3230 3134 3034  wClients (201404
+00001f90: 3232 292e 0a0a 2020 2020 2020 2020 3a6f  22)...        :o
+00001fa0: 626a 3a20 2054 6865 2064 6174 6162 6173  bj:  The databas
+00001fb0: 6520 6f62 6a65 6374 0a20 2020 2020 2020  e object.       
+00001fc0: 203a 6172 3a20 2020 5468 6520 6163 7469   :ar:   The acti
+00001fd0: 6f6e 2072 6571 7565 7374 0a20 2020 2020  on request.     
+00001fe0: 2020 203a 6261 3a20 2054 6865 2062 6f75     :ba:  The bou
+00001ff0: 6e64 2061 6374 696f 6e0a 2020 2020 2020  nd action.      
+00002000: 2020 3a72 6571 7565 7374 5f6b 7761 7267    :request_kwarg
+00002010: 733a 206b 6579 776f 7264 2061 7267 756d  s: keyword argum
+00002020: 656e 7473 2074 6f20 666f 7277 6172 6465  ents to forwarde
+00002030: 6420 746f 2074 6865 2063 6869 6c64 2061  d to the child a
+00002040: 6374 696f 6e20 7265 7175 6573 740a 0a20  ction request.. 
+00002050: 2020 2020 2020 2041 6e79 206b 6579 776f         Any keywo
+00002060: 7264 206f 7468 6572 2061 7267 756d 656e  rd other argumen
+00002070: 7473 2061 7265 2066 6f72 7761 7264 6564  ts are forwarded
+00002080: 2074 6f20 3a6d 6574 683a 6061 7232 6a73   to :meth:`ar2js
+00002090: 602e 0a0a 2020 2020 2020 2020 4e72 3700  `...        Nr7.
+000020a0: 0000 2903 da07 7265 7175 6573 74da 0573  ..)...request..s
+000020b0: 7061 776e da05 6172 326a 7329 0772 4000  pawn..ar2js).r@.
+000020c0: 0000 72db 0000 0072 ca00 0000 7290 0000  ..r....r....r...
+000020d0: 00da 0e72 6571 7565 7374 5f6b 7761 7267  ...request_kwarg
+000020e0: 73da 0673 7461 7475 73da 0373 6172 7237  s..status..sarr7
+000020f0: 0000 0072 3700 0000 7238 0000 00da 1761  ...r7...r8.....a
+00002100: 6374 696f 6e5f 6361 6c6c 5f6f 6e5f 696e  ction_call_on_in
+00002110: 7374 616e 6365 0f01 0000 7308 0000 0008  stance....s.....
+00002120: 0e12 0112 0314 017a 2052 656e 6465 7265  .......z Rendere
+00002130: 722e 6163 7469 6f6e 5f63 616c 6c5f 6f6e  r.action_call_on
+00002140: 5f69 6e73 7461 6e63 6563 0200 0000 0000  _instancec......
+00002150: 0000 0000 0000 0400 0000 0400 0000 4300  ..............C.
+00002160: 0000 732c 0000 007c 016a 0070 057c 016a  ..s,...|.j.p.|.j
+00002170: 017d 0274 02a0 037c 0264 01a1 027d 037c  .}.t...|.d...}.|
+00002180: 0364 0175 0072 1264 0153 0064 027c 0316  .d.u.r.d.S.d.|..
+00002190: 0053 0029 037a bf0a 2020 2020 2020 2020  .S.).z..        
+000021a0: 5573 6573 2061 6e20 696e 7465 726e 616c  Uses an internal
+000021b0: 206d 6170 7069 6e67 2066 6f72 2069 636f   mapping for ico
+000021c0: 6e20 6e61 6d65 7320 746f 2063 6f6e 7665  n names to conve
+000021d0: 7274 2065 7869 7374 696e 6720 6963 6f6e  rt existing icon
+000021e0: 7320 696e 746f 2072 6561 6374 2d75 7361  s into react-usa
+000021f0: 626c 652e 0a20 2020 2020 2020 203a 7061  ble..        :pa
+00002200: 7261 6d20 6163 7469 6f6e 3a0a 2020 2020  ram action:.    
+00002210: 2020 2020 3a72 6574 7572 6e3a 2073 7472      :return: str
+00002220: 3a20 6120 6963 6f6e 206e 616d 6520 666f  : a icon name fo
+00002230: 7220 6569 7468 6572 2070 7269 6d65 2d72  r either prime-r
+00002240: 6561 6374 206f 7220 6963 6f6e 380a 2020  eact or icon8.  
+00002250: 2020 2020 2020 4e7a 0570 6920 2573 2904        Nz.pi %s).
+00002260: da0f 7265 6163 745f 6963 6f6e 5f6e 616d  ..react_icon_nam
+00002270: 65da 0969 636f 6e5f 6e61 6d65 722e 0000  e..icon_namer...
+00002280: 00da 0367 6574 2904 7240 0000 0072 6d00  ...get).r@...rm.
+00002290: 0000 72a0 0000 00da 0a72 6561 6374 5f69  ..r......react_i
+000022a0: 636f 6e72 3700 0000 7237 0000 0072 3800  conr7...r7...r8.
+000022b0: 0000 72a5 0000 0024 0100 0073 0a00 0000  ..r....$...s....
+000022c0: 0c07 0c01 0801 0401 0802 7a18 5265 6e64  ..........z.Rend
+000022d0: 6572 6572 2e67 6574 5f61 6374 696f 6e5f  erer.get_action_
+000022e0: 6963 6f6e 6303 0000 0000 0000 0000 0000  iconc...........
+000022f0: 0008 0000 0007 0000 004b 0000 0073 a400  .........K...s..
+00002300: 0000 7c01 6a00 7d04 7c01 6a01 7d05 6900  ..|.j.}.|.j.}.i.
+00002310: 7d06 7c05 6a02 a003 a100 721c 7c03 a004  }.|.j.....r.|...
+00002320: 7c00 a005 7c01 7c05 7c02 a103 a101 0100  |...|.|.|.......
+00002330: 7c06 a004 7c03 a101 0100 7c06 a004 7c00  |...|.....|...|.
+00002340: a006 7c01 7c05 7c02 a103 a101 0100 7c06  ..|.|.|.......|.
+00002350: a004 7c03 a101 0100 7c04 7c05 6a02 6a07  ..|.....|.|.j.j.
+00002360: 7c01 6a08 7c05 6a09 6a0a 7c06 6401 9c05  |.j.|.j.j.|.d...
+00002370: 7d07 740b 7c02 6402 8302 7243 7c02 6a0c  }.t.|.d...rC|.j.
+00002380: 7c07 6403 3c00 6e09 740d 7c02 740e 8302  |.d.<.n.t.|.t...
+00002390: 724c 7c02 7c07 6403 3c00 6404 740f 7c07  rL|.|.d.<.d.t.|.
+000023a0: 8301 1600 5300 2905 7a43 496d 706c 656d  ....S.).zCImplem
+000023b0: 656e 7473 203a 6d65 7468 3a60 6c69 6e6f  ents :meth:`lino
+000023c0: 2e63 6f72 652e 7265 6e64 6572 6572 2e48  .core.renderer.H
+000023d0: 746d 6c52 656e 6465 7265 722e 6172 326a  tmlRenderer.ar2j
+000023e0: 7360 2e0a 0a20 2020 2020 2020 2029 05da  s`...        )..
+000023f0: 0272 7072 9500 0000 da06 6f6e 4d61 696e  .rpr......onMain
+00002400: da07 6163 746f 7249 6472 e100 0000 72d9  ..actorIdr....r.
+00002410: 0000 00da 0273 72fa 1877 696e 646f 772e  .....sr..window.
+00002420: 4170 702e 7275 6e41 6374 696f 6e28 2573  App.runAction(%s
+00002430: 2929 10da 1072 6571 7565 7374 696e 675f  ))...requesting_
+00002440: 7061 6e65 6c72 a400 0000 726d 0000 0072  panelr....rm...r
+00002450: a300 0000 7278 0000 0072 d600 0000 da11  ....rx...r......
+00002460: 6765 745f 6163 7469 6f6e 5f70 6172 616d  get_action_param
+00002470: 7372 4e00 0000 da10 6973 5f6f 6e5f 6d61  srN.....is_on_ma
+00002480: 696e 5f61 6374 6f72 7299 0000 00da 0861  in_actorr......a
+00002490: 6374 6f72 5f69 6472 8300 0000 72d9 0000  ctor_idr....r...
+000024a0: 0072 a100 0000 7279 0000 0072 2600 0000  .r....ry...r&...
+000024b0: 2908 7240 0000 0072 ca00 0000 72db 0000  ).r@...r....r...
+000024c0: 0072 e100 0000 72e8 0000 0072 9000 0000  .r....r....r....
+000024d0: da06 7061 7261 6d73 da06 6a73 5f6f 626a  ..params..js_obj
+000024e0: 7237 0000 0072 3700 0000 7238 0000 0072  r7...r7...r8...r
+000024f0: df00 0000 3201 0000 732a 0000 0006 0406  ....2...s*......
+00002500: 0104 010a 0114 040a 0114 010a 0102 0306  ................
+00002510: 0104 0106 0102 0106 fb0a 070c 010a 0208  ................
+00002520: 0102 0206 0104 ff7a 0e52 656e 6465 7265  .......z.Rendere
+00002530: 722e 6172 326a 7363 0200 0000 0000 0000  r.ar2jsc........
+00002540: 0000 0000 0600 0000 0600 0000 4300 0000  ............C...
+00002550: 73bc 0100 007c 0174 006a 016a 0275 0072  s....|.t.j.j.u.r
+00002560: 0a74 0364 0183 0153 0074 047c 0174 0583  .t.d...S.t.|.t..
+00002570: 0272 1674 0664 02a0 077c 01a1 0183 0182  .r.t.d...|......
+00002580: 0174 047c 0174 086a 0983 0272 2009 007c  .t.|.t.j...r ..|
+00002590: 016a 0a53 0074 047c 0174 0b6a 0c83 0272  .j.S.t.|.t.j...r
+000025a0: 297c 016a 0d53 0074 047c 0174 0683 0272  )|.j.S.t.|.t...r
+000025b0: 3274 0e7c 0183 0153 0074 047c 0174 0f83  2t.|...S.t.|.t..
+000025c0: 0272 4a7c 016a 1064 0375 0072 3f7c 016a  .rJ|.j.d.u.r?|.j
+000025d0: 1153 0074 127c 016a 1374 127c 016a 1164  .S.t.|.j.t.|.j.d
+000025e0: 048d 0164 058d 0253 0074 047c 0174 1483  ...d...S.t.|.t..
+000025f0: 0272 cc7c 016a 1564 0375 0172 6d7c 00a0  .r.|.j.d.u.rm|..
+00002600: 1664 037c 016a 1564 03a1 037d 027c 0264  .d.|.j.d...}.|.d
+00002610: 0375 0173 624a 0082 0164 067c 0216 007d  .u.sbJ...d.|...}
+00002620: 037c 00a0 177c 017c 0264 03a1 0353 007c  .|...|.|.d...S.|
+00002630: 016a 1864 0375 0172 957c 016a 1972 857c  .j.d.u.r.|.j.r.|
+00002640: 016a 186a 1a64 0d69 007c 016a 19a4 018e  .j.j.d.i.|.j....
+00002650: 017d 047c 00a0 1b7c 04a1 017d 036e 087c  .}.|...|...}.n.|
+00002660: 00a0 1c64 037c 016a 1869 00a1 037d 037c  ...d.|.j.i...}.|
+00002670: 00a0 177c 017c 037c 016a 1da1 0353 007c  ...|.|.|.j...S.|
+00002680: 016a 1e64 0375 0172 a764 067c 016a 1e16  .j.d.u.r.d.|.j..
+00002690: 007d 037c 00a0 177c 017c 037c 016a 1da1  .}.|...|.|.|.j..
+000026a0: 0353 007c 016a 1f64 0375 0172 b07c 016a  .S.|.j.d.u.r.|.j
+000026b0: 1f7d 056e 037c 016a 1353 007c 016a 106a  .}.n.|.j.S.|.j.j
+000026c0: 1064 0375 0072 c574 1264 077c 016a 1374  .d.u.r.t.d.|.j.t
+000026d0: 0364 087c 0516 0083 0164 098d 0353 0074  .d.|.....d...S.t
+000026e0: 127c 016a 137c 0564 0a8d 0253 0074 047c  .|.j.|.d...S.t.|
+000026f0: 0174 0383 0272 dc74 207c 0064 0b64 0c83  .t...r.t |.d.d..
+00002700: 0372 dc74 0e7c 016a 2183 0153 007c 0153  .r.t.|.j!..S.|.S
+00002710: 0029 0e7a 540a 2020 2020 2020 2020 4164  .).zT.        Ad
+00002720: 6469 7469 6f6e 616c 2063 6f6e 7665 7274  ditional convert
+00002730: 696e 6720 6c6f 6769 6320 666f 7220 7365  ing logic for se
+00002740: 7269 616c 697a 696e 6720 5079 7468 6f6e  rializing Python
+00002750: 2076 616c 7565 7320 746f 206a 736f 6e2e   values to json.
+00002760: 0a20 2020 2020 2020 20da 104c 414e 4755  .        ..LANGU
+00002770: 4147 455f 4348 4f49 4345 537a 0b32 3032  AGE_CHOICESz.202
+00002780: 3130 3531 3720 7b7d 4e29 0172 6900 0000  10517 {}N).ri...
+00002790: 2902 7245 0000 0072 5600 0000 7a02 2573  ).rE...rV...z.%s
+000027a0: da06 6275 7474 6f6e 7a23 6675 6e63 7469  ..buttonz#functi
+000027b0: 6f6e 2829 207b 204c 696e 6f2e 6c6f 6164  on() { Lino.load
+000027c0: 5f75 726c 2827 2573 2729 3b20 7d29 03da  _url('%s'); })..
+000027d0: 0578 7479 7065 7245 0000 00da 0768 616e  .xtyperE.....han
+000027e0: 646c 6572 2902 7245 0000 00da 0468 7265  dler).rE.....hre
+000027f0: 6672 6f00 0000 4672 3700 0000 2922 7204  fro...Fr7...)"r.
+00002800: 0000 0072 7000 0000 72f3 0000 0072 2700  ...rp...r....r'.
+00002810: 0000 72a1 0000 0072 1c00 0000 da09 4578  ..r....r......Ex
+00002820: 6365 7074 696f 6e72 d300 0000 720d 0000  ceptionr....r...
+00002830: 00da 0643 686f 6963 6572 4400 0000 7205  ...ChoicerD...r.
+00002840: 0000 00da 054d 6f64 656c 72d9 0000 0072  .....Modelr....r
+00002850: 4600 0000 720a 0000 00da 0670 6172 656e  F...r......paren
+00002860: 7472 6900 0000 7272 0000 0072 9600 0000  tri...rr...r....
+00002870: 720b 0000 00da 0869 6e73 7461 6e63 65da  r......instance.
+00002880: 1069 6e73 7461 6e63 655f 6861 6e64 6c65  .instance_handle
+00002890: 72da 0c68 616e 646c 6572 5f69 7465 6d72  r..handler_itemr
+000028a0: a400 0000 72f1 0000 0072 dd00 0000 da0f  ....r....r......
+000028b0: 7265 7175 6573 745f 6861 6e64 6c65 72da  request_handler.
+000028c0: 0b61 6374 696f 6e5f 6361 6c6c 72b3 0000  .action_callr...
+000028d0: 00da 0a6a 6176 6173 6372 6970 7472 f700  ...javascriptr..
+000028e0: 0000 da07 6765 7461 7474 72da 0173 2906  ....getattr..s).
+000028f0: 7240 0000 0072 a600 0000 da01 68da 026a  r@...r......h..j
+00002900: 7372 ca00 0000 da03 7572 6c72 3700 0000  sr......urlr7...
+00002910: 7237 0000 0072 3800 0000 723f 0000 0053  r7...r8...r?...S
+00002920: 0100 0073 5400 0000 0c04 0801 0a01 0e01  ...sT...........
+00002930: 0c01 0201 0603 0c01 0601 0a01 0801 0a01  ................
+00002940: 0a01 0601 1603 0a02 0a01 1001 0c01 0801  ................
+00002950: 0e01 0a01 0601 1401 0c01 1002 1001 0a02  ................
+00002960: 0a01 1001 0a01 0801 0607 0c02 0202 0601  ................
+00002970: 0a02 06fd 0e04 1602 0a02 0402 7a18 5265  ............z.Re
+00002980: 6e64 6572 6572 2e70 7932 6a73 5f63 6f6e  nderer.py2js_con
+00002990: 7665 7274 6572 6304 0000 0000 0000 0000  verterc.........
+000029a0: 0000 0005 0000 0004 0000 0043 0000 0073  ...........C...s
+000029b0: 5000 0000 7400 7c01 6a01 7c02 6401 8d02  P...t.|.j.|.d...
+000029c0: 7d04 7c01 6a02 721a 7c01 6a02 6a03 6a04  }.|.j.r.|.j.j.j.
+000029d0: 721a 7c04 6a05 6402 7c01 6a02 6a03 6a04  r.|.j.d.|.j.j.j.
+000029e0: 1700 6403 8d01 0100 7406 6a07 6a08 7226  ..d.....t.j.j.r&
+000029f0: 7c03 7226 7c04 6a05 7c03 6404 8d01 0100  |.r&|.j.|.d.....
+00002a00: 7c04 5300 2905 da00 2902 7245 0000 0072  |.S.)...).rE...r
+00002a10: f600 0000 7a07 782d 7462 6172 2d29 01da  ....z.x-tbar-)..
+00002a20: 0769 636f 6e43 6c73 2901 da07 746f 6f6c  .iconCls)...tool
+00002a30: 5469 7029 0972 7200 0000 7296 0000 0072  Tip).rr...r....r
+00002a40: a400 0000 726d 0000 0072 e500 0000 7278  ....rm...r....rx
+00002a50: 0000 0072 0400 0000 7270 0000 00da 0d75  ...r....rp.....u
+00002a60: 7365 5f71 7569 636b 7469 7073 2905 7240  se_quicktips).r@
+00002a70: 0000 00da 026d 6972 f600 0000 72b3 0000  .....mir....r...
+00002a80: 00da 0164 7237 0000 0072 3700 0000 7238  ...dr7...r7...r8
+00002a90: 0000 0072 fe00 0000 a101 0000 730c 0000  ...r........s...
+00002aa0: 000e 0410 0116 010c 010c 0304 017a 1552  .............z.R
+00002ab0: 656e 6465 7265 722e 6861 6e64 6c65 725f  enderer.handler_
+00002ac0: 6974 656d 6302 0000 0000 0000 0000 0000  itemc...........
+00002ad0: 0005 0000 0005 0000 004f 0000 0073 2000  .........O...s .
+00002ae0: 0000 7c01 6a00 6402 6900 7c03 a401 8e01  ..|.j.d.i.|.....
+00002af0: 7d04 7c00 a001 7c01 7c01 6a02 7c04 a103  }.|...|.|.j.|...
+00002b00: 5300 2903 7a36 2047 656e 6572 6174 6573  S.).z6 Generates
+00002b10: 206a 7320 7374 7269 6e67 2066 6f72 2061   js string for a
+00002b20: 6374 696f 6e20 6275 7474 6f6e 2063 616c  ction button cal
+00002b30: 6c73 2e0a 2020 2020 2020 2020 4e72 3700  ls..        Nr7.
+00002b40: 0000 2903 72bf 0000 0072 0001 0000 72a4  ..).r....r....r.
+00002b50: 0000 0029 0572 4000 0000 72ca 0000 0072  ...).r@...r....r
+00002b60: cb00 0000 72cc 0000 0072 cd00 0000 7237  ....r....r....r7
+00002b70: 0000 0072 3700 0000 7238 0000 0072 ff00  ...r7...r8...r..
+00002b80: 0000 af01 0000 7304 0000 0010 0410 017a  ......s........z
+00002b90: 1852 656e 6465 7265 722e 7265 7175 6573  .Renderer.reques
+00002ba0: 745f 6861 6e64 6c65 7263 0400 0000 0000  t_handlerc......
+00002bb0: 0000 0000 0000 0800 0000 0800 0000 4300  ..............C.
+00002bc0: 0000 739c 0000 007c 026a 007d 047c 02a0  ..s....|.j.}.|..
+00002bd0: 01a1 00a0 0264 0164 02a1 025c 027d 057d  .....d.d...\.}.}
+00002be0: 067c 0373 1169 007d 037c 0164 0075 0172  .|.s.i.}.|.d.u.r
+00002bf0: 2274 037c 0164 0383 0272 227c 016a 0464  "t.|.d...r"|.j.d
+00002c00: 0869 007c 03a4 018e 017d 037c 0172 2d7c  .i.|.....}.|.r-|
+00002c10: 016a 0572 2d7c 016a 057c 0374 066a 073c  .j.r-|.j.|.t.j.<
+00002c20: 007c 0664 046b 0272 3974 037c 0364 0583  .|.d.k.r9t.|.d..
+00002c30: 0272 397c 0364 053d 007c 0164 0075 0072  .r9|.d.=.|.d.u.r
+00002c40: 3f64 006e 027c 016a 087d 0764 0674 0974  ?d.n.|.j.}.d.t.t
+00002c50: 0a7c 067c 057c 037c 0764 078d 0483 0116  .|.|.|.|.d......
+00002c60: 0053 0029 094e da01 2e72 2d00 0000 72bf  .S.).N...r-...r.
+00002c70: 0000 00da 0467 7269 6472 d000 0000 72ec  .....gridr....r.
+00002c80: 0000 0029 0472 9500 0000 72ea 0000 0072  ...).r....r....r
+00002c90: e100 0000 72e8 0000 0072 3700 0000 290b  ....r....r7...).
+00002ca0: 726d 0000 00da 0966 756c 6c5f 6e61 6d65  rm.....full_name
+00002cb0: da06 7273 706c 6974 7283 0000 0072 bf00  ..rsplitr....r..
+00002cc0: 0000 da0a 7375 6273 745f 7573 6572 720c  ....subst_userr.
+00002cd0: 0000 00da 1455 524c 5f50 4152 414d 5f53  .....URL_PARAM_S
+00002ce0: 5542 5354 5f55 5345 5272 ed00 0000 7226  UBST_USERr....r&
+00002cf0: 0000 0072 7200 0000 2908 7240 0000 0072  ...rr...).r@...r
+00002d00: ca00 0000 72a4 0000 0072 e100 0000 7250  ....r....r....rP
+00002d10: 0000 0072 ea00 0000 7295 0000 0072 e800  ...r....r....r..
+00002d20: 0000 7237 0000 0072 3700 0000 7238 0000  ..r7...r7...r8..
+00002d30: 0072 0001 0000 b901 0000 7322 0000 0006  .r........s"....
+00002d40: 0214 0204 0204 0112 0210 010a 020c 0112  ................
+00002d50: 1106 0112 0206 0202 0102 0102 0102 010a  ................
+00002d60: fc7a 1452 656e 6465 7265 722e 6163 7469  .z.Renderer.acti
+00002d70: 6f6e 5f63 616c 6c63 0200 0000 0000 0000  on_callc........
+00002d80: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
+00002d90: 732e 0000 007c 0173 0464 0053 0074 007c  s....|.s.d.S.t.|
+00002da0: 0174 0183 0273 0d74 017c 0183 017d 0174  .t...s.t.|...}.t
+00002db0: 027c 0164 0164 028d 027d 0164 037c 0117  .|.d.d...}.d.|..
+00002dc0: 0053 0029 044e 4629 01da 0571 756f 7465  .S.).NF)...quote
+00002dd0: 7a0b 6a61 7661 7363 7269 7074 3a29 0372  z.javascript:).r
+00002de0: a100 0000 7246 0000 0072 0300 0000 2902  ....rF...r....).
+00002df0: 7240 0000 0072 0501 0000 7237 0000 0072  r@...r....r7...r
+00002e00: 3700 0000 7238 0000 00da 066a 7332 7572  7...r8.....js2ur
+00002e10: 6ce3 0100 0073 0c00 0000 0401 0401 0a02  l....s..........
+00002e20: 0801 0c01 0801 7a0f 5265 6e64 6572 6572  ......z.Renderer
+00002e30: 2e6a 7332 7572 6c63 0600 0000 0000 0000  .js2urlc........
+00002e40: 0000 0000 0700 0000 0400 0000 4300 0000  ............C...
+00002e50: 7356 0000 0074 006a 016a 0272 2774 006a  sV...t.j.j.r't.j
+00002e60: 016a 0372 0f64 017c 047c 0566 0216 007d  .j.r.d.|.|.f...}
+00002e70: 066e 0264 027d 067c 0272 1974 0464 037c  .n.d.}.|.r.t.d.|
+00002e80: 067c 0283 037d 067c 0672 297c 016a 0564  .|...}.|.r)|.j.d
+00002e90: 047c 037c 0666 0216 0064 058d 0101 0064  .|.|.f...d.....d
+00002ea0: 0053 0064 0053 0064 0053 0029 064e 7a08  .S.d.S.d.S.).Nz.
+00002eb0: 2825 732e 2573 2920 7207 0100 007a 047b  (%s.%s) r....z.{
+00002ec0: 7d7b 7d7a 0728 2573 2c25 7329 2901 da08  }{}z.(%s,%s))...
+00002ed0: 7175 6963 6b74 6970 2906 7204 0000 0072  quicktip).r....r
+00002ee0: 7000 0000 720a 0100 00da 1973 686f 775f  p...r......show_
+00002ef0: 696e 7465 726e 616c 5f66 6965 6c64 5f6e  internal_field_n
+00002f00: 616d 6573 7206 0000 0072 7800 0000 2907  amesr....rx...).
+00002f10: 7240 0000 0072 cc00 0000 72b3 0000 0072  r@...r....r....r
+00002f20: 7500 0000 da0a 6461 7461 736f 7572 6365  u.....datasource
+00002f30: da09 6669 656c 646e 616d 65da 0374 7474  ..fieldname..ttt
+00002f40: 7237 0000 0072 3700 0000 7238 0000 00da  r7...r7...r8....
+00002f50: 0d61 6464 5f68 656c 705f 7465 7874 ec01  .add_help_text..
+00002f60: 0000 7318 0000 0008 0108 010e 0104 0204  ..s.............
+00002f70: 010c 0104 0108 0402 010e ff04 f504 077a  ...............z
+00002f80: 1652 656e 6465 7265 722e 6164 645f 6865  .Renderer.add_he
+00002f90: 6c70 5f74 6578 7463 0200 0000 0000 0000  lp_textc........
+00002fa0: 0000 0000 0500 0000 0300 0000 4300 0000  ............C...
+00002fb0: 7356 0000 0074 0083 007d 0264 017c 0117  sV...t...}.d.|..
+00002fc0: 0064 0217 007d 037c 006a 01a0 0264 03a1  .d...}.|.j...d..
+00002fd0: 0164 0419 007d 047c 0264 0575 0172 1c7c  .d...}.|.d.u.r.|
+00002fe0: 037c 026a 0364 0217 0037 007d 037c 0374  .|.j.d...7.}.|.t
+00002ff0: 04a0 05a1 0064 0317 007c 0417 0037 007d  .....d...|...7.}
+00003000: 0364 067c 047c 0366 0353 0029 077a 2c4c  .d.|.|.f.S.).z,L
+00003010: 696b 6520 6c69 6e6f 5f6a 735f 7061 7274  ike lino_js_part
+00003020: 732c 2062 7574 2066 6f72 2061 6374 6f72  s, but for actor
+00003030: 5f6c 6576 656c 2064 6174 61da 054c 696e  _level data..Lin
+00003040: 6f5f da01 5f72 0d01 0000 722f 0000 004e  o_.._r....r/...N
+00003050: da05 6361 6368 6529 0672 2900 0000 da11  ..cache).r).....
+00003060: 6c69 6e6f 5f77 6562 5f74 656d 706c 6174  lino_web_templat
+00003070: 6572 1001 0000 7244 0000 0072 0700 0000  er....rD...r....
+00003080: da0c 6765 745f 6c61 6e67 7561 6765 2905  ..get_language).
+00003090: 7240 0000 0072 ea00 0000 da09 7573 6572  r@...r......user
+000030a0: 5f74 7970 65da 0866 696c 656e 616d 65da  _type..filename.
+000030b0: 0966 696c 655f 7479 7065 7237 0000 0072  .file_typer7...r
+000030c0: 3700 0000 7238 0000 00da 156c 696e 6f5f  7...r8.....lino_
+000030d0: 6a73 5f70 6172 7473 5f63 6875 6e6b 6564  js_parts_chunked
+000030e0: fb01 0000 730e 0000 0006 020c 0110 0108  ....s...........
+000030f0: 010e 0114 010a 017a 1e52 656e 6465 7265  .......z.Rendere
+00003100: 722e 6c69 6e6f 5f6a 735f 7061 7274 735f  r.lino_js_parts_
+00003110: 6368 756e 6b65 6463 0200 0000 0000 0000  chunkedc........
+00003120: 0000 0000 1100 0000 0600 0000 4300 0000  ............C...
+00003130: 73de 0100 0067 007d 0267 007d 037c 0144  s....g.}.g.}.|.D
+00003140: 005d e47d 047c 04a0 00a1 007d 057c 0573  .].}.|.....}.|.s
+00003150: 127c 046a 016a 0272 cc74 036a 047c 046a  .|.j.j.r.t.j.|.j
+00003160: 016a 0569 017d 067c 0572 237c 066a 067c  .j.i.}.|.r#|.j.|
+00003170: 056a 076a 0864 018d 0101 007c 046a 016a  .j.j.d.....|.j.j
+00003180: 0272 c767 007d 0774 0983 007d 087c 046a  .r.g.}.t...}.|.j
+00003190: 0aa0 0b7c 046a 0174 0c83 00a1 0244 005d  ...|.j.t.....D.]
+000031a0: 727d 0974 097c 096a 016a 0564 028d 017d  r}.t.|.j.j.d...}
+000031b0: 0a7c 096a 016a 0d7d 0b7c 0b72 487c 0b7c  .|.j.j.}.|.rH|.|
+000031c0: 0a64 033c 007c 096a 016a 0e7d 0c7c 0c72  .d.<.|.j.j.}.|.r
+000031d0: 5e74 0f7c 0c83 0172 5a7c 0c7c 096a 0a83  ^t.|...rZ|.|.j..
+000031e0: 017c 0a64 043c 006e 047c 0c7c 0a64 043c  .|.d.<.n.|.|.d.<
+000031f0: 007c 096a 016a 1064 0575 0172 847c 096a  .|.j.j.d.u.r.|.j
+00003200: 016a 107d 0d7c 0d7c 0876 0072 747c 087c  .j.}.|.|.v.rt|.|
+00003210: 0d19 00a0 117c 0aa1 0101 006e 1574 097c  .....|.....n.t.|
+00003220: 0d64 068d 017d 0e7c 0a67 017c 087c 0d3c  .d...}.|.g.|.|.<
+00003230: 007c 07a0 117c 0ea1 0101 006e 057c 07a0  .|...|.....n.|..
+00003240: 117c 0aa1 0101 007c 096a 016a 1272 a774  .|.....|.j.j.r.t
+00003250: 137c 096a 016a 1283 017d 0f74 147c 0f64  .|.j.j...}.t.|.d
+00003260: 0783 0273 9e7c 096a 016a 057c 0f64 073c  ...s.|.j.j.|.d.<
+00003270: 007c 0f7c 0376 0172 a77c 03a0 117c 0fa1  .|.|.v.r.|...|..
+00003280: 0101 0071 357c 0872 c374 157c 0783 0144  ...q5|.r.t.|...D
+00003290: 005d 145c 027d 107d 0a7c 0aa0 1664 0864  .].\.}.}.|...d.d
+000032a0: 09a1 0272 c27c 087c 0a64 0819 0019 007c  ...r.|.|.d.....|
+000032b0: 077c 1019 0064 0a3c 0071 ae7c 077c 0664  .|...d.<.q.|.|.d
+000032c0: 0b3c 007c 02a0 117c 06a1 0101 007c 046a  .<.|...|.....|.j
+000032d0: 016a 1272 ea74 137c 046a 016a 1283 017d  .j.r.t.|.j.j...}
+000032e0: 0f74 147c 0f64 0783 0273 e17c 046a 016a  .t.|.d...s.|.j.j
+000032f0: 057c 0f64 073c 007c 0f7c 0376 0172 ea7c  .|.d.<.|.|.v.r.|
+00003300: 03a0 117c 0fa1 0101 0071 067c 027c 0366  ...|.....q.|.|.f
+00003310: 0253 0029 0c7a 4543 6f6e 7665 7274 7320  .S.).zEConverts 
+00003320: 6f66 2061 6c6c 2074 6865 2062 6f75 6e64  of all the bound
+00003330: 6163 7469 6f6e 7320 6f66 2061 6e20 6163  actions of an ac
+00003340: 746f 7220 746f 206a 736f 6e20 666f 726d  tor to json form
+00003350: 6174 2e0a 2020 2020 2020 2020 a901 7266  at..        ..rf
+00003360: 0000 0029 0172 9500 0000 72b3 0000 00da  ...).r....r.....
+00003370: 0a6a 735f 6861 6e64 6c65 724e 2901 da05  .js_handlerN)...
+00003380: 636f 6d62 6f72 9000 0000 7226 0100 0046  combor....r&...F
+00003390: 7256 0000 00da 0e74 6f6f 6c62 6172 4163  rV.....toolbarAc
+000033a0: 7469 6f6e 7329 17da 1167 6574 5f6c 6179  tions)...get_lay
+000033b0: 6f75 745f 6861 6e64 656c 726d 0000 00da  out_handelrm....
+000033c0: 0b77 696e 646f 775f 7479 7065 720c 0000  .window_typer...
+000033d0: 00da 1555 524c 5f50 4152 414d 5f41 4354  ...URL_PARAM_ACT
+000033e0: 494f 4e5f 4e41 4d45 724e 0000 0072 7800  ION_NAMErN...rx.
+000033f0: 0000 72ac 0000 0072 8800 0000 7272 0000  ..r....r....rr..
+00003400: 0072 9900 0000 da13 6765 745f 746f 6f6c  .r......get_tool
+00003410: 6261 725f 6163 7469 6f6e 7372 2900 0000  bar_actionsr)...
+00003420: 72b3 0000 0072 2501 0000 7230 0000 00da  r....r%...r0....
+00003430: 0b63 6f6d 626f 5f67 726f 7570 da06 6170  .combo_group..ap
+00003440: 7065 6e64 da06 686f 746b 6579 da04 7661  pend..hotkey..va
+00003450: 7273 7283 0000 0072 3100 0000 72e6 0000  rsr....r1...r...
+00003460: 0029 1172 4000 0000 da0c 6163 7469 6f6e  .).r@.....action
+00003470: 735f 6c69 7374 72a7 0000 00da 0768 6f74  s_listr......hot
+00003480: 6b65 7973 7290 0000 00da 026c 68da 1161  keysr......lh..a
+00003490: 6374 696f 6e5f 6465 7363 7269 7074 6f72  ction_descriptor
+000034a0: da04 7462 6173 da09 636f 6d62 6f5f 6d61  ..tbas..combo_ma
+000034b0: 7072 5000 0000 da03 7462 6172 b300 0000  prP.....tbar....
+000034c0: 7225 0100 0072 2c01 0000 7226 0100 0072  r%...r,...r&...r
+000034d0: 2e01 0000 7235 0000 0072 3700 0000 7237  ....r5...r7...r7
+000034e0: 0000 0072 3800 0000 da0c 6163 7469 6f6e  ...r8.....action
+000034f0: 7332 6a73 6f6e 0502 0000 7368 0000 0004  s2json....sh....
+00003500: 0404 0108 0208 010c 010e 0204 0110 0108  ................
+00003510: 0104 0106 0106 0208 0108 ff0e 0308 010c  ................
+00003520: 0108 0104 0108 0110 0108 020c 0208 0108  ................
+00003530: 0210 010a 020a 010c 010a 0208 020c 010a  ................
+00003540: 010c 0108 010a 0102 8004 0210 010c 0114  ................
+00003550: 0102 8008 020a 0208 020c 010a 010c 0108  ................
+00003560: 010a 0102 8008 027a 1552 656e 6465 7265  .......z.Rendere
+00003570: 722e 6163 7469 6f6e 7332 6a73 6f6e 6302  r.actions2jsonc.
+00003580: 0000 0000 0000 0000 0000 0005 0000 0005  ................
+00003590: 0000 0043 0000 0073 5800 0000 6700 7d02  ...C...sX...g.}.
+000035a0: 6400 7d03 7c01 4400 5d14 7d04 7c04 6401  d.}.|.D.].}.|.d.
+000035b0: 1900 6400 7500 7213 7c04 6402 1900 7d03  ..d.u.r.|.d...}.
+000035c0: 7106 7c02 a000 7401 7c04 8301 a101 0100  q.|...t.|.......
+000035d0: 7106 7402 7c02 6403 6404 8400 6405 8d02  q.t.|.d.d...d...
+000035e0: 7d02 7c02 a000 6400 7c03 6702 a101 0100  }.|...d.|.g.....
+000035f0: 7c02 5300 2906 4e72 0100 0000 722d 0000  |.S.).Nr....r-..
+00003600: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+00003610: 0000 0200 0000 5300 0000 7308 0000 007c  ......S...s....|
+00003620: 0064 0119 0053 0029 024e 7201 0000 0072  .d...S.).Nr....r
+00003630: 3700 0000 2901 7236 0000 0072 3700 0000  7...).r6...r7...
+00003640: 7237 0000 0072 3800 0000 da08 3c6c 616d  r7...r8.....<lam
+00003650: 6264 613e 5102 0000 7302 0000 0008 007a  bda>Q...s......z
+00003660: 2c52 656e 6465 7265 722e 6469 7370 6c61  ,Renderer.displa
+00003670: 795f 6d6f 6465 326a 736f 6e2e 3c6c 6f63  y_mode2json.<loc
+00003680: 616c 733e 2e3c 6c61 6d62 6461 3ea9 0172  als>.<lambda>..r
+00003690: 3400 0000 2903 722d 0100 0072 7900 0000  4...).r-...ry...
+000036a0: da06 736f 7274 6564 2905 7240 0000 00da  ..sorted).r@....
+000036b0: 0c64 6973 706c 6179 5f6d 6f64 65da 0364  .display_mode..d
+000036c0: 6d73 da03 646d 6472 9300 0000 7237 0000  ms..dmdr....r7..
+000036d0: 0072 3700 0000 7238 0000 00da 1164 6973  .r7...r8.....dis
+000036e0: 706c 6179 5f6d 6f64 6532 6a73 6f6e 4902  play_mode2jsonI.
+000036f0: 0000 7312 0000 0004 0104 0108 010c 010a  ..s.............
+00003700: 0110 0210 010e 0104 017a 1a52 656e 6465  .........z.Rende
+00003710: 7265 722e 6469 7370 6c61 795f 6d6f 6465  rer.display_mode
+00003720: 326a 736f 6e63 0200 0000 0000 0000 0000  2jsonc..........
+00003730: 0000 1100 0000 0800 0000 4300 0000 7322  ..........C...s"
+00003740: 0300 0074 007c 0183 0172 0974 017c 0174  ...t.|...r.t.|.t
+00003750: 0283 0273 0b4a 0082 017c 00a0 037c 016a  ...s.J...|...|.j
+00003760: 04a1 015c 027d 027d 0374 057c 016a 067c  ...\.}.}.t.|.j.|
+00003770: 027c 01a0 07a1 0074 087c 016a 0983 017c  .|.....t.|.j...|
+00003780: 01a0 0a74 0b83 00a1 010c 0064 018d 057d  ...t.......d...}
+00003790: 0474 0c7c 0383 0172 317c 046a 0d7c 0364  .t.|...r1|.j.|.d
+000037a0: 028d 0101 007c 01a0 0ea1 007d 057c 056a  .....|.....}.|.j
+000037b0: 0f64 0075 0072 4374 106a 116a 12a0 1364  .d.u.rCt.j.j...d
+000037c0: 037c 01a1 0201 006e 5d74 147c 0564 0483  .|.....n]t.|.d..
+000037d0: 0272 9767 007d 0664 057d 077c 05a0 15a1  .r.g.}.d.}.|....
+000037e0: 007d 087c 0844 005d 407d 097c 00a0 167c  .}.|.D.]@}.|...|
+000037f0: 09a1 017d 0a7c 0a6a 0d74 177c 056a 0f6a  ...}.|.j.t.|.j.j
+00003800: 187c 096a 196a 1a64 0664 0784 0064 088d  .|.j.j.d.d...d..
+00003810: 037c 0717 0064 098d 0101 0074 1b7c 0974  .|...d.....t.|.t
+00003820: 1c83 0272 8474 1b7c 0974 1d83 0273 847c  ...r.t.|.t...s.|
+00003830: 0a6a 0d7c 0a64 0a19 0064 0b17 0064 0c8d  .j.|.d...d...d..
+00003840: 0101 007c 0764 0b37 007d 0774 1b7c 0974  ...|.d.7.}.t.|.t
+00003850: 1e83 0272 8d7c 0764 0d37 007d 077c 06a0  ...r.|.d.7.}.|..
+00003860: 1f7c 0aa1 0101 0071 527c 067c 0464 0e3c  .|.....qR|.|.d.<
+00003870: 007c 04a0 0d74 207c 056a 0f64 0f83 02a1  .|...t |.j.d....
+00003880: 0101 007c 04a0 0d74 207c 0164 1083 02a1  ...|...t |.d....
+00003890: 0101 0074 147c 016a 2164 1183 0272 b47c  ...t.|.j!d...r.|
+000038a0: 046a 0d64 1264 138d 0101 0074 007c 016a  .j.d.d.....t.|.j
+000038b0: 2183 0172 c574 017c 016a 2174 2283 0272  !..r.t.|.j!t"..r
+000038c0: c57c 046a 0d64 1264 148d 0101 007c 016a  .|.j.d.d.....|.j
+000038d0: 2364 0075 0172 d27c 00a0 247c 016a 23a1  #d.u.r.|..$|.j#.
+000038e0: 017c 0464 153c 007c 016a 2564 0075 0172  .|.d.<.|.j%d.u.r
+000038f0: e77c 016a 25a0 26a1 007d 0b7c 0b64 0075  .|.j%.&..}.|.d.u
+00003900: 0172 e77c 046a 0d7c 0b6a 2764 168d 0101  .r.|.j.|.j'd....
+00003910: 007c 016a 2872 f37c 046a 0d74 297c 016a  .|.j(r.|.j.t)|.j
+00003920: 2883 0164 178d 0101 0074 2a7c 0164 1864  (..d.....t*|.d.d
+00003930: 0083 037d 0c7c 0c64 0075 0190 0172 057c  ...}.|.d.u...r.|
+00003940: 046a 0d7c 0c6a 2764 198d 0101 0074 2a7c  .j.|.j'd.....t*|
+00003950: 0164 1a64 0083 037d 0d7c 0d64 0075 0190  .d.d...}.|.d.u..
+00003960: 0172 177c 046a 0d7c 0d6a 2764 1b8d 0101  .r.|.j.|.j'd....
+00003970: 0074 2a7c 016a 2164 1c69 0083 037d 0e7c  .t*|.j!d.i...}.|
+00003980: 0e90 0172 2e7c 046a 0d64 1d64 1e84 007c  ...r.|.j.d.d...|
+00003990: 0ea0 2ba1 0044 0083 0164 1f8d 0101 0074  ..+..D...d.....t
+000039a0: 106a 11a0 2c64 20a1 0190 0172 5174 2a7c  .j..,d ....rQt*|
+000039b0: 0164 2164 0083 0364 0075 0190 0172 5174  .d!d...d.u...rQt
+000039c0: 147c 016a 2164 2283 0290 0172 517c 046a  .|.j!d"....rQ|.j
+000039d0: 0d74 2d6a 2ea0 2f7c 016a 21a1 016a 3064  .t-j../|.j!..j0d
+000039e0: 238d 0101 0064 2444 005d 177d 0f74 2a7c  #....d$D.].}.t*|
+000039f0: 017c 0f64 0083 037d 107c 1064 0075 0190  .|.d...}.|.d.u..
+00003a00: 0172 697c 04a0 0d7c 0f7c 106a 316a 3269  .ri|...|.|.j1j2i
+00003a10: 01a1 0101 0090 0171 537c 016a 3364 0075  .......qS|.j3d.u
+00003a20: 0190 0172 8f7c 046a 0d7c 016a 336a 2764  ...r.|.j.|.j3j'd
+00003a30: 2564 2684 007c 016a 336a 346a 3544 0083  %d&..|.j3j4j5D..
+00003a40: 0164 278d 0201 0074 147c 0164 2883 0290  .d'....t.|.d(...
+00003a50: 0172 8f7c 046a 0d7c 016a 3664 298d 0101  .r.|.j.|.j6d)...
+00003a60: 007c 0453 0029 2a4e 2905 da02 6964 7230  .|.S.)*N)...idr0
+00003a70: 0100 0072 9600 0000 da05 736c 6176 65da  ...r......slave.
+00003a80: 0865 6469 7461 626c 6529 0172 3101 0000  .editable).r1...
+00003a90: 7a0f 2573 2068 6173 206e 6f20 7374 6f72  z.%s has no stor
+00003aa0: 65da 0b67 6574 5f63 6f6c 756d 6e73 7201  e..get_columnsr.
+00003ab0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00003ac0: 0100 0000 0100 0000 5300 0000 7306 0000  ........S...s...
+00003ad0: 007c 006a 0053 0072 3b00 0000 a901 7253  .|.j.S.r;.....rS
+00003ae0: 0000 00a9 0172 8d00 0000 7237 0000 0072  .....r....r7...r
+00003af0: 3700 0000 7238 0000 0072 3801 0000 6e02  7...r8...r8...n.
+00003b00: 0000 7302 0000 0006 007a 2552 656e 6465  ..s......z%Rende
+00003b10: 7265 722e 6163 746f 7232 6a73 6f6e 2e3c  rer.actor2json.<
+00003b20: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
+00003b30: 7239 0100 0029 01da 0c66 6965 6c64 735f  r9...)...fields_
+00003b40: 696e 6465 7872 4501 0000 722d 0000 0029  indexrE...r-...)
+00003b50: 01da 1366 6965 6c64 735f 696e 6465 785f  ...fields_index_
+00003b60: 6869 6464 656e e902 0000 00da 0363 6f6c  hidden.......col
+00003b70: da08 706b 5f69 6e64 6578 7ad0 7072 6576  ..pk_indexz.prev
+00003b80: 6965 775f 6c69 6d69 7420 7573 655f 6465  iew_limit use_de
+00003b90: 7461 696c 5f70 6172 616d 5f70 616e 656c  tail_param_panel
+00003ba0: 2075 7365 5f64 6574 6169 6c5f 7061 7261   use_detail_para
+00003bb0: 6d73 5f76 616c 7565 2068 6964 655f 6e61  ms_value hide_na
+00003bc0: 7669 6761 746f 7220 7573 655f 6465 7461  vigator use_deta
+00003bd0: 696c 5f70 6172 616d 735f 7661 6c75 6520  il_params_value 
+00003be0: 7265 6163 745f 7265 7370 6f6e 7369 7665  react_responsive
+00003bf0: 206d 6178 5f72 656e 6465 725f 6465 7074   max_render_dept
+00003c00: 6820 7369 6d70 6c65 5f73 6c61 7665 6772  h simple_slavegr
+00003c10: 6964 5f68 6561 6465 7220 7061 6769 6e61  id_header pagina
+00003c20: 746f 725f 7465 6d70 6c61 7465 2068 6964  tor_template hid
+00003c30: 655f 746f 705f 746f 6f6c 6261 7220 6869  e_top_toolbar hi
+00003c40: 6465 5f69 665f 656d 7074 7920 da04 6669  de_if_empty ..fi
+00003c50: 6c65 5429 01da 0d63 6f6e 7461 696e 5f6d  leT)...contain_m
+00003c60: 6564 6961 2901 da09 6564 6974 5f73 6166  edia)...edit_saf
+00003c70: 6572 3b01 0000 7224 0100 0029 01da 0d61  er;...r$...)...a
+00003c80: 6374 6976 655f 6669 656c 6473 da0b 6361  ctive_fields..ca
+00003c90: 7264 5f6c 6179 6f75 7429 0172 4e01 0000  rd_layout).rN...
+00003ca0: da0b 6c69 7374 5f6c 6179 6f75 7429 0172  ..list_layout).r
+00003cb0: 4f01 0000 da0e 5f63 686f 6f73 6572 735f  O....._choosers_
+00003cc0: 6469 6374 6301 0000 0000 0000 0000 0000  dictc...........
+00003cd0: 0003 0000 0005 0000 0053 0000 0073 2200  .........S...s".
+00003ce0: 0000 6900 7c00 5d0d 5c02 7d01 7d02 7c01  ..i.|.].\.}.}.|.
+00003cf0: 6400 6401 8400 7c02 6a00 4400 8301 9302  d.d...|.j.D.....
+00003d00: 7102 5300 2902 6301 0000 0000 0000 0000  q.S.).c.........
+00003d10: 0000 0002 0000 0003 0000 0053 0000 00f3  ...........S....
+00003d20: 1200 0000 6700 7c00 5d05 7d01 7c01 6a00  ....g.|.].}.|.j.
+00003d30: 9102 7102 5300 7237 0000 0072 4301 0000  ..q.S.r7...rC...
+00003d40: 2902 7247 0000 00da 0263 6672 3700 0000  ).rG.....cfr7...
+00003d50: 7237 0000 0072 3800 0000 7249 0000 00a7  r7...r8...rI....
+00003d60: 0200 00f3 0200 0000 1200 7a32 5265 6e64  ..........z2Rend
+00003d70: 6572 6572 2e61 6374 6f72 326a 736f 6e2e  erer.actor2json.
+00003d80: 3c6c 6f63 616c 733e 2e3c 6469 6374 636f  <locals>.<dictco
+00003d90: 6d70 3e2e 3c6c 6973 7463 6f6d 703e 2901  mp>.<listcomp>).
+00003da0: da0e 636f 6e74 6578 745f 6669 656c 6473  ..context_fields
+00003db0: 2903 7247 0000 00da 0266 6e72 4800 0000  ).rG.....fnrH...
+00003dc0: 7237 0000 0072 3700 0000 7238 0000 0072  r7...r7...r8...r
+00003dd0: 4d00 0000 a702 0000 7306 0000 0006 0006  M.......s.......
+00003de0: 0116 ff7a 2752 656e 6465 7265 722e 6163  ...z'Renderer.ac
+00003df0: 746f 7232 6a73 6f6e 2e3c 6c6f 6361 6c73  tor2json.<locals
+00003e00: 3e2e 3c64 6963 7463 6f6d 703e 2901 da0c  >.<dictcomp>)...
+00003e10: 6368 6f6f 7365 725f 6469 6374 da0c 636f  chooser_dict..co
+00003e20: 6e74 656e 7474 7970 6573 da05 6d6f 6465  ntenttypes..mode
+00003e30: 6cda 055f 6d65 7461 2901 da0c 636f 6e74  l.._meta)...cont
+00003e40: 656e 745f 7479 7065 2903 da0d 6465 7461  ent_type)...deta
+00003e50: 696c 5f61 6374 696f 6eda 0d69 6e73 6572  il_action..inser
+00003e60: 745f 6163 7469 6f6e da0e 6465 6661 756c  t_action..defaul
+00003e70: 745f 6163 7469 6f6e 6301 0000 0000 0000  t_actionc.......
+00003e80: 0000 0000 0002 0000 0003 0000 0053 0000  .............S..
+00003e90: 0072 5101 0000 7237 0000 0072 4301 0000  .rQ...r7...rC...
+00003ea0: 2902 7247 0000 0072 8d00 0000 7237 0000  ).rG...r....r7..
+00003eb0: 0072 3700 0000 7238 0000 0072 4900 0000  .r7...r8...rI...
+00003ec0: b702 0000 7253 0100 007a 2752 656e 6465  ....rS...z'Rende
+00003ed0: 7265 722e 6163 746f 7232 6a73 6f6e 2e3c  rer.actor2json.<
+00003ee0: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00003ef0: 703e 2902 da0d 7061 7261 6d73 5f6c 6179  p>)...params_lay
+00003f00: 6f75 74da 0d70 6172 616d 735f 6669 656c  out..params_fiel
+00003f10: 6473 da10 7061 7261 6d73 5f70 616e 656c  ds..params_panel
+00003f20: 5f70 6f73 2901 7260 0100 0029 3772 2c00  _pos).r`...)7r,.
+00003f30: 0000 72b5 0000 0072 1b00 0000 7237 0100  ..r....r....r7..
+00003f40: 00da 0d5f 6163 7469 6f6e 735f 6c69 7374  ..._actions_list
+00003f50: 7272 0000 0072 f000 0000 da0f 6765 745f  rr...r......get_
+00003f60: 6163 746f 725f 6c61 6265 6cda 0462 6f6f  actor_label..boo
+00003f70: 6cda 066d 6173 7465 72da 0c68 6964 655f  l..master..hide_
+00003f80: 6564 6974 696e 6772 2900 0000 72d2 0000  editingr)...r...
+00003f90: 0072 7800 0000 da0a 6765 745f 6861 6e64  .rx.....get_hand
+00003fa0: 6c65 da05 7374 6f72 6572 0400 0000 7270  le..storer....rp
+00003fb0: 0000 00da 066c 6f67 6765 72da 0777 6172  .....logger..war
+00003fc0: 6e69 6e67 7283 0000 0072 4201 0000 72ab  ningr....rB...r.
+00003fd0: 0000 0072 3900 0000 da0b 6c69 7374 5f66  ...r9.....list_f
+00003fe0: 6965 6c64 7372 b700 0000 7253 0000 0072  ieldsr....rS...r
+00003ff0: a100 0000 721f 0000 0072 2000 0000 7222  ....r....r ...r"
+00004000: 0000 0072 2d01 0000 7228 0000 0072 5801  ...r-...r(...rX.
+00004010: 0000 722b 0000 0072 3b01 0000 723e 0100  ..r+...r;...r>..
+00004020: 0072 5b01 0000 da11 6765 745f 7769 6e64  .r[.....get_wind
+00004030: 6f77 5f6c 6179 6f75 7472 8800 0000 724d  ow_layoutr....rM
+00004040: 0100 0072 7900 0000 7202 0100 0072 6900  ...ry...r....ri.
+00004050: 0000 7277 0000 0072 0e00 0000 da07 6f62  ..rw...r......ob
+00004060: 6a65 6374 73da 0d67 6574 5f66 6f72 5f6d  jects..get_for_m
+00004070: 6f64 656c 72d9 0000 0072 6d00 0000 724e  odelr....rm...rN
+00004080: 0000 0072 5e01 0000 da0c 7061 7261 6d73  ...r^.....params
+00004090: 5f73 746f 7265 da0c 7061 7261 6d5f 6669  _store..param_fi
+000040a0: 656c 6473 7260 0100 0029 1172 4000 0000  eldsr`...).r@...
+000040b0: 72a6 0000 00da 0261 6cda 0268 6b72 a700  r......al..hkr..
+000040c0: 0000 da02 6168 da07 636f 6c75 6d6e 73da  ....ah..columns.
+000040d0: 0969 6e64 6578 5f6d 6f64 da09 636f 6c5f  .index_mod..col_
+000040e0: 656c 656d 7372 4801 0000 720c 0100 00da  elemsrH...r.....
+000040f0: 0277 6c72 4e01 0000 724f 0100 0072 5601  .wlrN...rO...rV.
+00004100: 0000 72b8 0000 0072 9000 0000 7237 0000  ..r....r....r7..
+00004110: 0072 3700 0000 7238 0000 00da 0a61 6374  .r7...r8.....act
+00004120: 6f72 326a 736f 6e55 0200 0073 9200 0000  or2jsonU...s....
+00004130: 1601 1001 0601 0201 0601 0801 0c01 06fc  ................
+00004140: 0807 0c01 0802 0a01 1201 0a03 0401 0401  ................
+00004150: 0801 0801 0a01 1201 0601 04ff 0201 08ff  ................
+00004160: 1402 1403 0801 0a01 0801 0c01 0801 1205  ................
+00004170: 1001 0c0d 0c01 1602 0c01 0a02 1001 0a02  ................
+00004180: 0a01 0801 0e01 0602 1201 0c02 0a01 0e01  ................
+00004190: 0c02 0a01 0e02 0e03 0601 0a01 0601 0aff  ................
+000041a0: 2603 0201 06ff 1803 0801 0c01 0a01 1201  &...............
+000041b0: 0480 0c02 0402 0601 1201 06fe 0c04 0e01  ................
+000041c0: 0401 7a13 5265 6e64 6572 6572 2e61 6374  ..z.Renderer.act
+000041d0: 6f72 326a 736f 6e63 0200 0000 0000 0000  or2jsonc........
+000041e0: 0000 0000 0400 0000 0600 0000 0300 0000  ................
+000041f0: 7364 0000 0064 0188 015f 0088 016a 0144  sd...d..._...j.D
+00004200: 005d 2289 0088 006a 0264 0075 0172 0e71  .]"....j.d.u.r.q
+00004210: 0674 036a 046a 0588 01a0 0688 006a 07a1  .t.j.j.......j..
+00004220: 018e 007d 0287 0087 0166 0264 0264 0384  ...}.....f.d.d..
+00004230: 087d 0374 086a 096a 0aa0 0b7c 027c 037c  .}.t.j.j...|.|.|
+00004240: 01a1 0301 0071 0664 0488 015f 0074 0c83  .....q.d..._.t..
+00004250: 00a0 0d7c 01a1 0153 0029 054e 5463 0100  ...|...S.).NTc..
+00004260: 0000 0000 0000 0000 0000 0100 0000 0600  ................
+00004270: 0000 1300 0000 7318 0000 007c 00a0 0074  ......s....|...t
+00004280: 0188 01a0 0288 00a1 0183 01a1 0101 0064  ...............d
+00004290: 0053 0072 3b00 0000 2903 728c 0000 0072  .S.r;...).r....r
+000042a0: 2600 0000 7277 0100 0072 4401 0000 a902  &...rw...rD.....
+000042b0: 7299 0000 0072 4000 0000 7237 0000 0072  r....r@...r7...r
+000042c0: 3800 0000 728c 0000 00c6 0200 0073 0200  8...r........s..
+000042d0: 0000 1801 7a26 5265 6e64 6572 6572 2e62  ....z&Renderer.b
+000042e0: 7569 6c64 5f6a 735f 6361 6368 652e 3c6c  uild_js_cache.<l
+000042f0: 6f63 616c 733e 2e77 7269 7465 4629 0e72  ocals>.writeF).r
+00004300: 6f00 0000 726b 0000 00da 0f67 6574 5f68  o...rk.....get_h
+00004310: 616e 646c 655f 6e61 6d65 727e 0000 00da  andle_namer~....
+00004320: 0470 6174 68da 046a 6f69 6e72 2301 0000  .path..joinr#...
+00004330: 72f0 0000 0072 0400 0000 7270 0000 0072  r....r....rp...r
+00004340: 2300 0000 da0f 6d61 6b65 5f63 6163 6865  #.....make_cache
+00004350: 5f66 696c 6572 3c00 0000 da0e 6275 696c  _filer<.....buil
+00004360: 645f 6a73 5f63 6163 6865 2904 7240 0000  d_js_cache).r@..
+00004370: 00da 0566 6f72 6365 7255 0100 0072 8c00  ...forcerU...r..
+00004380: 0000 7242 0000 0072 7801 0000 7238 0000  ..rB...rx...r8..
+00004390: 0072 7d01 0000 bd02 0000 7312 0000 0006  .r}.......s.....
+000043a0: 020a 020a 0102 0114 010e 0214 0306 020c  ................
+000043b0: 017a 1752 656e 6465 7265 722e 6275 696c  .z.Renderer.buil
+000043c0: 645f 6a73 5f63 6163 6865 723b 0000 0029  d_js_cacher;...)
+000043d0: 2072 b400 0000 da0a 5f5f 6d6f 6475 6c65   r......__module
+000043e0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+000043f0: da07 5f5f 646f 635f 5fda 0e69 735f 696e  ..__doc__..is_in
+00004400: 7465 7261 6374 6976 65da 0863 616e 5f61  teractive..can_a
+00004410: 7574 6872 1e01 0000 7222 0100 00da 1873  uthr....r".....s
+00004420: 7570 706f 7274 5f64 6173 6862 6f61 7264  upport_dashboard
+00004430: 5f6c 6179 6f75 7472 3d00 0000 7294 0000  _layoutr=...r...
+00004440: 0072 4f00 0000 7287 0000 0072 ab00 0000  .rO...r....r....
+00004450: 72b9 0000 0072 cf00 0000 72dc 0000 0072  r....r....r....r
+00004460: e300 0000 72a5 0000 0072 df00 0000 723f  ....r....r....r?
+00004470: 0000 0072 fe00 0000 72ff 0000 0072 0001  ...r....r....r..
+00004480: 0000 7214 0100 0072 1a01 0000 7223 0100  ..r....r....r#..
+00004490: 0072 3701 0000 723e 0100 0072 7701 0000  .r7...r>...rw...
+000044a0: 727d 0100 00da 0d5f 5f63 6c61 7373 6365  r}.....__classce
+000044b0: 6c6c 5f5f 7237 0000 0072 3700 0000 7242  ll__r7...r7...rB
+000044c0: 0000 0072 3800 0000 723a 0000 003b 0000  ...r8...r:...;..
+000044d0: 0073 3c00 0000 0800 0401 0403 0401 0402  .s<.............
+000044e0: 0401 0401 0c02 0804 0855 081d 0808 081f  .........U......
+000044f0: 0803 0a18 0212 0aff 0815 080e 0821 084e  .............!.N
+00004500: 080e 080a 082a 0809 080f 080a 0844 080c  .....*.......D..
+00004510: 1468 723a 0000 0072 3b00 0000 2948 727e  .hr:...r;...)Hr~
+00004520: 0000 00da 0770 6174 686c 6962 7202 0000  .....pathlibr...
+00004530: 00da 0468 746d 6c72 0300 0000 da0b 646a  ...htmlr......dj
+00004540: 616e 676f 2e63 6f6e 6672 0400 0000 da09  ango.confr......
+00004550: 646a 616e 676f 2e64 6272 0500 0000 da11  django.dbr......
+00004560: 646a 616e 676f 2e75 7469 6c73 2e74 6578  django.utils.tex
+00004570: 7472 0600 0000 da0c 646a 616e 676f 2e75  tr......django.u
+00004580: 7469 6c73 7207 0000 00da 126c 696e 6f2e  tilsr......lino.
+00004590: 636f 7265 2e72 656e 6465 7265 7272 0800  core.rendererr..
+000045a0: 0000 7209 0000 00da 0f6c 696e 6f2e 636f  ..r......lino.co
+000045b0: 7265 2e6d 656e 7573 720a 0000 0072 0b00  re.menusr....r..
+000045c0: 0000 da09 6c69 6e6f 2e63 6f72 6572 0c00  ....lino.corer..
+000045d0: 0000 720d 0000 00da 0e6c 696e 6f2e 636f  ..r......lino.co
+000045e0: 7265 2e67 666b 7372 0e00 0000 da1e 6c69  re.gfksr......li
+000045f0: 6e6f 2e6d 6f64 6c69 622e 6578 746a 732e  no.modlib.extjs.
+00004600: 6578 745f 7265 6e64 6572 6572 720f 0000  ext_rendererr...
+00004610: 00da 116c 696e 6f2e 636f 7265 2e61 6374  ...lino.core.act
+00004620: 696f 6e73 7210 0000 0072 1100 0000 7212  ionsr....r....r.
+00004630: 0000 0072 1300 0000 7214 0000 0072 1500  ...r....r....r..
+00004640: 0000 7216 0000 0072 1700 0000 da15 6c69  ..r....r......li
+00004650: 6e6f 2e63 6f72 652e 626f 756e 6461 6374  no.core.boundact
+00004660: 696f 6e72 1800 0000 da15 6c69 6e6f 2e63  ionr......lino.c
+00004670: 6f72 652e 6368 6f69 6365 6c69 7374 7372  ore.choicelistsr
+00004680: 1900 0000 da1e 6c69 6e6f 2e6d 6f64 6c69  ......lino.modli
+00004690: 622e 7379 7374 656d 2e63 686f 6963 656c  b.system.choicel
+000046a0: 6973 7473 721a 0000 00da 106c 696e 6f2e  istsr......lino.
+000046b0: 636f 7265 2e61 6374 6f72 7372 1b00 0000  core.actorsr....
+000046c0: da11 6c69 6e6f 2e63 6f72 652e 6c61 796f  ..lino.core.layo
+000046d0: 7574 7372 1c00 0000 721d 0000 00da 0f6c  utsr....r......l
+000046e0: 696e 6f2e 636f 7265 2e65 6c65 6d73 721e  ino.core.elemsr.
+000046f0: 0000 0072 1f00 0000 7220 0000 0072 2100  ...r....r ...r!.
+00004700: 0000 7222 0000 0072 2300 0000 da0a 6574  ..r"...r#.....et
+00004710: 6765 6e2e 6874 6d6c 7224 0000 00da 0a6c  gen.htmlr$.....l
+00004720: 696e 6f2e 7574 696c 7372 2500 0000 da10  ino.utilsr%.....
+00004730: 6c69 6e6f 2e75 7469 6c73 2e6a 7367 656e  lino.utils.jsgen
+00004740: 7226 0000 0072 2700 0000 7228 0000 00da  r&...r'...r(....
+00004750: 176c 696e 6f2e 6d6f 646c 6962 2e75 7365  .lino.modlib.use
+00004760: 7273 2e75 7469 6c73 7229 0000 0072 2a00  rs.utilsr)...r*.
+00004770: 0000 da19 6c69 6e6f 2e6d 6f64 6c69 622e  ....lino.modlib.
+00004780: 7379 7374 656d 2e6d 6978 696e 7372 2b00  system.mixinsr+.
+00004790: 0000 da07 696e 7370 6563 7472 2c00 0000  ....inspectr,...
+000047a0: da05 6963 6f6e 7372 2e00 0000 7239 0000  ..iconsr....r9..
+000047b0: 0072 3a00 0000 7237 0000 0072 3700 0000  .r:...r7...r7...
+000047c0: 7237 0000 0072 3800 0000 da08 3c6d 6f64  r7...r8.....<mod
+000047d0: 756c 653e 0100 0000 733c 0000 0008 040c  ule>....s<......
+000047e0: 010c 010c 010c 010c 010c 0110 0210 020c  ................
+000047f0: 010c 010c 010c 0128 020c 030c 010c 010c  .......(........
+00004800: 0110 011c 010c 020c 020c 0214 0110 020c  ................
+00004810: 010c 020c 020a 0314 0d                   .........
```

### Comparing `lino_react-23.6.2/lino_react/react/__pycache__/renderer.cpython-38.pyc` & `lino_react-23.7.0/lino_react/react/__pycache__/renderer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.2/lino_react/react/__pycache__/views.cpython-310.pyc` & `lino_react-23.7.0/lino_react/react/__pycache__/views.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.2/lino_react/react/__pycache__/views.cpython-38.pyc` & `lino_react-23.7.0/lino_react/react/__pycache__/views.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.2/lino_react/react/config/react/main.html` & `lino_react-23.7.0/lino_react/react/config/react/main.html`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.2/lino_react/react/config/react/service-worker.js` & `lino_react-23.7.0/lino_react/react/config/react/service-worker.js`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.2/lino_react/react/icons.py` & `lino_react-23.7.0/lino_react/react/icons.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.2/lino_react/react/renderer.py` & `lino_react-23.7.0/lino_react/react/renderer.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
 from etgen.html import E
 
 from lino.utils import jsgen
 from lino.utils.jsgen import py2js, js_code, obj2dict
 
 from lino.modlib.users.utils import get_user_profile, with_user_profile
+from lino.modlib.system.mixins import EditSafe
 
 from inspect import isclass
 
 from .icons import REACT_ICON_MAPPING
 
 
 def find(itter, target, key=None):
@@ -645,14 +646,17 @@
                                   "hide_top_toolbar "
                                   "hide_if_empty "
                                ))
 
         if hasattr(v.model, "file"):
             result.update(contain_media=True)
 
+        if isclass(v.model) and issubclass(v.model, EditSafe):
+            result.update(edit_safe=True)
+
         if v.display_mode is not None:
             result['display_mode'] = self.display_mode2json(v.display_mode)
 
         if v.detail_action is not None:
             wl = v.detail_action.get_window_layout()
             if wl is not None:
                 result.update(window_layout=wl._formpanel_name)
```

### Comparing `lino_react-23.6.2/lino_react/react/static/media/color.6441e63a.png` & `lino_react-23.7.0/lino_react/react/static/media/color.6441e63a.png`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.2/lino_react/react/static/media/color.c7a33805.png` & `lino_react-23.7.0/lino_react/react/static/media/color.c7a33805.png`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.2/lino_react/react/static/media/line.567f5738.gif` & `lino_react-23.7.0/lino_react/react/static/media/line.567f5738.gif`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.2/lino_react/react/static/media/primeicons.2d2afb27.eot` & `lino_react-23.7.0/lino_react/react/static/media/primeicons.2d2afb27.eot`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.2/lino_react/react/static/media/primeicons.3a0d4a58.ttf` & `lino_react-23.7.0/lino_react/react/static/media/primeicons.3a0d4a58.ttf`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.2/lino_react/react/static/media/primeicons.66ee0deb.woff` & `lino_react-23.7.0/lino_react/react/static/media/primeicons.66ee0deb.woff`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.2/lino_react/react/static/media/primeicons.c55d94a2.svg` & `lino_react-23.7.0/lino_react/react/static/media/primeicons.c55d94a2.svg`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.2/lino_react/react/static/media/primeicons.df0140f8.ttf` & `lino_react-23.7.0/lino_react/react/static/media/primeicons.df0140f8.ttf`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.2/lino_react/react/static/media/primeicons.dfbfef2d.eot` & `lino_react-23.7.0/lino_react/react/static/media/primeicons.dfbfef2d.eot`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.2/lino_react/react/static/media/primeicons.e5e0e944.svg` & `lino_react-23.7.0/lino_react/react/static/media/primeicons.e5e0e944.svg`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.2/lino_react/react/static/media/primeicons.e61f3495.woff` & `lino_react-23.7.0/lino_react/react/static/media/primeicons.e61f3495.woff`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.2/lino_react/react/static/react/main.js` & `lino_react-23.7.0/lino_react/react/static/react/main.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -696,15 +696,19 @@
                                     detail: "Record Deleted"
                                 }), rp && rp.hasOwnProperty("parent") && !rp.parent.props.router.match.isExact ? _this.router.history.goBack() : _this.router.history.go(0)), response.success && "/" === response.goto_url && response.close_window && (document.querySelector("#sign_in_submit").submit(), _this.fetch_user_settings(), _this.dashboard && _this.dashboard.reloadData()), response.close_window && (_this.data.dialogs.length ? (_this.data.dialogs.pop().onClose(), rp && rp.reload && 0 === _this.data.dialogs.length ? (console.warn("Dialog with parent as rp."), rp.reload()) : window.postMessage("refresh_ss_panel", "*"), _this.setState({
                                     loading: !1
                                 })) : _this.router.history.goBack()), response.goto_url && _this.router.history.push(response.goto_url), response.open_url && window.open(response.open_url, "foo", ""), response.message && (_this.toast.show({
                                     severity: response.alert ? response.alert.toLowerCase() : response.success ? "success" : "info",
                                     summary: response.alert || (response.success ? "Success" : "Info"),
                                     detail: response.message
-                                }), _this.data.user_state_change && (delete _this.data.user_state_change, _this.fetch_user_settings())), response.clear_site_cache && (window.localStorage.clear(), _this.fetch_user_settings(null, !1, !0)), !response.refresh && !response.refresh_all || response.record_deleted || (rp && rp.rp.includes("dashboard") && "dashboard-main" !== rp.rp && _this.rps["dashboard-main"].reload(), rp && rp.reload(), null == rp && _this.dashboard && _this.dashboard.reloadData()), response.refresh_delayed_value && window.postMessage("refresh_ss_panel", "*")
+                                }), _this.data.user_state_change && (delete _this.data.user_state_change, _this.fetch_user_settings())), response.clear_site_cache && (window.localStorage.clear(), _this.fetch_user_settings(null, !1, !0)), !response.refresh && !response.refresh_all || response.record_deleted || (rp && rp.rp.includes("dashboard") && "dashboard-main" !== rp.rp && _this.rps["dashboard-main"].reload(), rp && rp.reload(), null == rp && _this.dashboard && _this.dashboard.reloadData()), response.refresh_delayed_value && window.postMessage("refresh_ss_panel", "*"), response.hasOwnProperty("editing_mode") && rp && (rp.hasOwnProperty("parent") ? (rp.parent.data.editing_mode = response.editing_mode, rp.parent.setState({
+                                    loading: !1
+                                })) : (rp.data.editing_mode = response.editing_mode, rp.setState({
+                                    loading: !1
+                                })))
                             }, _this.searchMethod = function(e) {}, _this.create_menu = function(layout) {
                                 var miStore = [];
                                 _this.data.counter = [0];
                                 var convert = function convert(mi, store) {
                                         var menu, storeMenu = {};
                                         if (mi.text) {
                                             var id = _this.data.counter[0].toString();
@@ -2772,15 +2776,15 @@
                     disabledFields: {}
                 };
                 const __WEBPACK_DEFAULT_EXPORT__ = LinoBbar
             },
             6149: (e, t, n) => {
                 "use strict";
                 n.d(t, {
-                    Z: () => Xe
+                    Z: () => Ye
                 });
                 var o = n(3379),
                     r = n.n(o),
                     i = n(5397);
                 r()(i.Z, {
                     insert: "head",
                     singleton: !1
@@ -4809,134 +4813,122 @@
                             var n = arguments[t];
                             for (var o in n) Object.prototype.hasOwnProperty.call(n, o) && (e[o] = n[o])
                         }
                         return e
                     }, Be.apply(this, arguments)
                 }
 
-                function Fe(e, t, n, o, r, i, a) {
+                function Fe(e, t) {
+                    var n = Object.keys(e);
+                    if (Object.getOwnPropertySymbols) {
+                        var o = Object.getOwnPropertySymbols(e);
+                        t && (o = o.filter((function(t) {
+                            return Object.getOwnPropertyDescriptor(e, t).enumerable
+                        }))), n.push.apply(n, o)
+                    }
+                    return n
+                }
+
+                function ze(e, t, n) {
+                    return t in e ? Object.defineProperty(e, t, {
+                        value: n,
+                        enumerable: !0,
+                        configurable: !0,
+                        writable: !0
+                    }) : e[t] = n, e
+                }
+
+                function Ue(e, t, n, o, r, i, a) {
                     try {
                         var l = e[i](a),
                             s = l.value
                     } catch (e) {
                         return void n(e)
                     }
                     l.done ? t(s) : Promise.resolve(s).then(o, r)
                 }
 
-                function ze(e) {
+                function Ke(e) {
                     return function() {
                         var t = this,
                             n = arguments;
                         return new Promise((function(o, r) {
                             var i = e.apply(t, n);
 
                             function a(e) {
-                                Fe(i, o, r, a, l, "next", e)
+                                Ue(i, o, r, a, l, "next", e)
                             }
 
                             function l(e) {
-                                Fe(i, o, r, a, l, "throw", e)
+                                Ue(i, o, r, a, l, "throw", e)
                             }
                             a(void 0)
                         }))
                     }
                 }
 
-                function Ue(e, t) {
-                    var n = Object.keys(e);
-                    if (Object.getOwnPropertySymbols) {
-                        var o = Object.getOwnPropertySymbols(e);
-                        t && (o = o.filter((function(t) {
-                            return Object.getOwnPropertyDescriptor(e, t).enumerable
-                        }))), n.push.apply(n, o)
-                    }
-                    return n
-                }
-
-                function Ke(e) {
-                    for (var t = 1; t < arguments.length; t++) {
-                        var n = null != arguments[t] ? arguments[t] : {};
-                        t % 2 ? Ue(Object(n), !0).forEach((function(t) {
-                            He(e, t, n[t])
-                        })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Ue(Object(n)).forEach((function(t) {
-                            Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
-                        }))
-                    }
-                    return e
-                }
-
-                function He(e, t, n) {
-                    return t in e ? Object.defineProperty(e, t, {
-                        value: n,
-                        enumerable: !0,
-                        configurable: !0,
-                        writable: !0
-                    }) : e[t] = n, e
-                }
-
-                function We(e, t) {
+                function He(e, t) {
                     for (var n = 0; n < t.length; n++) {
                         var o = t[n];
                         o.enumerable = o.enumerable || !1, o.configurable = !0, "value" in o && (o.writable = !0), Object.defineProperty(e, o.key, o)
                     }
                 }
 
-                function Ve(e, t) {
-                    return Ve = Object.setPrototypeOf || function(e, t) {
+                function We(e, t) {
+                    return We = Object.setPrototypeOf || function(e, t) {
                         return e.__proto__ = t, e
-                    }, Ve(e, t)
+                    }, We(e, t)
                 }
 
-                function Ge(e, t) {
+                function Ve(e, t) {
                     if (t && ("object" === Ne(t) || "function" == typeof t)) return t;
                     if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
-                    return Ze(e)
+                    return Ge(e)
                 }
 
-                function Ze(e) {
+                function Ge(e) {
                     if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                     return e
                 }
 
-                function Ye(e) {
-                    return Ye = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
+                function Ze(e) {
+                    return Ze = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
                         return e.__proto__ || Object.getPrototypeOf(e)
-                    }, Ye(e)
+                    }, Ze(e)
                 }
-                var Xe = function(e) {
+                var Ye = function(e) {
                     ! function(e, t) {
                         if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
                         Object.defineProperty(e, "prototype", {
                             value: Object.create(t && t.prototype, {
                                 constructor: {
                                     value: e,
                                     writable: !0,
                                     configurable: !0
                                 }
                             }),
                             writable: !1
-                        }), t && Ve(e, t)
+                        }), t && We(e, t)
                     }(d, e);
                     var t, n, o, r, i, p, u = (i = d, p = function() {
                         if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
                         if (Reflect.construct.sham) return !1;
                         if ("function" == typeof Proxy) return !0;
                         try {
                             return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
                         } catch (e) {
                             return !1
                         }
                     }(), function() {
-                        var e, t = Ye(i);
+                        var e, t = Ze(i);
                         if (p) {
-                            var n = Ye(this).constructor;
+                            var n = Ze(this).constructor;
                             e = Reflect.construct(t, arguments, n)
                         } else e = t.apply(this, arguments);
-                        return Ge(this, e)
+                        return Ve(this, e)
                     });
 
                     function d(e) {
                         var t;
                         ! function(e, t) {
                             if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
                         }(this, d), t = u.call(this, e);
@@ -4982,25 +4974,25 @@
                             })),
                             sortCol: void 0,
                             sortField: void 0,
                             sortFieldName: void 0,
                             sortOrder: 0,
                             title: "",
                             topRow: 0
-                        }, t.actionWrapper = t.actionWrapper.bind(Ze(t)), t.consumeServerResponse = t.consumeServerResponse.bind(Ze(t)), t.get_current_grid_config = t.get_current_grid_config.bind(Ze(t)), t.get_full_id = t.get_full_id.bind(Ze(t)), t.getData = t.getData.bind(Ze(t)), t.getOne = t.getOne.bind(Ze(t)), t.getUri = t.getUri.bind(Ze(t)), t.handleWindowChange = (0, _.Ds)(t.handleWindowChange.bind(Ze(t)), 50), t.messageInterceptor = t.messageInterceptor.bind(Ze(t)), t.registerScroll = t.registerScroll.bind(Ze(t)), t.multiRowView = t.multiRowView.bind(Ze(t)), t.onKeyDown = t.onKeyDown.bind(Ze(t)), t.onRowDoubleClick = t.onRowDoubleClick.bind(Ze(t)), t.onSort = t.onSort.bind(Ze(t)), t.refresh = t.refresh.bind(Ze(t)), t.quickFilter = (0, _.Ds)(t.quickFilter.bind(Ze(t)), 200), t.reload = t.reload.bind(Ze(t)), t.reset = t.reset.bind(Ze(t)), t.update_params_values = t.update_params_values.bind(Ze(t)), t.updateUrlValues = t.updateUrlValues.bind(Ze(t)), t
+                        }, t.actionWrapper = t.actionWrapper.bind(Ge(t)), t.consumeServerResponse = t.consumeServerResponse.bind(Ge(t)), t.get_current_grid_config = t.get_current_grid_config.bind(Ge(t)), t.get_full_id = t.get_full_id.bind(Ge(t)), t.getData = t.getData.bind(Ge(t)), t.getOne = t.getOne.bind(Ge(t)), t.getUri = t.getUri.bind(Ge(t)), t.handleWindowChange = (0, _.Ds)(t.handleWindowChange.bind(Ge(t)), 50), t.messageInterceptor = t.messageInterceptor.bind(Ge(t)), t.registerScroll = t.registerScroll.bind(Ge(t)), t.multiRowView = t.multiRowView.bind(Ge(t)), t.onKeyDown = t.onKeyDown.bind(Ge(t)), t.onRowDoubleClick = t.onRowDoubleClick.bind(Ge(t)), t.onSort = t.onSort.bind(Ge(t)), t.refresh = t.refresh.bind(Ge(t)), t.quickFilter = (0, _.Ds)(t.quickFilter.bind(Ge(t)), 200), t.reload = t.reload.bind(Ge(t)), t.reset = t.reset.bind(Ge(t)), t.update_params_values = t.update_params_values.bind(Ge(t)), t
                     }
                     return t = d, n = [{
                         key: "get_full_id",
                         value: function() {
                             return "".concat(this.props.packId, ".").concat(this.props.actorId)
                         }
                     }, {
                         key: "componentDidMount",
                         value: function() {
-                            if (this.controller = new(m()), this.refresh(), window.addEventListener("resize", this.handleWindowChange), window.addEventListener("keydown", this.onKeyDown), window.addEventListener("message", this.messageInterceptor), this.props.parentBody) {
+                            if (console.log((0, _.VW)(this.props.router)), this.controller = new(m()), this.refresh(), window.addEventListener("resize", this.handleWindowChange), window.addEventListener("keydown", this.onKeyDown), window.addEventListener("message", this.messageInterceptor), this.props.parentBody) {
                                 window.addEventListener("scroll", this.registerScroll);
                                 var e = this.props.router.history.location.pathname,
                                     t = window.App.data.scrollIndex,
                                     n = t.indexOf(e);
                                 n >= 0 ? t.pop(n) : t.length >= 99 && (t.pop(0), delete window.App.data.scroll[e]), t.push(e)
                             }
                         }
@@ -5119,22 +5111,14 @@
                                         rp: this,
                                         status: r
                                     })
                                 }
                             } else console.warn(this.props.actorData.id + " has no attribute detail_action")
                         }
                     }, {
-                        key: "updateUrlValues",
-                        value: function(e) {
-                            var t = g.parse(this.props.router.history.location.search);
-                            Object.assign(t, Ke({}, e)), this.props.router.history.replace({
-                                search: g.stringify(t)
-                            })
-                        }
-                    }, {
                         key: "actionWrapper",
                         value: function(e) {
                             this.data.detail_window ? (this.data.taskId += 1, this.data.task = e, this.setState({
                                 loading: !1
                             })) : e()
                         }
                     }, {
@@ -5204,15 +5188,15 @@
                         key: "getUri",
                         value: function(e) {
                             var t = "api/".concat(this.props.packId, "/").concat(this.props.actorId);
                             return void 0 !== e && (t += "?".concat(g.stringify(e))), t
                         }
                     }, {
                         key: "getData",
-                        value: (r = ze(y().mark((function e(t, n, o) {
+                        value: (r = Ke(y().mark((function e(t, n, o) {
                             var r, i = this,
                                 a = arguments;
                             return y().wrap((function(e) {
                                 for (;;) switch (e.prev = e.next) {
                                     case 0:
                                         return (r = a.length > 3 && void 0 !== a[3] && a[3]) && Object.assign(this.data, {
                                             loading: !0,
@@ -5233,15 +5217,15 @@
                                 }
                             }), e, this)
                         }))), function(e, t, n) {
                             return r.apply(this, arguments)
                         })
                     }, {
                         key: "getOne",
-                        value: (o = ze(y().mark((function e(t, n, o, r) {
+                        value: (o = Ke(y().mark((function e(t, n, o, r) {
                             var i = this;
                             return y().wrap((function(e) {
                                 for (;;) switch (e.prev = e.next) {
                                     case 0:
                                         return e.next = 2, (0, b.he)("api/".concat(this.props.packId, "/").concat(this.props.actorId, "/").concat(t, "?").concat(g.stringify(n)), {
                                             signal: o
                                         }).then(window.App.handleAjaxResponse).then((function(e) {
@@ -5320,15 +5304,25 @@
                                 window_width: window.innerWidth
                             })
                         }
                     }, {
                         key: "update_params_values",
                         value: function(e, t, n) {
                             (0, _.ku)(this.data.params_values, this.props.actorData.params_fields);
-                            var o = Object.assign({}, this.data.params_values, Ke({}, e)),
+                            var o = Object.assign({}, this.data.params_values, function(e) {
+                                    for (var t = 1; t < arguments.length; t++) {
+                                        var n = null != arguments[t] ? arguments[t] : {};
+                                        t % 2 ? Fe(Object(n), !0).forEach((function(t) {
+                                            ze(e, t, n[t])
+                                        })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Fe(Object(n)).forEach((function(t) {
+                                            Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
+                                        }))
+                                    }
+                                    return e
+                                }({}, e)),
                                 r = (0, _.ku)(o, this.props.actorData.params_fields);
                             this.data.pv = r, Object.assign(this.data, {
                                 params_values: o
                             }), this.reload()
                         }
                     }, {
                         key: "get_current_grid_config",
@@ -5434,25 +5428,27 @@
                                         onSort: e.onSort,
                                         pv: e.state.pv,
                                         ref: function(t) {
                                             return e.GridElement = t
                                         },
                                         refresh: e.refresh,
                                         reload_timestamp: e.data.reload_timestamp,
+                                        router: t,
                                         rows: e.data.rows,
                                         sr: e.data.sr,
                                         show_columns: e.data.show_columns,
                                         sortField: e.data.sortField,
                                         sortOrder: e.data.sortOrder
                                     })) : [me.UZ, me.do].includes(e.state.layout) ? a.createElement("div", {
                                         dangerouslySetInnerHTML: {
                                             __html: e.data.html_text
                                         }
                                     }) : a.createElement(_e, {
-                                        parent: e
+                                        parent: e,
+                                        router: t
                                     }), !e.state.loading && a.createElement(Re, {
                                         parent: e,
                                         router: t
                                     }))
                                 }
                             }))), !this.state.loading && this.data.detail_window && a.createElement(l.AW, {
                                 path: this.state.static_page ? "".concat(this.props.router.match.path) : "".concat(this.props.router.match.path, "/:pk"),
@@ -5512,22 +5508,22 @@
                                         showPVDialog: !1
                                     })
                                 }
                             }, this.props.actorData.params_layout && this.state.showPVDialog && a.createElement(Le, {
                                 parent: this
                             })))
                         }
-                    }], n && We(t.prototype, n), Object.defineProperty(t, "prototype", {
+                    }], n && He(t.prototype, n), Object.defineProperty(t, "prototype", {
                         writable: !1
                     }), d
                 }(a.Component);
-                Xe.propTypes = {
+                Ye.propTypes = {
                     inDetail: f().bool,
                     depth: f().number
-                }, Xe.defaultProps = {
+                }, Ye.defaultProps = {
                     inDetail: !1,
                     depth: 0
                 }
             },
             7573: (e, t, n) => {
                 "use strict";
                 n.d(t, {
@@ -13232,17 +13228,16 @@
                             return wn(this, n), (o = t.call(this, e)).state = {
                                 activeIndex: u.parse(e.router.location.search).tab || 0
                             }, o.setActiveIndex = o.setActiveIndex.bind(Sn(o)), o
                         }
                         return xn(n, [{
                             key: "setActiveIndex",
                             value: function(e) {
-                                var t = u.parse(this.props.router.location.search);
-                                t.tab = e.index, t = u.stringify(t), this.props.router.history.replace({
-                                    search: t
+                                (0, Ge.k_)(this.props.router, {
+                                    tab: e.index
                                 }), this.setState({
                                     activeIndex: e.index
                                 })
                             }
                         }, {
                             key: "render",
                             value: function() {
@@ -14440,21 +14435,21 @@
                         value: function() {
                             window.addEventListener("beforeunload", this.onBeforeUnload), window.addEventListener("popstate", this.onPopState), window.addEventListener("keydown", this.onKeyDown)
                         }
                     }, {
                         key: "getSnapshotBeforeUpdate",
                         value: function(e, t) {
                             var n = {};
-                            return l().isEqual(e.data, this.props.data) || (n.newValue = !0), e.taskId !== this.props.taskId && (n.newTask = !0), e.editing_mode !== this.props.editing_mode && (n.editing_mode = this.props.editing_mode), n
+                            return l().isEqual(e.data, this.props.data) || (n.newValue = !0), e.taskId !== this.props.taskId && (n.newTask = !0), e.editing_mode !== this.props.editing_mode && (n.editing_mode = this.props.editing_mode), l().isEqual(e.disabled_fields, this.props.disabled_fields) || (n.dfChanges = !0), n
                         }
                     }, {
                         key: "componentDidUpdate",
                         value: function(e, t, n) {
                             var o = {};
-                            n.newValue && (this.data.data = this.props.data, this.data.original_data = (0, a.cloneDeep)(this.props.data), o.loading = !1), n.hasOwnProperty("editing_mode") && (n.editing_mode || (this.parent.data.data = this.data.original_data, this.data.editorDirty = !1, window.postMessage("editorClean", "*")), o.editing_mode = n.editing_mode), n.newTask && this.saveThenDo(this.props.task), Object.keys(o).length && this.setState(o)
+                            n.newValue && (this.data.data = this.props.data, this.data.original_data = (0, a.cloneDeep)(this.props.data), o.loading = !1), n.hasOwnProperty("editing_mode") && (n.editing_mode || (this.parent.data.data = this.data.original_data, this.data.editorDirty = !1, window.postMessage("editorClean", "*")), o.editing_mode = n.editing_mode), n.newTask && this.saveThenDo(this.props.task), n.dfChanges && (o.disabled_fields = this.props.disabled_fields), Object.keys(o).length && this.setState(o)
                         }
                     }, {
                         key: "componentWillUnmount",
                         value: function() {
                             window.removeEventListener("beforeunload", this.onBeforeUnload), window.removeEventListener("popstate", this.onPopState), window.removeEventListener("keydown", this.onKeyDown), delete window.Detail, window.postMessage("editorClean", "*")
                         }
                     }, {
@@ -15301,15 +15296,15 @@
                                 }
                             })) : null
                         }
                     }, {
                         key: "renderEditorButton",
                         value: function() {
                             var e = this;
-                            return this.parent.data.detail_window && this.parent.props.actorData.editable ? o.createElement("span", {
+                            return this.parent.data.detail_window && this.parent.props.actorData.editable && !this.parent.props.actorData.edit_safe ? o.createElement("span", {
                                 hidden: this.parent.data.data.disable_editing
                             }, o.createElement(c.C, {
                                 checked: !this.parent.data.editing_mode,
                                 className: "l-bbar-editor-button",
                                 onChange: function(t) {
                                     e.parent.data.editing_mode = !e.parent.data.editing_mode, e.parent.setState({
                                         loading: !1
@@ -15454,130 +15449,146 @@
                         }
                     }]), n
                 }(o.Component)
             },
             9502: (e, t, n) => {
                 "use strict";
                 n.d(t, {
-                    eJ: () => l,
-                    tq: () => p,
-                    ol: () => u,
-                    rX: () => c,
-                    Ds: () => d,
-                    a_: () => f,
-                    qI: () => h,
-                    ku: () => m,
-                    dm: () => b,
-                    ah: () => g,
-                    pP: () => v,
-                    un: () => y
+                    eJ: () => s,
+                    tq: () => u,
+                    k_: () => c,
+                    VW: () => d,
+                    ol: () => f,
+                    rX: () => h,
+                    Ds: () => m,
+                    a_: () => b,
+                    qI: () => g,
+                    ku: () => v,
+                    dm: () => y,
+                    ah: () => w,
+                    pP: () => k,
+                    un: () => x
                 });
                 var o = n(2279),
                     r = n.n(o),
-                    i = n(1008);
+                    i = n(7705),
+                    a = n(1008);
 
-                function a(e) {
-                    return a = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+                function l(e) {
+                    return l = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                         return typeof e
                     } : function(e) {
                         return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-                    }, a(e)
+                    }, l(e)
                 }
 
-                function l(e) {
+                function s(e) {
                     return e.router.match && e.router.match.isExact ? "show" === e.actorData.default_action ? -99998 : void 0 : parseInt(e.router.history.location.pathname.split("/")[4])
                 }
-                var s = function(e) {
+                var p = function(e) {
                     return e != e
                 };
 
-                function p() {
+                function u() {
                     return window.matchMedia("only screen and (max-width: 760px)").matches
                 }
 
-                function u(e, t) {
+                function c(e, t, n) {
+                    var o = i.parse(e.location.search);
+                    return Object.assign(o, t), o = i.stringify(o), n ? e.history.replace({
+                        search: o
+                    }) : e.history.push({
+                        search: o
+                    }), e
+                }
+
+                function d(e, t) {
+                    return i.parse(e.history.location.search)
+                }
+
+                function f(e, t) {
                     for (var n = void 0, o = 0; o < e.length; o++) {
                         var r = e[o],
                             i = r[0];
                         if (null != i) {
                             if (i > t) {
                                 n = r[1];
                                 break
                             }
                         } else n = r[1]
                     }
                     return n
                 }
 
-                function c(e) {
-                    return !i.X8.includes(e) && window.hasOwnProperty("Detail") && window.App.data.editorDirty
+                function h(e) {
+                    return !a.X8.includes(e) && window.hasOwnProperty("Detail") && window.App.data.editorDirty
                 }
 
-                function d(e) {
+                function m(e) {
                     var t, n = this,
                         o = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 300;
                     return function() {
                         for (var r = arguments.length, i = new Array(r), a = 0; a < r; a++) i[a] = arguments[a];
                         clearTimeout(t), t = setTimeout((function() {
                             e.apply(n, i)
                         }), o)
                     }
                 }
 
-                function f(e) {
+                function b(e) {
                     return function(t, n) {
                         var o;
                         t && (o = void 0 === n ? r()(t) : n, e[o] = t, t.rp = o), Object.keys(e).forEach((function(t) {
                             null === e[t] && delete e[t]
                         }))
                     }
                 }
 
-                function h(e, t, n) {
+                function g(e, t, n) {
                     var o = {
                         rp: void 0,
                         rp_obj: void 0
                     };
                     if ("string" == typeof e) o.rp_obj = t[e];
                     else if (e) {
                         var i = r()(e);
-                        t[i] ? (o.rp = i, o.rp_obj = t[i]) : n && (o.rp = i, o.rp_obj = e, f(t)(e, i))
+                        t[i] ? (o.rp = i, o.rp_obj = t[i]) : n && (o.rp = i, o.rp_obj = e, b(t)(e, i))
                     }
                     return o
                 }
 
-                function m(e, t) {
+                function v(e, t) {
                     var n = Object.keys(e);
                     return t.map((function(t) {
                         var o;
                         return void 0 === (o = n.includes(t + "Hidden") ? e[t + "Hidden"] : e[t]) && (o = null), o
                     }))
                 }
 
-                function b() {
+                function y() {
                     var e, t, n, o;
 
                     function r(e, t) {
                         var i;
-                        if (s(e) && s(t) && "number" == typeof e && "number" == typeof t) return !0;
+                        if (p(e) && p(t) && "number" == typeof e && "number" == typeof t) return !0;
                         if (e === t) return !0;
                         if ("function" == typeof e && "function" == typeof t || e instanceof Date && t instanceof Date || e instanceof RegExp && t instanceof RegExp || e instanceof String && t instanceof String || e instanceof Number && t instanceof Number) return e.toString() === t.toString();
                         if (!(e instanceof Object && t instanceof Object)) return !1;
                         if (e.isPrototypeOf(t) || t.isPrototypeOf(e)) return !1;
                         if (e.constructor !== t.constructor) return !1;
                         if (e.prototype !== t.prototype) return !1;
                         if (n.indexOf(e) > -1 || o.indexOf(t) > -1) return !1;
                         for (i in t) {
                             if (t.hasOwnProperty(i) !== e.hasOwnProperty(i)) return !1;
-                            if (a(t[i]) !== a(e[i])) return !1
+                            if (l(t[i]) !== l(e[i])) return !1
                         }
                         for (i in e) {
                             if (t.hasOwnProperty(i) !== e.hasOwnProperty(i)) return !1;
-                            if (a(t[i]) !== a(e[i])) return !1;
-                            switch (a(e[i])) {
+                            if (l(t[i]) !== l(e[i])) return !1;
+                            switch (l(e[i])) {
                                 case "object":
                                 case "function":
                                     if (n.push(e), o.push(t), !r(e[i], t[i])) return !1;
                                     n.pop(), o.pop();
                                     break;
                                 default:
                                     if (e[i] !== t[i]) return !1
@@ -15587,74 +15598,35 @@
                     }
                     if (arguments.length < 1) return !0;
                     for (e = 1, t = arguments.length; e < t; e++)
                         if (n = [], o = [], !r(arguments[0], arguments[e])) return !1;
                     return !0
                 }
 
-                function g(e) {
+                function w(e) {
                     var t = "",
                         n = window.App.state.user_settings,
                         o = n.user_type,
                         r = n.lang,
                         i = n.site_name;
                     return [null, void 0].includes(e) || (t = "_".concat(e)), "ActorData_".concat(window.App.state.user_settings.su_user_type || o, "_").concat(r, "_").concat(i).concat(t)
                 }
 
-                function v(e, t) {
+                function k(e, t) {
                     return e.reduceRight((function(e, n) {
                         return e.push(t(n)), e
                     }), [])
                 }
 
-                function y(e) {
+                function x(e) {
                     var t, n = 0;
                     if (0 === e.length) return n;
                     for (t = 0; t < e.length; t++) n = (n << 5) - n + e.charCodeAt(t), n |= 0;
                     return n
                 }
-                window.WindowStateManager || function(e) {
-                    var t, n, o, r = "WINDOW_VALIDATION",
-                        i = !1,
-                        a = !1,
-                        l = !1,
-                        s = !1;
-
-                    function p(t, r, a) {
-                        o = a, l = t, s = r, n = Date.now().toString(), e.addEventListener("beforeunload", (function() {
-                            c()
-                        })), e.addEventListener("unload", (function() {
-                            c()
-                        })), u.call(this), i = !0, o.call(this, this)
-                    }
-
-                    function u() {
-                        var e = this,
-                            p = a;
-                        t = null === (t = localStorage.getItem(r)) || "NaN" === t ? [] : JSON.parse(t), s && document.hasFocus() && i ? (t.splice(t.indexOf(n), 1), t.push(n), a = !0, localStorage.setItem(r, JSON.stringify(t))) : i ? a = t.length <= 1 || (l ? t[t.length - 1] : t[0]) === n : 0 === t.length ? (a = !0, t[0] = n, localStorage.setItem(r, JSON.stringify(t))) : (a = !1, t.push(n), localStorage.setItem(r, JSON.stringify(t))), p !== a && o.call(this, this), setTimeout((function() {
-                            u.call(e)
-                        }), 100)
-                    }
-
-                    function c() {
-                        for (var e = JSON.parse(localStorage.getItem(r)), t = 0, o = e.length; t < o; t++)
-                            if (e[t] === n) {
-                                e.splice(t, 1);
-                                break
-                            } localStorage.setItem(r, JSON.stringify(e))
-                    }
-                    p.prototype.isMainWindow = function() {
-                        return a
-                    }, p.prototype.resetWindows = function() {
-                        localStorage.removeItem(r)
-                    }, p.prototype.makeMain = function() {
-                        var e = JSON.parse(localStorage.getItem(r));
-                        e.splice(e.indexOf(n), 1), e.push(n), localStorage.setItem(r, JSON.stringify(e))
-                    }, e.WindowStateManager = p
-                }(window)
             },
             1266: (e, t, n) => {
                 "use strict";
                 n.d(t, {
                     C: () => d
                 });
                 var o = n(2437),
```

### Comparing `lino_react-23.6.2/lino_react/react/static/react/main.js.LICENSE.txt` & `lino_react-23.7.0/lino_react/react/static/react/main.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.2/lino_react/react/views.py` & `lino_react-23.7.0/lino_react/react/views.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.2/lino_react/setup_info.py` & `lino_react-23.7.0/lino_react/setup_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: UTF-8 -*-
 # Copyright 2015-2023 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
 SETUP_INFO = dict(
     name='lino_react',
-    version='23.6.2',
+    version='23.7.0',
     install_requires=['lino'],
     tests_require=[],
     test_suite='tests',
     description="The React front end for Lino",
     license_files=['COPYING'],
     include_package_data=False,
     zip_safe=False,
```

### Comparing `lino_react-23.6.2/lino_react.egg-info/PKG-INFO` & `lino_react-23.7.0/lino_react.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lino-react
-Version: 23.6.2
+Version: 23.7.0
 Summary: The React front end for Lino
 Home-page: https://gitlab.com/lino-framework/react
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 Classifier:   Programming Language :: Python
 Classifier:   Programming Language :: Python :: 3
 Classifier:   Development Status :: 5 - Production/Stable
```

### Comparing `lino_react-23.6.2/lino_react.egg-info/SOURCES.txt` & `lino_react-23.7.0/lino_react.egg-info/SOURCES.txt`

 * *Files identical despite different names*

