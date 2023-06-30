# Comparing `tmp/django_subscriptions_rt-0.0.1-py3-none-any.whl.zip` & `tmp/django_subscriptions_rt-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,39 +1,111 @@
-Zip file size: 29668 bytes, number of entries: 37
--rw-r--r--  2.0 unx        0 b- defN 22-Mar-18 08:11 subscriptions/__init__.py
--rw-r--r--  2.0 unx     2439 b- defN 22-Mar-21 17:25 subscriptions/admin.py
--rw-r--r--  2.0 unx      240 b- defN 22-Mar-21 12:11 subscriptions/exceptions.py
--rw-r--r--  2.0 unx      988 b- defN 22-Mar-15 20:09 subscriptions/fields.py
--rw-r--r--  2.0 unx     4907 b- defN 22-Mar-23 19:41 subscriptions/functions.py
--rw-r--r--  2.0 unx      503 b- defN 22-Mar-23 19:41 subscriptions/middleware.py
--rw-r--r--  2.0 unx    11585 b- defN 22-Mar-21 17:22 subscriptions/models.py
--rw-r--r--  2.0 unx      419 b- defN 22-Mar-21 17:20 subscriptions/urls.py
--rw-r--r--  2.0 unx      986 b- defN 22-Mar-09 09:25 subscriptions/utils.py
--rw-r--r--  2.0 unx     2131 b- defN 22-Mar-23 19:41 subscriptions/views.py
--rw-r--r--  2.0 unx        0 b- defN 22-Mar-23 19:55 subscriptions/api/__init__.py
--rw-r--r--  2.0 unx      365 b- defN 22-Mar-15 13:28 subscriptions/api/fields.py
--rw-r--r--  2.0 unx     1112 b- defN 22-Mar-21 17:30 subscriptions/api/serializers.py
--rw-r--r--  2.0 unx      645 b- defN 22-Mar-23 19:41 subscriptions/api/urls.py
--rw-r--r--  2.0 unx     2135 b- defN 22-Mar-21 17:30 subscriptions/api/views.py
--rw-r--r--  2.0 unx    14454 b- defN 22-Mar-23 19:42 subscriptions/migrations/0001_initial.py
--rw-r--r--  2.0 unx      387 b- defN 22-Mar-23 19:42 subscriptions/migrations/0002_alter_subscription_begin.py
--rw-r--r--  2.0 unx      668 b- defN 22-Mar-23 19:42 subscriptions/migrations/0003_alter_plan_charge_amount_alter_usage_datetime.py
--rw-r--r--  2.0 unx      400 b- defN 22-Mar-23 19:42 subscriptions/migrations/0004_rename_begin_subscription_start.py
--rw-r--r--  2.0 unx      433 b- defN 22-Mar-23 19:42 subscriptions/migrations/0005_plan_slug.py
--rw-r--r--  2.0 unx     1245 b- defN 22-Mar-23 19:42 subscriptions/migrations/0006_alter_plan_charge_period_and_more.py
--rw-r--r--  2.0 unx    33494 b- defN 22-Mar-23 19:42 subscriptions/migrations/0007_subscriptionpayment_and_more.py
--rw-r--r--  2.0 unx      935 b- defN 22-Mar-23 19:42 subscriptions/migrations/0008_rename_vendor_subscriptionpayment_provider_name_and_more.py
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-09 11:49 subscriptions/migrations/__init__.py
--rw-r--r--  2.0 unx     1668 b- defN 22-Mar-21 17:11 subscriptions/providers/__init__.py
--rw-r--r--  2.0 unx     1133 b- defN 22-Mar-21 17:16 subscriptions/providers/dummy/__init__.py
--rw-r--r--  2.0 unx      119 b- defN 22-Mar-18 12:06 subscriptions/providers/dummy/forms.py
+Zip file size: 163771 bytes, number of entries: 109
+-rw-rw----  2.0 unx        0 b- defN 23-Jun-06 14:40 subscriptions/__init__.py
+-rw-rw----  2.0 unx     4175 b- defN 23-Jun-06 14:40 subscriptions/admin.py
+-rw-rw----  2.0 unx      895 b- defN 23-Jun-24 12:42 subscriptions/defaults.py
+-rw-rw----  2.0 unx      471 b- defN 23-Jun-06 14:40 subscriptions/exceptions.py
+-rw-rw----  2.0 unx      988 b- defN 23-Jun-06 14:40 subscriptions/fields.py
+-rw-rw----  2.0 unx    11808 b- defN 23-Jun-24 12:42 subscriptions/functions.py
+-rw-rw----  2.0 unx      376 b- defN 22-Dec-15 09:06 subscriptions/logging.py
+-rw-rw----  2.0 unx      402 b- defN 23-Jun-20 11:30 subscriptions/metrics.py
+-rw-rw----  2.0 unx      477 b- defN 23-Jun-06 14:40 subscriptions/middleware.py
+-rw-rw----  2.0 unx    20912 b- defN 23-Jun-24 12:42 subscriptions/models.py
+-rw-rw----  2.0 unx     9701 b- defN 23-Jun-24 12:42 subscriptions/reports.py
+-rw-rw----  2.0 unx     2824 b- defN 23-Jun-06 14:40 subscriptions/signals.py
+-rw-rw----  2.0 unx     7540 b- defN 23-Jun-30 15:28 subscriptions/tasks.py
+-rw-rw----  2.0 unx      457 b- defN 23-Jun-06 14:40 subscriptions/urls.py
+-rw-rw----  2.0 unx     1433 b- defN 23-Jun-24 12:42 subscriptions/utils.py
+-rw-rw----  2.0 unx     1718 b- defN 23-Jun-06 14:40 subscriptions/validators.py
+-rw-rw----  2.0 unx     1719 b- defN 23-Jun-06 14:40 subscriptions/views.py
+-rw-rw----  2.0 unx      168 b- defN 23-Jun-07 09:52 subscriptions/__pycache__/__init__.cpython-310.pyc
+-rw-rw----  2.0 unx      166 b- defN 23-Jun-07 09:26 subscriptions/__pycache__/__init__.cpython-39.pyc
+-rw-rw----  2.0 unx     4606 b- defN 23-Jun-07 09:26 subscriptions/__pycache__/admin.cpython-39.pyc
+-rw-rw----  2.0 unx      864 b- defN 23-May-27 13:00 subscriptions/__pycache__/defaults.cpython-39.pyc
+-rw-rw----  2.0 unx     1380 b- defN 23-Jun-07 09:26 subscriptions/__pycache__/exceptions.cpython-39.pyc
+-rw-rw----  2.0 unx     1920 b- defN 23-Jun-07 09:52 subscriptions/__pycache__/fields.cpython-310.pyc
+-rw-rw----  2.0 unx     1911 b- defN 23-Jun-07 09:26 subscriptions/__pycache__/fields.cpython-39.pyc
+-rw-rw----  2.0 unx    11126 b- defN 23-Jun-30 15:10 subscriptions/__pycache__/functions.cpython-39.pyc
+-rw-r--r--  2.0 unx     3391 b- defN 22-Feb-28 10:06 subscriptions/__pycache__/helpers.cpython-39.pyc
+-rw-rw----  2.0 unx      832 b- defN 23-Jun-07 09:34 subscriptions/__pycache__/middleware.cpython-39.pyc
+-rw-rw----  2.0 unx    20655 b- defN 23-Jun-07 09:52 subscriptions/__pycache__/models.cpython-310.pyc
+-rw-rw----  2.0 unx    20708 b- defN 23-Jun-30 15:10 subscriptions/__pycache__/models.cpython-39.pyc
+-rw-rw----  2.0 unx     1870 b- defN 23-Jun-07 09:26 subscriptions/__pycache__/signals.cpython-39.pyc
+-rw-rw----  2.0 unx      561 b- defN 23-Jun-07 09:34 subscriptions/__pycache__/urls.cpython-39.pyc
+-rw-rw----  2.0 unx     1705 b- defN 23-Jun-30 15:10 subscriptions/__pycache__/utils.cpython-39.pyc
+-rw-rw----  2.0 unx     2457 b- defN 23-Jun-07 09:34 subscriptions/__pycache__/views.cpython-39.pyc
+-rw-rw----  2.0 unx      365 b- defN 23-Jun-06 14:40 subscriptions/api/fields.py
+-rw-rw----  2.0 unx     3184 b- defN 23-Jun-24 12:42 subscriptions/api/serializers.py
+-rw-rw----  2.0 unx     1164 b- defN 23-Jun-24 12:42 subscriptions/api/urls.py
+-rw-rw----  2.0 unx     8367 b- defN 23-Jun-24 12:42 subscriptions/api/views.py
+-rw-r--r--  2.0 unx      758 b- defN 22-Mar-15 13:28 subscriptions/api/__pycache__/fields.cpython-39.pyc
+-rw-rw----  2.0 unx     4870 b- defN 23-Jun-30 15:10 subscriptions/api/__pycache__/serializers.cpython-39.pyc
+-rw-rw----  2.0 unx     1062 b- defN 23-Jun-30 15:10 subscriptions/api/__pycache__/urls.cpython-39.pyc
+-rw-rw----  2.0 unx     8925 b- defN 23-Jun-30 15:10 subscriptions/api/__pycache__/views.cpython-39.pyc
+-rw-rw----  2.0 unx      379 b- defN 23-Jun-06 14:40 subscriptions/management/commands/check_unfinished_payments.py
+-rw-rw----  2.0 unx    47602 b- defN 23-Jun-06 14:40 subscriptions/migrations/0001_initial.py
+-rw-rw----  2.0 unx     1520 b- defN 23-Jun-06 14:40 subscriptions/migrations/0002_subscriptionpayment_metadata_and_more.py
+-rw-rw----  2.0 unx      766 b- defN 23-Jun-06 14:40 subscriptions/migrations/0003_remove_subscriptionpayment_subscription_charge_date_and_more.py
+-rw-rw----  2.0 unx      488 b- defN 23-Jun-06 14:40 subscriptions/migrations/0004_remove_plan_unique_plan_slug_remove_plan_slug.py
+-rw-rw----  2.0 unx     1212 b- defN 23-Jun-06 14:40 subscriptions/migrations/0005_alter_subscriptionpayment_metadata_and_more.py
+-rw-rw----  2.0 unx      430 b- defN 23-Jun-06 14:40 subscriptions/migrations/0006_subscription_quantity.py
+-rw-rw----  2.0 unx      662 b- defN 23-Jun-06 14:40 subscriptions/migrations/0007_alter_subscriptionpayment_provider_transaction_id_and_more.py
+-rw-rw----  2.0 unx      452 b- defN 23-Jun-06 14:40 subscriptions/migrations/0008_subscriptionpayment_quantity.py
+-rw-rw----  2.0 unx    42010 b- defN 23-Jun-06 14:40 subscriptions/migrations/0009_auto_20220711_2159.py
+-rw-rw----  2.0 unx      404 b- defN 23-Jun-06 14:40 subscriptions/migrations/0010_subscription_auto_prolong_and_more.py
+-rw-rw----  2.0 unx    42039 b- defN 23-Jun-06 14:40 subscriptions/migrations/0011_alter_plan_charge_amount_currency_alter_plan_id_and_more.py
+-rw-rw----  2.0 unx     1213 b- defN 23-Jun-06 14:40 subscriptions/migrations/0012_subscription_uid_subscriptionpayment_uid_and_more.py
+-rw-rw----  2.0 unx      824 b- defN 23-Jun-06 14:40 subscriptions/migrations/0013_alter_subscription_uid_alter_subscriptionpayment_uid_and_more.py
+-rw-rw----  2.0 unx     1162 b- defN 23-Jun-06 14:40 subscriptions/migrations/0014_subscriptionpayment_subscription_uid_and_more.py
+-rw-rw----  2.0 unx      996 b- defN 23-Jun-06 14:40 subscriptions/migrations/0015_auto_20220728_1920.py
+-rw-rw----  2.0 unx      599 b- defN 23-Jun-06 14:40 subscriptions/migrations/0016_remove_subscriptionpayment_subscription_and_more.py
+-rw-rw----  2.0 unx     1218 b- defN 23-Jun-06 14:40 subscriptions/migrations/0017_alter_subscriptionpayment_subscription_uid_and_more.py
+-rw-rw----  2.0 unx     2128 b- defN 23-Jun-06 14:40 subscriptions/migrations/0018_remove_subscription_id_remove_subscriptionpayment_id_and_more.py
+-rw-rw----  2.0 unx      789 b- defN 23-Jun-06 14:40 subscriptions/migrations/0019_rename_subscription_uid_subscriptionpayment_subscription_and_more.py
+-rw-rw----  2.0 unx      849 b- defN 23-Jun-06 14:40 subscriptions/migrations/0020_alter_subscriptionpaymentrefund_original_payment_and_more.py
+-rw-rw----  2.0 unx     1058 b- defN 23-Jun-06 14:40 subscriptions/migrations/0021_alter_subscriptionpayment_subscription_and_more.py
+-rw-rw----  2.0 unx     1491 b- defN 23-Jun-06 14:40 subscriptions/migrations/0022_alter_subscriptionpayment_subscription_and_more.py
+-rw-rw----  2.0 unx      936 b- defN 23-Jun-06 14:40 subscriptions/migrations/0023_alter_subscription_options_and_more.py
+-rw-rw----  2.0 unx      777 b- defN 23-Jun-06 14:40 subscriptions/migrations/0024_alter_subscriptionpayment_amount_and_more.py
+-rw-rw----  2.0 unx     1552 b- defN 23-Jun-06 14:40 subscriptions/migrations/0025_feature_tier_plan_tier.py
+-rw-rw----  2.0 unx      789 b- defN 23-Jun-06 14:40 subscriptions/migrations/0026_alter_subscriptionpayment_status_and_more.py
+-rw-rw----  2.0 unx     3572 b- defN 23-Jun-06 14:40 subscriptions/migrations/0027_auto_20221109_1525.py
+-rw-rw----  2.0 unx      391 b- defN 23-Jun-06 14:40 subscriptions/migrations/0028_tier_level.py
+-rw-rw----  2.0 unx    65854 b- defN 23-Jun-06 14:40 subscriptions/migrations/0029_alter_plan_charge_amount_currency_and_more.py
+-rw-rw----  2.0 unx      423 b- defN 23-Jun-06 14:40 subscriptions/migrations/0030_feature_is_negative.py
+-rw-rw----  2.0 unx      578 b- defN 23-Jun-06 14:40 subscriptions/migrations/0031_alter_plan_tier.py
+-rw-rw----  2.0 unx     4039 b- defN 23-Mar-23 11:19 subscriptions/migrations/0032_alter_subscriptionpayment_options_and_more.py
+-rw-rw----  2.0 unx     1223 b- defN 23-Apr-17 13:22 subscriptions/migrations/0032_auto_20230417_1312.py
+-rw-rw----  2.0 unx    49637 b- defN 23-Jun-24 12:42 subscriptions/migrations/0032_subscription_initial_charge_offset_and_more.py
+-rw-rw----  2.0 unx        0 b- defN 23-Jun-06 14:40 subscriptions/migrations/__init__.py
+-rw-rw----  2.0 unx     3076 b- defN 23-Jun-24 12:42 subscriptions/providers/__init__.py
+-rw-rw----  2.0 unx     3784 b- defN 23-Jun-30 15:10 subscriptions/providers/__pycache__/__init__.cpython-39.pyc
+-rw-rw----  2.0 unx    16960 b- defN 23-Jun-24 12:42 subscriptions/providers/apple_in_app/__init__.py
+-rw-rw----  2.0 unx     6144 b- defN 23-Jun-06 14:40 subscriptions/providers/apple_in_app/api.py
+-rw-rw----  2.0 unx    10521 b- defN 23-Jun-06 14:40 subscriptions/providers/apple_in_app/app_store.py
+-rw-rw----  2.0 unx      685 b- defN 23-Jun-06 14:40 subscriptions/providers/apple_in_app/enums.py
+-rw-rw----  2.0 unx      959 b- defN 23-Jun-06 14:40 subscriptions/providers/apple_in_app/exceptions.py
+-rw-rw----  2.0 unx      583 b- defN 23-Jun-06 14:40 subscriptions/providers/apple_in_app/certs/AppleRootCA-G3.cer
+-rw-rw----  2.0 unx     1215 b- defN 22-Oct-26 12:16 subscriptions/providers/apple_in_app/certs/AppleRootCertificate.cer
+-rw-rw----  2.0 unx     5288 b- defN 23-Jun-24 12:42 subscriptions/providers/dummy/__init__.py
+-rw-rw----  2.0 unx      119 b- defN 23-Jun-06 14:40 subscriptions/providers/dummy/forms.py
+-rw-r--r--  2.0 unx      198 b- defN 22-May-31 13:16 subscriptions/providers/dummy/serializers.py
+-rw-rw----  2.0 unx     3221 b- defN 23-Jun-30 15:10 subscriptions/providers/dummy/__pycache__/__init__.cpython-39.pyc
+-rw-rw----  2.0 unx      446 b- defN 23-Jun-07 09:34 subscriptions/providers/dummy/__pycache__/forms.cpython-39.pyc
+-rw-r--r--  2.0 unx      724 b- defN 22-Mar-10 11:50 subscriptions/providers/dummy/__pycache__/models.cpython-39.pyc
+-rw-rw----  2.0 unx    24879 b- defN 23-Jun-30 15:23 subscriptions/providers/google_in_app/__init__.py
+-rw-rw----  2.0 unx      107 b- defN 23-Jun-06 14:40 subscriptions/providers/google_in_app/exceptions.py
+-rw-rw----  2.0 unx     7645 b- defN 23-Jun-14 10:42 subscriptions/providers/google_in_app/models.py
+-rw-rw----  2.0 unx       52 b- defN 23-Jun-13 22:12 subscriptions/providers/google_in_app/tasks.py
+-rw-rw----  2.0 unx     9610 b- defN 23-Jun-24 12:42 subscriptions/providers/paddle/__init__.py
+-rw-rw----  2.0 unx     6697 b- defN 23-Jun-08 13:32 subscriptions/providers/paddle/api.py
+-rw-rw----  2.0 unx      714 b- defN 23-Jun-06 14:40 subscriptions/providers/paddle/models.py
 -rw-r--r--  2.0 unx       67 b- defN 22-Mar-18 09:11 subscriptions/providers/stripe/__init__.py
 -rw-r--r--  2.0 unx      386 b- defN 22-Mar-10 11:45 subscriptions/providers/stripe/models.py
--rw-r--r--  2.0 unx      203 b- defN 22-Mar-18 12:40 subscriptions/templates/subscriptions/pay.html
--rw-r--r--  2.0 unx      142 b- defN 22-Mar-21 15:38 subscriptions/templates/subscriptions/payment-success.html
--rw-r--r--  2.0 unx       74 b- defN 22-Mar-23 19:52 subscriptions/templates/subscriptions/plan.html
--rw-r--r--  2.0 unx      171 b- defN 22-Mar-18 08:42 subscriptions/templates/subscriptions/plans.html
--rw-r--r--  2.0 unx     1248 b- defN 22-Mar-24 09:24 django_subscriptions_rt-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Mar-24 09:24 django_subscriptions_rt-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 22-Mar-24 09:24 django_subscriptions_rt-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3521 b- defN 22-Mar-24 09:24 django_subscriptions_rt-0.0.1.dist-info/RECORD
-37 files, 89309 bytes uncompressed, 23840 bytes compressed:  73.3%
+-rw-rw----  2.0 unx       74 b- defN 23-Jun-06 14:40 subscriptions/templates/subscriptions/plan.html
+-rw-rw----  2.0 unx      171 b- defN 23-Jun-06 14:40 subscriptions/templates/subscriptions/plans.html
+-rw-rw----  2.0 unx      142 b- defN 23-Jun-06 14:40 subscriptions/templates/subscriptions/subscribe-success.html
+-rw-rw----  2.0 unx      203 b- defN 23-Jun-06 14:40 subscriptions/templates/subscriptions/subscribe.html
+-rw-rw----  2.0 unx    16294 b- defN 23-Jun-30 17:03 django_subscriptions_rt-1.0.2.dist-info/METADATA
+-rw-rw----  2.0 unx       92 b- defN 23-Jun-30 17:03 django_subscriptions_rt-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-30 17:03 django_subscriptions_rt-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    11690 b- defN 23-Jun-30 17:03 django_subscriptions_rt-1.0.2.dist-info/RECORD
+109 files, 581733 bytes uncompressed, 144309 bytes compressed:  75.2%
```

## zipnote {}

```diff
@@ -1,112 +1,328 @@
 Filename: subscriptions/__init__.py
 Comment: 
 
 Filename: subscriptions/admin.py
 Comment: 
 
+Filename: subscriptions/defaults.py
+Comment: 
+
 Filename: subscriptions/exceptions.py
 Comment: 
 
 Filename: subscriptions/fields.py
 Comment: 
 
 Filename: subscriptions/functions.py
 Comment: 
 
+Filename: subscriptions/logging.py
+Comment: 
+
+Filename: subscriptions/metrics.py
+Comment: 
+
 Filename: subscriptions/middleware.py
 Comment: 
 
 Filename: subscriptions/models.py
 Comment: 
 
+Filename: subscriptions/reports.py
+Comment: 
+
+Filename: subscriptions/signals.py
+Comment: 
+
+Filename: subscriptions/tasks.py
+Comment: 
+
 Filename: subscriptions/urls.py
 Comment: 
 
 Filename: subscriptions/utils.py
 Comment: 
 
+Filename: subscriptions/validators.py
+Comment: 
+
 Filename: subscriptions/views.py
 Comment: 
 
-Filename: subscriptions/api/__init__.py
+Filename: subscriptions/__pycache__/__init__.cpython-310.pyc
+Comment: 
+
+Filename: subscriptions/__pycache__/__init__.cpython-39.pyc
+Comment: 
+
+Filename: subscriptions/__pycache__/admin.cpython-39.pyc
+Comment: 
+
+Filename: subscriptions/__pycache__/defaults.cpython-39.pyc
+Comment: 
+
+Filename: subscriptions/__pycache__/exceptions.cpython-39.pyc
+Comment: 
+
+Filename: subscriptions/__pycache__/fields.cpython-310.pyc
+Comment: 
+
+Filename: subscriptions/__pycache__/fields.cpython-39.pyc
+Comment: 
+
+Filename: subscriptions/__pycache__/functions.cpython-39.pyc
+Comment: 
+
+Filename: subscriptions/__pycache__/helpers.cpython-39.pyc
+Comment: 
+
+Filename: subscriptions/__pycache__/middleware.cpython-39.pyc
+Comment: 
+
+Filename: subscriptions/__pycache__/models.cpython-310.pyc
+Comment: 
+
+Filename: subscriptions/__pycache__/models.cpython-39.pyc
+Comment: 
+
+Filename: subscriptions/__pycache__/signals.cpython-39.pyc
+Comment: 
+
+Filename: subscriptions/__pycache__/urls.cpython-39.pyc
+Comment: 
+
+Filename: subscriptions/__pycache__/utils.cpython-39.pyc
+Comment: 
+
+Filename: subscriptions/__pycache__/views.cpython-39.pyc
 Comment: 
 
 Filename: subscriptions/api/fields.py
 Comment: 
 
 Filename: subscriptions/api/serializers.py
 Comment: 
 
 Filename: subscriptions/api/urls.py
 Comment: 
 
 Filename: subscriptions/api/views.py
 Comment: 
 
+Filename: subscriptions/api/__pycache__/fields.cpython-39.pyc
+Comment: 
+
+Filename: subscriptions/api/__pycache__/serializers.cpython-39.pyc
+Comment: 
+
+Filename: subscriptions/api/__pycache__/urls.cpython-39.pyc
+Comment: 
+
+Filename: subscriptions/api/__pycache__/views.cpython-39.pyc
+Comment: 
+
+Filename: subscriptions/management/commands/check_unfinished_payments.py
+Comment: 
+
 Filename: subscriptions/migrations/0001_initial.py
 Comment: 
 
-Filename: subscriptions/migrations/0002_alter_subscription_begin.py
+Filename: subscriptions/migrations/0002_subscriptionpayment_metadata_and_more.py
+Comment: 
+
+Filename: subscriptions/migrations/0003_remove_subscriptionpayment_subscription_charge_date_and_more.py
+Comment: 
+
+Filename: subscriptions/migrations/0004_remove_plan_unique_plan_slug_remove_plan_slug.py
+Comment: 
+
+Filename: subscriptions/migrations/0005_alter_subscriptionpayment_metadata_and_more.py
+Comment: 
+
+Filename: subscriptions/migrations/0006_subscription_quantity.py
+Comment: 
+
+Filename: subscriptions/migrations/0007_alter_subscriptionpayment_provider_transaction_id_and_more.py
+Comment: 
+
+Filename: subscriptions/migrations/0008_subscriptionpayment_quantity.py
+Comment: 
+
+Filename: subscriptions/migrations/0009_auto_20220711_2159.py
+Comment: 
+
+Filename: subscriptions/migrations/0010_subscription_auto_prolong_and_more.py
+Comment: 
+
+Filename: subscriptions/migrations/0011_alter_plan_charge_amount_currency_alter_plan_id_and_more.py
+Comment: 
+
+Filename: subscriptions/migrations/0012_subscription_uid_subscriptionpayment_uid_and_more.py
 Comment: 
 
-Filename: subscriptions/migrations/0003_alter_plan_charge_amount_alter_usage_datetime.py
+Filename: subscriptions/migrations/0013_alter_subscription_uid_alter_subscriptionpayment_uid_and_more.py
 Comment: 
 
-Filename: subscriptions/migrations/0004_rename_begin_subscription_start.py
+Filename: subscriptions/migrations/0014_subscriptionpayment_subscription_uid_and_more.py
 Comment: 
 
-Filename: subscriptions/migrations/0005_plan_slug.py
+Filename: subscriptions/migrations/0015_auto_20220728_1920.py
 Comment: 
 
-Filename: subscriptions/migrations/0006_alter_plan_charge_period_and_more.py
+Filename: subscriptions/migrations/0016_remove_subscriptionpayment_subscription_and_more.py
 Comment: 
 
-Filename: subscriptions/migrations/0007_subscriptionpayment_and_more.py
+Filename: subscriptions/migrations/0017_alter_subscriptionpayment_subscription_uid_and_more.py
 Comment: 
 
-Filename: subscriptions/migrations/0008_rename_vendor_subscriptionpayment_provider_name_and_more.py
+Filename: subscriptions/migrations/0018_remove_subscription_id_remove_subscriptionpayment_id_and_more.py
+Comment: 
+
+Filename: subscriptions/migrations/0019_rename_subscription_uid_subscriptionpayment_subscription_and_more.py
+Comment: 
+
+Filename: subscriptions/migrations/0020_alter_subscriptionpaymentrefund_original_payment_and_more.py
+Comment: 
+
+Filename: subscriptions/migrations/0021_alter_subscriptionpayment_subscription_and_more.py
+Comment: 
+
+Filename: subscriptions/migrations/0022_alter_subscriptionpayment_subscription_and_more.py
+Comment: 
+
+Filename: subscriptions/migrations/0023_alter_subscription_options_and_more.py
+Comment: 
+
+Filename: subscriptions/migrations/0024_alter_subscriptionpayment_amount_and_more.py
+Comment: 
+
+Filename: subscriptions/migrations/0025_feature_tier_plan_tier.py
+Comment: 
+
+Filename: subscriptions/migrations/0026_alter_subscriptionpayment_status_and_more.py
+Comment: 
+
+Filename: subscriptions/migrations/0027_auto_20221109_1525.py
+Comment: 
+
+Filename: subscriptions/migrations/0028_tier_level.py
+Comment: 
+
+Filename: subscriptions/migrations/0029_alter_plan_charge_amount_currency_and_more.py
+Comment: 
+
+Filename: subscriptions/migrations/0030_feature_is_negative.py
+Comment: 
+
+Filename: subscriptions/migrations/0031_alter_plan_tier.py
+Comment: 
+
+Filename: subscriptions/migrations/0032_alter_subscriptionpayment_options_and_more.py
+Comment: 
+
+Filename: subscriptions/migrations/0032_auto_20230417_1312.py
+Comment: 
+
+Filename: subscriptions/migrations/0032_subscription_initial_charge_offset_and_more.py
 Comment: 
 
 Filename: subscriptions/migrations/__init__.py
 Comment: 
 
 Filename: subscriptions/providers/__init__.py
 Comment: 
 
+Filename: subscriptions/providers/__pycache__/__init__.cpython-39.pyc
+Comment: 
+
+Filename: subscriptions/providers/apple_in_app/__init__.py
+Comment: 
+
+Filename: subscriptions/providers/apple_in_app/api.py
+Comment: 
+
+Filename: subscriptions/providers/apple_in_app/app_store.py
+Comment: 
+
+Filename: subscriptions/providers/apple_in_app/enums.py
+Comment: 
+
+Filename: subscriptions/providers/apple_in_app/exceptions.py
+Comment: 
+
+Filename: subscriptions/providers/apple_in_app/certs/AppleRootCA-G3.cer
+Comment: 
+
+Filename: subscriptions/providers/apple_in_app/certs/AppleRootCertificate.cer
+Comment: 
+
 Filename: subscriptions/providers/dummy/__init__.py
 Comment: 
 
 Filename: subscriptions/providers/dummy/forms.py
 Comment: 
 
-Filename: subscriptions/providers/stripe/__init__.py
+Filename: subscriptions/providers/dummy/serializers.py
 Comment: 
 
-Filename: subscriptions/providers/stripe/models.py
+Filename: subscriptions/providers/dummy/__pycache__/__init__.cpython-39.pyc
+Comment: 
+
+Filename: subscriptions/providers/dummy/__pycache__/forms.cpython-39.pyc
+Comment: 
+
+Filename: subscriptions/providers/dummy/__pycache__/models.cpython-39.pyc
+Comment: 
+
+Filename: subscriptions/providers/google_in_app/__init__.py
 Comment: 
 
-Filename: subscriptions/templates/subscriptions/pay.html
+Filename: subscriptions/providers/google_in_app/exceptions.py
 Comment: 
 
-Filename: subscriptions/templates/subscriptions/payment-success.html
+Filename: subscriptions/providers/google_in_app/models.py
+Comment: 
+
+Filename: subscriptions/providers/google_in_app/tasks.py
+Comment: 
+
+Filename: subscriptions/providers/paddle/__init__.py
+Comment: 
+
+Filename: subscriptions/providers/paddle/api.py
+Comment: 
+
+Filename: subscriptions/providers/paddle/models.py
+Comment: 
+
+Filename: subscriptions/providers/stripe/__init__.py
+Comment: 
+
+Filename: subscriptions/providers/stripe/models.py
 Comment: 
 
 Filename: subscriptions/templates/subscriptions/plan.html
 Comment: 
 
 Filename: subscriptions/templates/subscriptions/plans.html
 Comment: 
 
-Filename: django_subscriptions_rt-0.0.1.dist-info/METADATA
+Filename: subscriptions/templates/subscriptions/subscribe-success.html
+Comment: 
+
+Filename: subscriptions/templates/subscriptions/subscribe.html
+Comment: 
+
+Filename: django_subscriptions_rt-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: django_subscriptions_rt-0.0.1.dist-info/WHEEL
+Filename: django_subscriptions_rt-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: django_subscriptions_rt-0.0.1.dist-info/top_level.txt
+Filename: django_subscriptions_rt-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: django_subscriptions_rt-0.0.1.dist-info/RECORD
+Filename: django_subscriptions_rt-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## subscriptions/admin.py

```diff
@@ -1,27 +1,62 @@
 from django.contrib import admin
 
-from .models import Plan, Quota, Resource, Subscription, SubscriptionPayment, SubscriptionPaymentRefund, Tax, Usage
+from .models import Plan, Quota, Resource, Subscription, SubscriptionPayment, SubscriptionPaymentRefund, Tax, Usage, Tier, Feature
+
+
+class QuotaInline(admin.TabularInline):
+    model = Quota
+    extra = 0
+
+
+@admin.register(Feature)
+class FeatureAdmin(admin.ModelAdmin):
+    list_display = 'codename', 'description',
+    search_fields = 'codename',
+    ordering = 'codename',
+
+
+@admin.register(Tier)
+class TierAdmin(admin.ModelAdmin):
+    list_display = 'codename', 'description', 'is_default', 'level',
+    search_fields = 'codename',
+    ordering = '-level', 'codename',
 
 
 @admin.register(Plan)
 class PlanAdmin(admin.ModelAdmin):
-    list_display = 'codename', 'name', 'charge_amount', 'charge_period', 'max_duration', 'is_enabled',
+    list_display = 'codename', 'name', 'is_recurring', 'charge_amount', 'charge_period', 'max_duration', 'tier', 'is_enabled',
     list_filter = 'is_enabled',
     search_fields = 'codename', 'name',
     ordering = '-pk',
-    prepopulated_fields = {'slug': ('name',)}
+    inlines = QuotaInline,
+
+    @admin.display(boolean=True, description='recurring')
+    def is_recurring(self, instance):
+        return instance.is_recurring()
+
+
+class SubscriptionPaymentInline(admin.StackedInline):
+    model = SubscriptionPayment
+    extra = 0
+    fields = 'uid', 'created', 'status', 'amount', 'quantity', 'provider_codename', 'provider_transaction_id', 'subscription_start', 'subscription_end',
+    readonly_fields = 'created',
+    ordering = '-subscription_end',
 
 
 @admin.register(Subscription)
 class SubscriptionAdmin(admin.ModelAdmin):
     list_display = 'user', 'plan', 'start', 'end',
+    autocomplete_fields = 'user',
     list_filter = 'plan', 'start', 'end',
-    search_fields = 'user',
-    ordering = '-pk',
+    search_fields = 'user__email', 'user__first_name', 'user__last_name',
+    inlines = [
+        SubscriptionPaymentInline,
+    ]
+    ordering = '-start', 'uid',
 
 
 @admin.register(Resource)
 class ResourceAdmin(admin.ModelAdmin):
     list_display = 'codename', 'units',
     search_fields = 'codename',
     ordering = 'codename',
@@ -33,37 +68,52 @@
     list_filter = 'plan', 'resource', 'recharge_period', 'burns_in',
     ordering = 'plan', 'resource', 'pk',
 
 
 @admin.register(Usage)
 class UsageAdmin(admin.ModelAdmin):
     list_display = 'user', 'resource', 'amount', 'datetime',
+    autocomplete_fields = 'user',
     list_filter = 'datetime', 'resource',
-    search_fields = 'user',
+    search_fields = 'user__email', 'user__first_name', 'user__last_name',
     ordering = '-pk',
 
 
+class SubscriptionPaymentRefundInline(admin.StackedInline):
+    model = SubscriptionPaymentRefund
+    extra = 0
+    fields = 'uid', 'original_payment', 'created', 'status', 'amount', 'provider_codename', 'provider_transaction_id',
+    readonly_fields = 'created',
+    ordering = '-original_payment__subscription_end',
+
+
 @admin.register(SubscriptionPayment)
 class SubscriptionPaymentAdmin(admin.ModelAdmin):
-    list_display = 'pk', 'status', 'created', 'updated', 'amount', 'user', 'subscription', 'subscription_charge_date', 'provider_name',
-    list_filter = 'subscription__plan', 'status', 'created', 'updated', 'provider_name',
-    search_fields = 'user', 'amount',
+    list_display = 'pk', 'status', 'created', 'amount', 'user', 'subscription_start', 'subscription_end',
+    autocomplete_fields = 'user', 'subscription',
+    list_filter = 'subscription__plan', 'status', 'created', 'updated', 'provider_codename',
+    search_fields = 'uid', 'user__email', 'user__first_name', 'user__last_name', 'amount',
+    inlines = [
+        SubscriptionPaymentRefundInline,
+    ]
     queryset = SubscriptionPayment.objects.select_related('subscription__plan')
-    ordering = '-pk',
+    ordering = '-created',
 
 
 @admin.register(SubscriptionPaymentRefund)
 class SubscriptionPaymentRefundAdmin(admin.ModelAdmin):
     list_display = 'pk', 'status', 'original_payment', 'created', 'updated', 'amount'
+    autocomplete_fields = 'original_payment',
     list_filter = 'status', 'created', 'updated',
-    search_fieds = 'original_payment__user'
+    search_fields = 'original_payment__user__email',
     queryset = SubscriptionPaymentRefund.objects.select_related('original_payment__user')
-    ordering = '-pk',
+    ordering = '-created',
 
 
 @admin.register(Tax)
 class TaxAdmin(admin.ModelAdmin):
     list_display = 'subscription_payment', 'amount',
+    autocomplete_fields = 'subscription_payment',
     list_filter = 'subscription_payment__status',
-    search_fields = 'subscription_payment',
+    search_fields = 'subscription_payment__user__email',
     queryset = Tax.objects.select_related('subscription_payment')
     ordering = '-pk',
```

