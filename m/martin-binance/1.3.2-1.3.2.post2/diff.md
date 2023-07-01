# Comparing `tmp/martin_binance-1.3.2.tar.gz` & `tmp/martin_binance-1.3.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martin_binance-1.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "martin_binance-1.3.2.post2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `martin_binance-1.3.2.tar` & `martin_binance-1.3.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1079 2023-06-29 19:06:04.244467 martin_binance-1.3.2/LICENSE
--rwxr-xr-x   0        0        0     4025 2023-06-29 19:06:04.244467 martin_binance-1.3.2/README.md
--rw-r--r--   0        0        0     2013 2023-06-29 19:06:04.288467 martin_binance-1.3.2/martin_binance/__init__.py
--rw-r--r--   0        0        0     4642 2023-06-29 19:06:04.288467 martin_binance-1.3.2/martin_binance/backtest/OoTSP.py
--rw-r--r--   0        0        0     2946 2023-06-29 19:06:04.288467 martin_binance-1.3.2/martin_binance/backtest/VCoSEL.py
--rw-r--r--   0        0        0        0 2023-06-29 19:06:04.288467 martin_binance-1.3.2/martin_binance/backtest/__init__.py
--rw-r--r--   0        0        0    14575 2023-06-29 19:06:04.288467 martin_binance-1.3.2/martin_binance/backtest/exchange_simulator.py
--rw-r--r--   0        0        0     6721 2023-06-29 19:06:04.288467 martin_binance-1.3.2/martin_binance/cli_0_BTCUSDT.py.template
--rw-r--r--   0        0        0     6716 2023-06-29 19:06:04.288467 martin_binance-1.3.2/martin_binance/cli_1_BTCUSDT.py.template
--rw-r--r--   0        0        0     6722 2023-06-29 19:06:04.288467 martin_binance-1.3.2/martin_binance/cli_2_TESTBTCTESTUSDT.py.template
--rw-r--r--   0        0        0     4707 2023-06-29 19:06:04.288467 martin_binance-1.3.2/martin_binance/client.py
--rw-r--r--   0        0        0   186112 2023-06-29 19:06:04.288467 martin_binance-1.3.2/martin_binance/executor.py
--rw-r--r--   0        0        0   237568 2023-06-29 19:06:04.288467 martin_binance-1.3.2/martin_binance/funds_rate.db.template
--rwxr-xr-x   0        0        0   337272 2023-06-29 19:06:04.292467 martin_binance-1.3.2/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so
--rw-r--r--   0        0        0      376 2023-06-29 19:06:04.292467 martin_binance-1.3.2/martin_binance/margin/margin_req.txt
--rw-r--r--   0        0        0      348 2023-06-29 19:06:04.292467 martin_binance-1.3.2/martin_binance/margin/margin_req_win.txt
--rw-r--r--   0        0        0    82924 2023-06-29 19:06:04.292467 martin_binance-1.3.2/martin_binance/margin_wrapper.py
--rw-r--r--   0        0        0     1472 2023-06-29 19:06:04.292467 martin_binance-1.3.2/martin_binance/ms_cfg.toml.template
--rw-r--r--   0        0        0      485 2023-06-29 19:06:04.292467 martin_binance-1.3.2/martin_binance/service/.tmux.conf
--rwxr-xr-x   0        0        0      319 2023-06-29 19:06:04.292467 martin_binance-1.3.2/martin_binance/service/funds_export.service
--rwxr-xr-x   0        0        0    16282 2023-06-29 19:06:04.292467 martin_binance-1.3.2/martin_binance/service/funds_rate_exporter.py
--rwxr-xr-x   0        0        0    75764 2023-06-29 19:06:04.292467 martin_binance-1.3.2/martin_binance/service/grafana.json
--rwxr-xr-x   0        0        0     1282 2023-06-29 19:06:04.292467 martin_binance-1.3.2/martin_binance/service/relaunch.py
--rwxr-xr-x   0        0        0      271 2023-06-29 19:06:04.292467 martin_binance-1.3.2/martin_binance/service/relaunch.service
--rwxr-xr-x   0        0        0      372 2023-06-29 19:06:04.292467 martin_binance-1.3.2/martin_binance/service/tmux.service
--rw-r--r--   0        0        0     1427 2023-06-29 19:06:04.292467 martin_binance-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     5320 1970-01-01 00:00:00.000000 martin_binance-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-07-01 14:30:02.560426 martin_binance-1.3.2.post2/LICENSE
+-rwxr-xr-x   0        0        0     4025 2023-07-01 14:30:02.560426 martin_binance-1.3.2.post2/README.md
+-rw-r--r--   0        0        0     2015 2023-07-01 14:30:02.604426 martin_binance-1.3.2.post2/martin_binance/__init__.py
+-rw-r--r--   0        0        0     4642 2023-07-01 14:30:02.604426 martin_binance-1.3.2.post2/martin_binance/backtest/OoTSP.py
+-rw-r--r--   0        0        0     2946 2023-07-01 14:30:02.604426 martin_binance-1.3.2.post2/martin_binance/backtest/VCoSEL.py
+-rw-r--r--   0        0        0        0 2023-07-01 14:30:02.604426 martin_binance-1.3.2.post2/martin_binance/backtest/__init__.py
+-rw-r--r--   0        0        0    14575 2023-07-01 14:30:02.604426 martin_binance-1.3.2.post2/martin_binance/backtest/exchange_simulator.py
+-rw-r--r--   0        0        0     6721 2023-07-01 14:30:02.604426 martin_binance-1.3.2.post2/martin_binance/cli_0_BTCUSDT.py.template
+-rw-r--r--   0        0        0     6716 2023-07-01 14:30:02.604426 martin_binance-1.3.2.post2/martin_binance/cli_1_BTCUSDT.py.template
+-rw-r--r--   0        0        0     6722 2023-07-01 14:30:02.604426 martin_binance-1.3.2.post2/martin_binance/cli_2_TESTBTCTESTUSDT.py.template
+-rw-r--r--   0        0        0     4707 2023-07-01 14:30:02.604426 martin_binance-1.3.2.post2/martin_binance/client.py
+-rw-r--r--   0        0        0   186091 2023-07-01 14:30:02.604426 martin_binance-1.3.2.post2/martin_binance/executor.py
+-rw-r--r--   0        0        0   237568 2023-07-01 14:30:02.608426 martin_binance-1.3.2.post2/martin_binance/funds_rate.db.template
+-rwxr-xr-x   0        0        0   337272 2023-07-01 14:30:02.608426 martin_binance-1.3.2.post2/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0      376 2023-07-01 14:30:02.608426 martin_binance-1.3.2.post2/martin_binance/margin/margin_req.txt
+-rw-r--r--   0        0        0      348 2023-07-01 14:30:02.608426 martin_binance-1.3.2.post2/martin_binance/margin/margin_req_win.txt
+-rw-r--r--   0        0        0    83511 2023-07-01 14:30:02.608426 martin_binance-1.3.2.post2/martin_binance/margin_wrapper.py
+-rw-r--r--   0        0        0     1472 2023-07-01 14:30:02.612426 martin_binance-1.3.2.post2/martin_binance/ms_cfg.toml.template
+-rw-r--r--   0        0        0      485 2023-07-01 14:30:02.612426 martin_binance-1.3.2.post2/martin_binance/service/.tmux.conf
+-rwxr-xr-x   0        0        0      319 2023-07-01 14:30:02.612426 martin_binance-1.3.2.post2/martin_binance/service/funds_export.service
+-rwxr-xr-x   0        0        0    16282 2023-07-01 14:30:02.612426 martin_binance-1.3.2.post2/martin_binance/service/funds_rate_exporter.py
+-rwxr-xr-x   0        0        0    75764 2023-07-01 14:30:02.612426 martin_binance-1.3.2.post2/martin_binance/service/grafana.json
+-rwxr-xr-x   0        0        0     1282 2023-07-01 14:30:02.612426 martin_binance-1.3.2.post2/martin_binance/service/relaunch.py
+-rwxr-xr-x   0        0        0      271 2023-07-01 14:30:02.612426 martin_binance-1.3.2.post2/martin_binance/service/relaunch.service
+-rwxr-xr-x   0        0        0      372 2023-07-01 14:30:02.612426 martin_binance-1.3.2.post2/martin_binance/service/tmux.service
+-rw-r--r--   0        0        0     1427 2023-07-01 14:30:02.612426 martin_binance-1.3.2.post2/pyproject.toml
+-rw-r--r--   0        0        0     5326 1970-01-01 00:00:00.000000 martin_binance-1.3.2.post2/PKG-INFO
```

### Comparing `martin_binance-1.3.2/LICENSE` & `martin_binance-1.3.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2/README.md` & `martin_binance-1.3.2.post2/README.md`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2/martin_binance/__init__.py` & `martin_binance-1.3.2.post2/martin_binance/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Free trading system for Binance SPOT API
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.2"
+__version__ = "1.3.2-2"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 from pathlib import Path
 from shutil import copy
 
 STANDALONE = True
```

