# Comparing `tmp/mfhpo_simulator-1.1.0-py3-none-any.whl.zip` & `tmp/mfhpo_simulator-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 18041 bytes, number of entries: 10
--rw-rw-r--  2.0 unx      483 b- defN 23-Jun-14 20:07 benchmark_simulator/__init__.py
--rw-rw-r--  2.0 unx     2845 b- defN 23-Jun-10 22:16 benchmark_simulator/_constants.py
--rw-rw-r--  2.0 unx    10604 b- defN 23-Jun-14 17:27 benchmark_simulator/_secure_proc.py
+Zip file size: 11781 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx      606 b- defN 23-Jul-01 05:59 benchmark_simulator/__init__.py
+-rw-rw-r--  2.0 unx     6226 b- defN 23-Jul-01 05:59 benchmark_simulator/_constants.py
+-rw-rw-r--  2.0 unx    11199 b- defN 23-Jul-01 05:59 benchmark_simulator/_secure_proc.py
 -rw-rw-r--  2.0 unx     1772 b- defN 23-Jun-14 22:34 benchmark_simulator/_utils.py
--rw-rw-r--  2.0 unx    29922 b- defN 23-Jun-14 19:51 benchmark_simulator/simulator.py
--rw-rw-r--  2.0 unx    10760 b- defN 23-Jun-14 22:36 mfhpo_simulator-1.1.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx      307 b- defN 23-Jun-14 22:36 mfhpo_simulator-1.1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-14 22:36 mfhpo_simulator-1.1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       20 b- defN 23-Jun-14 22:36 mfhpo_simulator-1.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      872 b- defN 23-Jun-14 22:36 mfhpo_simulator-1.1.0.dist-info/RECORD
-10 files, 57677 bytes uncompressed, 16541 bytes compressed:  71.3%
+-rw-rw-r--  2.0 unx      332 b- defN 23-Jul-01 05:59 benchmark_simulator/simulator.py
+-rw-rw-r--  2.0 unx    10760 b- defN 23-Jul-01 05:59 mfhpo_simulator-1.2.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      307 b- defN 23-Jul-01 05:59 mfhpo_simulator-1.2.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-01 05:59 mfhpo_simulator-1.2.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       20 b- defN 23-Jul-01 05:59 mfhpo_simulator-1.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      870 b- defN 23-Jul-01 05:59 mfhpo_simulator-1.2.0.dist-info/RECORD
+10 files, 32184 bytes uncompressed, 10281 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: benchmark_simulator/_utils.py
 Comment: 
 
 Filename: benchmark_simulator/simulator.py
 Comment: 
 
-Filename: mfhpo_simulator-1.1.0.dist-info/LICENSE
+Filename: mfhpo_simulator-1.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: mfhpo_simulator-1.1.0.dist-info/METADATA
+Filename: mfhpo_simulator-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: mfhpo_simulator-1.1.0.dist-info/WHEEL
+Filename: mfhpo_simulator-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: mfhpo_simulator-1.1.0.dist-info/top_level.txt
+Filename: mfhpo_simulator-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: mfhpo_simulator-1.1.0.dist-info/RECORD
+Filename: mfhpo_simulator-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## benchmark_simulator/__init__.py

```diff
@@ -1,13 +1,19 @@
-from benchmark_simulator._constants import ObjectiveFuncType
-from benchmark_simulator.simulator import CentralWorkerManager, ObjectiveFuncWorker
+from benchmark_simulator._constants import AbstractAskTellOptimizer, ObjectiveFuncType
+from benchmark_simulator.simulator import AskTellWorkerManager, CentralWorkerManager, ObjectiveFuncWorker
 
 
-__version__ = "1.1.0"
+__version__ = "1.2.0"
 __copyright__ = "Copyright (C) 2023 Shuhei Watanabe"
 __licence__ = "Apache-2.0 License"
 __author__ = "Shuhei Watanabe"
 __author_email__ = "shuhei.watanabe.utokyo@gmail.com"
 __url__ = "https://github.com/nabenabe0928/mfhpo-simulator"
 
 
-__all__ = ["CentralWorkerManager", "ObjectiveFuncType", "ObjectiveFuncWorker"]
+__all__ = [
+    "AbstractAskTellOptimizer",
+    "AskTellWorkerManager",
+    "CentralWorkerManager",
+    "ObjectiveFuncType",
+    "ObjectiveFuncWorker",
+]
```

## benchmark_simulator/_constants.py

