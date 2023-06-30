# Comparing `tmp/trongrid_extractor-0.3.6.tar.gz` & `tmp/trongrid_extractor-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trongrid_extractor-0.3.6.tar", max compression
+gzip compressed data, was "trongrid_extractor-0.3.7.tar", max compression
```

## Comparing `trongrid_extractor-0.3.6.tar` & `trongrid_extractor-0.3.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      837 2023-06-30 06:31:51.716505 trongrid_extractor-0.3.6/CHANGELOG.md
--rw-r--r--   0        0        0       36 2023-06-27 21:57:40.566976 trongrid_extractor-0.3.6/LICENSE
--rw-r--r--   0        0        0     3788 2023-06-29 06:44:04.355607 trongrid_extractor-0.3.6/README.md
--rw-r--r--   0        0        0      710 2023-06-30 06:31:51.722193 trongrid_extractor-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      459 2023-06-28 08:24:37.997172 trongrid_extractor-0.3.6/trongrid_extractor/__init__.py
--rw-r--r--   0        0        0    11137 2023-06-30 06:29:48.277928 trongrid_extractor-0.3.6/trongrid_extractor/api.py
--rw-r--r--   0        0        0      326 2023-06-29 00:31:04.580384 trongrid_extractor-0.3.6/trongrid_extractor/config.py
--rw-r--r--   0        0        0     1557 2023-06-30 02:06:04.627281 trongrid_extractor-0.3.6/trongrid_extractor/helpers/address_helpers.py
--rw-r--r--   0        0        0     2243 2023-06-28 19:11:14.811112 trongrid_extractor-0.3.6/trongrid_extractor/helpers/argument_parser.py
--rw-r--r--   0        0        0     2194 2023-06-30 02:06:04.627545 trongrid_extractor-0.3.6/trongrid_extractor/helpers/csv_helper.py
--rw-r--r--   0        0        0      196 2023-06-28 02:11:34.501085 trongrid_extractor-0.3.6/trongrid_extractor/helpers/dict_helper.py
--rw-r--r--   0        0        0      274 2023-06-28 19:37:05.672421 trongrid_extractor-0.3.6/trongrid_extractor/helpers/string_constants.py
--rw-r--r--   0        0        0     1431 2023-06-27 21:52:41.750623 trongrid_extractor-0.3.6/trongrid_extractor/helpers/time_helpers.py
--rw-r--r--   0        0        0     2283 2023-06-28 08:31:15.138247 trongrid_extractor-0.3.6/trongrid_extractor/progress_tracker.py
--rw-r--r--   0        0        0     3667 2023-06-30 06:23:34.464107 trongrid_extractor-0.3.6/trongrid_extractor/response.py
--rw-r--r--   0        0        0     4336 2023-06-28 19:40:28.066469 trongrid_extractor-0.3.6/trongrid_extractor/trc20_txn.py
--rw-r--r--   0        0        0     4430 1970-01-01 00:00:00.000000 trongrid_extractor-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-30 20:58:13.936581 trongrid_extractor-0.3.7/CHANGELOG.md
+-rw-r--r--   0        0        0       36 2023-06-27 21:57:40.566976 trongrid_extractor-0.3.7/LICENSE
+-rw-r--r--   0        0        0     3788 2023-06-29 06:44:04.355607 trongrid_extractor-0.3.7/README.md
+-rw-r--r--   0        0        0      710 2023-06-30 20:58:13.941289 trongrid_extractor-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      459 2023-06-28 08:24:37.997172 trongrid_extractor-0.3.7/trongrid_extractor/__init__.py
+-rw-r--r--   0        0        0    10610 2023-06-30 20:46:17.424340 trongrid_extractor-0.3.7/trongrid_extractor/api.py
+-rw-r--r--   0        0        0      326 2023-06-29 00:31:04.580384 trongrid_extractor-0.3.7/trongrid_extractor/config.py
+-rw-r--r--   0        0        0     1888 2023-06-30 20:53:24.022671 trongrid_extractor-0.3.7/trongrid_extractor/helpers/address_helpers.py
+-rw-r--r--   0        0        0     2243 2023-06-28 19:11:14.811112 trongrid_extractor-0.3.7/trongrid_extractor/helpers/argument_parser.py
+-rw-r--r--   0        0        0     2194 2023-06-30 02:06:04.627545 trongrid_extractor-0.3.7/trongrid_extractor/helpers/csv_helper.py
+-rw-r--r--   0        0        0      196 2023-06-28 02:11:34.501085 trongrid_extractor-0.3.7/trongrid_extractor/helpers/dict_helper.py
+-rw-r--r--   0        0        0      311 2023-06-30 20:08:48.989251 trongrid_extractor-0.3.7/trongrid_extractor/helpers/string_constants.py
+-rw-r--r--   0        0        0     1431 2023-06-27 21:52:41.750623 trongrid_extractor-0.3.7/trongrid_extractor/helpers/time_helpers.py
+-rw-r--r--   0        0        0     3097 2023-06-30 20:48:09.350683 trongrid_extractor-0.3.7/trongrid_extractor/progress_tracker.py
+-rw-r--r--   0        0        0     3741 2023-06-30 19:31:04.142646 trongrid_extractor-0.3.7/trongrid_extractor/response.py
+-rw-r--r--   0        0        0     4336 2023-06-28 19:40:28.066469 trongrid_extractor-0.3.7/trongrid_extractor/trc20_txn.py
+-rw-r--r--   0        0        0     4430 1970-01-01 00:00:00.000000 trongrid_extractor-0.3.7/PKG-INFO
```

### Comparing `trongrid_extractor-0.3.6/CHANGELOG.md` & `trongrid_extractor-0.3.7/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # NEXT RELEASE
 
