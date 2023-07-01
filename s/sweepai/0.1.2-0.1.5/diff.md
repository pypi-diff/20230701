# Comparing `tmp/sweepai-0.1.2.tar.gz` & `tmp/sweepai-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweepai-0.1.2.tar", max compression
+gzip compressed data, was "sweepai-0.1.5.tar", max compression
```

## Comparing `sweepai-0.1.2.tar` & `sweepai-0.1.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.1.2/LICENSE
--rw-r--r--   0        0        0     1103 2023-07-01 07:52:45.459406 sweepai-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-15 06:30:41.945190 sweepai-0.1.2/src/__init__.py
--rw-r--r--   0        0        0    10056 2023-06-30 23:50:43.893232 sweepai-0.1.2/src/api.py
--rw-r--r--   0        0        0     3918 2023-07-01 07:28:30.813206 sweepai-0.1.2/src/app/api_client.py
--rw-r--r--   0        0        0     8697 2023-07-01 06:53:00.643340 sweepai-0.1.2/src/app/backend.py
--rw-r--r--   0        0        0     3311 2023-07-01 06:28:16.381542 sweepai-0.1.2/src/app/config.py
--rw-r--r--   0        0        0      744 2023-07-01 06:34:10.612287 sweepai-0.1.2/src/app/sweepai.py
--rw-r--r--   0        0        0     6348 2023-07-01 06:20:34.657237 sweepai-0.1.2/src/app/ui.py
--rw-r--r--   0        0        0        0 2023-03-21 00:50:54.566288 sweepai-0.1.2/src/core/__init__.py
--rw-r--r--   0        0        0    15838 2023-06-30 23:50:43.893232 sweepai-0.1.2/src/core/chat.py
--rw-r--r--   0        0        0     2541 2023-06-30 23:50:43.893232 sweepai-0.1.2/src/core/code_repair.py
--rw-r--r--   0        0        0     6815 2023-06-30 23:50:43.893232 sweepai-0.1.2/src/core/entities.py
--rw-r--r--   0        0        0    12775 2023-06-30 23:50:43.896566 sweepai-0.1.2/src/core/prompts.py
--rw-r--r--   0        0        0     3509 2023-06-21 23:04:06.027667 sweepai-0.1.2/src/core/react.py
--rw-r--r--   0        0        0    15463 2023-07-01 03:28:14.554557 sweepai-0.1.2/src/core/sweep_bot.py
--rw-r--r--   0        0        0    12319 2023-06-30 23:50:43.896566 sweepai-0.1.2/src/core/vector_db.py
--rw-r--r--   0        0        0     2536 2023-06-16 23:50:11.723074 sweepai-0.1.2/src/events.py
--rw-r--r--   0        0        0        0 2023-03-21 00:50:54.566288 sweepai-0.1.2/src/handlers/__init__.py
--rw-r--r--   0        0        0     3126 2023-06-30 07:26:46.313809 sweepai-0.1.2/src/handlers/create_pr.py
--rw-r--r--   0        0        0     5882 2023-06-30 23:50:43.896566 sweepai-0.1.2/src/handlers/on_comment.py
--rw-r--r--   0        0        0     3403 2023-06-30 23:50:43.896566 sweepai-0.1.2/src/handlers/on_review.py
--rw-r--r--   0        0        0    11236 2023-06-30 23:50:43.896566 sweepai-0.1.2/src/handlers/on_ticket.py
--rw-r--r--   0        0        0    19469 2023-06-27 19:07:01.581627 sweepai-0.1.2/src/slack.py
--rw-r--r--   0        0        0        0 2023-03-19 00:13:25.553442 sweepai-0.1.2/src/utils/__init__.py
--rw-r--r--   0        0        0      385 2023-06-27 05:32:32.711633 sweepai-0.1.2/src/utils/config.py
--rw-r--r--   0        0        0      670 2023-06-30 23:57:36.298069 sweepai-0.1.2/src/utils/constants.py
--rw-r--r--   0        0        0     3633 2023-06-30 23:50:43.896566 sweepai-0.1.2/src/utils/diff.py
--rw-r--r--   0        0        0      511 2023-06-15 23:48:37.899560 sweepai-0.1.2/src/utils/event_logger.py
--rw-r--r--   0        0        0     5237 2023-06-26 21:11:27.030016 sweepai-0.1.2/src/utils/file_change_functions.py
--rw-r--r--   0        0        0     8083 2023-06-27 05:32:32.714966 sweepai-0.1.2/src/utils/github_utils.py
--rw-r--r--   0        0        0       98 2023-06-15 23:48:37.899560 sweepai-0.1.2/src/utils/hash.py
--rw-r--r--   0        0        0      822 2023-06-15 23:48:37.899560 sweepai-0.1.2/src/utils/huggingface.py
--rw-r--r--   0        0        0     5335 2023-06-30 23:50:43.896566 sweepai-0.1.2/src/utils/prompt_constructor.py
--rw-r--r--   0        0        0      748 2023-06-30 23:50:43.896566 sweepai-0.1.2/src/utils/scorer.py
--rw-r--r--   0        0        0     1490 2023-06-26 21:11:27.030016 sweepai-0.1.2/src/utils/snippets.py
--rw-r--r--   0        0        0    11470 2023-06-30 23:50:43.896566 sweepai-0.1.2/src/utils/utils.py
--rw-r--r--   0        0        0     1616 2023-07-01 07:52:47.673708 sweepai-0.1.2/setup.py
--rw-r--r--   0        0        0     1528 2023-07-01 07:52:47.674046 sweepai-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1113 2023-07-01 08:08:56.467976 sweepai-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-15 06:30:41.945190 sweepai-0.1.5/sweepai/__init__.py
+-rw-r--r--   0        0        0    10084 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/api.py
+-rw-r--r--   0        0        0     3930 2023-07-01 08:08:47.031293 sweepai-0.1.5/sweepai/app/api_client.py
+-rw-r--r--   0        0        0     8725 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/app/backend.py
+-rw-r--r--   0        0        0     3311 2023-07-01 06:28:16.381542 sweepai-0.1.5/sweepai/app/config.py
+-rw-r--r--   0        0        0      752 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/app/sweepai.py
+-rw-r--r--   0        0        0     6364 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/app/ui.py
+-rw-r--r--   0        0        0        0 2023-03-21 00:50:54.566288 sweepai-0.1.5/sweepai/core/__init__.py
+-rw-r--r--   0        0        0    15858 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/core/chat.py
+-rw-r--r--   0        0        0     2553 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/core/code_repair.py
+-rw-r--r--   0        0        0     6815 2023-06-30 23:50:43.893232 sweepai-0.1.5/sweepai/core/entities.py
+-rw-r--r--   0        0        0    12775 2023-06-30 23:50:43.896566 sweepai-0.1.5/sweepai/core/prompts.py
+-rw-r--r--   0        0        0     3509 2023-06-21 23:04:06.027667 sweepai-0.1.5/sweepai/core/react.py
+-rw-r--r--   0        0        0    15487 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/core/sweep_bot.py
+-rw-r--r--   0        0        0    12335 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/core/vector_db.py
+-rw-r--r--   0        0        0     2536 2023-06-16 23:50:11.723074 sweepai-0.1.5/sweepai/events.py
+-rw-r--r--   0        0        0        0 2023-03-21 00:50:54.566288 sweepai-0.1.5/sweepai/handlers/__init__.py
+-rw-r--r--   0        0        0     3150 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/handlers/create_pr.py
+-rw-r--r--   0        0        0     5906 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/handlers/on_comment.py
+-rw-r--r--   0        0        0     3423 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/handlers/on_review.py
+-rw-r--r--   0        0        0    11280 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/handlers/on_ticket.py
+-rw-r--r--   0        0        0    19497 2023-07-01 08:08:43.804621 sweepai-0.1.5/sweepai/slack.py
+-rw-r--r--   0        0        0        0 2023-03-19 00:13:25.553442 sweepai-0.1.5/sweepai/utils/__init__.py
+-rw-r--r--   0        0        0      385 2023-06-27 05:32:32.711633 sweepai-0.1.5/sweepai/utils/config.py
+-rw-r--r--   0        0        0      670 2023-06-30 23:57:36.298069 sweepai-0.1.5/sweepai/utils/constants.py
+-rw-r--r--   0        0        0     3633 2023-06-30 23:50:43.896566 sweepai-0.1.5/sweepai/utils/diff.py
+-rw-r--r--   0        0        0      511 2023-06-15 23:48:37.899560 sweepai-0.1.5/sweepai/utils/event_logger.py
+-rw-r--r--   0        0        0     5245 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/utils/file_change_functions.py
+-rw-r--r--   0        0        0     8099 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/utils/github_utils.py
+-rw-r--r--   0        0        0       98 2023-06-15 23:48:37.899560 sweepai-0.1.5/sweepai/utils/hash.py
+-rw-r--r--   0        0        0      822 2023-06-15 23:48:37.899560 sweepai-0.1.5/sweepai/utils/huggingface.py
+-rw-r--r--   0        0        0     5339 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/utils/prompt_constructor.py
+-rw-r--r--   0        0        0      748 2023-06-30 23:50:43.896566 sweepai-0.1.5/sweepai/utils/scorer.py
+-rw-r--r--   0        0        0     1498 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/utils/snippets.py
+-rw-r--r--   0        0        0    11474 2023-07-01 08:08:27.324592 sweepai-0.1.5/sweepai/utils/utils.py
+-rw-r--r--   0        0        0     1642 2023-07-01 08:09:02.877154 sweepai-0.1.5/setup.py
+-rw-r--r--   0        0        0     1528 2023-07-01 08:09:02.877362 sweepai-0.1.5/PKG-INFO
```

### Comparing `sweepai-0.1.2/LICENSE` & `sweepai-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.2/pyproject.toml` & `sweepai-0.1.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "sweepai"
-version = "0.1.2"
+version = "0.1.5"
 description = "Sweep software chores"
 authors = ["Kevin Lu", "William Zeng", "Luke Jagg"]
 packages = [
-    { include = "src" }
+    { include = "sweepai" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 openai = "^0.27.2"
 python-dotenv = "^1.0.0"
 fastapi = "^0.94.1"
@@ -48,8 +48,8 @@
 jupyter = "^1.0.0"
 ipykernel = "^6.23.1"
 
 [mypy]
 check_untyped_defs = true
 
 [tool.poetry.scripts]
-sweepai = "src.app.sweep:app"
+sweepai = "sweepai.app.sweepai:app"
```

### Comparing `sweepai-0.1.2/src/api.py` & `sweepai-0.1.5/sweepai/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import time
 from loguru import logger
 import modal
 from pydantic import ValidationError
-from src.handlers.create_pr import create_pr  # type: ignore
+from sweepai.handlers.create_pr import create_pr  # type: ignore
 
-from src.handlers.on_ticket import on_ticket
-from src.handlers.on_comment import on_comment
-from src.utils.constants import API_NAME, BOT_TOKEN_NAME, LABEL_COLOR, LABEL_DESCRIPTION, LABEL_NAME, SWEEP_LOGIN
-from src.events import (
+from sweepai.handlers.on_ticket import on_ticket
+from sweepai.handlers.on_comment import on_comment
+from sweepai.utils.constants import API_NAME, BOT_TOKEN_NAME, LABEL_COLOR, LABEL_DESCRIPTION, LABEL_NAME, SWEEP_LOGIN
+from sweepai.events import (
     CommentCreatedRequest,
     InstallationCreatedRequest,
     IssueCommentRequest,
     IssueRequest,
     PRRequest,
     ReposAddedRequest,
 )
-from src.utils.event_logger import posthog
-from src.utils.github_utils import get_github_client, index_full_repository
+from sweepai.utils.event_logger import posthog
+from sweepai.utils.github_utils import get_github_client, index_full_repository
 from fastapi import HTTPException, Request
 
 stub = modal.Stub(API_NAME)
 image = (
     modal.Image.debian_slim()
     .apt_install("git")
     .pip_install(
```

### Comparing `sweepai-0.1.2/src/app/api_client.py` & `sweepai-0.1.5/sweepai/app/api_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import webbrowser
 import httpx
 from pydantic import BaseModel
 import requests
 import json
 from loguru import logger
 
-from src.app.config import SweepChatConfig
-from src.core.entities import PullRequest, Snippet
-from src.utils.constants import PREFIX
+from sweepai.app.config import SweepChatConfig
+from sweepai.core.entities import PullRequest, Snippet
+from sweepai.utils.constants import PREFIX
 
 def break_json(raw_json: str):
     # turns something like {"function_call": {"arguments": " \""}}{"function_call": {"arguments": "summary"}} into two objects
     try:
         yield json.loads(raw_json)
     except json.JSONDecodeError:
         for i in range(1, len(raw_json)):
```

### Comparing `sweepai-0.1.2/src/app/backend.py` & `sweepai-0.1.5/sweepai/app/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 import fastapi
 from github import Github
 import modal
 from loguru import logger
 from fastapi import FastAPI
 from fastapi.responses import StreamingResponse
 from pydantic import BaseModel
-from src.app.config import SweepChatConfig
+from sweepai.app.config import SweepChatConfig
 
-from src.core.chat import ChatGPT
-from src.core.entities import FileChangeRequest, Function, Message, PullRequest, Snippet
-from src.core.sweep_bot import SweepBot
-from src.utils.constants import API_NAME, BOT_TOKEN_NAME, DB_NAME, PREFIX
-from src.utils.github_utils import get_github_client, get_installation_id
-from src.core.prompts import gradio_system_message_prompt
+from sweepai.core.chat import ChatGPT
+from sweepai.core.entities import FileChangeRequest, Function, Message, PullRequest, Snippet
+from sweepai.core.sweep_bot import SweepBot
+from sweepai.utils.constants import API_NAME, BOT_TOKEN_NAME, DB_NAME, PREFIX
+from sweepai.utils.github_utils import get_github_client, get_installation_id
+from sweepai.core.prompts import gradio_system_message_prompt
 
 get_relevant_snippets = modal.Function.from_name(DB_NAME, "get_relevant_snippets")
 
 stub = modal.Stub(PREFIX + "-ui")
 image = (
     modal.Image.debian_slim()
     .apt_install("git")
```

### Comparing `sweepai-0.1.2/src/app/config.py` & `sweepai-0.1.5/sweepai/app/config.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.2/src/app/sweepai.py` & `sweepai-0.1.5/sweepai/app/sweepai.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import typer
 from rich import print
 
-from src.app.config import SweepChatConfig
+from sweepai.app.config import SweepChatConfig
 
 epilog = "Sweep is a AI junior developer. Docs at https://docs.sweep.dev, install at https://github.com/apps/sweep-ai and support at https://discord.gg/sweep-ai."
 
 app = typer.Typer(epilog=epilog)
 
 @app.command()
 def start():
     """
     Launch Sweep Chat in the browser
     """
     SweepChatConfig.load()
-    from src.app.ui import demo
+    from sweepai.app.ui import demo
     demo.queue()
     demo.launch(enable_queue=True, inbrowser=True)
     
 @app.command()
 def auth():
     """
     Reauthenticate with Github API for Sweep to work (for token expiry)
```

### Comparing `sweepai-0.1.2/src/app/ui.py` & `sweepai-0.1.5/sweepai/app/ui.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 from github import Github
 import gradio as gr
 from loguru import logger
 import modal
 
-from src.app.api_client import APIClient
-from src.app.config import SweepChatConfig
-from src.core.entities import Snippet
-from src.utils.constants import DB_NAME
+from sweepai.app.api_client import APIClient
+from sweepai.app.config import SweepChatConfig
+from sweepai.core.entities import Snippet
+from sweepai.utils.constants import DB_NAME
 
 get_relevant_snippets = modal.Function.lookup(DB_NAME, "get_relevant_snippets")
 config = SweepChatConfig.load()
 
 api_client = APIClient(config=config)
 
 pr_summary_template = """💡 I'll create the following PR:
```

### Comparing `sweepai-0.1.2/src/core/chat.py` & `sweepai-0.1.5/sweepai/core/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 import modal
 import openai
 import anthropic
 from loguru import logger
 from pydantic import BaseModel
 import backoff
 
-from src.core.entities import (
+from sweepai.core.entities import (
     Function,
     Message,
 )
-from src.core.prompts import (
+from sweepai.core.prompts import (
     system_message_prompt,
     system_message_issue_comment_prompt,
 )
-from src.utils.constants import UTILS_NAME
-from src.utils.prompt_constructor import HumanMessagePrompt
-from src.core.entities import Message, Function
+from sweepai.utils.constants import UTILS_NAME
+from sweepai.utils.prompt_constructor import HumanMessagePrompt
+from sweepai.core.entities import Message, Function
 
 # TODO: combine anthropic and openai
 
 AnthropicModel = (
     Literal["claude-v1"]
     | Literal["claude-v1.3-100k"]
     | Literal["claude-instant-v1.1-100k"]
```

### Comparing `sweepai-0.1.2/src/core/code_repair.py` & `sweepai-0.1.5/sweepai/core/code_repair.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 import subprocess
-from src.core.chat import ChatGPT
-from src.core.entities import Message
-from src.core.prompts import code_repair_system_prompt, code_repair_prompt
+from sweepai.core.chat import ChatGPT
+from sweepai.core.entities import Message
+from sweepai.core.prompts import code_repair_system_prompt, code_repair_prompt
 
 response_regex = r"```[^\n]*(?P<response>.+)```"
 
 
 class CodeRepairer(ChatGPT):
     # idk why this part breaks
     # messages: list[Message] = [Message(role="system", content=code_repair_system_prompt)]
```

### Comparing `sweepai-0.1.2/src/core/entities.py` & `sweepai-0.1.5/sweepai/core/entities.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.2/src/core/prompts.py` & `sweepai-0.1.5/sweepai/core/prompts.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.2/src/core/react.py` & `sweepai-0.1.5/sweepai/core/react.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.2/src/core/sweep_bot.py` & `sweepai-0.1.5/sweepai/core/sweep_bot.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,35 +2,35 @@
 from loguru import logger
 import github
 from github.Repository import Repository
 from github.ContentFile import ContentFile
 from github.GithubException import GithubException
 import modal
 from pydantic import BaseModel
-from src.core.code_repair import CodeRepairer
+from sweepai.core.code_repair import CodeRepairer
 
-from src.core.entities import (
+from sweepai.core.entities import (
     FileChange,
     FileChangeRequest,
     FilesToChange,
     PullRequest,
     RegexMatchError,
     Function,
     Snippet
 )
-from src.core.chat import ChatGPT
-from src.core.prompts import (
+from sweepai.core.chat import ChatGPT
+from sweepai.core.prompts import (
     files_to_change_prompt,
     pull_request_prompt,
     create_file_prompt,
     modify_file_prompt,
     modify_file_plan_prompt,
 )
-from src.utils.constants import DB_NAME
-from src.utils.diff import format_contents, generate_diff, generate_new_file, is_markdown
+from sweepai.utils.constants import DB_NAME
+from sweepai.utils.diff import format_contents, generate_diff, generate_new_file, is_markdown
 
 
 class CodeGenBot(ChatGPT):
 
     def get_files_to_change(self):
         file_change_requests: list[FileChangeRequest] = []
         for count in range(5):
```

### Comparing `sweepai-0.1.2/src/core/vector_db.py` & `sweepai-0.1.5/sweepai/core/vector_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 from tqdm import tqdm
 import modal
 from modal import method
 from deeplake.core.vectorstore.deeplake_vectorstore import DeepLakeVectorStore
 from github import Github
 from git import Repo
 
-from src.core.entities import Snippet
-from src.utils.event_logger import posthog
-from src.utils.hash import hash_sha256
-from src.utils.scorer import compute_score
+from sweepai.core.entities import Snippet
+from sweepai.utils.event_logger import posthog
+from sweepai.utils.hash import hash_sha256
+from sweepai.utils.scorer import compute_score
 
 from ..utils.github_utils import get_token
 from ..utils.constants import DB_NAME, BOT_TOKEN_NAME, ENV, UTILS_NAME
 from ..utils.config import SweepConfig
 import time
 
 # TODO: Lots of cleanups can be done here with these constants
```

### Comparing `sweepai-0.1.2/src/events.py` & `sweepai-0.1.5/sweepai/events.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.2/src/handlers/create_pr.py` & `sweepai-0.1.5/sweepai/handlers/create_pr.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 import os
 import openai
 
 from loguru import logger
 import modal
 
-from src.core.entities import FileChangeRequest, PullRequest
-from src.core.sweep_bot import SweepBot
-from src.handlers.on_review import review_pr
-from src.utils.event_logger import posthog
-from src.utils.github_utils import get_github_client
-from src.utils.constants import DB_NAME, PREFIX
+from sweepai.core.entities import FileChangeRequest, PullRequest
+from sweepai.core.sweep_bot import SweepBot
+from sweepai.handlers.on_review import review_pr
+from sweepai.utils.event_logger import posthog
+from sweepai.utils.github_utils import get_github_client
+from sweepai.utils.constants import DB_NAME, PREFIX
 
 github_access_token = os.environ.get("GITHUB_TOKEN")
 openai.api_key = os.environ.get("OPENAI_API_KEY")
 
 update_index = modal.Function.lookup(DB_NAME, "update_index")
 
 num_of_snippets_to_query = 10
```

### Comparing `sweepai-0.1.2/src/handlers/on_comment.py` & `sweepai-0.1.5/sweepai/handlers/on_comment.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 # TODO: Add file validation
 
 import os
 import openai
 
 from loguru import logger
 
-from src.core.sweep_bot import SweepBot
-from src.handlers.on_review import get_pr_diffs
-from src.utils.event_logger import posthog
-from src.utils.github_utils import (
+from sweepai.core.sweep_bot import SweepBot
+from sweepai.handlers.on_review import get_pr_diffs
+from sweepai.utils.event_logger import posthog
+from sweepai.utils.github_utils import (
     get_github_client,
     search_snippets,
 )
-from src.utils.prompt_constructor import HumanMessageCommentPrompt
-from src.utils.constants import PREFIX
+from sweepai.utils.prompt_constructor import HumanMessageCommentPrompt
+from sweepai.utils.constants import PREFIX
 
 github_access_token = os.environ.get("GITHUB_TOKEN")
 openai.api_key = os.environ.get("OPENAI_API_KEY")
 
 
 def on_comment(
     repo_full_name: str,
```

### Comparing `sweepai-0.1.2/src/handlers/on_review.py` & `sweepai-0.1.5/sweepai/handlers/on_review.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Take a PR and provide an AI generated review of the PR.
 """
 from loguru import logger
-from src.core.entities import DiffSummarization, PullRequestComment
-from src.core.prompts import review_prompt
-from src.core.sweep_bot import SweepBot
+from sweepai.core.entities import DiffSummarization, PullRequestComment
+from sweepai.core.prompts import review_prompt
+from sweepai.core.sweep_bot import SweepBot
 
-from src.utils.github_utils import get_file_contents
-from src.utils.prompt_constructor import HumanMessageFinalPRComment, HumanMessagePromptReview, HumanMessageReviewFollowup
+from sweepai.utils.github_utils import get_file_contents
+from sweepai.utils.prompt_constructor import HumanMessageFinalPRComment, HumanMessagePromptReview, HumanMessageReviewFollowup
 
 # Plan:
 # 1. Get PR
 # 2. Get files changed
 # 3. Come up with some comments for the PR
 # 4. Take comments and add them to the PR
```

### Comparing `sweepai-0.1.2/src/handlers/on_ticket.py` & `sweepai-0.1.5/sweepai/handlers/on_ticket.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 import os
 import openai
 
 from loguru import logger
 import modal
 
-from src.core.entities import FileChangeRequest, Snippet
-from src.core.prompts import (
+from sweepai.core.entities import FileChangeRequest, Snippet
+from sweepai.core.prompts import (
     reply_prompt,
 )
-from src.core.sweep_bot import SweepBot
-from src.core.prompts import issue_comment_prompt
-from src.handlers.create_pr import create_pr
-from src.handlers.on_comment import on_comment
-from src.handlers.on_review import review_pr
-from src.utils.event_logger import posthog
-from src.utils.github_utils import get_github_client, search_snippets
-from src.utils.prompt_constructor import HumanMessagePrompt
-from src.utils.constants import DB_NAME, PREFIX, UTILS_NAME
+from sweepai.core.sweep_bot import SweepBot
+from sweepai.core.prompts import issue_comment_prompt
+from sweepai.handlers.create_pr import create_pr
+from sweepai.handlers.on_comment import on_comment
+from sweepai.handlers.on_review import review_pr
+from sweepai.utils.event_logger import posthog
+from sweepai.utils.github_utils import get_github_client, search_snippets
+from sweepai.utils.prompt_constructor import HumanMessagePrompt
+from sweepai.utils.constants import DB_NAME, PREFIX, UTILS_NAME
 
 github_access_token = os.environ.get("GITHUB_TOKEN")
 openai.api_key = os.environ.get("OPENAI_API_KEY")
 
 update_index = modal.Function.lookup(DB_NAME, "update_index")
 
 bot_suffix = "I'm a bot that handles simple bugs and feature requests \
```

### Comparing `sweepai-0.1.2/src/slack.py` & `sweepai-0.1.5/sweepai/slack.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 from fastapi import FastAPI, HTTPException, Request, Response
 from fastapi.responses import RedirectResponse
 
 import modal
 from pydantic import BaseModel
 from pymongo import MongoClient
 import requests
-from src.core.entities import FileChangeRequest, Function, PullRequest
+from sweepai.core.entities import FileChangeRequest, Function, PullRequest
 import slack_sdk
 from loguru import logger
 from slack_sdk.oauth.installation_store import Installation, InstallationStore, Bot
 
-from src.core.sweep_bot import SweepBot
-from src.utils.github_utils import get_github_client
-from src.utils.constants import API_NAME, BOT_TOKEN_NAME, PREFIX, SLACK_NAME
-from src.core.prompts import slack_slash_command_prompt
-from src.utils.github_utils import get_installation_id
-import src.utils.event_logger
+from sweepai.core.sweep_bot import SweepBot
+from sweepai.utils.github_utils import get_github_client
+from sweepai.utils.constants import API_NAME, BOT_TOKEN_NAME, PREFIX, SLACK_NAME
+from sweepai.core.prompts import slack_slash_command_prompt
+from sweepai.utils.github_utils import get_installation_id
+import sweepai.utils.event_logger
 
 image = modal.Image \
     .debian_slim() \
     .apt_install("git") \
     .pip_install(
         "slack-sdk",
         "slack-bolt",
```

### Comparing `sweepai-0.1.2/src/utils/constants.py` & `sweepai-0.1.5/sweepai/utils/constants.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.2/src/utils/diff.py` & `sweepai-0.1.5/sweepai/utils/diff.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.2/src/utils/file_change_functions.py` & `sweepai-0.1.5/sweepai/utils/file_change_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from loguru import logger
-from src.core.chat import Function
-from src.utils.diff import format_contents
+from sweepai.core.chat import Function
+from sweepai.utils.diff import format_contents
 
 modify_file_function = Function(
     name="modify_file",
     description="Edits the code in a file. Use start_line and end_line to completely cover the line indexes of code that should be replaced. Indent and format the code in the edits. Output the code in the order it should appear in the file. Make sure start_line and end_line do not overlap between code edits.",
     parameters={
         "type": "object",
         "properties": {
```

### Comparing `sweepai-0.1.2/src/utils/github_utils.py` & `sweepai-0.1.5/sweepai/utils/github_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 from github.Repository import Repository
 from loguru import logger
 from git import Repo
 
 from jwt import encode
 import requests
 from tqdm import tqdm
-from src.core.entities import Snippet
-from src.utils.config import SweepConfig
-from src.utils.constants import APP_ID, DB_NAME
-from src.utils.event_logger import posthog
+from sweepai.core.entities import Snippet
+from sweepai.utils.config import SweepConfig
+from sweepai.utils.constants import APP_ID, DB_NAME
+from sweepai.utils.event_logger import posthog
 
 
 def make_valid_string(string: str):
     pattern = r"[^\w./-]+"
     return re.sub(pattern, "_", string)
```

### Comparing `sweepai-0.1.2/src/utils/huggingface.py` & `sweepai-0.1.5/sweepai/utils/huggingface.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.2/src/utils/prompt_constructor.py` & `sweepai-0.1.5/sweepai/utils/prompt_constructor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pydantic import BaseModel
-from src.core.prompts import (
+from sweepai.core.prompts import (
     human_message_prompt,
     human_message_prompt_comment,
     human_message_review_prompt,
     diff_section_prompt,
     review_follow_up_prompt,
     final_review_prompt,
     comment_line_prompt
```

### Comparing `sweepai-0.1.2/src/utils/scorer.py` & `sweepai-0.1.5/sweepai/utils/scorer.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.2/src/utils/snippets.py` & `sweepai-0.1.5/sweepai/utils/snippets.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from loguru import logger
 import modal
 
-from src.core.chat import Snippet
-from src.utils.constants import UTILS_NAME
+from sweepai.core.chat import Snippet
+from sweepai.utils.constants import UTILS_NAME
 
 chunker = modal.Function.lookup(UTILS_NAME, "Chunking.chunk")
 
 def format_snippets(snippets: list[Snippet]):
     snippets: list[Snippet] = snippets[::-1]
 
     num_full_files = 3
```

### Comparing `sweepai-0.1.2/src/utils/utils.py` & `sweepai-0.1.5/sweepai/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from dataclasses import dataclass
 import re
 
 import modal
 from modal import method
 from loguru import logger
 
-from src.utils.constants import UTILS_NAME
+from sweepai.utils.constants import UTILS_NAME
 
 stub = modal.Stub(UTILS_NAME)
 tiktoken_image = modal.Image.debian_slim().pip_install("tiktoken", "loguru", "anthropic")
 
 TIKTOKEN_CACHE_DIR = "/root/cache/tiktoken"
 tiktoken_volume = modal.SharedVolume().persist("tiktoken-models")
```

### Comparing `sweepai-0.1.2/setup.py` & `sweepai-0.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['src', 'src.app', 'src.core', 'src.handlers', 'src.utils']
+['sweepai', 'sweepai.app', 'sweepai.core', 'sweepai.handlers', 'sweepai.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['GitPython>=3.1.31,<4.0.0',
  'PyGithub==1.58.2',
@@ -38,19 +38,19 @@
  'tiktoken>=0.3.2,<0.4.0',
  'tree-sitter>=0.20.1,<0.21.0',
  'types-requests>=2.28.11.15,<3.0.0.0',
  'urllib3>=2.0.3,<3.0.0',
  'uvicorn>=0.21.0,<0.22.0']
 
 entry_points = \
-{'console_scripts': ['sweepai = src.app.sweep:app']}
+{'console_scripts': ['sweepai = sweepai.app.sweepai:app']}
 
 setup_kwargs = {
     'name': 'sweepai',
-    'version': '0.1.2',
+    'version': '0.1.5',
     'description': 'Sweep software chores',
     'long_description': None,
     'author': 'Kevin Lu',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `sweepai-0.1.2/PKG-INFO` & `sweepai-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweepai
-Version: 0.1.2
+Version: 0.1.5
 Summary: Sweep software chores
 Author: Kevin Lu
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: GitPython (>=3.1.31,<4.0.0)
 Requires-Dist: PyGithub (==1.58.2)
 Requires-Dist: PyJWT (>=2.6.0,<3.0.0)
```

