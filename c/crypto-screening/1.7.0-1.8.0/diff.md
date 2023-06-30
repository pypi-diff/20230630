# Comparing `tmp/crypto-screening-1.7.0.tar.gz` & `tmp/crypto-screening-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-1.7.0.tar", last modified: Fri Jun 30 10:48:33 2023, max compression
+gzip compressed data, was "crypto-screening-1.8.0.tar", last modified: Fri Jun 30 14:58:53 2023, max compression
```

## Comparing `crypto-screening-1.7.0.tar` & `crypto-screening-1.8.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 10:48:33.003560 crypto-screening-1.7.0/
--rw-rw-rw-   0        0        0       98 2023-06-30 10:48:32.000000 crypto-screening-1.7.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2085 2023-06-30 10:48:33.002560 crypto-screening-1.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     1264 2023-06-23 16:52:27.000000 crypto-screening-1.7.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.7.0/build.py
-drwxrwxrwx   0        0        0        0 2023-06-30 10:48:32.983559 crypto-screening-1.7.0/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-06-30 10:48:32.995559 crypto-screening-1.7.0/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17713 2023-06-28 11:01:21.000000 crypto-screening-1.7.0/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-1.7.0/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0    10359 2023-06-30 09:27:48.000000 crypto-screening-1.7.0/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    19287 2023-06-28 10:54:03.000000 crypto-screening-1.7.0/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-1.7.0/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.7.0/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     2665 2023-06-23 16:52:27.000000 crypto-screening-1.7.0/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-06-30 10:48:32.995559 crypto-screening-1.7.0/crypto_screening/market/
-drwxrwxrwx   0        0        0        0 2023-06-30 10:48:32.997559 crypto-screening-1.7.0/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10832 2023-06-30 09:27:04.000000 crypto-screening-1.7.0/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      889 2023-06-30 09:21:25.000000 crypto-screening-1.7.0/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     8839 2023-06-30 09:21:46.000000 crypto-screening-1.7.0/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-06-30 10:48:33.002560 crypto-screening-1.7.0/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-1.7.0/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    13648 2023-06-30 10:44:18.000000 crypto-screening-1.7.0/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0     3391 2023-06-30 10:45:18.000000 crypto-screening-1.7.0/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    32765 2023-06-30 10:47:24.000000 crypto-screening-1.7.0/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    24997 2023-06-30 10:47:57.000000 crypto-screening-1.7.0/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0     5401 2023-06-30 10:44:43.000000 crypto-screening-1.7.0/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-1.7.0/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2378 2023-06-27 10:23:45.000000 crypto-screening-1.7.0/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9894 2023-06-25 16:31:01.000000 crypto-screening-1.7.0/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-1.7.0/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-06-30 10:48:32.992560 crypto-screening-1.7.0/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2085 2023-06-30 10:48:32.000000 crypto-screening-1.7.0/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1053 2023-06-30 10:48:32.000000 crypto-screening-1.7.0/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 10:48:32.000000 crypto-screening-1.7.0/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-06-30 10:48:32.000000 crypto-screening-1.7.0/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-30 10:48:32.000000 crypto-screening-1.7.0/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-06-30 10:48:32.000000 crypto-screening-1.7.0/pyproject.toml
--rw-rw-rw-   0        0        0       99 2023-06-28 09:56:21.000000 crypto-screening-1.7.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.7.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 10:48:33.003560 crypto-screening-1.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-06-30 10:48:29.000000 crypto-screening-1.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:58:53.025201 crypto-screening-1.8.0/
+-rw-rw-rw-   0        0        0       98 2023-06-30 14:58:51.000000 crypto-screening-1.8.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2085 2023-06-30 14:58:53.025201 crypto-screening-1.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1264 2023-06-23 16:52:27.000000 crypto-screening-1.8.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.8.0/build.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:58:52.943381 crypto-screening-1.8.0/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-06-30 14:58:52.964370 crypto-screening-1.8.0/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-1.8.0/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-1.8.0/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0    10101 2023-06-30 14:50:05.000000 crypto-screening-1.8.0/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18811 2023-06-30 14:56:10.000000 crypto-screening-1.8.0/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-1.8.0/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.8.0/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5200 2023-06-30 14:44:13.000000 crypto-screening-1.8.0/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:58:52.969368 crypto-screening-1.8.0/crypto_screening/market/
+drwxrwxrwx   0        0        0        0 2023-06-30 14:58:52.986370 crypto-screening-1.8.0/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10832 2023-06-30 09:27:04.000000 crypto-screening-1.8.0/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      889 2023-06-30 09:21:25.000000 crypto-screening-1.8.0/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     8839 2023-06-30 09:21:46.000000 crypto-screening-1.8.0/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:58:53.024207 crypto-screening-1.8.0/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-1.8.0/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    13648 2023-06-30 10:44:18.000000 crypto-screening-1.8.0/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0     3391 2023-06-30 10:45:18.000000 crypto-screening-1.8.0/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    32765 2023-06-30 10:47:24.000000 crypto-screening-1.8.0/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    24997 2023-06-30 10:47:57.000000 crypto-screening-1.8.0/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0     5401 2023-06-30 10:44:43.000000 crypto-screening-1.8.0/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-1.8.0/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-1.8.0/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9898 2023-06-30 14:44:13.000000 crypto-screening-1.8.0/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-1.8.0/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:58:52.957371 crypto-screening-1.8.0/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2085 2023-06-30 14:58:52.000000 crypto-screening-1.8.0/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1053 2023-06-30 14:58:52.000000 crypto-screening-1.8.0/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 14:58:52.000000 crypto-screening-1.8.0/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-06-30 14:58:52.000000 crypto-screening-1.8.0/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-30 14:58:52.000000 crypto-screening-1.8.0/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-06-30 14:58:51.000000 crypto-screening-1.8.0/pyproject.toml
+-rw-rw-rw-   0        0        0       99 2023-06-28 09:56:21.000000 crypto-screening-1.8.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.8.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 14:58:53.025201 crypto-screening-1.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-06-30 14:58:22.000000 crypto-screening-1.8.0/setup.py
```

### Comparing `crypto-screening-1.7.0/PKG-INFO` & `crypto-screening-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.7.0
+Version: 1.8.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.7.0/README.md` & `crypto-screening-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.7.0/build.py` & `crypto-screening-1.8.0/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.7.0/crypto_screening/collect/assets.py` & `crypto-screening-1.8.0/crypto_screening/collect/assets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # assets.py
 
