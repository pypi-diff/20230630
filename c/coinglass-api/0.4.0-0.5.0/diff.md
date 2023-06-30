# Comparing `tmp/coinglass_api-0.4.0.tar.gz` & `tmp/coinglass_api-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coinglass_api-0.4.0.tar", max compression
+gzip compressed data, was "coinglass_api-0.5.0.tar", max compression
```

## Comparing `coinglass_api-0.4.0.tar` & `coinglass_api-0.5.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-01-15 20:06:02.595582 coinglass_api-0.4.0/LICENSE.md
--rw-r--r--   0        0        0     4133 2023-05-16 13:38:17.827854 coinglass_api-0.4.0/README.md
--rw-r--r--   0        0        0       57 2023-01-15 18:42:45.746707 coinglass_api-0.4.0/coinglass_api/__init__.py
--rw-r--r--   0        0        0    14259 2023-05-16 13:36:00.313830 coinglass_api-0.4.0/coinglass_api/api.py
--rw-r--r--   0        0        0      809 2023-05-16 13:38:31.432471 coinglass_api-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4877 1970-01-01 00:00:00.000000 coinglass_api-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-01-15 20:06:02.595582 coinglass_api-0.5.0/LICENSE.md
+-rw-r--r--   0        0        0     4267 2023-06-30 12:39:55.834401 coinglass_api-0.5.0/README.md
+-rw-r--r--   0        0        0       57 2023-01-15 18:42:45.746707 coinglass_api-0.5.0/coinglass_api/__init__.py
+-rw-r--r--   0        0        0    17895 2023-06-30 12:23:48.647991 coinglass_api-0.5.0/coinglass_api/api.py
+-rw-r--r--   0        0        0      809 2023-06-30 12:28:58.463408 coinglass_api-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5011 1970-01-01 00:00:00.000000 coinglass_api-0.5.0/PKG-INFO
```

### Comparing `coinglass_api-0.4.0/LICENSE.md` & `coinglass_api-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `coinglass_api-0.4.0/README.md` & `coinglass_api-0.5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Coinglass API
 [![PyPi version](https://img.shields.io/pypi/v/coinglass-api)](https://pypi.python.org/pypi/coinglass-api/)
-[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100//)
-[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3110//)
+[![Downloads](https://pepy.tech/badge/coinglass-api)](https://pepy.tech/project/coinglass-api)
 [![codecov](https://codecov.io/gh/dineshpinto/coinglass-api/branch/main/graph/badge.svg?token=XTJRRU2W1T)](https://codecov.io/gh/dineshpinto/coinglass-api)
+[![API unittest](https://github.com/dineshpinto/coinglass-api/actions/workflows/api_unitests.yml/badge.svg)](https://github.com/dineshpinto/coinglass-api/actions/workflows/api_unitests.yml)
 
 ## Unofficial Python client for Coinglass API
 
 Wrapper around the [Coinglass API](https://coinglass.com/pricing) to fetch data about the crypto markets.
-All data is output in pandas DataFrames (single or multi-index) and all time series data uses a DateTimeIndex.
+All data is output in pandas DataFrames (single or multi-index) and all time series data uses a `DateTimeIndex`.
 
-**Note**: Currently only supports the `indicator` API endpoint.
+**Note**: Currently supports the `indicator` and `index` API endpoints.
 
 ![Example Plot](https://github.com/dineshpinto/coinglass-api/blob/main/examples/example_plot.jpg?raw=true)
 
 ## Installation
 
 ```bash
 pip install coinglass-api
@@ -42,14 +42,19 @@
 liq_ohlc_eth_dydx = cg.liquidation_pair(ex="dYdX", pair="ETH-USD", interval="h4")
 
 # Get liquidation data for BTC
 liq_btc = cg.liquidation_symbol(symbol="BTC", interval="h4")
 
 # Get long/short ratios for BTC
 lsr_btc = cg.long_short_symbol(symbol="BTC", interval="h4")
+
+# Get GBTC market history
+gbtc_history = cg.grayscale_market_history()
+
+# and more...
 ```
 
 ## Examples
 
 ```
 >>> cg.funding(ex="dYdX", pair="ETH-USD", interval="h8").head()
 ```
```

### Comparing `coinglass_api-0.4.0/coinglass_api/api.py` & `coinglass_api-0.5.0/coinglass_api/api.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,35 +7,47 @@
 
     def __init__(self, coinglass_secret: str):
         """
         Args:
             coinglass_secret: key from Coinglass, get one at https://www.coinglass.com/pricing
         """
         self.__coinglass_secret = coinglass_secret
