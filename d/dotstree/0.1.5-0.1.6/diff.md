# Comparing `tmp/dotstree-0.1.5.tar.gz` & `tmp/dotstree-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotstree-0.1.5.tar", last modified: Sat Jul  1 04:56:17 2023, max compression
+gzip compressed data, was "dotstree-0.1.6.tar", last modified: Sat Jul  1 06:40:15 2023, max compression
```

## Comparing `dotstree-0.1.5.tar` & `dotstree-0.1.6.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2023-07-01 04:56:17.837905 dotstree-0.1.5/
--rw-r--r--   0 chaim     (1000) chaim     (1000)       38 2021-07-05 00:18:19.000000 dotstree-0.1.5/.gitignore
--rw-r--r--   0 chaim     (1000) chaim     (1000)     1368 2023-07-01 04:56:17.837905 dotstree-0.1.5/PKG-INFO
--rw-r--r--   0 chaim     (1000) chaim     (1000)     1110 2021-07-26 00:19:00.000000 dotstree-0.1.5/README.md
-drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2023-07-01 04:56:17.837905 dotstree-0.1.5/doc/
--rw-r--r--   0 chaim     (1000) chaim     (1000)     8227 2021-07-13 05:16:01.000000 dotstree-0.1.5/doc/details.md
--rw-r--r--   0 chaim     (1000) chaim     (1000)     2334 2021-07-19 03:03:12.000000 dotstree-0.1.5/doc/howto.md
--rw-r--r--   0 chaim     (1000) chaim     (1000)     1102 2021-07-13 05:16:01.000000 dotstree-0.1.5/doc/why-not-gnu-stow.md
--rw-r--r--   0 chaim     (1000) chaim     (1000)       38 2023-07-01 04:56:17.837905 dotstree-0.1.5/setup.cfg
--rw-r--r--   0 chaim     (1000) chaim     (1000)      782 2023-07-01 04:55:46.000000 dotstree-0.1.5/setup.py
-drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2023-07-01 04:56:17.834571 dotstree-0.1.5/src/
-drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2023-07-01 04:56:17.837905 dotstree-0.1.5/src/dotstree/
--rw-r--r--   0 chaim     (1000) chaim     (1000)        0 2023-06-30 22:28:39.000000 dotstree-0.1.5/src/dotstree/__init__.py
--rw-r--r--   0 chaim     (1000) chaim     (1000)     3391 2023-07-01 04:55:46.000000 dotstree-0.1.5/src/dotstree/lib.py
--rw-r--r--   0 chaim     (1000) chaim     (1000)     4885 2023-07-01 04:55:46.000000 dotstree-0.1.5/src/dotstree/main.py
-drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2023-07-01 04:56:17.837905 dotstree-0.1.5/src/dotstree.egg-info/
--rw-r--r--   0 chaim     (1000) chaim     (1000)     1368 2023-07-01 04:56:17.000000 dotstree-0.1.5/src/dotstree.egg-info/PKG-INFO
--rw-r--r--   0 chaim     (1000) chaim     (1000)      406 2023-07-01 04:56:17.000000 dotstree-0.1.5/src/dotstree.egg-info/SOURCES.txt
--rw-r--r--   0 chaim     (1000) chaim     (1000)        1 2023-07-01 04:56:17.000000 dotstree-0.1.5/src/dotstree.egg-info/dependency_links.txt
--rw-r--r--   0 chaim     (1000) chaim     (1000)       44 2023-07-01 04:56:17.000000 dotstree-0.1.5/src/dotstree.egg-info/entry_points.txt
--rw-r--r--   0 chaim     (1000) chaim     (1000)       62 2023-07-01 04:56:17.000000 dotstree-0.1.5/src/dotstree.egg-info/requires.txt
--rw-r--r--   0 chaim     (1000) chaim     (1000)        9 2023-07-01 04:56:17.000000 dotstree-0.1.5/src/dotstree.egg-info/top_level.txt
-drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2023-07-01 04:56:17.837905 dotstree-0.1.5/tests/
--rw-r--r--   0 chaim     (1000) chaim     (1000)     2334 2023-06-30 22:28:39.000000 dotstree-0.1.5/tests/test_install_symlink.py
--rw-r--r--   0 chaim     (1000) chaim     (1000)      293 2021-07-19 04:45:19.000000 dotstree-0.1.5/yaghm.yaml
+drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2023-07-01 06:40:15.658418 dotstree-0.1.6/
+-rw-r--r--   0 chaim     (1000) chaim     (1000)       38 2021-07-05 00:18:19.000000 dotstree-0.1.6/.gitignore
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     1368 2023-07-01 06:40:15.658418 dotstree-0.1.6/PKG-INFO
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     1110 2021-07-26 00:19:00.000000 dotstree-0.1.6/README.md
+drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2023-07-01 06:40:15.658418 dotstree-0.1.6/doc/
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     8227 2021-07-13 05:16:01.000000 dotstree-0.1.6/doc/details.md
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     2334 2021-07-19 03:03:12.000000 dotstree-0.1.6/doc/howto.md
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     1102 2021-07-13 05:16:01.000000 dotstree-0.1.6/doc/why-not-gnu-stow.md
+-rw-r--r--   0 chaim     (1000) chaim     (1000)       38 2023-07-01 06:40:15.658418 dotstree-0.1.6/setup.cfg
+-rw-r--r--   0 chaim     (1000) chaim     (1000)      782 2023-07-01 06:40:05.000000 dotstree-0.1.6/setup.py
+drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2023-07-01 06:40:15.658418 dotstree-0.1.6/src/
+drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2023-07-01 06:40:15.658418 dotstree-0.1.6/src/dotstree/
+-rw-r--r--   0 chaim     (1000) chaim     (1000)        0 2023-06-30 22:28:39.000000 dotstree-0.1.6/src/dotstree/__init__.py
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     3391 2023-07-01 05:15:29.000000 dotstree-0.1.6/src/dotstree/lib.py
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     5128 2023-07-01 06:40:05.000000 dotstree-0.1.6/src/dotstree/main.py
+drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2023-07-01 06:40:15.658418 dotstree-0.1.6/src/dotstree.egg-info/
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     1368 2023-07-01 06:40:15.000000 dotstree-0.1.6/src/dotstree.egg-info/PKG-INFO
+-rw-r--r--   0 chaim     (1000) chaim     (1000)      468 2023-07-01 06:40:15.000000 dotstree-0.1.6/src/dotstree.egg-info/SOURCES.txt
+-rw-r--r--   0 chaim     (1000) chaim     (1000)        1 2023-07-01 06:40:15.000000 dotstree-0.1.6/src/dotstree.egg-info/dependency_links.txt
+-rw-r--r--   0 chaim     (1000) chaim     (1000)       44 2023-07-01 06:40:15.000000 dotstree-0.1.6/src/dotstree.egg-info/entry_points.txt
+-rw-r--r--   0 chaim     (1000) chaim     (1000)       62 2023-07-01 06:40:15.000000 dotstree-0.1.6/src/dotstree.egg-info/requires.txt
+-rw-r--r--   0 chaim     (1000) chaim     (1000)        9 2023-07-01 06:40:15.000000 dotstree-0.1.6/src/dotstree.egg-info/top_level.txt
+drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2023-07-01 06:40:15.658418 dotstree-0.1.6/tests/
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     1281 2023-07-01 06:40:05.000000 dotstree-0.1.6/tests/test_check_symlinks_status.py
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     2334 2023-06-30 22:28:39.000000 dotstree-0.1.6/tests/test_install_symlink.py
+-rw-r--r--   0 chaim     (1000) chaim     (1000)      218 2023-07-01 06:40:05.000000 dotstree-0.1.6/tests/test_status_icon.py
+-rw-r--r--   0 chaim     (1000) chaim     (1000)      293 2021-07-19 04:45:19.000000 dotstree-0.1.6/yaghm.yaml
```

### Comparing `dotstree-0.1.5/PKG-INFO` & `dotstree-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotstree
-Version: 0.1.5
+Version: 0.1.6
 Summary: Flexible dotfile manager based on directory trees.
 Home-page: https://www.github.com/metov/dotstree
 Author: Azat Akhmetov
 Author-email: azatinfo@yandex.com
 Description-Content-Type: text/markdown
 
 # Dotfiles manager based on directory trees