-from typing import Optional, Dict, Iterable, List, Union
+from typing import Optional, Dict, Iterable, Set, Union
 
 from crypto_screening.process import mutual_string_values
 from crypto_screening.symbols import symbol_to_parts, symbol_to_pair
 from crypto_screening.collect.exchanges import exchanges_data
 from crypto_screening.collect.symbols import (
     all_exchange_symbols, exchange_symbols
 )
@@ -27,15 +27,15 @@
     "exchanges_symbols_base_assets"
 ]
 
 def all_exchange_assets(
         exchange: str,
         separator: Optional[str] = None,
         adjust: Optional[bool] = True,
-) -> List[str]:
+) -> Set[str]:
     """
     Collects the symbols from the exchanges.
 
     :param exchange: The name of the exchange.
     :param adjust: The value to adjust the invalid exchanges.
     :param separator: The separator of the assets.
 
@@ -56,22 +56,22 @@
         # end if
 
         if quote not in assets:
             assets.append(quote)
         # end if
     # end for
 
-    return assets
+    return set(assets)
 # end all_exchange_assets
 
 def all_exchange_base_assets(
         exchange: str,
         separator: Optional[str] = None,
         adjust: Optional[bool] = True,
-) -> List[str]:
+) -> Set[str]:
     """
     Collects the symbols from the exchanges.
 
     :param exchange: The name of the exchange.
     :param adjust: The value to adjust the invalid exchanges.
     :param separator: The separator of the assets.
 
@@ -88,22 +88,22 @@
         base, _ = symbol_to_parts(symbol=symbol, separator=separator)
 
         if base not in assets:
             assets.append(base)
         # end if
     # end for
 
-    return assets
+    return set(assets)
 # end all_exchange_base_assets
 
 def all_exchange_quote_assets(
         exchange: str,
         separator: Optional[str] = None,
         adjust: Optional[bool] = True,
-) -> List[str]:
+) -> Set[str]:
     """
     Collects the symbols from the exchanges.
 
     :param exchange: The name of the exchange.
     :param adjust: The value to adjust the invalid exchanges.
     :param separator: The separator of the assets.
 
@@ -120,26 +120,26 @@
         _, quote = symbol_to_parts(symbol=symbol, separator=separator)
 
         if quote not in assets:
             assets.append(quote)
         # end if
     # end for
 
-    return assets
+    return set(assets)
 # end all_exchange_quote_assets
 
 def exchange_assets(
         exchange: str,
         separator: Optional[str] = None,
         adjust: Optional[bool] = True,
         bases: Optional[Iterable[str]] = None,
         quotes: Optional[Iterable[str]] = None,
         included: Optional[Iterable[str]] = None,
         excluded: Optional[Iterable[str]] = None
-) -> List[str]:
+) -> Set[str]:
     """
     Collects the assets from the exchanges.
 
     :param exchange: The name of the exchange.
     :param bases: The bases of the asset pairs.
     :param quotes: The quotes of the asset pairs.
     :param adjust: The value to adjust the invalid exchanges.
