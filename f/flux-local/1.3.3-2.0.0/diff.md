# Comparing `tmp/flux-local-1.3.3.tar.gz` & `tmp/flux-local-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-local-1.3.3.tar", last modified: Fri Jun 30 03:59:07 2023, max compression
+gzip compressed data, was "flux-local-2.0.0.tar", last modified: Sat Jul  1 18:49:40 2023, max compression
```

## Comparing `flux-local-1.3.3.tar` & `flux-local-2.0.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:07.250721 flux-local-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 03:58:57.000000 flux-local-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-06-30 03:59:07.250721 flux-local-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-06-30 03:58:57.000000 flux-local-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:07.250721 flux-local-1.3.3/flux_local/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-30 03:58:57.000000 flux-local-1.3.3/flux_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-30 03:58:57.000000 flux-local-1.3.3/flux_local/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-30 03:58:57.000000 flux-local-1.3.3/flux_local/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25824 2023-06-30 03:58:57.000000 flux-local-1.3.3/flux_local/git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-06-30 03:58:57.000000 flux-local-1.3.3/flux_local/helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-06-30 03:58:57.000000 flux-local-1.3.3/flux_local/kustomize.py
--rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-06-30 03:58:57.000000 flux-local-1.3.3/flux_local/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:07.250721 flux-local-1.3.3/flux_local/tool/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-30 03:58:57.000000 flux-local-1.3.3/flux_local/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-30 03:58:57.000000 flux-local-1.3.3/flux_local/tool/build.py
--rw-r--r--   0 runner    (1001) docker     (123)    16262 2023-06-30 03:58:57.000000 flux-local-1.3.3/flux_local/tool/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-30 03:58:57.000000 flux-local-1.3.3/flux_local/tool/flux_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-30 03:58:57.000000 flux-local-1.3.3/flux_local/tool/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-06-30 03:58:57.000000 flux-local-1.3.3/flux_local/tool/get.py
--rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-06-30 03:58:57.000000 flux-local-1.3.3/flux_local/tool/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-06-30 03:58:57.000000 flux-local-1.3.3/flux_local/tool/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-06-30 03:58:57.000000 flux-local-1.3.3/flux_local/tool/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:07.250721 flux-local-1.3.3/flux_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-06-30 03:59:07.000000 flux-local-1.3.3/flux_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-30 03:59:07.000000 flux-local-1.3.3/flux_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 03:59:07.000000 flux-local-1.3.3/flux_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-30 03:59:07.000000 flux-local-1.3.3/flux_local.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-30 03:59:07.000000 flux-local-1.3.3/flux_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-30 03:59:07.000000 flux-local-1.3.3/flux_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-30 03:59:07.250721 flux-local-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-30 03:58:57.000000 flux-local-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:59:07.250721 flux-local-1.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-30 03:58:57.000000 flux-local-1.3.3/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-06-30 03:58:57.000000 flux-local-1.3.3/tests/test_git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-30 03:58:57.000000 flux-local-1.3.3/tests/test_helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-06-30 03:58:57.000000 flux-local-1.3.3/tests/test_kustomize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-06-30 03:58:57.000000 flux-local-1.3.3/tests/test_manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:49:40.254690 flux-local-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-01 18:49:30.000000 flux-local-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-07-01 18:49:40.254690 flux-local-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-07-01 18:49:30.000000 flux-local-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:49:40.250690 flux-local-2.0.0/flux_local/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25824 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/kustomize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:49:40.254690 flux-local-2.0.0/flux_local/tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/tool/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/tool/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/tool/flux_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/tool/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/tool/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/tool/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14191 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/tool/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-07-01 18:49:30.000000 flux-local-2.0.0/flux_local/tool/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:49:40.250690 flux-local-2.0.0/flux_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-07-01 18:49:40.000000 flux-local-2.0.0/flux_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-01 18:49:40.000000 flux-local-2.0.0/flux_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 18:49:40.000000 flux-local-2.0.0/flux_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-01 18:49:40.000000 flux-local-2.0.0/flux_local.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-01 18:49:40.000000 flux-local-2.0.0/flux_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-01 18:49:40.000000 flux-local-2.0.0/flux_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-01 18:49:40.254690 flux-local-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-01 18:49:30.000000 flux-local-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:49:40.254690 flux-local-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-01 18:49:30.000000 flux-local-2.0.0/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-07-01 18:49:30.000000 flux-local-2.0.0/tests/test_git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-01 18:49:30.000000 flux-local-2.0.0/tests/test_helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-01 18:49:30.000000 flux-local-2.0.0/tests/test_kustomize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-07-01 18:49:30.000000 flux-local-2.0.0/tests/test_manifest.py
```

### Comparing `flux-local-1.3.3/LICENSE` & `flux-local-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.3/PKG-INFO` & `flux-local-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-local
-Version: 1.3.3
+Version: 2.0.0
 Summary: flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 Home-page: https://github.com/allenporter/flux-local
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
```

### Comparing `flux-local-1.3.3/README.md` & `flux-local-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.3/flux_local/command.py` & `flux-local-2.0.0/flux_local/command.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.3/flux_local/exceptions.py` & `flux-local-2.0.0/flux_local/exceptions.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.3/flux_local/git_repo.py` & `flux-local-2.0.0/flux_local/git_repo.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.3/flux_local/helm.py` & `flux-local-2.0.0/flux_local/helm.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,38 +21,38 @@
 Then to actually instantiate a template from a HelmRelease:
 ```python
 from flux_local.manifest import HelmRelease
 
 releases = await kustomize.grep("kind=^HelmRelease$").objects()
 if not len(releases) == 1:
     raise ValueError("Expected only one HelmRelease")
-tmpl = helm.template(
-    HelmRelease.parse_doc(releases[0]),
-    releases[0]["spec"].get("values"))
+tmpl = helm.template(HelmRelease.parse_doc(releases[0]))
 objects = await tmpl.objects()
 for object in objects:
     print(f"Found object {object['apiVersion']} {object['kind']}")
 ```
 """
 
 import datetime
+from dataclasses import dataclass
 import logging
 from pathlib import Path
 from typing import Any
 
 import aiofiles
 import yaml
 
 from . import command
 from .kustomize import Kustomize
 from .manifest import HelmRelease, HelmRepository, CRD_KIND, SECRET_KIND, REPO_TYPE_OCI
 from .exceptions import HelmException
 
 __all__ = [
     "Helm",
+    "Options",
 ]
 
 _LOGGER = logging.getLogger(__name__)
 
 
 HELM_BIN = "helm"
 
@@ -84,14 +84,62 @@
                     "url": repo.url,
                 }
                 for repo in self._repos
             ],
         }
 
 
+@dataclass
+class Options:
+    """Options to use when inflating a Helm chart.
+
+    Internally, these translate into either command line flags or
+    resource kinds that will be filtered form the output.
+    """
+
+    skip_crds: bool = True
+    """Skip CRDs when building the output."""
+
+    skip_tests: bool = True
+    """Don't run helm tests on the output."""
+
+    skip_secrets: bool = False
+    """Don't emit secrets in the output."""
+
+    kube_version: str | None = None
+    """Value of the helm --kube-version flag."""
+
+    api_versions: str | None = None
+    """Value of the helm --api-versions flag."""
+
+    @property
+    def template_args(self) -> list[str]:
+        """Helm template CLI arguments built from the options."""
+        args = []
+        if self.skip_crds:
+            args.append("--skip-crds")
+        if self.skip_tests:
+            args.append("--skip-tests")
+        if self.kube_version:
+            args.extend(["--kube-version", self.kube_version])
+        if self.api_versions:
+            args.extend(["--api-versions", self.api_versions])
+        return args
+
+    @property
+    def skip_resources(self) -> list[str]:
+        """A list of CRD resources to filter from the output."""
+        skips = []
+        if self.skip_crds:
+            skips.append(CRD_KIND)
+        if self.skip_secrets:
+            skips.append(SECRET_KIND)
+        return skips
+
+
 class Helm:
     """Manages local HelmRepository state."""
 
     def __init__(self, tmp_dir: Path, cache_dir: Path) -> None:
         """Initialize Helm."""
         self._tmp_dir = tmp_dir
         self._repo_config_file = self._tmp_dir / "repository-config.yaml"