-        self._base_url = "https://open-api.coinglass.com/public/v2/indicator/"
+        self._base_url = "https://open-api.coinglass.com/public/v2/"
         self._session = requests.Session()
 
     def _get(self, endpoint: str, params: dict = None) -> dict:
         headers = {
             "accept": "application/json",
             "coinglassSecret": self.__coinglass_secret
         }
         url = self._base_url + endpoint
         return self._session.request('GET', url, params=params, headers=headers, timeout=30).json()
 
     @staticmethod
-    def _create_dataframe(data: list[dict], time_col: str) -> pd.DataFrame:
+    def _create_dataframe(
+            data: list[dict],
+            time_col: str,
+            unit: str | None = "ms",
+            cast_objects_to_numeric: bool = False
+    ) -> pd.DataFrame:
         """ Create pandas DataFrame from list of dicts """
         df = pd.DataFrame(data)
-        df["time"] = pd.to_datetime(df[time_col], unit="ms")
+        if time_col == "time":
+            df.rename(columns={"time": "t"}, inplace=True)
+            time_col = "t"
+        df["time"] = pd.to_datetime(df[time_col], unit=unit)
         df.drop(columns=[time_col], inplace=True)
         df.set_index("time", inplace=True, drop=True)
 
         if "t" in df.columns:
             df.drop(columns=["t"], inplace=True)
+
+        if cast_objects_to_numeric:
+            cols = df.columns[df.dtypes.eq('object')]
+            df[cols] = df[cols].apply(pd.to_numeric)
         return df
 
     @staticmethod
     def _check_for_errors(response: dict) -> None:
         """ Check for errors in response """
         if not response["success"]:
             raise Exception(f"Code {response['code']}: {response['msg']}")
@@ -60,15 +72,15 @@
             start_time: start time in milliseconds
             end_time: end time in milliseconds
 
         Returns:
             pandas DataFrame with funding rate
         """
         response = self._get(
-            endpoint="funding",
+            endpoint="indicator/funding",
             params={"ex": ex, "pair": pair, "interval": interval, "limit": limit,
                     "start_time": start_time, "end_time": end_time}
         )
         self._check_for_errors(response)
         data = response["data"]
         return self._create_dataframe(data, time_col="createTime")
 
@@ -92,15 +104,15 @@
             start_time: start time in milliseconds
             end_time: end time in milliseconds
 
         Returns:
             pandas DataFrame with funding rate in OHLC format for an exchange pair
         """
         response = self._get(
-            endpoint="funding_ohlc",
+            endpoint="indicator/funding_ohlc",
             params={"ex": ex, "pair": pair, "interval": interval, "limit": limit,
                     "start_time": start_time, "end_time": end_time}
         )
         self._check_for_errors(response)
         data = response["data"]
         return self._create_dataframe(data, time_col="t")
 
@@ -122,15 +134,15 @@
             start_time: start time in milliseconds
             end_time: end time in milliseconds
 
         Returns:
             pandas DataFrame with funding rate
         """
         response = self._get(
-            endpoint="funding_avg",
+            endpoint="indicator/funding_avg",
             params={"symbol": symbol, "interval": interval, "limit": limit,
                     "start_time": start_time, "end_time": end_time}
         )
         self._check_for_errors(response)
         data = response["data"]
         return self._create_dataframe(data, time_col="createTime")
 
@@ -154,15 +166,15 @@
             start_time: start time in milliseconds
             end_time: end time in milliseconds
 
         Returns:
             pandas DataFrame with open interest in OHLC format for an exchange pair
         """
         response = self._get(
-            endpoint="open_interest_ohlc",
+            endpoint="indicator/open_interest_ohlc",
             params={"ex": ex, "pair": pair, "interval": interval, "limit": limit,
                     "start_time": start_time, "end_time": end_time}
         )
         self._check_for_errors(response)
         data = response["data"]
         return self._create_dataframe(data, time_col="t")
 
@@ -184,15 +196,15 @@
             start_time: start time in milliseconds
             end_time: end time in milliseconds
 
         Returns:
             pandas DataFrame with aggregated open interest in OHLC format
         """
         response = self._get(
-            endpoint="open_interest_aggregated_ohlc",
+            endpoint="indicator/open_interest_aggregated_ohlc",
             params={"symbol": symbol, "interval": interval, "limit": limit,
                     "start_time": start_time, "end_time": end_time}
         )
         self._check_for_errors(response)
         data = response["data"]
         return self._create_dataframe(data, time_col="t")
 
@@ -214,15 +226,15 @@
             start_time: start time in milliseconds
             end_time: end time in milliseconds
 
         Returns:
             pandas DataFrame with liquidation data
         """
         response = self._get(
-            endpoint="liquidation_symbol",
+            endpoint="indicator/liquidation_symbol",
             params={"symbol": symbol, "interval": interval, "limit": limit,
                     "start_time": start_time, "end_time": end_time}
         )
         self._check_for_errors(response)
         data = response["data"]
         return self._create_dataframe(data, time_col="createTime")
 
