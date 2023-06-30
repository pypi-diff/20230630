# Comparing `tmp/capitalpayments-0.1.3.tar.gz` & `tmp/capitalpayments-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capitalpayments-0.1.3.tar", last modified: Mon May 15 22:01:04 2023, max compression
+gzip compressed data, was "capitalpayments-0.1.4.tar", last modified: Fri Jun 30 19:21:26 2023, max compression
```

## Comparing `capitalpayments-0.1.3.tar` & `capitalpayments-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-15 22:01:04.286302 capitalpayments-0.1.3/
--rw-r--r--   0 javierfernandez   (501) staff       (20)     1066 2023-05-11 21:44:06.000000 capitalpayments-0.1.3/LICENSE
--rw-r--r--   0 javierfernandez   (501) staff       (20)     5871 2023-05-15 22:01:04.286169 capitalpayments-0.1.3/PKG-INFO
--rw-r--r--   0 javierfernandez   (501) staff       (20)     5301 2023-05-15 21:59:57.000000 capitalpayments-0.1.3/README.md
-drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-15 22:01:04.285092 capitalpayments-0.1.3/capitalpayments/
--rw-r--r--   0 javierfernandez   (501) staff       (20)       36 2023-05-12 00:50:40.000000 capitalpayments-0.1.3/capitalpayments/__init__.py
--rw-r--r--   0 javierfernandez   (501) staff       (20)     7598 2023-05-15 21:41:57.000000 capitalpayments-0.1.3/capitalpayments/capitalpaymentscore.py
--rw-r--r--   0 javierfernandez   (501) staff       (20)      620 2023-05-11 23:35:08.000000 capitalpayments-0.1.3/capitalpayments/ipn.py
--rw-r--r--   0 javierfernandez   (501) staff       (20)     1757 2023-05-15 21:47:02.000000 capitalpayments-0.1.3/capitalpayments/url_manager.py
-drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-15 22:01:04.285872 capitalpayments-0.1.3/capitalpayments.egg-info/
--rw-r--r--   0 javierfernandez   (501) staff       (20)     5871 2023-05-15 22:01:04.000000 capitalpayments-0.1.3/capitalpayments.egg-info/PKG-INFO
--rw-r--r--   0 javierfernandez   (501) staff       (20)      341 2023-05-15 22:01:04.000000 capitalpayments-0.1.3/capitalpayments.egg-info/SOURCES.txt
--rw-r--r--   0 javierfernandez   (501) staff       (20)        1 2023-05-15 22:01:04.000000 capitalpayments-0.1.3/capitalpayments.egg-info/dependency_links.txt
--rw-r--r--   0 javierfernandez   (501) staff       (20)        9 2023-05-15 22:01:04.000000 capitalpayments-0.1.3/capitalpayments.egg-info/requires.txt
--rw-r--r--   0 javierfernandez   (501) staff       (20)       16 2023-05-15 22:01:04.000000 capitalpayments-0.1.3/capitalpayments.egg-info/top_level.txt
--rw-r--r--   0 javierfernandez   (501) staff       (20)       38 2023-05-15 22:01:04.286338 capitalpayments-0.1.3/setup.cfg
--rw-r--r--   0 javierfernandez   (501) staff       (20)     1091 2023-05-15 22:00:50.000000 capitalpayments-0.1.3/setup.py
+drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-06-30 19:21:26.802167 capitalpayments-0.1.4/
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     1066 2023-05-11 21:44:06.000000 capitalpayments-0.1.4/LICENSE
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     6258 2023-06-30 19:21:26.802024 capitalpayments-0.1.4/PKG-INFO
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     5689 2023-06-30 19:18:46.000000 capitalpayments-0.1.4/README.md
+drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-06-30 19:21:26.801185 capitalpayments-0.1.4/capitalpayments/
+-rw-r--r--   0 javierfernandez   (501) staff       (20)       36 2023-05-12 00:50:40.000000 capitalpayments-0.1.4/capitalpayments/__init__.py
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     8440 2023-06-30 19:16:38.000000 capitalpayments-0.1.4/capitalpayments/capitalpaymentscore.py
+-rw-r--r--   0 javierfernandez   (501) staff       (20)      620 2023-05-11 23:35:08.000000 capitalpayments-0.1.4/capitalpayments/ipn.py
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     1935 2023-06-30 19:09:46.000000 capitalpayments-0.1.4/capitalpayments/url_manager.py
+drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-06-30 19:21:26.801825 capitalpayments-0.1.4/capitalpayments.egg-info/
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     6258 2023-06-30 19:21:26.000000 capitalpayments-0.1.4/capitalpayments.egg-info/PKG-INFO
+-rw-r--r--   0 javierfernandez   (501) staff       (20)      341 2023-06-30 19:21:26.000000 capitalpayments-0.1.4/capitalpayments.egg-info/SOURCES.txt
+-rw-r--r--   0 javierfernandez   (501) staff       (20)        1 2023-06-30 19:21:26.000000 capitalpayments-0.1.4/capitalpayments.egg-info/dependency_links.txt
+-rw-r--r--   0 javierfernandez   (501) staff       (20)        9 2023-06-30 19:21:26.000000 capitalpayments-0.1.4/capitalpayments.egg-info/requires.txt
+-rw-r--r--   0 javierfernandez   (501) staff       (20)       16 2023-06-30 19:21:26.000000 capitalpayments-0.1.4/capitalpayments.egg-info/top_level.txt
+-rw-r--r--   0 javierfernandez   (501) staff       (20)       38 2023-06-30 19:21:26.802211 capitalpayments-0.1.4/setup.cfg
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     1091 2023-06-30 19:20:59.000000 capitalpayments-0.1.4/setup.py
```

### Comparing `capitalpayments-0.1.3/LICENSE` & `capitalpayments-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `capitalpayments-0.1.3/PKG-INFO` & `capitalpayments-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capitalpayments
-Version: 0.1.3
+Version: 0.1.4
 Summary: For Api Capital Payments
 Author: Javier (leqjl93)
 Author-email: <javier.fernandez.pa93@gmail.com>
 Keywords: python,capitalpayments,paymentprocessor,usdt.trc20
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -110,89 +110,89 @@
 
 from sdk import SDK
 
 sdk = SDK('api_key','api_secret')
 
 # retrieves invoice data
 response = sdk.createInvoice({
-    'invoice_id' => 'invoice_id' # string 
-    'amount' => 'amount' # float|int 
-    'whatsApp' => 'whatsApp' # (optional) int whatsapp full number
-    'name' => 'customer_name' #  (optional) string customer's name
+    'invoice_id' : 'invoice_id' # string 
+    'amount' : 'amount' # float|int 
+    'whatsApp' : 'whatsApp' # (optional) int whatsapp full number
+    'name' : 'customer_name' #  (optional) string customer's name
 })
 
 ```
 # Create invoices
 
 ```
 
 from sdk import SDK
 
 sdk = SDK('api_key','api_secret')
 
 # retrieves invoices data
 response = sdk.createInvoices([
     {
-        'invoice_id' => 'invoice_id' # string 
-        'amount' => 'amount' # float|int 
-        'whatsApp' => 'whatsApp' # (optional) int whatsapp full number
-        'name' => 'customer_name' #  (optional) string customer's name
+        'invoice_id' : 'invoice_id' # string 
+        'amount' : 'amount' # float|int 
+        'whatsApp' : 'whatsApp' # (optional) int whatsapp full number
+        'name' : 'customer_name' #  (optional) string customer's name
     },
     {
-        'invoice_id' => 'invoice_id' # string 
-        'amount' => 'amount' # float|int 
-        'whatsApp' => 'whatsApp' # (optional) int whatsapp full number
-        'name' => 'customer_name' #  (optional) string customer's name
+        'invoice_id' : 'invoice_id' # string 
+        'amount' : 'amount' # float|int 
+        'whatsApp' : 'whatsApp' # (optional) int whatsapp full number
+        'name' : 'customer_name' #  (optional) string customer's name
     }
 ])
 
 ```
 # Get invoice status
 
 ```
 
 from sdk import SDK
 
 sdk = SDK('api_key','api_secret')
 
 # get the invoice status
 response = sdk.getInvoiceStatus({
-    'invoice_id' => 'invoice_id' # string 
+    'invoice_id' : 'invoice_id' # string 
 })
 
 ```
 
 # Cancel invoice
 
 ```
 
 from sdk import SDK
 
 sdk = SDK('api_key','api_secret')
 
 # get the invoice status
 response = sdk.cancelInvoice({
-    'invoice_id' => 'invoice_id' # string 
+    'invoice_id' : 'invoice_id' # string 
 })
 
 ```
 
 # Create payout
 
 ```
 
 from sdk import SDK
 
 sdk = SDK('api_key','api_secret')
 
-# get the payout data
+# retrieve the payout data
 response = sdk.createPayout({
-    'payout_id' => 'payout_id' # string 
-    'amount' => 'amount' # float|int 
-    'address' => 'USDT.TRC20WalletAddress' # string
+    'payout_id' : 'payout_id' # string 
+    'amount' : 'amount' # float|int 
+    'address' : 'USDT.TRC20WalletAddress' # string
 })
 
 ```
 
 # Create payouts
 
 ```
@@ -200,22 +200,22 @@
 from sdk import SDK
 
 sdk = SDK('api_key','api_secret')
 
 # retrieves payouts data
 response = sdk.createPayouts([
     {
-        'payout_id' => 'payout_id' # string 
-        'amount' => 'amount' # float|int 
-        'address' => 'USDT.TRC20WalletAddress' # string
+        'payout_id' : 'payout_id' # string 
+        'amount' : 'amount' # float|int 
+        'address' : 'USDT.TRC20WalletAddress' # string
     },
     {
-        'payout_id' => 'payout_id' # string 
-        'amount' => 'amount' # float|int 
-        'address' => 'USDT.TRC20WalletAddress' # string
+        'payout_id' : 'payout_id' # string 
+        'amount' : 'amount' # float|int 
+        'address' : 'USDT.TRC20WalletAddress' # string
     },
 ])
 
 ```
 
 # Get payout status
 