```diff
@@ -1,59 +1,164 @@
 from __future__ import annotations
 
 import os
+from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any, Final, Protocol
 
+import numpy as np
+
 
 DIR_NAME: Final[str] = "mfhpo-simulator-info/"
 INF: Final[float] = float(1 << 30)
 
 
 @dataclass(frozen=True)
 class _TimeStampDictType:
     prev_timestamp: float
     waited_time: float
 
 
 @dataclass(frozen=True)
+class _TimeNowDictType:
+    before_sample: float
+    after_sample: float
+
+
+@dataclass(frozen=True)
 class _StateType:
     runtime: float = 0.0
     cumtime: float = 0.0
     fidel: int = 0
     seed: int | None = None
 
 
 @dataclass(frozen=True)
 class _InfoPaths:
     proc_alloc: str
     result: str
     state_cache: str
     worker_cumtime: str
     timestamp: str
+    timenow: str
 
 
-class _SharedDataLocations(Enum):
+@dataclass(frozen=True)
+class _ResultData:
+    cumtime: float
+    eval_config: dict[str, Any]
+    results: dict[str, float]
+    fidels: dict[str, int | float]
+    seed: int | None
+
+
+class _SharedDataFileNames(Enum):
     proc_alloc: str = "proc_alloc.json"
     result: str = "results.json"
     state_cache: str = "state_cache.json"
     worker_cumtime: str = "simulated_cumtime.json"
     timestamp: str = "timestamp.json"
+    timenow: str = "timenow.json"
 
 
 @dataclass(frozen=True)
 class _TimeValue:
     terminated: float = float(1 << 40)
     crashed: float = float(1 << 41)
 
 
+@dataclass(frozen=True)
+class _WrapperVars:
+    subdir_name: str
+    n_workers: int
+    obj_func: ObjectiveFuncType
+    n_actual_evals_in_opt: int
+    n_evals: int
+    obj_keys: list[str]
+    runtime_key: str
+    fidel_keys: list[str] | None
+    seed: int | None
+    continual_max_fidel: int | None
+    max_waiting_time: float
+    check_interval_time: float
+    store_config: bool
+
+    def validate(self) -> None:
+        if self.n_actual_evals_in_opt < self.n_workers + self.n_evals:
+            threshold = self.n_workers + self.n_evals
+            # In fact, n_workers + n_evals - 1 is the real minimum threshold.
+            raise ValueError(
+                "Cannot guarantee that optimziers will not hang. "
+                f"Use n_actual_evals_in_opt >= {threshold} (= n_evals + n_workers) at least. "
+                "Note that our package cannot change your optimizer setting, so "
+                "make sure that you changed your optimizer setting, but not only `n_actual_evals_in_opt`."
+            )
+
+
+@dataclass(frozen=True)
+class _WorkerVars:
+    continual_eval: bool
+    worker_id: str
+    worker_index: int
+    rng: np.random.RandomState
+    use_fidel: bool
+    stored_obj_keys: list[str]
+
+
 _TIME_VALUES = _TimeValue()
 
 
+class AbstractAskTellOptimizer(metaclass=ABCMeta):
+    @abstractmethod
+    def ask(self) -> tuple[dict[str, Any], dict[str, int | float] | None]:
+        """
+        The ask method to sample a configuration using an optimizer.
+
+        Args:
+            None
+
+        Returns:
+            (eval_config, fidels) (tuple[dict[str, Any], dict[str, int | float] | None]):
+                * eval_config (dict[str, Any]):
+                    The configuration to evaluate.
+                    The key is the hyperparameter name and its value is the corresponding hyperparameter value.
+                    For example, when returning {"alpha": 0.1, "beta": 0.3}, the objective function evaluates
+                    the hyperparameter configuration with alpha=0.1 and beta=0.3.
+                * fidels (dict[str, int | float] | None):
+                    The fidelity parameters to be used for the evaluation of the objective function.
+                    If not multi-fidelity optimization, simply return None.
+        """
+        raise NotImplementedError
+
+    @abstractmethod
+    def tell(
+        self,
+        eval_config: dict[str, Any],
+        results: dict[str, float],
+        *,
+        fidels: dict[str, int | float] | None,
+    ) -> None:
+        """
+        The tell method to register for a tuple of configuration, fidelity, and the results to an optimizer.
+
+        Args:
+            eval_config (dict[str, Any]):
+                The evaluated configuration.
+            results (dict[str, float]):
+                The dict of the return values from the objective function.
+            fidels (dict[str, int | float] | None):
+                The fidelity parameters used in the evaluation.
+
+        Returns:
+            None
+        """
+        raise NotImplementedError
+
+
 class ObjectiveFuncType(Protocol):
     def __call__(
         self,
         eval_config: dict[str, Any],
         *,
         fidels: dict[str, int | float] | None = None,
         seed: int | None = None,
@@ -84,8 +189,8 @@
                 It must have `objective metric` and `runtime` at least.
                 Otherwise, any other metrics are optional.
         """
         raise NotImplementedError
 
 
 def _get_file_paths(dir_name: str) -> _InfoPaths:
-    return _InfoPaths(**{fn.name: os.path.join(dir_name, fn.value) for fn in _SharedDataLocations})
+    return _InfoPaths(**{fn.name: os.path.join(dir_name, fn.value) for fn in _SharedDataFileNames})
```

## benchmark_simulator/_secure_proc.py

