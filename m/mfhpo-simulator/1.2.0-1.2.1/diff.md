# Comparing `tmp/mfhpo_simulator-1.2.0-py3-none-any.whl.zip` & `tmp/mfhpo_simulator-1.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,23 @@
-Zip file size: 11781 bytes, number of entries: 10
--rw-rw-r--  2.0 unx      606 b- defN 23-Jul-01 05:59 benchmark_simulator/__init__.py
--rw-rw-r--  2.0 unx     6226 b- defN 23-Jul-01 05:59 benchmark_simulator/_constants.py
--rw-rw-r--  2.0 unx    11199 b- defN 23-Jul-01 05:59 benchmark_simulator/_secure_proc.py
+Zip file size: 33910 bytes, number of entries: 21
+-rw-rw-r--  2.0 unx      560 b- defN 23-Jul-01 06:00 benchmark_simulator/__init__.py
+-rw-rw-r--  2.0 unx     6127 b- defN 23-Jul-01 05:59 benchmark_simulator/_constants.py
+-rw-rw-r--  2.0 unx    11227 b- defN 23-Jul-01 05:59 benchmark_simulator/_secure_proc.py
 -rw-rw-r--  2.0 unx     1772 b- defN 23-Jun-14 22:34 benchmark_simulator/_utils.py
--rw-rw-r--  2.0 unx      332 b- defN 23-Jul-01 05:59 benchmark_simulator/simulator.py
--rw-rw-r--  2.0 unx    10760 b- defN 23-Jul-01 05:59 mfhpo_simulator-1.2.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx      307 b- defN 23-Jul-01 05:59 mfhpo_simulator-1.2.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-01 05:59 mfhpo_simulator-1.2.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       20 b- defN 23-Jul-01 05:59 mfhpo_simulator-1.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      870 b- defN 23-Jul-01 05:59 mfhpo_simulator-1.2.0.dist-info/RECORD
-10 files, 32184 bytes uncompressed, 10281 bytes compressed:  68.1%
+-rw-rw-r--  2.0 unx    20853 b- defN 23-Jul-01 05:59 benchmark_simulator/simulator.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-01 05:59 tests/__init__.py
+-rw-rw-r--  2.0 unx     3134 b- defN 23-Jul-01 05:59 tests/test_optimize.py
+-rw-rw-r--  2.0 unx     4795 b- defN 23-Jul-01 05:59 tests/test_optimize_with_ask_and_tell.py
+-rw-rw-r--  2.0 unx     2954 b- defN 23-Jul-01 05:59 tests/test_order_check.py
+-rw-rw-r--  2.0 unx     3060 b- defN 23-Jul-01 05:59 tests/test_order_check_with_ask_and_tell.py
+-rw-rw-r--  2.0 unx     5395 b- defN 23-Jul-01 05:59 tests/test_secure_proc.py
+-rw-rw-r--  2.0 unx    14769 b- defN 23-Jul-01 05:59 tests/test_simulator.py
+-rw-rw-r--  2.0 unx     9617 b- defN 23-Jul-01 06:00 tests/test_simulator_for_ask_and_tell.py
+-rw-rw-r--  2.0 unx     5579 b- defN 23-Jul-01 05:59 tests/test_timeout_error.py
+-rw-rw-r--  2.0 unx     2139 b- defN 23-Jul-01 05:59 tests/test_utils.py
+-rw-rw-r--  2.0 unx     5250 b- defN 23-Jul-01 05:59 tests/utils.py
+-rw-rw-r--  2.0 unx    10760 b- defN 23-Jul-01 06:03 mfhpo_simulator-1.2.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      307 b- defN 23-Jul-01 06:03 mfhpo_simulator-1.2.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-01 06:03 mfhpo_simulator-1.2.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       26 b- defN 23-Jul-01 06:03 mfhpo_simulator-1.2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1792 b- defN 23-Jul-01 06:03 mfhpo_simulator-1.2.1.dist-info/RECORD
+21 files, 110208 bytes uncompressed, 30984 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -9,23 +9,56 @@
 
 Filename: benchmark_simulator/_utils.py
 Comment: 
 
 Filename: benchmark_simulator/simulator.py
 Comment: 
 
