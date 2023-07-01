# Comparing `tmp/cloci-0.1.1.tar.gz` & `tmp/cloci-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloci-0.1.1.tar", last modified: Sat Jul  1 02:47:04 2023, max compression
+gzip compressed data, was "cloci-0.1.2.tar", last modified: Sat Jul  1 02:48:09 2023, max compression
```

## Comparing `cloci-0.1.1.tar` & `cloci-0.1.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-07-01 02:47:04.084038 cloci-0.1.1/
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)      107 2023-07-01 02:42:18.000000 cloci-0.1.1/.gitignore
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    34207 2023-06-21 18:37:49.000000 cloci-0.1.1/LICENSE
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)    43924 2023-07-01 02:47:04.081049 cloci-0.1.1/PKG-INFO
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     3894 2023-06-21 18:37:25.000000 cloci-0.1.1/README.md
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)      740 2023-06-30 00:13:59.000000 cloci-0.1.1/TODO.md
-drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-07-01 02:47:03.861047 cloci-0.1.1/archive/
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    73986 2023-04-12 16:22:58.000000 cloci-0.1.1/archive/hgx2gcfs.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    74097 2023-04-12 16:22:58.000000 cloci-0.1.1/archive/hgx2hlgs.py
-drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-07-01 02:47:03.866049 cloci-0.1.1/cloci/
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    46352 2023-07-01 02:39:13.000000 cloci-0.1.1/cloci/cloci.py
-drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-07-01 02:47:03.976043 cloci-0.1.1/cloci/lib/
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-04-17 04:15:01.000000 cloci-0.1.1/cloci/lib/__init__.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    27794 2023-06-28 00:57:46.000000 cloci-0.1.1/cloci/lib/evo_conco.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    18698 2023-06-28 00:57:46.000000 cloci-0.1.1/cloci/lib/generate_nulls.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    16702 2023-06-28 00:57:46.000000 cloci-0.1.1/cloci/lib/hgp2hgx.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    74248 2023-07-01 02:46:40.000000 cloci-0.1.1/cloci/lib/hgx2hlgs.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    36251 2023-05-30 17:06:24.000000 cloci-0.1.1/cloci/lib/input_parsing.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    37967 2023-06-30 16:53:27.000000 cloci-0.1.1/cloci/lib/output_data.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     7114 2023-05-30 17:03:59.000000 cloci-0.1.1/cloci/lib/treecalcs.py
-drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-07-01 02:47:04.026039 cloci-0.1.1/cloci/tools/
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-07-01 02:39:38.000000 cloci-0.1.1/cloci/tools/__init__.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    23167 2023-07-01 02:39:15.000000 cloci-0.1.1/cloci/tools/cloci2enrich.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    13966 2023-07-01 02:39:16.000000 cloci-0.1.1/cloci/tools/cloci2stats.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    16906 2023-07-01 02:39:22.000000 cloci-0.1.1/cloci/tools/hg2hg_net.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     9825 2023-07-01 02:39:16.000000 cloci-0.1.1/cloci/tools/hlg2biofile.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    17264 2023-07-01 02:39:16.000000 cloci-0.1.1/cloci/tools/hlg2hlg_net.py
-drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-07-01 02:47:03.924047 cloci-0.1.1/cloci.egg-info/
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)    43924 2023-07-01 02:47:03.000000 cloci-0.1.1/cloci.egg-info/PKG-INFO
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)      684 2023-07-01 02:47:03.000000 cloci-0.1.1/cloci.egg-info/SOURCES.txt
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)        1 2023-07-01 02:47:03.000000 cloci-0.1.1/cloci.egg-info/dependency_links.txt
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)      250 2023-07-01 02:47:03.000000 cloci-0.1.1/cloci.egg-info/entry_points.txt
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)       23 2023-07-01 02:47:03.000000 cloci-0.1.1/cloci.egg-info/requires.txt
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)        6 2023-07-01 02:47:03.000000 cloci-0.1.1/cloci.egg-info/top_level.txt
-drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-07-01 02:47:04.076041 cloci-0.1.1/etc/
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)    75323 2023-06-16 22:03:00.000000 cloci-0.1.1/etc/boundaries.png
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)   307022 2023-06-16 22:03:00.000000 cloci-0.1.1/etc/pipeline.png
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)    42013 2023-06-16 22:03:00.000000 cloci-0.1.1/etc/recovery.png
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     1217 2023-07-01 02:46:50.000000 cloci-0.1.1/pyproject.toml
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)       38 2023-07-01 02:47:04.084067 cloci-0.1.1/setup.cfg
+drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-07-01 02:48:09.083149 cloci-0.1.2/
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)      107 2023-07-01 02:42:18.000000 cloci-0.1.2/.gitignore
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    34207 2023-06-21 18:37:49.000000 cloci-0.1.2/LICENSE
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)    43924 2023-07-01 02:48:09.081150 cloci-0.1.2/PKG-INFO
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     3894 2023-06-21 18:37:25.000000 cloci-0.1.2/README.md
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)      740 2023-06-30 00:13:59.000000 cloci-0.1.2/TODO.md
+drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-07-01 02:48:08.839162 cloci-0.1.2/archive/
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    73986 2023-04-12 16:22:58.000000 cloci-0.1.2/archive/hgx2gcfs.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    74097 2023-04-12 16:22:58.000000 cloci-0.1.2/archive/hgx2hlgs.py
+drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-07-01 02:48:08.862160 cloci-0.1.2/cloci/
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    46352 2023-07-01 02:39:13.000000 cloci-0.1.2/cloci/cloci.py
+drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-07-01 02:48:09.023160 cloci-0.1.2/cloci/lib/
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-04-17 04:15:01.000000 cloci-0.1.2/cloci/lib/__init__.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    27794 2023-06-28 00:57:46.000000 cloci-0.1.2/cloci/lib/evo_conco.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    18698 2023-06-28 00:57:46.000000 cloci-0.1.2/cloci/lib/generate_nulls.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    16702 2023-06-28 00:57:46.000000 cloci-0.1.2/cloci/lib/hgp2hgx.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    74248 2023-07-01 02:46:40.000000 cloci-0.1.2/cloci/lib/hgx2hlgs.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    36251 2023-05-30 17:06:24.000000 cloci-0.1.2/cloci/lib/input_parsing.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    37967 2023-06-30 16:53:27.000000 cloci-0.1.2/cloci/lib/output_data.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     7114 2023-05-30 17:03:59.000000 cloci-0.1.2/cloci/lib/treecalcs.py
+drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-07-01 02:48:09.064150 cloci-0.1.2/cloci/tools/
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-07-01 02:39:38.000000 cloci-0.1.2/cloci/tools/__init__.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    23167 2023-07-01 02:39:15.000000 cloci-0.1.2/cloci/tools/cloci2enrich.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    13966 2023-07-01 02:39:16.000000 cloci-0.1.2/cloci/tools/cloci2stats.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    16906 2023-07-01 02:39:22.000000 cloci-0.1.2/cloci/tools/hg2hg_net.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     9825 2023-07-01 02:39:16.000000 cloci-0.1.2/cloci/tools/hlg2biofile.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    17264 2023-07-01 02:39:16.000000 cloci-0.1.2/cloci/tools/hlg2hlg_net.py
+drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-07-01 02:48:08.959156 cloci-0.1.2/cloci.egg-info/
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)    43924 2023-07-01 02:48:08.000000 cloci-0.1.2/cloci.egg-info/PKG-INFO
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)      684 2023-07-01 02:48:08.000000 cloci-0.1.2/cloci.egg-info/SOURCES.txt
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)        1 2023-07-01 02:48:08.000000 cloci-0.1.2/cloci.egg-info/dependency_links.txt
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)      250 2023-07-01 02:48:08.000000 cloci-0.1.2/cloci.egg-info/entry_points.txt
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)       30 2023-07-01 02:48:08.000000 cloci-0.1.2/cloci.egg-info/requires.txt
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)        6 2023-07-01 02:48:08.000000 cloci-0.1.2/cloci.egg-info/top_level.txt
+drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2023-07-01 02:48:09.077152 cloci-0.1.2/etc/
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)    75323 2023-06-16 22:03:00.000000 cloci-0.1.2/etc/boundaries.png
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)   307022 2023-06-16 22:03:00.000000 cloci-0.1.2/etc/pipeline.png
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)    42013 2023-06-16 22:03:00.000000 cloci-0.1.2/etc/recovery.png
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     1227 2023-07-01 02:47:56.000000 cloci-0.1.2/pyproject.toml
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)       38 2023-07-01 02:48:09.084150 cloci-0.1.2/setup.cfg
```

### Comparing `cloci-0.1.1/LICENSE` & `cloci-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cloci-0.1.1/PKG-INFO` & `cloci-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloci
-Version: 0.1.1
+Version: 0.1.2
 Summary: Co-occurrence Locus and Orthologous Cluster Identifier
 Author-email: Zachary Konkel <konkelzach@protonmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `cloci-0.1.1/README.md` & `cloci-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cloci-0.1.1/TODO.md` & `cloci-0.1.2/TODO.md`

 * *Files identical despite different names*

