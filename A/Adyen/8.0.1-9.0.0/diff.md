# Comparing `tmp/Adyen-8.0.1.tar.gz` & `tmp/Adyen-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Adyen-8.0.1.tar", last modified: Thu Mar 30 10:33:11 2023, max compression
+gzip compressed data, was "Adyen-9.0.0.tar", last modified: Fri Jun 30 13:00:28 2023, max compression
```

## Comparing `Adyen-8.0.1.tar` & `Adyen-9.0.0.tar`

### file list

```diff
@@ -1,113 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:33:11.039349 Adyen-8.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:33:11.015349 Adyen-8.0.1/Adyen/
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23531 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/httpclient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:33:11.015349 Adyen-8.0.1/Adyen/services/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:33:11.019349 Adyen-8.0.1/Adyen/services/balancePlatform/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/balancePlatform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/balancePlatform/account_holders_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/balancePlatform/balance_accounts_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/balancePlatform/bank_account_validation_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/balancePlatform/payment_instrument_groups_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/balancePlatform/payment_instruments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/balancePlatform/platform_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/balancePlatform/transaction_rules_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/binLookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:33:11.019349 Adyen-8.0.1/Adyen/services/checkout/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/checkout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/checkout/classic_checkout_sdk_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/checkout/modifications_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/checkout/orders_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/checkout/payment_links_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/checkout/payments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/checkout/recurring_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/checkout/utility_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/dataProtection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:33:11.023349 Adyen-8.0.1/Adyen/services/legalEntityManagement/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/legalEntityManagement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/legalEntityManagement/business_lines_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/legalEntityManagement/documents_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/legalEntityManagement/hosted_onboarding_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/legalEntityManagement/legal_entities_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/legalEntityManagement/terms_of_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/legalEntityManagement/transfer_instruments_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:33:11.031349 Adyen-8.0.1/Adyen/services/management/
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/management/account_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/management/account_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/management/account_store_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/management/allowed_origins_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/management/allowed_origins_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/management/api_credentials_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/management/api_credentials_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/management/api_key_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/management/api_key_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/management/client_key_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/management/client_key_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/management/my_api_credential_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/management/payment_methods_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/management/payout_settings_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/management/terminal_actions_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/management/terminal_actions_terminal_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/management/terminal_orders_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/management/terminal_orders_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/management/terminal_settings_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/management/terminal_settings_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/management/terminal_settings_store_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/management/terminal_settings_terminal_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/management/terminals_terminal_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/management/users_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/management/users_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/management/webhooks_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/management/webhooks_merchant_level_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:33:11.031349 Adyen-8.0.1/Adyen/services/payments/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/payments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/payments/general_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/payments/modifications_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:33:11.031349 Adyen-8.0.1/Adyen/services/payouts/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/payouts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/payouts/initialization_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/payouts/instant_payouts_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/payouts/reviewing_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/recurring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/storedValue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:33:11.031349 Adyen-8.0.1/Adyen/services/transfers/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/transfers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/transfers/transactions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/services/transfers/transfers_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-03-30 10:32:55.000000 Adyen-8.0.1/Adyen/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:33:11.015349 Adyen-8.0.1/Adyen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-03-30 10:33:10.000000 Adyen-8.0.1/Adyen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-03-30 10:33:11.000000 Adyen-8.0.1/Adyen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 10:33:10.000000 Adyen-8.0.1/Adyen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-30 10:33:10.000000 Adyen-8.0.1/Adyen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-30 10:32:55.000000 Adyen-8.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-03-30 10:33:11.039349 Adyen-8.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-03-30 10:32:55.000000 Adyen-8.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-30 10:33:11.039349 Adyen-8.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-30 10:32:55.000000 Adyen-8.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:33:11.039349 Adyen-8.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-30 10:32:55.000000 Adyen-8.0.1/test/BaseTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-03-30 10:32:55.000000 Adyen-8.0.1/test/BinLookupTest.py
--rw-r--r--   0 runner    (1001) docker     (123)    32846 2023-03-30 10:32:55.000000 Adyen-8.0.1/test/CheckoutTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-03-30 10:32:55.000000 Adyen-8.0.1/test/CheckoutUtilityTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-03-30 10:32:55.000000 Adyen-8.0.1/test/ConfigurationTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-03-30 10:32:55.000000 Adyen-8.0.1/test/DataProtectionTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-03-30 10:32:55.000000 Adyen-8.0.1/test/DetermineEndpointTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-03-30 10:32:55.000000 Adyen-8.0.1/test/LegalEntityManagementTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-03-30 10:32:55.000000 Adyen-8.0.1/test/ManagementTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-03-30 10:32:55.000000 Adyen-8.0.1/test/ModificationTest.py
--rw-r--r--   0 runner    (1001) docker     (123)    18978 2023-03-30 10:32:55.000000 Adyen-8.0.1/test/PaymentTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-03-30 10:32:55.000000 Adyen-8.0.1/test/RecurringTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-03-30 10:32:55.000000 Adyen-8.0.1/test/StoredValueTest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-03-30 10:32:55.000000 Adyen-8.0.1/test/TerminalTest.py
--rw-r--r--   0 runner    (1001) docker     (123)    14395 2023-03-30 10:32:55.000000 Adyen-8.0.1/test/ThirdPartyPayoutTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-03-30 10:32:55.000000 Adyen-8.0.1/test/TransfersTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-03-30 10:32:55.000000 Adyen-8.0.1/test/UtilTest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:32:55.000000 Adyen-8.0.1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:00:28.789552 Adyen-9.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:00:28.777551 Adyen-9.0.0/Adyen/
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23474 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/httpclient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:00:28.777551 Adyen-9.0.0/Adyen/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:00:28.781551 Adyen-9.0.0/Adyen/services/balancePlatform/
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/balancePlatform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/balancePlatform/account_holders_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/balancePlatform/balance_accounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/balancePlatform/bank_account_validation_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/balancePlatform/grant_accounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/balancePlatform/grant_offers_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/balancePlatform/payment_instrument_groups_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/balancePlatform/payment_instruments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/balancePlatform/platform_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/balancePlatform/transaction_rules_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/binlookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:00:28.781551 Adyen-9.0.0/Adyen/services/checkout/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/checkout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/checkout/classic_checkout_sdk_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/checkout/modifications_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/checkout/orders_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/checkout/payment_links_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/checkout/payments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/checkout/recurring_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/checkout/utility_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/dataProtection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:00:28.781551 Adyen-9.0.0/Adyen/services/legalEntityManagement/
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/legalEntityManagement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/legalEntityManagement/business_lines_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/legalEntityManagement/documents_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/legalEntityManagement/hosted_onboarding_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/legalEntityManagement/legal_entities_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/legalEntityManagement/pci_questionnaires_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/legalEntityManagement/terms_of_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/legalEntityManagement/transfer_instruments_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:00:28.785551 Adyen-9.0.0/Adyen/services/management/
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/account_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/account_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/account_store_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/allowed_origins_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/allowed_origins_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/api_credentials_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/api_credentials_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/api_key_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/api_key_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/client_key_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/client_key_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/my_api_credential_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/payment_methods_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/payout_settings_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/split_configuration_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/terminal_actions_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/terminal_actions_terminal_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/terminal_orders_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/terminal_orders_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/terminal_settings_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/terminal_settings_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/terminal_settings_store_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/terminal_settings_terminal_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/terminals_terminal_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/users_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/users_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/webhooks_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/webhooks_merchant_level_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:00:28.785551 Adyen-9.0.0/Adyen/services/payments/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/payments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/payments/general_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/payments/modifications_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:00:28.785551 Adyen-9.0.0/Adyen/services/payouts/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/payouts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/payouts/initialization_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/payouts/instant_payouts_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/payouts/reviewing_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/recurring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/storedValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:00:28.785551 Adyen-9.0.0/Adyen/services/transfers/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/transfers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/transfers/capital_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/transfers/transactions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/transfers/transfers_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:00:28.777551 Adyen-9.0.0/Adyen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-30 13:00:28.000000 Adyen-9.0.0/Adyen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-06-30 13:00:28.000000 Adyen-9.0.0/Adyen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 13:00:28.000000 Adyen-9.0.0/Adyen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-30 13:00:28.000000 Adyen-9.0.0/Adyen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-30 13:00:17.000000 Adyen-9.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-30 13:00:28.789552 Adyen-9.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-06-30 13:00:17.000000 Adyen-9.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-30 13:00:28.789552 Adyen-9.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-30 13:00:17.000000 Adyen-9.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:00:28.789552 Adyen-9.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/BaseTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/BinLookupTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32846 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/CheckoutTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/CheckoutUtilityTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/ClientTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/ConfigurationTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/DataProtectionTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/DetermineEndpointTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/LegalEntityManagementTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/ManagementTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/ModificationTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18978 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/PaymentTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/RecurringTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/StoredValueTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/TerminalTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/ThirdPartyPayoutTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/TransfersTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/UtilTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/__init__.py
```

### Comparing `Adyen-8.0.1/Adyen/__init__.py` & `Adyen-9.0.0/Adyen/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     AdyenManagementApi,
     AdyenCheckoutApi,
     AdyenTerminalApi,
     AdyenLegalEntityManagementApi,
     AdyenDataProtectionApi,
     AdyenTransfersApi,
     AdyenStoredValueApi,
