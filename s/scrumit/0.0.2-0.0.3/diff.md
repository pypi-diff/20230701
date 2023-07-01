# Comparing `tmp/scrumit-0.0.2.tar.gz` & `tmp/scrumit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrumit-0.0.2.tar", last modified: Sat Jul  1 13:34:54 2023, max compression
+gzip compressed data, was "scrumit-0.0.3.tar", last modified: Sat Jul  1 13:47:20 2023, max compression
```

## Comparing `scrumit-0.0.2.tar` & `scrumit-0.0.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 komronvalijonov   (501) staff       (20)        0 2023-07-01 13:34:54.117727 scrumit-0.0.2/
--rw-r--r--   0 komronvalijonov   (501) staff       (20)    35149 2023-07-01 13:19:25.000000 scrumit-0.0.2/LICENSE
--rw-r--r--   0 komronvalijonov   (501) staff       (20)    45955 2023-07-01 13:34:54.117555 scrumit-0.0.2/PKG-INFO
--rw-r--r--   0 komronvalijonov   (501) staff       (20)     5027 2023-07-01 13:17:07.000000 scrumit-0.0.2/README.md
--rw-r--r--   0 komronvalijonov   (501) staff       (20)      722 2023-07-01 13:34:49.000000 scrumit-0.0.2/pyproject.toml
--rw-r--r--   0 komronvalijonov   (501) staff       (20)      122 2023-07-01 13:34:18.000000 scrumit-0.0.2/requirements.chill
-drwxr-xr-x   0 komronvalijonov   (501) staff       (20)        0 2023-07-01 13:34:54.111781 scrumit-0.0.2/scrumit/
--rw-r--r--   0 komronvalijonov   (501) staff       (20)        0 2023-06-30 11:43:24.000000 scrumit-0.0.2/scrumit/__init__.py
--rw-r--r--   0 komronvalijonov   (501) staff       (20)     1631 2023-07-01 13:08:08.000000 scrumit-0.0.2/scrumit/cmd.py
--rw-r--r--   0 komronvalijonov   (501) staff       (20)     2456 2023-07-01 13:08:08.000000 scrumit-0.0.2/scrumit/config.py
--rw-r--r--   0 komronvalijonov   (501) staff       (20)      702 2023-07-01 00:20:17.000000 scrumit-0.0.2/scrumit/default_paraphraser_examples.json
--rw-r--r--   0 komronvalijonov   (501) staff       (20)     2602 2023-06-30 15:12:33.000000 scrumit-0.0.2/scrumit/default_recognizer_examples.json
-drwxr-xr-x   0 komronvalijonov   (501) staff       (20)        0 2023-07-01 13:34:54.113545 scrumit-0.0.2/scrumit/entity/
--rw-r--r--   0 komronvalijonov   (501) staff       (20)       74 2023-07-01 13:08:21.000000 scrumit-0.0.2/scrumit/entity/__init__.py
--rw-r--r--   0 komronvalijonov   (501) staff       (20)     1037 2023-07-01 01:12:22.000000 scrumit-0.0.2/scrumit/entity/paraphraser.py
--rw-r--r--   0 komronvalijonov   (501) staff       (20)     2231 2023-06-30 15:48:06.000000 scrumit-0.0.2/scrumit/entity/recognizer.py
--rw-r--r--   0 komronvalijonov   (501) staff       (20)     1442 2023-07-01 01:45:33.000000 scrumit-0.0.2/scrumit/entity/scrumit.py
-drwxr-xr-x   0 komronvalijonov   (501) staff       (20)        0 2023-07-01 13:34:54.114245 scrumit-0.0.2/scrumit/paraphraser/
--rw-r--r--   0 komronvalijonov   (501) staff       (20)       33 2023-07-01 00:28:23.000000 scrumit-0.0.2/scrumit/paraphraser/__init__.py
-drwxr-xr-x   0 komronvalijonov   (501) staff       (20)        0 2023-07-01 13:34:54.114682 scrumit-0.0.2/scrumit/paraphraser/backends/
--rw-r--r--   0 komronvalijonov   (501) staff       (20)       52 2023-07-01 00:20:43.000000 scrumit-0.0.2/scrumit/paraphraser/backends/__init__.py
--rw-r--r--   0 komronvalijonov   (501) staff       (20)     6724 2023-07-01 01:18:55.000000 scrumit-0.0.2/scrumit/paraphraser/backends/openai.py
--rw-r--r--   0 komronvalijonov   (501) staff       (20)      557 2023-07-01 00:28:09.000000 scrumit-0.0.2/scrumit/paraphraser/base.py
--rw-r--r--   0 komronvalijonov   (501) staff       (20)     1364 2023-07-01 00:20:17.000000 scrumit-0.0.2/scrumit/paraphraser/exceptions.py
-drwxr-xr-x   0 komronvalijonov   (501) staff       (20)        0 2023-07-01 13:34:54.115491 scrumit-0.0.2/scrumit/recognizer/
--rw-r--r--   0 komronvalijonov   (501) staff       (20)       33 2023-07-01 00:24:21.000000 scrumit-0.0.2/scrumit/recognizer/__init__.py
-drwxr-xr-x   0 komronvalijonov   (501) staff       (20)        0 2023-07-01 13:34:54.115977 scrumit-0.0.2/scrumit/recognizer/backends/
--rw-r--r--   0 komronvalijonov   (501) staff       (20)       51 2023-07-01 00:24:25.000000 scrumit-0.0.2/scrumit/recognizer/backends/__init__.py
--rw-r--r--   0 komronvalijonov   (501) staff       (20)     5460 2023-07-01 13:08:08.000000 scrumit-0.0.2/scrumit/recognizer/backends/openai.py
--rw-r--r--   0 komronvalijonov   (501) staff       (20)      742 2023-06-30 21:34:51.000000 scrumit-0.0.2/scrumit/recognizer/base.py
--rw-r--r--   0 komronvalijonov   (501) staff       (20)      993 2023-07-01 00:20:17.000000 scrumit-0.0.2/scrumit/recognizer/exceptions.py
-drwxr-xr-x   0 komronvalijonov   (501) staff       (20)        0 2023-07-01 13:34:54.116954 scrumit-0.0.2/scrumit/scrumer/
--rw-r--r--   0 komronvalijonov   (501) staff       (20)       43 2023-07-01 11:35:18.000000 scrumit-0.0.2/scrumit/scrumer/__init__.py
--rw-r--r--   0 komronvalijonov   (501) staff       (20)      426 2023-07-01 11:35:18.000000 scrumit-0.0.2/scrumit/scrumer/base.py
--rw-r--r--   0 komronvalijonov   (501) staff       (20)      417 2023-07-01 01:32:26.000000 scrumit-0.0.2/scrumit/scrumer/exceptions.py
--rw-r--r--   0 komronvalijonov   (501) staff       (20)     2360 2023-07-01 11:35:18.000000 scrumit-0.0.2/scrumit/scrumer/scrumit.py
-drwxr-xr-x   0 komronvalijonov   (501) staff       (20)        0 2023-07-01 13:34:54.112687 scrumit-0.0.2/scrumit.egg-info/
--rw-r--r--   0 komronvalijonov   (501) staff       (20)    45955 2023-07-01 13:34:54.000000 scrumit-0.0.2/scrumit.egg-info/PKG-INFO
--rw-r--r--   0 komronvalijonov   (501) staff       (20)     1012 2023-07-01 13:34:54.000000 scrumit-0.0.2/scrumit.egg-info/SOURCES.txt
--rw-r--r--   0 komronvalijonov   (501) staff       (20)        1 2023-07-01 13:34:54.000000 scrumit-0.0.2/scrumit.egg-info/dependency_links.txt
--rw-r--r--   0 komronvalijonov   (501) staff       (20)       45 2023-07-01 13:34:54.000000 scrumit-0.0.2/scrumit.egg-info/entry_points.txt
--rw-r--r--   0 komronvalijonov   (501) staff       (20)      122 2023-07-01 13:34:54.000000 scrumit-0.0.2/scrumit.egg-info/requires.txt
--rw-r--r--   0 komronvalijonov   (501) staff       (20)        8 2023-07-01 13:34:54.000000 scrumit-0.0.2/scrumit.egg-info/top_level.txt
--rw-r--r--   0 komronvalijonov   (501) staff       (20)       38 2023-07-01 13:34:54.117768 scrumit-0.0.2/setup.cfg
-drwxr-xr-x   0 komronvalijonov   (501) staff       (20)        0 2023-07-01 13:34:54.117316 scrumit-0.0.2/tests/
--rw-r--r--   0 komronvalijonov   (501) staff       (20)        0 2023-06-29 14:58:02.000000 scrumit-0.0.2/tests/test_paraphraser.py
--rw-r--r--   0 komronvalijonov   (501) staff       (20)        0 2023-06-30 12:41:15.000000 scrumit-0.0.2/tests/test_recognizer.py
--rw-r--r--   0 komronvalijonov   (501) staff       (20)        0 2023-06-30 12:37:51.000000 scrumit-0.0.2/tests/test_scrumit.py
+drwxr-xr-x   0 komronvalijonov   (501) staff       (20)        0 2023-07-01 13:47:20.610431 scrumit-0.0.3/
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)    35149 2023-07-01 13:19:25.000000 scrumit-0.0.3/LICENSE
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)    45955 2023-07-01 13:47:20.610264 scrumit-0.0.3/PKG-INFO
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)     5027 2023-07-01 13:17:07.000000 scrumit-0.0.3/README.md
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)      720 2023-07-01 13:46:13.000000 scrumit-0.0.3/pyproject.toml
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)     1027 2023-07-01 13:43:00.000000 scrumit-0.0.3/requirements.txt
+drwxr-xr-x   0 komronvalijonov   (501) staff       (20)        0 2023-07-01 13:47:20.606663 scrumit-0.0.3/scrumit/
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)        0 2023-06-30 11:43:24.000000 scrumit-0.0.3/scrumit/__init__.py
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)     1631 2023-07-01 13:08:08.000000 scrumit-0.0.3/scrumit/cmd.py
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)     2456 2023-07-01 13:08:08.000000 scrumit-0.0.3/scrumit/config.py
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)      702 2023-07-01 00:20:17.000000 scrumit-0.0.3/scrumit/default_paraphraser_examples.json
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)     2602 2023-06-30 15:12:33.000000 scrumit-0.0.3/scrumit/default_recognizer_examples.json
+drwxr-xr-x   0 komronvalijonov   (501) staff       (20)        0 2023-07-01 13:47:20.608141 scrumit-0.0.3/scrumit/entity/
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)       74 2023-07-01 13:08:21.000000 scrumit-0.0.3/scrumit/entity/__init__.py
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)     1037 2023-07-01 01:12:22.000000 scrumit-0.0.3/scrumit/entity/paraphraser.py
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)     2231 2023-06-30 15:48:06.000000 scrumit-0.0.3/scrumit/entity/recognizer.py
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)     1442 2023-07-01 01:45:33.000000 scrumit-0.0.3/scrumit/entity/scrumit.py
+drwxr-xr-x   0 komronvalijonov   (501) staff       (20)        0 2023-07-01 13:47:20.608491 scrumit-0.0.3/scrumit/paraphraser/
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)       33 2023-07-01 00:28:23.000000 scrumit-0.0.3/scrumit/paraphraser/__init__.py
+drwxr-xr-x   0 komronvalijonov   (501) staff       (20)        0 2023-07-01 13:47:20.608731 scrumit-0.0.3/scrumit/paraphraser/backends/
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)       52 2023-07-01 00:20:43.000000 scrumit-0.0.3/scrumit/paraphraser/backends/__init__.py
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)     6724 2023-07-01 01:18:55.000000 scrumit-0.0.3/scrumit/paraphraser/backends/openai.py
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)      557 2023-07-01 00:28:09.000000 scrumit-0.0.3/scrumit/paraphraser/base.py
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)     1364 2023-07-01 00:20:17.000000 scrumit-0.0.3/scrumit/paraphraser/exceptions.py
+drwxr-xr-x   0 komronvalijonov   (501) staff       (20)        0 2023-07-01 13:47:20.609073 scrumit-0.0.3/scrumit/recognizer/
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)       33 2023-07-01 00:24:21.000000 scrumit-0.0.3/scrumit/recognizer/__init__.py
+drwxr-xr-x   0 komronvalijonov   (501) staff       (20)        0 2023-07-01 13:47:20.609304 scrumit-0.0.3/scrumit/recognizer/backends/
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)       51 2023-07-01 00:24:25.000000 scrumit-0.0.3/scrumit/recognizer/backends/__init__.py
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)     5460 2023-07-01 13:08:08.000000 scrumit-0.0.3/scrumit/recognizer/backends/openai.py
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)      742 2023-06-30 21:34:51.000000 scrumit-0.0.3/scrumit/recognizer/base.py
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)      993 2023-07-01 00:20:17.000000 scrumit-0.0.3/scrumit/recognizer/exceptions.py
+drwxr-xr-x   0 komronvalijonov   (501) staff       (20)        0 2023-07-01 13:47:20.609743 scrumit-0.0.3/scrumit/scrumer/
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)       43 2023-07-01 11:35:18.000000 scrumit-0.0.3/scrumit/scrumer/__init__.py
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)      426 2023-07-01 11:35:18.000000 scrumit-0.0.3/scrumit/scrumer/base.py
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)      417 2023-07-01 01:32:26.000000 scrumit-0.0.3/scrumit/scrumer/exceptions.py
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)     2360 2023-07-01 11:35:18.000000 scrumit-0.0.3/scrumit/scrumer/scrumit.py
+drwxr-xr-x   0 komronvalijonov   (501) staff       (20)        0 2023-07-01 13:47:20.607522 scrumit-0.0.3/scrumit.egg-info/
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)    45955 2023-07-01 13:47:20.000000 scrumit-0.0.3/scrumit.egg-info/PKG-INFO
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)     1010 2023-07-01 13:47:20.000000 scrumit-0.0.3/scrumit.egg-info/SOURCES.txt
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)        1 2023-07-01 13:47:20.000000 scrumit-0.0.3/scrumit.egg-info/dependency_links.txt
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)       45 2023-07-01 13:47:20.000000 scrumit-0.0.3/scrumit.egg-info/entry_points.txt
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)     1027 2023-07-01 13:47:20.000000 scrumit-0.0.3/scrumit.egg-info/requires.txt
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)        8 2023-07-01 13:47:20.000000 scrumit-0.0.3/scrumit.egg-info/top_level.txt
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)       38 2023-07-01 13:47:20.610467 scrumit-0.0.3/setup.cfg
+drwxr-xr-x   0 komronvalijonov   (501) staff       (20)        0 2023-07-01 13:47:20.610039 scrumit-0.0.3/tests/
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)        0 2023-06-29 14:58:02.000000 scrumit-0.0.3/tests/test_paraphraser.py
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)        0 2023-06-30 12:41:15.000000 scrumit-0.0.3/tests/test_recognizer.py
+-rw-r--r--   0 komronvalijonov   (501) staff       (20)        0 2023-06-30 12:37:51.000000 scrumit-0.0.3/tests/test_scrumit.py
```

### Comparing `scrumit-0.0.2/LICENSE` & `scrumit-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scrumit-0.0.2/PKG-INFO` & `scrumit-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrumit
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package that converts raw text to scrum user stories
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `scrumit-0.0.2/README.md` & `scrumit-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `scrumit-0.0.2/pyproject.toml` & `scrumit-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 description = "Package that converts raw text to scrum user stories"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
 ]
