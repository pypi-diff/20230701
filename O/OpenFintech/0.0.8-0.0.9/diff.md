# Comparing `tmp/OpenFintech-0.0.8.tar.gz` & `tmp/OpenFintech-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenFintech-0.0.8.tar", last modified: Fri Jun 30 23:20:09 2023, max compression
+gzip compressed data, was "OpenFintech-0.0.9.tar", last modified: Sat Jul  1 00:10:38 2023, max compression
```

## Comparing `OpenFintech-0.0.8.tar` & `OpenFintech-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-06-30 23:20:09.291715 OpenFintech-0.0.8/
--rw-r--r--   0 harri      (501) staff       (20)    11357 2023-06-05 19:27:30.000000 OpenFintech-0.0.8/LICENSE
-drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-06-30 23:20:09.290403 OpenFintech-0.0.8/OpenFintech/
--rw-r--r--   0 harri      (501) staff       (20)     6253 2023-06-30 23:16:16.000000 OpenFintech-0.0.8/OpenFintech/FinData.py
--rw-r--r--   0 harri      (501) staff       (20)     3643 2023-06-30 18:57:40.000000 OpenFintech-0.0.8/OpenFintech/FinMongo.py
--rw-r--r--   0 harri      (501) staff       (20)     2407 2023-06-30 20:43:07.000000 OpenFintech-0.0.8/OpenFintech/Market.py
--rw-r--r--   0 harri      (501) staff       (20)     5495 2023-06-30 20:43:08.000000 OpenFintech-0.0.8/OpenFintech/Model.py
--rw-r--r--   0 harri      (501) staff       (20)     7511 2023-06-30 18:57:40.000000 OpenFintech-0.0.8/OpenFintech/User.py
--rw-r--r--   0 harri      (501) staff       (20)      225 2023-06-30 18:57:40.000000 OpenFintech-0.0.8/OpenFintech/__init__.py
--rw-r--r--   0 harri      (501) staff       (20)      855 2023-06-30 18:57:40.000000 OpenFintech-0.0.8/OpenFintech/utilities.py
-drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-06-30 23:20:09.291303 OpenFintech-0.0.8/OpenFintech.egg-info/
--rw-r--r--   0 harri      (501) staff       (20)       77 2023-06-30 23:20:09.000000 OpenFintech-0.0.8/OpenFintech.egg-info/PKG-INFO
--rw-r--r--   0 harri      (501) staff       (20)      325 2023-06-30 23:20:09.000000 OpenFintech-0.0.8/OpenFintech.egg-info/SOURCES.txt
--rw-r--r--   0 harri      (501) staff       (20)        1 2023-06-30 23:20:09.000000 OpenFintech-0.0.8/OpenFintech.egg-info/dependency_links.txt
--rw-r--r--   0 harri      (501) staff       (20)       12 2023-06-30 23:20:09.000000 OpenFintech-0.0.8/OpenFintech.egg-info/top_level.txt
--rw-r--r--   0 harri      (501) staff       (20)       77 2023-06-30 23:20:09.291542 OpenFintech-0.0.8/PKG-INFO
--rw-r--r--   0 harri      (501) staff       (20)    11338 2023-06-13 17:15:54.000000 OpenFintech-0.0.8/README.md
--rw-r--r--   0 harri      (501) staff       (20)       38 2023-06-30 23:20:09.291765 OpenFintech-0.0.8/setup.cfg
--rw-r--r--   0 harri      (501) staff       (20)      128 2023-06-30 23:19:42.000000 OpenFintech-0.0.8/setup.py
+drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-07-01 00:10:38.934098 OpenFintech-0.0.9/
+-rw-r--r--   0 harri      (501) staff       (20)    11357 2023-06-05 19:27:30.000000 OpenFintech-0.0.9/LICENSE
+drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-07-01 00:10:38.932693 OpenFintech-0.0.9/OpenFintech/
+-rw-r--r--   0 harri      (501) staff       (20)     6200 2023-07-01 00:10:16.000000 OpenFintech-0.0.9/OpenFintech/FinData.py
+-rw-r--r--   0 harri      (501) staff       (20)     2472 2023-06-30 23:37:45.000000 OpenFintech-0.0.9/OpenFintech/FinMongo.py
+-rw-r--r--   0 harri      (501) staff       (20)     1779 2023-07-01 00:10:15.000000 OpenFintech-0.0.9/OpenFintech/Market.py
+-rw-r--r--   0 harri      (501) staff       (20)     5495 2023-06-30 23:33:41.000000 OpenFintech-0.0.9/OpenFintech/Model.py
+-rw-r--r--   0 harri      (501) staff       (20)     7511 2023-06-30 23:50:27.000000 OpenFintech-0.0.9/OpenFintech/User.py
+-rw-r--r--   0 harri      (501) staff       (20)      225 2023-06-30 23:34:44.000000 OpenFintech-0.0.9/OpenFintech/__init__.py
+-rw-r--r--   0 harri      (501) staff       (20)      855 2023-06-30 18:57:40.000000 OpenFintech-0.0.9/OpenFintech/utilities.py
+drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-07-01 00:10:38.933693 OpenFintech-0.0.9/OpenFintech.egg-info/
+-rw-r--r--   0 harri      (501) staff       (20)       77 2023-07-01 00:10:38.000000 OpenFintech-0.0.9/OpenFintech.egg-info/PKG-INFO
+-rw-r--r--   0 harri      (501) staff       (20)      325 2023-07-01 00:10:38.000000 OpenFintech-0.0.9/OpenFintech.egg-info/SOURCES.txt
+-rw-r--r--   0 harri      (501) staff       (20)        1 2023-07-01 00:10:38.000000 OpenFintech-0.0.9/OpenFintech.egg-info/dependency_links.txt
+-rw-r--r--   0 harri      (501) staff       (20)       12 2023-07-01 00:10:38.000000 OpenFintech-0.0.9/OpenFintech.egg-info/top_level.txt
+-rw-r--r--   0 harri      (501) staff       (20)       77 2023-07-01 00:10:38.933923 OpenFintech-0.0.9/PKG-INFO
+-rw-r--r--   0 harri      (501) staff       (20)    11338 2023-06-13 17:15:54.000000 OpenFintech-0.0.9/README.md
+-rw-r--r--   0 harri      (501) staff       (20)       38 2023-07-01 00:10:38.934151 OpenFintech-0.0.9/setup.cfg
+-rw-r--r--   0 harri      (501) staff       (20)      128 2023-07-01 00:10:21.000000 OpenFintech-0.0.9/setup.py
```

### Comparing `OpenFintech-0.0.8/LICENSE` & `OpenFintech-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenFintech-0.0.8/OpenFintech/FinData.py` & `OpenFintech-0.0.9/OpenFintech/FinData.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from .utilities import create_logger
 from .FinMongo import FinMongo
 from datetime import datetime as dt
