# Comparing `tmp/betfair_parser-0.2.0.tar.gz` & `tmp/betfair_parser-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betfair_parser-0.2.0.tar", max compression
+gzip compressed data, was "betfair_parser-0.2.1.tar", max compression
```

## Comparing `betfair_parser-0.2.0.tar` & `betfair_parser-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0        0 2023-02-17 06:17:12.705223 betfair_parser-0.2.0/betfair_parser/__init__.py
--rw-r--r--   0        0        0      919 2023-02-24 04:45:44.811742 betfair_parser-0.2.0/betfair_parser/core.py
--rw-r--r--   0        0        0        0 2023-02-17 06:17:12.706435 betfair_parser-0.2.0/betfair_parser/spec/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 01:56:57.283786 betfair_parser-0.2.0/betfair_parser/spec/accounts/__init__.py
--rw-r--r--   0        0        0     2589 2023-05-20 01:56:57.284082 betfair_parser-0.2.0/betfair_parser/spec/accounts/enums.py
--rw-r--r--   0        0        0        0 2023-05-20 01:56:57.284124 betfair_parser-0.2.0/betfair_parser/spec/accounts/exceptions.py
--rw-r--r--   0        0        0     2584 2023-05-20 01:56:57.284257 betfair_parser-0.2.0/betfair_parser/spec/accounts/operations.py
--rw-r--r--   0        0        0    10884 2023-05-20 01:56:57.284389 betfair_parser-0.2.0/betfair_parser/spec/accounts/type_definitions.py
--rw-r--r--   0        0        0        0 2023-05-20 01:56:57.284468 betfair_parser-0.2.0/betfair_parser/spec/betting/__init__.py
--rw-r--r--   0        0        0    20267 2023-05-20 01:56:57.284702 betfair_parser-0.2.0/betfair_parser/spec/betting/enums.py
--rw-r--r--   0        0        0     1811 2023-05-20 01:56:57.284819 betfair_parser-0.2.0/betfair_parser/spec/betting/exceptions.py
--rw-r--r--   0        0        0     9434 2023-05-20 01:56:57.284942 betfair_parser-0.2.0/betfair_parser/spec/betting/listings.py
--rw-r--r--   0        0        0     8003 2023-05-20 01:56:57.285056 betfair_parser-0.2.0/betfair_parser/spec/betting/orders.py
--rw-r--r--   0        0        0    28629 2023-05-20 01:56:57.285245 betfair_parser-0.2.0/betfair_parser/spec/betting/type_definitions.py
--rw-r--r--   0        0        0     5331 2023-05-20 01:56:57.285473 betfair_parser-0.2.0/betfair_parser/spec/common.py
--rw-r--r--   0        0        0      717 2023-05-20 01:56:57.285784 betfair_parser-0.2.0/betfair_parser/spec/constants.py
--rw-r--r--   0        0        0     3569 2023-05-20 01:56:57.285934 betfair_parser-0.2.0/betfair_parser/spec/error.py
--rw-r--r--   0        0        0     1768 2023-05-20 01:56:57.286037 betfair_parser-0.2.0/betfair_parser/spec/heartbeat.py
--rw-r--r--   0        0        0     3399 2023-05-20 01:56:57.286141 betfair_parser-0.2.0/betfair_parser/spec/navigation.py
--rw-r--r--   0        0        0     2903 2023-05-20 01:56:57.286235 betfair_parser-0.2.0/betfair_parser/spec/race_status.py
--rw-r--r--   0        0        0      324 2023-02-17 06:17:12.708820 betfair_parser-0.2.0/betfair_parser/spec/streaming/__init__.py
--rw-r--r--   0        0        0     6274 2023-05-20 01:56:57.286455 betfair_parser-0.2.0/betfair_parser/spec/streaming/mcm.py
--rw-r--r--   0        0        0     2241 2023-05-20 01:56:57.286612 betfair_parser-0.2.0/betfair_parser/spec/streaming/ocm.py
--rw-r--r--   0        0        0     2416 2023-05-20 01:56:57.286756 betfair_parser-0.2.0/betfair_parser/spec/streaming/status.py
--rw-r--r--   0        0        0     2148 2023-05-20 01:56:57.286841 betfair_parser-0.2.0/betfair_parser/strenums.py
--rw-r--r--   0        0        0      645 2023-05-20 01:56:57.287292 betfair_parser-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 betfair_parser-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-02-17 06:17:12.705223 betfair_parser-0.2.1/betfair_parser/__init__.py
+-rw-r--r--   0        0        0      919 2023-02-24 04:45:44.811742 betfair_parser-0.2.1/betfair_parser/core.py
+-rw-r--r--   0        0        0        0 2023-02-17 06:17:12.706435 betfair_parser-0.2.1/betfair_parser/spec/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 01:56:57.283786 betfair_parser-0.2.1/betfair_parser/spec/accounts/__init__.py
+-rw-r--r--   0        0        0     2589 2023-05-20 01:56:57.284082 betfair_parser-0.2.1/betfair_parser/spec/accounts/enums.py
+-rw-r--r--   0        0        0        0 2023-05-20 01:56:57.284124 betfair_parser-0.2.1/betfair_parser/spec/accounts/exceptions.py
+-rw-r--r--   0        0        0     2634 2023-05-20 09:01:10.296344 betfair_parser-0.2.1/betfair_parser/spec/accounts/operations.py
+-rw-r--r--   0        0        0    10884 2023-05-20 01:56:57.284389 betfair_parser-0.2.1/betfair_parser/spec/accounts/type_definitions.py
+-rw-r--r--   0        0        0        0 2023-05-20 01:56:57.284468 betfair_parser-0.2.1/betfair_parser/spec/betting/__init__.py
+-rw-r--r--   0        0        0    20267 2023-05-20 01:56:57.284702 betfair_parser-0.2.1/betfair_parser/spec/betting/enums.py
+-rw-r--r--   0        0        0     1811 2023-05-20 01:56:57.284819 betfair_parser-0.2.1/betfair_parser/spec/betting/exceptions.py
+-rw-r--r--   0        0        0     9622 2023-05-20 09:01:10.296578 betfair_parser-0.2.1/betfair_parser/spec/betting/listings.py
+-rw-r--r--   0        0        0     8145 2023-05-20 09:01:10.296800 betfair_parser-0.2.1/betfair_parser/spec/betting/orders.py
+-rw-r--r--   0        0        0    28632 2023-05-20 09:01:10.297106 betfair_parser-0.2.1/betfair_parser/spec/betting/type_definitions.py
+-rw-r--r--   0        0        0     5374 2023-05-20 09:01:10.297336 betfair_parser-0.2.1/betfair_parser/spec/common.py
+-rw-r--r--   0        0        0      717 2023-05-20 01:56:57.285784 betfair_parser-0.2.1/betfair_parser/spec/constants.py
+-rw-r--r--   0        0        0     3601 2023-05-20 09:01:10.297529 betfair_parser-0.2.1/betfair_parser/spec/error.py
+-rw-r--r--   0        0        0     1768 2023-05-20 01:56:57.286037 betfair_parser-0.2.1/betfair_parser/spec/heartbeat.py
+-rw-r--r--   0        0        0     3399 2023-05-20 01:56:57.286141 betfair_parser-0.2.1/betfair_parser/spec/navigation.py
+-rw-r--r--   0        0        0     2938 2023-05-20 09:01:10.297731 betfair_parser-0.2.1/betfair_parser/spec/race_status.py
+-rw-r--r--   0        0        0      324 2023-02-17 06:17:12.708820 betfair_parser-0.2.1/betfair_parser/spec/streaming/__init__.py
+-rw-r--r--   0        0        0     6274 2023-05-20 01:56:57.286455 betfair_parser-0.2.1/betfair_parser/spec/streaming/mcm.py
+-rw-r--r--   0        0        0     2241 2023-05-20 01:56:57.286612 betfair_parser-0.2.1/betfair_parser/spec/streaming/ocm.py
+-rw-r--r--   0        0        0     2416 2023-05-20 01:56:57.286756 betfair_parser-0.2.1/betfair_parser/spec/streaming/status.py
+-rw-r--r--   0        0        0     2148 2023-05-20 01:56:57.286841 betfair_parser-0.2.1/betfair_parser/strenums.py
+-rw-r--r--   0        0        0      645 2023-05-20 09:01:10.297915 betfair_parser-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 betfair_parser-0.2.1/PKG-INFO
```

### Comparing `betfair_parser-0.2.0/betfair_parser/core.py` & `betfair_parser-0.2.1/betfair_parser/core.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.0/betfair_parser/spec/accounts/enums.py` & `betfair_parser-0.2.1/betfair_parser/spec/accounts/enums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.0/betfair_parser/spec/accounts/operations.py` & `betfair_parser-0.2.1/betfair_parser/spec/accounts/operations.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 from betfair_parser.spec.accounts.enums import IncludeItem, Wallet
 from betfair_parser.spec.accounts.type_definitions import (
     AccountDetailsResponse,
     AccountFundsResponse,
     AccountStatementReport,
     CurrencyRate,
 )
