# Comparing `tmp/dotstree-0.1.4.tar.gz` & `tmp/dotstree-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotstree-0.1.4.tar", last modified: Tue Nov  1 03:28:29 2022, max compression
+gzip compressed data, was "dotstree-0.1.5.tar", last modified: Sat Jul  1 04:56:17 2023, max compression
```

## Comparing `dotstree-0.1.4.tar` & `dotstree-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,25 @@
-drwxr-xr-x   0 chad      (1000) chad      (1000)        0 2022-11-01 03:28:29.760373 dotstree-0.1.4/
--rw-r--r--   0 chad      (1000) chad      (1000)     1368 2022-11-01 03:28:29.760373 dotstree-0.1.4/PKG-INFO
--rw-r--r--   0 chad      (1000) chad      (1000)     1110 2021-07-26 00:19:00.000000 dotstree-0.1.4/README.md
--rw-r--r--   0 chad      (1000) chad      (1000)       38 2022-11-01 03:28:29.760373 dotstree-0.1.4/setup.cfg
--rw-r--r--   0 chad      (1000) chad      (1000)      782 2022-11-01 03:28:17.000000 dotstree-0.1.4/setup.py
-drwxr-xr-x   0 chad      (1000) chad      (1000)        0 2022-11-01 03:28:29.760373 dotstree-0.1.4/src/
-drwxr-xr-x   0 chad      (1000) chad      (1000)        0 2022-11-01 03:28:29.760373 dotstree-0.1.4/src/dotstree/
--rw-r--r--   0 chad      (1000) chad      (1000)        0 2022-11-01 02:18:59.000000 dotstree-0.1.4/src/dotstree/__init__.py
--rw-r--r--   0 chad      (1000) chad      (1000)     3333 2022-11-01 02:18:59.000000 dotstree-0.1.4/src/dotstree/lib.py
--rw-r--r--   0 chad      (1000) chad      (1000)     4861 2022-11-01 03:28:17.000000 dotstree-0.1.4/src/dotstree/main.py
-drwxr-xr-x   0 chad      (1000) chad      (1000)        0 2022-11-01 03:28:29.760373 dotstree-0.1.4/src/dotstree.egg-info/
--rw-r--r--   0 chad      (1000) chad      (1000)     1368 2022-11-01 03:28:29.000000 dotstree-0.1.4/src/dotstree.egg-info/PKG-INFO
--rw-r--r--   0 chad      (1000) chad      (1000)      302 2022-11-01 03:28:29.000000 dotstree-0.1.4/src/dotstree.egg-info/SOURCES.txt
--rw-r--r--   0 chad      (1000) chad      (1000)        1 2022-11-01 03:28:29.000000 dotstree-0.1.4/src/dotstree.egg-info/dependency_links.txt
--rw-r--r--   0 chad      (1000) chad      (1000)       44 2022-11-01 03:28:29.000000 dotstree-0.1.4/src/dotstree.egg-info/entry_points.txt
--rw-r--r--   0 chad      (1000) chad      (1000)       62 2022-11-01 03:28:29.000000 dotstree-0.1.4/src/dotstree.egg-info/requires.txt
--rw-r--r--   0 chad      (1000) chad      (1000)        9 2022-11-01 03:28:29.000000 dotstree-0.1.4/src/dotstree.egg-info/top_level.txt
+drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2023-07-01 04:56:17.837905 dotstree-0.1.5/
+-rw-r--r--   0 chaim     (1000) chaim     (1000)       38 2021-07-05 00:18:19.000000 dotstree-0.1.5/.gitignore
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     1368 2023-07-01 04:56:17.837905 dotstree-0.1.5/PKG-INFO
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     1110 2021-07-26 00:19:00.000000 dotstree-0.1.5/README.md
+drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2023-07-01 04:56:17.837905 dotstree-0.1.5/doc/
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     8227 2021-07-13 05:16:01.000000 dotstree-0.1.5/doc/details.md
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     2334 2021-07-19 03:03:12.000000 dotstree-0.1.5/doc/howto.md
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     1102 2021-07-13 05:16:01.000000 dotstree-0.1.5/doc/why-not-gnu-stow.md
+-rw-r--r--   0 chaim     (1000) chaim     (1000)       38 2023-07-01 04:56:17.837905 dotstree-0.1.5/setup.cfg
+-rw-r--r--   0 chaim     (1000) chaim     (1000)      782 2023-07-01 04:55:46.000000 dotstree-0.1.5/setup.py
+drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2023-07-01 04:56:17.834571 dotstree-0.1.5/src/
+drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2023-07-01 04:56:17.837905 dotstree-0.1.5/src/dotstree/
+-rw-r--r--   0 chaim     (1000) chaim     (1000)        0 2023-06-30 22:28:39.000000 dotstree-0.1.5/src/dotstree/__init__.py
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     3391 2023-07-01 04:55:46.000000 dotstree-0.1.5/src/dotstree/lib.py
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     4885 2023-07-01 04:55:46.000000 dotstree-0.1.5/src/dotstree/main.py
+drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2023-07-01 04:56:17.837905 dotstree-0.1.5/src/dotstree.egg-info/
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     1368 2023-07-01 04:56:17.000000 dotstree-0.1.5/src/dotstree.egg-info/PKG-INFO
+-rw-r--r--   0 chaim     (1000) chaim     (1000)      406 2023-07-01 04:56:17.000000 dotstree-0.1.5/src/dotstree.egg-info/SOURCES.txt
+-rw-r--r--   0 chaim     (1000) chaim     (1000)        1 2023-07-01 04:56:17.000000 dotstree-0.1.5/src/dotstree.egg-info/dependency_links.txt
+-rw-r--r--   0 chaim     (1000) chaim     (1000)       44 2023-07-01 04:56:17.000000 dotstree-0.1.5/src/dotstree.egg-info/entry_points.txt
+-rw-r--r--   0 chaim     (1000) chaim     (1000)       62 2023-07-01 04:56:17.000000 dotstree-0.1.5/src/dotstree.egg-info/requires.txt
+-rw-r--r--   0 chaim     (1000) chaim     (1000)        9 2023-07-01 04:56:17.000000 dotstree-0.1.5/src/dotstree.egg-info/top_level.txt
+drwxr-xr-x   0 chaim     (1000) chaim     (1000)        0 2023-07-01 04:56:17.837905 dotstree-0.1.5/tests/
+-rw-r--r--   0 chaim     (1000) chaim     (1000)     2334 2023-06-30 22:28:39.000000 dotstree-0.1.5/tests/test_install_symlink.py
+-rw-r--r--   0 chaim     (1000) chaim     (1000)      293 2021-07-19 04:45:19.000000 dotstree-0.1.5/yaghm.yaml
```

### Comparing `dotstree-0.1.4/PKG-INFO` & `dotstree-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotstree
-Version: 0.1.4
+Version: 0.1.5
 Summary: Flexible dotfile manager based on directory trees.
 Home-page: https://www.github.com/metov/dotstree
 Author: Azat Akhmetov
 Author-email: azatinfo@yandex.com
 Description-Content-Type: text/markdown
 
 # Dotfiles manager based on directory trees