-from coincap import CoinCap
 import pandas as pd
 import requests
 
-# TODO: 
-    # Handling edge cases (where error occurs when the DB has no data, how to loop and get the data and sucessfully handle the method call)
-    # Crypto overview and intraday methods (would require seperate logic for handling keys)
+# TODO:     
     # Static methods that extend any given timeseries price data pandas DF with indicator data
+    # Crypto Intraday method (can be pulled from Alphavantage)
     # Verify that Pymongo find_one is returning the last record of the collection (by ticker)
+    # Handling edge cases (where error occurs when the DB has no data, how to loop and get the data and sucessfully handle the method call)
 
 
 class FinData:
     def __init__(self, database=None, logger=None, key="", keys=[], refresh=30):
 
         # Setup logger if required
         if logger==None: logger=create_logger("market")
```

### Comparing `OpenFintech-0.0.8/OpenFintech/FinMongo.py` & `OpenFintech-0.0.9/OpenFintech/FinMongo.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import logging
 import pymongo_inmemory
 from pymongo import MongoClient, errors
 from .utilities import create_logger
 # TODO: 
-# Finish __str__
-# Add CRUD features (with returns optionally in Pandas DF's)
-# Add custom error message returns (dict/JSON like an API would)
+# Add static function that, given a collection, returns the last record that was entered into it (carrying any other filter as given)
 
 class FinMongo:
 
     def __init__(self, host: str = None, logger:logging.Logger = None):
 
         if logger==None: logger = create_logger("finmongo")
         self.logger=logger
@@ -59,41 +57,8 @@
                 docs = collection.count_documents({})
                 c_info = {
                     'collection': c_name,
                     'doc_count': docs
                 }
                 db_info["collections"].append(c_info)
             database_info.append(db_info)
