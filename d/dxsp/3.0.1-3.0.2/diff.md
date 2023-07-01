# Comparing `tmp/dxsp-3.0.1.tar.gz` & `tmp/dxsp-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-3.0.1.tar", max compression
+gzip compressed data, was "dxsp-3.0.2.tar", max compression
```

## Comparing `dxsp-3.0.1.tar` & `dxsp-3.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-07-01 18:09:46.447126 dxsp-3.0.1/LICENSE
--rw-r--r--   0        0        0     2249 2023-07-01 18:09:46.447126 dxsp-3.0.1/README.md
--rw-r--r--   0        0        0      114 2023-07-01 18:09:47.347126 dxsp-3.0.1/dxsp/__init__.py
--rw-r--r--   0        0        0      418 2023-07-01 18:09:46.447126 dxsp-3.0.1/dxsp/config.py
--rw-r--r--   0        0        0     8027 2023-07-01 18:09:46.447126 dxsp-3.0.1/dxsp/default_settings.toml
--rw-r--r--   0        0        0    14882 2023-07-01 18:09:46.447126 dxsp-3.0.1/dxsp/main.py
--rw-r--r--   0        0        0      103 2023-07-01 18:09:46.447126 dxsp-3.0.1/dxsp/protocols/__init__.py
--rw-r--r--   0        0        0     3598 2023-07-01 18:09:46.447126 dxsp-3.0.1/dxsp/protocols/oneinch.py
--rw-r--r--   0        0        0     2189 2023-07-01 18:09:46.447126 dxsp-3.0.1/dxsp/protocols/uniswap.py
--rw-r--r--   0        0        0      941 2023-07-01 18:09:46.447126 dxsp-3.0.1/dxsp/protocols/zerox.py
--rw-r--r--   0        0        0     2118 2023-07-01 18:09:47.343126 dxsp-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     3051 1970-01-01 00:00:00.000000 dxsp-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-01 21:19:40.483796 dxsp-3.0.2/LICENSE
+-rw-r--r--   0        0        0     2249 2023-07-01 21:19:40.483796 dxsp-3.0.2/README.md
+-rw-r--r--   0        0        0      114 2023-07-01 21:19:41.363792 dxsp-3.0.2/dxsp/__init__.py
+-rw-r--r--   0        0        0      418 2023-07-01 21:19:40.483796 dxsp-3.0.2/dxsp/config.py
+-rw-r--r--   0        0        0     8028 2023-07-01 21:19:40.483796 dxsp-3.0.2/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    15086 2023-07-01 21:19:40.483796 dxsp-3.0.2/dxsp/main.py
+-rw-r--r--   0        0        0      103 2023-07-01 21:19:40.483796 dxsp-3.0.2/dxsp/protocols/__init__.py
+-rw-r--r--   0        0        0     3536 2023-07-01 21:19:40.483796 dxsp-3.0.2/dxsp/protocols/oneinch.py
+-rw-r--r--   0        0        0     2335 2023-07-01 21:19:40.483796 dxsp-3.0.2/dxsp/protocols/uniswap.py
+-rw-r--r--   0        0        0      941 2023-07-01 21:19:40.483796 dxsp-3.0.2/dxsp/protocols/zerox.py
+-rw-r--r--   0        0        0     2118 2023-07-01 21:19:41.363792 dxsp-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3051 1970-01-01 00:00:00.000000 dxsp-3.0.2/PKG-INFO
```

### Comparing `dxsp-3.0.1/LICENSE` & `dxsp-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-3.0.1/README.md` & `dxsp-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-3.0.1/dxsp/default_settings.toml` & `dxsp-3.0.2/dxsp/default_settings.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 [default]
 VALUE = "On default"
 dxsp_enabled = true
 loglevel = "INFO"
