# Comparing `tmp/crypto-screening-1.6.0.tar.gz` & `tmp/crypto-screening-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-1.6.0.tar", last modified: Fri Jun 30 09:57:45 2023, max compression
+gzip compressed data, was "crypto-screening-1.7.0.tar", last modified: Fri Jun 30 10:48:33 2023, max compression
```

## Comparing `crypto-screening-1.6.0.tar` & `crypto-screening-1.7.0.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 09:57:45.901259 crypto-screening-1.6.0/
--rw-rw-rw-   0        0        0       98 2023-06-30 09:57:45.000000 crypto-screening-1.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2085 2023-06-30 09:57:45.901259 crypto-screening-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     1264 2023-06-23 16:52:27.000000 crypto-screening-1.6.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.6.0/build.py
-drwxrwxrwx   0        0        0        0 2023-06-30 09:57:45.886754 crypto-screening-1.6.0/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-06-30 09:57:45.893751 crypto-screening-1.6.0/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17713 2023-06-28 11:01:21.000000 crypto-screening-1.6.0/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-1.6.0/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0    10359 2023-06-30 09:27:48.000000 crypto-screening-1.6.0/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    19287 2023-06-28 10:54:03.000000 crypto-screening-1.6.0/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-1.6.0/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.6.0/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     2665 2023-06-23 16:52:27.000000 crypto-screening-1.6.0/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-06-30 09:57:45.894751 crypto-screening-1.6.0/crypto_screening/market/
-drwxrwxrwx   0        0        0        0 2023-06-30 09:57:45.896751 crypto-screening-1.6.0/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10832 2023-06-30 09:27:04.000000 crypto-screening-1.6.0/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      889 2023-06-30 09:21:25.000000 crypto-screening-1.6.0/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     8839 2023-06-30 09:21:46.000000 crypto-screening-1.6.0/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-06-30 09:57:45.900259 crypto-screening-1.6.0/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      179 2023-06-30 09:14:39.000000 crypto-screening-1.6.0/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    18775 2023-06-30 09:22:16.000000 crypto-screening-1.6.0/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0    32700 2023-06-30 09:23:12.000000 crypto-screening-1.6.0/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    24937 2023-06-30 09:23:33.000000 crypto-screening-1.6.0/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-1.6.0/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2378 2023-06-27 10:23:45.000000 crypto-screening-1.6.0/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9894 2023-06-25 16:31:01.000000 crypto-screening-1.6.0/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-1.6.0/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-06-30 09:57:45.890743 crypto-screening-1.6.0/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2085 2023-06-30 09:57:45.000000 crypto-screening-1.6.0/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      960 2023-06-30 09:57:45.000000 crypto-screening-1.6.0/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 09:57:45.000000 crypto-screening-1.6.0/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-06-30 09:57:45.000000 crypto-screening-1.6.0/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-30 09:57:45.000000 crypto-screening-1.6.0/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-06-30 09:41:35.000000 crypto-screening-1.6.0/pyproject.toml
--rw-rw-rw-   0        0        0       99 2023-06-28 09:56:21.000000 crypto-screening-1.6.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.6.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 09:57:45.901259 crypto-screening-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-06-30 09:41:28.000000 crypto-screening-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 10:48:33.003560 crypto-screening-1.7.0/
+-rw-rw-rw-   0        0        0       98 2023-06-30 10:48:32.000000 crypto-screening-1.7.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2085 2023-06-30 10:48:33.002560 crypto-screening-1.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1264 2023-06-23 16:52:27.000000 crypto-screening-1.7.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.7.0/build.py
+drwxrwxrwx   0        0        0        0 2023-06-30 10:48:32.983559 crypto-screening-1.7.0/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-06-30 10:48:32.995559 crypto-screening-1.7.0/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17713 2023-06-28 11:01:21.000000 crypto-screening-1.7.0/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-1.7.0/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0    10359 2023-06-30 09:27:48.000000 crypto-screening-1.7.0/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    19287 2023-06-28 10:54:03.000000 crypto-screening-1.7.0/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-1.7.0/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.7.0/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     2665 2023-06-23 16:52:27.000000 crypto-screening-1.7.0/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-06-30 10:48:32.995559 crypto-screening-1.7.0/crypto_screening/market/
+drwxrwxrwx   0        0        0        0 2023-06-30 10:48:32.997559 crypto-screening-1.7.0/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10832 2023-06-30 09:27:04.000000 crypto-screening-1.7.0/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      889 2023-06-30 09:21:25.000000 crypto-screening-1.7.0/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     8839 2023-06-30 09:21:46.000000 crypto-screening-1.7.0/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-06-30 10:48:33.002560 crypto-screening-1.7.0/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-1.7.0/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    13648 2023-06-30 10:44:18.000000 crypto-screening-1.7.0/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0     3391 2023-06-30 10:45:18.000000 crypto-screening-1.7.0/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    32765 2023-06-30 10:47:24.000000 crypto-screening-1.7.0/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    24997 2023-06-30 10:47:57.000000 crypto-screening-1.7.0/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0     5401 2023-06-30 10:44:43.000000 crypto-screening-1.7.0/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-1.7.0/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2378 2023-06-27 10:23:45.000000 crypto-screening-1.7.0/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9894 2023-06-25 16:31:01.000000 crypto-screening-1.7.0/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-1.7.0/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-06-30 10:48:32.992560 crypto-screening-1.7.0/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2085 2023-06-30 10:48:32.000000 crypto-screening-1.7.0/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1053 2023-06-30 10:48:32.000000 crypto-screening-1.7.0/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 10:48:32.000000 crypto-screening-1.7.0/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-06-30 10:48:32.000000 crypto-screening-1.7.0/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-30 10:48:32.000000 crypto-screening-1.7.0/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-06-30 10:48:32.000000 crypto-screening-1.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0       99 2023-06-28 09:56:21.000000 crypto-screening-1.7.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.7.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 10:48:33.003560 crypto-screening-1.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-06-30 10:48:29.000000 crypto-screening-1.7.0/setup.py
```

### Comparing `crypto-screening-1.6.0/PKG-INFO` & `crypto-screening-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.6.0
+Version: 1.7.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.6.0/README.md` & `crypto-screening-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.6.0/build.py` & `crypto-screening-1.7.0/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.6.0/crypto_screening/collect/assets.py` & `crypto-screening-1.7.0/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.6.0/crypto_screening/collect/exchanges.py` & `crypto-screening-1.7.0/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.6.0/crypto_screening/collect/screeners.py` & `crypto-screening-1.7.0/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.6.0/crypto_screening/collect/symbols.py` & `crypto-screening-1.7.0/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.6.0/crypto_screening/dataset.py` & `crypto-screening-1.7.0/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.6.0/crypto_screening/interval.py` & `crypto-screening-1.7.0/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.6.0/crypto_screening/market/foundation/data.py` & `crypto-screening-1.7.0/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.6.0/crypto_screening/market/foundation/protocols.py` & `crypto-screening-1.7.0/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.6.0/crypto_screening/market/foundation/waiting.py` & `crypto-screening-1.7.0/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.6.0/crypto_screening/market/screeners/base.py` & `crypto-screening-1.7.0/crypto_screening/market/screeners/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,39 +4,38 @@
 import time
 from typing import (
     Optional, Union, Dict, Iterable, Any, List
 )
 
 import pandas as pd
 
