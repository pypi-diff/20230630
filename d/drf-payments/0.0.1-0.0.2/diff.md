# Comparing `tmp/drf_payments-0.0.1.tar.gz` & `tmp/drf_payments-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_payments-0.0.1.tar", max compression
+gzip compressed data, was "drf_payments-0.0.2.tar", max compression
```

## Comparing `drf_payments-0.0.1.tar` & `drf_payments-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1072 2023-05-30 11:46:48.880529 drf_payments-0.0.1/LICENSE
--rw-r--r--   0        0        0     3858 2023-06-30 07:12:37.523906 drf_payments-0.0.1/README.md
--rw-r--r--   0        0        0     3266 2023-06-27 09:38:48.343158 drf_payments-0.0.1/drf_payments/__init__.py
--rw-r--r--   0        0        0     2409 2023-06-27 15:07:46.411823 drf_payments-0.0.1/drf_payments/authorizenet/__init__.py
--rw-r--r--   0        0        0     3297 2023-06-27 05:27:03.687434 drf_payments-0.0.1/drf_payments/braintree/__init__.py
--rw-r--r--   0        0        0      956 2023-06-26 10:56:30.963922 drf_payments-0.0.1/drf_payments/constants.py
--rw-r--r--   0        0        0     1790 2023-06-20 06:48:32.729284 drf_payments-0.0.1/drf_payments/core.py
--rw-r--r--   0        0        0     7891 2023-06-27 08:47:58.120027 drf_payments-0.0.1/drf_payments/mixins.py
--rw-r--r--   0        0        0     2991 2023-06-20 10:20:17.278091 drf_payments-0.0.1/drf_payments/models.py
--rw-r--r--   0        0        0     4357 2023-06-30 06:58:16.087869 drf_payments-0.0.1/drf_payments/paypal/__init__.py
--rw-r--r--   0        0        0     8212 2023-06-30 06:33:52.336065 drf_payments-0.0.1/drf_payments/stripe/__init__.py
--rw-r--r--   0        0        0      518 2023-06-26 05:38:01.571605 drf_payments-0.0.1/drf_payments/urls.py
--rw-r--r--   0        0        0     2471 2023-06-30 07:19:58.045338 drf_payments-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4607 1970-01-01 00:00:00.000000 drf_payments-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-30 12:43:53.146039 drf_payments-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3845 2023-06-30 12:43:53.146039 drf_payments-0.0.2/README.md
+-rw-r--r--   0        0        0     3266 2023-06-30 12:43:53.146039 drf_payments-0.0.2/drf_payments/__init__.py
+-rw-r--r--   0        0        0     2831 2023-06-30 12:43:53.150039 drf_payments-0.0.2/drf_payments/authorizenet/__init__.py
+-rw-r--r--   0        0        0     4610 2023-06-30 12:43:53.150039 drf_payments-0.0.2/drf_payments/braintree/__init__.py
+-rw-r--r--   0        0        0      956 2023-06-30 12:43:53.150039 drf_payments-0.0.2/drf_payments/constants.py
+-rw-r--r--   0        0        0     1796 2023-06-30 12:43:53.150039 drf_payments-0.0.2/drf_payments/core.py
+-rw-r--r--   0        0        0     7891 2023-06-30 12:43:53.150039 drf_payments-0.0.2/drf_payments/mixins.py
+-rw-r--r--   0        0        0     2991 2023-06-30 12:43:53.150039 drf_payments-0.0.2/drf_payments/models.py
+-rw-r--r--   0        0        0     4357 2023-06-30 12:43:53.150039 drf_payments-0.0.2/drf_payments/paypal/__init__.py
+-rw-r--r--   0        0        0     8236 2023-06-30 12:43:53.150039 drf_payments-0.0.2/drf_payments/stripe/__init__.py
+-rw-r--r--   0        0        0      518 2023-06-30 12:43:53.150039 drf_payments-0.0.2/drf_payments/urls.py
+-rw-r--r--   0        0        0     3240 2023-06-30 12:43:53.150039 drf_payments-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5076 1970-01-01 00:00:00.000000 drf_payments-0.0.2/PKG-INFO
```

### Comparing `drf_payments-0.0.1/LICENSE` & `drf_payments-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_payments-0.0.1/README.md` & `drf_payments-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # DRF payments
 
 <p align="center">
   <a href="https://dufran.github.io/drf-payments/"><img src="https://img.shields.io/badge/doc-mkdocs-02a6f2?style=flat-square&logo=read-the-docs" alt="Documentation"></a>
