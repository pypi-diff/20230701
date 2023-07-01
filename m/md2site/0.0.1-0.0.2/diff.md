# Comparing `tmp/md2site-0.0.1.tar.gz` & `tmp/md2site-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md2site-0.0.1.tar", max compression
+gzip compressed data, was "md2site-0.0.2.tar", max compression
```

## Comparing `md2site-0.0.1.tar` & `md2site-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,10 @@
--rw-r--r--   0        0        0    35150 2023-06-30 04:57:44.432528 md2site-0.0.1/LICENSE.md
--rw-r--r--   0        0        0       56 2023-06-30 04:57:44.447034 md2site-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-06-30 04:57:44.447067 md2site-0.0.1/md2site/__init__.py
--rw-r--r--   0        0        0     1002 2023-06-30 04:57:44.447202 md2site-0.0.1/md2site/generator.py
--rw-r--r--   0        0        0      320 2023-06-29 08:00:43.125549 md2site-0.0.1/md2site/link.py
--rw-r--r--   0        0        0     1792 2023-06-30 04:57:44.447293 md2site-0.0.1/md2site/post.py
--rw-r--r--   0        0        0        0 2023-06-30 04:57:44.455610 md2site-0.0.1/md2site/py.typed
--rw-r--r--   0        0        0     1169 2023-06-30 04:57:44.447382 md2site-0.0.1/md2site/renderer.py
--rw-r--r--   0        0        0      156 2023-06-30 04:57:44.447465 md2site-0.0.1/md2site/site.py
--rw-r--r--   0        0        0      193 2023-06-30 04:26:06.695130 md2site-0.0.1/md2site/test_render.py
--rw-r--r--   0        0        0     1015 2023-06-30 04:57:44.458453 md2site-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1013 1970-01-01 00:00:00.000000 md2site-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35150 2023-06-30 04:57:44.432528 md2site-0.0.2/LICENSE.md
+-rw-r--r--   0        0        0       56 2023-06-30 04:57:44.447034 md2site-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 04:57:44.447067 md2site-0.0.2/md2site/__init__.py
+-rw-r--r--   0        0        0     3056 2023-07-01 09:23:51.293045 md2site-0.0.2/md2site/generator.py
+-rw-r--r--   0        0        0     2409 2023-07-01 09:43:22.171523 md2site-0.0.2/md2site/post.py
+-rw-r--r--   0        0        0        0 2023-06-30 04:57:44.455610 md2site-0.0.2/md2site/py.typed
+-rw-r--r--   0        0        0     2169 2023-07-01 05:43:16.526132 md2site-0.0.2/md2site/renderer.py
+-rw-r--r--   0        0        0      406 2023-07-01 09:21:44.135485 md2site-0.0.2/md2site/site.py
+-rw-r--r--   0        0        0     1015 2023-07-01 09:46:39.237254 md2site-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1013 1970-01-01 00:00:00.000000 md2site-0.0.2/PKG-INFO
```

### Comparing `md2site-0.0.1/LICENSE.md` & `md2site-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `md2site-0.0.1/md2site/post.py` & `md2site-0.0.2/md2site/post.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
-from dataclasses import dataclass
-from datetime import datetime
+from dataclasses import dataclass, field
+from datetime import datetime, timezone
 from pathlib import Path
 from typing import TextIO
 import os
 
 import yaml
 
 
@@ -16,48 +16,67 @@
 
 @dataclass
 class Post:
     """
     All information necessary to render a post.
     """
 
+    name: str
     title: str
     content: str
     summary: str
     created_at: datetime
     slug: str
-    backlinks: list[str] = list()
+    backlinks: list[str] = field(default_factory=list)
 
     @classmethod
     def from_file(cls, filepath: Path) -> Post:
         with open(filepath, "r", encoding="utf-8") as f:
             content = separate_frontmatter(f)
             name = filepath.stem
-            created_at = datetime.fromtimestamp(os.path.getctime(filepath))
+            if "title" in content.frontmatter:
+                title = content.frontmatter["title"]
+            else:
+                title = name
+
+            if "date" in content.frontmatter:
+                created_at = content.frontmatter["date"]
+                print(created_at)
+            else:
+                created_at = datetime.fromtimestamp(os.path.getctime(filepath)).replace(
+                    tzinfo=timezone.utc
+                )
+                print(created_at)
             return Post(
-                title=name,
+                name=name,
+                title=title,
                 content=content.body,
                 summary=content.body[:140],
                 created_at=created_at,
                 slug=name_to_slug(name),
             )
 
 
 def parse_frontmatter(yaml_text: str) -> dict[str, str]:
-    return yaml.safe_load(yaml_text)
+    parsed = yaml.safe_load(yaml_text)
+    if parsed is not None:
+        return parsed
+    else:
+        return {}
 
 
 def separate_frontmatter(markdown: TextIO) -> MarkdownContent:
     is_frontmatter = False
     frontmatter_lines: list[str] = []
     body_lines: list[str] = []
     for line_number, line in enumerate(markdown):
-        if line_number == 0 and line == "---":
+        if line_number == 0 and line.strip() == "---":
+            is_frontmatter = True
             continue
-        if is_frontmatter and line == "---":
+        if is_frontmatter and line.strip() == "---":
             is_frontmatter = False
             continue
         if is_frontmatter:
             frontmatter_lines.append(line)
         else:
             body_lines.append(line)
```

### Comparing `md2site-0.0.1/pyproject.toml` & `md2site-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "md2site"
-version = "0.0.1"
+version = "0.0.2"
 description = "A static site generator with bare-minimum functionality."
 license = "GPL-3.0-or-later"
 authors = ["Yoonseop Kang <e0engoon@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/e0en/md2site"
 repository = "https://github.com/e0en/md2site"
 classifiers = [
```

### Comparing `md2site-0.0.1/PKG-INFO` & `md2site-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2site
-Version: 0.0.1
+Version: 0.0.2
 Summary: A static site generator with bare-minimum functionality.
 Home-page: https://github.com/e0en/md2site
 License: GPL-3.0-or-later
 Author: Yoonseop Kang
 Author-email: e0engoon@gmail.com
 Requires-Python: >=3.10.5,<4.0.0
 Classifier: Development Status :: 1 - Planning
```

