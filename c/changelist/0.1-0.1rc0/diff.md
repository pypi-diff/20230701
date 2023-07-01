# Comparing `tmp/changelist-0.1.tar.gz` & `tmp/changelist-0.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "changelist-0.1.tar", last modified: Sat Jul  1 18:52:31 2023, max compression
+gzip compressed data, was "changelist-0.1rc0.tar", last modified: Sat Jul  1 14:29:14 2023, max compression
```

## Comparing `changelist-0.1.tar` & `changelist-0.1rc0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-01 18:52:31.109760 changelist-0.1/
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1504 2023-07-01 14:23:22.000000 changelist-0.1/LICENSE.txt
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     4566 2023-07-01 18:52:31.108760 changelist-0.1/PKG-INFO
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2245 2023-07-01 18:46:12.000000 changelist-0.1/README.md
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)      961 2023-07-01 18:48:26.000000 changelist-0.1/pyproject.toml
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)       38 2023-07-01 18:52:31.109760 changelist-0.1/setup.cfg
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-01 18:52:31.105760 changelist-0.1/src/
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-01 18:52:31.107760 changelist-0.1/src/changelist/
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)        0 2023-07-01 14:23:22.000000 changelist-0.1/src/changelist/__init__.py
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)    18007 2023-07-01 18:25:14.000000 changelist-0.1/src/changelist/__main__.py
-drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-01 18:52:31.108760 changelist-0.1/src/changelist.egg-info/
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)     4566 2023-07-01 18:52:31.000000 changelist-0.1/src/changelist.egg-info/PKG-INFO
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)      320 2023-07-01 18:52:31.000000 changelist-0.1/src/changelist.egg-info/SOURCES.txt
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)        1 2023-07-01 18:52:31.000000 changelist-0.1/src/changelist.egg-info/dependency_links.txt
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)       56 2023-07-01 18:52:31.000000 changelist-0.1/src/changelist.egg-info/entry_points.txt
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)       64 2023-07-01 18:52:31.000000 changelist-0.1/src/changelist.egg-info/requires.txt
--rw-r--r--   0 jarrod   (10000) jarrod   (10000)       11 2023-07-01 18:52:31.000000 changelist-0.1/src/changelist.egg-info/top_level.txt
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-01 14:29:14.071294 changelist-0.1rc0/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1504 2023-07-01 14:23:22.000000 changelist-0.1rc0/LICENSE.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      929 2023-07-01 14:29:14.070294 changelist-0.1rc0/PKG-INFO
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      364 2023-07-01 14:23:22.000000 changelist-0.1rc0/README.md
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      765 2023-07-01 14:24:19.000000 changelist-0.1rc0/pyproject.toml
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       38 2023-07-01 14:29:14.071294 changelist-0.1rc0/setup.cfg
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-01 14:29:14.067294 changelist-0.1rc0/src/
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-01 14:29:14.068294 changelist-0.1rc0/src/changelist/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)        0 2023-07-01 14:23:22.000000 changelist-0.1rc0/src/changelist/__init__.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)    17930 2023-07-01 14:23:22.000000 changelist-0.1rc0/src/changelist/__main__.py
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-07-01 14:29:14.070294 changelist-0.1rc0/src/changelist.egg-info/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      929 2023-07-01 14:29:14.000000 changelist-0.1rc0/src/changelist.egg-info/PKG-INFO
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      320 2023-07-01 14:29:14.000000 changelist-0.1rc0/src/changelist.egg-info/SOURCES.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)        1 2023-07-01 14:29:14.000000 changelist-0.1rc0/src/changelist.egg-info/dependency_links.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       56 2023-07-01 14:29:14.000000 changelist-0.1rc0/src/changelist.egg-info/entry_points.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       38 2023-07-01 14:29:14.000000 changelist-0.1rc0/src/changelist.egg-info/requires.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       11 2023-07-01 14:29:14.000000 changelist-0.1rc0/src/changelist.egg-info/top_level.txt
```

### Comparing `changelist-0.1/LICENSE.txt` & `changelist-0.1rc0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `changelist-0.1/pyproject.toml` & `changelist-0.1rc0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "changelist"
-version = "0.1"
+version = "0.1rc0"
 requires-python = ">=3.9"
 readme = "README.md"
-license = {file = "LICENSE.txt"}
+license = {file = "LICENSE"}
 classifiers = [
   "Development Status :: 3 - Alpha",
   "License :: OSI Approved :: BSD License",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
@@ -26,23 +26,7 @@
 ]
 
 [project.urls]
 "Source" = "https://github.com/scientific-python/changelist"
 
 [project.scripts]
 changelist = "changelist.__main__:main"
-
-[project.optional-dependencies]
-lint = ["pre-commit == 3.3.3"]
-
-[tool.ruff]
-line-length = 88
-target-version = "py39"
-select = [
-    "C",
-    "E",
-    "F",
-    "W",
-    "B",
-    "I",
-    "UP",
-]
```

