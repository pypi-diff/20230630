# Comparing `tmp/crypto-screening-1.5.0.tar.gz` & `tmp/crypto-screening-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-1.5.0.tar", last modified: Thu Jun 29 13:13:03 2023, max compression
+gzip compressed data, was "crypto-screening-1.6.0.tar", last modified: Fri Jun 30 09:57:45 2023, max compression
```

## Comparing `crypto-screening-1.5.0.tar` & `crypto-screening-1.6.0.tar`

### file list

```diff
@@ -1,35 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 13:13:03.251758 crypto-screening-1.5.0/
--rw-rw-rw-   0        0        0       98 2023-06-29 13:13:02.000000 crypto-screening-1.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2085 2023-06-29 13:13:03.251758 crypto-screening-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1264 2023-06-23 16:52:27.000000 crypto-screening-1.5.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.5.0/build.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:13:03.207789 crypto-screening-1.5.0/crypto_screening/
--rw-rw-rw-   0        0        0     6694 2023-06-23 16:52:27.000000 crypto-screening-1.5.0/crypto_screening/base.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:13:03.250759 crypto-screening-1.5.0/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17713 2023-06-28 11:01:21.000000 crypto-screening-1.5.0/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0      496 2023-06-27 10:17:11.000000 crypto-screening-1.5.0/crypto_screening/collect/document.py
--rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-1.5.0/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0     9680 2023-06-28 12:47:21.000000 crypto-screening-1.5.0/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    19287 2023-06-28 10:54:03.000000 crypto-screening-1.5.0/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    12548 2023-06-29 10:13:27.000000 crypto-screening-1.5.0/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      869 2023-06-27 10:20:56.000000 crypto-screening-1.5.0/crypto_screening/document.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.5.0/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0      180 2023-06-23 16:52:27.000000 crypto-screening-1.5.0/crypto_screening/hints.py
--rw-rw-rw-   0        0        0     2665 2023-06-23 16:52:27.000000 crypto-screening-1.5.0/crypto_screening/interval.py
--rw-rw-rw-   0        0        0    32948 2023-06-29 10:37:44.000000 crypto-screening-1.5.0/crypto_screening/ohlcv.py
--rw-rw-rw-   0        0        0    24970 2023-06-29 13:10:14.000000 crypto-screening-1.5.0/crypto_screening/orderbook.py
--rw-rw-rw-   0        0        0     2378 2023-06-27 10:23:45.000000 crypto-screening-1.5.0/crypto_screening/process.py
--rw-rw-rw-   0        0        0    34609 2023-06-29 13:12:38.000000 crypto-screening-1.5.0/crypto_screening/screener.py
--rw-rw-rw-   0        0        0     9894 2023-06-25 16:31:01.000000 crypto-screening-1.5.0/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-1.5.0/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:13:03.222789 crypto-screening-1.5.0/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2085 2023-06-29 13:13:03.000000 crypto-screening-1.5.0/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      812 2023-06-29 13:13:03.000000 crypto-screening-1.5.0/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 13:13:03.000000 crypto-screening-1.5.0/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-06-29 13:13:03.000000 crypto-screening-1.5.0/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-29 13:13:03.000000 crypto-screening-1.5.0/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-06-29 13:13:02.000000 crypto-screening-1.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       99 2023-06-28 09:56:21.000000 crypto-screening-1.5.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.5.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 13:13:03.251758 crypto-screening-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-06-29 12:20:25.000000 crypto-screening-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:57:45.901259 crypto-screening-1.6.0/
+-rw-rw-rw-   0        0        0       98 2023-06-30 09:57:45.000000 crypto-screening-1.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2085 2023-06-30 09:57:45.901259 crypto-screening-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1264 2023-06-23 16:52:27.000000 crypto-screening-1.6.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.6.0/build.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:57:45.886754 crypto-screening-1.6.0/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-06-30 09:57:45.893751 crypto-screening-1.6.0/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17713 2023-06-28 11:01:21.000000 crypto-screening-1.6.0/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-1.6.0/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0    10359 2023-06-30 09:27:48.000000 crypto-screening-1.6.0/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    19287 2023-06-28 10:54:03.000000 crypto-screening-1.6.0/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-1.6.0/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.6.0/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     2665 2023-06-23 16:52:27.000000 crypto-screening-1.6.0/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:57:45.894751 crypto-screening-1.6.0/crypto_screening/market/
+drwxrwxrwx   0        0        0        0 2023-06-30 09:57:45.896751 crypto-screening-1.6.0/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10832 2023-06-30 09:27:04.000000 crypto-screening-1.6.0/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      889 2023-06-30 09:21:25.000000 crypto-screening-1.6.0/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     8839 2023-06-30 09:21:46.000000 crypto-screening-1.6.0/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:57:45.900259 crypto-screening-1.6.0/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      179 2023-06-30 09:14:39.000000 crypto-screening-1.6.0/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    18775 2023-06-30 09:22:16.000000 crypto-screening-1.6.0/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0    32700 2023-06-30 09:23:12.000000 crypto-screening-1.6.0/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    24937 2023-06-30 09:23:33.000000 crypto-screening-1.6.0/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-1.6.0/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2378 2023-06-27 10:23:45.000000 crypto-screening-1.6.0/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9894 2023-06-25 16:31:01.000000 crypto-screening-1.6.0/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-1.6.0/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:57:45.890743 crypto-screening-1.6.0/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2085 2023-06-30 09:57:45.000000 crypto-screening-1.6.0/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      960 2023-06-30 09:57:45.000000 crypto-screening-1.6.0/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 09:57:45.000000 crypto-screening-1.6.0/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-06-30 09:57:45.000000 crypto-screening-1.6.0/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-30 09:57:45.000000 crypto-screening-1.6.0/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-06-30 09:41:35.000000 crypto-screening-1.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0       99 2023-06-28 09:56:21.000000 crypto-screening-1.6.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.6.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 09:57:45.901259 crypto-screening-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-06-30 09:41:28.000000 crypto-screening-1.6.0/setup.py
```

### Comparing `crypto-screening-1.5.0/PKG-INFO` & `crypto-screening-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.5.0
+Version: 1.6.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.5.0/README.md` & `crypto-screening-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.5.0/build.py` & `crypto-screening-1.6.0/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.5.0/crypto_screening/collect/assets.py` & `crypto-screening-1.6.0/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.5.0/crypto_screening/collect/exchanges.py` & `crypto-screening-1.6.0/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.5.0/crypto_screening/collect/screeners.py` & `crypto-screening-1.6.0/crypto_screening/collect/screeners.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,31 @@
     List, Union, Tuple
 )
 
 from crypto_screening.symbols import symbol_to_pair
 from crypto_screening.collect.symbols import (
     matching_symbol_pair, MarketSymbolSignature
 )
