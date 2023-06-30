# Comparing `tmp/sweep-1.3.0.0-py3.8.egg` & `tmp/sweep-2.0.0.0-py3.10.egg`

## zipinfo {}

```diff
@@ -1,23 +1,25 @@
-Zip file size: 12911 bytes, number of entries: 21
--rw-rw-rw-  2.0 fat     2061 b- defN 22-Nov-08 19:29 EGG-INFO/PKG-INFO
--rw-rw-rw-  2.0 fat      641 b- defN 22-Nov-08 19:29 EGG-INFO/SOURCES.txt
--rw-rw-rw-  2.0 fat        1 b- defN 22-Nov-08 19:29 EGG-INFO/dependency_links.txt
--rw-rw-rw-  2.0 fat        2 b- defN 22-Nov-08 19:25 EGG-INFO/not-zip-safe
--rw-rw-rw-  2.0 fat       51 b- defN 22-Nov-08 19:29 EGG-INFO/requires.txt
--rw-rw-rw-  2.0 fat        6 b- defN 22-Nov-08 19:29 EGG-INFO/top_level.txt
--rw-rw-rw-  2.0 fat      217 b- defN 22-Nov-08 19:29 sweep/__init__.pyc
--rw-rw-rw-  2.0 fat     2551 b- defN 22-Nov-08 19:29 sweep/default_proj_mat_ope.pyc
--rw-rw-rw-  2.0 fat     3663 b- defN 22-Nov-08 19:29 sweep/fas2sweep.pyc
--rw-rw-rw-  2.0 fat      382 b- defN 22-Nov-08 19:29 sweep/sweep_support/__init__.pyc
--rw-rw-rw-  2.0 fat      651 b- defN 22-Nov-08 19:29 sweep/sweep_support/aa2idx.pyc
--rw-rw-rw-  2.0 fat      716 b- defN 22-Nov-08 19:29 sweep/sweep_support/aa2int.pyc
--rw-rw-rw-  2.0 fat      343 b- defN 22-Nov-08 19:29 sweep/sweep_support/fastaread.pyc
--rw-rw-rw-  2.0 fat      605 b- defN 22-Nov-08 19:29 sweep/sweep_support/generate_chunk.pyc
--rw-rw-rw-  2.0 fat      299 b- defN 22-Nov-08 19:29 sweep/sweep_support/ij2inds.pyc
--rw-rw-rw-  2.0 fat      833 b- defN 22-Nov-08 19:29 sweep/sweep_support/mask2vec.pyc
--rw-rw-rw-  2.0 fat     2150 b- defN 22-Nov-08 19:29 sweep/sweep_support/matlab_like.pyc
--rw-rw-rw-  2.0 fat      671 b- defN 22-Nov-08 19:29 sweep/sweep_support/nt2int.pyc
--rw-rw-rw-  2.0 fat      496 b- defN 22-Nov-08 19:29 sweep/sweep_support/orth.pyc
--rw-rw-rw-  2.0 fat      461 b- defN 22-Nov-08 19:29 sweep/sweep_support/orthbase.pyc
--rw-rw-rw-  2.0 fat      412 b- defN 22-Nov-08 19:29 sweep/sweep_support/seq2list.pyc
-21 files, 17212 bytes uncompressed, 10133 bytes compressed:  41.1%
+Zip file size: 16057 bytes, number of entries: 23
+-rw-rw-rw-  2.0 fat     6349 b- defN 23-Jun-30 20:34 EGG-INFO/PKG-INFO
+-rw-rw-rw-  2.0 fat      671 b- defN 23-Jun-30 20:34 EGG-INFO/SOURCES.txt
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-30 20:34 EGG-INFO/dependency_links.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Jun-30 20:02 EGG-INFO/not-zip-safe
+-rw-rw-rw-  2.0 fat       32 b- defN 23-Jun-30 20:34 EGG-INFO/requires.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Jun-30 20:34 EGG-INFO/top_level.txt
+-rw-rw-rw-  2.0 fat      316 b- defN 23-Jun-30 20:34 sweep/__init__.pyc
+-rw-rw-rw-  2.0 fat      698 b- defN 23-Jun-30 20:34 sweep/calc_proj_mat_size.pyc
+-rw-rw-rw-  2.0 fat     3244 b- defN 23-Jun-30 20:34 sweep/default_proj_mat_ope.pyc
+-rw-rw-rw-  2.0 fat     5282 b- defN 23-Jun-30 20:34 sweep/fas2sweep.pyc
+-rw-rw-rw-  2.0 fat      515 b- defN 23-Jun-30 20:34 sweep/fastaread.pyc
+-rw-rw-rw-  2.0 fat      565 b- defN 23-Jun-30 20:34 sweep/is_orthonormal.pyc
+-rw-rw-rw-  2.0 fat      662 b- defN 23-Jun-30 20:34 sweep/orthbase.pyc
+-rw-rw-rw-  2.0 fat      350 b- defN 23-Jun-30 20:34 sweep/sweep_support/__init__.pyc
+-rw-rw-rw-  2.0 fat      601 b- defN 23-Jun-30 20:34 sweep/sweep_support/aa2idx.pyc
+-rw-rw-rw-  2.0 fat      807 b- defN 23-Jun-30 20:34 sweep/sweep_support/aa2int.pyc
+-rw-rw-rw-  2.0 fat      578 b- defN 23-Jun-30 20:34 sweep/sweep_support/generate_chunk.pyc
+-rw-rw-rw-  2.0 fat      301 b- defN 23-Jun-30 20:34 sweep/sweep_support/ij2inds.pyc
+-rw-rw-rw-  2.0 fat      764 b- defN 23-Jun-30 20:34 sweep/sweep_support/mask2vec_bin.pyc
+-rw-rw-rw-  2.0 fat      843 b- defN 23-Jun-30 20:34 sweep/sweep_support/mask2vec_count.pyc
+-rw-rw-rw-  2.0 fat      762 b- defN 23-Jun-30 20:34 sweep/sweep_support/nt2int.pyc
+-rw-rw-rw-  2.0 fat      451 b- defN 23-Jun-30 20:34 sweep/sweep_support/orth.pyc
+-rw-rw-rw-  2.0 fat      483 b- defN 23-Jun-30 20:34 sweep/sweep_support/seq2list.pyc
+23 files, 24283 bytes uncompressed, 13065 bytes compressed:  46.2%
```

## zipnote «TEMP»/diffoscope_u2fulzs4_/tmpfz794rs5_.zip

```diff
@@ -15,50 +15,56 @@
 
 Filename: EGG-INFO/top_level.txt
 Comment: 
 
 Filename: sweep/__init__.pyc
 Comment: 
 
+Filename: sweep/calc_proj_mat_size.pyc
+Comment: 
+
 Filename: sweep/default_proj_mat_ope.pyc
 Comment: 
 
 Filename: sweep/fas2sweep.pyc
 Comment: 
 
+Filename: sweep/fastaread.pyc
+Comment: 
+
+Filename: sweep/is_orthonormal.pyc
+Comment: 
+
+Filename: sweep/orthbase.pyc
+Comment: 
+
 Filename: sweep/sweep_support/__init__.pyc
 Comment: 
 
 Filename: sweep/sweep_support/aa2idx.pyc
 Comment: 
 
 Filename: sweep/sweep_support/aa2int.pyc
 Comment: 
 
-Filename: sweep/sweep_support/fastaread.pyc
-Comment: 
-
 Filename: sweep/sweep_support/generate_chunk.pyc
 Comment: 
 
 Filename: sweep/sweep_support/ij2inds.pyc
 Comment: 
 
-Filename: sweep/sweep_support/mask2vec.pyc
+Filename: sweep/sweep_support/mask2vec_bin.pyc
 Comment: 
 
-Filename: sweep/sweep_support/matlab_like.pyc
+Filename: sweep/sweep_support/mask2vec_count.pyc
 Comment: 
 
 Filename: sweep/sweep_support/nt2int.pyc
 Comment: 
 
 Filename: sweep/sweep_support/orth.pyc
 Comment: 
 
-Filename: sweep/sweep_support/orthbase.pyc
-Comment: 
-
 Filename: sweep/sweep_support/seq2list.pyc
 Comment: 
 
 Zip file comment:
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,37 +1,115 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: sweep
-Version: 1.3.0.0
-Summary: SWeeP is a tool to representing large biological sequences datasets in compact vectors
-Home-page: https://github.com/diogomachado-bioinfo/sweep
+Version: 2.0.0.0
+Summary: SWeeP is a tool for representing large biological sequences datasets in compact vectors
 Author: Diogo de J. S. Machado
 Author-email: diogomachado.bioinfo@gmail.com
-License: UNKNOWN
-Description: SWeeP Overview
-        ====================
-        This package is a python version of the tool described in the article available at <https://www.nature.com/articles/s41598-019-55627-4>. **Please quote the article**.
-        
-        Use
-        ------------
-        To use SWeeP in python, install the package with the command "pip install sweep" and import the package in your code, as in the example:
-        
-        .. code-block:: python
-        
-            from sweep import fastaread, fas2sweep
-            fasta = fastaread ("fasta_file_path")
-            vect = fas2sweep (fasta)
-        	
-        The default configurations are intended for vectorization of amino acid sequences. The default output is the matrix already projected, with 600 columns. **See the article if you need information about the projection method**.
-        
-        The default projection matrix has dimensions 160000x600. It is necessary generate a new matrix if other masks are used or another projection size is desired. To generate the orthonormal matrix for projection, a function called orthbase is available on the package. For example, if the goal is to change the projection size to 300, just use:
-        
-        .. code-block:: python
-        
-            from sweep import fastaread, fas2sweep, orthbase
-            ob = orthbase(160000,300)
-            fasta = fastaread ("fasta_file_path")
-            vect = fas2sweep (fasta, orth_mat = ob)
-        	
-        It is also possible obtain the result without projection, for this is necessary set the parameter "projection" to "False".
-        
-        For the nucleotide sequences vectorization is possible set the parameter fasta_type to "NT".
-Platform: UNKNOWN
+License: BSD-3-Clause
+Description-Content-Type: markdown
+
+  -----------------------------------
+  SWeeP: Sequence Window Projection
+  -----------------------------------
+
+This Python package implements the SWeeP (Sequence Window Projection)
+algorithm for representing large biological sequence datasets in compact
+vectors. SWeeP allows efficient processing and analysis of sequence data
+by converting sequences into fixed-length feature vectors.
+
+# Installation
+
+To use SWeeP in Python, install the package with the following command:
+
+    pip install sweep
+
+# Usage
+
+## Downloading the Default Projection Matrix
+
+In the first use of fas2sweep with the default parameter, it will be
+necessary to download the default projection matrix. It is not necessary
+for use with custom projection matrix, as
+demonstrated in the "Changing Projection Matrix" topic.
+
+    from sweep import down_proj_mat
+    down_proj_mat() # Downloads the default projection matrix file
+
+## Handling Amino Acid Sequences
+
+The default configurations of SWeeP are intended for vectorization of
+amino acid sequences. The default output is a matrix already projected
+with 600 columns. Here\'s an example of how to use SWeeP with amino acid
+sequences:
+
+    from sweep import fastaread, fas2sweep
+
+    fasta = fastaread("fasta_file_path")
+    vect = fas2sweep(fasta)
+
+## Changing Projection Matrix
+
+To change the projection matrix, a new orthonormal matrix can be
+generated using the orthbase function. For example,
+here is an example of how to change the projection size to 300:
+
+    from sweep import fastaread, fas2sweep, orthbase
+
+    ob = orthbase(160000, 300)
+    fasta = fastaread("fasta_file_path")
+    vect = fas2sweep(fasta, orth_mat=ob)
+
+## Handling Nucleotide Sequences
+
+For nucleotide sequences, there is no default projection matrix
+available in this version. Therefore, to work with nucleotides
+is possible to create a custom projection matrix using the
+orthbase function. The matrix size can be calculated using
+the calc_proj_mat_size function. Here is an example:
+
+    from sweep import fastaread, fas2sweep, orthbase, calc_proj_mat_size
+
+    mask = [4, 7, 4]
+    matrix_size = calc_proj_mat_size(mask, 'NT')
+    ob = orthbase(matrix_size, 600)
+    fasta = fastaread("fasta_file_path")
+    vect = fas2sweep(fasta, mask=mask, orth_mat=ob, fasta_type='NT')
+
+## Available Functions
+
+Here is a summary of the
+functions available in the SWeeP package:
+
+| Function                            | Description                                                                      | Input                                                          | Output                                          |
+|-------------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------|-------------------------------------------------|
+| ``fastaread``                       | Reads a FASTA file and returns a list of sequence records                        | ``fastaname`` (str): Path to the FASTA file                    | ``records`` (list): List of sequence records    |
+| ``fas2sweep``                       | Converts a list of sequences into SWeeP vectors                                  | ``fasta`` (list): List of sequence records                     | ``vect`` (numpy.ndarray): SWeeP vectors         |
+| ``orthbase``                        | Generates an orthonormal projection matrix of the specified size                 | ``lin`` (int): Number of rows                                  | ``mret`` (numpy.ndarray): Orthonormal matrix    |
+| ``calc_proj_mat_size``              | Calculates the number of lines in the projection matrix for a given mask         | ``mask`` (list): Mask specifying dimensions                    | ``lines`` (int): Number of lines in the matrix  |
+| ``md5``                             | Calculates the MD5 hash of a file                                                | ``fname`` (str): Path to the file                              | ``hash_md5`` (str): MD5 hash of the file        |
+| ``down_proj_mat``                   | Downloads the default projection matrix file                                     | ``destination`` (str): Path to the destination file (optional) | None                                            |
+| ``return_proj_mat_not_found_error`` | Raises an exception indicating that the default projection matrix is not found   | None                                                           | None                                            |
+| ``check_default_proj_mat``          | Checks if the default projection matrix exists and matches the expected MD5 hash | ``file`` (str): Path to the projection matrix file             | None                                            |
+| ``get_default_proj_mat``            | Retrieves the default projection matrix                                          | None                                                           | ``orth_mat`` (numpy.ndarray): Projection matrix |
+
+## Article Reference
+
+If you use the SWeeP algorithm or this Python package in your research work, please cite the
+following article:
+
+``` none
+@article{De Pierri2020,
+  title={SWeeP: representing large biological sequences datasets in compact vectors},
+  author={De Pierri, Camilla Reginatto and Voyceik, Ricardo and Santos de Mattos, LetÃ­cia Graziela Costa and Kulik, Mariane GonÃ§alves and Camargo, JosuÃ© Oliveira and Repula de Oliveira, Aryel Marlus and de Lima Nichio, Bruno Thiago and Marchaukoski, Jeroniza Nunes and da Silva Filho, Antonio Camilo and Guizelini, Dieval and Ortega, J. Miguel and Pedrosa, Fabio O. and Raittz, Roberto Tadeu},
+  journal={Scientific Reports},
+  volume={10},
+  number={1},
+  pages={91},
+  year={2020},
+  doi={10.1038/s41598-019-55627-4},
+  url={https://doi.org/10.1038/s41598-019-55627-4},
+  issn={2045-2322}
+}
+```
+
+Please refer to the article for a detailed description of the SWeeP
+algorithm and its applications.
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## EGG-INFO/SOURCES.txt

```diff
@@ -1,23 +1,25 @@
-README.rst
+README.md
 setup.py
 sweep/__init__.py
+sweep/calc_proj_mat_size.py
 sweep/default_proj_mat_ope.py
 sweep/fas2sweep.py
+sweep/fastaread.py
+sweep/is_orthonormal.py
+sweep/orthbase.py
 sweep.egg-info/PKG-INFO
 sweep.egg-info/SOURCES.txt
 sweep.egg-info/dependency_links.txt
 sweep.egg-info/not-zip-safe
 sweep.egg-info/requires.txt
 sweep.egg-info/top_level.txt
 sweep/sweep_support/__init__.py
 sweep/sweep_support/aa2idx.py
 sweep/sweep_support/aa2int.py
-sweep/sweep_support/fastaread.py
 sweep/sweep_support/generate_chunk.py
 sweep/sweep_support/ij2inds.py
-sweep/sweep_support/mask2vec.py
-sweep/sweep_support/matlab_like.py
+sweep/sweep_support/mask2vec_bin.py
+sweep/sweep_support/mask2vec_count.py
 sweep/sweep_support/nt2int.py
 sweep/sweep_support/orth.py
-sweep/sweep_support/orthbase.py
 sweep/sweep_support/seq2list.py
```

## EGG-INFO/requires.txt

```diff
@@ -1,6 +1,5 @@
 numpy
 Biopython
 scipy
-more_itertools
 tqdm
-requests
+h5py
```

## sweep/__init__.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Mar 22 02:38:19 2022 UTC, .py size: 135 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,14 +1,20 @@
-00000000: 550d 0d0a 0000 0000 9b36 3962 8700 0000  U........69b....
+00000000: 6f0d 0d0a 0000 0000 8036 9f64 fc00 0000  o........6.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 1c00 0000 6400  .....@...s....d.
+00000020: 0002 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 5400 6400 6401 6c01 5400 6400  d.l.T.d.d.l.T.d.
-00000040: 6401 6c02 5400 6402 5300 2903 e901 0000  d.l.T.d.S.).....
-00000050: 0029 01da 012a 4e29 035a 0d73 7765 6570  .)...*N).Z.sweep
-00000060: 5f73 7570 706f 7274 5a09 6661 7332 7377  _supportZ.fas2sw
-00000070: 6565 705a 1464 6566 6175 6c74 5f70 726f  eepZ.default_pro
-00000080: 6a5f 6d61 745f 6f70 65a9 0072 0300 0000  j_mat_ope..r....
-00000090: 7203 0000 00fa 2b62 7569 6c64 5c62 6469  r.....+build\bdi
-000000a0: 7374 2e77 696e 2d61 6d64 3634 5c65 6767  st.win-amd64\egg
-000000b0: 5c73 7765 6570 5c5f 5f69 6e69 745f 5f2e  \sweep\__init__.
-000000c0: 7079 da08 3c6d 6f64 756c 653e 0300 0000  py..<module>....
-000000d0: 7304 0000 0008 0108 01                   s........
+00000040: 6401 6c02 5400 6400 6401 6c03 5400 6400  d.l.T.d.d.l.T.d.
+00000050: 6401 6c04 5400 6400 6401 6c05 5400 6400  d.l.T.d.d.l.T.d.
+00000060: 6401 6c06 5400 6402 5300 2903 e901 0000  d.l.T.d.S.).....
+00000070: 0029 01da 012a 4e29 075a 0d73 7765 6570  .)...*N).Z.sweep
+00000080: 5f73 7570 706f 7274 5a09 6661 7332 7377  _supportZ.fas2sw
+00000090: 6565 705a 1464 6566 6175 6c74 5f70 726f  eepZ.default_pro
+000000a0: 6a5f 6d61 745f 6f70 655a 086f 7274 6862  j_mat_opeZ.orthb
+000000b0: 6173 655a 0966 6173 7461 7265 6164 5a0e  aseZ.fastareadZ.
+000000c0: 6973 5f6f 7274 686f 6e6f 726d 616c 5a12  is_orthonormalZ.
+000000d0: 6361 6c63 5f70 726f 6a5f 6d61 745f 7369  calc_proj_mat_si
+000000e0: 7a65 a900 7203 0000 0072 0300 0000 fa2b  ze..r....r.....+
+000000f0: 6275 696c 645c 6264 6973 742e 7769 6e2d  build\bdist.win-
+00000100: 616d 6436 345c 6567 675c 7377 6565 705c  amd64\egg\sweep\
+00000110: 5f5f 696e 6974 5f5f 2e70 79da 083c 6d6f  __init__.py..<mo
+00000120: 6475 6c65 3e01 0000 0073 0e00 0000 0802  dule>....s......
+00000130: 0801 0801 0801 0801 0801 0c01            ............
```

## sweep/default_proj_mat_ope.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sun Nov  6 02:22:02 2022 UTC, .py size: 2543 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,160 +1,203 @@
-00000000: 550d 0d0a 0000 0000 4a1a 6763 ef09 0000  U.......J.gc....
+00000000: 6f0d 0d0a 0000 0000 c556 9f64 ce0c 0000  o........V.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6402 6403 8400 5a05 640c  d.l.Z.d.d...Z.d.
 00000060: 6404 6405 8401 5a06 6406 6407 8400 5a07  d.d...Z.d.d...Z.
 00000070: 6408 6409 8400 5a08 640a 640b 8400 5a09  d.d...Z.d.d...Z.
 00000080: 6401 5300 290d e900 0000 004e 6301 0000  d.S.)......Nc...
-00000090: 0000 0000 0000 0000 0003 0000 0009 0000  ................
-000000a0: 0003 0000 0073 4800 0000 7400 a001 a100  .....sH...t.....
-000000b0: 7d01 7402 7c00 6401 8302 8f28 8900 7403  }.t.|.d....(..t.
+00000090: 0000 0000 0000 0000 0003 0000 0008 0000  ................
+000000a0: 0003 0000 0073 6200 0000 7400 a001 a100  .....sb...t.....
+000000b0: 7d01 7402 7c00 6401 8302 8f1c 8900 7403  }.t.|.d.......t.
 000000c0: 8700 6601 6402 6403 8408 6404 8302 4400  ..f.d.d...d...D.