-Filename: mfhpo_simulator-1.2.0.dist-info/LICENSE
+Filename: tests/__init__.py
 Comment: 
 
-Filename: mfhpo_simulator-1.2.0.dist-info/METADATA
+Filename: tests/test_optimize.py
 Comment: 
 
-Filename: mfhpo_simulator-1.2.0.dist-info/WHEEL
+Filename: tests/test_optimize_with_ask_and_tell.py
 Comment: 
 
-Filename: mfhpo_simulator-1.2.0.dist-info/top_level.txt
+Filename: tests/test_order_check.py
 Comment: 
 
-Filename: mfhpo_simulator-1.2.0.dist-info/RECORD
+Filename: tests/test_order_check_with_ask_and_tell.py
+Comment: 
+
+Filename: tests/test_secure_proc.py
+Comment: 
+
+Filename: tests/test_simulator.py
+Comment: 
+
+Filename: tests/test_simulator_for_ask_and_tell.py
+Comment: 
+
+Filename: tests/test_timeout_error.py
+Comment: 
+
+Filename: tests/test_utils.py
+Comment: 
+
+Filename: tests/utils.py
+Comment: 
+
+Filename: mfhpo_simulator-1.2.1.dist-info/LICENSE
+Comment: 
+
+Filename: mfhpo_simulator-1.2.1.dist-info/METADATA
+Comment: 
+
+Filename: mfhpo_simulator-1.2.1.dist-info/WHEEL
+Comment: 
+
+Filename: mfhpo_simulator-1.2.1.dist-info/top_level.txt
+Comment: 
+
+Filename: mfhpo_simulator-1.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## benchmark_simulator/__init__.py

```diff
@@ -1,19 +1,18 @@
 from benchmark_simulator._constants import AbstractAskTellOptimizer, ObjectiveFuncType
-from benchmark_simulator.simulator import AskTellWorkerManager, CentralWorkerManager, ObjectiveFuncWorker
+from benchmark_simulator.simulator import ObjectiveFuncWrapper, get_multiple_wrappers
 
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 __copyright__ = "Copyright (C) 2023 Shuhei Watanabe"
 __licence__ = "Apache-2.0 License"
 __author__ = "Shuhei Watanabe"
 __author_email__ = "shuhei.watanabe.utokyo@gmail.com"
 __url__ = "https://github.com/nabenabe0928/mfhpo-simulator"
 
 
 __all__ = [
     "AbstractAskTellOptimizer",
-    "AskTellWorkerManager",
-    "CentralWorkerManager",
+    "ObjectiveFuncWrapper",
     "ObjectiveFuncType",
-    "ObjectiveFuncWorker",
+    "get_multiple_wrappers",
 ]
```

## benchmark_simulator/_constants.py

```diff
@@ -10,20 +10,14 @@
 
 
 DIR_NAME: Final[str] = "mfhpo-simulator-info/"
 INF: Final[float] = float(1 << 30)
 
 
 @dataclass(frozen=True)
-class _TimeStampDictType:
-    prev_timestamp: float
-    waited_time: float
-
-
-@dataclass(frozen=True)
 class _TimeNowDictType:
     before_sample: float
     after_sample: float
 
 
 @dataclass(frozen=True)
 class _StateType:
@@ -65,15 +59,15 @@
 class _TimeValue:
     terminated: float = float(1 << 40)
     crashed: float = float(1 << 41)
 
 
 @dataclass(frozen=True)
 class _WrapperVars:
-    subdir_name: str
+    save_dir_name: str
     n_workers: int
     obj_func: ObjectiveFuncType
     n_actual_evals_in_opt: int
     n_evals: int
     obj_keys: list[str]
     runtime_key: str
     fidel_keys: list[str] | None
```

## benchmark_simulator/_secure_proc.py

