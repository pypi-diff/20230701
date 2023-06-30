# Comparing `tmp/rubi-2.0.5.tar.gz` & `tmp/rubi-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubi-2.0.5.tar", max compression
+gzip compressed data, was "rubi-2.0.6.tar", max compression
```

## Comparing `rubi-2.0.5.tar` & `rubi-2.0.6.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    11357 2023-02-09 17:21:21.757346 rubi-2.0.5/LICENSE
--rw-r--r--   0        0        0     2757 2023-06-01 22:20:20.359716 rubi-2.0.5/README.md
--rw-r--r--   0        0        0     6735 2023-06-01 18:59:40.464065 rubi-2.0.5/network_config/ERC20.json
--rw-r--r--   0        0        0     1920 2023-06-01 18:59:40.464275 rubi-2.0.5/network_config/README.md
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.464692 rubi-2.0.5/network_config/abitrum_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.464994 rubi-2.0.5/network_config/abitrum_goerli/abis/router.json
--rw-r--r--   0        0        0      633 2023-06-13 17:59:13.620185 rubi-2.0.5/network_config/abitrum_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.465638 rubi-2.0.5/network_config/optimism/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.467925 rubi-2.0.5/network_config/optimism/abis/router.json
--rw-r--r--   0        0        0      651 2023-06-13 17:59:13.620375 rubi-2.0.5/network_config/optimism/network.yaml
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468441 rubi-2.0.5/network_config/optimism_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.468572 rubi-2.0.5/network_config/optimism_goerli/abis/router.json
--rw-r--r--   0        0        0      508 2023-06-13 17:59:13.620539 rubi-2.0.5/network_config/optimism_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468889 rubi-2.0.5/network_config/polygon_mumbai/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.469043 rubi-2.0.5/network_config/polygon_mumbai/abis/router.json
--rw-r--r--   0        0        0      619 2023-06-13 17:59:13.620686 rubi-2.0.5/network_config/polygon_mumbai/network.yaml
--rw-r--r--   0        0        0      748 2023-06-28 02:48:58.418121 rubi-2.0.5/pyproject.toml
--rw-r--r--   0        0        0      104 2023-06-21 19:17:01.151640 rubi-2.0.5/rubi/__init__.py
--rw-r--r--   0        0        0    25763 2023-06-21 19:17:01.151931 rubi-2.0.5/rubi/client.py
--rw-r--r--   0        0        0      163 2023-06-21 19:17:01.152075 rubi-2.0.5/rubi/contracts/__init__.py
--rw-r--r--   0        0        0    61077 2023-06-01 18:59:40.472708 rubi-2.0.5/rubi/contracts/aid.py
--rw-r--r--   0        0        0    11403 2023-06-21 19:17:01.152239 rubi-2.0.5/rubi/contracts/base_contract.py
--rw-r--r--   0        0        0       73 2023-06-21 19:17:01.152321 rubi-2.0.5/rubi/contracts/contract_types/__init__.py
--rw-r--r--   0        0        0    15968 2023-06-21 19:17:01.152942 rubi-2.0.5/rubi/contracts/contract_types/events.py
--rw-r--r--   0        0        0     2675 2023-06-28 02:48:32.616209 rubi-2.0.5/rubi/contracts/contract_types/transaction_reciept.py
--rw-r--r--   0        0        0    16609 2023-06-21 19:17:01.153278 rubi-2.0.5/rubi/contracts/erc20.py
--rw-r--r--   0        0        0    24669 2023-06-21 19:17:01.153743 rubi-2.0.5/rubi/contracts/market.py
--rw-r--r--   0        0        0    14847 2023-06-21 19:17:01.153923 rubi-2.0.5/rubi/contracts/router.py
--rw-r--r--   0        0        0      257 2023-06-01 18:59:40.473763 rubi-2.0.5/rubi/data/README.md
--rw-r--r--   0        0        0       33 2023-02-14 16:34:53.717274 rubi-2.0.5/rubi/data/__init__.py
--rw-r--r--   0        0        0     3968 2023-06-01 18:59:40.473880 rubi-2.0.5/rubi/data/data.py
--rw-r--r--   0        0        0     1198 2023-02-14 16:34:53.717485 rubi-2.0.5/rubi/data/processing/README.md
--rw-r--r--   0        0        0       64 2023-02-14 16:34:53.717551 rubi-2.0.5/rubi/data/processing/__init__.py
--rw-r--r--   0        0        0    20226 2023-03-28 22:32:44.963776 rubi-2.0.5/rubi/data/processing/aid.py
--rw-r--r--   0        0        0       31 2023-02-14 16:34:53.717742 rubi-2.0.5/rubi/data/processing/helper/__init__.py
--rw-r--r--   0        0        0     2292 2023-02-14 16:34:53.717833 rubi-2.0.5/rubi/data/processing/helper/processing.py
--rw-r--r--   0        0        0    10226 2023-02-14 16:34:53.717931 rubi-2.0.5/rubi/data/processing/user.py
--rw-r--r--   0        0        0       69 2023-02-14 16:34:53.718073 rubi-2.0.5/rubi/data/sources/__init__.py
--rw-r--r--   0        0        0    21161 2023-03-28 22:32:44.964336 rubi-2.0.5/rubi/data/sources/aid.py
--rw-r--r--   0        0        0     1194 2023-02-14 16:34:53.718302 rubi-2.0.5/rubi/data/sources/helper/README.md
--rw-r--r--   0        0        0       76 2023-02-14 16:34:53.718369 rubi-2.0.5/rubi/data/sources/helper/__init__.py
--rw-r--r--   0        0        0    12589 2023-02-27 02:08:49.086543 rubi-2.0.5/rubi/data/sources/helper/gas.py
--rw-r--r--   0        0        0    15373 2023-02-14 16:34:53.718597 rubi-2.0.5/rubi/data/sources/helper/price.py
--rw-r--r--   0        0        0     7319 2023-02-14 16:34:53.718699 rubi-2.0.5/rubi/data/sources/helper/rolodex.py
--rw-r--r--   0        0        0    22425 2023-02-14 16:34:53.718888 rubi-2.0.5/rubi/data/sources/market.py
--rw-r--r--   0        0        0       72 2023-06-01 18:59:40.474197 rubi-2.0.5/rubi/network/__init__.py
--rw-r--r--   0        0        0     7596 2023-06-23 20:01:50.707431 rubi-2.0.5/rubi/network/network.py
--rw-r--r--   0        0        0       66 2023-06-21 19:17:01.154162 rubi-2.0.5/rubi/rubicon_types/__init__.py
--rw-r--r--   0        0        0    15552 2023-06-21 19:17:01.154405 rubi-2.0.5/rubi/rubicon_types/order.py
--rw-r--r--   0        0        0     5727 2023-06-21 19:17:01.154503 rubi-2.0.5/rubi/rubicon_types/orderbook.py
--rw-r--r--   0        0        0     2776 2023-06-21 19:17:01.154577 rubi-2.0.5/rubi/rubicon_types/pair.py
--rw-r--r--   0        0        0     3545 1970-01-01 00:00:00.000000 rubi-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-09 17:21:21.757346 rubi-2.0.6/LICENSE
+-rw-r--r--   0        0        0     2757 2023-06-01 22:20:20.359716 rubi-2.0.6/README.md
+-rw-r--r--   0        0        0     6735 2023-06-01 18:59:40.464065 rubi-2.0.6/network_config/ERC20.json
+-rw-r--r--   0        0        0     1920 2023-06-01 18:59:40.464275 rubi-2.0.6/network_config/README.md
+-rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.464692 rubi-2.0.6/network_config/abitrum_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.464994 rubi-2.0.6/network_config/abitrum_goerli/abis/router.json
+-rw-r--r--   0        0        0      633 2023-06-30 02:50:06.551418 rubi-2.0.6/network_config/abitrum_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.465638 rubi-2.0.6/network_config/optimism/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.467925 rubi-2.0.6/network_config/optimism/abis/router.json
+-rw-r--r--   0        0        0      651 2023-06-30 02:50:06.551545 rubi-2.0.6/network_config/optimism/network.yaml
+-rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468441 rubi-2.0.6/network_config/optimism_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.468572 rubi-2.0.6/network_config/optimism_goerli/abis/router.json
+-rw-r--r--   0        0        0      560 2023-06-30 22:38:54.821457 rubi-2.0.6/network_config/optimism_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468889 rubi-2.0.6/network_config/polygon_mumbai/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.469043 rubi-2.0.6/network_config/polygon_mumbai/abis/router.json
+-rw-r--r--   0        0        0      619 2023-06-30 02:50:06.551793 rubi-2.0.6/network_config/polygon_mumbai/network.yaml
+-rw-r--r--   0        0        0      898 2023-06-30 22:38:54.823155 rubi-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0      104 2023-06-30 02:50:06.553692 rubi-2.0.6/rubi/__init__.py
+-rw-r--r--   0        0        0    26255 2023-06-30 22:38:54.823356 rubi-2.0.6/rubi/client.py
+-rw-r--r--   0        0        0      163 2023-06-30 02:50:06.554484 rubi-2.0.6/rubi/contracts/__init__.py
+-rw-r--r--   0        0        0    61077 2023-06-01 18:59:40.472708 rubi-2.0.6/rubi/contracts/aid.py
+-rw-r--r--   0        0        0    11860 2023-06-30 22:38:54.823525 rubi-2.0.6/rubi/contracts/base_contract.py
+-rw-r--r--   0        0        0       74 2023-06-30 22:38:54.823906 rubi-2.0.6/rubi/contracts/contract_types/__init__.py
+-rw-r--r--   0        0        0    15968 2023-06-30 02:50:06.555210 rubi-2.0.6/rubi/contracts/contract_types/events.py
+-rw-r--r--   0        0        0     2708 2023-06-30 22:38:54.824073 rubi-2.0.6/rubi/contracts/contract_types/transaction_reciept.py
+-rw-r--r--   0        0        0    17101 2023-06-30 22:38:54.824447 rubi-2.0.6/rubi/contracts/erc20.py
+-rw-r--r--   0        0        0    24668 2023-06-30 22:38:54.824645 rubi-2.0.6/rubi/contracts/market.py
+-rw-r--r--   0        0        0    14847 2023-06-30 02:50:06.556060 rubi-2.0.6/rubi/contracts/router.py
+-rw-r--r--   0        0        0      257 2023-06-30 02:50:03.540922 rubi-2.0.6/rubi/data/README.md
+-rw-r--r--   0        0        0       33 2023-06-30 02:50:03.541036 rubi-2.0.6/rubi/data/__init__.py
+-rw-r--r--   0        0        0     3968 2023-06-30 02:50:03.541150 rubi-2.0.6/rubi/data/data.py
+-rw-r--r--   0        0        0     1198 2023-06-30 02:50:03.541258 rubi-2.0.6/rubi/data/processing/README.md
+-rw-r--r--   0        0        0       64 2023-06-30 02:50:03.541320 rubi-2.0.6/rubi/data/processing/__init__.py
+-rw-r--r--   0        0        0    20226 2023-06-30 02:50:03.541646 rubi-2.0.6/rubi/data/processing/aid.py
+-rw-r--r--   0        0        0       31 2023-06-30 02:50:03.541785 rubi-2.0.6/rubi/data/processing/helper/__init__.py
+-rw-r--r--   0        0        0     2292 2023-06-30 02:50:03.541878 rubi-2.0.6/rubi/data/processing/helper/processing.py
+-rw-r--r--   0        0        0    10226 2023-06-30 02:50:03.541970 rubi-2.0.6/rubi/data/processing/user.py
+-rw-r--r--   0        0        0       69 2023-06-30 02:50:03.542086 rubi-2.0.6/rubi/data/sources/__init__.py
+-rw-r--r--   0        0        0    21161 2023-06-30 02:50:03.542477 rubi-2.0.6/rubi/data/sources/aid.py
+-rw-r--r--   0        0        0     1194 2023-06-30 02:50:03.542594 rubi-2.0.6/rubi/data/sources/helper/README.md
+-rw-r--r--   0        0        0       76 2023-06-30 02:50:03.542657 rubi-2.0.6/rubi/data/sources/helper/__init__.py
+-rw-r--r--   0        0        0    12589 2023-06-30 02:50:03.542925 rubi-2.0.6/rubi/data/sources/helper/gas.py
+-rw-r--r--   0        0        0    15373 2023-06-30 02:50:03.543041 rubi-2.0.6/rubi/data/sources/helper/price.py
+-rw-r--r--   0        0        0     7319 2023-06-30 02:50:03.543148 rubi-2.0.6/rubi/data/sources/helper/rolodex.py
+-rw-r--r--   0        0        0    22425 2023-06-30 02:50:03.543454 rubi-2.0.6/rubi/data/sources/market.py
+-rw-r--r--   0        0        0       72 2023-06-01 18:59:40.474197 rubi-2.0.6/rubi/network/__init__.py
+-rw-r--r--   0        0        0     7596 2023-06-30 02:50:06.556325 rubi-2.0.6/rubi/network/network.py
+-rw-r--r--   0        0        0       66 2023-06-30 02:50:06.556396 rubi-2.0.6/rubi/rubicon_types/__init__.py
+-rw-r--r--   0        0        0    15554 2023-06-30 22:38:54.825030 rubi-2.0.6/rubi/rubicon_types/order.py
+-rw-r--r--   0        0        0     6305 2023-06-30 22:38:54.825201 rubi-2.0.6/rubi/rubicon_types/orderbook.py
+-rw-r--r--   0        0        0     2776 2023-06-30 02:50:06.556913 rubi-2.0.6/rubi/rubicon_types/pair.py
+-rw-r--r--   0        0        0     3545 1970-01-01 00:00:00.000000 rubi-2.0.6/PKG-INFO
```

### Comparing `rubi-2.0.5/LICENSE` & `rubi-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/README.md` & `rubi-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/network_config/ERC20.json` & `rubi-2.0.6/network_config/ERC20.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/network_config/README.md` & `rubi-2.0.6/network_config/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/network_config/abitrum_goerli/abis/market.json` & `rubi-2.0.6/network_config/abitrum_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/network_config/abitrum_goerli/abis/router.json` & `rubi-2.0.6/network_config/abitrum_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/network_config/abitrum_goerli/network.yaml` & `rubi-2.0.6/network_config/abitrum_goerli/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/network_config/optimism/abis/market.json` & `rubi-2.0.6/network_config/optimism/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/network_config/optimism/abis/router.json` & `rubi-2.0.6/network_config/optimism/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/network_config/optimism/network.yaml` & `rubi-2.0.6/network_config/optimism/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/network_config/optimism_goerli/abis/market.json` & `rubi-2.0.6/network_config/optimism_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/network_config/optimism_goerli/abis/router.json` & `rubi-2.0.6/network_config/optimism_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/network_config/polygon_mumbai/abis/market.json` & `rubi-2.0.6/network_config/polygon_mumbai/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/network_config/polygon_mumbai/abis/router.json` & `rubi-2.0.6/network_config/polygon_mumbai/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/network_config/polygon_mumbai/network.yaml` & `rubi-2.0.6/network_config/polygon_mumbai/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/rubi/client.py` & `rubi-2.0.6/rubi/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from _decimal import Decimal
 from multiprocessing import Queue
 from threading import Thread
 from time import sleep
 from typing import Union, List, Optional, Dict, Type, Any, Callable
 
 from eth_typing import ChecksumAddress