-    AdyenBalancePlatformApi
+    AdyenBalancePlatformApi,
 )
 
 from .httpclient import HTTPClient
 
 
 class Adyen(AdyenBase):
     def __init__(self, **kwargs):
```

### Comparing `Adyen-8.0.1/Adyen/client.py` & `Adyen-9.0.0/Adyen/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 class AdyenClient(object):
     IDEMPOTENCY_HEADER_NAME = 'Idempotency-Key'
     APPLICATION_INFO_HEADER_NAME = 'adyen-library-name'
     APPLICATION_VERSION_HEADER_NAME = 'adyen-library-version'
     """A requesting client that interacts with Adyen. This class holds the
     adyen logic of Adyen HTTP API communication. This is the object that can
-    maintain its own username, password, merchant_account, hmac and skin_code.
+    maintain its own username, password and hmac.
     When these values aren't within this object, the root adyen module
     variables will be used.
 
     The public methods and call_api only return AdyenResult objects.
     Otherwise raising various validation and communication errors.
 
     Args:
@@ -91,15 +91,15 @@
             api_payout_version=None,
             api_recurring_version=None,
             api_terminal_version=None,
             api_legal_entity_management_version=None,
             api_data_protection_version=None,
             api_transfers_version=None,
             api_stored_value_version=None,
-            api_balance_platform_version=None
+            api_balance_platform_version=None,
     ):
         self.username = username
         self.password = password
         self.xapikey = xapikey
         self.review_payout_username = review_payout_username
         self.review_payout_password = review_payout_password
         self.store_payout_username = store_payout_username
@@ -208,25 +208,25 @@
                     'live': settings.BASE_DATA_PROTECION_URL.format(platform),
                     'test': settings.BASE_DATA_PROTECION_URL.format(platform)
                 }
             },
             'transfers': {
                 'version': self.api_transfers_version,
                 'base_url': {
-                    'live': settings.BASE_TRANSFERS_URL.format(platform),
-                    'test': settings.BASE_TRANSFERS_URL.format(platform)
+                    'live': settings.BASE_BTL_URL.format(platform),
+                    'test': settings.BASE_BTL_URL.format(platform)
                 }
             },
             'storedValue': {
                 'version': self.api_stored_value_version,
                 'base_url': {
                     'live': settings.BASE_STORED_VALUE_URL.format(platform),
                     'test': settings.BASE_STORED_VALUE_URL.format(platform)
                 }
-            }
+            },
         }
 
         version = versions_and_urls[service]['version']
         base_url = versions_and_urls[service]['base_url'][platform]
         # Match urls that require a live prefix and do not have one
 
         if platform == 'live' and '{live_prefix}' in base_url:
@@ -356,15 +356,15 @@
             request_data,
             service,
             method,
             endpoint,
             idempotency_key=None,
             **kwargs
     ):
-        """This will call the adyen api. username, password, merchant_account,
+        """This will call the adyen api. username, password,
         and platform are pulled from root module level and or self object.
         AdyenResult will be returned on 200 response. Otherwise, an exception
         is raised.
 
         Args:
             idempotency_key: https://docs.adyen.com/development-resources
             /api-idempotency
```

### Comparing `Adyen-8.0.1/Adyen/exceptions.py` & `Adyen-9.0.0/Adyen/exceptions.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/httpclient.py` & `Adyen-9.0.0/Adyen/httpclient.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/__init__.py` & `Adyen-9.0.0/Adyen/services/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .base import AdyenBase
-from .binLookup import AdyenBinlookupApi
+from .binlookup import AdyenBinlookupApi
 from .checkout import AdyenCheckoutApi
 from .payments import AdyenPaymentsApi
 from .payouts import AdyenPayoutsApi
 from .recurring import AdyenRecurringApi
 from .terminal import AdyenTerminalApi
 from .management import AdyenManagementApi
 from .legalEntityManagement import AdyenLegalEntityManagementApi
```

### Comparing `Adyen-8.0.1/Adyen/services/balancePlatform/__init__.py` & `Adyen-9.0.0/Adyen/services/balancePlatform/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from ..base import AdyenServiceBase
 from .account_holders_api import AccountHoldersApi
 from .balance_accounts_api import BalanceAccountsApi
 from .bank_account_validation_api import BankAccountValidationApi
+from .grant_accounts_api import GrantAccountsApi
+from .grant_offers_api import GrantOffersApi
 from .payment_instrument_groups_api import PaymentInstrumentGroupsApi
 from .payment_instruments_api import PaymentInstrumentsApi
 from .platform_api import PlatformApi
 from .transaction_rules_api import TransactionRulesApi
 
 
 class AdyenBalancePlatformApi(AdyenServiceBase):
@@ -16,11 +18,13 @@
     """
 
     def __init__(self, client=None):
         super(AdyenBalancePlatformApi, self).__init__(client=client)
         self.account_holders_api = AccountHoldersApi(client=client)
         self.balance_accounts_api = BalanceAccountsApi(client=client)
         self.bank_account_validation_api = BankAccountValidationApi(client=client)
