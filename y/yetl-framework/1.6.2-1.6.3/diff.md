# Comparing `tmp/yetl-framework-1.6.2.tar.gz` & `tmp/yetl-framework-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-1.6.2.tar", last modified: Sat Jul  1 17:43:18 2023, max compression
+gzip compressed data, was "yetl-framework-1.6.3.tar", last modified: Sat Jul  1 19:44:59 2023, max compression
```

## Comparing `yetl-framework-1.6.2.tar` & `yetl-framework-1.6.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 17:43:18.906231 yetl-framework-1.6.2/
--rw-r--r--   0 vsts      (1001) docker     (123)     1093 2023-07-01 17:43:18.906231 yetl-framework-1.6.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      596 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-01 17:43:18.906231 yetl-framework-1.6.2/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1217 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 17:43:18.902231 yetl-framework-1.6.2/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1141 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/yetl/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 17:43:18.902231 yetl-framework-1.6.2/yetl/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)     2845 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/yetl/cli/_init.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 17:43:18.902231 yetl-framework-1.6.2/yetl/cli/metadata_provider/
--rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/yetl/cli/metadata_provider/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16286 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/yetl/cli/metadata_provider/_xlsx.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 17:43:18.902231 yetl-framework-1.6.2/yetl/config/
--rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/yetl/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3284 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/yetl/config/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2195 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/yetl/config/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/yetl/config/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/yetl/config/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1309 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/yetl/config/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/yetl/config/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/yetl/config/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10103 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/yetl/config/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/yetl/config/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5064 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/yetl/config/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17636 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/yetl/config/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 17:43:18.902231 yetl-framework-1.6.2/yetl/config/table/
--rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/yetl/config/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4693 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/yetl/config/table/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/yetl/config/table/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6541 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/yetl/config/table/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4662 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/yetl/config/table/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/yetl/config/table/_table_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/yetl/config/table/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 17:43:18.906231 yetl-framework-1.6.2/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      167 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1312 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/yetl/workflow/_dlt.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-07-01 17:42:21.000000 yetl-framework-1.6.2/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 17:43:18.906231 yetl-framework-1.6.2/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     1093 2023-07-01 17:43:18.000000 yetl-framework-1.6.2/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      999 2023-07-01 17:43:18.000000 yetl-framework-1.6.2/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-01 17:43:18.000000 yetl-framework-1.6.2/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-01 17:43:18.000000 yetl-framework-1.6.2/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       57 2023-07-01 17:43:18.000000 yetl-framework-1.6.2/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-07-01 17:43:18.000000 yetl-framework-1.6.2/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 19:44:59.919225 yetl-framework-1.6.3/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1093 2023-07-01 19:44:59.919225 yetl-framework-1.6.3/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      596 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-01 19:44:59.919225 yetl-framework-1.6.3/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1217 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 19:44:59.911225 yetl-framework-1.6.3/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1141 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/yetl/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 19:44:59.911225 yetl-framework-1.6.3/yetl/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2845 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/yetl/cli/_init.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 19:44:59.911225 yetl-framework-1.6.3/yetl/cli/metadata_provider/
+-rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/yetl/cli/metadata_provider/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16286 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/yetl/cli/metadata_provider/_xlsx.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 19:44:59.915225 yetl-framework-1.6.3/yetl/config/
+-rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/yetl/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3284 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/yetl/config/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2195 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/yetl/config/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/yetl/config/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/yetl/config/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1309 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/yetl/config/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/yetl/config/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/yetl/config/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10027 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/yetl/config/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/yetl/config/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5064 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/yetl/config/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17636 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/yetl/config/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 19:44:59.915225 yetl-framework-1.6.3/yetl/config/table/
+-rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/yetl/config/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4741 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/yetl/config/table/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/yetl/config/table/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6541 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/yetl/config/table/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4662 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/yetl/config/table/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/yetl/config/table/_table_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/yetl/config/table/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 19:44:59.915225 yetl-framework-1.6.3/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      167 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1312 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/yetl/workflow/_dlt.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-07-01 19:43:59.000000 yetl-framework-1.6.3/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 19:44:59.919225 yetl-framework-1.6.3/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1093 2023-07-01 19:44:59.000000 yetl-framework-1.6.3/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      999 2023-07-01 19:44:59.000000 yetl-framework-1.6.3/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-01 19:44:59.000000 yetl-framework-1.6.3/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-01 19:44:59.000000 yetl-framework-1.6.3/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       57 2023-07-01 19:44:59.000000 yetl-framework-1.6.3/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-07-01 19:44:59.000000 yetl-framework-1.6.3/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-1.6.2/PKG-INFO` & `yetl-framework-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.6.2
+Version: 1.6.3
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.6.2/README.md` & `yetl-framework-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.2/setup.py` & `yetl-framework-1.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="1.6.2",
+    version="1.6.3",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
```

### Comparing `yetl-framework-1.6.2/yetl/__main__.py` & `yetl-framework-1.6.3/yetl/__main__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.2/yetl/cli/_init.py` & `yetl-framework-1.6.3/yetl/cli/_init.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.2/yetl/cli/metadata_provider/_xlsx.py` & `yetl-framework-1.6.3/yetl/cli/metadata_provider/_xlsx.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.2/yetl/config/__init__.py` & `yetl-framework-1.6.3/yetl/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.2/yetl/config/_config.py` & `yetl-framework-1.6.3/yetl/config/_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.2/yetl/config/_decorators.py` & `yetl-framework-1.6.3/yetl/config/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.2/yetl/config/_logging_config.py` & `yetl-framework-1.6.3/yetl/config/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.2/yetl/config/_project.py` & `yetl-framework-1.6.3/yetl/config/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.2/yetl/config/_spark_context.py` & `yetl-framework-1.6.3/yetl/config/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.2/yetl/config/_tables.py` & `yetl-framework-1.6.3/yetl/config/_tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,46 +48,46 @@
         for stage_name, table_type in self.table_data["tables"].items():
             stage_type = StageType(stage_name)
             for table_type_name, database in table_type.items():
                 table_type = TableType(table_type_name)
                 push_down_properties = {}
                 for database_name, table in database.items():
                     if PushDownProperties.has_not_value(database_name):
