# Comparing `tmp/gitmopy-0.3.5.2.tar.gz` & `tmp/gitmopy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitmopy-0.3.5.2.tar", max compression
+gzip compressed data, was "gitmopy-0.4.0.tar", max compression
```

## Comparing `gitmopy-0.3.5.2.tar` & `gitmopy-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1070 2023-06-16 22:59:50.534602 gitmopy-0.3.5.2/LICENSE
--rw-r--r--   0        0        0     7758 2023-06-27 19:13:53.503733 gitmopy-0.3.5.2/README.md
--rw-r--r--   0        0        0      112 2023-06-16 19:39:04.304895 gitmopy-0.3.5.2/gitmopy/__init__.py
--rw-r--r--   0        0        0    15076 2023-06-27 19:13:12.371022 gitmopy-0.3.5.2/gitmopy/cli.py
--rw-r--r--   0        0        0     6871 2023-06-27 14:20:26.669816 gitmopy-0.3.5.2/gitmopy/git.py
--rw-r--r--   0        0        0     2972 2023-06-27 13:10:13.038440 gitmopy-0.3.5.2/gitmopy/history.py
--rw-r--r--   0        0        0     8761 2023-06-27 14:20:26.670390 gitmopy-0.3.5.2/gitmopy/prompt.py
--rw-r--r--   0        0        0    21278 2023-06-27 13:10:13.040862 gitmopy-0.3.5.2/gitmopy/utils.py
--rw-r--r--   0        0        0      580 2023-06-27 19:13:44.007974 gitmopy-0.3.5.2/pyproject.toml
--rw-r--r--   0        0        0     8743 1970-01-01 00:00:00.000000 gitmopy-0.3.5.2/setup.py
--rw-r--r--   0        0        0     8388 1970-01-01 00:00:00.000000 gitmopy-0.3.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-16 22:59:50.534602 gitmopy-0.4.0/LICENSE
+-rw-r--r--   0        0        0     7978 2023-06-30 23:12:55.485417 gitmopy-0.4.0/README.md
+-rw-r--r--   0        0        0      112 2023-06-16 19:39:04.304895 gitmopy-0.4.0/gitmopy/__init__.py
+-rw-r--r--   0        0        0    15715 2023-06-30 23:12:55.486562 gitmopy-0.4.0/gitmopy/cli.py
+-rw-r--r--   0        0        0     8580 2023-06-30 23:12:55.487270 gitmopy-0.4.0/gitmopy/constants.py
+-rw-r--r--   0        0        0     6899 2023-06-30 23:12:55.488544 gitmopy-0.4.0/gitmopy/git.py
+-rw-r--r--   0        0        0     3218 2023-06-30 23:12:55.489041 gitmopy-0.4.0/gitmopy/history.py
+-rw-r--r--   0        0        0     8690 2023-06-30 23:12:55.489763 gitmopy-0.4.0/gitmopy/prompt.py
+-rw-r--r--   0        0        0     7413 2023-06-30 23:12:55.490210 gitmopy-0.4.0/gitmopy/utils.py
+-rw-r--r--   0        0        0      578 2023-06-30 23:12:55.490739 gitmopy-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     8964 1970-01-01 00:00:00.000000 gitmopy-0.4.0/setup.py
+-rw-r--r--   0        0        0     8606 1970-01-01 00:00:00.000000 gitmopy-0.4.0/PKG-INFO
```

### Comparing `gitmopy-0.3.5.2/LICENSE` & `gitmopy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gitmopy-0.3.5.2/README.md` & `gitmopy-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # `gitmopy`
 
