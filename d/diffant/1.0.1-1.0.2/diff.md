# Comparing `tmp/diffant-1.0.1.tar.gz` & `tmp/diffant-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffant-1.0.1.tar", max compression
+gzip compressed data, was "diffant-1.0.2.tar", max compression
```

## Comparing `diffant-1.0.1.tar` & `diffant-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2023-06-30 14:30:46.195418 diffant-1.0.1/LICENSE
--rw-r--r--   0        0        0     4087 2023-06-30 16:01:39.294711 diffant-1.0.1/README.md
--rw-r--r--   0        0        0      169 2023-06-23 14:54:16.052445 diffant-1.0.1/diffant/__init__.py
--rw-r--r--   0        0        0    13780 2023-06-30 15:57:50.187364 diffant-1.0.1/diffant/diffabc.py
--rw-r--r--   0        0        0     1072 2023-06-29 17:56:20.082459 diffant-1.0.1/diffant/diffini.py
--rw-r--r--   0        0        0     1121 2023-06-28 21:48:02.247536 diffant-1.0.1/diffant/diffjson.py
--rw-r--r--   0        0        0     2141 2023-06-28 23:00:39.610174 diffant-1.0.1/diffant/diffxml.py
--rw-r--r--   0        0        0     1132 2023-06-29 17:31:32.565365 diffant-1.0.1/diffant/diffyml.py
--rw-r--r--   0        0        0      655 2023-06-30 16:01:07.110238 diffant-1.0.1/diffant/exceptions.py
--rw-r--r--   0        0        0     4246 2023-06-30 16:00:12.361435 diffant-1.0.1/diffant/main.py
--rw-r--r--   0        0        0     2553 2023-06-27 21:11:06.231309 diffant-1.0.1/diffant/nested.py
--rw-r--r--   0        0        0     1115 2023-06-30 20:12:02.728690 diffant-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4794 1970-01-01 00:00:00.000000 diffant-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-30 14:30:46.195418 diffant-1.0.2/LICENSE
+-rw-r--r--   0        0        0     4187 2023-06-30 23:33:01.963065 diffant-1.0.2/README.md
+-rw-r--r--   0        0        0      169 2023-06-23 14:54:16.052445 diffant-1.0.2/diffant/__init__.py
+-rw-r--r--   0        0        0    13780 2023-06-30 15:57:50.187364 diffant-1.0.2/diffant/diffabc.py
+-rw-r--r--   0        0        0     1072 2023-06-29 17:56:20.082459 diffant-1.0.2/diffant/diffini.py
+-rw-r--r--   0        0        0     1121 2023-06-28 21:48:02.247536 diffant-1.0.2/diffant/diffjson.py
+-rw-r--r--   0        0        0     2141 2023-06-28 23:00:39.610174 diffant-1.0.2/diffant/diffxml.py
+-rw-r--r--   0        0        0     1132 2023-06-29 17:31:32.565365 diffant-1.0.2/diffant/diffyml.py
+-rw-r--r--   0        0        0      655 2023-06-30 16:01:07.110238 diffant-1.0.2/diffant/exceptions.py
+-rw-r--r--   0        0        0     4246 2023-06-30 16:00:12.361435 diffant-1.0.2/diffant/main.py
+-rw-r--r--   0        0        0     2553 2023-06-27 21:11:06.231309 diffant-1.0.2/diffant/nested.py
+-rw-r--r--   0        0        0     1435 2023-06-30 22:36:14.881070 diffant-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5069 1970-01-01 00:00:00.000000 diffant-1.0.2/PKG-INFO
```

### Comparing `diffant-1.0.1/LICENSE` & `diffant-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `diffant-1.0.1/README.md` & `diffant-1.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 # `diffant`
-
 `diffant` uses the structure of configuration files to do a more helpful comparison than standard diff.
 
 `diffant` allows you to compare:
 
 * ini
 * json
 * yaml
 
-
-
 For example, for the purpose of comparing configuration, these two files are the same. There should be no diff:
 
 | file_01.ini             | file_02.ini               |
 | ----------------------- | ------------------------- |
 | `[info]`                | `[info]`                  |
 | `email=bob@example.com` | `phone=212-555-1212`      |
 | `phone=212-555-1212`    | `email = bob@example.com` |
 
 `diffant` can meaningfully compare a heavily commented original configuration file with many lines to a minimized comment-less  configuration file and find how the defaults have changed.
 
 You are not limited to comparing 2 files, `diffant` can compare many files.
 
 ## SAMPLE OUTPUT
-```code
+```
 fruit:  apple
           tests/sample_input.dirs/simple/file01.json
           tests/sample_input.dirs/simple/file03.json
 
         cherry
           tests/sample_input.dirs/simple/file02.json
 
@@ -120,24 +117,29 @@
 ```
 ## REQUIREMENTS
 * pip
 * python >= 3.8
 
 ## LICENSE
 GNU General Public License v3.0
+
 ## SETUP
-    `pip3 install diffant`
+```
+pip3 install diffant
+```
 
 ## USAGE
-
 ```
 diffant  <directory with files of same type>
 ```
 
 ## BUGS
-
 1. The files you are comparing need to be  at the top level of a directory that you supply as a positional argument to `diffant`
