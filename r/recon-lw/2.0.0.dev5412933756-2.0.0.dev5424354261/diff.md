# Comparing `tmp/recon_lw-2.0.0.dev5412933756.tar.gz` & `tmp/recon_lw-2.0.0.dev5424354261.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5412933756.tar", last modified: Thu Jun 29 13:45:40 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5424354261.tar", last modified: Fri Jun 30 15:10:10 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5412933756.tar` & `recon_lw-2.0.0.dev5424354261.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 13:45:40.000000 recon_lw-2.0.0.dev5412933756/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-29 13:44:42.000000 recon_lw-2.0.0.dev5412933756/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-29 13:45:40.000000 recon_lw-2.0.0.dev5412933756/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-29 13:44:42.000000 recon_lw-2.0.0.dev5412933756/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-29 13:45:13.000000 recon_lw-2.0.0.dev5412933756/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 13:45:40.000000 recon_lw-2.0.0.dev5412933756/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-29 13:44:42.000000 recon_lw-2.0.0.dev5412933756/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     4937 2023-06-29 13:44:42.000000 recon_lw-2.0.0.dev5412933756/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-29 13:44:42.000000 recon_lw-2.0.0.dev5412933756/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-06-29 13:44:42.000000 recon_lw-2.0.0.dev5412933756/recon_lw/SequenceCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-06-29 13:44:42.000000 recon_lw-2.0.0.dev5412933756/recon_lw/StateSequenceGenerator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-29 13:44:42.000000 recon_lw-2.0.0.dev5412933756/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-29 13:44:42.000000 recon_lw-2.0.0.dev5412933756/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13503 2023-06-29 13:44:42.000000 recon_lw-2.0.0.dev5412933756/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    34334 2023-06-29 13:44:42.000000 recon_lw-2.0.0.dev5412933756/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    23879 2023-06-29 13:44:42.000000 recon_lw-2.0.0.dev5412933756/recon_lw/recon_ob_cross_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     6293 2023-06-29 13:44:42.000000 recon_lw-2.0.0.dev5412933756/recon_lw/recon_ob_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 13:45:40.000000 recon_lw-2.0.0.dev5412933756/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-29 13:45:40.000000 recon_lw-2.0.0.dev5412933756/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-29 13:45:40.000000 recon_lw-2.0.0.dev5412933756/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-29 13:45:40.000000 recon_lw-2.0.0.dev5412933756/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-29 13:45:40.000000 recon_lw-2.0.0.dev5412933756/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-29 13:45:40.000000 recon_lw-2.0.0.dev5412933756/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-29 13:44:42.000000 recon_lw-2.0.0.dev5412933756/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-29 13:45:40.000000 recon_lw-2.0.0.dev5412933756/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-29 13:44:42.000000 recon_lw-2.0.0.dev5412933756/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 13:45:40.000000 recon_lw-2.0.0.dev5412933756/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-29 13:44:42.000000 recon_lw-2.0.0.dev5412933756/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 15:10:10.000000 recon_lw-2.0.0.dev5424354261/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-30 15:10:10.000000 recon_lw-2.0.0.dev5424354261/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-30 15:09:51.000000 recon_lw-2.0.0.dev5424354261/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 15:10:10.000000 recon_lw-2.0.0.dev5424354261/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4937 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/recon_lw/SequenceCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/recon_lw/StateSequenceGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13503 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34667 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23879 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/recon_lw/recon_ob_cross_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6293 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/recon_lw/recon_ob_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 15:10:10.000000 recon_lw-2.0.0.dev5424354261/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-30 15:10:10.000000 recon_lw-2.0.0.dev5424354261/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-30 15:10:10.000000 recon_lw-2.0.0.dev5424354261/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 15:10:10.000000 recon_lw-2.0.0.dev5424354261/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-30 15:10:10.000000 recon_lw-2.0.0.dev5424354261/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-30 15:10:10.000000 recon_lw-2.0.0.dev5424354261/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-30 15:10:10.000000 recon_lw-2.0.0.dev5424354261/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 15:10:10.000000 recon_lw-2.0.0.dev5424354261/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-30 15:09:26.000000 recon_lw-2.0.0.dev5424354261/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5412933756/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5424354261/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5412933756/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5424354261/recon_lw/LastStateMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5412933756/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5424354261/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5412933756/recon_lw/SequenceCache.py` & `recon_lw-2.0.0.dev5424354261/recon_lw/SequenceCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5412933756/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5424354261/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5412933756/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5424354261/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5412933756/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5424354261/recon_lw/recon_ob.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,39 +377,46 @@
         max_levels = order_book["aggr_max_levels"]
     else:
         log.append(copy.deepcopy(order_book))
 
     return {}, log
 
 
