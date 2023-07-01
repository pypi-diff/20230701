# Comparing `tmp/sweepai-0.1.1.tar.gz` & `tmp/sweepai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweepai-0.1.1.tar", max compression
+gzip compressed data, was "sweepai-0.1.2.tar", max compression
```

## Comparing `sweepai-0.1.1.tar` & `sweepai-0.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.1.1/LICENSE
--rw-r--r--   0        0        0     1102 2023-07-01 07:39:32.877485 sweepai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-15 06:30:41.945190 sweepai-0.1.1/src/__init__.py
--rw-r--r--   0        0        0    10056 2023-06-30 23:50:43.893232 sweepai-0.1.1/src/api.py
--rw-r--r--   0        0        0     3918 2023-07-01 07:28:30.813206 sweepai-0.1.1/src/app/api_client.py
--rw-r--r--   0        0        0     8697 2023-07-01 06:53:00.643340 sweepai-0.1.1/src/app/backend.py
--rw-r--r--   0        0        0     3311 2023-07-01 06:28:16.381542 sweepai-0.1.1/src/app/config.py
--rw-r--r--   0        0        0      744 2023-07-01 06:34:10.612287 sweepai-0.1.1/src/app/sweepai.py
--rw-r--r--   0        0        0     6348 2023-07-01 06:20:34.657237 sweepai-0.1.1/src/app/ui.py
--rw-r--r--   0        0        0        0 2023-03-21 00:50:54.566288 sweepai-0.1.1/src/core/__init__.py
--rw-r--r--   0        0        0    15838 2023-06-30 23:50:43.893232 sweepai-0.1.1/src/core/chat.py
--rw-r--r--   0        0        0     2541 2023-06-30 23:50:43.893232 sweepai-0.1.1/src/core/code_repair.py
--rw-r--r--   0        0        0     6815 2023-06-30 23:50:43.893232 sweepai-0.1.1/src/core/entities.py
--rw-r--r--   0        0        0    12775 2023-06-30 23:50:43.896566 sweepai-0.1.1/src/core/prompts.py
--rw-r--r--   0        0        0     3509 2023-06-21 23:04:06.027667 sweepai-0.1.1/src/core/react.py
--rw-r--r--   0        0        0    15463 2023-07-01 03:28:14.554557 sweepai-0.1.1/src/core/sweep_bot.py
--rw-r--r--   0        0        0    12319 2023-06-30 23:50:43.896566 sweepai-0.1.1/src/core/vector_db.py
--rw-r--r--   0        0        0     2536 2023-06-16 23:50:11.723074 sweepai-0.1.1/src/events.py
--rw-r--r--   0        0        0        0 2023-03-21 00:50:54.566288 sweepai-0.1.1/src/handlers/__init__.py
--rw-r--r--   0        0        0     3126 2023-06-30 07:26:46.313809 sweepai-0.1.1/src/handlers/create_pr.py
--rw-r--r--   0        0        0     5882 2023-06-30 23:50:43.896566 sweepai-0.1.1/src/handlers/on_comment.py
--rw-r--r--   0        0        0     3403 2023-06-30 23:50:43.896566 sweepai-0.1.1/src/handlers/on_review.py
--rw-r--r--   0        0        0    11236 2023-06-30 23:50:43.896566 sweepai-0.1.1/src/handlers/on_ticket.py
--rw-r--r--   0        0        0    19469 2023-06-27 19:07:01.581627 sweepai-0.1.1/src/slack.py
--rw-r--r--   0        0        0        0 2023-03-19 00:13:25.553442 sweepai-0.1.1/src/utils/__init__.py
--rw-r--r--   0        0        0      385 2023-06-27 05:32:32.711633 sweepai-0.1.1/src/utils/config.py
--rw-r--r--   0        0        0      670 2023-06-30 23:57:36.298069 sweepai-0.1.1/src/utils/constants.py
--rw-r--r--   0        0        0     3633 2023-06-30 23:50:43.896566 sweepai-0.1.1/src/utils/diff.py
--rw-r--r--   0        0        0      511 2023-06-15 23:48:37.899560 sweepai-0.1.1/src/utils/event_logger.py
--rw-r--r--   0        0        0     5237 2023-06-26 21:11:27.030016 sweepai-0.1.1/src/utils/file_change_functions.py
--rw-r--r--   0        0        0     8083 2023-06-27 05:32:32.714966 sweepai-0.1.1/src/utils/github_utils.py
--rw-r--r--   0        0        0       98 2023-06-15 23:48:37.899560 sweepai-0.1.1/src/utils/hash.py
--rw-r--r--   0        0        0      822 2023-06-15 23:48:37.899560 sweepai-0.1.1/src/utils/huggingface.py
--rw-r--r--   0        0        0     5335 2023-06-30 23:50:43.896566 sweepai-0.1.1/src/utils/prompt_constructor.py
--rw-r--r--   0        0        0      748 2023-06-30 23:50:43.896566 sweepai-0.1.1/src/utils/scorer.py
--rw-r--r--   0        0        0     1490 2023-06-26 21:11:27.030016 sweepai-0.1.1/src/utils/snippets.py
--rw-r--r--   0        0        0    11470 2023-06-30 23:50:43.896566 sweepai-0.1.1/src/utils/utils.py
--rw-r--r--   0        0        0     1615 2023-07-01 07:39:35.046439 sweepai-0.1.1/setup.py
--rw-r--r--   0        0        0     1528 2023-07-01 07:39:35.046753 sweepai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1103 2023-07-01 07:52:45.459406 sweepai-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-15 06:30:41.945190 sweepai-0.1.2/src/__init__.py
+-rw-r--r--   0        0        0    10056 2023-06-30 23:50:43.893232 sweepai-0.1.2/src/api.py
+-rw-r--r--   0        0        0     3918 2023-07-01 07:28:30.813206 sweepai-0.1.2/src/app/api_client.py
+-rw-r--r--   0        0        0     8697 2023-07-01 06:53:00.643340 sweepai-0.1.2/src/app/backend.py
+-rw-r--r--   0        0        0     3311 2023-07-01 06:28:16.381542 sweepai-0.1.2/src/app/config.py
+-rw-r--r--   0        0        0      744 2023-07-01 06:34:10.612287 sweepai-0.1.2/src/app/sweepai.py
+-rw-r--r--   0        0        0     6348 2023-07-01 06:20:34.657237 sweepai-0.1.2/src/app/ui.py
+-rw-r--r--   0        0        0        0 2023-03-21 00:50:54.566288 sweepai-0.1.2/src/core/__init__.py
+-rw-r--r--   0        0        0    15838 2023-06-30 23:50:43.893232 sweepai-0.1.2/src/core/chat.py
+-rw-r--r--   0        0        0     2541 2023-06-30 23:50:43.893232 sweepai-0.1.2/src/core/code_repair.py
+-rw-r--r--   0        0        0     6815 2023-06-30 23:50:43.893232 sweepai-0.1.2/src/core/entities.py
+-rw-r--r--   0        0        0    12775 2023-06-30 23:50:43.896566 sweepai-0.1.2/src/core/prompts.py
+-rw-r--r--   0        0        0     3509 2023-06-21 23:04:06.027667 sweepai-0.1.2/src/core/react.py
+-rw-r--r--   0        0        0    15463 2023-07-01 03:28:14.554557 sweepai-0.1.2/src/core/sweep_bot.py
+-rw-r--r--   0        0        0    12319 2023-06-30 23:50:43.896566 sweepai-0.1.2/src/core/vector_db.py
+-rw-r--r--   0        0        0     2536 2023-06-16 23:50:11.723074 sweepai-0.1.2/src/events.py
+-rw-r--r--   0        0        0        0 2023-03-21 00:50:54.566288 sweepai-0.1.2/src/handlers/__init__.py
+-rw-r--r--   0        0        0     3126 2023-06-30 07:26:46.313809 sweepai-0.1.2/src/handlers/create_pr.py
+-rw-r--r--   0        0        0     5882 2023-06-30 23:50:43.896566 sweepai-0.1.2/src/handlers/on_comment.py
+-rw-r--r--   0        0        0     3403 2023-06-30 23:50:43.896566 sweepai-0.1.2/src/handlers/on_review.py
+-rw-r--r--   0        0        0    11236 2023-06-30 23:50:43.896566 sweepai-0.1.2/src/handlers/on_ticket.py
+-rw-r--r--   0        0        0    19469 2023-06-27 19:07:01.581627 sweepai-0.1.2/src/slack.py
+-rw-r--r--   0        0        0        0 2023-03-19 00:13:25.553442 sweepai-0.1.2/src/utils/__init__.py
+-rw-r--r--   0        0        0      385 2023-06-27 05:32:32.711633 sweepai-0.1.2/src/utils/config.py
+-rw-r--r--   0        0        0      670 2023-06-30 23:57:36.298069 sweepai-0.1.2/src/utils/constants.py
+-rw-r--r--   0        0        0     3633 2023-06-30 23:50:43.896566 sweepai-0.1.2/src/utils/diff.py
+-rw-r--r--   0        0        0      511 2023-06-15 23:48:37.899560 sweepai-0.1.2/src/utils/event_logger.py
+-rw-r--r--   0        0        0     5237 2023-06-26 21:11:27.030016 sweepai-0.1.2/src/utils/file_change_functions.py
+-rw-r--r--   0        0        0     8083 2023-06-27 05:32:32.714966 sweepai-0.1.2/src/utils/github_utils.py
+-rw-r--r--   0        0        0       98 2023-06-15 23:48:37.899560 sweepai-0.1.2/src/utils/hash.py
+-rw-r--r--   0        0        0      822 2023-06-15 23:48:37.899560 sweepai-0.1.2/src/utils/huggingface.py
+-rw-r--r--   0        0        0     5335 2023-06-30 23:50:43.896566 sweepai-0.1.2/src/utils/prompt_constructor.py
+-rw-r--r--   0        0        0      748 2023-06-30 23:50:43.896566 sweepai-0.1.2/src/utils/scorer.py
+-rw-r--r--   0        0        0     1490 2023-06-26 21:11:27.030016 sweepai-0.1.2/src/utils/snippets.py
+-rw-r--r--   0        0        0    11470 2023-06-30 23:50:43.896566 sweepai-0.1.2/src/utils/utils.py
+-rw-r--r--   0        0        0     1616 2023-07-01 07:52:47.673708 sweepai-0.1.2/setup.py
+-rw-r--r--   0        0        0     1528 2023-07-01 07:52:47.674046 sweepai-0.1.2/PKG-INFO
```

### Comparing `sweepai-0.1.1/LICENSE` & `sweepai-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/pyproject.toml` & `sweepai-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sweepai"
-version = "0.1.1"
+version = "0.1.2"
 description = "Sweep software chores"
 authors = ["Kevin Lu", "William Zeng", "Luke Jagg"]
 packages = [
     { include = "src" }
 ]
 
 [tool.poetry.dependencies]