-headers = {User-Agent= 'Mozilla/5.0'}
-token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
-token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
-token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
-trading_asset = "USDT"
-trading_asset_address = "0xdAC17F958D2ee523a2206206994597C13D831ec7"
-trading_risk_amount = 10 # 10% of the position
-dex_trading_slippage = 2 # 2% slippage
 dex_wallet_address = "0x1234567890123456789012345678901234567890"
 dex_private_key = "0xdeadbeef45ab87712ad64ccb3b10217737f7faacbf2872e88fdd9a537d8fe266" 
-dex_chain_id = 1
 dex_protocol_type = "uniswap_v2" #0x
+dex_chain_id = 1
 dex_rpc = "https://rpc.ankr.com/eth"
-dex_block_explorer_url = "https://api.etherscan.io/api?"
-dex_block_explorer_api =  "798437294880920392"
+dex_0x_url = "https://api.0x.org/mainnet"
+dex_0x_api_key = "" 
 dex_router_contract_addr = "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D"
 dex_router_abi_url = "https://raw.githubusercontent.com/uniswap-python/uniswap-python/master/uniswap/assets/uniswap-v2/router02.abi"
 dex_erc20_abi_url = "https://raw.githubusercontent.com/Uniswap/interface/44c355c7f0f8ab5bdb3e0790560e84e59f5666f7/src/abis/erc20.json"
 dex_quoter_contract_addr = "0x61fFE014bA17989E743c5F6cB21bF9697530B21e"
 dex_quoter_abi_url = "https://raw.githubusercontent.com/uniswap-python/uniswap-python/master/uniswap/assets/uniswap-v3/quoter.abi"
-dex_0x_url = "https://api.0x.org/mainnet"
-dex_0x_api_key = "" 
-
-
-
+dex_block_explorer_url = "https://api.etherscan.io/api?"
+dex_block_explorer_api =  "798437294880920392"
+headers = {User-Agent= 'Mozilla/5.0'}
+token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
+token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
+token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
+trading_asset = "USDT"
+trading_asset_address = "0xdAC17F958D2ee523a2206206994597C13D831ec7"
+trading_risk_amount = 10 # 10% of the position
+dex_trading_slippage = 2 # 2% slippage
 
 
 
 
 
 
 
@@ -38,90 +35,92 @@
 ## SETTINGS ##
 ## FOR TEST ##
 ##############
 [test_uniswap_chain_1]
 VALUE = "On Testing"
 dxsp_enabled = true
 loglevel = "DEBUG"
-headers = {User-Agent= 'Mozilla/5.0'}
-token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
-token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
-token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
-trading_asset = "USDT"
-trading_asset_address = "0xdAC17F958D2ee523a2206206994597C13D831ec7"
-trading_risk_amount = 10 
-dex_trading_slippage = 2
 dex_wallet_address = "0x1a9C8182C09F50C8318d769245beA52c32BE35BC" 
 dex_private_key = "0xdeadbeet45ab87712ad64ccb3b10217737f7faacbf2872e88fdd9a537d8fe266" 
-dex_chain_id = 1
 dex_protocol_type = "uniswap_v2"
+dex_chain_id = 1
 dex_rpc = "https://rpc.ankr.com/eth"
 dex_router_contract_addr = "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D"
 dex_router_abi_url = "https://raw.githubusercontent.com/uniswap-python/uniswap-python/master/uniswap/assets/uniswap-v2/router02.abi"
 dex_erc20_abi_url = "https://raw.githubusercontent.com/Uniswap/interface/44c355c7f0f8ab5bdb3e0790560e84e59f5666f7/src/abis/erc20.json"
 dex_quoter_contract_addr = "0x61fFE014bA17989E743c5F6cB21bF9697530B21e"
 dex_quoter_abi_url = "https://raw.githubusercontent.com/uniswap-python/uniswap-python/master/uniswap/assets/uniswap-v3/quoter.abi"
+trading_asset = "USDT"
+trading_asset_address = "0xdAC17F958D2ee523a2206206994597C13D831ec7"
+trading_risk_amount = 10 
+dex_trading_slippage = 2
+headers = {User-Agent= 'Mozilla/5.0'}
+token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
+token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
+token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
 
 [test_zerox_chain_1]
 VALUE = "test_zerox"
 loglevel = "DEBUG"
 dxsp_enabled = true
