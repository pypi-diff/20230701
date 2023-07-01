# Comparing `tmp/md2site-0.0.2.tar.gz` & `tmp/md2site-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md2site-0.0.2.tar", max compression
+gzip compressed data, was "md2site-0.0.3.tar", max compression
```

## Comparing `md2site-0.0.2.tar` & `md2site-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35150 2023-06-30 04:57:44.432528 md2site-0.0.2/LICENSE.md
--rw-r--r--   0        0        0       56 2023-06-30 04:57:44.447034 md2site-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-06-30 04:57:44.447067 md2site-0.0.2/md2site/__init__.py
--rw-r--r--   0        0        0     3056 2023-07-01 09:23:51.293045 md2site-0.0.2/md2site/generator.py
--rw-r--r--   0        0        0     2409 2023-07-01 09:43:22.171523 md2site-0.0.2/md2site/post.py
--rw-r--r--   0        0        0        0 2023-06-30 04:57:44.455610 md2site-0.0.2/md2site/py.typed
--rw-r--r--   0        0        0     2169 2023-07-01 05:43:16.526132 md2site-0.0.2/md2site/renderer.py
--rw-r--r--   0        0        0      406 2023-07-01 09:21:44.135485 md2site-0.0.2/md2site/site.py
--rw-r--r--   0        0        0     1015 2023-07-01 09:46:39.237254 md2site-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1013 1970-01-01 00:00:00.000000 md2site-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35150 2023-06-30 04:57:44.432528 md2site-0.0.3/LICENSE.md
+-rw-r--r--   0        0        0       56 2023-06-30 04:57:44.447034 md2site-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 04:57:44.447067 md2site-0.0.3/md2site/__init__.py
+-rw-r--r--   0        0        0     3277 2023-07-01 10:28:09.244428 md2site-0.0.3/md2site/generator.py
+-rw-r--r--   0        0        0     2409 2023-07-01 09:43:22.171523 md2site-0.0.3/md2site/post.py
+-rw-r--r--   0        0        0        0 2023-06-30 04:57:44.455610 md2site-0.0.3/md2site/py.typed
+-rw-r--r--   0        0        0     2169 2023-07-01 05:43:16.526132 md2site-0.0.3/md2site/renderer.py
+-rw-r--r--   0        0        0      406 2023-07-01 09:21:44.135485 md2site-0.0.3/md2site/site.py
+-rw-r--r--   0        0        0     1015 2023-07-01 10:29:18.872479 md2site-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1013 1970-01-01 00:00:00.000000 md2site-0.0.3/PKG-INFO
```

### Comparing `md2site-0.0.2/LICENSE.md` & `md2site-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `md2site-0.0.2/md2site/generator.py` & `md2site-0.0.3/md2site/generator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,27 @@
+import os
 from pathlib import Path
 import shutil
 
 import jinja2
 import toml
 
 from md2site.post import Post, name_to_slug
 from md2site.site import PostMetaData, Site
 
 from md2site.renderer import Parser, Renderer, extract_wikilinks
 
 
+def prepare_output_folder():
+    output_folder = Path("dist")
+    if output_folder.exists():
+        shutil.rmtree(output_folder, ignore_errors=True)
+    os.makedirs(output_folder)
+
+
 def load_config() -> Site:
     raw_config = toml.load("config.toml")
     name = raw_config["name"]
     base_url = raw_config["base_url"]
     return Site(base_url, name)
 
 
@@ -93,14 +101,15 @@
     for file in Path("./template").iterdir():
         if file.name.endswith(".html"):
             continue
         shutil.copyfile(file, output_folder / file.name)
 
 
 def generate():
+    prepare_output_folder()
     copy_static_files()
     site = load_config()
     posts = load_post_files()
     site.link_map = build_link_map(posts)
     site.recent_posts = [
         PostMetaData(p.name, p.title, p.created_at) for p in posts[:10]
     ]
```

### Comparing `md2site-0.0.2/md2site/post.py` & `md2site-0.0.3/md2site/post.py`

 * *Files identical despite different names*

### Comparing `md2site-0.0.2/md2site/renderer.py` & `md2site-0.0.3/md2site/renderer.py`

 * *Files identical despite different names*

### Comparing `md2site-0.0.2/pyproject.toml` & `md2site-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "md2site"
-version = "0.0.2"
+version = "0.0.3"
 description = "A static site generator with bare-minimum functionality."
 license = "GPL-3.0-or-later"
 authors = ["Yoonseop Kang <e0engoon@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/e0en/md2site"
 repository = "https://github.com/e0en/md2site"
 classifiers = [
```

### Comparing `md2site-0.0.2/PKG-INFO` & `md2site-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2site
-Version: 0.0.2
+Version: 0.0.3
 Summary: A static site generator with bare-minimum functionality.
 Home-page: https://github.com/e0en/md2site
 License: GPL-3.0-or-later
 Author: Yoonseop Kang
 Author-email: e0engoon@gmail.com
 Requires-Python: >=3.10.5,<4.0.0
 Classifier: Development Status :: 1 - Planning
```