-  <a href="https://github.com/dufran/drf-payments/releases/latest"><img src="https://img.shields.io/github/release/dufran/drf-payments.svg?style=flat-square" alt="GitHub release"></a>
   <a href="https://github.com/dufran/drf-payments/actions?workflow=publish"><img src="https://img.shields.io/github/actions/workflow/status/dufran/drf-payments/publish" alt="Build Status"></a>
   <a href="https://github.com/Dufran/drf-payments/actions/workflows/tests.yml" ><img src="https://github.com/Dufran/drf-payments/actions/workflows/tests.yml/badge.svg?branch=main" alt="Tests"/></a>
-
-<a><img src="https://img.shields.io/pypi/pyversions/django-payments"/></a>
-<a><img src="https://img.shields.io/pypi/frameworkversions/django/django-payments"/></a>
-
+<img alt="PyPI" src="https://img.shields.io/pypi/v/drf-payments">
+<a><img src="https://img.shields.io/pypi/pyversions/drf-payments"/></a>
+<a><img src="https://img.shields.io/pypi/frameworkversions/django/drf-payments"/></a>
+<img alt="GitHub tag (latest SemVer pre-release)" src="https://img.shields.io/github/v/tag/dufran/drf-payments">
 </p>
 
 Package to handle various payments provider inside your drf project
 
 This package will allow you to create transactional payments on various payment providers:
 
 - Stripe
```

### Comparing `drf_payments-0.0.1/drf_payments/__init__.py` & `drf_payments-0.0.2/drf_payments/__init__.py`

 * *Files identical despite different names*

### Comparing `drf_payments-0.0.1/drf_payments/authorizenet/__init__.py` & `drf_payments-0.0.2/drf_payments/authorizenet/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,49 @@
 import requests
 
-from drf_payments.constants import PaymentStatus
+from drf_payments.constants import PaymentError, PaymentStatus
 
 from ..core import BasicProvider
 
 RESPONSE_STATUS = {
     "1": PaymentStatus.CONFIRMED,
     "2": PaymentStatus.REJECTED,
 }
 
 
 class AuthorizeNetProvider(BasicProvider):
-    """Payment provider for Authorize.Net.
+    """AuthorizeNetProvider
 
-    This backend implements payments using the Advanced Integration Method (AIM) from
-    `Authorize.Net <https://www.authorize.net/>`_.
-    Due to test environment not create actual transaction currently can't implement refund method
+    AuthorizeNetProvider
+    it handles:
+
+    - Creating a payment
+    - Immediately change payment status due to missing webhook in sanbox mode
+
+    Args:
+        login_id (string): Your authorizenet login_id
+        transaction_key (string): Your authorizenet transaction_key
+        endpoint (string): Your authorizenet endpoint
     """
 
     def __init__(self, login_id, transaction_key, endpoint="https://test.authorize.net/gateway/transact.dll", **kwargs):
         self.login_id = login_id
         self.transaction_key = transaction_key
         self.endpoint = endpoint
 
     def process_payment(self, payment):
-        """Due to official SDK don't support python 3.10 onwards  manual implementation required"""
+        """process_payment
+
+        Create payment and immediately change  status if status OK
+
+        Args:
+            payment (payment): Payment instance
+        """
+        # sourcery skip: dict-assign-update-to-union
+        # * Due to official SDK don't support python 3.10 onwards  manual implementation required
         data = {
             "x_amount": payment.total,
             "x_refId": payment.id,
             "x_currency_code": payment.currency,
             "x_description": payment.description,
             "x_first_name": payment.billing_first_name,
             "x_last_name": payment.billing_last_name,
@@ -44,15 +59,18 @@
             "x_method": "CC",
             "x_type": "AUTH_CAPTURE",
         }
         # *  Append card data to payload
         data.update(payment.extra_data["card"])
         resp = requests.post(self.endpoint, data=data)
         data = resp.text.split("|")
