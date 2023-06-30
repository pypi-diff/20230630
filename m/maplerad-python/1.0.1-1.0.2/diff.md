# Comparing `tmp/maplerad-python-1.0.1.tar.gz` & `tmp/maplerad-python-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maplerad-python-1.0.1.tar", max compression
+gzip compressed data, was "maplerad-python-1.0.2.tar", max compression
```

## Comparing `maplerad-python-1.0.1.tar` & `maplerad-python-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1635 2023-06-30 11:59:06.818135 maplerad-python-1.0.1/LICENSE.md
--rw-r--r--   0        0        0     1689 2023-06-30 14:01:14.299687 maplerad-python-1.0.1/README.md
--rw-r--r--   0        0        0       22 2023-06-29 14:22:53.856818 maplerad-python-1.0.1/maplerad_python/__init__.py
--rw-r--r--   0        0        0     4413 2023-06-30 14:57:46.767749 maplerad-python-1.0.1/maplerad_python/auth.py
--rw-r--r--   0        0        0     4079 2023-06-30 12:52:23.662106 maplerad-python-1.0.1/maplerad_python/bill.py
--rw-r--r--   0        0        0     3319 2023-06-30 12:59:53.614552 maplerad-python-1.0.1/maplerad_python/collections.py
--rw-r--r--   0        0        0     4150 2023-06-30 13:09:39.156429 maplerad-python-1.0.1/maplerad_python/counterparty.py
--rw-r--r--   0        0        0    16208 2023-06-30 12:50:53.346324 maplerad-python-1.0.1/maplerad_python/customer.py
--rw-r--r--   0        0        0     2117 2023-06-30 11:57:51.831240 maplerad-python-1.0.1/maplerad_python/exceptions.py
--rw-r--r--   0        0        0     3968 2023-06-30 13:10:24.258777 maplerad-python-1.0.1/maplerad_python/fx.py
--rw-r--r--   0        0        0     2521 2023-06-30 13:13:03.537385 maplerad-python-1.0.1/maplerad_python/identity.py
--rw-r--r--   0        0        0     3551 2023-06-30 13:16:34.923043 maplerad-python-1.0.1/maplerad_python/institution.py
--rw-r--r--   0        0        0    10745 2023-06-30 14:01:34.074985 maplerad-python-1.0.1/maplerad_python/issuing.py
--rw-r--r--   0        0        0     3853 2023-06-30 13:43:55.160072 maplerad-python-1.0.1/maplerad_python/misc.py
--rw-r--r--   0        0        0     2435 2023-06-30 13:41:16.275583 maplerad-python-1.0.1/maplerad_python/transactions.py
--rw-r--r--   0        0        0     5666 2023-06-30 13:47:47.234067 maplerad-python-1.0.1/maplerad_python/transfer.py
--rw-r--r--   0        0        0     2512 2023-06-30 13:49:05.722874 maplerad-python-1.0.1/maplerad_python/wallets.py
--rw-r--r--   0        0        0      678 2023-06-30 14:59:10.295899 maplerad-python-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2452 2023-06-30 14:59:34.297670 maplerad-python-1.0.1/setup.py
--rw-r--r--   0        0        0     2413 2023-06-30 14:59:34.298495 maplerad-python-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1635 2023-06-30 11:59:06.818135 maplerad-python-1.0.2/LICENSE.md
+-rw-r--r--   0        0        0     1689 2023-06-30 14:01:14.299687 maplerad-python-1.0.2/README.md
+-rw-r--r--   0        0        0       22 2023-06-29 14:22:53.856818 maplerad-python-1.0.2/maplerad_python/__init__.py
+-rw-r--r--   0        0        0     4526 2023-06-30 18:01:50.318694 maplerad-python-1.0.2/maplerad_python/auth.py
+-rw-r--r--   0        0        0     4079 2023-06-30 12:52:23.662106 maplerad-python-1.0.2/maplerad_python/bill.py
+-rw-r--r--   0        0        0     3319 2023-06-30 12:59:53.614552 maplerad-python-1.0.2/maplerad_python/collections.py
+-rw-r--r--   0        0        0     4150 2023-06-30 13:09:39.156429 maplerad-python-1.0.2/maplerad_python/counterparty.py
+-rw-r--r--   0        0        0    16251 2023-06-30 17:39:17.039157 maplerad-python-1.0.2/maplerad_python/customer.py
+-rw-r--r--   0        0        0     2117 2023-06-30 11:57:51.831240 maplerad-python-1.0.2/maplerad_python/exceptions.py
+-rw-r--r--   0        0        0     3968 2023-06-30 13:10:24.258777 maplerad-python-1.0.2/maplerad_python/fx.py
+-rw-r--r--   0        0        0     2521 2023-06-30 13:13:03.537385 maplerad-python-1.0.2/maplerad_python/identity.py
+-rw-r--r--   0        0        0     3551 2023-06-30 13:16:34.923043 maplerad-python-1.0.2/maplerad_python/institution.py
+-rw-r--r--   0        0        0    10745 2023-06-30 14:01:34.074985 maplerad-python-1.0.2/maplerad_python/issuing.py
+-rw-r--r--   0        0        0     3853 2023-06-30 13:43:55.160072 maplerad-python-1.0.2/maplerad_python/misc.py
+-rw-r--r--   0        0        0     2435 2023-06-30 13:41:16.275583 maplerad-python-1.0.2/maplerad_python/transactions.py
+-rw-r--r--   0        0        0     5666 2023-06-30 13:47:47.234067 maplerad-python-1.0.2/maplerad_python/transfer.py
+-rw-r--r--   0        0        0     2512 2023-06-30 13:49:05.722874 maplerad-python-1.0.2/maplerad_python/wallets.py
+-rw-r--r--   0        0        0      678 2023-06-30 17:25:27.964350 maplerad-python-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2452 2023-06-30 18:02:34.288056 maplerad-python-1.0.2/setup.py
+-rw-r--r--   0        0        0     2413 2023-06-30 18:02:34.289193 maplerad-python-1.0.2/PKG-INFO
```

### Comparing `maplerad-python-1.0.1/LICENSE.md` & `maplerad-python-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `maplerad-python-1.0.1/README.md` & `maplerad-python-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `maplerad-python-1.0.1/maplerad_python/auth.py` & `maplerad-python-1.0.2/maplerad_python/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,30 +67,33 @@
 
     def __request_adapter__(self):
         """
         default requests adapter
         """
         session = requests.Session()
         adapter = HTTPAdapter(max_retries=3)