-from web3.types import EventData
+from web3.types import EventData, Nonce
 
 from rubi.contracts import (
     RubiconMarket,
     RubiconRouter,
     ERC20,
     TransactionReceipt,
     EmitFeeEvent
@@ -186,23 +186,23 @@
         :type new_base_asset_allowance: Optional[Decimal]
         :param new_quote_asset_allowance: New allowance for the quote asset. (optional, default is None).
         :type new_quote_asset_allowance: Optional[Decimal]
         :raises PairDoesNotExistException: If the pair does not exist in the clients internal _pairs dict.
         """
         pair = self.get_pair(pair_name=pair_name)
 
-        if new_base_asset_allowance and pair.current_base_asset_allowance != new_base_asset_allowance:
+        if new_base_asset_allowance is not None and pair.current_base_asset_allowance != new_base_asset_allowance:
             self._update_asset_allowance(
                 asset=pair.base_asset,
                 spender=self.market.address,
                 new_allowance=new_base_asset_allowance
             )
             pair.update_base_asset_allowance(new_base_asset_allowance=new_base_asset_allowance)
 
-        if new_quote_asset_allowance and pair.current_base_asset_allowance != new_quote_asset_allowance:
+        if new_quote_asset_allowance is not None and pair.current_quote_asset_allowance != new_quote_asset_allowance:
             self._update_asset_allowance(
                 asset=pair.quote_asset,
                 spender=self.market.address,
                 new_allowance=new_quote_asset_allowance
             )
             pair.update_quote_asset_allowance(new_quote_asset_allowance=new_quote_asset_allowance)
 
@@ -238,14 +238,26 @@
             new_base_asset_allowance=Decimal("0"),
             new_quote_asset_allowance=Decimal("0")
         )
 
         del self._pairs[pair_name]
 
     ######################################################################
+    # nonce methods
+    ######################################################################
+
+    def get_nonce(self) -> Nonce:
+        """Get the current transaction count of the wallet to determine the nonce
+
+        :return: The current nonce of the wallet
+        :rtype: Nonce
+        """
+        return self.network.w3.eth.get_transaction_count(self.wallet)
+
+    ######################################################################
     # orderbook methods
     ######################################################################
 
     def get_orderbook(self, pair_name: str) -> OrderBook:
         """Retrieve the order book for a specific pair from the Rubicon Router.
 
         :param pair_name: Name of the pair to retrieve the order book for.
@@ -417,24 +429,24 @@
 
         match order.order_side:
             case OrderSide.BUY:
                 return self.market.buy_all_amount(
                     buy_gem=pair.base_asset.address,
                     buy_amt=pair.base_asset.to_integer(order.size),
                     pay_gem=pair.quote_asset.address,
-                    max_fill_amount=pair.quote_asset.to_integer(order.worst_execution_price),
-                    **transaction.args(),
+                    max_fill_amount=pair.quote_asset.to_integer(order.worst_execution_price * order.size),
+                    **transaction.args()
                 )
             case OrderSide.SELL:
                 return self.market.sell_all_amount(
                     pay_gem=pair.base_asset.address,
                     pay_amt=pair.base_asset.to_integer(order.size),
                     buy_gem=pair.quote_asset.address,
-                    min_fill_amount=pair.quote_asset.to_integer(order.worst_execution_price),
-                    **transaction.args(),
+                    min_fill_amount=pair.quote_asset.to_integer(order.worst_execution_price * order.size),
+                    **transaction.args()
                 )
 
     def place_limit_order(self, transaction: Transaction) -> TransactionReceipt:
         """Place a limit order transaction by executing the specified transaction object. The transaction object should
         contain a single order of type NewLimitOrder.
 
         :param transaction: Transaction object containing the limit order.
@@ -453,23 +465,23 @@
         match order.order_side:
             case OrderSide.BUY:
                 return self.market.offer(
                     pay_amt=pair.quote_asset.to_integer(order.price * order.size),
                     pay_gem=pair.quote_asset.address,
                     buy_amt=pair.base_asset.to_integer(order.size),
                     buy_gem=pair.base_asset.address,
-                    **transaction.args(),
+                    **transaction.args()
                 )
             case OrderSide.SELL:
                 return self.market.offer(
                     pay_amt=pair.base_asset.to_integer(order.size),
                     pay_gem=pair.base_asset.address,
                     buy_amt=pair.quote_asset.to_integer(order.price * order.size),
                     buy_gem=pair.quote_asset.address,
-                    **transaction.args(),
+                    **transaction.args()
                 )
 
     def cancel_limit_order(self, transaction: Transaction) -> TransactionReceipt:
         """Place a limit order cancel transaction by executing the specified transaction object. The transaction object
         should contain a single order of type NewCancelOrder.
 
         :param transaction: Transaction object containing the cancel order.
@@ -481,15 +493,15 @@
         if len(transaction.orders) > 1:
             raise Exception("call place_order with one order only")
 
         order: NewCancelOrder = transaction.orders[0]  # noqa
 
         return self.market.cancel(
             id=order.order_id,
-            **transaction.args(),
+            **transaction.args()
         )
 
     def batch_place_limit_orders(self, transaction: Transaction) -> TransactionReceipt:
         """Place multiple limit orders in a batch transaction.
 
         :param transaction: Transaction object containing multiple limit orders.
         :type transaction: Transaction
@@ -518,15 +530,15 @@
                     buy_gems.append(pair.quote_asset.address)
 
         return self.market.batch_offer(
             pay_amts=pay_amts,
             pay_gems=pay_gems,
             buy_amts=buy_amts,
             buy_gems=buy_gems,
-            **transaction.args(),
+            **transaction.args()
         )
 
     def batch_update_limit_orders(self, transaction: Transaction) -> TransactionReceipt:
         """Update multiple limit orders in a batch transaction.
 
         :param transaction: Transaction object containing multiple limit order updates.
         :type transaction: Transaction
@@ -559,15 +571,15 @@
 
         return self.market.batch_requote(
             ids=order_ids,
             pay_amts=pay_amts,
             pay_gems=pay_gems,
             buy_amts=buy_amts,
             buy_gems=buy_gems,
-            **transaction.args(),
+            **transaction.args()
         )
 
     def batch_cancel_limit_orders(self, transaction: Transaction) -> TransactionReceipt:
         """Cancel multiple limit orders in a batch transaction.
 
         :param transaction: Transaction object containing multiple limit order cancellations.
         :type transaction: Transaction
@@ -579,15 +591,15 @@
         for order in transaction.orders:
             order: NewCancelOrder
 
             order_ids.append(order.order_id)
 
         return self.market.batch_cancel(
             ids=order_ids,
-            **transaction.args(),
+            **transaction.args()
         )
 
     ######################################################################
     # helper methods
     ######################################################################
 
     # TODO: revisit as the safer thing is to set approval to 0 and then set approval to new_allowance
```

### Comparing `rubi-2.0.5/rubi/contracts/aid.py` & `rubi-2.0.6/rubi/contracts/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/rubi/contracts/base_contract.py` & `rubi-2.0.6/rubi/contracts/base_contract.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging as log
+import time
 from threading import Thread
 from time import sleep
 from typing import Optional, Callable, Type, Dict, Any
 
 from eth_account.datastructures import SignedTransaction
 from eth_typing import ChecksumAddress
 from web3 import Web3
@@ -117,23 +118,25 @@
         """
 
         event_filter = event_type.create_event_filter(contract=self.contract, argument_filters=argument_filters)
         handler = event_handler if event_handler is not None else event_type.default_handler
 
         thread = Thread(
             target=self._start_default_event_poller,
-            args=(pair_name, event_type, event_filter, handler, poll_time),
+            args=(pair_name, event_type, self.contract, argument_filters, event_filter, handler, poll_time),
             daemon=True
         )
         thread.start()
 
     @staticmethod
     def _start_default_event_poller(
         pair_name: str,
         event_type: Type[BaseEvent],
+        contract: Contract,
+        argument_filters: Optional[Dict[str, Any]],
         event_filter: LogFilter,
         event_handler: Callable,
         poll_time: int
     ) -> None:
         """Start the default event poller loop. This thread will stop if the pair is removed from the client.
 
         :param pair_name: The name of the event pair.
@@ -152,14 +155,19 @@
         while polling:
             try:
                 for event_data in event_filter.get_new_entries():
                     event_handler(pair_name, event_type, event_data)
             except Exception as e:
                 log.error(e)
 
+                # The filter has been deleted by the node and needs to be recreated
+                if "filter not found" in str(e):
+                    event_filter = event_type.create_event_filter(contract=contract, argument_filters=argument_filters)
+                    log.info(f"event filter for: {event_type} has been recreated")
+
                 # TODO: this is a hack to detect if a PairDoesNotExistException is raised and polling should stop.
                 #  Currently an additional except PairDoesNotExistException as e: cannot be added as this causes a
                 #  circular import. Think about restructuring the directories to avoid this (e.g one root level types
                 #  directory).
                 if "add pair to the client" in str(e):
                     polling = False
 
@@ -213,14 +221,15 @@
         )
 
         signed_txn = self.w3.eth.account.sign_transaction(
             transaction_dict=txn,
             private_key=self.key
         )
 
+        log.debug(f"SENDING TRANSACTION, nonce: {nonce}, timestamp: {time.time_ns()}")
         self.w3.eth.send_raw_transaction(signed_txn.rawTransaction)
 
         return self._wait_for_transaction_receipt(transaction=signed_txn)
 
     def _transaction_params(
         self,
         nonce: Optional[Nonce],
@@ -258,17 +267,16 @@
         return {key: value for key, value in transaction.items() if value is not None}
 
     def _wait_for_transaction_receipt(self, transaction: SignedTransaction) -> TransactionReceipt:
         """Wait for the transaction receipt and check if the transaction was successful.
 
         :param transaction: The signed transaction object.
         :type transaction: SignedTransaction
-        :raises Exception: If the transaction fails.
         """
+
         result = TransactionReceipt.from_tx_receipt(
             tx_receipt=self.w3.eth.wait_for_transaction_receipt(transaction.hash)
         )
 
-        if result.status == 0:
-            raise Exception(f"transaction {transaction.hash.hex()} failed")
+        log.debug(f"RECEIVED RESULT, timestamp: {time.time_ns()}")
 
         return result
```

### Comparing `rubi-2.0.5/rubi/contracts/contract_types/events.py` & `rubi-2.0.6/rubi/contracts/contract_types/events.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/rubi/contracts/contract_types/transaction_reciept.py` & `rubi-2.0.6/rubi/contracts/contract_types/transaction_reciept.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from _decimal import Decimal
 from typing import Optional
 
 from eth_typing import BlockNumber, ChecksumAddress
 from hexbytes import HexBytes
 from web3.types import Wei, TxReceipt
 
 
@@ -18,15 +19,15 @@
         to_address: ChecksumAddress,
         status: int,
         transaction_hash: HexBytes,
         transaction_index: int,
         l1_fee: Optional[int] = None,
         l1_gas_price: Optional[int] = None,
         l1_gas_used: Optional[int] = None,
-        l1_fee_scalar: Optional[float] = None
+        l1_fee_scalar: Optional[Decimal] = None
     ):
         self.block_number = block_number
         self.contract_address = contract_address
         self.effective_gas_price = effective_gas_price
         self.gas_used = gas_used
         self.from_address = from_address
         self.to_address = to_address
@@ -50,13 +51,13 @@
             to_address=tx_receipt["to"],
             status=tx_receipt["status"],
             transaction_hash=tx_receipt["transactionHash"],
             transaction_index=tx_receipt["transactionIndex"],
             l1_fee=None if tx_receipt.get("l1Fee") is None else int(tx_receipt.get("l1Fee"), 16),
             l1_gas_price=None if tx_receipt.get("l1GasPrice") is None else int(tx_receipt.get("l1GasPrice"), 16),
             l1_gas_used=None if tx_receipt.get("l1GasUsed") is None else int(tx_receipt.get("l1GasUsed"), 16),
-            l1_fee_scalar=None if tx_receipt.get("l1FeeScalar") is None else float(tx_receipt.get("l1FeeScalar"))
+            l1_fee_scalar=None if tx_receipt.get("l1FeeScalar") is None else Decimal(tx_receipt.get("l1FeeScalar"))
         )
 
     def __repr__(self):
         items = ("{}={!r}".format(k, self.__dict__[k]) for k in self.__dict__)
         return "{}({})".format(type(self).__name__, ", ".join(items))
```

### Comparing `rubi-2.0.5/rubi/contracts/erc20.py` & `rubi-2.0.6/rubi/contracts/erc20.py`

 * *Files 3% similar despite different names*

```diff
@@ -400,7 +400,18 @@
         :rtype: int
         """
 
         if number == Decimal("0"):
             return 0
         else:
             return int(number * (10 ** self.decimal))
+
+    def max_approval_amount(self) -> Decimal:
+        """return the max uint256 token approval amount. Note: this is not very secure and if you give this approval you
+        should revoke it when you are done!
+
+        :return: the max approval amount of a uint256 token in Decimal representation
+        :rtype: Decimal
+        """
+        max_uint256 = "0xffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff"
+
+        return self.to_decimal(number=int(max_uint256, base=16))
```

### Comparing `rubi-2.0.5/rubi/contracts/market.py` & `rubi-2.0.6/rubi/contracts/market.py`

 * *Files 0% similar despite different names*

```diff
@@ -414,15 +414,15 @@
         self,
         ids: List[int],
         pay_amts: List[int],
         pay_gems: List[ChecksumAddress],
         buy_amts: List[int],
         buy_gems: List[ChecksumAddress],
         nonce: Optional[int] = None,
-        gas: int = 3500000,
+        gas: int = 800000,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
     ) -> TransactionReceipt:
         """Batch update a set of offers in a single transaction and return a list of new offer ids
 
         :param ids: the ids of the offers to cancel
         :type ids: List[int]
@@ -463,15 +463,15 @@
     def sell_all_amount(
         self,
         pay_gem: ChecksumAddress,
         pay_amt: int,
         buy_gem: ChecksumAddress,
         min_fill_amount: int,
         nonce: Optional[int] = None,
-        gas: int = 350000,
+        gas: int = 500000,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
     ) -> TransactionReceipt:
         """Sell the pay_amt of the pay_gem token in exchange for buy_gem, on the condition that you receive at least the
         min_fill_amount of the buy_gem token
 
         :param pay_gem: the address of the tokens being sold