-000000d0: 5d0e 7d02 7c01 a004 7c02 a101 0100 7126  ].}.|...|.....q&
-000000e0: 5700 3500 5100 5200 5800 7c01 a005 a100  W.5.Q.R.X.|.....
-000000f0: 5300 2905 4eda 0272 6263 0000 0000 0000  S.).N..rbc......
-00000100: 0000 0000 0000 0000 0000 0300 0000 1300  ................
-00000110: 0000 730a 0000 0088 00a0 0064 01a1 0153  ..s........d...S
-00000120: 0029 024e e900 1000 0029 01da 0472 6561  .).N.....)...rea
-00000130: 64a9 00a9 01da 0166 7205 0000 00fa 3762  d......fr.....7b
-00000140: 7569 6c64 5c62 6469 7374 2e77 696e 2d61  uild\bdist.win-a
-00000150: 6d64 3634 5c65 6767 5c73 7765 6570 5c64  md64\egg\sweep\d
-00000160: 6566 6175 6c74 5f70 726f 6a5f 6d61 745f  efault_proj_mat_
-00000170: 6f70 652e 7079 da08 3c6c 616d 6264 613e  ope.py..<lambda>
-00000180: 0b00 0000 f300 0000 007a 156d 6435 2e3c  .........z.md5.<
-00000190: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
-000001a0: 720a 0000 0029 06da 0768 6173 686c 6962  r....)...hashlib
-000001b0: da03 6d64 35da 046f 7065 6eda 0469 7465  ..md5..open..ite
-000001c0: 72da 0675 7064 6174 65da 0968 6578 6469  r..update..hexdi
-000001d0: 6765 7374 2903 da05 666e 616d 655a 0868  gest)...fnameZ.h
-000001e0: 6173 685f 6d64 35da 0563 6875 6e6b 7205  ash_md5..chunkr.
-000001f0: 0000 0072 0600 0000 7208 0000 0072 0c00  ...r....r....r..
-00000200: 0000 0800 0000 730a 0000 0000 0108 010c  ......s.........
-00000210: 0116 0116 0172 0c00 0000 6301 0000 0000  .....r....c.....
-00000220: 0000 0000 0000 000a 0000 0009 0000 0043  ...............C
-00000230: 0000 0073 4e01 0000 7c00 6400 6b02 722e  ...sN...|.d.k.r.
-00000240: 7400 6a01 a002 7400 6a01 a003 7404 a101  t.j...t.j...t...
-00000250: a101 7d01 7400 6a01 a005 7c01 6401 a102  ..}.t.j...|.d...
-00000260: 7d02 7c02 7d00 7a26 7406 7c00 8301 6402  }.|.}.z&t.|...d.
-00000270: 6b02 7252 7407 6403 7c00 1600 6404 6405  k.rRt.d.|...d.d.
-00000280: 8d02 0100 5700 6400 5300 5700 6e14 0400  ....W.d.S.W.n...
-00000290: 7408 6b0a 7268 0100 0100 0100 5900 6e02  t.k.rh......Y.n.
-000002a0: 5800 6406 7d03 7409 7c00 6407 8302 8fb6  X.d.}.t.|.d.....
-000002b0: 7d04 7407 6408 7c00 1600 6404 6405 8d02  }.t.d.|...d.d...
-000002c0: 0100 7407 6409 7400 6a01 a00a 7c00 a101  ..t.d.t.j...|...
-000002d0: 1600 6404 6405 8d02 0100 740b 6a0c 7c03  ..d.d.....t.j.|.
-000002e0: 6404 640a 8d02 7d05 7c05 6a0d a00c 640b  d.d...}.|.j...d.
-000002f0: a101 7d06 640c 7d07 740e 7c06 8301 7d06  ..}.d.}.t.|...}.
-00000300: 7c05 6a0f 640d 640e 8d01 4400 5d54 7d08  |.j.d.d...D.]T}.
-00000310: 7c07 7410 7c08 8301 3700 7d07 7c04 a011  |.t.|...7.}.|...
-00000320: 7c08 a101 0100 740e 640f 7c07 1400 7c06  |.....t.d.|...|.
-00000330: 1b00 8301 7d09 7412 6a13 a011 6410 6411  ....}.t.j...d.d.
-00000340: 7c09 1400 6412 640f 7c09 1800 1400 6602  |...d.d.|.....f.
-00000350: 1600 a101 0100 7412 6a13 a014 a100 0100  ......t.j.......
-00000360: 71d4 5700 3500 5100 5200 5800 7406 7c00  q.W.5.Q.R.X.t.|.
-00000370: 8301 6402 6b03 9001 724a 7415 6413 8301  ..d.k...rJt.d...
-00000380: 8201 6400 5300 2914 4efa 2773 7765 6570  ..d.S.).N.'sweep
-00000390: 2d64 6566 6175 6c74 2d70 726f 6a65 6374  -default-project
-000003a0: 696f 6e2d 6d61 7472 6978 2d36 3030 2e6d  ion-matrix-600.m
-000003b0: 6174 da20 6631 3835 3837 6163 3739 6334  at. f18587ac79c4
-000003c0: 3532 6534 3139 6630 6263 6232 3035 3964  52e419f0bcb2059d
-000003d0: 3636 3139 7a3a 5468 6520 6465 6661 756c  6619z:The defaul
-000003e0: 7420 7072 6f6a 6563 7469 6f6e 206d 6174  t projection mat
-000003f0: 7269 7820 6973 2061 6c72 6561 6479 2061  rix is already a
-00000400: 7661 696c 6162 6c65 2061 7420 3c25 733e  vailable at <%s>
-00000410: 5429 01da 0566 6c75 7368 7aa1 6874 7470  T)...flushz.http
-00000420: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
-00000430: 696f 676f 6d61 6368 6164 6f2d 6269 6f69  iogomachado-bioi
-00000440: 6e66 6f2f 7377 6565 702d 6465 6661 756c  nfo/sweep-defaul
-00000450: 742d 7072 6f6a 6563 7469 6f6e 2d6d 6174  t-projection-mat
-00000460: 7269 782f 7265 6c65 6173 6573 2f64 6f77  rix/releases/dow
-00000470: 6e6c 6f61 642f 7377 6565 702d 6465 6661  nload/sweep-defa
-00000480: 756c 742d 7072 6f6a 6563 7469 6f6e 2d6d  ult-projection-m
-00000490: 6174 7269 782f 7377 6565 702d 6465 6661  atrix/sweep-defa
-000004a0: 756c 742d 7072 6f6a 6563 7469 6f6e 2d6d  ult-projection-m
-000004b0: 6174 7269 782d 3630 302e 6d61 74da 0277  atrix-600.mat..w
-000004c0: 627a 2054 6865 2064 6f77 6e6c 6f61 6420  bz The download 
-000004d0: 6465 7374 696e 6174 696f 6e20 6973 203c  destination is <
-000004e0: 2573 3e7a 0e44 6f77 6e6c 6f61 6469 6e67  %s>z.Downloading
-000004f0: 2025 7329 01da 0673 7472 6561 6d7a 0e63   %s)...streamz.c
-00000500: 6f6e 7465 6e74 2d6c 656e 6774 6872 0100  ontent-lengthr..
-00000510: 0000 7203 0000 0029 01da 0a63 6875 6e6b  ..r....)...chunk
-00000520: 5f73 697a 65e9 3200 0000 7a07 0d5b 2573  _size.2...z..[%s
-00000530: 2573 5dfa 013d fa01 207a 0f44 6f77 6e6c  %s]..=.. z.Downl
-00000540: 6f61 6420 6661 696c 6564 2916 da02 6f73  oad failed)...os
-00000550: da04 7061 7468 da07 6469 726e 616d 65da  ..path..dirname.
-00000560: 0872 6561 6c70 6174 68da 085f 5f66 696c  .realpath..__fil
-00000570: 655f 5fda 046a 6f69 6e72 0c00 0000 da05  e__..joinr......
-00000580: 7072 696e 74da 1146 696c 654e 6f74 466f  print..FileNotFo
-00000590: 756e 6445 7272 6f72 720d 0000 00da 0862  undErrorr......b
-000005a0: 6173 656e 616d 65da 0872 6571 7565 7374  asename..request
-000005b0: 73da 0367 6574 da07 6865 6164 6572 73da  s..get..headers.
-000005c0: 0369 6e74 5a0c 6974 6572 5f63 6f6e 7465  .intZ.iter_conte
-000005d0: 6e74 da03 6c65 6eda 0577 7269 7465 da03  nt..len..write..
-000005e0: 7379 73da 0673 7464 6f75 7472 1500 0000  sys..stdoutr....
-000005f0: da09 4578 6365 7074 696f 6e29 0a5a 0b64  ..Exception).Z.d
-00000600: 6573 7469 6e61 7469 6f6e da08 6c69 624c  estination..libL
-00000610: 6f63 616c da0e 6d61 745f 6669 6c65 5f6c  ocal..mat_file_l
-00000620: 6f63 616c da04 6c69 6e6b 7207 0000 00da  ocal..linkr.....
-00000630: 0872 6573 706f 6e73 655a 0f74 6f74 616c  .responseZ.total
-00000640: 5f66 696c 655f 7369 7a65 da01 63da 0464  _file_size..c..d
-00000650: 6174 61da 0173 7205 0000 0072 0500 0000  ata..sr....r....
-00000660: 7208 0000 00da 0d64 6f77 6e5f 7072 6f6a  r......down_proj
-00000670: 5f6d 6174 0e00 0000 7334 0000 0000 0108  _mat....s4......
-00000680: 0114 010e 0104 0102 010c 0110 010a 010e  ................
-00000690: 0106 0104 010c 0110 0118 010e 010c 0104  ................
-000006a0: 0108 0110 010c 010a 0110 0120 0116 010e  ........... ....
-000006b0: 0172 3500 0000 6300 0000 0000 0000 0000  .r5...c.........
-000006c0: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
-000006d0: 1000 0000 6401 7d00 7400 7c00 8301 8201  ....d.}.t.|.....
-000006e0: 6400 5300 2902 4e7a 6844 6566 6175 6c74  d.S.).NzhDefault
-000006f0: 2070 726f 6a65 6374 696f 6e20 6d61 7472   projection matr
-00000700: 6978 206e 6f74 2066 6f75 6e64 2c20 746f  ix not found, to
-00000710: 2064 6f77 6e6c 6f61 6420 6974 2075 7365   download it use
-00000720: 3a0a 6672 6f6d 2073 7765 6570 2069 6d70  :.from sweep imp
-00000730: 6f72 7420 646f 776e 5f70 726f 6a5f 6d61  ort down_proj_ma
-00000740: 740a 646f 776e 5f70 726f 6a5f 6d61 7428  t.down_proj_mat(
-00000750: 2929 0172 2d00 0000 2901 5a09 6572 726f  )).r-...).Z.erro
-00000760: 725f 7374 7272 0500 0000 7205 0000 0072  r_strr....r....r
-00000770: 0800 0000 da1f 7265 7475 726e 5f70 726f  ......return_pro
-00000780: 6a5f 6d61 745f 6e6f 745f 666f 756e 645f  j_mat_not_found_
-00000790: 6572 726f 7229 0000 0073 0400 0000 0001  error)...s......
-000007a0: 0401 7236 0000 0063 0100 0000 0000 0000  ..r6...c........
-000007b0: 0000 0000 0100 0000 0800 0000 4300 0000  ............C...
-000007c0: 7336 0000 007a 1674 007c 0083 0164 016b  s6...z.t.|...d.k
-000007d0: 0372 1474 0183 0001 0057 006e 1a04 0074  .r.t.....W.n...t
-000007e0: 026b 0a72 3001 0001 0001 0074 0183 0001  .k.r0......t....
-000007f0: 0059 006e 0258 0064 0053 0029 024e 7214  .Y.n.X.d.S.).Nr.
-00000800: 0000 0029 0372 0c00 0000 7236 0000 0072  ...).r....r6...r
-00000810: 2300 0000 2901 da04 6669 6c65 7205 0000  #...)...filer...
-00000820: 0072 0500 0000 7208 0000 00da 1663 6865  .r....r......che
-00000830: 636b 5f64 6566 6175 6c74 5f70 726f 6a5f  ck_default_proj_
-00000840: 6d61 742c 0000 0073 0a00 0000 0001 0201  mat,...s........
-00000850: 0c01 0a01 0e01 7238 0000 0063 0000 0000  ......r8...c....
-00000860: 0000 0000 0000 0000 0400 0000 0500 0000  ................
-00000870: 4300 0000 7358 0000 0074 006a 01a0 0274  C...sX...t.j...t
-00000880: 006a 01a0 0374 04a1 01a1 017d 0074 006a  .j...t.....}.t.j
-00000890: 01a0 057c 0064 01a1 027d 0174 067c 0183  ...|.d...}.t.|..
-000008a0: 0101 0074 07a0 087c 0164 02a1 027d 0274  ...t...|.d...}.t
-000008b0: 097c 02a0 0aa1 0083 0164 0319 007d 037c  .|.......d...}.|
-000008c0: 027c 0319 0064 0419 006a 0b7d 027c 0253  .|...d...j.}.|.S
-000008d0: 0029 054e 7213 0000 00da 0172 7201 0000  .).Nr......rr...
-000008e0: 0072 0500 0000 290c 721c 0000 0072 1d00  .r....).r....r..
-000008f0: 0000 721e 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
-00000900: 0072 2100 0000 7238 0000 00da 0468 3570  .r!...r8.....h5p
-00000910: 795a 0446 696c 65da 046c 6973 74da 046b  yZ.File..list..k
-00000920: 6579 73da 0154 2904 722e 0000 0072 2f00  eys..T).r....r/.
-00000930: 0000 5a08 6f72 7468 5f6d 6174 da08 7661  ..Z.orth_mat..va
-00000940: 725f 6e61 6d65 7205 0000 0072 0500 0000  r_namer....r....
-00000950: 7208 0000 00da 1467 6574 5f64 6566 6175  r......get_defau
-00000960: 6c74 5f70 726f 6a5f 6d61 7432 0000 0073  lt_proj_mat2...s
-00000970: 0e00 0000 0001 1401 0e01 0801 0c01 1001  ................
-00000980: 0e01 723f 0000 0029 014e 290a 722b 0000  ..r?...).N).r+..
-00000990: 0072 2500 0000 720b 0000 0072 1c00 0000  .r%...r....r....
-000009a0: 723a 0000 0072 0c00 0000 7235 0000 0072  r:...r....r5...r
-000009b0: 3600 0000 7238 0000 0072 3f00 0000 7205  6...r8...r?...r.
-000009c0: 0000 0072 0500 0000 7205 0000 0072 0800  ...r....r....r..
-000009d0: 0000 da08 3c6d 6f64 756c 653e 0300 0000  ....<module>....
-000009e0: 7312 0000 0008 0108 0108 0108 0108 0108  s...............
-000009f0: 060a 1b08 0308 06                        .......
+000000d0: 5d07 7d02 7c01 a004 7c02 a101 0100 7113  ].}.|...|.....q.
+000000e0: 5700 6405 0400 0400 8303 0100 7c01 a005  W.d.........|...
+000000f0: a100 5300 3100 7328 7701 0100 0100 0100  ..S.1.s(w.......
+00000100: 5900 0100 7c01 a005 a100 5300 2906 7a8e  Y...|.....S.).z.
+00000110: 0a20 2020 2043 616c 6375 6c61 7465 2074  .    Calculate t
+00000120: 6865 204d 4435 2068 6173 6820 6f66 2061  he MD5 hash of a
+00000130: 2066 696c 652e 0a0a 2020 2020 4172 6773   file...    Args
+00000140: 3a0a 2020 2020 2020 2020 666e 616d 6520  :.        fname 
+00000150: 2873 7472 293a 2050 6174 6820 746f 2074  (str): Path to t
+00000160: 6865 2066 696c 652e 0a0a 2020 2020 5265  he file...    Re
+00000170: 7475 726e 733a 0a20 2020 2020 2020 2073  turns:.        s
+00000180: 7472 3a20 4d44 3520 6861 7368 206f 6620  tr: MD5 hash of 
+00000190: 7468 6520 6669 6c65 2e0a 2020 2020 da02  the file..    ..
+000001a0: 7262 6300 0000 0000 0000 0000 0000 0000  rbc.............
+000001b0: 0000 0003 0000 0013 0000 0073 0a00 0000  ...........s....
+000001c0: 8800 a000 6401 a101 5300 2902 4ee9 0010  ....d...S.).N...
+000001d0: 0000 2901 da04 7265 6164 a900 a901 da01  ..)...read......
+000001e0: 6672 0500 0000 fa37 6275 696c 645c 6264  fr.....7build\bd
+000001f0: 6973 742e 7769 6e2d 616d 6436 345c 6567  ist.win-amd64\eg
+00000200: 675c 7377 6565 705c 6465 6661 756c 745f  g\sweep\default_
+00000210: 7072 6f6a 5f6d 6174 5f6f 7065 2e70 79da  proj_mat_ope.py.
+00000220: 083c 6c61 6d62 6461 3e16 0000 0073 0200  .<lambda>....s..
+00000230: 0000 0a00 7a15 6d64 352e 3c6c 6f63 616c  ....z.md5.<local
+00000240: 733e 2e3c 6c61 6d62 6461 3ef3 0000 0000  s>.<lambda>.....
+00000250: 4e29 06da 0768 6173 686c 6962 da03 6d64  N)...hashlib..md
+00000260: 35da 046f 7065 6eda 0469 7465 72da 0675  5..open..iter..u
+00000270: 7064 6174 65da 0968 6578 6469 6765 7374  pdate..hexdigest
+00000280: 2903 da05 666e 616d 655a 0868 6173 685f  )...fnameZ.hash_
+00000290: 6d64 35da 0563 6875 6e6b 7205 0000 0072  md5..chunkr....r
+000002a0: 0600 0000 7208 0000 0072 0c00 0000 0a00  ....r....r......
+000002b0: 0000 7312 0000 0008 0a0c 0116 010c 0102  ..s.............
+000002c0: ff0a ff08 0310 fd08 0372 0c00 0000 6301  .........r....c.
+000002d0: 0000 0000 0000 0000 0000 000a 0000 0009  ................
+000002e0: 0000 0043 0000 0073 5e01 0000 7c00 6401  ...C...s^...|.d.
+000002f0: 7500 7217 7400 6a01 a002 7400 6a01 a003  u.r.t.j...t.j...
+00000300: 7404 a101 a101 7d01 7400 6a01 a005 7c01  t.....}.t.j...|.
+00000310: 6402 a102 7d02 7c02 7d00 7a13 7406 7c00  d...}.|.}.z.t.|.
+00000320: 8301 6403 6b02 7229 7407 6404 7c00 1600  ..d.k.r)t.d.|...
+00000330: 6405 6406 8d02 0100 5700 6401 5300 5700  d.d.....W.d.S.W.
+00000340: 6e09 0400 7408 7933 0100 0100 0100 5900  n...t.y3......Y.
+00000350: 6e01 7700 6407 7d03 7409 7c00 6408 8302  n.w.d.}.t.|.d...
+00000360: 8f60 7d04 7407 6409 7c00 1600 6405 6406  .`}.t.d.|...d.d.
+00000370: 8d02 0100 7407 640a 7400 6a01 a00a 7c00  ....t.d.t.j...|.
+00000380: a101 1600 6405 6406 8d02 0100 740b 6a0c  ....d.d.....t.j.
+00000390: 7c03 6405 640b 8d02 7d05 7c05 6a0d a00c  |.d.d...}.|.j...
+000003a0: 640c a101 7d06 640d 7d07 740e 7c06 8301  d...}.d.}.t.|...
+000003b0: 7d06 7c05 6a0f 640e 640f 8d01 4400 5d2a  }.|.j.d.d...D.]*
+000003c0: 7d08 7c07 7410 7c08 8301 3700 7d07 7c04  }.|.t.|...7.}.|.
+000003d0: a011 7c08 a101 0100 740e 6410 7c07 1400  ..|.....t.d.|...
+000003e0: 7c06 1b00 8301 7d09 7412 6a13 a011 6411  |.....}.t.j...d.
+000003f0: 6412 7c09 1400 6413 6410 7c09 1800 1400  d.|...d.d.|.....
+00000400: 6602 1600 a101 0100 7412 6a13 a014 a100  f.......t.j.....
+00000410: 0100 7169 5700 6401 0400 0400 8303 0100  ..qiW.d.........
+00000420: 6e08 3100 739e 7701 0100 0100 0100 5900  n.1.s.w.......Y.
+00000430: 0100 7406 7c00 8301 6403 6b03 72ad 7415  ..t.|...d.k.r.t.
+00000440: 6414 8301 8201 6401 5300 2915 7a95 0a20  d.....d.S.).z.. 
+00000450: 2020 2044 6f77 6e6c 6f61 6420 7468 6520     Download the 
+00000460: 6465 6661 756c 7420 7072 6f6a 6563 7469  default projecti
+00000470: 6f6e 206d 6174 7269 782e 0a0a 2020 2020  on matrix...    
+00000480: 4172 6773 3a0a 2020 2020 2020 2020 6465  Args:.        de
+00000490: 7374 696e 6174 696f 6e20 2873 7472 2c20  stination (str, 
+000004a0: 6f70 7469 6f6e 616c 293a 2050 6174 6820  optional): Path 
+000004b0: 746f 2073 6176 6520 7468 6520 646f 776e  to save the down
+000004c0: 6c6f 6164 6564 2066 696c 652e 2044 6566  loaded file. Def
+000004d0: 6175 6c74 7320 746f 204e 6f6e 652e 0a20  aults to None.. 
+000004e0: 2020 204e fa27 7377 6565 702d 6465 6661     N.'sweep-defa
+000004f0: 756c 742d 7072 6f6a 6563 7469 6f6e 2d6d  ult-projection-m
+00000500: 6174 7269 782d 3630 302e 6d61 74da 2066  atrix-600.mat. f
+00000510: 3138 3538 3761 6337 3963 3435 3265 3431  18587ac79c452e41
+00000520: 3966 3062 6362 3230 3539 6436 3631 397a  9f0bcb2059d6619z
+00000530: 3a54 6865 2064 6566 6175 6c74 2070 726f  :The default pro
+00000540: 6a65 6374 696f 6e20 6d61 7472 6978 2069  jection matrix i
+00000550: 7320 616c 7265 6164 7920 6176 6169 6c61  s already availa
+00000560: 626c 6520 6174 203c 2573 3e54 2901 da05  ble at <%s>T)...
+00000570: 666c 7573 687a a168 7474 7073 3a2f 2f67  flushz.https://g
+00000580: 6974 6875 622e 636f 6d2f 6469 6f67 6f6d  ithub.com/diogom
+00000590: 6163 6861 646f 2d62 696f 696e 666f 2f73  achado-bioinfo/s
+000005a0: 7765 6570 2d64 6566 6175 6c74 2d70 726f  weep-default-pro
+000005b0: 6a65 6374 696f 6e2d 6d61 7472 6978 2f72  jection-matrix/r
+000005c0: 656c 6561 7365 732f 646f 776e 6c6f 6164  eleases/download
+000005d0: 2f73 7765 6570 2d64 6566 6175 6c74 2d70  /sweep-default-p
+000005e0: 726f 6a65 6374 696f 6e2d 6d61 7472 6978  rojection-matrix
+000005f0: 2f73 7765 6570 2d64 6566 6175 6c74 2d70  /sweep-default-p
+00000600: 726f 6a65 6374 696f 6e2d 6d61 7472 6978  rojection-matrix
+00000610: 2d36 3030 2e6d 6174 da02 7762 7a20 5468  -600.mat..wbz Th
+00000620: 6520 646f 776e 6c6f 6164 2064 6573 7469  e download desti
+00000630: 6e61 7469 6f6e 2069 7320 3c25 733e 7a0e  nation is <%s>z.
+00000640: 446f 776e 6c6f 6164 696e 6720 2573 2901  Downloading %s).
+00000650: da06 7374 7265 616d 7a0e 636f 6e74 656e  ..streamz.conten
+00000660: 742d 6c65 6e67 7468 7201 0000 0072 0300  t-lengthr....r..
+00000670: 0000 2901 da0a 6368 756e 6b5f 7369 7a65  ..)...chunk_size
+00000680: e932 0000 007a 070d 5b25 7325 735d fa01  .2...z..[%s%s]..
+00000690: 3dfa 0120 7a0f 446f 776e 6c6f 6164 2066  =.. z.Download f
+000006a0: 6169 6c65 6429 16da 026f 73da 0470 6174  ailed)...os..pat
+000006b0: 68da 0764 6972 6e61 6d65 da08 7265 616c  h..dirname..real
+000006c0: 7061 7468 da08 5f5f 6669 6c65 5f5f da04  path..__file__..
+000006d0: 6a6f 696e 720c 0000 00da 0570 7269 6e74  joinr......print
+000006e0: da11 4669 6c65 4e6f 7446 6f75 6e64 4572  ..FileNotFoundEr
+000006f0: 726f 7272 0d00 0000 da08 6261 7365 6e61  rorr......basena
+00000700: 6d65 da08 7265 7175 6573 7473 da03 6765  me..requests..ge
+00000710: 74da 0768 6561 6465 7273 da03 696e 745a  t..headers..intZ
+00000720: 0c69 7465 725f 636f 6e74 656e 74da 036c  .iter_content..l
+00000730: 656e da05 7772 6974 65da 0373 7973 da06  en..write..sys..
+00000740: 7374 646f 7574 7215 0000 00da 0945 7863  stdoutr......Exc
+00000750: 6570 7469 6f6e 290a da0b 6465 7374 696e  eption)...destin
+00000760: 6174 696f 6eda 086c 6962 4c6f 6361 6cda  ation..libLocal.
+00000770: 0e6d 6174 5f66 696c 655f 6c6f 6361 6cda  .mat_file_local.
+00000780: 046c 696e 6b72 0700 0000 da08 7265 7370  .linkr......resp
+00000790: 6f6e 7365 5a0f 746f 7461 6c5f 6669 6c65  onseZ.total_file
+000007a0: 5f73 697a 65da 0163 da04 6461 7461 da01  _size..c..data..
+000007b0: 7372 0500 0000 7205 0000 0072 0800 0000  sr....r....r....
+000007c0: da0d 646f 776e 5f70 726f 6a5f 6d61 741b  ..down_proj_mat.
+000007d0: 0000 0073 3e00 0000 0807 1401 0e01 0401  ...s>...........
+000007e0: 0202 0c01 1001 0601 04fe 0c03 0401 02ff  ................
+000007f0: 0403 0c02 1001 1801 0e01 0c01 0401 0801  ................
+00000800: 1001 0c01 0a01 1001 2001 0c01 02fb 1cf9  ........ .......
+00000810: 0c0e 0801 04ff 7236 0000 0063 0000 0000  ......r6...c....
+00000820: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+00000830: 4300 0000 730c 0000 0064 017d 0074 007c  C...s....d.}.t.|
+00000840: 0083 0182 0129 027a 590a 2020 2020 5261  .....).zY.    Ra
+00000850: 6973 6520 616e 2065 7863 6570 7469 6f6e  ise an exception
+00000860: 2069 6e64 6963 6174 696e 6720 7468 6174   indicating that
+00000870: 2074 6865 2064 6566 6175 6c74 2070 726f   the default pro
+00000880: 6a65 6374 696f 6e20 6d61 7472 6978 2077  jection matrix w
+00000890: 6173 206e 6f74 2066 6f75 6e64 2e0a 2020  as not found..  
+000008a0: 2020 7a68 4465 6661 756c 7420 7072 6f6a    zhDefault proj
+000008b0: 6563 7469 6f6e 206d 6174 7269 7820 6e6f  ection matrix no
+000008c0: 7420 666f 756e 642c 2074 6f20 646f 776e  t found, to down
+000008d0: 6c6f 6164 2069 7420 7573 653a 0a66 726f  load it use:.fro
+000008e0: 6d20 7377 6565 7020 696d 706f 7274 2064  m sweep import d
+000008f0: 6f77 6e5f 7072 6f6a 5f6d 6174 0a64 6f77  own_proj_mat.dow
+00000900: 6e5f 7072 6f6a 5f6d 6174 2829 2901 722d  n_proj_mat()).r-
+00000910: 0000 0029 015a 0965 7272 6f72 5f73 7472  ...).Z.error_str
+00000920: 7205 0000 0072 0500 0000 7208 0000 00da  r....r....r.....
+00000930: 1f72 6574 7572 6e5f 7072 6f6a 5f6d 6174  .return_proj_mat
+00000940: 5f6e 6f74 5f66 6f75 6e64 5f65 7272 6f72  _not_found_error
+00000950: 4200 0000 7304 0000 0004 0408 0172 3700  B...s........r7.
+00000960: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
+00000970: 0000 0008 0000 0043 0000 0073 3a00 0000  .......C...s:...
+00000980: 7a0f 7400 7c00 8301 6401 6b03 720d 7401  z.t.|...d.k.r.t.
+00000990: 8300 0100 5700 6402 5300 5700 6402 5300  ....W.d.S.W.d.S.
+000009a0: 0400 7402 791c 0100 0100 0100 7401 8300  ..t.y.......t...
+000009b0: 0100 5900 6402 5300 7700 2903 7a83 0a20  ..Y.d.S.w.).z.. 
+000009c0: 2020 2043 6865 636b 2069 6620 7468 6520     Check if the 
+000009d0: 6465 6661 756c 7420 7072 6f6a 6563 7469  default projecti
+000009e0: 6f6e 206d 6174 7269 7820 6578 6973 7473  on matrix exists
+000009f0: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
+00000a00: 2020 2020 2066 696c 6520 2873 7472 293a       file (str):
+00000a10: 2050 6174 6820 746f 2074 6865 2064 6566   Path to the def
+00000a20: 6175 6c74 2070 726f 6a65 6374 696f 6e20  ault projection 
+00000a30: 6d61 7472 6978 2066 696c 652e 0a20 2020  matrix file..   
+00000a40: 2072 1400 0000 4e29 0372 0c00 0000 7237   r....N).r....r7
+00000a50: 0000 0072 2300 0000 2901 da04 6669 6c65  ...r#...)...file
+00000a60: 7205 0000 0072 0500 0000 7208 0000 00da  r....r....r.....
+00000a70: 1663 6865 636b 5f64 6566 6175 6c74 5f70  .check_default_p
+00000a80: 726f 6a5f 6d61 744a 0000 0073 0e00 0000  roj_matJ...s....
+00000a90: 0207 0c01 0c01 06ff 0c02 0c01 02ff 7239  ..............r9
+00000aa0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000ab0: 0400 0000 0500 0000 4300 0000 7358 0000  ........C...sX..
+00000ac0: 0074 006a 01a0 0274 006a 01a0 0374 04a1  .t.j...t.j...t..
+00000ad0: 01a1 017d 0074 006a 01a0 057c 0064 01a1  ...}.t.j...|.d..
+00000ae0: 027d 0174 067c 0183 0101 0074 07a0 087c  .}.t.|.....t...|
+00000af0: 0164 02a1 027d 0274 097c 02a0 0aa1 0083  .d...}.t.|......
+00000b00: 0164 0319 007d 037c 027c 0319 0064 0419  .d...}.|.|...d..
+00000b10: 006a 0b7d 027c 0253 0029 057a 6a0a 2020  .j.}.|.S.).zj.  
+00000b20: 2020 4765 7420 7468 6520 6465 6661 756c    Get the defaul
+00000b30: 7420 7072 6f6a 6563 7469 6f6e 206d 6174  t projection mat
+00000b40: 7269 782e 0a0a 2020 2020 5265 7475 726e  rix...    Return
+00000b50: 733a 0a20 2020 2020 2020 206e 6461 7272  s:.        ndarr
+00000b60: 6179 3a20 5468 6520 6465 6661 756c 7420  ay: The default 
+00000b70: 7072 6f6a 6563 7469 6f6e 206d 6174 7269  projection matri
+00000b80: 782e 0a20 2020 2072 1300 0000 da01 7272  x..    r......rr
+00000b90: 0100 0000 7205 0000 0029 0c72 1c00 0000  ....r....).r....
+00000ba0: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
+00000bb0: 2000 0000 7221 0000 0072 3900 0000 da04   ...r!...r9.....
+00000bc0: 6835 7079 5a04 4669 6c65 da04 6c69 7374  h5pyZ.File..list
+00000bd0: da04 6b65 7973 da01 5429 0472 2f00 0000  ..keys..T).r/...
+00000be0: 7230 0000 005a 086f 7274 685f 6d61 745a  r0...Z.orth_matZ
+00000bf0: 0876 6172 5f6e 616d 6572 0500 0000 7205  .var_namer....r.
+00000c00: 0000 0072 0800 0000 da14 6765 745f 6465  ...r......get_de
+00000c10: 6661 756c 745f 7072 6f6a 5f6d 6174 5800  fault_proj_matX.
+00000c20: 0000 730e 0000 0014 070e 0108 010c 0110  ..s.............
+00000c30: 010e 0104 0172 3f00 0000 2901 4e29 0a72  .....r?...).N).r
+00000c40: 2b00 0000 7225 0000 0072 0b00 0000 721c  +...r%...r....r.
+00000c50: 0000 0072 3b00 0000 720c 0000 0072 3600  ...r;...r....r6.
+00000c60: 0000 7237 0000 0072 3900 0000 723f 0000  ..r7...r9...r?..
+00000c70: 0072 0500 0000 7205 0000 0072 0500 0000  .r....r....r....
+00000c80: 7208 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000c90: 0000 0073 1400 0000 0803 0801 0801 0801  ...s............
+00000ca0: 0801 0802 0a11 0827 0808 0c0e            .......'....
```