## subscriptions/exceptions.py

```diff
@@ -1,17 +1,31 @@
-
-
 class QuotaLimitExceeded(Exception):
     pass
 
 
 class InconsistentQuotaCache(Exception):
     pass
 
 
 class ProviderNotFound(Exception):
     pass
 
 
+class ProlongationImpossible(Exception):
+    pass
+
+
+class SubscriptionError(Exception):
+    pass
+
+
 class PaymentError(Exception):
-    user_message: str = 'unknown error'
+    user_message: str = 'unknown error'  # TODO: won't work with __init__()
     code = 'unknown'
+
+
+class BadReferencePayment(PaymentError):
+    pass
+
+
+class InvalidOperation(Exception):
+    pass
```

## subscriptions/functions.py

```diff
@@ -1,20 +1,29 @@
-from datetime import datetime
+from contextlib import contextmanager, suppress
+from datetime import datetime, timedelta, timezone
+from functools import cached_property
+from itertools import chain
 from logging import getLogger
 from operator import attrgetter
-from typing import Dict, Iterable, Iterator, List, Optional
+from typing import Callable, Dict, Iterable, Iterator, List, Optional, Set
 
+from django.conf import settings
+from django.contrib.auth import get_user_model
 from django.contrib.auth.models import AbstractUser
+from django.core.cache import InvalidCacheBackendError, caches
+from django.core.cache.backends.base import BaseCache
+from django.db import transaction
 from django.db.models import Prefetch
 from django.utils.timezone import now
 from more_itertools import spy
 
-from subscriptions.exceptions import QuotaLimitExceeded
-from subscriptions.models import Quota, QuotaCache, QuotaChunk, Resource, Subscription, Usage
-from subscriptions.utils import merge_iter
+from .defaults import DEFAULT_SUBSCRIPTIONS_CACHE_NAME
+from .exceptions import InconsistentQuotaCache, QuotaLimitExceeded
+from .models import INFINITY, Feature, Plan, Quota, QuotaCache, QuotaChunk, Resource, Subscription, Tier, Usage
+from .utils import merge_iter
 
 log = getLogger(__name__)
 
 
 def iter_subscriptions_involved(user: AbstractUser, at: datetime) -> Iterator['Subscription']:
     subscriptions = (
         Subscription.objects
@@ -37,15 +46,15 @@
         from_ = min(from_, subscription.start)
 
 
 def iter_subscriptions_quota_chunks(
     subscriptions: Iterable[Subscription],
     since: datetime,
     until: datetime,
-    sort_by: callable = attrgetter('start'),
+    sort_by: Callable = attrgetter('start'),
 ) -> Iterator[QuotaChunk]:
     return merge_iter(
         *(
             subscription.iter_quota_chunks(
                 since=since,
                 until=until,
                 sort_by=sort_by,
@@ -61,27 +70,33 @@
     at: Optional[datetime] = None,
     quota_cache: Optional[QuotaCache] = None,
 ) -> List[QuotaChunk]:
 
     at = at or now()
     subscriptions_involved = iter_subscriptions_involved(user=user, at=at)
 
+    if quota_cache and quota_cache.datetime > at:
+        log.warning('Not using quota cache %s because it is newer than requested time %s', quota_cache, at)
+        quota_cache = None
+
     if quota_cache:
-        assert at >= quota_cache.datetime
-        subscriptions_involved = filter(lambda subscription: subscription.end > quota_cache.datetime, subscriptions_involved)
+        subscriptions_involved = (
+            sub for sub in subscriptions_involved
+            if sub.end > quota_cache.datetime
+        )
 
     first_subscriptions_involved, subscriptions_involved = spy(subscriptions_involved, 1)
     if not first_subscriptions_involved:
         return []
 
     quota_chunks = iter_subscriptions_quota_chunks(
         subscriptions_involved,
         since=quota_cache and quota_cache.datetime,
         until=at,
-        sort_by=attrgetter('start'),
+        sort_by=attrgetter('start', 'end'),
     )
     if quota_cache:
         quota_chunks = quota_cache.apply(quota_chunks)
 
     first_quota_chunks, quota_chunks = spy(quota_chunks, 1)
     if not first_quota_chunks:
         return []
@@ -103,15 +118,15 @@
         if not active_chunks or active_chunks[-1].start <= date:
             for chunk in quota_chunks:
                 active_chunks.append(chunk)
                 if chunk.start > date:
                     break
 
         # remove stale chunks
-        active_chunks = [chunk for chunk in active_chunks if chunk.end >= date and chunk.remains]
+        active_chunks = [chunk for chunk in active_chunks if chunk.end >= date]
 
         # select & sort chunks to consume from
         chunks_to_consume = sorted(
             (chunk for chunk in active_chunks if chunk.start <= date < chunk.end and chunk.resource.id == resource_id),
             key=attrgetter('end'),
         )
 
@@ -123,15 +138,15 @@
                 break
             else:
                 amount -= chunk.remains
                 chunk.remains = 0
 
         # check whether limit was exceeded (== amount was fully covered by chunks consumed)
         if amount:
-            raise QuotaLimitExceeded(f'Quota limit exceeded: {date=} {amount=}')
+            log.error('Quota limit exceeded: usage date=%s overused=%s', date, amount)
 
     # ---- now calculate remaining amount at `at` ----
 
     # leave chunks that exist at `at`
     active_chunks = [chunk for chunk in active_chunks if chunk.includes(at)]
 
     # add chunks to active_chunks until they bypass "date"
@@ -141,18 +156,198 @@
 
         if chunk.includes(at):
             active_chunks.append(chunk)
 
     return active_chunks
 
 
+def get_cache_name() -> str:
+    return getattr(settings, 'SUBSCRIPTIONS_CACHE_NAME', DEFAULT_SUBSCRIPTIONS_CACHE_NAME)
+
+
+def get_cache_or_none(cache_name: str) -> Optional[BaseCache]:
+    try:
+        return caches[cache_name]
+    except InvalidCacheBackendError:
+        log.exception('Could not access cache "%s"', cache_name)
+
+
 def get_remaining_amount(
     user: AbstractUser,
     at: Optional[datetime] = None,
-    quota_cache: Optional[QuotaCache] = None,
 ) -> Dict[Resource, int]:
+    at = at or now()
+
+    cache = get_cache_or_none(get_cache_name())
+    quota_cache = cache and cache.get(user.pk, None)
+
+    try:
+        remaining_chunks = get_remaining_chunks(user=user, at=at, quota_cache=quota_cache)
+    except InconsistentQuotaCache:
+        log.exception('Dropping inconsistent quota cache for user %s', user.pk)
+        cache.delete(user.pk)
+        remaining_chunks = get_remaining_chunks(user=user, at=at)
+
+    if cache and (not quota_cache or quota_cache.datetime < at < now()):
+        cache.set(user.pk, QuotaCache(
+            datetime=at,
+            chunks=remaining_chunks,
+        ))
 
     amount = {}
-    for chunk in get_remaining_chunks(user=user, at=at, quota_cache=quota_cache):
+    for chunk in remaining_chunks:
         amount[chunk.resource] = amount.setdefault(chunk.resource, 0) + chunk.remains
 
     return amount
+
+
+@contextmanager
+def use_resource(user: AbstractUser, resource: Resource, amount: int = 1, raises: bool = True) -> int:
+    with transaction.atomic():
+        available = get_remaining_amount(user).get(resource, 0)
+        remains = available - amount
+
+        if remains < 0 and raises:
+            raise QuotaLimitExceeded(f'Not enough {resource}: tried to use {amount}, but only {available} is available')
+
+        Usage.objects.create(
+            user=user,
+            resource=resource,
+            amount=amount,
+        )
+        yield remains
+
+
+def merge_feature_sets(*feature_sets: Iterable[Feature]) -> Set[Feature]:
+    """
+    Merge features from different subscriptions in human-meaningful way.
+    Positive feature stays if it appears in at least one subscription,
+    negative feature stays if it appears in all subscriptions.
+    """
+    features = set(chain(*feature_sets))
+
+    # remove negative feature if there is at least one set without it;
+    # for example, if there are sets {SHOW_ADS, ...}, {SHOW_ADS, ...}, {...},
+    # then result won't contain SHOW_ADS feature
+    negative_features = {feature for feature in features if feature.is_negative}
+    for negative_feature in negative_features:
+        if any(negative_feature not in feature_set for feature_set in feature_sets):
+            features.remove(negative_feature)
+
+    return features
+
+
+class cache:
+
+    def __init__(self, key: str, cache_name: str = 'default', timeout: Optional[timedelta] = None, version: Optional[int] = None):
+        self.cache_name = cache_name
+        self.key = key
+        self.timeout = timeout
+        self.version = version
+
+    def __call__(self, fn: Callable) -> Callable:
+
+        class Wrapper:
+            def __init__(self_, fn: Callable):
+                self_.fn = fn
+                self_.timeout = self.timeout
+                self_.version = self.version
+
+            @cached_property
+            def cache(self_) -> BaseCache:
+                return caches[self.cache_name]
+
+            @classmethod
+            def get_key(cls, *args, **kwargs) -> str:
+                if args or kwargs:
+                    raise NotImplementedError()
+                return self.key
+
+            def __call__(self_, *args, **kwargs):
+                key = self_.get_key(*args, **kwargs)
+                return self_.cache.get_or_set(
+                    key,
+                    lambda: self_.fn(*args, **kwargs),
+                    timeout=self_.timeout and int(self_.timeout.total_seconds()),
+                    version=self_.version,
+                )
+
+            def cache_clear(self_, *args, **kwargs) -> bool:
+                key = self_.get_key(*args, **kwargs)
+                return self_.cache.delete(key)
+
+        return Wrapper(fn)
+
+
+def get_default_features() -> Set[Feature]:
+    default_tiers = Tier.objects.filter(is_default=True).prefetch_related('features')
+    return merge_feature_sets(*(tier.features.all() for tier in default_tiers))
+
+
+def get_default_plan_id() -> Optional[int]:
+    with suppress(AttributeError, ImportError):
+        from constance import config
+        return config.SUBSCRIPTIONS_DEFAULT_PLAN_ID
+
+
+def get_default_plan() -> Optional[Plan]:
+    from .models import Plan
+
+    if not (default_plan_id := get_default_plan_id()):
+        return
+
+    return Plan.objects.get(id=default_plan_id)
+
+
+def add_default_plan_to_users():
+    User = get_user_model()
+
+    try:
+        default_plan = get_default_plan()
+    except Plan.DoesNotExist:
+        return
+
+    now_ = now()
+    for user in User.objects.all():
+        last_subscription = user.subscriptions.recurring().order_by('end').last()
+        if last_subscription and last_subscription.plan == default_plan and last_subscription.end > now_:
+            continue
+
+        start = max(last_subscription.end, now_) if last_subscription else now_
+        Subscription.objects.create(
+            user=user,
+            plan=default_plan,
+            start=start,
+            end=start+INFINITY,
+        )
+
+
+def get_resource_refresh_moments(
+    user: AbstractUser,
+    at: Optional[datetime] = None,
+    assume_subscription_refresh: bool = True,
+) -> dict[Resource, datetime]:
+    """
+    For given user and moment in time, provides information when all the resources will be refreshed.
+    If the given resource won't be refreshed (e.g. because subscription ends), it will be absent from the dictionary.
+
+    If `assume_subscription_refresh` is set to `True` we allow
+    the recharge moments to be beyond the current subscription end.
+    """
+    at = at or now()
+    result = {}
+    datetime_max = datetime.max.replace(tzinfo=timezone.utc)
+
+    for subscription in iter_subscriptions_involved(user, at):
+        for quota in subscription.plan.quotas.all():
+            # Find first moment after `at` that will be a recharge.
+            recharge_moment = subscription.start
+            while recharge_moment < at:
+                recharge_moment += quota.recharge_period
+            # If we get a recharge after the subscription will end, it is of no use.
+            if recharge_moment >= subscription.end and not assume_subscription_refresh:
+                continue
+            # If multiple quotas from multiple subscription affect this resource,
+            # point at the one that happens earliest.
+            result[quota.resource] = min(result.get(quota.resource, datetime_max), recharge_moment)
+
+    return result
```

## subscriptions/middleware.py

```diff
@@ -1,11 +1,11 @@
 from django.utils.deprecation import MiddlewareMixin
 
-from subscriptions.functions import get_remaining_amount
-from subscriptions.models import Subscription
+from .functions import get_remaining_amount
+from .models import Subscription
 
 
 class SubscriptionsMiddleware(MiddlewareMixin):
     def process_request(self, request):
         is_auth = request.user.is_authenticated
         request.user.active_subscriptions = Subscription.objects.filter(user=request.user).active() if is_auth else []
         request.user.quotas = get_remaining_amount(user=request.user) if is_auth else {}
```

## subscriptions/models.py

```diff
@@ -1,26 +1,36 @@
 from __future__ import annotations
 
+from collections import defaultdict
+from contextlib import suppress
 from dataclasses import dataclass
 from datetime import datetime, timedelta
-from itertools import count, islice, zip_longest
+from itertools import count, islice
+from logging import getLogger
 from operator import attrgetter
-from typing import TYPE_CHECKING, Iterable, Iterator, List, Optional
+from typing import TYPE_CHECKING, Callable, Iterable, Iterator, List, Optional
+from uuid import uuid4
 
 from dateutil.relativedelta import relativedelta
 from django.conf import settings
+from django.contrib.auth.models import AbstractBaseUser
+from django.core.serializers.json import DjangoJSONEncoder
 from django.db import models
-from django.db.models import Index, QuerySet, UniqueConstraint
+from django.db.models import F, Q, DateTimeField, ExpressionWrapper, Index, QuerySet, UniqueConstraint
+from django.db.models.functions import Least
 from django.urls import reverse
 from django.utils.timezone import now
+from pydantic import BaseModel
 
-from .exceptions import InconsistentQuotaCache, QuotaLimitExceeded
+from .exceptions import InconsistentQuotaCache, PaymentError, ProlongationImpossible, ProviderNotFound
 from .fields import MoneyField, RelativeDurationField
 from .utils import merge_iter
 
+log = getLogger(__name__)
+
 if TYPE_CHECKING:
     from .providers import Provider
 
 INFINITY = relativedelta(days=365 * 1000)
 
 
 class Resource(models.Model):
@@ -32,137 +42,223 @@
             UniqueConstraint(fields=['codename'], name='unique_resource'),
         ]
 
     def __str__(self) -> str:
         return self.codename
 
 
+class Feature(models.Model):
+    codename = models.CharField(max_length=255, unique=True)
+    description = models.TextField(blank=True)
+    is_negative = models.BooleanField(default=False)
+
+    def __str__(self) -> str:
+        return self.codename
+
+
+class Tier(models.Model):
+    codename = models.CharField(max_length=255, unique=True)
+    description = models.TextField(blank=True)
+    is_default = models.BooleanField(db_index=True, default=False)
+    level = models.SmallIntegerField(default=0)
+
+    features = models.ManyToManyField(Feature)
+
+    def __str__(self) -> str:
+        return self.codename
+
+
 class Plan(models.Model):
     codename = models.CharField(max_length=255)
     name = models.CharField(max_length=255)
-    slug = models.SlugField()
     charge_amount = MoneyField(blank=True, null=True)
     charge_period = RelativeDurationField(blank=True, help_text='leave blank for one-time charge')
     max_duration = RelativeDurationField(blank=True, help_text='leave blank to make it an infinite subscription')
+    tier = models.ForeignKey(
+        Tier,
+        on_delete=models.PROTECT,
+        blank=True,
+        null=True,
+        help_text='group of features connected to this plan',
+        related_name='plans',
+    )
+    metadata = models.JSONField(blank=True, default=dict, encoder=DjangoJSONEncoder)
     is_enabled = models.BooleanField(default=True)
 
     class Meta:
         constraints = [
             UniqueConstraint(fields=['codename'], name='unique_plan_codename'),
-            UniqueConstraint(fields=['slug'], name='unique_plan_slug'),
         ]
 
     def __str__(self) -> str:
-        return self.name
+        return f'{self.id} {self.name}'
 
     def get_absolute_url(self) -> str:
-        return reverse('plan', kwargs={'plan_slug': self.slug})
+        return reverse('plan', kwargs={'plan_id': self.id})
 
     def save(self, *args, **kwargs):
         self.charge_period = self.charge_period or INFINITY
         self.max_duration = self.max_duration or INFINITY
         return super().save(*args, **kwargs)
 
+    def is_recurring(self) -> bool:
+        return self.charge_period != INFINITY
+
 
 @dataclass
 class QuotaChunk:
     resource: Resource
     start: datetime
     end: datetime
+    amount: int
     remains: int
 
     def __str__(self) -> str:
-        return f'{self.remains} {self.resource} {self.start} - {self.end}'
+        return f'{self.remains}/{self.amount} {self.resource} {self.start} - {self.end}'
 
     def includes(self, date: datetime) -> bool:
         return self.start <= date < self.end
 
     def same_lifetime(self, other: 'QuotaChunk') -> bool:
         return self.start == other.start and self.end == other.end
 
 
 @dataclass
 class QuotaCache:
     datetime: datetime
     chunks: List[QuotaChunk]
 
-    def apply(self, chunks: Iterable[QuotaChunk]) -> Iterator[QuotaChunk]:
-        cached_chunks = iter(self.chunks)
-
-        # match chunks and cached_chunks one-by-one
-        check_cached_pair = True
-        for i, (chunk, cached_chunk) in enumerate(zip_longest(chunks, cached_chunks, fillvalue=None)):
-            if not chunk and cached_chunk:
-                raise InconsistentQuotaCache(f'Non-paired cached chunk detected at position {i}: {cached_chunk}')
-
-            elif chunk and cached_chunk:
-                if not chunk.same_lifetime(cached_chunk):
-                    raise InconsistentQuotaCache(f'Non-matched cached chunk detected at position {i}: {chunk=}, {cached_chunk=}')
-
-                yield cached_chunk
-
-            elif chunk and not cached_chunk:
-                if check_cached_pair:
-                    if chunk.includes(self.datetime):
-                        raise InconsistentQuotaCache(f'No cached chunk for {chunk}')
-                    check_cached_pair = False
+    def apply(self, target_chunks: Iterable[QuotaChunk]) -> Iterator[QuotaChunk]:
+        """
+        Apply itself to `chunks` without intercepting their order,
+        and yield application results.
+        """
+
+        get_key = attrgetter('resource', 'start', 'end', 'amount')
+        cached_chunks = defaultdict(list)
+        for chunk in self.chunks:
+            cached_chunks[get_key(chunk)].append(chunk)
+
+        for target_chunk in target_chunks:
+            key = get_key(target_chunk)
+            try:
+                yield cached_chunks[key].pop()
+            except IndexError:
+                yield target_chunk
 
-                yield chunk
+        if any((non_paired := values) for values in cached_chunks.values()):
+            raise InconsistentQuotaCache(f'Non-paired cached chunk(s) detected: {non_paired}')
 
 
 class SubscriptionQuerySet(models.QuerySet):
+
+    def overlap(self, since: datetime, until: datetime, include_until: bool = False) -> QuerySet:
+        """ Filter subscriptions that overlap with [since, until) period (include_until==False) or [since, until] period (include_until==True) . """
+        return self.filter(**{
+            'end__gte': since,
+            'start__lte' if include_until else 'start__lt': until,
+        })
+
     def active(self, at: Optional[datetime] = None) -> QuerySet:
         at = at or now()
-        return self.filter(start__lte=at, end__gt=at)
+        return self.overlap(at, at, include_until=True)
+
+    def expiring(self, within: datetime, since: Optional[datetime] = None) -> QuerySet:
+        since = since or now()
+        return self.filter(end__gte=since, end__lte=since + within)
+
+    def recurring(self, predicate: bool = True) -> QuerySet:
+        subscriptions = self.select_related('plan')
+        return subscriptions.exclude(plan__charge_period=INFINITY) if predicate else subscriptions.filter(plan__charge_period=INFINITY)
+
+    def with_ages(self, at: Optional[datetime] = None) -> QuerySet:
+        return self.annotate(
+            age=ExpressionWrapper(Least(at or now(), F('end')) - F('start'), output_field=DateTimeField()),
+        )
+
+    def ended_or_ending(self) -> QuerySet:
+        now_ = now()
+        return self.filter(Q(end__lte=now_) | Q(end__gt=now_, auto_prolong=False))
+
+    def new(self, since: datetime, until: datetime) -> QuerySet:
+        """ Newly created subscriptions within selected period. """
+        return self.filter(start__gte=since, start__lte=until)
 
-    def expiring(self, within: datetime, from_: Optional[datetime] = None) -> QuerySet:
-        from_ = from_ or now()
-        return self.filter(end__gte=from_, end__lte=from_ + within)
+
+def default_initial_charge() -> relativedelta:
+    return relativedelta()
 
 
 class Subscription(models.Model):
+    uid = models.UUIDField(primary_key=True, default=uuid4)
     user = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.PROTECT, related_name='subscriptions')
     plan = models.ForeignKey(Plan, on_delete=models.PROTECT, related_name='subscriptions')
+    auto_prolong = models.BooleanField(default=True)
+    quantity = models.PositiveIntegerField(default=1)
+    initial_charge_offset = RelativeDurationField(default=default_initial_charge)
     start = models.DateTimeField(blank=True)
     end = models.DateTimeField(blank=True)
 
     objects = SubscriptionQuerySet.as_manager()
 
+    class Meta:
+        get_latest_by = 'start'
+
+    @property
+    def id(self) -> Optional[str]:
+        return self.uid and str(self.uid)
+
+    @property
+    def short_id(self) -> Optional[str]:
+        with suppress(TypeError):
+            return self.id[:8]
+
     def __str__(self) -> str:
-        return f'{self.user} @ {self.plan}, {self.start} - {self.end}'
+        return f'{self.short_id} {self.user} {self.plan}, {self.start} - {self.end}'
+
+    @property
+    def max_end(self) -> datetime:
+        return self.start + self.plan.max_duration
 
     def save(self, *args, **kwargs):
         self.start = self.start or now()
-        self.end = self.end or (self.start + self.plan.max_duration)
-        return super().save(*args, **kwargs)
+        self.end = self.end or min(self.start + self.plan.charge_period, self.max_end)
+        super().save(*args, **kwargs)
+        self.adjust_default_subscription()
 
     def stop(self):
         self.end = now()
-        self.save(update_fields=['end'])
+        self.auto_prolong = False
+        self.save(update_fields=['end', 'auto_prolong'])
 
-    @classmethod
-    def get_expiring(cls, within: timedelta) -> QuerySet:
-        return cls.objects.active().expiring(within)
+    def prolong(self) -> datetime:
+        """ Returns next uncovered charge_date or subscription.max_end """
 
-    def prolong(self, for_: Optional[relativedelta] = None):
-        if for_:
-            self.end += for_
+        next_charge_dates = islice(self.iter_charge_dates(since=self.end), 2)
+        if (first_charge_date := next(next_charge_dates)) and self.end == first_charge_date:
+            try:
+                end = next(next_charge_dates)
+            except StopIteration as exc:
+                raise ProlongationImpossible('No next charge date') from exc
         else:
-            max_end = self.start + self.plan.max_duration
-            next_charge_dates = list(islice(self.iter_charge_dates(since=self.end), 2))
-            next_charge_date = next_charge_dates[1] if next_charge_dates[0] == self.end else next_charge_dates[0]
-            self.end = min(max_end, next_charge_date)
+            end = first_charge_date
 
-        self.save()
+        if end > (max_end := self.max_end):
+            if self.end >= max_end:
+                raise ProlongationImpossible('Current subscription end is already the maximum end')
+
+            end = max_end
+
+        return end
 
     def iter_quota_chunks(
         self,
         since: Optional[datetime] = None,
         until: Optional[datetime] = None,
-        sort_by: callable = attrgetter('start'),
+        sort_by: Callable = attrgetter('start'),
     ) -> Iterator[QuotaChunk]:
 
         quotas = self.plan.quotas.all()
         yield from merge_iter(
             *(self._iter_single_quota_chunks(quota=quota, since=since, until=until) for quota in quotas),
             key=sort_by,
         )
@@ -177,48 +273,101 @@
             start = self.start + i * quota.recharge_period
             if start < min_start_time:
                 continue
 
             if start > until:
                 return
 
+            amount = quota.limit * self.quantity
             yield QuotaChunk(
                 resource=quota.resource,
                 start=start,
                 end=min(start + quota.burns_in, self.end),
-                remains=quota.limit,
+                amount=amount,
+                remains=amount,
             )
 
-    def iter_charge_dates(self, since: Optional[datetime] = None) -> Iterator[datetime]:
-        """ Including first charge (i.e. charge to create subscription) """
+    def iter_charge_dates(
+        self,
+        since: datetime | None = None,
+        until: datetime | None = None,
+    ) -> Iterator[datetime]:
+        """ Including first charge """
+
         charge_period = self.plan.charge_period
         since = since or self.start
 
         for i in count(start=0):
-            charge_date = self.start + charge_period * i
+            charge_date = self.start + self.initial_charge_offset + charge_period * i
 
             if charge_date < since:
                 continue
 
+            if until and charge_date > until:
+                return
+
+            if charge_period == INFINITY and i != 0:
+                return
+
             yield charge_date
-            if charge_period == INFINITY:
-                break
 
-    # def get_payment_url(self) -> Optional[str]:
-    #     charge_dates = list(islice(self.iter_charge_dates(since=self.end), 1))
-    #     if not charge_dates:
-    #         return
-
-    #     provider = get_provider(self.provider_name)
-    #     return provider.generate_payment_url(
-    #         charge_date=charge_dates[0],
-    #         subscription_id=self.id,
-    #         amount=self.plan.charge_amount,
-    #         user=self.user,
-    #     )
+    def charge_offline(self):
+        from .providers import get_provider
+
+        last_payment = SubscriptionPayment.get_last_successful(self.user)
+        if not last_payment:
+            raise PaymentError('There is no previous successful payment to take credentials from')
+
+        provider_codename = last_payment.provider_codename
+        try:
+            provider = get_provider(provider_codename)
+        except ProviderNotFound as exc:
+            raise PaymentError(f'Could not retrieve provider "{provider_codename}"') from exc
+
+        provider.charge_offline(
+            user=self.user,
+            plan=self.plan,
+            subscription=self,
+            quantity=self.quantity,
+            reference_payment=last_payment,
+        )
+
+    def adjust_default_subscription(self):
+        # this subscription pushes out every default subscription out of its (start,end) period;
+        # IMPORTANT: this does not "fill in" gaps with default sub if current subscription is shrinked
+
+        from .functions import get_default_plan
+
+        try:
+            default_plan = get_default_plan()
+        except Plan.DoesNotExist:
+            return
+
+        if self.plan == default_plan or not self.plan.is_recurring():
+            return
+
+        default_subscriptions = (
+            Subscription.objects
+            .overlap(self.start, self.end, include_until=True)
+            .filter(user=self.user, plan=default_plan)
+        )
+
+        for default_subscription in default_subscriptions:
+            if default_subscription.start < self.start:  # split default subscription into two parts
+                default_subscription.end = self.start
+                default_subscription.save()
+
+                default_subscription.pk = None
+                default_subscription.start = self.end
+                default_subscription.end = self.end + INFINITY
+                default_subscription.save()
+
+            else:  # just shift default subscription to end of current subscription
+                default_subscription.start = self.end
+                default_subscription.save()
 
 
 class Quota(models.Model):
     plan = models.ForeignKey(Plan, on_delete=models.CASCADE, related_name='quotas')
     resource = models.ForeignKey(Resource, on_delete=models.CASCADE, related_name='quotas')
     limit = models.PositiveIntegerField()
     recharge_period = RelativeDurationField(blank=True, help_text='leave blank for recharging only after each subscription prolongation (charge)')
@@ -226,15 +375,15 @@
 
     class Meta:
         constraints = [
             UniqueConstraint(fields=['plan', 'resource'], name='unique_quota'),
         ]
 
     def __str__(self) -> str:
-        return f'{self.resource} {self.limit:,}{self.resource.units}/{self.recharge_period}, burns in {self.burns_in}'
+        return f'{self.id} {self.resource} {self.limit:,}{self.resource.units}/{self.recharge_period}, burns in {self.burns_in}'
 
     def save(self, *args, **kwargs):
         self.recharge_period = self.recharge_period or self.plan.charge_period
         self.burns_in = self.burns_in or self.recharge_period
         return super().save(*args, **kwargs)
 
 
@@ -246,73 +395,167 @@
 
     class Meta:
         indexes = [
             Index(fields=['user', 'resource']),
         ]
 
     def __str__(self) -> str:
-        return f'{self.amount:,}{self.resource.units} {self.resource} at {self.datetime}'
+        return f'{self.id} {self.amount:,}{self.resource.units} {self.resource} at {self.datetime}'
 
     def save(self, *args, **kwargs):
-        from .functions import get_remaining_amount
-
         self.datetime = self.datetime or now()
-
-        remains = get_remaining_amount(user=self.user, at=self.datetime).get(self.resource, 0)
-        if remains < self.amount:
-            raise QuotaLimitExceeded(f'Tried to use {self.amount} {self.resource}(s) while only {remains} is allowed')
-
         return super().save(*args, **kwargs)
 
 
 class AbstractTransaction(models.Model):
 
     class Status(models.IntegerChoices):
         PENDING = 0
         PREAUTH = 1
         COMPLETED = 2
-        CANCELED = 3
+        CANCELLED = 3
         ERROR = 4
 
-    provider_name = models.CharField(max_length=255)
-    provider_transaction_id = models.CharField(max_length=255)
+    uid = models.UUIDField(primary_key=True, blank=True)
+    provider_codename = models.CharField(max_length=255)
+    provider_transaction_id = models.CharField(max_length=255, blank=True, null=True)
     status = models.PositiveSmallIntegerField(choices=Status.choices, default=Status.PENDING)
-    amount = MoneyField()
+    amount = MoneyField(blank=True, null=True)  # set None for services where the payment information is completely out of reach
     # source = models.ForeignKey(MoneyStorage, on_delete=models.PROTECT, related_name='transactions_out')
     # destination = models.ForeignKey(MoneyStorage, on_delete=models.PROTECT, related_name='transactions_in')
+    metadata = models.JSONField(blank=True, default=dict, encoder=DjangoJSONEncoder)
     created = models.DateTimeField(blank=True, editable=False)
     updated = models.DateTimeField(blank=True, editable=False)
 
     class Meta:
         abstract = True
+        indexes = [
+            Index(fields=('provider_codename', 'provider_transaction_id')),
+        ]
+        get_latest_by = 'created'
 
     def save(self, *args, **kwargs):
         now_ = now()
+        self.uid = self.uid or uuid4()
         self.created = self.created or now_
         self.updated = now_
         return super().save(*args, **kwargs)
 
+    @property
+    def id(self) -> Optional[str]:
+        return self.uid and str(self.uid)
+
+    @property
+    def short_id(self) -> Optional[str]:
+        with suppress(TypeError):
+            return self.id[:8]
+
     def __str__(self) -> str:
-        return f'{self.get_status_display()} {self.amount} via {self.provider_name}'
+        return f'{self.short_id} {self.get_status_display()} {self.amount}'
 
     @property
     def provider(self) -> Provider:
         from .providers import get_provider
-        return get_provider(self.provider_name)
+        return get_provider(self.provider_codename)
 
 
 class SubscriptionPayment(AbstractTransaction):
-    user = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.PROTECT, related_name='%(class)ss')
-    subscription = models.ForeignKey(Subscription, on_delete=models.PROTECT, blank=True, null=True, related_name='%(class)ss')
-    subscription_charge_date = models.DateTimeField()
+    user = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.PROTECT, related_name='payments')
+    plan = models.ForeignKey(Plan, on_delete=models.PROTECT, related_name='payments')
+    subscription = models.ForeignKey(Subscription, on_delete=models.PROTECT, blank=True, null=True, related_name='payments')
+    quantity = models.PositiveIntegerField(default=1)
+
+    # If not specifying following fields, they are set automatically after Subscription
+    # creation / prolongation; however, it works other way round as well: if these fields
+    # are set, their values will be used to adjust subscription duration; this is handy
+    # when payment and subscription info comes from external source and is out of control
+    # of the application.
+    subscription_start = models.DateTimeField(blank=True, null=True)  # TODO: paid from
+    subscription_end = models.DateTimeField(blank=True, null=True)  # TODO: paid until
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._initial_status = self.uid and self.status
+
+    # TODO: changing latest() to `subscription_end` may not work well when subscription_end is None
+    # class Meta:
+    #     get_latest_by = 'subscription_end'
+
+    def __str__(self) -> str:
+        return f'{self.short_id} {self.get_status_display()} {self.user} {self.amount} from={self.subscription_start} until={self.subscription_end}'
+
+    def save(self, *args, **kwargs):
+        assert bool(self.subscription_start) == bool(self.subscription_end), \
+            "subscription_start and subscription_end should both be either set or not"
+
+        if self.status == self.Status.COMPLETED:
+            if (subscription := self.subscription):
+                self.subscription_start = self.subscription_start or subscription.end
+
+                if self.subscription_end:
+                    assert self.subscription_end > self.subscription_start
+
+                    # change existing subscription duration based on payment's end
+                    if self.subscription_end <= subscription.end:
+                        log.warning('Payment\'s end (%s) is earlier than current subscription\'s end (%s) -> payment has no effect', self.subscription_end, subscription.end)
+                    else:
+                        subscription.end = self.subscription_end
+
+                else:
+                    # prolong existing subscription and set payment's (start, end)
+                    subscription.end = subscription.prolong()  # TODO: what if this fails?
+                    self.subscription_end = subscription.end
+
+                subscription.save()
+
+            else:
+                self.subscription = Subscription.objects.create(
+                    user=self.user,
+                    plan=self.plan,
+                    quantity=self.quantity,
+                    start=self.subscription_start,
+                    end=self.subscription_end,
+                )
+                # in case subscription_start and subscription_end are empty:
+                self.subscription_start = self.subscription.start
+                self.subscription_end = self.subscription.end
+
+            new_status = self.status != self._initial_status and self.status
+            if new_status == self.Status.COMPLETED:
+                pass  # TODO: send email if not silent
+
+        return super().save(*args, **kwargs)
+
+    @classmethod
+    def get_last_successful(cls, user: AbstractBaseUser) -> Optional[SubscriptionPayment]:
+        with suppress(cls.DoesNotExist):
+            return cls.objects.filter(
+                user=user,
+                status=SubscriptionPayment.Status.COMPLETED,
+            ).latest()
+
+    @property
+    def meta(self) -> BaseModel:
+        from .providers import get_provider
+
+        provider = get_provider(self.provider_codename)
+        return provider.metadata_class.parse_obj(self.metadata)
+
+    @meta.setter
+    def meta(self, value: BaseModel):
+        self.metadata = value.dict()
 
 
 class SubscriptionPaymentRefund(AbstractTransaction):
     original_payment = models.ForeignKey(SubscriptionPayment, on_delete=models.PROTECT, related_name='refunds')
+    # TODO: add support by providers
 
 
 class Tax(models.Model):
     subscription_payment = models.ForeignKey(SubscriptionPayment, on_delete=models.PROTECT, related_name='taxes')
     amount = MoneyField()
 
     def __str__(self) -> str:
-        return f'{self.amount}'
+        return f'{self.id} {self.amount}'
+
+
+from .signals import create_default_subscription_for_new_user  # noqa
```

