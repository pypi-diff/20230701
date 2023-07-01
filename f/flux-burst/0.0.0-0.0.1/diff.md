# Comparing `tmp/flux-burst-0.0.0.tar.gz` & `tmp/flux-burst-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-burst-0.0.0.tar", last modified: Sun Jun 25 03:17:14 2023, max compression
+gzip compressed data, was "flux-burst-0.0.1.tar", last modified: Sat Jul  1 06:52:49 2023, max compression
```

## Comparing `flux-burst-0.0.0.tar` & `flux-burst-0.0.1.tar`

### file list

```diff
@@ -1,32 +1,37 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 03:17:14.214355 flux-burst-0.0.0/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-06-23 19:26:31.000000 flux-burst-0.0.0/COPYRIGHT
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-06-23 19:26:31.000000 flux-burst-0.0.0/LICENSE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      313 2023-06-23 19:45:55.000000 flux-burst-0.0.0/MANIFEST.in
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-06-23 19:26:31.000000 flux-burst-0.0.0/NOTICE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13359 2023-06-25 03:17:14.214355 flux-burst-0.0.0/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12549 2023-06-25 03:17:09.000000 flux-burst-0.0.0/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 03:17:14.210355 flux-burst-0.0.0/flux_burst.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13359 2023-06-25 03:17:14.000000 flux-burst-0.0.0/flux_burst.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      595 2023-06-25 03:17:14.000000 flux-burst-0.0.0/flux_burst.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-25 03:17:14.000000 flux-burst-0.0.0/flux_burst.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       53 2023-06-25 03:17:14.000000 flux-burst-0.0.0/flux_burst.egg-info/entry_points.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-25 03:17:14.000000 flux-burst-0.0.0/flux_burst.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      115 2023-06-25 03:17:14.000000 flux-burst-0.0.0/flux_burst.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       10 2023-06-25 03:17:14.000000 flux-burst-0.0.0/flux_burst.egg-info/top_level.txt
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 03:17:14.210355 flux-burst-0.0.0/fluxburst/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       62 2023-06-23 19:45:55.000000 flux-burst-0.0.0/fluxburst/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7971 2023-06-25 03:17:09.000000 flux-burst-0.0.0/fluxburst/client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      577 2023-06-23 20:10:49.000000 flux-burst-0.0.0/fluxburst/defaults.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6127 2023-06-23 19:43:36.000000 flux-burst-0.0.0/fluxburst/logger.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2430 2023-06-25 03:17:09.000000 flux-burst-0.0.0/fluxburst/plugins.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      365 2023-06-24 04:45:23.000000 flux-burst-0.0.0/fluxburst/selectors.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      444 2023-06-24 04:45:23.000000 flux-burst-0.0.0/fluxburst/sorting.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 03:17:14.214355 flux-burst-0.0.0/fluxburst/utils/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      540 2023-06-23 19:26:33.000000 flux-burst-0.0.0/fluxburst/utils/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6250 2023-06-23 19:45:55.000000 flux-burst-0.0.0/fluxburst/utils/fileio.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1692 2023-06-23 19:41:30.000000 flux-burst-0.0.0/fluxburst/utils/misc.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3188 2023-06-23 19:45:55.000000 flux-burst-0.0.0/fluxburst/utils/terminal.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1109 2023-06-23 20:19:17.000000 flux-burst-0.0.0/fluxburst/version.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-06-23 19:26:31.000000 flux-burst-0.0.0/pyproject.toml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      371 2023-06-25 03:17:14.214355 flux-burst-0.0.0/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3440 2023-06-23 20:19:45.000000 flux-burst-0.0.0/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 06:52:49.261483 flux-burst-0.0.1/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-06-23 19:26:31.000000 flux-burst-0.0.1/COPYRIGHT
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-06-23 19:26:31.000000 flux-burst-0.0.1/LICENSE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      313 2023-06-23 19:45:55.000000 flux-burst-0.0.1/MANIFEST.in
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-06-23 19:26:31.000000 flux-burst-0.0.1/NOTICE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4499 2023-07-01 06:52:49.261483 flux-burst-0.0.1/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3662 2023-06-25 21:04:01.000000 flux-burst-0.0.1/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 06:52:49.261483 flux-burst-0.0.1/flux_burst.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4499 2023-07-01 06:52:49.000000 flux-burst-0.0.1/flux_burst.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      723 2023-07-01 06:52:49.000000 flux-burst-0.0.1/flux_burst.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-01 06:52:49.000000 flux-burst-0.0.1/flux_burst.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       53 2023-07-01 06:52:49.000000 flux-burst-0.0.1/flux_burst.egg-info/entry_points.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-25 03:17:14.000000 flux-burst-0.0.1/flux_burst.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      177 2023-07-01 06:52:49.000000 flux-burst-0.0.1/flux_burst.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       10 2023-07-01 06:52:49.000000 flux-burst-0.0.1/flux_burst.egg-info/top_level.txt
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 06:52:49.261483 flux-burst-0.0.1/fluxburst/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       62 2023-06-23 19:45:55.000000 flux-burst-0.0.1/fluxburst/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7997 2023-07-01 06:52:00.000000 flux-burst-0.0.1/fluxburst/client.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      746 2023-07-01 06:52:00.000000 flux-burst-0.0.1/fluxburst/defaults.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 06:52:49.261483 flux-burst-0.0.1/fluxburst/kubernetes/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      209 2023-07-01 06:52:00.000000 flux-burst-0.0.1/fluxburst/kubernetes/README.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       43 2023-07-01 06:52:00.000000 flux-burst-0.0.1/fluxburst/kubernetes/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5061 2023-07-01 06:52:00.000000 flux-burst-0.0.1/fluxburst/kubernetes/cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6537 2023-07-01 06:52:00.000000 flux-burst-0.0.1/fluxburst/kubernetes/plugins.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6127 2023-06-23 19:43:36.000000 flux-burst-0.0.1/fluxburst/logger.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2430 2023-06-30 06:24:43.000000 flux-burst-0.0.1/fluxburst/plugins.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      365 2023-06-24 04:45:23.000000 flux-burst-0.0.1/fluxburst/selectors.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      444 2023-06-24 04:45:23.000000 flux-burst-0.0.1/fluxburst/sorting.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 06:52:49.261483 flux-burst-0.0.1/fluxburst/utils/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      540 2023-06-23 19:26:33.000000 flux-burst-0.0.1/fluxburst/utils/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6250 2023-06-23 19:45:55.000000 flux-burst-0.0.1/fluxburst/utils/fileio.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1692 2023-06-23 19:41:30.000000 flux-burst-0.0.1/fluxburst/utils/misc.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3188 2023-06-23 19:45:55.000000 flux-burst-0.0.1/fluxburst/utils/terminal.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1262 2023-07-01 06:52:09.000000 flux-burst-0.0.1/fluxburst/version.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-06-23 19:26:31.000000 flux-burst-0.0.1/pyproject.toml
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      210 2023-07-01 06:52:49.261483 flux-burst-0.0.1/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3578 2023-07-01 06:52:00.000000 flux-burst-0.0.1/setup.py
```

### Comparing `flux-burst-0.0.0/LICENSE` & `flux-burst-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.0/NOTICE` & `flux-burst-0.0.1/NOTICE`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.0/flux_burst.egg-info/SOURCES.txt` & `flux-burst-0.0.1/flux_burst.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -17,11 +17,15 @@
 fluxburst/client.py
 fluxburst/defaults.py
 fluxburst/logger.py
 fluxburst/plugins.py
 fluxburst/selectors.py
 fluxburst/sorting.py
 fluxburst/version.py
+fluxburst/kubernetes/README.md
+fluxburst/kubernetes/__init__.py
+fluxburst/kubernetes/cluster.py
+fluxburst/kubernetes/plugins.py
 fluxburst/utils/__init__.py
 fluxburst/utils/fileio.py
 fluxburst/utils/misc.py
 fluxburst/utils/terminal.py
```

