# Comparing `tmp/chargebee-2.8.4.tar.gz` & `tmp/chargebee-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chargebee-2.8.4.tar", last modified: Thu Jul 22 06:41:33 2021, max compression
+gzip compressed data, was "dist/chargebee-2.9.0.tar", last modified: Mon Aug 16 06:32:58 2021, max compression
```

## Comparing `chargebee-2.8.4.tar` & `chargebee-2.9.0.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 goutham    (535) ec2-user   (500)        0 2021-07-22 06:41:33.000000 chargebee-2.8.4/
--rw-r--r--   0 goutham    (535) ec2-user   (500)       34 2021-07-22 06:20:15.000000 chargebee-2.8.4/MANIFEST.in
--rw-r--r--   0 goutham    (535) ec2-user   (500)       59 2021-07-22 06:41:33.000000 chargebee-2.8.4/setup.cfg
-drwxr-xr-x   0 goutham    (535) ec2-user   (500)        0 2021-07-22 06:41:32.000000 chargebee-2.8.4/chargebee.egg-info/
--rw-r--r--   0 goutham    (535) ec2-user   (500)     2098 2021-07-22 06:41:32.000000 chargebee-2.8.4/chargebee.egg-info/SOURCES.txt
--rw-r--r--   0 goutham    (535) ec2-user   (500)      292 2021-07-22 06:41:32.000000 chargebee-2.8.4/chargebee.egg-info/PKG-INFO
--rw-r--r--   0 goutham    (535) ec2-user   (500)        1 2021-07-22 06:41:32.000000 chargebee-2.8.4/chargebee.egg-info/dependency_links.txt
--rw-r--r--   0 goutham    (535) ec2-user   (500)       10 2021-07-22 06:41:32.000000 chargebee-2.8.4/chargebee.egg-info/top_level.txt
--rw-r--r--   0 goutham    (535) ec2-user   (500)        9 2021-07-22 06:41:32.000000 chargebee-2.8.4/chargebee.egg-info/requires.txt
-drwxr-xr-x   0 goutham    (535) ec2-user   (500)        0 2021-07-22 06:41:32.000000 chargebee-2.8.4/chargebee/
--rw-r--r--   0 goutham    (535) ec2-user   (500)     1314 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/request.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)      309 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/compat.py
-drwxr-xr-x   0 goutham    (535) ec2-user   (500)        0 2021-07-22 06:41:33.000000 chargebee-2.8.4/chargebee/ssl/
--rw-r--r--   0 goutham    (535) ec2-user   (500)   217141 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/ssl/ca-certs.crt
--rw-r--r--   0 goutham    (535) ec2-user   (500)      278 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/__init__.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)       18 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/version.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)      321 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/main.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     3372 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/http_request.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)      872 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/api_error.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)      545 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/environment.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)    15630 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/result.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)      314 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/list_result.py
-drwxr-xr-x   0 goutham    (535) ec2-user   (500)        0 2021-07-22 06:41:33.000000 chargebee-2.8.4/chargebee/models/
--rw-r--r--   0 goutham    (535) ec2-user   (500)     1519 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/card.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     1863 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/time_machine.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     1168 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/usage.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)      232 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/hierarchy.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)      873 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/coupon_code.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     7394 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/customer.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)      437 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/resource_migration.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)      288 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/token.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     1184 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/promotional_credit.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     2417 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/coupon.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     1509 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/event.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     2545 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/__init__.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     1403 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/quote_line_group.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)       70 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/content.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     1691 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/invoice_estimate.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)      177 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/download.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)      862 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/comment.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     2772 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/plan.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     4084 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/hosted_page.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)      779 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/subscription_estimate.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)      662 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/address.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     9024 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/invoice.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     3319 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/transaction.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)      447 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/site_migration_detail.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     1414 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/attached_item.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     1705 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/credit_note_estimate.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)      219 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/third_party_payment_method.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)      361 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/contract_term.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     3971 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/credit_note.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     3901 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/export.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     1096 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/payment_intent.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     4637 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/order.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     4272 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/estimate.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     1634 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/unbilled_charge.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     2166 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/addon.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     1478 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/coupon_set.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     1364 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/item.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     1168 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/portal_session.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     2128 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/quoted_subscription.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)      267 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/contact.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)    10384 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/subscription.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     1478 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/virtual_bank_account.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     2130 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/item_price.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)      525 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/advance_invoice_schedule.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     3718 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/payment_source.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     1053 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/item_family.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     1763 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/gift.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)      573 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/shipping_address.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     6493 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/quote.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     1494 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/models/differential_price.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     2371 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/model.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     1231 2021-07-22 06:20:15.000000 chargebee-2.8.4/chargebee/util.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)      292 2021-07-22 06:41:33.000000 chargebee-2.8.4/PKG-INFO
--rw-r--r--   0 goutham    (535) ec2-user   (500)      776 2021-07-22 06:20:15.000000 chargebee-2.8.4/setup.py
--rw-r--r--   0 goutham    (535) ec2-user   (500)     1546 2021-07-22 06:20:15.000000 chargebee-2.8.4/README.md
+drwxr-xr-x   0 goutham    (535) ec2-user   (500)        0 2021-08-16 06:32:58.000000 chargebee-2.9.0/
+-rw-r--r--   0 goutham    (535) ec2-user   (500)       34 2021-08-16 06:27:37.000000 chargebee-2.9.0/MANIFEST.in
+-rw-r--r--   0 goutham    (535) ec2-user   (500)       59 2021-08-16 06:32:58.000000 chargebee-2.9.0/setup.cfg
+drwxr-xr-x   0 goutham    (535) ec2-user   (500)        0 2021-08-16 06:32:58.000000 chargebee-2.9.0/chargebee.egg-info/
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     2132 2021-08-16 06:32:58.000000 chargebee-2.9.0/chargebee.egg-info/SOURCES.txt
+-rw-r--r--   0 goutham    (535) ec2-user   (500)      292 2021-08-16 06:32:58.000000 chargebee-2.9.0/chargebee.egg-info/PKG-INFO
+-rw-r--r--   0 goutham    (535) ec2-user   (500)        1 2021-08-16 06:32:58.000000 chargebee-2.9.0/chargebee.egg-info/dependency_links.txt
+-rw-r--r--   0 goutham    (535) ec2-user   (500)       10 2021-08-16 06:32:58.000000 chargebee-2.9.0/chargebee.egg-info/top_level.txt
+-rw-r--r--   0 goutham    (535) ec2-user   (500)        9 2021-08-16 06:32:58.000000 chargebee-2.9.0/chargebee.egg-info/requires.txt
+drwxr-xr-x   0 goutham    (535) ec2-user   (500)        0 2021-08-16 06:32:58.000000 chargebee-2.9.0/chargebee/
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     1314 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/request.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)      309 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/compat.py
+drwxr-xr-x   0 goutham    (535) ec2-user   (500)        0 2021-08-16 06:32:58.000000 chargebee-2.9.0/chargebee/ssl/
+-rw-r--r--   0 goutham    (535) ec2-user   (500)   217141 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/ssl/ca-certs.crt
+-rw-r--r--   0 goutham    (535) ec2-user   (500)      278 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/__init__.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)       18 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/version.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)      321 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/main.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     3372 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/http_request.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)      872 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/api_error.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)      545 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/environment.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)    15917 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/result.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)      314 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/list_result.py
+drwxr-xr-x   0 goutham    (535) ec2-user   (500)        0 2021-08-16 06:32:58.000000 chargebee-2.9.0/chargebee/models/
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     1519 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/card.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     1863 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/time_machine.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     1168 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/usage.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)      232 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/hierarchy.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)      873 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/coupon_code.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     7394 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/customer.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)      437 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/resource_migration.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)      288 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/token.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     1184 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/promotional_credit.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     2417 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/coupon.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     1509 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/event.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     2545 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/__init__.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     1403 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/quote_line_group.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)       70 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/content.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     1691 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/invoice_estimate.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)      177 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/download.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)      862 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/comment.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     2772 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/plan.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     4084 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/hosted_page.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)      779 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/subscription_estimate.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)      662 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/address.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     9040 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/invoice.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     3335 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/transaction.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)      447 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/site_migration_detail.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     1226 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/attached_item.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     1705 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/credit_note_estimate.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)      219 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/third_party_payment_method.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)      361 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/contract_term.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     3987 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/credit_note.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)      982 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/quoted_charge.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     3901 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/export.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     1096 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/payment_intent.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     4637 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/order.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     4272 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/estimate.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     1634 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/unbilled_charge.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     2166 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/addon.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     1478 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/coupon_set.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     1364 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/item.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     1168 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/portal_session.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     1850 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/quoted_subscription.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)      267 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/contact.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)    10408 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/subscription.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     1478 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/virtual_bank_account.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     2130 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/item_price.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)      525 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/advance_invoice_schedule.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     3718 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/payment_source.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     1053 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/item_family.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     1763 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/gift.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)      573 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/shipping_address.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     6493 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/quote.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     1494 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/models/differential_price.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     2371 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/model.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     1231 2021-08-16 06:27:36.000000 chargebee-2.9.0/chargebee/util.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)      292 2021-08-16 06:32:58.000000 chargebee-2.9.0/PKG-INFO
+-rw-r--r--   0 goutham    (535) ec2-user   (500)      776 2021-08-16 06:27:37.000000 chargebee-2.9.0/setup.py
+-rw-r--r--   0 goutham    (535) ec2-user   (500)     1546 2021-08-16 06:27:37.000000 chargebee-2.9.0/README.md
```

### Comparing `chargebee-2.8.4/chargebee.egg-info/SOURCES.txt` & `chargebee-2.9.0/chargebee.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 chargebee/models/payment_intent.py
 chargebee/models/payment_source.py
 chargebee/models/plan.py
 chargebee/models/portal_session.py
 chargebee/models/promotional_credit.py
 chargebee/models/quote.py
 chargebee/models/quote_line_group.py