## subscriptions/urls.py

```diff
@@ -1,10 +1,10 @@
 from django.urls import path
 
-from .views import PlanListView, PlanPaymentSuccessView, PlanPaymentView, PlanView
+from .views import PlanListView, PlanSubscriptionSuccessView, PlanSubscriptionView, PlanView
 
 urlpatterns = [
     path('', PlanListView.as_view(), name='plan_list'),
-    path('<slug:plan_slug>/', PlanView.as_view(), name='plan'),
-    path('<slug:plan_slug>/pay/', PlanPaymentView.as_view(), name='plan_payment'),
-    path('success', PlanPaymentSuccessView.as_view(), name='plan_payment_success'),
+    path('<int:plan_id>/', PlanView.as_view(), name='plan'),  # TODO
+    path('<int:plan_id>/subscribe/', PlanSubscriptionView.as_view(), name='plan_subscription'),
+    path('success', PlanSubscriptionSuccessView.as_view(), name='plan_subscription_success'),
 ]
```

## subscriptions/utils.py

```diff
@@ -1,20 +1,28 @@
-from typing import Dict, Iterable, Iterator, TypeVar
+from typing import Callable, Dict, Iterable, Iterator, TypeVar
+from datetime import datetime
+from django.conf import settings
+from djmoney.money import Money
+
+from .defaults import DEFAULT_SUBSCRIPTIONS_CURRENCY
+
 
 T = TypeVar('T')
 
 
 class NonMonothonicSequence(Exception):
     pass
 
 
-def merge_iter(*iterables: Iterable[T], key: callable = lambda x: x) -> Iterator[T]:
+def merge_iter(*iterables: Iterable[T], key: Callable = lambda x: x) -> Iterator[T]:
     values: Dict[Iterable[T], T] = {}
-    iterables = [iter(it) for it in iterables]
+
+    # accumulate first value from each iterable
     for iterable in iterables:
+        iterable = iter(iterable)
         try:
             values[iterable] = next(iterable)
         except StopIteration:
             pass
 
     last_min_value = None
     while values:
@@ -24,7 +32,15 @@
             raise NonMonothonicSequence(f'{last_min_value=}, {min_value=}')
         yield (last_min_value := min_value)
         iterable = next(it for it, val in values.items() if val == min_value)
         try:
             values[iterable] = next(iterable)
         except StopIteration:
             del values[iterable]
+
+
+def fromisoformat(value: str) -> datetime:
+    return datetime.fromisoformat(value.replace('Z', '+00:00'))
+
+
+default_currency = getattr(settings, 'SUBSCRIPTIONS_DEFAULT_CURRENCY', DEFAULT_SUBSCRIPTIONS_CURRENCY)
+NO_MONEY = Money(0, default_currency)
```

## subscriptions/views.py

```diff
@@ -1,13 +1,11 @@
-from django.conf import settings
 from django.contrib.auth.mixins import LoginRequiredMixin
 from django.core.exceptions import ValidationError
-from django.http import Http404, HttpResponseRedirect
-from django.urls import reverse_lazy
-from django.views.generic import DetailView, ListView, TemplateView, View
+from django.http import Http404
+from django.views.generic import DetailView, ListView, TemplateView
 
 from .exceptions import PaymentError, ProviderNotFound
 from .models import Plan
 from .providers import get_provider
 
 
 class PlanListView(ListView):
@@ -17,44 +15,38 @@
 
 
 class PlanView(DetailView):
     template_name = 'subscriptions/plan.html'
     model = Plan
 
     def get_object(self):
-        return self.model.objects.get(slug=self.kwargs['plan_slug'])
+        return self.model.objects.get(id=self.kwargs['id'])
 
 
-class PlanPaymentView(LoginRequiredMixin, PlanView):
-    template_name = 'subscriptions/pay.html'
-    success_url = reverse_lazy('plan_payment_success')
+class PlanSubscriptionView(LoginRequiredMixin, PlanView):
+    template_name = 'subscriptions/subscribe.html'
 
     def dispatch(self, request, *args, **kwargs):
-        self.provider_name = request.GET.get('provider', next(iter(settings.PAYMENT_PROVIDERS.keys())))
+        self.provider_codename = request.GET.get('provider')
         try:
-            self.payment_provider = get_provider(self.provider_name)
+            self.payment_provider = get_provider(self.provider_codename)
         except ProviderNotFound:
             raise Http404()
 
-        self.plan = Plan.objects.get(slug=kwargs['plan_slug'])
-
-        if (redirect_url := self.payment_provider.redirect_url):
-            return HttpResponseRedirect(redirect_url)
-
+        self.plan = Plan.objects.get(id=kwargs['id'])
         self.form = form(request.POST or None) if (form := self.payment_provider.form) else None
 
         return super().dispatch(request, *args, **kwargs)
 
     def post(self, request, *args, **kwargs):
 
         if self.form.is_valid():
             try:
-                self.payment = self.payment_provider.process_payment(form_data=self.form.data, request=request, plan=self.plan)
-                return HttpResponseRedirect(self.success_url)
+                return self.payment_provider.process_subscription_request(request=request)
             except PaymentError as exc:
                 self.form.add_error(None, ValidationError(exc.user_message, code=exc.code))
 
         return super().get(request, *args, **kwargs)
 
 
-class PlanPaymentSuccessView(TemplateView):
-    template_name = 'subscriptions/payment-success.html'
+class PlanSubscriptionSuccessView(TemplateView):
+    template_name = 'subscriptions/subscribe-success.html'
```

## subscriptions/api/serializers.py

```diff
@@ -1,38 +1,96 @@
+from contextlib import suppress
+from datetime import datetime
 from decimal import Decimal
 from typing import Optional
+from django.utils.timezone import now
 
-from rest_framework.serializers import ModelSerializer, Serializer, SerializerMethodField
+from rest_framework.serializers import BooleanField, CharField, DateTimeField, IntegerField, ModelSerializer, PrimaryKeyRelatedField, Serializer, SerializerMethodField
 
 from ..fields import relativedelta_to_dict
-from ..models import Plan, Subscription
+from ..models import Plan, Subscription, SubscriptionPayment
 
 
 class PlanSerializer(ModelSerializer):
     charge_amount = SerializerMethodField()
     charge_period = SerializerMethodField()
     max_duration = SerializerMethodField()
 
     class Meta:
         model = Plan
-        fields = 'id', 'codename', 'name', 'charge_amount', 'charge_amount_currency', 'charge_period', 'max_duration',
+        fields = 'id', 'codename', 'name', 'charge_amount', 'charge_amount_currency', 'charge_period', 'max_duration', 'is_recurring', 'metadata',
 
     def get_charge_amount(self, obj) -> Optional[Decimal]:
-        return obj.charge_amount and obj.charge_amount.amount
+        if obj.charge_amount is not None:
+            return obj.charge_amount.amount
 
     def get_charge_period(self, obj) -> dict:
         return relativedelta_to_dict(obj.charge_period)
 
     def get_max_duration(self, obj) -> dict:
         return relativedelta_to_dict(obj.max_duration)
 
 
 class SubscriptionSerializer(ModelSerializer):
     plan = PlanSerializer()
+    next_charge_date = SerializerMethodField()
 
     class Meta:
         model = Subscription
-        fields = 'id', 'plan', 'start', 'end',
+        fields = 'id', 'plan', 'quantity', 'start', 'end', 'next_charge_date',
 
+    def get_next_charge_date(self, obj) -> Optional[datetime]:
+        with suppress(StopIteration):
+            return next(obj.iter_charge_dates(since=now()))
 
-class PaymentSerializer(Serializer):
+
+class PaymentProviderSerializer(Serializer):
+    name = CharField(read_only=True)
+
+
+class PaymentProviderListSerializer(Serializer):
+    providers = PaymentProviderSerializer(read_only=True, many=True)
+
+
+class SubscriptionSelectSerializer(Serializer):
+    plan = PrimaryKeyRelatedField(queryset=Plan.objects.all())
+    quantity = IntegerField(default=1)
+    redirect_url = CharField(read_only=True)
+    background_charge_succeeded = BooleanField(default=False)
+    payment_id = CharField(read_only=True)
+
+
+class WebhookSerializer(Serializer):
+    pass
+
+
+class ResourcesSerializer(Serializer):
     pass  # TODO
+
+
+class SubscriptionPaymentSerializer(ModelSerializer):
+    status = SerializerMethodField()
+    amount = SerializerMethodField()
+    currency = SerializerMethodField()
+    total = SerializerMethodField()
+    subscription = SubscriptionSerializer()
+    paid_from = DateTimeField(source='subscription_start')
+    paid_to = DateTimeField(source='subscription_end')
+
+    class Meta:
+        model = SubscriptionPayment
+        fields = 'id', 'status', 'subscription', 'quantity', 'amount', 'currency', 'total', 'paid_from', 'paid_to', 'created',
+
+    def get_status(self, obj) -> str:
+        return obj.get_status_display().lower()
+
+    def get_amount(self, obj) -> Optional[Decimal]:
+        if obj.amount is not None:
+            return obj.amount.amount
+
+    def get_currency(self, obj) -> Optional[str]:
+        if obj.amount is not None:
+            return str(obj.amount.currency)
+
+    def get_total(self, obj) -> Optional[Decimal]:
+        if obj.amount is not None:
+            return obj.amount.amount * obj.quantity
```

## subscriptions/api/urls.py

```diff
@@ -1,11 +1,28 @@
 from django.urls import re_path
-from subscriptions.api.views import PaymentProviderListView, PaymentView, PaymentWebhookView, PlanListView, \
-                               SubscriptionListView
+from django.views.decorators.csrf import csrf_exempt
+
+from ..providers import get_providers
+from .views import PaymentView, PlanListView, ResourcesView, SubscriptionCancelView, SubscriptionListView, SubscriptionSelectView, build_payment_webhook_view
 
 urlpatterns = [
-    re_path(r'^plans/?$', PlanListView.as_view(), name='plans'),
-    re_path(r'^payment-providers/?$', PaymentProviderListView.as_view(), name='payment_providers'),
-    re_path(r'^subscriptions/?$', SubscriptionListView.as_view(), name='subscriptions'),
-    re_path(r'^pay/?$', PaymentView.as_view(), name='payment'),
-    re_path(r'^webhook/(?P<payment_provider_name>\w+)/?$', PaymentWebhookView.as_view(), name='payment_webhook'),
+    re_path(r'plans/?$', PlanListView.as_view(), name='plans'),
+    re_path(r'subscriptions/?$', SubscriptionListView.as_view(), name='subscriptions'),
+    re_path(r'subscriptions/(?P<uid>[0-9a-f-]{36})/?$', SubscriptionCancelView.as_view(), name='subscription_cancel'),
+    re_path(r'subscribe/?$', SubscriptionSelectView.as_view(), name='subscribe'),
+    re_path(r'resources/?$', ResourcesView.as_view(), name='resources'),
+    re_path(r'payments/(?P<uid>[0-9a-f-]{36})/?$', PaymentView.as_view(), name='payment'),
 ]
+
+for provider in get_providers():
+    if not provider.is_enabled:
+        continue
+
+    urlpatterns += [
+        re_path(
+            f'webhook/{provider.codename}/?$',
+            csrf_exempt(
+                build_payment_webhook_view(provider).as_view()
+            ),
+            name=f'payment_webhook_{provider.codename}',
+        ),
+    ]
```

## subscriptions/api/views.py

```diff
@@ -1,64 +1,233 @@
+from __future__ import annotations
+
+import logging
+from typing import Type
+
+from dateutil.relativedelta import relativedelta
 from django.conf import settings
-from rest_framework.exceptions import NotFound
-from rest_framework.generics import ListAPIView, ListCreateAPIView
+from django.db import transaction
+from django.http import QueryDict
+from django.utils.timezone import now
+from rest_framework.exceptions import PermissionDenied
+from rest_framework.views import APIView
+from rest_framework.generics import DestroyAPIView, GenericAPIView, ListAPIView, RetrieveAPIView
 from rest_framework.permissions import AllowAny, IsAuthenticated
 from rest_framework.response import Response
 from rest_framework.schemas.openapi import AutoSchema
-from rest_framework.views import APIView
 
-from ..exceptions import ProviderNotFound
-from ..models import Plan, Subscription
-from ..providers import get_provider
-from .serializers import PaymentSerializer, PlanSerializer, SubscriptionSerializer
+from subscriptions.functions import get_remaining_amount
+
+from ..defaults import DEFAULT_SUBSCRIPTIONS_SUCCESS_URL, DEFAULT_SUBSCRIPTIONS_TRIAL_PERIOD
+from ..exceptions import PaymentError, SubscriptionError
+from ..models import Plan, Subscription, SubscriptionPayment
+from ..providers import Provider, get_provider, get_providers
+from ..validators import get_validators
+from .serializers import PaymentProviderListSerializer, PlanSerializer, ResourcesSerializer, SubscriptionPaymentSerializer, SubscriptionSelectSerializer, SubscriptionSerializer, WebhookSerializer
+
+log = logging.getLogger(__name__)
+
+
+class ResourceHeadersMixin(APIView):
+    def finalize_response(self, request, *args, **kwargs):
+        response = super().finalize_response(request, *args, **kwargs)
+        if request.user.is_authenticated:
+            for resource, remains in get_remaining_amount(request.user).items():
+                response[f'X-Resource-{resource.codename.capitalize()}'] = remains
+        return response
 
 
 class PlanListView(ListAPIView):
     permission_classes = AllowAny,
     queryset = Plan.objects.filter(is_enabled=True)
     serializer_class = PlanSerializer
     schema = AutoSchema()
     ordering = '-id',
 
 
-class PaymentProviderListView(APIView):
+class PaymentProviderListView(GenericAPIView):
     permission_classes = AllowAny,
     exposed_info_keys = 'description',
+    serializer_class = PaymentProviderListSerializer
 
     def get(self, request, *args, **kwargs) -> Response:
-        providers = {
-            provider: {key: info.get(key) for key in self.exposed_info_keys}
-            for provider, info in settings.PAYMENT_PROVIDERS.items()
-        }
-        return Response(providers)
+        serializer = self.serializer_class({
+            'providers': [
+                {'name': provider.codename}
+                for provider in get_providers()
+                if provider.is_enabled
+            ],
+        })
+
+        return Response(serializer.data)
 
 
-class SubscriptionListView(ListCreateAPIView):
+class SubscriptionListView(ListAPIView):
     permission_classes = IsAuthenticated,
-    queryset = Subscription.objects.active().select_related('plan')
     serializer_class = SubscriptionSerializer
     schema = AutoSchema()
-    ordering = '-end', '-id',
+    ordering = '-end', '-uid',
+
+    def get_queryset(self):
+        return Subscription.objects.active().select_related('plan').filter(user=self.request.user)
 
 
-class PaymentView(APIView):
+class SubscriptionCancelView(DestroyAPIView):
     permission_classes = IsAuthenticated,
-    serializer_class = PaymentSerializer
+    serializer_class = SubscriptionSerializer
     schema = AutoSchema()
+    lookup_url_kwarg = 'uid'
+
+    def get_queryset(self):
+        return Subscription.objects.active().filter(user=self.request.user)
 
+    def perform_destroy(self, instance):
+        instance.end = now()
+        instance.auto_prolong = False
+        instance.save()
+
+
+class SubscriptionSelectView(GenericAPIView):
+    permission_classes = IsAuthenticated,
+    serializer_class = SubscriptionSelectSerializer
+    schema = AutoSchema()
+
+    @classmethod
+    def select_payment_provider(cls) -> Type[Provider]:
+        return get_provider()
+
+    @classmethod
+    def get_trial_period(cls, plan, user) -> relativedelta:
+        trial_period = getattr(settings, 'SUBSCRIPTIONS_TRIAL_PERIOD', DEFAULT_SUBSCRIPTIONS_TRIAL_PERIOD)
+
+        if (
+            trial_period and
+            plan.charge_amount and
+            plan.is_recurring() and
+            not user.payments.filter(status=SubscriptionPayment.Status.COMPLETED).exists() and
+            not user.subscriptions.recurring().exists()
+        ):
+            return trial_period
+
+        return relativedelta(0)
+
+    @transaction.atomic(durable=True)
     def post(self, request, *args, **kwargs) -> Response:
-        raise NotImplementedError()
+        serializer = self.get_serializer(data=request.data)
+        serializer.is_valid(raise_exception=True)
+        # TODO: handle quantity
+
+        plan = serializer.validated_data['plan']
+        quantity = serializer.validated_data['quantity']
+        charge_params = {
+            'user': request.user,
+            'plan': plan,
+            'quantity': quantity,
+        }
 
+        active_subscriptions = request.user.subscriptions.active().order_by('end')
+        for validator in get_validators():
+            try:
+                validator(active_subscriptions, plan)
+            except SubscriptionError as exc:
+                raise PermissionDenied(detail=str(exc)) from exc
 
-class PaymentWebhookView(APIView):
-    permission_classes = AllowAny,
+        provider = self.select_payment_provider()
+        background_charge_succeeded = False
 
-    def dispatch(self, request, *args, **kwargs) -> Response:
         try:
-            self.provider = get_provider(kwargs['payment_provider_name'])
-        except ProviderNotFound:
-            raise NotFound(detail='Provider not found')
+            payment = provider.charge_offline(**charge_params)
+            background_charge_succeeded = True
+            redirect_url = getattr(settings, 'SUBSCRIPTIONS_SUCCESS_URL', DEFAULT_SUBSCRIPTIONS_SUCCESS_URL)
+        except Exception as exc:
+            if not isinstance(exc, (PaymentError, NotImplementedError)):
+                log.exception('Offline charge error')
+
+        if not background_charge_succeeded:
+            trial_period = self.get_trial_period(plan, request.user)
+
+            if trial_period:
+                now_ = now()
+                charge_params.update({
+                    'amount': plan.charge_amount * 0,  # this makes currencies match
+                    'subscription_start': now_,
+                    'subscription_end': now_ + trial_period,
+                })
+
+            payment, redirect_url = provider.charge_online(**charge_params)
+
+            if trial_period:
+                assert not payment.subscription
+                payment.subscription = Subscription.objects.create(
+                    user=request.user,
+                    plan=plan,
+                    quantity=quantity,
+                    start=now_,
+                    end=now_,
+                    initial_charge_offset=trial_period,
+                )
+                payment.subscription.save()
+                payment.save()
+
+        return Response(self.serializer_class({
+            'redirect_url': redirect_url,
+            'background_charge_succeeded': background_charge_succeeded,
+            'quantity': payment.quantity,
+            'plan': payment.plan,
+            'payment_id': payment.id,
+        }).data)
 
-        return super().dispatch(request, *args, **kwargs)
+
+class PaymentWebhookView(GenericAPIView):
+    permission_classes = AllowAny,
+    schema = AutoSchema()
+    serializer_class = WebhookSerializer
 
     def post(self, request, *args, **kwargs) -> Response:
-        return self.provider.handle_webhook(request=request)
+        payload = request.data
+        if isinstance(payload, QueryDict):
+            payload = payload.dict()
+        log.info('Webhook at %s received payload %s', request.build_absolute_uri(), payload)
+        return self.provider.webhook(request=request, payload=payload)
+
+
+def build_payment_webhook_view(provider: Provider) -> GenericAPIView:
+    codename = provider.codename
+
+    class _PaymentWebhookView(PaymentWebhookView):
+        schema = AutoSchema(operation_id_base=f'_{codename}_webhook')
+        provider = get_provider(codename)
+
+    return _PaymentWebhookView
+
+
+class ResourcesView(GenericAPIView):
+    permission_classes = IsAuthenticated,
+    serializer_class = ResourcesSerializer
+    pagination_class = None
+    schema = AutoSchema()
+
+    def get(self, request, *args, **kwargs) -> Response:
+        return Response({
+            resource.codename: amount for resource, amount
+            in get_remaining_amount(request.user).items()
+        })
+
+
+class PaymentView(RetrieveAPIView):
+    """
+    GET request just asks backend to show whatever it has in database, while POST asks backend to force-fetch data from payment provider.
+    """
+    permission_classes = IsAuthenticated,
+    serializer_class = SubscriptionPaymentSerializer
+    schema = AutoSchema()
+    queryset = SubscriptionPayment.objects.all()
+    lookup_url_kwarg = 'uid'
+
+    def post(self, request, *args, **kwargs):
+        """ Fetch payment status from the provider and update status if needed """
+        payment = self.get_object()
+        if payment.status == SubscriptionPayment.Status.PENDING:
+            provider = get_provider(payment.provider_codename)
+            provider.check_payments([payment])
+
+        return self.get(request, *args, **kwargs)
```

## subscriptions/migrations/0001_initial.py