### Comparing `martin_binance-1.3.2/martin_binance/backtest/OoTSP.py` & `martin_binance-1.3.2.post2/martin_binance/backtest/OoTSP.py`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2/martin_binance/backtest/VCoSEL.py` & `martin_binance-1.3.2.post2/martin_binance/backtest/VCoSEL.py`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2/martin_binance/backtest/exchange_simulator.py` & `martin_binance-1.3.2.post2/martin_binance/backtest/exchange_simulator.py`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2/martin_binance/cli_0_BTCUSDT.py.template` & `martin_binance-1.3.2.post2/martin_binance/cli_0_BTCUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2/martin_binance/cli_1_BTCUSDT.py.template` & `martin_binance-1.3.2.post2/martin_binance/cli_1_BTCUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2/martin_binance/cli_2_TESTBTCTESTUSDT.py.template` & `martin_binance-1.3.2.post2/martin_binance/cli_2_TESTBTCTESTUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2/martin_binance/client.py` & `martin_binance-1.3.2.post2/martin_binance/client.py`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2/martin_binance/executor.py` & `martin_binance-1.3.2.post2/martin_binance/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ####################################################################
 # Cyclic grid strategy based on martingale
 ##################################################################
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.1-3"
+__version__ = "1.3.2-2"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = 'https://github.com/DogsTailFarmer'
 ##################################################################
 import sys
 import gc
 import statistics
 from decimal import Decimal, ROUND_FLOOR, ROUND_CEILING
