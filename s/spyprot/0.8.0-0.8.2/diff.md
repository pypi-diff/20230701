# Comparing `tmp/spyprot-0.8.0-py3-none-any.whl.zip` & `tmp/spyprot-0.8.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 42615 bytes, number of entries: 17
+Zip file size: 42686 bytes, number of entries: 17
 -rw-rw-r--  2.0 unx     4889 b- defN 21-Oct-18 11:17 spyprot/Command.py
 -rw-rw-r--  2.0 unx     2862 b- defN 21-Oct-18 11:17 spyprot/EditPdbXyz.py
 -rw-rw-r--  2.0 unx      236 b- defN 21-Jan-27 16:33 spyprot/__init__.py
 -rw-rw-r--  2.0 unx     2226 b- defN 21-Oct-18 11:17 spyprot/cddf_parser.py
 -rw-rw-r--  2.0 unx    21726 b- defN 22-Jan-28 13:31 spyprot/cif2Wanda.py
 -rw-rw-r--  2.0 unx     2034 b- defN 21-Nov-21 13:34 spyprot/common.py
 -rw-rw-r--  2.0 unx    17949 b- defN 22-Nov-20 11:27 spyprot/fetchAnnotations.py
 -rw-rw-r--  2.0 unx    39414 b- defN 22-Nov-23 00:57 spyprot/fetchChainInfo.py
 -rw-rw-r--  2.0 unx    18701 b- defN 21-Oct-18 11:17 spyprot/fetchPDBinfo.py
 -rw-rw-r--  2.0 unx    10504 b- defN 21-Nov-19 00:47 spyprot/idMapping.py
--rw-rw-r--  2.0 unx     5788 b- defN 23-Jun-30 23:06 spyprot/ilbsm_database_downloader.py
+-rw-rw-r--  2.0 unx     5937 b- defN 23-Jul-01 07:58 spyprot/ilbsm_database_downloader.py
 -rw-rw-r--  2.0 unx    22843 b- defN 21-Oct-18 11:17 spyprot/pdb2Wanda.py
 -rw-rw-r--  2.0 unx    15115 b- defN 21-Nov-18 01:38 spyprot/spyProt.py
--rw-rw-r--  2.0 unx     1715 b- defN 23-Jun-30 23:43 spyprot-0.8.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       86 b- defN 23-Jun-30 23:43 spyprot-0.8.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-Jun-30 23:43 spyprot-0.8.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1330 b- defN 23-Jun-30 23:43 spyprot-0.8.0.dist-info/RECORD
-17 files, 167426 bytes uncompressed, 40473 bytes compressed:  75.8%
+-rw-rw-r--  2.0 unx     1715 b- defN 23-Jul-01 08:03 spyprot-0.8.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       86 b- defN 23-Jul-01 08:03 spyprot-0.8.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-Jul-01 08:03 spyprot-0.8.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1330 b- defN 23-Jul-01 08:03 spyprot-0.8.2.dist-info/RECORD
+17 files, 167575 bytes uncompressed, 40544 bytes compressed:  75.8%
```

## zipnote {}

```diff
@@ -33,20 +33,20 @@
 
 Filename: spyprot/pdb2Wanda.py
 Comment: 
 
 Filename: spyprot/spyProt.py
 Comment: 
 
-Filename: spyprot-0.8.0.dist-info/METADATA
+Filename: spyprot-0.8.2.dist-info/METADATA
 Comment: 
 
-Filename: spyprot-0.8.0.dist-info/WHEEL
+Filename: spyprot-0.8.2.dist-info/WHEEL
 Comment: 
 
-Filename: spyprot-0.8.0.dist-info/top_level.txt
+Filename: spyprot-0.8.2.dist-info/top_level.txt
 Comment: 
 
-Filename: spyprot-0.8.0.dist-info/RECORD
+Filename: spyprot-0.8.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spyprot/ilbsm_database_downloader.py