@@ -223,30 +223,30 @@
 
 from sdk import SDK
 
 sdk = SDK('api_key','api_secret')
 
 # get the payout status
 response = sdk.getPayoutStatus({
-    'payout_id' => 'payout_id' # string 
+    'payout_id' : 'payout_id' # string 
 })
 
 ```
 
 # Cancel payout 
 
 ```
 
 from sdk import SDK
 
 sdk = SDK('api_key','api_secret')
 
 # cancel payout  
 response = sdk.cancelPayout({
-    'payout_id' => 'PayoutId', # @string
+    'payout_id' : 'PayoutId', # @string
 })
 
 ```
 
 # create item
 
 ```
@@ -355,7 +355,38 @@
 sdk = SDK('api_key','api_secret')
 
 # get customer by id
 response = sdk.getCustomer({
     'customer_id' : 'customer_id', # @string
 })
 ```
+
+# set test invoice as payed
+
+```
+
+from sdk import SDK
+
+sdk = SDK('api_key','api_secret')
+
+# requires invoice_id
+response = sdk.setTestInvoiceAsPayed({
+    'invoice_id' : 'invoice_id'
+})
+
+```
+```
+
+# set deposit wallet
+
+```
+
+from sdk import SDK
+
+sdk = SDK('api_key','api_secret')
+
+# requires tron wallet address 
+response = sdk.setDepositWallet({
+    'address' : 'TTCkwzmTZHjN4VSVRVz7s1h5btjWGfvnF9'
+})
+
+```
```

### Comparing `capitalpayments-0.1.3/README.md` & `capitalpayments-0.1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -93,89 +93,89 @@
 
 from sdk import SDK
 
 sdk = SDK('api_key','api_secret')
 
 # retrieves invoice data
 response = sdk.createInvoice({
-    'invoice_id' => 'invoice_id' # string 
-    'amount' => 'amount' # float|int 
-    'whatsApp' => 'whatsApp' # (optional) int whatsapp full number
-    'name' => 'customer_name' #  (optional) string customer's name
+    'invoice_id' : 'invoice_id' # string 
+    'amount' : 'amount' # float|int 
+    'whatsApp' : 'whatsApp' # (optional) int whatsapp full number
+    'name' : 'customer_name' #  (optional) string customer's name
 })
 
 ```
 # Create invoices
 
 ```
 
 from sdk import SDK
 
 sdk = SDK('api_key','api_secret')
 
 # retrieves invoices data
 response = sdk.createInvoices([
     {
-        'invoice_id' => 'invoice_id' # string 
-        'amount' => 'amount' # float|int 
-        'whatsApp' => 'whatsApp' # (optional) int whatsapp full number
-        'name' => 'customer_name' #  (optional) string customer's name
+        'invoice_id' : 'invoice_id' # string 
+        'amount' : 'amount' # float|int 
+        'whatsApp' : 'whatsApp' # (optional) int whatsapp full number
+        'name' : 'customer_name' #  (optional) string customer's name
     },
     {
-        'invoice_id' => 'invoice_id' # string 
-        'amount' => 'amount' # float|int 
-        'whatsApp' => 'whatsApp' # (optional) int whatsapp full number
-        'name' => 'customer_name' #  (optional) string customer's name
+        'invoice_id' : 'invoice_id' # string 
+        'amount' : 'amount' # float|int 
+        'whatsApp' : 'whatsApp' # (optional) int whatsapp full number
+        'name' : 'customer_name' #  (optional) string customer's name
     }
 ])
 
 ```
 # Get invoice status
 
 ```
 
 from sdk import SDK
 
 sdk = SDK('api_key','api_secret')
 
 # get the invoice status
 response = sdk.getInvoiceStatus({
-    'invoice_id' => 'invoice_id' # string 
+    'invoice_id' : 'invoice_id' # string 
 })
 
 ```
 
 # Cancel invoice
 
 ```
 
 from sdk import SDK
 
 sdk = SDK('api_key','api_secret')
 
 # get the invoice status
 response = sdk.cancelInvoice({
-    'invoice_id' => 'invoice_id' # string 
+    'invoice_id' : 'invoice_id' # string 
 })
 
 ```
 
 # Create payout
 
 ```
 
 from sdk import SDK
 
 sdk = SDK('api_key','api_secret')
 
