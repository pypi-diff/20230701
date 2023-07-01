# Comparing `tmp/pywhu3d-0.2.4-py3-none-any.whl.zip` & `tmp/pywhu3d-0.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 35234 bytes, number of entries: 19
+Zip file size: 35241 bytes, number of entries: 19
 -rw-r--r--  2.0 unx        0 b- defN 22-Oct-30 14:16 pywhu3d/__init__.py
 -rw-r--r--  2.0 unx    12694 b- defN 23-May-22 06:22 pywhu3d/evaluation.py
--rw-r--r--  2.0 unx    25890 b- defN 23-Jul-01 10:44 pywhu3d/tool.py
+-rw-r--r--  2.0 unx    25900 b- defN 23-Jul-01 10:49 pywhu3d/tool.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Oct-30 14:17 pywhu3d/configs/__init__.py
 -rw-r--r--  2.0 unx     5172 b- defN 22-Dec-03 05:50 pywhu3d/configs/als_config.py
 -rw-r--r--  2.0 unx     2285 b- defN 22-Jan-25 02:28 pywhu3d/configs/base_config.py
 -rw-r--r--  2.0 unx    11576 b- defN 22-Nov-05 11:35 pywhu3d/configs/mls_config.py
 -rw-r--r--  2.0 unx    13768 b- defN 22-Nov-19 08:32 pywhu3d/configs/mls_config_pole.py
--rw-r--r--  2.0 unx    11037 b- defN 23-Jul-01 10:32 pywhu3d/configs/mls_w_config.py
+-rw-r--r--  2.0 unx    11046 b- defN 23-Jul-01 10:57 pywhu3d/configs/mls_w_config.py
 -rw-r--r--  2.0 unx     7411 b- defN 22-Nov-05 11:35 pywhu3d/configs/paris_config.py
 -rw-r--r--  2.0 unx     4395 b- defN 22-Nov-05 11:35 pywhu3d/configs/s3dis_config.py
 -rw-r--r--  2.0 unx     4283 b- defN 20-Dec-31 16:00 pywhu3d/configs/scannet_config.py
 -rw-r--r--  2.0 unx     4740 b- defN 22-Nov-05 11:35 pywhu3d/configs/toronto_config.py
 -rw-r--r--  2.0 unx      186 b- defN 21-Jan-23 10:04 pywhu3d/configs/wrap_configs.py
--rw-r--r--  2.0 unx     1076 b- defN 23-Jul-01 10:48 pywhu3d-0.2.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     1199 b- defN 23-Jul-01 10:48 pywhu3d-0.2.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-01 10:48 pywhu3d-0.2.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-01 10:48 pywhu3d-0.2.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1575 b- defN 23-Jul-01 10:48 pywhu3d-0.2.4.dist-info/RECORD
-19 files, 107387 bytes uncompressed, 32662 bytes compressed:  69.6%
+-rw-r--r--  2.0 unx     1076 b- defN 23-Jul-01 10:57 pywhu3d-0.2.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1199 b- defN 23-Jul-01 10:57 pywhu3d-0.2.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-01 10:57 pywhu3d-0.2.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-01 10:57 pywhu3d-0.2.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1575 b- defN 23-Jul-01 10:57 pywhu3d-0.2.5.dist-info/RECORD
+19 files, 107406 bytes uncompressed, 32669 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: pywhu3d/configs/toronto_config.py
 Comment: 
 
 Filename: pywhu3d/configs/wrap_configs.py
 Comment: 
 
-Filename: pywhu3d-0.2.4.dist-info/LICENSE
+Filename: pywhu3d-0.2.5.dist-info/LICENSE
 Comment: 
 
-Filename: pywhu3d-0.2.4.dist-info/METADATA
+Filename: pywhu3d-0.2.5.dist-info/METADATA
 Comment: 
 
-Filename: pywhu3d-0.2.4.dist-info/WHEEL
+Filename: pywhu3d-0.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: pywhu3d-0.2.4.dist-info/top_level.txt
+Filename: pywhu3d-0.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: pywhu3d-0.2.4.dist-info/RECORD
+Filename: pywhu3d-0.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pywhu3d/tool.py

```diff
@@ -638,15 +638,15 @@
         # self.compute_normals()
         whu3d.interprete_labels()
         whu3d.compute_normals(radius=0.8)
         whu3d.save_divided_blocks(out_dir='', num_points=600000, size=(20, 20), stride=10, threshold=100,
                                   show_points=False)
 
 if __name__ == '__main__':
-    data_root = '/Users/hanxu/data/whu'
+    data_root = '/Users/hanxu/data/whu3d-dataset'
     # scenes = ['0404', '0940']
     whu3d = WHU3D(data_root=data_root, data_type='mls', format='txt')
     # whu3d.vis('0404', 'pc')
     whu3d.export_h5()
     whu3d.get_label_map()
     attr = whu3d.get_data_attribute('coords')
     whu3d.list_attributes()
```

