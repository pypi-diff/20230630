# Comparing `tmp/trongrid_extractor-0.3.5.tar.gz` & `tmp/trongrid_extractor-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trongrid_extractor-0.3.5.tar", max compression
+gzip compressed data, was "trongrid_extractor-0.3.6.tar", max compression
```

## Comparing `trongrid_extractor-0.3.5.tar` & `trongrid_extractor-0.3.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      786 2023-06-30 05:35:48.751268 trongrid_extractor-0.3.5/CHANGELOG.md
--rw-r--r--   0        0        0       36 2023-06-27 21:57:40.566976 trongrid_extractor-0.3.5/LICENSE
--rw-r--r--   0        0        0     3788 2023-06-29 06:44:04.355607 trongrid_extractor-0.3.5/README.md
--rw-r--r--   0        0        0      681 2023-06-30 05:35:48.758091 trongrid_extractor-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      459 2023-06-28 08:24:37.997172 trongrid_extractor-0.3.5/trongrid_extractor/__init__.py
--rw-r--r--   0        0        0    11479 2023-06-30 05:29:58.300565 trongrid_extractor-0.3.5/trongrid_extractor/api.py
--rw-r--r--   0        0        0      326 2023-06-29 00:31:04.580384 trongrid_extractor-0.3.5/trongrid_extractor/config.py
--rw-r--r--   0        0        0     1557 2023-06-30 02:06:04.627281 trongrid_extractor-0.3.5/trongrid_extractor/helpers/address_helpers.py
--rw-r--r--   0        0        0     2243 2023-06-28 19:11:14.811112 trongrid_extractor-0.3.5/trongrid_extractor/helpers/argument_parser.py
--rw-r--r--   0        0        0     2194 2023-06-30 02:06:04.627545 trongrid_extractor-0.3.5/trongrid_extractor/helpers/csv_helper.py
--rw-r--r--   0        0        0      196 2023-06-28 02:11:34.501085 trongrid_extractor-0.3.5/trongrid_extractor/helpers/dict_helper.py
--rw-r--r--   0        0        0      274 2023-06-28 19:37:05.672421 trongrid_extractor-0.3.5/trongrid_extractor/helpers/string_constants.py
--rw-r--r--   0        0        0     1431 2023-06-27 21:52:41.750623 trongrid_extractor-0.3.5/trongrid_extractor/helpers/time_helpers.py
--rw-r--r--   0        0        0     2283 2023-06-28 08:31:15.138247 trongrid_extractor-0.3.5/trongrid_extractor/progress_tracker.py
--rw-r--r--   0        0        0     3490 2023-06-30 05:35:14.960607 trongrid_extractor-0.3.5/trongrid_extractor/response.py
--rw-r--r--   0        0        0     4336 2023-06-28 19:40:28.066469 trongrid_extractor-0.3.5/trongrid_extractor/trc20_txn.py
--rw-r--r--   0        0        0     4380 1970-01-01 00:00:00.000000 trongrid_extractor-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      837 2023-06-30 06:31:51.716505 trongrid_extractor-0.3.6/CHANGELOG.md
+-rw-r--r--   0        0        0       36 2023-06-27 21:57:40.566976 trongrid_extractor-0.3.6/LICENSE
+-rw-r--r--   0        0        0     3788 2023-06-29 06:44:04.355607 trongrid_extractor-0.3.6/README.md
+-rw-r--r--   0        0        0      710 2023-06-30 06:31:51.722193 trongrid_extractor-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      459 2023-06-28 08:24:37.997172 trongrid_extractor-0.3.6/trongrid_extractor/__init__.py
+-rw-r--r--   0        0        0    11137 2023-06-30 06:29:48.277928 trongrid_extractor-0.3.6/trongrid_extractor/api.py
+-rw-r--r--   0        0        0      326 2023-06-29 00:31:04.580384 trongrid_extractor-0.3.6/trongrid_extractor/config.py
+-rw-r--r--   0        0        0     1557 2023-06-30 02:06:04.627281 trongrid_extractor-0.3.6/trongrid_extractor/helpers/address_helpers.py
+-rw-r--r--   0        0        0     2243 2023-06-28 19:11:14.811112 trongrid_extractor-0.3.6/trongrid_extractor/helpers/argument_parser.py
+-rw-r--r--   0        0        0     2194 2023-06-30 02:06:04.627545 trongrid_extractor-0.3.6/trongrid_extractor/helpers/csv_helper.py
+-rw-r--r--   0        0        0      196 2023-06-28 02:11:34.501085 trongrid_extractor-0.3.6/trongrid_extractor/helpers/dict_helper.py
+-rw-r--r--   0        0        0      274 2023-06-28 19:37:05.672421 trongrid_extractor-0.3.6/trongrid_extractor/helpers/string_constants.py
+-rw-r--r--   0        0        0     1431 2023-06-27 21:52:41.750623 trongrid_extractor-0.3.6/trongrid_extractor/helpers/time_helpers.py
+-rw-r--r--   0        0        0     2283 2023-06-28 08:31:15.138247 trongrid_extractor-0.3.6/trongrid_extractor/progress_tracker.py
+-rw-r--r--   0        0        0     3667 2023-06-30 06:23:34.464107 trongrid_extractor-0.3.6/trongrid_extractor/response.py
+-rw-r--r--   0        0        0     4336 2023-06-28 19:40:28.066469 trongrid_extractor-0.3.6/trongrid_extractor/trc20_txn.py
+-rw-r--r--   0        0        0     4430 1970-01-01 00:00:00.000000 trongrid_extractor-0.3.6/PKG-INFO
```

### Comparing `trongrid_extractor-0.3.5/CHANGELOG.md` & `trongrid_extractor-0.3.6/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # NEXT RELEASE
 
