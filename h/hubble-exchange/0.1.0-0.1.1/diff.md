# Comparing `tmp/hubble_exchange-0.1.0.tar.gz` & `tmp/hubble_exchange-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubble_exchange-0.1.0.tar", last modified: Thu Jun 29 11:54:42 2023, max compression
+gzip compressed data, was "hubble_exchange-0.1.1.tar", last modified: Fri Jun 30 07:14:10 2023, max compression
```

## Comparing `hubble_exchange-0.1.0.tar` & `hubble_exchange-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-06-29 11:54:42.617306 hubble_exchange-0.1.0/
--rw-r--r--   0 shubham    (501) staff       (20)     1072 2023-06-28 09:55:40.000000 hubble_exchange-0.1.0/LICENSE
--rw-r--r--   0 shubham    (501) staff       (20)      101 2023-06-29 11:35:24.000000 hubble_exchange-0.1.0/MANIFEST.in
--rw-r--r--   0 shubham    (501) staff       (20)     1516 2023-06-29 11:54:42.617111 hubble_exchange-0.1.0/PKG-INFO
--rw-r--r--   0 shubham    (501) staff       (20)     2068 2023-06-29 11:42:50.000000 hubble_exchange-0.1.0/README.md
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-06-29 11:54:42.615568 hubble_exchange-0.1.0/hubble_exchange/
--rw-r--r--   0 shubham    (501) staff       (20)      187 2023-06-28 16:09:21.000000 hubble_exchange-0.1.0/hubble_exchange/__init__.py
--rw-r--r--   0 shubham    (501) staff       (20)     5733 2023-06-29 11:30:00.000000 hubble_exchange-0.1.0/hubble_exchange/client.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-06-29 11:54:42.616459 hubble_exchange-0.1.0/hubble_exchange/contract_abis/
--rw-r--r--   0 shubham    (501) staff       (20)    23029 2023-06-28 04:43:57.000000 hubble_exchange-0.1.0/hubble_exchange/contract_abis/OrderBook.json
--rw-r--r--   0 shubham    (501) staff       (20)     2384 2023-06-29 08:43:56.000000 hubble_exchange-0.1.0/hubble_exchange/models.py
--rw-r--r--   0 shubham    (501) staff       (20)     3914 2023-06-29 11:35:10.000000 hubble_exchange-0.1.0/hubble_exchange/order_book.py
--rw-r--r--   0 shubham    (501) staff       (20)     1592 2023-06-29 08:55:15.000000 hubble_exchange-0.1.0/hubble_exchange/utils.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-06-29 11:54:42.616312 hubble_exchange-0.1.0/hubble_exchange.egg-info/
--rw-r--r--   0 shubham    (501) staff       (20)     1516 2023-06-29 11:54:42.000000 hubble_exchange-0.1.0/hubble_exchange.egg-info/PKG-INFO
--rw-r--r--   0 shubham    (501) staff       (20)      427 2023-06-29 11:54:42.000000 hubble_exchange-0.1.0/hubble_exchange.egg-info/SOURCES.txt
--rw-r--r--   0 shubham    (501) staff       (20)        1 2023-06-29 11:54:42.000000 hubble_exchange-0.1.0/hubble_exchange.egg-info/dependency_links.txt
--rw-r--r--   0 shubham    (501) staff       (20)       90 2023-06-29 11:54:42.000000 hubble_exchange-0.1.0/hubble_exchange.egg-info/requires.txt
--rw-r--r--   0 shubham    (501) staff       (20)       16 2023-06-29 11:54:42.000000 hubble_exchange-0.1.0/hubble_exchange.egg-info/top_level.txt
--rw-r--r--   0 shubham    (501) staff       (20)      864 2023-06-29 11:54:20.000000 hubble_exchange-0.1.0/pyproject.toml
--rw-r--r--   0 shubham    (501) staff       (20)       38 2023-06-29 11:54:42.617352 hubble_exchange-0.1.0/setup.cfg
--rw-r--r--   0 shubham    (501) staff       (20)       69 2023-06-29 07:08:06.000000 hubble_exchange-0.1.0/setup.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-06-30 07:14:10.299959 hubble_exchange-0.1.1/
+-rw-r--r--   0 shubham    (501) staff       (20)     1072 2023-06-28 09:55:40.000000 hubble_exchange-0.1.1/LICENSE
+-rw-r--r--   0 shubham    (501) staff       (20)      101 2023-06-29 11:35:24.000000 hubble_exchange-0.1.1/MANIFEST.in
+-rw-r--r--   0 shubham    (501) staff       (20)     1516 2023-06-30 07:14:10.299781 hubble_exchange-0.1.1/PKG-INFO
+-rw-r--r--   0 shubham    (501) staff       (20)     2068 2023-06-29 11:42:50.000000 hubble_exchange-0.1.1/README.md
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-06-30 07:14:10.298042 hubble_exchange-0.1.1/hubble_exchange/
+-rw-r--r--   0 shubham    (501) staff       (20)      187 2023-06-28 16:09:21.000000 hubble_exchange-0.1.1/hubble_exchange/__init__.py
+-rw-r--r--   0 shubham    (501) staff       (20)     5629 2023-06-30 06:44:07.000000 hubble_exchange-0.1.1/hubble_exchange/client.py
+-rw-r--r--   0 shubham    (501) staff       (20)      205 2023-06-30 06:22:24.000000 hubble_exchange-0.1.1/hubble_exchange/constants.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-06-30 07:14:10.299122 hubble_exchange-0.1.1/hubble_exchange/contract_abis/
+-rw-r--r--   0 shubham    (501) staff       (20)    23029 2023-06-28 04:43:57.000000 hubble_exchange-0.1.1/hubble_exchange/contract_abis/OrderBook.json
+-rw-r--r--   0 shubham    (501) staff       (20)     1170 2023-06-30 06:41:16.000000 hubble_exchange-0.1.1/hubble_exchange/eip712.py
+-rw-r--r--   0 shubham    (501) staff       (20)     2384 2023-06-29 08:43:56.000000 hubble_exchange-0.1.1/hubble_exchange/models.py
+-rw-r--r--   0 shubham    (501) staff       (20)     3487 2023-06-30 06:39:11.000000 hubble_exchange-0.1.1/hubble_exchange/order_book.py
+-rw-r--r--   0 shubham    (501) staff       (20)     1592 2023-06-29 08:55:15.000000 hubble_exchange-0.1.1/hubble_exchange/utils.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-06-30 07:14:10.298879 hubble_exchange-0.1.1/hubble_exchange.egg-info/
+-rw-r--r--   0 shubham    (501) staff       (20)     1516 2023-06-30 07:14:10.000000 hubble_exchange-0.1.1/hubble_exchange.egg-info/PKG-INFO
+-rw-r--r--   0 shubham    (501) staff       (20)      482 2023-06-30 07:14:10.000000 hubble_exchange-0.1.1/hubble_exchange.egg-info/SOURCES.txt
+-rw-r--r--   0 shubham    (501) staff       (20)        1 2023-06-30 07:14:10.000000 hubble_exchange-0.1.1/hubble_exchange.egg-info/dependency_links.txt
+-rw-r--r--   0 shubham    (501) staff       (20)      112 2023-06-30 07:14:10.000000 hubble_exchange-0.1.1/hubble_exchange.egg-info/requires.txt
+-rw-r--r--   0 shubham    (501) staff       (20)       16 2023-06-30 07:14:10.000000 hubble_exchange-0.1.1/hubble_exchange.egg-info/top_level.txt
+-rw-r--r--   0 shubham    (501) staff       (20)      896 2023-06-30 07:13:13.000000 hubble_exchange-0.1.1/pyproject.toml
+-rw-r--r--   0 shubham    (501) staff       (20)       38 2023-06-30 07:14:10.300020 hubble_exchange-0.1.1/setup.cfg
+-rw-r--r--   0 shubham    (501) staff       (20)       69 2023-06-29 07:08:06.000000 hubble_exchange-0.1.1/setup.py
```

### Comparing `hubble_exchange-0.1.0/LICENSE` & `hubble_exchange-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.1.0/PKG-INFO` & `hubble_exchange-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubble_exchange
-Version: 0.1.0
+Version: 0.1.1
 Summary: Official python SDK for Hubble Exchange
 Author-email: Lumos <lumos@hubble.exchange>
 License: MIT License
         
         Copyright (c) 2023 Hubble Exchange
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `hubble_exchange-0.1.0/README.md` & `hubble_exchange-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.1.0/hubble_exchange/client.py` & `hubble_exchange-0.1.1/hubble_exchange/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from hexbytes import HexBytes
 from hubble_exchange.models import (
     Order,
     OrderStatusResponse,
     OrderBookDepthResponse,
     GetPositionsResponse,
     OrderBookDepthUpdateResponse,
-    Message,
     WebsocketResponse,
 )
 from hubble_exchange.order_book import OrderBookClient
 from hubble_exchange.utils import (
     get_rpc_endpoint,
     get_websocket_endpoint,
     float_to_scaled_int,
@@ -93,27 +92,25 @@
                 order.salt = get_new_salt()
 
         return self.orderBookClient.place_orders(orders)
 
     def place_single_order(
         self, market: int, base_asset_quantity: float, price: float, reduce_only: bool
     ) -> Order:
-        salt = str(int(time.time())) + str(random.randint(0, 1000))
-        salt_int = int(salt)
         order = Order(
             id=None,
             amm_index=market,
             trader=self.trader_address,
             base_asset_quantity=float_to_scaled_int(base_asset_quantity, 18),
             price=float_to_scaled_int(price, 6),
             salt=get_new_salt(),
             reduce_only=reduce_only,
         )
-        tx_hash = self.orderBookClient.place_order(order)
-        order.id = tx_hash
+        order_hash = self.orderBookClient.place_order(order)
+        order.id = order_hash
         return order
 
     def cancel_orders(self, orders: List[Order]) -> None:
         self.orderBookClient.cancel_orders(orders)
 
     def cancel_order_by_id(self, order_id: HexBytes) -> None:
         order_status = self.get_order_status(order_id)
```