-from represent import Modifiers, BaseModel
+from represent import Modifiers
 
 from multithreading import Caller, multi_threaded_call
 
-from crypto_screening.process import find_string_value
-from crypto_screening.dataset import save_dataset, load_dataset, DATE_TIME
+from crypto_screening.dataset import save_dataset, load_dataset
 from crypto_screening.symbols import Separator
 from crypto_screening.validate import validate_exchange, validate_symbol
 from crypto_screening.market.foundation.waiting import (
     base_wait_for_initialization, base_wait_for_dynamic_initialization,
     base_wait_for_dynamic_update, base_wait_for_update, WaitingState
 )
 from crypto_screening.market.foundation.data import DataCollector
+from crypto_screening.market.screeners.recorder import (
+    MarketRecorder, create_market_dataframe
+)
 from crypto_screening.market.foundation.protocols import (
     BaseMultiScreenerProtocol, BaseScreenerProtocol
 )
 
 __all__ = [
     "BaseScreener",
     "BaseMultiScreener",
-    "MarketRecorder",
     "structure_screeners_datasets",
-    "structure_screener_datasets",
-    "create_market_dataframe",
-    "validate_market"
+    "structure_screener_datasets"
 ]
 
 class BaseScreener(DataCollector, BaseScreenerProtocol):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
