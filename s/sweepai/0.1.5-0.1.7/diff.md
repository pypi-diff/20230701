# Comparing `tmp/sweepai-0.1.5.tar.gz` & `tmp/sweepai-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweepai-0.1.5.tar", max compression
+gzip compressed data, was "sweepai-0.1.7.tar", max compression
```

## Comparing `sweepai-0.1.5.tar` & `sweepai-0.1.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.1.5/LICENSE
--rw-r--r--   0        0        0     1113 2023-07-01 08:08:56.467976 sweepai-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-15 06:30:41.945190 sweepai-0.1.5/sweepai/__init__.py
--rw-r--r--   0        0        0    10084 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/api.py
--rw-r--r--   0        0        0     3930 2023-07-01 08:08:47.031293 sweepai-0.1.5/sweepai/app/api_client.py
--rw-r--r--   0        0        0     8725 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/app/backend.py
--rw-r--r--   0        0        0     3311 2023-07-01 06:28:16.381542 sweepai-0.1.5/sweepai/app/config.py
--rw-r--r--   0        0        0      752 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/app/sweepai.py
--rw-r--r--   0        0        0     6364 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/app/ui.py
--rw-r--r--   0        0        0        0 2023-03-21 00:50:54.566288 sweepai-0.1.5/sweepai/core/__init__.py
--rw-r--r--   0        0        0    15858 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/core/chat.py
--rw-r--r--   0        0        0     2553 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/core/code_repair.py
--rw-r--r--   0        0        0     6815 2023-06-30 23:50:43.893232 sweepai-0.1.5/sweepai/core/entities.py
--rw-r--r--   0        0        0    12775 2023-06-30 23:50:43.896566 sweepai-0.1.5/sweepai/core/prompts.py
--rw-r--r--   0        0        0     3509 2023-06-21 23:04:06.027667 sweepai-0.1.5/sweepai/core/react.py
--rw-r--r--   0        0        0    15487 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/core/sweep_bot.py
--rw-r--r--   0        0        0    12335 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/core/vector_db.py
--rw-r--r--   0        0        0     2536 2023-06-16 23:50:11.723074 sweepai-0.1.5/sweepai/events.py
--rw-r--r--   0        0        0        0 2023-03-21 00:50:54.566288 sweepai-0.1.5/sweepai/handlers/__init__.py
--rw-r--r--   0        0        0     3150 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/handlers/create_pr.py
--rw-r--r--   0        0        0     5906 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/handlers/on_comment.py
--rw-r--r--   0        0        0     3423 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/handlers/on_review.py
--rw-r--r--   0        0        0    11280 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/handlers/on_ticket.py
--rw-r--r--   0        0        0    19497 2023-07-01 08:08:43.804621 sweepai-0.1.5/sweepai/slack.py
--rw-r--r--   0        0        0        0 2023-03-19 00:13:25.553442 sweepai-0.1.5/sweepai/utils/__init__.py
--rw-r--r--   0        0        0      385 2023-06-27 05:32:32.711633 sweepai-0.1.5/sweepai/utils/config.py
--rw-r--r--   0        0        0      670 2023-06-30 23:57:36.298069 sweepai-0.1.5/sweepai/utils/constants.py
--rw-r--r--   0        0        0     3633 2023-06-30 23:50:43.896566 sweepai-0.1.5/sweepai/utils/diff.py
--rw-r--r--   0        0        0      511 2023-06-15 23:48:37.899560 sweepai-0.1.5/sweepai/utils/event_logger.py
--rw-r--r--   0        0        0     5245 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/utils/file_change_functions.py
--rw-r--r--   0        0        0     8099 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/utils/github_utils.py
--rw-r--r--   0        0        0       98 2023-06-15 23:48:37.899560 sweepai-0.1.5/sweepai/utils/hash.py
--rw-r--r--   0        0        0      822 2023-06-15 23:48:37.899560 sweepai-0.1.5/sweepai/utils/huggingface.py
--rw-r--r--   0        0        0     5339 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/utils/prompt_constructor.py
--rw-r--r--   0        0        0      748 2023-06-30 23:50:43.896566 sweepai-0.1.5/sweepai/utils/scorer.py
--rw-r--r--   0        0        0     1498 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/utils/snippets.py
--rw-r--r--   0        0        0    11474 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/utils/utils.py
--rw-r--r--   0        0        0     1642 2023-07-01 08:09:02.877154 sweepai-0.1.5/setup.py
--rw-r--r--   0        0        0     1528 2023-07-01 08:09:02.877362 sweepai-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1139 2023-07-01 08:29:52.557114 sweepai-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-15 06:30:41.945190 sweepai-0.1.7/sweepai/__init__.py
+-rw-r--r--   0        0        0    10084 2023-07-01 08:08:27.324592 sweepai-0.1.7/sweepai/api.py
+-rw-r--r--   0        0        0     3958 2023-07-01 08:23:13.136307 sweepai-0.1.7/sweepai/app/api_client.py
+-rw-r--r--   0        0        0     8688 2023-07-01 08:11:53.394950 sweepai-0.1.7/sweepai/app/backend.py
+-rw-r--r--   0        0        0      752 2023-07-01 08:20:31.182615 sweepai-0.1.7/sweepai/app/cli.py
+-rw-r--r--   0        0        0     3311 2023-07-01 06:28:16.381542 sweepai-0.1.7/sweepai/app/config.py
+-rw-r--r--   0        0        0     6364 2023-07-01 08:08:27.324592 sweepai-0.1.7/sweepai/app/ui.py
+-rw-r--r--   0        0        0        0 2023-03-21 00:50:54.566288 sweepai-0.1.7/sweepai/core/__init__.py
+-rw-r--r--   0        0        0    15858 2023-07-01 08:08:27.324592 sweepai-0.1.7/sweepai/core/chat.py
+-rw-r--r--   0        0        0     2553 2023-07-01 08:08:27.324592 sweepai-0.1.7/sweepai/core/code_repair.py
+-rw-r--r--   0        0        0     6815 2023-06-30 23:50:43.893232 sweepai-0.1.7/sweepai/core/entities.py
+-rw-r--r--   0        0        0    12775 2023-06-30 23:50:43.896566 sweepai-0.1.7/sweepai/core/prompts.py
+-rw-r--r--   0        0        0     3509 2023-06-21 23:04:06.027667 sweepai-0.1.7/sweepai/core/react.py
+-rw-r--r--   0        0        0    15487 2023-07-01 08:08:27.324592 sweepai-0.1.7/sweepai/core/sweep_bot.py
+-rw-r--r--   0        0        0    12335 2023-07-01 08:08:27.324592 sweepai-0.1.7/sweepai/core/vector_db.py
+-rw-r--r--   0        0        0     2536 2023-06-16 23:50:11.723074 sweepai-0.1.7/sweepai/events.py
+-rw-r--r--   0        0        0        0 2023-03-21 00:50:54.566288 sweepai-0.1.7/sweepai/handlers/__init__.py
+-rw-r--r--   0        0        0     3150 2023-07-01 08:08:27.324592 sweepai-0.1.7/sweepai/handlers/create_pr.py
+-rw-r--r--   0        0        0     5906 2023-07-01 08:08:27.324592 sweepai-0.1.7/sweepai/handlers/on_comment.py
+-rw-r--r--   0        0        0     3423 2023-07-01 08:08:27.324592 sweepai-0.1.7/sweepai/handlers/on_review.py
+-rw-r--r--   0        0        0    11280 2023-07-01 08:08:27.324592 sweepai-0.1.7/sweepai/handlers/on_ticket.py
+-rw-r--r--   0        0        0    19497 2023-07-01 08:08:43.804621 sweepai-0.1.7/sweepai/slack.py
+-rw-r--r--   0        0        0        0 2023-03-19 00:13:25.553442 sweepai-0.1.7/sweepai/utils/__init__.py
+-rw-r--r--   0        0        0      385 2023-06-27 05:32:32.711633 sweepai-0.1.7/sweepai/utils/config.py
+-rw-r--r--   0        0        0      670 2023-06-30 23:57:36.298069 sweepai-0.1.7/sweepai/utils/constants.py
+-rw-r--r--   0        0        0     3633 2023-06-30 23:50:43.896566 sweepai-0.1.7/sweepai/utils/diff.py
+-rw-r--r--   0        0        0      511 2023-06-15 23:48:37.899560 sweepai-0.1.7/sweepai/utils/event_logger.py
+-rw-r--r--   0        0        0     5245 2023-07-01 08:08:27.324592 sweepai-0.1.7/sweepai/utils/file_change_functions.py
+-rw-r--r--   0        0        0     8099 2023-07-01 08:08:27.324592 sweepai-0.1.7/sweepai/utils/github_utils.py
+-rw-r--r--   0        0        0       98 2023-06-15 23:48:37.899560 sweepai-0.1.7/sweepai/utils/hash.py
+-rw-r--r--   0        0        0      822 2023-06-15 23:48:37.899560 sweepai-0.1.7/sweepai/utils/huggingface.py
+-rw-r--r--   0        0        0     5339 2023-07-01 08:08:27.324592 sweepai-0.1.7/sweepai/utils/prompt_constructor.py
+-rw-r--r--   0        0        0      748 2023-06-30 23:50:43.896566 sweepai-0.1.7/sweepai/utils/scorer.py
+-rw-r--r--   0        0        0     1498 2023-07-01 08:08:27.324592 sweepai-0.1.7/sweepai/utils/snippets.py
+-rw-r--r--   0        0        0    11474 2023-07-01 08:08:27.324592 sweepai-0.1.7/sweepai/utils/utils.py
+-rw-r--r--   0        0        0     1690 2023-07-01 08:30:13.086476 sweepai-0.1.7/setup.py
+-rw-r--r--   0        0        0     1528 2023-07-01 08:30:13.086691 sweepai-0.1.7/PKG-INFO
```

### Comparing `sweepai-0.1.5/LICENSE` & `sweepai-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.5/pyproject.toml` & `sweepai-0.1.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sweepai"
-version = "0.1.5"
+version = "0.1.7"
 description = "Sweep software chores"
 authors = ["Kevin Lu", "William Zeng", "Luke Jagg"]
 packages = [
     { include = "sweepai" }
 ]
 
 [tool.poetry.dependencies]
