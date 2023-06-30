# Comparing `tmp/crypto-screening-1.8.0.tar.gz` & `tmp/crypto-screening-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-1.8.0.tar", last modified: Fri Jun 30 14:58:53 2023, max compression
+gzip compressed data, was "crypto-screening-1.8.1.tar", last modified: Fri Jun 30 15:39:06 2023, max compression
```

## Comparing `crypto-screening-1.8.0.tar` & `crypto-screening-1.8.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 14:58:53.025201 crypto-screening-1.8.0/
--rw-rw-rw-   0        0        0       98 2023-06-30 14:58:51.000000 crypto-screening-1.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2085 2023-06-30 14:58:53.025201 crypto-screening-1.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     1264 2023-06-23 16:52:27.000000 crypto-screening-1.8.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.8.0/build.py
-drwxrwxrwx   0        0        0        0 2023-06-30 14:58:52.943381 crypto-screening-1.8.0/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-06-30 14:58:52.964370 crypto-screening-1.8.0/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-1.8.0/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-1.8.0/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0    10101 2023-06-30 14:50:05.000000 crypto-screening-1.8.0/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18811 2023-06-30 14:56:10.000000 crypto-screening-1.8.0/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-1.8.0/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.8.0/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5200 2023-06-30 14:44:13.000000 crypto-screening-1.8.0/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-06-30 14:58:52.969368 crypto-screening-1.8.0/crypto_screening/market/
-drwxrwxrwx   0        0        0        0 2023-06-30 14:58:52.986370 crypto-screening-1.8.0/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10832 2023-06-30 09:27:04.000000 crypto-screening-1.8.0/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      889 2023-06-30 09:21:25.000000 crypto-screening-1.8.0/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     8839 2023-06-30 09:21:46.000000 crypto-screening-1.8.0/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-06-30 14:58:53.024207 crypto-screening-1.8.0/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-1.8.0/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    13648 2023-06-30 10:44:18.000000 crypto-screening-1.8.0/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0     3391 2023-06-30 10:45:18.000000 crypto-screening-1.8.0/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    32765 2023-06-30 10:47:24.000000 crypto-screening-1.8.0/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    24997 2023-06-30 10:47:57.000000 crypto-screening-1.8.0/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0     5401 2023-06-30 10:44:43.000000 crypto-screening-1.8.0/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-1.8.0/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-1.8.0/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9898 2023-06-30 14:44:13.000000 crypto-screening-1.8.0/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-1.8.0/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-06-30 14:58:52.957371 crypto-screening-1.8.0/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2085 2023-06-30 14:58:52.000000 crypto-screening-1.8.0/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1053 2023-06-30 14:58:52.000000 crypto-screening-1.8.0/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 14:58:52.000000 crypto-screening-1.8.0/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-06-30 14:58:52.000000 crypto-screening-1.8.0/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-30 14:58:52.000000 crypto-screening-1.8.0/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-06-30 14:58:51.000000 crypto-screening-1.8.0/pyproject.toml
--rw-rw-rw-   0        0        0       99 2023-06-28 09:56:21.000000 crypto-screening-1.8.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.8.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 14:58:53.025201 crypto-screening-1.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-06-30 14:58:22.000000 crypto-screening-1.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 15:39:06.779683 crypto-screening-1.8.1/
+-rw-rw-rw-   0        0        0       98 2023-06-30 15:39:06.000000 crypto-screening-1.8.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2085 2023-06-30 15:39:06.779683 crypto-screening-1.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1264 2023-06-23 16:52:27.000000 crypto-screening-1.8.1/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.8.1/build.py
+drwxrwxrwx   0        0        0        0 2023-06-30 15:39:06.758684 crypto-screening-1.8.1/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-06-30 15:39:06.771716 crypto-screening-1.8.1/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-1.8.1/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-1.8.1/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0    10119 2023-06-30 15:31:03.000000 crypto-screening-1.8.1/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18829 2023-06-30 15:31:13.000000 crypto-screening-1.8.1/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-1.8.1/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.8.1/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5267 2023-06-30 15:34:44.000000 crypto-screening-1.8.1/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-06-30 15:39:06.771716 crypto-screening-1.8.1/crypto_screening/market/
+drwxrwxrwx   0        0        0        0 2023-06-30 15:39:06.773684 crypto-screening-1.8.1/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10832 2023-06-30 09:27:04.000000 crypto-screening-1.8.1/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      889 2023-06-30 09:21:25.000000 crypto-screening-1.8.1/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     7987 2023-06-30 15:33:11.000000 crypto-screening-1.8.1/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-06-30 15:39:06.778684 crypto-screening-1.8.1/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-1.8.1/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    13648 2023-06-30 10:44:18.000000 crypto-screening-1.8.1/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0     3391 2023-06-30 10:45:18.000000 crypto-screening-1.8.1/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    32765 2023-06-30 10:47:24.000000 crypto-screening-1.8.1/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    24997 2023-06-30 10:47:57.000000 crypto-screening-1.8.1/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0     5401 2023-06-30 10:44:43.000000 crypto-screening-1.8.1/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-1.8.1/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-1.8.1/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9964 2023-06-30 15:35:25.000000 crypto-screening-1.8.1/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-1.8.1/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-06-30 15:39:06.767684 crypto-screening-1.8.1/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2085 2023-06-30 15:39:06.000000 crypto-screening-1.8.1/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1053 2023-06-30 15:39:06.000000 crypto-screening-1.8.1/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 15:39:06.000000 crypto-screening-1.8.1/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-06-30 15:39:06.000000 crypto-screening-1.8.1/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-30 15:39:06.000000 crypto-screening-1.8.1/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-06-30 15:39:06.000000 crypto-screening-1.8.1/pyproject.toml
+-rw-rw-rw-   0        0        0       99 2023-06-28 09:56:21.000000 crypto-screening-1.8.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.8.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 15:39:06.779683 crypto-screening-1.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-06-30 15:38:55.000000 crypto-screening-1.8.1/setup.py
```

### Comparing `crypto-screening-1.8.0/PKG-INFO` & `crypto-screening-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.8.0
+Version: 1.8.1
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.8.0/README.md` & `crypto-screening-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.0/build.py` & `crypto-screening-1.8.1/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.0/crypto_screening/collect/assets.py` & `crypto-screening-1.8.1/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.0/crypto_screening/collect/exchanges.py` & `crypto-screening-1.8.1/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.0/crypto_screening/collect/screeners.py` & `crypto-screening-1.8.1/crypto_screening/collect/screeners.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
             # end if
         # end for
     # end for
 
     return set(pairs)
 # end matching_screener_pairs
 
