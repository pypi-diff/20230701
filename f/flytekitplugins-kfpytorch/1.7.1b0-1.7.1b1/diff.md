# Comparing `tmp/flytekitplugins-kfpytorch-1.7.1b0.tar.gz` & `tmp/flytekitplugins-kfpytorch-1.7.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-kfpytorch-1.7.1b0.tar", last modified: Fri Jun 16 18:14:22 2023, max compression
+gzip compressed data, was "flytekitplugins-kfpytorch-1.7.1b1.tar", last modified: Tue Jun 27 22:00:56 2023, max compression
```

## Comparing `flytekitplugins-kfpytorch-1.7.1b0.tar` & `flytekitplugins-kfpytorch-1.7.1b1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:22.558407 flytekitplugins-kfpytorch-1.7.1b0/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-16 18:14:22.554407 flytekitplugins-kfpytorch-1.7.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-16 18:13:54.000000 flytekitplugins-kfpytorch-1.7.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:22.554407 flytekitplugins-kfpytorch-1.7.1b0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:22.554407 flytekitplugins-kfpytorch-1.7.1b0/flytekitplugins/kfpytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-16 18:13:54.000000 flytekitplugins-kfpytorch-1.7.1b0/flytekitplugins/kfpytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14917 2023-06-16 18:13:54.000000 flytekitplugins-kfpytorch-1.7.1b0/flytekitplugins/kfpytorch/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:14:22.554407 flytekitplugins-kfpytorch-1.7.1b0/flytekitplugins_kfpytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-16 18:14:22.000000 flytekitplugins-kfpytorch-1.7.1b0/flytekitplugins_kfpytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-16 18:14:22.000000 flytekitplugins-kfpytorch-1.7.1b0/flytekitplugins_kfpytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 18:14:22.000000 flytekitplugins-kfpytorch-1.7.1b0/flytekitplugins_kfpytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 18:14:22.000000 flytekitplugins-kfpytorch-1.7.1b0/flytekitplugins_kfpytorch.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-16 18:14:22.000000 flytekitplugins-kfpytorch-1.7.1b0/flytekitplugins_kfpytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 18:14:22.000000 flytekitplugins-kfpytorch-1.7.1b0/flytekitplugins_kfpytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 18:14:22.558407 flytekitplugins-kfpytorch-1.7.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-16 18:14:14.000000 flytekitplugins-kfpytorch-1.7.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:56.852686 flytekitplugins-kfpytorch-1.7.1b1/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-27 22:00:56.852686 flytekitplugins-kfpytorch-1.7.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-27 22:00:35.000000 flytekitplugins-kfpytorch-1.7.1b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:56.848686 flytekitplugins-kfpytorch-1.7.1b1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:56.848686 flytekitplugins-kfpytorch-1.7.1b1/flytekitplugins/kfpytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-27 22:00:35.000000 flytekitplugins-kfpytorch-1.7.1b1/flytekitplugins/kfpytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16408 2023-06-27 22:00:35.000000 flytekitplugins-kfpytorch-1.7.1b1/flytekitplugins/kfpytorch/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:56.852686 flytekitplugins-kfpytorch-1.7.1b1/flytekitplugins_kfpytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-27 22:00:56.000000 flytekitplugins-kfpytorch-1.7.1b1/flytekitplugins_kfpytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-27 22:00:56.000000 flytekitplugins-kfpytorch-1.7.1b1/flytekitplugins_kfpytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 22:00:56.000000 flytekitplugins-kfpytorch-1.7.1b1/flytekitplugins_kfpytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 22:00:56.000000 flytekitplugins-kfpytorch-1.7.1b1/flytekitplugins_kfpytorch.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-27 22:00:56.000000 flytekitplugins-kfpytorch-1.7.1b1/flytekitplugins_kfpytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 22:00:56.000000 flytekitplugins-kfpytorch-1.7.1b1/flytekitplugins_kfpytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 22:00:56.852686 flytekitplugins-kfpytorch-1.7.1b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-27 22:00:50.000000 flytekitplugins-kfpytorch-1.7.1b1/setup.py
```

### Comparing `flytekitplugins-kfpytorch-1.7.1b0/PKG-INFO` & `flytekitplugins-kfpytorch-1.7.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfpytorch
-Version: 1.7.1b0
+Version: 1.7.1b1
 Summary: K8s based Pytorch plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kfpytorch-1.7.1b0/README.md` & `flytekitplugins-kfpytorch-1.7.1b1/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-kfpytorch-1.7.1b0/flytekitplugins/kfpytorch/task.py` & `flytekitplugins-kfpytorch-1.7.1b1/flytekitplugins/kfpytorch/task.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from google.protobuf.json_format import MessageToDict
 
 import flytekit
 from flytekit import PythonFunctionTask, Resources
 from flytekit.configuration import SerializationSettings
 from flytekit.core.resources import convert_resources_to_resource_model
 from flytekit.extend import IgnoreOutputs, TaskPlugins
