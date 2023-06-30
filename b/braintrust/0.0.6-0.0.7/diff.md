# Comparing `tmp/braintrust-0.0.6.tar.gz` & `tmp/braintrust-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braintrust-0.0.6.tar", last modified: Thu Jun 22 22:13:35 2023, max compression
+gzip compressed data, was "braintrust-0.0.7.tar", last modified: Fri Jun 30 23:15:39 2023, max compression
```

## Comparing `braintrust-0.0.6.tar` & `braintrust-0.0.7.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-22 22:13:35.238494 braintrust-0.0.6/
--rw-r--r--   0 ankur      (501) staff       (20)      483 2023-06-22 22:13:35.238348 braintrust-0.0.6/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)       49 2023-04-02 02:49:19.000000 braintrust-0.0.6/README.md
--rw-r--r--   0 ankur      (501) staff       (20)       38 2023-06-22 22:13:35.238539 braintrust-0.0.6/setup.cfg
--rw-r--r--   0 ankur      (501) staff       (20)     1623 2023-06-21 20:59:50.000000 braintrust-0.0.6/setup.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-22 22:13:35.234596 braintrust-0.0.6/src/
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-22 22:13:35.236592 braintrust-0.0.6/src/braintrust/
--rw-r--r--   0 ankur      (501) staff       (20)    19765 2023-06-22 22:10:44.000000 braintrust-0.0.6/src/braintrust/__init__.py
--rw-r--r--   0 ankur      (501) staff       (20)      427 2023-06-21 20:59:50.000000 braintrust-0.0.6/src/braintrust/aws.py
--rw-r--r--   0 ankur      (501) staff       (20)      125 2023-06-22 22:10:44.000000 braintrust-0.0.6/src/braintrust/cache.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-22 22:13:35.237510 braintrust-0.0.6/src/braintrust/cli/
--rw-r--r--   0 ankur      (501) staff       (20)        0 2023-06-21 20:59:50.000000 braintrust-0.0.6/src/braintrust/cli/__init__.py
--rw-r--r--   0 ankur      (501) staff       (20)     1406 2023-06-21 20:59:50.000000 braintrust-0.0.6/src/braintrust/cli/__main__.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-22 22:13:35.238147 braintrust-0.0.6/src/braintrust/cli/install/
--rw-r--r--   0 ankur      (501) staff       (20)      472 2023-06-21 20:59:50.000000 braintrust-0.0.6/src/braintrust/cli/install/__init__.py
--rw-r--r--   0 ankur      (501) staff       (20)     8207 2023-06-21 20:59:50.000000 braintrust-0.0.6/src/braintrust/cli/install/api.py
--rw-r--r--   0 ankur      (501) staff       (20)     6421 2023-06-21 20:59:50.000000 braintrust-0.0.6/src/braintrust/cli/install/redshift.py
--rw-r--r--   0 ankur      (501) staff       (20)      811 2023-04-15 21:46:41.000000 braintrust-0.0.6/src/braintrust/oai.py
--rw-r--r--   0 ankur      (501) staff       (20)       18 2023-06-22 22:11:17.000000 braintrust-0.0.6/src/braintrust/version.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-22 22:13:35.237308 braintrust-0.0.6/src/braintrust.egg-info/
--rw-r--r--   0 ankur      (501) staff       (20)      483 2023-06-22 22:13:35.000000 braintrust-0.0.6/src/braintrust.egg-info/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)      543 2023-06-22 22:13:35.000000 braintrust-0.0.6/src/braintrust.egg-info/SOURCES.txt
--rw-r--r--   0 ankur      (501) staff       (20)        1 2023-06-22 22:13:35.000000 braintrust-0.0.6/src/braintrust.egg-info/dependency_links.txt
--rw-r--r--   0 ankur      (501) staff       (20)       60 2023-06-22 22:13:35.000000 braintrust-0.0.6/src/braintrust.egg-info/entry_points.txt
--rw-r--r--   0 ankur      (501) staff       (20)      302 2023-06-22 22:13:35.000000 braintrust-0.0.6/src/braintrust.egg-info/requires.txt
--rw-r--r--   0 ankur      (501) staff       (20)       11 2023-06-22 22:13:35.000000 braintrust-0.0.6/src/braintrust.egg-info/top_level.txt
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:15:39.478192 braintrust-0.0.7/
+-rw-r--r--   0 ankur      (501) staff       (20)      483 2023-06-30 23:15:39.478017 braintrust-0.0.7/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)       49 2023-04-02 02:49:19.000000 braintrust-0.0.7/README.md
+-rw-r--r--   0 ankur      (501) staff       (20)       38 2023-06-30 23:15:39.478246 braintrust-0.0.7/setup.cfg
+-rw-r--r--   0 ankur      (501) staff       (20)     1640 2023-06-30 23:03:25.000000 braintrust-0.0.7/setup.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:15:39.473242 braintrust-0.0.7/src/
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:15:39.475991 braintrust-0.0.7/src/braintrust/
+-rw-r--r--   0 ankur      (501) staff       (20)    35300 2023-06-30 23:03:25.000000 braintrust-0.0.7/src/braintrust/__init__.py
+-rw-r--r--   0 ankur      (501) staff       (20)      427 2023-06-22 23:54:28.000000 braintrust-0.0.7/src/braintrust/aws.py
+-rw-r--r--   0 ankur      (501) staff       (20)      171 2023-06-30 23:03:25.000000 braintrust-0.0.7/src/braintrust/cache.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:15:39.477049 braintrust-0.0.7/src/braintrust/cli/
+-rw-r--r--   0 ankur      (501) staff       (20)        0 2023-06-22 23:54:28.000000 braintrust-0.0.7/src/braintrust/cli/__init__.py
+-rw-r--r--   0 ankur      (501) staff       (20)     1406 2023-06-22 23:54:28.000000 braintrust-0.0.7/src/braintrust/cli/__main__.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:15:39.477754 braintrust-0.0.7/src/braintrust/cli/install/
+-rw-r--r--   0 ankur      (501) staff       (20)      472 2023-06-22 23:54:28.000000 braintrust-0.0.7/src/braintrust/cli/install/__init__.py
+-rw-r--r--   0 ankur      (501) staff       (20)     8207 2023-06-22 23:54:28.000000 braintrust-0.0.7/src/braintrust/cli/install/api.py
+-rw-r--r--   0 ankur      (501) staff       (20)     6421 2023-06-22 23:54:28.000000 braintrust-0.0.7/src/braintrust/cli/install/redshift.py
+-rw-r--r--   0 ankur      (501) staff       (20)      399 2023-06-30 23:03:25.000000 braintrust-0.0.7/src/braintrust/duckutil.py
+-rw-r--r--   0 ankur      (501) staff       (20)     2878 2023-06-30 23:03:25.000000 braintrust-0.0.7/src/braintrust/gitutil.py
+-rw-r--r--   0 ankur      (501) staff       (20)      811 2023-04-15 21:46:41.000000 braintrust-0.0.7/src/braintrust/oai.py
+-rw-r--r--   0 ankur      (501) staff       (20)      307 2023-06-30 23:03:25.000000 braintrust-0.0.7/src/braintrust/util.py
+-rw-r--r--   0 ankur      (501) staff       (20)       18 2023-06-30 23:15:16.000000 braintrust-0.0.7/src/braintrust/version.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:15:39.476824 braintrust-0.0.7/src/braintrust.egg-info/
+-rw-r--r--   0 ankur      (501) staff       (20)      483 2023-06-30 23:15:39.000000 braintrust-0.0.7/src/braintrust.egg-info/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)      619 2023-06-30 23:15:39.000000 braintrust-0.0.7/src/braintrust.egg-info/SOURCES.txt
+-rw-r--r--   0 ankur      (501) staff       (20)        1 2023-06-30 23:15:39.000000 braintrust-0.0.7/src/braintrust.egg-info/dependency_links.txt
+-rw-r--r--   0 ankur      (501) staff       (20)       60 2023-06-30 23:15:39.000000 braintrust-0.0.7/src/braintrust.egg-info/entry_points.txt
+-rw-r--r--   0 ankur      (501) staff       (20)      316 2023-06-30 23:15:39.000000 braintrust-0.0.7/src/braintrust.egg-info/requires.txt
+-rw-r--r--   0 ankur      (501) staff       (20)       11 2023-06-30 23:15:39.000000 braintrust-0.0.7/src/braintrust.egg-info/top_level.txt
```

### Comparing `braintrust-0.0.6/setup.py` & `braintrust-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 version_contents = {}
 with open(os.path.join(dir_name, "src", "braintrust", "version.py"), encoding="utf-8") as f:
     exec(f.read(), version_contents)
 
 with open(os.path.join(dir_name, "README.md"), "r", encoding="utf-8") as f:
     long_description = f.read()
 