-@dataclass(repr=False, slots=True)
+@dataclass(repr=False, slots=True, unsafe_hash=True)
 class MarketScreenerSignature(MarketSymbolSignature):
     """A class to represent the data for the execution of a trade."""
 
     screener: Optional[BaseScreener] = None
 # end MarketScreenerSignature
 
 def matching_screener_signatures(
```

### Comparing `crypto-screening-1.8.0/crypto_screening/collect/symbols.py` & `crypto-screening-1.8.1/crypto_screening/collect/symbols.py`

 * *Files 0% similar despite different names*

```diff
@@ -547,15 +547,15 @@
             # end if
         # end for
     # end for
 
     return set(pairs)
 # end matching_symbol_pairs
 
-@dataclass(repr=False, slots=True)
+@dataclass(repr=False, slots=True, unsafe_hash=True)
 class MarketSymbolSignature(BaseModel):
     """A class to represent the data for the execution of a trade."""
 
     asset: str
     currency: str
     exchange: str
 # end MarketPairSignature
```

### Comparing `crypto-screening-1.8.0/crypto_screening/dataset.py` & `crypto-screening-1.8.1/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.0/crypto_screening/interval.py` & `crypto-screening-1.8.1/crypto_screening/interval.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # interval.py
 
 from typing import Tuple, Union, Iterable
-
+from dataclasses import dataclass
 import datetime as dt
 
 from represent import BaseModel, Modifiers
 
 
 __all__ = [
     "interval_to_duration",
@@ -34,15 +34,15 @@
     HOURS: dt.timedelta(hours=1),
     DAYS: dt.timedelta(days=1),
     WEEKS: dt.timedelta(days=7),
     MONTHS: dt.timedelta(days=30),
     YEARS: dt.timedelta(days=365)
 }
 
-
+@dataclass(init=False, repr=False)
 class Interval(BaseModel):
     """
     A class to represent a trading pair.
 
     This object represents a pair of assets that can be traded.
 
     attributes:
```

### Comparing `crypto-screening-1.8.0/crypto_screening/market/foundation/data.py` & `crypto-screening-1.8.1/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.0/crypto_screening/market/foundation/protocols.py` & `crypto-screening-1.8.1/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.0/crypto_screening/market/foundation/waiting.py` & `crypto-screening-1.8.1/crypto_screening/market/foundation/waiting.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # waiting.py
 
 import datetime as dt
 import time
+from dataclasses import dataclass
 from typing import (
-    Optional, Union, Iterable,
+    Optional, Union, Iterable, ClassVar,
     Generic, TypeVar, Callable, List
 )
 
 from represent import BaseModel, Modifiers
 
 from crypto_screening.market.foundation.protocols import (
     BaseScreenerProtocol, BaseMultiScreenerProtocol
@@ -21,60 +22,31 @@
     "base_wait_for_dynamic_initialization"
 ]
 
 _BaseScreener = TypeVar(
     "_BaseScreener", BaseScreenerProtocol, BaseMultiScreenerProtocol
 )
 
+@dataclass(repr=False, slots=True)
 class WaitingState(BaseModel, Generic[_BaseScreener]):
     """A class to represent the waiting state of screener objects."""
 
-    modifiers = Modifiers(hidden=["screeners"], properties=["time"])
+    screeners: Iterable[Union[_BaseScreener]]
+    start: dt.datetime
+    end: dt.datetime
+    stop: Optional[bool] = False
+    delay: Optional[float] = 0
+    count: Optional[int] = 0
+    canceled: Optional[bool] = False
+    cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
 
-    __slots__ = (
-        "screeners", "delay", "count",
-        "canceled", "cancel", "start", "end"
+    modifiers: ClassVar[Modifiers] = Modifiers(
+        hidden=["screeners"], properties=["time"]
     )
 
-    def __init__(
-            self,
-            screeners: Iterable[Union[_BaseScreener]],
-            start: dt.datetime,
-            end: dt.datetime,
-            stop: Optional[bool] = None,
-            delay: Optional[float] = None,
-            count: Optional[int] = None,
-            canceled: Optional[bool] = None,
-            cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
-    ) -> None:
-        """
-        Defines the class attributes.
-
-        :param screeners: The screener objects.
-        :param start: The start time.
-        :param end: The end time.
-        :param stop: The stop value.
-        :param delay: The waiting delay.
-        :param count: The iterations count.
-        :param canceled: The value for the waiting being canceled.
-        :param cancel: The time to cancel the waiting.
-        """
-
-        self.screeners = screeners
-
-        self.start = start
-        self.end = end
-        self.cancel = cancel
-
-        self.stop = stop or False
-        self.canceled = canceled or False
-        self.delay = delay or 0
-        self.count = count or 0
-    # end __init__
-
     @property
     def time(self) -> dt.timedelta:
         """
         Returns the amount of waited time.
 
         :return: The waiting time.
         """
```

### Comparing `crypto-screening-1.8.0/crypto_screening/market/screeners/base.py` & `crypto-screening-1.8.1/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.0/crypto_screening/market/screeners/container.py` & `crypto-screening-1.8.1/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.0/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-1.8.1/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.0/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-1.8.1/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.0/crypto_screening/market/screeners/recorder.py` & `crypto-screening-1.8.1/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.0/crypto_screening/market/waiting.py` & `crypto-screening-1.8.1/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.0/crypto_screening/process.py` & `crypto-screening-1.8.1/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.0/crypto_screening/symbols.py` & `crypto-screening-1.8.1/crypto_screening/symbols.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # symbols.py
 
+from dataclasses import dataclass
 from typing import (
-    Optional, Tuple, Dict,
-    Any, List, Iterable, Union
+    Optional, Tuple, Dict, Any, List, Iterable, Union
 )
 
 from represent import BaseModel, Modifiers
 
 __all__ = [
     "Pair",
     "symbol_to_pair",
@@ -28,14 +28,15 @@
 
 class Separator:
     """A class to contain the separator value."""
 
     value = "/"
 # end Separator
 
+@dataclass(init=False, repr=False)
 class Pair(BaseModel):
     """
     A class to represent a trading pair.
 
     This object represents a pair of assets that can be traded.
 
     attributes:
```

### Comparing `crypto-screening-1.8.0/crypto_screening/validate.py` & `crypto-screening-1.8.1/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.0/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-1.8.1/crypto_screening.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.8.0
+Version: 1.8.1
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.8.0/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-1.8.1/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.0/pyproject.toml` & `crypto-screening-1.8.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '1.8.0'
+version = '1.8.1'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-1.8.0/setup.py` & `crypto-screening-1.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='1.8.0',
+        version='1.8.1',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