-        message = data[3]
+        try:
+            message = data[3]
+        except IndexError as e:
+            raise PaymentError("Wrong response") from e
         status = "error"
         if resp.ok and RESPONSE_STATUS.get(data[0], False):
             status = RESPONSE_STATUS.get(data[0], status)
             payment.transaction_id = data[6]
             payment.status = status.name
             payment.save(update_fields=["transaction_id", "status"])
         else:
```

### Comparing `drf_payments-0.0.1/drf_payments/constants.py` & `drf_payments-0.0.2/drf_payments/constants.py`

 * *Files identical despite different names*

### Comparing `drf_payments-0.0.1/drf_payments/core.py` & `drf_payments-0.0.2/drf_payments/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Dict, Tuple
 
 from django.conf import settings
 from django.utils.module_loading import import_string
 
-PAYMENT_VARIANTS: Dict[str, Tuple[str, Dict]] = {"default": ("payments.dummy.DummyProvider", {})}
+PAYMENT_VARIANTS: Dict[str, Tuple[str, Dict]] = {"default": ("drf_payments.stripe.StripeProvider", {})}
 
 
 class BasicProvider:
     """Defined a base provider API.
 
     All providers backends should subclass this class.
```

### Comparing `drf_payments-0.0.1/drf_payments/mixins.py` & `drf_payments-0.0.2/drf_payments/mixins.py`

 * *Files identical despite different names*

### Comparing `drf_payments-0.0.1/drf_payments/models.py` & `drf_payments-0.0.2/drf_payments/models.py`

 * *Files identical despite different names*

### Comparing `drf_payments-0.0.1/drf_payments/paypal/__init__.py` & `drf_payments-0.0.2/drf_payments/paypal/__init__.py`

 * *Files identical despite different names*

### Comparing `drf_payments-0.0.1/drf_payments/stripe/__init__.py` & `drf_payments-0.0.2/drf_payments/stripe/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,16 +200,16 @@
         super().__init__(**kwargs)
         self.secret_key = secret_key
         self.public_key = public_key
 
     def process_payment(self, payment):
         """process_payment
 
-        Process payment, require `payment_method.id` to be passed in payment.transaction_id
-        upon creation
+        Process payment, require `payment_method.id` that should be generated on client side and
+        passed in payment.transaction_id
 
         Args:
             payment (payment): Payment instance
         """
         stripe.api_key = self.secret_key
         # * Create payment intent with payment method generated on FE
         intent_data = {
```

### Comparing `drf_payments-0.0.1/drf_payments/urls.py` & `drf_payments-0.0.2/drf_payments/urls.py`

 * *Files identical despite different names*

### Comparing `drf_payments-0.0.1/pyproject.toml` & `drf_payments-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,57 @@
 [tool.poetry]
 authors = ["Oleksandr Korol <oleksandr.korol@coaxsoft.com>"]
-description = ""
+classifiers = [
+  "Framework :: Django :: 3.2",
+  "Framework :: Django :: 4.0",
+  "Framework :: Django :: 4.1",
+  "Framework :: Django :: 4.2",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: BSD License",
+  "Operating System :: OS Independent",
+  "Programming Language :: Python",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Framework :: Django",
+]
+description = "Package to handle various payments provider inside your drf project"
 license = "MIT"
 name = "drf-payments"
 packages = [{include = "drf_payments"}]
 readme = "README.md"
-version = "0.0.1"
+version = "0.0.2"
 [project.urls]
 Documentation = "https://dufran.github.io/drf-payments/"
+Homepage = "https://example.com"
 Repository = "https://github.com/Dufran/drf-payments"
+
 [tool.poetry.dependencies]
 Django = ">3.2.0"
 braintree = "^4.20.0"
 django-phonenumber-field = {extras = ["phonenumberslite"], version = "^7.1.0"}
 djangorestframework = "^3.14.0"
+drf-yasg = "^1.21.5"
 python = ">=3.8"
 stripe = "^5.4"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 ruff = "^0.0.270"
 
 [tool.poetry.group.test.dependencies]
 coverage = {extras = ["toml"], version = "^7.2.7"}
 tox = "^4.6.3"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.3"
-mkdocstrings = {extras = ["python"], version = "^0.22.0"}
-mkdocs-material = "^9.1.17"
 mkdocs-awesome-pages-plugin = "^2.9.1"
+mkdocs-material = "^9.1.17"
+mkdocstrings = {extras = ["python"], version = "^0.22.0"}
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 # Ruff settings
 [tool.ruff]
 ignore = ["RUF005"]
@@ -94,26 +112,30 @@
 show_missing = true
 skip_empty = true
 [tool.tox]
 legacy_tox_ini = """
     [tox]
     env_list =
         py{38,39,310}-django{320}