@@ -21,36 +23,36 @@
 
     method = "AccountAPING/v1.0/getAccountDetails"
     params: dict = {}
     return_type = Response[AccountDetailsResponse]
 
 
 class getAccountStatementParams(BaseMessage, frozen=True):
-    locale: str | None = None  # The language to be used where applicable. Defaults to account settings
-    fromRecord: int | None = None  # Specifies the first record that will be returned, defaults to 0
-    recordCount: int | None = None  # Specifies the maximum number of records to be returned. Maximum 100
+    locale: Optional[str] = None  # The language to be used where applicable. Defaults to account settings
+    fromRecord: Optional[int] = None  # Specifies the first record that will be returned, defaults to 0
+    recordCount: Optional[int] = None  # Specifies the maximum number of records to be returned. Maximum 100
 
     # Return items with an itemDate within this date range. Both from and to date times are inclusive.
     # If from is not specified then the oldest available items will be in range. If to is not specified
     # then the latest items will be in range. nb. This itemDataRange is currently only applied when
     # includeItem is set to ALL or not specified, else items are NOT bound by itemDate.
     # Please note:  You can only retrieve account statement items for the last 90 days.
-    itemDateRange: TimeRange | None = None
-    includeItem: IncludeItem | None = None  # Which items to include, if not specified then defaults to ALL.
-    wallet: Wallet | None = None  # Which wallet to return statementItems for. Defaults to UK
+    itemDateRange: Optional[TimeRange] = None
+    includeItem: Optional[IncludeItem] = None  # Which items to include, if not specified then defaults to ALL.
+    wallet: Optional[Wallet] = None  # Which wallet to return statementItems for. Defaults to UK
 
 
 class getAccountStatement(Request, kw_only=True, frozen=True):
     method = "AccountAPING/v1.0/getAccountStatement"
     params: getAccountStatementParams
     return_type = AccountStatementReport
 
 
 class listCurrencyRatesParams(BaseMessage, frozen=True):