@@ -131,27 +179,24 @@
                 [HELM_BIN, "repo", "update"] + self._flags, exc=HelmException
             )
         )
 
     async def template(
         self,
         release: HelmRelease,
-        values: dict[str, Any] | None = None,
-        skip_crds: bool = True,
-        skip_tests: bool = True,
-        skip_secrets: bool = False,
-        kube_version: str | None = None,
-        api_versions: str | None = None,
+        options: Options | None = None,
     ) -> Kustomize:
         """Return command line arguments to template the specified chart.
 
         The default values will come from the `HelmRelease`, though you can
         also specify values directory if not present in cluster manifest
         e.g. it came from a truncated yaml.
         """
+        if options is None:
+            options = Options()
         repo = next(
             iter([repo for repo in self._repos if repo.repo_name == release.repo_name]),
             None,
         )
         if not repo:
             raise HelmException(
                 f"Unable to find HelmRepository for {release.chart.chart_name} for "
@@ -161,38 +206,24 @@
             HELM_BIN,
             "template",
             release.name,
             _chart_name(repo, release),
             "--namespace",
             release.namespace,
         ]
-        if skip_crds:
-            args.append("--skip-crds")
-        if skip_tests:
-            args.append("--skip-tests")
+        args.extend(options.template_args)
         if release.chart.version:
             args.extend(
                 [
                     "--version",
                     release.chart.version,
                 ]
             )
