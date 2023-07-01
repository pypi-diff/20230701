# Comparing `tmp/yetl-framework-1.6.0.dev1.tar.gz` & `tmp/yetl-framework-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-1.6.0.dev1.tar", last modified: Sat Jul  1 15:25:32 2023, max compression
+gzip compressed data, was "yetl-framework-1.6.1.tar", last modified: Sat Jul  1 17:27:57 2023, max compression
```

## Comparing `yetl-framework-1.6.0.dev1.tar` & `yetl-framework-1.6.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 15:25:32.843798 yetl-framework-1.6.0.dev1/
--rw-r--r--   0 vsts      (1001) docker     (123)     1098 2023-07-01 15:25:32.843798 yetl-framework-1.6.0.dev1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      596 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-01 15:25:32.843798 yetl-framework-1.6.0.dev1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1222 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 15:25:32.839799 yetl-framework-1.6.0.dev1/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1141 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/yetl/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 15:25:32.839799 yetl-framework-1.6.0.dev1/yetl/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)     2845 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/yetl/cli/_init.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 15:25:32.839799 yetl-framework-1.6.0.dev1/yetl/cli/metadata_provider/
--rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/yetl/cli/metadata_provider/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16277 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/yetl/cli/metadata_provider/_xlsx.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 15:25:32.839799 yetl-framework-1.6.0.dev1/yetl/config/
--rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/yetl/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3284 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/yetl/config/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2195 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/yetl/config/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/yetl/config/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/yetl/config/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1309 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/yetl/config/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/yetl/config/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/yetl/config/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10103 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/yetl/config/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/yetl/config/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5040 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/yetl/config/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17636 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/yetl/config/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 15:25:32.843798 yetl-framework-1.6.0.dev1/yetl/config/table/
--rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/yetl/config/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4693 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/yetl/config/table/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/yetl/config/table/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6541 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/yetl/config/table/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4612 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/yetl/config/table/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/yetl/config/table/_table_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/yetl/config/table/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 15:25:32.843798 yetl-framework-1.6.0.dev1/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      167 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1312 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/yetl/workflow/_dlt.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-07-01 15:24:31.000000 yetl-framework-1.6.0.dev1/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 15:25:32.843798 yetl-framework-1.6.0.dev1/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     1098 2023-07-01 15:25:32.000000 yetl-framework-1.6.0.dev1/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      999 2023-07-01 15:25:32.000000 yetl-framework-1.6.0.dev1/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-01 15:25:32.000000 yetl-framework-1.6.0.dev1/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-01 15:25:32.000000 yetl-framework-1.6.0.dev1/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       57 2023-07-01 15:25:32.000000 yetl-framework-1.6.0.dev1/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-07-01 15:25:32.000000 yetl-framework-1.6.0.dev1/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 17:27:57.957928 yetl-framework-1.6.1/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1093 2023-07-01 17:27:57.957928 yetl-framework-1.6.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      596 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-01 17:27:57.957928 yetl-framework-1.6.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1217 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 17:27:57.953928 yetl-framework-1.6.1/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1141 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/yetl/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 17:27:57.953928 yetl-framework-1.6.1/yetl/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2845 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/yetl/cli/_init.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 17:27:57.953928 yetl-framework-1.6.1/yetl/cli/metadata_provider/
+-rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/yetl/cli/metadata_provider/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16286 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/yetl/cli/metadata_provider/_xlsx.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 17:27:57.953928 yetl-framework-1.6.1/yetl/config/
+-rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/yetl/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3284 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/yetl/config/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2195 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/yetl/config/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/yetl/config/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/yetl/config/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1309 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/yetl/config/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/yetl/config/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/yetl/config/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10103 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/yetl/config/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/yetl/config/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5040 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/yetl/config/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17636 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/yetl/config/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 17:27:57.953928 yetl-framework-1.6.1/yetl/config/table/
+-rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/yetl/config/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4693 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/yetl/config/table/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/yetl/config/table/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6541 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/yetl/config/table/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4612 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/yetl/config/table/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/yetl/config/table/_table_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/yetl/config/table/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 17:27:57.953928 yetl-framework-1.6.1/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      167 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1312 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/yetl/workflow/_dlt.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-07-01 17:27:03.000000 yetl-framework-1.6.1/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-01 17:27:57.957928 yetl-framework-1.6.1/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1093 2023-07-01 17:27:57.000000 yetl-framework-1.6.1/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      999 2023-07-01 17:27:57.000000 yetl-framework-1.6.1/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-01 17:27:57.000000 yetl-framework-1.6.1/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-01 17:27:57.000000 yetl-framework-1.6.1/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       57 2023-07-01 17:27:57.000000 yetl-framework-1.6.1/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-07-01 17:27:57.000000 yetl-framework-1.6.1/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-1.6.0.dev1/PKG-INFO` & `yetl-framework-1.6.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.6.0.dev1
+Version: 1.6.1
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.6.0.dev1/README.md` & `yetl-framework-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.0.dev1/setup.py` & `yetl-framework-1.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="1.6.0.dev1",
+    version="1.6.1",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
```

### Comparing `yetl-framework-1.6.0.dev1/yetl/__main__.py` & `yetl-framework-1.6.1/yetl/__main__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.0.dev1/yetl/cli/_init.py` & `yetl-framework-1.6.1/yetl/cli/_init.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.0.dev1/yetl/cli/metadata_provider/_xlsx.py` & `yetl-framework-1.6.1/yetl/cli/metadata_provider/_xlsx.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     }
 
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
 
     stage: StageType = Field(...)
     table_type: TableType = Field(...)
