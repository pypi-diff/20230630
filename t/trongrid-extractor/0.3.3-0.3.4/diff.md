# Comparing `tmp/trongrid_extractor-0.3.3.tar.gz` & `tmp/trongrid_extractor-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trongrid_extractor-0.3.3.tar", max compression
+gzip compressed data, was "trongrid_extractor-0.3.4.tar", max compression
```

## Comparing `trongrid_extractor-0.3.3.tar` & `trongrid_extractor-0.3.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      520 2023-06-29 01:32:11.771651 trongrid_extractor-0.3.3/CHANGELOG.md
--rw-r--r--   0        0        0       36 2023-06-27 21:57:40.566976 trongrid_extractor-0.3.3/LICENSE
--rw-r--r--   0        0        0     3248 2023-06-29 01:07:40.251353 trongrid_extractor-0.3.3/README.md
--rw-r--r--   0        0        0      681 2023-06-29 01:32:11.775622 trongrid_extractor-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      459 2023-06-28 08:24:37.997172 trongrid_extractor-0.3.3/trongrid_extractor/__init__.py
--rw-r--r--   0        0        0    13269 2023-06-29 01:30:37.778406 trongrid_extractor-0.3.3/trongrid_extractor/api.py
--rw-r--r--   0        0        0      326 2023-06-29 00:31:04.580384 trongrid_extractor-0.3.3/trongrid_extractor/config.py
--rw-r--r--   0        0        0     1350 2023-06-28 19:08:18.556101 trongrid_extractor-0.3.3/trongrid_extractor/helpers/address_helpers.py
--rw-r--r--   0        0        0     2243 2023-06-28 19:11:14.811112 trongrid_extractor-0.3.3/trongrid_extractor/helpers/argument_parser.py
--rw-r--r--   0        0        0     2158 2023-06-29 01:27:50.985603 trongrid_extractor-0.3.3/trongrid_extractor/helpers/csv_helper.py
--rw-r--r--   0        0        0      196 2023-06-28 02:11:34.501085 trongrid_extractor-0.3.3/trongrid_extractor/helpers/dict_helper.py
--rw-r--r--   0        0        0      274 2023-06-28 19:37:05.672421 trongrid_extractor-0.3.3/trongrid_extractor/helpers/string_constants.py
--rw-r--r--   0        0        0     1431 2023-06-27 21:52:41.750623 trongrid_extractor-0.3.3/trongrid_extractor/helpers/time_helpers.py
--rw-r--r--   0        0        0     2283 2023-06-28 08:31:15.138247 trongrid_extractor-0.3.3/trongrid_extractor/progress_tracker.py
--rw-r--r--   0        0        0     4336 2023-06-28 19:40:28.066469 trongrid_extractor-0.3.3/trongrid_extractor/trc20_txn.py
--rw-r--r--   0        0        0     3840 1970-01-01 00:00:00.000000 trongrid_extractor-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      617 2023-06-30 02:06:32.017372 trongrid_extractor-0.3.4/CHANGELOG.md
+-rw-r--r--   0        0        0       36 2023-06-27 21:57:40.566976 trongrid_extractor-0.3.4/LICENSE
+-rw-r--r--   0        0        0     3788 2023-06-29 06:44:04.355607 trongrid_extractor-0.3.4/README.md
+-rw-r--r--   0        0        0      681 2023-06-30 02:06:32.023511 trongrid_extractor-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      459 2023-06-28 08:24:37.997172 trongrid_extractor-0.3.4/trongrid_extractor/__init__.py
+-rw-r--r--   0        0        0    12028 2023-06-30 02:06:04.627001 trongrid_extractor-0.3.4/trongrid_extractor/api.py
+-rw-r--r--   0        0        0      326 2023-06-29 00:31:04.580384 trongrid_extractor-0.3.4/trongrid_extractor/config.py
+-rw-r--r--   0        0        0     1557 2023-06-30 02:06:04.627281 trongrid_extractor-0.3.4/trongrid_extractor/helpers/address_helpers.py
+-rw-r--r--   0        0        0     2243 2023-06-28 19:11:14.811112 trongrid_extractor-0.3.4/trongrid_extractor/helpers/argument_parser.py
+-rw-r--r--   0        0        0     2194 2023-06-30 02:06:04.627545 trongrid_extractor-0.3.4/trongrid_extractor/helpers/csv_helper.py
+-rw-r--r--   0        0        0      196 2023-06-28 02:11:34.501085 trongrid_extractor-0.3.4/trongrid_extractor/helpers/dict_helper.py
+-rw-r--r--   0        0        0      274 2023-06-28 19:37:05.672421 trongrid_extractor-0.3.4/trongrid_extractor/helpers/string_constants.py
+-rw-r--r--   0        0        0     1431 2023-06-27 21:52:41.750623 trongrid_extractor-0.3.4/trongrid_extractor/helpers/time_helpers.py
+-rw-r--r--   0        0        0     2283 2023-06-28 08:31:15.138247 trongrid_extractor-0.3.4/trongrid_extractor/progress_tracker.py
+-rw-r--r--   0        0        0     3000 2023-06-30 02:06:04.627829 trongrid_extractor-0.3.4/trongrid_extractor/response.py
+-rw-r--r--   0        0        0     4336 2023-06-28 19:40:28.066469 trongrid_extractor-0.3.4/trongrid_extractor/trc20_txn.py
+-rw-r--r--   0        0        0     4380 1970-01-01 00:00:00.000000 trongrid_extractor-0.3.4/PKG-INFO
```

### Comparing `trongrid_extractor-0.3.3/README.md` & `trongrid_extractor-0.3.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -57,14 +57,23 @@
 ### Publishing
 1. Update `pyproject.toml` version number
 1. Update `CHANGELOG.md`
 1. `poetry publish --build --repository chain_argos_pypi`
 
 ## TODO
 1. Walk forward not backward
