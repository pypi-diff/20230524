# Comparing `tmp/dxsp-2.3.0.tar.gz` & `tmp/dxsp-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.3.0.tar", max compression
+gzip compressed data, was "dxsp-2.3.1.tar", max compression
```

## Comparing `dxsp-2.3.0.tar` & `dxsp-2.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-05-24 10:19:16.102585 dxsp-2.3.0/LICENSE
--rw-r--r--   0        0        0     2439 2023-05-24 10:19:16.102585 dxsp-2.3.0/README.md
--rw-r--r--   0        0        0       86 2023-05-24 10:19:17.146592 dxsp-2.3.0/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-24 10:19:16.102585 dxsp-2.3.0/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-24 10:19:16.102585 dxsp-2.3.0/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      388 2023-05-24 10:19:16.102585 dxsp-2.3.0/dxsp/config.py
--rw-r--r--   0        0        0     3315 2023-05-24 10:19:16.102585 dxsp-2.3.0/dxsp/default_settings.toml
--rw-r--r--   0        0        0    25909 2023-05-24 10:19:16.102585 dxsp-2.3.0/dxsp/main.py
--rw-r--r--   0        0        0     1960 2023-05-24 10:19:17.146592 dxsp-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 dxsp-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-24 14:56:23.577067 dxsp-2.3.1/LICENSE
+-rw-r--r--   0        0        0     2439 2023-05-24 14:56:23.581067 dxsp-2.3.1/README.md
+-rw-r--r--   0        0        0       86 2023-05-24 14:56:24.453069 dxsp-2.3.1/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-24 14:56:23.581067 dxsp-2.3.1/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-24 14:56:23.581067 dxsp-2.3.1/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      388 2023-05-24 14:56:23.581067 dxsp-2.3.1/dxsp/config.py
+-rw-r--r--   0        0        0     3552 2023-05-24 14:56:23.581067 dxsp-2.3.1/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    26416 2023-05-24 14:56:23.581067 dxsp-2.3.1/dxsp/main.py
+-rw-r--r--   0        0        0     1973 2023-05-24 14:56:24.453069 dxsp-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 dxsp-2.3.1/PKG-INFO
```

### Comparing `dxsp-2.3.0/LICENSE` & `dxsp-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.3.0/README.md` & `dxsp-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.3.0/dxsp/assets/blockchains.py` & `dxsp-2.3.1/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.3.0/dxsp/default_settings.toml` & `dxsp-2.3.1/dxsp/default_settings.toml`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 #chain_1 #see below for other chain ids or use https://chainlist.org to overwrite settings
 dex_chain_id = 1
 dex_protocol_type = "uniswap_v2" #0x | 1inch | uniswap_v3
 dex_rpc = "https://rpc.ankr.com/eth"
 dex_block_explorer_url = "https://api.etherscan.io/api?"
 dex_block_explorer_api =  "798437294880920392"  #this is an example
 dex_router_contract_addr = "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D" #UNI_V2
+dex_router_abi_url = "https://raw.githubusercontent.com/uniswap-python/uniswap-python/master/uniswap/assets/uniswap-v2/router02.abi"
+dex_erc20_abi_url = "https://raw.githubusercontent.com/web3/web3.js/4.x/fixtures/build/ERC20Token.json"
 # dex_router_contract_addr = "0x68b3465833fb72A70ecDF485E0e4C7bD8665Fc45" #UNI_V3
 dex_quoter_contract_addr = "0x61fFE014bA17989E743c5F6cB21bF9697530B21e" #UNI_V3_QUOTERV2
 #protocol specific
 #🦄1inch
 dex_1inch_url = "https://api.1inch.exchange/v5.0/"
 dex_1inch_limit_url = "https://limit-orders.1inch.io/v3.0/"
 #0️⃣0x
```

### Comparing `dxsp-2.3.0/dxsp/main.py` & `dxsp-2.3.1/dxsp/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,26 +294,26 @@
                              x['symbol'] == token.upper()]
             api_dict = [sub['api_symbol'] for sub in filtered_dict]
             for i in api_dict:
                 coin_dict = self.cg.get_coin_by_id(i)
                 try:
                     if coin_dict['platforms'][f'{self.cg_platform}']:
                         return coin_dict
-                except KeyError:
+                except (KeyError, requests.exceptions.HTTPError):
                     pass
         except Exception as e:
             self.logger.error("search_cg %s", e)
             return
 
     async def search_cg_contract(self, token):
         """search coingecko contract"""
         try:
             coin_info = await self.search_cg(token)
-            if coin_info is not None:
-                return coin_info['platforms'][f'{self.cg_platform}']
+            return (coin_info['platforms'][f'{self.cg_platform}']
+                    if coin_info is not None else None)
         except Exception as e:
             self.logger.error(" search_cg_contract: %s", e)
             return
 
     async def get_contract_address(self, token_list_url, symbol):
         """Given a token symbol and json tokenlist, get token address"""
         try:
@@ -329,14 +329,17 @@
 
     async def get_token_contract(self, token):
         """Given a token symbol, returns a contract object. """
         self.logger.debug("get_token_contract %s", token)
         try:
             token_address = await self.search_contract(token)
             token_abi = await self.get_abi(token_address)
+            if token_abi is None:
+                self.logger.debug("using setting dex_erc20_abi_url")
+                token_abi = requests.get(settings.dex_erc20_abi_url).text
             return self.w3.eth.contract(
                 address=token_address,
                 abi=token_abi)
         except Exception as e:
             self.logger.error("get_token_contract %s", e)
             return
 
@@ -362,14 +365,17 @@
 
         except Exception as e:
             self.logger.error("_get: %s", e)
 
     async def router(self):
         try:
             router_abi = await self.get_abi(settings.dex_router_contract_addr)
+            if router_abi is None:
+                self.logger.debug("using setting dex_router_abi_url")
+                router_abi = requests.get(settings.dex_router_abi_url).text
             self.logger.debug("router_abi: %s", router_abi)
             router = self.w3.eth.contract(
                 address=self.w3.to_checksum_address(
                     settings.dex_router_contract_addr),
                 abi=router_abi)
             return router
         except Exception as e:
@@ -573,15 +579,17 @@
         self.logger.debug("get_quote_uniswap")
         try:
             if self.protocol_type == "uniswap_v2":
                 router_instance = await self.router()
                 quote = router_instance.functions.getAmountsOut(
                     amount,
                     [asset_in_address, asset_out_address]).call()
-                quote = str(quote[1])
+                self.logger.error("quote %s", quote)
+                if isinstance(quote, list):
+                    quote = str(quote[0])
             elif self.protocol_type == "uniswap_v3":
                 quoter = await self.quoter()
                 sqrtPriceLimitX96 = 0
                 fee = 3000
                 quote = quoter.functions.quoteExactInputSingle(
                     asset_in_address,
                     asset_out_address,
```

### Comparing `dxsp-2.3.0/pyproject.toml` & `dxsp-2.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.3.0"
+version = "2.3.1"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
@@ -40,15 +40,15 @@
   "*Test"
 ]
 log_format = "%(asctime)s - %(levelname)s - %(name)s - %(message)s"
 log_level = "DEBUG"
 pythonpath = [
   "."
 ]
-addopts = "--ignore-glob=example_*"
+addopts = "--capture=no --ignore-glob=example_*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 version_variable = ["pyproject.toml:version","dxsp/__init__.py:__version__"]
```

### Comparing `dxsp-2.3.0/PKG-INFO` & `dxsp-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.3.0
+Version: 2.3.1
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

