# Comparing `tmp/container_helpers-0.0.4.tar.gz` & `tmp/container_helpers-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "container_helpers-0.0.4.tar", max compression
+gzip compressed data, was "container_helpers-0.0.5.tar", max compression
```

## Comparing `container_helpers-0.0.4.tar` & `container_helpers-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2023-07-01 01:12:22.465664 container_helpers-0.0.4/LICENSE
--rw-r--r--   0        0        0      438 2023-07-01 01:12:22.465664 container_helpers-0.0.4/containers/__init__.py
--rw-r--r--   0        0        0     1237 2023-07-01 01:12:22.465664 container_helpers-0.0.4/containers/data_types.py
--rw-r--r--   0        0        0        0 2023-07-01 01:12:22.465664 container_helpers-0.0.4/containers/providers/__init__.py
--rw-r--r--   0        0        0      190 2023-07-01 01:12:22.465664 container_helpers-0.0.4/containers/providers/base.py
--rw-r--r--   0        0        0      773 2023-07-01 01:12:22.465664 container_helpers-0.0.4/containers/providers/helpers.py
--rw-r--r--   0        0        0     5119 2023-07-01 01:12:22.465664 container_helpers-0.0.4/containers/providers/podman.py
--rw-r--r--   0        0        0      388 2023-07-01 01:12:22.465664 container_helpers-0.0.4/containers/services/__init__.py
--rw-r--r--   0        0        0     2720 2023-07-01 01:12:22.465664 container_helpers-0.0.4/containers/services/base.py
--rw-r--r--   0        0        0     4474 2023-07-01 01:12:22.465664 container_helpers-0.0.4/containers/services/windows.py
--rw-r--r--   0        0        0      568 2023-07-01 01:12:22.465664 container_helpers-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 container_helpers-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-01 06:46:17.196872 container_helpers-0.0.5/LICENSE
+-rw-r--r--   0        0        0      438 2023-07-01 06:46:17.196872 container_helpers-0.0.5/containers/__init__.py
+-rw-r--r--   0        0        0     1237 2023-07-01 06:46:17.196872 container_helpers-0.0.5/containers/data_types.py
+-rw-r--r--   0        0        0        0 2023-07-01 06:46:17.196872 container_helpers-0.0.5/containers/providers/__init__.py
+-rw-r--r--   0        0        0      190 2023-07-01 06:46:17.196872 container_helpers-0.0.5/containers/providers/base.py
+-rw-r--r--   0        0        0      773 2023-07-01 06:46:17.196872 container_helpers-0.0.5/containers/providers/helpers.py
+-rw-r--r--   0        0        0     5119 2023-07-01 06:46:17.196872 container_helpers-0.0.5/containers/providers/podman.py
+-rw-r--r--   0        0        0      388 2023-07-01 06:46:17.196872 container_helpers-0.0.5/containers/services/__init__.py
+-rw-r--r--   0        0        0     2720 2023-07-01 06:46:17.196872 container_helpers-0.0.5/containers/services/base.py
+-rw-r--r--   0        0        0     4470 2023-07-01 06:46:17.200872 container_helpers-0.0.5/containers/services/windows.py
+-rw-r--r--   0        0        0      568 2023-07-01 06:46:17.200872 container_helpers-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 container_helpers-0.0.5/PKG-INFO
```

### Comparing `container_helpers-0.0.4/LICENSE` & `container_helpers-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `container_helpers-0.0.4/containers/data_types.py` & `container_helpers-0.0.5/containers/data_types.py`

 * *Files identical despite different names*

### Comparing `container_helpers-0.0.4/containers/providers/helpers.py` & `container_helpers-0.0.5/containers/providers/helpers.py`

 * *Files identical despite different names*

### Comparing `container_helpers-0.0.4/containers/providers/podman.py` & `container_helpers-0.0.5/containers/providers/podman.py`

 * *Files identical despite different names*

### Comparing `container_helpers-0.0.4/containers/services/base.py` & `container_helpers-0.0.5/containers/services/base.py`

 * *Files identical despite different names*