@@ -165,26 +165,26 @@
         # end if
 
         if quote not in assets:
             assets.append(quote)
         # end if
     # end for
 
-    return assets
+    return set(assets)
 # end exchange_assets
 
 def exchange_base_assets(
         exchange: str,
         separator: Optional[str] = None,
         adjust: Optional[bool] = True,
         bases: Optional[Iterable[str]] = None,
         quotes: Optional[Iterable[str]] = None,
         included: Optional[Iterable[str]] = None,
         excluded: Optional[Iterable[str]] = None
-) -> List[str]:
+) -> Set[str]:
     """
     Collects the assets from the exchanges.
 
     :param exchange: The name of the exchange.
     :param bases: The bases of the asset pairs.
     :param adjust: The value to adjust the invalid exchanges.
     :param quotes: The quotes of the asset pairs.
@@ -206,26 +206,26 @@
         base, _ = symbol_to_parts(symbol=symbol, separator=separator)
 
         if base not in assets:
             assets.append(base)
         # end if
     # end for
 
-    return assets
+    return set(assets)
 # end exchange_assets
 
 def exchange_quote_assets(
         exchange: str,
         separator: Optional[str] = None,
         adjust: Optional[bool] = True,
         bases: Optional[Iterable[str]] = None,
         quotes: Optional[Iterable[str]] = None,
         included: Optional[Iterable[str]] = None,
         excluded: Optional[Iterable[str]] = None
-) -> List[str]:
+) -> Set[str]:
     """
     Collects the assets from the exchanges.
 
     :param exchange: The name of the exchange.
     :param bases: The bases of the asset pairs.
     :param adjust: The value to adjust the invalid exchanges.
     :param quotes: The quotes of the asset pairs.
@@ -247,26 +247,26 @@
         _, quote = symbol_to_parts(symbol=symbol, separator=separator)
 
         if quote not in assets:
             assets.append(quote)
         # end if
     # end for
 
-    return assets
+    return set(assets)
 # end exchange_assets
 
 def exchanges_assets(
         exchanges: Optional[Iterable[str]] = None,
         adjust: Optional[bool] = True,
         separator: Optional[str] = None,
         bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
-) -> Dict[str, List[str]]:
+) -> Dict[str, Set[str]]:
     """
     Collects the symbols from the exchanges.
 
     :param exchanges: The exchanges.
     :param quotes: The quotes of the asset pairs.
     :param bases: The bases of the asset pairs.
     :param excluded: The excluded symbols.
@@ -289,15 +289,15 @@
         exchanges: Optional[Iterable[str]] = None,
         adjust: Optional[bool] = True,
         separator: Optional[str] = None,
         bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
-) -> Dict[str, List[str]]:
+) -> Dict[str, Set[str]]:
     """
     Collects the symbols from the exchanges.
 
     :param exchanges: The exchanges.
     :param quotes: The quotes of the asset pairs.
     :param bases: The bases of the asset pairs.
     :param excluded: The excluded symbols.
@@ -320,15 +320,15 @@
         exchanges: Optional[Iterable[str]] = None,
         adjust: Optional[bool] = True,
         separator: Optional[str] = None,
         bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
-) -> Dict[str, List[str]]:
+) -> Dict[str, Set[str]]:
     """
     Collects the symbols from the exchanges.
 
     :param exchanges: The exchanges.
     :param quotes: The quotes of the asset pairs.
     :param bases: The bases of the asset pairs.
     :param excluded: The excluded symbols.
@@ -346,15 +346,15 @@
         adjust=adjust, separator=separator, bases=bases, included=included
     )
 # end exchanges_quote_assets
 
 def exchanges_symbols_assets(
         data: Dict[str, Iterable[str]],
         separator: Optional[str] = None
-) -> Dict[str, List[str]]:
+) -> Dict[str, Set[str]]:
     """
     Finds the currencies from the screeners.
 
     :param data: The data to process.
     :param separator: The separator of the assets.
 
     :return: The currencies from the screeners.
@@ -388,15 +388,15 @@
 
     return results
 # end exchanges_symbols_assets
 
 def exchanges_symbols_base_assets(
         data: Dict[str, Iterable[str]],
         separator: Optional[str] = None
-) -> Dict[str, List[str]]:
+) -> Dict[str, Set[str]]:
     """
     Finds the currencies from the screeners.
 
     :param data: The data to process.
     :param separator: The separator of the assets.
 
     :return: The currencies from the screeners.
@@ -419,15 +419,15 @@
         for exchange, symbols in result.items()
     }
 # end exchanges_symbols_base_assets
 
 def exchanges_symbols_quote_assets(
         data: Dict[str, Iterable[str]],
         separator: Optional[str] = None
-) -> Dict[str, List[str]]:
+) -> Dict[str, Set[str]]:
     """
     Finds the currencies from the screeners.
 
     :param data: The data to process.
     :param separator: The separator of the assets.
 
     :return: The currencies from the screeners.