```diff
@@ -1,13 +1,14 @@
-# Generated by Django 4.0.2 on 2022-02-09 11:49
+# Generated by Django 4.0.3 on 2022-03-28 19:58
 
 from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
 import djmoney.models.fields
+import subscriptions.fields
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
@@ -17,58 +18,104 @@
     operations = [
         migrations.CreateModel(
             name='Plan',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('codename', models.CharField(max_length=255)),
                 ('name', models.CharField(max_length=255)),
+                ('slug', models.SlugField()),
                 ('charge_amount_currency', djmoney.models.fields.CurrencyField(choices=[('XUA', 'ADB Unit of Account'), ('AFN', 'Afghan Afghani'), ('AFA', 'Afghan Afghani (1927–2002)'), ('ALL', 'Albanian Lek'), ('ALK', 'Albanian Lek (1946–1965)'), ('DZD', 'Algerian Dinar'), ('ADP', 'Andorran Peseta'), ('AOA', 'Angolan Kwanza'), ('AOK', 'Angolan Kwanza (1977–1991)'), ('AON', 'Angolan New Kwanza (1990–2000)'), ('AOR', 'Angolan Readjusted Kwanza (1995–1999)'), ('ARA', 'Argentine Austral'), ('ARS', 'Argentine Peso'), ('ARM', 'Argentine Peso (1881–1970)'), ('ARP', 'Argentine Peso (1983–1985)'), ('ARL', 'Argentine Peso Ley (1970–1983)'), ('AMD', 'Armenian Dram'), ('AWG', 'Aruban Florin'), ('AUD', 'Australian Dollar'), ('ATS', 'Austrian Schilling'), ('AZN', 'Azerbaijani Manat'), ('AZM', 'Azerbaijani Manat (1993–2006)'), ('BSD', 'Bahamian Dollar'), ('BHD', 'Bahraini Dinar'), ('BDT', 'Bangladeshi Taka'), ('BBD', 'Barbadian Dollar'), ('BYN', 'Belarusian Ruble'), ('BYB', 'Belarusian Ruble (1994–1999)'), ('BYR', 'Belarusian Ruble (2000–2016)'), ('BEF', 'Belgian Franc'), ('BEC', 'Belgian Franc (convertible)'), ('BEL', 'Belgian Franc (financial)'), ('BZD', 'Belize Dollar'), ('BMD', 'Bermudan Dollar'), ('BTN', 'Bhutanese Ngultrum'), ('BOB', 'Bolivian Boliviano'), ('BOL', 'Bolivian Boliviano (1863–1963)'), ('BOV', 'Bolivian Mvdol'), ('BOP', 'Bolivian Peso'), ('BAM', 'Bosnia-Herzegovina Convertible Mark'), ('BAD', 'Bosnia-Herzegovina Dinar (1992–1994)'), ('BAN', 'Bosnia-Herzegovina New Dinar (1994–1997)'), ('BWP', 'Botswanan Pula'), ('BRC', 'Brazilian Cruzado (1986–1989)'), ('BRZ', 'Brazilian Cruzeiro (1942–1967)'), ('BRE', 'Brazilian Cruzeiro (1990–1993)'), ('BRR', 'Brazilian Cruzeiro (1993–1994)'), ('BRN', 'Brazilian New Cruzado (1989–1990)'), ('BRB', 'Brazilian New Cruzeiro (1967–1986)'), ('BRL', 'Brazilian Real'), ('GBP', 'British Pound'), ('BND', 'Brunei Dollar'), ('BGL', 'Bulgarian Hard Lev'), ('BGN', 'Bulgarian Lev'), ('BGO', 'Bulgarian Lev (1879–1952)'), ('BGM', 'Bulgarian Socialist Lev'), ('BUK', 'Burmese Kyat'), ('BIF', 'Burundian Franc'), ('XPF', 'CFP Franc'), ('KHR', 'Cambodian Riel'), ('CAD', 'Canadian Dollar'), ('CVE', 'Cape Verdean Escudo'), ('KYD', 'Cayman Islands Dollar'), ('XAF', 'Central African CFA Franc'), ('CLE', 'Chilean Escudo'), ('CLP', 'Chilean Peso'), ('CLF', 'Chilean Unit of Account (UF)'), ('CNX', 'Chinese People’s Bank Dollar'), ('CNY', 'Chinese Yuan'), ('CNH', 'Chinese Yuan (offshore)'), ('COP', 'Colombian Peso'), ('COU', 'Colombian Real Value Unit'), ('KMF', 'Comorian Franc'), ('CDF', 'Congolese Franc'), ('CRC', 'Costa Rican Colón'), ('HRD', 'Croatian Dinar'), ('HRK', 'Croatian Kuna'), ('CUC', 'Cuban Convertible Peso'), ('CUP', 'Cuban Peso'), ('CYP', 'Cypriot Pound'), ('CZK', 'Czech Koruna'), ('CSK', 'Czechoslovak Hard Koruna'), ('DKK', 'Danish Krone'), ('DJF', 'Djiboutian Franc'), ('DOP', 'Dominican Peso'), ('NLG', 'Dutch Guilder'), ('XCD', 'East Caribbean Dollar'), ('DDM', 'East German Mark'), ('ECS', 'Ecuadorian Sucre'), ('ECV', 'Ecuadorian Unit of Constant Value'), ('EGP', 'Egyptian Pound'), ('GQE', 'Equatorial Guinean Ekwele'), ('ERN', 'Eritrean Nakfa'), ('EEK', 'Estonian Kroon'), ('ETB', 'Ethiopian Birr'), ('EUR', 'Euro'), ('XBA', 'European Composite Unit'), ('XEU', 'European Currency Unit'), ('XBB', 'European Monetary Unit'), ('XBC', 'European Unit of Account (XBC)'), ('XBD', 'European Unit of Account (XBD)'), ('FKP', 'Falkland Islands Pound'), ('FJD', 'Fijian Dollar'), ('FIM', 'Finnish Markka'), ('FRF', 'French Franc'), ('XFO', 'French Gold Franc'), ('XFU', 'French UIC-Franc'), ('GMD', 'Gambian Dalasi'), ('GEK', 'Georgian Kupon Larit'), ('GEL', 'Georgian Lari'), ('DEM', 'German Mark'), ('GHS', 'Ghanaian Cedi'), ('GHC', 'Ghanaian Cedi (1979–2007)'), ('GIP', 'Gibraltar Pound'), ('XAU', 'Gold'), ('GRD', 'Greek Drachma'), ('GTQ', 'Guatemalan Quetzal'), ('GWP', 'Guinea-Bissau Peso'), ('GNF', 'Guinean Franc'), ('GNS', 'Guinean Syli'), ('GYD', 'Guyanaese Dollar'), ('HTG', 'Haitian Gourde'), ('HNL', 'Honduran Lempira'), ('HKD', 'Hong Kong Dollar'), ('HUF', 'Hungarian Forint'), ('IMP', 'IMP'), ('ISK', 'Icelandic Króna'), ('ISJ', 'Icelandic Króna (1918–1981)'), ('INR', 'Indian Rupee'), ('IDR', 'Indonesian Rupiah'), ('IRR', 'Iranian Rial'), ('IQD', 'Iraqi Dinar'), ('IEP', 'Irish Pound'), ('ILS', 'Israeli New Shekel'), ('ILP', 'Israeli Pound'), ('ILR', 'Israeli Shekel (1980–1985)'), ('ITL', 'Italian Lira'), ('JMD', 'Jamaican Dollar'), ('JPY', 'Japanese Yen'), ('JOD', 'Jordanian Dinar'), ('KZT', 'Kazakhstani Tenge'), ('KES', 'Kenyan Shilling'), ('KWD', 'Kuwaiti Dinar'), ('KGS', 'Kyrgystani Som'), ('LAK', 'Laotian Kip'), ('LVL', 'Latvian Lats'), ('LVR', 'Latvian Ruble'), ('LBP', 'Lebanese Pound'), ('LSL', 'Lesotho Loti'), ('LRD', 'Liberian Dollar'), ('LYD', 'Libyan Dinar'), ('LTL', 'Lithuanian Litas'), ('LTT', 'Lithuanian Talonas'), ('LUL', 'Luxembourg Financial Franc'), ('LUC', 'Luxembourgian Convertible Franc'), ('LUF', 'Luxembourgian Franc'), ('MOP', 'Macanese Pataca'), ('MKD', 'Macedonian Denar'), ('MKN', 'Macedonian Denar (1992–1993)'), ('MGA', 'Malagasy Ariary'), ('MGF', 'Malagasy Franc'), ('MWK', 'Malawian Kwacha'), ('MYR', 'Malaysian Ringgit'), ('MVR', 'Maldivian Rufiyaa'), ('MVP', 'Maldivian Rupee (1947–1981)'), ('MLF', 'Malian Franc'), ('MTL', 'Maltese Lira'), ('MTP', 'Maltese Pound'), ('MRU', 'Mauritanian Ouguiya'), ('MRO', 'Mauritanian Ouguiya (1973–2017)'), ('MUR', 'Mauritian Rupee'), ('MXV', 'Mexican Investment Unit'), ('MXN', 'Mexican Peso'), ('MXP', 'Mexican Silver Peso (1861–1992)'), ('MDC', 'Moldovan Cupon'), ('MDL', 'Moldovan Leu'), ('MCF', 'Monegasque Franc'), ('MNT', 'Mongolian Tugrik'), ('MAD', 'Moroccan Dirham'), ('MAF', 'Moroccan Franc'), ('MZE', 'Mozambican Escudo'), ('MZN', 'Mozambican Metical'), ('MZM', 'Mozambican Metical (1980–2006)'), ('MMK', 'Myanmar Kyat'), ('NAD', 'Namibian Dollar'), ('NPR', 'Nepalese Rupee'), ('ANG', 'Netherlands Antillean Guilder'), ('TWD', 'New Taiwan Dollar'), ('NZD', 'New Zealand Dollar'), ('NIO', 'Nicaraguan Córdoba'), ('NIC', 'Nicaraguan Córdoba (1988–1991)'), ('NGN', 'Nigerian Naira'), ('KPW', 'North Korean Won'), ('NOK', 'Norwegian Krone'), ('OMR', 'Omani Rial'), ('PKR', 'Pakistani Rupee'), ('XPD', 'Palladium'), ('PAB', 'Panamanian Balboa'), ('PGK', 'Papua New Guinean Kina'), ('PYG', 'Paraguayan Guarani'), ('PEI', 'Peruvian Inti'), ('PEN', 'Peruvian Sol'), ('PES', 'Peruvian Sol (1863–1965)'), ('PHP', 'Philippine Piso'), ('XPT', 'Platinum'), ('PLN', 'Polish Zloty'), ('PLZ', 'Polish Zloty (1950–1995)'), ('PTE', 'Portuguese Escudo'), ('GWE', 'Portuguese Guinea Escudo'), ('QAR', 'Qatari Rial'), ('XRE', 'RINET Funds'), ('RHD', 'Rhodesian Dollar'), ('RON', 'Romanian Leu'), ('ROL', 'Romanian Leu (1952–2006)'), ('RUB', 'Russian Ruble'), ('RUR', 'Russian Ruble (1991–1998)'), ('RWF', 'Rwandan Franc'), ('SVC', 'Salvadoran Colón'), ('WST', 'Samoan Tala'), ('SAR', 'Saudi Riyal'), ('RSD', 'Serbian Dinar'), ('CSD', 'Serbian Dinar (2002–2006)'), ('SCR', 'Seychellois Rupee'), ('SLL', 'Sierra Leonean Leone'), ('XAG', 'Silver'), ('SGD', 'Singapore Dollar'), ('SKK', 'Slovak Koruna'), ('SIT', 'Slovenian Tolar'), ('SBD', 'Solomon Islands Dollar'), ('SOS', 'Somali Shilling'), ('ZAR', 'South African Rand'), ('ZAL', 'South African Rand (financial)'), ('KRH', 'South Korean Hwan (1953–1962)'), ('KRW', 'South Korean Won'), ('KRO', 'South Korean Won (1945–1953)'), ('SSP', 'South Sudanese Pound'), ('SUR', 'Soviet Rouble'), ('ESP', 'Spanish Peseta'), ('ESA', 'Spanish Peseta (A account)'), ('ESB', 'Spanish Peseta (convertible account)'), ('XDR', 'Special Drawing Rights'), ('LKR', 'Sri Lankan Rupee'), ('SHP', 'St. Helena Pound'), ('XSU', 'Sucre'), ('SDD', 'Sudanese Dinar (1992–2007)'), ('SDG', 'Sudanese Pound'), ('SDP', 'Sudanese Pound (1957–1998)'), ('SRD', 'Surinamese Dollar'), ('SRG', 'Surinamese Guilder'), ('SZL', 'Swazi Lilangeni'), ('SEK', 'Swedish Krona'), ('CHF', 'Swiss Franc'), ('SYP', 'Syrian Pound'), ('STN', 'São Tomé & Príncipe Dobra'), ('STD', 'São Tomé & Príncipe Dobra (1977–2017)'), ('TVD', 'TVD'), ('TJR', 'Tajikistani Ruble'), ('TJS', 'Tajikistani Somoni'), ('TZS', 'Tanzanian Shilling'), ('XTS', 'Testing Currency Code'), ('THB', 'Thai Baht'), ('XXX', 'The codes assigned for transactions where no currency is involved'), ('TPE', 'Timorese Escudo'), ('TOP', 'Tongan Paʻanga'), ('TTD', 'Trinidad & Tobago Dollar'), ('TND', 'Tunisian Dinar'), ('TRY', 'Turkish Lira'), ('TRL', 'Turkish Lira (1922–2005)'), ('TMT', 'Turkmenistani Manat'), ('TMM', 'Turkmenistani Manat (1993–2009)'), ('USD', 'US Dollar'), ('USN', 'US Dollar (Next day)'), ('USS', 'US Dollar (Same day)'), ('UGX', 'Ugandan Shilling'), ('UGS', 'Ugandan Shilling (1966–1987)'), ('UAH', 'Ukrainian Hryvnia'), ('UAK', 'Ukrainian Karbovanets'), ('AED', 'United Arab Emirates Dirham'), ('UYW', 'Uruguayan Nominal Wage Index Unit'), ('UYU', 'Uruguayan Peso'), ('UYP', 'Uruguayan Peso (1975–1993)'), ('UYI', 'Uruguayan Peso (Indexed Units)'), ('UZS', 'Uzbekistani Som'), ('VUV', 'Vanuatu Vatu'), ('VES', 'Venezuelan Bolívar'), ('VEB', 'Venezuelan Bolívar (1871–2008)'), ('VEF', 'Venezuelan Bolívar (2008–2018)'), ('VND', 'Vietnamese Dong'), ('VNN', 'Vietnamese Dong (1978–1985)'), ('CHE', 'WIR Euro'), ('CHW', 'WIR Franc'), ('XOF', 'West African CFA Franc'), ('YDD', 'Yemeni Dinar'), ('YER', 'Yemeni Rial'), ('YUN', 'Yugoslavian Convertible Dinar (1990–1992)'), ('YUD', 'Yugoslavian Hard Dinar (1966–1990)'), ('YUM', 'Yugoslavian New Dinar (1994–2002)'), ('YUR', 'Yugoslavian Reformed Dinar (1992–1993)'), ('ZWN', 'ZWN'), ('ZRN', 'Zairean New Zaire (1993–1998)'), ('ZRZ', 'Zairean Zaire (1971–1993)'), ('ZMW', 'Zambian Kwacha'), ('ZMK', 'Zambian Kwacha (1968–2012)'), ('ZWD', 'Zimbabwean Dollar (1980–2008)'), ('ZWR', 'Zimbabwean Dollar (2008)'), ('ZWL', 'Zimbabwean Dollar (2009)')], default='USD', editable=False, max_length=3)),
-                ('charge_amount', djmoney.models.fields.MoneyField(decimal_places=2, default_currency='USD', max_digits=14)),
-                ('charge_period', models.DurationField(blank=True, help_text='leave blank for one-time charge')),
-                ('subscription_duration', models.DurationField(blank=True, help_text='leave blank to make it an infinite subscription')),
+                ('charge_amount', djmoney.models.fields.MoneyField(blank=True, decimal_places=2, default_currency='USD', max_digits=14, null=True)),
+                ('charge_period', subscriptions.fields.RelativeDurationField(blank=True, encoder=subscriptions.fields.RelativedeltaEncoder, help_text='leave blank for one-time charge')),
+                ('max_duration', subscriptions.fields.RelativeDurationField(blank=True, encoder=subscriptions.fields.RelativedeltaEncoder, help_text='leave blank to make it an infinite subscription')),
                 ('is_enabled', models.BooleanField(default=True)),
             ],
         ),
         migrations.CreateModel(
             name='Quota',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('limit', models.PositiveIntegerField()),
-                ('recharge_period', models.DurationField(blank=True, help_text='leave blank for recharging only after each subscription prolongation (charge)')),
-                ('burns_in', models.DurationField(blank=True, help_text='leave blank to burn each recharge period')),
+                ('recharge_period', subscriptions.fields.RelativeDurationField(blank=True, encoder=subscriptions.fields.RelativedeltaEncoder, help_text='leave blank for recharging only after each subscription prolongation (charge)')),
+                ('burns_in', subscriptions.fields.RelativeDurationField(blank=True, encoder=subscriptions.fields.RelativedeltaEncoder, help_text='leave blank to burn each recharge period')),
             ],
         ),
         migrations.CreateModel(
             name='Resource',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('codename', models.CharField(max_length=255)),
                 ('units', models.CharField(blank=True, max_length=255)),
             ],
         ),
         migrations.CreateModel(
+            name='Subscription',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('start', models.DateTimeField(blank=True)),
+                ('end', models.DateTimeField(blank=True)),
+                ('plan', models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, related_name='subscriptions', to='subscriptions.plan')),
+                ('user', models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, related_name='subscriptions', to=settings.AUTH_USER_MODEL)),
+            ],
+        ),
+        migrations.CreateModel(
+            name='SubscriptionPayment',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('provider_codename', models.CharField(max_length=255)),
+                ('provider_transaction_id', models.CharField(max_length=255)),
+                ('status', models.PositiveSmallIntegerField(choices=[(0, 'Pending'), (1, 'Preauth'), (2, 'Completed'), (3, 'Canceled'), (4, 'Error')], default=0)),
+                ('amount_currency', djmoney.models.fields.CurrencyField(choices=[('XUA', 'ADB Unit of Account'), ('AFN', 'Afghan Afghani'), ('AFA', 'Afghan Afghani (1927–2002)'), ('ALL', 'Albanian Lek'), ('ALK', 'Albanian Lek (1946–1965)'), ('DZD', 'Algerian Dinar'), ('ADP', 'Andorran Peseta'), ('AOA', 'Angolan Kwanza'), ('AOK', 'Angolan Kwanza (1977–1991)'), ('AON', 'Angolan New Kwanza (1990–2000)'), ('AOR', 'Angolan Readjusted Kwanza (1995–1999)'), ('ARA', 'Argentine Austral'), ('ARS', 'Argentine Peso'), ('ARM', 'Argentine Peso (1881–1970)'), ('ARP', 'Argentine Peso (1983–1985)'), ('ARL', 'Argentine Peso Ley (1970–1983)'), ('AMD', 'Armenian Dram'), ('AWG', 'Aruban Florin'), ('AUD', 'Australian Dollar'), ('ATS', 'Austrian Schilling'), ('AZN', 'Azerbaijani Manat'), ('AZM', 'Azerbaijani Manat (1993–2006)'), ('BSD', 'Bahamian Dollar'), ('BHD', 'Bahraini Dinar'), ('BDT', 'Bangladeshi Taka'), ('BBD', 'Barbadian Dollar'), ('BYN', 'Belarusian Ruble'), ('BYB', 'Belarusian Ruble (1994–1999)'), ('BYR', 'Belarusian Ruble (2000–2016)'), ('BEF', 'Belgian Franc'), ('BEC', 'Belgian Franc (convertible)'), ('BEL', 'Belgian Franc (financial)'), ('BZD', 'Belize Dollar'), ('BMD', 'Bermudan Dollar'), ('BTN', 'Bhutanese Ngultrum'), ('BOB', 'Bolivian Boliviano'), ('BOL', 'Bolivian Boliviano (1863–1963)'), ('BOV', 'Bolivian Mvdol'), ('BOP', 'Bolivian Peso'), ('BAM', 'Bosnia-Herzegovina Convertible Mark'), ('BAD', 'Bosnia-Herzegovina Dinar (1992–1994)'), ('BAN', 'Bosnia-Herzegovina New Dinar (1994–1997)'), ('BWP', 'Botswanan Pula'), ('BRC', 'Brazilian Cruzado (1986–1989)'), ('BRZ', 'Brazilian Cruzeiro (1942–1967)'), ('BRE', 'Brazilian Cruzeiro (1990–1993)'), ('BRR', 'Brazilian Cruzeiro (1993–1994)'), ('BRN', 'Brazilian New Cruzado (1989–1990)'), ('BRB', 'Brazilian New Cruzeiro (1967–1986)'), ('BRL', 'Brazilian Real'), ('GBP', 'British Pound'), ('BND', 'Brunei Dollar'), ('BGL', 'Bulgarian Hard Lev'), ('BGN', 'Bulgarian Lev'), ('BGO', 'Bulgarian Lev (1879–1952)'), ('BGM', 'Bulgarian Socialist Lev'), ('BUK', 'Burmese Kyat'), ('BIF', 'Burundian Franc'), ('XPF', 'CFP Franc'), ('KHR', 'Cambodian Riel'), ('CAD', 'Canadian Dollar'), ('CVE', 'Cape Verdean Escudo'), ('KYD', 'Cayman Islands Dollar'), ('XAF', 'Central African CFA Franc'), ('CLE', 'Chilean Escudo'), ('CLP', 'Chilean Peso'), ('CLF', 'Chilean Unit of Account (UF)'), ('CNX', 'Chinese People’s Bank Dollar'), ('CNY', 'Chinese Yuan'), ('CNH', 'Chinese Yuan (offshore)'), ('COP', 'Colombian Peso'), ('COU', 'Colombian Real Value Unit'), ('KMF', 'Comorian Franc'), ('CDF', 'Congolese Franc'), ('CRC', 'Costa Rican Colón'), ('HRD', 'Croatian Dinar'), ('HRK', 'Croatian Kuna'), ('CUC', 'Cuban Convertible Peso'), ('CUP', 'Cuban Peso'), ('CYP', 'Cypriot Pound'), ('CZK', 'Czech Koruna'), ('CSK', 'Czechoslovak Hard Koruna'), ('DKK', 'Danish Krone'), ('DJF', 'Djiboutian Franc'), ('DOP', 'Dominican Peso'), ('NLG', 'Dutch Guilder'), ('XCD', 'East Caribbean Dollar'), ('DDM', 'East German Mark'), ('ECS', 'Ecuadorian Sucre'), ('ECV', 'Ecuadorian Unit of Constant Value'), ('EGP', 'Egyptian Pound'), ('GQE', 'Equatorial Guinean Ekwele'), ('ERN', 'Eritrean Nakfa'), ('EEK', 'Estonian Kroon'), ('ETB', 'Ethiopian Birr'), ('EUR', 'Euro'), ('XBA', 'European Composite Unit'), ('XEU', 'European Currency Unit'), ('XBB', 'European Monetary Unit'), ('XBC', 'European Unit of Account (XBC)'), ('XBD', 'European Unit of Account (XBD)'), ('FKP', 'Falkland Islands Pound'), ('FJD', 'Fijian Dollar'), ('FIM', 'Finnish Markka'), ('FRF', 'French Franc'), ('XFO', 'French Gold Franc'), ('XFU', 'French UIC-Franc'), ('GMD', 'Gambian Dalasi'), ('GEK', 'Georgian Kupon Larit'), ('GEL', 'Georgian Lari'), ('DEM', 'German Mark'), ('GHS', 'Ghanaian Cedi'), ('GHC', 'Ghanaian Cedi (1979–2007)'), ('GIP', 'Gibraltar Pound'), ('XAU', 'Gold'), ('GRD', 'Greek Drachma'), ('GTQ', 'Guatemalan Quetzal'), ('GWP', 'Guinea-Bissau Peso'), ('GNF', 'Guinean Franc'), ('GNS', 'Guinean Syli'), ('GYD', 'Guyanaese Dollar'), ('HTG', 'Haitian Gourde'), ('HNL', 'Honduran Lempira'), ('HKD', 'Hong Kong Dollar'), ('HUF', 'Hungarian Forint'), ('IMP', 'IMP'), ('ISK', 'Icelandic Króna'), ('ISJ', 'Icelandic Króna (1918–1981)'), ('INR', 'Indian Rupee'), ('IDR', 'Indonesian Rupiah'), ('IRR', 'Iranian Rial'), ('IQD', 'Iraqi Dinar'), ('IEP', 'Irish Pound'), ('ILS', 'Israeli New Shekel'), ('ILP', 'Israeli Pound'), ('ILR', 'Israeli Shekel (1980–1985)'), ('ITL', 'Italian Lira'), ('JMD', 'Jamaican Dollar'), ('JPY', 'Japanese Yen'), ('JOD', 'Jordanian Dinar'), ('KZT', 'Kazakhstani Tenge'), ('KES', 'Kenyan Shilling'), ('KWD', 'Kuwaiti Dinar'), ('KGS', 'Kyrgystani Som'), ('LAK', 'Laotian Kip'), ('LVL', 'Latvian Lats'), ('LVR', 'Latvian Ruble'), ('LBP', 'Lebanese Pound'), ('LSL', 'Lesotho Loti'), ('LRD', 'Liberian Dollar'), ('LYD', 'Libyan Dinar'), ('LTL', 'Lithuanian Litas'), ('LTT', 'Lithuanian Talonas'), ('LUL', 'Luxembourg Financial Franc'), ('LUC', 'Luxembourgian Convertible Franc'), ('LUF', 'Luxembourgian Franc'), ('MOP', 'Macanese Pataca'), ('MKD', 'Macedonian Denar'), ('MKN', 'Macedonian Denar (1992–1993)'), ('MGA', 'Malagasy Ariary'), ('MGF', 'Malagasy Franc'), ('MWK', 'Malawian Kwacha'), ('MYR', 'Malaysian Ringgit'), ('MVR', 'Maldivian Rufiyaa'), ('MVP', 'Maldivian Rupee (1947–1981)'), ('MLF', 'Malian Franc'), ('MTL', 'Maltese Lira'), ('MTP', 'Maltese Pound'), ('MRU', 'Mauritanian Ouguiya'), ('MRO', 'Mauritanian Ouguiya (1973–2017)'), ('MUR', 'Mauritian Rupee'), ('MXV', 'Mexican Investment Unit'), ('MXN', 'Mexican Peso'), ('MXP', 'Mexican Silver Peso (1861–1992)'), ('MDC', 'Moldovan Cupon'), ('MDL', 'Moldovan Leu'), ('MCF', 'Monegasque Franc'), ('MNT', 'Mongolian Tugrik'), ('MAD', 'Moroccan Dirham'), ('MAF', 'Moroccan Franc'), ('MZE', 'Mozambican Escudo'), ('MZN', 'Mozambican Metical'), ('MZM', 'Mozambican Metical (1980–2006)'), ('MMK', 'Myanmar Kyat'), ('NAD', 'Namibian Dollar'), ('NPR', 'Nepalese Rupee'), ('ANG', 'Netherlands Antillean Guilder'), ('TWD', 'New Taiwan Dollar'), ('NZD', 'New Zealand Dollar'), ('NIO', 'Nicaraguan Córdoba'), ('NIC', 'Nicaraguan Córdoba (1988–1991)'), ('NGN', 'Nigerian Naira'), ('KPW', 'North Korean Won'), ('NOK', 'Norwegian Krone'), ('OMR', 'Omani Rial'), ('PKR', 'Pakistani Rupee'), ('XPD', 'Palladium'), ('PAB', 'Panamanian Balboa'), ('PGK', 'Papua New Guinean Kina'), ('PYG', 'Paraguayan Guarani'), ('PEI', 'Peruvian Inti'), ('PEN', 'Peruvian Sol'), ('PES', 'Peruvian Sol (1863–1965)'), ('PHP', 'Philippine Piso'), ('XPT', 'Platinum'), ('PLN', 'Polish Zloty'), ('PLZ', 'Polish Zloty (1950–1995)'), ('PTE', 'Portuguese Escudo'), ('GWE', 'Portuguese Guinea Escudo'), ('QAR', 'Qatari Rial'), ('XRE', 'RINET Funds'), ('RHD', 'Rhodesian Dollar'), ('RON', 'Romanian Leu'), ('ROL', 'Romanian Leu (1952–2006)'), ('RUB', 'Russian Ruble'), ('RUR', 'Russian Ruble (1991–1998)'), ('RWF', 'Rwandan Franc'), ('SVC', 'Salvadoran Colón'), ('WST', 'Samoan Tala'), ('SAR', 'Saudi Riyal'), ('RSD', 'Serbian Dinar'), ('CSD', 'Serbian Dinar (2002–2006)'), ('SCR', 'Seychellois Rupee'), ('SLL', 'Sierra Leonean Leone'), ('XAG', 'Silver'), ('SGD', 'Singapore Dollar'), ('SKK', 'Slovak Koruna'), ('SIT', 'Slovenian Tolar'), ('SBD', 'Solomon Islands Dollar'), ('SOS', 'Somali Shilling'), ('ZAR', 'South African Rand'), ('ZAL', 'South African Rand (financial)'), ('KRH', 'South Korean Hwan (1953–1962)'), ('KRW', 'South Korean Won'), ('KRO', 'South Korean Won (1945–1953)'), ('SSP', 'South Sudanese Pound'), ('SUR', 'Soviet Rouble'), ('ESP', 'Spanish Peseta'), ('ESA', 'Spanish Peseta (A account)'), ('ESB', 'Spanish Peseta (convertible account)'), ('XDR', 'Special Drawing Rights'), ('LKR', 'Sri Lankan Rupee'), ('SHP', 'St. Helena Pound'), ('XSU', 'Sucre'), ('SDD', 'Sudanese Dinar (1992–2007)'), ('SDG', 'Sudanese Pound'), ('SDP', 'Sudanese Pound (1957–1998)'), ('SRD', 'Surinamese Dollar'), ('SRG', 'Surinamese Guilder'), ('SZL', 'Swazi Lilangeni'), ('SEK', 'Swedish Krona'), ('CHF', 'Swiss Franc'), ('SYP', 'Syrian Pound'), ('STN', 'São Tomé & Príncipe Dobra'), ('STD', 'São Tomé & Príncipe Dobra (1977–2017)'), ('TVD', 'TVD'), ('TJR', 'Tajikistani Ruble'), ('TJS', 'Tajikistani Somoni'), ('TZS', 'Tanzanian Shilling'), ('XTS', 'Testing Currency Code'), ('THB', 'Thai Baht'), ('XXX', 'The codes assigned for transactions where no currency is involved'), ('TPE', 'Timorese Escudo'), ('TOP', 'Tongan Paʻanga'), ('TTD', 'Trinidad & Tobago Dollar'), ('TND', 'Tunisian Dinar'), ('TRY', 'Turkish Lira'), ('TRL', 'Turkish Lira (1922–2005)'), ('TMT', 'Turkmenistani Manat'), ('TMM', 'Turkmenistani Manat (1993–2009)'), ('USD', 'US Dollar'), ('USN', 'US Dollar (Next day)'), ('USS', 'US Dollar (Same day)'), ('UGX', 'Ugandan Shilling'), ('UGS', 'Ugandan Shilling (1966–1987)'), ('UAH', 'Ukrainian Hryvnia'), ('UAK', 'Ukrainian Karbovanets'), ('AED', 'United Arab Emirates Dirham'), ('UYW', 'Uruguayan Nominal Wage Index Unit'), ('UYU', 'Uruguayan Peso'), ('UYP', 'Uruguayan Peso (1975–1993)'), ('UYI', 'Uruguayan Peso (Indexed Units)'), ('UZS', 'Uzbekistani Som'), ('VUV', 'Vanuatu Vatu'), ('VES', 'Venezuelan Bolívar'), ('VEB', 'Venezuelan Bolívar (1871–2008)'), ('VEF', 'Venezuelan Bolívar (2008–2018)'), ('VND', 'Vietnamese Dong'), ('VNN', 'Vietnamese Dong (1978–1985)'), ('CHE', 'WIR Euro'), ('CHW', 'WIR Franc'), ('XOF', 'West African CFA Franc'), ('YDD', 'Yemeni Dinar'), ('YER', 'Yemeni Rial'), ('YUN', 'Yugoslavian Convertible Dinar (1990–1992)'), ('YUD', 'Yugoslavian Hard Dinar (1966–1990)'), ('YUM', 'Yugoslavian New Dinar (1994–2002)'), ('YUR', 'Yugoslavian Reformed Dinar (1992–1993)'), ('ZWN', 'ZWN'), ('ZRN', 'Zairean New Zaire (1993–1998)'), ('ZRZ', 'Zairean Zaire (1971–1993)'), ('ZMW', 'Zambian Kwacha'), ('ZMK', 'Zambian Kwacha (1968–2012)'), ('ZWD', 'Zimbabwean Dollar (1980–2008)'), ('ZWR', 'Zimbabwean Dollar (2008)'), ('ZWL', 'Zimbabwean Dollar (2009)')], default='USD', editable=False, max_length=3)),
+                ('amount', djmoney.models.fields.MoneyField(decimal_places=2, default_currency='USD', max_digits=14)),
+                ('created', models.DateTimeField(blank=True, editable=False)),
+                ('updated', models.DateTimeField(blank=True, editable=False)),
+                ('subscription_charge_date', models.DateTimeField()),
+                ('subscription', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.PROTECT, related_name='%(class)ss', to='subscriptions.subscription')),
+                ('user', models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, related_name='%(class)ss', to=settings.AUTH_USER_MODEL)),
+            ],
+            options={
+                'abstract': False,
+            },
+        ),
+        migrations.CreateModel(
             name='Usage',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('amount', models.PositiveIntegerField(default=1)),
-                ('datetime', models.DateTimeField(auto_now_add=True)),
+                ('datetime', models.DateTimeField(blank=True)),
                 ('resource', models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, related_name='usages', to='subscriptions.resource')),
                 ('user', models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, related_name='usages', to=settings.AUTH_USER_MODEL)),
             ],
         ),
         migrations.CreateModel(
-            name='Subscription',
+            name='Tax',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('begin', models.DateTimeField(auto_now_add=True)),
-                ('end', models.DateTimeField(blank=True)),
-                ('plan', models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, related_name='subscriptions', to='subscriptions.plan')),
-                ('user', models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, related_name='subscriptions', to=settings.AUTH_USER_MODEL)),
+                ('amount_currency', djmoney.models.fields.CurrencyField(choices=[('XUA', 'ADB Unit of Account'), ('AFN', 'Afghan Afghani'), ('AFA', 'Afghan Afghani (1927–2002)'), ('ALL', 'Albanian Lek'), ('ALK', 'Albanian Lek (1946–1965)'), ('DZD', 'Algerian Dinar'), ('ADP', 'Andorran Peseta'), ('AOA', 'Angolan Kwanza'), ('AOK', 'Angolan Kwanza (1977–1991)'), ('AON', 'Angolan New Kwanza (1990–2000)'), ('AOR', 'Angolan Readjusted Kwanza (1995–1999)'), ('ARA', 'Argentine Austral'), ('ARS', 'Argentine Peso'), ('ARM', 'Argentine Peso (1881–1970)'), ('ARP', 'Argentine Peso (1983–1985)'), ('ARL', 'Argentine Peso Ley (1970–1983)'), ('AMD', 'Armenian Dram'), ('AWG', 'Aruban Florin'), ('AUD', 'Australian Dollar'), ('ATS', 'Austrian Schilling'), ('AZN', 'Azerbaijani Manat'), ('AZM', 'Azerbaijani Manat (1993–2006)'), ('BSD', 'Bahamian Dollar'), ('BHD', 'Bahraini Dinar'), ('BDT', 'Bangladeshi Taka'), ('BBD', 'Barbadian Dollar'), ('BYN', 'Belarusian Ruble'), ('BYB', 'Belarusian Ruble (1994–1999)'), ('BYR', 'Belarusian Ruble (2000–2016)'), ('BEF', 'Belgian Franc'), ('BEC', 'Belgian Franc (convertible)'), ('BEL', 'Belgian Franc (financial)'), ('BZD', 'Belize Dollar'), ('BMD', 'Bermudan Dollar'), ('BTN', 'Bhutanese Ngultrum'), ('BOB', 'Bolivian Boliviano'), ('BOL', 'Bolivian Boliviano (1863–1963)'), ('BOV', 'Bolivian Mvdol'), ('BOP', 'Bolivian Peso'), ('BAM', 'Bosnia-Herzegovina Convertible Mark'), ('BAD', 'Bosnia-Herzegovina Dinar (1992–1994)'), ('BAN', 'Bosnia-Herzegovina New Dinar (1994–1997)'), ('BWP', 'Botswanan Pula'), ('BRC', 'Brazilian Cruzado (1986–1989)'), ('BRZ', 'Brazilian Cruzeiro (1942–1967)'), ('BRE', 'Brazilian Cruzeiro (1990–1993)'), ('BRR', 'Brazilian Cruzeiro (1993–1994)'), ('BRN', 'Brazilian New Cruzado (1989–1990)'), ('BRB', 'Brazilian New Cruzeiro (1967–1986)'), ('BRL', 'Brazilian Real'), ('GBP', 'British Pound'), ('BND', 'Brunei Dollar'), ('BGL', 'Bulgarian Hard Lev'), ('BGN', 'Bulgarian Lev'), ('BGO', 'Bulgarian Lev (1879–1952)'), ('BGM', 'Bulgarian Socialist Lev'), ('BUK', 'Burmese Kyat'), ('BIF', 'Burundian Franc'), ('XPF', 'CFP Franc'), ('KHR', 'Cambodian Riel'), ('CAD', 'Canadian Dollar'), ('CVE', 'Cape Verdean Escudo'), ('KYD', 'Cayman Islands Dollar'), ('XAF', 'Central African CFA Franc'), ('CLE', 'Chilean Escudo'), ('CLP', 'Chilean Peso'), ('CLF', 'Chilean Unit of Account (UF)'), ('CNX', 'Chinese People’s Bank Dollar'), ('CNY', 'Chinese Yuan'), ('CNH', 'Chinese Yuan (offshore)'), ('COP', 'Colombian Peso'), ('COU', 'Colombian Real Value Unit'), ('KMF', 'Comorian Franc'), ('CDF', 'Congolese Franc'), ('CRC', 'Costa Rican Colón'), ('HRD', 'Croatian Dinar'), ('HRK', 'Croatian Kuna'), ('CUC', 'Cuban Convertible Peso'), ('CUP', 'Cuban Peso'), ('CYP', 'Cypriot Pound'), ('CZK', 'Czech Koruna'), ('CSK', 'Czechoslovak Hard Koruna'), ('DKK', 'Danish Krone'), ('DJF', 'Djiboutian Franc'), ('DOP', 'Dominican Peso'), ('NLG', 'Dutch Guilder'), ('XCD', 'East Caribbean Dollar'), ('DDM', 'East German Mark'), ('ECS', 'Ecuadorian Sucre'), ('ECV', 'Ecuadorian Unit of Constant Value'), ('EGP', 'Egyptian Pound'), ('GQE', 'Equatorial Guinean Ekwele'), ('ERN', 'Eritrean Nakfa'), ('EEK', 'Estonian Kroon'), ('ETB', 'Ethiopian Birr'), ('EUR', 'Euro'), ('XBA', 'European Composite Unit'), ('XEU', 'European Currency Unit'), ('XBB', 'European Monetary Unit'), ('XBC', 'European Unit of Account (XBC)'), ('XBD', 'European Unit of Account (XBD)'), ('FKP', 'Falkland Islands Pound'), ('FJD', 'Fijian Dollar'), ('FIM', 'Finnish Markka'), ('FRF', 'French Franc'), ('XFO', 'French Gold Franc'), ('XFU', 'French UIC-Franc'), ('GMD', 'Gambian Dalasi'), ('GEK', 'Georgian Kupon Larit'), ('GEL', 'Georgian Lari'), ('DEM', 'German Mark'), ('GHS', 'Ghanaian Cedi'), ('GHC', 'Ghanaian Cedi (1979–2007)'), ('GIP', 'Gibraltar Pound'), ('XAU', 'Gold'), ('GRD', 'Greek Drachma'), ('GTQ', 'Guatemalan Quetzal'), ('GWP', 'Guinea-Bissau Peso'), ('GNF', 'Guinean Franc'), ('GNS', 'Guinean Syli'), ('GYD', 'Guyanaese Dollar'), ('HTG', 'Haitian Gourde'), ('HNL', 'Honduran Lempira'), ('HKD', 'Hong Kong Dollar'), ('HUF', 'Hungarian Forint'), ('IMP', 'IMP'), ('ISK', 'Icelandic Króna'), ('ISJ', 'Icelandic Króna (1918–1981)'), ('INR', 'Indian Rupee'), ('IDR', 'Indonesian Rupiah'), ('IRR', 'Iranian Rial'), ('IQD', 'Iraqi Dinar'), ('IEP', 'Irish Pound'), ('ILS', 'Israeli New Shekel'), ('ILP', 'Israeli Pound'), ('ILR', 'Israeli Shekel (1980–1985)'), ('ITL', 'Italian Lira'), ('JMD', 'Jamaican Dollar'), ('JPY', 'Japanese Yen'), ('JOD', 'Jordanian Dinar'), ('KZT', 'Kazakhstani Tenge'), ('KES', 'Kenyan Shilling'), ('KWD', 'Kuwaiti Dinar'), ('KGS', 'Kyrgystani Som'), ('LAK', 'Laotian Kip'), ('LVL', 'Latvian Lats'), ('LVR', 'Latvian Ruble'), ('LBP', 'Lebanese Pound'), ('LSL', 'Lesotho Loti'), ('LRD', 'Liberian Dollar'), ('LYD', 'Libyan Dinar'), ('LTL', 'Lithuanian Litas'), ('LTT', 'Lithuanian Talonas'), ('LUL', 'Luxembourg Financial Franc'), ('LUC', 'Luxembourgian Convertible Franc'), ('LUF', 'Luxembourgian Franc'), ('MOP', 'Macanese Pataca'), ('MKD', 'Macedonian Denar'), ('MKN', 'Macedonian Denar (1992–1993)'), ('MGA', 'Malagasy Ariary'), ('MGF', 'Malagasy Franc'), ('MWK', 'Malawian Kwacha'), ('MYR', 'Malaysian Ringgit'), ('MVR', 'Maldivian Rufiyaa'), ('MVP', 'Maldivian Rupee (1947–1981)'), ('MLF', 'Malian Franc'), ('MTL', 'Maltese Lira'), ('MTP', 'Maltese Pound'), ('MRU', 'Mauritanian Ouguiya'), ('MRO', 'Mauritanian Ouguiya (1973–2017)'), ('MUR', 'Mauritian Rupee'), ('MXV', 'Mexican Investment Unit'), ('MXN', 'Mexican Peso'), ('MXP', 'Mexican Silver Peso (1861–1992)'), ('MDC', 'Moldovan Cupon'), ('MDL', 'Moldovan Leu'), ('MCF', 'Monegasque Franc'), ('MNT', 'Mongolian Tugrik'), ('MAD', 'Moroccan Dirham'), ('MAF', 'Moroccan Franc'), ('MZE', 'Mozambican Escudo'), ('MZN', 'Mozambican Metical'), ('MZM', 'Mozambican Metical (1980–2006)'), ('MMK', 'Myanmar Kyat'), ('NAD', 'Namibian Dollar'), ('NPR', 'Nepalese Rupee'), ('ANG', 'Netherlands Antillean Guilder'), ('TWD', 'New Taiwan Dollar'), ('NZD', 'New Zealand Dollar'), ('NIO', 'Nicaraguan Córdoba'), ('NIC', 'Nicaraguan Córdoba (1988–1991)'), ('NGN', 'Nigerian Naira'), ('KPW', 'North Korean Won'), ('NOK', 'Norwegian Krone'), ('OMR', 'Omani Rial'), ('PKR', 'Pakistani Rupee'), ('XPD', 'Palladium'), ('PAB', 'Panamanian Balboa'), ('PGK', 'Papua New Guinean Kina'), ('PYG', 'Paraguayan Guarani'), ('PEI', 'Peruvian Inti'), ('PEN', 'Peruvian Sol'), ('PES', 'Peruvian Sol (1863–1965)'), ('PHP', 'Philippine Piso'), ('XPT', 'Platinum'), ('PLN', 'Polish Zloty'), ('PLZ', 'Polish Zloty (1950–1995)'), ('PTE', 'Portuguese Escudo'), ('GWE', 'Portuguese Guinea Escudo'), ('QAR', 'Qatari Rial'), ('XRE', 'RINET Funds'), ('RHD', 'Rhodesian Dollar'), ('RON', 'Romanian Leu'), ('ROL', 'Romanian Leu (1952–2006)'), ('RUB', 'Russian Ruble'), ('RUR', 'Russian Ruble (1991–1998)'), ('RWF', 'Rwandan Franc'), ('SVC', 'Salvadoran Colón'), ('WST', 'Samoan Tala'), ('SAR', 'Saudi Riyal'), ('RSD', 'Serbian Dinar'), ('CSD', 'Serbian Dinar (2002–2006)'), ('SCR', 'Seychellois Rupee'), ('SLL', 'Sierra Leonean Leone'), ('XAG', 'Silver'), ('SGD', 'Singapore Dollar'), ('SKK', 'Slovak Koruna'), ('SIT', 'Slovenian Tolar'), ('SBD', 'Solomon Islands Dollar'), ('SOS', 'Somali Shilling'), ('ZAR', 'South African Rand'), ('ZAL', 'South African Rand (financial)'), ('KRH', 'South Korean Hwan (1953–1962)'), ('KRW', 'South Korean Won'), ('KRO', 'South Korean Won (1945–1953)'), ('SSP', 'South Sudanese Pound'), ('SUR', 'Soviet Rouble'), ('ESP', 'Spanish Peseta'), ('ESA', 'Spanish Peseta (A account)'), ('ESB', 'Spanish Peseta (convertible account)'), ('XDR', 'Special Drawing Rights'), ('LKR', 'Sri Lankan Rupee'), ('SHP', 'St. Helena Pound'), ('XSU', 'Sucre'), ('SDD', 'Sudanese Dinar (1992–2007)'), ('SDG', 'Sudanese Pound'), ('SDP', 'Sudanese Pound (1957–1998)'), ('SRD', 'Surinamese Dollar'), ('SRG', 'Surinamese Guilder'), ('SZL', 'Swazi Lilangeni'), ('SEK', 'Swedish Krona'), ('CHF', 'Swiss Franc'), ('SYP', 'Syrian Pound'), ('STN', 'São Tomé & Príncipe Dobra'), ('STD', 'São Tomé & Príncipe Dobra (1977–2017)'), ('TVD', 'TVD'), ('TJR', 'Tajikistani Ruble'), ('TJS', 'Tajikistani Somoni'), ('TZS', 'Tanzanian Shilling'), ('XTS', 'Testing Currency Code'), ('THB', 'Thai Baht'), ('XXX', 'The codes assigned for transactions where no currency is involved'), ('TPE', 'Timorese Escudo'), ('TOP', 'Tongan Paʻanga'), ('TTD', 'Trinidad & Tobago Dollar'), ('TND', 'Tunisian Dinar'), ('TRY', 'Turkish Lira'), ('TRL', 'Turkish Lira (1922–2005)'), ('TMT', 'Turkmenistani Manat'), ('TMM', 'Turkmenistani Manat (1993–2009)'), ('USD', 'US Dollar'), ('USN', 'US Dollar (Next day)'), ('USS', 'US Dollar (Same day)'), ('UGX', 'Ugandan Shilling'), ('UGS', 'Ugandan Shilling (1966–1987)'), ('UAH', 'Ukrainian Hryvnia'), ('UAK', 'Ukrainian Karbovanets'), ('AED', 'United Arab Emirates Dirham'), ('UYW', 'Uruguayan Nominal Wage Index Unit'), ('UYU', 'Uruguayan Peso'), ('UYP', 'Uruguayan Peso (1975–1993)'), ('UYI', 'Uruguayan Peso (Indexed Units)'), ('UZS', 'Uzbekistani Som'), ('VUV', 'Vanuatu Vatu'), ('VES', 'Venezuelan Bolívar'), ('VEB', 'Venezuelan Bolívar (1871–2008)'), ('VEF', 'Venezuelan Bolívar (2008–2018)'), ('VND', 'Vietnamese Dong'), ('VNN', 'Vietnamese Dong (1978–1985)'), ('CHE', 'WIR Euro'), ('CHW', 'WIR Franc'), ('XOF', 'West African CFA Franc'), ('YDD', 'Yemeni Dinar'), ('YER', 'Yemeni Rial'), ('YUN', 'Yugoslavian Convertible Dinar (1990–1992)'), ('YUD', 'Yugoslavian Hard Dinar (1966–1990)'), ('YUM', 'Yugoslavian New Dinar (1994–2002)'), ('YUR', 'Yugoslavian Reformed Dinar (1992–1993)'), ('ZWN', 'ZWN'), ('ZRN', 'Zairean New Zaire (1993–1998)'), ('ZRZ', 'Zairean Zaire (1971–1993)'), ('ZMW', 'Zambian Kwacha'), ('ZMK', 'Zambian Kwacha (1968–2012)'), ('ZWD', 'Zimbabwean Dollar (1980–2008)'), ('ZWR', 'Zimbabwean Dollar (2008)'), ('ZWL', 'Zimbabwean Dollar (2009)')], default='USD', editable=False, max_length=3)),
+                ('amount', djmoney.models.fields.MoneyField(decimal_places=2, default_currency='USD', max_digits=14)),
+                ('subscription_payment', models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, related_name='taxes', to='subscriptions.subscriptionpayment')),
             ],
         ),
+        migrations.CreateModel(
+            name='SubscriptionPaymentRefund',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('provider_codename', models.CharField(max_length=255)),
+                ('provider_transaction_id', models.CharField(max_length=255)),
+                ('status', models.PositiveSmallIntegerField(choices=[(0, 'Pending'), (1, 'Preauth'), (2, 'Completed'), (3, 'Canceled'), (4, 'Error')], default=0)),
+                ('amount_currency', djmoney.models.fields.CurrencyField(choices=[('XUA', 'ADB Unit of Account'), ('AFN', 'Afghan Afghani'), ('AFA', 'Afghan Afghani (1927–2002)'), ('ALL', 'Albanian Lek'), ('ALK', 'Albanian Lek (1946–1965)'), ('DZD', 'Algerian Dinar'), ('ADP', 'Andorran Peseta'), ('AOA', 'Angolan Kwanza'), ('AOK', 'Angolan Kwanza (1977–1991)'), ('AON', 'Angolan New Kwanza (1990–2000)'), ('AOR', 'Angolan Readjusted Kwanza (1995–1999)'), ('ARA', 'Argentine Austral'), ('ARS', 'Argentine Peso'), ('ARM', 'Argentine Peso (1881–1970)'), ('ARP', 'Argentine Peso (1983–1985)'), ('ARL', 'Argentine Peso Ley (1970–1983)'), ('AMD', 'Armenian Dram'), ('AWG', 'Aruban Florin'), ('AUD', 'Australian Dollar'), ('ATS', 'Austrian Schilling'), ('AZN', 'Azerbaijani Manat'), ('AZM', 'Azerbaijani Manat (1993–2006)'), ('BSD', 'Bahamian Dollar'), ('BHD', 'Bahraini Dinar'), ('BDT', 'Bangladeshi Taka'), ('BBD', 'Barbadian Dollar'), ('BYN', 'Belarusian Ruble'), ('BYB', 'Belarusian Ruble (1994–1999)'), ('BYR', 'Belarusian Ruble (2000–2016)'), ('BEF', 'Belgian Franc'), ('BEC', 'Belgian Franc (convertible)'), ('BEL', 'Belgian Franc (financial)'), ('BZD', 'Belize Dollar'), ('BMD', 'Bermudan Dollar'), ('BTN', 'Bhutanese Ngultrum'), ('BOB', 'Bolivian Boliviano'), ('BOL', 'Bolivian Boliviano (1863–1963)'), ('BOV', 'Bolivian Mvdol'), ('BOP', 'Bolivian Peso'), ('BAM', 'Bosnia-Herzegovina Convertible Mark'), ('BAD', 'Bosnia-Herzegovina Dinar (1992–1994)'), ('BAN', 'Bosnia-Herzegovina New Dinar (1994–1997)'), ('BWP', 'Botswanan Pula'), ('BRC', 'Brazilian Cruzado (1986–1989)'), ('BRZ', 'Brazilian Cruzeiro (1942–1967)'), ('BRE', 'Brazilian Cruzeiro (1990–1993)'), ('BRR', 'Brazilian Cruzeiro (1993–1994)'), ('BRN', 'Brazilian New Cruzado (1989–1990)'), ('BRB', 'Brazilian New Cruzeiro (1967–1986)'), ('BRL', 'Brazilian Real'), ('GBP', 'British Pound'), ('BND', 'Brunei Dollar'), ('BGL', 'Bulgarian Hard Lev'), ('BGN', 'Bulgarian Lev'), ('BGO', 'Bulgarian Lev (1879–1952)'), ('BGM', 'Bulgarian Socialist Lev'), ('BUK', 'Burmese Kyat'), ('BIF', 'Burundian Franc'), ('XPF', 'CFP Franc'), ('KHR', 'Cambodian Riel'), ('CAD', 'Canadian Dollar'), ('CVE', 'Cape Verdean Escudo'), ('KYD', 'Cayman Islands Dollar'), ('XAF', 'Central African CFA Franc'), ('CLE', 'Chilean Escudo'), ('CLP', 'Chilean Peso'), ('CLF', 'Chilean Unit of Account (UF)'), ('CNX', 'Chinese People’s Bank Dollar'), ('CNY', 'Chinese Yuan'), ('CNH', 'Chinese Yuan (offshore)'), ('COP', 'Colombian Peso'), ('COU', 'Colombian Real Value Unit'), ('KMF', 'Comorian Franc'), ('CDF', 'Congolese Franc'), ('CRC', 'Costa Rican Colón'), ('HRD', 'Croatian Dinar'), ('HRK', 'Croatian Kuna'), ('CUC', 'Cuban Convertible Peso'), ('CUP', 'Cuban Peso'), ('CYP', 'Cypriot Pound'), ('CZK', 'Czech Koruna'), ('CSK', 'Czechoslovak Hard Koruna'), ('DKK', 'Danish Krone'), ('DJF', 'Djiboutian Franc'), ('DOP', 'Dominican Peso'), ('NLG', 'Dutch Guilder'), ('XCD', 'East Caribbean Dollar'), ('DDM', 'East German Mark'), ('ECS', 'Ecuadorian Sucre'), ('ECV', 'Ecuadorian Unit of Constant Value'), ('EGP', 'Egyptian Pound'), ('GQE', 'Equatorial Guinean Ekwele'), ('ERN', 'Eritrean Nakfa'), ('EEK', 'Estonian Kroon'), ('ETB', 'Ethiopian Birr'), ('EUR', 'Euro'), ('XBA', 'European Composite Unit'), ('XEU', 'European Currency Unit'), ('XBB', 'European Monetary Unit'), ('XBC', 'European Unit of Account (XBC)'), ('XBD', 'European Unit of Account (XBD)'), ('FKP', 'Falkland Islands Pound'), ('FJD', 'Fijian Dollar'), ('FIM', 'Finnish Markka'), ('FRF', 'French Franc'), ('XFO', 'French Gold Franc'), ('XFU', 'French UIC-Franc'), ('GMD', 'Gambian Dalasi'), ('GEK', 'Georgian Kupon Larit'), ('GEL', 'Georgian Lari'), ('DEM', 'German Mark'), ('GHS', 'Ghanaian Cedi'), ('GHC', 'Ghanaian Cedi (1979–2007)'), ('GIP', 'Gibraltar Pound'), ('XAU', 'Gold'), ('GRD', 'Greek Drachma'), ('GTQ', 'Guatemalan Quetzal'), ('GWP', 'Guinea-Bissau Peso'), ('GNF', 'Guinean Franc'), ('GNS', 'Guinean Syli'), ('GYD', 'Guyanaese Dollar'), ('HTG', 'Haitian Gourde'), ('HNL', 'Honduran Lempira'), ('HKD', 'Hong Kong Dollar'), ('HUF', 'Hungarian Forint'), ('IMP', 'IMP'), ('ISK', 'Icelandic Króna'), ('ISJ', 'Icelandic Króna (1918–1981)'), ('INR', 'Indian Rupee'), ('IDR', 'Indonesian Rupiah'), ('IRR', 'Iranian Rial'), ('IQD', 'Iraqi Dinar'), ('IEP', 'Irish Pound'), ('ILS', 'Israeli New Shekel'), ('ILP', 'Israeli Pound'), ('ILR', 'Israeli Shekel (1980–1985)'), ('ITL', 'Italian Lira'), ('JMD', 'Jamaican Dollar'), ('JPY', 'Japanese Yen'), ('JOD', 'Jordanian Dinar'), ('KZT', 'Kazakhstani Tenge'), ('KES', 'Kenyan Shilling'), ('KWD', 'Kuwaiti Dinar'), ('KGS', 'Kyrgystani Som'), ('LAK', 'Laotian Kip'), ('LVL', 'Latvian Lats'), ('LVR', 'Latvian Ruble'), ('LBP', 'Lebanese Pound'), ('LSL', 'Lesotho Loti'), ('LRD', 'Liberian Dollar'), ('LYD', 'Libyan Dinar'), ('LTL', 'Lithuanian Litas'), ('LTT', 'Lithuanian Talonas'), ('LUL', 'Luxembourg Financial Franc'), ('LUC', 'Luxembourgian Convertible Franc'), ('LUF', 'Luxembourgian Franc'), ('MOP', 'Macanese Pataca'), ('MKD', 'Macedonian Denar'), ('MKN', 'Macedonian Denar (1992–1993)'), ('MGA', 'Malagasy Ariary'), ('MGF', 'Malagasy Franc'), ('MWK', 'Malawian Kwacha'), ('MYR', 'Malaysian Ringgit'), ('MVR', 'Maldivian Rufiyaa'), ('MVP', 'Maldivian Rupee (1947–1981)'), ('MLF', 'Malian Franc'), ('MTL', 'Maltese Lira'), ('MTP', 'Maltese Pound'), ('MRU', 'Mauritanian Ouguiya'), ('MRO', 'Mauritanian Ouguiya (1973–2017)'), ('MUR', 'Mauritian Rupee'), ('MXV', 'Mexican Investment Unit'), ('MXN', 'Mexican Peso'), ('MXP', 'Mexican Silver Peso (1861–1992)'), ('MDC', 'Moldovan Cupon'), ('MDL', 'Moldovan Leu'), ('MCF', 'Monegasque Franc'), ('MNT', 'Mongolian Tugrik'), ('MAD', 'Moroccan Dirham'), ('MAF', 'Moroccan Franc'), ('MZE', 'Mozambican Escudo'), ('MZN', 'Mozambican Metical'), ('MZM', 'Mozambican Metical (1980–2006)'), ('MMK', 'Myanmar Kyat'), ('NAD', 'Namibian Dollar'), ('NPR', 'Nepalese Rupee'), ('ANG', 'Netherlands Antillean Guilder'), ('TWD', 'New Taiwan Dollar'), ('NZD', 'New Zealand Dollar'), ('NIO', 'Nicaraguan Córdoba'), ('NIC', 'Nicaraguan Córdoba (1988–1991)'), ('NGN', 'Nigerian Naira'), ('KPW', 'North Korean Won'), ('NOK', 'Norwegian Krone'), ('OMR', 'Omani Rial'), ('PKR', 'Pakistani Rupee'), ('XPD', 'Palladium'), ('PAB', 'Panamanian Balboa'), ('PGK', 'Papua New Guinean Kina'), ('PYG', 'Paraguayan Guarani'), ('PEI', 'Peruvian Inti'), ('PEN', 'Peruvian Sol'), ('PES', 'Peruvian Sol (1863–1965)'), ('PHP', 'Philippine Piso'), ('XPT', 'Platinum'), ('PLN', 'Polish Zloty'), ('PLZ', 'Polish Zloty (1950–1995)'), ('PTE', 'Portuguese Escudo'), ('GWE', 'Portuguese Guinea Escudo'), ('QAR', 'Qatari Rial'), ('XRE', 'RINET Funds'), ('RHD', 'Rhodesian Dollar'), ('RON', 'Romanian Leu'), ('ROL', 'Romanian Leu (1952–2006)'), ('RUB', 'Russian Ruble'), ('RUR', 'Russian Ruble (1991–1998)'), ('RWF', 'Rwandan Franc'), ('SVC', 'Salvadoran Colón'), ('WST', 'Samoan Tala'), ('SAR', 'Saudi Riyal'), ('RSD', 'Serbian Dinar'), ('CSD', 'Serbian Dinar (2002–2006)'), ('SCR', 'Seychellois Rupee'), ('SLL', 'Sierra Leonean Leone'), ('XAG', 'Silver'), ('SGD', 'Singapore Dollar'), ('SKK', 'Slovak Koruna'), ('SIT', 'Slovenian Tolar'), ('SBD', 'Solomon Islands Dollar'), ('SOS', 'Somali Shilling'), ('ZAR', 'South African Rand'), ('ZAL', 'South African Rand (financial)'), ('KRH', 'South Korean Hwan (1953–1962)'), ('KRW', 'South Korean Won'), ('KRO', 'South Korean Won (1945–1953)'), ('SSP', 'South Sudanese Pound'), ('SUR', 'Soviet Rouble'), ('ESP', 'Spanish Peseta'), ('ESA', 'Spanish Peseta (A account)'), ('ESB', 'Spanish Peseta (convertible account)'), ('XDR', 'Special Drawing Rights'), ('LKR', 'Sri Lankan Rupee'), ('SHP', 'St. Helena Pound'), ('XSU', 'Sucre'), ('SDD', 'Sudanese Dinar (1992–2007)'), ('SDG', 'Sudanese Pound'), ('SDP', 'Sudanese Pound (1957–1998)'), ('SRD', 'Surinamese Dollar'), ('SRG', 'Surinamese Guilder'), ('SZL', 'Swazi Lilangeni'), ('SEK', 'Swedish Krona'), ('CHF', 'Swiss Franc'), ('SYP', 'Syrian Pound'), ('STN', 'São Tomé & Príncipe Dobra'), ('STD', 'São Tomé & Príncipe Dobra (1977–2017)'), ('TVD', 'TVD'), ('TJR', 'Tajikistani Ruble'), ('TJS', 'Tajikistani Somoni'), ('TZS', 'Tanzanian Shilling'), ('XTS', 'Testing Currency Code'), ('THB', 'Thai Baht'), ('XXX', 'The codes assigned for transactions where no currency is involved'), ('TPE', 'Timorese Escudo'), ('TOP', 'Tongan Paʻanga'), ('TTD', 'Trinidad & Tobago Dollar'), ('TND', 'Tunisian Dinar'), ('TRY', 'Turkish Lira'), ('TRL', 'Turkish Lira (1922–2005)'), ('TMT', 'Turkmenistani Manat'), ('TMM', 'Turkmenistani Manat (1993–2009)'), ('USD', 'US Dollar'), ('USN', 'US Dollar (Next day)'), ('USS', 'US Dollar (Same day)'), ('UGX', 'Ugandan Shilling'), ('UGS', 'Ugandan Shilling (1966–1987)'), ('UAH', 'Ukrainian Hryvnia'), ('UAK', 'Ukrainian Karbovanets'), ('AED', 'United Arab Emirates Dirham'), ('UYW', 'Uruguayan Nominal Wage Index Unit'), ('UYU', 'Uruguayan Peso'), ('UYP', 'Uruguayan Peso (1975–1993)'), ('UYI', 'Uruguayan Peso (Indexed Units)'), ('UZS', 'Uzbekistani Som'), ('VUV', 'Vanuatu Vatu'), ('VES', 'Venezuelan Bolívar'), ('VEB', 'Venezuelan Bolívar (1871–2008)'), ('VEF', 'Venezuelan Bolívar (2008–2018)'), ('VND', 'Vietnamese Dong'), ('VNN', 'Vietnamese Dong (1978–1985)'), ('CHE', 'WIR Euro'), ('CHW', 'WIR Franc'), ('XOF', 'West African CFA Franc'), ('YDD', 'Yemeni Dinar'), ('YER', 'Yemeni Rial'), ('YUN', 'Yugoslavian Convertible Dinar (1990–1992)'), ('YUD', 'Yugoslavian Hard Dinar (1966–1990)'), ('YUM', 'Yugoslavian New Dinar (1994–2002)'), ('YUR', 'Yugoslavian Reformed Dinar (1992–1993)'), ('ZWN', 'ZWN'), ('ZRN', 'Zairean New Zaire (1993–1998)'), ('ZRZ', 'Zairean Zaire (1971–1993)'), ('ZMW', 'Zambian Kwacha'), ('ZMK', 'Zambian Kwacha (1968–2012)'), ('ZWD', 'Zimbabwean Dollar (1980–2008)'), ('ZWR', 'Zimbabwean Dollar (2008)'), ('ZWL', 'Zimbabwean Dollar (2009)')], default='USD', editable=False, max_length=3)),
+                ('amount', djmoney.models.fields.MoneyField(decimal_places=2, default_currency='USD', max_digits=14)),
+                ('created', models.DateTimeField(blank=True, editable=False)),
+                ('updated', models.DateTimeField(blank=True, editable=False)),
+                ('original_payment', models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, related_name='refunds', to='subscriptions.subscriptionpayment')),
+            ],
+            options={
+                'abstract': False,
+            },
+        ),
         migrations.AddConstraint(
             model_name='resource',
             constraint=models.UniqueConstraint(fields=('codename',), name='unique_resource'),
         ),
         migrations.AddField(
             model_name='quota',
             name='plan',
@@ -77,18 +124,22 @@
         migrations.AddField(
             model_name='quota',
             name='resource',
             field=models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='quotas', to='subscriptions.resource'),
         ),
         migrations.AddConstraint(
             model_name='plan',
-            constraint=models.UniqueConstraint(fields=('codename',), name='unique_plan'),
+            constraint=models.UniqueConstraint(fields=('codename',), name='unique_plan_codename'),
+        ),
+        migrations.AddConstraint(
+            model_name='plan',
+            constraint=models.UniqueConstraint(fields=('slug',), name='unique_plan_slug'),
         ),
         migrations.AddIndex(
             model_name='usage',
-            index=models.Index(fields=['user', 'resource'], name='subscriptions_us_user_id_40fe43_idx'),
+            index=models.Index(fields=['user', 'resource'], name='subscriptio_user_id_37f524_idx'),
         ),
         migrations.AddConstraint(
             model_name='quota',
             constraint=models.UniqueConstraint(fields=('plan', 'resource'), name='unique_quota'),
         ),
     ]
```