@@ -1237,15 +1237,15 @@
         part_amount_first = Decimal('0')
         part_amount_second = Decimal('0')
         if grid_filled:
             for v in self.part_amount.values():
                 part_amount_first += v[0]
                 part_amount_second += v[1]
         #
-        if grid_no_change and tp_no_change:
+        if STANDALONE or (grid_no_change and tp_no_change):
             if grid_hold:
                 self.message_log("Restore, no grid orders, place from hold now", tlg=True)
                 self.place_grid_part()
             elif no_orders:
                 self.restart = True
                 self.message_log("Restore, no orders, restart", tlg=True)
                 self.start()
@@ -1421,15 +1421,15 @@
             elif grid_more and self.orders_init:
                 self.message_log('Restored, some grid order(s) was placed', tlg=True)
 
             elif tp_placed:
                 self.message_log('Restored, take profit order(s) was placed', tlg=True)
 
             else:
-                self.message_log('Restored, unknown state. Investigation needed', tlg=True)
+                self.message_log('Restored', tlg=True)
 
     def start(self, profit_f: Decimal = f2d(0), profit_s: Decimal = f2d(0)) -> None:
         self.message_log('Start')
         if self.command == 'stopped':
             self.message_log('Strategy stopped, waiting manual action')
             return
         # Cancel take profit order in all state
