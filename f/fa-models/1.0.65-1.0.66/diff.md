# Comparing `tmp/fa-models-1.0.65.tar.gz` & `tmp/fa-models-1.0.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fa-models-1.0.65.tar", last modified: Fri Jun 30 14:17:16 2023, max compression
+gzip compressed data, was "fa-models-1.0.66.tar", last modified: Sat Jul  1 17:58:37 2023, max compression
```

## Comparing `fa-models-1.0.65.tar` & `fa-models-1.0.66.tar`

### file list

```diff
@@ -1,36 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:17:16.296353 fa-models-1.0.65/
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-30 14:17:16.296353 fa-models-1.0.65/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-06-30 14:16:47.000000 fa-models-1.0.65/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:17:16.292353 fa-models-1.0.65/fa_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-30 14:17:16.000000 fa-models-1.0.65/fa_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-30 14:17:16.000000 fa-models-1.0.65/fa_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:17:16.000000 fa-models-1.0.65/fa_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-30 14:17:16.000000 fa-models-1.0.65/fa_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 14:17:16.000000 fa-models-1.0.65/fa_models.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:17:16.292353 fa-models-1.0.65/famodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:16:47.000000 fa-models-1.0.65/famodels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:17:16.296353 fa-models-1.0.65/famodels/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:16:47.000000 fa-models-1.0.65/famodels/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-30 14:16:47.000000 fa-models-1.0.65/famodels/models/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-30 14:16:47.000000 fa-models-1.0.65/famodels/models/direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-30 14:16:47.000000 fa-models-1.0.65/famodels/models/exchange_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-30 14:16:47.000000 fa-models-1.0.65/famodels/models/fund.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-30 14:16:47.000000 fa-models-1.0.65/famodels/models/investor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-30 14:16:47.000000 fa-models-1.0.65/famodels/models/order.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-30 14:16:47.000000 fa-models-1.0.65/famodels/models/order_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-30 14:16:47.000000 fa-models-1.0.65/famodels/models/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-30 14:16:47.000000 fa-models-1.0.65/famodels/models/processed_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-30 14:16:47.000000 fa-models-1.0.65/famodels/models/side.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-30 14:16:47.000000 fa-models-1.0.65/famodels/models/signal_supplier.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-30 14:16:47.000000 fa-models-1.0.65/famodels/models/state_of_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-30 14:16:47.000000 fa-models-1.0.65/famodels/models/state_of_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-30 14:16:47.000000 fa-models-1.0.65/famodels/models/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-30 14:16:47.000000 fa-models-1.0.65/famodels/models/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-30 14:16:47.000000 fa-models-1.0.65/famodels/models/trading_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-30 14:16:47.000000 fa-models-1.0.65/famodels/models/virtual_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-30 14:17:07.000000 fa-models-1.0.65/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:17:16.296353 fa-models-1.0.65/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-30 14:16:47.000000 fa-models-1.0.65/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:17:16.296353 fa-models-1.0.65/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-30 14:16:47.000000 fa-models-1.0.65/tests/test_investor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-30 14:16:47.000000 fa-models-1.0.65/tests/test_processed_trading_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:58:37.148902 fa-models-1.0.66/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-01 17:58:37.148902 fa-models-1.0.66/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-01 17:58:02.000000 fa-models-1.0.66/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:58:37.144901 fa-models-1.0.66/fa_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-01 17:58:37.000000 fa-models-1.0.66/fa_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-01 17:58:37.000000 fa-models-1.0.66/fa_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 17:58:37.000000 fa-models-1.0.66/fa_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-01 17:58:37.000000 fa-models-1.0.66/fa_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-01 17:58:37.000000 fa-models-1.0.66/fa_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:58:37.144901 fa-models-1.0.66/famodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:58:37.148902 fa-models-1.0.66/famodels/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/investor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/order_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/processed_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/side.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/signal_supplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/state_of_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/state_of_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/trading_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/virtual_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-01 17:58:27.000000 fa-models-1.0.66/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 17:58:37.148902 fa-models-1.0.66/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-01 17:58:02.000000 fa-models-1.0.66/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:58:37.148902 fa-models-1.0.66/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-07-01 17:58:02.000000 fa-models-1.0.66/tests/test_investor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-01 17:58:02.000000 fa-models-1.0.66/tests/test_processed_trading_signal.py
```

### Comparing `fa-models-1.0.65/PKG-INFO` & `fa-models-1.0.66/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.65
-Summary: The library describes the most common models used in trading systems. It is based on sqlmodel and offers many built-in features like serialization and data generators.
+Version: 1.0.66
+Summary: A simple library of trading models.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # fa-models
 A set of models often used for trading services. The library offers merely models, tests and data and schema generators. The Schemas Generator offers to translate the models to Avro Schemas written in JSON.
 
 ## Sponsors
