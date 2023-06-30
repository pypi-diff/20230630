# Comparing `tmp/ntropy_sdk-4.9.0rc8.tar.gz` & `tmp/ntropy_sdk-4.9.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntropy_sdk-4.9.0rc8.tar", last modified: Thu Aug 25 21:30:01 2022, max compression
+gzip compressed data, was "ntropy_sdk-4.9.1rc1.tar", last modified: Fri Aug 26 12:25:35 2022, max compression
```

## Comparing `ntropy_sdk-4.9.0rc8.tar` & `ntropy_sdk-4.9.1rc1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 jorge     (1000) jorge     (1000)        0 2022-08-25 21:30:01.956672 ntropy_sdk-4.9.0rc8/
--rw-r--r--   0 jorge     (1000) jorge     (1000)     3490 2022-07-11 17:04:47.000000 ntropy_sdk-4.9.0rc8/CONTRIBUTING.rst
--rw-r--r--   0 jorge     (1000) jorge     (1000)     1073 2022-07-11 17:04:47.000000 ntropy_sdk-4.9.0rc8/LICENSE
--rw-r--r--   0 jorge     (1000) jorge     (1000)      242 2022-07-11 17:04:47.000000 ntropy_sdk-4.9.0rc8/MANIFEST.in
--rw-r--r--   0 jorge     (1000) jorge     (1000)     2289 2022-08-25 21:30:01.960006 ntropy_sdk-4.9.0rc8/PKG-INFO
--rw-r--r--   0 jorge     (1000) jorge     (1000)     1638 2022-07-27 13:20:46.000000 ntropy_sdk-4.9.0rc8/README.md
-drwxr-xr-x   0 jorge     (1000) jorge     (1000)        0 2022-08-25 21:30:01.956672 ntropy_sdk-4.9.0rc8/ntropy_sdk/
--rw-r--r--   0 jorge     (1000) jorge     (1000)      248 2022-08-25 21:29:58.000000 ntropy_sdk-4.9.0rc8/ntropy_sdk/__init__.py
--rw-r--r--   0 jorge     (1000) jorge     (1000)     3198 2022-08-24 00:26:33.000000 ntropy_sdk-4.9.0rc8/ntropy_sdk/income_check.py
--rw-r--r--   0 jorge     (1000) jorge     (1000)     7413 2022-08-24 00:26:14.000000 ntropy_sdk-4.9.0rc8/ntropy_sdk/models.py
--rw-r--r--   0 jorge     (1000) jorge     (1000)    54958 2022-08-25 12:00:52.000000 ntropy_sdk-4.9.0rc8/ntropy_sdk/ntropy_sdk.py
--rw-r--r--   0 jorge     (1000) jorge     (1000)     2670 2022-08-12 14:40:24.000000 ntropy_sdk-4.9.0rc8/ntropy_sdk/utils.py
-drwxr-xr-x   0 jorge     (1000) jorge     (1000)        0 2022-08-25 21:30:01.956672 ntropy_sdk-4.9.0rc8/ntropy_sdk.egg-info/
--rw-r--r--   0 jorge     (1000) jorge     (1000)     2289 2022-08-25 21:30:01.000000 ntropy_sdk-4.9.0rc8/ntropy_sdk.egg-info/PKG-INFO
--rw-r--r--   0 jorge     (1000) jorge     (1000)      477 2022-08-25 21:30:01.000000 ntropy_sdk-4.9.0rc8/ntropy_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 jorge     (1000) jorge     (1000)        1 2022-08-25 21:30:01.000000 ntropy_sdk-4.9.0rc8/ntropy_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 jorge     (1000) jorge     (1000)       63 2022-08-25 21:30:01.000000 ntropy_sdk-4.9.0rc8/ntropy_sdk.egg-info/entry_points.txt
--rw-r--r--   0 jorge     (1000) jorge     (1000)        1 2022-08-25 21:30:01.000000 ntropy_sdk-4.9.0rc8/ntropy_sdk.egg-info/not-zip-safe
--rw-r--r--   0 jorge     (1000) jorge     (1000)       77 2022-08-25 21:30:01.000000 ntropy_sdk-4.9.0rc8/ntropy_sdk.egg-info/requires.txt
--rw-r--r--   0 jorge     (1000) jorge     (1000)       11 2022-08-25 21:30:01.000000 ntropy_sdk-4.9.0rc8/ntropy_sdk.egg-info/top_level.txt
--rw-r--r--   0 jorge     (1000) jorge     (1000)      538 2022-08-25 21:30:01.960006 ntropy_sdk-4.9.0rc8/setup.cfg
--rw-r--r--   0 jorge     (1000) jorge     (1000)     1455 2022-08-25 21:29:58.000000 ntropy_sdk-4.9.0rc8/setup.py
-drwxr-xr-x   0 jorge     (1000) jorge     (1000)        0 2022-08-25 21:30:01.956672 ntropy_sdk-4.9.0rc8/tests/
--rw-r--r--   0 jorge     (1000) jorge     (1000)      150 2022-07-11 17:04:47.000000 ntropy_sdk-4.9.0rc8/tests/__init__.py
--rw-r--r--   0 jorge     (1000) jorge     (1000)     2956 2022-08-24 00:26:14.000000 ntropy_sdk-4.9.0rc8/tests/test_models.py
--rw-r--r--   0 jorge     (1000) jorge     (1000)    17473 2022-08-18 10:38:09.000000 ntropy_sdk-4.9.0rc8/tests/test_sdk.py
+drwxr-xr-x   0 jorge     (1000) jorge     (1000)        0 2022-08-26 12:25:35.013763 ntropy_sdk-4.9.1rc1/
+-rw-r--r--   0 jorge     (1000) jorge     (1000)     3490 2022-07-11 17:04:47.000000 ntropy_sdk-4.9.1rc1/CONTRIBUTING.rst
+-rw-r--r--   0 jorge     (1000) jorge     (1000)     1073 2022-07-11 17:04:47.000000 ntropy_sdk-4.9.1rc1/LICENSE
+-rw-r--r--   0 jorge     (1000) jorge     (1000)      242 2022-07-11 17:04:47.000000 ntropy_sdk-4.9.1rc1/MANIFEST.in
+-rw-r--r--   0 jorge     (1000) jorge     (1000)     2289 2022-08-26 12:25:35.013763 ntropy_sdk-4.9.1rc1/PKG-INFO
+-rw-r--r--   0 jorge     (1000) jorge     (1000)     1638 2022-07-27 13:20:46.000000 ntropy_sdk-4.9.1rc1/README.md
+drwxr-xr-x   0 jorge     (1000) jorge     (1000)        0 2022-08-26 12:25:35.013763 ntropy_sdk-4.9.1rc1/ntropy_sdk/
+-rw-r--r--   0 jorge     (1000) jorge     (1000)      248 2022-08-26 12:24:47.000000 ntropy_sdk-4.9.1rc1/ntropy_sdk/__init__.py
+-rw-r--r--   0 jorge     (1000) jorge     (1000)     3198 2022-08-25 21:45:04.000000 ntropy_sdk-4.9.1rc1/ntropy_sdk/income_check.py
+-rw-r--r--   0 jorge     (1000) jorge     (1000)     7413 2022-08-25 21:45:04.000000 ntropy_sdk-4.9.1rc1/ntropy_sdk/models.py
+-rw-r--r--   0 jorge     (1000) jorge     (1000)    55794 2022-08-26 11:49:25.000000 ntropy_sdk-4.9.1rc1/ntropy_sdk/ntropy_sdk.py
+-rw-r--r--   0 jorge     (1000) jorge     (1000)     2045 2022-08-26 12:14:36.000000 ntropy_sdk-4.9.1rc1/ntropy_sdk/subscription_management.py
+-rw-r--r--   0 jorge     (1000) jorge     (1000)     2670 2022-08-12 14:40:24.000000 ntropy_sdk-4.9.1rc1/ntropy_sdk/utils.py
+drwxr-xr-x   0 jorge     (1000) jorge     (1000)        0 2022-08-26 12:25:35.013763 ntropy_sdk-4.9.1rc1/ntropy_sdk.egg-info/
+-rw-r--r--   0 jorge     (1000) jorge     (1000)     2289 2022-08-26 12:25:34.000000 ntropy_sdk-4.9.1rc1/ntropy_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 jorge     (1000) jorge     (1000)      515 2022-08-26 12:25:34.000000 ntropy_sdk-4.9.1rc1/ntropy_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 jorge     (1000) jorge     (1000)        1 2022-08-26 12:25:34.000000 ntropy_sdk-4.9.1rc1/ntropy_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 jorge     (1000) jorge     (1000)       63 2022-08-26 12:25:34.000000 ntropy_sdk-4.9.1rc1/ntropy_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 jorge     (1000) jorge     (1000)        1 2022-08-26 12:25:34.000000 ntropy_sdk-4.9.1rc1/ntropy_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 jorge     (1000) jorge     (1000)       77 2022-08-26 12:25:34.000000 ntropy_sdk-4.9.1rc1/ntropy_sdk.egg-info/requires.txt
+-rw-r--r--   0 jorge     (1000) jorge     (1000)       11 2022-08-26 12:25:34.000000 ntropy_sdk-4.9.1rc1/ntropy_sdk.egg-info/top_level.txt
+-rw-r--r--   0 jorge     (1000) jorge     (1000)      538 2022-08-26 12:25:35.017096 ntropy_sdk-4.9.1rc1/setup.cfg
+-rw-r--r--   0 jorge     (1000) jorge     (1000)     1455 2022-08-26 12:24:57.000000 ntropy_sdk-4.9.1rc1/setup.py
+drwxr-xr-x   0 jorge     (1000) jorge     (1000)        0 2022-08-26 12:25:35.013763 ntropy_sdk-4.9.1rc1/tests/
+-rw-r--r--   0 jorge     (1000) jorge     (1000)      150 2022-07-11 17:04:47.000000 ntropy_sdk-4.9.1rc1/tests/__init__.py
+-rw-r--r--   0 jorge     (1000) jorge     (1000)     2956 2022-08-25 21:45:04.000000 ntropy_sdk-4.9.1rc1/tests/test_models.py
+-rw-r--r--   0 jorge     (1000) jorge     (1000)    17473 2022-08-18 10:38:09.000000 ntropy_sdk-4.9.1rc1/tests/test_sdk.py
```

### Comparing `ntropy_sdk-4.9.0rc8/CONTRIBUTING.rst` & `ntropy_sdk-4.9.1rc1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ntropy_sdk-4.9.0rc8/LICENSE` & `ntropy_sdk-4.9.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `ntropy_sdk-4.9.0rc8/PKG-INFO` & `ntropy_sdk-4.9.1rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntropy_sdk
-Version: 4.9.0rc8
+Version: 4.9.1rc1
 Summary: SDK for the Ntropy API
 Home-page: https://github.com/ntropy-network/ntropy-sdk
 Author: David Buchmann
 Author-email: david@ntropy.com
 License: MIT license
 Keywords: ntropy_sdk
 Platform: UNKNOWN
```