-    fromCurrency: str | None = None  # The currency from which the rates are computed. Only GBP for now.
+    fromCurrency: Optional[str] = None  # The currency from which the rates are computed. Only GBP for now.
 
 
 class listCurrencyRates(Request, kw_only=True, frozen=True):
     """Returns a list of currency rates based on given currency. Updates only once per hour."""
 
     method = "AccountAPING/v1.0/listCurrencyRates"
     return_type = list[CurrencyRate]
```

### Comparing `betfair_parser-0.2.0/betfair_parser/spec/accounts/type_definitions.py` & `betfair_parser-0.2.1/betfair_parser/spec/accounts/type_definitions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.0/betfair_parser/spec/betting/enums.py` & `betfair_parser-0.2.1/betfair_parser/spec/betting/enums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.0/betfair_parser/spec/betting/exceptions.py` & `betfair_parser-0.2.1/betfair_parser/spec/betting/exceptions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.0/betfair_parser/spec/betting/listings.py` & `betfair_parser-0.2.1/betfair_parser/spec/betting/listings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 from betfair_parser.spec.betting.enums import (
     MarketProjection,
     MarketSort,
     MatchProjection,
     OrderProjection,
     TimeGranularity,
 )
@@ -20,15 +22,15 @@
     VenueResult,
 )
 from betfair_parser.spec.common import BaseMessage, BetId, Date, MarketId, Request, Response, SelectionId
 
 
 class ListingParams(BaseMessage, frozen=True):
     filter: MarketFilter
