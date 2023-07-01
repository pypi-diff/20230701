# Comparing `tmp/openabc-1.0.3.tar.gz` & `tmp/openabc-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openabc-1.0.3.tar", last modified: Sat Apr 22 03:38:08 2023, max compression
+gzip compressed data, was "openabc-1.0.4.tar", last modified: Sat Jul  1 20:59:43 2023, max compression
```

## Comparing `openabc-1.0.3.tar` & `openabc-1.0.4.tar`

### file list

```diff
@@ -1,49 +1,62 @@
-drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-22 03:38:08.000000 openabc-1.0.3/
--rw-rw----   0 sliu     (61642) sliu     (61642)     1080 2023-04-14 18:10:57.000000 openabc-1.0.3/LICENSE
--rw-rw----   0 sliu     (61642) sliu     (61642)      121 2023-04-14 20:42:49.000000 openabc-1.0.3/MANIFEST.in
--rw-rw----   0 sliu     (61642) sliu     (61642)     1377 2023-04-22 03:38:08.000000 openabc-1.0.3/PKG-INFO
--rw-rw----   0 sliu     (61642) sliu     (61642)     1094 2023-04-14 21:02:42.000000 openabc-1.0.3/README.md
--rw-rw----   0 sliu     (61642) sliu     (61642)      428 2023-04-22 03:20:37.000000 openabc-1.0.3/pyproject.toml
--rw-rw----   0 sliu     (61642) sliu     (61642)       38 2023-04-22 03:38:08.000000 openabc-1.0.3/setup.cfg
-drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-22 03:38:08.000000 openabc-1.0.3/src/
-drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-22 03:38:08.000000 openabc-1.0.3/src/openabc/
--rw-rw----   0 sliu     (61642) sliu     (61642)       23 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/__init__.py
-drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-22 03:38:08.000000 openabc-1.0.3/src/openabc/forcefields/
--rw-rw----   0 sliu     (61642) sliu     (61642)       73 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/__init__.py
--rw-rw----   0 sliu     (61642) sliu     (61642)    11969 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/cg_model.py
-drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-22 03:38:08.000000 openabc-1.0.3/src/openabc/forcefields/functional_terms/
--rw-rw----   0 sliu     (61642) sliu     (61642)      114 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/functional_terms/__init__.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     1316 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/functional_terms/angle_terms.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     4121 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/functional_terms/bond_terms.py
--rw-rw----   0 sliu     (61642) sliu     (61642)      716 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/functional_terms/dihedral_terms.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     9268 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/functional_terms/nonbonded_terms.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     3281 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/functional_terms/zero_offset_nonbonded_terms.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     4779 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/hps_model.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     3058 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/hps_zero_offset_model.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     9863 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/moff_mrg_model.py
-drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-22 03:38:08.000000 openabc-1.0.3/src/openabc/forcefields/parameters/
--rw-rw----   0 sliu     (61642) sliu     (61642)     4287 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/parameters/HPS_KR_parameters.csv
--rw-rw----   0 sliu     (61642) sliu     (61642)     4904 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/parameters/HPS_Urry_parameters.csv
--rw-rw----   0 sliu     (61642) sliu     (61642)    11557 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/parameters/MOFF_contact_parameters.csv
--rw-rw----   0 sliu     (61642) sliu     (61642)     3372 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/parameters/parse_hps_parameters.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     1231 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/parameters/parse_moff_parameters.py
--rw-rw----   0 sliu     (61642) sliu     (61642)    12545 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/parameters/template_MOFF.top
-drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-22 03:38:08.000000 openabc-1.0.3/src/openabc/forcefields/parsers/
--rw-rw----   0 sliu     (61642) sliu     (61642)      110 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/parsers/__init__.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     4016 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/parsers/hps_parser.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     9129 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/parsers/moff_parser.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     7485 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/parsers/mrg_parser.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     7347 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/rigid.py
-drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-22 03:38:08.000000 openabc-1.0.3/src/openabc/utils/
--rw-rw----   0 sliu     (61642) sliu     (61642)     9311 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/utils/CA2AA.py
--rw-rw----   0 sliu     (61642) sliu     (61642)        0 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/utils/__init__.py
--rw-rw----   0 sliu     (61642) sliu     (61642)    11105 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/utils/helper_functions.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     5142 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/utils/insert.py
--rw-rw----   0 sliu     (61642) sliu     (61642)    11519 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/utils/legacy_shadow_map.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     9107 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/utils/replica_exchange.py
--rw-rw----   0 sliu     (61642) sliu     (61642)    15160 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/utils/shadow_map.py
-drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-22 03:38:08.000000 openabc-1.0.3/src/openabc.egg-info/
--rw-rw----   0 sliu     (61642) sliu     (61642)     1377 2023-04-22 03:38:08.000000 openabc-1.0.3/src/openabc.egg-info/PKG-INFO
--rw-rw----   0 sliu     (61642) sliu     (61642)     1562 2023-04-22 03:38:08.000000 openabc-1.0.3/src/openabc.egg-info/SOURCES.txt
--rw-rw----   0 sliu     (61642) sliu     (61642)        1 2023-04-22 03:38:08.000000 openabc-1.0.3/src/openabc.egg-info/dependency_links.txt
--rw-rw----   0 sliu     (61642) sliu     (61642)        8 2023-04-22 03:38:08.000000 openabc-1.0.3/src/openabc.egg-info/top_level.txt
+drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-07-01 20:59:43.000000 openabc-1.0.4/
+-rw-rw----   0 sliu     (61642) sliu     (61642)     1080 2023-04-03 01:33:01.000000 openabc-1.0.4/LICENSE
+-rw-rw----   0 sliu     (61642) sliu     (61642)      151 2023-07-01 20:58:48.000000 openabc-1.0.4/MANIFEST.in
+-rw-rw----   0 sliu     (61642) sliu     (61642)     5457 2023-07-01 20:59:43.000000 openabc-1.0.4/PKG-INFO
+-rw-rw----   0 sliu     (61642) sliu     (61642)     5174 2023-06-30 20:33:26.000000 openabc-1.0.4/README.md
+drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-07-01 20:59:42.000000 openabc-1.0.4/openabc/
+-rw-rw----   0 sliu     (61642) sliu     (61642)       23 2023-06-30 20:23:48.000000 openabc-1.0.4/openabc/__init__.py
+drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-07-01 20:59:42.000000 openabc-1.0.4/openabc/forcefields/
+-rw-rw----   0 sliu     (61642) sliu     (61642)      110 2023-06-30 20:23:47.000000 openabc-1.0.4/openabc/forcefields/__init__.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)    12326 2023-06-30 20:23:47.000000 openabc-1.0.4/openabc/forcefields/cg_model.py
+drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-07-01 20:59:42.000000 openabc-1.0.4/openabc/forcefields/functional_terms/
+-rw-rw----   0 sliu     (61642) sliu     (61642)      114 2023-06-30 20:23:47.000000 openabc-1.0.4/openabc/forcefields/functional_terms/__init__.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     1971 2023-06-30 20:23:47.000000 openabc-1.0.4/openabc/forcefields/functional_terms/angle_terms.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     5486 2023-06-30 20:23:47.000000 openabc-1.0.4/openabc/forcefields/functional_terms/bond_terms.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)      712 2023-06-30 20:23:47.000000 openabc-1.0.4/openabc/forcefields/functional_terms/dihedral_terms.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)    12637 2023-06-30 20:23:47.000000 openabc-1.0.4/openabc/forcefields/functional_terms/nonbonded_terms.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     3154 2023-06-30 20:23:47.000000 openabc-1.0.4/openabc/forcefields/functional_terms/zero_offset_nonbonded_terms.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     4617 2023-06-30 20:23:47.000000 openabc-1.0.4/openabc/forcefields/hps_model.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     2960 2023-06-30 20:23:47.000000 openabc-1.0.4/openabc/forcefields/hps_zero_offset_model.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)    11022 2023-06-30 20:23:47.000000 openabc-1.0.4/openabc/forcefields/moff_mrg_model.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     4814 2023-06-30 20:23:48.000000 openabc-1.0.4/openabc/forcefields/mpipi_model.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     1785 2023-06-30 20:23:48.000000 openabc-1.0.4/openabc/forcefields/mpipi_zero_offset_model.py
+drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-07-01 20:59:42.000000 openabc-1.0.4/openabc/forcefields/parameters/
+-rw-rw----   0 sliu     (61642) sliu     (61642)     4287 2023-06-30 20:23:47.000000 openabc-1.0.4/openabc/forcefields/parameters/HPS_KR_parameters.csv
+-rw-rw----   0 sliu     (61642) sliu     (61642)     4904 2023-06-30 20:23:47.000000 openabc-1.0.4/openabc/forcefields/parameters/HPS_Urry_parameters.csv
+-rw-rw----   0 sliu     (61642) sliu     (61642)    11557 2023-06-30 20:23:47.000000 openabc-1.0.4/openabc/forcefields/parameters/MOFF_contact_parameters.csv
+-rw-rw----   0 sliu     (61642) sliu     (61642)     9161 2023-06-30 20:23:47.000000 openabc-1.0.4/openabc/forcefields/parameters/Mpipi_parameters.csv
+-rw-r-----   0 sliu     (61642) sliu     (61642)    74920 2023-06-30 20:23:47.000000 openabc-1.0.4/openabc/forcefields/parameters/lammps_Mpipi_RNA.in
+-rw-rw----   0 sliu     (61642) sliu     (61642)     3372 2023-06-30 20:23:47.000000 openabc-1.0.4/openabc/forcefields/parameters/parse_hps_parameters.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     1217 2023-06-30 20:23:47.000000 openabc-1.0.4/openabc/forcefields/parameters/parse_moff_parameters.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     2133 2023-06-30 20:23:47.000000 openabc-1.0.4/openabc/forcefields/parameters/parse_mpipi_parameters.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)    12545 2023-06-30 20:23:47.000000 openabc-1.0.4/openabc/forcefields/parameters/template_MOFF.top
+drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-07-01 20:59:42.000000 openabc-1.0.4/openabc/forcefields/parsers/
+-rw-rw----   0 sliu     (61642) sliu     (61642)      173 2023-06-30 20:23:47.000000 openabc-1.0.4/openabc/forcefields/parsers/__init__.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     3939 2023-06-30 20:23:47.000000 openabc-1.0.4/openabc/forcefields/parsers/hps_parser.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)    10453 2023-06-30 20:23:47.000000 openabc-1.0.4/openabc/forcefields/parsers/moff_parser.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     7283 2023-06-30 20:23:47.000000 openabc-1.0.4/openabc/forcefields/parsers/mpipi_parsers.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     7563 2023-06-30 20:23:47.000000 openabc-1.0.4/openabc/forcefields/parsers/mrg_parser.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     7435 2023-06-30 20:23:47.000000 openabc-1.0.4/openabc/forcefields/rigid.py
+drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-07-01 20:59:42.000000 openabc-1.0.4/openabc/lib/
+-rw-rw----   0 sliu     (61642) sliu     (61642)        0 2023-06-30 20:23:48.000000 openabc-1.0.4/openabc/lib/__init__.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)       91 2023-06-30 20:23:48.000000 openabc-1.0.4/openabc/lib/dna_lib.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)      447 2023-06-30 20:23:48.000000 openabc-1.0.4/openabc/lib/physical_constants.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)      681 2023-06-30 20:23:48.000000 openabc-1.0.4/openabc/lib/protein_lib.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)       83 2023-06-30 20:23:48.000000 openabc-1.0.4/openabc/lib/rna_lib.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)       88 2023-06-30 20:23:48.000000 openabc-1.0.4/openabc/lib/unit_conversion.py
+drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-07-01 20:59:43.000000 openabc-1.0.4/openabc/utils/
+-rw-rw----   0 sliu     (61642) sliu     (61642)     9311 2023-06-30 20:23:48.000000 openabc-1.0.4/openabc/utils/CA2AA.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)        0 2023-06-30 20:23:48.000000 openabc-1.0.4/openabc/utils/__init__.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)    12155 2023-06-30 20:23:48.000000 openabc-1.0.4/openabc/utils/helper_functions.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     5142 2023-06-30 20:23:48.000000 openabc-1.0.4/openabc/utils/insert.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)    11519 2023-06-30 20:23:48.000000 openabc-1.0.4/openabc/utils/legacy_shadow_map.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     9300 2023-06-30 20:23:48.000000 openabc-1.0.4/openabc/utils/replica_exchange.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)    15004 2023-06-30 20:23:48.000000 openabc-1.0.4/openabc/utils/shadow_map.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     1347 2023-06-30 20:23:48.000000 openabc-1.0.4/openabc/utils/stride.py
+drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-07-01 20:59:42.000000 openabc-1.0.4/openabc.egg-info/
+-rw-rw----   0 sliu     (61642) sliu     (61642)     5457 2023-07-01 20:59:42.000000 openabc-1.0.4/openabc.egg-info/PKG-INFO
+-rw-rw----   0 sliu     (61642) sliu     (61642)     1899 2023-07-01 20:59:42.000000 openabc-1.0.4/openabc.egg-info/SOURCES.txt
+-rw-rw----   0 sliu     (61642) sliu     (61642)        1 2023-07-01 20:59:42.000000 openabc-1.0.4/openabc.egg-info/dependency_links.txt
+-rw-rw----   0 sliu     (61642) sliu     (61642)        8 2023-07-01 20:59:42.000000 openabc-1.0.4/openabc.egg-info/top_level.txt
+-rw-rw----   0 sliu     (61642) sliu     (61642)      467 2023-07-01 20:45:54.000000 openabc-1.0.4/pyproject.toml
+-rw-rw----   0 sliu     (61642) sliu     (61642)       38 2023-07-01 20:59:43.000000 openabc-1.0.4/setup.cfg
```

### Comparing `openabc-1.0.3/LICENSE` & `openabc-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openabc-1.0.3/src/openabc/forcefields/cg_model.py` & `openabc-1.0.4/openabc/forcefields/cg_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 import numpy as np
 import pandas as pd