```diff
@@ -117,10 +117,13 @@
         if not file_name.find('{0}') >= 0:
             file_name = '{0}_{1}_{2}' + file_name
         directory_dir = os.path.join(self.directory, protein[0], protein[1]) if self.create_separate_dirs else self.directory
         if self.create_separate_dirs and not os.path.exists(directory_dir):
             os.makedirs(directory_dir, exist_ok=True)
         download_path = os.path.join(directory_dir, os.path.basename(file_name.format(protein[0], protein[1], protein[2])))
         link = download_url.format(protein[0], protein[1], protein[2], protein[3])
-        with urlopen(link) as image, open(download_path, 'wb') as f:
-            f.write(image.read())
+        try:
+            with urlopen(link) as image, open(download_path, 'wb') as f:
+                f.write(image.read())
+        except Exception as e:
+            logger.error(f'Error downloading file {link} or not writable: {download_path}\n{e}')
         logger.debug('Downloaded %s', link)
```

## Comparing `spyprot-0.8.0.dist-info/METADATA` & `spyprot-0.8.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyprot
-Version: 0.8.0
+Version: 0.8.2
 Summary: This package provides a set of tools for accessing protein databases and manipulating PDB/CIF files.
 Home-page: https://github.com/ilbsm/spyProt
 Author: INTERDISCIPLINARY LABORATORY of BIOLOGICAL SYSTEMS MODELLING, University of Warsaw, Warsaw, Poland
 Author-email: bmjastrzebski@gmail.com, p.rubach@cent.uw.edu.pl
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `spyprot-0.8.0.dist-info/RECORD` & `spyprot-0.8.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 spyprot/cddf_parser.py,sha256=D759I_uKAD-nixDSCz8txnnVGU9oPegE0D00vT-4cwg,2226
 spyprot/cif2Wanda.py,sha256=0-7N1vviI8Wv_yIk14RQD1QxOv2tTwyrOh2Noe51wKE,21726
 spyprot/common.py,sha256=fVC5p06aVb3_I7SdiHfY_aTyTo4pcXcj0erFae-MBTY,2034
 spyprot/fetchAnnotations.py,sha256=fkOeIHeARdlknSkS8pLKYE6N8DGURn-O5SkQNq-yVeQ,17949
 spyprot/fetchChainInfo.py,sha256=_jE7McWSt4FjB3SevjGulJTfwjBtlTFbDXcZGMLsVTQ,39414
 spyprot/fetchPDBinfo.py,sha256=id9Iujp_kA22SwhbSv64lVBAfruYHiT_kDIK62WlfDI,18701
 spyprot/idMapping.py,sha256=Dv3LoaAOHrj-g_3EPTsUOJeSvYCPaxJRB3P0xmdgErg,10504
-spyprot/ilbsm_database_downloader.py,sha256=0s0uyRUxm2PJcE8eXbbR0apNRYPEbPOroN_YaVJjJVI,5788
+spyprot/ilbsm_database_downloader.py,sha256=NyMShpkbkgHYyTcYd_xYBNXYm0cbe80CkQWBny55qb0,5937
 spyprot/pdb2Wanda.py,sha256=z76oJrWNw-uxCfiMh4oNdXidrYAl1gozL2HWRABktb4,22843
 spyprot/spyProt.py,sha256=uWTqTJ5ikZ4IJFo9Ne7eoNxWMnpjdllf1DtdqT1U8OQ,15115
-spyprot-0.8.0.dist-info/METADATA,sha256=x6CKlteEyDJLpcdoPe2IOFHy43TDEG5zDHVwtBs7mog,1715
-spyprot-0.8.0.dist-info/WHEEL,sha256=DueAsW6E8XIw2snDYANiEbP441s0xNQrJIWO3pKUKFM,86
-spyprot-0.8.0.dist-info/top_level.txt,sha256=_JSz314Is19_4IVMW8VzAtpHCueCVF2yP6Lz7aQAYug,8
-spyprot-0.8.0.dist-info/RECORD,,
+spyprot-0.8.2.dist-info/METADATA,sha256=FsEVLeLChzM3d1TAv2G5nVE0PEeToGaONry325AibZA,1715
+spyprot-0.8.2.dist-info/WHEEL,sha256=DueAsW6E8XIw2snDYANiEbP441s0xNQrJIWO3pKUKFM,86
+spyprot-0.8.2.dist-info/top_level.txt,sha256=_JSz314Is19_4IVMW8VzAtpHCueCVF2yP6Lz7aQAYug,8
+spyprot-0.8.2.dist-info/RECORD,,
```