@@ -455,15 +455,15 @@
         adjust: Optional[bool] = True,
         separator: Optional[str] = None,
         bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         data: Optional[Dict[str, Iterable[str]]] = None
-) -> Dict[str, List[str]]:
+) -> Dict[str, Set[str]]:
     """
     Collects the symbols from the exchanges.
 
     :param exchanges: The exchanges.
     :param quotes: The quotes of the asset pairs.
     :param bases: The bases of the asset pairs.
     :param excluded: The excluded symbols.
@@ -488,15 +488,15 @@
         adjust: Optional[bool] = True,
         separator: Optional[str] = None,
         bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         data: Optional[Dict[str, Iterable[str]]] = None
-) -> Dict[str, List[str]]:
+) -> Dict[str, Set[str]]:
     """
     Collects the symbols from the exchanges.
 
     :param exchanges: The exchanges.
     :param quotes: The quotes of the asset pairs.
     :param bases: The bases of the asset pairs.
     :param excluded: The excluded symbols.
@@ -521,15 +521,15 @@
         adjust: Optional[bool] = True,
         separator: Optional[str] = None,
         bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         data: Optional[Dict[str, Iterable[str]]] = None
-) -> Dict[str, List[str]]:
+) -> Dict[str, Set[str]]:
     """
     Collects the symbols from the exchanges.
 
     :param exchanges: The exchanges.
     :param quotes: The quotes of the asset pairs.
     :param bases: The bases of the asset pairs.
     :param excluded: The excluded symbols.
```

### Comparing `crypto-screening-1.7.0/crypto_screening/collect/exchanges.py` & `crypto-screening-1.8.0/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.7.0/crypto_screening/collect/screeners.py` & `crypto-screening-1.8.0/crypto_screening/collect/screeners.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # screeners.py
 
+from dataclasses import dataclass
 from typing import (
     Optional, Dict, Iterable,
-    List, Union, Tuple
+    Set, Union, Tuple, List
 )
 
 from crypto_screening.symbols import symbol_to_pair
 from crypto_screening.collect.symbols import (
     matching_symbol_pair, MarketSymbolSignature
 )
 from crypto_screening.market.screeners.base import (
@@ -59,27 +60,27 @@
 ExchangesAssetMatches = Union[Dict[Iterable[str], AssetMatches], AssetMatches]
 
 def matching_screener_pairs(
         screeners: Iterable[BaseScreener],
         matches: Optional[ExchangesAssetMatches] = None,
         separator: Optional[str] = None,
         empty: Optional[bool] = True
-) -> List[Tuple[BaseScreener, BaseScreener]]:
+) -> Set[Tuple[BaseScreener, BaseScreener]]:
     """
     Checks if the screeners are valid with the matching currencies.
 
     :param screeners: The screeners.
     :param matches: The currencies.
     :param separator: The separator of the assets.
     :param empty: Allows empty screeners.
 
     :return: The validation value for the symbols.
     """
 
-    pairs = []
+    pairs: List[Tuple[BaseScreener, BaseScreener]] = []
 
     if not empty:
         screeners = remove_empty_screeners(screeners=screeners)
     # end if
 
     for screener1 in screeners:
         for screener2 in screeners:
@@ -98,52 +99,31 @@
                 separator=separator
             ):
                 pairs.append((screener1, screener2))
             # end if
         # end for
     # end for
 
-    return pairs
+    return set(pairs)
 # end matching_screener_pairs
 
+@dataclass(repr=False, slots=True)
 class MarketScreenerSignature(MarketSymbolSignature):
     """A class to represent the data for the execution of a trade."""
 
-    __slots__ = "screener",
-
-    def __init__(
-            self,
-            asset: str,
-            currency: str,
-            exchange: str,
-            screener: Optional[BaseScreener] = None
-    ) -> None:
-        """
-        Defines the class attributes.
-
-        :param asset: The traded asset.
-        :param currency: The currency to trade the asset with.
-        :param exchange: The exchange platform.
-        """
-
-        super().__init__(
-            asset=asset, currency=currency, exchange=exchange
-        )
-
-        self.screener = screener
-    # end __init__
+    screener: Optional[BaseScreener] = None
 # end MarketScreenerSignature
 
 def matching_screener_signatures(
-        data: Optional[List[Tuple[BaseScreener, BaseScreener]]] = None,
+        data: Optional[Set[Tuple[BaseScreener, BaseScreener]]] = None,
         screeners: Optional[Iterable[BaseScreener]] = None,
         matches: Optional[ExchangesAssetMatches] = None,
         separator: Optional[str] = None,
         empty: Optional[bool] = True
-) -> List[Tuple[MarketScreenerSignature, MarketScreenerSignature]]:
+) -> Set[Tuple[MarketScreenerSignature, MarketScreenerSignature]]:
     """
     Checks if the screeners are valid with the matching currencies.
 
     :param data: The data for the pairs.
     :param screeners: The screeners.
     :param matches: The currencies.
     :param separator: The separator of the assets.