### Comparing `ntropy_sdk-4.9.0rc8/README.md` & `ntropy_sdk-4.9.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `ntropy_sdk-4.9.0rc8/ntropy_sdk/income_check.py` & `ntropy_sdk-4.9.1rc1/ntropy_sdk/income_check.py`

 * *Files identical despite different names*

### Comparing `ntropy_sdk-4.9.0rc8/ntropy_sdk/models.py` & `ntropy_sdk-4.9.1rc1/ntropy_sdk/models.py`

 * *Files identical despite different names*

### Comparing `ntropy_sdk-4.9.0rc8/ntropy_sdk/ntropy_sdk.py` & `ntropy_sdk-4.9.1rc1/ntropy_sdk/ntropy_sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import requests
 from pydantic import BaseModel, Field, validator, NonNegativeFloat
 from requests_toolbelt.adapters.socket_options import TCPKeepAliveAdapter
 from tqdm.auto import tqdm
 
 from ntropy_sdk import __version__
 from ntropy_sdk.income_check import IncomeReport
+from ntropy_sdk.subscription_management import SubscriptionReport
 from ntropy_sdk.utils import (
     AccountHolderType,
     EntryType,
     RecurrenceType,
     TransactionType,
     dict_to_str,
     singledispatchmethod,
@@ -270,15 +271,15 @@
         """Returns a dictionary of non-empty fields for a LabeledTransaction.
 
         Returns
         ------
         dict
             A dictionary of the LabeledTransaction's fields.
         """
-        return self.dict()
+        return self.dict(exclude_none=True)
 
 
 class AccountHolder(BaseModel):
     """A financial account holder."""
 
     id: str = Field(
         description="Unique identifier for the account holder in your system."
@@ -1544,14 +1545,36 @@
             raise ValueError("account_holder_id should be of type string")
 
         url = f"/v2/account-holder/{account_holder_id}/income"
 
         response = self.retry_ratelimited_request("POST", url, {})
         return IncomeReport(response.json())
 
+    def get_account_subscription_report(self, account_holder_id: str) -> dict:
+        """Returns the subscription report of an account holder's Transaction history
+
+        Parameters
+        ----------
+        account_holder_id : str
+            The unique identifier for the account holder.
+
+        Returns
+        -------
+        SubscriptionReport:
+            An IncomeReport object for this account holder's history
+        """
+
+        if not isinstance(account_holder_id, str):
+            raise ValueError("account_holder_id should be of type string")
+
+        url = f"/v2/account-holder/{account_holder_id}/subscription"
+
+        response = self.retry_ratelimited_request("POST", url, {})
+        return SubscriptionReport(response.json())
+
     def get_labels(self, account_holder_type: str) -> dict:
         """Returns a hierarchy of possible labels for a specific type.
 
         Parameters
         ----------
         account_holder_type : {"consumer", "business", "freelance", "unknown"}
             The account holder type.
```

### Comparing `ntropy_sdk-4.9.0rc8/ntropy_sdk/utils.py` & `ntropy_sdk-4.9.1rc1/ntropy_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `ntropy_sdk-4.9.0rc8/ntropy_sdk.egg-info/PKG-INFO` & `ntropy_sdk-4.9.1rc1/ntropy_sdk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntropy-sdk
-Version: 4.9.0rc8
+Version: 4.9.1rc1
 Summary: SDK for the Ntropy API
 Home-page: https://github.com/ntropy-network/ntropy-sdk
 Author: David Buchmann
 Author-email: david@ntropy.com
 License: MIT license
 Keywords: ntropy_sdk
 Platform: UNKNOWN
```

### Comparing `ntropy_sdk-4.9.0rc8/setup.cfg` & `ntropy_sdk-4.9.1rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 4.9.0rc8
+current_version = 4.9.1rc1
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(rc(?P<pre>\d+))?
 serialize = 
 	{major}.{minor}.{patch}rc{pre}
 	{major}.{minor}.{patch}
```

### Comparing `ntropy_sdk-4.9.0rc8/setup.py` & `ntropy_sdk-4.9.1rc1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     keywords="ntropy_sdk",
     name="ntropy_sdk",
     packages=find_packages(include=["ntropy_sdk", "ntropy_sdk.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/ntropy-network/ntropy-sdk",
-    version="4.9.0rc8",
+    version="4.9.1rc1",
     zip_safe=False,
 )
```

### Comparing `ntropy_sdk-4.9.0rc8/tests/test_models.py` & `ntropy_sdk-4.9.1rc1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ntropy_sdk-4.9.0rc8/tests/test_sdk.py` & `ntropy_sdk-4.9.1rc1/tests/test_sdk.py`

 * *Files identical despite different names*

