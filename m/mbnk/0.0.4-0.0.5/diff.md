# Comparing `tmp/mbnk-0.0.4.tar.gz` & `tmp/mbnk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbnk-0.0.4.tar", max compression
+gzip compressed data, was "mbnk-0.0.5.tar", max compression
```

## Comparing `mbnk-0.0.4.tar` & `mbnk-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      692 2023-05-05 16:01:16.349631 mbnk-0.0.4/README.md
--rw-r--r--   0        0        0      290 2023-06-29 11:51:13.889758 mbnk-0.0.4/mbnk/__init__.py
--rw-r--r--   0        0        0      108 2023-06-26 17:49:44.968379 mbnk-0.0.4/mbnk/asyncio/__init__.py
--rw-r--r--   0        0        0     5334 2023-06-29 11:43:17.215861 mbnk-0.0.4/mbnk/asyncio/mbnk.py
--rw-r--r--   0        0        0     2014 2023-06-26 20:24:53.337731 mbnk-0.0.4/mbnk/decorators.py
--rw-r--r--   0        0        0     1031 2023-06-26 19:21:25.551426 mbnk-0.0.4/mbnk/enums.py
--rw-r--r--   0        0        0        0 2023-06-26 17:26:19.588213 mbnk-0.0.4/mbnk/exceptions.py
--rw-r--r--   0        0        0       24 2023-05-05 14:27:50.660629 mbnk-0.0.4/mbnk/instances/__init__.py
--rw-r--r--   0        0        0     1027 2023-05-05 15:24:33.653100 mbnk-0.0.4/mbnk/instances/instances.py
--rw-r--r--   0        0        0     6498 2023-06-26 17:52:49.728848 mbnk-0.0.4/mbnk/monobank.py
--rw-r--r--   0        0        0      554 2023-05-05 15:32:04.350739 mbnk-0.0.4/mbnk/responses.py
--rw-r--r--   0        0        0      104 2023-05-05 14:19:51.878618 mbnk-0.0.4/mbnk/utils/__init__.py
--rw-r--r--   0        0        0      276 2023-06-26 19:48:53.018019 mbnk-0.0.4/mbnk/utils/builders.py
--rw-r--r--   0        0        0      152 2023-06-26 16:15:25.376467 mbnk-0.0.4/mbnk/utils/is_exception.py
--rw-r--r--   0        0        0      141 2023-06-26 16:51:30.107547 mbnk-0.0.4/mbnk/utils/to_camel_case.py
--rw-r--r--   0        0        0      505 2023-05-01 23:52:09.567523 mbnk-0.0.4/mbnk/utils/webhook_authentication.py
--rw-r--r--   0        0        0      313 2023-06-29 11:50:31.722997 mbnk-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 mbnk-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      692 2023-05-05 16:01:16.349631 mbnk-0.0.5/README.md
+-rw-r--r--   0        0        0      290 2023-06-29 11:51:13.889758 mbnk-0.0.5/mbnk/__init__.py
+-rw-r--r--   0        0        0      108 2023-06-26 17:49:44.968379 mbnk-0.0.5/mbnk/asyncio/__init__.py
+-rw-r--r--   0        0        0     5328 2023-06-29 20:11:46.028867 mbnk-0.0.5/mbnk/asyncio/mbnk.py
+-rw-r--r--   0        0        0     2014 2023-06-26 20:24:53.337731 mbnk-0.0.5/mbnk/decorators.py
+-rw-r--r--   0        0        0     1031 2023-06-26 19:21:25.551426 mbnk-0.0.5/mbnk/enums.py
+-rw-r--r--   0        0        0        0 2023-06-26 17:26:19.588213 mbnk-0.0.5/mbnk/exceptions.py
+-rw-r--r--   0        0        0       24 2023-05-05 14:27:50.660629 mbnk-0.0.5/mbnk/instances/__init__.py
+-rw-r--r--   0        0        0     1027 2023-05-05 15:24:33.653100 mbnk-0.0.5/mbnk/instances/instances.py
+-rw-r--r--   0        0        0     6498 2023-06-26 17:52:49.728848 mbnk-0.0.5/mbnk/monobank.py
+-rw-r--r--   0        0        0      554 2023-05-05 15:32:04.350739 mbnk-0.0.5/mbnk/responses.py
+-rw-r--r--   0        0        0      104 2023-05-05 14:19:51.878618 mbnk-0.0.5/mbnk/utils/__init__.py
+-rw-r--r--   0        0        0      276 2023-06-26 19:48:53.018019 mbnk-0.0.5/mbnk/utils/builders.py
+-rw-r--r--   0        0        0      152 2023-06-26 16:15:25.376467 mbnk-0.0.5/mbnk/utils/is_exception.py
+-rw-r--r--   0        0        0      141 2023-06-26 16:51:30.107547 mbnk-0.0.5/mbnk/utils/to_camel_case.py
+-rw-r--r--   0        0        0      505 2023-05-01 23:52:09.567523 mbnk-0.0.5/mbnk/utils/webhook_authentication.py
+-rw-r--r--   0        0        0      313 2023-06-29 20:12:01.856796 mbnk-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 mbnk-0.0.5/PKG-INFO
```

### Comparing `mbnk-0.0.4/README.md` & `mbnk-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mbnk-0.0.4/mbnk/asyncio/mbnk.py` & `mbnk-0.0.5/mbnk/asyncio/mbnk.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,27 +51,27 @@
         self.__headers__ = headers
 
     @async_post_request(url=MonoPayApiUrls.invoice_create)
     def create(
             self,
             amount: int,
             ccy: Optional[int] = None,
-            merchant_payment_info: Optional = None,
+            merchant_paym_info: Optional = None,
             redirect_url: Optional[str] = None,
             web_hook_url: Optional[str] = None,
             validity: Optional[int] = None,
             payment_type: Optional[str] = None,
             qr_id: Optional = None,
             save_card_data: Optional = None,
             **kwargs
     ):
         """
         :param amount:
         :param ccy:
-        :param merchant_payment_info:
+        :param merchant_paym_info:
         :param redirect_url:
         :param web_hook_url:
         :param validity:
         :param payment_type:
         :param qr_id:
         :param save_card_data:
         :return:
```

### Comparing `mbnk-0.0.4/mbnk/decorators.py` & `mbnk-0.0.5/mbnk/decorators.py`

 * *Files identical despite different names*

### Comparing `mbnk-0.0.4/mbnk/enums.py` & `mbnk-0.0.5/mbnk/enums.py`

 * *Files identical despite different names*

### Comparing `mbnk-0.0.4/mbnk/instances/instances.py` & `mbnk-0.0.5/mbnk/instances/instances.py`

 * *Files identical despite different names*

### Comparing `mbnk-0.0.4/mbnk/monobank.py` & `mbnk-0.0.5/mbnk/monobank.py`

 * *Files identical despite different names*

### Comparing `mbnk-0.0.4/mbnk/responses.py` & `mbnk-0.0.5/mbnk/responses.py`

 * *Files identical despite different names*

### Comparing `mbnk-0.0.4/PKG-INFO` & `mbnk-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbnk
-Version: 0.0.4
+Version: 0.0.5
 Summary: Sync/Async version monobank api
 License: MIT
 Author: yeghorkikhai
 Author-email: yeghorkikhai@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