```

### Comparing `dotstree-0.1.4/README.md` & `dotstree-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `dotstree-0.1.4/setup.py` & `dotstree-0.1.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from pathlib import Path
 
 from setuptools import find_packages
 
 setup(
     name="dotstree",
-    version="0.1.4",
+    version="0.1.5",
     description="Flexible dotfile manager based on directory trees.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://www.github.com/metov/dotstree",
     author="Azat Akhmetov",
     author_email="azatinfo@yandex.com",
     packages=find_packages(where="src"),
```

### Comparing `dotstree-0.1.4/src/dotstree/lib.py` & `dotstree-0.1.5/src/dotstree/lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,8 +116,14 @@
         return False
 
     return True
 
 
 def run_command(cmd, workdir, capture_output=True):
     log.debug(f"Running {cmd}")
-    return subprocess.run(cmd, shell=True, capture_output=capture_output, cwd=workdir)
+    return subprocess.run(
+        cmd,
+        shell=True,
+        capture_output=capture_output,
+        cwd=workdir,
+        text=True,
+    )
```

### Comparing `dotstree-0.1.4/src/dotstree/main.py` & `dotstree-0.1.5/src/dotstree/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     else:
         log.critical("Unexpected arguments")
 
 
 def check_specs(all_specs):
     status = []
     for name, spec in tqdm(all_specs.items()):
-
         layer, _, spec_name = name.rpartition("/")
         res = {"Layer": layer, "Spec": spec_name}
 
         t1 = time()
         res["Symlinks"] = "⚪"
         if "symlinks" in spec:
             res["Symlinks"] = "🟢"
@@ -72,16 +71,16 @@
         if "check" in spec:
             result = run_command(spec["check"], spec["path"])
             if result.returncode == 0:
                 res["Program"] = "🟢"
             else:
                 res["Program"] = "🔴"
                 msg = f"Command: {spec['check']}"
-                log.info(msg + f"\nStandard error:\n{result.stderr.decode()}")
-                log.debug(f"Standard output:\n{result.stdout.decode()}")
+                log.info(msg + f"\nStandard error:\n{result.stderr}")
+                log.debug(f"Standard output:\n{result.stdout}")
 
         t3 = time()
 
         res["Symlink time"] = t2 - t1
         res["Check time"] = t3 - t2
 
         status.append(res)
@@ -100,26 +99,28 @@
         if "symlinks" in spec:
             for ln in spec.get("symlinks"):
                 install_symlink(Path(ln["from"]).expanduser(), Path(ln["to"]))
 
         if "install" in spec:
             if "check" in spec:
                 result = run_command("pwd", spec["path"].absolute())
-                print(result.stdout.decode())
+                print(result.stdout)
 
                 result = run_command(spec["check"], spec["path"])
                 if result.returncode == 0:
                     log.info(f"Skipping {name} because check command succeeded.")
                     continue
 
             log.info(f"Installing {name}")
             install_cmd = spec["install"]
-            res = run_command(install_cmd, spec["path"], capture_output=False)
+            res = run_command(install_cmd, spec["path"], capture_output=True)
+            log.debug(f"Output from command:\n{res.stdout}")
+
             if res.returncode != 0:
-                msg = res.stderr.decode() if res.stderr else str(res.stderr)
+                msg = res.stderr if res.stderr else str(res.stderr)
                 log.error(f"{spec['install']} failed with:\n{msg}")
 
 
 def install_symlink(origin, target):
     if symlink_is_correct(origin, target):
         log.debug(f"Skipping {origin} because it already points to {target}")
         return
```

### Comparing `dotstree-0.1.4/src/dotstree.egg-info/PKG-INFO` & `dotstree-0.1.5/src/dotstree.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotstree
-Version: 0.1.4
+Version: 0.1.5
 Summary: Flexible dotfile manager based on directory trees.
 Home-page: https://www.github.com/metov/dotstree
 Author: Azat Akhmetov
 Author-email: azatinfo@yandex.com
 Description-Content-Type: text/markdown
 
 # Dotfiles manager based on directory trees
```

