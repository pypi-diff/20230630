# Comparing `tmp/django-vendor-promo-0.2.7.tar.gz` & `tmp/django-vendor-promo-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-vendor-promo-0.2.7.tar", last modified: Tue Jun  6 17:05:10 2023, max compression
+gzip compressed data, was "django-vendor-promo-0.2.8.tar", last modified: Fri Jun 30 16:32:32 2023, max compression
```

## Comparing `django-vendor-promo-0.2.7.tar` & `django-vendor-promo-0.2.8.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:05:10.012522 django-vendor-promo-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/LICENSE.mit.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-06 17:05:10.012522 django-vendor-promo-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 17:05:10.012522 django-vendor-promo-0.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:05:10.004521 django-vendor-promo-0.2.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:05:10.004521 django-vendor-promo-0.2.7/src/django_vendor_promo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-06 17:05:09.000000 django-vendor-promo-0.2.7/src/django_vendor_promo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-06 17:05:10.000000 django-vendor-promo-0.2.7/src/django_vendor_promo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:05:09.000000 django-vendor-promo-0.2.7/src/django_vendor_promo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-06 17:05:09.000000 django-vendor-promo-0.2.7/src/django_vendor_promo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-06 17:05:09.000000 django-vendor-promo-0.2.7/src/django_vendor_promo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:05:10.008522 django-vendor-promo-0.2.7/src/vendorpromo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:05:10.008522 django-vendor-promo-0.2.7/src/vendorpromo/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:05:10.008522 django-vendor-promo-0.2.7/src/vendorpromo/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/api/v1/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:05:10.008522 django-vendor-promo-0.2.7/src/vendorpromo/api/v1/vouchery/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/api/v1/vouchery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/api/v1/vouchery/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/api/v1/vouchery/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/integrations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:05:10.008522 django-vendor-promo-0.2.7/src/vendorpromo/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/migrations/0002_affiliate_couponcode_promotionalcampaign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/migrations/0003_auto_20230524_1701.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/migrations/0004_affiliate_name_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/migrations/0005_alter_couponcode_code.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:05:10.008522 django-vendor-promo-0.2.7/src/vendorpromo/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/processors/DummyProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/processors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/processors/stripe.py
--rw-r--r--   0 runner    (1001) docker     (123)    17456 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/processors/vouchery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:05:10.004521 django-vendor-promo-0.2.7/src/vendorpromo/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:05:10.012522 django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/affiliate_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/affiliate_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/coupon_code_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/coupon_code_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:05:10.012522 django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/includes/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/includes/promocode_apply.html
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/processor_site_config.html
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/processor_site_config_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/promo.html
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/promo_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/promocode_formset.html
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/promotional_campaign_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/promotional_campaign_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/vouchery_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/vouchery_integration.html
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/vouchery_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:05:10.012522 django-vendor-promo-0.2.7/src/vendorpromo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7234 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/tests/test_affiliate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/tests/test_coupon_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    21273 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/tests/test_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/tests/test_promo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/tests/test_promotional_campaign.py
--rw-r--r--   0 runner    (1001) docker     (123)    20938 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/tests/test_stripe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15017 2023-06-06 17:03:58.000000 django-vendor-promo-0.2.7/src/vendorpromo/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:32:32.985111 django-vendor-promo-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/LICENSE.mit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-30 16:32:32.985111 django-vendor-promo-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 16:32:32.989111 django-vendor-promo-0.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:32:32.969111 django-vendor-promo-0.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:32:32.973111 django-vendor-promo-0.2.8/src/django_vendor_promo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-30 16:32:32.000000 django-vendor-promo-0.2.8/src/django_vendor_promo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-30 16:32:32.000000 django-vendor-promo-0.2.8/src/django_vendor_promo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:32:32.000000 django-vendor-promo-0.2.8/src/django_vendor_promo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-30 16:32:32.000000 django-vendor-promo-0.2.8/src/django_vendor_promo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-30 16:32:32.000000 django-vendor-promo-0.2.8/src/django_vendor_promo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:32:32.977111 django-vendor-promo-0.2.8/src/vendorpromo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:32:32.977111 django-vendor-promo-0.2.8/src/vendorpromo/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:32:32.977111 django-vendor-promo-0.2.8/src/vendorpromo/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/api/v1/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:32:32.977111 django-vendor-promo-0.2.8/src/vendorpromo/api/v1/vouchery/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/api/v1/vouchery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/api/v1/vouchery/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/api/v1/vouchery/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/integrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:32:32.985111 django-vendor-promo-0.2.8/src/vendorpromo/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/migrations/0002_affiliate_couponcode_promotionalcampaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/migrations/0003_auto_20230524_1701.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/migrations/0004_affiliate_name_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/migrations/0005_alter_couponcode_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:32:32.985111 django-vendor-promo-0.2.8/src/vendorpromo/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/processors/DummyProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/processors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/processors/stripe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17454 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/processors/vouchery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:32:32.969111 django-vendor-promo-0.2.8/src/vendorpromo/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:32:32.985111 django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/affiliate_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/affiliate_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/coupon_code_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/coupon_code_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:32:32.985111 django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/includes/promocode_apply.html
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/processor_site_config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/processor_site_config_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/promo.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/promo_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/promocode_formset.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/promotional_campaign_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/promotional_campaign_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/vouchery_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/vouchery_integration.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/vouchery_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:32:32.985111 django-vendor-promo-0.2.8/src/vendorpromo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7234 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/tests/test_affiliate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/tests/test_coupon_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21273 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/tests/test_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/tests/test_promo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/tests/test_promotional_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20938 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/tests/test_stripe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15017 2023-06-30 16:31:36.000000 django-vendor-promo-0.2.8/src/vendorpromo/views.py
```

### Comparing `django-vendor-promo-0.2.7/PKG-INFO` & `django-vendor-promo-0.2.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vendor-promo
-Version: 0.2.7
+Version: 0.2.8
 Summary: Extension to Django Vendor to add Promo Code capabilities
 Author: Roberto Himmelbauer
 Author-email: Grant Viklund <renderbox@gmail.com>
 Project-URL: Homepage, https://github.com/renderbox/django-vendor-promo/
 Project-URL: Bug Tracker, https://github.com/renderbox/django-vendor-promo/issues
 Keywords: django,app
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `django-vendor-promo-0.2.7/pyproject.toml` & `django-vendor-promo-0.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 [project]
 name = "django-vendor-promo"
-version = "0.2.7"
+version = "0.2.8"
 
 authors = [
   { name="Grant Viklund", email="renderbox@gmail.com" },
   { name="Roberto Himmelbauer" }
 ]
 description = "Extension to Django Vendor to add Promo Code capabilities"
 readme = "README.md"
```

