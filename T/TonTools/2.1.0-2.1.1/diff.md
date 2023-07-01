# Comparing `tmp/TonTools-2.1.0.tar.gz` & `tmp/TonTools-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/TonTools-2.1.0.tar", last modified: Tue Jun  6 11:47:59 2023, max compression
+gzip compressed data, was "dist/TonTools-2.1.1.tar", last modified: Sat Jul  1 13:19:37 2023, max compression
```

## Comparing `TonTools-2.1.0.tar` & `TonTools-2.1.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-06-06 11:47:59.696432 TonTools-2.1.0/
--rw-r--r--   0 maxankurb   (501) staff       (20)     1071 2023-03-09 07:49:38.000000 TonTools-2.1.0/LICENSE
--rw-r--r--   0 maxankurb   (501) staff       (20)      202 2023-06-06 11:47:59.695809 TonTools-2.1.0/PKG-INFO
--rw-r--r--   0 maxankurb   (501) staff       (20)    11394 2023-05-27 17:27:22.000000 TonTools-2.1.0/README.md
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-06-06 11:47:59.685202 TonTools-2.1.0/TonTools/
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-06-06 11:47:59.691533 TonTools-2.1.0/TonTools/Contracts/
--rw-r--r--   0 maxankurb   (501) staff       (20)     5305 2023-05-22 11:16:39.000000 TonTools-2.1.0/TonTools/Contracts/Contract.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     3909 2023-06-06 11:47:34.000000 TonTools-2.1.0/TonTools/Contracts/Jetton.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     5661 2023-03-01 07:15:23.000000 TonTools-2.1.0/TonTools/Contracts/NFT.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     6091 2023-03-29 17:48:14.000000 TonTools-2.1.0/TonTools/Contracts/Wallet.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     1336 2023-05-22 11:16:39.000000 TonTools-2.1.0/TonTools/Contracts/utils.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-06-06 11:47:59.695362 TonTools-2.1.0/TonTools/Providers/
--rw-r--r--   0 maxankurb   (501) staff       (20)    21420 2023-06-06 11:47:34.000000 TonTools-2.1.0/TonTools/Providers/DtonClient.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    15041 2023-03-01 08:22:28.000000 TonTools-2.1.0/TonTools/Providers/LsClient.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    10949 2023-05-22 11:16:39.000000 TonTools-2.1.0/TonTools/Providers/TonApiClient.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    16109 2023-05-25 19:05:58.000000 TonTools-2.1.0/TonTools/Providers/TonCenterClient.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     2568 2023-06-06 11:47:34.000000 TonTools-2.1.0/TonTools/Providers/utils.py
--rw-r--r--   0 maxankurb   (501) staff       (20)      323 2023-05-22 11:16:39.000000 TonTools-2.1.0/TonTools/__init__.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-06-06 11:47:59.688285 TonTools-2.1.0/TonTools.egg-info/
--rw-r--r--   0 maxankurb   (501) staff       (20)      202 2023-06-06 11:47:59.000000 TonTools-2.1.0/TonTools.egg-info/PKG-INFO
--rw-r--r--   0 maxankurb   (501) staff       (20)      514 2023-06-06 11:47:59.000000 TonTools-2.1.0/TonTools.egg-info/SOURCES.txt
--rw-r--r--   0 maxankurb   (501) staff       (20)        1 2023-06-06 11:47:59.000000 TonTools-2.1.0/TonTools.egg-info/dependency_links.txt
--rw-r--r--   0 maxankurb   (501) staff       (20)      114 2023-06-06 11:47:59.000000 TonTools-2.1.0/TonTools.egg-info/requires.txt
--rw-r--r--   0 maxankurb   (501) staff       (20)       47 2023-06-06 11:47:59.000000 TonTools-2.1.0/TonTools.egg-info/top_level.txt
--rw-r--r--   0 maxankurb   (501) staff       (20)       38 2023-06-06 11:47:59.696542 TonTools-2.1.0/setup.cfg
--rw-r--r--   0 maxankurb   (501) staff       (20)      513 2023-06-06 11:47:55.000000 TonTools-2.1.0/setup.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-01 13:19:37.806505 TonTools-2.1.1/
+-rw-r--r--   0 maxankurb   (501) staff       (20)     1071 2023-03-09 07:49:38.000000 TonTools-2.1.1/LICENSE
+-rw-r--r--   0 maxankurb   (501) staff       (20)      202 2023-07-01 13:19:37.806196 TonTools-2.1.1/PKG-INFO
+-rw-r--r--   0 maxankurb   (501) staff       (20)    11720 2023-07-01 13:13:19.000000 TonTools-2.1.1/README.md
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-01 13:19:37.797068 TonTools-2.1.1/TonTools/
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-01 13:19:37.801349 TonTools-2.1.1/TonTools/Contracts/
+-rw-r--r--   0 maxankurb   (501) staff       (20)     5376 2023-07-01 13:03:20.000000 TonTools-2.1.1/TonTools/Contracts/Contract.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     3909 2023-06-06 11:47:34.000000 TonTools-2.1.1/TonTools/Contracts/Jetton.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     5661 2023-03-01 07:15:23.000000 TonTools-2.1.1/TonTools/Contracts/NFT.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     6091 2023-03-29 17:48:14.000000 TonTools-2.1.1/TonTools/Contracts/Wallet.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     1336 2023-05-22 11:16:39.000000 TonTools-2.1.1/TonTools/Contracts/utils.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-01 13:19:37.805796 TonTools-2.1.1/TonTools/Providers/
+-rw-r--r--   0 maxankurb   (501) staff       (20)    21420 2023-06-06 11:47:34.000000 TonTools-2.1.1/TonTools/Providers/DtonClient.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    15041 2023-03-01 08:22:28.000000 TonTools-2.1.1/TonTools/Providers/LsClient.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    10949 2023-05-22 11:16:39.000000 TonTools-2.1.1/TonTools/Providers/TonApiClient.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    16477 2023-07-01 13:07:06.000000 TonTools-2.1.1/TonTools/Providers/TonCenterClient.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     4437 2023-07-01 12:59:15.000000 TonTools-2.1.1/TonTools/Providers/_orbs_ton_access.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     2569 2023-07-01 12:46:44.000000 TonTools-2.1.1/TonTools/Providers/utils.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)      323 2023-05-22 11:16:39.000000 TonTools-2.1.1/TonTools/__init__.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-01 13:19:37.799027 TonTools-2.1.1/TonTools.egg-info/
+-rw-r--r--   0 maxankurb   (501) staff       (20)      202 2023-07-01 13:19:37.000000 TonTools-2.1.1/TonTools.egg-info/PKG-INFO
+-rw-r--r--   0 maxankurb   (501) staff       (20)      553 2023-07-01 13:19:37.000000 TonTools-2.1.1/TonTools.egg-info/SOURCES.txt
+-rw-r--r--   0 maxankurb   (501) staff       (20)        1 2023-07-01 13:19:37.000000 TonTools-2.1.1/TonTools.egg-info/dependency_links.txt
+-rw-r--r--   0 maxankurb   (501) staff       (20)      114 2023-07-01 13:19:37.000000 TonTools-2.1.1/TonTools.egg-info/requires.txt
+-rw-r--r--   0 maxankurb   (501) staff       (20)       47 2023-07-01 13:19:37.000000 TonTools-2.1.1/TonTools.egg-info/top_level.txt
+-rw-r--r--   0 maxankurb   (501) staff       (20)       38 2023-07-01 13:19:37.806592 TonTools-2.1.1/setup.cfg
+-rw-r--r--   0 maxankurb   (501) staff       (20)      513 2023-07-01 13:17:10.000000 TonTools-2.1.1/setup.py
```

### Comparing `TonTools-2.1.0/LICENSE` & `TonTools-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TonTools-2.1.0/README.md` & `TonTools-2.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,20 +34,28 @@
 
 ### TonCenterClient
 
 [TonCenter](https://toncenter.com/api/v2/) is an Api which uses [lite servers](https://ton.org/docs/participate/nodes/node-types)
 
 To initialize TonCenterClient: 
 ```python
-client = TonCenterClient(base_url='http://127.0.0.1:80/', addresses_form=addresses_form)
+client = TonCenterClient(base_url='http://127.0.0.1:80/')
 or
-client = TonCenterClient(api_key, addresses_form)
+client = TonCenterClient(api_key)
 ```
 Notice that TonCenter has Limit 10 RPS with Api Key, so It's highly recommend to use [Local TonCenter](https://github.com/toncenter/ton-http-api) 
-and specify your host in `base_url` parameter.
+and specify your host in `base_url` parameter or use the [Orbs Ton Access](https://www.orbs.com/ton-access/): 
+
+```python
+client = TonCenterClient(orbs_access=True,
+                         testnet=True)
+
+contract = Contract('EQBvW8Z5huBkMJYdnfAEM5JqTNkuWX3diqYENkWsIL0XggGG', client)
+print((await contract.get_transactions(limit=10))[-1].out_msgs[0].destination)  # kQCdaMggjCXoW867yRXilPw2bu8Av9dSBlGGCdDPIGNLKM8N
+```
 
 ### LsClient
 
 **LsClient** gets data from blockhain using [lite servers](https://ton.org/docs/participate/nodes/node-types) (based on [pytonlib](https://github.com/psylopunk/pytonlib))
 
 To initialize LsClient: 
 ```python
```

### Comparing `TonTools-2.1.0/TonTools/Contracts/Contract.py` & `TonTools-2.1.1/TonTools/Contracts/Contract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import base64
 import json
+import typing
 
 from tonsdk.utils import Address, InvalidAddressError, b64str_to_bytes
 from tonsdk.boc import Cell, Slice
 from .utils import transaction_status, known_prefixes
 
 
 def isBase64(sb):
@@ -81,16 +82,16 @@
     def __init__(self, data: dict):
         self.utime = data['utime']
         self.fee = data['fee']
         self.data = data['data']
         self.hash = data['hash']
         self.lt = data['lt']
         self.status = transaction_status(data['data']) if 'status' not in data else data['status']
-        self.in_msg = InMsg(data['in_msg'])
-        self.out_msgs = [OutMsg(out_msg) for out_msg in data['out_msgs']]
+        self.in_msg: InMsg = InMsg(data['in_msg'])
+        self.out_msgs: typing.List[OutMsg] = [OutMsg(out_msg) for out_msg in data['out_msgs']]
 
     def to_dict(self):
         return {
             'utime': self.utime,
             'fee': self.fee,
             'data': self.data,
             'hash': self.hash,
@@ -135,15 +136,15 @@
 
 class Contract:
     def __init__(self, address, provider):
         Address(address)  # raises tonsdk.utils.InvalidAddressError if address is not valid
         self.address = address
         self.provider = provider
 
-    async def get_transactions(self, limit: int = 10**9, limit_per_one_request: int = 100):
+    async def get_transactions(self, limit: int = 10**9, limit_per_one_request: int = 100)  -> typing.List[Transaction]:
         return await self.provider.get_transactions(self.address, limit, limit_per_one_request)
 
     async def run_get_method(self, method: str, stack: list):  # TonCenterClient or LsClient required
         """
         Please, note that currently the response types for TonCenterClient, LsClient and DtonClient are different.
         Will be improved in future versions.
         """
```

### Comparing `TonTools-2.1.0/TonTools/Contracts/Jetton.py` & `TonTools-2.1.1/TonTools/Contracts/Jetton.py`

 * *Files identical despite different names*

### Comparing `TonTools-2.1.0/TonTools/Contracts/NFT.py` & `TonTools-2.1.1/TonTools/Contracts/NFT.py`

 * *Files identical despite different names*

### Comparing `TonTools-2.1.0/TonTools/Contracts/Wallet.py` & `TonTools-2.1.1/TonTools/Contracts/Wallet.py`

 * *Files identical despite different names*

### Comparing `TonTools-2.1.0/TonTools/Contracts/utils.py` & `TonTools-2.1.1/TonTools/Contracts/utils.py`

 * *Files identical despite different names*

### Comparing `TonTools-2.1.0/TonTools/Providers/DtonClient.py` & `TonTools-2.1.1/TonTools/Providers/DtonClient.py`

 * *Files identical despite different names*

### Comparing `TonTools-2.1.0/TonTools/Providers/LsClient.py` & `TonTools-2.1.1/TonTools/Providers/LsClient.py`

 * *Files identical despite different names*

### Comparing `TonTools-2.1.0/TonTools/Providers/TonApiClient.py` & `TonTools-2.1.1/TonTools/Providers/TonApiClient.py`

 * *Files identical despite different names*

### Comparing `TonTools-2.1.0/TonTools/Providers/TonCenterClient.py` & `TonTools-2.1.1/TonTools/Providers/TonCenterClient.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from tonsdk.utils import Address, bytes_to_b64str
 
 from ..Contracts.NFT import NftItem, NftCollection
 from ..Contracts.Contract import Transaction
 from ..Contracts.Wallet import Wallet
 from ..Contracts.Jetton import Jetton, JettonWallet
 from .utils import markets_adresses, get, process_jetton_data
+from ._orbs_ton_access import get_http_endpoint
 
 
 class TonCenterClientError(BaseException):
     pass
 
 
 class GetMethodError(TonCenterClientError):
@@ -35,27 +36,34 @@
 
 class TonCenterClient:
 
     def __init__(self,
                  key: str = None,
                  addresses_form='user_friendly',  # addresses_form could be 'raw' or 'user_friendly'.
                  base_url=None,
-                 testnet=False
+                 testnet=False,
+                 orbs_access=False  # https://www.orbs.com/ton-access/
                  ):
         self.form = addresses_form
         self.delay = 0
         self.base_url = base_url
+        self.testnet = testnet
+        if orbs_access:
+            self.headers = {}
+            if testnet:
+                self.base_url = get_http_endpoint({'network': 'testnet', 'protocol': 'rest'})
+                return
+            self.base_url = get_http_endpoint({'protocol': 'rest'})
+            return
         if testnet:
-            self.testnet = True
             if base_url is None:
                 self.base_url = 'https://testnet.toncenter.com/api/v2/'
             else:
                 self.base_url = base_url
         else:
-            self.testnet = False
             if base_url is None:
                 self.base_url = 'https://toncenter.com/api/v2/'
             else:
                 self.base_url = base_url
         if key:
             self.headers = {
                 'X-API-Key': key
```

### Comparing `TonTools-2.1.0/TonTools/Providers/utils.py` & `TonTools-2.1.1/TonTools/Providers/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -48,8 +48,8 @@
             return await response.json(content_type=None)
 
 markets_adresses = {
     '0:584ee61b2dff0837116d0fcb5078d93964bcbe9c05fd6a141b1bfca5d6a43e18': 'Getgems Sales',
     '0:a3935861f79daf59a13d6d182e1640210c02f98e3df18fda74b8f5ab141abf18': 'Getgems Sales',
     '0:eb2eaf97ea32993470127208218748758a88374ad2bbd739fc75c9ab3a3f233d': 'Disintar Marketplace',
     '0:1ecdb7672d5b0b4aaf2d9d5573687c7190aa6849804d9e7d7aef71975ac03e2e': 'TON Diamonds'
-}
+}
```

### Comparing `TonTools-2.1.0/setup.py` & `TonTools-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 import setuptools
 
 requirements = ["tonsdk>=1.0.13", "ton>=0.26", "aiohttp>=3.8.1", "setuptools>=65.3.0", "requests>=2.28.1", "pytonlib>=0.0.46", "graphql-query==1.0.3"]
 
 setup(
     name='TonTools',
-    version='2.1.0',
+    version='2.1.1',
     packages=['TonTools', 'TonTools/Contracts', 'TonTools/Providers'],
     url='',
     license='MIT License',
     author='yungwine',
     author_email='cyrbatoff@gmail.com',
     description='Explore TON Blockchain with python',
     install_requires=requirements,
```

