# Comparing `tmp/crochet-2.0.0.tar.gz` & `tmp/crochet-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crochet-2.0.0.tar", last modified: Mon May 10 20:34:43 2021, max compression
+gzip compressed data, was "crochet-2.1.1.tar", last modified: Sat Jul  1 20:54:22 2023, max compression
```

## Comparing `crochet-2.0.0.tar` & `crochet-2.1.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 itamarst  (1000) itamarst  (1000)        0 2021-05-10 20:34:43.542455 crochet-2.0.0/
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)     1090 2013-10-05 20:47:11.000000 crochet-2.0.0/LICENSE
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)      186 2014-05-31 19:55:36.000000 crochet-2.0.0/MANIFEST.in
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)    12499 2021-05-10 20:34:43.542455 crochet-2.0.0/PKG-INFO
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)     2301 2021-05-10 20:34:24.000000 crochet-2.0.0/README.rst
-drwxrwxr-x   0 itamarst  (1000) itamarst  (1000)        0 2021-05-10 20:34:43.542455 crochet-2.0.0/crochet/
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)     1132 2021-05-10 20:34:24.000000 crochet-2.0.0/crochet/__init__.py
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)      799 2021-05-10 20:34:24.000000 crochet-2.0.0/crochet/__init__.pyi
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)    16237 2021-05-10 20:34:24.000000 crochet-2.0.0/crochet/_eventloop.py
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)     1488 2017-08-09 20:33:23.000000 crochet-2.0.0/crochet/_resultstore.py
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)     1591 2019-06-07 18:56:32.000000 crochet-2.0.0/crochet/_shutdown.py
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)      411 2017-08-09 20:33:23.000000 crochet-2.0.0/crochet/_util.py
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)      471 2021-05-10 20:34:43.542455 crochet-2.0.0/crochet/_version.py
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)     1759 2021-05-10 20:34:24.000000 crochet-2.0.0/crochet/mypy.py
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)        0 2021-05-10 20:34:24.000000 crochet-2.0.0/crochet/py.typed
-drwxrwxr-x   0 itamarst  (1000) itamarst  (1000)        0 2021-05-10 20:34:43.540455 crochet-2.0.0/crochet/tests/
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)      190 2017-08-09 20:33:23.000000 crochet-2.0.0/crochet/tests/__init__.py
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)    34829 2021-05-10 20:34:24.000000 crochet-2.0.0/crochet/tests/test_api.py
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)     2638 2017-08-09 20:33:23.000000 crochet-2.0.0/crochet/tests/test_logging.py
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)    14220 2021-05-10 20:34:24.000000 crochet-2.0.0/crochet/tests/test_mypy.py
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)     1885 2017-08-09 20:33:23.000000 crochet-2.0.0/crochet/tests/test_process.py
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)     2353 2017-08-09 20:33:23.000000 crochet-2.0.0/crochet/tests/test_resultstore.py
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)    11411 2021-05-10 20:34:24.000000 crochet-2.0.0/crochet/tests/test_setup.py
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)     3365 2017-08-09 20:33:23.000000 crochet-2.0.0/crochet/tests/test_shutdown.py
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)     1724 2017-08-09 20:33:23.000000 crochet-2.0.0/crochet/tests/test_util.py
-drwxrwxr-x   0 itamarst  (1000) itamarst  (1000)        0 2021-05-10 20:34:43.539455 crochet-2.0.0/crochet.egg-info/
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)    12499 2021-05-10 20:34:43.000000 crochet-2.0.0/crochet.egg-info/PKG-INFO
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)     1045 2021-05-10 20:34:43.000000 crochet-2.0.0/crochet.egg-info/SOURCES.txt
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)        1 2021-05-10 20:34:43.000000 crochet-2.0.0/crochet.egg-info/dependency_links.txt
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)       20 2021-05-10 20:34:43.000000 crochet-2.0.0/crochet.egg-info/requires.txt
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)        8 2021-05-10 20:34:43.000000 crochet-2.0.0/crochet.egg-info/top_level.txt
-drwxrwxr-x   0 itamarst  (1000) itamarst  (1000)        0 2021-05-10 20:34:43.541455 crochet-2.0.0/docs/
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)     5568 2013-09-16 23:37:18.000000 crochet-2.0.0/docs/Makefile
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)      381 2017-08-09 20:32:39.000000 crochet-2.0.0/docs/api-reference.rst
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)     7612 2021-05-10 20:34:24.000000 crochet-2.0.0/docs/api.rst
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)      664 2017-08-08 19:57:34.000000 crochet-2.0.0/docs/async.rst
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)     7849 2017-08-09 20:32:39.000000 crochet-2.0.0/docs/conf.py
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)     1290 2021-05-10 20:34:24.000000 crochet-2.0.0/docs/index.rst
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)      853 2017-08-08 20:00:04.000000 crochet-2.0.0/docs/introduction.rst
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)     5098 2013-09-16 23:37:18.000000 crochet-2.0.0/docs/make.bat
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)     6923 2021-05-10 20:34:24.000000 crochet-2.0.0/docs/news.rst
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)     2347 2021-05-10 20:34:24.000000 crochet-2.0.0/docs/type-checking.rst
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)     2320 2017-08-08 20:00:44.000000 crochet-2.0.0/docs/using.rst
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)     3604 2017-08-08 20:01:40.000000 crochet-2.0.0/docs/workarounds.rst
-drwxrwxr-x   0 itamarst  (1000) itamarst  (1000)        0 2021-05-10 20:34:43.542455 crochet-2.0.0/examples/
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)      962 2021-05-10 20:34:24.000000 crochet-2.0.0/examples/async.py
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)      955 2015-04-25 18:16:28.000000 crochet-2.0.0/examples/blockingdns.py
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)     1415 2014-01-11 21:33:15.000000 crochet-2.0.0/examples/downloader.py
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)     1228 2014-05-31 18:26:34.000000 crochet-2.0.0/examples/fromtwisted.py
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)     1020 2015-04-18 22:10:35.000000 crochet-2.0.0/examples/mxquery.py
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)     2648 2014-04-06 22:05:06.000000 crochet-2.0.0/examples/scheduling.py
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)     1973 2014-04-06 22:05:06.000000 crochet-2.0.0/examples/ssh.py
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)      446 2017-08-17 18:54:20.000000 crochet-2.0.0/examples/testing.py
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)       45 2021-05-10 20:34:24.000000 crochet-2.0.0/requirements-dev.txt
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)      200 2021-05-10 20:34:43.542455 crochet-2.0.0/setup.cfg
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)     1396 2021-05-10 20:34:24.000000 crochet-2.0.0/setup.py
--rw-rw-r--   0 itamarst  (1000) itamarst  (1000)    65747 2016-04-13 20:04:38.000000 crochet-2.0.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:54:22.325390 crochet-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-01 20:54:17.000000 crochet-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-01 20:54:17.000000 crochet-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-07-01 20:54:22.325390 crochet-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-01 20:54:17.000000 crochet-2.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:54:22.325390 crochet-2.1.1/crochet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-01 20:54:17.000000 crochet-2.1.1/crochet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-01 20:54:17.000000 crochet-2.1.1/crochet/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15558 2023-07-01 20:54:17.000000 crochet-2.1.1/crochet/_eventloop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-01 20:54:17.000000 crochet-2.1.1/crochet/_resultstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-01 20:54:17.000000 crochet-2.1.1/crochet/_shutdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-01 20:54:17.000000 crochet-2.1.1/crochet/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-01 20:54:22.325390 crochet-2.1.1/crochet/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-01 20:54:17.000000 crochet-2.1.1/crochet/mypy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 20:54:17.000000 crochet-2.1.1/crochet/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:54:22.321390 crochet-2.1.1/crochet/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-01 20:54:17.000000 crochet-2.1.1/crochet/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33323 2023-07-01 20:54:17.000000 crochet-2.1.1/crochet/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-01 20:54:17.000000 crochet-2.1.1/crochet/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14220 2023-07-01 20:54:17.000000 crochet-2.1.1/crochet/tests/test_mypy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-01 20:54:17.000000 crochet-2.1.1/crochet/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-01 20:54:17.000000 crochet-2.1.1/crochet/tests/test_resultstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-07-01 20:54:17.000000 crochet-2.1.1/crochet/tests/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-01 20:54:17.000000 crochet-2.1.1/crochet/tests/test_shutdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-01 20:54:17.000000 crochet-2.1.1/crochet/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:54:22.321390 crochet-2.1.1/crochet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-07-01 20:54:22.000000 crochet-2.1.1/crochet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-01 20:54:22.000000 crochet-2.1.1/crochet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 20:54:22.000000 crochet-2.1.1/crochet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-01 20:54:22.000000 crochet-2.1.1/crochet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-01 20:54:22.000000 crochet-2.1.1/crochet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:54:22.325390 crochet-2.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-01 20:54:17.000000 crochet-2.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-01 20:54:17.000000 crochet-2.1.1/docs/api-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-07-01 20:54:17.000000 crochet-2.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-01 20:54:17.000000 crochet-2.1.1/docs/async.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-07-01 20:54:17.000000 crochet-2.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-01 20:54:17.000000 crochet-2.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-01 20:54:17.000000 crochet-2.1.1/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-07-01 20:54:17.000000 crochet-2.1.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-01 20:54:17.000000 crochet-2.1.1/docs/news.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-01 20:54:17.000000 crochet-2.1.1/docs/type-checking.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-01 20:54:17.000000 crochet-2.1.1/docs/using.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-01 20:54:17.000000 crochet-2.1.1/docs/workarounds.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:54:22.325390 crochet-2.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-01 20:54:17.000000 crochet-2.1.1/examples/async.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-01 20:54:17.000000 crochet-2.1.1/examples/blockingdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-01 20:54:17.000000 crochet-2.1.1/examples/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-01 20:54:17.000000 crochet-2.1.1/examples/fromtwisted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-01 20:54:17.000000 crochet-2.1.1/examples/mxquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-01 20:54:17.000000 crochet-2.1.1/examples/scheduling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-01 20:54:17.000000 crochet-2.1.1/examples/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-01 20:54:17.000000 crochet-2.1.1/examples/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-01 20:54:17.000000 crochet-2.1.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-01 20:54:22.325390 crochet-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-01 20:54:17.000000 crochet-2.1.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65747 2023-07-01 20:54:17.000000 crochet-2.1.1/versioneer.py
```

### Comparing `crochet-2.0.0/LICENSE` & `crochet-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/PKG-INFO` & `crochet-2.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,328 +1,333 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: crochet
-Version: 2.0.0
+Version: 2.1.1
 Summary: Use Twisted anywhere!
 Home-page: https://github.com/itamarst/crochet
 Maintainer: Itamar Turner-Trauring
 Maintainer-email: itamar@itamarst.org
 License: MIT
