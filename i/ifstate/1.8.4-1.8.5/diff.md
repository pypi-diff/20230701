# Comparing `tmp/ifstate-1.8.4.tar.gz` & `tmp/ifstate-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifstate-1.8.4.tar", last modified: Thu Jun  8 12:57:02 2023, max compression
+gzip compressed data, was "ifstate-1.8.5.tar", last modified: Sat Jul  1 17:05:43 2023, max compression
```

## Comparing `ifstate-1.8.4.tar` & `ifstate-1.8.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.773380 ifstate-1.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-08 12:56:45.000000 ifstate-1.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-08 12:57:02.769379 ifstate-1.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-08 12:56:45.000000 ifstate-1.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.765380 ifstate-1.8.4/ifstate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:56:45.000000 ifstate-1.8.4/ifstate/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6391 2023-06-08 12:56:45.000000 ifstate-1.8.4/ifstate/ifstate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-08 12:56:45.000000 ifstate-1.8.4/ifstate/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.765380 ifstate-1.8.4/ifstate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-08 12:57:02.000000 ifstate-1.8.4/ifstate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-08 12:57:02.000000 ifstate-1.8.4/ifstate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:57:02.000000 ifstate-1.8.4/ifstate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 12:57:02.000000 ifstate-1.8.4/ifstate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-08 12:57:02.000000 ifstate-1.8.4/ifstate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-08 12:57:02.000000 ifstate-1.8.4/ifstate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.769379 ifstate-1.8.4/libifstate/
--rw-r--r--   0 runner    (1001) docker     (123)    23902 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.769379 ifstate-1.8.4/libifstate/address/
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/address/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.769379 ifstate-1.8.4/libifstate/bpf/
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/bpf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/bpf/ctypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10818 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/bpf/map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.769379 ifstate-1.8.4/libifstate/brport/
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/brport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.769379 ifstate-1.8.4/libifstate/link/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22110 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/link/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/link/physical.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/link/tun.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/link/veth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.769379 ifstate-1.8.4/libifstate/neighbour/
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/neighbour/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.769379 ifstate-1.8.4/libifstate/parser/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/parser/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/parser/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.769379 ifstate-1.8.4/libifstate/routing/
--rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/routing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.769379 ifstate-1.8.4/libifstate/sysctl/
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/sysctl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.769379 ifstate-1.8.4/libifstate/tc/
--rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/tc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.769379 ifstate-1.8.4/libifstate/wireguard/
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/wireguard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.769379 ifstate-1.8.4/libifstate/xdp/
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/xdp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.769379 ifstate-1.8.4/schema/
--rw-r--r--   0 runner    (1001) docker     (123)   178382 2023-06-08 12:56:45.000000 ifstate-1.8.4/schema/ifstate.conf.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 12:57:02.773380 ifstate-1.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-08 12:56:45.000000 ifstate-1.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.761737 ifstate-1.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 17:05:32.000000 ifstate-1.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-01 17:05:43.761737 ifstate-1.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-01 17:05:32.000000 ifstate-1.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.757737 ifstate-1.8.5/ifstate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:32.000000 ifstate-1.8.5/ifstate/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7289 2023-07-01 17:05:32.000000 ifstate-1.8.5/ifstate/ifstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-01 17:05:32.000000 ifstate-1.8.5/ifstate/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.757737 ifstate-1.8.5/ifstate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-01 17:05:43.000000 ifstate-1.8.5/ifstate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-01 17:05:43.000000 ifstate-1.8.5/ifstate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 17:05:43.000000 ifstate-1.8.5/ifstate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-01 17:05:43.000000 ifstate-1.8.5/ifstate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-01 17:05:43.000000 ifstate-1.8.5/ifstate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-01 17:05:43.000000 ifstate-1.8.5/ifstate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.757737 ifstate-1.8.5/libifstate/
+-rw-r--r--   0 runner    (1001) docker     (123)    23902 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.757737 ifstate-1.8.5/libifstate/address/
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/address/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.757737 ifstate-1.8.5/libifstate/bpf/
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/bpf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/bpf/ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10818 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/bpf/map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.757737 ifstate-1.8.5/libifstate/brport/
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/brport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.761737 ifstate-1.8.5/libifstate/link/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22757 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/link/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/link/physical.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/link/tun.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/link/veth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.761737 ifstate-1.8.5/libifstate/neighbour/
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/neighbour/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.761737 ifstate-1.8.5/libifstate/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/parser/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/parser/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.761737 ifstate-1.8.5/libifstate/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/routing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.761737 ifstate-1.8.5/libifstate/sysctl/
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/sysctl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.761737 ifstate-1.8.5/libifstate/tc/
+-rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/tc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.761737 ifstate-1.8.5/libifstate/wireguard/
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/wireguard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.761737 ifstate-1.8.5/libifstate/xdp/
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/xdp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.757737 ifstate-1.8.5/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)   178382 2023-07-01 17:05:32.000000 ifstate-1.8.5/schema/ifstate.conf.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 17:05:43.761737 ifstate-1.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-01 17:05:32.000000 ifstate-1.8.5/setup.py
```

### Comparing `ifstate-1.8.4/LICENSE` & `ifstate-1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.4/PKG-INFO` & `ifstate-1.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifstate
-Version: 1.8.4
+Version: 1.8.5
 Summary: Manage host interface settings in a declarative manner
 Home-page: https://ifstate.net/
 Author: Thomas Liske
 Author-email: thomas@fiasko-nw.net
 License: GPL3+
 Description-Content-Type: text/markdown
 Provides-Extra: shell