+        self.grant_accounts_api = GrantAccountsApi(client=client)
+        self.grant_offers_api = GrantOffersApi(client=client)
         self.payment_instrument_groups_api = PaymentInstrumentGroupsApi(client=client)
         self.payment_instruments_api = PaymentInstrumentsApi(client=client)
         self.platform_api = PlatformApi(client=client)
         self.transaction_rules_api = TransactionRulesApi(client=client)
```

### Comparing `Adyen-8.0.1/Adyen/services/balancePlatform/account_holders_api.py` & `Adyen-9.0.0/Adyen/services/balancePlatform/account_holders_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/balancePlatform/balance_accounts_api.py` & `Adyen-9.0.0/Adyen/services/balancePlatform/balance_accounts_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/balancePlatform/bank_account_validation_api.py` & `Adyen-9.0.0/Adyen/services/balancePlatform/bank_account_validation_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/balancePlatform/payment_instrument_groups_api.py` & `Adyen-9.0.0/Adyen/services/balancePlatform/payment_instrument_groups_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/balancePlatform/payment_instruments_api.py` & `Adyen-9.0.0/Adyen/services/balancePlatform/payment_instruments_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,17 +16,17 @@
         """
         Get a payment instrument
         """
         endpoint = f"/paymentInstruments/{id}"
         method = "GET"
         return self.client.call_adyen_api(None, self.service, method, endpoint, idempotency_key, **kwargs)
 