-    locale: str | None = None
+    locale: Optional[str] = None
 
 
 class listCompetitions(Request, kw_only=True, frozen=True):
     """
     Returns a list of Competitions (i.e., World Cup 2013) associated with the markets selected by
     the MarketFilter. Currently only Football markets have an associated competition.
     """
@@ -93,24 +95,30 @@
 
 
 # More complex listings
 
 
 class listMarketBookParams(BaseMessage, frozen=True):
     marketIds: list[str]  # One or more market ids
-    priceProjection: PriceProjection | None = None  # The projection of price data you want to receive in the response
-    orderProjection: OrderProjection | None = None  # The orders you want to receive in the response
-    matchProjection: MatchProjection | None = None  # If you ask for orders, specifies the representation of matches
-    includeOverallPosition: bool | None = None  # If you ask for orders, returns matches for each selection
-    partitionMatchedByStrategyRef: bool | None = None  # Returns the breakdown of matches by strategy for each selection
-    customerStrategyRefs: set[str] | None = None
-    currencyCode: str | None = None  # A Betfair standard currency code
-    locale: str | None = None  # The language used for the response
-    matchedSince: Date | None = None  # Restricts to orders with at least one fragment matched since the specified date
-    betIds: set[BetId] | None = None  # Restricts to orders with the specified bet IDs
+    priceProjection: Optional[
+        PriceProjection
+    ] = None  # The projection of price data you want to receive in the response
+    orderProjection: Optional[OrderProjection] = None  # The orders you want to receive in the response
+    matchProjection: Optional[MatchProjection] = None  # If you ask for orders, specifies the representation of matches
+    includeOverallPosition: Optional[bool] = None  # If you ask for orders, returns matches for each selection
+    partitionMatchedByStrategyRef: Optional[
+        bool
+    ] = None  # Returns the breakdown of matches by strategy for each selection
+    customerStrategyRefs: Optional[set[str]] = None
+    currencyCode: Optional[str] = None  # A Betfair standard currency code
+    locale: Optional[str] = None  # The language used for the response
+    matchedSince: Optional[
+        Date
+    ] = None  # Restricts to orders with at least one fragment matched since the specified date
+    betIds: Optional[set[BetId]] = None  # Restricts to orders with the specified bet IDs
 
 
 class listMarketBook(Request, kw_only=True, frozen=True):
     """
     Returns a list of dynamic data about markets. Dynamic data includes prices, the status of the
     market, the status of selections, the traded volume, and the status of any orders you have
     placed in the market.
@@ -132,18 +140,18 @@
     method = "SportsAPING/v1.0/listMarketBook"
     params: listMarketBookParams
     return_type = Response[list[MarketBook]]
 
 
 class listMarketCatalogueParams(BaseMessage, kw_only=True, frozen=True):
     filter: MarketFilter  # The filter to select desired markets
-    marketProjection: set[MarketProjection] | None = None  # The type and amount of data returned about the market
-    sort: MarketSort | None = None  # The order of the results, defaults to RANK
+    marketProjection: Optional[set[MarketProjection]] = None  # The type and amount of data returned about the market
+    sort: Optional[MarketSort] = None  # The order of the results, defaults to RANK
     maxResults: int  # Limit on the total number of results returned
-    locale: str | None = None  # The language used for the response
+    locale: Optional[str] = None  # The language used for the response
 
 
 class listMarketCatalogue(Request, kw_only=True, frozen=True):
     """
     Returns a list of information about published (ACTIVE/SUSPENDED) markets that does not change
     (or changes very rarely). You use listMarketCatalogue to retrieve the name of the market, the
     names of selections and other information about markets.  Market Data Request Limits apply to
@@ -171,25 +179,31 @@
     params: listMarketProfitAndLossParams
     return_type = Response[list[MarketProfitAndLoss]]
 
 
 class listRunnerBookParams(BaseMessage, frozen=True):
     marketId: MarketId  # The unique id for the market
     selectionId: SelectionId  # The unique id for the selection in the market
