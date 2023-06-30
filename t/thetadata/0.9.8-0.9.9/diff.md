# Comparing `tmp/thetadata-0.9.8.tar.gz` & `tmp/thetadata-0.9.9.tar.gz`

## Comparing `thetadata-0.9.8.tar` & `thetadata-0.9.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 thetadata-0.9.8/mkdocs.yml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 thetadata-0.9.8/setup.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 thetadata-0.9.8/.github/workflows/main.yml
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 thetadata-0.9.8/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/__init__.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/connection_msgs.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/explanation.md
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/how-to-guides.md
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/index.md
--rw-r--r--   0        0        0    51619 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/logo.png
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/manipulate_df.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/manipulate_series.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/reference.md
--rw-r--r--   0        0        0    30099 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/tutorials.md
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/options/__init__.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/options/cancel_streams.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/options/eod.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/options/get_last.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/options/list_roots.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/options/open_interest_streaming.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/options/quote_1min.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/options/quote_streaming.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/options/quote_tick.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/options/trade_streaming.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/options/trade_streaming_full.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/stocks/__init__.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/stocks/eod.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/stocks/get_last.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/stocks/list_roots.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/stocks/quote_1min.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 thetadata-0.9.8/docs/stocks/quote_tick.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 thetadata-0.9.8/tests/__init__.py
--rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 thetadata-0.9.8/tests/test_client.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 thetadata-0.9.8/tests/test_docs.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 thetadata-0.9.8/thetadata/__init__.py
--rw-r--r--   0        0        0    58685 2020-02-02 00:00:00.000000 thetadata-0.9.8/thetadata/client.py
--rw-r--r--   0        0        0    20348 2020-02-02 00:00:00.000000 thetadata-0.9.8/thetadata/enums.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 thetadata-0.9.8/thetadata/exceptions.py
--rw-r--r--   0        0        0    14571 2020-02-02 00:00:00.000000 thetadata-0.9.8/thetadata/parsing.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 thetadata-0.9.8/thetadata/py.typed
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 thetadata-0.9.8/thetadata/terminal.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 thetadata-0.9.8/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 thetadata-0.9.8/LICENSE
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 thetadata-0.9.8/README.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 thetadata-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 thetadata-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 thetadata-0.9.9/mkdocs.yml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 thetadata-0.9.9/setup.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 thetadata-0.9.9/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 thetadata-0.9.9/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.9/docs/__init__.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 thetadata-0.9.9/docs/connection_msgs.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 thetadata-0.9.9/docs/explanation.md
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 thetadata-0.9.9/docs/how-to-guides.md
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 thetadata-0.9.9/docs/index.md
+-rw-r--r--   0        0        0    51619 2020-02-02 00:00:00.000000 thetadata-0.9.9/docs/logo.png
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 thetadata-0.9.9/docs/manipulate_df.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 thetadata-0.9.9/docs/manipulate_series.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 thetadata-0.9.9/docs/reference.md
+-rw-r--r--   0        0        0    30099 2020-02-02 00:00:00.000000 thetadata-0.9.9/docs/tutorials.md
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.9/docs/options/__init__.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 thetadata-0.9.9/docs/options/cancel_streams.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 thetadata-0.9.9/docs/options/eod.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 thetadata-0.9.9/docs/options/get_last.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 thetadata-0.9.9/docs/options/list_roots.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 thetadata-0.9.9/docs/options/open_interest_streaming.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 thetadata-0.9.9/docs/options/quote_1min.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 thetadata-0.9.9/docs/options/quote_streaming.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 thetadata-0.9.9/docs/options/quote_tick.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 thetadata-0.9.9/docs/options/trade_streaming.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 thetadata-0.9.9/docs/options/trade_streaming_full.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.9/docs/stocks/__init__.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 thetadata-0.9.9/docs/stocks/eod.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 thetadata-0.9.9/docs/stocks/get_last.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 thetadata-0.9.9/docs/stocks/list_roots.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 thetadata-0.9.9/docs/stocks/quote_1min.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 thetadata-0.9.9/docs/stocks/quote_tick.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 thetadata-0.9.9/tests/__init__.py
+-rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 thetadata-0.9.9/tests/test_client.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 thetadata-0.9.9/tests/test_docs.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 thetadata-0.9.9/thetadata/__init__.py
+-rw-r--r--   0        0        0    58742 2020-02-02 00:00:00.000000 thetadata-0.9.9/thetadata/client.py
+-rw-r--r--   0        0        0    20348 2020-02-02 00:00:00.000000 thetadata-0.9.9/thetadata/enums.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 thetadata-0.9.9/thetadata/exceptions.py
+-rw-r--r--   0        0        0    14571 2020-02-02 00:00:00.000000 thetadata-0.9.9/thetadata/parsing.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 thetadata-0.9.9/thetadata/py.typed
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 thetadata-0.9.9/thetadata/terminal.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 thetadata-0.9.9/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 thetadata-0.9.9/LICENSE
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 thetadata-0.9.9/README.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 thetadata-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 thetadata-0.9.9/PKG-INFO
```

### Comparing `thetadata-0.9.8/mkdocs.yml` & `thetadata-0.9.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/.github/workflows/main.yml` & `thetadata-0.9.9/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/.github/workflows/python-publish.yml` & `thetadata-0.9.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/docs/connection_msgs.py` & `thetadata-0.9.9/docs/connection_msgs.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/docs/explanation.md` & `thetadata-0.9.9/docs/explanation.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/docs/how-to-guides.md` & `thetadata-0.9.9/docs/how-to-guides.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/docs/index.md` & `thetadata-0.9.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/docs/logo.png` & `thetadata-0.9.9/docs/logo.png`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/docs/manipulate_series.py` & `thetadata-0.9.9/docs/manipulate_series.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/docs/tutorials.md` & `thetadata-0.9.9/docs/tutorials.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/docs/options/cancel_streams.py` & `thetadata-0.9.9/docs/options/cancel_streams.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/docs/options/eod.py` & `thetadata-0.9.9/docs/options/eod.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/docs/options/get_last.py` & `thetadata-0.9.9/docs/options/get_last.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/docs/options/open_interest_streaming.py` & `thetadata-0.9.9/docs/options/open_interest_streaming.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/docs/options/quote_1min.py` & `thetadata-0.9.9/docs/options/quote_1min.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/docs/options/quote_streaming.py` & `thetadata-0.9.9/docs/options/quote_streaming.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/docs/options/quote_tick.py` & `thetadata-0.9.9/docs/options/quote_tick.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/docs/options/trade_streaming.py` & `thetadata-0.9.9/docs/options/trade_streaming.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/docs/options/trade_streaming_full.py` & `thetadata-0.9.9/docs/options/trade_streaming_full.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/docs/stocks/eod.py` & `thetadata-0.9.9/docs/stocks/eod.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/docs/stocks/get_last.py` & `thetadata-0.9.9/docs/stocks/get_last.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/docs/stocks/quote_1min.py` & `thetadata-0.9.9/docs/stocks/quote_1min.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/docs/stocks/quote_tick.py` & `thetadata-0.9.9/docs/stocks/quote_tick.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/tests/test_client.py` & `thetadata-0.9.9/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/tests/test_docs.py` & `thetadata-0.9.9/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/thetadata/client.py` & `thetadata-0.9.9/thetadata/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,29 +23,30 @@
     TickBody,
     ListBody,
     parse_list_REST, parse_flexible_REST, parse_hist_REST, parse_hist_REST_stream, parse_hist_REST_stream_ijson,
 )
 from .terminal import check_download, launch_terminal
 
 _NOT_CONNECTED_MSG = "You must establish a connection first."
-_VERSION = '0.9.8'
+_VERSION = '0.9.9'
 URL_BASE = "http://127.0.0.1:25510/"
 
 
 def _format_strike(strike: float) -> int:
     """Round USD to the nearest tenth of a cent, acceptable by the terminal."""
     return round(strike * 1000)
 
 
 def _format_date(dt: date) -> str:
     """Format a date obj into a string acceptable by the terminal."""
     return dt.strftime("%Y%m%d")
 
 
 def ms_to_time(ms_of_day: int) -> datetime.time:
+    """Converts milliseconds of day to a time object."""
     return datetime(year=2000, month=1, day=1, hour=int((ms_of_day / (1000 * 60 * 60)) % 24),
                     minute=int(ms_of_day / (1000 * 60)) % 60, second=int((ms_of_day / 1000) % 60),
                     microsecond=(ms_of_day % 1000) * 1000).time()
 
 
 _pt_to_price_mul = [
     0,
```

