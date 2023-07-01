# Comparing `tmp/nopasaran-0.2.1.tar.gz` & `tmp/nopasaran-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nopasaran-0.2.1.tar", last modified: Sat Jul  1 11:31:09 2023, max compression
+gzip compressed data, was "nopasaran-0.2.2.tar", last modified: Sat Jul  1 13:05:38 2023, max compression
```

## Comparing `nopasaran-0.2.1.tar` & `nopasaran-0.2.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:31:09.807741 nopasaran-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 11:30:50.000000 nopasaran-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-07-01 11:31:09.807741 nopasaran-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-01 11:30:50.000000 nopasaran-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:31:09.803741 nopasaran-0.2.1/nopasaran/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 11:30:50.000000 nopasaran-0.2.1/nopasaran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-01 11:30:50.000000 nopasaran-0.2.1/nopasaran/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:31:09.807741 nopasaran-0.2.1/nopasaran/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 11:30:50.000000 nopasaran-0.2.1/nopasaran/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-01 11:30:50.000000 nopasaran-0.2.1/nopasaran/controllers/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-01 11:30:50.000000 nopasaran-0.2.1/nopasaran/controllers/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-01 11:30:50.000000 nopasaran-0.2.1/nopasaran/controllers/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-01 11:30:50.000000 nopasaran-0.2.1/nopasaran/controllers/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:31:09.807741 nopasaran-0.2.1/nopasaran/interpreters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 11:30:50.000000 nopasaran-0.2.1/nopasaran/interpreters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-07-01 11:30:50.000000 nopasaran-0.2.1/nopasaran/interpreters/action_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-07-01 11:30:50.000000 nopasaran-0.2.1/nopasaran/interpreters/condition_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-01 11:30:50.000000 nopasaran-0.2.1/nopasaran/interpreters/transition_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:31:09.807741 nopasaran-0.2.1/nopasaran/ipsec_tunnels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 11:30:50.000000 nopasaran-0.2.1/nopasaran/ipsec_tunnels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-01 11:30:50.000000 nopasaran-0.2.1/nopasaran/ipsec_tunnels/ipsec_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:31:09.807741 nopasaran-0.2.1/nopasaran/machines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 11:30:50.000000 nopasaran-0.2.1/nopasaran/machines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-01 11:30:50.000000 nopasaran-0.2.1/nopasaran/machines/machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:31:09.807741 nopasaran-0.2.1/nopasaran/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 11:30:50.000000 nopasaran-0.2.1/nopasaran/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-01 11:30:50.000000 nopasaran-0.2.1/nopasaran/parsers/interpreter_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:31:09.807741 nopasaran-0.2.1/nopasaran/sniffers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 11:30:50.000000 nopasaran-0.2.1/nopasaran/sniffers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-01 11:30:50.000000 nopasaran-0.2.1/nopasaran/sniffers/sniffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-01 11:30:50.000000 nopasaran-0.2.1/nopasaran/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:31:09.807741 nopasaran-0.2.1/nopasaran.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-07-01 11:31:09.000000 nopasaran-0.2.1/nopasaran.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-01 11:31:09.000000 nopasaran-0.2.1/nopasaran.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 11:31:09.000000 nopasaran-0.2.1/nopasaran.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-01 11:31:09.000000 nopasaran-0.2.1/nopasaran.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-01 11:31:09.000000 nopasaran-0.2.1/nopasaran.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-01 11:31:09.000000 nopasaran-0.2.1/nopasaran.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 11:31:09.807741 nopasaran-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-01 11:31:09.000000 nopasaran-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:31:09.807741 nopasaran-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 11:30:50.000000 nopasaran-0.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:38.731066 nopasaran-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 13:05:29.000000 nopasaran-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-07-01 13:05:38.727066 nopasaran-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-01 13:05:29.000000 nopasaran-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:38.723066 nopasaran-0.2.2/nopasaran/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:38.727066 nopasaran-0.2.2/nopasaran/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/controllers/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/controllers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/controllers/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/controllers/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:38.727066 nopasaran-0.2.2/nopasaran/interpreters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/interpreters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/interpreters/action_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/interpreters/condition_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/interpreters/transition_interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:38.727066 nopasaran-0.2.2/nopasaran/ipsec_tunnels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/ipsec_tunnels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/ipsec_tunnels/ipsec_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:38.727066 nopasaran-0.2.2/nopasaran/machines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/machines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/machines/machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:38.727066 nopasaran-0.2.2/nopasaran/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/parsers/interpreter_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:38.727066 nopasaran-0.2.2/nopasaran/sniffers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/sniffers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/sniffers/sniffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-01 13:05:29.000000 nopasaran-0.2.2/nopasaran/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:38.727066 nopasaran-0.2.2/nopasaran.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-07-01 13:05:38.000000 nopasaran-0.2.2/nopasaran.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-01 13:05:38.000000 nopasaran-0.2.2/nopasaran.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 13:05:38.000000 nopasaran-0.2.2/nopasaran.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-01 13:05:38.000000 nopasaran-0.2.2/nopasaran.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-01 13:05:38.000000 nopasaran-0.2.2/nopasaran.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-01 13:05:38.000000 nopasaran-0.2.2/nopasaran.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 13:05:38.731066 nopasaran-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-01 13:05:37.000000 nopasaran-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:38.727066 nopasaran-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:05:29.000000 nopasaran-0.2.2/tests/__init__.py
```

### Comparing `nopasaran-0.2.1/LICENSE` & `nopasaran-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.1/PKG-INFO` & `nopasaran-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopasaran
-Version: 0.2.1
+Version: 0.2.2
 Summary: NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.
 Home-page: https://github.com/BenIlies/NoPASARAN
 Author: Ilies Benhabbour
 Author-email: ilies.benhabbour@kaust.edu.sa
 License: UNKNOWN
 Description: # NoPASARAN