-    handicap: float | None = None  # The handicap associated with the runner in case of Asian handicap market
-    priceProjection: PriceProjection | None = None  # The projection of price data you want to receive in the response
-    orderProjection: OrderProjection | None = None  # The orders you want to receive in the response
-    matchProjection: MatchProjection | None = None  # If you ask for orders, specifies the representation of matches
-    includeOverallPosition: bool | None = None  # If you ask for orders, returns matches for each selection
-    partitionMatchedByStrategyRef: bool | None = None  # Returns the breakdown of matches by strategy for each selection
-    customerStrategyRefs: set[str] | None = None
-    currencyCode: str | None = None  # A Betfair standard currency code
-    locale: str | None = None  # The language used for the response
-    matchedSince: Date | None = None  # Restricts to orders with at least one fragment matched since the specified date
-    betIds: set[BetId] | None = None  # Restricts to orders with the specified bet IDs
+    handicap: Optional[float] = None  # The handicap associated with the runner in case of Asian handicap market
+    priceProjection: Optional[
+        PriceProjection
+    ] = None  # The projection of price data you want to receive in the response
+    orderProjection: Optional[OrderProjection] = None  # The orders you want to receive in the response
+    matchProjection: Optional[MatchProjection] = None  # If you ask for orders, specifies the representation of matches
+    includeOverallPosition: Optional[bool] = None  # If you ask for orders, returns matches for each selection
+    partitionMatchedByStrategyRef: Optional[
+        bool
+    ] = None  # Returns the breakdown of matches by strategy for each selection
+    customerStrategyRefs: Optional[set[str]] = None
+    currencyCode: Optional[str] = None  # A Betfair standard currency code
+    locale: Optional[str] = None  # The language used for the response
+    matchedSince: Optional[
+        Date
+    ] = None  # Restricts to orders with at least one fragment matched since the specified date
+    betIds: Optional[set[BetId]] = None  # Restricts to orders with the specified bet IDs
 
 
 class listRunnerBook(Request, kw_only=True, frozen=True):
     """
     Returns a list of dynamic data about a market and a specified runner. Dynamic data includes
     prices, the status of the market, the status of selections, the traded volume, and the status
     of any orders you have placed in the market..
```

### Comparing `betfair_parser-0.2.0/betfair_parser/spec/betting/orders.py` & `betfair_parser-0.2.1/betfair_parser/spec/betting/orders.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 import msgspec
 
 from betfair_parser.spec.betting.enums import BetStatus, GroupBy, OrderBy, OrderProjection, Side, SortDir
 from betfair_parser.spec.betting.type_definitions import (
     CancelExecutionReport,
     CancelInstruction,
     ClearedOrderSummaryReport,
@@ -27,17 +29,17 @@
     TimeRange,
 )
 
 
 class placeOrdersParams(BaseMessage, frozen=True):
     marketId: str
     instructions: list[PlaceInstruction]
-    customerRef: CustomerRef | None = None
-    marketVersion: MarketVersion | None = None
-    customerStrategyRef: CustomerStrategyRef | None = None
+    customerRef: Optional[CustomerRef] = None
+    marketVersion: Optional[MarketVersion] = None
+    customerStrategyRef: Optional[CustomerStrategyRef] = None
     async_: bool = msgspec.field(name="async", default=False)
 
 
 class placeOrders(Request, kw_only=True, frozen=True):
     """Place new orders into market.
 
     Please note that additional bet sizing rules apply to bets placed into the Italian Exchange.
@@ -50,17 +52,17 @@
 
     method = "SportsAPING/v1.0/placeOrders"
     params: placeOrdersParams
     return_type = Response[PlaceExecutionReport]
 
 
 class cancelOrdersParams(BaseMessage, frozen=True):
-    marketId: str | None = None
-    instructions: list[CancelInstruction] | None = None
-    customerRef: CustomerRef | None = None
+    marketId: Optional[str] = None
+    instructions: Optional[list[CancelInstruction]] = None
+    customerRef: Optional[CustomerRef] = None
 
 
 class cancelOrders(Request, kw_only=True, frozen=True):
     """
     Cancel all bets OR cancel all bets on a market OR fully or partially cancel particular
     orders on a market. Only LIMIT orders can be cancelled or partially cancelled once placed.
     """
@@ -69,16 +71,16 @@
     params: cancelOrdersParams
     return_type = Response[CancelExecutionReport]
 
 
 class replaceOrdersParams(BaseMessage, frozen=True):
     marketId: str
     instructions: list[ReplaceInstruction]