### Comparing `cloci-0.1.1/archive/hgx2gcfs.py` & `cloci-0.1.2/archive/hgx2gcfs.py`

 * *Files identical despite different names*

### Comparing `cloci-0.1.1/archive/hgx2hlgs.py` & `cloci-0.1.2/archive/hgx2hlgs.py`

 * *Files identical despite different names*

### Comparing `cloci-0.1.1/cloci/cloci.py` & `cloci-0.1.2/cloci/cloci.py`

 * *Files identical despite different names*

### Comparing `cloci-0.1.1/cloci/lib/evo_conco.py` & `cloci-0.1.2/cloci/lib/evo_conco.py`

 * *Files identical despite different names*

### Comparing `cloci-0.1.1/cloci/lib/generate_nulls.py` & `cloci-0.1.2/cloci/lib/generate_nulls.py`

 * *Files identical despite different names*

### Comparing `cloci-0.1.1/cloci/lib/hgp2hgx.py` & `cloci-0.1.2/cloci/lib/hgp2hgx.py`

 * *Files identical despite different names*

### Comparing `cloci-0.1.1/cloci/lib/hgx2hlgs.py` & `cloci-0.1.2/cloci/lib/hgx2hlgs.py`

 * *Files identical despite different names*

### Comparing `cloci-0.1.1/cloci/lib/input_parsing.py` & `cloci-0.1.2/cloci/lib/input_parsing.py`

 * *Files identical despite different names*

