# Comparing `tmp/flux-burst-gke-0.0.0.tar.gz` & `tmp/flux-burst-gke-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-burst-gke-0.0.0.tar", last modified: Sun Jun 25 03:12:35 2023, max compression
+gzip compressed data, was "flux-burst-gke-0.0.1.tar", last modified: Sat Jul  1 07:04:00 2023, max compression
```

## Comparing `flux-burst-gke-0.0.0.tar` & `flux-burst-gke-0.0.1.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 03:12:35.729155 flux-burst-gke-0.0.0/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-06-24 19:35:42.000000 flux-burst-gke-0.0.0/COPYRIGHT
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-06-24 19:35:39.000000 flux-burst-gke-0.0.0/LICENSE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      215 2023-06-23 23:45:36.000000 flux-burst-gke-0.0.0/MANIFEST.in
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-06-24 19:35:45.000000 flux-burst-gke-0.0.0/NOTICE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1501 2023-06-25 03:12:35.729155 flux-burst-gke-0.0.0/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      683 2023-06-24 19:36:41.000000 flux-burst-gke-0.0.0/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 03:12:35.729155 flux-burst-gke-0.0.0/flux_burst_gke.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1501 2023-06-25 03:12:35.000000 flux-burst-gke-0.0.0/flux_burst_gke.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      432 2023-06-25 03:12:35.000000 flux-burst-gke-0.0.0/flux_burst_gke.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-25 03:12:35.000000 flux-burst-gke-0.0.0/flux_burst_gke.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-25 03:12:35.000000 flux-burst-gke-0.0.0/flux_burst_gke.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      109 2023-06-25 03:12:35.000000 flux-burst-gke-0.0.0/flux_burst_gke.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       14 2023-06-25 03:12:35.000000 flux-burst-gke-0.0.0/flux_burst_gke.egg-info/top_level.txt
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 03:12:35.729155 flux-burst-gke-0.0.0/fluxburst_gke/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      624 2023-06-25 03:11:54.000000 flux-burst-gke-0.0.0/fluxburst_gke/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5065 2023-06-25 03:11:54.000000 flux-burst-gke-0.0.0/fluxburst_gke/cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      337 2023-06-24 05:32:09.000000 flux-burst-gke-0.0.0/fluxburst_gke/defaults.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    11847 2023-06-25 03:12:09.000000 flux-burst-gke-0.0.0/fluxburst_gke/plugin.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1130 2023-06-24 05:30:10.000000 flux-burst-gke-0.0.0/fluxburst_gke/version.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-06-23 23:28:22.000000 flux-burst-gke-0.0.0/pyproject.toml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      157 2023-06-25 03:12:35.729155 flux-burst-gke-0.0.0/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3162 2023-06-24 19:36:42.000000 flux-burst-gke-0.0.0/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 07:04:00.672516 flux-burst-gke-0.0.1/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-06-24 19:35:42.000000 flux-burst-gke-0.0.1/COPYRIGHT
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-06-24 19:35:39.000000 flux-burst-gke-0.0.1/LICENSE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      215 2023-06-23 23:45:36.000000 flux-burst-gke-0.0.1/MANIFEST.in
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-06-24 19:35:45.000000 flux-burst-gke-0.0.1/NOTICE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1837 2023-07-01 07:04:00.672516 flux-burst-gke-0.0.1/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1019 2023-07-01 07:03:06.000000 flux-burst-gke-0.0.1/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 07:04:00.672516 flux-burst-gke-0.0.1/flux_burst_gke.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1837 2023-07-01 07:04:00.000000 flux-burst-gke-0.0.1/flux_burst_gke.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      381 2023-07-01 07:04:00.000000 flux-burst-gke-0.0.1/flux_burst_gke.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-01 07:04:00.000000 flux-burst-gke-0.0.1/flux_burst_gke.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-25 03:12:35.000000 flux-burst-gke-0.0.1/flux_burst_gke.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      109 2023-07-01 07:04:00.000000 flux-burst-gke-0.0.1/flux_burst_gke.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       14 2023-07-01 07:04:00.000000 flux-burst-gke-0.0.1/flux_burst_gke.egg-info/top_level.txt
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 07:04:00.672516 flux-burst-gke-0.0.1/fluxburst_gke/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      624 2023-06-25 03:11:54.000000 flux-burst-gke-0.0.1/fluxburst_gke/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5590 2023-07-01 07:03:06.000000 flux-burst-gke-0.0.1/fluxburst_gke/plugin.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1130 2023-07-01 07:03:34.000000 flux-burst-gke-0.0.1/fluxburst_gke/version.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-06-23 23:28:22.000000 flux-burst-gke-0.0.1/pyproject.toml
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      157 2023-07-01 07:04:00.672516 flux-burst-gke-0.0.1/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3162 2023-06-24 19:36:42.000000 flux-burst-gke-0.0.1/setup.py
```

### Comparing `flux-burst-gke-0.0.0/LICENSE` & `flux-burst-gke-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-burst-gke-0.0.0/NOTICE` & `flux-burst-gke-0.0.1/NOTICE`

 * *Files identical despite different names*

### Comparing `flux-burst-gke-0.0.0/PKG-INFO` & `flux-burst-gke-0.0.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-burst-gke
-Version: 0.0.0
+Version: 0.0.1
 Summary: A bursting plugin for Flux and GKE
 Home-page: https://github.com/converged-computing/flux-burst-gke
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: flux,flux-framework,workflow,example,plugin
@@ -22,14 +22,18 @@
 License-File: LICENSE
 License-File: NOTICE
 
 # Flux Burst Plugin for GKE
 
 This is an example implementation for an external bursting plugin for Flux.
 For instructions, see the [main flux-burst repository](https://github.com/converged-computing/flux-burst).
+Tutorials are available under the [flux operator](https://github.com/flux-framework/flux-operator/tree/main/examples/experimental/bursting)
+
+![https://raw.githubusercontent.com/converged-computing/flux-burst/main/docs/assets/img/logo.png](https://raw.githubusercontent.com/converged-computing/flux-burst/main/docs/assets/img/logo.png)
+
 
 **under development**
 
 ## License
 
 HPCIC DevTools is distributed under the terms of the MIT license.
 All new contributions must be made under this license.
```

### Comparing `flux-burst-gke-0.0.0/README.md` & `flux-burst-gke-0.0.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Flux Burst Plugin for GKE
 
 This is an example implementation for an external bursting plugin for Flux.
 For instructions, see the [main flux-burst repository](https://github.com/converged-computing/flux-burst).
+Tutorials are available under the [flux operator](https://github.com/flux-framework/flux-operator/tree/main/examples/experimental/bursting)
+
+![https://raw.githubusercontent.com/converged-computing/flux-burst/main/docs/assets/img/logo.png](https://raw.githubusercontent.com/converged-computing/flux-burst/main/docs/assets/img/logo.png)
+
 
 **under development**
 
 ## License
 
 HPCIC DevTools is distributed under the terms of the MIT license.
 All new contributions must be made under this license.
```

### Comparing `flux-burst-gke-0.0.0/flux_burst_gke.egg-info/PKG-INFO` & `flux-burst-gke-0.0.1/flux_burst_gke.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-burst-gke
-Version: 0.0.0
+Version: 0.0.1
 Summary: A bursting plugin for Flux and GKE
 Home-page: https://github.com/converged-computing/flux-burst-gke
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: flux,flux-framework,workflow,example,plugin
@@ -22,14 +22,18 @@
 License-File: LICENSE
 License-File: NOTICE
 
 # Flux Burst Plugin for GKE
 
 This is an example implementation for an external bursting plugin for Flux.
 For instructions, see the [main flux-burst repository](https://github.com/converged-computing/flux-burst).
+Tutorials are available under the [flux operator](https://github.com/flux-framework/flux-operator/tree/main/examples/experimental/bursting)
+
+![https://raw.githubusercontent.com/converged-computing/flux-burst/main/docs/assets/img/logo.png](https://raw.githubusercontent.com/converged-computing/flux-burst/main/docs/assets/img/logo.png)
+
 
 **under development**
 
 ## License
 
 HPCIC DevTools is distributed under the terms of the MIT license.
 All new contributions must be made under this license.
```

### Comparing `flux-burst-gke-0.0.0/fluxburst_gke/__init__.py` & `flux-burst-gke-0.0.1/fluxburst_gke/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-burst-gke-0.0.0/fluxburst_gke/version.py` & `flux-burst-gke-0.0.1/fluxburst_gke/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2023 Lawrence Livermore National Security, LLC and other
 # HPCIC DevTools Developers. See the top-level COPYRIGHT file for details.
 #
 # SPDX-License-Identifier: (MIT)
 
-__version__ = "0.0.0"
+__version__ = "0.0.1"
 AUTHOR = "Vanessa Sochat"
 EMAIL = "vsoch@users.noreply.github.com"
 NAME = "flux-burst-gke"
 PACKAGE_URL = "https://github.com/converged-computing/flux-burst-gke"
 KEYWORDS = "flux, flux-framework, workflow, example, plugin"
 DESCRIPTION = "A bursting plugin for Flux and GKE"
 LICENSE = "LICENSE"
```

### Comparing `flux-burst-gke-0.0.0/setup.py` & `flux-burst-gke-0.0.1/setup.py`

 * *Files identical despite different names*