-        if kube_version:
-            args.extend(["--kube-version", kube_version])
-        if api_versions:
-            args.extend(["--api-versions", api_versions])
-        if release.values and not values:
-            values = release.values
-        if values:
+        if release.values:
             values_path = self._tmp_dir / f"{release.release_name}-values.yaml"
             async with aiofiles.open(values_path, mode="w") as values_file:
-                await values_file.write(yaml.dump(values, sort_keys=False))
+                await values_file.write(yaml.dump(release.values, sort_keys=False))
             args.extend(["--values", str(values_path)])
         cmd = Kustomize([command.Command(args + self._flags, exc=HelmException)])
-        skips = []
-        if skip_crds:
-            skips.append(CRD_KIND)
-        if skip_secrets:
-            skips.append(SECRET_KIND)
-        if skips:
-            cmd = cmd.skip_resources(skips)
+        if options.skip_resources:
+            cmd = cmd.skip_resources(options.skip_resources)
         return cmd
```

### Comparing `flux-local-1.3.3/flux_local/kustomize.py` & `flux-local-2.0.0/flux_local/kustomize.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.3/flux_local/manifest.py` & `flux-local-2.0.0/flux_local/manifest.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.3/flux_local/tool/diff.py` & `flux-local-2.0.0/flux_local/tool/diff.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Flux-local diff action."""
 
 import asyncio
 import functools
 import os
-from argparse import ArgumentParser
-from argparse import _SubParsersAction as SubParsersAction
+from argparse import ArgumentParser, _SubParsersAction as SubParsersAction
 from contextlib import contextmanager
 from dataclasses import asdict
 import difflib
 import logging
 import pathlib
 import shlex
 import tempfile
@@ -310,14 +309,15 @@
                 description=(
                     "The diff command does a local kustomize build, then inflates "
                     "the helm template and compares with the repo and prints the diff."
                 ),
             ),
         )
         selector.add_hr_selector_flags(args)
+        selector.add_helm_options_flags(args)
         add_diff_flags(args)
         args.set_defaults(cls=cls)
         return args
 
     async def run(  # type: ignore[no-untyped-def]
         self,
         output: str,
@@ -329,14 +329,15 @@
         """Async Action implementation."""
         query = selector.build_hr_selector(**kwargs)
         content = ObjectOutput(strip_attrs)
         helm_visitor = HelmVisitor()
         query.kustomization.visitor = content.visitor()
         query.helm_repo.visitor = helm_visitor.repo_visitor()
         query.helm_release.visitor = helm_visitor.release_visitor()
+        options = selector.build_helm_options(**kwargs)
         await git_repo.build_manifest(
             selector=query, options=selector.options(**kwargs)
         )
 
         orig_content = ObjectOutput(strip_attrs)
         orig_helm_visitor = HelmVisitor()
         with create_diff_path(query.path, **kwargs) as path_selector:
@@ -385,24 +386,18 @@
                 orig_helm_visitor.releases[cluster_path] = releases
 
         helm_content = ObjectOutput(strip_attrs)
         orig_helm_content = ObjectOutput(strip_attrs)
         with tempfile.TemporaryDirectory() as helm_cache_dir:
             await asyncio.gather(
                 helm_visitor.inflate(
-                    pathlib.Path(helm_cache_dir),
-                    helm_content.visitor(),
-                    query.helm_release.skip_crds,
-                    skip_secrets=query.helm_release.skip_secrets,
+                    pathlib.Path(helm_cache_dir), helm_content.visitor(), options
                 ),
                 orig_helm_visitor.inflate(
-                    pathlib.Path(helm_cache_dir),
-                    orig_helm_content.visitor(),
-                    query.helm_release.skip_crds,
-                    skip_secrets=query.helm_release.skip_secrets,
+                    pathlib.Path(helm_cache_dir), orig_helm_content.visitor(), options
                 ),
             )
 
         if output == "yaml":
             for line in perform_yaml_diff(
                 orig_helm_content, helm_content, unified, limit_bytes
             ):
@@ -426,14 +421,19 @@
     def register(
         cls, subparsers: SubParsersAction  # type: ignore[type-arg]
     ) -> ArgumentParser:
         """Register the subparser commands."""
         args: ArgumentParser = subparsers.add_parser(
             "diff",
             help="Diff a local flux resource",
+            description="""You may also use flux-local to verify your local changes
+                to cluster resources have the desird effect. This is similar to flux
+                diff but entirely local. This will run a local kustomize build first
+                against the local repo then again against a prior repo revision, then
+                prints the output.""",
         )
         subcmds = args.add_subparsers(
             title="Available commands",
             required=True,
         )
         DiffKustomizationAction.register(subcmds)
         DiffHelmReleaseAction.register(subcmds)
```

### Comparing `flux-local-1.3.3/flux_local/tool/flux_local.py` & `flux-local-2.0.0/flux_local/tool/flux_local.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,41 @@
 """Command line tool for building, diffing, validating flux local repositories."""
 
 import argparse
 import asyncio
 import logging
-import pathlib
 import sys
 import traceback
 from typing import Any
 
 import yaml
 
 from . import build, diff, get, test
 from flux_local.exceptions import FluxException
 
 _LOGGER = logging.getLogger(__name__)
 
 
+def _make_parser() -> argparse.ArgumentParser:
+    parser = argparse.ArgumentParser(
+        description="Command line utility for inspecting a local flux repository.",
+    )
+    parser.add_argument(
+        "--log-level", choices=["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]
+    )
+
+    subparsers = parser.add_subparsers(dest="command", help="Command", required=True)
+
+    build.BuildAction.register(subparsers)
+    get.GetAction.register(subparsers)
+    diff.DiffAction.register(subparsers)
+    test.TestAction.register(subparsers)
+    return parser
+
+
 def main() -> None:
     """Flux-local command line tool main entry point."""
 
     def str_presenter(dumper: yaml.Dumper, data: Any) -> Any:
         """Represent multi-line yaml strings as you'd expect.
 
         See https://github.com/yaml/pyyaml/issues/240
