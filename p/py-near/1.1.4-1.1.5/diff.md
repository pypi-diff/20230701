# Comparing `tmp/py_near-1.1.4.tar.gz` & `tmp/py_near-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_near-1.1.4.tar", max compression
+gzip compressed data, was "py_near-1.1.5.tar", max compression
```

## Comparing `py_near-1.1.4.tar` & `py_near-1.1.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1023 2022-06-08 20:31:53.650813 py_near-1.1.4/LICENSE
--rw-r--r--   0        0        0     3974 2023-01-24 19:13:04.795857 py_near-1.1.4/README.md
--rw-r--r--   0        0        0     1572 2023-06-30 22:41:35.919743 py_near-1.1.4/pyproject.toml
--rw-r--r--   0        0        0       50 2023-01-24 19:13:04.796695 py_near-1.1.4/src/py_near/__init__.py
--rw-r--r--   0        0        0    16398 2023-06-25 09:24:16.858826 py_near-1.1.4/src/py_near/account.py
--rw-r--r--   0        0        0      164 2023-05-05 18:03:26.714114 py_near-1.1.4/src/py_near/constants.py
--rw-r--r--   0        0        0        0 2023-01-24 19:13:04.797084 py_near-1.1.4/src/py_near/dapps/__init__.py
--rw-r--r--   0        0        0      231 2023-01-24 19:13:04.797225 py_near-1.1.4/src/py_near/dapps/core.py
--rw-r--r--   0        0        0       29 2023-01-24 19:13:04.797457 py_near-1.1.4/src/py_near/dapps/ft/__init__.py
--rw-r--r--   0        0        0     6717 2023-01-24 19:13:04.797637 py_near-1.1.4/src/py_near/dapps/ft/async_client.py
--rw-r--r--   0        0        0       92 2023-01-24 19:13:04.797752 py_near-1.1.4/src/py_near/dapps/ft/exceptions.py
--rw-r--r--   0        0        0      186 2023-01-24 19:13:04.797873 py_near-1.1.4/src/py_near/dapps/ft/models.py
--rw-r--r--   0        0        0      856 2023-01-24 19:13:04.797998 py_near-1.1.4/src/py_near/dapps/fts.py
--rw-r--r--   0        0        0       32 2023-01-24 19:13:04.798157 py_near-1.1.4/src/py_near/dapps/keypom/__init__.py
--rw-r--r--   0        0        0     1422 2023-01-24 19:13:04.798347 py_near-1.1.4/src/py_near/dapps/keypom/async_client.py
--rw-r--r--   0        0        0       45 2023-01-24 19:13:04.798480 py_near-1.1.4/src/py_near/dapps/keypom/exceptions.py
--rw-r--r--   0        0        0     2166 2023-01-24 19:13:04.798618 py_near-1.1.4/src/py_near/dapps/keypom/models.py
--rw-r--r--   0        0        0       32 2023-01-24 19:13:04.798770 py_near-1.1.4/src/py_near/dapps/phone/__init__.py
--rw-r--r--   0        0        0     6849 2023-01-24 19:13:04.799023 py_near-1.1.4/src/py_near/dapps/phone/async_client.py
--rw-r--r--   0        0        0       45 2023-01-24 19:13:04.799162 py_near-1.1.4/src/py_near/dapps/phone/exceptions.py
--rw-r--r--   0        0        0      332 2023-01-24 19:13:04.799299 py_near-1.1.4/src/py_near/dapps/phone/models.py
--rw-r--r--   0        0        0       34 2023-01-24 19:13:04.799462 py_near-1.1.4/src/py_near/dapps/staking/__init__.py
--rw-r--r--   0        0        0     5203 2023-01-24 19:13:04.799614 py_near-1.1.4/src/py_near/dapps/staking/async_client.py
--rw-r--r--   0        0        0       92 2023-01-24 19:13:04.799691 py_near-1.1.4/src/py_near/dapps/staking/exceptions.py
--rw-r--r--   0        0        0      124 2023-01-24 19:13:04.799806 py_near-1.1.4/src/py_near/dapps/staking/models.py
--rw-r--r--   0        0        0        0 2023-01-24 19:13:04.799907 py_near-1.1.4/src/py_near/exceptions/__init__.py
--rw-r--r--   0        0        0     4839 2023-06-23 06:51:52.490064 py_near-1.1.4/src/py_near/exceptions/exceptions.py
--rw-r--r--   0        0        0     7642 2023-06-23 01:16:29.606235 py_near-1.1.4/src/py_near/exceptions/provider.py
--rw-r--r--   0        0        0     9426 2023-06-30 22:36:51.489270 py_near-1.1.4/src/py_near/models.py
--rw-r--r--   0        0        0     8328 2023-06-26 04:51:57.598319 py_near-1.1.4/src/py_near/providers.py
--rw-r--r--   0        0        0     2566 2023-06-25 09:24:16.867476 py_near-1.1.4/src/py_near/transactions.py
--rw-r--r--   0        0        0      126 2023-06-26 04:51:57.591322 py_near-1.1.4/src/py_near/utils.py
--rw-r--r--   0        0        0     4661 1970-01-01 00:00:00.000000 py_near-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1023 2022-06-08 20:31:53.650813 py_near-1.1.5/LICENSE
+-rw-r--r--   0        0        0     3974 2023-01-24 19:13:04.795857 py_near-1.1.5/README.md
+-rw-r--r--   0        0        0     1572 2023-06-30 22:53:36.347696 py_near-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-01-24 19:13:04.796695 py_near-1.1.5/src/py_near/__init__.py
+-rw-r--r--   0        0        0    16388 2023-06-30 22:53:13.518209 py_near-1.1.5/src/py_near/account.py
+-rw-r--r--   0        0        0      164 2023-05-05 18:03:26.714114 py_near-1.1.5/src/py_near/constants.py
+-rw-r--r--   0        0        0        0 2023-01-24 19:13:04.797084 py_near-1.1.5/src/py_near/dapps/__init__.py
+-rw-r--r--   0        0        0      231 2023-01-24 19:13:04.797225 py_near-1.1.5/src/py_near/dapps/core.py
+-rw-r--r--   0        0        0       29 2023-01-24 19:13:04.797457 py_near-1.1.5/src/py_near/dapps/ft/__init__.py
+-rw-r--r--   0        0        0     6717 2023-01-24 19:13:04.797637 py_near-1.1.5/src/py_near/dapps/ft/async_client.py
+-rw-r--r--   0        0        0       92 2023-01-24 19:13:04.797752 py_near-1.1.5/src/py_near/dapps/ft/exceptions.py
+-rw-r--r--   0        0        0      186 2023-01-24 19:13:04.797873 py_near-1.1.5/src/py_near/dapps/ft/models.py
+-rw-r--r--   0        0        0      856 2023-01-24 19:13:04.797998 py_near-1.1.5/src/py_near/dapps/fts.py
+-rw-r--r--   0        0        0       32 2023-01-24 19:13:04.798157 py_near-1.1.5/src/py_near/dapps/keypom/__init__.py
+-rw-r--r--   0        0        0     1422 2023-01-24 19:13:04.798347 py_near-1.1.5/src/py_near/dapps/keypom/async_client.py
+-rw-r--r--   0        0        0       45 2023-01-24 19:13:04.798480 py_near-1.1.5/src/py_near/dapps/keypom/exceptions.py
+-rw-r--r--   0        0        0     2166 2023-01-24 19:13:04.798618 py_near-1.1.5/src/py_near/dapps/keypom/models.py
+-rw-r--r--   0        0        0       32 2023-01-24 19:13:04.798770 py_near-1.1.5/src/py_near/dapps/phone/__init__.py
+-rw-r--r--   0        0        0     6849 2023-01-24 19:13:04.799023 py_near-1.1.5/src/py_near/dapps/phone/async_client.py
+-rw-r--r--   0        0        0       45 2023-01-24 19:13:04.799162 py_near-1.1.5/src/py_near/dapps/phone/exceptions.py
+-rw-r--r--   0        0        0      332 2023-01-24 19:13:04.799299 py_near-1.1.5/src/py_near/dapps/phone/models.py
+-rw-r--r--   0        0        0       34 2023-01-24 19:13:04.799462 py_near-1.1.5/src/py_near/dapps/staking/__init__.py
+-rw-r--r--   0        0        0     5203 2023-01-24 19:13:04.799614 py_near-1.1.5/src/py_near/dapps/staking/async_client.py
+-rw-r--r--   0        0        0       92 2023-01-24 19:13:04.799691 py_near-1.1.5/src/py_near/dapps/staking/exceptions.py
+-rw-r--r--   0        0        0      124 2023-01-24 19:13:04.799806 py_near-1.1.5/src/py_near/dapps/staking/models.py
+-rw-r--r--   0        0        0        0 2023-01-24 19:13:04.799907 py_near-1.1.5/src/py_near/exceptions/__init__.py
+-rw-r--r--   0        0        0     4839 2023-06-23 06:51:52.490064 py_near-1.1.5/src/py_near/exceptions/exceptions.py
+-rw-r--r--   0        0        0     7642 2023-06-23 01:16:29.606235 py_near-1.1.5/src/py_near/exceptions/provider.py
+-rw-r--r--   0        0        0     9426 2023-06-30 22:36:51.489270 py_near-1.1.5/src/py_near/models.py
+-rw-r--r--   0        0        0     8328 2023-06-26 04:51:57.598319 py_near-1.1.5/src/py_near/providers.py
+-rw-r--r--   0        0        0     2566 2023-06-25 09:24:16.867476 py_near-1.1.5/src/py_near/transactions.py
+-rw-r--r--   0        0        0      126 2023-06-26 04:51:57.591322 py_near-1.1.5/src/py_near/utils.py
+-rw-r--r--   0        0        0     4661 1970-01-01 00:00:00.000000 py_near-1.1.5/PKG-INFO
```

### Comparing `py_near-1.1.4/LICENSE` & `py_near-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py_near-1.1.4/README.md` & `py_near-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `py_near-1.1.4/pyproject.toml` & `py_near-1.1.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-near"
-version = "1.1.4"
+version = "1.1.5"
 description="Pretty simple and fully asynchronous framework for working with NEAR blockchain"
 authors = ["pvolnov <petr@herewallet.app>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 ed25519 = "^1.5"
@@ -18,15 +18,15 @@
 flake8 = "^4.0.1"
 Sphinx = "^4.3.2"
 sphinx-rtd-theme = "^1.0.0"
 base58 = "^2.1.1"
 
 [project]
 name = "py-near"
-version = "1.1.3"
+version = "1.1.5"
 description = "Pretty simple and fully asynchronous framework for working with NEAR blockchaink"
 authors = [ {name = "pvolnov", email = "petr@herewallet.app"} ]
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 dependencies=["base58", "ed25519", "aiohttp", "py-near-primitives", "pydantic"]
 keywords = ["python", "near", "async"]
 classifiers = [
```