```

### Comparing `martin_binance-1.3.2/martin_binance/funds_rate.db.template` & `martin_binance-1.3.2.post2/martin_binance/funds_rate.db.template`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so` & `martin_binance-1.3.2.post2/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2/martin_binance/margin_wrapper.py` & `martin_binance-1.3.2.post2/martin_binance/margin_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 margin.de <-> Python strategy <-> <margin_wrapper> <-> exchanges-wrapper <-> Exchanges API/WSS
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.2"
+__version__ = "1.3.2-2"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 import ast
 import asyncio
 import simplejson as json
 import logging
@@ -420,15 +420,15 @@
     ticker = {}
     funds = {}
     order_book = {}
     order_id = int(datetime.now().strftime("%S%M")) * 1000
     wait_order_id = []  # List of placed orders for time-out detect
     canceled_order_id = []  # List canceled orders  for time-out detect
     trades = []  # List of trades associated with strategy (limit = TRADES_LIST_LIMIT)
-    orders = []  # List orders associated with strategy
+    orders = {}  # {int(id): Order(), } of orders associated with strategy
     tcm = None  # TradingCapabilityManager
     last_state = None
     rate_limiter = RATE_LIMITER
     start_time_ms = int(time.time() * 1000)
     send_request = None
     for_request = None
     wss_fire_up = False
@@ -496,26 +496,26 @@
         cls.order_book = {}
         cls.order_id = int(datetime.now().strftime("%S%M")) * 1000
         cls.wait_order_id = []  # List of placed orders for time-out detect
         cls.canceled_order_id = []  # List canceled orders  for time-out detect
         cls.all_trades = []  # List of all (limit = ALL_TRADES_LIST_LIMIT) trades for a specific account and symbol
         cls.trades = []  # List of trades associated with strategy (limit = TRADES_LIST_LIMIT)
         cls.all_orders = []  # List of all open orders for symbol
-        cls.orders = []  # List orders associated with strategy
+        cls.orders = {}  # Set of orders associated with strategy
         cls.strategy.get_buffered_funds_last_time = cls.strategy.get_time()
         cls.rate_limiter = RATE_LIMITER
         cls.start_time_ms = int(time.time() * 1000)
         cls.backtest = {}
         cls.bulk_orders_cancel = {}
 
     def message_log(self, *args, **kwargs):
         pass  # meant to be overridden in a subclass
 
     def order_exist(self, _id) -> bool:
-        return any(i.id == _id for i in self.orders)
+        return bool(self.orders.get(_id))
 
     def get_trading_capability_manager(self) -> TradingCapabilityManager:
         return self.tcm
 
     def get_first_currency(self) -> str:
         return self.info_symbol.get('baseAsset')
 
@@ -552,15 +552,15 @@
             time.sleep(0.035)
         return cls.order_id
 
     def get_buffered_completed_trades(self, _get_all_trades: bool = False) -> List[PrivateTrade]:
         return self.trades
 
     def get_buffered_open_orders(self) -> List[Order]:
-        return self.orders
+        return list(self.orders.values())
 
     def get_time(self) -> float:
         """
         For backtesting purpose. Calculating monotonic local time based on self.time_operational['new'] value.
         It can be set from external source as int(time.time()) getting from historical data. If can't setting
         return system int(time.time()) Unix time.
         :return: int
@@ -582,19 +582,19 @@
         else:
             last = time.time()
         return last
 
     def open_orders_snapshot(self):
         orders_buy = {}
         orders_sell = {}
-        for order in self.orders:
+        for k, order in self.orders.items():
             if order.buy:
-                orders_buy[order.id] = order.price
+                orders_buy[k] = order.price
             else:
-                orders_sell[order.id] = order.price
+                orders_sell[k] = order.price
         self.grid_buy.update({int(time.time() * 1000): pd.Series(orders_buy)})
         self.grid_sell.update({int(time.time() * 1000): pd.Series(orders_sell)})
 
     @staticmethod
     def get_buffered_recent_candles(candle_size_in_minutes: int, number_of_candles: int = 50,
                                     include_current_building_candle: bool = False) -> List[Candle]:
         size = convert_from_minute(candle_size_in_minutes)
@@ -662,15 +662,15 @@
         except (KeyboardInterrupt, asyncio.CancelledError):
             break
 
 
 def last_state_update(cls, last_state):
     last_state[ms_order_id] = json.dumps(cls.order_id)
     last_state['ms_start_time_ms'] = json.dumps(cls.start_time_ms)
-    last_state[ms_orders] = jsonpickle.encode(cls.orders)
+    last_state[ms_orders] = jsonpickle.encode(cls.orders, keys=True)
     last_state['ms_trades'] = jsonpickle.encode(cls.trades)
 
 
 async def save_asset():
     """
     Update account asset list and value in t_asset
     """
@@ -990,15 +990,15 @@
             funds = {cls.base_asset: FundsEntry(cls.funds[cls.base_asset]),
                      cls.quote_asset: FundsEntry(cls.funds[cls.quote_asset])}
             cls.strategy.on_new_funds(funds)
 
 
 async def buffered_orders():
     cls = StrategyBase
-    exch_orders_id = []
+    exch_orders = {}
     save_orders_id = []
     restore = False
     run = False
     while not run:
         try:
             res = await cls.send_request(cls.stub.CheckStream, api_pb2.MarketRequest, symbol=cls.symbol)
         except Exception as ex:
@@ -1017,15 +1017,22 @@
             if cls.last_state:
                 cls.strategy.message_log("Trying restore saved state after restart", color=ms.Style.GREEN)
                 # Restore StrategyBase class var
                 cls.order_id = json.loads(cls.last_state.pop(ms_order_id,
                                                              str(int(datetime.now().strftime("%S%M")) * 1000)))
                 cls.start_time_ms = json.loads(cls.last_state.pop('ms_start_time_ms', str(int(time.time() * 1000))))
                 cls.trades = jsonpickle.decode(cls.last_state.pop('ms_trades', '[]'))
-                cls.orders = jsonpickle.decode(cls.last_state.pop(ms_orders, '[]'))
+                # TODO change after update and restart
+                # cls.orders = jsonpickle.decode(cls.last_state.pop(ms_orders, '{}'), keys=True)
+                _orders_from_save = jsonpickle.decode(cls.last_state.pop(ms_orders, '{}'), keys=True)
+                if isinstance(_orders_from_save, list):
+                    for _o in _orders_from_save:
+                        cls.orders[_o.id] = _o
+                else:
+                    cls.orders = _orders_from_save
                 #
                 cls.strategy.restore_strategy_state(cls.last_state)
 
             if restore:
                 cls.strategy.message_log("Trying restore saved state after lost connection to host",
                                          color=ms.Style.GREEN)
 
@@ -1034,30 +1041,32 @@
                 raise UserWarning("Can't fetch open orders")
             StrategyBase.rate_limiter = max(StrategyBase.rate_limiter, _orders.rate_limiter)
             orders = json_format.MessageToDict(_orders).get('items', [])
             # print(f"buffered_orders.orders: {orders}")
             part_id = []
             for order in orders:
                 _id = int(order['orderId'])
-                exch_orders_id.append(_id)
+                exch_orders[_id] = Order(order)
                 if (order.get('status', None) == 'PARTIALLY_FILLED'
                         and order_trades_sum(_id) < Decimal(order['executedQty'])):
                     part_id.append(_id)
-            for i in cls.orders:
-                save_orders_id.append(i.id)
+            # Add TP id
+            if cls.strategy.tp_order_id:
+                save_orders_id.append(cls.strategy.tp_order_id)
+            # Add grid id's
+            save_orders_id.extend(list(cls.orders))
             # Missed fill event list
-            diff_id = list(set(save_orders_id).difference(exch_orders_id))
+            diff_id = list(set(save_orders_id).difference(set(exch_orders)))
             # print(f"buffered_orders.diff_id: {diff_id}")
             # Erroneously not deleted order
-            diff_excess_id = list(set(exch_orders_id).
+            diff_excess_id = list(set(exch_orders).
                                   difference(save_orders_id).
                                   intersection(cls.canceled_order_id))
             # print(f"buffered_orders.diff_excess_id: {diff_excess_id}")
-            exch_orders_id.clear()
-            save_orders_id.clear()
+
             if diff_id or part_id:
                 cls.strategy.message_log(f"Perhaps was missed event for order(s): {diff_id + part_id},"
                                          f" checking it", log_level=LogLevel.WARNING, tlg=False)
                 for _id in list(set(diff_id + part_id)):
                     await fetch_order(_id, _filled_update_call=True)
                 part_id.clear()
             if diff_excess_id:
@@ -1073,15 +1082,17 @@
 
             if ms.MODE == 'TC' and cls.last_state:
                 last_state = cls.strategy.save_strategy_state(return_only=True)
                 last_state_update(cls, last_state)
                 with cls.state_file.open(mode='w') as outfile:
                     json.dump(last_state, outfile, sort_keys=True, indent=4, ensure_ascii=False)
                 cls.strategy.start_collect = True
-
+            cls.orders.update(exch_orders)
+            exch_orders.clear()
+            save_orders_id.clear()
             cls.last_state = None
             restore = False
 
         except asyncio.CancelledError:
             # print("buffered_orders.Cancelled")
             run = False
         except UserWarning as ex:
@@ -1150,24 +1161,23 @@
 
 async def on_order_update():
     cls = StrategyBase
     try:
         async for event in cls.for_request(cls.stub.OnOrderUpdate, api_pb2.MarketRequest, symbol=cls.symbol):
             # Only for registered orders on own pair
             ed = ast.literal_eval(json.loads(event.result))
-            # print(f"on_order_update.ed: {ed}")
             on_order_update_handler(cls, ed)
     except Exception as ex:
         logger.warning(f"Exception on WSS, on_order_update loop closed: {ex}\n{traceback.format_exc()}")
         cls.wss_fire_up = True
 
 
 def on_order_update_handler(cls, ed):
     if (cls.symbol == ed['symbol']
-            and cls.strategy.order_exist(ed['order_id'])
+            and (cls.strategy.order_exist(ed['order_id']) or cls.strategy.tp_order_id == ed['order_id'])
             and ed['order_status'] in ('FILLED', 'PARTIALLY_FILLED')):
         if ed['order_status'] == 'FILLED':
             # Remove from all_orders and orders lists
             remove_from_orders_lists([ed['order_id']])
         if trade_not_exist(ed['order_id'], ed['trade_id']):
             trade = {"qty": ed['last_executed_quantity'],
                      "isBuyer": bool(ed['side'] == 'BUY'),
@@ -1252,15 +1262,15 @@
                          "price": price,
                          "time": order.timestamp}
                 # cls.strategy.message_log(f"place_limit_order_callback.trade: {trade}", color=ms.Style.YELLOW)
                 if len(cls.trades) > TRADES_LIST_LIMIT:
                     del cls.trades[0]
                 cls.trades.append(PrivateTrade(trade))
             if executed_qty < orig_qty:
-                cls.orders.append(order)
+                cls.orders[order.id] =  order
             if ms.MODE == 'TC' and cls.strategy.start_collect:
                 cls.strategy.open_orders_snapshot()
             elif ms.MODE == 'S':
                 await on_funds_update()
             cls.strategy.on_place_order_success(_id, order)
 
 
@@ -1326,16 +1336,16 @@
         cls.strategy.message_log(f"Exception on cancel all orders for {_id}:\n{_ex}")
     else:
         # print(f"cancel_all_order_call.result: {result}")
         # Remove from all_orders and orders lists
         if result and result.get('status') == 'CANCELED':
             remove_from_orders_lists([_id])
             cls.strategy.message_log(f"Cancel order {_id} success", color=ms.Style.GREEN)
-            cls.strategy.on_cancel_order_success(_id, Order(result), cancel_all=True)
             cls.canceled_order_id.append(_id)
+            cls.strategy.on_cancel_order_success(_id, Order(result), cancel_all=True)
 
 
 async def cancel_order_timeout(_id):
     cls = StrategyBase
     await asyncio.sleep(ORDER_TIMEOUT)
     if _id in cls.canceled_order_id:
         cls.canceled_order_id.remove(_id)
@@ -1388,15 +1398,15 @@
             cls.strategy.message_log(f"Not sent {amount} {symbol} to main account\n,{res.result}",
                                      log_level=LogLevel.ERROR)
 
 
 def remove_from_orders_lists(_order_id_list: []) -> None:
     cls = StrategyBase
     # print(f"remove_from_orders_lists._order_id: {_order_id}")
-    cls.orders[:] = [i for i in cls.orders if i.id not in _order_id_list]
+    [cls.orders.pop(i, None) for i in _order_id_list]
 
 
 def remove_from_trades_lists(_order_id) -> None:
     cls = StrategyBase
     # print(f"remove_from_trades_lists._order_id: {_order_id}")
     cls.trades[:] = [i for i in cls.trades if i.order_id != _order_id]
 
@@ -1606,15 +1616,15 @@
     cls.for_request = _session.for_request
 
 
 def restore_state_before_backtesting(cls):
     saved_state = load_file(cls.state_file)
     cls.order_id = json.loads(saved_state.pop(ms_order_id, "0"))
     cls.trades = jsonpickle.decode(saved_state.pop('ms_trades', '[]'))
-    cls.orders = jsonpickle.decode(saved_state.pop(ms_orders, '[]'))
+    cls.orders = jsonpickle.decode(saved_state.pop(ms_orders, '{}'))
     orders = json.loads(saved_state.get('orders'))
     # Restore initial state
     cls.strategy.cycle_buy = json.loads(saved_state.get('cycle_buy'))
     cls.strategy.reverse = json.loads(saved_state.get('reverse'))
     cls.strategy.deposit_first = ms.f2d(json.loads(saved_state.get('deposit_first')))
     cls.strategy.deposit_second = ms.f2d(json.loads(saved_state.get('deposit_second')))
     if cls.strategy.reverse:
```