```diff
@@ -2,28 +2,29 @@
 
 import fcntl
 import os
 import time
 import warnings
 
 from benchmark_simulator._constants import (
-    _SharedDataLocations,
+    _SharedDataFileNames,
     _StateType,
     _TIME_VALUES,
+    _TimeNowDictType,
     _TimeStampDictType,
 )
 from benchmark_simulator._utils import _SecureLock
 
 import numpy as np
 
 import ujson as json  # type: ignore
 
 
 def _init_simulator(dir_name: str) -> None:
-    for fn in _SharedDataLocations:
+    for fn in _SharedDataFileNames:
         path = os.path.join(dir_name, fn.value)
         with open(path, "a+") as f:
             fcntl.flock(f.fileno(), fcntl.LOCK_EX)
             f.seek(0)
             content = f.read()
             if len(content) < 2:
                 f.seek(0)
@@ -48,14 +49,27 @@
         alloc = {pid: idx for idx, pid in enumerate(sorted_pids)}
         f.seek(0)
         json.dump(alloc, f, indent=4)
 
     return alloc
 
 
+def _record_timenow(path: str, timenow_data: _TimeNowDictType, lock: _SecureLock) -> None:
+    with lock.edit(path) as f:
+        record = json.load(f)
+        for k, v in timenow_data.__dict__.items():
+            if k not in record:
+                record[k] = [v]
+            else:
+                record[k].append(v)
+
+        f.seek(0)
+        json.dump(record, f, indent=4)
+
+
 def _record_cumtime(path: str, worker_id: str, cumtime: float, lock: _SecureLock) -> None:
     with lock.edit(path) as f:
         record = json.load(f)
         prev_cumtime = record.get(worker_id, 0.0)
         record[worker_id] = np.clip(cumtime, a_min=prev_cumtime, a_max=_TIME_VALUES.crashed)
         f.seek(0)
         json.dump(record, f, indent=4)
@@ -102,14 +116,21 @@
 def _fetch_cache_states(path: str, config_hash: int, lock: _SecureLock) -> list[_StateType]:
     with lock.read(path) as f:
         states = json.load(f).get(str(config_hash), [])
 
     return [_StateType(runtime=state[0], cumtime=state[1], fidel=state[2], seed=state[3]) for state in states]
 
 
+def _fetch_timenow(path: str, lock: _SecureLock) -> dict[str, np.ndarray]:
+    with lock.read(path) as f:
+        data = {k: np.asarray(v) for k, v in json.load(f).items()}
+
+    return data
+
+
 def _fetch_cumtimes(path: str, lock: _SecureLock) -> dict[str, float]:
     with lock.read(path) as f:
         cumtimes = json.load(f)
 
     return cumtimes
```

## benchmark_simulator/simulator.py