+from flytekit.loggers import logger
 
 TORCH_IMPORT_ERROR_MESSAGE = "PyTorch is not installed. Please install `flytekitplugins-kfpytorch['elastic']`."
 
 
 @dataclass
 class RestartPolicy(Enum):
     """
@@ -195,32 +196,43 @@
         return MessageToDict(pytorch_job)
 
 
 # Register the Pytorch Plugin into the flytekit core plugin system
 TaskPlugins.register_pythontask_plugin(PyTorch, PyTorchFunctionTask)
 
 
-def spawn_helper(fn: bytes, kwargs) -> Any:
+def spawn_helper(fn: bytes, raw_output_prefix: str, checkpoint_dest: str, checkpoint_src: str, kwargs) -> Any:
     """Help to spawn worker processes.
 
     The purpose of this function is to 1) be pickleable so that it can be used with
     the multiprocessing start method `spawn` and 2) to call a cloudpickle-serialized
     function passed to it. This function itself doesn't have to be pickleable. Without
     such a helper task functions, which are not pickleable, couldn't be used with the
     start method `spawn`.
 
     Args:
         fn (bytes): Cloudpickle-serialized target function to be executed in the worker process.
+        raw_output_prefix (str): Where to write offloaded data (files, directories, dataframes).
+        checkpoint_dest (str): If a previous checkpoint exists, this path should is set to the folder
+            that contains the checkpoint information.
+        checkpoint_src (str): Location where the new checkpoint should be copied to.
 
     Returns:
         The return value of the received target function.
     """
-    fn = cloudpickle.loads(fn)
-    return_val = fn(**kwargs)
-    return return_val
+    from flytekit.bin.entrypoint import setup_execution
+
+    with setup_execution(
+        raw_output_data_prefix=raw_output_prefix,
+        checkpoint_path=checkpoint_dest,
+        prev_checkpoint=checkpoint_src,
+    ):
+        fn = cloudpickle.loads(fn)
+        return_val = fn(**kwargs)
+        return return_val
 
 
 class PytorchElasticFunctionTask(PythonFunctionTask[Elastic]):
     """
     Plugin for distributed training with torch elastic/torchrun (see
     https://pytorch.org/docs/stable/elastic/run.html).
     """
@@ -270,14 +282,23 @@
             raise ImportError(TORCH_IMPORT_ERROR_MESSAGE)
 
         if isinstance(self.task_config.nproc_per_node, str):
             nproc = run.determine_local_world_size(self.task_config.nproc_per_node)
         else:
             nproc = self.task_config.nproc_per_node
 
+        dist_env_vars_set = os.environ.get("PET_NNODES") is not None
+        if not dist_env_vars_set and self.min_nodes > 1:
+            logger.warning(
+                (
+                    f"`nnodes` is set to {self.task_config.nnodes} in elastic task but execution appears "
+                    "to not run in a `PyTorchJob`. Rendezvous might timeout."
+                )
+            )
+
         config = LaunchConfig(
             run_id=flytekit.current_context().execution_id.name,
             min_nodes=self.min_nodes,
             max_nodes=self.max_nodes,
             nproc_per_node=nproc,
             rdzv_backend=self.rdzv_backend,  # rdzv settings
             rdzv_endpoint=os.environ.get("PET_RDZV_ENDPOINT", "localhost:0"),
@@ -292,15 +313,25 @@
             The torch elastic launcher then launches the spawn_helper function (which is pickleable)
             instead of the task function. This helper function, in the child-process, then deserializes
             the task function, again with cloudpickle, and executes it.
             """
             launcher_target_func = spawn_helper
 
             dumped_target_function = cloudpickle.dumps(self._task_function)
-            launcher_args = (dumped_target_function, kwargs)
+
+            ctx = flytekit.current_context()
+            try:
+                checkpoint_dest = ctx.checkpoint._checkpoint_dest
+                checkpoint_src = ctx.checkpoint._checkpoint_src
+            except NotImplementedError:
+                # Not using checkpointing in parent process
+                checkpoint_dest = None
+                checkpoint_src = None
+
+            launcher_args = (dumped_target_function, ctx.raw_output_prefix, checkpoint_dest, checkpoint_src, kwargs)
         elif self.task_config.start_method == "fork":
             """
             The torch elastic launcher doesn't support passing kwargs to the target function,
             only args. Flyte only works with kwargs. Thus, we create a closure which already has
             the task kwargs bound. We tell the torch elastic launcher to start this function in
             the child processes.
             """
```

### Comparing `flytekitplugins-kfpytorch-1.7.1b0/flytekitplugins_kfpytorch.egg-info/PKG-INFO` & `flytekitplugins-kfpytorch-1.7.1b1/flytekitplugins_kfpytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfpytorch
-Version: 1.7.1b0
+Version: 1.7.1b1
 Summary: K8s based Pytorch plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kfpytorch-1.7.1b0/setup.py` & `flytekitplugins-kfpytorch-1.7.1b1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "kfpytorch"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["cloudpickle", "flyteidl>=1.5.1", "flytekit>=1.6.1"]
 
-__version__ = "1.7.1b0"
+__version__ = "1.7.1b1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="K8s based Pytorch plugin for Flytekit",
```