-An interactive Python implementation of the Gitmoji standard: https://gitmoji.dev/
+An interactive Python implementation of the Gitmoji convention: [gitmoji.dev/](https://gitmoji.dev/)
 
 ```text
 pip install gitmopy
 ```
 
 ![demo-gitmopy](./assets/demo-gitmopy.gif)
 
@@ -17,14 +17,16 @@
 * Press **`tab`** to **auto-complete**
   * Press `tab` on an empty line to see history
 * **Restart commit** with **`crtl+c`**
   * The keyboard interruption will be caught once, then press `enter` to restart
 * Push (and set upstream if need be)
 * Commit again 🔄
 
+Use your own emojis by editing the "custom emojis" file listed by `gitmopy info`!
+
 ## Suggested shortcuts
 
 ```bash
 alias gpy="gitmopy"
 alias gpyc="gitmopy commit"
 alias gpya="gitmopy commit --add"
 alias gpyk="gitmopy commit --add --keep-alive"
@@ -84,18 +86,19 @@
 
 ## User guide
 
 ```text
 $ gitmopy info
 
 gitmopy info:
-  version : 0.3.5.2
-  app path: /Users/victor/.gitmopy
-  history : /Users/victor/.gitmopy/history.json
-  config  : /Users/victor/.gitmopy/config.yaml
+  version      : 0.4.0
+  app path     : /Users/victor/.gitmopy
+  history      : /Users/victor/.gitmopy/history.json
+  config       : /Users/victor/.gitmopy/config.yaml
+  custom emojis: /Users/victor/.gitmopy/custom_gitmojis.yaml
 
 Current configuration:
   skip_scope      : False
   skip_message    : False
   capitalize_title: True
   enable_history  : True
 ```
@@ -169,15 +172,15 @@
 
 * Features
   * *If requested:*
     * Install hook
     * `git commit` flags (like `-S`)
     * max history length (if loading the json becomes slow)
 * Tests
-  * https://typer.tiangolo.com/tutorial/testing/
+  * [typer.tiangolo.com/tutorial/testing/](https://typer.tiangolo.com/tutorial/testing/)
   * 👋 **Help wanted**
 * Docs
   * Not critical
 
 ## Resources
 
 `gitmopy` is inspired by [`gitmoji-cli`](https://github.com/carloscuesta/gitmoji-cli).
```

### Comparing `gitmopy-0.3.5.2/gitmopy/cli.py` & `gitmopy-0.4.0/gitmopy/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,22 @@
 from typing import List, Optional
 
 import git
 import typer
 from git import Repo
 from typing_extensions import Annotated
 
+from gitmopy.constants import (
+    APP_PATH,
+    COLORS,
+    CONFIG_PATH,
+    HISTORY_PATH,
+    USER_EMOJIS_PATH,
+    _sentinels,
+)
 from gitmopy.git import (
     CatchRemoteException,
     format_remotes_diff,
     get_files_status,
     has_upstreams,
 )
 from gitmopy.history import gitmojis_setup, save_to_history
@@ -20,19 +28,14 @@
     commit_prompt,
     config_prompt,
     git_add_prompt,
     set_upstream_prompt,
     what_now_prompt,
 )
 from gitmopy.utils import (
-    APP_PATH,
-    CONFIG_PATH,
-    HISTORY_PATH,
-    COLORS,
-    _sentinels,
     col,
     console,
     load_config,
     message_from_commit_dict,
     print,
     print_staged_files,
     resolve_path,
@@ -67,14 +70,17 @@
         Returns:
             Any: The wrapped function's return value or the ``_sentinels["cancelled"]``
                 sentinel if the function was aborted.
         """
         return_value = _sentinels["cancelled"]
         try:
             return_value = func(*_args, **_kwargs)
+        except Exception as e:
+            if not isinstance(e, KeyboardInterrupt):
+                print(e)
         finally:
             return return_value
 
     return_value = _func(*args, **kwargs)
     if return_value is not _sentinels["cancelled"]:
         # function was not aborted
         return return_value
@@ -138,27 +144,37 @@
 
     if commit_again:
         print()
 
     return commit_again
 
 
-def push_cli(repo, remote):
-    # push to remotes. If several remotes, use either the values from --remote
-    # or prompt the user to choose them.
-    # If no remote, ignore push.
+def push_cli(repo, remote_cli_args):
+    """
+    Push to user remotes.
+
+    If several remotes, use either the values from --remote or prompt the user to
+    select them.
+
+    Args:
+        repo (Repo): The git repository.
+        remote_cli_args (List[str]): The remotes passed as CLI arguments.
+
+    Raises:
+        typer.Abort: If no remote is selected.
+    """
     if len(repo.remotes) == 0:
         print(col("No remote found. Ignoring push.", "y"))
     else:
         # default: contain "origin"
         selected_remotes = set([repo.remotes[0].name])
         if len(repo.remotes) > 1:
-            if remote:
+            if remote_cli_args:
                 # use --remote values
-                selected_remotes = set(remote)
+                selected_remotes = set(remote_cli_args)
             else:
                 # PROMPT: choose remote
                 selected_remotes = choose_remote_prompt(repo.remotes)
             if not selected_remotes:
                 # stop if no remote selected
                 print(col("No remote selected. Aborting.", "y"))
                 raise typer.Abort()
@@ -199,33 +215,43 @@
                     else:
                         with CatchRemoteException(remote.name) as cre:
                             repo.git.push(remote.name, repo.active_branch.name)
                     if cre and not cre.error:
                         print(done)
 
 
-def pull_cli(repo, remote_cli_args):
-    # pull from remotes. If several remotes, use either the values from --remote
-    # or prompt the user to choose them.
-    # If no remote, ignore push.
+def pull_cli(repo: Repo, remote_cli_args: List[str]):
+    """
+    Pull from remotes.
+
+    If several remotes, use either the values from --remote, or prompt the user
+    to choose them.
+
+    Args:
+        repo (git.Repo): The git repository.
+        remote_cli_args (List[str]): The remotes passed as CLI arguments.
+
+    Raises:
+        typer.Abort: Stops the process if the users does not choose a remote.
+    """
     if len(repo.remotes) == 0:
         print(col("No remote found. Ignoring pull.", "y"))
     else:
         selected_remotes = set([repo.remotes[0].name])
         if len(repo.remotes) > 1:
             if remote_cli_args:
                 # use --remote values
                 selected_remotes = set(remote_cli_args)
             else:
                 # PROMPT: choose remote
                 selected_remotes = choose_remote_prompt(repo.remotes)
             if not selected_remotes:
                 # stop if no remote selected
                 print(col("No remote selected. Aborting.", "y"))
-                raise typer.Exit(1)
+                raise typer.Abort()
             selected_remotes = set(selected_remotes)
         print()
 
         # there is at least one remote to push to at this point
         for remote in repo.remotes:
             if remote.name in selected_remotes:
                 wait = col(f"Pulling from remote {remote.name}...", "o")
@@ -429,20 +455,20 @@
 def info():
     """
     Command to print gitmopy's info.
     """
     import gitmopy
 
     print("\n[b u green3]gitmopy info:[/b u green3]")
-    print("  version :", gitmopy.__version__)
-    print("  app path:", str(APP_PATH))
+    print("  version      :", gitmopy.__version__)
+    print("  app path     :", str(APP_PATH))
     if HISTORY_PATH.exists():
-        print("  history :", str(HISTORY_PATH))
-    if CONFIG_PATH:
-        print("  config  :", str(CONFIG_PATH))
+        print("  history      :", str(HISTORY_PATH))
+    print("  config       :", str(CONFIG_PATH))
+    print("  custom emojis:", str(USER_EMOJIS_PATH))
     config = load_config()
     print(f"\n[u]{col('Current configuration:', 'b', True)}[/u]")
     max_l = max([len(k) for k in config.keys()])
     for k, v in config.items():
         print(f"  {k:{max_l}}: {v}")
     print()
```

### Comparing `gitmopy-0.3.5.2/gitmopy/git.py` & `gitmopy-0.4.0/gitmopy/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 `gitmopy`'s Git-related utility functions.
 """
 from typing import Dict, List, Union
 
-from git import Repo, Remote
+from git import Remote, Repo
 from git.exc import GitCommandError
 
-from gitmopy.utils import _sentinels, print, col
+from gitmopy.constants import _sentinels
+from gitmopy.utils import col, print
 
 
 class CatchRemoteException:
     def __init__(self, remote: str):
         """
         Context manager to catch GitCommandError when pushing to a remote.
 
@@ -80,15 +81,14 @@
         remotes (List[Union[str, Remote]]): List of remotes to check.
         branch_name (str): Name of the branch to check.
 
     Returns:
         Dict[str, bool]: Dictionnary of booleans indicating if each remote has the
             branch.
     """
-
     fetch_all(repo)
     remote_has_upstream = {
         r.name if isinstance(r, Remote) else r: False for r in remotes
     }
     remote_refs = {
         ref.remote_name: True
         for ref in repo.refs
```

### Comparing `gitmopy-0.3.5.2/gitmopy/history.py` & `gitmopy-0.4.0/gitmopy/history.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,111 +3,113 @@
 
 In particular:
 * sort emojis by timestamp
 * prepare history for prompt completion (title, scope, message)
 """
 import json
 from datetime import datetime
-from typing import Dict, List, Optional
+from typing import Dict, List
 
-from gitmopy.utils import GITMOJIS, HISTORY_PATH, load_config, print
-
-HISTORY = []
+import gitmopy.constants as gpyc
+from gitmopy.utils import col, load_config, load_user_gitmojis, print
 
 
 def load_history() -> List[Dict[str, str]]:
     """
     Load history from ``${HISTORY_PATH}`` file.
 
     Returns an empty list if the file does not exist.
     """
-    global HISTORY
     history = []
 
-    if HISTORY_PATH.exists():
-        history = json.loads(HISTORY_PATH.read_text())
+    if gpyc.HISTORY_PATH.exists():
+        try:
+            history = json.loads(gpyc.HISTORY_PATH.read_text())
+        except Exception as e:
+            print(
+                col(f"Error loading history from {str(gpyc.HISTORY_PATH)}", "red", True)
+            )
+            print(e)
+            history = []
 
-    HISTORY = history
+    gpyc.HISTORY = history
 
 
 def timestamp() -> int:
     """
     Get the current local timestamp as an int.
 
     Returns:
         int: Current timestamp.
     """
     return int(datetime.now().timestamp())
 
 
-def save_to_history(
-    commit_dict: Dict[str, str], history: Optional[List[Dict[str, str]]] = None
-) -> None:
+def save_to_history(commit_dict: Dict[str, str]) -> None:
     """
     Writes a commit dictionnary to the history file in ``${HISTORY_PATH}``.
 
     Args:
         commit_dict (dict): The commit details to write to the history file.
             Keys must be "emoji", "scope", "title" and "message". A "timestamp"
             key will be added automatically.
         history (list, optional): History to append to. Will use the global one if
             ``None``. Defaults to ``None``.
     """
-    if history is None:
-        history = HISTORY
-    history.append(
+    gpyc.HISTORY.append(
         {
             **commit_dict,
             "timestamp": timestamp(),
         }
     )
-    if not HISTORY_PATH.parent.exists():
-        HISTORY_PATH.parent.mkdir(parents=True)
-        print("[bold green]Created history file in", str(HISTORY_PATH), end="\n\n")
+    if not gpyc.HISTORY_PATH.parent.exists():
+        gpyc.HISTORY_PATH.parent.mkdir(parents=True)
+    if not gpyc.HISTORY_PATH.exists():
+        print("[bold green]Created history file in", str(gpyc.HISTORY_PATH), end="\n\n")
 
-    HISTORY_PATH.write_text(json.dumps(history))
+    gpyc.HISTORY_PATH.write_text(json.dumps(gpyc.HISTORY))
 
 
-def sort_emojis(
-    gitmojis: List[Dict[str, str]], history: Optional[List[Dict[str, str]]] = None
-) -> List[Dict[str, str]]:
+def sort_emojis() -> List[Dict[str, str]]:
     """
     Sort emojis by most recent usage in history.
 
     Args:
         gitmojis (list): All gitmojis available as a list of dicts.
         history (list, optional): History to sort from. Will use the global one if
             ``None``. Defaults to ``None``.
 
     Returns:
         List[Dict[str, str]]: Sorted gitmojis.
     """
-    if history is None:
-        history = HISTORY
     dater = {}
-    for commit in history:
+    for commit in gpyc.HISTORY:
         dater[commit["emoji"]] = commit["timestamp"]
-    gitmojis.sort(key=lambda x: dater.get(x["emoji"], 0), reverse=True)
+    gpyc.GITMOJIS.sort(key=lambda x: dater.get(x["emoji"], 0), reverse=True)
 
 
 def gitmojis_setup() -> None:
     """
     Setup the emoji list.
 
     * loads the config
     * adds ``name`` and ``value`` keys to each emoji (for prompt Choices)
     * loads the history (if enabled)
     * sorts the emojis by most recent usage in history (if enabled)
     """
-    global GITMOJIS
-
     config = load_config()
-
-    for k, e in enumerate(GITMOJIS):
-        GITMOJIS[k]["name"] = e["emoji"] + " " + e["description"]
-        GITMOJIS[k]["value"] = e["emoji"]
+    emo_dict = {e["emoji"]: e for e in gpyc.GITMOJIS}
+    user_emojis = load_user_gitmojis()
+    for u in user_emojis:
+        emo_dict[u["emoji"]] = u
+
+    gpyc.GITMOJIS = list(emo_dict.values())
+
+    for k, e in enumerate(gpyc.GITMOJIS):
+        gpyc.GITMOJIS[k]["name"] = e["emoji"] + " " + e["description"]
+        gpyc.GITMOJIS[k]["value"] = e["emoji"]
 
     if not config["enable_history"]:
         return
 
     load_history()
-    sort_emojis(GITMOJIS)
+    sort_emojis()
```

### Comparing `gitmopy-0.3.5.2/gitmopy/prompt.py` & `gitmopy-0.4.0/gitmopy/prompt.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,24 +7,16 @@
 from typing import Any, Dict, List, Optional
 
 from InquirerPy import inquirer
 from InquirerPy.base.control import Choice
 from prompt_toolkit.completion import Completer, Completion
 from prompt_toolkit.document import Document
 
-from gitmopy import history as gmp_history
-from gitmopy.utils import (
-    APP_PATH,
-    DEFAULT_CHOICES,
-    GITMOJIS,
-    load_config,
-    safe_capitalize,
-    save_config,
-    choice_separator,
-)
+import gitmopy.constants as gpyc
+from gitmopy.utils import choice_separator, load_config, safe_capitalize, save_config
 
 
 class GMPCompleter(Completer):
     def __init__(self, key: str, max_results: Optional[int] = 10):
         """
         A completer that completes a text prompt from the user's history.
 
@@ -34,15 +26,15 @@
         Args:
             key (str): Key to complete from. Must be one of "scope", "title", "message".
             max_results (int): Maximum number of results to return. Defaults to 10.
         """
         self.key = key
         self.max_results = max_results
         self.candidates = {}
-        for c in gmp_history.HISTORY:
+        for c in gpyc.HISTORY:
             if c[key] not in self.candidates:
                 self.candidates[c[key]] = c["timestamp"]
             else:
                 self.candidates[c[key]] = max(self.candidates[c[key]], c["timestamp"])
         super().__init__()
 
     def get_completions(self, document: Document, complete_event: Any) -> Completion:
@@ -91,15 +83,15 @@
         dict: User-specified commit as a dict with keys
             ``"emoji"``, ``"scope"``, ``"title"``, ``"message"``.
     """
     # get the commit's gitmoji
     emoji = (
         inquirer.fuzzy(
             message="Select gitmoji:",
-            choices=GITMOJIS,
+            choices=gpyc.GITMOJIS,
             multiselect=False,
             max_height="70%",
             mandatory=True,
             qmark="❓",
             amark="✓",
         )
         .execute()
@@ -180,21 +172,21 @@
 
     Will save the configuration in ``${APP_PATH}/config.yaml``.
     """
     config = load_config()
 
     choices = [
         Choice(c["value"], c["name"], config.get(c["value"], c["default"]))
-        for c in DEFAULT_CHOICES
+        for c in gpyc.DEFAULT_CHOICES
     ]
 
     selected = inquirer.checkbox(
         message="Configure gitmopy locally.",
         instruction="Use 'space' to (de-)select, 'enter' to validate.",
-        long_instruction=f"Config will be saved in {str(APP_PATH)}/config.yaml.",
+        long_instruction=f"Config will be saved in {str(gpyc.APP_PATH)}/config.yaml.",
         choices=choices,
         cycle=True,
         transformer=lambda result: "",
         qmark="❓",
         amark="✓",
     ).execute()
 
@@ -286,16 +278,17 @@
         amark="✓",
         default=True,
     ).execute()
 
 
 def what_now_prompt(choices: Dict[str, str]) -> str:
     """
-    Prompt the user to select what to do next. Choices must be a
-    dict like `{value: name}`
+    Prompt the user to select what to do next.
+
+    Choices must be a dictlike `{value: name}`.
 
     Args:
         choices (Dict[str, str]): Available choices.
 
     Returns:
         str: User's choice.
     """
```

### Comparing `gitmopy-0.3.5.2/pyproject.toml` & `gitmopy-0.4.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gitmopy"
-version = "0.3.5.2"
+version = "0.4.0"
 description = "A python command-line for gitmoji"
 authors = ["vict0rsch <vsch@pm.me>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gitmopy-0.3.5.2/setup.py` & `gitmopy-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
  'typer[all]>=0.8.0']
 
 entry_points = \
 {'console_scripts': ['gitmopy = gitmopy.cli:app']}
 
 setup_kwargs = {
     'name': 'gitmopy',
-    'version': '0.3.5.2',
+    'version': '0.4.0',
     'description': 'A python command-line for gitmoji',
-    'long_description': '# `gitmopy`\n\nAn interactive Python implementation of the Gitmoji standard: https://gitmoji.dev/\n\n```text\npip install gitmopy\n```\n\n![demo-gitmopy](./assets/demo-gitmopy.gif)\n\n## How to use\n\n* I typically use `$ gitmopy commit --add --keep-alive`\n* Navigate through options with ⬆️ and ⬇️\n* **Select** option with **`space`**\n* **Validate** selection with **`enter`**\n* Press **`tab`** to **auto-complete**\n  * Press `tab` on an empty line to see history\n* **Restart commit** with **`crtl+c`**\n  * The keyboard interruption will be caught once, then press `enter` to restart\n* Push (and set upstream if need be)\n* Commit again 🔄\n\n## Suggested shortcuts\n\n```bash\nalias gpy="gitmopy"\nalias gpyc="gitmopy commit"\nalias gpya="gitmopy commit --add"\nalias gpyk="gitmopy commit --add --keep-alive"\n```\n\n![gpyk depo](assets/gpyk.png)\n\n## Examples\n\n```bash\n# Typical daily use-case\n# ----------------------\n\n# continuously commit, interactively select files to stage\n$ gitmopy commit --add --keep-alive\n\n# same using an alias, + push after every commit (could be dangerous)\n$ gpyk --push\n\n\n# Specific usage\n# --------------\n\n# commit currently staged files. Will fail if no file is staged.\n$ gitmopy commit\n\n# Enable interactive file selection if no file is currently staged. Ignored if\n# there are staged files.\n$ gitmopy commit --add\n\n# Commit continuously: don\'t leave the CLI after the first commit but restart\n# the commit procedure.\n$ gitmopy commit --keep-alive\n\n# Push to remote repositories after commit.\n# Interactively select remotes to push to if there are more than 1.\n$ gitmopy commit --push\n\n# Push to specific remotes\n$ gitmopy commit --push --remote origin --remote upstream\n\n# Make and display a commit message without staging/committing/pushing\n$ gitmopy commit --dry\n\n# configure gitmopy\n$ gitmopy config\n\n# print version, data paths and current configuration\n$ gitmopy info\n\n# print helps\n$ gitmopy --help\n$ gitmopy commit --help\n```\n\n⚠️ The sync feature is still experimental. It will `pull` then `push` but in the case of several remotes and the branch not existing on one of them, I recommend you deal with it with `git` manually.\n\n## User guide\n\n```text\n$ gitmopy info\n\ngitmopy info:\n  version : 0.3.5.2\n  app path: /Users/victor/.gitmopy\n  history : /Users/victor/.gitmopy/history.json\n  config  : /Users/victor/.gitmopy/config.yaml\n\nCurrent configuration:\n  skip_scope      : False\n  skip_message    : False\n  capitalize_title: True\n  enable_history  : True\n```\n\nUpdate configuration with\n\n```text\n$ gitmopy config\n$ gitmopy config\n❓ Configure gitmopy locally. Use \'space\' to (de-)select, \'enter\' to validate.\n❯ ○ Skip commit scope\n  ○ Skip commit message\n  ◉ Capitalize commit title\n  ◉ Remember commit history for auto-complete and emoji sorting\n\nConfig will be saved in /Users/victor/.gitmopy/config.yaml.\n```\n\nGet help with\n\n```text\n$ gitmopy --help\n\n Usage: gitmopy [OPTIONS] COMMAND [ARGS]...\n\n╭─ Options ───────────────────────────────────────────────────────────────────────────╮\n│ --install-completion          Install completion for the current shell.             │\n│ --show-completion             Show completion for the current shell, to copy it or  │\n│                               customize the installation.                           │\n│ --help                        Show this message and exit.                           │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Commands ──────────────────────────────────────────────────────────────────────────╮\n│ commit  Commit staged files. Use --add to interactively select files to stage if    │\n│         none is already staged                                                      │\n│ config  Configure gitmopy                                                           │\n│ info    Print gitmopy info                                                          │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n\n$ gitmopy commit --help\n\n Usage: gitmopy commit [OPTIONS]\n\n Commit staged files. Use --add to interactively select files to stage if none is\n already staged\n\n╭─ Options ───────────────────────────────────────────────────────────────────────────╮\n│ --repo                             TEXT  Path to the git repository [default: .]    │\n│ --add           --no-add                 Whether or not to interactively select     │\n│                                          files to stage if none is already staged   │\n│                                          [default: no-add]                          │\n│ --push          --no-push                Whether to `git push` after commit. If     │\n│                                          multiple remotes exist, you will be asked  │\n│                                          to interactively choose the ones to push   │\n│                                          to. Use --remote to skip interactive       │\n│                                          selection. Disabled by default.            │\n│                                          [default: no-push]                         │\n│ --dry           --no-dry                 Whether or not to actually commit.         │\n│                                          [default: no-dry]                          │\n│ --remote                           TEXT  Remote to push to after commit. Use to     │\n│                                          skip interactive remote selection when     │\n│                                          several exist. Use several \'--remote       │\n│                                          {remote name}\' to push to multiple remotes │\n│ --keep-alive    --no-keep-alive          Whether or not to keep the app alive after │\n│                                          commit, to be ready for another one.       │\n│                                          [default: no-keep-alive]                   │\n│ --help                                   Show this message and exit.                │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n## To Do\n\n* Features\n  * *If requested:*\n    * Install hook\n    * `git commit` flags (like `-S`)\n    * max history length (if loading the json becomes slow)\n* Tests\n  * https://typer.tiangolo.com/tutorial/testing/\n  * 👋 **Help wanted**\n* Docs\n  * Not critical\n\n## Resources\n\n`gitmopy` is inspired by [`gitmoji-cli`](https://github.com/carloscuesta/gitmoji-cli).\n\nIt is built thanks to:\n\n* [`typer`](https://github.com/tiangolo/typer)\n* [`InquirePy`](https://github.com/kazhala/InquirerPy)\n* [`GitPython`](https://github.com/gitpython-developers/GitPython)\n',
+    'long_description': '# `gitmopy`\n\nAn interactive Python implementation of the Gitmoji convention: [gitmoji.dev/](https://gitmoji.dev/)\n\n```text\npip install gitmopy\n```\n\n![demo-gitmopy](./assets/demo-gitmopy.gif)\n\n## How to use\n\n* I typically use `$ gitmopy commit --add --keep-alive`\n* Navigate through options with ⬆️ and ⬇️\n* **Select** option with **`space`**\n* **Validate** selection with **`enter`**\n* Press **`tab`** to **auto-complete**\n  * Press `tab` on an empty line to see history\n* **Restart commit** with **`crtl+c`**\n  * The keyboard interruption will be caught once, then press `enter` to restart\n* Push (and set upstream if need be)\n* Commit again 🔄\n\nUse your own emojis by editing the "custom emojis" file listed by `gitmopy info`!\n\n## Suggested shortcuts\n\n```bash\nalias gpy="gitmopy"\nalias gpyc="gitmopy commit"\nalias gpya="gitmopy commit --add"\nalias gpyk="gitmopy commit --add --keep-alive"\n```\n\n![gpyk depo](assets/gpyk.png)\n\n## Examples\n\n```bash\n# Typical daily use-case\n# ----------------------\n\n# continuously commit, interactively select files to stage\n$ gitmopy commit --add --keep-alive\n\n# same using an alias, + push after every commit (could be dangerous)\n$ gpyk --push\n\n\n# Specific usage\n# --------------\n\n# commit currently staged files. Will fail if no file is staged.\n$ gitmopy commit\n\n# Enable interactive file selection if no file is currently staged. Ignored if\n# there are staged files.\n$ gitmopy commit --add\n\n# Commit continuously: don\'t leave the CLI after the first commit but restart\n# the commit procedure.\n$ gitmopy commit --keep-alive\n\n# Push to remote repositories after commit.\n# Interactively select remotes to push to if there are more than 1.\n$ gitmopy commit --push\n\n# Push to specific remotes\n$ gitmopy commit --push --remote origin --remote upstream\n\n# Make and display a commit message without staging/committing/pushing\n$ gitmopy commit --dry\n\n# configure gitmopy\n$ gitmopy config\n\n# print version, data paths and current configuration\n$ gitmopy info\n\n# print helps\n$ gitmopy --help\n$ gitmopy commit --help\n```\n\n⚠️ The sync feature is still experimental. It will `pull` then `push` but in the case of several remotes and the branch not existing on one of them, I recommend you deal with it with `git` manually.\n\n## User guide\n\n```text\n$ gitmopy info\n\ngitmopy info:\n  version      : 0.4.0\n  app path     : /Users/victor/.gitmopy\n  history      : /Users/victor/.gitmopy/history.json\n  config       : /Users/victor/.gitmopy/config.yaml\n  custom emojis: /Users/victor/.gitmopy/custom_gitmojis.yaml\n\nCurrent configuration:\n  skip_scope      : False\n  skip_message    : False\n  capitalize_title: True\n  enable_history  : True\n```\n\nUpdate configuration with\n\n```text\n$ gitmopy config\n$ gitmopy config\n❓ Configure gitmopy locally. Use \'space\' to (de-)select, \'enter\' to validate.\n❯ ○ Skip commit scope\n  ○ Skip commit message\n  ◉ Capitalize commit title\n  ◉ Remember commit history for auto-complete and emoji sorting\n\nConfig will be saved in /Users/victor/.gitmopy/config.yaml.\n```\n\nGet help with\n\n```text\n$ gitmopy --help\n\n Usage: gitmopy [OPTIONS] COMMAND [ARGS]...\n\n╭─ Options ───────────────────────────────────────────────────────────────────────────╮\n│ --install-completion          Install completion for the current shell.             │\n│ --show-completion             Show completion for the current shell, to copy it or  │\n│                               customize the installation.                           │\n│ --help                        Show this message and exit.                           │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Commands ──────────────────────────────────────────────────────────────────────────╮\n│ commit  Commit staged files. Use --add to interactively select files to stage if    │\n│         none is already staged                                                      │\n│ config  Configure gitmopy                                                           │\n│ info    Print gitmopy info                                                          │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n\n$ gitmopy commit --help\n\n Usage: gitmopy commit [OPTIONS]\n\n Commit staged files. Use --add to interactively select files to stage if none is\n already staged\n\n╭─ Options ───────────────────────────────────────────────────────────────────────────╮\n│ --repo                             TEXT  Path to the git repository [default: .]    │\n│ --add           --no-add                 Whether or not to interactively select     │\n│                                          files to stage if none is already staged   │\n│                                          [default: no-add]                          │\n│ --push          --no-push                Whether to `git push` after commit. If     │\n│                                          multiple remotes exist, you will be asked  │\n│                                          to interactively choose the ones to push   │\n│                                          to. Use --remote to skip interactive       │\n│                                          selection. Disabled by default.            │\n│                                          [default: no-push]                         │\n│ --dry           --no-dry                 Whether or not to actually commit.         │\n│                                          [default: no-dry]                          │\n│ --remote                           TEXT  Remote to push to after commit. Use to     │\n│                                          skip interactive remote selection when     │\n│                                          several exist. Use several \'--remote       │\n│                                          {remote name}\' to push to multiple remotes │\n│ --keep-alive    --no-keep-alive          Whether or not to keep the app alive after │\n│                                          commit, to be ready for another one.       │\n│                                          [default: no-keep-alive]                   │\n│ --help                                   Show this message and exit.                │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n## To Do\n\n* Features\n  * *If requested:*\n    * Install hook\n    * `git commit` flags (like `-S`)\n    * max history length (if loading the json becomes slow)\n* Tests\n  * [typer.tiangolo.com/tutorial/testing/](https://typer.tiangolo.com/tutorial/testing/)\n  * 👋 **Help wanted**\n* Docs\n  * Not critical\n\n## Resources\n\n`gitmopy` is inspired by [`gitmoji-cli`](https://github.com/carloscuesta/gitmoji-cli).\n\nIt is built thanks to:\n\n* [`typer`](https://github.com/tiangolo/typer)\n* [`InquirePy`](https://github.com/kazhala/InquirerPy)\n* [`GitPython`](https://github.com/gitpython-developers/GitPython)\n',
     'author': 'vict0rsch',
     'author_email': 'vsch@pm.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `gitmopy-0.3.5.2/PKG-INFO` & `gitmopy-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitmopy
-Version: 0.3.5.2
+Version: 0.4.0
 Summary: A python command-line for gitmoji
 License: MIT
 Author: vict0rsch
 Author-email: vsch@pm.me
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 Requires-Dist: inquirerpy (>=0.3.4,<0.4.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: typer[all] (>=0.8.0)
 Description-Content-Type: text/markdown
 
 # `gitmopy`
 
-An interactive Python implementation of the Gitmoji standard: https://gitmoji.dev/
+An interactive Python implementation of the Gitmoji convention: [gitmoji.dev/](https://gitmoji.dev/)
 
 ```text
 pip install gitmopy
 ```
 
 ![demo-gitmopy](./assets/demo-gitmopy.gif)
 
@@ -36,14 +36,16 @@
 * Press **`tab`** to **auto-complete**
   * Press `tab` on an empty line to see history
 * **Restart commit** with **`crtl+c`**
   * The keyboard interruption will be caught once, then press `enter` to restart
 * Push (and set upstream if need be)
 * Commit again 🔄
 
+Use your own emojis by editing the "custom emojis" file listed by `gitmopy info`!
+
 ## Suggested shortcuts
 
 ```bash
 alias gpy="gitmopy"
 alias gpyc="gitmopy commit"
 alias gpya="gitmopy commit --add"
 alias gpyk="gitmopy commit --add --keep-alive"
@@ -103,18 +105,19 @@
 
 ## User guide
 
 ```text
 $ gitmopy info
 
 gitmopy info:
-  version : 0.3.5.2
-  app path: /Users/victor/.gitmopy
-  history : /Users/victor/.gitmopy/history.json
-  config  : /Users/victor/.gitmopy/config.yaml
+  version      : 0.4.0
+  app path     : /Users/victor/.gitmopy
+  history      : /Users/victor/.gitmopy/history.json
+  config       : /Users/victor/.gitmopy/config.yaml
+  custom emojis: /Users/victor/.gitmopy/custom_gitmojis.yaml
 
 Current configuration:
   skip_scope      : False
   skip_message    : False
   capitalize_title: True
   enable_history  : True
 ```
@@ -188,15 +191,15 @@
 
 * Features
   * *If requested:*
     * Install hook
     * `git commit` flags (like `-S`)
     * max history length (if loading the json becomes slow)
 * Tests
-  * https://typer.tiangolo.com/tutorial/testing/
+  * [typer.tiangolo.com/tutorial/testing/](https://typer.tiangolo.com/tutorial/testing/)
   * 👋 **Help wanted**
 * Docs
   * Not critical
 
 ## Resources
 
 `gitmopy` is inspired by [`gitmoji-cli`](https://github.com/carloscuesta/gitmoji-cli).
```