+chargebee/models/quoted_charge.py
 chargebee/models/quoted_subscription.py
 chargebee/models/resource_migration.py
 chargebee/models/shipping_address.py
 chargebee/models/site_migration_detail.py
 chargebee/models/subscription.py
 chargebee/models/subscription_estimate.py
 chargebee/models/third_party_payment_method.py
```

### Comparing `chargebee-2.8.4/chargebee/request.py` & `chargebee-2.9.0/chargebee/request.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/ssl/ca-certs.crt` & `chargebee-2.9.0/chargebee/ssl/ca-certs.crt`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/http_request.py` & `chargebee-2.9.0/chargebee/http_request.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/api_error.py` & `chargebee-2.9.0/chargebee/api_error.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/environment.py` & `chargebee-2.9.0/chargebee/environment.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/result.py` & `chargebee-2.9.0/chargebee/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,18 +136,24 @@
         quote = self._get('quote', Quote,
         {'line_items' : Quote.LineItem, 'discounts' : Quote.Discount, 'line_item_discounts' : Quote.LineItemDiscount, 'taxes' : Quote.Tax, 'line_item_taxes' : Quote.LineItemTax, 'line_item_tiers' : Quote.LineItemTier, 'shipping_address' : Quote.ShippingAddress, 'billing_address' : Quote.BillingAddress});
         return quote;
 
     @property
     def quoted_subscription(self):
         quoted_subscription = self._get('quoted_subscription', QuotedSubscription,
-        {'addons' : QuotedSubscription.Addon, 'event_based_addons' : QuotedSubscription.EventBasedAddon, 'coupons' : QuotedSubscription.Coupon, 'discounts' : QuotedSubscription.Discount, 'subscription_items' : QuotedSubscription.SubscriptionItem, 'item_tiers' : QuotedSubscription.ItemTier, 'quoted_contract_term' : QuotedSubscription.QuotedContractTerm});
+        {'addons' : QuotedSubscription.Addon, 'event_based_addons' : QuotedSubscription.EventBasedAddon, 'coupons' : QuotedSubscription.Coupon, 'subscription_items' : QuotedSubscription.SubscriptionItem, 'item_tiers' : QuotedSubscription.ItemTier, 'quoted_contract_term' : QuotedSubscription.QuotedContractTerm});
         return quoted_subscription;
 
     @property
+    def quoted_charge(self):
+        quoted_charge = self._get('quoted_charge', QuotedCharge,
+        {'charges' : QuotedCharge.Charge, 'addons' : QuotedCharge.Addon, 'invoice_items' : QuotedCharge.InvoiceItem, 'item_tiers' : QuotedCharge.ItemTier, 'coupons' : QuotedCharge.Coupon});
+        return quoted_charge;
+
+    @property
     def quote_line_group(self):
         quote_line_group = self._get('quote_line_group', QuoteLineGroup,
         {'line_items' : QuoteLineGroup.LineItem, 'discounts' : QuoteLineGroup.Discount, 'line_item_discounts' : QuoteLineGroup.LineItemDiscount, 'taxes' : QuoteLineGroup.Tax, 'line_item_taxes' : QuoteLineGroup.LineItemTax});
         return quote_line_group;
 
     @property
     def plan(self):
@@ -232,15 +238,14 @@
 
     @property
     def payment_intent(self):
         payment_intent = self._get('payment_intent', PaymentIntent,
         {'payment_attempt' : PaymentIntent.PaymentAttempt});
         return payment_intent;
 
-
     @property
     def item_family(self):
         item_family = self._get('item_family', ItemFamily);
         return item_family;
 
     @property
     def item(self):
@@ -261,14 +266,15 @@
 
     @property
     def differential_price(self):
         differential_price = self._get('differential_price', DifferentialPrice,
         {'tiers' : DifferentialPrice.Tier, 'parent_periods' : DifferentialPrice.ParentPeriod});
         return differential_price;
 
+
     @property
     def unbilled_charges(self):
         unbilled_charges = self._get_list('unbilled_charges', UnbilledCharge,
         {'tiers' : UnbilledCharge.Tier});
         return unbilled_charges;
 
     @property
@@ -297,14 +303,15 @@
 
     @property
     def differential_prices(self):
         differential_prices = self._get_list('differential_prices', DifferentialPrice,
         {'tiers' : DifferentialPrice.Tier, 'parent_periods' : DifferentialPrice.ParentPeriod});
         return differential_prices;
 
+
     def _get_list(self, type, cls, sub_types={}, dependant_types={}, dependant_sub_types={}):
         if not type in self._response:
             return None
         
         set_val = []
         for obj in self._response[type]:
             if isinstance(obj, dict):
```