### Comparing `django-vendor-promo-0.2.7/src/django_vendor_promo.egg-info/PKG-INFO` & `django-vendor-promo-0.2.8/src/django_vendor_promo.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vendor-promo
-Version: 0.2.7
+Version: 0.2.8
 Summary: Extension to Django Vendor to add Promo Code capabilities
 Author: Roberto Himmelbauer
 Author-email: Grant Viklund <renderbox@gmail.com>
 Project-URL: Homepage, https://github.com/renderbox/django-vendor-promo/
 Project-URL: Bug Tracker, https://github.com/renderbox/django-vendor-promo/issues
 Keywords: django,app
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `django-vendor-promo-0.2.7/src/django_vendor_promo.egg-info/SOURCES.txt` & `django-vendor-promo-0.2.8/src/django_vendor_promo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/admin.py` & `django-vendor-promo-0.2.8/src/vendorpromo/admin.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/api/v1/urls.py` & `django-vendor-promo-0.2.8/src/vendorpromo/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/api/v1/views.py` & `django-vendor-promo-0.2.8/src/vendorpromo/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/api/v1/vouchery/views.py` & `django-vendor-promo-0.2.8/src/vendorpromo/api/v1/vouchery/views.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/config.py` & `django-vendor-promo-0.2.8/src/vendorpromo/config.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/forms.py` & `django-vendor-promo-0.2.8/src/vendorpromo/forms.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/integrations.py` & `django-vendor-promo-0.2.8/src/vendorpromo/integrations.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/migrations/0001_initial.py` & `django-vendor-promo-0.2.8/src/vendorpromo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/migrations/0002_affiliate_couponcode_promotionalcampaign.py` & `django-vendor-promo-0.2.8/src/vendorpromo/migrations/0002_affiliate_couponcode_promotionalcampaign.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/migrations/0003_auto_20230524_1701.py` & `django-vendor-promo-0.2.8/src/vendorpromo/migrations/0003_auto_20230524_1701.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/migrations/0004_affiliate_name_type.py` & `django-vendor-promo-0.2.8/src/vendorpromo/migrations/0004_affiliate_name_type.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/models.py` & `django-vendor-promo-0.2.8/src/vendorpromo/models.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/processors/base.py` & `django-vendor-promo-0.2.8/src/vendorpromo/processors/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -137,14 +137,18 @@
     def update_coupon_code(self, coupon_form):
         coupon_code = coupon_form.save(commit=True)
         return coupon_code
 
     def delete_coupon_code(self, coupon_code):
         coupon_code.delete()
 
+    def set_active_coupon_code(self, coupon_code, is_active):
+        coupon_code.active = is_active
+        coupon_code.save()
+
     ################
     # Processor Functions
     def is_code_valid(self, code):
         """
         Overwrite funtion to call external promo services.
         Eg. call Vouchary.io API to see if the code entered is valid.
         """
```

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/processors/stripe.py` & `django-vendor-promo-0.2.8/src/vendorpromo/processors/stripe.py`

 * *Files 11% similar despite different names*

```diff
@@ -83,14 +83,28 @@
         del(promotion_code_data['max_redemptions'])
 
         stripe_coupon = self.stripe_builder.stripe_update_object(self.stripe_builder.stripe.PromotionCode, coupon_code.meta['stripe_id'], promotion_code_data)
 
         if not stripe_coupon:
             return None  # Think about returning an error
 