@@ -246,15 +258,15 @@
             start_time: start time in milliseconds
             end_time: end time in milliseconds
 
         Returns:
             pandas DataFrame with liquidation data for an exchange pair
         """
         response = self._get(
-            endpoint="liquidation_pair",
+            endpoint="indicator/liquidation_pair",
             params={"ex": ex, "pair": pair, "interval": interval, "limit": limit,
                     "start_time": start_time, "end_time": end_time}
         )
         self._check_for_errors(response)
         data = response["data"]
         return self._create_dataframe(data, time_col="t")
 
@@ -278,15 +290,15 @@
             start_time: start time in milliseconds
             end_time: end time in milliseconds
 
         Returns:
             pandas DataFrame with long/short ratio for an exchange pair
         """
         response = self._get(
-            endpoint="long_short_accounts",
+            endpoint="indicator/long_short_accounts",
             params={"ex": ex, "pair": pair, "interval": interval, "limit": limit,
                     "start_time": start_time, "end_time": end_time}
         )
         self._check_for_errors(response)
         data = response["data"]
         return self._create_dataframe(data, time_col="createTime")
 
@@ -308,15 +320,15 @@
             start_time: start time in milliseconds
             end_time: end time in milliseconds
 
         Returns:
             pandas DataFrame with long/short ratio
         """
         response = self._get(
-            endpoint="long_short_symbol",
+            endpoint="indicator/long_short_symbol",
             params={"symbol": symbol, "interval": interval, "limit": limit,
                     "start_time": start_time, "end_time": end_time}
         )
         self._check_for_errors(response)
         data = response["data"]
         return self._create_dataframe(data, time_col="t")
 
@@ -340,15 +352,15 @@
             start_time: start time in milliseconds
             end_time: end time in milliseconds
 
         Returns:
             pandas DataFrame with top accounts long/short ratio for an exchange pair
         """
         response = self._get(
-            endpoint="top_long_short_account_ratio",
+            endpoint="indicator/top_long_short_account_ratio",
             params={"ex": ex, "pair": pair, "interval": interval, "limit": limit,
                     "start_time": start_time, "end_time": end_time}
         )
         self._check_for_errors(response)
         data = response["data"]
         return self._create_dataframe(data, time_col="createTime")
 
