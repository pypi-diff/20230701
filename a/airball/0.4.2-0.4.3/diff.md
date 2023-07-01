# Comparing `tmp/airball-0.4.2.tar.gz` & `tmp/airball-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airball-0.4.2.tar", last modified: Fri Jun 30 08:24:13 2023, max compression
+gzip compressed data, was "airball-0.4.3.tar", last modified: Sat Jul  1 04:49:16 2023, max compression
```

## Comparing `airball-0.4.2.tar` & `airball-0.4.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-06-30 08:24:13.230597 airball-0.4.2/
--rw-r--r--   0 zyrxvo     (501) staff       (20)    35149 2022-05-02 19:30:08.000000 airball-0.4.2/LICENSE
--rw-r--r--   0 zyrxvo     (501) staff       (20)     1023 2023-06-30 08:24:13.230480 airball-0.4.2/PKG-INFO
--rw-r--r--   0 zyrxvo     (501) staff       (20)      472 2023-02-16 19:20:04.000000 airball-0.4.2/README.md
--rw-r--r--   0 zyrxvo     (501) staff       (20)       85 2022-06-02 19:07:19.000000 airball-0.4.2/pyproject.toml
--rw-r--r--   0 zyrxvo     (501) staff       (20)       38 2023-06-30 08:24:13.230638 airball-0.4.2/setup.cfg
--rw-r--r--   0 zyrxvo     (501) staff       (20)      922 2023-06-30 08:22:52.000000 airball-0.4.2/setup.py
-drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-06-30 08:24:13.227773 airball-0.4.2/src/
-drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-06-30 08:24:13.229484 airball-0.4.2/src/airball/
--rw-r--r--   0 zyrxvo     (501) staff       (20)      334 2023-06-30 08:23:00.000000 airball-0.4.2/src/airball/__init__.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)     9107 2023-06-30 08:21:41.000000 airball-0.4.2/src/airball/analytic.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)    14527 2023-06-30 08:16:39.000000 airball-0.4.2/src/airball/environments.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)    11157 2023-06-29 08:34:54.000000 airball-0.4.2/src/airball/flybys.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)     7787 2023-06-30 07:51:03.000000 airball-0.4.2/src/airball/imf.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)    15000 2023-02-09 02:16:12.000000 airball-0.4.2/src/airball/particle.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)    21713 2023-06-30 06:28:22.000000 airball-0.4.2/src/airball/stars.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)     8774 2023-06-30 08:05:48.000000 airball-0.4.2/src/airball/tools.py
--rw-r--r--   0 zyrxvo     (501) staff       (20)      181 2023-06-29 01:38:57.000000 airball-0.4.2/src/airball/units.py
-drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-06-30 08:24:13.230320 airball-0.4.2/src/airball.egg-info/
--rw-r--r--   0 zyrxvo     (501) staff       (20)     1023 2023-06-30 08:24:13.000000 airball-0.4.2/src/airball.egg-info/PKG-INFO
--rw-r--r--   0 zyrxvo     (501) staff       (20)      419 2023-06-30 08:24:13.000000 airball-0.4.2/src/airball.egg-info/SOURCES.txt
--rw-r--r--   0 zyrxvo     (501) staff       (20)        1 2023-06-30 08:24:13.000000 airball-0.4.2/src/airball.egg-info/dependency_links.txt
--rw-r--r--   0 zyrxvo     (501) staff       (20)       35 2023-06-30 08:24:13.000000 airball-0.4.2/src/airball.egg-info/requires.txt
--rw-r--r--   0 zyrxvo     (501) staff       (20)        8 2023-06-30 08:24:13.000000 airball-0.4.2/src/airball.egg-info/top_level.txt
+drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-07-01 04:49:16.175901 airball-0.4.3/
+-rw-r--r--   0 zyrxvo     (501) staff       (20)    35149 2022-05-02 19:30:08.000000 airball-0.4.3/LICENSE
+-rw-r--r--   0 zyrxvo     (501) staff       (20)     2919 2023-07-01 04:49:16.175752 airball-0.4.3/PKG-INFO
+-rw-r--r--   0 zyrxvo     (501) staff       (20)     2368 2023-07-01 04:45:58.000000 airball-0.4.3/README.md
+-rw-r--r--   0 zyrxvo     (501) staff       (20)       85 2022-06-02 19:07:19.000000 airball-0.4.3/pyproject.toml
+-rw-r--r--   0 zyrxvo     (501) staff       (20)       38 2023-07-01 04:49:16.175961 airball-0.4.3/setup.cfg
+-rw-r--r--   0 zyrxvo     (501) staff       (20)      922 2023-07-01 04:48:58.000000 airball-0.4.3/setup.py
+drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-07-01 04:49:16.172818 airball-0.4.3/src/
+drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-07-01 04:49:16.174527 airball-0.4.3/src/airball/
+-rw-r--r--   0 zyrxvo     (501) staff       (20)      334 2023-07-01 04:49:03.000000 airball-0.4.3/src/airball/__init__.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)     9107 2023-07-01 04:32:22.000000 airball-0.4.3/src/airball/analytic.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)    14527 2023-06-30 08:16:39.000000 airball-0.4.3/src/airball/environments.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)    11157 2023-06-29 08:34:54.000000 airball-0.4.3/src/airball/flybys.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)     7787 2023-06-30 07:51:03.000000 airball-0.4.3/src/airball/imf.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)    15000 2023-02-09 02:16:12.000000 airball-0.4.3/src/airball/particle.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)    21713 2023-06-30 06:28:22.000000 airball-0.4.3/src/airball/stars.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)     8774 2023-06-30 08:05:48.000000 airball-0.4.3/src/airball/tools.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)      181 2023-06-29 01:38:57.000000 airball-0.4.3/src/airball/units.py
+drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2023-07-01 04:49:16.175258 airball-0.4.3/src/airball.egg-info/
+-rw-r--r--   0 zyrxvo     (501) staff       (20)     2919 2023-07-01 04:49:16.000000 airball-0.4.3/src/airball.egg-info/PKG-INFO
+-rw-r--r--   0 zyrxvo     (501) staff       (20)      419 2023-07-01 04:49:16.000000 airball-0.4.3/src/airball.egg-info/SOURCES.txt
+-rw-r--r--   0 zyrxvo     (501) staff       (20)        1 2023-07-01 04:49:16.000000 airball-0.4.3/src/airball.egg-info/dependency_links.txt
+-rw-r--r--   0 zyrxvo     (501) staff       (20)       35 2023-07-01 04:49:16.000000 airball-0.4.3/src/airball.egg-info/requires.txt
+-rw-r--r--   0 zyrxvo     (501) staff       (20)        8 2023-07-01 04:49:16.000000 airball-0.4.3/src/airball.egg-info/top_level.txt
```

### Comparing `airball-0.4.2/LICENSE` & `airball-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `airball-0.4.2/setup.py` & `airball-0.4.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="airball",
-    version="0.4.2",
+    version="0.4.3",
     author="Garett Brown",
     author_email="garett.brown@mail.utoronto.ca",
     description="A package for implementing flybys in hannorein/rebound",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zyrxvo/airball/",
     project_urls={
```

### Comparing `airball-0.4.2/src/airball/analytic.py` & `airball-0.4.3/src/airball/analytic.py`

 * *Files identical despite different names*

### Comparing `airball-0.4.2/src/airball/environments.py` & `airball-0.4.3/src/airball/environments.py`

 * *Files identical despite different names*

### Comparing `airball-0.4.2/src/airball/flybys.py` & `airball-0.4.3/src/airball/flybys.py`

 * *Files identical despite different names*

### Comparing `airball-0.4.2/src/airball/imf.py` & `airball-0.4.3/src/airball/imf.py`

 * *Files identical despite different names*

### Comparing `airball-0.4.2/src/airball/particle.py` & `airball-0.4.3/src/airball/particle.py`

 * *Files identical despite different names*

### Comparing `airball-0.4.2/src/airball/stars.py` & `airball-0.4.3/src/airball/stars.py`

 * *Files identical despite different names*

### Comparing `airball-0.4.2/src/airball/tools.py` & `airball-0.4.3/src/airball/tools.py`

 * *Files identical despite different names*

