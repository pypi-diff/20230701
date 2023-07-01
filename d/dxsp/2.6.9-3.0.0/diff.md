# Comparing `tmp/dxsp-2.6.9.tar.gz` & `tmp/dxsp-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.6.9.tar", max compression
+gzip compressed data, was "dxsp-3.0.0.tar", max compression
```

## Comparing `dxsp-2.6.9.tar` & `dxsp-3.0.0.tar`

### file list

```diff
@@ -1,8 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-06-11 11:51:34.177079 dxsp-2.6.9/LICENSE
--rw-r--r--   0        0        0     2348 2023-06-11 11:51:34.177079 dxsp-2.6.9/README.md
--rw-r--r--   0        0        0       86 2023-06-11 11:51:55.705159 dxsp-2.6.9/dxsp/__init__.py
--rw-r--r--   0        0        0      387 2023-06-11 11:51:34.177079 dxsp-2.6.9/dxsp/config.py
--rw-r--r--   0        0        0     3699 2023-06-11 11:51:34.177079 dxsp-2.6.9/dxsp/default_settings.toml
--rw-r--r--   0        0        0    18704 2023-06-11 11:51:34.177079 dxsp-2.6.9/dxsp/main.py
--rw-r--r--   0        0        0     1552 2023-06-11 11:51:55.705159 dxsp-2.6.9/pyproject.toml
--rw-r--r--   0        0        0     3154 1970-01-01 00:00:00.000000 dxsp-2.6.9/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-01 17:42:01.895242 dxsp-3.0.0/LICENSE
+-rw-r--r--   0        0        0     2339 2023-07-01 17:42:01.895242 dxsp-3.0.0/README.md
+-rw-r--r--   0        0        0      114 2023-07-01 17:42:02.795255 dxsp-3.0.0/dxsp/__init__.py
+-rw-r--r--   0        0        0      418 2023-07-01 17:42:01.895242 dxsp-3.0.0/dxsp/config.py
+-rw-r--r--   0        0        0     8027 2023-07-01 17:42:01.895242 dxsp-3.0.0/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    14882 2023-07-01 17:42:01.895242 dxsp-3.0.0/dxsp/main.py
+-rw-r--r--   0        0        0      103 2023-07-01 17:42:01.895242 dxsp-3.0.0/dxsp/protocols/__init__.py
+-rw-r--r--   0        0        0     3598 2023-07-01 17:42:01.895242 dxsp-3.0.0/dxsp/protocols/oneinch.py
+-rw-r--r--   0        0        0     2189 2023-07-01 17:42:01.895242 dxsp-3.0.0/dxsp/protocols/uniswap.py
+-rw-r--r--   0        0        0      941 2023-07-01 17:42:01.895242 dxsp-3.0.0/dxsp/protocols/zerox.py
+-rw-r--r--   0        0        0     2118 2023-07-01 17:42:02.795255 dxsp-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3141 1970-01-01 00:00:00.000000 dxsp-3.0.0/PKG-INFO
```

### Comparing `dxsp-2.6.9/LICENSE` & `dxsp-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.6.9/README.md` & `dxsp-3.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # DXSP (DeX SwaP)
 
 |<img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/231213427-63ea2752-13d5-4993-aee2-90671b57fc6e.png">  | A python defi swap helper package. Swap made easy |
 | ------------- | ------------- |
