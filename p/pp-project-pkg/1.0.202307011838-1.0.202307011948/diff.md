# Comparing `tmp/pp_project_pkg-1.0.202307011838-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202307011948-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 12417 bytes, number of entries: 19
+Zip file size: 12634 bytes, number of entries: 19
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 22:23 mlflow_pipelines/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 22:23 mlflow_pipelines/fetch_data/__init__.py
 -rw-rw-r--  2.0 unx      887 b- defN 23-Jun-27 22:23 mlflow_pipelines/fetch_data/get_data.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 22:23 mlflow_pipelines/train_model/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 22:23 mlflow_pipelines/train_model/model_train.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 22:23 mlflow_pipelines/upload_data/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 22:23 mlflow_pipelines/upload_data/data_upload.py
 -rw-rw-r--  2.0 unx       71 b- defN 23-Jun-07 11:24 pp_project_pkg/__init__.py
 -rw-rw-r--  2.0 unx     5335 b- defN 23-Jun-23 12:39 pp_project_pkg/linear_train.py
 -rw-rw-r--  2.0 unx      577 b- defN 23-Jun-07 11:24 pp_project_pkg/newsvendor.py
 -rw-rw-r--  2.0 unx     9252 b- defN 23-Jun-27 22:23 pp_project_pkg/pp_tables.py
--rw-rw-r--  2.0 unx     6657 b- defN 23-Jun-23 12:39 pp_project_pkg/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jul-01 18:38 pp_project_pkg/version.py
--rw-rw-r--  2.0 unx     5164 b- defN 23-Jun-27 22:23 pp_project_pkg/wrangling.py
--rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-07 11:24 pp_project_pkg-1.0.202307011838.data/scripts/pp_project_run.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jul-01 18:39 pp_project_pkg-1.0.202307011838.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-01 18:39 pp_project_pkg-1.0.202307011838.dist-info/WHEEL
--rw-rw-r--  2.0 unx       32 b- defN 23-Jul-01 18:39 pp_project_pkg-1.0.202307011838.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1721 b- defN 23-Jul-01 18:39 pp_project_pkg-1.0.202307011838.dist-info/RECORD
-19 files, 31691 bytes uncompressed, 9511 bytes compressed:  70.0%
+-rw-rw-r--  2.0 unx     7448 b- defN 23-Jul-01 19:37 pp_project_pkg/utils.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jul-01 19:48 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx     5395 b- defN 23-Jul-01 19:48 pp_project_pkg/wrangling.py
+-rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-07 11:24 pp_project_pkg-1.0.202307011948.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jul-01 19:49 pp_project_pkg-1.0.202307011948.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-01 19:49 pp_project_pkg-1.0.202307011948.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       32 b- defN 23-Jul-01 19:49 pp_project_pkg-1.0.202307011948.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1721 b- defN 23-Jul-01 19:49 pp_project_pkg-1.0.202307011948.dist-info/RECORD
+19 files, 32713 bytes uncompressed, 9728 bytes compressed:  70.3%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307011838.data/scripts/pp_project_run.py
+Filename: pp_project_pkg-1.0.202307011948.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307011838.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202307011948.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307011838.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202307011948.dist-info/WHEEL
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307011838.dist-info/top_level.txt
+Filename: pp_project_pkg-1.0.202307011948.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307011838.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202307011948.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pp_project_pkg/utils.py