+### 0.3.7
+* Delete output CSV if it already exists
+* Fix bug with resuming from CSV with out of order rows
+* Only do a rescue when it is impossible to load next page
+* Add a bunch of tokens (`HT`, `SUN`, `JST`, `BTT`, etc.)
+
 ### 0.3.6
 * Simplify inner logic and retries etc.
 
 ### 0.3.5
 * Avoid endless loop on `is_false_complete_response()`
 * Refactor `response.pretty_print()`
 * Don't allow walkbacks to walk back past the start of the period
```

### Comparing `trongrid_extractor-0.3.6/README.md` & `trongrid_extractor-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.6/pyproject.toml` & `trongrid_extractor-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trongrid-extractor"
-version = "0.3.6"
+version = "0.3.7"
 description = "Extract transactions from the Trongrid API."
 authors = ["Chain Argos"]
 readme = "README.md"
 packages = [{include = "trongrid_extractor"}]
 homepage = "https://chainargos.com"
 
 include = [
```

### Comparing `trongrid_extractor-0.3.6/trongrid_extractor/api.py` & `trongrid_extractor-0.3.7/trongrid_extractor/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 '''
 API wrapper for TronGrid.
 '''
+import os
 import tempfile
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 import pendulum
 from pendulum import DateTime
 
@@ -56,87 +57,74 @@
         """
         contract_url = f"{self.base_uri}contracts/{contract_addr}/events"
         log.info(f"Retrieving '{event_name}' events since {since} until {until} from '{contract_url}'")
         params = Api.build_params(since, until, extra={'event_name': event_name})
         log.info(f"Initial params: {params}")
 
         # Resume from CSV if requested
-        if resume_csv:
-            if not resume_csv.exists():
-                raise ValueError(f"CSV '{resume_csv}' doesn't exist!")
-
-            progress_tracker = ProgressTracker.resume_from_csv(resume_csv)
-            params[MAX_TIMESTAMP] = progress_tracker.earliest_block_timestamp_seen
-            log.info(f"Resuming CSV '{resume_csv}' from {ms_to_datetime(params[MAX_TIMESTAMP])}...")
-            output_csv_filename = resume_csv
-        else:
-            progress_tracker = ProgressTracker()
-            output_csv_filename = output_csv_path(contract_addr, output_dir, filename_suffix)
+        output_csv = resume_csv or output_csv_path(contract_addr, output_dir, filename_suffix)
+        progress_tracker = ProgressTracker(output_csv, resume_from_csv=resume_csv is not None)
+        params[MAX_TIMESTAMP] = progress_tracker.earliest_timestamp_seen_ms or params[MAX_TIMESTAMP]
 
         # Start retrieving
         response = Response.get_response(contract_url, params)
-        retrieved_txns = Trc20Txn.extract_from_events(response.response)
-        retrieved_txns = progress_tracker.remove_already_processed_txns(retrieved_txns)
+        retrieved_txns = progress_tracker.process_response(response.response)
+        write_rows(output_csv, retrieved_txns)
         force_continue_from_rescue = False
 
-        # Write to CSV
-        write_rows(output_csv_filename, retrieved_txns)
-
-        # This uses the "next_url" approach which fails after a while.
+        # This uses the "next_url" approach which fails after 5 pages
         while response.is_continuable_response() or force_continue_from_rescue:
-            force_continue_from_rescue = False
-            next_url = response.next_url()
-
             # Pull the next record
-            if next_url is not None:
-                response = Response.get_response(next_url)
+            if response.next_url() is not None:
+                response = Response.get_response(response.next_url())
             elif force_continue_from_rescue:
                 log.info(f"Forcibly continuing so making a request for {params}")
                 response = Response.get_response(contract_url, params)
             else:
                 log.error(f"Unparseable response!")
                 response.pretty_print()
                 raise ValueError("Unparseable response!")
 
+            force_continue_from_rescue = False
+
             # Trongrid doesn't like it when you page more than 5 pages of 200 results. When the
             # "next URL" paging fails we go back to filtering by timestamp but move the
             # max_timestamp parameter back.
             if not response.was_successful():
                 log.info(f"Failed to retrieve provided next URL. Moving end timestamp and restarting...")
-                params[MAX_TIMESTAMP] = progress_tracker.earliest_block_timestamp_seen
+                params[MAX_TIMESTAMP] = progress_tracker.earliest_timestamp_seen_ms
                 response = Response.get_response(contract_url, params)
             elif response.is_paging_complete():
-                log.info(f"Paging complete for {params}, backing up max_timestamp but should we do this?")
+                log.info(f"Paging complete for {params} so will end loop...")
                 response.print_abbreviated()
 
-            retrieved_txns = Trc20Txn.extract_from_events(response.response)
-            retrieved_txns = progress_tracker.remove_already_processed_txns(retrieved_txns)
+            retrieved_txns = progress_tracker.process_response(response.response)
 
             # See comment on _rescue_extraction() but tl;dr TronGrid is broken.
             # TODO: is this actually necessary?
-            if len(retrieved_txns) == 0:
+            if len(retrieved_txns) == 0 and not response.is_continuable_response():
                 for walkback_seconds in RESCUE_DURATION_WALKBACK_SECONDS:
                     log.warning(f"0 txns found. We seem to be stuck at {ms_to_datetime(params[MAX_TIMESTAMP])}.")
                     log.warning(f"  (Maybe) Last request params: {params}")
                     response.print_abbreviated()
 
                     # Get txns
                     retrieved_txns = self._rescue_extraction(contract_url, params, walkback_seconds)
                     retrieved_txns = progress_tracker.remove_already_processed_txns(retrieved_txns)
 
                     if len(retrieved_txns) > 0:
                         log.info(f"Rescued {len(retrieved_txns)}, forcibly continuing...")
                         force_continue_from_rescue = True
                         break
 
-            write_rows(output_csv_filename, retrieved_txns)
+            write_rows(output_csv, retrieved_txns)
 
         log.info("Extraction loop is complete; here is the last response from the api for params: {params}")
         response.print_abbreviated()
-        return output_csv_filename
+        return output_csv
 
     def trc20_xfers_for_wallet(self, contract_addr: str, wallet_addr: str, token_type: str = TRC20) -> List[Trc20Txn]:
         """Use the TRC20 endpoint to get transfers for a particular wallet/token combo."""
         raise ValueError("Needs revision to use ProgressTracker and more.")
         wallet_url = f"{self.base_uri}accounts/{wallet_addr}/transactions/{token_type}"
         params = Api.build_params(extra={'contract_address': contract_addr})
         response = Response.get_response(wallet_url, params)
```

### Comparing `trongrid_extractor-0.3.6/trongrid_extractor/helpers/address_helpers.py` & `trongrid_extractor-0.3.7/trongrid_extractor/helpers/address_helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,21 +5,27 @@
 from typing import Optional
 
 import base58
 
 from trongrid_extractor.helpers.dict_helper import get_dict_key_by_value
 
 TOKEN_ADDRESSES = {
-    'TN3W4H6rK2ce4vX9YnFQHwKENnHjoxb3m9': 'BTCT',
+    'TN3W4H6rK2ce4vX9YnFQHwKENnHjoxb3m9': 'BTCT',  # BTC on Tron (?!)
+    'TAFjULxiVgT4qWk6UZwjqwZXTSaGaqnVp4': 'BTT',
     'TMz2SWatiAtZVVcH2ebpsbVtYwUPT9EdjH': 'BUSD',
+    'TDyvndWuvX5xTBwHPYJi7J3Yq8pq8yh62h': 'HT',    # Huobi Token
+    'TCFLL5dx5ZJdKnWuesXxi1VPwjLVmWZZy9': 'JST',
+    'TSSMHYeV2uE9qYH95DqyoCuNCzEL1NvU3S': 'SUN',
     'TUpMhErZL2fhh4sVNULAbNKLokS4GjC1F4': 'TUSD',
     'TEkxiTehnzSmSe2XqrBj4w32RUN966rdz8': 'USDC',
     'TPYmHEhy5n8TCEfYGqW2rPxsghSfzghPDn': 'USDD',
     'TMwFHYXLJaRUPeW6421aqXL4ZEzPRFGkGT': 'USDJ',
     'TR7NHqjeKQxGTCi8q8ZY4pL8otSzgjLj6t': 'USDT',
+    'TLa2f6VPqDgRE67v1736s7bJ8Ray5wYjU7': 'WIN',
+    'TNUC9Qb1rRpS5CbWLmNMxXBjyFoydXjWFR': 'WTRX',
 }
 
 
 def symbol_for_address(address: str) -> Optional[str]:
     return TOKEN_ADDRESSES.get(address)
```

### Comparing `trongrid_extractor-0.3.6/trongrid_extractor/helpers/argument_parser.py` & `trongrid_extractor-0.3.7/trongrid_extractor/helpers/argument_parser.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.6/trongrid_extractor/helpers/csv_helper.py` & `trongrid_extractor-0.3.7/trongrid_extractor/helpers/csv_helper.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.6/trongrid_extractor/helpers/time_helpers.py` & `trongrid_extractor-0.3.7/trongrid_extractor/helpers/time_helpers.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.6/trongrid_extractor/response.py` & `trongrid_extractor-0.3.7/trongrid_extractor/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         raw_response = requests.get(url, headers=JSON_HEADERS, params=params)
         response = cls(raw_response, deepcopy(params))
 
         if response.is_false_complete_response():
             msg = f"False positive reponse! {response.response}"
             log.error(msg)
             response.pretty_print()
+            log.warning(dump.dump_all(self.raw_response).decode('utf-8'))
             raise ValueError(msg)
 
         return response
 
     def is_continuable_response(self) -> bool:
         return self.next_url() is not None
```

### Comparing `trongrid_extractor-0.3.6/trongrid_extractor/trc20_txn.py` & `trongrid_extractor-0.3.7/trongrid_extractor/trc20_txn.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.6/PKG-INFO` & `trongrid_extractor-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trongrid-extractor
-Version: 0.3.6
+Version: 0.3.7
 Summary: Extract transactions from the Trongrid API.
 Home-page: https://chainargos.com
 Author: Chain Argos
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