-from crypto_screening.screener import BaseScreener, BaseMultiScreener
+from crypto_screening.market.screeners.base import (
+    BaseScreener, BaseMultiScreener
+)
 
 __all__ = [
     "matching_screener_signatures",
     "matching_screener_pair",
     "matching_screener_pairs",
     "MarketScreenerSignature",
     "find_screeners",
     "structure_screeners",
     "live_screeners",
     "remove_empty_screeners",
     "screeners_exchanges_symbols",
     "structure_exchanges_symbols_screeners",
-    "structure_exchanges_symbols_screener"
+    "structure_exchanges_symbols_screener",
+    "gather_screeners"
 ]
 
 AssetMatches = Iterable[Iterable[str]]
 
 def matching_screener_pair(
         screener1: BaseScreener,
         screener2: BaseScreener, /, *,
@@ -334,8 +337,33 @@
             structure.
             setdefault(screener.exchange, {}).
             setdefault(screener.symbol, screener)
         )
     # end for
 
     return structure
-# end structure_exchanges_symbols_screener
+# end structure_exchanges_symbols_screener
+
+def gather_screeners(
+        screeners: Iterable[Union[BaseScreener, BaseMultiScreener]]
+) -> List[BaseScreener]:
+    """
+    Gathers the base screeners.
+
+    :param screeners: The screeners to process.
+
+    :return: The gathered base screeners.
+    """
+
+    checked_screeners = []
+
+    for screener in screeners:
+        if isinstance(screener, BaseScreener):
+            checked_screeners.append(screener)
+
+        elif isinstance(screener, BaseMultiScreener):
+            checked_screeners.extend(screener.screeners)
+        # end if
+    # end for
+
+    return checked_screeners
+# end gather_screeners
```

### Comparing `crypto-screening-1.5.0/crypto_screening/collect/symbols.py` & `crypto-screening-1.6.0/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.5.0/crypto_screening/dataset.py` & `crypto-screening-1.6.0/crypto_screening/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 from typing import (
     Union, Optional, Tuple, Iterable,
     Any, Callable, Dict
 )
 
 import pandas as pd
 