### Comparing `chargebee-2.8.4/chargebee/models/card.py` & `chargebee-2.9.0/chargebee/models/card.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/time_machine.py` & `chargebee-2.9.0/chargebee/models/time_machine.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/usage.py` & `chargebee-2.9.0/chargebee/models/usage.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/coupon_code.py` & `chargebee-2.9.0/chargebee/models/coupon_code.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/customer.py` & `chargebee-2.9.0/chargebee/models/customer.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/promotional_credit.py` & `chargebee-2.9.0/chargebee/models/promotional_credit.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/coupon.py` & `chargebee-2.9.0/chargebee/models/coupon.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/event.py` & `chargebee-2.9.0/chargebee/models/event.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/__init__.py` & `chargebee-2.9.0/chargebee/models/__init__.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/quote_line_group.py` & `chargebee-2.9.0/chargebee/models/quote_line_group.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/invoice_estimate.py` & `chargebee-2.9.0/chargebee/models/invoice_estimate.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/comment.py` & `chargebee-2.9.0/chargebee/models/comment.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/plan.py` & `chargebee-2.9.0/chargebee/models/plan.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/hosted_page.py` & `chargebee-2.9.0/chargebee/models/hosted_page.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/subscription_estimate.py` & `chargebee-2.9.0/chargebee/models/subscription_estimate.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/address.py` & `chargebee-2.9.0/chargebee/models/address.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/invoice.py` & `chargebee-2.9.0/chargebee/models/invoice.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
       pass
 
     fields = ["id", "po_number", "customer_id", "subscription_id", "recurring", "status", "vat_number", \
     "price_type", "date", "due_date", "net_term_days", "exchange_rate", "currency_code", "total", \
     "amount_paid", "amount_adjusted", "write_off_amount", "credits_applied", "amount_due", "paid_at", \
     "dunning_status", "next_retry_at", "voided_at", "resource_version", "updated_at", "sub_total", \
     "sub_total_in_local_currency", "total_in_local_currency", "local_currency_code", "tax", "first_invoice", \
-    "new_sales_amount", "has_advance_charges", "term_finalized", "is_gifted", "expected_payment_date", \
+    "new_sales_amount", "has_advance_charges", "term_finalized", "is_gifted", "generated_at", "expected_payment_date", \
     "amount_to_collect", "round_off_amount", "line_items", "discounts", "line_item_discounts", "taxes", \
     "line_item_taxes", "line_item_tiers", "linked_payments", "dunning_attempts", "applied_credits", \
     "adjustment_credit_notes", "issued_credit_notes", "linked_orders", "notes", "shipping_address", \
     "billing_address", "payment_owner", "void_reason_code", "deleted", "vat_number_prefix"]
 
 
     @staticmethod