@@ -241,200 +240,14 @@
             end = time.time()
 
             time.sleep(max([delay - (end - start), 1]))
         # end while
     # end saving_loop
 # end BaseScreener
 
-Market = Dict[str, Dict[str, pd.DataFrame]]
-
-def create_market_dataframe(columns: Optional[Iterable[str]] = None) -> pd.DataFrame:
-    """
-    Creates a dataframe for the order book data.
-
-    :param columns: The dataset columns.
-
-    :return: The dataframe.
-    """
-
-    market = pd.DataFrame(
-        {column: [] for column in columns or []}, index=[]
-    )
-    market.index.name = DATE_TIME
-
-    return market
-# end create_market_dataframe
-
-def validate_market(data: Any) -> Market:
-    """
-    Validates the data.
-
-    :param data: The data to validate.
-
-    :return: The valid data.
-    """
-
-    if data is None:
-        return {}
-    # end if
-
-    try:
-        if not isinstance(data, dict):
-            raise ValueError
-        # end if
-
-        for exchange, values in data.items():
-            if not (
-                    isinstance(exchange, str) and
-                    (
-                            (
-                                    isinstance(values, dict) and
-                                    all(
-                                        isinstance(symbol, str) and
-                                        isinstance(dataset, pd.DataFrame)
-                                        for symbol, dataset in values.items()
-                                    )
-                            ) or (all(isinstance(value, str) for value in values))
-                    )
-            ):
-                raise ValueError
-            # end if
-
-            if not isinstance(values, dict):
-                data[exchange] = {
-                    symbol: create_market_dataframe()
-                    for symbol in values
-                }
-            # end if
-        # end for
-
-    except (TypeError, ValueError):
-        raise ValueError(
-            f"Data must be of type {Market}, not: {data}."
-        )
-    # end try
-
-    return data
-# end validate_market
-
-class MarketRecorder(BaseModel):
-    """
-    A class to represent a crypto data feed recorder.
-    This object passes the record method to the handler object to record
-    the data fetched by the handler.
-
-    Parameters:
-
-    - market:
-        The market structure of the data to store the fetched data in.
-        This structure is a dictionary with exchange names as keys
-        and dictionaries as values, where their keys are symbols,
-        and their values are the dataframes to record the data.
-
-    >>> from crypto_screening.market.screeners import MarketRecorder
-    >>>
-    >>> market = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
-    >>>
-    >>> recorder = MarketRecorder(data=market)
-
-    """
-
-    modifiers = Modifiers(**BaseModel.modifiers)
-    modifiers.hidden.append("market")
-
-    __slots__ = "market"
-
-    def __init__(self, market: Optional[Market] = None) -> None:
-        """
-        Defines the class attributes.
-
-        :param market: The object to fill with the crypto feed record.
-        """
-
-        self.market = self.validate_market(data=market)
-    # end __init__
-
-    @staticmethod
-    def validate_market(data: Any) -> Market:
-        """
-        Validates the data.
-
-        :param data: The data to validate.
-
-        :return: The valid data.
-        """
-
-        return validate_market(data=data)
-    # end validate_market
-
-    def structure(self) -> Dict[str, List[str]]:
-        """
-        Returns the structure of the market data.
-
-        :return: The structure of the market.
-        """
-
-        return {
-            exchange: list(symbols.keys())
-            for exchange, symbols in self.market.items()
-        }
-    # end structure
-
-    def data(self, exchange: str, symbol: str) -> pd.DataFrame:
-        """
-        Returns the market data of the symbol from the exchange.
-
-        :param exchange: The source name of the exchange.
-        :param symbol: The symbol of the pair.
-
-        :return: The dataset of the spread data.
-        """
-
-        exchange = find_string_value(
-            value=exchange, values=self.market.keys()
-        )
-
-        validate_exchange(
-            exchange=exchange,
-            exchanges=self.market.keys(),
-            provider=self
-        )
-
-        validate_symbol(
-            symbol=symbol,
-            exchange=exchange,
-            exchanges=self.market.keys(),
-            symbols=self.market[exchange],
-            provider=self
-        )
-
-        return self.market[exchange][symbol]
-    # end data
-
-    def in_market(self, exchange: str, symbol: str) -> bool:
-        """
-        Returns the market data of the symbol from the exchange.
-
-        :param exchange: The source name of the exchange.
-        :param symbol: The symbol of the pair.
-
-        :return: The dataset of the spread data.
-        """
-
-        try:
-            self.data(exchange=exchange, symbol=symbol)
-
-            return True
-
-        except ValueError:
-            return False
-        # end try
-    # end in_market
-# end MarketRecorder
-
 class BaseMultiScreener(DataCollector, BaseMultiScreenerProtocol):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
