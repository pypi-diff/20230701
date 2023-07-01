# Comparing `tmp/ctd-python-0.1.3.tar.gz` & `tmp/ctd-python-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctd-python-0.1.3.tar", last modified: Mon Jun 26 02:00:00 2023, max compression
+gzip compressed data, was "ctd-python-0.2.0.tar", last modified: Sat Jul  1 14:28:11 2023, max compression
```

## Comparing `ctd-python-0.1.3.tar` & `ctd-python-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-26 02:00:00.430099 ctd-python-0.1.3/
--rw-r--r--   0 john       (501) staff       (20)     1509 2023-06-26 02:00:00.429691 ctd-python-0.1.3/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)      887 2023-06-26 01:02:36.000000 ctd-python-0.1.3/README.md
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-26 02:00:00.425668 ctd-python-0.1.3/ctd/
--rw-r--r--   0 john       (501) staff       (20)       31 2023-06-26 00:20:15.000000 ctd-python-0.1.3/ctd/__init__.py
--rw-r--r--   0 john       (501) staff       (20)     3333 2023-06-26 01:59:46.000000 ctd-python-0.1.3/ctd/get_data.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-26 02:00:00.426596 ctd-python-0.1.3/ctd/unzipped_data/
--rw-r--r--   0 john       (501) staff       (20)        0 2023-06-25 23:36:26.000000 ctd-python-0.1.3/ctd/unzipped_data/__init__.py
--rw-r--r--   0 john       (501) staff       (20)     1072 2023-06-26 00:49:30.000000 ctd-python-0.1.3/ctd/utils.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-06-26 02:00:00.429084 ctd-python-0.1.3/ctd_python.egg-info/
--rw-r--r--   0 john       (501) staff       (20)     1509 2023-06-26 02:00:00.000000 ctd-python-0.1.3/ctd_python.egg-info/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)      262 2023-06-26 02:00:00.000000 ctd-python-0.1.3/ctd_python.egg-info/SOURCES.txt
--rw-r--r--   0 john       (501) staff       (20)        1 2023-06-26 02:00:00.000000 ctd-python-0.1.3/ctd_python.egg-info/dependency_links.txt
--rw-r--r--   0 john       (501) staff       (20)       21 2023-06-26 02:00:00.000000 ctd-python-0.1.3/ctd_python.egg-info/requires.txt
--rw-r--r--   0 john       (501) staff       (20)        4 2023-06-26 02:00:00.000000 ctd-python-0.1.3/ctd_python.egg-info/top_level.txt
--rw-r--r--   0 john       (501) staff       (20)       38 2023-06-26 02:00:00.430351 ctd-python-0.1.3/setup.cfg
--rw-r--r--   0 john       (501) staff       (20)      544 2023-06-26 01:59:57.000000 ctd-python-0.1.3/setup.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-07-01 14:28:11.458213 ctd-python-0.2.0/
+-rw-r--r--   0 john       (501) staff       (20)     1509 2023-07-01 14:28:11.457820 ctd-python-0.2.0/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)      887 2023-06-26 01:02:36.000000 ctd-python-0.2.0/README.md
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-07-01 14:28:11.454928 ctd-python-0.2.0/ctd/
+-rw-r--r--   0 john       (501) staff       (20)       31 2023-06-26 00:20:15.000000 ctd-python-0.2.0/ctd/__init__.py
+-rw-r--r--   0 john       (501) staff       (20)     4088 2023-07-01 14:22:38.000000 ctd-python-0.2.0/ctd/get_data.py
+-rw-r--r--   0 john       (501) staff       (20)     1072 2023-06-26 00:49:30.000000 ctd-python-0.2.0/ctd/utils.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-07-01 14:28:11.457271 ctd-python-0.2.0/ctd_python.egg-info/
+-rw-r--r--   0 john       (501) staff       (20)     1509 2023-07-01 14:28:11.000000 ctd-python-0.2.0/ctd_python.egg-info/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)      232 2023-07-01 14:28:11.000000 ctd-python-0.2.0/ctd_python.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (501) staff       (20)        1 2023-07-01 14:28:11.000000 ctd-python-0.2.0/ctd_python.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (501) staff       (20)       21 2023-07-01 14:28:11.000000 ctd-python-0.2.0/ctd_python.egg-info/requires.txt
+-rw-r--r--   0 john       (501) staff       (20)        4 2023-07-01 14:28:11.000000 ctd-python-0.2.0/ctd_python.egg-info/top_level.txt
+-rw-r--r--   0 john       (501) staff       (20)       38 2023-07-01 14:28:11.458341 ctd-python-0.2.0/setup.cfg
+-rw-r--r--   0 john       (501) staff       (20)      544 2023-07-01 14:26:43.000000 ctd-python-0.2.0/setup.py
```

### Comparing `ctd-python-0.1.3/PKG-INFO` & `ctd-python-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctd-python
-Version: 0.1.3
+Version: 0.2.0
 Summary: Python interface to access data from The Comparative Toxicogenomics Database (CTD)
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## CTD Python
         
         Pyhton interface to access data from The Comparative Toxicogenomics Database (CTD)
```

### Comparing `ctd-python-0.1.3/README.md` & `ctd-python-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ctd-python-0.1.3/ctd/get_data.py` & `ctd-python-0.2.0/ctd/get_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import requests
 from tqdm import tqdm
 import pandas as pd
 
 PACKAGE_DIR = os.path.dirname(__file__)
 RAW_DATA_DIR = os.path.join(PACKAGE_DIR, 'unzipped_data')
 