## sweep/fas2sweep.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Nov  8 07:19:56 2022 UTC, .py size: 4580 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,229 +1,331 @@
-00000000: 550d 0d0a 0000 0000 1c03 6a63 e411 0000  U.........jc....
+00000000: 6f0d 0d0a 0000 0000 a65e 9f64 5c19 0000  o........^.d\...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0008 0000 0040 0000 0073 9600 0000 6400  .....@...s....d.
+00000020: 0003 0000 0040 0000 0073 9a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
-00000040: 6d04 5a04 6d05 5a05 6d06 5a06 0100 6400  m.Z.m.Z.m.Z...d.
-00000050: 6402 6c07 6d08 5a08 0100 6403 6404 6c09  d.l.m.Z...d.d.l.
-00000060: 5a09 6403 6404 6c0a 5a0a 6403 6404 6c0b  Z.d.d.l.Z.d.d.l.
-00000070: 5a0c 6403 6404 6c0d 5a0e 6403 6404 6c0f  Z.d.d.l.Z.d.d.l.
-00000080: 5a0f 6403 6405 6c10 6d11 5a11 6d12 5a12  Z.d.d.l.m.Z.m.Z.
-00000090: 0100 6403 6406 6c13 6d13 5a13 0100 6403  ..d.d.l.m.Z...d.
-000000a0: 6407 6c14 6d15 5a15 6d16 5a16 0100 6403  d.l.m.Z.m.Z...d.
-000000b0: 6404 6c17 5a17 640e 640c 640d 8401 5a18  d.l.Z.d.d.d...Z.
-000000c0: 6404 5300 290f e901 0000 0029 06da 086d  d.S.)......)...m
-000000d0: 6173 6b32 7665 63da 0e67 656e 6572 6174  ask2vec..generat
-000000e0: 655f 6368 756e 6bda 066c 656e 6774 68da  e_chunk..length.
-000000f0: 0463 6569 6cda 0473 697a 65da 0966 6173  .ceil..size..fas
-00000100: 7461 7265 6164 2901 da16 6368 6563 6b5f  taread)...check_
-00000110: 6465 6661 756c 745f 7072 6f6a 5f6d 6174  default_proj_mat
-00000120: e900 0000 004e 2902 da0a 6c69 6c5f 6d61  .....N)...lil_ma
-00000130: 7472 6978 da06 6873 7461 636b 2901 da04  trix..hstack)...
-00000140: 7471 646d 2902 da08 5061 7261 6c6c 656c  tqdm)...Parallel
-00000150: da07 6465 6c61 7965 6446 e9e8 0300 0054  ..delayedF.....T
-00000160: da02 4141 6309 0000 0000 0000 0000 0000  ..AAc...........
-00000170: 001a 0000 000a 0000 0003 0000 0073 e402  .............s..
-00000180: 0000 7c07 6400 6b08 721a 8805 6401 6b02  ..|.d.k.r...d.k.
-00000190: 7216 6401 7d07 6e04 6402 7d07 8803 6400  r.d.}.n.d.}...d.
-000001a0: 6b08 7232 7400 a001 6403 6404 6403 6703  k.r2t...d.d.d.g.
-000001b0: a101 8903 7c06 6405 6b02 7240 6406 8900  ....|.d.k.r@d...
-000001c0: 6e0c 7c06 6407 6b02 724c 6408 8900 7402  n.|.d.k.rLd...t.
-000001d0: 7403 7404 8803 8301 8301 8301 7d09 7403  t.t.........}.t.
-000001e0: 8803 6409 1900 8803 6403 1900 6702 8301  ..d.....d...g...
-000001f0: 7d0a 7405 8803 8301 640a 6b03 738e 7c09  }.t.....d.k.s.|.
-00000200: 7406 6b02 739c 7c09 7400 6a07 6b02 739c  t.k.s.|.t.j.k.s.
-00000210: 640b 7d0b 7408 7c0b 8301 8201 6e3e 8804  d.}.t.|.....n>..
-00000220: 6400 6b09 72b2 8805 73b2 7408 640c 8301  d.k.r...s.t.d...
-00000230: 8201 6e28 7c0a 640d 6b04 72c2 7c06 6405  ..n(|.d.k.r.|.d.
-00000240: 6b02 73d2 7c0a 640e 6b04 72da 7c06 6407  k.s.|.d.k.r.|.d.
-00000250: 6b02 72da 7408 640f 8301 8201 7409 7c00  k.r.t.d.....t.|.
-00000260: 740a 8302 72ee 740b 7c00 8301 7d0c 6e04  t...r.t.|...}.n.
-00000270: 7c00 7d0c 6700 7d0d 6700 8906 7c0c 4400  |.}.g.}.g...|.D.
-00000280: 5d24 7d0e 8806 a00c 740a 7c0e 6a0d 8301  ]$}.....t.|.j...
-00000290: a101 0100 7c0d a00c 740a 7c0e 6a0e 8301  ....|...t.|.j...
-000002a0: a101 0100 71fe 7400 a001 8806 a101 8906  ....q.t.........
-000002b0: 7400 a001 7c0d a101 7d0d 7400 a00f 7405  t...|...}.t...t.
-000002c0: a101 7d0f 7400 a001 7c0f 8806 8301 a101  ..}.t...|.......
-000002d0: 7d10 7c10 7403 8803 8301 6b00 7d11 7403  }.|.t.....k.}.t.
-000002e0: 7c11 a010 7406 a101 8301 6409 6b04 9001  |...t.....d.k...
-000002f0: 727c 6410 7d0b 7408 7c0b 8301 8201 7411  r|d.}.t.|.....t.
-00000300: 7405 8806 8301 7c04 1b00 8301 7d12 7412  t.....|.....}.t.
-00000310: 7c12 7413 8806 8301 8302 6404 1800 8901  |.t.......d.....
-00000320: 8800 8803 6409 1900 1300 8800 8803 6403  ....d.........d.
-00000330: 1900 1300 1400 7d13 8805 9002 7250 8804  ......}.....rP..
-00000340: 6400 6b08 9002 7232 7c13 6411 6b03 9001  d.k...r2|.d.k...
-00000350: 72dc 6412 7d0b 7408 7c0b 8301 8201 7414  r.d.}.t.|.....t.
-00000360: 6a15 a016 7414 6a15 a017 7418 a101 a101  j...t.j...t.....
-00000370: 7d14 7414 6a15 a019 7c14 6413 a102 7d15  }.t.j...|.d...}.
-00000380: 741a 7c15 8301 0100 741b a01c 7c15 6414  t.|.....t...|.d.
-00000390: a102 8904 7404 8804 a01d a100 8301 6409  ....t.........d.
-000003a0: 1900 7d16 8804 7c16 1900 6415 1900 6a1e  ..}...|...d...j.
-000003b0: 8904 6e1e 741f 8804 8301 6409 1900 7c13  ..n.t.....d...|.
-000003c0: 6b03 9002 7250 6416 7d0b 7408 7c0b 8301  k...rPd.}.t.|...
-000003d0: 8201 8700 8703 6602 6417 6418 8408 8902  ......f.d.d.....
-000003e0: 8701 8702 8704 8705 8706 6605 6419 641a  ..........f.d.d.
-000003f0: 8408 8907 641b 7d17 7420 6a21 641c 7c17  ....d.}.t j!d.|.
-00000400: 641d 8d02 0100 7422 a023 7424 6409 7c12  d.....t".#t$d.|.
-00000410: 8302 a101 7d18 7425 7c08 641e 8d01 8707  ....}.t%|.d.....
-00000420: 6601 641f 6420 8408 7426 7c18 6409 6401  f.d.d ..t&|.d.d.
-00000430: 6421 7427 6a28 7c03 0c00 6422 8d06 4400  d!t'j(|...d"..D.
-00000440: 8301 8301 7d19 7429 7c19 8301 6a1e a02a  ....}.t)|...j..*
-00000450: a100 7d19 7c07 9002 72e0 7c19 a02b a100  ..}.|...r.|..+..
-00000460: 7d19 7c19 5300 2923 4e54 46e9 0200 0000  }.|.S.)#NTF.....
-00000470: 7201 0000 0072 1000 0000 e914 0000 005a  r....r.........Z
-00000480: 024e 54e9 0400 0000 7209 0000 00e9 0300  .NT.....r.......
-00000490: 0000 7a2c 4d61 736b 206d 7573 7420 6265  ..z,Mask must be
-000004a0: 2061 6e20 6172 7261 7920 7769 7468 2033   an array with 3
-000004b0: 2069 6e74 6567 6572 2076 616c 7565 732e   integer values.
-000004c0: 7a3a 5468 6520 6f72 7468 5f6d 6174 2070  z:The orth_mat p
-000004d0: 6172 616d 6574 6572 2069 7320 756e 6e65  arameter is unne
-000004e0: 6365 7373 6172 7920 6966 2070 726f 6a65  cessary if proje
-000004f0: 6374 696f 6e3d 4661 6c73 652e e905 0000  ction=False.....
-00000500: 00e9 0a00 0000 7a27 5468 6520 7369 7a65  ......z'The size
-00000510: 206f 6620 7468 6520 6d61 736b 2070 6172   of the mask par
-00000520: 7473 2069 7320 746f 6f20 6869 6768 2e7a  ts is too high.z
-00000530: 2f54 6865 7265 2061 7265 2073 6571 7565  /There are seque
-00000540: 6e63 6573 2073 6d61 6c6c 6572 2074 6861  nces smaller tha
-00000550: 6e20 7468 6520 6d61 736b 2073 697a 652e  n the mask size.
-00000560: 6900 7102 007a a054 6865 2064 6566 6175  i.q..z.The defau
-00000570: 6c74 206d 6174 7269 7820 6973 2069 6e74  lt matrix is int
-00000580: 656e 6465 6420 666f 7220 7468 6520 7377  ended for the sw
-00000590: 6565 7020 6f66 2061 6d69 6e6f 2061 6369  eep of amino aci
-000005a0: 6473 2077 6974 6820 7468 6520 6465 6661  ds with the defa
-000005b0: 756c 7420 6d61 736b 2c20 666f 7220 6f74  ult mask, for ot
-000005c0: 6865 7220 6361 7365 7320 796f 7520 6361  her cases you ca
-000005d0: 6e20 6469 7361 626c 6520 7468 6520 7072  n disable the pr
-000005e0: 6f6a 6563 7469 6f6e 206f 7220 7365 7420  ojection or set 
-000005f0: 7468 6520 6f72 7468 5f6d 6174 2070 6172  the orth_mat par
-00000600: 616d 6574 6572 2e7a 2773 7765 6570 2d64  ameter.z'sweep-d
-00000610: 6566 6175 6c74 2d70 726f 6a65 6374 696f  efault-projectio
-00000620: 6e2d 6d61 7472 6978 2d36 3030 2e6d 6174  n-matrix-600.mat
-00000630: da01 72a9 007a b554 6865 2064 6566 696e  ..r..z.The defin
-00000640: 6564 206f 7274 685f 6d61 7420 646f 6573  ed orth_mat does
-00000650: 206e 6f74 2068 6176 6520 7468 6520 6170   not have the ap
-00000660: 7072 6f70 7269 6174 6520 6469 6d65 6e73  propriate dimens
-00000670: 696f 6e73 2e0a 5468 6520 6e75 6d62 6572  ions..The number
-00000680: 206f 6620 6c69 6e65 7320 6d75 7374 2062   of lines must b
-00000690: 653a 0a28 782a 2a6d 6173 6b5b 305d 292a  e:.(x**mask[0])*
-000006a0: 2878 2a2a 6d61 736b 5b32 5d29 2c0a 7768  (x**mask[2]),.wh
-000006b0: 6572 6520 783d 3230 2c20 6966 2066 6173  ere x=20, if fas
-000006c0: 7461 5f74 7970 653d 3d27 4141 272c 0a61  ta_type=='AA',.a
-000006d0: 6e64 2078 3d34 2c20 6966 2066 6173 7461  nd x=4, if fasta
-000006e0: 5f74 7970 653d 3d27 4e54 272e 6301 0000  _type=='NT'.c...
-000006f0: 0000 0000 0000 0000 0001 0000 0004 0000  ................
-00000700: 0013 0000 0073 1000 0000 7400 7c00 8801  .....s....t.|...
-00000710: 8800 8303 6401 1900 5300 2902 4e72 0900  ....d...S.).Nr..
-00000720: 0000 2901 7202 0000 0029 01da 0161 2902  ..).r....)...a).
-00000730: da07 6465 6653 697a 65da 046d 6173 6b72  ..defSize..maskr
-00000740: 1800 0000 fa2c 6275 696c 645c 6264 6973  .....,build\bdis
-00000750: 742e 7769 6e2d 616d 6436 345c 6567 675c  t.win-amd64\egg\
-00000760: 7377 6565 705c 6661 7332 7377 6565 702e  sweep\fas2sweep.
-00000770: 7079 da08 3c6c 616d 6264 613e 5700 0000  py..<lambda>W...
-00000780: f300 0000 007a 1b66 6173 3273 7765 6570  .....z.fas2sweep
-00000790: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
-000007a0: 613e 6301 0000 0000 0000 0000 0000 0003  a>c.............
-000007b0: 0000 0009 0000 0013 0000 0073 8200 0000  ...........s....
-000007c0: 8804 7400 a001 7402 7403 8800 7c00 6401  ..t...t.t...|.d.
-000007d0: 6602 1900 8301 7403 8800 7c00 6402 6602  f.....t...|.d.f.
-000007e0: 1900 8301 6402 1700 8302 a101 1900 7d01  ....d.........}.
-000007f0: 7404 a005 7c01 a101 7d01 8803 7260 7400  t...|...}...r`t.
-00000800: a001 7c01 a006 8801 a101 a007 a100 a101  ..|.............
-00000810: 7d02 7400 a008 7c02 8802 a102 7d02 6e18  }.t...|.....}.n.
-00000820: 7c01 a006 8801 a101 7d02 7400 a001 7c02  |.......}.t...|.
-00000830: a007 a100 a101 7d02 7409 7c02 8301 6a0a  ......}.t.|...j.
-00000840: 5300 2903 4e72 0900 0000 7201 0000 0029  S.).Nr....r....)
-00000850: 0bda 026e 70da 0561 7272 6179 da05 7261  ...np..array..ra
-00000860: 6e67 65da 0369 6e74 da02 7064 da06 5365  nge..int..pd..Se
-00000870: 7269 6573 5a05 6170 706c 795a 0774 6f5f  riesZ.applyZ.to_
-00000880: 6c69 7374 da03 646f 7472 0a00 0000 da01  list..dotr......
-00000890: 5429 03da 0169 5a05 7061 7263 4d5a 0557  T)...iZ.parcMZ.W
-000008a0: 3136 306b 2905 da03 6964 78da 036d 3276  160k)...idx..m2v
-000008b0: da08 6f72 7468 5f6d 6174 da0a 7072 6f6a  ..orth_mat..proj
-000008c0: 6563 7469 6f6e da04 7365 7173 7218 0000  ection..seqsr...
-000008d0: 0072 1c00 0000 da0b 7377 6565 705f 6368  .r......sweep_ch
-000008e0: 756e 6b58 0000 0073 1000 0000 0001 3001  unkX...s......0.
-000008f0: 0a01 0401 1401 0e02 0a01 0e01 7a1e 6661  ............z.fa
-00000900: 7332 7377 6565 702e 3c6c 6f63 616c 733e  s2sweep.<locals>
-00000910: 2e73 7765 6570 5f63 6875 6e6b 7a44 2e2a  .sweep_chunkzD.*
-00000920: 4120 776f 726b 6572 2073 746f 7070 6564  A worker stopped
-00000930: 2077 6869 6c65 2073 6f6d 6520 6a6f 6273   while some jobs
-00000940: 2077 6572 6520 6769 7665 6e20 746f 2074   were given to t
-00000950: 6865 2065 7865 6375 746f 725c 2e20 5420  he executor\. T 
-00000960: 2e2a da06 6967 6e6f 7265 2901 da07 6d65  .*..ignore)...me
-00000970: 7373 6167 6529 01da 066e 5f6a 6f62 7363  ssage)...n_jobsc
-00000980: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000990: 0300 0000 3300 0000 731a 0000 007c 005d  ....3...s....|.]
-000009a0: 127d 0174 0088 0083 017c 0183 0156 0001  .}.t.....|...V..
-000009b0: 0071 0264 0053 0029 014e 2901 720e 0000  .q.d.S.).N).r...
-000009c0: 0029 02da 022e 3072 2700 0000 2901 722d  .)....0r'...).r-
-000009d0: 0000 0072 1800 0000 721c 0000 00da 093c  ...r....r......<
-000009e0: 6765 6e65 7870 723e 6500 0000 7304 0000  genexpr>e...s...
-000009f0: 0004 0002 007a 1c66 6173 3273 7765 6570  .....z.fas2sweep
-00000a00: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
-00000a10: 7072 3e7a 0d52 756e 6e69 6e67 2053 5765  pr>z.Running SWe
-00000a20: 6550 2905 da08 706f 7369 7469 6f6e 5a05  eP)...positionZ.
-00000a30: 6c65 6176 65da 0464 6573 63da 0466 696c  leave..desc..fil
-00000a40: 65da 0764 6973 6162 6c65 292c 721f 0000  e..disable),r...
-00000a50: 0072 2000 0000 da04 7479 7065 da03 7375  .r .....type..su
-00000a60: 6dda 046c 6973 74da 036c 656e 7222 0000  m..list..lenr"..
-00000a70: 005a 0569 6e74 3332 da09 4578 6365 7074  .Z.int32..Except
-00000a80: 696f 6eda 0a69 7369 6e73 7461 6e63 65da  ion..isinstance.
-00000a90: 0373 7472 7207 0000 00da 0661 7070 656e  .strr......appen
-00000aa0: 64da 0373 6571 da0b 6465 7363 7269 7074  d..seq..descript
-00000ab0: 696f 6e5a 0976 6563 746f 7269 7a65 5a06  ionZ.vectorizeZ.
-00000ac0: 6173 7479 7065 7205 0000 0072 0300 0000  astyper....r....
-00000ad0: 7204 0000 00da 026f 73da 0470 6174 68da  r......os..path.
-00000ae0: 0764 6972 6e61 6d65 da08 7265 616c 7061  .dirname..realpa
-00000af0: 7468 da08 5f5f 6669 6c65 5f5f da04 6a6f  th..__file__..jo
-00000b00: 696e 7208 0000 00da 0468 3570 795a 0446  inr......h5pyZ.F
-00000b10: 696c 65da 046b 6579 7372 2600 0000 7206  ile..keysr&...r.
-00000b20: 0000 00da 0877 6172 6e69 6e67 73da 0e66  .....warnings..f
-00000b30: 696c 7465 7277 6172 6e69 6e67 7372 2300  ilterwarningsr#.
-00000b40: 0000 7224 0000 0072 2100 0000 720d 0000  ..r$...r!...r...
-00000b50: 0072 0c00 0000 da03 7379 73da 0673 7464  .r......sys..std
-00000b60: 6f75 7472 0b00 0000 5a05 746f 6373 725a  outr....Z.tocsrZ
-00000b70: 0774 6f64 656e 7365 291a 5a04 7866 6173  .todense).Z.xfas
-00000b80: 722a 0000 0072 1b00 0000 da07 7665 7262  r*...r......verb
-00000b90: 6f73 65da 0a63 6875 6e6b 5f73 697a 6572  ose..chunk_sizer
-00000ba0: 2b00 0000 5a0a 6661 7374 615f 7479 7065  +...Z.fasta_type
-00000bb0: 5a0c 7265 7475 726e 5f64 656e 7365 7230  Z.return_denser0
-00000bc0: 0000 005a 096d 6173 6b5f 7479 7065 5a08  ...Z.mask_typeZ.
-00000bd0: 6d61 736b 5f73 756d 722f 0000 005a 0866  mask_sumr/...Z.f
-00000be0: 6173 5f63 656c 6cda 0768 6561 6465 7273  as_cell..headers
-00000bf0: 7227 0000 005a 0476 6c65 6e5a 0873 6571  r'...Z.vlenZ.seq
-00000c00: 5f73 697a 655a 0d68 6561 6465 7273 5f73  _sizeZ.headers_s
-00000c10: 6d61 6c6c da06 6368 756e 6b73 5a09 726f  mall..chunksZ.ro
-00000c20: 7773 5f73 697a 655a 086c 6962 4c6f 6361  ws_sizeZ.libLoca
-00000c30: 6c5a 0e6d 6174 5f66 696c 655f 6c6f 6361  lZ.mat_file_loca
-00000c40: 6cda 0876 6172 5f6e 616d 655a 0377 6172  l..var_nameZ.war
-00000c50: 5a07 7261 6e67 655f 735a 0972 6573 756c  Z.range_sZ.resul
-00000c60: 744d 6174 7218 0000 0029 0872 1a00 0000  tMatr....).r....
-00000c70: 7228 0000 0072 2900 0000 721b 0000 0072  r(...r)...r....r
-00000c80: 2a00 0000 722b 0000 0072 2c00 0000 722d  *...r+...r,...r-
-00000c90: 0000 0072 1c00 0000 da09 6661 7332 7377  ...r......fas2sw
-00000ca0: 6565 700e 0000 0073 9600 0000 0003 0801  eep....s........
-00000cb0: 0801 0602 0401 0801 1001 0801 0601 0801  ................
-00000cc0: 0401 1001 1401 1e01 0401 0a01 0c01 0a01  ................
-00000cd0: 1001 06ff 0201 06ff 0202 0802 0a01 0a02  ................
-00000ce0: 0401 0401 0401 0801 1001 1201 0a01 0a02  ................
-00000cf0: 0a01 0e01 0c01 1401 0401 0802 1001 1201  ................
-00000d00: 1801 0601 0a01 0a01 0404 0802 1401 0801  ................
-00000d10: 02ff 0402 0801 0c01 1001 1002 1201 0406  ................
-00000d20: 0802 0e01 140a 0401 0e01 1001 1401 0200  ................
-00000d30: 0200 0200 0200 0401 04fe 0c03 0e02 0601  ................
-00000d40: 0801 7252 0000 0029 084e 4e46 720f 0000  ..rR...).NNFr...
-00000d50: 0054 7210 0000 004e 7201 0000 0029 195a  .Tr....Nr....).Z
-00000d60: 0d73 7765 6570 5f73 7570 706f 7274 7202  .sweep_supportr.
-00000d70: 0000 0072 0300 0000 7204 0000 0072 0500  ...r....r....r..
-00000d80: 0000 7206 0000 0072 0700 0000 5a14 6465  ..r....r....Z.de
-00000d90: 6661 756c 745f 7072 6f6a 5f6d 6174 5f6f  fault_proj_mat_o
-00000da0: 7065 7208 0000 0072 4700 0000 7241 0000  per....rG...rA..
-00000db0: 00da 056e 756d 7079 721f 0000 005a 0670  ...numpyr....Z.p
-00000dc0: 616e 6461 7372 2300 0000 724b 0000 005a  andasr#...rK...Z
-00000dd0: 0c73 6369 7079 2e73 7061 7273 6572 0a00  .scipy.sparser..
-00000de0: 0000 720b 0000 0072 0c00 0000 5a06 6a6f  ..r....r....Z.jo
-00000df0: 626c 6962 720d 0000 0072 0e00 0000 7249  blibr....r....rI
-00000e00: 0000 0072 5200 0000 7218 0000 0072 1800  ...rR...r....r..
-00000e10: 0000 7218 0000 0072 1c00 0000 da08 3c6d  ..r....r......<m
-00000e20: 6f64 756c 653e 0300 0000 7320 0000 0020  odule>....s ... 
-00000e30: 010c 0108 0108 0108 0108 0108 0110 010c  ................
-00000e40: 0110 0108 0100 0100 0000 0000 0100 fe    ...............
+00000040: 0100 6400 6402 6c04 6d05 5a05 6d06 5a06  ..d.d.l.m.Z.m.Z.
+00000050: 0100 6400 6403 6c07 6d08 5a08 0100 6404  ..d.d.l.m.Z...d.
+00000060: 6405 6c09 5a09 6404 6405 6c0a 5a0a 6404  d.l.Z.d.d.l.Z.d.
+00000070: 6405 6c0b 5a0b 6404 6405 6c0c 5a0d 6404  d.l.Z.d.d.l.Z.d.
+00000080: 6405 6c0e 5a0e 6404 6406 6c0f 6d10 5a10  d.l.Z.d.d.l.m.Z.
+00000090: 6d11 5a11 0100 6404 6407 6c12 6d12 5a12  m.Z...d.d.l.m.Z.
+000000a0: 0100 6404 6408 6c13 6d14 5a14 6d15 5a15  ..d.d.l.m.Z.m.Z.
+000000b0: 0100 0909 090c 0905 0900 6410 640e 640f  ..........d.d.d.
+000000c0: 8401 5a16 6405 5300 2911 e901 0000 0029  ..Z.d.S.)......)
+000000d0: 03da 0c6d 6173 6b32 7665 635f 6269 6eda  ...mask2vec_bin.
+000000e0: 0e6d 6173 6b32 7665 635f 636f 756e 74da  .mask2vec_count.
+000000f0: 0e67 656e 6572 6174 655f 6368 756e 6b29  .generate_chunk)
+00000100: 02da 0966 6173 7461 7265 6164 da12 6361  ...fastaread..ca
+00000110: 6c63 5f70 726f 6a5f 6d61 745f 7369 7a65  lc_proj_mat_size
+00000120: 2901 da16 6368 6563 6b5f 6465 6661 756c  )...check_defaul
+00000130: 745f 7072 6f6a 5f6d 6174 e900 0000 004e  t_proj_mat.....N
+00000140: 2902 da0a 6c69 6c5f 6d61 7472 6978 da06  )...lil_matrix..
+00000150: 7673 7461 636b 2901 da04 7471 646d 2902  vstack)...tqdm).
+00000160: da08 5061 7261 6c6c 656c da07 6465 6c61  ..Parallel..dela
+00000170: 7965 64da 0662 696e 6172 7946 e9e8 0300  yed..binaryF....
+00000180: 0054 da02 4141 630b 0000 0000 0000 0000  .T..AAc.........
+00000190: 0000 001b 0000 000a 0000 0003 0000 0073  ...............s
+000001a0: e202 0000 8801 6401 7500 720d 8808 720a  ......d.u.r...r.
+000001b0: 7400 6a01 8901 6e03 7400 6a02 8901 8805  t.j...n.t.j.....
+000001c0: 6401 7500 7218 7400 a003 6700 6402 a201  d.u.r.t...g.d...
+000001d0: a101 8905 7c07 6403 6b02 721f 6404 8900  ....|.d.k.r.d...
+000001e0: 6e06 7c07 6405 6b02 7225 6406 8900 7404  n.|.d.k.r%d...t.
+000001f0: 7405 7406 8805 8301 8301 8301 7d0b 7405  t.t.........}.t.
+00000200: 8805 6407 1900 8805 6408 1900 6702 8301  ..d.....d...g...
+00000210: 7d0c 7407 8805 8301 6409 6b03 7346 7c0b  }.t.....d.k.sF|.
+00000220: 7408 6b02 734c 7c0b 7400 6a02 6b02 734c  t.k.sL|.t.j.k.sL
+00000230: 640a 7d0d 7409 7c0d 8301 8201 8807 6401  d.}.t.|.......d.
+00000240: 7501 7256 8808 7356 7409 640b 8301 8201  u.rV..sVt.d.....
+00000250: 7c0c 640c 6b04 725e 7c07 6403 6b02 7366  |.d.k.r^|.d.k.sf
+00000260: 7c0c 640d 6b04 726a 7c07 6405 6b02 726a  |.d.k.rj|.d.k.rj
+00000270: 7409 640e 8301 8201 740a 7c00 740b 8302  t.d.....t.|.t...
+00000280: 7274 740c 7c00 8301 7d0e 6e02 7c00 7d0e  rtt.|...}.n.|.}.
+00000290: 6700 8909 7c0e 4400 5d0a 7d0f 8809 a00d  g...|.D.].}.....
+000002a0: 740b 7c0f 6a0e 8301 a101 0100 717a 740f  t.|.j.......qzt.
+000002b0: a010 7407 8809 8301 7c05 1b00 a101 7d10  ..t.....|.....}.
+000002c0: 7407 8809 8301 7d11 7c08 73af 7405 8805  t.....}.|.s.t...
+000002d0: 8301 7d12 7411 8809 8301 4400 5d12 5c02  ..}.t.....D.].\.
+000002e0: 7d0f 7d13 7407 7c13 8301 7c12 6b00 72ae  }.}.t.|...|.k.r.
+000002f0: 640f 7c0f 1600 7d0d 7409 7c0d 8301 8201  d.|...}.t.|.....
+00000300: 719c 7412 7c10 7c11 8302 6410 1800 8902  q.t.|.|...d.....
+00000310: 8800 8805 6407 1900 1300 8800 8805 6408  ....d.........d.
+00000320: 1900 1300 1400 7d14 8808 9001 721e 8807  ......}.....r...
+00000330: 6401 7500 72fe 7c14 6411 6b03 72d3 6412  d.u.r.|.d.k.r.d.
+00000340: 7d0d 7409 7c0d 8301 8201 7413 6a14 a015  }.t.|.....t.j...
+00000350: 7413 6a14 a016 7417 a101 a101 7d15 7413  t.j...t.....}.t.
+00000360: 6a14 a018 7c15 6413 a102 7d16 7419 7c16  j...|.d...}.t.|.
+00000370: 8301 0100 741a a01b 7c16 6414 a102 8907  ....t...|.d.....
+00000380: 7406 8807 a01c a100 8301 6407 1900 7d17  t.........d...}.
+00000390: 8807 7c17 1900 6415 1900 6a1d 8907 6e16  ..|...d...j...n.
+000003a0: 8807 6a1e 6407 1900 7c14 6b03 9001 7214  ..j.d...|.k...r.
+000003b0: 741f 8805 7c07 8302 7d18 6416 a020 7c18  t...|...}.d.. |.
+000003c0: a101 7d0d 7409 7c0d 8301 8201 8807 a021  ..}.t.|........!
+000003d0: 8801 a101 8907 8807 6a1e 6410 1900 8903  ........j.d.....
+000003e0: 7c03 6417 6b02 9001 7226 7422 8906 6e07  |.d.k...r&t"..n.
+000003f0: 7c03 6418 6b02 9001 722d 7423 8906 8700  |.d.k...r-t#....
+00000400: 8705 8706 6603 6419 641a 8408 8904 8701  ....f.d.d.......
+00000410: 8702 8703 8704 8707 8708 8709 6607 641b  ............f.d.
+00000420: 641c 8408 890a 7424 6407 7c10 8302 7d19  d.....t$d.|...}.
+00000430: 7425 7c0a 641d 641e 8d02 870a 6601 641f  t%|.d.d.....f.d.
+00000440: 6420 8408 7426 7c19 6407 6421 6422 7427  d ..t&|.d.d!d"t'
+00000450: 6a28 7c04 0c00 6423 8d06 4400 8301 8301  j(|...d#..D.....
+00000460: 7d1a 8808 9001 7269 7400 a029 7c1a a101  }.....rit..)|...
+00000470: 7d1a 7c1a 5300 742a 7429 7c1a 8301 8301  }.|.S.t*t)|.....
+00000480: 7d1a 7c1a 5300 2924 61e3 0400 000a 2020  }.|.S.)$a.....  
+00000490: 2020 5065 7266 6f72 6d20 7468 6520 5357    Perform the SW
+000004a0: 6565 5020 616c 676f 7269 7468 6d20 6f6e  eeP algorithm on
+000004b0: 2073 6571 7565 6e63 6573 2069 6e20 4641   sequences in FA
+000004c0: 5354 4120 666f 726d 6174 2e0a 0a20 2020  STA format...   
+000004d0: 2041 7267 733a 0a20 2020 2020 2020 2078   Args:.        x
+000004e0: 6661 7320 2873 7472 206f 7220 6c69 7374  fas (str or list
+000004f0: 293a 2050 6174 6820 746f 2074 6865 2046  ): Path to the F
+00000500: 4153 5441 2066 696c 6520 6f72 2061 206c  ASTA file or a l
+00000510: 6973 7420 6f66 2046 4153 5441 2073 6571  ist of FASTA seq
+00000520: 7565 6e63 6573 2e0a 2020 2020 2020 2020  uences..        
+00000530: 6f72 7468 5f6d 6174 2028 6e64 6172 7261  orth_mat (ndarra
+00000540: 792c 206f 7074 696f 6e61 6c29 3a20 5072  y, optional): Pr
+00000550: 6f6a 6563 7469 6f6e 206d 6174 7269 782e  ojection matrix.
+00000560: 2049 6620 6e6f 7420 7072 6f76 6964 6564   If not provided
+00000570: 2c20 7468 6520 6465 6661 756c 7420 6d61  , the default ma
+00000580: 7472 6978 2077 696c 6c20 6265 2075 7365  trix will be use
+00000590: 642e 0a20 2020 2020 2020 206d 6173 6b20  d..        mask 
+000005a0: 286e 6461 7272 6179 2c20 6f70 7469 6f6e  (ndarray, option
+000005b0: 616c 293a 204d 6173 6b20 666f 7220 656e  al): Mask for en
+000005c0: 636f 6469 6e67 2e20 4966 206e 6f74 2070  coding. If not p
+000005d0: 726f 7669 6465 642c 2074 6865 2064 6566  rovided, the def
+000005e0: 6175 6c74 206d 6173 6b20 5b32 2c20 312c  ault mask [2, 1,
+000005f0: 2032 5d20 7769 6c6c 2062 6520 7573 6564   2] will be used
+00000600: 2e0a 2020 2020 2020 2020 636f 6d70 6f73  ..        compos
+00000610: 6974 696f 6e20 2873 7472 2c20 6f70 7469  ition (str, opti
+00000620: 6f6e 616c 293a 2043 6f6d 706f 7369 7469  onal): Compositi
+00000630: 6f6e 2074 7970 652e 2045 6974 6865 7220  on type. Either 
+00000640: 2762 696e 6172 7927 206f 7220 2763 6f75  'binary' or 'cou
+00000650: 6e74 272e 2044 6566 6175 6c74 7320 746f  nt'. Defaults to
+00000660: 2027 6269 6e61 7279 272e 0a20 2020 2020   'binary'..     
+00000670: 2020 2076 6572 626f 7365 2028 626f 6f6c     verbose (bool
+00000680: 2c20 6f70 7469 6f6e 616c 293a 2056 6572  , optional): Ver
+00000690: 626f 7369 7479 206d 6f64 652e 2044 6566  bosity mode. Def
+000006a0: 6175 6c74 7320 746f 2046 616c 7365 2e0a  aults to False..
+000006b0: 2020 2020 2020 2020 6368 756e 6b5f 7369          chunk_si
+000006c0: 7a65 2028 696e 742c 206f 7074 696f 6e61  ze (int, optiona
+000006d0: 6c29 3a20 5369 7a65 206f 6620 6561 6368  l): Size of each
+000006e0: 2063 6875 6e6b 2066 6f72 2063 6f6e 6375   chunk for concu
+000006f0: 7272 656e 7420 7072 6f63 6573 7369 6e67  rrent processing
+00000700: 2062 7920 6a6f 622e 2044 6566 6175 6c74   by job. Default
+00000710: 7320 746f 2031 3030 302e 0a20 2020 2020  s to 1000..     
+00000720: 2020 2070 726f 6a65 6374 696f 6e20 2862     projection (b
+00000730: 6f6f 6c2c 206f 7074 696f 6e61 6c29 3a20  ool, optional): 
+00000740: 5065 7266 6f72 6d20 7072 6f6a 6563 7469  Perform projecti
+00000750: 6f6e 2e20 4465 6661 756c 7473 2074 6f20  on. Defaults to 
+00000760: 5472 7565 2e0a 2020 2020 2020 2020 6661  True..        fa
+00000770: 7374 615f 7479 7065 2028 7374 722c 206f  sta_type (str, o
+00000780: 7074 696f 6e61 6c29 3a20 5479 7065 206f  ptional): Type o
+00000790: 6620 4641 5354 4120 7365 7175 656e 6365  f FASTA sequence
+000007a0: 732e 2045 6974 6865 7220 2741 4127 2066  s. Either 'AA' f
+000007b0: 6f72 2061 6d69 6e6f 2061 6369 6473 206f  or amino acids o
+000007c0: 7220 274e 5427 2066 6f72 206e 7563 6c65  r 'NT' for nucle
+000007d0: 6f74 6964 6573 2e20 4465 6661 756c 7473  otides. Defaults
+000007e0: 2074 6f20 2741 4127 2e0a 2020 2020 2020   to 'AA'..      
+000007f0: 2020 736b 6970 5f73 6571 5f6c 656e 5f63    skip_seq_len_c
+00000800: 6865 636b 2028 626f 6f6c 2c20 6f70 7469  heck (bool, opti
+00000810: 6f6e 616c 293a 2053 6b69 7020 7468 6520  onal): Skip the 
+00000820: 6368 6563 6b20 666f 7220 7365 7175 656e  check for sequen
+00000830: 6365 206c 656e 6774 682e 2044 6566 6175  ce length. Defau
+00000840: 6c74 7320 746f 2046 616c 7365 2e0a 2020  lts to False..  
+00000850: 2020 2020 2020 6474 7970 6520 2864 7479        dtype (dty
+00000860: 7065 2c20 6f70 7469 6f6e 616c 293a 2044  pe, optional): D
+00000870: 6174 6120 7479 7065 206f 6620 7468 6520  ata type of the 
+00000880: 6f75 7470 7574 206d 6174 7269 782e 2049  output matrix. I
+00000890: 6620 6e6f 7420 7072 6f76 6964 6564 2c20  f not provided, 
+000008a0: 666c 6f61 7433 3220 6973 2075 7365 6420  float32 is used 
+000008b0: 666f 7220 7072 6f6a 6563 7469 6f6e 2061  for projection a
+000008c0: 6e64 2069 6e74 3332 2066 6f72 206e 6f20  nd int32 for no 
+000008d0: 7072 6f6a 6563 7469 6f6e 2e0a 2020 2020  projection..    
+000008e0: 2020 2020 6e5f 6a6f 6273 2028 696e 742c      n_jobs (int,
+000008f0: 206f 7074 696f 6e61 6c29 3a20 4e75 6d62   optional): Numb
+00000900: 6572 206f 6620 7061 7261 6c6c 656c 206a  er of parallel j
+00000910: 6f62 732e 2044 6566 6175 6c74 7320 746f  obs. Defaults to
+00000920: 2031 2e0a 0a20 2020 2052 6574 7572 6e73   1...    Returns
+00000930: 3a0a 2020 2020 2020 2020 6e64 6172 7261  :.        ndarra
+00000940: 7920 6f72 2073 7061 7273 6520 6d61 7472  y or sparse matr
+00000950: 6978 3a20 5265 7375 6c74 696e 6720 5357  ix: Resulting SW
+00000960: 6565 5020 6d61 7472 6978 2e0a 2020 2020  eeP matrix..    
+00000970: 4e29 03e9 0200 0000 7201 0000 0072 1100  N)......r....r..
+00000980: 0000 7210 0000 00e9 1400 0000 5a02 4e54  ..r.........Z.NT
+00000990: e904 0000 0072 0800 0000 7211 0000 00e9  .....r....r.....
+000009a0: 0300 0000 7a2c 4d61 736b 206d 7573 7420  ....z,Mask must 
+000009b0: 6265 2061 6e20 6172 7261 7920 7769 7468  be an array with
+000009c0: 2033 2069 6e74 6567 6572 2076 616c 7565   3 integer value
+000009d0: 732e 7a3a 5468 6520 6f72 7468 5f6d 6174  s.z:The orth_mat
+000009e0: 2070 6172 616d 6574 6572 2069 7320 756e   parameter is un
+000009f0: 6e65 6365 7373 6172 7920 6966 2070 726f  necessary if pro
+00000a00: 6a65 6374 696f 6e3d 4661 6c73 652e e905  jection=False...
+00000a10: 0000 00e9 0a00 0000 7a27 5468 6520 7369  ........z'The si
+00000a20: 7a65 206f 6620 7468 6520 6d61 736b 2070  ze of the mask p
+00000a30: 6172 7473 2069 7320 746f 6f20 6869 6768  arts is too high
+00000a40: 2e7a 2753 6571 7565 6e63 6520 2569 2073  .z'Sequence %i s
+00000a50: 6d61 6c6c 6572 2074 6861 6e20 7468 6520  maller than the 
+00000a60: 6d61 736b 2073 697a 652e 7201 0000 0069  mask size.r....i
+00000a70: 0071 0200 7aa0 5468 6520 6465 6661 756c  .q..z.The defaul
+00000a80: 7420 6d61 7472 6978 2069 7320 696e 7465  t matrix is inte
+00000a90: 6e64 6564 2066 6f72 2074 6865 2073 7765  nded for the swe
+00000aa0: 6570 206f 6620 616d 696e 6f20 6163 6964  ep of amino acid
+00000ab0: 7320 7769 7468 2074 6865 2064 6566 6175  s with the defau
+00000ac0: 6c74 206d 6173 6b2c 2066 6f72 206f 7468  lt mask, for oth
+00000ad0: 6572 2063 6173 6573 2079 6f75 2063 616e  er cases you can
+00000ae0: 2064 6973 6162 6c65 2074 6865 2070 726f   disable the pro
+00000af0: 6a65 6374 696f 6e20 6f72 2073 6574 2074  jection or set t
+00000b00: 6865 206f 7274 685f 6d61 7420 7061 7261  he orth_mat para
+00000b10: 6d65 7465 722e 7a27 7377 6565 702d 6465  meter.z'sweep-de
+00000b20: 6661 756c 742d 7072 6f6a 6563 7469 6f6e  fault-projection
+00000b30: 2d6d 6174 7269 782d 3630 302e 6d61 74da  -matrix-600.mat.
+00000b40: 0172 a900 6177 0100 0054 6865 2064 6566  .r..aw...The def
+00000b50: 696e 6564 206f 7274 685f 6d61 7420 646f  ined orth_mat do
+00000b60: 6573 206e 6f74 2068 6176 6520 7468 6520  es not have the 
+00000b70: 6170 7072 6f70 7269 6174 6520 6469 6d65  appropriate dime
+00000b80: 6e73 696f 6e73 2e0a 0a54 6865 206e 756d  nsions...The num
+00000b90: 6265 7220 6f66 206c 696e 6573 206d 7573  ber of lines mus
+00000ba0: 7420 6265 3a0a 2878 2a2a 6d61 736b 5b30  t be:.(x**mask[0
+00000bb0: 5d29 2a28 782a 2a6d 6173 6b5b 325d 292c  ])*(x**mask[2]),
+00000bc0: 0a77 6865 7265 2078 3d32 302c 2069 6620  .where x=20, if 
+00000bd0: 6661 7374 615f 7479 7065 3d3d 2741 4127  fasta_type=='AA'
+00000be0: 2c0a 616e 6420 783d 342c 2069 6620 6661  ,.and x=4, if fa
+00000bf0: 7374 615f 7479 7065 3d3d 274e 5427 2e0a  sta_type=='NT'..
+00000c00: 0a55 7369 6e67 2074 6865 2066 756e 6374  .Using the funct
+00000c10: 696f 6e20 7377 6565 702e 6361 6c63 5f70  ion sweep.calc_p
+00000c20: 726f 6a5f 6d61 745f 7369 7a65 2069 7320  roj_mat_size is 
+00000c30: 706f 7373 6962 6c65 2074 6f20 6368 6563  possible to chec
+00000c40: 6b20 7468 6520 6e65 6365 7373 6172 7920  k the necessary 
+00000c50: 7369 7a65 2061 6e64 2073 7765 6570 2e6f  size and sweep.o
+00000c60: 7274 6862 6173 6520 746f 2063 7265 6174  rthbase to creat
+00000c70: 6520 7468 6520 7072 6f6a 6563 7469 6f6e  e the projection
+00000c80: 206d 6174 2e0a 0a57 6974 6820 7468 6520   mat...With the 
+00000c90: 6375 7272 656e 7420 696e 7075 742c 2074  current input, t
+00000ca0: 6865 206e 756d 6265 7220 6f66 206c 696e  he number of lin
+00000cb0: 6573 2073 686f 756c 6420 6265 207b 7d2e  es should be {}.
+00000cc0: 720e 0000 00da 0563 6f75 6e74 6301 0000  r......countc...
+00000cd0: 0000 0000 0000 0000 0001 0000 0004 0000  ................
+00000ce0: 0013 0000 0073 1000 0000 8802 7c00 8801  .....s......|...
+00000cf0: 8800 8303 6401 1900 5300 2902 4e72 0800  ....d...S.).Nr..
+00000d00: 0000 7218 0000 0029 01da 0161 2903 da07  ..r....)...a)...
+00000d10: 6465 6653 697a 65da 046d 6173 6bda 086d  defSize..mask..m
+00000d20: 6173 6b32 7665 6372 1800 0000 fa2c 6275  ask2vecr.....,bu
+00000d30: 696c 645c 6264 6973 742e 7769 6e2d 616d  ild\bdist.win-am
+00000d40: 6436 345c 6567 675c 7377 6565 705c 6661  d64\egg\sweep\fa
+00000d50: 7332 7377 6565 702e 7079 da08 3c6c 616d  s2sweep.py..<lam
+00000d60: 6264 613e 8200 0000 7302 0000 0010 007a  bda>....s......z
+00000d70: 1b66 6173 3273 7765 6570 2e3c 6c6f 6361  .fas2sweep.<loca
+00000d80: 6c73 3e2e 3c6c 616d 6264 613e 6301 0000  ls>.<lambda>c...
+00000d90: 0000 0000 0000 0000 0005 0000 0006 0000  ................
+00000da0: 0013 0000 0073 8800 0000 8806 7400 8801  .....s......t...
+00000db0: 7c00 6401 6602 1900 8301 7400 8801 7c00  |.d.f.....t...|.
+00000dc0: 6402 6602 1900 8301 6402 1700 8502 1900  d.f.....d.......
+00000dd0: 7d01 7401 6a02 8703 6601 6403 6404 8408  }.t.j...f.d.d...
+00000de0: 7c01 4400 8301 8800 6405 8d02 7d02 8805  |.D.....d...}...
+00000df0: 723c 7c02 6a03 6401 1900 7d03 7401 6a04  r<|.j.d...}.t.j.
+00000e00: 7c03 8802 6602 8800 6405 8d02 7d04 7401  |...f...d...}.t.
+00000e10: 6a05 7c02 8804 7c04 6406 8d03 7d02 7c02  j.|...|.d...}.|.
+00000e20: 5300 7406 7c02 8800 6405 8d02 7d02 7c02  S.t.|...d...}.|.
+00000e30: 5300 2907 4e72 0800 0000 7201 0000 0063  S.).Nr....r....c
+00000e40: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000e50: 0400 0000 1300 0000 7314 0000 0067 007c  ........s....g.|
+00000e60: 005d 067d 0188 007c 0183 0191 0271 0253  .].}...|.....q.S
+00000e70: 0072 1800 0000 7218 0000 0029 02da 022e  .r....r....)....
+00000e80: 30da 0178 2901 da03 6d32 7672 1800 0000  0..x)...m2vr....
+00000e90: 721e 0000 00da 0a3c 6c69 7374 636f 6d70  r......<listcomp
+00000ea0: 3e86 0000 0073 0200 0000 1400 7a32 6661  >....s......z2fa
+00000eb0: 7332 7377 6565 702e 3c6c 6f63 616c 733e  s2sweep.<locals>
+00000ec0: 2e73 7765 6570 5f63 6875 6e6b 2e3c 6c6f  .sweep_chunk.<lo
+00000ed0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+00000ee0: 2901 da05 6474 7970 6529 01da 036f 7574  )...dtype)...out
+00000ef0: 2907 da03 696e 74da 026e 70da 0561 7272  )...int..np..arr
+00000f00: 6179 da05 7368 6170 655a 057a 6572 6f73  ay..shapeZ.zeros
+00000f10: da03 646f 7472 0900 0000 2905 da01 695a  ..dotr....)...iZ
+00000f20: 0570 6172 634d 5a07 6f75 745f 6d61 74da  .parcMZ.out_mat.
+00000f30: 016e 7225 0000 0029 0772 2400 0000 da03  .nr%...).r$.....
+00000f40: 6964 78da 016d 7222 0000 00da 086f 7274  idx..mr".....ort
+00000f50: 685f 6d61 74da 0a70 726f 6a65 6374 696f  h_mat..projectio
+00000f60: 6eda 0473 6571 7372 1800 0000 721e 0000  n..seqsr....r...
+00000f70: 00da 0b73 7765 6570 5f63 6875 6e6b 8400  ...sweep_chunk..
+00000f80: 0000 7312 0000 0028 011c 0104 010a 0112  ..s....(........
+00000f90: 0110 0104 030c ff04 017a 1e66 6173 3273  .........z.fas2s
+00000fa0: 7765 6570 2e3c 6c6f 6361 6c73 3e2e 7377  weep.<locals>.sw
+00000fb0: 6565 705f 6368 756e 6bda 0774 6872 6561  eep_chunk..threa
+00000fc0: 6473 2902 da06 6e5f 6a6f 6273 5a06 7072  ds)...n_jobsZ.pr
+00000fd0: 6566 6572 6301 0000 0000 0000 0000 0000  eferc...........
+00000fe0: 0002 0000 0003 0000 0033 0000 0073 1c00  .........3...s..
+00000ff0: 0000 8100 7c00 5d09 7d01 7400 8800 8301  ....|.].}.t.....
+00001000: 7c01 8301 5600 0100 7102 6400 5300 2901  |...V...q.d.S.).
+00001010: 4e29 0172 0d00 0000 2902 7220 0000 0072  N).r....).r ...r
+00001020: 2b00 0000 2901 7232 0000 0072 1800 0000  +...).r2...r....
+00001030: 721e 0000 00da 093c 6765 6e65 7870 723e  r......<genexpr>
+00001040: 9200 0000 7304 0000 0002 801a 007a 1c66  ....s........z.f
+00001050: 6173 3273 7765 6570 2e3c 6c6f 6361 6c73  as2sweep.<locals
+00001060: 3e2e 3c67 656e 6578 7072 3e54 7a0d 5275  >.<genexpr>Tz.Ru
+00001070: 6e6e 696e 6720 5357 6565 5029 05da 0870  nning SWeeP)...p
+00001080: 6f73 6974 696f 6e5a 056c 6561 7665 da04  ositionZ.leave..
+00001090: 6465 7363 da04 6669 6c65 da07 6469 7361  desc..file..disa
+000010a0: 626c 6529 2b72 2700 0000 5a07 666c 6f61  ble)+r'...Z.floa
+000010b0: 7433 325a 0569 6e74 3332 7228 0000 00da  t32Z.int32r(....
+000010c0: 0474 7970 65da 0373 756d da04 6c69 7374  .type..sum..list
+000010d0: da03 6c65 6e72 2600 0000 da09 4578 6365  ..lenr&.....Exce
+000010e0: 7074 696f 6eda 0a69 7369 6e73 7461 6e63  ption..isinstanc
+000010f0: 65da 0373 7472 7205 0000 00da 0661 7070  e..strr......app
+00001100: 656e 64da 0373 6571 da04 6d61 7468 da04  end..seq..math..
+00001110: 6365 696c da09 656e 756d 6572 6174 6572  ceil..enumerater
+00001120: 0400 0000 da02 6f73 da04 7061 7468 da07  ......os..path..
+00001130: 6469 726e 616d 65da 0872 6561 6c70 6174  dirname..realpat
+00001140: 68da 085f 5f66 696c 655f 5fda 046a 6f69  h..__file__..joi
+00001150: 6e72 0700 0000 da04 6835 7079 5a04 4669  nr......h5pyZ.Fi
+00001160: 6c65 da04 6b65 7973 da01 5472 2900 0000  le..keys..Tr)...
+00001170: 7206 0000 00da 0666 6f72 6d61 745a 0661  r......formatZ.a
+00001180: 7374 7970 6572 0200 0000 7203 0000 00da  styper....r.....
+00001190: 0572 616e 6765 720c 0000 0072 0b00 0000  .ranger....r....
+000011a0: da03 7379 73da 0673 7464 6f75 7472 0a00  ..sys..stdoutr..
+000011b0: 0000 7209 0000 0029 1b5a 0478 6661 7372  ..r....).Z.xfasr
+000011c0: 2f00 0000 721c 0000 005a 0b63 6f6d 706f  /...r....Z.compo
+000011d0: 7369 7469 6f6e da07 7665 7262 6f73 65da  sition..verbose.
+000011e0: 0a63 6875 6e6b 5f73 697a 6572 3000 0000  .chunk_sizer0...
+000011f0: 5a0a 6661 7374 615f 7479 7065 5a12 736b  Z.fasta_typeZ.sk
+00001200: 6970 5f73 6571 5f6c 656e 5f63 6865 636b  ip_seq_len_check
+00001210: 7224 0000 0072 3400 0000 5a09 6d61 736b  r$...r4...Z.mask
+00001220: 5f74 7970 655a 086d 6173 6b5f 7375 6dda  _typeZ.mask_sum.
+00001230: 076d 6573 7361 6765 5a08 6661 735f 6365  .messageZ.fas_ce
+00001240: 6c6c 722b 0000 00da 0663 6875 6e6b 735a  llr+.....chunksZ
+00001250: 086c 656e 5f73 6571 735a 0873 756d 5f6d  .len_seqsZ.sum_m
+00001260: 6173 6b72 2c00 0000 5a09 726f 7773 5f73  askr,...Z.rows_s
+00001270: 697a 655a 086c 6962 4c6f 6361 6c5a 0e6d  izeZ.libLocalZ.m
+00001280: 6174 5f66 696c 655f 6c6f 6361 6c5a 0876  at_file_localZ.v
+00001290: 6172 5f6e 616d 655a 0c6d 6174 5f73 697a  ar_nameZ.mat_siz
+000012a0: 655f 6e65 635a 0772 616e 6765 5f73 5a0a  e_necZ.range_sZ.
+000012b0: 7265 7375 6c74 5f6d 6174 7218 0000 0029  result_matr....)
+000012c0: 0b72 1b00 0000 7224 0000 0072 2d00 0000  .r....r$...r-...
+000012d0: 722e 0000 0072 2200 0000 721c 0000 0072  r....r"...r....r
+000012e0: 1d00 0000 722f 0000 0072 3000 0000 7231  ....r/...r0...r1
+000012f0: 0000 0072 3200 0000 721e 0000 00da 0966  ...r2...r......f
+00001300: 6173 3273 7765 6570 1000 0000 738e 0000  as2sweep....s...
+00001310: 0008 1804 0108 0106 0208 020e 0108 0206  ................
+00001320: 0108 0104 0110 0214 011e 0304 0108 010c  ................
+00001330: 0308 0120 0308 010a 030a 0104 0204 0208  ... ............
+00001340: 0112 0112 0308 0104 0308 0110 010c 0108  ................
+00001350: 0108 0102 fe0e 0518 0106 0208 0108 0104  ................
+00001360: 0108 0214 030e 0108 010c 0110 0110 0110  ................
+00001370: 020a 0102 0106 0602 fa08 070a 010a 010a  ................
+00001380: 0206 010a 0104 0110 0318 020a 0b16 030c  ................
+00001390: 0104 010c fe06 050a 0104 040c fe04 0272  ...............r
+000013a0: 5700 0000 290a 4e4e 720e 0000 0046 720f  W...).NNr....Fr.
+000013b0: 0000 0054 7210 0000 0046 4e72 0100 0000  ...Tr....FNr....
+000013c0: 2917 5a0d 7377 6565 705f 7375 7070 6f72  ).Z.sweep_suppor
+000013d0: 7472 0200 0000 7203 0000 0072 0400 0000  tr....r....r....
+000013e0: da00 7205 0000 0072 0600 0000 5a14 6465  ..r....r....Z.de
+000013f0: 6661 756c 745f 7072 6f6a 5f6d 6174 5f6f  fault_proj_mat_o
+00001400: 7065 7207 0000 0072 4300 0000 724c 0000  per....rC...rL..
+00001410: 0072 4600 0000 da05 6e75 6d70 7972 2700  .rF.....numpyr'.
+00001420: 0000 7251 0000 005a 0c73 6369 7079 2e73  ..rQ...Z.scipy.s
+00001430: 7061 7273 6572 0900 0000 720a 0000 0072  parser....r....r
+00001440: 0b00 0000 5a06 6a6f 626c 6962 720c 0000  ....Z.joblibr...
+00001450: 0072 0d00 0000 7257 0000 0072 1800 0000  .r....rW...r....
+00001460: 7218 0000 0072 1800 0000 721e 0000 00da  r....r....r.....
+00001470: 083c 6d6f 6475 6c65 3e01 0000 0073 2000  .<module>....s .
+00001480: 0000 1403 1001 0c01 0801 0801 0801 0801  ................
+00001490: 0801 1001 0c01 1001 0202 0201 0201 0201  ................
+000014a0: 0efd                                     ..
```

