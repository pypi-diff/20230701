# Comparing `tmp/sourceknight-0.2.tar.gz` & `tmp/sourceknight-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourceknight-0.2.tar", last modified: Fri Dec 30 04:26:51 2022, max compression
+gzip compressed data, was "sourceknight-0.3.tar", last modified: Sat Jul  1 17:02:26 2023, max compression
```

## Comparing `sourceknight-0.2.tar` & `sourceknight-0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 04:26:51.331364 sourceknight-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2022-12-30 04:26:41.000000 sourceknight-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2022-12-30 04:26:51.331364 sourceknight-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2022-12-30 04:26:41.000000 sourceknight-0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2022-12-30 04:26:41.000000 sourceknight-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-30 04:26:51.331364 sourceknight-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      657 2022-12-30 04:26:41.000000 sourceknight-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 04:26:51.331364 sourceknight-0.2/sourceknight/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2022-12-30 04:26:41.000000 sourceknight-0.2/sourceknight/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2022-12-30 04:26:41.000000 sourceknight-0.2/sourceknight/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2022-12-30 04:26:41.000000 sourceknight-0.2/sourceknight/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2022-12-30 04:26:41.000000 sourceknight-0.2/sourceknight/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 04:26:51.331364 sourceknight-0.2/sourceknight/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2022-12-30 04:26:41.000000 sourceknight-0.2/sourceknight/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2022-12-30 04:26:41.000000 sourceknight-0.2/sourceknight/drivers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2022-12-30 04:26:41.000000 sourceknight-0.2/sourceknight/drivers/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2022-12-30 04:26:41.000000 sourceknight-0.2/sourceknight/drivers/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2022-12-30 04:26:41.000000 sourceknight-0.2/sourceknight/drivers/tar.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-30 04:26:41.000000 sourceknight-0.2/sourceknight/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2022-12-30 04:26:41.000000 sourceknight-0.2/sourceknight/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2022-12-30 04:26:41.000000 sourceknight-0.2/sourceknight/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2022-12-30 04:26:41.000000 sourceknight-0.2/sourceknight/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2022-12-30 04:26:41.000000 sourceknight-0.2/sourceknight/unpack.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2022-12-30 04:26:41.000000 sourceknight-0.2/sourceknight/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2022-12-30 04:26:41.000000 sourceknight-0.2/sourceknight/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 04:26:51.331364 sourceknight-0.2/sourceknight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2022-12-30 04:26:51.000000 sourceknight-0.2/sourceknight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      662 2022-12-30 04:26:51.000000 sourceknight-0.2/sourceknight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-30 04:26:51.000000 sourceknight-0.2/sourceknight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2022-12-30 04:26:51.000000 sourceknight-0.2/sourceknight.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2022-12-30 04:26:51.000000 sourceknight-0.2/sourceknight.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-30 04:26:51.000000 sourceknight-0.2/sourceknight.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:02:26.043079 sourceknight-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-01 17:02:16.000000 sourceknight-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-07-01 17:02:26.043079 sourceknight-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-07-01 17:02:16.000000 sourceknight-0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-01 17:02:16.000000 sourceknight-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 17:02:26.043079 sourceknight-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-01 17:02:16.000000 sourceknight-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:02:26.043079 sourceknight-0.3/sourceknight/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-01 17:02:16.000000 sourceknight-0.3/sourceknight/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-07-01 17:02:16.000000 sourceknight-0.3/sourceknight/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-01 17:02:16.000000 sourceknight-0.3/sourceknight/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-01 17:02:16.000000 sourceknight-0.3/sourceknight/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:02:26.043079 sourceknight-0.3/sourceknight/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-01 17:02:16.000000 sourceknight-0.3/sourceknight/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-01 17:02:16.000000 sourceknight-0.3/sourceknight/drivers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-01 17:02:16.000000 sourceknight-0.3/sourceknight/drivers/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-01 17:02:16.000000 sourceknight-0.3/sourceknight/drivers/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-01 17:02:16.000000 sourceknight-0.3/sourceknight/drivers/tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-01 17:02:16.000000 sourceknight-0.3/sourceknight/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-01 17:02:16.000000 sourceknight-0.3/sourceknight/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-01 17:02:16.000000 sourceknight-0.3/sourceknight/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-01 17:02:16.000000 sourceknight-0.3/sourceknight/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-01 17:02:16.000000 sourceknight-0.3/sourceknight/unpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-01 17:02:16.000000 sourceknight-0.3/sourceknight/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-07-01 17:02:16.000000 sourceknight-0.3/sourceknight/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:02:26.043079 sourceknight-0.3/sourceknight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-07-01 17:02:26.000000 sourceknight-0.3/sourceknight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-01 17:02:26.000000 sourceknight-0.3/sourceknight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 17:02:26.000000 sourceknight-0.3/sourceknight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-01 17:02:26.000000 sourceknight-0.3/sourceknight.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-01 17:02:26.000000 sourceknight-0.3/sourceknight.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-01 17:02:26.000000 sourceknight-0.3/sourceknight.egg-info/top_level.txt
```

### Comparing `sourceknight-0.2/LICENSE` & `sourceknight-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sourceknight-0.2/PKG-INFO` & `sourceknight-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sourceknight
-Version: 0.2
+Version: 0.3
 Summary: simple dependency manager for sourcemod projects
 Home-page: https://github.com/tmick0/sourceknight
 Author: travis mick
 Author-email: root@lo.calho.st
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -29,22 +29,22 @@
 
 The core concept of `sourceknight` is the *project*, which encapsulates any plugins you're trying to build and their dependencies (including sourcemod itself).
 
 A *project directory* will include a *project file* called `sourceknight.yaml` that defines all the parameters of your project, including its name,
 its dependencies, and the plugins it will build. The project file is written in [YAML](https://en.wikipedia.org/wiki/YAML).
 
 If building your own plugin, your project directory will likely also include any sourcepawn files you need, but this is optional --
-you can also also use `sourcepawn` just to simplify compiling a collection of third party plugins by declaring them as dependencies.
+you can also also use `sourceknight` just to simplify compiling a collection of third party plugins by declaring them as dependencies.
 
 A minimal `sourceknight.yaml` might look something like this:
 
 ```yaml
 project:
   name: myplugin-example
-  sourceknight: 0.2
+  sourceknight: 0.3
   dependencies:
     - name: sourcemod
       type: tar
       version: 1.10.0-git6503
       location: https://sm.alliedmods.net/smdrop/1.10/sourcemod-1.10.0-git6503-linux.tar.gz
       unpack:
       - source: /addons
@@ -76,14 +76,15 @@
 
 - `location`: URL to download the tar file from
 - Optional: `version`, which can be manually specified to help prevent re-downloading the same file unnecessarily
 
 **`git`:**
 
 - `repo`: Git repository URL to clone
+- Optional: `version`, a commit tag or branch to checkout instead of the default
 
 Both of these types of dependencies must have an `unpack` block, which tells us which files to copy out of them and where they belong relative to the `sourceknight` *build root*. The build root is a hidden directory maintained by `sourceknight` which will contain the entire sourcemod tree (i.e., it will contain the `addons` directory) as well as any other dependencies and sources specified by your project.
 
 In the example above, the `unpack` declaration for `sourcemod` says to unpack the `/addons` directory to `/addons`. In sourcemod's case, this means we're copying the entire contents of the archive. However, the [extended example project file](example/sourceknight.yaml) includes other examples of unpack declarations. Note that the destination of an unpack operation is always relative to the build tree. Multiple `source`, `dest` pairs can be specified in the `unpack` section if needed.
 
 ### Build specification
```

### Comparing `sourceknight-0.2/README.md` & `sourceknight-0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,22 +18,22 @@
 
 The core concept of `sourceknight` is the *project*, which encapsulates any plugins you're trying to build and their dependencies (including sourcemod itself).
 
 A *project directory* will include a *project file* called `sourceknight.yaml` that defines all the parameters of your project, including its name,
 its dependencies, and the plugins it will build. The project file is written in [YAML](https://en.wikipedia.org/wiki/YAML).
 
 If building your own plugin, your project directory will likely also include any sourcepawn files you need, but this is optional --
-you can also also use `sourcepawn` just to simplify compiling a collection of third party plugins by declaring them as dependencies.
+you can also also use `sourceknight` just to simplify compiling a collection of third party plugins by declaring them as dependencies.
 
 A minimal `sourceknight.yaml` might look something like this:
 
 ```yaml
 project:
   name: myplugin-example
-  sourceknight: 0.2
+  sourceknight: 0.3
   dependencies:
     - name: sourcemod
       type: tar
       version: 1.10.0-git6503
       location: https://sm.alliedmods.net/smdrop/1.10/sourcemod-1.10.0-git6503-linux.tar.gz
       unpack:
       - source: /addons
@@ -65,14 +65,15 @@
 
 - `location`: URL to download the tar file from
 - Optional: `version`, which can be manually specified to help prevent re-downloading the same file unnecessarily
 
 **`git`:**
 
 - `repo`: Git repository URL to clone
+- Optional: `version`, a commit tag or branch to checkout instead of the default
 
 Both of these types of dependencies must have an `unpack` block, which tells us which files to copy out of them and where they belong relative to the `sourceknight` *build root*. The build root is a hidden directory maintained by `sourceknight` which will contain the entire sourcemod tree (i.e., it will contain the `addons` directory) as well as any other dependencies and sources specified by your project.
 
 In the example above, the `unpack` declaration for `sourcemod` says to unpack the `/addons` directory to `/addons`. In sourcemod's case, this means we're copying the entire contents of the archive. However, the [extended example project file](example/sourceknight.yaml) includes other examples of unpack declarations. Note that the destination of an unpack operation is always relative to the build tree. Multiple `source`, `dest` pairs can be specified in the `unpack` section if needed.
 
 ### Build specification
```

### Comparing `sourceknight-0.2/setup.py` & `sourceknight-0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 from pathlib import Path
 
 setup(
     name="sourceknight",
-    version="0.2",
+    version="0.3",
     author="travis mick",
     author_email="root@lo.calho.st",
     description="simple dependency manager for sourcemod projects",
     long_description=(Path(__file__).parent / "README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/tmick0/sourceknight",
     packages=['sourceknight', 'sourceknight.drivers'],
```

### Comparing `sourceknight-0.2/sourceknight/build.py` & `sourceknight-0.3/sourceknight/build.py`

 * *Files identical despite different names*

### Comparing `sourceknight-0.2/sourceknight/compile.py` & `sourceknight-0.3/sourceknight/compile.py`

 * *Files identical despite different names*

### Comparing `sourceknight-0.2/sourceknight/context.py` & `sourceknight-0.3/sourceknight/context.py`

 * *Files identical despite different names*

### Comparing `sourceknight-0.2/sourceknight/dependencies.py` & `sourceknight-0.3/sourceknight/dependencies.py`

 * *Files identical despite different names*

### Comparing `sourceknight-0.2/sourceknight/drivers/base.py` & `sourceknight-0.3/sourceknight/drivers/base.py`

 * *Files identical despite different names*

### Comparing `sourceknight-0.2/sourceknight/drivers/git.py` & `sourceknight-0.3/sourceknight/drivers/git.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,25 +14,33 @@
 
     def check_update(self, current_model):
         return True
 
     def update(self, mgr):
         loc = os.path.join(self._ctx._path, '.sourceknight', 'cache', self._model.name)
         
+        fetched = False
         if os.path.isdir(loc):
             repo = git.Repo(loc)
-            logging.info(' Pulling from {:s}'.format(repo.remote().url))
-            repo.remote().pull()
         else:
             logging.info(' Cloning from {:s}'.format(self._model.params['repo']))
             repo = git.Repo.clone_from(self._model.params['repo'], loc)
+            fetched = True
 
-        # TODO: handle branches, tags, etc
         if self._model.version is None:
+            if not fetched:
+                logging.info(' Pulling from {:s}'.format(repo.remote().url))
+                repo.remote().pull()
             self._model.version = repo.head.commit.hexsha
+        else:
+            if not fetched:
+                logging.info(' Fetching from {:s}'.format(repo.remote().url))
+                repo.remote().fetch()
+            repo.head.reset(self._model.version, working_tree=True)
+
         self._ctx._state.update(dependencies={
             self._model.name: self._model.state(location=os.path.relpath(loc, self._ctx._path), driver='git')
         })
 
     def unpack(self, mgr, locations):
         for l in locations:
             if l['source'][0] == '/':
```

### Comparing `sourceknight-0.2/sourceknight/drivers/tar.py` & `sourceknight-0.3/sourceknight/drivers/tar.py`

 * *Files identical despite different names*

### Comparing `sourceknight-0.2/sourceknight/main.py` & `sourceknight-0.3/sourceknight/main.py`

 * *Files identical despite different names*

### Comparing `sourceknight-0.2/sourceknight/state.py` & `sourceknight-0.3/sourceknight/state.py`

 * *Files identical despite different names*

### Comparing `sourceknight-0.2/sourceknight/status.py` & `sourceknight-0.3/sourceknight/status.py`

 * *Files identical despite different names*

### Comparing `sourceknight-0.2/sourceknight/unpack.py` & `sourceknight-0.3/sourceknight/unpack.py`

 * *Files identical despite different names*

### Comparing `sourceknight-0.2/sourceknight/update.py` & `sourceknight-0.3/sourceknight/update.py`

 * *Files identical despite different names*

### Comparing `sourceknight-0.2/sourceknight/utils.py` & `sourceknight-0.3/sourceknight/utils.py`

 * *Files identical despite different names*

### Comparing `sourceknight-0.2/sourceknight.egg-info/PKG-INFO` & `sourceknight-0.3/sourceknight.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sourceknight
-Version: 0.2
+Version: 0.3
 Summary: simple dependency manager for sourcemod projects
 Home-page: https://github.com/tmick0/sourceknight
 Author: travis mick
 Author-email: root@lo.calho.st
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -29,22 +29,22 @@
 
 The core concept of `sourceknight` is the *project*, which encapsulates any plugins you're trying to build and their dependencies (including sourcemod itself).
 
 A *project directory* will include a *project file* called `sourceknight.yaml` that defines all the parameters of your project, including its name,
 its dependencies, and the plugins it will build. The project file is written in [YAML](https://en.wikipedia.org/wiki/YAML).
 
 If building your own plugin, your project directory will likely also include any sourcepawn files you need, but this is optional --
-you can also also use `sourcepawn` just to simplify compiling a collection of third party plugins by declaring them as dependencies.
+you can also also use `sourceknight` just to simplify compiling a collection of third party plugins by declaring them as dependencies.
 
 A minimal `sourceknight.yaml` might look something like this:
 
 ```yaml
 project:
   name: myplugin-example
-  sourceknight: 0.2
+  sourceknight: 0.3
   dependencies:
     - name: sourcemod
       type: tar
       version: 1.10.0-git6503
       location: https://sm.alliedmods.net/smdrop/1.10/sourcemod-1.10.0-git6503-linux.tar.gz
       unpack:
       - source: /addons
@@ -76,14 +76,15 @@
 
 - `location`: URL to download the tar file from
 - Optional: `version`, which can be manually specified to help prevent re-downloading the same file unnecessarily
 
 **`git`:**
 
 - `repo`: Git repository URL to clone
+- Optional: `version`, a commit tag or branch to checkout instead of the default
 
 Both of these types of dependencies must have an `unpack` block, which tells us which files to copy out of them and where they belong relative to the `sourceknight` *build root*. The build root is a hidden directory maintained by `sourceknight` which will contain the entire sourcemod tree (i.e., it will contain the `addons` directory) as well as any other dependencies and sources specified by your project.
 
 In the example above, the `unpack` declaration for `sourcemod` says to unpack the `/addons` directory to `/addons`. In sourcemod's case, this means we're copying the entire contents of the archive. However, the [extended example project file](example/sourceknight.yaml) includes other examples of unpack declarations. Note that the destination of an unpack operation is always relative to the build tree. Multiple `source`, `dest` pairs can be specified in the `unpack` section if needed.
 
 ### Build specification
```

### Comparing `sourceknight-0.2/sourceknight.egg-info/SOURCES.txt` & `sourceknight-0.3/sourceknight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