```diff
@@ -6,15 +6,14 @@
 import warnings
 
 from benchmark_simulator._constants import (
     _SharedDataFileNames,
     _StateType,
     _TIME_VALUES,
     _TimeNowDictType,
-    _TimeStampDictType,
 )
 from benchmark_simulator._utils import _SecureLock
 
 import numpy as np
 
 import ujson as json  # type: ignore
 
@@ -71,18 +70,18 @@
         record = json.load(f)
         prev_cumtime = record.get(worker_id, 0.0)
         record[worker_id] = np.clip(cumtime, a_min=prev_cumtime, a_max=_TIME_VALUES.crashed)
         f.seek(0)
         json.dump(record, f, indent=4)
 
 
-def _record_timestamp(path: str, worker_id: str, prev_timestamp: float, waited_time: float, lock: _SecureLock) -> None:
+def _record_timestamp(path: str, worker_id: str, prev_timestamp: float, lock: _SecureLock) -> None:
     with lock.edit(path) as f:
         record = json.load(f)
-        record[worker_id] = dict(prev_timestamp=prev_timestamp, waited_time=waited_time)
+        record[worker_id] = prev_timestamp
         f.seek(0)
         json.dump(record, f, indent=4)
 
 
 def _cache_state(
     path: str, config_hash: int, new_state: _StateType, lock: _SecureLock, update_index: int | None = None
 ) -> None:
@@ -130,17 +129,17 @@
 def _fetch_cumtimes(path: str, lock: _SecureLock) -> dict[str, float]:
     with lock.read(path) as f:
         cumtimes = json.load(f)
 
     return cumtimes
 
 
-def _fetch_timestamps(path: str, lock: _SecureLock) -> dict[str, _TimeStampDictType]:
+def _fetch_timestamps(path: str, lock: _SecureLock) -> dict[str, float]:
     with lock.read(path) as f:
-        timestamps = {th: _TimeStampDictType(**ts_dict) for th, ts_dict in json.load(f).items()}
+        timestamps = json.load(f)
 
     return timestamps
 
 
 def _fetch_proc_alloc(path: str, lock: _SecureLock) -> dict[int, int]:
     return _complete_proc_allocation(path=path, lock=lock)
 
@@ -175,17 +174,20 @@
         result = len(json.load(f)) == n_workers
 
     return result
 
 
 def _is_allocation_ready(path: str, n_workers: int, lock: _SecureLock) -> bool:
     with lock.read(path) as f:
-        result = len(json.load(f)) == n_workers
+        n_allocs = len(json.load(f))
 
-    return result
+    if n_allocs > n_workers:
+        raise ValueError(_get_timeout_message("the allocation of procs", path))
+
+    return n_allocs == n_workers
 
 
 def _get_worker_id_to_idx(path: str, lock: _SecureLock) -> dict[str, int]:
     with lock.read(path) as f:
         result = {worker_id: idx for idx, worker_id in enumerate(json.load(f).keys())}
 
     return result
@@ -194,15 +196,15 @@
 def _is_min_cumtime(path: str, worker_id: str, lock: _SecureLock) -> bool:
     cumtimes = _fetch_cumtimes(path=path, lock=lock)
     proc_cumtime = cumtimes[worker_id]
     return min(cumtime for cumtime in cumtimes.values()) == proc_cumtime
 
 
 def _start_timestamp(path: str, worker_id: str, prev_timestamp: float, lock: _SecureLock) -> None:
-    _record_timestamp(path=path, worker_id=worker_id, prev_timestamp=time.time(), waited_time=0.0, lock=lock)
+    _record_timestamp(path=path, worker_id=worker_id, prev_timestamp=time.time(), lock=lock)
 
 
 def _start_worker_timer(path: str, worker_id: str, lock: _SecureLock) -> None:
     _record_cumtime(path=path, worker_id=worker_id, cumtime=0.0, lock=lock)
 
 
 def _finish_worker_timer(path: str, worker_id: str, lock: _SecureLock) -> None:
@@ -217,18 +219,21 @@
     cumtimes = _fetch_cumtimes(path=path, lock=lock)
     worker_id = min(cumtimes, key=cumtimes.get)  # type: ignore[arg-type]
     _kill_worker_timer(path=path, worker_id=worker_id, lock=lock)
 
 
 def _get_timeout_message(cause: str, path: str) -> str:
     dir_name = os.path.join(*path.split("/")[:-1])
-    msg = f"Timeout in {cause}. There could be two possible reasons:\n"
-    msg += f"(1) The path {dir_name} already existed before the execution of the program.\n"
-    msg += "(2) n_workers specified in your optimizer and that in the simulator might be different."
-    return msg
+    msg = [
+        f"Timeout in {cause}. There could be three possible reasons:",
+        f"(1) The path {dir_name} already existed before the execution of the program.",
+        "(2) n_workers specified in your optimizer and that in the simulator might be different.",
+        "(3) launch_multiple_wrappers_from_user_side is incorrectly set.",
+    ]
+    return "\n".join(msg)
 
 
 def _wait_proc_allocation(
     path: str, n_workers: int, lock: _SecureLock, waiting_time: float = 1e-2, time_limit: float = 10.0
 ) -> dict[int, int]:
     start = time.time()
     waiting_time *= 1 + np.random.random()
```