-    def get_reveal_information_of_payment_instrument(self, id, idempotency_key=None, **kwargs):
+    def get_pan_of_payment_instrument(self, id, idempotency_key=None, **kwargs):
         """
-        Get the reveal information of a payment instrument
+        Get the PAN of a payment instrument
         """
         endpoint = f"/paymentInstruments/{id}/reveal"
         method = "GET"
         return self.client.call_adyen_api(None, self.service, method, endpoint, idempotency_key, **kwargs)
 
     def get_all_transaction_rules_for_payment_instrument(self, id, idempotency_key=None, **kwargs):
         """
```

### Comparing `Adyen-8.0.1/Adyen/services/balancePlatform/platform_api.py` & `Adyen-9.0.0/Adyen/services/balancePlatform/platform_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/balancePlatform/transaction_rules_api.py` & `Adyen-9.0.0/Adyen/services/balancePlatform/transaction_rules_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/base.py` & `Adyen-9.0.0/Adyen/services/base.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/binLookup.py` & `Adyen-9.0.0/Adyen/services/binlookup.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/checkout/__init__.py` & `Adyen-9.0.0/Adyen/services/checkout/__init__.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/checkout/classic_checkout_sdk_api.py` & `Adyen-9.0.0/Adyen/services/checkout/classic_checkout_sdk_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/checkout/modifications_api.py` & `Adyen-9.0.0/Adyen/services/checkout/modifications_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/checkout/orders_api.py` & `Adyen-9.0.0/Adyen/services/checkout/orders_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/checkout/payment_links_api.py` & `Adyen-9.0.0/Adyen/services/checkout/payment_links_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/checkout/payments_api.py` & `Adyen-9.0.0/Adyen/services/checkout/payments_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/checkout/recurring_api.py` & `Adyen-9.0.0/Adyen/services/checkout/recurring_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/checkout/utility_api.py` & `Adyen-9.0.0/Adyen/services/checkout/utility_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/dataProtection.py` & `Adyen-9.0.0/Adyen/services/dataProtection.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/legalEntityManagement/__init__.py` & `Adyen-9.0.0/Adyen/services/legalEntityManagement/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from ..base import AdyenServiceBase
 from .business_lines_api import BusinessLinesApi
 from .documents_api import DocumentsApi
 from .hosted_onboarding_api import HostedOnboardingApi
 from .legal_entities_api import LegalEntitiesApi
+from .pci_questionnaires_api import PCIQuestionnairesApi
 from .terms_of_service_api import TermsOfServiceApi
 from .transfer_instruments_api import TransferInstrumentsApi
 
 
 class AdyenLegalEntityManagementApi(AdyenServiceBase):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
@@ -16,9 +17,10 @@
 
     def __init__(self, client=None):
         super(AdyenLegalEntityManagementApi, self).__init__(client=client)
         self.business_lines_api = BusinessLinesApi(client=client)
         self.documents_api = DocumentsApi(client=client)
         self.hosted_onboarding_api = HostedOnboardingApi(client=client)
         self.legal_entities_api = LegalEntitiesApi(client=client)
+        self.pci_questionnaires_api = PCIQuestionnairesApi(client=client)
         self.terms_of_service_api = TermsOfServiceApi(client=client)
         self.transfer_instruments_api = TransferInstrumentsApi(client=client)
```

### Comparing `Adyen-8.0.1/Adyen/services/legalEntityManagement/business_lines_api.py` & `Adyen-9.0.0/Adyen/services/legalEntityManagement/business_lines_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/legalEntityManagement/documents_api.py` & `Adyen-9.0.0/Adyen/services/legalEntityManagement/documents_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/legalEntityManagement/hosted_onboarding_api.py` & `Adyen-9.0.0/Adyen/services/legalEntityManagement/hosted_onboarding_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/legalEntityManagement/legal_entities_api.py` & `Adyen-9.0.0/Adyen/services/legalEntityManagement/legal_entities_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,7 +40,15 @@
         """
         Create a legal entity
         """
         endpoint = f"/legalEntities"
         method = "POST"
         return self.client.call_adyen_api(request, self.service, method, endpoint, idempotency_key, **kwargs)
 
+    def check_legal_entitys_verification_errors(self, id, idempotency_key=None, **kwargs):
+        """
+        Check a legal entity's verification errors
+        """
+        endpoint = f"/legalEntities/{id}/checkVerificationErrors"
+        method = "POST"
+        return self.client.call_adyen_api(None, self.service, method, endpoint, idempotency_key, **kwargs)
+
```

### Comparing `Adyen-8.0.1/Adyen/services/legalEntityManagement/terms_of_service_api.py` & `Adyen-9.0.0/Adyen/services/legalEntityManagement/terms_of_service_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,22 +16,14 @@
         """
         Get Terms of Service information for a legal entity
         """
         endpoint = f"/legalEntities/{id}/termsOfServiceAcceptanceInfos"
         method = "GET"
         return self.client.call_adyen_api(None, self.service, method, endpoint, idempotency_key, **kwargs)
 
-    def get_terms_of_service_status(self, id, idempotency_key=None, **kwargs):
-        """
-        Get Terms of Service status
-        """
-        endpoint = f"/legalEntities/{id}/termsOfServiceStatus"
-        method = "GET"
-        return self.client.call_adyen_api(None, self.service, method, endpoint, idempotency_key, **kwargs)
-
     def accept_terms_of_service(self, request, id, termsofservicedocumentid, idempotency_key=None, **kwargs):
         """
         Accept Terms of Service
         """
         endpoint = f"/legalEntities/{id}/termsOfService/{termsofservicedocumentid}"
         method = "PATCH"
         return self.client.call_adyen_api(request, self.service, method, endpoint, idempotency_key, **kwargs)
```

### Comparing `Adyen-8.0.1/Adyen/services/legalEntityManagement/transfer_instruments_api.py` & `Adyen-9.0.0/Adyen/services/legalEntityManagement/transfer_instruments_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/management/__init__.py` & `Adyen-9.0.0/Adyen/services/management/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .allowed_origins_company_level_api import AllowedOriginsCompanyLevelApi
 from .allowed_origins_merchant_level_api import AllowedOriginsMerchantLevelApi
 from .client_key_company_level_api import ClientKeyCompanyLevelApi
 from .client_key_merchant_level_api import ClientKeyMerchantLevelApi
 from .my_api_credential_api import MyAPICredentialApi
 from .payment_methods_merchant_level_api import PaymentMethodsMerchantLevelApi
 from .payout_settings_merchant_level_api import PayoutSettingsMerchantLevelApi
+from .split_configuration_merchant_level_api import SplitConfigurationMerchantLevelApi
 from .terminal_actions_company_level_api import TerminalActionsCompanyLevelApi
 from .terminal_actions_terminal_level_api import TerminalActionsTerminalLevelApi
 from .terminal_orders_company_level_api import TerminalOrdersCompanyLevelApi
 from .terminal_orders_merchant_level_api import TerminalOrdersMerchantLevelApi
 from .terminal_settings_company_level_api import TerminalSettingsCompanyLevelApi
 from .terminal_settings_merchant_level_api import TerminalSettingsMerchantLevelApi
 from .terminal_settings_store_level_api import TerminalSettingsStoreLevelApi
@@ -47,14 +48,15 @@
         self.allowed_origins_company_level_api = AllowedOriginsCompanyLevelApi(client=client)
         self.allowed_origins_merchant_level_api = AllowedOriginsMerchantLevelApi(client=client)
         self.client_key_company_level_api = ClientKeyCompanyLevelApi(client=client)
         self.client_key_merchant_level_api = ClientKeyMerchantLevelApi(client=client)
         self.my_api_credential_api = MyAPICredentialApi(client=client)
         self.payment_methods_merchant_level_api = PaymentMethodsMerchantLevelApi(client=client)
         self.payout_settings_merchant_level_api = PayoutSettingsMerchantLevelApi(client=client)
+        self.split_configuration_merchant_level_api = SplitConfigurationMerchantLevelApi(client=client)
         self.terminal_actions_company_level_api = TerminalActionsCompanyLevelApi(client=client)
         self.terminal_actions_terminal_level_api = TerminalActionsTerminalLevelApi(client=client)
         self.terminal_orders_company_level_api = TerminalOrdersCompanyLevelApi(client=client)
         self.terminal_orders_merchant_level_api = TerminalOrdersMerchantLevelApi(client=client)
         self.terminal_settings_company_level_api = TerminalSettingsCompanyLevelApi(client=client)
         self.terminal_settings_merchant_level_api = TerminalSettingsMerchantLevelApi(client=client)
         self.terminal_settings_store_level_api = TerminalSettingsStoreLevelApi(client=client)
```

### Comparing `Adyen-8.0.1/Adyen/services/management/account_company_level_api.py` & `Adyen-9.0.0/Adyen/services/management/account_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/management/account_merchant_level_api.py` & `Adyen-9.0.0/Adyen/services/management/account_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/management/account_store_level_api.py` & `Adyen-9.0.0/Adyen/services/management/account_store_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/management/allowed_origins_company_level_api.py` & `Adyen-9.0.0/Adyen/services/management/allowed_origins_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/management/allowed_origins_merchant_level_api.py` & `Adyen-9.0.0/Adyen/services/management/allowed_origins_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/management/api_credentials_company_level_api.py` & `Adyen-9.0.0/Adyen/services/management/api_credentials_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/management/api_credentials_merchant_level_api.py` & `Adyen-9.0.0/Adyen/services/management/api_credentials_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/management/api_key_company_level_api.py` & `Adyen-9.0.0/Adyen/services/management/api_key_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/management/api_key_merchant_level_api.py` & `Adyen-9.0.0/Adyen/services/management/api_key_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/management/client_key_company_level_api.py` & `Adyen-9.0.0/Adyen/services/management/client_key_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/management/client_key_merchant_level_api.py` & `Adyen-9.0.0/Adyen/services/management/client_key_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/management/my_api_credential_api.py` & `Adyen-9.0.0/Adyen/services/management/my_api_credential_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/management/payment_methods_merchant_level_api.py` & `Adyen-9.0.0/Adyen/services/management/payment_methods_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/management/payout_settings_merchant_level_api.py` & `Adyen-9.0.0/Adyen/services/management/payout_settings_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/management/terminal_actions_company_level_api.py` & `Adyen-9.0.0/Adyen/services/management/terminal_actions_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/management/terminal_actions_terminal_level_api.py` & `Adyen-9.0.0/Adyen/services/management/terminal_actions_terminal_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/management/terminal_orders_company_level_api.py` & `Adyen-9.0.0/Adyen/services/management/terminal_orders_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/management/terminal_orders_merchant_level_api.py` & `Adyen-9.0.0/Adyen/services/management/terminal_orders_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/management/terminal_settings_company_level_api.py` & `Adyen-9.0.0/Adyen/services/management/terminal_settings_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/management/terminal_settings_merchant_level_api.py` & `Adyen-9.0.0/Adyen/services/management/terminal_settings_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/management/terminal_settings_store_level_api.py` & `Adyen-9.0.0/Adyen/services/management/terminal_settings_store_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/management/terminal_settings_terminal_level_api.py` & `Adyen-9.0.0/Adyen/services/management/terminal_settings_terminal_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/management/terminals_terminal_level_api.py` & `Adyen-9.0.0/Adyen/services/management/terminals_terminal_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/management/users_company_level_api.py` & `Adyen-9.0.0/Adyen/services/management/users_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/management/users_merchant_level_api.py` & `Adyen-9.0.0/Adyen/services/management/users_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/management/webhooks_company_level_api.py` & `Adyen-9.0.0/Adyen/services/management/webhooks_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/management/webhooks_merchant_level_api.py` & `Adyen-9.0.0/Adyen/services/management/webhooks_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/payments/__init__.py` & `Adyen-9.0.0/Adyen/services/payments/__init__.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/payments/general_api.py` & `Adyen-9.0.0/Adyen/services/payments/general_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/payments/modifications_api.py` & `Adyen-9.0.0/Adyen/services/payments/modifications_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/payouts/__init__.py` & `Adyen-9.0.0/Adyen/services/payouts/__init__.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/payouts/initialization_api.py` & `Adyen-9.0.0/Adyen/services/payouts/initialization_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,31 +8,31 @@
     Do not edit the class manually.
     """
 
     def __init__(self, client=None):
         super(InitializationApi, self).__init__(client=client)
         self.service = "payouts"
 
-    def store_payout_details(self, request, idempotency_key=None, **kwargs):
+    def store_detail(self, request, idempotency_key=None, **kwargs):
         """
         Store payout details
         """
         endpoint = f"/storeDetail"
         method = "POST"
         return self.client.call_adyen_api(request, self.service, method, endpoint, idempotency_key, **kwargs)
 
-    def store_details_and_submit_payout(self, request, idempotency_key=None, **kwargs):
+    def store_detail_and_submit_third_party(self, request, idempotency_key=None, **kwargs):
         """
         Store details and submit a payout
         """
         endpoint = f"/storeDetailAndSubmitThirdParty"
         method = "POST"
         return self.client.call_adyen_api(request, self.service, method, endpoint, idempotency_key, **kwargs)
 