-def ob_trade_order(order_id: str, traded_size: int, str_time_of_event, order_book: dict) -> tuple:
+def ob_trade_order(order_id: str, traded_price: float, traded_size: int, str_time_of_event, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
         reset_aggr_seq(order_book)
 
-    old_side, old_price, old_size = find_order_position(order_id, order_book)
-    log = []
-    if old_side is None:
-        return {"error": order_id + " not found"}, []
-    if traded_size > old_size:
-        return {"error": "traded size > resting size"}, []
-    elif traded_size == old_size:
-        reflect_price_update_in_version(old_side, old_price, str_time_of_event,order_book)
-        order_book[old_side][old_price].pop(order_id)
-        if len(order_book[old_side][old_price]) == 0:
-            order_book[old_side].pop(old_price)
-            log.append(copy.deepcopy(order_book))
+    errors = process_trade(traded_price, order_book)
+    update_time_and_version(str_time_of_event, order_book)
+    order_book["aggr_seq"]["limit_delta"] = 1
+    order_book["aggr_seq"]["top_delta"] = 1
+
+    if order_id is not None:
+        old_side, old_price, old_size = find_order_position(order_id, order_book)
+        log = []
+        if old_side is None:
+            return {"error": order_id + " not found"}, []
+        if traded_size > old_size:
+            return {"error": "traded size > resting size"}, []
+        elif traded_size == old_size:
+            order_book[old_side][old_price].pop(order_id)
+            if len(order_book[old_side][old_price]) == 0:
+                order_book[old_side].pop(old_price)
+                log.append(copy.deepcopy(order_book))
+            else:
+                log.append(copy.deepcopy(order_book))
         else:
+            order_book[old_side][old_price][order_id] -= traded_size
             log.append(copy.deepcopy(order_book))
+        return errors, log
     else:
-        reflect_price_update_in_version(old_side, old_price, str_time_of_event ,order_book)
-        order_book[old_side][old_price][order_id] -= traded_size
-        log.append(copy.deepcopy(order_book))
-    return {}, log
+        return errors, [copy.deepcopy(order_book)]
+
 
 
 def ob_clean_book(str_time_of_event, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
         reset_aggr_seq(order_book)
@@ -590,20 +597,15 @@
 
     update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["top_delta"] = 1
 
     return {}, [copy.deepcopy(order_book)]
 
 
-def ob_market_data_trade(trade_price: float, str_time_of_event, order_book: dict):
-    if "aggr_seq" not in order_book:
-        init_aggr_seq(order_book)
-    else:
-        reset_aggr_seq(order_book)
-
+def process_trade(trade_price: float, order_book: dict):
     errors = {}
     if "max_price" not in order_book or order_book["max_price"] is None:
         order_book["max_price"] = trade_price
 
     if "min_price" not in order_book or order_book["min_price"] is None:
         order_book["min_price"] = trade_price
 
@@ -616,18 +618,28 @@
         order_book["max_price"] = trade_price
     if trade_price < order_book["min_price"]:
         order_book["min_price"] = trade_price
     if "total_n_trades" not in order_book:
         order_book["total_n_trades"] = 1
     else:
         order_book["total_n_trades"] += 1
+    return errors
+
+
+def ob_market_data_trade(trade_price: float, str_time_of_event, order_book: dict):
+    if "aggr_seq" not in order_book:
+        init_aggr_seq(order_book)
+    else:
+        reset_aggr_seq(order_book)
+
+    errors = process_trade(trade_price, order_book)
 
     update_time_and_version(str_time_of_event, order_book)
-    order_book["aggr_seq"]["top_delta"] = 0
-    order_book["aggr_seq"]["limit_delta"] = 0
+    order_book["aggr_seq"]["top_delta"] = 1
+    order_book["aggr_seq"]["limit_delta"] = 1
 
     return errors, [copy.deepcopy(order_book)]
 
 
 def ob_indicative_open_price(open_price: float, open_size: int, 
                              open_mid_price: float, str_time_of_event, order_book: dict):
     if "aggr_seq" not in order_book:
```

### Comparing `recon_lw-2.0.0.dev5412933756/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5424354261/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5412933756/recon_lw/recon_ob_stats.py` & `recon_lw-2.0.0.dev5424354261/recon_lw/recon_ob_stats.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5412933756/recon_lw.egg-info/SOURCES.txt` & `recon_lw-2.0.0.dev5424354261/recon_lw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5412933756/setup.py` & `recon_lw-2.0.0.dev5424354261/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5412933756/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5424354261/test/test_recon_ob.py`

 * *Files identical despite different names*