-        return str(database_info)
-
-if __name__ == "__main__": 
-    import os 
-    from dotenv import load_dotenv
-    load_dotenv()
-    MONGO_USER = os.getenv('MONGO_USER')
-    MONGO_PASS = os.getenv('MONGO_PASS') 
-    #handler = FinMongo(f"mongodb+srv://{MONGO_USER}:{MONGO_PASS}@cluster0.lvkyalc.mongodb.net/?retryWrites=true&w=majority")     
-    handler = FinMongo() # in-memory
-    client = handler.client
-
-    # Code to test db, collection, and document creation
-    # In MongoDB, db's and collections are not created untill they have data added to them
-    mydb = client["mydatabase"]
-    mycol = mydb["users"]
-    sample_data = {
-        "date_created": None,
-        "user_id": 3, "username": "Brown",
-        # For analytical purposes
-        "major":"CS", "year": 30,
-        "email": None, "password": None
-    }
-
-    #x = mycol.insert_one(sample_data)
-    #print(client.list_database_names())
-    #print(mydb.list_collection_names())
-    #print(x.inserted_id)
-    
-    # Debug:
-    print("------------Printing Handler--------------")
-    print(handler)
-    print("Attempting to disconnect handler")
-    handler.disconnect() # Disconnect the handler (and the MongoDB client) after use
+        return str(database_info)
```

### Comparing `OpenFintech-0.0.8/OpenFintech/Market.py` & `OpenFintech-0.0.9/OpenFintech/Market.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from .utilities import create_logger
 from .FinMongo import FinMongo
 # TODO:
-# Position CRUD Functions
 # Trade CRUD Functions
-# NOTE: (Required) Integrate FinData (Alphavantage Wrapper Package) into Market to get the required Trade and Position Data. The Market package should also be able to return this data when requested.
 # Implement __str__ to provide an overview of the market
 
 class Market: # Provides simulated backtesting and real-time testing functionalities.
 
     def __init__(self, database=None, logger=None):
         
         if logger==None: logger=create_logger("market")
@@ -21,63 +19,35 @@
 
         self.database = database
         self.positions = self.database["positions"]
         self.buffer = {} # NOTE: {{open_position: awaiting signal,..} -> Replaced with associated closing position before being registered as a trade # NOTE: This is something to take into consideration when designing the ERD for the system/software
         self.trades = self.database["trades"]
         return
 
-    # Realtime (Provides simulated running functionality)
-    def open_position(self):
-        return
-    
-    def close_position(self):
-        return
-    
-    def update_position(self):
-        return
-    
-    def view_position(self):
-        return
-
-    # Backtesting 
+    # TODO: Backtesting (NOTE: Use the ERD and other CRUD functions for reference. Keep default parameters in mind. Feel free to create static methods if you need)
     def create_trade(self):
         return
-    
     def read_trade(self):
         return
-    
     def update_tade(self):
         return
-    
     def delete_trade(self):
         return
     
+    # Realtime (Provides simulated running functionality) NOTE: Ignore these for now
+    def open_position(self):
+        return
+    def close_position(self):
+        return
+    def update_position(self):
+        return
+    def view_position(self):
+        return
+
     # Close database and cleanup
     def close(self):
         if self.inmemory==True: self.mongo.disconnect()
         return
     
     # For providing an overview of the market
     def __str__(self):
         return
-
-
-if __name__=='__main__':
-    sample_trade = {
-        "date_created":None, 
-        "trade_dt":None,
-        # Composite primary key for identifying this document (for future reference)
-        "user_id":None, 
-        "config_id":None,
-        # For identifying the trade and its related session
-        "session_id":None, 
-        "trade_id":None, 
-        # Trade information
-        "ticker":None, 
-        "type":None, 
-        "price":None, 
-        "quantity":None, 
-        "total":None
-    }
-
-    market = Market()
-    market.close()
```

### Comparing `OpenFintech-0.0.8/OpenFintech/Model.py` & `OpenFintech-0.0.9/OpenFintech/Model.py`

 * *Files identical despite different names*

### Comparing `OpenFintech-0.0.8/OpenFintech/User.py` & `OpenFintech-0.0.9/OpenFintech/User.py`

 * *Files identical despite different names*

### Comparing `OpenFintech-0.0.8/OpenFintech/utilities.py` & `OpenFintech-0.0.9/OpenFintech/utilities.py`

 * *Files identical despite different names*

### Comparing `OpenFintech-0.0.8/README.md` & `OpenFintech-0.0.9/README.md`

 * *Files identical despite different names*

