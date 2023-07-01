# Comparing `tmp/slskit-2022.4.0.tar.gz` & `tmp/slskit-2023.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slskit-2022.4.0.tar", max compression
+gzip compressed data, was "slskit-2023.7.0.tar", max compression
```

## Comparing `slskit-2022.4.0.tar` & `slskit-2023.7.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     3225 2022-04-20 19:04:44.085598 slskit-2022.4.0/README.md
--rw-r--r--   0        0        0      961 2022-04-21 07:09:06.123628 slskit-2022.4.0/pyproject.toml
--rw-r--r--   0        0        0      137 2022-04-21 07:08:12.824204 slskit-2022.4.0/slskit/__init__.py
--rw-r--r--   0        0        0     3433 2022-04-21 07:07:16.716508 slskit-2022.4.0/slskit/__main__.py
--rw-r--r--   0        0        0        0 2021-10-31 10:37:24.306587 slskit-2022.4.0/slskit/lib/__init__.py
--rw-r--r--   0        0        0      650 2021-10-31 10:37:24.306698 slskit-2022.4.0/slskit/lib/cli.py
--rw-r--r--   0        0        0      645 2022-04-21 07:04:00.445477 slskit-2022.4.0/slskit/lib/logging.py
--rw-r--r--   0        0        0     3096 2021-10-31 10:37:24.306897 slskit-2022.4.0/slskit/opts.py
--rw-r--r--   0        0        0      689 2021-11-17 20:45:11.864318 slskit-2022.4.0/slskit/pillar.py
--rw-r--r--   0        0        0     1922 2021-10-31 10:37:24.307095 slskit-2022.4.0/slskit/state.py
--rw-r--r--   0        0        0     1255 2021-11-17 20:45:11.864621 slskit-2022.4.0/slskit/template.py
--rw-r--r--   0        0        0      434 2021-10-31 10:37:24.307308 slskit-2022.4.0/slskit/types.py
--rw-r--r--   0        0        0     4257 2022-04-21 07:14:33.839821 slskit-2022.4.0/setup.py
--rw-r--r--   0        0        0     4081 2022-04-21 07:14:33.840224 slskit-2022.4.0/PKG-INFO
+-rw-r--r--   0        0        0     3217 2023-07-01 12:08:32.539763 slskit-2023.7.0/README.md
+-rw-r--r--   0        0        0      837 2023-07-01 12:32:26.878158 slskit-2023.7.0/pyproject.toml
+-rw-r--r--   0        0        0      137 2023-07-01 12:30:06.564639 slskit-2023.7.0/slskit/__init__.py
+-rw-r--r--   0        0        0     3694 2022-11-01 10:02:15.211048 slskit-2023.7.0/slskit/__main__.py
+-rw-r--r--   0        0        0        0 2021-10-31 10:37:24.306587 slskit-2023.7.0/slskit/lib/__init__.py
+-rw-r--r--   0        0        0      650 2021-10-31 10:37:24.306698 slskit-2023.7.0/slskit/lib/cli.py
+-rw-r--r--   0        0        0      207 2022-10-25 21:19:05.939371 slskit-2023.7.0/slskit/lib/logging.py
+-rw-r--r--   0        0        0     3197 2022-11-01 09:43:48.801428 slskit-2023.7.0/slskit/opts.py
+-rw-r--r--   0        0        0      689 2021-11-17 20:45:11.864318 slskit-2023.7.0/slskit/pillar.py
+-rw-r--r--   0        0        0     1922 2021-10-31 10:37:24.307095 slskit-2023.7.0/slskit/state.py
+-rw-r--r--   0        0        0     1255 2021-11-17 20:45:11.864621 slskit-2023.7.0/slskit/template.py
+-rw-r--r--   0        0        0      434 2021-10-31 10:37:24.307308 slskit-2023.7.0/slskit/types.py
+-rw-r--r--   0        0        0     4096 1970-01-01 00:00:00.000000 slskit-2023.7.0/PKG-INFO
```

### Comparing `slskit-2022.4.0/README.md` & `slskit-2023.7.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 # slskit
 
