# Comparing `tmp/container_helpers-0.0.1.tar.gz` & `tmp/container_helpers-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "container_helpers-0.0.1.tar", max compression
+gzip compressed data, was "container_helpers-0.0.3.tar", max compression
```

## Comparing `container_helpers-0.0.1.tar` & `container_helpers-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2023-06-30 22:02:31.816520 container_helpers-0.0.1/LICENSE
--rw-r--r--   0        0        0      438 2023-06-30 22:34:17.308061 container_helpers-0.0.1/containers/__init__.py
--rw-r--r--   0        0        0     1237 2023-06-30 22:36:47.312658 container_helpers-0.0.1/containers/data_types.py
--rw-r--r--   0        0        0        0 2023-06-30 22:34:17.328061 container_helpers-0.0.1/containers/providers/__init__.py
--rw-r--r--   0        0        0      190 2023-06-30 22:34:17.338061 container_helpers-0.0.1/containers/providers/base.py
--rw-r--r--   0        0        0      773 2023-06-30 22:34:17.348062 container_helpers-0.0.1/containers/providers/helpers.py
--rw-r--r--   0        0        0     5119 2023-06-30 22:34:17.358062 container_helpers-0.0.1/containers/providers/podman.py
--rw-r--r--   0        0        0      253 2023-06-30 22:34:17.368062 container_helpers-0.0.1/containers/services/__init__.py
--rw-r--r--   0        0        0     2537 2023-06-30 22:57:25.249947 container_helpers-0.0.1/containers/services/base.py
--rw-r--r--   0        0        0     4474 2023-06-30 22:34:17.378062 container_helpers-0.0.1/containers/services/windows.py
--rw-r--r--   0        0        0      568 2023-06-30 23:26:58.694482 container_helpers-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 container_helpers-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-01 00:38:21.685644 container_helpers-0.0.3/LICENSE
+-rw-r--r--   0        0        0      438 2023-07-01 00:38:21.685644 container_helpers-0.0.3/containers/__init__.py
+-rw-r--r--   0        0        0     1237 2023-07-01 00:38:21.685644 container_helpers-0.0.3/containers/data_types.py
+-rw-r--r--   0        0        0        0 2023-07-01 00:38:21.685644 container_helpers-0.0.3/containers/providers/__init__.py
+-rw-r--r--   0        0        0      190 2023-07-01 00:38:21.685644 container_helpers-0.0.3/containers/providers/base.py
+-rw-r--r--   0        0        0      773 2023-07-01 00:38:21.685644 container_helpers-0.0.3/containers/providers/helpers.py
+-rw-r--r--   0        0        0     5119 2023-07-01 00:38:21.685644 container_helpers-0.0.3/containers/providers/podman.py
+-rw-r--r--   0        0        0      253 2023-07-01 00:38:21.685644 container_helpers-0.0.3/containers/services/__init__.py
+-rw-r--r--   0        0        0     2556 2023-07-01 00:38:21.685644 container_helpers-0.0.3/containers/services/base.py
+-rw-r--r--   0        0        0     4474 2023-07-01 00:38:21.685644 container_helpers-0.0.3/containers/services/windows.py
+-rw-r--r--   0        0        0      568 2023-07-01 00:38:21.685644 container_helpers-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 container_helpers-0.0.3/PKG-INFO
```

### Comparing `container_helpers-0.0.1/LICENSE` & `container_helpers-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `container_helpers-0.0.1/containers/data_types.py` & `container_helpers-0.0.3/containers/data_types.py`

 * *Files identical despite different names*

### Comparing `container_helpers-0.0.1/containers/providers/helpers.py` & `container_helpers-0.0.3/containers/providers/helpers.py`

 * *Files identical despite different names*

### Comparing `container_helpers-0.0.1/containers/providers/podman.py` & `container_helpers-0.0.3/containers/providers/podman.py`

 * *Files identical despite different names*

### Comparing `container_helpers-0.0.1/containers/services/base.py` & `container_helpers-0.0.3/containers/services/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,18 +58,20 @@
     @contextlib.asynccontextmanager
     async def run(
         self,
         container: Container,
         stdin: typing.Optional[int] = None,
         stdout: typing.Optional[int] = None,
         stderr: typing.Optional[int] = None,
-        log_level: typing.Optional[str] = "debug",
+        log_level: typing.Optional[str] = None,
     ) -> typing.AsyncContextManager[asyncio.subprocess.Process]:
         command = self.podman.build_command(container, log_level=log_level)
-        self.logger.info("Run container with command: %s", " ".join(map(shlex.quote, command)))
+        self.logger.info(
+            "Run container with command: %s", " ".join(map(shlex.quote, command))
+        )
         proc = await asyncio.create_subprocess_exec(
             *command,
             stdin=stdin,
             stdout=stdout,
             stderr=stderr,
         )
         yield proc
```

### Comparing `container_helpers-0.0.1/containers/services/windows.py` & `container_helpers-0.0.3/containers/services/windows.py`

 * *Files identical despite different names*

### Comparing `container_helpers-0.0.1/pyproject.toml` & `container_helpers-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "container-helpers"
-version = "0.0.1"
+version = "0.0.3"
 description = "Helpers for running docker or podman containers easily in Python"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 repository = "https://github.com/LaunchPlatform/container-helpers"
 packages = [{include = "containers"}]
 
 [tool.poetry.dependencies]
```

### Comparing `container_helpers-0.0.1/PKG-INFO` & `container_helpers-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: container-helpers
-Version: 0.0.1
+Version: 0.0.3
 Summary: Helpers for running docker or podman containers easily in Python
 Home-page: https://github.com/LaunchPlatform/container-helpers
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