@@ -510,15 +510,15 @@
     def buy_all_amount(
         self,
         buy_gem: ChecksumAddress,
         buy_amt: int,
         pay_gem: ChecksumAddress,
         max_fill_amount: int,
         nonce: Optional[int] = None,
-        gas: int = 350000,
+        gas: int = 500000,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None
     ) -> TransactionReceipt:
         """Buy the buy_amt of the buy_gem token in exchange for pay_gem, on the condition that it does not exceed the
         max_fill_amount of the pay_gem token
 
         :param buy_gem: the address of the tokens being bought
```

### Comparing `rubi-2.0.5/rubi/contracts/router.py` & `rubi-2.0.6/rubi/contracts/router.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/rubi/data/data.py` & `rubi-2.0.6/rubi/data/data.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/rubi/data/processing/README.md` & `rubi-2.0.6/rubi/data/processing/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/rubi/data/processing/aid.py` & `rubi-2.0.6/rubi/data/processing/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/rubi/data/processing/helper/processing.py` & `rubi-2.0.6/rubi/data/processing/helper/processing.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/rubi/data/processing/user.py` & `rubi-2.0.6/rubi/data/processing/user.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/rubi/data/sources/aid.py` & `rubi-2.0.6/rubi/data/sources/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/rubi/data/sources/helper/README.md` & `rubi-2.0.6/rubi/data/sources/helper/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/rubi/data/sources/helper/gas.py` & `rubi-2.0.6/rubi/data/sources/helper/gas.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/rubi/data/sources/helper/price.py` & `rubi-2.0.6/rubi/data/sources/helper/price.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/rubi/data/sources/helper/rolodex.py` & `rubi-2.0.6/rubi/data/sources/helper/rolodex.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/rubi/data/sources/market.py` & `rubi-2.0.6/rubi/data/sources/market.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/rubi/network/network.py` & `rubi-2.0.6/rubi/network/network.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/rubi/rubicon_types/order.py` & `rubi-2.0.6/rubi/rubicon_types/order.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
     """
     Class representing a transaction to be executed on chain
 
     :param orders: The list of orders to include in the transaction.
     :type orders: List[BaseNewOrder]
     :param nonce: The nonce for the transaction (optional).
     :type nonce: int