## sweep/sweep_support/__init__.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sat Apr 30 08:32:10 2022 UTC, .py size: 347 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,24 +1,22 @@
-00000000: 550d 0d0a 0000 0000 0af4 6c62 5b01 0000  U.........lb[...
+00000000: 6f0d 0d0a 0000 0000 8336 9f64 2f01 0000  o........6.d/...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
+00000020: 0002 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 5400 6400 6401 6c01 5400 6400  d.l.T.d.d.l.T.d.
 00000040: 6401 6c02 5400 6400 6401 6c03 5400 6400  d.l.T.d.d.l.T.d.
 00000050: 6401 6c04 5400 6400 6401 6c05 5400 6400  d.l.T.d.d.l.T.d.
-00000060: 6401 6c06 5400 6400 6401 6c04 5400 6400  d.l.T.d.d.l.T.d.
-00000070: 6401 6c07 5400 6400 6401 6c08 5400 6400  d.l.T.d.d.l.T.d.
-00000080: 6401 6c09 5400 6400 6401 6c0a 5400 6402  d.l.T.d.d.l.T.d.
-00000090: 5300 2903 e901 0000 0029 01da 012a 4e29  S.)......)...*N)
-000000a0: 0b5a 0661 6132 696e 745a 066e 7432 696e  .Z.aa2intZ.nt2in
-000000b0: 745a 0661 6132 6964 785a 0769 6a32 696e  tZ.aa2idxZ.ij2in
-000000c0: 6473 5a0e 6765 6e65 7261 7465 5f63 6875  dsZ.generate_chu
-000000d0: 6e6b 5a08 7365 7132 6c69 7374 5a08 6d61  nkZ.seq2listZ.ma
-000000e0: 736b 3276 6563 5a0b 6d61 746c 6162 5f6c  sk2vecZ.matlab_l
-000000f0: 696b 655a 046f 7274 685a 086f 7274 6862  ikeZ.orthZ.orthb
-00000100: 6173 655a 0966 6173 7461 7265 6164 a900  aseZ.fastaread..
-00000110: 7203 0000 0072 0300 0000 fa39 6275 696c  r....r.....9buil
-00000120: 645c 6264 6973 742e 7769 6e2d 616d 6436  d\bdist.win-amd6
-00000130: 345c 6567 675c 7377 6565 705c 7377 6565  4\egg\sweep\swee
-00000140: 705f 7375 7070 6f72 745c 5f5f 696e 6974  p_support\__init
-00000150: 5f5f 2e70 79da 083c 6d6f 6475 6c65 3e03  __.py..<module>.
-00000160: 0000 0073 1600 0000 0801 0801 0801 0801  ...s............
-00000170: 0801 0801 0801 0801 0801 0801 0801       ..............
+00000060: 6401 6c06 5400 6400 6401 6c07 5400 6400  d.l.T.d.d.l.T.d.
+00000070: 6401 6c04 5400 6400 6401 6c08 5400 6402  d.l.T.d.d.l.T.d.
+00000080: 5300 2903 e901 0000 0029 01da 012a 4e29  S.)......)...*N)
+00000090: 095a 0661 6132 696e 745a 066e 7432 696e  .Z.aa2intZ.nt2in
+000000a0: 745a 0661 6132 6964 785a 0769 6a32 696e  tZ.aa2idxZ.ij2in
+000000b0: 6473 5a0e 6765 6e65 7261 7465 5f63 6875  dsZ.generate_chu
+000000c0: 6e6b 5a08 7365 7132 6c69 7374 5a0c 6d61  nkZ.seq2listZ.ma
+000000d0: 736b 3276 6563 5f62 696e 5a0e 6d61 736b  sk2vec_binZ.mask
+000000e0: 3276 6563 5f63 6f75 6e74 5a04 6f72 7468  2vec_countZ.orth
+000000f0: a900 7203 0000 0072 0300 0000 fa39 6275  ..r....r.....9bu
+00000100: 696c 645c 6264 6973 742e 7769 6e2d 616d  ild\bdist.win-am
+00000110: 6436 345c 6567 675c 7377 6565 705c 7377  d64\egg\sweep\sw
+00000120: 6565 705f 7375 7070 6f72 745c 5f5f 696e  eep_support\__in
+00000130: 6974 5f5f 2e70 79da 083c 6d6f 6475 6c65  it__.py..<module
+00000140: 3e01 0000 0073 1400 0000 0802 0801 0801  >....s..........
+00000150: 0801 0801 0801 0801 0801 0801 0c01       ..............
```

## sweep/sweep_support/aa2idx.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Mar 22 02:38:19 2022 UTC, .py size: 471 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,41 +1,38 @@
-00000000: 550d 0d0a 0000 0000 9b36 3962 d701 0000  U........69b....
+00000000: 6f0d 0d0a 0000 0000 03c0 4d64 bb01 0000  o.........Md....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
+00000020: 0002 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 6d00 5a00 0100 6400 6402 6c01  d.l.m.Z...d.d.l.
-00000040: 6d01 5a01 0100 6403 6404 6c02 5a03 6400  m.Z...d.d.l.Z.d.
-00000050: 6405 6c04 6d05 5a05 6d06 5a06 0100 6406  d.l.m.Z.m.Z...d.
-00000060: 6407 8400 5a07 6404 5300 2908 e901 0000  d...Z.d.S.).....
-00000070: 0029 01da 0661 6132 696e 7429 01da 066e  .)...aa2int)...n
-00000080: 7432 696e 74e9 0000 0000 4e29 02da 0672  t2int.....N)...r
-00000090: 6570 6d61 74da 0473 697a 6563 0200 0000  epmat..sizec....
-000000a0: 0000 0000 0000 0000 0800 0000 0500 0000  ................
-000000b0: 4300 0000 7388 0000 0074 007c 0083 015c  C...s....t.|...\
-000000c0: 027d 027d 037c 0164 016b 0272 2a74 01a0  .}.}.|.d.k.r*t..
-000000d0: 0274 037c 0083 01a1 0164 0218 006a 047d  .t.|.....d...j.}
-000000e0: 046e 1c7c 0164 036b 0272 4674 01a0 0274  .n.|.d.k.rFt...t
-000000f0: 057c 0083 01a1 0164 0218 006a 047d 0474  .|.....d...j.}.t
-00000100: 0674 0774 0864 047c 0383 0283 017c 0264  .t.t.d.|.....|.d
-00000110: 0283 036a 047d 0574 067c 017c 037c 0283  ...j.}.t.|.|.|..
-00000120: 037d 0674 016a 097c 067c 0513 007c 0414  .}.t.j.|.|...|..
-00000130: 0064 0464 058d 0264 0217 007d 077c 0753  .d.d...d...}.|.S
-00000140: 0029 064e e914 0000 0072 0100 0000 e904  .).N.....r......
-00000150: 0000 0072 0400 0000 2901 5a04 6178 6973  ...r....).Z.axis
-00000160: 290a 7206 0000 00da 026e 70da 0561 7272  ).r......np..arr
-00000170: 6179 7202 0000 00da 0154 7203 0000 0072  ayr......Tr....r
-00000180: 0500 0000 da04 6c69 7374 da05 7261 6e67  ......list..rang
-00000190: 65da 0373 756d 2908 5a04 7873 6571 5a07  e..sum).Z.xseqZ.
-000001a0: 6465 6653 697a 65da 016e da01 6d5a 0376  defSize..n..mZ.v
-000001b0: 6c73 5a03 706f 74da 0174 5a04 6d72 6574  lsZ.pot..tZ.mret
-000001c0: a900 7212 0000 00fa 3762 7569 6c64 5c62  ..r.....7build\b
-000001d0: 6469 7374 2e77 696e 2d61 6d64 3634 5c65  dist.win-amd64\e
-000001e0: 6767 5c73 7765 6570 5c73 7765 6570 5f73  gg\sweep\sweep_s
-000001f0: 7570 706f 7274 5c61 6132 6964 782e 7079  upport\aa2idx.py
-00000200: da06 6161 3269 6478 0700 0000 7312 0000  ..aa2idx....s...
-00000210: 0000 010c 0108 0116 0108 0114 0118 010c  ................
-00000220: 011a 0172 1400 0000 2908 7202 0000 0072  ...r....).r....r
-00000230: 0300 0000 da05 6e75 6d70 7972 0900 0000  ......numpyr....
-00000240: 5a0b 6d61 746c 6162 5f6c 696b 6572 0500  Z.matlab_liker..
-00000250: 0000 7206 0000 0072 1400 0000 7212 0000  ..r....r....r...
-00000260: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
-00000270: da08 3c6d 6f64 756c 653e 0300 0000 7308  ..<module>....s.
-00000280: 0000 000c 010c 0108 0110 01              ...........
+00000040: 6d01 5a01 0100 6403 6404 6c02 5a03 6405  m.Z...d.d.l.Z.d.
+00000050: 6406 8400 5a04 6404 5300 2907 e901 0000  d...Z.d.S.).....
+00000060: 0029 01da 0661 6132 696e 7429 01da 066e  .)...aa2int)...n
+00000070: 7432 696e 74e9 0000 0000 4e63 0200 0000  t2int.....Nc....
+00000080: 0000 0000 0000 0000 0800 0000 0500 0000  ................
+00000090: 4300 0000 7390 0000 0074 00a0 017c 00a1  C...s....t...|..
+000000a0: 016a 025c 027d 027d 037c 0164 016b 0272  .j.\.}.}.|.d.k.r
+000000b0: 1774 00a0 0174 037c 0083 01a1 0164 0218  .t...t.|.....d..
+000000c0: 006a 047d 046e 0e7c 0164 036b 0272 2574  .j.}.n.|.d.k.r%t
+000000d0: 00a0 0174 057c 0083 01a1 0164 0218 006a  ...t.|.....d...j
+000000e0: 047d 0474 00a0 0674 0764 047c 0383 027c  .}.t...t.d.|...|
+000000f0: 0264 0266 02a1 026a 047d 0574 00a0 067c  .d.f...j.}.t...|
+00000100: 017c 037c 0266 02a1 027d 0674 006a 087c  .|.|.f...}.t.j.|
+00000110: 067c 0513 007c 0414 0064 0464 058d 0264  .|...|...d.d...d
+00000120: 0217 007d 077c 0753 0029 064e e914 0000  ...}.|.S.).N....
+00000130: 0072 0100 0000 e904 0000 0072 0400 0000  .r.........r....
+00000140: 2901 5a04 6178 6973 2909 da02 6e70 da05  ).Z.axis)...np..
+00000150: 6172 7261 79da 0573 6861 7065 7202 0000  array..shaper...
+00000160: 00da 0154 7203 0000 005a 0474 696c 65da  ...Tr....Z.tile.
+00000170: 0572 616e 6765 da03 7375 6d29 085a 0478  .range..sum).Z.x
+00000180: 7365 715a 0764 6566 5369 7a65 da01 6eda  seqZ.defSize..n.
+00000190: 016d 5a03 766c 735a 0370 6f74 da01 745a  .mZ.vlsZ.pot..tZ
+000001a0: 046d 7265 74a9 0072 1000 0000 fa37 6275  .mret..r.....7bu
+000001b0: 696c 645c 6264 6973 742e 7769 6e2d 616d  ild\bdist.win-am
+000001c0: 6436 345c 6567 675c 7377 6565 705c 7377  d64\egg\sweep\sw
+000001d0: 6565 705f 7375 7070 6f72 745c 6161 3269  eep_support\aa2i
+000001e0: 6478 2e70 79da 0661 6132 6964 7806 0000  dx.py..aa2idx...
+000001f0: 0073 1200 0000 1001 0801 1601 0801 1401  .s..............
+00000200: 1801 1001 1a01 0401 7212 0000 0029 0572  ........r....).r
+00000210: 0200 0000 7203 0000 00da 056e 756d 7079  ....r......numpy
+00000220: 7207 0000 0072 1200 0000 7210 0000 0072  r....r....r....r
+00000230: 1000 0000 7210 0000 0072 1100 0000 da08  ....r....r......
+00000240: 3c6d 6f64 756c 653e 0100 0000 7308 0000  <module>....s...
+00000250: 000c 020c 0108 010c 01                   .........
```