```diff
@@ -1,666 +1,6 @@
-""" A collection of utilities for a simulation of multi-fidelity optimizations.
+from benchmark_simulator._simulator._worker import ObjectiveFuncWorker
+from benchmark_simulator._simulator._worker_manager import CentralWorkerManager
+from benchmark_simulator._simulator._worker_manager_for_ask_and_tell import AskTellWorkerManager
 
-In multi-fidelity optimizations, as we often evaluate configs in parallel,
-it is essential to manage the order of config allocations to each worker.
-We allow such appropriate allocations with the utilities in this file.
-To guarantee the safety, we share variables with each process using the file system.
 
-We first define some terminologies:
-* simulator: A system that manages simulated runtimes to allow optimizations of a tabular/surrogate benchmark
-             without waiting for actual runtimes.
-* worker: Worker instantiates an objective function with a given config and evaluates it.
-* proc: Each worker will be instantiated in each process.
-* worker_id: The time hash generated for each worker.
-* pid or proc_id: The process ID for each proc obtained by `os.getpid()`, which is an integer.
-* index: The index of each worker. (it will be one of the integers in [0, N - 1] where N is the # of workers.)
-
-Now we describe each file shared with each process.
-Note that each file takes the json-dict format and we write down as follows:
-    * key1 -- val1
-    * key2 -- val2
-    :
-    * keyN -- valN
-
-1. mfhpo-simulator-info/*/proc_alloc.json
-    * proc1_id -- worker1_id
-    * proc2_id -- worker2_id
-    :
-    * procN_id -- workerN_id
-Note that we need this file only if we have multiple processes in one run.
-For example, when we use multiprocessing, we might need it.
-`procX_id` is fetched by `os.getpid()` and `workerX_id` is initially generated by `generate_time_hash()`.
-
-2. mfhpo-simulator-info/*/results.json
-    * obj1_name -- list[obj1 at the n-th evaluation]
-    * obj2_name -- list[obj2 at the n-th evaluation]
-    :
-    * objM_name -- list[objM at the n-th evaluation]
-    * cumtime -- list[cumtime up to the n-th evaluation]
-    * index -- list[the index of the worker of the n-th evaluation]
-This file is necessary for post-hoc analysis.
-
-3. mfhpo-simulator-info/*/state_cache.json
-    * config1 -- list[tuple[runtime, cumtime, fidel, seed]]
-    * config2 -- list[tuple[runtime, cumtime, fidel, seed]]
-    :
-    * configN -- list[tuple[runtime, cumtime, fidel, seed]]
-This file tells you the states of each config.
-Runtime tells how long it took to evaluate configX up to the intermediate result.
-Since we would like to use this information only for the restart of trainings,
-we discard the information after each config reaches the full-fidelity training.
-Each list gets more than two elements if evaluations of the same configs happen.
-
-4. mfhpo-simulator-info/*/simulated_cumtime.json
-    * worker1_id -- cumtime1
-    * worker2_id -- cumtime2
-    :
-    * workerN_id -- cumtimeN
-This file tells you how much time each worker virtually spends in the simulation
-and we need this information to manage the order of job allocations to each worker.
-
-5. mfhpo-simulator-info/*/timestamp.json
-    * worker1_id -- {"prev_timestamp": prev_timestamp1, "waited_time": waited_time1}
-    * worker1_id -- {"prev_timestamp": prev_timestamp2, "waited_time": waited_time2}
-    :
-    * workerN_id -- {"prev_timestamp": prev_timestampN, "waited_time": waited_timeN}
-This file tells the last checkpoint timestamp of each worker (prev_timestamp) and
-how much time each worker waited for other workers in the last call.
-"""
-from __future__ import annotations
-
-import os
-import threading
-import time
-from abc import ABCMeta, abstractmethod
-from dataclasses import dataclass
-from multiprocessing import Pool
-from typing import Any
-
-from benchmark_simulator._constants import (
-    DIR_NAME,
-    INF,
-    ObjectiveFuncType,
-    _StateType,
-    _TIME_VALUES,
-    _TimeStampDictType,
-    _get_file_paths,
-)
-from benchmark_simulator._secure_proc import (
-    _allocate_proc_to_worker,
-    _cache_state,
-    _delete_state,
-    _fetch_cache_states,
-    _fetch_cumtimes,
-    _fetch_proc_alloc,
-    _fetch_timestamps,
-    _finish_worker_timer,
-    _init_simulator,
-    _is_allocation_ready,
-    _is_simulator_terminated,
-    _record_cumtime,
-    _record_result,
-    _record_timestamp,
-    _start_timestamp,
-    _start_worker_timer,
-    _wait_all_workers,
-    _wait_proc_allocation,
-    _wait_until_next,
-)
-from benchmark_simulator._utils import _SecureLock, _generate_time_hash
-
-import numpy as np
-
-
-@dataclass(frozen=True)
-class _WrapperVars:
-    subdir_name: str
-    n_workers: int
-    obj_func: ObjectiveFuncType
-    n_actual_evals_in_opt: int
-    n_evals: int
-    obj_keys: list[str]
-    runtime_key: str
-    fidel_keys: list[str] | None
-    seed: int | None
-    continual_max_fidel: int | None
-    max_waiting_time: float
-    check_interval_time: float
-    store_config: bool
-
-
-@dataclass(frozen=True)
-class _WorkerVars:
-    continual_eval: bool
-    worker_id: str
-    worker_index: int
-    rng: np.random.RandomState
-    use_fidel: bool
-    stored_obj_keys: list[str]
-
-
-class _BaseWrapperInterface(metaclass=ABCMeta):
-    """A base wrapper class for each worker or manager.
-    This wrapper class serves the shared interface of worker and manager class.
-
-    Attributes:
-        dir_name (str):
-            The directory name where all the information will be stored.
-        obj_keys (list[str]):
-            The objective (or constraint) names that will be stored in the result file.
-        runtime_key (str):
-            The runtime name that will be used for the scheduling.
-        fidel_keys (list[str]):
-            The fidelity names that will be used in the input `fidels`.
-    """
-
-    def __init__(
-        self,
-        subdir_name: str,
-        n_workers: int,
-        obj_func: ObjectiveFuncType,
-        n_actual_evals_in_opt: int,
-        n_evals: int,
-        fidel_keys: list[str] | None = None,
-        obj_keys: list[str] | None = None,
-        runtime_key: str = "runtime",
-        seed: int | None = None,
-        continual_max_fidel: int | None = None,
-        max_waiting_time: float = np.inf,
-        check_interval_time: float = 1e-4,
-        store_config: bool = False,
-    ):
-        """The initialization of a wrapper class.
-
-        Both ObjectiveFuncWorker and CentralWorkerManager have the same interface and the same set of control params.
-
-        Args:
-            subdir_name (str):
-                The subdirectory name to store all running information.
-            n_workers (int):
-                The number of workers to use. In other words, how many parallel workers to use.
-            obj_func (ObjectiveFuncType):
-                A callable object that serves as the objective function.
-                Args:
-                    eval_config: dict[str, Any]
-                    fidels: dict[str, int | float] | None
-                    seed: int | None
-                    **data_to_scatter: Any
-                Returns:
-                    results: dict[str, float]
-                        It must return `objective metric` and `runtime` at least.
-            n_actual_evals_in_opt (int):
-                The number of evaluations that optimizers do and it is used only for raising an error in init.
-                Note that the number of evaluations means
-                how many times we call the objective function during the optimization.
-                This number is needed to automatically finish the worker class.
-                We cannot know the timing of the termination without this information, and thus optimizers hang.
-            n_evals (int):
-                How many configurations we would like to collect.
-                More specifically, how many times we call the objective function during the optimization.
-                We can guarantee that `results.json` has at least this number of evaluations.
-            fidel_keys (list[str] | None):
-                The fidelity names to be used in the objective function.
-                If None, we assume that no fidelity is used.
-            obj_keys (list[str] | None):
-                The keys of the objective metrics used in `results` returned by func.
-            runtime_key (str):
-                The key of the runtime metric used in `results` returned by func.
-            seed (int | None):
-                The random seed to be used to allocate random seed to each call.
-            continual_max_fidel (int | None):
-                The maximum fidelity to used in continual evaluations.
-                This is valid only if we use a single fidelity.
-                If not None, each call is a continuation from the call with the same eval_config and lower fidel.
-                For example, when we already trained the objective with configA and training_epoch=10,
-                we probably would like to continue the training from epoch 10 rather than from scratch
-                for call with configA and training_epoch=30.
-                continual_eval=True calculates the runtime considers this.
-                If False, each call is considered to be processed from scratch.
-            check_interval_time (float):
-                How often each worker should check whether they could be assigned a new job.
-                For example, if 1e-2 is specified, each worker check whether they can get a new job every 1e-2 seconds.
-                If there are many workers, too small check_interval_time may cause a big bottleneck.
-                On the other hand, a big check_interval_time spends more time for waiting.
-                By default, check_interval_time is set to a relatively small number, so users might rather want to
-                increase the number to avoid the bottleneck for many workers.
-            max_waiting_time (float):
-                The maximum waiting time to judge hang.
-                If any one of the workers does not do any updates for this amount of time, we raise TimeoutError.
-            store_config (bool):
-                Whether to store all config/fidel information.
-                The information is sorted chronologically.
-                When you do large-scale experiments, this may incur too much storage consumption.
-        """
-        self._wrapper_vars = _WrapperVars(
-            subdir_name=subdir_name,
-            n_workers=n_workers,
-            obj_func=obj_func,
-            n_actual_evals_in_opt=n_actual_evals_in_opt,
-            n_evals=n_evals,
-            fidel_keys=fidel_keys,
-            obj_keys=obj_keys if obj_keys is not None else ["loss"],
-            runtime_key=runtime_key,
-            seed=seed,
-            continual_max_fidel=continual_max_fidel,
-            max_waiting_time=max_waiting_time,
-            check_interval_time=check_interval_time,
-            store_config=store_config,
-        )
-        self._lock = _SecureLock()
-        self._dir_name = os.path.join(DIR_NAME, subdir_name)
-        self._paths = _get_file_paths(self.dir_name)
-        self._obj_keys, self._runtime_key = self._wrapper_vars.obj_keys, runtime_key
-        self._fidel_keys = [] if fidel_keys is None else fidel_keys[:]
-        self._init_wrapper()
-
-    @property
-    def dir_name(self) -> str:
-        return self._dir_name
-
-    @property
-    def obj_keys(self) -> list[str]:
-        return self._obj_keys[:]
-
-    @property
-    def runtime_key(self) -> str:
-        return self._runtime_key
-
-    @property
-    def fidel_keys(self) -> list[str]:
-        return self._fidel_keys[:]
-
-    @abstractmethod
-    def _init_wrapper(self) -> None:
-        raise NotImplementedError
-
-
-class ObjectiveFuncWorker(_BaseWrapperInterface):
-    """A worker class for each worker.
-    This worker class is supposed to be instantiated for each worker.
-    For example, if we use 4 workers for an optimization, then four instances should be created.
-    """
-
-    def __repr__(self) -> str:
-        return f"Worker-{self._worker_vars.worker_id}"
-
-    def _guarantee_no_hang(self) -> None:
-        n_workers, n_evals = self._wrapper_vars.n_workers, self._wrapper_vars.n_evals
-        n_actual_evals_in_opt = self._wrapper_vars.n_actual_evals_in_opt
-        if n_actual_evals_in_opt < n_workers + n_evals:
-            threshold = n_workers + n_evals
-            # In fact, n_workers + n_evals - 1 is the real minimum threshold.
-            raise ValueError(
-                "Cannot guarantee that optimziers will not hang. "
-                f"Use n_actual_evals_in_opt >= {threshold} (= n_evals + n_workers) at least. "
-                "Note that our package cannot change your optimizer setting, so "
-                "make sure that you changed your optimizer setting, but not only `n_actual_evals_in_opt`."
-            )
-
-    def _validate_fidel_args(self, continual_eval: bool) -> None:
-        # Guarantee the sufficiency: continual_eval ==> len(fidel_keys) == 1
-        if continual_eval and len(self._fidel_keys) != 1:
-            raise ValueError(
-                f"continual_max_fidel is valid only if fidel_keys has only one element, but got {self._fidel_keys}"
-            )
-
-    def _init_worker(self, worker_id: str) -> None:
-        os.makedirs(self.dir_name, exist_ok=True)
-        _init_simulator(dir_name=self.dir_name)
-        _start_worker_timer(path=self._paths.worker_cumtime, worker_id=worker_id, lock=self._lock)
-
-    def _alloc_index(self, worker_id: str) -> int:
-        worker_id_to_index = _wait_all_workers(
-            path=self._paths.worker_cumtime, n_workers=self._wrapper_vars.n_workers, lock=self._lock
-        )
-        time.sleep(1e-2)  # buffer before the optimization
-        return worker_id_to_index[worker_id]
-
-    def _init_wrapper(self) -> None:
-        continual_eval = self._wrapper_vars.continual_max_fidel is not None
-        worker_id = _generate_time_hash()
-        self._guarantee_no_hang()
-        self._validate_fidel_args(continual_eval)
-        self._init_worker(worker_id)
-        worker_index = self._alloc_index(worker_id)
-        self._worker_vars = _WorkerVars(
-            continual_eval=continual_eval,
-            worker_id=worker_id,
-            worker_index=worker_index,
-            rng=np.random.RandomState(self._wrapper_vars.seed),
-            use_fidel=self._wrapper_vars.fidel_keys is not None,
-            stored_obj_keys=list(set(self.obj_keys + [self.runtime_key])),
-        )
-
-        # These variables change over time and must be either loaded from file system or updated.
-        self._cumtime = 0.0
-        self._terminated = False
-        self._crashed = False
-        self._used_config: dict[str, Any] = {}
-
-    def _validate(self, fidels: dict[str, int | float] | None) -> None:
-        if self._crashed:
-            raise InterruptedError(
-                "The simulation is interrupted due to deadlock or the dead of at least one of the workers.\n"
-                "This error could be avoided by increasing `max_waiting_time` (however, np.inf is discouraged).\n"
-            )
-        if not self._worker_vars.use_fidel and fidels is not None:
-            raise ValueError(
-                "Objective function got keyword `fidels`, but fidel_keys was not provided in worker instantiation."
-            )
-        if self._worker_vars.use_fidel and fidels is None:
-            raise ValueError(
-                "Objective function did not get keyword `fidels`, but fidel_keys was provided in worker instantiation."
-            )
-
-    def _validate_output(self, results: dict[str, float]) -> None:
-        keys_in_output = set(results.keys())
-        keys = set(self._worker_vars.stored_obj_keys)
-        if keys_in_output.intersection(keys) != keys:
-            raise KeyError(
-                f"The output of objective must be a superset of {list(keys)} specified in obj_keys and runtime_key, "
-                f"but got {results}"
-            )
-
-    @staticmethod
-    def _validate_provided_fidels(fidels: dict[str, int | float] | None) -> int:
-        if fidels is None or len(fidels.values()) != 1:
-            raise ValueError(
-                f"fidels must have only one element when continual_max_fidel is provided, but got {fidels}"
-            )
-
-        fidel = next(iter(fidels.values()))
-        if not isinstance(fidel, int):
-            raise ValueError(f"Fidelity for continual evaluation must be integer, but got {fidel}")
-        if fidel < 0:
-            raise ValueError(f"Fidelity for continual evaluation must be non-negative, but got {fidel}")
-
-        return fidel
-
-    def _get_cached_state_and_index(self, config_hash: int, fidel: int) -> tuple[_StateType, int | None]:
-        cached_states = _fetch_cache_states(path=self._paths.state_cache, config_hash=config_hash, lock=self._lock)
-        intermediate_avail = [state.cumtime <= self._cumtime and state.fidel < fidel for state in cached_states]
-        cached_state_index = intermediate_avail.index(True) if any(intermediate_avail) else None
-        if cached_state_index is None:
-            # initial seed, note: 1 << 30 is a huge number that fits 32bit.
-            init_state = _StateType(seed=self._worker_vars.rng.randint(1 << 30))
-            return init_state, None
-        else:
-            return cached_states[cached_state_index], cached_state_index
-
-    def _update_state(
-        self,
-        config_hash: int,
-        fidel: int,
-        total_runtime: float,
-        seed: int | None,
-        cached_state_index: int | None,
-    ) -> None:
-        kwargs = dict(path=self._paths.state_cache, config_hash=config_hash, lock=self._lock)
-        if fidel != self._wrapper_vars.continual_max_fidel:  # update the cache data
-            new_state = _StateType(runtime=total_runtime, cumtime=self._cumtime, fidel=fidel, seed=seed)
-            _cache_state(new_state=new_state, update_index=cached_state_index, **kwargs)  # type: ignore[arg-type]
-        elif cached_state_index is not None:  # if None, newly start and train till the end, so no need to delete.
-            _delete_state(index=cached_state_index, **kwargs)  # type: ignore[arg-type]
-
-    def _wait_other_workers(self) -> None:
-        """
-        Wait until the worker's cumulative runtime becomes the smallest.
-        The smallest cumulative runtime implies that the order in the record will not disturbed
-        even if the worker reports its results now.
-        """
-        wait_start, worker_id = time.time(), self._worker_vars.worker_id
-        max_waiting_time = self._wrapper_vars.max_waiting_time
-        _wait_until_next(
-            path=self._paths.worker_cumtime,
-            worker_id=worker_id,
-            max_waiting_time=max_waiting_time,
-            waiting_time=self._wrapper_vars.check_interval_time,
-            lock=self._lock,
-        )
-        _record_timestamp(
-            path=self._paths.timestamp,
-            worker_id=worker_id,
-            prev_timestamp=time.time(),
-            waited_time=time.time() - wait_start,
-            lock=self._lock,
-        )
-
-    def _query_obj_func(
-        self,
-        eval_config: dict[str, Any],
-        fidels: dict[str, int | float] | None,
-        seed: int | None,
-        **data_to_scatter: Any,
-    ) -> dict[str, float]:
-        if self._wrapper_vars.store_config:
-            self._used_config = eval_config.copy()
-            self._used_config.update(**(fidels if fidels is not None else {}), seed=seed)
-
-        return self._wrapper_vars.obj_func(eval_config=eval_config, fidels=fidels, seed=seed, **data_to_scatter)
-
-    def _proc_output_from_scratch(
-        self, eval_config: dict[str, Any], fidels: dict[str, int | float] | None, **data_to_scatter: Any
-    ) -> dict[str, float]:
-        _fidels: dict[str, int | float] = {} if fidels is None else fidels.copy()
-        if self._worker_vars.use_fidel and set(_fidels.keys()) != set(self._fidel_keys):
-            raise KeyError(f"The keys in fidels must be identical to fidel_keys, but got {fidels}")
-
-        seed = self._worker_vars.rng.randint(1 << 30)
-        results = self._query_obj_func(eval_config=eval_config, seed=seed, fidels=fidels, **data_to_scatter)
-        self._validate_output(results)
-        self._cumtime += results[self.runtime_key]
-        return {k: results[k] for k in self._worker_vars.stored_obj_keys}
-
-    def _proc_output_from_existing_state(
-        self, eval_config: dict[str, Any], fidel: int, **data_to_scatter: Any
-    ) -> dict[str, float]:
-        config_hash: int = hash(str(eval_config))
-        cached_state, cached_state_index = self._get_cached_state_and_index(config_hash=config_hash, fidel=fidel)
-        _fidels: dict[str, int | float] = {self._fidel_keys[0]: fidel}
-        results = self._query_obj_func(
-            eval_config=eval_config, seed=cached_state.seed, fidels=_fidels, **data_to_scatter
-        )
-        self._validate_output(results)
-        total_runtime = results[self.runtime_key]
-        actual_runtime = max(0.0, total_runtime - cached_state.runtime)
-        self._cumtime += actual_runtime
-        self._update_state(
-            total_runtime=total_runtime,
-            cached_state_index=cached_state_index,
-            seed=cached_state.seed,
-            config_hash=config_hash,
-            fidel=fidel,
-        )
-        return {**{k: results[k] for k in self._obj_keys}, self.runtime_key: actual_runtime}
-
-    def _proc_output(
-        self, eval_config: dict[str, Any], fidels: dict[str, int | float] | None, **data_to_scatter: Any
-    ) -> dict[str, float]:
-        if not self._worker_vars.continual_eval:
-            return self._proc_output_from_scratch(eval_config=eval_config, fidels=fidels, **data_to_scatter)
-
-        # Otherwise, we try the continual evaluation
-        fidel = self._validate_provided_fidels(fidels)
-        return self._proc_output_from_existing_state(eval_config=eval_config, fidel=fidel, **data_to_scatter)
-
-    def _post_proc(self, results: dict[str, float]) -> None:
-        # First, record the simulated cumulative runtime after calling the objective
-        _record_cumtime(
-            path=self._paths.worker_cumtime,
-            worker_id=self._worker_vars.worker_id,
-            cumtime=self._cumtime,
-            lock=self._lock,
-        )
-        # Wait till the cumulative runtime becomes the smallest
-        self._wait_other_workers()
-
-        row = dict(
-            cumtime=self._cumtime,
-            worker_index=self._worker_vars.worker_index,
-            **{k: results[k] for k in self._obj_keys},
-            **self._used_config,
-        )
-        # Record the results to the main database when the cumulative runtime is the smallest
-        _record_result(
-            self._paths.result, results=row, fixed=bool(not self._wrapper_vars.store_config), lock=self._lock
-        )
-        self._used_config = {}  # Make it empty
-        if _is_simulator_terminated(self._paths.result, max_evals=self._wrapper_vars.n_evals, lock=self._lock):
-            self._finish()
-
-    def _load_timestamps(self) -> _TimeStampDictType:
-        timestamp_dict = _fetch_timestamps(self._paths.timestamp, lock=self._lock)
-        worker_id = self._worker_vars.worker_id
-        if worker_id not in timestamp_dict:  # Initialize the timestamp
-            init_timestamp = _TimeStampDictType(prev_timestamp=time.time(), waited_time=0.0)
-            _start_timestamp(
-                path=self._paths.timestamp,
-                worker_id=worker_id,
-                prev_timestamp=init_timestamp.prev_timestamp,
-                lock=self._lock,
-            )
-            return init_timestamp
-
-        timestamp = timestamp_dict[worker_id]
-        self._cumtime = _fetch_cumtimes(self._paths.worker_cumtime, lock=self._lock)[worker_id]
-        self._terminated = self._cumtime >= _TIME_VALUES.terminated - 1e-5
-        self._crashed = self._cumtime >= _TIME_VALUES.crashed - 1e-5
-        return timestamp
-
-    def __call__(
-        self,
-        eval_config: dict[str, Any],
-        *,
-        fidels: dict[str, int | float] | None = None,
-        **data_to_scatter: Any,
-    ) -> dict[str, float]:
-        """The method to close the worker instance.
-        This method must be called before we finish the optimization.
-        If not called, optimization modules are likely to hang at the end.
-
-        Args:
-            eval_config (dict[str, Any]):
-                The configuration to be used in the objective function.
-            fidels (dict[str, int | float] | None):
-                The fidelities to be used in the objective function. Typically training epoch in deep learning.
-                If None, no-fidelity opt.
-            **data_to_scatter (Any):
-                Data to scatter across workers.
-                For example, when the objective function instance has a large file,
-                Dask, which is a typical module for parallel optimization, must serialize/deserialize
-                the objective function instances. It causes a significant bottleneck.
-                By using dask.scatter, we can avoid this problem and this kwargs serves for this purpose.
-                Note that since the handling of parallel workers vary depending on packages,
-                users must adapt by themselves.
-
-        Returns:
-            results (dict[str, float]):
-                The results of the objective function given the inputs.
-                It must have `objective metric` and `runtime` at least.
-                Otherwise, any other metrics are optional.
-        """
-        timestamp = self._load_timestamps()
-        self._validate(fidels=fidels)
-        if self._terminated:
-            return {**{k: INF for k in self._obj_keys}, self.runtime_key: INF}
-
-        sampling_time = max(0.0, time.time() - timestamp.prev_timestamp - timestamp.waited_time)
-        self._cumtime += sampling_time
-
-        results = self._proc_output(eval_config, fidels, **data_to_scatter)
-        self._post_proc(results)
-        return results
-
-    def _finish(self) -> None:
-        """The method to close the worker instance.
-        This method must be called before we finish the optimization.
-        If not called, optimization modules are likely to hang.
-        """
-        _finish_worker_timer(path=self._paths.worker_cumtime, worker_id=self._worker_vars.worker_id, lock=self._lock)
-        self._terminated = True
-
-
-class CentralWorkerManager(_BaseWrapperInterface):
-    """A central worker manager class.
-    This class is supposed to be instantiated if the optimizer module uses multiprocessing.
-    For example, Dask, multiprocessing, and joblib would need this class.
-    This class recognizes each worker by process ID.
-    Therefore, process ID for each worker must be always unique and identical.
-    """
-
-    def _init_wrapper(self) -> None:
-        self._workers: list[ObjectiveFuncWorker]
-        self._main_pid = os.getpid()
-        self._init_workers()
-        self._pid_to_index: dict[int, int] = {}
-
-    def _init_workers(self) -> None:
-        if os.path.exists(self.dir_name):
-            raise FileExistsError(f"The directory `{self.dir_name}` already exists. Remove it first.")
-
-        pool = Pool()
-        results = []
-        for _ in range(self._wrapper_vars.n_workers):
-            results.append(pool.apply_async(ObjectiveFuncWorker, kwds=self._wrapper_vars.__dict__))
-
-        pool.close()
-        pool.join()
-        self._workers = [result.get() for result in results]
-
-    def _init_alloc(self, pid: int) -> None:
-        path = self._paths.proc_alloc
-        if not _is_allocation_ready(path=path, n_workers=self._wrapper_vars.n_workers, lock=self._lock):
-            _allocate_proc_to_worker(path=path, pid=pid, lock=self._lock)
-            self._pid_to_index = _wait_proc_allocation(
-                path=path, n_workers=self._wrapper_vars.n_workers, lock=self._lock
-            )
-        else:
-            self._pid_to_index = _fetch_proc_alloc(path=path, lock=self._lock)
-
-    def __call__(
-        self,
-        eval_config: dict[str, Any],
-        *,
-        fidels: dict[str, int | float] | None = None,
-        **data_to_scatter: Any,
-    ) -> dict[str, float]:
-        """The meta-wrapper method of the objective function method in WorkerFunc instances.
-
-        This method recognizes each WorkerFunc by process ID and call the corresponding worker based on the ID.
-
-        Args:
-            eval_config (dict[str, Any]):
-                The configuration to be used in the objective function.
-            fidels (dict[str, int | float] | None):
-                The fidelities to be used in the objective function. Typically training epoch in deep learning.
-                If None, no-fidelity opt.
-            **data_to_scatter (Any):
-                Data to scatter across workers.
-                For example, when the objective function instance has a large file,
-                Dask, which is a typical module for parallel optimization, must serialize/deserialize
-                the objective function instances. It causes a significant bottleneck.
-                By using dask.scatter, we can avoid this problem and this kwargs serves for this purpose.
-                Note that since the handling of parallel workers vary depending on packages,
-                users must adapt by themselves.
-
-        Returns:
-            results (dict[str, float]):
-                The results of the objective function given the inputs.
-                It must have `objective metric` and `runtime` at least.
-                Otherwise, any other metrics are optional.
-        """
-        pid = os.getpid()
-        pid = threading.get_ident() if pid == self._main_pid else pid
-        if len(self._pid_to_index) != self._wrapper_vars.n_workers:
-            self._init_alloc(pid)
-
-        if pid not in self._pid_to_index:
-            raise ProcessLookupError(
-                f"An unknown process/thread with ID {pid} was specified.\n"
-                "It is likely that one of the workers crashed and a new worker was added.\n"
-                f"However, worker additions are not allowed in {self.__class__.__name__}."
-            )
-
-        worker_index = self._pid_to_index[pid]
-        results = self._workers[worker_index](eval_config=eval_config, fidels=fidels, **data_to_scatter)
-        return results
+__all__ = ["AskTellWorkerManager", "ObjectiveFuncWorker", "CentralWorkerManager"]
```

## Comparing `mfhpo_simulator-1.1.0.dist-info/LICENSE` & `mfhpo_simulator-1.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