-    def submit_payout(self, request, idempotency_key=None, **kwargs):
+    def submit_third_party(self, request, idempotency_key=None, **kwargs):
         """
         Submit a payout
         """
         endpoint = f"/submitThirdParty"
         method = "POST"
         return self.client.call_adyen_api(request, self.service, method, endpoint, idempotency_key, **kwargs)
```

### Comparing `Adyen-8.0.1/Adyen/services/payouts/instant_payouts_api.py` & `Adyen-9.0.0/Adyen/services/payouts/instant_payouts_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Do not edit the class manually.
     """
 
     def __init__(self, client=None):
         super(InstantPayoutsApi, self).__init__(client=client)
         self.service = "payouts"
 
-    def make_instant_card_payout(self, request, idempotency_key=None, **kwargs):
+    def payout(self, request, idempotency_key=None, **kwargs):
         """
         Make an instant card payout
         """
         endpoint = f"/payout"
         method = "POST"
         return self.client.call_adyen_api(request, self.service, method, endpoint, idempotency_key, **kwargs)
```

### Comparing `Adyen-8.0.1/Adyen/services/payouts/reviewing_api.py` & `Adyen-9.0.0/Adyen/services/payouts/reviewing_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,23 +8,23 @@
     Do not edit the class manually.
     """
 
     def __init__(self, client=None):
         super(ReviewingApi, self).__init__(client=client)
         self.service = "payouts"
 
-    def confirm_payout(self, request, idempotency_key=None, **kwargs):
+    def confirm_third_party(self, request, idempotency_key=None, **kwargs):
         """
         Confirm a payout
         """
         endpoint = f"/confirmThirdParty"
         method = "POST"
         return self.client.call_adyen_api(request, self.service, method, endpoint, idempotency_key, **kwargs)
 
-    def cancel_payout(self, request, idempotency_key=None, **kwargs):
+    def decline_third_party(self, request, idempotency_key=None, **kwargs):
         """
         Cancel a payout
         """
         endpoint = f"/declineThirdParty"
         method = "POST"
         return self.client.call_adyen_api(request, self.service, method, endpoint, idempotency_key, **kwargs)
```

### Comparing `Adyen-8.0.1/Adyen/services/recurring.py` & `Adyen-9.0.0/Adyen/services/recurring.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/storedValue.py` & `Adyen-9.0.0/Adyen/services/storedValue.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/terminal.py` & `Adyen-9.0.0/Adyen/services/terminal.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/transfers/__init__.py` & `Adyen-9.0.0/Adyen/services/transfers/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from ..base import AdyenServiceBase
+from .capital_api import CapitalApi
 from .transactions_api import TransactionsApi
 from .transfers_api import TransfersApi
 
 
 class AdyenTransfersApi(AdyenServiceBase):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, client=None):
         super(AdyenTransfersApi, self).__init__(client=client)
+        self.capital_api = CapitalApi(client=client)
         self.transactions_api = TransactionsApi(client=client)
         self.transfers_api = TransfersApi(client=client)
```

### Comparing `Adyen-8.0.1/Adyen/services/transfers/transactions_api.py` & `Adyen-9.0.0/Adyen/services/transfers/transactions_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/services/transfers/transfers_api.py` & `Adyen-9.0.0/Adyen/services/transfers/transfers_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen/settings.py` & `Adyen-9.0.0/Adyen/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Those constants are used from the library only
 BASE_DATA_PROTECION_URL = "https://ca-{}.adyen.com/ca/services/DataProtectionService"
 BASE_CONFIGURATION_URL = "https://balanceplatform-api-{}.adyen.com/bcl"
+BASE_BTL_URL = "https://balanceplatform-api-{}.adyen.com/btl"
 BASE_TERMINAL_URL = "https://postfmapi-{}.adyen.com/postfmapi/terminal"
-BASE_TRANSFERS_URL = "https://balanceplatform-api-{}.adyen.com/btl"
 BASE_MANAGEMENT_URL = "https://management-{}.adyen.com"
 BASE_LEGAL_ENTITY_MANAGEMENT_URL = "https://kyc-{}.adyen.com/lem"
 PAL_LIVE_ENDPOINT_URL_TEMPLATE = "https://{live_prefix}-pal-live" \
                                  ".adyenpayments.com/pal/servlet"
 PAL_TEST_URL = "https://pal-test.adyen.com/pal/servlet"
 ENDPOINT_CHECKOUT_TEST = "https://checkout-test.adyen.com"
 ENDPOINT_CHECKOUT_LIVE_SUFFIX = "https://{live_prefix}-checkout-live" \
@@ -18,12 +18,12 @@
 API_CHECKOUT_UTILITY_VERSION = "v1"
 API_DATA_PROTECION_VERSION = "v1"
 API_MANAGEMENT_VERSION = "v1"
 API_RECURRING_VERSION = "v68"
 API_PAYMENT_VERSION = "v68"
 API_PAYOUT_VERSION = "v68"
 API_TERMINAL_VERSION = "v1"
-LIB_VERSION = "8.0.1"
 API_TRANSFERS_VERSION = "v3"
-API_LEGAL_ENTITY_MANAGEMENT_VERSION = "v2"
+API_LEGAL_ENTITY_MANAGEMENT_VERSION = "v3"
 API_STORED_VALUE_VERSION = "v46"
 LIB_NAME = "adyen-python-api-library"
+LIB_VERSION = "9.0.0"
```

### Comparing `Adyen-8.0.1/Adyen/util.py` & `Adyen-9.0.0/Adyen/util.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/Adyen.egg-info/PKG-INFO` & `Adyen-9.0.0/Adyen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Adyen
-Version: 8.0.1
+Version: 9.0.0
 Summary: Adyen Python Api
 Home-page: https://github.com/Adyen/adyen-python-api-library
 Author: Adyen
 Author-email: support@adyen.com
 Maintainer: Adyen
 Maintainer-email: support@adyen.com
 Keywords: payments,adyen,fintech
```

### Comparing `Adyen-8.0.1/Adyen.egg-info/SOURCES.txt` & `Adyen-9.0.0/Adyen.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,23 +10,25 @@
 Adyen/util.py
 Adyen.egg-info/PKG-INFO
 Adyen.egg-info/SOURCES.txt
 Adyen.egg-info/dependency_links.txt
 Adyen.egg-info/top_level.txt
 Adyen/services/__init__.py
 Adyen/services/base.py
-Adyen/services/binLookup.py
+Adyen/services/binlookup.py
 Adyen/services/dataProtection.py
 Adyen/services/recurring.py
 Adyen/services/storedValue.py
 Adyen/services/terminal.py
 Adyen/services/balancePlatform/__init__.py
 Adyen/services/balancePlatform/account_holders_api.py
 Adyen/services/balancePlatform/balance_accounts_api.py
 Adyen/services/balancePlatform/bank_account_validation_api.py
+Adyen/services/balancePlatform/grant_accounts_api.py
+Adyen/services/balancePlatform/grant_offers_api.py
 Adyen/services/balancePlatform/payment_instrument_groups_api.py
 Adyen/services/balancePlatform/payment_instruments_api.py
 Adyen/services/balancePlatform/platform_api.py
 Adyen/services/balancePlatform/transaction_rules_api.py
 Adyen/services/checkout/__init__.py
 Adyen/services/checkout/classic_checkout_sdk_api.py
 Adyen/services/checkout/modifications_api.py