## sweep/sweep_support/aa2int.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Mar 22 02:38:19 2022 UTC, .py size: 821 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,45 +1,51 @@
-00000000: 550d 0d0a 0000 0000 9b36 3962 3503 0000  U........69b5...
+00000000: 6f0d 0d0a 0000 0000 8db5 4d64 3903 0000  o.........Md9...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 1c00 0000 6400  .....@...s....d.
-00000030: 6401 6c00 5a01 6400 6401 6c02 5a03 6402  d.l.Z.d.d.l.Z.d.
-00000040: 6403 8400 5a04 6401 5300 2904 e900 0000  d...Z.d.S.).....
-00000050: 004e 6301 0000 0000 0000 0000 0000 0002  .Nc.............
-00000060: 0000 001e 0000 0043 0000 0073 6000 0000  .......C...s`...
-00000070: 7400 a001 7402 6a03 a004 7c00 a101 a101  t...t.j...|.....
-00000080: 7d00 6401 6402 6403 6404 6405 6406 6407  }.d.d.d.d.d.d.d.
-00000090: 6408 6409 640a 640b 640c 640d 640e 640a  d.d.d.d.d.d.d.d.
-000000a0: 640f 6410 6411 6412 6413 640a 6414 6415  d.d.d.d.d.d.d.d.
-000000b0: 6416 6417 6418 6419 641a 640a 641b 9c1d  d.d.d.d.d.d.d...
-000000c0: 7d01 7c00 a005 7c01 a101 7d00 7c00 5300  }.|...|...}.|.S.
-000000d0: 291c 4ee9 0100 0000 e915 0000 00e9 0500  ).N.............
-000000e0: 0000 e904 0000 00e9 0700 0000 e90e 0000  ................
-000000f0: 00e9 0800 0000 e909 0000 00e9 0a00 0000  ................
-00000100: 7201 0000 00e9 0c00 0000 e90b 0000 00e9  r...............
-00000110: 0d00 0000 e903 0000 00e9 0f00 0000 e906  ................
-00000120: 0000 00e9 0200 0000 e910 0000 00e9 1100  ................
-00000130: 0000 e914 0000 00e9 1200 0000 e917 0000  ................
-00000140: 00e9 1300 0000 e916 0000 00e9 1800 0000  ................
-00000150: e919 0000 0029 1dda 0161 da01 62da 0163  .....)...a..b..c
-00000160: da01 64da 0165 da01 66da 0167 da01 68da  ..d..e..f..g..h.
-00000170: 0169 da01 6ada 016b da01 6cda 016d da01  .i..j..k..l..m..
-00000180: 6eda 016f da01 70da 0171 da01 72da 0173  n..o..p..q..r..s
-00000190: da01 74da 0175 da01 76da 0177 da01 78da  ..t..u..v..w..x.
-000001a0: 0179 da01 7ada 012a fa01 2dfa 013f 2906  .y..z..*..-..?).
-000001b0: da02 7064 5a09 4461 7461 4672 616d 65da  ..pdZ.DataFrame.
-000001c0: 026e 70da 0463 6861 72da 056c 6f77 6572  .np..char..lower
-000001d0: da07 7265 706c 6163 6529 025a 0761 615f  ..replace).Z.aa_
-000001e0: 6c69 7374 da03 6d61 70a9 0072 3e00 0000  list..map..r>...
-000001f0: fa37 6275 696c 645c 6264 6973 742e 7769  .7build\bdist.wi
-00000200: 6e2d 616d 6436 345c 6567 675c 7377 6565  n-amd64\egg\swee
-00000210: 705c 7377 6565 705f 7375 7070 6f72 745c  p\sweep_support\
-00000220: 6161 3269 6e74 2e70 79da 0661 6132 696e  aa2int.py..aa2in
-00000230: 7405 0000 0073 4200 0000 0001 1201 0201  t....sB.........
-00000240: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00000250: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00000260: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00000270: 0201 0201 0201 02e4 061e 0a01 7240 0000  ............r@..
-00000280: 0029 05da 056e 756d 7079 7239 0000 005a  .)...numpyr9...Z
-00000290: 0670 616e 6461 7372 3800 0000 7240 0000  .pandasr8...r@..
-000002a0: 0072 3e00 0000 723e 0000 0072 3e00 0000  .r>...r>...r>...
-000002b0: 723f 0000 00da 083c 6d6f 6475 6c65 3e03  r?.....<module>.
-000002c0: 0000 0073 0400 0000 0801 0801            ...s........
+00000020: 0002 0000 0040 0000 0073 1400 0000 6400  .....@...s....d.
+00000030: 6401 6c00 5a01 6402 6403 8400 5a02 6401  d.l.Z.d.d...Z.d.
+00000040: 5300 2904 e900 0000 004e 6301 0000 0000  S.)......Nc.....
+00000050: 0000 0000 0000 0003 0000 000e 0000 0043  ...............C
+00000060: 0000 0073 ac00 0000 6900 6401 6402 9301  ...s....i.d.d...
+00000070: 6403 6404 9301 6405 6406 9301 6407 6408  d.d...d.d...d.d.
+00000080: 9301 6409 640a 9301 640b 640c 9301 640d  ..d.d...d.d...d.
+00000090: 640e 9301 640f 6410 9301 6411 6412 9301  d...d.d...d.d...
+000000a0: 6413 6414 9301 6415 6416 9301 6417 6418  d.d...d.d...d.d.
+000000b0: 9301 6419 641a 9301 641b 641c 9301 641d  ..d.d...d.d...d.
+000000c0: 6414 9301 641e 641f 9301 6420 6421 9301  d...d.d...d d!..
+000000d0: 6422 6423 6424 6414 6425 6426 6427 6428  d"d#d$d.d%d&d'd(
+000000e0: 6429 642a 642b 6414 642c 9c0c a501 7d01  d)d*d+d.d,....}.
+000000f0: 7400 6a01 a002 7c00 a101 7d00 7400 a003  t.j...|...}.t...
+00000100: 7c01 6a04 a101 7d02 7c02 7c00 8301 7d00  |.j...}.|.|...}.
+00000110: 7c00 5300 292d 4eda 0161 e901 0000 00da  |.S.)-N..a......
+00000120: 0162 e915 0000 00da 0163 e905 0000 00da  .b.......c......
+00000130: 0164 e904 0000 00da 0165 e907 0000 00da  .d.......e......
+00000140: 0166 e90e 0000 00da 0167 e908 0000 00da  .f.......g......
+00000150: 0168 e909 0000 00da 0169 e90a 0000 00da  .h.......i......
+00000160: 016a 7201 0000 00da 016b e90c 0000 00da  .jr......k......
+00000170: 016c e90b 0000 00da 016d e90d 0000 00da  .l.......m......
+00000180: 016e e903 0000 00da 016f da01 70e9 0f00  .n.......o..p...
+00000190: 0000 da01 71e9 0600 0000 e902 0000 00e9  ....q...........
+000001a0: 1000 0000 e911 0000 00e9 1400 0000 e912  ................
+000001b0: 0000 00e9 1700 0000 e913 0000 00e9 1600  ................
+000001c0: 0000 e918 0000 00e9 1900 0000 290c da01  ............)...
+000001d0: 72da 0173 da01 74da 0175 da01 76da 0177  r..s..t..u..v..w
+000001e0: da01 78da 0179 da01 7ada 012a fa01 2dfa  ..x..y..z..*..-.
+000001f0: 013f 2905 da02 6e70 da04 6368 6172 da05  .?)...np..char..
+00000200: 6c6f 7765 725a 0976 6563 746f 7269 7a65  lowerZ.vectorize
+00000210: da03 6765 7429 035a 0761 615f 6c69 7374  ..get).Z.aa_list
+00000220: da03 6d61 705a 086d 6170 5f66 756e 63a9  ..mapZ.map_func.
+00000230: 0072 3d00 0000 fa37 6275 696c 645c 6264  .r=....7build\bd
+00000240: 6973 742e 7769 6e2d 616d 6436 345c 6567  ist.win-amd64\eg
+00000250: 675c 7377 6565 705c 7377 6565 705f 7375  g\sweep\sweep_su
+00000260: 7070 6f72 745c 6161 3269 6e74 2e70 79da  pport\aa2int.py.
+00000270: 0661 6132 696e 7404 0000 0073 6400 0000  .aa2int....sd...
+00000280: 0801 0401 02ff 0402 02fe 0403 02fd 0404  ................
+00000290: 02fc 0405 02fb 0406 02fa 0407 02f9 0408  ................
+000002a0: 02f8 0409 02f7 040a 02f6 040b 02f5 040c  ................
+000002b0: 02f4 040d 02f3 040e 02f2 040f 02f1 0410  ................
+000002c0: 02f0 0211 0201 0201 0201 0201 0201 0201  ................
+000002d0: 0201 0201 0201 0201 0201 08e4 0c1e 0c01  ................
+000002e0: 0801 0401 723f 0000 0029 03da 056e 756d  ....r?...)...num
+000002f0: 7079 7238 0000 0072 3f00 0000 723d 0000  pyr8...r?...r=..
+00000300: 0072 3d00 0000 723d 0000 0072 3e00 0000  .r=...r=...r>...
+00000310: da08 3c6d 6f64 756c 653e 0100 0000 7304  ..<module>....s.
+00000320: 0000 0008 020c 01                        .......
```