```diff
@@ -1,15 +1,15 @@
 import wml.visionml as wv
 import datetime
 import mb.pandas as pd
 from .pp_tables import queries
 from .wrangling import wrangling_data
 
 __all__ = ['site_date_res','check_if_valid_date','check_report_close_date','create_date_table',
-           'download_upload_dates_report','compare_report_dates','upload_waste_data','get_drivers_data']
+           'download_upload_dates_report','compare_report_dates','upload_waste_data','get_drivers_data','upload_drivers_data']
 
 
 def site_date_res(site_id= 30607):
     """
     Get the site date report closure data
     Args:
         site_id : Site id for fetching the date wise result. Site_id : 30607 (Waldof Astoria)
@@ -142,14 +142,19 @@
         if logger:
             logger.info("Uploading date : {}".format(date_str))
         a = queries(date=date_str)
         queries_res = a.run_all()
         queries_date = a.date
         res= wrangling_data(queries_res,date=queries_date)
         res.to_sql(name='waldorf_waste_data',con=wv.ml_engine,schema='pp_tables' ,if_exists='append',index=False)
+        
+        #uploading drivers data
+        res_driver = get_drivers_data(date=date_str)
+        res_driver.to_sql(name='waldorf_drivers_data',con=wv.ml_engine,schema='pp_tables' ,if_exists='append',index=False)
+
         if logger:
             logger.info("Uploaded date : {}".format(date_str))
     if logger:
         logger.info("Uploaded records total : {}".format(len(dates)))
     
 def get_drivers_data(site_id= 30607, date='2023-06-06' ,logger=None):
     """ 
@@ -178,8 +183,24 @@
     where vd.view_service_id  = vs.id 
     and vmpc.view_service_id = vs.id
     and vcs.id  = vs.view_current_state_id
     and vcs.site_id = {}
     and date(vs.start_date) = '{}'
     order by vs.start_date desc """.format(site_id,date)
         
-    return wv.read_sql(q1,wv.ml_engine)
+    return wv.read_sql(q1,wv.ml_engine)
+
+def upload_drivers_data(data,logger=None):
+    """
+    Function to upload the drivers data to the database
+    Args:
+        data : data to be uploaded
+    Returns:
+        None
+    """
+    #columns = ['start_date','site_id','meal_period','driver_type','label','value']
+    assert len(data.columns) == 6, "Dataframe should have 6 columns"
+    
+    data.to_sql(name='waldorf_drivers_data',con=wv.ml_engine,schema='pp_tables' ,if_exists='append',index=False)
+    if logger:
+        logger.info("Uploaded records total : {}".format(len(data)))
+
```

## pp_project_pkg/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('07')
 VERSION_DAY = int('01')
-VERSION_HOUR = int('18')
-VERSION_MINUTE = int('38')
+VERSION_HOUR = int('19')
+VERSION_MINUTE = int('48')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202307011838
-version_date = '2023/07/01 18:38'
+PATCH_VERSION = 202307011948
+version_date = '2023/07/01 19:48'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## pp_project_pkg/wrangling.py

```diff
@@ -55,35 +55,40 @@
      
     if logger and site_data:
         logger.info('Site info {} : {}'.format(site_data['site_id'],site_info['tracker_name'].values[0]))
         logger.info('Cover count for the date {} : {}'.format(site_data['date'],cover_count))
         logger.info('pp_production_rework total : {}'.format(pp_production_rework['rework'].sum()))
 
     # Filter the filtered dataframe based on the 'local_time' column
-    itemised_overproduction = filtered_df.loc[(filtered_df['local_time'].dt.time >= meal_period_start_dt.time()) & (filtered_df['local_time'].dt.time <= meal_period_end_dt.time())]
-    itemised_overproduction = itemised_overproduction[list(waste_data_for_site.columns)]
+    try:     
+        itemised_overproduction = filtered_df.loc[(filtered_df['local_time'].dt.time >= meal_period_start_dt.time()) & (filtered_df['local_time'].dt.time <= meal_period_end_dt.time())]
+        itemised_overproduction = itemised_overproduction[list(waste_data_for_site.columns)]
+    except:
+        print("Error in filtering the dataframe")
+        print("filtered_df : {}".format(filtered_df.head()))
+        print("filetered_df['local_time'] : {}'.format(filtered_df['local_time'])")
 
     joined_df = food_items.join(itemised_overproduction.set_index('item_id'), on='waste_identifier', how='left',rsuffix='_2')
 
     # Group the joined dataframe by 'food_item_id' and calculate the sum of 'weight_g' column while replacing null values with 0
     grouped_df = joined_df.groupby('food_item_id')['weight_g'].sum().fillna(0)
 
     # Convert the resulting series object to a dataframe
     overproduction = pd.DataFrame(grouped_df).reset_index().rename(columns={'weight_g': 'quantity_g'})
 
     joined_df = pd.merge(food_items, overproduction, how='left', on='food_item_id').fillna(0)
 
     # Join the resulting dataframe with 'actual_production_and_rework' dataframe on 'taxonomy_code' column and replace null values with 0
     joined_df2 = pd.merge(joined_df, actual_production_and_rework, how='left', on='taxonomy_code').fillna(0)
 
-    print(joined_df2.columns)
+    #print(joined_df2.columns)
     # Select the required columns from the resulting dataframe
     result_df = joined_df2[[ 'name_x', 'taxonomy_code', 'quantity_g_y', 'rework_g', 'quantity_g_x']]
 
-    print(result_df.columns)
+    #print(result_df.columns)
     # Rename the columns to match the column names in the SQL query
     meal_service_summary = result_df.rename(columns={'name_x': 'name','quantity_g_y': 'actual_production', 'rework_g': 'rework_or_reuse', 'quantity_g_x': 'waste'})
 
     meal_service_summary_df = meal_service_summary.copy()
 
     # Calculate the new columns as required
     meal_service_summary_df['covers'] = cover_count
```