+        py{38,39,310,311}-django{400}
         py{38,39,310,311}-django{410}
         py{38,39,310,311}-django{420}
-        
+
 
     [testenv]
     allowlist_externals = 
         make
     commands = 
         make tests
     deps = 
         coverage
         tomli
         braintree
         stripe
+        djangorestframework
+        django-phonenumber-field[phonenumberslite]
         django320: Django>=3.2,<3.3
+        django400: Django>=4.0,<4.1
         django410: Django>=4.1,<4.2
         django420: Django>=4.2,<5.0
 
 """
```

### Comparing `drf_payments-0.0.1/PKG-INFO` & `drf_payments-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,48 @@
 Metadata-Version: 2.1
 Name: drf-payments
-Version: 0.0.1
-Summary: 
+Version: 0.0.2
+Summary: Package to handle various payments provider inside your drf project
 License: MIT
 Author: Oleksandr Korol
 Author-email: oleksandr.korol@coaxsoft.com
 Requires-Python: >=3.8
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Django (>3.2.0)
 Requires-Dist: braintree (>=4.20.0,<5.0.0)
 Requires-Dist: django-phonenumber-field[phonenumberslite] (>=7.1.0,<8.0.0)
 Requires-Dist: djangorestframework (>=3.14.0,<4.0.0)
+Requires-Dist: drf-yasg (>=1.21.5,<2.0.0)
 Requires-Dist: stripe (>=5.4,<6.0)
 Description-Content-Type: text/markdown
 
 # DRF payments
 
 <p align="center">
   <a href="https://dufran.github.io/drf-payments/"><img src="https://img.shields.io/badge/doc-mkdocs-02a6f2?style=flat-square&logo=read-the-docs" alt="Documentation"></a>
-  <a href="https://github.com/dufran/drf-payments/releases/latest"><img src="https://img.shields.io/github/release/dufran/drf-payments.svg?style=flat-square" alt="GitHub release"></a>
   <a href="https://github.com/dufran/drf-payments/actions?workflow=publish"><img src="https://img.shields.io/github/actions/workflow/status/dufran/drf-payments/publish" alt="Build Status"></a>
   <a href="https://github.com/Dufran/drf-payments/actions/workflows/tests.yml" ><img src="https://github.com/Dufran/drf-payments/actions/workflows/tests.yml/badge.svg?branch=main" alt="Tests"/></a>
-
-<a><img src="https://img.shields.io/pypi/pyversions/django-payments"/></a>
-<a><img src="https://img.shields.io/pypi/frameworkversions/django/django-payments"/></a>
-
+<img alt="PyPI" src="https://img.shields.io/pypi/v/drf-payments">
+<a><img src="https://img.shields.io/pypi/pyversions/drf-payments"/></a>
+<a><img src="https://img.shields.io/pypi/frameworkversions/django/drf-payments"/></a>
+<img alt="GitHub tag (latest SemVer pre-release)" src="https://img.shields.io/github/v/tag/dufran/drf-payments">
 </p>
 
 Package to handle various payments provider inside your drf project
 
 This package will allow you to create transactional payments on various payment providers:
 
 - Stripe
```