```

### Comparing `chargebee-2.8.4/chargebee/models/transaction.py` & `chargebee-2.9.0/chargebee/models/transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     fields = ["id", "customer_id", "subscription_id", "gateway_account_id", "payment_source_id", \
     "payment_method", "reference_number", "gateway", "type", "date", "settled_at", "exchange_rate", \
     "currency_code", "amount", "id_at_gateway", "status", "fraud_flag", "initiator_type", "three_d_secure", \
     "authorization_reason", "error_code", "error_text", "voided_at", "resource_version", "updated_at", \
     "fraud_reason", "amount_unused", "masked_card_number", "reference_transaction_id", "refunded_txn_id", \
     "reference_authorization_id", "amount_capturable", "reversal_transaction_id", "linked_invoices", \
-    "linked_credit_notes", "linked_refunds", "linked_payments", "deleted", "merchant_reference_id"]
+    "linked_credit_notes", "linked_refunds", "linked_payments", "deleted", "iin", "last4", "merchant_reference_id"]
 
 
     @staticmethod
     def create_authorization(params, env=None, headers=None):
         return request.send('post', request.uri_path("transactions","create_authorization"), params, env, headers)
 
     @staticmethod
```

### Comparing `chargebee-2.8.4/chargebee/models/attached_item.py` & `chargebee-2.9.0/chargebee/models/attached_item.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,11 +24,7 @@
     @staticmethod
     def delete(id, params, env=None, headers=None):
         return request.send('post', request.uri_path("attached_items",id,"delete"), params, env, headers)
 
     @staticmethod
     def list(id, params=None, env=None, headers=None):
         return request.send_list_request('get', request.uri_path("items",id,"attached_items"), params, env, headers)