### Comparing `flux-burst-0.0.0/fluxburst/client.py` & `flux-burst-0.0.1/fluxburst/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,14 +144,15 @@
             for _, plugin in self.iter_plugins():
                 # Give to first burstable plugin that can accept
                 if plugin.schedule(job):
                     # Remove the burstable attribute so it isn't assigned to another
                     # This is more for development - we could likely use a better way
                     self.mark_as_scheduled(job, plugin.name)
                     scheduled = True
+                    break
 
             # But if we cannot match, return to caller
             if not scheduled:
                 unmatched.append(job)
 
         if unmatched:
             logger.warning(f"There are {len(unmatched)} jobs that cannot be bursted.")
```

### Comparing `flux-burst-0.0.0/fluxburst/logger.py` & `flux-burst-0.0.1/fluxburst/logger.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.0/fluxburst/plugins.py` & `flux-burst-0.0.1/fluxburst/plugins.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.0/fluxburst/utils/__init__.py` & `flux-burst-0.0.1/fluxburst/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.0/fluxburst/utils/fileio.py` & `flux-burst-0.0.1/fluxburst/utils/fileio.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.0/fluxburst/utils/misc.py` & `flux-burst-0.0.1/fluxburst/utils/misc.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.0/fluxburst/utils/terminal.py` & `flux-burst-0.0.1/fluxburst/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.0/fluxburst/version.py` & `flux-burst-0.0.1/fluxburst/version.py`

 * *Files 5% similar despite different names*

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
 NAME = "flux-burst"
 PACKAGE_URL = "https://github.com/converged-computing/flux-burst"
 KEYWORDS = "cloud, flux-framework, flux, bursting"
 DESCRIPTION = "Flux module that enables burstable plugins."
 LICENSE = "LICENSE"
@@ -20,13 +20,18 @@
     ("jsonschema", {"min_version": None}),
     ("rich", {"min_version": None}),
     ("oras", {"min_version": None}),
     ("requests", {"min_version": None}),
     ("pick", {"min_version": None}),
 )
 
+INSTALL_REQUIRES_KUBERNETES = (
+    ("kubernetes", {"min_version": None}),
+    ("fluxoperator", {"min_version": None}),
+)
+
 TESTS_REQUIRES = (("pytest", {"min_version": "4.6.2"}),)
 
 ################################################################################
 # Submodule Requirements (versions that include database)
 
-INSTALL_REQUIRES_ALL = INSTALL_REQUIRES + TESTS_REQUIRES
+INSTALL_REQUIRES_ALL = INSTALL_REQUIRES + INSTALL_REQUIRES_KUBERNETES + TESTS_REQUIRES
```