### Comparing `martin_binance-1.3.2/martin_binance/ms_cfg.toml.template` & `martin_binance-1.3.2.post2/martin_binance/ms_cfg.toml.template`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2/martin_binance/service/funds_rate_exporter.py` & `martin_binance-1.3.2.post2/martin_binance/service/funds_rate_exporter.py`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2/martin_binance/service/grafana.json` & `martin_binance-1.3.2.post2/martin_binance/service/grafana.json`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2/martin_binance/service/relaunch.py` & `martin_binance-1.3.2.post2/martin_binance/service/relaunch.py`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2/pyproject.toml` & `martin_binance-1.3.2.post2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `martin_binance-1.3.2/PKG-INFO` & `martin_binance-1.3.2.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: martin-binance
-Version: 1.3.2
+Version: 1.3.2.post2
 Summary: Free trading system for Binance SPOT API
 Author-email: Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: martin-binance Version: 1.3.2 Summary: Free trading
-system for Binance SPOT API Author-email: Jerry Fedorenko
+Metadata-Version: 2.1 Name: martin-binance Version: 1.3.2.post2 Summary: Free
+trading system for Binance SPOT API Author-email: Jerry Fedorenko
 fedorenko@yahoo.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Programming Language :: Python :: 3 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: Unix Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: MacOS Requires-
 Dist: exchanges-wrapper==1.3.2 Requires-Dist: margin-strategy-sdk==0.0.11
 Requires-Dist: aiohttp==3.8.4 Requires-Dist: grpcio==1.48.1 Requires-Dist:
```