+from pprint import pprint
 
 def download_resource(resource: str) -> str:
     url_dl_pattern = 'http://ctdbase.org/reports/{resource}.csv.gz'
     url = url_dl_pattern.format(resource=resource)
 
     logging.info('[download_resource]: downloading: %s', resource)
     local_filename = os.path.join(RAW_DATA_DIR, f"{resource}.csv")
@@ -67,38 +68,53 @@
         - Exposure Studies
         - Chemicals
         - Genes
         - ChemicalGeneInteractions
         - ChemicalDiseaseInteractions
         - Diseases
     """
+
     RESOURCES = {
-        'GeneInteractionTypes': 'CTD_chem_gene_ixn_types',
-        'ChemicalPathwaysEnriched': 'CTD_chem_pathways_enriched',
-        'GeneDisease': 'CTD_genes_diseases',
-        'GenePathways': 'CTD_genes_pathways',
-        'DiseasePathways': 'CTD_diseases_pathways',
-        'ChemocalPhenoTypeInteractions': 'CTD_pheno_term_ixns',
-        'Exposure Studies': 'CTD_exposure_studies',
-        'Chemicals': 'CTD_chemicals',
-        'Genes': 'CTD_genes',
-        'ChemicalGeneInteractions': 'CTD_chem_gene_ixns',
-        'ChemicalDiseaseInteractions': 'CTD_chemicals_diseases',
-        'Diseases': 'CTD_diseases'
+        'GeneInteractionTypes': {'filename': 'CTD_chem_gene_ixn_types'},
+        'ChemicalPathwaysEnriched': {'filename': 'CTD_chem_pathways_enriched'},
+        'GeneDisease': {'filename': 'CTD_genes_diseases'},
+        'GenePathways': {'filename': 'CTD_genes_pathways'},
+        'DiseasePathways': {'filename': 'CTD_diseases_pathways'},
+        'ChemocalPhenoTypeInteractions': {'filename': 'CTD_pheno_term_ixns'},
+        'Exposure Studies': {'filename': 'CTD_exposure_studies'},
+        'Chemicals': {'filename': 'CTD_chemicals'},
+        'Genes': {'filename': 'CTD_genes'},
+        'ChemicalGeneInteractions': {'filename': 'CTD_chem_gene_ixns'},
+        'ChemicalDiseaseInteractions': {'filename': 'CTD_chemicals_diseases', 'dtypes': {'ChemicalName': str,'ChemicalID': str,'CasRN': str,'DiseaseName': str,'DiseaseID': str,'DirectEvidence': str,'InferenceGeneSymbol': str,'InferenceScore': float,'OmimIDs': str,'PubMedIDs': str}},
+        'Diseases': {'filename': 'CTD_chem_gene_ixn_types'}
     }
 
-    resource_name = RESOURCES.get(resource)
-    if not resource_name:
+    resource_obj = RESOURCES.get(resource)
+
+    filename = resource_obj.get('filename')
+    dtypes = resource_obj.get('dtypes')
+
+    if not resource_obj:
         raise Exception(f"The resource '{resource}' is not available. Please check https://ctdbase.org/downloads/ for available resources.")
 
-    download_resource(resource_name)
+    download_resource(filename)
 
-    line_number = 27  # files have the same header, TODO need to make dynamic
-    the_file = os.path.join(RAW_DATA_DIR, f"{resource_name}.csv")
+    fields_line = '# Fields:'
+    header_line = '#'
+    the_file = os.path.join(RAW_DATA_DIR, f"{filename}.csv")
 
+    fields_line_number = None
     with open(the_file, 'r') as reader:
         for i, row in enumerate(reader):
-            if i == line_number:
-                header = row.replace("# ", "").split(",")
+            if 'Fields:' in row:
+                fields_line_number = i + 1
+            elif i == fields_line_number:
+                fields_line = row.strip("# ").strip()
+                fields = [field.strip() for field in fields_line.split(",")]
+
+    df = pd.read_csv(the_file, skiprows=fields_line_number + 1, names=fields, dtype=dtypes)
 
-    df = pd.read_csv(the_file, skiprows=29, names=header)
     return df
+
+
+if __name__ == '__main__':
+    get_data('ChemicalDiseaseInteractions')
```

### Comparing `ctd-python-0.1.3/ctd/utils.py` & `ctd-python-0.2.0/ctd/utils.py`

 * *Files identical despite different names*

### Comparing `ctd-python-0.1.3/ctd_python.egg-info/PKG-INFO` & `ctd-python-0.2.0/ctd_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctd-python
-Version: 0.1.3
+Version: 0.2.0
 Summary: Python interface to access data from The Comparative Toxicogenomics Database (CTD)
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## CTD Python
         
         Pyhton interface to access data from The Comparative Toxicogenomics Database (CTD)
```

### Comparing `ctd-python-0.1.3/setup.py` & `ctd-python-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='ctd-python',
-    version='0.1.3',
+    version='0.2.0',
     description='Python interface to access data from The Comparative Toxicogenomics Database (CTD)',
     packages=['ctd'],
     install_requires=[
         'requests',
         'pandas',
         'tqdm'
     ],
```

