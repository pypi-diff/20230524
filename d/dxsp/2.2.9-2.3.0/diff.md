# Comparing `tmp/dxsp-2.2.9.tar.gz` & `tmp/dxsp-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.2.9.tar", max compression
+gzip compressed data, was "dxsp-2.3.0.tar", max compression
```

## Comparing `dxsp-2.2.9.tar` & `dxsp-2.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-05-15 12:54:04.853267 dxsp-2.2.9/LICENSE
--rw-r--r--   0        0        0     2605 2023-05-15 12:54:04.853267 dxsp-2.2.9/README.md
--rw-r--r--   0        0        0       86 2023-05-15 12:54:05.785266 dxsp-2.2.9/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-15 12:54:04.853267 dxsp-2.2.9/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-15 12:54:04.853267 dxsp-2.2.9/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      388 2023-05-15 12:54:04.853267 dxsp-2.2.9/dxsp/config.py
--rw-r--r--   0        0        0     3139 2023-05-15 12:54:04.853267 dxsp-2.2.9/dxsp/default_settings.toml
--rw-r--r--   0        0        0    28625 2023-05-15 12:54:04.853267 dxsp-2.2.9/dxsp/main.py
--rw-r--r--   0        0        0     1831 2023-05-15 12:54:05.785266 dxsp-2.2.9/pyproject.toml
--rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 dxsp-2.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-24 10:19:16.102585 dxsp-2.3.0/LICENSE
+-rw-r--r--   0        0        0     2439 2023-05-24 10:19:16.102585 dxsp-2.3.0/README.md
+-rw-r--r--   0        0        0       86 2023-05-24 10:19:17.146592 dxsp-2.3.0/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-24 10:19:16.102585 dxsp-2.3.0/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-24 10:19:16.102585 dxsp-2.3.0/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      388 2023-05-24 10:19:16.102585 dxsp-2.3.0/dxsp/config.py
+-rw-r--r--   0        0        0     3315 2023-05-24 10:19:16.102585 dxsp-2.3.0/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    25909 2023-05-24 10:19:16.102585 dxsp-2.3.0/dxsp/main.py
+-rw-r--r--   0        0        0     1960 2023-05-24 10:19:17.146592 dxsp-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 dxsp-2.3.0/PKG-INFO
```

### Comparing `dxsp-2.2.9/LICENSE` & `dxsp-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.2.9/README.md` & `dxsp-2.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,52 @@
 # DXSP (DeX SwaP)
 
 |<img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/231213427-63ea2752-13d5-4993-aee2-90671b57fc6e.png">  | A python defi swap helper package. Swap made easy |
 | ------------- | ------------- |