+    def set_active_stripe_promotion_code(self, coupon_code, is_active):
+        promotion_code_data = self.build_promotion_code(coupon_code)
+        promotion_code_data['active'] = is_active
+        del(promotion_code_data['coupon'])
+        del(promotion_code_data['code'])
+        del(promotion_code_data['metadata'])
+        del(promotion_code_data['expires_at'])
+        del(promotion_code_data['max_redemptions'])
+
+        stripe_coupon = self.stripe_builder.stripe_update_object(self.stripe_builder.stripe.PromotionCode, coupon_code.meta['stripe_id'], promotion_code_data)
+
+        if not stripe_coupon:
+            return None  # Think about returning an error
+
     ################
     # Promotion Management
     def create_promo(self, promo_form):
         '''
         Override if you need to do additional steps when creating a Promo instance,
         such as creating the promo code in an external service if needed.
         '''
@@ -131,14 +145,20 @@
 
     def update_coupon_code(self, coupon_form):
         coupon_code = super().update_coupon_code(coupon_form)
         self.update_stripe_promotion_code(coupon_code)
 
         return coupon_code
 
+    def set_active_coupon_code(self, coupon_code, is_active):
+        super().set_active_coupon_code(coupon_code, is_active)
+        self.set_active_stripe_promotion_code(coupon_code, is_active)
+
+        return coupon_code
+
     ################
     # Processor Functions
     def is_code_valid(self, coupon_code):
         if 'stripe_id' not in coupon_code.meta:
             return False
         
         return True
```

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/processors/vouchery.py` & `django-vendor-promo-0.2.8/src/vendorpromo/processors/vouchery.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         "type": "SetDiscount",
         "discount_type": "percentage",
         "discount_value": 0  # The actual discount is set in the Offer instance.
     }
     credentials = None
 
     def __init__(self, site, invoice=None):
-        super().__init__(invoice=invoice)
+        super().__init__(site, invoice)
         self.set_credentials(site)
 
 
     def set_credentials(self, site):
         self.credentials = VoucheryIntegration(site)
         if self.credentials.instance:
            self.BASE_URL = self.credentials.instance.client_url
```

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/affiliate_detail.html` & `django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/affiliate_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/affiliate_list.html` & `django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/affiliate_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/coupon_code_detail.html` & `django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/coupon_code_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/coupon_code_list.html` & `django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/coupon_code_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/includes/promocode_apply.html` & `django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/includes/promocode_apply.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/processor_site_config_list.html` & `django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/processor_site_config_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/promo.html` & `django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/promo.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/promo_list.html` & `django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/promo_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/promocode_formset.html` & `django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/promocode_formset.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/promotional_campaign_detail.html` & `django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/promotional_campaign_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/promotional_campaign_list.html` & `django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/promotional_campaign_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/vouchery_detail.html` & `django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/vouchery_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/vouchery_integration.html` & `django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/vouchery_integration.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/templates/vendorpromo/vouchery_list.html` & `django-vendor-promo-0.2.8/src/vendorpromo/templates/vendorpromo/vouchery_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/tests/test_affiliate.py` & `django-vendor-promo-0.2.8/src/vendorpromo/tests/test_affiliate.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/tests/test_api.py` & `django-vendor-promo-0.2.8/src/vendorpromo/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/tests/test_coupon_code.py` & `django-vendor-promo-0.2.8/src/vendorpromo/tests/test_coupon_code.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/tests/test_processor.py` & `django-vendor-promo-0.2.8/src/vendorpromo/tests/test_processor.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/tests/test_promo.py` & `django-vendor-promo-0.2.8/src/vendorpromo/tests/test_promo.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/tests/test_promotional_campaign.py` & `django-vendor-promo-0.2.8/src/vendorpromo/tests/test_promotional_campaign.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/tests/test_stripe.py` & `django-vendor-promo-0.2.8/src/vendorpromo/tests/test_stripe.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/urls.py` & `django-vendor-promo-0.2.8/src/vendorpromo/urls.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.2.7/src/vendorpromo/views.py` & `django-vendor-promo-0.2.8/src/vendorpromo/views.py`

 * *Files identical despite different names*