@@ -36,14 +38,15 @@
 Adyen/services/checkout/recurring_api.py
 Adyen/services/checkout/utility_api.py
 Adyen/services/legalEntityManagement/__init__.py
 Adyen/services/legalEntityManagement/business_lines_api.py
 Adyen/services/legalEntityManagement/documents_api.py
 Adyen/services/legalEntityManagement/hosted_onboarding_api.py
 Adyen/services/legalEntityManagement/legal_entities_api.py
+Adyen/services/legalEntityManagement/pci_questionnaires_api.py
 Adyen/services/legalEntityManagement/terms_of_service_api.py
 Adyen/services/legalEntityManagement/transfer_instruments_api.py
 Adyen/services/management/__init__.py
 Adyen/services/management/account_company_level_api.py
 Adyen/services/management/account_merchant_level_api.py
 Adyen/services/management/account_store_level_api.py
 Adyen/services/management/allowed_origins_company_level_api.py
@@ -53,14 +56,15 @@
 Adyen/services/management/api_key_company_level_api.py
 Adyen/services/management/api_key_merchant_level_api.py
 Adyen/services/management/client_key_company_level_api.py
 Adyen/services/management/client_key_merchant_level_api.py
 Adyen/services/management/my_api_credential_api.py
 Adyen/services/management/payment_methods_merchant_level_api.py
 Adyen/services/management/payout_settings_merchant_level_api.py
+Adyen/services/management/split_configuration_merchant_level_api.py
 Adyen/services/management/terminal_actions_company_level_api.py
 Adyen/services/management/terminal_actions_terminal_level_api.py
 Adyen/services/management/terminal_orders_company_level_api.py
 Adyen/services/management/terminal_orders_merchant_level_api.py
 Adyen/services/management/terminal_settings_company_level_api.py
 Adyen/services/management/terminal_settings_merchant_level_api.py
 Adyen/services/management/terminal_settings_store_level_api.py
@@ -74,20 +78,22 @@
 Adyen/services/payments/general_api.py
 Adyen/services/payments/modifications_api.py
 Adyen/services/payouts/__init__.py
 Adyen/services/payouts/initialization_api.py
 Adyen/services/payouts/instant_payouts_api.py
 Adyen/services/payouts/reviewing_api.py
 Adyen/services/transfers/__init__.py
+Adyen/services/transfers/capital_api.py
 Adyen/services/transfers/transactions_api.py
 Adyen/services/transfers/transfers_api.py
 test/BaseTest.py
 test/BinLookupTest.py
 test/CheckoutTest.py
 test/CheckoutUtilityTest.py
+test/ClientTest.py
 test/ConfigurationTest.py
 test/DataProtectionTest.py
 test/DetermineEndpointTest.py
 test/LegalEntityManagementTest.py
 test/ManagementTest.py
 test/ModificationTest.py
 test/PaymentTest.py
```

### Comparing `Adyen-8.0.1/LICENSE.md` & `Adyen-9.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/PKG-INFO` & `Adyen-9.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Adyen
-Version: 8.0.1
+Version: 9.0.0
 Summary: Adyen Python Api
 Home-page: https://github.com/Adyen/adyen-python-api-library
 Author: Adyen
 Author-email: support@adyen.com
 Maintainer: Adyen
 Maintainer-email: support@adyen.com
 Keywords: payments,adyen,fintech
