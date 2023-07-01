# Comparing `tmp/dark-gateway-0.0.1a0.tar.gz` & `tmp/dark-gateway-0.0.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dark-gateway-0.0.1a0.tar", last modified: Sat Jul  1 15:31:51 2023, max compression
+gzip compressed data, was "dark-gateway-0.0.1rc0.tar", last modified: Sat Jul  1 14:41:01 2023, max compression
```

## Comparing `dark-gateway-0.0.1a0.tar` & `dark-gateway-0.0.1rc0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:31:51.987171 dark-gateway-0.0.1a0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 15:31:48.000000 dark-gateway-0.0.1a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-01 15:31:51.987171 dark-gateway-0.0.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 15:31:48.000000 dark-gateway-0.0.1a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:31:51.987171 dark-gateway-0.0.1a0/dark/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-01 15:31:48.000000 dark-gateway-0.0.1a0/dark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:31:51.987171 dark-gateway-0.0.1a0/dark/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-01 15:31:48.000000 dark-gateway-0.0.1a0/dark/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-07-01 15:31:48.000000 dark-gateway-0.0.1a0/dark/gateway/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:31:51.987171 dark-gateway-0.0.1a0/dark/gateway/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 15:31:48.000000 dark-gateway-0.0.1a0/dark/gateway/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-07-01 15:31:48.000000 dark-gateway-0.0.1a0/dark/gateway/util/libs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13540 2023-07-01 15:31:48.000000 dark-gateway-0.0.1a0/dark/gateway/util/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:31:51.987171 dark-gateway-0.0.1a0/dark_gateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-01 15:31:51.000000 dark-gateway-0.0.1a0/dark_gateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-01 15:31:51.000000 dark-gateway-0.0.1a0/dark_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 15:31:51.000000 dark-gateway-0.0.1a0/dark_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-01 15:31:51.000000 dark-gateway-0.0.1a0/dark_gateway.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 15:31:51.987171 dark-gateway-0.0.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-01 15:31:50.000000 dark-gateway-0.0.1a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:41:01.017794 dark-gateway-0.0.1rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 14:40:58.000000 dark-gateway-0.0.1rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-01 14:41:01.017794 dark-gateway-0.0.1rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 14:40:58.000000 dark-gateway-0.0.1rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:41:01.017794 dark-gateway-0.0.1rc0/dark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 14:40:58.000000 dark-gateway-0.0.1rc0/dark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:41:01.017794 dark-gateway-0.0.1rc0/dark/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-01 14:40:58.000000 dark-gateway-0.0.1rc0/dark/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-01 14:40:58.000000 dark-gateway-0.0.1rc0/dark/gateway/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:41:01.017794 dark-gateway-0.0.1rc0/dark/gateway/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 14:40:58.000000 dark-gateway-0.0.1rc0/dark/gateway/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-07-01 14:40:58.000000 dark-gateway-0.0.1rc0/dark/gateway/util/libs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13540 2023-07-01 14:40:58.000000 dark-gateway-0.0.1rc0/dark/gateway/util/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 14:41:01.017794 dark-gateway-0.0.1rc0/dark_gateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-01 14:41:00.000000 dark-gateway-0.0.1rc0/dark_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-01 14:41:01.000000 dark-gateway-0.0.1rc0/dark_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 14:41:00.000000 dark-gateway-0.0.1rc0/dark_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-01 14:41:00.000000 dark-gateway-0.0.1rc0/dark_gateway.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 14:41:01.017794 dark-gateway-0.0.1rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-01 14:41:00.000000 dark-gateway-0.0.1rc0/setup.py
```

### Comparing `dark-gateway-0.0.1a0/LICENSE` & `dark-gateway-0.0.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dark-gateway-0.0.1a0/dark/gateway/core.py` & `dark-gateway-0.0.1rc0/dark/gateway/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,68 +17,46 @@
 
 # from eth_tester import PyEVMBackend
 from web3.providers.eth_tester import EthereumTesterProvider
 
 
 class DarkGateway:
     def __init__(self, blockchain_net_name: str,
-                 blockchain_config: configparser.SectionProxy):
+                 blockchain_config: configparser.SectionProxy,
+                 deployed_contracts_config:configparser.ConfigParser):
         
         #TODO: MODIFY CONSTRUCTOR PARAMATERS
         assert type(blockchain_net_name) == str, "blockchain_net_name must be str type"
         assert type(blockchain_config) == configparser.SectionProxy, "blockchain_config must be configparser.SectionProxy type"