## subscriptions/providers/__init__.py

```diff
@@ -1,52 +1,93 @@
-from abc import ABC, abstractmethod
+from dataclasses import dataclass
+from datetime import datetime
 from functools import lru_cache
 from logging import getLogger
-from typing import Optional
+from typing import ClassVar, Iterable, List, Optional, Tuple
 
 from django.conf import settings
+from django.contrib.auth.models import AbstractBaseUser
 from django.forms import Form
-from django.http import HttpRequest
 from django.utils.module_loading import import_string
+from djmoney.money import Money
+from more_itertools import first, one
+from pydantic import BaseModel
 from rest_framework.request import Request
 from rest_framework.response import Response
 
+from ..defaults import DEFAULT_SUBSCRIPTIONS_PAYMENT_PROVIDERS
 from ..exceptions import ProviderNotFound
-from ..models import Plan, SubscriptionPayment
+from ..models import Plan, Subscription, SubscriptionPayment
 
 log = getLogger(__name__)
 
 
-class Provider(ABC):
-    name: Optional[str] = None
-    form: Optional[Form] = None
-    redirect_url: Optional[str] = None
-
-    def __init__(self, **kwargs):
-        for k, v in kwargs.items():
-            setattr(self, k, v)
-
-    @abstractmethod
-    def process_payment(self, form_data: dict, request: Optional[HttpRequest], plan: Plan) -> SubscriptionPayment:
-        ...
-
-    def handle_webhook(self, request: Request) -> Response:
-        log.warning(f'Webhook for "{self.name}" triggered without explicit handler')
-        return Response({})
+@dataclass
+class Provider:
+    codename: ClassVar[str]
+    is_external: ClassVar[bool]
+    is_enabled: ClassVar[bool] = True
+    form: ClassVar[Optional[Form]] = None
+    metadata_class: ClassVar[BaseModel] = BaseModel
+
+    def get_amount(self, user: AbstractBaseUser, plan: Plan) -> Money:
+        return plan.charge_amount
+
+    def charge_online(
+        self,
+        user: AbstractBaseUser,
+        plan: Plan,
+        subscription: Optional[Subscription] = None,
+        amount: Optional[Money] = None,
+        quantity: int = 1,
+        subscription_start: Optional[datetime] = None,
+        subscription_end: Optional[datetime] = None,
+    ) -> Tuple[SubscriptionPayment, str]:
+        raise NotImplementedError()
+
+    def charge_offline(
+        self,
+        user: AbstractBaseUser,
+        plan: Plan,
+        subscription: Optional[Subscription] = None,
+        amount: Optional[Money] = None,
+        quantity: int = 1,
+        reference_payment: Optional[SubscriptionPayment] = None,
+    ) -> SubscriptionPayment:
+        raise NotImplementedError()
+
+    def webhook(self, request: Request, payload: dict) -> Response:
+        log.warning(f'Webhook for "{self.codename}" triggered without explicit handler')
+        return Response(payload)
+
+    def check_payments(self, payments: Iterable[SubscriptionPayment]):
+        raise NotImplementedError()
 
 
 @lru_cache
-def get_provider(provider_name: str) -> Provider:
-    try:
-        info = settings.PAYMENT_PROVIDERS[provider_name]
-    except KeyError as exc:
-        raise ProviderNotFound(f'Provider "{provider_name}" not found in settings.PAYMENT_PROVIDERS') from exc
+def get_providers() -> List[Provider]:
+    providers = []
+    seen_codenames = set()
+
+    payment_providers = getattr(settings, 'SUBSCRIPTIONS_PAYMENT_PROVIDERS', DEFAULT_SUBSCRIPTIONS_PAYMENT_PROVIDERS)
+
+    for class_path in payment_providers:
+        provider = import_string(class_path)()
+        assert provider.codename not in seen_codenames, f'Duplicate codename "{provider.codename}"'
+        providers.append(provider)
+        seen_codenames.add(provider.codename)
+
+    return providers
+
+
+@lru_cache
+def get_provider(codename: Optional[str] = None) -> Provider:
+    if not (providers := get_providers()):
+        raise ProviderNotFound('No providers defined')
+
+    if not codename:
+        return first(providers)
 
     try:
-        class_ = import_string(info['class'])
-    except ImportError as exc:
-        raise ProviderNotFound(f'Provider "{provider_name}" not found: cannot import module "{info["class"]}"') from exc
-
-    kwargs = {k: v for k, v in info.items() if k != 'class'}
-    assert 'name' not in kwargs
-    kwargs['name'] = provider_name
-    return class_(**kwargs)
+        return one(provider for provider in providers if provider.codename == codename)
+    except (ValueError, IndexError) as exc:
+        raise ProviderNotFound(f'Provider with codename "{codename}" not found') from exc
```

## subscriptions/providers/dummy/__init__.py

```diff
@@ -1,37 +1,144 @@
-from uuid import uuid4
-
-from django.db import transaction
-from django.http import HttpRequest
-from django.utils.timezone import now
+from dataclasses import dataclass
+from datetime import datetime
+from typing import ClassVar, Iterable, Optional, Tuple
+
+from django.contrib.auth.models import AbstractBaseUser
+from django.forms import Form
+from django.utils.crypto import get_random_string
+from djmoney.money import Money
 from rest_framework.request import Request
 from rest_framework.response import Response
+from rest_framework.status import HTTP_200_OK, HTTP_404_NOT_FOUND, HTTP_400_BAD_REQUEST
 
+from ...exceptions import PaymentError
 from ...models import Plan, Subscription, SubscriptionPayment
 from .. import Provider
 from .forms import DummyForm
 
 
+@dataclass  # TODO: not needed?
 class DummyProvider(Provider):
-    form = DummyForm
+    codename: ClassVar[str] = 'dummy'
+    form: ClassVar[Form] = DummyForm
 
-    @transaction.atomic
-    def process_payment(self, form_data: dict, request: HttpRequest, plan: Plan) -> SubscriptionPayment:
+    _payment_url: ClassVar[str] = '/payment/{}/'
 
-        subscription = Subscription.objects.create(
-            user=request.user,
+    def charge_online(
+        self,
+        user: AbstractBaseUser,
+        plan: Plan,
+        subscription: Optional[Subscription] = None,
+        amount: Optional[Money] = None,
+        quantity: int = 1,
+        subscription_start: Optional[datetime] = None,
+        subscription_end: Optional[datetime] = None,
+    ) -> Tuple[SubscriptionPayment, str]:
+
+        transaction_id = get_random_string(8)
+        if amount is None:
+            amount = self.get_amount(user=user, plan=plan)
+
+        payment = SubscriptionPayment.objects.create(  # TODO: limit number of creations per day
+            provider_codename=self.codename,
+            provider_transaction_id=transaction_id,
+            amount=amount,
+            quantity=quantity,
+            user=user,
             plan=plan,
-            start=now(),
+            subscription=subscription,
+            subscription_start=subscription_start,
+            subscription_end=subscription_end,
         )
+        return payment, self._payment_url.format(transaction_id)
 
-        return SubscriptionPayment.objects.create(
-            provider_name=self.name,
-            provider_transaction_id=uuid4(),
+    def charge_offline(
+        self,
+        user: AbstractBaseUser,
+        plan: Plan, subscription: Optional[Subscription] = None,
+        amount: Optional[Money] = None,
+        quantity: int = 1,
+        reference_payment: Optional[SubscriptionPayment] = None,
+    ) -> SubscriptionPayment:
+
+        if not user.payments.filter(
+            provider_codename=self.codename,
             status=SubscriptionPayment.Status.COMPLETED,
-            amount=plan.charge_amount or 0,
-            user=request.user,
+        ).exists():
+            raise PaymentError('Cannot offline-charge without previous successful charge')
+
+        if amount is None:
+            amount = self.get_amount(user=user, plan=plan)
+
+        return SubscriptionPayment.objects.create(  # TODO: limit number of creations per day
+            provider_codename=self.codename,
+            provider_transaction_id=get_random_string(8),
+            amount=self.get_amount(user=user, plan=plan),
+            quantity=quantity,
+            user=user,
+            plan=plan,
             subscription=subscription,
-            subscription_charge_date=subscription.start,
+            status=SubscriptionPayment.Status.COMPLETED,
         )
 
-    def handle_webhook(self, request: Request) -> Response:
-        return Response(request.data)
+    def webhook(self, request: Request, payload: dict) -> Response:
+        if not (transaction_id := payload.get('transaction_id')):
+            return Response(status=HTTP_400_BAD_REQUEST)
+
+        try:
+            payment = SubscriptionPayment.objects.get(provider_transaction_id=transaction_id)
+        except SubscriptionPayment.DoesNotExist:
+            return Response(status=HTTP_404_NOT_FOUND)
+
+        if payment.status != payment.Status.PENDING:
+            return Response(status=HTTP_400_BAD_REQUEST)
+
+        payment.status = SubscriptionPayment.Status.COMPLETED
+        payment.save()
+        return Response(status=HTTP_200_OK)
+
+    def check_payments(self, payments: Iterable[SubscriptionPayment]):
+        pass
+
+    # TODO: what to do with this?
+    # @transaction.atomic
+    # def process_subscription_request(self, request: HttpRequest, serializer: PaymentSerializer) -> Response:
+    #     plan = serializer.validated_data['plan']
+
+    #     now_ = now()
+    #     subscription = request.user.subscriptions.active().filter(plan=plan).order_by('-end').last()
+    #     if created := not bool(subscription):
+    #         if not plan.is_enabled:
+    #             raise PermissionDenied(detail='Cannot register new subscription because the plan is disabled')
+
+    #         subscription = Subscription.objects.create(
+    #             user=request.user,
+    #             plan=plan,
+    #             start=now_,
+    #         )
+
+    #     try:
+    #         charge_date = next(subscription.iter_charge_dates(since=now_))
+    #     except StopIteration as exc:
+    #         raise PermissionDenied(detail='No ongoing charge dates found') from exc
+
+    #     SubscriptionPayment.objects.create(
+    #         provider_codename=self.codename,
+    #         provider_transaction_id=uuid4(),
+    #         status=SubscriptionPayment.Status.COMPLETED,
+    #         amount=plan.charge_amount or 0,
+    #         user=request.user,
+    #         subscription=subscription,
+    #         subscription_charge_date=charge_date,
+    #     )
+
+    #     if not created:
+    #         try:
+    #             subscription.prolong()
+    #         except ProlongationImpossible as exc:
+    #             raise PermissionDenied(detail='Cannot prolong subscription') from exc
+
+    #     result = PaymentSerializer({
+    #         'plan': plan,
+    #     })
+
+    #     return Response(result.data)
```

## Comparing `subscriptions/migrations/0003_alter_plan_charge_amount_alter_usage_datetime.py` & `subscriptions/migrations/0024_alter_subscriptionpayment_amount_and_more.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# Generated by Django 4.0.2 on 2022-02-18 08:45
+# Generated by Django 4.0.3 on 2022-10-23 19:29
 
-from django.db import migrations, models
+from django.db import migrations
 import djmoney.models.fields
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('subscriptions', '0002_alter_subscription_begin'),
+        ('subscriptions', '0023_alter_subscription_options_and_more'),
     ]
 
     operations = [
         migrations.AlterField(
-            model_name='plan',
-            name='charge_amount',
+            model_name='subscriptionpayment',
+            name='amount',
             field=djmoney.models.fields.MoneyField(blank=True, decimal_places=2, default_currency='USD', max_digits=14, null=True),
         ),
         migrations.AlterField(
-            model_name='usage',
-            name='datetime',
-            field=models.DateTimeField(blank=True),
+            model_name='subscriptionpaymentrefund',
+            name='amount',
+            field=djmoney.models.fields.MoneyField(blank=True, decimal_places=2, default_currency='USD', max_digits=14, null=True),
         ),
     ]
```

## Comparing `subscriptions/migrations/0006_alter_plan_charge_period_and_more.py` & `subscriptions/migrations/0005_alter_subscriptionpayment_metadata_and_more.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,32 @@
-# Generated by Django 4.0.3 on 2022-03-09 20:42
+# Generated by Django 4.0.3 on 2022-06-06 11:54
 