## sweep/sweep_support/generate_chunk.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Mar 22 02:38:19 2022 UTC, .py size: 386 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,38 +1,37 @@
-00000000: 550d 0d0a 0000 0000 9b36 3962 8201 0000  U........69b....
+00000000: 6f0d 0d0a 0000 0000 10bd 4d64 b601 0000  o.........Md....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
-00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
-00000040: 6d04 5a04 0100 6402 6403 6c05 5a06 6404  m.Z...d.d.l.Z.d.
-00000050: 6405 8400 5a07 6403 5300 2906 e901 0000  d...Z.d.S.).....
-00000060: 0029 04da 0566 6c6f 6f72 da06 7265 706d  .)...floor..repm
-00000070: 6174 da05 7a65 726f 73da 046f 6e65 73e9  at..zeros..ones.
-00000080: 0000 0000 4e63 0200 0000 0000 0000 0000  ....Nc..........
-00000090: 0000 0400 0000 0900 0000 4300 0000 736a  ..........C...sj
-000000a0: 0000 0074 007c 017c 001b 0083 017d 0274  ...t.|.|.....}.t
-000000b0: 017c 027c 0064 0183 0374 02a0 0374 0474  .|.|.d...t...t.t
-000000c0: 0564 027c 0083 0283 0174 0474 0564 037c  .d.|.....t.t.d.|
-000000d0: 0064 0317 0083 0283 0167 02a1 016a 0614  .d.......g...j..
-000000e0: 0074 026a 0774 087c 0064 0383 0274 097c  .t.j.t.|.d...t.|
-000000f0: 0064 0383 0266 0264 0364 048d 0217 007d  .d...f.d.d.....}
-00000100: 037c 017c 0364 053c 007c 0353 0029 064e  .|.|.d.<.|.S.).N
-00000110: e902 0000 0072 0600 0000 7201 0000 0029  .....r....r....)
-00000120: 015a 0461 7869 7329 02e9 ffff ffff 7201  .Z.axis)......r.
-00000130: 0000 0029 0a72 0200 0000 7203 0000 00da  ...).r....r.....
-00000140: 026e 70da 0561 7272 6179 da04 6c69 7374  .np..array..list
-00000150: da05 7261 6e67 65da 0154 5a0b 636f 6e63  ..range..TZ.conc
-00000160: 6174 656e 6174 6572 0500 0000 7204 0000  atenater....r...
-00000170: 0029 04da 0663 6875 6e6b 735a 0866 696c  .)...chunksZ.fil
-00000180: 655f 6c65 6eda 017a 5a06 6964 784d 6174  e_len..zZ.idxMat
-00000190: a900 7210 0000 00fa 3f62 7569 6c64 5c62  ..r.....?build\b
-000001a0: 6469 7374 2e77 696e 2d61 6d64 3634 5c65  dist.win-amd64\e
-000001b0: 6767 5c73 7765 6570 5c73 7765 6570 5f73  gg\sweep\sweep_s
-000001c0: 7570 706f 7274 5c67 656e 6572 6174 655f  upport\generate_
-000001d0: 6368 756e 6b2e 7079 da0e 6765 6e65 7261  chunk.py..genera
-000001e0: 7465 5f63 6875 6e6b 0500 0000 7308 0000  te_chunk....s...
-000001f0: 0000 010c 0152 0108 0172 1200 0000 2908  .....R...r....).
-00000200: 5a0b 6d61 746c 6162 5f6c 696b 6572 0200  Z.matlab_liker..
-00000210: 0000 7203 0000 0072 0400 0000 7205 0000  ..r....r....r...
-00000220: 00da 056e 756d 7079 7209 0000 0072 1200  ...numpyr....r..
-00000230: 0000 7210 0000 0072 1000 0000 7210 0000  ..r....r....r...
-00000240: 0072 1100 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00000250: 0300 0000 7304 0000 0018 0108 01         ....s........
+00000020: 0002 0000 0040 0000 0073 1c00 0000 6400  .....@...s....d.
+00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6402  d.l.Z.d.d.l.Z.d.
+00000040: 6403 8400 5a03 6401 5300 2904 e900 0000  d...Z.d.S.).....
+00000050: 004e 6302 0000 0000 0000 0000 0000 0004  .Nc.............
+00000060: 0000 0009 0000 0043 0000 0073 7800 0000  .......C...sx...
+00000070: 7400 a001 7c01 7c00 1b00 a101 7d02 7402  t...|.|.....}.t.
+00000080: a003 7c02 7c00 6401 6602 a102 7402 a004  ..|.|.d.f...t...
+00000090: 7405 7406 6402 7c00 8302 8301 7405 7406  t.t.d.|.....t.t.
+000000a0: 6403 7c00 6403 1700 8302 8301 6702 a101  d.|.d.......g...
+000000b0: 6a07 1400 7402 6a08 7402 a009 7c00 6403  j...t.j.t...|.d.
+000000c0: 6602 a101 7402 a00a 7c00 6403 6602 a101  f...t...|.d.f...
+000000d0: 6602 6403 6404 8d02 1700 7d03 7c01 7c03  f.d.d.....}.|.|.
+000000e0: 6405 3c00 7c03 5300 2906 4ee9 0200 0000  d.<.|.S.).N.....
+000000f0: 7201 0000 00e9 0100 0000 2901 5a04 6178  r.........).Z.ax
+00000100: 6973 2902 e9ff ffff ff72 0300 0000 290b  is)......r....).
+00000110: da04 6d61 7468 da05 666c 6f6f 72da 026e  ..math..floor..n
+00000120: 705a 0474 696c 65da 0561 7272 6179 da04  pZ.tile..array..
+00000130: 6c69 7374 da05 7261 6e67 65da 0154 5a0b  list..range..TZ.
+00000140: 636f 6e63 6174 656e 6174 655a 046f 6e65  concatenateZ.one
+00000150: 735a 057a 6572 6f73 2904 da06 6368 756e  sZ.zeros)...chun
+00000160: 6b73 5a08 6669 6c65 5f6c 656e da0a 6368  ksZ.file_len..ch
+00000170: 756e 6b5f 7369 7a65 5a0d 6368 756e 6b5f  unk_sizeZ.chunk_
+00000180: 696e 6469 6365 73a9 0072 0e00 0000 fa3f  indices..r.....?
+00000190: 6275 696c 645c 6264 6973 742e 7769 6e2d  build\bdist.win-
+000001a0: 616d 6436 345c 6567 675c 7377 6565 705c  amd64\egg\sweep\
+000001b0: 7377 6565 705f 7375 7070 6f72 745c 6765  sweep_support\ge
+000001c0: 6e65 7261 7465 5f63 6875 6e6b 2e70 79da  nerate_chunk.py.
+000001d0: 0e67 656e 6572 6174 655f 6368 756e 6b05  .generate_chunk.
+000001e0: 0000 0073 1000 0000 0e01 0e01 2601 02ff  ...s........&...
+000001f0: 2402 04fe 0803 0401 7210 0000 0029 0472  $.......r....).r
+00000200: 0500 0000 da05 6e75 6d70 7972 0700 0000  ......numpyr....
+00000210: 7210 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
+00000220: 0e00 0000 720f 0000 00da 083c 6d6f 6475  ....r......<modu
+00000230: 6c65 3e01 0000 0073 0600 0000 0802 0801  le>....s........
+00000240: 0c01                                     ..
```

## sweep/sweep_support/ij2inds.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Mar 22 02:38:19 2022 UTC, .py size: 118 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,19 +1,19 @@
-00000000: 550d 0d0a 0000 0000 9b36 3962 7600 0000  U........69bv...
+00000000: 6f0d 0d0a 0000 0000 9b36 3962 7600 0000  o........69bv...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 0c00 0000 6400  .....@...s....d.
 00000030: 6401 8400 5a00 6402 5300 2903 6302 0000  d...Z.d.S.).c...
 00000040: 0000 0000 0000 0000 0002 0000 0004 0000  ................
 00000050: 0043 0000 0073 2800 0000 7c00 6400 6400  .C...s(...|.d.d.
 00000060: 8502 6401 6602 1900 6401 1800 7c01 1400  ..d.f...d...|...
 00000070: 7c00 6400 6400 8502 6402 6602 1900 1700  |.d.d...d.f.....
 00000080: 5300 2903 4ee9 0100 0000 e900 0000 00a9  S.).N...........
 00000090: 0029 025a 0369 6a73 5a05 746d 636f 6c72  .).Z.ijsZ.tmcolr
 000000a0: 0300 0000 7203 0000 00fa 3862 7569 6c64  ....r.....8build
 000000b0: 5c62 6469 7374 2e77 696e 2d61 6d64 3634  \bdist.win-amd64
 000000c0: 5c65 6767 5c73 7765 6570 5c73 7765 6570  \egg\sweep\sweep
 000000d0: 5f73 7570 706f 7274 5c69 6a32 696e 6473  _support\ij2inds
 000000e0: 2e70 79da 0769 6a32 696e 6473 0300 0000  .py..ij2inds....
-000000f0: 7302 0000 0000 0172 0500 0000 4e29 0172  s......r....N).r
+000000f0: 7302 0000 0028 0172 0500 0000 4e29 0172  s....(.r....N).r
 00000100: 0500 0000 7203 0000 0072 0300 0000 7203  ....r....r....r.
 00000110: 0000 0072 0400 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000120: 653e 0300 0000 f300 0000 00              e>.........
+00000120: 653e 0100 0000 7302 0000 000c 02         e>....s......
```