-|[![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/) ![Version](https://img.shields.io/pypi/v/dxsp)<br>  ![Pypi](https://img.shields.io/pypi/dm/dxsp) [![Docker Pulls](https://badgen.net/docker/pulls/mraniki/dxsp)](https://hub.docker.com/r/mraniki/dxsp)<br>[![✨Flow](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/dxsp/branch/main/graph/badge.svg?token=39ED0ZA6IH)](https://codecov.io/gh/mraniki/dxsp) <br>![](https://healthchecks.io/badge/227be4cc-702a-4ac8-b37b-d3d5a3/UcTrNrys-2/dxsp.svg)<br>[![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko)|24 blockchains (ETH, BSC, ARB, MATIC, OPT...)<br>2 swap protocol (1inch API, UniV2 router)
+|[![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/) ![Version](https://img.shields.io/pypi/v/dxsp)<br>  ![Pypi](https://img.shields.io/pypi/dm/dxsp) [![Docker Pulls](https://badgen.net/docker/pulls/mraniki/dxsp)](https://hub.docker.com/r/mraniki/dxsp)<br> [![✨Flow](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/dxsp/branch/main/graph/badge.svg?token=39ED0ZA6IH)](https://codecov.io/gh/mraniki/dxsp) <br>![](https://healthchecks.io/badge/227be4cc-702a-4ac8-b37b-d3d5a3/UcTrNrys-2/dxsp.svg)<br>[![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko)|Key blockchains (ETH, BSC, ARB, MATIC, OPT...)<br>Key swap protocol (UniV2 router)
 
 Key features:
 
 - Any blockchains mainnet or testnet supported by web3py, 1inch or uniswap type router.
-- 2 swap protocol type supported:
-  - Uniswap version 2 router protocol type
-  - 1inch API v5
+
 
 Other features:
 
 - Translate token symbol to contract address via user defined tokenlist format or coingecko api
 - Connect to web3 automatically (optionn to provide a web3 object)
 - Approve contract and sign transaction
 - Quote a given token
 - Use Base trading symbol like stablecoin
 - Settings to use the module for your own setup
 
-# Install
+## Install
 
 `pip install dxsp`
 
-# How to use it
+## How to use it
 
 ```
 from dxsp import DexSwap
 
  dex = DexSwap()
  #BUY 10 USDC to SWAP with BITCOIN
  demo_tx = await dex.get_swap('USDT','wBTC',10)
  print("demo_tx ", demo_tx)
 ```
 
-## Example
+### Example
 
 [example](https://github.com/mraniki/dxsp/blob/main/examples/example.py)
 
 
-## Real use case
+### Real use case
 
 [TalkyTrader, submit trading order to CEX & DEX with messaging platform (Telegram, Matrix and Discord)](https://github.com/mraniki/tt)
 
-# Documentation
-
-<https://github.com/mraniki/dxsp/wiki>
-
-## 🚧 Roadmap
+## Documentation
 
-[🚧 Roadmap](https://github.com/mraniki/dxsp/milestones)
+[wiki](https://github.com/mraniki/dxsp/wiki)
 
 ## Questions? Want to help?
 
 [![discord](https://badgen.net/badge/icon/discord/purple?icon=discord&label)](https://discord.gg/vegJQGrRRa)
 [![telegram](https://badgen.net/badge/icon/telegram?icon=telegram&label)](https://t.me/TTTalkyTraderChat/1)
```

### Comparing `dxsp-2.2.9/dxsp/assets/blockchains.py` & `dxsp-2.3.0/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.2.9/dxsp/default_settings.toml` & `dxsp-2.3.0/dxsp/default_settings.toml`

 * *Files 9% similar despite different names*

```diff
@@ -14,22 +14,23 @@
 dex_private_key = "0x111111111117dc0aaaaaa0fa6a738034aaaa302" #this is an example
 #chain_1 #see below for other chain ids or use https://chainlist.org to overwrite settings
 dex_chain_id = 1
 dex_protocol_type = "uniswap_v2" #0x | 1inch | uniswap_v3
 dex_rpc = "https://rpc.ankr.com/eth"
 dex_block_explorer_url = "https://api.etherscan.io/api?"
 dex_block_explorer_api =  "798437294880920392"  #this is an example
-dex_router_contract_addr = "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D" 
-
+dex_router_contract_addr = "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D" #UNI_V2
+# dex_router_contract_addr = "0x68b3465833fb72A70ecDF485E0e4C7bD8665Fc45" #UNI_V3
+dex_quoter_contract_addr = "0x61fFE014bA17989E743c5F6cB21bF9697530B21e" #UNI_V3_QUOTERV2
 #protocol specific
 #🦄1inch
 dex_1inch_url = "https://api.1inch.exchange/v5.0/"
 dex_1inch_limit_url = "https://limit-orders.1inch.io/v3.0/"
 #0️⃣0x
-dex_0x_url = "https://api.0x.org/mainnet/"
+dex_0x_url = "https://api.0x.org/mainnet"
 dex_0x_api_key = "" 
 #🪐apollo
 dex_apollo_url = "https://fapi.apollox.finance/"
 dex_apollo_spot_api_key = ""
 dex_apollo_spot_api_secret = ""
 dex_apollo_future_api_key = ""
 dex_apollo_future_api_secret = ""
```

### Comparing `dxsp-2.2.9/dxsp/main.py` & `dxsp-2.3.0/dxsp/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """
  DEX SWAP Main
 """
 
 import logging
 
 import requests
-from uniswap import Uniswap
 from dxsp import __version__
 from dxsp.config import settings
 
 from pycoingecko import CoinGeckoAPI
 from web3 import Web3
 
 
 class DexSwap:
-    """Do a swap."""
+    """swap  class"""
 
     def __init__(self, w3: Web3 | None = None,):
         """build a dex object """
         self.logger = logging.getLogger(name="DexSwap")
         self.logger.info("DexSwap: %s", __version__)
 
         self.w3 = w3 or Web3(Web3.HTTPProvider(settings.dex_rpc))
@@ -32,24 +31,14 @@
         self.protocol_type = settings.dex_protocol_type
         self.chain_id = settings.dex_chain_id
         # USER
         self.wallet_address = self.w3.to_checksum_address(
             settings.dex_wallet_address)
         self.private_key = settings.dex_private_key
 
-        # UNISWAP 🦄
-        # if self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
-        #     self.uniswap = Uniswap(
-        #         address=self.wallet_address,
-        #         private_key=self.private_key,
-        #         router_contract_addr=settings.dex_router_contract_addr,
-        #         version=2 if self.protocol_type == "uniswap_v2" else 3,
-        #         web3=self.w3,
-        #         default_slippage=settings.dex_trading_slippage)
-
         # COINGECKO 🦎
         try:
             self.cg = CoinGeckoAPI()
             assetplatform = self.cg.get_asset_platforms()
             output_dict = [x for x in assetplatform if x['chain_identifier']
                            == int(self.chain_id)]
             self.cg_platform = output_dict[0]['id']
@@ -65,32 +54,24 @@
         asset_in_address = await self.search_contract(symbol)
         asset_out_symbol = settings.trading_quote_ccy
         asset_out_address = await self.search_contract(asset_out_symbol)
         if asset_out_address is None:
             self.logger.warning("No Valid Contract")
             return
         try:
-            if self.protocol_type in ["1inch", "1inch_limit"]:
-                self.logger.debug("1inch getquote")
-                return await self.get_quote_1inch(
-                    asset_in_address,
-                    asset_out_address)
             if self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
                 self.logger.debug("uniswap getquote")
                 return await self.get_quote_uniswap(
                     asset_in_address,
                     asset_out_address)
             if self.protocol_type == "0x":
                 self.logger.debug("0x getquote")
                 return await self.get_quote_0x(
-                    symbol,
-                    asset_out_symbol,)
-            if self.protocol_type == "apollo":
-                self.logger.debug("apollo getquote")
-                return await self.get_quote_apollo()
+                    asset_in_address,
+                    asset_out_address,)
 
         except Exception as e:
             self.logger.error("get_quote %s", e)
             return
 
     async def get_swap(
                 self,
@@ -107,17 +88,15 @@
                 asset_out_symbol)
             asset_out_contract = await self.get_token_contract(
                 asset_out_symbol)
             if asset_out_contract is None:
                 raise ValueError("No contract identified")
             asset_out_balance = await self.get_token_balance(asset_out_symbol)
             if asset_out_balance == (0 or None):
-                self.logger.warning("No Money")
                 raise ValueError("No Money")
-                return
             # ASSETS IN
             asset_in_address = await self.search_contract(asset_in_symbol)
             self.logger.debug("asset_in_address %s", asset_in_address)
             if asset_in_address is None:
                 return
 
             # AMOUNT
@@ -129,36 +108,30 @@
 
             order_amount = int(
                 (asset_out_amount_converted *
                  (settings.dex_trading_slippage/100)))
             self.logger.debug("order_amount %s", order_amount)
 
             # VERIFY IF ASSET OUT IS APPROVED otherwise get it approved
-            if (await self.get_approve(asset_out_address)) is None:
+            if await self.get_approve(asset_out_address) is None:
                 return
 
             # UNISWAP V2
             if self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
                 swap_order = await self.get_swap_uniswap(
                     asset_out_address,
                     asset_in_address,
                     order_amount)
             # 0x
-            if self.protocol_type == "0x":
+            elif self.protocol_type == "0x":
                 swap_order = await self.get_quote_0x(
-                    asset_in_symbol,
-                    asset_out_symbol,)
-                await self.get_sign(swap_order)
-
-            # 1INCH
-            if self.protocol_type in ["1inch"]:
-                swap_order = await self.get_swap_1inch(
                     asset_out_address,
                     asset_in_address,
                     order_amount)
+                await self.get_sign(swap_order)
 
             if swap_order:
                 self.logger.debug("swap_order %s", swap_order)
                 signed_order = await self.get_sign(swap_order)
                 order_hash = str(self.w3.to_hex(signed_order))
                 order_hash_details = self.w3.wait_for_transaction_receipt(
                                         order_hash,
@@ -246,40 +219,71 @@
                 return order['confirmation']
 
         except Exception as e:
             self.logger.debug("error execute_order %s", e)
             return "error processing order in DXSP"
 
 # 📝CONTRACT SEARCH
-    async def search_contract(
-                            self,
-                            token
-                            ):
+    # async def search_contract(
+    #                         self,
+    #                         token
+    #                         ):
+    #     """search a contract function"""
+    #     self.logger.debug("search_contract")
+
+    #     try:
+    #         token_contract = await self.get_contract_address(
+    #             settings.token_personal_list,
+    #             token)
+    #         if token_contract is None:
+    #             token_contract = await self.get_contract_address(
+    #                 settings.token_testnet_list,
+    #                 token)
+    #             if token_contract is None:
+    #                 token_contract = await self.get_contract_address(
+    #                     settings.token_mainnet_list,
+    #                     token)
+    #                 if token_contract is None:
+    #                     token_contract = await self.search_cg_contract(
+    #                         token)
+    #         if token_contract is not None:
+    #             self.logger.info("%s token: contract found %s",
+    #                              token, token_contract)
+    #             return self.w3.to_checksum_address(token_contract)
+    #         return f"no contract found for {token}"
+    #     except Exception as e:
+    #         self.logger.error("search_contract %s", e)
+    #         return
+    async def search_contract(self, token):
         """search a contract function"""
         self.logger.debug("search_contract")
 
         try:
-            token_contract = await self.get_contract_address(
+            contract_lists = [
                 settings.token_personal_list,
-                token)
-            if token_contract is None:
+                settings.token_testnet_list,
+                settings.token_mainnet_list,
+            ]
+
+            for contract_list in contract_lists:
                 token_contract = await self.get_contract_address(
-                    settings.token_testnet_list,
-                    token)
-                if token_contract is None:
-                    token_contract = await self.get_contract_address(
-                        settings.token_mainnet_list,
-                        token)
-                    if token_contract is None:
-                        token_contract = await self.search_cg_contract(
-                            token)
+                    contract_list,
+                    token
+                )
+                if token_contract is not None:
+                    self.logger.info("%s token: contract found %s",
+                                     token, token_contract)
+                    return self.w3.to_checksum_address(token_contract)
+
+            token_contract = await self.search_cg_contract(token)
             if token_contract is not None:
                 self.logger.info("%s token: contract found %s",
                                  token, token_contract)
                 return self.w3.to_checksum_address(token_contract)
+
             return f"no contract found for {token}"
         except Exception as e:
             self.logger.error("search_contract %s", e)
             return
 
     async def search_cg(self, token):
         """search coingecko"""
@@ -340,15 +344,15 @@
     async def _get(
         self,
         url,
         params=None,
         headers=None
             ):
         try:
-            # self.logger.debug("url: %s", url)
+            self.logger.debug("url: %s", url)
             # self.logger.debug("_header: %s", settings.headers)
             response = requests.get(
                 url,
                 params=params,
                 headers=headers,
                 timeout=10)
             # self.logger.debug("_response: %s", response)
@@ -367,20 +371,30 @@
                 address=self.w3.to_checksum_address(
                     settings.dex_router_contract_addr),
                 abi=router_abi)
             return router
         except Exception as e:
             self.logger.error("router setup: %s", e)
 
+    async def quoter(self):
+        try:
+            quoter_abi = await self.get_abi(settings.dex_quoter_contract_addr)
+            self.logger.debug("quoter_abi: %s", quoter_abi)
+            quoter = self.w3.eth.contract(
+                address=self.w3.to_checksum_address(
+                    settings.dex_quoter_contract_addr),
+                abi=quoter_abi)
+            return quoter
+        except Exception as e:
+            self.logger.error("quoter setup: %s", e)
+
     async def get_approve(self, asset_out_address):
 
         try:
-            if self.protocol_type in ["1inch", "1inch_limit"]:
-                await self.get_approve_1inch(asset_out_address)
-            elif self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
+            if self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
                 await self.get_approve_uniswap(asset_out_address)
         except Exception as e:
             self.logger.error("get_approve %s", e)
             return None
 
     async def get_sign(self, transaction):
 
@@ -436,16 +450,15 @@
                     "action": "getabi",
                     "address": addr,
                     "apikey": settings.dex_block_explorer_api
                     }
                 # Make a GET request to the block explorer URL
                 resp = await self._get(
                     url=settings.dex_block_explorer_url,
-                    params=params,
-                     )
+                    params=params,)
                 # If the response status is 1, log the ABI
                 if resp['status'] == "1":
                     self.logger.debug("ABI found %s", resp)
                     abi = resp["result"]
                     return abi
                 # If no ABI is identified, log a warning
                 self.logger.warning("No ABI identified")
@@ -534,30 +547,51 @@
         try:
             self.logger.debug("get_account_position")
             return
         except Exception as e:
             self.logger.error("get_account_position: %s", e)
             return 0
 
+    async def get_account_margin(
+        self
+         ):
+
+        try:
+            self.logger.debug("get_account_margin")
+            return
+        except Exception as e:
+            self.logger.error("get_account_margin: %s", e)
+            return 0
+
 # PROTOCOL SPECIFIC
-# uniswap v2 🦄
+# uniswap  🦄
     async def get_quote_uniswap(
         self,
         asset_in_address,
         asset_out_address,
         amount=1
     ):
         self.logger.debug("get_quote_uniswap")
         try:
-            router_instance = await self.router()
-            quote = router_instance.functions.getAmountsOut(
-                amount,
-                [asset_in_address, asset_out_address]).call()
-
-            return quote[1]
+            if self.protocol_type == "uniswap_v2":
+                router_instance = await self.router()
+                quote = router_instance.functions.getAmountsOut(
+                    amount,
+                    [asset_in_address, asset_out_address]).call()
+                quote = str(quote[1])
+            elif self.protocol_type == "uniswap_v3":
+                quoter = await self.quoter()
+                sqrtPriceLimitX96 = 0
+                fee = 3000
+                quote = quoter.functions.quoteExactInputSingle(
+                    asset_in_address,
+                    asset_out_address,
+                    fee, amount, sqrtPriceLimitX96).call()
+            return ("🦄 " + quote + " " +
+                    settings.trading_quote_ccy)
         except Exception as e:
             self.logger.error("get_quote_uniswap %s", e)
             return
 
     async def get_approve_uniswap(self, asset_out_address):
 
         try:
@@ -592,29 +626,34 @@
 
     async def get_swap_uniswap(
         self,
         asset_out_address,
         asset_in_address,
         amount
     ):
-        order_path_dex = [asset_out_address, asset_in_address]
+        try:
+            if self.protocol_type == "uniswap_v2":
+                order_path_dex = [asset_out_address, asset_in_address]
 
-        deadline = self.w3.eth.get_block("latest")["timestamp"] + 3600
-        order_min_amount = self.get_quote_uniswap(
-            asset_in_address,
-            asset_out_address,
-            amount)[0]
-        router_instance = await self.router()
-        swap_order = router_instance.functions.swapExactTokensForTokens(
-                        amount,
-                        order_min_amount,
-                        order_path_dex,
-                        self.wallet_address,
-                        deadline)
-        return swap_order
+                deadline = self.w3.eth.get_block("latest")["timestamp"] + 3600
+                order_min_amount = self.get_quote_uniswap(
+                    asset_in_address,
+                    asset_out_address,
+                    amount)[0]
+                router_instance = await self.router()
+                swap_order = (
+                    router_instance.functions.swapExactTokensForTokens(
+                        amount, order_min_amount,
+                        order_path_dex, self.wallet_address,
+                        deadline))
+                return swap_order
+            if self.protocol_type == "uniswap_v3":
+                return None
+        except Exception as e:
+            self.logger.error("get_approve_uniswap %s", e)
 
 # 0️⃣x
     async def get_quote_0x(
         self,
         asset_in_address,
         asset_out_address,
         amount=1
@@ -624,137 +663,21 @@
 
             quote_url = (
                 settings.dex_0x_url
                 + "/swap/v1/quote?buyToken="
                 + str(asset_in_address)
                 + "&sellToken="
                 + str(asset_out_address)
-                + "&sellAmount="
+                + "&buyAmount="
                 + str(asset_out_amount))
             quote_response = await self._get(
                 quote_url,
                 params=None,
                 headers={"0x-api-key": settings.dex_0x_api_key}
                 )
             self.logger.debug("quote_response %s", quote_response)
             if quote_response:
-                quote_amount = quote_response['guaranteedPrice']
-                self.logger.debug("quote_amount %s", quote_amount)
-                # quote_decimals = quote_response['fromToken']['decimals']
-                quote = self.w3.from_wei(int(quote_amount), 'ether')
-                # /(10 ** quote_decimals))
-                return round(quote, 2)
+                quote = quote_response['guaranteedPrice']
+                self.logger.debug("quote_amount %s", quote)
+                return round(float(quote), 3)
         except Exception as e:
             self.logger.error("get_quote_0x %s", e)
-
-# 1inch 🦄
-    async def get_quote_1inch(
-        self,
-        asset_in_address,
-        asset_out_address,
-        amount=1
-    ):
-        try:
-            asset_out_amount = self.w3.to_wei(amount, 'ether')
-            quote_url = (
-                settings.dex_1inch_url
-                + str(self.chain_id)
-                + "/quote?fromTokenAddress="
-                + str(asset_in_address)
-                + "&toTokenAddress="
-                + str(asset_out_address)
-                + "&amount="
-                + str(asset_out_amount))
-            quote_response = await self._get(
-                url=quote_url,
-                params=None,
-                headers=settings.headers)
-            self.logger.debug("quote_response %s", quote_response)
-            if quote_response:
-                quote_amount = quote_response['toTokenAmount']
-                self.logger.debug("quote_amount %s", quote_amount)
-                # quote_decimals = quote_response['fromToken']['decimals']
-                quote = self.w3.from_wei(int(quote_amount), 'ether')
-                # /(10 ** quote_decimals))
-                return round(quote, 2)
-        except Exception as e:
-            self.logger.error("get_quote_1inch %s", e)
-
-    async def get_approve_1inch(self, asset_out_address):
-        try:
-            approval_check_URL = (
-                settings.dex_1inch_url
-                + str(self.chain_id)
-                + "/approve/allowance?tokenAddress="
-                + str(asset_out_address)
-                + "&walletAddress="
-                + str(self.wallet_address))
-            approval_response = await self._get(
-                url=approval_check_URL,
-                params=None,
-                headers=settings.headers)
-            approval_check = approval_response['allowance']
-            if (approval_check == 0):
-                approval_URL = (
-                    settings.dex_1inch_url
-                    + str(self.chain_id)
-                    + "/approve/transaction?tokenAddress="
-                    + str(asset_out_address))
-                approval_response = await self._get(approval_URL)
-                return approval_response
-        except Exception as e:
-            self.logger.error("get_approve_1inch %s", e)
-            return None
-
-    async def get_swap_1inch(
-        self,
-        asset_out_address,
-        asset_in_address,
-        amount
-    ):
-        swap_url = (
-            settings.dex_1inch_url
-            + str(self.chain_id)
-            + "/swap?fromTokenAddress="
-            + asset_out_address
-            + "&toTokenAddress="
-            + asset_in_address
-            + "&amount="
-            + amount
-            + "&fromAddress="
-            + self.wallet_address
-            + "&slippage="
-            + settings.dex_trading_slippage
-            )
-        swap_order = await self._get(
-            url=swap_url,
-            params=None,
-            headers=settings.headers  # headers={'User-Agent': 'Mozilla/5.0'},
-            )
-        swap_order_status = swap_order['statusCode']
-        if swap_order_status != 200:
-            return
-        return swap_order
-
-# apollo finance
-    async def get_quote_apollo(self,):
-        quote_url = (
-            settings.dex_apollo_url
-            + "/fapi/v1/ticker/price"
-            )
-        quote_response = await self._get(
-            url=quote_url,
-            params=None,
-            headers=settings.headers  # headers={'User-Agent': 'Mozilla/5.0'},
-            )
-        self.logger.debug("get_quote_apollo %s", quote_response)
-        quote = quote_response['price']
-        return quote
-
-    async def get_swap_apollo(self):
-        self.logger.warning("Not available")
-    # $ curl -H "X-MBX-APIKEY: dsdfsdf" -X POST
-    # 'https://fapi/apollox.finance/fapi/v1/order?symbol=BTCUSDT&side=BUY&
-    # type=LIMIT&quantity=1&price=9000&timeInForce=GTC&recvWindow=5000&timestamp=1591702613943&
-    # signature= 3c661234138461fcc7a7d8746c6558c9
-    # 842d4e10870d2ecbedf7777cad694af9'
-        return
```

### Comparing `dxsp-2.2.9/pyproject.toml` & `dxsp-2.3.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.2.9"
+version = "2.3.0"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
 "Changelog" =  "https://github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst"
 "Support" =  "https://github.com/mraniki/dxsp/discussions"
 "Issues" =  "https://github.com/mraniki/dxsp/issues"
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.11"
+python = "^3.10"
 asyncio = "*"
 dynaconf = "*"
-web3 = ">=6.0.0"
+web3 = "^6.0.0"
 pycoingecko = "*"
 # uniswap-python = "*"
 # web3client = "*"
 #web3-ethereum-defi = "*"
 # web3client = ">=1.1.8"
 # # many-abis = ">=0.1.7"
 # apollox-connector-python = "*"
 
 
 [tool.poetry.dev-dependencies]
 python-semantic-release = "*"
 pytest = "*"
 pytest-cov = "*"
 pytest-asyncio = "*"
+pytest-mock = "*"
 
 [tool.pytest.ini_options]
 testpaths = "tests/"
 python_classes = [
   "Test*",
   "*Test"
 ]
@@ -53,13 +54,10 @@
 version_variable = ["pyproject.toml:version","dxsp/__init__.py:__version__"]
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "pip install poetry && poetry build"
 commit_parser = "semantic_release.history.emoji_parser"
 use_textual_changelog_sections = true
-
-#patch_emoji # 🐛🚑⚡🔒👽🔍💬🥅♿🍏🐧🏁🤖
-#:ambulance:, :lock:, :bug:, :zap:, :goal_net:, :alien:, :wheelchair:, :speech_balloon:, :mag:, :apple:, :penguin:, :checkered_flag:, :robot:, :green_apple
-#minor_emoji #✨🥚🚸📱💄📈
-#:sparkles:, :children_crossing:, :lipstick:, :iphone:, :egg:, :chart_with_upwards_trend
-#major_emoji¶ #💥:boom:
+major_emoji = "💥,:boom:,BREAKING CHANGE"
+minor_emoji = "feat,🥚,🚀,💄,✨,:rocket:,:sparkles:,:lipstick:,:egg:"
+patch_emoji = "fix,🎨,🐛,🚑,⚡,🔥,🚨,♻️,🔧,⬆️,🩹,👷,📝,🔒,👽,💬,🥅,✅,🐳,🙈,⚗️,🧐,🔇,🔊,:mute:,:loud_sound:,:monocle_face:,:alembic:,:see_no_evil:,:white_check_mark:,:arrow_up:,:recycle:,:fire,:whale:,:art:,:ambulance:,:lock:,:arrow_up:,:bug:,:zap:,:goal_net:,:alien:,:speech_balloon:,:rotating_light:,:construction_worker:"
```

### Comparing `dxsp-2.2.9/PKG-INFO` & `dxsp-2.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,79 +1,74 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.2.9
+Version: 2.3.0
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
-Requires-Python: >=3.10,<3.11
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asyncio
 Requires-Dist: dynaconf
 Requires-Dist: pycoingecko
-Requires-Dist: web3 (>=6.0.0)
+Requires-Dist: web3 (>=6.0.0,<7.0.0)
 Project-URL: Changelog, https://github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/dxsp/issues
 Project-URL: Support, https://github.com/mraniki/dxsp/discussions
 Description-Content-Type: text/markdown
 
 # DXSP (DeX SwaP)
 
 |<img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/231213427-63ea2752-13d5-4993-aee2-90671b57fc6e.png">  | A python defi swap helper package. Swap made easy |
 | ------------- | ------------- |
-|[![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/) ![Version](https://img.shields.io/pypi/v/dxsp)<br>  ![Pypi](https://img.shields.io/pypi/dm/dxsp) [![Docker Pulls](https://badgen.net/docker/pulls/mraniki/dxsp)](https://hub.docker.com/r/mraniki/dxsp)<br>[![✨Flow](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/dxsp/branch/main/graph/badge.svg?token=39ED0ZA6IH)](https://codecov.io/gh/mraniki/dxsp) <br>![](https://healthchecks.io/badge/227be4cc-702a-4ac8-b37b-d3d5a3/UcTrNrys-2/dxsp.svg)<br>[![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko)|24 blockchains (ETH, BSC, ARB, MATIC, OPT...)<br>2 swap protocol (1inch API, UniV2 router)
+|[![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/) ![Version](https://img.shields.io/pypi/v/dxsp)<br>  ![Pypi](https://img.shields.io/pypi/dm/dxsp) [![Docker Pulls](https://badgen.net/docker/pulls/mraniki/dxsp)](https://hub.docker.com/r/mraniki/dxsp)<br> [![✨Flow](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/dxsp/branch/main/graph/badge.svg?token=39ED0ZA6IH)](https://codecov.io/gh/mraniki/dxsp) <br>![](https://healthchecks.io/badge/227be4cc-702a-4ac8-b37b-d3d5a3/UcTrNrys-2/dxsp.svg)<br>[![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko)|Key blockchains (ETH, BSC, ARB, MATIC, OPT...)<br>Key swap protocol (UniV2 router)
 
 Key features:
 
 - Any blockchains mainnet or testnet supported by web3py, 1inch or uniswap type router.
-- 2 swap protocol type supported:
-  - Uniswap version 2 router protocol type
-  - 1inch API v5
+
 
 Other features:
 
 - Translate token symbol to contract address via user defined tokenlist format or coingecko api
 - Connect to web3 automatically (optionn to provide a web3 object)
 - Approve contract and sign transaction
 - Quote a given token
 - Use Base trading symbol like stablecoin
 - Settings to use the module for your own setup
 
-# Install
+## Install
 
 `pip install dxsp`
 
-# How to use it
+## How to use it
 
 ```
 from dxsp import DexSwap
 
  dex = DexSwap()
  #BUY 10 USDC to SWAP with BITCOIN
  demo_tx = await dex.get_swap('USDT','wBTC',10)
  print("demo_tx ", demo_tx)
 ```
 
-## Example
+### Example
 
 [example](https://github.com/mraniki/dxsp/blob/main/examples/example.py)
 
 
-## Real use case
+### Real use case
 
 [TalkyTrader, submit trading order to CEX & DEX with messaging platform (Telegram, Matrix and Discord)](https://github.com/mraniki/tt)
 
-# Documentation
-
-<https://github.com/mraniki/dxsp/wiki>
-
-## 🚧 Roadmap
+## Documentation
 
-[🚧 Roadmap](https://github.com/mraniki/dxsp/milestones)
+[wiki](https://github.com/mraniki/dxsp/wiki)
 
 ## Questions? Want to help?
 
 [![discord](https://badgen.net/badge/icon/discord/purple?icon=discord&label)](https://discord.gg/vegJQGrRRa)
 [![telegram](https://badgen.net/badge/icon/telegram?icon=telegram&label)](https://t.me/TTTalkyTraderChat/1)
```