-    customerRef: CustomerRef | None = None
-    marketVersion: MarketVersion | None = None
+    customerRef: Optional[CustomerRef] = None
+    marketVersion: Optional[MarketVersion] = None
     async_: bool = msgspec.field(name="async", default=False)
 
 
 class replaceOrders(Request, kw_only=True, frozen=True):
     """
     This operation is logically a bulk cancel followed by a bulk place. The cancel is completed
     first then the new orders are placed. The new orders will be placed atomically in that they
@@ -89,37 +91,39 @@
     method = "SportsAPING/v1.0/replaceOrders"
     params: replaceOrdersParams
     return_type = Response[ReplaceExecutionReport]
 
 
 class listClearedOrdersParams(BaseMessage, frozen=True):
     betStatus: BetStatus  # Restricts the results to the specified status.
-    eventTypeIds: set[EventTypeId] | None = None  # Restricts the results to the specified Event Type IDs.
-    eventIds: set[EventId] | None = None  # Restricts the results to the specified Event IDs.
-    marketIds: set[MarketId] | None = None  # Restricts the results to the specified market IDs.
-    runnerIds: set[RunnerId] | None = None  # Restricts the results to the specified Runners.
-    betIds: set[BetId] | None = None  # Restricts the results to the specified bet IDs, maximum 1000 betId per request
-    customerOrderRefs: set[CustomerOrderRef] | None = None
-    customerStrategyRefs: set[CustomerStrategyRef] | None = None
-    side: Side | None = None  # Restricts the results to the specified side.
+    eventTypeIds: Optional[set[EventTypeId]] = None  # Restricts the results to the specified Event Type IDs.
+    eventIds: Optional[set[EventId]] = None  # Restricts the results to the specified Event IDs.
+    marketIds: Optional[set[MarketId]] = None  # Restricts the results to the specified market IDs.
+    runnerIds: Optional[set[RunnerId]] = None  # Restricts the results to the specified Runners.
+    betIds: Optional[
+        set[BetId]
+    ] = None  # Restricts the results to the specified bet IDs, maximum 1000 betId per request
+    customerOrderRefs: Optional[set[CustomerOrderRef]] = None
+    customerStrategyRefs: Optional[set[CustomerStrategyRef]] = None
+    side: Optional[Side] = None  # Restricts the results to the specified side.
 
     # Optionally restricts the results to be from/to the specified settled date. This date is inclusive,
     # i.e. if an order was cleared on exactly this date (to the millisecond) then it will be included
     # in the results. If the from is later than the to, no results will be returned.
     # Please Note: if you have a longer running market that is settled at multiple different times
     # then there is no way to get the returned market rollup to only include bets settled in a certain
     # date range, it will always return the overall position from the market including all settlements.
-    settledDateRange: TimeRange | None = None
+    settledDateRange: Optional[TimeRange] = None
 
     # If not supplied then the lowest level is returned, i.e. bet by bet This is only applicable to SETTLED BetStatus.
-    groupBy: GroupBy | None = None
-    includeItemDescription: bool | None = None
-    locale: str | None = None  # The language used for the itemDescription, defaults to account settings
-    fromRecord: int | None = None  # Specifies the first record that will be returned. Records start at index zero.
-    recordCount: int | None = None  # Number of records from the index position 'fromRecord', maximum 1000
+    groupBy: Optional[GroupBy] = None
+    includeItemDescription: Optional[bool] = None
+    locale: Optional[str] = None  # The language used for the itemDescription, defaults to account settings
+    fromRecord: Optional[int] = None  # Specifies the first record that will be returned. Records start at index zero.
+    recordCount: Optional[int] = None  # Number of records from the index position 'fromRecord', maximum 1000
 
 
 class listClearedOrders(Request, kw_only=True, frozen=True):
     """
     Returns a list of settled bets based on the bet status, ordered by settled date. To retrieve
     more than 1000 records, you need to make use of the fromRecord and recordCount parameters.
 
@@ -138,25 +142,25 @@
 
 
 class listCurrentOrdersParams(BaseMessage, frozen=True):
     """
     Parameters for retrieving a list of current orders.
     """
 