```

### Comparing `Adyen-8.0.1/README.md` & `Adyen-9.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 ![Python](https://user-images.githubusercontent.com/55943882/212274988-4e58b807-d39b-4274-b712-06008b1ef5fc.png)
 
 # Adyen APIs Library for Python
 
-[![version](https://img.shields.io/badge/version-8.0.1-blue.svg)](https://docs.adyen.com/development-resources/libraries)
+[![version](https://img.shields.io/pypi/v/Adyen.svg)](https://docs.adyen.com/development-resources/libraries)
 
 This is the officially supported Python library for using Adyen's APIs.
 
 ## Supported API versions
 | API | Description | Service Name | Supported version |
 | --- | ----------- | ------------ | ----------------- | 
-|[BIN lookup API](https://docs.adyen.com/api-explorer/#/BinLookup/v52/overview) | The BIN Lookup API provides endpoints for retrieving information based on a given BIN. | binLookup | **v52** |
-| [Balance Platform API](https://docs.adyen.com/api-explorer/balanceplatform/1/overview) | The Balance Platform API enables you to create a platform where you can onboard your users as account holders and create balance accounts, cards, and business accounts. | balancePlatform | **v2** |
-| [Checkout API](https://docs.adyen.com/api-explorer/#/CheckoutService/v69/overview)| Our latest integration for accepting online payments. | checkout | **v70** |
+|[BIN lookup API](https://docs.adyen.com/api-explorer/BinLookup/52/overview) | The BIN Lookup API provides endpoints for retrieving information based on a given BIN. | binLookup | **v52** |
+| [Balance Platform API](https://docs.adyen.com/api-explorer/balanceplatform/2/overview) | The Balance Platform API enables you to create a platform where you can onboard your users as account holders and create balance accounts, cards, and business accounts. | balancePlatform | **v2** |
+| [Checkout API](https://docs.adyen.com/api-explorer/Checkout/70/overview)| Our latest integration for accepting online payments. | checkout | **v70** |
 | [Data Protection API](https://docs.adyen.com/development-resources/data-protection-api) | Endpoint for requesting data erasure. | dataProtection | **v1** |
-| [Legal Entity Management API](https://docs.adyen.com/api-explorer/legalentity/latest/overview) | Endpoint to manage legal entities | legalEntityManagement | **v2** |
-| [Management API](https://docs.adyen.com/api-explorer/#/ManagementService/v1/overview)| Configure and manage your Adyen company and merchant accounts, stores, and payment terminals. | management | **v1** |
-| [Payments API](https://docs.adyen.com/api-explorer/#/Payment/v68/overview)| Our classic integration for online payments. | payments | **v68** |
-| [Payouts API](https://docs.adyen.com/api-explorer/#/Payout/v68/overview)| Endpoints for sending funds to your customers. | payouts | **v68** |
-| [POS Terminal Management API](https://docs.adyen.com/api-explorer/#/postfmapi/v1/overview)| Endpoints for managing your point-of-sale payment terminals. | terminal | **v1** |
-| [Recurring API](https://docs.adyen.com/api-explorer/#/Recurring/v68/overview)| Endpoints for managing saved payment details. | recurring | **v68** |
+| [Legal Entity Management API](https://docs.adyen.com/api-explorer/legalentity/3/overview) | Endpoint to manage legal entities | legalEntityManagement | **v3** |
+| [Management API](https://docs.adyen.com/api-explorer/Management/1/overview)| Configure and manage your Adyen company and merchant accounts, stores, and payment terminals. | management | **v1** |
+| [Payments API](https://docs.adyen.com/api-explorer/Payment/68/overview)| Our classic integration for online payments. | payments | **v68** |
+| [Payouts API](https://docs.adyen.com/api-explorer/Payout/68/overview)| Endpoints for sending funds to your customers. | payouts | **v68** |
+| [POS Terminal Management API](https://docs.adyen.com/api-explorer/postfmapi/1/overview)| Endpoints for managing your point-of-sale payment terminals. | terminal | **v1** |
+| [Recurring API](https://docs.adyen.com/api-explorer/Recurring/68/overview)| Endpoints for managing saved payment details. | recurring | **v68** |
 | [Stored Value API](https://docs.adyen.com/payment-methods/gift-cards/stored-value-api) | Endpoints for managing gift cards. | storedValue | **v46** |
 | [Transfers API](https://docs.adyen.com/api-explorer/transfers/3/overview) | Endpoints for managing transfers, getting information about transactions or moving fund | transfers | **v3** |
 
 For more information, refer to our [documentation](https://docs.adyen.com/) or the [API Explorer](https://docs.adyen.com/api-explorer/).
 
 
 
  
  
 ## Prerequisites
  
 -   [Adyen test account](https://docs.adyen.com/get-started-with-adyen)
 -   [API key](https://docs.adyen.com/development-resources/api-credentials#generate-api-key). For testing, your API credential needs to have the [API PCI Payments role](https://docs.adyen.com/development-resources/api-credentials#roles).
-- Python 3.6
+- Python 3.6 or higher
 - Packages (optional): requests or pycurl  
  
 
  ## Installation
 
 ### For development purposes
 
@@ -61,15 +61,14 @@
 import Adyen
 
 adyen = Adyen.Adyen()
 
 adyen.payment.client.xapikey = "YourXapikey"
 adyen.payment.client.hmac = "YourHMACkey"
 adyen.payment.client.platform = "test" # Environment to use the library in.
-adyen.payment.client.merchant_account = "merchant account name from CA"
 ~~~~
 ### Consuming Services
 Every API the library supports is represented by a service object. The name of the service matching the corresponding API is listed in the [Integrations](#supported-api-versions) section of this document.
 #### Using all services
 ~~~~python
 import Adyen
 adyen = Adyen.Adyen()
@@ -157,14 +156,16 @@
 <p>AdyenEndpointInvalidFormat</p>
 </details>
 
 ### Example integration
  
 For a closer look at how our Python library works, clone our [example integration](https://github.com/adyen-examples/adyen-python-online-payments). This includes commented code, highlighting key features and concepts, and examples of API calls that can be made using the library.
 
+## Feedback
+We value your input! Help us enhance our API Libraries and improve the integration experience by providing your feedback. Please take a moment to fill out [our feedback form](https://forms.gle/A4EERrR6CWgKWe5r9) to share your thoughts, suggestions or ideas.
 
 ## Contributing
  
 We encourage you to contribute to this repository, so everyone can benefit from new features, bug fixes, and any other improvements.
  
  
 Have a look at our [contributing guidelines](https://github.com/Adyen/adyen-python-api-library/blob/develop/CONTRIBUTING.md) to find out how to raise a pull request.
```

### Comparing `Adyen-8.0.1/setup.py` & `Adyen-9.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Adyen',
     packages=find_packages(include="Adyen*"),
-    version='8.0.1',
+    version='9.0.0',
     maintainer='Adyen',
     maintainer_email='support@adyen.com',
     description='Adyen Python Api',
     long_description="A Python client library for accessing Adyen APIs",
     author='Adyen',
     author_email='support@adyen.com',
     url='https://github.com/Adyen/adyen-python-api-library',
```

### Comparing `Adyen-8.0.1/test/BaseTest.py` & `Adyen-9.0.0/test/BaseTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/test/BinLookupTest.py` & `Adyen-9.0.0/test/BinLookupTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/test/CheckoutTest.py` & `Adyen-9.0.0/test/CheckoutTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/test/CheckoutUtilityTest.py` & `Adyen-9.0.0/test/CheckoutUtilityTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/test/ConfigurationTest.py` & `Adyen-9.0.0/test/ConfigurationTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/test/DataProtectionTest.py` & `Adyen-9.0.0/test/DataProtectionTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/test/DetermineEndpointTest.py` & `Adyen-9.0.0/test/DetermineEndpointTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/test/LegalEntityManagementTest.py` & `Adyen-9.0.0/test/LegalEntityManagementTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/test/ManagementTest.py` & `Adyen-9.0.0/test/ManagementTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/test/ModificationTest.py` & `Adyen-9.0.0/test/ModificationTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/test/PaymentTest.py` & `Adyen-9.0.0/test/PaymentTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/test/RecurringTest.py` & `Adyen-9.0.0/test/RecurringTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/test/StoredValueTest.py` & `Adyen-9.0.0/test/StoredValueTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/test/TerminalTest.py` & `Adyen-9.0.0/test/TerminalTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/test/ThirdPartyPayoutTest.py` & `Adyen-9.0.0/test/ThirdPartyPayoutTest.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     def test_confirm_success(self):
         request = {
             "merchantAccount": "YourMerchantAccount",
             "originalReference": "YourReference"
         }
         resp = 'test/mocks/payout/confirm-success.json'
         self.adyen.client = self.test.create_client_from_file(200, request, resp)
-        result = self.adyen.payout.reviewing_api.confirm_payout(request)
+        result = self.adyen.payout.reviewing_api.confirm_third_party(request)
         self.adyen.client.http_client.request.assert_called_once_with(
             'POST',
             f'https://pal-test.adyen.com/pal/servlet/Payout/{self.payout_version}/confirmThirdParty',
             headers={'adyen-library-name': 'adyen-python-api-library', 'adyen-library-version': settings.LIB_VERSION},
             json=request,
             username='YourWSUser',
             password='YourWSPassword',
@@ -47,26 +47,26 @@
             "originalReference": ""
         }
         resp = 'test/mocks/payout/confirm-missing-reference.json'
         self.adyen.client = self.test.create_client_from_file(500, request, resp)
         self.assertRaisesRegex(
             Adyen.AdyenAPICommunicationError,
             "AdyenAPICommunicationError:{'status': 500, 'errorCode': '702', 'message': \"Required field 'merchantAccount' is null\", 'errorType': 'validation'}",
-            self.adyen.payout.reviewing_api.confirm_payout,
+            self.adyen.payout.reviewing_api.confirm_third_party,
             request
         )
 
     def test_decline_success(self):
         request = {
             "merchantAccount": "YourMerchantAccount",
             "originalReference": "YourReference"
         }
         resp = 'test/mocks/payout/decline-success.json'
         self.adyen.client = self.test.create_client_from_file(200, request, resp)
-        result = self.adyen.payout.reviewing_api.cancel_payout(request)
+        result = self.adyen.payout.reviewing_api.decline_third_party(request)
         self.adyen.client.http_client.request.assert_called_once_with(
             'POST',
             f'https://pal-test.adyen.com/pal/servlet/Payout/{self.payout_version}/declineThirdParty',
             headers={'adyen-library-name': 'adyen-python-api-library', 'adyen-library-version': settings.LIB_VERSION},
             json=request,
             username='YourWSUser',
             password='YourWSPassword',
@@ -81,15 +81,15 @@
             "originalReference": ""
         }
         resp = 'test/mocks/payout/decline-missing-reference.json'
         self.adyen.client = self.test.create_client_from_file(500, request, resp)
         self.assertRaisesRegex(
             Adyen.AdyenAPICommunicationError,
             "AdyenAPICommunicationError:{'status': 500, 'errorCode': '702', 'message': \"Required field 'merchantAccount' is null\", 'errorType': 'validation'}",
-            self.adyen.payout.reviewing_api.confirm_payout,
+            self.adyen.payout.reviewing_api.confirm_third_party,
             request
         )
 
     def test_store_detail_bank_success(self):
         request = {
             "bank": {
                 "bankName": "AbnAmro",
@@ -105,15 +105,15 @@
                 "contract": "PAYOUT"
             },
             "shopperEmail": "ref@email.com",
             "shopperReference": "ref"
         }
         resp = 'test/mocks/payout/storeDetail-success.json'
         self.adyen.client = self.test.create_client_from_file(200, request, resp)
-        result = self.adyen.payout.initialization_api.store_payout_details(request)
+        result = self.adyen.payout.initialization_api.store_detail(request)
         self.adyen.client.http_client.request.assert_called_once_with(
             'POST',
             f'https://pal-test.adyen.com/pal/servlet/Payout/{self.payout_version}/storeDetail',
             headers={'adyen-library-name': 'adyen-python-api-library', 'adyen-library-version': settings.LIB_VERSION},
             json=request,
             username='YourWSUser',
             password='YourWSPassword'
@@ -135,15 +135,15 @@
             "merchantAccount": "YourMerchantAccount",
             "shopperEmail": "ref@email.com",
             "shopperReference": "ref",
             "selectedRecurringDetailReference": "LATEST"
         }
         resp = 'test/mocks/payout/submit-success.json'
         self.adyen.client = self.test.create_client_from_file(200, request, resp)
-        result = self.adyen.payout.initialization_api.submit_payout(request)
+        result = self.adyen.payout.initialization_api.submit_third_party(request)
         self.adyen.client.http_client.request.assert_called_once_with(
             'POST',
             f'https://pal-test.adyen.com/pal/servlet/Payout/{self.payout_version}/submitThirdParty',
             headers={'adyen-library-name': 'adyen-python-api-library', 'adyen-library-version': settings.LIB_VERSION},
             json=request,
             username='YourWSUser',
             password='YourWSPassword'
@@ -168,15 +168,15 @@
         }
         resp = 'test/mocks/payout/submit-invalid-reference.json'
         self.adyen.client = self.test.create_client_from_file(422, request, resp)
         self.assertRaisesRegex(
             Adyen.AdyenAPIUnprocessableEntity,
             "AdyenAPIUnprocessableEntity:{'status': 422, 'errorCode': '800',"
             " 'message': 'Contract not found', 'errorType': 'validation'}",
-            self.adyen.payout.initialization_api.submit_payout,
+            self.adyen.payout.initialization_api.submit_third_party,
             request
         )
 
     def test_store_detail_and_submit_missing_reference(self):
         request = {
             "amount": {
                 "value": "100000",
@@ -198,15 +198,15 @@
         resp = 'test/mocks/payout/submit-missing-reference.json'
         self.adyen.client = self.test.create_client_from_file(422, request, resp)
 
         self.assertRaisesRegex(
             Adyen.AdyenAPIUnprocessableEntity,
             "AdyenAPIUnprocessableEntity:{'status': 422, 'message': 'Contract not found',"
             " 'errorCode': '800', 'errorType': 'validation'}",
-            self.adyen.payout.initialization_api.store_details_and_submit_payout,
+            self.adyen.payout.initialization_api.store_detail_and_submit_third_party,
             request
         )
 
     def test_store_detail_and_submit_missing_payment(self):
         request = {
             "amount": {
                 "value": "100000",
@@ -222,15 +222,15 @@
         }
         resp = 'test/mocks/payout/storeDetailAndSubmit-missing-payment.json'
         self.adyen.client = self.test.create_client_from_file(422, request, resp)
         self.assertRaisesRegex(
             Adyen.AdyenAPIUnprocessableEntity,
             "AdyenAPIUnprocessableEntity:{'status': 422, 'errorCode': '000',"
             " 'message': 'Please supply paymentDetails', 'errorType': 'validation'}",
-            self.adyen.payout.initialization_api.store_details_and_submit_payout,
+            self.adyen.payout.initialization_api.store_detail_and_submit_third_party,
             request
         )
 
     def test_store_detail_and_submit_invalid_iban(self):
         request = {
             "amount": {
                 "value": "100000",
@@ -251,15 +251,15 @@
         }
         resp = 'test/mocks/payout/storeDetailAndSubmit-invalid-iban.json'
         self.adyen.client = self.test.create_client_from_file(422, request, resp)
         self.assertRaisesRegex(
             Adyen.AdyenAPIUnprocessableEntity,
             "AdyenAPIUnprocessableEntity:{'status': 422, 'errorCode': '161',"
             " 'message': 'Invalid iban', 'errorType': 'validation'}",
-            self.adyen.payout.initialization_api.store_details_and_submit_payout,
+            self.adyen.payout.initialization_api.store_detail_and_submit_third_party,
             request
         )
 
     def test_store_detail_and_submit_card_success(self):
         request = {
             "amount": {
                 "value": "100000",
@@ -278,15 +278,15 @@
                 "expiryYear": "2018",
                 "cvc": "737",
                 "holderName": "John Smith"
             }
         }
         resp = 'test/mocks/payout/storeDetailAndSubmit-card-success.json'
         self.adyen.client = self.test.create_client_from_file(200, request, resp)
-        result = self.adyen.payout.initialization_api.store_details_and_submit_payout(request)
+        result = self.adyen.payout.initialization_api.store_detail_and_submit_third_party(request)
         self.adyen.client.http_client.request.assert_called_once_with(
             'POST',
             f'https://pal-test.adyen.com/pal/servlet/Payout/{self.payout_version}/storeDetailAndSubmitThirdParty',
             headers={'adyen-library-name': 'adyen-python-api-library', 'adyen-library-version': settings.LIB_VERSION},
             json=request,
             username='YourWSUser',
             password='YourWSPassword'
@@ -312,15 +312,15 @@
             },
             "reference": "YourReference",
             "shopperEmail": "ref@email.com",
             "shopperReference": "ref"
         }
         resp = 'test/mocks/payout/storeDetailAndSubmit-bank-success.json'
         self.adyen.client = self.test.create_client_from_file(200, request, resp)
-        result = self.adyen.payout.initialization_api.store_details_and_submit_payout(request)
+        result = self.adyen.payout.initialization_api.store_detail_and_submit_third_party(request)
         self.adyen.client.http_client.request.assert_called_once_with(
             'POST',
             f'https://pal-test.adyen.com/pal/servlet/Payout/{self.payout_version}/storeDetailAndSubmitThirdParty',
             headers={'adyen-library-name': 'adyen-python-api-library', 'adyen-library-version': settings.LIB_VERSION},
             json=request,
             username='YourWSUser',
             password='YourWSPassword'
```

### Comparing `Adyen-8.0.1/test/TransfersTest.py` & `Adyen-9.0.0/test/TransfersTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-8.0.1/test/UtilTest.py` & `Adyen-9.0.0/test/UtilTest.py`

 * *Files identical despite different names*