-    :param gas: The gas limit for the transaction (optional)
+    :param gas: The gas limit for the transaction (optional).
     :type gas: int
     :param max_fee_per_gas: The maximum fee per gas for the transaction (optional).
     :type max_fee_per_gas: int
     :param max_priority_fee_per_gas: The maximum priority fee per gas for the transaction (optional).
     :type max_priority_fee_per_gas: int
     """
 
@@ -224,14 +224,15 @@
         self.nonce = nonce
         self.gas = gas
         self.max_fee_per_gas = max_fee_per_gas
         self.max_priority_fee_per_gas = max_priority_fee_per_gas
 
     def args(self) -> Dict:
         """Creates a dictionary of not None arguments to pass to contract functions.
+
         :return: dictionary of arguments used to send transactions.
         :rtype: Dict
         """
         args = {
             "nonce": self.nonce,
             "gas": self.gas,
             "max_fee_per_gas": self.max_fee_per_gas,
```

### Comparing `rubi-2.0.5/rubi/rubicon_types/orderbook.py` & `rubi-2.0.6/rubi/rubicon_types/orderbook.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,14 +50,23 @@
         """Returns the price of the best level on the book side.
 
         :return: The price of the best level.
         :rtype: Decimal
         """
         return self.levels[0].price
 
+    def remove_liquidity_from_book(self, price: Decimal, size: Decimal):
+        for i, level in enumerate(self.levels):
+            if price == level.price:
+                if size == level.size:
+                    del self.levels[i]
+                else:
+                    self.levels[i] = BookLevel(price=price, size=level.size - size)
+                return
+
     @classmethod
     def from_rubicon_offers(
         cls,
         book_side: OrderSide,
         offers: List[List[int]],
         base_asset: ERC20,
         quote_asset: ERC20
@@ -174,10 +183,19 @@
         """Calculate the mid-price of the order book.
 
         :return: mid-price.
         :rtype: Decimal
         """
         return (self.best_bid() + self.best_ask()) / 2
 
+    def spread(self) -> Decimal:
+        """Calculate the current bid ask spread of the order book.
+
+        :return: spread
+        :rtype: Decimal
+        """
+
+        return self.best_ask() - self.best_bid()
+
     def __repr__(self):
         items = ("{}={!r}".format(k, self.__dict__[k]) for k in self.__dict__)
         return "{}({})".format(type(self).__name__, ", ".join(items))
```

### Comparing `rubi-2.0.5/rubi/rubicon_types/pair.py` & `rubi-2.0.6/rubi/rubicon_types/pair.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.5/PKG-INFO` & `rubi-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubi
-Version: 2.0.5
+Version: 2.0.6
 Summary: A python SDK for the Rubicon Protocol
 Author: denver
 Author-email: denver@rubicon.finance
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -15,15 +15,15 @@
 Requires-Dist: eth-utils (==2.1.0)
 Requires-Dist: hexbytes (==0.3.0)
 Requires-Dist: py-evm (==0.7.0a2)
 Requires-Dist: pytest (==7.3.1)
 Requires-Dist: pyyaml (==6.0.0)
 Requires-Dist: sphinx (==7.0.1) ; extra == "docs"
 Requires-Dist: subgrounds[dash] (==1.6.0)
-Requires-Dist: web3 (==6.4.0)
+Requires-Dist: web3 (==6.5.0)
 Description-Content-Type: text/markdown
 
 # rubi
 
 rubi is a python SDK for the Rubicon Protocol and has a variety of functionality for interacting with the protocol.
 Documentation related to rubi and its functionality can be found [here](https://rubi.readthedocs.io/en/latest/#).
```

