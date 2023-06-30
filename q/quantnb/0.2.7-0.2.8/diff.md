# Comparing `tmp/quantnb-0.2.7.tar.gz` & `tmp/quantnb-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantnb-0.2.7.tar", max compression
+gzip compressed data, was "quantnb-0.2.8.tar", max compression
```

## Comparing `quantnb-0.2.7.tar` & `quantnb-0.2.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      112 2023-06-07 12:08:16.607057 quantnb-0.2.7/README.md
--rw-r--r--   0        0        0      543 2023-06-30 23:47:02.953704 quantnb-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      280 2023-06-08 09:33:29.937029 quantnb-0.2.7/quantnb/__init__.py
--rw-r--r--   0        0        0     5857 2023-06-10 15:34:06.176901 quantnb-0.2.7/quantnb/core/backtester.py
--rw-r--r--   0        0        0     8199 2023-06-08 09:25:10.940100 quantnb-0.2.7/quantnb/core/backtester_old.py
--rw-r--r--   0        0        0       80 2023-06-08 09:25:10.940100 quantnb-0.2.7/quantnb/core/enums.py
--rw-r--r--   0        0        0     1337 2023-06-30 23:07:30.161852 quantnb-0.2.7/quantnb/helpers/S_calculate_metrics.py
--rw-r--r--   0        0        0      357 2023-06-08 09:25:10.940100 quantnb-0.2.7/quantnb/helpers/S_print_orders.py
--rw-r--r--   0        0        0      728 2023-06-08 09:25:10.940100 quantnb-0.2.7/quantnb/helpers/S_print_trades.py
--rw-r--r--   0        0        0      300 2023-06-08 09:25:10.940100 quantnb-0.2.7/quantnb/helpers/__init__.py
--rw-r--r--   0        0        0      793 2023-06-08 09:25:10.940100 quantnb-0.2.7/quantnb/helpers/analyze_trade_duration.py
--rw-r--r--   0        0        0      380 2023-06-08 09:25:10.940100 quantnb-0.2.7/quantnb/helpers/calculate_average_freq.py
--rw-r--r--   0        0        0     1038 2023-06-08 09:25:10.940100 quantnb-0.2.7/quantnb/helpers/calculate_pf_stats.py
--rw-r--r--   0        0        0      390 2023-06-08 09:25:10.940100 quantnb-0.2.7/quantnb/helpers/calculate_risk_free.py
--rw-r--r--   0        0        0      213 2023-06-08 09:25:10.940100 quantnb-0.2.7/quantnb/helpers/get_average_trade_duration.py
--rw-r--r--   0        0        0      672 2023-06-08 09:25:10.940100 quantnb-0.2.7/quantnb/helpers/get_realized_pf_value.py
--rw-r--r--   0        0        0      325 2023-06-08 09:25:10.940100 quantnb-0.2.7/quantnb/helpers/plot_lines.py
--rw-r--r--   0        0        0      731 2023-06-08 09:25:10.940100 quantnb-0.2.7/quantnb/helpers/save_to_csv.py
--rw-r--r--   0        0        0      109 2023-06-08 09:25:10.940100 quantnb-0.2.7/quantnb/indicators/EMA.py
--rw-r--r--   0        0        0      109 2023-06-08 09:25:10.940100 quantnb-0.2.7/quantnb/indicators/SMA.py
--rw-r--r--   0        0        0       79 2023-06-08 09:25:10.940100 quantnb-0.2.7/quantnb/indicators/__init__.py
--rw-r--r--   0        0        0      160 2023-06-08 09:25:10.940100 quantnb-0.2.7/quantnb/indicators/cross_below.py
--rw-r--r--   0        0        0      391 2023-06-08 09:25:10.940100 quantnb-0.2.7/quantnb/lib/__init__.py
--rw-r--r--   0        0        0     1143 2023-06-08 09:25:10.940100 quantnb-0.2.7/quantnb/lib/create_binance_dataframe.py
--rw-r--r--   0        0        0      905 2023-06-08 09:25:10.940100 quantnb-0.2.7/quantnb/lib/fetch_binance_data.py
--rw-r--r--   0        0        0      359 2023-06-08 09:25:10.940100 quantnb-0.2.7/quantnb/lib/find_files.py
--rw-r--r--   0        0        0     1127 2023-06-08 09:25:10.940100 quantnb-0.2.7/quantnb/lib/multiprocess.py
--rw-r--r--   0        0        0      889 2023-06-08 09:25:10.940100 quantnb-0.2.7/quantnb/lib/optimize.py
--rw-r--r--   0        0        0      241 2023-06-08 09:25:10.940100 quantnb-0.2.7/quantnb/lib/resample.py
--rw-r--r--   0        0        0     3103 2023-06-30 23:45:05.631988 quantnb-0.2.7/quantnb/strategies/S_base.py
--rw-r--r--   0        0        0     2245 2023-06-30 23:38:29.961758 quantnb-0.2.7/quantnb/strategies/S_test.py
--rw-r--r--   0        0        0       29 2023-06-08 09:25:10.940100 quantnb-0.2.7/quantnb/strategies/__init__.py
--rw-r--r--   0        0        0      678 2023-06-08 09:25:10.940100 quantnb-0.2.7/quantnb/tests/benchmark_multiple_assets.py
--rw-r--r--   0        0        0      698 2023-06-08 09:25:10.940100 quantnb-0.2.7/quantnb/tests/optimisation_combine_files.py
--rw-r--r--   0        0        0      906 1970-01-01 00:00:00.000000 quantnb-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      112 2023-06-07 12:08:16.607057 quantnb-0.2.8/README.md
+-rw-r--r--   0        0        0      543 2023-06-30 23:49:16.096814 quantnb-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      280 2023-06-08 09:33:29.937029 quantnb-0.2.8/quantnb/__init__.py
+-rw-r--r--   0        0        0     5857 2023-06-10 15:34:06.176901 quantnb-0.2.8/quantnb/core/backtester.py
+-rw-r--r--   0        0        0     8199 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/core/backtester_old.py
+-rw-r--r--   0        0        0       80 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/core/enums.py
+-rw-r--r--   0        0        0     1337 2023-06-30 23:07:30.161852 quantnb-0.2.8/quantnb/helpers/S_calculate_metrics.py
+-rw-r--r--   0        0        0      357 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/helpers/S_print_orders.py
+-rw-r--r--   0        0        0      728 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/helpers/S_print_trades.py
+-rw-r--r--   0        0        0      300 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/helpers/__init__.py
+-rw-r--r--   0        0        0      793 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/helpers/analyze_trade_duration.py
+-rw-r--r--   0        0        0      380 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/helpers/calculate_average_freq.py
+-rw-r--r--   0        0        0     1038 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/helpers/calculate_pf_stats.py
+-rw-r--r--   0        0        0      390 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/helpers/calculate_risk_free.py
+-rw-r--r--   0        0        0      213 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/helpers/get_average_trade_duration.py
+-rw-r--r--   0        0        0      672 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/helpers/get_realized_pf_value.py
+-rw-r--r--   0        0        0      325 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/helpers/plot_lines.py
+-rw-r--r--   0        0        0      731 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/helpers/save_to_csv.py
+-rw-r--r--   0        0        0      109 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/indicators/EMA.py
+-rw-r--r--   0        0        0      109 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/indicators/SMA.py
+-rw-r--r--   0        0        0       79 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/indicators/__init__.py
+-rw-r--r--   0        0        0      160 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/indicators/cross_below.py
+-rw-r--r--   0        0        0      391 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/lib/__init__.py
+-rw-r--r--   0        0        0     1143 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/lib/create_binance_dataframe.py
+-rw-r--r--   0        0        0      905 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/lib/fetch_binance_data.py
+-rw-r--r--   0        0        0      359 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/lib/find_files.py
+-rw-r--r--   0        0        0     1127 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/lib/multiprocess.py
+-rw-r--r--   0        0        0      889 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/lib/optimize.py
+-rw-r--r--   0        0        0      241 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/lib/resample.py
+-rw-r--r--   0        0        0     3034 2023-06-30 23:49:02.624505 quantnb-0.2.8/quantnb/strategies/S_base.py
+-rw-r--r--   0        0        0     2245 2023-06-30 23:38:29.961758 quantnb-0.2.8/quantnb/strategies/S_test.py
+-rw-r--r--   0        0        0       29 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/strategies/__init__.py
+-rw-r--r--   0        0        0      678 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/tests/benchmark_multiple_assets.py
+-rw-r--r--   0        0        0      698 2023-06-08 09:25:10.940100 quantnb-0.2.8/quantnb/tests/optimisation_combine_files.py
+-rw-r--r--   0        0        0      906 1970-01-01 00:00:00.000000 quantnb-0.2.8/PKG-INFO
```

### Comparing `quantnb-0.2.7/pyproject.toml` & `quantnb-0.2.8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quantnb"
-version = "0.2.7"
+version = "0.2.8"
 description = ""
 authors = ["Alpha <piotr@piotryordanov.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 numba = "^0.57.0"
```

### Comparing `quantnb-0.2.7/quantnb/core/backtester.py` & `quantnb-0.2.8/quantnb/core/backtester.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.7/quantnb/core/backtester_old.py` & `quantnb-0.2.8/quantnb/core/backtester_old.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.7/quantnb/helpers/S_calculate_metrics.py` & `quantnb-0.2.8/quantnb/helpers/S_calculate_metrics.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.7/quantnb/helpers/S_print_trades.py` & `quantnb-0.2.8/quantnb/helpers/S_print_trades.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.7/quantnb/helpers/analyze_trade_duration.py` & `quantnb-0.2.8/quantnb/helpers/analyze_trade_duration.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.7/quantnb/helpers/calculate_pf_stats.py` & `quantnb-0.2.8/quantnb/helpers/calculate_pf_stats.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.7/quantnb/helpers/get_realized_pf_value.py` & `quantnb-0.2.8/quantnb/helpers/get_realized_pf_value.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.7/quantnb/helpers/save_to_csv.py` & `quantnb-0.2.8/quantnb/helpers/save_to_csv.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.7/quantnb/lib/create_binance_dataframe.py` & `quantnb-0.2.8/quantnb/lib/create_binance_dataframe.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.7/quantnb/lib/fetch_binance_data.py` & `quantnb-0.2.8/quantnb/lib/fetch_binance_data.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.7/quantnb/lib/multiprocess.py` & `quantnb-0.2.8/quantnb/lib/multiprocess.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.7/quantnb/lib/optimize.py` & `quantnb-0.2.8/quantnb/lib/optimize.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.7/quantnb/strategies/S_base.py` & `quantnb-0.2.8/quantnb/strategies/S_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,20 +39,15 @@
             commissions=self.commmision, initial_capital=self.initial_capital
         )
         bt.set_data(open, high, low, close, index)
         sl = None
         if self.use_sl:
             sl = self.sl.values
 
-        bt.backtest(
-            self.entries.values,
-            self.exits.values,
-            sl,
-            False,  # use_sl,
-        )
+        bt.backtest(self.entries.values, self.exits.values, sl, use_sl)
 
         return (
             bt.final_value,
             bt.equity,
             bt.orders[: bt.order_idx, :],
             bt.trades[: bt.trade_idx, :],
         )
```

### Comparing `quantnb-0.2.7/quantnb/strategies/S_test.py` & `quantnb-0.2.8/quantnb/strategies/S_test.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.7/quantnb/tests/benchmark_multiple_assets.py` & `quantnb-0.2.8/quantnb/tests/benchmark_multiple_assets.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.7/quantnb/tests/optimisation_combine_files.py` & `quantnb-0.2.8/quantnb/tests/optimisation_combine_files.py`

 * *Files identical despite different names*

### Comparing `quantnb-0.2.7/PKG-INFO` & `quantnb-0.2.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantnb
-Version: 0.2.7
+Version: 0.2.8
 Summary: 
 Author: Alpha
 Author-email: piotr@piotryordanov.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipython (>=8.14.0,<9.0.0)
```