-from crypto_screening.hints import Number
-
 __all__ = [
     "row_to_dataset",
     "save_dataset",
     "load_dataset",
     "update_dataset",
     "split_dataset",
     "strip_dataset",
@@ -130,15 +128,15 @@
             base[column] = new[column]
         # end if
     # end for
 # end update_dataset
 
 def split_dataset(
         dataset: Union[pd.DataFrame, pd.Series],
-        size: Optional[Number] = None,
+        size: Optional[Union[int, float]] = None,
         length: Optional[int] = None
 ) -> Tuple[pd.DataFrame, pd.DataFrame]:
     """
     Splits the new_dataset into to parts at the point of the given size.
 
     :param dataset: The new_dataset to split.
     :param size: The size of the first part.
```

### Comparing `crypto-screening-1.5.0/crypto_screening/interval.py` & `crypto-screening-1.6.0/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.5.0/crypto_screening/ohlcv.py` & `crypto-screening-1.6.0/crypto_screening/market/screeners/ohlcv.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,21 @@
 import ccxt.pro as ccxtpro
 import ccxt.async_support as async_ccxt
 
 from represent import Modifiers
 
 from multithreading import Caller, multi_threaded_call
 
-from crypto_screening.hints import Number
 from crypto_screening.dataset import (
     OPEN, HIGH, LOW, CLOSE, VOLUME, BIDS, ASKS,
     DATE_TIME, OHLCV_COLUMNS, ASKS_VOLUME, BIDS_VOLUME
 )
 from crypto_screening.interval import interval_to_total_time
-from crypto_screening.screener import (
-    wait_for_update, BaseMultiScreener, structure_screener_datasets,
+from crypto_screening.market.screeners import (
+    BaseMultiScreener, structure_screener_datasets,
     BaseScreener, MarketRecorder, create_market_dataframe
 )
 
 __all__ = [
     "OHLCVScreener",
     "MarketOHLCVScreener",
     "market_ohlcv_recorder",
@@ -121,29 +120,28 @@
 
     - options:
         The ccxt options for the backend screening process.
 
     - cencel:
         The time to cancel screening process after no new data is fetched.
 
-    >>> from crypto_screening.ohlcv import OHLCVScreener
-    >>> from crypto_screening.screener import wait_for_initialization
+    >>> from crypto_screening.market.screeners import OHLCVScreener
     >>>
-    >>> dataset = OHLCVScreener(
+    >>> screener = OHLCVScreener(
     >>>     symbol="BTC/USD", exchange="binance"
     >>> )
     >>>
-    >>> dataset.run(wait=True)
+    >>> screener.run(wait=True)
     >>>
-    >>> print(dataset.market.iloc[-1].splitlines()[0])
+    >>> print(screener.market.iloc[-1].splitlines()[0])
     >>>
     >>> while True:
-    >>>     print(dataset.market.iloc[-1].splitlines()[-1])
+    >>>     screener.wait_for_update()
     >>>
-    >>>     wait_for_update(dataset)
+    >>>     print(screener.market.iloc[-1].splitlines()[-1])
     """
 
     modifiers = Modifiers(**BaseScreener.modifiers)
     modifiers.excluded.append('task')
 
     __slots__ = "interval", "pro", "market", "options", "task"
 
@@ -164,18 +162,18 @@
             self,
             symbol: str,
             exchange: str,
             interval: Optional[str] = None,
             pro: Optional[bool] = True,
             data: Optional[pd.DataFrame] = None,
             length: Optional[Union[bool, int]] = None,
-            delay: Optional[Union[Number, dt.timedelta]] = None,
+            delay: Optional[Union[float, dt.timedelta]] = None,
             location: Optional[str] = None,
             options: Optional[Dict[str, Any]] = None,
-            cancel: Optional[Union[Number, dt.timedelta]] = None
+            cancel: Optional[Union[float, dt.timedelta]] = None
     ) -> None:
         """
         Defines the class attributes.
 
         :param symbol: The symbol of the asset.
         :param exchange: The exchange to get source data from.
         :param interval: The interval for the data.
@@ -354,15 +352,15 @@
         """
 
         return super().dataset_path(location=location).replace(
             '.csv', f'_{self.interval}.csv'
         )
     # end dataset_path
 