-        for scheme in ["https://","https://"]:
+        for scheme in ["https://","http://"]:
             session.mount(scheme,adapter)
         session.headers.update({
             "accept": "application/json",
             "content-type": "application/json",
             "Authorization": f"Bearer {self.secret_key}"
         })
         return session
     
-    def __request__(self,method,path,**kwargs):
+    def __request__(self, method, path, **kwargs):
         if self.environment == "PRODUCTION":
-            url = "https://api.maplerad.com/"+path
+            url = "https://api.maplerad.com/v1" + path
         else:
-            url = "https://sandbox.api.maplerad.com"+path
-        
-        self.session.request(method,url,json=None,)
+            url = "https://sandbox.api.maplerad.com/v1" + path
+
+        response = self.session.request(method, url=url, **kwargs)
+        print("Request URL:", response.url)  # Print the complete URL
+
+        return response
 
     
     def customer(self):
         """
         customer related
         """
         return Customer(self.__request__)
```

### Comparing `maplerad-python-1.0.1/maplerad_python/bill.py` & `maplerad-python-1.0.2/maplerad_python/bill.py`

 * *Files identical despite different names*

### Comparing `maplerad-python-1.0.1/maplerad_python/collections.py` & `maplerad-python-1.0.2/maplerad_python/collections.py`

 * *Files identical despite different names*

### Comparing `maplerad-python-1.0.1/maplerad_python/counterparty.py` & `maplerad-python-1.0.2/maplerad_python/counterparty.py`

 * *Files identical despite different names*

### Comparing `maplerad-python-1.0.1/maplerad_python/customer.py` & `maplerad-python-1.0.2/maplerad_python/customer.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     def __init__(self, request):
         self.request = request
 
     def create_full_customer(self, payload: dict):
         """
         The class to create the full customer
 
-        :param payload: the request dict as seen in `https://maplerad.dev/docs/create-customer`
+        :param payload: the request dict as seen in `the docs
 
         Usage::
             >>> payload = {
                 "first_name": user.first_name,
                 "last_name": user.last_name,
                 "email": user.email,
                 "identification_number": document_number,
@@ -236,35 +236,36 @@
                 raise ConnectionRefusedError("You are unauthorized due to wrong keys")
             else:
                 return response.json()
 
         except (ConnectionError, ConnectTimeout, HTTPError):
             raise PostException("Error connecting to maplerad")
 
-    def get_all_customers(self):
+    def get_all_customers(self,page:int=1,page_size:int=100):
         """
         Get details of all customers.
 
         :return: JSON response from the API.
 
         Usage:
         >>> from maplerad_python import Authenticate
         >>> auth = Authenticate(secret_key,"DEVELOPMENT")
         >>> result = customer.get_all_customers()
         """
         try:
-            endpoint = "/customers"
+            endpoint = f"/customers?page={page}&page_size={page_size}"
             response = self.request("GET", endpoint)
 
             if response.status_code in (200, 201):
                 return response.json()
             elif response.status_code == 401:
                 raise ConnectionRefusedError("You are unauthorized due to wrong keys")
             else:
                 return response.json()
+            
 
         except (ConnectionError, ConnectTimeout, HTTPError):
             raise PostException("Error connecting to maplerad")
 
     def get_customer_cards(self, customer_id: str):
         """
         Get customer's cards.