```

### Comparing `dotstree-0.1.5/README.md` & `dotstree-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `dotstree-0.1.5/doc/details.md` & `dotstree-0.1.6/doc/details.md`

 * *Files identical despite different names*

### Comparing `dotstree-0.1.5/doc/howto.md` & `dotstree-0.1.6/doc/howto.md`

 * *Files identical despite different names*

### Comparing `dotstree-0.1.5/doc/why-not-gnu-stow.md` & `dotstree-0.1.6/doc/why-not-gnu-stow.md`

 * *Files identical despite different names*

### Comparing `dotstree-0.1.5/setup.py` & `dotstree-0.1.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from pathlib import Path
 
 from setuptools import find_packages
 
 setup(
     name="dotstree",
-    version="0.1.5",
+    version="0.1.6",
     description="Flexible dotfile manager based on directory trees.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://www.github.com/metov/dotstree",
     author="Azat Akhmetov",
     author_email="azatinfo@yandex.com",
     packages=find_packages(where="src"),
```

### Comparing `dotstree-0.1.5/src/dotstree/lib.py` & `dotstree-0.1.6/src/dotstree/lib.py`

 * *Files identical despite different names*

### Comparing `dotstree-0.1.5/src/dotstree/main.py` & `dotstree-0.1.6/src/dotstree/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,42 +45,35 @@
         install_specs(spec)
     elif args["check"]:
         check_specs(spec)
     else:
         log.critical("Unexpected arguments")
 
 
+def status_icon(status: bool | None) -> str:
+    if status:
+        return "🟢"
+
+    if status == False:
+        return "🔴"
+
+    return "⚪"
+
+
 def check_specs(all_specs):
     status = []
     for name, spec in tqdm(all_specs.items()):
         layer, _, spec_name = name.rpartition("/")
         res = {"Layer": layer, "Spec": spec_name}
 
         t1 = time()
-        res["Symlinks"] = "⚪"
-        if "symlinks" in spec:
-            res["Symlinks"] = "🟢"
-            for ln in spec.get("symlinks"):
-                origin = Path(ln["from"]).expanduser()
-                target = Path(ln["to"])
-                if not symlink_is_correct(Path(origin), Path(target)):
-                    res["Symlinks"] = "🔴"
+        res["Symlinks"] = status_icon(check_symlinks_status(spec))
 
         t2 = time()
-
-        res["Program"] = "⚪"
-        if "check" in spec:
-            result = run_command(spec["check"], spec["path"])
-            if result.returncode == 0:
-                res["Program"] = "🟢"
-            else:
-                res["Program"] = "🔴"
-                msg = f"Command: {spec['check']}"
-                log.info(msg + f"\nStandard error:\n{result.stderr}")
-                log.debug(f"Standard output:\n{result.stdout}")
+        res["Program"] = status_icon(check_program_status(spec))
 
         t3 = time()
 
         res["Symlink time"] = t2 - t1
         res["Check time"] = t3 - t2
 
         status.append(res)
@@ -90,14 +83,43 @@
     status.sort(key=itemgetter("Program"), reverse=True)
     status.sort(key=itemgetter("Symlinks"), reverse=True)
     status.sort(key=itemgetter("Layer"))
     status.sort(key=lambda d: d["Layer"] != "")
     print(tabulate(status, headers="keys", floatfmt=".3f"))
 
 
+def check_symlinks_status(spec: dict) -> bool | None:
+    if "symlinks" not in spec:
+        return None
+
+    # Note that an empty symlinks block is always "correct"
+
+    for ln in spec["symlinks"]:
+        origin = Path(ln["from"]).expanduser()
+        target = Path(ln["to"])
+        if not symlink_is_correct(Path(origin), Path(target)):
+            return False
+
+    return True
+
+
+def check_program_status(spec: dict) -> bool | None:
+    if "check" not in spec:
+        return None
+
+    result = run_command(spec["check"], spec["path"])
+    if result.returncode == 0:
+        return True
+
+    msg = f"Command: {spec['check']}"
+    log.debug(f"Standard output:\n{result.stdout}")
+    log.info(msg + f"\nStandard error:\n{result.stderr}")
+    return False
+
+
 def install_specs(all_specs):
     for name, spec in tqdm(all_specs.items()):
         if "symlinks" in spec:
             for ln in spec.get("symlinks"):
                 install_symlink(Path(ln["from"]).expanduser(), Path(ln["to"]))
 
         if "install" in spec:
```

### Comparing `dotstree-0.1.5/src/dotstree.egg-info/PKG-INFO` & `dotstree-0.1.6/src/dotstree.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotstree
-Version: 0.1.5
+Version: 0.1.6
 Summary: Flexible dotfile manager based on directory trees.
 Home-page: https://www.github.com/metov/dotstree
 Author: Azat Akhmetov
 Author-email: azatinfo@yandex.com
 Description-Content-Type: text/markdown
 
 # Dotfiles manager based on directory trees
```

### Comparing `dotstree-0.1.5/tests/test_install_symlink.py` & `dotstree-0.1.6/tests/test_install_symlink.py`

 * *Files identical despite different names*