## sweep/sweep_support/nt2int.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Mar 22 02:38:19 2022 UTC, .py size: 813 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,42 +1,48 @@
-00000000: 550d 0d0a 0000 0000 9b36 3962 2d03 0000  U........69b-...
+00000000: 6f0d 0d0a 0000 0000 c9b7 4d64 3103 0000  o.........Md1...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 1c00 0000 6400  .....@...s....d.
-00000030: 6401 6c00 5a01 6400 6401 6c02 5a03 6402  d.l.Z.d.d.l.Z.d.
-00000040: 6403 8400 5a04 6401 5300 2904 e900 0000  d...Z.d.S.).....
-00000050: 004e 6301 0000 0000 0000 0000 0000 0002  .Nc.............
-00000060: 0000 001e 0000 0043 0000 0073 6000 0000  .......C...s`...
-00000070: 7400 a001 7402 6a03 a004 7c00 a101 a101  t...t.j...|.....
-00000080: 7d00 6401 6402 6403 6404 6405 6405 6406  }.d.d.d.d.d.d.d.
-00000090: 6407 6405 6405 6408 6405 6409 640a 6405  d.d.d.d.d.d.d.d.
-000000a0: 6405 6405 640b 640c 640d 640d 640e 640f  d.d.d.d.d.d.d.d.
-000000b0: 640a 6410 6405 6405 6411 6405 6412 9c1d  d.d.d.d.d.d.d...
-000000c0: 7d01 7c00 a005 7c01 a101 7d00 7c00 5300  }.|...|...}.|.S.
-000000d0: 2913 4ee9 0100 0000 e90b 0000 00e9 0200  ).N.............
-000000e0: 0000 e90c 0000 0072 0100 0000 e903 0000  .......r........
-000000f0: 00e9 0d00 0000 e907 0000 00e9 0800 0000  ................
-00000100: e90f 0000 00e9 0500 0000 e909 0000 00e9  ................
-00000110: 0400 0000 e90e 0000 00e9 0a00 0000 e906  ................
-00000120: 0000 00e9 1000 0000 291d da01 61da 0162  ........)...a..b
-00000130: da01 63da 0164 da01 65da 0166 da01 67da  ..c..d..e..f..g.
-00000140: 0168 da01 69da 016a da01 6bda 016c da01  .h..i..j..k..l..
-00000150: 6dda 016e da01 6fda 0170 da01 71da 0172  m..n..o..p..q..r
-00000160: da01 73da 0174 da01 75da 0176 da01 77da  ..s..t..u..v..w.
-00000170: 0178 da01 79da 017a da01 2afa 012d fa01  .x..y..z..*..-..
-00000180: 3f29 06da 0270 645a 0944 6174 6146 7261  ?)...pdZ.DataFra
-00000190: 6d65 da02 6e70 da04 6368 6172 da05 6c6f  me..np..char..lo
-000001a0: 7765 72da 0772 6570 6c61 6365 2902 5a07  wer..replace).Z.
-000001b0: 6e74 5f6c 6973 74da 036d 6170 a900 7235  nt_list..map..r5
-000001c0: 0000 00fa 3762 7569 6c64 5c62 6469 7374  ....7build\bdist
-000001d0: 2e77 696e 2d61 6d64 3634 5c65 6767 5c73  .win-amd64\egg\s
-000001e0: 7765 6570 5c73 7765 6570 5f73 7570 706f  weep\sweep_suppo
-000001f0: 7274 5c6e 7432 696e 742e 7079 da06 6e74  rt\nt2int.py..nt
-00000200: 3269 6e74 0500 0000 7342 0000 0000 0112  2int....sB......
-00000210: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00000220: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00000230: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00000240: 0102 0102 0102 0102 0102 e406 1e0a 0172  ...............r
-00000250: 3700 0000 2905 da05 6e75 6d70 7972 3000  7...)...numpyr0.
-00000260: 0000 5a06 7061 6e64 6173 722f 0000 0072  ..Z.pandasr/...r
-00000270: 3700 0000 7235 0000 0072 3500 0000 7235  7...r5...r5...r5
-00000280: 0000 0072 3600 0000 da08 3c6d 6f64 756c  ...r6.....<modul
-00000290: 653e 0300 0000 7304 0000 0008 0108 01    e>....s........
+00000020: 0002 0000 0040 0000 0073 1400 0000 6400  .....@...s....d.
+00000030: 6401 6c00 5a01 6402 6403 8400 5a02 6401  d.l.Z.d.d...Z.d.
+00000040: 5300 2904 e900 0000 004e 6301 0000 0000  S.)......Nc.....
+00000050: 0000 0000 0000 0003 0000 000e 0000 0043  ...............C
+00000060: 0000 0073 ac00 0000 6900 6401 6402 9301  ...s....i.d.d...
+00000070: 6403 6404 9301 6405 6406 9301 6407 6408  d.d...d.d...d.d.
+00000080: 9301 6409 640a 9301 640b 640a 9301 640c  ..d.d...d.d...d.
+00000090: 640d 9301 640e 640f 9301 6410 640a 9301  d...d.d...d.d...
+000000a0: 6411 640a 9301 6412 6413 9301 6414 640a  d.d...d.d...d.d.
+000000b0: 9301 6415 6416 9301 6417 6418 9301 6419  ..d.d...d.d...d.
+000000c0: 640a 9301 641a 640a 9301 641b 640a 9301  d...d.d...d.d...
+000000d0: 641c 641d 641e 641e 641f 6420 6418 6421  d.d.d.d.d.d d.d!
+000000e0: 640a 640a 6422 640a 6423 9c0c a501 7d01  d.d.d"d.d#....}.
+000000f0: 7400 6a01 a002 7c00 a101 7d00 7400 a003  t.j...|...}.t...
+00000100: 7c01 6a04 a101 7d02 7c02 7c00 8301 7d00  |.j...}.|.|...}.
+00000110: 7c00 5300 2924 4eda 0161 e901 0000 00da  |.S.)$N..a......
+00000120: 0162 e90b 0000 00da 0163 e902 0000 00da  .b.......c......
+00000130: 0164 e90c 0000 00da 0165 7201 0000 00da  .d.......er.....
+00000140: 0166 da01 67e9 0300 0000 da01 68e9 0d00  .f..g.......h...
+00000150: 0000 da01 69da 016a da01 6be9 0700 0000  ....i..j..k.....
+00000160: da01 6cda 016d e908 0000 00da 016e e90f  ..l..m.......n..
+00000170: 0000 00da 016f da01 70da 0171 e905 0000  .....o..p..q....
+00000180: 00e9 0900 0000 e904 0000 00e9 0e00 0000  ................
+00000190: e90a 0000 00e9 0600 0000 e910 0000 0029  ...............)
+000001a0: 0cda 0172 da01 73da 0174 da01 75da 0176  ...r..s..t..u..v
+000001b0: da01 77da 0178 da01 79da 017a da01 2afa  ..w..x..y..z..*.
+000001c0: 012d fa01 3f29 05da 026e 70da 0463 6861  .-..?)...np..cha
+000001d0: 72da 056c 6f77 6572 5a09 7665 6374 6f72  r..lowerZ.vector
+000001e0: 697a 65da 0367 6574 2903 5a07 6e74 5f6c  ize..get).Z.nt_l
+000001f0: 6973 74da 036d 6170 5a08 6d61 705f 6675  ist..mapZ.map_fu
+00000200: 6e63 a900 7234 0000 00fa 3762 7569 6c64  nc..r4....7build
+00000210: 5c62 6469 7374 2e77 696e 2d61 6d64 3634  \bdist.win-amd64
+00000220: 5c65 6767 5c73 7765 6570 5c73 7765 6570  \egg\sweep\sweep
+00000230: 5f73 7570 706f 7274 5c6e 7432 696e 742e  _support\nt2int.
+00000240: 7079 da06 6e74 3269 6e74 0400 0000 7364  py..nt2int....sd
+00000250: 0000 0008 0104 0102 ff04 0202 fe04 0302  ................
+00000260: fd04 0402 fc04 0502 fb04 0602 fa04 0702  ................
+00000270: f904 0802 f804 0902 f704 0a02 f604 0b02  ................
+00000280: f504 0c02 f404 0d02 f304 0e02 f204 0f02  ................
+00000290: f104 1002 f002 1102 0102 0102 0102 0102  ................
+000002a0: 0102 0102 0102 0102 0102 0102 0108 e40c  ................
+000002b0: 1e0c 0108 0104 0172 3600 0000 2903 da05  .......r6...)...
+000002c0: 6e75 6d70 7972 2f00 0000 7236 0000 0072  numpyr/...r6...r
+000002d0: 3400 0000 7234 0000 0072 3400 0000 7235  4...r4...r4...r5
+000002e0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+000002f0: 0073 0400 0000 0802 0c01                 .s........
```

