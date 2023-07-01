# Comparing `tmp/vanna-0.0.3.tar.gz` & `tmp/vanna-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanna-0.0.3.tar", last modified: Fri Jun 23 19:25:50 2023, max compression
+gzip compressed data, was "vanna-0.0.4.tar", last modified: Sat Jul  1 01:49:17 2023, max compression
```

## Comparing `vanna-0.0.3.tar` & `vanna-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:25:50.081479 vanna-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-23 19:25:40.000000 vanna-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-23 19:25:50.081479 vanna-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-23 19:25:40.000000 vanna-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-23 19:25:40.000000 vanna-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 19:25:50.081479 vanna-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:25:50.081479 vanna-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:25:50.081479 vanna-0.0.3/src/vanna/
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-06-23 19:25:40.000000 vanna-0.0.3/src/vanna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-23 19:25:40.000000 vanna-0.0.3/src/vanna/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:25:50.081479 vanna-0.0.3/src/vanna.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-23 19:25:50.000000 vanna-0.0.3/src/vanna.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-23 19:25:50.000000 vanna-0.0.3/src/vanna.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 19:25:50.000000 vanna-0.0.3/src/vanna.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-23 19:25:50.000000 vanna-0.0.3/src/vanna.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 19:25:50.000000 vanna-0.0.3/src/vanna.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:49:17.141005 vanna-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-01 01:49:05.000000 vanna-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-01 01:49:17.141005 vanna-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 01:49:05.000000 vanna-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-01 01:49:05.000000 vanna-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 01:49:17.141005 vanna-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:49:17.141005 vanna-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:49:17.141005 vanna-0.0.4/src/vanna/
+-rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-07-01 01:49:05.000000 vanna-0.0.4/src/vanna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-01 01:49:05.000000 vanna-0.0.4/src/vanna/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 01:49:17.141005 vanna-0.0.4/src/vanna.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-01 01:49:17.000000 vanna-0.0.4/src/vanna.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-01 01:49:17.000000 vanna-0.0.4/src/vanna.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 01:49:17.000000 vanna-0.0.4/src/vanna.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-01 01:49:17.000000 vanna-0.0.4/src/vanna.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-01 01:49:17.000000 vanna-0.0.4/src/vanna.egg-info/top_level.txt
```

### Comparing `vanna-0.0.3/LICENSE` & `vanna-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vanna-0.0.3/PKG-INFO` & `vanna-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vanna
-Version: 0.0.3
+Version: 0.0.4
 Summary: Generate SQL queries from natural language
 Author-email: Zain Hoda <zain@vanna.ai>
 Project-URL: Homepage, https://github.com/vanna-ai/vanna-py
 Project-URL: Bug Tracker, https://github.com/vanna-ai/vanna-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vanna-0.0.3/pyproject.toml` & `vanna-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "vanna"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Zain Hoda", email="zain@vanna.ai" },
 ]
 description = "Generate SQL queries from natural language"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -14,8 +14,8 @@
 ]
 dependencies = [
     "requests", "tabulate", "plotly"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/vanna-ai/vanna-py"
-"Bug Tracker" = "https://github.com/vanna-ai/vanna-py/issues"
+"Bug Tracker" = "https://github.com/vanna-ai/vanna-py/issues"
```

### Comparing `vanna-0.0.3/src/vanna/types.py` & `vanna-0.0.4/src/vanna/types.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from __future__ import annotations
-from typing import List
+from typing import List, Dict
 from dataclasses import dataclass
 
 @dataclass
 class Status:
     success: bool
     message: str
 
 @dataclass
+class QuestionList:
+    questions: List[FullQuestionDocument]
+
+@dataclass
 class FullQuestionDocument:
     id: QuestionId
     question: Question
     answer: SQLAnswer | None
     data: DataResult | None
     plotly: PlotlyResult | None
 
@@ -31,14 +35,33 @@
     id: str
 
 @dataclass
 class Question:
     question: str
 
 @dataclass
+class QuestionCategory:
+    question: str
+    category: str
+
+    NO_SQL_GENERATED = "No SQL Generated"
+    SQL_UNABLE_TO_RUN = "SQL Unable to Run"
+    BOOTSTRAP_TRAINING_QUERY = "Bootstrap Training Query"
+    ASSUMED_CORRECT = "Assumed Correct"
+    FLAGGED_FOR_REVIEW = "Flagged for Review"
+    REVIEWED_AND_APPROVED = "Reviewed and Approved"
+    REVIEWED_AND_REJECTED = "Reviewed and Rejected"
+    REVIEWED_AND_UPDATED = "Reviewed and Updated" 
+
+@dataclass
+class AccuracyStats:
+    num_questions: int
+    data: Dict[str, int]
+
+@dataclass
 class Followup:
     followup: str
 
 @dataclass
 class QuestionEmbedding:
     question: Question
     embedding: List[float]
```

### Comparing `vanna-0.0.3/src/vanna.egg-info/PKG-INFO` & `vanna-0.0.4/src/vanna.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vanna
-Version: 0.0.3
+Version: 0.0.4
 Summary: Generate SQL queries from natural language
 Author-email: Zain Hoda <zain@vanna.ai>
 Project-URL: Homepage, https://github.com/vanna-ai/vanna-py
 Project-URL: Bug Tracker, https://github.com/vanna-ai/vanna-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