-import simtk.openmm as mm
-import simtk.openmm.app as app
-import simtk.unit as unit
-from openmmplumed import PlumedForce
+try:
+    import openmm as mm
+    import openmm.app as app
+    import openmm.unit as unit
+except ImportError:
+    import simtk.openmm as mm
+    import simtk.openmm.app as app
+    import simtk.unit as unit
+try:
+    from openmmplumed import PlumedForce
+except ImportError:
+    print('openmmplumed is not installed. PlumedForce is not supported.')
 from openabc.forcefields.rigid import createRigidBodies
 import openabc.utils.helper_functions as helper_functions
 import sys
 import os
 
 class CGModel(object):
     """
@@ -181,16 +189,20 @@
         
         Reference
         ---------
             PLUMED website: https://www.plumed.org/
         
         """
         with open(plumed_script_path, 'r') as input_reader:
-            force = PlumedForce(input_reader.read())
-        self.system.addForce(force)
+            plumed_script = input_reader.read()
+        try:
+            force = PlumedForce(plumed_script)
+            self.system.addForce(force)
+        except NameError:
+            print('PlumedForce is not loaded.')
     
     def save_system(self, system_xml='system.xml'):
         """
         Save system to readable xml format. 
         
         Parameters
         ----------
@@ -214,15 +226,14 @@
         with open(state_xml, 'w') as output_writer:
             state = self.simulation.context.getState(getPositions=True, getVelocities=True, getForces=True, 
                                                      getEnergy=True, getParameters=True, 
                                                      enforcePeriodicBox=self.use_pbc)
             output_writer.write(mm.XmlSerializer.serialize(state))
     
     def set_simulation(self, integrator, platform_name='CPU', properties={'Precision': 'mixed'}, init_coord=None):
-        platform = mm.Platform.getPlatformByName(platform_name)
         """
         Set OpenMM simulation.
         
         Parameters
         ----------
         integrator : OpenMM Integrator
             OpenMM integrator. 
@@ -233,14 +244,15 @@
         properties : dict
             OpenMM simulation platform properties. 
         
         init_coord : None or array-like
             Initial coordinate. 
         
         """
+        platform = mm.Platform.getPlatformByName(platform_name)
         print(f'Use platform: {platform_name}')
         if platform_name in ['CUDA', 'OpenCL']:
             if 'Precision' not in properties:
                 properties['Precision'] = 'mixed'
             precision = properties['Precision']
             print(f'Use precision: {precision}')
             self.simulation = app.Simulation(self.top, self.system, integrator, platform, properties)
```

### Comparing `openabc-1.0.3/src/openabc/forcefields/functional_terms/nonbonded_terms.py` & `openabc-1.0.4/openabc/forcefields/functional_terms/nonbonded_terms.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 import numpy as np
 import pandas as pd
-import simtk.openmm as mm
-import simtk.openmm.app as app
-import simtk.unit as unit
+try:
+    import openmm as mm
+    import openmm.unit as unit
+except ImportError:
+    import simtk.openmm as mm
+    import simtk.unit as unit
+from openabc.lib.physical_constants import NA, kB, EC, VEP
 import math
 import sys
 import os
 
-'''
+"""
 Note addGlobalParameter can automatically convert the values to the correct unit. 
 Be careful that addGlobalParameter sets global parameters that is used by all the forces in the system. 