-# get the payout data
+# retrieve the payout data
 response = sdk.createPayout({
-    'payout_id' => 'payout_id' # string 
-    'amount' => 'amount' # float|int 
-    'address' => 'USDT.TRC20WalletAddress' # string
+    'payout_id' : 'payout_id' # string 
+    'amount' : 'amount' # float|int 
+    'address' : 'USDT.TRC20WalletAddress' # string
 })
 
 ```
 
 # Create payouts
 
 ```
@@ -183,22 +183,22 @@
 from sdk import SDK
 
 sdk = SDK('api_key','api_secret')
 
 # retrieves payouts data
 response = sdk.createPayouts([
     {
-        'payout_id' => 'payout_id' # string 
-        'amount' => 'amount' # float|int 
-        'address' => 'USDT.TRC20WalletAddress' # string
+        'payout_id' : 'payout_id' # string 
+        'amount' : 'amount' # float|int 
+        'address' : 'USDT.TRC20WalletAddress' # string
     },
     {
-        'payout_id' => 'payout_id' # string 
-        'amount' => 'amount' # float|int 
-        'address' => 'USDT.TRC20WalletAddress' # string
+        'payout_id' : 'payout_id' # string 
+        'amount' : 'amount' # float|int 
+        'address' : 'USDT.TRC20WalletAddress' # string
     },
 ])
 
 ```
 
 # Get payout status
 
@@ -206,30 +206,30 @@
 
 from sdk import SDK
 
 sdk = SDK('api_key','api_secret')
 
 # get the payout status
 response = sdk.getPayoutStatus({
-    'payout_id' => 'payout_id' # string 
+    'payout_id' : 'payout_id' # string 
 })
 
 ```
 
 # Cancel payout 
 
 ```
 
 from sdk import SDK
 
 sdk = SDK('api_key','api_secret')
 
 # cancel payout  
 response = sdk.cancelPayout({
-    'payout_id' => 'PayoutId', # @string
+    'payout_id' : 'PayoutId', # @string
 })
 
 ```
 
 # create item
 
 ```
@@ -337,8 +337,39 @@
 
 sdk = SDK('api_key','api_secret')
 
 # get customer by id
 response = sdk.getCustomer({
     'customer_id' : 'customer_id', # @string
 })
-```
+```
+
+# set test invoice as payed
+
+```
+
+from sdk import SDK
+
+sdk = SDK('api_key','api_secret')
+
+# requires invoice_id
+response = sdk.setTestInvoiceAsPayed({
+    'invoice_id' : 'invoice_id'
+})
+
+```
+```
+
+# set deposit wallet
+
+```
+
+from sdk import SDK
+
+sdk = SDK('api_key','api_secret')
+
+# requires tron wallet address 
+response = sdk.setDepositWallet({
+    'address' : 'TTCkwzmTZHjN4VSVRVz7s1h5btjWGfvnF9'
+})
+
+```
```

### Comparing `capitalpayments-0.1.3/capitalpayments/capitalpaymentscore.py` & `capitalpayments-0.1.4/capitalpayments/capitalpaymentscore.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,8 +207,30 @@
                 url_manager['get_payout_status'], 
                 headers = {'Content-Type': 'application/json'},
                 auth = (self.api_key, self.api_secret),
                 json = data
             )
             return response.json()
         else: 
