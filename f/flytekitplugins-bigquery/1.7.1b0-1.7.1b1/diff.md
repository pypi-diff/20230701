# Comparing `tmp/flytekitplugins-bigquery-1.7.1b0.tar.gz` & `tmp/flytekitplugins-bigquery-1.7.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-bigquery-1.7.1b0.tar", last modified: Fri Jun 16 18:14:16 2023, max compression
+gzip compressed data, was "flytekitplugins-bigquery-1.7.1b1.tar", last modified: Tue Jun 27 22:00:52 2023, max compression
```

## Comparing `flytekitplugins-bigquery-1.7.1b0.tar` & `flytekitplugins-bigquery-1.7.1b1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:16.414468 flytekitplugins-bigquery-1.7.1b0/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-16 18:14:16.414468 flytekitplugins-bigquery-1.7.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-16 18:13:54.000000 flytekitplugins-bigquery-1.7.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:16.414468 flytekitplugins-bigquery-1.7.1b0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:16.414468 flytekitplugins-bigquery-1.7.1b0/flytekitplugins/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-16 18:13:54.000000 flytekitplugins-bigquery-1.7.1b0/flytekitplugins/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-16 18:13:54.000000 flytekitplugins-bigquery-1.7.1b0/flytekitplugins/bigquery/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-16 18:13:54.000000 flytekitplugins-bigquery-1.7.1b0/flytekitplugins/bigquery/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:16.414468 flytekitplugins-bigquery-1.7.1b0/flytekitplugins_bigquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-16 18:14:16.000000 flytekitplugins-bigquery-1.7.1b0/flytekitplugins_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-16 18:14:16.000000 flytekitplugins-bigquery-1.7.1b0/flytekitplugins_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 18:14:16.000000 flytekitplugins-bigquery-1.7.1b0/flytekitplugins_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-16 18:14:16.000000 flytekitplugins-bigquery-1.7.1b0/flytekitplugins_bigquery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 18:14:16.000000 flytekitplugins-bigquery-1.7.1b0/flytekitplugins_bigquery.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 18:14:16.000000 flytekitplugins-bigquery-1.7.1b0/flytekitplugins_bigquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 18:14:16.000000 flytekitplugins-bigquery-1.7.1b0/flytekitplugins_bigquery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 18:14:16.414468 flytekitplugins-bigquery-1.7.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-16 18:14:14.000000 flytekitplugins-bigquery-1.7.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:52.044587 flytekitplugins-bigquery-1.7.1b1/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-27 22:00:52.040587 flytekitplugins-bigquery-1.7.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-27 22:00:35.000000 flytekitplugins-bigquery-1.7.1b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:52.040587 flytekitplugins-bigquery-1.7.1b1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:52.040587 flytekitplugins-bigquery-1.7.1b1/flytekitplugins/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-27 22:00:35.000000 flytekitplugins-bigquery-1.7.1b1/flytekitplugins/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-27 22:00:35.000000 flytekitplugins-bigquery-1.7.1b1/flytekitplugins/bigquery/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-27 22:00:35.000000 flytekitplugins-bigquery-1.7.1b1/flytekitplugins/bigquery/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:52.040587 flytekitplugins-bigquery-1.7.1b1/flytekitplugins_bigquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-27 22:00:52.000000 flytekitplugins-bigquery-1.7.1b1/flytekitplugins_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-27 22:00:52.000000 flytekitplugins-bigquery-1.7.1b1/flytekitplugins_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 22:00:52.000000 flytekitplugins-bigquery-1.7.1b1/flytekitplugins_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-27 22:00:52.000000 flytekitplugins-bigquery-1.7.1b1/flytekitplugins_bigquery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 22:00:52.000000 flytekitplugins-bigquery-1.7.1b1/flytekitplugins_bigquery.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 22:00:52.000000 flytekitplugins-bigquery-1.7.1b1/flytekitplugins_bigquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 22:00:52.000000 flytekitplugins-bigquery-1.7.1b1/flytekitplugins_bigquery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 22:00:52.044587 flytekitplugins-bigquery-1.7.1b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-27 22:00:50.000000 flytekitplugins-bigquery-1.7.1b1/setup.py
```

### Comparing `flytekitplugins-bigquery-1.7.1b0/PKG-INFO` & `flytekitplugins-bigquery-1.7.1b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-bigquery
-Version: 1.7.1b0
+Version: 1.7.1b1
 Summary: This package holds the Bigquery plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-bigquery-1.7.1b0/README.md` & `flytekitplugins-bigquery-1.7.1b1/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-bigquery-1.7.1b0/flytekitplugins/bigquery/agent.py` & `flytekitplugins-bigquery-1.7.1b1/flytekitplugins/bigquery/agent.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 import datetime
 import json
 from dataclasses import asdict, dataclass
 from typing import Dict, Optional
 
 import grpc
-from flyteidl.admin.agent_pb2 import SUCCEEDED, CreateTaskResponse, DeleteTaskResponse, GetTaskResponse, Resource
+from flyteidl.admin.agent_pb2 import (
+    PERMANENT_FAILURE,
+    SUCCEEDED,
+    CreateTaskResponse,
+    DeleteTaskResponse,
+    GetTaskResponse,
+    Resource,
+)
 from google.cloud import bigquery
 
 from flytekit import FlyteContextManager, StructuredDataset, logger
 from flytekit.core.type_engine import TypeEngine
 from flytekit.extend.backend.base_agent import AgentBase, AgentRegistry, convert_to_flyte_state
 from flytekit.models import literals
 from flytekit.models.literals import LiteralMap