```

### Comparing `nopasaran-0.2.1/README.md` & `nopasaran-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.1/nopasaran/__main__.py` & `nopasaran-0.2.2/nopasaran/__main__.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.1/nopasaran/controllers/controller.py` & `nopasaran-0.2.2/nopasaran/controllers/controller.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.1/nopasaran/controllers/factory.py` & `nopasaran-0.2.2/nopasaran/controllers/factory.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.1/nopasaran/controllers/protocol.py` & `nopasaran-0.2.2/nopasaran/controllers/protocol.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.1/nopasaran/interpreters/action_interpreter.py` & `nopasaran-0.2.2/nopasaran/interpreters/action_interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.1/nopasaran/interpreters/condition_interpreter.py` & `nopasaran-0.2.2/nopasaran/interpreters/condition_interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.1/nopasaran/interpreters/transition_interpreter.py` & `nopasaran-0.2.2/nopasaran/interpreters/transition_interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.1/nopasaran/ipsec_tunnels/ipsec_conf.py` & `nopasaran-0.2.2/nopasaran/ipsec_tunnels/ipsec_conf.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.1/nopasaran/machines/machine.py` & `nopasaran-0.2.2/nopasaran/machines/machine.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.1/nopasaran/parsers/interpreter_parser.py` & `nopasaran-0.2.2/nopasaran/parsers/interpreter_parser.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.1/nopasaran/sniffers/sniffer.py` & `nopasaran-0.2.2/nopasaran/sniffers/sniffer.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.1/nopasaran/utils.py` & `nopasaran-0.2.2/nopasaran/utils.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.1/nopasaran.egg-info/PKG-INFO` & `nopasaran-0.2.2/nopasaran.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopasaran
-Version: 0.2.1
+Version: 0.2.2
 Summary: NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.
 Home-page: https://github.com/BenIlies/NoPASARAN
 Author: Ilies Benhabbour
 Author-email: ilies.benhabbour@kaust.edu.sa
 License: UNKNOWN
 Description: # NoPASARAN
```

### Comparing `nopasaran-0.2.1/nopasaran.egg-info/SOURCES.txt` & `nopasaran-0.2.2/nopasaran.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.1/setup.py` & `nopasaran-0.2.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,17 +6,18 @@
     long_description = fh.read()
 
 # Read requirements from requirements.txt file
 requirements_file = os.path.join(os.path.dirname(__file__), "requirements.txt")
 with open(requirements_file, "r") as f:
     requirements = [str(req) for req in parse_requirements(f)]
 
+# Version will automatically be updated when pushed on the main branch
 setup(
     name="nopasaran",
-    version="0.2.1",
+    version='0.2.2',
     author="Ilies Benhabbour",
     author_email="ilies.benhabbour@kaust.edu.sa",
     description="NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BenIlies/NoPASARAN",
     packages=find_packages(),
@@ -28,8 +29,8 @@
     python_requires=">=3.8",
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'nopasaran = nopasaran.__main__:main'
         ]
     }
-)
+)
```

