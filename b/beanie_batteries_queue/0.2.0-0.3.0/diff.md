# Comparing `tmp/beanie_batteries_queue-0.2.0.tar.gz` & `tmp/beanie_batteries_queue-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanie_batteries_queue-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "beanie_batteries_queue-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `beanie_batteries_queue-0.2.0.tar` & `beanie_batteries_queue-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      373 2023-06-09 19:45:53.159658 beanie_batteries_queue-0.2.0/.github/workflows/github-actions-publish-project.yml
--rw-r--r--   0        0        0      816 2023-06-09 19:45:53.159658 beanie_batteries_queue-0.2.0/.github/workflows/github-actions-tests.yml
--rw-r--r--   0        0        0     2623 2023-06-09 19:45:53.159658 beanie_batteries_queue-0.2.0/.gitignore
--rw-r--r--   0        0        0      475 2023-06-09 19:45:53.159658 beanie_batteries_queue-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11343 2023-06-09 19:45:53.159658 beanie_batteries_queue-0.2.0/LICENSE
--rw-r--r--   0        0        0      145 2023-06-09 19:45:53.159658 beanie_batteries_queue-0.2.0/README.md
--rw-r--r--   0        0        0      180 2023-06-09 19:45:53.159658 beanie_batteries_queue-0.2.0/beanie_batteries_queue/__init__.py
--rw-r--r--   0        0        0     5189 2023-06-09 19:45:53.159658 beanie_batteries_queue-0.2.0/beanie_batteries_queue/queue.py
--rw-r--r--   0        0        0     2375 2023-06-09 19:45:53.159658 beanie_batteries_queue-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-09 19:45:53.159658 beanie_batteries_queue-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1291 2023-06-09 19:45:53.159658 beanie_batteries_queue-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0     1186 2023-06-09 19:45:53.159658 beanie_batteries_queue-0.2.0/tests/tasks.py
--rw-r--r--   0        0        0     7542 2023-06-09 19:45:53.159658 beanie_batteries_queue-0.2.0/tests/test_tasks.py
--rw-r--r--   0        0        0     1080 1970-01-01 00:00:00.000000 beanie_batteries_queue-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      373 2023-06-30 23:34:43.004442 beanie_batteries_queue-0.3.0/.github/workflows/github-actions-publish-project.yml
+-rw-r--r--   0        0        0      816 2023-06-30 23:34:43.004442 beanie_batteries_queue-0.3.0/.github/workflows/github-actions-tests.yml
+-rw-r--r--   0        0        0     2623 2023-06-30 23:34:43.004442 beanie_batteries_queue-0.3.0/.gitignore
+-rw-r--r--   0        0        0      475 2023-06-30 23:34:43.004442 beanie_batteries_queue-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11343 2023-06-30 23:34:43.004442 beanie_batteries_queue-0.3.0/LICENSE
+-rw-r--r--   0        0        0      145 2023-06-30 23:34:43.004442 beanie_batteries_queue-0.3.0/README.md
+-rw-r--r--   0        0        0      180 2023-06-30 23:34:43.004442 beanie_batteries_queue-0.3.0/beanie_batteries_queue/__init__.py
+-rw-r--r--   0        0        0     5189 2023-06-30 23:34:43.004442 beanie_batteries_queue-0.3.0/beanie_batteries_queue/queue.py
+-rw-r--r--   0        0        0     2371 2023-06-30 23:34:43.004442 beanie_batteries_queue-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 23:34:43.004442 beanie_batteries_queue-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     1291 2023-06-30 23:34:43.004442 beanie_batteries_queue-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     1180 2023-06-30 23:34:43.008442 beanie_batteries_queue-0.3.0/tests/tasks.py
+-rw-r--r--   0        0        0     7536 2023-06-30 23:34:43.008442 beanie_batteries_queue-0.3.0/tests/test_tasks.py
+-rw-r--r--   0        0        0     1076 1970-01-01 00:00:00.000000 beanie_batteries_queue-0.3.0/PKG-INFO
```

### Comparing `beanie_batteries_queue-0.2.0/.github/workflows/github-actions-tests.yml` & `beanie_batteries_queue-0.3.0/.github/workflows/github-actions-tests.yml`

 * *Files identical despite different names*

### Comparing `beanie_batteries_queue-0.2.0/.gitignore` & `beanie_batteries_queue-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `beanie_batteries_queue-0.2.0/LICENSE` & `beanie_batteries_queue-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beanie_batteries_queue-0.2.0/beanie_batteries_queue/queue.py` & `beanie_batteries_queue-0.3.0/beanie_batteries_queue/queue.py`

 * *Files identical despite different names*

### Comparing `beanie_batteries_queue-0.2.0/pyproject.toml` & `beanie_batteries_queue-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "beanie_batteries_queue"
-version = "0.2.0"
+version = "0.3.0"
 description = "Simple queue system for Beanie"
 readme = "README.md"
 requires-python = ">=3.7,<4.0"
 license = { file="LICENSE" }
 authors = [
     {name = "Roman Right", email = "roman-right@protonmail.com"}
 ]
 keywords = ["mongodb", "odm", "orm", "pydantic", "mongo", "async", "python", "beanie", "queue", "beanie-batteries-queue"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
 ]
 dependencies = [
-    "beanie==1.20.0b1",
+    "beanie>=1.20",
 ]
 
 [project.optional-dependencies]
 test = [
     "pre-commit>=2.3.0",
     "pytest>=6.0.0",
     "pytest-asyncio>=0.21.0",
```

### Comparing `beanie_batteries_queue-0.2.0/tests/conftest.py` & `beanie_batteries_queue-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `beanie_batteries_queue-0.2.0/tests/tasks.py` & `beanie_batteries_queue-0.3.0/tests/tasks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Optional
 
 from beanie import Link
 from pydantic import Field
 
-from beanie_batteries_queue.queue import Task, DependencyType
+from beanie_batteries_queue import Task, DependencyType
 
 
 class SimpleTask(Task):
     s: str
 
 
 class TaskWithDirectDependency(Task):
```

### Comparing `beanie_batteries_queue-0.2.0/tests/test_tasks.py` & `beanie_batteries_queue-0.3.0/tests/test_tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from beanie_batteries_queue.queue import State, Priority
+from beanie_batteries_queue import State, Priority
 from tests.tasks import (
     SimpleTask,
     TaskWithDirectDependency,
     TaskWithAllOfDependency,
     TaskWithAnyOfDependency,
     TaskWithOptionalDependency,
     TaskWithOptionalAllOfDependency,
```

### Comparing `beanie_batteries_queue-0.2.0/PKG-INFO` & `beanie_batteries_queue-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: beanie_batteries_queue
-Version: 0.2.0
+Version: 0.3.0
 Summary: Simple queue system for Beanie
 Keywords: mongodb,odm,orm,pydantic,mongo,async,python,beanie,queue,beanie-batteries-queue
 Author-email: Roman Right <roman-right@protonmail.com>
 Requires-Python: >=3.7,<4.0
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: beanie==1.20.0b1
+Requires-Dist: beanie>=1.20
 Requires-Dist: pre-commit>=2.3.0 ; extra == "test"
 Requires-Dist: pytest>=6.0.0 ; extra == "test"
 Requires-Dist: pytest-asyncio>=0.21.0 ; extra == "test"
 Requires-Dist: pytest-cov>=2.8.1 ; extra == "test"
 Requires-Dist: dnspython>=2.1.0 ; extra == "test"
 Requires-Dist: flake8>=3 ; extra == "test"
 Requires-Dist: pyright>=0 ; extra == "test"
```