### Comparing `hubble_exchange-0.1.0/hubble_exchange/contract_abis/OrderBook.json` & `hubble_exchange-0.1.1/hubble_exchange/contract_abis/OrderBook.json`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.1.0/hubble_exchange/models.py` & `hubble_exchange-0.1.1/hubble_exchange/models.py`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.1.0/hubble_exchange/utils.py` & `hubble_exchange-0.1.1/hubble_exchange/utils.py`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.1.0/hubble_exchange.egg-info/PKG-INFO` & `hubble_exchange-0.1.1/hubble_exchange.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubble-exchange
-Version: 0.1.0
+Version: 0.1.1
 Summary: Official python SDK for Hubble Exchange
 Author-email: Lumos <lumos@hubble.exchange>
 License: MIT License
         
         Copyright (c) 2023 Hubble Exchange
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `hubble_exchange-0.1.0/pyproject.toml` & `hubble_exchange-0.1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 author_email = "lumos@hubble.exchange"
 long_description = {file = "README.md"}
 long_description_content_type = "text/markdown"
 url = "https://github.com/hubble-exchange/python-sdk"
 
 [project]
 name = "hubble_exchange"
-version = "0.1.0"
+version = "0.1.1"
 description = "Official python SDK for Hubble Exchange"
 authors = [{name = "Lumos", email = "lumos@hubble.exchange"}]
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 dependencies = [
     "web3 >= 6.5.0",
     "eth_typing >= 3.4.0",
     "eth_account >= 0.8.0",
     "requests >= 2.31.0",
-    "websocket-client >= 1.6.0"
+    "websocket-client >= 1.6.0",
+    "eip712-structs >= 1.1.0",
 ]
 keywords = ["hubble", "exchange", "perpetual", "futures", "sdk", "python", "ethereum", "web3"]
 
 [tool.setuptools]
 packages = ["hubble_exchange", "hubble_exchange.contract_abis"]
 include-package-data = true
```