### Comparing `cloci-0.1.1/cloci/lib/output_data.py` & `cloci-0.1.2/cloci/lib/output_data.py`

 * *Files identical despite different names*

### Comparing `cloci-0.1.1/cloci/lib/treecalcs.py` & `cloci-0.1.2/cloci/lib/treecalcs.py`

 * *Files identical despite different names*

### Comparing `cloci-0.1.1/cloci/tools/cloci2enrich.py` & `cloci-0.1.2/cloci/tools/cloci2enrich.py`

 * *Files identical despite different names*

### Comparing `cloci-0.1.1/cloci/tools/cloci2stats.py` & `cloci-0.1.2/cloci/tools/cloci2stats.py`

 * *Files identical despite different names*

### Comparing `cloci-0.1.1/cloci/tools/hg2hg_net.py` & `cloci-0.1.2/cloci/tools/hg2hg_net.py`

 * *Files identical despite different names*

### Comparing `cloci-0.1.1/cloci/tools/hlg2biofile.py` & `cloci-0.1.2/cloci/tools/hlg2biofile.py`

 * *Files identical despite different names*

### Comparing `cloci-0.1.1/cloci/tools/hlg2hlg_net.py` & `cloci-0.1.2/cloci/tools/hlg2hlg_net.py`

 * *Files identical despite different names*

### Comparing `cloci-0.1.1/cloci.egg-info/PKG-INFO` & `cloci-0.1.2/cloci.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloci
-Version: 0.1.1
+Version: 0.1.2
 Summary: Co-occurrence Locus and Orthologous Cluster Identifier
 Author-email: Zachary Konkel <konkelzach@protonmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `cloci-0.1.1/cloci.egg-info/SOURCES.txt` & `cloci-0.1.2/cloci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloci-0.1.1/etc/boundaries.png` & `cloci-0.1.2/etc/boundaries.png`

 * *Files identical despite different names*

### Comparing `cloci-0.1.1/etc/pipeline.png` & `cloci-0.1.2/etc/pipeline.png`

 * *Files identical despite different names*

### Comparing `cloci-0.1.1/etc/recovery.png` & `cloci-0.1.2/etc/recovery.png`

 * *Files identical despite different names*

### Comparing `cloci-0.1.1/pyproject.toml` & `cloci-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cloci"
-version = "0.01.1"
+version = "0.01.2"
 authors = [{name="Zachary Konkel", email="konkelzach@protonmail.com"}]
 description = "Co-occurrence Locus and Orthologous Cluster Identifier"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = '>=3.0,<4'
-dependencies = ['mycotools', 'cogent3', 'tqdm']
+dependencies = ['mycotools', 'cogent3', 'tqdm', 'plotly']
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
     "Operating System :: POSIX :: Linux",
 ]
 
 [project.urls]
```