-from django.db import migrations
-import subscriptions.fields
+import django.core.serializers.json
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('subscriptions', '0005_plan_slug'),
+        ('subscriptions', '0004_remove_plan_unique_plan_slug_remove_plan_slug'),
     ]
 
     operations = [
         migrations.AlterField(
-            model_name='plan',
-            name='charge_period',
-            field=subscriptions.fields.RelativeDurationField(blank=True, help_text='leave blank for one-time charge'),
+            model_name='subscriptionpayment',
+            name='metadata',
+            field=models.JSONField(blank=True, default=dict, encoder=django.core.serializers.json.DjangoJSONEncoder),
         ),
         migrations.AlterField(
-            model_name='plan',
-            name='subscription_duration',
-            field=subscriptions.fields.RelativeDurationField(blank=True, help_text='DD HH:MM:SS; leave blank to make it an infinite subscription'),
+            model_name='subscriptionpaymentrefund',
+            name='metadata',
+            field=models.JSONField(blank=True, default=dict, encoder=django.core.serializers.json.DjangoJSONEncoder),
         ),
-        migrations.AlterField(
-            model_name='quota',
-            name='burns_in',
-            field=subscriptions.fields.RelativeDurationField(blank=True, help_text='leave blank to burn each recharge period'),
+        migrations.AddIndex(
+            model_name='subscriptionpayment',
+            index=models.Index(fields=['provider_codename', 'provider_transaction_id'], name='subscriptio_provide_db7519_idx'),
         ),
-        migrations.AlterField(
-            model_name='quota',
-            name='recharge_period',
-            field=subscriptions.fields.RelativeDurationField(blank=True, help_text='leave blank for recharging only after each subscription prolongation (charge)'),
+        migrations.AddIndex(
+            model_name='subscriptionpaymentrefund',
+            index=models.Index(fields=['provider_codename', 'provider_transaction_id'], name='subscriptio_provide_3a088f_idx'),
         ),
     ]
```

## Comparing `subscriptions/migrations/0007_subscriptionpayment_and_more.py` & `subscriptions/migrations/0009_auto_20220711_2159.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-# Generated by Django 4.0.3 on 2022-03-10 20:39
+# Generated by Django 3.2.11 on 2022-07-11 21:59
 
-import django.db.models.deletion
-import djmoney.models.fields
-import subscriptions.fields
-from dateutil.relativedelta import relativedelta
-from django.conf import settings
 from django.db import migrations, models
+import djmoney.models.fields
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        migrations.swappable_dependency(settings.AUTH_USER_MODEL),
-        ('subscriptions', '0006_alter_plan_charge_period_and_more'),
+        ('subscriptions', '0008_subscriptionpayment_quantity'),
     ]
 
     operations = [
-        migrations.CreateModel(
-            name='SubscriptionPayment',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('vendor', models.CharField(max_length=255)),
-                ('vendor_transaction_id', models.CharField(max_length=255)),
-                ('status', models.PositiveSmallIntegerField(choices=[(0, 'Pending'), (1, 'Preauth'), (2, 'Completed'), (3, 'Canceled'), (4, 'Error')], default=0)),
-                ('amount_currency', djmoney.models.fields.CurrencyField(choices=[('XUA', 'ADB Unit of Account'), ('AFN', 'Afghan Afghani'), ('AFA', 'Afghan Afghani (1927–2002)'), ('ALL', 'Albanian Lek'), ('ALK', 'Albanian Lek (1946–1965)'), ('DZD', 'Algerian Dinar'), ('ADP', 'Andorran Peseta'), ('AOA', 'Angolan Kwanza'), ('AOK', 'Angolan Kwanza (1977–1991)'), ('AON', 'Angolan New Kwanza (1990–2000)'), ('AOR', 'Angolan Readjusted Kwanza (1995–1999)'), ('ARA', 'Argentine Austral'), ('ARS', 'Argentine Peso'), ('ARM', 'Argentine Peso (1881–1970)'), ('ARP', 'Argentine Peso (1983–1985)'), ('ARL', 'Argentine Peso Ley (1970–1983)'), ('AMD', 'Armenian Dram'), ('AWG', 'Aruban Florin'), ('AUD', 'Australian Dollar'), ('ATS', 'Austrian Schilling'), ('AZN', 'Azerbaijani Manat'), ('AZM', 'Azerbaijani Manat (1993–2006)'), ('BSD', 'Bahamian Dollar'), ('BHD', 'Bahraini Dinar'), ('BDT', 'Bangladeshi Taka'), ('BBD', 'Barbadian Dollar'), ('BYN', 'Belarusian Ruble'), ('BYB', 'Belarusian Ruble (1994–1999)'), ('BYR', 'Belarusian Ruble (2000–2016)'), ('BEF', 'Belgian Franc'), ('BEC', 'Belgian Franc (convertible)'), ('BEL', 'Belgian Franc (financial)'), ('BZD', 'Belize Dollar'), ('BMD', 'Bermudan Dollar'), ('BTN', 'Bhutanese Ngultrum'), ('BOB', 'Bolivian Boliviano'), ('BOL', 'Bolivian Boliviano (1863–1963)'), ('BOV', 'Bolivian Mvdol'), ('BOP', 'Bolivian Peso'), ('BAM', 'Bosnia-Herzegovina Convertible Mark'), ('BAD', 'Bosnia-Herzegovina Dinar (1992–1994)'), ('BAN', 'Bosnia-Herzegovina New Dinar (1994–1997)'), ('BWP', 'Botswanan Pula'), ('BRC', 'Brazilian Cruzado (1986–1989)'), ('BRZ', 'Brazilian Cruzeiro (1942–1967)'), ('BRE', 'Brazilian Cruzeiro (1990–1993)'), ('BRR', 'Brazilian Cruzeiro (1993–1994)'), ('BRN', 'Brazilian New Cruzado (1989–1990)'), ('BRB', 'Brazilian New Cruzeiro (1967–1986)'), ('BRL', 'Brazilian Real'), ('GBP', 'British Pound'), ('BND', 'Brunei Dollar'), ('BGL', 'Bulgarian Hard Lev'), ('BGN', 'Bulgarian Lev'), ('BGO', 'Bulgarian Lev (1879–1952)'), ('BGM', 'Bulgarian Socialist Lev'), ('BUK', 'Burmese Kyat'), ('BIF', 'Burundian Franc'), ('XPF', 'CFP Franc'), ('KHR', 'Cambodian Riel'), ('CAD', 'Canadian Dollar'), ('CVE', 'Cape Verdean Escudo'), ('KYD', 'Cayman Islands Dollar'), ('XAF', 'Central African CFA Franc'), ('CLE', 'Chilean Escudo'), ('CLP', 'Chilean Peso'), ('CLF', 'Chilean Unit of Account (UF)'), ('CNX', 'Chinese People’s Bank Dollar'), ('CNY', 'Chinese Yuan'), ('CNH', 'Chinese Yuan (offshore)'), ('COP', 'Colombian Peso'), ('COU', 'Colombian Real Value Unit'), ('KMF', 'Comorian Franc'), ('CDF', 'Congolese Franc'), ('CRC', 'Costa Rican Colón'), ('HRD', 'Croatian Dinar'), ('HRK', 'Croatian Kuna'), ('CUC', 'Cuban Convertible Peso'), ('CUP', 'Cuban Peso'), ('CYP', 'Cypriot Pound'), ('CZK', 'Czech Koruna'), ('CSK', 'Czechoslovak Hard Koruna'), ('DKK', 'Danish Krone'), ('DJF', 'Djiboutian Franc'), ('DOP', 'Dominican Peso'), ('NLG', 'Dutch Guilder'), ('XCD', 'East Caribbean Dollar'), ('DDM', 'East German Mark'), ('ECS', 'Ecuadorian Sucre'), ('ECV', 'Ecuadorian Unit of Constant Value'), ('EGP', 'Egyptian Pound'), ('GQE', 'Equatorial Guinean Ekwele'), ('ERN', 'Eritrean Nakfa'), ('EEK', 'Estonian Kroon'), ('ETB', 'Ethiopian Birr'), ('EUR', 'Euro'), ('XBA', 'European Composite Unit'), ('XEU', 'European Currency Unit'), ('XBB', 'European Monetary Unit'), ('XBC', 'European Unit of Account (XBC)'), ('XBD', 'European Unit of Account (XBD)'), ('FKP', 'Falkland Islands Pound'), ('FJD', 'Fijian Dollar'), ('FIM', 'Finnish Markka'), ('FRF', 'French Franc'), ('XFO', 'French Gold Franc'), ('XFU', 'French UIC-Franc'), ('GMD', 'Gambian Dalasi'), ('GEK', 'Georgian Kupon Larit'), ('GEL', 'Georgian Lari'), ('DEM', 'German Mark'), ('GHS', 'Ghanaian Cedi'), ('GHC', 'Ghanaian Cedi (1979–2007)'), ('GIP', 'Gibraltar Pound'), ('XAU', 'Gold'), ('GRD', 'Greek Drachma'), ('GTQ', 'Guatemalan Quetzal'), ('GWP', 'Guinea-Bissau Peso'), ('GNF', 'Guinean Franc'), ('GNS', 'Guinean Syli'), ('GYD', 'Guyanaese Dollar'), ('HTG', 'Haitian Gourde'), ('HNL', 'Honduran Lempira'), ('HKD', 'Hong Kong Dollar'), ('HUF', 'Hungarian Forint'), ('IMP', 'IMP'), ('ISK', 'Icelandic Króna'), ('ISJ', 'Icelandic Króna (1918–1981)'), ('INR', 'Indian Rupee'), ('IDR', 'Indonesian Rupiah'), ('IRR', 'Iranian Rial'), ('IQD', 'Iraqi Dinar'), ('IEP', 'Irish Pound'), ('ILS', 'Israeli New Shekel'), ('ILP', 'Israeli Pound'), ('ILR', 'Israeli Shekel (1980–1985)'), ('ITL', 'Italian Lira'), ('JMD', 'Jamaican Dollar'), ('JPY', 'Japanese Yen'), ('JOD', 'Jordanian Dinar'), ('KZT', 'Kazakhstani Tenge'), ('KES', 'Kenyan Shilling'), ('KWD', 'Kuwaiti Dinar'), ('KGS', 'Kyrgystani Som'), ('LAK', 'Laotian Kip'), ('LVL', 'Latvian Lats'), ('LVR', 'Latvian Ruble'), ('LBP', 'Lebanese Pound'), ('LSL', 'Lesotho Loti'), ('LRD', 'Liberian Dollar'), ('LYD', 'Libyan Dinar'), ('LTL', 'Lithuanian Litas'), ('LTT', 'Lithuanian Talonas'), ('LUL', 'Luxembourg Financial Franc'), ('LUC', 'Luxembourgian Convertible Franc'), ('LUF', 'Luxembourgian Franc'), ('MOP', 'Macanese Pataca'), ('MKD', 'Macedonian Denar'), ('MKN', 'Macedonian Denar (1992–1993)'), ('MGA', 'Malagasy Ariary'), ('MGF', 'Malagasy Franc'), ('MWK', 'Malawian Kwacha'), ('MYR', 'Malaysian Ringgit'), ('MVR', 'Maldivian Rufiyaa'), ('MVP', 'Maldivian Rupee (1947–1981)'), ('MLF', 'Malian Franc'), ('MTL', 'Maltese Lira'), ('MTP', 'Maltese Pound'), ('MRU', 'Mauritanian Ouguiya'), ('MRO', 'Mauritanian Ouguiya (1973–2017)'), ('MUR', 'Mauritian Rupee'), ('MXV', 'Mexican Investment Unit'), ('MXN', 'Mexican Peso'), ('MXP', 'Mexican Silver Peso (1861–1992)'), ('MDC', 'Moldovan Cupon'), ('MDL', 'Moldovan Leu'), ('MCF', 'Monegasque Franc'), ('MNT', 'Mongolian Tugrik'), ('MAD', 'Moroccan Dirham'), ('MAF', 'Moroccan Franc'), ('MZE', 'Mozambican Escudo'), ('MZN', 'Mozambican Metical'), ('MZM', 'Mozambican Metical (1980–2006)'), ('MMK', 'Myanmar Kyat'), ('NAD', 'Namibian Dollar'), ('NPR', 'Nepalese Rupee'), ('ANG', 'Netherlands Antillean Guilder'), ('TWD', 'New Taiwan Dollar'), ('NZD', 'New Zealand Dollar'), ('NIO', 'Nicaraguan Córdoba'), ('NIC', 'Nicaraguan Córdoba (1988–1991)'), ('NGN', 'Nigerian Naira'), ('KPW', 'North Korean Won'), ('NOK', 'Norwegian Krone'), ('OMR', 'Omani Rial'), ('PKR', 'Pakistani Rupee'), ('XPD', 'Palladium'), ('PAB', 'Panamanian Balboa'), ('PGK', 'Papua New Guinean Kina'), ('PYG', 'Paraguayan Guarani'), ('PEI', 'Peruvian Inti'), ('PEN', 'Peruvian Sol'), ('PES', 'Peruvian Sol (1863–1965)'), ('PHP', 'Philippine Piso'), ('XPT', 'Platinum'), ('PLN', 'Polish Zloty'), ('PLZ', 'Polish Zloty (1950–1995)'), ('PTE', 'Portuguese Escudo'), ('GWE', 'Portuguese Guinea Escudo'), ('QAR', 'Qatari Rial'), ('XRE', 'RINET Funds'), ('RHD', 'Rhodesian Dollar'), ('RON', 'Romanian Leu'), ('ROL', 'Romanian Leu (1952–2006)'), ('RUB', 'Russian Ruble'), ('RUR', 'Russian Ruble (1991–1998)'), ('RWF', 'Rwandan Franc'), ('SVC', 'Salvadoran Colón'), ('WST', 'Samoan Tala'), ('SAR', 'Saudi Riyal'), ('RSD', 'Serbian Dinar'), ('CSD', 'Serbian Dinar (2002–2006)'), ('SCR', 'Seychellois Rupee'), ('SLL', 'Sierra Leonean Leone'), ('XAG', 'Silver'), ('SGD', 'Singapore Dollar'), ('SKK', 'Slovak Koruna'), ('SIT', 'Slovenian Tolar'), ('SBD', 'Solomon Islands Dollar'), ('SOS', 'Somali Shilling'), ('ZAR', 'South African Rand'), ('ZAL', 'South African Rand (financial)'), ('KRH', 'South Korean Hwan (1953–1962)'), ('KRW', 'South Korean Won'), ('KRO', 'South Korean Won (1945–1953)'), ('SSP', 'South Sudanese Pound'), ('SUR', 'Soviet Rouble'), ('ESP', 'Spanish Peseta'), ('ESA', 'Spanish Peseta (A account)'), ('ESB', 'Spanish Peseta (convertible account)'), ('XDR', 'Special Drawing Rights'), ('LKR', 'Sri Lankan Rupee'), ('SHP', 'St. Helena Pound'), ('XSU', 'Sucre'), ('SDD', 'Sudanese Dinar (1992–2007)'), ('SDG', 'Sudanese Pound'), ('SDP', 'Sudanese Pound (1957–1998)'), ('SRD', 'Surinamese Dollar'), ('SRG', 'Surinamese Guilder'), ('SZL', 'Swazi Lilangeni'), ('SEK', 'Swedish Krona'), ('CHF', 'Swiss Franc'), ('SYP', 'Syrian Pound'), ('STN', 'São Tomé & Príncipe Dobra'), ('STD', 'São Tomé & Príncipe Dobra (1977–2017)'), ('TVD', 'TVD'), ('TJR', 'Tajikistani Ruble'), ('TJS', 'Tajikistani Somoni'), ('TZS', 'Tanzanian Shilling'), ('XTS', 'Testing Currency Code'), ('THB', 'Thai Baht'), ('XXX', 'The codes assigned for transactions where no currency is involved'), ('TPE', 'Timorese Escudo'), ('TOP', 'Tongan Paʻanga'), ('TTD', 'Trinidad & Tobago Dollar'), ('TND', 'Tunisian Dinar'), ('TRY', 'Turkish Lira'), ('TRL', 'Turkish Lira (1922–2005)'), ('TMT', 'Turkmenistani Manat'), ('TMM', 'Turkmenistani Manat (1993–2009)'), ('USD', 'US Dollar'), ('USN', 'US Dollar (Next day)'), ('USS', 'US Dollar (Same day)'), ('UGX', 'Ugandan Shilling'), ('UGS', 'Ugandan Shilling (1966–1987)'), ('UAH', 'Ukrainian Hryvnia'), ('UAK', 'Ukrainian Karbovanets'), ('AED', 'United Arab Emirates Dirham'), ('UYW', 'Uruguayan Nominal Wage Index Unit'), ('UYU', 'Uruguayan Peso'), ('UYP', 'Uruguayan Peso (1975–1993)'), ('UYI', 'Uruguayan Peso (Indexed Units)'), ('UZS', 'Uzbekistani Som'), ('VUV', 'Vanuatu Vatu'), ('VES', 'Venezuelan Bolívar'), ('VEB', 'Venezuelan Bolívar (1871–2008)'), ('VEF', 'Venezuelan Bolívar (2008–2018)'), ('VND', 'Vietnamese Dong'), ('VNN', 'Vietnamese Dong (1978–1985)'), ('CHE', 'WIR Euro'), ('CHW', 'WIR Franc'), ('XOF', 'West African CFA Franc'), ('YDD', 'Yemeni Dinar'), ('YER', 'Yemeni Rial'), ('YUN', 'Yugoslavian Convertible Dinar (1990–1992)'), ('YUD', 'Yugoslavian Hard Dinar (1966–1990)'), ('YUM', 'Yugoslavian New Dinar (1994–2002)'), ('YUR', 'Yugoslavian Reformed Dinar (1992–1993)'), ('ZWN', 'ZWN'), ('ZRN', 'Zairean New Zaire (1993–1998)'), ('ZRZ', 'Zairean Zaire (1971–1993)'), ('ZMW', 'Zambian Kwacha'), ('ZMK', 'Zambian Kwacha (1968–2012)'), ('ZWD', 'Zimbabwean Dollar (1980–2008)'), ('ZWR', 'Zimbabwean Dollar (2008)'), ('ZWL', 'Zimbabwean Dollar (2009)')], default='USD', editable=False, max_length=3)),
-                ('amount', djmoney.models.fields.MoneyField(decimal_places=2, default_currency='USD', max_digits=14)),
-                ('created', models.DateTimeField(blank=True, editable=False)),
-                ('updated', models.DateTimeField(blank=True, editable=False)),
-                ('subscription_charge_date', models.DateTimeField()),
-                ('subscription', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.PROTECT, related_name='%(class)ss', to='subscriptions.subscription')),
-                ('user', models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, related_name='%(class)ss', to=settings.AUTH_USER_MODEL)),
-            ],
-            options={
-                'abstract': False,
-            },
-        ),
-        migrations.RemoveField(
+        migrations.AlterField(
             model_name='plan',
-            name='subscription_duration',
+            name='charge_amount_currency',
+            field=djmoney.models.fields.CurrencyField(choices=[('XUA', 'ADB Unit of Account'), ('AFN', 'Afghan Afghani'), ('AFA', 'Afghan Afghani (1927–2002)'), ('ALL', 'Albanian Lek'), ('ALK', 'Albanian Lek (1946–1965)'), ('DZD', 'Algerian Dinar'), ('ADP', 'Andorran Peseta'), ('AOA', 'Angolan Kwanza'), ('AOK', 'Angolan Kwanza (1977–1991)'), ('AON', 'Angolan New Kwanza (1990–2000)'), ('AOR', 'Angolan Readjusted Kwanza (1995–1999)'), ('ARA', 'Argentine Austral'), ('ARS', 'Argentine Peso'), ('ARM', 'Argentine Peso (1881–1970)'), ('ARP', 'Argentine Peso (1983–1985)'), ('ARL', 'Argentine Peso Ley (1970–1983)'), ('AMD', 'Armenian Dram'), ('AWG', 'Aruban Florin'), ('AUD', 'Australian Dollar'), ('ATS', 'Austrian Schilling'), ('AZN', 'Azerbaijani Manat'), ('AZM', 'Azerbaijani Manat (1993–2006)'), ('BSD', 'Bahamian Dollar'), ('BHD', 'Bahraini Dinar'), ('BDT', 'Bangladeshi Taka'), ('BBD', 'Barbadian Dollar'), ('BYN', 'Belarusian Ruble'), ('BYB', 'Belarusian Ruble (1994–1999)'), ('BYR', 'Belarusian Ruble (2000–2016)'), ('BEF', 'Belgian Franc'), ('BEC', 'Belgian Franc (convertible)'), ('BEL', 'Belgian Franc (financial)'), ('BZD', 'Belize Dollar'), ('BMD', 'Bermudan Dollar'), ('BTN', 'Bhutanese Ngultrum'), ('BOB', 'Bolivian Boliviano'), ('BOL', 'Bolivian Boliviano (1863–1963)'), ('BOV', 'Bolivian Mvdol'), ('BOP', 'Bolivian Peso'), ('BAM', 'Bosnia-Herzegovina Convertible Mark'), ('BAD', 'Bosnia-Herzegovina Dinar (1992–1994)'), ('BAN', 'Bosnia-Herzegovina New Dinar (1994–1997)'), ('BWP', 'Botswanan Pula'), ('BRC', 'Brazilian Cruzado (1986–1989)'), ('BRZ', 'Brazilian Cruzeiro (1942–1967)'), ('BRE', 'Brazilian Cruzeiro (1990–1993)'), ('BRR', 'Brazilian Cruzeiro (1993–1994)'), ('BRN', 'Brazilian New Cruzado (1989–1990)'), ('BRB', 'Brazilian New Cruzeiro (1967–1986)'), ('BRL', 'Brazilian Real'), ('GBP', 'British Pound'), ('BND', 'Brunei Dollar'), ('BGL', 'Bulgarian Hard Lev'), ('BGN', 'Bulgarian Lev'), ('BGO', 'Bulgarian Lev (1879–1952)'), ('BGM', 'Bulgarian Socialist Lev'), ('BUK', 'Burmese Kyat'), ('BIF', 'Burundian Franc'), ('XPF', 'CFP Franc'), ('KHR', 'Cambodian Riel'), ('CAD', 'Canadian Dollar'), ('CVE', 'Cape Verdean Escudo'), ('KYD', 'Cayman Islands Dollar'), ('XAF', 'Central African CFA Franc'), ('CLE', 'Chilean Escudo'), ('CLP', 'Chilean Peso'), ('CLF', 'Chilean Unit of Account (UF)'), ('CNX', 'Chinese People’s Bank Dollar'), ('CNY', 'Chinese Yuan'), ('CNH', 'Chinese Yuan (offshore)'), ('COP', 'Colombian Peso'), ('COU', 'Colombian Real Value Unit'), ('KMF', 'Comorian Franc'), ('CDF', 'Congolese Franc'), ('CRC', 'Costa Rican Colón'), ('HRD', 'Croatian Dinar'), ('HRK', 'Croatian Kuna'), ('CUC', 'Cuban Convertible Peso'), ('CUP', 'Cuban Peso'), ('CYP', 'Cypriot Pound'), ('CZK', 'Czech Koruna'), ('CSK', 'Czechoslovak Hard Koruna'), ('DKK', 'Danish Krone'), ('DJF', 'Djiboutian Franc'), ('DOP', 'Dominican Peso'), ('NLG', 'Dutch Guilder'), ('XCD', 'East Caribbean Dollar'), ('DDM', 'East German Mark'), ('ECS', 'Ecuadorian Sucre'), ('ECV', 'Ecuadorian Unit of Constant Value'), ('EGP', 'Egyptian Pound'), ('GQE', 'Equatorial Guinean Ekwele'), ('ERN', 'Eritrean Nakfa'), ('EEK', 'Estonian Kroon'), ('ETB', 'Ethiopian Birr'), ('EUR', 'Euro'), ('XBA', 'European Composite Unit'), ('XEU', 'European Currency Unit'), ('XBB', 'European Monetary Unit'), ('XBC', 'European Unit of Account (XBC)'), ('XBD', 'European Unit of Account (XBD)'), ('FKP', 'Falkland Islands Pound'), ('FJD', 'Fijian Dollar'), ('FIM', 'Finnish Markka'), ('FRF', 'French Franc'), ('XFO', 'French Gold Franc'), ('XFU', 'French UIC-Franc'), ('GMD', 'Gambian Dalasi'), ('GEK', 'Georgian Kupon Larit'), ('GEL', 'Georgian Lari'), ('DEM', 'German Mark'), ('GHS', 'Ghanaian Cedi'), ('GHC', 'Ghanaian Cedi (1979–2007)'), ('GIP', 'Gibraltar Pound'), ('XAU', 'Gold'), ('GRD', 'Greek Drachma'), ('GTQ', 'Guatemalan Quetzal'), ('GWP', 'Guinea-Bissau Peso'), ('GNF', 'Guinean Franc'), ('GNS', 'Guinean Syli'), ('GYD', 'Guyanaese Dollar'), ('HTG', 'Haitian Gourde'), ('HNL', 'Honduran Lempira'), ('HKD', 'Hong Kong Dollar'), ('HUF', 'Hungarian Forint'), ('IMP', 'IMP'), ('ISK', 'Icelandic Króna'), ('ISJ', 'Icelandic Króna (1918–1981)'), ('INR', 'Indian Rupee'), ('IDR', 'Indonesian Rupiah'), ('IRR', 'Iranian Rial'), ('IQD', 'Iraqi Dinar'), ('IEP', 'Irish Pound'), ('ILS', 'Israeli New Shekel'), ('ILP', 'Israeli Pound'), ('ILR', 'Israeli Shekel (1980–1985)'), ('ITL', 'Italian Lira'), ('JMD', 'Jamaican Dollar'), ('JPY', 'Japanese Yen'), ('JOD', 'Jordanian Dinar'), ('KZT', 'Kazakhstani Tenge'), ('KES', 'Kenyan Shilling'), ('KWD', 'Kuwaiti Dinar'), ('KGS', 'Kyrgystani Som'), ('LAK', 'Laotian Kip'), ('LVL', 'Latvian Lats'), ('LVR', 'Latvian Ruble'), ('LBP', 'Lebanese Pound'), ('LSL', 'Lesotho Loti'), ('LRD', 'Liberian Dollar'), ('LYD', 'Libyan Dinar'), ('LTL', 'Lithuanian Litas'), ('LTT', 'Lithuanian Talonas'), ('LUL', 'Luxembourg Financial Franc'), ('LUC', 'Luxembourgian Convertible Franc'), ('LUF', 'Luxembourgian Franc'), ('MOP', 'Macanese Pataca'), ('MKD', 'Macedonian Denar'), ('MKN', 'Macedonian Denar (1992–1993)'), ('MGA', 'Malagasy Ariary'), ('MGF', 'Malagasy Franc'), ('MWK', 'Malawian Kwacha'), ('MYR', 'Malaysian Ringgit'), ('MVR', 'Maldivian Rufiyaa'), ('MVP', 'Maldivian Rupee (1947–1981)'), ('MLF', 'Malian Franc'), ('MTL', 'Maltese Lira'), ('MTP', 'Maltese Pound'), ('MRU', 'Mauritanian Ouguiya'), ('MRO', 'Mauritanian Ouguiya (1973–2017)'), ('MUR', 'Mauritian Rupee'), ('MXV', 'Mexican Investment Unit'), ('MXN', 'Mexican Peso'), ('MXP', 'Mexican Silver Peso (1861–1992)'), ('MDC', 'Moldovan Cupon'), ('MDL', 'Moldovan Leu'), ('MCF', 'Monegasque Franc'), ('MNT', 'Mongolian Tugrik'), ('MAD', 'Moroccan Dirham'), ('MAF', 'Moroccan Franc'), ('MZE', 'Mozambican Escudo'), ('MZN', 'Mozambican Metical'), ('MZM', 'Mozambican Metical (1980–2006)'), ('MMK', 'Myanmar Kyat'), ('NAD', 'Namibian Dollar'), ('NPR', 'Nepalese Rupee'), ('ANG', 'Netherlands Antillean Guilder'), ('TWD', 'New Taiwan Dollar'), ('NZD', 'New Zealand Dollar'), ('NIO', 'Nicaraguan Córdoba'), ('NIC', 'Nicaraguan Córdoba (1988–1991)'), ('NGN', 'Nigerian Naira'), ('KPW', 'North Korean Won'), ('NOK', 'Norwegian Krone'), ('OMR', 'Omani Rial'), ('PKR', 'Pakistani Rupee'), ('XPD', 'Palladium'), ('PAB', 'Panamanian Balboa'), ('PGK', 'Papua New Guinean Kina'), ('PYG', 'Paraguayan Guarani'), ('PEI', 'Peruvian Inti'), ('PEN', 'Peruvian Sol'), ('PES', 'Peruvian Sol (1863–1965)'), ('PHP', 'Philippine Peso'), ('XPT', 'Platinum'), ('PLN', 'Polish Zloty'), ('PLZ', 'Polish Zloty (1950–1995)'), ('PTE', 'Portuguese Escudo'), ('GWE', 'Portuguese Guinea Escudo'), ('QAR', 'Qatari Rial'), ('XRE', 'RINET Funds'), ('RHD', 'Rhodesian Dollar'), ('RON', 'Romanian Leu'), ('ROL', 'Romanian Leu (1952–2006)'), ('RUB', 'Russian Ruble'), ('RUR', 'Russian Ruble (1991–1998)'), ('RWF', 'Rwandan Franc'), ('SVC', 'Salvadoran Colón'), ('WST', 'Samoan Tala'), ('SAR', 'Saudi Riyal'), ('RSD', 'Serbian Dinar'), ('CSD', 'Serbian Dinar (2002–2006)'), ('SCR', 'Seychellois Rupee'), ('SLL', 'Sierra Leonean Leone'), ('XAG', 'Silver'), ('SGD', 'Singapore Dollar'), ('SKK', 'Slovak Koruna'), ('SIT', 'Slovenian Tolar'), ('SBD', 'Solomon Islands Dollar'), ('SOS', 'Somali Shilling'), ('ZAR', 'South African Rand'), ('ZAL', 'South African Rand (financial)'), ('KRH', 'South Korean Hwan (1953–1962)'), ('KRW', 'South Korean Won'), ('KRO', 'South Korean Won (1945–1953)'), ('SSP', 'South Sudanese Pound'), ('SUR', 'Soviet Rouble'), ('ESP', 'Spanish Peseta'), ('ESA', 'Spanish Peseta (A account)'), ('ESB', 'Spanish Peseta (convertible account)'), ('XDR', 'Special Drawing Rights'), ('LKR', 'Sri Lankan Rupee'), ('SHP', 'St. Helena Pound'), ('XSU', 'Sucre'), ('SDD', 'Sudanese Dinar (1992–2007)'), ('SDG', 'Sudanese Pound'), ('SDP', 'Sudanese Pound (1957–1998)'), ('SRD', 'Surinamese Dollar'), ('SRG', 'Surinamese Guilder'), ('SZL', 'Swazi Lilangeni'), ('SEK', 'Swedish Krona'), ('CHF', 'Swiss Franc'), ('SYP', 'Syrian Pound'), ('STN', 'São Tomé & Príncipe Dobra'), ('STD', 'São Tomé & Príncipe Dobra (1977–2017)'), ('TVD', 'TVD'), ('TJR', 'Tajikistani Ruble'), ('TJS', 'Tajikistani Somoni'), ('TZS', 'Tanzanian Shilling'), ('XTS', 'Testing Currency Code'), ('THB', 'Thai Baht'), ('XXX', 'The codes assigned for transactions where no currency is involved'), ('TPE', 'Timorese Escudo'), ('TOP', 'Tongan Paʻanga'), ('TTD', 'Trinidad & Tobago Dollar'), ('TND', 'Tunisian Dinar'), ('TRY', 'Turkish Lira'), ('TRL', 'Turkish Lira (1922–2005)'), ('TMT', 'Turkmenistani Manat'), ('TMM', 'Turkmenistani Manat (1993–2009)'), ('USD', 'US Dollar'), ('USN', 'US Dollar (Next day)'), ('USS', 'US Dollar (Same day)'), ('UGX', 'Ugandan Shilling'), ('UGS', 'Ugandan Shilling (1966–1987)'), ('UAH', 'Ukrainian Hryvnia'), ('UAK', 'Ukrainian Karbovanets'), ('AED', 'United Arab Emirates Dirham'), ('UYW', 'Uruguayan Nominal Wage Index Unit'), ('UYU', 'Uruguayan Peso'), ('UYP', 'Uruguayan Peso (1975–1993)'), ('UYI', 'Uruguayan Peso (Indexed Units)'), ('UZS', 'Uzbekistani Som'), ('VUV', 'Vanuatu Vatu'), ('VES', 'Venezuelan Bolívar'), ('VEB', 'Venezuelan Bolívar (1871–2008)'), ('VEF', 'Venezuelan Bolívar (2008–2018)'), ('VND', 'Vietnamese Dong'), ('VNN', 'Vietnamese Dong (1978–1985)'), ('CHE', 'WIR Euro'), ('CHW', 'WIR Franc'), ('XOF', 'West African CFA Franc'), ('YDD', 'Yemeni Dinar'), ('YER', 'Yemeni Rial'), ('YUN', 'Yugoslavian Convertible Dinar (1990–1992)'), ('YUD', 'Yugoslavian Hard Dinar (1966–1990)'), ('YUM', 'Yugoslavian New Dinar (1994–2002)'), ('YUR', 'Yugoslavian Reformed Dinar (1992–1993)'), ('ZWN', 'ZWN'), ('ZRN', 'Zairean New Zaire (1993–1998)'), ('ZRZ', 'Zairean Zaire (1971–1993)'), ('ZMW', 'Zambian Kwacha'), ('ZMK', 'Zambian Kwacha (1968–2012)'), ('ZWD', 'Zimbabwean Dollar (1980–2008)'), ('ZWR', 'Zimbabwean Dollar (2008)'), ('ZWL', 'Zimbabwean Dollar (2009)')], default='USD', editable=False, max_length=3),
         ),
-        migrations.AddField(
+        migrations.AlterField(
             model_name='plan',
-            name='max_duration',
-            field=subscriptions.fields.RelativeDurationField(blank=True, default=relativedelta(), help_text='leave blank to make it an infinite subscription'),
-            preserve_default=False,
-        ),
-        migrations.CreateModel(
-            name='Tax',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('amount_currency', djmoney.models.fields.CurrencyField(choices=[('XUA', 'ADB Unit of Account'), ('AFN', 'Afghan Afghani'), ('AFA', 'Afghan Afghani (1927–2002)'), ('ALL', 'Albanian Lek'), ('ALK', 'Albanian Lek (1946–1965)'), ('DZD', 'Algerian Dinar'), ('ADP', 'Andorran Peseta'), ('AOA', 'Angolan Kwanza'), ('AOK', 'Angolan Kwanza (1977–1991)'), ('AON', 'Angolan New Kwanza (1990–2000)'), ('AOR', 'Angolan Readjusted Kwanza (1995–1999)'), ('ARA', 'Argentine Austral'), ('ARS', 'Argentine Peso'), ('ARM', 'Argentine Peso (1881–1970)'), ('ARP', 'Argentine Peso (1983–1985)'), ('ARL', 'Argentine Peso Ley (1970–1983)'), ('AMD', 'Armenian Dram'), ('AWG', 'Aruban Florin'), ('AUD', 'Australian Dollar'), ('ATS', 'Austrian Schilling'), ('AZN', 'Azerbaijani Manat'), ('AZM', 'Azerbaijani Manat (1993–2006)'), ('BSD', 'Bahamian Dollar'), ('BHD', 'Bahraini Dinar'), ('BDT', 'Bangladeshi Taka'), ('BBD', 'Barbadian Dollar'), ('BYN', 'Belarusian Ruble'), ('BYB', 'Belarusian Ruble (1994–1999)'), ('BYR', 'Belarusian Ruble (2000–2016)'), ('BEF', 'Belgian Franc'), ('BEC', 'Belgian Franc (convertible)'), ('BEL', 'Belgian Franc (financial)'), ('BZD', 'Belize Dollar'), ('BMD', 'Bermudan Dollar'), ('BTN', 'Bhutanese Ngultrum'), ('BOB', 'Bolivian Boliviano'), ('BOL', 'Bolivian Boliviano (1863–1963)'), ('BOV', 'Bolivian Mvdol'), ('BOP', 'Bolivian Peso'), ('BAM', 'Bosnia-Herzegovina Convertible Mark'), ('BAD', 'Bosnia-Herzegovina Dinar (1992–1994)'), ('BAN', 'Bosnia-Herzegovina New Dinar (1994–1997)'), ('BWP', 'Botswanan Pula'), ('BRC', 'Brazilian Cruzado (1986–1989)'), ('BRZ', 'Brazilian Cruzeiro (1942–1967)'), ('BRE', 'Brazilian Cruzeiro (1990–1993)'), ('BRR', 'Brazilian Cruzeiro (1993–1994)'), ('BRN', 'Brazilian New Cruzado (1989–1990)'), ('BRB', 'Brazilian New Cruzeiro (1967–1986)'), ('BRL', 'Brazilian Real'), ('GBP', 'British Pound'), ('BND', 'Brunei Dollar'), ('BGL', 'Bulgarian Hard Lev'), ('BGN', 'Bulgarian Lev'), ('BGO', 'Bulgarian Lev (1879–1952)'), ('BGM', 'Bulgarian Socialist Lev'), ('BUK', 'Burmese Kyat'), ('BIF', 'Burundian Franc'), ('XPF', 'CFP Franc'), ('KHR', 'Cambodian Riel'), ('CAD', 'Canadian Dollar'), ('CVE', 'Cape Verdean Escudo'), ('KYD', 'Cayman Islands Dollar'), ('XAF', 'Central African CFA Franc'), ('CLE', 'Chilean Escudo'), ('CLP', 'Chilean Peso'), ('CLF', 'Chilean Unit of Account (UF)'), ('CNX', 'Chinese People’s Bank Dollar'), ('CNY', 'Chinese Yuan'), ('CNH', 'Chinese Yuan (offshore)'), ('COP', 'Colombian Peso'), ('COU', 'Colombian Real Value Unit'), ('KMF', 'Comorian Franc'), ('CDF', 'Congolese Franc'), ('CRC', 'Costa Rican Colón'), ('HRD', 'Croatian Dinar'), ('HRK', 'Croatian Kuna'), ('CUC', 'Cuban Convertible Peso'), ('CUP', 'Cuban Peso'), ('CYP', 'Cypriot Pound'), ('CZK', 'Czech Koruna'), ('CSK', 'Czechoslovak Hard Koruna'), ('DKK', 'Danish Krone'), ('DJF', 'Djiboutian Franc'), ('DOP', 'Dominican Peso'), ('NLG', 'Dutch Guilder'), ('XCD', 'East Caribbean Dollar'), ('DDM', 'East German Mark'), ('ECS', 'Ecuadorian Sucre'), ('ECV', 'Ecuadorian Unit of Constant Value'), ('EGP', 'Egyptian Pound'), ('GQE', 'Equatorial Guinean Ekwele'), ('ERN', 'Eritrean Nakfa'), ('EEK', 'Estonian Kroon'), ('ETB', 'Ethiopian Birr'), ('EUR', 'Euro'), ('XBA', 'European Composite Unit'), ('XEU', 'European Currency Unit'), ('XBB', 'European Monetary Unit'), ('XBC', 'European Unit of Account (XBC)'), ('XBD', 'European Unit of Account (XBD)'), ('FKP', 'Falkland Islands Pound'), ('FJD', 'Fijian Dollar'), ('FIM', 'Finnish Markka'), ('FRF', 'French Franc'), ('XFO', 'French Gold Franc'), ('XFU', 'French UIC-Franc'), ('GMD', 'Gambian Dalasi'), ('GEK', 'Georgian Kupon Larit'), ('GEL', 'Georgian Lari'), ('DEM', 'German Mark'), ('GHS', 'Ghanaian Cedi'), ('GHC', 'Ghanaian Cedi (1979–2007)'), ('GIP', 'Gibraltar Pound'), ('XAU', 'Gold'), ('GRD', 'Greek Drachma'), ('GTQ', 'Guatemalan Quetzal'), ('GWP', 'Guinea-Bissau Peso'), ('GNF', 'Guinean Franc'), ('GNS', 'Guinean Syli'), ('GYD', 'Guyanaese Dollar'), ('HTG', 'Haitian Gourde'), ('HNL', 'Honduran Lempira'), ('HKD', 'Hong Kong Dollar'), ('HUF', 'Hungarian Forint'), ('IMP', 'IMP'), ('ISK', 'Icelandic Króna'), ('ISJ', 'Icelandic Króna (1918–1981)'), ('INR', 'Indian Rupee'), ('IDR', 'Indonesian Rupiah'), ('IRR', 'Iranian Rial'), ('IQD', 'Iraqi Dinar'), ('IEP', 'Irish Pound'), ('ILS', 'Israeli New Shekel'), ('ILP', 'Israeli Pound'), ('ILR', 'Israeli Shekel (1980–1985)'), ('ITL', 'Italian Lira'), ('JMD', 'Jamaican Dollar'), ('JPY', 'Japanese Yen'), ('JOD', 'Jordanian Dinar'), ('KZT', 'Kazakhstani Tenge'), ('KES', 'Kenyan Shilling'), ('KWD', 'Kuwaiti Dinar'), ('KGS', 'Kyrgystani Som'), ('LAK', 'Laotian Kip'), ('LVL', 'Latvian Lats'), ('LVR', 'Latvian Ruble'), ('LBP', 'Lebanese Pound'), ('LSL', 'Lesotho Loti'), ('LRD', 'Liberian Dollar'), ('LYD', 'Libyan Dinar'), ('LTL', 'Lithuanian Litas'), ('LTT', 'Lithuanian Talonas'), ('LUL', 'Luxembourg Financial Franc'), ('LUC', 'Luxembourgian Convertible Franc'), ('LUF', 'Luxembourgian Franc'), ('MOP', 'Macanese Pataca'), ('MKD', 'Macedonian Denar'), ('MKN', 'Macedonian Denar (1992–1993)'), ('MGA', 'Malagasy Ariary'), ('MGF', 'Malagasy Franc'), ('MWK', 'Malawian Kwacha'), ('MYR', 'Malaysian Ringgit'), ('MVR', 'Maldivian Rufiyaa'), ('MVP', 'Maldivian Rupee (1947–1981)'), ('MLF', 'Malian Franc'), ('MTL', 'Maltese Lira'), ('MTP', 'Maltese Pound'), ('MRU', 'Mauritanian Ouguiya'), ('MRO', 'Mauritanian Ouguiya (1973–2017)'), ('MUR', 'Mauritian Rupee'), ('MXV', 'Mexican Investment Unit'), ('MXN', 'Mexican Peso'), ('MXP', 'Mexican Silver Peso (1861–1992)'), ('MDC', 'Moldovan Cupon'), ('MDL', 'Moldovan Leu'), ('MCF', 'Monegasque Franc'), ('MNT', 'Mongolian Tugrik'), ('MAD', 'Moroccan Dirham'), ('MAF', 'Moroccan Franc'), ('MZE', 'Mozambican Escudo'), ('MZN', 'Mozambican Metical'), ('MZM', 'Mozambican Metical (1980–2006)'), ('MMK', 'Myanmar Kyat'), ('NAD', 'Namibian Dollar'), ('NPR', 'Nepalese Rupee'), ('ANG', 'Netherlands Antillean Guilder'), ('TWD', 'New Taiwan Dollar'), ('NZD', 'New Zealand Dollar'), ('NIO', 'Nicaraguan Córdoba'), ('NIC', 'Nicaraguan Córdoba (1988–1991)'), ('NGN', 'Nigerian Naira'), ('KPW', 'North Korean Won'), ('NOK', 'Norwegian Krone'), ('OMR', 'Omani Rial'), ('PKR', 'Pakistani Rupee'), ('XPD', 'Palladium'), ('PAB', 'Panamanian Balboa'), ('PGK', 'Papua New Guinean Kina'), ('PYG', 'Paraguayan Guarani'), ('PEI', 'Peruvian Inti'), ('PEN', 'Peruvian Sol'), ('PES', 'Peruvian Sol (1863–1965)'), ('PHP', 'Philippine Piso'), ('XPT', 'Platinum'), ('PLN', 'Polish Zloty'), ('PLZ', 'Polish Zloty (1950–1995)'), ('PTE', 'Portuguese Escudo'), ('GWE', 'Portuguese Guinea Escudo'), ('QAR', 'Qatari Rial'), ('XRE', 'RINET Funds'), ('RHD', 'Rhodesian Dollar'), ('RON', 'Romanian Leu'), ('ROL', 'Romanian Leu (1952–2006)'), ('RUB', 'Russian Ruble'), ('RUR', 'Russian Ruble (1991–1998)'), ('RWF', 'Rwandan Franc'), ('SVC', 'Salvadoran Colón'), ('WST', 'Samoan Tala'), ('SAR', 'Saudi Riyal'), ('RSD', 'Serbian Dinar'), ('CSD', 'Serbian Dinar (2002–2006)'), ('SCR', 'Seychellois Rupee'), ('SLL', 'Sierra Leonean Leone'), ('XAG', 'Silver'), ('SGD', 'Singapore Dollar'), ('SKK', 'Slovak Koruna'), ('SIT', 'Slovenian Tolar'), ('SBD', 'Solomon Islands Dollar'), ('SOS', 'Somali Shilling'), ('ZAR', 'South African Rand'), ('ZAL', 'South African Rand (financial)'), ('KRH', 'South Korean Hwan (1953–1962)'), ('KRW', 'South Korean Won'), ('KRO', 'South Korean Won (1945–1953)'), ('SSP', 'South Sudanese Pound'), ('SUR', 'Soviet Rouble'), ('ESP', 'Spanish Peseta'), ('ESA', 'Spanish Peseta (A account)'), ('ESB', 'Spanish Peseta (convertible account)'), ('XDR', 'Special Drawing Rights'), ('LKR', 'Sri Lankan Rupee'), ('SHP', 'St. Helena Pound'), ('XSU', 'Sucre'), ('SDD', 'Sudanese Dinar (1992–2007)'), ('SDG', 'Sudanese Pound'), ('SDP', 'Sudanese Pound (1957–1998)'), ('SRD', 'Surinamese Dollar'), ('SRG', 'Surinamese Guilder'), ('SZL', 'Swazi Lilangeni'), ('SEK', 'Swedish Krona'), ('CHF', 'Swiss Franc'), ('SYP', 'Syrian Pound'), ('STN', 'São Tomé & Príncipe Dobra'), ('STD', 'São Tomé & Príncipe Dobra (1977–2017)'), ('TVD', 'TVD'), ('TJR', 'Tajikistani Ruble'), ('TJS', 'Tajikistani Somoni'), ('TZS', 'Tanzanian Shilling'), ('XTS', 'Testing Currency Code'), ('THB', 'Thai Baht'), ('XXX', 'The codes assigned for transactions where no currency is involved'), ('TPE', 'Timorese Escudo'), ('TOP', 'Tongan Paʻanga'), ('TTD', 'Trinidad & Tobago Dollar'), ('TND', 'Tunisian Dinar'), ('TRY', 'Turkish Lira'), ('TRL', 'Turkish Lira (1922–2005)'), ('TMT', 'Turkmenistani Manat'), ('TMM', 'Turkmenistani Manat (1993–2009)'), ('USD', 'US Dollar'), ('USN', 'US Dollar (Next day)'), ('USS', 'US Dollar (Same day)'), ('UGX', 'Ugandan Shilling'), ('UGS', 'Ugandan Shilling (1966–1987)'), ('UAH', 'Ukrainian Hryvnia'), ('UAK', 'Ukrainian Karbovanets'), ('AED', 'United Arab Emirates Dirham'), ('UYW', 'Uruguayan Nominal Wage Index Unit'), ('UYU', 'Uruguayan Peso'), ('UYP', 'Uruguayan Peso (1975–1993)'), ('UYI', 'Uruguayan Peso (Indexed Units)'), ('UZS', 'Uzbekistani Som'), ('VUV', 'Vanuatu Vatu'), ('VES', 'Venezuelan Bolívar'), ('VEB', 'Venezuelan Bolívar (1871–2008)'), ('VEF', 'Venezuelan Bolívar (2008–2018)'), ('VND', 'Vietnamese Dong'), ('VNN', 'Vietnamese Dong (1978–1985)'), ('CHE', 'WIR Euro'), ('CHW', 'WIR Franc'), ('XOF', 'West African CFA Franc'), ('YDD', 'Yemeni Dinar'), ('YER', 'Yemeni Rial'), ('YUN', 'Yugoslavian Convertible Dinar (1990–1992)'), ('YUD', 'Yugoslavian Hard Dinar (1966–1990)'), ('YUM', 'Yugoslavian New Dinar (1994–2002)'), ('YUR', 'Yugoslavian Reformed Dinar (1992–1993)'), ('ZWN', 'ZWN'), ('ZRN', 'Zairean New Zaire (1993–1998)'), ('ZRZ', 'Zairean Zaire (1971–1993)'), ('ZMW', 'Zambian Kwacha'), ('ZMK', 'Zambian Kwacha (1968–2012)'), ('ZWD', 'Zimbabwean Dollar (1980–2008)'), ('ZWR', 'Zimbabwean Dollar (2008)'), ('ZWL', 'Zimbabwean Dollar (2009)')], default='USD', editable=False, max_length=3)),
-                ('amount', djmoney.models.fields.MoneyField(decimal_places=2, default_currency='USD', max_digits=14)),
-                ('subscription_payment', models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, related_name='taxes', to='subscriptions.subscriptionpayment')),
-            ],
-        ),
-        migrations.CreateModel(
-            name='SubscriptionPaymentRefund',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('vendor', models.CharField(max_length=255)),
-                ('vendor_transaction_id', models.CharField(max_length=255)),
-                ('status', models.PositiveSmallIntegerField(choices=[(0, 'Pending'), (1, 'Preauth'), (2, 'Completed'), (3, 'Canceled'), (4, 'Error')], default=0)),
-                ('amount_currency', djmoney.models.fields.CurrencyField(choices=[('XUA', 'ADB Unit of Account'), ('AFN', 'Afghan Afghani'), ('AFA', 'Afghan Afghani (1927–2002)'), ('ALL', 'Albanian Lek'), ('ALK', 'Albanian Lek (1946–1965)'), ('DZD', 'Algerian Dinar'), ('ADP', 'Andorran Peseta'), ('AOA', 'Angolan Kwanza'), ('AOK', 'Angolan Kwanza (1977–1991)'), ('AON', 'Angolan New Kwanza (1990–2000)'), ('AOR', 'Angolan Readjusted Kwanza (1995–1999)'), ('ARA', 'Argentine Austral'), ('ARS', 'Argentine Peso'), ('ARM', 'Argentine Peso (1881–1970)'), ('ARP', 'Argentine Peso (1983–1985)'), ('ARL', 'Argentine Peso Ley (1970–1983)'), ('AMD', 'Armenian Dram'), ('AWG', 'Aruban Florin'), ('AUD', 'Australian Dollar'), ('ATS', 'Austrian Schilling'), ('AZN', 'Azerbaijani Manat'), ('AZM', 'Azerbaijani Manat (1993–2006)'), ('BSD', 'Bahamian Dollar'), ('BHD', 'Bahraini Dinar'), ('BDT', 'Bangladeshi Taka'), ('BBD', 'Barbadian Dollar'), ('BYN', 'Belarusian Ruble'), ('BYB', 'Belarusian Ruble (1994–1999)'), ('BYR', 'Belarusian Ruble (2000–2016)'), ('BEF', 'Belgian Franc'), ('BEC', 'Belgian Franc (convertible)'), ('BEL', 'Belgian Franc (financial)'), ('BZD', 'Belize Dollar'), ('BMD', 'Bermudan Dollar'), ('BTN', 'Bhutanese Ngultrum'), ('BOB', 'Bolivian Boliviano'), ('BOL', 'Bolivian Boliviano (1863–1963)'), ('BOV', 'Bolivian Mvdol'), ('BOP', 'Bolivian Peso'), ('BAM', 'Bosnia-Herzegovina Convertible Mark'), ('BAD', 'Bosnia-Herzegovina Dinar (1992–1994)'), ('BAN', 'Bosnia-Herzegovina New Dinar (1994–1997)'), ('BWP', 'Botswanan Pula'), ('BRC', 'Brazilian Cruzado (1986–1989)'), ('BRZ', 'Brazilian Cruzeiro (1942–1967)'), ('BRE', 'Brazilian Cruzeiro (1990–1993)'), ('BRR', 'Brazilian Cruzeiro (1993–1994)'), ('BRN', 'Brazilian New Cruzado (1989–1990)'), ('BRB', 'Brazilian New Cruzeiro (1967–1986)'), ('BRL', 'Brazilian Real'), ('GBP', 'British Pound'), ('BND', 'Brunei Dollar'), ('BGL', 'Bulgarian Hard Lev'), ('BGN', 'Bulgarian Lev'), ('BGO', 'Bulgarian Lev (1879–1952)'), ('BGM', 'Bulgarian Socialist Lev'), ('BUK', 'Burmese Kyat'), ('BIF', 'Burundian Franc'), ('XPF', 'CFP Franc'), ('KHR', 'Cambodian Riel'), ('CAD', 'Canadian Dollar'), ('CVE', 'Cape Verdean Escudo'), ('KYD', 'Cayman Islands Dollar'), ('XAF', 'Central African CFA Franc'), ('CLE', 'Chilean Escudo'), ('CLP', 'Chilean Peso'), ('CLF', 'Chilean Unit of Account (UF)'), ('CNX', 'Chinese People’s Bank Dollar'), ('CNY', 'Chinese Yuan'), ('CNH', 'Chinese Yuan (offshore)'), ('COP', 'Colombian Peso'), ('COU', 'Colombian Real Value Unit'), ('KMF', 'Comorian Franc'), ('CDF', 'Congolese Franc'), ('CRC', 'Costa Rican Colón'), ('HRD', 'Croatian Dinar'), ('HRK', 'Croatian Kuna'), ('CUC', 'Cuban Convertible Peso'), ('CUP', 'Cuban Peso'), ('CYP', 'Cypriot Pound'), ('CZK', 'Czech Koruna'), ('CSK', 'Czechoslovak Hard Koruna'), ('DKK', 'Danish Krone'), ('DJF', 'Djiboutian Franc'), ('DOP', 'Dominican Peso'), ('NLG', 'Dutch Guilder'), ('XCD', 'East Caribbean Dollar'), ('DDM', 'East German Mark'), ('ECS', 'Ecuadorian Sucre'), ('ECV', 'Ecuadorian Unit of Constant Value'), ('EGP', 'Egyptian Pound'), ('GQE', 'Equatorial Guinean Ekwele'), ('ERN', 'Eritrean Nakfa'), ('EEK', 'Estonian Kroon'), ('ETB', 'Ethiopian Birr'), ('EUR', 'Euro'), ('XBA', 'European Composite Unit'), ('XEU', 'European Currency Unit'), ('XBB', 'European Monetary Unit'), ('XBC', 'European Unit of Account (XBC)'), ('XBD', 'European Unit of Account (XBD)'), ('FKP', 'Falkland Islands Pound'), ('FJD', 'Fijian Dollar'), ('FIM', 'Finnish Markka'), ('FRF', 'French Franc'), ('XFO', 'French Gold Franc'), ('XFU', 'French UIC-Franc'), ('GMD', 'Gambian Dalasi'), ('GEK', 'Georgian Kupon Larit'), ('GEL', 'Georgian Lari'), ('DEM', 'German Mark'), ('GHS', 'Ghanaian Cedi'), ('GHC', 'Ghanaian Cedi (1979–2007)'), ('GIP', 'Gibraltar Pound'), ('XAU', 'Gold'), ('GRD', 'Greek Drachma'), ('GTQ', 'Guatemalan Quetzal'), ('GWP', 'Guinea-Bissau Peso'), ('GNF', 'Guinean Franc'), ('GNS', 'Guinean Syli'), ('GYD', 'Guyanaese Dollar'), ('HTG', 'Haitian Gourde'), ('HNL', 'Honduran Lempira'), ('HKD', 'Hong Kong Dollar'), ('HUF', 'Hungarian Forint'), ('IMP', 'IMP'), ('ISK', 'Icelandic Króna'), ('ISJ', 'Icelandic Króna (1918–1981)'), ('INR', 'Indian Rupee'), ('IDR', 'Indonesian Rupiah'), ('IRR', 'Iranian Rial'), ('IQD', 'Iraqi Dinar'), ('IEP', 'Irish Pound'), ('ILS', 'Israeli New Shekel'), ('ILP', 'Israeli Pound'), ('ILR', 'Israeli Shekel (1980–1985)'), ('ITL', 'Italian Lira'), ('JMD', 'Jamaican Dollar'), ('JPY', 'Japanese Yen'), ('JOD', 'Jordanian Dinar'), ('KZT', 'Kazakhstani Tenge'), ('KES', 'Kenyan Shilling'), ('KWD', 'Kuwaiti Dinar'), ('KGS', 'Kyrgystani Som'), ('LAK', 'Laotian Kip'), ('LVL', 'Latvian Lats'), ('LVR', 'Latvian Ruble'), ('LBP', 'Lebanese Pound'), ('LSL', 'Lesotho Loti'), ('LRD', 'Liberian Dollar'), ('LYD', 'Libyan Dinar'), ('LTL', 'Lithuanian Litas'), ('LTT', 'Lithuanian Talonas'), ('LUL', 'Luxembourg Financial Franc'), ('LUC', 'Luxembourgian Convertible Franc'), ('LUF', 'Luxembourgian Franc'), ('MOP', 'Macanese Pataca'), ('MKD', 'Macedonian Denar'), ('MKN', 'Macedonian Denar (1992–1993)'), ('MGA', 'Malagasy Ariary'), ('MGF', 'Malagasy Franc'), ('MWK', 'Malawian Kwacha'), ('MYR', 'Malaysian Ringgit'), ('MVR', 'Maldivian Rufiyaa'), ('MVP', 'Maldivian Rupee (1947–1981)'), ('MLF', 'Malian Franc'), ('MTL', 'Maltese Lira'), ('MTP', 'Maltese Pound'), ('MRU', 'Mauritanian Ouguiya'), ('MRO', 'Mauritanian Ouguiya (1973–2017)'), ('MUR', 'Mauritian Rupee'), ('MXV', 'Mexican Investment Unit'), ('MXN', 'Mexican Peso'), ('MXP', 'Mexican Silver Peso (1861–1992)'), ('MDC', 'Moldovan Cupon'), ('MDL', 'Moldovan Leu'), ('MCF', 'Monegasque Franc'), ('MNT', 'Mongolian Tugrik'), ('MAD', 'Moroccan Dirham'), ('MAF', 'Moroccan Franc'), ('MZE', 'Mozambican Escudo'), ('MZN', 'Mozambican Metical'), ('MZM', 'Mozambican Metical (1980–2006)'), ('MMK', 'Myanmar Kyat'), ('NAD', 'Namibian Dollar'), ('NPR', 'Nepalese Rupee'), ('ANG', 'Netherlands Antillean Guilder'), ('TWD', 'New Taiwan Dollar'), ('NZD', 'New Zealand Dollar'), ('NIO', 'Nicaraguan Córdoba'), ('NIC', 'Nicaraguan Córdoba (1988–1991)'), ('NGN', 'Nigerian Naira'), ('KPW', 'North Korean Won'), ('NOK', 'Norwegian Krone'), ('OMR', 'Omani Rial'), ('PKR', 'Pakistani Rupee'), ('XPD', 'Palladium'), ('PAB', 'Panamanian Balboa'), ('PGK', 'Papua New Guinean Kina'), ('PYG', 'Paraguayan Guarani'), ('PEI', 'Peruvian Inti'), ('PEN', 'Peruvian Sol'), ('PES', 'Peruvian Sol (1863–1965)'), ('PHP', 'Philippine Piso'), ('XPT', 'Platinum'), ('PLN', 'Polish Zloty'), ('PLZ', 'Polish Zloty (1950–1995)'), ('PTE', 'Portuguese Escudo'), ('GWE', 'Portuguese Guinea Escudo'), ('QAR', 'Qatari Rial'), ('XRE', 'RINET Funds'), ('RHD', 'Rhodesian Dollar'), ('RON', 'Romanian Leu'), ('ROL', 'Romanian Leu (1952–2006)'), ('RUB', 'Russian Ruble'), ('RUR', 'Russian Ruble (1991–1998)'), ('RWF', 'Rwandan Franc'), ('SVC', 'Salvadoran Colón'), ('WST', 'Samoan Tala'), ('SAR', 'Saudi Riyal'), ('RSD', 'Serbian Dinar'), ('CSD', 'Serbian Dinar (2002–2006)'), ('SCR', 'Seychellois Rupee'), ('SLL', 'Sierra Leonean Leone'), ('XAG', 'Silver'), ('SGD', 'Singapore Dollar'), ('SKK', 'Slovak Koruna'), ('SIT', 'Slovenian Tolar'), ('SBD', 'Solomon Islands Dollar'), ('SOS', 'Somali Shilling'), ('ZAR', 'South African Rand'), ('ZAL', 'South African Rand (financial)'), ('KRH', 'South Korean Hwan (1953–1962)'), ('KRW', 'South Korean Won'), ('KRO', 'South Korean Won (1945–1953)'), ('SSP', 'South Sudanese Pound'), ('SUR', 'Soviet Rouble'), ('ESP', 'Spanish Peseta'), ('ESA', 'Spanish Peseta (A account)'), ('ESB', 'Spanish Peseta (convertible account)'), ('XDR', 'Special Drawing Rights'), ('LKR', 'Sri Lankan Rupee'), ('SHP', 'St. Helena Pound'), ('XSU', 'Sucre'), ('SDD', 'Sudanese Dinar (1992–2007)'), ('SDG', 'Sudanese Pound'), ('SDP', 'Sudanese Pound (1957–1998)'), ('SRD', 'Surinamese Dollar'), ('SRG', 'Surinamese Guilder'), ('SZL', 'Swazi Lilangeni'), ('SEK', 'Swedish Krona'), ('CHF', 'Swiss Franc'), ('SYP', 'Syrian Pound'), ('STN', 'São Tomé & Príncipe Dobra'), ('STD', 'São Tomé & Príncipe Dobra (1977–2017)'), ('TVD', 'TVD'), ('TJR', 'Tajikistani Ruble'), ('TJS', 'Tajikistani Somoni'), ('TZS', 'Tanzanian Shilling'), ('XTS', 'Testing Currency Code'), ('THB', 'Thai Baht'), ('XXX', 'The codes assigned for transactions where no currency is involved'), ('TPE', 'Timorese Escudo'), ('TOP', 'Tongan Paʻanga'), ('TTD', 'Trinidad & Tobago Dollar'), ('TND', 'Tunisian Dinar'), ('TRY', 'Turkish Lira'), ('TRL', 'Turkish Lira (1922–2005)'), ('TMT', 'Turkmenistani Manat'), ('TMM', 'Turkmenistani Manat (1993–2009)'), ('USD', 'US Dollar'), ('USN', 'US Dollar (Next day)'), ('USS', 'US Dollar (Same day)'), ('UGX', 'Ugandan Shilling'), ('UGS', 'Ugandan Shilling (1966–1987)'), ('UAH', 'Ukrainian Hryvnia'), ('UAK', 'Ukrainian Karbovanets'), ('AED', 'United Arab Emirates Dirham'), ('UYW', 'Uruguayan Nominal Wage Index Unit'), ('UYU', 'Uruguayan Peso'), ('UYP', 'Uruguayan Peso (1975–1993)'), ('UYI', 'Uruguayan Peso (Indexed Units)'), ('UZS', 'Uzbekistani Som'), ('VUV', 'Vanuatu Vatu'), ('VES', 'Venezuelan Bolívar'), ('VEB', 'Venezuelan Bolívar (1871–2008)'), ('VEF', 'Venezuelan Bolívar (2008–2018)'), ('VND', 'Vietnamese Dong'), ('VNN', 'Vietnamese Dong (1978–1985)'), ('CHE', 'WIR Euro'), ('CHW', 'WIR Franc'), ('XOF', 'West African CFA Franc'), ('YDD', 'Yemeni Dinar'), ('YER', 'Yemeni Rial'), ('YUN', 'Yugoslavian Convertible Dinar (1990–1992)'), ('YUD', 'Yugoslavian Hard Dinar (1966–1990)'), ('YUM', 'Yugoslavian New Dinar (1994–2002)'), ('YUR', 'Yugoslavian Reformed Dinar (1992–1993)'), ('ZWN', 'ZWN'), ('ZRN', 'Zairean New Zaire (1993–1998)'), ('ZRZ', 'Zairean Zaire (1971–1993)'), ('ZMW', 'Zambian Kwacha'), ('ZMK', 'Zambian Kwacha (1968–2012)'), ('ZWD', 'Zimbabwean Dollar (1980–2008)'), ('ZWR', 'Zimbabwean Dollar (2008)'), ('ZWL', 'Zimbabwean Dollar (2009)')], default='USD', editable=False, max_length=3)),
-                ('amount', djmoney.models.fields.MoneyField(decimal_places=2, default_currency='USD', max_digits=14)),
-                ('created', models.DateTimeField(blank=True, editable=False)),
-                ('updated', models.DateTimeField(blank=True, editable=False)),
-                ('original_payment', models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, related_name='refunds', to='subscriptions.subscriptionpayment')),
-            ],
-            options={
-                'abstract': False,
-            },
+            name='id',
+            field=models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
+        ),
+        migrations.AlterField(
+            model_name='quota',
+            name='id',
+            field=models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
+        ),
+        migrations.AlterField(
+            model_name='resource',
+            name='id',
+            field=models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
+        ),
+        migrations.AlterField(
+            model_name='subscription',
+            name='id',
+            field=models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
+        ),
+        migrations.AlterField(
+            model_name='subscriptionpayment',
+            name='amount_currency',
+            field=djmoney.models.fields.CurrencyField(choices=[('XUA', 'ADB Unit of Account'), ('AFN', 'Afghan Afghani'), ('AFA', 'Afghan Afghani (1927–2002)'), ('ALL', 'Albanian Lek'), ('ALK', 'Albanian Lek (1946–1965)'), ('DZD', 'Algerian Dinar'), ('ADP', 'Andorran Peseta'), ('AOA', 'Angolan Kwanza'), ('AOK', 'Angolan Kwanza (1977–1991)'), ('AON', 'Angolan New Kwanza (1990–2000)'), ('AOR', 'Angolan Readjusted Kwanza (1995–1999)'), ('ARA', 'Argentine Austral'), ('ARS', 'Argentine Peso'), ('ARM', 'Argentine Peso (1881–1970)'), ('ARP', 'Argentine Peso (1983–1985)'), ('ARL', 'Argentine Peso Ley (1970–1983)'), ('AMD', 'Armenian Dram'), ('AWG', 'Aruban Florin'), ('AUD', 'Australian Dollar'), ('ATS', 'Austrian Schilling'), ('AZN', 'Azerbaijani Manat'), ('AZM', 'Azerbaijani Manat (1993–2006)'), ('BSD', 'Bahamian Dollar'), ('BHD', 'Bahraini Dinar'), ('BDT', 'Bangladeshi Taka'), ('BBD', 'Barbadian Dollar'), ('BYN', 'Belarusian Ruble'), ('BYB', 'Belarusian Ruble (1994–1999)'), ('BYR', 'Belarusian Ruble (2000–2016)'), ('BEF', 'Belgian Franc'), ('BEC', 'Belgian Franc (convertible)'), ('BEL', 'Belgian Franc (financial)'), ('BZD', 'Belize Dollar'), ('BMD', 'Bermudan Dollar'), ('BTN', 'Bhutanese Ngultrum'), ('BOB', 'Bolivian Boliviano'), ('BOL', 'Bolivian Boliviano (1863–1963)'), ('BOV', 'Bolivian Mvdol'), ('BOP', 'Bolivian Peso'), ('BAM', 'Bosnia-Herzegovina Convertible Mark'), ('BAD', 'Bosnia-Herzegovina Dinar (1992–1994)'), ('BAN', 'Bosnia-Herzegovina New Dinar (1994–1997)'), ('BWP', 'Botswanan Pula'), ('BRC', 'Brazilian Cruzado (1986–1989)'), ('BRZ', 'Brazilian Cruzeiro (1942–1967)'), ('BRE', 'Brazilian Cruzeiro (1990–1993)'), ('BRR', 'Brazilian Cruzeiro (1993–1994)'), ('BRN', 'Brazilian New Cruzado (1989–1990)'), ('BRB', 'Brazilian New Cruzeiro (1967–1986)'), ('BRL', 'Brazilian Real'), ('GBP', 'British Pound'), ('BND', 'Brunei Dollar'), ('BGL', 'Bulgarian Hard Lev'), ('BGN', 'Bulgarian Lev'), ('BGO', 'Bulgarian Lev (1879–1952)'), ('BGM', 'Bulgarian Socialist Lev'), ('BUK', 'Burmese Kyat'), ('BIF', 'Burundian Franc'), ('XPF', 'CFP Franc'), ('KHR', 'Cambodian Riel'), ('CAD', 'Canadian Dollar'), ('CVE', 'Cape Verdean Escudo'), ('KYD', 'Cayman Islands Dollar'), ('XAF', 'Central African CFA Franc'), ('CLE', 'Chilean Escudo'), ('CLP', 'Chilean Peso'), ('CLF', 'Chilean Unit of Account (UF)'), ('CNX', 'Chinese People’s Bank Dollar'), ('CNY', 'Chinese Yuan'), ('CNH', 'Chinese Yuan (offshore)'), ('COP', 'Colombian Peso'), ('COU', 'Colombian Real Value Unit'), ('KMF', 'Comorian Franc'), ('CDF', 'Congolese Franc'), ('CRC', 'Costa Rican Colón'), ('HRD', 'Croatian Dinar'), ('HRK', 'Croatian Kuna'), ('CUC', 'Cuban Convertible Peso'), ('CUP', 'Cuban Peso'), ('CYP', 'Cypriot Pound'), ('CZK', 'Czech Koruna'), ('CSK', 'Czechoslovak Hard Koruna'), ('DKK', 'Danish Krone'), ('DJF', 'Djiboutian Franc'), ('DOP', 'Dominican Peso'), ('NLG', 'Dutch Guilder'), ('XCD', 'East Caribbean Dollar'), ('DDM', 'East German Mark'), ('ECS', 'Ecuadorian Sucre'), ('ECV', 'Ecuadorian Unit of Constant Value'), ('EGP', 'Egyptian Pound'), ('GQE', 'Equatorial Guinean Ekwele'), ('ERN', 'Eritrean Nakfa'), ('EEK', 'Estonian Kroon'), ('ETB', 'Ethiopian Birr'), ('EUR', 'Euro'), ('XBA', 'European Composite Unit'), ('XEU', 'European Currency Unit'), ('XBB', 'European Monetary Unit'), ('XBC', 'European Unit of Account (XBC)'), ('XBD', 'European Unit of Account (XBD)'), ('FKP', 'Falkland Islands Pound'), ('FJD', 'Fijian Dollar'), ('FIM', 'Finnish Markka'), ('FRF', 'French Franc'), ('XFO', 'French Gold Franc'), ('XFU', 'French UIC-Franc'), ('GMD', 'Gambian Dalasi'), ('GEK', 'Georgian Kupon Larit'), ('GEL', 'Georgian Lari'), ('DEM', 'German Mark'), ('GHS', 'Ghanaian Cedi'), ('GHC', 'Ghanaian Cedi (1979–2007)'), ('GIP', 'Gibraltar Pound'), ('XAU', 'Gold'), ('GRD', 'Greek Drachma'), ('GTQ', 'Guatemalan Quetzal'), ('GWP', 'Guinea-Bissau Peso'), ('GNF', 'Guinean Franc'), ('GNS', 'Guinean Syli'), ('GYD', 'Guyanaese Dollar'), ('HTG', 'Haitian Gourde'), ('HNL', 'Honduran Lempira'), ('HKD', 'Hong Kong Dollar'), ('HUF', 'Hungarian Forint'), ('IMP', 'IMP'), ('ISK', 'Icelandic Króna'), ('ISJ', 'Icelandic Króna (1918–1981)'), ('INR', 'Indian Rupee'), ('IDR', 'Indonesian Rupiah'), ('IRR', 'Iranian Rial'), ('IQD', 'Iraqi Dinar'), ('IEP', 'Irish Pound'), ('ILS', 'Israeli New Shekel'), ('ILP', 'Israeli Pound'), ('ILR', 'Israeli Shekel (1980–1985)'), ('ITL', 'Italian Lira'), ('JMD', 'Jamaican Dollar'), ('JPY', 'Japanese Yen'), ('JOD', 'Jordanian Dinar'), ('KZT', 'Kazakhstani Tenge'), ('KES', 'Kenyan Shilling'), ('KWD', 'Kuwaiti Dinar'), ('KGS', 'Kyrgystani Som'), ('LAK', 'Laotian Kip'), ('LVL', 'Latvian Lats'), ('LVR', 'Latvian Ruble'), ('LBP', 'Lebanese Pound'), ('LSL', 'Lesotho Loti'), ('LRD', 'Liberian Dollar'), ('LYD', 'Libyan Dinar'), ('LTL', 'Lithuanian Litas'), ('LTT', 'Lithuanian Talonas'), ('LUL', 'Luxembourg Financial Franc'), ('LUC', 'Luxembourgian Convertible Franc'), ('LUF', 'Luxembourgian Franc'), ('MOP', 'Macanese Pataca'), ('MKD', 'Macedonian Denar'), ('MKN', 'Macedonian Denar (1992–1993)'), ('MGA', 'Malagasy Ariary'), ('MGF', 'Malagasy Franc'), ('MWK', 'Malawian Kwacha'), ('MYR', 'Malaysian Ringgit'), ('MVR', 'Maldivian Rufiyaa'), ('MVP', 'Maldivian Rupee (1947–1981)'), ('MLF', 'Malian Franc'), ('MTL', 'Maltese Lira'), ('MTP', 'Maltese Pound'), ('MRU', 'Mauritanian Ouguiya'), ('MRO', 'Mauritanian Ouguiya (1973–2017)'), ('MUR', 'Mauritian Rupee'), ('MXV', 'Mexican Investment Unit'), ('MXN', 'Mexican Peso'), ('MXP', 'Mexican Silver Peso (1861–1992)'), ('MDC', 'Moldovan Cupon'), ('MDL', 'Moldovan Leu'), ('MCF', 'Monegasque Franc'), ('MNT', 'Mongolian Tugrik'), ('MAD', 'Moroccan Dirham'), ('MAF', 'Moroccan Franc'), ('MZE', 'Mozambican Escudo'), ('MZN', 'Mozambican Metical'), ('MZM', 'Mozambican Metical (1980–2006)'), ('MMK', 'Myanmar Kyat'), ('NAD', 'Namibian Dollar'), ('NPR', 'Nepalese Rupee'), ('ANG', 'Netherlands Antillean Guilder'), ('TWD', 'New Taiwan Dollar'), ('NZD', 'New Zealand Dollar'), ('NIO', 'Nicaraguan Córdoba'), ('NIC', 'Nicaraguan Córdoba (1988–1991)'), ('NGN', 'Nigerian Naira'), ('KPW', 'North Korean Won'), ('NOK', 'Norwegian Krone'), ('OMR', 'Omani Rial'), ('PKR', 'Pakistani Rupee'), ('XPD', 'Palladium'), ('PAB', 'Panamanian Balboa'), ('PGK', 'Papua New Guinean Kina'), ('PYG', 'Paraguayan Guarani'), ('PEI', 'Peruvian Inti'), ('PEN', 'Peruvian Sol'), ('PES', 'Peruvian Sol (1863–1965)'), ('PHP', 'Philippine Peso'), ('XPT', 'Platinum'), ('PLN', 'Polish Zloty'), ('PLZ', 'Polish Zloty (1950–1995)'), ('PTE', 'Portuguese Escudo'), ('GWE', 'Portuguese Guinea Escudo'), ('QAR', 'Qatari Rial'), ('XRE', 'RINET Funds'), ('RHD', 'Rhodesian Dollar'), ('RON', 'Romanian Leu'), ('ROL', 'Romanian Leu (1952–2006)'), ('RUB', 'Russian Ruble'), ('RUR', 'Russian Ruble (1991–1998)'), ('RWF', 'Rwandan Franc'), ('SVC', 'Salvadoran Colón'), ('WST', 'Samoan Tala'), ('SAR', 'Saudi Riyal'), ('RSD', 'Serbian Dinar'), ('CSD', 'Serbian Dinar (2002–2006)'), ('SCR', 'Seychellois Rupee'), ('SLL', 'Sierra Leonean Leone'), ('XAG', 'Silver'), ('SGD', 'Singapore Dollar'), ('SKK', 'Slovak Koruna'), ('SIT', 'Slovenian Tolar'), ('SBD', 'Solomon Islands Dollar'), ('SOS', 'Somali Shilling'), ('ZAR', 'South African Rand'), ('ZAL', 'South African Rand (financial)'), ('KRH', 'South Korean Hwan (1953–1962)'), ('KRW', 'South Korean Won'), ('KRO', 'South Korean Won (1945–1953)'), ('SSP', 'South Sudanese Pound'), ('SUR', 'Soviet Rouble'), ('ESP', 'Spanish Peseta'), ('ESA', 'Spanish Peseta (A account)'), ('ESB', 'Spanish Peseta (convertible account)'), ('XDR', 'Special Drawing Rights'), ('LKR', 'Sri Lankan Rupee'), ('SHP', 'St. Helena Pound'), ('XSU', 'Sucre'), ('SDD', 'Sudanese Dinar (1992–2007)'), ('SDG', 'Sudanese Pound'), ('SDP', 'Sudanese Pound (1957–1998)'), ('SRD', 'Surinamese Dollar'), ('SRG', 'Surinamese Guilder'), ('SZL', 'Swazi Lilangeni'), ('SEK', 'Swedish Krona'), ('CHF', 'Swiss Franc'), ('SYP', 'Syrian Pound'), ('STN', 'São Tomé & Príncipe Dobra'), ('STD', 'São Tomé & Príncipe Dobra (1977–2017)'), ('TVD', 'TVD'), ('TJR', 'Tajikistani Ruble'), ('TJS', 'Tajikistani Somoni'), ('TZS', 'Tanzanian Shilling'), ('XTS', 'Testing Currency Code'), ('THB', 'Thai Baht'), ('XXX', 'The codes assigned for transactions where no currency is involved'), ('TPE', 'Timorese Escudo'), ('TOP', 'Tongan Paʻanga'), ('TTD', 'Trinidad & Tobago Dollar'), ('TND', 'Tunisian Dinar'), ('TRY', 'Turkish Lira'), ('TRL', 'Turkish Lira (1922–2005)'), ('TMT', 'Turkmenistani Manat'), ('TMM', 'Turkmenistani Manat (1993–2009)'), ('USD', 'US Dollar'), ('USN', 'US Dollar (Next day)'), ('USS', 'US Dollar (Same day)'), ('UGX', 'Ugandan Shilling'), ('UGS', 'Ugandan Shilling (1966–1987)'), ('UAH', 'Ukrainian Hryvnia'), ('UAK', 'Ukrainian Karbovanets'), ('AED', 'United Arab Emirates Dirham'), ('UYW', 'Uruguayan Nominal Wage Index Unit'), ('UYU', 'Uruguayan Peso'), ('UYP', 'Uruguayan Peso (1975–1993)'), ('UYI', 'Uruguayan Peso (Indexed Units)'), ('UZS', 'Uzbekistani Som'), ('VUV', 'Vanuatu Vatu'), ('VES', 'Venezuelan Bolívar'), ('VEB', 'Venezuelan Bolívar (1871–2008)'), ('VEF', 'Venezuelan Bolívar (2008–2018)'), ('VND', 'Vietnamese Dong'), ('VNN', 'Vietnamese Dong (1978–1985)'), ('CHE', 'WIR Euro'), ('CHW', 'WIR Franc'), ('XOF', 'West African CFA Franc'), ('YDD', 'Yemeni Dinar'), ('YER', 'Yemeni Rial'), ('YUN', 'Yugoslavian Convertible Dinar (1990–1992)'), ('YUD', 'Yugoslavian Hard Dinar (1966–1990)'), ('YUM', 'Yugoslavian New Dinar (1994–2002)'), ('YUR', 'Yugoslavian Reformed Dinar (1992–1993)'), ('ZWN', 'ZWN'), ('ZRN', 'Zairean New Zaire (1993–1998)'), ('ZRZ', 'Zairean Zaire (1971–1993)'), ('ZMW', 'Zambian Kwacha'), ('ZMK', 'Zambian Kwacha (1968–2012)'), ('ZWD', 'Zimbabwean Dollar (1980–2008)'), ('ZWR', 'Zimbabwean Dollar (2008)'), ('ZWL', 'Zimbabwean Dollar (2009)')], default='USD', editable=False, max_length=3),
+        ),
+        migrations.AlterField(
+            model_name='subscriptionpayment',
+            name='id',
+            field=models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
+        ),
+        migrations.AlterField(
+            model_name='subscriptionpaymentrefund',
+            name='amount_currency',
+            field=djmoney.models.fields.CurrencyField(choices=[('XUA', 'ADB Unit of Account'), ('AFN', 'Afghan Afghani'), ('AFA', 'Afghan Afghani (1927–2002)'), ('ALL', 'Albanian Lek'), ('ALK', 'Albanian Lek (1946–1965)'), ('DZD', 'Algerian Dinar'), ('ADP', 'Andorran Peseta'), ('AOA', 'Angolan Kwanza'), ('AOK', 'Angolan Kwanza (1977–1991)'), ('AON', 'Angolan New Kwanza (1990–2000)'), ('AOR', 'Angolan Readjusted Kwanza (1995–1999)'), ('ARA', 'Argentine Austral'), ('ARS', 'Argentine Peso'), ('ARM', 'Argentine Peso (1881–1970)'), ('ARP', 'Argentine Peso (1983–1985)'), ('ARL', 'Argentine Peso Ley (1970–1983)'), ('AMD', 'Armenian Dram'), ('AWG', 'Aruban Florin'), ('AUD', 'Australian Dollar'), ('ATS', 'Austrian Schilling'), ('AZN', 'Azerbaijani Manat'), ('AZM', 'Azerbaijani Manat (1993–2006)'), ('BSD', 'Bahamian Dollar'), ('BHD', 'Bahraini Dinar'), ('BDT', 'Bangladeshi Taka'), ('BBD', 'Barbadian Dollar'), ('BYN', 'Belarusian Ruble'), ('BYB', 'Belarusian Ruble (1994–1999)'), ('BYR', 'Belarusian Ruble (2000–2016)'), ('BEF', 'Belgian Franc'), ('BEC', 'Belgian Franc (convertible)'), ('BEL', 'Belgian Franc (financial)'), ('BZD', 'Belize Dollar'), ('BMD', 'Bermudan Dollar'), ('BTN', 'Bhutanese Ngultrum'), ('BOB', 'Bolivian Boliviano'), ('BOL', 'Bolivian Boliviano (1863–1963)'), ('BOV', 'Bolivian Mvdol'), ('BOP', 'Bolivian Peso'), ('BAM', 'Bosnia-Herzegovina Convertible Mark'), ('BAD', 'Bosnia-Herzegovina Dinar (1992–1994)'), ('BAN', 'Bosnia-Herzegovina New Dinar (1994–1997)'), ('BWP', 'Botswanan Pula'), ('BRC', 'Brazilian Cruzado (1986–1989)'), ('BRZ', 'Brazilian Cruzeiro (1942–1967)'), ('BRE', 'Brazilian Cruzeiro (1990–1993)'), ('BRR', 'Brazilian Cruzeiro (1993–1994)'), ('BRN', 'Brazilian New Cruzado (1989–1990)'), ('BRB', 'Brazilian New Cruzeiro (1967–1986)'), ('BRL', 'Brazilian Real'), ('GBP', 'British Pound'), ('BND', 'Brunei Dollar'), ('BGL', 'Bulgarian Hard Lev'), ('BGN', 'Bulgarian Lev'), ('BGO', 'Bulgarian Lev (1879–1952)'), ('BGM', 'Bulgarian Socialist Lev'), ('BUK', 'Burmese Kyat'), ('BIF', 'Burundian Franc'), ('XPF', 'CFP Franc'), ('KHR', 'Cambodian Riel'), ('CAD', 'Canadian Dollar'), ('CVE', 'Cape Verdean Escudo'), ('KYD', 'Cayman Islands Dollar'), ('XAF', 'Central African CFA Franc'), ('CLE', 'Chilean Escudo'), ('CLP', 'Chilean Peso'), ('CLF', 'Chilean Unit of Account (UF)'), ('CNX', 'Chinese People’s Bank Dollar'), ('CNY', 'Chinese Yuan'), ('CNH', 'Chinese Yuan (offshore)'), ('COP', 'Colombian Peso'), ('COU', 'Colombian Real Value Unit'), ('KMF', 'Comorian Franc'), ('CDF', 'Congolese Franc'), ('CRC', 'Costa Rican Colón'), ('HRD', 'Croatian Dinar'), ('HRK', 'Croatian Kuna'), ('CUC', 'Cuban Convertible Peso'), ('CUP', 'Cuban Peso'), ('CYP', 'Cypriot Pound'), ('CZK', 'Czech Koruna'), ('CSK', 'Czechoslovak Hard Koruna'), ('DKK', 'Danish Krone'), ('DJF', 'Djiboutian Franc'), ('DOP', 'Dominican Peso'), ('NLG', 'Dutch Guilder'), ('XCD', 'East Caribbean Dollar'), ('DDM', 'East German Mark'), ('ECS', 'Ecuadorian Sucre'), ('ECV', 'Ecuadorian Unit of Constant Value'), ('EGP', 'Egyptian Pound'), ('GQE', 'Equatorial Guinean Ekwele'), ('ERN', 'Eritrean Nakfa'), ('EEK', 'Estonian Kroon'), ('ETB', 'Ethiopian Birr'), ('EUR', 'Euro'), ('XBA', 'European Composite Unit'), ('XEU', 'European Currency Unit'), ('XBB', 'European Monetary Unit'), ('XBC', 'European Unit of Account (XBC)'), ('XBD', 'European Unit of Account (XBD)'), ('FKP', 'Falkland Islands Pound'), ('FJD', 'Fijian Dollar'), ('FIM', 'Finnish Markka'), ('FRF', 'French Franc'), ('XFO', 'French Gold Franc'), ('XFU', 'French UIC-Franc'), ('GMD', 'Gambian Dalasi'), ('GEK', 'Georgian Kupon Larit'), ('GEL', 'Georgian Lari'), ('DEM', 'German Mark'), ('GHS', 'Ghanaian Cedi'), ('GHC', 'Ghanaian Cedi (1979–2007)'), ('GIP', 'Gibraltar Pound'), ('XAU', 'Gold'), ('GRD', 'Greek Drachma'), ('GTQ', 'Guatemalan Quetzal'), ('GWP', 'Guinea-Bissau Peso'), ('GNF', 'Guinean Franc'), ('GNS', 'Guinean Syli'), ('GYD', 'Guyanaese Dollar'), ('HTG', 'Haitian Gourde'), ('HNL', 'Honduran Lempira'), ('HKD', 'Hong Kong Dollar'), ('HUF', 'Hungarian Forint'), ('IMP', 'IMP'), ('ISK', 'Icelandic Króna'), ('ISJ', 'Icelandic Króna (1918–1981)'), ('INR', 'Indian Rupee'), ('IDR', 'Indonesian Rupiah'), ('IRR', 'Iranian Rial'), ('IQD', 'Iraqi Dinar'), ('IEP', 'Irish Pound'), ('ILS', 'Israeli New Shekel'), ('ILP', 'Israeli Pound'), ('ILR', 'Israeli Shekel (1980–1985)'), ('ITL', 'Italian Lira'), ('JMD', 'Jamaican Dollar'), ('JPY', 'Japanese Yen'), ('JOD', 'Jordanian Dinar'), ('KZT', 'Kazakhstani Tenge'), ('KES', 'Kenyan Shilling'), ('KWD', 'Kuwaiti Dinar'), ('KGS', 'Kyrgystani Som'), ('LAK', 'Laotian Kip'), ('LVL', 'Latvian Lats'), ('LVR', 'Latvian Ruble'), ('LBP', 'Lebanese Pound'), ('LSL', 'Lesotho Loti'), ('LRD', 'Liberian Dollar'), ('LYD', 'Libyan Dinar'), ('LTL', 'Lithuanian Litas'), ('LTT', 'Lithuanian Talonas'), ('LUL', 'Luxembourg Financial Franc'), ('LUC', 'Luxembourgian Convertible Franc'), ('LUF', 'Luxembourgian Franc'), ('MOP', 'Macanese Pataca'), ('MKD', 'Macedonian Denar'), ('MKN', 'Macedonian Denar (1992–1993)'), ('MGA', 'Malagasy Ariary'), ('MGF', 'Malagasy Franc'), ('MWK', 'Malawian Kwacha'), ('MYR', 'Malaysian Ringgit'), ('MVR', 'Maldivian Rufiyaa'), ('MVP', 'Maldivian Rupee (1947–1981)'), ('MLF', 'Malian Franc'), ('MTL', 'Maltese Lira'), ('MTP', 'Maltese Pound'), ('MRU', 'Mauritanian Ouguiya'), ('MRO', 'Mauritanian Ouguiya (1973–2017)'), ('MUR', 'Mauritian Rupee'), ('MXV', 'Mexican Investment Unit'), ('MXN', 'Mexican Peso'), ('MXP', 'Mexican Silver Peso (1861–1992)'), ('MDC', 'Moldovan Cupon'), ('MDL', 'Moldovan Leu'), ('MCF', 'Monegasque Franc'), ('MNT', 'Mongolian Tugrik'), ('MAD', 'Moroccan Dirham'), ('MAF', 'Moroccan Franc'), ('MZE', 'Mozambican Escudo'), ('MZN', 'Mozambican Metical'), ('MZM', 'Mozambican Metical (1980–2006)'), ('MMK', 'Myanmar Kyat'), ('NAD', 'Namibian Dollar'), ('NPR', 'Nepalese Rupee'), ('ANG', 'Netherlands Antillean Guilder'), ('TWD', 'New Taiwan Dollar'), ('NZD', 'New Zealand Dollar'), ('NIO', 'Nicaraguan Córdoba'), ('NIC', 'Nicaraguan Córdoba (1988–1991)'), ('NGN', 'Nigerian Naira'), ('KPW', 'North Korean Won'), ('NOK', 'Norwegian Krone'), ('OMR', 'Omani Rial'), ('PKR', 'Pakistani Rupee'), ('XPD', 'Palladium'), ('PAB', 'Panamanian Balboa'), ('PGK', 'Papua New Guinean Kina'), ('PYG', 'Paraguayan Guarani'), ('PEI', 'Peruvian Inti'), ('PEN', 'Peruvian Sol'), ('PES', 'Peruvian Sol (1863–1965)'), ('PHP', 'Philippine Peso'), ('XPT', 'Platinum'), ('PLN', 'Polish Zloty'), ('PLZ', 'Polish Zloty (1950–1995)'), ('PTE', 'Portuguese Escudo'), ('GWE', 'Portuguese Guinea Escudo'), ('QAR', 'Qatari Rial'), ('XRE', 'RINET Funds'), ('RHD', 'Rhodesian Dollar'), ('RON', 'Romanian Leu'), ('ROL', 'Romanian Leu (1952–2006)'), ('RUB', 'Russian Ruble'), ('RUR', 'Russian Ruble (1991–1998)'), ('RWF', 'Rwandan Franc'), ('SVC', 'Salvadoran Colón'), ('WST', 'Samoan Tala'), ('SAR', 'Saudi Riyal'), ('RSD', 'Serbian Dinar'), ('CSD', 'Serbian Dinar (2002–2006)'), ('SCR', 'Seychellois Rupee'), ('SLL', 'Sierra Leonean Leone'), ('XAG', 'Silver'), ('SGD', 'Singapore Dollar'), ('SKK', 'Slovak Koruna'), ('SIT', 'Slovenian Tolar'), ('SBD', 'Solomon Islands Dollar'), ('SOS', 'Somali Shilling'), ('ZAR', 'South African Rand'), ('ZAL', 'South African Rand (financial)'), ('KRH', 'South Korean Hwan (1953–1962)'), ('KRW', 'South Korean Won'), ('KRO', 'South Korean Won (1945–1953)'), ('SSP', 'South Sudanese Pound'), ('SUR', 'Soviet Rouble'), ('ESP', 'Spanish Peseta'), ('ESA', 'Spanish Peseta (A account)'), ('ESB', 'Spanish Peseta (convertible account)'), ('XDR', 'Special Drawing Rights'), ('LKR', 'Sri Lankan Rupee'), ('SHP', 'St. Helena Pound'), ('XSU', 'Sucre'), ('SDD', 'Sudanese Dinar (1992–2007)'), ('SDG', 'Sudanese Pound'), ('SDP', 'Sudanese Pound (1957–1998)'), ('SRD', 'Surinamese Dollar'), ('SRG', 'Surinamese Guilder'), ('SZL', 'Swazi Lilangeni'), ('SEK', 'Swedish Krona'), ('CHF', 'Swiss Franc'), ('SYP', 'Syrian Pound'), ('STN', 'São Tomé & Príncipe Dobra'), ('STD', 'São Tomé & Príncipe Dobra (1977–2017)'), ('TVD', 'TVD'), ('TJR', 'Tajikistani Ruble'), ('TJS', 'Tajikistani Somoni'), ('TZS', 'Tanzanian Shilling'), ('XTS', 'Testing Currency Code'), ('THB', 'Thai Baht'), ('XXX', 'The codes assigned for transactions where no currency is involved'), ('TPE', 'Timorese Escudo'), ('TOP', 'Tongan Paʻanga'), ('TTD', 'Trinidad & Tobago Dollar'), ('TND', 'Tunisian Dinar'), ('TRY', 'Turkish Lira'), ('TRL', 'Turkish Lira (1922–2005)'), ('TMT', 'Turkmenistani Manat'), ('TMM', 'Turkmenistani Manat (1993–2009)'), ('USD', 'US Dollar'), ('USN', 'US Dollar (Next day)'), ('USS', 'US Dollar (Same day)'), ('UGX', 'Ugandan Shilling'), ('UGS', 'Ugandan Shilling (1966–1987)'), ('UAH', 'Ukrainian Hryvnia'), ('UAK', 'Ukrainian Karbovanets'), ('AED', 'United Arab Emirates Dirham'), ('UYW', 'Uruguayan Nominal Wage Index Unit'), ('UYU', 'Uruguayan Peso'), ('UYP', 'Uruguayan Peso (1975–1993)'), ('UYI', 'Uruguayan Peso (Indexed Units)'), ('UZS', 'Uzbekistani Som'), ('VUV', 'Vanuatu Vatu'), ('VES', 'Venezuelan Bolívar'), ('VEB', 'Venezuelan Bolívar (1871–2008)'), ('VEF', 'Venezuelan Bolívar (2008–2018)'), ('VND', 'Vietnamese Dong'), ('VNN', 'Vietnamese Dong (1978–1985)'), ('CHE', 'WIR Euro'), ('CHW', 'WIR Franc'), ('XOF', 'West African CFA Franc'), ('YDD', 'Yemeni Dinar'), ('YER', 'Yemeni Rial'), ('YUN', 'Yugoslavian Convertible Dinar (1990–1992)'), ('YUD', 'Yugoslavian Hard Dinar (1966–1990)'), ('YUM', 'Yugoslavian New Dinar (1994–2002)'), ('YUR', 'Yugoslavian Reformed Dinar (1992–1993)'), ('ZWN', 'ZWN'), ('ZRN', 'Zairean New Zaire (1993–1998)'), ('ZRZ', 'Zairean Zaire (1971–1993)'), ('ZMW', 'Zambian Kwacha'), ('ZMK', 'Zambian Kwacha (1968–2012)'), ('ZWD', 'Zimbabwean Dollar (1980–2008)'), ('ZWR', 'Zimbabwean Dollar (2008)'), ('ZWL', 'Zimbabwean Dollar (2009)')], default='USD', editable=False, max_length=3),
+        ),
+        migrations.AlterField(
+            model_name='subscriptionpaymentrefund',
+            name='id',
+            field=models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
+        ),
+        migrations.AlterField(
+            model_name='tax',
+            name='amount_currency',
+            field=djmoney.models.fields.CurrencyField(choices=[('XUA', 'ADB Unit of Account'), ('AFN', 'Afghan Afghani'), ('AFA', 'Afghan Afghani (1927–2002)'), ('ALL', 'Albanian Lek'), ('ALK', 'Albanian Lek (1946–1965)'), ('DZD', 'Algerian Dinar'), ('ADP', 'Andorran Peseta'), ('AOA', 'Angolan Kwanza'), ('AOK', 'Angolan Kwanza (1977–1991)'), ('AON', 'Angolan New Kwanza (1990–2000)'), ('AOR', 'Angolan Readjusted Kwanza (1995–1999)'), ('ARA', 'Argentine Austral'), ('ARS', 'Argentine Peso'), ('ARM', 'Argentine Peso (1881–1970)'), ('ARP', 'Argentine Peso (1983–1985)'), ('ARL', 'Argentine Peso Ley (1970–1983)'), ('AMD', 'Armenian Dram'), ('AWG', 'Aruban Florin'), ('AUD', 'Australian Dollar'), ('ATS', 'Austrian Schilling'), ('AZN', 'Azerbaijani Manat'), ('AZM', 'Azerbaijani Manat (1993–2006)'), ('BSD', 'Bahamian Dollar'), ('BHD', 'Bahraini Dinar'), ('BDT', 'Bangladeshi Taka'), ('BBD', 'Barbadian Dollar'), ('BYN', 'Belarusian Ruble'), ('BYB', 'Belarusian Ruble (1994–1999)'), ('BYR', 'Belarusian Ruble (2000–2016)'), ('BEF', 'Belgian Franc'), ('BEC', 'Belgian Franc (convertible)'), ('BEL', 'Belgian Franc (financial)'), ('BZD', 'Belize Dollar'), ('BMD', 'Bermudan Dollar'), ('BTN', 'Bhutanese Ngultrum'), ('BOB', 'Bolivian Boliviano'), ('BOL', 'Bolivian Boliviano (1863–1963)'), ('BOV', 'Bolivian Mvdol'), ('BOP', 'Bolivian Peso'), ('BAM', 'Bosnia-Herzegovina Convertible Mark'), ('BAD', 'Bosnia-Herzegovina Dinar (1992–1994)'), ('BAN', 'Bosnia-Herzegovina New Dinar (1994–1997)'), ('BWP', 'Botswanan Pula'), ('BRC', 'Brazilian Cruzado (1986–1989)'), ('BRZ', 'Brazilian Cruzeiro (1942–1967)'), ('BRE', 'Brazilian Cruzeiro (1990–1993)'), ('BRR', 'Brazilian Cruzeiro (1993–1994)'), ('BRN', 'Brazilian New Cruzado (1989–1990)'), ('BRB', 'Brazilian New Cruzeiro (1967–1986)'), ('BRL', 'Brazilian Real'), ('GBP', 'British Pound'), ('BND', 'Brunei Dollar'), ('BGL', 'Bulgarian Hard Lev'), ('BGN', 'Bulgarian Lev'), ('BGO', 'Bulgarian Lev (1879–1952)'), ('BGM', 'Bulgarian Socialist Lev'), ('BUK', 'Burmese Kyat'), ('BIF', 'Burundian Franc'), ('XPF', 'CFP Franc'), ('KHR', 'Cambodian Riel'), ('CAD', 'Canadian Dollar'), ('CVE', 'Cape Verdean Escudo'), ('KYD', 'Cayman Islands Dollar'), ('XAF', 'Central African CFA Franc'), ('CLE', 'Chilean Escudo'), ('CLP', 'Chilean Peso'), ('CLF', 'Chilean Unit of Account (UF)'), ('CNX', 'Chinese People’s Bank Dollar'), ('CNY', 'Chinese Yuan'), ('CNH', 'Chinese Yuan (offshore)'), ('COP', 'Colombian Peso'), ('COU', 'Colombian Real Value Unit'), ('KMF', 'Comorian Franc'), ('CDF', 'Congolese Franc'), ('CRC', 'Costa Rican Colón'), ('HRD', 'Croatian Dinar'), ('HRK', 'Croatian Kuna'), ('CUC', 'Cuban Convertible Peso'), ('CUP', 'Cuban Peso'), ('CYP', 'Cypriot Pound'), ('CZK', 'Czech Koruna'), ('CSK', 'Czechoslovak Hard Koruna'), ('DKK', 'Danish Krone'), ('DJF', 'Djiboutian Franc'), ('DOP', 'Dominican Peso'), ('NLG', 'Dutch Guilder'), ('XCD', 'East Caribbean Dollar'), ('DDM', 'East German Mark'), ('ECS', 'Ecuadorian Sucre'), ('ECV', 'Ecuadorian Unit of Constant Value'), ('EGP', 'Egyptian Pound'), ('GQE', 'Equatorial Guinean Ekwele'), ('ERN', 'Eritrean Nakfa'), ('EEK', 'Estonian Kroon'), ('ETB', 'Ethiopian Birr'), ('EUR', 'Euro'), ('XBA', 'European Composite Unit'), ('XEU', 'European Currency Unit'), ('XBB', 'European Monetary Unit'), ('XBC', 'European Unit of Account (XBC)'), ('XBD', 'European Unit of Account (XBD)'), ('FKP', 'Falkland Islands Pound'), ('FJD', 'Fijian Dollar'), ('FIM', 'Finnish Markka'), ('FRF', 'French Franc'), ('XFO', 'French Gold Franc'), ('XFU', 'French UIC-Franc'), ('GMD', 'Gambian Dalasi'), ('GEK', 'Georgian Kupon Larit'), ('GEL', 'Georgian Lari'), ('DEM', 'German Mark'), ('GHS', 'Ghanaian Cedi'), ('GHC', 'Ghanaian Cedi (1979–2007)'), ('GIP', 'Gibraltar Pound'), ('XAU', 'Gold'), ('GRD', 'Greek Drachma'), ('GTQ', 'Guatemalan Quetzal'), ('GWP', 'Guinea-Bissau Peso'), ('GNF', 'Guinean Franc'), ('GNS', 'Guinean Syli'), ('GYD', 'Guyanaese Dollar'), ('HTG', 'Haitian Gourde'), ('HNL', 'Honduran Lempira'), ('HKD', 'Hong Kong Dollar'), ('HUF', 'Hungarian Forint'), ('IMP', 'IMP'), ('ISK', 'Icelandic Króna'), ('ISJ', 'Icelandic Króna (1918–1981)'), ('INR', 'Indian Rupee'), ('IDR', 'Indonesian Rupiah'), ('IRR', 'Iranian Rial'), ('IQD', 'Iraqi Dinar'), ('IEP', 'Irish Pound'), ('ILS', 'Israeli New Shekel'), ('ILP', 'Israeli Pound'), ('ILR', 'Israeli Shekel (1980–1985)'), ('ITL', 'Italian Lira'), ('JMD', 'Jamaican Dollar'), ('JPY', 'Japanese Yen'), ('JOD', 'Jordanian Dinar'), ('KZT', 'Kazakhstani Tenge'), ('KES', 'Kenyan Shilling'), ('KWD', 'Kuwaiti Dinar'), ('KGS', 'Kyrgystani Som'), ('LAK', 'Laotian Kip'), ('LVL', 'Latvian Lats'), ('LVR', 'Latvian Ruble'), ('LBP', 'Lebanese Pound'), ('LSL', 'Lesotho Loti'), ('LRD', 'Liberian Dollar'), ('LYD', 'Libyan Dinar'), ('LTL', 'Lithuanian Litas'), ('LTT', 'Lithuanian Talonas'), ('LUL', 'Luxembourg Financial Franc'), ('LUC', 'Luxembourgian Convertible Franc'), ('LUF', 'Luxembourgian Franc'), ('MOP', 'Macanese Pataca'), ('MKD', 'Macedonian Denar'), ('MKN', 'Macedonian Denar (1992–1993)'), ('MGA', 'Malagasy Ariary'), ('MGF', 'Malagasy Franc'), ('MWK', 'Malawian Kwacha'), ('MYR', 'Malaysian Ringgit'), ('MVR', 'Maldivian Rufiyaa'), ('MVP', 'Maldivian Rupee (1947–1981)'), ('MLF', 'Malian Franc'), ('MTL', 'Maltese Lira'), ('MTP', 'Maltese Pound'), ('MRU', 'Mauritanian Ouguiya'), ('MRO', 'Mauritanian Ouguiya (1973–2017)'), ('MUR', 'Mauritian Rupee'), ('MXV', 'Mexican Investment Unit'), ('MXN', 'Mexican Peso'), ('MXP', 'Mexican Silver Peso (1861–1992)'), ('MDC', 'Moldovan Cupon'), ('MDL', 'Moldovan Leu'), ('MCF', 'Monegasque Franc'), ('MNT', 'Mongolian Tugrik'), ('MAD', 'Moroccan Dirham'), ('MAF', 'Moroccan Franc'), ('MZE', 'Mozambican Escudo'), ('MZN', 'Mozambican Metical'), ('MZM', 'Mozambican Metical (1980–2006)'), ('MMK', 'Myanmar Kyat'), ('NAD', 'Namibian Dollar'), ('NPR', 'Nepalese Rupee'), ('ANG', 'Netherlands Antillean Guilder'), ('TWD', 'New Taiwan Dollar'), ('NZD', 'New Zealand Dollar'), ('NIO', 'Nicaraguan Córdoba'), ('NIC', 'Nicaraguan Córdoba (1988–1991)'), ('NGN', 'Nigerian Naira'), ('KPW', 'North Korean Won'), ('NOK', 'Norwegian Krone'), ('OMR', 'Omani Rial'), ('PKR', 'Pakistani Rupee'), ('XPD', 'Palladium'), ('PAB', 'Panamanian Balboa'), ('PGK', 'Papua New Guinean Kina'), ('PYG', 'Paraguayan Guarani'), ('PEI', 'Peruvian Inti'), ('PEN', 'Peruvian Sol'), ('PES', 'Peruvian Sol (1863–1965)'), ('PHP', 'Philippine Peso'), ('XPT', 'Platinum'), ('PLN', 'Polish Zloty'), ('PLZ', 'Polish Zloty (1950–1995)'), ('PTE', 'Portuguese Escudo'), ('GWE', 'Portuguese Guinea Escudo'), ('QAR', 'Qatari Rial'), ('XRE', 'RINET Funds'), ('RHD', 'Rhodesian Dollar'), ('RON', 'Romanian Leu'), ('ROL', 'Romanian Leu (1952–2006)'), ('RUB', 'Russian Ruble'), ('RUR', 'Russian Ruble (1991–1998)'), ('RWF', 'Rwandan Franc'), ('SVC', 'Salvadoran Colón'), ('WST', 'Samoan Tala'), ('SAR', 'Saudi Riyal'), ('RSD', 'Serbian Dinar'), ('CSD', 'Serbian Dinar (2002–2006)'), ('SCR', 'Seychellois Rupee'), ('SLL', 'Sierra Leonean Leone'), ('XAG', 'Silver'), ('SGD', 'Singapore Dollar'), ('SKK', 'Slovak Koruna'), ('SIT', 'Slovenian Tolar'), ('SBD', 'Solomon Islands Dollar'), ('SOS', 'Somali Shilling'), ('ZAR', 'South African Rand'), ('ZAL', 'South African Rand (financial)'), ('KRH', 'South Korean Hwan (1953–1962)'), ('KRW', 'South Korean Won'), ('KRO', 'South Korean Won (1945–1953)'), ('SSP', 'South Sudanese Pound'), ('SUR', 'Soviet Rouble'), ('ESP', 'Spanish Peseta'), ('ESA', 'Spanish Peseta (A account)'), ('ESB', 'Spanish Peseta (convertible account)'), ('XDR', 'Special Drawing Rights'), ('LKR', 'Sri Lankan Rupee'), ('SHP', 'St. Helena Pound'), ('XSU', 'Sucre'), ('SDD', 'Sudanese Dinar (1992–2007)'), ('SDG', 'Sudanese Pound'), ('SDP', 'Sudanese Pound (1957–1998)'), ('SRD', 'Surinamese Dollar'), ('SRG', 'Surinamese Guilder'), ('SZL', 'Swazi Lilangeni'), ('SEK', 'Swedish Krona'), ('CHF', 'Swiss Franc'), ('SYP', 'Syrian Pound'), ('STN', 'São Tomé & Príncipe Dobra'), ('STD', 'São Tomé & Príncipe Dobra (1977–2017)'), ('TVD', 'TVD'), ('TJR', 'Tajikistani Ruble'), ('TJS', 'Tajikistani Somoni'), ('TZS', 'Tanzanian Shilling'), ('XTS', 'Testing Currency Code'), ('THB', 'Thai Baht'), ('XXX', 'The codes assigned for transactions where no currency is involved'), ('TPE', 'Timorese Escudo'), ('TOP', 'Tongan Paʻanga'), ('TTD', 'Trinidad & Tobago Dollar'), ('TND', 'Tunisian Dinar'), ('TRY', 'Turkish Lira'), ('TRL', 'Turkish Lira (1922–2005)'), ('TMT', 'Turkmenistani Manat'), ('TMM', 'Turkmenistani Manat (1993–2009)'), ('USD', 'US Dollar'), ('USN', 'US Dollar (Next day)'), ('USS', 'US Dollar (Same day)'), ('UGX', 'Ugandan Shilling'), ('UGS', 'Ugandan Shilling (1966–1987)'), ('UAH', 'Ukrainian Hryvnia'), ('UAK', 'Ukrainian Karbovanets'), ('AED', 'United Arab Emirates Dirham'), ('UYW', 'Uruguayan Nominal Wage Index Unit'), ('UYU', 'Uruguayan Peso'), ('UYP', 'Uruguayan Peso (1975–1993)'), ('UYI', 'Uruguayan Peso (Indexed Units)'), ('UZS', 'Uzbekistani Som'), ('VUV', 'Vanuatu Vatu'), ('VES', 'Venezuelan Bolívar'), ('VEB', 'Venezuelan Bolívar (1871–2008)'), ('VEF', 'Venezuelan Bolívar (2008–2018)'), ('VND', 'Vietnamese Dong'), ('VNN', 'Vietnamese Dong (1978–1985)'), ('CHE', 'WIR Euro'), ('CHW', 'WIR Franc'), ('XOF', 'West African CFA Franc'), ('YDD', 'Yemeni Dinar'), ('YER', 'Yemeni Rial'), ('YUN', 'Yugoslavian Convertible Dinar (1990–1992)'), ('YUD', 'Yugoslavian Hard Dinar (1966–1990)'), ('YUM', 'Yugoslavian New Dinar (1994–2002)'), ('YUR', 'Yugoslavian Reformed Dinar (1992–1993)'), ('ZWN', 'ZWN'), ('ZRN', 'Zairean New Zaire (1993–1998)'), ('ZRZ', 'Zairean Zaire (1971–1993)'), ('ZMW', 'Zambian Kwacha'), ('ZMK', 'Zambian Kwacha (1968–2012)'), ('ZWD', 'Zimbabwean Dollar (1980–2008)'), ('ZWR', 'Zimbabwean Dollar (2008)'), ('ZWL', 'Zimbabwean Dollar (2009)')], default='USD', editable=False, max_length=3),
+        ),
+        migrations.AlterField(
+            model_name='tax',
+            name='id',
+            field=models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
+        ),
+        migrations.AlterField(
+            model_name='usage',
+            name='id',
+            field=models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
         ),
     ]