-    betIds: set[BetId] | None = None  # Restricts the results to the specified bet IDs
-    marketIds: set[str] | None = None  # Restricts the results to the specified market IDs
-    orderProjection: OrderProjection | None = None  # Restricts the results to the specified order status
-    customerOrderRefs: set[CustomerOrderRef] | None = None
-    customerStrategyRefs: set[CustomerStrategyRef] | None = None
-    dateRange: TimeRange | None = None  # Restricts the results to be from/to the specified date
-    orderBy: OrderBy | None = None  # Specifies how the results will be ordered
-    sortDir: SortDir | None = None  # Specifies the direction the results will be sorted in
-    fromRecord: int | None = None  # Specifies the first record that will be returned
-    recordCount: int | None = None  # Specifies how many records will be returned
-    includeItemDescription: bool | None = None
+    betIds: Optional[set[BetId]] = None  # Restricts the results to the specified bet IDs
+    marketIds: Optional[set[str]] = None  # Restricts the results to the specified market IDs
+    orderProjection: Optional[OrderProjection] = None  # Restricts the results to the specified order status
+    customerOrderRefs: Optional[set[CustomerOrderRef]] = None
+    customerStrategyRefs: Optional[set[CustomerStrategyRef]] = None
+    dateRange: Optional[TimeRange] = None  # Restricts the results to be from/to the specified date
+    orderBy: Optional[OrderBy] = None  # Specifies how the results will be ordered
+    sortDir: Optional[SortDir] = None  # Specifies the direction the results will be sorted in
+    fromRecord: Optional[int] = None  # Specifies the first record that will be returned
+    recordCount: Optional[int] = None  # Specifies how many records will be returned
+    includeItemDescription: Optional[bool] = None
 
 
 class listCurrentOrders(Request, kw_only=True, frozen=True):
     """
     Returns a list of your current orders. Optionally you can filter and sort your current orders
     using the various parameters, setting none of the parameters will return all of your current
     orders up to a maximum of 1000 bets, ordered BY_BET and sorted EARLIEST_TO_LATEST. To retrieve
```

### Comparing `betfair_parser-0.2.0/betfair_parser/spec/betting/type_definitions.py` & `betfair_parser-0.2.1/betfair_parser/spec/betting/type_definitions.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,15 @@
     selectionId: int  # The unique id for the selection
     runnerName: str  # The name of the runner
 
     # The handicap applies to market with the MarketBettingType ASIAN_HANDICAP_SINGLE_LINE
     # & ASIAN_HANDICAP_DOUBLE_LINE only
     handicap: float
     sortPriority: Optional[int] = None  # This is marked as REQUIRED in the API doc, but omitted sometimes
-    metadata: Optional[dict[str, str | None]] = None  # Metadata associated with the runner
+    metadata: Optional[dict[str, Optional[str]]] = None  # Metadata associated with the runner
 
     @property
     def runner_name(self):
         # TODO: This should be gone, as soon all fields are renamed
         return self.runnerName
 
     @property
```

### Comparing `betfair_parser-0.2.0/betfair_parser/spec/common.py` & `betfair_parser-0.2.1/betfair_parser/spec/common.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import datetime
-from typing import Annotated, Generic, Literal, Optional, TypeVar
+from typing import Annotated, Generic, Literal, Optional, TypeVar, Union
 
 import msgspec
 
 from betfair_parser.strenums import DocumentedEnum, StrEnum, auto, doc
 
 
 class IntStr(int):
@@ -70,15 +70,15 @@
     jsonrpc: Literal["2.0"] = "2.0"
     id: int = 1
     result: ResultType = None
 
 
 class Request(BaseMessage, kw_only=True, frozen=True):
     method: str
-    params: BaseMessage | dict
+    params: Union[BaseMessage, dict]
     jsonrpc: Literal["2.0"] = "2.0"
     id: int = 1
     response_type = None  # not to be serialized, so no type definition
     throws = None  # not to be serialized, so no type definition
 
 
 # Type aliases with minimalistic validation
@@ -92,19 +92,19 @@
 EventId = Annotated[str, msgspec.Meta(title="EventId")]
 EventTypeId = Annotated[IntStr, msgspec.Meta(title="EventTypeId")]
 CountryCode = Annotated[str, msgspec.Meta(title="CountryCode", min_length=2, max_length=3)]
 ExchangeId = Annotated[str, msgspec.Meta(title="ExchangeId")]
 CompetitionId = Annotated[str, msgspec.Meta(title="CompetitionId")]
 Price = Annotated[FloatStr, msgspec.Meta(title="Price")]
 Size = Annotated[FloatStr, msgspec.Meta(title="Size")]
-BetId = Annotated[str | int, msgspec.Meta(title="BetId")]
-MatchId = Annotated[str | int, msgspec.Meta(title="MatchId")]
-CustomerRef = Annotated[str | int, msgspec.Meta(title="CustomerRef")]
-CustomerOrderRef = Annotated[str | int, msgspec.Meta(title="CustomerOrderRef")]
-CustomerStrategyRef = Annotated[str | int, msgspec.Meta(title="CustomerStrategyRef")]
+BetId = Annotated[Union[str, int], msgspec.Meta(title="BetId")]
+MatchId = Annotated[Union[str, int], msgspec.Meta(title="MatchId")]
+CustomerRef = Annotated[Union[str, int], msgspec.Meta(title="CustomerRef")]
+CustomerOrderRef = Annotated[Union[str, int], msgspec.Meta(title="CustomerOrderRef")]
+CustomerStrategyRef = Annotated[Union[str, int], msgspec.Meta(title="CustomerStrategyRef")]
 
 
 # Enums and type definitions, that are used in multiple parts of the API
 
 
 class OrderType(DocumentedEnum):
     LIMIT = doc("A normal exchange limit order for immediate execution")
```

### Comparing `betfair_parser-0.2.0/betfair_parser/spec/constants.py` & `betfair_parser-0.2.1/betfair_parser/spec/constants.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.0/betfair_parser/spec/error.py` & `betfair_parser-0.2.1/betfair_parser/spec/error.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from typing import Union
+
 from betfair_parser.spec.common import BaseMessage
 from betfair_parser.strenums import DocumentedEnum, doc
 
 
 class Error(BaseMessage, frozen=True):
-    code: int | str
+    code: Union[int, str]
     message: str
 
 
 class ErrorResponse(BaseMessage, frozen=True):
     error: Error
```

### Comparing `betfair_parser-0.2.0/betfair_parser/spec/heartbeat.py` & `betfair_parser-0.2.1/betfair_parser/spec/heartbeat.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.0/betfair_parser/spec/navigation.py` & `betfair_parser-0.2.1/betfair_parser/spec/navigation.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.0/betfair_parser/spec/race_status.py` & `betfair_parser-0.2.1/betfair_parser/spec/race_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 from betfair_parser.spec.common import BaseMessage, Date, Request, Response
 from betfair_parser.strenums import DocumentedEnum, doc
 
 
 class RaceStatus(DocumentedEnum):
     DORMANT = doc("There is no data available for this race.")
     DELAYED = doc("The start of the race has been delayed")
@@ -43,15 +45,15 @@
     raceStatus: RaceStatus  # The current status of the race.
     lastUpdated: Date  # This is the time the data was last updated
     sequence: int  # This is the unique identifier associated to each update of the data
     responseCode: ResponseCode
 
 
 class listRaceDetailsParams(BaseMessage, frozen=True):
-    meetingIds: set[str] | None = None  # Restricts the results to the specified meeting IDs.
-    raceIds: set[str] | None = None  # Restricts the results to the specified race IDs.
+    meetingIds: Optional[set[str]] = None  # Restricts the results to the specified meeting IDs.
+    raceIds: Optional[set[str]] = None  # Restricts the results to the specified race IDs.
 
 
 class listRaceDetail(Request, frozen=True):
     method = "ScoresAPING/v1.0/listRaceDetails"
     params: listRaceDetailsParams
     return_type = Response[list[RaceDetails]]
```

### Comparing `betfair_parser-0.2.0/betfair_parser/spec/streaming/mcm.py` & `betfair_parser-0.2.1/betfair_parser/spec/streaming/mcm.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.0/betfair_parser/spec/streaming/ocm.py` & `betfair_parser-0.2.1/betfair_parser/spec/streaming/ocm.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.0/betfair_parser/spec/streaming/status.py` & `betfair_parser-0.2.1/betfair_parser/spec/streaming/status.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.0/betfair_parser/strenums.py` & `betfair_parser-0.2.1/betfair_parser/strenums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.2.0/pyproject.toml` & `betfair_parser-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "betfair_parser"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["Bradley McElroy <bradley.mcelroy@live.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 msgspec = "^0.15.1"
 fsspec = ">=2022"
```