-    catalog: str = Field(...)
+    catalog: str = Field(default=None)
     database: str = Field(...)
     table: str = Field(...)
     sql: str = Field(default=None)
     id: str = Field(default=None)
     depends_on: str = Field(default=None)
     deltalake_delta_properties: str = Field(default=None)
     custom_properties: Dict[str, Any] = Field(default=None)
```

### Comparing `yetl-framework-1.6.0.dev1/yetl/config/__init__.py` & `yetl-framework-1.6.1/yetl/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.0.dev1/yetl/config/_config.py` & `yetl-framework-1.6.1/yetl/config/_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.0.dev1/yetl/config/_decorators.py` & `yetl-framework-1.6.1/yetl/config/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.0.dev1/yetl/config/_logging_config.py` & `yetl-framework-1.6.1/yetl/config/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.0.dev1/yetl/config/_project.py` & `yetl-framework-1.6.1/yetl/config/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.0.dev1/yetl/config/_spark_context.py` & `yetl-framework-1.6.1/yetl/config/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.0.dev1/yetl/config/_tables.py` & `yetl-framework-1.6.1/yetl/config/_tables.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.0.dev1/yetl/config/_timeslice.py` & `yetl-framework-1.6.1/yetl/config/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.0.dev1/yetl/config/_utils.py` & `yetl-framework-1.6.1/yetl/config/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.0.dev1/yetl/config/deltalake.py` & `yetl-framework-1.6.1/yetl/config/deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.0.dev1/yetl/config/table/_deltalake.py` & `yetl-framework-1.6.1/yetl/config/table/_deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.0.dev1/yetl/config/table/_factory.py` & `yetl-framework-1.6.1/yetl/config/table/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.0.dev1/yetl/config/table/_read.py` & `yetl-framework-1.6.1/yetl/config/table/_read.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.0.dev1/yetl/config/table/_table.py` & `yetl-framework-1.6.1/yetl/config/table/_table.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.0.dev1/yetl/workflow/_dlt.py` & `yetl-framework-1.6.1/yetl/workflow/_dlt.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.0.dev1/yetl/workflow/_multi_threaded.py` & `yetl-framework-1.6.1/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.0.dev1/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-1.6.1/yetl_framework.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.6.0.dev1
+Version: 1.6.1
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.6.0.dev1/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-1.6.1/yetl_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