-![release](https://img.shields.io/github/release/gediminasz/slskit.svg)
-![python](https://img.shields.io/pypi/pyversions/slskit)
-![build](https://github.com/gediminasz/slskit/workflows/CI/badge.svg?branch=master)
-![black](https://img.shields.io/badge/code%20style-black-000000.svg)
-
 ```
 Usage: slskit [OPTIONS] COMMAND [ARGS]...
 
 Options:
   --version                       Show the version and exit.
   -c, --config TEXT               path to slskit configuration file (default:
                                   slskit.yaml or slskit.yml)
-
-  -l, --log-level [CRITICAL|FATAL|ERROR|WARN|WARNING|INFO|DEBUG|NOTSET|QUIET|PROFILE|TRACE|GARBAGE]
+  -l, --log-level [CRITICAL|FATAL|ERROR|WARN|WARNING|INFO|DEBUG|NOTSET|VERBOSE|QUIET|PROFILE|TRACE|GARBAGE]
+  --salt-output TEXT              Alternative Salt outputter, e.g. nested,
+                                  json, yaml, etc.
   --help                          Show this message and exit.
 
 Commands:
   highstate  render highstate for specified minions
   pillars    render pillar items for specified minions
   refresh    invoke saltutil.sync_all runner
   sls        render a given sls for specified minions
   template   render a file template for specified minions
 ```
 
-- Supported Python versions: 3.7, 3.8, 3.9
-- Supported Salt versions: 3001, 3002, 3003, 3004
+- Supported Python versions: 3.8, 3.9, 3.10
+- Supported Salt versions: 3005, 3006
 
 ---
 
 ## Workaround for libcrypto.dylib failing to load on macOS
 
 If `slskit` fails with `zsh: abort` or `Abort trap: 6`, inspect the error by running the command with `PYTHONDEVMODE=1`. If the issue is with `_load_libcrypto` call in `rsax931.py`, edit `salt/utils/rsax931.py` line 38:
 
@@ -124,8 +120,9 @@
 ```
 
 ---
 
 
 ## External links
 
-- https://saltproject.io/salt-platform-support/
+- https://docs.saltproject.io/salt/install-guide/en/latest/topics/salt-version-support-lifecycle.html
+- https://docs.saltproject.io/salt/install-guide/en/latest/topics/salt-python-version-support.html
```

### Comparing `slskit-2022.4.0/pyproject.toml` & `slskit-2023.7.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 [tool.poetry]
 name = "slskit"
-version = "2022.4.0"
+version = "2023.7.0"
 authors = ["Gediminas Zlatkus <gediminas.zlatkus@gmail.com>"]
 description = "Tools for checking Salt state validity"
 readme = "README.md"
 homepage = "https://github.com/gediminasz/slskit"
 repository = "https://github.com/gediminasz/slskit"
 keywords = ["salt", "saltstack", "sls"]
 classifiers = ["Topic :: Software Development :: Quality Assurance"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-click = "^8.1.2"
-colorlog = "^6.6.0"
-funcy = "^1.17"
-# TODO remove Jinja2 line when this fix is released https://github.com/saltstack/salt/issues/61848
-Jinja2 = "<3.1"
-jsonschema = "^4.4.0"
-salt = ">=3001.0"
+python = "^3.8"
+click = "^8.1.3"
+colorlog = "^6.7.0"
+funcy = "^2.0"
+jsonschema = "^4.17.3"
+salt = ">=3005.0"
 
-[tool.poetry.dev-dependencies]
-black = "^22.3.0"
-GitPython = "^3.1.27"
-mypy = "^0.942"
-pylint = "^2.13.7"
-pytest = "^7.1.1"
-pytest-snapshot = "^0.8.1"
-types-PyYAML = "^6.0.7"
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+gitpython = "^3.1.31"
+mypy = "^1.4.1"
+pytest = "^7.4.0"
+pytest-snapshot = "^0.9.0"
+types-pyyaml = "^6.0.12.10"
 
 [tool.poetry.scripts]
 slskit = 'slskit:run_module'
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `slskit-2022.4.0/slskit/__main__.py` & `slskit-2023.7.0/slskit/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import logging
 import sys
 from typing import List
 from unittest.mock import patch
 
 import click
+import colorlog
 import salt.output
 import salt.runners.saltutil
 import salt.utils.yaml
 
 import slskit.lib.cli
 import slskit.lib.logging
 import slskit.pillar
@@ -32,20 +33,29 @@
 )
 @click.option(
     "-l",
     "--log-level",
     default="WARNING",
     type=click.Choice(slskit.lib.logging.LEVEL_CHOICES),
 )
+@click.option(
+    "--salt-output",
+    help="Alternative Salt outputter, e.g. nested, json, yaml, etc.",
+)
 @click.pass_context
-def cli(ctx: click.Context, config_path: str, log_level: str) -> None:
+def cli(ctx: click.Context, config_path: str, log_level: str, salt_output: str) -> None:
+    dynamic_overrides = {}
+    if salt_output:
+        dynamic_overrides["output"] = salt_output
+
     ctx.ensure_object(dict)
-    ctx.obj["config"] = Config(config_path)
+    ctx.obj["config"] = Config(config_path, dynamic_overrides)
+
     log_level = getattr(logging, log_level)
-    slskit.lib.logging.basic_config(level=log_level)
+    colorlog.basicConfig(level=log_level, force=True)
 
 
 @cli.command(help="render highstate for specified minions")
 @slskit.lib.cli.minion_id_argument()
 @click.pass_context
 def highstate(ctx: click.Context, minion_id: List[str]) -> None:
     minion_dict = slskit.state.show_highstate(minion_id, ctx.obj["config"])
```

### Comparing `slskit-2022.4.0/slskit/lib/cli.py` & `slskit-2023.7.0/slskit/lib/cli.py`

 * *Files identical despite different names*

### Comparing `slskit-2022.4.0/slskit/opts.py` & `slskit-2023.7.0/slskit/opts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os
 from dataclasses import dataclass
+from functools import cached_property
 from typing import Any, Optional, cast
 
 import jsonschema
 import salt.config
 import salt.utils
 import yaml
-from funcy import cached_property, get_in, post_processing
+from funcy import get_in, post_processing
 
 from . import PACKAGE_NAME
 from .types import AnyDict
 
 DEFAULT_CONFIG_PATHS = (f"{PACKAGE_NAME}.yaml", f"{PACKAGE_NAME}.yml")
 
 SCHEMA: AnyDict = {
@@ -44,14 +45,15 @@
     jsonschema.validate(instance, schema or SCHEMA)
     return instance
 
 
 @dataclass
 class Config:
     config_path: str
+    dynamic_overrides: AnyDict
 
     @cached_property
     def opts(self) -> AnyDict:
         overrides = {
             "root_dir": f".{PACKAGE_NAME}",
             "state_events": False,
             "file_client": "local",
@@ -59,14 +61,15 @@
 
         if self._get_setting("slskit.skip_fileserver_update", True):
             # skip fileserver update for faster rendering
             # see salt.fileserver.FSChan implementation
             overrides["__fs_update"] = True
 
         overrides.update(self.settings.get("salt", {}))
+        overrides.update(self.dynamic_overrides)
         opts = salt.config.apply_minion_config(overrides)
         return cast(AnyDict, opts)
 
     @cached_property
     def roster(self) -> AnyDict:
         result = self._get_setting(f"{PACKAGE_NAME}.roster", {})
         return cast(AnyDict, result)
```

### Comparing `slskit-2022.4.0/slskit/pillar.py` & `slskit-2023.7.0/slskit/pillar.py`

 * *Files identical despite different names*

### Comparing `slskit-2022.4.0/slskit/state.py` & `slskit-2023.7.0/slskit/state.py`

 * *Files identical despite different names*

### Comparing `slskit-2022.4.0/slskit/template.py` & `slskit-2023.7.0/slskit/template.py`

 * *Files identical despite different names*

### Comparing `slskit-2022.4.0/setup.py` & `slskit-2023.7.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,152 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: slskit
+Version: 2023.7.0
+Summary: Tools for checking Salt state validity
+Home-page: https://github.com/gediminasz/slskit
+Keywords: salt,saltstack,sls
+Author: Gediminas Zlatkus
+Author-email: gediminas.zlatkus@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Quality Assurance
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: colorlog (>=6.7.0,<7.0.0)
+Requires-Dist: funcy (>=2.0,<3.0)
+Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
+Requires-Dist: salt (>=3005.0)
+Project-URL: Repository, https://github.com/gediminasz/slskit
+Description-Content-Type: text/markdown
+
+# slskit
+
+```
+Usage: slskit [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  --version                       Show the version and exit.
+  -c, --config TEXT               path to slskit configuration file (default:
+                                  slskit.yaml or slskit.yml)
+  -l, --log-level [CRITICAL|FATAL|ERROR|WARN|WARNING|INFO|DEBUG|NOTSET|VERBOSE|QUIET|PROFILE|TRACE|GARBAGE]
+  --salt-output TEXT              Alternative Salt outputter, e.g. nested,
+                                  json, yaml, etc.
+  --help                          Show this message and exit.
+
+Commands:
+  highstate  render highstate for specified minions
+  pillars    render pillar items for specified minions
+  refresh    invoke saltutil.sync_all runner
+  sls        render a given sls for specified minions
+  template   render a file template for specified minions
+```
+
+- Supported Python versions: 3.8, 3.9, 3.10
+- Supported Salt versions: 3005, 3006
+
+---
+
+## Workaround for libcrypto.dylib failing to load on macOS
+
+If `slskit` fails with `zsh: abort` or `Abort trap: 6`, inspect the error by running the command with `PYTHONDEVMODE=1`. If the issue is with `_load_libcrypto` call in `rsax931.py`, edit `salt/utils/rsax931.py` line 38:
+
+```diff
+-lib = find_library('crypto')
++lib = "/usr/local/opt/openssl@1.1/lib/libcrypto.dylib"
+```
+
+More info:
+
+- https://github.com/saltstack/salt/issues/55084
+- https://github.com/Homebrew/homebrew-core/pull/45895/files#diff-5bdebf3b9146d50b15f9a0dc7e7def27R131-R133
+
+## Workaround for exception raised when processing __virtual__ function
+
+When seeing errors like these:
+
+```
+ERROR:salt.loader:Exception raised when processing __virtual__ function for salt.loaded.int.module.freebsdkmod. Module will not be loaded: 'kernel'
+WARNING:salt.loader:salt.loaded.int.module.freebsdkmod.__virtual__() is wrongly returning `None`. It should either return `True`, `False` or a new name. If you're the developer of the module 'freebsdkmod', please fix this.
+```
+
+You may need to add a corresponding grain to `slskit.yaml` file, e.g.:
+
+```yaml
+# slskit.yaml
+
+slskit:
+  roster:
+    foo:
+      grains:
+        kernel: Linux
+```
+
+You can find values for grains by inspecting `grains.items` on your real minions.
+
+## How to keep your grains DRY
+
+Use `default_grains` option to avoid duplicating the same grains over all minions:
+
+```yaml
+# slskit.yaml
+
+slskit:
+  roster:
+    foo:
+    bar:
+    baz:
+  default_grains:
+    os: Ubuntu
+```
+
+For more advanced cases use YAML anchors:
+
+```yaml
+# slskit.yaml
+
+_grains:
+  ubuntu: &ubuntu
+    os: Ubuntu
+  fedora: &fedora
+    os: Fedora
+
+slskit:
+  roster:
+    u1:
+      grains:
+        <<: *ubuntu
+    u2:
+      grains:
+        <<: *ubuntu
+    f1:
+      grains:
+        <<: *fedora
+    f2:
+      grains:
+        <<: *fedora
+```
+
+## How to reduce output verbosity
+
+Use Salt's [`output` configuration option](https://docs.saltstack.com/en/latest/ref/configuration/master.html#output), e.g.:
+
+```yaml
+# slskit.yaml
+
+salt:
+  output: yaml
+
+slskit:
+  ...
+```
 
-packages = \
-['slskit', 'slskit.lib']
+---
 
-package_data = \
-{'': ['*']}
 
-install_requires = \
-['Jinja2<3.1',
- 'click>=8.1.2,<9.0.0',
- 'colorlog>=6.6.0,<7.0.0',
- 'funcy>=1.17,<2.0',
- 'jsonschema>=4.4.0,<5.0.0',
- 'salt>=3001.0']
-
-entry_points = \
-{'console_scripts': ['slskit = slskit:run_module']}
-
-setup_kwargs = {
-    'name': 'slskit',
-    'version': '2022.4.0',
-    'description': 'Tools for checking Salt state validity',
-    'long_description': '# slskit\n\n![release](https://img.shields.io/github/release/gediminasz/slskit.svg)\n![python](https://img.shields.io/pypi/pyversions/slskit)\n![build](https://github.com/gediminasz/slskit/workflows/CI/badge.svg?branch=master)\n![black](https://img.shields.io/badge/code%20style-black-000000.svg)\n\n```\nUsage: slskit [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n  --version                       Show the version and exit.\n  -c, --config TEXT               path to slskit configuration file (default:\n                                  slskit.yaml or slskit.yml)\n\n  -l, --log-level [CRITICAL|FATAL|ERROR|WARN|WARNING|INFO|DEBUG|NOTSET|QUIET|PROFILE|TRACE|GARBAGE]\n  --help                          Show this message and exit.\n\nCommands:\n  highstate  render highstate for specified minions\n  pillars    render pillar items for specified minions\n  refresh    invoke saltutil.sync_all runner\n  sls        render a given sls for specified minions\n  template   render a file template for specified minions\n```\n\n- Supported Python versions: 3.7, 3.8, 3.9\n- Supported Salt versions: 3001, 3002, 3003, 3004\n\n---\n\n## Workaround for libcrypto.dylib failing to load on macOS\n\nIf `slskit` fails with `zsh: abort` or `Abort trap: 6`, inspect the error by running the command with `PYTHONDEVMODE=1`. If the issue is with `_load_libcrypto` call in `rsax931.py`, edit `salt/utils/rsax931.py` line 38:\n\n```diff\n-lib = find_library(\'crypto\')\n+lib = "/usr/local/opt/openssl@1.1/lib/libcrypto.dylib"\n```\n\nMore info:\n\n- https://github.com/saltstack/salt/issues/55084\n- https://github.com/Homebrew/homebrew-core/pull/45895/files#diff-5bdebf3b9146d50b15f9a0dc7e7def27R131-R133\n\n## Workaround for exception raised when processing __virtual__ function\n\nWhen seeing errors like these:\n\n```\nERROR:salt.loader:Exception raised when processing __virtual__ function for salt.loaded.int.module.freebsdkmod. Module will not be loaded: \'kernel\'\nWARNING:salt.loader:salt.loaded.int.module.freebsdkmod.__virtual__() is wrongly returning `None`. It should either return `True`, `False` or a new name. If you\'re the developer of the module \'freebsdkmod\', please fix this.\n```\n\nYou may need to add a corresponding grain to `slskit.yaml` file, e.g.:\n\n```yaml\n# slskit.yaml\n\nslskit:\n  roster:\n    foo:\n      grains:\n        kernel: Linux\n```\n\nYou can find values for grains by inspecting `grains.items` on your real minions.\n\n## How to keep your grains DRY\n\nUse `default_grains` option to avoid duplicating the same grains over all minions:\n\n```yaml\n# slskit.yaml\n\nslskit:\n  roster:\n    foo:\n    bar:\n    baz:\n  default_grains:\n    os: Ubuntu\n```\n\nFor more advanced cases use YAML anchors:\n\n```yaml\n# slskit.yaml\n\n_grains:\n  ubuntu: &ubuntu\n    os: Ubuntu\n  fedora: &fedora\n    os: Fedora\n\nslskit:\n  roster:\n    u1:\n      grains:\n        <<: *ubuntu\n    u2:\n      grains:\n        <<: *ubuntu\n    f1:\n      grains:\n        <<: *fedora\n    f2:\n      grains:\n        <<: *fedora\n```\n\n## How to reduce output verbosity\n\nUse Salt\'s [`output` configuration option](https://docs.saltstack.com/en/latest/ref/configuration/master.html#output), e.g.:\n\n```yaml\n# slskit.yaml\n\nsalt:\n  output: yaml\n\nslskit:\n  ...\n```\n\n---\n\n\n## External links\n\n- https://saltproject.io/salt-platform-support/\n',
-    'author': 'Gediminas Zlatkus',
-    'author_email': 'gediminas.zlatkus@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/gediminasz/slskit',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+## External links
 
+- https://docs.saltproject.io/salt/install-guide/en/latest/topics/salt-version-support-lifecycle.html
+- https://docs.saltproject.io/salt/install-guide/en/latest/topics/salt-python-version-support.html
 
-setup(**setup_kwargs)
```

