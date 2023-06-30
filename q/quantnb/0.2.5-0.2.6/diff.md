# Comparing `tmp/quantnb-0.2.5.tar.gz` & `tmp/quantnb-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantnb-0.2.5.tar", max compression
+gzip compressed data, was "quantnb-0.2.6.tar", max compression
```

## Comparing `quantnb-0.2.5.tar` & `quantnb-0.2.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      112 2023-06-07 12:08:16.607057 quantnb-0.2.5/README.md
--rw-r--r--   0        0        0      543 2023-06-30 23:07:36.301930 quantnb-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      280 2023-06-08 09:33:29.937029 quantnb-0.2.5/quantnb/__init__.py
--rw-r--r--   0        0        0     5857 2023-06-10 15:34:06.176901 quantnb-0.2.5/quantnb/core/backtester.py
--rw-r--r--   0        0        0     8199 2023-06-08 09:25:10.940100 quantnb-0.2.5/quantnb/core/backtester_old.py
--rw-r--r--   0        0        0       80 2023-06-08 09:25:10.940100 quantnb-0.2.5/quantnb/core/enums.py
--rw-r--r--   0        0        0     1337 2023-06-30 23:07:30.161852 quantnb-0.2.5/quantnb/helpers/S_calculate_metrics.py
--rw-r--r--   0        0        0      357 2023-06-08 09:25:10.940100 quantnb-0.2.5/quantnb/helpers/S_print_orders.py
--rw-r--r--   0        0        0      728 2023-06-08 09:25:10.940100 quantnb-0.2.5/quantnb/helpers/S_print_trades.py
--rw-r--r--   0        0        0      300 2023-06-08 09:25:10.940100 quantnb-0.2.5/quantnb/helpers/__init__.py
--rw-r--r--   0        0        0      793 2023-06-08 09:25:10.940100 quantnb-0.2.5/quantnb/helpers/analyze_trade_duration.py
--rw-r--r--   0        0        0      380 2023-06-08 09:25:10.940100 quantnb-0.2.5/quantnb/helpers/calculate_average_freq.py
--rw-r--r--   0        0        0     1038 2023-06-08 09:25:10.940100 quantnb-0.2.5/quantnb/helpers/calculate_pf_stats.py
--rw-r--r--   0        0        0      390 2023-06-08 09:25:10.940100 quantnb-0.2.5/quantnb/helpers/calculate_risk_free.py
--rw-r--r--   0        0        0      213 2023-06-08 09:25:10.940100 quantnb-0.2.5/quantnb/helpers/get_average_trade_duration.py
--rw-r--r--   0        0        0      672 2023-06-08 09:25:10.940100 quantnb-0.2.5/quantnb/helpers/get_realized_pf_value.py
--rw-r--r--   0        0        0      325 2023-06-08 09:25:10.940100 quantnb-0.2.5/quantnb/helpers/plot_lines.py
--rw-r--r--   0        0        0      731 2023-06-08 09:25:10.940100 quantnb-0.2.5/quantnb/helpers/save_to_csv.py
--rw-r--r--   0        0        0      109 2023-06-08 09:25:10.940100 quantnb-0.2.5/quantnb/indicators/EMA.py
--rw-r--r--   0        0        0      109 2023-06-08 09:25:10.940100 quantnb-0.2.5/quantnb/indicators/SMA.py
--rw-r--r--   0        0        0       79 2023-06-08 09:25:10.940100 quantnb-0.2.5/quantnb/indicators/__init__.py
--rw-r--r--   0        0        0      160 2023-06-08 09:25:10.940100 quantnb-0.2.5/quantnb/indicators/cross_below.py
--rw-r--r--   0        0        0      391 2023-06-08 09:25:10.940100 quantnb-0.2.5/quantnb/lib/__init__.py
--rw-r--r--   0        0        0     1143 2023-06-08 09:25:10.940100 quantnb-0.2.5/quantnb/lib/create_binance_dataframe.py
--rw-r--r--   0        0        0      905 2023-06-08 09:25:10.940100 quantnb-0.2.5/quantnb/lib/fetch_binance_data.py
--rw-r--r--   0        0        0      359 2023-06-08 09:25:10.940100 quantnb-0.2.5/quantnb/lib/find_files.py
--rw-r--r--   0        0        0     1127 2023-06-08 09:25:10.940100 quantnb-0.2.5/quantnb/lib/multiprocess.py
--rw-r--r--   0        0        0      889 2023-06-08 09:25:10.940100 quantnb-0.2.5/quantnb/lib/optimize.py
--rw-r--r--   0        0        0      241 2023-06-08 09:25:10.940100 quantnb-0.2.5/quantnb/lib/resample.py
--rw-r--r--   0        0        0     3068 2023-06-30 22:37:11.121477 quantnb-0.2.5/quantnb/strategies/S_base.py
--rw-r--r--   0        0        0     2245 2023-06-08 09:33:14.890354 quantnb-0.2.5/quantnb/strategies/S_test.py
--rw-r--r--   0        0        0       29 2023-06-08 09:25:10.940100 quantnb-0.2.5/quantnb/strategies/__init__.py
--rw-r--r--   0        0        0      678 2023-06-08 09:25:10.940100 quantnb-0.2.5/quantnb/tests/benchmark_multiple_assets.py
--rw-r--r--   0        0        0      698 2023-06-08 09:25:10.940100 quantnb-0.2.5/quantnb/tests/optimisation_combine_files.py
--rw-r--r--   0        0        0      906 1970-01-01 00:00:00.000000 quantnb-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      112 2023-06-07 12:08:16.607057 quantnb-0.2.6/README.md
+-rw-r--r--   0        0        0      543 2023-06-30 23:40:37.172812 quantnb-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      280 2023-06-08 09:33:29.937029 quantnb-0.2.6/quantnb/__init__.py
+-rw-r--r--   0        0        0     5857 2023-06-10 15:34:06.176901 quantnb-0.2.6/quantnb/core/backtester.py
+-rw-r--r--   0        0        0     8199 2023-06-08 09:25:10.940100 quantnb-0.2.6/quantnb/core/backtester_old.py
+-rw-r--r--   0        0        0       80 2023-06-08 09:25:10.940100 quantnb-0.2.6/quantnb/core/enums.py
+-rw-r--r--   0        0        0     1337 2023-06-30 23:07:30.161852 quantnb-0.2.6/quantnb/helpers/S_calculate_metrics.py
+-rw-r--r--   0        0        0      357 2023-06-08 09:25:10.940100 quantnb-0.2.6/quantnb/helpers/S_print_orders.py
+-rw-r--r--   0        0        0      728 2023-06-08 09:25:10.940100 quantnb-0.2.6/quantnb/helpers/S_print_trades.py
+-rw-r--r--   0        0        0      300 2023-06-08 09:25:10.940100 quantnb-0.2.6/quantnb/helpers/__init__.py
+-rw-r--r--   0        0        0      793 2023-06-08 09:25:10.940100 quantnb-0.2.6/quantnb/helpers/analyze_trade_duration.py
+-rw-r--r--   0        0        0      380 2023-06-08 09:25:10.940100 quantnb-0.2.6/quantnb/helpers/calculate_average_freq.py
+-rw-r--r--   0        0        0     1038 2023-06-08 09:25:10.940100 quantnb-0.2.6/quantnb/helpers/calculate_pf_stats.py
+-rw-r--r--   0        0        0      390 2023-06-08 09:25:10.940100 quantnb-0.2.6/quantnb/helpers/calculate_risk_free.py
+-rw-r--r--   0        0        0      213 2023-06-08 09:25:10.940100 quantnb-0.2.6/quantnb/helpers/get_average_trade_duration.py
+-rw-r--r--   0        0        0      672 2023-06-08 09:25:10.940100 quantnb-0.2.6/quantnb/helpers/get_realized_pf_value.py
+-rw-r--r--   0        0        0      325 2023-06-08 09:25:10.940100 quantnb-0.2.6/quantnb/helpers/plot_lines.py
+-rw-r--r--   0        0        0      731 2023-06-08 09:25:10.940100 quantnb-0.2.6/quantnb/helpers/save_to_csv.py
+-rw-r--r--   0        0        0      109 2023-06-08 09:25:10.940100 quantnb-0.2.6/quantnb/indicators/EMA.py
+-rw-r--r--   0        0        0      109 2023-06-08 09:25:10.940100 quantnb-0.2.6/quantnb/indicators/SMA.py
+-rw-r--r--   0        0        0       79 2023-06-08 09:25:10.940100 quantnb-0.2.6/quantnb/indicators/__init__.py
+-rw-r--r--   0        0        0      160 2023-06-08 09:25:10.940100 quantnb-0.2.6/quantnb/indicators/cross_below.py
+-rw-r--r--   0        0        0      391 2023-06-08 09:25:10.940100 quantnb-0.2.6/quantnb/lib/__init__.py
+-rw-r--r--   0        0        0     1143 2023-06-08 09:25:10.940100 quantnb-0.2.6/quantnb/lib/create_binance_dataframe.py
+-rw-r--r--   0        0        0      905 2023-06-08 09:25:10.940100 quantnb-0.2.6/quantnb/lib/fetch_binance_data.py
+-rw-r--r--   0        0        0      359 2023-06-08 09:25:10.940100 quantnb-0.2.6/quantnb/lib/find_files.py
+-rw-r--r--   0        0        0     1127 2023-06-08 09:25:10.940100 quantnb-0.2.6/quantnb/lib/multiprocess.py
+-rw-r--r--   0        0        0      889 2023-06-08 09:25:10.940100 quantnb-0.2.6/quantnb/lib/optimize.py
+-rw-r--r--   0        0        0      241 2023-06-08 09:25:10.940100 quantnb-0.2.6/quantnb/lib/resample.py
+-rw-r--r--   0        0        0     3103 2023-06-30 23:40:14.129874 quantnb-0.2.6/quantnb/strategies/S_base.py
+-rw-r--r--   0        0        0     2245 2023-06-30 23:38:29.961758 quantnb-0.2.6/quantnb/strategies/S_test.py
+-rw-r--r--   0        0        0       29 2023-06-08 09:25:10.940100 quantnb-0.2.6/quantnb/strategies/__init__.py
+-rw-r--r--   0        0        0      678 2023-06-08 09:25:10.940100 quantnb-0.2.6/quantnb/tests/benchmark_multiple_assets.py
+-rw-r--r--   0        0        0      698 2023-06-08 09:25:10.940100 quantnb-0.2.6/quantnb/tests/optimisation_combine_files.py
+-rw-r--r--   0        0        0      906 1970-01-01 00:00:00.000000 quantnb-0.2.6/PKG-INFO
```

### Comparing `quantnb-0.2.5/pyproject.toml` & `quantnb-0.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quantnb"
-version = "0.2.5"
+version = "0.2.6"
 description = ""
 authors = ["Alpha <piotr@piotryordanov.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 numba = "^0.57.0"
```

### Comparing `quantnb-0.2.5/quantnb/core/backtester.py` & `quantnb-0.2.6/quantnb/core/backtester.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.5/quantnb/core/backtester_old.py` & `quantnb-0.2.6/quantnb/core/backtester_old.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.5/quantnb/helpers/S_calculate_metrics.py` & `quantnb-0.2.6/quantnb/helpers/S_calculate_metrics.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.5/quantnb/helpers/S_print_trades.py` & `quantnb-0.2.6/quantnb/helpers/S_print_trades.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.5/quantnb/helpers/analyze_trade_duration.py` & `quantnb-0.2.6/quantnb/helpers/analyze_trade_duration.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.5/quantnb/helpers/calculate_pf_stats.py` & `quantnb-0.2.6/quantnb/helpers/calculate_pf_stats.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.5/quantnb/helpers/get_realized_pf_value.py` & `quantnb-0.2.6/quantnb/helpers/get_realized_pf_value.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.5/quantnb/helpers/save_to_csv.py` & `quantnb-0.2.6/quantnb/helpers/save_to_csv.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.5/quantnb/lib/create_binance_dataframe.py` & `quantnb-0.2.6/quantnb/lib/create_binance_dataframe.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.5/quantnb/lib/fetch_binance_data.py` & `quantnb-0.2.6/quantnb/lib/fetch_binance_data.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.5/quantnb/lib/multiprocess.py` & `quantnb-0.2.6/quantnb/lib/multiprocess.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.5/quantnb/lib/optimize.py` & `quantnb-0.2.6/quantnb/lib/optimize.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.5/quantnb/strategies/S_base.py` & `quantnb-0.2.6/quantnb/strategies/S_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 from quantnb.core.backtester import Backtester
 import matplotlib.pyplot as plt
 
 from quantnb.helpers import save_to_csv, print_orders, print_trades, calculate_metrics
 
 
 class S_base:
-    def __init__(self, data, offset=0, commission=0.0002, initial_capital=10000):
+    def __init__(
+        self, data, offset=0, commission=0.0002, initial_capital=10000, use_sl=False
+    ):
         data = data[offset:]
 
         data.rename(
             columns={"close": "Close", "high": "High", "low": "Low", "open": "Open"},
             inplace=True,
         )
         data.index = data.index.astype(int) // 10**9
         self.data = data
         self.commmision = commission
         self.initial_capital = initial_capital
-        self.use_sl = False
+        self.use_sl = use_sl
 
     def simulation(self, mode, use_sl):
         close = self.data.Close
         size = np.full_like(close, 1)
         multiplier = 1
         size = size * multiplier
 
@@ -54,15 +56,15 @@
             bt.orders[: bt.order_idx, :],
             bt.trades[: bt.trade_idx, :],
         )
 
     def backtest(self, params):
         self.get_signals(params)
         (final_value, equity, orders_arr, trades_arr) = self.simulation(
-            mode=1, use_sl=False
+            mode=1, use_sl=self.use_sl
         )
         self.orders_arr = orders_arr
 
         dd, total_return, ratio, buy_and_hold = calculate_metrics(
             equity, self.data, final_value, self.initial_capital
         )
```

### Comparing `quantnb-0.2.5/quantnb/strategies/S_test.py` & `quantnb-0.2.6/quantnb/strategies/S_test.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.5/quantnb/tests/benchmark_multiple_assets.py` & `quantnb-0.2.6/quantnb/tests/benchmark_multiple_assets.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.5/quantnb/tests/optimisation_combine_files.py` & `quantnb-0.2.6/quantnb/tests/optimisation_combine_files.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.5/PKG-INFO` & `quantnb-0.2.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantnb
-Version: 0.2.5
+Version: 0.2.6
 Summary: 
 Author: Alpha
 Author-email: piotr@piotryordanov.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipython (>=8.14.0,<9.0.0)
```