### Comparing `py_near-1.1.4/src/py_near/account.py` & `py_near-1.1.5/src/py_near/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             "latest_block_hash"
         ]
         self._latest_block_height = (await self._provider.get_status())["sync_info"][
             "latest_block_height"
         ]
         self._latest_block_hash_ts = utils.timestamp()
 
-    async def _sign_and_submit_tx(
+    async def sign_and_submit_tx(
         self, receiver_id, actions: List[Action], nowait=False
     ) -> Union[TransactionResult, str]:
         """
         Sign transaction and send it to blockchain
         :param receiver_id:
         :param actions: list of actions
         :param nowait: if nowait is True, return transaction hash, else wait execution
@@ -200,15 +200,15 @@
         """
         Send money to account_id
         :param account_id: receiver account id
         :param amount: amount in yoctoNEAR
         :param nowait: if nowait is True, return transaction hash, else wait execution
         :return: transaction hash or TransactionResult
         """
-        return await self._sign_and_submit_tx(
+        return await self.sign_and_submit_tx(
             account_id, [transactions.create_transfer_action(amount)], nowait
         )
 
     async def function_call(
         self,
         contract_id: str,
         method_name: str,
@@ -224,15 +224,15 @@
         :param args: json params for method
         :param gas: amount of attachment gas. Default is 200000000000000
         :param amount: amount of attachment NEAR, Default is 0
         :param nowait: if nowait is True, return transaction hash, else wait execution
         :return: transaction hash or TransactionResult
         """
         args = json.dumps(args).encode("utf8")
-        return await self._sign_and_submit_tx(
+        return await self.sign_and_submit_tx(
             contract_id,
             [transactions.create_function_call_action(method_name, args, gas, amount)],
             nowait,
         )
 
     async def create_account(
         self,
@@ -251,15 +251,15 @@
         :return: transaction hash or TransactionResult
         """
         actions = [
             transactions.create_create_account_action(),
             transactions.create_full_access_key_action(public_key),
             transactions.create_transfer_action(initial_balance),
         ]
-        return await self._sign_and_submit_tx(account_id, actions, nowait)
+        return await self.sign_and_submit_tx(account_id, actions, nowait)
 
     async def add_public_key(
         self,
         public_key: Union[str, bytes],
         receiver_id: str,
         method_names: List[str] = None,
         allowance: int = constants.ALLOWANCE,
@@ -277,41 +277,41 @@
         if method_names is None:
             method_names = []
         actions = [
             transactions.create_function_call_access_key_action(
                 public_key, allowance, receiver_id, method_names
             ),
         ]
-        return await self._sign_and_submit_tx(self.account_id, actions, nowait)
+        return await self.sign_and_submit_tx(self.account_id, actions, nowait)
 
     async def add_full_access_public_key(
         self, public_key: Union[str, bytes], nowait=False
     ) -> TransactionResult:
         """
         Add public key to account with full access
         :param public_key: public_key to add
         :param nowait: if nowait is True, return transaction hash, else wait execution
         :return: transaction hash or TransactionResult
         """
         actions = [
             transactions.create_full_access_key_action(public_key),
         ]
-        return await self._sign_and_submit_tx(self.account_id, actions, nowait)
+        return await self.sign_and_submit_tx(self.account_id, actions, nowait)
 
     async def delete_public_key(self, public_key: Union[str, bytes], nowait=False):
         """
         Delete public key from account
         :param public_key: public_key to delete
         :param nowait: is nowait is True, return transaction hash, else wait execution
         :return: transaction hash or TransactionResult
         """
         actions = [
             transactions.create_delete_access_key_action(public_key),
         ]
-        return await self._sign_and_submit_tx(self.account_id, actions, nowait)
+        return await self.sign_and_submit_tx(self.account_id, actions, nowait)
 
     async def call_delegate_transaction(
         self,
         delegate_action: Union[DelegateAction, DelegateActionModel],
         signature: Union[bytes, str],
         nowait=False,
     ):
@@ -319,40 +319,40 @@
             signature = base58.b58decode(signature.replace("ed25519:", ""))
         if isinstance(delegate_action, DelegateActionModel):
             delegate_action = delegate_action.near_delegate_action
 
         actions = [
             transactions.create_signed_delegate(delegate_action, signature),
         ]
-        return await self._sign_and_submit_tx(
+        return await self.sign_and_submit_tx(
             delegate_action.sender_id, actions, nowait
         )
 
     async def deploy_contract(self, contract_code: bytes, nowait=False):
         """
         Deploy smart contract to account
         :param contract_code: smart contract code
         :param nowait: if nowait is True, return transaction hash, else wait execution
         :return: transaction hash or TransactionResult
         """
-        return await self._sign_and_submit_tx(
+        return await self.sign_and_submit_tx(
             self.account_id,
             [transactions.create_deploy_contract_action(contract_code)],
             nowait,
         )
 
     async def stake(self, public_key: str, amount: str, nowait=False):
         """
         Stake NEAR on account. Account must have enough balance to be in validators pool
         :param public_key: public_key to stake
         :param amount: amount of NEAR to stake
         :param nowait: if nowait is True, return transaction hash, else wait execution
         :return: transaction hash or TransactionResult
         """
-        return await self._sign_and_submit_tx(
+        return await self.sign_and_submit_tx(
             self.account_id,
             [transactions.create_staking_action(public_key, amount)],
             nowait,
         )
 
     async def view_function(
         self, contract_id: str, method_name: str, args: dict
```

### Comparing `py_near-1.1.4/src/py_near/dapps/ft/async_client.py` & `py_near-1.1.5/src/py_near/dapps/ft/async_client.py`

 * *Files identical despite different names*

### Comparing `py_near-1.1.4/src/py_near/dapps/fts.py` & `py_near-1.1.5/src/py_near/dapps/fts.py`

 * *Files identical despite different names*

### Comparing `py_near-1.1.4/src/py_near/dapps/keypom/async_client.py` & `py_near-1.1.5/src/py_near/dapps/keypom/async_client.py`

 * *Files identical despite different names*

### Comparing `py_near-1.1.4/src/py_near/dapps/keypom/models.py` & `py_near-1.1.5/src/py_near/dapps/keypom/models.py`

 * *Files identical despite different names*

### Comparing `py_near-1.1.4/src/py_near/dapps/phone/async_client.py` & `py_near-1.1.5/src/py_near/dapps/phone/async_client.py`

 * *Files identical despite different names*

### Comparing `py_near-1.1.4/src/py_near/dapps/staking/async_client.py` & `py_near-1.1.5/src/py_near/dapps/staking/async_client.py`

 * *Files identical despite different names*

### Comparing `py_near-1.1.4/src/py_near/exceptions/exceptions.py` & `py_near-1.1.5/src/py_near/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `py_near-1.1.4/src/py_near/exceptions/provider.py` & `py_near-1.1.5/src/py_near/exceptions/provider.py`

 * *Files identical despite different names*

### Comparing `py_near-1.1.4/src/py_near/models.py` & `py_near-1.1.5/src/py_near/models.py`

 * *Files identical despite different names*

### Comparing `py_near-1.1.4/src/py_near/providers.py` & `py_near-1.1.5/src/py_near/providers.py`

 * *Files identical despite different names*

### Comparing `py_near-1.1.4/src/py_near/transactions.py` & `py_near-1.1.5/src/py_near/transactions.py`

 * *Files identical despite different names*

### Comparing `py_near-1.1.4/PKG-INFO` & `py_near-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-near
-Version: 1.1.4
+Version: 1.1.5
 Summary: Pretty simple and fully asynchronous framework for working with NEAR blockchain
 Author: pvolnov
 Author-email: petr@herewallet.app
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