-version = "0.0.2"
+version = "0.0.3"
 requires-python = ">=3.10.9"
 dynamic = ["dependencies"]
 license = { file = "LICENSE" }
 
 [tool.setuptools.dynamic]
-dependencies = { file = ["requirements.chill"] }
+dependencies = { file = ["requirements.txt"] }
 
 [tool.setuptools.package-data]
 scrumit = ["default_paraphraser_examples.json", "default_recognizer_examples.json"]
 
 [project.scripts]
 scrumit = "scrumit.cmd:main"
```

### Comparing `scrumit-0.0.2/scrumit/cmd.py` & `scrumit-0.0.3/scrumit/cmd.py`

 * *Files identical despite different names*

### Comparing `scrumit-0.0.2/scrumit/config.py` & `scrumit-0.0.3/scrumit/config.py`

 * *Files identical despite different names*

### Comparing `scrumit-0.0.2/scrumit/default_paraphraser_examples.json` & `scrumit-0.0.3/scrumit/default_paraphraser_examples.json`

 * *Files identical despite different names*

### Comparing `scrumit-0.0.2/scrumit/default_recognizer_examples.json` & `scrumit-0.0.3/scrumit/default_recognizer_examples.json`

 * *Files identical despite different names*

### Comparing `scrumit-0.0.2/scrumit/entity/paraphraser.py` & `scrumit-0.0.3/scrumit/entity/paraphraser.py`

 * *Files identical despite different names*

### Comparing `scrumit-0.0.2/scrumit/entity/recognizer.py` & `scrumit-0.0.3/scrumit/entity/recognizer.py`

 * *Files identical despite different names*

### Comparing `scrumit-0.0.2/scrumit/entity/scrumit.py` & `scrumit-0.0.3/scrumit/entity/scrumit.py`

 * *Files identical despite different names*

### Comparing `scrumit-0.0.2/scrumit/paraphraser/backends/openai.py` & `scrumit-0.0.3/scrumit/paraphraser/backends/openai.py`

 * *Files identical despite different names*

### Comparing `scrumit-0.0.2/scrumit/paraphraser/base.py` & `scrumit-0.0.3/scrumit/paraphraser/base.py`

 * *Files identical despite different names*

### Comparing `scrumit-0.0.2/scrumit/paraphraser/exceptions.py` & `scrumit-0.0.3/scrumit/paraphraser/exceptions.py`

 * *Files identical despite different names*

### Comparing `scrumit-0.0.2/scrumit/recognizer/backends/openai.py` & `scrumit-0.0.3/scrumit/recognizer/backends/openai.py`

 * *Files identical despite different names*

### Comparing `scrumit-0.0.2/scrumit/recognizer/base.py` & `scrumit-0.0.3/scrumit/recognizer/base.py`

 * *Files identical despite different names*

### Comparing `scrumit-0.0.2/scrumit/recognizer/exceptions.py` & `scrumit-0.0.3/scrumit/recognizer/exceptions.py`

 * *Files identical despite different names*

### Comparing `scrumit-0.0.2/scrumit/scrumer/scrumit.py` & `scrumit-0.0.3/scrumit/scrumer/scrumit.py`

 * *Files identical despite different names*

### Comparing `scrumit-0.0.2/scrumit.egg-info/PKG-INFO` & `scrumit-0.0.3/scrumit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrumit
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package that converts raw text to scrum user stories
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `scrumit-0.0.2/scrumit.egg-info/SOURCES.txt` & `scrumit-0.0.3/scrumit.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
-requirements.chill
+requirements.txt
 scrumit/__init__.py
 scrumit/cmd.py
 scrumit/config.py
 scrumit/default_paraphraser_examples.json
 scrumit/default_recognizer_examples.json
 scrumit.egg-info/PKG-INFO
 scrumit.egg-info/SOURCES.txt
```