@@ -155,18 +135,18 @@
     if (data is None) and (screeners is None):
         raise ValueError(
             f"One of 'screeners' and 'data' parameters must be given, "
             f"when 'data' is superior to 'screeners'."
         )
 
     elif (not screeners) and (not data):
-        return []
+        return set()
     # end if
 
-    pairs = []
+    pairs: List[Tuple[MarketScreenerSignature, MarketScreenerSignature]] = []
 
     data = data or matching_screener_pairs(
         screeners=screeners, matches=matches,
         separator=separator, empty=empty
     )
 
     for screener1, screener2 in data:
@@ -185,37 +165,37 @@
                     exchange=screener2.exchange,
                     screener=screener2
                 )
             )
         )
     # end for
 
-    return pairs
+    return set(pairs)
 # end matching_screener_signatures
 
 def live_screeners(
         screeners: Iterable[Union[BaseScreener, BaseMultiScreener]]
-) -> List[Union[BaseScreener, BaseMultiScreener]]:
+) -> Set[Union[BaseScreener, BaseMultiScreener]]:
     """
     Returns a list of all the live create_screeners.
 
     :param screeners: The create_screeners to search from.
 
     :return: A list the live create_screeners.
     """
 
-    return [
+    return {
         screener for screener in screeners
         if (
             screener.screening and (
                 isinstance(screener, BaseMultiScreener) or
                 len(screener.market) > 0
             )
         )
-    ]
+    }
 # end live_screeners
 
 def structure_screeners(
         screeners: Iterable[BaseScreener]
 ) -> Dict[str, Dict[str, List[BaseScreener]]]:
     """
     Structures the screener objects by exchanges and symbols
@@ -269,31 +249,31 @@
 
     return [
         screener for screener in screeners
         if len(screener.market) > 0
     ]
 # end remove_empty_screeners
 
-def screeners_exchanges_symbols(screeners: Iterable[BaseScreener]) -> Dict[str, List[str]]:
+def screeners_exchanges_symbols(screeners: Iterable[BaseScreener]) -> Dict[str, Set[str]]:
     """
     Collects the structure of the screeners exchanges and symbols.
 
     :param screeners: The screeners to process.
 
     :return: The collected structure of exchanges and symbols.
     """
 
-    data = {}
+    data: Dict[str, Set[str]] = {}
 
     for screener in screeners:
-        data.setdefault(screener.exchange, []).append(screener.symbol)
+        data.setdefault(screener.exchange, set()).add(screener.symbol)
     # end for
 
     return {
-        exchange: list(set(symbols))
+        exchange: symbols
         for exchange, symbols in data.items()
         if symbols
     }
 # end screeners_exchanges_symbols
 
 def structure_exchanges_symbols_screeners(
         screeners: Iterable[BaseScreener]
@@ -302,15 +282,15 @@
     Structures the screener objects by exchanges and symbols
 
     :param screeners: The screeners to structure.
 
     :return: The structure of the screeners.
     """
 
-    structure = {}
+    structure: Dict[str, Dict[str, List[BaseScreener]]] = {}
 
     for screener in screeners:
         (
             structure.
             setdefault(screener.exchange, {}).
             setdefault(screener.symbol, [])
         ).append(screener)
@@ -326,15 +306,15 @@
     Structures the screener objects by exchanges and symbols
 
     :param screeners: The screeners to structure.
 
     :return: The structure of the screeners.
     """
 
-    structure = {}
+    structure: Dict[str, Dict[str, BaseScreener]] = {}
 
     for screener in screeners:
         (
             structure.
             setdefault(screener.exchange, {}).
             setdefault(screener.symbol, screener)
         )
@@ -350,15 +330,15 @@
     Gathers the base screeners.
 
     :param screeners: The screeners to process.
 
     :return: The gathered base screeners.
     """
 
-    checked_screeners = []
+    checked_screeners: List[BaseScreener] = []
 
     for screener in screeners:
         if isinstance(screener, BaseScreener):
             checked_screeners.append(screener)
 
         elif isinstance(screener, BaseMultiScreener):
             checked_screeners.extend(screener.screeners)
