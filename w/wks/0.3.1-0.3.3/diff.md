# Comparing `tmp/wks-0.3.1.tar.gz` & `tmp/wks-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wks-0.3.1.tar", last modified: Sat Jul  1 14:36:09 2023, max compression
+gzip compressed data, was "wks-0.3.3.tar", last modified: Sat Jul  1 14:46:30 2023, max compression
```

## Comparing `wks-0.3.1.tar` & `wks-0.3.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-07-01 14:36:09.072088 wks-0.3.1/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2823 2023-07-01 14:36:09.072088 wks-0.3.1/PKG-INFO
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2480 2023-05-14 09:17:40.000000 wks-0.3.1/README.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       38 2023-07-01 14:36:09.072088 wks-0.3.1/setup.cfg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      625 2023-07-01 14:35:24.000000 wks-0.3.1/setup.py
--rwxrwxr-x   0 gregwar   (1000) gregwar   (1000)      592 2022-09-26 20:46:36.000000 wks-0.3.1/wks
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-07-01 14:36:09.072088 wks-0.3.1/wks.egg-info/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2823 2023-07-01 14:36:09.000000 wks-0.3.1/wks.egg-info/PKG-INFO
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      516 2023-07-01 14:36:09.000000 wks-0.3.1/wks.egg-info/SOURCES.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        1 2023-07-01 14:36:09.000000 wks-0.3.1/wks.egg-info/dependency_links.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       16 2023-07-01 14:36:09.000000 wks-0.3.1/wks.egg-info/requires.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       10 2023-07-01 14:36:09.000000 wks-0.3.1/wks.egg-info/top_level.txt
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-07-01 14:36:09.072088 wks-0.3.1/workspace/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       20 2022-09-26 20:46:36.000000 wks-0.3.1/workspace/__init__.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4412 2023-05-14 09:16:16.000000 wks-0.3.1/workspace/cmake.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      914 2022-09-26 20:46:36.000000 wks-0.3.1/workspace/command_build.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      608 2023-06-23 13:31:36.000000 wks-0.3.1/workspace/command_clean.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      178 2022-09-26 20:46:36.000000 wks-0.3.1/workspace/command_cmake.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      376 2022-09-26 20:46:36.000000 wks-0.3.1/workspace/command_cmd.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1147 2022-09-26 20:46:36.000000 wks-0.3.1/workspace/command_graph.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      716 2022-09-26 20:46:36.000000 wks-0.3.1/workspace/command_help.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      422 2022-09-26 20:46:36.000000 wks-0.3.1/workspace/command_install.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      313 2022-09-26 20:46:36.000000 wks-0.3.1/workspace/command_pull.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1760 2022-09-26 20:46:36.000000 wks-0.3.1/workspace/command_status.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      397 2023-06-23 13:29:46.000000 wks-0.3.1/workspace/commands.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      297 2022-09-26 20:46:36.000000 wks-0.3.1/workspace/env.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5747 2023-07-01 14:35:08.000000 wks-0.3.1/workspace/git.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      620 2022-09-26 20:46:36.000000 wks-0.3.1/workspace/message.py
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-07-01 14:46:30.776096 wks-0.3.3/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2823 2023-07-01 14:46:30.776096 wks-0.3.3/PKG-INFO
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2480 2023-05-14 09:17:40.000000 wks-0.3.3/README.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       38 2023-07-01 14:46:30.776096 wks-0.3.3/setup.cfg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      625 2023-07-01 14:46:11.000000 wks-0.3.3/setup.py
+-rwxrwxr-x   0 gregwar   (1000) gregwar   (1000)      592 2022-09-26 20:46:36.000000 wks-0.3.3/wks
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-07-01 14:46:30.776096 wks-0.3.3/wks.egg-info/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2823 2023-07-01 14:46:30.000000 wks-0.3.3/wks.egg-info/PKG-INFO
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      516 2023-07-01 14:46:30.000000 wks-0.3.3/wks.egg-info/SOURCES.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        1 2023-07-01 14:46:30.000000 wks-0.3.3/wks.egg-info/dependency_links.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       16 2023-07-01 14:46:30.000000 wks-0.3.3/wks.egg-info/requires.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       10 2023-07-01 14:46:30.000000 wks-0.3.3/wks.egg-info/top_level.txt
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-07-01 14:46:30.776096 wks-0.3.3/workspace/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       20 2022-09-26 20:46:36.000000 wks-0.3.3/workspace/__init__.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4412 2023-05-14 09:16:16.000000 wks-0.3.3/workspace/cmake.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      914 2022-09-26 20:46:36.000000 wks-0.3.3/workspace/command_build.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      608 2023-06-23 13:31:36.000000 wks-0.3.3/workspace/command_clean.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      178 2022-09-26 20:46:36.000000 wks-0.3.3/workspace/command_cmake.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      376 2022-09-26 20:46:36.000000 wks-0.3.3/workspace/command_cmd.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1147 2022-09-26 20:46:36.000000 wks-0.3.3/workspace/command_graph.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      716 2022-09-26 20:46:36.000000 wks-0.3.3/workspace/command_help.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      422 2022-09-26 20:46:36.000000 wks-0.3.3/workspace/command_install.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      313 2022-09-26 20:46:36.000000 wks-0.3.3/workspace/command_pull.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1760 2022-09-26 20:46:36.000000 wks-0.3.3/workspace/command_status.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      397 2023-06-23 13:29:46.000000 wks-0.3.3/workspace/commands.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      297 2022-09-26 20:46:36.000000 wks-0.3.3/workspace/env.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6172 2023-07-01 14:45:54.000000 wks-0.3.3/workspace/git.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      620 2022-09-26 20:46:36.000000 wks-0.3.3/workspace/message.py
```

### Comparing `wks-0.3.1/PKG-INFO` & `wks-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wks
-Version: 0.3.1
+Version: 0.3.3
 Summary: Simple dependencies manager for cmake projects in your workspace
 Home-page: https://github.com/rhoban/wks/
 Author: Rhoban team
 Author-email: team@rhoban.com
 License: UNKNOWN
 Keywords: wks workspace deps
 Platform: UNKNOWN