+            raise TypeError("Not payout id")
+    def setDepositWallet(self,data):
+        if data.get('address'):
+            response = requests.post(
+                url_manager['set_deposit_wallet'], 
+                headers = {'Content-Type': 'application/json'},
+                auth = (self.api_key, self.api_secret),
+                json = data
+            )
+            return response.json()
+        else: 
+            raise TypeError("Not payout id")
+    def setTestInvoiceAsPayed(self,data):
+        if data.get('invoice_id'):
+            response = requests.post(
+                url_manager['set_invoice_as_payed'], 
+                headers = {'Content-Type': 'application/json'},
+                auth = (self.api_key, self.api_secret),
+                json = data
+            )
+            return response.json()
+        else: 
             raise TypeError("Not payout id")
```

### Comparing `capitalpayments-0.1.3/capitalpayments/ipn.py` & `capitalpayments-0.1.4/capitalpayments/ipn.py`

 * *Files identical despite different names*

### Comparing `capitalpayments-0.1.3/capitalpayments/url_manager.py` & `capitalpayments-0.1.4/capitalpayments/url_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 url_manager = {
     'get_environment': 'https://www.capitalpayments.me/app/api/getEnvironment',
     'get_account': 'https://www.capitalpayments.me/app/api/getAccount',
     'login': 'https://www.capitalpayments.me/app/api/login',
+    'set_deposit_wallet': 'https://www.capitalpayments.me/app/api/setDepositWallet',
 
     # invoices
     'create_invoice': 'https://www.capitalpayments.me/app/api/createInvoice',
     'create_invoices' : 'https://www.capitalpayments.me/app/api/createInvoices',
     'get_invoice_status': 'https://www.capitalpayments.me/app/api/getInvoiceStatus',
     'cancel_invoice': 'https://www.capitalpayments.me/app/api/cancelInvoice',
+    'set_invoice_as_payed' : 'https://www.capitalpayments.me/app/api/setTestInvoiceAsPayed',
     
     # payouts
     'create_payout': 'https://www.capitalpayments.me/app/api/createPayout',
     'create_payouts': 'https://www.capitalpayments.me/app/api/createPayouts',
     'get_payout_status': 'https://www.capitalpayments.me/app/api/getPayoutStatus',
     'cancel_payout': 'https://www.capitalpayments.me/app/api/cancelPayout',
```

### Comparing `capitalpayments-0.1.3/capitalpayments.egg-info/PKG-INFO` & `capitalpayments-0.1.4/capitalpayments.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capitalpayments
-Version: 0.1.3
+Version: 0.1.4
 Summary: For Api Capital Payments
 Author: Javier (leqjl93)
 Author-email: <javier.fernandez.pa93@gmail.com>
 Keywords: python,capitalpayments,paymentprocessor,usdt.trc20
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -110,89 +110,89 @@
 
 from sdk import SDK
 
 sdk = SDK('api_key','api_secret')
 
 # retrieves invoice data
 response = sdk.createInvoice({
-    'invoice_id' => 'invoice_id' # string 
-    'amount' => 'amount' # float|int 
-    'whatsApp' => 'whatsApp' # (optional) int whatsapp full number
-    'name' => 'customer_name' #  (optional) string customer's name
+    'invoice_id' : 'invoice_id' # string 
+    'amount' : 'amount' # float|int 
+    'whatsApp' : 'whatsApp' # (optional) int whatsapp full number
+    'name' : 'customer_name' #  (optional) string customer's name
 })
 
 ```
 # Create invoices
 
 ```
 
 from sdk import SDK
 
 sdk = SDK('api_key','api_secret')
 
 # retrieves invoices data
 response = sdk.createInvoices([
     {
-        'invoice_id' => 'invoice_id' # string 
-        'amount' => 'amount' # float|int 
-        'whatsApp' => 'whatsApp' # (optional) int whatsapp full number
-        'name' => 'customer_name' #  (optional) string customer's name
+        'invoice_id' : 'invoice_id' # string 
+        'amount' : 'amount' # float|int 
+        'whatsApp' : 'whatsApp' # (optional) int whatsapp full number
+        'name' : 'customer_name' #  (optional) string customer's name
     },
     {
-        'invoice_id' => 'invoice_id' # string 
-        'amount' => 'amount' # float|int 
-        'whatsApp' => 'whatsApp' # (optional) int whatsapp full number
-        'name' => 'customer_name' #  (optional) string customer's name
+        'invoice_id' : 'invoice_id' # string 
+        'amount' : 'amount' # float|int 
+        'whatsApp' : 'whatsApp' # (optional) int whatsapp full number
+        'name' : 'customer_name' #  (optional) string customer's name
     }
 ])
 
 ```
 # Get invoice status
 
 ```
 
 from sdk import SDK
 
 sdk = SDK('api_key','api_secret')
 
 # get the invoice status
 response = sdk.getInvoiceStatus({
-    'invoice_id' => 'invoice_id' # string 
+    'invoice_id' : 'invoice_id' # string 
 })
 
 ```
 
 # Cancel invoice
 
 ```
 
 from sdk import SDK
 
 sdk = SDK('api_key','api_secret')
 
 # get the invoice status
 response = sdk.cancelInvoice({
-    'invoice_id' => 'invoice_id' # string 
+    'invoice_id' : 'invoice_id' # string 
 })
 
 ```
 
 # Create payout
 
 ```
 
 from sdk import SDK
 
 sdk = SDK('api_key','api_secret')
 
-# get the payout data
+# retrieve the payout data
 response = sdk.createPayout({
-    'payout_id' => 'payout_id' # string 
-    'amount' => 'amount' # float|int 
-    'address' => 'USDT.TRC20WalletAddress' # string
+    'payout_id' : 'payout_id' # string 
+    'amount' : 'amount' # float|int 
+    'address' : 'USDT.TRC20WalletAddress' # string
 })
 
 ```
 
 # Create payouts
 
 ```
@@ -200,22 +200,22 @@
 from sdk import SDK
 
 sdk = SDK('api_key','api_secret')
 
 # retrieves payouts data
 response = sdk.createPayouts([
     {
-        'payout_id' => 'payout_id' # string 
-        'amount' => 'amount' # float|int 
-        'address' => 'USDT.TRC20WalletAddress' # string
+        'payout_id' : 'payout_id' # string 
+        'amount' : 'amount' # float|int 
+        'address' : 'USDT.TRC20WalletAddress' # string
     },
     {
-        'payout_id' => 'payout_id' # string 
-        'amount' => 'amount' # float|int 
-        'address' => 'USDT.TRC20WalletAddress' # string
+        'payout_id' : 'payout_id' # string 
+        'amount' : 'amount' # float|int 
+        'address' : 'USDT.TRC20WalletAddress' # string
     },
 ])
 
 ```
 
 # Get payout status
 
@@ -223,30 +223,30 @@
 
 from sdk import SDK
 
 sdk = SDK('api_key','api_secret')
 
 # get the payout status
 response = sdk.getPayoutStatus({
-    'payout_id' => 'payout_id' # string 
+    'payout_id' : 'payout_id' # string 
 })
 
 ```
 
 # Cancel payout 
 
 ```
 
 from sdk import SDK
 
 sdk = SDK('api_key','api_secret')
 
 # cancel payout  
 response = sdk.cancelPayout({
-    'payout_id' => 'PayoutId', # @string
+    'payout_id' : 'PayoutId', # @string
 })
 
 ```
 
 # create item
 
 ```
@@ -355,7 +355,38 @@
 sdk = SDK('api_key','api_secret')
 
 # get customer by id
 response = sdk.getCustomer({
     'customer_id' : 'customer_id', # @string
 })
 ```
+
+# set test invoice as payed
+
+```
+
+from sdk import SDK
+
+sdk = SDK('api_key','api_secret')
+
+# requires invoice_id
+response = sdk.setTestInvoiceAsPayed({
+    'invoice_id' : 'invoice_id'
+})
+
+```
+```
+
+# set deposit wallet
+
+```
+
+from sdk import SDK
+
+sdk = SDK('api_key','api_secret')
+
+# requires tron wallet address 
+response = sdk.setDepositWallet({
+    'address' : 'TTCkwzmTZHjN4VSVRVz7s1h5btjWGfvnF9'
+})
+
+```
```

### Comparing `capitalpayments-0.1.3/setup.py` & `capitalpayments-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 DESCRIPTION = 'For Api Capital Payments'
 LONG_DESCRIPTION = 'This SDK connects to Capital Payments Payment Processor Api.'
 
 # Setting up
 setup(
     name="capitalpayments",
     version=VERSION,
```