@@ -48,8 +48,9 @@
 jupyter = "^1.0.0"
 ipykernel = "^6.23.1"
 
 [mypy]
 check_untyped_defs = true
 
 [tool.poetry.scripts]
-sweepai = "sweepai.app.sweepai:app"
+sweep = "sweepai.app.cli:app"
+sweepai = "sweepai.app.cli:app"
```

### Comparing `sweepai-0.1.5/sweepai/api.py` & `sweepai-0.1.7/sweepai/api.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.5/sweepai/app/api_client.py` & `sweepai-0.1.7/sweepai/app/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,14 +52,15 @@
             self.api_endpoint + "/search",
             json={
                 "query": query,
                 "n_results": n_results,
                 "config": self.config.dict(),
             }
         )
+        print(results.text)
         snippets = [Snippet(**item) for item in results.json()]
         return snippets
     
     def create_pr(
         self,
         file_change_requests: list[tuple[str, str]],
         pull_request: PullRequest,
```

### Comparing `sweepai-0.1.5/sweepai/app/backend.py` & `sweepai-0.1.7/sweepai/app/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,11 +231,11 @@
         system_message = gradio_system_message_prompt.format(
             snippets="\n".join([snippet.denotation + f"\n```{snippet.get_snippet()}```" for snippet in request.snippets]),
             repo_name=request.config.repo_full_name,
             repo_description="" # TODO: fill this
         )
         chatgpt = ChatGPT(messages=[Message(role="system", content=system_message, key="system")] + messages[:-1])
         return StreamingResponse(
-            (json.dumps(chunk) for chunk in chatgpt.chat_stream(messages[-1].content, model="gpt-4-0613", functions=functions, function_call={"name": "create_pr"})),
+            (json.dumps(chunk) for chunk in chatgpt.chat_stream(messages[-1].content, model="gpt-4-0613", functions=functions)),
             media_type="text/event-stream"
         )
     return app
```

### Comparing `sweepai-0.1.5/sweepai/app/config.py` & `sweepai-0.1.7/sweepai/app/config.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.5/sweepai/app/sweepai.py` & `sweepai-0.1.7/sweepai/app/cli.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.5/sweepai/app/ui.py` & `sweepai-0.1.7/sweepai/app/ui.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.5/sweepai/core/chat.py` & `sweepai-0.1.7/sweepai/core/chat.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.5/sweepai/core/code_repair.py` & `sweepai-0.1.7/sweepai/core/code_repair.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.5/sweepai/core/entities.py` & `sweepai-0.1.7/sweepai/core/entities.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.5/sweepai/core/prompts.py` & `sweepai-0.1.7/sweepai/core/prompts.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.5/sweepai/core/react.py` & `sweepai-0.1.7/sweepai/core/react.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.5/sweepai/core/sweep_bot.py` & `sweepai-0.1.7/sweepai/core/sweep_bot.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.5/sweepai/core/vector_db.py` & `sweepai-0.1.7/sweepai/core/vector_db.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.5/sweepai/events.py` & `sweepai-0.1.7/sweepai/events.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.5/sweepai/handlers/create_pr.py` & `sweepai-0.1.7/sweepai/handlers/create_pr.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.5/sweepai/handlers/on_comment.py` & `sweepai-0.1.7/sweepai/handlers/on_comment.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.5/sweepai/handlers/on_review.py` & `sweepai-0.1.7/sweepai/handlers/on_review.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.5/sweepai/handlers/on_ticket.py` & `sweepai-0.1.7/sweepai/handlers/on_ticket.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.5/sweepai/slack.py` & `sweepai-0.1.7/sweepai/slack.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.5/sweepai/utils/constants.py` & `sweepai-0.1.7/sweepai/utils/constants.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.5/sweepai/utils/diff.py` & `sweepai-0.1.7/sweepai/utils/diff.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.5/sweepai/utils/file_change_functions.py` & `sweepai-0.1.7/sweepai/utils/file_change_functions.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.5/sweepai/utils/github_utils.py` & `sweepai-0.1.7/sweepai/utils/github_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.5/sweepai/utils/huggingface.py` & `sweepai-0.1.7/sweepai/utils/huggingface.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.5/sweepai/utils/prompt_constructor.py` & `sweepai-0.1.7/sweepai/utils/prompt_constructor.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.5/sweepai/utils/scorer.py` & `sweepai-0.1.7/sweepai/utils/scorer.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.5/sweepai/utils/snippets.py` & `sweepai-0.1.7/sweepai/utils/snippets.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.5/sweepai/utils/utils.py` & `sweepai-0.1.7/sweepai/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.5/setup.py` & `sweepai-0.1.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,19 +38,20 @@
  'tiktoken>=0.3.2,<0.4.0',
  'tree-sitter>=0.20.1,<0.21.0',
  'types-requests>=2.28.11.15,<3.0.0.0',
  'urllib3>=2.0.3,<3.0.0',
  'uvicorn>=0.21.0,<0.22.0']
 
 entry_points = \
-{'console_scripts': ['sweepai = sweepai.app.sweepai:app']}
+{'console_scripts': ['sweep = sweepai.app.cli:app',
+                     'sweepai = sweepai.app.cli:app']}
 
 setup_kwargs = {
     'name': 'sweepai',
-    'version': '0.1.5',
+    'version': '0.1.7',
     'description': 'Sweep software chores',
     'long_description': None,
     'author': 'Kevin Lu',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `sweepai-0.1.5/PKG-INFO` & `sweepai-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweepai
-Version: 0.1.5
+Version: 0.1.7
 Summary: Sweep software chores
 Author: Kevin Lu
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: GitPython (>=3.1.31,<4.0.0)
 Requires-Dist: PyGithub (==1.58.2)
 Requires-Dist: PyJWT (>=2.6.0,<3.0.0)
```