-install_requires = ["openai", "GitPython", "requests"]
+install_requires = ["duckdb==0.8.1", "openai", "GitPython", "requests"]
 
 extras_require = {
     "cli": ["boto3", "psycopg2-binary"],
     "dev": [
         "black",
         "build",
         "flake8",
```

### Comparing `braintrust-0.0.6/src/braintrust/cli/__main__.py` & `braintrust-0.0.7/src/braintrust/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.6/src/braintrust/cli/install/api.py` & `braintrust-0.0.7/src/braintrust/cli/install/api.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.6/src/braintrust/cli/install/redshift.py` & `braintrust-0.0.7/src/braintrust/cli/install/redshift.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.6/src/braintrust/oai.py` & `braintrust-0.0.7/src/braintrust/oai.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.6/src/braintrust.egg-info/SOURCES.txt` & `braintrust-0.0.7/src/braintrust.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 README.md
 setup.py
 src/braintrust/__init__.py
 src/braintrust/aws.py
 src/braintrust/cache.py
+src/braintrust/duckutil.py
+src/braintrust/gitutil.py
 src/braintrust/oai.py
+src/braintrust/util.py
 src/braintrust/version.py
 src/braintrust.egg-info/PKG-INFO
 src/braintrust.egg-info/SOURCES.txt
 src/braintrust.egg-info/dependency_links.txt
 src/braintrust.egg-info/entry_points.txt
 src/braintrust.egg-info/requires.txt
 src/braintrust.egg-info/top_level.txt
```