```

### Comparing `crypto-screening-1.7.0/crypto_screening/collect/symbols.py` & `crypto-screening-1.8.0/crypto_screening/collect/symbols.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # symbols.py
 
+from dataclasses import dataclass
 from typing import (
     Optional, Dict, Iterable,
-    List, Union, Tuple
+    Set, Union, Tuple
 )
 
 from represent import BaseModel
 
 
 from crypto_screening.process import (
     find_string_value, upper_string_values,
@@ -38,15 +39,15 @@
 def include_symbols(
         symbols: Iterable[str],
         separator: Optional[str] = None,
         adjust: Optional[bool] = True,
         bases: Optional[Iterable[str]] = None,
         quotes: Optional[Iterable[str]] = None,
         included: Optional[Iterable[str]] = None
-) -> List[str]:
+) -> Set[str]:
     """
     Removes all symbols with not matching base or quote.
 
     :param symbols: The symbols to filter.
     :param separator: The separator for the symbols.
     :param bases: The bases to include.
     :param adjust: The value to adjust the invalid exchanges.
@@ -87,25 +88,25 @@
             (find_string_value(value=base, values=bases) in bases) or
             (find_string_value(value=quote, values=quotes) in quotes)
         ):
             saved.append(symbol)
         # end if
     # end for
 
-    return saved
+    return set(saved)
 # end include_symbols
 
 def exclude_symbols(
         symbols: Iterable[str],
         separator: Optional[str] = None,
         adjust: Optional[bool] = True,
         bases: Optional[Iterable[str]] = None,
         quotes: Optional[Iterable[str]] = None,
         excluded: Optional[Iterable[str]] = None
-) -> List[str]:
+) -> Set[str]:
     """
     Removes all symbols with the matching base or quote.
 
     :param symbols: The symbols to filter.
     :param separator: The separator for the symbols.
     :param bases: The bases to exclude.
     :param quotes: The quotes to exclude.
@@ -148,36 +149,36 @@
         ):
             continue
         # end if
 
         saved.append(symbol)
     # end for
 
-    return saved
+    return set(saved)
 # end exclude_symbols
 
 def include_exchanges_symbols(
         data: Dict[str, Iterable[str]],
         bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
-) -> Dict[str, List[str]]:
+) -> Dict[str, Set[str]]:
     """
     Removes all symbols with not matching base or quote.
 
     :param data: The data to filter.
     :param bases: The bases to include.
     :param quotes: The quotes to include.
     :param included: The symbols to include.
 
     :return: The filtered symbols.
     """
 
     if all(value is None for value in (bases, quotes, included)):
-        return {exchange: list(symbols) for exchange, symbols in data.items()}
+        return {exchange: set(symbols) for exchange, symbols in data.items()}
     # end if
 
     if not isinstance(quotes, dict):
         saved_quotes = quotes
         quotes = {exchange: saved_quotes for exchange in data}
     # end if
 
@@ -205,28 +206,28 @@
 # end include_exchanges_symbols
 
 def exclude_exchanges_symbols(
         data: Dict[str, Iterable[str]],
         bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
-) -> Dict[str, List[str]]:
+) -> Dict[str, Set[str]]:
     """
     Removes all symbols with the matching base or quote.
 
     :param data: The data to filter.
     :param bases: The bases to exclude.
     :param quotes: The quotes to exclude.
     :param excluded: The symbols to exclude.
 
     :return: The filtered symbols.
     """
 
     if all(value is None for value in (bases, quotes, excluded)):
-        return {exchange: list(symbols) for exchange, symbols in data.items()}
+        return {exchange: set(symbols) for exchange, symbols in data.items()}
     # end if
 
     if not isinstance(quotes, dict):
         saved_quotes = quotes
         quotes = {exchange: saved_quotes for exchange in data}
     # end if
 
@@ -254,15 +255,15 @@
 # end exclude_exchanges_symbols
 
 def all_exchange_symbols(
         exchange: str,
         separator: Optional[str] = None,
         adjust: Optional[bool] = True,
         test: Optional[bool] = False
-) -> List[str]:
+) -> Set[str]:
     """
     Collects the symbols from the exchanges.
 
     :param exchange: The name of the exchange.
     :param adjust: The value to adjust the invalid exchanges.
     :param separator: The separator of the assets.
     :param test: Include test assets.
@@ -312,23 +313,23 @@
 
             else:
                 raise e
             # end if
         # end try
     # end for
 
-    return symbols
+    return set(symbols)
 # end all_exchange_symbols
 
 def all_exchanges_symbols(
         exchanges: Iterable[str],
         separator: Optional[str] = None,
         adjust: Optional[bool] = True,
         test: Optional[bool] = False
-) -> Dict[str, List[str]]:
+) -> Dict[str, Set[str]]:
     """
     Collects the symbols from the exchanges.
 
     :param exchanges: The name of the exchange.
     :param adjust: The value to adjust the invalid exchanges.
     :param separator: The separator of the assets.
     :param test: Include test assets.