-'''
-
-# define some constants based on CODATA
-NA = unit.AVOGADRO_CONSTANT_NA # Avogadro constant
-kB = unit.BOLTZMANN_CONSTANT_kB  # Boltzmann constant
-EC = 1.602176634e-19*unit.coulomb # elementary charge
-VEP = 8.8541878128e-12*unit.farad/unit.meter # vacuum electric permittivity
+"""
 
 def moff_mrg_contact_term(atom_types, df_exclusions, use_pbc, alpha_map, epsilon_map, eta=0.7/unit.angstrom, 
                           r0=8.0*unit.angstrom, cutoff=2.0*unit.nanometer, force_group=5):
-    '''
+    """
     MOFF+MRG model nonbonded contact term.
-    '''
+    """
     eta_value = eta.value_in_unit(unit.nanometer**-1)
     r0_value = r0.value_in_unit(unit.nanometer)
     cutoff_value = cutoff.value_in_unit(unit.nanometer)
     contacts = mm.CustomNonbondedForce(f'''energy;
                energy=(energy1+energy2-offset1-offset2)*step({cutoff_value}-r);
                energy1=alpha_con/(r^12);
                energy2=-0.5*epsilon_con*(1+tanh({eta_value}*({r0_value}-r)));
@@ -50,19 +48,19 @@
     else:
         contacts.setNonbondedMethod(contacts.CutoffNonPeriodic)
     contacts.setCutoffDistance(cutoff)
     contacts.setForceGroup(force_group)
     return contacts
 
 
-def hps_ah_term(atom_types, df_exclusions, use_pbc, epsilon, sigma_ah_map, lambda_ah_map, force_group=2):
-    '''
-    HPS model nonbonded contact term (form proposed by Ashbaugh and Hatch). 
+def ashbaugh_hatch_term(atom_types, df_exclusions, use_pbc, epsilon, sigma_ah_map, lambda_ah_map, force_group=2):
+    """
+    Ashbaugh-Hatch potential. 
     The cutoff is 4*sigma_ah. 
-    '''
+    """
     lj_at_cutoff = 4*epsilon*((1/4)**12 - (1/4)**6)
     contacts = mm.CustomNonbondedForce(f'''energy;
                energy=(f1+f2-offset)*step(4*sigma_ah-r);
                offset=lambda_ah*{lj_at_cutoff};
                f1=(lj+(1-lambda_ah)*{epsilon})*step(2^(1/6)*sigma_ah-r);
                f2=lambda_ah*lj*step(r-2^(1/6)*sigma_ah);
                lj=4*{epsilon}*((sigma_ah/r)^12-(sigma_ah/r)^6);
@@ -86,17 +84,17 @@
     contacts.setCutoffDistance(4*np.amax(sigma_ah_map))
     contacts.setForceGroup(force_group)
     return contacts
 
 
 def ddd_dh_elec_term(charges, df_exclusions, use_pbc, salt_conc=150.0*unit.millimolar, 
                      temperature=300.0*unit.kelvin, cutoff=4.0*unit.nanometer, force_group=6):
-    '''
+    """
     Debye-Huckel potential with a distance-dependent dielectric.
-    '''
+    """
     alpha = NA*EC**2/(4*np.pi*VEP)
     gamma = VEP*kB*temperature/(2.0*NA*salt_conc*EC**2)
     # use a distance-dependent relative permittivity (dielectric)
     dielectric_water = 78.4
     A = -8.5525
     kappa = 7.7839
     B = dielectric_water - A
@@ -125,19 +123,19 @@
     elec.setForceGroup(force_group)
     return elec
     
 
 def ddd_dh_elec_switch_term(charges, df_exclusions, use_pbc, salt_conc=150.0*unit.millimolar, 
                             temperature=300.0*unit.kelvin, cutoff1=1.2*unit.nanometer, cutoff2=1.5*unit.nanometer, 
                             switch_coeff=[1, 0, 0, -10, 15, -6], force_group=6):
-    '''
+    """
     Debye-Huckel potential with a distance-dependent dielectric and a switch function. 
     The switch function value changes from 1 to 0 smoothly as distance r changes from cutoff1 to cutoff2. 
     To make sure the switch function works properly, the zeroth order coefficient has to be 1, and the sum of all the coefficients in switch_coeff has to be 0. 
-    '''
+    """
     alpha = NA*EC**2/(4*np.pi*VEP)
     gamma = VEP*kB*temperature/(2.0*NA*salt_conc*EC**2)
     # use a distance-dependent relative permittivity (dielectric)
     dielectric_water = 78.4
     A = -8.5525
     kappa = 7.7839
     B = dielectric_water - A
@@ -173,17 +171,46 @@
     elec.setCutoffDistance(cutoff2)
     elec.setForceGroup(force_group)
     return elec
 
 
 def dh_elec_term(charges, df_exclusions, use_pbc, ldby=1*unit.nanometer, dielectric_water=80.0, 
                  cutoff=3.5*unit.nanometer, force_group=3):
-    '''
-    Debye-Huckel potential with a constant dielectric.
-    '''
+    """
+    Debye-Huckel potential with a constant dielectric. 
+    
+    Parameters
+    ----------
+    charges : sequence-like
+        Atom charges. 
+    
+    df_exclusions : pd.DataFrame
+        Nonbonded exclusions. 
+    
+    use_pbc : bool
+        Whether to use PBC. 
+    
+    ldby : Quantity
+        Debye length. 
+    
+    dielectric_water : float or int
+        Water dielectric constant. 
+    
+    cutoff : Quantity
+        Cutoff distance. 
+    
+    force_group : int
+        Force group. 
+    
+    returns
+    -------
+    elec : Force
+        Electrostatic interaction force. 
+    
+    """
     alpha = NA*EC**2/(4*np.pi*VEP)
     ldby_value = ldby.value_in_unit(unit.nanometer)
     alpha_value = alpha.value_in_unit(unit.kilojoule_per_mole*unit.nanometer)
     cutoff_value = cutoff.value_in_unit(unit.nanometer)
     elec = mm.CustomNonbondedForce(f'''energy;
            energy=q1*q2*{alpha_value}*((exp(-r/{ldby_value})/r)-offset)*step({cutoff_value}-r)/{dielectric_water};
            offset={math.exp(-cutoff_value/ldby_value)/cutoff_value};
@@ -198,8 +225,78 @@
     else:
         elec.setNonbondedMethod(elec.CutoffNonPeriodic)
     elec.setCutoffDistance(cutoff)
     elec.setForceGroup(force_group)
     return elec
 
 
+def wang_frenkel_term(atom_types, df_exclusions, use_pbc, epsilon_wf_map, sigma_wf_map, mu_wf_map, nu_wf_map=1, 
+                      cutoff_to_sigma_ratio=3, force_group=3):
+    """
+    Wang-Fenkel potential term. 
+    
+    Parameters
+    ----------
+    atom_types : sequence-like
+        Atom types. 
+    
+    df_exclusions : pd.DataFrame
+        Nonbonded exclusions. 
+    
+    use_pbc : bool
+        Whether to use PBC. 
+    
+    epsilon_wf_map : 2d sequence-like
+        Matrix of epsilon parameter. 
+    
+    sigma_wf_map : 2d sequence-like
+        Matrix of sigma parameter. 
+    
+    mu_wf_map : 2d sequence-like
+        Matrix of mu parameter. 
+    
+    nu_wf_map : float or int or 2d sequence-like
+        Matrix of nu parameter. 
+        If this variable is float or int, then it means all the pairs have the same nu value. 
+    
+    cutoff_to_sigma_ratio : float or int
+        The ratio of cutoff to sigma. 
+    
+    """
+    contacts = mm.CustomNonbondedForce(f'''energy;
+               energy=epsilon_wf*alpha_wf*g1*g2*step({cutoff_to_sigma_ratio}*sigma_wf-r);
+               g1=(sigma_wf/r)^(2*mu_wf)-1;
+               g2=(({cutoff_to_sigma_ratio}*sigma_wf/r)^(2*mu_wf)-1)^(2*nu_wf);
+               alpha_wf=2*nu_wf*f1*((f2/(2*nu_wf*(f1-1)))^f2);
+               f1={cutoff_to_sigma_ratio}^(2*mu_wf);
+               f2=2*nu_wf+1;
+               epsilon_wf=epsilon_wf_map(atom_type1, atom_type2);
+               sigma_wf=sigma_wf_map(atom_type1, atom_type2);
+               mu_wf=mu_wf_map(atom_type1, atom_type2);
+               nu_wf=nu_wf_map(atom_type1, atom_type2);
+               ''')
+    n_atom_types = epsilon_wf_map.shape[0]
+    discrete_2d_epsilon_wf_map = mm.Discrete2DFunction(n_atom_types, n_atom_types, epsilon_wf_map.ravel().tolist())
+    discrete_2d_sigma_wf_map = mm.Discrete2DFunction(n_atom_types, n_atom_types, sigma_wf_map.ravel().tolist())
+    discrete_2d_mu_wf_map = mm.Discrete2DFunction(n_atom_types, n_atom_types, mu_wf_map.ravel().tolist())
+    if (isinstance(nu_wf_map, int)) or (isinstance(nu_wf_map, float)):
+        nu_wf_map = np.full((n_atom_types, n_atom_types), nu_wf_map)
+    discrete_2d_nu_wf_map = mm.Discrete2DFunction(n_atom_types, n_atom_types, nu_wf_map.ravel().tolist())
+    contacts.addTabulatedFunction('epsilon_wf_map', discrete_2d_epsilon_wf_map)
+    contacts.addTabulatedFunction('sigma_wf_map', discrete_2d_sigma_wf_map)
+    contacts.addTabulatedFunction('mu_wf_map', discrete_2d_mu_wf_map)
+    contacts.addTabulatedFunction('nu_wf_map', discrete_2d_nu_wf_map)
+    contacts.addPerParticleParameter('atom_type')
+    for each in atom_types:
+        contacts.addParticle([each])
+    for i, row in df_exclusions.iterrows():
+        contacts.addExclusion(int(row['a1']), int(row['a2']))
+    if use_pbc:
+        contacts.setNonbondedMethod(contacts.CutoffPeriodic)
+    else:
+        contacts.setNonbondedMethod(contacts.CutoffNonPeriodic)
+    contacts.setCutoffDistance(cutoff_to_sigma_ratio*np.amax(sigma_wf_map))
+    contacts.setForceGroup(force_group)
+    return contacts
+    
+
```

### Comparing `openabc-1.0.3/src/openabc/forcefields/functional_terms/zero_offset_nonbonded_terms.py` & `openabc-1.0.4/openabc/forcefields/functional_terms/zero_offset_nonbonded_terms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 import numpy as np
 import pandas as pd
-import simtk.openmm as mm
-import simtk.openmm.app as app
-import simtk.unit as unit
+try:
+    import openmm as mm
+    import openmm.unit as unit
+except:
+    import simtk.openmm as mm
+    import simtk.unit as unit
+from openabc.lib.physical_constants import NA, kB, EC, VEP
 import math
 import sys
 import os
 
-'''
+"""
 Define some nonbonded interactions with zero offset.
 These forces are used for comparing with outputs from other softwares. 
-'''
+"""
 
-# define some constants based on CODATA
-NA = unit.AVOGADRO_CONSTANT_NA # Avogadro constant
-kB = unit.BOLTZMANN_CONSTANT_kB  # Boltzmann constant
-EC = 1.602176634e-19*unit.coulomb # elementary charge
-VEP = 8.8541878128e-12*unit.farad/unit.meter # vacuum electric permittivity
-
-def hps_ah_zero_offset_term(atom_types, df_exclusions, use_pbc, epsilon, sigma_ah_map, lambda_ah_map, force_group=2):
-    '''
+def ashbaugh_hatch_zero_offset_term(atom_types, df_exclusions, use_pbc, epsilon, sigma_ah_map, lambda_ah_map, 
+                                    force_group=2):
+    """
     HPS model nonbonded contact term (form proposed by Ashbaugh and Hatch). 
     The cutoff is 4*sigma_ah. 
-    '''
+    """
     contacts = mm.CustomNonbondedForce(f'''energy;
                energy=(f1+f2-offset)*step(4*sigma_ah-r);
                offset=0;
                f1=(lj+(1-lambda_ah)*{epsilon})*step(2^(1/6)*sigma_ah-r);
                f2=lambda_ah*lj*step(r-2^(1/6)*sigma_ah);
                lj=4*{epsilon}*((sigma_ah/r)^12-(sigma_ah/r)^6);
                sigma_ah=sigma_ah_map(atom_type1, atom_type2);
@@ -49,17 +48,17 @@
     contacts.setCutoffDistance(4*np.amax(sigma_ah_map))
     contacts.setForceGroup(force_group)
     return contacts
 
 
 def dh_elec_zero_offset_term(charges, df_exclusions, use_pbc, ldby=1*unit.nanometer, dielectric_water=80.0, 
                              cutoff=3.5*unit.nanometer, force_group=3):
-    '''
+    """
     Debye-Huckel potential with a constant dielectric.
-    '''
+    """
     alpha = NA*EC**2/(4*np.pi*VEP)
     ldby_value = ldby.value_in_unit(unit.nanometer)
     alpha_value = alpha.value_in_unit(unit.kilojoule_per_mole*unit.nanometer)
     cutoff_value = cutoff.value_in_unit(unit.nanometer)
     elec = mm.CustomNonbondedForce(f'''energy;
            energy=q1*q2*{alpha_value}*((exp(-r/{ldby_value})/r)-offset)*step({cutoff_value}-r)/{dielectric_water};
            offset=0;
```

### Comparing `openabc-1.0.3/src/openabc/forcefields/hps_model.py` & `openabc-1.0.4/openabc/forcefields/hps_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 import numpy as np
 import pandas as pd
-import simtk.openmm as mm
-import simtk.openmm.app as app
-import simtk.unit as unit
+try:
+    import openmm.unit as unit
+except ImportError:
+    import simtk.unit as unit
 from openabc.forcefields.cg_model import CGModel
-from openabc.forcefields.functional_terms import bond_terms
-from openabc.forcefields.functional_terms import nonbonded_terms
+from openabc.forcefields import functional_terms
+from openabc.lib.protein_lib import _amino_acids
+from openabc.lib.unit_conversion import _kcal_to_kj
 import sys
 import os
 
 __location__ = os.path.dirname(os.path.abspath(__file__))
 
-_amino_acids = ['ALA', 'ARG', 'ASN', 'ASP', 'CYS',
-                'GLN', 'GLU', 'GLY', 'HIS', 'ILE',
-                'LEU', 'LYS', 'MET', 'PHE', 'PRO',
-                'SER', 'THR', 'TRP', 'TYR', 'VAL']
-
-_kcal_to_kj = 4.184
-
 class HPSModel(CGModel):
     """
-    A class for HPS model that represents a mixture of HPS model proteins. 
+    The class for HPS model that represents a mixture of HPS model proteins. 
     
     This class inherits CGModel class. 
     """
     def __init__(self):
         """
         Initialize. 
+        
         """
         self.atoms = None
         self.bonded_attr_names = ['protein_bonds', 'exclusions']
         
     def add_protein_bonds(self, force_group=1):
         """
         Add protein bonds. 
@@ -38,15 +34,15 @@
         Parameters
         ----------
         force_group : int
             Force group. 
         
         """
         print('Add protein bonds.')
-        force = bond_terms.harmonic_bond_term(self.protein_bonds, self.use_pbc, force_group)
+        force = functional_terms.harmonic_bond_term(self.protein_bonds, self.use_pbc, force_group)
         self.system.addForce(force)
     
     def add_contacts(self, hydropathy_scale='Urry', epsilon=0.2*_kcal_to_kj, mu=1, delta=0.08, force_group=2):
         """
         Add nonbonded contacts. 
         
         The raw hydropathy scale is scaled and shifted by: mu*lambda - delta
@@ -86,16 +82,16 @@
             atom_type2 = _amino_acids.index(row['atom_type2'])
             sigma_ah_map[atom_type1, atom_type2] = row['sigma']
             sigma_ah_map[atom_type2, atom_type1] = row['sigma']
             lambda_ah_map[atom_type1, atom_type2] = row['lambda']
             lambda_ah_map[atom_type2, atom_type1] = row['lambda']
         print(f'Scale factor mu = {mu} and shift delta = {delta}.')
         lambda_ah_map = mu*lambda_ah_map - delta
-        force = nonbonded_terms.hps_ah_term(atom_types, self.exclusions, self.use_pbc, epsilon, sigma_ah_map, 
-                                            lambda_ah_map, force_group)
+        force = functional_terms.ashbaugh_hatch_term(atom_types, self.exclusions, self.use_pbc, epsilon, 
+                                                    sigma_ah_map, lambda_ah_map, force_group)
         self.system.addForce(force)
     
     def add_dh_elec(self, ldby=1*unit.nanometer, dielectric_water=80.0, cutoff=3.5*unit.nanometer, force_group=3):
         """
         Add Debye-Huckel electrostatic interactions. 
         
         Parameters
@@ -113,16 +109,16 @@
             Force group. 
         
         """
         print('Add Debye-Huckel electrostatic interactions.')
         print(f'Set Debye length as {ldby.value_in_unit(unit.nanometer)} nm.')
         print(f'Set water dielectric as {dielectric_water}.')
         charges = self.atoms['charge'].tolist()
-        force = nonbonded_terms.dh_elec_term(charges, self.exclusions, self.use_pbc, ldby, dielectric_water, cutoff, 
-                                             force_group)
+        force = functional_terms.dh_elec_term(charges, self.exclusions, self.use_pbc, ldby, dielectric_water, 
+                                              cutoff, force_group)
         self.system.addForce(force)
 
     def add_all_default_forces(self):
         """
         Add all the forces with default settings. 
         """
         print('Add all the forces with default settings.')
```

### Comparing `openabc-1.0.3/src/openabc/forcefields/hps_zero_offset_model.py` & `openabc-1.0.4/openabc/forcefields/hps_zero_offset_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 import numpy as np
 import pandas as pd
-import simtk.openmm as mm
-import simtk.openmm.app as app
-import simtk.unit as unit
+try:
+    import openmm.unit as unit
+except ImportError:
+    import simtk.unit as unit
 from openabc.forcefields.hps_model import HPSModel
-from openabc.forcefields.functional_terms.zero_offset_nonbonded_terms import hps_ah_zero_offset_term
+from openabc.forcefields.functional_terms.zero_offset_nonbonded_terms import ashbaugh_hatch_zero_offset_term
 from openabc.forcefields.functional_terms.zero_offset_nonbonded_terms import dh_elec_zero_offset_term
+from openabc.lib.protein_lib import _amino_acids
+from openabc.lib.unit_conversion import _kcal_to_kj
 import sys
 import os
 
 __location__ = os.path.dirname(os.path.abspath(__file__))
 
-_amino_acids = ['ALA', 'ARG', 'ASN', 'ASP', 'CYS',
-                'GLN', 'GLU', 'GLY', 'HIS', 'ILE',
-                'LEU', 'LYS', 'MET', 'PHE', 'PRO',
-                'SER', 'THR', 'TRP', 'TYR', 'VAL']
-
-_kcal_to_kj = 4.184
-
 class HPSZeroOffsetModel(HPSModel):
     """
     An HPS model with zero offset for nonbonded interactions. 
     This model is only used for comparisons, as HOOMD-Blue HPS model does not shift nonbonded potential to zero at cutoff. 
     """
     def add_contacts(self, hydropathy_scale='Urry', epsilon=0.2*_kcal_to_kj, mu=1, delta=0.08, force_group=2):
         print('Add nonbonded contacts.')
@@ -41,16 +37,16 @@
             atom_type2 = _amino_acids.index(row['atom_type2'])
             sigma_ah_map[atom_type1, atom_type2] = row['sigma']
             sigma_ah_map[atom_type2, atom_type1] = row['sigma']
             lambda_ah_map[atom_type1, atom_type2] = row['lambda']
             lambda_ah_map[atom_type2, atom_type1] = row['lambda']
         print(f'Scale factor mu = {mu} and shift delta = {delta}.')
         lambda_ah_map = mu*lambda_ah_map - delta
-        force = hps_ah_zero_offset_term(atom_types, self.exclusions, self.use_pbc, epsilon, sigma_ah_map, 
-                                        lambda_ah_map, force_group)
+        force = ashbaugh_hatch_zero_offset_term(atom_types, self.exclusions, self.use_pbc, epsilon, sigma_ah_map, 
+                                                lambda_ah_map, force_group)
         self.system.addForce(force)
     
     def add_dh_elec(self, ldby=1*unit.nanometer, dielectric_water=80.0, cutoff=3.5*unit.nanometer, force_group=3):
         print('Add Debye-Huckel electrostatic interactions.')
         print(f'Set Debye length as {ldby.value_in_unit(unit.nanometer)} nm.')
         print(f'Set water dielectric as {dielectric_water}.')
         charges = self.atoms['charge'].tolist()
```

### Comparing `openabc-1.0.3/src/openabc/forcefields/moff_mrg_model.py` & `openabc-1.0.4/openabc/forcefields/moff_mrg_model.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 import numpy as np
 import pandas as pd
-import simtk.openmm as mm
-import simtk.openmm.app as app
-import simtk.unit as unit
+try:
+    import openmm.unit as unit
+except ImportError:
+    import simtk.unit as unit
 from openabc.forcefields.cg_model import CGModel
 from openabc.forcefields import functional_terms
+from openabc.lib.protein_lib import _amino_acids
+from openabc.lib.dna_lib import _dna_nucleotides
 import sys
 import os
 
 __location__ = os.path.dirname(os.path.abspath(__file__))
 
-_amino_acids = ['ALA', 'ARG', 'ASN', 'ASP', 'CYS',
-                'GLN', 'GLU', 'GLY', 'HIS', 'ILE',
-                'LEU', 'LYS', 'MET', 'PHE', 'PRO',
-                'SER', 'THR', 'TRP', 'TYR', 'VAL']
-
-_nucleotides = ['DA', 'DC', 'DG', 'DT']
-
 class MOFFMRGModel(CGModel):
     """
     A class for MOFF+MRG model that represents a mixture of MOFF proteins and MRG DNA. 
     """
     def __init__(self):
         """
         Initialize. 
@@ -41,30 +37,53 @@
         
         """
         if hasattr(self, 'protein_bonds'):
             print('Add protein bonds.')
             force = functional_terms.harmonic_bond_term(self.protein_bonds, self.use_pbc, force_group)
             self.system.addForce(force)
 
-    def add_protein_angles(self, force_group=2):
+    def add_protein_angles(self, threshold=130*np.pi/180, clip=False, force_group=2):
         """
         Add protein angles.
         
+        Note that the angle potential is a harmonic angle potential, which may lead to unstable simulation if harmonic potential center is too large.
+        
+        Based on some tests, theta0 <= 130 degrees (130*np.pi/180 radians) can facilitate 10 fs timestep. 
+        
         Parameters
         ----------
+        threshold : float or int
+            The suggested upper limit value of theta0.
+        
+        clip : bool
+            Whether to change theta0 values larger than threshold to threshold.
+            If True, all the theta0 values larger than threshold will be changed to threshold. 
+            If False, do not change theta0 values.
+        
         force_group : int
             Force group. 
         
         """
         if hasattr(self, 'protein_angles'):
-            print('Add protein angles.')
+            any_theta0_beyond_threshold = False
+            for i, row in self.protein_angles.iterrows():
+                a1 = int(row['a1'])
+                a2 = int(row['a2'])
+                a3 = int(row['a3'])
+                theta0 = float(row['theta0'])
+                if theta0 > threshold:
+                    print(f'Warning: angle composed of atom ({a1}, {a2}, {a3}) has theta0 equal to {theta0}, which is larger than the threshold value equal to {threshold}!')
+                    any_theta0_beyond_threshold = True
+            if clip and any_theta0_beyond_threshold:
+                print(f'Decrease all the theta0 values larger than {threshold} to {threshold}.')
+                self.protein_angles.loc[self.protein_angles['theta0'] > threshold, 'theta0'] = threshold
             force = functional_terms.harmonic_angle_term(self.protein_angles, self.use_pbc, force_group)
             self.system.addForce(force)
     
-    def add_protein_dihedrals(self, k_dihedral_1=3.0, k_dihedral_3=1.5, force_group=3):
+    def add_protein_dihedrals(self, force_group=3):
         """
         Add protein dihedrals. 
         
         Parameters
         ----------
         force_group : int
             Force group. 
@@ -173,27 +192,27 @@
         
         """
         print('Add protein and DNA nonbonded contacts.')
         atom_types = []
         for i, row in self.atoms.iterrows():
             if (row['resname'] in _amino_acids) and (row['name'] == 'CA'):
                 atom_types.append(_amino_acids.index(row['resname']))
-            elif (row['resname'] in _nucleotides) and (row['name'] == 'NU'):
+            elif (row['resname'] in _dna_nucleotides) and (row['name'] == 'DN'):
                 atom_types.append(20)
             else:
                 sys.exit('Error: atom type cannot recognize.')
         df_MOFF_contact_parameters = pd.read_csv(f'{__location__}/parameters/MOFF_contact_parameters.csv')
         alpha_map, epsilon_map = np.zeros((21, 21)), np.zeros((21, 21))
         for i, row in df_MOFF_contact_parameters.iterrows():
-            atom_type1 = _amino_acids.index(row['atom_type1'])
-            atom_type2 = _amino_acids.index(row['atom_type2'])
-            alpha_map[atom_type1, atom_type2] = row['alpha']
-            alpha_map[atom_type2, atom_type1] = row['alpha']
-            epsilon_map[atom_type1, atom_type2] = row['epsilon']
-            epsilon_map[atom_type2, atom_type1] = row['epsilon']
+            a1 = _amino_acids.index(row['atom_type1'])
+            a2 = _amino_acids.index(row['atom_type2'])
+            alpha_map[a1, a2] = row['alpha']
+            alpha_map[a2, a1] = row['alpha']
+            epsilon_map[a1, a2] = row['epsilon']
+            epsilon_map[a2, a1] = row['epsilon']
         alpha_map[:20, 20] = alpha_protein_dna
         alpha_map[20, :20] = alpha_protein_dna
         alpha_map[20, 20] = alpha_dna_dna
         epsilon_map[:20, 20] = epsilon_protein_dna
         epsilon_map[20, :20] = epsilon_protein_dna
         epsilon_map[20, 20] = epsilon_dna_dna
         force = functional_terms.moff_mrg_contact_term(atom_types, self.exclusions, self.use_pbc, alpha_map, 
@@ -218,15 +237,15 @@
         
         cutoff1 : Quantity
             Cutoff distance 1. 
         
         cutoff2 : Quantity
             Cutoff distance 2. 
         
-        switch_coeff : list
+        switch_coeff : sequence-like
             Switch function coefficients. 
         
         add_native_pair_elec : bool
             Whether to add electrostatic interactions between native pairs. 
         
         force_group : int
             Force group.
```

### Comparing `openabc-1.0.3/src/openabc/forcefields/parameters/HPS_KR_parameters.csv` & `openabc-1.0.4/openabc/forcefields/parameters/HPS_KR_parameters.csv`

 * *Files identical despite different names*

### Comparing `openabc-1.0.3/src/openabc/forcefields/parameters/HPS_Urry_parameters.csv` & `openabc-1.0.4/openabc/forcefields/parameters/HPS_Urry_parameters.csv`

 * *Files identical despite different names*

### Comparing `openabc-1.0.3/src/openabc/forcefields/parameters/MOFF_contact_parameters.csv` & `openabc-1.0.4/openabc/forcefields/parameters/MOFF_contact_parameters.csv`

 * *Files identical despite different names*

### Comparing `openabc-1.0.3/src/openabc/forcefields/parameters/parse_hps_parameters.py` & `openabc-1.0.4/openabc/forcefields/parameters/parse_hps_parameters.py`

 * *Files identical despite different names*

### Comparing `openabc-1.0.3/src/openabc/forcefields/parameters/parse_moff_parameters.py` & `openabc-1.0.4/openabc/forcefields/parameters/parse_moff_parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 
 """
 Use this script to produce the .csv files for MOFF nonbonded interaction parameters. 
 The nonbonded interaction form is: abs(epsilon)*(sigma^12)/(r^12)-0.5*epsilon*(1+tanh(eta*(r0-r))).
 Set alpha=abs(epsilon)*(sigma^12).
 """
-df_contact_parameters = pd.DataFrame(columns=['atom_type1', 'atom_type2', 'alpha', 'epsilon', 'sigma'])
+df_MOFF_parameters = pd.DataFrame(columns=['atom_type1', 'atom_type2', 'alpha', 'epsilon', 'sigma'])
 
 with open('template_MOFF.top', 'r') as input_reader:
     template_MOFF_lines = input_reader.readlines()
 
 n_lines = len(template_MOFF_lines)
 for i in range(n_lines):
     if 'nonbond_params' in template_MOFF_lines[i]:
@@ -24,14 +24,12 @@
     elements = template_MOFF_lines[i].split()
     if len(elements) == 5:
         atom_type1 = elements[0]
         atom_type2 = elements[1]
         epsilon = float(elements[3])
         alpha = float(elements[4])
         sigma = (alpha/abs(epsilon))**(1/12)
-        df_contact_parameters.loc[len(df_contact_parameters.index)] = [atom_type1, atom_type2, alpha, epsilon, sigma]
-
-df_contact_parameters.to_csv('MOFF_contact_parameters.csv', index=False)
-
+        df_MOFF_parameters.loc[len(df_MOFF_parameters.index)] = [atom_type1, atom_type2, alpha, epsilon, sigma]
 
+df_MOFF_parameters.to_csv('MOFF_contact_parameters.csv', index=False)
```

### Comparing `openabc-1.0.3/src/openabc/forcefields/parameters/template_MOFF.top` & `openabc-1.0.4/openabc/forcefields/parameters/template_MOFF.top`

 * *Files identical despite different names*

### Comparing `openabc-1.0.3/src/openabc/forcefields/parsers/hps_parser.py` & `openabc-1.0.4/openabc/forcefields/parsers/hps_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,24 @@
 import numpy as np
 import pandas as pd
-import simtk.openmm as mm
-import simtk.openmm.app as app
-import simtk.unit as unit
 from openabc.utils import helper_functions
+from openabc.lib.protein_lib import _amino_acids
+from openabc.lib.unit_conversion import _kcal_to_kj
 import sys
 import os
 
-_amino_acids = ['ALA', 'ARG', 'ASN', 'ASP', 'CYS',
-                'GLN', 'GLU', 'GLY', 'HIS', 'ILE',
-                'LEU', 'LYS', 'MET', 'PHE', 'PRO',
-                'SER', 'THR', 'TRP', 'TYR', 'VAL']
-
 _hps_amino_acid_mass_dict = dict(ALA=71.08, ARG=156.20, ASN=114.10, ASP=115.10, CYS=103.10, 
-                                GLN=128.10, GLU=129.10, GLY=57.05, HIS=137.10, ILE=113.20, 
-                                LEU=113.20, LYS=128.20, MET=131.20, PHE=147.20, PRO=97.12, 
-                                SER=87.08, THR=101.10, TRP=186.20, TYR=163.20, VAL=99.07)
+                                 GLN=128.10, GLU=129.10, GLY=57.05, HIS=137.10, ILE=113.20, 
+                                 LEU=113.20, LYS=128.20, MET=131.20, PHE=147.20, PRO=97.12, 
+                                 SER=87.08, THR=101.10, TRP=186.20, TYR=163.20, VAL=99.07)
 
 _hps_amino_acid_charge_dict = dict(ALA=0.0, ARG=1.0, ASN=0.0, ASP=-1.0, CYS=0.0, 
-                                  GLN=0.0, GLU=-1.0, GLY=0.0, HIS=0.5, ILE=0.0,
-                                  LEU=0.0, LYS=1.0, MET=0.0, PHE=0.0, PRO=0.0,
-                                  SER=0.0, THR=0.0, TRP=0.0, TYR=0.0, VAL=0.0)
-
-_kcal_to_kj = 4.184
+                                   GLN=0.0, GLU=-1.0, GLY=0.0, HIS=0.5, ILE=0.0,
+                                   LEU=0.0, LYS=1.0, MET=0.0, PHE=0.0, PRO=0.0,
+                                   SER=0.0, THR=0.0, TRP=0.0, TYR=0.0, VAL=0.0)
 
 class HPSParser(object):
     """
     HPS protein parser.
     """
     def __init__(self, ca_pdb, default_parse=True):
         """
@@ -62,22 +54,28 @@
         ca_pdb : str
             Output path for the CA pdb file. 
         
         write_TER : bool
             Whether to write TER between two chains. 
         
         default_parse : bool
-            Whether to parse with default settings. 
+            Whether to parse with default settings.
+        
+        Returns
+        ------- 
+        result : class instance
+            A class instance. 
         
         """
         helper_functions.atomistic_pdb_to_ca_pdb(atomistic_pdb, ca_pdb, write_TER)
-        return cls(ca_pdb, default_parse)
+        result = cls(ca_pdb, default_parse)
+        return result
     
     def parse_mol(self, exclude12=True, mass_dict=_hps_amino_acid_mass_dict, 
-                     charge_dict=_hps_amino_acid_charge_dict):
+                  charge_dict=_hps_amino_acid_charge_dict):
         """
         Parse molecule. 
         
         Parameters
         ----------
         exclude12 : bool
             Whether to exclude nonbonded interactions between 1-2 atoms.
```

### Comparing `openabc-1.0.3/src/openabc/forcefields/parsers/moff_parser.py` & `openabc-1.0.4/openabc/forcefields/parsers/moff_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 import numpy as np
 import pandas as pd
-import simtk.openmm as mm
-import simtk.openmm.app as app
-import simtk.unit as unit
 import mdtraj
 from openabc.utils import helper_functions
 from openabc.utils.shadow_map import find_ca_pairs_from_atomistic_pdb
+from openabc.lib.protein_lib import _amino_acids
 import sys
 import os
 
-_amino_acids = ['ALA', 'ARG', 'ASN', 'ASP', 'CYS',
-                'GLN', 'GLU', 'GLY', 'HIS', 'ILE',
-                'LEU', 'LYS', 'MET', 'PHE', 'PRO',
-                'SER', 'THR', 'TRP', 'TYR', 'VAL']
-
 _moff_amino_acid_mass_dict = dict(ALA=71.08, ARG=156.20, ASN=114.10, ASP=115.10, CYS=103.10, 
                                   GLN=128.10, GLU=129.10, GLY=57.05, HIS=137.10, ILE=113.20, 
                                   LEU=113.20, LYS=128.20, MET=131.20, PHE=147.20, PRO=97.12, 
                                   SER=87.08, THR=101.10, TRP=186.20, TYR=163.20, VAL=99.07)
 
 _moff_amino_acid_charge_dict = dict(ALA=0.0, ARG=1.0, ASN=0.0, ASP=-1.0, CYS=0.0, 
                                     GLN=0.0, GLU=-1.0, GLY=0.0, HIS=0.25, ILE=0.0,
@@ -33,18 +26,18 @@
     def __init__(self, atomistic_pdb, ca_pdb, default_parse=True):
         """
         Initialize a protein with MOFF model. 
         
         Parameters
         ----------
         atomistic_pdb : str
-            Path for the atomistic pdb file. 
+            Atomistic pdb file path. 
         
         ca_pdb : str
-            path for the CA pdb file. 
+            CA pdb file path. 
         
         default_parse : bool
             Whether to parse with default settings. 
         
         """
         self.atomistic_pdb = atomistic_pdb
         self.pdb = ca_pdb
@@ -54,33 +47,39 @@
         if default_parse:
             print('Parse molecule with default settings.')
             self.parse_mol()
 
     @classmethod
     def from_atomistic_pdb(cls, atomistic_pdb, ca_pdb, write_TER=False, default_parse=True):
         """
-        Initialize an HPS model protein from atomistic pdb. 
+        Initialize a MOFF model protein from atomistic pdb. 
         
         Parameters
         ----------
         atomistic_pdb : str
-            Path for the atomistic pdb file. 
+            Atomistic pdb file path. 
         
         ca_pdb : str
-            path for the CA pdb file. 
+            CA pdb file path. 
             
         write_TER : bool
             Whether to write TER between two chains. 
         
         default_parse : bool
             Whether to parse with default settings. 
         
+        Returns
+        ------- 
+        result : class instance
+            A class instance. 
+        
         """
         helper_functions.atomistic_pdb_to_ca_pdb(atomistic_pdb, ca_pdb, write_TER)
-        return cls(atomistic_pdb, ca_pdb, default_parse)
+        result = cls(atomistic_pdb, ca_pdb, default_parse)
+        return result
     
     def parse_exclusions(self, exclude12=True, exclude13=True, exclude14=True, exclude_native_pairs=True):
         """
         Parse nonbonded exclusions based on bonds, angles, dihedrals, and native pairs.
         
         Parameters
         ----------
@@ -111,15 +110,15 @@
             for i, row in self.native_pairs.iterrows():
                 exclusions.append((int(row['a1']), int(row['a2'])))
         exclusions = np.array(sorted(exclusions))
         self.exclusions = pd.DataFrame(exclusions, columns=['a1', 'a2']).drop_duplicates(ignore_index=True)
         
     def parse_mol(self, get_native_pairs=True, frame=0, radius=0.1, bonded_radius=0.05, cutoff=0.6, box=None, 
                   use_pbc=False, exclude12=True, exclude13=True, exclude14=True, exclude_native_pairs=True, 
-                  mass_dict=_moff_amino_acid_mass_dict, charge_dict=_moff_amino_acid_charge_dict):
+                  mass_dict=_moff_amino_acid_mass_dict, charge_dict=_moff_amino_acid_charge_dict, ss=None, ordered_ss_names=['H', 'E']):
         """
         Parse molecule.
         
         Parameters
         ----------
         get_native_pairs : bool
             Whether to get native pairs from atomistic pdb with shadow algorithm. 
@@ -134,17 +133,17 @@
             Shadow algorithm bonded radius. 
         
         cutoff : float or int
             Shadow algorithm cutoff. 
         
         box : None or np.ndarray
         Specify box shape. 
-        Note `use_pbc` = False is only compatible with orthogonal box. 
-        If `use_pbc` = False, then set `box` as None. 
-        If `use_pbc` = True, then `box` = np.array([lx, ly, lz, alpha1, alpha2, alpha3]). 
+        Note setting `use_pbc` as False is only compatible with orthogonal box. 
+        If `use_pbc` is False, then set `box` as None. 
+        If `use_pbc` is True, then `box` = np.array([lx, ly, lz, alpha1, alpha2, alpha3]). 
         
         use_pbc : bool
             Whether to use periodic boundary condition (PBC) for searching native pairs. 
         
         exclude12 : bool
             Whether to exclude nonbonded interactions between 1-2 atom pairs. 
         
@@ -159,14 +158,23 @@
         
         mass_dict : dict
             Mass dictionary. 
         
         charge_dict : dict
             Charge dictionary. 
         
+        ss : None or sequence-like
+            Secondary structure type of each residue. 
+            If None, no secondary structure information is provided and all the native pairs are kept.
+            If not None, then only native pairs within continuous ordered 
+        
+        ordered_ss_names : sequence-like
+            The names of ordered secondary structures. 
+            The default value is ['H', 'E'], where 'H' represents alpha-helix, and 'E' represents beta strand. 
+        
         """
         # set bonds, angles, and dihedrals
         bonds, angles, dihedrals = [], [], []
         n_atoms = len(self.atoms.index)
         for atom1 in range(n_atoms):
             chain1 = self.atoms.loc[atom1, 'chainID']
             if atom1 < n_atoms - 1:
@@ -200,15 +208,30 @@
             row = dihedrals[i].tolist() + [3, 3*(phi[i] + np.pi), 1.5]
             self.protein_dihedrals.loc[len(self.protein_dihedrals.index)] = row
         # set native pairs
         if get_native_pairs:
             print('Get native pairs with shadow algorithm.')
             self.native_pairs = find_ca_pairs_from_atomistic_pdb(self.atomistic_pdb, frame, radius, bonded_radius, 
                                                                  cutoff, box, use_pbc)
-            self.native_pairs.loc[:, 'epsilon'] = 3.0
+            self.native_pairs.loc[:, 'epsilon'] = 3.0  
+            if ss is not None:
+                assert n_atoms == len(ss) # the length of ss should be equal to the number of CA atoms
+                print('Secondary structure information is provided.')
+                print('Only native pairs within the continuous ordered secondary structure domains are kept.')
+                old_native_pairs = self.native_pairs
+                new_native_pairs = pd.DataFrame(columns=self.native_pairs.columns)
+                for i, row in old_native_pairs.iterrows():
+                    a1 = int(row['a1'])
+                    a2 = int(row['a2'])
+                    if a1 > a2:
+                        a1, a2 = a2, a1
+                    if ss[a1] in ordered_ss_names:
+                        if all([x == ss[a1] for x in ss[a1:a2 + 1]]):
+                            new_native_pairs.loc[len(new_native_pairs.index)] = row
+                self.native_pairs = new_native_pairs
         # set exclusions
         self.parse_exclusions(exclude12, exclude13, exclude14, exclude_native_pairs) 
         # set mass and charge
         for i, row in self.atoms.iterrows():
             self.atoms.loc[i, 'mass'] = mass_dict[row['resname']]
             self.atoms.loc[i, 'charge'] = charge_dict[row['resname']]
```

### Comparing `openabc-1.0.3/src/openabc/forcefields/parsers/mrg_parser.py` & `openabc-1.0.4/openabc/forcefields/parsers/mrg_parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 import numpy as np
 import pandas as pd
-import simtk.openmm as mm
-import simtk.openmm.app as app
-import simtk.unit as unit
 from openabc.utils import helper_functions
+from openabc.lib.dna_lib import _dna_nucleotides
+from openabc.lib.unit_conversion import _kcal_to_kj, _deg_to_rad
 import sys
 import os
 
-_nucleotides = ['DA', 'DC', 'DG', 'DT']
-
-_kcal_to_kj = 4.184
-_deg_to_rad = np.pi/180
-
 _k_mrg_dna_bonds = _kcal_to_kj*np.array([262.5, -226, 149])
 _r0_mrg_dna_bonds = 0.496
 _k_mrg_dna_angles = _kcal_to_kj*np.array([9.22, 4.16, 1.078])
 _theta0_mrg_dna_angles = 156*_deg_to_rad
 _delta_mrg_dna_fan_bonds = np.arange(-5, 6)
 _k_mrg_dna_fan_bonds = _kcal_to_kj*np.array([[4.67, 2.1, 1.46], 
                                              [1.324e-4, -12.2, 18.5], 
@@ -48,15 +42,15 @@
             Whether to parse with default settings. 
         
         """
         self.pdb = cg_pdb
         self.atoms = helper_functions.parse_pdb(self.pdb)
         # check if all the atoms are CG nucleotide atoms
         atom_names = self.atoms['name']
-        assert (self.atoms['resname'].isin(_nucleotides).all() and atom_names.eq('NU').all())
+        assert (self.atoms['resname'].isin(_dna_nucleotides).all() and atom_names.eq('DN').all())
         # check if there are only 2 chains
         unique_chainID = list(set(self.atoms['chainID'].tolist()))
         assert len(unique_chainID) == 2
         # check if the first half is the first ssDNA, and the second half is the second ssDNA
         n_atoms = len(self.atoms.index)
         n_bp = int(n_atoms/2)
         first_half_atoms = self.atoms.loc[0:n_bp - 1]
@@ -83,17 +77,23 @@
         
         write_TER : bool
             Whether to write TER between two chains. 
         
         default_parse : bool
             Whether to parse with default settings. 
         
+        Returns
+        ------- 
+        result : class instance
+            A class instance. 
+        
         """
         helper_functions.atomistic_pdb_to_nucleotide_pdb(atomistic_pdb, cg_pdb, write_TER)
-        return cls(cg_pdb, default_parse)
+        result = cls(cg_pdb, default_parse)
+        return result
     
     def parse_exclusions(self, exclude12=True, exclude13=True):
         """
         Parse nonbonded exclusions based on bonds and angles. 
         Note nonbonded interactions are not excluded for atom pairs with fan bonds. 
         
         Parameters
```

### Comparing `openabc-1.0.3/src/openabc/forcefields/rigid.py` & `openabc-1.0.4/openabc/forcefields/rigid.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,20 @@
 DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE
 USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 __author__ = "Peter Eastman"
 __version__ = "1.0"
 
-import simtk.openmm as mm
-import simtk.unit as unit
+try:
+    import openmm as mm
+    import openmm.unit as unit
+except ImportError:
+    import simtk.openmm as mm
+    import simtk.unit as unit
 import numpy as np
 import numpy.linalg as lin
 from itertools import combinations
 
 def createRigidBodies(system, positions, bodies):
     """Modify a System to turn specified sets of particles into rigid bodies.
```

### Comparing `openabc-1.0.3/src/openabc/utils/CA2AA.py` & `openabc-1.0.4/openabc/utils/CA2AA.py`

 * *Files identical despite different names*

### Comparing `openabc-1.0.3/src/openabc/utils/helper_functions.py` & `openabc-1.0.4/openabc/utils/helper_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,24 @@
 import numpy as np
 import pandas as pd
 import mdtraj
 import sys
 import os
+from openabc.lib.protein_lib import _amino_acids, _amino_acid_1_letter_to_3_letters_dict
+from openabc.lib.dna_lib import _dna_nucleotides
+from openabc.lib.rna_lib import _rna_nucleotides
 
 """
 Some code is adapted from Open3SPN2. 
 
 Open3SPN2 and OpenAWSEM paper: 
 Lu, Wei, et al. "OpenAWSEM with Open3SPN2: A fast, flexible, and accessible framework for large-scale coarse-grained biomolecular simulations." PLoS computational biology 17.2 (2021): e1008308.
 """
 
-_amino_acids = ['ALA', 'ARG', 'ASN', 'ASP', 'CYS',
-                'GLN', 'GLU', 'GLY', 'HIS', 'ILE',
-                'LEU', 'LYS', 'MET', 'PHE', 'PRO',
-                'SER', 'THR', 'TRP', 'TYR', 'VAL']
-
-_nucleotides = ['DA', 'DC', 'DG', 'DT']
-
-_amino_acid_1_letter_to_3_letters_dict = dict(A='ALA', R='ARG', N='ASN', D='ASP', C='CYS', 
-                                              Q='GLN', E='GLU', G='GLY', H='HIS', I='ILE', 
-                                              L='LEU', K='LYS', M='MET', F='PHE', P='PRO', 
-                                              S='SER', T='THR', W='TRP', Y='TYR', V='VAL')
-
+_nucleotides = _dna_nucleotides + _rna_nucleotides
 
 def parse_pdb(pdb_file):
     """
     Load pdb file as pandas dataframe.
     
     Parameters
     ----------
@@ -125,15 +117,15 @@
     ca_pdb_atoms['serial'] = list(range(1, len(ca_pdb_atoms.index) + 1))
     ca_pdb_atoms.loc[:, 'charge'] = '' # remove charge
     write_pdb(ca_pdb_atoms, ca_pdb, write_TER)
     
 
 def atomistic_pdb_to_nucleotide_pdb(atomistic_pdb, cg_nucleotide_pdb, write_TER=False):
     """
-    Convert atomistic pdb to DNA nucleotide pdb (i.e. one CG bead per nucleotide). 
+    Convert DNA or RNA atomistic pdb to nucleotide pdb (i.e. one CG bead per nucleotide). 
     The position of each CG nucleotide bead is the geometric center of all the nucleotide atoms in the pdb.
     
     Parameters
     ----------
     atomistic_pdb : str
         Path for the atomistic pdb file. 
 
@@ -152,15 +144,23 @@
     atomistic_pdb_atoms.index = chainID.astype(str) + '_' + resSeq.astype(str)
     cg_nucleotide_pdb_atoms = pd.DataFrame(columns=atomistic_pdb_atoms.columns)
     for each in atomistic_pdb_atoms.index.drop_duplicates():
         residue_atoms = atomistic_pdb_atoms.loc[each]
         coord = np.mean(residue_atoms[['x', 'y', 'z']].to_numpy(), axis=0)
         row = residue_atoms.iloc[0].copy()
         row[['x', 'y', 'z']] = coord
-        row[['name', 'occupancy', 'tempFactor', 'element', 'charge']] = ['NU', 1.0, 1.0, '', '']
+        resname = row['resname']
+        # set atom name to distinguish DNA and RNA nucleotides
+        if resname in _dna_nucleotides:
+            name = 'DN'
+        elif resname in _rna_nucleotides:
+            name = 'RN'
+        else:
+            name = ''
+        row[['name', 'occupancy', 'tempFactor', 'element', 'charge']] = [name, 1.0, 1.0, '', '']
         cg_nucleotide_pdb_atoms.loc[len(cg_nucleotide_pdb_atoms.index)] = row
     cg_nucleotide_pdb_atoms['serial'] = list(range(1, len(cg_nucleotide_pdb_atoms.index) + 1))
     write_pdb(cg_nucleotide_pdb_atoms, cg_nucleotide_pdb, write_TER)
 
 
 def build_straight_CA_chain(sequence, r0=0.38):
     """
@@ -180,16 +180,55 @@
         A pandas dataframe includes atom information. 
     
     """
     n_atoms = len(sequence)
     data = []
     for i in range(n_atoms):
         resname = _amino_acid_1_letter_to_3_letters_dict[sequence[i]]
-        atom_i_dict = {'recname': 'ATOM', 'name': 'CA', 'altLoc': '', 'resname': resname, 'chainID': 'A', 'iCode': '', 
-                       'occupancy': 1.0, 'tempFactor': 1.0, 'element': 'C', 'charge': ''}
+        atom_i_dict = {'recname': 'ATOM', 'name': 'CA', 'altLoc': '', 'resname': resname, 'chainID': 'A', 
+                       'iCode': '', 'occupancy': 1.0, 'tempFactor': 1.0, 'element': 'C', 'charge': ''}
+        data.append(atom_i_dict)
+    df_atoms = pd.DataFrame(data)
+    df_atoms['serial'] = list(range(1, n_atoms + 1))
+    df_atoms['resSeq'] = list(range(1, n_atoms + 1))
+    df_atoms.loc[:, 'x'] = 0
+    df_atoms.loc[:, 'y'] = 0
+    z = r0*np.arange(n_atoms)
+    z -= np.mean(z)
+    df_atoms['z'] = z*10 # convert nm to angstroms
+    df_atoms['z'] = df_atoms['z'].round(3)
+    return df_atoms
+
+
+def build_straight_chain(n_atoms, chainID, r0):
+    """
+    Build a straight chain. 
+    Each atom is viewed as one residue. 
+    
+    Parameters
+    ----------
+    n_atoms : int
+        The number of atoms along the chain. 
+    
+    chainID : floar or int or str
+        Chain ID. 
+    
+    r0 : float or int
+        Distance in unit nm between neighboring atoms along the chain. 
+    
+    Returns
+    -------
+    df_atoms : pd.DataFrame
+        A pandas dataframe includes atom information. 
+        
+    """
+    data = []
+    for i in range(n_atoms):
+        atom_i_dict = {'recname': 'ATOM', 'name': '', 'altLoc': '', 'resname': '', 'chainID': chainID, 
+                       'iCode': '', 'occupancy': 1.0, 'tempFactor': 1.0, 'element': '', 'charge': ''}
         data.append(atom_i_dict)
     df_atoms = pd.DataFrame(data)
     df_atoms['serial'] = list(range(1, n_atoms + 1))
     df_atoms['resSeq'] = list(range(1, n_atoms + 1))
     df_atoms.loc[:, 'x'] = 0
     df_atoms.loc[:, 'y'] = 0
     z = r0*np.arange(n_atoms)
```

### Comparing `openabc-1.0.3/src/openabc/utils/insert.py` & `openabc-1.0.4/openabc/utils/insert.py`

 * *Files identical despite different names*

### Comparing `openabc-1.0.3/src/openabc/utils/legacy_shadow_map.py` & `openabc-1.0.4/openabc/utils/legacy_shadow_map.py`

 * *Files identical despite different names*

### Comparing `openabc-1.0.3/src/openabc/utils/replica_exchange.py` & `openabc-1.0.4/openabc/utils/replica_exchange.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 import numpy as np
 import pandas as pd
-import simtk.openmm as mm
-import simtk.openmm.app as app
-import simtk.unit as unit
+try:
+    import openmm as mm
+    import openmm.app as app
+    import openmm.unit as unit
+except ImportError:
+    import simtk.openmm as mm
+    import simtk.openmm.app as app
+    import simtk.unit as unit
+from openabc.lib.physical_constants import GAS_CONST
 import sys
 import os
-import torch
+try:
+    import torch
+except ImportError:
+    print('torch is not supported.')
 import math
 import time
 
 """
 The code is adapted from Xinqiang Ding's script. 
 """
 
 # set gas constant R
-GAS_CONSTANT_R = (1.0*unit.BOLTZMANN_CONSTANT_kB*unit.AVOGADRO_CONSTANT_NA).value_in_unit(unit.kilojoule_per_mole/unit.kelvin)
+GAS_CONST_value = GAS_CONST.value_in_unit(unit.kilojoule_per_mole/unit.kelvin)
 
 class TemperatureReplicaExchange(object):
     """
     Temperature replica exchange class for performing temperature replica exchange (TRE) simulations. 
     
     Note only positions and scaled velocities are exchanged, while other internal states of the simulations are not exchanged. This means the class may not be properly applied to simulations involving other internal states. For example, Nose-Hoover integrator may not work properly as it includes internal chain states. 
     
@@ -168,15 +177,15 @@
             torch.distributed.all_gather(gathered_velocities, velocities)
             torch.distributed.all_gather(gathered_potential_energy, potential_energy)
             gathered_potential_energy = torch.stack(gathered_potential_energy).reshape(-1)
             if self.rank == 0:
                 for j in range(self.n_replicas - 1):
                     n_exchange_attempts += 1
                     delta_potential_energy = gathered_potential_energy[j] - gathered_potential_energy[j + 1]
-                    delta_beta = (1/self.temperatures[j] - 1/self.temperatures[j + 1])/GAS_CONSTANT_R
+                    delta_beta = (1/self.temperatures[j] - 1/self.temperatures[j + 1])/GAS_CONST_value
                     if np.random.uniform(0, 1) < math.exp(delta_beta*delta_potential_energy):
                         n_accepted_exchange_attempts += 1
                         gathered_positions[j], gathered_positions[j + 1] = gathered_positions[j + 1], gathered_positions[j]
                         alpha = (self.temperatures[j]/self.temperatures[j + 1])**0.5
                         gathered_velocities[j], gathered_velocities[j + 1] = alpha*gathered_velocities[j + 1], gathered_velocities[j]/alpha
                         gathered_potential_energy[j], gathered_potential_energy[j + 1] = gathered_potential_energy[j + 1], gathered_potential_energy[j]
             else:
```

### Comparing `openabc-1.0.3/src/openabc/utils/shadow_map.py` & `openabc-1.0.4/openabc/utils/shadow_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import pandas as pd
 import mdtraj
 from MDAnalysis.lib.nsgrid import FastNS
+from openabc.lib.protein_lib import _amino_acids
 import networkx as nx
 import math
 import sys
 import os
 
 __location__ = os.path.dirname(os.path.abspath(__file__))
 
@@ -18,19 +19,14 @@
 Noel, Jeffrey K., Paul C. Whitford, and José N. Onuchic. "The shadow map: a general contact definition for capturing the dynamics of biomolecular folding and function." The journal of physical chemistry B 116.29 (2012): 8692-8702.
 
 This algorithm is applied to find contacts between residues (a residue can be an amino acid or a nucleotide)
 
 This script also includes some useful functions. 
 '''
 
-_amino_acids = ['ALA', 'ARG', 'ASN', 'ASP', 'CYS',
-                'GLN', 'GLU', 'GLY', 'HIS', 'ILE',
-                'LEU', 'LYS', 'MET', 'PHE', 'PRO',
-                'SER', 'THR', 'TRP', 'TYR', 'VAL']
-
 
 def get_neighbor_pairs_and_distances(coord, cutoff=0.6, box=None, use_pbc=False):
     '''
     Find spatially neighboring atom pairs within cutoff range based on MDAnalysis. 
     
     Parameters
     ----------
@@ -319,16 +315,16 @@
     
     Returns
     -------
     df_ca_pairs : pd.DataFrame
         Pandas DataFrame including CA atom pair indices and distances. 
     
     '''
-    res_pairs, df_atoms = find_res_pairs_from_atomistic_pdb(atomistic_pdb, frame, radius, bonded_radius, cutoff, box, 
-                                                            use_pbc)
+    res_pairs, df_atoms = find_res_pairs_from_atomistic_pdb(atomistic_pdb, frame, radius, bonded_radius, cutoff, 
+                                                            box, use_pbc)
     # pick out CA atoms for each residue
     dict_res_CA = {}
     for i, row in df_atoms.iterrows():
         if (row['resName'] in _amino_acids) and (row['name'] == 'CA'):
             unique_resSeq = df_atoms.loc[i, 'unique_resSeq']
             dict_res_CA[unique_resSeq] = i
     df_ca_pairs = pd.DataFrame(columns=['a1', 'a2', 'mu'])
```

### Comparing `openabc-1.0.3/src/openabc.egg-info/SOURCES.txt` & `openabc-1.0.4/openabc.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,51 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-src/openabc/__init__.py
-src/openabc.egg-info/PKG-INFO
-src/openabc.egg-info/SOURCES.txt
-src/openabc.egg-info/dependency_links.txt
-src/openabc.egg-info/top_level.txt
-src/openabc/forcefields/__init__.py
-src/openabc/forcefields/cg_model.py
-src/openabc/forcefields/hps_model.py
-src/openabc/forcefields/hps_zero_offset_model.py
-src/openabc/forcefields/moff_mrg_model.py
-src/openabc/forcefields/rigid.py
-src/openabc/forcefields/functional_terms/__init__.py
-src/openabc/forcefields/functional_terms/angle_terms.py
-src/openabc/forcefields/functional_terms/bond_terms.py
-src/openabc/forcefields/functional_terms/dihedral_terms.py
-src/openabc/forcefields/functional_terms/nonbonded_terms.py
-src/openabc/forcefields/functional_terms/zero_offset_nonbonded_terms.py
-src/openabc/forcefields/parameters/HPS_KR_parameters.csv
-src/openabc/forcefields/parameters/HPS_Urry_parameters.csv
-src/openabc/forcefields/parameters/MOFF_contact_parameters.csv
-src/openabc/forcefields/parameters/parse_hps_parameters.py
-src/openabc/forcefields/parameters/parse_moff_parameters.py
-src/openabc/forcefields/parameters/template_MOFF.top
-src/openabc/forcefields/parsers/__init__.py
-src/openabc/forcefields/parsers/hps_parser.py
-src/openabc/forcefields/parsers/moff_parser.py
-src/openabc/forcefields/parsers/mrg_parser.py
-src/openabc/utils/CA2AA.py
-src/openabc/utils/__init__.py
-src/openabc/utils/helper_functions.py
-src/openabc/utils/insert.py
-src/openabc/utils/legacy_shadow_map.py
-src/openabc/utils/replica_exchange.py
-src/openabc/utils/shadow_map.py
+openabc/__init__.py
+openabc.egg-info/PKG-INFO
+openabc.egg-info/SOURCES.txt
+openabc.egg-info/dependency_links.txt
+openabc.egg-info/top_level.txt
+openabc/forcefields/__init__.py
+openabc/forcefields/cg_model.py
+openabc/forcefields/hps_model.py
+openabc/forcefields/hps_zero_offset_model.py
+openabc/forcefields/moff_mrg_model.py
+openabc/forcefields/mpipi_model.py
+openabc/forcefields/mpipi_zero_offset_model.py
+openabc/forcefields/rigid.py
+openabc/forcefields/functional_terms/__init__.py
+openabc/forcefields/functional_terms/angle_terms.py
+openabc/forcefields/functional_terms/bond_terms.py
+openabc/forcefields/functional_terms/dihedral_terms.py
+openabc/forcefields/functional_terms/nonbonded_terms.py
+openabc/forcefields/functional_terms/zero_offset_nonbonded_terms.py
+openabc/forcefields/parameters/HPS_KR_parameters.csv
+openabc/forcefields/parameters/HPS_Urry_parameters.csv
+openabc/forcefields/parameters/MOFF_contact_parameters.csv
+openabc/forcefields/parameters/Mpipi_parameters.csv
+openabc/forcefields/parameters/lammps_Mpipi_RNA.in
+openabc/forcefields/parameters/parse_hps_parameters.py
+openabc/forcefields/parameters/parse_moff_parameters.py
+openabc/forcefields/parameters/parse_mpipi_parameters.py
+openabc/forcefields/parameters/template_MOFF.top
+openabc/forcefields/parsers/__init__.py
+openabc/forcefields/parsers/hps_parser.py
+openabc/forcefields/parsers/moff_parser.py
+openabc/forcefields/parsers/mpipi_parsers.py
+openabc/forcefields/parsers/mrg_parser.py
+openabc/lib/__init__.py
+openabc/lib/dna_lib.py
+openabc/lib/physical_constants.py
+openabc/lib/protein_lib.py
+openabc/lib/rna_lib.py
+openabc/lib/unit_conversion.py
+openabc/utils/CA2AA.py
+openabc/utils/__init__.py
+openabc/utils/helper_functions.py
+openabc/utils/insert.py
+openabc/utils/legacy_shadow_map.py
+openabc/utils/replica_exchange.py
+openabc/utils/shadow_map.py
+openabc/utils/stride.py
```

