# Comparing `tmp/sweep-2.0.0.0-py3.10.egg` & `tmp/sweep-2.0.0.1-py3.10.egg`

## zipinfo {}

```diff
@@ -1,25 +1,25 @@
-Zip file size: 16057 bytes, number of entries: 23
--rw-rw-rw-  2.0 fat     6349 b- defN 23-Jun-30 20:34 EGG-INFO/PKG-INFO
--rw-rw-rw-  2.0 fat      671 b- defN 23-Jun-30 20:34 EGG-INFO/SOURCES.txt
--rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-30 20:34 EGG-INFO/dependency_links.txt
+Zip file size: 16085 bytes, number of entries: 23
+-rw-rw-rw-  2.0 fat     6412 b- defN 23-Jun-30 20:42 EGG-INFO/PKG-INFO
+-rw-rw-rw-  2.0 fat      671 b- defN 23-Jun-30 20:42 EGG-INFO/SOURCES.txt
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-30 20:42 EGG-INFO/dependency_links.txt
 -rw-rw-rw-  2.0 fat        2 b- defN 23-Jun-30 20:02 EGG-INFO/not-zip-safe
--rw-rw-rw-  2.0 fat       32 b- defN 23-Jun-30 20:34 EGG-INFO/requires.txt
--rw-rw-rw-  2.0 fat        6 b- defN 23-Jun-30 20:34 EGG-INFO/top_level.txt
--rw-rw-rw-  2.0 fat      316 b- defN 23-Jun-30 20:34 sweep/__init__.pyc
--rw-rw-rw-  2.0 fat      698 b- defN 23-Jun-30 20:34 sweep/calc_proj_mat_size.pyc
--rw-rw-rw-  2.0 fat     3244 b- defN 23-Jun-30 20:34 sweep/default_proj_mat_ope.pyc
--rw-rw-rw-  2.0 fat     5282 b- defN 23-Jun-30 20:34 sweep/fas2sweep.pyc
--rw-rw-rw-  2.0 fat      515 b- defN 23-Jun-30 20:34 sweep/fastaread.pyc
--rw-rw-rw-  2.0 fat      565 b- defN 23-Jun-30 20:34 sweep/is_orthonormal.pyc
--rw-rw-rw-  2.0 fat      662 b- defN 23-Jun-30 20:34 sweep/orthbase.pyc
--rw-rw-rw-  2.0 fat      350 b- defN 23-Jun-30 20:34 sweep/sweep_support/__init__.pyc
--rw-rw-rw-  2.0 fat      601 b- defN 23-Jun-30 20:34 sweep/sweep_support/aa2idx.pyc
--rw-rw-rw-  2.0 fat      807 b- defN 23-Jun-30 20:34 sweep/sweep_support/aa2int.pyc
--rw-rw-rw-  2.0 fat      578 b- defN 23-Jun-30 20:34 sweep/sweep_support/generate_chunk.pyc
--rw-rw-rw-  2.0 fat      301 b- defN 23-Jun-30 20:34 sweep/sweep_support/ij2inds.pyc
--rw-rw-rw-  2.0 fat      764 b- defN 23-Jun-30 20:34 sweep/sweep_support/mask2vec_bin.pyc
--rw-rw-rw-  2.0 fat      843 b- defN 23-Jun-30 20:34 sweep/sweep_support/mask2vec_count.pyc
--rw-rw-rw-  2.0 fat      762 b- defN 23-Jun-30 20:34 sweep/sweep_support/nt2int.pyc
--rw-rw-rw-  2.0 fat      451 b- defN 23-Jun-30 20:34 sweep/sweep_support/orth.pyc
--rw-rw-rw-  2.0 fat      483 b- defN 23-Jun-30 20:34 sweep/sweep_support/seq2list.pyc
-23 files, 24283 bytes uncompressed, 13065 bytes compressed:  46.2%
+-rw-rw-rw-  2.0 fat       32 b- defN 23-Jun-30 20:42 EGG-INFO/requires.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Jun-30 20:42 EGG-INFO/top_level.txt
+-rw-rw-rw-  2.0 fat      316 b- defN 23-Jun-30 20:42 sweep/__init__.pyc
+-rw-rw-rw-  2.0 fat      698 b- defN 23-Jun-30 20:42 sweep/calc_proj_mat_size.pyc
+-rw-rw-rw-  2.0 fat     3244 b- defN 23-Jun-30 20:42 sweep/default_proj_mat_ope.pyc
+-rw-rw-rw-  2.0 fat     5282 b- defN 23-Jun-30 20:42 sweep/fas2sweep.pyc
+-rw-rw-rw-  2.0 fat      515 b- defN 23-Jun-30 20:42 sweep/fastaread.pyc
+-rw-rw-rw-  2.0 fat      565 b- defN 23-Jun-30 20:42 sweep/is_orthonormal.pyc
+-rw-rw-rw-  2.0 fat      662 b- defN 23-Jun-30 20:42 sweep/orthbase.pyc
+-rw-rw-rw-  2.0 fat      350 b- defN 23-Jun-30 20:42 sweep/sweep_support/__init__.pyc
+-rw-rw-rw-  2.0 fat      601 b- defN 23-Jun-30 20:42 sweep/sweep_support/aa2idx.pyc
+-rw-rw-rw-  2.0 fat      807 b- defN 23-Jun-30 20:42 sweep/sweep_support/aa2int.pyc
+-rw-rw-rw-  2.0 fat      578 b- defN 23-Jun-30 20:42 sweep/sweep_support/generate_chunk.pyc
+-rw-rw-rw-  2.0 fat      301 b- defN 23-Jun-30 20:42 sweep/sweep_support/ij2inds.pyc
+-rw-rw-rw-  2.0 fat      764 b- defN 23-Jun-30 20:42 sweep/sweep_support/mask2vec_bin.pyc
+-rw-rw-rw-  2.0 fat      843 b- defN 23-Jun-30 20:42 sweep/sweep_support/mask2vec_count.pyc
+-rw-rw-rw-  2.0 fat      762 b- defN 23-Jun-30 20:42 sweep/sweep_support/nt2int.pyc
+-rw-rw-rw-  2.0 fat      451 b- defN 23-Jun-30 20:42 sweep/sweep_support/orth.pyc
+-rw-rw-rw-  2.0 fat      483 b- defN 23-Jun-30 20:42 sweep/sweep_support/seq2list.pyc
+23 files, 24346 bytes uncompressed, 13093 bytes compressed:  46.2%
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: sweep
-Version: 2.0.0.0
+Version: 2.0.0.1
 Summary: SWeeP is a tool for representing large biological sequences datasets in compact vectors
+Home-page: https://github.com/diogomachado-bioinfo/sweep
 Author: Diogo de J. S. Machado
 Author-email: diogomachado.bioinfo@gmail.com
 License: BSD-3-Clause
-Description-Content-Type: markdown
+Description-Content-Type: text/markdown
 
   -----------------------------------
   SWeeP: Sequence Window Projection
   -----------------------------------
 
 This Python package implements the SWeeP (Sequence Window Projection)
 algorithm for representing large biological sequence datasets in compact
```