```

### Comparing `crypto-screening-1.6.0/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-1.7.0/crypto_screening/market/screeners/ohlcv.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,19 @@
 from multithreading import Caller, multi_threaded_call
 
 from crypto_screening.dataset import (
     OPEN, HIGH, LOW, CLOSE, VOLUME, BIDS, ASKS,
     DATE_TIME, OHLCV_COLUMNS, ASKS_VOLUME, BIDS_VOLUME
 )
 from crypto_screening.interval import interval_to_total_time
-from crypto_screening.market.screeners import (
-    BaseMultiScreener, structure_screener_datasets,
-    BaseScreener, MarketRecorder, create_market_dataframe
+from crypto_screening.market.screeners.base import (
+    BaseMultiScreener, structure_screener_datasets, BaseScreener
+)
+from crypto_screening.market.screeners.recorder import (
+    MarketRecorder, create_market_dataframe
 )
 
 __all__ = [
     "OHLCVScreener",
     "MarketOHLCVScreener",
     "market_ohlcv_recorder",
     "MarketOHLCVRecorder",
```

### Comparing `crypto-screening-1.6.0/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-1.7.0/crypto_screening/market/screeners/orderbook.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,18 +20,19 @@
 from cryptofeed.types import OrderBook
 from cryptofeed.defines import L2_BOOK
 
 from crypto_screening.dataset import (
     BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME
 )
 from crypto_screening.symbols import adjust_symbol, Separator
-from crypto_screening.market.screeners import (
-    BaseScreener, BaseMultiScreener,
-    create_market_dataframe, MarketRecorder,
-    structure_screener_datasets
+from crypto_screening.market.screeners.base import (
+    BaseScreener, BaseMultiScreener, structure_screener_datasets
+)
+from crypto_screening.market.screeners.recorder import (
+    create_market_dataframe, MarketRecorder
 )
 from crypto_screening.exchanges import EXCHANGES, EXCHANGE_NAMES
 from crypto_screening.process import find_string_value
 
 __all__ = [
     "MarketHandler",
     "MarketOrderbookScreener",
```

### Comparing `crypto-screening-1.6.0/crypto_screening/market/waiting.py` & `crypto-screening-1.7.0/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.6.0/crypto_screening/process.py` & `crypto-screening-1.7.0/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.6.0/crypto_screening/symbols.py` & `crypto-screening-1.7.0/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.6.0/crypto_screening/validate.py` & `crypto-screening-1.7.0/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.6.0/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-1.7.0/crypto_screening.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.6.0
+Version: 1.7.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.6.0/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-1.7.0/crypto_screening.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -22,9 +22,11 @@
 crypto_screening/collect/symbols.py
 crypto_screening/market/waiting.py
 crypto_screening/market/foundation/data.py
 crypto_screening/market/foundation/protocols.py
 crypto_screening/market/foundation/waiting.py
 crypto_screening/market/screeners/__init__.py
 crypto_screening/market/screeners/base.py
+crypto_screening/market/screeners/container.py
 crypto_screening/market/screeners/ohlcv.py
-crypto_screening/market/screeners/orderbook.py
+crypto_screening/market/screeners/orderbook.py
+crypto_screening/market/screeners/recorder.py
```

### Comparing `crypto-screening-1.6.0/pyproject.toml` & `crypto-screening-1.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '1.6.0'
+version = '1.7.0'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-1.6.0/setup.py` & `crypto-screening-1.7.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='1.6.0',
+        version='1.7.0',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