-
-    @staticmethod
-    def list_internal(params=None, env=None, headers=None):
-        return request.send('get', request.uri_path("attached_items","list_internal"), params, env, headers)
```

### Comparing `chargebee-2.8.4/chargebee/models/credit_note_estimate.py` & `chargebee-2.9.0/chargebee/models/credit_note_estimate.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/credit_note.py` & `chargebee-2.9.0/chargebee/models/credit_note.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
       pass
     class Allocation(Model):
       fields = ["invoice_id", "allocated_amount", "allocated_at", "invoice_date", "invoice_status"]
       pass
 
     fields = ["id", "customer_id", "subscription_id", "reference_invoice_id", "type", "reason_code", \
     "status", "vat_number", "date", "price_type", "currency_code", "total", "amount_allocated", \
-    "amount_refunded", "amount_available", "refunded_at", "voided_at", "resource_version", "updated_at", \
-    "sub_total", "sub_total_in_local_currency", "total_in_local_currency", "local_currency_code", \
+    "amount_refunded", "amount_available", "refunded_at", "voided_at", "generated_at", "resource_version", \
+    "updated_at", "sub_total", "sub_total_in_local_currency", "total_in_local_currency", "local_currency_code", \
     "round_off_amount", "fractional_correction", "line_items", "discounts", "line_item_discounts", \
     "line_item_tiers", "taxes", "line_item_taxes", "linked_refunds", "allocations", "deleted", "create_reason_code", \
     "vat_number_prefix"]
 
 
     @staticmethod
     def create(params, env=None, headers=None):
```

### Comparing `chargebee-2.8.4/chargebee/models/export.py` & `chargebee-2.9.0/chargebee/models/export.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/payment_intent.py` & `chargebee-2.9.0/chargebee/models/payment_intent.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/order.py` & `chargebee-2.9.0/chargebee/models/order.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/estimate.py` & `chargebee-2.9.0/chargebee/models/estimate.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/unbilled_charge.py` & `chargebee-2.9.0/chargebee/models/unbilled_charge.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/addon.py` & `chargebee-2.9.0/chargebee/models/addon.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/coupon_set.py` & `chargebee-2.9.0/chargebee/models/coupon_set.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/item.py` & `chargebee-2.9.0/chargebee/models/item.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/portal_session.py` & `chargebee-2.9.0/chargebee/models/portal_session.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/quoted_subscription.py` & `chargebee-2.9.0/chargebee/models/quoted_subscription.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,28 +7,25 @@
     class Addon(Model):
       fields = ["id", "quantity", "unit_price", "amount", "trial_end", "remaining_billing_cycles", "quantity_in_decimal", "unit_price_in_decimal", "amount_in_decimal"]
       pass
     class EventBasedAddon(Model):
       fields = ["id", "quantity", "unit_price", "service_period_in_days", "on_event", "charge_once", "quantity_in_decimal", "unit_price_in_decimal"]
       pass
     class Coupon(Model):