-Freya Alpha
-The Kára System
+Freya Alpha,
+The Kára System,
 Spark & Hale Robotic Industries
 
 ## TODO
 - [ ] Create Default values for enum, array, set, map, etc.
 
 ## General
 Run and compiled for Python 3.9.13.
@@ -114,15 +114,15 @@
 ```
 
 Upload to test-pypi to validate: 
 ```
 twine upload -r testpypi dist/*
 ```
 
-Login with username: svabra (password should be known)
+Login with username: (password should be known)
 
 If the test-upload was successful, finally, upload to pypi production: 
 
 ```
 twine upload dist/*
 ```
```

### Comparing `fa-models-1.0.65/README.md` & `fa-models-1.0.66/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # fa-models
 A set of models often used for trading services. The library offers merely models, tests and data and schema generators. The Schemas Generator offers to translate the models to Avro Schemas written in JSON.
 
 ## Sponsors
-Freya Alpha
-The Kára System
+Freya Alpha,
+The Kára System,
 Spark & Hale Robotic Industries
 
 ## TODO
 - [ ] Create Default values for enum, array, set, map, etc.
 
 ## General
 Run and compiled for Python 3.9.13.
@@ -101,15 +101,15 @@
 ```
 
 Upload to test-pypi to validate: 
 ```
 twine upload -r testpypi dist/*
 ```
 
-Login with username: svabra (password should be known)
+Login with username: (password should be known)
 
 If the test-upload was successful, finally, upload to pypi production: 
 
 ```
 twine upload dist/*
 ```
```

### Comparing `fa-models-1.0.65/fa_models.egg-info/PKG-INFO` & `fa-models-1.0.66/fa_models.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.65
-Summary: The library describes the most common models used in trading systems. It is based on sqlmodel and offers many built-in features like serialization and data generators.
+Version: 1.0.66
+Summary: A simple library of trading models.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # fa-models
 A set of models often used for trading services. The library offers merely models, tests and data and schema generators. The Schemas Generator offers to translate the models to Avro Schemas written in JSON.
 
 ## Sponsors
-Freya Alpha
-The Kára System
+Freya Alpha,
+The Kára System,
 Spark & Hale Robotic Industries
 
 ## TODO
 - [ ] Create Default values for enum, array, set, map, etc.
 
 ## General
 Run and compiled for Python 3.9.13.
@@ -114,15 +114,15 @@
 ```
 
 Upload to test-pypi to validate: 
 ```
 twine upload -r testpypi dist/*
 ```
 
-Login with username: svabra (password should be known)
+Login with username: (password should be known)
 
 If the test-upload was successful, finally, upload to pypi production: 
 
 ```
 twine upload dist/*
 ```
```

### Comparing `fa-models-1.0.65/fa_models.egg-info/SOURCES.txt` & `fa-models-1.0.66/fa_models.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -6,24 +6,21 @@
 fa_models.egg-info/dependency_links.txt
 fa_models.egg-info/requires.txt
 fa_models.egg-info/top_level.txt
 famodels/__init__.py
 famodels/models/__init__.py
 famodels/models/algorithm.py
 famodels/models/direction.py
-famodels/models/exchange_key.py
-famodels/models/fund.py
 famodels/models/investor.py
 famodels/models/order.py
 famodels/models/order_type.py
 famodels/models/person.py
 famodels/models/processed_signal.py
 famodels/models/side.py
 famodels/models/signal_supplier.py
 famodels/models/state_of_signal.py
 famodels/models/state_of_trade.py
-famodels/models/subscription.py
 famodels/models/trade.py
 famodels/models/trading_signal.py
 famodels/models/virtual_order.py
 tests/test_investor.py
 tests/test_processed_trading_signal.py
```

### Comparing `fa-models-1.0.65/famodels/models/algorithm.py` & `fa-models-1.0.66/famodels/models/algorithm.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 print(f"The env-var REDIS_OM_URL is: {REDIS_OM_URL}")
 
 class Algorithm(JsonModel):
     algo_id: str = Field(index=True)   
     provider_id: str = Field(index=True) 
     
     class Meta:
-        global_key_prefix="fa-investor-processing"
+        # global_key_prefix="fa-investor-processing"
         model_key_prefix="algorithm"
         database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
```

### Comparing `fa-models-1.0.65/famodels/models/fund.py` & `fa-models-1.0.66/famodels/models/order.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,38 @@
-from datetime import datetime
-import os
-from typing import List, Optional
-from redis_om import (Field, JsonModel, EmbeddedJsonModel)
+from typing import List, Set, Optional
+from famodels.models.state_of_trade import StateOfTrade
+from famodels.models.direction import Direction
+from famodels.models.order_type import OrderType
+from famodels.models.side import Side
+from redis_om import (Field, JsonModel)
 from redis_om.connections import get_redis_connection
-
-from famodels.models.subscription import Subscription
+import os
 
 REDIS_OM_URL = os.environ.get("REDIS_OM_URL")
 print(f"The env-var REDIS_OM_URL is: {REDIS_OM_URL}")
 
-class Fund(EmbeddedJsonModel):
-    fund_id:str = Field(index=True)
-    name:str = Field(index=True)
-    investor_id:str = Field(index=True)    
-    subscriptions: Optional[List[Subscription]] = Field(index=False)  
-    compounding: bool = Field(index=True)
-    absolute_max_amount: float
 
-    
+class Order(JsonModel):
+    """This model is for hot orders ONLY! Use ColdOrder for paper trading.
+    """
+    id: str = Field(index=True)
+    signal_id: str = Field(index=True)
+    algo_id: str = Field(index=True)
+    order_type: OrderType = Field(index=True, default=OrderType.LIMIT)        
+    market: str = Field(index=True)
+    exchange: str = Field(index=True)
+    direction: Direction = Field(index=True)
+    side: Side = Field(index=True)
+    price: float
+    amount: float    
+    account: str = Field(index=True)
+    pos_idx: int = Field(index=True)
+    timestamp_of_order: int = Field(index=True)
+    comission: float    
+
     class Meta:
-        global_key_prefix="fa-investor-processing"
-        model_key_prefix="fund"
+        # global_key_prefix="order-and-trade-processing"
+        model_key_prefix="order"
         database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
 
-    def add_subscription(self, subscription):
-        if subscription not in self.list_of_subscriptions:
-            self.list_of_subscriptions.append(subscription)
+    def __getitem__(self, key):
+        return self.__dict__[key]
```

### Comparing `fa-models-1.0.65/famodels/models/processed_signal.py` & `fa-models-1.0.66/famodels/models/processed_signal.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,12 +17,12 @@
     """
     id: Optional[str]
     """This id will be added by Freya Alpha."""
     status: StateOfSignal = Field(index=True)
     process_info: List[str]
 
     class Meta:
-        global_key_prefix="signal-processing"
+        # global_key_prefix="signal-processing"
         model_key_prefix="processed-signal"
         database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
 
 # Migrator().run()
```

### Comparing `fa-models-1.0.65/famodels/models/signal_supplier.py` & `fa-models-1.0.66/famodels/models/signal_supplier.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,10 +15,10 @@
     name: str = Field(index=True)
     accountable: Person = Field(index=True)
     contact: Person = Field(index=True)
     is_qualified: bool = Field(index=True, default=0)
     algorithms: List[Algorithm] = Field(index=True)
     
     class Meta:
-        global_key_prefix="fa-investor-processing"
+        # global_key_prefix="fa-investor-processing"
         model_key_prefix="signal-supplier"
         database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
```

### Comparing `fa-models-1.0.65/famodels/models/state_of_trade.py` & `fa-models-1.0.66/famodels/models/state_of_trade.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.65/famodels/models/trade.py` & `fa-models-1.0.66/famodels/models/trade.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     take_profit:Optional[int] = None
     stop_loss:Optional[int] = None
     """This is usually the receiving timestamp."""        
     profit_and_loss_percentage: Optional[float] = None
     profit_and_loss_amount: Optional[float] = None
 
     class Meta:
-        global_key_prefix="order-and-trade-processing"
+        # global_key_prefix="order-and-trade-processing"
         model_key_prefix="trade"
         database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
 
     def __getitem__(self, key):
         return self.__dict__[key]    
     
 # Migrator().run()
```

### Comparing `fa-models-1.0.65/famodels/models/trading_signal.py` & `fa-models-1.0.66/famodels/models/trading_signal.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,12 +48,12 @@
     # https://www.youtube.com/watch?v=ZP2j7bmWfmU
     timestamp_of_creation: int = Field(index=True)
     """The timestamp in milliseconds when the signal was created by the signal supplier."""
     timestamp_of_registration: Optional[int]
     """The timestamp in milliseconds when the signal was entering our interface. This will be overridden."""    
 
     class Meta:
-        global_key_prefix="signal-processing"
+        # global_key_prefix="signal-processing"
         model_key_prefix="raw-signal"
         database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
 
 # Migrator().run()
```

### Comparing `fa-models-1.0.65/famodels/models/virtual_order.py` & `fa-models-1.0.66/famodels/models/virtual_order.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.65/setup.py` & `fa-models-1.0.66/setup.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.65/tests/test_processed_trading_signal.py` & `fa-models-1.0.66/tests/test_processed_trading_signal.py`

 * *Files identical despite different names*