### Comparing `thetadata-0.9.8/thetadata/enums.py` & `thetadata-0.9.9/thetadata/enums.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/thetadata/exceptions.py` & `thetadata-0.9.9/thetadata/exceptions.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/thetadata/parsing.py` & `thetadata-0.9.9/thetadata/parsing.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/thetadata/terminal.py` & `thetadata-0.9.9/thetadata/terminal.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/LICENSE` & `thetadata-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/README.md` & `thetadata-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.8/pyproject.toml` & `thetadata-0.9.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "thetadata"
-version = "0.9.8"
+version = "0.9.9"
 authors = [
   { name="Bailey Danseglio", email="bailey@thetadata.net" },
   { name="Adler Weber", email="redacted@thetadata.net" },
 ]
 description = "Python API for Thetadata"
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `thetadata-0.9.8/PKG-INFO` & `thetadata-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thetadata
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python API for Thetadata
 Project-URL: Homepage, https://thetadata.net
 Project-URL: Source, https://thetadata-api.github.io/thetadata-python/reference/
 Project-URL: Bug Tracker, https://github.com/ThetaData-API/thetadata-python/issues
 Project-URL: Documentation, https://thetadata-api.github.io/thetadata-python/
 Author-email: Bailey Danseglio <bailey@thetadata.net>, Adler Weber <redacted@thetadata.net>
 License: MIT License
```