-      fields = ["coupon_id", "apply_till", "applied_count", "coupon_code"]
-      pass
-    class Discount(Model):
-      fields = ["id", "invoice_name", "type", "percentage", "amount", "currency_code", "duration_type", "period", "period_unit", "included_in_mrr", "apply_on", "item_price_id", "created_at", "apply_till", "applied_count"]
+      fields = ["coupon_id"]
       pass
     class SubscriptionItem(Model):
       fields = ["item_price_id", "item_type", "quantity", "quantity_in_decimal", "metered_quantity", "last_calculated_at", "unit_price", "unit_price_in_decimal", "amount", "amount_in_decimal", "free_quantity", "free_quantity_in_decimal", "trial_end", "billing_cycles", "service_period_days", "charge_on_event", "charge_once", "charge_on_option"]
       pass
     class ItemTier(Model):
       fields = ["item_price_id", "starting_unit", "ending_unit", "price", "starting_unit_in_decimal", "ending_unit_in_decimal", "price_in_decimal"]
       pass
     class QuotedContractTerm(Model):
       fields = ["contract_start", "contract_end", "billing_cycle", "action_at_term_end", "total_contract_value", "cancellation_cutoff_period"]
       pass
 
     fields = ["id", "plan_id", "plan_quantity", "plan_unit_price", "setup_fee", "billing_period", \
     "billing_period_unit", "start_date", "trial_end", "remaining_billing_cycles", "po_number", "auto_collection", \
-    "plan_quantity_in_decimal", "plan_unit_price_in_decimal", "contract_term_billing_cycle_on_renewal", \
-    "addons", "event_based_addons", "coupons", "discounts", "subscription_items", "item_tiers", \
-    "quoted_contract_term"]
+    "plan_quantity_in_decimal", "plan_unit_price_in_decimal", "changes_scheduled_at", "change_option", \
+    "contract_term_billing_cycle_on_renewal", "addons", "event_based_addons", "coupons", "subscription_items", \
+    "item_tiers", "quoted_contract_term"]
```

### Comparing `chargebee-2.8.4/chargebee/models/subscription.py` & `chargebee-2.9.0/chargebee/models/subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     "contract_term_billing_cycle_on_renewal", "override_relationship", "pause_date", "resume_date", \
     "cancelled_at", "cancel_reason", "affiliate_token", "created_from_ip", "resource_version", "updated_at", \
     "has_scheduled_advance_invoices", "has_scheduled_changes", "payment_source_id", "plan_free_quantity_in_decimal", \
     "plan_amount_in_decimal", "cancel_schedule_created_at", "offline_payment_method", "channel", \
     "subscription_items", "item_tiers", "charged_items", "due_invoices_count", "due_since", "total_dues", \
     "mrr", "exchange_rate", "base_currency_code", "addons", "event_based_addons", "charged_event_based_addons", \
     "coupon", "coupons", "shipping_address", "referral_info", "invoice_notes", "meta_data", "metadata", \
-    "deleted", "contract_term", "cancel_reason_code", "free_period", "free_period_unit", "create_pending_invoices", \
-    "auto_close_invoices"]
+    "deleted", "changes_scheduled_at", "contract_term", "cancel_reason_code", "free_period", "free_period_unit", \
+    "create_pending_invoices", "auto_close_invoices"]
 
 
     @staticmethod
     def create(params, env=None, headers=None):
         return request.send('post', request.uri_path("subscriptions"), params, env, headers)
 
     @staticmethod
```

### Comparing `chargebee-2.8.4/chargebee/models/virtual_bank_account.py` & `chargebee-2.9.0/chargebee/models/virtual_bank_account.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/item_price.py` & `chargebee-2.9.0/chargebee/models/item_price.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/advance_invoice_schedule.py` & `chargebee-2.9.0/chargebee/models/advance_invoice_schedule.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/payment_source.py` & `chargebee-2.9.0/chargebee/models/payment_source.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/item_family.py` & `chargebee-2.9.0/chargebee/models/item_family.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/gift.py` & `chargebee-2.9.0/chargebee/models/gift.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/shipping_address.py` & `chargebee-2.9.0/chargebee/models/shipping_address.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/quote.py` & `chargebee-2.9.0/chargebee/models/quote.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/models/differential_price.py` & `chargebee-2.9.0/chargebee/models/differential_price.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/model.py` & `chargebee-2.9.0/chargebee/model.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/chargebee/util.py` & `chargebee-2.9.0/chargebee/util.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/setup.py` & `chargebee-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `chargebee-2.8.4/README.md` & `chargebee-2.9.0/README.md`

 * *Files identical despite different names*

