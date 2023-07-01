# Comparing `tmp/tui_rsync-0.8.15.tar.gz` & `tmp/tui_rsync-0.8.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tui_rsync-0.8.15.tar", max compression
+gzip compressed data, was "tui_rsync-0.8.16.tar", max compression
```

## Comparing `tui_rsync-0.8.15.tar` & `tui_rsync-0.8.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      389 2023-06-26 15:12:16.917128 tui_rsync-0.8.15/README.rst
--rw-r--r--   0        0        0      725 2023-06-26 15:12:16.917128 tui_rsync-0.8.15/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-26 15:12:16.917128 tui_rsync-0.8.15/tui_rsync/__init__.py
--rw-r--r--   0        0        0      163 2023-06-26 15:12:16.917128 tui_rsync-0.8.15/tui_rsync/cli/__init__.py
--rw-r--r--   0        0        0     1889 2023-06-26 15:12:16.917128 tui_rsync-0.8.15/tui_rsync/cli/cli.py
--rw-r--r--   0        0        0       47 2023-06-26 15:12:16.917128 tui_rsync-0.8.15/tui_rsync/cli/groups/__init__.py
--rw-r--r--   0        0        0     1814 2023-06-26 15:12:16.917128 tui_rsync-0.8.15/tui_rsync/cli/groups/group_prompt.py
--rw-r--r--   0        0        0     2432 2023-06-26 15:12:16.917128 tui_rsync-0.8.15/tui_rsync/cli/groups/group_remove.py
--rw-r--r--   0        0        0     2374 2023-06-26 15:12:16.917128 tui_rsync-0.8.15/tui_rsync/cli/groups/group_show.py
--rw-r--r--   0        0        0     3600 2023-06-26 15:12:16.917128 tui_rsync-0.8.15/tui_rsync/cli/groups/group_update.py
--rw-r--r--   0        0        0     2761 2023-06-26 15:12:16.917128 tui_rsync-0.8.15/tui_rsync/cli/groups/groups.py
--rw-r--r--   0        0        0     3018 2023-06-26 15:12:16.917128 tui_rsync-0.8.15/tui_rsync/cli/label_prompt.py
--rw-r--r--   0        0        0     2110 2023-06-26 15:12:16.917128 tui_rsync-0.8.15/tui_rsync/cli/path_prompt.py
--rw-r--r--   0        0        0     2000 2023-06-26 15:12:16.917128 tui_rsync-0.8.15/tui_rsync/cli/rsync.py
--rw-r--r--   0        0        0       47 2023-06-26 15:12:16.917128 tui_rsync-0.8.15/tui_rsync/cli/source/__init__.py
--rw-r--r--   0        0        0     3349 2023-06-26 15:12:16.917128 tui_rsync-0.8.15/tui_rsync/cli/source/source.py
--rw-r--r--   0        0        0     2414 2023-06-26 15:12:16.917128 tui_rsync-0.8.15/tui_rsync/cli/source/source_remove.py
--rw-r--r--   0        0        0     2644 2023-06-26 15:12:16.917128 tui_rsync-0.8.15/tui_rsync/cli/source/source_show.py
--rw-r--r--   0        0        0     4146 2023-06-26 15:12:16.917128 tui_rsync-0.8.15/tui_rsync/cli/source/source_update.py
--rw-r--r--   0        0        0     4311 2023-06-26 15:12:16.917128 tui_rsync-0.8.15/tui_rsync/cli/sync.py
--rw-r--r--   0        0        0       38 2023-06-26 15:12:16.917128 tui_rsync-0.8.15/tui_rsync/config/__init__.py
--rw-r--r--   0        0        0     2211 2023-06-26 15:12:16.917128 tui_rsync-0.8.15/tui_rsync/config/app.py
--rw-r--r--   0        0        0      156 2023-06-26 15:12:16.917128 tui_rsync-0.8.15/tui_rsync/main.py
--rw-r--r--   0        0        0      230 2023-06-26 15:12:16.917128 tui_rsync-0.8.15/tui_rsync/models/__init__.py
--rw-r--r--   0        0        0     7537 2023-06-26 15:12:16.921129 tui_rsync-0.8.15/tui_rsync/models/models.py
--rw-r--r--   0        0        0     1422 1970-01-01 00:00:00.000000 tui_rsync-0.8.15/setup.py
--rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 tui_rsync-0.8.15/PKG-INFO
+-rw-r--r--   0        0        0      389 2023-07-01 08:36:04.475264 tui_rsync-0.8.16/README.rst
+-rw-r--r--   0        0        0      725 2023-07-01 08:36:04.475264 tui_rsync-0.8.16/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-01 08:36:04.475264 tui_rsync-0.8.16/tui_rsync/__init__.py
+-rw-r--r--   0        0        0      163 2023-07-01 08:36:04.475264 tui_rsync-0.8.16/tui_rsync/cli/__init__.py
+-rw-r--r--   0        0        0     1889 2023-07-01 08:36:04.475264 tui_rsync-0.8.16/tui_rsync/cli/cli.py
+-rw-r--r--   0        0        0       47 2023-07-01 08:36:04.475264 tui_rsync-0.8.16/tui_rsync/cli/groups/__init__.py
+-rw-r--r--   0        0        0     1814 2023-07-01 08:36:04.475264 tui_rsync-0.8.16/tui_rsync/cli/groups/group_prompt.py
+-rw-r--r--   0        0        0     2432 2023-07-01 08:36:04.475264 tui_rsync-0.8.16/tui_rsync/cli/groups/group_remove.py
+-rw-r--r--   0        0        0     2666 2023-07-01 08:36:04.475264 tui_rsync-0.8.16/tui_rsync/cli/groups/group_show.py
+-rw-r--r--   0        0        0     3600 2023-07-01 08:36:04.475264 tui_rsync-0.8.16/tui_rsync/cli/groups/group_update.py
+-rw-r--r--   0        0        0     2761 2023-07-01 08:36:04.475264 tui_rsync-0.8.16/tui_rsync/cli/groups/groups.py
+-rw-r--r--   0        0        0     3018 2023-07-01 08:36:04.475264 tui_rsync-0.8.16/tui_rsync/cli/label_prompt.py
+-rw-r--r--   0        0        0     2110 2023-07-01 08:36:04.475264 tui_rsync-0.8.16/tui_rsync/cli/path_prompt.py
+-rw-r--r--   0        0        0     2000 2023-07-01 08:36:04.475264 tui_rsync-0.8.16/tui_rsync/cli/rsync.py
+-rw-r--r--   0        0        0       47 2023-07-01 08:36:04.475264 tui_rsync-0.8.16/tui_rsync/cli/source/__init__.py
+-rw-r--r--   0        0        0     3349 2023-07-01 08:36:04.475264 tui_rsync-0.8.16/tui_rsync/cli/source/source.py
+-rw-r--r--   0        0        0     2414 2023-07-01 08:36:04.475264 tui_rsync-0.8.16/tui_rsync/cli/source/source_remove.py
+-rw-r--r--   0        0        0     2644 2023-07-01 08:36:04.475264 tui_rsync-0.8.16/tui_rsync/cli/source/source_show.py
+-rw-r--r--   0        0        0     4146 2023-07-01 08:36:04.475264 tui_rsync-0.8.16/tui_rsync/cli/source/source_update.py
+-rw-r--r--   0        0        0     4311 2023-07-01 08:36:04.475264 tui_rsync-0.8.16/tui_rsync/cli/sync.py
+-rw-r--r--   0        0        0       38 2023-07-01 08:36:04.479264 tui_rsync-0.8.16/tui_rsync/config/__init__.py
+-rw-r--r--   0        0        0     2211 2023-07-01 08:36:04.479264 tui_rsync-0.8.16/tui_rsync/config/app.py
+-rw-r--r--   0        0        0      156 2023-07-01 08:36:04.479264 tui_rsync-0.8.16/tui_rsync/main.py
+-rw-r--r--   0        0        0      230 2023-07-01 08:36:04.479264 tui_rsync-0.8.16/tui_rsync/models/__init__.py
+-rw-r--r--   0        0        0     7537 2023-07-01 08:36:04.479264 tui_rsync-0.8.16/tui_rsync/models/models.py
+-rw-r--r--   0        0        0     1422 1970-01-01 00:00:00.000000 tui_rsync-0.8.16/setup.py
+-rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 tui_rsync-0.8.16/PKG-INFO
```

### Comparing `tui_rsync-0.8.15/pyproject.toml` & `tui_rsync-0.8.16/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tui-rsync"
-version = "0.8.15"
+version = "0.8.16"
 description = "tui-rsync will help you to manage yours backups."
 authors = ["Kostiantyn Klochko <kostya_klochko@ukr.net>"]
 readme = "README.rst"
 license = "GPL-3.0-or-later"
 packages = [{include = "tui_rsync"}]
 repository = "https://gitlab.com/KKlochko/tui-rsync"
 keywords = ["tui", "cli", "rsync", "backup"]
