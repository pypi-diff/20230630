# Comparing `tmp/trongrid_extractor-0.3.4.tar.gz` & `tmp/trongrid_extractor-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trongrid_extractor-0.3.4.tar", max compression
+gzip compressed data, was "trongrid_extractor-0.3.5.tar", max compression
```

## Comparing `trongrid_extractor-0.3.4.tar` & `trongrid_extractor-0.3.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      617 2023-06-30 02:06:32.017372 trongrid_extractor-0.3.4/CHANGELOG.md
--rw-r--r--   0        0        0       36 2023-06-27 21:57:40.566976 trongrid_extractor-0.3.4/LICENSE
--rw-r--r--   0        0        0     3788 2023-06-29 06:44:04.355607 trongrid_extractor-0.3.4/README.md
--rw-r--r--   0        0        0      681 2023-06-30 02:06:32.023511 trongrid_extractor-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      459 2023-06-28 08:24:37.997172 trongrid_extractor-0.3.4/trongrid_extractor/__init__.py
--rw-r--r--   0        0        0    12028 2023-06-30 02:06:04.627001 trongrid_extractor-0.3.4/trongrid_extractor/api.py
--rw-r--r--   0        0        0      326 2023-06-29 00:31:04.580384 trongrid_extractor-0.3.4/trongrid_extractor/config.py
--rw-r--r--   0        0        0     1557 2023-06-30 02:06:04.627281 trongrid_extractor-0.3.4/trongrid_extractor/helpers/address_helpers.py
--rw-r--r--   0        0        0     2243 2023-06-28 19:11:14.811112 trongrid_extractor-0.3.4/trongrid_extractor/helpers/argument_parser.py
--rw-r--r--   0        0        0     2194 2023-06-30 02:06:04.627545 trongrid_extractor-0.3.4/trongrid_extractor/helpers/csv_helper.py
--rw-r--r--   0        0        0      196 2023-06-28 02:11:34.501085 trongrid_extractor-0.3.4/trongrid_extractor/helpers/dict_helper.py
--rw-r--r--   0        0        0      274 2023-06-28 19:37:05.672421 trongrid_extractor-0.3.4/trongrid_extractor/helpers/string_constants.py
--rw-r--r--   0        0        0     1431 2023-06-27 21:52:41.750623 trongrid_extractor-0.3.4/trongrid_extractor/helpers/time_helpers.py
--rw-r--r--   0        0        0     2283 2023-06-28 08:31:15.138247 trongrid_extractor-0.3.4/trongrid_extractor/progress_tracker.py
--rw-r--r--   0        0        0     3000 2023-06-30 02:06:04.627829 trongrid_extractor-0.3.4/trongrid_extractor/response.py
--rw-r--r--   0        0        0     4336 2023-06-28 19:40:28.066469 trongrid_extractor-0.3.4/trongrid_extractor/trc20_txn.py
--rw-r--r--   0        0        0     4380 1970-01-01 00:00:00.000000 trongrid_extractor-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      786 2023-06-30 05:35:48.751268 trongrid_extractor-0.3.5/CHANGELOG.md
+-rw-r--r--   0        0        0       36 2023-06-27 21:57:40.566976 trongrid_extractor-0.3.5/LICENSE
+-rw-r--r--   0        0        0     3788 2023-06-29 06:44:04.355607 trongrid_extractor-0.3.5/README.md
+-rw-r--r--   0        0        0      681 2023-06-30 05:35:48.758091 trongrid_extractor-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      459 2023-06-28 08:24:37.997172 trongrid_extractor-0.3.5/trongrid_extractor/__init__.py
+-rw-r--r--   0        0        0    11479 2023-06-30 05:29:58.300565 trongrid_extractor-0.3.5/trongrid_extractor/api.py
+-rw-r--r--   0        0        0      326 2023-06-29 00:31:04.580384 trongrid_extractor-0.3.5/trongrid_extractor/config.py
+-rw-r--r--   0        0        0     1557 2023-06-30 02:06:04.627281 trongrid_extractor-0.3.5/trongrid_extractor/helpers/address_helpers.py
+-rw-r--r--   0        0        0     2243 2023-06-28 19:11:14.811112 trongrid_extractor-0.3.5/trongrid_extractor/helpers/argument_parser.py
+-rw-r--r--   0        0        0     2194 2023-06-30 02:06:04.627545 trongrid_extractor-0.3.5/trongrid_extractor/helpers/csv_helper.py
+-rw-r--r--   0        0        0      196 2023-06-28 02:11:34.501085 trongrid_extractor-0.3.5/trongrid_extractor/helpers/dict_helper.py
+-rw-r--r--   0        0        0      274 2023-06-28 19:37:05.672421 trongrid_extractor-0.3.5/trongrid_extractor/helpers/string_constants.py
+-rw-r--r--   0        0        0     1431 2023-06-27 21:52:41.750623 trongrid_extractor-0.3.5/trongrid_extractor/helpers/time_helpers.py
+-rw-r--r--   0        0        0     2283 2023-06-28 08:31:15.138247 trongrid_extractor-0.3.5/trongrid_extractor/progress_tracker.py
+-rw-r--r--   0        0        0     3490 2023-06-30 05:35:14.960607 trongrid_extractor-0.3.5/trongrid_extractor/response.py
+-rw-r--r--   0        0        0     4336 2023-06-28 19:40:28.066469 trongrid_extractor-0.3.5/trongrid_extractor/trc20_txn.py
+-rw-r--r--   0        0        0     4380 1970-01-01 00:00:00.000000 trongrid_extractor-0.3.5/PKG-INFO
```

### Comparing `trongrid_extractor-0.3.4/README.md` & `trongrid_extractor-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.4/pyproject.toml` & `trongrid_extractor-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trongrid-extractor"
-version = "0.3.4"
+version = "0.3.5"
 description = "Extract transactions from the Trongrid API."
 authors = ["Chain Argos"]
 readme = "README.md"
 packages = [{include = "trongrid_extractor"}]
 homepage = "https://chainargos.com"
 
 include = [
```

### Comparing `trongrid_extractor-0.3.4/trongrid_extractor/api.py` & `trongrid_extractor-0.3.5/trongrid_extractor/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,31 @@
 '''
 API wrapper for TronGrid.
 '''
-import os
 import tempfile
-from copy import deepcopy
 from pathlib import Path
-from time import sleep
 from typing import Any, Dict, List, Optional
 
 import pendulum
-import requests
 from pendulum import DateTime
-from rich.pretty import pprint
-from tenacity import after_log, retry, stop_after_attempt, wait_exponential
 
 from trongrid_extractor.config import log
 from trongrid_extractor.helpers.csv_helper import *
 from trongrid_extractor.helpers.string_constants import *
 from trongrid_extractor.helpers.time_helpers import *
 from trongrid_extractor.progress_tracker import ProgressTracker
 from trongrid_extractor.response import Response
 from trongrid_extractor.trc20_txn import Trc20Txn
 
 MAX_TRADES_PER_CALL = 200
 
 RESCUE_DURATION_WALKBACK_SECONDS = [
     20,
-    3600,
-    24 * 3600
+    200,
+    1000,
 ]
 
 ONE_SECOND_MS = 1000.0
 EMPTY_RESPONSE_RETRY_AFTER_SECONDS = 60
 
 # Currently we poll from the most recent to the earliest events which is perhaps non optimal
 ORDER_BY_BLOCK_TIMESTAMP_ASC = 'block_timestamp,asc'
@@ -92,68 +86,61 @@
             force_continue_from_rescue = False
             next_url = response.next_url()
 
             # Pull the next record
             if next_url is not None:
                 log.debug(f"Retrieving next URL '{next_url}'...")
                 response = Response.get_response(next_url)
-            elif response.is_false_complete_response():
-                # TODO: this should really use a retry block, otherwise can be an infinite loop
-                log.warning(f"0 row response! Sleeping {EMPTY_RESPONSE_RETRY_AFTER_SECONDS}s and trying again...")
-                log.warning(f"   Params: {params}\n   Response:")
-                pprint(response, expand_all=True)
-                sleep(EMPTY_RESPONSE_RETRY_AFTER_SECONDS)
-                response = Response.get_response(contract_url, params)
             else:
                 log.error(f"Unparseable response!")
-                pprint(response, expand_all=True)
+                response.pretty_print()
                 raise ValueError("Unparseable response!")
 
             # Handle case where Trongrid barfs because we paged too much
-            if response.is_paging_complete():
-                log.info(f"Paging complete for {params}.")
-                log.info(f"Setting {MAX_TIMESTAMP} to {progress_tracker.earliest_block_timestamp_seen}")
-
-                # Log a simplified version of the response
-                pprint(response.without_data(), expand_all=True)
-                params[MAX_TIMESTAMP] = progress_tracker.earliest_block_timestamp_seen
-                response = Response.get_response(contract_url, params)
-            elif not response.was_successful():
+            if not response.was_successful():
                 # When the "next URL" paging fails we go back to filtering by timestamp but move
                 # the max_timestamp parameter. (I tried something involving the response[META][FINGERPRINT]
                 # but it didn't help.)
                 log.info(f"Failed to retrieve provided next URL. Moving end timestamp and restarting...")
                 log.debug(f"  Next URL: '{next_url}'.\n  Setting {MAX_TIMESTAMP} to {params[MAX_TIMESTAMP]}")
                 params[MAX_TIMESTAMP] = progress_tracker.earliest_block_timestamp_seen
                 response = Response.get_response(contract_url, params)
+            elif response.is_paging_complete():
+                log.info(f"Paging complete for {params}.")
+                log.info(f"Setting {MAX_TIMESTAMP} to {progress_tracker.earliest_block_timestamp_seen}")
+
+                # Log a simplified version of the response
+                response.print_abbreviated()
+                params[MAX_TIMESTAMP] = progress_tracker.earliest_block_timestamp_seen
+                response = Response.get_response(contract_url, params)
 
             retrieved_txns = Trc20Txn.extract_from_events(response.response)
             retrieved_txns = progress_tracker.remove_already_processed_txns(retrieved_txns)
 
             # See comment on _rescue_extraction() but tl;dr TronGrid is broken.
             # TODO: is this actually necessary?
             if len(retrieved_txns) == 0:
                 for walkback_seconds in RESCUE_DURATION_WALKBACK_SECONDS:
                     log.warning(f"0 txns found. We seem to be stuck at {ms_to_datetime(params[MAX_TIMESTAMP])}.")
                     log.warning(f"  (Maybe) Last request params: {params}")
-                    pprint(response.response, expand_all=True)
+                    response.print_abbreviated()
 
                     # Get txns
                     retrieved_txns = self._rescue_extraction(contract_url, params, walkback_seconds)
                     retrieved_txns = progress_tracker.remove_already_processed_txns(retrieved_txns)
 
                     if len(retrieved_txns) > 0:
                         log.info(f"Rescued {len(retrieved_txns)}, forcibly continuing...")
                         force_continue_from_rescue = True
                         break
 
             write_rows(output_csv_filename, retrieved_txns)
 
         log.info("Extraction loop is complete; here is the last response from the api for params: {params}")
-        pprint(response, expand_all=True)
+        response.print_abbreviated()
         return output_csv_filename
 
     def trc20_xfers_for_wallet(self, contract_addr: str, wallet_addr: str, token_type: str = TRC20) -> List[Trc20Txn]:
         """Use the TRC20 endpoint to get transfers for a particular wallet/token combo."""
         raise ValueError("Needs revision to use ProgressTracker and more.")
         wallet_url = f"{self.base_uri}accounts/{wallet_addr}/transactions/{token_type}"
         params = Api.build_params(extra={'contract_address': contract_addr})
@@ -198,43 +185,46 @@
 
         Example problematic call:
              extract_tron_transactions TR7NHqjeKQxGTCi8q8ZY4pL8otSzgjLj6t -u 2023-06-26T13:16:24+00:00
         """
         log.warning(f"Attempting rescue by requesting from max_timestamp minus {walkback} seconds...")
         log.debug(f"Params before new min_timestamp: {params}")
 
+        if params[MIN_TIMESTAMP] == params[MAX_TIMESTAMP]:
+            log.warning(f"Min and max timestamp are already the same ({ms_to_datetime(params[MIN_TIMESTAMP])})")
+            return []
+
         old_min_timestamp = params[MIN_TIMESTAMP]
-        params[MIN_TIMESTAMP] = params[MAX_TIMESTAMP] - (walkback * 1000.0)
+        new_min_timestamp = params[MAX_TIMESTAMP] - (walkback * 1000.0)
+        params[MIN_TIMESTAMP] = max(old_min_timestamp, new_min_timestamp)
         response: Response = Response.get_response(url, params)
         txns = Trc20Txn.extract_from_events(response.response)
-        subtract_one_second = True
+        has_retrieved_all_pages = True
 
         while response.is_continuable_response():
             next_url = response.next_url()
             log.debug(f"Retrieving next URL '{next_url}'...")
             response = Response.get_response(next_url)
 
             if not response.was_successful():
-                msg = f"Failed to retrieve next_url: '{next_url}'"
-                log.error(f"{msg}\n\nFinal response:")
-                pprint(response.response, expand_all=True)
-                # If we fail to page all the whole response that means we might not yet have all the
-                # records for that second in time.
-                subtract_one_second = False
+                log.error(f"Failed to retrieve next_url: '{next_url}'\n\nFinal response:")
+                response.pretty_print()
+                # If we fail to page all the way we need to be cautious about moving the window
+                has_retrieved_all_pages = False
                 break
 
             last_txns = Trc20Txn.extract_from_events(response.response)
             log.info(f"Rescued {len(last_txns)} more records")
             txns.extend(last_txns)
 
-        log.debug(f"Exiting loop; no META or next url. Here's the final response: {response}")
-        params[MAX_TIMESTAMP] = params[MIN_TIMESTAMP]
-
-        if subtract_one_second:
-            params[MAX_TIMESTAMP] -= ONE_SECOND_MS
+        if has_retrieved_all_pages:
+            log.info(f"Retrieved all pages in the rescue attempt!")
+            params[MAX_TIMESTAMP] = params[MIN_TIMESTAMP] - ONE_SECOND_MS
+        else:
+            params[MAX_TIMESTAMP] = min([t.ms_from_epoch for t in txns])
 
         params[MIN_TIMESTAMP] = old_min_timestamp
         log.info(f"  Returning {len(txns)} transactions from _rescue_extraction(), modified params in place.")
         log.debug(f"Modified params: {params}")
         return txns
 
     @staticmethod
```

### Comparing `trongrid_extractor-0.3.4/trongrid_extractor/helpers/address_helpers.py` & `trongrid_extractor-0.3.5/trongrid_extractor/helpers/address_helpers.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.4/trongrid_extractor/helpers/argument_parser.py` & `trongrid_extractor-0.3.5/trongrid_extractor/helpers/argument_parser.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.4/trongrid_extractor/helpers/csv_helper.py` & `trongrid_extractor-0.3.5/trongrid_extractor/helpers/csv_helper.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.4/trongrid_extractor/helpers/time_helpers.py` & `trongrid_extractor-0.3.5/trongrid_extractor/helpers/time_helpers.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.4/trongrid_extractor/progress_tracker.py` & `trongrid_extractor-0.3.5/trongrid_extractor/progress_tracker.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.4/trongrid_extractor/response.py` & `trongrid_extractor-0.3.5/trongrid_extractor/response.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 import logging
 from copy import deepcopy
 from dataclasses import dataclass
 from typing import Any, Dict, Union
 
 import requests
+from rich.pretty import pprint
 from tenacity import after_log, retry, stop_after_attempt, wait_exponential
 
 from trongrid_extractor.config import log
 from trongrid_extractor.helpers.csv_helper import *
 from trongrid_extractor.helpers.string_constants import *
 from trongrid_extractor.helpers.time_helpers import *
 
@@ -19,39 +20,47 @@
 
 @dataclass
 class Response:
     response: Dict[str, Any]
     params: Dict[str, Any]
 
     @classmethod
-    @retry(wait=wait_exponential(multiplier=1, min=4, max=60), stop=stop_after_attempt(7), after=after_log(log, logging.DEBUG))
+    @retry(wait=wait_exponential(multiplier=1, min=15, max=300), stop=stop_after_attempt(5), after=after_log(log, logging.DEBUG))
     def get_response(cls, url: str, params: Optional[Dict[str, Union[str, int, float]]] = None) -> 'Response':
         """Hit the endpoint and extract JSON data."""
         params = params or {}
 
         # Min/Max timestamps are INCLUSIVE.
         if MIN_TIMESTAMP in params and MAX_TIMESTAMP in params:
             msg = f"Requesting records from {ms_to_datetime(params[MIN_TIMESTAMP])} to {ms_to_datetime(params[MAX_TIMESTAMP])}."
             log.info(msg)
 
         log.debug(f"\nURL: {url}\nParams: {params}")
-        response = requests.get(url, headers=JSON_HEADERS, params=params).json()
-        log.debug(f"Response: {response}")
-        return cls(response, deepcopy(params))
+        response_dict = requests.get(url, headers=JSON_HEADERS, params=params).json()
+        log.debug(f"Response: {response_dict}")
+        response = cls(response_dict, deepcopy(params))
+
+        if response.is_false_complete_response():
+            msg = f"False positive reponse! {response.response}"
+            log.error(msg)
+            response.pretty_print()
+            raise ValueError(msg)
+
+        return response
 
     def is_continuable_response(self) -> bool:
         return self.next_url() is not None
 
     def is_paging_complete(self) -> bool:
         page_size = self.page_size() or 0
         return self.was_successful() and page_size > 0 and self.next_url() is None
 
     def is_false_complete_response(self) -> bool:
         """Sometimes for no reason TronGrid just returns 0 rows to a query that would otherwise return rows."""
-        return self.was_successful() and self.page_size() == 0 and self.next_url() is None
+        return self.was_successful() and self.page_size() == 0 and DATA not in self.response and self.next_url() is None
 
     def was_successful(self) -> bool:
         if SUCCESS not in self.response:
             log.warning(f"No '{SUCCESS}' key found in response!\n{self.response}")
             return False
 
         success = self.response[SUCCESS]
@@ -70,7 +79,13 @@
             return self.response[META][PAGE_SIZE]
 
     def without_data(self) -> Dict[str, Any]:
         """Return the response JSON just without the 'data' field."""
         abbreviated_response = deepcopy(self.response)
         abbreviated_response['data'] = f"[Skipping {len(self.response['data'])} elements of 'data' array]"
         return abbreviated_response
+
+    def pretty_print(self) -> None:
+        pprint(self, expand_all=True)
+
+    def print_abbreviated(self) -> None:
+        pprint(self.without_data(), expand_all=True)
```

### Comparing `trongrid_extractor-0.3.4/trongrid_extractor/trc20_txn.py` & `trongrid_extractor-0.3.5/trongrid_extractor/trc20_txn.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.4/PKG-INFO` & `trongrid_extractor-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trongrid-extractor
-Version: 0.3.4
+Version: 0.3.5
 Summary: Extract transactions from the Trongrid API.
 Home-page: https://chainargos.com
 Author: Chain Argos
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

