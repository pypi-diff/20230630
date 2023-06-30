# Comparing `tmp/fern_moneykit-0.0.6.tar.gz` & `tmp/fern_moneykit-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_moneykit-0.0.6.tar", max compression
+gzip compressed data, was "fern_moneykit-0.0.8.tar", max compression
```

## Comparing `fern_moneykit-0.0.6.tar` & `fern_moneykit-0.0.8.tar`

### file list

```diff
@@ -1,118 +1,118 @@
--rw-r--r--   0        0        0     1593 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/README.md
--rw-r--r--   0        0        0      376 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     5027 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/__init__.py
--rw-r--r--   0        0        0     4045 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/base_client.py
--rw-r--r--   0        0        0      348 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/core/__init__.py
--rw-r--r--   0        0        0      426 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      217 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/environment.py
--rw-r--r--   0        0        0      538 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/errors/__init__.py
--rw-r--r--   0        0        0      248 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/errors/bad_request_error.py
--rw-r--r--   0        0        0      247 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/errors/forbidden_error.py
--rw-r--r--   0        0        0      246 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/errors/not_found_error.py
--rw-r--r--   0        0        0      354 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/errors/too_many_requests_error.py
--rw-r--r--   0        0        0      250 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/errors/unauthorized_error.py
--rw-r--r--   0        0        0      333 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/py.typed
--rw-r--r--   0        0        0      292 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/resources/access_token/__init__.py
--rw-r--r--   0        0        0     8239 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/resources/access_token/client.py
--rw-r--r--   0        0        0       65 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/resources/accounts/__init__.py
--rw-r--r--   0        0        0    15664 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/resources/accounts/client.py
--rw-r--r--   0        0        0       65 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/resources/identity/__init__.py
--rw-r--r--   0        0        0     5467 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/resources/identity/client.py
--rw-r--r--   0        0        0       65 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/resources/institutions/__init__.py
--rw-r--r--   0        0        0     7584 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/resources/institutions/client.py
--rw-r--r--   0        0        0       65 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/resources/link_session/__init__.py
--rw-r--r--   0        0        0     9149 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/resources/link_session/client.py
--rw-r--r--   0        0        0       65 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/resources/links/__init__.py
--rw-r--r--   0        0        0    15095 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/resources/links/client.py
--rw-r--r--   0        0        0       65 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/resources/products/__init__.py
--rw-r--r--   0        0        0     5258 2023-06-16 00:02:13.856112 fern_moneykit-0.0.6/src/moneykit/resources/products/client.py
--rw-r--r--   0        0        0       65 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/resources/transactions/__init__.py
--rw-r--r--   0        0        0    14542 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/resources/transactions/client.py
--rw-r--r--   0        0        0     6819 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/__init__.py
--rw-r--r--   0        0        0     2708 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/account.py
--rw-r--r--   0        0        0     2223 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/account_balances.py
--rw-r--r--   0        0        0      964 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/account_group.py
--rw-r--r--   0        0        0     2854 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/account_identity.py
--rw-r--r--   0        0        0     1327 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/account_numbers.py
--rw-r--r--   0        0        0     1204 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/account_numbers_link_product.py
--rw-r--r--   0        0        0     1187 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/account_numbers_product_settings.py
--rw-r--r--   0        0        0     2154 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/account_type.py
--rw-r--r--   0        0        0     2872 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/account_with_account_numbers.py
--rw-r--r--   0        0        0     1078 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/accounts_link_product.py
--rw-r--r--   0        0        0      996 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/ach_number.py
--rw-r--r--   0        0        0     1380 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/address.py
--rw-r--r--   0        0        0     1015 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/api_error_auth_expired_access_token_response.py
--rw-r--r--   0        0        0      984 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/api_error_auth_unauthorized_response.py
--rw-r--r--   0        0        0     1004 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/api_error_rate_limit_exceeded_response.py
--rw-r--r--   0        0        0      880 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/bacs_number.py
--rw-r--r--   0        0        0     1328 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/basic_account_details.py
--rw-r--r--   0        0        0     1432 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/body_generate_access_token_auth_token_post.py
--rw-r--r--   0        0        0      560 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/country.py
--rw-r--r--   0        0        0      855 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/create_link_session_response.py
--rw-r--r--   0        0        0    21806 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/currency.py
--rw-r--r--   0        0        0      851 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/cursor_pagination.py
--rw-r--r--   0        0        0      934 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/customer_app.py
--rw-r--r--   0        0        0      975 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/eft_number.py
--rw-r--r--   0        0        0      973 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/email.py
--rw-r--r--   0        0        0      953 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/exchange_token_response.py
--rw-r--r--   0        0        0     1058 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/generate_access_token_response.py
--rw-r--r--   0        0        0      923 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/get_account_numbers_response.py
--rw-r--r--   0        0        0      923 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/get_account_response.py
--rw-r--r--   0        0        0      994 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/get_accounts_response.py
--rw-r--r--   0        0        0     1037 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/get_institutions_response.py
--rw-r--r--   0        0        0     1480 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/get_transactions_response.py
--rw-r--r--   0        0        0     1000 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/get_user_accounts_response.py
--rw-r--r--   0        0        0      956 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/get_user_links_response.py
--rw-r--r--   0        0        0     1222 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/get_user_transactions_response.py
--rw-r--r--   0        0        0     1094 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/http_validation_error.py
--rw-r--r--   0        0        0     1179 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/identity_link_product.py
--rw-r--r--   0        0        0     1181 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/identity_product_settings.py
--rw-r--r--   0        0        0      977 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/identity_response.py
--rw-r--r--   0        0        0     1950 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/institution.py
--rw-r--r--   0        0        0      951 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/institution_error_not_found_response.py
--rw-r--r--   0        0        0      857 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/international_number.py
--rw-r--r--   0        0        0     1358 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/introspect_client_response.py
--rw-r--r--   0        0        0      877 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/jwk_set.py
--rw-r--r--   0        0        0     2109 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/link_common.py
--rw-r--r--   0        0        0      978 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/link_error_bad_state_response.py
--rw-r--r--   0        0        0      978 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/link_error_deleted_response.py
--rw-r--r--   0        0        0      984 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/link_error_forbidden_action_response.py
--rw-r--r--   0        0        0      937 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/link_error_not_found_response.py
--rw-r--r--   0        0        0      957 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/link_error_unauthorized_access_response.py
--rw-r--r--   0        0        0      985 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/link_permission_scope.py
--rw-r--r--   0        0        0      850 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/link_permissions.py
--rw-r--r--   0        0        0     1198 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/link_products.py
--rw-r--r--   0        0        0     2544 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/link_response.py
--rw-r--r--   0        0        0     1784 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/link_session_customer_user.py
--rw-r--r--   0        0        0     1364 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/link_session_customer_user_email.py
--rw-r--r--   0        0        0     1744 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/link_session_customer_user_phone.py
--rw-r--r--   0        0        0      999 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/link_session_error_forbidden_config_response.py
--rw-r--r--   0        0        0     1002 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/link_session_error_invalid_token_exchange.py
--rw-r--r--   0        0        0     1972 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/link_session_setting_overrides.py
--rw-r--r--   0        0        0     1262 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/link_state_changed_webhook.py
--rw-r--r--   0        0        0     1104 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/money_link_features.py
--rw-r--r--   0        0        0     1347 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/owner.py
--rw-r--r--   0        0        0     1103 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/phone_number.py
--rw-r--r--   0        0        0      792 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/phone_number_type.py
--rw-r--r--   0        0        0      895 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/product.py
--rw-r--r--   0        0        0     1132 2023-06-16 00:02:13.860112 fern_moneykit-0.0.6/src/moneykit/types/products_settings.py
--rw-r--r--   0        0        0      910 2023-06-16 00:02:13.868112 fern_moneykit-0.0.6/src/moneykit/types/provider.py
--rw-r--r--   0        0        0     1292 2023-06-16 00:02:13.868112 fern_moneykit-0.0.6/src/moneykit/types/public_link_error.py
--rw-r--r--   0        0        0     1077 2023-06-16 00:02:13.868112 fern_moneykit-0.0.6/src/moneykit/types/public_link_state.py
--rw-r--r--   0        0        0     1689 2023-06-16 00:02:13.868112 fern_moneykit-0.0.6/src/moneykit/types/requested_link_permission.py
--rw-r--r--   0        0        0       88 2023-06-16 00:02:13.868112 fern_moneykit-0.0.6/src/moneykit/types/supported_version.py
--rw-r--r--   0        0        0     3097 2023-06-16 00:02:13.868112 fern_moneykit-0.0.6/src/moneykit/types/transaction.py
--rw-r--r--   0        0        0     1298 2023-06-16 00:02:13.868112 fern_moneykit-0.0.6/src/moneykit/types/transaction_diff.py
--rw-r--r--   0        0        0     1499 2023-06-16 00:02:13.868112 fern_moneykit-0.0.6/src/moneykit/types/transaction_sync_response.py
--rw-r--r--   0        0        0      501 2023-06-16 00:02:13.868112 fern_moneykit-0.0.6/src/moneykit/types/transaction_type.py
--rw-r--r--   0        0        0      519 2023-06-16 00:02:13.868112 fern_moneykit-0.0.6/src/moneykit/types/transaction_type_filter.py
--rw-r--r--   0        0        0     1195 2023-06-16 00:02:13.868112 fern_moneykit-0.0.6/src/moneykit/types/transactions_link_product.py
--rw-r--r--   0        0        0     1525 2023-06-16 00:02:13.868112 fern_moneykit-0.0.6/src/moneykit/types/transactions_product_settings.py
--rw-r--r--   0        0        0      893 2023-06-16 00:02:13.868112 fern_moneykit-0.0.6/src/moneykit/types/validation_error.py
--rw-r--r--   0        0        0      133 2023-06-16 00:02:13.868112 fern_moneykit-0.0.6/src/moneykit/types/validation_error_location_item.py
--rw-r--r--   0        0        0     2103 1970-01-01 00:00:00.000000 fern_moneykit-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     3261 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/README.md
+-rw-r--r--   0        0        0      376 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     5027 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/__init__.py
+-rw-r--r--   0        0        0     4045 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/client.py
+-rw-r--r--   0        0        0      348 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      217 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/environment.py
+-rw-r--r--   0        0        0      538 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/errors/__init__.py
+-rw-r--r--   0        0        0      248 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/errors/bad_request_error.py
+-rw-r--r--   0        0        0      247 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/errors/forbidden_error.py
+-rw-r--r--   0        0        0      246 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/errors/not_found_error.py
+-rw-r--r--   0        0        0      354 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/errors/too_many_requests_error.py
+-rw-r--r--   0        0        0      250 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      333 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/py.typed
+-rw-r--r--   0        0        0      292 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/resources/access_token/__init__.py
+-rw-r--r--   0        0        0     8239 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/resources/access_token/client.py
+-rw-r--r--   0        0        0       65 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/resources/accounts/__init__.py
+-rw-r--r--   0        0        0    15664 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/resources/accounts/client.py
+-rw-r--r--   0        0        0       65 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/resources/identity/__init__.py
+-rw-r--r--   0        0        0     5467 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/resources/identity/client.py
+-rw-r--r--   0        0        0       65 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/resources/institutions/__init__.py
+-rw-r--r--   0        0        0     7584 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/resources/institutions/client.py
+-rw-r--r--   0        0        0       65 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/resources/link_session/__init__.py
+-rw-r--r--   0        0        0     9149 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/resources/link_session/client.py
+-rw-r--r--   0        0        0       65 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/resources/links/__init__.py
+-rw-r--r--   0        0        0    15095 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/resources/links/client.py
+-rw-r--r--   0        0        0       65 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/resources/products/__init__.py
+-rw-r--r--   0        0        0     5258 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/resources/products/client.py
+-rw-r--r--   0        0        0       65 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/resources/transactions/__init__.py
+-rw-r--r--   0        0        0    14542 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/resources/transactions/client.py
+-rw-r--r--   0        0        0     6819 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/__init__.py
+-rw-r--r--   0        0        0     2708 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/account.py
+-rw-r--r--   0        0        0     2223 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/account_balances.py
+-rw-r--r--   0        0        0      964 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/account_group.py
+-rw-r--r--   0        0        0     2854 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/account_identity.py
+-rw-r--r--   0        0        0     1327 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/account_numbers.py
+-rw-r--r--   0        0        0     1204 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/account_numbers_link_product.py
+-rw-r--r--   0        0        0     1187 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/account_numbers_product_settings.py
+-rw-r--r--   0        0        0     2154 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/account_type.py
+-rw-r--r--   0        0        0     2872 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/account_with_account_numbers.py
+-rw-r--r--   0        0        0     1078 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/accounts_link_product.py
+-rw-r--r--   0        0        0      996 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/ach_number.py
+-rw-r--r--   0        0        0     1380 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/address.py
+-rw-r--r--   0        0        0     1015 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/api_error_auth_expired_access_token_response.py
+-rw-r--r--   0        0        0      984 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/api_error_auth_unauthorized_response.py
+-rw-r--r--   0        0        0     1004 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/api_error_rate_limit_exceeded_response.py
+-rw-r--r--   0        0        0      880 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/bacs_number.py
+-rw-r--r--   0        0        0     1328 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/basic_account_details.py
+-rw-r--r--   0        0        0     1432 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/body_generate_access_token_auth_token_post.py
+-rw-r--r--   0        0        0      560 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/country.py
+-rw-r--r--   0        0        0      855 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/create_link_session_response.py
+-rw-r--r--   0        0        0    21806 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/currency.py
+-rw-r--r--   0        0        0      851 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/cursor_pagination.py
+-rw-r--r--   0        0        0      934 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/customer_app.py
+-rw-r--r--   0        0        0      975 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/eft_number.py
+-rw-r--r--   0        0        0      973 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/email.py
+-rw-r--r--   0        0        0      953 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/exchange_token_response.py
+-rw-r--r--   0        0        0     1058 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/generate_access_token_response.py
+-rw-r--r--   0        0        0      923 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/get_account_numbers_response.py
+-rw-r--r--   0        0        0      923 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/get_account_response.py
+-rw-r--r--   0        0        0      994 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/get_accounts_response.py
+-rw-r--r--   0        0        0     1037 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/get_institutions_response.py
+-rw-r--r--   0        0        0     1480 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/get_transactions_response.py
+-rw-r--r--   0        0        0     1000 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/get_user_accounts_response.py
+-rw-r--r--   0        0        0      956 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/get_user_links_response.py
+-rw-r--r--   0        0        0     1222 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/get_user_transactions_response.py
+-rw-r--r--   0        0        0     1094 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/http_validation_error.py
+-rw-r--r--   0        0        0     1179 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/identity_link_product.py
+-rw-r--r--   0        0        0     1181 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/identity_product_settings.py
+-rw-r--r--   0        0        0      977 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/identity_response.py
+-rw-r--r--   0        0        0     1950 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/institution.py
+-rw-r--r--   0        0        0      951 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/institution_error_not_found_response.py
+-rw-r--r--   0        0        0      857 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/international_number.py
+-rw-r--r--   0        0        0     1358 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/introspect_client_response.py
+-rw-r--r--   0        0        0      877 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/jwk_set.py
+-rw-r--r--   0        0        0     2109 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/link_common.py
+-rw-r--r--   0        0        0      978 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/link_error_bad_state_response.py
+-rw-r--r--   0        0        0      978 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/link_error_deleted_response.py
+-rw-r--r--   0        0        0      984 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/link_error_forbidden_action_response.py
+-rw-r--r--   0        0        0      937 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/link_error_not_found_response.py
+-rw-r--r--   0        0        0      957 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/link_error_unauthorized_access_response.py
+-rw-r--r--   0        0        0      985 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/link_permission_scope.py
+-rw-r--r--   0        0        0      850 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/link_permissions.py
+-rw-r--r--   0        0        0     1198 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/link_products.py
+-rw-r--r--   0        0        0     2544 2023-06-16 00:43:23.314083 fern_moneykit-0.0.8/src/moneykit/types/link_response.py
+-rw-r--r--   0        0        0     1784 2023-06-16 00:43:23.318083 fern_moneykit-0.0.8/src/moneykit/types/link_session_customer_user.py
+-rw-r--r--   0        0        0     1364 2023-06-16 00:43:23.318083 fern_moneykit-0.0.8/src/moneykit/types/link_session_customer_user_email.py
+-rw-r--r--   0        0        0     1744 2023-06-16 00:43:23.318083 fern_moneykit-0.0.8/src/moneykit/types/link_session_customer_user_phone.py
+-rw-r--r--   0        0        0      999 2023-06-16 00:43:23.318083 fern_moneykit-0.0.8/src/moneykit/types/link_session_error_forbidden_config_response.py
+-rw-r--r--   0        0        0     1002 2023-06-16 00:43:23.318083 fern_moneykit-0.0.8/src/moneykit/types/link_session_error_invalid_token_exchange.py
+-rw-r--r--   0        0        0     1972 2023-06-16 00:43:23.318083 fern_moneykit-0.0.8/src/moneykit/types/link_session_setting_overrides.py
+-rw-r--r--   0        0        0     1262 2023-06-16 00:43:23.318083 fern_moneykit-0.0.8/src/moneykit/types/link_state_changed_webhook.py
+-rw-r--r--   0        0        0     1104 2023-06-16 00:43:23.318083 fern_moneykit-0.0.8/src/moneykit/types/money_link_features.py
+-rw-r--r--   0        0        0     1347 2023-06-16 00:43:23.318083 fern_moneykit-0.0.8/src/moneykit/types/owner.py
+-rw-r--r--   0        0        0     1103 2023-06-16 00:43:23.318083 fern_moneykit-0.0.8/src/moneykit/types/phone_number.py
+-rw-r--r--   0        0        0      792 2023-06-16 00:43:23.318083 fern_moneykit-0.0.8/src/moneykit/types/phone_number_type.py
+-rw-r--r--   0        0        0      895 2023-06-16 00:43:23.318083 fern_moneykit-0.0.8/src/moneykit/types/product.py
+-rw-r--r--   0        0        0     1132 2023-06-16 00:43:23.318083 fern_moneykit-0.0.8/src/moneykit/types/products_settings.py
+-rw-r--r--   0        0        0      910 2023-06-16 00:43:23.318083 fern_moneykit-0.0.8/src/moneykit/types/provider.py
+-rw-r--r--   0        0        0     1292 2023-06-16 00:43:23.318083 fern_moneykit-0.0.8/src/moneykit/types/public_link_error.py
+-rw-r--r--   0        0        0     1077 2023-06-16 00:43:23.318083 fern_moneykit-0.0.8/src/moneykit/types/public_link_state.py
+-rw-r--r--   0        0        0     1689 2023-06-16 00:43:23.318083 fern_moneykit-0.0.8/src/moneykit/types/requested_link_permission.py
+-rw-r--r--   0        0        0       88 2023-06-16 00:43:23.318083 fern_moneykit-0.0.8/src/moneykit/types/supported_version.py
+-rw-r--r--   0        0        0     3097 2023-06-16 00:43:23.318083 fern_moneykit-0.0.8/src/moneykit/types/transaction.py
+-rw-r--r--   0        0        0     1298 2023-06-16 00:43:23.318083 fern_moneykit-0.0.8/src/moneykit/types/transaction_diff.py
+-rw-r--r--   0        0        0     1499 2023-06-16 00:43:23.318083 fern_moneykit-0.0.8/src/moneykit/types/transaction_sync_response.py
+-rw-r--r--   0        0        0      501 2023-06-16 00:43:23.318083 fern_moneykit-0.0.8/src/moneykit/types/transaction_type.py
+-rw-r--r--   0        0        0      519 2023-06-16 00:43:23.318083 fern_moneykit-0.0.8/src/moneykit/types/transaction_type_filter.py
+-rw-r--r--   0        0        0     1195 2023-06-16 00:43:23.318083 fern_moneykit-0.0.8/src/moneykit/types/transactions_link_product.py
+-rw-r--r--   0        0        0     1525 2023-06-16 00:43:23.318083 fern_moneykit-0.0.8/src/moneykit/types/transactions_product_settings.py
+-rw-r--r--   0        0        0      893 2023-06-16 00:43:23.318083 fern_moneykit-0.0.8/src/moneykit/types/validation_error.py
+-rw-r--r--   0        0        0      133 2023-06-16 00:43:23.318083 fern_moneykit-0.0.8/src/moneykit/types/validation_error_location_item.py
+-rw-r--r--   0        0        0     3771 1970-01-01 00:00:00.000000 fern_moneykit-0.0.8/PKG-INFO
```

### Comparing `fern_moneykit-0.0.6/src/moneykit/__init__.py` & `fern_moneykit-0.0.8/src/moneykit/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/base_client.py` & `fern_moneykit-0.0.8/src/moneykit/client.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/core/datetime_utils.py` & `fern_moneykit-0.0.8/src/moneykit/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/core/jsonable_encoder.py` & `fern_moneykit-0.0.8/src/moneykit/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/errors/__init__.py` & `fern_moneykit-0.0.8/src/moneykit/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/resources/access_token/client.py` & `fern_moneykit-0.0.8/src/moneykit/resources/access_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/resources/accounts/client.py` & `fern_moneykit-0.0.8/src/moneykit/resources/accounts/client.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/resources/identity/client.py` & `fern_moneykit-0.0.8/src/moneykit/resources/identity/client.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/resources/institutions/client.py` & `fern_moneykit-0.0.8/src/moneykit/resources/institutions/client.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/resources/link_session/client.py` & `fern_moneykit-0.0.8/src/moneykit/resources/link_session/client.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/resources/links/client.py` & `fern_moneykit-0.0.8/src/moneykit/resources/links/client.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/resources/products/client.py` & `fern_moneykit-0.0.8/src/moneykit/resources/products/client.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/resources/transactions/client.py` & `fern_moneykit-0.0.8/src/moneykit/resources/transactions/client.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/__init__.py` & `fern_moneykit-0.0.8/src/moneykit/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/account.py` & `fern_moneykit-0.0.8/src/moneykit/types/account.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/account_balances.py` & `fern_moneykit-0.0.8/src/moneykit/types/account_balances.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/account_group.py` & `fern_moneykit-0.0.8/src/moneykit/types/account_group.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/account_identity.py` & `fern_moneykit-0.0.8/src/moneykit/types/account_identity.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/account_numbers.py` & `fern_moneykit-0.0.8/src/moneykit/types/account_numbers.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/account_numbers_link_product.py` & `fern_moneykit-0.0.8/src/moneykit/types/account_numbers_link_product.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/account_numbers_product_settings.py` & `fern_moneykit-0.0.8/src/moneykit/types/account_numbers_product_settings.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/account_type.py` & `fern_moneykit-0.0.8/src/moneykit/types/account_type.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/account_with_account_numbers.py` & `fern_moneykit-0.0.8/src/moneykit/types/account_with_account_numbers.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/accounts_link_product.py` & `fern_moneykit-0.0.8/src/moneykit/types/accounts_link_product.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/ach_number.py` & `fern_moneykit-0.0.8/src/moneykit/types/ach_number.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/address.py` & `fern_moneykit-0.0.8/src/moneykit/types/address.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/api_error_auth_expired_access_token_response.py` & `fern_moneykit-0.0.8/src/moneykit/types/api_error_auth_expired_access_token_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/api_error_auth_unauthorized_response.py` & `fern_moneykit-0.0.8/src/moneykit/types/api_error_auth_unauthorized_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/api_error_rate_limit_exceeded_response.py` & `fern_moneykit-0.0.8/src/moneykit/types/api_error_rate_limit_exceeded_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/bacs_number.py` & `fern_moneykit-0.0.8/src/moneykit/types/bacs_number.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/basic_account_details.py` & `fern_moneykit-0.0.8/src/moneykit/types/basic_account_details.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/body_generate_access_token_auth_token_post.py` & `fern_moneykit-0.0.8/src/moneykit/types/body_generate_access_token_auth_token_post.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/country.py` & `fern_moneykit-0.0.8/src/moneykit/types/country.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/create_link_session_response.py` & `fern_moneykit-0.0.8/src/moneykit/types/create_link_session_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/currency.py` & `fern_moneykit-0.0.8/src/moneykit/types/currency.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/cursor_pagination.py` & `fern_moneykit-0.0.8/src/moneykit/types/cursor_pagination.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/customer_app.py` & `fern_moneykit-0.0.8/src/moneykit/types/customer_app.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/eft_number.py` & `fern_moneykit-0.0.8/src/moneykit/types/eft_number.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/email.py` & `fern_moneykit-0.0.8/src/moneykit/types/email.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/exchange_token_response.py` & `fern_moneykit-0.0.8/src/moneykit/types/exchange_token_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/generate_access_token_response.py` & `fern_moneykit-0.0.8/src/moneykit/types/generate_access_token_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/get_account_numbers_response.py` & `fern_moneykit-0.0.8/src/moneykit/types/get_account_numbers_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/get_account_response.py` & `fern_moneykit-0.0.8/src/moneykit/types/get_account_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/get_accounts_response.py` & `fern_moneykit-0.0.8/src/moneykit/types/get_accounts_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/get_institutions_response.py` & `fern_moneykit-0.0.8/src/moneykit/types/get_institutions_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/get_transactions_response.py` & `fern_moneykit-0.0.8/src/moneykit/types/get_transactions_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/get_user_accounts_response.py` & `fern_moneykit-0.0.8/src/moneykit/types/get_user_accounts_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/get_user_links_response.py` & `fern_moneykit-0.0.8/src/moneykit/types/get_user_links_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/get_user_transactions_response.py` & `fern_moneykit-0.0.8/src/moneykit/types/get_user_transactions_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/http_validation_error.py` & `fern_moneykit-0.0.8/src/moneykit/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/identity_link_product.py` & `fern_moneykit-0.0.8/src/moneykit/types/identity_link_product.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/identity_product_settings.py` & `fern_moneykit-0.0.8/src/moneykit/types/identity_product_settings.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/identity_response.py` & `fern_moneykit-0.0.8/src/moneykit/types/identity_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/institution.py` & `fern_moneykit-0.0.8/src/moneykit/types/institution.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/institution_error_not_found_response.py` & `fern_moneykit-0.0.8/src/moneykit/types/institution_error_not_found_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/international_number.py` & `fern_moneykit-0.0.8/src/moneykit/types/international_number.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/introspect_client_response.py` & `fern_moneykit-0.0.8/src/moneykit/types/introspect_client_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/jwk_set.py` & `fern_moneykit-0.0.8/src/moneykit/types/jwk_set.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/link_common.py` & `fern_moneykit-0.0.8/src/moneykit/types/link_common.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/link_error_bad_state_response.py` & `fern_moneykit-0.0.8/src/moneykit/types/link_error_bad_state_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/link_error_deleted_response.py` & `fern_moneykit-0.0.8/src/moneykit/types/link_error_deleted_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/link_error_forbidden_action_response.py` & `fern_moneykit-0.0.8/src/moneykit/types/link_error_forbidden_action_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/link_error_not_found_response.py` & `fern_moneykit-0.0.8/src/moneykit/types/link_error_not_found_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/link_error_unauthorized_access_response.py` & `fern_moneykit-0.0.8/src/moneykit/types/link_error_unauthorized_access_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/link_permission_scope.py` & `fern_moneykit-0.0.8/src/moneykit/types/link_permission_scope.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/link_permissions.py` & `fern_moneykit-0.0.8/src/moneykit/types/link_permissions.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/link_products.py` & `fern_moneykit-0.0.8/src/moneykit/types/link_products.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/link_response.py` & `fern_moneykit-0.0.8/src/moneykit/types/link_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/link_session_customer_user.py` & `fern_moneykit-0.0.8/src/moneykit/types/link_session_customer_user.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/link_session_customer_user_email.py` & `fern_moneykit-0.0.8/src/moneykit/types/link_session_customer_user_email.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/link_session_customer_user_phone.py` & `fern_moneykit-0.0.8/src/moneykit/types/link_session_customer_user_phone.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/link_session_error_forbidden_config_response.py` & `fern_moneykit-0.0.8/src/moneykit/types/link_session_error_forbidden_config_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/link_session_error_invalid_token_exchange.py` & `fern_moneykit-0.0.8/src/moneykit/types/link_session_error_invalid_token_exchange.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/link_session_setting_overrides.py` & `fern_moneykit-0.0.8/src/moneykit/types/link_session_setting_overrides.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/link_state_changed_webhook.py` & `fern_moneykit-0.0.8/src/moneykit/types/link_state_changed_webhook.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/money_link_features.py` & `fern_moneykit-0.0.8/src/moneykit/types/money_link_features.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/owner.py` & `fern_moneykit-0.0.8/src/moneykit/types/owner.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/phone_number.py` & `fern_moneykit-0.0.8/src/moneykit/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/phone_number_type.py` & `fern_moneykit-0.0.8/src/moneykit/types/phone_number_type.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/product.py` & `fern_moneykit-0.0.8/src/moneykit/types/product.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/products_settings.py` & `fern_moneykit-0.0.8/src/moneykit/types/products_settings.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/provider.py` & `fern_moneykit-0.0.8/src/moneykit/types/provider.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/public_link_error.py` & `fern_moneykit-0.0.8/src/moneykit/types/public_link_error.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/public_link_state.py` & `fern_moneykit-0.0.8/src/moneykit/types/public_link_state.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/requested_link_permission.py` & `fern_moneykit-0.0.8/src/moneykit/types/requested_link_permission.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/transaction.py` & `fern_moneykit-0.0.8/src/moneykit/types/transaction.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/transaction_diff.py` & `fern_moneykit-0.0.8/src/moneykit/types/transaction_diff.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/transaction_sync_response.py` & `fern_moneykit-0.0.8/src/moneykit/types/transaction_sync_response.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/transaction_type_filter.py` & `fern_moneykit-0.0.8/src/moneykit/types/transaction_type_filter.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/transactions_link_product.py` & `fern_moneykit-0.0.8/src/moneykit/types/transactions_link_product.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/transactions_product_settings.py` & `fern_moneykit-0.0.8/src/moneykit/types/transactions_product_settings.py`

 * *Files identical despite different names*

### Comparing `fern_moneykit-0.0.6/src/moneykit/types/validation_error.py` & `fern_moneykit-0.0.8/src/moneykit/types/validation_error.py`

 * *Files identical despite different names*