@@ -26,14 +33,16 @@
     str: "STRING",
 }
 
 
 @dataclass
 class Metadata:
     job_id: str
+    project: str
+    location: str
 
 
 class BigQueryAgent(AgentBase):
     def __init__(self):
         super().__init__(task_type="bigquery_query_job_task")
 
     def create(
@@ -46,55 +55,63 @@
         job_config = None
         if inputs:
             ctx = FlyteContextManager.current_context()
             python_interface_inputs = {
                 name: TypeEngine.guess_python_type(lt.type) for name, lt in task_template.interface.inputs.items()
             }
             native_inputs = TypeEngine.literal_map_to_kwargs(ctx, inputs, python_interface_inputs)
-
             logger.info(f"Create BigQuery job config with inputs: {native_inputs}")
             job_config = bigquery.QueryJobConfig(
                 query_parameters=[
                     bigquery.ScalarQueryParameter(name, pythonTypeToBigQueryType[python_interface_inputs[name]], val)
                     for name, val in native_inputs.items()
                 ]
             )
 
         custom = task_template.custom
-        client = bigquery.Client(project=custom["ProjectID"], location=custom["Location"])
+        project = custom["ProjectID"]
+        location = custom["Location"]
+        client = bigquery.Client(project=project, location=location)
         query_job = client.query(task_template.sql.statement, job_config=job_config)
+        metadata = Metadata(job_id=str(query_job.job_id), location=location, project=project)
 
-        return CreateTaskResponse(
-            resource_meta=json.dumps(asdict(Metadata(job_id=str(query_job.job_id)))).encode("utf-8")
-        )
+        return CreateTaskResponse(resource_meta=json.dumps(asdict(metadata)).encode("utf-8"))
 
     def get(self, context: grpc.ServicerContext, resource_meta: bytes) -> GetTaskResponse:
         client = bigquery.Client()
         metadata = Metadata(**json.loads(resource_meta.decode("utf-8")))
-        job = client.get_job(metadata.job_id)
+        job = client.get_job(metadata.job_id, metadata.project, metadata.location)
+        if job.errors:
+            logger.error(job.errors.__str__())
+            context.set_code(grpc.StatusCode.INTERNAL)
+            context.set_details(job.errors.__str__())
+            return GetTaskResponse(resource=Resource(state=PERMANENT_FAILURE))
         cur_state = convert_to_flyte_state(str(job.state))
         res = None
 
         if cur_state == SUCCEEDED:
             ctx = FlyteContextManager.current_context()
-            output_location = f"bq://{job.destination.project}:{job.destination.dataset_id}.{job.destination.table_id}"
-            res = literals.LiteralMap(
-                {
-                    "results": TypeEngine.to_literal(
-                        ctx,
-                        StructuredDataset(uri=output_location),
-                        StructuredDataset,
-                        LiteralType(structured_dataset_type=StructuredDatasetType(format="")),
-                    )
-                }
-            )
+            if job.destination:
+                output_location = (
+                    f"bq://{job.destination.project}:{job.destination.dataset_id}.{job.destination.table_id}"
+                )
+                res = literals.LiteralMap(
+                    {
+                        "results": TypeEngine.to_literal(
+                            ctx,
+                            StructuredDataset(uri=output_location),
+                            StructuredDataset,
+                            LiteralType(structured_dataset_type=StructuredDatasetType(format="")),
+                        )
+                    }
+                ).to_flyte_idl()
 
-        return GetTaskResponse(resource=Resource(state=cur_state, outputs=res.to_flyte_idl()))
+        return GetTaskResponse(resource=Resource(state=cur_state, outputs=res))
 
     def delete(self, context: grpc.ServicerContext, resource_meta: bytes) -> DeleteTaskResponse:
         client = bigquery.Client()
         metadata = Metadata(**json.loads(resource_meta.decode("utf-8")))
-        client.cancel_job(metadata.job_id)
+        client.cancel_job(metadata.job_id, metadata.project, metadata.location)
         return DeleteTaskResponse()
 
 
 AgentRegistry.register(BigQueryAgent())
```

### Comparing `flytekitplugins-bigquery-1.7.1b0/flytekitplugins/bigquery/task.py` & `flytekitplugins-bigquery-1.7.1b1/flytekitplugins/bigquery/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-bigquery-1.7.1b0/flytekitplugins_bigquery.egg-info/PKG-INFO` & `flytekitplugins-bigquery-1.7.1b1/flytekitplugins_bigquery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-bigquery
-Version: 1.7.1b0
+Version: 1.7.1b1
 Summary: This package holds the Bigquery plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-bigquery-1.7.1b0/setup.py` & `flytekitplugins-bigquery-1.7.1b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "bigquery"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "google-cloud-bigquery"]
 
-__version__ = "1.7.1b0"
+__version__ = "1.7.1b1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds the Bigquery plugins for flytekit",
```