@@ -48,8 +48,8 @@
 jupyter = "^1.0.0"
 ipykernel = "^6.23.1"
 
 [mypy]
 check_untyped_defs = true
 
 [tool.poetry.scripts]
-sweepai = "src.app.sweep.py"
+sweepai = "src.app.sweep:app"
```

### Comparing `sweepai-0.1.1/src/api.py` & `sweepai-0.1.2/src/api.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/src/app/api_client.py` & `sweepai-0.1.2/src/app/api_client.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/src/app/backend.py` & `sweepai-0.1.2/src/app/backend.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/src/app/config.py` & `sweepai-0.1.2/src/app/config.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/src/app/sweepai.py` & `sweepai-0.1.2/src/app/sweepai.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/src/app/ui.py` & `sweepai-0.1.2/src/app/ui.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/src/core/chat.py` & `sweepai-0.1.2/src/core/chat.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/src/core/code_repair.py` & `sweepai-0.1.2/src/core/code_repair.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/src/core/entities.py` & `sweepai-0.1.2/src/core/entities.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/src/core/prompts.py` & `sweepai-0.1.2/src/core/prompts.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/src/core/react.py` & `sweepai-0.1.2/src/core/react.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/src/core/sweep_bot.py` & `sweepai-0.1.2/src/core/sweep_bot.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/src/core/vector_db.py` & `sweepai-0.1.2/src/core/vector_db.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/src/events.py` & `sweepai-0.1.2/src/events.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/src/handlers/create_pr.py` & `sweepai-0.1.2/src/handlers/create_pr.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/src/handlers/on_comment.py` & `sweepai-0.1.2/src/handlers/on_comment.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/src/handlers/on_review.py` & `sweepai-0.1.2/src/handlers/on_review.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/src/handlers/on_ticket.py` & `sweepai-0.1.2/src/handlers/on_ticket.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/src/slack.py` & `sweepai-0.1.2/src/slack.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/src/utils/constants.py` & `sweepai-0.1.2/src/utils/constants.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/src/utils/diff.py` & `sweepai-0.1.2/src/utils/diff.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/src/utils/file_change_functions.py` & `sweepai-0.1.2/src/utils/file_change_functions.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/src/utils/github_utils.py` & `sweepai-0.1.2/src/utils/github_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/src/utils/huggingface.py` & `sweepai-0.1.2/src/utils/huggingface.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/src/utils/prompt_constructor.py` & `sweepai-0.1.2/src/utils/prompt_constructor.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/src/utils/scorer.py` & `sweepai-0.1.2/src/utils/scorer.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/src/utils/snippets.py` & `sweepai-0.1.2/src/utils/snippets.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/src/utils/utils.py` & `sweepai-0.1.2/src/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.1/setup.py` & `sweepai-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,19 +38,19 @@
  'tiktoken>=0.3.2,<0.4.0',
  'tree-sitter>=0.20.1,<0.21.0',
  'types-requests>=2.28.11.15,<3.0.0.0',
  'urllib3>=2.0.3,<3.0.0',
  'uvicorn>=0.21.0,<0.22.0']
 
 entry_points = \
-{'console_scripts': ['sweepai = src.app.sweep.py']}
+{'console_scripts': ['sweepai = src.app.sweep:app']}
 
 setup_kwargs = {
     'name': 'sweepai',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Sweep software chores',
     'long_description': None,
     'author': 'Kevin Lu',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `sweepai-0.1.1/PKG-INFO` & `sweepai-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweepai
-Version: 0.1.1
+Version: 0.1.2
 Summary: Sweep software chores
 Author: Kevin Lu
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: GitPython (>=3.1.31,<4.0.0)
 Requires-Dist: PyGithub (==1.58.2)
 Requires-Dist: PyJWT (>=2.6.0,<3.0.0)
```