@@ -349,15 +350,15 @@
         exchange: Optional[str] = None,
         separator: Optional[str] = None,
         adjust: Optional[bool] = True,
         bases: Optional[Iterable[str]] = None,
         quotes: Optional[Iterable[str]] = None,
         included: Optional[Iterable[str]] = None,
         excluded: Optional[Iterable[str]] = None
-) -> List[str]:
+) -> Set[str]:
     """
     Collects the symbols from the exchanges.
 
     :param exchange: The name of the exchange.
     :param quotes: The quotes of the asset pairs.
     :param adjust: The value to adjust the invalid exchanges.
     :param bases: The bases of the asset pairs.
@@ -368,35 +369,31 @@
     :return: The data of the exchanges.
     """
 
     symbols = all_exchange_symbols(
         exchange=exchange, adjust=adjust, separator=separator
     )
 
-    return list(
-        set(
-            exclude_symbols(
-                symbols=include_symbols(
-                    symbols=symbols, included=included,
-                    bases=bases, quotes=quotes, separator=separator
-                ), excluded=excluded, separator=separator, adjust=adjust
-            )
-        )
+    return exclude_symbols(
+        symbols=include_symbols(
+            symbols=symbols, included=included,
+            bases=bases, quotes=quotes, separator=separator
+        ), excluded=excluded, separator=separator, adjust=adjust
     )
 # end exchange_symbols
 
 def exchanges_symbols(
         exchanges: Optional[Iterable[str]] = None,
         adjust: Optional[bool] = True,
         separator: Optional[str] = None,
         bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
-) -> Dict[str, List[str]]:
+) -> Dict[str, Set[str]]:
     """
     Collects the symbols from the exchanges.
 
     :param exchanges: The exchanges.
     :param quotes: The quotes of the asset pairs.
     :param excluded: The excluded symbols.
     :param adjust: The value to adjust the invalid exchanges.
@@ -419,15 +416,15 @@
         adjust: Optional[bool] = True,
         separator: Optional[str] = None,
         bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         data: Optional[Dict[str, Iterable[str]]] = None
-) -> Dict[str, List[str]]:
+) -> Dict[str, Set[str]]:
     """
     Collects the symbols from the exchanges.
 
     :param exchanges: The exchanges.
     :param quotes: The quotes of the asset pairs.
     :param excluded: The excluded symbols.
     :param adjust: The value to adjust the invalid exchanges.
@@ -494,15 +491,15 @@
             return False
         # end if
     # end for
 
     return False
 # end matching_symbol_pair
 
-ExchangeSymbolPairs = List[Tuple[Tuple[str, str], Tuple[str, str]]]
+ExchangeSymbolPairs = Set[Tuple[Tuple[str, str], Tuple[str, str]]]
 ExchangesAssetMatches = Union[Dict[Iterable[str], AssetMatches], AssetMatches]
 
 def matching_symbol_pairs(
         data: Dict[str, Iterable[str]],
         matches: Optional[ExchangesAssetMatches] = None,
         separator: Optional[str] = None
 ) -> ExchangeSymbolPairs:
@@ -547,48 +544,32 @@
                 pairs.append(
                     ((exchange1, symbol1), (exchange2, symbol2))
                 )
             # end if
         # end for
     # end for
 
-    return pairs
+    return set(pairs)
 # end matching_symbol_pairs
 
+@dataclass(repr=False, slots=True)
 class MarketSymbolSignature(BaseModel):
     """A class to represent the data for the execution of a trade."""
 