-Description: Crochet: Use Twisted anywhere!
-        ==============================
-        
-        Crochet is an MIT-licensed library that makes it easier to use Twisted from
-        regular blocking code. Some use cases include:
-        
-        * Easily use Twisted from a blocking framework like Django or Flask.
-        * Write a library that provides a blocking API, but uses Twisted for its
-          implementation.
-        * Port blocking code to Twisted more easily, by keeping a backwards
-          compatibility layer.
-        * Allow normal Twisted programs that use threads to interact with Twisted more
-          cleanly from their threaded parts. For example, this can be useful when using
-          Twisted as a `WSGI container`_.
-        
-        .. _WSGI container: https://twistedmatrix.com/documents/current/web/howto/web-in-60/wsgi.html
-        
-        Crochet is maintained by Itamar Turner-Trauring.
-        
-          **Note:** Crochet development is pretty slow these days because mostly it **Just Works**. PyPI shows about 30,000 downloads a month, so existing users seem happy: https://pypistats.org/packages/crochet
-        
-        You can install Crochet by running::
-        
-          $ pip install crochet
-        
-        Downloads are available on `PyPI`_.
-        
-        Documentation can be found on `Read The Docs`_.
-        
-        Bugs and feature requests should be filed at the project `Github page`_.
-        
-        .. _Read the Docs: https://crochet.readthedocs.org/
-        .. _Github page: https://github.com/itamarst/crochet/
-        .. _PyPI: https://pypi.python.org/pypi/crochet
-        
-        
-        API and features
-        ================
-        
-        Crochet supports Python 3.6, 3.7, 3.8, and 3.9 as well as PyPy3.
-        Python 2.7 and 3.5 support is available in older releases.
-        
-        Crochet provides the following basic APIs:
-        
-        * Allow blocking code to call into Twisted and block until results are available
-          or a timeout is hit, using the ``crochet.wait_for`` decorator.
-        * A lower-level API (``crochet.run_in_reactor``) allows blocking code to run
-          code "in the background" in the Twisted thread, with the ability to repeatedly
-          check if it's done.
-        
-        Crochet will do the following on your behalf in order to enable these APIs:
-        
-        * Transparently start Twisted's reactor in a thread it manages.
-        * Shut down the reactor automatically when the process' main thread finishes.
-        * Hook up Twisted's log system to the Python standard library ``logging``
-          framework. Unlike Twisted's built-in ``logging`` bridge, this includes
-          support for blocking `Handler` instances.
-        
-        What's New
-        ==========
-        
-        2.0.0
-        ^^^^^
-        
-        New features:
-        
-        * It's possible to decorate ``async/await`` Twisted functions with ``@wait_for`` and ``@run_in_reactor``, thanks to Árni Már Jónsson.
-        * Added type hints, thanks to Merlin Davis.
-        * Added formal support for Python 3.9.
-        
-        
-        Removed features:
-        
-        * Dropped the deprecated APIs ``@wait_for_reactor``, ``@in_reactor``, ``DeferredResult``, the ``wrapped_function`` attribute, and unlimited timeouts on ``EventualResult.wait()``.
-        * Dropped support for Python 2.7 and 3.5.
-        
-        1.12.0
-        ^^^^^^
-        
-        Bug fixes:
-        
-        * Fix a timeout overflow bug in 32-bit machines.
-        
-        
-        1.11.0
-        ^^^^^^
-        
-        New features:
-        
-        * Added support for Python 3.8 and PyPy 3.
-        
-        Backwards incompatibility:
-        
-        * Dropped support for Python 3.4, since latest Twisted doesn't support it.
-        
-        1.10.0
-        ^^^^^^
-        
-        New features:
-        
-        * Added support for Python 3.7. Thanks to Jeremy Cline for the patch.
-        
-        1.9.0
-        ^^^^^
-        
-        New features:
-        
-        * The underlying callable wrapped ``@run_in_reactor`` and ``@wait_for`` is now available via the more standard ``__wrapped__`` attribute.
-        
-        Backwards incompatibility (in tests):
-        
-        * This was actually introduced in 1.8.0: ``wrapped_function`` may not always be available on decorated callables.
-          You should use ``__wrapped__`` instead.
-        
-        Bug fixes:
-        
-        * Fixed regression in 1.8.0 where bound method couldn't be wrapped.
-          Thanks to 2mf for the bug report.
-        
-        1.8.0
-        ^^^^^
-        
-        New features:
-        
-        * Signatures on decorated functions now match the original functions.
-          Thanks to Mikhail Terekhov for the original patch.
-        * Documentation improvements, including an API reference.
-        
-        Bug fixes:
-        
-        * Switched to EPoll reactor for logging thread.
-          Anecdotal evidence suggests this fixes some issues on AWS Lambda, but it's not clear why.
-          Thanks to Rolando Espinoza for the patch.
-        * It's now possible to call ``@run_in_reactor`` and ``@wait_for`` above a ``@classmethod``.
-          Thanks to vak for the bug report.
-        
-        1.7.0
-        ^^^^^
-        
-        Bug fixes:
-        
-        * If the Python ``logging.Handler`` throws an exception Crochet no longer goes into a death spiral.
-          Thanks to Michael Schlenker for the bug report.
-        
-        Removed features:
-        
-        * Versions of Twisted < 16.0 are no longer supported (i.e. no longer tested in CI.)
-        
-        1.6.0
-        ^^^^^
-        
-        New features:
-        
-        * Added support for Python 3.6.
-        
-        1.5.0
-        ^^^^^
-        
-        New features:
-        
-        * Added support for Python 3.5.
-        
-        Removed features:
-        
-        * Python 2.6, Python 3.3, and versions of Twisted < 15.0 are no longer supported.
-        
-        1.4.0
-        ^^^^^
-        
-        New features:
-        
-        * Added support for Python 3.4.
-        
-        Documentation:
-        
-        * Added a section on known issues and workarounds.
-        
-        Bug fixes:
-        
-        * Main thread detection (used to determine when Crochet should shutdown) is now less fragile.
-          This means Crochet now supports more environments, e.g. uWSGI.
-          Thanks to Ben Picolo for the patch.
-        
-        1.3.0
-        ^^^^^
-        
-        Bug fixes:
-        
-        * It is now possible to call ``EventualResult.wait()`` (or functions
-          wrapped in ``wait_for``) at import time if another thread holds the
-          import lock. Thanks to Ken Struys for the patch.
-        
-        1.2.0
-        ^^^^^
-        New features:
-        
-        * ``crochet.wait_for`` implements the timeout/cancellation pattern documented
-          in previous versions of Crochet. ``crochet.wait_for_reactor`` and
-          ``EventualResult.wait(timeout=None)`` are now deprecated, since lacking
-          timeouts they could potentially block forever.
-        * Functions wrapped with ``wait_for`` and ``run_in_reactor`` can now be accessed
-          via the ``wrapped_function`` attribute, to ease unit testing of the underlying
-          Twisted code.
-        
-        API changes:
-        
-        * It is no longer possible to call ``EventualResult.wait()`` (or functions
-          wrapped with ``wait_for``) at import time, since this can lead to deadlocks
-          or prevent other threads from importing. Thanks to Tom Prince for the bug
-          report.
-        
-        Bug fixes:
-        
-        * ``warnings`` are no longer erroneously turned into Twisted log messages.
-        * The reactor is now only imported when ``crochet.setup()`` or
-          ``crochet.no_setup()`` are called, allowing daemonization if only ``crochet``
-          is imported (http://tm.tl/7105). Thanks to Daniel Nephin for the bug report.
-        
-        Documentation:
-        
-        * Improved motivation, added contact info and news to the documentation.
-        * Better example of using Crochet from a normal Twisted application.
-        
-        1.1.0
-        ^^^^^
-        Bug fixes:
-        
-        * ``EventualResult.wait()`` can now be used safely from multiple threads,
-          thanks to Gavin Panella for reporting the bug.
-        * Fixed reentrancy deadlock in the logging code caused by
-          http://bugs.python.org/issue14976, thanks to Rod Morehead for reporting the
-          bug.
-        * Crochet now installs on Python 3.3 again, thanks to Ben Cordero.
-        * Crochet should now work on Windows, thanks to Konstantinos Koukopoulos.
-        * Crochet tests can now run without adding its absolute path to PYTHONPATH or
-          installing it first.
-        
-        Documentation:
-        
-        * ``EventualResult.original_failure`` is now documented.
-        
-        1.0.0
-        ^^^^^
-        Documentation:
-        
-        * Added section on use cases and alternatives. Thanks to Tobias Oberstein for
-          the suggestion.
-        
-        Bug fixes:
-        
-        * Twisted does not have to be pre-installed to run ``setup.py``, thanks to
-          Paul Weaver for bug report and Chris Scutcher for patch.
-        * Importing Crochet does not have side-effects (installing reactor event)
-          any more.
-        * Blocking calls are interrupted earlier in the shutdown process, to reduce
-          scope for deadlocks. Thanks to rmorehead for bug report.
-        
-        0.9.0
-        ^^^^^
-        New features:
-        
-        * Expanded and much improved documentation, including a new section with
-          design suggestions.
-        * New decorator ``@wait_for_reactor`` added, a simpler alternative to
-          ``@run_in_reactor``.
-        * Refactored ``@run_in_reactor``, making it a bit more responsive.
-        * Blocking operations which would otherwise never finish due to reactor having
-          stopped (``EventualResult.wait()`` or ``@wait_for_reactor`` decorated call)
-          will be interrupted with a ``ReactorStopped`` exception. Thanks to rmorehead
-          for the bug report.
-        
-        Bug fixes:
-        
-        * ``@run_in_reactor`` decorated functions (or rather, their generated wrapper)
-          are interrupted by Ctrl-C.
-        * On POSIX platforms, a workaround is installed to ensure processes started by
-          `reactor.spawnProcess` have their exit noticed. See `Twisted ticket 6378`_
-          for more details about the underlying issue.
-        
-        .. _Twisted ticket 6378: http://tm.tl/6738
-        
-        0.8.1
-        ^^^^^
-        * ``EventualResult.wait()`` now raises error if called in the reactor thread,
-          thanks to David Buchmann.
-        * Unittests are now included in the release tarball.
-        * Allow Ctrl-C to interrupt ``EventualResult.wait(timeout=None)``.
-        
-        0.7.0
-        ^^^^^
-        * Improved documentation.
-        
-        0.6.0
-        ^^^^^
-        * Renamed ``DeferredResult`` to ``EventualResult``, to reduce confusion with
-          Twisted's ``Deferred`` class. The old name still works, but is deprecated.
-        * Deprecated ``@in_reactor``, replaced with ``@run_in_reactor`` which doesn't
-          change the arguments to the wrapped function. The deprecated API still works,
-          however.
-        * Unhandled exceptions in ``EventualResult`` objects are logged.
-        * Added more examples.
-        * ``setup.py sdist`` should work now.
-        
-        0.5.0
-        ^^^^^
-        * Initial release.
-        
 Keywords: twisted threading
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6.0
+Requires-Python: >=3.8.0
+License-File: LICENSE
+
+Crochet: Use Twisted anywhere!
+==============================
+
+Crochet is an MIT-licensed library that makes it easier to use Twisted from
+regular blocking code. Some use cases include:
+
+* Easily use Twisted from a blocking framework like Django or Flask.
+* Write a library that provides a blocking API, but uses Twisted for its
+  implementation.
+* Port blocking code to Twisted more easily, by keeping a backwards
+  compatibility layer.
+* Allow normal Twisted programs that use threads to interact with Twisted more
+  cleanly from their threaded parts. For example, this can be useful when using
+  Twisted as a `WSGI container`_.
+
+.. _WSGI container: https://twistedmatrix.com/documents/current/web/howto/web-in-60/wsgi.html
+
+Crochet is maintained by Itamar Turner-Trauring.
+
+  **Note:** Crochet development is pretty slow these days because mostly it **Just Works**. PyPI shows about 30,000 downloads a month, so existing users seem happy: https://pypistats.org/packages/crochet
+
+You can install Crochet by running::
+
+  $ pip install crochet
+
+Downloads are available on `PyPI`_.
+
+Documentation can be found on `Read The Docs`_.
+
+Bugs and feature requests should be filed at the project `Github page`_.
+
+.. _Read the Docs: https://crochet.readthedocs.org/
+.. _Github page: https://github.com/itamarst/crochet/
+.. _PyPI: https://pypi.python.org/pypi/crochet
+
+
+API and features
+================
+
+Crochet supports Python 3.8, 3.9, 3.10, and 3.11 as well as PyPy3.
+
+Crochet provides the following basic APIs:
+
+* Allow blocking code to call into Twisted and block until results are available
+  or a timeout is hit, using the ``crochet.wait_for`` decorator.
+* A lower-level API (``crochet.run_in_reactor``) allows blocking code to run
+  code "in the background" in the Twisted thread, with the ability to repeatedly
+  check if it's done.
+
+Crochet will do the following on your behalf in order to enable these APIs:
+
+* Transparently start Twisted's reactor in a thread it manages.
+* Shut down the reactor automatically when the process' main thread finishes.
+* Hook up Twisted's log system to the Python standard library ``logging``
+  framework. Unlike Twisted's built-in ``logging`` bridge, this includes
+  support for blocking `Handler` instances.
+
+What's New
+==========
+
+2.1.0
+^^^^^
+
+* Various internal modernizations and maintenance.
+* Dropped Python 3.6 and 3.7 support.
+
+2.0.0
+^^^^^
+
+New features:
+
+* It's possible to decorate ``async/await`` Twisted functions with ``@wait_for`` and ``@run_in_reactor``, thanks to Árni Már Jónsson.
+* Added type hints, thanks to Merlin Davis.
+* Added formal support for Python 3.9.
+
+
+Removed features:
+
+* Dropped the deprecated APIs ``@wait_for_reactor``, ``@in_reactor``, ``DeferredResult``, the ``wrapped_function`` attribute, and unlimited timeouts on ``EventualResult.wait()``.
+* Dropped support for Python 2.7 and 3.5.
+
+1.12.0
+^^^^^^
+
+Bug fixes:
+
+* Fix a timeout overflow bug in 32-bit machines.
+
+
+1.11.0
+^^^^^^
+
+New features:
+
+* Added support for Python 3.8 and PyPy 3.
+
+Backwards incompatibility:
+
+* Dropped support for Python 3.4, since latest Twisted doesn't support it.
+
+1.10.0
+^^^^^^
+
+New features:
+
+* Added support for Python 3.7. Thanks to Jeremy Cline for the patch.
+
+1.9.0
+^^^^^
+
+New features:
+
+* The underlying callable wrapped ``@run_in_reactor`` and ``@wait_for`` is now available via the more standard ``__wrapped__`` attribute.
+
+Backwards incompatibility (in tests):
+
+* This was actually introduced in 1.8.0: ``wrapped_function`` may not always be available on decorated callables.
+  You should use ``__wrapped__`` instead.
+
+Bug fixes:
+
+* Fixed regression in 1.8.0 where bound method couldn't be wrapped.
+  Thanks to 2mf for the bug report.
+
+1.8.0
+^^^^^
+
+New features:
+
+* Signatures on decorated functions now match the original functions.
+  Thanks to Mikhail Terekhov for the original patch.
+* Documentation improvements, including an API reference.
+
+Bug fixes:
+
+* Switched to EPoll reactor for logging thread.
+  Anecdotal evidence suggests this fixes some issues on AWS Lambda, but it's not clear why.
+  Thanks to Rolando Espinoza for the patch.
+* It's now possible to call ``@run_in_reactor`` and ``@wait_for`` above a ``@classmethod``.
+  Thanks to vak for the bug report.
+
+1.7.0
+^^^^^
+
+Bug fixes:
+
+* If the Python ``logging.Handler`` throws an exception Crochet no longer goes into a death spiral.
+  Thanks to Michael Schlenker for the bug report.
+
+Removed features:
+
+* Versions of Twisted < 16.0 are no longer supported (i.e. no longer tested in CI.)
+
+1.6.0
+^^^^^
+
+New features:
+
+* Added support for Python 3.6.
+
+1.5.0
+^^^^^
+
+New features:
+
+* Added support for Python 3.5.
+
+Removed features:
+
+* Python 2.6, Python 3.3, and versions of Twisted < 15.0 are no longer supported.
+
+1.4.0
+^^^^^
+
+New features:
+
+* Added support for Python 3.4.
+
+Documentation:
+
+* Added a section on known issues and workarounds.
+
+Bug fixes:
+
+* Main thread detection (used to determine when Crochet should shutdown) is now less fragile.
+  This means Crochet now supports more environments, e.g. uWSGI.
+  Thanks to Ben Picolo for the patch.
+
+1.3.0
+^^^^^
+
+Bug fixes:
+
+* It is now possible to call ``EventualResult.wait()`` (or functions
+  wrapped in ``wait_for``) at import time if another thread holds the
+  import lock. Thanks to Ken Struys for the patch.
+
+1.2.0
+^^^^^
+New features:
+
+* ``crochet.wait_for`` implements the timeout/cancellation pattern documented
+  in previous versions of Crochet. ``crochet.wait_for_reactor`` and
+  ``EventualResult.wait(timeout=None)`` are now deprecated, since lacking
+  timeouts they could potentially block forever.
+* Functions wrapped with ``wait_for`` and ``run_in_reactor`` can now be accessed
+  via the ``wrapped_function`` attribute, to ease unit testing of the underlying
+  Twisted code.
+
+API changes:
+
+* It is no longer possible to call ``EventualResult.wait()`` (or functions
+  wrapped with ``wait_for``) at import time, since this can lead to deadlocks
+  or prevent other threads from importing. Thanks to Tom Prince for the bug
+  report.
+
+Bug fixes:
+
+* ``warnings`` are no longer erroneously turned into Twisted log messages.
+* The reactor is now only imported when ``crochet.setup()`` or
+  ``crochet.no_setup()`` are called, allowing daemonization if only ``crochet``
+  is imported (http://tm.tl/7105). Thanks to Daniel Nephin for the bug report.
+
+Documentation:
+
+* Improved motivation, added contact info and news to the documentation.
+* Better example of using Crochet from a normal Twisted application.
+
+1.1.0
+^^^^^
+Bug fixes:
+
+* ``EventualResult.wait()`` can now be used safely from multiple threads,
+  thanks to Gavin Panella for reporting the bug.
+* Fixed reentrancy deadlock in the logging code caused by
+  http://bugs.python.org/issue14976, thanks to Rod Morehead for reporting the
+  bug.
+* Crochet now installs on Python 3.3 again, thanks to Ben Cordero.
+* Crochet should now work on Windows, thanks to Konstantinos Koukopoulos.
+* Crochet tests can now run without adding its absolute path to PYTHONPATH or
+  installing it first.
+
+Documentation:
+
+* ``EventualResult.original_failure`` is now documented.
+
+1.0.0
+^^^^^
+Documentation:
+
+* Added section on use cases and alternatives. Thanks to Tobias Oberstein for
+  the suggestion.
+
+Bug fixes:
+
+* Twisted does not have to be pre-installed to run ``setup.py``, thanks to
+  Paul Weaver for bug report and Chris Scutcher for patch.
+* Importing Crochet does not have side-effects (installing reactor event)
+  any more.
+* Blocking calls are interrupted earlier in the shutdown process, to reduce
+  scope for deadlocks. Thanks to rmorehead for bug report.
+
+0.9.0
+^^^^^
+New features:
+
+* Expanded and much improved documentation, including a new section with
+  design suggestions.
+* New decorator ``@wait_for_reactor`` added, a simpler alternative to
+  ``@run_in_reactor``.
+* Refactored ``@run_in_reactor``, making it a bit more responsive.
+* Blocking operations which would otherwise never finish due to reactor having
+  stopped (``EventualResult.wait()`` or ``@wait_for_reactor`` decorated call)
+  will be interrupted with a ``ReactorStopped`` exception. Thanks to rmorehead
+  for the bug report.
+
+Bug fixes:
+
+* ``@run_in_reactor`` decorated functions (or rather, their generated wrapper)
+  are interrupted by Ctrl-C.
+* On POSIX platforms, a workaround is installed to ensure processes started by
+  `reactor.spawnProcess` have their exit noticed. See `Twisted ticket 6378`_
+  for more details about the underlying issue.
+
+.. _Twisted ticket 6378: http://tm.tl/6738
+
+0.8.1
+^^^^^
+* ``EventualResult.wait()`` now raises error if called in the reactor thread,
+  thanks to David Buchmann.
+* Unittests are now included in the release tarball.
+* Allow Ctrl-C to interrupt ``EventualResult.wait(timeout=None)``.
+
+0.7.0
+^^^^^
+* Improved documentation.
+
+0.6.0
+^^^^^
+* Renamed ``DeferredResult`` to ``EventualResult``, to reduce confusion with
+  Twisted's ``Deferred`` class. The old name still works, but is deprecated.
+* Deprecated ``@in_reactor``, replaced with ``@run_in_reactor`` which doesn't
+  change the arguments to the wrapped function. The deprecated API still works,
+  however.
+* Unhandled exceptions in ``EventualResult`` objects are logged.
+* Added more examples.
+* ``setup.py sdist`` should work now.
+
+0.5.0
+^^^^^
+* Initial release.
```

### Comparing `crochet-2.0.0/README.rst` & `crochet-2.1.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -33,16 +33,15 @@
 .. _Github page: https://github.com/itamarst/crochet/
 .. _PyPI: https://pypi.python.org/pypi/crochet
 
 
 API and features
 ================
 
-Crochet supports Python 3.6, 3.7, 3.8, and 3.9 as well as PyPy3.
-Python 2.7 and 3.5 support is available in older releases.
+Crochet supports Python 3.8, 3.9, 3.10, and 3.11 as well as PyPy3.
 
 Crochet provides the following basic APIs:
 
 * Allow blocking code to call into Twisted and block until results are available
   or a timeout is hit, using the ``crochet.wait_for`` decorator.
 * A lower-level API (``crochet.run_in_reactor``) allows blocking code to run
   code "in the background" in the Twisted thread, with the ability to repeatedly
```

### Comparing `crochet-2.0.0/crochet/__init__.py` & `crochet-2.1.1/crochet/__init__.py`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/crochet/__init__.pyi` & `crochet-2.1.1/crochet/__init__.pyi`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/crochet/_eventloop.py` & `crochet-2.1.1/crochet/_eventloop.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """
 Expose Twisted's event loop to threaded programs.
 """
 
-from __future__ import absolute_import
-
-import select
 import threading
 import weakref
 import warnings
 from inspect import iscoroutinefunction
 from functools import wraps
+from queue import SimpleQueue
 
 from twisted.python import threadable
 from twisted.python.runtime import platform
 from twisted.python.failure import Failure
 from twisted.python.log import PythonLoggingObserver, err
 from twisted.internet.defer import maybeDeferred, ensureDeferred
 from twisted.internet.task import LoopingCall
@@ -223,69 +221,59 @@
             return None
         if isinstance(result, Failure):
             return result
         else:
             return None
 
 
+_STOP = object()
+
+
 class ThreadLogObserver(object):
     """
     A log observer that wraps another observer, and calls it in a thread.
 
     In particular, used to wrap PythonLoggingObserver, so that blocking
     logging.py Handlers don't block the event loop.
-
-    Once Python 3.6 support is dropped, this can use a queue.SimpleQueue object
-    instead of a whole 'nother event loop.
     """
 
     def __init__(self, observer):
         self._observer = observer
-        if getattr(select, "epoll", None):
-            from twisted.internet.epollreactor import EPollReactor
-            reactorFactory = EPollReactor
-        elif getattr(select, "poll", None):
-            from twisted.internet.pollreactor import PollReactor
-            reactorFactory = PollReactor
-        else:
-            from twisted.internet.selectreactor import SelectReactor
-            reactorFactory = SelectReactor
-        self._logWritingReactor = reactorFactory()
-        self._logWritingReactor._registerAsIOThread = False
+        self._queue = SimpleQueue()
         self._thread = threading.Thread(
             target=self._reader, name="CrochetLogWriter")
         self._thread.start()
 
     def _reader(self):
         """
         Runs in a thread, reads messages from a queue and writes them to
         the wrapped observer.
         """
-        self._logWritingReactor.run(installSignalHandlers=False)
+        while True:
+            msg = self._queue.get()
+            if msg is _STOP:
+                return
+            try:
+                self._observer(msg)
+            except Exception:
+                # Lower-level logging system blew up, nothing we can do, so
+                # just drop on the floor.
+                pass
 
     def stop(self):
         """
         Stop the thread.
         """
-        self._logWritingReactor.callFromThread(self._logWritingReactor.stop)
+        self._queue.put(_STOP)
 
     def __call__(self, msg):
         """
         A log observer that writes to a queue.
         """
-
-        def log():
-            try:
-                self._observer(msg)
-            except Exception:
-                # Lower-level logging system blew up, nothing we can do, so
-                # just drop on the floor.
-                pass
-
-        self._logWritingReactor.callFromThread(log)
+        self._queue.put(msg)
 
 
 class EventLoop(object):
     """
     Initialization infrastructure for running a reactor in a thread.
     """
```

### Comparing `crochet-2.0.0/crochet/_resultstore.py` & `crochet-2.1.1/crochet/_resultstore.py`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/crochet/_shutdown.py` & `crochet-2.1.1/crochet/_shutdown.py`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/crochet/mypy.py` & `crochet-2.1.1/crochet/mypy.py`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/crochet/tests/test_api.py` & `crochet-2.1.1/crochet/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,29 +8,28 @@
 import subprocess
 import time
 import gc
 import sys
 import weakref
 import tempfile
 import os
-import imp
 import inspect
 from unittest import SkipTest
 
 from twisted.trial.unittest import TestCase
 from twisted.internet.defer import succeed, Deferred, fail, CancelledError
 from twisted.python.failure import Failure
 from twisted.python import threadable
 from twisted.python.runtime import platform
 
 from .._eventloop import (
     EventLoop, EventualResult, TimeoutError, ResultRegistry, ReactorStopped)
 from .test_setup import FakeReactor
 from .. import (
-    _main, setup, retrieve_result, _store, no_setup,
+    _main, setup as setup_crochet, retrieve_result, _store, no_setup,
     run_in_reactor, wait_for)
 from ..tests import crochet_directory
 
 if platform.type == "posix":
     try:
         from twisted.internet.process import reapAllProcesses
     except (SyntaxError, ImportError):
@@ -203,15 +202,16 @@
     def test_timeout(self):
         """
         If no result is available, wait(timeout) will throw a TimeoutError.
         """
         start = time.time()
         dr = EventualResult(Deferred(), None)
         self.assertRaises(TimeoutError, dr.wait, timeout=0.03)
-        self.assertTrue(abs(time.time() - start - 0.03) < 0.005)
+        # be a little lenient for slow computers:
+        self.assertTrue(abs(time.time() - start) < 0.05)
 
     def test_timeout_twice(self):
         """
         If no result is available, a second call to wait(timeout) will also
         result in a TimeoutError exception.
         """
         dr = EventualResult(Deferred(), None)
@@ -521,58 +521,14 @@
 from crochet import EventualResult
 from twisted.internet.defer import Deferred
 
 EventualResult(Deferred(), None).wait(1.0)
 """)
         self.assertRaises(RuntimeError, __import__, "shouldbeunimportable")
 
-    def test_waiting_during_different_thread_importing(self):
-        """
-        EventualResult.wait() should work if called while a module is
-        being imported in a different thread. See
-        EventualResultTests.test_noWaitingDuringImport for the explanation of
-        what should happen if an import is happening in the current thread.
-        """
-        test_complete = threading.Event()
-        lock_held = threading.Event()
-        er = EventualResult(succeed(123), None)
-
-        def other_thread():
-            imp.acquire_lock()
-            lock_held.set()
-            test_complete.wait()
-            imp.release_lock()
-
-        t = threading.Thread(target=other_thread)
-        t.start()
-        lock_held.wait()
-
-        # While the imp lock is held by the other thread, we can't
-        # allow exceptions/assertions to happen because trial will
-        # try to do an import causing a deadlock instead of a
-        # failure. We collect all assertion pairs (result, expected),
-        # wait for the import lock to be released, and then check our
-        # assertions at the end of the test.
-        assertions = []
-
-        # we want to run .wait while the other thread has the lock acquired
-        assertions.append((imp.lock_held(), True))
-        try:
-            assertions.append((er.wait(0.1), 123))
-        finally:
-            test_complete.set()
-
-        assertions.append((imp.lock_held(), True))
-
-        test_complete.set()
-
-        t.join()
-
-        [self.assertEqual(result, expected) for result, expected in assertions]
-
 
 class RunInReactorTests(TestCase):
     """
     Tests for the run_in_reactor decorator.
     """
 
     def test_signature(self):
@@ -1096,15 +1052,15 @@
         """
         An EventLoop object configured with the real reactor and
         _shutdown.register is exposed via its public methods.
         """
         from twisted.python.log import startLoggingWithObserver
         from crochet import _shutdown
         self.assertIsInstance(_main, EventLoop)
-        self.assertEqual(_main.setup, setup)
+        self.assertEqual(_main.setup, setup_crochet)
         self.assertEqual(_main.no_setup, no_setup)
         self.assertEqual(_main.run_in_reactor, run_in_reactor)
         self.assertEqual(_main.wait_for, wait_for)
         self.assertIdentical(_main._atexit_register, _shutdown.register)
         self.assertIdentical(
             _main._startLoggingWithObserver, startLoggingWithObserver)
         self.assertIdentical(_main._watchdog_thread, _shutdown._watchdog)
```

### Comparing `crochet-2.0.0/crochet/tests/test_logging.py` & `crochet-2.1.1/crochet/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/crochet/tests/test_mypy.py` & `crochet-2.1.1/crochet/tests/test_mypy.py`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/crochet/tests/test_process.py` & `crochet-2.1.1/crochet/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/crochet/tests/test_resultstore.py` & `crochet-2.1.1/crochet/tests/test_resultstore.py`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/crochet/tests/test_setup.py` & `crochet-2.1.1/crochet/tests/test_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,19 +254,19 @@
         reaps = []
         s = EventLoop(
             lambda: reactor,
             lambda f, *g: None,
             reapAllProcesses=lambda: reaps.append(1))
         s.setup()
         reactor.advance(0.1)
-        self.assertEquals(reaps, [1])
+        self.assertEqual(reaps, [1])
         reactor.advance(0.1)
-        self.assertEquals(reaps, [1, 1])
+        self.assertEqual(reaps, [1, 1])
         reactor.advance(0.1)
-        self.assertEquals(reaps, [1, 1, 1])
+        self.assertEqual(reaps, [1, 1, 1])
 
     def test_non_posix(self):
         """
         On non-POSIX systems, setup() does not install a LoopingCall.
         """
         if platform.type == "posix":
             raise SkipTest("This test is for non-POSIX systems.")
```

### Comparing `crochet-2.0.0/crochet/tests/test_shutdown.py` & `crochet-2.1.1/crochet/tests/test_shutdown.py`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/crochet/tests/test_util.py` & `crochet-2.1.1/crochet/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/crochet.egg-info/PKG-INFO` & `crochet-2.1.1/crochet.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,328 +1,333 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: crochet
-Version: 2.0.0
+Version: 2.1.1
 Summary: Use Twisted anywhere!
 Home-page: https://github.com/itamarst/crochet
 Maintainer: Itamar Turner-Trauring
 Maintainer-email: itamar@itamarst.org
 License: MIT
-Description: Crochet: Use Twisted anywhere!
-        ==============================
-        
-        Crochet is an MIT-licensed library that makes it easier to use Twisted from
-        regular blocking code. Some use cases include:
-        
-        * Easily use Twisted from a blocking framework like Django or Flask.
-        * Write a library that provides a blocking API, but uses Twisted for its
-          implementation.
-        * Port blocking code to Twisted more easily, by keeping a backwards
-          compatibility layer.
-        * Allow normal Twisted programs that use threads to interact with Twisted more
-          cleanly from their threaded parts. For example, this can be useful when using
-          Twisted as a `WSGI container`_.
-        
-        .. _WSGI container: https://twistedmatrix.com/documents/current/web/howto/web-in-60/wsgi.html
-        
-        Crochet is maintained by Itamar Turner-Trauring.
-        
-          **Note:** Crochet development is pretty slow these days because mostly it **Just Works**. PyPI shows about 30,000 downloads a month, so existing users seem happy: https://pypistats.org/packages/crochet
-        
-        You can install Crochet by running::
-        
-          $ pip install crochet
-        
-        Downloads are available on `PyPI`_.
-        
-        Documentation can be found on `Read The Docs`_.
-        
-        Bugs and feature requests should be filed at the project `Github page`_.
-        
-        .. _Read the Docs: https://crochet.readthedocs.org/
-        .. _Github page: https://github.com/itamarst/crochet/
-        .. _PyPI: https://pypi.python.org/pypi/crochet
-        
-        
-        API and features
-        ================
-        
-        Crochet supports Python 3.6, 3.7, 3.8, and 3.9 as well as PyPy3.
-        Python 2.7 and 3.5 support is available in older releases.
-        
-        Crochet provides the following basic APIs:
-        
-        * Allow blocking code to call into Twisted and block until results are available
-          or a timeout is hit, using the ``crochet.wait_for`` decorator.
-        * A lower-level API (``crochet.run_in_reactor``) allows blocking code to run
-          code "in the background" in the Twisted thread, with the ability to repeatedly
-          check if it's done.
-        
-        Crochet will do the following on your behalf in order to enable these APIs:
-        
-        * Transparently start Twisted's reactor in a thread it manages.
-        * Shut down the reactor automatically when the process' main thread finishes.
-        * Hook up Twisted's log system to the Python standard library ``logging``
-          framework. Unlike Twisted's built-in ``logging`` bridge, this includes
-          support for blocking `Handler` instances.
-        
-        What's New
-        ==========
-        
-        2.0.0
-        ^^^^^
-        
-        New features:
-        
-        * It's possible to decorate ``async/await`` Twisted functions with ``@wait_for`` and ``@run_in_reactor``, thanks to Árni Már Jónsson.
-        * Added type hints, thanks to Merlin Davis.
-        * Added formal support for Python 3.9.
-        
-        
-        Removed features:
-        
-        * Dropped the deprecated APIs ``@wait_for_reactor``, ``@in_reactor``, ``DeferredResult``, the ``wrapped_function`` attribute, and unlimited timeouts on ``EventualResult.wait()``.
-        * Dropped support for Python 2.7 and 3.5.
-        
-        1.12.0
-        ^^^^^^
-        
-        Bug fixes:
-        
-        * Fix a timeout overflow bug in 32-bit machines.
-        
-        
-        1.11.0
-        ^^^^^^
-        
-        New features:
-        
-        * Added support for Python 3.8 and PyPy 3.
-        
-        Backwards incompatibility:
-        
-        * Dropped support for Python 3.4, since latest Twisted doesn't support it.
-        
-        1.10.0
-        ^^^^^^
-        
-        New features:
-        
-        * Added support for Python 3.7. Thanks to Jeremy Cline for the patch.
-        
-        1.9.0
-        ^^^^^
-        
-        New features:
-        
-        * The underlying callable wrapped ``@run_in_reactor`` and ``@wait_for`` is now available via the more standard ``__wrapped__`` attribute.
-        
-        Backwards incompatibility (in tests):
-        
-        * This was actually introduced in 1.8.0: ``wrapped_function`` may not always be available on decorated callables.
-          You should use ``__wrapped__`` instead.
-        
-        Bug fixes:
-        
-        * Fixed regression in 1.8.0 where bound method couldn't be wrapped.
-          Thanks to 2mf for the bug report.
-        
-        1.8.0
-        ^^^^^
-        
-        New features:
-        
-        * Signatures on decorated functions now match the original functions.
-          Thanks to Mikhail Terekhov for the original patch.
-        * Documentation improvements, including an API reference.
-        
-        Bug fixes:
-        
-        * Switched to EPoll reactor for logging thread.
-          Anecdotal evidence suggests this fixes some issues on AWS Lambda, but it's not clear why.
-          Thanks to Rolando Espinoza for the patch.
-        * It's now possible to call ``@run_in_reactor`` and ``@wait_for`` above a ``@classmethod``.
-          Thanks to vak for the bug report.
-        
-        1.7.0
-        ^^^^^
-        
-        Bug fixes:
-        
-        * If the Python ``logging.Handler`` throws an exception Crochet no longer goes into a death spiral.
-          Thanks to Michael Schlenker for the bug report.
-        
-        Removed features:
-        
-        * Versions of Twisted < 16.0 are no longer supported (i.e. no longer tested in CI.)
-        
-        1.6.0
-        ^^^^^
-        
-        New features:
-        
-        * Added support for Python 3.6.
-        
-        1.5.0
-        ^^^^^
-        
-        New features:
-        
-        * Added support for Python 3.5.
-        
-        Removed features:
-        
-        * Python 2.6, Python 3.3, and versions of Twisted < 15.0 are no longer supported.
-        
-        1.4.0
-        ^^^^^
-        
-        New features:
-        
-        * Added support for Python 3.4.
-        
-        Documentation:
-        
-        * Added a section on known issues and workarounds.
-        
-        Bug fixes:
-        
-        * Main thread detection (used to determine when Crochet should shutdown) is now less fragile.
-          This means Crochet now supports more environments, e.g. uWSGI.
-          Thanks to Ben Picolo for the patch.
-        
-        1.3.0
-        ^^^^^
-        
-        Bug fixes:
-        
-        * It is now possible to call ``EventualResult.wait()`` (or functions
-          wrapped in ``wait_for``) at import time if another thread holds the
-          import lock. Thanks to Ken Struys for the patch.
-        
-        1.2.0
-        ^^^^^
-        New features:
-        
-        * ``crochet.wait_for`` implements the timeout/cancellation pattern documented
-          in previous versions of Crochet. ``crochet.wait_for_reactor`` and
-          ``EventualResult.wait(timeout=None)`` are now deprecated, since lacking
-          timeouts they could potentially block forever.
-        * Functions wrapped with ``wait_for`` and ``run_in_reactor`` can now be accessed
-          via the ``wrapped_function`` attribute, to ease unit testing of the underlying
-          Twisted code.
-        
-        API changes:
-        
-        * It is no longer possible to call ``EventualResult.wait()`` (or functions
-          wrapped with ``wait_for``) at import time, since this can lead to deadlocks
-          or prevent other threads from importing. Thanks to Tom Prince for the bug
-          report.
-        
-        Bug fixes:
-        
-        * ``warnings`` are no longer erroneously turned into Twisted log messages.
-        * The reactor is now only imported when ``crochet.setup()`` or
-          ``crochet.no_setup()`` are called, allowing daemonization if only ``crochet``
-          is imported (http://tm.tl/7105). Thanks to Daniel Nephin for the bug report.
-        
-        Documentation:
-        
-        * Improved motivation, added contact info and news to the documentation.
-        * Better example of using Crochet from a normal Twisted application.
-        
-        1.1.0
-        ^^^^^
-        Bug fixes:
-        
-        * ``EventualResult.wait()`` can now be used safely from multiple threads,
-          thanks to Gavin Panella for reporting the bug.
-        * Fixed reentrancy deadlock in the logging code caused by
-          http://bugs.python.org/issue14976, thanks to Rod Morehead for reporting the
-          bug.
-        * Crochet now installs on Python 3.3 again, thanks to Ben Cordero.
-        * Crochet should now work on Windows, thanks to Konstantinos Koukopoulos.
-        * Crochet tests can now run without adding its absolute path to PYTHONPATH or
-          installing it first.
-        
-        Documentation:
-        
-        * ``EventualResult.original_failure`` is now documented.
-        
-        1.0.0
-        ^^^^^
-        Documentation:
-        
-        * Added section on use cases and alternatives. Thanks to Tobias Oberstein for
-          the suggestion.
-        
-        Bug fixes:
-        
-        * Twisted does not have to be pre-installed to run ``setup.py``, thanks to
-          Paul Weaver for bug report and Chris Scutcher for patch.
-        * Importing Crochet does not have side-effects (installing reactor event)
-          any more.
-        * Blocking calls are interrupted earlier in the shutdown process, to reduce
-          scope for deadlocks. Thanks to rmorehead for bug report.
-        
-        0.9.0
-        ^^^^^
-        New features:
-        
-        * Expanded and much improved documentation, including a new section with
-          design suggestions.
-        * New decorator ``@wait_for_reactor`` added, a simpler alternative to
-          ``@run_in_reactor``.
-        * Refactored ``@run_in_reactor``, making it a bit more responsive.
-        * Blocking operations which would otherwise never finish due to reactor having
-          stopped (``EventualResult.wait()`` or ``@wait_for_reactor`` decorated call)
-          will be interrupted with a ``ReactorStopped`` exception. Thanks to rmorehead
-          for the bug report.
-        
-        Bug fixes:
-        
-        * ``@run_in_reactor`` decorated functions (or rather, their generated wrapper)
-          are interrupted by Ctrl-C.
-        * On POSIX platforms, a workaround is installed to ensure processes started by
-          `reactor.spawnProcess` have their exit noticed. See `Twisted ticket 6378`_
-          for more details about the underlying issue.
-        
-        .. _Twisted ticket 6378: http://tm.tl/6738
-        
-        0.8.1
-        ^^^^^
-        * ``EventualResult.wait()`` now raises error if called in the reactor thread,
-          thanks to David Buchmann.
-        * Unittests are now included in the release tarball.
-        * Allow Ctrl-C to interrupt ``EventualResult.wait(timeout=None)``.
-        
-        0.7.0
-        ^^^^^
-        * Improved documentation.
-        
-        0.6.0
-        ^^^^^
-        * Renamed ``DeferredResult`` to ``EventualResult``, to reduce confusion with
-          Twisted's ``Deferred`` class. The old name still works, but is deprecated.
-        * Deprecated ``@in_reactor``, replaced with ``@run_in_reactor`` which doesn't
-          change the arguments to the wrapped function. The deprecated API still works,
-          however.
-        * Unhandled exceptions in ``EventualResult`` objects are logged.
-        * Added more examples.
-        * ``setup.py sdist`` should work now.
-        
-        0.5.0
-        ^^^^^
-        * Initial release.
-        
 Keywords: twisted threading
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6.0
+Requires-Python: >=3.8.0
+License-File: LICENSE
+
+Crochet: Use Twisted anywhere!
+==============================
+
+Crochet is an MIT-licensed library that makes it easier to use Twisted from
+regular blocking code. Some use cases include:
+
+* Easily use Twisted from a blocking framework like Django or Flask.
+* Write a library that provides a blocking API, but uses Twisted for its
+  implementation.
+* Port blocking code to Twisted more easily, by keeping a backwards
+  compatibility layer.
+* Allow normal Twisted programs that use threads to interact with Twisted more
+  cleanly from their threaded parts. For example, this can be useful when using
+  Twisted as a `WSGI container`_.
+
+.. _WSGI container: https://twistedmatrix.com/documents/current/web/howto/web-in-60/wsgi.html
+
+Crochet is maintained by Itamar Turner-Trauring.
+
+  **Note:** Crochet development is pretty slow these days because mostly it **Just Works**. PyPI shows about 30,000 downloads a month, so existing users seem happy: https://pypistats.org/packages/crochet
+
+You can install Crochet by running::
+
+  $ pip install crochet
+
+Downloads are available on `PyPI`_.
+
+Documentation can be found on `Read The Docs`_.
+
+Bugs and feature requests should be filed at the project `Github page`_.
+
+.. _Read the Docs: https://crochet.readthedocs.org/
+.. _Github page: https://github.com/itamarst/crochet/
+.. _PyPI: https://pypi.python.org/pypi/crochet
+
+
+API and features
+================
+
+Crochet supports Python 3.8, 3.9, 3.10, and 3.11 as well as PyPy3.
+
+Crochet provides the following basic APIs:
+
+* Allow blocking code to call into Twisted and block until results are available
+  or a timeout is hit, using the ``crochet.wait_for`` decorator.
+* A lower-level API (``crochet.run_in_reactor``) allows blocking code to run
+  code "in the background" in the Twisted thread, with the ability to repeatedly
+  check if it's done.
+
+Crochet will do the following on your behalf in order to enable these APIs:
+
+* Transparently start Twisted's reactor in a thread it manages.
+* Shut down the reactor automatically when the process' main thread finishes.
+* Hook up Twisted's log system to the Python standard library ``logging``
+  framework. Unlike Twisted's built-in ``logging`` bridge, this includes
+  support for blocking `Handler` instances.
+
+What's New
+==========
+
+2.1.0
+^^^^^
+
+* Various internal modernizations and maintenance.
+* Dropped Python 3.6 and 3.7 support.
+
+2.0.0
+^^^^^
+
+New features:
+
+* It's possible to decorate ``async/await`` Twisted functions with ``@wait_for`` and ``@run_in_reactor``, thanks to Árni Már Jónsson.
+* Added type hints, thanks to Merlin Davis.
+* Added formal support for Python 3.9.
+
+
+Removed features:
+
+* Dropped the deprecated APIs ``@wait_for_reactor``, ``@in_reactor``, ``DeferredResult``, the ``wrapped_function`` attribute, and unlimited timeouts on ``EventualResult.wait()``.
+* Dropped support for Python 2.7 and 3.5.
+
+1.12.0
+^^^^^^
+
+Bug fixes:
+
+* Fix a timeout overflow bug in 32-bit machines.
+
+
+1.11.0
+^^^^^^
+
+New features:
+
+* Added support for Python 3.8 and PyPy 3.
+
+Backwards incompatibility:
+
+* Dropped support for Python 3.4, since latest Twisted doesn't support it.
+
+1.10.0
+^^^^^^
+
+New features:
+
+* Added support for Python 3.7. Thanks to Jeremy Cline for the patch.
+
+1.9.0
+^^^^^
+
+New features:
+
+* The underlying callable wrapped ``@run_in_reactor`` and ``@wait_for`` is now available via the more standard ``__wrapped__`` attribute.
+
+Backwards incompatibility (in tests):
+
+* This was actually introduced in 1.8.0: ``wrapped_function`` may not always be available on decorated callables.
+  You should use ``__wrapped__`` instead.
+
+Bug fixes:
+
+* Fixed regression in 1.8.0 where bound method couldn't be wrapped.
+  Thanks to 2mf for the bug report.
+
+1.8.0
+^^^^^
+
+New features:
+
+* Signatures on decorated functions now match the original functions.
+  Thanks to Mikhail Terekhov for the original patch.
+* Documentation improvements, including an API reference.
+
+Bug fixes:
+
+* Switched to EPoll reactor for logging thread.
+  Anecdotal evidence suggests this fixes some issues on AWS Lambda, but it's not clear why.
+  Thanks to Rolando Espinoza for the patch.
+* It's now possible to call ``@run_in_reactor`` and ``@wait_for`` above a ``@classmethod``.
+  Thanks to vak for the bug report.
+
+1.7.0
+^^^^^
+
+Bug fixes:
+
+* If the Python ``logging.Handler`` throws an exception Crochet no longer goes into a death spiral.
+  Thanks to Michael Schlenker for the bug report.
+
+Removed features:
+
+* Versions of Twisted < 16.0 are no longer supported (i.e. no longer tested in CI.)
+
+1.6.0
+^^^^^
+
+New features:
+
+* Added support for Python 3.6.
+
+1.5.0
+^^^^^
+
+New features:
+
+* Added support for Python 3.5.
+
+Removed features:
+
+* Python 2.6, Python 3.3, and versions of Twisted < 15.0 are no longer supported.
+
+1.4.0
+^^^^^
+
+New features:
+
+* Added support for Python 3.4.
+
+Documentation:
+
+* Added a section on known issues and workarounds.
+
+Bug fixes:
+
+* Main thread detection (used to determine when Crochet should shutdown) is now less fragile.
+  This means Crochet now supports more environments, e.g. uWSGI.
+  Thanks to Ben Picolo for the patch.
+
+1.3.0
+^^^^^
+
+Bug fixes:
+
+* It is now possible to call ``EventualResult.wait()`` (or functions
+  wrapped in ``wait_for``) at import time if another thread holds the
+  import lock. Thanks to Ken Struys for the patch.
+
+1.2.0
+^^^^^
+New features:
+
+* ``crochet.wait_for`` implements the timeout/cancellation pattern documented
+  in previous versions of Crochet. ``crochet.wait_for_reactor`` and
+  ``EventualResult.wait(timeout=None)`` are now deprecated, since lacking
+  timeouts they could potentially block forever.
+* Functions wrapped with ``wait_for`` and ``run_in_reactor`` can now be accessed
+  via the ``wrapped_function`` attribute, to ease unit testing of the underlying
+  Twisted code.
+
+API changes:
+
+* It is no longer possible to call ``EventualResult.wait()`` (or functions
+  wrapped with ``wait_for``) at import time, since this can lead to deadlocks
+  or prevent other threads from importing. Thanks to Tom Prince for the bug
+  report.
+
+Bug fixes:
+
+* ``warnings`` are no longer erroneously turned into Twisted log messages.
+* The reactor is now only imported when ``crochet.setup()`` or
+  ``crochet.no_setup()`` are called, allowing daemonization if only ``crochet``
+  is imported (http://tm.tl/7105). Thanks to Daniel Nephin for the bug report.
+
+Documentation:
+
+* Improved motivation, added contact info and news to the documentation.
+* Better example of using Crochet from a normal Twisted application.
+
+1.1.0
+^^^^^
+Bug fixes:
+
+* ``EventualResult.wait()`` can now be used safely from multiple threads,
+  thanks to Gavin Panella for reporting the bug.
+* Fixed reentrancy deadlock in the logging code caused by
+  http://bugs.python.org/issue14976, thanks to Rod Morehead for reporting the
+  bug.
+* Crochet now installs on Python 3.3 again, thanks to Ben Cordero.
+* Crochet should now work on Windows, thanks to Konstantinos Koukopoulos.
+* Crochet tests can now run without adding its absolute path to PYTHONPATH or
+  installing it first.
+
+Documentation:
+
+* ``EventualResult.original_failure`` is now documented.
+
+1.0.0
+^^^^^
+Documentation:
+
+* Added section on use cases and alternatives. Thanks to Tobias Oberstein for
+  the suggestion.
+
+Bug fixes:
+
+* Twisted does not have to be pre-installed to run ``setup.py``, thanks to
+  Paul Weaver for bug report and Chris Scutcher for patch.
+* Importing Crochet does not have side-effects (installing reactor event)
+  any more.
+* Blocking calls are interrupted earlier in the shutdown process, to reduce
+  scope for deadlocks. Thanks to rmorehead for bug report.
+
+0.9.0
+^^^^^
+New features:
+
+* Expanded and much improved documentation, including a new section with
+  design suggestions.
+* New decorator ``@wait_for_reactor`` added, a simpler alternative to
+  ``@run_in_reactor``.
+* Refactored ``@run_in_reactor``, making it a bit more responsive.
+* Blocking operations which would otherwise never finish due to reactor having
+  stopped (``EventualResult.wait()`` or ``@wait_for_reactor`` decorated call)
+  will be interrupted with a ``ReactorStopped`` exception. Thanks to rmorehead
+  for the bug report.
+
+Bug fixes:
+
+* ``@run_in_reactor`` decorated functions (or rather, their generated wrapper)
+  are interrupted by Ctrl-C.
+* On POSIX platforms, a workaround is installed to ensure processes started by
+  `reactor.spawnProcess` have their exit noticed. See `Twisted ticket 6378`_
+  for more details about the underlying issue.
+
+.. _Twisted ticket 6378: http://tm.tl/6738
+
+0.8.1
+^^^^^
+* ``EventualResult.wait()`` now raises error if called in the reactor thread,
+  thanks to David Buchmann.
+* Unittests are now included in the release tarball.
+* Allow Ctrl-C to interrupt ``EventualResult.wait(timeout=None)``.
+
+0.7.0
+^^^^^
+* Improved documentation.
+
+0.6.0
+^^^^^
+* Renamed ``DeferredResult`` to ``EventualResult``, to reduce confusion with
+  Twisted's ``Deferred`` class. The old name still works, but is deprecated.
+* Deprecated ``@in_reactor``, replaced with ``@run_in_reactor`` which doesn't
+  change the arguments to the wrapped function. The deprecated API still works,
+  however.
+* Unhandled exceptions in ``EventualResult`` objects are logged.
+* Added more examples.
+* ``setup.py sdist`` should work now.
+
+0.5.0
+^^^^^
+* Initial release.
```

### Comparing `crochet-2.0.0/crochet.egg-info/SOURCES.txt` & `crochet-2.1.1/crochet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/docs/Makefile` & `crochet-2.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/docs/api.rst` & `crochet-2.1.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/docs/async.rst` & `crochet-2.1.1/docs/async.rst`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/docs/conf.py` & `crochet-2.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/docs/index.rst` & `crochet-2.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/docs/introduction.rst` & `crochet-2.1.1/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/docs/make.bat` & `crochet-2.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/docs/news.rst` & `crochet-2.1.1/docs/news.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 What's New
 ==========
 
+2.1.0
+^^^^^
+
+* Various internal modernizations and maintenance.
+* Dropped Python 3.6 and 3.7 support.
+
 2.0.0
 ^^^^^
 
 New features:
 
 * It's possible to decorate ``async/await`` Twisted functions with ``@wait_for`` and ``@run_in_reactor``, thanks to Árni Már Jónsson.
 * Added type hints, thanks to Merlin Davis.
```

### Comparing `crochet-2.0.0/docs/type-checking.rst` & `crochet-2.1.1/docs/type-checking.rst`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/docs/using.rst` & `crochet-2.1.1/docs/using.rst`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/docs/workarounds.rst` & `crochet-2.1.1/docs/workarounds.rst`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/examples/async.py` & `crochet-2.1.1/examples/async.py`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/examples/blockingdns.py` & `crochet-2.1.1/examples/blockingdns.py`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/examples/downloader.py` & `crochet-2.1.1/examples/downloader.py`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/examples/fromtwisted.py` & `crochet-2.1.1/examples/fromtwisted.py`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/examples/mxquery.py` & `crochet-2.1.1/examples/mxquery.py`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/examples/scheduling.py` & `crochet-2.1.1/examples/scheduling.py`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/examples/ssh.py` & `crochet-2.1.1/examples/ssh.py`

 * *Files identical despite different names*

### Comparing `crochet-2.0.0/setup.py` & `crochet-2.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,26 +16,26 @@
 
 setup(
     classifiers=[
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
     ],
     name='crochet',
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     description="Use Twisted anywhere!",
-    python_requires=">=3.6.0",
+    python_requires=">=3.8.0",
     install_requires=[
         "Twisted>=16.0",
         "wrapt",
     ],
     keywords="twisted threading",
     license="MIT",
     package_data={"crochet": ["py.typed", "*.pyi"]},
```

### Comparing `crochet-2.0.0/versioneer.py` & `crochet-2.1.1/versioneer.py`

 * *Files identical despite different names*