### Comparing `container_helpers-0.0.4/containers/services/windows.py` & `container_helpers-0.0.5/containers/services/windows.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,38 +9,38 @@
 from ..data_types import BindMount
 from ..data_types import Container
 from ..data_types import Mount
 from ..data_types import PathType
 from .base import ContainersService
 
 
-def _to_wsl_path(path: pathlib.Path):
+def to_wsl_path(path: pathlib.Path):
     if not isinstance(path, pathlib.WindowsPath):
         raise ValueError(f"Expected windows path but got {path.__class__} instead")
     new_path = pathlib.Path(path)
     if new_path.drive == "":
         return new_path.as_posix()
     _, *parts = new_path.parts
     return str(
         pathlib.PurePosixPath("/mnt", new_path.drive.rstrip(":").lower(), *parts)
     )
 
 
-def _is_unc_path(path: PathType) -> bool:
+def is_unc_path(path: PathType) -> bool:
     path = pathlib.Path(path)
     return path.drive.startswith("\\")
 
 
 class WindowsContainersService(ContainersService):
     @contextlib.asynccontextmanager
     async def _make_temp_copy(
         self, src: typing.Optional[pathlib.Path], suffix: typing.Optional[str] = None
     ) -> typing.AsyncContextManager[pathlib.Path]:
         # Only copy if the drive is provided and a UNC path
-        if src is not None and _is_unc_path(src):
+        if src is not None and is_unc_path(src):
             with (
                 open(src, "rb") as src_file,
                 tempfile.NamedTemporaryFile(suffix=suffix) as temp_file,
             ):
                 self.logger.debug(
                     "Make a temp copy of seccomp profile from %s to native windows filesystem at %s",
                     src,
@@ -59,27 +59,28 @@
     ) -> typing.AsyncContextManager[typing.List[Mount]]:
         with tempfile.TemporaryDirectory() as temp_folder:
             temp_folder_path = pathlib.Path(temp_folder)
             new_mounts = []
             for i, mount in enumerate(mounts):
                 if (
                     not isinstance(mount, BindMount)
-                    or not _is_unc_path(mount.source)
+                    or not is_unc_path(mount.source)
                     or not mount.readonly
                 ):
                     new_mounts.append(mount)
                     continue
                 new_source = temp_folder_path / f"mount-{i}"
                 self.logger.info(
                     "Copy readonly UNC mount from %s to %s", mount.source, new_source
                 )
                 shutil.copytree(mount.source, new_source)
                 mount.source = new_source
                 new_mounts.append(mount)
             yield new_mounts
+
     @contextlib.asynccontextmanager
     async def run(
         self,
         container: Container,
         stdin: typing.Optional[int] = None,
         stdout: typing.Optional[int] = None,
         stderr: typing.Optional[int] = None,
@@ -105,11 +106,11 @@
             self._copy_readonly_unc_mounts(container.mounts) as new_mounts,
         ):
             if temp_seccomp_profile is not None:
                 # Not only we need to copy to native window filesystem, we also
                 # need to convert it into WSL path for podman in the podman WSL machine
                 # to read
                 # ref: https://github.com/containers/podman/issues/14494
-                container.security_options.seccomp = _to_wsl_path(temp_seccomp_profile)
+                container.security_options.seccomp = to_wsl_path(temp_seccomp_profile)
             container.mounts = new_mounts
             async with super().run(container, stdin, stdout, stderr, log_level) as proc:
                 yield proc
```

### Comparing `container_helpers-0.0.4/pyproject.toml` & `container_helpers-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "container-helpers"
-version = "0.0.4"
+version = "0.0.5"
 description = "Helpers for running docker or podman containers easily in Python"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 repository = "https://github.com/LaunchPlatform/container-helpers"
 packages = [{include = "containers"}]
 
 [tool.poetry.dependencies]
```

### Comparing `container_helpers-0.0.4/PKG-INFO` & `container_helpers-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: container-helpers
-Version: 0.0.4
+Version: 0.0.5
 Summary: Helpers for running docker or podman containers easily in Python
 Home-page: https://github.com/LaunchPlatform/container-helpers
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