-    __slots__ = "asset", "currency", "exchange"
-
-    def __init__(
-            self,
-            asset: str,
-            currency: str,
-            exchange: str
-    ) -> None:
-        """
-        Defines the class attributes.
-
-        :param asset: The traded asset.
-        :param currency: The currency to trade the asset with.
-        :param exchange: The exchange platform.
-        """
-
-        self.asset = asset
-        self.exchange = exchange
-        self.currency = currency
-    # end __init__
+    asset: str
+    currency: str
+    exchange: str
 # end MarketPairSignature
 
 def matching_symbol_signatures(
         pairs: Optional[ExchangeSymbolPairs] = None,
         data: Optional[Dict[str, Iterable[str]]] = None,
         matches: Optional[ExchangesAssetMatches] = None,
         separator: Optional[str] = None
-) -> List[Tuple[MarketSymbolSignature, MarketSymbolSignature]]:
+) -> Set[Tuple[MarketSymbolSignature, MarketSymbolSignature]]:
     """
     Checks if the screeners are valid with the matching currencies.
 
     :param data: The data for the pairs.
     :param pairs: The pairs' data.
     :param matches: The currencies.
     :param separator: The separator of the assets.
@@ -599,15 +580,15 @@
     if (data is None) and (pairs is None):
         raise ValueError(
             f"One of 'pairs' and 'data' parameters must be given, "
             f"when 'pairs' is superior to 'data'."
         )
 
     elif (not pairs) and (not data):
-        return []
+        return set()
     # end if
 
     new_pairs = []
 
     pairs = pairs or matching_symbol_pairs(
         data=data, matches=matches, separator=separator
     )
@@ -626,9 +607,9 @@
                     asset=asset2, currency=currency2,
                     exchange=exchange2
                 )
             )
         )
     # end for
 
-    return new_pairs
+    return set(new_pairs)
 # end matching_symbol_signatures
```

### Comparing `crypto-screening-1.7.0/crypto_screening/dataset.py` & `crypto-screening-1.8.0/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.7.0/crypto_screening/market/foundation/data.py` & `crypto-screening-1.8.0/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.7.0/crypto_screening/market/foundation/protocols.py` & `crypto-screening-1.8.0/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.7.0/crypto_screening/market/foundation/waiting.py` & `crypto-screening-1.8.0/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.7.0/crypto_screening/market/screeners/base.py` & `crypto-screening-1.8.0/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.7.0/crypto_screening/market/screeners/container.py` & `crypto-screening-1.8.0/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.7.0/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-1.8.0/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.7.0/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-1.8.0/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.7.0/crypto_screening/market/screeners/recorder.py` & `crypto-screening-1.8.0/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.7.0/crypto_screening/market/waiting.py` & `crypto-screening-1.8.0/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.7.0/crypto_screening/process.py` & `crypto-screening-1.8.0/crypto_screening/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # process.py
 
-from typing import Iterable, List, Optional, Dict
+from typing import Iterable, List, Set, Optional, Dict
 
 __all__ = [
     "find_string_value",
     "upper_string_values",
     "lower_string_values",
     "mutual_string_values"
 ]
@@ -60,15 +60,15 @@
     return [value.lower() for value in values]
 # end lower_string_values
 
 def mutual_string_values(
         data: Dict[str, Iterable[str]],
         minimum: Optional[int] = None,
         maximum: Optional[int] = None
-) -> Dict[str, List[str]]:
+) -> Dict[str, Set[str]]:
     """
     Collects the symbols from the exchanges.
 
     :param data: The exchanges' data.
     :param minimum: The minimum amount of counts for a value.
     :param maximum: The maximum amount of counts for a value.
 
@@ -88,13 +88,13 @@
     for key in data:
         for value in data[key]:
             values[value] = values.setdefault(value, 0) + 1
         # end for
     # end for
 
     return {
-        key: [
+        key: {
             value for value in data[key]
             if minimum <= values.get(value, 0) <= maximum
-        ] for key in data
+        } for key in data
     }
 # end mutual_exchanges_assets
```

### Comparing `crypto-screening-1.7.0/crypto_screening/symbols.py` & `crypto-screening-1.8.0/crypto_screening/symbols.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
         self.base = base
         self.quote = quote
 
         self.parts = (self.base, self.quote)
     # end __init__
 
-    def __getitem__(self, item: Union[slice, int]) -> Union[str, Iterable[str]]:
+    def __getitem__(self, item: Union[slice, int]) -> Union[str, Tuple[str, str]]:
         """
         Returns the items.
 
         :param item: The slice item.
 
         :return: The items in the object to get with the slice.
         """
@@ -94,15 +94,15 @@
 
         :return: The length of the assets.
         """
 
         return len(self.parts)
     # end __len__
 
-    def __iter__(self) -> Iterable[str]:
+    def __iter__(self) -> Tuple[str, str]:
         """
         Returns the object as an iterable.
 
         :return: The iterable object.
         """
 
         yield from self.parts
```

### Comparing `crypto-screening-1.7.0/crypto_screening/validate.py` & `crypto-screening-1.8.0/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.7.0/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-1.8.0/crypto_screening.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.7.0
+Version: 1.8.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.7.0/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-1.8.0/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.7.0/pyproject.toml` & `crypto-screening-1.8.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '1.7.0'
+version = '1.8.0'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-1.7.0/setup.py` & `crypto-screening-1.8.0/setup.py`

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
-        version='1.7.0',
+        version='1.8.0',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