```

### Comparing `tui_rsync-0.8.15/tui_rsync/cli/cli.py` & `tui_rsync-0.8.16/tui_rsync/cli/cli.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.15/tui_rsync/cli/groups/group_prompt.py` & `tui_rsync-0.8.16/tui_rsync/cli/groups/group_prompt.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.15/tui_rsync/cli/groups/group_remove.py` & `tui_rsync-0.8.16/tui_rsync/cli/groups/group_remove.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.15/tui_rsync/cli/groups/group_show.py` & `tui_rsync-0.8.16/tui_rsync/cli/source/source_show.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,36 +18,47 @@
 ################################################################################
 
 from rich.console import Console
 from rich.prompt import Prompt
 from typing import List, Optional
 import typer
 
-from tui_rsync.models.models import Group, GroupSource
-from tui_rsync.cli.groups.group_prompt import GroupPrompt
+from tui_rsync.models.models import Source, Destination, SyncCommand, Path
+from tui_rsync.cli.label_prompt import LabelPrompt
+from tui_rsync.models.models import all_labels
 
 console = Console()
-group_show = typer.Typer()
+source_show = typer.Typer()
 
-@group_show.command()
+@source_show.command()
 def one(
-    group_label: str = typer.Option(
-        None, "--group-label", "-l",
-        help="[b]The label[/] is a uniq identification of a [b]group[/].",
+    label: str = typer.Option(
+        None, "--label", "-l",
+        help="[b]The label[/] is a uniq identification of a [b]source[/].",
         show_default=False
     ),
 ):
     """
-    [green b]Show[/] an [yellow]existing group[/].
+    [green b]Show[/] an [yellow]existing source[/].
     """
-    if group_label is None:
-        console.print("What is the [yellow b]label of the group[/]? ")
-        group_label = GroupPrompt.get_label_fzf()
+    if label is None:
+        console.print("What is the [yellow b]label of source[/]? ")
+        label = LabelPrompt.get_label_fzf()
 
-    if not Group.is_exist(group_label):
+    if not Source.is_exist(label):
         console.print("[red b][ERROR][/] Source does not exists!!!")
         return
 
-    group = Group.get_group(group_label)
+    source = Source.get_source(label)
 
-    console.print(group.show_format())
+    console.print(source.show_format())
+
+@source_show.command()
+def all():
+    """
+    [green b]Show[/] [yellow]all existing sources[/].
+    """
+
+    for label in all_labels().iterator():
+        source = Source.get_source(label.label)
+        console.print(source.show_format())
```

### Comparing `tui_rsync-0.8.15/tui_rsync/cli/groups/group_update.py` & `tui_rsync-0.8.16/tui_rsync/cli/groups/group_update.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.15/tui_rsync/cli/groups/groups.py` & `tui_rsync-0.8.16/tui_rsync/cli/groups/groups.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.15/tui_rsync/cli/label_prompt.py` & `tui_rsync-0.8.16/tui_rsync/cli/label_prompt.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.15/tui_rsync/cli/path_prompt.py` & `tui_rsync-0.8.16/tui_rsync/cli/path_prompt.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.15/tui_rsync/cli/rsync.py` & `tui_rsync-0.8.16/tui_rsync/cli/rsync.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.15/tui_rsync/cli/source/source.py` & `tui_rsync-0.8.16/tui_rsync/cli/source/source.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.15/tui_rsync/cli/source/source_remove.py` & `tui_rsync-0.8.16/tui_rsync/cli/source/source_remove.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.15/tui_rsync/cli/source/source_show.py` & `tui_rsync-0.8.16/tui_rsync/cli/groups/group_show.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,47 +18,46 @@
 ################################################################################
 
 from rich.console import Console
 from rich.prompt import Prompt
 from typing import List, Optional
 import typer
 
-from tui_rsync.models.models import Source, Destination, SyncCommand, Path
-from tui_rsync.cli.label_prompt import LabelPrompt
-from tui_rsync.models.models import all_labels
+from tui_rsync.models.models import Group, GroupSource
+from tui_rsync.cli.groups.group_prompt import GroupPrompt
+from tui_rsync.models.models import all_group_labels
 
 console = Console()
-source_show = typer.Typer()
+group_show = typer.Typer()
 
-@source_show.command()
+@group_show.command()
 def one(
-    label: str = typer.Option(
-        None, "--label", "-l",
-        help="[b]The label[/] is a uniq identification of a [b]source[/].",
+    group_label: str = typer.Option(
+        None, "--group-label", "-l",
+        help="[b]The label[/] is a uniq identification of a [b]group[/].",
         show_default=False
     ),
 ):
     """
-    [green b]Show[/] an [yellow]existing source[/].
+    [green b]Show[/] an [yellow]existing group[/].
     """
-    if label is None:
-        console.print("What is the [yellow b]label of source[/]? ")
-        label = LabelPrompt.get_label_fzf()
+    if group_label is None:
+        console.print("What is the [yellow b]label of the group[/]? ")
+        group_label = GroupPrompt.get_label_fzf()
 
-    if not Source.is_exist(label):
+    if not Group.is_exist(group_label):
         console.print("[red b][ERROR][/] Source does not exists!!!")
         return
 
-    source = Source.get_source(label)
+    group = Group.get_group(group_label)
 
-    console.print(source.show_format())
+    console.print(group.show_format())
 
-@source_show.command()
+@group_show.command()
 def all():
     """
-    [green b]Show[/] [yellow]all existing sources[/].
+    [green b]Show[/] [yellow]all existing groups[/].
     """
-
-    for label in all_labels().iterator():
-        source = Source.get_source(label.label)
-        console.print(source.show_format())
+    for label in all_group_labels().iterator():
+        group = Group.get_group(label.label)
+        console.print(group.show_format())
```

### Comparing `tui_rsync-0.8.15/tui_rsync/cli/source/source_update.py` & `tui_rsync-0.8.16/tui_rsync/cli/source/source_update.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.15/tui_rsync/cli/sync.py` & `tui_rsync-0.8.16/tui_rsync/cli/sync.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.15/tui_rsync/config/app.py` & `tui_rsync-0.8.16/tui_rsync/config/app.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.15/tui_rsync/models/models.py` & `tui_rsync-0.8.16/tui_rsync/models/models.py`

 * *Files identical despite different names*

### Comparing `tui_rsync-0.8.15/setup.py` & `tui_rsync-0.8.16/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'typer>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['tui-rsync = tui_rsync.main:main']}
 
 setup_kwargs = {
     'name': 'tui-rsync',
-    'version': '0.8.15',
+    'version': '0.8.16',
     'description': 'tui-rsync will help you to manage yours backups.',
     'long_description': 'tui-rsync\n=========\n\n|PyPI version|\n\ntui-rsync is the application that will help you to manage yours backups.\nIt uses rsync for syncing backups.\n\nDependencies\n============\n\n-  rsync\n-  fzf\n\nAuthor\n======\n\nKostiantyn Klochko (c) 2023\n\nLicense\n=======\n\nUnder GNU GPL v3 license\n\n.. |PyPI version| image:: https://badge.fury.io/py/tui-rsync.svg\n   :target: https://badge.fury.io/py/tui-rsync\n',
     'author': 'Kostiantyn Klochko',
     'author_email': 'kostya_klochko@ukr.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/KKlochko/tui-rsync',
```

### Comparing `tui_rsync-0.8.15/PKG-INFO` & `tui_rsync-0.8.16/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui-rsync
-Version: 0.8.15
+Version: 0.8.16
 Summary: tui-rsync will help you to manage yours backups.
 Home-page: https://gitlab.com/KKlochko/tui-rsync
 License: GPL-3.0-or-later
 Keywords: tui,cli,rsync,backup
 Author: Kostiantyn Klochko
 Author-email: kostya_klochko@ukr.net
 Requires-Python: >=3.10,<4.0
```

