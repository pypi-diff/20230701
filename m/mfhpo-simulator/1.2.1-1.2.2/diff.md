# Comparing `tmp/mfhpo_simulator-1.2.1-py3-none-any.whl.zip` & `tmp/mfhpo_simulator-1.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,17 @@
-Zip file size: 33910 bytes, number of entries: 21
--rw-rw-r--  2.0 unx      560 b- defN 23-Jul-01 06:00 benchmark_simulator/__init__.py
+Zip file size: 26041 bytes, number of entries: 15
+-rw-rw-r--  2.0 unx      560 b- defN 23-Jul-01 06:46 benchmark_simulator/__init__.py
 -rw-rw-r--  2.0 unx     6127 b- defN 23-Jul-01 05:59 benchmark_simulator/_constants.py
 -rw-rw-r--  2.0 unx    11227 b- defN 23-Jul-01 05:59 benchmark_simulator/_secure_proc.py
 -rw-rw-r--  2.0 unx     1772 b- defN 23-Jun-14 22:34 benchmark_simulator/_utils.py
 -rw-rw-r--  2.0 unx    20853 b- defN 23-Jul-01 05:59 benchmark_simulator/simulator.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Jul-01 05:59 tests/__init__.py
--rw-rw-r--  2.0 unx     3134 b- defN 23-Jul-01 05:59 tests/test_optimize.py
--rw-rw-r--  2.0 unx     4795 b- defN 23-Jul-01 05:59 tests/test_optimize_with_ask_and_tell.py
--rw-rw-r--  2.0 unx     2954 b- defN 23-Jul-01 05:59 tests/test_order_check.py
--rw-rw-r--  2.0 unx     3060 b- defN 23-Jul-01 05:59 tests/test_order_check_with_ask_and_tell.py
--rw-rw-r--  2.0 unx     5395 b- defN 23-Jul-01 05:59 tests/test_secure_proc.py
--rw-rw-r--  2.0 unx    14769 b- defN 23-Jul-01 05:59 tests/test_simulator.py
--rw-rw-r--  2.0 unx     9617 b- defN 23-Jul-01 06:00 tests/test_simulator_for_ask_and_tell.py
--rw-rw-r--  2.0 unx     5579 b- defN 23-Jul-01 05:59 tests/test_timeout_error.py
--rw-rw-r--  2.0 unx     2139 b- defN 23-Jul-01 05:59 tests/test_utils.py
--rw-rw-r--  2.0 unx     5250 b- defN 23-Jul-01 05:59 tests/utils.py
--rw-rw-r--  2.0 unx    10760 b- defN 23-Jul-01 06:03 mfhpo_simulator-1.2.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx      307 b- defN 23-Jul-01 06:03 mfhpo_simulator-1.2.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-01 06:03 mfhpo_simulator-1.2.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       26 b- defN 23-Jul-01 06:03 mfhpo_simulator-1.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1792 b- defN 23-Jul-01 06:03 mfhpo_simulator-1.2.1.dist-info/RECORD
-21 files, 110208 bytes uncompressed, 30984 bytes compressed:  71.9%
+-rw-rw-r--  2.0 unx     2544 b- defN 23-Jul-01 05:59 benchmark_simulator/_simulator/_base_wrapper.py
+-rw-rw-r--  2.0 unx     2978 b- defN 23-Jul-01 05:59 benchmark_simulator/_simulator/_utils.py
+-rw-rw-r--  2.0 unx    11790 b- defN 23-Jul-01 05:59 benchmark_simulator/_simulator/_worker.py
+-rw-rw-r--  2.0 unx     3142 b- defN 23-Jul-01 05:59 benchmark_simulator/_simulator/_worker_manager.py
+-rw-rw-r--  2.0 unx     8367 b- defN 23-Jul-01 05:59 benchmark_simulator/_simulator/_worker_manager_for_ask_and_tell.py
+-rw-rw-r--  2.0 unx    10760 b- defN 23-Jul-01 06:48 mfhpo_simulator-1.2.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      307 b- defN 23-Jul-01 06:48 mfhpo_simulator-1.2.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-01 06:48 mfhpo_simulator-1.2.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       51 b- defN 23-Jul-01 06:48 mfhpo_simulator-1.2.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1401 b- defN 23-Jul-01 06:48 mfhpo_simulator-1.2.2.dist-info/RECORD
+15 files, 81971 bytes uncompressed, 23675 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -9,56 +9,38 @@
 
 Filename: benchmark_simulator/_utils.py
 Comment: 
 
 Filename: benchmark_simulator/simulator.py
 Comment: 
 
-Filename: tests/__init__.py
+Filename: benchmark_simulator/_simulator/_base_wrapper.py
 Comment: 
 
-Filename: tests/test_optimize.py
+Filename: benchmark_simulator/_simulator/_utils.py
 Comment: 
 
-Filename: tests/test_optimize_with_ask_and_tell.py
+Filename: benchmark_simulator/_simulator/_worker.py
 Comment: 
 
-Filename: tests/test_order_check.py
+Filename: benchmark_simulator/_simulator/_worker_manager.py
 Comment: 
 
-Filename: tests/test_order_check_with_ask_and_tell.py
+Filename: benchmark_simulator/_simulator/_worker_manager_for_ask_and_tell.py
 Comment: 
 
-Filename: tests/test_secure_proc.py
+Filename: mfhpo_simulator-1.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: tests/test_simulator.py
+Filename: mfhpo_simulator-1.2.2.dist-info/METADATA
 Comment: 
 
-Filename: tests/test_simulator_for_ask_and_tell.py
+Filename: mfhpo_simulator-1.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: tests/test_timeout_error.py
+Filename: mfhpo_simulator-1.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: tests/test_utils.py
-Comment: 
-
-Filename: tests/utils.py
-Comment: 
-
-Filename: mfhpo_simulator-1.2.1.dist-info/LICENSE
-Comment: 
-
-Filename: mfhpo_simulator-1.2.1.dist-info/METADATA
-Comment: 
-
-Filename: mfhpo_simulator-1.2.1.dist-info/WHEEL
-Comment: 
-
-Filename: mfhpo_simulator-1.2.1.dist-info/top_level.txt
-Comment: 
-
-Filename: mfhpo_simulator-1.2.1.dist-info/RECORD
+Filename: mfhpo_simulator-1.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## benchmark_simulator/__init__.py

```diff
@@ -1,12 +1,12 @@
 from benchmark_simulator._constants import AbstractAskTellOptimizer, ObjectiveFuncType
 from benchmark_simulator.simulator import ObjectiveFuncWrapper, get_multiple_wrappers
 
 
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 __copyright__ = "Copyright (C) 2023 Shuhei Watanabe"
 __licence__ = "Apache-2.0 License"
 __author__ = "Shuhei Watanabe"
 __author_email__ = "shuhei.watanabe.utokyo@gmail.com"
 __url__ = "https://github.com/nabenabe0928/mfhpo-simulator"
```

## Comparing `mfhpo_simulator-1.2.1.dist-info/LICENSE` & `mfhpo_simulator-1.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