@@ -372,14 +384,102 @@
             start_time: start time in milliseconds
             end_time: end time in milliseconds
 
         Returns:
             pandas DataFrame with top positions long/short ratio for an exchange pair
         """
         response = self._get(
-            endpoint="top_long_short_position_ratio",
+            endpoint="indicator/top_long_short_position_ratio",
             params={"ex": ex, "pair": pair, "interval": interval, "limit": limit,
                     "start_time": start_time, "end_time": end_time}
         )
         self._check_for_errors(response)
         data = response["data"]
         return self._create_dataframe(data, time_col="createTime")
+
+    def bitcoin_bubble_index(self) -> pd.DataFrame:
+        response = self._get(
+            endpoint="index/bitcoin_bubble_index",
+        )
+        self._check_for_errors(response)
+        data = response["data"]
+        return self._create_dataframe(data, time_col="time", unit=None)
+
+    def ahr999(self) -> pd.DataFrame:
+        response = self._get(
+            endpoint="index/ahr999",
+        )
+        self._check_for_errors(response)
+        data = response["data"]
+        return self._create_dataframe(data, time_col="date", unit=None)
+
+    def tow_year_ma_multiplier(self) -> pd.DataFrame:
+        response = self._get(
+            endpoint="index/tow_year_MA_multiplier",
+        )
+        self._check_for_errors(response)
+        data = response["data"]
+        return self._create_dataframe(data, time_col="createTime")
+
+    def tow_hundred_week_moving_avg_heatmap(self) -> pd.DataFrame:
+        response = self._get(
+            endpoint="index/tow_hundred_week_moving_avg_heatmap",
+        )
+        self._check_for_errors(response)
+        data = response["data"]
+        return self._create_dataframe(data, time_col="createTime")
+
+    def puell_multiple(self) -> pd.DataFrame:
+        response = self._get(
+            endpoint="index/puell_multiple",
+        )
+        self._check_for_errors(response)
+        data = response["data"]
+        return self._create_dataframe(data, time_col="createTime")
+
+    def stock_flow(self) -> pd.DataFrame:
+        response = self._get(
+            endpoint="index/stock_flow",
+        )
+        self._check_for_errors(response)
+        data = response["data"]
+        return self._create_dataframe(data, time_col="createTime", unit=None)
+
+    def pi(self) -> pd.DataFrame:
+        response = self._get(
+            endpoint="index/pi",
+        )
+        self._check_for_errors(response)
+        data = response["data"]
+        return self._create_dataframe(data, time_col="createTime", cast_objects_to_numeric=True)
+
+    def golden_ratio_multiplier(self) -> pd.DataFrame:
+        response = self._get(
+            endpoint="index/golden_ratio_multiplier",
+        )
+        self._check_for_errors(response)
+        data = response["data"]
+        return self._create_dataframe(data, time_col="createTime", cast_objects_to_numeric=True)
+
+    def bitcoin_profitable_days(self) -> pd.DataFrame:
+        response = self._get(
+            endpoint="index/bitcoin_profitable_days",
+        )
+        self._check_for_errors(response)
+        data = response["data"]
+        return self._create_dataframe(data, time_col="createTime")
+
+    def log_log_regression(self) -> pd.DataFrame:
+        response = self._get(
+            endpoint="index/log_log_regression",
+        )
+        self._check_for_errors(response)
+        data = response["data"]
+        return self._create_dataframe(data, time_col="createTime")
+
+    def grayscale_market_history(self) -> pd.DataFrame:
+        response = self._get(
+            endpoint="index/grayscale_market_history",
+        )
+        self._check_for_errors(response)
+        data = response["data"]
+        return self._create_dataframe(data, time_col="dateList")
```

### Comparing `coinglass_api-0.4.0/pyproject.toml` & `coinglass_api-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coinglass-api"
-version = "0.4.0"
+version = "0.5.0"
 repository = "https://github.com/dineshpinto/coinglass-api"
 homepage = "https://github.com/dineshpinto/coinglass-api"
 license = "MIT"
 keywords = ["coinglass", "api", "crypto", "cryptocurrency", "bitcoin", "ethereum", "binance", "dydx", "okex"]
 description = "Unofficial Python client for Coinglass API"
 authors = ["dineshpinto <annual.fallout_0z@gmail.com>"]
 readme = "README.md"
```

### Comparing `coinglass_api-0.4.0/PKG-INFO` & `coinglass_api-0.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinglass-api
-Version: 0.4.0
+Version: 0.5.0
 Summary: Unofficial Python client for Coinglass API
 Home-page: https://github.com/dineshpinto/coinglass-api
 License: MIT
 Keywords: coinglass,api,crypto,cryptocurrency,bitcoin,ethereum,binance,dydx,okex
 Author: dineshpinto
 Author-email: annual.fallout_0z@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -15,24 +15,24 @@
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Repository, https://github.com/dineshpinto/coinglass-api
 Description-Content-Type: text/markdown
 
 # Coinglass API
 [![PyPi version](https://img.shields.io/pypi/v/coinglass-api)](https://pypi.python.org/pypi/coinglass-api/)
-[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100//)
-[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3110//)
+[![Downloads](https://pepy.tech/badge/coinglass-api)](https://pepy.tech/project/coinglass-api)
 [![codecov](https://codecov.io/gh/dineshpinto/coinglass-api/branch/main/graph/badge.svg?token=XTJRRU2W1T)](https://codecov.io/gh/dineshpinto/coinglass-api)
+[![API unittest](https://github.com/dineshpinto/coinglass-api/actions/workflows/api_unitests.yml/badge.svg)](https://github.com/dineshpinto/coinglass-api/actions/workflows/api_unitests.yml)
 
 ## Unofficial Python client for Coinglass API
 
 Wrapper around the [Coinglass API](https://coinglass.com/pricing) to fetch data about the crypto markets.
-All data is output in pandas DataFrames (single or multi-index) and all time series data uses a DateTimeIndex.
+All data is output in pandas DataFrames (single or multi-index) and all time series data uses a `DateTimeIndex`.
 
-**Note**: Currently only supports the `indicator` API endpoint.
+**Note**: Currently supports the `indicator` and `index` API endpoints.
 
 ![Example Plot](https://github.com/dineshpinto/coinglass-api/blob/main/examples/example_plot.jpg?raw=true)
 
 ## Installation
 
 ```bash
 pip install coinglass-api
@@ -61,14 +61,19 @@
 liq_ohlc_eth_dydx = cg.liquidation_pair(ex="dYdX", pair="ETH-USD", interval="h4")
 
 # Get liquidation data for BTC
 liq_btc = cg.liquidation_symbol(symbol="BTC", interval="h4")
 
 # Get long/short ratios for BTC
 lsr_btc = cg.long_short_symbol(symbol="BTC", interval="h4")
+
+# Get GBTC market history
+gbtc_history = cg.grayscale_market_history()
+
+# and more...
 ```
 
 ## Examples
 
 ```
 >>> cg.funding(ex="dYdX", pair="ETH-USD", interval="h8").head()
 ```
```