```

### Comparing `ifstate-1.8.4/README.md` & `ifstate-1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.4/ifstate/ifstate.py` & `ifstate-1.8.5/ifstate/ifstate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python3
 
 from libifstate.parser import YamlParser
 from libifstate import __version__, IfState
-from libifstate.exception import FeatureMissingError, LinkNoConfigFound, ParserValidationError, ParserOpenError, ParserIncludeError
+from libifstate.exception import FeatureMissingError, LinkNoConfigFound, ParserValidationError, ParserOpenError, ParserParseError, ParserIncludeError
 from libifstate.util import logger, IfStateLogging
 from collections import namedtuple
 from copy import deepcopy
+from setproctitle import setproctitle
 
 import argparse
 import logging
 import re
 import signal
 import sys
 import yaml
@@ -30,14 +31,58 @@
     "SHOW"     : "show running network config",
     "SHOWALL"  : "show running network config (more settings)",
     "VRRP"     : "run as keepalived notify script",
     "VRRP_FIFO": "run as keepalived notify_fifo_script",
     "SHELL"    : "launch interactive python shell (pyroute2)",
 }
 
+class IfsConfigHandler():
+    def __init__(self, fn, soft_schema):
+        self.fn = fn
+        self.soft_schema = soft_schema
+
+        self.ifs = self.load_config()
+
+    def sighup_handler(self, signum, frame):
+        logger.info("SIGHUP: reloading configuration")
+        try:
+            self.ifs = self.load_config()
+        except Exception:
+            pass
+
+    def load_config(self):
+        try:
+            parser = YamlParser(self.fn)
+        except ParserOpenError as ex:
+            logger.error(
+                "Config loading from {} failed: {}".format(ex.fn, ex.msg))
+            raise ex
+        except ParserParseError as ex:
+            logger.error("Config parsing failed:\n\n{}".format(str(ex)))
+            raise ex
+        except ParserIncludeError as ex:
+            logger.error(
+                "Config include file {} failed: {}".format(ex.fn, ex.msg))
+            raise ex
+
+        try:
+            ifstates = parser.config()
+
+            ifs = IfState()
+            ifs.update(ifstates, self.soft_schema)
+            return ifs
+        except ParserValidationError as ex:
+            logger.error("Config validation failed for {}".format(ex.detail))
+            raise ex
+        except FeatureMissingError as ex:
+            logger.error(
+                "Config uses unavailable feature: {}".format(ex.feature))
+            raise ex
+
+
 def shell():
     from ifstate.shell import IfStateConsole
     import pyroute2
 
     shell = IfStateConsole()
     shell.interact(banner=f"ifstate {__version__}; pyroute2 {pyroute2.__version__}")
 
@@ -78,93 +123,79 @@
     if args.verbose:
         lvl = logging.DEBUG
     elif args.quiet:
         lvl = logging.ERROR
     else:
         lvl = logging.INFO
 
+    if args.action == Actions.VRRP_FIFO:
+        setproctitle("ifstate-{}@{}".format(args.action, args.fifo))
+    else:
+        setproctitle("ifstate-{}".format(args.action))
+
     if args.action == Actions.SHELL:
         shell()
         exit(0)
 
     ifslog = IfStateLogging(lvl, action=args.action)
-    ifs = IfState()
 
     if args.action in [Actions.SHOW, Actions.SHOWALL]:
         # preserve dict order on python 3.7+
         if sys.version_info >= (3, 7):
             yaml.add_representer(
                 dict, lambda self, data: yaml.representer.SafeRepresenter.represent_dict(self, data.items()))
+        ifs = IfState()
         print(yaml.dump(ifs.show(args.action == Actions.SHOWALL)))
 
         ifslog.quit()
         exit(0)
 
     if args.action in [Actions.CHECK, Actions.APPLY, Actions.VRRP, Actions.VRRP_FIFO]:
         try:
-            parser = YamlParser(args.config)
-        except ParserOpenError as ex:
-            logger.error(
-                "Config loading from {} failed: {}".format(ex.fn, ex.msg))
-            ifslog.quit()
-            exit(1)
-        except yaml.parser.ParserError as ex:
-            logger.error("Config parsing failed:\n\n{}".format(str(ex)))
+            ifs_config = IfsConfigHandler(args.config, args.soft_schema)
+        except (ParserOpenError,
+                ParserParseError,
+                ParserIncludeError,
+                ParserValidationError,
+                FeatureMissingError) as ex:
             ifslog.quit()
-            exit(2)
-        except ParserIncludeError as ex:
-            logger.error(
-                "Config include file {} failed: {}".format(ex.fn, ex.msg))
-            ifslog.quit()
-            exit(3)
-
-        try:
-            ifstates = parser.config()
-            ifs.update(ifstates, args.soft_schema)
-        except ParserValidationError as ex:
-            logger.error("Config validation failed for {}".format(ex.detail))
-            ifslog.quit()
-            exit(4)
-        except FeatureMissingError as ex:
-            logger.error(
-                "Config uses unavailable feature: {}".format(ex.feature))
-            ifslog.quit()
-            exit(5)
+            exit(ex.exit_code())
 
         if args.action == Actions.CHECK:
             try:
-                ifs.check()
+                ifs_config.ifs.check()
             except LinkNoConfigFound:
                 pass
         elif args.action == Actions.VRRP_FIFO:
+            signal.signal(signal.SIGHUP, ifs_config.sighup_handler)
+            signal.signal(signal.SIGPIPE, signal.SIG_IGN)
+            signal.signal(signal.SIGTERM, signal.SIG_IGN)
+
             status_pattern = re.compile(
                 r'(group|instance) "([^"]+)" (unknown|fault|backup|master)( \d+)?$', re.IGNORECASE)
 
             with open(args.fifo) as fifo:
                 for line in fifo:
                     m = status_pattern.match(line.strip())
                     if m:
-                        signal.signal(signal.SIGHUP, signal.SIG_IGN)
-                        signal.signal(signal.SIGPIPE, signal.SIG_IGN)
-                        signal.signal(signal.SIGTERM, signal.SIG_IGN)
                         try:
-                            ifs_tmp = deepcopy(ifs)
+                            ifs_tmp = deepcopy(ifs_config.ifs)
                             ifs_tmp.apply(m.group(1), m.group(2), m.group(3))
                         except:
                             pass
         else:
             # ignore some well-known signals to prevent interruptions (i.e. due to ssh connection loss)
             signal.signal(signal.SIGHUP, signal.SIG_IGN)
             signal.signal(signal.SIGPIPE, signal.SIG_IGN)
             signal.signal(signal.SIGTERM, signal.SIG_IGN)
             try:
                 if args.action == Actions.APPLY:
-                    ifs.apply()
+                    ifs_config.ifs.apply()
                 elif args.action == Actions.VRRP:
-                    ifs.apply(
+                    ifs_config.ifs.apply(
                         args.type, args.name, args.state)
             except LinkNoConfigFound:
                 pass
 
         ifslog.quit()
```

### Comparing `ifstate-1.8.4/ifstate/shell.py` & `ifstate-1.8.5/ifstate/shell.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.4/ifstate.egg-info/PKG-INFO` & `ifstate-1.8.5/ifstate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifstate
-Version: 1.8.4
+Version: 1.8.5
 Summary: Manage host interface settings in a declarative manner
 Home-page: https://ifstate.net/
 Author: Thomas Liske
 Author-email: thomas@fiasko-nw.net
 License: GPL3+
 Description-Content-Type: text/markdown
 Provides-Extra: shell
```

### Comparing `ifstate-1.8.4/ifstate.egg-info/SOURCES.txt` & `ifstate-1.8.5/ifstate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.4/libifstate/__init__.py` & `ifstate-1.8.5/libifstate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 import os
 import pkgutil
 import re
 import json
 import errno
 import logging
 
-__version__ = "1.8.4"
+__version__ = "1.8.5"
 
 
 class IfState():
     def __init__(self):
         logger.debug('IfState {}'.format(__version__))
         self.links = {}
         self.addresses = {}
```

### Comparing `ifstate-1.8.4/libifstate/address/__init__.py` & `ifstate-1.8.5/libifstate/address/__init__.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.4/libifstate/bpf/__init__.py` & `ifstate-1.8.5/libifstate/bpf/__init__.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.4/libifstate/bpf/ctypes.py` & `ifstate-1.8.5/libifstate/bpf/ctypes.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.4/libifstate/bpf/map.py` & `ifstate-1.8.5/libifstate/bpf/map.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.4/libifstate/brport/__init__.py` & `ifstate-1.8.5/libifstate/brport/__init__.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.4/libifstate/exception.py` & `ifstate-1.8.5/libifstate/exception.py`

 * *Files 20% similar despite different names*

```diff
@@ -51,14 +51,17 @@
     def set_quiet(self, quiet):
         self.quiet = quiet
 
 class FeatureMissingError(Exception):
     def __init__(self, feature):
         self.feature = feature
 
+    def exit_code(self):
+        return 5
+
 
 class LinkCannotAdd(Exception):
     pass
 
 
 class LinkTypeUnknown(Exception):
     pass
@@ -75,20 +78,29 @@
 class LinkNoConfigFound(Exception):
     pass
 
 class ParserValidationError(Exception):
     def __init__(self, detail):
         self.detail = detail
 
+    def exit_code(self):
+        return 4
+
 class ParserOSError(Exception):
     def __init__(self, oserr):
         self.fn = oserr.filename
         self.msg = oserr.strerror
 
 class ParserOpenError(ParserOSError):
-    pass
+    def exit_code(self):
+        return 1
 
 class ParserIncludeError(ParserOSError):
-    pass
+    def exit_code(self):
+        return 3
+
+class ParserParseError(Exception):
+    def exit_code(self):
+        return 2
 
 class RouteDupblicate(Exception):
     pass
```

### Comparing `ifstate-1.8.4/libifstate/link/base.py` & `ifstate-1.8.5/libifstate/link/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -456,14 +456,23 @@
                 peer = self.settings.pop('peer', None)
 
                 if has_ifname_change:
                     self.prevent_altname_conflict()
 
                 try:
                     ipr.link('set', index=self.idx, **(self.settings))
+
+                    for setting in self.settings.keys():
+                        if self.get_if_attr(setting) != self.settings[setting]:
+                            if self.cap_create:
+                                logger.debug('  %s: setting could not be changed', setting, extra={'iface': self.settings['ifname']})
+                                excpts.add('set', Exception('ip link set'), **{setting: self.settings[setting]})
+                            else:
+                                logger.warning('%s setting could not be changed', setting,
+                                               extra={'iface': self.settings['ifname']})
                 except Exception as err:
                     if not isinstance(err, netlinkerror_classes):
                         raise
                     excpts.add('set', err, **(self.settings))
 
                 # restore settings
                 if state is not None:
```

### Comparing `ifstate-1.8.4/libifstate/link/physical.py` & `ifstate-1.8.5/libifstate/link/physical.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.4/libifstate/link/tun.py` & `ifstate-1.8.5/libifstate/link/tun.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.4/libifstate/link/veth.py` & `ifstate-1.8.5/libifstate/link/veth.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.4/libifstate/log.py` & `ifstate-1.8.5/libifstate/log.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.4/libifstate/neighbour/__init__.py` & `ifstate-1.8.5/libifstate/neighbour/__init__.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.4/libifstate/parser/base.py` & `ifstate-1.8.5/libifstate/parser/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from libifstate.util import logger
 from libifstate.exception import ParserValidationError
 from abc import ABC, abstractmethod
+from copy import deepcopy
 
 
 class Parser(ABC):
     _default_ifstates = {
         'ignore': {
             'ipaddr_builtin': [
                 'fe80::/10'
@@ -94,15 +95,15 @@
                         a[key] = b[key]
                 else:
                     a[key] = b[key]
         return a
 
     def config(self):
         # merge builtin defaults with config
-        cfg = (self.merge(self._default_ifstates, self.ifstates))
+        cfg = (self.merge(deepcopy(Parser._default_ifstates), self.ifstates))
 
         # 'ignore' should still be an object
         try:
             iter(cfg["ignore"])
         except TypeError:
             raise ParserValidationError("$.ignore: is not of type 'object'")
```

### Comparing `ifstate-1.8.4/libifstate/routing/__init__.py` & `ifstate-1.8.5/libifstate/routing/__init__.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.4/libifstate/sysctl/__init__.py` & `ifstate-1.8.5/libifstate/sysctl/__init__.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.4/libifstate/tc/__init__.py` & `ifstate-1.8.5/libifstate/tc/__init__.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.4/libifstate/util.py` & `ifstate-1.8.5/libifstate/util.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.4/libifstate/wireguard/__init__.py` & `ifstate-1.8.5/libifstate/wireguard/__init__.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.4/libifstate/xdp/__init__.py` & `ifstate-1.8.5/libifstate/xdp/__init__.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.4/schema/ifstate.conf.schema.json` & `ifstate-1.8.5/schema/ifstate.conf.schema.json`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.4/setup.py` & `ifstate-1.8.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,16 @@
     raise RuntimeError("Unable to find version string.")
 
 
 def install_requires():
     requires = [
         "jsonschema",
         "pyroute2",
-        "pyyaml"
+        "pyyaml",
+        "setproctitle"
     ]
 
     return requires
 
 
 setup(
     name="ifstate",
```