## sweep/sweep_support/orth.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Mar 22 02:38:19 2022 UTC, .py size: 252 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,31 +1,29 @@
-00000000: 550d 0d0a 0000 0000 9b36 3962 fc00 0000  U........69b....
+00000000: 6f0d 0d0a 0000 0000 17c8 4f64 f200 0000  o.........Od....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
-00000030: 6401 6c00 5a01 6402 6403 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
-00000040: 6d04 5a04 6d05 5a05 6d06 5a06 0100 6404  m.Z.m.Z.m.Z...d.
-00000050: 6405 8400 5a07 6401 5300 2906 e900 0000  d...Z.d.S.).....
-00000060: 004e e901 0000 0029 04da 0373 7664 da04  .N.....)...svd..
-00000070: 6469 6167 da03 6570 73da 0473 697a 6563  diag..eps..sizec
-00000080: 0100 0000 0000 0000 0000 0000 0500 0000  ................
-00000090: 0400 0000 4300 0000 7354 0000 0074 007c  ....C...sT...t.|
-000000a0: 0083 015c 027d 017d 0274 017c 0283 017d  ...\.}.}.t.|...}
-000000b0: 0274 0274 037c 0083 0183 017c 0264 0119  .t.t.|.....|.d..
-000000c0: 0014 0074 0464 0283 0114 007d 0374 057c  ...t.d.....}.t.|
-000000d0: 027c 036b 0483 017d 047c 0164 0064 0085  .|.k...}.|.d.d..
-000000e0: 0264 017c 0485 0266 0219 007d 017c 0153  .d.|...f...}.|.S
-000000f0: 0029 034e 7201 0000 005a 0664 6f75 626c  .).Nr....Z.doubl
-00000100: 6529 0672 0300 0000 7204 0000 00da 036d  e).r....r......m
-00000110: 6178 7206 0000 0072 0500 0000 da03 7375  axr....r......su
-00000120: 6d29 05da 0141 da01 51da 0153 5a03 746f  m)...A..Q..SZ.to
-00000130: 6cda 0172 a900 720d 0000 00fa 3562 7569  l..r..r.....5bui
-00000140: 6c64 5c62 6469 7374 2e77 696e 2d61 6d64  ld\bdist.win-amd
-00000150: 3634 5c65 6767 5c73 7765 6570 5c73 7765  64\egg\sweep\swe
-00000160: 6570 5f73 7570 706f 7274 5c6f 7274 682e  ep_support\orth.
-00000170: 7079 da04 6f72 7468 0500 0000 730c 0000  py..orth....s...
-00000180: 0000 010c 0108 011c 010c 0114 0172 0f00  .............r..
-00000190: 0000 2908 da05 6e75 6d70 79da 026e 705a  ..)...numpy..npZ
-000001a0: 0b6d 6174 6c61 625f 6c69 6b65 7203 0000  .matlab_liker...
-000001b0: 0072 0400 0000 7205 0000 0072 0600 0000  .r....r....r....
-000001c0: 720f 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
-000001d0: 0d00 0000 720e 0000 00da 083c 6d6f 6475  ....r......<modu
-000001e0: 6c65 3e03 0000 0073 0400 0000 0801 1801  le>....s........
+00000020: 0002 0000 0040 0000 0073 1400 0000 6400  .....@...s....d.
+00000030: 6401 6c00 5a01 6402 6403 8400 5a02 6401  d.l.Z.d.d...Z.d.
+00000040: 5300 2904 e900 0000 004e 6301 0000 0000  S.)......Nc.....
+00000050: 0000 0000 0000 0006 0000 0004 0000 0043  ...............C
+00000060: 0000 0073 5800 0000 7400 6a01 6a02 7c00  ...sX...t.j.j.|.
+00000070: 6401 6402 8d02 5c03 7d01 7d02 7d03 7403  d.d...\.}.}.}.t.
+00000080: 7c00 6a04 8301 7c02 6403 1900 1400 7400  |.j...|.d.....t.
+00000090: a005 6404 a101 6a06 1400 7d04 7407 7c02  ..d...j...}.t.|.
+000000a0: 7c04 6b04 8301 7d05 7c01 6400 6400 8502  |.k...}.|.d.d...
+000000b0: 6403 7c05 8502 6602 1900 7d01 7c01 5300  d.|...f...}.|.S.
+000000c0: 2905 4e46 2901 5a0d 6675 6c6c 5f6d 6174  ).NF).Z.full_mat
+000000d0: 7269 6365 7372 0100 0000 5a06 646f 7562  ricesr....Z.doub
+000000e0: 6c65 2908 da02 6e70 5a06 6c69 6e61 6c67  le)...npZ.linalg
+000000f0: 5a03 7376 64da 036d 6178 da05 7368 6170  Z.svd..max..shap
+00000100: 655a 0566 696e 666f da03 6570 73da 0373  eZ.finfo..eps..s
+00000110: 756d 2906 da01 41da 0151 da01 535a 0256  um)...A..Q..SZ.V
+00000120: 745a 0374 6f6c da01 72a9 0072 0b00 0000  tZ.tol..r..r....
+00000130: fa35 6275 696c 645c 6264 6973 742e 7769  .5build\bdist.wi
+00000140: 6e2d 616d 6436 345c 6567 675c 7377 6565  n-amd64\egg\swee
+00000150: 705c 7377 6565 705f 7375 7070 6f72 745c  p\sweep_support\
+00000160: 6f72 7468 2e70 79da 046f 7274 6805 0000  orth.py..orth...
+00000170: 0073 0a00 0000 1601 1e01 0c01 1401 0401  .s..............
+00000180: 720d 0000 0029 03da 056e 756d 7079 7202  r....)...numpyr.
+00000190: 0000 0072 0d00 0000 720b 0000 0072 0b00  ...r....r....r..
+000001a0: 0000 720b 0000 0072 0c00 0000 da08 3c6d  ..r....r......<m
+000001b0: 6f64 756c 653e 0100 0000 7304 0000 0008  odule>....s.....
+000001c0: 020c 02                                  ...
```

## sweep/sweep_support/seq2list.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Mar 22 02:38:19 2022 UTC, .py size: 239 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,26 +1,31 @@
-00000000: 550d 0d0a 0000 0000 9b36 3962 ef00 0000  U........69b....
+00000000: 6f0d 0d0a 0000 0000 6fb3 4d64 3d01 0000  o.......o.Md=...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 1c00 0000 6400  .....@...s....d.
-00000030: 6401 6c00 5a01 6400 6401 6c02 5a03 6402  d.l.Z.d.d.l.Z.d.
-00000040: 6403 8400 5a04 6401 5300 2904 e900 0000  d...Z.d.S.).....
-00000050: 004e 6302 0000 0000 0000 0000 0000 0003  .Nc.............
-00000060: 0000 0007 0000 0043 0000 0073 3800 0000  .......C...s8...
-00000070: 7400 7c00 8301 7d00 7401 a002 7c00 a101  t.|...}.t...|...
-00000080: 7d02 7401 a002 7400 7403 6a04 7c02 a005  }.t...t.t.j.|...
-00000090: a100 7c01 6401 8d02 8301 a101 7d02 7401  ..|.d.......}.t.
-000000a0: a002 7c02 a101 5300 2902 4e29 01da 016e  ..|...S.).N)...n
-000000b0: 2906 da04 6c69 7374 da02 6e70 da05 6172  )...list..np..ar
-000000c0: 7261 79da 036d 6974 5a08 7769 6e64 6f77  ray..mitZ.window
-000000d0: 6564 5a05 7261 7665 6c29 035a 0473 646e  edZ.ravel).Z.sdn
-000000e0: 61da 0171 da01 62a9 0072 0900 0000 fa39  a..q..b..r.....9
-000000f0: 6275 696c 645c 6264 6973 742e 7769 6e2d  build\bdist.win-
-00000100: 616d 6436 345c 6567 675c 7377 6565 705c  amd64\egg\sweep\
-00000110: 7377 6565 705f 7375 7070 6f72 745c 7365  sweep_support\se
-00000120: 7132 6c69 7374 2e70 79da 0873 6571 326c  q2list.py..seq2l
-00000130: 6973 7405 0000 0073 0800 0000 0001 0801  ist....s........
-00000140: 0a01 1c01 720b 0000 0029 05da 056e 756d  ....r....)...num
-00000150: 7079 7204 0000 00da 0e6d 6f72 655f 6974  pyr......more_it
-00000160: 6572 746f 6f6c 7372 0600 0000 720b 0000  ertoolsr....r...
-00000170: 0072 0900 0000 7209 0000 0072 0900 0000  .r....r....r....
-00000180: 720a 0000 00da 083c 6d6f 6475 6c65 3e03  r......<module>.
-00000190: 0000 0073 0400 0000 0801 0801            ...s........
+00000020: 0002 0000 0040 0000 0073 1400 0000 6400  .....@...s....d.
+00000030: 6401 6c00 5a01 6402 6403 8400 5a02 6401  d.l.Z.d.d...Z.d.
+00000040: 5300 2904 e900 0000 004e 6302 0000 0000  S.)......Nc.....
+00000050: 0000 0000 0000 0005 0000 0005 0000 0043  ...............C
+00000060: 0000 0073 7c00 0000 7400 a001 7402 7c00  ...s|...t...t.|.
+00000070: 8301 a101 7d00 7c00 6a03 6401 1900 7d02  ....}.|.j.d...}.
+00000080: 7c02 7c01 6b00 7215 7400 a001 6700 a101  |.|.k.r.t...g...
+00000090: 5300 7400 6a04 7c02 7c01 1800 6402 1700  S.t.j.|.|...d...
+000000a0: 7c01 6602 7c00 6a05 6403 8d02 7d03 7406  |.f.|.j.d...}.t.
+000000b0: 7c01 8301 4400 5d14 7d04 7c00 7c04 7c02  |...D.].}.|.|.|.
+000000c0: 7c01 1800 7c04 1700 6402 1700 8502 1900  |...|...d.......
+000000d0: 7c03 6400 6400 8502 7c04 6602 3c00 7127  |.d.d...|.f.<.q'
+000000e0: 7c03 5300 2904 4e72 0100 0000 e901 0000  |.S.).Nr........
+000000f0: 0029 01da 0564 7479 7065 2907 da02 6e70  .)...dtype)...np
+00000100: da05 6172 7261 79da 046c 6973 74da 0573  ..array..list..s
+00000110: 6861 7065 5a05 7a65 726f 7372 0300 0000  hapeZ.zerosr....
+00000120: da05 7261 6e67 6529 055a 0473 646e 61da  ..range).Z.sdna.
+00000130: 0171 da01 6eda 0162 da01 69a9 0072 0d00  .q..n..b..i..r..
+00000140: 0000 fa39 6275 696c 645c 6264 6973 742e  ...9build\bdist.
+00000150: 7769 6e2d 616d 6436 345c 6567 675c 7377  win-amd64\egg\sw
+00000160: 6565 705c 7377 6565 705f 7375 7070 6f72  eep\sweep_suppor
+00000170: 745c 7365 7132 6c69 7374 2e70 79da 0873  t\seq2list.py..s
+00000180: 6571 326c 6973 7404 0000 0073 1000 0000  eq2list....s....
+00000190: 0e01 0a01 0801 0a01 1c01 0c01 2601 0401  ............&...
+000001a0: 720f 0000 0029 03da 056e 756d 7079 7204  r....)...numpyr.
+000001b0: 0000 0072 0f00 0000 720d 0000 0072 0d00  ...r....r....r..
+000001c0: 0000 720d 0000 0072 0e00 0000 da08 3c6d  ..r....r......<m
+000001d0: 6f64 756c 653e 0100 0000 7304 0000 0008  odule>....s.....
+000001e0: 020c 01                                  ...
```

## Comparing `sweep/sweep_support/mask2vec.pyc` & `sweep/sweep_support/mask2vec_count.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Mar 22 02:38:19 2022 UTC, .py size: 709 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-00000000: 550d 0d0a 0000 0000 9b36 3962 c502 0000  U........69b....
+00000000: 6f0d 0d0a 0000 0000 ace7 9d64 6303 0000  o..........dc...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
+00000020: 0003 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 6d00 5a00 0100 6400 6402 6c01  d.l.m.Z...d.d.l.
 00000040: 6d01 5a01 0100 6400 6403 6c02 6d02 5a02  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6404 6c03 6d04 5a04 0100 6405  ..d.d.l.m.Z...d.
-00000060: 6406 6c05 5a06 6407 6400 6407 6703 6408  d.l.Z.d.d.d.g.d.
-00000070: 6602 6409 640a 8401 5a07 6406 5300 290b  f.d.d...Z.d.S.).
-00000080: e901 0000 0029 01da 0873 6571 326c 6973  .....)...seq2lis
-00000090: 7429 01da 0661 6132 6964 7829 01da 0769  t)...aa2idx)...i
-000000a0: 6a32 696e 6473 2901 da05 7a65 726f 73e9  j2inds)...zeros.
-000000b0: 0000 0000 4ee9 0200 0000 e914 0000 0063  ....N..........c
-000000c0: 0300 0000 0000 0000 0000 0000 0b00 0000  ................
-000000d0: 0900 0000 4300 0000 73ee 0000 007c 0164  ....C...s....|.d
-000000e0: 0119 007c 0164 0219 0017 007c 0164 0319  ...|.d.....|.d..
-000000f0: 0017 007d 0374 007c 0074 017c 0383 0183  ...}.t.|.t.|....
-00000100: 027d 0474 02a0 0374 047c 0464 0064 0085  .}.t...t.|.d.d..
-00000110: 0264 017c 0164 0119 0085 0266 0219 007c  .d.|.d.....f...|
-00000120: 0283 0274 047c 0464 0064 0085 027c 037c  ...t.|.d.d...|.|
-00000130: 0164 0319 0018 007c 0385 0266 0219 007c  .d.....|...f...|
-00000140: 0283 0267 02a1 016a 057d 0574 026a 067c  ...g...j.}.t.j.|
-00000150: 0564 0164 048d 027d 057c 027c 0164 0119  .d.d...}.|.|.d..
-00000160: 0013 007d 0674 077c 057c 0683 027d 077c  ...}.t.|.|...}.|
-00000170: 027c 0164 0319 0013 007d 0874 0864 027c  .|.d.....}.t.d.|
-00000180: 067c 0814 0083 027d 097c 027c 0164 0119  .|.....}.|.|.d..
-00000190: 0013 007c 027c 0164 0319 0013 0014 007d  ...|.|.d.......}
-000001a0: 0a7c 077c 077c 0a6b 0119 007d 0764 027c  .|.|.|.k...}.d.|
-000001b0: 0964 017c 0764 0218 0066 023c 007c 09a0  .d.|.d...f.<.|..
-000001c0: 0974 01a1 017d 097c 0953 0029 054e 7206  .t...}.|.S.).Nr.
-000001d0: 0000 0072 0100 0000 7207 0000 0029 015a  ...r....r....).Z
-000001e0: 0461 7869 7329 0a72 0200 0000 da03 696e  .axis).r......in
-000001f0: 74da 026e 70da 0561 7272 6179 7203 0000  t..np..arrayr...
-00000200: 00da 0154 da06 756e 6971 7565 7204 0000  ...T..uniquer...
-00000210: 0072 0500 0000 5a06 6173 7479 7065 290b  .r....Z.astype).
-00000220: 5a04 7873 6571 da04 6d61 736b 5a07 6465  Z.xseq..maskZ.de
-00000230: 6653 697a 65da 0174 da05 736c 6963 655a  fSize..t..sliceZ
-00000240: 0278 79da 056c 696e 6573 5a04 696e 6473  .xy..linesZ.inds
-00000250: da04 636f 6c73 da01 4d5a 0972 6f77 735f  ..cols..MZ.rows_
-00000260: 7369 7a65 a900 7214 0000 00fa 3962 7569  size..r.....9bui
-00000270: 6c64 5c62 6469 7374 2e77 696e 2d61 6d64  ld\bdist.win-amd
-00000280: 3634 5c65 6767 5c73 7765 6570 5c73 7765  64\egg\sweep\swe
-00000290: 6570 5f73 7570 706f 7274 5c6d 6173 6b32  ep_support\mask2
-000002a0: 7665 632e 7079 da08 6d61 736b 3276 6563  vec.py..mask2vec
-000002b0: 0800 0000 731e 0000 0000 0118 010e 0120  ....s.......... 
-000002c0: 0120 ff08 020e 010c 010a 010c 010e 0118  . ..............
-000002d0: 010c 0110 010a 0172 1600 0000 2908 7202  .......r....).r.
-000002e0: 0000 0072 0300 0000 7204 0000 005a 0b6d  ...r....r....Z.m
-000002f0: 6174 6c61 625f 6c69 6b65 7205 0000 00da  atlab_liker.....
-00000300: 056e 756d 7079 720a 0000 0072 1600 0000  .numpyr....r....
-00000310: 7214 0000 0072 1400 0000 7214 0000 0072  r....r....r....r
-00000320: 1500 0000 da08 3c6d 6f64 756c 653e 0300  ......<module>..
-00000330: 0000 730a 0000 000c 010c 010c 010c 0108  ..s.............
-00000340: 01                                       .
+00000050: 0100 6404 6405 6c03 5a04 6700 6406 a201  ..d.d.l.Z.g.d...
+00000060: 6407 6602 6408 6409 8401 5a05 6405 5300  d.f.d.d...Z.d.S.
+00000070: 290a e901 0000 0029 01da 0873 6571 326c  )......)...seq2l
+00000080: 6973 7429 01da 0661 6132 6964 7829 01da  ist)...aa2idx)..
+00000090: 0769 6a32 696e 6473 e900 0000 004e 2903  .ij2inds.....N).
+000000a0: e902 0000 0072 0100 0000 7206 0000 00e9  .....r....r.....
+000000b0: 1400 0000 6303 0000 0000 0000 0000 0000  ....c...........
+000000c0: 000b 0000 0009 0000 0043 0000 0073 d200  .........C...s..
+000000d0: 0000 7c01 6401 1900 7c01 6402 1900 1700  ..|.d...|.d.....
+000000e0: 7c01 6403 1900 1700 7d03 7400 7c00 7401  |.d.....}.t.|.t.
+000000f0: 7c03 8301 8302 7d04 7402 a003 7404 7c04  |.....}.t...t.|.
+00000100: 6400 6400 8502 6401 7c01 6401 1900 8502  d.d...d.|.d.....
+00000110: 6602 1900 7c02 8302 7404 7c04 6400 6400  f...|...t.|.d.d.
+00000120: 8502 7c03 7c01 6403 1900 1800 7c03 8502  ..|.|.d.....|...
+00000130: 6602 1900 7c02 8302 6702 a101 6a05 7d05  f...|...g...j.}.
+00000140: 7c02 7c01 6401 1900 1300 7d06 7406 7c05  |.|.d.....}.t.|.
+00000150: 7c06 8302 7d07 7c02 7c01 6403 1900 1300  |...}.|.|.d.....
+00000160: 7d08 7402 6a07 6402 7c06 7c08 1400 6602  }.t.j.d.|.|...f.
+00000170: 7401 6404 8d02 7d09 7402 6a08 7c07 6405  t.d...}.t.j.|.d.
+00000180: 6405 6406 6400 6407 8d05 5c02 7d07 7d0a  d.d.d.d...\.}.}.
+00000190: 7c0a 7c09 6401 7c07 6402 1800 6602 3c00  |.|.d.|.d...f.<.
+000001a0: 7c09 5300 2908 4e72 0500 0000 7201 0000  |.S.).Nr....r...
+000001b0: 0072 0600 0000 2901 5a05 6474 7970 6546  .r....).Z.dtypeF
+000001c0: 5429 045a 0c72 6574 7572 6e5f 696e 6465  T).Z.return_inde
+000001d0: 785a 0e72 6574 7572 6e5f 696e 7665 7273  xZ.return_invers
+000001e0: 655a 0d72 6574 7572 6e5f 636f 756e 7473  eZ.return_counts
+000001f0: 5a04 6178 6973 2909 7202 0000 00da 0369  Z.axis).r......i
+00000200: 6e74 da02 6e70 da05 6172 7261 7972 0300  nt..np..arrayr..
+00000210: 0000 da01 5472 0400 0000 5a05 7a65 726f  ....Tr....Z.zero
+00000220: 73da 0675 6e69 7175 6529 0b5a 0478 7365  s..unique).Z.xse
+00000230: 71da 046d 6173 6b5a 0764 6566 5369 7a65  q..maskZ.defSize
+00000240: da01 74da 0573 6c69 6365 5a02 7879 da05  ..t..sliceZ.xy..
+00000250: 6c69 6e65 735a 0469 6e64 73da 0463 6f6c  linesZ.inds..col
+00000260: 73da 014d da06 636f 756e 7473 a900 7214  s..M..counts..r.
+00000270: 0000 00fa 3f62 7569 6c64 5c62 6469 7374  ....?build\bdist
+00000280: 2e77 696e 2d61 6d64 3634 5c65 6767 5c73  .win-amd64\egg\s
+00000290: 7765 6570 5c73 7765 6570 5f73 7570 706f  weep\sweep_suppo
+000002a0: 7274 5c6d 6173 6b32 7665 635f 636f 756e  rt\mask2vec_coun
+000002b0: 742e 7079 da0e 6d61 736b 3276 6563 5f63  t.py..mask2vec_c
+000002c0: 6f75 6e74 0700 0000 7326 0000 0018 010e  ount....s&......
+000002d0: 0120 0120 0104 ff02 0102 ff0c 020a 010c  . . ............
+000002e0: 0116 0106 0302 0102 0102 0102 010a fc10  ................
+000002f0: 0504 0172 1600 0000 2906 7202 0000 0072  ...r....).r....r
+00000300: 0300 0000 7204 0000 00da 056e 756d 7079  ....r......numpy
+00000310: 7209 0000 0072 1600 0000 7214 0000 0072  r....r....r....r
+00000320: 1400 0000 7214 0000 0072 1500 0000 da08  ....r....r......
+00000330: 3c6d 6f64 756c 653e 0100 0000 730a 0000  <module>....s...
+00000340: 000c 020c 010c 0108 0116 01              ...........
```