-headers = {User-Agent= 'Mozilla/5.0'}
-token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
-token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
-token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
-trading_asset = "USDT"
-trading_asset_address = "0xdAC17F958D2ee523a2206206994597C13D831ec7"
-trading_risk_amount = 10
-dex_trading_slippage = 2
 dex_wallet_address = "0x1a9C8182C09F50C8318d769245beA52c32BE35BC" 
 dex_private_key = "0xdeadbeet45ab87712ad64ccb3b10217737f7faacbf2872e88fdd9a537d8fe266" 
+dex_protocol_type = "0x"
 dex_chain_id = 1
 dex_rpc = "https://rpc.ankr.com/eth"
-dex_protocol_type = "0x"
 dex_0x_url = "https://api.0x.org/"
 dex_router_contract_addr = "0xdef1c0ded9bec7f1a1670819833240f027b25eff"
 dex_router_abi_url = "https://raw.githubusercontent.com/0xProject/protocol/development/packages/contract-artifacts/artifacts/Exchange.json"
 dex_erc20_abi_url = "https://raw.githubusercontent.com/0xProject/protocol/development/packages/contract-artifacts/artifacts/ERC20Token.json"
+trading_asset = "USDT"
+trading_asset_address = "0xdAC17F958D2ee523a2206206994597C13D831ec7"
+trading_risk_amount = 10
+dex_trading_slippage = 2
+headers = {User-Agent= 'Mozilla/5.0'}
+token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
+token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
+token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
+
 
 [test_uniswap_chain5]
 VALUE = "On Testnet"
 loglevel = "DEBUG"
 dxsp_enabled = true
-dex_chain_id = 5
-dex_rpc = "https://rpc.ankr.com/eth_goerli"
-dex_block_explorer_url = "https://api-Goerli.etherscan.io/api?"
-headers = {User-Agent= 'Mozilla/5.0'}
-token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
-token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
-token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
-trading_asset = "USDT"
-trading_asset_address = "0xdAC17F958D2ee523a2206206994597C13D831ec7"
-trading_risk_amount = 10
-dex_trading_slippage = 2
 dex_wallet_address = "0x1a9C8182C09F50C8318d769245beA52c32BE35BC" 
 dex_private_key = "0xdeadbeet45ab87712ad64ccb3b10217737f7faacbf2872e88fdd9a537d8fe266" 
 dex_protocol_type = "uniswap_v2"
+dex_chain_id = 5
+dex_rpc = "https://rpc.ankr.com/eth_goerli"
+# dex_block_explorer_url = "https://api-Goerli.etherscan.io/api?"
 dex_router_contract_addr = "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D"
 dex_router_abi_url = "https://raw.githubusercontent.com/uniswap-python/uniswap-python/master/uniswap/assets/uniswap-v2/router02.abi"
 dex_erc20_abi_url = "https://raw.githubusercontent.com/Uniswap/interface/44c355c7f0f8ab5bdb3e0790560e84e59f5666f7/src/abis/erc20.json"
+trading_asset = "USDT"
+trading_asset_address = "0xdAC17F958D2ee523a2206206994597C13D831ec7"
+trading_risk_amount = 10
+dex_trading_slippage = 2
+headers = {User-Agent= 'Mozilla/5.0'}
+token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
+token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
+token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
 
 [test_pancake_chain_56]
 VALUE = "chain_56"
 dex_chain_id = 56
 dxsp_enabled = true
 dex_wallet_address = "0xf977814e90da44bfa03b6295a0616a897441acec"
+dex_protocol_type = "0x"
 dex_rpc = "https://rpc.ankr.com/bsc"
+dex_0x_url = "https://bsc.api.0x.org/"
+dex_router_contract_addr = "0x10ED43C718714eb63d5aA57B78B54704E256024E"
 dex_block_explorer_url = "https://api.bscscan.com/api?"
 dex_block_explorer_api =  ""
 trading_asset = "BUSD"
 trading_asset_address = "0xe9e7cea3dedca5984780bafc599bd69add087d56"