+### 0.3.6
+* Simplify inner logic and retries etc.
+
 ### 0.3.5
 * Avoid endless loop on `is_false_complete_response()`
 * Refactor `response.pretty_print()`
 * Don't allow walkbacks to walk back past the start of the period
 
 ### 0.3.4
 * `Response` object refactor
```

### Comparing `trongrid_extractor-0.3.5/README.md` & `trongrid_extractor-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.5/pyproject.toml` & `trongrid_extractor-0.3.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trongrid-extractor"
-version = "0.3.5"
+version = "0.3.6"
 description = "Extract transactions from the Trongrid API."
 authors = ["Chain Argos"]
 readme = "README.md"
 packages = [{include = "trongrid_extractor"}]
 homepage = "https://chainargos.com"
 
 include = [
@@ -15,14 +15,15 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
 pendulum = "^2.1.2"
 rich = "^13.4.1"
 base58 = "^2.1.1"
 tenacity = "^8.2.2"
+requests_toolbelt = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `trongrid_extractor-0.3.5/trongrid_extractor/api.py` & `trongrid_extractor-0.3.6/trongrid_extractor/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,38 +84,33 @@
         # This uses the "next_url" approach which fails after a while.
         while response.is_continuable_response() or force_continue_from_rescue:
             force_continue_from_rescue = False
             next_url = response.next_url()
 
             # Pull the next record
             if next_url is not None:
-                log.debug(f"Retrieving next URL '{next_url}'...")
                 response = Response.get_response(next_url)
+            elif force_continue_from_rescue:
+                log.info(f"Forcibly continuing so making a request for {params}")
+                response = Response.get_response(contract_url, params)
             else:
                 log.error(f"Unparseable response!")
                 response.pretty_print()
                 raise ValueError("Unparseable response!")
 
-            # Handle case where Trongrid barfs because we paged too much
+            # Trongrid doesn't like it when you page more than 5 pages of 200 results. When the
+            # "next URL" paging fails we go back to filtering by timestamp but move the
+            # max_timestamp parameter back.
             if not response.was_successful():
-                # When the "next URL" paging fails we go back to filtering by timestamp but move
-                # the max_timestamp parameter. (I tried something involving the response[META][FINGERPRINT]
-                # but it didn't help.)
                 log.info(f"Failed to retrieve provided next URL. Moving end timestamp and restarting...")
-                log.debug(f"  Next URL: '{next_url}'.\n  Setting {MAX_TIMESTAMP} to {params[MAX_TIMESTAMP]}")
                 params[MAX_TIMESTAMP] = progress_tracker.earliest_block_timestamp_seen
                 response = Response.get_response(contract_url, params)
             elif response.is_paging_complete():
-                log.info(f"Paging complete for {params}.")
-                log.info(f"Setting {MAX_TIMESTAMP} to {progress_tracker.earliest_block_timestamp_seen}")
-
-                # Log a simplified version of the response
+                log.info(f"Paging complete for {params}, backing up max_timestamp but should we do this?")
                 response.print_abbreviated()
-                params[MAX_TIMESTAMP] = progress_tracker.earliest_block_timestamp_seen
-                response = Response.get_response(contract_url, params)
 
             retrieved_txns = Trc20Txn.extract_from_events(response.response)
             retrieved_txns = progress_tracker.remove_already_processed_txns(retrieved_txns)
 
             # See comment on _rescue_extraction() but tl;dr TronGrid is broken.
             # TODO: is this actually necessary?
             if len(retrieved_txns) == 0:
```

### Comparing `trongrid_extractor-0.3.5/trongrid_extractor/helpers/address_helpers.py` & `trongrid_extractor-0.3.6/trongrid_extractor/helpers/address_helpers.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.5/trongrid_extractor/helpers/argument_parser.py` & `trongrid_extractor-0.3.6/trongrid_extractor/helpers/argument_parser.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.5/trongrid_extractor/helpers/csv_helper.py` & `trongrid_extractor-0.3.6/trongrid_extractor/helpers/csv_helper.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.5/trongrid_extractor/helpers/time_helpers.py` & `trongrid_extractor-0.3.6/trongrid_extractor/helpers/time_helpers.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.5/trongrid_extractor/progress_tracker.py` & `trongrid_extractor-0.3.6/trongrid_extractor/progress_tracker.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.5/trongrid_extractor/response.py` & `trongrid_extractor-0.3.6/trongrid_extractor/response.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,45 +3,49 @@
 """
 import logging
 from copy import deepcopy
 from dataclasses import dataclass
 from typing import Any, Dict, Union
 
 import requests
+from requests_toolbelt.utils import dump
 from rich.pretty import pprint
 from tenacity import after_log, retry, stop_after_attempt, wait_exponential
 
 from trongrid_extractor.config import log
 from trongrid_extractor.helpers.csv_helper import *
 from trongrid_extractor.helpers.string_constants import *
 from trongrid_extractor.helpers.time_helpers import *
 
 JSON_HEADERS = {'Accept': 'application/json'}
 
 
 @dataclass
 class Response:
-    response: Dict[str, Any]
+    raw_response: requests.models.Response
     params: Dict[str, Any]
 
+    def __post_init__(self):
+        log.debug(dump.dump_all(self.raw_response).decode('utf-8'))
+        self.response = self.raw_response.json()
+
     @classmethod
     @retry(wait=wait_exponential(multiplier=1, min=15, max=300), stop=stop_after_attempt(5), after=after_log(log, logging.DEBUG))
     def get_response(cls, url: str, params: Optional[Dict[str, Union[str, int, float]]] = None) -> 'Response':
         """Hit the endpoint and extract JSON data."""
         params = params or {}
 
         # Min/Max timestamps are INCLUSIVE.
         if MIN_TIMESTAMP in params and MAX_TIMESTAMP in params:
             msg = f"Requesting records from {ms_to_datetime(params[MIN_TIMESTAMP])} to {ms_to_datetime(params[MAX_TIMESTAMP])}."
             log.info(msg)
 
-        log.debug(f"\nURL: {url}\nParams: {params}")
-        response_dict = requests.get(url, headers=JSON_HEADERS, params=params).json()
-        log.debug(f"Response: {response_dict}")
-        response = cls(response_dict, deepcopy(params))
+        log.debug(f"Request URL: {url}\nParams: {params}")
+        raw_response = requests.get(url, headers=JSON_HEADERS, params=params)
+        response = cls(raw_response, deepcopy(params))
 
         if response.is_false_complete_response():
             msg = f"False positive reponse! {response.response}"
             log.error(msg)
             response.pretty_print()
             raise ValueError(msg)
 
@@ -52,15 +56,15 @@
 
     def is_paging_complete(self) -> bool:
         page_size = self.page_size() or 0
         return self.was_successful() and page_size > 0 and self.next_url() is None
 
     def is_false_complete_response(self) -> bool:
         """Sometimes for no reason TronGrid just returns 0 rows to a query that would otherwise return rows."""
-        return self.was_successful() and self.page_size() == 0 and DATA not in self.response and self.next_url() is None
+        return self.was_successful() and self.page_size() == 0 and DATA and self.next_url() is None
 
     def was_successful(self) -> bool:
         if SUCCESS not in self.response:
             log.warning(f"No '{SUCCESS}' key found in response!\n{self.response}")
             return False
 
         success = self.response[SUCCESS]
@@ -82,10 +86,11 @@
         """Return the response JSON just without the 'data' field."""
         abbreviated_response = deepcopy(self.response)
         abbreviated_response['data'] = f"[Skipping {len(self.response['data'])} elements of 'data' array]"
         return abbreviated_response
 
     def pretty_print(self) -> None:
         pprint(self, expand_all=True)
+        pprint(self.response, expand_all=True)
 
     def print_abbreviated(self) -> None:
         pprint(self.without_data(), expand_all=True)
```

### Comparing `trongrid_extractor-0.3.5/trongrid_extractor/trc20_txn.py` & `trongrid_extractor-0.3.6/trongrid_extractor/trc20_txn.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.5/PKG-INFO` & `trongrid_extractor-0.3.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: trongrid-extractor
-Version: 0.3.5
+Version: 0.3.6
 Summary: Extract transactions from the Trongrid API.
 Home-page: https://chainargos.com
 Author: Chain Argos
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: base58 (>=2.1.1,<3.0.0)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: requests_toolbelt (>=1.0.0,<2.0.0)
 Requires-Dist: rich (>=13.4.1,<14.0.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Description-Content-Type: text/markdown
 
 # Usage
 ## Command Line
 Run `extract_tron_transactions --help` to see the command line options.
```