-|[![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/) ![Version](https://img.shields.io/pypi/v/dxsp)<br>  ![Pypi](https://img.shields.io/pypi/dm/dxsp) [![Docker Pulls](https://badgen.net/docker/pulls/mraniki/dxsp)](https://hub.docker.com/r/mraniki/dxsp)<br> [![✨Flow](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/dxsp/branch/main/graph/badge.svg?token=39ED0ZA6IH)](https://codecov.io/gh/mraniki/dxsp) <br>![](https://healthchecks.io/badge/227be4cc-702a-4ac8-b37b-d3d5a3/UcTrNrys-2/dxsp.svg)<br>[![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko)|Key blockchains (ETH, BSC, ARB, MATIC, OPT...)<br>Key swap protocol (UniV2 router)
+|[![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/) ![Version](https://img.shields.io/pypi/v/dxsp)<br>  ![Pypi](https://img.shields.io/pypi/dm/dxsp) <br>[![👷Flow](https://github.com/mraniki/dxsp/actions/workflows/%F0%9F%91%B7Flow.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml)<br>[![codebeat badge](https://codebeat.co/badges/b1376839-73bc-4b41-bfc1-2fb099f1fc2a)](https://codebeat.co/projects/github-com-mraniki-dxsp-main)<br>[![codecov](https://codecov.io/gh/mraniki/dxsp/branch/main/graph/badge.svg?token=39ED0ZA6IH)](https://codecov.io/gh/mraniki/dxsp) <br>[![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko)|Key blockchains (ETH, BSC, ARB, MATIC, OPT...)<br>Key swap protocol (UniV2 0x)
 
 Key features:
 
-- Any blockchains mainnet or testnet supported by web3py, 1inch or uniswap type router.
+- Any blockchains mainnet or testnet supported by web3py, uniswap type router (uniswap, pancakeswap) or 0x.
 
 
 Other features:
 
-- Translate token symbol to contract address via user defined tokenlist format or coingecko api
-- Connect to web3 automatically (optionn to provide a web3 object)
+- Translate token symbol to contract address via user defined tokenlist format or coingecko API
+- Connect to web3 automatically or use your own w3
 - Approve contract and sign transaction
 - Quote a given token
-- Use Base trading symbol like stablecoin
+- Use Base trading symbol like stablecoin for risk management approach
 - Settings to use the module for your own setup
 
 ## Install
 
 `pip install dxsp`
 
 ## How to use it
```

### Comparing `dxsp-2.6.9/dxsp/main.py` & `dxsp-3.0.0/dxsp/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,300 +5,258 @@
 import logging
 from typing import Optional
 
 import requests
 from pycoingecko import CoinGeckoAPI
 from web3 import Web3
 from web3.gas_strategies.time_based import medium_gas_price_strategy
-
 from dxsp import __version__
 from dxsp.config import settings
 
+
 class DexSwap:
     """swap  class"""
     def __init__(self, w3: Optional[Web3] = None):
         self.logger = logging.getLogger(name="DexSwap")
-
         self.w3 = w3 or Web3(Web3.HTTPProvider(settings.dex_rpc))
         self.w3.eth.set_gas_price_strategy(medium_gas_price_strategy)
         try:
             if self.w3.net.listening:
                 self.logger.info("connected %s",self.w3)
         except Exception as error:
             raise error
 
-        self.protocol_type = settings.dex_protocol_type
         self.chain_id = settings.dex_chain_id
         self.wallet_address = self.w3.to_checksum_address(
             settings.dex_wallet_address)
         self.account = f"{str(self.chain_id)} - {str(self.wallet_address[-8:])}"
         self.private_key = settings.dex_private_key
-
+        
         self.cg = CoinGeckoAPI()
+                    
+        self.protocol_type = settings.dex_protocol_type
+        self.dex_swap = None
+        self.router = None
+        self.quoter = None
+
+
+    async def get_protocol(self):
+        """ protocol init """
+        from dxsp.protocols import DexSwapUniswap, DexSwapZeroX, DexSwapOneInch
+        if self.protocol_type == "0x":
+            self.dex_swap = DexSwapZeroX()
+        elif self.protocol_type == "1inch":
+            self.dex_swap = DexSwapOneInch()
+        else:
+            self.dex_swap = DexSwapUniswap()
 
-    async def execute_order(self, order_params):
-        """Execute swap function."""
-        action = order_params.get('action')
-        instrument = order_params.get('instrument')
-        quantity = order_params.get('quantity', 1)
 
+    async def execute_order(self, order_params):
+        """ Execute swap function. """
         try:
+            action = order_params.get('action')
+            instrument = order_params.get('instrument')
+            quantity = order_params.get('quantity', 1)
             sell_token, buy_token = (
-                (settings.trading_asset, instrument)
+                (settings.trading_asset_address, instrument)
                 if action == 'BUY'
-                else (instrument, settings.trading_asset))
-
-            sell_contract = await self.get_token_contract(sell_token)
-            sell_decimals = sell_contract.functions.decimals().call() or 18
-
-            sell_balance = await self.get_token_balance(sell_token)
-            risk_percentage = settings.trading_risk_amount
-            sell_amount = (sell_balance / (risk_percentage ** sell_decimals)) * (float(quantity) / 100)
-
-            order = await self.get_swap(sell_token, buy_token, sell_amount)
+                else (instrument, settings.trading_asset_address))
+            order = await self.get_swap(sell_token, buy_token, quantity)
             if order:
-                return order['confirmation']
-        except Exception:
-            raise ValueError("Order execution failed")
-
-    async def get_quote(self, sell_token):
-        """
-        Asynchronously gets a quote for a specified sell token using the given `sell_token` parameter,
-        """
-        buy_address = await self.search_contract(settings.trading_asset)
-        sell_address = await self.search_contract(sell_token)
-        if sell_address is None:
-            return
-
-        try:
-            if self.protocol_type in {"uniswap_v2", "uniswap_v3"}:
-                return await self.get_quote_uniswap(
-                    buy_address,
-                    sell_address)
-
-            if self.protocol_type == "0x":
-                return await self.get_0x_quote(
-                    buy_address,
-                    sell_address)
-
-        except Exception as error:
-            raise error
-
-    async def get_swap(self, sell_token: str, buy_token: str, amount: int) -> None:
-        """Main swap function"""
-        try:
-            sell_token_address = await self.search_contract(sell_token)
-            sell_token_balance = await self.get_token_balance(sell_token)
-            if not sell_token_address or sell_token_balance in (0, None):
-                raise ValueError("No Money")
-
-            buy_token_address = await self.search_contract(buy_token)
-            if not buy_token_address:
-                raise ValueError("contract not found")
-
+                    trade_confirmation = (
+                        f"⬇️ {instrument}" if (action == "SELL") else f"⬆️ {instrument}\n")
+                    trade_confirmation += order
+                    return trade_confirmation
+
+        except Exception as error:
+            return f"⚠️ order execution: {error}"
+
+    async def get_swap(self, sell_token: str, buy_token: str, quantity: int) -> None:
+        """ Main swap function """
+        try:
+            await self.get_protocol()
+            sell_token_address = sell_token
+            if not sell_token.startswith("0x"):
+                sell_token_address = await self.search_contract_address(sell_token)
+            sell_token_balance = await self.get_token_balance(sell_token_address)
+            buy_token_address = buy_token
+            if not buy_token_address.startswith("0x"):   
+                buy_token_address = await self.search_contract_address(buy_token)
+            sell_amount = await self.calculate_sell_amount(sell_token_address, quantity)
             sell_token_amount_wei = self.w3.to_wei(
-                amount * 10 ** (await self.get_token_decimals(sell_token)), "ether")
+                sell_amount * 10 ** (await self.get_token_decimals(sell_token_address)), "ether")
 
-            if await self.get_approve(sell_token) is None:
-                raise ValueError("approval failed")
+            await self.get_approve(sell_token_address)
 
-            swap_order = await self.get_swap_order(
-                sell_token_address, buy_token_address, sell_token_amount_wei)
-            if not swap_order:
-                raise ValueError("swawp order not executed")
+            order_amount = int(sell_token_amount_wei * (settings.dex_trading_slippage / 100))
+            order = await self.dex_swap.get_swap(sell_token_address, buy_token_address, order_amount)
 
-            if self.protocol_type == "0x":
-                await self.get_sign(swap_order)
+            if not order:
+                raise ValueError("swap order not executed")
 
-            signed_order = await self.get_sign(swap_order)
+            signed_order = await self.get_sign(order)
             order_hash = str(self.w3.to_hex(signed_order))
+            receipt = self.w3.wait_for_transaction_receipt(order_hash)
 
-            if self.w3.wait_for_transaction_receipt(
-                order_hash, timeout=120, poll_latency=0.1)["status"] != 1:
-                return
+            if receipt["status"] != 1:
+                raise ValueError("receipt failed")
 
-            await self.get_confirmation(order_hash)
+            return await self.get_confirmation(receipt['transactionHash'])
 
-        except Exception as error:
+        except ValueError as error:
             raise error
 
-### ------🛠️ W3 UTILS ---------
 
-
-    async def get(self, url, params=None, headers=None):
-        try:
-            self.logger.debug(f"Requesting URL: {url}")
-            response = requests.get(url, params=params, headers=headers, timeout=10)
-            if response.status_code == 200:
-                return response.json()
-
-        except Exception as error:
-            raise error
-
-
-    async def router(self):
+    async def get_quote(self, sell_token):
+        """ gets a quote for a token """
         try:
-            router_abi = await self.get_abi(settings.dex_router_contract_addr)
-            if router_abi is None:
-                router_abi = await self.get(settings.dex_router_abi_url)
-            return self.w3.eth.contract(
-                address=self.w3.to_checksum_address(
-                    settings.dex_router_contract_addr
-                ),
-                abi=router_abi,
-            )
+            await self.get_protocol()
+            buy_address = settings.trading_asset_address
+            sell_address = await self.search_contract_address(sell_token)
+            quote = await self.dex_swap.get_quote(buy_address, sell_address)
+            return f"🦄 {quote} {settings.trading_asset}"
         except Exception as error:
             raise error
 
-    async def get_name(self):
-        try:
-            return settings.dex_router_contract_addr[-8:]
-        except Exception as error:
-            raise error
 
-    async def quoter(self):
+    async def get_approve(self, token_address):
+        """ approve a token """
         try:
-            quoter_abi = await self.get_abi(settings.dex_quoter_contract_addr)
-            if quoter_abi is None:
-                quoter_abi = await self.get(settings.dex_quoter_abi_url)
-            contract = self.w3.eth.contract(
-                address=self.w3.to_checksum_address(
-                    settings.dex_quoter_contract_addr),
-                abi=quoter_abi)
-            return contract
+            contract = await self.get_token_contract(token_address)
+            if contract is None:
+                return
+            approved_amount = self.w3.to_wei(2 ** 64 - 1, 'ether')
+            owner_address = self.w3.to_checksum_address(self.wallet_address)
+            dex_router_address = self.w3.to_checksum_address(settings.dex_router_contract_addr)
+            allowance = contract.functions.allowance(owner_address, dex_router_address).call()
+            if allowance == 0:
+                approval_tx = contract.functions.approve(dex_router_address, approved_amount)
+                approval_tx_hash = await self.get_sign(approval_tx.transact())
+                return self.w3.eth.wait_for_transaction_receipt(approval_tx_hash)
         except Exception as error:
-            raise error
+            raise ValueError(f"Approval failed {error}") 
 
-    async def get_approve(self, symbol):
-        try:
-            if self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
-                await self.get_approve_uniswap(symbol)
-        except Exception as error:
-            self.logger.debug("error %s", error)
-            return None
 
     async def get_sign(self, transaction):
+        """ sign a transaction """
         try:
             if self.protocol_type in ['uniswap_v2', 'uniswap_v3']:
                 transaction_params = {
                     'from': self.wallet_address,
                     'gas': await self.get_gas(transaction),
                     'gasPrice': await self.get_gas_price(),
                     'nonce': self.w3.eth.get_transaction_count(
                         self.wallet_address),
                 }
                 transaction = transaction.build_transaction(transaction_params)
             signed = self.w3.eth.account.sign_transaction(
                 transaction, self.private_key)
-            return self.w3.eth.send_raw_transaction(signed.rawTransaction)
+            return self.w3.eth.send_raw_transaction(signed)
         except Exception as error:
             raise error
 
-    async def get_abi(self, address):
-        if not settings.dex_block_explorer_api:
-            self.logger.warning("No block_explorer_api.")
-            return None
+### ------🛠️ W3 UTILS ---------
+    async def get(self, url, params=None, headers=None):
+        """ gets a url payload """
+        try:
+            self.logger.debug(f"Requesting URL: {url}")
+            response = requests.get(url, params=params, headers=headers, timeout=10)
+            if response.status_code == 200:
+                return response.json()
 
-        params = {
-            "module": "contract",
-            "action": "getabi",
-            "address": address,
-            "apikey": settings.dex_block_explorer_api
-        }
+        except Exception as error:
+            raise error
 
+    async def router_contract(self):
+        """ create a router contract """
         try:
-            resp = await self.get(
-                url=settings.dex_block_explorer_url, params=params)
-            if resp['status'] == "1":
-                self.logger.debug("ABI found %s", resp)
-                return resp["result"]
-            else:
-                self.logger.warning("No ABI identified")
-                return None
+            router_abi = await self.get(settings.dex_router_abi_url)
+            self.router = self.w3.eth.contract(
+                address=self.w3.to_checksum_address(
+                    settings.dex_router_contract_addr
+                ),
+                abi=router_abi,
+            )
         except Exception as error:
-            self.logger.error("get_abi %s", error)
-            return None
+            raise error
 
-    async def get_swap_order(self, sell_token_address: str, buy_token_address: str, sell_token_amount_wei: int) -> Optional[str]:
-        """Get swap order"""
-        order_amount = int(sell_token_amount_wei * (settings.dex_trading_slippage / 100))
-
-        if self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
-            return await self.get_swap_uniswap(sell_token_address, buy_token_address, order_amount)
-        elif self.protocol_type == "0x":
-            order = await self.get_0x_quote(sell_token_address, buy_token_address, order_amount)
-            return order if not order else await self.get_sign(order)
+    async def quoter_contract(self):
+        """ create a quoter contract """
+        try:
+            quoter_abi = await self.get(settings.dex_quoter_abi_url)
+            self.quoter = self.w3.eth.contract(
+                address=self.w3.to_checksum_address(
+                    settings.dex_quoter_contract_addr),
+                abi=quoter_abi)
+        except Exception as error:
+            raise error
 
-        return None
+    async def calculate_sell_amount(self, sell_token_address, quantity):
+        """Returns amount based on risk percentage."""
+        sell_balance = await self.get_token_balance(sell_token_address)
+        sell_contract = await self.get_token_contract(sell_token_address)
+        sell_decimals = sell_contract.functions.decimals().call() if sell_contract is not None else 18
+        risk_percentage = settings.trading_risk_amount
+        return (sell_balance / (risk_percentage ** sell_decimals)) * (float(quantity) / 100)
 
-    async def get_confirmation(self, order_hash):
+    async def get_confirmation(self, transactionHash):
         """Returns trade confirmation."""
         try:
-            receipt = self.w3.eth.get_transaction(order_hash)
-            block = self.w3.eth.get_block(receipt["blockNumber"])
+            transaction = self.w3.eth.get_transaction(transactionHash)
+            block = self.w3.eth.get_block(transaction["blockNumber"])
             return {
                 "timestamp": block["timestamp"],
-                "id": receipt["blockHash"],
-                "instrument": receipt["to"],
-                "contract": receipt["to"],
-                "amount": receipt["value"],
-                "price": receipt["value"],  # To be determined.
-                "fee": receipt["gas"],
+                "id": transactionHash,
+                "instrument": transaction["to"],
+                "contract": transaction["to"], # TBD To be determined.
+                "amount": transaction["value"],
+                "price": transaction["value"],  # TBD To be determined.
+                "fee": transaction["gas"],
                 "confirmation": (
-                    f"➕ Size: {round(receipt['value'], 4)}\n"
-                    f"⚫️ Entry: {round(receipt['value'], 4)}\n"
-                    f"ℹ️ {receipt['blockHash']}\n"
+                    f"➕ Size: {round(transaction['value'], 4)}\n"
+                    f"⚫️ Entry: {round(transaction['value'], 4)}\n"
+                    f"ℹ️ {transactionHash}\n"
+                    f"⛽ {transaction['gas']}\n"
                     f"🗓️ {block['timestamp']}"
                 ),
             }
         except Exception as error:
             raise error
 
-
     async def get_gas(self, transaction):
         """get gas estimate"""
         gas_limit = self.w3.eth.estimate_gas(transaction) * 1.25
         return int(self.w3.to_wei(gas_limit, 'wei'))
 
-
     async def get_gas_price(self):
         """search get gas price"""
         return round(self.w3.from_wei(self.w3.eth.generate_gas_price(), 'gwei'), 2)
 
 ### ------✍️ CONTRACT ---------
-    async def search_contract(self, token):
+    async def search_contract_address(self, token):
         """search a contract function"""
-        self.logger.debug("search_contract")
-
-        try:
-            contract_lists = [
-                settings.token_personal_list,
-                settings.token_testnet_list,
-                settings.token_mainnet_list,
-            ]
-
-            for contract_list in contract_lists:
-                token_contract = await self.get_contract_address(
-                    contract_list,
-                    token
-                )
-                if token_contract is not None:
-                    self.logger.info("%s token: contract found %s",
-                                     token, token_contract)
-                    return self.w3.to_checksum_address(token_contract)
 
-            token_contract = await self.search_cg_contract(token)
+        contract_lists = [
+            settings.token_personal_list,
+            settings.token_testnet_list,
+            settings.token_mainnet_list,
+        ]
+        for contract_list in contract_lists:
+            token_contract = await self.get_token_address(
+                contract_list,
+                token
+            )
             if token_contract is not None:
-                self.logger.info("%s token: contract found %s",
-                                 token, token_contract)
                 return self.w3.to_checksum_address(token_contract)
 
-            return None
-        except Exception:
-            return None
+        token_contract = await self.search_cg_contract(token)
+        if token_contract is None:
+            raise ValueError("Invalid Token")
+        return self.w3.to_checksum_address(token_contract)
+
 
     async def search_cg_platform(self):
         """search coingecko platform"""
         asset_platforms = self.cg.get_asset_platforms()
         output_dict = next(
             x for x in asset_platforms
             if x["chain_identifier"] == int(self.chain_id)
@@ -330,158 +288,92 @@
             coin_info = await self.search_cg(token)
             return (coin_info['platforms'][f'{await self.search_cg_platform()}']
                     if coin_info is not None else None)
         except Exception as e:
             self.logger.error(" search_cg_contract: %s", e)
             return
 
-    async def get_contract_address(self, token_list_url, symbol):
+    async def get_token_address(self, token_list_url, symbol):
         """Given a token symbol and json tokenlist, get token address"""
-        try:
-            token_list = await self.get(token_list_url)
-            token_search = token_list['tokens']
-            for keyval in token_search:
-                if (keyval['symbol'] == symbol and
-                   keyval['chainId'] == self.chain_id):
-                    return keyval['address']
-        except Exception as e:
-            self.logger.debug("get_contract_address %s", e)
-            return
+        token_list = await self.get(token_list_url)
+        token_search = token_list['tokens']
+        for keyval in token_search:
+            if (keyval['symbol'] == symbol and
+                keyval['chainId'] == self.chain_id):
+                return keyval['address']
+
+    async def get_token_contract(self, token_address):
+        """Given a token address, returns a contract object. """
+        token_abi = await self.get_explorer_abi(token_address)
+        if token_abi is None:
+            token_abi = await self.get(settings.dex_erc20_abi_url)
+        return self.w3.eth.contract(
+            address=token_address,
+            abi=token_abi)
 
-    async def get_token_contract(self, token):
-        """Given a token symbol, returns a contract object. """
+
+    async def get_token_decimals(self, token_address: str) -> Optional[int]:
+        """Get token decimals"""
+        contract = await self.get_token_contract(token_address)
+        return 18 if not contract else contract.functions.decimals().call() or 18
+
+    async def get_token_balance(self, token_address: str) -> Optional[int]:
+        """Get token balance"""
+        contract = await self.get_token_contract(token_address)
+        if contract is None or contract.functions is None:
+            raise ValueError("No Balance")
+        balance = contract.functions.balanceOf(self.wallet_address).call()
+        if balance is None:
+            raise ValueError("No Balance")
+        return balance
+
+
+    async def get_explorer_abi(self, address):
+        if not settings.dex_block_explorer_api:
+            return None
+
+        params = {
+            "module": "contract",
+            "action": "getabi",
+            "address": address,
+            "apikey": settings.dex_block_explorer_api
+        }
         try:
-            token_address = await self.search_contract(token)
-            token_abi = await self.get_abi(token_address)
-            if token_abi is None:
-                token_abi = await self.get(settings.dex_erc20_abi_url)
-            return self.w3.eth.contract(
-                address=token_address,
-                abi=token_abi)
-        except Exception as e:
-            raise e
+            resp = await self.get(
+                url=settings.dex_block_explorer_url, params=params)
+            if resp['status'] == "1":
+                self.logger.debug("ABI found %s", resp)
+                return resp["result"]
+            else:
+                return None
+        except Exception as error:
+            return None
+
 
 # 🔒 USER RELATED
-    async def get_token_balance(self, token_symbol: str) -> Optional[int]:
-        """Get token balance"""
-        # contract_address = await self.search_contract(token_symbol)
-        # if not contract_address:
-        #     return None
-        contract = await self.get_token_contract(token_symbol)
-        if not contract:
-            return 0
-        return contract.functions.balanceOf(self.wallet_address).call()
 
-    async def get_token_decimals(self, token_symbol: str) -> Optional[int]:
-        """Get token decimals"""
-        contract = await self.get_token_contract(token_symbol)
-        return 18 if not contract else contract.functions.decimals().call() or 18
+    async def get_name(self):
+        return settings.dex_router_contract_addr[-8:]
+
 
     async def get_account_balance(self):
         try:
             account_balance = self.w3.eth.get_balance(
                 self.w3.to_checksum_address(self.wallet_address))
             account_balance = self.w3.from_wei(account_balance, 'ether')
             trading_asset_balance = await self.get_trading_asset_balance()
             if trading_asset_balance:
                 account_balance += f"💵{trading_asset_balance}"
             return round(account_balance, 5)
-
         except Exception:
             return 0
 
     async def get_trading_asset_balance(self):
-        try:
-            trading_asset_balance = await self.get_token_balance(
-                settings.trading_asset)
-            return trading_asset_balance if trading_asset_balance else 0
-        except Exception:
-            return 0
+        trading_asset_balance = await self.get_token_balance(
+            settings.trading_asset_address)
+        return trading_asset_balance if trading_asset_balance else 0
 
     async def get_account_position(self):
         return 0
 
     async def get_account_margin(self):
         return 0
-
-# PROTOCOL SPECIFIC
-# uniswap  🦄
-    async def get_quote_uniswap(
-        self,
-        asset_in_address,
-        asset_out_address,
-        amount=1
-    ):
-        self.logger.debug("get_quote_uniswap")
-        try:
-            if self.protocol_type == "uniswap_v2":
-                router_instance = await self.router()
-                quote = router_instance.functions.getAmountsOut(
-                    amount,
-                    [asset_in_address, asset_out_address]).call()
-                self.logger.error("quote %s", quote)
-                if isinstance(quote, list):
-                    quote = str(quote[0])
-            elif self.protocol_type == "uniswap_v3":
-                quoter = await self.quoter()
-                sqrtPriceLimitX96 = 0
-                fee = 3000
-                quote = quoter.functions.quoteExactInputSingle(
-                    asset_in_address,
-                    asset_out_address,
-                    fee, amount, sqrtPriceLimitX96).call()
-            return f"🦄 {quote} {settings.trading_asset}"
-        except Exception as e:
-            raise e
-
-    async def get_approve_uniswap(self, symbol):
-        try:
-            contract = await self.get_token_contract(symbol)
-            approved_amount = self.w3.to_wei(2 ** 64 - 1, 'ether')
-            owner_address = self.w3.to_checksum_address(self.wallet_address)
-            dex_router_address = self.w3.to_checksum_address(settings.dex_router_contract_addr)
-            allowance = contract.functions.allowance(owner_address, dex_router_address).call()
-            self.logger.debug("allowance %s", allowance)
-            if allowance == 0:
-                approval_tx = contract.functions.approve(dex_router_address, approved_amount)
-                approval_tx_hash = await self.get_sign(approval_tx)
-                return self.w3.eth.wait_for_transaction_receipt(
-                    approval_tx_hash, timeout=120, poll_latency=0.1
-                )
-        except Exception as e:
-            raise e
-
-
-    async def get_swap_uniswap(self, asset_out_address, asset_in_address, amount):
-        try:
-            path = [self.w3.to_checksum_address(asset_out_address),
-                    self.w3.to_checksum_address(asset_in_address)]
-            deadline = self.w3.eth.get_block("latest")["timestamp"] + 3600
-            router_instance = await self.router()
-            min_amount = self.get_quote_uniswap(
-                asset_in_address, asset_out_address, amount)[0]
-
-            if self.protocol_type == "uniswap_v2":
-                return router_instance.functions.swapExactTokensForTokens(
-                    int(amount),
-                    int(min_amount),
-                    tuple(path),
-                    self.wallet_address,
-                    deadline,
-                )
-            elif self.protocol_type == "uniswap_v3":
-                return None
-        except Exception as e:
-            raise e
-
-# 0️⃣x
-    async def get_0x_quote(self, buy_address, sell_address, amount=1):
-        try:
-            out_amount = self.w3.to_wei(amount, 'ether')
-            url = f"{settings.dex_0x_url}/swap/v1/quote?buyToken={str(buy_address)}&sellToken={str(sell_address)}&buyAmount={str(out_amount)}"
-            headers = {"0x-api-key": settings.dex_0x_api_key}
-            response = await self.get(url, params=None, headers=headers)
-            print(response)
-            if response:
-                return round(float(response['guaranteedPrice']), 3)
-        except Exception as e:
-            raise e
```

### Comparing `dxsp-2.6.9/pyproject.toml` & `dxsp-3.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,69 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.6.9"
+version = "3.0.0"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
 
 [tool.poetry.urls]
 "Changelog" =  "https://github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst"
 "Support" =  "https://github.com/mraniki/dxsp/discussions"
 "Issues" =  "https://github.com/mraniki/dxsp/issues"
 
 [tool.poetry.dependencies]
-python = "^3.10.0"
+python = "^3.10"
 dynaconf = "^3.1.12"
 web3 = "^6.4.0"
 pycoingecko = "^3.1.0"
+#eip712 = "^0.2.1"
+#eth-ape'[recommended-plugins]' = "^0.6.11"
 
 [tool.poetry.dev-dependencies]
 python-semantic-release = "^7.34.3"
-pytest = "^7.0.0"
-pytest-cov = "*"
-pytest-asyncio = "*"
-pytest-mock = "*"
+pytest = "^7.0"
+pytest-cov = "^4.1"
+pytest-asyncio = "^0.21.0"
+pytest-mock = "^3.11.1"
+eth_tester = "^0.9.0b2"
 
 [tool.pytest.ini_options]
 pythonpath = "."
 testpaths = "tests"
 python_classes = "Test*"
 log_format = "%(asctime)s - %(levelname)s - %(name)s - %(message)s"
 log_level = "DEBUG"
 
 [tool.coverage.run]
 omit = [
     "tests/*",
-    "examples/*"
+    "examples/*",
+    "docs/*",
+    "*/config.py"
 ]
 
+[tool.poetry.group.docs.dependencies]
+sphinx = "^7.0.1"
+sphinx-autoapi = "^2.1.0"
+furo = "^2023.5.20"
+
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
+
 [tool.semantic_release]
 version_variable = ["pyproject.toml:version","dxsp/__init__.py:__version__"]
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "pip install poetry && poetry build"
 commit_parser = "semantic_release.history.emoji_parser"
 use_textual_changelog_sections = true
-major_emoji = "💥"
-minor_emoji = "🥚,🚀,💄,✨"
-patch_emoji = "🎨,🐛,🚑,⚡,🔥,🚨,♻️,🔧,⬆️,🩹,👷,📝,🔒,👽,💬,🥅,✅,🐳,🙈,⚗️,🧐,🔇,🔊"
+major_emoji = "BREAKING,💥,:boom:"
+minor_emoji = "feat,🥚,:egg:,🚀,:rocket:,💄,:lipstick:,✨,:sparkles:"
+patch_emoji = "fix,bump,Update,🎨,:art:,🐛,:bug:,🚑,:ambulance:,⚡,:zap:,🔥,:fire:,🚨,:rotating_light:,♻️,:recycle:,🔧,:wrench:,⬆️,:arrow_up:,🩹,:adhesive_bandage:,👷,:construction_worker:,📝,:memo:,🔒,:lock:,👽,:alien:,💬,:speech_balloon:,🥅,:goal_net:,✅,:white_check_mark:,🐳,:whale:,🙈,:see_no_evil:,⚗️,:alembic:,🧐,:monocle_face:,🔇,:mute:,🔊:volume:"
```

### Comparing `dxsp-2.6.9/PKG-INFO` & `dxsp-3.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.6.9
+Version: 3.0.0
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
-Requires-Python: >=3.10.0,<4.0.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
 Requires-Dist: pycoingecko (>=3.1.0,<4.0.0)
 Requires-Dist: web3 (>=6.4.0,<7.0.0)
@@ -18,28 +18,28 @@
 Project-URL: Support, https://github.com/mraniki/dxsp/discussions
 Description-Content-Type: text/markdown
 
 # DXSP (DeX SwaP)
 
 |<img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/231213427-63ea2752-13d5-4993-aee2-90671b57fc6e.png">  | A python defi swap helper package. Swap made easy |
 | ------------- | ------------- |
-|[![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/) ![Version](https://img.shields.io/pypi/v/dxsp)<br>  ![Pypi](https://img.shields.io/pypi/dm/dxsp) [![Docker Pulls](https://badgen.net/docker/pulls/mraniki/dxsp)](https://hub.docker.com/r/mraniki/dxsp)<br> [![✨Flow](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/dxsp/branch/main/graph/badge.svg?token=39ED0ZA6IH)](https://codecov.io/gh/mraniki/dxsp) <br>![](https://healthchecks.io/badge/227be4cc-702a-4ac8-b37b-d3d5a3/UcTrNrys-2/dxsp.svg)<br>[![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko)|Key blockchains (ETH, BSC, ARB, MATIC, OPT...)<br>Key swap protocol (UniV2 router)
+|[![wiki](https://img.shields.io/badge/🪙🗿-wiki-0080ff)](https://talkytrader.gitbook.io/talky/) [![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/) ![Version](https://img.shields.io/pypi/v/dxsp)<br>  ![Pypi](https://img.shields.io/pypi/dm/dxsp) <br>[![👷Flow](https://github.com/mraniki/dxsp/actions/workflows/%F0%9F%91%B7Flow.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml)<br>[![codebeat badge](https://codebeat.co/badges/b1376839-73bc-4b41-bfc1-2fb099f1fc2a)](https://codebeat.co/projects/github-com-mraniki-dxsp-main)<br>[![codecov](https://codecov.io/gh/mraniki/dxsp/branch/main/graph/badge.svg?token=39ED0ZA6IH)](https://codecov.io/gh/mraniki/dxsp) <br>[![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko)|Key blockchains (ETH, BSC, ARB, MATIC, OPT...)<br>Key swap protocol (UniV2 0x)
 
 Key features:
 
-- Any blockchains mainnet or testnet supported by web3py, 1inch or uniswap type router.
+- Any blockchains mainnet or testnet supported by web3py, uniswap type router (uniswap, pancakeswap) or 0x.
 
 
 Other features:
 
-- Translate token symbol to contract address via user defined tokenlist format or coingecko api
-- Connect to web3 automatically (optionn to provide a web3 object)
+- Translate token symbol to contract address via user defined tokenlist format or coingecko API
+- Connect to web3 automatically or use your own w3
 - Approve contract and sign transaction
 - Quote a given token
-- Use Base trading symbol like stablecoin
+- Use Base trading symbol like stablecoin for risk management approach
 - Settings to use the module for your own setup
 
 ## Install
 
 `pip install dxsp`
 
 ## How to use it
```