## pywhu3d/configs/mls_w_config.py

```diff
@@ -142,14 +142,15 @@
     'detector': 15,  # '独立探头',
     'fence': 16,  # '围墙/栅栏',
     'wire': 17,  # '电线',
     'pole': 18
 } # 23
 
 sem_map = {
+    0:0,
     1:1,
     2:2,
     3:3,
     4:4,
     5:5,
     6:6,
     7:7,
```

## Comparing `pywhu3d-0.2.4.dist-info/LICENSE` & `pywhu3d-0.2.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pywhu3d-0.2.4.dist-info/METADATA` & `pywhu3d-0.2.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywhu3d
-Version: 0.2.4
+Version: 0.2.5
 Summary: Example pywhu3d tool Package
 Home-page: https://github.com/astroy
 Author: Xu Han
 Author-email: hanxu@glad3d.com
 Keywords: whu3d,dataset,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

## Comparing `pywhu3d-0.2.4.dist-info/RECORD` & `pywhu3d-0.2.5.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 pywhu3d/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pywhu3d/evaluation.py,sha256=YKLLYbuzpD6lQkJMB_91rXio9iw97ssXY307U9HgeI4,12694
-pywhu3d/tool.py,sha256=vIKulpV_-djx7LXxgYx7QYYprGGP-PNIz8VP9rvMBkI,25890
+pywhu3d/tool.py,sha256=YNVcKnG1HUGpeATz8ISI3KzfVWX1lcGEdP2WEgirzNY,25900
 pywhu3d/configs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pywhu3d/configs/als_config.py,sha256=rA-T6OyyM085K8p7T_-iejYr3Xj7qEebI0YwleBiFXc,5172
 pywhu3d/configs/base_config.py,sha256=6UCAS9UCipC_h6quwik6KulWZkp2KxkTYbApRCrRiGQ,2285
 pywhu3d/configs/mls_config.py,sha256=StVuLEMN9gRyywnhMD7JpHBVCNN47PNf2swkRxegEOw,11576
 pywhu3d/configs/mls_config_pole.py,sha256=aTtouZrropJ_fbhUNcWjzdc-pTWV3fVeGE3IZ4_fldU,13768
-pywhu3d/configs/mls_w_config.py,sha256=4hXVha8TVHj34Ulc7yluynUFEvTMNJHEhx4_zif_f2w,11037
+pywhu3d/configs/mls_w_config.py,sha256=ejIgD4K9zlGc1-Nussr9qETLQkpqADUCqXcGz9S-yic,11046
 pywhu3d/configs/paris_config.py,sha256=JrBFXzUkLLMT20bRLlLIUqooXFWftu_qwa5avvG083Q,7411
 pywhu3d/configs/s3dis_config.py,sha256=bB8-j0um70lPLv03PeZvw-LkjKYLOc0bvzYVozsdFyw,4395
 pywhu3d/configs/scannet_config.py,sha256=dJjkjiP1l3VEWQ1Uluwd7lum_3LMvFt0l7TPz1NydgI,4283
 pywhu3d/configs/toronto_config.py,sha256=SxYgYKJ6bf7zaNlmszNdpwTy7126kCW9HsEwWT0xeXI,4740
 pywhu3d/configs/wrap_configs.py,sha256=9Lezbp6IStVpvS2BJiNm_qQ-9e9gyXT5TN-h_L4UbJg,186
-pywhu3d-0.2.4.dist-info/LICENSE,sha256=jAt62vPGMrWssYEKav2xAaDp8wjtKQScCguopKunN8Q,1076
-pywhu3d-0.2.4.dist-info/METADATA,sha256=Mcf4ptbqf_3S5eP9DgXOCNmkYtOVvlld_pReYpIMYKU,1199
-pywhu3d-0.2.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pywhu3d-0.2.4.dist-info/top_level.txt,sha256=XacQWDtHJRY_akQP8PPiX56iNHQ_epUiFTGekh1FP7g,8
-pywhu3d-0.2.4.dist-info/RECORD,,
+pywhu3d-0.2.5.dist-info/LICENSE,sha256=jAt62vPGMrWssYEKav2xAaDp8wjtKQScCguopKunN8Q,1076
+pywhu3d-0.2.5.dist-info/METADATA,sha256=vW_2bPu0xHEC9GYGmHe8s-ZU-VmhcGa69DZE8BUVrOs,1199
+pywhu3d-0.2.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pywhu3d-0.2.5.dist-info/top_level.txt,sha256=XacQWDtHJRY_akQP8PPiX56iNHQ_epUiFTGekh1FP7g,8
+pywhu3d-0.2.5.dist-info/RECORD,,
```