```

### Comparing `wks-0.3.1/README.md` & `wks-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `wks-0.3.1/setup.py` & `wks-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="wks",
-    version="0.3.1",
+    version="0.3.3",
     author="Rhoban team",
     author_email="team@rhoban.com",
     description="Simple dependencies manager for cmake projects in your workspace",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rhoban/wks/",
     packages=setuptools.find_packages(),
```

### Comparing `wks-0.3.1/wks` & `wks-0.3.3/wks`

 * *Files identical despite different names*

### Comparing `wks-0.3.1/wks.egg-info/PKG-INFO` & `wks-0.3.3/wks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wks
-Version: 0.3.1
+Version: 0.3.3
 Summary: Simple dependencies manager for cmake projects in your workspace
 Home-page: https://github.com/rhoban/wks/
 Author: Rhoban team
 Author-email: team@rhoban.com
 License: UNKNOWN
 Keywords: wks workspace deps
 Platform: UNKNOWN
```

### Comparing `wks-0.3.1/wks.egg-info/SOURCES.txt` & `wks-0.3.3/wks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wks-0.3.1/workspace/cmake.py` & `wks-0.3.3/workspace/cmake.py`

 * *Files identical despite different names*

### Comparing `wks-0.3.1/workspace/command_build.py` & `wks-0.3.3/workspace/command_build.py`

 * *Files identical despite different names*

### Comparing `wks-0.3.1/workspace/command_clean.py` & `wks-0.3.3/workspace/command_clean.py`

 * *Files identical despite different names*

### Comparing `wks-0.3.1/workspace/command_graph.py` & `wks-0.3.3/workspace/command_graph.py`

 * *Files identical despite different names*

### Comparing `wks-0.3.1/workspace/command_help.py` & `wks-0.3.3/workspace/command_help.py`

 * *Files identical despite different names*

### Comparing `wks-0.3.1/workspace/command_status.py` & `wks-0.3.3/workspace/command_status.py`

 * *Files identical despite different names*

### Comparing `wks-0.3.1/workspace/git.py` & `wks-0.3.3/workspace/git.py`

 * *Files 5% similar despite different names*

```diff
@@ -122,45 +122,58 @@
             if scan_dependencies(directory):
                 changed = True
 
 
 def global_command(command, vendor_filter=None):
     message.bright("* Running global command: %s" % command)
 
-    use_threads = os.getenv('WKS_NO_THREADS') is None
+    use_threads = os.getenv("WKS_NO_THREADS") is None
     directories = get_directories()
 
     threads: list[threading.Thread] = [None] * len(directories)
     processes: list[subprocess.CompletedProcess] = threads.copy()
+    has_error: bool = False
 
     def thread_func(index: int, dir: str, cmd: str):
         processes[index] = subprocess.run(cmd.split(), stdout=subprocess.PIPE, stderr=subprocess.STDOUT, cwd=dir)
 
+    def show_output(process):
+        if process.returncode != 0:
+            print(message.error(process.stdout.decode()))
+        else:
+            print(process.stdout.decode())
+
     for index, directory in enumerate(directories):
         if vendor_filter is not None:
             parts = directory.split("/")
             vendor = parts[-2]
             if vendor.lower() != vendor_filter.lower():
                 continue
 
         if use_threads:
             threads[index] = threading.Thread(None, thread_func, args=(index, directory, command))
             threads[index].start()
         else:
             message.bright("> %s" % directory)
             thread_func(index, directory, command)
-            print(processes[index].stdout.decode())
+            show_output(processes[index])
+            if processes[index].returncode != 0:
+                has_error = True
 
     if use_threads:
         for index, directory in enumerate(directories):
             threads[index].join()
             message.bright("- In %s ..." % os.path.realpath(directory))
-            print(processes[index].stdout.decode())
+            show_output(processes[index])
+            if processes[index].returncode != 0:
+                has_error = True
 
     print("")
+    if has_error:
+        print(message.error("Some commands failed"))
 
 
 def status(directory):
     output = subprocess.getoutput("cd %s; git status --porcelain=v1" % directory)
     return output
```

### Comparing `wks-0.3.1/workspace/message.py` & `wks-0.3.3/workspace/message.py`

 * *Files identical despite different names*

