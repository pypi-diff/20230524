# Comparing `tmp/rubi-1.3.1.tar.gz` & `tmp/rubi-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubi-1.3.1.tar", max compression
+gzip compressed data, was "rubi-1.3.2.tar", max compression
```

## Comparing `rubi-1.3.1.tar` & `rubi-1.3.2.tar`

### file list

```diff
@@ -1,39 +1,38 @@
--rw-r--r--   0        0        0    11357 2023-02-09 17:21:21.757346 rubi-1.3.1/LICENSE
--rw-r--r--   0        0        0     1301 2023-02-14 16:34:53.712864 rubi-1.3.1/README.md
--rw-r--r--   0        0        0      718 2023-02-28 17:59:52.512396 rubi-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      735 2023-02-14 16:34:53.715731 rubi-1.3.1/rubi/README.md
--rw-r--r--   0        0        0       25 2023-02-09 17:21:21.760544 rubi-1.3.1/rubi/__init__.py
--rw-r--r--   0        0        0       22 2023-02-09 17:21:21.760681 rubi-1.3.1/rubi/book/__init__.py
--rw-r--r--   0        0        0     6750 2023-02-09 17:21:21.760791 rubi-1.3.1/rubi/book/book.py
--rw-r--r--   0        0        0      183 2023-02-14 16:34:53.715874 rubi-1.3.1/rubi/contracts/__init__.py
--rw-r--r--   0        0        0    61065 2023-02-14 16:34:53.716268 rubi-1.3.1/rubi/contracts/aid.py
--rw-r--r--   0        0        0       69 2023-02-09 17:21:21.761424 rubi-1.3.1/rubi/contracts/helper/__init__.py
--rw-r--r--   0        0        0     6735 2023-02-09 17:21:21.761755 rubi-1.3.1/rubi/contracts/helper/abis/ERC20.json
--rw-r--r--   0        0        0    17057 2023-02-09 17:21:21.762046 rubi-1.3.1/rubi/contracts/helper/abis/MarketAid.json
--rw-r--r--   0        0        0     2649 2023-02-09 17:21:21.762146 rubi-1.3.1/rubi/contracts/helper/abis/MarketAidFactory.json
--rw-r--r--   0        0        0    37232 2023-02-09 17:21:21.762272 rubi-1.3.1/rubi/contracts/helper/abis/RubiconMarket.json
--rw-r--r--   0        0        0    15314 2023-02-09 17:21:21.762375 rubi-1.3.1/rubi/contracts/helper/abis/RubiconRouter.json
--rw-r--r--   0        0        0    22002 2023-02-14 16:34:53.716553 rubi-1.3.1/rubi/contracts/helper/erc20.py
--rw-r--r--   0        0        0     5371 2023-02-14 16:34:53.716723 rubi-1.3.1/rubi/contracts/helper/rolodex.py
--rw-r--r--   0        0        0    38518 2023-02-14 16:34:53.716886 rubi-1.3.1/rubi/contracts/market.py
--rw-r--r--   0        0        0    11564 2023-02-14 16:34:53.717077 rubi-1.3.1/rubi/contracts/router.py
--rw-r--r--   0        0        0      206 2023-02-14 16:34:53.717196 rubi-1.3.1/rubi/data/README.md
--rw-r--r--   0        0        0       33 2023-02-14 16:34:53.717274 rubi-1.3.1/rubi/data/__init__.py
--rw-r--r--   0        0        0     3932 2023-02-14 16:34:53.717374 rubi-1.3.1/rubi/data/data.py
--rw-r--r--   0        0        0     1198 2023-02-14 16:34:53.717485 rubi-1.3.1/rubi/data/processing/README.md
--rw-r--r--   0        0        0       64 2023-02-14 16:34:53.717551 rubi-1.3.1/rubi/data/processing/__init__.py
--rw-r--r--   0        0        0    13964 2023-02-28 17:54:34.917046 rubi-1.3.1/rubi/data/processing/aid.py
--rw-r--r--   0        0        0       31 2023-02-14 16:34:53.717742 rubi-1.3.1/rubi/data/processing/helper/__init__.py
--rw-r--r--   0        0        0     2292 2023-02-14 16:34:53.717833 rubi-1.3.1/rubi/data/processing/helper/processing.py
--rw-r--r--   0        0        0    10226 2023-02-14 16:34:53.717931 rubi-1.3.1/rubi/data/processing/user.py
--rw-r--r--   0        0        0       69 2023-02-14 16:34:53.718073 rubi-1.3.1/rubi/data/sources/__init__.py
--rw-r--r--   0        0        0    20955 2023-02-28 17:23:09.587519 rubi-1.3.1/rubi/data/sources/aid.py
--rw-r--r--   0        0        0     1194 2023-02-14 16:34:53.718302 rubi-1.3.1/rubi/data/sources/helper/README.md
--rw-r--r--   0        0        0       76 2023-02-14 16:34:53.718369 rubi-1.3.1/rubi/data/sources/helper/__init__.py
--rw-r--r--   0        0        0    12589 2023-02-27 02:08:49.086543 rubi-1.3.1/rubi/data/sources/helper/gas.py
--rw-r--r--   0        0        0    15373 2023-02-14 16:34:53.718597 rubi-1.3.1/rubi/data/sources/helper/price.py
--rw-r--r--   0        0        0     7319 2023-02-14 16:34:53.718699 rubi-1.3.1/rubi/data/sources/helper/rolodex.py
--rw-r--r--   0        0        0    22425 2023-02-14 16:34:53.718888 rubi-1.3.1/rubi/data/sources/market.py
--rw-r--r--   0        0        0     8258 2023-02-14 16:34:53.719121 rubi-1.3.1/rubi/rubi.py
--rw-r--r--   0        0        0     2485 1970-01-01 00:00:00.000000 rubi-1.3.1/setup.py
--rw-r--r--   0        0        0     2128 1970-01-01 00:00:00.000000 rubi-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-09 17:21:21.757346 rubi-1.3.2/LICENSE
+-rw-r--r--   0        0        0     1282 2023-05-24 19:25:18.033040 rubi-1.3.2/README.md
+-rw-r--r--   0        0        0      676 2023-05-24 19:27:47.087742 rubi-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0      734 2023-05-24 19:25:18.036048 rubi-1.3.2/rubi/README.md
+-rw-r--r--   0        0        0       25 2023-02-09 17:21:21.760544 rubi-1.3.2/rubi/__init__.py
+-rw-r--r--   0        0        0       22 2023-02-09 17:21:21.760681 rubi-1.3.2/rubi/book/__init__.py
+-rw-r--r--   0        0        0     6750 2023-02-09 17:21:21.760791 rubi-1.3.2/rubi/book/book.py
+-rw-r--r--   0        0        0      183 2023-02-14 16:34:53.715874 rubi-1.3.2/rubi/contracts/__init__.py
+-rw-r--r--   0        0        0    61065 2023-02-14 16:34:53.716268 rubi-1.3.2/rubi/contracts/aid.py
+-rw-r--r--   0        0        0       69 2023-02-09 17:21:21.761424 rubi-1.3.2/rubi/contracts/helper/__init__.py
+-rw-r--r--   0        0        0     6735 2023-02-09 17:21:21.761755 rubi-1.3.2/rubi/contracts/helper/abis/ERC20.json
+-rw-r--r--   0        0        0    17057 2023-02-09 17:21:21.762046 rubi-1.3.2/rubi/contracts/helper/abis/MarketAid.json
+-rw-r--r--   0        0        0     2649 2023-02-09 17:21:21.762146 rubi-1.3.2/rubi/contracts/helper/abis/MarketAidFactory.json
+-rw-r--r--   0        0        0    37232 2023-02-09 17:21:21.762272 rubi-1.3.2/rubi/contracts/helper/abis/RubiconMarket.json
+-rw-r--r--   0        0        0    15314 2023-02-09 17:21:21.762375 rubi-1.3.2/rubi/contracts/helper/abis/RubiconRouter.json
+-rw-r--r--   0        0        0    22002 2023-02-14 16:34:53.716553 rubi-1.3.2/rubi/contracts/helper/erc20.py
+-rw-r--r--   0        0        0     5371 2023-02-14 16:34:53.716723 rubi-1.3.2/rubi/contracts/helper/rolodex.py
+-rw-r--r--   0        0        0    38518 2023-02-14 16:34:53.716886 rubi-1.3.2/rubi/contracts/market.py
+-rw-r--r--   0        0        0    11564 2023-02-14 16:34:53.717077 rubi-1.3.2/rubi/contracts/router.py
+-rw-r--r--   0        0        0      206 2023-02-14 16:34:53.717196 rubi-1.3.2/rubi/data/README.md
+-rw-r--r--   0        0        0       33 2023-02-14 16:34:53.717274 rubi-1.3.2/rubi/data/__init__.py
+-rw-r--r--   0        0        0     3932 2023-02-14 16:34:53.717374 rubi-1.3.2/rubi/data/data.py
+-rw-r--r--   0        0        0     1198 2023-02-14 16:34:53.717485 rubi-1.3.2/rubi/data/processing/README.md
+-rw-r--r--   0        0        0       64 2023-02-14 16:34:53.717551 rubi-1.3.2/rubi/data/processing/__init__.py
+-rw-r--r--   0        0        0    20226 2023-03-28 22:32:44.963776 rubi-1.3.2/rubi/data/processing/aid.py
+-rw-r--r--   0        0        0       31 2023-02-14 16:34:53.717742 rubi-1.3.2/rubi/data/processing/helper/__init__.py
+-rw-r--r--   0        0        0     2292 2023-02-14 16:34:53.717833 rubi-1.3.2/rubi/data/processing/helper/processing.py
+-rw-r--r--   0        0        0    10226 2023-02-14 16:34:53.717931 rubi-1.3.2/rubi/data/processing/user.py
+-rw-r--r--   0        0        0       69 2023-02-14 16:34:53.718073 rubi-1.3.2/rubi/data/sources/__init__.py
+-rw-r--r--   0        0        0    21161 2023-03-28 22:32:44.964336 rubi-1.3.2/rubi/data/sources/aid.py
+-rw-r--r--   0        0        0     1194 2023-02-14 16:34:53.718302 rubi-1.3.2/rubi/data/sources/helper/README.md
+-rw-r--r--   0        0        0       76 2023-02-14 16:34:53.718369 rubi-1.3.2/rubi/data/sources/helper/__init__.py
+-rw-r--r--   0        0        0    12589 2023-02-27 02:08:49.086543 rubi-1.3.2/rubi/data/sources/helper/gas.py
+-rw-r--r--   0        0        0    15373 2023-02-14 16:34:53.718597 rubi-1.3.2/rubi/data/sources/helper/price.py
+-rw-r--r--   0        0        0     7319 2023-02-14 16:34:53.718699 rubi-1.3.2/rubi/data/sources/helper/rolodex.py
+-rw-r--r--   0        0        0    22425 2023-02-14 16:34:53.718888 rubi-1.3.2/rubi/data/sources/market.py
+-rw-r--r--   0        0        0     8258 2023-05-24 19:15:33.694846 rubi-1.3.2/rubi/rubi.py
+-rw-r--r--   0        0        0     2102 1970-01-01 00:00:00.000000 rubi-1.3.2/PKG-INFO
```

### Comparing `rubi-1.3.1/LICENSE` & `rubi-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rubi-1.3.1/README.md` & `rubi-1.3.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -5,12 +5,12 @@
 the underlying goal of the design of rubi is to decrease user friction when interacting with the protocol, and when interacting with the sdk. we want to enable the user
 as much access as possible without requiring any input from the user. for example, by breaking up the contract functionality into read and write classes, we enable the user to
 use the sdk to read from the protocol without passing in any keys. within the data classes, we aim to provide as much information as possible to the user without requiring any 
 additional input such as api keys. when it is clearly useful, we will add higher level classes that provide additional functionality to the user by requiring additional input. 
 
 ### SDK Disclaimer
 