-    async def async_get_market(self) -> Dict[str, Number]:
+    async def async_get_market(self) -> Dict[str, float]:
         """
         Gets the market data.
 
         :return: The bids and asks.
         """
 
         exchange = configure_exchange(
@@ -376,15 +374,15 @@
             method = exchange.fetch_tickers
 
         elif hasattr(exchange, "watch_tickers"):
             method = exchange.watch_tickers
         # end if
 
         data = await method(symbols=[self.symbol])
-        data: Dict[str, Union[Number, Dict[str, Number]]]
+        data: Dict[str, Union[float, Dict[str, float]]]
 
         if self.symbol in data:
             data = data[self.symbol]
         # end if
 
         data[ASKS.lower()] = data.get("ask")
         data[BIDS.lower()] = data.get("bid")
@@ -437,15 +435,15 @@
 
     def update_market(self) -> None:
         """Updates the market data."""
 
         asyncio.run(self.async_update_market())
     # end update_market
 
-    def get_market(self) -> Dict[str, Number]:
+    def get_market(self) -> Dict[str, float]:
         """
         Gets the market data.
 
         :return: The market data.
         """
 
         return asyncio.run(self.async_get_market())
@@ -511,15 +509,15 @@
 
     - market:
         The market structure of the data to store the fetched data in.
         This structure is a dictionary with exchange names as keys
         and dictionaries as values, where their keys are symbols,
         and their values are the dataframes to record the data.
 
-    >>> from crypto_screening.ohlcv import market_ohlcv_recorder
+    >>> from crypto_screening.market.screeners import market_ohlcv_recorder
     >>>
     >>> market = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
     >>> recorder = market_ohlcv_recorder(data=market)
     """
 
     COLUMNS = OHLCVScreener.COLUMNS
@@ -611,28 +609,24 @@
 
     - options:
         The ccxt options for the backend screening process.
 
     - cencel:
         The time to cancel screening process after no new data is fetched.
 
-    >>> from crypto_screening.ohlcv import MarketOHLCVScreener
-    >>> from crypto_screening.screener import wait_for_initialization
+    >>> from crypto_screening.market.screeners import MarketOHLCVScreener
     >>>
     >>> screener = MarketOHLCVScreener(
     >>>     data={
     >>>         "binance": ["BTC/USDT", "AAVE/EUR"],
     >>>         "bittrex": ["GRT/USD", "BTC/USD"]
     >>>     }
     >>> )
     >>>
     >>> screener.run(wait=True)
-    >>>
-    >>> while True:
-    >>>     screener.wait_for_update()
     """
 
     __slots__ = "interval", "pro", "options", "task", "exchanges", "length"
 
     INTERVAL = OHLCVScreener.INTERVAL
 
     PRO = OHLCVScreener.PRO
@@ -645,20 +639,20 @@
     COLUMNS = OHLCVScreener.COLUMNS
 
     screeners: List[OHLCVScreener]
 
     def __init__(
             self,
             interval: Optional[str] = None,
-            delay: Optional[Union[Number, dt.timedelta]] = None,
+            delay: Optional[Union[float, dt.timedelta]] = None,
             length: Optional[Union[int, bool]] = None,
             location: Optional[str] = None,
             pro: Optional[bool] = None,
             options: Optional[Dict[str, Any]] = None,
-            cancel: Optional[Union[Number, dt.timedelta]] = None,
+            cancel: Optional[Union[float, dt.timedelta]] = None,
             screeners: Optional[Iterable[OHLCVScreener]] = None,
             recorder: Optional[MarketRecorder] = None
     ) -> None:
         """
         Defines the class attributes.
 
         :param interval: The interval of the data to load.
@@ -697,18 +691,18 @@
 
     def create_screener(
             self,
             symbol: str,
             exchange: str,
             pro: Optional[bool] = True,
             length: Optional[Union[bool, int]] = None,
-            delay: Optional[Union[Number, dt.timedelta]] = None,
+            delay: Optional[Union[float, dt.timedelta]] = None,
             location: Optional[str] = None,
             options: Optional[Dict[str, Any]] = None,
-            cancel: Optional[Union[Number, dt.timedelta]] = None,
+            cancel: Optional[Union[float, dt.timedelta]] = None,
             container: Optional[Dict[str, Dict[str, OHLCVScreener]]] = None
     ) -> OHLCVScreener:
         """
         Creates the screener and inserts it into the container.
 
         :param container: The container to contain the new screener.
         :param symbol: The symbol of the screener.
@@ -753,18 +747,18 @@
 
     def _create_screener(
             self,
             symbol: str,
             exchange: str,
             pro: Optional[bool] = True,
             length: Optional[Union[bool, int]] = None,
-            delay: Optional[Union[Number, dt.timedelta]] = None,
+            delay: Optional[Union[float, dt.timedelta]] = None,
             location: Optional[str] = None,
             options: Optional[Dict[str, Any]] = None,
-            cancel: Optional[Union[Number, dt.timedelta]] = None,
+            cancel: Optional[Union[float, dt.timedelta]] = None,
             container: Optional[Dict[str, Dict[str, Optional[OHLCVScreener]]]] = None,
     ) -> OHLCVScreener:
         """
         Creates the screener and inserts it into the container.
 
         :param container: The container to contain the new screener.
         :param symbol: The symbol of the screener.
@@ -798,18 +792,18 @@
 
     def _create_screeners(
             self,
             symbols: Iterable[str],
             exchange: str,
             pro: Optional[bool] = True,
             length: Optional[Union[bool, int]] = None,
-            delay: Optional[Union[Number, dt.timedelta]] = None,
+            delay: Optional[Union[float, dt.timedelta]] = None,
             location: Optional[str] = None,
             options: Optional[Dict[str, Any]] = None,
-            cancel: Optional[Union[Number, dt.timedelta]] = None,
+            cancel: Optional[Union[float, dt.timedelta]] = None,
             container: Optional[Dict[str, Dict[str, Optional[OHLCVScreener]]]] = None,
             wait: Optional[bool] = True
     ) -> Dict[str, Optional[OHLCVScreener]]:
         """
         Creates the screener and inserts it into the container.
 
         :param container: The container to contain the new screener.
@@ -852,18 +846,18 @@
         return container
     # end _create_screeners
 
     def create_screeners(
             self,
             pro: Optional[bool] = True,
             length: Optional[Union[bool, int]] = None,
-            delay: Optional[Union[Number, dt.timedelta]] = None,
+            delay: Optional[Union[float, dt.timedelta]] = None,
             location: Optional[str] = None,
             options: Optional[Dict[str, Any]] = None,
-            cancel: Optional[Union[Number, dt.timedelta]] = None,
+            cancel: Optional[Union[float, dt.timedelta]] = None,
     ) -> List[OHLCVScreener]:
         """
         Initializes the create_screeners.
 
         :param pro: The value to use the pro interface.
         :param location: The saving location for the data.
         :param delay: The delay between each data fetching request.
@@ -922,15 +916,15 @@
 
         :return: The dataset of the spread data.
         """
 
         return self.recorder.ohlcv(exchange=exchange, symbol=symbol)
     # end ohlcv
 
-    async def async_get_market(self) -> Dict[str, Dict[str, Dict[str, Number]]]:
+    async def async_get_market(self) -> Dict[str, Dict[str, Dict[str, float]]]:
         """
         Gets the market data.
 
         :return: The market data.
         """
 
         market = {exchange: {} for exchange in self.exchanges}
@@ -954,15 +948,15 @@
 
     def update_market(self) -> None:
         """Updates the market data."""
 
         asyncio.run(self.async_update_market())
     # end update_market
 
-    def get_market(self) -> Dict[str, Dict[str, Dict[str, Number]]]:
+    def get_market(self) -> Dict[str, Dict[str, Dict[str, float]]]:
         """
         Gets the market data.
 
         :return: The market data.
         """
 
         return asyncio.run(self.async_get_market())
@@ -987,15 +981,15 @@
             screener.terminate()
         # end for
     # end terminate
 
     def start_screening(
             self,
             save: Optional[bool] = True,
-            timeout: Optional[Union[Number, dt.timedelta, dt.datetime]] = None
+            timeout: Optional[Union[float, dt.timedelta, dt.datetime]] = None
     ) -> None:
         """
         Starts the screening process.
 
         :param save: The value to save the data.
         :param timeout: The valur to add a timeout to the process.
         """
@@ -1016,16 +1010,16 @@
 
     def run(
             self,
             screen: Optional[bool] = True,
             save: Optional[bool] = True,
             block: Optional[bool] = False,
             update: Optional[bool] = True,
-            wait: Optional[Union[bool, Number, dt.timedelta, dt.datetime]] = False,
-            timeout: Optional[Union[Number, dt.timedelta, dt.datetime]] = None
+            wait: Optional[Union[bool, float, dt.timedelta, dt.datetime]] = False,
+            timeout: Optional[Union[float, dt.timedelta, dt.datetime]] = None
     ) -> None:
         """
         Runs the process of the price screening.
 
         :param screen: The value to start the screening.
         :param save: The value to save the data.
         :param wait: The value to wait after starting to run the process.
@@ -1046,20 +1040,20 @@
 # end MarketOHLCVScreener
 
 Market = Dict[str, Dict[str, pd.DataFrame]]
 
 def market_ohlcv_screener(
         data: Dict[str, Iterable[str]],
         interval: Optional[str] = None,
-        delay: Optional[Union[Number, dt.timedelta]] = None,
+        delay: Optional[Union[float, dt.timedelta]] = None,
         length: Optional[Union[int, bool]] = None,
         location: Optional[str] = None,
         pro: Optional[bool] = None,
         options: Optional[Dict[str, Any]] = None,
-        cancel: Optional[Union[Number, dt.timedelta]] = None,
+        cancel: Optional[Union[float, dt.timedelta]] = None,
         market: Optional[Market] = None,
         recorder: Optional[MarketOHLCVRecorder] = None,
 ) -> MarketOHLCVScreener:
     """
     Creates the market screener object for the data.
 
     :param data: The market data.
```

### Comparing `crypto-screening-1.5.0/crypto_screening/orderbook.py` & `crypto-screening-1.6.0/crypto_screening/market/screeners/orderbook.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,20 +20,19 @@
 from cryptofeed.types import OrderBook
 from cryptofeed.defines import L2_BOOK
 
 from crypto_screening.dataset import (
     BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME
 )
 from crypto_screening.symbols import adjust_symbol, Separator
-from crypto_screening.screener import (
+from crypto_screening.market.screeners import (
     BaseScreener, BaseMultiScreener,
     create_market_dataframe, MarketRecorder,
     structure_screener_datasets
 )
-from crypto_screening.hints import Number
 from crypto_screening.exchanges import EXCHANGES, EXCHANGE_NAMES
 from crypto_screening.process import find_string_value
 
 __all__ = [
     "MarketHandler",
     "MarketOrderbookScreener",
     "add_feeds",
@@ -114,15 +113,15 @@
 
     - market:
         The market structure of the data to store the fetched data in.
         This structure is a dictionary with exchange names as keys
         and dictionaries as values, where their keys are symbols,
         and their values are the dataframes to record the data.
 
-    >>> from crypto_screening.orderbook import market_orderbook_recorder
+    >>> from crypto_screening.market.screeners import market_orderbook_recorder
     >>>
     >>> market = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
     >>> recorder = market_orderbook_recorder(data=market)
     """
 
     __slots__ = "market"
@@ -335,15 +334,15 @@
 
     - handler:
         The handler object to handle the data feed.
 
     - recorder:
         The recorder object to record the data of the market from the feed.
 
-    >>> from crypto_screening.orderbook import market_orderbook_screener
+    >>> from crypto_screening.market.screeners import market_orderbook_screener
     >>>
     >>> structure = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
     >>> screener = market_orderbook_screener(data=structure)
     >>> screener.run()
     """
 
@@ -367,17 +366,17 @@
 
     COLUMNS = MarketOrderbookRecorder.COLUMNS
 
     def __init__(
             self,
             screeners: Optional[Iterable[OrderbookScreener]] = None,
             location: Optional[str] = None,
-            cancel: Optional[Union[Number, dt.timedelta]] = None,
-            delay: Optional[Union[Number, dt.timedelta]] = None,
-            refresh: Optional[Union[Number, dt.timedelta, bool]] = None,
+            cancel: Optional[Union[float, dt.timedelta]] = None,
+            delay: Optional[Union[float, dt.timedelta]] = None,
+            refresh: Optional[Union[float, dt.timedelta, bool]] = None,
             limited: Optional[bool] = None,
             handler: Optional[FeedHandler] = None,
             amount: Optional[int] = None,
             recorder: Optional[MarketOrderbookRecorder] = None
     ) -> None:
         """
         Creates the class attributes.
@@ -417,16 +416,16 @@
     # end __init__
 
     def create_screener(
             self,
             symbol: str,
             exchange: str,
             location: Optional[str] = None,
-            cancel: Optional[Union[Number, dt.timedelta]] = None,
-            delay: Optional[Union[Number, dt.timedelta]] = None,
+            cancel: Optional[Union[float, dt.timedelta]] = None,
+            delay: Optional[Union[float, dt.timedelta]] = None,
             container: Optional[Dict[str, Dict[str, OrderbookScreener]]] = None
     ) -> OrderbookScreener:
         """
         Defines the class attributes.
 
         :param symbol: The symbol of the asset.
         :param exchange: The exchange to get source data from.
@@ -461,16 +460,16 @@
 
         return screener
     # end create_screener
 
     def create_screeners(
             self,
             location: Optional[str] = None,
-            cancel: Optional[Union[Number, dt.timedelta]] = None,
-            delay: Optional[Union[Number, dt.timedelta]] = None,
+            cancel: Optional[Union[float, dt.timedelta]] = None,
+            delay: Optional[Union[float, dt.timedelta]] = None,
             container: Optional[Dict[str, Dict[str, OrderbookScreener]]] = None
     ) -> List[OrderbookScreener]:
         """
         Defines the class attributes.
 
         :param location: The saving location for the data.
         :param cancel: The time to cancel the waiting.
@@ -719,16 +718,16 @@
     def run(
             self,
             save: Optional[bool] = True,
             block: Optional[bool] = False,
             update: Optional[bool] = True,
             screen: Optional[bool] = True,
             loop: Optional[asyncio.AbstractEventLoop] = None,
-            wait: Optional[Union[bool, Number, dt.timedelta, dt.datetime]] = False,
-            timeout: Optional[Union[Number, dt.timedelta, dt.datetime]] = None,
+            wait: Optional[Union[bool, float, dt.timedelta, dt.datetime]] = False,
+            timeout: Optional[Union[float, dt.timedelta, dt.datetime]] = None,
     ) -> None:
         """
         Runs the program.
 
         :param save: The value to save the data.
         :param wait: The value to wait after starting to run the process.
         :param block: The value to block the execution.
@@ -773,21 +772,21 @@
         market=create_orderbook_market(data=data)
     )
 # end market_orderbook_recorder
 
 def market_orderbook_screener(
         data: Dict[str, Iterable[str]],
         location: Optional[str] = None,
-        cancel: Optional[Union[Number, dt.timedelta]] = None,
-        delay: Optional[Union[Number, dt.timedelta]] = None,
+        cancel: Optional[Union[float, dt.timedelta]] = None,
+        delay: Optional[Union[float, dt.timedelta]] = None,
         limited: Optional[bool] = None,
         handler: Optional[FeedHandler] = None,
         market: Optional[Market] = None,
         amount: Optional[int] = None,
-        refresh: Optional[Union[Number, dt.timedelta, bool]] = None,
+        refresh: Optional[Union[float, dt.timedelta, bool]] = None,
         recorder: Optional[MarketOrderbookRecorder] = None,
         fixed: Optional[bool] = True,
         separator: Optional[str] = None,
         parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
 ) -> MarketOrderbookScreener:
     """
     Creates the market screener object for the data.
```

### Comparing `crypto-screening-1.5.0/crypto_screening/process.py` & `crypto-screening-1.6.0/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.5.0/crypto_screening/symbols.py` & `crypto-screening-1.6.0/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.5.0/crypto_screening/validate.py` & `crypto-screening-1.6.0/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.5.0/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-1.6.0/crypto_screening.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.5.0
+Version: 1.6.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.5.0/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-1.6.0/crypto_screening.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 MANIFEST.in
 README.md
 build.py
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 setup.py
-crypto_screening/base.py
 crypto_screening/dataset.py
-crypto_screening/document.py
 crypto_screening/exchanges.py
-crypto_screening/hints.py
 crypto_screening/interval.py
-crypto_screening/ohlcv.py
-crypto_screening/orderbook.py
 crypto_screening/process.py
-crypto_screening/screener.py
 crypto_screening/symbols.py
 crypto_screening/validate.py
 crypto_screening.egg-info/PKG-INFO
 crypto_screening.egg-info/SOURCES.txt
 crypto_screening.egg-info/dependency_links.txt
 crypto_screening.egg-info/requires.txt
 crypto_screening.egg-info/top_level.txt
 crypto_screening/collect/assets.py
-crypto_screening/collect/document.py
 crypto_screening/collect/exchanges.py
 crypto_screening/collect/screeners.py
-crypto_screening/collect/symbols.py
+crypto_screening/collect/symbols.py
+crypto_screening/market/waiting.py
+crypto_screening/market/foundation/data.py
+crypto_screening/market/foundation/protocols.py
+crypto_screening/market/foundation/waiting.py
+crypto_screening/market/screeners/__init__.py
+crypto_screening/market/screeners/base.py
+crypto_screening/market/screeners/ohlcv.py
+crypto_screening/market/screeners/orderbook.py
```

### Comparing `crypto-screening-1.5.0/pyproject.toml` & `crypto-screening-1.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '1.5.0'
+version = '1.6.0'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-1.5.0/setup.py` & `crypto-screening-1.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='1.5.0',
+        version='1.6.0',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