+1. USDT looks incomplete here as 9pm was the last time:
+   ```
+   WARNING - 0 txns found. We seem to be stuck at 2020-07-09T21:04:24+00:00.
+   [2023-06-29, 06:34:36 UTC] {logging_mixin.py:137} INFO -                     WARNING    Last request params:                   api.py:127
+                             {'only_confirmed': 'true', 'limit': 200,
+                             'min_timestamp': 1594252801000.0,
+                             'max_timestamp': 1594328664000.0,
+                             'event_name': 'Transfer'}
+    ```
 1. USDD around this time should be double checked:
    ```
     INFO       Returning 1000 transactions from _rescue_extraction(), modified params in place.                                    api.py:191
     INFO     Writing 1000 rows to 'events_USDD_written_2023-06-28T04.22.00.csv'...                                           csv_helper.py:17
     [06/28/23 10:22:34] INFO       Removed 200 duplicate transactions...                                                                   progress_tracker.py:47
     WARNING  0 txns found. We seem to be stuck at 2023-01-26T03:18:54+00:00.                                                       api.py:103
     WARNING    Last request params: {'only_confirmed': 'true', 'limit': 200, 'min_timestamp': 1483228800000.0, 'max_timestamp':    api.py:104
```

### Comparing `trongrid_extractor-0.3.3/pyproject.toml` & `trongrid_extractor-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trongrid-extractor"
-version = "0.3.3"
+version = "0.3.4"
 description = "Extract transactions from the Trongrid API."
 authors = ["Chain Argos"]
 readme = "README.md"
 packages = [{include = "trongrid_extractor"}]
 homepage = "https://chainargos.com"
 
 include = [
```

### Comparing `trongrid_extractor-0.3.3/trongrid_extractor/api.py` & `trongrid_extractor-0.3.4/trongrid_extractor/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 '''
 API wrapper for TronGrid.
 '''
 import os
 import tempfile
+from copy import deepcopy
 from pathlib import Path
 from time import sleep
 from typing import Any, Dict, List, Optional
 
 import pendulum
 import requests
 from pendulum import DateTime
@@ -14,19 +15,25 @@
 from tenacity import after_log, retry, stop_after_attempt, wait_exponential
 
 from trongrid_extractor.config import log
 from trongrid_extractor.helpers.csv_helper import *
 from trongrid_extractor.helpers.string_constants import *
 from trongrid_extractor.helpers.time_helpers import *
 from trongrid_extractor.progress_tracker import ProgressTracker
+from trongrid_extractor.response import Response
 from trongrid_extractor.trc20_txn import Trc20Txn
 
-JSON_HEADERS = {'Accept': 'application/json'}
 MAX_TRADES_PER_CALL = 200
-RESCUE_WINDOW_DURATION_MS = 20000.0
+
+RESCUE_DURATION_WALKBACK_SECONDS = [
+    20,
+    3600,
+    24 * 3600
+]
+
 ONE_SECOND_MS = 1000.0
 EMPTY_RESPONSE_RETRY_AFTER_SECONDS = 60
 
 # Currently we poll from the most recent to the earliest events which is perhaps non optimal
 ORDER_BY_BLOCK_TIMESTAMP_ASC = 'block_timestamp,asc'
 ORDER_BY_BLOCK_TIMESTAMP_DESC = 'block_timestamp,desc'
 
@@ -50,15 +57,15 @@
         """
         Get events by contract address and write to CSV. This is the endpoint that actually works
         to get all transactions (unlike the '[CONTRACT_ADDRESS]/transactions' endpoint).
 
         Test harness: https://developers.tron.network/v4.0/reference/events-by-contract-address
         """
         contract_url = f"{self.base_uri}contracts/{contract_addr}/events"
-        log.info(f"Retrieving {event_name} events from {since} to {until} from '{contract_url}'")
+        log.info(f"Retrieving '{event_name}' events since {since} until {until} from '{contract_url}'")
         params = Api.build_params(since, until, extra={'event_name': event_name})
         log.info(f"Initial params: {params}")
 
         # Resume from CSV if requested
         if resume_csv:
             if not resume_csv.exists():
                 raise ValueError(f"CSV '{resume_csv}' doesn't exist!")
@@ -68,97 +75,102 @@
             log.info(f"Resuming CSV '{resume_csv}' from {ms_to_datetime(params[MAX_TIMESTAMP])}...")
             output_csv_filename = resume_csv
         else:
             progress_tracker = ProgressTracker()
             output_csv_filename = output_csv_path(contract_addr, output_dir, filename_suffix)
 
         # Start retrieving
-        response = Api.get_response(contract_url, params)
-        retrieved_txns = Trc20Txn.extract_from_events(response)
+        response = Response.get_response(contract_url, params)
+        retrieved_txns = Trc20Txn.extract_from_events(response.response)
         retrieved_txns = progress_tracker.remove_already_processed_txns(retrieved_txns)
         force_continue_from_rescue = False
 
         # Write to CSV
         write_rows(output_csv_filename, retrieved_txns)
 
         # This uses the "next_url" approach which fails after a while.
-        while self._is_continuable_response(response) or force_continue_from_rescue:
+        while response.is_continuable_response() or force_continue_from_rescue:
             force_continue_from_rescue = False
-            next_url = self._next_url(response)
+            next_url = response.next_url()
 
             # Pull the next record
             if next_url is not None:
                 log.debug(f"Retrieving next URL '{next_url}'...")
-                response = Api.get_response(next_url)
-            elif self._is_false_complete_response(response):
+                response = Response.get_response(next_url)
+            elif response.is_false_complete_response():
                 # TODO: this should really use a retry block, otherwise can be an infinite loop
                 log.warning(f"0 row response! Sleeping {EMPTY_RESPONSE_RETRY_AFTER_SECONDS}s and trying again...")
                 log.warning(f"   Params: {params}\n   Response:")
                 pprint(response, expand_all=True)
                 sleep(EMPTY_RESPONSE_RETRY_AFTER_SECONDS)
-                response = Api.get_response(contract_url, params)
+                response = Response.get_response(contract_url, params)
             else:
                 log.error(f"Unparseable response!")
                 pprint(response, expand_all=True)
                 raise ValueError("Unparseable response!")
 
             # Handle case where Trongrid barfs because we paged too much
-            if self._is_paging_complete_response(response):
+            if response.is_paging_complete():
                 log.info(f"Paging complete for {params}.")
-                log.info(f"Seting {MAX_TIMESTAMP} to {progress_tracker.earliest_block_timestamp_seen}")
-                pprint(response, expand_all=True)
+                log.info(f"Setting {MAX_TIMESTAMP} to {progress_tracker.earliest_block_timestamp_seen}")
+
+                # Log a simplified version of the response
+                pprint(response.without_data(), expand_all=True)
                 params[MAX_TIMESTAMP] = progress_tracker.earliest_block_timestamp_seen
-                response = Api.get_response(contract_url, params)
-            elif not response[SUCCESS]:
+                response = Response.get_response(contract_url, params)
+            elif not response.was_successful():
                 # When the "next URL" paging fails we go back to filtering by timestamp but move
                 # the max_timestamp parameter. (I tried something involving the response[META][FINGERPRINT]
                 # but it didn't help.)
                 log.info(f"Failed to retrieve provided next URL. Moving end timestamp and restarting...")
                 log.debug(f"  Next URL: '{next_url}'.\n  Setting {MAX_TIMESTAMP} to {params[MAX_TIMESTAMP]}")
                 params[MAX_TIMESTAMP] = progress_tracker.earliest_block_timestamp_seen
-                response = Api.get_response(contract_url, params)
+                response = Response.get_response(contract_url, params)
 
-            retrieved_txns = Trc20Txn.extract_from_events(response)
+            retrieved_txns = Trc20Txn.extract_from_events(response.response)
             retrieved_txns = progress_tracker.remove_already_processed_txns(retrieved_txns)
 
             # See comment on _rescue_extraction() but tl;dr TronGrid is broken.
             # TODO: is this actually necessary?
             if len(retrieved_txns) == 0:
-                log.warning(f"0 txns found. We seem to be stuck at {ms_to_datetime(params[MAX_TIMESTAMP])}.")
-                log.warning(f"  Last request params: {params}")
-                pprint(response, expand_all=True)
-                retrieved_txns = self._rescue_extraction(contract_url, params)
-                retrieved_txns = progress_tracker.remove_already_processed_txns(retrieved_txns)
-
-                if len(retrieved_txns) > 0:
-                    force_continue_from_rescue = True
-                else:
-                    log.warning(f"Not continuing because _rescue_extraction() returned no rows.")
+                for walkback_seconds in RESCUE_DURATION_WALKBACK_SECONDS:
+                    log.warning(f"0 txns found. We seem to be stuck at {ms_to_datetime(params[MAX_TIMESTAMP])}.")
+                    log.warning(f"  (Maybe) Last request params: {params}")
+                    pprint(response.response, expand_all=True)
+
+                    # Get txns
+                    retrieved_txns = self._rescue_extraction(contract_url, params, walkback_seconds)
+                    retrieved_txns = progress_tracker.remove_already_processed_txns(retrieved_txns)
+
+                    if len(retrieved_txns) > 0:
+                        log.info(f"Rescued {len(retrieved_txns)}, forcibly continuing...")
+                        force_continue_from_rescue = True
+                        break
 
             write_rows(output_csv_filename, retrieved_txns)
 
         log.info("Extraction loop is complete; here is the last response from the api for params: {params}")
         pprint(response, expand_all=True)
         return output_csv_filename
 
     def trc20_xfers_for_wallet(self, contract_addr: str, wallet_addr: str, token_type: str = TRC20) -> List[Trc20Txn]:
         """Use the TRC20 endpoint to get transfers for a particular wallet/token combo."""
         raise ValueError("Needs revision to use ProgressTracker and more.")
         wallet_url = f"{self.base_uri}accounts/{wallet_addr}/transactions/{token_type}"
         params = Api.build_params(extra={'contract_address': contract_addr})
-        response = Api.get_response(wallet_url, params)
+        response = Response.get_response(wallet_url, params)
         txns = Trc20Txn.extract_from_wallet_transactions(response)
 
         while META in response and 'links' in response[META]:
             if DATA not in response or len(response[DATA]) == 0:
                 break
 
             min_timestamp = min([tx.ms_from_epoch for tx in txns])
             params[MAX_TIMESTAMP] = min_timestamp
-            response = Api.get_response(wallet_url, params)
+            response = Response.get_response(wallet_url, params)
             txns.extend(Trc20Txn.extract_from_wallet_transactions(response))
 
         unique_txns = Trc20Txn.unique_txns(txns)
         log.info(f"Extracted a total of {len(txns)} txns ({len(unique_txns)} unique txns).")
         return unique_txns
 
     def txns_for_token(self, contract_addr: str) -> List[Trc20Txn]:
@@ -167,69 +179,54 @@
         events_for_token() and it doesn't work as well.
 
         Test harness: https://developers.tron.network/v4.0/reference/testinput
         """
         raise ValueError("This endpoint doesn't really work.")
         contract_url = f"{self.base_uri}contracts/{contract_addr}/transactions"
         params = Api.build_params(extra={'contract_address': contract_addr})
-        response = Api.get_response(contract_url, params)
+        response = Response.get_response(contract_url, params)
         return response
 
-    def _is_continuable_response(self, response: Dict[str, Any]) -> bool:
-        return self._next_url(response) is not None
-
-    def _is_paging_complete_response(self, response: Dict[str, Any]) -> bool:
-        page_size = self._page_size(response) or 0
-        return response[SUCCESS] and page_size > 0 and self._next_url(response) is None
-
-    def _is_false_complete_response(self, response: Dict[str, Any]) -> bool:
-        """Sometimes for no reason TronGrid just returns 0 rows to a query that would otherwise return rows."""
-        return response[SUCCESS] and self._page_size(response) == 0 and self._next_url(response) is None
-
-    def _next_url(self, response: Dict[str, any]) -> Optional[str]:
-        if META in response and LINKS in response[META] and NEXT in response[META][LINKS]:
-            return response[META][LINKS][NEXT]
-
-    def _page_size(self, response: Dict[str, Any]) -> Optional[int]:
-        if META in response and PAGE_SIZE in response[META]:
-            return response[META][PAGE_SIZE]
-
-    def _rescue_extraction(self, url: str, params: Dict[str, Union[str, float]]) -> List[Trc20Txn]:
+    def _rescue_extraction(self, url: str, params: Dict[str, Union[str, float]], walkback: int) -> List[Trc20Txn]:
         """
         Try a smaller time range; maybe the "next URL" thing will work. The idea here is that the
         'next' URL paging doesn't work very well if you request a large timespan - it only lets
         you retrieve a few pages before barfing. So here we temporarily switch to a much smaller
         time range.
 
+        IMPORTANT: The 'params' dict is modified by this method!
+        'walkback' is the number of seconds between min_timestamp and max_timestamp
+
         Example problematic call:
              extract_tron_transactions TR7NHqjeKQxGTCi8q8ZY4pL8otSzgjLj6t -u 2023-06-26T13:16:24+00:00
         """
-        log.warning(f"Attempting rescue by requesting from max_timestamp minus {RESCUE_WINDOW_DURATION_MS} ms...")
-        log.debug(f"Params: {params}")
+        log.warning(f"Attempting rescue by requesting from max_timestamp minus {walkback} seconds...")
+        log.debug(f"Params before new min_timestamp: {params}")
+
         old_min_timestamp = params[MIN_TIMESTAMP]
-        params[MIN_TIMESTAMP] = params[MAX_TIMESTAMP] - RESCUE_WINDOW_DURATION_MS
-        response = Api.get_response(url, params)
-        txns = Trc20Txn.extract_from_events(response)
+        params[MIN_TIMESTAMP] = params[MAX_TIMESTAMP] - (walkback * 1000.0)
+        response: Response = Response.get_response(url, params)
+        txns = Trc20Txn.extract_from_events(response.response)
         subtract_one_second = True
 
-        while self._is_continuable_response(response):
-            next_url = response[META][LINKS][NEXT]
+        while response.is_continuable_response():
+            next_url = response.next_url()
             log.debug(f"Retrieving next URL '{next_url}'...")
-            response = Api.get_response(next_url)
+            response = Response.get_response(next_url)
 
-            if not response[SUCCESS]:
+            if not response.was_successful():
                 msg = f"Failed to retrieve next_url: '{next_url}'"
                 log.error(f"{msg}\n\nFinal response:")
-                pprint(response, expand_all=True)
+                pprint(response.response, expand_all=True)
                 # If we fail to page all the whole response that means we might not yet have all the
                 # records for that second in time.
                 subtract_one_second = False
                 break
 
-            last_txns = Trc20Txn.extract_from_events(response)
+            last_txns = Trc20Txn.extract_from_events(response.response)
             log.info(f"Rescued {len(last_txns)} more records")
             txns.extend(last_txns)
 
         log.debug(f"Exiting loop; no META or next url. Here's the final response: {response}")
         params[MAX_TIMESTAMP] = params[MIN_TIMESTAMP]
 
         if subtract_one_second:
@@ -237,30 +234,14 @@
 
         params[MIN_TIMESTAMP] = old_min_timestamp
         log.info(f"  Returning {len(txns)} transactions from _rescue_extraction(), modified params in place.")
         log.debug(f"Modified params: {params}")
         return txns
 
     @staticmethod
-    @retry(wait=wait_exponential(multiplier=1, min=4, max=60), stop=stop_after_attempt(7), after=after_log(log, logging.DEBUG))
-    def get_response(url: str, params: Optional[Dict[str, str]] = None) -> Dict[str, Any]:
-        """Hit the endpoint and extract JSON data."""
-        params = params or {}
-
-        # Min/Max timestamps are INCLUSIVE.
-        if MIN_TIMESTAMP in params and MAX_TIMESTAMP in params:
-            msg = f"Requesting records from {ms_to_datetime(params[MIN_TIMESTAMP])} to {ms_to_datetime(params[MAX_TIMESTAMP])}."
-            log.info(msg)
-
-        log.debug(f"\nURL: {url}\nParams: {params}")
-        response = requests.get(url, headers=JSON_HEADERS, params=params).json()
-        log.debug(f"Response: {response}")
-        return response
-
-    @staticmethod
     def build_params(
             min_timestamp: Optional[DateTime] = None,
             max_timestamp: Optional[DateTime] = None,
             extra: Optional[Dict[str, Any]] = None
         ) -> Dict[str, Union[str, float, int]]:
         """Build params for requests. Anything besides min and max timestamp should go in 'extra'."""
         params = {
```

### Comparing `trongrid_extractor-0.3.3/trongrid_extractor/helpers/address_helpers.py` & `trongrid_extractor-0.3.4/trongrid_extractor/helpers/address_helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,37 +6,43 @@
 
 import base58
 
 from trongrid_extractor.helpers.dict_helper import get_dict_key_by_value
 
 TOKEN_ADDRESSES = {
     'TN3W4H6rK2ce4vX9YnFQHwKENnHjoxb3m9': 'BTCT',
+    'TMz2SWatiAtZVVcH2ebpsbVtYwUPT9EdjH': 'BUSD',
     'TUpMhErZL2fhh4sVNULAbNKLokS4GjC1F4': 'TUSD',
     'TEkxiTehnzSmSe2XqrBj4w32RUN966rdz8': 'USDC',
     'TPYmHEhy5n8TCEfYGqW2rPxsghSfzghPDn': 'USDD',
     'TMwFHYXLJaRUPeW6421aqXL4ZEzPRFGkGT': 'USDJ',
     'TR7NHqjeKQxGTCi8q8ZY4pL8otSzgjLj6t': 'USDT',
 }
 
 
 def symbol_for_address(address: str) -> Optional[str]:
     return TOKEN_ADDRESSES.get(address)
 
 
 def hex_to_tron(address: str) -> str:
-    """Convert a hex address to the more commonly used Txxxxxxxxx style."""
-    if (address.startswith('0x')):
+    """Convert a hex address to the more commonly used Txxxxxxxxx base58 style."""
+    if address.startswith('0x'):
         address = '41' + address[2:]
 
-    if (len(address) % 2 == 1):
+    if len(address) % 2 == 1:
         address = '0' + address
 
     return base58.b58encode_check(bytes.fromhex(address)).decode()
 
 
+def tron_to_hex(address: str) -> str:
+    """Convert a Tron base58 address to a hexadecimal string."""
+    return base58.b58decode_check(address).hex()
+
+
 def is_contract_address(address: str) -> bool:
     """Returns true if it looks like a Tron contract address."""
     return address[0] == 'T' and len(address) == 34
 
 
 def address_of_symbol(symbol: str) -> Optional[str]:
     try:
```

### Comparing `trongrid_extractor-0.3.3/trongrid_extractor/helpers/argument_parser.py` & `trongrid_extractor-0.3.4/trongrid_extractor/helpers/argument_parser.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.3/trongrid_extractor/helpers/csv_helper.py` & `trongrid_extractor-0.3.4/trongrid_extractor/helpers/csv_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     dir = dir or Path('')
     filename = csv_prefix(address)
 
     if suffix:
         filename += f"{suffix}_"
 
     filename += csv_suffix()
-    return dir.joinpath(filename)
+    return dir.joinpath(filename.replace(':', '.').replace('/', '.'))
 
 
 def load_csv(csv_path: Union[str, Path]) -> List[Dict[str, Any]]:
     with open(Path(csv_path), mode='r') as csvfile:
         return [
             row
             for row in csv.DictReader(csvfile, delimiter=',')
```

### Comparing `trongrid_extractor-0.3.3/trongrid_extractor/helpers/time_helpers.py` & `trongrid_extractor-0.3.4/trongrid_extractor/helpers/time_helpers.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.3/trongrid_extractor/progress_tracker.py` & `trongrid_extractor-0.3.4/trongrid_extractor/progress_tracker.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.3/trongrid_extractor/trc20_txn.py` & `trongrid_extractor-0.3.4/trongrid_extractor/trc20_txn.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.3/PKG-INFO` & `trongrid_extractor-0.3.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trongrid-extractor
-Version: 0.3.3
+Version: 0.3.4
 Summary: Extract transactions from the Trongrid API.
 Home-page: https://chainargos.com
 Author: Chain Argos
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -74,14 +74,23 @@
 ### Publishing
 1. Update `pyproject.toml` version number
 1. Update `CHANGELOG.md`
 1. `poetry publish --build --repository chain_argos_pypi`
 
 ## TODO
 1. Walk forward not backward
+1. USDT looks incomplete here as 9pm was the last time:
+   ```
+   WARNING - 0 txns found. We seem to be stuck at 2020-07-09T21:04:24+00:00.
+   [2023-06-29, 06:34:36 UTC] {logging_mixin.py:137} INFO -                     WARNING    Last request params:                   api.py:127
+                             {'only_confirmed': 'true', 'limit': 200,
+                             'min_timestamp': 1594252801000.0,
+                             'max_timestamp': 1594328664000.0,
+                             'event_name': 'Transfer'}
+    ```
 1. USDD around this time should be double checked:
    ```
     INFO       Returning 1000 transactions from _rescue_extraction(), modified params in place.                                    api.py:191
     INFO     Writing 1000 rows to 'events_USDD_written_2023-06-28T04.22.00.csv'...                                           csv_helper.py:17
     [06/28/23 10:22:34] INFO       Removed 200 duplicate transactions...                                                                   progress_tracker.py:47
     WARNING  0 txns found. We seem to be stuck at 2023-01-26T03:18:54+00:00.                                                       api.py:103
     WARNING    Last request params: {'only_confirmed': 'true', 'limit': 200, 'min_timestamp': 1483228800000.0, 'max_timestamp':    api.py:104
```