## Comparing `pp_project_pkg-1.0.202307011838.data/scripts/pp_project_run.py` & `pp_project_pkg-1.0.202307011948.data/scripts/pp_project_run.py`

 * *Files identical despite different names*

## Comparing `pp_project_pkg-1.0.202307011838.dist-info/RECORD` & `pp_project_pkg-1.0.202307011948.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 mlflow_pipelines/train_model/model_train.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_pipelines/upload_data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_pipelines/upload_data/data_upload.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pp_project_pkg/__init__.py,sha256=9idX2X6SQKZg--ziGy6Ii9OB-kz9hOX1nEG9a0xEW9g,71
 pp_project_pkg/linear_train.py,sha256=xW9v6KON3cAC3-4yP50rC6VCwv0tCeJ6h25oILWyGRw,5335
 pp_project_pkg/newsvendor.py,sha256=E6JHp0Vtmq63toKM6bO3xTAdCgwmAZzRua-w10wrc5Y,577
 pp_project_pkg/pp_tables.py,sha256=aNBP-aExfiPWTINChNLIzIIgTUrVo-z26Oq8cLTky2w,9252
-pp_project_pkg/utils.py,sha256=qWUhyGz6Vz_0SOF_SvQbRlr2qxEIl2kqjvE32pZSipw,6657
-pp_project_pkg/version.py,sha256=SWgo7sAvKrqYItUOx42FF4pvA6lRvH_qNKHejY2fTm8,396
-pp_project_pkg/wrangling.py,sha256=yhSUk82kjfgbEDRpHj-eqf2IfXuvTYRu_l2jWKKtw5U,5164
-pp_project_pkg-1.0.202307011838.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
-pp_project_pkg-1.0.202307011838.dist-info/METADATA,sha256=VO_7LtSc1DSDqj6A0tsX1FUAJIe0TOypMa_QFIDjEc0,191
-pp_project_pkg-1.0.202307011838.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-pp_project_pkg-1.0.202307011838.dist-info/top_level.txt,sha256=aTmpGcM2s0GVN0z4bWc23t0I3mXhHxeqKNzUWghwIRA,32
-pp_project_pkg-1.0.202307011838.dist-info/RECORD,,
+pp_project_pkg/utils.py,sha256=KmLqDW3F66lo5e4oQFNCMrUZGVtFkHbqgxjyODeeVY8,7448
+pp_project_pkg/version.py,sha256=Zoflwovbuc01qfrfW2ScJex2Oj8aK_Bg--glhIxpiTc,396
+pp_project_pkg/wrangling.py,sha256=nbwQXo6AJ1HQ-bbMXBEdYYMSJvfL3RwU9yQCPYSxV-E,5395
+pp_project_pkg-1.0.202307011948.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
+pp_project_pkg-1.0.202307011948.dist-info/METADATA,sha256=-pQ_bc0F_Mm2UxyWeZU1qZDurG_EpaSyzJP1Ot3Cdo4,191
+pp_project_pkg-1.0.202307011948.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+pp_project_pkg-1.0.202307011948.dist-info/top_level.txt,sha256=aTmpGcM2s0GVN0z4bWc23t0I3mXhHxeqKNzUWghwIRA,32
+pp_project_pkg-1.0.202307011948.dist-info/RECORD,,
```