```

### Comparing `maplerad-python-1.0.1/maplerad_python/exceptions.py` & `maplerad-python-1.0.2/maplerad_python/exceptions.py`

 * *Files identical despite different names*

### Comparing `maplerad-python-1.0.1/maplerad_python/fx.py` & `maplerad-python-1.0.2/maplerad_python/fx.py`

 * *Files identical despite different names*

### Comparing `maplerad-python-1.0.1/maplerad_python/identity.py` & `maplerad-python-1.0.2/maplerad_python/identity.py`

 * *Files identical despite different names*

### Comparing `maplerad-python-1.0.1/maplerad_python/institution.py` & `maplerad-python-1.0.2/maplerad_python/institution.py`

 * *Files identical despite different names*

### Comparing `maplerad-python-1.0.1/maplerad_python/issuing.py` & `maplerad-python-1.0.2/maplerad_python/issuing.py`

 * *Files identical despite different names*

### Comparing `maplerad-python-1.0.1/maplerad_python/misc.py` & `maplerad-python-1.0.2/maplerad_python/misc.py`

 * *Files identical despite different names*

### Comparing `maplerad-python-1.0.1/maplerad_python/transactions.py` & `maplerad-python-1.0.2/maplerad_python/transactions.py`

 * *Files identical despite different names*

### Comparing `maplerad-python-1.0.1/maplerad_python/transfer.py` & `maplerad-python-1.0.2/maplerad_python/transfer.py`

 * *Files identical despite different names*

### Comparing `maplerad-python-1.0.1/maplerad_python/wallets.py` & `maplerad-python-1.0.2/maplerad_python/wallets.py`

 * *Files identical despite different names*

### Comparing `maplerad-python-1.0.1/pyproject.toml` & `maplerad-python-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maplerad-python"
-version = "1.0.1"
+version = "1.0.2"
 description = "API wrapper for Maplerad"
 authors = ["madvirus-ops <edwinayabie1@gmail.com>"]
 homepage = "https://maplerad.com"
 documentation = "https://maplerad.dev/reference"
 readme="README.md"
 license = "MIT"
 maintainers = [
```

### Comparing `maplerad-python-1.0.1/setup.py` & `maplerad-python-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.31.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'maplerad-python',
-    'version': '1.0.1',
+    'version': '1.0.2',
     'description': 'API wrapper for Maplerad',
     'long_description': '# The Maplerad Python API Wrapper\n\nThe library follows an object-oriented approach\n\nThere are currently twelve (12) base categories namely:\n\n-   Customer\n-   Collections\n-   Transfer\n-   Bills\n-   Wallets\n-   Issuing\n-   Identity\n-   Transactions\n-   Counterparty\n-   Forex\n-   Institutions\n-   Misc\n\n#### Learn more from the [docs](https://maplerad.dev/reference)\n\n# Installation\n\n```shell\n $  pip install maplerad-python\n\n```\n\n# Authorization\n\nA secret key is needed for authorization. It can be gotten from the Maplerad dashboard\n\n# Environments\n\nMaplerad provides two environments to ensure a smooth and easy experience.\n\n-   sandbox: for development\n-   live: for production\n\n## Sandbox\n\nSandbox is your playground. You can credit your test wallets and use that to test your integrations, no real money will be debited or credited.\nEnsure to switch to Live when you are ready to launch.\n\n## Live\n\nAll method calls under Live will be charged and real money will be debited or credited.\nYou are advised to use this when you have fully tested your integrations and are ready to launch your product.\n\n# Usage\n\n```py\n# import the package\nfrom maplerad_python.auth import Authentication\n\n\nsecret_key = os.getenv("MAPLERAD_SECRET_KEY")\nenvironment = "DEVELOPMENT"\n\nauth = Authenticate(secret_key,environment)\n```\n\n## Get all Customers\n\n```py\ncustomer = auth.customers()\nresult = customer.get_all_customers()\n\n```\n\n## Create a Card\n\n```py\nissuing = auth.issuing()\npayload = {\n    "customer_id": "123456789",\n    "type": "VIRTUAL",\n    "currency": "USD",\n    "auto_approve": True,\n    "brand": "VISA",\n    "amount": 1000,\n    "card_pin": 1234\n    }\nresult = issuing.create_card(payload)\n\n\n\n```',
     'author': 'madvirus-ops',
     'author_email': 'edwinayabie1@gmail.com',
     'maintainer': 'madvirus-ops',
     'maintainer_email': 'edwinayabie1@gmail.com',
     'url': 'https://maplerad.com',
```

### Comparing `maplerad-python-1.0.1/PKG-INFO` & `maplerad-python-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maplerad-python
-Version: 1.0.1
+Version: 1.0.2
 Summary: API wrapper for Maplerad
 Home-page: https://maplerad.com
 License: MIT
 Keywords: maplerad,maplerad python package,maplerad python wrapper
 Author: madvirus-ops
 Author-email: edwinayabie1@gmail.com
 Maintainer: madvirus-ops
```