-This codebase is in Alpha and could contain bugs or change significantly between versions. Contributing through Issues or Pull Requests is welcome!
+this codebase is in Alpha and could contain bugs or change significantly between versions. contributing through Issues or Pull Requests is welcome!
 
 ### Protocol Disclaimer
 
-Please refer to [this](https://docs.rubicon.finance/docs/protocol/rubicon-pools/risks) for information on the risks associated to the Rubicon Protocol.
+please refer to [this](https://docs.rubicon.finance/protocol/risks) for information on the risks associated to the Rubicon Protocol.
```

### Comparing `rubi-1.3.1/pyproject.toml` & `rubi-1.3.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "rubi"
-version = "1.3.1"
+version = "1.3.2"
 description = "a python SDK for the Rubicon Protocol"
 authors = ["denver <denver@rubicon.finance>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-sphinx = "^5.3.0"
-web3 = { version = "^6.0.0b", allow-prereleases = true }
+sphinx = "7.0.1"
+web3 = "^6.4.0"
 hexbytes = "^0.3.0"
 attributedict = "^0.3.0"
-eth-abi = "^3.0.1"
-pytest = "^7.2.0"
-eth-tester = "^0.8.0b1"
-py-evm = "^0.6.1a1"
+eth-abi = "^4.0.0"
+pytest = "^7.3.1"
+eth-tester = "^0.9.0b1"
+py-evm = "^0.7.0a2"
 eth-utils = "^2.1.0"
-subgrounds = { version = "^1.0.3", extras = ["dash"] }
+subgrounds = { version = "^1.5.1", extras = ["dash"] }
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = "^0.21.0"
 ipykernel = "^6.5.0"
 jupyter = "^1.0.0"
 
 [tool.poetry.extras]
```

### Comparing `rubi-1.3.1/rubi/README.md` & `rubi-1.3.2/rubi/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 # decisions and considerations 
 
 ### writing to the chain 
 throughout the codebase we offer the user the option to pass in a nonce argument or derive it from chain state if none is provided (via the `get_nonce` function). aspirationally, we want 
 to support a python based nonce manager that can be used to manage nonces for the user. until then, this optional parameter is meant to enable the user to manage nonces themselves. when a
-user does not provide a nonce, we derive it from chain state accordingly. in this case, we also wait for the transaction to be confirmed before continueing. if the transaction fails, 
+user does not provide a nonce, we derive it from chain state accordingly. in this case, we also wait for the transaction to be confirmed before continuing. if the transaction fails, 
 an exception is raised and the program is exited. the user can override this behavior by managing nonces themselves.
```

### Comparing `rubi-1.3.1/rubi/book/book.py` & `rubi-1.3.2/rubi/book/book.py`

 * *Files identical despite different names*

### Comparing `rubi-1.3.1/rubi/contracts/aid.py` & `rubi-1.3.2/rubi/contracts/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-1.3.1/rubi/contracts/helper/abis/ERC20.json` & `rubi-1.3.2/rubi/contracts/helper/abis/ERC20.json`

 * *Files identical despite different names*

### Comparing `rubi-1.3.1/rubi/contracts/helper/abis/MarketAid.json` & `rubi-1.3.2/rubi/contracts/helper/abis/MarketAid.json`

 * *Files identical despite different names*

### Comparing `rubi-1.3.1/rubi/contracts/helper/abis/MarketAidFactory.json` & `rubi-1.3.2/rubi/contracts/helper/abis/MarketAidFactory.json`

 * *Files identical despite different names*

### Comparing `rubi-1.3.1/rubi/contracts/helper/abis/RubiconMarket.json` & `rubi-1.3.2/rubi/contracts/helper/abis/RubiconMarket.json`

 * *Files identical despite different names*

### Comparing `rubi-1.3.1/rubi/contracts/helper/abis/RubiconRouter.json` & `rubi-1.3.2/rubi/contracts/helper/abis/RubiconRouter.json`

 * *Files identical despite different names*

### Comparing `rubi-1.3.1/rubi/contracts/helper/erc20.py` & `rubi-1.3.2/rubi/contracts/helper/erc20.py`

 * *Files identical despite different names*

### Comparing `rubi-1.3.1/rubi/contracts/helper/rolodex.py` & `rubi-1.3.2/rubi/contracts/helper/rolodex.py`

 * *Files identical despite different names*

### Comparing `rubi-1.3.1/rubi/contracts/market.py` & `rubi-1.3.2/rubi/contracts/market.py`

 * *Files identical despite different names*

### Comparing `rubi-1.3.1/rubi/contracts/router.py` & `rubi-1.3.2/rubi/contracts/router.py`

 * *Files identical despite different names*

### Comparing `rubi-1.3.1/rubi/data/data.py` & `rubi-1.3.2/rubi/data/data.py`

 * *Files identical despite different names*

### Comparing `rubi-1.3.1/rubi/data/processing/README.md` & `rubi-1.3.2/rubi/data/processing/README.md`

 * *Files identical despite different names*

### Comparing `rubi-1.3.1/rubi/data/processing/aid.py` & `rubi-1.3.2/rubi/data/processing/aid.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,15 +9,116 @@
 
     def __init__(self, subgrounds, chain_id, AidData):
         """constructor method to initialize the data source class"""
 
         self.price = Price()
         self.process = Process()
         self.network = networks[chain_id]()
-        self.market_aid = AidData #AidData(subgrounds, chain_id)
+        self.market_aid = AidData 
+
+    def recreate_aid_history(self, aid, bin_size = 60, raw=False): 
+        """this method takes an aid address and builds a dataframe of that aid balance over time. its precision is to the second. it does this by taking the ending assset balance at each second.
+        
+        :param aid: the address of the aid instance
+        :type aid: str
+        :param bin_size: the bin size of the analysis (for now this only adjusts the price data precision)
+        :type bin_size: int
+        :return: a dataframe that shows the various asset balances of the aid instance over a period of time
+        :rtype: pandas.DataFrame (columns: )
+        """
+
+        # get the aid history
+        df = self.market_aid.get_aid_history(aid = aid, bin_size = bin_size)
+
+        # create a dataframe the encompasses the period of the aid history 
+        min_timestamp = int(df['timestamp'].min())
+        max_timestamp = int(df['timestamp'].max())
+        timestamp_range = list(range(min_timestamp, max_timestamp))
+        history = pd.DataFrame(timestamp_range, columns=['timestamp'])
+
+        # group by asset 
+        aid_history_grouped = df.groupby('asset')
+
+        # iterate through each group and get the balance at the max index position for every timestamp
+        for asset, group in aid_history_grouped:
+            
+            # make sure the group is sorted by: block, block_index, timestamp
+            group = group.sort_values(by = ['block', 'block_index', 'timestamp']).reset_index(drop = True)
+
+            # set this sorted index as a column so we can identify the end balance of an asset 
+            group['sorted_index'] = group.index
+
+            # get the sum of the credits and debits for each timestamp
+            credits = group.groupby(['timestamp']).agg({'credits_debits' : 'sum'}).reset_index()
+            credits_raw = group.groupby(['timestamp']).agg({'credits_debits_raw' : 'sum'}).reset_index()
+
+            # fill in the credits and debits for each timestamp
+            history[f'{asset}_credits'] = history['timestamp'].map(credits.set_index('timestamp')['credits_debits'].to_dict()).fillna(0)
+            history[f'{asset}_credits_raw'] = history['timestamp'].map(credits_raw.set_index('timestamp')['credits_debits_raw'].to_dict()).fillna(0)
+
+            # go through and get the max sorted_index for each timestamp
+            idx = group.groupby(['timestamp'])['sorted_index'].idxmax()
+            filtered_group = group.loc[idx]
+
+            # fill in the balance for each asset at the end of each timestamp
+            history[f'{asset}_balance'] = history['timestamp'].map(filtered_group.set_index('timestamp')['balance'].to_dict()).fillna(method='ffill').fillna(0)
+            history[f'{asset}_balance_raw'] = history['timestamp'].map(filtered_group.set_index('timestamp')['balance_raw'].to_dict()).fillna(method='ffill').fillna(0)
+
+            # get coinbase ticker for the pair and retrieve the price data
+            ticker = self.network.coinbase_tickers[asset]
+            prices = self.price.get_price_in_range(start = min_timestamp, end = max_timestamp, pair = ticker)
+
+            # fill in the price for each asset at the beginning of each minute period
+            history[f'{asset}_price'] = history['timestamp'].map(prices).fillna(method='ffill').fillna(method='bfill').fillna(0)
+
+        assets = [asset for asset, group in aid_history_grouped]
+
+        return {'data' : history, 'assets' : assets}
+
+    def evaluate_aid_performance(self, data, assets, start_time=None, end_time=None):
+        """this function simply takes an aid history, truncates the dataframe by a start and end time (if given), and compares the book value of holding the asset balance at the beginning of the period (adjusting for any deposits / withdrawals during the period) against the actual aid balances. this function is intended to be used with dataframes created by the function `recreate_aid_history`
+        
+        :param data: a dataframe (ideally returned by the function recreate_aid_history) 
+        :type data: pandas.DataFrame
+        :param assets: an array of relevant assests for the dataframe (ideally returned by the function recreate_aid_history) 
+        :type assets: array 
+        :param start_time: the start time of which to conduct an analysis for (this determines what asset mix is used in comparison against the aids real book value / real asset mix)
+        :type start_time: int
+        :param end_time: the end time of which to conduct the analysis through 
+        :param end_time: int
+        """
+
+        if start_time:
+            data = data[data['timestamp'] >= start_time].reset_index(drop = True)
+        if end_time: 
+            data = data[data['timestamp'] <= end_time].reset_index(drop = True)
+
+        # set the credits equal to the balance of each asset at index 0
+        for asset in assets:
+            data[f'{asset}_credits'].iloc[0] = data[f'{asset}_balance'].iloc[0]
+            data[f'{asset}_credits_raw'].iloc[0] = data[f'{asset}_balance_raw'].iloc[0]
+
+            # create a cumulative sum of the credits and debits
+            data[f'{asset}_credits_total'] = data[f'{asset}_credits'].cumsum()
+            data[f'{asset}_credits_total_raw'] = data[f'{asset}_credits_raw'].cumsum()
+
+            # calculate the delta from the credits totals
+            data[f'{asset}_balance_delta'] = data[f'{asset}_balance'] - data[f'{asset}_credits_total']
+            data[f'{asset}_balance_delta_raw'] = data[f'{asset}_balance_raw'] - data[f'{asset}_credits_total_raw']
+
+            # calculate the usd value of the balance, credits, and delta
+            data[f'{asset}_balance_usd'] = data[f'{asset}_balance'] * data[f'{asset}_price']
+            data[f'{asset}_credits_total_usd'] = data[f'{asset}_credits_total'] * data[f'{asset}_price']
+            data[f'{asset}_balance_delta_usd'] = data[f'{asset}_balance_delta'] * data[f'{asset}_price']
+
+        data['total_balance_usd'] = data[[f'{asset}_balance_usd' for asset in assets]].sum(axis = 1)
+        data['total_credits_usd'] = data[[f'{asset}_credits_total_usd' for asset in assets]].sum(axis = 1)
+        data['total_balance_delta_usd'] = data[[f'{asset}_balance_delta_usd' for asset in assets]].sum(axis = 1) 
+
+        return {'data' : data, 'assets' : assets}
 
     def analyze_aid_history(self, aid, start_time=None, end_time=None, bin_size=60, raw=False):
         """this method takes the aid history entities and composes a dataframe that shows the various asset balances of the aid instance over a period of time, the entire aid history if no start and end time are provided. one caveat, when a dataframe begins after the aid instance was created, the first row has a credit of the balance at that point in time.
         
         :param aid: the address of the aid instance
         :type aid: str
         :param start_time: the start time of the analysis
@@ -84,15 +185,15 @@
                 credits_debits[asset] = group.set_index('timestamp').to_dict()['credits_debits']
 
         # build the dataframe
         history = pd.DataFrame(timestamp_range, columns=['timestamp'])
     
         # add in the data for each asset
         for asset in assets:
-            history[f'{asset}_balance'] = history['timestamp'].map(asset_balances[asset].get).fillna(method='ffill').fillna(0)
+            history[f'{asset}_balance'] = history['timestamp'].map(asset_balances[asset]).fillna(method='ffill').fillna(0)
 
         for asset in assets: 
             history[f'{asset}_hodl_balance'] = history['timestamp'].map(credits_debits[asset]).fillna(method='ffill').fillna(0)
         
         for asset in assets:
             history[f'{asset}_delta'] = history['timestamp'].map(asset_deltas[asset]).fillna(method='ffill').fillna(0)
```

### Comparing `rubi-1.3.1/rubi/data/processing/helper/processing.py` & `rubi-1.3.2/rubi/data/processing/helper/processing.py`

 * *Files identical despite different names*

### Comparing `rubi-1.3.1/rubi/data/processing/user.py` & `rubi-1.3.2/rubi/data/processing/user.py`

 * *Files identical despite different names*

### Comparing `rubi-1.3.1/rubi/data/sources/aid.py` & `rubi-1.3.2/rubi/data/sources/aid.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,19 @@
         if asset:
             where['aid_token_'] = {'token' : asset.lower()}
         if start_time:
             where['timestamp_gte'] = start_time
         if end_time:
             where['timestamp_lte'] = end_time
 
-        histories = self.market_aid.Query.aidTokenHistories(first = first, where = [AidToken.aid == aid.lower()])
+        #histories = self.market_aid.Query.aidTokenHistories(first = first, where = [AidToken.aid == aid.lower()])
+        if where:
+            histories = self.market_aid.Query.aidTokenHistories(first = first, where = where)
+        else:
+            histories = self.market_aid.Query.aidTokenHistories(first = first)
 
         field_paths = [
             histories.timestamp,
             histories.time_bin,
             histories.aid_token.token.symbol,
             histories.balance_formatted,
             histories.balance_change_formatted,
```

### Comparing `rubi-1.3.1/rubi/data/sources/helper/README.md` & `rubi-1.3.2/rubi/data/sources/helper/README.md`

 * *Files identical despite different names*

### Comparing `rubi-1.3.1/rubi/data/sources/helper/gas.py` & `rubi-1.3.2/rubi/data/sources/helper/gas.py`

 * *Files identical despite different names*

### Comparing `rubi-1.3.1/rubi/data/sources/helper/price.py` & `rubi-1.3.2/rubi/data/sources/helper/price.py`

 * *Files identical despite different names*

### Comparing `rubi-1.3.1/rubi/data/sources/helper/rolodex.py` & `rubi-1.3.2/rubi/data/sources/helper/rolodex.py`

 * *Files identical despite different names*

### Comparing `rubi-1.3.1/rubi/data/sources/market.py` & `rubi-1.3.2/rubi/data/sources/market.py`

 * *Files identical despite different names*

### Comparing `rubi-1.3.1/rubi/rubi.py` & `rubi-1.3.2/rubi/rubi.py`

 * *Files identical despite different names*

### Comparing `rubi-1.3.1/PKG-INFO` & `rubi-1.3.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: rubi
-Version: 1.3.1
+Version: 1.3.2
 Summary: a python SDK for the Rubicon Protocol
 Author: denver
 Author-email: denver@rubicon.finance
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Requires-Dist: attributedict (>=0.3.0,<0.4.0)
-Requires-Dist: eth-abi (>=3.0.1,<4.0.0)
-Requires-Dist: eth-tester (>=0.8.0b1,<0.9.0)
+Requires-Dist: eth-abi (>=4.0.0,<5.0.0)
+Requires-Dist: eth-tester (>=0.9.0b1,<0.10.0)
 Requires-Dist: eth-utils (>=2.1.0,<3.0.0)
 Requires-Dist: hexbytes (>=0.3.0,<0.4.0)
-Requires-Dist: py-evm (>=0.6.1a1,<0.7.0)
-Requires-Dist: pytest (>=7.2.0,<8.0.0)
-Requires-Dist: sphinx (>=5.3.0,<6.0.0) ; extra == "docs"
-Requires-Dist: subgrounds[dash] (>=1.0.3,<2.0.0)
-Requires-Dist: web3 (>=6.0.0b,<7.0.0)
+Requires-Dist: py-evm (>=0.7.0a2,<0.8.0)
+Requires-Dist: pytest (>=7.3.1,<8.0.0)
+Requires-Dist: sphinx (==7.0.1) ; extra == "docs"
+Requires-Dist: subgrounds[dash] (>=1.5.1,<2.0.0)
+Requires-Dist: web3 (>=6.4.0,<7.0.0)
 Description-Content-Type: text/markdown
 
 # rubi
 rubi is a python SDK for the Rubicon Protocol and has a variety of functionality for interacting with the protocol. documentation related to rubi and its functionality can be found [here](https://rubi.readthedocs.io/en/latest/#). 
 
 ### Design Goals
 the underlying goal of the design of rubi is to decrease user friction when interacting with the protocol, and when interacting with the sdk. we want to enable the user
 as much access as possible without requiring any input from the user. for example, by breaking up the contract functionality into read and write classes, we enable the user to
 use the sdk to read from the protocol without passing in any keys. within the data classes, we aim to provide as much information as possible to the user without requiring any 
 additional input such as api keys. when it is clearly useful, we will add higher level classes that provide additional functionality to the user by requiring additional input. 
 
 ### SDK Disclaimer
 
-This codebase is in Alpha and could contain bugs or change significantly between versions. Contributing through Issues or Pull Requests is welcome!
+this codebase is in Alpha and could contain bugs or change significantly between versions. contributing through Issues or Pull Requests is welcome!
 
 ### Protocol Disclaimer
 
-Please refer to [this](https://docs.rubicon.finance/docs/protocol/rubicon-pools/risks) for information on the risks associated to the Rubicon Protocol.
+please refer to [this](https://docs.rubicon.finance/protocol/risks) for information on the risks associated to the Rubicon Protocol.
```