```

## Comparing `subscriptions/migrations/0008_rename_vendor_subscriptionpayment_provider_name_and_more.py` & `subscriptions/migrations/0019_rename_subscription_uid_subscriptionpayment_subscription_and_more.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,28 @@
-# Generated by Django 4.0.3 on 2022-03-11 12:39
+# Generated by Django 4.0.3 on 2022-07-28 19:33
 
 from django.db import migrations
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('subscriptions', '0007_subscriptionpayment_and_more'),
+        ('subscriptions', '0018_remove_subscription_id_remove_subscriptionpayment_id_and_more'),
     ]
 
     operations = [
         migrations.RenameField(
             model_name='subscriptionpayment',
-            old_name='vendor',
-            new_name='provider_name',
-        ),
-        migrations.RenameField(
-            model_name='subscriptionpayment',
-            old_name='vendor_transaction_id',
-            new_name='provider_transaction_id',
+            old_name='subscription_uid',
+            new_name='subscription',
         ),
         migrations.RenameField(
             model_name='subscriptionpaymentrefund',
-            old_name='vendor',
-            new_name='provider_name',
+            old_name='original_payment_uid',
+            new_name='original_payment',
         ),
         migrations.RenameField(
-            model_name='subscriptionpaymentrefund',
-            old_name='vendor_transaction_id',
-            new_name='provider_transaction_id',
+            model_name='tax',
+            old_name='subscription_payment_uid',
+            new_name='subscription_payment',
         ),
     ]
```

