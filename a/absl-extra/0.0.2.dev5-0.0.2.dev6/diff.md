# Comparing `tmp/absl_extra-0.0.2.dev5.tar.gz` & `tmp/absl_extra-0.0.2.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absl_extra-0.0.2.dev5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "absl_extra-0.0.2.dev6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `absl_extra-0.0.2.dev5.tar` & `absl_extra-0.0.2.dev6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1588 2023-07-01 14:58:11.054847 absl_extra-0.0.2.dev5/Readme.md
--rw-r--r--   0        0        0      646 2023-07-01 14:58:11.058847 absl_extra-0.0.2.dev5/absl_extra/__init__.py
--rw-r--r--   0        0        0       64 2023-07-01 14:58:11.058847 absl_extra-0.0.2.dev5/absl_extra/py.typed
--rw-r--r--   0        0        0        0 2023-07-01 14:58:11.058847 absl_extra-0.0.2.dev5/absl_extra/src/__init__.py
--rw-r--r--   0        0        0     1202 2023-07-01 14:58:11.058847 absl_extra-0.0.2.dev5/absl_extra/src/jax_utils.py
--rw-r--r--   0        0        0     2061 2023-07-01 14:58:11.058847 absl_extra-0.0.2.dev5/absl_extra/src/logging_utils.py
--rw-r--r--   0        0        0     2487 2023-07-01 14:58:11.058847 absl_extra-0.0.2.dev5/absl_extra/src/notifier.py
--rw-r--r--   0        0        0     4277 2023-07-01 14:58:11.058847 absl_extra-0.0.2.dev5/absl_extra/src/tasks.py
--rw-r--r--   0        0        0     4522 2023-07-01 14:58:11.058847 absl_extra-0.0.2.dev5/absl_extra/src/tf_utils.py
--rw-r--r--   0        0        0      914 2023-07-01 14:58:11.058847 absl_extra-0.0.2.dev5/pyproject.toml
--rw-r--r--   0        0        0     2693 1970-01-01 00:00:00.000000 absl_extra-0.0.2.dev5/PKG-INFO
+-rw-r--r--   0        0        0     1588 2023-07-01 17:34:16.831045 absl_extra-0.0.2.dev6/Readme.md
+-rw-r--r--   0        0        0      646 2023-07-01 17:34:16.831045 absl_extra-0.0.2.dev6/absl_extra/__init__.py
+-rw-r--r--   0        0        0       64 2023-07-01 17:34:16.831045 absl_extra-0.0.2.dev6/absl_extra/py.typed
+-rw-r--r--   0        0        0        0 2023-07-01 17:34:16.831045 absl_extra-0.0.2.dev6/absl_extra/src/__init__.py
+-rw-r--r--   0        0        0     1202 2023-07-01 17:34:16.831045 absl_extra-0.0.2.dev6/absl_extra/src/jax_utils.py
+-rw-r--r--   0        0        0     2061 2023-07-01 17:34:16.831045 absl_extra-0.0.2.dev6/absl_extra/src/logging_utils.py
+-rw-r--r--   0        0        0     2487 2023-07-01 17:34:16.831045 absl_extra-0.0.2.dev6/absl_extra/src/notifier.py
+-rw-r--r--   0        0        0     4281 2023-07-01 17:34:16.831045 absl_extra-0.0.2.dev6/absl_extra/src/tasks.py
+-rw-r--r--   0        0        0     4522 2023-07-01 17:34:16.831045 absl_extra-0.0.2.dev6/absl_extra/src/tf_utils.py
+-rw-r--r--   0        0        0      914 2023-07-01 17:34:16.831045 absl_extra-0.0.2.dev6/pyproject.toml
+-rw-r--r--   0        0        0     2693 1970-01-01 00:00:00.000000 absl_extra-0.0.2.dev6/PKG-INFO
```

### Comparing `absl_extra-0.0.2.dev5/Readme.md` & `absl_extra-0.0.2.dev6/Readme.md`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.2.dev5/absl_extra/__init__.py` & `absl_extra-0.0.2.dev6/absl_extra/__init__.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.2.dev5/absl_extra/src/jax_utils.py` & `absl_extra-0.0.2.dev6/absl_extra/src/jax_utils.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.2.dev5/absl_extra/src/logging_utils.py` & `absl_extra-0.0.2.dev6/absl_extra/src/logging_utils.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.2.dev5/absl_extra/src/notifier.py` & `absl_extra-0.0.2.dev6/absl_extra/src/notifier.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.2.dev5/absl_extra/src/tasks.py` & `absl_extra-0.0.2.dev6/absl_extra/src/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
         kwargs = {}
 
         if util.find_spec("ml_collections") and config_file is not None:
             config = config_flags.DEFINE_config_file("config", default=config_file)
             config = config.value
             logging.info(
-                f"Config: {json.dumps(dict(config), sort_keys=True, indent=4)}"
+                f"Config: {json.dumps(config.to_dict(), sort_keys=True, indent=4)}"
             )
             kwargs["config"] = config
         logging.info("-" * 50)
         if db is not None:
             kwargs["db"] = db
         notifier.notify_job_started(f"{app_name}.{task_name}")
         ret_val = task.fn(cmd, **kwargs)
```

### Comparing `absl_extra-0.0.2.dev5/absl_extra/src/tf_utils.py` & `absl_extra-0.0.2.dev6/absl_extra/src/tf_utils.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.2.dev5/pyproject.toml` & `absl_extra-0.0.2.dev6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "absl_extra"
-version = "0.0.2dev5"
+version = "0.0.2dev6"
 description = "A wrapper to run and monitor absl app."
 readme = "Readme.md"
 requires-python = ">=3.8"
 authors = [
     { name = "Artem Sereda", email = "artem.sereda.tub@gmail.com" }
 ]
 maintainers = [
```

### Comparing `absl_extra-0.0.2.dev5/PKG-INFO` & `absl_extra-0.0.2.dev6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absl_extra
-Version: 0.0.2.dev5
+Version: 0.0.2.dev6
 Summary: A wrapper to run and monitor absl app.
 Author-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Maintainer-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Requires-Dist: absl_py
```