### Comparing `changelist-0.1/src/changelist/__main__.py` & `changelist-0.1rc0/src/changelist/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 """Prepare an automatic changelog from GitHub's pull requests."""
 
 
-import argparse
-import json
-import logging
 import os
 import re
 import sys
+import argparse
+import logging
 import tempfile
-from collections import OrderedDict
-from collections.abc import Iterable
-from dataclasses import dataclass
+import json
 from pathlib import Path
+from dataclasses import dataclass
 from typing import Callable, Union
+from collections.abc import Iterable
+from collections import OrderedDict
 
 import requests
 import requests_cache
+from tqdm import tqdm
 from github import Github
-from github.Commit import Commit
-from github.NamedUser import NamedUser
 from github.PullRequest import PullRequest
-from tqdm import tqdm
+from github.NamedUser import NamedUser
+from github.Commit import Commit
+
 
 logger = logging.getLogger(__name__)
 
 here = Path(__file__).parent
 
 REQUESTS_CACHE_PATH = Path(tempfile.gettempdir()) / "github_cache.sqlite"
 
@@ -143,16 +144,16 @@
             logger.warning(
                 "reached page limit while querying authors in %r, "
                 "only the first %i authors will be included",
                 commit["commitUrl"],
                 self.PAGE_LIMIT,
             )
 
-        coauthors = {}
-        for _i, edge in enumerate(edges):
+        coauthors = dict()
+        for i, edge in enumerate(edges):
             node = edge["node"]
             user = node["user"]
             if user is None:
                 logger.warning(
                     "could not determine GitHub user for %r in %r",
                     node,
                     commit["commitUrl"],
@@ -216,16 +217,16 @@
 
     version: str = "x.y.z"
     title_template: str = "{repo_name} {version}"
     intro_template: str = """
 We're happy to announce the release of {repo_name} {version}!
 """
     outro_template: str = (
-        "_These lists are automatically generated, and may not be complete or may "
-        "contain duplicates._\n"
+        "*These lists are automatically generated, and may not be complete or may "
+        "contain duplicates.*\n"
     )
     # Associate regexes matching PR labels to a section titles in the release notes
     regex_section_map: tuple[tuple[str, str], ...] = (
         (".*Highlight.*", "Highlights"),
         (".*New feature.*", "New Features"),
         (".*Enhancement.*", "Enhancements"),
         (".*Performance.*", "Performance"),
@@ -325,19 +326,18 @@
         link = self._format_link(f"#{pr.number}", f"{pr.html_url}")
         yield f"  ({link}).\n"
 
     def _format_pr_section(
         self, title: str, pull_requests: set[PullRequest]
     ) -> Iterable[str]:
         """Format a section title and list its pull requests sorted by merge date."""
-        if pull_requests:
-            yield from self._format_section_title(title, level=2)
-            for pr in sorted(pull_requests, key=lambda pr: pr.merged_at):
-                yield from self._format_pull_request(pr)
-            yield "\n"
+        yield from self._format_section_title(title, level=2)
+        for pr in sorted(pull_requests, key=lambda pr: pr.merged_at):
+            yield from self._format_pull_request(pr)
+        yield "\n"
 
     def _format_user_line(self, user: Union[NamedUser]) -> str:
         line = f"@{user.login}"
         line = self._format_link(line, user.html_url)
         if user.name:
             line = f"{user.name} ({line})"
         return line + ",\n"
@@ -361,17 +361,15 @@
 
         yield f"{len(reviewers)} reviewers added to this release (alphabetically):\n"
         reviewers_lines = map(self._format_user_line, reviewers)
         yield from sorted(reviewers_lines, key=lambda s: s.lower())
         yield "\n"
 
     def _format_intro(self):
-        intro = self.intro_template.format(
-            repo_name=self.repo_name, version=self.version
-        )
+        intro = self.intro_template.format(repo_name=self.repo_name, version=self.version)
         # Make sure to return exactly one line at a time
         yield from (f"{line}\n" for line in intro.split("\n"))
 
     def _format_outro(self) -> Iterable[str]:
         outro = self.outro_template
         # Make sure to return exactly one line at a time
         yield from (f"{line}\n" for line in outro.split("\n"))
@@ -465,15 +463,15 @@
     """
     level = {0: logging.WARNING, 1: logging.INFO}.get(verbose, logging.DEBUG)
     logger.setLevel(level)
 
     requests_cache.install_cache(
         REQUESTS_CACHE_PATH, backend="sqlite", expire_after=3600
     )
-    print(f"Using requests cache at {REQUESTS_CACHE_PATH}", file=sys.stderr)
+    print(f"Using requests cache at {REQUESTS_CACHE_PATH}")
     if clear_cache:
         requests_cache.clear()
         logger.info("cleared requests cache at %s", REQUESTS_CACHE_PATH)
 
     gh_token = os.environ.get("GH_TOKEN")
     if gh_token is None:
         raise RuntimeError(
```

