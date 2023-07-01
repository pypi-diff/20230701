# Comparing `tmp/chroma_datasets-0.1.1.tar.gz` & `tmp/chroma_datasets-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chroma_datasets-0.1.1.tar", last modified: Thu Jun 29 00:07:50 2023, max compression
+gzip compressed data, was "chroma_datasets-0.1.2.tar", last modified: Sat Jul  1 21:32:37 2023, max compression
```

## Comparing `chroma_datasets-0.1.1.tar` & `chroma_datasets-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,35 @@
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-06-29 00:07:50.645078 chroma_datasets-0.1.1/
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-06-29 00:07:50.639825 chroma_datasets-0.1.1/.chroma/
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-06-29 00:07:50.643850 chroma_datasets-0.1.1/.chroma/index/
--rw-r--r--   0 jeff       (501) staff       (20)    35646 2023-06-28 23:55:25.000000 chroma_datasets-0.1.1/.chroma/index/id_to_uuid_67fbb097-2cd8-47fd-88d8-1e73045b3d26.pkl
--rw-r--r--   0 jeff       (501) staff       (20)    35639 2023-06-29 00:01:33.000000 chroma_datasets-0.1.1/.chroma/index/id_to_uuid_72651421-1dac-4dd2-83a1-d5754e43606e.pkl
--rw-r--r--   0 jeff       (501) staff       (20)  1859576 2023-06-28 23:55:25.000000 chroma_datasets-0.1.1/.chroma/index/index_67fbb097-2cd8-47fd-88d8-1e73045b3d26.bin
--rw-r--r--   0 jeff       (501) staff       (20)  1859576 2023-06-29 00:01:33.000000 chroma_datasets-0.1.1/.chroma/index/index_72651421-1dac-4dd2-83a1-d5754e43606e.bin
--rw-r--r--   0 jeff       (501) staff       (20)      105 2023-06-28 23:55:25.000000 chroma_datasets-0.1.1/.chroma/index/index_metadata_67fbb097-2cd8-47fd-88d8-1e73045b3d26.pkl
--rw-r--r--   0 jeff       (501) staff       (20)      105 2023-06-29 00:01:33.000000 chroma_datasets-0.1.1/.chroma/index/index_metadata_72651421-1dac-4dd2-83a1-d5754e43606e.pkl
--rw-r--r--   0 jeff       (501) staff       (20)    41715 2023-06-28 23:55:25.000000 chroma_datasets-0.1.1/.chroma/index/uuid_to_id_67fbb097-2cd8-47fd-88d8-1e73045b3d26.pkl
--rw-r--r--   0 jeff       (501) staff       (20)    41715 2023-06-29 00:01:33.000000 chroma_datasets-0.1.1/.chroma/index/uuid_to_id_72651421-1dac-4dd2-83a1-d5754e43606e.pkl
--rw-r--r--   0 jeff       (501) staff       (20)    11357 2023-06-28 23:45:35.000000 chroma_datasets-0.1.1/LICENSE.md
--rw-r--r--   0 jeff       (501) staff       (20)      644 2023-06-29 00:07:50.644934 chroma_datasets-0.1.1/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)       70 2023-06-29 00:06:00.000000 chroma_datasets-0.1.1/README.md
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-06-29 00:07:50.643999 chroma_datasets-0.1.1/bin/
--rw-r--r--   0 jeff       (501) staff       (20)      151 2023-06-28 23:46:19.000000 chroma_datasets-0.1.1/bin/version
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-06-29 00:07:50.644138 chroma_datasets-0.1.1/chroma_datasets/
--rw-r--r--   0 jeff       (501) staff       (20)     2115 2023-06-29 00:07:24.000000 chroma_datasets-0.1.1/chroma_datasets/__init__.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-06-29 00:07:50.644757 chroma_datasets-0.1.1/chroma_datasets/__pycache__/
--rw-r--r--   0 jeff       (501) staff       (20)      312 2023-06-28 23:49:38.000000 chroma_datasets-0.1.1/chroma_datasets/__pycache__/__init__.cpython-310.pyc
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-06-29 00:07:50.644642 chroma_datasets-0.1.1/chroma_datasets.egg-info/
--rw-r--r--   0 jeff       (501) staff       (20)      644 2023-06-29 00:07:50.000000 chroma_datasets-0.1.1/chroma_datasets.egg-info/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)      838 2023-06-29 00:07:50.000000 chroma_datasets-0.1.1/chroma_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 jeff       (501) staff       (20)        1 2023-06-29 00:07:50.000000 chroma_datasets-0.1.1/chroma_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 jeff       (501) staff       (20)       16 2023-06-29 00:07:50.000000 chroma_datasets-0.1.1/chroma_datasets.egg-info/top_level.txt
--rw-r--r--   0 jeff       (501) staff       (20)      808 2023-06-29 00:07:03.000000 chroma_datasets-0.1.1/pyproject.toml
--rw-r--r--   0 jeff       (501) staff       (20)        0 2023-06-29 00:06:54.000000 chroma_datasets-0.1.1/requirements.txt
--rw-r--r--   0 jeff       (501) staff       (20)       38 2023-06-29 00:07:50.645116 chroma_datasets-0.1.1/setup.cfg
--rw-r--r--   0 jeff       (501) staff       (20)    18343 2023-06-29 00:03:36.000000 chroma_datasets-0.1.1/test.ipynb
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-01 21:32:37.718657 chroma_datasets-0.1.2/
+-rw-r--r--   0 jeff       (501) staff       (20)      130 2023-07-01 20:58:36.000000 chroma_datasets-0.1.2/.gitignore
+-rw-r--r--   0 jeff       (501) staff       (20)      166 2023-07-01 21:08:45.000000 chroma_datasets-0.1.2/DEVELOP.md
+-rw-r--r--   0 jeff       (501) staff       (20)    11357 2023-06-28 23:45:35.000000 chroma_datasets-0.1.2/LICENSE.md
+-rw-r--r--   0 jeff       (501) staff       (20)     4551 2023-07-01 21:32:37.718509 chroma_datasets-0.1.2/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)     3934 2023-07-01 21:13:04.000000 chroma_datasets-0.1.2/README.md
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-01 21:32:37.711707 chroma_datasets-0.1.2/bin/
+-rw-r--r--   0 jeff       (501) staff       (20)      151 2023-06-28 23:46:19.000000 chroma_datasets-0.1.2/bin/version
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-01 21:32:37.712065 chroma_datasets-0.1.2/chroma_datasets/
+-rw-r--r--   0 jeff       (501) staff       (20)      200 2023-07-01 21:32:29.000000 chroma_datasets-0.1.2/chroma_datasets/__init__.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-01 21:32:37.712793 chroma_datasets-0.1.2/chroma_datasets/__pycache__/
+-rw-r--r--   0 jeff       (501) staff       (20)      312 2023-06-28 23:49:38.000000 chroma_datasets-0.1.2/chroma_datasets/__pycache__/__init__.cpython-310.pyc
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-01 21:32:37.717493 chroma_datasets-0.1.2/chroma_datasets/datasets/
+-rw-r--r--   0 jeff       (501) staff       (20)     1250 2023-07-01 14:06:36.000000 chroma_datasets-0.1.2/chroma_datasets/datasets/glue.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1374 2023-07-01 16:33:30.000000 chroma_datasets-0.1.2/chroma_datasets/datasets/paul_graham_essay.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1690 2023-07-01 15:56:05.000000 chroma_datasets-0.1.2/chroma_datasets/datasets/sciq.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1302 2023-07-01 15:56:11.000000 chroma_datasets-0.1.2/chroma_datasets/datasets/state_of_the_union.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1621 2023-07-01 20:57:28.000000 chroma_datasets-0.1.2/chroma_datasets/types.py
+-rw-r--r--   0 jeff       (501) staff       (20)     5869 2023-07-01 20:56:41.000000 chroma_datasets-0.1.2/chroma_datasets/utils.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-01 21:32:37.712673 chroma_datasets-0.1.2/chroma_datasets.egg-info/
+-rw-r--r--   0 jeff       (501) staff       (20)     4551 2023-07-01 21:32:37.000000 chroma_datasets-0.1.2/chroma_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)      741 2023-07-01 21:32:37.000000 chroma_datasets-0.1.2/chroma_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff       (501) staff       (20)        1 2023-07-01 21:32:37.000000 chroma_datasets-0.1.2/chroma_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       19 2023-07-01 21:32:37.000000 chroma_datasets-0.1.2/chroma_datasets.egg-info/requires.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       16 2023-07-01 21:32:37.000000 chroma_datasets-0.1.2/chroma_datasets.egg-info/top_level.txt
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-01 21:32:37.717998 chroma_datasets-0.1.2/examples/
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-01 21:32:37.718284 chroma_datasets-0.1.2/examples/data/
+-rw-r--r--   0 jeff       (501) staff       (20)    78216 2023-07-01 14:06:09.000000 chroma_datasets-0.1.2/examples/data/paul_graham_essay.txt
+-rw-r--r--   0 jeff       (501) staff       (20)    39027 2023-06-29 16:17:28.000000 chroma_datasets-0.1.2/examples/data/state_of_the_union.txt
+-rw-r--r--   0 jeff       (501) staff       (20)     2906 2023-07-01 20:52:41.000000 chroma_datasets-0.1.2/examples/example_export.ipynb
+-rw-r--r--   0 jeff       (501) staff       (20)     2566 2023-07-01 20:53:26.000000 chroma_datasets-0.1.2/examples/example_import.ipynb
+-rw-r--r--   0 jeff       (501) staff       (20)     2944 2023-07-01 20:53:57.000000 chroma_datasets-0.1.2/examples/example_misc_hf_import.ipynb
+-rw-r--r--   0 jeff       (501) staff       (20)      879 2023-07-01 21:00:51.000000 chroma_datasets-0.1.2/pyproject.toml
+-rw-r--r--   0 jeff       (501) staff       (20)       18 2023-07-01 16:05:53.000000 chroma_datasets-0.1.2/requirements.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       38 2023-07-01 21:32:37.718698 chroma_datasets-0.1.2/setup.cfg
```

### Comparing `chroma_datasets-0.1.1/LICENSE.md` & `chroma_datasets-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `chroma_datasets-0.1.1/pyproject.toml` & `chroma_datasets-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [project]
 name = "chroma_datasets"
-version = "0.1.1"
+version = "0.1.2"
 
 authors = [
   { name="Jeff Huber", email="jeff@trychroma.com" },
   { name="Anton Troynikov", email="anton@trychroma.com" }
 ]
-description = "Chroma Datasets."
+description = "Chroma Datasets - easy to use datasets for vector retrieval"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
+  "langchain",
+  "datasets"
 ]
 
 [tool.pytest.ini_options]
 pythonpath = ["."]
 
 [project.urls]
 "Homepage" = "https://github.com/chroma-core/chroma-datasets"
```