-dex_protocol_type = "0x"
-dex_router_contract_addr = "0x10ED43C718714eb63d5aA57B78B54704E256024E"
-dex_0x_url = "https://bsc.api.0x.org/"
+
 
 # [test_oneinch_chain_1]
 # VALUE = "1inchtesting"
 # loglevel = "DEBUG"
 # dxsp_enabled = true
 # headers = {User-Agent= 'Mozilla/5.0'}
 # token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
```

### Comparing `dxsp-3.0.1/dxsp/main.py` & `dxsp-3.0.2/dxsp/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,16 @@
             raise error
 
         self.chain_id = settings.dex_chain_id
         self.wallet_address = self.w3.to_checksum_address(
             settings.dex_wallet_address)
         self.account = f"{str(self.chain_id)} - {str(self.wallet_address[-8:])}"
         self.private_key = settings.dex_private_key
-        
+        self.trading_asset_address = self.w3.to_checksum_address(
+            settings.trading_asset_address)
         self.cg = CoinGeckoAPI()
                     
         self.protocol_type = settings.dex_protocol_type
         self.dex_swap = None
         self.router = None
         self.quoter = None
 
@@ -53,17 +54,17 @@
     async def execute_order(self, order_params):
         """ Execute swap function. """
         try:
             action = order_params.get('action')
             instrument = order_params.get('instrument')
             quantity = order_params.get('quantity', 1)
             sell_token, buy_token = (
-                (settings.trading_asset_address, instrument)
+                (self.trading_asset_address, instrument)
                 if action == 'BUY'
-                else (instrument, settings.trading_asset_address))
+                else (instrument, self.trading_asset_address))
             order = await self.get_swap(sell_token, buy_token, quantity)
             if order:
                     trade_confirmation = (
                         f"⬇️ {instrument}" if (action == "SELL") else f"⬆️ {instrument}\n")
                     trade_confirmation += order
                     return trade_confirmation
 
@@ -106,20 +107,20 @@
             raise error
 
 
     async def get_quote(self, sell_token):
         """ gets a quote for a token """
         try:
             await self.get_protocol()
-            buy_address = settings.trading_asset_address
+            buy_address = self.trading_asset_address
             sell_address = await self.search_contract_address(sell_token)
             quote = await self.dex_swap.get_quote(buy_address, sell_address)
             return f"🦄 {quote} {settings.trading_asset}"
         except Exception as error:
-            raise error
+            return f"⚠️: {error}"
 
 
     async def get_approve(self, token_address):
         """ approve a token """
         try:
             contract = await self.get_token_contract(token_address)
             if contract is None:
@@ -172,14 +173,16 @@
             router_abi = await self.get(settings.dex_router_abi_url)
             self.router = self.w3.eth.contract(
                 address=self.w3.to_checksum_address(
                     settings.dex_router_contract_addr
                 ),
                 abi=router_abi,
             )
+            if self.router.functions is None:
+                raise ValueError("Router/Chain setup incorrect")
         except Exception as error:
             raise error
 
     async def quoter_contract(self):
         """ create a quoter contract """
         try:
             quoter_abi = await self.get(settings.dex_quoter_abi_url)
@@ -237,25 +240,25 @@
 
         contract_lists = [
             settings.token_personal_list,
             settings.token_testnet_list,
             settings.token_mainnet_list,
         ]
         for contract_list in contract_lists:
-            token_contract = await self.get_token_address(
+            token_address = await self.get_token_address(
                 contract_list,
                 token
             )
-            if token_contract is not None:
-                return self.w3.to_checksum_address(token_contract)
+            if token_address is not None:
+                return self.w3.to_checksum_address(token_address)
 
-        token_contract = await self.search_cg_contract(token)
-        if token_contract is None:
+        token_address = await self.search_cg_contract(token)
+        if token_address is None:
             raise ValueError("Invalid Token")
-        return self.w3.to_checksum_address(token_contract)
+        return self.w3.to_checksum_address(token_address)
 
 
     async def search_cg_platform(self):
         """search coingecko platform"""
         asset_platforms = self.cg.get_asset_platforms()
         output_dict = next(
             x for x in asset_platforms
@@ -365,15 +368,15 @@
                 account_balance += f"💵{trading_asset_balance}"
             return round(account_balance, 5)
         except Exception:
             return 0
 
     async def get_trading_asset_balance(self):
         trading_asset_balance = await self.get_token_balance(
-            settings.trading_asset_address)
+            self.trading_asset_address)
         return trading_asset_balance if trading_asset_balance else 0
 
     async def get_account_position(self):
         return 0
 
     async def get_account_margin(self):
         return 0
```

### Comparing `dxsp-3.0.1/dxsp/protocols/oneinch.py` & `dxsp-3.0.2/dxsp/protocols/oneinch.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 from dxsp.main import DexSwap
 
 #https://github.com/mraniki/dxsp/issues/189 
 
 class DexSwapOneInch(DexSwap):
     async def get_quote(
         self,
-        asset_in_address,
-        asset_out_address,
+        buy_address,
+        sell_address,
         amount=1
     ):
         #try:
         pass
-        #     asset_out_amount = self.w3.to_wei(amount, 'ether')
+        #     min_amount = self.w3.to_wei(amount, 'ether')
         #     quote_url = (
         #         settings.dex_1inch_url
         #         + str(self.chain_id)
         #         + "/quote?fromTokenAddress="
-        #         + str(asset_in_address)
+        #         + str(buy_address)
         #         + "&toTokenAddress="
-        #         + str(asset_out_address)
+        #         + str(sell_address)
         #         + "&amount="
-        #         + str(asset_out_amount))
+        #         + str(min_amount))
         #     quote_response = await self._get(
         #         url=quote_url,
         #         params=None,
         #         headers=settings.headers)
         #     self.logger.debug("quote_response %s", quote_response)
         #     if quote_response:
         #         quote_amount = quote_response['toTokenAmount']
@@ -44,46 +44,46 @@
     #     # pass
     #     try:
     #         pass
             # approval_check_URL = (
             #     settings.dex_1inch_url
             #     + str(self.chain_id)
             #     + "/approve/allowance?tokenAddress="
-            #     + str(asset_out_address)
+            #     + str(sell_address)
             #     + "&walletAddress="
             #     + str(self.wallet_address))
             # approval_response = await self._get(
             #     url=approval_check_URL,
             #     params=None,
             #     headers=settings.headers)
             # approval_check = approval_response['allowance']
             # if (approval_check == 0):
             #     approval_URL = (
             #         settings.dex_1inch_url
             #         + str(self.chain_id)
             #         + "/approve/transaction?tokenAddress="
-            #         + str(asset_out_address))
+            #         + str(sell_address))
             #     approval_response = await self._get(approval_URL)
             #     return approval_response
     #     except Exception as error:
     #         raise ValueError(f"Approval failed {error}") 
 
 
 
-    # async def get_swap(self, asset_out_address, asset_in_address, amount):
+    # async def get_swap(self, sell_address, buy_address, amount):
 
     #     try:
     #         pass
             # swap_url = (
             #     settings.dex_1inch_url
             #     + str(self.chain_id)
             #     + "/swap?fromTokenAddress="
-            #     + asset_out_address
+            #     + sell_address
             #     + "&toTokenAddress="
-            #     + asset_in_address
+            #     + buy_address
             #     + "&amount="
             #     + amount
             #     + "&fromAddress="
             #     + self.wallet_address
             #     + "&slippage="
             #     + settings.dex_trading_slippage
             #     )
```

### Comparing `dxsp-3.0.1/dxsp/protocols/zerox.py` & `dxsp-3.0.2/dxsp/protocols/zerox.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.0.1/pyproject.toml` & `dxsp-3.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "3.0.1"
+version = "3.0.2"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
```

### Comparing `dxsp-3.0.1/PKG-INFO` & `dxsp-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 3.0.1
+Version: 3.0.2
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

