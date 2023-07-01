# Comparing `tmp/ctd-python-0.2.0.tar.gz` & `tmp/ctd-python-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctd-python-0.2.0.tar", last modified: Sat Jul  1 14:28:11 2023, max compression
+gzip compressed data, was "ctd-python-0.2.1.tar", last modified: Sat Jul  1 14:39:58 2023, max compression
```

## Comparing `ctd-python-0.2.0.tar` & `ctd-python-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-07-01 14:28:11.458213 ctd-python-0.2.0/
--rw-r--r--   0 john       (501) staff       (20)     1509 2023-07-01 14:28:11.457820 ctd-python-0.2.0/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)      887 2023-06-26 01:02:36.000000 ctd-python-0.2.0/README.md
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-07-01 14:28:11.454928 ctd-python-0.2.0/ctd/
--rw-r--r--   0 john       (501) staff       (20)       31 2023-06-26 00:20:15.000000 ctd-python-0.2.0/ctd/__init__.py
--rw-r--r--   0 john       (501) staff       (20)     4088 2023-07-01 14:22:38.000000 ctd-python-0.2.0/ctd/get_data.py
--rw-r--r--   0 john       (501) staff       (20)     1072 2023-06-26 00:49:30.000000 ctd-python-0.2.0/ctd/utils.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-07-01 14:28:11.457271 ctd-python-0.2.0/ctd_python.egg-info/
--rw-r--r--   0 john       (501) staff       (20)     1509 2023-07-01 14:28:11.000000 ctd-python-0.2.0/ctd_python.egg-info/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)      232 2023-07-01 14:28:11.000000 ctd-python-0.2.0/ctd_python.egg-info/SOURCES.txt
--rw-r--r--   0 john       (501) staff       (20)        1 2023-07-01 14:28:11.000000 ctd-python-0.2.0/ctd_python.egg-info/dependency_links.txt
--rw-r--r--   0 john       (501) staff       (20)       21 2023-07-01 14:28:11.000000 ctd-python-0.2.0/ctd_python.egg-info/requires.txt
--rw-r--r--   0 john       (501) staff       (20)        4 2023-07-01 14:28:11.000000 ctd-python-0.2.0/ctd_python.egg-info/top_level.txt
--rw-r--r--   0 john       (501) staff       (20)       38 2023-07-01 14:28:11.458341 ctd-python-0.2.0/setup.cfg
--rw-r--r--   0 john       (501) staff       (20)      544 2023-07-01 14:26:43.000000 ctd-python-0.2.0/setup.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-07-01 14:39:58.689334 ctd-python-0.2.1/
+-rw-r--r--   0 john       (501) staff       (20)     1509 2023-07-01 14:39:58.688768 ctd-python-0.2.1/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)      887 2023-06-26 01:02:36.000000 ctd-python-0.2.1/README.md
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-07-01 14:39:58.685043 ctd-python-0.2.1/ctd/
+-rw-r--r--   0 john       (501) staff       (20)       31 2023-06-26 00:20:15.000000 ctd-python-0.2.1/ctd/__init__.py
+-rw-r--r--   0 john       (501) staff       (20)     4058 2023-07-01 14:39:43.000000 ctd-python-0.2.1/ctd/get_data.py
+-rw-r--r--   0 john       (501) staff       (20)     1072 2023-06-26 00:49:30.000000 ctd-python-0.2.1/ctd/utils.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-07-01 14:39:58.688144 ctd-python-0.2.1/ctd_python.egg-info/
+-rw-r--r--   0 john       (501) staff       (20)     1509 2023-07-01 14:39:58.000000 ctd-python-0.2.1/ctd_python.egg-info/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)      232 2023-07-01 14:39:58.000000 ctd-python-0.2.1/ctd_python.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (501) staff       (20)        1 2023-07-01 14:39:58.000000 ctd-python-0.2.1/ctd_python.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (501) staff       (20)       21 2023-07-01 14:39:58.000000 ctd-python-0.2.1/ctd_python.egg-info/requires.txt
+-rw-r--r--   0 john       (501) staff       (20)        4 2023-07-01 14:39:58.000000 ctd-python-0.2.1/ctd_python.egg-info/top_level.txt
+-rw-r--r--   0 john       (501) staff       (20)       38 2023-07-01 14:39:58.689472 ctd-python-0.2.1/setup.cfg
+-rw-r--r--   0 john       (501) staff       (20)      544 2023-07-01 14:39:51.000000 ctd-python-0.2.1/setup.py
```

### Comparing `ctd-python-0.2.0/PKG-INFO` & `ctd-python-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctd-python
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python interface to access data from The Comparative Toxicogenomics Database (CTD)
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## CTD Python
         
         Pyhton interface to access data from The Comparative Toxicogenomics Database (CTD)
```

### Comparing `ctd-python-0.2.0/README.md` & `ctd-python-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ctd-python-0.2.0/ctd/get_data.py` & `ctd-python-0.2.1/ctd/get_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         'DiseasePathways': {'filename': 'CTD_diseases_pathways'},
         'ChemocalPhenoTypeInteractions': {'filename': 'CTD_pheno_term_ixns'},
         'Exposure Studies': {'filename': 'CTD_exposure_studies'},
         'Chemicals': {'filename': 'CTD_chemicals'},
         'Genes': {'filename': 'CTD_genes'},
         'ChemicalGeneInteractions': {'filename': 'CTD_chem_gene_ixns'},
         'ChemicalDiseaseInteractions': {'filename': 'CTD_chemicals_diseases', 'dtypes': {'ChemicalName': str,'ChemicalID': str,'CasRN': str,'DiseaseName': str,'DiseaseID': str,'DirectEvidence': str,'InferenceGeneSymbol': str,'InferenceScore': float,'OmimIDs': str,'PubMedIDs': str}},
-        'Diseases': {'filename': 'CTD_chem_gene_ixn_types'}
+        'Diseases': {'filename': 'CTD_diseases'}
     }
 
     resource_obj = RESOURCES.get(resource)
 
     filename = resource_obj.get('filename')
     dtypes = resource_obj.get('dtypes')
 
@@ -113,8 +113,8 @@
 
     df = pd.read_csv(the_file, skiprows=fields_line_number + 1, names=fields, dtype=dtypes)
 
     return df
 
 
 if __name__ == '__main__':
-    get_data('ChemicalDiseaseInteractions')
+    get_data('Diseases')
```

### Comparing `ctd-python-0.2.0/ctd/utils.py` & `ctd-python-0.2.1/ctd/utils.py`

 * *Files identical despite different names*

### Comparing `ctd-python-0.2.0/ctd_python.egg-info/PKG-INFO` & `ctd-python-0.2.1/ctd_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctd-python
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python interface to access data from The Comparative Toxicogenomics Database (CTD)
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ## CTD Python
         
         Pyhton interface to access data from The Comparative Toxicogenomics Database (CTD)
```

### Comparing `ctd-python-0.2.0/setup.py` & `ctd-python-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='ctd-python',
-    version='0.2.0',
+    version='0.2.1',
     description='Python interface to access data from The Comparative Toxicogenomics Database (CTD)',
     packages=['ctd'],
     install_requires=[
         'requests',
         'pandas',
         'tqdm'
     ],
```