@@ -29,63 +45,15 @@
         )
 
     yaml.add_representer(str, str_presenter)
 
     # https://github.com/yaml/pyyaml/issues/89
     yaml.Loader.yaml_implicit_resolvers.pop("=")
 
-    parser = argparse.ArgumentParser(
-        description="Command line utility for inspecting a local flux repository.",
-    )
-    parser.add_argument(
-        "--log-level", choices=["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]
-    )
-
-    subparsers = parser.add_subparsers(dest="command", help="Command", required=True)
-
-    build_args = subparsers.add_parser(
-        "build",
-        help="Build local flux Kustomization target from a local directory",
-    )
-    build_args.add_argument(
-        "path", type=pathlib.Path, help="Path to the kustomization or charts"
-    )
-    build_args.add_argument(
-        "--enable-helm",
-        type=bool,
-        action=argparse.BooleanOptionalAction,
-        help="Enable use of HelmRelease inflation",
-    )
-    # pylint: disable=duplicate-code
-    build_args.add_argument(
-        "--skip-crds",
-        type=bool,
-        default=False,
-        action=argparse.BooleanOptionalAction,
-        help="Allows disabling of outputting CRDs to reduce output size",
-    )
-    build_args.add_argument(
-        "--skip-secrets",
-        type=bool,
-        default=True,
-        action=argparse.BooleanOptionalAction,
-        help="Omit secrets from the output to reduce random output.",
-    )
-    build_args.add_argument(
-        "--kustomize-build-flags",
-        type=str,
-        default="",
-        help="If present, additional flags to pass to `kustomize build`",
-    )
-    build_args.set_defaults(cls=build.BuildAction)
-
-    get.GetAction.register(subparsers)
-    diff.DiffAction.register(subparsers)
-    test.TestAction.register(subparsers)
-
+    parser = _make_parser()
     args = parser.parse_args()
 
     if args.log_level:
         logging.basicConfig(level=args.log_level)
 
     action = args.cls()
     try:
```

### Comparing `flux-local-1.3.3/flux_local/tool/format.py` & `flux-local-2.0.0/flux_local/tool/format.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.3/flux_local/tool/get.py` & `flux-local-2.0.0/flux_local/tool/get.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Flux-local get action."""
 
 import logging
-from argparse import ArgumentParser
-from argparse import _SubParsersAction as SubParsersAction
+from argparse import ArgumentParser, _SubParsersAction as SubParsersAction
 from typing import cast, Any
 
 from flux_local import git_repo
 
 from .format import PrintFormatter, YamlFormatter
 from . import selector
```

### Comparing `flux-local-1.3.3/flux_local/tool/selector.py` & `flux-local-2.0.0/flux_local/tool/selector.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Namespace,
 )
 import logging
 import pathlib
 import shlex
 from typing import Any
 
-from flux_local import git_repo
+from flux_local import git_repo, helm
 
 _LOGGER = logging.getLogger(__name__)
 
 DEFAULT_NAMESPACE = "flux-system"
 
 
 class SourceAppendAction(Action):
@@ -66,14 +66,19 @@
     args.add_argument(
         "--namespace",
         "-n",
         type=str,
         default=DEFAULT_NAMESPACE,
         help="If present, the namespace scope for this request",
     )
+    add_common_flags(args)
+
+
+def add_common_flags(args: ArgumentParser) -> None:
+    """Add flags that are common to selectors and other command types."""
     args.add_argument(
         "--skip-crds",
         type=str,
         default=True,
         action=BooleanOptionalAction,
         help="When true do not include CRDs to reduce output size",
     )
@@ -158,14 +163,41 @@
         selector.helm_release.namespace = None
     selector.helm_release.skip_crds = kwargs["skip_crds"]
     selector.helm_release.skip_secrets = kwargs["skip_secrets"]
     selector.cluster_policy.enabled = False
     return selector
 
 
+def add_helm_options_flags(args: ArgumentParser) -> None:
+    """Add common helm template options flags to the arguments object."""
+    args.add_argument(
+        "--kube-version",
+        help="Kubernetes version used for Capabilities.KubeVersion",
+    )
+    args.add_argument(
+        "--api-versions",
+        "-a",
+        help="Kubernetes api versions used for helm Capabilities.APIVersions",
+    )
+
+
+def build_helm_options(**kwargs) -> helm.Options:  # type: ignore[no-untyped-def]
+    """Build a helm Options object from the flags.
+
+    This assumes that the hr selector and helm options flags methods were
+    called to add arguments to the parser.
+    """
+    return helm.Options(
+        skip_crds=kwargs["skip_crds"],
+        skip_secrets=kwargs["skip_secrets"],
+        kube_version=kwargs.get("kube_version"),
+        api_versions=kwargs.get("api_versions"),
+    )
+
+
 def add_cluster_selector_flags(args: ArgumentParser) -> None:
     """Add common flux cluster selector flags to the arguments object."""
     add_selector_flags(args)
 
 
 def build_cluster_selector(  # type: ignore[no-untyped-def]
     **kwargs,
```

### Comparing `flux-local-1.3.3/flux_local/tool/test.py` & `flux-local-2.0.0/flux_local/tool/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """Flux local test action."""
 
-from argparse import ArgumentParser, BooleanOptionalAction
-from argparse import _SubParsersAction as SubParsersAction
+from argparse import (
+    ArgumentParser,
+    BooleanOptionalAction,
+    _SubParsersAction as SubParsersAction,
+)
 import asyncio
 from dataclasses import dataclass
 import logging
 import pathlib
 import tempfile
 from pathlib import Path
 import sys
 from typing import cast, Generator, Any
 
 import nest_asyncio
 import pytest
 
 from flux_local import git_repo, kustomize
-from flux_local.helm import Helm
+from flux_local.helm import Helm, Options
 from flux_local.manifest import (
     Manifest,
     Cluster,
     Kustomization,
     HelmRelease,
     HelmRepository,
 )
@@ -29,16 +32,15 @@
 
 
 @dataclass
 class TestConfig:
     """Test configuration, which are parameters to types of the tests."""
 
     options: git_repo.Options
-    kube_version: str | None = None
-    api_versions: str | None = None
+    helm_options: Options
 
 
 class HelmReleaseTest(pytest.Item):
     """Test case for a Kustomization."""
 
     cluster: Cluster
     kustomization: Kustomization
@@ -83,17 +85,15 @@
             tempfile.TemporaryDirectory() as tmp_dir,
         ):
             helm = Helm(pathlib.Path(tmp_dir), pathlib.Path(helm_cache_dir))
             helm.add_repos(self.active_repos())
             await helm.update()
             cmd = await helm.template(
                 self.helm_release,
-                skip_crds=True,
-                kube_version=self.test_config.kube_version,
-                api_versions=self.test_config.api_versions,
+                self.test_config.helm_options,
             )
             await cmd.objects()
             await cmd.validate_policies(self.cluster.cluster_policies)
 
     def active_repos(self) -> list[HelmRepository]:
         """Return HelpRepositories referenced by a HelmRelease."""
         repo_key = "-".join(
@@ -332,14 +332,18 @@
     ) -> ArgumentParser:
         """Register the subparser commands."""
         args = cast(
             ArgumentParser,
             subparsers.add_parser(
                 "test",
                 help="Build and validate the cluster",
+                description="""You can verify that the resources in the cluster
+                    are formatted properly before commit or as part of a CI
+                    system. The flux-local test command will build the
+                    Kustomization resources in the cluster.""",
             ),
         )
         args.add_argument(
             "--enable-helm",
             type=bool,
             action=BooleanOptionalAction,
             help="Enable use of HelmRelease inflation",
@@ -370,23 +374,15 @@
             "--verbosity",
             action="store",
             type=int,
             metavar="N",
             dest="verbosity",
             help="Set verbosity. Default is 0",
         )
-        args.add_argument(
-            "--kube-version",
-            help="Kubernetes version used for Capabilities.KubeVersion",
-        )
-        args.add_argument(
-            "--api-versions",
-            "-a",
-            help="Kubernetes api versions used for helm Capabilities.APIVersions",
-        )
+        selector.add_helm_options_flags(args)
         args.set_defaults(cls=cls, verbosity=0)
         selector.add_cluster_selector_flags(args)
         return args
 
     async def run(  # type: ignore[no-untyped-def]
         self,
         enable_helm: bool,
@@ -408,14 +404,15 @@
                 test_path = None
         query.kustomization.namespace = query.cluster.namespace
         query.kustomization.skip_crds = True
         query.helm_release.enabled = enable_helm
         query.helm_release.namespace = None
         query.cluster_policy.enabled = enable_kyverno
         options = selector.options(**kwargs)
+        helm_options = selector.build_helm_options(**kwargs)
 
         nest_asyncio.apply()
         pytest_args = [
             "--verbosity",
             str(verbosity),
             "--no-header",
             "--disable-warnings",
@@ -427,16 +424,15 @@
         retcode = pytest.main(
             pytest_args,
             plugins=[
                 ManifestPlugin(
                     query,
                     TestConfig(
                         options=options,
-                        kube_version=kube_version,
-                        api_versions=api_versions,
+                        helm_options=helm_options,
                     ),
                     test_filter=[str(test_path)] if test_path else [],
                 )
             ],
         )
         if retcode:
             sys.exit(retcode)
```

### Comparing `flux-local-1.3.3/flux_local/tool/visitor.py` & `flux-local-2.0.0/flux_local/tool/visitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import logging
 import pathlib
 import tempfile
 import yaml
 from typing import Any
 
 from flux_local import git_repo
+from flux_local.helm import Helm, Options
 from flux_local.kustomize import Kustomize
-from flux_local.helm import Helm
 from flux_local.manifest import (
     HelmRelease,
     Kustomization,
     HelmRepository,
     ClusterPolicy,
 )
 
@@ -200,18 +200,17 @@
 
 
 async def inflate_release(
     cluster_path: pathlib.Path,
     helm: Helm,
     release: HelmRelease,
     visitor: git_repo.ResourceVisitor,
-    skip_crds: bool,
-    skip_secrets: bool,
+    options: Options,
 ) -> None:
-    cmd = await helm.template(release, skip_crds=skip_crds, skip_secrets=skip_secrets)
+    cmd = await helm.template(release, options)
     # We can ignore the Kustomiation path since we're essentially grouping by cluster
     await visitor.func(cluster_path, pathlib.Path(""), release, cmd)
 
 
 class HelmVisitor:
     """Helper that visits Helm related objects and handles inflation."""
 
@@ -266,49 +265,50 @@
 
         return git_repo.ResourceVisitor(func=add_release)
 
     async def inflate(
         self,
         helm_cache_dir: pathlib.Path,
         visitor: git_repo.ResourceVisitor,
-        skip_crds: bool,
-        skip_secrets: bool,
+        options: Options,
     ) -> None:
         """Expand and notify about HelmReleases discovered."""
         cluster_paths = set(list(self.releases)) | set(list(self.repos))
         tasks = [
             self.inflate_cluster(
                 helm_cache_dir,
                 pathlib.Path(cluster_path),
                 visitor,
-                skip_crds,
-                skip_secrets,
+                options,
             )
             for cluster_path in cluster_paths
         ]
         _LOGGER.debug("Waiting for cluster inflation to complete")
         await asyncio.gather(*tasks)
 
     async def inflate_cluster(
         self,
         helm_cache_dir: pathlib.Path,
         cluster_path: pathlib.Path,
         visitor: git_repo.ResourceVisitor,
-        skip_crds: bool,
-        skip_secrets: bool,
+        options: Options,
     ) -> None:
         _LOGGER.debug("Inflating Helm charts in cluster %s", cluster_path)
         if not self.releases:
             return
         with tempfile.TemporaryDirectory() as tmp_dir:
             helm = Helm(pathlib.Path(tmp_dir), helm_cache_dir)
             if active_repos := self.active_repos(str(cluster_path)):
                 helm.add_repos(active_repos)
                 await helm.update()
             tasks = [
                 inflate_release(
-                    cluster_path, helm, release, visitor, skip_crds, skip_secrets
+                    cluster_path,
+                    helm,
+                    release,
+                    visitor,
+                    options,
                 )
                 for release in self.releases.get(str(cluster_path), [])
             ]
             _LOGGER.debug("Waiting for tasks to inflate %s", cluster_path)
             await asyncio.gather(*tasks)
```

### Comparing `flux-local-1.3.3/flux_local.egg-info/PKG-INFO` & `flux-local-2.0.0/flux_local.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-local
-Version: 1.3.3
+Version: 2.0.0
 Summary: flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 Home-page: https://github.com/allenporter/flux-local
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
```

### Comparing `flux-local-1.3.3/flux_local.egg-info/SOURCES.txt` & `flux-local-2.0.0/flux_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.3/setup.cfg` & `flux-local-2.0.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flux-local
-version = 1.3.3
+version = 2.0.0
 description = flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 long_description = file: README.md
 long_description_content_type = text/markdown
 prodid = github.com/allenporter/flux-local
 url = https://github.com/allenporter/flux-local
 author = Allen Porter
 author_email = allen.porter@gmail.com
```

### Comparing `flux-local-1.3.3/tests/test_command.py` & `flux-local-2.0.0/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.3/tests/test_git_repo.py` & `flux-local-2.0.0/tests/test_git_repo.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.3/tests/test_helm.py` & `flux-local-2.0.0/tests/test_helm.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.3/tests/test_kustomize.py` & `flux-local-2.0.0/tests/test_kustomize.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.3/tests/test_manifest.py` & `flux-local-2.0.0/tests/test_manifest.py`

 * *Files identical despite different names*