+                        catalog = table.get(PushDownProperties.CATALOG.value)
+                        del table[PushDownProperties.CATALOG.value]
                         for table_name, table_properties in table.items():
-                            if PushDownProperties.has_not_value(table_name):
-                                table_config = {
-                                    KeyContants.DATABASE.value: database_name,
-                                    KeyContants.TABLE.value: table_name,
-                                    KeyContants.STAGE.value: stage_type,
-                                    KeyContants.TABLE_TYPE.value: table_type,
-                                    KeyContants.PROJECT.value: self.table_data.get(
-                                        KeyContants.PROJECT.value
-                                    ),
-                                    KeyContants.TIMESLICE.value: self.table_data.get(
-                                        KeyContants.TIMESLICE.value
-                                    ),
-                                    KeyContants.CONFIG_PATH.value: self.table_data.get(
-                                        KeyContants.CONFIG_PATH.value
-                                    ),
-                                }
-                                if table_properties:
-                                    table_config = {**table_config, **table_properties}
-                                table_config = {**push_down_properties, **table_config}
-                                for p, v in push_down_properties.items():
-                                    if isinstance(v, dict) and table_config.get(p):
-                                        table_config[p] = {**v, **table_config[p]}
-                                    else:
-                                        table_config[p] = v
-                                stage_config = self.table_data.get(stage_type.value, {})
-                                stage_config = stage_config.get(table_type.value, {})
-                                table_config = {**stage_config, **table_config}
-                                index = f"{stage_name}.{database_name}.{table_name}"
-                                self.tables_index[index] = table_config
-                            else:
-                                push_down_properties[table_name] = table_properties
+                            table_config = {
+                                KeyContants.DATABASE.value: database_name,
+                                KeyContants.TABLE.value: table_name,
+                                KeyContants.STAGE.value: stage_type,
+                                KeyContants.TABLE_TYPE.value: table_type,
+                                KeyContants.PROJECT.value: self.table_data.get(
+                                    KeyContants.PROJECT.value
+                                ),
+                                KeyContants.TIMESLICE.value: self.table_data.get(
+                                    KeyContants.TIMESLICE.value
+                                ),
+                                KeyContants.CONFIG_PATH.value: self.table_data.get(
+                                    KeyContants.CONFIG_PATH.value
+                                ),
+                            }
+                            if table_properties:
+                                table_config = {**table_config, **table_properties}
+                            table_config = {**push_down_properties, **table_config}
+                            table_config[PushDownProperties.CATALOG.value] = catalog
+                            for p, v in push_down_properties.items():
+                                if isinstance(v, dict) and table_config.get(p):
+                                    table_config[p] = {**v, **table_config[p]}
+                                else:
+                                    table_config[p] = v
+                            stage_config = self.table_data.get(stage_type.value, {})
+                            stage_config = stage_config.get(table_type.value, {})
+                            table_config = {**stage_config, **table_config}
+                            index = f"{stage_name}.{database_name}.{table_name}"
+                            self.tables_index[index] = table_config
                     else:
                         push_down_properties[database_name] = table
 
     table_data: dict = Field(...)
     tables_index: Dict[str, Table] = Field(default={})
     delta_properties: Dict[str, str] = Field(default=None)
     _logger: Any = PrivateAttr(default=None)
```

### Comparing `yetl-framework-1.6.2/yetl/config/_timeslice.py` & `yetl-framework-1.6.3/yetl/config/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.2/yetl/config/_utils.py` & `yetl-framework-1.6.3/yetl/config/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.2/yetl/config/deltalake.py` & `yetl-framework-1.6.3/yetl/config/deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.2/yetl/config/table/_deltalake.py` & `yetl-framework-1.6.3/yetl/config/table/_deltalake.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,16 @@
                 self._replacements[
                     JinjaVariables.DELTA_PROPERTIES
                 ] = delta_properties_sql
             self.database = render_jinja(self.database, self._replacements)
             self.table = render_jinja(self.table, self._replacements)
             self.location = render_jinja(self.location, self._replacements)
             self.path = render_jinja(self.path, self._replacements)
-            self.location = os.path.join(self.location, self.path)
+            if self.location and self.path:
+                self.location = os.path.join(self.location, self.path)
             if not is_databricks():
                 self.location = f"{self.config_path}/../data{self.location}"
                 self.location = os.path.abspath(self.location)
             self._replacements[JinjaVariables.LOCATION] = self.location
 
             if self.sql:
                 # render the path
```

### Comparing `yetl-framework-1.6.2/yetl/config/table/_factory.py` & `yetl-framework-1.6.3/yetl/config/table/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.2/yetl/config/table/_read.py` & `yetl-framework-1.6.3/yetl/config/table/_read.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.2/yetl/config/table/_table.py` & `yetl-framework-1.6.3/yetl/config/table/_table.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.2/yetl/workflow/_dlt.py` & `yetl-framework-1.6.3/yetl/workflow/_dlt.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.2/yetl/workflow/_multi_threaded.py` & `yetl-framework-1.6.3/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.2/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-1.6.3/yetl_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.6.2
+Version: 1.6.3
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.6.2/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-1.6.3/yetl_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