-        
+        assert type(deployed_contracts_config) == configparser.ConfigParser, "deployed_contracts_config must be configparser.ConfigParser type"
 
         # w3dark config parameter
         self.__blockchain_net_name = blockchain_net_name
         self.__blockchain_config = blockchain_config
-        
+        self.__deployed_contracts_config = deployed_contracts_config
+
         # important variables
         self.w3 = self.__load_blockchain_driver(blockchain_net_name,blockchain_config)
         self.__deployed_contracts_dicts = None
-
-        # bc execution parameters
-        self.__chain_id,self.__min_gas_price,self.__pk = self.get_exec_parameters()
-
-        # account
-        self.account = self.w3.eth.account.privateKeyToAccount(self.__pk)
-
-  
-    def load_deployed_smart_contracts(self,deployed_contracts_config:configparser.ConfigParser):
+    
+    def load_deployed_smart_contracts(self):
         """
             Load the deployed smart contracts
             - Ity is essential notice that it is important to configure the smart contract
         """
-        assert type(deployed_contracts_config) == configparser.ConfigParser, "deployed_contracts_config must be configparser.ConfigParser type"
-        # self.__deployed_contracts_config = deployed_contracts_config
 
         contracts_dict = {}
-        for k in list(deployed_contracts_config.keys()):
+        for k in list(self.__deployed_contracts_config.keys()):
             if k != 'DEFAULT':
-                addr = deployed_contracts_config[k]['addr']
-                c_abi = ast.literal_eval(deployed_contracts_config[k]['abi'])['abi']
+                addr = self.__deployed_contracts_config[k]['addr']
+                c_abi = ast.literal_eval(self.__deployed_contracts_config[k]['abi'])['abi']
                 contracts_dict[k] = self.w3.eth.contract(address=addr, abi=c_abi)
 
         # TODO: CHECK IF CONTRANCT DICT ARE EMPTY
-        # return contracts_dict
-        self.deployed_contracts = contracts_dict
-        
-    
-    def get_exec_parameters(self):
-        """
-            Return the blockchain execution parameters
-            - chain_id
-            - ming_gas_price
-            - pk
-        """
-        
-        chain_id = int(self.blockchain_conf['chain_id'])
-        min_gas_price = int(self.blockchain_conf['min_gas_price'])
-        pk = self.blockchain_conf['account_priv_key']
-        return chain_id,min_gas_price,pk
+        return contracts_dict
 
 
     ###
     ### private methods
     ###
     def __load_blockchain_driver(blockchain_net_name: str,blockchain_config: configparser.SectionProxy) -> Web3:
         """
```

### Comparing `dark-gateway-0.0.1a0/dark/gateway/util/libs.py` & `dark-gateway-0.0.1rc0/dark/gateway/util/libs.py`

 * *Files identical despite different names*

### Comparing `dark-gateway-0.0.1a0/dark/gateway/util/setup.py` & `dark-gateway-0.0.1rc0/dark/gateway/util/setup.py`

 * *Files identical despite different names*

### Comparing `dark-gateway-0.0.1a0/setup.py` & `dark-gateway-0.0.1rc0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 local = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(local, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 
 # This gets deployed when a new release is made by github actions
-VERSION = '0.0.1a'
+VERSION = '0.0.1c'
 # VERSION = '0.0.1'
 
 # CHANGEME VARS
 PACKAGE_NAME = "dark-gateway"
 DESCRIPTION = 'dARK Gateway libs'
 LONG_DESCRIPTION = 'dARK web3 libs to connect applications to the dARK'
 AUTHOR_NAME = "Thiago Nóbrega"
```