### Comparing `flux-burst-0.0.0/setup.py` & `flux-burst-0.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 # MAIN #########################################################################
 ################################################################################
 
 if __name__ == "__main__":
     INSTALL_REQUIRES = get_reqs(lookup)
     TESTS_REQUIRES = get_reqs(lookup, "TESTS_REQUIRES")
     INSTALL_REQUIRES_ALL = get_reqs(lookup, "INSTALL_REQUIRES_ALL")
-
+    INSTALL_REQUIRES_KUBERNETES = get_reqs(lookup, "INSTALL_REQUIRES_KUBERNETES")
     setup(
         name=NAME,
         version=VERSION,
         author=AUTHOR,
         author_email=EMAIL,
         maintainer=AUTHOR,
         packages=find_packages(),
@@ -88,14 +88,15 @@
         long_description_content_type="text/markdown",
         keywords=KEYWORDS,
         setup_requires=["pytest-runner"],
         install_requires=INSTALL_REQUIRES,
         tests_require=TESTS_REQUIRES,
         extras_require={
             "all": [INSTALL_REQUIRES_ALL],
+            "kubernetes": [INSTALL_REQUIRES_KUBERNETES],
         },
         classifiers=[
             "Intended Audience :: Science/Research",
             "Intended Audience :: Developers",
             "License :: OSI Approved :: MIT License",
             "Programming Language :: Python",
             "Topic :: Software Development",
```