## benchmark_simulator/simulator.py

```diff
@@ -1,6 +1,421 @@
-from benchmark_simulator._simulator._worker import ObjectiveFuncWorker
-from benchmark_simulator._simulator._worker_manager import CentralWorkerManager
-from benchmark_simulator._simulator._worker_manager_for_ask_and_tell import AskTellWorkerManager
+""" A collection of utilities for a simulation of multi-fidelity optimizations.
 
+In multi-fidelity optimizations, as we often evaluate configs in parallel,
+it is essential to manage the order of config allocations to each worker.
+We allow such appropriate allocations with the utilities in this file.
+To guarantee the safety, we share variables with each process using the file system.
 
-__all__ = ["AskTellWorkerManager", "ObjectiveFuncWorker", "CentralWorkerManager"]
+We first define some terminologies:
+* simulator: A system that manages simulated runtimes to allow optimizations of a tabular/surrogate benchmark
+             without waiting for actual runtimes.
+* worker: Worker instantiates an objective function with a given config and evaluates it.
+* proc: Each worker will be instantiated in each process.
+* worker_id: The time hash generated for each worker.
+* pid or proc_id: The process ID for each proc obtained by `os.getpid()`, which is an integer.
+* index: The index of each worker. (it will be one of the integers in [0, N - 1] where N is the # of workers.)
+
+Now we describe each file shared with each process.
+Note that each file takes the json-dict format and we write down as follows:
+    * key1 -- val1
+    * key2 -- val2
+    :
+    * keyN -- valN
+
+1. mfhpo-simulator-info/*/proc_alloc.json
+    * proc1_id -- worker1_id
+    * proc2_id -- worker2_id
+    :
+    * procN_id -- workerN_id
+Note that we need this file only if we have multiple processes in one run.
+For example, when we use multiprocessing, we might need it.
+`procX_id` is fetched by `os.getpid()` and `workerX_id` is initially generated by `generate_time_hash()`.
+
+2. mfhpo-simulator-info/*/results.json
+    * obj1_name -- list[obj1 at the n-th evaluation]
+    * obj2_name -- list[obj2 at the n-th evaluation]
+    :
+    * objM_name -- list[objM at the n-th evaluation]
+    * cumtime -- list[cumtime up to the n-th evaluation]
+    * index -- list[the index of the worker of the n-th evaluation]
+This file is necessary for post-hoc analysis.
+
+3. mfhpo-simulator-info/*/state_cache.json
+    * config1 -- list[tuple[runtime, cumtime, fidel, seed]]
+    * config2 -- list[tuple[runtime, cumtime, fidel, seed]]
+    :
+    * configN -- list[tuple[runtime, cumtime, fidel, seed]]
+This file tells you the states of each config.
+Runtime tells how long it took to evaluate configX up to the intermediate result.
+Since we would like to use this information only for the restart of trainings,
+we discard the information after each config reaches the full-fidelity training.
+Each list gets more than two elements if evaluations of the same configs happen.
+
+4. mfhpo-simulator-info/*/simulated_cumtime.json
+    * worker1_id -- cumtime1
+    * worker2_id -- cumtime2
+    :
+    * workerN_id -- cumtimeN
+This file tells you how much time each worker virtually spends in the simulation
+and we need this information to manage the order of job allocations to each worker.
+
+5. mfhpo-simulator-info/*/timestamp.json
+    * worker1_id -- prev_timestamp1
+    * worker2_id -- prev_timestamp2
+    :
+    * workerN_id -- prev_timestampN
+This file tells the last checkpoint timestamp of each worker (prev_timestamp).
+
+6. mfhpo-simulator-info/*/timenow.json
+    * before_sample -- [time1 before sample, time2 before sample, ...]
+    * after_sample -- [time1 after sample, time2 after sample, ...]
+This file is used to consider the sampling time.
+after_sample is the latest cumtime immediately after the last sample and before_sample is before the last sample.
+"""
+from __future__ import annotations
+
+import os
+from datetime import datetime
+from multiprocessing import Pool
+from typing import Any
+
+from benchmark_simulator._constants import AbstractAskTellOptimizer, DIR_NAME, ObjectiveFuncType, _WrapperVars
+from benchmark_simulator._simulator._worker import _ObjectiveFuncWorker
+from benchmark_simulator._simulator._worker_manager import _CentralWorkerManager
+from benchmark_simulator._simulator._worker_manager_for_ask_and_tell import _AskTellWorkerManager
+
+import numpy as np
+
+
+def get_multiple_wrappers(
+    obj_func: ObjectiveFuncType,
+    save_dir_name: str | None = None,
+    n_workers: int = 4,
+    n_actual_evals_in_opt: int = 105,
+    n_evals: int = 100,
+    fidel_keys: list[str] | None = None,
+    obj_keys: list[str] | None = None,
+    runtime_key: str = "runtime",
+    seed: int | None = None,
+    continual_max_fidel: int | None = None,
+    max_waiting_time: float = np.inf,
+    check_interval_time: float = 1e-4,
+    store_config: bool = False,
+) -> list[ObjectiveFuncWrapper]:
+    """Return multiple wrapper instances.
+
+    Args:
+        obj_func (ObjectiveFuncType):
+            A callable object that serves as the objective function.
+            Args:
+                eval_config: dict[str, Any]
+                fidels: dict[str, int | float] | None
+                seed: int | None
+                **data_to_scatter: Any
+            Returns:
+                results: dict[str, float]
+                    It must return `objective metric` and `runtime` at least.
+        save_dir_name (str | None):
+            The subdirectory name to store all running information.
+        n_workers (int):
+            The number of workers to use. In other words, how many parallel workers to use.
+        n_actual_evals_in_opt (int):
+            The number of evaluations that optimizers do and it is used only for raising an error in init.
+            Note that the number of evaluations means
+            how many times we call the objective function during the optimization.
+            This number is needed to automatically finish the worker class.
+            We cannot know the timing of the termination without this information, and thus optimizers hang.
+        n_evals (int):
+            How many configurations we would like to collect.
+            More specifically, how many times we call the objective function during the optimization.
+            We can guarantee that `results.json` has at least this number of evaluations.
+        fidel_keys (list[str] | None):
+            The fidelity names to be used in the objective function.
+            If None, we assume that no fidelity is used.
+        obj_keys (list[str] | None):
+            The keys of the objective metrics used in `results` returned by func.
+        runtime_key (str):
+            The key of the runtime metric used in `results` returned by func.
+        seed (int | None):
+            The random seed to be used to allocate random seed to each call.
+        continual_max_fidel (int | None):
+            The maximum fidelity to used in continual evaluations.
+            This is valid only if we use a single fidelity.
+            If not None, each call is a continuation from the call with the same eval_config and lower fidel.
+            For example, when we already trained the objective with configA and training_epoch=10,
+            we probably would like to continue the training from epoch 10 rather than from scratch
+            for call with configA and training_epoch=30.
+            continual_eval=True calculates the runtime considers this.
+            If False, each call is considered to be processed from scratch.
+        check_interval_time (float):
+            How often each worker should check whether they could be assigned a new job.
+            For example, if 1e-2 is specified, each worker check whether they can get a new job every 1e-2 seconds.
+            If there are many workers, too small check_interval_time may cause a big bottleneck.
+            On the other hand, a big check_interval_time spends more time for waiting.
+            By default, check_interval_time is set to a relatively small number, so users might rather want to
+            increase the number to avoid the bottleneck for many workers.
+        max_waiting_time (float):
+            The maximum waiting time to judge hang.
+            If any one of the workers does not do any updates for this amount of time, we raise TimeoutError.
+        store_config (bool):
+            Whether to store all config/fidel information.
+            The information is sorted chronologically.
+            When you do large-scale experiments, this may incur too much storage consumption.
+
+    Returns:
+        wrappers (list[ObjectiveFuncWrapper]):
+            A list of wrappers.
+            It contains n_workers of worker wrappers.
+    """
+    curtime = datetime.now().strftime("%Y-%m-%d-%H:%M:%S")
+    save_dir_name = save_dir_name if save_dir_name is not None else f"data-{curtime}"
+
+    dir_name = os.path.join(DIR_NAME, save_dir_name)
+    if os.path.exists(dir_name):
+        raise FileExistsError(f"The directory `{dir_name}` already exists. Remove it first.")
+
+    wrapper_kwargs = dict(
+        obj_func=obj_func,
+        save_dir_name=save_dir_name,
+        launch_multiple_wrappers_from_user_side=True,
+        n_workers=n_workers,
+        n_actual_evals_in_opt=n_actual_evals_in_opt,
+        n_evals=n_evals,
+        fidel_keys=fidel_keys,
+        obj_keys=obj_keys,
+        runtime_key=runtime_key,
+        seed=seed,
+        continual_max_fidel=continual_max_fidel,
+        max_waiting_time=max_waiting_time,
+        check_interval_time=check_interval_time,
+        store_config=store_config,
+    )
+    pool = Pool()
+    results = []
+    for _ in range(n_workers):
+        results.append(pool.apply_async(ObjectiveFuncWrapper, kwds=wrapper_kwargs))
+
+    pool.close()
+    pool.join()
+    return [result.get() for result in results]
+
+
+class ObjectiveFuncWrapper:
+    def __init__(
+        self,
+        obj_func: ObjectiveFuncType,
+        launch_multiple_wrappers_from_user_side: bool = False,
+        ask_and_tell: bool = False,
+        save_dir_name: str | None = None,
+        n_workers: int = 4,
+        n_actual_evals_in_opt: int = 105,
+        n_evals: int = 100,
+        fidel_keys: list[str] | None = None,
+        obj_keys: list[str] | None = None,
+        runtime_key: str = "runtime",
+        seed: int | None = None,
+        continual_max_fidel: int | None = None,
+        max_waiting_time: float = np.inf,
+        check_interval_time: float = 1e-4,
+        store_config: bool = False,
+    ):
+        """The initialization of a wrapper class.
+
+        Both ObjectiveFuncWorker and CentralWorkerManager have the same interface and the same set of control params.
+
+        Args:
+            obj_func (ObjectiveFuncType):
+                A callable object that serves as the objective function.
+                Args:
+                    eval_config: dict[str, Any]
+                    fidels: dict[str, int | float] | None
+                    seed: int | None
+                    **data_to_scatter: Any
+                Returns:
+                    results: dict[str, float]
+                        It must return `objective metric` and `runtime` at least.
+            launch_multiple_wrappers_from_user_side (bool):
+                Whether users need to launch multiple objective function wrappers from user side.
+                Examples of such cases are available at:
+                    - https://github.com/nabenabe0928/mfhpo-simulator/blob/main/examples/bohb.py
+                    - https://github.com/nabenabe0928/mfhpo-simulator/blob/main/examples/neps.py
+                The first case is so obvious that users need to instantiate multiple worker objects.
+                The second case is a bit tricky because multiple workers are instantiated in different main processes.
+                In this case as well, it is obviously not one worker launch.
+            ask_and_tell (bool):
+                Whether to use an ask-and-tell interface optimizer.
+                If True, the optimization loop will be run in the API side and hence users need to call simulate()
+                to start simulation and the wrapper will be an optimizer wrapper rather than a function wrapper.
+            save_dir_name (str | None):
+                The subdirectory name to store all running information.
+            n_workers (int):
+                The number of workers to use. In other words, how many parallel workers to use.
+            n_actual_evals_in_opt (int):
+                The number of evaluations that optimizers do and it is used only for raising an error in init.
+                Note that the number of evaluations means
+                how many times we call the objective function during the optimization.
+                This number is needed to automatically finish the worker class.
+                We cannot know the timing of the termination without this information, and thus optimizers hang.
+            n_evals (int):
+                How many configurations we would like to collect.
+                More specifically, how many times we call the objective function during the optimization.
+                We can guarantee that `results.json` has at least this number of evaluations.
+            fidel_keys (list[str] | None):
+                The fidelity names to be used in the objective function.
+                If None, we assume that no fidelity is used.
+            obj_keys (list[str] | None):
+                The keys of the objective metrics used in `results` returned by func.
+            runtime_key (str):
+                The key of the runtime metric used in `results` returned by func.
+            seed (int | None):
+                The random seed to be used to allocate random seed to each call.
+            continual_max_fidel (int | None):
+                The maximum fidelity to used in continual evaluations.
+                This is valid only if we use a single fidelity.
+                If not None, each call is a continuation from the call with the same eval_config and lower fidel.
+                For example, when we already trained the objective with configA and training_epoch=10,
+                we probably would like to continue the training from epoch 10 rather than from scratch
+                for call with configA and training_epoch=30.
+                continual_eval=True calculates the runtime considers this.
+                If False, each call is considered to be processed from scratch.
+            check_interval_time (float):
+                How often each worker should check whether they could be assigned a new job.
+                For example, if 1e-2 is specified, each worker check whether they can get a new job every 1e-2 seconds.
+                If there are many workers, too small check_interval_time may cause a big bottleneck.
+                On the other hand, a big check_interval_time spends more time for waiting.
+                By default, check_interval_time is set to a relatively small number, so users might rather want to
+                increase the number to avoid the bottleneck for many workers.
+            max_waiting_time (float):
+                The maximum waiting time to judge hang.
+                If any one of the workers does not do any updates for this amount of time, we raise TimeoutError.
+            store_config (bool):
+                Whether to store all config/fidel information.
+                The information is sorted chronologically.
+                When you do large-scale experiments, this may incur too much storage consumption.
+        """
+        curtime = datetime.now().strftime("%Y-%m-%d-%H:%M:%S")
+        wrapper_vars = _WrapperVars(
+            obj_func=obj_func,
+            save_dir_name=save_dir_name if save_dir_name is not None else f"data-{curtime}",
+            n_workers=n_workers,
+            n_actual_evals_in_opt=n_actual_evals_in_opt,
+            n_evals=n_evals,
+            fidel_keys=fidel_keys,
+            obj_keys=obj_keys if obj_keys is not None else ["loss"],
+            runtime_key=runtime_key,
+            seed=seed,
+            continual_max_fidel=continual_max_fidel,
+            max_waiting_time=max_waiting_time,
+            check_interval_time=check_interval_time,
+            store_config=store_config,
+        )
+
+        self._main_wrapper: _AskTellWorkerManager | _CentralWorkerManager | _ObjectiveFuncWorker
+        self._validate(
+            save_dir_name=save_dir_name,
+            ask_and_tell=ask_and_tell,
+            launch_multiple_wrappers_from_user_side=launch_multiple_wrappers_from_user_side,
+        )
+        if ask_and_tell:
+            self._main_wrapper = _AskTellWorkerManager(wrapper_vars)
+        elif launch_multiple_wrappers_from_user_side:
+            self._main_wrapper = _ObjectiveFuncWorker(wrapper_vars)
+        else:
+            self._main_wrapper = _CentralWorkerManager(wrapper_vars)
+
+    @property
+    def dir_name(self) -> str:
+        return self._main_wrapper.dir_name
+
+    @property
+    def obj_keys(self) -> list[str]:
+        return self._main_wrapper.obj_keys
+
+    @property
+    def runtime_key(self) -> str:
+        return self._main_wrapper.runtime_key
+
+    @property
+    def fidel_keys(self) -> list[str]:
+        return self._main_wrapper.fidel_keys
+
+    @property
+    def n_actual_evals_in_opt(self) -> int:
+        return self._main_wrapper._wrapper_vars.n_actual_evals_in_opt
+
+    @property
+    def n_workers(self) -> int:
+        return self._main_wrapper._wrapper_vars.n_workers
+
+    def _validate(
+        self,
+        save_dir_name: str | None,
+        ask_and_tell: bool,
+        launch_multiple_wrappers_from_user_side: bool,
+    ) -> None:
+        if ask_and_tell and launch_multiple_wrappers_from_user_side:
+            raise ValueError(
+                "ask_and_tell and launch_multiple_wrappers_from_user_side cannot be True at the same time."
+            )
+        if launch_multiple_wrappers_from_user_side and save_dir_name is None:
+            raise ValueError(
+                "When launch_multiple_wrappers_from_user_side is False, save_dir_name must be specified so that \n"
+                "each worker recognizes with which processes it shares the optimization results."
+            )
+
+    def __call__(
+        self,
+        eval_config: dict[str, Any],
+        *,
+        fidels: dict[str, int | float] | None = None,
+        **data_to_scatter: Any,
+    ) -> dict[str, float]:
+        """The meta-wrapper method of the objective function method in WorkerFunc instances.
+
+        This method recognizes each WorkerFunc by process ID and call the corresponding worker based on the ID.
+
+        Args:
+            eval_config (dict[str, Any]):
+                The configuration to be used in the objective function.
+            fidels (dict[str, int | float] | None):
+                The fidelities to be used in the objective function. Typically training epoch in deep learning.
+                If None, no-fidelity opt.
+            **data_to_scatter (Any):
+                Data to scatter across workers.
+                For example, when the objective function instance has a large file,
+                Dask, which is a typical module for parallel optimization, must serialize/deserialize
+                the objective function instances. It causes a significant bottleneck.
+                By using dask.scatter, we can avoid this problem and this kwargs serves for this purpose.
+                Note that since the handling of parallel workers vary depending on packages,
+                users must adapt by themselves.
+
+        Returns:
+            results (dict[str, float]):
+                The results of the objective function given the inputs.
+                It must have `objective metric` and `runtime` at least.
+                Otherwise, any other metrics are optional.
+        """
+        return self._main_wrapper(eval_config=eval_config, fidels=fidels, **data_to_scatter)
+
+    def simulate(self, opt: AbstractAskTellOptimizer) -> None:
+        """
+        Start the simulation using only the main process.
+        Unlike the other worker wrappers, each objective function will not run in parallel.
+        Instead, we internally simulate the cumulative runtime for each worker.
+        For this sake, the optimizer must take so-called ask-and-tell interface.
+        It means that optimizer can communicate with this class via `ask` and `tell` methods.
+        As long as the optimizer takes this interface, arbitrary optimizers can be used for this class.
+
+        Although this class may not be able to guarantee the exact behavior using parallel optimization,
+        this class is safer than the other wrappers because it is thread-safe.
+        Furthermore, if users want to try a large n_workers, this class is much safer and executable.
+
+        Args:
+            opt (AbstractAskTellOptimizer):
+                An optimizer that has `ask` and `tell` methods.
+                For example, if we run a sequential optimization, the expected loop looks like:
+                    for i in range(100):
+                        eval_config, fidels = opt.ask()
+                        results = obj_func(eval_config, fidels)
+                        opt.tell(eval_config, results, fidels)
+        """
+        self._main_wrapper.simulate(opt)
```

## Comparing `mfhpo_simulator-1.2.0.dist-info/LICENSE` & `mfhpo_simulator-1.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