-1. The files need to have an extension that reflects their contents (ini,json.yaml)
+1. The files need to have an extension that reflects their contents (ini,json.yml)
 1. You can't compare files of different types or have files of different types in your input directory.
 
 ##  SUPPORT
-    email dan@omacneil.org
+dan@omacneil.org
+
+## CONTRIBUTORS
+* @morgan: Helpful tweak to README.md
+* [cpat-gpt](https://chat.openai.com/): about 50% of the code
```

### Comparing `diffant-1.0.1/diffant/diffabc.py` & `diffant-1.0.2/diffant/diffabc.py`

 * *Files identical despite different names*

### Comparing `diffant-1.0.1/diffant/diffini.py` & `diffant-1.0.2/diffant/diffini.py`

 * *Files identical despite different names*

### Comparing `diffant-1.0.1/diffant/diffjson.py` & `diffant-1.0.2/diffant/diffjson.py`

 * *Files identical despite different names*

### Comparing `diffant-1.0.1/diffant/diffxml.py` & `diffant-1.0.2/diffant/diffxml.py`

 * *Files identical despite different names*

### Comparing `diffant-1.0.1/diffant/diffyml.py` & `diffant-1.0.2/diffant/diffyml.py`

 * *Files identical despite different names*

### Comparing `diffant-1.0.1/diffant/exceptions.py` & `diffant-1.0.2/diffant/exceptions.py`

 * *Files identical despite different names*

### Comparing `diffant-1.0.1/diffant/main.py` & `diffant-1.0.2/diffant/main.py`

 * *Files identical despite different names*

### Comparing `diffant-1.0.1/diffant/nested.py` & `diffant-1.0.2/diffant/nested.py`

 * *Files identical despite different names*

### Comparing `diffant-1.0.1/pyproject.toml` & `diffant-1.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 [tool.poetry]
 name = "diffant"
-version = "1.0.1"
+version = "1.0.2"
 description = "tool to compare structured files like json, ini , yaml"
 authors = ["omacneil <dan@omacneil.org>"]
-license = "GNU General Public License v3.0"
+license = "GPL-3.0-or-later"
 readme  = "README.md"
 homepage = "https://github.com/omacneil/diffant"
 repository = "https://github.com/omacneil/diffant"
+keywords = ["json", "yaml","ini","diff","configuration","compare"]
+classifiers=[
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
+    ]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 pyyaml = "6.0"
 types-pyyaml = "6.0.12.10"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `diffant-1.0.1/PKG-INFO` & `diffant-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 Metadata-Version: 2.1
 Name: diffant
-Version: 1.0.1
+Version: 1.0.2
 Summary: tool to compare structured files like json, ini , yaml
 Home-page: https://github.com/omacneil/diffant
-License: GNU General Public License v3.0
+License: GPL-3.0-or-later
+Keywords: json,yaml,ini,diff,configuration,compare
 Author: omacneil
 Author-email: dan@omacneil.org
 Requires-Python: >=3.8.1,<4.0.0
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: pyyaml (==6.0)
 Requires-Dist: types-pyyaml (==6.0.12.10)
 Project-URL: Repository, https://github.com/omacneil/diffant
 Description-Content-Type: text/markdown
 
 # `diffant`
-
 `diffant` uses the structure of configuration files to do a more helpful comparison than standard diff.
 
 `diffant` allows you to compare:
 
 * ini
 * json
 * yaml
 
-
-
 For example, for the purpose of comparing configuration, these two files are the same. There should be no diff:
 
 | file_01.ini             | file_02.ini               |
 | ----------------------- | ------------------------- |
 | `[info]`                | `[info]`                  |
 | `email=bob@example.com` | `phone=212-555-1212`      |
 | `phone=212-555-1212`    | `email = bob@example.com` |
 
 `diffant` can meaningfully compare a heavily commented original configuration file with many lines to a minimized comment-less  configuration file and find how the defaults have changed.
 
 You are not limited to comparing 2 files, `diffant` can compare many files.
 
 ## SAMPLE OUTPUT
-```code
+```
 fruit:  apple
           tests/sample_input.dirs/simple/file01.json
           tests/sample_input.dirs/simple/file03.json
 
         cherry
           tests/sample_input.dirs/simple/file02.json
 
@@ -139,25 +139,30 @@
 ```
 ## REQUIREMENTS
 * pip
 * python >= 3.8
 
 ## LICENSE
 GNU General Public License v3.0
+
 ## SETUP
-    `pip3 install diffant`
+```
+pip3 install diffant
+```
 
 ## USAGE
-
 ```
 diffant  <directory with files of same type>
 ```
 
 ## BUGS
-
 1. The files you are comparing need to be  at the top level of a directory that you supply as a positional argument to `diffant`
-1. The files need to have an extension that reflects their contents (ini,json.yaml)
+1. The files need to have an extension that reflects their contents (ini,json.yml)
 1. You can't compare files of different types or have files of different types in your input directory.
 
 ##  SUPPORT
-    email dan@omacneil.org
+dan@omacneil.org
+
+## CONTRIBUTORS
+* @morgan: Helpful tweak to README.md
+* [cpat-gpt](https://chat.openai.com/): about 50% of the code
```

